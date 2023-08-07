# Comparing `tmp/neco_f-0.0.6.tar.gz` & `tmp/neco_f-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neco_f-0.0.6.tar", last modified: Sat Aug  5 10:13:18 2023, max compression
+gzip compressed data, was "neco_f-0.0.7.tar", last modified: Mon Aug  7 09:48:41 2023, max compression
```

## Comparing `neco_f-0.0.6.tar` & `neco_f-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 10:13:18.675034 neco_f-0.0.6/
--rw-rw-rw-   0        0        0     1085 2023-08-04 07:53:17.000000 neco_f-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      628 2023-08-05 10:13:18.675034 neco_f-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-08-05 10:13:11.000000 neco_f-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-08-05 10:13:18.660387 neco_f-0.0.6/neco_f.egg-info/
--rw-rw-rw-   0        0        0      628 2023-08-05 10:13:18.000000 neco_f-0.0.6/neco_f.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-08-05 10:13:18.000000 neco_f-0.0.6/neco_f.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 10:13:18.000000 neco_f-0.0.6/neco_f.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      118 2023-08-05 10:13:18.000000 neco_f-0.0.6/neco_f.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-05 10:13:18.000000 neco_f-0.0.6/neco_f.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-05 10:13:18.676011 neco_f-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1166 2023-08-05 10:12:32.000000 neco_f-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-05 10:13:18.673081 neco_f-0.0.6/src/
--rw-rw-rw-   0        0        0        0 2023-08-04 08:13:48.000000 neco_f-0.0.6/src/__init__.py
--rw-rw-rw-   0        0        0     7064 2023-08-05 09:57:20.000000 neco_f-0.0.6/src/always_used.py
--rw-rw-rw-   0        0        0     1459 2023-08-05 09:57:20.000000 neco_f-0.0.6/src/api_.py
--rw-rw-rw-   0        0        0      904 2023-08-04 07:05:59.000000 neco_f-0.0.6/src/auto_pip.py
--rw-rw-rw-   0        0        0     4774 2023-08-05 09:57:20.000000 neco_f-0.0.6/src/internet.py
--rw-rw-rw-   0        0        0     1921 2023-08-05 09:56:00.000000 neco_f-0.0.6/src/jiemi.py
--rw-rw-rw-   0        0        0      505 2023-08-05 10:12:15.000000 neco_f-0.0.6/src/logger.py
--rw-rw-rw-   0        0        0     1161 2023-07-27 08:04:13.000000 neco_f-0.0.6/src/os_time.py
--rw-rw-rw-   0        0        0     1750 2023-08-04 07:10:04.000000 neco_f-0.0.6/src/pic_.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:48:41.691514 neco_f-0.0.7/
+-rw-rw-rw-   0        0        0     1085 2023-08-04 07:53:17.000000 neco_f-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      628 2023-08-07 09:48:41.690514 neco_f-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-08-05 10:13:11.000000 neco_f-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 09:48:41.680514 neco_f-0.0.7/neco_f.egg-info/
+-rw-rw-rw-   0        0        0      628 2023-08-07 09:48:41.000000 neco_f-0.0.7/neco_f.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-08-07 09:48:41.000000 neco_f-0.0.7/neco_f.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 09:48:41.000000 neco_f-0.0.7/neco_f.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-08-07 09:48:41.000000 neco_f-0.0.7/neco_f.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-07 09:48:41.000000 neco_f-0.0.7/neco_f.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 09:48:41.691514 neco_f-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1167 2023-08-07 09:48:23.000000 neco_f-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:48:41.689514 neco_f-0.0.7/src/
+-rw-rw-rw-   0        0        0        0 2023-08-04 08:13:48.000000 neco_f-0.0.7/src/__init__.py
+-rw-rw-rw-   0        0        0     7064 2023-08-05 09:57:20.000000 neco_f-0.0.7/src/always_used.py
+-rw-rw-rw-   0        0        0     1452 2023-08-05 14:17:01.000000 neco_f-0.0.7/src/api_.py
+-rw-rw-rw-   0        0        0      904 2023-08-04 07:05:59.000000 neco_f-0.0.7/src/auto_pip.py
+-rw-rw-rw-   0        0        0     4774 2023-08-05 09:57:20.000000 neco_f-0.0.7/src/internet.py
+-rw-rw-rw-   0        0        0     1904 2023-08-07 09:47:36.000000 neco_f-0.0.7/src/jiemi.py
+-rw-rw-rw-   0        0        0      505 2023-08-05 11:10:04.000000 neco_f-0.0.7/src/logger.py
+-rw-rw-rw-   0        0        0     1151 2023-08-07 09:47:49.000000 neco_f-0.0.7/src/os_time.py
+-rw-rw-rw-   0        0        0     1750 2023-08-04 07:10:04.000000 neco_f-0.0.7/src/pic_.py
```

### Comparing `neco_f-0.0.6/LICENSE` & `neco_f-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `neco_f-0.0.6/PKG-INFO` & `neco_f-0.0.7/neco_f.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: neco_f
-Version: 0.0.6
+Name: neco-f
+Version: 0.0.7
 Summary: 一个鱼龙混杂的库
 Home-page: https://github.com/sweetnotice/neco_f
 Author: neco_arc
 Author-email: 3306601284@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neco_f-0.0.6/neco_f.egg-info/PKG-INFO` & `neco_f-0.0.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: neco-f
-Version: 0.0.6
+Name: neco_f
+Version: 0.0.7
 Summary: 一个鱼龙混杂的库
 Home-page: https://github.com/sweetnotice/neco_f
 Author: neco_arc
 Author-email: 3306601284@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neco_f-0.0.6/setup.py` & `neco_f-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open('README.md', mode='r', encoding='utf-8') as f:
     long_description = f.read()
 setup(
     name='neco_f',
-    version='0.0.6',
+    version='0.0.7',
     author='neco_arc',
     author_email='3306601284@qq.com',
     description='一个鱼龙混杂的库',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/sweetnotice/neco_f',
     classifiers=[
@@ -22,15 +22,15 @@
     install_requires=[
         #    'hm3u8dl-cli',
         # 'pygame',
         'requests',
         'pyinstaller',
         'tqdm',
         'urllib3',
-        'selenium',
+#        'selenium',
         'pycryptodome',  # 解密
         'playsound',  # 音乐播放
         'pyautogui',  # 自动化
         'pillow',  # 图像识别
         'plyer',  # 通知
         'pyexecjs2',  # py解析使用js
         'opencv-python',
```

### Comparing `neco_f-0.0.6/src/always_used.py` & `neco_f-0.0.7/src/always_used.py`

 * *Files identical despite different names*

### Comparing `neco_f-0.0.6/src/api_.py` & `neco_f-0.0.7/src/api_.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# api
 import requests
 import random
 from pprint import pprint
 
 
 class Api:
     def __init__(self):
```

### Comparing `neco_f-0.0.6/src/auto_pip.py` & `neco_f-0.0.7/src/auto_pip.py`

 * *Files identical despite different names*

### Comparing `neco_f-0.0.6/src/internet.py` & `neco_f-0.0.7/src/internet.py`

 * *Files identical despite different names*

### Comparing `neco_f-0.0.6/src/jiemi.py` & `neco_f-0.0.7/src/jiemi.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import base64
-import urllib.parse
-from Crypto.Cipher import AES
-import re
-import base64
-import binascii
-
-
-def debase64_(data: str):
-    return base64.b64decode(data).decode('utf-8').encode().decode('unicode_escape')
-
-
-def deescape_(data: str):
-    return urllib.parse.unquote(data.replace('%u', '\\u').encode().decode('unicode-escape'))
-
-
-def deunicode_(data: str):
-    return data.encode('utf-8').decode('unicode_escape')
-
-
-def deaes_cbc(data: str, key: str, iv: str):
-    def add_16(par):  # ²¹Î»µ½16±¶ÊýÎ»
-        while len(par) % 16 != 0:
-            par += b'\x00'
-        return par
-
-    # ¶Ôkey½øÐÐ²¹Î» ¡£key£¬iv ½øÐÐ±àÂë£¬°Ñdata±àÂë³É×Ö½Ú
-    key = add_16(key.encode('utf-8'))
-    iv = iv.encode('utf-8')
-    if '/' in data or '+' in data or '=' in data:  # ÎªÆÕÍ¨×Ö½Ú
-        data = base64.decodebytes(data.encode('utf-8'))
-    else:
-        data = binascii.a2b_hex(data.encode('utf-8'))  # ÎªÊ®ÁùÎ»Êý
-    aes = AES.new(key, AES.MODE_CBC, iv)
-    text = aes.decrypt(data)
-    text = re.sub(r'[\x00-\x08\x0b\x0c\x0e-\x1f\x7f-\xff]', "", text.decode('utf-8'))
-    return text
-
-
-def yinhua_jiemi(jump_url, key='57A891D97E332A9D'):
-    import requests
-    import re
-    """
-    :param url:Ó£»¨¶¯Âþ½âÎöÍøÖ·
-    :return:
-    """
-    headers = {
-        'user-agent': 'Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/102.0.0.0 Safari/537.36',
-    }
-    url = 'https://danmu.yhdmjx.com/m3u8.php?url=' + jump_url
-    resp = requests.get(url).text
-    iv = re.search('<script>var.?bt_token.?=.?"(?P<iv>.*?)";.?</script>', resp)['iv']
-    data = re.search('getVideoInfo\("(?P<data>.*?)"\)', resp)['data']
-    url = deaes_cbc(data, key, iv)
-    return url
-
-
-if __name__ == '__main__':
-    url = 'https://danmu.yhdmjx.com/m3u8.php?url=ksxUY0Bd5nJghA51z%2FAPtRkpMKTYl2cAnnQGM3ZLcqRHFyfmO2GUfBvm9fTyDDg0'
+import base64
+import urllib.parse
+from Crypto.Cipher import AES
+import re
+import base64
+import binascii
+
+
+def debase64_(data: str):
+    return base64.b64decode(data).decode('utf-8').encode().decode('unicode_escape')
+
+
+def deescape_(data: str):
+    return urllib.parse.unquote(data.replace('%u', '\\u').encode().decode('unicode-escape'))
+
+
+def deunicode_(data: str):
+    return data.encode('utf-8').decode('unicode_escape')
+
+
+def deaes_cbc(data: str, key: str, iv: str):
+    def add_16(par):  # 补位到16倍数位
+        while len(par) % 16 != 0:
+            par += b'\x00'
+        return par
+
+    # 对key进行补位 。key，iv 进行编码，把data编码成字节
+    key = add_16(key.encode('utf-8'))
+    iv = iv.encode('utf-8')
+    if '/' in data or '+' in data or '=' in data:  # 为普通字节
+        data = base64.decodebytes(data.encode('utf-8'))
+    else:
+        data = binascii.a2b_hex(data.encode('utf-8'))  # 为十六位数
+    aes = AES.new(key, AES.MODE_CBC, iv)
+    text = aes.decrypt(data)
+    text = re.sub(r'[\x00-\x08\x0b\x0c\x0e-\x1f\x7f-\xff]', "", text.decode('utf-8'))
+    return text
+
+
+def yinhua_jiemi(jump_url, key='57A891D97E332A9D'):
+    import requests
+    import re
+    """
+    :param url:樱花动漫解析网址
+    :return:
+    """
+    headers = {
+        'user-agent': 'Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/102.0.0.0 Safari/537.36',
+    }
+    url = 'https://danmu.yhdmjx.com/m3u8.php?url=' + jump_url
+    resp = requests.get(url).text
+    iv = re.search('<script>var.?bt_token.?=.?"(?P<iv>.*?)";.?</script>', resp)['iv']
+    data = re.search('getVideoInfo\("(?P<data>.*?)"\)', resp)['data']
+    url = deaes_cbc(data, key, iv)
+    return url
+
+
+if __name__ == '__main__':
+    url = 'https://danmu.yhdmjx.com/m3u8.php?url=ksxUY0Bd5nJghA51z%2FAPtRkpMKTYl2cAnnQGM3ZLcqRHFyfmO2GUfBvm9fTyDDg0'
     print(yinhua_jiemi(url))
```

#### encoding

```diff
@@ -1 +1 @@
-iso-8859-1
+utf-8
```

### Comparing `neco_f-0.0.6/src/pic_.py` & `neco_f-0.0.7/src/pic_.py`

 * *Files identical despite different names*

