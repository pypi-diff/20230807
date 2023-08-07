# Comparing `tmp/upathlib-0.8.2b1.tar.gz` & `tmp/upathlib-0.8.2b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upathlib-0.8.2b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "upathlib-0.8.2b2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `upathlib-0.8.2b1.tar` & `upathlib-0.8.2b2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1067 2022-12-13 07:44:37.384893 upathlib-0.8.2b1/LICENSE
--rw-r--r--   0        0        0      993 2023-03-30 16:49:23.794031 upathlib-0.8.2b1/README.rst
--rw-r--r--   0        0        0     1699 2023-06-19 05:49:42.294835 upathlib-0.8.2b1/pyproject.toml
--rw-r--r--   0        0        0     2321 2023-06-26 06:41:12.182147 upathlib-0.8.2b1/src/upathlib/__init__.py
--rw-r--r--   0        0        0     4694 2023-04-20 04:34:46.179551 upathlib-0.8.2b1/src/upathlib/_blob.py
--rw-r--r--   0        0        0    10749 2023-05-13 05:38:06.231654 upathlib-0.8.2b1/src/upathlib/_local.py
--rw-r--r--   0        0        0     7935 2023-04-20 04:34:46.179551 upathlib-0.8.2b1/src/upathlib/_tests.py
--rw-r--r--   0        0        0    34431 2023-06-19 05:53:18.492312 upathlib-0.8.2b1/src/upathlib/_upath.py
--rw-r--r--   0        0        0     2310 2023-06-19 05:53:18.492312 upathlib-0.8.2b1/src/upathlib/_util.py
--rw-r--r--   0        0        0    12562 2023-04-10 08:06:32.346660 upathlib-0.8.2b1/src/upathlib/azure.py
--rw-r--r--   0        0        0    26375 2023-06-26 06:49:05.987099 upathlib-0.8.2b1/src/upathlib/gcs.py
--rw-r--r--   0        0        0        0 2022-12-13 07:44:37.384893 upathlib-0.8.2b1/src/upathlib/py.typed
--rw-r--r--   0        0        0     3763 2023-04-10 08:06:32.346660 upathlib-0.8.2b1/src/upathlib/serializer.py
--rw-r--r--   0        0        0     2348 1970-01-01 00:00:00.000000 upathlib-0.8.2b1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-12-13 07:44:37.384893 upathlib-0.8.2b2/LICENSE
+-rw-r--r--   0        0        0      993 2023-03-30 16:49:23.794031 upathlib-0.8.2b2/README.rst
+-rw-r--r--   0        0        0     1699 2023-06-19 05:49:42.294835 upathlib-0.8.2b2/pyproject.toml
+-rw-r--r--   0        0        0     2321 2023-07-14 19:06:43.581164 upathlib-0.8.2b2/src/upathlib/__init__.py
+-rw-r--r--   0        0        0     4703 2023-07-14 19:04:52.286413 upathlib-0.8.2b2/src/upathlib/_blob.py
+-rw-r--r--   0        0        0    10749 2023-05-13 05:38:06.231654 upathlib-0.8.2b2/src/upathlib/_local.py
+-rw-r--r--   0        0        0     7935 2023-04-20 04:34:46.179551 upathlib-0.8.2b2/src/upathlib/_tests.py
+-rw-r--r--   0        0        0    34431 2023-06-19 05:53:18.492312 upathlib-0.8.2b2/src/upathlib/_upath.py
+-rw-r--r--   0        0        0     2323 2023-07-14 19:05:23.580889 upathlib-0.8.2b2/src/upathlib/_util.py
+-rw-r--r--   0        0        0    12596 2023-07-14 19:06:05.493350 upathlib-0.8.2b2/src/upathlib/azure.py
+-rw-r--r--   0        0        0    26400 2023-07-14 19:06:18.976707 upathlib-0.8.2b2/src/upathlib/gcs.py
+-rw-r--r--   0        0        0        0 2022-12-13 07:44:37.384893 upathlib-0.8.2b2/src/upathlib/py.typed
+-rw-r--r--   0        0        0     3763 2023-04-10 08:06:32.346660 upathlib-0.8.2b2/src/upathlib/serializer.py
+-rw-r--r--   0        0        0     2348 1970-01-01 00:00:00.000000 upathlib-0.8.2b2/PKG-INFO
```

### Comparing `upathlib-0.8.2b1/LICENSE` & `upathlib-0.8.2b2/LICENSE`

 * *Files identical despite different names*

### Comparing `upathlib-0.8.2b1/README.rst` & `upathlib-0.8.2b2/README.rst`

 * *Files identical despite different names*

### Comparing `upathlib-0.8.2b1/pyproject.toml` & `upathlib-0.8.2b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `upathlib-0.8.2b1/src/upathlib/__init__.py` & `upathlib-0.8.2b2/src/upathlib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 One use case is the package `biglist <https://biglist.readthedocs.io/en/latest/>`__,
 where the class `Biglist <https://biglist.readthedocs.io/en/latest/#biglist.Biglist>`__ takes a Upath object to indicate its location of storage.
 It does not care whether the storage is local or in a cloud blob store---it
 simply uses the common API to operate the storage.
 """
 
-__version__ = "0.8.2b1"
+__version__ = "0.8.2b2"
 
 
 from pathlib import Path
 from typing import Union
 
 from ._blob import BlobUpath
 from ._local import LocalPathType, LocalUpath
```

### Comparing `upathlib-0.8.2b1/src/upathlib/_blob.py` & `upathlib-0.8.2b2/src/upathlib/_blob.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 def _resolve_local_path(p: LocalPathType):
     if isinstance(p, str):
         p = pathlib.Path(p)
     if isinstance(p, pathlib.Path):
         p = LocalUpath(str(p.resolve().absolute()))
     else:
-        assert isinstance(p, LocalUpath)
+        assert isinstance(p, LocalUpath), type(p)
     return p
 
 
 class BlobUpath(Upath):
     """
     BlobUpath is a base class for paths in a *cloud* storage, aka "blob store".
     This is in contrast to a *local* disk storage, which is implemnted by :class:`LocalUpath`.
```

### Comparing `upathlib-0.8.2b1/src/upathlib/_local.py` & `upathlib-0.8.2b2/src/upathlib/_local.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.8.2b1/src/upathlib/_tests.py` & `upathlib-0.8.2b2/src/upathlib/_tests.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.8.2b1/src/upathlib/_upath.py` & `upathlib-0.8.2b2/src/upathlib/_upath.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.8.2b1/src/upathlib/_util.py` & `upathlib-0.8.2b2/src/upathlib/_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                 if max_workers is not None:
                     warnings.warn(
                         f"size of the 'default' thread pool is determined internally; the input {max_workers} is ignored"
                     )
                     max_workers = None
             else:
                 if max_workers is not None:
-                    assert 1 <= max_workers <= 64
+                    assert 1 <= max_workers <= 64, max_workers
             executor = ThreadPoolExecutor(max_workers)
             _global_thread_pools_[name] = executor
     return executor
 
 
 if hasattr(os, 'register_at_fork'):  # not available on Windows
```

### Comparing `upathlib-0.8.2b1/src/upathlib/azure.py` & `upathlib-0.8.2b2/src/upathlib/azure.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,18 +51,18 @@
 
     def __init__(
         self,
         *paths: str,
         container_name: str = None,
     ):
         if container_name is None:
-            assert len(paths) == 1
+            assert len(paths) == 1, paths
             path = paths[0]
             account_url = self.get_account_info()["account_url"]
-            assert path.startswith(account_url)
+            assert path.startswith(account_url), path
             path = path[len(account_url) :]
             k = path.find("/")
             if k < 0:
                 container_name = path
                 paths = ("/",)
             else:
                 container_name = path[:k]
@@ -142,15 +142,15 @@
         # TODO: use `overwrite`
         with self._provide_blob_client():
             with source._provide_blob_client():
                 copy = self._blob_client.start_copy_from_url(
                     source._blob_client.url,
                     requires_sync=True,
                 )
-                assert copy["copy_status"] == "success"
+                assert copy["copy_status"] == "success", copy['copy_status']
 
     def _copy_file(self, target: Upath, *, overwrite=False):
         if isinstance(target, AzureBlobUpath):
             target._copy_file_from(self, overwrite=overwrite)
         else:
             super()._copy_file(target, overwrite=overwrite)
```

### Comparing `upathlib-0.8.2b1/src/upathlib/gcs.py` & `upathlib-0.8.2b2/src/upathlib/gcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,27 +185,27 @@
         if bucket_name is None:
             # The first arg must be like
             #   'gs://bucket-name'
             # or
             #   'gs://bucket-name/path...'
 
             p0 = paths[0]
-            assert p0.startswith("gs://")
+            assert p0.startswith("gs://"), p0
             p0 = p0[5:]
             k = p0.find("/")
             if k < 0:
                 bucket_name = p0
                 paths = paths[1:]
             else:
                 bucket_name = p0[:k]
                 p0 = p0[k:]
                 paths = (p0, *paths[1:])
 
         super().__init__(*paths)
-        assert bucket_name
+        assert bucket_name, bucket_name
         self.bucket_name = bucket_name
         self._bucket_ = None
         self._lock_count: int = 0
         self._generation = -1
         self._quiet_multidownload = True
 
     def __repr__(self) -> str:
@@ -583,15 +583,15 @@
         """
         Remove the current dir and all the content under it recursively.
         Return the number of blobs removed.
         """
         z = super().remove_dir(**kwargs)
         prefix = self.blob_name + "/"
         for p in self._client().list_blobs(self._bucket(), prefix=prefix):
-            assert p.name.endswith("/")
+            assert p.name.endswith("/"), p.name
             p.delete()
         return z
 
     def remove_file(self) -> None:
         """
         Remove the current blob.
         """
```

### Comparing `upathlib-0.8.2b1/src/upathlib/serializer.py` & `upathlib-0.8.2b2/src/upathlib/serializer.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.8.2b1/PKG-INFO` & `upathlib-0.8.2b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upathlib
-Version: 0.8.2b1
+Version: 0.8.2b2
 Summary: The package *upathlib*
 Author-email: Zepu Zhang <zepu.zhang@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

