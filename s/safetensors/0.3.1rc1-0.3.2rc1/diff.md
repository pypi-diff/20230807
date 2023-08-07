# Comparing `tmp/safetensors-0.3.1rc1.tar.gz` & `tmp/safetensors-0.3.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safetensors-0.3.1rc1.tar", last modified: Mon Apr 24 15:00:13 2023, max compression
+gzip compressed data, was "safetensors-0.3.2rc1.tar", last modified: Mon Aug  7 14:41:58 2023, max compression
```

## Comparing `safetensors-0.3.1rc1.tar` & `safetensors-0.3.2rc1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-24 15:00:12.000000 safetensors-0.3.1rc1/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.598883 safetensors-0.3.1rc1/py_src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.598883 safetensors-0.3.1rc1/py_src/safetensors/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/py_src/safetensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/py_src/safetensors/flax.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/py_src/safetensors/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/py_src/safetensors/paddle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/py_src/safetensors/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    14270 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/py_src/safetensors/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/py_src/safetensors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-24 15:00:13.000000 safetensors-0.3.1rc1/py_src/safetensors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-24 15:00:13.000000 safetensors-0.3.1rc1/py_src/safetensors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:00:13.000000 safetensors-0.3.1rc1/py_src/safetensors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:00:13.000000 safetensors-0.3.1rc1/py_src/safetensors.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-24 15:00:13.000000 safetensors-0.3.1rc1/py_src/safetensors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 15:00:13.000000 safetensors-0.3.1rc1/py_src/safetensors.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/safetensors-lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     9588 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/README.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/safetensors-lib/benches/
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/benches/benchmark.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/safetensors-lib/fuzz/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/fuzz/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/fuzz/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/safetensors-lib/fuzz/fuzz_targets/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/fuzz/fuzz_targets/fuzz_target_1.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/safetensors-lib/src/
--rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/src/slice.rs
--rw-r--r--   0 runner    (1001) docker     (123)    39349 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/safetensors-lib/src/tensor.rs
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:00:13.602883 safetensors-0.3.1rc1/src/
--rw-r--r--   0 runner    (1001) docker     (123)    33654 2023-04-24 14:59:50.000000 safetensors-0.3.1rc1/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:41:58.076787 safetensors-0.3.2rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-07 14:41:57.000000 safetensors-0.3.2rc1/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-07 14:41:47.000000 safetensors-0.3.2rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-08-07 14:41:58.076787 safetensors-0.3.2rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-07 14:41:47.000000 safetensors-0.3.2rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:41:58.072787 safetensors-0.3.2rc1/py_src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:41:58.076787 safetensors-0.3.2rc1/py_src/safetensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-07 14:41:47.000000 safetensors-0.3.2rc1/py_src/safetensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-08-07 14:41:47.000000 safetensors-0.3.2rc1/py_src/safetensors/flax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-08-07 14:41:47.000000 safetensors-0.3.2rc1/py_src/safetensors/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-08-07 14:41:47.000000 safetensors-0.3.2rc1/py_src/safetensors/paddle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-08-07 14:41:47.000000 safetensors-0.3.2rc1/py_src/safetensors/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16091 2023-08-07 14:41:47.000000 safetensors-0.3.2rc1/py_src/safetensors/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:41:58.076787 safetensors-0.3.2rc1/py_src/safetensors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-08-07 14:41:58.000000 safetensors-0.3.2rc1/py_src/safetensors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-07 14:41:58.000000 safetensors-0.3.2rc1/py_src/safetensors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 14:41:58.000000 safetensors-0.3.2rc1/py_src/safetensors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 14:41:58.000000 safetensors-0.3.2rc1/py_src/safetensors.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-07 14:41:58.000000 safetensors-0.3.2rc1/py_src/safetensors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 14:41:58.000000 safetensors-0.3.2rc1/py_src/safetensors.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-07 14:41:47.000000 safetensors-0.3.2rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:41:58.076787 safetensors-0.3.2rc1/safetensors-lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-07 14:41:47.000000 safetensors-0.3.2rc1/safetensors-lib/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-08-07 14:41:47.000000 safetensors-0.3.2rc1/safetensors-lib/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-08-07 14:41:47.000000 safetensors-0.3.2rc1/safetensors-lib/README.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:41:58.076787 safetensors-0.3.2rc1/safetensors-lib/benches/
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-08-07 14:41:47.000000 safetensors-0.3.2rc1/safetensors-lib/benches/benchmark.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:41:58.076787 safetensors-0.3.2rc1/safetensors-lib/fuzz/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-07 14:41:47.000000 safetensors-0.3.2rc1/safetensors-lib/fuzz/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-07 14:41:47.000000 safetensors-0.3.2rc1/safetensors-lib/fuzz/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:41:58.076787 safetensors-0.3.2rc1/safetensors-lib/fuzz/fuzz_targets/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-07 14:41:47.000000 safetensors-0.3.2rc1/safetensors-lib/fuzz/fuzz_targets/fuzz_target_1.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:41:58.076787 safetensors-0.3.2rc1/safetensors-lib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-08-07 14:41:47.000000 safetensors-0.3.2rc1/safetensors-lib/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-08-07 14:41:47.000000 safetensors-0.3.2rc1/safetensors-lib/src/slice.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    39729 2023-08-07 14:41:47.000000 safetensors-0.3.2rc1/safetensors-lib/src/tensor.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-07 14:41:58.076787 safetensors-0.3.2rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-08-07 14:41:47.000000 safetensors-0.3.2rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:41:58.076787 safetensors-0.3.2rc1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    35465 2023-08-07 14:41:47.000000 safetensors-0.3.2rc1/src/lib.rs
```

### Comparing `safetensors-0.3.1rc1/PKG-INFO` & `safetensors-0.3.2rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safetensors
-Version: 0.3.1rc1
+Version: 0.3.2rc1
 Summary: Fast and Safe Tensor serialization
 Home-page: https://github.com/huggingface/safetensors
 Author: 
 Author-email: 
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -22,14 +22,15 @@
 Provides-Extra: torch
 Provides-Extra: numpy
 Provides-Extra: tensorflow
 Provides-Extra: jax
 Provides-Extra: paddlepaddle
 Provides-Extra: quality
 Provides-Extra: testing
+Provides-Extra: pinned-tf
 Provides-Extra: all
 Provides-Extra: dev
 
 ## Installation
 
 ```
 pip install safetensors
```

### Comparing `safetensors-0.3.1rc1/README.md` & `safetensors-0.3.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.1rc1/py_src/safetensors/flax.py` & `safetensors-0.3.2rc1/py_src/safetensors/flax.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import os
 from typing import Dict, Optional, Union
 
 import numpy as np
 
 import jax.numpy as jnp
+from jax import Array
 from safetensors import numpy
 
 
-def save(tensors: Dict[str, jnp.DeviceArray], metadata: Optional[Dict[str, str]] = None) -> bytes:
+def save(tensors: Dict[str, Array], metadata: Optional[Dict[str, str]] = None) -> bytes:
     """
     Saves a dictionnary of tensors into raw bytes in safetensors format.
 
     Args:
-        tensors (`Dict[str, jnp.DeviceArray]`):
+        tensors (`Dict[str, Array]`):
             The incoming tensors. Tensors need to be contiguous and dense.
         metadata (`Dict[str, str]`, *optional*, defaults to `None`):
             Optional text only metadata you might want to save in your header.
             For instance it can be useful to specify more about the underlying
             tensors. This is purely informative and does not affect tensor loading.
 
     Returns:
@@ -33,23 +34,23 @@
     ```
     """
     np_tensors = _jnp2np(tensors)
     return numpy.save(np_tensors, metadata=metadata)
 
 
 def save_file(
-    tensors: Dict[str, jnp.DeviceArray],
+    tensors: Dict[str, Array],
     filename: Union[str, os.PathLike],
     metadata: Optional[Dict[str, str]] = None,
 ) -> None:
     """
     Saves a dictionnary of tensors into raw bytes in safetensors format.
 
     Args:
-        tensors (`Dict[str, jnp.DeviceArray]`):
+        tensors (`Dict[str, Array]`):
             The incoming tensors. Tensors need to be contiguous and dense.
         filename (`str`, or `os.PathLike`)):
             The filename we're saving into.
         metadata (`Dict[str, str]`, *optional*, defaults to `None`):
             Optional text only metadata you might want to save in your header.
             For instance it can be useful to specify more about the underlying
             tensors. This is purely informative and does not affect tensor loading.
@@ -67,24 +68,24 @@
     save(tensors, "model.safetensors")
     ```
     """
     np_tensors = _jnp2np(tensors)
     return numpy.save_file(np_tensors, filename, metadata=metadata)
 
 
-def load(data: bytes) -> Dict[str, jnp.DeviceArray]:
+def load(data: bytes) -> Dict[str, Array]:
     """
     Loads a safetensors file into flax format from pure bytes.
 
     Args:
         data (`bytes`):
             The content of a safetensors file
 
     Returns:
-        `Dict[str, jnp.DeviceArray]`: dictionary that contains name as key, value as `jnp.DeviceArray` on cpu
+        `Dict[str, Array]`: dictionary that contains name as key, value as `Array` on cpu
 
     Example:
 
     ```python
     from safetensors.flax import load
 
     file_path = "./my_folder/bert.safetensors"
@@ -94,44 +95,44 @@
     loaded = load(data)
     ```
     """
     flat = numpy.load(data)
     return _np2jnp(flat)
 
 
-def load_file(filename: Union[str, os.PathLike]) -> Dict[str, jnp.DeviceArray]:
+def load_file(filename: Union[str, os.PathLike]) -> Dict[str, Array]:
     """
     Loads a safetensors file into flax format.
 
     Args:
         filename (`str`, or `os.PathLike`)):
             The name of the file which contains the tensors
         device (`Dict[str, any]`, *optional*, defaults to `cpu`):
             The device where the tensors need to be located after load.
             available options are all regular flax device locations
 
     Returns:
-        `Dict[str, jnp.DeviceArray]`: dictionary that contains name as key, value as `jnp.DeviceArray`
+        `Dict[str, Array]`: dictionary that contains name as key, value as `Array`
 
     Example:
 
     ```python
     from safetensors.flax import load_file
 
     file_path = "./my_folder/bert.safetensors"
     loaded = load_file(file_path)
     ```
     """
     flat = numpy.load_file(filename)
     return _np2jnp(flat)
 
 
-def _np2jnp(numpy_dict: Dict[str, np.ndarray]) -> Dict[str, jnp.DeviceArray]:
+def _np2jnp(numpy_dict: Dict[str, np.ndarray]) -> Dict[str, Array]:
     for k, v in numpy_dict.items():
         numpy_dict[k] = jnp.array(v)
     return numpy_dict
 
 
-def _jnp2np(jnp_dict: Dict[str, jnp.DeviceArray]) -> Dict[str, np.array]:
+def _jnp2np(jnp_dict: Dict[str, Array]) -> Dict[str, np.array]:
     for k, v in jnp_dict.items():
         jnp_dict[k] = np.asarray(v)
     return jnp_dict
```

### Comparing `safetensors-0.3.1rc1/py_src/safetensors/numpy.py` & `safetensors-0.3.2rc1/py_src/safetensors/numpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 def save(tensor_dict: Dict[str, np.ndarray], metadata: Optional[Dict[str, str]] = None) -> bytes:
     """
     Saves a dictionnary of tensors into raw bytes in safetensors format.
 
     Args:
-        tensors (`Dict[str, np.ndarray]`):
+        tensor_dict (`Dict[str, np.ndarray]`):
             The incoming tensors. Tensors need to be contiguous and dense.
         metadata (`Dict[str, str]`, *optional*, defaults to `None`):
             Optional text only metadata you might want to save in your header.
             For instance it can be useful to specify more about the underlying
             tensors. This is purely informative and does not affect tensor loading.
 
     Returns:
@@ -30,29 +30,29 @@
 
     tensors = {"embedding": np.zeros((512, 1024)), "attention": np.zeros((256, 256))}
     byte_data = save(tensors)
     ```
     """
     for tensor in tensor_dict.values():
         if not _is_little_endian(tensor):
-            raise ValueError("Safetensor format only accepts little endian")
+            tensor.byteswap(inplace=True)
     flattened = {k: {"dtype": v.dtype.name, "shape": v.shape, "data": v.tobytes()} for k, v in tensor_dict.items()}
     serialized = serialize(flattened, metadata=metadata)
     result = bytes(serialized)
     return result
 
 
 def save_file(
     tensor_dict: Dict[str, np.ndarray], filename: Union[str, os.PathLike], metadata: Optional[Dict[str, str]] = None
 ) -> None:
     """
     Saves a dictionnary of tensors into raw bytes in safetensors format.
 
     Args:
-        tensors (`Dict[str, np.ndarray]`):
+        tensor_dict (`Dict[str, np.ndarray]`):
             The incoming tensors. Tensors need to be contiguous and dense.
         filename (`str`, or `os.PathLike`)):
             The filename we're saving into.
         metadata (`Dict[str, str]`, *optional*, defaults to `None`):
             Optional text only metadata you might want to save in your header.
             For instance it can be useful to specify more about the underlying
             tensors. This is purely informative and does not affect tensor loading.
@@ -68,15 +68,15 @@
 
     tensors = {"embedding": np.zeros((512, 1024)), "attention": np.zeros((256, 256))}
     save(tensors, "model.safetensors")
     ```
     """
     for tensor in tensor_dict.values():
         if not _is_little_endian(tensor):
-            raise ValueError("Safetensor format only accepts little endian")
+            tensor.byteswap(inplace=True)
     flattened = {k: {"dtype": v.dtype.name, "shape": v.shape, "data": v.tobytes()} for k, v in tensor_dict.items()}
     serialize_file(flattened, filename, metadata=metadata)
 
 
 def load(data: bytes) -> Dict[str, np.ndarray]:
     """
     Loads a safetensors file into numpy format from pure bytes.
```

### Comparing `safetensors-0.3.1rc1/py_src/safetensors/paddle.py` & `safetensors-0.3.2rc1/py_src/safetensors/paddle.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.1rc1/py_src/safetensors/tensorflow.py` & `safetensors-0.3.2rc1/py_src/safetensors/tensorflow.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.1rc1/py_src/safetensors/torch.py` & `safetensors-0.3.2rc1/py_src/safetensors/torch.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,79 +16,129 @@
         try:
             return tensor.storage().data_ptr()
         except NotImplementedError:
             # Fallback for meta storage
             return 0
 
 
+def _end_ptr(tensor: torch.Tensor) -> int:
+    if tensor.nelement():
+        stop = tensor.view(-1)[-1].data_ptr() + _SIZE[tensor.dtype]
+    else:
+        stop = tensor.data_ptr()
+    return stop
+
+
 def storage_size(tensor: torch.Tensor) -> int:
     try:
         return tensor.untyped_storage().nbytes()
     except AttributeError:
         # Fallback for torch==1.10
         try:
             return tensor.storage().size() * _SIZE[tensor.dtype]
         except NotImplementedError:
             # Fallback for meta storage
             # On torch >=2.0 this is the tensor size
             return tensor.nelement() * _SIZE[tensor.dtype]
 
 
+def _filter_shared_not_shared(tensors: List[Set[str]], state_dict: Dict[str, torch.Tensor]) -> List[Set[str]]:
+    filtered_tensors = []
+    for shared in tensors:
+
+        if len(shared) < 2:
+            filtered_tensors.append(shared)
+            continue
+
+        areas = []
+        for name in shared:
+            tensor = state_dict[name]
+            areas.append((tensor.data_ptr(), _end_ptr(tensor), name))
+        areas.sort()
+
+        _, last_stop, last_name = areas[0]
+        filtered_tensors.append({last_name})
+        for start, stop, name in areas[1:]:
+            if start >= last_stop:
+                filtered_tensors.append({name})
+            else:
+                filtered_tensors[-1].add(name)
+            last_stop = stop
+
+    return filtered_tensors
+
+
 def _find_shared_tensors(state_dict: Dict[str, torch.Tensor]) -> List[Set[str]]:
     tensors = defaultdict(set)
     for k, v in state_dict.items():
-        if v.device != torch.device("meta"):
+        if v.device != torch.device("meta") and storage_ptr(v) != 0 and storage_size(v) != 0:
             # Need to add device as key because of multiple GPU.
-            tensors[(storage_ptr(v), v.device)].add(k)
+            tensors[(v.device, storage_ptr(v), storage_size(v))].add(k)
     tensors = list(sorted(tensors.values()))
+    tensors = _filter_shared_not_shared(tensors, state_dict)
     return tensors
 
 
 def _is_complete(tensor: torch.Tensor) -> bool:
     return tensor.data_ptr() == storage_ptr(tensor) and tensor.nelement() * _SIZE[tensor.dtype] == storage_size(tensor)
 
 
 def _remove_duplicate_names(
-    state_dict: Dict[str, torch.Tensor], preferred_names: List[str] = None
+    state_dict: Dict[str, torch.Tensor],
+    *,
+    preferred_names: Optional[List[str]] = None,
+    discard_names: Optional[List[str]] = None,
 ) -> Dict[str, List[str]]:
     if preferred_names is None:
         preferred_names = []
     preferred_names = set(preferred_names)
+    if discard_names is None:
+        discard_names = []
+    discard_names = set(discard_names)
 
     shareds = _find_shared_tensors(state_dict)
     to_remove = defaultdict(list)
     for shared in shareds:
-        complete_names = [name for name in shared if _is_complete(state_dict[name])]
+        complete_names = set([name for name in shared if _is_complete(state_dict[name])])
         if not complete_names:
             raise RuntimeError(
-                f"Error while trying to find names to remove to save state dict, but found no suitable name to keep for saving amongst: {shared}. None is covering the entire storage.Refusing to save/load the model since you could be storing much more memory than needed. Please refer to https://huggingface.co/docs/safetensors/torch_shared_tensors for more information. Or open an issue."
+                "Error while trying to find names to remove to save state dict, but found no suitable name to keep"
+                f" for saving amongst: {shared}. None is covering the entire storage.Refusing to save/load the model"
+                " since you could be storing much more memory than needed. Please refer to"
+                " https://huggingface.co/docs/safetensors/torch_shared_tensors for more information. Or open an"
+                " issue."
             )
 
-        preferred = preferred_names.intersection(set(complete_names))
+        keep_name = sorted(list(complete_names))[0]
+
         # Mecanism to preferentially select keys to keep
-        # coming from the on-disk file to allow\
+        # coming from the on-disk file to allow
         # loading models saved with a different choice
         # of keep_name
+        preferred = complete_names.difference(discard_names)
         if preferred:
             keep_name = sorted(list(preferred))[0]
-        else:
-            keep_name = sorted(complete_names)[0]
+
+        if preferred_names:
+            preferred = preferred_names.intersection(complete_names)
+            if preferred:
+                keep_name = sorted(list(preferred))[0]
         for name in sorted(shared):
             if name != keep_name:
                 to_remove[keep_name].append(name)
     return to_remove
 
 
 def save_model(
     model: torch.nn.Module, filename: str, metadata: Optional[Dict[str, str]] = None, force_contiguous: bool = True
 ):
     """
     Saves a given torch model to specified filename.
     This method exists specifically to avoid tensor sharing issues which are
-    not allowed in `safetensors`. [More information on tensor sharing](torch_shared_tensors)
+    not allowed in `safetensors`. [More information on tensor sharing](../torch_shared_tensors)
 
     Args:
         model (`torch.nn.Module`):
             The model to save on disk.
         filename (`str`):
             The filename location to save the file
         metadata (`Dict[str, str]`, *optional*):
@@ -124,15 +174,15 @@
         raise ValueError(msg)
 
 
 def load_model(model: torch.nn.Module, filename: str, strict=True) -> Tuple[List[str], List[str]]:
     """
     Loads a given filename onto a torch model.
     This method exists specifically to avoid tensor sharing issues which are
-    not allowed in `safetensors`. [More information on tensor sharing](torch_shared_tensors)
+    not allowed in `safetensors`. [More information on tensor sharing](../torch_shared_tensors)
 
     Args:
         model (`torch.nn.Module`):
             The model to load onto.
         filename (`str`):
             The filename location to load the file from.
         strict (`bool`, *optional*, defaults to True):
@@ -364,33 +414,40 @@
     total_bytes = length * bytes_per_item
 
     ptr = tensor.data_ptr()
     if ptr == 0:
         return b""
     newptr = ctypes.cast(ptr, ctypes.POINTER(ctypes.c_ubyte))
     data = np.ctypeslib.as_array(newptr, (total_bytes,))  # no internal copy
-
+    if sys.byteorder == "big":
+        data.byteswap(inplace=True)
     return data.tobytes()
 
 
 def _flatten(tensors: Dict[str, torch.Tensor]) -> Dict[str, Dict[str, Any]]:
-    if sys.byteorder == "big":
-        raise ValueError("Big endian is not supported, serialization need to be in little endian")
     if not isinstance(tensors, dict):
         raise ValueError(f"Expected a dict of [str, torch.Tensor] but received {type(tensors)}")
-    ptrs = defaultdict(set)
+
+    invalid_tensors = []
     for k, v in tensors.items():
         if not isinstance(v, torch.Tensor):
             raise ValueError(f"Key `{k}` is invalid, expected torch.Tensor but received {type(v)}")
 
-        if v.layout == torch.strided:
-            ptrs[storage_ptr(v)].add(k)
+        if v.layout != torch.strided:
+            invalid_tensors.append(k)
+    if invalid_tensors:
+        raise ValueError(
+            f"You are trying to save a sparse tensors: `{invalid_tensors}` which this library does not support."
+            " You can make it a dense tensor before saving with `.to_dense()` but be aware this might"
+            " make a much larger file than needed."
+        )
 
+    shared_pointers = _find_shared_tensors(tensors)
     failing = []
-    for ptr, names in ptrs.items():
+    for names in shared_pointers:
         if len(names) > 1:
             failing.append(names)
 
     if failing:
         raise RuntimeError(
             f"""
             Some tensors share memory, this will lead to duplicate memory on disk and potential differences when loading them again: {failing}.
```

### Comparing `safetensors-0.3.1rc1/py_src/safetensors.egg-info/PKG-INFO` & `safetensors-0.3.2rc1/py_src/safetensors.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safetensors
-Version: 0.3.1rc1
+Version: 0.3.2rc1
 Summary: Fast and Safe Tensor serialization
 Home-page: https://github.com/huggingface/safetensors
 Author: 
 Author-email: 
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -22,14 +22,15 @@
 Provides-Extra: torch
 Provides-Extra: numpy
 Provides-Extra: tensorflow
 Provides-Extra: jax
 Provides-Extra: paddlepaddle
 Provides-Extra: quality
 Provides-Extra: testing
+Provides-Extra: pinned-tf
 Provides-Extra: all
 Provides-Extra: dev
 
 ## Installation
 
 ```
 pip install safetensors
```

### Comparing `safetensors-0.3.1rc1/py_src/safetensors.egg-info/SOURCES.txt` & `safetensors-0.3.2rc1/py_src/safetensors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.1rc1/py_src/safetensors.egg-info/requires.txt` & `safetensors-0.3.2rc1/py_src/safetensors.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 [all]
 torch>=1.10
 numpy>=1.21.6
-tensorflow>=2.11.0
+tensorflow==2.11.0
 jax>=0.3.25
 flax>=0.6.3
 jaxlib>=0.3.25
 paddlepaddle>=2.4.1
 black==22.3
 isort>=5.5.4
 flake8>=3.8.3
@@ -16,15 +16,15 @@
 pytest>=7.2.0
 pytest-benchmark>=4.0.0
 h5py>=3.7.0
 
 [dev]
 torch>=1.10
 numpy>=1.21.6
-tensorflow>=2.11.0
+tensorflow==2.11.0
 jax>=0.3.25
 flax>=0.6.3
 jaxlib>=0.3.25
 paddlepaddle>=2.4.1
 black==22.3
 isort>=5.5.4
 flake8>=3.8.3
@@ -42,14 +42,17 @@
 
 [numpy]
 numpy>=1.21.6
 
 [paddlepaddle]
 paddlepaddle>=2.4.1
 
+[pinned-tf]
+tensorflow==2.11.0
+
 [quality]
 black==22.3
 isort>=5.5.4
 flake8>=3.8.3
 click==8.0.4
 
 [tensorflow]
```

### Comparing `safetensors-0.3.1rc1/safetensors-lib/Cargo.toml` & `safetensors-0.3.2rc1/safetensors-lib/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "safetensors"
-version = "0.3.1"
+version = "0.3.2"
 edition = "2021"
 homepage = "https://github.com/huggingface/safetensors"
 repository = "https://github.com/huggingface/safetensors"
 documentation = "https://docs.rs/safetensors/"
 license = "Apache-2.0"
 keywords = ["safetensors", "huggingface", "Tensors", "Pytorch", "Tensorflow"]
 readme = "./README.md"
```

### Comparing `safetensors-0.3.1rc1/safetensors-lib/README.md` & `safetensors-0.3.2rc1/safetensors-lib/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+<p align="center">
+  <picture>
+    <source media="(prefers-color-scheme: dark)" srcset="https://huggingface.co/datasets/safetensors/assets/raw/main/banner-dark.svg">
+    <source media="(prefers-color-scheme: light)" srcset="https://huggingface.co/datasets/safetensors/assets/raw/main/banner-light.svg">
+    <img alt="Hugging Face Safetensors Library" src="https://huggingface.co/datasets/safetensors/assets/raw/main/banner-light.svg" style="max-width: 100%;">
+  </picture>
+  <br/>
+  <br/>
+</p>
+
 Python
 [![Pypi](https://img.shields.io/pypi/v/safetensors.svg)](https://pypi.org/pypi/safetensors/)
 [![Documentation](https://img.shields.io/website/http/huggingface.co/docs/safetensors/index.svg?label=docs)](https://huggingface.co/docs/safetensors/index)
 [![Codecov](https://codecov.io/github/huggingface/safetensors/coverage.svg?branch=main)](https://codecov.io/gh/huggingface/safetensors)
 [![Downloads](https://static.pepy.tech/badge/safetensors/month)](https://pepy.tech/project/safetensors)
 
 Rust
@@ -63,16 +73,16 @@
 [Python documentation](https://huggingface.co/docs/safetensors/index)
 
 
 ### Format
 
 - 8 bytes: `N`, a u64 int, containing the size of the header
 - N bytes: a JSON utf-8 string representing the header.
-  - The header is a dict like `{"TENSOR_NAME": {"dtype": "F16", "shape": [1, 16, 256], "offsets": [BEGIN, END]}, "NEXT_TENSOR_NAME": {...}, ...}`, where offsets point to the tensor data relative to the beginning of the byte buffer, with `BEGIN` as the starting offset and `END` as the one-past offset (so total tensor byte size = `END - BEGIN`).
-  - A special key `__metadata__` is allowed to contain free form text-to-text map.
+  - The header is a dict like `{"TENSOR_NAME": {"dtype": "F16", "shape": [1, 16, 256], "data_offsets": [BEGIN, END]}, "NEXT_TENSOR_NAME": {...}, ...}`, where offsets point to the tensor data relative to the beginning of the byte buffer, with `BEGIN` as the starting offset and `END` as the one-past offset (so total tensor byte size = `END - BEGIN`).
+  - A special key `__metadata__` is allowed to contain free form string-to-string map. Arbitrary JSON is not allowed, all values must be strings.
 - Rest of the file: byte-buffer.
 
 Notes:
  - Duplicate keys are disallowed. Not all parsers may respect this.
  - In general the subset of JSON is implicitly decided by `serde_json` for
  this library. Anything obscure might be modified at a later time, that odd ways
  to represent integer, newlines and escapes in utf-8 strings. This would only
@@ -80,14 +90,16 @@
  - Tensor values are not checked against, in particular NaN and +/-Inf could
  be in the file
  - Empty tensors (tensors with 1 dimension being 0) are allowed.
  They are not storing any data in the databuffer, yet retaining size in the header.
  They don't really bring a lot of values but are accepted since they are valid tensors
  from traditional tensor libraries perspective (torch, tensorflow, numpy, ..).
  - 0-rank Tensors (tensors with shape `[]`) are allowed, they are merely a scalar.
+ - The byte buffer needs to be entirely indexed, and cannot contain holes. This prevents
+ the creation of polyglot files.
 
 
 ### Yet another format ?
 
 The main rationale for this crate is to remove the need to use
 `pickle` on `PyTorch` which is used by default.
 There are other formats out there used by machine learning and more general
```

### Comparing `safetensors-0.3.1rc1/safetensors-lib/benches/benchmark.rs` & `safetensors-0.3.2rc1/safetensors-lib/benches/benchmark.rs`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.1rc1/safetensors-lib/src/lib.rs` & `safetensors-0.3.2rc1/safetensors-lib/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,16 @@
 //![Python documentation](https://huggingface.co/docs/safetensors/index)
 //!
 //!
 //!## Format
 //!
 //! - 8 bytes: `N`, a u64 int, containing the size of the header
 //! - N bytes: a JSON utf-8 string representing the header.
-//!   - The header is a dict like `{"TENSOR_NAME": {"dtype": "F16", "shape": [1, 16, 256], "offsets": [BEGIN, END]}, "NEXT_TENSOR_NAME": {...}, ...}`, where offsets point to the tensor data relative to the beginning of the byte buffer, with `BEGIN` as the starting offset and `END` as the one-past offset (so total tensor byte size = `END - BEGIN`).
-//!   - A special key `__metadata__` is allowed to contain free form text-to-text map.
+//!   - The header is a dict like `{"TENSOR_NAME": {"dtype": "F16", "shape": [1, 16, 256], "data_offsets": [BEGIN, END]}, "NEXT_TENSOR_NAME": {...}, ...}`, where offsets point to the tensor data relative to the beginning of the byte buffer, with `BEGIN` as the starting offset and `END` as the one-past offset (so total tensor byte size = `END - BEGIN`).
+//!   - A special key `__metadata__` is allowed to contain free form string-to-string map. Arbitrary JSON is not allowed, all values must be strings.
 //! - Rest of the file: byte-buffer.
 //!
 //! Notes:
 //!  - Duplicate keys are disallowed. Not all parsers may respect this.
 //!  - In general the subset of JSON is implicitly decided by `serde_json` for
 //!  this library. Anything obscure might be modified at a later time, that odd ways
 //!  to represent integer, newlines and escapes in utf-8 strings. This would only
@@ -67,14 +67,16 @@
 //!  - Tensor values are not checked against, in particular NaN and +/-Inf could
 //!  be in the file
 //!  - Empty tensors (tensors with 1 dimension being 0) are allowed.
 //!  They are not storing any data in the databuffer, yet retaining size in the header.
 //!  They don't really bring a lot of values but are accepted since they are valid tensors
 //!  from traditional tensor libraries perspective (torch, tensorflow, numpy, ..).
 //!  - 0-rank Tensors (tensors with shape `[]`) are allowed, they are merely a scalar.
+//!  - The byte buffer needs to be entirely indexed, and cannot contain holes. This prevents
+//!  the creation of polyglot files.
 //!
 //!
 //!## Yet another format ?
 //!
 //!The main rationale for this crate is to remove the need to use
 //!`pickle` on `PyTorch` which is used by default.
 //!There are other formats out there used by machine learning and more general
```

### Comparing `safetensors-0.3.1rc1/safetensors-lib/src/slice.rs` & `safetensors-0.3.2rc1/safetensors-lib/src/slice.rs`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.1rc1/safetensors-lib/src/tensor.rs` & `safetensors-0.3.2rc1/safetensors-lib/src/tensor.rs`

 * *Files 2% similar despite different names*

```diff
@@ -370,20 +370,32 @@
                 Err(SafeTensorError::TensorNotFound(tensor_name.to_string()))
             }
         } else {
             Err(SafeTensorError::TensorNotFound(tensor_name.to_string()))
         }
     }
 
-    /// Allow the user to get a specific tensor within the SafeTensors.
-    /// The tensor returned is merely a view and the data is not owned by this
-    /// structure.
+    /// Return the names of the tensors within the SafeTensors.
+    /// These are used as keys to access to the actual tensors, that can be
+    /// retrieved using the tensor method.
     pub fn names(&self) -> Vec<&'_ String> {
         self.metadata.index_map.keys().collect()
     }
+
+    /// Return how many tensors are currently stored within the SafeTensors.
+    #[inline]
+    pub fn len(&self) -> usize {
+        self.metadata.tensors.len()
+    }
+
+    /// Indicate if the SafeTensors contains or not any tensor.
+    #[inline]
+    pub fn is_empty(&self) -> bool {
+        self.metadata.tensors.is_empty()
+    }
 }
 
 /// The stuct representing the header of safetensor files which allow
 /// indexing into the raw byte-buffer array and how to interpret it.
 #[derive(Debug, Clone)]
 pub struct Metadata {
     metadata: Option<HashMap<String, String>>,
@@ -941,14 +953,15 @@
 
     #[test]
     fn test_deserialization() {
         let serialized = b"<\x00\x00\x00\x00\x00\x00\x00{\"test\":{\"dtype\":\"I32\",\"shape\":[2,2],\"data_offsets\":[0,16]}}\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00";
 
         let loaded = SafeTensors::deserialize(serialized).unwrap();
 
+        assert_eq!(loaded.len(), 1);
         assert_eq!(loaded.names(), vec!["test"]);
         let tensor = loaded.tensor("test").unwrap();
         assert_eq!(tensor.shape(), vec![2, 2]);
         assert_eq!(tensor.dtype(), Dtype::I32);
         // 16 bytes
         assert_eq!(tensor.data(), b"\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0\0");
     }
```

### Comparing `safetensors-0.3.1rc1/setup.cfg` & `safetensors-0.3.2rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `safetensors-0.3.1rc1/setup.py` & `safetensors-0.3.2rc1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,18 +41,20 @@
 extras["tensorflow"] = deps_list("tensorflow")
 extras["jax"] = deps_list("jax", "flax", "jaxlib")
 extras["paddlepaddle"] = deps_list("paddlepaddle")
 extras["quality"] = deps_list("black", "isort", "flake8", "click")
 extras["testing"] = (
     deps_list("setuptools_rust", "huggingface_hub", "pytest", "pytest-benchmark", "h5py") + extras["numpy"]
 )
+# pinning tf version 2.11.0 for doc-builder
+extras["pinned-tf"] = ["tensorflow==2.11.0"]
 extras["all"] = (
     extras["torch"]
     + extras["numpy"]
-    + extras["tensorflow"]
+    + extras["pinned-tf"]
     + extras["jax"]
     + extras["paddlepaddle"]
     + extras["quality"]
     + extras["testing"]
 )
 extras["dev"] = extras["all"]
```

### Comparing `safetensors-0.3.1rc1/src/lib.rs` & `safetensors-0.3.2rc1/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -372,20 +372,43 @@
                     let size: PyObject = buffer.len().into_py(py);
                     let shared: PyObject = false.into_py(py);
                     let (size_name, storage_name) = if version >= Version::new(2, 0, 0) {
                         (intern!(py, "nbytes"), intern!(py, "UntypedStorage"))
                     } else {
                         (intern!(py, "size"), intern!(py, "ByteStorage"))
                     };
-                    let kwargs =
-                        [(intern!(py, "shared"), shared), (size_name, size)].into_py_dict(py);
-                    let storage = module
-                        .getattr(storage_name)?
-                        .getattr(intern!(py, "from_file"))?
-                        .call((py_filename,), Some(kwargs))?;
+
+                    let sys = PyModule::import(py, intern!(py, "sys"))?;
+                    let byteorder: String = sys.getattr(intern!(py, "byteorder"))?.extract()?;
+
+                    let storage = if byteorder == "big" {
+                        let torch_uint8: PyObject = get_pydtype(module, Dtype::U8)?;
+                        let kwargs = [
+                            (intern!(py, "dtype"), torch_uint8),
+                            (intern!(py, "byte_order"), "big".into_py(py)),
+                        ]
+                        .into_py_dict(py);
+                        let builtins = PyModule::import(py, intern!(py, "builtins"))?;
+                        let py_buffer = builtins
+                            .getattr(intern!(py, "open"))?
+                            .call1((py_filename, intern!(py, "rb")))?
+                            .getattr(intern!(py, "read"))?
+                            .call0()?;
+                        module
+                            .getattr(storage_name)?
+                            .getattr(intern!(py, "from_buffer"))?
+                            .call((py_buffer,), Some(kwargs))?
+                    } else {
+                        let kwargs =
+                            [(intern!(py, "shared"), shared), (size_name, size)].into_py_dict(py);
+                        module
+                            .getattr(storage_name)?
+                            .getattr(intern!(py, "from_file"))?
+                            .call((py_filename,), Some(kwargs))?
+                    };
 
                     let untyped: &PyAny = match storage.getattr(intern!(py, "untyped")) {
                         Ok(untyped) => untyped,
                         Err(_) => storage.getattr(intern!(py, "_untyped"))?,
                     };
                     let storage = untyped.call0()?.into_py(py);
                     let gil_storage = GILOnceCell::new();
@@ -689,14 +712,34 @@
     /// ```
     pub fn get_shape(&self, py: Python) -> PyResult<PyObject> {
         let shape = self.info.shape.clone();
         let shape: PyObject = shape.into_py(py);
         Ok(shape)
     }
 
+    /// Returns the dtype of the full underlying tensor
+    ///
+    /// Returns:
+    ///     (`str`):
+    ///         The dtype of the full tensor
+    ///
+    /// Example:
+    /// ```python
+    /// from safetensors import safe_open
+    ///
+    /// with safe_open("model.safetensors", framework="pt", device=0) as f:
+    ///     tslice = f.get_slice("embedding")
+    ///     dtype = tslice.get_dtype() # "F32"
+    /// ```
+    pub fn get_dtype(&self, py: Python) -> PyResult<PyObject> {
+        let dtype = self.info.dtype;
+        let dtype: PyObject = format!("{:?}", dtype).into_py(py);
+        Ok(dtype)
+    }
+
     pub fn __getitem__(&self, slices: Slice) -> PyResult<PyObject> {
         let slices: Vec<&PySlice> = match slices {
             Slice::Slice(slice) => vec![slice],
             Slice::Slices(slices) => slices,
         };
 
         match &self.storage.as_ref() {
```

