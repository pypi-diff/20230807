# Comparing `tmp/fastervit-0.9.3.tar.gz` & `tmp/fastervit-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ali/Desktop/Gitlab_repos/FasterViT_pip_test/dist/.tmp-g4tgee92/fastervit-0.9.3.tar", last modified: Thu Jul 20 14:32:02 2023, max compression
+gzip compressed data, was "/home/ali/Desktop/Gitlab_repos/FasterViT_pip_test/dist/.tmp-6ntbhaj0/fastervit-0.9.4.tar", last modified: Mon Aug  7 06:34:46 2023, max compression
```

## Comparing `fastervit-0.9.3.tar` & `fastervit-0.9.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-20 14:32:02.000000 fastervit-0.9.3/
--rw-rw-r--   0 ali       (1000) ali       (1000)     4146 2023-07-07 22:05:20.000000 fastervit-0.9.3/LICENSE
--rw-rw-r--   0 ali       (1000) ali       (1000)       45 2023-07-07 22:05:20.000000 fastervit-0.9.3/MANIFEST.in
--rw-rw-r--   0 ali       (1000) ali       (1000)     8238 2023-07-20 14:32:02.000000 fastervit-0.9.3/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)     7287 2023-07-20 14:31:18.000000 fastervit-0.9.3/README.md
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-20 14:32:02.000000 fastervit-0.9.3/fastervit/
--rw-rw-r--   0 ali       (1000) ali       (1000)       41 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/__init__.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-20 14:32:02.000000 fastervit-0.9.3/fastervit/assets/
--rw-rw-r--   0 ali       (1000) ali       (1000)   100537 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/assets/hierarchial_attn.png
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-20 14:32:02.000000 fastervit-0.9.3/fastervit/models/
--rw-rw-r--   0 ali       (1000) ali       (1000)       96 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/models/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    49072 2023-07-07 22:14:53.000000 fastervit-0.9.3/fastervit/models/faster_vit.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    50830 2023-07-07 22:20:22.000000 fastervit-0.9.3/fastervit/models/faster_vit_any_res.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     7844 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/models/registry.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-20 14:32:02.000000 fastervit-0.9.3/fastervit/scheduler/
--rw-rw-r--   0 ali       (1000) ali       (1000)      291 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/scheduler/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     4161 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/scheduler/cosine_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     2098 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/scheduler/multistep_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3457 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/scheduler/plateau_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     4003 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/scheduler/poly_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     5095 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/scheduler/scheduler.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3907 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/scheduler/scheduler_factory.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1902 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/scheduler/step_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3936 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/scheduler/tanh_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      734 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/tensorboard.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    49422 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/train.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-20 14:32:02.000000 fastervit-0.9.3/fastervit/utils/
--rw-rw-r--   0 ali       (1000) ali       (1000)        0 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/utils/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    19251 2023-07-07 22:05:20.000000 fastervit-0.9.3/fastervit/utils/datasets.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    16159 2023-07-07 22:17:54.000000 fastervit-0.9.3/fastervit/validate.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-07-20 14:32:02.000000 fastervit-0.9.3/fastervit.egg-info/
--rw-rw-r--   0 ali       (1000) ali       (1000)     8238 2023-07-20 14:32:02.000000 fastervit-0.9.3/fastervit.egg-info/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)      824 2023-07-20 14:32:02.000000 fastervit-0.9.3/fastervit.egg-info/SOURCES.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)        1 2023-07-20 14:32:02.000000 fastervit-0.9.3/fastervit.egg-info/dependency_links.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       32 2023-07-20 14:32:02.000000 fastervit-0.9.3/fastervit.egg-info/requires.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       10 2023-07-20 14:32:02.000000 fastervit-0.9.3/fastervit.egg-info/top_level.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)      126 2023-07-20 14:32:02.000000 fastervit-0.9.3/setup.cfg
--rw-rw-r--   0 ali       (1000) ali       (1000)     1549 2023-07-20 14:30:03.000000 fastervit-0.9.3/setup.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-08-07 06:34:46.000000 fastervit-0.9.4/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4146 2023-08-07 06:13:51.000000 fastervit-0.9.4/LICENSE
+-rw-rw-r--   0 ali       (1000) ali       (1000)       45 2023-08-07 06:13:51.000000 fastervit-0.9.4/MANIFEST.in
+-rw-rw-r--   0 ali       (1000) ali       (1000)     8239 2023-08-07 06:34:46.000000 fastervit-0.9.4/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)     7289 2023-08-07 06:34:14.000000 fastervit-0.9.4/README.md
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-08-07 06:34:46.000000 fastervit-0.9.4/fastervit/
+-rw-rw-r--   0 ali       (1000) ali       (1000)       41 2023-08-07 06:13:51.000000 fastervit-0.9.4/fastervit/__init__.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-08-07 06:34:46.000000 fastervit-0.9.4/fastervit/assets/
+-rw-rw-r--   0 ali       (1000) ali       (1000)   100537 2023-08-07 06:13:51.000000 fastervit-0.9.4/fastervit/assets/hierarchial_attn.png
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-08-07 06:34:46.000000 fastervit-0.9.4/fastervit/models/
+-rw-rw-r--   0 ali       (1000) ali       (1000)       96 2023-08-07 06:13:51.000000 fastervit-0.9.4/fastervit/models/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    49072 2023-08-07 06:19:02.000000 fastervit-0.9.4/fastervit/models/faster_vit.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    50831 2023-08-07 06:20:00.000000 fastervit-0.9.4/fastervit/models/faster_vit_any_res.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     7844 2023-08-07 06:13:51.000000 fastervit-0.9.4/fastervit/models/registry.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-08-07 06:34:46.000000 fastervit-0.9.4/fastervit/scheduler/
+-rw-rw-r--   0 ali       (1000) ali       (1000)      291 2023-08-07 06:13:51.000000 fastervit-0.9.4/fastervit/scheduler/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4161 2023-08-07 06:13:51.000000 fastervit-0.9.4/fastervit/scheduler/cosine_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     2098 2023-08-07 06:13:51.000000 fastervit-0.9.4/fastervit/scheduler/multistep_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3457 2023-08-07 06:13:51.000000 fastervit-0.9.4/fastervit/scheduler/plateau_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4003 2023-08-07 06:13:51.000000 fastervit-0.9.4/fastervit/scheduler/poly_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     5095 2023-08-07 06:13:51.000000 fastervit-0.9.4/fastervit/scheduler/scheduler.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3907 2023-08-07 06:13:51.000000 fastervit-0.9.4/fastervit/scheduler/scheduler_factory.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1902 2023-08-07 06:13:51.000000 fastervit-0.9.4/fastervit/scheduler/step_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3936 2023-08-07 06:13:51.000000 fastervit-0.9.4/fastervit/scheduler/tanh_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      734 2023-08-07 06:13:51.000000 fastervit-0.9.4/fastervit/tensorboard.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    49422 2023-08-07 06:13:51.000000 fastervit-0.9.4/fastervit/train.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-08-07 06:34:46.000000 fastervit-0.9.4/fastervit/utils/
+-rw-rw-r--   0 ali       (1000) ali       (1000)        0 2023-08-07 06:13:51.000000 fastervit-0.9.4/fastervit/utils/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    19251 2023-08-07 06:13:51.000000 fastervit-0.9.4/fastervit/utils/datasets.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    16159 2023-08-07 06:13:51.000000 fastervit-0.9.4/fastervit/validate.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-08-07 06:34:46.000000 fastervit-0.9.4/fastervit.egg-info/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     8239 2023-08-07 06:34:46.000000 fastervit-0.9.4/fastervit.egg-info/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)      824 2023-08-07 06:34:46.000000 fastervit-0.9.4/fastervit.egg-info/SOURCES.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)        1 2023-08-07 06:34:46.000000 fastervit-0.9.4/fastervit.egg-info/dependency_links.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       32 2023-08-07 06:34:46.000000 fastervit-0.9.4/fastervit.egg-info/requires.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       10 2023-08-07 06:34:46.000000 fastervit-0.9.4/fastervit.egg-info/top_level.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)      126 2023-08-07 06:34:46.000000 fastervit-0.9.4/setup.cfg
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1549 2023-08-07 06:20:24.000000 fastervit-0.9.4/setup.py
```

### Comparing `fastervit-0.9.3/LICENSE` & `fastervit-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.3/PKG-INFO` & `fastervit-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastervit
-Version: 0.9.3
+Version: 0.9.4
 Summary: FasterViT: Fast Vision Transformers with Hierarchical Attention
 Home-page: https://github.com/NVlabs/FasterViT
 Author: Ali Hatamizadeh
 Author-email: ahatamiz123@gmail.com
 License: NVIDIA Source Code License-NC
 Keywords: pytorch pretrained models efficientnet mobilenetv3 mnasnet resnet vision transformer vit
 Classifier: Programming Language :: Python :: 3.7
@@ -300,7 +300,8 @@
 
 For license information regarding the timm repository, please refer to its [repository](https://github.com/rwightman/pytorch-image-models).
 
 For license information regarding the ImageNet dataset, please see the [ImageNet official website](https://www.image-net.org/). 
 
 ## Acknowledgement
 This repository is built on top of the [timm](https://github.com/huggingface/pytorch-image-models) repository. We thank [Ross Wrightman](https://rwightman.com/) for creating and maintaining this high-quality library.
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastervit Version: 0.9.3 Summary: FasterViT: Fast
+Metadata-Version: 2.1 Name: fastervit Version: 0.9.4 Summary: FasterViT: Fast
 Vision Transformers with Hierarchical Attention Home-page: https://github.com/
 NVlabs/FasterViT Author: Ali Hatamizadeh Author-email: ahatamiz123@gmail.com
 License: NVIDIA Source Code License-NC Keywords: pytorch pretrained models
 efficientnet mobilenetv3 mnasnet resnet vision transformer vit Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `fastervit-0.9.3/README.md` & `fastervit-0.9.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -277,8 +277,9 @@
 This work is made available under the NVIDIA Source Code License-NC. Click [here](LICENSE) to view a copy of this license.
 
 For license information regarding the timm repository, please refer to its [repository](https://github.com/rwightman/pytorch-image-models).
 
 For license information regarding the ImageNet dataset, please see the [ImageNet official website](https://www.image-net.org/). 
 
 ## Acknowledgement
-This repository is built on top of the [timm](https://github.com/huggingface/pytorch-image-models) repository. We thank [Ross Wrightman](https://rwightman.com/) for creating and maintaining this high-quality library.
+This repository is built on top of the [timm](https://github.com/huggingface/pytorch-image-models) repository. We thank [Ross Wrightman](https://rwightman.com/) for creating and maintaining this high-quality library.
+
```

### Comparing `fastervit-0.9.3/fastervit/assets/hierarchial_attn.png` & `fastervit-0.9.4/fastervit/assets/hierarchial_attn.png`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.3/fastervit/models/faster_vit.py` & `fastervit-0.9.4/fastervit/models/faster_vit.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.3/fastervit/models/faster_vit_any_res.py` & `fastervit-0.9.4/fastervit/models/faster_vit_any_res.py`

 * *Files 0% similar despite different names*

```diff
@@ -1067,15 +1067,15 @@
                       window_size=window_size,
                       ct_size=ct_size,
                       dim=dim,
                       in_dim=in_dim,
                       mlp_ratio=mlp_ratio,
                       resolution=resolution,
                       drop_path_rate=drop_path_rate,
-                      hat=hat
+                      hat=hat,
                       **kwargs)
     model.default_cfg = default_cfgs['faster_vit_2_any_res']
     if pretrained:
         if not Path(model_path).is_file():
             url = model.default_cfg['url']
             torch.hub.download_url_to_file(url=url, dst=model_path)
         model._load_state_dict(model_path)
```

### Comparing `fastervit-0.9.3/fastervit/models/registry.py` & `fastervit-0.9.4/fastervit/models/registry.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.3/fastervit/scheduler/cosine_lr.py` & `fastervit-0.9.4/fastervit/scheduler/cosine_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.3/fastervit/scheduler/multistep_lr.py` & `fastervit-0.9.4/fastervit/scheduler/multistep_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.3/fastervit/scheduler/plateau_lr.py` & `fastervit-0.9.4/fastervit/scheduler/plateau_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.3/fastervit/scheduler/poly_lr.py` & `fastervit-0.9.4/fastervit/scheduler/poly_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.3/fastervit/scheduler/scheduler.py` & `fastervit-0.9.4/fastervit/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.3/fastervit/scheduler/scheduler_factory.py` & `fastervit-0.9.4/fastervit/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.3/fastervit/scheduler/step_lr.py` & `fastervit-0.9.4/fastervit/scheduler/step_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.3/fastervit/scheduler/tanh_lr.py` & `fastervit-0.9.4/fastervit/scheduler/tanh_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.3/fastervit/tensorboard.py` & `fastervit-0.9.4/fastervit/tensorboard.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.3/fastervit/train.py` & `fastervit-0.9.4/fastervit/train.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.3/fastervit/utils/datasets.py` & `fastervit-0.9.4/fastervit/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.3/fastervit/validate.py` & `fastervit-0.9.4/fastervit/validate.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.3/fastervit.egg-info/PKG-INFO` & `fastervit-0.9.4/fastervit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastervit
-Version: 0.9.3
+Version: 0.9.4
 Summary: FasterViT: Fast Vision Transformers with Hierarchical Attention
 Home-page: https://github.com/NVlabs/FasterViT
 Author: Ali Hatamizadeh
 Author-email: ahatamiz123@gmail.com
 License: NVIDIA Source Code License-NC
 Keywords: pytorch pretrained models efficientnet mobilenetv3 mnasnet resnet vision transformer vit
 Classifier: Programming Language :: Python :: 3.7
@@ -300,7 +300,8 @@
 
 For license information regarding the timm repository, please refer to its [repository](https://github.com/rwightman/pytorch-image-models).
 
 For license information regarding the ImageNet dataset, please see the [ImageNet official website](https://www.image-net.org/). 
 
 ## Acknowledgement
 This repository is built on top of the [timm](https://github.com/huggingface/pytorch-image-models) repository. We thank [Ross Wrightman](https://rwightman.com/) for creating and maintaining this high-quality library.
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastervit Version: 0.9.3 Summary: FasterViT: Fast
+Metadata-Version: 2.1 Name: fastervit Version: 0.9.4 Summary: FasterViT: Fast
 Vision Transformers with Hierarchical Attention Home-page: https://github.com/
 NVlabs/FasterViT Author: Ali Hatamizadeh Author-email: ahatamiz123@gmail.com
 License: NVIDIA Source Code License-NC Keywords: pytorch pretrained models
 efficientnet mobilenetv3 mnasnet resnet vision transformer vit Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `fastervit-0.9.3/fastervit.egg-info/SOURCES.txt` & `fastervit-0.9.4/fastervit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastervit-0.9.3/setup.py` & `fastervit-0.9.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='fastervit',
-    version='0.9.3',
+    version='0.9.4',
     description='FasterViT: Fast Vision Transformers with Hierarchical Attention',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/NVlabs/FasterViT',
     author='Ali Hatamizadeh',
     author_email='ahatamiz123@gmail.com',
     classifiers=[
```

