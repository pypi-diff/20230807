# Comparing `tmp/sscred_fork-0.2.20.tar.gz` & `tmp/sscred_fork-0.2.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sscred_fork-0.2.20.tar", last modified: Mon Aug  7 16:17:46 2023, max compression
+gzip compressed data, was "dist/sscred_fork-0.2.21.tar", last modified: Mon Aug  7 16:18:57 2023, max compression
```

## Comparing `sscred_fork-0.2.20.tar` & `sscred_fork-0.2.21.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-07 16:17:46.000000 sscred_fork-0.2.20/
--rw-r--r--   0 benjaminK   (501) staff       (20)     1537 2023-06-29 18:39:09.000000 sscred_fork-0.2.20/LICENSE
--rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-08-07 16:17:46.000000 sscred_fork-0.2.20/PKG-INFO
--rw-r--r--   0 benjaminK   (501) staff       (20)     8328 2023-06-29 18:39:09.000000 sscred_fork-0.2.20/README.md
--rw-r--r--   0 benjaminK   (501) staff       (20)      878 2023-08-07 16:17:46.000000 sscred_fork-0.2.20/setup.cfg
--rw-r--r--   0 benjaminK   (501) staff       (20)     1583 2023-07-05 10:12:24.000000 sscred_fork-0.2.20/setup.py
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-07 16:17:46.000000 sscred_fork-0.2.20/sscred/
--rw-r--r--   0 benjaminK   (501) staff       (20)      503 2023-08-07 16:17:41.000000 sscred_fork-0.2.20/sscred/__init__.py
--rw-r--r--   0 benjaminK   (501) staff       (20)    15214 2023-08-07 16:17:21.000000 sscred_fork-0.2.20/sscred/acl.py
--rw-r--r--   0 benjaminK   (501) staff       (20)    12797 2023-08-06 18:51:14.000000 sscred_fork-0.2.20/sscred/blind_pedersen.py
--rw-r--r--   0 benjaminK   (501) staff       (20)    16436 2023-06-29 18:39:09.000000 sscred_fork-0.2.20/sscred/blind_signature.py
--rw-r--r--   0 benjaminK   (501) staff       (20)     7555 2023-08-07 16:11:58.000000 sscred_fork-0.2.20/sscred/commitment.py
--rw-r--r--   0 benjaminK   (501) staff       (20)       31 2023-06-29 18:39:09.000000 sscred_fork-0.2.20/sscred/config.py
--rw-r--r--   0 benjaminK   (501) staff       (20)     6722 2023-07-07 14:29:32.000000 sscred_fork-0.2.20/sscred/pack.py
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-07 16:17:46.000000 sscred_fork-0.2.20/sscred_fork.egg-info/
--rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-08-07 16:17:46.000000 sscred_fork-0.2.20/sscred_fork.egg-info/PKG-INFO
--rw-r--r--   0 benjaminK   (501) staff       (20)      367 2023-08-07 16:17:46.000000 sscred_fork-0.2.20/sscred_fork.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminK   (501) staff       (20)        1 2023-08-07 16:17:46.000000 sscred_fork-0.2.20/sscred_fork.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminK   (501) staff       (20)       43 2023-08-07 16:17:46.000000 sscred_fork-0.2.20/sscred_fork.egg-info/requires.txt
--rw-r--r--   0 benjaminK   (501) staff       (20)        7 2023-08-07 16:17:46.000000 sscred_fork-0.2.20/sscred_fork.egg-info/top_level.txt
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-07 16:17:46.000000 sscred_fork-0.2.20/test/
--rw-r--r--   0 benjaminK   (501) staff       (20)    11039 2023-06-29 18:39:09.000000 sscred_fork-0.2.20/test/test_sscred.py
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-07 16:18:57.000000 sscred_fork-0.2.21/
+-rw-r--r--   0 benjaminK   (501) staff       (20)     1537 2023-06-29 18:39:09.000000 sscred_fork-0.2.21/LICENSE
+-rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-08-07 16:18:57.000000 sscred_fork-0.2.21/PKG-INFO
+-rw-r--r--   0 benjaminK   (501) staff       (20)     8328 2023-06-29 18:39:09.000000 sscred_fork-0.2.21/README.md
+-rw-r--r--   0 benjaminK   (501) staff       (20)      878 2023-08-07 16:18:57.000000 sscred_fork-0.2.21/setup.cfg
+-rw-r--r--   0 benjaminK   (501) staff       (20)     1583 2023-07-05 10:12:24.000000 sscred_fork-0.2.21/setup.py
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-07 16:18:57.000000 sscred_fork-0.2.21/sscred/
+-rw-r--r--   0 benjaminK   (501) staff       (20)      503 2023-08-07 16:18:51.000000 sscred_fork-0.2.21/sscred/__init__.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)    15214 2023-08-07 16:17:21.000000 sscred_fork-0.2.21/sscred/acl.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)    12849 2023-08-07 16:18:39.000000 sscred_fork-0.2.21/sscred/blind_pedersen.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)    16436 2023-06-29 18:39:09.000000 sscred_fork-0.2.21/sscred/blind_signature.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)     7555 2023-08-07 16:11:58.000000 sscred_fork-0.2.21/sscred/commitment.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)       31 2023-06-29 18:39:09.000000 sscred_fork-0.2.21/sscred/config.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)     6722 2023-07-07 14:29:32.000000 sscred_fork-0.2.21/sscred/pack.py
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-07 16:18:57.000000 sscred_fork-0.2.21/sscred_fork.egg-info/
+-rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-08-07 16:18:57.000000 sscred_fork-0.2.21/sscred_fork.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminK   (501) staff       (20)      367 2023-08-07 16:18:57.000000 sscred_fork-0.2.21/sscred_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminK   (501) staff       (20)        1 2023-08-07 16:18:57.000000 sscred_fork-0.2.21/sscred_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminK   (501) staff       (20)       43 2023-08-07 16:18:57.000000 sscred_fork-0.2.21/sscred_fork.egg-info/requires.txt
+-rw-r--r--   0 benjaminK   (501) staff       (20)        7 2023-08-07 16:18:57.000000 sscred_fork-0.2.21/sscred_fork.egg-info/top_level.txt
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-07 16:18:57.000000 sscred_fork-0.2.21/test/
+-rw-r--r--   0 benjaminK   (501) staff       (20)    11039 2023-06-29 18:39:09.000000 sscred_fork-0.2.21/test/test_sscred.py
```

### Comparing `sscred_fork-0.2.20/LICENSE` & `sscred_fork-0.2.21/LICENSE`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.20/PKG-INFO` & `sscred_fork-0.2.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sscred_fork
-Version: 0.2.20
+Version: 0.2.21
 Summary: Single Show Credentials: A Python library for anonymous authentication.
 Home-page: https://github.com/spring-epfl/SSCred
 Author: Kasra EdalatNejad
 Author-email: kasra.edalat@epfl.ch
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `sscred_fork-0.2.20/README.md` & `sscred_fork-0.2.21/README.md`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.20/setup.cfg` & `sscred_fork-0.2.21/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sscred
-version = 0.2.20
+version = 0.2.21
 license = BSD-3-Clause
 author = Kasra EdalatNejad
 author_email = kasra.edalat@epfl.ch
 description = Single Show Credentials: A Python library for anonymous authentication.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/spring-epfl/SSCred
```

### Comparing `sscred_fork-0.2.20/setup.py` & `sscred_fork-0.2.21/setup.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.20/sscred/acl.py` & `sscred_fork-0.2.21/sscred/acl.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.20/sscred/blind_pedersen.py` & `sscred_fork-0.2.21/sscred/blind_pedersen.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from petlib.bn import Bn
 from petlib.ec import EcGroup, EcPt
 
 from zksk import Secret, DLRep
 from zksk.base import NIZK
 from zksk.exceptions import StatementMismatch
 
-from .commitment import PedersenCommitment, PedersenParameters
+from .commitment import PedersenCommitment, PedersenParameters, PedersenRandom
 
 
 class BlindedPedersenParam(PedersenParameters):
     """ Common parameters for blinded Pedersen.
     This class provides both vanilla and blinded Pedersen commits. The vanilla
     commit is compatible with PedersenCommitment.
     """
@@ -115,25 +115,25 @@
             (PedersenCommitment): commitment
             (PedersenRand): commitment's randomness
         """
 
         values = [self.process_raw_value(raw) for raw in raw_values]
         return super(BlindedPedersenParam, self).commit(values)
     
-    def extend_commit(self, old_commitment: PedersenCommitment, raw_values: List[Union[Bn, str, bytes]]) -> PedersenCommitment:
+    def extend_commit(self, old_commitment: PedersenCommitment, old_rand: PedersenRandom, raw_values: List[Union[Bn, str, bytes]]) -> PedersenCommitment:
         """Extend a commitment with new values.
 
         Args:
             raw_values (List[Union[Bn, str, bytes]]): new values to be added to the commitment
 
         Returns:
             PedersenCommitment: extended commitment
         """
         values = [self.process_raw_value(raw) for raw in raw_values]
-        return super(BlindedPedersenParam, self).extend_commit(old_commitment, values)
+        return super(BlindedPedersenParam, self).extend_commit(old_commitment, old_rand, values)
 
 
     def blind_commit(self, raw_values, blindness_rand=None, h_rand=None):
         """"a blind commitment to values.
 
         Arguments blindness_rand and h_rand enable ACL compatability.
```

### Comparing `sscred_fork-0.2.20/sscred/blind_signature.py` & `sscred_fork-0.2.21/sscred/blind_signature.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.20/sscred/commitment.py` & `sscred_fork-0.2.21/sscred/commitment.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.20/sscred/pack.py` & `sscred_fork-0.2.21/sscred/pack.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.20/sscred_fork.egg-info/PKG-INFO` & `sscred_fork-0.2.21/sscred_fork.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sscred-fork
-Version: 0.2.20
+Version: 0.2.21
 Summary: Single Show Credentials: A Python library for anonymous authentication.
 Home-page: https://github.com/spring-epfl/SSCred
 Author: Kasra EdalatNejad
 Author-email: kasra.edalat@epfl.ch
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `sscred_fork-0.2.20/test/test_sscred.py` & `sscred_fork-0.2.21/test/test_sscred.py`

 * *Files identical despite different names*

