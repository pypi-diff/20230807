# Comparing `tmp/sscred_fork-0.2.15.tar.gz` & `tmp/sscred_fork-0.2.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sscred_fork-0.2.15.tar", last modified: Sun Aug  6 18:46:32 2023, max compression
+gzip compressed data, was "dist/sscred_fork-0.2.16.tar", last modified: Sun Aug  6 18:52:04 2023, max compression
```

## Comparing `sscred_fork-0.2.15.tar` & `sscred_fork-0.2.16.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-06 18:46:32.000000 sscred_fork-0.2.15/
--rw-r--r--   0 benjaminK   (501) staff       (20)     1537 2023-06-29 18:39:09.000000 sscred_fork-0.2.15/LICENSE
--rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-08-06 18:46:32.000000 sscred_fork-0.2.15/PKG-INFO
--rw-r--r--   0 benjaminK   (501) staff       (20)     8328 2023-06-29 18:39:09.000000 sscred_fork-0.2.15/README.md
--rw-r--r--   0 benjaminK   (501) staff       (20)      878 2023-08-06 18:46:32.000000 sscred_fork-0.2.15/setup.cfg
--rw-r--r--   0 benjaminK   (501) staff       (20)     1583 2023-07-05 10:12:24.000000 sscred_fork-0.2.15/setup.py
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-06 18:46:32.000000 sscred_fork-0.2.15/sscred/
--rw-r--r--   0 benjaminK   (501) staff       (20)      503 2023-08-06 18:46:10.000000 sscred_fork-0.2.15/sscred/__init__.py
--rw-r--r--   0 benjaminK   (501) staff       (20)    14708 2023-08-06 18:28:13.000000 sscred_fork-0.2.15/sscred/acl.py
--rw-r--r--   0 benjaminK   (501) staff       (20)    12745 2023-08-06 18:16:06.000000 sscred_fork-0.2.15/sscred/blind_pedersen.py
--rw-r--r--   0 benjaminK   (501) staff       (20)    16436 2023-06-29 18:39:09.000000 sscred_fork-0.2.15/sscred/blind_signature.py
--rw-r--r--   0 benjaminK   (501) staff       (20)     7368 2023-08-06 18:08:24.000000 sscred_fork-0.2.15/sscred/commitment.py
--rw-r--r--   0 benjaminK   (501) staff       (20)       31 2023-06-29 18:39:09.000000 sscred_fork-0.2.15/sscred/config.py
--rw-r--r--   0 benjaminK   (501) staff       (20)     6722 2023-07-07 14:29:32.000000 sscred_fork-0.2.15/sscred/pack.py
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-06 18:46:32.000000 sscred_fork-0.2.15/sscred_fork.egg-info/
--rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-08-06 18:46:32.000000 sscred_fork-0.2.15/sscred_fork.egg-info/PKG-INFO
--rw-r--r--   0 benjaminK   (501) staff       (20)      367 2023-08-06 18:46:32.000000 sscred_fork-0.2.15/sscred_fork.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminK   (501) staff       (20)        1 2023-08-06 18:46:32.000000 sscred_fork-0.2.15/sscred_fork.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminK   (501) staff       (20)       43 2023-08-06 18:46:32.000000 sscred_fork-0.2.15/sscred_fork.egg-info/requires.txt
--rw-r--r--   0 benjaminK   (501) staff       (20)        7 2023-08-06 18:46:32.000000 sscred_fork-0.2.15/sscred_fork.egg-info/top_level.txt
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-06 18:46:32.000000 sscred_fork-0.2.15/test/
--rw-r--r--   0 benjaminK   (501) staff       (20)    11039 2023-06-29 18:39:09.000000 sscred_fork-0.2.15/test/test_sscred.py
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-06 18:52:04.000000 sscred_fork-0.2.16/
+-rw-r--r--   0 benjaminK   (501) staff       (20)     1537 2023-06-29 18:39:09.000000 sscred_fork-0.2.16/LICENSE
+-rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-08-06 18:52:04.000000 sscred_fork-0.2.16/PKG-INFO
+-rw-r--r--   0 benjaminK   (501) staff       (20)     8328 2023-06-29 18:39:09.000000 sscred_fork-0.2.16/README.md
+-rw-r--r--   0 benjaminK   (501) staff       (20)      878 2023-08-06 18:52:04.000000 sscred_fork-0.2.16/setup.cfg
+-rw-r--r--   0 benjaminK   (501) staff       (20)     1583 2023-07-05 10:12:24.000000 sscred_fork-0.2.16/setup.py
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-06 18:52:04.000000 sscred_fork-0.2.16/sscred/
+-rw-r--r--   0 benjaminK   (501) staff       (20)      503 2023-08-06 18:51:51.000000 sscred_fork-0.2.16/sscred/__init__.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)    15082 2023-08-06 18:49:31.000000 sscred_fork-0.2.16/sscred/acl.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)    12797 2023-08-06 18:51:14.000000 sscred_fork-0.2.16/sscred/blind_pedersen.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)    16436 2023-06-29 18:39:09.000000 sscred_fork-0.2.16/sscred/blind_signature.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)     7368 2023-08-06 18:08:24.000000 sscred_fork-0.2.16/sscred/commitment.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)       31 2023-06-29 18:39:09.000000 sscred_fork-0.2.16/sscred/config.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)     6722 2023-07-07 14:29:32.000000 sscred_fork-0.2.16/sscred/pack.py
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-06 18:52:04.000000 sscred_fork-0.2.16/sscred_fork.egg-info/
+-rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-08-06 18:52:03.000000 sscred_fork-0.2.16/sscred_fork.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminK   (501) staff       (20)      367 2023-08-06 18:52:03.000000 sscred_fork-0.2.16/sscred_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminK   (501) staff       (20)        1 2023-08-06 18:52:03.000000 sscred_fork-0.2.16/sscred_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminK   (501) staff       (20)       43 2023-08-06 18:52:03.000000 sscred_fork-0.2.16/sscred_fork.egg-info/requires.txt
+-rw-r--r--   0 benjaminK   (501) staff       (20)        7 2023-08-06 18:52:03.000000 sscred_fork-0.2.16/sscred_fork.egg-info/top_level.txt
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-06 18:52:04.000000 sscred_fork-0.2.16/test/
+-rw-r--r--   0 benjaminK   (501) staff       (20)    11039 2023-06-29 18:39:09.000000 sscred_fork-0.2.16/test/test_sscred.py
```

### Comparing `sscred_fork-0.2.15/LICENSE` & `sscred_fork-0.2.16/LICENSE`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.15/PKG-INFO` & `sscred_fork-0.2.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sscred_fork
-Version: 0.2.15
+Version: 0.2.16
 Summary: Single Show Credentials: A Python library for anonymous authentication.
 Home-page: https://github.com/spring-epfl/SSCred
 Author: Kasra EdalatNejad
 Author-email: kasra.edalat@epfl.ch
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `sscred_fork-0.2.15/README.md` & `sscred_fork-0.2.16/README.md`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.15/setup.cfg` & `sscred_fork-0.2.16/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sscred
-version = 0.2.15
+version = 0.2.16
 license = BSD-3-Clause
 author = Kasra EdalatNejad
 author_email = kasra.edalat@epfl.ch
 description = Single Show Credentials: A Python library for anonymous authentication.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/spring-epfl/SSCred
```

### Comparing `sscred_fork-0.2.15/setup.py` & `sscred_fork-0.2.16/setup.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.15/sscred/acl.py` & `sscred_fork-0.2.16/sscred/acl.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,14 +219,25 @@
 
         Returns:
             Tuple[SignerCommitMessage, SignerCommitmentInternalState] 
         """
         commit = commitment.commit
         g = self.param.g
         return super()._commit(lambda rnd, commit=commit, g=g: commit + rnd * g)
+    
+    def verify_proof(
+        self,
+        prove_attr_msg: ProveAttrKnowledgeMessage,
+        ) -> None:
+        valid_commit = prove_attr_msg.commit.verify_proof(
+            pparam = self.public.bc_param,
+            proof = prove_attr_msg.nizk_proof
+        )
+        if not valid_commit:
+            raise ACLAttributeProofIsInvalid("Attribute proof is invalid.")
 
 
 class ACLUser(AbeUser):
     """An ACL user which receives a credential.
     This class stores a state and only supports one credential at a time.
 
     Attributes:
```

### Comparing `sscred_fork-0.2.15/sscred/blind_pedersen.py` & `sscred_fork-0.2.16/sscred/blind_pedersen.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,25 +115,25 @@
             (PedersenCommitment): commitment
             (PedersenRand): commitment's randomness
         """
 
         values = [self.process_raw_value(raw) for raw in raw_values]
         return super(BlindedPedersenParam, self).commit(values)
     
-    def extend_commit(self, raw_values: List[Union[Bn, str, bytes]]) -> PedersenCommitment:
+    def extend_commit(self, old_commitment: PedersenCommitment, raw_values: List[Union[Bn, str, bytes]]) -> PedersenCommitment:
         """Extend a commitment with new values.
 
         Args:
             raw_values (List[Union[Bn, str, bytes]]): new values to be added to the commitment
 
         Returns:
             PedersenCommitment: extended commitment
         """
         values = [self.process_raw_value(raw) for raw in raw_values]
-        return super(BlindedPedersenParam, self).extend_commit(values)
+        return super(BlindedPedersenParam, self).extend_commit(old_commitment, values)
 
 
     def blind_commit(self, raw_values, blindness_rand=None, h_rand=None):
         """"a blind commitment to values.
 
         Arguments blindness_rand and h_rand enable ACL compatability.
```

### Comparing `sscred_fork-0.2.15/sscred/blind_signature.py` & `sscred_fork-0.2.16/sscred/blind_signature.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.15/sscred/commitment.py` & `sscred_fork-0.2.16/sscred/commitment.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.15/sscred/pack.py` & `sscred_fork-0.2.16/sscred/pack.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.15/sscred_fork.egg-info/PKG-INFO` & `sscred_fork-0.2.16/sscred_fork.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sscred-fork
-Version: 0.2.15
+Version: 0.2.16
 Summary: Single Show Credentials: A Python library for anonymous authentication.
 Home-page: https://github.com/spring-epfl/SSCred
 Author: Kasra EdalatNejad
 Author-email: kasra.edalat@epfl.ch
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `sscred_fork-0.2.15/test/test_sscred.py` & `sscred_fork-0.2.16/test/test_sscred.py`

 * *Files identical despite different names*

