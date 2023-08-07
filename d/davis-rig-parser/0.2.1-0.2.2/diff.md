# Comparing `tmp/davis_rig_parser-0.2.1.tar.gz` & `tmp/davis_rig_parser-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "davis_rig_parser-0.2.1.tar", last modified: Thu Jul 27 16:18:01 2023, max compression
+gzip compressed data, was "davis_rig_parser-0.2.2.tar", last modified: Mon Aug  7 16:44:39 2023, max compression
```

## Comparing `davis_rig_parser-0.2.1.tar` & `davis_rig_parser-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-27 16:18:01.218374 davis_rig_parser-0.2.1/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-27 16:18:01.218374 davis_rig_parser-0.2.1/PKG-INFO
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)     5477 2023-07-06 15:43:33.000000 davis_rig_parser-0.2.1/README.md
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-27 16:18:01.218374 davis_rig_parser-0.2.1/davis_rig_parser/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       56 2023-06-28 16:47:39.000000 davis_rig_parser-0.2.1/davis_rig_parser/__init__.py
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)    19819 2023-07-27 16:13:47.000000 davis_rig_parser-0.2.1/davis_rig_parser/davis_rig_parser.py
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-27 16:18:01.218374 davis_rig_parser-0.2.1/davis_rig_parser.egg-info/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-07-27 16:18:01.000000 davis_rig_parser-0.2.1/davis_rig_parser.egg-info/PKG-INFO
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      297 2023-07-27 16:18:01.000000 davis_rig_parser-0.2.1/davis_rig_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)        1 2023-07-27 16:18:01.000000 davis_rig_parser-0.2.1/davis_rig_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       44 2023-07-27 16:18:01.000000 davis_rig_parser-0.2.1/davis_rig_parser.egg-info/requires.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       17 2023-07-27 16:18:01.000000 davis_rig_parser-0.2.1/davis_rig_parser.egg-info/top_level.txt
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       38 2023-07-27 16:18:01.222375 davis_rig_parser-0.2.1/setup.cfg
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      467 2023-07-27 16:17:34.000000 davis_rig_parser-0.2.1/setup.py
-drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-07-27 16:18:01.218374 davis_rig_parser-0.2.1/tests/
--rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      304 2023-07-05 16:49:12.000000 davis_rig_parser-0.2.1/tests/test.py
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-08-07 16:44:39.674874 davis_rig_parser-0.2.2/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-08-07 16:44:39.674874 davis_rig_parser-0.2.2/PKG-INFO
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)     5859 2023-08-07 16:39:15.000000 davis_rig_parser-0.2.2/README.md
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-08-07 16:44:39.674874 davis_rig_parser-0.2.2/davis_rig_parser/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       56 2023-06-28 16:47:39.000000 davis_rig_parser-0.2.2/davis_rig_parser/__init__.py
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)    19916 2023-08-07 16:40:48.000000 davis_rig_parser-0.2.2/davis_rig_parser/davis_rig_parser.py
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-08-07 16:44:39.674874 davis_rig_parser-0.2.2/davis_rig_parser.egg-info/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      270 2023-08-07 16:44:39.000000 davis_rig_parser-0.2.2/davis_rig_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      297 2023-08-07 16:44:39.000000 davis_rig_parser-0.2.2/davis_rig_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)        1 2023-08-07 16:44:39.000000 davis_rig_parser-0.2.2/davis_rig_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       44 2023-08-07 16:44:39.000000 davis_rig_parser-0.2.2/davis_rig_parser.egg-info/requires.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       17 2023-08-07 16:44:39.000000 davis_rig_parser-0.2.2/davis_rig_parser.egg-info/top_level.txt
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)       38 2023-08-07 16:44:39.674874 davis_rig_parser-0.2.2/setup.cfg
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      467 2023-08-07 16:43:28.000000 davis_rig_parser-0.2.2/setup.py
+drwxrwxr-x   0 senecascott  (1000) senecascott  (1000)        0 2023-08-07 16:44:39.674874 davis_rig_parser-0.2.2/tests/
+-rw-rw-r--   0 senecascott  (1000) senecascott  (1000)      304 2023-07-05 16:49:12.000000 davis_rig_parser-0.2.2/tests/test.py
```

### Comparing `davis_rig_parser-0.2.1/README.md` & `davis_rig_parser-0.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,17 @@
 ```
 You're now ready to use davis_rig_parser to create dataframes!
 
 ## Creating The Dataframe
 
 ### Setting Up the Text Files
 
-Make sure you have a folder where the only .txt files are the Med Associates gustometer standardized output for the Davis Rig, you should put all .txt files you want to be turned into a dataframe in the same folder for ease. If you have a .txt file with supplemental animal info, put those in a separate folder. You should have two different folders. They don't have to be stored in adjacent folders, just different folders.
+Make sure you have a folder where the only .txt files are the Med Associates gustometer standardized output for the Davis Rig, you should put all .txt files you want to be turned into a dataframe in the same folder for ease. 
+
+If you have a .txt file with supplemental animal info, put those in a separate folder. In this case, you should have two different folders. They don't have to be stored in adjacent folders, just different folders.
 
 ### Running the code
 
 You can create the dataframe as a variable in your code and/or save it as a .df file. The first 2 examples will save a .df file in the same directory chosen (chosen in the pop up or passed as dir_name). The title of the .df file will be '/chosen_directory/27_06_2023_grouped_dframe.df' where 27_06_2023 is the current date in day_month_year format. 
 ```python
 import davis_rig_parser
 
@@ -81,32 +83,40 @@
 
 If you would like to change the bout size you are using change the bout_pause parameter. It is 300 by default. 
 
 ```python
 import davis_rig_parser
 
 davis_rig_parser.create_df(bout_pause=300)
+#Keep in mind you can change multiple parameters at once
+davis_rig_parser.create_df(bout_pause=300, min_latency=100, min_ILI=75)
 ```
 #### Minimum Latency
 
 The Davis Rig will occasionally record false licks when the shutter opens. If the latency of the recorded 'first lick' is less than min_ILI, this 'first lick' is considered shutter openning rather than a true lick. The 1st, 2nd, 3rd...etc licks are summed until the latency is greater than 100ms by default. The number of summed ILIs is deleted from the Licks column in the .txt file. 
 ```python
 import davis_rig_parser
 
 davis_rig_parser.create_df(min_latency=100)
+#Keep in mind you can change multiple at once
+davis_rig_parser.create_df(bout_pause=300, min_latency=100)
+
 ```
 Possible false licks created by the shutter closing are not accounted for. 
 #### Minimum Possible ILI
 
 The parser will delete all interlick intervals (ILIs) under the min_ILI threshold. These small ILIs are not possible for a rat tounge to move faster than ~75ms. Their source is unknown for certain, but they might be created by the animals bumping into the spout. It is 75 by default. The number of deleted ILIs is deleted from the Licks column in the .txt file. 
 ```python
 import davis_rig_parser
 
 davis_rig_parser.create_df(min_ILI=75)
+#Keep in mind you can change multiple parameters at once
+davis_rig_parser.create_df(bout_pause=300, min_latency=100, min_ILI=75)
 ```
+
 ## License
 
 This project is licensed under the terms of the GNU General Public License v3.0.
 
 The GNU General Public License is a free, copyleft license for software and other kinds of works. The GNU General Public License is intended to guarantee your freedom to share and change all versions of a program--to make sure it remains free software for all its users.
 
 For more details, please check the [LICENSE](./LICENSE) file in the repository, or read the [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.en.html).
```

### Comparing `davis_rig_parser-0.2.1/davis_rig_parser/davis_rig_parser.py` & `davis_rig_parser-0.2.2/davis_rig_parser/davis_rig_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -422,14 +422,18 @@
     df['LENGTH'] = df['LENGTH'].str.strip().astype(int)
     
     #Length is the length given to the shutter opening, but since the 
     #first lick(s) could be false, the actual time the rat has to lick
     #is Tri_Length
     df['Tri_LENGTH'] = df['LENGTH'] - df['Tri_LENGTH']
     
+    df['Bouts'] = df['Bouts'].apply(lambda x: [] if isinstance(x, int) and x == 0 else x)
+
+
+    
     #Save dataframe for later use/plotting/analyses
     #timestamped with date
     if save_df==True:
         df.to_pickle(dir_name+'/%s_grouped_dframe.df' %(date.today().strftime("%d_%m_%Y")))
 
     return df
```

