# Comparing `tmp/poseutil-0.0.9.tar.gz` & `tmp/poseutil-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poseutil-0.0.9.tar", last modified: Wed Jul 19 05:10:42 2023, max compression
+gzip compressed data, was "poseutil-0.1.0.tar", last modified: Mon Aug  7 06:57:43 2023, max compression
```

## Comparing `poseutil-0.0.9.tar` & `poseutil-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 05:10:42.894706 poseutil-0.0.9/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      442 2023-07-19 05:10:42.894545 poseutil-0.0.9/PKG-INFO
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 05:10:42.892690 poseutil-0.0.9/poseutil.egg-info/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      442 2023-07-19 05:10:42.000000 poseutil-0.0.9/poseutil.egg-info/PKG-INFO
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      412 2023-07-19 05:10:42.000000 poseutil-0.0.9/poseutil.egg-info/SOURCES.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-07-19 05:10:42.000000 poseutil-0.0.9/poseutil.egg-info/dependency_links.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-07-19 05:10:42.000000 poseutil-0.0.9/poseutil.egg-info/not-zip-safe
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        6 2023-07-19 05:10:42.000000 poseutil-0.0.9/poseutil.egg-info/top_level.txt
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)       38 2023-07-19 05:10:42.894758 poseutil-0.0.9/setup.cfg
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      600 2023-07-19 05:10:40.000000 poseutil-0.0.9/setup.py
-drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-07-19 05:10:42.894352 poseutil-0.0.9/utils/
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2604 2023-07-19 01:21:30.000000 poseutil-0.0.9/utils/ReadFrameData.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     8057 2023-07-19 03:35:52.000000 poseutil-0.0.9/utils/common_component.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    14188 2023-07-19 01:21:13.000000 poseutil-0.0.9/utils/const.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     1073 2023-07-19 01:20:45.000000 poseutil-0.0.9/utils/csvHelper.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6660 2023-07-19 05:09:23.000000 poseutil-0.0.9/utils/cv_util.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6715 2023-07-19 05:08:52.000000 poseutil-0.0.9/utils/math_util.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    15066 2023-07-19 03:40:40.000000 poseutil-0.0.9/utils/normarlize.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    72850 2023-07-19 05:09:51.000000 poseutil-0.0.9/utils/poseMeasure.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    15159 2023-07-19 01:17:51.000000 poseutil-0.0.9/utils/poseMeasureFormat.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6154 2023-07-19 02:18:56.000000 poseutil-0.0.9/utils/pose_util.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2281 2023-07-19 02:05:47.000000 poseutil-0.0.9/utils/qt_component.py
--rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    11602 2023-07-19 05:10:20.000000 poseutil-0.0.9/utils/version.py
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-08-07 06:57:43.378781 poseutil-0.1.0/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      442 2023-08-07 06:57:43.378626 poseutil-0.1.0/PKG-INFO
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-08-07 06:57:43.376003 poseutil-0.1.0/poseutil.egg-info/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      442 2023-08-07 06:57:43.000000 poseutil-0.1.0/poseutil.egg-info/PKG-INFO
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      412 2023-08-07 06:57:43.000000 poseutil-0.1.0/poseutil.egg-info/SOURCES.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-08-07 06:57:43.000000 poseutil-0.1.0/poseutil.egg-info/dependency_links.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        1 2023-07-19 05:10:42.000000 poseutil-0.1.0/poseutil.egg-info/not-zip-safe
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)        6 2023-08-07 06:57:43.000000 poseutil-0.1.0/poseutil.egg-info/top_level.txt
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)       38 2023-08-07 06:57:43.378826 poseutil-0.1.0/setup.cfg
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)      600 2023-08-07 06:56:57.000000 poseutil-0.1.0/setup.py
+drwxr-xr-x   0 jeong-yeongjae   (501) staff       (20)        0 2023-08-07 06:57:43.378408 poseutil-0.1.0/utils/
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2604 2023-08-07 06:40:06.000000 poseutil-0.1.0/utils/ReadFrameData.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     8541 2023-08-07 06:54:32.000000 poseutil-0.1.0/utils/common_component.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    14188 2023-08-07 06:40:06.000000 poseutil-0.1.0/utils/const.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     1073 2023-08-07 06:40:06.000000 poseutil-0.1.0/utils/csvHelper.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6660 2023-08-07 06:40:06.000000 poseutil-0.1.0/utils/cv_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6715 2023-08-07 06:40:06.000000 poseutil-0.1.0/utils/math_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    15066 2023-08-07 06:40:06.000000 poseutil-0.1.0/utils/normarlize.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    72850 2023-08-07 06:40:06.000000 poseutil-0.1.0/utils/poseMeasure.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    15159 2023-08-07 06:40:06.000000 poseutil-0.1.0/utils/poseMeasureFormat.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     6154 2023-08-07 06:40:06.000000 poseutil-0.1.0/utils/pose_util.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)     2281 2023-08-07 06:40:06.000000 poseutil-0.1.0/utils/qt_component.py
+-rw-r--r--   0 jeong-yeongjae   (501) staff       (20)    11602 2023-08-07 06:40:06.000000 poseutil-0.1.0/utils/version.py
```

### Comparing `poseutil-0.0.9/setup.py` & `poseutil-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='poseutil',
-    version='0.0.9',
+    version='0.1.0',
     description='pose engine utils',
     author='jyj902',
     author_email='jyj902@naver.com',
     url='',
     requires=['sklearn','pandas','numpy','cv2','pickle'],
     py_modules=['utils'],
     packages=['utils'],
```

### Comparing `poseutil-0.0.9/utils/ReadFrameData.py` & `poseutil-0.1.0/utils/ReadFrameData.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.9/utils/common_component.py` & `poseutil-0.1.0/utils/common_component.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 import gzip, pickle
 import numpy as np
 import cv2
 import re, json
 import tensorflow as tf
 import struct, itertools
 import matplotlib.pyplot as plt
-
 from utils.const import *
 from utils.poseMeasure import PoseMeasure
 from utils.normarlize import getPoseEmbeddingList
 from utils.version import VersionCaster
-
+from utils.pose_util import Coordinate
 
 def get_dance_audio_list():
     audio_list_path = DANCE_AUDIO_PATH
     sorted_list = sorted(os.listdir(audio_list_path))
     if 'common' in sorted_list:
         sorted_list.remove('common')
     return sorted(sorted_list)
@@ -40,18 +39,18 @@
     with open(json_path, 'r') as f:
         data =  json.load(f)
     return data[audio_name]
 
 def write_json_data(json_path, data):
     with open(json_path, 'w') as f:
         json.dump(data, f, indent=4)
-    
+
 def get_audio_name(audio_path):
     return audio_path.split("/")[-1].split(".")[0].split("_")[0]
-    
+
 def add_infomation_circle(img, text):
     mask = img.copy()
     cv2.circle(mask, (150,150), 150, (0, 0, 0), -1)
     cv2.putText(mask, text, (60, 220), cv2.FONT_HERSHEY_SIMPLEX, 8, (255, 255, 255), 5)
     return cv2.addWeighted(img, 0.3, mask, 0.7, 0)
 
 def get_speed(audio_path):
@@ -65,15 +64,15 @@
 def sort_list_dir(path):
     dir_list = os.listdir(path)
     dir_list.sort()
     return dir_list
 
 def time_jpg_priority(x):
     return int(x.split('/')[-1].split('.')[0])
-    
+
 def create_directory(directory):
     try:
         if not os.path.exists(directory):
             os.makedirs(directory)
         else:
             shutil.rmtree(directory)
             os.makedirs(directory)
@@ -99,51 +98,46 @@
     with gzip.open(path) as f:
         pickle_data = pickle.load(f)
     return pickle_data
 
 def load_img_list(name):
     img_list = sorted(glob.glob(f"{DANCE_IMG_PATH}/{name}/*.jpg"), key=lambda x: int(x.split("/")[-1].replace(".jpg", "")))
     return img_list
-    
+
 def search_timetable(origin_timetable, compare_timetable, origin_num, compare_num):
     sync_num = 0
     origin_time = origin_timetable[origin_num]
     compare_time = compare_timetable[compare_num]
     while origin_time >= compare_time:
         sync_num += 1
         compare_time = compare_timetable[compare_num + sync_num]
-    
     prev_compare_time = compare_timetable[compare_num + sync_num -1]
-
     if abs(origin_time - compare_time) < abs(origin_time - prev_compare_time):
         return int(compare_num + sync_num), compare_time
     else :
         return int(compare_num + sync_num - 1), prev_compare_time
-
+    
 def rewind_search_timetable(origin_timetable, compare_timetable, origin_num, compare_num):
     sync_num = 0
     origin_time = origin_timetable[origin_num]
     compare_time = compare_timetable[compare_num]
     while origin_time <= compare_time:
         sync_num -= 1
         compare_time = compare_timetable[compare_num + sync_num]
-    
     prev_compare_time = compare_timetable[compare_num + sync_num + 1]
-
     if abs(origin_time - compare_time) < abs(origin_time - prev_compare_time):
         return int(compare_num + sync_num), compare_time
     else :
         return int(compare_num + sync_num + 1), prev_compare_time
     
 def load_tflite_model(path):
     model = tf.lite.Interpreter(model_path=path)
     model.allocate_tensors()
     input_index = model.get_input_details()[0]['index']
     output_index = model.get_output_details()[0]['index']
-
     return model, input_index, output_index
 
 def inference_tflite_model(model, input, input_index, output_index):
     model.set_tensor(input_index, input)
     model.invoke()
     return model.get_tensor(output_index)
 
@@ -172,18 +166,16 @@
         factor *= ratio
     return sorted(emaSmoothing.items(), key=lambda x: x[1], reverse=True)[0][0], emaSmoothing
 
 def process(file):
     unpack_data = []
     with open(file, "rb") as f:
         data = f.read()
-
     for cell in range(0, int(len(data)), 4):
         unpack_data.append(struct.unpack('i', data[cell: cell+4])[0])
-    
     return unpack_data
 
 def pop_header(data):
     casting_data = []
     header = data.pop(0)
     version = VersionCaster(header)
     line = version.get_version_casting_line()
@@ -191,49 +183,56 @@
         casting_data.append(data[line_cnt : line_cnt + line])
     return casting_data, header
 
 def get_bin_data(file):
     bin_data = process(file)
     header = bin_data.pop(0)
     versionCaster = VersionCaster(header)
-
     data = np.array(bin_data)
     info_data = versionCaster.get_data(data)
     return info_data
 
 def plot_confusion_matrix(cm, model_path, target_names=None, cmap=None, normalize=True, labels=True, title='Confusion matrix'):
     accuracy = np.trace(cm) / float(np.sum(cm))
     misclass = 1 - accuracy
-
     if cmap is None:
         cmap = plt.get_cmap('Blues')
-
     if normalize:
         cm = cm.astype('float') / cm.sum(axis=1)[:, np.newaxis]
-        
     plt.figure(figsize=(8, 8))
     plt.imshow(cm, interpolation='nearest', cmap=cmap)
     plt.title(title)
     plt.colorbar()
-
     thresh = cm.max() / 1.5 if normalize else cm.max() / 2
-    
     if target_names is not None:
         tick_marks = np.arange(len(target_names))
         plt.xticks(tick_marks, target_names)
         plt.yticks(tick_marks, target_names)
-    
     if labels:
         for i, j in itertools.product(range(cm.shape[0]), range(cm.shape[1])):
             if normalize:
                 plt.text(j, i, "{:0.4f}".format(cm[i, j]),
                          horizontalalignment="center",
                          color="white" if cm[i, j] > thresh else "black")
             else:
                 plt.text(j, i, "{:,}".format(cm[i, j]),
                          horizontalalignment="center",
                          color="white" if cm[i, j] > thresh else "black")
-
     plt.tight_layout()
     plt.ylabel('True label')
     plt.xlabel('Predicted label\naccuracy={:0.4f}; misclass={:0.4f}'.format(accuracy, misclass))
     plt.savefig(f"{model_path}/confusion_matrix.png")
+
+def flip(frames):
+    flip_data = []
+    for frame in frames:
+        temp = []
+        for idx, coord in enumerate(frame):
+            if idx <= 10:
+                temp.append(coord)
+            else:
+                if idx % 2 == 1:
+                    temp.append(Coordinate(640-frame[idx+1].x, frame[idx+1].y, frame[idx+1].z))
+                else:
+                    temp.append(Coordinate(640-frame[idx-1].x, frame[idx-1].y, frame[idx-1].z))
+        flip_data.append(temp)
+    return flip_data
```

### Comparing `poseutil-0.0.9/utils/const.py` & `poseutil-0.1.0/utils/const.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.9/utils/csvHelper.py` & `poseutil-0.1.0/utils/csvHelper.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.9/utils/cv_util.py` & `poseutil-0.1.0/utils/cv_util.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.9/utils/math_util.py` & `poseutil-0.1.0/utils/math_util.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.9/utils/normarlize.py` & `poseutil-0.1.0/utils/normarlize.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.9/utils/poseMeasure.py` & `poseutil-0.1.0/utils/poseMeasure.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.9/utils/poseMeasureFormat.py` & `poseutil-0.1.0/utils/poseMeasureFormat.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.9/utils/pose_util.py` & `poseutil-0.1.0/utils/pose_util.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.9/utils/qt_component.py` & `poseutil-0.1.0/utils/qt_component.py`

 * *Files identical despite different names*

### Comparing `poseutil-0.0.9/utils/version.py` & `poseutil-0.1.0/utils/version.py`

 * *Files identical despite different names*

