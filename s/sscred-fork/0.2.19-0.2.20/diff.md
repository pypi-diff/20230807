# Comparing `tmp/sscred_fork-0.2.19.tar.gz` & `tmp/sscred_fork-0.2.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sscred_fork-0.2.19.tar", last modified: Mon Aug  7 16:14:13 2023, max compression
+gzip compressed data, was "dist/sscred_fork-0.2.20.tar", last modified: Mon Aug  7 16:17:46 2023, max compression
```

## Comparing `sscred_fork-0.2.19.tar` & `sscred_fork-0.2.20.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-07 16:14:13.000000 sscred_fork-0.2.19/
--rw-r--r--   0 benjaminK   (501) staff       (20)     1537 2023-06-29 18:39:09.000000 sscred_fork-0.2.19/LICENSE
--rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-08-07 16:14:13.000000 sscred_fork-0.2.19/PKG-INFO
--rw-r--r--   0 benjaminK   (501) staff       (20)     8328 2023-06-29 18:39:09.000000 sscred_fork-0.2.19/README.md
--rw-r--r--   0 benjaminK   (501) staff       (20)      878 2023-08-07 16:14:13.000000 sscred_fork-0.2.19/setup.cfg
--rw-r--r--   0 benjaminK   (501) staff       (20)     1583 2023-07-05 10:12:24.000000 sscred_fork-0.2.19/setup.py
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-07 16:14:13.000000 sscred_fork-0.2.19/sscred/
--rw-r--r--   0 benjaminK   (501) staff       (20)      503 2023-08-07 16:14:02.000000 sscred_fork-0.2.19/sscred/__init__.py
--rw-r--r--   0 benjaminK   (501) staff       (20)    15082 2023-08-06 18:49:31.000000 sscred_fork-0.2.19/sscred/acl.py
--rw-r--r--   0 benjaminK   (501) staff       (20)    12797 2023-08-06 18:51:14.000000 sscred_fork-0.2.19/sscred/blind_pedersen.py
--rw-r--r--   0 benjaminK   (501) staff       (20)    16436 2023-06-29 18:39:09.000000 sscred_fork-0.2.19/sscred/blind_signature.py
--rw-r--r--   0 benjaminK   (501) staff       (20)     7555 2023-08-07 16:11:58.000000 sscred_fork-0.2.19/sscred/commitment.py
--rw-r--r--   0 benjaminK   (501) staff       (20)       31 2023-06-29 18:39:09.000000 sscred_fork-0.2.19/sscred/config.py
--rw-r--r--   0 benjaminK   (501) staff       (20)     6722 2023-07-07 14:29:32.000000 sscred_fork-0.2.19/sscred/pack.py
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-07 16:14:13.000000 sscred_fork-0.2.19/sscred_fork.egg-info/
--rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-08-07 16:14:13.000000 sscred_fork-0.2.19/sscred_fork.egg-info/PKG-INFO
--rw-r--r--   0 benjaminK   (501) staff       (20)      367 2023-08-07 16:14:13.000000 sscred_fork-0.2.19/sscred_fork.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminK   (501) staff       (20)        1 2023-08-07 16:14:13.000000 sscred_fork-0.2.19/sscred_fork.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminK   (501) staff       (20)       43 2023-08-07 16:14:13.000000 sscred_fork-0.2.19/sscred_fork.egg-info/requires.txt
--rw-r--r--   0 benjaminK   (501) staff       (20)        7 2023-08-07 16:14:13.000000 sscred_fork-0.2.19/sscred_fork.egg-info/top_level.txt
-drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-07 16:14:13.000000 sscred_fork-0.2.19/test/
--rw-r--r--   0 benjaminK   (501) staff       (20)    11039 2023-06-29 18:39:09.000000 sscred_fork-0.2.19/test/test_sscred.py
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-07 16:17:46.000000 sscred_fork-0.2.20/
+-rw-r--r--   0 benjaminK   (501) staff       (20)     1537 2023-06-29 18:39:09.000000 sscred_fork-0.2.20/LICENSE
+-rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-08-07 16:17:46.000000 sscred_fork-0.2.20/PKG-INFO
+-rw-r--r--   0 benjaminK   (501) staff       (20)     8328 2023-06-29 18:39:09.000000 sscred_fork-0.2.20/README.md
+-rw-r--r--   0 benjaminK   (501) staff       (20)      878 2023-08-07 16:17:46.000000 sscred_fork-0.2.20/setup.cfg
+-rw-r--r--   0 benjaminK   (501) staff       (20)     1583 2023-07-05 10:12:24.000000 sscred_fork-0.2.20/setup.py
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-07 16:17:46.000000 sscred_fork-0.2.20/sscred/
+-rw-r--r--   0 benjaminK   (501) staff       (20)      503 2023-08-07 16:17:41.000000 sscred_fork-0.2.20/sscred/__init__.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)    15214 2023-08-07 16:17:21.000000 sscred_fork-0.2.20/sscred/acl.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)    12797 2023-08-06 18:51:14.000000 sscred_fork-0.2.20/sscred/blind_pedersen.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)    16436 2023-06-29 18:39:09.000000 sscred_fork-0.2.20/sscred/blind_signature.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)     7555 2023-08-07 16:11:58.000000 sscred_fork-0.2.20/sscred/commitment.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)       31 2023-06-29 18:39:09.000000 sscred_fork-0.2.20/sscred/config.py
+-rw-r--r--   0 benjaminK   (501) staff       (20)     6722 2023-07-07 14:29:32.000000 sscred_fork-0.2.20/sscred/pack.py
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-07 16:17:46.000000 sscred_fork-0.2.20/sscred_fork.egg-info/
+-rw-r--r--   0 benjaminK   (501) staff       (20)     9226 2023-08-07 16:17:46.000000 sscred_fork-0.2.20/sscred_fork.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminK   (501) staff       (20)      367 2023-08-07 16:17:46.000000 sscred_fork-0.2.20/sscred_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminK   (501) staff       (20)        1 2023-08-07 16:17:46.000000 sscred_fork-0.2.20/sscred_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminK   (501) staff       (20)       43 2023-08-07 16:17:46.000000 sscred_fork-0.2.20/sscred_fork.egg-info/requires.txt
+-rw-r--r--   0 benjaminK   (501) staff       (20)        7 2023-08-07 16:17:46.000000 sscred_fork-0.2.20/sscred_fork.egg-info/top_level.txt
+drwxr-xr-x   0 benjaminK   (501) staff       (20)        0 2023-08-07 16:17:46.000000 sscred_fork-0.2.20/test/
+-rw-r--r--   0 benjaminK   (501) staff       (20)    11039 2023-06-29 18:39:09.000000 sscred_fork-0.2.20/test/test_sscred.py
```

### Comparing `sscred_fork-0.2.19/LICENSE` & `sscred_fork-0.2.20/LICENSE`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.19/PKG-INFO` & `sscred_fork-0.2.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sscred_fork
-Version: 0.2.19
+Version: 0.2.20
 Summary: Single Show Credentials: A Python library for anonymous authentication.
 Home-page: https://github.com/spring-epfl/SSCred
 Author: Kasra EdalatNejad
 Author-email: kasra.edalat@epfl.ch
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `sscred_fork-0.2.19/README.md` & `sscred_fork-0.2.20/README.md`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.19/setup.cfg` & `sscred_fork-0.2.20/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sscred
-version = 0.2.19
+version = 0.2.20
 license = BSD-3-Clause
 author = Kasra EdalatNejad
 author_email = kasra.edalat@epfl.ch
 description = Single Show Credentials: A Python library for anonymous authentication.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/spring-epfl/SSCred
```

### Comparing `sscred_fork-0.2.19/setup.py` & `sscred_fork-0.2.20/setup.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.19/sscred/acl.py` & `sscred_fork-0.2.20/sscred/acl.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,27 +189,27 @@
         if not valid_commit:
             raise ACLAttributeProofIsInvalid("Attribute proof is invalid.")
         
         commit = prove_attr_msg.commit.commit
         g = self.param.g
         return super()._commit(lambda rnd, commit=commit, g=g: commit + rnd * g)
     
-    def extend_commit(self, old_commitment: PedersenCommitment, new_values: Collection[Attribute]) -> PedersenCommitment:
-        """Extend a Pedersen commitment with new values.
+    # def extend_commit(self, old_commitment: PedersenCommitment, new_values: Collection[Attribute]) -> PedersenCommitment:
+    #     """Extend a Pedersen commitment with new values.
 
-        Args:
-            old_commitment (PedersenCommitment): old commitment
-            new_values (Collection[Bn]): new values to be added to the commitment
-
-        Returns:
-            PedersenCommitment: new, extended commitment
-        """
-        bc_param: BlindedPedersenParam = self.public.bc_param
-        new_pcommit: PedersenCommitment = bc_param.extend_commit(old_commitment, new_values)
-        return new_pcommit
+    #     Args:
+    #         old_commitment (PedersenCommitment): old commitment
+    #         new_values (Collection[Bn]): new values to be added to the commitment
+
+    #     Returns:
+    #         PedersenCommitment: new, extended commitment
+    #     """
+    #     bc_param: BlindedPedersenParam = self.public.bc_param
+    #     new_pcommit: PedersenCommitment = bc_param.extend_commit(old_commitment, new_values)
+    #     return new_pcommit
 
     
     def abe_commit(
         self,
         commitment: PedersenCommitment
         ) -> Tuple[SignerCommitMessage, SignerCommitmentInternalState]:
         """Perform AbeSignature's commit phase.
@@ -303,17 +303,20 @@
         Args:
             old_commitment (PedersenCommitment): old commitment
             new_values (Collection[Bn]): new values to be added to the commitment
 
         Returns:
             PedersenCommitment: new, extended commitment
         """
-        self.attributes += tuple(new_values)
         bc_param: BlindedPedersenParam = self.public.bc_param
-        new_pcommit: PedersenCommitment = bc_param.extend_commit(old_commitment, new_values)
+        self.attributes += tuple(new_values)
+        new_pcommit, new_prand = bc_param.extend_commit(old_commitment, self.prand, new_values)
+        self.pcommit, self.prand = new_pcommit, new_prand
+
+        self.user_attr_commitment = new_pcommit
         return new_pcommit
 
 
     def compute_credential(
             self,
             response: SignerResponseMessage,
             challenge_state: UserBlindedChallengeInternalState
```

### Comparing `sscred_fork-0.2.19/sscred/blind_pedersen.py` & `sscred_fork-0.2.20/sscred/blind_pedersen.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.19/sscred/blind_signature.py` & `sscred_fork-0.2.20/sscred/blind_signature.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.19/sscred/commitment.py` & `sscred_fork-0.2.20/sscred/commitment.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.19/sscred/pack.py` & `sscred_fork-0.2.20/sscred/pack.py`

 * *Files identical despite different names*

### Comparing `sscred_fork-0.2.19/sscred_fork.egg-info/PKG-INFO` & `sscred_fork-0.2.20/sscred_fork.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sscred-fork
-Version: 0.2.19
+Version: 0.2.20
 Summary: Single Show Credentials: A Python library for anonymous authentication.
 Home-page: https://github.com/spring-epfl/SSCred
 Author: Kasra EdalatNejad
 Author-email: kasra.edalat@epfl.ch
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `sscred_fork-0.2.19/test/test_sscred.py` & `sscred_fork-0.2.20/test/test_sscred.py`

 * *Files identical despite different names*

