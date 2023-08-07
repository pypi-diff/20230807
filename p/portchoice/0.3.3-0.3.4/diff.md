# Comparing `tmp/portchoice-0.3.3.tar.gz` & `tmp/portchoice-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portchoice-0.3.3.tar", max compression
+gzip compressed data, was "portchoice-0.3.4.tar", max compression
```

## Comparing `portchoice-0.3.3.tar` & `portchoice-0.3.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       22 2023-08-04 14:46:35.283731 portchoice-0.3.3/portchoice/__init__.py
--rw-r--r--   0        0        0    14724 2023-08-04 14:46:35.283911 portchoice-0.3.3/portchoice/design.py
--rw-r--r--   0        0        0     4735 2023-08-04 14:46:35.284050 portchoice-0.3.3/portchoice/generate.py
--rw-r--r--   0        0        0    45456 2023-08-05 15:05:05.301162 portchoice-0.3.3/portchoice/models.py
--rw-r--r--   0        0        0     6537 2023-08-04 14:46:35.284511 portchoice-0.3.3/portchoice/utils.py
--rw-r--r--   0        0        0      454 2023-08-04 14:58:44.247382 portchoice-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      709 2023-08-05 15:32:50.423727 portchoice-0.3.3/setup.py
--rw-r--r--   0        0        0      535 2023-08-05 15:32:50.424466 portchoice-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-08-04 14:46:35.283731 portchoice-0.3.4/portchoice/__init__.py
+-rw-r--r--   0        0        0    14724 2023-08-04 14:46:35.283911 portchoice-0.3.4/portchoice/design.py
+-rw-r--r--   0        0        0     4735 2023-08-04 14:46:35.284050 portchoice-0.3.4/portchoice/generate.py
+-rw-r--r--   0        0        0    45581 2023-08-07 16:27:22.847663 portchoice-0.3.4/portchoice/models.py
+-rw-r--r--   0        0        0     6537 2023-08-04 14:46:35.284511 portchoice-0.3.4/portchoice/utils.py
+-rw-r--r--   0        0        0      454 2023-08-07 16:27:41.168267 portchoice-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      709 2023-08-07 16:28:24.147707 portchoice-0.3.4/setup.py
+-rw-r--r--   0        0        0      535 2023-08-07 16:28:24.148161 portchoice-0.3.4/PKG-INFO
```

### Comparing `portchoice-0.3.3/portchoice/design.py` & `portchoice-0.3.4/portchoice/design.py`

 * *Files identical despite different names*

### Comparing `portchoice-0.3.3/portchoice/generate.py` & `portchoice-0.3.4/portchoice/generate.py`

 * *Files identical despite different names*

### Comparing `portchoice-0.3.3/portchoice/models.py` & `portchoice-0.3.4/portchoice/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1085,14 +1085,18 @@
             if delta_0 is None:
                 delta_0 = pars[par_count]
                 par_count += 1
 
             # Construct individual utility functions
             Vj = delta_j + Xb + Zt
 
+            # If dimension of Vp is 1, then add new axis
+            if Vj.ndim == 1:
+                Vj = Vj[np.newaxis,:]
+
             # Construct utility functions of the portfolios
             Vp = Vj @ combinations.T
 
             if interactions is not None:
                 for s in range(len(interactions)):
                     syn = ' & '.join(['(combinations[:,' + str(ss) + ']==1)' for ss in interactions[s]])
                     Vp = Vp + eval(syn)*delta_ij[s]
```

### Comparing `portchoice-0.3.3/portchoice/utils.py` & `portchoice-0.3.4/portchoice/utils.py`

 * *Files identical despite different names*

### Comparing `portchoice-0.3.3/setup.py` & `portchoice-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numdifftools>=0.9.40,<0.10.0', 'pandas>=1.4.2,<2.0.0', 'pyDOE2>=1.3.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'portchoice',
-    'version': '0.3.3',
+    'version': '0.3.4',
     'description': 'Modules to design and estimate portfolio choice models',
     'long_description': None,
     'author': 'Jose Ignacio Hernandez',
     'author_email': 'j.i.hernandez@tudelft.nl',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `portchoice-0.3.3/PKG-INFO` & `portchoice-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portchoice
-Version: 0.3.3
+Version: 0.3.4
 Summary: Modules to design and estimate portfolio choice models
 Author: Jose Ignacio Hernandez
 Author-email: j.i.hernandez@tudelft.nl
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
```

