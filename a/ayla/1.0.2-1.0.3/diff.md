# Comparing `tmp/ayla-1.0.2.tar.gz` & `tmp/ayla-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayla-1.0.2.tar", last modified: Thu Mar 16 05:13:12 2023, max compression
+gzip compressed data, was "ayla-1.0.3.tar", max compression
```

## Comparing `ayla-1.0.2.tar` & `ayla-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 05:13:12.539245 ayla-1.0.2/
--rw-rw-rw-   0        0        0     1067 2023-03-15 04:30:01.000000 ayla-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1123 2023-03-16 05:13:12.539245 ayla-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-03-16 02:25:08.000000 ayla-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-16 05:13:12.503003 ayla-1.0.2/ayla/
--rw-rw-rw-   0        0        0     1201 2023-03-16 05:12:39.000000 ayla-1.0.2/ayla/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:13:12.531681 ayla-1.0.2/ayla/cards/
--rw-rw-rw-   0        0        0     1126 2023-03-15 04:28:59.000000 ayla-1.0.2/ayla/cards/__init__.py
--rw-rw-rw-   0        0        0     9987 2023-03-16 05:09:41.000000 ayla-1.0.2/ayla/cards/card.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:13:12.533683 ayla-1.0.2/ayla/errors/
--rw-rw-rw-   0        0        0     1181 2023-03-16 04:31:17.000000 ayla-1.0.2/ayla/errors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:13:12.536195 ayla-1.0.2/ayla/scrobbles/
--rw-rw-rw-   0        0        0     1100 2023-03-15 04:08:47.000000 ayla-1.0.2/ayla/scrobbles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:13:12.527679 ayla-1.0.2/ayla.egg-info/
--rw-rw-rw-   0        0        0     1123 2023-03-16 05:13:12.000000 ayla-1.0.2/ayla.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-03-16 05:13:12.000000 ayla-1.0.2/ayla.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 05:13:12.000000 ayla-1.0.2/ayla.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-03-16 05:13:12.000000 ayla-1.0.2/ayla.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-16 05:13:12.000000 ayla-1.0.2/ayla.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-16 05:13:12.540243 ayla-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1087 2023-03-16 04:25:50.000000 ayla-1.0.2/setup.py
+-rwxr-xr-x   0        0        0     1201 2023-03-16 05:20:27.975394 ayla-1.0.3/Ayla/__init__.py
+-rwxr-xr-x   0        0        0     1123 2023-03-25 04:48:24.915937 ayla-1.0.3/Ayla/ayla.egg-info/PKG-INFO
+-rwxr-xr-x   0        0        0      361 2023-03-25 04:48:24.934191 ayla-1.0.3/Ayla/ayla.egg-info/SOURCES.txt
+-rwxr-xr-x   0        0        0        1 2023-03-25 04:48:24.915937 ayla-1.0.3/Ayla/ayla.egg-info/dependency_links.txt
+-rwxr-xr-x   0        0        0       14 2023-03-25 04:48:24.916937 ayla-1.0.3/Ayla/ayla.egg-info/requires.txt
+-rwxr-xr-x   0        0        0       23 2023-03-25 04:48:24.918936 ayla-1.0.3/Ayla/ayla.egg-info/top_level.txt
+-rwxr-xr-x   0        0        0     1126 2023-03-15 04:28:59.324531 ayla-1.0.3/Ayla/cards/__init__.py
+-rwxr-xr-x   0        0        0     1276 2023-03-25 04:35:22.554521 ayla-1.0.3/Ayla/cards/__pycache__/__init__.cpython-39.pyc
+-rwxr-xr-x   0        0        0     6706 2023-03-25 04:35:22.558032 ayla-1.0.3/Ayla/cards/__pycache__/card.cpython-39.pyc
+-rwxr-xr-x   0        0        0        0 2023-03-20 03:46:26.405743 ayla-1.0.3/Ayla/cards/assets/__init__.py
+-rwxr-xr-x   0        0        0      842 2023-01-24 08:46:18.000000 ayla-1.0.3/Ayla/cards/assets/curveborder.png
+-rwxr-xr-x   0        0        0     2710 2023-02-18 02:17:04.000000 ayla-1.0.3/Ayla/cards/assets/curvedoverlay.png
+-rwxr-xr-x   0        0        0        0 2023-03-20 03:46:34.392685 ayla-1.0.3/Ayla/cards/assets/fonts/__init__.py
+-rwxr-xr-x   0        0        0    66976 2019-11-25 21:12:12.000000 ayla-1.0.3/Ayla/cards/assets/fonts/juice.otf
+-rwxr-xr-x   0        0        0    60288 2023-01-24 08:46:18.000000 ayla-1.0.3/Ayla/cards/assets/fonts/levelfont.otf
+-rwxr-xr-x   0        0        0   141612 2022-09-22 02:39:26.000000 ayla-1.0.3/Ayla/cards/assets/fonts/poppins.ttf
+-rwxr-xr-x   0        0        0    26156 2012-09-26 21:36:18.000000 ayla-1.0.3/Ayla/cards/assets/fonts/rabbit.ttf
+-rwxr-xr-x   0        0        0     9742 2023-01-24 08:46:18.000000 ayla-1.0.3/Ayla/cards/assets/mask_circle.jpg
+-rwxr-xr-x   0        0        0     6394 2023-01-24 08:46:18.000000 ayla-1.0.3/Ayla/cards/assets/overlay1.png
+-rwxr-xr-x   0        0        0     1339 2023-02-12 14:41:14.000000 ayla-1.0.3/Ayla/cards/assets/pic.png
+-rwxr-xr-x   0        0        0      318 2023-02-17 05:28:00.000000 ayla-1.0.3/Ayla/cards/assets/transparent_mask.png
+-rwxr-xr-x   0        0        0     9987 2023-03-16 05:09:41.540526 ayla-1.0.3/Ayla/cards/card.py
+-rwxr-xr-x   0        0        0     1181 2023-03-16 04:31:17.158782 ayla-1.0.3/Ayla/errors/__init__.py
+-rwxr-xr-x   0        0        0     1453 2023-03-25 04:35:22.566041 ayla-1.0.3/Ayla/errors/__pycache__/__init__.cpython-39.pyc
+-rwxr-xr-x   0        0        0     1100 2023-03-15 04:08:47.084140 ayla-1.0.3/Ayla/scrobbles/__init__.py
+-rwxr-xr-x   0        0        0     1067 2023-03-15 04:30:01.510284 ayla-1.0.3/LICENSE
+-rwxr-xr-x   0        0        0      303 2023-03-16 02:25:08.662548 ayla-1.0.3/README.md
+-rw-r--r--   0        0        0      588 2023-08-06 23:13:39.688187 ayla-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 ayla-1.0.3/PKG-INFO
```

### Comparing `ayla-1.0.2/LICENSE` & `ayla-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ayla-1.0.2/PKG-INFO` & `ayla-1.0.3/Ayla/ayla.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayla
-Version: 1.0.2
+Version: 1.0.3
 Summary: Some functions used in KuuhakuTeam projects
 Home-page: https://github.com/KuuhakuTeam/Ayla
 Author: fnixdev
 Author-email: luisgatn000@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ayla-1.0.2/ayla/__init__.py` & `ayla-1.0.3/Ayla/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,13 +17,13 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 __author__ = "fnixdev"
 __copyright__ = "Copyright 2023-present fnixdev"
 
 
 from .cards import RankCard
```

### Comparing `ayla-1.0.2/ayla/cards/__init__.py` & `ayla-1.0.3/Ayla/cards/__init__.py`

 * *Files identical despite different names*

### Comparing `ayla-1.0.2/ayla/cards/card.py` & `ayla-1.0.3/Ayla/cards/card.py`

 * *Files identical despite different names*

### Comparing `ayla-1.0.2/ayla/errors/__init__.py` & `ayla-1.0.3/Ayla/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `ayla-1.0.2/ayla/scrobbles/__init__.py` & `ayla-1.0.3/Ayla/scrobbles/__init__.py`

 * *Files identical despite different names*

