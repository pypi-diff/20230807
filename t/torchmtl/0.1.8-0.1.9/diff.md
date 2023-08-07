# Comparing `tmp/torchmtl-0.1.8.tar.gz` & `tmp/torchmtl-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmtl-0.1.8.tar", last modified: Sun Nov 15 15:03:16 2020, max compression
+gzip compressed data, was "torchmtl-0.1.9.tar", max compression
```

## Comparing `torchmtl-0.1.8.tar` & `torchmtl-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rwxr-xr-x   0        0        0     1071 2020-10-20 12:37:09.000000 torchmtl-0.1.8/LICENSE
--rw-r--r--   0        0        0     6140 2020-11-07 11:50:39.475081 torchmtl-0.1.8/README.md
--rwxr-xr-x   0        0        0      523 2020-11-15 15:02:33.430654 torchmtl-0.1.8/pyproject.toml
--rwxr-xr-x   0        0        0      144 2020-11-15 15:02:18.131826 torchmtl-0.1.8/torchmtl/__init__.py
--rwxr-xr-x   0        0        0     6612 2020-11-15 14:58:51.021622 torchmtl-0.1.8/torchmtl/model_builder.py
--rw-r--r--   0        0        0     1050 2020-11-15 12:43:33.391060 torchmtl-0.1.8/torchmtl/wrapping_layers.py
--rw-r--r--   0        0        0     7075 2020-11-15 15:03:17.042272 torchmtl-0.1.8/setup.py
--rw-r--r--   0        0        0     6760 2020-11-15 15:03:17.042699 torchmtl-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-06 23:02:26.228741 torchmtl-0.1.9/LICENSE
+-rw-r--r--   0        0        0     6482 2023-08-06 23:02:26.228870 torchmtl-0.1.9/README.md
+-rw-r--r--   0        0        0      524 2023-08-07 03:30:24.257264 torchmtl-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      144 2023-08-06 23:02:26.230584 torchmtl-0.1.9/torchmtl/__init__.py
+-rw-r--r--   0        0        0     6612 2023-08-06 23:02:26.230692 torchmtl-0.1.9/torchmtl/model_builder.py
+-rw-r--r--   0        0        0     1050 2023-08-06 23:02:26.230774 torchmtl-0.1.9/torchmtl/wrapping_layers.py
+-rw-r--r--   0        0        0     7247 1970-01-01 00:00:00.000000 torchmtl-0.1.9/PKG-INFO
```

### Comparing `torchmtl-0.1.8/LICENSE` & `torchmtl-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `torchmtl-0.1.8/README.md` & `torchmtl-0.1.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 ![torchMTL Logo](https://github.com/chrisby/torchMTL/blob/main/images/torchmtl_logo.png "torchMTL Logo")    
 A lightweight module for Multi-Task Learning in pytorch.
 
 `torchmtl` tries to help you composing modular multi-task architectures with minimal effort. All you need is a list of dictionaries in which you define your layers and how they build on each other. From this, `torchmtl` constructs a meta-computation graph which is executed in each forward pass of the created `MTLModel`. To combine outputs from multiple layers, simple [wrapper functions](https://github.com/chrisby/torchMTL/blob/main/torchmtl/wrapping_layers.py) are provided.
 
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4362515.svg)](https://doi.org/10.5281/zenodo.4362515)
+
+
 ### Installation
 `torchmtl` can be installed via `pip`:
 ```
 pip install torchmtl
 ```
 
 ### Quickstart (or find examples [here](https://github.com/chrisby/torchMTL/tree/main/examples))
@@ -122,8 +125,19 @@
 { ...,
   'layers' = SimpleSelect(selection_axis=0),
   ...
 }
 ```
 It should be trivial to write your own wrapping layers, but I try to provide useful ones with this library. If you have any layers in mind but no time to implement them, feel free to [open an issue](https://github.com/chrisby/torchMTL/issues).
 
+#### Cite
+```
+@misc{torchMTL: A lightweight module for Multi-Task Learning in pytorch,
+  author = {Bock, Christian},
+  doi = {10.5281/zenodo.4362515},
+  url = {https://github.com/chrisby/torchMTL},
+  year = {2020}
+}
+```
+
+#### Credits
 Logo credits and license: I reused and remixed (moved the dot and rotated the resulting logo a couple times) the pytorch logo from [here](https://github.com/pytorch/pytorch/blob/master/docs/source/_static/img/pytorch-logo-dark.png) (accessed through [wikimedia commons](https://commons.wikimedia.org/wiki/File:Pytorch_logo.png)) which can be used under the [Attribution-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-sa/4.0/deed.en) license. Hence, this logo falls under the same license.
```

### Comparing `torchmtl-0.1.8/pyproject.toml` & `torchmtl-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "torchmtl"
-version = "0.1.8"
+version = "0.1.9"
 description = "A lightweight module for Multi-Task Learning in pytorch"
 authors = ["Christian Bock <christian.bock@bsse.ethz.ch>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-torch = "^1.6.0"
+torch = ">=1.6.0"
 networkx = "^2.5"
 matplotlib = "^3.3.2"
 scipy = "^1.5.3"
 
 [tool.poetry.dev-dependencies]
 jupyter = "^1.0.0"
 notebook = "^6.1.4"
```

### Comparing `torchmtl-0.1.8/torchmtl/model_builder.py` & `torchmtl-0.1.9/torchmtl/model_builder.py`

 * *Files identical despite different names*

### Comparing `torchmtl-0.1.8/torchmtl/wrapping_layers.py` & `torchmtl-0.1.9/torchmtl/wrapping_layers.py`

 * *Files identical despite different names*

### Comparing `torchmtl-0.1.8/setup.py` & `torchmtl-0.1.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,165 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['torchmtl']
-
-package_data = \
-{'': ['*']}
+Metadata-Version: 2.1
+Name: torchmtl
+Version: 0.1.9
+Summary: A lightweight module for Multi-Task Learning in pytorch
+License: MIT
+Author: Christian Bock
+Author-email: christian.bock@bsse.ethz.ch
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: matplotlib (>=3.3.2,<4.0.0)
+Requires-Dist: networkx (>=2.5,<3.0)
+Requires-Dist: scipy (>=1.5.3,<2.0.0)
+Requires-Dist: torch (>=1.6.0)
+Description-Content-Type: text/markdown
+
+![torchMTL Logo](https://github.com/chrisby/torchMTL/blob/main/images/torchmtl_logo.png "torchMTL Logo")    
+A lightweight module for Multi-Task Learning in pytorch.
+
+`torchmtl` tries to help you composing modular multi-task architectures with minimal effort. All you need is a list of dictionaries in which you define your layers and how they build on each other. From this, `torchmtl` constructs a meta-computation graph which is executed in each forward pass of the created `MTLModel`. To combine outputs from multiple layers, simple [wrapper functions](https://github.com/chrisby/torchMTL/blob/main/torchmtl/wrapping_layers.py) are provided.
+
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4362515.svg)](https://doi.org/10.5281/zenodo.4362515)
+
+
+### Installation
+`torchmtl` can be installed via `pip`:
+```
+pip install torchmtl
+```
+
+### Quickstart (or find examples [here](https://github.com/chrisby/torchMTL/tree/main/examples))
+Assume you want to train a network on three tasks as shown below.  
+![example](https://github.com/chrisby/torchMTL/blob/main/images/example.png "example")  
+
+To construct such an architecture with `torchmtl`, you simply have to define the following list
+
+```python
+tasks = [
+        {
+            'name': "Embed1",
+            'layers': Sequential(*[Linear(16, 32), Linear(32, 8)]),
+            # No anchor_layer means this layer receives input directly
+        },    
+        {
+            'name': "Embed2",
+            'layers': Sequential(*[Linear(16, 32), Linear(32, 8)]),
+            # No anchor_layer means this layer receives input directly
+        },
+        {
+            'name': "CatTask",
+            'layers': Concat(dim=1),
+            'loss_weight': 1.0,
+            'anchor_layer': ['Embed1', 'Embed2']
+        },
+        {
+            'name': "Task1",
+            'layers': Sequential(*[Linear(8, 32), Linear(32, 1)]),
+            'loss': MSELoss(),
+            'loss_weight': 1.0,
+            'anchor_layer': 'Embed1'            
+        },
+        {
+            'name': "Task2",
+            'layers': Sequential(*[Linear(8, 64), Linear(64, 1)]),
+            'loss': BCEWithLogitsLoss(),
+            'loss_weight': 1.0,
+            'anchor_layer': 'Embed2'            
+        }, 
+        {
+            'name': "FNN",
+            'layers': Sequential(*[Linear(16, 32), Linear(32, 32)]),
+            'anchor_layer': 'CatTask'
+        },
+        {
+            'name': "Task3",
+            'layers': Sequential(*[Linear(32, 16), Linear(16, 1)]),
+            'anchor_layer': 'FNN',
+            'loss': MSELoss(),
+            'loss_weight': 'auto',
+            'loss_init_val': 1.0
+        }
+    ]
+```
+
+You can build your final model with the following lines in which you specify from which layers you would like to receive the output.
+```python
+from torchmtl import MTLModel
+model = MTLModel(tasks, output_tasks=['Task1', 'Task2', 'Task3'])
+```
+
+This constructs a **meta-computation graph** which is executed in each forward pass of your `model`. You can verify whether the graph was properly built by plotting it using the `networkx` library:
+```python
+import networkx as nx
+pos = nx.planar_layout(model.g)
+nx.draw(model.g, pos, font_size=14, node_color="y", node_size=450, with_labels=True)
+```
+![graph example](https://github.com/chrisby/torchMTL/blob/main/images/torchmtl_graph.png "graph example")  
+
+#### The training loop
+You can now enter the typical `pytorch` training loop and you will have access to everything you need to update your model:
+```python
+for X, y in data_loader:
+    optimizer.zero_grad()
+
+    # Our model will return a list of predictions (from the layers specified in `output_tasks`),
+    # loss functions, and regularization parameters (as defined in the tasks variable)
+    y_hat, l_funcs, l_weights = model(X)
+    
+    loss = 0
+    # We can now iterate over the tasks and accumulate the losses
+    for i in range(len(y_hat)):
+        loss += l_weights[i] * l_funcs[i](y_hat[i], y[i])
+    
+    loss.backward()
+    optimizer.step()
+
+```
+
+### Details on the layer definition
+There are 6 keys that can be specified (`name` and `layers` **must** always be present):  
+
+**`layers`**  
+Basically takes any `nn.Module` that you can think of. You can plug in a transformer or just a handful of fully connected layers.  
+
+**`anchor_layer`**  
+This defines from which other layer this layer receives its input. Take care that the respective dimensions match.  
+
+**`loss`**  
+The loss function you want to compute on the output of this layer (`l_funcs`). Can be set to `None` or omitted altogether when only access to the layer's output is needed.   
+
+**`loss_weight`**  
+The scalar with which you want to regularize the respective loss (`l_weights`). If set to `'auto'`, a `nn.Parameter` is returned which will be updated through backpropagation. Can be set to `None` or omitted altogether when only access to the layer's output is needed.  
+
+**`loss_init_val`**  
+Only needed if `loss_weight: 'auto'`. The initialization value of the `loss_weight` parameter.
+
+### Wrapping functions
+Nodes of the **meta-computation graph** don't have to be pytorch Modules. They can be *concatenation* functions or indexing functions that return a certain element of the input. If your `X` consists of two types of input data `X=[X_1, X_2]`, you can use the `SimpleSelect` layer to select the `X_1` by setting  
+```python
+from torchmtl.wrapping_layers import SimpleSelect
+{ ...,
+  'layers' = SimpleSelect(selection_axis=0),
+  ...
+}
+```
+It should be trivial to write your own wrapping layers, but I try to provide useful ones with this library. If you have any layers in mind but no time to implement them, feel free to [open an issue](https://github.com/chrisby/torchMTL/issues).
 
-install_requires = \
-['matplotlib>=3.3.2,<4.0.0',
- 'networkx>=2.5,<3.0',
- 'scipy>=1.5.3,<2.0.0',
- 'torch>=1.6.0,<2.0.0']
-
-setup_kwargs = {
-    'name': 'torchmtl',
-    'version': '0.1.8',
-    'description': 'A lightweight module for Multi-Task Learning in pytorch',
-    'long_description': '![torchMTL Logo](https://github.com/chrisby/torchMTL/blob/main/images/torchmtl_logo.png "torchMTL Logo")    \nA lightweight module for Multi-Task Learning in pytorch.\n\n`torchmtl` tries to help you composing modular multi-task architectures with minimal effort. All you need is a list of dictionaries in which you define your layers and how they build on each other. From this, `torchmtl` constructs a meta-computation graph which is executed in each forward pass of the created `MTLModel`. To combine outputs from multiple layers, simple [wrapper functions](https://github.com/chrisby/torchMTL/blob/main/torchmtl/wrapping_layers.py) are provided.\n\n### Installation\n`torchmtl` can be installed via `pip`:\n```\npip install torchmtl\n```\n\n### Quickstart (or find examples [here](https://github.com/chrisby/torchMTL/tree/main/examples))\nAssume you want to train a network on three tasks as shown below.  \n![example](https://github.com/chrisby/torchMTL/blob/main/images/example.png "example")  \n\nTo construct such an architecture with `torchmtl`, you simply have to define the following list\n\n```python\ntasks = [\n        {\n            \'name\': "Embed1",\n            \'layers\': Sequential(*[Linear(16, 32), Linear(32, 8)]),\n            # No anchor_layer means this layer receives input directly\n        },    \n        {\n            \'name\': "Embed2",\n            \'layers\': Sequential(*[Linear(16, 32), Linear(32, 8)]),\n            # No anchor_layer means this layer receives input directly\n        },\n        {\n            \'name\': "CatTask",\n            \'layers\': Concat(dim=1),\n            \'loss_weight\': 1.0,\n            \'anchor_layer\': [\'Embed1\', \'Embed2\']\n        },\n        {\n            \'name\': "Task1",\n            \'layers\': Sequential(*[Linear(8, 32), Linear(32, 1)]),\n            \'loss\': MSELoss(),\n            \'loss_weight\': 1.0,\n            \'anchor_layer\': \'Embed1\'            \n        },\n        {\n            \'name\': "Task2",\n            \'layers\': Sequential(*[Linear(8, 64), Linear(64, 1)]),\n            \'loss\': BCEWithLogitsLoss(),\n            \'loss_weight\': 1.0,\n            \'anchor_layer\': \'Embed2\'            \n        }, \n        {\n            \'name\': "FNN",\n            \'layers\': Sequential(*[Linear(16, 32), Linear(32, 32)]),\n            \'anchor_layer\': \'CatTask\'\n        },\n        {\n            \'name\': "Task3",\n            \'layers\': Sequential(*[Linear(32, 16), Linear(16, 1)]),\n            \'anchor_layer\': \'FNN\',\n            \'loss\': MSELoss(),\n            \'loss_weight\': \'auto\',\n            \'loss_init_val\': 1.0\n        }\n    ]\n```\n\nYou can build your final model with the following lines in which you specify from which layers you would like to receive the output.\n```python\nfrom torchmtl import MTLModel\nmodel = MTLModel(tasks, output_tasks=[\'Task1\', \'Task2\', \'Task3\'])\n```\n\nThis constructs a **meta-computation graph** which is executed in each forward pass of your `model`. You can verify whether the graph was properly built by plotting it using the `networkx` library:\n```python\nimport networkx as nx\npos = nx.planar_layout(model.g)\nnx.draw(model.g, pos, font_size=14, node_color="y", node_size=450, with_labels=True)\n```\n![graph example](https://github.com/chrisby/torchMTL/blob/main/images/torchmtl_graph.png "graph example")  \n\n#### The training loop\nYou can now enter the typical `pytorch` training loop and you will have access to everything you need to update your model:\n```python\nfor X, y in data_loader:\n    optimizer.zero_grad()\n\n    # Our model will return a list of predictions (from the layers specified in `output_tasks`),\n    # loss functions, and regularization parameters (as defined in the tasks variable)\n    y_hat, l_funcs, l_weights = model(X)\n    \n    loss = 0\n    # We can now iterate over the tasks and accumulate the losses\n    for i in range(len(y_hat)):\n        loss += l_weights[i] * l_funcs[i](y_hat[i], y[i])\n    \n    loss.backward()\n    optimizer.step()\n\n```\n\n### Details on the layer definition\nThere are 6 keys that can be specified (`name` and `layers` **must** always be present):  \n\n**`layers`**  \nBasically takes any `nn.Module` that you can think of. You can plug in a transformer or just a handful of fully connected layers.  \n\n**`anchor_layer`**  \nThis defines from which other layer this layer receives its input. Take care that the respective dimensions match.  \n\n**`loss`**  \nThe loss function you want to compute on the output of this layer (`l_funcs`). Can be set to `None` or omitted altogether when only access to the layer\'s output is needed.   \n\n**`loss_weight`**  \nThe scalar with which you want to regularize the respective loss (`l_weights`). If set to `\'auto\'`, a `nn.Parameter` is returned which will be updated through backpropagation. Can be set to `None` or omitted altogether when only access to the layer\'s output is needed.  \n\n**`loss_init_val`**  \nOnly needed if `loss_weight: \'auto\'`. The initialization value of the `loss_weight` parameter.\n\n### Wrapping functions\nNodes of the **meta-computation graph** don\'t have to be pytorch Modules. They can be *concatenation* functions or indexing functions that return a certain element of the input. If your `X` consists of two types of input data `X=[X_1, X_2]`, you can use the `SimpleSelect` layer to select the `X_1` by setting  \n```python\nfrom torchmtl.wrapping_layers import SimpleSelect\n{ ...,\n  \'layers\' = SimpleSelect(selection_axis=0),\n  ...\n}\n```\nIt should be trivial to write your own wrapping layers, but I try to provide useful ones with this library. If you have any layers in mind but no time to implement them, feel free to [open an issue](https://github.com/chrisby/torchMTL/issues).\n\nLogo credits and license: I reused and remixed (moved the dot and rotated the resulting logo a couple times) the pytorch logo from [here](https://github.com/pytorch/pytorch/blob/master/docs/source/_static/img/pytorch-logo-dark.png) (accessed through [wikimedia commons](https://commons.wikimedia.org/wiki/File:Pytorch_logo.png)) which can be used under the [Attribution-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-sa/4.0/deed.en) license. Hence, this logo falls under the same license. \n',
-    'author': 'Christian Bock',
-    'author_email': 'christian.bock@bsse.ethz.ch',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+#### Cite
+```
+@misc{torchMTL: A lightweight module for Multi-Task Learning in pytorch,
+  author = {Bock, Christian},
+  doi = {10.5281/zenodo.4362515},
+  url = {https://github.com/chrisby/torchMTL},
+  year = {2020}
 }
+```
 
+#### Credits
+Logo credits and license: I reused and remixed (moved the dot and rotated the resulting logo a couple times) the pytorch logo from [here](https://github.com/pytorch/pytorch/blob/master/docs/source/_static/img/pytorch-logo-dark.png) (accessed through [wikimedia commons](https://commons.wikimedia.org/wiki/File:Pytorch_logo.png)) which can be used under the [Attribution-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-sa/4.0/deed.en) license. Hence, this logo falls under the same license. 
 
-setup(**setup_kwargs)
```

