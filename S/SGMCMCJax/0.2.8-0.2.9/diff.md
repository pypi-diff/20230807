# Comparing `tmp/SGMCMCJax-0.2.8.tar.gz` & `tmp/SGMCMCJax-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SGMCMCJax-0.2.8.tar", last modified: Sun Oct  3 15:41:56 2021, max compression
+gzip compressed data, was "dist/SGMCMCJax-0.2.9.tar", last modified: Tue Oct  5 18:18:12 2021, max compression
```

## Comparing `SGMCMCJax-0.2.8.tar` & `SGMCMCJax-0.2.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 jeremiecoullon   (501) staff       (20)        0 2021-10-03 15:41:56.728146 SGMCMCJax-0.2.8/
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)     3144 2021-10-03 15:41:56.728338 SGMCMCJax-0.2.8/PKG-INFO
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)     2124 2021-08-13 10:19:55.000000 SGMCMCJax-0.2.8/README.md
-drwxr-xr-x   0 jeremiecoullon   (501) staff       (20)        0 2021-10-03 15:41:56.712221 SGMCMCJax-0.2.8/SGMCMCJax.egg-info/
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)     3144 2021-10-03 15:41:56.000000 SGMCMCJax-0.2.8/SGMCMCJax.egg-info/PKG-INFO
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)      742 2021-10-03 15:41:56.000000 SGMCMCJax-0.2.8/SGMCMCJax.egg-info/SOURCES.txt
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)        1 2021-10-03 15:41:56.000000 SGMCMCJax-0.2.8/SGMCMCJax.egg-info/dependency_links.txt
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)      135 2021-10-03 15:41:56.000000 SGMCMCJax-0.2.8/SGMCMCJax.egg-info/requires.txt
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)       19 2021-10-03 15:41:56.000000 SGMCMCJax-0.2.8/SGMCMCJax.egg-info/top_level.txt
-drwxr-xr-x   0 jeremiecoullon   (501) staff       (20)        0 2021-10-03 15:41:56.715703 SGMCMCJax-0.2.8/examples/
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)        0 2021-10-03 15:41:43.000000 SGMCMCJax-0.2.8/examples/__init__.py
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)      924 2021-10-03 15:41:43.000000 SGMCMCJax-0.2.8/examples/gauss_optimize.py
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)      807 2021-10-03 15:41:43.000000 SGMCMCJax-0.2.8/examples/gauss_sample_sgld.py
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)     1951 2021-10-03 15:41:43.000000 SGMCMCJax-0.2.8/examples/sgmcmc_nuts_demo.py
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)     3884 2021-10-03 15:41:43.000000 SGMCMCJax-0.2.8/examples/sgmcmc_utils.py
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)      102 2021-10-03 15:41:56.728919 SGMCMCJax-0.2.8/setup.cfg
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)     1002 2021-10-03 15:41:43.000000 SGMCMCJax-0.2.8/setup.py
-drwxr-xr-x   0 jeremiecoullon   (501) staff       (20)        0 2021-10-03 15:41:56.724456 SGMCMCJax-0.2.8/sgmcmcjax/
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)       22 2021-10-03 15:41:43.000000 SGMCMCJax-0.2.8/sgmcmcjax/__init__.py
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)     5490 2021-09-28 15:34:24.000000 SGMCMCJax-0.2.8/sgmcmcjax/diffusion_util.py
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)     5795 2021-08-13 10:09:11.000000 SGMCMCJax-0.2.8/sgmcmcjax/diffusions.py
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)     4720 2021-09-28 15:34:24.000000 SGMCMCJax-0.2.8/sgmcmcjax/gradient_estimation.py
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)     9730 2021-08-23 16:15:54.000000 SGMCMCJax-0.2.8/sgmcmcjax/kernels.py
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)     1105 2021-07-05 15:20:47.000000 SGMCMCJax-0.2.8/sgmcmcjax/ksd.py
-drwxr-xr-x   0 jeremiecoullon   (501) staff       (20)        0 2021-10-03 15:41:56.725423 SGMCMCJax-0.2.8/sgmcmcjax/models/
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)        0 2021-10-03 15:13:51.000000 SGMCMCJax-0.2.8/sgmcmcjax/models/__init__.py
-drwxr-xr-x   0 jeremiecoullon   (501) staff       (20)        0 2021-10-03 15:41:56.727921 SGMCMCJax-0.2.8/sgmcmcjax/models/bayesian_NN/
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)     1256 2021-10-03 15:13:51.000000 SGMCMCJax-0.2.8/sgmcmcjax/models/bayesian_NN/NN_data.py
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)     1583 2021-10-03 15:13:51.000000 SGMCMCJax-0.2.8/sgmcmcjax/models/bayesian_NN/NN_model.py
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)        0 2021-10-03 15:13:51.000000 SGMCMCJax-0.2.8/sgmcmcjax/models/bayesian_NN/__init__.py
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)     1856 2021-10-03 15:13:51.000000 SGMCMCJax-0.2.8/sgmcmcjax/models/logistic_regression.py
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)     2317 2021-10-03 15:41:43.000000 SGMCMCJax-0.2.8/sgmcmcjax/optimizer.py
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)     3692 2021-09-28 16:08:13.000000 SGMCMCJax-0.2.8/sgmcmcjax/samplers.py
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)      890 2021-09-28 15:34:24.000000 SGMCMCJax-0.2.8/sgmcmcjax/types.py
--rw-r--r--   0 jeremiecoullon   (501) staff       (20)     3197 2021-08-12 15:22:16.000000 SGMCMCJax-0.2.8/sgmcmcjax/util.py
+drwxr-xr-x   0 jeremiecoullon   (501) staff       (20)        0 2021-10-05 18:18:12.102155 SGMCMCJax-0.2.9/
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)     3144 2021-10-05 18:18:12.102300 SGMCMCJax-0.2.9/PKG-INFO
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)     2124 2021-08-13 10:19:55.000000 SGMCMCJax-0.2.9/README.md
+drwxr-xr-x   0 jeremiecoullon   (501) staff       (20)        0 2021-10-05 18:18:12.091611 SGMCMCJax-0.2.9/SGMCMCJax.egg-info/
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)     3144 2021-10-05 18:18:11.000000 SGMCMCJax-0.2.9/SGMCMCJax.egg-info/PKG-INFO
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)      792 2021-10-05 18:18:11.000000 SGMCMCJax-0.2.9/SGMCMCJax.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)        1 2021-10-05 18:18:11.000000 SGMCMCJax-0.2.9/SGMCMCJax.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)      135 2021-10-05 18:18:11.000000 SGMCMCJax-0.2.9/SGMCMCJax.egg-info/requires.txt
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)       10 2021-10-05 18:18:11.000000 SGMCMCJax-0.2.9/SGMCMCJax.egg-info/top_level.txt
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)      102 2021-10-05 18:18:12.102749 SGMCMCJax-0.2.9/setup.cfg
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)     1002 2021-10-05 18:18:02.000000 SGMCMCJax-0.2.9/setup.py
+drwxr-xr-x   0 jeremiecoullon   (501) staff       (20)        0 2021-10-05 18:18:12.097005 SGMCMCJax-0.2.9/sgmcmcjax/
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)       22 2021-10-05 18:18:02.000000 SGMCMCJax-0.2.9/sgmcmcjax/__init__.py
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)     5490 2021-09-28 15:34:24.000000 SGMCMCJax-0.2.9/sgmcmcjax/diffusion_util.py
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)     5795 2021-10-03 17:42:02.000000 SGMCMCJax-0.2.9/sgmcmcjax/diffusions.py
+drwxr-xr-x   0 jeremiecoullon   (501) staff       (20)        0 2021-10-05 18:18:12.099179 SGMCMCJax-0.2.9/sgmcmcjax/examples/
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)        0 2021-10-05 18:18:02.000000 SGMCMCJax-0.2.9/sgmcmcjax/examples/__init__.py
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)      924 2021-10-05 18:18:02.000000 SGMCMCJax-0.2.9/sgmcmcjax/examples/gauss_optimize.py
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)      807 2021-10-05 18:18:02.000000 SGMCMCJax-0.2.9/sgmcmcjax/examples/gauss_sample_sgld.py
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)     1983 2021-10-05 18:18:02.000000 SGMCMCJax-0.2.9/sgmcmcjax/examples/sgmcmc_nuts_demo.py
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)     2709 2021-10-05 18:18:02.000000 SGMCMCJax-0.2.9/sgmcmcjax/examples/sgmcmc_utils.py
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)     4720 2021-09-28 15:34:24.000000 SGMCMCJax-0.2.9/sgmcmcjax/gradient_estimation.py
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)     9730 2021-08-23 16:15:54.000000 SGMCMCJax-0.2.9/sgmcmcjax/kernels.py
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)     1105 2021-07-05 15:20:47.000000 SGMCMCJax-0.2.9/sgmcmcjax/ksd.py
+drwxr-xr-x   0 jeremiecoullon   (501) staff       (20)        0 2021-10-05 18:18:12.099928 SGMCMCJax-0.2.9/sgmcmcjax/models/
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)        0 2021-10-03 15:13:51.000000 SGMCMCJax-0.2.9/sgmcmcjax/models/__init__.py
+drwxr-xr-x   0 jeremiecoullon   (501) staff       (20)        0 2021-10-05 18:18:12.101961 SGMCMCJax-0.2.9/sgmcmcjax/models/bayesian_NN/
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)     1256 2021-10-03 15:13:51.000000 SGMCMCJax-0.2.9/sgmcmcjax/models/bayesian_NN/NN_data.py
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)     1583 2021-10-03 15:13:51.000000 SGMCMCJax-0.2.9/sgmcmcjax/models/bayesian_NN/NN_model.py
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)        0 2021-10-03 15:13:51.000000 SGMCMCJax-0.2.9/sgmcmcjax/models/bayesian_NN/__init__.py
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)     1856 2021-10-03 15:13:51.000000 SGMCMCJax-0.2.9/sgmcmcjax/models/logistic_regression.py
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)     2317 2021-10-03 15:41:43.000000 SGMCMCJax-0.2.9/sgmcmcjax/optimizer.py
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)     3692 2021-09-28 16:08:13.000000 SGMCMCJax-0.2.9/sgmcmcjax/samplers.py
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)      890 2021-09-28 15:34:24.000000 SGMCMCJax-0.2.9/sgmcmcjax/types.py
+-rw-r--r--   0 jeremiecoullon   (501) staff       (20)     3197 2021-08-12 15:22:16.000000 SGMCMCJax-0.2.9/sgmcmcjax/util.py
```

### Comparing `SGMCMCJax-0.2.8/PKG-INFO` & `SGMCMCJax-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SGMCMCJax
-Version: 0.2.8
+Version: 0.2.9
 Summary: SGMCMC samplers in JAX
 Home-page: https://github.com/jeremiecoullon/SGMCMCJax
 Author: Jeremie Coullon
 Author-email: jeremie.coullon@gmail.com
 License: LICENSE.txt
 Description: # SGMCMCJax
```

### Comparing `SGMCMCJax-0.2.8/README.md` & `SGMCMCJax-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `SGMCMCJax-0.2.8/SGMCMCJax.egg-info/PKG-INFO` & `SGMCMCJax-0.2.9/SGMCMCJax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SGMCMCJax
-Version: 0.2.8
+Version: 0.2.9
 Summary: SGMCMC samplers in JAX
 Home-page: https://github.com/jeremiecoullon/SGMCMCJax
 Author: Jeremie Coullon
 Author-email: jeremie.coullon@gmail.com
 License: LICENSE.txt
 Description: # SGMCMCJax
```

### Comparing `SGMCMCJax-0.2.8/SGMCMCJax.egg-info/SOURCES.txt` & `SGMCMCJax-0.2.9/SGMCMCJax.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 setup.cfg
 setup.py
 SGMCMCJax.egg-info/PKG-INFO
 SGMCMCJax.egg-info/SOURCES.txt
 SGMCMCJax.egg-info/dependency_links.txt
 SGMCMCJax.egg-info/requires.txt
 SGMCMCJax.egg-info/top_level.txt
-examples/__init__.py
-examples/gauss_optimize.py
-examples/gauss_sample_sgld.py
-examples/sgmcmc_nuts_demo.py
-examples/sgmcmc_utils.py
 sgmcmcjax/__init__.py
 sgmcmcjax/diffusion_util.py
 sgmcmcjax/diffusions.py
 sgmcmcjax/gradient_estimation.py
 sgmcmcjax/kernels.py
 sgmcmcjax/ksd.py
 sgmcmcjax/optimizer.py
 sgmcmcjax/samplers.py
 sgmcmcjax/types.py
 sgmcmcjax/util.py
+sgmcmcjax/examples/__init__.py
+sgmcmcjax/examples/gauss_optimize.py
+sgmcmcjax/examples/gauss_sample_sgld.py
+sgmcmcjax/examples/sgmcmc_nuts_demo.py
+sgmcmcjax/examples/sgmcmc_utils.py
 sgmcmcjax/models/__init__.py
 sgmcmcjax/models/logistic_regression.py
 sgmcmcjax/models/bayesian_NN/NN_data.py
 sgmcmcjax/models/bayesian_NN/NN_model.py
 sgmcmcjax/models/bayesian_NN/__init__.py
```

### Comparing `SGMCMCJax-0.2.8/examples/gauss_optimize.py` & `SGMCMCJax-0.2.9/sgmcmcjax/examples/gauss_optimize.py`

 * *Files identical despite different names*

### Comparing `SGMCMCJax-0.2.8/examples/gauss_sample_sgld.py` & `SGMCMCJax-0.2.9/sgmcmcjax/examples/gauss_sample_sgld.py`

 * *Files identical despite different names*

### Comparing `SGMCMCJax-0.2.8/examples/sgmcmc_nuts_demo.py` & `SGMCMCJax-0.2.9/sgmcmcjax/examples/sgmcmc_nuts_demo.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from jax.lax import scan
 from jax import vmap, jit, random
 import jax.numpy as jnp
 import optax
 
 from blackjax import nuts, stan_warmup
 from sgmcmcjax.samplers import build_sgld_sampler
-from sgmcmc_utils import build_nuts_sampler, build_optax_optimizer
+from .sgmcmc_utils import build_nuts_sampler
+from sgmcmcjax.optimizer import build_optax_optimizer
 
 # We use the 'quickstart' example from
 # https://github.com/jeremiecoullon/SGMCMCJax
 
 def loglikelihood(theta, x):
     return -0.5*jnp.dot(x-theta, x-theta)
```

### Comparing `SGMCMCJax-0.2.8/setup.py` & `SGMCMCJax-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         "matplotlib==3.3.3",
         "sphinx-copybutton==0.3.5",
     ],
 }
 
 setup(
     name='SGMCMCJax',
-    version='0.2.8',
+    version='0.2.9',
     author='Jeremie Coullon',
     author_email='jeremie.coullon@gmail.com',
     packages=find_packages(".", exclude=["tests"]),
     license='LICENSE.txt',
     description='SGMCMC samplers in JAX',
     long_description=README,
     long_description_content_type="text/markdown",
```

### Comparing `SGMCMCJax-0.2.8/sgmcmcjax/diffusion_util.py` & `SGMCMCJax-0.2.9/sgmcmcjax/diffusion_util.py`

 * *Files identical despite different names*

### Comparing `SGMCMCJax-0.2.8/sgmcmcjax/diffusions.py` & `SGMCMCJax-0.2.9/sgmcmcjax/diffusions.py`

 * *Files identical despite different names*

### Comparing `SGMCMCJax-0.2.8/sgmcmcjax/gradient_estimation.py` & `SGMCMCJax-0.2.9/sgmcmcjax/gradient_estimation.py`

 * *Files identical despite different names*

### Comparing `SGMCMCJax-0.2.8/sgmcmcjax/kernels.py` & `SGMCMCJax-0.2.9/sgmcmcjax/kernels.py`

 * *Files identical despite different names*

### Comparing `SGMCMCJax-0.2.8/sgmcmcjax/ksd.py` & `SGMCMCJax-0.2.9/sgmcmcjax/ksd.py`

 * *Files identical despite different names*

### Comparing `SGMCMCJax-0.2.8/sgmcmcjax/models/bayesian_NN/NN_data.py` & `SGMCMCJax-0.2.9/sgmcmcjax/models/bayesian_NN/NN_data.py`

 * *Files identical despite different names*

### Comparing `SGMCMCJax-0.2.8/sgmcmcjax/models/bayesian_NN/NN_model.py` & `SGMCMCJax-0.2.9/sgmcmcjax/models/bayesian_NN/NN_model.py`

 * *Files identical despite different names*

### Comparing `SGMCMCJax-0.2.8/sgmcmcjax/models/logistic_regression.py` & `SGMCMCJax-0.2.9/sgmcmcjax/models/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `SGMCMCJax-0.2.8/sgmcmcjax/optimizer.py` & `SGMCMCJax-0.2.9/sgmcmcjax/optimizer.py`

 * *Files identical despite different names*

### Comparing `SGMCMCJax-0.2.8/sgmcmcjax/samplers.py` & `SGMCMCJax-0.2.9/sgmcmcjax/samplers.py`

 * *Files identical despite different names*

### Comparing `SGMCMCJax-0.2.8/sgmcmcjax/types.py` & `SGMCMCJax-0.2.9/sgmcmcjax/types.py`

 * *Files identical despite different names*

### Comparing `SGMCMCJax-0.2.8/sgmcmcjax/util.py` & `SGMCMCJax-0.2.9/sgmcmcjax/util.py`

 * *Files identical despite different names*

