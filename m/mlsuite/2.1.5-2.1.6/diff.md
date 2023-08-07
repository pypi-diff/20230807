# Comparing `tmp/mlsuite-2.1.5.tar.gz` & `tmp/mlsuite-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlsuite-2.1.5.tar", last modified: Mon Jun 12 06:44:47 2023, max compression
+gzip compressed data, was "mlsuite-2.1.6.tar", last modified: Mon Aug  7 09:17:00 2023, max compression
```

## Comparing `mlsuite-2.1.5.tar` & `mlsuite-2.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)        0 2023-06-12 06:44:47.309284 mlsuite-2.1.5/
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)     1067 2022-08-30 02:42:20.000000 mlsuite-2.1.5/LICENSE
-drwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)        0 2023-06-12 06:44:47.292789 mlsuite-2.1.5/MLsuite/
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     8860 2023-06-12 05:35:05.000000 mlsuite-2.1.5/MLsuite/MLArguments.py
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)    26629 2023-04-28 08:19:34.000000 mlsuite-2.1.5/MLsuite/MLEstimators.py
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     1931 2022-07-07 10:04:52.000000 mlsuite-2.1.5/MLsuite/MLLogging.py
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     2197 2023-04-07 02:10:21.000000 mlsuite-2.1.5/MLsuite/MLOpenWrite.py
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)      836 2022-09-06 09:45:06.000000 mlsuite-2.1.5/MLsuite/MLPipeline.py
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     4450 2023-06-12 03:50:49.000000 mlsuite-2.1.5/MLsuite/MLPredicting.py
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)    28223 2023-06-12 06:43:29.000000 mlsuite-2.1.5/MLsuite/MLSupervising.py
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     3424 2022-07-07 10:04:52.000000 mlsuite-2.1.5/MLsuite/MLUtilities.py
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)       17 2022-09-06 06:29:23.000000 mlsuite-2.1.5/MLsuite/__init__.py
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     2118 2022-12-14 01:57:48.000000 mlsuite-2.1.5/MLsuite/main.py
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)     1285 2023-06-12 06:44:47.307899 mlsuite-2.1.5/PKG-INFO
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)     3762 2023-06-12 06:43:42.000000 mlsuite-2.1.5/README.md
-drwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)        0 2023-06-12 06:44:47.305323 mlsuite-2.1.5/mlsuite.egg-info/
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)     1285 2023-06-12 06:44:47.000000 mlsuite-2.1.5/mlsuite.egg-info/PKG-INFO
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)      414 2023-06-12 06:44:47.000000 mlsuite-2.1.5/mlsuite.egg-info/SOURCES.txt
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)        1 2023-06-12 06:44:47.000000 mlsuite-2.1.5/mlsuite.egg-info/dependency_links.txt
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)      115 2023-06-12 06:44:47.000000 mlsuite-2.1.5/mlsuite.egg-info/requires.txt
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)        8 2023-06-12 06:44:47.000000 mlsuite-2.1.5/mlsuite.egg-info/top_level.txt
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)      455 2022-09-06 10:51:20.000000 mlsuite-2.1.5/mlsuite.py
--rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)       38 2023-06-12 06:44:47.309947 mlsuite-2.1.5/setup.cfg
--rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     1823 2023-06-12 05:36:57.000000 mlsuite-2.1.5/setup.py
+drwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)        0 2023-08-07 09:17:00.055357 mlsuite-2.1.6/
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)     1067 2022-08-30 02:42:20.000000 mlsuite-2.1.6/LICENSE
+drwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)        0 2023-08-07 09:17:00.042848 mlsuite-2.1.6/MLsuite/
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     9233 2023-08-07 07:36:40.000000 mlsuite-2.1.6/MLsuite/MLArguments.py
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)    26547 2023-08-07 07:00:22.000000 mlsuite-2.1.6/MLsuite/MLEstimators.py
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     1931 2022-07-07 10:04:52.000000 mlsuite-2.1.6/MLsuite/MLLogging.py
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     2197 2023-04-07 02:10:21.000000 mlsuite-2.1.6/MLsuite/MLOpenWrite.py
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)      836 2022-09-06 09:45:06.000000 mlsuite-2.1.6/MLsuite/MLPipeline.py
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     4450 2023-06-12 03:50:49.000000 mlsuite-2.1.6/MLsuite/MLPredicting.py
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)    31556 2023-08-07 08:27:50.000000 mlsuite-2.1.6/MLsuite/MLSupervising.py
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     3424 2023-08-07 08:12:51.000000 mlsuite-2.1.6/MLsuite/MLUtilities.py
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)       17 2022-09-06 06:29:23.000000 mlsuite-2.1.6/MLsuite/__init__.py
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     2118 2022-12-14 01:57:48.000000 mlsuite-2.1.6/MLsuite/main.py
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)     1285 2023-08-07 09:17:00.053738 mlsuite-2.1.6/PKG-INFO
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)     4055 2023-08-07 09:11:17.000000 mlsuite-2.1.6/README.md
+drwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)        0 2023-08-07 09:17:00.051317 mlsuite-2.1.6/mlsuite.egg-info/
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)     1285 2023-08-07 09:16:59.000000 mlsuite-2.1.6/mlsuite.egg-info/PKG-INFO
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)      414 2023-08-07 09:16:59.000000 mlsuite-2.1.6/mlsuite.egg-info/SOURCES.txt
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)        1 2023-08-07 09:16:59.000000 mlsuite-2.1.6/mlsuite.egg-info/dependency_links.txt
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)      115 2023-08-07 09:16:59.000000 mlsuite-2.1.6/mlsuite.egg-info/requires.txt
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)        8 2023-08-07 09:16:59.000000 mlsuite-2.1.6/mlsuite.egg-info/top_level.txt
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)      455 2022-09-06 10:51:20.000000 mlsuite-2.1.6/mlsuite.py
+-rw-r--r--   0 li.suxing (31799) basic_bioinfo  (2003)       38 2023-08-07 09:17:00.055807 mlsuite-2.1.6/setup.cfg
+-rwxr-xr-x   0 li.suxing (31799) basic_bioinfo  (2003)     1823 2023-08-07 09:13:55.000000 mlsuite-2.1.6/setup.py
```

### Comparing `mlsuite-2.1.5/LICENSE` & `mlsuite-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mlsuite-2.1.5/MLsuite/MLArguments.py` & `mlsuite-2.1.6/MLsuite/MLArguments.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 2. python mlsuite.py Auto    -i data.traintest.txt -g group.new.txt -p data.predict.txt -o testdt/ -m DT -pn 0.9 -f (10 times sample grouping and 10 models)
 3. python mlsuite.py Auto    -i data.traintest.txt -g group.new.txt -o testdt/ -m DT -pn 0.9
 4. python mlsuite.py Fitting -i data.traintest.txt -g group.new.txt -o testdt/ -m DT -pn 0.9
 5. python mlsuite.py Fitting -i data.traintest.txt -g group.new.txt -o testdt/ -m DT -pn 0.9 -f (10 times sample grouping and 10 models)
 6. python mlsuite.py Predict -p data.predict.txt   -g group.new.txt -x modelpath/ -y predictdt/ -m DT -pn 0.9.''')
 
     parser.add_argument('-V','--version',action ='version',
-                version='mlsuite version 2.1.5')
+                version='mlsuite version 2.1.6')
     subparsers = parser.add_subparsers(dest="commands",
                     help='machine learning models help.')
     ### Fitting module
     P_fitting  = subparsers.add_parser('Fitting',conflict_handler='resolve', add_help=False)
     P_fitting.add_argument("-f", "--fit_10", action="store_true", default=False,
                     help='''fitting modeling by 10 times sample spliting''')
     P_fitting.add_argument("-i", "--input",type=str,
@@ -83,14 +83,18 @@
 **LPO..................LeavePOut()
 **LOU..................LeaveOneOut()
 ''')
     P_fitting.add_argument("-pn", "--pc_number", type=float, default=0,
                     help='''select PC numbers, default is 0 that means not to do PCA analysis, >1 means selecting PC numbers,
                             >0 and <1 means select the number of components such that the amount of variance that needs to be
                             explained is greater than the percentage specified by pc_number.''')
+    P_fitting.add_argument("-pc", "--pc_center", action="store_false",
+                    help='''PCA input data center, default is not open. If open, parameter "pc_number" is not 0.''')
+    P_fitting.add_argument("-ps", "--pc_scale", action="store_true",
+                    help='''PCA input data scale, default is not open. If open, parameter "pc_number" is not 0.''')
     P_fitting.add_argument("-am", "--Addmode", type=str, default='LinearSVM',
                     help='''use additional model to adjust modeling in RF, GBDT and XGB estimators. N means no addition.''')
     P_fitting.add_argument("-rd", "--random",type=int, default=123456,
                     help="the random seeds for cross validation when using StratifiedShuffleSplit.")
     P_fitting.add_argument("-tz", "--testS",type=float, default=0.3,
                     help="the test size for cross validation when using StratifiedShuffleSplit.")
     P_fitting.add_argument("-sc", "--SearchCV",type=str, nargs='?', default='GSCV', choices=['GSCV','RSCV',],
```

### Comparing `mlsuite-2.1.5/MLsuite/MLEstimators.py` & `mlsuite-2.1.6/MLsuite/MLEstimators.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,26 +195,26 @@
                             'C': np.power(10, np.linspace(-2, 2, 10)),
                            }],
                 'RSCV'  : {}
                 }},
         'SVMrbf'        : {
             'estimator' : SVC(kernel='rbf',  probability=True, decision_function_shape='ovr', random_state=123456),
             'parameters': {
-                'GSCV'  : { 'gamma': [1e1, 1e0, 1e-1, 1e-2, 1e-3, 1e-4, 1e-5, 'scale'],
-                            'tol': [ 1e-7, 1e-6, 1e-5, 1e-4, 1e-3, 1e-2, 1e-1 ],
-                            'C': np.power(10, np.linspace(-2, 2, 10)),
+                'GSCV'  : { 'gamma': [1e0, 1e-1, 1e-2, 1e-3, 'scale'],
+                            'tol': [ 1e-4, 1e-3, 1e-2 ],
+                            'C': np.power(10, np.linspace(-2, 0, 10)),
                           },
                 'RSCV'  : {}
                 }},
         'SVMpoly'        : {
             'estimator' : SVC(kernel='poly',  probability=True, decision_function_shape='ovr', random_state=123456),
             'parameters': {
-                'GSCV'  : { 'gamma': [1e1, 1e0, 1e-1, 1e-2, 1e-3, 1e-4, 1e-5, 'scale'],
-                            'tol': [ 1e-7, 1e-6, 1e-5, 1e-4, 1e-3, 1e-2, 1e-1 ],
-                            'C': np.power(10, np.linspace(-2, 2, 10)),
+                'GSCV'  : { 'gamma': [1e0, 1e-1, 1e-2, 1e-3, 'scale'],
+                            'tol': [ 1e-4, 1e-3, 1e-2 ],
+                            'C': np.power(10, np.linspace(-2, 0, 10)),
                           },
                 'RSCV'  : {}
                 }},
         'RVMrbf'        : {
             'estimator' : RVC(kernel='rbf', n_iter=1000, threshold_alpha=1e9),
             'parameters': {
                 'GSCV'  : { 'tol': [ 1e-5, 1e-4, 1e-3, 1e-2, 1e-1 ],
```

### Comparing `mlsuite-2.1.5/MLsuite/MLLogging.py` & `mlsuite-2.1.6/MLsuite/MLLogging.py`

 * *Files identical despite different names*

### Comparing `mlsuite-2.1.5/MLsuite/MLOpenWrite.py` & `mlsuite-2.1.6/MLsuite/MLOpenWrite.py`

 * *Files identical despite different names*

### Comparing `mlsuite-2.1.5/MLsuite/MLPipeline.py` & `mlsuite-2.1.6/MLsuite/MLPipeline.py`

 * *Files identical despite different names*

### Comparing `mlsuite-2.1.5/MLsuite/MLPredicting.py` & `mlsuite-2.1.6/MLsuite/MLPredicting.py`

 * *Files identical despite different names*

### Comparing `mlsuite-2.1.5/MLsuite/MLSupervising.py` & `mlsuite-2.1.6/MLsuite/MLSupervising.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,29 +12,143 @@
 
 from .MLUtilities import MyThread, _predict_proba_lr, CrossvalidationSplit, Check_Label, Check_Binar
 from .MLEstimators import ML
 from .MLOpenWrite import OpenM, Openf
 from sklearn.model_selection import GridSearchCV, RandomizedSearchCV
 from sklearn.metrics import (accuracy_score, f1_score, recall_score, precision_score,
                              balanced_accuracy_score, roc_auc_score, average_precision_score)
-from sklearn.decomposition import PCA
 from sklearn.preprocessing import OneHotEncoder
 from sklearn.calibration import CalibratedClassifierCV
 from scipy.sparse import vstack
 import os
 import numpy as np
 import pandas as pd
 import re
 import time
 import joblib
 pd.set_option('display.max_rows', 100000)
 pd.set_option('display.max_columns', 100000)
 pd.set_option('display.width', 100000)
 
 
+class pca_svd():
+    def __init__(self, k):
+        self.k = k
+
+    def fit(self, x, center=True, scale=False):
+        '''
+        x: pca降维初始数据， np.arary数组，行表示样本，列表示特征
+        '''
+        self.x = np.asarray(x)
+        self.x_mean = self.x.mean(axis = 0)
+        self.x_std = self.x.std(axis = 0)
+
+        # center
+        if center == True:
+            x_center = self.x - self.x_mean
+        else:
+            x_center = self.x
+        
+        # scale
+        if scale == True:
+            x_zscore = x_center/self.x_std
+        else:
+            x_zscore = x_center
+        
+        # data matrix
+        data_mat = x_zscore
+
+        # svd
+        U, vals, V = np.linalg.svd(data_mat)
+        vals = np.square(vals)
+        vecs = V.T
+        self.eig_vals = np.round(vals/np.sum(vals), 4)
+        self.eig_vecs = vecs
+
+        # 根据k，判定输出维度out_k
+        if self.k >=1:
+            self.out_k = self.k
+        elif self.k > 0 and self.k < 1:
+            pc_explain = self.eig_vals.cumsum()
+            cumratio_bool = pc_explain >= self.k
+            tmp = np.where(cumratio_bool == True)[0][0] + 1
+            self.out_k = tmp
+ 
+
+    def fit_transform(self, x, center=True, scale=False):
+        '''
+        x: pca降维初始数据， np.arary数组，行表示样本，列表示特征
+        '''
+        self.x = np.asarray(x)
+        self.x_mean = self.x.mean(axis = 0)
+        self.x_std = self.x.std(axis = 0)
+
+        # center
+        if center == True:
+            x_center = x - self.x_mean
+        else:
+            x_center = x
+        
+        # scale
+        if scale == True:
+            x_zscore = x_center/self.x_std
+        else:
+            x_zscore = x_center
+        
+        # cov matrix
+        data_mat = x_zscore
+
+        # svd
+        U, vals, V = np.linalg.svd(data_mat)
+        vals = np.square(vals)
+        vecs = V.T
+        self.eig_vals = np.round(vals/np.sum(vals), 4)
+        self.eig_vecs = vecs
+
+        # 根据k，判定输出维度out_k
+        if self.k >=1:
+            self.out_k = self.k
+        elif self.k > 0 and self.k < 1:
+            pc_explain = self.eig_vals.cumsum()
+            cumratio_bool = pc_explain >= self.k
+            tmp = np.where(cumratio_bool == True)[0][0] + 1
+            self.out_k = tmp
+
+        # 在新维度上的结果
+        new_x = np.matmul(x_zscore, self.eig_vecs)
+        self.new_x = new_x
+
+        return(new_x[:, 0:self.out_k])
+
+
+    def transform(self, y, center=True, scale=False):
+        '''
+        y: pca降维验证数据， np.arary数组，行表示样本，列表示特征
+        '''
+        y = np.asarray(y)
+
+        # center
+        if center == True:
+            y_center = y - self.x_mean
+        else:
+            y_center = y
+        
+        # scale
+        if scale == True:
+            y_zscore = y_center/self.x_std
+        else:
+            y_zscore = y_center
+
+        # 在新维度上的结果
+        new_y = np.matmul(y_zscore, self.eig_vecs)
+        self.new_y = new_y
+
+        return(new_y[:, 0:self.out_k])
+
+
 # obj: data grouping (default is 13 sets of data)
 class sampleSplit:
     def __init__(self, arg):
         self.arg = arg
     def CVSplit(self, Xdf, Ydf):
         all_test = []
         all_split = []
@@ -303,15 +417,15 @@
             y_pred = [Y_TRUE]
             for _i, _m in enumerate(_cv):
                 model = _m['model']
                 clf = _m['clf']
                 model_x_names = _m['features']
                 if 'pca_clf' in _m:
                     pca_clf = _m['pca_clf']
-                    tmp = pd.DataFrame(pca_clf.transform(pDFall[xa]), index=pDFall.index)
+                    tmp = pd.DataFrame(pca_clf.transform(pDFall[xa], center=self.arg.pc_center, scale=self.arg.pc_scale), index=pDFall.index)
                     tmp.columns = ["PC"+str(j) for j in range(1, tmp.shape[1]+1)]
                     x_pred = tmp[model_x_names]
                 else:
                     x_pred = pDFall[model_x_names]
                 if 'leaf' in _m.keys():
                     leaf = _m['leaf']
                     x_pred, OHE = HyperparamOptimal.OneHot(self.model, _cv[0]['clf'], x_pred, leaf)
@@ -478,17 +592,20 @@
                 x_train, y_train = train[Xi], train[Yi]
                 x_test , y_test  = test[Xi], test[Yi]
                 if args.pc_number != 0:
                     if args.pc_number >= 1:
                         pc_number = int(args.pc_number)
                     else:
                         pc_number = args.pc_number
-                    pca_clf = PCA(n_components=pc_number).fit(x_train)
-                    x_train = pd.DataFrame(pca_clf.transform(x_train), index=x_train.index)
-                    x_test = pd.DataFrame(pca_clf.transform(x_test), index=x_test.index)
+                    print(pc_number)
+                    pca_clf = pca_svd(k=pc_number)
+                    pca_clf.fit(x_train, center=args.pc_center, scale=args.pc_scale)
+                    print(pca_clf.out_k)
+                    x_train = pd.DataFrame(pca_clf.transform(x_train, center=args.pc_center, scale=args.pc_scale), index=x_train.index)
+                    x_test = pd.DataFrame(pca_clf.transform(x_test, center=args.pc_center, scale=args.pc_scale), index=x_test.index)
                     x_train.columns = ["PC"+str(j) for j in range(1, x_train.shape[1]+1)]
                     x_test.columns = ["PC"+str(j) for j in range(1, x_test.shape[1]+1)]
             #    t = MyThread(modeling, (args, x_train, x_test, y_train, y_test, Typi, DFall[Yi].nunique(), repeat, i, len(sample_group_index)))
             #    threads.append(t)
             #for i in range(len(sample_group_index)):
             #    threads[i].setDaemon(True)
             #    threads[i].start()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mlsuite-2.1.5/MLsuite/MLUtilities.py` & `mlsuite-2.1.6/MLsuite/MLUtilities.py`

 * *Files identical despite different names*

### Comparing `mlsuite-2.1.5/MLsuite/main.py` & `mlsuite-2.1.6/MLsuite/main.py`

 * *Files identical despite different names*

### Comparing `mlsuite-2.1.5/PKG-INFO` & `mlsuite-2.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlsuite
-Version: 2.1.5
+Version: 2.1.6
 Summary: The traditional machine learning analysis based on sklearn package
 Home-page: https://git.genecast.com.cn/narwhal/mlsuite
 Author: suxing li
 Author-email: li.suxing@genecast.com.cn
 Maintainer: suxing li
 Maintainer-email: li.suxing@genecast.com.cn
 Platform: all
```

### Comparing `mlsuite-2.1.5/README.md` & `mlsuite-2.1.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # mlsuite
 
 ## Install
 
 ```
-pip install mlsuite==2.1.5
+pip install mlsuite==2.1.6
 pip install https://github.com/JamesRitchie/scikit-rvm/archive/master.zip
 ```
 
 ## Usage
 
 Notice: used pyhton3, not python2
 
@@ -32,14 +32,18 @@
 2. python mlsuite.py Auto    -i data.traintest.txt -g group.new.txt -p data.predict.txt -o testdt/ -m DT -pn 0.9 -f (10 times sample grouping and 10 models)
 3. python mlsuite.py Auto    -i data.traintest.txt -g group.new.txt -o testdt/ -m DT -pn 0.9
 4. python mlsuite.py Fitting -i data.traintest.txt -g group.new.txt -o testdt/ -m DT -pn 0.9
 5. python mlsuite.py Fitting -i data.traintest.txt -g group.new.txt -o testdt/ -m DT -pn 0.9 -f (10 times sample grouping and 10 models)
 6. python mlsuite.py Predict -p data.predict.txt   -g group.new.txt -x modelpath/ -y predictdt/ -m DT -pn 0.9.
 
 ## Update log
+### v2.1.6
+1. Remove sklearn PCA modula, PCA analysis by self-written script in SVD method
+2. "Fitting" module has been added "-pc|--pc_center" and "-ps|--pc__scale" arguments, indicate data should to be center or scale before PCA analysis. default data center is open, data scale is closed.
+
 ### v2.1.5
 1. "Fitting" module has been added "-pn|--pc_number" arguments, which the spliting training data was reduced dimensions by PCA, and assign the number of PCs (integer, [1,Inf)) or the cumulative contribution ratio (float, (0, 1)).
 
 ### v2.1.4
 1. "Fitting" module has been added "-f|--fit_10" arguments, which the input training dataset was splited into 10 train/test groups, and got 10 models.
 
 ### v2.1.3
```

### Comparing `mlsuite-2.1.5/mlsuite.egg-info/PKG-INFO` & `mlsuite-2.1.6/mlsuite.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlsuite
-Version: 2.1.5
+Version: 2.1.6
 Summary: The traditional machine learning analysis based on sklearn package
 Home-page: https://git.genecast.com.cn/narwhal/mlsuite
 Author: suxing li
 Author-email: li.suxing@genecast.com.cn
 Maintainer: suxing li
 Maintainer-email: li.suxing@genecast.com.cn
 Platform: all
```

### Comparing `mlsuite-2.1.5/setup.py` & `mlsuite-2.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages, setup
 from glob import glob
 from os.path import dirname, join
 import os
 
 setup(
     name='mlsuite',
-    version='2.1.5',
+    version='2.1.6',
     description='The traditional machine learning analysis based on sklearn package',
     author='suxing li',
     author_email='li.suxing@genecast.com.cn',
     maintainer='suxing li',
     maintainer_email='li.suxing@genecast.com.cn',
     packages=find_packages(where='.', exclude=(), include=('*',)),
     include_package_data=True,
```

