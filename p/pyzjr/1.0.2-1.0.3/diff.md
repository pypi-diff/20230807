# Comparing `tmp/pyzjr-1.0.2.tar.gz` & `tmp/pyzjr-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyzjr-1.0.2.tar", last modified: Thu Aug  3 09:12:55 2023, max compression
+gzip compressed data, was "dist\pyzjr-1.0.3.tar", last modified: Mon Aug  7 17:19:04 2023, max compression
```

## Comparing `pyzjr-1.0.2.tar` & `pyzjr-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 09:12:55.000000 pyzjr-1.0.2/
--rw-rw-rw-   0        0        0     2838 2023-08-03 09:12:55.000000 pyzjr-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1634 2023-07-27 10:30:52.000000 pyzjr-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 09:12:55.000000 pyzjr-1.0.2/pyzjr/
--rw-rw-rw-   0        0        0     3959 2023-07-02 08:05:46.000000 pyzjr-1.0.2/pyzjr/ColorModule.py
--rw-rw-rw-   0        0        0    17203 2023-07-11 01:30:30.000000 pyzjr-1.0.2/pyzjr/Enimage.py
--rw-rw-rw-   0        0        0     3654 2023-08-03 09:11:06.000000 pyzjr-1.0.2/pyzjr/FM.py
--rw-rw-rw-   0        0        0     9085 2023-07-15 12:01:54.000000 pyzjr-1.0.2/pyzjr/MinIO.py
--rw-rw-rw-   0        0        0     7996 2023-08-02 11:13:43.000000 pyzjr-1.0.2/pyzjr/PIC.py
--rw-rw-rw-   0        0        0     6505 2023-07-26 16:48:15.000000 pyzjr-1.0.2/pyzjr/Showimage.py
--rw-rw-rw-   0        0        0     4544 2023-07-04 09:36:13.000000 pyzjr-1.0.2/pyzjr/TrackBar.py
--rw-rw-rw-   0        0        0      312 2023-07-12 11:15:25.000000 pyzjr-1.0.2/pyzjr/Z.py
--rw-rw-rw-   0        0        0      976 2023-08-03 09:12:37.000000 pyzjr-1.0.2/pyzjr/__init__.py
--rw-rw-rw-   0        0        0     6168 2023-08-02 08:10:51.000000 pyzjr-1.0.2/pyzjr/definition.py
--rw-rw-rw-   0        0        0     2491 2023-08-02 10:24:51.000000 pyzjr-1.0.2/pyzjr/utils.py
--rw-rw-rw-   0        0        0     4832 2023-07-24 15:58:50.000000 pyzjr-1.0.2/pyzjr/video.py
--rw-rw-rw-   0        0        0     3637 2023-07-27 04:09:54.000000 pyzjr-1.0.2/pyzjr/zmath.py
-drwxrwxrwx   0        0        0        0 2023-08-03 09:12:55.000000 pyzjr-1.0.2/pyzjr.egg-info/
--rw-rw-rw-   0        0        0     2838 2023-08-03 09:12:54.000000 pyzjr-1.0.2/pyzjr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-08-03 09:12:55.000000 pyzjr-1.0.2/pyzjr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 09:12:54.000000 pyzjr-1.0.2/pyzjr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-08-03 09:12:54.000000 pyzjr-1.0.2/pyzjr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-08-03 09:12:54.000000 pyzjr-1.0.2/pyzjr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 09:12:55.000000 pyzjr-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2044 2023-08-03 09:11:55.000000 pyzjr-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 17:19:04.000000 pyzjr-1.0.3/
+-rw-rw-rw-   0        0        0     2838 2023-08-07 17:19:04.000000 pyzjr-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1634 2023-07-27 10:30:52.000000 pyzjr-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 17:19:04.000000 pyzjr-1.0.3/pyzjr/
+-rw-rw-rw-   0        0        0     3959 2023-07-02 08:05:46.000000 pyzjr-1.0.3/pyzjr/ColorModule.py
+-rw-rw-rw-   0        0        0    17203 2023-07-11 01:30:30.000000 pyzjr-1.0.3/pyzjr/Enimage.py
+-rw-rw-rw-   0        0        0     2779 2023-08-03 14:18:50.000000 pyzjr-1.0.3/pyzjr/FM.py
+-rw-rw-rw-   0        0        0    10325 2023-08-05 14:35:09.000000 pyzjr-1.0.3/pyzjr/PIC.py
+-rw-rw-rw-   0        0        0     6505 2023-07-26 16:48:15.000000 pyzjr-1.0.3/pyzjr/Showimage.py
+-rw-rw-rw-   0        0        0     4544 2023-07-04 09:36:13.000000 pyzjr-1.0.3/pyzjr/TrackBar.py
+-rw-rw-rw-   0        0        0      706 2023-08-07 17:18:38.000000 pyzjr-1.0.3/pyzjr/Z.py
+-rw-rw-rw-   0        0        0      949 2023-08-07 17:18:40.000000 pyzjr-1.0.3/pyzjr/__init__.py
+-rw-rw-rw-   0        0        0     6168 2023-08-02 08:10:51.000000 pyzjr-1.0.3/pyzjr/definition.py
+-rw-rw-rw-   0        0        0     2358 2023-08-05 16:23:19.000000 pyzjr-1.0.3/pyzjr/net.py
+-rw-rw-rw-   0        0        0     3274 2023-08-07 04:37:03.000000 pyzjr-1.0.3/pyzjr/utils.py
+-rw-rw-rw-   0        0        0     4832 2023-07-24 15:58:50.000000 pyzjr-1.0.3/pyzjr/video.py
+-rw-rw-rw-   0        0        0     3637 2023-08-04 13:06:34.000000 pyzjr-1.0.3/pyzjr/zmath.py
+drwxrwxrwx   0        0        0        0 2023-08-07 17:19:04.000000 pyzjr-1.0.3/pyzjr.egg-info/
+-rw-rw-rw-   0        0        0     2838 2023-08-07 17:19:04.000000 pyzjr-1.0.3/pyzjr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-08-07 17:19:04.000000 pyzjr-1.0.3/pyzjr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 17:19:04.000000 pyzjr-1.0.3/pyzjr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-08-07 17:19:04.000000 pyzjr-1.0.3/pyzjr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-07 17:19:04.000000 pyzjr-1.0.3/pyzjr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 17:19:04.000000 pyzjr-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2051 2023-08-07 17:18:39.000000 pyzjr-1.0.3/setup.py
```

### Comparing `pyzjr-1.0.2/PKG-INFO` & `pyzjr-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzjr
-Version: 1.0.2
+Version: 1.0.3
 Summary:  A computer vision library that supports Win, packaged with patches for visual libraries such as                 Opencv, matplotlib, and image. In the future, Pytorch will also be supported, all of which are personal (Auorui)                 engineering code experience. 
 Home-page: https://github.com/Auorui/pyzjr
 Author: Auorui
 Author-email: zjricetea@gmail.com
 License: MIT
 Description: 
         # pyzjr
```

### Comparing `pyzjr-1.0.2/README.md` & `pyzjr-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyzjr-1.0.2/pyzjr/ColorModule.py` & `pyzjr-1.0.3/pyzjr/ColorModule.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.0.2/pyzjr/Enimage.py` & `pyzjr-1.0.3/pyzjr/Enimage.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.0.2/pyzjr/FM.py` & `pyzjr-1.0.3/pyzjr/FM.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,29 @@
-from tqdm import tqdm
-import requests
 import cv2
 import os, shutil
-from matplotlib import pyplot as plt
 from PIL import Image
 import imghdr
 
 
-def download_file(url):
-    """
-    :param url:下载文件所在url链接
-    :return: 下载的位置处于根目录
-    """
-    print("------", "Start download with urllib")
-    name = url.split("/")[-1]
-    resp = requests.get(url, stream=True)
-    content_size = int(resp.headers['Content-Length']) / 1024  # 确定整个安装包的大小
-    # 下载到上一级目录
-    path = os.path.abspath(os.path.dirname(os.getcwd())) + "\\" + name
-    # 下载到该目录
-    path = os.getcwd() + "\\" + name
-    print("File path:  ", path)
-    with open(path, "wb") as file:
-        print("File total size is:  ", content_size)
-        for data in tqdm(iterable=resp.iter_content(1024), total=content_size, unit='k', desc=name):
-            file.write(data)
-    print("------", "finish download with urllib\n\n")
-
-def getPhotopath(paths):
+def getPhotopath(paths,debug=True):
     """
     * log
         0.0.19以后修改了一个比较大的bug
         1.0.2后将图片和所有文件路径分开
     :param paths: 文件夹路径
     :return: 包含图片路径的列表
     """
     img_formats = ['jpg', 'jpeg', 'png', 'gif', 'bmp', 'tif', 'tiff', 'webp', 'raw']
     imgfile = []
     allfile = []
     file_list = os.listdir(paths)
     for i in file_list:
-        if i[0] in ['n', 't', 'r', 'b', 'f'] or i[0].isdigit():
-            print(f"Error: 文件名 {i} 开头出现错误！")
+        if debug:
+            if i[0] in ['n', 't', 'r', 'b', 'f'] or i[0].isdigit():
+                print(f"Error: 文件名 {i} 开头出现错误！")
         newph = os.path.join(paths, i).replace("\\", "/")
         allfile.append(newph)
         _, file_ext = os.path.splitext(newph)
         if file_ext[1:] in img_formats:
             imgfile.append(newph)
 
     return imgfile,allfile
```

### Comparing `pyzjr-1.0.2/pyzjr/PIC.py` & `pyzjr-1.0.3/pyzjr/PIC.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import cv2
 from pylab import *
 import pyzjr.TrackBar as Trace
 import pyzjr.Z as Z
-
-from skimage.morphology import skeletonize
-from skimage.filters import threshold_otsu
+from pyzjr.zmath import *
+from skimage.morphology import skeletonize,disk
+from skimage.filters import threshold_otsu,rank
 from skimage.color import rgb2gray
 from skimage import measure
 
+
 from torchvision import transforms
 
 def addnoisy(image, n=10000):
     """
     :param image: 原始图像
     :param n: 添加椒盐的次数,默认为10000
     :return: 返回被椒盐处理后的图像
@@ -201,8 +202,71 @@
     mask = np.zeros(image.shape, dtype=np.uint8)
     for box in boxes:
         x1, y1, x2, y2 = box
         mask[y1:y2, x1:x2] = 255
     if mask.ndim == 3 and mask.shape[-1] > 1:
         mask = mask[:, :, 0]
     masked_image = cv2.bitwise_and(image, image, mask=mask)
-    return mask, masked_image
+    return mask, masked_image
+
+
+def bilinear_interpolation(image, scale):
+    """
+    双线性插值
+    :param image: 原始图像。
+    :param scale: 规格,如1.5为,放大1.5倍
+    """
+    ah, aw, channel = image.shape
+    bh, bw = int(ah * scale), int(aw * scale)
+    dst_img = np.zeros((bh, bw, channel), np.uint8)
+
+    y_coords, x_coords = np.meshgrid(np.arange(bh), np.arange(bw), indexing='ij')
+    AX = (x_coords + 0.5) / scale - 0.5   # 移向像素中心
+    AY = (y_coords + 0.5) / scale - 0.5
+
+    x1 = np.floor(AX).astype(int)
+    y1 = np.floor(AY).astype(int)
+    x2 = np.minimum(x1 + 1, aw - 1)
+    y2 = np.minimum(y1 + 1, ah - 1)
+    R1 = ((x2 - AX)[:, :, np.newaxis] * image[y1, x1]).astype(float) + (
+                (AX - x1)[:, :, np.newaxis] * image[y1, x2]).astype(float)
+    R2 = ((x2 - AX)[:, :, np.newaxis] * image[y2, x1]).astype(float) + (
+                (AX - x1)[:, :, np.newaxis] * image[y2, x2]).astype(float)
+
+    dst_img = (y2 - AY)[:, :, np.newaxis] * R1 + (AY - y1)[:, :, np.newaxis] * R2
+
+    return dst_img.astype(np.uint8)
+
+def drawOutline(blackbackground,contours,mode=0,color=Z.green):
+    """
+    绘制边缘轮廓
+    :param blackbackground: 背景图
+    :param contours: [(x,y),...]
+    :param mode: 默认模式0,可选模式0或1
+    :param color: 默认绿色
+    :return: 
+    """
+    if mode==0:
+        contours = Advancedlist(contours, "Y")
+        contour = [np.array([point], dtype=np.int32) for point in contours]
+        cv2.drawContours(blackbackground, contour, -1, color, thickness=-1)
+    elif mode==1:
+        for i in range(len(contours) - 1):
+            start = contours[i]
+            end = contours[i + 1]
+            cv2.line(blackbackground, start, end, color=color, thickness=1)
+
+
+def gradientOutline(img,radius=2):
+    """
+    对图像进行梯度边缘检测，并返回边缘强度图像。
+    
+    :param img: 输入的图像(内部有二值转化)
+    :param radius: 半径,默认为2。
+    :return: 返回经过梯度边缘检测处理后的边缘强度图像
+    """
+    image = BinaryImg(img)
+    denoised = rank.median(image, disk(radius))
+    gradient = rank.gradient(denoised, disk(radius))
+    gradient = cv2.cvtColor(gradient, cv2.COLOR_GRAY2BGR)
+
+    return gradient
```

### Comparing `pyzjr-1.0.2/pyzjr/Showimage.py` & `pyzjr-1.0.3/pyzjr/Showimage.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.0.2/pyzjr/TrackBar.py` & `pyzjr-1.0.3/pyzjr/TrackBar.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.0.2/pyzjr/__init__.py` & `pyzjr-1.0.3/pyzjr/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,27 @@
   At present, it is only for my personal use. If you want to
   use it, please contact me. Here are my email and WeChat.
 - WeChat: z15583909992
 - Email: zjricetea@gmail.com
 - Note: Currently still being updated, please refer to the latest version for any changes that may occur
 """
 
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 
 import cv2
 
 from pyzjr.Enimage import Filter,Enhance,Random_Enhance,Retinex
 from pyzjr.definition import *
 from pyzjr.ColorModule import *
 from pyzjr.definition import *
 from pyzjr.TrackBar import *
 from pyzjr.utils import *
 from pyzjr.video import *
 from pyzjr.Z import * 
 from pyzjr.zmath import *
-from pyzjr.MinIO import *
 from pyzjr.PIC import *
 from pyzjr.FM import *
 from pyzjr.Showimage import *
 
 repair_TELEA=cv2.INPAINT_TELEA
 repair_NS=cv2.INPAINT_NS
 Lap_64F=cv2.CV_64F
```

### Comparing `pyzjr-1.0.2/pyzjr/definition.py` & `pyzjr-1.0.3/pyzjr/definition.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.0.2/pyzjr/utils.py` & `pyzjr-1.0.3/pyzjr/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import cv2
-import math
 import numpy as np
-import os, shutil
 from matplotlib import pyplot as plt
+from PIL import Image
 
 def getContours(img, cThr=(100, 100), showCanny=False, minArea=1000, filter=0, draw=True):
     """
     :param img: 输入图像
     :param cThr: 阈值
     :param showCanny:展示经过处理后的边缘,默认Fales
     :param minArea: 更改大小
@@ -64,8 +63,31 @@
                 if box_area >= fb_area:
                     final_boxes.remove(fb)
                 else:
                     is_inner = True
                     break
         if not is_inner:
             final_boxes.append(box)
-    return final_boxes
+    return final_boxes
+
+def cvt8png(pngpath, target=(255, 255, 255), convert=(128, 0, 0)):
+    """
+    Voc: RGB 8位png彩图转换
+    :param pngpath: 为保证是按照cv2的方式读入,所以传入路径即可
+    :param target: 目标颜色,RGB方式
+    :param convert: 转换颜色,同RGB格式
+    :return:
+    """
+    png = cv2.imread(pngpath)
+    png = cv2.cvtColor(png, cv2.COLOR_BGR2RGB)
+    h, w = png.shape[:2]
+
+    mask = np.all(png == target, axis=-1)
+    out_png = np.zeros((h, w, 3), dtype=np.uint8)
+    out_png[mask] = convert
+    out_png[~mask] = png[~mask]
+
+    out_png_pil = Image.fromarray(out_png)
+    out_png_pil = out_png_pil.convert("P", palette=Image.ADAPTIVE, colors=256)
+    out_png_cv = cv2.cvtColor(np.array(out_png), cv2.COLOR_RGB2BGR)
+
+    return out_png_cv
```

### Comparing `pyzjr-1.0.2/pyzjr/video.py` & `pyzjr-1.0.3/pyzjr/video.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.0.2/pyzjr/zmath.py` & `pyzjr-1.0.3/pyzjr/zmath.py`

 * *Files identical despite different names*

### Comparing `pyzjr-1.0.2/pyzjr.egg-info/PKG-INFO` & `pyzjr-1.0.3/pyzjr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzjr
-Version: 1.0.2
+Version: 1.0.3
 Summary:  A computer vision library that supports Win, packaged with patches for visual libraries such as                 Opencv, matplotlib, and image. In the future, Pytorch will also be supported, all of which are personal (Auorui)                 engineering code experience. 
 Home-page: https://github.com/Auorui/pyzjr
 Author: Auorui
 Author-email: zjricetea@gmail.com
 License: MIT
 Description: 
         # pyzjr
```

### Comparing `pyzjr-1.0.2/setup.py` & `pyzjr-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # these things are needed for the README.md show on pypi (if you dont need delete it)
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 
-VERSION = '1.0.2'
+VERSION = '1.0.3'
 DESCRIPTION = ' A computer vision library that supports Win, packaged with patches for visual libraries such as \
                 Opencv, matplotlib, and image. In the future, Pytorch will also be supported, all of which are personal (Auorui) \
                 engineering code experience. '
 LONG_DESCRIPTION = 'pyzjr is a computer vision library that supports Win'
 
 setup(
     name="pyzjr",
@@ -43,16 +43,16 @@
         'matplotlib',
         'numpy',
         'imageio',
         'scikit-image',
         'torch',
         'opencv-python',
         'pillow',
-        'minio',
-        'torchvision'
+        'torchvision',
+        'torchsummary'
     ],
     keywords=['python', 'computer vision', 'pyzjr','windows'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Microsoft :: Windows",
```

