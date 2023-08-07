# Comparing `tmp/HaploDynamics-0.1b9.tar.gz` & `tmp/HaploDynamics-0.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HaploDynamics-0.1b9.tar", last modified: Mon Aug  7 02:23:37 2023, max compression
+gzip compressed data, was "HaploDynamics-0.2b0.tar", last modified: Mon Aug  7 04:36:08 2023, max compression
```

## Comparing `HaploDynamics-0.1b9.tar` & `HaploDynamics-0.2b0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 02:23:37.812746 HaploDynamics-0.1b9/
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 02:23:37.812746 HaploDynamics-0.1b9/HaploDynamics/
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 02:23:37.812746 HaploDynamics-0.1b9/HaploDynamics/Framework/
--rw-rw-r--   0 remy      (1000) remy      (1000)       22 2023-08-07 02:23:26.000000 HaploDynamics-0.1b9/HaploDynamics/Framework/__init__.py
--rw-rw-r--   0 remy      (1000) remy      (1000)       67 2023-08-07 02:23:26.000000 HaploDynamics-0.1b9/HaploDynamics/Framework/future.py
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 02:23:37.812746 HaploDynamics-0.1b9/HaploDynamics/HaploDX/
--rw-rw-r--   0 remy      (1000) remy      (1000)    17508 2023-08-07 02:23:26.000000 HaploDynamics-0.1b9/HaploDynamics/HaploDX/HaploDX.py
--rw-rw-r--   0 remy      (1000) remy      (1000)       23 2023-08-07 02:23:26.000000 HaploDynamics-0.1b9/HaploDynamics/HaploDX/__init__.py
--rw-rw-r--   0 remy      (1000) remy      (1000)       60 2023-08-07 02:23:26.000000 HaploDynamics-0.1b9/HaploDynamics/__init__.py
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 02:23:37.812746 HaploDynamics-0.1b9/HaploDynamics.egg-info/
--rw-rw-r--   0 remy      (1000) remy      (1000)     9277 2023-08-07 02:23:37.000000 HaploDynamics-0.1b9/HaploDynamics.egg-info/PKG-INFO
--rw-rw-r--   0 remy      (1000) remy      (1000)      383 2023-08-07 02:23:37.000000 HaploDynamics-0.1b9/HaploDynamics.egg-info/SOURCES.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)        1 2023-08-07 02:23:37.000000 HaploDynamics-0.1b9/HaploDynamics.egg-info/dependency_links.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)        6 2023-08-07 02:23:37.000000 HaploDynamics-0.1b9/HaploDynamics.egg-info/requires.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)       14 2023-08-07 02:23:37.000000 HaploDynamics-0.1b9/HaploDynamics.egg-info/top_level.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)    35149 2023-08-07 02:23:26.000000 HaploDynamics-0.1b9/LICENSE
--rw-rw-r--   0 remy      (1000) remy      (1000)     9277 2023-08-07 02:23:37.816745 HaploDynamics-0.1b9/PKG-INFO
--rw-rw-r--   0 remy      (1000) remy      (1000)     8393 2023-08-07 02:23:26.000000 HaploDynamics-0.1b9/README.md
--rw-rw-r--   0 remy      (1000) remy      (1000)       79 2023-08-07 02:23:37.816745 HaploDynamics-0.1b9/setup.cfg
--rw-rw-r--   0 remy      (1000) remy      (1000)     1257 2023-08-07 02:23:26.000000 HaploDynamics-0.1b9/setup.py
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 04:36:08.972797 HaploDynamics-0.2b0/
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 04:36:08.972797 HaploDynamics-0.2b0/HaploDynamics/
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 04:36:08.972797 HaploDynamics-0.2b0/HaploDynamics/Framework/
+-rw-rw-r--   0 remy      (1000) remy      (1000)       22 2023-08-07 04:33:10.000000 HaploDynamics-0.2b0/HaploDynamics/Framework/__init__.py
+-rw-rw-r--   0 remy      (1000) remy      (1000)       67 2023-08-07 04:33:10.000000 HaploDynamics-0.2b0/HaploDynamics/Framework/future.py
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 04:36:08.972797 HaploDynamics-0.2b0/HaploDynamics/HaploDX/
+-rw-rw-r--   0 remy      (1000) remy      (1000)    17508 2023-08-07 04:33:10.000000 HaploDynamics-0.2b0/HaploDynamics/HaploDX/HaploDX.py
+-rw-rw-r--   0 remy      (1000) remy      (1000)       23 2023-08-07 04:33:10.000000 HaploDynamics-0.2b0/HaploDynamics/HaploDX/__init__.py
+-rw-rw-r--   0 remy      (1000) remy      (1000)       60 2023-08-07 04:33:10.000000 HaploDynamics-0.2b0/HaploDynamics/__init__.py
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-07 04:36:08.972797 HaploDynamics-0.2b0/HaploDynamics.egg-info/
+-rw-rw-r--   0 remy      (1000) remy      (1000)    11076 2023-08-07 04:36:08.000000 HaploDynamics-0.2b0/HaploDynamics.egg-info/PKG-INFO
+-rw-rw-r--   0 remy      (1000) remy      (1000)      383 2023-08-07 04:36:08.000000 HaploDynamics-0.2b0/HaploDynamics.egg-info/SOURCES.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)        1 2023-08-07 04:36:08.000000 HaploDynamics-0.2b0/HaploDynamics.egg-info/dependency_links.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)        6 2023-08-07 04:36:08.000000 HaploDynamics-0.2b0/HaploDynamics.egg-info/requires.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)       14 2023-08-07 04:36:08.000000 HaploDynamics-0.2b0/HaploDynamics.egg-info/top_level.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)    35149 2023-08-07 04:33:10.000000 HaploDynamics-0.2b0/LICENSE
+-rw-rw-r--   0 remy      (1000) remy      (1000)    11076 2023-08-07 04:36:08.972797 HaploDynamics-0.2b0/PKG-INFO
+-rw-rw-r--   0 remy      (1000) remy      (1000)    10192 2023-08-07 04:33:10.000000 HaploDynamics-0.2b0/README.md
+-rw-rw-r--   0 remy      (1000) remy      (1000)       79 2023-08-07 04:36:08.972797 HaploDynamics-0.2b0/setup.cfg
+-rw-rw-r--   0 remy      (1000) remy      (1000)     1257 2023-08-07 04:33:10.000000 HaploDynamics-0.2b0/setup.py
```

### Comparing `HaploDynamics-0.1b9/HaploDynamics/HaploDX/HaploDX.py` & `HaploDynamics-0.2b0/HaploDynamics/HaploDX/HaploDX.py`

 * *Files identical despite different names*

### Comparing `HaploDynamics-0.1b9/HaploDynamics.egg-info/PKG-INFO` & `HaploDynamics-0.2b0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,41 @@
-Metadata-Version: 2.1
-Name: HaploDynamics
-Version: 0.1b9
-Summary: A python library to develop genomic data simulators
-Home-page: https://github.com/remytuyeras/HaploDynamics
-Download-URL: https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.9.tar.gz
-Author: Remy Tuyeras
-Author-email: rtuyeras@gmail.com
-License: gpl-3.0
-Keywords: Simulator,Genomics,Genomic,Microarray,SNP chip,VCF,Linkage disequilibrium,Hardy-Weinberg equilibrium
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # HaploDynamics
 The python library **HaploDynamics**, or **HaploDX** for short, provides a collection of functions that can be used to simulate population-specific genomic data. This package is part of the Genetic Simulator Resources (GSR) catalog (click the link below for more information).
 
 <div style="width: 180px; margin: 0 auto;"><a href="https://surveillance.cancer.gov/genetic-simulation-resources/"><img src="https://surveillance.cancer.gov/gsr/static/img/gsr_tile.jpg" alt="Catalogued on GSR" width="180" height="60" /></a></div>
 
-## News
+## New features recently added
 
-* Adding installation procedure via ```pip```
-* Adding the module ```Framework``` for a class-based development framework
+* Installation via ```pip```;
+* A class-based module ```Framework``` for software development and experimentations.
 
 ## Installation
 
 ### Manual installation
-Download the github package using the following command.
+Download the github package by using the following command in a terminal.
 ```bash
 $ git clone https://github.com/remytuyeras/HaploDynamics.git
 ```
-Then, from your current directory, record the absolute path leading to the main module of the package, as shown below.
+Then, from your current directory, record the absolute path leading to the downloaded package, as shown below.
 ```bash
 $ ls
 HaploDynamics
 $ cd HaploDynamics/
 $ pwd
-path/to/main/module/HaploDynamics
+absolute/path/to/HaploDynamics
 ```
-To import the modules of the library to your script, use the following syntax where you must replace ```path/to/main/module/HaploDynamics``` with the path that you obtained above.
+To import the modules of the library to your script, use the following syntax where you need replace ```absolute/path/to/HaploDynamics``` with the path that you obtained above.
 ```python
 import sys
-sys.path.insert (0,"path/to/main/module/HaploDynamics")
+sys.path.insert (0,"absolute/path/to/HaploDynamics")
 import HaploDynamics.HaploDX as hdx
 import HaploDynamics.Framework as hdx_frm
 ```
-### Pip [still in progress]
-Install the package using ```pip install``` as follows.
+### Installation via Pip
+Install the package by using ```pip install``` as follows.
 ```bash
 $ pip install HaploDynamics
 ```
 Then, you can import the modules of the library to your script as follows.
 ```python
 import HaploDynamics.HaploDX as hdx
 import HaploDynamics.Framework as hdx_frm
@@ -75,38 +55,95 @@
 Parameters | Type | Values
 | :--- | :--- | :---
 ```blocks```  | ```list[int]``` | List of positive integers, ideally between 1 and 40.
 ```strength```  | ```float``` | From -1 (little linkage) to 1 (high linkage)
 ```population```  | ```float``` | From 0 (for more rare mutations) to 1 (for less rare mutations)
 ```Npop```  | ```int```  | Positive integer specifying the number of individuals in the genomic matrix
 
-The generation of each locus in a VCF file tend to be linear in the parameter ```Npop```. For example, one genetic variant can take from 0.3 to 0.8 seconds to be generated/simulated when we set ```Npop=100000``` (this may vary depending on your machine). The estimated time complexity for an average machine is shown below.
+The generation of each locus in a VCF file tends to be linear in the parameter ```Npop```. On average, a genetic variant can take from 0.3 to 0.8 seconds to be generated when ```Npop=100000``` (this may vary depending on your machine). The estimated time complexity for an average machine is shown below.
 
-![GitHub Logo](/time_complexity.png)
+![](/img/time_complexity.png) 
 
-The following script shows how to display the linkage disequilibirum correlations associated with the simulated data.
+## Use cases
+The following script shows how to display linkage disequilibirum correlations for the simulated data.
 ```python
 import matplotlib.pyplot as plt
 import HaploDynamics.HaploDX as hdx
 
-simulated_data = hdx.genmatrix([20,5,20,35,30,15],strength=1,population=0.1,Npop=1000)
+simulated_data = hdx.genmatrix([20,20,20,20,20,20],strength=1,population=0.1,Npop=1000)
 hdx.create_vcfgz("genomic-data.simulation.v1",*simulated_data)
 
 rel, m, _ = hdx.LD_corr_matrix(simulated_data[0])
 plt.imshow(hdx.display(rel,m))
 plt.show()
 ```
-The following plot is an example of the output that can be returned by the previous script when using 6 LD-blocks of 20kb each.
+A typical output for the previous script should look as follows.
+![](/img/simulation_LD_0.png) 
+
+The following script shows how you can control linkage disequilibrium by using LD-blocks of varying legnths. You can display the graph relating distances between pairs of SNPS to average correlation scores by using the last output of the function ```LD_corr_matrix()```.
+
+```python
+import matplotlib.pyplot as plt
+import HaploDynamics.HaploDX as hdx
+
+ld_blocks = [5,5,5,10,20,5,5,5,5,5,5,1,1,1,2,2,10,20,40]
+strength=1
+population=0.1
+Npop = 1000
+simulated_data = hdx.genmatrix(ld_blocks,strength,population,Npop)
+hdx.create_vcfgz("genomic-data.simulation.v1",*simulated_data)
+
+#Correlations
+rel, m, dist = hdx.LD_corr_matrix(simulated_data[0])
+plt.imshow(hdx.display(rel,m))
+plt.show()
+
+#from SNP-distance to average correlaions
+plt.plot([i for i in range(len(dist)-1)],dist[1:])
+plt.ylim([0, 1])
+plt.show()
+```
+Typical outputs for the previous script should look as follows.
 
-![alt text](http://www.normalesup.org/~tuyeras/node_diss/blg/blg_stat/img/LD_block_corr_strength_high.png)
+Correlations            |  SNP-distance to average correlations
+:-------------------------:|:-------------------------:
+![](/img/simulation_LD_1.png)  |  ![](/img/simulation_dist_1.png)
 
+Finally, the following script shows how you can generate large regions of linkage.
 
-## HaploDX Functions
+```python
+import matplotlib.pyplot as plt
+import HaploDynamics.HaploDX as hdx
+
+ld_blocks = [1] * 250
+strength=1
+population=0.1
+Npop = 1000
+simulated_data = hdx.genmatrix(ld_blocks,strength,population,Npop)
+hdx.create_vcfgz("genomic-data.simulation.v1",*simulated_data)
 
-You can find a complete presentation (or in fact a thorough tutorial) of the **HaploDX** library on my personal webpage (<a href="https://www.normalesup.org/~tuyeras/node_diss/blg/home.php?page=blg_stat/stat_1/home.php">here</a>). Below is the list of all functions accessible from the library. It is recommended to first experiment with the functions presented in the [Data Generation](#data-generation) section.
+#Correlations
+rel, m, dist = hdx.LD_corr_matrix(simulated_data[0])
+plt.imshow(hdx.display(rel,m))
+plt.show()
+
+#from SNP-distance to average correlaions
+plt.plot([i for i in range(len(dist)-1)],dist[1:])
+plt.ylim([0, 1])
+plt.show()
+```
+Typical outputs for the previous script should look as follows.
+
+Correlations            |  SNP-distance to average correlations
+:-------------------------:|:-------------------------:
+![](/img/simulation_LD_2.png)  |  ![](/img/simulation_dist_2.png)
+
+## Functions from HaploDX
+
+You can find a complete presentation (or in fact a thorough tutorial) of the **HaploDX** module on my personal webpage (<a href="https://www.normalesup.org/~tuyeras/node_diss/blg/home.php?page=blg_stat/stat_1/home.php">here</a>). Below is the list of all functions accessible from the library. It is recommended to first experiment with the functions presented in the [Data Generation](#data-generation) section.
 
 ### Population and Allele Frequency Spectrum Modeling
 
 ```python
 def stochastic_line(a: float,b: float,sigma: float) -> Callable[float,float]
 ```
 ```python
@@ -211,7 +248,11 @@
 - _note:_ this function cannot be used with ```genmatrix()``` since the ```pre_matrix``` is not returned
 ```python
 def display(rel: list[list],m: float) -> list[list[tuple[float,float,float]]]
 ```
 ```python
 def minor_haplotype(sub_pre_matrix: list[list]) -> float
 ```
+
+## Classes from Framework
+
+To be added.
```

#### html2text {}

```diff
@@ -1,119 +1,130 @@
-Metadata-Version: 2.1 Name: HaploDynamics Version: 0.1b9 Summary: A python
-library to develop genomic data simulators Home-page: https://github.com/
-remytuyeras/HaploDynamics Download-URL: https://github.com/remytuyeras/
-HaploDynamics/archive/refs/tags/v0.1-beta.9.tar.gz Author: Remy Tuyeras Author-
-email: rtuyeras@gmail.com License: gpl-3.0 Keywords:
-Simulator,Genomics,Genomic,Microarray,SNP chip,VCF,Linkage
-disequilibrium,Hardy-Weinberg equilibrium Classifier: Development Status :: 4 -
-Beta Classifier: Intended Audience :: Developers Classifier: Intended Audience
-:: Science/Research Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.9 Description-Content-Type: text/markdown License-File:
-LICENSE # HaploDynamics The python library **HaploDynamics**, or **HaploDX**
-for short, provides a collection of functions that can be used to simulate
-population-specific genomic data. This package is part of the Genetic Simulator
-Resources (GSR) catalog (click the link below for more information).
+# HaploDynamics The python library **HaploDynamics**, or **HaploDX** for short,
+provides a collection of functions that can be used to simulate population-
+specific genomic data. This package is part of the Genetic Simulator Resources
+(GSR) catalog (click the link below for more information).
 [Catalogued_on_GSR]
-## News * Adding installation procedure via ```pip``` * Adding the module
-```Framework``` for a class-based development framework ## Installation ###
-Manual installation Download the github package using the following command.
-```bash $ git clone https://github.com/remytuyeras/HaploDynamics.git ``` Then,
-from your current directory, record the absolute path leading to the main
-module of the package, as shown below. ```bash $ ls HaploDynamics $ cd
-HaploDynamics/ $ pwd path/to/main/module/HaploDynamics ``` To import the
-modules of the library to your script, use the following syntax where you must
-replace ```path/to/main/module/HaploDynamics``` with the path that you obtained
-above. ```python import sys sys.path.insert (0,"path/to/main/module/
+## New features recently added * Installation via ```pip```; * A class-based
+module ```Framework``` for software development and experimentations. ##
+Installation ### Manual installation Download the github package by using the
+following command in a terminal. ```bash $ git clone https://github.com/
+remytuyeras/HaploDynamics.git ``` Then, from your current directory, record the
+absolute path leading to the downloaded package, as shown below. ```bash $ ls
+HaploDynamics $ cd HaploDynamics/ $ pwd absolute/path/to/HaploDynamics ``` To
+import the modules of the library to your script, use the following syntax
+where you need replace ```absolute/path/to/HaploDynamics``` with the path that
+you obtained above. ```python import sys sys.path.insert (0,"absolute/path/to/
 HaploDynamics") import HaploDynamics.HaploDX as hdx import
-HaploDynamics.Framework as hdx_frm ``` ### Pip [still in progress] Install the
-package using ```pip install``` as follows. ```bash $ pip install HaploDynamics
-``` Then, you can import the modules of the library to your script as follows.
-```python import HaploDynamics.HaploDX as hdx import HaploDynamics.Framework as
-hdx_frm ``` ## Quick start The following script generates a VCF file containing
-simulated diploid genotypes for a population of 1000 individuals with LD-blocks
-of length 20kb, 5kb, 20kb, 35kb, 30kb and 15kb. ```python import
-HaploDynamics.HaploDX as hdx simulated_data = hdx.genmatrix(
+HaploDynamics.Framework as hdx_frm ``` ### Installation via Pip Install the
+package by using ```pip install``` as follows. ```bash $ pip install
+HaploDynamics ``` Then, you can import the modules of the library to your
+script as follows. ```python import HaploDynamics.HaploDX as hdx import
+HaploDynamics.Framework as hdx_frm ``` ## Quick start The following script
+generates a VCF file containing simulated diploid genotypes for a population of
+1000 individuals with LD-blocks of length 20kb, 5kb, 20kb, 35kb, 30kb and 15kb.
+```python import HaploDynamics.HaploDX as hdx simulated_data = hdx.genmatrix(
 [20,5,20,35,30,15],strength=1,population=0.1,Npop=1000) hdx.create_vcfgz
 ("genomic-data.simulation.v1",*simulated_data) ``` The equation
 ```strength=1``` forces a high amount of linkage disequilibrium and the
 equation ```population=0.1``` increases the likelyhood of the simulated
 population to have rare mutations (e.g. to simulate a population profile close
 to African and South-Asian populations). More generally, the function
 ```genmatrix()``` takes the following types of parameters: Parameters | Type |
 Values | :--- | :--- | :--- ```blocks``` | ```list[int]``` | List of positive
 integers, ideally between 1 and 40. ```strength``` | ```float``` | From -1
 (little linkage) to 1 (high linkage) ```population``` | ```float``` | From 0
 (for more rare mutations) to 1 (for less rare mutations) ```Npop``` | ```int```
 | Positive integer specifying the number of individuals in the genomic matrix
-The generation of each locus in a VCF file tend to be linear in the parameter
-```Npop```. For example, one genetic variant can take from 0.3 to 0.8 seconds
-to be generated/simulated when we set ```Npop=100000``` (this may vary
-depending on your machine). The estimated time complexity for an average
-machine is shown below. ![GitHub Logo](/time_complexity.png) The following
-script shows how to display the linkage disequilibirum correlations associated
-with the simulated data. ```python import matplotlib.pyplot as plt import
-HaploDynamics.HaploDX as hdx simulated_data = hdx.genmatrix(
-[20,5,20,35,30,15],strength=1,population=0.1,Npop=1000) hdx.create_vcfgz
-("genomic-data.simulation.v1",*simulated_data) rel, m, _ = hdx.LD_corr_matrix
-(simulated_data[0]) plt.imshow(hdx.display(rel,m)) plt.show() ``` The following
-plot is an example of the output that can be returned by the previous script
-when using 6 LD-blocks of 20kb each. ![alt text](http://www.normalesup.org/
-~tuyeras/node_diss/blg/blg_stat/img/LD_block_corr_strength_high.png) ## HaploDX
-Functions You can find a complete presentation (or in fact a thorough tutorial)
-of the **HaploDX** library on my personal webpage (here). Below is the list of
-all functions accessible from the library. It is recommended to first
-experiment with the functions presented in the [Data Generation](#data-
-generation) section. ### Population and Allele Frequency Spectrum Modeling
-```python def stochastic_line(a: float,b: float,sigma: float) -> Callable
-[float,float] ``` ```python population_mut = stochastic_line(0.08,0.17,0.01)
-``` ```python def afs_distribution(index: int,alpha: float = 4/30) -> float ```
-```python def afs_intervals(pick: float,alpha: float = 4/30) -> list[float] ```
-```python def afs_sample(alpha: float = 4/30) -> float ``` ```python def
-genotype_schema(alpha: float = 4/30) -> tuple[float,list[float]] ``` ```python
-def genotype(hwp: list[float],minor: int) -> tuple[int,int] ``` ```python gref
-= lambda g: g[0] if g[0] in [2,0] else g[1] ``` ```python def population_mld(t:
-float) -> tuple[float,float,float] ``` ### LD and HardyâWeinberg Principle
-Modeling ```python def decay(initial: float,halfwidth: float,shift: float) -
-> Callable[float,float] ``` ```python def ref_alt_function(y: float,x: float) -
-> float ``` ```python def alt_alt_function(y: float,z: float,x: float) -> float
-``` ```python def amplifier(beta: float,p: float,q: float,s: float = 1) -
-> float ``` ```python def lb_freq(beta: float,gamma: float,previous_freq:
-float,distance: float,shift: float) -> float ``` ```python def ub_freq(beta:
+The generation of each locus in a VCF file tends to be linear in the parameter
+```Npop```. On average, a genetic variant can take from 0.3 to 0.8 seconds to
+be generated when ```Npop=100000``` (this may vary depending on your machine).
+The estimated time complexity for an average machine is shown below. ![](/img/
+time_complexity.png) ## Use cases The following script shows how to display
+linkage disequilibirum correlations for the simulated data. ```python import
+matplotlib.pyplot as plt import HaploDynamics.HaploDX as hdx simulated_data =
+hdx.genmatrix([20,20,20,20,20,20],strength=1,population=0.1,Npop=1000)
+hdx.create_vcfgz("genomic-data.simulation.v1",*simulated_data) rel, m, _ =
+hdx.LD_corr_matrix(simulated_data[0]) plt.imshow(hdx.display(rel,m)) plt.show()
+``` A typical output for the previous script should look as follows. ![](/img/
+simulation_LD_0.png) The following script shows how you can control linkage
+disequilibrium by using LD-blocks of varying legnths. You can display the graph
+relating distances between pairs of SNPS to average correlation scores by using
+the last output of the function ```LD_corr_matrix()```. ```python import
+matplotlib.pyplot as plt import HaploDynamics.HaploDX as hdx ld_blocks =
+[5,5,5,10,20,5,5,5,5,5,5,1,1,1,2,2,10,20,40] strength=1 population=0.1 Npop =
+1000 simulated_data = hdx.genmatrix(ld_blocks,strength,population,Npop)
+hdx.create_vcfgz("genomic-data.simulation.v1",*simulated_data) #Correlations
+rel, m, dist = hdx.LD_corr_matrix(simulated_data[0]) plt.imshow(hdx.display
+(rel,m)) plt.show() #from SNP-distance to average correlaions plt.plot([i for i
+in range(len(dist)-1)],dist[1:]) plt.ylim([0, 1]) plt.show() ``` Typical
+outputs for the previous script should look as follows. Correlations | SNP-
+distance to average correlations :-------------------------:|:-----------------
+--------: ![](/img/simulation_LD_1.png) | ![](/img/simulation_dist_1.png)
+Finally, the following script shows how you can generate large regions of
+linkage. ```python import matplotlib.pyplot as plt import HaploDynamics.HaploDX
+as hdx ld_blocks = [1] * 250 strength=1 population=0.1 Npop = 1000
+simulated_data = hdx.genmatrix(ld_blocks,strength,population,Npop)
+hdx.create_vcfgz("genomic-data.simulation.v1",*simulated_data) #Correlations
+rel, m, dist = hdx.LD_corr_matrix(simulated_data[0]) plt.imshow(hdx.display
+(rel,m)) plt.show() #from SNP-distance to average correlaions plt.plot([i for i
+in range(len(dist)-1)],dist[1:]) plt.ylim([0, 1]) plt.show() ``` Typical
+outputs for the previous script should look as follows. Correlations | SNP-
+distance to average correlations :-------------------------:|:-----------------
+--------: ![](/img/simulation_LD_2.png) | ![](/img/simulation_dist_2.png) ##
+Functions from HaploDX You can find a complete presentation (or in fact a
+thorough tutorial) of the **HaploDX** module on my personal webpage (here).
+Below is the list of all functions accessible from the library. It is
+recommended to first experiment with the functions presented in the [Data
+Generation](#data-generation) section. ### Population and Allele Frequency
+Spectrum Modeling ```python def stochastic_line(a: float,b: float,sigma: float)
+-> Callable[float,float] ``` ```python population_mut = stochastic_line
+(0.08,0.17,0.01) ``` ```python def afs_distribution(index: int,alpha: float =
+4/30) -> float ``` ```python def afs_intervals(pick: float,alpha: float = 4/30)
+-> list[float] ``` ```python def afs_sample(alpha: float = 4/30) -> float ```
+```python def genotype_schema(alpha: float = 4/30) -> tuple[float,list[float]]
+``` ```python def genotype(hwp: list[float],minor: int) -> tuple[int,int] ```
+```python gref = lambda g: g[0] if g[0] in [2,0] else g[1] ``` ```python def
+population_mld(t: float) -> tuple[float,float,float] ``` ### LD and
+HardyâWeinberg Principle Modeling ```python def decay(initial:
+float,halfwidth: float,shift: float) -> Callable[float,float] ``` ```python def
+ref_alt_function(y: float,x: float) -> float ``` ```python def alt_alt_function
+(y: float,z: float,x: float) -> float ``` ```python def amplifier(beta:
+float,p: float,q: float,s: float = 1) -> float ``` ```python def lb_freq(beta:
 float,gamma: float,previous_freq: float,distance: float,shift: float) -> float
-``` ```python def linkage_disequilibrium(alpha: float,beta: float,gamma:
-float,strength: float = -1) -> Callable[float,Callabel[float,tuple
-[float,float]]] ``` ```python def cond_genotype_schema(previous_maf:
-float,distance: float,alpha: float,beta: float,gamma: float,strength: float = -
-1) -> tuple[float,list[float],float] ``` ### Data Generation ```python def
-SNP_distribution(reference: float,length: float) -> list[float] ```
-**Description** - generates the list of positions for the VCF file ```python
-def initiate_block(reference: float,alpha: float,Npop: int = 1000) -> tuple
-[float,list[list],list[list]] ``` **Description** - initializes the first LD-
-block of the simulation - the parameter ```reference``` refers to the first
-locus position at which the generation starts ```python def continue_block
-(maf0: float,pre_matrix: list[list],matrix: list[list],positions: list
-[float],alpha: float,beta: float,gamma: float,strength: int = -1,Npop: int =
-1000) -> tuple[float,list[list],list[list]] ``` **Description** - generates an
-LD-block from a given position with a given minor allele frequency - augments
-the genomic matrix with further genetic variants as specified by the arguments
-```python def genmatrix(blocks: list[int],strength: float,population:
-float,Npop: int) ``` **Description** - implements a basic genomic matrix
-generator using ```SNP_distribution()```, ```initiate_block()``` and
-```continue_block()``` - _note:_ many possible improvements or variations of
-this function are possible (see tutorial here for more detail) ```python def
-gt_vcf(value: int)-> str ``` ```python def create_vcfgz(vcf_name: str,matrix:
-list[list],alpha: float,beta: float,gamma: float,system: str = "unix") -> None
-``` **Description** - generates a VCF file from a ```matrix``` generated by
-```initiate_block()```, ```continue_block()``` or ```genmatrix()``` ### LD
-Analytics ```python def LD_corr_matrix(matrix: list[list]) -> tuple[list
-[list],float,list[float]] ``` **Description** - generates a (non-normalized)
-correlation matrix from a ```matrix``` generated by ```initiate_block()```,
-```continue_block()``` or ```genmatrix()``` ```python def LD_r2_matrix
-(pre_matrix: list[list]) -> tuple[list[list],float,list[float]] ```
-**Description** - generates a (non-normalized) LD-r2 matrix from a
+``` ```python def ub_freq(beta: float,gamma: float,previous_freq:
+float,distance: float,shift: float) -> float ``` ```python def
+linkage_disequilibrium(alpha: float,beta: float,gamma: float,strength: float =
+-1) -> Callable[float,Callabel[float,tuple[float,float]]] ``` ```python def
+cond_genotype_schema(previous_maf: float,distance: float,alpha: float,beta:
+float,gamma: float,strength: float = -1) -> tuple[float,list[float],float] ```
+### Data Generation ```python def SNP_distribution(reference: float,length:
+float) -> list[float] ``` **Description** - generates the list of positions for
+the VCF file ```python def initiate_block(reference: float,alpha: float,Npop:
+int = 1000) -> tuple[float,list[list],list[list]] ``` **Description** -
+initializes the first LD-block of the simulation - the parameter
+```reference``` refers to the first locus position at which the generation
+starts ```python def continue_block(maf0: float,pre_matrix: list[list],matrix:
+list[list],positions: list[float],alpha: float,beta: float,gamma:
+float,strength: int = -1,Npop: int = 1000) -> tuple[float,list[list],list
+[list]] ``` **Description** - generates an LD-block from a given position with
+a given minor allele frequency - augments the genomic matrix with further
+genetic variants as specified by the arguments ```python def genmatrix(blocks:
+list[int],strength: float,population: float,Npop: int) ``` **Description** -
+implements a basic genomic matrix generator using ```SNP_distribution()```,
+```initiate_block()``` and ```continue_block()``` - _note:_ many possible
+improvements or variations of this function are possible (see tutorial here for
+more detail) ```python def gt_vcf(value: int)-> str ``` ```python def
+create_vcfgz(vcf_name: str,matrix: list[list],alpha: float,beta: float,gamma:
+float,system: str = "unix") -> None ``` **Description** - generates a VCF file
+from a ```matrix``` generated by ```initiate_block()```, ```continue_block()```
+or ```genmatrix()``` ### LD Analytics ```python def LD_corr_matrix(matrix: list
+[list]) -> tuple[list[list],float,list[float]] ``` **Description** - generates
+a (non-normalized) correlation matrix from a ```matrix``` generated by
+```initiate_block()```, ```continue_block()``` or ```genmatrix()``` ```python
+def LD_r2_matrix(pre_matrix: list[list]) -> tuple[list[list],float,list[float]]
+``` **Description** - generates a (non-normalized) LD-r2 matrix from a
 ```pre_matrix``` generated by ```initiate_block()```, ```continue_block()``` -
 _note:_ this function cannot be used with ```genmatrix()``` since the
 ```pre_matrix``` is not returned ```python def display(rel: list[list],m:
 float) -> list[list[tuple[float,float,float]]] ``` ```python def
-minor_haplotype(sub_pre_matrix: list[list]) -> float ```
+minor_haplotype(sub_pre_matrix: list[list]) -> float ``` ## Classes from
+Framework To be added.
```

### Comparing `HaploDynamics-0.1b9/LICENSE` & `HaploDynamics-0.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `HaploDynamics-0.1b9/PKG-INFO` & `HaploDynamics-0.2b0/HaploDynamics.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: HaploDynamics
-Version: 0.1b9
+Version: 0.2b0
 Summary: A python library to develop genomic data simulators
 Home-page: https://github.com/remytuyeras/HaploDynamics
-Download-URL: https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.9.tar.gz
+Download-URL: https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.2-beta.0.tar.gz
 Author: Remy Tuyeras
 Author-email: rtuyeras@gmail.com
 License: gpl-3.0
 Keywords: Simulator,Genomics,Genomic,Microarray,SNP chip,VCF,Linkage disequilibrium,Hardy-Weinberg equilibrium
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -19,43 +19,43 @@
 License-File: LICENSE
 
 # HaploDynamics
 The python library **HaploDynamics**, or **HaploDX** for short, provides a collection of functions that can be used to simulate population-specific genomic data. This package is part of the Genetic Simulator Resources (GSR) catalog (click the link below for more information).
 
 <div style="width: 180px; margin: 0 auto;"><a href="https://surveillance.cancer.gov/genetic-simulation-resources/"><img src="https://surveillance.cancer.gov/gsr/static/img/gsr_tile.jpg" alt="Catalogued on GSR" width="180" height="60" /></a></div>
 
-## News
+## New features recently added
 
-* Adding installation procedure via ```pip```
-* Adding the module ```Framework``` for a class-based development framework
+* Installation via ```pip```;
+* A class-based module ```Framework``` for software development and experimentations.
 
 ## Installation
 
 ### Manual installation
-Download the github package using the following command.
+Download the github package by using the following command in a terminal.
 ```bash
 $ git clone https://github.com/remytuyeras/HaploDynamics.git
 ```
-Then, from your current directory, record the absolute path leading to the main module of the package, as shown below.
+Then, from your current directory, record the absolute path leading to the downloaded package, as shown below.
 ```bash
 $ ls
 HaploDynamics
 $ cd HaploDynamics/
 $ pwd
-path/to/main/module/HaploDynamics
+absolute/path/to/HaploDynamics
 ```
-To import the modules of the library to your script, use the following syntax where you must replace ```path/to/main/module/HaploDynamics``` with the path that you obtained above.
+To import the modules of the library to your script, use the following syntax where you need replace ```absolute/path/to/HaploDynamics``` with the path that you obtained above.
 ```python
 import sys
-sys.path.insert (0,"path/to/main/module/HaploDynamics")
+sys.path.insert (0,"absolute/path/to/HaploDynamics")
 import HaploDynamics.HaploDX as hdx
 import HaploDynamics.Framework as hdx_frm
 ```
-### Pip [still in progress]
-Install the package using ```pip install``` as follows.
+### Installation via Pip
+Install the package by using ```pip install``` as follows.
 ```bash
 $ pip install HaploDynamics
 ```
 Then, you can import the modules of the library to your script as follows.
 ```python
 import HaploDynamics.HaploDX as hdx
 import HaploDynamics.Framework as hdx_frm
@@ -75,38 +75,95 @@
 Parameters | Type | Values
 | :--- | :--- | :---
 ```blocks```  | ```list[int]``` | List of positive integers, ideally between 1 and 40.
 ```strength```  | ```float``` | From -1 (little linkage) to 1 (high linkage)
 ```population```  | ```float``` | From 0 (for more rare mutations) to 1 (for less rare mutations)
 ```Npop```  | ```int```  | Positive integer specifying the number of individuals in the genomic matrix
 
-The generation of each locus in a VCF file tend to be linear in the parameter ```Npop```. For example, one genetic variant can take from 0.3 to 0.8 seconds to be generated/simulated when we set ```Npop=100000``` (this may vary depending on your machine). The estimated time complexity for an average machine is shown below.
+The generation of each locus in a VCF file tends to be linear in the parameter ```Npop```. On average, a genetic variant can take from 0.3 to 0.8 seconds to be generated when ```Npop=100000``` (this may vary depending on your machine). The estimated time complexity for an average machine is shown below.
 
-![GitHub Logo](/time_complexity.png)
+![](/img/time_complexity.png) 
 
-The following script shows how to display the linkage disequilibirum correlations associated with the simulated data.
+## Use cases
+The following script shows how to display linkage disequilibirum correlations for the simulated data.
 ```python
 import matplotlib.pyplot as plt
 import HaploDynamics.HaploDX as hdx
 
-simulated_data = hdx.genmatrix([20,5,20,35,30,15],strength=1,population=0.1,Npop=1000)
+simulated_data = hdx.genmatrix([20,20,20,20,20,20],strength=1,population=0.1,Npop=1000)
 hdx.create_vcfgz("genomic-data.simulation.v1",*simulated_data)
 
 rel, m, _ = hdx.LD_corr_matrix(simulated_data[0])
 plt.imshow(hdx.display(rel,m))
 plt.show()
 ```
-The following plot is an example of the output that can be returned by the previous script when using 6 LD-blocks of 20kb each.
+A typical output for the previous script should look as follows.
+![](/img/simulation_LD_0.png) 
 
-![alt text](http://www.normalesup.org/~tuyeras/node_diss/blg/blg_stat/img/LD_block_corr_strength_high.png)
+The following script shows how you can control linkage disequilibrium by using LD-blocks of varying legnths. You can display the graph relating distances between pairs of SNPS to average correlation scores by using the last output of the function ```LD_corr_matrix()```.
 
+```python
+import matplotlib.pyplot as plt
+import HaploDynamics.HaploDX as hdx
 
-## HaploDX Functions
+ld_blocks = [5,5,5,10,20,5,5,5,5,5,5,1,1,1,2,2,10,20,40]
+strength=1
+population=0.1
+Npop = 1000
+simulated_data = hdx.genmatrix(ld_blocks,strength,population,Npop)
+hdx.create_vcfgz("genomic-data.simulation.v1",*simulated_data)
 
-You can find a complete presentation (or in fact a thorough tutorial) of the **HaploDX** library on my personal webpage (<a href="https://www.normalesup.org/~tuyeras/node_diss/blg/home.php?page=blg_stat/stat_1/home.php">here</a>). Below is the list of all functions accessible from the library. It is recommended to first experiment with the functions presented in the [Data Generation](#data-generation) section.
+#Correlations
+rel, m, dist = hdx.LD_corr_matrix(simulated_data[0])
+plt.imshow(hdx.display(rel,m))
+plt.show()
+
+#from SNP-distance to average correlaions
+plt.plot([i for i in range(len(dist)-1)],dist[1:])
+plt.ylim([0, 1])
+plt.show()
+```
+Typical outputs for the previous script should look as follows.
+
+Correlations            |  SNP-distance to average correlations
+:-------------------------:|:-------------------------:
+![](/img/simulation_LD_1.png)  |  ![](/img/simulation_dist_1.png)
+
+Finally, the following script shows how you can generate large regions of linkage.
+
+```python
+import matplotlib.pyplot as plt
+import HaploDynamics.HaploDX as hdx
+
+ld_blocks = [1] * 250
+strength=1
+population=0.1
+Npop = 1000
+simulated_data = hdx.genmatrix(ld_blocks,strength,population,Npop)
+hdx.create_vcfgz("genomic-data.simulation.v1",*simulated_data)
+
+#Correlations
+rel, m, dist = hdx.LD_corr_matrix(simulated_data[0])
+plt.imshow(hdx.display(rel,m))
+plt.show()
+
+#from SNP-distance to average correlaions
+plt.plot([i for i in range(len(dist)-1)],dist[1:])
+plt.ylim([0, 1])
+plt.show()
+```
+Typical outputs for the previous script should look as follows.
+
+Correlations            |  SNP-distance to average correlations
+:-------------------------:|:-------------------------:
+![](/img/simulation_LD_2.png)  |  ![](/img/simulation_dist_2.png)
+
+## Functions from HaploDX
+
+You can find a complete presentation (or in fact a thorough tutorial) of the **HaploDX** module on my personal webpage (<a href="https://www.normalesup.org/~tuyeras/node_diss/blg/home.php?page=blg_stat/stat_1/home.php">here</a>). Below is the list of all functions accessible from the library. It is recommended to first experiment with the functions presented in the [Data Generation](#data-generation) section.
 
 ### Population and Allele Frequency Spectrum Modeling
 
 ```python
 def stochastic_line(a: float,b: float,sigma: float) -> Callable[float,float]
 ```
 ```python
@@ -211,7 +268,11 @@
 - _note:_ this function cannot be used with ```genmatrix()``` since the ```pre_matrix``` is not returned
 ```python
 def display(rel: list[list],m: float) -> list[list[tuple[float,float,float]]]
 ```
 ```python
 def minor_haplotype(sub_pre_matrix: list[list]) -> float
 ```
+
+## Classes from Framework
+
+To be added.
```

#### html2text {}

```diff
@@ -1,119 +1,142 @@
-Metadata-Version: 2.1 Name: HaploDynamics Version: 0.1b9 Summary: A python
+Metadata-Version: 2.1 Name: HaploDynamics Version: 0.2b0 Summary: A python
 library to develop genomic data simulators Home-page: https://github.com/
 remytuyeras/HaploDynamics Download-URL: https://github.com/remytuyeras/
-HaploDynamics/archive/refs/tags/v0.1-beta.9.tar.gz Author: Remy Tuyeras Author-
+HaploDynamics/archive/refs/tags/v0.2-beta.0.tar.gz Author: Remy Tuyeras Author-
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
-## News * Adding installation procedure via ```pip``` * Adding the module
-```Framework``` for a class-based development framework ## Installation ###
-Manual installation Download the github package using the following command.
-```bash $ git clone https://github.com/remytuyeras/HaploDynamics.git ``` Then,
-from your current directory, record the absolute path leading to the main
-module of the package, as shown below. ```bash $ ls HaploDynamics $ cd
-HaploDynamics/ $ pwd path/to/main/module/HaploDynamics ``` To import the
-modules of the library to your script, use the following syntax where you must
-replace ```path/to/main/module/HaploDynamics``` with the path that you obtained
-above. ```python import sys sys.path.insert (0,"path/to/main/module/
+## New features recently added * Installation via ```pip```; * A class-based
+module ```Framework``` for software development and experimentations. ##
+Installation ### Manual installation Download the github package by using the
+following command in a terminal. ```bash $ git clone https://github.com/
+remytuyeras/HaploDynamics.git ``` Then, from your current directory, record the
+absolute path leading to the downloaded package, as shown below. ```bash $ ls
+HaploDynamics $ cd HaploDynamics/ $ pwd absolute/path/to/HaploDynamics ``` To
+import the modules of the library to your script, use the following syntax
+where you need replace ```absolute/path/to/HaploDynamics``` with the path that
+you obtained above. ```python import sys sys.path.insert (0,"absolute/path/to/
 HaploDynamics") import HaploDynamics.HaploDX as hdx import
-HaploDynamics.Framework as hdx_frm ``` ### Pip [still in progress] Install the
-package using ```pip install``` as follows. ```bash $ pip install HaploDynamics
-``` Then, you can import the modules of the library to your script as follows.
-```python import HaploDynamics.HaploDX as hdx import HaploDynamics.Framework as
-hdx_frm ``` ## Quick start The following script generates a VCF file containing
-simulated diploid genotypes for a population of 1000 individuals with LD-blocks
-of length 20kb, 5kb, 20kb, 35kb, 30kb and 15kb. ```python import
-HaploDynamics.HaploDX as hdx simulated_data = hdx.genmatrix(
+HaploDynamics.Framework as hdx_frm ``` ### Installation via Pip Install the
+package by using ```pip install``` as follows. ```bash $ pip install
+HaploDynamics ``` Then, you can import the modules of the library to your
+script as follows. ```python import HaploDynamics.HaploDX as hdx import
+HaploDynamics.Framework as hdx_frm ``` ## Quick start The following script
+generates a VCF file containing simulated diploid genotypes for a population of
+1000 individuals with LD-blocks of length 20kb, 5kb, 20kb, 35kb, 30kb and 15kb.
+```python import HaploDynamics.HaploDX as hdx simulated_data = hdx.genmatrix(
 [20,5,20,35,30,15],strength=1,population=0.1,Npop=1000) hdx.create_vcfgz
 ("genomic-data.simulation.v1",*simulated_data) ``` The equation
 ```strength=1``` forces a high amount of linkage disequilibrium and the
 equation ```population=0.1``` increases the likelyhood of the simulated
 population to have rare mutations (e.g. to simulate a population profile close
 to African and South-Asian populations). More generally, the function
 ```genmatrix()``` takes the following types of parameters: Parameters | Type |
 Values | :--- | :--- | :--- ```blocks``` | ```list[int]``` | List of positive
 integers, ideally between 1 and 40. ```strength``` | ```float``` | From -1
 (little linkage) to 1 (high linkage) ```population``` | ```float``` | From 0
 (for more rare mutations) to 1 (for less rare mutations) ```Npop``` | ```int```
 | Positive integer specifying the number of individuals in the genomic matrix
-The generation of each locus in a VCF file tend to be linear in the parameter
-```Npop```. For example, one genetic variant can take from 0.3 to 0.8 seconds
-to be generated/simulated when we set ```Npop=100000``` (this may vary
-depending on your machine). The estimated time complexity for an average
-machine is shown below. ![GitHub Logo](/time_complexity.png) The following
-script shows how to display the linkage disequilibirum correlations associated
-with the simulated data. ```python import matplotlib.pyplot as plt import
-HaploDynamics.HaploDX as hdx simulated_data = hdx.genmatrix(
-[20,5,20,35,30,15],strength=1,population=0.1,Npop=1000) hdx.create_vcfgz
-("genomic-data.simulation.v1",*simulated_data) rel, m, _ = hdx.LD_corr_matrix
-(simulated_data[0]) plt.imshow(hdx.display(rel,m)) plt.show() ``` The following
-plot is an example of the output that can be returned by the previous script
-when using 6 LD-blocks of 20kb each. ![alt text](http://www.normalesup.org/
-~tuyeras/node_diss/blg/blg_stat/img/LD_block_corr_strength_high.png) ## HaploDX
-Functions You can find a complete presentation (or in fact a thorough tutorial)
-of the **HaploDX** library on my personal webpage (here). Below is the list of
-all functions accessible from the library. It is recommended to first
-experiment with the functions presented in the [Data Generation](#data-
-generation) section. ### Population and Allele Frequency Spectrum Modeling
-```python def stochastic_line(a: float,b: float,sigma: float) -> Callable
-[float,float] ``` ```python population_mut = stochastic_line(0.08,0.17,0.01)
-``` ```python def afs_distribution(index: int,alpha: float = 4/30) -> float ```
-```python def afs_intervals(pick: float,alpha: float = 4/30) -> list[float] ```
-```python def afs_sample(alpha: float = 4/30) -> float ``` ```python def
-genotype_schema(alpha: float = 4/30) -> tuple[float,list[float]] ``` ```python
-def genotype(hwp: list[float],minor: int) -> tuple[int,int] ``` ```python gref
-= lambda g: g[0] if g[0] in [2,0] else g[1] ``` ```python def population_mld(t:
-float) -> tuple[float,float,float] ``` ### LD and HardyâWeinberg Principle
-Modeling ```python def decay(initial: float,halfwidth: float,shift: float) -
-> Callable[float,float] ``` ```python def ref_alt_function(y: float,x: float) -
-> float ``` ```python def alt_alt_function(y: float,z: float,x: float) -> float
-``` ```python def amplifier(beta: float,p: float,q: float,s: float = 1) -
-> float ``` ```python def lb_freq(beta: float,gamma: float,previous_freq:
-float,distance: float,shift: float) -> float ``` ```python def ub_freq(beta:
+The generation of each locus in a VCF file tends to be linear in the parameter
+```Npop```. On average, a genetic variant can take from 0.3 to 0.8 seconds to
+be generated when ```Npop=100000``` (this may vary depending on your machine).
+The estimated time complexity for an average machine is shown below. ![](/img/
+time_complexity.png) ## Use cases The following script shows how to display
+linkage disequilibirum correlations for the simulated data. ```python import
+matplotlib.pyplot as plt import HaploDynamics.HaploDX as hdx simulated_data =
+hdx.genmatrix([20,20,20,20,20,20],strength=1,population=0.1,Npop=1000)
+hdx.create_vcfgz("genomic-data.simulation.v1",*simulated_data) rel, m, _ =
+hdx.LD_corr_matrix(simulated_data[0]) plt.imshow(hdx.display(rel,m)) plt.show()
+``` A typical output for the previous script should look as follows. ![](/img/
+simulation_LD_0.png) The following script shows how you can control linkage
+disequilibrium by using LD-blocks of varying legnths. You can display the graph
+relating distances between pairs of SNPS to average correlation scores by using
+the last output of the function ```LD_corr_matrix()```. ```python import
+matplotlib.pyplot as plt import HaploDynamics.HaploDX as hdx ld_blocks =
+[5,5,5,10,20,5,5,5,5,5,5,1,1,1,2,2,10,20,40] strength=1 population=0.1 Npop =
+1000 simulated_data = hdx.genmatrix(ld_blocks,strength,population,Npop)
+hdx.create_vcfgz("genomic-data.simulation.v1",*simulated_data) #Correlations
+rel, m, dist = hdx.LD_corr_matrix(simulated_data[0]) plt.imshow(hdx.display
+(rel,m)) plt.show() #from SNP-distance to average correlaions plt.plot([i for i
+in range(len(dist)-1)],dist[1:]) plt.ylim([0, 1]) plt.show() ``` Typical
+outputs for the previous script should look as follows. Correlations | SNP-
+distance to average correlations :-------------------------:|:-----------------
+--------: ![](/img/simulation_LD_1.png) | ![](/img/simulation_dist_1.png)
+Finally, the following script shows how you can generate large regions of
+linkage. ```python import matplotlib.pyplot as plt import HaploDynamics.HaploDX
+as hdx ld_blocks = [1] * 250 strength=1 population=0.1 Npop = 1000
+simulated_data = hdx.genmatrix(ld_blocks,strength,population,Npop)
+hdx.create_vcfgz("genomic-data.simulation.v1",*simulated_data) #Correlations
+rel, m, dist = hdx.LD_corr_matrix(simulated_data[0]) plt.imshow(hdx.display
+(rel,m)) plt.show() #from SNP-distance to average correlaions plt.plot([i for i
+in range(len(dist)-1)],dist[1:]) plt.ylim([0, 1]) plt.show() ``` Typical
+outputs for the previous script should look as follows. Correlations | SNP-
+distance to average correlations :-------------------------:|:-----------------
+--------: ![](/img/simulation_LD_2.png) | ![](/img/simulation_dist_2.png) ##
+Functions from HaploDX You can find a complete presentation (or in fact a
+thorough tutorial) of the **HaploDX** module on my personal webpage (here).
+Below is the list of all functions accessible from the library. It is
+recommended to first experiment with the functions presented in the [Data
+Generation](#data-generation) section. ### Population and Allele Frequency
+Spectrum Modeling ```python def stochastic_line(a: float,b: float,sigma: float)
+-> Callable[float,float] ``` ```python population_mut = stochastic_line
+(0.08,0.17,0.01) ``` ```python def afs_distribution(index: int,alpha: float =
+4/30) -> float ``` ```python def afs_intervals(pick: float,alpha: float = 4/30)
+-> list[float] ``` ```python def afs_sample(alpha: float = 4/30) -> float ```
+```python def genotype_schema(alpha: float = 4/30) -> tuple[float,list[float]]
+``` ```python def genotype(hwp: list[float],minor: int) -> tuple[int,int] ```
+```python gref = lambda g: g[0] if g[0] in [2,0] else g[1] ``` ```python def
+population_mld(t: float) -> tuple[float,float,float] ``` ### LD and
+HardyâWeinberg Principle Modeling ```python def decay(initial:
+float,halfwidth: float,shift: float) -> Callable[float,float] ``` ```python def
+ref_alt_function(y: float,x: float) -> float ``` ```python def alt_alt_function
+(y: float,z: float,x: float) -> float ``` ```python def amplifier(beta:
+float,p: float,q: float,s: float = 1) -> float ``` ```python def lb_freq(beta:
 float,gamma: float,previous_freq: float,distance: float,shift: float) -> float
-``` ```python def linkage_disequilibrium(alpha: float,beta: float,gamma:
-float,strength: float = -1) -> Callable[float,Callabel[float,tuple
-[float,float]]] ``` ```python def cond_genotype_schema(previous_maf:
-float,distance: float,alpha: float,beta: float,gamma: float,strength: float = -
-1) -> tuple[float,list[float],float] ``` ### Data Generation ```python def
-SNP_distribution(reference: float,length: float) -> list[float] ```
-**Description** - generates the list of positions for the VCF file ```python
-def initiate_block(reference: float,alpha: float,Npop: int = 1000) -> tuple
-[float,list[list],list[list]] ``` **Description** - initializes the first LD-
-block of the simulation - the parameter ```reference``` refers to the first
-locus position at which the generation starts ```python def continue_block
-(maf0: float,pre_matrix: list[list],matrix: list[list],positions: list
-[float],alpha: float,beta: float,gamma: float,strength: int = -1,Npop: int =
-1000) -> tuple[float,list[list],list[list]] ``` **Description** - generates an
-LD-block from a given position with a given minor allele frequency - augments
-the genomic matrix with further genetic variants as specified by the arguments
-```python def genmatrix(blocks: list[int],strength: float,population:
-float,Npop: int) ``` **Description** - implements a basic genomic matrix
-generator using ```SNP_distribution()```, ```initiate_block()``` and
-```continue_block()``` - _note:_ many possible improvements or variations of
-this function are possible (see tutorial here for more detail) ```python def
-gt_vcf(value: int)-> str ``` ```python def create_vcfgz(vcf_name: str,matrix:
-list[list],alpha: float,beta: float,gamma: float,system: str = "unix") -> None
-``` **Description** - generates a VCF file from a ```matrix``` generated by
-```initiate_block()```, ```continue_block()``` or ```genmatrix()``` ### LD
-Analytics ```python def LD_corr_matrix(matrix: list[list]) -> tuple[list
-[list],float,list[float]] ``` **Description** - generates a (non-normalized)
-correlation matrix from a ```matrix``` generated by ```initiate_block()```,
-```continue_block()``` or ```genmatrix()``` ```python def LD_r2_matrix
-(pre_matrix: list[list]) -> tuple[list[list],float,list[float]] ```
-**Description** - generates a (non-normalized) LD-r2 matrix from a
+``` ```python def ub_freq(beta: float,gamma: float,previous_freq:
+float,distance: float,shift: float) -> float ``` ```python def
+linkage_disequilibrium(alpha: float,beta: float,gamma: float,strength: float =
+-1) -> Callable[float,Callabel[float,tuple[float,float]]] ``` ```python def
+cond_genotype_schema(previous_maf: float,distance: float,alpha: float,beta:
+float,gamma: float,strength: float = -1) -> tuple[float,list[float],float] ```
+### Data Generation ```python def SNP_distribution(reference: float,length:
+float) -> list[float] ``` **Description** - generates the list of positions for
+the VCF file ```python def initiate_block(reference: float,alpha: float,Npop:
+int = 1000) -> tuple[float,list[list],list[list]] ``` **Description** -
+initializes the first LD-block of the simulation - the parameter
+```reference``` refers to the first locus position at which the generation
+starts ```python def continue_block(maf0: float,pre_matrix: list[list],matrix:
+list[list],positions: list[float],alpha: float,beta: float,gamma:
+float,strength: int = -1,Npop: int = 1000) -> tuple[float,list[list],list
+[list]] ``` **Description** - generates an LD-block from a given position with
+a given minor allele frequency - augments the genomic matrix with further
+genetic variants as specified by the arguments ```python def genmatrix(blocks:
+list[int],strength: float,population: float,Npop: int) ``` **Description** -
+implements a basic genomic matrix generator using ```SNP_distribution()```,
+```initiate_block()``` and ```continue_block()``` - _note:_ many possible
+improvements or variations of this function are possible (see tutorial here for
+more detail) ```python def gt_vcf(value: int)-> str ``` ```python def
+create_vcfgz(vcf_name: str,matrix: list[list],alpha: float,beta: float,gamma:
+float,system: str = "unix") -> None ``` **Description** - generates a VCF file
+from a ```matrix``` generated by ```initiate_block()```, ```continue_block()```
+or ```genmatrix()``` ### LD Analytics ```python def LD_corr_matrix(matrix: list
+[list]) -> tuple[list[list],float,list[float]] ``` **Description** - generates
+a (non-normalized) correlation matrix from a ```matrix``` generated by
+```initiate_block()```, ```continue_block()``` or ```genmatrix()``` ```python
+def LD_r2_matrix(pre_matrix: list[list]) -> tuple[list[list],float,list[float]]
+``` **Description** - generates a (non-normalized) LD-r2 matrix from a
 ```pre_matrix``` generated by ```initiate_block()```, ```continue_block()``` -
 _note:_ this function cannot be used with ```genmatrix()``` since the
 ```pre_matrix``` is not returned ```python def display(rel: list[list],m:
 float) -> list[list[tuple[float,float,float]]] ``` ```python def
-minor_haplotype(sub_pre_matrix: list[list]) -> float ```
+minor_haplotype(sub_pre_matrix: list[list]) -> float ``` ## Classes from
+Framework To be added.
```

### Comparing `HaploDynamics-0.1b9/setup.py` & `HaploDynamics-0.2b0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
   name = 'HaploDynamics',
   packages=setuptools.find_packages(include=['HaploDynamics','HaploDynamics.HaploDX','HaploDynamics.Framework']),
-  version = 'v0.1-beta.9',
+  version = 'v0.2-beta.0',
   license='gpl-3.0',
   author = 'Remy Tuyeras',
   author_email = 'rtuyeras@gmail.com',
   description = 'A python library to develop genomic data simulators',
   long_description = long_description,
   long_description_content_type = "text/markdown",
   url = 'https://github.com/remytuyeras/HaploDynamics',
-  download_url = 'https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.9.tar.gz',
+  download_url = 'https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.2-beta.0.tar.gz',
   keywords = ['Simulator', 'Genomics', 'Genomic', 'Microarray','SNP chip','VCF', 'Linkage disequilibrium', 'Hardy-Weinberg equilibrium'],
   install_requires=['scipy'],
   classifiers=[
     'Development Status :: 4 - Beta',  #"3 - Alpha", "4 - Beta" or "5 - Production/Stable"
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'Topic :: Software Development :: Build Tools',
```

