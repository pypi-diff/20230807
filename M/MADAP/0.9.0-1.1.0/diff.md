# Comparing `tmp/MADAP-0.9.0.tar.gz` & `tmp/MADAP-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MADAP-0.9.0.tar", last modified: Sun Oct  2 22:16:58 2022, max compression
+gzip compressed data, was "MADAP-1.1.0.tar", last modified: Mon Aug  7 11:20:05 2023, max compression
```

## Comparing `MADAP-0.9.0.tar` & `MADAP-1.1.0.tar`

### file list

```diff
@@ -1,80 +1,83 @@
-drwxrwxrwx   0        0        0        0 2022-10-02 22:16:48.649145 MADAP-0.9.0/
--rw-rw-rw-   0        0        0      180 2022-10-02 19:59:36.000000 MADAP-0.9.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3497 2022-10-02 21:17:53.000000 MADAP-0.9.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      165 2022-10-02 22:13:22.000000 MADAP-0.9.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1097 2022-10-02 19:59:36.000000 MADAP-0.9.0/LICENSE
-drwxrwxrwx   0        0        0        0 2022-10-02 22:16:58.844704 MADAP-0.9.0/MADAP.egg-info/
--rw-rw-rw-   0        0        0     4829 2022-10-02 22:16:58.000000 MADAP-0.9.0/MADAP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1773 2022-10-02 22:16:58.000000 MADAP-0.9.0/MADAP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-02 22:16:58.000000 MADAP-0.9.0/MADAP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2022-10-02 22:16:58.000000 MADAP-0.9.0/MADAP.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-10-02 22:15:26.000000 MADAP-0.9.0/MADAP.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      148 2022-10-02 22:16:58.000000 MADAP-0.9.0/MADAP.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2022-10-02 22:16:58.000000 MADAP-0.9.0/MADAP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      252 2022-10-02 21:55:02.000000 MADAP-0.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4829 2022-10-02 22:16:58.853704 MADAP-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     3555 2022-10-02 22:09:58.000000 MADAP-0.9.0/README.rst
-drwxrwxrwx   0        0        0        0 2022-10-02 22:16:48.612641 MADAP-0.9.0/docs/
--rw-rw-rw-   0        0        0        0 2022-09-30 15:36:40.000000 MADAP-0.9.0/docs/.nojekyll
--rw-rw-rw-   0        0        0      658 2022-08-23 21:03:25.000000 MADAP-0.9.0/docs/Makefile
-drwxrwxrwx   0        0        0        0 2022-10-02 22:16:48.587143 MADAP-0.9.0/docs/build/
-drwxrwxrwx   0        0        0        0 2022-10-02 22:16:48.613642 MADAP-0.9.0/docs/build/html/
--rw-rw-rw-   0        0        0        0 2022-10-02 21:11:54.000000 MADAP-0.9.0/docs/build/html/.nojekyll
--rwxrwxrwx   0        0        0      804 2022-08-23 21:03:25.000000 MADAP-0.9.0/docs/make.bat
-drwxrwxrwx   0        0        0        0 2022-10-02 22:16:48.615143 MADAP-0.9.0/docs/source/
--rw-rw-rw-   0        0        0     2311 2022-09-30 15:36:40.000000 MADAP-0.9.0/docs/source/conf.py
-drwxrwxrwx   0        0        0        0 2022-10-02 22:16:48.617143 MADAP-0.9.0/docs/source/generated_arrhenius/
--rw-rw-rw-   0        0        0      341 2022-07-26 20:46:09.000000 MADAP-0.9.0/docs/source/generated_arrhenius/arrhenius.rst
--rw-rw-rw-   0        0        0       71 2022-07-26 20:42:22.000000 MADAP-0.9.0/docs/source/generated_arrhenius/modules.rst
-drwxrwxrwx   0        0        0        0 2022-10-02 22:16:48.619145 MADAP-0.9.0/docs/source/generated_impedance/
--rw-rw-rw-   0        0        0      381 2022-08-20 17:46:12.000000 MADAP-0.9.0/docs/source/generated_impedance/impedance.rst
--rw-rw-rw-   0        0        0       71 2022-07-26 20:42:11.000000 MADAP-0.9.0/docs/source/generated_impedance/modules.rst
-drwxrwxrwx   0        0        0        0 2022-10-02 22:16:48.619644 MADAP-0.9.0/docs/source/generated_voltammetry/
--rw-rw-rw-   0        0        0       24 2022-07-26 20:42:04.000000 MADAP-0.9.0/docs/source/generated_voltammetry/modules.rst
--rw-rw-rw-   0        0        0      790 2022-07-26 20:48:13.000000 MADAP-0.9.0/docs/source/index.rst
--rw-rw-rw-   0        0        0      479 2022-10-02 21:14:24.000000 MADAP-0.9.0/pages-publish.sh
--rw-rw-rw-   0        0        0      137 2022-09-30 15:36:40.000000 MADAP-0.9.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-10-02 22:16:58.857703 MADAP-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0     2152 2022-10-02 22:09:31.000000 MADAP-0.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-02 22:16:48.622143 MADAP-0.9.0/src/
--rw-rw-rw-   0        0        0        0 2022-10-02 20:34:57.000000 MADAP-0.9.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-02 22:16:48.623142 MADAP-0.9.0/src/madap/
--rw-rw-rw-   0        0        0        0 2022-09-30 15:36:40.000000 MADAP-0.9.0/src/madap/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-02 22:16:48.625142 MADAP-0.9.0/src/madap/data_acquisition/
--rw-rw-rw-   0        0        0        0 2022-09-30 15:36:40.000000 MADAP-0.9.0/src/madap/data_acquisition/__init__.py
--rw-rw-rw-   0        0        0     5375 2022-10-02 17:29:16.000000 MADAP-0.9.0/src/madap/data_acquisition/data_acquisition.py
-drwxrwxrwx   0        0        0        0 2022-10-02 22:16:48.626643 MADAP-0.9.0/src/madap/echem/
--rw-rw-rw-   0        0        0        0 2022-09-30 15:36:40.000000 MADAP-0.9.0/src/madap/echem/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-02 22:16:48.629642 MADAP-0.9.0/src/madap/echem/arrhenius/
--rw-rw-rw-   0        0        0        0 2022-09-30 15:36:40.000000 MADAP-0.9.0/src/madap/echem/arrhenius/__init__.py
--rw-rw-rw-   0        0        0     7936 2022-10-02 17:02:22.000000 MADAP-0.9.0/src/madap/echem/arrhenius/arrhenius.py
--rw-rw-rw-   0        0        0     4824 2022-10-02 15:29:07.000000 MADAP-0.9.0/src/madap/echem/arrhenius/arrhenius_plotting.py
-drwxrwxrwx   0        0        0        0 2022-10-02 22:16:48.632143 MADAP-0.9.0/src/madap/echem/e_impedance/
--rw-rw-rw-   0        0        0        0 2022-09-30 15:36:40.000000 MADAP-0.9.0/src/madap/echem/e_impedance/__init__.py
--rw-rw-rw-   0        0        0    19397 2022-10-02 15:22:25.000000 MADAP-0.9.0/src/madap/echem/e_impedance/e_impedance.py
--rw-rw-rw-   0        0        0    12557 2022-10-02 13:59:09.000000 MADAP-0.9.0/src/madap/echem/e_impedance/e_impedance_plotting.py
--rw-rw-rw-   0        0        0     1464 2022-09-30 15:36:40.000000 MADAP-0.9.0/src/madap/echem/procedure.py
-drwxrwxrwx   0        0        0        0 2022-10-02 22:16:48.637642 MADAP-0.9.0/src/madap/echem/voltammetry/
--rw-rw-rw-   0        0        0        0 2022-09-30 15:36:40.000000 MADAP-0.9.0/src/madap/echem/voltammetry/__init__.py
--rw-rw-rw-   0        0        0      496 2022-09-30 15:36:40.000000 MADAP-0.9.0/src/madap/echem/voltammetry/voltammetry.py
--rw-rw-rw-   0        0        0      903 2022-09-30 15:36:40.000000 MADAP-0.9.0/src/madap/echem/voltammetry/voltammetry_CA.py
--rw-rw-rw-   0        0        0      584 2022-09-30 15:36:40.000000 MADAP-0.9.0/src/madap/echem/voltammetry/voltammetry_CP.py
--rw-rw-rw-   0        0        0      743 2022-09-30 15:36:40.000000 MADAP-0.9.0/src/madap/echem/voltammetry/voltammetry_CV.py
--rw-rw-rw-   0        0        0      518 2022-09-30 15:36:40.000000 MADAP-0.9.0/src/madap/echem/voltammetry/voltammetry_plotting.py
-drwxrwxrwx   0        0        0        0 2022-10-02 22:16:48.639643 MADAP-0.9.0/src/madap/logger/
--rw-rw-rw-   0        0        0        0 2022-09-30 15:36:40.000000 MADAP-0.9.0/src/madap/logger/__init__.py
--rw-rw-rw-   0        0        0     1460 2022-10-01 21:47:55.000000 MADAP-0.9.0/src/madap/logger/logger.py
-drwxrwxrwx   0        0        0        0 2022-10-02 22:16:48.641142 MADAP-0.9.0/src/madap/plotting/
--rw-rw-rw-   0        0        0        0 2022-09-30 15:36:40.000000 MADAP-0.9.0/src/madap/plotting/__init__.py
--rw-rw-rw-   0        0        0     6789 2022-10-01 21:48:32.000000 MADAP-0.9.0/src/madap/plotting/plotting.py
-drwxrwxrwx   0        0        0        0 2022-10-02 22:16:48.644146 MADAP-0.9.0/src/madap/plotting/styles/
--rw-rw-rw-   0        0        0      937 2022-09-30 15:36:40.000000 MADAP-0.9.0/src/madap/plotting/styles/nature.mplstyle
--rw-rw-rw-   0        0        0       43 2022-09-30 15:36:40.000000 MADAP-0.9.0/src/madap/plotting/styles/no-latex.mplstyle
--rw-rw-rw-   0        0        0     1158 2022-09-30 15:36:40.000000 MADAP-0.9.0/src/madap/plotting/styles/science.mplstyle
-drwxrwxrwx   0        0        0        0 2022-10-02 22:16:48.647643 MADAP-0.9.0/src/madap/utils/
--rw-rw-rw-   0        0        0        0 2022-09-30 15:36:40.000000 MADAP-0.9.0/src/madap/utils/__init__.py
--rw-rw-rw-   0        0        0     3369 2022-10-02 14:12:11.000000 MADAP-0.9.0/src/madap/utils/gui_elements.py
--rw-rw-rw-   0        0        0     2805 2022-09-30 15:36:40.000000 MADAP-0.9.0/src/madap/utils/suggested_circuits.py
--rw-rw-rw-   0        0        0     3068 2022-10-02 15:24:26.000000 MADAP-0.9.0/src/madap/utils/utils.py
--rw-rw-rw-   0        0        0    14515 2022-10-02 17:10:45.000000 MADAP-0.9.0/src/madap_cli.py
--rw-rw-rw-   0        0        0    15873 2022-10-02 16:03:24.000000 MADAP-0.9.0/src/madap_gui.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:05.724044 MADAP-1.1.0/
+-rw-rw-rw-   0        0        0      180 2022-10-02 19:59:36.000000 MADAP-1.1.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3497 2022-10-02 21:17:53.000000 MADAP-1.1.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      638 2023-08-07 11:17:38.000000 MADAP-1.1.0/HISTORY.rst
+-rw-rw-rw-   0        0        0     1097 2022-10-02 19:59:36.000000 MADAP-1.1.0/LICENSE
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:05.690037 MADAP-1.1.0/MADAP.egg-info/
+-rw-rw-rw-   0        0        0     5850 2023-08-07 11:20:05.000000 MADAP-1.1.0/MADAP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1726 2023-08-07 11:20:05.000000 MADAP-1.1.0/MADAP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 11:20:05.000000 MADAP-1.1.0/MADAP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-08-07 11:20:05.000000 MADAP-1.1.0/MADAP.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-10-02 22:15:26.000000 MADAP-1.1.0/MADAP.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      148 2023-08-07 11:20:05.000000 MADAP-1.1.0/MADAP.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       43 2023-08-07 11:20:05.000000 MADAP-1.1.0/MADAP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      254 2022-10-16 15:37:36.000000 MADAP-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5850 2023-08-07 11:20:05.724044 MADAP-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4233 2023-08-07 11:19:49.000000 MADAP-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:05.692038 MADAP-1.1.0/docs/
+-rw-rw-rw-   0        0        0        0 2022-09-30 15:36:40.000000 MADAP-1.1.0/docs/.nojekyll
+-rw-rw-rw-   0        0        0      658 2022-08-23 21:03:25.000000 MADAP-1.1.0/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:05.663038 MADAP-1.1.0/docs/build/
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:05.693037 MADAP-1.1.0/docs/build/html/
+-rw-rw-rw-   0        0        0        0 2022-10-16 15:43:34.000000 MADAP-1.1.0/docs/build/html/.nojekyll
+-rwxrwxrwx   0        0        0      804 2022-08-23 21:03:25.000000 MADAP-1.1.0/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:05.694539 MADAP-1.1.0/docs/source/
+-rw-rw-rw-   0        0        0     2276 2022-10-16 15:37:31.000000 MADAP-1.1.0/docs/source/conf.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:05.696537 MADAP-1.1.0/docs/source/generated_arrhenius/
+-rw-rw-rw-   0        0        0      341 2022-07-26 20:46:09.000000 MADAP-1.1.0/docs/source/generated_arrhenius/arrhenius.rst
+-rw-rw-rw-   0        0        0       71 2022-07-26 20:42:22.000000 MADAP-1.1.0/docs/source/generated_arrhenius/modules.rst
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:05.697537 MADAP-1.1.0/docs/source/generated_impedance/
+-rw-rw-rw-   0        0        0      381 2022-08-20 17:46:12.000000 MADAP-1.1.0/docs/source/generated_impedance/impedance.rst
+-rw-rw-rw-   0        0        0       71 2022-07-26 20:42:11.000000 MADAP-1.1.0/docs/source/generated_impedance/modules.rst
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:05.698537 MADAP-1.1.0/docs/source/generated_voltammetry/
+-rw-rw-rw-   0        0        0       24 2022-07-26 20:42:04.000000 MADAP-1.1.0/docs/source/generated_voltammetry/modules.rst
+-rw-rw-rw-   0        0        0     1677 2022-10-03 12:28:15.000000 MADAP-1.1.0/docs/source/index.rst
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:05.699037 MADAP-1.1.0/docs/source/usage/
+-rw-rw-rw-   0        0        0     4736 2022-10-16 15:37:27.000000 MADAP-1.1.0/docs/source/usage/usage.rst
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:05.701041 MADAP-1.1.0/figures_creation/
+-rw-rw-rw-   0        0        0        0 2022-09-23 21:03:52.000000 MADAP-1.1.0/figures_creation/__init__.py
+-rw-rw-rw-   0        0        0     7915 2022-08-27 19:45:44.000000 MADAP-1.1.0/figures_creation/test_joblib.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:05.702036 MADAP-1.1.0/madap/
+-rw-rw-rw-   0        0        0        0 2022-10-16 14:31:52.000000 MADAP-1.1.0/madap/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:05.703037 MADAP-1.1.0/madap/data_acquisition/
+-rw-rw-rw-   0        0        0        0 2022-09-30 15:36:40.000000 MADAP-1.1.0/madap/data_acquisition/__init__.py
+-rw-rw-rw-   0        0        0     5375 2023-08-07 10:58:30.000000 MADAP-1.1.0/madap/data_acquisition/data_acquisition.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:05.704537 MADAP-1.1.0/madap/echem/
+-rw-rw-rw-   0        0        0        0 2022-09-30 15:36:40.000000 MADAP-1.1.0/madap/echem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:05.707038 MADAP-1.1.0/madap/echem/arrhenius/
+-rw-rw-rw-   0        0        0        0 2022-09-30 15:36:40.000000 MADAP-1.1.0/madap/echem/arrhenius/__init__.py
+-rw-rw-rw-   0        0        0     7936 2022-10-02 17:02:22.000000 MADAP-1.1.0/madap/echem/arrhenius/arrhenius.py
+-rw-rw-rw-   0        0        0     4824 2022-10-02 15:29:07.000000 MADAP-1.1.0/madap/echem/arrhenius/arrhenius_plotting.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:05.709539 MADAP-1.1.0/madap/echem/e_impedance/
+-rw-rw-rw-   0        0        0        0 2022-09-30 15:36:40.000000 MADAP-1.1.0/madap/echem/e_impedance/__init__.py
+-rw-rw-rw-   0        0        0    20295 2023-08-07 11:04:20.000000 MADAP-1.1.0/madap/echem/e_impedance/e_impedance.py
+-rw-rw-rw-   0        0        0    12557 2022-10-02 13:59:09.000000 MADAP-1.1.0/madap/echem/e_impedance/e_impedance_plotting.py
+-rw-rw-rw-   0        0        0     1464 2022-09-30 15:36:40.000000 MADAP-1.1.0/madap/echem/procedure.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:05.714538 MADAP-1.1.0/madap/echem/voltammetry/
+-rw-rw-rw-   0        0        0        0 2022-09-30 15:36:40.000000 MADAP-1.1.0/madap/echem/voltammetry/__init__.py
+-rw-rw-rw-   0        0        0      496 2023-08-07 10:58:30.000000 MADAP-1.1.0/madap/echem/voltammetry/voltammetry.py
+-rw-rw-rw-   0        0        0      903 2023-08-07 10:58:30.000000 MADAP-1.1.0/madap/echem/voltammetry/voltammetry_CA.py
+-rw-rw-rw-   0        0        0      584 2023-08-07 10:58:30.000000 MADAP-1.1.0/madap/echem/voltammetry/voltammetry_CP.py
+-rw-rw-rw-   0        0        0      743 2022-09-30 15:36:40.000000 MADAP-1.1.0/madap/echem/voltammetry/voltammetry_CV.py
+-rw-rw-rw-   0        0        0      518 2023-08-07 10:58:30.000000 MADAP-1.1.0/madap/echem/voltammetry/voltammetry_plotting.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:05.716037 MADAP-1.1.0/madap/logger/
+-rw-rw-rw-   0        0        0        0 2022-09-30 15:36:40.000000 MADAP-1.1.0/madap/logger/__init__.py
+-rw-rw-rw-   0        0        0     1460 2022-10-01 21:47:55.000000 MADAP-1.1.0/madap/logger/logger.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:05.717537 MADAP-1.1.0/madap/plotting/
+-rw-rw-rw-   0        0        0        0 2022-09-30 15:36:40.000000 MADAP-1.1.0/madap/plotting/__init__.py
+-rw-rw-rw-   0        0        0     6789 2022-10-01 21:48:32.000000 MADAP-1.1.0/madap/plotting/plotting.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:05.720043 MADAP-1.1.0/madap/plotting/styles/
+-rw-rw-rw-   0        0        0      937 2022-09-30 15:36:40.000000 MADAP-1.1.0/madap/plotting/styles/nature.mplstyle
+-rw-rw-rw-   0        0        0       43 2022-09-30 15:36:40.000000 MADAP-1.1.0/madap/plotting/styles/no-latex.mplstyle
+-rw-rw-rw-   0        0        0     1158 2022-09-30 15:36:40.000000 MADAP-1.1.0/madap/plotting/styles/science.mplstyle
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:05.723042 MADAP-1.1.0/madap/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-30 15:36:40.000000 MADAP-1.1.0/madap/utils/__init__.py
+-rw-rw-rw-   0        0        0     3369 2022-10-02 14:12:11.000000 MADAP-1.1.0/madap/utils/gui_elements.py
+-rw-rw-rw-   0        0        0     2805 2023-08-07 10:49:51.000000 MADAP-1.1.0/madap/utils/suggested_circuits.py
+-rw-rw-rw-   0        0        0     3068 2023-08-07 10:39:59.000000 MADAP-1.1.0/madap/utils/utils.py
+-rw-rw-rw-   0        0        0    14515 2023-08-07 10:58:30.000000 MADAP-1.1.0/madap_cli.py
+-rw-rw-rw-   0        0        0    15874 2022-10-17 20:11:37.000000 MADAP-1.1.0/madap_gui.py
+-rw-rw-rw-   0        0        0      479 2022-10-02 21:14:24.000000 MADAP-1.1.0/pages-publish.sh
+-rw-rw-rw-   0        0        0      137 2022-09-30 15:36:40.000000 MADAP-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 11:20:05.724545 MADAP-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2054 2023-08-07 11:17:48.000000 MADAP-1.1.0/setup.py
```

### Comparing `MADAP-0.9.0/CONTRIBUTING.rst` & `MADAP-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `MADAP-0.9.0/LICENSE` & `MADAP-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `MADAP-0.9.0/MADAP.egg-info/PKG-INFO` & `MADAP-1.1.0/MADAP.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: MADAP
-Version: 0.9.0
+Version: 1.1.0
 Summary: This is MADAP, a software package for the analysis of electrochemical data.
 Home-page: https://github.com/fuzhanrahmanian/MADAP
 Author: Fuzhan Rahmanian
 Author-email: fuzhanrahmanian@gmail.com
 License: MIT license
 Keywords: madap
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS.rst
 
+.. image:: logo.png
+    :align: center
+
 MADAP
 ~~~~~
 
 Modular and Autonomous Data Analysis Platform (MADAP) is a
 well-documented python package which can be used for electrochmeical
 data analysis.
 
@@ -63,15 +64,17 @@
 
    pip install MADAP
 
 
 Usage
 ~~~~~
 
-MADAP can be used in a python script as follows:
+A brief tutorial video of the basic of MADAP usage can found  `here <https://youtu.be/nL-eJpb1AxI>`_. 
+
+MADAP can be used in a python script as follows: 
 
 .. code:: python
 
     from madap.echem.arrhenius import arrhenius
     from madap.echem.e_impedance import e_impedance
     from madap.data_acquisition import data_acquisition as da
 
@@ -122,28 +125,56 @@
 
 
 Citation
 ~~~~~~~~
 
 If you use MADAP in your research, please cite this GitHub repository https://github.com/fuzhanrahmanian/MADAP.
 
+.. image:: https://zenodo.org/badge/494354435.svg
+   :target: https://zenodo.org/badge/latestdoi/494354435
+
 
 References
 ~~~~~~~~~~
 
 This package is based relies on the following packages and papers:
 - Impedance GitHub repository by Matthew D. Murbach and Brian Gerwe and Neal Dawson-Elli and Lok-kun Tsui: `link <https://github.com/ECSHackWeek/impedance.py>`__
 - A Method for Improving the Robustness of linear Kramers-Kronig Validity Tests DOI: https://doi.org/10.1016/j.electacta.2014.01.034
 
+Acknowledgement
+~~~~~~~~~~~~~~~
+
+This project has received funding from the European Union’s [Horizon 2020 research and innovation programme](https://ec.europa.eu/programmes/horizon2020/en) under grant agreement [No 957189](https://cordis.europa.eu/project/id/957189). The project is part of BATTERY 2030+, the large-scale European research initiative for inventing the sustainable batteries of the future.
+
+
 =======
 History
 =======
 
+1.1.0 (2023-08-07)
+-------------------
+* Fixes issue with mismatch array length when positive imaginary data is given
+
+0.11.0 (2022-10-16)
+-------------------
+
+* Fixed bugs concering the package installation.
+* Improved the documentation.
+* Imrpoved the file structure.
+* madap_gui and madap_cli are now in the same package and can be used as standalone scripts/commands.
+
+0.10.0 (2022-10-03)
+-------------------
+
+* Updated support of the python versions
+
 0.9.0 (2022-10-02)
 ------------------
 
 * Update documentation
 
 0.8.0 (2022-10-02)
 ------------------
 
 * First release on PyPI.
+
+
```

### Comparing `MADAP-0.9.0/MADAP.egg-info/SOURCES.txt` & `MADAP-1.1.0/MADAP.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
+madap_cli.py
+madap_gui.py
 pages-publish.sh
 requirements.txt
 setup.py
 MADAP.egg-info/PKG-INFO
 MADAP.egg-info/SOURCES.txt
 MADAP.egg-info/dependency_links.txt
 MADAP.egg-info/entry_points.txt
@@ -21,38 +23,38 @@
 docs/source/conf.py
 docs/source/index.rst
 docs/source/generated_arrhenius/arrhenius.rst
 docs/source/generated_arrhenius/modules.rst
 docs/source/generated_impedance/impedance.rst
 docs/source/generated_impedance/modules.rst
 docs/source/generated_voltammetry/modules.rst
-src/__init__.py
-src/madap_cli.py
-src/madap_gui.py
-src/madap/__init__.py
-src/madap/data_acquisition/__init__.py
-src/madap/data_acquisition/data_acquisition.py
-src/madap/echem/__init__.py
-src/madap/echem/procedure.py
-src/madap/echem/arrhenius/__init__.py
-src/madap/echem/arrhenius/arrhenius.py
-src/madap/echem/arrhenius/arrhenius_plotting.py
-src/madap/echem/e_impedance/__init__.py
-src/madap/echem/e_impedance/e_impedance.py
-src/madap/echem/e_impedance/e_impedance_plotting.py
-src/madap/echem/voltammetry/__init__.py
-src/madap/echem/voltammetry/voltammetry.py
-src/madap/echem/voltammetry/voltammetry_CA.py
-src/madap/echem/voltammetry/voltammetry_CP.py
-src/madap/echem/voltammetry/voltammetry_CV.py
-src/madap/echem/voltammetry/voltammetry_plotting.py
-src/madap/logger/__init__.py
-src/madap/logger/logger.py
-src/madap/plotting/__init__.py
-src/madap/plotting/plotting.py
-src/madap/plotting/styles/nature.mplstyle
-src/madap/plotting/styles/no-latex.mplstyle
-src/madap/plotting/styles/science.mplstyle
-src/madap/utils/__init__.py
-src/madap/utils/gui_elements.py
-src/madap/utils/suggested_circuits.py
-src/madap/utils/utils.py
+docs/source/usage/usage.rst
+figures_creation/__init__.py
+figures_creation/test_joblib.py
+madap/__init__.py
+madap/data_acquisition/__init__.py
+madap/data_acquisition/data_acquisition.py
+madap/echem/__init__.py
+madap/echem/procedure.py
+madap/echem/arrhenius/__init__.py
+madap/echem/arrhenius/arrhenius.py
+madap/echem/arrhenius/arrhenius_plotting.py
+madap/echem/e_impedance/__init__.py
+madap/echem/e_impedance/e_impedance.py
+madap/echem/e_impedance/e_impedance_plotting.py
+madap/echem/voltammetry/__init__.py
+madap/echem/voltammetry/voltammetry.py
+madap/echem/voltammetry/voltammetry_CA.py
+madap/echem/voltammetry/voltammetry_CP.py
+madap/echem/voltammetry/voltammetry_CV.py
+madap/echem/voltammetry/voltammetry_plotting.py
+madap/logger/__init__.py
+madap/logger/logger.py
+madap/plotting/__init__.py
+madap/plotting/plotting.py
+madap/plotting/styles/nature.mplstyle
+madap/plotting/styles/no-latex.mplstyle
+madap/plotting/styles/science.mplstyle
+madap/utils/__init__.py
+madap/utils/gui_elements.py
+madap/utils/suggested_circuits.py
+madap/utils/utils.py
```

### Comparing `MADAP-0.9.0/PKG-INFO` & `MADAP-1.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: MADAP
-Version: 0.9.0
+Version: 1.1.0
 Summary: This is MADAP, a software package for the analysis of electrochemical data.
 Home-page: https://github.com/fuzhanrahmanian/MADAP
 Author: Fuzhan Rahmanian
 Author-email: fuzhanrahmanian@gmail.com
 License: MIT license
 Keywords: madap
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS.rst
 
+.. image:: logo.png
+    :align: center
+
 MADAP
 ~~~~~
 
 Modular and Autonomous Data Analysis Platform (MADAP) is a
 well-documented python package which can be used for electrochmeical
 data analysis.
 
@@ -63,15 +64,17 @@
 
    pip install MADAP
 
 
 Usage
 ~~~~~
 
-MADAP can be used in a python script as follows:
+A brief tutorial video of the basic of MADAP usage can found  `here <https://youtu.be/nL-eJpb1AxI>`_. 
+
+MADAP can be used in a python script as follows: 
 
 .. code:: python
 
     from madap.echem.arrhenius import arrhenius
     from madap.echem.e_impedance import e_impedance
     from madap.data_acquisition import data_acquisition as da
 
@@ -122,28 +125,56 @@
 
 
 Citation
 ~~~~~~~~
 
 If you use MADAP in your research, please cite this GitHub repository https://github.com/fuzhanrahmanian/MADAP.
 
+.. image:: https://zenodo.org/badge/494354435.svg
+   :target: https://zenodo.org/badge/latestdoi/494354435
+
 
 References
 ~~~~~~~~~~
 
 This package is based relies on the following packages and papers:
 - Impedance GitHub repository by Matthew D. Murbach and Brian Gerwe and Neal Dawson-Elli and Lok-kun Tsui: `link <https://github.com/ECSHackWeek/impedance.py>`__
 - A Method for Improving the Robustness of linear Kramers-Kronig Validity Tests DOI: https://doi.org/10.1016/j.electacta.2014.01.034
 
+Acknowledgement
+~~~~~~~~~~~~~~~
+
+This project has received funding from the European Union’s [Horizon 2020 research and innovation programme](https://ec.europa.eu/programmes/horizon2020/en) under grant agreement [No 957189](https://cordis.europa.eu/project/id/957189). The project is part of BATTERY 2030+, the large-scale European research initiative for inventing the sustainable batteries of the future.
+
+
 =======
 History
 =======
 
+1.1.0 (2023-08-07)
+-------------------
+* Fixes issue with mismatch array length when positive imaginary data is given
+
+0.11.0 (2022-10-16)
+-------------------
+
+* Fixed bugs concering the package installation.
+* Improved the documentation.
+* Imrpoved the file structure.
+* madap_gui and madap_cli are now in the same package and can be used as standalone scripts/commands.
+
+0.10.0 (2022-10-03)
+-------------------
+
+* Updated support of the python versions
+
 0.9.0 (2022-10-02)
 ------------------
 
 * Update documentation
 
 0.8.0 (2022-10-02)
 ------------------
 
 * First release on PyPI.
+
+
```

### Comparing `MADAP-0.9.0/README.rst` & `MADAP-1.1.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+.. image:: logo.png
+    :align: center
+
 MADAP
 ~~~~~
 
 Modular and Autonomous Data Analysis Platform (MADAP) is a
 well-documented python package which can be used for electrochmeical
 data analysis.
 
@@ -35,15 +38,17 @@
 
    pip install MADAP
 
 
 Usage
 ~~~~~
 
-MADAP can be used in a python script as follows:
+A brief tutorial video of the basic of MADAP usage can found  `here <https://youtu.be/nL-eJpb1AxI>`_. 
+
+MADAP can be used in a python script as follows: 
 
 .. code:: python
 
     from madap.echem.arrhenius import arrhenius
     from madap.echem.e_impedance import e_impedance
     from madap.data_acquisition import data_acquisition as da
 
@@ -94,14 +99,22 @@
 
 
 Citation
 ~~~~~~~~
 
 If you use MADAP in your research, please cite this GitHub repository https://github.com/fuzhanrahmanian/MADAP.
 
+.. image:: https://zenodo.org/badge/494354435.svg
+   :target: https://zenodo.org/badge/latestdoi/494354435
+
 
 References
 ~~~~~~~~~~
 
 This package is based relies on the following packages and papers:
 - Impedance GitHub repository by Matthew D. Murbach and Brian Gerwe and Neal Dawson-Elli and Lok-kun Tsui: `link <https://github.com/ECSHackWeek/impedance.py>`__
-- A Method for Improving the Robustness of linear Kramers-Kronig Validity Tests DOI: https://doi.org/10.1016/j.electacta.2014.01.034
+- A Method for Improving the Robustness of linear Kramers-Kronig Validity Tests DOI: https://doi.org/10.1016/j.electacta.2014.01.034
+
+Acknowledgement
+~~~~~~~~~~~~~~~
+
+This project has received funding from the European Union’s [Horizon 2020 research and innovation programme](https://ec.europa.eu/programmes/horizon2020/en) under grant agreement [No 957189](https://cordis.europa.eu/project/id/957189). The project is part of BATTERY 2030+, the large-scale European research initiative for inventing the sustainable batteries of the future.
```

### Comparing `MADAP-0.9.0/docs/Makefile` & `MADAP-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `MADAP-0.9.0/docs/make.bat` & `MADAP-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `MADAP-0.9.0/docs/source/conf.py` & `MADAP-1.1.0/docs/source/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 
 import os
 import sys
-sys.path.insert(0, os.path.abspath(os.path.join("..","..", "src")))
-sys.path.insert(0, os.path.abspath(os.path.join("..","..","src","madap", "logger")))
-sys.path.insert(0, os.path.abspath(os.path.join("..","..","src","madap", "echem")))
+sys.path.insert(0, os.path.abspath("../.."))
+sys.path.insert(0, os.path.abspath(os.path.join("..","..","madap", "logger")))
+sys.path.insert(0, os.path.abspath(os.path.join("..","..","madap", "echem")))
 # -- Project information -----------------------------------------------------
 
 project = 'MADAP'
 copyright = '2022, Fuzhan Rahmanian'
 author = 'Fuzhan Rahmanian'
 
 # The full version, including alpha/beta/rc tags
```

### Comparing `MADAP-0.9.0/setup.py` & `MADAP-1.1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,48 +20,46 @@
         "impedance==1.4.1"]
 
 test_requirements = ['pytest>=3', ]
 
 setup(
     author="Fuzhan Rahmanian",
     author_email='fuzhanrahmanian@gmail.com',
-    python_requires='>=3.6',
+    python_requires='>=3.9',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Topic :: Scientific/Engineering :: Chemistry',
         'Topic :: Scientific/Engineering :: Physics',
         'Topic :: Scientific/Engineering :: Visualization',
     ],
     description="This is MADAP, a software package for the analysis of electrochemical data.",
     entry_points={
         'console_scripts': [
-            'cli=src.madap_cli:main',
-            'gui=src.madap_gui:main',
+            'madap_cli=madap_cli:main',
+            'madap_gui=madap_gui:main',
         ],
     },
     extras_require={
         "dev": ["pytest>=3", ],
     },
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='madap',
     name='MADAP',
-    packages=find_packages(include=['src', 'src.*']),
-    #package_dir = {'': 'src'},
+    packages=find_packages(),
+    py_modules=['madap_cli', 'madap_gui'],
+    package_data={'madap/plotting/styles': ['*.mplstyle']},
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/fuzhanrahmanian/MADAP',
-    version='0.9.0',
+    version='1.1.0',
     zip_safe=False,
 )
```

### Comparing `MADAP-0.9.0/src/madap/data_acquisition/data_acquisition.py` & `MADAP-1.1.0/madap/data_acquisition/data_acquisition.py`

 * *Files identical despite different names*

### Comparing `MADAP-0.9.0/src/madap/echem/arrhenius/arrhenius.py` & `MADAP-1.1.0/madap/echem/arrhenius/arrhenius.py`

 * *Files identical despite different names*

### Comparing `MADAP-0.9.0/src/madap/echem/arrhenius/arrhenius_plotting.py` & `MADAP-1.1.0/madap/echem/arrhenius/arrhenius_plotting.py`

 * *Files identical despite different names*

### Comparing `MADAP-0.9.0/src/madap/echem/e_impedance/e_impedance.py` & `MADAP-1.1.0/madap/echem/e_impedance/e_impedance.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,16 +91,18 @@
         self.eval_fit_linkk = None
         self.z_linkk = None
         self.res_real = None
         self.res_imag = None
         self.chi_val = None
         self.custom_circuit = None
         self.z_fit = None
+        self.z_fit_clean = None
         self.impedance.phase_shift = self._calculate_phase_shift() if self.impedance.phase_shift is None else self.impedance.phase_shift
         self.figure = None
+        self.pos_img_index = None
 
 
     # Schönleber, M. et al. A Method for Improving the Robustness of
     # linear Kramers-Kronig Validity Tests.
     # Electrochimica Acta 131, 20–27 (2014) doi: 10.1016/j.electacta.2014.01.034.
     def analyze(self):
         """General function for performing the impedance analysis.
@@ -116,14 +118,16 @@
                                                         max_M=self.max_rc_element,
                                                         fit_type=self.fit_type,
                                                         add_cap=self.val_low_freq)
         self.chi_val = self._chi_calculation()
         log.info(f"Chi value from lin_KK method is {self.chi_val}")
 
         if any(x < 0 for x in self.impedance.imaginary_impedance):
+            # Find the indexes of the positive values
+            self.pos_img_index = np.where(self.impedance.imaginary_impedance > 0)
             f_circuit, z_circuit = preprocessing.ignoreBelowX(f_circuit, z_circuit)
 
         # if the user did not choose any circuit, some default suggestions will be applied.
         if (self.suggested_circuit and self.initial_value) is None:
 
             for guess_circuit, guess_value in suggested_circuits.items():
                 # apply some random guess
@@ -256,18 +260,25 @@
         name = utils.assemble_file_name(optional_name, self.__class__.__name__, "circuit.json") if \
         optional_name else utils.assemble_file_name(self.__class__.__name__, "circuit.json")
 
         self.custom_circuit.save(os.path.join(save_dir, f"{name}"))
         added_data = {'rc_linKK': self.num_rc_linkk, "eval_fit_linKK": self.eval_fit_linkk, "RMSE_fit_error": self.rmse_calc,
                       "conductivity [S/cm]": self.conductivity, "chi_square": self.chi_val}
         utils.append_to_save_data(directory=save_dir, added_data=added_data, name=name)
+        # check if the positive index is available
+        if self.pos_img_index is not None:
+            self._insert_nan_values()
+        else:
+            self.z_fit_clean = self.z_fit
+
+
         # Save the dataset
         data = utils.assemble_data_frame(**{"frequency [Hz]": self.impedance.frequency,
                                             "impedance [\u03a9]": self.impedance.real_impedance + 1j*self.impedance.imaginary_impedance,
-                                            "fit_impedance [\u03a9]": self.z_fit, "residual_real":self.res_real, "residual_imag":self.res_imag,
+                                            "fit_impedance [\u03a9]": self.z_fit_clean, "residual_real":self.res_real, "residual_imag":self.res_imag,
                                             "Z_linKK [\u03a9]": self.z_linkk})
         data_name = utils.assemble_file_name(optional_name, self.__class__.__name__, "data.csv") if \
                         optional_name else  utils.assemble_file_name(self.__class__.__name__, "data.csv")
 
         utils.save_data_as_csv(save_dir, data, data_name)
 
     def perform_all_actions(self, save_dir:str, plots:list, optional_name:str = None):
@@ -344,14 +355,26 @@
         """
         guess_value = [guess_initial_resistance if element == 'x' else element for element in guess_value]
         guess_value = [guess_initial_resistance if element == 'y' else element for element in guess_value]
         guess_value = [guess_initial_resistance if element == 'z' else element for element in guess_value]
         guess_value = [guess_initial_resistance if element == 't' else element for element in guess_value]
         return guess_value
 
+    def _insert_nan_values(self):
+        """Insert nan values in the fit for the positive imaginary impedance values.
+        """
+        self.z_fit_clean = np.empty(len(self.z_fit) + len(self.pos_img_index[0]), dtype=np.complex128)
+        self.z_fit_clean[:] = np.nan
+        j = 0
+        for i in range(len(self.z_fit_clean)):
+            if i in self.pos_img_index[0].tolist():
+                continue
+            self.z_fit_clean[i] = self.z_fit[j]
+            j += 1
+
 class Mottschotcky(EIS, EChemProcedure):
     """ Class for performing the Mottschotcky procedure.
 
     Args:
         EIS (class): General EIS class
         EChemProcedure (class): General abstract EChem Procedure class
     """
```

### Comparing `MADAP-0.9.0/src/madap/echem/e_impedance/e_impedance_plotting.py` & `MADAP-1.1.0/madap/echem/e_impedance/e_impedance_plotting.py`

 * *Files identical despite different names*

### Comparing `MADAP-0.9.0/src/madap/echem/procedure.py` & `MADAP-1.1.0/madap/echem/procedure.py`

 * *Files identical despite different names*

### Comparing `MADAP-0.9.0/src/madap/echem/voltammetry/voltammetry_CA.py` & `MADAP-1.1.0/madap/echem/voltammetry/voltammetry_CA.py`

 * *Files identical despite different names*

### Comparing `MADAP-0.9.0/src/madap/echem/voltammetry/voltammetry_CP.py` & `MADAP-1.1.0/madap/echem/voltammetry/voltammetry_CP.py`

 * *Files identical despite different names*

### Comparing `MADAP-0.9.0/src/madap/echem/voltammetry/voltammetry_CV.py` & `MADAP-1.1.0/madap/echem/voltammetry/voltammetry_CV.py`

 * *Files identical despite different names*

### Comparing `MADAP-0.9.0/src/madap/echem/voltammetry/voltammetry_plotting.py` & `MADAP-1.1.0/madap/echem/voltammetry/voltammetry_plotting.py`

 * *Files identical despite different names*

### Comparing `MADAP-0.9.0/src/madap/logger/logger.py` & `MADAP-1.1.0/madap/logger/logger.py`

 * *Files identical despite different names*

### Comparing `MADAP-0.9.0/src/madap/plotting/plotting.py` & `MADAP-1.1.0/madap/plotting/plotting.py`

 * *Files identical despite different names*

### Comparing `MADAP-0.9.0/src/madap/plotting/styles/nature.mplstyle` & `MADAP-1.1.0/madap/plotting/styles/nature.mplstyle`

 * *Files identical despite different names*

### Comparing `MADAP-0.9.0/src/madap/plotting/styles/science.mplstyle` & `MADAP-1.1.0/madap/plotting/styles/science.mplstyle`

 * *Files identical despite different names*

### Comparing `MADAP-0.9.0/src/madap/utils/gui_elements.py` & `MADAP-1.1.0/madap/utils/gui_elements.py`

 * *Files identical despite different names*

### Comparing `MADAP-0.9.0/src/madap/utils/suggested_circuits.py` & `MADAP-1.1.0/madap/utils/suggested_circuits.py`

 * *Files identical despite different names*

### Comparing `MADAP-0.9.0/src/madap/utils/utils.py` & `MADAP-1.1.0/madap/utils/utils.py`

 * *Files identical despite different names*

### Comparing `MADAP-0.9.0/src/madap_cli.py` & `MADAP-1.1.0/madap_cli.py`

 * *Files identical despite different names*

### Comparing `MADAP-0.9.0/src/madap_gui.py` & `MADAP-1.1.0/madap_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
                              font=("Arial", 13), pad=(1,(20,0)))],
                     [sg.InputText(key="-upper_limit_quantile-", tooltip=gui_elements.UPPER_LIMIT_QUANTILE_HELP,
                                   enable_events=True, default_text="0.99")],
                     [sg.Text("Lower limit of quantile (optional)",justification='left',
                              font=("Arial", 13), pad=(1,(20,0)))],
                     [sg.InputText(key="-lower_limit_quantile-", tooltip=gui_elements.LOWER_LIMIT_QUANTILE_HELP,
                                   enable_events=True, default_text="0.01")],
-                    [sg.Text('Suggeted Circuit',justification='left', font=("Arial", 13),
+                    [sg.Text('Suggested Circuit',justification='left', font=("Arial", 13),
                              pad=(1,(20,0)))],
                     [sg.InputText(key="-suggested_circuit-", tooltip=gui_elements.SUGGESTED_CIRCUIT_HELP,
                                   default_text="R0-p(R1,CPE1)")],
                     [sg.Text('Initial Value', justification='left', font=("Arial", 13), pad=(1,(20,0)))],
                     [sg.InputText(key="-initial_value-", enable_events=True, tooltip=gui_elements.INITIAL_VALUES_HELP,
                                   default_text="[860, 3e+5, 1e-09, 0.90]")],
                     [sg.Text('Plots',justification='left', font=("Arial", 13), pad=(1,(20,0)))],
```

