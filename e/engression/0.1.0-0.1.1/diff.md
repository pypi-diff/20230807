# Comparing `tmp/engression-0.1.0.tar.gz` & `tmp/engression-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "engression-0.1.0.tar", last modified: Fri Aug  4 12:08:46 2023, max compression
+gzip compressed data, was "engression-0.1.1.tar", last modified: Mon Aug  7 06:42:42 2023, max compression
```

## Comparing `engression-0.1.0.tar` & `engression-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 shenxi   (571559) staff       (20)        0 2023-08-04 12:08:46.120067 engression-0.1.0/
--rw-r--r--   0 shenxi   (571559) staff       (20)     1522 2023-07-06 08:06:16.000000 engression-0.1.0/LICENSE
--rw-r--r--   0 shenxi   (571559) staff       (20)     3192 2023-08-04 12:08:46.119933 engression-0.1.0/PKG-INFO
--rw-r--r--   0 shenxi   (571559) staff       (20)     2876 2023-08-04 10:06:11.000000 engression-0.1.0/README.md
-drwxr-xr-x   0 shenxi   (571559) staff       (20)        0 2023-08-04 12:08:46.118685 engression-0.1.0/engression/
--rw-r--r--   0 shenxi   (571559) staff       (20)      363 2023-08-01 07:59:51.000000 engression-0.1.0/engression/__init__.py
-drwxr-xr-x   0 shenxi   (571559) staff       (20)        0 2023-08-04 12:08:46.119778 engression-0.1.0/engression/data/
--rw-r--r--   0 shenxi   (571559) staff       (20)        0 2023-07-01 15:22:34.000000 engression-0.1.0/engression/data/__init__.py
--rw-r--r--   0 shenxi   (571559) staff       (20)     1980 2023-07-01 15:22:34.000000 engression-0.1.0/engression/data/loader.py
--rw-r--r--   0 shenxi   (571559) staff       (20)     2673 2023-07-01 15:22:34.000000 engression-0.1.0/engression/data/simulator.py
--rw-r--r--   0 shenxi   (571559) staff       (20)    18122 2023-08-04 11:51:17.000000 engression-0.1.0/engression/engression.py
--rw-r--r--   0 shenxi   (571559) staff       (20)    17650 2023-08-04 12:01:31.000000 engression-0.1.0/engression/engression_bagged.py
--rw-r--r--   0 shenxi   (571559) staff       (20)     2354 2023-07-24 19:22:24.000000 engression-0.1.0/engression/loss_func.py
--rw-r--r--   0 shenxi   (571559) staff       (20)     6430 2023-07-24 19:22:41.000000 engression-0.1.0/engression/models.py
--rw-r--r--   0 shenxi   (571559) staff       (20)     1910 2023-07-02 13:49:25.000000 engression-0.1.0/engression/utils.py
-drwxr-xr-x   0 shenxi   (571559) staff       (20)        0 2023-08-04 12:08:46.119431 engression-0.1.0/engression.egg-info/
--rw-r--r--   0 shenxi   (571559) staff       (20)     3192 2023-08-04 12:08:46.000000 engression-0.1.0/engression.egg-info/PKG-INFO
--rw-r--r--   0 shenxi   (571559) staff       (20)      423 2023-08-04 12:08:46.000000 engression-0.1.0/engression.egg-info/SOURCES.txt
--rw-r--r--   0 shenxi   (571559) staff       (20)        1 2023-08-04 12:08:46.000000 engression-0.1.0/engression.egg-info/dependency_links.txt
--rw-r--r--   0 shenxi   (571559) staff       (20)       23 2023-08-04 12:08:46.000000 engression-0.1.0/engression.egg-info/requires.txt
--rw-r--r--   0 shenxi   (571559) staff       (20)       11 2023-08-04 12:08:46.000000 engression-0.1.0/engression.egg-info/top_level.txt
--rw-r--r--   0 shenxi   (571559) staff       (20)       38 2023-08-04 12:08:46.120111 engression-0.1.0/setup.cfg
--rw-r--r--   0 shenxi   (571559) staff       (20)      633 2023-08-04 12:08:01.000000 engression-0.1.0/setup.py
+drwxr-xr-x   0 shenxi   (571559) staff       (20)        0 2023-08-07 06:42:42.249768 engression-0.1.1/
+-rw-r--r--   0 shenxi   (571559) staff       (20)     1522 2023-07-06 08:06:16.000000 engression-0.1.1/LICENSE
+-rw-r--r--   0 shenxi   (571559) staff       (20)     3192 2023-08-07 06:42:42.249662 engression-0.1.1/PKG-INFO
+-rw-r--r--   0 shenxi   (571559) staff       (20)     2876 2023-08-04 10:06:11.000000 engression-0.1.1/README.md
+drwxr-xr-x   0 shenxi   (571559) staff       (20)        0 2023-08-07 06:42:42.248677 engression-0.1.1/engression/
+-rw-r--r--   0 shenxi   (571559) staff       (20)      363 2023-08-01 07:59:51.000000 engression-0.1.1/engression/__init__.py
+drwxr-xr-x   0 shenxi   (571559) staff       (20)        0 2023-08-07 06:42:42.249499 engression-0.1.1/engression/data/
+-rw-r--r--   0 shenxi   (571559) staff       (20)        0 2023-07-01 15:22:34.000000 engression-0.1.1/engression/data/__init__.py
+-rw-r--r--   0 shenxi   (571559) staff       (20)     1993 2023-08-06 20:58:00.000000 engression-0.1.1/engression/data/loader.py
+-rw-r--r--   0 shenxi   (571559) staff       (20)     2666 2023-08-06 20:58:22.000000 engression-0.1.1/engression/data/simulator.py
+-rw-r--r--   0 shenxi   (571559) staff       (20)    18341 2023-08-07 06:41:18.000000 engression-0.1.1/engression/engression.py
+-rw-r--r--   0 shenxi   (571559) staff       (20)    17590 2023-08-06 20:56:37.000000 engression-0.1.1/engression/engression_bagged.py
+-rw-r--r--   0 shenxi   (571559) staff       (20)     2354 2023-07-24 19:22:24.000000 engression-0.1.1/engression/loss_func.py
+-rw-r--r--   0 shenxi   (571559) staff       (20)     6430 2023-07-24 19:22:41.000000 engression-0.1.1/engression/models.py
+-rw-r--r--   0 shenxi   (571559) staff       (20)     1910 2023-08-06 21:03:08.000000 engression-0.1.1/engression/utils.py
+drwxr-xr-x   0 shenxi   (571559) staff       (20)        0 2023-08-07 06:42:42.249215 engression-0.1.1/engression.egg-info/
+-rw-r--r--   0 shenxi   (571559) staff       (20)     3192 2023-08-07 06:42:42.000000 engression-0.1.1/engression.egg-info/PKG-INFO
+-rw-r--r--   0 shenxi   (571559) staff       (20)      423 2023-08-07 06:42:42.000000 engression-0.1.1/engression.egg-info/SOURCES.txt
+-rw-r--r--   0 shenxi   (571559) staff       (20)        1 2023-08-07 06:42:42.000000 engression-0.1.1/engression.egg-info/dependency_links.txt
+-rw-r--r--   0 shenxi   (571559) staff       (20)       45 2023-08-07 06:42:42.000000 engression-0.1.1/engression.egg-info/requires.txt
+-rw-r--r--   0 shenxi   (571559) staff       (20)       11 2023-08-07 06:42:42.000000 engression-0.1.1/engression.egg-info/top_level.txt
+-rw-r--r--   0 shenxi   (571559) staff       (20)       38 2023-08-07 06:42:42.249802 engression-0.1.1/setup.cfg
+-rw-r--r--   0 shenxi   (571559) staff       (20)      633 2023-08-07 06:42:16.000000 engression-0.1.1/setup.py
```

### Comparing `engression-0.1.0/LICENSE` & `engression-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `engression-0.1.0/PKG-INFO` & `engression-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: engression
-Version: 0.1.0
+Version: 0.1.1
 Summary: Engression Modelling
 Home-page: https://github.com/xwshen51/engression
 Author: Xinwei Shen and Nicolai Meinshausen
 Author-email: xinwei.shen@stat.math.ethz.ch
 License: BSD 3-Clause License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `engression-0.1.0/README.md` & `engression-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `engression-0.1.0/engression/data/loader.py` & `engression-0.1.1/engression/data/loader.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 def make_dataloader(x, y, batch_size=128, shuffle=True, num_workers=0):
     """Make dataloader.
 
     Args:
         x (torch.Tensor): data of predictors.
         y (torch.Tensor): data of responses.
-        batch_size (int, optional): _description_. Defaults to 128.
-        shuffle (bool, optional): _description_. Defaults to True.
-        num_workers (int, optional): _description_. Defaults to 0.
+        batch_size (int, optional): batch size. Defaults to 128.
+        shuffle (bool, optional): whether to shuffle data. Defaults to True.
+        num_workers (int, optional): number of workers. Defaults to 0.
 
     Returns:
-        _type_: _description_
+        DataLoader: data loader
     """
     dataset = TensorDataset(x, y)
     dataloader = DataLoader(dataset, batch_size=batch_size, shuffle=shuffle, num_workers=num_workers)
     return dataloader
 
 def partition_data(x_full, y_full, cut_quantile=0.3, split_train="smaller"):
     """Partition data into training and test sets.
```

### Comparing `engression-0.1.0/engression/data/simulator.py` & `engression-0.1.1/engression/data/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         true_function (str, optional): true function g^\star. Defaults to 'softplus'. Choices: ['softplus', 'cubic','square', 'log'].
         n (int, optional): sample size. Defaults to 10000.
         x_lower (int, optional): lower bound of the training support. Defaults to 0.
         x_upper (int, optional): upper bound of the training support. Defaults to 2.
         noise_std (int, optional): standard deviation of the noise. Defaults to 1.
         noise_dist (str, optional): noise distribution. Defaults to 'gaussian'. Choices: ['gaussian', 'uniform'].
         train (bool, optional): generate data for training. Defaults to True.
-        device (str or torch.device, optional): _description_. Defaults to torch.device('cpu').
+        device (str or torch.device, optional): device. Defaults to torch.device('cpu').
 
     Returns:
         tuple of torch.Tensors: data simulated from a pre-ANM.
     """
     if isinstance(true_function, str):
         if true_function == 'softplus':
             true_function = lambda x: nn.Softplus()(x)
```

### Comparing `engression-0.1.0/engression/engression.py` & `engression-0.1.1/engression/engression.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,34 +37,33 @@
     engressor.train(x, y, num_epoches=num_epoches, batch_size=batch_size, 
                     print_every_nepoch=print_every_nepoch, print_times_per_epoch=print_times_per_epoch, 
                     standardize=standardize, verbose=verbose)
     return engressor
 
 
 class Engressor(object):
+    """Engressor class.
 
+    Args:
+        in_dim (int): input dimension
+        out_dim (int): output dimension
+        num_layer (int, optional): number of layers. Defaults to 2.
+        hidden_dim (int, optional): number of neurons per layer. Defaults to 100.
+        noise_dim (int, optional): noise dimension. Defaults to 100.
+        lr (float, optional): learning rate. Defaults to 0.001.
+        num_epoches (int, optional): number of epoches. Defaults to 500.
+        batch_size (int, optional): batch size. Defaults to None, referring to the full batch.
+        standardize (bool, optional): whether to standardize data during training. Defaults to True.
+        device (str or torch.device, optional): device. Defaults to "cpu". Choices = ["cpu", "gpu", "cuda"].
+        check_device (bool, optional): whether to check the device. Defaults to True.
+    """
     def __init__(self, 
                  in_dim, out_dim, num_layer=2, hidden_dim=100, noise_dim=100,
                  lr=0.001, num_epoches=500, batch_size=None, standardize=True, 
                  device="cpu", check_device=True): 
-        """Engressor class.
-
-        Args:
-            in_dim (int): input dimension
-            out_dim (int): output dimension
-            num_layer (int, optional): number of layers. Defaults to 2.
-            hidden_dim (int, optional): number of neurons per layer. Defaults to 100.
-            noise_dim (int, optional): noise dimension. Defaults to 100.
-            lr (float, optional): learning rate. Defaults to 0.001.
-            num_epoches (int, optional): number of epoches. Defaults to 500.
-            batch_size (int, optional): batch size. Defaults to None, referring to the full batch.
-            standardize (bool, optional): whether to standardize data during training. Defaults to True.
-            device (str or torch.device, optional): device. Defaults to "cpu". Choices = ["cpu", "gpu", "cuda"].
-            check_device (bool, optional): whether to check the device. Defaults to True.
-        """
         super().__init__()
         self.num_layer = num_layer
         self.hidden_dim = hidden_dim
         self.noise_dim = noise_dim
         self.lr = lr
         self.num_epoches = num_epoches
         self.batch_size = batch_size
@@ -119,15 +118,21 @@
         Returns:
             torch.Tensor: standardized data.
         """
         self.x_mean = torch.mean(x, dim=0)
         self.x_std = torch.std(x, dim=0)
         self.y_mean = torch.mean(y, dim=0)
         self.y_std = torch.std(y, dim=0)
-        return (x - self.x_mean) / self.x_std, (y - self.y_mean) / self.y_std
+        x_standardized = (x - self.x_mean) / self.x_std
+        y_standardized = (y - self.y_mean) / self.y_std
+        self.x_mean = self.x_mean.to(self.device)
+        self.x_std = self.x_std.to(self.device)
+        self.y_mean = self.y_mean.to(self.device)
+        self.y_std = self.y_std.to(self.device)
+        return x_standardized, y_standardized
 
     def standardize_data(self, x, y=None):
         """Standardize the data, if self.standardize is True.
 
         Args:
             x (torch.Tensor): training data of predictors.
             y (torch.Tensor, optional): _description_. Defaults to None.
@@ -185,21 +190,21 @@
         if batch_size is None:
             batch_size = self.batch_size
         if standardize:
             self.standardize = standardize
             
         x = vectorize(x)
         y = vectorize(y)
-        x = x.to(self.device)
-        y = y.to(self.device)
         if self.standardize:
             if verbose:
                 print("Data is standardized for training only; the printed training losses are on the standardized scale. \n" +
                     "However during evaluation, the predictions, evaluation metrics, and plots will be on the original scale.\n")
             x, y = self._standardize_data_and_record_stats(x, y)
+        x = x.to(self.device)
+        y = y.to(self.device)
         
         if batch_size >= x.size(0)//2:
             if verbose:
                 print("Batch is larger than half of the sample size. Training based on full-batch gradient descent.")
             self.batch_size = x.size(0)
             for epoch_idx in range(num_epoches):
                 self.model.zero_grad()
```

### Comparing `engression-0.1.0/engression/engression_bagged.py` & `engression-0.1.1/engression/engression_bagged.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,35 +37,35 @@
                                 device=device, standardize=standardize, 
                                 ensemble_size=ensemble_size, val_loss_type=val_loss_type)
     engressor.train(x, y)
     return engressor
 
 
 class BaggedEngressor(object):
+    """Bagged engressor.
+
+    Args:
+        in_dim (int): input dimension
+        out_dim (int): output dimension
+        num_layer (int, optional): number of layers. Defaults to 2.
+        hidden_dim (int, optional): number of neurons per layer. Defaults to 100.
+        noise_dim (int, optional): noise dimension. Defaults to 100.
+        lr (float, optional): learning rate. Defaults to 0.001.
+        num_epoches (int, optional): number of epoches. Defaults to 500.
+        batch_size (int, optional): batch size. Defaults to None, referring to the full batch.
+        device (str or torch.device, optional): device. Defaults to "cpu".
+        standardize (bool, optional): whether to standardize data. Defaults to True.
+        ensemble_size (int, optional): number of models for ensemble. Defaults to 10.
+        val_loss_type (str, optional): loss type for validation. Defaults to "energy". Choices: ["l1", "l2", "energy"].
+    """
     def __init__(self, 
                  in_dim, out_dim, num_layer=2, hidden_dim=100, noise_dim=100,
                  lr=0.001, num_epoches=500, batch_size=None, 
                  device="cpu", standardize=True,
                  ensemble_size=10, val_loss_type="energy"): 
-        """Bagged engressor.
-
-        Args:
-            in_dim (int): input dimension
-            out_dim (int): output dimension
-            num_layer (int, optional): number of layers. Defaults to 2.
-            hidden_dim (int, optional): number of neurons per layer. Defaults to 100.
-            noise_dim (int, optional): noise dimension. Defaults to 100.
-            lr (float, optional): learning rate. Defaults to 0.001.
-            num_epoches (int, optional): number of epoches. Defaults to 500.
-            batch_size (int, optional): batch size. Defaults to None, referring to the full batch.
-            device (str or torch.device, optional): device. Defaults to "cpu".
-            standardize (bool, optional): whether to standardize data. Defaults to True.
-            ensemble_size (int, optional): number of models for ensemble. Defaults to 10.
-            val_loss_type (str, optional): loss type for validation. Defaults to "energy". Choices: ["l1", "l2", "energy"].
-        """
         super().__init__()
         self.num_layer = num_layer
         self.hidden_dim = hidden_dim
         self.noise_dim = noise_dim
         self.lr = lr
         self.num_epoches = num_epoches
         self.batch_size = batch_size
```

### Comparing `engression-0.1.0/engression/loss_func.py` & `engression-0.1.1/engression/loss_func.py`

 * *Files identical despite different names*

### Comparing `engression-0.1.0/engression/models.py` & `engression-0.1.1/engression/models.py`

 * *Files identical despite different names*

### Comparing `engression-0.1.0/engression/utils.py` & `engression-0.1.1/engression/utils.py`

 * *Files identical despite different names*

### Comparing `engression-0.1.0/engression.egg-info/PKG-INFO` & `engression-0.1.1/engression.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: engression
-Version: 0.1.0
+Version: 0.1.1
 Summary: Engression Modelling
 Home-page: https://github.com/xwshen51/engression
 Author: Xinwei Shen and Nicolai Meinshausen
 Author-email: xinwei.shen@stat.math.ethz.ch
 License: BSD 3-Clause License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `engression-0.1.0/setup.py` & `engression-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open('requirements.txt') as f:
     install_requires = [l.strip() for l in f]
     
 
 setup(
     name='engression',
-    version='0.1.0',
+    version='0.1.1',
     description='Engression Modelling',
     url='https://github.com/xwshen51/engression',
     author='Xinwei Shen and Nicolai Meinshausen',
     author_email='xinwei.shen@stat.math.ethz.ch',
     install_requires=install_requires,
     long_description=long_description,
     long_description_content_type="text/markdown",
```

