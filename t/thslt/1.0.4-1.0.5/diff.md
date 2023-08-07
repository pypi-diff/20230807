# Comparing `tmp/thslt-1.0.4.tar.gz` & `tmp/thslt-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thslt-1.0.4.tar", last modified: Fri Aug  4 18:49:05 2023, max compression
+gzip compressed data, was "thslt-1.0.5.tar", last modified: Mon Aug  7 15:59:04 2023, max compression
```

## Comparing `thslt-1.0.4.tar` & `thslt-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 18:49:05.480769 thslt-1.0.4/
--rw-rw-rw-   0        0        0     1074 2023-08-03 02:26:25.000000 thslt-1.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0       21 2023-08-04 15:50:02.000000 thslt-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     5658 2023-08-04 18:49:05.478767 thslt-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5162 2023-08-04 18:44:20.000000 thslt-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-08-04 18:49:05.480769 thslt-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      739 2023-08-04 18:47:32.000000 thslt-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 18:49:05.359767 thslt-1.0.4/thslt/
--rw-rw-rw-   0        0        0    38915 2023-08-04 04:26:46.000000 thslt-1.0.4/thslt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 18:49:05.475768 thslt-1.0.4/thslt.egg-info/
--rw-rw-rw-   0        0        0     5658 2023-08-04 18:49:05.000000 thslt-1.0.4/thslt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-08-04 18:49:05.000000 thslt-1.0.4/thslt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 18:49:05.000000 thslt-1.0.4/thslt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-08-04 18:49:05.000000 thslt-1.0.4/thslt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 15:59:04.947897 thslt-1.0.5/
+-rw-rw-rw-   0        0        0     1074 2023-08-03 02:26:25.000000 thslt-1.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       21 2023-08-04 15:50:02.000000 thslt-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     5580 2023-08-07 15:59:04.945896 thslt-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5014 2023-08-07 15:56:59.000000 thslt-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-07 15:59:04.947897 thslt-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      809 2023-08-07 15:58:39.000000 thslt-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 15:59:04.879898 thslt-1.0.5/thslt/
+-rw-rw-rw-   0        0        0    38915 2023-08-04 04:26:46.000000 thslt-1.0.5/thslt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 15:59:04.942897 thslt-1.0.5/thslt.egg-info/
+-rw-rw-rw-   0        0        0     5580 2023-08-07 15:59:03.000000 thslt-1.0.5/thslt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-08-07 15:59:04.000000 thslt-1.0.5/thslt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 15:59:03.000000 thslt-1.0.5/thslt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-07 15:59:04.000000 thslt-1.0.5/thslt.egg-info/top_level.txt
```

### Comparing `thslt-1.0.4/LICENSE.txt` & `thslt-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thslt-1.0.4/PKG-INFO` & `thslt-1.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: thslt
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Thai sign language translator library used with Mediapipe that translate Thai hand sign language into plain Thai characters. 
+Home-page: https://github.com/Mon4sm/Thai-sign-language-translator.git
 Author: Papangkon Ninarundech
-Author-email: papangkonsk@gmail.com
+Author-email: realninzx@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -20,15 +21,14 @@
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [Configuration](#configuration)
 - [Features](#features)
-- [Documentation](#documentation)
 - [License](#license)
 - [Support](#support)
 - [Acknowledgments](#acknowledgments)
 
 ## Installation
 ### Use the following methods to install nessecary libraries
  - To install OpenCV, use the following command
@@ -97,39 +97,32 @@
 text_encode = [] 
 ```
 
 ## Features
 ### Translate
   - use this function after you create a loop for OpenCV
 ```
-translate(frame,handlabel,results,text_encode)
+translate(frame,results,text_encode)
 ```
+#### Parameters
 - frame = capture.read()
 - results = Hands.process(bgrtorgb)
 - text_encode = [ ]
 ### Decode
  - use this function after you exit the loop for OpenCV to encode <span style="background-color: gray; padding: 2px 4px; border-radius: 4px; color:black;">text_encode</span>
 ```
 translation = encode(text_encode)
 ```
-## Documentation
-
-The document is not finished yet.
-
 ## License
 
 Copyright 2023 Papangkon Ninarundech
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-## Support
-
-Contact +66 097-153-3812 for more information
-
 ## Acknowledgments
 
 Thank you to the individuals who assisted in creating this project.
  - Mr.Jiraroj Wiruchpongsanon
```

### Comparing `thslt-1.0.4/README.md` & `thslt-1.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [Configuration](#configuration)
 - [Features](#features)
-- [Documentation](#documentation)
 - [License](#license)
 - [Support](#support)
 - [Acknowledgments](#acknowledgments)
 
 ## Installation
 ### Use the following methods to install nessecary libraries
  - To install OpenCV, use the following command
@@ -84,39 +83,32 @@
 text_encode = [] 
 ```
 
 ## Features
 ### Translate
   - use this function after you create a loop for OpenCV
 ```
-translate(frame,handlabel,results,text_encode)
+translate(frame,results,text_encode)
 ```
+#### Parameters
 - frame = capture.read()
 - results = Hands.process(bgrtorgb)
 - text_encode = [ ]
 ### Decode
  - use this function after you exit the loop for OpenCV to encode <span style="background-color: gray; padding: 2px 4px; border-radius: 4px; color:black;">text_encode</span>
 ```
 translation = encode(text_encode)
 ```
-## Documentation
-
-The document is not finished yet.
-
 ## License
 
 Copyright 2023 Papangkon Ninarundech
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-## Support
-
-Contact +66 097-153-3812 for more information
-
 ## Acknowledgments
 
 Thank you to the individuals who assisted in creating this project.
  - Mr.Jiraroj Wiruchpongsanon
```

### Comparing `thslt-1.0.4/setup.py` & `thslt-1.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="thslt",
-    version="1.0.4 ",
+    version="1.0.5 ",
     author="Papangkon Ninarundech",
-    author_email="papangkonsk@gmail.com",
+    author_email="realninzx@gmail.com",
+    url="https://github.com/Mon4sm/Thai-sign-language-translator.git",
     description="A Thai sign language translator library used with Mediapipe that translate Thai hand sign language into plain Thai characters. ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: MIT License",
```

### Comparing `thslt-1.0.4/thslt/__init__.py` & `thslt-1.0.5/thslt/__init__.py`

 * *Files identical despite different names*

### Comparing `thslt-1.0.4/thslt.egg-info/PKG-INFO` & `thslt-1.0.5/thslt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: thslt
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Thai sign language translator library used with Mediapipe that translate Thai hand sign language into plain Thai characters. 
+Home-page: https://github.com/Mon4sm/Thai-sign-language-translator.git
 Author: Papangkon Ninarundech
-Author-email: papangkonsk@gmail.com
+Author-email: realninzx@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -20,15 +21,14 @@
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [Configuration](#configuration)
 - [Features](#features)
-- [Documentation](#documentation)
 - [License](#license)
 - [Support](#support)
 - [Acknowledgments](#acknowledgments)
 
 ## Installation
 ### Use the following methods to install nessecary libraries
  - To install OpenCV, use the following command
@@ -97,39 +97,32 @@
 text_encode = [] 
 ```
 
 ## Features
 ### Translate
   - use this function after you create a loop for OpenCV
 ```
-translate(frame,handlabel,results,text_encode)
+translate(frame,results,text_encode)
 ```
+#### Parameters
 - frame = capture.read()
 - results = Hands.process(bgrtorgb)
 - text_encode = [ ]
 ### Decode
  - use this function after you exit the loop for OpenCV to encode <span style="background-color: gray; padding: 2px 4px; border-radius: 4px; color:black;">text_encode</span>
 ```
 translation = encode(text_encode)
 ```
-## Documentation
-
-The document is not finished yet.
-
 ## License
 
 Copyright 2023 Papangkon Ninarundech
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-## Support
-
-Contact +66 097-153-3812 for more information
-
 ## Acknowledgments
 
 Thank you to the individuals who assisted in creating this project.
  - Mr.Jiraroj Wiruchpongsanon
```

