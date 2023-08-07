# Comparing `tmp/HaploDynamics-0.1b3.tar.gz` & `tmp/HaploDynamics-0.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HaploDynamics-0.1b3.tar", last modified: Sun Aug  6 18:54:15 2023, max compression
+gzip compressed data, was "HaploDynamics-0.1b4.tar", last modified: Mon Aug  7 01:31:16 2023, max compression
```

## Comparing `HaploDynamics-0.1b3.tar` & `HaploDynamics-0.1b4.tar`

### file list

```diff
@@ -1,18 +1,12 @@
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-06 18:54:15.142546 HaploDynamics-0.1b3/
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-06 18:54:15.142546 HaploDynamics-0.1b3/Framework/
--rw-rw-r--   0 remy      (1000) remy      (1000)       22 2023-08-06 18:51:05.000000 HaploDynamics-0.1b3/Framework/__init__.py
--rw-rw-r--   0 remy      (1000) remy      (1000)       67 2023-08-06 18:51:05.000000 HaploDynamics-0.1b3/Framework/future.py
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-06 18:54:15.142546 HaploDynamics-0.1b3/HaploDX/
--rw-rw-r--   0 remy      (1000) remy      (1000)    17508 2023-08-06 18:51:05.000000 HaploDynamics-0.1b3/HaploDX/HaploDX.py
--rw-rw-r--   0 remy      (1000) remy      (1000)       23 2023-08-06 18:51:05.000000 HaploDynamics-0.1b3/HaploDX/__init__.py
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-06 18:54:15.142546 HaploDynamics-0.1b3/HaploDynamics.egg-info/
--rw-rw-r--   0 remy      (1000) remy      (1000)     8396 2023-08-06 18:54:15.000000 HaploDynamics-0.1b3/HaploDynamics.egg-info/PKG-INFO
--rw-rw-r--   0 remy      (1000) remy      (1000)      301 2023-08-06 18:54:15.000000 HaploDynamics-0.1b3/HaploDynamics.egg-info/SOURCES.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)        1 2023-08-06 18:54:15.000000 HaploDynamics-0.1b3/HaploDynamics.egg-info/dependency_links.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)        6 2023-08-06 18:54:15.000000 HaploDynamics-0.1b3/HaploDynamics.egg-info/requires.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)       18 2023-08-06 18:54:15.000000 HaploDynamics-0.1b3/HaploDynamics.egg-info/top_level.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)    35149 2023-08-06 18:51:05.000000 HaploDynamics-0.1b3/LICENSE
--rw-rw-r--   0 remy      (1000) remy      (1000)     8396 2023-08-06 18:54:15.142546 HaploDynamics-0.1b3/PKG-INFO
--rw-rw-r--   0 remy      (1000) remy      (1000)     7512 2023-08-06 18:51:05.000000 HaploDynamics-0.1b3/README.md
--rw-rw-r--   0 remy      (1000) remy      (1000)       79 2023-08-06 18:54:15.142546 HaploDynamics-0.1b3/setup.cfg
--rw-rw-r--   0 remy      (1000) remy      (1000)     1213 2023-08-06 18:51:19.000000 HaploDynamics-0.1b3/setup.py
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 01:31:16.696850 HaploDynamics-0.1b4/
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 01:31:16.696850 HaploDynamics-0.1b4/HaploDynamics.egg-info/
+-rw-rw-r--   0 remy      (1000) remy      (1000)     9277 2023-08-07 01:31:16.000000 HaploDynamics-0.1b4/HaploDynamics.egg-info/PKG-INFO
+-rw-rw-r--   0 remy      (1000) remy      (1000)      220 2023-08-07 01:31:16.000000 HaploDynamics-0.1b4/HaploDynamics.egg-info/SOURCES.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)        1 2023-08-07 01:31:16.000000 HaploDynamics-0.1b4/HaploDynamics.egg-info/dependency_links.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)        6 2023-08-07 01:31:16.000000 HaploDynamics-0.1b4/HaploDynamics.egg-info/requires.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)        1 2023-08-07 01:31:16.000000 HaploDynamics-0.1b4/HaploDynamics.egg-info/top_level.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)    35149 2023-08-07 01:26:43.000000 HaploDynamics-0.1b4/LICENSE
+-rw-rw-r--   0 remy      (1000) remy      (1000)     9277 2023-08-07 01:31:16.696850 HaploDynamics-0.1b4/PKG-INFO
+-rw-rw-r--   0 remy      (1000) remy      (1000)     8393 2023-08-07 01:26:43.000000 HaploDynamics-0.1b4/README.md
+-rw-rw-r--   0 remy      (1000) remy      (1000)       79 2023-08-07 01:31:16.696850 HaploDynamics-0.1b4/setup.cfg
+-rw-rw-r--   0 remy      (1000) remy      (1000)     1213 2023-08-07 01:28:07.000000 HaploDynamics-0.1b4/setup.py
```

### Comparing `HaploDynamics-0.1b3/HaploDynamics.egg-info/PKG-INFO` & `HaploDynamics-0.1b4/HaploDynamics.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: HaploDynamics
-Version: 0.1b3
+Version: 0.1b4
 Summary: A python library to develop genomic data simulators
 Home-page: https://github.com/remytuyeras/HaploDynamics
-Download-URL: https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.3.tar.gz
+Download-URL: https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.4.tar.gz
 Author: Remy Tuyeras
 Author-email: rtuyeras@gmail.com
 License: gpl-3.0
 Keywords: Simulator,Genomics,Genomic,Microarray,SNP chip,VCF,Linkage disequilibrium,Hardy-Weinberg equilibrium
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -19,29 +19,51 @@
 License-File: LICENSE
 
 # HaploDynamics
 The python library **HaploDynamics**, or **HaploDX** for short, provides a collection of functions that can be used to simulate population-specific genomic data. This package is part of the Genetic Simulator Resources (GSR) catalog (click the link below for more information).
 
 <div style="width: 180px; margin: 0 auto;"><a href="https://surveillance.cancer.gov/genetic-simulation-resources/"><img src="https://surveillance.cancer.gov/gsr/static/img/gsr_tile.jpg" alt="Catalogued on GSR" width="180" height="60" /></a></div>
 
+## News
+
+* Adding installation procedure via ```pip```
+* Adding the module ```Framework``` for a class-based development framework
+
 ## Installation
 
 ### Manual installation
+Download the github package using the following command.
 ```bash
 $ git clone https://github.com/remytuyeras/HaploDynamics.git
 ```
-Then, create your script where the folder ```HaploDynamics``` is located.
+Then, from your current directory, record the absolute path leading to the main module of the package, as shown below.
 ```bash
 $ ls
 HaploDynamics
-$ touch myscript.py
+$ cd HaploDynamics/
+$ pwd
+path/to/main/module/HaploDynamics
+```
+To import the modules of the library to your script, use the following syntax where you must replace ```path/to/main/module/HaploDynamics``` with the path that you obtained above.
+```python
+import sys
+sys.path.insert (0,"path/to/main/module/HaploDynamics")
+import HaploDynamics.HaploDX as hdx
+import HaploDynamics.Framework as hdx_frm
+```
+### Pip [still in progress]
+Install the package using ```pip install``` as follows.
+```bash
+$ pip install HaploDynamics
+```
+Then, you can import the modules of the library to your script as follows.
+```python
+import HaploDynamics.HaploDX as hdx
+import HaploDynamics.Framework as hdx_frm
 ```
-### Pip
-Coming soon
-
 ## Quick start
 
 The following script generates a VCF file containing simulated diploid genotypes for a population of 1000 individuals with LD-blocks of length 20kb, 5kb, 20kb, 35kb, 30kb and 15kb. 
 ```python
 import HaploDynamics.HaploDX as hdx
 
 simulated_data = hdx.genmatrix([20,5,20,35,30,15],strength=1,population=0.1,Npop=1000)
@@ -189,9 +211,7 @@
 - _note:_ this function cannot be used with ```genmatrix()``` since the ```pre_matrix``` is not returned
 ```python
 def display(rel: list[list],m: float) -> list[list[tuple[float,float,float]]]
 ```
 ```python
 def minor_haplotype(sub_pre_matrix: list[list]) -> float
 ```
-
-
```

#### html2text {}

```diff
@@ -1,31 +1,43 @@
-Metadata-Version: 2.1 Name: HaploDynamics Version: 0.1b3 Summary: A python
+Metadata-Version: 2.1 Name: HaploDynamics Version: 0.1b4 Summary: A python
 library to develop genomic data simulators Home-page: https://github.com/
 remytuyeras/HaploDynamics Download-URL: https://github.com/remytuyeras/
-HaploDynamics/archive/refs/tags/v0.1-beta.3.tar.gz Author: Remy Tuyeras Author-
+HaploDynamics/archive/refs/tags/v0.1-beta.4.tar.gz Author: Remy Tuyeras Author-
 email: rtuyeras@gmail.com License: gpl-3.0 Keywords:
 Simulator,Genomics,Genomic,Microarray,SNP chip,VCF,Linkage
 disequilibrium,Hardy-Weinberg equilibrium Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Intended Audience
 :: Science/Research Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Description-Content-Type: text/markdown License-File:
 LICENSE # HaploDynamics The python library **HaploDynamics**, or **HaploDX**
 for short, provides a collection of functions that can be used to simulate
 population-specific genomic data. This package is part of the Genetic Simulator
 Resources (GSR) catalog (click the link below for more information).
 [Catalogued_on_GSR]
-## Installation ### Manual installation ```bash $ git clone https://github.com/
-remytuyeras/HaploDynamics.git ``` Then, create your script where the folder
-```HaploDynamics``` is located. ```bash $ ls HaploDynamics $ touch myscript.py
-``` ### Pip Coming soon ## Quick start The following script generates a VCF
-file containing simulated diploid genotypes for a population of 1000
-individuals with LD-blocks of length 20kb, 5kb, 20kb, 35kb, 30kb and 15kb.
-```python import HaploDynamics.HaploDX as hdx simulated_data = hdx.genmatrix(
+## News * Adding installation procedure via ```pip``` * Adding the module
+```Framework``` for a class-based development framework ## Installation ###
+Manual installation Download the github package using the following command.
+```bash $ git clone https://github.com/remytuyeras/HaploDynamics.git ``` Then,
+from your current directory, record the absolute path leading to the main
+module of the package, as shown below. ```bash $ ls HaploDynamics $ cd
+HaploDynamics/ $ pwd path/to/main/module/HaploDynamics ``` To import the
+modules of the library to your script, use the following syntax where you must
+replace ```path/to/main/module/HaploDynamics``` with the path that you obtained
+above. ```python import sys sys.path.insert (0,"path/to/main/module/
+HaploDynamics") import HaploDynamics.HaploDX as hdx import
+HaploDynamics.Framework as hdx_frm ``` ### Pip [still in progress] Install the
+package using ```pip install``` as follows. ```bash $ pip install HaploDynamics
+``` Then, you can import the modules of the library to your script as follows.
+```python import HaploDynamics.HaploDX as hdx import HaploDynamics.Framework as
+hdx_frm ``` ## Quick start The following script generates a VCF file containing
+simulated diploid genotypes for a population of 1000 individuals with LD-blocks
+of length 20kb, 5kb, 20kb, 35kb, 30kb and 15kb. ```python import
+HaploDynamics.HaploDX as hdx simulated_data = hdx.genmatrix(
 [20,5,20,35,30,15],strength=1,population=0.1,Npop=1000) hdx.create_vcfgz
 ("genomic-data.simulation.v1",*simulated_data) ``` The equation
 ```strength=1``` forces a high amount of linkage disequilibrium and the
 equation ```population=0.1``` increases the likelyhood of the simulated
 population to have rare mutations (e.g. to simulate a population profile close
 to African and South-Asian populations). More generally, the function
 ```genmatrix()``` takes the following types of parameters: Parameters | Type |
```

### Comparing `HaploDynamics-0.1b3/LICENSE` & `HaploDynamics-0.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `HaploDynamics-0.1b3/PKG-INFO` & `HaploDynamics-0.1b4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: HaploDynamics
-Version: 0.1b3
+Version: 0.1b4
 Summary: A python library to develop genomic data simulators
 Home-page: https://github.com/remytuyeras/HaploDynamics
-Download-URL: https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.3.tar.gz
+Download-URL: https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.4.tar.gz
 Author: Remy Tuyeras
 Author-email: rtuyeras@gmail.com
 License: gpl-3.0
 Keywords: Simulator,Genomics,Genomic,Microarray,SNP chip,VCF,Linkage disequilibrium,Hardy-Weinberg equilibrium
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -19,29 +19,51 @@
 License-File: LICENSE
 
 # HaploDynamics
 The python library **HaploDynamics**, or **HaploDX** for short, provides a collection of functions that can be used to simulate population-specific genomic data. This package is part of the Genetic Simulator Resources (GSR) catalog (click the link below for more information).
 
 <div style="width: 180px; margin: 0 auto;"><a href="https://surveillance.cancer.gov/genetic-simulation-resources/"><img src="https://surveillance.cancer.gov/gsr/static/img/gsr_tile.jpg" alt="Catalogued on GSR" width="180" height="60" /></a></div>
 
+## News
+
+* Adding installation procedure via ```pip```
+* Adding the module ```Framework``` for a class-based development framework
+
 ## Installation
 
 ### Manual installation
+Download the github package using the following command.
 ```bash
 $ git clone https://github.com/remytuyeras/HaploDynamics.git
 ```
-Then, create your script where the folder ```HaploDynamics``` is located.
+Then, from your current directory, record the absolute path leading to the main module of the package, as shown below.
 ```bash
 $ ls
 HaploDynamics
-$ touch myscript.py
+$ cd HaploDynamics/
+$ pwd
+path/to/main/module/HaploDynamics
+```
+To import the modules of the library to your script, use the following syntax where you must replace ```path/to/main/module/HaploDynamics``` with the path that you obtained above.
+```python
+import sys
+sys.path.insert (0,"path/to/main/module/HaploDynamics")
+import HaploDynamics.HaploDX as hdx
+import HaploDynamics.Framework as hdx_frm
+```
+### Pip [still in progress]
+Install the package using ```pip install``` as follows.
+```bash
+$ pip install HaploDynamics
+```
+Then, you can import the modules of the library to your script as follows.
+```python
+import HaploDynamics.HaploDX as hdx
+import HaploDynamics.Framework as hdx_frm
 ```
-### Pip
-Coming soon
-
 ## Quick start
 
 The following script generates a VCF file containing simulated diploid genotypes for a population of 1000 individuals with LD-blocks of length 20kb, 5kb, 20kb, 35kb, 30kb and 15kb. 
 ```python
 import HaploDynamics.HaploDX as hdx
 
 simulated_data = hdx.genmatrix([20,5,20,35,30,15],strength=1,population=0.1,Npop=1000)
@@ -189,9 +211,7 @@
 - _note:_ this function cannot be used with ```genmatrix()``` since the ```pre_matrix``` is not returned
 ```python
 def display(rel: list[list],m: float) -> list[list[tuple[float,float,float]]]
 ```
 ```python
 def minor_haplotype(sub_pre_matrix: list[list]) -> float
 ```
-
-
```

#### html2text {}

```diff
@@ -1,31 +1,43 @@
-Metadata-Version: 2.1 Name: HaploDynamics Version: 0.1b3 Summary: A python
+Metadata-Version: 2.1 Name: HaploDynamics Version: 0.1b4 Summary: A python
 library to develop genomic data simulators Home-page: https://github.com/
 remytuyeras/HaploDynamics Download-URL: https://github.com/remytuyeras/
-HaploDynamics/archive/refs/tags/v0.1-beta.3.tar.gz Author: Remy Tuyeras Author-
+HaploDynamics/archive/refs/tags/v0.1-beta.4.tar.gz Author: Remy Tuyeras Author-
 email: rtuyeras@gmail.com License: gpl-3.0 Keywords:
 Simulator,Genomics,Genomic,Microarray,SNP chip,VCF,Linkage
 disequilibrium,Hardy-Weinberg equilibrium Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Intended Audience
 :: Science/Research Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Description-Content-Type: text/markdown License-File:
 LICENSE # HaploDynamics The python library **HaploDynamics**, or **HaploDX**
 for short, provides a collection of functions that can be used to simulate
 population-specific genomic data. This package is part of the Genetic Simulator
 Resources (GSR) catalog (click the link below for more information).
 [Catalogued_on_GSR]
-## Installation ### Manual installation ```bash $ git clone https://github.com/
-remytuyeras/HaploDynamics.git ``` Then, create your script where the folder
-```HaploDynamics``` is located. ```bash $ ls HaploDynamics $ touch myscript.py
-``` ### Pip Coming soon ## Quick start The following script generates a VCF
-file containing simulated diploid genotypes for a population of 1000
-individuals with LD-blocks of length 20kb, 5kb, 20kb, 35kb, 30kb and 15kb.
-```python import HaploDynamics.HaploDX as hdx simulated_data = hdx.genmatrix(
+## News * Adding installation procedure via ```pip``` * Adding the module
+```Framework``` for a class-based development framework ## Installation ###
+Manual installation Download the github package using the following command.
+```bash $ git clone https://github.com/remytuyeras/HaploDynamics.git ``` Then,
+from your current directory, record the absolute path leading to the main
+module of the package, as shown below. ```bash $ ls HaploDynamics $ cd
+HaploDynamics/ $ pwd path/to/main/module/HaploDynamics ``` To import the
+modules of the library to your script, use the following syntax where you must
+replace ```path/to/main/module/HaploDynamics``` with the path that you obtained
+above. ```python import sys sys.path.insert (0,"path/to/main/module/
+HaploDynamics") import HaploDynamics.HaploDX as hdx import
+HaploDynamics.Framework as hdx_frm ``` ### Pip [still in progress] Install the
+package using ```pip install``` as follows. ```bash $ pip install HaploDynamics
+``` Then, you can import the modules of the library to your script as follows.
+```python import HaploDynamics.HaploDX as hdx import HaploDynamics.Framework as
+hdx_frm ``` ## Quick start The following script generates a VCF file containing
+simulated diploid genotypes for a population of 1000 individuals with LD-blocks
+of length 20kb, 5kb, 20kb, 35kb, 30kb and 15kb. ```python import
+HaploDynamics.HaploDX as hdx simulated_data = hdx.genmatrix(
 [20,5,20,35,30,15],strength=1,population=0.1,Npop=1000) hdx.create_vcfgz
 ("genomic-data.simulation.v1",*simulated_data) ``` The equation
 ```strength=1``` forces a high amount of linkage disequilibrium and the
 equation ```population=0.1``` increases the likelyhood of the simulated
 population to have rare mutations (e.g. to simulate a population profile close
 to African and South-Asian populations). More generally, the function
 ```genmatrix()``` takes the following types of parameters: Parameters | Type |
```

### Comparing `HaploDynamics-0.1b3/README.md` & `HaploDynamics-0.1b4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,49 @@
 # HaploDynamics
 The python library **HaploDynamics**, or **HaploDX** for short, provides a collection of functions that can be used to simulate population-specific genomic data. This package is part of the Genetic Simulator Resources (GSR) catalog (click the link below for more information).
 
 <div style="width: 180px; margin: 0 auto;"><a href="https://surveillance.cancer.gov/genetic-simulation-resources/"><img src="https://surveillance.cancer.gov/gsr/static/img/gsr_tile.jpg" alt="Catalogued on GSR" width="180" height="60" /></a></div>
 
+## News
+
+* Adding installation procedure via ```pip```
+* Adding the module ```Framework``` for a class-based development framework
+
 ## Installation
 
 ### Manual installation
+Download the github package using the following command.
 ```bash
 $ git clone https://github.com/remytuyeras/HaploDynamics.git
 ```
-Then, create your script where the folder ```HaploDynamics``` is located.
+Then, from your current directory, record the absolute path leading to the main module of the package, as shown below.
 ```bash
 $ ls
 HaploDynamics
-$ touch myscript.py
+$ cd HaploDynamics/
+$ pwd
+path/to/main/module/HaploDynamics
+```
+To import the modules of the library to your script, use the following syntax where you must replace ```path/to/main/module/HaploDynamics``` with the path that you obtained above.
+```python
+import sys
+sys.path.insert (0,"path/to/main/module/HaploDynamics")
+import HaploDynamics.HaploDX as hdx
+import HaploDynamics.Framework as hdx_frm
+```
+### Pip [still in progress]
+Install the package using ```pip install``` as follows.
+```bash
+$ pip install HaploDynamics
+```
+Then, you can import the modules of the library to your script as follows.
+```python
+import HaploDynamics.HaploDX as hdx
+import HaploDynamics.Framework as hdx_frm
 ```
-### Pip
-Coming soon
-
 ## Quick start
 
 The following script generates a VCF file containing simulated diploid genotypes for a population of 1000 individuals with LD-blocks of length 20kb, 5kb, 20kb, 35kb, 30kb and 15kb. 
 ```python
 import HaploDynamics.HaploDX as hdx
 
 simulated_data = hdx.genmatrix([20,5,20,35,30,15],strength=1,population=0.1,Npop=1000)
@@ -169,9 +191,7 @@
 - _note:_ this function cannot be used with ```genmatrix()``` since the ```pre_matrix``` is not returned
 ```python
 def display(rel: list[list],m: float) -> list[list[tuple[float,float,float]]]
 ```
 ```python
 def minor_haplotype(sub_pre_matrix: list[list]) -> float
 ```
-
-
```

#### html2text {}

```diff
@@ -1,19 +1,31 @@
 # HaploDynamics The python library **HaploDynamics**, or **HaploDX** for short,
 provides a collection of functions that can be used to simulate population-
 specific genomic data. This package is part of the Genetic Simulator Resources
 (GSR) catalog (click the link below for more information).
 [Catalogued_on_GSR]
-## Installation ### Manual installation ```bash $ git clone https://github.com/
-remytuyeras/HaploDynamics.git ``` Then, create your script where the folder
-```HaploDynamics``` is located. ```bash $ ls HaploDynamics $ touch myscript.py
-``` ### Pip Coming soon ## Quick start The following script generates a VCF
-file containing simulated diploid genotypes for a population of 1000
-individuals with LD-blocks of length 20kb, 5kb, 20kb, 35kb, 30kb and 15kb.
-```python import HaploDynamics.HaploDX as hdx simulated_data = hdx.genmatrix(
+## News * Adding installation procedure via ```pip``` * Adding the module
+```Framework``` for a class-based development framework ## Installation ###
+Manual installation Download the github package using the following command.
+```bash $ git clone https://github.com/remytuyeras/HaploDynamics.git ``` Then,
+from your current directory, record the absolute path leading to the main
+module of the package, as shown below. ```bash $ ls HaploDynamics $ cd
+HaploDynamics/ $ pwd path/to/main/module/HaploDynamics ``` To import the
+modules of the library to your script, use the following syntax where you must
+replace ```path/to/main/module/HaploDynamics``` with the path that you obtained
+above. ```python import sys sys.path.insert (0,"path/to/main/module/
+HaploDynamics") import HaploDynamics.HaploDX as hdx import
+HaploDynamics.Framework as hdx_frm ``` ### Pip [still in progress] Install the
+package using ```pip install``` as follows. ```bash $ pip install HaploDynamics
+``` Then, you can import the modules of the library to your script as follows.
+```python import HaploDynamics.HaploDX as hdx import HaploDynamics.Framework as
+hdx_frm ``` ## Quick start The following script generates a VCF file containing
+simulated diploid genotypes for a population of 1000 individuals with LD-blocks
+of length 20kb, 5kb, 20kb, 35kb, 30kb and 15kb. ```python import
+HaploDynamics.HaploDX as hdx simulated_data = hdx.genmatrix(
 [20,5,20,35,30,15],strength=1,population=0.1,Npop=1000) hdx.create_vcfgz
 ("genomic-data.simulation.v1",*simulated_data) ``` The equation
 ```strength=1``` forces a high amount of linkage disequilibrium and the
 equation ```population=0.1``` increases the likelyhood of the simulated
 population to have rare mutations (e.g. to simulate a population profile close
 to African and South-Asian populations). More generally, the function
 ```genmatrix()``` takes the following types of parameters: Parameters | Type |
```

### Comparing `HaploDynamics-0.1b3/setup.py` & `HaploDynamics-0.1b4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
   name = 'HaploDynamics',
   packages=setuptools.find_packages(include=['HaploDX','Framework']),
-  version = 'v0.1-beta.3',
+  version = 'v0.1-beta.4',
   license='gpl-3.0',
   author = 'Remy Tuyeras',
   author_email = 'rtuyeras@gmail.com',
   description = 'A python library to develop genomic data simulators',
   long_description = long_description,
   long_description_content_type = "text/markdown",
   url = 'https://github.com/remytuyeras/HaploDynamics',
-  download_url = 'https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.3.tar.gz',
+  download_url = 'https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.4.tar.gz',
   keywords = ['Simulator', 'Genomics', 'Genomic', 'Microarray','SNP chip','VCF', 'Linkage disequilibrium', 'Hardy-Weinberg equilibrium'],
   install_requires=['scipy'],
   classifiers=[
     'Development Status :: 4 - Beta',  #"3 - Alpha", "4 - Beta" or "5 - Production/Stable"
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'Topic :: Software Development :: Build Tools',
```

