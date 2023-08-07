# Comparing `tmp/amalitech-subsys-june-0.9.8.tar.gz` & `tmp/amalitech-subsys-june-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amalitech-subsys-june-0.9.8.tar", last modified: Tue Aug  1 11:13:02 2023, max compression
+gzip compressed data, was "amalitech-subsys-june-0.9.9.tar", last modified: Tue Aug  1 11:13:37 2023, max compression
```

## Comparing `amalitech-subsys-june-0.9.8.tar` & `amalitech-subsys-june-0.9.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:13:02.786278 amalitech-subsys-june-0.9.8/
--rw-r--r--   0 root         (0) root         (0)     1075 2023-08-01 11:12:47.000000 amalitech-subsys-june-0.9.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      443 2023-08-01 11:13:02.782277 amalitech-subsys-june-0.9.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1527 2023-08-01 11:12:47.000000 amalitech-subsys-june-0.9.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:13:02.782277 amalitech-subsys-june-0.9.8/amalitech_subsys_june.egg-info/
--rw-r--r--   0 root         (0) root         (0)      443 2023-08-01 11:13:02.000000 amalitech-subsys-june-0.9.8/amalitech_subsys_june.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      559 2023-08-01 11:13:02.000000 amalitech-subsys-june-0.9.8/amalitech_subsys_june.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 11:13:02.000000 amalitech-subsys-june-0.9.8/amalitech_subsys_june.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-08-01 11:13:02.000000 amalitech-subsys-june-0.9.8/amalitech_subsys_june.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-08-01 11:13:02.000000 amalitech-subsys-june-0.9.8/amalitech_subsys_june.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-08-01 11:13:02.000000 amalitech-subsys-june-0.9.8/amalitech_subsys_june.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:13:02.782277 amalitech-subsys-june-0.9.8/app/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 11:12:47.000000 amalitech-subsys-june-0.9.8/app/__init__.py
--rw-r--r--   0 root         (0) root         (0)      314 2023-08-01 11:12:47.000000 amalitech-subsys-june-0.9.8/app/subsys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:13:02.782277 amalitech-subsys-june-0.9.8/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 11:12:47.000000 amalitech-subsys-june-0.9.8/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1219 2023-08-01 11:12:47.000000 amalitech-subsys-june-0.9.8/commands/config.py
--rw-r--r--   0 root         (0) root         (0)      316 2023-08-01 11:12:47.000000 amalitech-subsys-june-0.9.8/commands/init.py
--rw-r--r--   0 root         (0) root         (0)      999 2023-08-01 11:12:47.000000 amalitech-subsys-june-0.9.8/commands/snap.py
--rw-r--r--   0 root         (0) root         (0)     1427 2023-08-01 11:12:47.000000 amalitech-subsys-june-0.9.8/commands/submit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:13:02.782277 amalitech-subsys-june-0.9.8/services/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 11:12:47.000000 amalitech-subsys-june-0.9.8/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1384 2023-08-01 11:12:47.000000 amalitech-subsys-june-0.9.8/services/auth.py
--rw-r--r--   0 root         (0) root         (0)     2348 2023-08-01 11:12:47.000000 amalitech-subsys-june-0.9.8/services/submit.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 11:13:02.786278 amalitech-subsys-june-0.9.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      676 2023-08-01 11:13:02.000000 amalitech-subsys-june-0.9.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:13:02.782277 amalitech-subsys-june-0.9.8/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 11:12:47.000000 amalitech-subsys-june-0.9.8/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3348 2023-08-01 11:12:47.000000 amalitech-subsys-june-0.9.8/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)      982 2023-08-01 11:12:47.000000 amalitech-subsys-june-0.9.8/utils/repository.py
--rw-r--r--   0 root         (0) root         (0)     6876 2023-08-01 11:12:47.000000 amalitech-subsys-june-0.9.8/utils/snap.py
--rw-r--r--   0 root         (0) root         (0)     4842 2023-08-01 11:12:47.000000 amalitech-subsys-june-0.9.8/utils/stage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:13:37.286436 amalitech-subsys-june-0.9.9/
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-08-01 11:13:22.000000 amalitech-subsys-june-0.9.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      443 2023-08-01 11:13:37.286436 amalitech-subsys-june-0.9.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-08-01 11:13:22.000000 amalitech-subsys-june-0.9.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:13:37.286436 amalitech-subsys-june-0.9.9/amalitech_subsys_june.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      443 2023-08-01 11:13:37.000000 amalitech-subsys-june-0.9.9/amalitech_subsys_june.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      559 2023-08-01 11:13:37.000000 amalitech-subsys-june-0.9.9/amalitech_subsys_june.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 11:13:37.000000 amalitech-subsys-june-0.9.9/amalitech_subsys_june.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-08-01 11:13:37.000000 amalitech-subsys-june-0.9.9/amalitech_subsys_june.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-08-01 11:13:37.000000 amalitech-subsys-june-0.9.9/amalitech_subsys_june.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-08-01 11:13:37.000000 amalitech-subsys-june-0.9.9/amalitech_subsys_june.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:13:37.286436 amalitech-subsys-june-0.9.9/app/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 11:13:22.000000 amalitech-subsys-june-0.9.9/app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      314 2023-08-01 11:13:22.000000 amalitech-subsys-june-0.9.9/app/subsys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:13:37.286436 amalitech-subsys-june-0.9.9/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 11:13:22.000000 amalitech-subsys-june-0.9.9/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-08-01 11:13:22.000000 amalitech-subsys-june-0.9.9/commands/config.py
+-rw-r--r--   0 root         (0) root         (0)      316 2023-08-01 11:13:22.000000 amalitech-subsys-june-0.9.9/commands/init.py
+-rw-r--r--   0 root         (0) root         (0)      999 2023-08-01 11:13:22.000000 amalitech-subsys-june-0.9.9/commands/snap.py
+-rw-r--r--   0 root         (0) root         (0)     1427 2023-08-01 11:13:22.000000 amalitech-subsys-june-0.9.9/commands/submit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:13:37.286436 amalitech-subsys-june-0.9.9/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 11:13:22.000000 amalitech-subsys-june-0.9.9/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1384 2023-08-01 11:13:22.000000 amalitech-subsys-june-0.9.9/services/auth.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2023-08-01 11:13:22.000000 amalitech-subsys-june-0.9.9/services/submit.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 11:13:37.286436 amalitech-subsys-june-0.9.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      676 2023-08-01 11:13:36.000000 amalitech-subsys-june-0.9.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 11:13:37.286436 amalitech-subsys-june-0.9.9/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 11:13:22.000000 amalitech-subsys-june-0.9.9/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3348 2023-08-01 11:13:22.000000 amalitech-subsys-june-0.9.9/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)      982 2023-08-01 11:13:22.000000 amalitech-subsys-june-0.9.9/utils/repository.py
+-rw-r--r--   0 root         (0) root         (0)     6876 2023-08-01 11:13:22.000000 amalitech-subsys-june-0.9.9/utils/snap.py
+-rw-r--r--   0 root         (0) root         (0)     4842 2023-08-01 11:13:22.000000 amalitech-subsys-june-0.9.9/utils/stage.py
```

### Comparing `amalitech-subsys-june-0.9.8/LICENSE` & `amalitech-subsys-june-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `amalitech-subsys-june-0.9.8/README.md` & `amalitech-subsys-june-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `amalitech-subsys-june-0.9.8/amalitech_subsys_june.egg-info/SOURCES.txt` & `amalitech-subsys-june-0.9.9/amalitech_subsys_june.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amalitech-subsys-june-0.9.8/commands/config.py` & `amalitech-subsys-june-0.9.9/commands/config.py`

 * *Files identical despite different names*

### Comparing `amalitech-subsys-june-0.9.8/commands/snap.py` & `amalitech-subsys-june-0.9.9/commands/snap.py`

 * *Files identical despite different names*

### Comparing `amalitech-subsys-june-0.9.8/commands/submit.py` & `amalitech-subsys-june-0.9.9/commands/submit.py`

 * *Files identical despite different names*

### Comparing `amalitech-subsys-june-0.9.8/services/auth.py` & `amalitech-subsys-june-0.9.9/services/auth.py`

 * *Files identical despite different names*

### Comparing `amalitech-subsys-june-0.9.8/services/submit.py` & `amalitech-subsys-june-0.9.9/services/submit.py`

 * *Files identical despite different names*

### Comparing `amalitech-subsys-june-0.9.8/setup.py` & `amalitech-subsys-june-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="amalitech-subsys-june",
-    version="0.9.8",
+    version="0.9.9",
     packages=find_packages(),
     entry_points={"console_scripts": ["subsys = app.subsys:cli"]},
     install_requires=["click", "requests", "tqdm", "python-slugify"],
     author="Charles Biney, Eric Kodzi, Donal-Miles Gyasi",
     author_email="charles.biney@amalitech.org, eric.kodzi@amalitech.org, donal-miles.gyasi@amalitech.org",
     description="A git inspired assignment submission system.",
     classifiers=[
```

### Comparing `amalitech-subsys-june-0.9.8/utils/misc.py` & `amalitech-subsys-june-0.9.9/utils/misc.py`

 * *Files identical despite different names*

### Comparing `amalitech-subsys-june-0.9.8/utils/repository.py` & `amalitech-subsys-june-0.9.9/utils/repository.py`

 * *Files identical despite different names*

### Comparing `amalitech-subsys-june-0.9.8/utils/snap.py` & `amalitech-subsys-june-0.9.9/utils/snap.py`

 * *Files identical despite different names*

### Comparing `amalitech-subsys-june-0.9.8/utils/stage.py` & `amalitech-subsys-june-0.9.9/utils/stage.py`

 * *Files identical despite different names*

