# Comparing `tmp/PrivateModelArchitectures-0.1.tar.gz` & `tmp/PrivateModelArchitectures-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrivateModelArchitectures-0.1.tar", last modified: Wed Jul 26 07:28:00 2023, max compression
+gzip compressed data, was "PrivateModelArchitectures-0.1.1.tar", last modified: Mon Aug  7 08:52:40 2023, max compression
```

## Comparing `PrivateModelArchitectures-0.1.tar` & `PrivateModelArchitectures-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 zillera   (1004) zillera   (1004)        0 2023-07-26 07:28:00.281563 PrivateModelArchitectures-0.1/
--rw-rw-r--   0 zillera   (1004) zillera   (1004)      297 2023-07-26 07:28:00.281563 PrivateModelArchitectures-0.1/PKG-INFO
-drwxrwxr-x   0 zillera   (1004) zillera   (1004)        0 2023-07-26 07:28:00.281563 PrivateModelArchitectures-0.1/PrivateModelArchitectures/
--rw-rw-r--   0 zillera   (1004) zillera   (1004)      271 2023-07-26 07:17:04.000000 PrivateModelArchitectures-0.1/PrivateModelArchitectures/__init__.py
-drwxrwxr-x   0 zillera   (1004) zillera   (1004)        0 2023-07-26 07:28:00.281563 PrivateModelArchitectures-0.1/PrivateModelArchitectures/classification/
--rw-rw-r--   0 zillera   (1004) zillera   (1004)     4597 2023-07-26 06:30:17.000000 PrivateModelArchitectures-0.1/PrivateModelArchitectures/classification/ResNet.py
--rw-rw-r--   0 zillera   (1004) zillera   (1004)    12471 2023-07-26 06:30:17.000000 PrivateModelArchitectures-0.1/PrivateModelArchitectures/classification/SmoothNet.py
--rw-rw-r--   0 zillera   (1004) zillera   (1004)      141 2023-07-26 07:17:16.000000 PrivateModelArchitectures-0.1/PrivateModelArchitectures/classification/__init__.py
-drwxrwxr-x   0 zillera   (1004) zillera   (1004)        0 2023-07-26 07:28:00.281563 PrivateModelArchitectures-0.1/PrivateModelArchitectures/segmentation/
--rw-rw-r--   0 zillera   (1004) zillera   (1004)     7767 2023-07-26 06:30:17.000000 PrivateModelArchitectures-0.1/PrivateModelArchitectures/segmentation/LinkNet.py
--rw-rw-r--   0 zillera   (1004) zillera   (1004)     7838 2023-07-26 06:30:17.000000 PrivateModelArchitectures-0.1/PrivateModelArchitectures/segmentation/UNet.py
--rw-rw-r--   0 zillera   (1004) zillera   (1004)      130 2023-07-26 07:17:14.000000 PrivateModelArchitectures-0.1/PrivateModelArchitectures/segmentation/__init__.py
-drwxrwxr-x   0 zillera   (1004) zillera   (1004)        0 2023-07-26 07:28:00.281563 PrivateModelArchitectures-0.1/PrivateModelArchitectures.egg-info/
--rw-rw-r--   0 zillera   (1004) zillera   (1004)      297 2023-07-26 07:28:00.000000 PrivateModelArchitectures-0.1/PrivateModelArchitectures.egg-info/PKG-INFO
--rw-rw-r--   0 zillera   (1004) zillera   (1004)      558 2023-07-26 07:28:00.000000 PrivateModelArchitectures-0.1/PrivateModelArchitectures.egg-info/SOURCES.txt
--rw-rw-r--   0 zillera   (1004) zillera   (1004)        1 2023-07-26 07:28:00.000000 PrivateModelArchitectures-0.1/PrivateModelArchitectures.egg-info/dependency_links.txt
--rw-rw-r--   0 zillera   (1004) zillera   (1004)       26 2023-07-26 07:28:00.000000 PrivateModelArchitectures-0.1/PrivateModelArchitectures.egg-info/top_level.txt
--rw-rw-r--   0 zillera   (1004) zillera   (1004)      178 2023-07-26 06:30:17.000000 PrivateModelArchitectures-0.1/README.md
--rw-rw-r--   0 zillera   (1004) zillera   (1004)       38 2023-07-26 07:28:00.281563 PrivateModelArchitectures-0.1/setup.cfg
--rw-rw-r--   0 zillera   (1004) zillera   (1004)      509 2023-07-26 07:26:44.000000 PrivateModelArchitectures-0.1/setup.py
+drwxr-xr-x   0 zillera   (6422) tumuser  (20909)        0 2023-08-07 08:52:40.338865 PrivateModelArchitectures-0.1.1/
+-rw-r--r--   0 zillera   (6422) tumuser  (20909)      299 2023-08-07 08:52:40.334865 PrivateModelArchitectures-0.1.1/PKG-INFO
+drwxr-xr-x   0 zillera   (6422) tumuser  (20909)        0 2023-08-07 08:52:40.270865 PrivateModelArchitectures-0.1.1/PrivateModelArchitectures/
+-rw-r--r--   0 zillera   (6422) tumuser  (20909)      271 2023-08-03 09:55:42.000000 PrivateModelArchitectures-0.1.1/PrivateModelArchitectures/__init__.py
+drwxr-xr-x   0 zillera   (6422) tumuser  (20909)        0 2023-08-07 08:52:40.306865 PrivateModelArchitectures-0.1.1/PrivateModelArchitectures/classification/
+-rw-r--r--   0 zillera   (6422) tumuser  (20909)     5266 2023-08-07 08:40:29.000000 PrivateModelArchitectures-0.1.1/PrivateModelArchitectures/classification/ResNet.py
+-rw-r--r--   0 zillera   (6422) tumuser  (20909)    12471 2023-08-03 09:55:42.000000 PrivateModelArchitectures-0.1.1/PrivateModelArchitectures/classification/SmoothNet.py
+-rw-r--r--   0 zillera   (6422) tumuser  (20909)      141 2023-08-03 09:55:42.000000 PrivateModelArchitectures-0.1.1/PrivateModelArchitectures/classification/__init__.py
+drwxr-xr-x   0 zillera   (6422) tumuser  (20909)        0 2023-08-07 08:52:40.330865 PrivateModelArchitectures-0.1.1/PrivateModelArchitectures/segmentation/
+-rw-r--r--   0 zillera   (6422) tumuser  (20909)     7767 2023-08-03 09:55:42.000000 PrivateModelArchitectures-0.1.1/PrivateModelArchitectures/segmentation/LinkNet.py
+-rw-r--r--   0 zillera   (6422) tumuser  (20909)     7838 2023-08-03 09:55:42.000000 PrivateModelArchitectures-0.1.1/PrivateModelArchitectures/segmentation/UNet.py
+-rw-r--r--   0 zillera   (6422) tumuser  (20909)      130 2023-08-03 09:55:42.000000 PrivateModelArchitectures-0.1.1/PrivateModelArchitectures/segmentation/__init__.py
+drwxr-xr-x   0 zillera   (6422) tumuser  (20909)        0 2023-08-07 08:52:40.290865 PrivateModelArchitectures-0.1.1/PrivateModelArchitectures.egg-info/
+-rw-r--r--   0 zillera   (6422) tumuser  (20909)      299 2023-08-07 08:52:40.000000 PrivateModelArchitectures-0.1.1/PrivateModelArchitectures.egg-info/PKG-INFO
+-rw-r--r--   0 zillera   (6422) tumuser  (20909)      558 2023-08-07 08:52:40.000000 PrivateModelArchitectures-0.1.1/PrivateModelArchitectures.egg-info/SOURCES.txt
+-rw-r--r--   0 zillera   (6422) tumuser  (20909)        1 2023-08-07 08:52:40.000000 PrivateModelArchitectures-0.1.1/PrivateModelArchitectures.egg-info/dependency_links.txt
+-rw-r--r--   0 zillera   (6422) tumuser  (20909)       26 2023-08-07 08:52:40.000000 PrivateModelArchitectures-0.1.1/PrivateModelArchitectures.egg-info/top_level.txt
+-rw-r--r--   0 zillera   (6422) tumuser  (20909)      178 2023-08-03 09:55:42.000000 PrivateModelArchitectures-0.1.1/README.md
+-rw-r--r--   0 zillera   (6422) tumuser  (20909)       38 2023-08-07 08:52:40.338865 PrivateModelArchitectures-0.1.1/setup.cfg
+-rw-r--r--   0 zillera   (6422) tumuser  (20909)      511 2023-08-07 08:42:17.000000 PrivateModelArchitectures-0.1.1/setup.py
```

### Comparing `PrivateModelArchitectures-0.1/PrivateModelArchitectures/classification/ResNet.py` & `PrivateModelArchitectures-0.1.1/PrivateModelArchitectures/classification/ResNet.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from torch import nn
 import warnings
-
+from typing import Union
+from pathlib import Path
+from torch import nn, load
+from torchvision.datasets.utils import download_url
 
 def conv_bn_act(
     in_channels, out_channels, pool=False, act_func=nn.Mish, num_groups=None
 ):
     if num_groups is not None:
         warnings.warn("num_groups has no effect with BatchNorm")
     layers = [
@@ -14,16 +16,15 @@
     ]
     if pool:
         layers.append(nn.MaxPool2d(2))
     return nn.Sequential(*layers)
 
 
 def conv_gn_act(in_channels, out_channels, pool=False, act_func=nn.Mish, num_groups=32):
-    """Conv-GroupNorm-Activation
-    """
+    """Conv-GroupNorm-Activation"""
     layers = [
         nn.Conv2d(in_channels, out_channels, kernel_size=3, padding=1, bias=False),
         nn.GroupNorm(min(num_groups, out_channels), out_channels),
         act_func(),
     ]
     if pool:
         layers.append(nn.MaxPool2d(2))
@@ -32,17 +33,19 @@
 
 class ResNet9(nn.Module):
     def __init__(
         self,
         in_channels: int = 3,
         num_classes: int = 10,
         act_func: nn.Module = nn.Mish,
-        scale_norm: bool = False,
+        scale_norm: bool = True,
         norm_layer: str = "batch",
         num_groups: tuple[int, ...] = (32, 32, 32, 32),
+        use_pretrained_weights: bool = False,
+        root: Union[str, Path] = './'
     ):
         """9-layer Residual Network. Architecture:
         conv-conv-Residual(conv, conv)-conv-conv-Residual(conv-conv)-FC
         Args:
             in_channels (int, optional): Channels in the input image. Defaults to 3.
             num_classes (int, optional): Number of classes. Defaults to 10.
             act_func (nn.Module, optional): Activation function to use. Defaults to nn.Mish.
@@ -109,14 +112,26 @@
                 if norm_layer == "batch"
                 else nn.GroupNorm(min(groups[3], 256), 256)
             )  # type:ignore
         else:
             self.scale_norm_1 = nn.Identity()  # type:ignore
             self.scale_norm_2 = nn.Identity()  # type:ignore
 
+
+        if use_pretrained_weights:
+            assert in_channels == 3
+            assert num_classes == 165
+            assert scale_norm
+            assert norm_layer == 'group'
+            root = Path(root)
+            dl_path = 'https://syncandshare.lrz.de/dl/fi6PJUT8XcF2h51qH7kwgB/resnet9_radimagenet.pt'
+            download_url(dl_path, root=root)
+            state_dict = load(root / dl_path.split('/')[-1], map_location='cpu')
+            self.load_state_dict(state_dict)
+
     def forward(self, xb):
         out = self.conv1(xb)
         out = self.conv2(out)
         out = self.res1(out) + out
         out = self.scale_norm_1(out)
         out = self.conv3(out)
         out = self.conv4(out)
```

### Comparing `PrivateModelArchitectures-0.1/PrivateModelArchitectures/classification/SmoothNet.py` & `PrivateModelArchitectures-0.1.1/PrivateModelArchitectures/classification/SmoothNet.py`

 * *Files identical despite different names*

### Comparing `PrivateModelArchitectures-0.1/PrivateModelArchitectures/segmentation/LinkNet.py` & `PrivateModelArchitectures-0.1.1/PrivateModelArchitectures/segmentation/LinkNet.py`

 * *Files identical despite different names*

### Comparing `PrivateModelArchitectures-0.1/PrivateModelArchitectures/segmentation/UNet.py` & `PrivateModelArchitectures-0.1.1/PrivateModelArchitectures/segmentation/UNet.py`

 * *Files identical despite different names*

### Comparing `PrivateModelArchitectures-0.1/PrivateModelArchitectures.egg-info/SOURCES.txt` & `PrivateModelArchitectures-0.1.1/PrivateModelArchitectures.egg-info/SOURCES.txt`

 * *Files identical despite different names*

