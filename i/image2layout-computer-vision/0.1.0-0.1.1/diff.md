# Comparing `tmp/image2layout_computer_vision-0.1.0.tar.gz` & `tmp/image2layout_computer_vision-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image2layout_computer_vision-0.1.0.tar", last modified: Fri Aug  4 09:13:32 2023, max compression
+gzip compressed data, was "image2layout_computer_vision-0.1.1.tar", last modified: Mon Aug  7 06:12:59 2023, max compression
```

## Comparing `image2layout_computer_vision-0.1.0.tar` & `image2layout_computer_vision-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-04 09:13:32.237408 image2layout_computer_vision-0.1.0/
--rw-rw-r--   0 test      (1001) test      (1001)     1073 2023-07-20 04:03:09.000000 image2layout_computer_vision-0.1.0/LICENSE
--rw-rw-r--   0 test      (1001) test      (1001)     2845 2023-08-04 09:13:32.237408 image2layout_computer_vision-0.1.0/PKG-INFO
--rw-rw-r--   0 test      (1001) test      (1001)     2275 2023-08-04 09:12:59.000000 image2layout_computer_vision-0.1.0/README.md
--rw-rw-r--   0 test      (1001) test      (1001)      637 2023-08-04 08:35:55.000000 image2layout_computer_vision-0.1.0/pyproject.toml
--rw-rw-r--   0 test      (1001) test      (1001)       38 2023-08-04 09:13:32.237408 image2layout_computer_vision-0.1.0/setup.cfg
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-04 09:13:32.233408 image2layout_computer_vision-0.1.0/src/
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-04 09:13:32.233408 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/
--rw-rw-r--   0 test      (1001) test      (1001)      613 2023-08-04 08:58:07.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/__init__.py
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-04 09:13:32.237408 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/color_extract/
--rw-rw-r--   0 test      (1001) test      (1001)       95 2023-08-01 04:32:01.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/color_extract/__init__.py
--rw-rw-r--   0 test      (1001) test      (1001)    14464 2023-08-03 04:42:22.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/color_extract/main.py
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-04 09:13:32.237408 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/ocr/
--rw-rw-r--   0 test      (1001) test      (1001)      251 2023-08-04 08:48:54.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/ocr/__init__.py
--rw-rw-r--   0 test      (1001) test      (1001)    16279 2023-08-04 08:55:20.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/ocr/imagebox.py
--rw-rw-r--   0 test      (1001) test      (1001)     3625 2023-08-04 09:10:20.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/ocr/main.py
--rw-rw-r--   0 test      (1001) test      (1001)     6286 2023-07-26 05:47:05.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/ocr/model_layoutmlv2.py
--rw-rw-r--   0 test      (1001) test      (1001)     2160 2023-08-04 08:16:49.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/ocr/model_paddle.py
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-04 09:13:32.237408 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/utils/
--rw-rw-r--   0 test      (1001) test      (1001)      457 2023-08-04 08:57:51.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/utils/__init__.py
--rw-rw-r--   0 test      (1001) test      (1001)     7186 2023-08-04 09:09:14.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/utils/annotation.py
--rw-rw-r--   0 test      (1001) test      (1001)     4896 2023-08-01 04:32:01.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/utils/color_system.py
--rw-rw-r--   0 test      (1001) test      (1001)     3820 2023-08-03 10:44:05.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/utils/imaging.py
--rw-rw-r--   0 test      (1001) test      (1001)     2402 2023-08-02 09:28:26.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/utils/pixel_mask.py
--rw-rw-r--   0 test      (1001) test      (1001)     5469 2023-08-03 03:51:23.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/utils/timing.py
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-04 09:13:32.237408 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision.egg-info/
--rw-rw-r--   0 test      (1001) test      (1001)     2845 2023-08-04 09:13:32.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision.egg-info/PKG-INFO
--rw-rw-r--   0 test      (1001) test      (1001)     1052 2023-08-04 09:13:32.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision.egg-info/SOURCES.txt
--rw-rw-r--   0 test      (1001) test      (1001)        1 2023-08-04 09:13:32.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision.egg-info/dependency_links.txt
--rw-rw-r--   0 test      (1001) test      (1001)       74 2023-08-04 09:13:32.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision.egg-info/top_level.txt
--rw-rw-r--   0 test      (1001) test      (1001)    11005 2023-07-26 06:47:33.000000 image2layout_computer_vision-0.1.0/src/sandbox.py
--rw-rw-r--   0 test      (1001) test      (1001)    11193 2023-08-03 04:03:51.000000 image2layout_computer_vision-0.1.0/src/sandbox_color.py
--rw-rw-r--   0 test      (1001) test      (1001)     1246 2023-08-04 09:11:31.000000 image2layout_computer_vision-0.1.0/src/sandbox_ocr.py
--rw-rw-r--   0 test      (1001) test      (1001)      812 2023-08-03 04:47:50.000000 image2layout_computer_vision-0.1.0/src/test_color.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 06:12:59.328899 image2layout_computer_vision-0.1.1/
+-rw-rw-r--   0 test      (1001) test      (1001)     1073 2023-07-20 04:03:09.000000 image2layout_computer_vision-0.1.1/LICENSE
+-rw-rw-r--   0 test      (1001) test      (1001)     2794 2023-08-07 06:12:59.328899 image2layout_computer_vision-0.1.1/PKG-INFO
+-rw-rw-r--   0 test      (1001) test      (1001)     2224 2023-08-04 10:07:30.000000 image2layout_computer_vision-0.1.1/README.md
+-rw-rw-r--   0 test      (1001) test      (1001)      637 2023-08-07 06:08:55.000000 image2layout_computer_vision-0.1.1/pyproject.toml
+-rw-rw-r--   0 test      (1001) test      (1001)       38 2023-08-07 06:12:59.328899 image2layout_computer_vision-0.1.1/setup.cfg
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 06:12:59.324899 image2layout_computer_vision-0.1.1/src/
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 06:12:59.324899 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/
+-rw-rw-r--   0 test      (1001) test      (1001)      613 2023-08-04 08:58:07.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/__init__.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 06:12:59.328899 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/color_extract/
+-rw-rw-r--   0 test      (1001) test      (1001)       95 2023-08-01 04:32:01.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/color_extract/__init__.py
+-rw-rw-r--   0 test      (1001) test      (1001)    14464 2023-08-03 04:42:22.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/color_extract/main.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 06:12:59.328899 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/ocr/
+-rw-rw-r--   0 test      (1001) test      (1001)      251 2023-08-04 08:48:54.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/ocr/__init__.py
+-rw-rw-r--   0 test      (1001) test      (1001)    16279 2023-08-04 08:55:20.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/ocr/imagebox.py
+-rw-rw-r--   0 test      (1001) test      (1001)     3625 2023-08-04 09:10:20.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/ocr/main.py
+-rw-rw-r--   0 test      (1001) test      (1001)     6286 2023-07-26 05:47:05.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/ocr/model_layoutmlv2.py
+-rw-rw-r--   0 test      (1001) test      (1001)     2168 2023-08-07 06:07:52.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/ocr/model_paddle.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 06:12:59.328899 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/utils/
+-rw-rw-r--   0 test      (1001) test      (1001)      457 2023-08-04 08:57:51.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/utils/__init__.py
+-rw-rw-r--   0 test      (1001) test      (1001)     7186 2023-08-04 09:09:14.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/utils/annotation.py
+-rw-rw-r--   0 test      (1001) test      (1001)     4896 2023-08-01 04:32:01.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/utils/color_system.py
+-rw-rw-r--   0 test      (1001) test      (1001)     3820 2023-08-03 10:44:05.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/utils/imaging.py
+-rw-rw-r--   0 test      (1001) test      (1001)     2402 2023-08-02 09:28:26.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/utils/pixel_mask.py
+-rw-rw-r--   0 test      (1001) test      (1001)     5469 2023-08-03 03:51:23.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/utils/timing.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 06:12:59.324899 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision.egg-info/
+-rw-rw-r--   0 test      (1001) test      (1001)     2794 2023-08-07 06:12:59.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision.egg-info/PKG-INFO
+-rw-rw-r--   0 test      (1001) test      (1001)     1052 2023-08-07 06:12:59.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision.egg-info/SOURCES.txt
+-rw-rw-r--   0 test      (1001) test      (1001)        1 2023-08-07 06:12:59.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision.egg-info/dependency_links.txt
+-rw-rw-r--   0 test      (1001) test      (1001)       74 2023-08-07 06:12:59.000000 image2layout_computer_vision-0.1.1/src/image2layout_computer_vision.egg-info/top_level.txt
+-rw-rw-r--   0 test      (1001) test      (1001)    11005 2023-07-26 06:47:33.000000 image2layout_computer_vision-0.1.1/src/sandbox.py
+-rw-rw-r--   0 test      (1001) test      (1001)    11193 2023-08-03 04:03:51.000000 image2layout_computer_vision-0.1.1/src/sandbox_color.py
+-rw-rw-r--   0 test      (1001) test      (1001)     1246 2023-08-04 09:11:31.000000 image2layout_computer_vision-0.1.1/src/sandbox_ocr.py
+-rw-rw-r--   0 test      (1001) test      (1001)      812 2023-08-03 04:47:50.000000 image2layout_computer_vision-0.1.1/src/test_color.py
```

### Comparing `image2layout_computer_vision-0.1.0/LICENSE` & `image2layout_computer_vision-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.0/PKG-INFO` & `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: image2layout_computer_vision
-Version: 0.1.0
+Name: image2layout-computer-vision
+Version: 0.1.1
 Summary: image processing and stuff
 Author-email: Felix Do <felix.do.1030@gmail.com>
 Project-URL: Homepage, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Project-URL: Bug Tracker, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,37 +35,31 @@
 rm ~/conda.sh
 conda init --all --dry-run --verbose
 
 conda create -n cv python=3.10 -y
 conda activate cv
 ```
 
-2. Tesseract
-
-```bash
-sudo apt install tesseract-ocr libtesseract-dev -y
-```
-
-
 3. Python libraries (python>=3.8)
 
 ```bash
 # python -m pip install 'torch>=2.0' torchvision torchaudio
-conda install pytorch torchvision torchaudio cpuonly -c pytorch --name cv -y
-
-python -m pip install Pillow pandas numpy scikit-learn pyyaml==5.1 chardet pytesseract
-python -m pip install --upgrade datasets transformers
+python -m pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cpu
 
-python -m pip install 'git+https://github.com/facebookresearch/detectron2.git'
+python -m pip install datasets transformers scikit-learn
+python -m pip install --upgrade datasets transformers scikit-learn Pillow numpy pandas
+python -m pip install paddleocr paddlepaddle
 
 python -m pip install --upgrade image2layout-computer-vision
 ```
 
 ### Install with `docker`
 
+> OUTDATED - update in progress
+
 <!-- Replace `Dockerfile_cpu` with `Dockerfile` if running with GPU (not yet supported) -->
 ```bash
 sudo docker build --tag cv -f Dockerfile_cpu .
 
 sudo docker run -it -p 0.0.0.0:8000:8000 -p 0.0.0.0:8001:8001 -v $(pwd):/app cv bash
 
 ```
@@ -88,15 +82,15 @@
 
 2. Recognize texts
 
 ```python
 import image2layout_computer_vision as icv
 
 # 2 lists of dicts with keys [text, box, score]
-data_merged, data_raw = detect_text_full('path/to/image.png')
+data_merged, data_raw = icv.detect_text_full('path/to/image.png')
 ```
 
 3. Extract colors
 ```python
 import image2layout_computer_vision as icv
 
 color_bg, color_fg = icv.extract_colors('path/to/image.png')
```

### Comparing `image2layout_computer_vision-0.1.0/README.md` & `image2layout_computer_vision-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: image2layout_computer_vision
+Version: 0.1.1
+Summary: image processing and stuff
+Author-email: Felix Do <felix.do.1030@gmail.com>
+Project-URL: Homepage, https://github.com/felix-do-wizardry/image2layout-computer-vision
+Project-URL: Bug Tracker, https://github.com/felix-do-wizardry/image2layout-computer-vision
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # image2layout_computer_vision
 
 An image processing module for some computer vision tasks (public module for image2layout)
 
 Package Page: [pypi](https://pypi.org/project/image2layout-computer-vision/)
 
 Features:
@@ -21,37 +35,31 @@
 rm ~/conda.sh
 conda init --all --dry-run --verbose
 
 conda create -n cv python=3.10 -y
 conda activate cv
 ```
 
-2. Tesseract
-
-```bash
-sudo apt install tesseract-ocr libtesseract-dev -y
-```
-
-
 3. Python libraries (python>=3.8)
 
 ```bash
 # python -m pip install 'torch>=2.0' torchvision torchaudio
-conda install pytorch torchvision torchaudio cpuonly -c pytorch --name cv -y
+python -m pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cpu
 
-python -m pip install Pillow pandas numpy scikit-learn pyyaml==5.1 chardet pytesseract
-python -m pip install --upgrade datasets transformers
-
-python -m pip install 'git+https://github.com/facebookresearch/detectron2.git'
+python -m pip install datasets transformers scikit-learn
+python -m pip install --upgrade datasets transformers scikit-learn Pillow numpy pandas
+python -m pip install paddleocr paddlepaddle
 
 python -m pip install --upgrade image2layout-computer-vision
 ```
 
 ### Install with `docker`
 
+> OUTDATED - update in progress
+
 <!-- Replace `Dockerfile_cpu` with `Dockerfile` if running with GPU (not yet supported) -->
 ```bash
 sudo docker build --tag cv -f Dockerfile_cpu .
 
 sudo docker run -it -p 0.0.0.0:8000:8000 -p 0.0.0.0:8001:8001 -v $(pwd):/app cv bash
 
 ```
@@ -74,15 +82,15 @@
 
 2. Recognize texts
 
 ```python
 import image2layout_computer_vision as icv
 
 # 2 lists of dicts with keys [text, box, score]
-data_merged, data_raw = detect_text_full('path/to/image.png')
+data_merged, data_raw = icv.detect_text_full('path/to/image.png')
 ```
 
 3. Extract colors
 ```python
 import image2layout_computer_vision as icv
 
 color_bg, color_fg = icv.extract_colors('path/to/image.png')
```

### Comparing `image2layout_computer_vision-0.1.0/pyproject.toml` & `image2layout_computer_vision-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "Pillow",
   "numpy",
   "pandas",
 ]
 
 [project]
 name = "image2layout_computer_vision"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Felix Do", email="felix.do.1030@gmail.com" },
 ]
 description = "image processing and stuff"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/__init__.py` & `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/__init__.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/color_extract/main.py` & `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/color_extract/main.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/ocr/imagebox.py` & `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/ocr/imagebox.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/ocr/main.py` & `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/ocr/main.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/ocr/model_layoutmlv2.py` & `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/ocr/model_layoutmlv2.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/ocr/model_paddle.py` & `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/ocr/model_paddle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # %%
-from paddleocr import PaddleOCR, draw_ocr
 import time, os
 import numpy as np
 import pandas as pd
 import string
 import colorsys
 from PIL import Image, ImageDraw, ImageFont
 
@@ -29,14 +28,15 @@
             self._load()
     
     
     def __call__(self, *args, **kwargs):
         return self.forward(*args, **kwargs)
     
     def _load(self):
+        from paddleocr import PaddleOCR, draw_ocr
         self.paddle_ocr = PaddleOCR(
             lang='en',
             use_gpu=self.device in ['cuda'],
             use_angle_cls=True,
         )
         self.loaded = True
```

### Comparing `image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/utils/annotation.py` & `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/utils/annotation.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/utils/color_system.py` & `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/utils/color_system.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/utils/imaging.py` & `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/utils/imaging.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/utils/pixel_mask.py` & `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/utils/pixel_mask.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/utils/timing.py` & `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision/utils/timing.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.0/src/image2layout_computer_vision.egg-info/PKG-INFO` & `image2layout_computer_vision-0.1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: image2layout-computer-vision
-Version: 0.1.0
-Summary: image processing and stuff
-Author-email: Felix Do <felix.do.1030@gmail.com>
-Project-URL: Homepage, https://github.com/felix-do-wizardry/image2layout-computer-vision
-Project-URL: Bug Tracker, https://github.com/felix-do-wizardry/image2layout-computer-vision
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # image2layout_computer_vision
 
 An image processing module for some computer vision tasks (public module for image2layout)
 
 Package Page: [pypi](https://pypi.org/project/image2layout-computer-vision/)
 
 Features:
@@ -35,37 +21,31 @@
 rm ~/conda.sh
 conda init --all --dry-run --verbose
 
 conda create -n cv python=3.10 -y
 conda activate cv
 ```
 
-2. Tesseract
-
-```bash
-sudo apt install tesseract-ocr libtesseract-dev -y
-```
-
-
 3. Python libraries (python>=3.8)
 
 ```bash
 # python -m pip install 'torch>=2.0' torchvision torchaudio
-conda install pytorch torchvision torchaudio cpuonly -c pytorch --name cv -y
+python -m pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cpu
 
-python -m pip install Pillow pandas numpy scikit-learn pyyaml==5.1 chardet pytesseract
-python -m pip install --upgrade datasets transformers
-
-python -m pip install 'git+https://github.com/facebookresearch/detectron2.git'
+python -m pip install datasets transformers scikit-learn
+python -m pip install --upgrade datasets transformers scikit-learn Pillow numpy pandas
+python -m pip install paddleocr paddlepaddle
 
 python -m pip install --upgrade image2layout-computer-vision
 ```
 
 ### Install with `docker`
 
+> OUTDATED - update in progress
+
 <!-- Replace `Dockerfile_cpu` with `Dockerfile` if running with GPU (not yet supported) -->
 ```bash
 sudo docker build --tag cv -f Dockerfile_cpu .
 
 sudo docker run -it -p 0.0.0.0:8000:8000 -p 0.0.0.0:8001:8001 -v $(pwd):/app cv bash
 
 ```
@@ -88,15 +68,15 @@
 
 2. Recognize texts
 
 ```python
 import image2layout_computer_vision as icv
 
 # 2 lists of dicts with keys [text, box, score]
-data_merged, data_raw = detect_text_full('path/to/image.png')
+data_merged, data_raw = icv.detect_text_full('path/to/image.png')
 ```
 
 3. Extract colors
 ```python
 import image2layout_computer_vision as icv
 
 color_bg, color_fg = icv.extract_colors('path/to/image.png')
```

### Comparing `image2layout_computer_vision-0.1.0/src/image2layout_computer_vision.egg-info/SOURCES.txt` & `image2layout_computer_vision-0.1.1/src/image2layout_computer_vision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.0/src/sandbox.py` & `image2layout_computer_vision-0.1.1/src/sandbox.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.0/src/sandbox_color.py` & `image2layout_computer_vision-0.1.1/src/sandbox_color.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.0/src/sandbox_ocr.py` & `image2layout_computer_vision-0.1.1/src/sandbox_ocr.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.0/src/test_color.py` & `image2layout_computer_vision-0.1.1/src/test_color.py`

 * *Files identical despite different names*

