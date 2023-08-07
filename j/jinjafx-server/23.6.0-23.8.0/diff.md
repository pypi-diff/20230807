# Comparing `tmp/jinjafx_server-23.6.0.tar.gz` & `tmp/jinjafx_server-23.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinjafx_server-23.6.0.tar", last modified: Tue Jun  6 02:54:37 2023, max compression
+gzip compressed data, was "jinjafx_server-23.8.0.tar", last modified: Mon Aug  7 14:16:58 2023, max compression
```

## Comparing `jinjafx_server-23.6.0.tar` & `jinjafx_server-23.8.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:54:37.359567 jinjafx_server-23.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-06 02:54:33.000000 jinjafx_server-23.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10219 2023-06-06 02:54:37.359567 jinjafx_server-23.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-06-06 02:54:33.000000 jinjafx_server-23.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:54:37.359567 jinjafx_server-23.6.0/jinjafx_server/
--rwxr-xr-x   0 runner    (1001) docker     (123)    38849 2023-06-06 02:54:33.000000 jinjafx_server-23.6.0/jinjafx_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:54:37.359567 jinjafx_server-23.6.0/jinjafx_server/www/
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-06 02:54:33.000000 jinjafx_server-23.6.0/jinjafx_server/www/dt.html
--rw-r--r--   0 runner    (1001) docker     (123)    26749 2023-06-06 02:54:33.000000 jinjafx_server-23.6.0/jinjafx_server/www/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-06 02:54:33.000000 jinjafx_server-23.6.0/jinjafx_server/www/jinjafx.css
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-06 02:54:33.000000 jinjafx_server-23.6.0/jinjafx_server/www/jinjafx.png
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-06 02:54:33.000000 jinjafx_server-23.6.0/jinjafx_server/www/jinjafx_dt.js
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-06 02:54:33.000000 jinjafx_server-23.6.0/jinjafx_server/www/jinjafx_m.css
--rw-r--r--   0 runner    (1001) docker     (123)    62749 2023-06-06 02:54:33.000000 jinjafx_server-23.6.0/jinjafx_server/www/jinjafx_m.js
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-06 02:54:33.000000 jinjafx_server-23.6.0/jinjafx_server/www/jinjafx_o.css
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-06-06 02:54:33.000000 jinjafx_server-23.6.0/jinjafx_server/www/jinjafx_o.js
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-06 02:54:33.000000 jinjafx_server-23.6.0/jinjafx_server/www/obsolete.html
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-06 02:54:33.000000 jinjafx_server-23.6.0/jinjafx_server/www/obsolete.js
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-06-06 02:54:33.000000 jinjafx_server-23.6.0/jinjafx_server/www/output.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:54:37.359567 jinjafx_server-23.6.0/jinjafx_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10219 2023-06-06 02:54:37.000000 jinjafx_server-23.6.0/jinjafx_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-06 02:54:37.000000 jinjafx_server-23.6.0/jinjafx_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 02:54:37.000000 jinjafx_server-23.6.0/jinjafx_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-06 02:54:37.000000 jinjafx_server-23.6.0/jinjafx_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-06 02:54:37.000000 jinjafx_server-23.6.0/jinjafx_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-06 02:54:37.000000 jinjafx_server-23.6.0/jinjafx_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-06 02:54:33.000000 jinjafx_server-23.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 02:54:37.359567 jinjafx_server-23.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-06 02:54:33.000000 jinjafx_server-23.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:58.851555 jinjafx_server-23.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-07 14:16:55.000000 jinjafx_server-23.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10219 2023-08-07 14:16:58.851555 jinjafx_server-23.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-08-07 14:16:55.000000 jinjafx_server-23.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:58.851555 jinjafx_server-23.8.0/jinjafx_server/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38849 2023-08-07 14:16:55.000000 jinjafx_server-23.8.0/jinjafx_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:58.851555 jinjafx_server-23.8.0/jinjafx_server/www/
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-07 14:16:55.000000 jinjafx_server-23.8.0/jinjafx_server/www/dt.html
+-rw-r--r--   0 runner    (1001) docker     (123)    26749 2023-08-07 14:16:55.000000 jinjafx_server-23.8.0/jinjafx_server/www/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-08-07 14:16:55.000000 jinjafx_server-23.8.0/jinjafx_server/www/jinjafx.css
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-07 14:16:55.000000 jinjafx_server-23.8.0/jinjafx_server/www/jinjafx.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-08-07 14:16:55.000000 jinjafx_server-23.8.0/jinjafx_server/www/jinjafx_dt.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-08-07 14:16:55.000000 jinjafx_server-23.8.0/jinjafx_server/www/jinjafx_m.css
+-rw-r--r--   0 runner    (1001) docker     (123)    62749 2023-08-07 14:16:55.000000 jinjafx_server-23.8.0/jinjafx_server/www/jinjafx_m.js
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-08-07 14:16:55.000000 jinjafx_server-23.8.0/jinjafx_server/www/jinjafx_o.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-08-07 14:16:55.000000 jinjafx_server-23.8.0/jinjafx_server/www/jinjafx_o.js
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-07 14:16:55.000000 jinjafx_server-23.8.0/jinjafx_server/www/obsolete.html
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-07 14:16:55.000000 jinjafx_server-23.8.0/jinjafx_server/www/obsolete.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-08-07 14:16:55.000000 jinjafx_server-23.8.0/jinjafx_server/www/output.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:16:58.851555 jinjafx_server-23.8.0/jinjafx_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10219 2023-08-07 14:16:58.000000 jinjafx_server-23.8.0/jinjafx_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-07 14:16:58.000000 jinjafx_server-23.8.0/jinjafx_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 14:16:58.000000 jinjafx_server-23.8.0/jinjafx_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-07 14:16:58.000000 jinjafx_server-23.8.0/jinjafx_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-07 14:16:58.000000 jinjafx_server-23.8.0/jinjafx_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-07 14:16:58.000000 jinjafx_server-23.8.0/jinjafx_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-07 14:16:55.000000 jinjafx_server-23.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 14:16:58.851555 jinjafx_server-23.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-07 14:16:55.000000 jinjafx_server-23.8.0/setup.py
```

### Comparing `jinjafx_server-23.6.0/LICENSE` & `jinjafx_server-23.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jinjafx_server-23.6.0/PKG-INFO` & `jinjafx_server-23.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinjafx_server
-Version: 23.6.0
+Version: 23.8.0
 Summary: JinjaFx Server - Jinja2 Templating Tool
 Home-page: https://github.com/cmason3/jinjafx_server
 Author: Chris Mason
 Author-email: chris@netnix.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jinjafx_server-23.6.0/README.md` & `jinjafx_server-23.8.0/README.md`

 * *Files identical despite different names*

### Comparing `jinjafx_server-23.6.0/jinjafx_server/__init__.py` & `jinjafx_server-23.8.0/jinjafx_server/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from http.server import HTTPServer, BaseHTTPRequestHandler
 from jinja2 import __version__ as jinja2_version
 import jinjafx, os, io, sys, socket, signal, threading, yaml, json, base64, time, datetime, resource
 import re, argparse, hashlib, traceback, glob, hmac, uuid, struct, binascii, gzip, requests, ctypes
 import cmarkgfm, emoji
 
-__version__ = '23.6.0'
+__version__ = '23.8.0'
 
 lock = threading.RLock()
 base = os.path.abspath(os.path.dirname(__file__))
 
 aws_s3_url = None
 aws_access_key = None
 aws_secret_key = None
```

### Comparing `jinjafx_server-23.6.0/jinjafx_server/www/dt.html` & `jinjafx_server-23.8.0/jinjafx_server/www/dt.html`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <html lang="en">
   <head>
     <meta charset="utf-8">
     <meta http-equiv="Content-Security-Policy" content="default-src 'self'; style-src 'self' https://cdnjs.cloudflare.com 'unsafe-inline'">
     <meta name="viewport" content="width=1536, user-scalable=no">
     <title>JinjaFx DataTemplate</title>
     <link rel="shortcut icon" href="/874f2915/jinjafx.png">
-    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.0/css/bootstrap.min.css" integrity="sha512-t4GWSVZO1eC8BM339Xd7Uphw5s17a86tIZIj8qRxhnKub6WoyhnrxeCIMeAqBPgdZGlCcG2PrZjMc+Wr78+5Xg==" crossorigin="anonymous" referrerpolicy="no-referrer">
+    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.1/css/bootstrap.min.css" integrity="sha512-Z/def5z5u2aR89OuzYcxmDJ0Bnd5V1cKqBEbvLOiUNWdg9PQeXVvXLI90SE4QOHGlfLqUnDNVAYyZi8UwUTmWQ==" crossorigin="anonymous" referrerpolicy="no-referrer">
     <link rel="stylesheet" href="/f8555653/jinjafx.css">
     <script src="/00abd23c/jinjafx_dt.js"></script>
   </head>
   <body>
     <div id="wrap" class="p-2 bg-transparent">
       <button id="saveas" class="btn btn-secondary text-white float-end me-3 mt-3 d-none" type="button" title="Save DataTemplate As">
         <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
```

### Comparing `jinjafx_server-23.6.0/jinjafx_server/www/index.html` & `jinjafx_server-23.8.0/jinjafx_server/www/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -4,39 +4,39 @@
     <meta charset="utf-8">
     <meta http-equiv="Content-Security-Policy" content="default-src 'self'; style-src 'self' https://cdnjs.cloudflare.com 'unsafe-inline'; script-src 'self' https://cdnjs.cloudflare.com; img-src 'self' data:">
     <meta name="viewport" content="width=1536, user-scalable=no">
     <meta name="description" content="JinjaFx is a Python based Jinja2 Templating Tool with support for Ansible filters that renders output based on CSV or YAML datasets">
     <title>JinjaFx - Jinja2 Templating Tool</title>
     <script src="/6d052dbe/obsolete.js"></script>
     <link rel="shortcut icon" href="/874f2915/jinjafx.png">
-    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.0/css/bootstrap.min.css" integrity="sha512-t4GWSVZO1eC8BM339Xd7Uphw5s17a86tIZIj8qRxhnKub6WoyhnrxeCIMeAqBPgdZGlCcG2PrZjMc+Wr78+5Xg==" crossorigin="anonymous" referrerpolicy="no-referrer">
-    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.13/codemirror.min.css" integrity="sha512-uf06llspW44/LZpHzHT6qBOIVODjWtv4MxCricRxkzvopAlSWnTf6hpZTFxuuZcuNE9CBQhqE0Seu1CoRk84nQ==" crossorigin="anonymous" referrerpolicy="no-referrer">
-    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.13/addon/dialog/dialog.min.css" integrity="sha512-Vogm+Cii1SXP5oxWQyPdkA91rHB776209ZVvX4C/i4ypcfBlWVRXZGodoTDAyyZvO36JlTqDqkMhVKAYc7CMjQ==" crossorigin="anonymous" referrerpolicy="no-referrer">
-    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.13/addon/display/fullscreen.min.css" integrity="sha512-T8xB3MmwpA77VK9lUH3UkdUTnkmpqOxHF8OceOKaHrvpcXMSNX0xtpa9FoLTDAVO1JnB2UiMdVeI2V0HTHjTWA==" crossorigin="anonymous" referrerpolicy="no-referrer">
-    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.13/addon/fold/foldgutter.min.css" integrity="sha512-YwkMTlTHn8dBnwa47IF+cKsS00HPiiVhQ4DpwT1KF2gUftfFR7aefepabSPLAs6zrMyD89M3w0Ow6mQ5XJEUCw==" crossorigin="anonymous" referrerpolicy="no-referrer">
+    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.1/css/bootstrap.min.css" integrity="sha512-Z/def5z5u2aR89OuzYcxmDJ0Bnd5V1cKqBEbvLOiUNWdg9PQeXVvXLI90SE4QOHGlfLqUnDNVAYyZi8UwUTmWQ==" crossorigin="anonymous" referrerpolicy="no-referrer">
+    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.14/codemirror.min.css" integrity="sha512-uf06llspW44/LZpHzHT6qBOIVODjWtv4MxCricRxkzvopAlSWnTf6hpZTFxuuZcuNE9CBQhqE0Seu1CoRk84nQ==" crossorigin="anonymous" referrerpolicy="no-referrer">
+    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.14/addon/dialog/dialog.min.css" integrity="sha512-Vogm+Cii1SXP5oxWQyPdkA91rHB776209ZVvX4C/i4ypcfBlWVRXZGodoTDAyyZvO36JlTqDqkMhVKAYc7CMjQ==" crossorigin="anonymous" referrerpolicy="no-referrer">
+    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.14/addon/display/fullscreen.min.css" integrity="sha512-T8xB3MmwpA77VK9lUH3UkdUTnkmpqOxHF8OceOKaHrvpcXMSNX0xtpa9FoLTDAVO1JnB2UiMdVeI2V0HTHjTWA==" crossorigin="anonymous" referrerpolicy="no-referrer">
+    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.14/addon/fold/foldgutter.min.css" integrity="sha512-YwkMTlTHn8dBnwa47IF+cKsS00HPiiVhQ4DpwT1KF2gUftfFR7aefepabSPLAs6zrMyD89M3w0Ow6mQ5XJEUCw==" crossorigin="anonymous" referrerpolicy="no-referrer">
     <link rel="stylesheet" href="/f8555653/jinjafx.css">
     <link rel="stylesheet" href="/af18a9f8/jinjafx_m.css">
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.0/js/bootstrap.bundle.min.js" integrity="sha512-VK2zcvntEufaimc+efOYi622VN5ZacdnufnmX7zIhCPmjhKnOi9ZDMtg1/ug5l183f19gG1/cBstPO4D8N/Img==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.13/codemirror.min.js" integrity="sha512-sSWQXoxIkE0G4/xqLngx5C53oOZCgFRxWE79CvMX2X0IKx14W3j9Dpz/2MpRh58xb2W/h+Y4WAHJQA0qMMuxJg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.13/addon/selection/mark-selection.min.js" integrity="sha512-XaS0JPIY5yDTDaYIMjkoXz+LF/DEVhRn1eq9QOhJPhMuJGGPOKZTulF+LY8/uwd18k00CIaSe4f8fCyp/5U7IQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.13/addon/dialog/dialog.min.js" integrity="sha512-NAJeqwfpM7/nfX90EweQhjudb66diK3Y9mkBjb4xJ6wufuVqFVAjHd8mJW//CGHNR9cI8wUfDRJ0jtLzZ9v8Qg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.13/addon/display/fullscreen.min.js" integrity="sha512-8Rk4wB3MfgQfuOw95XW/vAU8PSTHWI5HddVRXfg+Ykk8CzsiOZkDpxVSrnYq2u/IqO499ooZ61fFHppuzB2ghA==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.13/addon/search/search.min.js" integrity="sha512-Mw3RqCUHTyvN3iSp5TSs731TiLqnKrxzyy2UVZv3+tJa524Rj7pBC7Ivv3ka2oDnkQwLOMHNDKU5nMJ16YRgrA==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.13/addon/search/searchcursor.min.js" integrity="sha512-+ZfZDC9gi1y9Xoxi9UUsSp+5k+AcFE0TRNjI0pfaAHQ7VZTaaoEpBZp9q9OvHdSomOze/7s5w27rcsYpT6xU6g==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.13/addon/edit/trailingspace.min.js" integrity="sha512-xcccdc2hhCFOxhdb8nh6lTpOS7gNTw36W/TIaDoNfydtLhxbebAqiqhY8zty5K5V57/Pgpb9wD27fH1UHYk8yQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.13/addon/fold/foldcode.min.js" integrity="sha512-Q2qfEJEU257Qlqc4/5g6iKuJNnn5L0xu2D48p8WHe9YC/kLj2UfkdGD01qfxWk+XIcHsZngcA8WuKcizF8MAHA==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.13/addon/fold/foldgutter.min.js" integrity="sha512-TRBGROluEM9UrFPnoCk0vW2PqqcMUyGJETe60qzktKTEiXmPhmxqJLYqOf7TsX4ulMbANjdpLY+DYk0aoht4gA==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.13/addon/mode/overlay.min.js" integrity="sha512-SNwKDMYQwymOPjleeZy1xbdlK1PAjJ6EAplvx0CvNFJbW/pF5ec3h0mAdDl1yySq9r3Qont4STM4W3le7FTm9w==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.13/mode/jinja2/jinja2.min.js" integrity="sha512-Z4le1RxwhD8lDCrspbBxjTLLP2HGC1+mKb9KHR2N/sEx8uOe2vre5XQo8YMPAz8FQTo43HjefjlDtjY4LtfaaQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.13/mode/yaml/yaml.min.js" integrity="sha512-+aXDZ93WyextRiAZpsRuJyiAZ38ztttUyO/H3FZx4gOAOv4/k9C6Um1CvHVtaowHZ2h7kH0d+orWvdBLPVwb4g==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.1/js/bootstrap.bundle.min.js" integrity="sha512-ToL6UYWePxjhDQKNioSi4AyJ5KkRxY+F1+Fi7Jgh0Hp5Kk2/s8FD7zusJDdonfe5B00Qw+B8taXxF6CFLnqNCw==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.14/codemirror.min.js" integrity="sha512-t5Lcu24FbQybGnoIbv1GXDx633tW0Hd4reBUx74EIq/2Q39FzskADNbjc605pQA9kkojC+8bRXhHKEXoKJs3rw==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.14/addon/selection/mark-selection.min.js" integrity="sha512-XaS0JPIY5yDTDaYIMjkoXz+LF/DEVhRn1eq9QOhJPhMuJGGPOKZTulF+LY8/uwd18k00CIaSe4f8fCyp/5U7IQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.14/addon/dialog/dialog.min.js" integrity="sha512-wORgIxiT2jtk5rkEfkQekASddOaXrblQLaFU0ls+KdpzJuy6RCjh/7DVv1haiIVQ88kae4hoWqj6BmXf7n9G5Q==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.14/addon/display/fullscreen.min.js" integrity="sha512-6ity42PCu271POvuw3xu4Y7TwreX7PB0ALWt3O51MYgeHIB3QYYvxMTFu8xMyle547HtpMa3HLjIZ3ACpficTw==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.14/addon/search/search.min.js" integrity="sha512-nVG8Yf3YjbBC5bjc8P0Vg/NLsWuShgNVMHbGanq/u4js7d71GVld/u2JKKU9MOk+nDRZV4Pl6PuGb93a4Oyt0w==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.14/addon/search/searchcursor.min.js" integrity="sha512-NvqB4zhyjudFSZLywSPayM4MO3/OS1zyCD/qSAlCaEuhXxo0SWIiTGqXl/eUvmMEABvsloZfQ8G8qbhv4E7OLA==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.14/addon/edit/trailingspace.min.js" integrity="sha512-xcccdc2hhCFOxhdb8nh6lTpOS7gNTw36W/TIaDoNfydtLhxbebAqiqhY8zty5K5V57/Pgpb9wD27fH1UHYk8yQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.14/addon/fold/foldcode.min.js" integrity="sha512-9pu1V/0h+OfpTNLbCZnMalfd2Iinys+euBVsq0Jghp1U5KJAkTYx1OIyEsrtyhuR/SI5k91k4+VUHDAGd5TMEQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.14/addon/fold/foldgutter.min.js" integrity="sha512-VloKQ3escS4gyLRZoLPu3n5NwRp019gN3bxgriGmyWeICdMpUOV/jINpE+Zt3GJiRmyBrKNZtcNlmJrffPY/ig==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.14/addon/mode/overlay.min.js" integrity="sha512-SNwKDMYQwymOPjleeZy1xbdlK1PAjJ6EAplvx0CvNFJbW/pF5ec3h0mAdDl1yySq9r3Qont4STM4W3le7FTm9w==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.14/mode/jinja2/jinja2.min.js" integrity="sha512-Z4le1RxwhD8lDCrspbBxjTLLP2HGC1+mKb9KHR2N/sEx8uOe2vre5XQo8YMPAz8FQTo43HjefjlDtjY4LtfaaQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.65.14/mode/yaml/yaml.min.js" integrity="sha512-+aXDZ93WyextRiAZpsRuJyiAZ38ztttUyO/H3FZx4gOAOv4/k9C6Um1CvHVtaowHZ2h7kH0d+orWvdBLPVwb4g==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/pako/2.1.0/pako_deflate.min.js" integrity="sha512-oEsmlMj4bUaKNfYtsxV2eZm+5L0I/JhLsXftLFKeywkgAq8QMLKRlZrMIkMC2AHZQ/gT8YtI+fP1WUwNjF1PoQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/split.js/1.6.5/split.min.js" integrity="sha512-lNjb0qWDVvt1zfSiXufaxtlFtenve3BLbvljxuMXuSr0DE0HYp5OhX0u89uwNd6MvlX1bgJ8ulfG4JMGurs8UA==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/js-yaml/4.1.0/js-yaml.min.js" integrity="sha512-CSBhVREyzHAjAFfBlIBakjoRUKp5h7VSweP0InR/pAJyptH7peuhCsqAI/snV+TwZmXZqoUklpXp6R6wMnYf5Q==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/dayjs/1.11.8/dayjs.min.js" integrity="sha512-af90l7+r/ujCury3kqomcoZ4aNuC4JP0xUUU682bqlRCLLvGJrc9L82zONFccLWmxcMXSqO9d6C7Rr39EkbT3Q==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/dayjs/1.11.8/plugin/relativeTime.min.js" integrity="sha512-MVzDPmm7QZ8PhEiqJXKz/zw2HJuv61waxb8XXuZMMs9b+an3LoqOqhOEt5Nq3LY1e4Ipbbd/e+AWgERdHlVgaA==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/dayjs/1.11.9/dayjs.min.js" integrity="sha512-q4Xn+ZU2K+dqJPL8a3TiyGsDa31IkR/rLt/w+fy8jLrx8TdXj0dLM1Aq4aPXnOOKxHEya/bD9DePDB2DHm4jJQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/dayjs/1.11.9/plugin/relativeTime.min.js" integrity="sha512-6RygaIDPDX6ddRU7XCHt5mE3D1z+cwvGk1OilDc91XVgqgBhgw5UgtQFZdlPSzC5IyeSKMQPzvtW+7+YFWb0TQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src="/2e3bfd58/jinjafx_m.js"></script>
   </head>
   <body>
     <div id="overlay"></div>
     <div id="wrap">
       <h1 class="d-none">JinjaFx - Jinja2 Templating Tool</h1>
       <div id="header" class="p-3">
```

### Comparing `jinjafx_server-23.6.0/jinjafx_server/www/jinjafx.css` & `jinjafx_server-23.8.0/jinjafx_server/www/jinjafx.css`

 * *Files identical despite different names*

### Comparing `jinjafx_server-23.6.0/jinjafx_server/www/jinjafx_dt.js` & `jinjafx_server-23.8.0/jinjafx_server/www/jinjafx_dt.js`

 * *Files identical despite different names*

### Comparing `jinjafx_server-23.6.0/jinjafx_server/www/jinjafx_m.css` & `jinjafx_server-23.8.0/jinjafx_server/www/jinjafx_m.css`

 * *Files identical despite different names*

### Comparing `jinjafx_server-23.6.0/jinjafx_server/www/jinjafx_m.js` & `jinjafx_server-23.8.0/jinjafx_server/www/jinjafx_m.js`

 * *Files identical despite different names*

### Comparing `jinjafx_server-23.6.0/jinjafx_server/www/jinjafx_o.css` & `jinjafx_server-23.8.0/jinjafx_server/www/jinjafx_o.css`

 * *Files identical despite different names*

### Comparing `jinjafx_server-23.6.0/jinjafx_server/www/jinjafx_o.js` & `jinjafx_server-23.8.0/jinjafx_server/www/jinjafx_o.js`

 * *Files identical despite different names*

### Comparing `jinjafx_server-23.6.0/jinjafx_server/www/output.html` & `jinjafx_server-23.8.0/jinjafx_server/www/output.html`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 <html lang="en">
   <head>
     <meta charset="utf-8">
     <meta http-equiv="Content-Security-Policy" content="default-src 'self'; style-src 'self' https://cdnjs.cloudflare.com 'unsafe-inline'; script-src 'self' https://cdnjs.cloudflare.com">
     <meta name="viewport" content="width=1536, user-scalable=no">
     <title>Generating...</title>
     <link rel="shortcut icon" href="/874f2915/jinjafx.png">
-    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.0/css/bootstrap.min.css" integrity="sha512-t4GWSVZO1eC8BM339Xd7Uphw5s17a86tIZIj8qRxhnKub6WoyhnrxeCIMeAqBPgdZGlCcG2PrZjMc+Wr78+5Xg==" crossorigin="anonymous" referrerpolicy="no-referrer">
+    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.1/css/bootstrap.min.css" integrity="sha512-Z/def5z5u2aR89OuzYcxmDJ0Bnd5V1cKqBEbvLOiUNWdg9PQeXVvXLI90SE4QOHGlfLqUnDNVAYyZi8UwUTmWQ==" crossorigin="anonymous" referrerpolicy="no-referrer">
     <link rel="stylesheet" href="/f8555653/jinjafx.css">
     <link rel="stylesheet" href="/e6166066/jinjafx_o.css">
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.0/js/bootstrap.bundle.min.js" integrity="sha512-VK2zcvntEufaimc+efOYi622VN5ZacdnufnmX7zIhCPmjhKnOi9ZDMtg1/ug5l183f19gG1/cBstPO4D8N/Img==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.1/js/bootstrap.bundle.min.js" integrity="sha512-ToL6UYWePxjhDQKNioSi4AyJ5KkRxY+F1+Fi7Jgh0Hp5Kk2/s8FD7zusJDdonfe5B00Qw+B8taXxF6CFLnqNCw==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/pako/2.1.0/pako_deflate.min.js" integrity="sha512-oEsmlMj4bUaKNfYtsxV2eZm+5L0I/JhLsXftLFKeywkgAq8QMLKRlZrMIkMC2AHZQ/gT8YtI+fP1WUwNjF1PoQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/dayjs/1.11.8/dayjs.min.js" integrity="sha512-af90l7+r/ujCury3kqomcoZ4aNuC4JP0xUUU682bqlRCLLvGJrc9L82zONFccLWmxcMXSqO9d6C7Rr39EkbT3Q==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/dayjs/1.11.8/plugin/advancedFormat.min.js" integrity="sha512-oOF6H/+bcZjL9xEZ71lPxWSLn62axEgf6jDBuge0rTy7HjcMmWLQ7Y46WVC0m1hGibeYyTeHLi1ZUrZTvt2QxQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/dayjs/1.11.9/dayjs.min.js" integrity="sha512-q4Xn+ZU2K+dqJPL8a3TiyGsDa31IkR/rLt/w+fy8jLrx8TdXj0dLM1Aq4aPXnOOKxHEya/bD9DePDB2DHm4jJQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/dayjs/1.11.9/plugin/advancedFormat.min.js" integrity="sha512-YT+XPOQl0M9AI8pIt/whGB4wmrpV6La6Q7i283l8zIP/syIqyt5uc8PTDqj3BskO9vHHHLym6Zjzmb29xGmtlw==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/jszip/3.10.1/jszip.min.js" integrity="sha512-XMVd28F1oH/O71fzwBnV7HucLxVwtxf26XV8P4wPk26EDxuGZ91N8bsOttmnomcCD3CS5ZMRL50H0GgOHvegtg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
     <script src="/6b770078/jinjafx_o.js"></script>
   </head>
   <body>
     <div id="status" class="alert alert-primary wait fw-bold">Generating Output...</div>
     <div id="wrap" class="d-none">
       <div id="header" class="p-3">
```

### Comparing `jinjafx_server-23.6.0/jinjafx_server.egg-info/PKG-INFO` & `jinjafx_server-23.8.0/jinjafx_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinjafx-server
-Version: 23.6.0
+Version: 23.8.0
 Summary: JinjaFx Server - Jinja2 Templating Tool
 Home-page: https://github.com/cmason3/jinjafx_server
 Author: Chris Mason
 Author-email: chris@netnix.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jinjafx_server-23.6.0/jinjafx_server.egg-info/SOURCES.txt` & `jinjafx_server-23.8.0/jinjafx_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jinjafx_server-23.6.0/setup.py` & `jinjafx_server-23.8.0/setup.py`

 * *Files identical despite different names*

