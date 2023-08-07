# Comparing `tmp/pycmtensor-1.5.0.tar.gz` & `tmp/pycmtensor-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycmtensor-1.5.0.tar", max compression
+gzip compressed data, was "pycmtensor-1.6.0.tar", max compression
```

## Comparing `pycmtensor-1.5.0.tar` & `pycmtensor-1.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1070 2023-07-26 09:47:51.097952 pycmtensor-1.5.0/LICENSE
--rw-r--r--   0        0        0     2255 2023-07-26 09:47:51.097952 pycmtensor-1.5.0/README.md
--rw-r--r--   0        0        0     2630 2023-07-26 09:47:51.185953 pycmtensor-1.5.0/pycmtensor/__init__.py
--rw-r--r--   0        0        0    10229 2023-07-26 09:47:51.185953 pycmtensor-1.5.0/pycmtensor/dataset.py
--rw-r--r--   0        0        0     2431 2023-07-26 09:47:51.185953 pycmtensor-1.5.0/pycmtensor/defaultconfig.py
--rw-r--r--   0        0        0    16484 2023-07-26 09:47:51.185953 pycmtensor-1.5.0/pycmtensor/expressions.py
--rw-r--r--   0        0        0    11310 2023-07-26 09:47:51.185953 pycmtensor-1.5.0/pycmtensor/functions.py
--rw-r--r--   0        0        0     1366 2023-07-26 09:47:51.185953 pycmtensor-1.5.0/pycmtensor/logger.py
--rw-r--r--   0        0        0     5000 2023-07-26 09:47:51.189953 pycmtensor-1.5.0/pycmtensor/models/MNL.py
--rw-r--r--   0        0        0      189 2023-07-26 09:47:51.189953 pycmtensor-1.5.0/pycmtensor/models/ResLogit.py
--rw-r--r--   0        0        0       80 2023-07-26 09:47:51.189953 pycmtensor-1.5.0/pycmtensor/models/__init__.py
--rw-r--r--   0        0        0    10110 2023-07-26 09:47:51.189953 pycmtensor-1.5.0/pycmtensor/models/basic.py
--rw-r--r--   0        0        0     6890 2023-07-26 09:47:51.189953 pycmtensor-1.5.0/pycmtensor/models/layers.py
--rw-r--r--   0        0        0    19470 2023-07-26 09:47:51.189953 pycmtensor-1.5.0/pycmtensor/optimizers.py
--rw-r--r--   0        0        0    16177 2023-07-26 09:47:51.189953 pycmtensor-1.5.0/pycmtensor/pycmtensor.py
--rw-r--r--   0        0        0     5168 2023-07-26 09:47:51.189953 pycmtensor-1.5.0/pycmtensor/results.py
--rw-r--r--   0        0        0     7126 2023-07-26 09:47:51.189953 pycmtensor-1.5.0/pycmtensor/scheduler.py
--rw-r--r--   0        0        0     3800 2023-07-26 09:47:51.189953 pycmtensor-1.5.0/pycmtensor/statistics.py
--rw-r--r--   0        0        0      268 2023-07-26 09:47:51.189953 pycmtensor-1.5.0/pycmtensor/utils.py
--rw-r--r--   0        0        0     2166 2023-07-26 09:47:51.189953 pycmtensor-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     3292 1970-01-01 00:00:00.000000 pycmtensor-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-07 13:24:52.789547 pycmtensor-1.6.0/LICENSE
+-rw-r--r--   0        0        0     2255 2023-08-07 13:24:52.789547 pycmtensor-1.6.0/README.md
+-rw-r--r--   0        0        0     2604 2023-08-07 13:24:52.881554 pycmtensor-1.6.0/pycmtensor/__init__.py
+-rw-r--r--   0        0        0    10248 2023-08-07 13:24:52.881554 pycmtensor-1.6.0/pycmtensor/dataset.py
+-rw-r--r--   0        0        0     2431 2023-08-07 13:24:52.881554 pycmtensor-1.6.0/pycmtensor/defaultconfig.py
+-rw-r--r--   0        0        0    16115 2023-08-07 13:24:52.881554 pycmtensor-1.6.0/pycmtensor/expressions.py
+-rw-r--r--   0        0        0    12237 2023-08-07 13:24:52.881554 pycmtensor-1.6.0/pycmtensor/functions.py
+-rw-r--r--   0        0        0     1366 2023-08-07 13:24:52.881554 pycmtensor-1.6.0/pycmtensor/logger.py
+-rw-r--r--   0        0        0     4995 2023-08-07 13:24:52.881554 pycmtensor-1.6.0/pycmtensor/models/MNL.py
+-rw-r--r--   0        0        0      189 2023-08-07 13:24:52.881554 pycmtensor-1.6.0/pycmtensor/models/ResLogit.py
+-rw-r--r--   0        0        0       80 2023-08-07 13:24:52.881554 pycmtensor-1.6.0/pycmtensor/models/__init__.py
+-rw-r--r--   0        0        0    11677 2023-08-07 13:24:52.881554 pycmtensor-1.6.0/pycmtensor/models/basic.py
+-rw-r--r--   0        0        0     9110 2023-08-07 13:24:52.881554 pycmtensor-1.6.0/pycmtensor/models/layers.py
+-rw-r--r--   0        0        0    21972 2023-08-07 13:24:52.881554 pycmtensor-1.6.0/pycmtensor/optimizers.py
+-rw-r--r--   0        0        0    16177 2023-08-07 13:24:52.881554 pycmtensor-1.6.0/pycmtensor/pycmtensor.py
+-rw-r--r--   0        0        0     4826 2023-08-07 13:24:52.881554 pycmtensor-1.6.0/pycmtensor/results.py
+-rw-r--r--   0        0        0     7126 2023-08-07 13:24:52.881554 pycmtensor-1.6.0/pycmtensor/scheduler.py
+-rw-r--r--   0        0        0     3997 2023-08-07 13:24:52.881554 pycmtensor-1.6.0/pycmtensor/statistics.py
+-rw-r--r--   0        0        0      268 2023-08-07 13:24:52.881554 pycmtensor-1.6.0/pycmtensor/utils.py
+-rw-r--r--   0        0        0     2166 2023-08-07 13:24:52.881554 pycmtensor-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3292 1970-01-01 00:00:00.000000 pycmtensor-1.6.0/PKG-INFO
```

### Comparing `pycmtensor-1.5.0/LICENSE` & `pycmtensor-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycmtensor-1.5.0/README.md` & `pycmtensor-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pycmtensor-1.5.0/pycmtensor/__init__.py` & `pycmtensor-1.6.0/pycmtensor/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Top-level package for PyCMTensor."""
 
 __author__ = """Melvin Wong"""
-__version__ = "1.5.0"
+__version__ = "1.6.0"
 
 import aesara
-from aesara.tensor.sharedvar import TensorSharedVariable as TensorSharedVariable
-from aesara.tensor.var import TensorVariable as TensorVariable
 from watermark import watermark
 
-import pycmtensor.optimizers
-import pycmtensor.scheduler
-from pycmtensor.defaultconfig import config
+import pycmtensor.defaultconfig as defaultconfig
+import pycmtensor.optimizers as optimizers
+import pycmtensor.scheduler as scheduler
+
+config = defaultconfig.config
 
 # aesara configs
 
 aesara.config.on_unused_input = "ignore"
 aesara.config.mode = "Mode"
 aesara.config.allow_gc = False
 
@@ -52,33 +52,34 @@
 config.add(
     "convergence_threshold",
     1e-4,
     "The gradient norm convergence threshold before model termination",
 )
 config.add(
     "optimizer",
-    pycmtensor.optimizers.Adam,
+    optimizers.Adam,
     "Optimization algorithm to use for model estimation",
 )
 
 config.add(
     "lr_scheduler",
-    pycmtensor.scheduler.ConstantLR,
+    scheduler.ConstantLR,
     "Learning rate scheduler to use for model estimation",
 )
 config.add("lr_ExpRangeCLR_gamma", 0.5, "Gamma parameter for `ExpRangeCLR`")
 config.add("lr_stepLR_factor", 0.5, "Drop step multiplier factor for `stepLR`")
 config.add("lr_stepLR_drop_every", 10, "Drop learning rate every n steps for `stepLR`")
 config.add("lr_CLR_cycle_steps", 16, "Steps per cycle for `CyclicLR`")
 config.add("lr_PolynomialLR_power", 0.999, "Power factor for `PolynomialLR`")
 config.add(
     "BFGS_warmup",
     10,
     "Discards this number of hessian matrix updates when running the `BFGS` algorithm",
 )
+config.add("beta_clipping", True, "Enables or disables Beta value clipping")
 
 
 def about():
     """Returns a `watermark.watermark` of various system information for debugging"""
     return watermark(
         python=True,
         datename=True,
```

### Comparing `pycmtensor-1.5.0/pycmtensor/dataset.py` & `pycmtensor-1.6.0/pycmtensor/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         """Base PyCMTensor Dataset class object
 
         This class stores the data in an array format, and a symbolic tensor reference
         variable object. To call the tensor variable, we invoke the label of the
         variable as an item in the Dataset class, like so:
         ```python
         ds = Dataset(df=df, choice="choice")
-        return ds["label_of_variable"]
+        return ds["label_of_variable"]  -> TensorVariable
         ```
 
         To call the data array, we use the `train_dataset()` or `valid_dataset()`
         method. See method reference for info about the arguments. For example:
         ```python
         # to get the data array for variable "time"
         arr = ds.train_dataset(ds["time"])
```

### Comparing `pycmtensor-1.5.0/pycmtensor/defaultconfig.py` & `pycmtensor-1.6.0/pycmtensor/defaultconfig.py`

 * *Files identical despite different names*

### Comparing `pycmtensor-1.5.0/pycmtensor/expressions.py` & `pycmtensor-1.6.0/pycmtensor/expressions.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,202 +75,194 @@
             "Composite",
             "Could",
             "ScalarFromTensor",
         ]:
             stdout = str.replace(stdout, s, " ")
         symbols = [s for s in str.split(stdout, " ") if len(s) > 0]
         symbols = list(set(symbols))
-        print(symbols)
         return symbols
 
 
-class Expressions:
+class TensorExpressions:
     """Base class for expression objects"""
 
     def __init__(self):
         pass
 
     def __add__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return self() + other
-        elif isinstance(other, (Beta, RandomDraws)):
+        elif isinstance(other, self):
             return self() + other()
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __radd__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return other + self()
-        elif isinstance(other, (Beta, RandomDraws)):
+        elif isinstance(other, self):
             return other() + self()
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __sub__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return self() - other
-        elif isinstance(other, (Beta, RandomDraws)):
+        elif isinstance(other, self):
             return self() - other()
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __rsub__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return other - self()
-        elif isinstance(other, (Beta, RandomDraws)):
+        elif isinstance(other, self):
             return other() - self()
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __mul__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             if self().ndim > 1:
                 return aet.dot(other, self().T)
             else:
                 return self() * other
-        elif isinstance(other, (Beta, RandomDraws)):
+        elif isinstance(other, self):
             return self() * other()
         else:
             raise NotImplementedError(
                 f"__mul__ {other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __rmul__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             if self().ndim > 1:
                 return aet.dot(other, self().T)
             else:
                 return self() * other
-        elif isinstance(other, (Beta, RandomDraws)):
+        elif isinstance(other, self):
             return self() * other()
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __div__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return self() / other
-        elif isinstance(other, (Beta, RandomDraws)):
+        elif isinstance(other, self):
             return self() / other()
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __rdiv__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return other / self()
-        elif isinstance(other, (Beta, RandomDraws)):
+        elif isinstance(other, self):
             return other() / self()
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __neg__(self):
-        if isinstance(self, (TensorVariable, TensorSharedVariable)):
-            return -self
-        elif isinstance(self, Beta):
-            return -self()
-        else:
-            raise NotImplementedError(
-                f"{self} must be a TensorVariable or TensorShared Variable object"
-            )
+        return -self()
 
     def __pow__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return aet.pow(self(), other)
-        elif isinstance(other, (Beta, RandomDraws)):
+        elif isinstance(other, self):
             return aet.pow(self(), other())
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __rpow__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return aet.pow(other, self())
-        elif isinstance(other, (Beta, RandomDraws)):
+        elif isinstance(other, self):
             return aet.pow(other(), self())
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __lt__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return aet.lt(self(), other)
-        elif isinstance(other, (Beta, RandomDraws)):
+        elif isinstance(other, self):
             return aet.lt(self(), other())
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __le__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return aet.le(self(), other)
-        elif isinstance(other, (Beta, RandomDraws)):
+        elif isinstance(other, self):
             return aet.le(self(), other())
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __gt__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return aet.gt(self(), other)
-        elif isinstance(other, (Beta, RandomDraws)):
+        elif isinstance(other, self):
             return aet.gt(self(), other())
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __ge__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return aet.ge(self(), other)
-        elif isinstance(other, (Beta, RandomDraws)):
+        elif isinstance(other, self):
             return aet.ge(self(), other())
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __eq__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return aet.eq(self(), other)
-        elif isinstance(other, (Beta, RandomDraws)):
+        elif isinstance(other, self):
             return aet.eq(self(), other())
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
     def __ne__(self, other):
         if isinstance(other, (TensorVariable, TensorSharedVariable)):
             return aet.neq(self(), other)
-        elif isinstance(other, (Beta, RandomDraws)):
+        elif isinstance(other, self):
             return aet.neq(self(), other())
         else:
             raise NotImplementedError(
                 f"{other} must be a TensorVariable or TensorShared Variable object"
             )
 
 
-class Param(Expressions):
+class Param(TensorExpressions):
     def __init__(self, name: str, value=None, lb=None, ub=None, status=0):
         """Constructor for model param object"""
         self._name = name
         self._status = status
         if value is not None:
             if not isinstance(value, np.ndarray):
                 value = np.asarray(value)
@@ -306,14 +298,17 @@
     def __repr__(self):
         return f"Param({self.name}, {self.shape})"
 
     def get_value(self):
         """Returns the numpy representation of the parameter value"""
         return self.shared_var.get_value()
 
+    def set_value(self, value):
+        self.shared_var.set_value(value)
+
     def reset_value(self):
         """Resets the value of the shared variable to the initial value"""
         self.shared_var.set_value(self.init_value)
 
 
 class Beta(Param):
     def __init__(self, name, value=0.0, lb=None, ub=None, status=0):
@@ -331,15 +326,15 @@
         self._init_value = np.asarray(value, dtype=FLOATX)
         self.shared_var = aesara.shared(self.init_value, name=name, borrow=True)
 
     def __repr__(self):
         return f"Beta({self.name}, {self.get_value()})"
 
 
-class RandomDraws(Expressions):
+class RandomDraws(TensorExpressions):
     """Constructor for model random draws"""
 
     def __init__(self, name: str, draw_type: str, n_draws: int):
         self._name = name
         self.n_draws = n_draws
         srng = RandomStream()
         draw_type = draw_type.lower()
@@ -430,15 +425,15 @@
 class Weight(Param):
     def __init__(self, name, size, value=None, init_type=None):
         """Class object for neural net weight matrix
 
         Args:
             name (str): name of the parameter
             size (Union[tuple,list]): size of the array
-            value (numpy.ndarray): initial values of the parameter. Defaults to `random.uniform(-1.0, 1.0, size)`
+            value (numpy.ndarray): initial values of the parameter. Defaults to `random.uniform(-0.1, 0.1, size)`
             init_type (str): initialization type, see notes
 
         Note:
             Initialization types are one of the following:
 
             * `"zeros"`: a 2-D array of zeros
 
@@ -455,33 +450,35 @@
             Specifying a weight array:
 
             ```python
             code
             ```
 
         """
+        from pycmtensor import config
+
         Param.__init__(self, name, lb=None, ub=None)
 
         # dimension of weight must be 2
         if len(size) != 2:
             raise ValueError(f"Invalid dimensions")
 
-        rng = np.random.default_rng()
+        rng = np.random.default_rng(seed=config.seed)
         n_in, n_out = size
 
         if value is None:
             if init_type == "zeros":
                 value = np.zeros(size, dtype=FLOATX)
             elif init_type == "he":
                 value = rng.normal(0, 1, size=size) * np.sqrt(2 / n_in)
             elif init_type == "glorot":
                 scale = np.sqrt(6 / (n_in + n_out))
                 value = rng.uniform(-1, 1, size) * scale
             else:
-                debug(f"Using default initialization")
+                debug(f"Weight {self.name} using default initialization U(-0.1, 0.1)")
                 value = rng.uniform(-0.1, 0.1, size=size)
 
         if value.shape != size:
             raise ValueError(f"init_value argument is not a valid array of size {size}")
 
         self._init_type = init_type
         self._init_value = value
```

### Comparing `pycmtensor-1.5.0/pycmtensor/functions.py` & `pycmtensor-1.6.0/pycmtensor/functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 # functions.py
 """PyCMTensor functions module"""
-from ctypes import util
-from typing import Union
-
-import aesara
 import aesara.tensor as aet
 import aesara.tensor.nlinalg as nlinalg
 import numpy as np
-from aesara.tensor.sharedvar import TensorSharedVariable
-from aesara.tensor.var import TensorVariable
 
-from pycmtensor.expressions import Beta, Expressions, Param
-from pycmtensor.logger import error, log
+from pycmtensor.expressions import Beta, Param
 
 __all__ = [
     "exp_mov_average",
     "logit",
     "loglikelihood",
     "rmse",
     "mae",
@@ -23,23 +16,45 @@
     "kl_multivar_norm",
     "errors",
     "second_order_derivative",
     "first_order_derivative",
 ]
 
 
-def exp_mov_average(
-    batch_avg: TensorVariable, moving_avg: TensorVariable, alpha: float = 0.1
-):
+def relu(x, alpha=0.0):
+    """Compute the element-wise rectified linear activation function.
+
+    Source taken from Theano 0.7.1
+
+    Args:
+        x (TensorVariable): symbolic tensor
+        alpha (Union[float, TensorSharedVariable]): Slope for negative input, usually
+            between 0 and 1. The default value of 0 will lead to the standard
+            rectifier, 1 will lead to a linear activation function, and any value in
+            between will give a leaky rectifier. A shared variable (broadcastable against `x`) will result in a parameterized rectifier with learnable slope
+            (s).
+
+    Returns:
+        (TensorVariable): Elementwise rectifier applied to `x`.
+    """
+    if alpha == 0.0:
+        return 0.5 * (x + aet.abs(x))
+    else:
+        f1 = 0.5 * (1 + alpha)
+        f2 = 0.5 * (1 - alpha)
+        return f1 * x + f2 * aet.abs(x)
+
+
+def exp_mov_average(batch_avg, moving_avg, alpha=0.1):
     """Calculates the exponential moving average (EMA) of a new minibatch
 
     Args:
-        batch_avg: the new batch value of the mean
-        moving_avg: the moving value of the accumulated mean
-        alpha: the moving average factor of the batch mean
+        batch_avg (TensorVariable): mean batch value
+        moving_avg (TensorVariable): accumulated mean
+        alpha (float): moving average factor of the batch mean
 
     Returns:
         (TensorVariable): the new moving average
 
     Note:
         The moving average will decay by the difference between the existing value
         and the new value multiplied by the moving average factor. A higher `alpha`
@@ -53,60 +68,57 @@
     while moving_avg.ndim < batch_avg.ndim:
         moving_avg = aet.expand_dims(moving_avg, -1)
 
     ema = batch_avg * alpha + moving_avg * (1 - alpha)
     return ema
 
 
-def logit(
-    utility: Union[list, tuple, TensorVariable],
-    avail: Union[list, tuple, TensorVariable] = None,
-):
+def logit(utility, avail=None):
     """Computes the Logit function, with availability conditions.
 
     Args:
-        utility: list of M utility equations
-        avail: list of M availability conditions,
+        utility (Union[list, tuple, TensorVariable]): utility equations
+        avail (Union[list, tuple, TensorVariable]): availability conditions,
             if no availability conditions are provided, defaults to `1` for all
             availabilities.
 
     Returns:
         (TensorVariable): A NxM matrix of probabilities.
 
     Note:
         The 0-th dimension is the numbering of alternatives, the N-th dimension is the size of the input (# rows).
     """
-
     if isinstance(utility, (list, tuple)):
         if (avail != None) and (len(utility) != len(avail)):
             msg = f"{utility} must have the same length as {avail}"
             raise ValueError(msg)
+
         _utility = utility
         for n, u in enumerate(_utility):
-            # convert u to vector representation if u is a scalar
-            if not isinstance(u, TensorVariable):
+            # convert u to tensor representation if u is an expression
+            if isinstance(u, Param):
                 utility[n] = aet.as_tensor_variable(u())
 
         # get maximum ndim from set of utlity equations
         max_ndim = max([u.ndim for u in utility])
-        _utility = utility
 
         # pad tensors to the left to have the same number of dimensions
-        utility = [aet.atleast_Nd(u, n=max_ndim) for u in _utility]
+        utility = [aet.atleast_Nd(u, n=max_ndim) for u in utility]
 
         # broadcast tensors across each other before stacking
         utility = aet.broadcast_arrays(*utility)
 
         # stack list of tensors to into a max_ndim+1 tensor
         U = aet.stack(utility)
 
     # use the utility inputs as is if given as a TensorVariable
-    elif isinstance(utility, TensorVariable):
-        U = utility
     else:
+        U = utility
+
+    if U is None:
         raise NotImplementedError(
             f"utility {utility} has to be a list, tuple or TensorVariable instance"
         )
 
     # calculate the probabilities
     prob = aet.special.softmax(U, axis=0)
 
@@ -123,43 +135,48 @@
 
         # normalize probabilities to sum to 1
         prob = prob / aet.sum(prob, axis=0, keepdims=1)
 
     return prob
 
 
-def log_likelihood(prob: TensorVariable, y: TensorVariable):
+def log_likelihood(prob, y, index=None):
     """Symbolic representation of the log likelihood cost function.
 
     Args:
-        prob: a `TensorVariable` matrix describing the choice probabilites
-        y: a `TensorVariable` referencing the choice variable
+        prob (TensorVariable): choice probabilites tensor
+        y (TensorVariable): choice variable tensor
+        index (TensorVariable): index tensor, if `None`, dynamically get the same of the
+            `y` tensor
 
     Returns:
-        (TensorVariable): a symbolic representation of the log likelihood with `ndim=0`.
+        (TensorVariable): a symbolic tensor of the log likelihood
 
     Note:
         The 0-th dimension is the numbering of alternatives, the N-th dimension is the size of the input (# rows).
     """
-    # calculate the log probabilitiy of axis 0
-    logprob = aet.log(prob)[y, ..., aet.arange(y.shape[0])]
+    # calculate the log probabilitiy over axis 0
+    if not index is None:
+        logprob = aet.log(prob)[y, ..., index]
+    else:
+        logprob = aet.log(prob)[y, ..., aet.arange(y.shape[0])]
 
     # take the average over all other non choice, non-n axes
     while logprob.ndim > 1:
         logprob = aet.mean(logprob, axis=1)
 
     return aet.sum(logprob)
 
 
-def rmse(y_hat: TensorVariable, y: TensorVariable):
+def rmse(y_hat, y):
     """Computes the root mean squared error (RMSE) between pairs of observations
 
     Args:
-        y_hat: model estimated values
-        y: ground truth values
+        y_hat (TensorVariable): model estimated values
+        y (TensorVariable): ground truth values
 
     Returns:
         (TensorVariable): symbolic scalar representation of the rmse
 
     Note:
         Tensor is flattened to a `dim=1` vector if the input tensor is `dim=2`.
 
@@ -170,20 +187,20 @@
     if y_hat.ndim < 1:
         y_hat = aet.flatten(y_hat)
         y = aet.flatten(y)
 
     return aet.sqrt(aet.mean(aet.sqr(y_hat - y)))
 
 
-def mae(y_hat: TensorVariable, y: TensorVariable):
+def mae(y_hat, y):
     """Computes the mean absolute error (MAE) between pairs of observations
 
     Args:
-        y_hat: model estimated values
-        y : ground truth values
+        y_hat (TensorVariable): model estimated values
+        y (TensorVariable): ground truth values
 
     Returns:
         (TensorVariable): symbolic scalar representation of the mean absolute error
 
     Note:
         Tensor is flattened to a `dim=1` vector if the input tensor is `dim=2`.
     """
@@ -193,20 +210,20 @@
     if y_hat.ndim < 1:
         y_hat = aet.flatten(y_hat)
         y = aet.flatten(y)
 
     return aet.mean(aet.abs(y_hat - y))
 
 
-def kl_divergence(p: TensorVariable, q: TensorVariable):
+def kl_divergence(p, q):
     """Computes the KL divergence loss between discrete distributions `p` and `q`.
 
     Args:
-        p: model output probabilities
-        q: ground truth probabilities
+        p (TensorVariable): model output probabilities
+        q (TensorVariable): ground truth probabilities
 
     Returns:
         (TensorVariable): a symbolic representation of the KL loss 
 
     Note:
         Formula:
 
@@ -281,73 +298,89 @@
         trace_term = nlinalg.trace(aet.dot(v1_inv, v0))
         prod_term = aet.dot((m1 - m0).T, aet.dot(v1_inv, (m1 - m0)))
         kld = aet.sum(det_term + trace_term + prod_term - k)
 
     return kld
 
 
-def errors(prob: TensorVariable, y: TensorVariable):
+def errors(prob, y):
     """Symbolic representation of the discrete prediction as a percentage error.
 
     Args:
-        prob: matrix describing the choice probabilites
-        y: the `TensorVariable` referencing the choice column
+        prob (TensorVariable): choice probabilites tensor
+        y (TensorVariable): choice variable tensor
 
     Returns:
         (TensorVariable): the mean prediction error over `y`
     """
     pred = aet.argmax(prob, axis=0)
 
     if y.dtype.startswith("int"):
         return aet.mean(aet.neq(pred, y))
     else:
         raise NotImplementedError(f"y should be int32 or int64", ("y.dtype:", y.dtype))
 
 
-def second_order_derivative(cost: TensorVariable, params: list[Beta]):
+def second_order_derivative(cost, params):
     """Symbolic representation of the 2nd order Hessian matrix given cost.
 
     Args:
-        cost: the cost function to compute the gradients over
-        params: list of params to compute the gradients over
+        cost (TensorVariable): function to compute the gradients over
+        params (List[Beta]): params to compute the gradients over
 
     Returns:
         (TensorVariable): the Hessian matrix of the cost function wrt to the params
 
     Note:
         Parameters with `status=1` are ignored.
     """
     if not isinstance(params, list):
         raise TypeError(f"params is not list instance. type(params)={type(params)}")
-    params = [p() for p in params if (p.status != 1)]
-    grads = aet.grad(cost, params, disconnected_inputs="ignore")
+
+    wrt_params = []
+    for p in params:
+        if isinstance(p, Beta):
+            param = p()
+            if hasattr(p, "output"):
+                param.name = p.name
+            wrt_params.append(param)
+
+    grads = aet.grad(cost, wrt_params, disconnected_inputs="ignore")
+    grads = [aet.sum(g) for g in grads]
     mat = aet.as_tensor_variable(np.zeros((len(grads), len(grads))))
     for i in range(len(grads)):
+        grad2 = aet.grad(grads[i], wrt_params, disconnected_inputs="ignore")
+        grad2 = [aet.sum(g) for g in grad2]
         mat = aet.set_subtensor(
             x=mat[i, :],
-            y=aet.grad(grads[i], params, disconnected_inputs="ignore"),
+            y=grad2,
         )
     return mat
 
 
-def first_order_derivative(cost: TensorVariable, params: list[Beta]):
+def first_order_derivative(cost, params):
     """Symbolic representation of the 1st order gradient vector given the cost.
 
     Args:
-        cost: the cost function to compute the gradients over
-        params: list of params to compute the gradients over
+        cost (TensorVariable): function to compute the gradients over
+        params (List[Beta]): params to compute the gradients over
 
     Returns:
         (TensorVariable): the gradient vector of the cost function wrt to the params
 
     Note:
         Parameters with `status=1` are ignored.
     """
-    if not isinstance(params, (dict, list)):
-        raise TypeError(
-            f"params is not list or dict instance. type(params)={type(params)}"
-        )
-    if isinstance(params, dict):
-        params = list(params.values())
-    params = [p() for p in params if (p.status != 1)]
-    grads = aet.grad(cost, params, disconnected_inputs="ignore")
+    if not isinstance(params, list):
+        raise TypeError(f"params is not list instance. type(params)={type(params)}")
+
+    wrt_params = []
+    for p in params:
+        if isinstance(p, Beta):
+            param = p()
+            if hasattr(p, "output"):
+                param.name = p.name
+            wrt_params.append(param)
+
+    grads = aet.grad(cost, wrt_params, disconnected_inputs="ignore")
+    grads = [aet.sum(g) for g in grads]
     return aet.as_tensor_variable(grads)
```

### Comparing `pycmtensor-1.5.0/pycmtensor/logger.py` & `pycmtensor-1.6.0/pycmtensor/logger.py`

 * *Files identical despite different names*

### Comparing `pycmtensor-1.5.0/pycmtensor/models/MNL.py` & `pycmtensor-1.6.0/pycmtensor/models/MNL.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 from time import perf_counter
-from typing import Dict, List, Tuple, Union
 
 import aesara
 import aesara.tensor as aet
 from aesara import pprint
-from aesara.tensor.var import TensorVariable
 
-from pycmtensor.expressions import Beta, ExpressionParser
+from pycmtensor.expressions import Beta
 from pycmtensor.functions import (
     errors,
     first_order_derivative,
     log_likelihood,
     logit,
     second_order_derivative,
 )
-from pycmtensor.logger import debug, info
+from pycmtensor.logger import info
 from pycmtensor.models.basic import BaseModel, drop_unused_variables, extract_params
 from pycmtensor.utils import time_format
 
 
-# class MNL(PyCMTensorModel):
 class MNL(BaseModel):
-    def __init__(
-        self,
-        ds,
-        params: Dict,
-        utility: Union[list[TensorVariable], TensorVariable],
-        av: List[TensorVariable] = None,
-        **kwargs: Tuple,
-    ):
+    def __init__(self, ds, params, utility, av=None, **kwargs):
         """Defines a Multinomial Logit model
 
         Args:
             ds (pycmtensor.Data): the database object
-            params: dictionary of name:parameter pair
-            utility: the vector of utility functions
-            av: list of availability conditions. If `None`, all
+            params (Dict): dictionary of name:parameter pair
+            utility (Union[list[TensorVariable], TensorVariable]): the vector of utility functions
+            av (List[TensorVariable]): list of availability conditions. If `None`, all
                 availability is set to 1
             **kwargs: Optional keyword arguments for modifying the model configuration settings. See [configuration](../../../user_guide/configuration) in the user guide for details on possible options
+
+        Attributes:
+            x (List[TensorVariable]):
+            y (TensorVariable):
+            xy (List[TensorVariable]):
+            betas (List[Beta]):
+            cost (TensorVariable):
+            p_y_given_x (TensorVariable):
+            ll (TensorVariable):
+            pred (TensorVariable):
         """
 
         super().__init__(**kwargs)
         self.name = "MNL"
         self.params = []  # keep track of all the Params
         self.betas = []  # keep track of the Betas
         self.updates = []  # keep track of the updates
-        self.learning_rate = aet.scalar("learning_rate")
+        self.index = aet.ivector("index")  # indices of the dataset
+        self.learning_rate = aet.scalar("learning_rate")  # learning rate tensor
 
         self.y = ds.y  # Definition of the symbolic choice output (tensor)
 
         self.p_y_given_x = logit(utility, av)  # expression for the choice probability
 
-        self.ll = log_likelihood(
-            self.p_y_given_x, self.y
-        )  # expression for the likelihood
+        # expression for the likelihood
+        self.ll = log_likelihood(self.p_y_given_x, self.y, self.index)
 
         self.cost = -(self.ll / self.y.shape[0])  # expression for the cost
 
         self.pred = aet.argmax(
             self.p_y_given_x, axis=0
         )  # expression for the prediction
 
@@ -65,40 +65,42 @@
         self.betas = [p for p in self.params if isinstance(p, Beta)]
 
         # drop unused variables form dataset
         drop_unused = drop_unused_variables(self.cost, self.params, ds())
         ds.drop(drop_unused)
 
         self.x = ds.x
+        self.xy = self.x + [self.y]
         info(f"inputs in {self.name}: {self.x}")
 
         start_time = perf_counter()
-        self.build_fns()
+        self.build_fn()
         build_time = round(perf_counter() - start_time, 3)
 
         self.results.build_time = time_format(build_time)
         info(f"Build time = {self.results.build_time}")
 
     def build_cost_updates_fn(self, updates):
         """Method to call to build/rebuilt cost function with updates to the model. Creates a class function `MNL.cost_updates_fn(*inputs, output, lr)` that receives a list of input variable arrays, the output array, and a learning rate.
 
         Args:
             updates (List[Tuple[TensorSharedVariable, TensorVariable]]): The list of tuples containing the target shared variable and the new value of the variable.
         """
         self.cost_updates_fn = aesara.function(
             name="cost_updates",
-            inputs=self.x + [self.y] + [self.learning_rate],
+            inputs=self.x + [self.y, self.learning_rate, self.index],
             outputs=self.cost,
             updates=updates,
         )
 
-    def build_fns(self):
-        """Method to call to build mathematical operations without updates to the model. Creates class functions: `MNL.log_likelihood_fn(*inputs, output)`, `MNL.choice_probabilities_fn(*inputs)`, `MNL.choice_predictions_fn(*inputs, output)`, `MNL.prediction_error_fn(*inputs, output)`, `MNL.hessian_fn(*inputs, output)`, `MNL.gradient_vector_fn(*inputs, output)`."""
+    def build_fn(self):
+        """Method to call to build mathematical operations without updates to the model"""
+
         self.log_likelihood_fn = aesara.function(
-            name="log_likelihood", inputs=self.x + [self.y], outputs=self.ll
+            name="log_likelihood", inputs=self.x + [self.y, self.index], outputs=self.ll
         )
 
         self.choice_probabilities_fn = aesara.function(
             name="choice_probabilities",
             inputs=self.x,
             outputs=self.p_y_given_x.swapaxes(0, 1),
         )
@@ -111,22 +113,22 @@
             name="prediction_error",
             inputs=self.x + [self.y],
             outputs=errors(self.p_y_given_x, self.y),
         )
 
         self.hessian_fn = aesara.function(
             name="hessian",
-            inputs=self.x + [self.y],
+            inputs=self.x + [self.y, self.index],
             outputs=second_order_derivative(-self.cost, self.betas),
             allow_input_downcast=True,
         )
 
         self.gradient_vector_fn = aesara.function(
             name="gradient_vector",
-            inputs=self.x + [self.y],
+            inputs=self.x + [self.y, self.index],
             outputs=first_order_derivative(-self.cost, self.betas),
             allow_input_downcast=True,
         )
 
     def __str__(self):
         return f"{self.name}"
```

### Comparing `pycmtensor-1.5.0/pycmtensor/models/basic.py` & `pycmtensor-1.6.0/pycmtensor/models/basic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,102 @@
 from collections import OrderedDict
 from time import perf_counter
-from typing import Union
 
 import numpy as np
 
-from pycmtensor import config
+import pycmtensor.defaultconfig as defaultconfig
 from pycmtensor.expressions import Beta, ExpressionParser, Param
 from pycmtensor.logger import debug, info, warning
 from pycmtensor.results import Results
 from pycmtensor.utils import time_format
 
+config = defaultconfig.config
+
 
 class BaseModel(object):
     def __init__(self, **kwargs):
         """Basic model class object
 
         Attributes:
             name (str): name of the model
-            config (Config): pycmtensor config object
-            rng (Generator): random number generator
-            params (list): list of model parameters (betas & weights)
+            config (pycmtensor.Config): pycmtensor config object
+            rng (numpy.random.Generator): random number generator
+            params (list): list of model parameters (`betas` & `weights`)
             betas (list): list of model scalar betas
+            sigmas (list): list of model scalar sigmas
             weights (list): list of model weight matrices
+            biases (list): list of model vector biases
             updates (list): list of (param, update) tuples
-            inputs (list): list of TensorVariables
-            outputs (TensorVariable): symbolic reference to the output TensorVariable
             learning_rate (TensorVariable): symbolic reference to the learning rate
             results (Results): stores the results of the model estimation
         """
-        self.name = "BaseModel"
         self.config = config
         self.rng = np.random.default_rng(config.seed)
-        self.params = []  # keep track of all the Params
-        self.betas = []  # keep track of the Betas
-        self.weights = []  # keep track of the Weights
-        self.updates = []  # keep track of the updates
+        self.weights = []
+        self.biases = []
+        self.betas = []
         self.results = Results()
 
         for key, value in kwargs.items():
             self.config.add(key, value)
 
         debug(f"Building model...")
 
     @property
-    def n_params(self) -> int:
+    def n_params(self):
         """Return the total number of estimated parameters"""
-        return self.n_betas + self.n_weights
+        return self.n_betas + self.n_weights + self.n_biases
 
     @property
-    def n_betas(self) -> int:
+    def n_betas(self):
         """Return the number of estimated Betas"""
         return len(self.betas)
 
     @property
-    def n_weights(self) -> int:
+    def n_weights(self):
+        """Return the total number of estimated Weight parameters"""
+        return np.sum([np.prod(w.shape) for w in self.weights])
+
+    @property
+    def n_biases(self):
         """Return the total number of estimated Weight parameters"""
-        return sum([w.size for w in self.get_weights()])
+        return np.sum([np.prod(b.shape) for b in self.biases])
 
-    def get_weights(self) -> list:
-        """Returns a list of Weight values"""
-        return [w.get_value() for w in self.weights]
-
-    def get_betas(self) -> list:
-        """Returns a list of Beta values"""
-        return [beta.get_value() for beta in self.betas]
+    def get_weights(self):
+        """Returns a dict of Weight values"""
+        return {w.name: w.get_value() for w in self.weights}
+
+    def get_biases(self):
+        """Returns a dict of Weight values"""
+        return {b.name: b.get_value() for b in self.biases}
+
+    def get_betas(self):
+        """Returns a dict of Beta values"""
+        return {beta.name: beta.get_value() for beta in self.betas}
 
     def reset_values(self):
         """Resets Model parameters to their initial value"""
         for p in self.params:
             p.reset_value()
 
+    def include_params_for_convergence(self, **kwargs):
+        """Returns a Ordered dict of parameters values to check for convergence
 
-def extract_params(cost, variables: Union[dict, list]):
+        Returns:
+            (OrderedDict): ordered dictionary of parameter values
+        """
+        return OrderedDict()
+
+
+def extract_params(cost, variables):
     """Extracts Param objects from variables
 
     Args:
-        cost (TensorVariable): the cost function to look for Param objects
-        variables: dictionary or list of local variables from the current program
+        cost (TensorVariable): function to evaluate
+        variables (Union[dict, list]): list of variables from the current program
     """
     params = []
     symbols = ExpressionParser().parse(cost)
     seen = set()
 
     if isinstance(variables, dict):
         variables = [v for _, v in variables.items()]
@@ -96,15 +112,25 @@
 
         params.append(variable)
         seen.add(variable.name)
 
     return params
 
 
-def drop_unused_variables(cost, params: Param, variables: dict) -> list:
+def drop_unused_variables(cost, params, variables):
+    """Internal method to remove ununsed tensors
+
+    Args:
+        cost (TensorVariable): function to evaluate
+        params (Param): param objects
+        variables (dict): list of array variables from the dataset
+
+    Returns:
+        (list): a list of param names which are not used in the model
+    """
     symbols = ExpressionParser().parse(cost)
     param_names = [p.name for p in params]
     symbols = [s for s in symbols if s not in param_names]
     return [var for var in list(variables) if var not in symbols]
 
 
 def train(model, ds, **kwargs):
@@ -147,56 +173,72 @@
         power=model.config.lr_PolynomialLR_power,
         cycle_steps=model.config.lr_CLR_cycle_steps,
         gamma=model.config.lr_ExpRangeCLR_gamma,
     )
 
     performance_graph = OrderedDict()
 
-    x_and_y = model.x + [model.y]
-    train_data = ds.train_dataset(x_and_y)
-    valid_data = ds.valid_dataset(x_and_y)
-    log_likelihood = model.log_likelihood_fn(*train_data)
+    x_y = model.x + [model.y]
+    train_data = ds.train_dataset(x_y)
+    valid_data = ds.valid_dataset(x_y)
+
+    t_index = np.arange(len(train_data[-1]))
+    log_likelihood = model.log_likelihood_fn(*train_data, t_index)
     error = model.prediction_error_fn(*valid_data)
 
     model.results.null_loglikelihood = log_likelihood
     model.results.best_loglikelihood = log_likelihood
     model.results.best_valid_error = error
-    model.results.params = model.params
+    model.results.best_step = 0
+    model.results.gnorm = np.nan
     model.results.n_train = n_train
     model.results.n_valid = n_valid
     model.results.n_params = model.n_params
     model.results.seed = model.config.seed
 
-    start_time = perf_counter()
-    info(
-        f"Start (n={n_train}, Step={step}, LL={model.results.null_loglikelihood:.2f}, Error={model.results.best_valid_error*100:.2f}%)"
+    params_prev = [p.get_value() for p in model.params if isinstance(p, Beta)]
+
+    model.results.betas = OrderedDict(
+        {p.name: p.get_value() for p in model.params if isinstance(p, Beta)}
     )
+    model.results.params = OrderedDict({p.name: p.get_value() for p in model.params})
 
-    params_prev = [p.get_value() for p in model.params if isinstance(p, Beta)]
+    p = model.include_params_for_convergence(train_data, t_index)
+    params_prev.extend(list(p.values()))
+    model.results.betas.update(p)
 
     batch_data = []
     for batch in range(n_train_batches):
-        batch_data.append(ds.train_dataset(x_and_y, batch, batch_size, shift))
+        batch_data.append(ds.train_dataset(x_y, batch, batch_size, shift))
+
+    start_time = perf_counter()
+    info(
+        f"Start (n={n_train}, Step={step}, LL={model.results.null_loglikelihood:.2f}, Error={model.results.best_valid_error*100:.2f}%)"
+    )
 
     while (step < max_steps) and (not done_looping):
         learning_rate = lr_scheduler(step)  # get learning rate at this step
 
         for i in range(n_train_batches):
-            model.cost_updates_fn(*batch_data[i], learning_rate)  # update model
+            index = np.arange(len(batch_data[i][-1]))
+            model.cost_updates_fn(*batch_data[i], learning_rate, index)  # update model
 
             if iteration % validation_freq == 0:
-                log_likelihood = model.log_likelihood_fn(*train_data)
+                log_likelihood = model.log_likelihood_fn(*train_data, t_index)
                 performance_graph[step] = {"log likelihood": log_likelihood}
 
                 params = [p.get_value() for p in model.params if isinstance(p, Beta)]
-                diff = [p_prev - p for p_prev, p in zip(params_prev, params)]
-                gnorm = np.sqrt(np.sum(np.square(diff)))
+                p = model.include_params_for_convergence(train_data, t_index)
+                params.extend(list(p.values()))
 
+                diff = [p_prev - p for p_prev, p in zip(params_prev, params)]
                 params_prev = params
 
+                gnorm = np.sqrt(np.sum(np.square(diff)))
+
                 if gnorm < (gnorm_tol / 5.0):
                     gnorm_tol = gnorm
                     info(
                         f"Train (Step={step}, LL={log_likelihood:.2f}, Error={error*100:.2f}%, gnorm={gnorm:.5e}, {iteration}/{patience})"
                     )
 
                 if log_likelihood > model.results.best_loglikelihood:
@@ -211,17 +253,24 @@
                             min(max(patience, iteration * patience_inc), max_iterations)
                         )
 
                     model.results.best_step = step
                     model.results.best_iteration = iteration
                     model.results.best_loglikelihood = log_likelihood
                     model.results.best_valid_error = error
-                    model.results.params = model.params
                     model.results.gnorm = gnorm
 
+                    for p in model.params:
+                        model.results.params[p.name] = p.get_value()
+                        if isinstance(p, Beta):
+                            model.results.betas[p.name] = p.get_value()
+
+                    p = model.include_params_for_convergence(train_data, t_index)
+                    model.results.betas.update(p)
+
                 if gnorm < convergence_threshold:
                     converged = True
                 else:
                     patience = int(
                         min(max(patience, iteration * patience_inc), max_iterations)
                     )
 
@@ -247,24 +296,25 @@
     else:
         info(
             f"Maximum number of iterations reached: {iteration}/{patience} (t={train_time})"
         )
 
     model.results.lr_history_graph = lr_scheduler.history
     model.results.performance_graph = performance_graph
-    model.params = model.results.params
 
-    betas = [param for param in model.params if isinstance(param, Beta)]
-    n_betas = len([b for b in betas if (b.status != 1)])
+    for p in model.params:
+        p.set_value(model.results.params[p.name])
+
+    n_betas = len(model.results.betas)
     gradient_vector = np.zeros((n_train, n_betas))
     hessian = np.zeros((n_train, n_betas, n_betas))
     for n in range(n_train):
         data = [[d[n]] for d in train_data]
-        gradient_vector[n, :] = model.gradient_vector_fn(*data)
-        hessian[n, :, :] = model.hessian_fn(*data)
+        gradient_vector[n, :] = model.gradient_vector_fn(*data, np.array([0]))
+        hessian[n, :, :] = model.hessian_fn(*data, np.array([0]))
 
     bhhh = gradient_vector[:, :, None] * gradient_vector[:, None, :]
 
     model.results.bhhh_matrix = bhhh
     model.results.hessian_matrix = hessian
 
     info(
```

### Comparing `pycmtensor-1.5.0/pycmtensor/models/layers.py` & `pycmtensor-1.6.0/pycmtensor/models/layers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,78 +1,152 @@
 # layers.py
 """Model layers"""
+
 import aesara
 import aesara.tensor as aet
 import numpy as np
-from aesara.tensor.math import sigmoid, tanh
-from aesara.tensor.nnet import relu
 
-from ..functions import exp_mov_average
-from ..logger import debug
+import pycmtensor.functions as functions
+from pycmtensor.expressions import Beta, Bias, TensorExpressions, Weight
+
+
+class Layer(TensorExpressions):
+    def __init__(self, name, input, status=0, **kwargs):
+        """Default class object
+
+        Args:
+            name (str): name of the layer for identification
+            input (TensorVariable): symbolic variable of the layer input
+
+        Attributes:
+            params (list): list of parameters of the layers
+            input (TensorVariable): symbolic variable of the layer input
+            output (TensorVariable): symbolic variable of the layer output
+
+        """
+        self._name = name
+        self._input = input
+        self._status = status
+
+    def __repr__(self):
+        return f"Layer({self.name}, size={self.n_in, self.n_out})"
+
+    def __call__(self):
+        return self._output
+
+    @property
+    def params(self):
+        return self._params
+
+    @property
+    def input(self):
+        return self._input
 
+    @property
+    def output(self):
+        return self._output
 
-class Layer:
-    """Default class type"""
+    @property
+    def name(self):
+        return self._name
 
-    pass
+    @property
+    def status(self):
+        return self._status
 
 
 class DenseLayer(Layer):
-    def __init__(self, w, bias, activation=None):
-        """Class object for dense layer
+    def __init__(
+        self, name, input, n_in, n_out, init_type=None, activation=None, **kwargs
+    ):
+        """Class object for dense layer. Compute the function $h=f(w^\\top x + bias)$
 
         Args:
-            w (TensorSharedVariable): layer weights with ndim=2
-            bias (TensorSharedVariable): layer bias with ndim=1
-            activation: the activation function, possible options are ``tanh``,
-                ``relu``, ``sigm``, ``None``
-
-        Note:
-            Layer activation function is set based on the type of weight initialization.
-            If weight init is "he", the activation is relu, if "glorot", the activation
-            is tanh, otherwise the activation defaults to sigm.
-            Setting activation to other than ``None`` overrides this.
+            input (TensorVariable): symbolic variable of the layer input
+            n_in (int): the number of input nodes
+            n_out (int): the number of output nodes
+            init_type (str): initialization type, possible options: `"zeros"`, `"he"`,
+                `"glorot"`, `None` (defaut)
+            activation (str): activation function $f$, possible options: `"tanh"`,
+                `"relu"`, `"sigmoid"`, `"softplus"`, `None` (defaut)
+
+        Attributes:
+            w (Weight): weight matrix of the layer
+            bias (Bias):
         """
+        Layer.__init__(self, name, input, **kwargs)
+        self.n_in = n_in
+        self.n_out = n_out
+
+        if (not init_type in ["zeros", "he", "glorot"]) and (not init_type is None):
+            raise KeyError
+
+        w = Weight(f"{name}_W", (n_in, n_out), init_type=init_type)
+        b = Bias(f"{name}_bias", (n_out,))
+
+        if activation == "tanh":
+            activation = aet.tanh
+        elif activation == "relu":
+            activation = functions.relu
+        elif activation == "softplus":
+            activation = aet.softplus
+        elif activation == "sigmoid":
+            activation = aet.sigmoid
 
+        self.activation = activation
+        self._w = w
+        self._bias = b
+        self._params = [self.w, self.bias]
+
+        linear = (self.w.T @ input) + self.bias  # -> (n_out, len(input))
+        if n_out == 1:
+            linear = aet.flatten(linear)  # (1, len(input)) -> (len(input),)
         if activation is None:
-            if w.init_type == "he":
-                activation = relu
-                debug(f"activation of DenseLayer({w.shape}) set as ReLU")
-            elif w.init_type == "glorot":
-                activation = tanh
-                debug(f"activation of DenseLayer({w.shape}) set as tanh")
-            else:
-                activation = sigmoid
-                debug(f"activation of DenseLayer({w.shape}) set as sigm")
+            self._output = aet.as_tensor_variable(linear)
         else:
-            activation = activation
+            self._output = activation(linear)
 
-        self.activation = activation
-        self.w = w
-        self.bias = bias
-        self.params = [w, bias]
+    @property
+    def w(self):
+        return self._w
 
-    def apply(self, input):
-        """Function to apply the input to the computational graph"""
-        if isinstance(input, (list, tuple)):
-            input = aet.stack(input)
-        self.input = input
+    @property
+    def bias(self):
+        return self._bias
 
-        h = aet.dot(self.input.swapaxes(0, -1), self.w()) + self.bias()
-        self._output = self.activation(h).swapaxes(0, -1)
+    def __repr__(self):
+        return f"DenseLayer({self.name}, {self.output})"
 
-    @property
-    def updates(self):
-        """Returns a list of update tuple pairs"""
-        return [()]
+    def __call__(self):
+        return Layer.__call__(self)
 
-    @property
-    def output(self):
-        """Returns the output of this layer"""
-        return self._output
+
+class TNBetaLayer(DenseLayer, Beta):
+    def __init__(self, name, input, init_type=None, activation=None, **kwargs):
+        """_summary_
+
+        Args:
+            name (str): name of the layer
+            input (Layer): previous layer of the neural net
+            init_type (str): initialization type, possible options: `"zeros"`, `"he"`,
+                `"glorot"`, `None` (defaut)
+            activation (str): activation function $f$, possible options: `"tanh"`,
+                `"relu"`, `"sigmoid"`, `"softplus"`, `None` (defaut)
+        """
+        if not isinstance(input, Layer):
+            raise TypeError(f"input  must be a Layer object. input type={type(input)}")
+        DenseLayer.__init__(
+            self, name, input.output, input.n_out, 1, init_type, activation, **kwargs
+        )
+
+        def __repr__(self):
+            return f"TNBetaLayer({self.name}, {self.output})"
+
+        def __call__(self):
+            return DenseLayer.__call__(self)
 
 
 class BatchNormLayer(Layer):
     def __init__(self, gamma, beta, batch_size, factor=0.05, epsilon=1e-6):
         """Class object for Batch Normalization layer
 
         Args:
@@ -108,16 +182,18 @@
         self.input = input
 
         # variance and mean of each batch of input during training
         batch_var = aet.var(self.input, axis=1)
         batch_mean = aet.mean(self.input, axis=1)
 
         # updates for the running mean and variance values
-        ema_var = exp_mov_average(batch_var, self._mv_mean, alpha=self.factor)
-        ema_mean = exp_mov_average(batch_mean, self._mv_var, alpha=self.factor)
+        ema_var = functions.exp_mov_average(batch_var, self._mv_mean, alpha=self.factor)
+        ema_mean = functions.exp_mov_average(
+            batch_mean, self._mv_var, alpha=self.factor
+        )
         self._updates.append((self._mv_var, ema_mean))
         self._updates.append((self._mv_mean, ema_var))
 
         # condition when training
         batch_std = aet.shape_padaxis(aet.sqrt(batch_var + self.epsilon), 1)
         h = (self.input - aet.shape_padaxis(batch_mean, 1)) / batch_std
         batch_norm = self.gamma() * h.swapaxes(0, -1) + self.beta()
```

### Comparing `pycmtensor-1.5.0/pycmtensor/optimizers.py` & `pycmtensor-1.6.0/pycmtensor/optimizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # optimizers.py
 """PyCMTensor optimizers module"""
 import aesara
 import aesara.tensor as aet
 from aesara import shared
 from aesara.ifelse import ifelse
 
-from pycmtensor.expressions import Beta
+import pycmtensor.defaultconfig as defaultconfig
+
+config = defaultconfig.config
 
 FLOATX = aesara.config.floatX
 
 __all__ = [
     "Adam",
     "Nadam",
     "Adamax",
     "Adadelta",
     "RMSProp",
+    "RProp",
     "Momentum",
     "NAG",
     "AdaGrad",
     "SGD",
-    "BFGS",
+    "SQNBFGS",
 ]
 
 
 class Optimizer:
     def __init__(self, name, epsilon=1e-8, **kwargs):
         """Base optimizer class
 
@@ -295,14 +298,64 @@
             updates.append((param, p_t))
             updates.append((accu, accu_t))
             updates.append((d, d_t))
 
         return updates
 
 
+class RProp(Optimizer):
+    def __init__(self, params, inc=1.05, dec=0.5, bounds=[1e-6, 50.0], **kwargs):
+        """An optimizer that implements the Rprop algorithm[^1]
+
+        Args:
+            params (list[TensorSharedVariable]): parameters of the model
+            inc (float, optional): increment step if same gradient direction
+            dec (float, optional): decrement step if different gradient direction
+            bounds (List[float]): min and maximum bounds for increment step
+
+        Attributes:
+            factor (List[TensorVariable]): learning rate factor multiplier (init=1.)
+            ghat (List[TensorVariable]): previous step gradients
+
+        [^1]: Igel, C., & Hüsken, M. (2003). Empirical evaluation of the improved Rprop learning algorithms. Neurocomputing, 50, 105-123.
+        """
+        super().__init__(name="RProp")
+        self.inc = inc
+        self.dec = dec
+        self.bounds = bounds
+
+        self._ghat = [
+            shared(aet.zeros_like(p()).eval()) for p in params if p.status != 1
+        ]
+        self._factor = [
+            shared(aet.ones_like(p()).eval()) for p in params if p.status != 1
+        ]
+
+    def update(self, cost, params, lr):
+        bounds = [(p.lb, p.ub) for p in params if p.status != 1]
+        params = [p() for p in params if p.status != 1]
+        grads = aet.grad(cost, params, disconnected_inputs="ignore")
+
+        updates = []
+        for param, grad, gh, f in zip(params, grads, self._ghat, self._factor):
+            if aet.gt(grad * gh, 0.0):
+                f_new = aet.clip(f * self.inc, *self.bounds)
+            elif aet.lt(grad * gh, 0.0):
+                f_new = aet.clip(f * self.dec, *self.bounds)
+            else:
+                f_new = f
+            p_t = param - lr * f_new * grad
+
+            updates.append((gh, grad))
+            updates.append((param, p_t))
+            updates.append((f, f_new))
+
+        return updates
+
+
 class RMSProp(Optimizer):
     def __init__(self, params, rho=0.9, **kwargs):
         """An optimizer that implements the RMSprop algorithm[^1]
 
         Args:
             params (list[TensorSharedVariable]): parameters of the model
             rho (float, optional): discounting factor for the history/coming gradient.
@@ -486,95 +539,102 @@
             p_t = clip(p_t, *b)
 
             updates.append((param, p_t))
 
         return updates
 
 
-class BFGS(Optimizer):
+class SQNBFGS(Optimizer):
     def __init__(self, params, config=None, **kwargs):
-        """An optimizer that implements the stochastic gradient algorithm
+        """A L-BFGS optimizer implementing the adaptive stochastic Quasi-Newton (SQN) based approach [^1]
 
         Args:
             params (list[TensorSharedVariable]): parameters of the model
             config (pycmtensor.config): pycmtensor config object
+
+        [^1]: Byrd, R. H., Hansen, S. L., Nocedal, J., & Singer, Y. (2016). A stochastic quasi-Newton method for large-scale optimization. SIAM Journal on Optimization, 26(2), 1008-1031.
         """
         super().__init__(name="BFGS")
         if config is not None:
-            if hasattr(config, "BFGS_warmup"):
-                self.warmup = aesara.shared(config.BFGS_warmup)
-            else:
-                raise KeyError
+            self.warmup = config.BFGS_warmup
+        else:
+            self.warmup = 20
 
         self._t = aesara.shared(1.0)
         self._y = [
-            shared(aet.zeros_like(p()).eval())
-            for p in params
-            if ((p.status != 1) and (isinstance(p, Beta)))
-        ]
-        self._s = [
-            shared(p().eval())
-            for p in params
-            if ((p.status != 1) and (isinstance(p, Beta)))
+            shared(aet.zeros_like(p()).eval()) for p in params if (p.status != 1)
         ]
         self._accu = [
-            shared(aet.zeros_like(p()).eval())
-            for p in params
-            if ((p.status != 1) and (isinstance(p, Beta)))
+            shared(aet.zeros_like(p()).eval()) for p in params if p.status != 1
         ]
-        self._H0 = aesara.shared(aet.eye(len(self._y), dtype=FLOATX).eval())
 
+        self._s = [shared(p().eval()) for p in params if (p.status != 1)]
+        self._yhat = [shared(p().eval()) for p in params if (p.status != 1)]
+
+        self._H0 = aesara.shared(aet.eye(len(self._y), dtype=FLOATX).eval())
         self.I = aesara.shared(aet.eye(len(self._y), dtype=FLOATX).eval())
 
     def update(self, cost, params, lr):
         T = self.warmup
         bounds = [(p.lb, p.ub) for p in params if p.status != 1]
         params = [p() for p in params if p.status != 1]
         grads = aet.grad(cost, params, disconnected_inputs="ignore")
 
         updates = []
-        for n, (param, grad, s, y, b) in enumerate(
-            zip(params, grads, self._s, self._y, bounds)
+        for n, (param, grad, s, y, yh, a, b) in enumerate(
+            zip(params, grads, self._s, self._y, self._yhat, self._accu, bounds)
         ):
+            # perform warm up for a few runs
             B = ifelse(
                 aet.lt(self._t, 2 * T),
                 then_branch=grad,
-                else_branch=aet.sum(self._H0[n, :] * grad),
+                else_branch=aet.sum(self._H0[n, n] * grad),
             )
+            # B = aet.sum(self._H0[n, n] * grad)
+
+            a_t = a + aet.sqr(B)
+            updates.append((a, a_t))
 
-            p_t = param - lr * B
+            p_t = param - lr / aet.sqrt(a_t + self.epsilon) * B
             p_t = clip(p_t, *b)
             updates.append((param, p_t))
 
-            s_new = param - s
+            s_new = p_t - param
             updates.append((s, s_new))
 
-            y_new = grad - y
+            yh_t = grad
+            updates.append((yh, yh_t))
+
+            y_new = grad - yh
             updates.append((y, y_new))
 
+        # BFGS update algorithm
         s_t = aet.atleast_2d(self._s, left=False)
         y_t = aet.atleast_2d(self._y, left=False)
         rho_t = 1 / (s_t.T @ y_t)
         li = self.I - rho_t * (s_t @ y_t.T)
         ri = self.I - rho_t * (y_t @ s_t.T)
         h_res = rho_t * (s_t @ s_t.T)
+
+        # update hessian only every T steps to save computational time
         H_new = ifelse(
             aet.ge(self._t, T) * aet.eq(self._t % T, 0),
             then_branch=li @ self._H0 @ ri + h_res,
             else_branch=self._H0,
         )
+        # H_new = li @ self._H0 @ ri + h_res
         updates.append((self._H0, H_new))
 
         updates.append((self._t, self._t + 1))
 
         return updates
 
 
 def clip(param, min, max):
-    if any([min, max]):
+    if any([min, max]) and (config.beta_clipping):
         if min is None:
             min = -9999.0
         if max is None:
             max = 9999.0
         return aet.clip(param, min, max)
     else:
         return param
```

### Comparing `pycmtensor-1.5.0/pycmtensor/pycmtensor.py` & `pycmtensor-1.6.0/pycmtensor/pycmtensor.py`

 * *Files identical despite different names*

### Comparing `pycmtensor-1.5.0/pycmtensor/results.py` & `pycmtensor-1.6.0/pycmtensor/results.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # results.py
 """PyCMTensor results module"""
 import numpy as np
 import pandas as pd
 from numpy import nan_to_num as nan2num
 
+import pycmtensor.models.layers as layers
 from pycmtensor.expressions import Beta
 from pycmtensor.statistics import *
 
 __all__ = ["Results"]
 
 
 class Results:
@@ -26,17 +27,15 @@
         self.best_loglikelihood = -np.inf
         self.best_valid_error = 1.0
         self.best_step = 0
 
         self.gnorm = None
         self.hessian_matrix = None
         self.bhhh_matrix = None
-        self.params = None
         self.betas = None
-        self.weights = None
 
         self.performance_graph = None
         self.lr_history_graph = None
 
     def rho_square(self):
         """Returns the rho square statistics"""
         return nan2num(1.0 - self.best_loglikelihood / self.null_loglikelihood)
@@ -85,58 +84,55 @@
         stats.loc["Bayesian Information Criterion"] = self.BIC()
         stats.loc["Final gradient norm"] = f"{self.gnorm:.5e}"
         return stats
 
     def beta_statistics(self):
         """Returns a pandas DataFrame of the model beta statistics"""
         n = len(self.hessian_matrix)
-        betas = [p for p in self.params if isinstance(p, Beta)]
         h = self.hessian_matrix.sum(axis=0)
         bh = self.bhhh_matrix.sum(axis=0)
 
         stats = pd.DataFrame(
-            index=[b.name for b in betas if (b.status != 1)], columns=["value"]
-        )
-        stats["std err"] = stderror(h, betas)
-        stats["t-test"] = t_test(stats["std err"], betas)
-        stats["p-value"] = p_value(stats["std err"], betas)
-
-        stats["rob. std err"] = rob_stderror(h, bh, betas)
-        stats["rob. t-test"] = t_test(stats["rob. std err"], betas)
-        stats["rob. p-value"] = p_value(stats["rob. std err"], betas)
-        stats.drop("value", axis=1, inplace=True)
-
-        df = pd.DataFrame(
-            data=[b().eval() for b in betas],
-            index=[b.name for b in betas],
+            index=self.betas,
+            data=[value.mean() for _, value in self.betas.items()],
             columns=["value"],
         )
-        stats = pd.concat([df, stats], axis=1).sort_index().fillna("-").astype("O")
 
+        stats["std err"] = stderror(h, self.betas)
+        stats["t-test"] = t_test(stats["std err"], self.betas)
+        stats["p-value"] = p_value(stats["std err"], self.betas)
+
+        stats["rob. std err"] = rob_stderror(h, bh, self.betas)
+        stats["rob. t-test"] = t_test(stats["rob. std err"], self.betas)
+        stats["rob. p-value"] = p_value(stats["rob. std err"], self.betas)
+
+        for key, value in self.betas.items():
+            if value.shape != ():
+                stats.at[key + " (sd)", "value"] = value.std()
+
+        stats = stats.sort_index().fillna("-").astype("O")
         return stats
 
     def model_correlation_matrix(self):
         """Returns a pandas DataFrame of the model correlation matrix"""
-        betas = [p for p in self.params if isinstance(p, Beta)]
         h = self.hessian_matrix.sum(axis=0)
 
         mat = pd.DataFrame(
-            columns=[b.name for b in betas if (b.status != 1)],
-            index=[b.name for b in betas if (b.status != 1)],
+            columns=self.betas,
+            index=self.betas,
             data=correlation_matrix(h),
         )
 
         return mat
 
     def model_robust_correlation_matrix(self):
         """Returns a pandas DataFrame of the model (robust) correlation matrix"""
-        betas = [p for p in self.params if isinstance(p, Beta)]
         h = self.hessian_matrix.sum(axis=0)
         bh = self.bhhh_matrix.sum(axis=0)
 
         mat = pd.DataFrame(
-            columns=[b.name for b in betas if (b.status != 1)],
-            index=[b.name for b in betas if (b.status != 1)],
+            columns=self.betas,
+            index=self.betas,
             data=rob_correlation_matrix(h, bh),
         )
 
         return mat
```

### Comparing `pycmtensor-1.5.0/pycmtensor/scheduler.py` & `pycmtensor-1.6.0/pycmtensor/scheduler.py`

 * *Files identical despite different names*

### Comparing `pycmtensor-1.5.0/pycmtensor/statistics.py` & `pycmtensor-1.6.0/pycmtensor/statistics.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     """
     cr = variance_covariance(h)
     return cr.dot(bh.dot(cr))
 
 
 def t_test(stderr, params):
     """Returns the t stats of ``params`` given the standard error (``stderr``)"""
-    params = [p() for p in params if (p.status != 1)]
-    return [p.eval() / s for p, s in zip(params, stderr)]
+    params = [value for key, value in params.items()]
+    return [p.mean() / s for p, s in zip(params, stderr)]
 
 
 def p_value(stderr, params):
     """Returns the p-value of ``params`` given the standard error (``stderr``)"""
     tTest = t_test(stderr, params)
     return [2.0 * (1.0 - stats.norm.cdf(abs(t))) for t in tTest]
 
@@ -46,35 +46,39 @@
 def stderror(h, params):
     """Returns the standard error of ``params`` given the Hessian (``h``)
 
     The std err is calculated as the square root of the variance covariance
     matrix.
 
     """
-    params = [p() for p in params if (p.status != 1)]
+    # params = [p for p in params if (p.status != 1)]
     varCovar = variance_covariance(h)
     stdErr = []
-    for i in range(len(params)):
-        if varCovar[i, i] < 0:
+    for i, p in enumerate(params):
+        if (params[p].shape == ()) and (params[p] == 0.0):
+            stdErr.append(np.nan)
+        elif varCovar[i, i] < 0:
             stdErr.append(np.finfo(float).max)
         else:
             stdErr.append(np.sqrt(varCovar[i, i] + 1e-8))  # for numerical stability
 
     return stdErr
 
 
 def rob_stderror(h, bh, params):
     """Returns the rob. standard error of ``params`` given the Hessian (``h``) and the
     BHHH matrix (``bh``)
     """
-    params = [p() for p in params if (p.status != 1)]
+    # params = [p for p in params if (p.status != 1)]
     robVarCovar = rob_variance_covariance(h, bh)
     robstderr = []
-    for i in range(len(params)):
-        if robVarCovar[i, i] < 0:
+    for i, p in enumerate(params):
+        if (params[p].shape == ()) and (params[p] == 0.0):
+            robstderr.append(np.nan)
+        elif robVarCovar[i, i] < 0:
             robstderr.append(np.finfo(float).max)
         else:
             robstderr.append(np.sqrt(robVarCovar[i, i] + 1e-8))
 
     return robstderr
```

### Comparing `pycmtensor-1.5.0/pyproject.toml` & `pycmtensor-1.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycmtensor"
-version = "1.5.0"
+version = "1.6.0"
 description = "Python Tensor based package for discrete choice modelling."
 authors = ["Melvin Wong <m.j.w.wong@tue.nl>"]
 license = "MIT"
 readme = "README.md"
 
 homepage = ""
 repository = "https://github.com/mwong009/pycmtensor"
@@ -69,15 +69,15 @@
 [tool.black]
 line-length = 88
 target-version = ["py311"]
 quiet = false
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.5.0"
+version = "1.6.0"
 tag_format = "v$version"
 version_files = [
     "pyproject.toml:version",
     "pycmtensor/__init__.py",
 ]
 
 [tool.pytest]
```

### Comparing `pycmtensor-1.5.0/PKG-INFO` & `pycmtensor-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycmtensor
-Version: 1.5.0
+Version: 1.6.0
 Summary: Python Tensor based package for discrete choice modelling.
 Home-page: https://github.com/mwong009/pycmtensor
 License: MIT
 Author: Melvin Wong
 Author-email: m.j.w.wong@tue.nl
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 4 - Beta
```

