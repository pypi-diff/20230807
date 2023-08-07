# Comparing `tmp/sscred_fork-0.2.17.tar.gz` & `tmp/sscred_fork-0.2.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sscred_fork-0.2.17.tar", last modified: Mon Aug  7 16:10:43 2023, max compression
+gzip compressed data, was "dist/sscred_fork-0.2.18.tar", last modified: Mon Aug  7 16:12:14 2023, max compression
```

## Comparing `sscred_fork-0.2.17.tar` & `sscred_fork-0.2.18.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-07 16:10:43.000000 sscred_fork-0.2.17/
--rw-r--r--   0 benjaminK   (501) staff       (20)     1537 2023-06-29 18:39:09.000000 sscred_fork-0.2.17/LICENSE
--rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-08-07 16:10:43.000000 sscred_fork-0.2.17/PKG-INFO
--rw-r--r--   0 benjaminK   (501) staff       (20)     8328 2023-06-29 18:39:09.000000 sscred_fork-0.2.17/README.md
--rw-r--r--   0 benjaminK   (501) staff       (20)      878 2023-08-07 16:10:43.000000 sscred_fork-0.2.17/setup.cfg
--rw-r--r--   0 benjaminK   (501) staff       (20)     1583 2023-07-05 10:12:24.000000 sscred_fork-0.2.17/setup.py
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-07 16:10:43.000000 sscred_fork-0.2.17/sscred/
--rw-r--r--   0 benjaminK   (501) staff       (20)      503 2023-08-07 16:10:11.000000 sscred_fork-0.2.17/sscred/__init__.py
--rw-r--r--   0 benjaminK   (501) staff       (20)    15082 2023-08-06 18:49:31.000000 sscred_fork-0.2.17/sscred/acl.py
--rw-r--r--   0 benjaminK   (501) staff       (20)    12797 2023-08-06 18:51:14.000000 sscred_fork-0.2.17/sscred/blind_pedersen.py
--rw-r--r--   0 benjaminK   (501) staff       (20)    16436 2023-06-29 18:39:09.000000 sscred_fork-0.2.17/sscred/blind_signature.py
--rw-r--r--   0 benjaminK   (501) staff       (20)     7560 2023-08-07 16:08:29.000000 sscred_fork-0.2.17/sscred/commitment.py
--rw-r--r--   0 benjaminK   (501) staff       (20)       31 2023-06-29 18:39:09.000000 sscred_fork-0.2.17/sscred/config.py
--rw-r--r--   0 benjaminK   (501) staff       (20)     6722 2023-07-07 14:29:32.000000 sscred_fork-0.2.17/sscred/pack.py
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-07 16:10:43.000000 sscred_fork-0.2.17/sscred_fork.egg-info/
--rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-08-07 16:10:43.000000 sscred_fork-0.2.17/sscred_fork.egg-info/PKG-INFO
--rw-r--r--   0 benjaminK   (501) staff       (20)      367 2023-08-07 16:10:43.000000 sscred_fork-0.2.17/sscred_fork.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminK   (501) staff       (20)        1 2023-08-07 16:10:43.000000 sscred_fork-0.2.17/sscred_fork.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminK   (501) staff       (20)       43 2023-08-07 16:10:43.000000 sscred_fork-0.2.17/sscred_fork.egg-info/requires.txt
--rw-r--r--   0 benjaminK   (501) staff       (20)        7 2023-08-07 16:10:43.000000 sscred_fork-0.2.17/sscred_fork.egg-info/top_level.txt
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-07 16:10:43.000000 sscred_fork-0.2.17/test/
--rw-r--r--   0 benjaminK   (501) staff       (20)    11039 2023-06-29 18:39:09.000000 sscred_fork-0.2.17/test/test_sscred.py
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-07 16:12:14.000000 sscred_fork-0.2.18/
+-rw-r--r--   0 benjaminK   (501) staff       (20)     1537 2023-06-29 18:39:09.000000 sscred_fork-0.2.18/LICENSE
+-rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-08-07 16:12:14.000000 sscred_fork-0.2.18/PKG-INFO
+-rw-r--r--   0 benjaminK   (501) staff       (20)     8328 2023-06-29 18:39:09.000000 sscred_fork-0.2.18/README.md
+-rw-r--r--   0 benjaminK   (501) staff       (20)      878 2023-08-07 16:12:14.000000 sscred_fork-0.2.18/setup.cfg
+-rw-r--r--   0 benjaminK   (501) staff       (20)     1583 2023-07-05 10:12:24.000000 sscred_fork-0.2.18/setup.py
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-07 16:12:14.000000 sscred_fork-0.2.18/sscred/
+-rw-r--r--   0 benjaminK   (501) staff       (20)      503 2023-08-07 16:12:07.000000 sscred_fork-0.2.18/sscred/__init__.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)    15082 2023-08-06 18:49:31.000000 sscred_fork-0.2.18/sscred/acl.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)    12797 2023-08-06 18:51:14.000000 sscred_fork-0.2.18/sscred/blind_pedersen.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)    16436 2023-06-29 18:39:09.000000 sscred_fork-0.2.18/sscred/blind_signature.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)     7555 2023-08-07 16:11:58.000000 sscred_fork-0.2.18/sscred/commitment.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)       31 2023-06-29 18:39:09.000000 sscred_fork-0.2.18/sscred/config.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)     6722 2023-07-07 14:29:32.000000 sscred_fork-0.2.18/sscred/pack.py
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-07 16:12:14.000000 sscred_fork-0.2.18/sscred_fork.egg-info/
+-rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-08-07 16:12:14.000000 sscred_fork-0.2.18/sscred_fork.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminK   (501) staff       (20)      367 2023-08-07 16:12:14.000000 sscred_fork-0.2.18/sscred_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminK   (501) staff       (20)        1 2023-08-07 16:12:14.000000 sscred_fork-0.2.18/sscred_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminK   (501) staff       (20)       43 2023-08-07 16:12:14.000000 sscred_fork-0.2.18/sscred_fork.egg-info/requires.txt
+-rw-r--r--   0 benjaminK   (501) staff       (20)        7 2023-08-07 16:12:14.000000 sscred_fork-0.2.18/sscred_fork.egg-info/top_level.txt
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-07 16:12:14.000000 sscred_fork-0.2.18/test/
+-rw-r--r--   0 benjaminK   (501) staff       (20)    11039 2023-06-29 18:39:09.000000 sscred_fork-0.2.18/test/test_sscred.py
```

### Comparing `sscred_fork-0.2.17/LICENSE` & `sscred_fork-0.2.18/LICENSE`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.17/PKG-INFO` & `sscred_fork-0.2.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sscred_fork
-Version: 0.2.17
+Version: 0.2.18
 Summary: Single Show Credentials: A Python library for anonymous authentication.
 Home-page: https://github.com/spring-epfl/SSCred
 Author: Kasra EdalatNejad
 Author-email: kasra.edalat@epfl.ch
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `sscred_fork-0.2.17/README.md` & `sscred_fork-0.2.18/README.md`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.17/setup.cfg` & `sscred_fork-0.2.18/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sscred
-version = 0.2.17
+version = 0.2.18
 license = BSD-3-Clause
 author = Kasra EdalatNejad
 author_email = kasra.edalat@epfl.ch
 description = Single Show Credentials: A Python library for anonymous authentication.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/spring-epfl/SSCred
```

### Comparing `sscred_fork-0.2.17/setup.py` & `sscred_fork-0.2.18/setup.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.17/sscred/acl.py` & `sscred_fork-0.2.18/sscred/acl.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.17/sscred/blind_pedersen.py` & `sscred_fork-0.2.18/sscred/blind_pedersen.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.17/sscred/blind_signature.py` & `sscred_fork-0.2.18/sscred/blind_signature.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.17/sscred/commitment.py` & `sscred_fork-0.2.18/sscred/commitment.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
         rand: Bn = self.q.random()
         C: EcPt = rand * self.H
         C += self.group.wsum(values, self.HS[:len(values)])
 
         return PedersenCommitment(C), PedersenRandom(rand)
     
-    def extend_commit(self, old_commitment: PedersenCommitment, old_rand: PedersenRandom=None, new_values: Collection[Bn]) -> PedersenCommitment:
+    def extend_commit(self, old_commitment: PedersenCommitment, old_rand: PedersenRandom, new_values: Collection[Bn]) -> PedersenCommitment:
         """Extend a commitment with new values.
 
         Args:
             old_commitment (PedersenCommitment): old commitment
             new_values (Bn mod q): new values to be added to the commitment
 
         Returns:
```

### Comparing `sscred_fork-0.2.17/sscred/pack.py` & `sscred_fork-0.2.18/sscred/pack.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.17/sscred_fork.egg-info/PKG-INFO` & `sscred_fork-0.2.18/sscred_fork.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sscred-fork
-Version: 0.2.17
+Version: 0.2.18
 Summary: Single Show Credentials: A Python library for anonymous authentication.
 Home-page: https://github.com/spring-epfl/SSCred
 Author: Kasra EdalatNejad
 Author-email: kasra.edalat@epfl.ch
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `sscred_fork-0.2.17/test/test_sscred.py` & `sscred_fork-0.2.18/test/test_sscred.py`

 * *Files identical despite different names*

