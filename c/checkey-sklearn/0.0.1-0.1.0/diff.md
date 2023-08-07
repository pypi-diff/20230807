# Comparing `tmp/checkey-sklearn-0.0.1.tar.gz` & `tmp/checkey-sklearn-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkey-sklearn-0.0.1.tar", last modified: Mon Aug  7 04:35:38 2023, max compression
+gzip compressed data, was "checkey-sklearn-0.1.0.tar", last modified: Mon Aug  7 04:51:50 2023, max compression
```

## Comparing `checkey-sklearn-0.0.1.tar` & `checkey-sklearn-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 04:35:38.056368 checkey-sklearn-0.0.1/
--rw-rw-rw-   0        0        0    34523 2023-08-07 03:09:58.000000 checkey-sklearn-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1789 2023-08-07 04:35:38.057536 checkey-sklearn-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-07 04:35:38.049364 checkey-sklearn-0.0.1/checkey-sklearn/
--rw-rw-rw-   0        0        0       59 2023-08-07 04:35:07.000000 checkey-sklearn-0.0.1/checkey-sklearn/__init__.py
--rw-rw-rw-   0        0        0    14587 2023-08-07 04:35:07.000000 checkey-sklearn-0.0.1/checkey-sklearn/improving_naive_bayes.py
--rw-rw-rw-   0        0        0     2843 2023-08-07 04:35:07.000000 checkey-sklearn-0.0.1/checkey-sklearn/topsis.py
-drwxrwxrwx   0        0        0        0 2023-08-07 04:35:38.055364 checkey-sklearn-0.0.1/checkey_sklearn.egg-info/
--rw-rw-rw-   0        0        0     1789 2023-08-07 04:35:37.000000 checkey-sklearn-0.0.1/checkey_sklearn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2023-08-07 04:35:37.000000 checkey-sklearn-0.0.1/checkey_sklearn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 04:35:37.000000 checkey-sklearn-0.0.1/checkey_sklearn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-08-07 04:35:37.000000 checkey-sklearn-0.0.1/checkey_sklearn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-08-07 04:35:37.000000 checkey-sklearn-0.0.1/checkey_sklearn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 04:35:38.057536 checkey-sklearn-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2054 2023-08-07 04:35:29.000000 checkey-sklearn-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 04:51:50.505072 checkey-sklearn-0.1.0/
+-rw-rw-rw-   0        0        0    34523 2023-08-07 03:09:58.000000 checkey-sklearn-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1781 2023-08-07 04:51:50.505072 checkey-sklearn-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-07 04:51:50.500042 checkey-sklearn-0.1.0/checkey_sklearn.egg-info/
+-rw-rw-rw-   0        0        0     1781 2023-08-07 04:51:50.000000 checkey-sklearn-0.1.0/checkey_sklearn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-08-07 04:51:50.000000 checkey-sklearn-0.1.0/checkey_sklearn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 04:51:50.000000 checkey-sklearn-0.1.0/checkey_sklearn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-08-07 04:51:50.000000 checkey-sklearn-0.1.0/checkey_sklearn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-07 04:51:50.000000 checkey-sklearn-0.1.0/checkey_sklearn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 04:51:50.504069 checkey-sklearn-0.1.0/chlearn/
+-rw-rw-rw-   0        0        0       59 2023-08-07 04:35:07.000000 checkey-sklearn-0.1.0/chlearn/__init__.py
+-rw-rw-rw-   0        0        0    14587 2023-08-07 04:35:07.000000 checkey-sklearn-0.1.0/chlearn/improving_naive_bayes.py
+-rw-rw-rw-   0        0        0     2843 2023-08-07 04:35:07.000000 checkey-sklearn-0.1.0/chlearn/topsis.py
+-rw-rw-rw-   0        0        0       42 2023-08-07 04:51:50.506075 checkey-sklearn-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2046 2023-08-07 04:51:46.000000 checkey-sklearn-0.1.0/setup.py
```

### Comparing `checkey-sklearn-0.0.1/LICENSE.txt` & `checkey-sklearn-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `checkey-sklearn-0.0.1/PKG-INFO` & `checkey-sklearn-0.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkey-sklearn
-Version: 0.0.1
+Version: 0.1.0
 Summary: 自己平时会使用的一些统计学和数学模型,目前有两个改进的朴素贝叶斯算法和一个TOPSIS
 Author: Checkey01
 Author-email: Chiaki2048@outlook.com
 Keywords: Machine Learning,Python
 License-File: LICENSE.txt
 
 
@@ -31,15 +31,15 @@
     GNU Affero General Public License for more details.
 
     You should have received a copy of the GNU Affero General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 ## 安装方法
 ```commandline
-pip install checkey-sklearn
+pip install chlearn
 ```
 
 ## 依赖的第三方模块包
 
 ```
 numpy
 pandas
```

### Comparing `checkey-sklearn-0.0.1/checkey-sklearn/improving_naive_bayes.py` & `checkey-sklearn-0.1.0/chlearn/improving_naive_bayes.py`

 * *Files identical despite different names*

### Comparing `checkey-sklearn-0.0.1/checkey-sklearn/topsis.py` & `checkey-sklearn-0.1.0/chlearn/topsis.py`

 * *Files identical despite different names*

### Comparing `checkey-sklearn-0.0.1/checkey_sklearn.egg-info/PKG-INFO` & `checkey-sklearn-0.1.0/checkey_sklearn.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkey-sklearn
-Version: 0.0.1
+Version: 0.1.0
 Summary: 自己平时会使用的一些统计学和数学模型,目前有两个改进的朴素贝叶斯算法和一个TOPSIS
 Author: Checkey01
 Author-email: Chiaki2048@outlook.com
 Keywords: Machine Learning,Python
 License-File: LICENSE.txt
 
 
@@ -31,15 +31,15 @@
     GNU Affero General Public License for more details.
 
     You should have received a copy of the GNU Affero General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 ## 安装方法
 ```commandline
-pip install checkey-sklearn
+pip install chlearn
 ```
 
 ## 依赖的第三方模块包
 
 ```
 numpy
 pandas
```

### Comparing `checkey-sklearn-0.0.1/setup.py` & `checkey-sklearn-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.1.0'
 DESCRIPTION = """
 自己平时会使用的一些统计学和数学模型,目前有两个改进的朴素贝叶斯算法和一个TOPSIS
 """
 LONG_DESCRIPTION = """
 # 使用说明
 
 自己平时会使用的一些统计学和数学模型,目前有两个改进的朴素贝叶斯算法和一个TOPSIS
@@ -28,15 +28,15 @@
     GNU Affero General Public License for more details.
 
     You should have received a copy of the GNU Affero General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 ## 安装方法
 ```commandline
-pip install checkey-sklearn
+pip install chlearn
 ```
 
 ## 依赖的第三方模块包
 
 ```
 numpy
 pandas
```

