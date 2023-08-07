# Comparing `tmp/lognflow-0.8.4.tar.gz` & `tmp/lognflow-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lognflow-0.8.4.tar", last modified: Wed Aug  2 23:05:52 2023, max compression
+gzip compressed data, was "lognflow-0.8.5.tar", last modified: Mon Aug  7 02:43:35 2023, max compression
```

## Comparing `lognflow-0.8.4.tar` & `lognflow-0.8.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:05:52.218510 lognflow-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-02 23:05:41.000000 lognflow-0.8.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-08-02 23:05:41.000000 lognflow-0.8.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-08-02 23:05:41.000000 lognflow-0.8.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-08-02 23:05:41.000000 lognflow-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-02 23:05:41.000000 lognflow-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-08-02 23:05:52.218510 lognflow-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-08-02 23:05:41.000000 lognflow-0.8.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:05:52.214510 lognflow-0.8.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-02 23:05:41.000000 lognflow-0.8.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 23:05:41.000000 lognflow-0.8.4/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-08-02 23:05:41.000000 lognflow-0.8.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 23:05:41.000000 lognflow-0.8.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 23:05:41.000000 lognflow-0.8.4/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-02 23:05:41.000000 lognflow-0.8.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-02 23:05:41.000000 lognflow-0.8.4/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-02 23:05:41.000000 lognflow-0.8.4/docs/lognflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-02 23:05:41.000000 lognflow-0.8.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 23:05:41.000000 lognflow-0.8.4/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-02 23:05:41.000000 lognflow-0.8.4/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:05:52.218510 lognflow-0.8.4/lognflow/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-02 23:05:41.000000 lognflow-0.8.4/lognflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64809 2023-08-02 23:05:41.000000 lognflow-0.8.4/lognflow/lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    13975 2023-08-02 23:05:41.000000 lognflow-0.8.4/lognflow/logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-08-02 23:05:41.000000 lognflow-0.8.4/lognflow/printprogress.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-08-02 23:05:41.000000 lognflow-0.8.4/lognflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:05:52.218510 lognflow-0.8.4/lognflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-08-02 23:05:52.000000 lognflow-0.8.4/lognflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-02 23:05:52.000000 lognflow-0.8.4/lognflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 23:05:52.000000 lognflow-0.8.4/lognflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 23:05:52.000000 lognflow-0.8.4/lognflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 23:05:52.000000 lognflow-0.8.4/lognflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 23:05:52.000000 lognflow-0.8.4/lognflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-02 23:05:52.218510 lognflow-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-02 23:05:41.000000 lognflow-0.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 23:05:52.218510 lognflow-0.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 23:05:41.000000 lognflow-0.8.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-08-02 23:05:41.000000 lognflow-0.8.4/tests/test_lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-08-02 23:05:41.000000 lognflow-0.8.4/tests/test_logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-08-02 23:05:41.000000 lognflow-0.8.4/tests/test_printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:43:35.186465 lognflow-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-07 02:43:25.000000 lognflow-0.8.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-08-07 02:43:25.000000 lognflow-0.8.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-08-07 02:43:25.000000 lognflow-0.8.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-08-07 02:43:25.000000 lognflow-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-07 02:43:25.000000 lognflow-0.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-08-07 02:43:35.186465 lognflow-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-08-07 02:43:25.000000 lognflow-0.8.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:43:35.186465 lognflow-0.8.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-07 02:43:25.000000 lognflow-0.8.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-07 02:43:25.000000 lognflow-0.8.5/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-08-07 02:43:25.000000 lognflow-0.8.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-07 02:43:25.000000 lognflow-0.8.5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-07 02:43:25.000000 lognflow-0.8.5/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-07 02:43:25.000000 lognflow-0.8.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-07 02:43:25.000000 lognflow-0.8.5/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-07 02:43:25.000000 lognflow-0.8.5/docs/lognflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-07 02:43:25.000000 lognflow-0.8.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-07 02:43:25.000000 lognflow-0.8.5/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-07 02:43:25.000000 lognflow-0.8.5/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:43:35.186465 lognflow-0.8.5/lognflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-07 02:43:25.000000 lognflow-0.8.5/lognflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63998 2023-08-07 02:43:25.000000 lognflow-0.8.5/lognflow/lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13975 2023-08-07 02:43:25.000000 lognflow-0.8.5/lognflow/logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-08-07 02:43:25.000000 lognflow-0.8.5/lognflow/printprogress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-08-07 02:43:25.000000 lognflow-0.8.5/lognflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:43:35.186465 lognflow-0.8.5/lognflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-08-07 02:43:35.000000 lognflow-0.8.5/lognflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-07 02:43:35.000000 lognflow-0.8.5/lognflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 02:43:35.000000 lognflow-0.8.5/lognflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 02:43:35.000000 lognflow-0.8.5/lognflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-07 02:43:35.000000 lognflow-0.8.5/lognflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-07 02:43:35.000000 lognflow-0.8.5/lognflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-07 02:43:35.186465 lognflow-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-07 02:43:25.000000 lognflow-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 02:43:35.186465 lognflow-0.8.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-07 02:43:25.000000 lognflow-0.8.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-08-07 02:43:25.000000 lognflow-0.8.5/tests/test_lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-08-07 02:43:25.000000 lognflow-0.8.5/tests/test_logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-08-07 02:43:25.000000 lognflow-0.8.5/tests/test_printprogress.py
```

### Comparing `lognflow-0.8.4/CONTRIBUTING.rst` & `lognflow-0.8.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.4/HISTORY.rst` & `lognflow-0.8.5/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -137,8 +137,13 @@
 -----------------
 * critical bug fixed in log_var to support v0.8.2
 
 0.8.4 (2023-08-03)
 -----------------
 * variable names that are pecular will always be fixed first.
 * suffix can be read form the file name.
-* time_tag will always accompany file name unless stated otherwised.
+* time_tag will always accompany file name unless stated otherwised.
+
+0.8.5 (2023-08-04)
+-----------------
+* Some functions can go to utils and be mentioned in the __init__
+* a bug was fixed in printprogress.
```

### Comparing `lognflow-0.8.4/LICENSE` & `lognflow-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.4/PKG-INFO` & `lognflow-0.8.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.8.4
+Version: 0.8.5
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -231,7 +231,12 @@
 * critical bug fixed in log_var to support v0.8.2
 
 0.8.4 (2023-08-03)
 -----------------
 * variable names that are pecular will always be fixed first.
 * suffix can be read form the file name.
 * time_tag will always accompany file name unless stated otherwised.
+
+0.8.5 (2023-08-04)
+-----------------
+* Some functions can go to utils and be mentioned in the __init__
+* a bug was fixed in printprogress.
```

### Comparing `lognflow-0.8.4/README.rst` & `lognflow-0.8.5/README.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.4/docs/Makefile` & `lognflow-0.8.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.4/docs/conf.py` & `lognflow-0.8.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.4/docs/installation.rst` & `lognflow-0.8.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.4/docs/make.bat` & `lognflow-0.8.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.4/lognflow/lognflow.py` & `lognflow-0.8.5/lognflow/lognflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,37 +41,37 @@
 import itertools
 from   dataclasses import dataclass
 import numpy as np
 
 import matplotlib.pyplot as plt
 import matplotlib.gridspec as gridspec
 from   matplotlib import animation
+from .utils import repr_raw, replace_all, select_directory
+from .plt_utils import plt_colorbar, plt_hist
 
 from .logviewer import logviewer
 
 @dataclass
 class varinlog:
-    data_array        : np.ndarray      
-    time_array        : np.ndarray    
-    curr_index        : int
-    file_start_time   : float          
-    suffix           : str
-    log_counter_limit : int
+    data_array          : np.ndarray      
+    time_array          : np.ndarray    
+    curr_index          : int
+    file_start_time     : float          
+    suffix              : str
+    log_counter_limit   : int
 
 @dataclass
 class textinlog:
     to_be_logged        : str   
     log_fpath           : pathlib.Path         
     log_size_limit      : int 
     log_size            : int     
     last_log_flush_time : float
     log_flush_period    : int
 
-from .utils import repr_raw, replace_all
-
 class lognflow:
     """Initialization
         
         lognflow creates a directory/attribute called log_dir and puts all 
         stored data in there, if logs_root is given. Otherwise give it log_dir
         to use. If you type
         
@@ -147,15 +147,17 @@
         if(log_dir is None):
             if(logs_root is None):
                 from tempfile import gettempdir
                 logs_root = gettempdir()
                 try:
                     logs_root = select_directory(logs_root)
                 except:
-                    pass
+                    print('no logs_root was provided.'
+                          + 'Could not open select_folder'
+                          + f'So a folder from tmp is chosen: {logs_root}')
             new_log_dir_found = False
             while(not new_log_dir_found):
                 log_dir_name = ''
                 if(log_dir_prefix is not None):
                     log_dir_name = str(log_dir_prefix)
                 if len(log_dir_name) > 0:
                     if log_dir_name[-1] != '_':
@@ -740,36 +742,22 @@
         except:
             if(close_plt):
                 plt.close()
             self.log_text(self.log_name,
                           f'Cannot save the plt instance {parameter_name}.')
             return None
      
-    def add_colorbar(self, mappable):
-        """ Add colobar to the current axis 
-            This is specially useful in plt.subplots
-            stackoverflow.com/questions/23876588/
-                matplotlib-colorbar-in-each-subplot
-        """
-        ax = mappable.axes
-        fig = ax.figure
-        from mpl_toolkits.axes_grid1 import make_axes_locatable
-        divider = make_axes_locatable(ax)
-        cax = divider.append_axes("right", size="5%", pad=0.05)
-        cbar = fig.colorbar(mappable, cax=cax)
-        # cbar.ax.tick_params(size=0.01)
-
     def log_multichannel_by_subplots(self, 
         parameter_name: str, 
         parameter_value: np.ndarray,
         frame_shape = None,
         image_format='jpeg', 
         dpi=1200, 
         time_tag: bool = None,
-        add_colorbar = False,
+        colorbar = False,
         remove_axis_ticks = True,
         return_figure = False,
         **kwargs):
         """log multiple images as a tiled square
             The image is logged using plt.imshow
             
             :param parameter_name: str
@@ -796,16 +784,16 @@
         fig, ax = plt.subplots(n_ch_r,n_ch_c)
         if(remove_axis_ticks):
             plt.setp(ax, xticks=[], yticks=[])
         for rcnt in range(n_ch_r):
             for ccnt in range(n_ch_c):
                 im = parameter_value[:,:, ccnt + rcnt * n_ch_c]
                 im_ch = ax[rcnt, ccnt].imshow(im, **kwargs)
-                if(add_colorbar):
-                    self.add_colorbar(im_ch)
+                if(colorbar):
+                    plt_colorbar(im_ch)
         if not return_figure:
             return self.log_plt(parameter_name = parameter_name,
                          image_format=image_format, dpi=dpi,
                          time_tag = time_tag)
         else:
             return fig
             
@@ -871,16 +859,18 @@
         except:
             self.log_text(self.log_name,
                           f'Cannot plot variable {parameter_name}.')
             return None
     
     def log_hist(self, parameter_name: str, 
                        parameter_value_list,
+                       labels_list = None,
                        n_bins = 10,
                        alpha = 0.5,
+                       normalize = False,
                        image_format='jpeg', dpi=1200,
                        time_tag: bool = None, 
                        **kwargs):
         """log a single histogram
             If you have a numpy array or a list of arrays (or indexable by
             first dimension, an array of 1D arrays), use this to log a hist
             if multiple inputs are given they will be plotted on top of each
@@ -901,33 +891,24 @@
                     use 1/number_of_your_variables.
             :param time_tag: bool
                     Wheather if the time stamp is in the file name or not.
                     
         """
         time_tag = self.time_tag if (time_tag is None) else time_tag
             
-        try:
-            if not isinstance(parameter_value_list, list):
-                parameter_value_list = [parameter_value_list]
-                
-            for list_cnt, parameter_value in enumerate(parameter_value_list):
-                bins, edges = np.histogram(parameter_value, n_bins)
-                plt.bar(edges[:-1], bins, 
-                        width =np.diff(edges).mean(), alpha=alpha)
-                plt.plot(edges[:-1], bins, **kwargs)
-            
-            fpath = self.log_plt(
-                parameter_name = parameter_name, 
-                image_format=image_format, dpi=dpi,
-                time_tag = time_tag)
-            return fpath
-        except:
-            self.log_text(self.log_name,
-                f'Cannot make the histogram for variable {parameter_name}.')
-            return None
+        plt_hist(parameter_value_list, 
+             n_bins = n_bins, alpha = alpha, 
+             normalize = normalize, 
+             labels_list = None, **kwargs)
+        
+        fpath = self.log_plt(
+            parameter_name = parameter_name, 
+            image_format=image_format, dpi=dpi,
+            time_tag = time_tag)
+        return fpath
     
     def log_scatter3(self, parameter_name: str,
                        parameter_value, image_format='jpeg', dpi=1200,
                        time_tag: bool = None, return_figure = False):
         """log a single scatter in 3D
             Scatter plotting in 3D
             
@@ -1083,21 +1064,19 @@
                     plt.colorbar(im)
                 if(remove_axis_ticks):
                     plt.setp(ax, xticks=[], yticks=[])
             else:
                 fig, ax = plt.subplots(1, 2)
                 im = ax[0].imshow(np.real(parameter_value), cmap = cmap, **kwargs)
                 if(colorbar):
-                    self.add_colorbar(im)
-                    # plt.colorbar(im)
+                    plt_colorbar(im)
                 ax[0].set_title('Real')    
                 im = ax[1].imshow(np.imag(parameter_value), cmap = cmap, **kwargs)
                 if(colorbar):
-                    self.add_colorbar(im)
-                    # plt.colorbar(im)
+                    plt_colorbar(im)
                 ax[1].set_title('Imag')
                 if(remove_axis_ticks):
                     plt.setp(ax[0], xticks=[], yticks=[])
                     plt.setp(ax[1], xticks=[], yticks=[])
                 
             fpath = self.log_plt(
                 parameter_name = parameter_name,
```

### Comparing `lognflow-0.8.4/lognflow/logviewer.py` & `lognflow-0.8.5/lognflow/logviewer.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.4/lognflow/printprogress.py` & `lognflow-0.8.5/lognflow/printprogress.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,17 +103,15 @@
         remTimeS = 0
         if(self.FLAG_ended):
             if(not self.FLAG_warning):
                 self.FLAG_warning = True
                 self._print_func('-' * self.numTicks)
         else:
             self.ck += ck
-            if(self.ck >= self.n_steps):
-                self.end()
-            else:
+            if(self.ck <= self.n_steps):
                 remTimeS = self._calc_ETA() # useful when print_function is None
                 cProg = int(self.numTicks*self.ck/(self.n_steps-1)/3)    
                 #3: because 3 charachters are used
                 while((self.prog < cProg) & (not self.FLAG_ended)):
                     self.prog += 1
                     remTimeS = self._calc_ETA()
                     if(remTimeS>356400): # less than 99d and more than 99h
@@ -130,14 +128,16 @@
                         self._print_func('m', end='')
                     elif(remTimeS>=0): # less than 99s and more than 0
                         progStr = "%02d" % int(ceil(remTimeS))
                         self._print_func(progStr, end='')
                         self._print_func('s', end='')
                     else:
                         self.end()
+            if(self.ck >= self.n_steps):
+                self.end()
         return remTimeS
     def end(self):
         if(not self.FLAG_ended):
             self._print_func('')
             self.FLAG_ended = True
             
     def __del__(self):
```

### Comparing `lognflow-0.8.4/lognflow/utils.py` & `lognflow-0.8.5/lognflow/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -98,8 +98,8 @@
         obj_out = dict()
         for cnt, _element in enumerate(txt):
             _element_key = str2type(_element.split(': ')[0])
             _element_value = str2type(_element.split(': ')[1])
             obj_out[_element_key] = _element_value
     else:
         obj_out = txt
-    return obj_out
+    return obj_out
```

### Comparing `lognflow-0.8.4/lognflow.egg-info/PKG-INFO` & `lognflow-0.8.5/lognflow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.8.4
+Version: 0.8.5
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -231,7 +231,12 @@
 * critical bug fixed in log_var to support v0.8.2
 
 0.8.4 (2023-08-03)
 -----------------
 * variable names that are pecular will always be fixed first.
 * suffix can be read form the file name.
 * time_tag will always accompany file name unless stated otherwised.
+
+0.8.5 (2023-08-04)
+-----------------
+* Some functions can go to utils and be mentioned in the __init__
+* a bug was fixed in printprogress.
```

### Comparing `lognflow-0.8.4/lognflow.egg-info/SOURCES.txt` & `lognflow-0.8.5/lognflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.4/setup.py` & `lognflow-0.8.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """The setup script for lognflow."""
 
 from setuptools import setup, find_packages
 
 __author__ = 'Alireza Sadri'
 __email__ = 'arsadri@gmail.com'
-__version__ = '0.8.4'
+__version__ = '0.8.5'
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
```

### Comparing `lognflow-0.8.4/tests/test_lognflow.py` & `lognflow-0.8.5/tests/test_lognflow.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.4/tests/test_logviewer.py` & `lognflow-0.8.5/tests/test_logviewer.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.4/tests/test_printprogress.py` & `lognflow-0.8.5/tests/test_printprogress.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 
 import pytest
 
 from lognflow import lognflow, select_directory, logviewer, printprogress
 
 import numpy as np
 
+import tempfile
+temp_dir = tempfile.gettempdir()
+
 @pytest.fixture
 def response():
     """Sample pytest fixture.
 
     See more at: http://doc.pytest.org/en/latest/fixture.html
     """
     # import requests
@@ -26,27 +29,41 @@
     N = 3000000
     pprog = printprogress(N)
     for _ in range(N):
         pprog()
     # assert input('Did it show you a progress bar? (y for yes)')=='y'
 
 def test_printprogress_with_logger():
-    logger = lognflow()
+    logger = lognflow(temp_dir)
     N = 1500000
     pprog = printprogress(N, print_function = logger, log_time_stamp = False)
     for _ in range(N):
         pprog()
         
 def test_printprogress_ETA():
-    logger = lognflow()
+    logger = lognflow(temp_dir)
     N = 500000
     pprog = printprogress(N, print_function = None)
     for _ in range(N):
         ETA = pprog()
         print(ETA)
     
+def test_specific_timing():
+    import time
+    logger = lognflow(temp_dir)
+    N = 7812
+    pprog = printprogress(N, title='Inference of 7812 points. ')
+    for _ in range(N):
+        counter = 0
+        while counter < 15000: 
+            counter += 1
+        pprog()
 
 if __name__ == '__main__':
-    test_printprogress_with_logger()
+    #-----IF RUN BY PYTHON------#
+    temp_dir = select_directory()
+    #---------------------------#
     test_printprogress_ETA()
+    test_specific_timing()
+    test_printprogress_with_logger()
     test_printprogress()
-    exit()
+    exit()
```

