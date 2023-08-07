# Comparing `tmp/LAM-0.4.6.tar.gz` & `tmp/LAM-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\LAM-0.4.6.tar", last modified: Mon Oct 11 22:38:22 2021, max compression
+gzip compressed data, was "dist\LAM-0.4.7.tar", last modified: Mon Aug  7 09:50:08 2023, max compression
```

## Comparing `LAM-0.4.6.tar` & `LAM-0.4.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2021-10-11 22:38:22.711555 LAM-0.4.6/
-drwxrwxrwx   0        0        0        0 2021-10-11 22:38:22.582742 LAM-0.4.6/LAM.egg-info/
--rw-rw-rw-   0        0        0     6097 2021-10-11 22:38:22.000000 LAM-0.4.6/LAM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      715 2021-10-11 22:38:22.000000 LAM-0.4.6/LAM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-10-11 22:38:22.000000 LAM-0.4.6/LAM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2021-10-11 22:38:22.000000 LAM-0.4.6/LAM.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      160 2021-10-11 22:38:22.000000 LAM-0.4.6/LAM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2021-10-11 22:38:22.000000 LAM-0.4.6/LAM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2020-06-14 20:56:23.000000 LAM-0.4.6/LICENSE.md
--rw-rw-rw-   0        0        0      147 2021-04-20 09:16:14.000000 LAM-0.4.6/MANIFEST.in
--rw-rw-rw-   0        0        0     6097 2021-10-11 22:38:22.711555 LAM-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     4981 2021-08-02 13:41:09.000000 LAM-0.4.6/README.md
-drwxrwxrwx   0        0        0        0 2021-10-11 22:38:22.603779 LAM-0.4.6/comp/
--rw-rw-rw-   0        0        0     3678 2021-01-13 09:05:40.000000 LAM-0.4.6/comp/ChannelPositionPlots.py
--rw-rw-rw-   0        0        0     4755 2021-04-30 05:24:54.000000 LAM-0.4.6/comp/ManualVectorPlots.py
--rw-rw-rw-   0        0        0     3028 2021-10-06 18:07:23.000000 LAM-0.4.6/comp/SubsetDataChannel.py
--rw-rw-rw-   0        0        0     8747 2020-08-06 09:48:48.000000 LAM-0.4.6/comp/combineSets.py
--rw-rw-rw-   0        0        0     5189 2020-03-31 16:45:32.000000 LAM-0.4.6/comp/rotator.py
--rw-rw-rw-   0        0        0      633 2021-04-20 09:16:14.000000 LAM-0.4.6/comp/script_descriptions.txt
--rw-rw-rw-   0        0        0    15043 2020-10-14 17:12:47.000000 LAM-0.4.6/comp/split_dataset.py
-drwxrwxrwx   0        0        0        0 2021-10-11 22:38:22.655502 LAM-0.4.6/docs/
--rw-rw-rw-   0        0        0     3346 2020-06-30 12:32:50.000000 LAM-0.4.6/docs/CommandLineArgs.txt
--rw-rw-rw-   0        0        0   717065 2021-08-04 08:18:15.000000 LAM-0.4.6/docs/UserManual_v0.4.3.pdf
-drwxrwxrwx   0        0        0        0 2021-10-11 22:38:22.657506 LAM-0.4.6/img/
--rw-rw-rw-   0        0        0    54454 2020-12-08 11:59:13.000000 LAM-0.4.6/img/lam.ico
--rw-rw-rw-   0        0        0      105 2021-06-28 15:09:27.000000 LAM-0.4.6/pyproject.toml
--rw-rw-rw-   0        0        0     1741 2021-10-11 22:38:22.712556 LAM-0.4.6/setup.cfg
--rw-rw-rw-   0        0        0       71 2020-10-07 09:12:48.000000 LAM-0.4.6/setup.py
-drwxrwxrwx   0        0        0        0 2021-10-11 22:38:22.710553 LAM-0.4.6/src/
--rw-rw-rw-   0        0        0      363 2020-10-23 08:24:12.000000 LAM-0.4.6/src/__init__.py
--rw-rw-rw-   0        0        0    34819 2021-10-11 21:33:52.000000 LAM-0.4.6/src/analysis.py
--rw-rw-rw-   0        0        0    28310 2021-09-22 19:14:17.000000 LAM-0.4.6/src/border_detect.py
--rw-rw-rw-   0        0        0    52813 2021-10-11 22:21:02.000000 LAM-0.4.6/src/interface.py
--rw-rw-rw-   0        0        0     9824 2020-10-27 08:15:36.000000 LAM-0.4.6/src/logger.py
--rw-rw-rw-   0        0        0     7569 2020-10-27 08:15:36.000000 LAM-0.4.6/src/parse_cmds.py
--rw-rw-rw-   0        0        0    35293 2021-04-20 09:56:10.000000 LAM-0.4.6/src/plot.py
--rw-rw-rw-   0        0        0    12201 2021-09-22 18:37:39.000000 LAM-0.4.6/src/plotfuncs.py
--rw-rw-rw-   0        0        0    44204 2021-08-03 13:10:48.000000 LAM-0.4.6/src/process.py
--rw-rw-rw-   0        0        0     2679 2020-10-23 10:21:11.000000 LAM-0.4.6/src/redirect.py
--rw-rw-rw-   0        0        0     8774 2021-08-04 08:01:52.000000 LAM-0.4.6/src/run.py
--rw-rw-rw-   0        0        0    10123 2021-09-20 12:43:38.000000 LAM-0.4.6/src/settings.py
--rw-rw-rw-   0        0        0     9425 2021-08-04 07:53:25.000000 LAM-0.4.6/src/statsMWW.py
--rw-rw-rw-   0        0        0    16318 2021-03-24 07:46:43.000000 LAM-0.4.6/src/system.py
--rw-rw-rw-   0        0        0     8162 2021-04-20 09:16:14.000000 LAM-0.4.6/src/vector_loop.py
--rw-rw-rw-   0        0        0       21 2021-10-11 21:35:31.000000 LAM-0.4.6/src/version.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:50:08.094145 LAM-0.4.7/
+drwxrwxrwx   0        0        0        0 2023-08-07 09:50:07.964017 LAM-0.4.7/LAM.egg-info/
+-rw-rw-rw-   0        0        0     7727 2023-08-07 09:50:07.000000 LAM-0.4.7/LAM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2023-08-07 09:50:07.000000 LAM-0.4.7/LAM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 09:50:07.000000 LAM-0.4.7/LAM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-08-07 09:50:07.000000 LAM-0.4.7/LAM.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      164 2023-08-07 09:50:07.000000 LAM-0.4.7/LAM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-07 09:50:07.000000 LAM-0.4.7/LAM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2020-06-14 20:56:23.000000 LAM-0.4.7/LICENSE.md
+-rw-rw-rw-   0        0        0      147 2021-04-20 09:16:14.000000 LAM-0.4.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     7727 2023-08-07 09:50:08.095147 LAM-0.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6550 2023-08-07 09:29:53.000000 LAM-0.4.7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 09:50:08.040730 LAM-0.4.7/comp/
+-rw-rw-rw-   0        0        0     3678 2021-01-13 09:05:40.000000 LAM-0.4.7/comp/ChannelPositionPlots.py
+-rw-rw-rw-   0        0        0     4755 2021-04-30 05:24:54.000000 LAM-0.4.7/comp/ManualVectorPlots.py
+-rw-rw-rw-   0        0        0     2977 2023-08-07 09:17:28.000000 LAM-0.4.7/comp/SubsetDataChannel.py
+-rw-rw-rw-   0        0        0     8747 2023-08-07 09:12:12.000000 LAM-0.4.7/comp/combineSets.py
+-rw-rw-rw-   0        0        0     5189 2020-03-31 16:45:32.000000 LAM-0.4.7/comp/rotator.py
+-rw-rw-rw-   0        0        0      633 2021-04-20 09:16:14.000000 LAM-0.4.7/comp/script_descriptions.txt
+-rw-rw-rw-   0        0        0    15043 2020-10-14 17:12:47.000000 LAM-0.4.7/comp/split_dataset.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:50:08.055368 LAM-0.4.7/docs/
+-rw-rw-rw-   0        0        0     3346 2020-06-30 12:32:50.000000 LAM-0.4.7/docs/CommandLineArgs.txt
+-rw-rw-rw-   0        0        0   717065 2021-08-04 08:18:15.000000 LAM-0.4.7/docs/UserManual_v0.4.3.pdf
+drwxrwxrwx   0        0        0        0 2023-08-07 09:50:08.075866 LAM-0.4.7/img/
+-rw-rw-rw-   0        0        0    54454 2020-12-08 11:59:13.000000 LAM-0.4.7/img/lam.ico
+-rw-rw-rw-   0        0        0      105 2021-06-28 15:09:27.000000 LAM-0.4.7/pyproject.toml
+-rw-rw-rw-   0        0        0     1827 2023-08-07 09:50:08.096148 LAM-0.4.7/setup.cfg
+-rw-rw-rw-   0        0        0       71 2020-10-07 09:12:48.000000 LAM-0.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:50:08.093145 LAM-0.4.7/src/
+-rw-rw-rw-   0        0        0      363 2020-10-23 08:24:12.000000 LAM-0.4.7/src/__init__.py
+-rw-rw-rw-   0        0        0    34670 2023-08-07 09:29:53.000000 LAM-0.4.7/src/analysis.py
+-rw-rw-rw-   0        0        0    28262 2023-08-07 09:29:53.000000 LAM-0.4.7/src/border_detect.py
+-rw-rw-rw-   0        0        0    52813 2023-08-07 08:52:20.000000 LAM-0.4.7/src/interface.py
+-rw-rw-rw-   0        0        0     9824 2020-10-27 08:15:36.000000 LAM-0.4.7/src/logger.py
+-rw-rw-rw-   0        0        0     7560 2023-08-07 09:29:53.000000 LAM-0.4.7/src/parse_cmds.py
+-rw-rw-rw-   0        0        0    35412 2023-08-07 09:29:53.000000 LAM-0.4.7/src/plot.py
+-rw-rw-rw-   0        0        0    12186 2023-08-07 09:29:53.000000 LAM-0.4.7/src/plotfuncs.py
+-rw-rw-rw-   0        0        0    43826 2023-08-07 09:29:53.000000 LAM-0.4.7/src/process.py
+-rw-rw-rw-   0        0        0     2679 2020-10-23 10:21:11.000000 LAM-0.4.7/src/redirect.py
+-rw-rw-rw-   0        0        0     8774 2023-08-07 08:43:59.000000 LAM-0.4.7/src/run.py
+-rw-rw-rw-   0        0        0    10123 2021-09-20 12:43:38.000000 LAM-0.4.7/src/settings.py
+-rw-rw-rw-   0        0        0     8813 2023-08-07 09:29:53.000000 LAM-0.4.7/src/statsMWW.py
+-rw-rw-rw-   0        0        0    16730 2023-08-07 09:29:53.000000 LAM-0.4.7/src/system.py
+-rw-rw-rw-   0        0        0     8162 2021-04-20 09:16:14.000000 LAM-0.4.7/src/vector_loop.py
+-rw-rw-rw-   0        0        0       21 2023-08-07 09:29:53.000000 LAM-0.4.7/src/version.py
```

### Comparing `LAM-0.4.6/LAM.egg-info/PKG-INFO` & `LAM-0.4.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: LAM
-Version: 0.4.6
-Summary: Linear Analysis of Midgut
-Home-page: UNKNOWN
-Author: Arto I. Viitanen
-Author-email: arto.viitanen@helsinki.fi
-License: GPL-3.0 License
-Project-URL: Project, https://github.com/hietakangas-laboratory/LAM
-Project-URL: Bug Reports, https://github.com/hietakangas-laboratory/LAM/issues
-Project-URL: Tutorial Videos, https://www.youtube.com/playlist?list=PLjv-8Gzxh3AynUtI3HaahU2oddMbDpgtx
-Project-URL: Publication, https://doi.org/10.1016/j.crmeth.2021.100059
-Project-URL: Research Group, https://www.helsinki.fi/en/researchgroups/nutrient-sensing
-Keywords: biology,data analysis,image object data
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: <3.9,>=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 ![](/img/lam.ico)
 
 # Linear Analysis of Midgut
 ### ---------------LAM---------------
 
 Linear Analysis of Midgut (LAM) is a tool for reducing the dimensionality of microscopy image–obtained data, and for
 subsequent quantification of variables and object counts while preserving spatial context. LAM’s intended use is to
@@ -35,54 +10,91 @@
 along the whole length of the midgut for multiple sample groups. Additionally, LAM has algorithms for the estimation of
 feature-to-feature nearest distances and for the detection of cell clusters, both of which also retain the regional
 context. LAM also approximates sample widths and can perform multivariate border-region detection on sample groups. The
 analysis is performed after image processing and object detection. Consequently, LAM requires coordinate data of the
 features as input.
 
 ### Installation
-LAM is used in a Python (>=3.7, <3.9) environment and can be found on PyPI. It can be installed with command
-**pip install lam**. Note that by installing this way, you will be restricted to the settings on the GUI and/or the
-available command line arguments, and will not be able to alter settings.py.
-
-You can alternatively install LAM from command line using the 'setup.py' by giving command:
-'python setup.py install' while located inside the LAM-master -directory. Windows-users are recommended to install
-Shapely>=1.7.0 from a pre-compiled wheel found [here](https://www.lfd.uci.edu/~gohlke/pythonlibs/#shapely) in order to
-properly link GEOS and cython. The wheel can be installed with **pip install path/to/wheel**.
-
-The distribution also includes docs/requirements.txt and docs/LAMenv.yml that can be used to install dependencies using
-pip or conda (Anaconda), respectively. Recommendation is to install LAM into its own virtual environment.
+LAM can be used in a Python (>=3.7, <=3.11) environment and can be found on PyPI. Recommendation is to install LAM into
+its own virtual environment. An easy and functional way to prepare the LAM-environment is by using the "recipe"-file,
+LAMenv.yml, to create a conda environment ([Download Anaconda](https://www.anaconda.com/download/)). Simply, in
+'Anaconda Prompt' give the following commands using functional path (e.g. <samp>"D:\user\LAM-master\LAMenv.yml"</samp>):
+```console
+conda env create -n lamenv -f="Path/To/LAM-master/LAMenv.yml"
+conda activate lamenv
+# [OPTIONAL]: pip install lam
+```
+
+As a PyPI-package, LAM can be installed with the command `pip install lam`. Installing LAM enables launching the
+graphical user interface (GUI) via prompt command `lam-run`. However, installing this way disables direct editing of
+<samp>"src/settings.py"</samp> and consequently restricts LAM to the settings available on the GUI and/or command line.
+However, a separate LAM-master **can be edited** and then be executed in the environment with command
+`python "Path/To/Alternate/src/run.py"`.
+
+LAM can alternatively be installed from command line using the 'setup.py' by giving command: `python setup.py install`
+while located inside the LAM-master -directory. ~~Windows-users are recommended to install Shapely>=1.7.0 from a
+pre-compiled wheel found [here](https://www.lfd.uci.edu/~gohlke/pythonlibs/#shapely) in order to properly link GEOS and
+cython. The wheel can be installed with **pip install path/to/wheel**.~~
 
-### Usage
-LAM is used by executing 'src/run.py' or with console command 'lam-run', both of which by default open up the graphical
-user interface. Settings can be handled through src/settings.py, but LAM also includes argument parsing for most
-important settings ('python src/run.py -h' OR 'lam-run -h'). Refer to 'docs/UserManual' for additional information.
-Several modules related to forming LAM-compatible folder structures can be found
-[here](https://github.com/hietakangas-laboratory/LAM-helper-modules).
+- UPDATE, 2023: conda installations of Shapely **are functional** for Windows.
 
-A video tutorial series on LAM can be found on YouTube
-[here](https://www.youtube.com/playlist?list=PLjv-8Gzxh3AynUtI3HaahU2oddMbDpgtx).
+---
 
-Hietakangas lab also provides a stitching script that uses ImageJ to properly stitch tile scan images for object
+### Usage
+LAM is used by executing <samp>"src/run.py"</samp> or with console command `lam-run`, both of which by default open up
+the GUI. Settings can be handled through <samp>src/settings.py</samp>, but LAM also includes argument parsing for most
+important settings (`python src/run.py -h` or `lam-run -h`). Refer to <samp>'docs/UserManual'</samp> for additional
+information.
+
+#### Run examples
+
+Note that many of LAM's command line arguments are toggles that switch the settings from their default behaviour as
+defined in <samp>"src/settings.py"</samp>. This allows for better customization when for example designing batch files
+(see <samp>"docs/run_split_count.bat"</samp>).
+
+```console
+# IN LAM ENVIRONMENT:
+# Launch GUI with default settings
+lam-run
+
+# Project and count the dataset at given path without GUI and bypassing user prompts (Linux path).
+lam-run -p ~/datasets/lam-data -o c -GD
+
+# Perform Count, Plots and Stats using 50 bins, and on input files with column names on the third row.  
+lam-run -p "D:\user\LAM-master\data" -o cls -b 50 -H 2
+
+# Launch GUI of a non-installed version of LAM and specify path to dataset
+python "D:\user\LAM-master\src\run.py" -p "D:\user\LAM-master\data"
+```
+
+#### Related material
+A video tutorial series on LAM can be found on
+YouTube [here](https://www.youtube.com/playlist?list=PLjv-8Gzxh3AynUtI3HaahU2oddMbDpgtx). Several modules related to
+forming LAM-compatible folder structures can be found
+[here](https://github.com/hietakangas-laboratory/LAM-helper-modules). Hietakangas lab also provides a stitching script that uses ImageJ to properly stitch tile scan images for object
 detection and following LAM analysis. The script can be found [here](https://github.com/hietakangas-laboratory/Stitch).
 
 For object segmentation and/or acquirement of label information, we also provide a wrapper package for
 [StarDist](https://github.com/stardist/stardist) called [predictSD](https://github.com/hietakangas-laboratory/predictSD)
 that includes several 3D deep learning models that have been trained on images from Aurox spinning disc confocal. The
 package can extract label information in a format that is directly usable by LAM.
 
+---
 ### Test data
 The 'data/'-directory includes a small test dataset of two sample groups with four samples each. Note that the
 sample number is not enough for a proper analysis; in ideal circumstances, it is recommended that each sample group
 should have >=10 samples. Refer to user-manual for additional information.
 
+---
 ### Publication
 * Viitanen, A., Gullmets, J., Morikka, J., Katajisto, P., Mattila, J., & Hietakangas, V. (2021). An image analysis method
 for regionally defined cellular phenotyping of the Drosophila midgut. Cell Reports Methods, Sep 27th.
 https://doi.org/10.1016/j.crmeth.2021.100059
-  
+
+---
 ### Additional Resources
 * [LAM helper modules](https://github.com/hietakangas-laboratory/LAM-helper-modules) - organize data for LAM input
 * [LAM tutorial videos](https://www.youtube.com/playlist?list=PLjv-8Gzxh3AynUtI3HaahU2oddMbDpgtx)
 * [predictSD](https://github.com/hietakangas-laboratory/predictSD) - a wrapper and some models for running
   [StarDist](https://github.com/stardist/stardist) segmentation with LAM-compatible output
 * [Stitch](https://github.com/hietakangas-laboratory/Stitch) - Tile scan image stitching
 
@@ -91,9 +103,7 @@
 
 ### Authors
 * Arto I. Viitanen - [Hietakangas laboratory](https://www.helsinki.fi/en/researchgroups/nutrient-sensing)
 
 ### Acknowledgments
 * Ville Hietakangas - [Hietakangas laboratory](https://www.helsinki.fi/en/researchgroups/nutrient-sensing/)
 * Jaakko Mattila - [Mattila laboratory](https://www.helsinki.fi/en/researchgroups/metabolism-and-signaling/)
-
-
```

### Comparing `LAM-0.4.6/LAM.egg-info/SOURCES.txt` & `LAM-0.4.7/LAM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LAM-0.4.6/LICENSE.md` & `LAM-0.4.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `LAM-0.4.6/PKG-INFO` & `LAM-0.4.7/LAM.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: LAM
-Version: 0.4.6
+Version: 0.4.7
 Summary: Linear Analysis of Midgut
-Home-page: UNKNOWN
 Author: Arto I. Viitanen
 Author-email: arto.viitanen@helsinki.fi
 License: GPL-3.0 License
 Project-URL: Project, https://github.com/hietakangas-laboratory/LAM
 Project-URL: Bug Reports, https://github.com/hietakangas-laboratory/LAM/issues
 Project-URL: Tutorial Videos, https://www.youtube.com/playlist?list=PLjv-8Gzxh3AynUtI3HaahU2oddMbDpgtx
 Project-URL: Publication, https://doi.org/10.1016/j.crmeth.2021.100059
 Project-URL: Research Group, https://www.helsinki.fi/en/researchgroups/nutrient-sensing
 Keywords: biology,data analysis,image object data
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: <3.9,>=3.7
+Requires-Python: <=3.11,>3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 ![](/img/lam.ico)
 
 # Linear Analysis of Midgut
 ### ---------------LAM---------------
@@ -35,54 +35,91 @@
 along the whole length of the midgut for multiple sample groups. Additionally, LAM has algorithms for the estimation of
 feature-to-feature nearest distances and for the detection of cell clusters, both of which also retain the regional
 context. LAM also approximates sample widths and can perform multivariate border-region detection on sample groups. The
 analysis is performed after image processing and object detection. Consequently, LAM requires coordinate data of the
 features as input.
 
 ### Installation
-LAM is used in a Python (>=3.7, <3.9) environment and can be found on PyPI. It can be installed with command
-**pip install lam**. Note that by installing this way, you will be restricted to the settings on the GUI and/or the
-available command line arguments, and will not be able to alter settings.py.
-
-You can alternatively install LAM from command line using the 'setup.py' by giving command:
-'python setup.py install' while located inside the LAM-master -directory. Windows-users are recommended to install
-Shapely>=1.7.0 from a pre-compiled wheel found [here](https://www.lfd.uci.edu/~gohlke/pythonlibs/#shapely) in order to
-properly link GEOS and cython. The wheel can be installed with **pip install path/to/wheel**.
+LAM can be used in a Python (>=3.7, <=3.11) environment and can be found on PyPI. Recommendation is to install LAM into
+its own virtual environment. An easy and functional way to prepare the LAM-environment is by using the "recipe"-file,
+LAMenv.yml, to create a conda environment ([Download Anaconda](https://www.anaconda.com/download/)). Simply, in
+'Anaconda Prompt' give the following commands using functional path (e.g. <samp>"D:\user\LAM-master\LAMenv.yml"</samp>):
+```console
+conda env create -n lamenv -f="Path/To/LAM-master/LAMenv.yml"
+conda activate lamenv
+# [OPTIONAL]: pip install lam
+```
+
+As a PyPI-package, LAM can be installed with the command `pip install lam`. Installing LAM enables launching the
+graphical user interface (GUI) via prompt command `lam-run`. However, installing this way disables direct editing of
+<samp>"src/settings.py"</samp> and consequently restricts LAM to the settings available on the GUI and/or command line.
+However, a separate LAM-master **can be edited** and then be executed in the environment with command
+`python "Path/To/Alternate/src/run.py"`.
+
+LAM can alternatively be installed from command line using the 'setup.py' by giving command: `python setup.py install`
+while located inside the LAM-master -directory. ~~Windows-users are recommended to install Shapely>=1.7.0 from a
+pre-compiled wheel found [here](https://www.lfd.uci.edu/~gohlke/pythonlibs/#shapely) in order to properly link GEOS and
+cython. The wheel can be installed with **pip install path/to/wheel**.~~
 
-The distribution also includes docs/requirements.txt and docs/LAMenv.yml that can be used to install dependencies using
-pip or conda (Anaconda), respectively. Recommendation is to install LAM into its own virtual environment.
+- UPDATE, 2023: conda installations of Shapely **are functional** for Windows.
 
-### Usage
-LAM is used by executing 'src/run.py' or with console command 'lam-run', both of which by default open up the graphical
-user interface. Settings can be handled through src/settings.py, but LAM also includes argument parsing for most
-important settings ('python src/run.py -h' OR 'lam-run -h'). Refer to 'docs/UserManual' for additional information.
-Several modules related to forming LAM-compatible folder structures can be found
-[here](https://github.com/hietakangas-laboratory/LAM-helper-modules).
-
-A video tutorial series on LAM can be found on YouTube
-[here](https://www.youtube.com/playlist?list=PLjv-8Gzxh3AynUtI3HaahU2oddMbDpgtx).
+---
 
-Hietakangas lab also provides a stitching script that uses ImageJ to properly stitch tile scan images for object
+### Usage
+LAM is used by executing <samp>"src/run.py"</samp> or with console command `lam-run`, both of which by default open up
+the GUI. Settings can be handled through <samp>src/settings.py</samp>, but LAM also includes argument parsing for most
+important settings (`python src/run.py -h` or `lam-run -h`). Refer to <samp>'docs/UserManual'</samp> for additional
+information.
+
+#### Run examples
+
+Note that many of LAM's command line arguments are toggles that switch the settings from their default behaviour as
+defined in <samp>"src/settings.py"</samp>. This allows for better customization when for example designing batch files
+(see <samp>"docs/run_split_count.bat"</samp>).
+
+```console
+# IN LAM ENVIRONMENT:
+# Launch GUI with default settings
+lam-run
+
+# Project and count the dataset at given path without GUI and bypassing user prompts (Linux path).
+lam-run -p ~/datasets/lam-data -o c -GD
+
+# Perform Count, Plots and Stats using 50 bins, and on input files with column names on the third row.  
+lam-run -p "D:\user\LAM-master\data" -o cls -b 50 -H 2
+
+# Launch GUI of a non-installed version of LAM and specify path to dataset
+python "D:\user\LAM-master\src\run.py" -p "D:\user\LAM-master\data"
+```
+
+#### Related material
+A video tutorial series on LAM can be found on
+YouTube [here](https://www.youtube.com/playlist?list=PLjv-8Gzxh3AynUtI3HaahU2oddMbDpgtx). Several modules related to
+forming LAM-compatible folder structures can be found
+[here](https://github.com/hietakangas-laboratory/LAM-helper-modules). Hietakangas lab also provides a stitching script that uses ImageJ to properly stitch tile scan images for object
 detection and following LAM analysis. The script can be found [here](https://github.com/hietakangas-laboratory/Stitch).
 
 For object segmentation and/or acquirement of label information, we also provide a wrapper package for
 [StarDist](https://github.com/stardist/stardist) called [predictSD](https://github.com/hietakangas-laboratory/predictSD)
 that includes several 3D deep learning models that have been trained on images from Aurox spinning disc confocal. The
 package can extract label information in a format that is directly usable by LAM.
 
+---
 ### Test data
 The 'data/'-directory includes a small test dataset of two sample groups with four samples each. Note that the
 sample number is not enough for a proper analysis; in ideal circumstances, it is recommended that each sample group
 should have >=10 samples. Refer to user-manual for additional information.
 
+---
 ### Publication
 * Viitanen, A., Gullmets, J., Morikka, J., Katajisto, P., Mattila, J., & Hietakangas, V. (2021). An image analysis method
 for regionally defined cellular phenotyping of the Drosophila midgut. Cell Reports Methods, Sep 27th.
 https://doi.org/10.1016/j.crmeth.2021.100059
-  
+
+---
 ### Additional Resources
 * [LAM helper modules](https://github.com/hietakangas-laboratory/LAM-helper-modules) - organize data for LAM input
 * [LAM tutorial videos](https://www.youtube.com/playlist?list=PLjv-8Gzxh3AynUtI3HaahU2oddMbDpgtx)
 * [predictSD](https://github.com/hietakangas-laboratory/predictSD) - a wrapper and some models for running
   [StarDist](https://github.com/stardist/stardist) segmentation with LAM-compatible output
 * [Stitch](https://github.com/hietakangas-laboratory/Stitch) - Tile scan image stitching
 
@@ -91,9 +128,7 @@
 
 ### Authors
 * Arto I. Viitanen - [Hietakangas laboratory](https://www.helsinki.fi/en/researchgroups/nutrient-sensing)
 
 ### Acknowledgments
 * Ville Hietakangas - [Hietakangas laboratory](https://www.helsinki.fi/en/researchgroups/nutrient-sensing/)
 * Jaakko Mattila - [Mattila laboratory](https://www.helsinki.fi/en/researchgroups/metabolism-and-signaling/)
-
-
```

### Comparing `LAM-0.4.6/comp/ChannelPositionPlots.py` & `LAM-0.4.7/comp/ChannelPositionPlots.py`

 * *Files identical despite different names*

### Comparing `LAM-0.4.6/comp/ManualVectorPlots.py` & `LAM-0.4.7/comp/ManualVectorPlots.py`

 * *Files identical despite different names*

### Comparing `LAM-0.4.6/comp/SubsetDataChannel.py` & `LAM-0.4.7/comp/SubsetDataChannel.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,25 +29,24 @@
 @author: Arto I. Viitanen
 """
 
 import pandas as pd
 import pathlib as pl
 
 # Give path to the analysis root directory:
-analysis_path = pl.Path(r'E:\Code_folder\DSS_no_split_points')
+analysis_path = pl.Path(r'E:\Code_folder\ALLSTATS')
 
 # Give name of data-file to subset
-data_channel = 'GFP.csv'
+data_channel = 'DAPI.csv'
 
 # Give filtering expressions to subset the data.
-# filtering = ['Area > 100', '`Intensity_Mean_Ch=2` <= 10']
-filtering = ['`Nearest_ID_Delta` > 0']
+filtering = ['Area > 100', '`Intensity_Mean_Ch=2` <= 10']
 
 # Give name for output-file.
-output_file = 'GFP_subset.csv'
+output_file = 'DAPI_subset.csv'
 
 
 def subset_data(paths: [pl.Path], file: str, filters: [str], filename: str):
     """Create a subset of a datachannel based on filter expressions."""
     for path in paths:  # Loop all sample-folders
         print(path.name)
         save_path = path.joinpath(filename)
```

### Comparing `LAM-0.4.6/comp/combineSets.py` & `LAM-0.4.7/comp/combineSets.py`

 * *Files identical despite different names*

### Comparing `LAM-0.4.6/comp/rotator.py` & `LAM-0.4.7/comp/rotator.py`

 * *Files identical despite different names*

### Comparing `LAM-0.4.6/comp/script_descriptions.txt` & `LAM-0.4.7/comp/script_descriptions.txt`

 * *Files identical despite different names*

### Comparing `LAM-0.4.6/comp/split_dataset.py` & `LAM-0.4.7/comp/split_dataset.py`

 * *Files identical despite different names*

### Comparing `LAM-0.4.6/docs/CommandLineArgs.txt` & `LAM-0.4.7/docs/CommandLineArgs.txt`

 * *Files identical despite different names*

### Comparing `LAM-0.4.6/docs/UserManual_v0.4.3.pdf` & `LAM-0.4.7/docs/UserManual_v0.4.3.pdf`

 * *Files identical despite different names*

### Comparing `LAM-0.4.6/img/lam.ico` & `LAM-0.4.7/img/lam.ico`

 * *Files identical despite different names*

### Comparing `LAM-0.4.6/setup.cfg` & `LAM-0.4.7/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -28,82 +28,88 @@
 000001b0: 6d61 7469 6373 0d0a 0950 726f 6772 616d  matics...Program
 000001c0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
 000001d0: 2050 7974 686f 6e20 3a3a 2033 2e37 0d0a   Python :: 3.7..
 000001e0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
 000001f0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
 00000200: 3a3a 2033 2e38 0d0a 0950 726f 6772 616d  :: 3.8...Program
 00000210: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000220: 2050 7974 686f 6e20 3a3a 2033 203a 3a20   Python :: 3 :: 
-00000230: 4f6e 6c79 0d0a 6b65 7977 6f72 6473 203d  Only..keywords =
-00000240: 200d 0a09 6269 6f6c 6f67 790d 0a09 6461   ...biology...da
-00000250: 7461 2061 6e61 6c79 7369 730d 0a09 696d  ta analysis...im
-00000260: 6167 6520 6f62 6a65 6374 2064 6174 610d  age object data.
-00000270: 0a70 726f 6a65 6374 5f75 726c 7320 3d20  .project_urls = 
-00000280: 0d0a 0950 726f 6a65 6374 203d 2068 7474  ...Project = htt
-00000290: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000002a0: 6869 6574 616b 616e 6761 732d 6c61 626f  hietakangas-labo
-000002b0: 7261 746f 7279 2f4c 414d 0d0a 0942 7567  ratory/LAM...Bug
-000002c0: 2052 6570 6f72 7473 203d 2068 7474 7073   Reports = https
-000002d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6869  ://github.com/hi
-000002e0: 6574 616b 616e 6761 732d 6c61 626f 7261  etakangas-labora
-000002f0: 746f 7279 2f4c 414d 2f69 7373 7565 730d  tory/LAM/issues.
-00000300: 0a09 5475 746f 7269 616c 2056 6964 656f  ..Tutorial Video
-00000310: 7320 3d20 6874 7470 733a 2f2f 7777 772e  s = https://www.
-00000320: 796f 7574 7562 652e 636f 6d2f 706c 6179  youtube.com/play
-00000330: 6c69 7374 3f6c 6973 743d 504c 6a76 2d38  list?list=PLjv-8
-00000340: 477a 7868 3341 796e 5574 4933 4861 6168  Gzxh3AynUtI3Haah
-00000350: 5532 6f64 644d 6244 7067 7478 0d0a 0950  U2oddMbDpgtx...P
-00000360: 7562 6c69 6361 7469 6f6e 203d 2068 7474  ublication = htt
-00000370: 7073 3a2f 2f64 6f69 2e6f 7267 2f31 302e  ps://doi.org/10.
-00000380: 3130 3136 2f6a 2e63 726d 6574 682e 3230  1016/j.crmeth.20
-00000390: 3231 2e31 3030 3035 390d 0a09 5265 7365  21.100059...Rese
-000003a0: 6172 6368 2047 726f 7570 203d 2068 7474  arch Group = htt
-000003b0: 7073 3a2f 2f77 7777 2e68 656c 7369 6e6b  ps://www.helsink
-000003c0: 692e 6669 2f65 6e2f 7265 7365 6172 6368  i.fi/en/research
-000003d0: 6772 6f75 7073 2f6e 7574 7269 656e 742d  groups/nutrient-
-000003e0: 7365 6e73 696e 670d 0a0d 0a5b 6f70 7469  sensing....[opti
-000003f0: 6f6e 735d 0d0a 7061 636b 6167 6573 203d  ons]..packages =
-00000400: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
-00000410: 6571 7569 7265 7320 3d20 0d0a 093e 3d33  equires = ...>=3
-00000420: 2e37 2c20 3c33 2e39 0d0a 696e 7374 616c  .7, <3.9..instal
-00000430: 6c5f 7265 7175 6972 6573 203d 200d 0a09  l_requires = ...
-00000440: 6e75 6d70 793e 3d31 2e31 380d 0a09 7061  numpy>=1.18...pa
-00000450: 6e64 6173 3e3d 312e 310d 0a09 6d61 7470  ndas>=1.1...matp
-00000460: 6c6f 746c 6962 3e3d 332e 312e 330d 0a09  lotlib>=3.1.3...
-00000470: 7061 7468 6c69 6232 3e3d 322e 330d 0a09  pathlib2>=2.3...
-00000480: 7363 6970 793e 3d31 2e35 0d0a 0973 6561  scipy>=1.5...sea
-00000490: 626f 726e 3e3d 302e 3131 2e30 0d0a 0973  born>=0.11.0...s
-000004a0: 6861 7065 6c79 3e3d 312e 372e 300d 0a09  hapely>=1.7.0...
-000004b0: 7363 696b 6974 2d69 6d61 6765 3e3d 302e  scikit-image>=0.
-000004c0: 3136 2e32 0d0a 0973 6369 6b69 742d 6c65  16.2...scikit-le
-000004d0: 6172 6e3e 3d30 2e32 322e 310d 0a09 7374  arn>=0.22.1...st
-000004e0: 6174 736d 6f64 656c 733e 3d30 2e31 312e  atsmodels>=0.11.
-000004f0: 300d 0a0d 0a5b 6f70 7469 6f6e 732e 6461  0....[options.da
-00000500: 7461 5f66 696c 6573 5d0d 0a69 6d67 203d  ta_files]..img =
-00000510: 200d 0a09 696d 672f 6c61 6d2e 6963 6f0d   ...img/lam.ico.
-00000520: 0a64 6f63 7320 3d20 0d0a 0952 4541 444d  .docs = ...READM
-00000530: 452e 6d64 0d0a 094c 4943 454e 5345 2e6d  E.md...LICENSE.m
-00000540: 640d 0a09 646f 6373 2f43 6f6d 6d61 6e64  d...docs/Command
-00000550: 4c69 6e65 4172 6773 2e74 7874 0d0a 0964  LineArgs.txt...d
-00000560: 6f63 732f 5573 6572 4d61 6e75 616c 5f76  ocs/UserManual_v
-00000570: 302e 342e 332e 7064 660d 0a63 6f6d 7061  0.4.3.pdf..compa
-00000580: 6e69 6f6e 203d 200d 0a09 636f 6d70 2f43  nion = ...comp/C
-00000590: 6861 6e6e 656c 506f 7369 7469 6f6e 506c  hannelPositionPl
-000005a0: 6f74 732e 7079 0d0a 0963 6f6d 702f 636f  ots.py...comp/co
-000005b0: 6d62 696e 6553 6574 732e 7079 0d0a 0963  mbineSets.py...c
-000005c0: 6f6d 702f 4d61 6e75 616c 5665 6374 6f72  omp/ManualVector
-000005d0: 506c 6f74 732e 7079 0d0a 0963 6f6d 702f  Plots.py...comp/
-000005e0: 726f 7461 746f 722e 7079 0d0a 0963 6f6d  rotator.py...com
-000005f0: 702f 7363 7269 7074 5f64 6573 6372 6970  p/script_descrip
-00000600: 7469 6f6e 732e 7478 740d 0a09 636f 6d70  tions.txt...comp
-00000610: 2f73 706c 6974 5f64 6174 6173 6574 2e70  /split_dataset.p
-00000620: 790d 0a09 636f 6d70 2f53 7562 7365 7444  y...comp/SubsetD
-00000630: 6174 6143 6861 6e6e 656c 2e70 790d 0a0d  ataChannel.py...
-00000640: 0a5b 6f70 7469 6f6e 732e 656e 7472 795f  .[options.entry_
-00000650: 706f 696e 7473 5d0d 0a63 6f6e 736f 6c65  points]..console
-00000660: 5f73 6372 6970 7473 203d 200d 0a09 6c61  _scripts = ...la
-00000670: 6d2d 7275 6e20 3d20 7372 632e 7275 6e3a  m-run = src.run:
-00000680: 7275 6e0d 0a0d 0a5b 7364 6973 745d 0d0a  run....[sdist]..
-00000690: 666f 726d 6174 7320 3d20 677a 7461 720d  formats = gztar.
-000006a0: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-000006b0: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-000006c0: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+00000220: 2050 7974 686f 6e20 3a3a 2033 2e39 0d0a   Python :: 3.9..
+00000230: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+00000240: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000250: 3a3a 2033 2e31 300d 0a09 5072 6f67 7261  :: 3.10...Progra
+00000260: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000270: 3a20 5079 7468 6f6e 203a 3a20 3320 3a3a  : Python :: 3 ::
+00000280: 204f 6e6c 790d 0a6b 6579 776f 7264 7320   Only..keywords 
+00000290: 3d20 0d0a 0962 696f 6c6f 6779 0d0a 0964  = ...biology...d
+000002a0: 6174 6120 616e 616c 7973 6973 0d0a 0969  ata analysis...i
+000002b0: 6d61 6765 206f 626a 6563 7420 6461 7461  mage object data
+000002c0: 0d0a 7072 6f6a 6563 745f 7572 6c73 203d  ..project_urls =
+000002d0: 200d 0a09 5072 6f6a 6563 7420 3d20 6874   ...Project = ht
+000002e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000002f0: 2f68 6965 7461 6b61 6e67 6173 2d6c 6162  /hietakangas-lab
+00000300: 6f72 6174 6f72 792f 4c41 4d0d 0a09 4275  oratory/LAM...Bu
+00000310: 6720 5265 706f 7274 7320 3d20 6874 7470  g Reports = http
+00000320: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
+00000330: 6965 7461 6b61 6e67 6173 2d6c 6162 6f72  ietakangas-labor
+00000340: 6174 6f72 792f 4c41 4d2f 6973 7375 6573  atory/LAM/issues
+00000350: 0d0a 0954 7574 6f72 6961 6c20 5669 6465  ...Tutorial Vide
+00000360: 6f73 203d 2068 7474 7073 3a2f 2f77 7777  os = https://www
+00000370: 2e79 6f75 7475 6265 2e63 6f6d 2f70 6c61  .youtube.com/pla
+00000380: 796c 6973 743f 6c69 7374 3d50 4c6a 762d  ylist?list=PLjv-
+00000390: 3847 7a78 6833 4179 6e55 7449 3348 6161  8Gzxh3AynUtI3Haa
+000003a0: 6855 326f 6464 4d62 4470 6774 780d 0a09  hU2oddMbDpgtx...
+000003b0: 5075 626c 6963 6174 696f 6e20 3d20 6874  Publication = ht
+000003c0: 7470 733a 2f2f 646f 692e 6f72 672f 3130  tps://doi.org/10
+000003d0: 2e31 3031 362f 6a2e 6372 6d65 7468 2e32  .1016/j.crmeth.2
+000003e0: 3032 312e 3130 3030 3539 0d0a 0952 6573  021.100059...Res
+000003f0: 6561 7263 6820 4772 6f75 7020 3d20 6874  earch Group = ht
+00000400: 7470 733a 2f2f 7777 772e 6865 6c73 696e  tps://www.helsin
+00000410: 6b69 2e66 692f 656e 2f72 6573 6561 7263  ki.fi/en/researc
+00000420: 6867 726f 7570 732f 6e75 7472 6965 6e74  hgroups/nutrient
+00000430: 2d73 656e 7369 6e67 0d0a 0d0a 5b6f 7074  -sensing....[opt
+00000440: 696f 6e73 5d0d 0a70 6163 6b61 6765 7320  ions]..packages 
+00000450: 3d20 6669 6e64 3a0d 0a70 7974 686f 6e5f  = find:..python_
+00000460: 7265 7175 6972 6573 203d 200d 0a09 3e33  requires = ...>3
+00000470: 2e36 2c20 3c3d 332e 3131 0d0a 696e 7374  .6, <=3.11..inst
+00000480: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
+00000490: 0a09 6d61 7470 6c6f 746c 6962 3e3d 332e  ..matplotlib>=3.
+000004a0: 312e 330d 0a09 6e75 6d70 793e 3d31 2e31  1.3...numpy>=1.1
+000004b0: 382e 310d 0a09 7061 6e64 6173 3e3d 312e  8.1...pandas>=1.
+000004c0: 310d 0a09 7061 7468 6c69 6232 3e3d 322e  1...pathlib2>=2.
+000004d0: 330d 0a09 7363 696b 6974 2d69 6d61 6765  3...scikit-image
+000004e0: 3e3d 302e 3136 2e32 0d0a 0973 6369 6b69  >=0.16.2...sciki
+000004f0: 742d 6c65 6172 6e3e 3d30 2e32 322e 310d  t-learn>=0.22.1.
+00000500: 0a09 7363 6970 793e 3d31 2e34 2e31 0d0a  ..scipy>=1.4.1..
+00000510: 0973 6561 626f 726e 3e3d 302e 3131 2e30  .seaborn>=0.11.0
+00000520: 0d0a 0973 6861 7065 6c79 3e3d 312e 372e  ...shapely>=1.7.
+00000530: 300d 0a09 7374 6174 736d 6f64 656c 733e  0...statsmodels>
+00000540: 3d30 2e31 312e 300d 0a0d 0a5b 6f70 7469  =0.11.0....[opti
+00000550: 6f6e 732e 6461 7461 5f66 696c 6573 5d0d  ons.data_files].
+00000560: 0a69 6d67 203d 200d 0a09 696d 672f 6c61  .img = ...img/la
+00000570: 6d2e 6963 6f0d 0a64 6f63 7320 3d20 0d0a  m.ico..docs = ..
+00000580: 0952 4541 444d 452e 6d64 0d0a 094c 4943  .README.md...LIC
+00000590: 454e 5345 2e6d 640d 0a09 646f 6373 2f43  ENSE.md...docs/C
+000005a0: 6f6d 6d61 6e64 4c69 6e65 4172 6773 2e74  ommandLineArgs.t
+000005b0: 7874 0d0a 0964 6f63 732f 5573 6572 4d61  xt...docs/UserMa
+000005c0: 6e75 616c 5f76 302e 342e 332e 7064 660d  nual_v0.4.3.pdf.
+000005d0: 0a63 6f6d 7061 6e69 6f6e 203d 200d 0a09  .companion = ...
+000005e0: 636f 6d70 2f43 6861 6e6e 656c 506f 7369  comp/ChannelPosi
+000005f0: 7469 6f6e 506c 6f74 732e 7079 0d0a 0963  tionPlots.py...c
+00000600: 6f6d 702f 636f 6d62 696e 6553 6574 732e  omp/combineSets.
+00000610: 7079 0d0a 0963 6f6d 702f 4d61 6e75 616c  py...comp/Manual
+00000620: 5665 6374 6f72 506c 6f74 732e 7079 0d0a  VectorPlots.py..
+00000630: 0963 6f6d 702f 726f 7461 746f 722e 7079  .comp/rotator.py
+00000640: 0d0a 0963 6f6d 702f 7363 7269 7074 5f64  ...comp/script_d
+00000650: 6573 6372 6970 7469 6f6e 732e 7478 740d  escriptions.txt.
+00000660: 0a09 636f 6d70 2f73 706c 6974 5f64 6174  ..comp/split_dat
+00000670: 6173 6574 2e70 790d 0a09 636f 6d70 2f53  aset.py...comp/S
+00000680: 7562 7365 7444 6174 6143 6861 6e6e 656c  ubsetDataChannel
+00000690: 2e70 790d 0a0d 0a5b 6f70 7469 6f6e 732e  .py....[options.
+000006a0: 656e 7472 795f 706f 696e 7473 5d0d 0a63  entry_points]..c
+000006b0: 6f6e 736f 6c65 5f73 6372 6970 7473 203d  onsole_scripts =
+000006c0: 200d 0a09 6c61 6d2d 7275 6e20 3d20 7372   ...lam-run = sr
+000006d0: 632e 7275 6e3a 7275 6e0d 0a0d 0a5b 7364  c.run:run....[sd
+000006e0: 6973 745d 0d0a 666f 726d 6174 7320 3d20  ist]..formats = 
+000006f0: 677a 7461 720d 0a0d 0a5b 6567 675f 696e  gztar....[egg_in
+00000700: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
+00000710: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
+00000720: 0a0d 0a                                  ...
```

### Comparing `LAM-0.4.6/src/analysis.py` & `LAM-0.4.7/src/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,21 +154,19 @@
         lg.logprint(LAM_logger, 'Plotting completed', 'i')
 
     def read_channel(self, path, groups, drop=False, name_sep=1):
         """Read channel data and concatenate sample group info into DF."""
         data = system.read_data(path, header=0, test=False)
         read_data = pd.DataFrame()
 
-        # Loop through given groups and give an identification variable for
-        # each sample belonging to the group.
+        # Loop through given groups and give an identification variable for each sample belonging to the group.
         for grp in groups:
-            namerreg = re.compile('^{}_'.format(grp), re.I)
             # Get only the samples that belong to the loop's current group
-            temp = data.loc[:, data.columns.str.contains(namerreg)].T
-            if Sett.Drop_Outliers and drop:  # conditionfull_dfy drop outliers
+            temp = data.loc[:, data.columns.str.startswith(f'{grp}_')].T
+            if Sett.Drop_Outliers and drop:  # drop outliers
                 temp = drop_outlier(temp)
             temp['Sample Group'] = grp  # Giving of sample group identification
             if read_data.empty:
                 read_data = temp
             else:
                 read_data = pd.concat([read_data, temp])
 
@@ -386,22 +384,21 @@
 class Group(Samplegroups):
     """For storing sample group-specific data."""
 
     def __init__(self, group, child=False):
         super().__init__(child=True)  # Inherit from samplegroups-class
         self.group = group  # group
         # For finding group-specific columns etc.
-        self.namer = '{}_'.format(group)
+        self.namer = f'{self.group}_'
 
         # When first initialized, create variables inherited by samples:
         if not child:
             self.color = self.grp_palette.get(self.group)
-            namerreg = re.compile("^{}".format(self.namer), re.I)
-            self.groupPaths = [p for p in self.sample_paths if namerreg.search(p.name)]
-            inds = self.sample_mps.columns.str.contains(self.namer)
+            self.groupPaths = [p for p in self.sample_paths if p.name.startswith(self.namer)]
+            inds = self.sample_mps.columns.str.startswith(self.namer)
             self.MPs = self.sample_mps.loc[:, inds]
 
 
 class Sample(Group):
     """For sample-specific data and handling sample-related functionalities."""
 
     def __init__(self, path, grp):
```

### Comparing `LAM-0.4.6/src/border_detect.py` & `LAM-0.4.7/src/border_detect.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,36 +86,36 @@
 class FullBorders:
     """Store sample scores from GetSampleBorders and find group peaks."""
 
     def __init__(self, samples, widths, anchor, palette):
         self.samples = samples
         self.width_data = widths
         self.anchor = anchor * 2
-        self.sample_starts = pd.Series()
+        self.sample_starts = pd.Series(dtype=np.int8)
         self.palette = palette
         self.scores = pd.DataFrame(columns=[p.name for p in samples], index=widths.index)
 
     def __call__(self, dirpath, threshold):
         # Fit a curve to sample data and get divergence of values
         flattened = self.flatten_scores()
 
         # Compute total scores of sample groups
         s_sums = get_group_total(flattened)
-        s_sums = s_sums.groupby(s_sums.group).apply(lambda x: x.assign(value=norm_func(x.value)))
+        score_sum = s_sums.groupby(s_sums.group, group_keys=False).apply(lambda x: x.assign(value=norm_func(x.value)))
 
         # Find group peaks
-        peaks = get_peak_data(s_sums, threshold)
+        peaks = get_peak_data(score_sum, threshold)
 
         # Create plots
         if Sett.Create_Border_Plots & Sett.Create_Plots:
             print('  Creating border plot  ...')
             # Transform data to plottable format
             scores = prepare_data(self.scores.T)
             # Plot
-            self.group_plots(scores, s_sums, peaks, dirpath)
+            self.group_plots(scores, score_sum, peaks, dirpath)
 
         # Readjust peak locations and indexing to original bins
         peaks.peak = peaks.peak.divide(2)
         self.sample_starts = self.sample_starts.divide(2)
         return self.scores.T, peaks
 
     def flatten_scores(self):
@@ -123,15 +123,14 @@
         # Add identifiers to data
         groups = [s[0] for s in self.scores.columns.str.split('_')]
         vals = self.scores.T.copy().assign(group=groups)
         # Group data based on sample groups
         grouped = vals.groupby('group')
         # Fit curve to values in each sample group
         curves = grouped.apply(lambda x: get_fit(x, x.name, id_var=['group']))
-        # re-index
         curves = curves.droplevel(1)
         # Subtract curve from each sample
         devs = vals.apply(lambda x, c=curves: x[:-1].subtract(c.loc[x.group, :]), axis=1)
         return devs
 
     def group_plots(self, scores, s_sums, peaks, dirpath):
         """Create plots of sample group border scores."""
@@ -453,24 +452,21 @@
         # Find prominence of found peaks
         prom = peak_prominences(total, peaks)[0]
         peaks = total.index[peaks].get_level_values(1).values
         peak_dict = {'group': grp, 'peak': peaks, 'prominence': prom, 'sign': 'pos'}
 
         # NEGATIVE peaks
         # neg_total = total * -1
-        # npeaks, _ = find_peaks(neg_total, distance=4, height=thresh,
-        #                           width=2)#, threshold=thresh)
+        # npeaks, _ = find_peaks(neg_total, distance=4, height=thresh, width=2)#, threshold=thresh)
         # nprom = peak_prominences(neg_total, npeaks)[0]
         # npeaks = neg_total.index[npeaks].get_level_values(1).values
-        # npeak_dict = {'group': grp, 'peak': npeaks, 'prominence': nprom * -1,
-        #               'sign': 'neg'}
+        # npeak_dict = {'group': grp, 'peak': npeaks, 'prominence': nprom * -1, 'sign': 'neg'}
 
         # Add groups data to full peak data
-        all_peaks = all_peaks.append(pd.DataFrame(peak_dict), ignore_index=True)
-        # all_peaks = all_peaks.append(pd.DataFrame(npeak_dict), ignore_index=True)
+        all_peaks = pd.concat([all_peaks, pd.DataFrame(peak_dict)], ignore_index=True)
     return all_peaks
 
 
 def get_diff(data):
     """Calculate bin-to-bin differences"""
     diff = data.diff()[1:]
     # Shift data by one index position to match locations
@@ -479,23 +475,23 @@
 
 
 def get_group_total(data):
     """Get smoothed total scores of groups."""
     # smoothed = smooth_data(data.T, win=7, tau=10).T
     trimmed = prepare_data(data)
     # Get mean score for each bin
-    s_sums = trimmed.groupby(['group', 'variable']).apply(lambda x: x.value.mean())
+    s_sums = trimmed.groupby(['group', 'variable'], group_keys=True).apply(lambda x: x.value.mean())
 
     # Transform to dataframe and assign necessary identifier columns
     s_sums = s_sums.to_frame(name='value')
-    s_sums = s_sums.groupby('group').apply(lambda x: x.assign(value=smooth_data(x.value, win=5, tau=10)))
-
+    s_sums = s_sums.groupby('group', group_keys=False).apply(
+        lambda x: x.assign(value=smooth_data(x.value, win=5, tau=10)))
     # Add identifier columns, i.e. groups and bins
-    s_sums = s_sums.assign(group=s_sums.index.get_level_values(0), variable=s_sums.index.get_level_values(1))
-    return s_sums
+    return s_sums.assign(group=s_sums.index.get_level_values(0),
+                         variable=s_sums.index.get_level_values(1))
 
 
 def get_sum_score(scores):
     """Find the summed score of the detection variables."""
     # Smooth raw scores and the sum for total
     s_sum = smooth_data(scores, win=7, tau=10).sum(axis=1)
     # trim zeros from array ends
@@ -564,15 +560,15 @@
     """Perform rolling smoothing to data."""
     smoothed_data = data.rolling(win, center=True, win_type='exponential').mean(tau=tau)
     return smoothed_data
 
 
 def trim_data(data, grouper='group'):
     """Trim bins where less than half of a sample group has values."""
-    grouped = data.groupby(grouper)
+    grouped = data.groupby(grouper, group_keys=False)
     # Create mask
     masks = grouped.apply(lambda x: x.isna().sum() < x.shape[0]/2)
     # Apply mask
     return grouped.apply(lambda x, m=masks: apply_mask(x, m.loc[x.name, :]))
 
 
 def apply_mask(arr, mask):
@@ -588,16 +584,16 @@
     except KeyError:
         data = data.melt()
 
     # Drop missing values
     data = data.dropna()
 
     # Take all x and y data
-    x_data = data.variable.values.astype(np.float)
-    y_data = data.value.values.astype(np.float)
+    x_data = data.variable.values.astype(np.int8)
+    y_data = data.value.values.astype(np.float32)
 
     #  #Fit x and y data with 4th degree polynomial
     # z = np.polyfit(x_data.astype(np.float), y_data.astype(np.float), 4)
     # f = np.poly1d(z)
     # x_curve = data.variable.unique()
     # y_curve = f(x_curve)
 
@@ -610,15 +606,15 @@
     # Create DF from obtained fit
     curve = pd.DataFrame(index=[name], columns=x_curve.astype(int), data=np.reshape(y_curve, (-1, len(y_curve))))
     return curve
 
 
 def norm_func(arr: pd.Series) -> pd.Series:
     """Normalize array between 0 and 1."""
-    return (arr-np.nanmin(arr))/(np.nanmax(arr)-np.nanmin(arr))
+    return (arr - np.nanmin(arr)) / (np.nanmax(arr) - np.nanmin(arr))
 
 
 def ask_peaks(peaks, gui_root):
     """Ask user input to determine plottable peaks."""
 
     if gui_root is not None:  # If GUI, make input window
         win = PeakDialog(data=peaks, master=gui_root)
```

### Comparing `LAM-0.4.6/src/interface.py` & `LAM-0.4.7/src/interface.py`

 * *Files identical despite different names*

### Comparing `LAM-0.4.6/src/logger.py` & `LAM-0.4.7/src/logger.py`

 * *Files identical despite different names*

### Comparing `LAM-0.4.6/src/parse_cmds.py` & `LAM-0.4.7/src/parse_cmds.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 def change_settings(parser):
     """Use parsed arguments to change settings."""
     changed_settings = {}  # For storing changed settings for printing
 
     # ADJUSTMENT OF SETTINGS BASED ON PARSED ARGUMENTS:
     # Work directory, i.e. analysis directory
     if parser.path:
-        Sett.workdir = pl.Path(parser.path)
+        Sett.workdir = parser.path
     print(f'Work directory: {Sett.workdir}')
 
     # Primary options
     if parser.options:
         primaries = primary_options(parser.options)
         print(f"Primary settings: {', '.join(primaries)}")
```

### Comparing `LAM-0.4.6/src/plot.py` & `LAM-0.4.7/src/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,23 +183,21 @@
     def stats(self, **kws):
         """Modify plot to include statistics."""
         stats = self.sec_data.stat_data
         __, ytop = plt.ylim()
         tytop = ytop*1.35
         ax = plt.gca()
         ax.set_ylim(top=tytop)
-        yaxis = [tytop, tytop]
 
         # Create secondary axis for significance plotting
         ax2 = plt.twinx()
         lkws = {'alpha': 0.85}
         xmin, xtop = stats.index.min(), stats.index.max()
         ax2.plot((xmin, xtop), (0, 0), linestyle='dashed', color='grey', linewidth=0.85, **lkws)
-        # Find top of original y-axis and create a buffer for twin to
-        # create a prettier plot
+        # Find top of original y-axis and create a buffer for twin to create a prettier plot
         bottom_add = 2.75*-Sett.ylim
         ax2.set_ylim(bottom=bottom_add, top=Sett.ylim)
         ax2.set_yticks(np.arange(0, Sett.ylim, 10))
         ax2.set_yticklabels(np.arange(0, Sett.ylim, 10))
         ax2.yaxis.set_label_coords(1.04, 0.85)
 
         # Creation of -log2 P-value axis and line plot
@@ -211,18 +209,18 @@
             ind = y_val[y_val.notnull()].index
             logvals = pd.Series(np.zeros(y_val.shape[0]), index=y_val.index)
             with warnings.catch_warnings():
                 warnings.simplefilter('ignore', category=RuntimeWarning)
                 logvals.loc[ind] = np.log2(y_val[ind].astype(np.float64))
             # Create twin axis with -log2 P-values
             ax2.plot(x_val, np.negative(logvals), color='dimgrey', linewidth=1.5, **lkws)
-            ax2.set_ylabel('P value\n(-log2)')
+            ax2.set_ylabel('\n-log2(p)', loc='top')  # , labelpad=0.05)
         # Create significance stars and color fills
         for index, row in stats.iterrows():
-            plot_significance(index, row, ax2, yaxis, yheight=0)
+            plot_significance(index, row, ax2, (tytop, tytop), yheight=0)
         # Add info on sliding window to plot
         if 'windowed' in kws:
             comment = "Window: lead {}, trail {}".format(Sett.lead, Sett.trail)
             plt.annotate(comment, (5, 5), xycoords='figure pixels')
 
     def stats_total(self, **kws):
         """Create statistical objects to total statistics-plots"""
@@ -482,19 +480,19 @@
         plotter(pfunc.heatmap, 'centerline', 'ticks', 'title', 'labels', **p_kws)
 
         # Plot sample group averages
         grouped = all_data.groupby(['Channel', 'Sample Group'])
         # Construct a dataframe with averages:
         avg_data = pd.DataFrame()
         for grp, data in grouped:
-            temp = pd.Series(data.mean(), name=grp[1])
-            temp['Channel'] = grp[0]
-            avg_data = avg_data.append(temp)
+            temp = data.select_dtypes(include=np.number).mean().rename(grp[1])
+            temp.at['Channel'] = grp[0]
+            avg_data = pd.concat([avg_data, temp], axis=1, ignore_index=False)
         # Create plot
-        plotter = MakePlot(avg_data, handle, 'Cluster Heatmaps - Groups')
+        plotter = MakePlot(avg_data.T, handle, 'Cluster Heatmaps - Groups')
         plotter(pfunc.heatmap, 'centerline', 'ticks', 'title', 'labels', 'peaks', **new_kws)
 
         # CLUSTER LINEPLOT
         m_kws = {'ylabel': 'Clustered cells', 'titley': 1.01, 'row': 'Channel', 'col': None,
                  'melt': {'id_vars': ['Channel', 'Sample Group'], 'var_name': 'Linear Position', 'value_name': 'Value'}}
         m_data = all_data.drop('Sample', axis=1)
         m_data = m_data.melt(id_vars=['Channel', 'Sample Group'], var_name='Linear Position', value_name='Value')
@@ -611,15 +609,15 @@
         handle = system.DataHandler(self.sgroups, path, savepath)
         # Give title
         data_name = str(path.stem).split('_')[1:]
         titlep = '-'.join(data_name)
         f_title = "{} = {}".format(stats.title, titlep)
         # Plot variable
         plotter = MakePlot(plot_data, handle, f_title, sec_data=stats)
-        ylabel = get_unit(data_name[-1])
+        ylabel = get_unit(data_name[2]) if len(data_name) == 3 else get_unit(data_name[-1])
         p_kws = {'col': None, 'row': None, 'ylabel': ylabel, 'label_first_only': True, 'gridspec': {'bottom': 0.2},
                  'melt': {'id_vars': ['Sample Group'], 'var_name': 'Linear Position', 'value_name': 'Value'}}
         if Sett.windowed:
             p_kws.update({'windowed': True})
 
         plotter(pfunc.lines, 'centerline', 'ticks', 'title', 'stats', 'labels', 'legend', 'peaks', **p_kws)
 
@@ -753,10 +751,10 @@
         return
     xaxis = [index-0.43, index+0.43]
     if row[3] is True:  # ctrl is greater
         p_str, color = significance_marker(row[1], MakePlot.LScolors)
     elif row[6] is True:  # ctrl is lesser
         p_str, color = significance_marker(row[4], MakePlot.GRcolors)
     if fill:
-        ax.fill_between(xaxis, yaxis, color=color, alpha=0.35, zorder=0)
+        ax.fill_between(xaxis, yaxis[1], y2=(0, 0), color=color, alpha=0.35, zorder=0)
     if stars:
         ax.annotate(p_str, (index, yheight), fontsize=8, ha='center')
```

### Comparing `LAM-0.4.6/src/plotfuncs.py` & `LAM-0.4.7/src/plotfuncs.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     # Create plot grid
     g = sns.FacetGrid(data=data, row=kws.get('row'), col=kws.get('col'), hue="Sample Group", sharex=False,
                       sharey=False, height=5, aspect=1)
     with warnings.catch_warnings():
         warnings.simplefilter('ignore', category=UserWarning)
         try:
             # Create plots
-            g = g.map(sns.kdeplot, 'Value_y', 'Value_x', shade_lowest=False, shade=False, linewidths=1.75, alpha=0.6)
+            g = g.map(sns.kdeplot, 'Value_y', 'Value_x', fill=False, linewidths=1.75, alpha=0.6)
         except np.linalg.LinAlgError:
             msg = '-> Confirm that all samples have proper channel data'
             fullmsg = f'Bivariate plot singular matrix\n{msg}'
             lg.logprint(LAM_logger, fullmsg, 'ex')
             print('ERROR: Bivariate plot singular matrix')
             print(msg)
             return g
@@ -163,15 +163,15 @@
 def lines(plotter, **kws):
     """Plot lines."""
     err_dict = {'alpha': 0.3}
     data = plotter.data
     # data = plotter.data.dropna()
     melt_kws = kws.get('melt')
     g = (plotter.g.map_dataframe(sns.lineplot, data=data, x=melt_kws.get('var_name'), y=melt_kws.get('value_name'),
-                                 ci='sd', err_style='band', hue=kws.get('hue'), dashes=False, alpha=1,
+                                 errorbar='sd', err_style='band', hue=kws.get('hue'), dashes=False, alpha=1,
                                  palette=plotter.handle.palette, err_kws=err_dict))
     # for ax in g.axes.flat:
     #     ax.set_ylim(100, 300)
     return g
 
 
 def skeleton_plot(savepath, samplename, binary_array, skeleton):
```

### Comparing `LAM-0.4.6/src/process.py` & `LAM-0.4.7/src/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,15 +335,15 @@
                 mp_dir_path = next(self.channelpaths.pop(i) for i, s in enumerate(self.channelpaths) if
                                    str('_' + mp_name + '_') in str(s))
                 mp_path = next(mp_dir_path.glob("*Position.csv"))
                 mp_data = system.read_data(mp_path, header=Sett.header_row, test=False)
                 mp_data = mp_data.loc[:, ['Position X', 'Position Y']]
                 if not mp_data.empty:
                     mp_bin = self.project_mps(mp_data, datadir, filename="MPs.csv")
-                    mp_df = pd.DataFrame({'MP': mp_bin.values.codes})
+                    mp_df = pd.DataFrame({'MP': mp_bin.values})
                     mp_df.to_csv(self.sampledir.joinpath("MPs.csv"), index=False)
             except (StopIteration, ValueError, UnboundLocalError):
                 mp_bin = None
                 msg = f'could not find MP position for {self.name}'
                 lg.logprint(LAM_logger, msg, 'e')
                 print("    -> Failed to find MP position data.")
         else:  # Sets measurement point values to zero when MP's are not used
@@ -351,59 +351,47 @@
             system.save_to_file(mp_bin, datadir, "MPs.csv")
             system.save_to_file(mp_bin, self.sampledir, "MPs.csv", append=False)
         return mp_bin
 
     def project_mps(self, positions, datadir, filename="some.csv"):
         """For the projection of spot coordinates onto the vector."""
         xy_positions = list(zip(positions['Position X'], positions['Position Y']))
-        # The shapely packages reguires transformation into Multipoints for the
-        # projection.
-        points = gm.MultiPoint(xy_positions)
-        # Find point of projection on the vector.
-        positions["VectPoint"] = [self.vector.interpolate(self.vector.project(gm.Point(x))) for x in points]
-        # Find normalized distance (0->1)
-        positions["NormDist"] = [self.vector.project(x, normalized=True) for x in positions["VectPoint"]]
-        # Find the bins that the points fall into
-        # Determine bins of each feature
-        edges = np.linspace(0, 1, Sett.projBins+1)
-        labels = np.arange(0, Sett.projBins)
-        positions["DistBin"] = pd.cut(positions["NormDist"], edges, labels=labels)
-        mp_bin = pd.Series(positions.loc[:, "DistBin"], name=self.name)
+        points = (gm.Point(c) for c in xy_positions)
+        # Find points of projection and respective normalized linear reference along vector
+        projected = [self.vector.interpolate(self.vector.project(p)) for p in points]
+        positions["NormDist"] = [self.vector.project(p, normalized=True) for p in projected]
+        # Get bins for the projected MPs
+        positions["DistBin"] = pd.cut(positions.loc[:, "NormDist"], bins=np.linspace(0, 1, Sett.projBins+1),
+                                      labels=np.arange(0, Sett.projBins), include_lowest=True)
+        # Format output and sanity check on results:
         self.data = positions
         self.test_projection(Sett.MPname)
-        # Save the obtained data:
+        mp_bin = pd.Series(positions.loc[:, "DistBin"], name=self.name)
         system.save_to_file(mp_bin.astype(int), datadir, filename)
         return mp_bin
 
     def project_channel(self, channel):
         """For projecting coordinates onto the vector."""
         data = channel.data
         xy_positions = list(zip(data['Position X'], data['Position Y']))
-        # Transformation into Multipoints required for projection:
         points = gm.MultiPoint(xy_positions)
-        # Find projection distance on the vector.
-        proj_vector_dist = [self.vector.project(x) for x in points]
-        # Find the exact point of projection
-        proj_points = [self.vector.interpolate(p) for p in proj_vector_dist]
-        # Find distance between feature and the point of projection
-        proj_dist = [p.distance(proj_points[i]) for i, p in enumerate(points)]
-        # Find normalized distance (0->1)
+
+        # Get linear references of projections, then interpolate coordinates and get normalized references.
+        proj_vector_dist = [self.vector.project(p) for p in points.geoms]
+        proj_points = [self.vector.interpolate(d) for d in proj_vector_dist]
         data["NormDist"] = [d / self.vector_length for d in proj_vector_dist]
-        # Determine bins of each feature
-        edges = np.linspace(0, 1, Sett.projBins+1)
-        labels = np.arange(0, Sett.projBins)
-        data["DistBin"] = pd.cut(data["NormDist"], labels=labels, bins=edges, include_lowest=True).astype('int')
 
-        # Assign data to DF and save the dataframe:
+        # Based on projection, assign bins for features on the channel
+        data["DistBin"] = pd.cut(data.loc[:, "NormDist"], labels=np.arange(0, Sett.projBins), bins=np.linspace(0, 1, Sett.projBins+1), include_lowest=True).astype('int')
+        # Format output, plus a sanity check on results
         data["VectPoint"] = [(round(p.x, 3), round(p.y, 3)) for p in proj_points]
-        data["ProjDist"] = proj_dist
+        data["ProjDist"] = [v.distance(p) for (v, p) in zip(points.geoms, proj_points)]
+        system.save_to_file(data, self.sampledir, f'{channel.name}.csv', append=False)
         self.data = data
         self.test_projection(channel.name)
-        channel_string = f'{channel.name}.csv'
-        system.save_to_file(data, self.sampledir, channel_string, append=False)
         return data
 
     def find_counts(self, channel_name, datadir):
         """Gather projected features and find bin counts."""
         counts = np.bincount(self.data['DistBin'], minlength=Sett.projBins)
         counts = pd.Series(np.nan_to_num(counts), name=self.name)
         channel_string = f'All_{channel_name}.csv'
@@ -520,16 +508,16 @@
         self.starts = None
 
     def averages(self, norm_counts: pd.DataFrame):
         """Find bin averages of channels."""
         # Find groups of each sample based on samplenames
         samples = norm_counts.columns.tolist()
         groups = set({s.casefold(): s.split('_')[0] for s in samples}.values())
-        cols = ["{}_All".format(g) for g in groups]
-        averages = pd.DataFrame(index=norm_counts.index, columns=cols)
+        # cols = ["{}_All".format(g) for g in groups]
+        averages = pd.DataFrame(index=norm_counts.index)
         for grp in groups:  # For each group found in data
             namer = "{}_".format(grp)
             group_data = norm_counts.loc[:, norm_counts.columns.str.startswith(namer)]
             # Calculate group averages
             averages.loc[:, "{}_All".format(grp)] = group_data.mean(axis=1)
         # Save average data
         filename = str('ChanAvg_{}.csv'.format(self.channel))
@@ -655,15 +643,15 @@
                         width += temp.tolist()[-1]
             return width
 
         edges = self.get_vector_edges(multip=2, points=False)
         cols = ['NormDist', 'ProjDist', 'hand']
         data = self.data.sort_values(by='NormDist').loc[:, cols]
         # Create series to hold width results
-        res = pd.Series(name=self.name, index=pd.RangeIndex(stop=len(edges)))
+        res = pd.Series(name=self.name, index=pd.RangeIndex(stop=len(edges)), dtype=np.float64)
         # Loop segments and get widths:
         for ind, _ in enumerate(edges[:-1]):
             d_index = data.loc[(data.NormDist >= edges[ind]) & (data.NormDist < edges[ind+1])].index
             res.iat[ind] = _get_approx_width(data.loc[d_index, :])
         filename = 'Sample_widths.csv'
         system.save_to_file(res, datadir, filename)
```

### Comparing `LAM-0.4.6/src/redirect.py` & `LAM-0.4.7/src/redirect.py`

 * *Files identical despite different names*

### Comparing `LAM-0.4.6/src/run.py` & `LAM-0.4.7/src/run.py`

 * *Files identical despite different names*

### Comparing `LAM-0.4.6/src/settings.py` & `LAM-0.4.7/src/settings.py`

 * *Files identical despite different names*

### Comparing `LAM-0.4.6/src/statsMWW.py` & `LAM-0.4.7/src/statsMWW.py`

 * *Files 10% similar despite different names*

```diff
@@ -201,43 +201,29 @@
             return [0, 0, 0]
 
         return [stat, pval, reject]
 
 
 def get_stats(row, row2, ind, stat_data):
     """Compare respective bins of both groups."""
-    unqs = np.unique(np.hstack((row, row2))).size
+    def mww(alt, r1=row, r2=row2):
+        return ss.mannwhitneyu(r1, r2, alternative=alt)
 
-    # If data rows are different, get stats
-    if (row.any() and row2.any()) and not np.array_equal(np.unique(row), np.unique(row2)) and unqs > 1:
-
-        with warnings.catch_warnings():
-            warnings.simplefilter('ignore', category=RuntimeWarning)
-            # Whether ctrl is greater
-            stat, pval = ss.mannwhitneyu(row, row2, alternative='greater')
-            stat_data.iat[ind, 0], stat_data.iat[ind, 2] = stat, pval
-            # Whether ctrl is lesser
-            __, pval = ss.mannwhitneyu(row, row2, alternative='less')
-            stat_data.iat[ind, 5] = pval
-            # Whether significant difference exists
-            __, pval = ss.mannwhitneyu(row, row2, alternative='two-sided')
-            stat_data.iat[ind, 8] = pval
-
-    else:  # If rows are same. input zeros
-        stat_data.iat[ind, 0], stat_data.iat[ind, 2] = 0, 0
-        stat_data.iat[ind, 5] = 0
-        stat_data.iat[ind, 8] = 0
+    if any([np.isnan(row).all(), np.isnan(row2).all()]):
+        stat_data.iloc[ind, [0, 2, 5, 8]] = np.nan
+    else:
+        results = map(mww, ['greater', 'less', 'two-sided'])
+        stat_data.iloc[ind, [0, 2]] = next(results)
+        stat_data.iloc[ind, 5] = next(results).pvalue
+        stat_data.iloc[ind, 8] = next(results).pvalue
     return stat_data
 
 
 def correct(stat_data, p_vals, corr_ind, rej_ind):
     """Correct for multipletesting."""
-
-    vals = p_vals.values  # Get P-values
-
-    with warnings.catch_warnings():  # Correct
-        warnings.simplefilter('ignore', category=RuntimeWarning)
-        reject, corr_p, _, _ = multi.multipletests(vals, method='fdr_bh', alpha=Sett.alpha)
-
+    tested = ~p_vals.isna().values
+    reject, corr_p, _, _ = multi.multipletests(p_vals[tested].values, method='fdr_bh', alpha=Sett.alpha)
     # Add corrected values to DF
-    stat_data.iloc[:, corr_ind], stat_data.iloc[:, rej_ind] = corr_p, reject
+    stat_data.iloc[tested, corr_ind] = corr_p
+    stat_data.iloc[tested, rej_ind] = reject
+    stat_data.iloc[~tested, rej_ind] = False
     return stat_data
```

### Comparing `LAM-0.4.6/src/system.py` & `LAM-0.4.7/src/system.py`

 * *Files 6% similar despite different names*

```diff
@@ -287,23 +287,31 @@
     if not test_vectors:
         return paths
 
     # Check that vector channel data are found
     if Sett.process_samples or (Sett.measure_width and Sett.process_counts):
         samples = [p for p in Sett.workdir.iterdir() if p.is_dir() and p.name != 'Analysis Data']
         failed = []
+        wrong_index = []
         for sample in samples:
             try:
                 next(sample.glob(f'*_{Sett.vectChannel}_*'))
             except StopIteration:
-                failed.append(sample.name)
-        if failed:
+                try:
+                    next(sample.glob(f'^{Sett.vectChannel}_*'))
+                    wrong_index.append(sample.name)
+                except StopIteration:
+                    failed.append(sample.name)
+        if failed or wrong_index:
             msg = f"Vector channel data not found for {', '.join(failed)}"
+            if wrong_index:
+                print("Channel folders MUST have channel name separated by underscores, e.g. 'sample_DAPI_stats'.")
+            else:
+                print("Check vector channel's name setting and/or file existence.")
             print(f'ERROR: {msg}')
-            print('Check vector channel setting or data.')
             lg.logprint(LAM_logger, msg, 'e')
             raise SystemExit
 
     # Find and store all sample names
     Store.samples = [p.name for p in paths.samplesdir.iterdir() if p.is_dir()]
     return paths
 
@@ -352,18 +360,18 @@
             mean = np.nanmean(values.astype('float'))
             std = np.nanstd(values.astype('float'))
         drop_val = Sett.dropSTD * std
         if raw:  # If data is not melted, replace outliers with NaN
             data.where(np.abs(values - mean) <= drop_val, other=np.nan, inplace=True)
         else:  # If data is melted and sorted, find indexes until val < drop
             idx = []
-            for ind, val in values.iteritems():
+            for (key, val) in values.items():
                 if np.abs(val - mean) < drop_val:
                     break
-                idx.append(ind)
+                idx.append(key)
             # Select data that fills criteria for validity
             data = data.loc[(data.index.difference(idx)), :]
         return data
 
     if raw:
         all_data = drop(all_data, col=None)
         return all_data
```

### Comparing `LAM-0.4.6/src/vector_loop.py` & `LAM-0.4.7/src/vector_loop.py`

 * *Files identical despite different names*

