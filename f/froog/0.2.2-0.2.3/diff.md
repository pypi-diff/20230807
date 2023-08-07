# Comparing `tmp/froog-0.2.2.tar.gz` & `tmp/froog-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "froog-0.2.2.tar", last modified: Fri Aug  4 22:30:04 2023, max compression
+gzip compressed data, was "froog-0.2.3.tar", last modified: Mon Aug  7 05:46:00 2023, max compression
```

## Comparing `froog-0.2.2.tar` & `froog-0.2.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-08-04 22:30:04.155346 froog-0.2.2/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       31 2023-07-16 20:10:22.000000 froog-0.2.2/LICENSE
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2498 2023-08-04 22:30:04.155245 froog-0.2.2/PKG-INFO
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2188 2023-08-04 21:49:12.000000 froog-0.2.2/README.md
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-08-04 22:30:04.152846 froog-0.2.2/froog/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       57 2023-07-26 06:32:22.000000 froog-0.2.2/froog/__init__.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2415 2023-08-04 17:46:53.000000 froog-0.2.2/froog/gradcheck.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     1880 2023-08-04 17:50:10.000000 froog-0.2.2/froog/nn.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)    14379 2023-08-04 17:42:33.000000 froog-0.2.2/froog/ops.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     9105 2023-08-04 19:50:36.000000 froog-0.2.2/froog/ops_gpu.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2450 2023-08-04 17:45:44.000000 froog-0.2.2/froog/optim.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     7713 2023-08-04 17:40:03.000000 froog-0.2.2/froog/tensor.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     3140 2023-08-04 19:49:21.000000 froog-0.2.2/froog/utils.py
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-08-04 22:30:04.153521 froog-0.2.2/froog.egg-info/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2498 2023-08-04 22:30:04.000000 froog-0.2.2/froog.egg-info/PKG-INFO
--rw-r--r--   0 kevinbuhler   (501) staff       (20)      396 2023-08-04 22:30:04.000000 froog-0.2.2/froog.egg-info/SOURCES.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)        1 2023-08-04 22:30:04.000000 froog-0.2.2/froog.egg-info/dependency_links.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       15 2023-08-04 22:30:04.000000 froog-0.2.2/froog.egg-info/requires.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)        6 2023-08-04 22:30:04.000000 froog-0.2.2/froog.egg-info/top_level.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       38 2023-08-04 22:30:04.155381 froog-0.2.2/setup.cfg
--rw-r--r--   0 kevinbuhler   (501) staff       (20)      836 2023-08-04 22:29:33.000000 froog-0.2.2/setup.py
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-08-04 22:30:04.154970 froog-0.2.2/tests/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     3172 2023-07-28 03:44:46.000000 froog-0.2.2/tests/test_conv_speed.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     1043 2023-07-28 04:44:12.000000 froog-0.2.2/tests/test_nn.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     4791 2023-08-04 17:47:26.000000 froog-0.2.2/tests/test_ops.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     1987 2023-07-27 02:40:39.000000 froog-0.2.2/tests/test_optim.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2618 2023-07-30 06:46:05.000000 froog-0.2.2/tests/test_tensor.py
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-08-07 05:46:00.966568 froog-0.2.3/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       31 2023-08-07 05:11:02.000000 froog-0.2.3/LICENSE
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2652 2023-08-07 05:46:00.966439 froog-0.2.3/PKG-INFO
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2336 2023-08-07 05:11:02.000000 froog-0.2.3/README.md
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-08-07 05:46:00.964130 froog-0.2.3/froog.egg-info/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2652 2023-08-07 05:46:00.000000 froog-0.2.3/froog.egg-info/PKG-INFO
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)      408 2023-08-07 05:46:00.000000 froog-0.2.3/froog.egg-info/SOURCES.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)        1 2023-08-07 05:46:00.000000 froog-0.2.3/froog.egg-info/dependency_links.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       26 2023-08-07 05:46:00.000000 froog-0.2.3/froog.egg-info/requires.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)        7 2023-08-07 05:46:00.000000 froog-0.2.3/froog.egg-info/top_level.txt
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-08-07 05:46:00.965532 froog-0.2.3/ribbit/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       60 2023-08-07 05:11:02.000000 froog-0.2.3/ribbit/__init__.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2419 2023-08-07 05:11:02.000000 froog-0.2.3/ribbit/gradcheck.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     1881 2023-08-07 05:11:02.000000 froog-0.2.3/ribbit/nn.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)    14381 2023-08-07 05:11:02.000000 froog-0.2.3/ribbit/ops.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)    12902 2023-08-07 05:11:02.000000 froog-0.2.3/ribbit/ops_gpu.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2451 2023-08-07 05:11:02.000000 froog-0.2.3/ribbit/optim.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     7723 2023-08-07 05:11:02.000000 froog-0.2.3/ribbit/tensor.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     3151 2023-08-07 05:11:02.000000 froog-0.2.3/ribbit/utils.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       38 2023-08-07 05:46:00.966601 froog-0.2.3/setup.cfg
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)      858 2023-08-07 05:45:52.000000 froog-0.2.3/setup.py
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-08-07 05:46:00.966268 froog-0.2.3/tests/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     3176 2023-08-07 05:11:02.000000 froog-0.2.3/tests/test_conv_speed.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     4897 2023-08-07 05:11:02.000000 froog-0.2.3/tests/test_models.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     5105 2023-08-07 05:11:02.000000 froog-0.2.3/tests/test_ops.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     1993 2023-08-07 05:11:02.000000 froog-0.2.3/tests/test_optim.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2634 2023-08-07 05:11:02.000000 froog-0.2.3/tests/test_tensor.py
```

### Comparing `froog-0.2.2/PKG-INFO` & `froog-0.2.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,75 @@
 Metadata-Version: 2.1
 Name: froog
-Version: 0.2.2
-Summary: INSANELY SIMPLE AI/ML FRAMEWORK
+Version: 0.2.3
+Summary: a beautifully simplistic ml framework
 Author: Kevin Buhler
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# froog <img src="https://github.com/kevbuh/froog/actions/workflows/test.yml/badge.svg" alt="unit test badge" >
+# ribbit <img src="https://github.com/kevbuh/ribbit/actions/workflows/test.yml/badge.svg" alt="unit test badge" >
 <div align="center" >
-  <img src="https://raw.githubusercontent.com/kevbuh/froog/main/assets/froog.png" alt="froog the frog" height="200">
+  <img src="https://raw.githubusercontent.com/kevbuh/ribbit/main/assets/ribbit.png" alt="ribbit the frog" height="200">
   <br/>
-  FROOG: fast real-time optimization of gradients 
+  ribbit: fast real-time optimization of gradients 
   <br/>
   a beautifully compact machine-learning library
   <br/>
-  <a href="https://github.com/kevbuh/froog">homepage</a> | <a href="https://github.com/kevbuh/froog/tree/main/docs">documentation</a> | <a href="https://pypi.org/project/froog/">pip</a>
+  <a href="https://github.com/kevbuh/ribbit">homepage</a> | <a href="https://github.com/kevbuh/ribbit/tree/main/docs">documentation</a> | <a href="https://pypi.org/project/ribbit/">pip</a>
   <br/>
   <br/>
 </div>
 
-FROOG is a SUPER SIMPLE machine learning framework with the goal of creating tools with AI --> easily and efficiently.
+RIBBIT is a SUPER SIMPLE machine learning framework with the goal of creating tools with AI --> easily and efficiently.
+
+It's an end-to-end framework, encapsulating everything from ensemble trees to deep neural networks (still working on all that lol)
 
 # Installation
 ```bash
-pip install froog
+pip install ribbit
 ```
 
 ### Overview of Features
-- <a href="https://github.com/kevbuh/froog/blob/main/froog/tensor.py">Custom Tensors</a> 
+- <a href="https://github.com/kevbuh/ribbit/blob/main/ribbit/tensor.py">Custom Tensors</a> 
   - Backpropagation
   - Automatic Differentiation (autograd)
       - Forward and backward passes
-- <a href="https://github.com/kevbuh/froog/blob/main/froog/ops.py">Comming ML Operations</a> 
+- <a href="https://github.com/kevbuh/ribbit/blob/main/ribbit/ops.py">ML Operations</a> 
   - 2D Convolutions (im2col)
   - Numerical gradient checking
   - Acceleration methods (Adam)
   - Avg & Max pooling
-- <a href="https://github.com/kevbuh/froog/blob/main/models/efficientnet.py">Efficient-Net</a> inference
-- <a href="https://github.com/kevbuh/froog/blob/main/froog/ops_gpu.py">GPU Support</a> 
-- and a bunch <a href="https://github.com/kevbuh/froog/tree/main/froog">more</a> 
+- <a href="https://github.com/kevbuh/ribbit/blob/main/models/efficientnet.py">EfficientNet</a> inference
+- <a href="https://github.com/kevbuh/ribbit/blob/main/ribbit/ops_gpu.py">GPU Support</a> 
+- and a bunch <a href="https://github.com/kevbuh/ribbit/tree/main/ribbit">more</a> 
 
 ### Sneak Peek
 ```python
-from froog.tensor import Tensor
-from froog.utils import Linear
-import froog.optim as optim
+from ribbit.tensor import Tensor
+from ribbit.utils import Linear
+import ribbit.optim as optim
 
 class mnistMLP:
   def __init__(self):
     self.l1 = Tensor(Linear(784, 128))
     self.l2 = Tensor(Linear(128, 10))
 
   def forward(self, x):
     return x.dot(self.l1).relu().dot(self.l2).logsoftmax()
 
 model = mnistMLP()
 optim = optim.SGD([model.l1, model.l2], lr=0.001)
 ```
 
 # Bounties
-THERES LOT OF STUFF TO WORK ON! VISIT THE <a href="https://github.com/kevbuh/froog/blob/main/docs/bounties.md">BOUNTY SHOP</a>
+THERES LOT OF STUFF TO WORK ON! VISIT THE <a href="https://github.com/kevbuh/ribbit/blob/main/docs/bounties.md">BOUNTY SHOP</a>
 
 Pull requests will be merged if they:
 * increase simplicity
 * increase functionality
 * increase efficiency
 
-more info on <a href="https://github.com/kevbuh/froog/blob/main/docs/contributing.md">contributing</a>
+more info on <a href="https://github.com/kevbuh/ribbit/blob/main/docs/contributing.md">contributing</a>
```

### Comparing `froog-0.2.2/README.md` & `froog-0.2.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,63 @@
-# froog <img src="https://github.com/kevbuh/froog/actions/workflows/test.yml/badge.svg" alt="unit test badge" >
+# ribbit <img src="https://github.com/kevbuh/ribbit/actions/workflows/test.yml/badge.svg" alt="unit test badge" >
 <div align="center" >
-  <img src="https://raw.githubusercontent.com/kevbuh/froog/main/assets/froog.png" alt="froog the frog" height="200">
+  <img src="https://raw.githubusercontent.com/kevbuh/ribbit/main/assets/ribbit.png" alt="ribbit the frog" height="200">
   <br/>
-  FROOG: fast real-time optimization of gradients 
+  ribbit: fast real-time optimization of gradients 
   <br/>
   a beautifully compact machine-learning library
   <br/>
-  <a href="https://github.com/kevbuh/froog">homepage</a> | <a href="https://github.com/kevbuh/froog/tree/main/docs">documentation</a> | <a href="https://pypi.org/project/froog/">pip</a>
+  <a href="https://github.com/kevbuh/ribbit">homepage</a> | <a href="https://github.com/kevbuh/ribbit/tree/main/docs">documentation</a> | <a href="https://pypi.org/project/ribbit/">pip</a>
   <br/>
   <br/>
 </div>
 
-FROOG is a SUPER SIMPLE machine learning framework with the goal of creating tools with AI --> easily and efficiently.
+RIBBIT is a SUPER SIMPLE machine learning framework with the goal of creating tools with AI --> easily and efficiently.
+
+It's an end-to-end framework, encapsulating everything from ensemble trees to deep neural networks (still working on all that lol)
 
 # Installation
 ```bash
-pip install froog
+pip install ribbit
 ```
 
 ### Overview of Features
-- <a href="https://github.com/kevbuh/froog/blob/main/froog/tensor.py">Custom Tensors</a> 
+- <a href="https://github.com/kevbuh/ribbit/blob/main/ribbit/tensor.py">Custom Tensors</a> 
   - Backpropagation
   - Automatic Differentiation (autograd)
       - Forward and backward passes
-- <a href="https://github.com/kevbuh/froog/blob/main/froog/ops.py">Comming ML Operations</a> 
+- <a href="https://github.com/kevbuh/ribbit/blob/main/ribbit/ops.py">ML Operations</a> 
   - 2D Convolutions (im2col)
   - Numerical gradient checking
   - Acceleration methods (Adam)
   - Avg & Max pooling
-- <a href="https://github.com/kevbuh/froog/blob/main/models/efficientnet.py">Efficient-Net</a> inference
-- <a href="https://github.com/kevbuh/froog/blob/main/froog/ops_gpu.py">GPU Support</a> 
-- and a bunch <a href="https://github.com/kevbuh/froog/tree/main/froog">more</a> 
+- <a href="https://github.com/kevbuh/ribbit/blob/main/models/efficientnet.py">EfficientNet</a> inference
+- <a href="https://github.com/kevbuh/ribbit/blob/main/ribbit/ops_gpu.py">GPU Support</a> 
+- and a bunch <a href="https://github.com/kevbuh/ribbit/tree/main/ribbit">more</a> 
 
 ### Sneak Peek
 ```python
-from froog.tensor import Tensor
-from froog.utils import Linear
-import froog.optim as optim
+from ribbit.tensor import Tensor
+from ribbit.utils import Linear
+import ribbit.optim as optim
 
 class mnistMLP:
   def __init__(self):
     self.l1 = Tensor(Linear(784, 128))
     self.l2 = Tensor(Linear(128, 10))
 
   def forward(self, x):
     return x.dot(self.l1).relu().dot(self.l2).logsoftmax()
 
 model = mnistMLP()
 optim = optim.SGD([model.l1, model.l2], lr=0.001)
 ```
 
 # Bounties
-THERES LOT OF STUFF TO WORK ON! VISIT THE <a href="https://github.com/kevbuh/froog/blob/main/docs/bounties.md">BOUNTY SHOP</a>
+THERES LOT OF STUFF TO WORK ON! VISIT THE <a href="https://github.com/kevbuh/ribbit/blob/main/docs/bounties.md">BOUNTY SHOP</a>
 
 Pull requests will be merged if they:
 * increase simplicity
 * increase functionality
 * increase efficiency
 
-more info on <a href="https://github.com/kevbuh/froog/blob/main/docs/contributing.md">contributing</a>
+more info on <a href="https://github.com/kevbuh/ribbit/blob/main/docs/contributing.md">contributing</a>
```

### Comparing `froog-0.2.2/froog/gradcheck.py` & `froog-0.2.3/ribbit/gradcheck.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # |    ___||   | ||  |   _   ||   _   ||    ___|
 # |   |___ |   |_||_ |  | |  ||  | |  ||   | __ 
 # |    ___||    __  ||  |_|  ||  |_|  ||   ||  |
 # |   |    |   |  | ||       ||       ||   |_| |
 # |___|    |___|  |_||_______||_______||_______|
 
 import numpy as np
-from froog.tensor import Tensor
-from froog.utils import mask_like
+from ribbit.tensor import Tensor
+from ribbit.utils import mask_like
 
 def jacobian(model, input):
   output = model(input)
 
   ji = input.data.reshape(-1).shape[-1]  # jacobian of input
   jo = output.data.reshape(-1).shape[-1] # jacobian of output
   J = np.zeros((jo, ji), dtype=np.float32)
@@ -26,15 +26,15 @@
 
 def numerical_jacobian(model, input, eps = 1e-6):
 #     """
 #     https://timvieira.github.io/blog/post/2017/04/21/how-to-test-gradient-implementations/
 #     Computes :
 #         First-order partial derivatives using Finite-Difference Approximation with Central Difference Method (CDM)
 #     Params:
-#         model : A froog model
+#         model : A ribbit model
 #         input : An input
 #         eps   : Perturbation step
 #     Returns:
 #         NJ    : an approx. of the Jacobian
 #     """
   output = model(input)
 
@@ -54,15 +54,15 @@
 
   return NJ
 
 def gradcheck(model, input, eps = 1e-06, atol = 1e-5, rtol = 0.001):
   """
   Checks whether computed gradient is close to numerical approximation of the Jacobian
   Params:
-    model       : froog model   
+    model       : ribbit model   
     eps         : eps used to see if gradient is within tolerances
     atol        : absolute tolerance
     rtol        : relative tolerance 
   Returns:
     test_passed : bool of whether the test passed
   """
   NJ = numerical_jacobian(model, input, eps)
```

### Comparing `froog-0.2.2/froog/nn.py` & `froog-0.2.3/ribbit/nn.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # |       ||    _ |  |       ||       ||       |
 # |    ___||   | ||  |   _   ||   _   ||    ___|
 # |   |___ |   |_||_ |  | |  ||  | |  ||   | __ 
 # |    ___||    __  ||  |_|  ||  |_|  ||   ||  |
 # |   |    |   |  | ||       ||       ||   |_| |
 # |___|    |___|  |_||_______||_______||_______|
 
-from froog.tensor import Tensor
+from ribbit.tensor import Tensor
 
 def swish(x):
   return x.mul(x.sigmoid())
 
 # *************************************
 #     _   ___   __   ____  ____  _____
 #    / | / / | / /  / __ \/ __ \/ ___/
@@ -40,15 +40,15 @@
     self.eps = eps
     self.weight = Tensor.zeros(sz)
     self.bias = Tensor.zeros(sz)
 
     # TODO: need running_mean and running_var
     self.running_mean = Tensor.zeros(sz)
     self.running_var = Tensor.zeros(sz)
-    self.num_batches_tracked = Tensor.zeros(0)
+    self.num_batches_tracked = Tensor.zeros(1)
 
   def __call__(self, x):
     x = x.sub(self.running_mean.reshape(shape=[1, -1, 1, 1]))
     x = x.mul(self.weight.reshape(shape=[1, -1, 1, 1]))
     x = x.div(self.running_var.add(Tensor([self.eps])).reshape(shape=[1, -1, 1, 1]).sqrt()) # TODO: shouldn't div go first?
     x = x.add(self.bias.reshape(shape=[1, -1, 1, 1]))
     return x
```

### Comparing `froog-0.2.2/froog/ops.py` & `froog-0.2.3/ribbit/ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # |    ___||   | ||  |   _   ||   _   ||    ___|
 # |   |___ |   |_||_ |  | |  ||  | |  ||   | __ 
 # |    ___||    __  ||  |_|  ||  |_|  ||   ||  |
 # |   |    |   |  | ||       ||       ||   |_| |
 # |___|    |___|  |_||_______||_______||_______|
 
 import numpy as np
-from froog.tensor import Function, register
-from froog.utils import im2col, col2im
+from ribbit.tensor import Function, register
+from ribbit.utils import im2col, col2im
 
 # *****************************************************
 #     ____  ___   _____ __________   ____  ____  _____
 #    / __ )/   | / ___//  _/ ____/  / __ \/ __ \/ ___/
 #   / __  / /| | \__ \ / // /      / / / / /_/ /\__ \ 
 #  / /_/ / ___ |___/ // // /___   / /_/ / ____/___/ / 
 # /_____/_/  |_/____/___/\____/   \____/_/    /____/
```

### Comparing `froog-0.2.2/froog/ops_gpu.py` & `froog-0.2.3/ribbit/ops_gpu.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,103 +15,105 @@
 
 def buffer_new(ctx, shape):
   res_g = cl.Buffer(ctx.cl_ctx, cl.mem_flags.WRITE_ONLY, 4*np.prod(shape))
   res_g.shape = shape
   res_g.dtype = np.float32
   return res_g
 
+def buffer_zeros(ctx, shape):
+  res_g = cl.Buffer(ctx.cl_ctx, cl.mem_flags.WRITE_ONLY | cl.mem_flags.COPY_HOST_PTR, hostbuf=np.zeros(shape))
+  res_g.shape = shape
+  res_g.dtype = np.float32
+  return res_g
+
 def buffer_like(ctx, x):
   return buffer_new(ctx, x.shape)
 
 @functools.lru_cache
 def clbuild(cl_ctx, prg):
   return cl.Program(cl_ctx, prg).build()
 
 def binary_op(ctx, code, x, y): 
+  if x.shape != y.shape:
+    raise Exception(f"binary op shape mismatch: {x.shape} != {y.shape}")
   ret = buffer_like(ctx, x)
   prg = clbuild(ctx.cl_ctx, """
-  __kernel void add(
+  __kernel void binop(
       __global const float *a_g, __global const float *b_g, __global float *res_g)
   {
     int gid = get_global_id(0);
-    """+code+"""
+    float a = a_g[gid];
+    float b = b_g[gid];
+    res_g[gid] = """+code+""";
   }
   """)
-  prg.add(ctx.cl_queue, [np.prod(ret.shape)], None, x, y, ret) # (queue, size, ???, arg1, arg2, dest)
+  prg.binop(ctx.cl_queue, [np.prod(ret.shape)], None, x, y, ret) # (queue, size, ???, arg1, arg2, dest)
   return ret
 
 def unary_op(ctx, code, x):
   ret = buffer_like(ctx, x)
   prg = clbuild(ctx.cl_ctx, """
-  __kernel void relu(
+  __kernel void unop(
       __global const float *a_g, __global float *res_g)
   {
     int gid = get_global_id(0);
-    """+code+"""
+    float a = a_g[gid];
+    res_g[gid] = """+code+"""
   }
   """)
-  prg.relu(ctx.cl_queue, [np.prod(ret.shape)], None, x, ret)
+  prg.unop(ctx.cl_queue, [np.prod(ret.shape)], None, x, ret)
   return ret
 
 class Add(Function):
   @staticmethod
   def forward(ctx, x, y):
-    return binary_op(ctx, 'res_g[gid] = a_g[gid] + b_g[gid];', x, y)
+    return binary_op(ctx, 'a+b', x, y)
 
   @staticmethod
   def backward(ctx, grad_output):
     return grad_output, grad_output
 register('add', Add, gpu=True)
 
 class Sub(Function):
   @staticmethod
   def forward(ctx, x, y):
-    return binary_op(ctx, 'res_g[gid] = a_g[gid] - b_g[gid];', x, y)
+    return binary_op(ctx, 'a-b', x, y)
 
   @staticmethod
   def backward(ctx, grad_output):
-    not_grad_output = unary_op(ctx, 'res_g[gid] = -a_g[gid];', grad_output)
+    not_grad_output = unary_op(ctx, '-a', grad_output)
     return grad_output, not_grad_output
 register('sub', Sub, gpu=True)
 
 class Mul(Function):
   @staticmethod
   def forward(ctx, x, y):
     ctx.save_for_backward(x, y)
 
-    # HACK
-    if y.shape == (1,):
-      return binary_op(ctx, 'res_g[gid] = a_g[gid] * b_g[0];', x, y)
-    elif x.shape == y.shape:
-      return binary_op(ctx, 'res_g[gid] = a_g[gid] * b_g[gid];', x, y)
-    else:
-      raise Exception("mismatched shapes %r %r" % (x.shape, y.shape))
-
-    return ret
+    return binary_op(ctx, 'a*b', x, y)
 
   @staticmethod
   def backward(ctx, grad_output):
     x,y = ctx.saved_tensors
-    return binary_op(ctx, 'res_g[gid] = a_g[gid] * b_g[gid];', y, grad_output),\
-           binary_op(ctx, 'res_g[gid] = a_g[gid] * b_g[gid];', x, grad_output)
+    return binary_op(ctx, 'a*b', y, grad_output), binary_op(ctx, 'a*b', x, grad_output)
 register('mul', Mul, gpu=True)
 
 class Pow(Function):
   @staticmethod
   def forward(ctx, x, y):
     ctx.save_for_backward(x, y)
-    return binary_op(ctx, 'res_g[gid] = pow(a_g[gid], b_g[gid]);', x, y)
+    return binary_op(ctx, 'pow(a,b)', x, y)
 
   @staticmethod
   def backward(ctx, grad_output):
     x,y = ctx.saved_tensors
-    gradx = binary_op(ctx, 'res_g[gid] = a_g[gid] * b_g[gid];', grad_output,
-                      binary_op(ctx, 'res_g[gid] = b_g[gid] * (pow((float)a_g[gid], (float)(b_g[gid]-1.0)));', x, y))
-    grady = binary_op(ctx, 'res_g[gid] = a_g[gid] * b_g[gid];', grad_output,
-                      binary_op(ctx, 'res_g[gid] = pow((float)a_g[gid], (float)b_g[gid]) * log(a_g[gid]);', x, y))
+    gradx = binary_op(ctx, 'a*b', grad_output,
+                      binary_op(ctx, 'b * (pow((float)a, (float)(b-1.0)));', x, y))
+    grady = binary_op(ctx, 'a*b', grad_output,
+                      binary_op(ctx, 'pow((float)a, (float)b) * log(a);', x, y))
     return gradx, grady
 register('pow', Pow, gpu=True)
 
 class Sum(Function):
   @staticmethod
   def forward(ctx, input):
     ctx.save_for_backward(input)
@@ -129,15 +131,25 @@
     """)
     prg.sum(ctx.cl_queue, [input.shape[0]], None, input, np.int32(np.prod(input.shape)), ret)
     return ret
 
   @staticmethod
   def backward(ctx, grad_output):
     input, = ctx.saved_tensors
-    return binary_op(ctx, 'res_g[gid] = b_g[0];', input, grad_output)  # Quick hack for fill
+    ret = buffer_like(ctx, input)
+    prg = clbuild(ctx.cl_ctx, """
+    __kernel void fill(
+        __global const float *a_g, __global float *res_g)
+    {
+      int gid = get_global_id(0);
+      res_g[gid] = a_g[0];
+    }
+    """)
+    prg.fill(ctx.cl_queue, [np.prod(ret.shape)], None, grad_output, ret)
+    return ret
 register('sum', Sum, gpu=True)
 
 class Dot(Function):
   """
   A[gid_y * size + i] accesses an element in the row gid_y of matrix A and the column i
   """
   @staticmethod
@@ -206,15 +218,26 @@
 
 # ***** SIMPLE OPS ********
 
 class Reshape(Function):
   @staticmethod
   def forward(ctx, x, shape):
     ctx.save_for_backward(x.shape)
-    x.shape = shape
+    ss = list(shape)
+
+    # ???
+    tsum = 1
+    for s in ss:
+      if s != -1:
+        tsum *= s
+    for i,s in enumerate(ss):
+      if s == -1:
+        ss[i] = np.prod(x.shape) // tsum
+    assert np.prod(x.shape) == np.prod(ss)
+    x.shape = tuple(ss)
     return x
 
   @staticmethod
   def backward(ctx, grad_output):
     in_shape, = ctx.saved_tensors
     grad_output.shape = in_shape
     return grad_output
@@ -222,20 +245,20 @@
 
 # ***** ACTIVATION OPS ********
 
 class ReLU(Function):
   @staticmethod
   def forward(ctx, input):
     ctx.save_for_backward(input)
-    return unary_op(ctx, 'res_g[gid] = max(a_g[gid], (float)0.);', input)
+    return unary_op(ctx, 'max(a, (float)0.);', input)
 
   @staticmethod
   def backward(ctx, grad_output):
     input, = ctx.saved_tensors
-    return binary_op(ctx, 'res_g[gid] = a_g[gid] * (b_g[gid] >= 0);', grad_output, input)
+    return binary_op(ctx, 'a * (b >= 0);', grad_output, input)
 register('relu', ReLU, gpu=True)
 
 class LogSoftmax(Function):
   @staticmethod
   def forward(ctx, input):
     lsum = buffer_new(ctx, (input.shape[0],))
     prg = clbuild(ctx.cl_ctx, """
@@ -290,7 +313,121 @@
     """)
     prg.lsmsub2(ctx.cl_queue, [grad_output.shape[0], grad_output.shape[1]], None,
       grad_output, output, np.int32(grad_output.shape[1]), grad_input)
 
     return grad_input
 register('logsoftmax', LogSoftmax, gpu=True)
 
+# ***** CONV OPS ********
+
+class Conv2D(Function):
+  @staticmethod
+  def forward(ctx, x, w, stride=1, groups=1):
+    if type(ctx.stride) == int:     # ctx stores function params
+      ctx.stride = (ctx.stride, ctx.stride)
+
+    cout, cin, H, W = w.shape
+    y_stride, x_stride = ctx.stride
+    bs,cin_,iy,ix = x.shape
+    oy,ox = (iy-(H-y_stride))//y_stride, (ix-(W-x_stride))//x_stride
+    
+    assert cin*ctx.groups == cin_
+    assert cout % ctx.groups == 0
+
+    rcout = cout//ctx.groups
+
+    # output buffer
+    ret = buffer_new(ctx, (bs, cout, oy, ox))
+    prg = clbuild(ctx.cl_ctx, """
+
+    __kernel void conv(__global const float *input, __global const float *weight, __global float *output,
+      int H, int W, int groups, int rcout, int cin, int oy, int ox, int iy, int ix, int ys, int xs) {
+
+      int B = get_global_id(0);  // range 0-bs
+      int Y = get_global_id(1);  // range 0-oy
+      int X = get_global_id(2);  // range 0-ox
+      int IY = Y*ys;
+      int IX = X*xs;
+      
+      // input  = (bs, groups, cin, iy, ix)
+      // weight = (groups, rcout, cin, H, W)
+      // output = (bs, groups, rcout, oy, ox)
+      for (int g = 0; g < groups; g++) {
+        for (int c = 0; c < rcout; c++) {
+          float acc = 0.0;
+          for (int ci = 0; ci < cin; ci++) {
+            for (int y = IY; y < IY+H; y++) {
+              for (int x = IX; x < IX+W; x++) {
+                acc += input[B*groups*cin*iy*ix + g*cin*iy*ix + ci*iy*ix + y*ix + x] * \
+                  weight[g*rcout*cin*H*W + c*cin*H*W + ci*H*W + (y-IY)*W + (x-IX)];
+              }
+            }
+          }
+          output[B*groups*rcout*oy*ox + g*rcout*oy*ox + c*oy*ox + Y*ox + X] = acc;
+        }
+      }
+    }
+    """)
+
+    prg.conv(ctx.cl_queue, [bs, oy, ox], None,
+      x, w, ret,
+      np.int32(H), np.int32(W),
+      np.int32(groups), np.int32(rcout), np.int32(cin),
+      np.int32(oy), np.int32(ox), 
+      np.int32(iy), np.int32(ix),
+      np.int32(y_stride), np.int32(x_stride)
+    )
+    return ret
+
+  @staticmethod
+  def backward(ctx, grad_output):
+    raise Exception("not implemented")
+
+register('conv2d', Conv2D, gpu=True)
+
+class Pad2D(Function):
+  @staticmethod
+  def forward(ctx, x, padding=None):
+    bs,cin,iy,ix = x.shape
+    oy,ox = iy+padding[0]+padding[1], ix+padding[2]+padding[3] # top, bottom, left, right
+    ret = buffer_zeros(ctx, (bs, cin, oy, ox))
+
+    prg = clbuild(ctx.cl_ctx, """
+    __kernel void pad2d(
+        __global const float *input, __global float *output,
+        int cin, int py, int px, int oy, int ox, int iy, int ix
+      )
+    {
+      int B = get_global_id(0);
+      int C = get_global_id(1);
+      int Y = get_global_id(2);
+      int iptr = B*cin*iy*ix + C*iy*ix + Y*ix;
+      int optr = B*cin*oy*ox + C*oy*ox + (Y+py)*ox + px;
+      for (int x = 0; x < ix; x++) {
+        output[optr+x] = input[iptr+x];
+      }
+    }
+    """)
+    prg.pad2d(ctx.cl_queue, [bs, cin, iy], None,
+        x, ret,
+        np.int32(cin), np.int32(padding[0]), np.int32(padding[2]),
+        np.int32(oy), np.int32(ox), np.int32(iy), np.int32(ix)
+      )
+    return ret
+
+  @staticmethod
+  def backward(ctx, grad_output):
+    raise Exception("write this")
+register('pad2d', Pad2D, gpu=True)
+
+class Sigmoid(Function):
+  @staticmethod
+  def forward(ctx, input):
+    ret = unary_op(ctx, '1./(1+exp(-a))', input)
+    ctx.save_for_backward(ret)
+    return ret
+
+  @staticmethod
+  def backward(ctx, grad_output):
+    ret, = ctx.saved_tensors
+    return binary_op(ctx, 'a * (b * (1 - b));', grad_output, ret)
+register('sigmoid', Sigmoid, gpu=True)
```

### Comparing `froog-0.2.2/froog/optim.py` & `froog-0.2.3/ribbit/optim.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # |    ___||   | ||  |   _   ||   _   ||    ___|
 # |   |___ |   |_||_ |  | |  ||  | |  ||   | __ 
 # |    ___||    __  ||  |_|  ||  |_|  ||   ||  |
 # |   |    |   |  | ||       ||       ||   |_| |
 # |___|    |___|  |_||_______||_______||_______|
 
 import numpy as np
-from froog.tensor import Tensor, GPU
+from ribbit.tensor import Tensor, GPU
 
 class Optimizer:
   def __init__(self, params):
     self.params = params
 
 class SGD(Optimizer):
   """
```

### Comparing `froog-0.2.2/froog/tensor.py` & `froog-0.2.3/ribbit/tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,15 @@
   def to_gpu(self):
     if not GPU:
       raise Exception("no gpu support! install pyopencl")
     if not self.gpu:
       init_gpu()
       assert self.data.dtype == np.float32 # GPU only allows float32
       # hostbuf is the data buffer on host machine with the data to be copied to the OpenCL buffer
-      data = cl.Buffer(cl_ctx, cl.mem_flags.READ_ONLY | cl.mem_flags.COPY_HOST_PTR, hostbuf=self.data) # from pyopencl docs
+      data = cl.Buffer(cl_ctx, cl.mem_flags.READ_ONLY | cl.mem_flags.COPY_HOST_PTR, hostbuf=self.data.ravel()) # from pyopencl docs
       data.shape = self.shape
       data.dtype = self.data.dtype
       ret = Tensor(data)
       if self.grad:
         ret.grad = self.grad.to_gpu()
       return ret
     else:
@@ -228,10 +228,10 @@
   
   setattr(Tensor, name, dispatch)
 
   if name in ['add', 'sub', 'mul', 'div']:
     setattr(Tensor, "__%s__" % name, dispatch)
     setattr(Tensor, "__i%s__" % name, lambda self,x: self.assign(dispatch(self,x)))
 
-import froog.ops # this registers all the operations
+import ribbit.ops # this registers all the operations
 if GPU:
-  import froog.ops_gpu
+  import ribbit.ops_gpu
```

### Comparing `froog-0.2.2/froog/utils.py` & `froog-0.2.3/ribbit/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 # |    ___||   | ||  |   _   ||   _   ||    ___|
 # |   |___ |   |_||_ |  | |  ||  | |  ||   | __ 
 # |    ___||    __  ||  |_|  ||  |_|  ||   ||  |
 # |   |    |   |  | ||       ||       ||   |_| |
 # |___|    |___|  |_||_______||_______||_______|
 
 import numpy as np
+import os
 from functools import lru_cache
 
 def Linear(*tensor_size):
   # TODO: why dividing by sqrt?
   ret = np.random.uniform(-1., 1., size=tensor_size)/np.sqrt(np.prod(tensor_size)) # random init weights
   return ret.astype(np.float32)
 
 def fetch(url):
   import requests, os, hashlib, tempfile
   fp = os.path.join(tempfile.gettempdir(), hashlib.md5(url.encode('utf-8')).hexdigest())
-  if os.path.isfile(fp):
+  if os.path.isfile(fp) and os.stat(fp).st_size > 0:
     print(f"opening cache from {url}...")
     with open(fp, "rb") as f:
       dat = f.read()
   else:
     print(f"fetching {url}")
     dat = requests.get(url).content
     with open(fp+".tmp", "wb") as f:
@@ -48,15 +49,14 @@
   idx_channel = np.tile(np.arange(cin).repeat(H*W), oy*ox)
   idx_y = np.tile(np.arange(H).repeat(W), oy*ox*cin) + np.arange(oy).repeat(ox*cin*H*W)
   idx_x = np.tile(np.arange(W), oy*ox*cin*H) + np.tile(np.arange(ox), oy).repeat(cin*H*W)
   OY, OX = oy+(H-1), ox+(W-1)
   idx = idx_channel * OY * OX + idx_y * OX + idx_x
   return idx
 
-# TODO: whats this doing? 
 @lru_cache
 def rearrange_col2im_index(oy, ox, cin, H, W):
   idx = get_im2col_index(oy, ox, cin, H, W)
   r_idx = np.zeros((np.max(idx)+1, H*W), dtype=idx.dtype)-1
   for i,x in enumerate(idx):
     for j in range(H*W):
       if r_idx[x,j] == -1:
```

### Comparing `froog-0.2.2/froog.egg-info/PKG-INFO` & `froog-0.2.3/froog.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,75 @@
 Metadata-Version: 2.1
 Name: froog
-Version: 0.2.2
-Summary: INSANELY SIMPLE AI/ML FRAMEWORK
+Version: 0.2.3
+Summary: a beautifully simplistic ml framework
 Author: Kevin Buhler
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# froog <img src="https://github.com/kevbuh/froog/actions/workflows/test.yml/badge.svg" alt="unit test badge" >
+# ribbit <img src="https://github.com/kevbuh/ribbit/actions/workflows/test.yml/badge.svg" alt="unit test badge" >
 <div align="center" >
-  <img src="https://raw.githubusercontent.com/kevbuh/froog/main/assets/froog.png" alt="froog the frog" height="200">
+  <img src="https://raw.githubusercontent.com/kevbuh/ribbit/main/assets/ribbit.png" alt="ribbit the frog" height="200">
   <br/>
-  FROOG: fast real-time optimization of gradients 
+  ribbit: fast real-time optimization of gradients 
   <br/>
   a beautifully compact machine-learning library
   <br/>
-  <a href="https://github.com/kevbuh/froog">homepage</a> | <a href="https://github.com/kevbuh/froog/tree/main/docs">documentation</a> | <a href="https://pypi.org/project/froog/">pip</a>
+  <a href="https://github.com/kevbuh/ribbit">homepage</a> | <a href="https://github.com/kevbuh/ribbit/tree/main/docs">documentation</a> | <a href="https://pypi.org/project/ribbit/">pip</a>
   <br/>
   <br/>
 </div>
 
-FROOG is a SUPER SIMPLE machine learning framework with the goal of creating tools with AI --> easily and efficiently.
+RIBBIT is a SUPER SIMPLE machine learning framework with the goal of creating tools with AI --> easily and efficiently.
+
+It's an end-to-end framework, encapsulating everything from ensemble trees to deep neural networks (still working on all that lol)
 
 # Installation
 ```bash
-pip install froog
+pip install ribbit
 ```
 
 ### Overview of Features
-- <a href="https://github.com/kevbuh/froog/blob/main/froog/tensor.py">Custom Tensors</a> 
+- <a href="https://github.com/kevbuh/ribbit/blob/main/ribbit/tensor.py">Custom Tensors</a> 
   - Backpropagation
   - Automatic Differentiation (autograd)
       - Forward and backward passes
-- <a href="https://github.com/kevbuh/froog/blob/main/froog/ops.py">Comming ML Operations</a> 
+- <a href="https://github.com/kevbuh/ribbit/blob/main/ribbit/ops.py">ML Operations</a> 
   - 2D Convolutions (im2col)
   - Numerical gradient checking
   - Acceleration methods (Adam)
   - Avg & Max pooling
-- <a href="https://github.com/kevbuh/froog/blob/main/models/efficientnet.py">Efficient-Net</a> inference
-- <a href="https://github.com/kevbuh/froog/blob/main/froog/ops_gpu.py">GPU Support</a> 
-- and a bunch <a href="https://github.com/kevbuh/froog/tree/main/froog">more</a> 
+- <a href="https://github.com/kevbuh/ribbit/blob/main/models/efficientnet.py">EfficientNet</a> inference
+- <a href="https://github.com/kevbuh/ribbit/blob/main/ribbit/ops_gpu.py">GPU Support</a> 
+- and a bunch <a href="https://github.com/kevbuh/ribbit/tree/main/ribbit">more</a> 
 
 ### Sneak Peek
 ```python
-from froog.tensor import Tensor
-from froog.utils import Linear
-import froog.optim as optim
+from ribbit.tensor import Tensor
+from ribbit.utils import Linear
+import ribbit.optim as optim
 
 class mnistMLP:
   def __init__(self):
     self.l1 = Tensor(Linear(784, 128))
     self.l2 = Tensor(Linear(128, 10))
 
   def forward(self, x):
     return x.dot(self.l1).relu().dot(self.l2).logsoftmax()
 
 model = mnistMLP()
 optim = optim.SGD([model.l1, model.l2], lr=0.001)
 ```
 
 # Bounties
-THERES LOT OF STUFF TO WORK ON! VISIT THE <a href="https://github.com/kevbuh/froog/blob/main/docs/bounties.md">BOUNTY SHOP</a>
+THERES LOT OF STUFF TO WORK ON! VISIT THE <a href="https://github.com/kevbuh/ribbit/blob/main/docs/bounties.md">BOUNTY SHOP</a>
 
 Pull requests will be merged if they:
 * increase simplicity
 * increase functionality
 * increase efficiency
 
-more info on <a href="https://github.com/kevbuh/froog/blob/main/docs/contributing.md">contributing</a>
+more info on <a href="https://github.com/kevbuh/ribbit/blob/main/docs/contributing.md">contributing</a>
```

### Comparing `froog-0.2.2/setup.py` & `froog-0.2.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 
 #!/usr/bin/env python3
-# this file specifies how the froog package is installed, including any necessary dependencies required to run
+# this file specifies how the ribbit package is installed, including any necessary dependencies required to run
 
 import os
 from setuptools import setup
 
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
   long_description = f.read()
 
 setup(name='froog',
-      version='0.2.2',
-      description='INSANELY SIMPLE AI/ML FRAMEWORK',
+      version='0.2.3',
+      description='a beautifully simplistic ml framework',
       author='Kevin Buhler',
       license='MIT',
       long_description=long_description,
       long_description_content_type='text/markdown',
-      packages = ['froog'],
+      packages = ['ribbit'],
       classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License"
       ],
-      install_requires=['numpy', 'requests'],
+      install_requires=['numpy', 'requests', 'matplotlib'],
       python_requires='>=3.8',
       include_package_data=True)
```

### Comparing `froog-0.2.2/tests/test_conv_speed.py` & `froog-0.2.3/tests/test_conv_speed.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 import cProfile
 import unittest
-from froog.tensor import Tensor
+from ribbit.tensor import Tensor
 import pstats
 import numpy as np
 import torch
 
 def start_profile():
   import time
   # multiplying by 1e9 converts seconds to nanoseconds
@@ -62,15 +62,15 @@
 
     self.fpt_baseline = (fpt*1000)/cnt
     self.bpt_baseline = (bpt*1000)/cnt
     print(f"avg torch forward pass : {self.fpt_baseline:.3f} ms")
     print(f"avg torch backward pass: {self.bpt_baseline:.3f} ms")
     print(tprof.key_averages().table(sort_by="self_cpu_time_total", row_limit=20))
 
-    # ****** froog results ******
+    # ****** ribbit results ******
 
     c1 = Tensor(c1.detach().numpy()) # detach from torch, turn into numpy array
     c2 = Tensor(c2.detach().numpy())
     l1 = Tensor(l1.detach().numpy())
 
     cnt = num_time
     fpt, bpt = 0.0, 0.0
@@ -90,13 +90,13 @@
       else:
         fpt += (et1-et0)
         bpt += (et2-et1)
 
     stop_profile(pr, sort='time')
     fpt = fpt*1000/cnt
     bpt = bpt*1000/cnt
-    print(f"avg froog forward pass:  {float(fpt):.3f} ms, {float(fpt/self.fpt_baseline):.2f}x off baseline of {self.fpt_baseline:.3f} ms")
-    print(f"avg froog backward pass: {float(bpt):.3f} ms, {float(fpt/self.bpt_baseline):.2f}x off baseline of {self.bpt_baseline:.3f} ms")
+    print(f"avg ribbit forward pass:  {float(fpt):.3f} ms, {float(fpt/self.fpt_baseline):.2f}x off baseline of {self.fpt_baseline:.3f} ms")
+    print(f"avg ribbit backward pass: {float(bpt):.3f} ms, {float(fpt/self.bpt_baseline):.2f}x off baseline of {self.bpt_baseline:.3f} ms")
   
     
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `froog-0.2.2/tests/test_ops.py` & `froog-0.2.3/tests/test_ops.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 import numpy as np
-from froog.tensor import Tensor, GPU
+from ribbit.tensor import Tensor, GPU
 import torch
 import unittest
 import timeit
 import functools
 
-def helper_test_op(shape, torch_func, froog_func, atol=1e-7, grad_atol=1e-7, gpu=False, forward_only=False):
+
+def helper_test_op(shape, torch_func, ribbit_func, atol=1e-7, grad_atol=1e-7, gpu=False, forward_only=False):
   torch_tensors = [torch.rand(x, requires_grad=True) for x in shape]
-  froog_tensors = [Tensor(x.detach().numpy()) for x in torch_tensors]
+  ribbit_tensors = [Tensor(x.detach().numpy()) for x in torch_tensors]
 
   if gpu:
-    froog_tensors = [x.to_gpu() for x in froog_tensors]
+    ribbit_tensors = [x.to_gpu() for x in ribbit_tensors]
 
   out = torch_func(*torch_tensors)
-  ret = froog_func(*froog_tensors)
+  ret = ribbit_func(*ribbit_tensors)
   
   np.testing.assert_allclose(ret.to_cpu().data, out.detach().numpy(), atol=atol)
 
   if not forward_only:
     out.mean().backward()
     ret.mean().backward()
 
-    for t, tt in zip(torch_tensors, froog_tensors):
+    for t, tt in zip(torch_tensors, ribbit_tensors):
       np.testing.assert_allclose(t.grad, tt.grad.to_cpu().data, atol=grad_atol)
 
   # test for speed
   # forward passes
-    torch_fwd = timeit.Timer(functools.partial(torch_func, *torch_tensors)).timeit(5) * 1000/5
-    froog_fwd = timeit.Timer(functools.partial(froog_func, *froog_tensors)).timeit(5) * 1000/5
+  torch_fwd = timeit.Timer(functools.partial(torch_func, *torch_tensors)).timeit(5) * 1000/5
+  ribbit_fwd = timeit.Timer(functools.partial(ribbit_func, *ribbit_tensors)).timeit(5) * 1000/5
 
   # backward passes
   if not forward_only:
     torch_fbp = timeit.Timer(functools.partial(lambda f,x: f(*x).mean().backward(), torch_func, torch_tensors)).timeit(5) * 1000/5
-    froog_fbp = timeit.Timer(functools.partial(lambda f,x: f(*x).mean().backward(), froog_func, froog_tensors)).timeit(5) * 1000/5
+    ribbit_fbp = timeit.Timer(functools.partial(lambda f,x: f(*x).mean().backward(), ribbit_func, ribbit_tensors)).timeit(5) * 1000/5
   else:
-    torch_fbp, froog_fbp = np.nan, np.nan
+    torch_fbp, ribbit_fbp = np.nan, np.nan
 
-  print(f"shape: {repr(shape) : >32} torch/froog fwd: {torch_fwd:.2f}/{froog_fwd:.2f} ms ({float(froog_fwd/torch_fwd):.2f}x slower) bp: {torch_fbp - torch_fwd:.2f}/{froog_fbp - froog_fwd:.2f} ms ({float((froog_fbp - froog_fwd)/(torch_fbp - torch_fwd)):.2f}x slower)")
+  print(f"shape: {repr(shape) : >32} torch/ribbit fwd: {torch_fwd:.2f}/{ribbit_fwd:.2f} ms ({float(ribbit_fwd/torch_fwd):.2f}x slower) bp: {torch_fbp - torch_fwd:.2f}/{ribbit_fbp - ribbit_fwd:.2f} ms ({float((ribbit_fbp - ribbit_fwd)/(torch_fbp - torch_fwd)):.2f}x slower)")
 
 
 class TestOps(unittest.TestCase):
   gpu = False
   # **************** Add ****************
   def test_add(self):
     helper_test_op([(45,65), (45,65)], lambda x,y: x+y, Tensor.add, gpu=self.gpu)
@@ -65,31 +66,31 @@
   def test_sqrt(self):
     helper_test_op([(45,65)], lambda x: x.sqrt(), Tensor.sqrt, gpu=self.gpu)
   # **************** Conv ****************
   def test_conv2d(self):
     for bs in [1,8]:
       for cin in [1,2,3]:
         for groups in [1,3] if cin == 3 else [1]:
-          for H in [2,5]:
-            for W in [2,3,5]:
+          for H in [1,2,5]:
+            for W in [1,2,3,5]:
               helper_test_op([(bs,cin,11,28), (6,cin//groups,H,W)],
                 lambda x,w: torch.nn.functional.conv2d(x,w,groups=groups).relu(),
-                lambda x,w: Tensor.conv2d(x,w,groups=groups).relu(), atol=2e-5, grad_atol=2e-6)
+                lambda x,w: Tensor.conv2d(x,w,groups=groups).relu(), atol=2e-5, grad_atol=2e-6, forward_only=self.gpu)
   def test_strided_conv2d(self):
     bs = 4
     cin = 3
     H,W = 3,3
     helper_test_op([(bs,cin,11,28), (4,cin,H,W)],
                     lambda x,w: torch.nn.functional.conv2d(x,w,stride=2).relu(),
                     lambda x,w: Tensor.conv2d(x,w,stride=2).relu(), 
-                    atol=2e-5, grad_atol=2e-6)
+                    atol=2e-5, grad_atol=2e-6, forward_only=self.gpu)
     helper_test_op([(bs,cin,11,28), (4,cin,H,W)],
                     lambda x,w: torch.nn.functional.conv2d(x,w,stride=(2,1)).relu(),
                     lambda x,w: Tensor.conv2d(x,w,stride=(2,1)).relu(),
-                    atol=2e-5, grad_atol=2e-6)
+                    atol=2e-5, grad_atol=2e-6, forward_only=self.gpu)
 
   # **************** Max Pool ****************
   def test_maxpool_sizes(self):
     for size in [(2,2), (3,3), (3,2), (5,5), (5,1)]:
       helper_test_op([(32,2,110,28)],
         lambda x: torch.nn.functional.max_pool2d(x, kernel_size=size),
         lambda x: Tensor.max_pool2d(x, kernel_size=size))
@@ -97,14 +98,17 @@
     helper_test_op([(32,2,110,28)], lambda x: torch.nn.functional.max_pool2d(x, (2,2)), Tensor.max_pool2d)
   # **************** Avg Pool ****************
   def test_avgpool2x2(self):
     helper_test_op([(32,2,111,28)], lambda x: torch.nn.functional.avg_pool2d(x, (2,2)), Tensor.avg_pool2d)
   # **************** Activations ****************
   def test_relu(self):
     helper_test_op([(45,65)], lambda x: x.relu(), Tensor.relu, gpu=self.gpu)
+  # **************** Padding ****************
+  def test_pad2d(self):
+    helper_test_op([(3,3,3,3)], lambda x: torch.nn.functional.pad(x, (1,1,1,1)), lambda x: x.pad2d(padding=(1,1,1,1)), gpu=self.gpu, forward_only=True)
 
 if GPU:
   class TestOpsGPU(TestOps):
     gpu = True
 
 if __name__ == '__main__':
   unittest.main(verbosity=2)
```

### Comparing `froog-0.2.2/tests/test_optim.py` & `froog-0.2.3/tests/test_optim.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import numpy as np
 import torch
 import unittest
-from froog.tensor import Tensor
-from froog.optim import Adam, SGD, RMSprop
+from ribbit.tensor import Tensor
+from ribbit.optim import Adam, SGD, RMSprop
 
 x_init = np.random.randn(1,3).astype(np.float32)
 W_init = np.random.randn(3,3).astype(np.float32)
 m_init = np.random.randn(1,3).astype(np.float32)
 
-def step_froog(optim, kwargs={}):
+def step_ribbit(optim, kwargs={}):
   model = FrogNet()
   optim = optim([model.x, model.W], **kwargs)
   out = model.forward()
   out.backward()
   optim.step()
   return model.x.data, model.W.data
 
@@ -46,20 +46,20 @@
     out = self.x.matmul(self.W).relu()
     out = torch.nn.functional.log_softmax(out, dim=1)
     out = out.mul(self.m).add(self.m).sum()
     return out
 
 class TestOptim(unittest.TestCase):
   def test_adam(self):
-    for x,y in zip(step_froog(Adam),step_pytorch(torch.optim.Adam)):
+    for x,y in zip(step_ribbit(Adam),step_pytorch(torch.optim.Adam)):
       np.testing.assert_allclose(x, y, atol=1e-6)
 
   def test_sgd(self):
-    for x,y in zip(step_froog(SGD, kwargs={'lr': 0.001}), step_pytorch(torch.optim.SGD, kwargs={'lr': 0.001})):
+    for x,y in zip(step_ribbit(SGD, kwargs={'lr': 0.001}), step_pytorch(torch.optim.SGD, kwargs={'lr': 0.001})):
       np.testing.assert_allclose(x, y, atol=1e-6)
 
   def test_rmsprop(self):
-    for x,y in zip(step_froog(RMSprop, kwargs={'lr': 0.001, 'decay': 0.99}), step_pytorch(torch.optim.RMSprop, kwargs={'lr': 0.001, 'alpha': 0.99})):
+    for x,y in zip(step_ribbit(RMSprop, kwargs={'lr': 0.001, 'decay': 0.99}), step_pytorch(torch.optim.RMSprop, kwargs={'lr': 0.001, 'alpha': 0.99})):
       np.testing.assert_allclose(x, y, atol=1e-6)
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `froog-0.2.2/tests/test_tensor.py` & `froog-0.2.3/tests/test_tensor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import numpy as np
 import torch
 import unittest
-from froog.tensor import Tensor, GPU
-from froog.gradcheck import numerical_jacobian, gradcheck, jacobian
+from ribbit.tensor import Tensor, GPU
+from ribbit.gradcheck import numerical_jacobian, gradcheck, jacobian
 
 x_init = np.random.randn(1,3).astype(np.float32)
 W_init = np.random.randn(3,3).astype(np.float32)
 m_init = np.random.randn(1,3).astype(np.float32)
 
 class TestTensor(unittest.TestCase):
   def test_jacobian(self):
     W = np.random.RandomState(1337).random((10, 5))
     x = np.random.RandomState(7331).random((1, 10)) - 0.5
 
     torch_x = torch.tensor(x, requires_grad=True)
     torch_W = torch.tensor(W, requires_grad=True)
     torch_func = lambda x: torch.nn.functional.log_softmax(x.matmul(torch_W).relu(), dim=1)
 
-    froog_x = Tensor(x)
-    froog_W = Tensor(W)
-    froog_func = lambda x: x.dot(froog_W).relu().logsoftmax()
+    ribbit_x = Tensor(x)
+    ribbit_W = Tensor(W)
+    ribbit_func = lambda x: x.dot(ribbit_W).relu().logsoftmax()
 
-    J = jacobian(froog_func, froog_x)
+    J = jacobian(ribbit_func, ribbit_x)
     PJ = torch.autograd.functional.jacobian(torch_func, torch_x).squeeze().numpy()
-    NJ = numerical_jacobian(froog_func, froog_x)
+    NJ = numerical_jacobian(ribbit_func, ribbit_x)
 
     np.testing.assert_allclose(PJ, J, atol = 1e-5)
     np.testing.assert_allclose(PJ, NJ, atol = 1e-5)
 
-    def test_froog():
+    def test_ribbit():
       x = Tensor(x_init)
       W = Tensor(W_init)
       m = Tensor(m_init)
       out = x.dot(W).relu()
       out = out.logsoftmax()
       out = out.mul(m).add(m).sum()
       out.backward()
@@ -44,15 +44,15 @@
       m = torch.tensor(m_init)
       out = x.matmul(W).relu()
       out = torch.nn.functional.log_softmax(out, dim=1)
       out = out.mul(m).add(m).sum()
       out.backward()
       return out.detach().numpy(), x.grad, W.grad
 
-    for x,y in zip(test_froog(), test_pytorch()):
+    for x,y in zip(test_ribbit(), test_pytorch()):
       np.testing.assert_allclose(x, y, atol=1e-5)
 
   def test_gradcheck(self):
     class TorchModel(torch.nn.Module):
       def __init__(self, weights_init):
         super(TorchModel, self).__init__()
         self.l1 = torch.nn.Linear(*weights_init.shape, bias = False)
@@ -62,15 +62,15 @@
         return torch.nn.functional.log_softmax(self.l1(x).relu(), dim=1)
 
     x = np.random.RandomState(7331).random((1, 10)) - 0.5
     W = np.random.RandomState(1337).random((10, 5))
 
     tiny_x = Tensor(x)
     tiny_W = Tensor(W)
-    froog_func = lambda x: x.dot(tiny_W).relu().logsoftmax()
+    ribbit_func = lambda x: x.dot(tiny_W).relu().logsoftmax()
 
-    self.assertTrue(gradcheck(froog_func, tiny_x))
-    self.assertTrue(gradcheck(froog_func, tiny_x)) 
-    self.assertFalse(gradcheck(froog_func, tiny_x, eps = 0.1)) 
+    self.assertTrue(gradcheck(ribbit_func, tiny_x))
+    self.assertTrue(gradcheck(ribbit_func, tiny_x)) 
+    self.assertFalse(gradcheck(ribbit_func, tiny_x, eps = 0.1)) 
 
 if __name__ == '__main__':
   unittest.main()
```

