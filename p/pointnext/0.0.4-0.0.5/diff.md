# Comparing `tmp/pointnext-0.0.4.tar.gz` & `tmp/pointnext-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pointnext-0.0.4.tar", last modified: Tue Jul 25 18:18:19 2023, max compression
+gzip compressed data, was "pointnext-0.0.5.tar", last modified: Mon Aug  7 18:04:43 2023, max compression
```

## Comparing `pointnext-0.0.4.tar` & `pointnext-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:18:19.630468 pointnext-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-25 18:16:16.000000 pointnext-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-25 18:16:16.000000 pointnext-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-25 18:18:19.630468 pointnext-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-25 18:16:16.000000 pointnext-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:18:19.626468 pointnext-0.0.4/csrc/
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-25 18:16:16.000000 pointnext-0.0.4/csrc/ball_query.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-25 18:16:16.000000 pointnext-0.0.4/csrc/ball_query_gpu.cu
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-25 18:16:16.000000 pointnext-0.0.4/csrc/ball_query_gpu.h
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-25 18:16:16.000000 pointnext-0.0.4/csrc/cuda_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-25 18:16:16.000000 pointnext-0.0.4/csrc/group_points.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-07-25 18:16:16.000000 pointnext-0.0.4/csrc/group_points_gpu.cu
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-25 18:16:16.000000 pointnext-0.0.4/csrc/group_points_gpu.h
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-25 18:16:16.000000 pointnext-0.0.4/csrc/interpolate.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-07-25 18:16:16.000000 pointnext-0.0.4/csrc/interpolate_gpu.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-25 18:16:16.000000 pointnext-0.0.4/csrc/interpolate_gpu.h
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-25 18:16:16.000000 pointnext-0.0.4/csrc/pointnet2_api.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-25 18:16:16.000000 pointnext-0.0.4/csrc/sampling.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-07-25 18:16:16.000000 pointnext-0.0.4/csrc/sampling_gpu.cu
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-25 18:16:16.000000 pointnext-0.0.4/csrc/sampling_gpu.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:18:19.626468 pointnext-0.0.4/pointnext/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 18:16:16.000000 pointnext-0.0.4/pointnext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-07-25 18:16:16.000000 pointnext-0.0.4/pointnext/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-25 18:16:16.000000 pointnext-0.0.4/pointnext/pointnext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-25 18:16:16.000000 pointnext-0.0.4/pointnext/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:18:19.626468 pointnext-0.0.4/pointnext.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-25 18:18:19.000000 pointnext-0.0.4/pointnext.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-25 18:18:19.000000 pointnext-0.0.4/pointnext.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:18:19.000000 pointnext-0.0.4/pointnext.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-25 18:18:19.000000 pointnext-0.0.4/pointnext.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 18:18:19.000000 pointnext-0.0.4/pointnext.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:18:19.630468 pointnext-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-25 18:16:16.000000 pointnext-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:04:43.587631 pointnext-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-07 18:02:20.000000 pointnext-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-07 18:02:20.000000 pointnext-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-07 18:04:43.587631 pointnext-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-08-07 18:02:20.000000 pointnext-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:04:43.579631 pointnext-0.0.5/csrc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-07 18:02:20.000000 pointnext-0.0.5/csrc/ball_query.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-08-07 18:02:20.000000 pointnext-0.0.5/csrc/ball_query_gpu.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-07 18:02:20.000000 pointnext-0.0.5/csrc/ball_query_gpu.h
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-07 18:02:20.000000 pointnext-0.0.5/csrc/cuda_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-07 18:02:20.000000 pointnext-0.0.5/csrc/group_points.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-08-07 18:02:20.000000 pointnext-0.0.5/csrc/group_points_gpu.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-07 18:02:20.000000 pointnext-0.0.5/csrc/group_points_gpu.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-07 18:02:20.000000 pointnext-0.0.5/csrc/interpolate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-08-07 18:02:20.000000 pointnext-0.0.5/csrc/interpolate_gpu.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-07 18:02:20.000000 pointnext-0.0.5/csrc/interpolate_gpu.h
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-08-07 18:02:20.000000 pointnext-0.0.5/csrc/pointnet2_api.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-07 18:02:20.000000 pointnext-0.0.5/csrc/sampling.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-08-07 18:02:20.000000 pointnext-0.0.5/csrc/sampling_gpu.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-08-07 18:02:20.000000 pointnext-0.0.5/csrc/sampling_gpu.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:04:43.583631 pointnext-0.0.5/pointnext/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-07 18:02:20.000000 pointnext-0.0.5/pointnext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-08-07 18:02:20.000000 pointnext-0.0.5/pointnext/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-08-07 18:02:20.000000 pointnext-0.0.5/pointnext/pointnext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-08-07 18:02:20.000000 pointnext-0.0.5/pointnext/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 18:04:43.587631 pointnext-0.0.5/pointnext.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-07 18:04:43.000000 pointnext-0.0.5/pointnext.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-07 18:04:43.000000 pointnext-0.0.5/pointnext.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 18:04:43.000000 pointnext-0.0.5/pointnext.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-07 18:04:43.000000 pointnext-0.0.5/pointnext.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-07 18:04:43.000000 pointnext-0.0.5/pointnext.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 18:04:43.587631 pointnext-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-08-07 18:02:20.000000 pointnext-0.0.5/setup.py
```

### Comparing `pointnext-0.0.4/LICENSE` & `pointnext-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pointnext-0.0.4/csrc/ball_query.cpp` & `pointnext-0.0.5/csrc/ball_query.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -22,18 +22,17 @@
 		      fprintf(stderr, "%s must be contiguous tensor at %s:%d\n", #x, __FILE__, __LINE__); \
 		      exit(-1); \
 		    } \
 } while (0)
 #define CHECK_INPUT(x) CHECK_CUDA(x);CHECK_CONTIGUOUS(x)
 
 
-int ball_query_wrapper_fast(int b, int n, int m, float radius, int nsample, 
+void ball_query_wrapper_fast(int64_t b, int64_t n, int64_t m, double radius, int64_t nsample,
     at::Tensor new_xyz_tensor, at::Tensor xyz_tensor, at::Tensor idx_tensor) {
     CHECK_INPUT(new_xyz_tensor);
     CHECK_INPUT(xyz_tensor);
     const float *new_xyz = new_xyz_tensor.data<float>();
     const float *xyz = xyz_tensor.data<float>();
     int *idx = idx_tensor.data<int>();
     
     ball_query_kernel_launcher_fast(b, n, m, radius, nsample, new_xyz, xyz, idx);
-    return 1;
 }
```

### Comparing `pointnext-0.0.4/csrc/ball_query_gpu.cu` & `pointnext-0.0.5/csrc/ball_query_gpu.cu`

 * *Files identical despite different names*

### Comparing `pointnext-0.0.4/csrc/group_points.cpp` & `pointnext-0.0.5/csrc/group_points.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -6,30 +6,28 @@
 
 #include <torch/serialize/tensor.h>
 #include <cuda.h>
 #include <cuda_runtime_api.h>
 #include <vector>
 #include "group_points_gpu.h"
 
-int group_points_grad_wrapper_fast(int b, int c, int n, int npoints, int nsample,
+void group_points_grad_wrapper_fast(int64_t b, int64_t c, int64_t n, int64_t npoints, int64_t nsample,
                                    at::Tensor grad_out_tensor, at::Tensor idx_tensor, at::Tensor grad_points_tensor)
 {
 
     float *grad_points = grad_points_tensor.data<float>();
     const int *idx = idx_tensor.data<int>();
     const float *grad_out = grad_out_tensor.data<float>();
 
     group_points_grad_kernel_launcher_fast(b, c, n, npoints, nsample, grad_out, idx, grad_points);
-    return 1;
 }
 
-int group_points_wrapper_fast(int b, int c, int n, int npoints, int nsample,
+void group_points_wrapper_fast(int64_t b, int64_t c, int64_t n, int64_t npoints, int64_t nsample,
                               at::Tensor points_tensor, at::Tensor idx_tensor, at::Tensor out_tensor)
 {
 
     const float *points = points_tensor.data<float>();
     const int *idx = idx_tensor.data<int>();
     float *out = out_tensor.data<float>();
 
     group_points_kernel_launcher_fast(b, c, n, npoints, nsample, points, idx, out);
-    return 1;
 }
```

### Comparing `pointnext-0.0.4/csrc/group_points_gpu.cu` & `pointnext-0.0.5/csrc/group_points_gpu.cu`

 * *Files identical despite different names*

### Comparing `pointnext-0.0.4/csrc/group_points_gpu.h` & `pointnext-0.0.5/csrc/sampling_gpu.h`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,29 @@
-#ifndef _GROUP_POINTS_GPU_H
-#define _GROUP_POINTS_GPU_H
+#ifndef _SAMPLING_GPU_H
+#define _SAMPLING_GPU_H
 
 #include <torch/serialize/tensor.h>
-#include <cuda.h>
-#include <cuda_runtime_api.h>
-#include <vector>
+#include <ATen/cuda/CUDAContext.h>
+#include<vector>
 
 
-int group_points_wrapper_fast(int b, int c, int n, int npoints, int nsample, 
+void gather_points_wrapper_fast(int64_t b, int64_t c, int64_t n, int64_t npoints,
     at::Tensor points_tensor, at::Tensor idx_tensor, at::Tensor out_tensor);
 
-void group_points_kernel_launcher_fast(int b, int c, int n, int npoints, int nsample, 
+void gather_points_kernel_launcher_fast(int b, int c, int n, int npoints, 
     const float *points, const int *idx, float *out);
 
-int group_points_grad_wrapper_fast(int b, int c, int n, int npoints, int nsample, 
+
+void gather_points_grad_wrapper_fast(int64_t b, int64_t c, int64_t n, int64_t npoints,
     at::Tensor grad_out_tensor, at::Tensor idx_tensor, at::Tensor grad_points_tensor);
 
-void group_points_grad_kernel_launcher_fast(int b, int c, int n, int npoints, int nsample, 
+void gather_points_grad_kernel_launcher_fast(int b, int c, int n, int npoints, 
     const float *grad_out, const int *idx, float *grad_points);
 
+
+void furthest_point_sampling_wrapper(int64_t b, int64_t n, int64_t m,
+    at::Tensor points_tensor, at::Tensor temp_tensor, at::Tensor idx_tensor);
+
+void furthest_point_sampling_kernel_launcher(int b, int n, int m, 
+    const float *dataset, float *temp, int *idxs);
+
 #endif
```

### Comparing `pointnext-0.0.4/csrc/interpolate.cpp` & `pointnext-0.0.5/csrc/interpolate.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -13,40 +13,40 @@
 #include <cuda.h>
 #include <cuda_runtime_api.h>
 #include "interpolate_gpu.h"
 
 
 
 
-void three_nn_wrapper_fast(int b, int n, int m, at::Tensor unknown_tensor, 
+void three_nn_wrapper_fast(int64_t b, int64_t n, int64_t m, at::Tensor unknown_tensor,
     at::Tensor known_tensor, at::Tensor dist2_tensor, at::Tensor idx_tensor) {
     const float *unknown = unknown_tensor.data<float>();
     const float *known = known_tensor.data<float>();
     float *dist2 = dist2_tensor.data<float>();
     int *idx = idx_tensor.data<int>();
 
     three_nn_kernel_launcher_fast(b, n, m, unknown, known, dist2, idx);
 }
 
 
-void three_interpolate_wrapper_fast(int b, int c, int m, int n,
+void three_interpolate_wrapper_fast(int64_t b, int64_t c, int64_t m, int64_t n,
                          at::Tensor points_tensor,
                          at::Tensor idx_tensor,
                          at::Tensor weight_tensor,
                          at::Tensor out_tensor) {
 
     const float *points = points_tensor.data<float>();
     const float *weight = weight_tensor.data<float>();
     float *out = out_tensor.data<float>();
     const int *idx = idx_tensor.data<int>();
 
     three_interpolate_kernel_launcher_fast(b, c, m, n, points, idx, weight, out);
 }
 
-void three_interpolate_grad_wrapper_fast(int b, int c, int n, int m,
+void three_interpolate_grad_wrapper_fast(int64_t b, int64_t c, int64_t n, int64_t m,
                             at::Tensor grad_out_tensor,
                             at::Tensor idx_tensor,
                             at::Tensor weight_tensor,
                             at::Tensor grad_points_tensor) {
 
     const float *grad_out = grad_out_tensor.data<float>();
     const float *weight = weight_tensor.data<float>();
```

### Comparing `pointnext-0.0.4/csrc/interpolate_gpu.cu` & `pointnext-0.0.5/csrc/interpolate_gpu.cu`

 * *Files identical despite different names*

### Comparing `pointnext-0.0.4/csrc/interpolate_gpu.h` & `pointnext-0.0.5/csrc/interpolate_gpu.h`

 * *Files 12% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 
 #include <torch/serialize/tensor.h>
 #include<vector>
 #include <cuda.h>
 #include <cuda_runtime_api.h>
 
 
-void three_nn_wrapper_fast(int b, int n, int m, at::Tensor unknown_tensor, 
+void three_nn_wrapper_fast(int64_t b, int64_t n, int64_t m, at::Tensor unknown_tensor,
   at::Tensor known_tensor, at::Tensor dist2_tensor, at::Tensor idx_tensor);
 
 void three_nn_kernel_launcher_fast(int b, int n, int m, const float *unknown,
 	const float *known, float *dist2, int *idx);
 
 
-void three_interpolate_wrapper_fast(int b, int c, int m, int n, at::Tensor points_tensor, 
+void three_interpolate_wrapper_fast(int64_t b, int64_t c, int64_t m, int64_t n, at::Tensor points_tensor,
     at::Tensor idx_tensor, at::Tensor weight_tensor, at::Tensor out_tensor);
 
 void three_interpolate_kernel_launcher_fast(int b, int c, int m, int n, 
     const float *points, const int *idx, const float *weight, float *out);
 
 
-void three_interpolate_grad_wrapper_fast(int b, int c, int n, int m, at::Tensor grad_out_tensor, 
+void three_interpolate_grad_wrapper_fast(int64_t b, int64_t c, int64_t n, int64_t m, at::Tensor grad_out_tensor,
     at::Tensor idx_tensor, at::Tensor weight_tensor, at::Tensor grad_points_tensor);
 
 void three_interpolate_grad_kernel_launcher_fast(int b, int c, int n, int m, const float *grad_out, 
     const int *idx, const float *weight, float *grad_points);
 
 #endif
```

### Comparing `pointnext-0.0.4/csrc/sampling.cpp` & `pointnext-0.0.5/csrc/sampling.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -9,40 +9,37 @@
 #include <ATen/cuda/CUDAContext.h>
 #include <vector>
 #include "sampling_gpu.h"
 
 
 
 
-int gather_points_wrapper_fast(int b, int c, int n, int npoints, 
+void gather_points_wrapper_fast(int64_t b, int64_t c, int64_t n, int64_t npoints,
     at::Tensor points_tensor, at::Tensor idx_tensor, at::Tensor out_tensor){
     const float *points = points_tensor.data<float>();
     const int *idx = idx_tensor.data<int>();
     float *out = out_tensor.data<float>();
 
     gather_points_kernel_launcher_fast(b, c, n, npoints, points, idx, out);
-    return 1;
 }
 
 
-int gather_points_grad_wrapper_fast(int b, int c, int n, int npoints, 
+void gather_points_grad_wrapper_fast(int64_t b, int64_t c, int64_t n, int64_t npoints,
     at::Tensor grad_out_tensor, at::Tensor idx_tensor, at::Tensor grad_points_tensor) {
 
     const float *grad_out = grad_out_tensor.data<float>();
     const int *idx = idx_tensor.data<int>();
     float *grad_points = grad_points_tensor.data<float>();
 
     gather_points_grad_kernel_launcher_fast(b, c, n, npoints, grad_out, idx, grad_points);
-    return 1;
 }
 
 
-int furthest_point_sampling_wrapper(int b, int n, int m, 
+void furthest_point_sampling_wrapper(int64_t b, int64_t n, int64_t m,
     at::Tensor points_tensor, at::Tensor temp_tensor, at::Tensor idx_tensor) {
 
     const float *points = points_tensor.data<float>();
     float *temp = temp_tensor.data<float>();
     int *idx = idx_tensor.data<int>();
 
     furthest_point_sampling_kernel_launcher(b, n, m, points, temp, idx);
-    return 1;
 }
```

### Comparing `pointnext-0.0.4/csrc/sampling_gpu.cu` & `pointnext-0.0.5/csrc/sampling_gpu.cu`

 * *Files identical despite different names*

### Comparing `pointnext-0.0.4/pointnext/ops.py` & `pointnext-0.0.5/pointnext/ops.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # This is adapted from https://github.com/guochengqian/openpoints/blob/2bc0bf9cb2aee0fcd61f6cdc3abca1207e5e809e/models/layers/subsample.py
 from typing import Tuple
 
 import torch
 from torch.autograd import Function
-from pointnext import _C
+from pathlib import Path
+torch.ops.load_library(Path(__file__).parent / '_C.so')
+_C = torch.ops.my_ops
+# from pointnext import _C
 
 
 class FurthestPointSampling(Function):
     @staticmethod
     def forward(ctx, xyz: torch.Tensor, npoint: int) -> torch.Tensor:
         """
         Uses iterative furthest point sampling to select a set of npoint features that have the largest
@@ -17,28 +20,30 @@
         :param npoint: int, number of features in the sampled set
         :return:
              output: (B, m) tensor containing the set (idx)
         """
         assert xyz.is_contiguous()
 
         B, N, _ = xyz.size()
-        # output = torch.cuda.IntTensor(B, npoint, device=xyz.device)
-        # temp = torch.cuda.FloatTensor(B, N, device=xyz.device).fill_(1e10)
-        output = torch.cuda.IntTensor(B, npoint)
-        temp = torch.cuda.FloatTensor(B, N).fill_(1e10)
+        output = torch.zeros(B, npoint, dtype=torch.int32, device=xyz.device)
+        temp = torch.full((B, N), fill_value=1e10, dtype=torch.float32, device=xyz.device)
 
         _C.furthest_point_sampling_wrapper(B, N, npoint, xyz, temp, output)
         return output
 
     @staticmethod
     def backward(xyz, a=None):
         return None, None
 
 
-furthest_point_sample = FurthestPointSampling.apply
+def furthest_point_sample(xyz: torch.Tensor, npoint: int) -> torch.Tensor:
+    if torch.jit.is_scripting() or torch.jit.is_tracing():
+        return FurthestPointSampling.forward(torch.zeros(1), xyz, npoint)
+    else:
+        return FurthestPointSampling.apply(xyz, npoint)
 
 
 class BallQuery(Function):
     @staticmethod
     def forward(ctx, src: torch.Tensor, query: torch.Tensor, radius: float, k: int) -> torch.Tensor:
         """
         :param ctx:
@@ -50,24 +55,29 @@
             idx: (b, m, k) tensor with the indicies of the features that form the query balls
         """
         assert src.is_contiguous()
         assert query.is_contiguous()
 
         b, n, _ = src.size()
         m = query.size(1)
-        idx = torch.cuda.IntTensor(b, m, k, device=src.device).zero_()
+        # idx = torch.cuda.IntTensor(b, m, k, device=src.device).zero_()
+        idx = torch.zeros(b, m, k, dtype=torch.int32, device=src.device)
         _C.ball_query_wrapper(b, n, m, radius, k, query, src, idx)
         return idx
 
     @staticmethod
     def backward(ctx, a=None):
         return None, None, None, None
 
 
-ball_query = BallQuery.apply
+def ball_query(src: torch.Tensor, query: torch.Tensor, radius: float, k: int) -> torch.Tensor:
+    if torch.jit.is_scripting() or torch.jit.is_tracing():
+        return BallQuery.forward(torch.zeros(1), src, query, radius, k)
+    else:
+        return BallQuery.apply(src, query, radius, k)
 
 
 class ThreeNN(Function):
 
     @staticmethod
     def forward(ctx, unknown: torch.Tensor, known: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
         """
@@ -91,15 +101,19 @@
         return torch.sqrt(dist2), idx
 
     @staticmethod
     def backward(ctx, a=None, b=None):
         return None, None
 
 
-three_nn = ThreeNN.apply
+def three_nn(unknown: torch.Tensor, known: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
+    if torch.jit.is_scripting() or torch.jit.is_tracing():
+        return ThreeNN.forward(torch.zeros(1), unknown, known)
+    else:
+        return ThreeNN.apply(unknown, known)
 
 
 class ThreeInterpolate(Function):
 
     @staticmethod
     @torch.cuda.amp.custom_fwd(cast_inputs=torch.float32)
     def forward(ctx, features: torch.Tensor, idx: torch.Tensor, weight: torch.Tensor) -> torch.Tensor:
@@ -140,15 +154,19 @@
         grad_features = torch.zeros([B, c, m], device='cuda', requires_grad=True)
         grad_out_data = grad_out.data.contiguous()
 
         _C.three_interpolate_grad_wrapper(B, c, n, m, grad_out_data, idx, weight, grad_features.data)
         return grad_features, None, None
 
 
-three_interpolate = ThreeInterpolate.apply
+def three_interpolate(features: torch.Tensor, idx: torch.Tensor, weight: torch.Tensor) -> torch.Tensor:
+    if torch.jit.is_scripting() or torch.jit.is_tracing():
+        return ThreeInterpolate.forward(torch.zeros(1), features, idx, weight)
+    else:
+        return ThreeInterpolate.apply(features, idx, weight)
 
 
 def three_interpolation(known_xyz, know_feat, unknown_xyz):
     """
     :param known_xyz: (b, m, 3)
     :param know_feat: (b, c, m)
     :param unknown_xyz: (b, n, 3)
```

### Comparing `pointnext-0.0.4/pointnext/pointnext.py` & `pointnext-0.0.5/pointnext/pointnext.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import torch.nn.functional as F
 
 from einops import repeat, rearrange
 # from .utils import farthest_point_sampling, ball_query_pytorch
 from .ops import ball_query, furthest_point_sample, three_interpolation
 
 
-
 def exists(val):
     return val is not None
 
 
 def default(*vals):
     for val in vals:
         if exists(val):
@@ -164,15 +163,15 @@
                           nn.ReLU())
             for in_d, out_d in zip(dims[:-1], dims[1:])
         ])
 
     def route(self, src_x, src_xyz, dst_x, dst_xyz, neighbor_idx=None, dists=None):
         # use knn and weighted average to get the features
         src_xyz = rearrange(src_xyz, 'b d n -> b n d').contiguous()
-        dst_xyz = rearrange(dst_x, 'b d m -> b m d').contiguous()
+        dst_xyz = rearrange(dst_xyz, 'b d m -> b m d').contiguous()
         lerp_x = three_interpolation(src_xyz, src_x, dst_xyz)
         dst_x = torch.cat([dst_x, lerp_x], dim=1)  # (b, d+d', m)
         return dst_x
 
     def forward(self, x, xyz, sub_x, sub_xyz):
         x = self.route(sub_x, sub_xyz, x, xyz)
         x = self.conv(x)
@@ -187,15 +186,25 @@
             dims=[32, 64, 128, 256, 512],  # dims[0] is the dim of the stem output
             blocks=[4, 7, 4, 4],  # blocks: sa + invres
             strides=[4, 4, 4, 4],
             radius=0.1,
             k=32,
             sa_layers=1,
     ):
+        """
+        :param in_dim: the dim of input features
+        :param dims: dims of each stage
+        :param blocks: number of blocks in each stage
+        :param strides: strides of each stage
+        :param radius: the first radius of sa layer
+        :param k: k at each stage
+        :param sa_layers: number of sa layers in each stage
+        """
         super().__init__()
+        self.encoder_dims = dims
 
         self.stem = nn.Sequential(
             nn.Conv1d(in_dim, dims[0], 1, bias=False),
             nn.BatchNorm1d(dims[0]),
             nn.ReLU()
         )
 
@@ -266,7 +275,27 @@
             out = self.decoder(feats)
         else:
             out = feats[-1][0]
         if exists(category):
             out = out + self.category_emb(category)[:, :, None]
         out = self.head(out)
         return out
+
+
+def pointnext_s(**kwargs):
+    model_kwargs = dict(blocks=[1, 1, 1, 1], sa_layers=2, **kwargs)
+    return PointNextEncoder(**model_kwargs)
+
+
+def pointnext_b(**kwargs):
+    model_kwargs = dict(blocks=[2, 3, 2, 2], sa_layers=1, **kwargs)
+    return PointNextEncoder(**model_kwargs)
+
+
+def pointnext_l(**kwargs):
+    model_kwargs = dict(blocks=[3, 5, 3, 3], sa_layers=1, **kwargs)
+    return PointNextEncoder(**model_kwargs)
+
+
+def pointnext_xl(**kwargs):
+    model_kwargs = dict(dims=[64, 128, 256, 512, 1024], blocks=[4, 7, 4, 4], sa_layers=1, **kwargs)
+    return PointNextEncoder(**model_kwargs)
```

### Comparing `pointnext-0.0.4/pointnext/utils.py` & `pointnext-0.0.5/pointnext/utils.py`

 * *Files identical despite different names*

### Comparing `pointnext-0.0.4/pointnext.egg-info/SOURCES.txt` & `pointnext-0.0.5/pointnext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pointnext-0.0.4/setup.py` & `pointnext-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         include_dirs=[thisdir / 'csrc'],
     )
 ]
 
 setup(
     name='pointnext',
     packages=find_packages(exclude=("csrc")),
-    version='0.0.4',
+    version='0.0.5',
     license='MIT',
     description='PointNext - Pytorch',
     author='Kaidi Shen',
     url='https://github.com/kentechx/pointnext',
     long_description_content_type='text/markdown',
     keywords=[
         '3D segmentation',
@@ -38,14 +38,14 @@
         'point cloud understanding',
     ],
     install_requires=[
         'torch>=1.10',
         'einops>=0.6.1',
     ],
     ext_modules=ext_modules,
-    cmdclass={"build_ext": BuildExtension},
+    cmdclass={"build_ext": BuildExtension.with_options(no_python_abi_suffix=True)},
     classifiers=[
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
     ],
 )
```

