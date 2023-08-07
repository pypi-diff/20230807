# Comparing `tmp/HaploDynamics-0.1b2.tar.gz` & `tmp/HaploDynamics-0.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HaploDynamics-0.1b2.tar", last modified: Sun Aug  6 18:47:44 2023, max compression
+gzip compressed data, was "HaploDynamics-0.1b3.tar", last modified: Sun Aug  6 18:54:15 2023, max compression
```

## Comparing `HaploDynamics-0.1b2.tar` & `HaploDynamics-0.1b3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-06 18:47:44.710133 HaploDynamics-0.1b2/
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-06 18:47:44.710133 HaploDynamics-0.1b2/Framework/
--rw-rw-r--   0 remy      (1000) remy      (1000)       22 2023-08-06 17:58:56.000000 HaploDynamics-0.1b2/Framework/__init__.py
--rw-rw-r--   0 remy      (1000) remy      (1000)       67 2023-08-06 18:02:03.000000 HaploDynamics-0.1b2/Framework/future.py
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-06 18:47:44.710133 HaploDynamics-0.1b2/HaploDX/
--rw-rw-r--   0 remy      (1000) remy      (1000)    17508 2023-08-06 17:21:31.000000 HaploDynamics-0.1b2/HaploDX/HaploDX.py
--rw-rw-r--   0 remy      (1000) remy      (1000)       23 2023-08-06 17:50:46.000000 HaploDynamics-0.1b2/HaploDX/__init__.py
-drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-06 18:47:44.710133 HaploDynamics-0.1b2/HaploDynamics.egg-info/
--rw-rw-r--   0 remy      (1000) remy      (1000)     8398 2023-08-06 18:47:44.000000 HaploDynamics-0.1b2/HaploDynamics.egg-info/PKG-INFO
--rw-rw-r--   0 remy      (1000) remy      (1000)      301 2023-08-06 18:47:44.000000 HaploDynamics-0.1b2/HaploDynamics.egg-info/SOURCES.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)        1 2023-08-06 18:47:44.000000 HaploDynamics-0.1b2/HaploDynamics.egg-info/dependency_links.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)        6 2023-08-06 18:47:44.000000 HaploDynamics-0.1b2/HaploDynamics.egg-info/requires.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)       18 2023-08-06 18:47:44.000000 HaploDynamics-0.1b2/HaploDynamics.egg-info/top_level.txt
--rw-rw-r--   0 remy      (1000) remy      (1000)    35149 2023-08-06 17:21:31.000000 HaploDynamics-0.1b2/LICENSE
--rw-rw-r--   0 remy      (1000) remy      (1000)     8398 2023-08-06 18:47:44.710133 HaploDynamics-0.1b2/PKG-INFO
--rw-rw-r--   0 remy      (1000) remy      (1000)     7514 2023-08-06 17:21:31.000000 HaploDynamics-0.1b2/README.md
--rw-rw-r--   0 remy      (1000) remy      (1000)       79 2023-08-06 18:47:44.710133 HaploDynamics-0.1b2/setup.cfg
--rw-rw-r--   0 remy      (1000) remy      (1000)     1213 2023-08-06 18:46:05.000000 HaploDynamics-0.1b2/setup.py
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-06 18:54:15.142546 HaploDynamics-0.1b3/
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-06 18:54:15.142546 HaploDynamics-0.1b3/Framework/
+-rw-rw-r--   0 remy      (1000) remy      (1000)       22 2023-08-06 18:51:05.000000 HaploDynamics-0.1b3/Framework/__init__.py
+-rw-rw-r--   0 remy      (1000) remy      (1000)       67 2023-08-06 18:51:05.000000 HaploDynamics-0.1b3/Framework/future.py
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-06 18:54:15.142546 HaploDynamics-0.1b3/HaploDX/
+-rw-rw-r--   0 remy      (1000) remy      (1000)    17508 2023-08-06 18:51:05.000000 HaploDynamics-0.1b3/HaploDX/HaploDX.py
+-rw-rw-r--   0 remy      (1000) remy      (1000)       23 2023-08-06 18:51:05.000000 HaploDynamics-0.1b3/HaploDX/__init__.py
+drwxrwxr-x   0 remy      (1000) remy      (1000)        0 2023-08-06 18:54:15.142546 HaploDynamics-0.1b3/HaploDynamics.egg-info/
+-rw-rw-r--   0 remy      (1000) remy      (1000)     8396 2023-08-06 18:54:15.000000 HaploDynamics-0.1b3/HaploDynamics.egg-info/PKG-INFO
+-rw-rw-r--   0 remy      (1000) remy      (1000)      301 2023-08-06 18:54:15.000000 HaploDynamics-0.1b3/HaploDynamics.egg-info/SOURCES.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)        1 2023-08-06 18:54:15.000000 HaploDynamics-0.1b3/HaploDynamics.egg-info/dependency_links.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)        6 2023-08-06 18:54:15.000000 HaploDynamics-0.1b3/HaploDynamics.egg-info/requires.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)       18 2023-08-06 18:54:15.000000 HaploDynamics-0.1b3/HaploDynamics.egg-info/top_level.txt
+-rw-rw-r--   0 remy      (1000) remy      (1000)    35149 2023-08-06 18:51:05.000000 HaploDynamics-0.1b3/LICENSE
+-rw-rw-r--   0 remy      (1000) remy      (1000)     8396 2023-08-06 18:54:15.142546 HaploDynamics-0.1b3/PKG-INFO
+-rw-rw-r--   0 remy      (1000) remy      (1000)     7512 2023-08-06 18:51:05.000000 HaploDynamics-0.1b3/README.md
+-rw-rw-r--   0 remy      (1000) remy      (1000)       79 2023-08-06 18:54:15.142546 HaploDynamics-0.1b3/setup.cfg
+-rw-rw-r--   0 remy      (1000) remy      (1000)     1213 2023-08-06 18:51:19.000000 HaploDynamics-0.1b3/setup.py
```

### Comparing `HaploDynamics-0.1b2/HaploDX/HaploDX.py` & `HaploDynamics-0.1b3/HaploDX/HaploDX.py`

 * *Files identical despite different names*

### Comparing `HaploDynamics-0.1b2/HaploDynamics.egg-info/PKG-INFO` & `HaploDynamics-0.1b3/HaploDynamics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: HaploDynamics
-Version: 0.1b2
+Version: 0.1b3
 Summary: A python library to develop genomic data simulators
 Home-page: https://github.com/remytuyeras/HaploDynamics
-Download-URL: https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.2.tar.gz
+Download-URL: https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.3.tar.gz
 Author: Remy Tuyeras
 Author-email: rtuyeras@gmail.com
 License: gpl-3.0
 Keywords: Simulator,Genomics,Genomic,Microarray,SNP chip,VCF,Linkage disequilibrium,Hardy-Weinberg equilibrium
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -21,32 +21,35 @@
 # HaploDynamics
 The python library **HaploDynamics**, or **HaploDX** for short, provides a collection of functions that can be used to simulate population-specific genomic data. This package is part of the Genetic Simulator Resources (GSR) catalog (click the link below for more information).
 
 <div style="width: 180px; margin: 0 auto;"><a href="https://surveillance.cancer.gov/genetic-simulation-resources/"><img src="https://surveillance.cancer.gov/gsr/static/img/gsr_tile.jpg" alt="Catalogued on GSR" width="180" height="60" /></a></div>
 
 ## Installation
 
+### Manual installation
 ```bash
 $ git clone https://github.com/remytuyeras/HaploDynamics.git
 ```
 Then, create your script where the folder ```HaploDynamics``` is located.
 ```bash
 $ ls
 HaploDynamics
 $ touch myscript.py
 ```
+### Pip
+Coming soon
 
 ## Quick start
 
 The following script generates a VCF file containing simulated diploid genotypes for a population of 1000 individuals with LD-blocks of length 20kb, 5kb, 20kb, 35kb, 30kb and 15kb. 
 ```python
-from HaploDynamics.HaploDX import genmatrix , create_vcfgz
+import HaploDynamics.HaploDX as hdx
 
-simulated_data = genmatrix([20,5,20,35,30,15],strength=1,population=0.1,Npop=1000)
-create_vcfgz("genomic-data.simulation.v1",*simulated_data)
+simulated_data = hdx.genmatrix([20,5,20,35,30,15],strength=1,population=0.1,Npop=1000)
+hdx.create_vcfgz("genomic-data.simulation.v1",*simulated_data)
 ```
 The equation ```strength=1``` forces a high amount of linkage disequilibrium and the equation ```population=0.1``` increases the likelyhood of the simulated population to have rare mutations (e.g. to simulate a population profile close to African and South-Asian populations). 
 
 More generally, the function ```genmatrix()``` takes the following types of parameters:
 Parameters | Type | Values
 | :--- | :--- | :---
 ```blocks```  | ```list[int]``` | List of positive integers, ideally between 1 and 40.
@@ -57,21 +60,21 @@
 The generation of each locus in a VCF file tend to be linear in the parameter ```Npop```. For example, one genetic variant can take from 0.3 to 0.8 seconds to be generated/simulated when we set ```Npop=100000``` (this may vary depending on your machine). The estimated time complexity for an average machine is shown below.
 
 ![GitHub Logo](/time_complexity.png)
 
 The following script shows how to display the linkage disequilibirum correlations associated with the simulated data.
 ```python
 import matplotlib.pyplot as plt
-from HaploDynamics.HaploDX import genmatrix, create_vcfgz, display, LD_corr_matrix
+import HaploDynamics.HaploDX as hdx
 
-simulated_data = genmatrix([20,5,20,35,30,15],strength=1,population=0.1,Npop=1000)
-create_vcfgz("genomic-data.simulation.v1",*simulated_data)
+simulated_data = hdx.genmatrix([20,5,20,35,30,15],strength=1,population=0.1,Npop=1000)
+hdx.create_vcfgz("genomic-data.simulation.v1",*simulated_data)
 
-rel, m, _ = LD_corr_matrix(simulated_data[0])
-plt.imshow(display(rel,m))
+rel, m, _ = hdx.LD_corr_matrix(simulated_data[0])
+plt.imshow(hdx.display(rel,m))
 plt.show()
 ```
 The following plot is an example of the output that can be returned by the previous script when using 6 LD-blocks of 20kb each.
 
 ![alt text](http://www.normalesup.org/~tuyeras/node_diss/blg/blg_stat/img/LD_block_corr_strength_high.png)
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1 Name: HaploDynamics Version: 0.1b2 Summary: A python
+Metadata-Version: 2.1 Name: HaploDynamics Version: 0.1b3 Summary: A python
 library to develop genomic data simulators Home-page: https://github.com/
 remytuyeras/HaploDynamics Download-URL: https://github.com/remytuyeras/
-HaploDynamics/archive/refs/tags/v0.1-beta.2.tar.gz Author: Remy Tuyeras Author-
+HaploDynamics/archive/refs/tags/v0.1-beta.3.tar.gz Author: Remy Tuyeras Author-
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
-## Installation ```bash $ git clone https://github.com/remytuyeras/
-HaploDynamics.git ``` Then, create your script where the folder
+## Installation ### Manual installation ```bash $ git clone https://github.com/
+remytuyeras/HaploDynamics.git ``` Then, create your script where the folder
 ```HaploDynamics``` is located. ```bash $ ls HaploDynamics $ touch myscript.py
-``` ## Quick start The following script generates a VCF file containing
-simulated diploid genotypes for a population of 1000 individuals with LD-blocks
-of length 20kb, 5kb, 20kb, 35kb, 30kb and 15kb. ```python from
-HaploDynamics.HaploDX import genmatrix , create_vcfgz simulated_data =
-genmatrix([20,5,20,35,30,15],strength=1,population=0.1,Npop=1000) create_vcfgz
+``` ### Pip Coming soon ## Quick start The following script generates a VCF
+file containing simulated diploid genotypes for a population of 1000
+individuals with LD-blocks of length 20kb, 5kb, 20kb, 35kb, 30kb and 15kb.
+```python import HaploDynamics.HaploDX as hdx simulated_data = hdx.genmatrix(
+[20,5,20,35,30,15],strength=1,population=0.1,Npop=1000) hdx.create_vcfgz
 ("genomic-data.simulation.v1",*simulated_data) ``` The equation
 ```strength=1``` forces a high amount of linkage disequilibrium and the
 equation ```population=0.1``` increases the likelyhood of the simulated
 population to have rare mutations (e.g. to simulate a population profile close
 to African and South-Asian populations). More generally, the function
 ```genmatrix()``` takes the following types of parameters: Parameters | Type |
 Values | :--- | :--- | :--- ```blocks``` | ```list[int]``` | List of positive
@@ -36,42 +36,41 @@
 | Positive integer specifying the number of individuals in the genomic matrix
 The generation of each locus in a VCF file tend to be linear in the parameter
 ```Npop```. For example, one genetic variant can take from 0.3 to 0.8 seconds
 to be generated/simulated when we set ```Npop=100000``` (this may vary
 depending on your machine). The estimated time complexity for an average
 machine is shown below. ![GitHub Logo](/time_complexity.png) The following
 script shows how to display the linkage disequilibirum correlations associated
-with the simulated data. ```python import matplotlib.pyplot as plt from
-HaploDynamics.HaploDX import genmatrix, create_vcfgz, display, LD_corr_matrix
-simulated_data = genmatrix(
-[20,5,20,35,30,15],strength=1,population=0.1,Npop=1000) create_vcfgz("genomic-
-data.simulation.v1",*simulated_data) rel, m, _ = LD_corr_matrix(simulated_data
-[0]) plt.imshow(display(rel,m)) plt.show() ``` The following plot is an example
-of the output that can be returned by the previous script when using 6 LD-
-blocks of 20kb each. ![alt text](http://www.normalesup.org/~tuyeras/node_diss/
-blg/blg_stat/img/LD_block_corr_strength_high.png) ## HaploDX Functions You can
-find a complete presentation (or in fact a thorough tutorial) of the
-**HaploDX** library on my personal webpage (here). Below is the list of all
-functions accessible from the library. It is recommended to first experiment
-with the functions presented in the [Data Generation](#data-generation)
-section. ### Population and Allele Frequency Spectrum Modeling ```python def
-stochastic_line(a: float,b: float,sigma: float) -> Callable[float,float] ```
-```python population_mut = stochastic_line(0.08,0.17,0.01) ``` ```python def
-afs_distribution(index: int,alpha: float = 4/30) -> float ``` ```python def
-afs_intervals(pick: float,alpha: float = 4/30) -> list[float] ``` ```python def
-afs_sample(alpha: float = 4/30) -> float ``` ```python def genotype_schema
-(alpha: float = 4/30) -> tuple[float,list[float]] ``` ```python def genotype
-(hwp: list[float],minor: int) -> tuple[int,int] ``` ```python gref = lambda g:
-g[0] if g[0] in [2,0] else g[1] ``` ```python def population_mld(t: float) -
-> tuple[float,float,float] ``` ### LD and HardyâWeinberg Principle Modeling
-```python def decay(initial: float,halfwidth: float,shift: float) -> Callable
-[float,float] ``` ```python def ref_alt_function(y: float,x: float) -> float
-``` ```python def alt_alt_function(y: float,z: float,x: float) -> float ```
-```python def amplifier(beta: float,p: float,q: float,s: float = 1) -> float
-``` ```python def lb_freq(beta: float,gamma: float,previous_freq:
+with the simulated data. ```python import matplotlib.pyplot as plt import
+HaploDynamics.HaploDX as hdx simulated_data = hdx.genmatrix(
+[20,5,20,35,30,15],strength=1,population=0.1,Npop=1000) hdx.create_vcfgz
+("genomic-data.simulation.v1",*simulated_data) rel, m, _ = hdx.LD_corr_matrix
+(simulated_data[0]) plt.imshow(hdx.display(rel,m)) plt.show() ``` The following
+plot is an example of the output that can be returned by the previous script
+when using 6 LD-blocks of 20kb each. ![alt text](http://www.normalesup.org/
+~tuyeras/node_diss/blg/blg_stat/img/LD_block_corr_strength_high.png) ## HaploDX
+Functions You can find a complete presentation (or in fact a thorough tutorial)
+of the **HaploDX** library on my personal webpage (here). Below is the list of
+all functions accessible from the library. It is recommended to first
+experiment with the functions presented in the [Data Generation](#data-
+generation) section. ### Population and Allele Frequency Spectrum Modeling
+```python def stochastic_line(a: float,b: float,sigma: float) -> Callable
+[float,float] ``` ```python population_mut = stochastic_line(0.08,0.17,0.01)
+``` ```python def afs_distribution(index: int,alpha: float = 4/30) -> float ```
+```python def afs_intervals(pick: float,alpha: float = 4/30) -> list[float] ```
+```python def afs_sample(alpha: float = 4/30) -> float ``` ```python def
+genotype_schema(alpha: float = 4/30) -> tuple[float,list[float]] ``` ```python
+def genotype(hwp: list[float],minor: int) -> tuple[int,int] ``` ```python gref
+= lambda g: g[0] if g[0] in [2,0] else g[1] ``` ```python def population_mld(t:
+float) -> tuple[float,float,float] ``` ### LD and HardyâWeinberg Principle
+Modeling ```python def decay(initial: float,halfwidth: float,shift: float) -
+> Callable[float,float] ``` ```python def ref_alt_function(y: float,x: float) -
+> float ``` ```python def alt_alt_function(y: float,z: float,x: float) -> float
+``` ```python def amplifier(beta: float,p: float,q: float,s: float = 1) -
+> float ``` ```python def lb_freq(beta: float,gamma: float,previous_freq:
 float,distance: float,shift: float) -> float ``` ```python def ub_freq(beta:
 float,gamma: float,previous_freq: float,distance: float,shift: float) -> float
 ``` ```python def linkage_disequilibrium(alpha: float,beta: float,gamma:
 float,strength: float = -1) -> Callable[float,Callabel[float,tuple
 [float,float]]] ``` ```python def cond_genotype_schema(previous_maf:
 float,distance: float,alpha: float,beta: float,gamma: float,strength: float = -
 1) -> tuple[float,list[float],float] ``` ### Data Generation ```python def
```

### Comparing `HaploDynamics-0.1b2/LICENSE` & `HaploDynamics-0.1b3/LICENSE`

 * *Files identical despite different names*

### Comparing `HaploDynamics-0.1b2/PKG-INFO` & `HaploDynamics-0.1b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: HaploDynamics
-Version: 0.1b2
+Version: 0.1b3
 Summary: A python library to develop genomic data simulators
 Home-page: https://github.com/remytuyeras/HaploDynamics
-Download-URL: https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.2.tar.gz
+Download-URL: https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.3.tar.gz
 Author: Remy Tuyeras
 Author-email: rtuyeras@gmail.com
 License: gpl-3.0
 Keywords: Simulator,Genomics,Genomic,Microarray,SNP chip,VCF,Linkage disequilibrium,Hardy-Weinberg equilibrium
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -21,32 +21,35 @@
 # HaploDynamics
 The python library **HaploDynamics**, or **HaploDX** for short, provides a collection of functions that can be used to simulate population-specific genomic data. This package is part of the Genetic Simulator Resources (GSR) catalog (click the link below for more information).
 
 <div style="width: 180px; margin: 0 auto;"><a href="https://surveillance.cancer.gov/genetic-simulation-resources/"><img src="https://surveillance.cancer.gov/gsr/static/img/gsr_tile.jpg" alt="Catalogued on GSR" width="180" height="60" /></a></div>
 
 ## Installation
 
+### Manual installation
 ```bash
 $ git clone https://github.com/remytuyeras/HaploDynamics.git
 ```
 Then, create your script where the folder ```HaploDynamics``` is located.
 ```bash
 $ ls
 HaploDynamics
 $ touch myscript.py
 ```
+### Pip
+Coming soon
 
 ## Quick start
 
 The following script generates a VCF file containing simulated diploid genotypes for a population of 1000 individuals with LD-blocks of length 20kb, 5kb, 20kb, 35kb, 30kb and 15kb. 
 ```python
-from HaploDynamics.HaploDX import genmatrix , create_vcfgz
+import HaploDynamics.HaploDX as hdx
 
-simulated_data = genmatrix([20,5,20,35,30,15],strength=1,population=0.1,Npop=1000)
-create_vcfgz("genomic-data.simulation.v1",*simulated_data)
+simulated_data = hdx.genmatrix([20,5,20,35,30,15],strength=1,population=0.1,Npop=1000)
+hdx.create_vcfgz("genomic-data.simulation.v1",*simulated_data)
 ```
 The equation ```strength=1``` forces a high amount of linkage disequilibrium and the equation ```population=0.1``` increases the likelyhood of the simulated population to have rare mutations (e.g. to simulate a population profile close to African and South-Asian populations). 
 
 More generally, the function ```genmatrix()``` takes the following types of parameters:
 Parameters | Type | Values
 | :--- | :--- | :---
 ```blocks```  | ```list[int]``` | List of positive integers, ideally between 1 and 40.
@@ -57,21 +60,21 @@
 The generation of each locus in a VCF file tend to be linear in the parameter ```Npop```. For example, one genetic variant can take from 0.3 to 0.8 seconds to be generated/simulated when we set ```Npop=100000``` (this may vary depending on your machine). The estimated time complexity for an average machine is shown below.
 
 ![GitHub Logo](/time_complexity.png)
 
 The following script shows how to display the linkage disequilibirum correlations associated with the simulated data.
 ```python
 import matplotlib.pyplot as plt
-from HaploDynamics.HaploDX import genmatrix, create_vcfgz, display, LD_corr_matrix
+import HaploDynamics.HaploDX as hdx
 
-simulated_data = genmatrix([20,5,20,35,30,15],strength=1,population=0.1,Npop=1000)
-create_vcfgz("genomic-data.simulation.v1",*simulated_data)
+simulated_data = hdx.genmatrix([20,5,20,35,30,15],strength=1,population=0.1,Npop=1000)
+hdx.create_vcfgz("genomic-data.simulation.v1",*simulated_data)
 
-rel, m, _ = LD_corr_matrix(simulated_data[0])
-plt.imshow(display(rel,m))
+rel, m, _ = hdx.LD_corr_matrix(simulated_data[0])
+plt.imshow(hdx.display(rel,m))
 plt.show()
 ```
 The following plot is an example of the output that can be returned by the previous script when using 6 LD-blocks of 20kb each.
 
 ![alt text](http://www.normalesup.org/~tuyeras/node_diss/blg/blg_stat/img/LD_block_corr_strength_high.png)
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1 Name: HaploDynamics Version: 0.1b2 Summary: A python
+Metadata-Version: 2.1 Name: HaploDynamics Version: 0.1b3 Summary: A python
 library to develop genomic data simulators Home-page: https://github.com/
 remytuyeras/HaploDynamics Download-URL: https://github.com/remytuyeras/
-HaploDynamics/archive/refs/tags/v0.1-beta.2.tar.gz Author: Remy Tuyeras Author-
+HaploDynamics/archive/refs/tags/v0.1-beta.3.tar.gz Author: Remy Tuyeras Author-
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
-## Installation ```bash $ git clone https://github.com/remytuyeras/
-HaploDynamics.git ``` Then, create your script where the folder
+## Installation ### Manual installation ```bash $ git clone https://github.com/
+remytuyeras/HaploDynamics.git ``` Then, create your script where the folder
 ```HaploDynamics``` is located. ```bash $ ls HaploDynamics $ touch myscript.py
-``` ## Quick start The following script generates a VCF file containing
-simulated diploid genotypes for a population of 1000 individuals with LD-blocks
-of length 20kb, 5kb, 20kb, 35kb, 30kb and 15kb. ```python from
-HaploDynamics.HaploDX import genmatrix , create_vcfgz simulated_data =
-genmatrix([20,5,20,35,30,15],strength=1,population=0.1,Npop=1000) create_vcfgz
+``` ### Pip Coming soon ## Quick start The following script generates a VCF
+file containing simulated diploid genotypes for a population of 1000
+individuals with LD-blocks of length 20kb, 5kb, 20kb, 35kb, 30kb and 15kb.
+```python import HaploDynamics.HaploDX as hdx simulated_data = hdx.genmatrix(
+[20,5,20,35,30,15],strength=1,population=0.1,Npop=1000) hdx.create_vcfgz
 ("genomic-data.simulation.v1",*simulated_data) ``` The equation
 ```strength=1``` forces a high amount of linkage disequilibrium and the
 equation ```population=0.1``` increases the likelyhood of the simulated
 population to have rare mutations (e.g. to simulate a population profile close
 to African and South-Asian populations). More generally, the function
 ```genmatrix()``` takes the following types of parameters: Parameters | Type |
 Values | :--- | :--- | :--- ```blocks``` | ```list[int]``` | List of positive
@@ -36,42 +36,41 @@
 | Positive integer specifying the number of individuals in the genomic matrix
 The generation of each locus in a VCF file tend to be linear in the parameter
 ```Npop```. For example, one genetic variant can take from 0.3 to 0.8 seconds
 to be generated/simulated when we set ```Npop=100000``` (this may vary
 depending on your machine). The estimated time complexity for an average
 machine is shown below. ![GitHub Logo](/time_complexity.png) The following
 script shows how to display the linkage disequilibirum correlations associated
-with the simulated data. ```python import matplotlib.pyplot as plt from
-HaploDynamics.HaploDX import genmatrix, create_vcfgz, display, LD_corr_matrix
-simulated_data = genmatrix(
-[20,5,20,35,30,15],strength=1,population=0.1,Npop=1000) create_vcfgz("genomic-
-data.simulation.v1",*simulated_data) rel, m, _ = LD_corr_matrix(simulated_data
-[0]) plt.imshow(display(rel,m)) plt.show() ``` The following plot is an example
-of the output that can be returned by the previous script when using 6 LD-
-blocks of 20kb each. ![alt text](http://www.normalesup.org/~tuyeras/node_diss/
-blg/blg_stat/img/LD_block_corr_strength_high.png) ## HaploDX Functions You can
-find a complete presentation (or in fact a thorough tutorial) of the
-**HaploDX** library on my personal webpage (here). Below is the list of all
-functions accessible from the library. It is recommended to first experiment
-with the functions presented in the [Data Generation](#data-generation)
-section. ### Population and Allele Frequency Spectrum Modeling ```python def
-stochastic_line(a: float,b: float,sigma: float) -> Callable[float,float] ```
-```python population_mut = stochastic_line(0.08,0.17,0.01) ``` ```python def
-afs_distribution(index: int,alpha: float = 4/30) -> float ``` ```python def
-afs_intervals(pick: float,alpha: float = 4/30) -> list[float] ``` ```python def
-afs_sample(alpha: float = 4/30) -> float ``` ```python def genotype_schema
-(alpha: float = 4/30) -> tuple[float,list[float]] ``` ```python def genotype
-(hwp: list[float],minor: int) -> tuple[int,int] ``` ```python gref = lambda g:
-g[0] if g[0] in [2,0] else g[1] ``` ```python def population_mld(t: float) -
-> tuple[float,float,float] ``` ### LD and HardyâWeinberg Principle Modeling
-```python def decay(initial: float,halfwidth: float,shift: float) -> Callable
-[float,float] ``` ```python def ref_alt_function(y: float,x: float) -> float
-``` ```python def alt_alt_function(y: float,z: float,x: float) -> float ```
-```python def amplifier(beta: float,p: float,q: float,s: float = 1) -> float
-``` ```python def lb_freq(beta: float,gamma: float,previous_freq:
+with the simulated data. ```python import matplotlib.pyplot as plt import
+HaploDynamics.HaploDX as hdx simulated_data = hdx.genmatrix(
+[20,5,20,35,30,15],strength=1,population=0.1,Npop=1000) hdx.create_vcfgz
+("genomic-data.simulation.v1",*simulated_data) rel, m, _ = hdx.LD_corr_matrix
+(simulated_data[0]) plt.imshow(hdx.display(rel,m)) plt.show() ``` The following
+plot is an example of the output that can be returned by the previous script
+when using 6 LD-blocks of 20kb each. ![alt text](http://www.normalesup.org/
+~tuyeras/node_diss/blg/blg_stat/img/LD_block_corr_strength_high.png) ## HaploDX
+Functions You can find a complete presentation (or in fact a thorough tutorial)
+of the **HaploDX** library on my personal webpage (here). Below is the list of
+all functions accessible from the library. It is recommended to first
+experiment with the functions presented in the [Data Generation](#data-
+generation) section. ### Population and Allele Frequency Spectrum Modeling
+```python def stochastic_line(a: float,b: float,sigma: float) -> Callable
+[float,float] ``` ```python population_mut = stochastic_line(0.08,0.17,0.01)
+``` ```python def afs_distribution(index: int,alpha: float = 4/30) -> float ```
+```python def afs_intervals(pick: float,alpha: float = 4/30) -> list[float] ```
+```python def afs_sample(alpha: float = 4/30) -> float ``` ```python def
+genotype_schema(alpha: float = 4/30) -> tuple[float,list[float]] ``` ```python
+def genotype(hwp: list[float],minor: int) -> tuple[int,int] ``` ```python gref
+= lambda g: g[0] if g[0] in [2,0] else g[1] ``` ```python def population_mld(t:
+float) -> tuple[float,float,float] ``` ### LD and HardyâWeinberg Principle
+Modeling ```python def decay(initial: float,halfwidth: float,shift: float) -
+> Callable[float,float] ``` ```python def ref_alt_function(y: float,x: float) -
+> float ``` ```python def alt_alt_function(y: float,z: float,x: float) -> float
+``` ```python def amplifier(beta: float,p: float,q: float,s: float = 1) -
+> float ``` ```python def lb_freq(beta: float,gamma: float,previous_freq:
 float,distance: float,shift: float) -> float ``` ```python def ub_freq(beta:
 float,gamma: float,previous_freq: float,distance: float,shift: float) -> float
 ``` ```python def linkage_disequilibrium(alpha: float,beta: float,gamma:
 float,strength: float = -1) -> Callable[float,Callabel[float,tuple
 [float,float]]] ``` ```python def cond_genotype_schema(previous_maf:
 float,distance: float,alpha: float,beta: float,gamma: float,strength: float = -
 1) -> tuple[float,list[float],float] ``` ### Data Generation ```python def
```

### Comparing `HaploDynamics-0.1b2/README.md` & `HaploDynamics-0.1b3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # HaploDynamics
 The python library **HaploDynamics**, or **HaploDX** for short, provides a collection of functions that can be used to simulate population-specific genomic data. This package is part of the Genetic Simulator Resources (GSR) catalog (click the link below for more information).
 
 <div style="width: 180px; margin: 0 auto;"><a href="https://surveillance.cancer.gov/genetic-simulation-resources/"><img src="https://surveillance.cancer.gov/gsr/static/img/gsr_tile.jpg" alt="Catalogued on GSR" width="180" height="60" /></a></div>
 
 ## Installation
 
+### Manual installation
 ```bash
 $ git clone https://github.com/remytuyeras/HaploDynamics.git
 ```
 Then, create your script where the folder ```HaploDynamics``` is located.
 ```bash
 $ ls
 HaploDynamics
 $ touch myscript.py
 ```
+### Pip
+Coming soon
 
 ## Quick start
 
 The following script generates a VCF file containing simulated diploid genotypes for a population of 1000 individuals with LD-blocks of length 20kb, 5kb, 20kb, 35kb, 30kb and 15kb. 
 ```python
-from HaploDynamics.HaploDX import genmatrix , create_vcfgz
+import HaploDynamics.HaploDX as hdx
 
-simulated_data = genmatrix([20,5,20,35,30,15],strength=1,population=0.1,Npop=1000)
-create_vcfgz("genomic-data.simulation.v1",*simulated_data)
+simulated_data = hdx.genmatrix([20,5,20,35,30,15],strength=1,population=0.1,Npop=1000)
+hdx.create_vcfgz("genomic-data.simulation.v1",*simulated_data)
 ```
 The equation ```strength=1``` forces a high amount of linkage disequilibrium and the equation ```population=0.1``` increases the likelyhood of the simulated population to have rare mutations (e.g. to simulate a population profile close to African and South-Asian populations). 
 
 More generally, the function ```genmatrix()``` takes the following types of parameters:
 Parameters | Type | Values
 | :--- | :--- | :---
 ```blocks```  | ```list[int]``` | List of positive integers, ideally between 1 and 40.
@@ -37,21 +40,21 @@
 The generation of each locus in a VCF file tend to be linear in the parameter ```Npop```. For example, one genetic variant can take from 0.3 to 0.8 seconds to be generated/simulated when we set ```Npop=100000``` (this may vary depending on your machine). The estimated time complexity for an average machine is shown below.
 
 ![GitHub Logo](/time_complexity.png)
 
 The following script shows how to display the linkage disequilibirum correlations associated with the simulated data.
 ```python
 import matplotlib.pyplot as plt
-from HaploDynamics.HaploDX import genmatrix, create_vcfgz, display, LD_corr_matrix
+import HaploDynamics.HaploDX as hdx
 
-simulated_data = genmatrix([20,5,20,35,30,15],strength=1,population=0.1,Npop=1000)
-create_vcfgz("genomic-data.simulation.v1",*simulated_data)
+simulated_data = hdx.genmatrix([20,5,20,35,30,15],strength=1,population=0.1,Npop=1000)
+hdx.create_vcfgz("genomic-data.simulation.v1",*simulated_data)
 
-rel, m, _ = LD_corr_matrix(simulated_data[0])
-plt.imshow(display(rel,m))
+rel, m, _ = hdx.LD_corr_matrix(simulated_data[0])
+plt.imshow(hdx.display(rel,m))
 plt.show()
 ```
 The following plot is an example of the output that can be returned by the previous script when using 6 LD-blocks of 20kb each.
 
 ![alt text](http://www.normalesup.org/~tuyeras/node_diss/blg/blg_stat/img/LD_block_corr_strength_high.png)
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
 # HaploDynamics The python library **HaploDynamics**, or **HaploDX** for short,
 provides a collection of functions that can be used to simulate population-
 specific genomic data. This package is part of the Genetic Simulator Resources
 (GSR) catalog (click the link below for more information).
 [Catalogued_on_GSR]
-## Installation ```bash $ git clone https://github.com/remytuyeras/
-HaploDynamics.git ``` Then, create your script where the folder
+## Installation ### Manual installation ```bash $ git clone https://github.com/
+remytuyeras/HaploDynamics.git ``` Then, create your script where the folder
 ```HaploDynamics``` is located. ```bash $ ls HaploDynamics $ touch myscript.py
-``` ## Quick start The following script generates a VCF file containing
-simulated diploid genotypes for a population of 1000 individuals with LD-blocks
-of length 20kb, 5kb, 20kb, 35kb, 30kb and 15kb. ```python from
-HaploDynamics.HaploDX import genmatrix , create_vcfgz simulated_data =
-genmatrix([20,5,20,35,30,15],strength=1,population=0.1,Npop=1000) create_vcfgz
+``` ### Pip Coming soon ## Quick start The following script generates a VCF
+file containing simulated diploid genotypes for a population of 1000
+individuals with LD-blocks of length 20kb, 5kb, 20kb, 35kb, 30kb and 15kb.
+```python import HaploDynamics.HaploDX as hdx simulated_data = hdx.genmatrix(
+[20,5,20,35,30,15],strength=1,population=0.1,Npop=1000) hdx.create_vcfgz
 ("genomic-data.simulation.v1",*simulated_data) ``` The equation
 ```strength=1``` forces a high amount of linkage disequilibrium and the
 equation ```population=0.1``` increases the likelyhood of the simulated
 population to have rare mutations (e.g. to simulate a population profile close
 to African and South-Asian populations). More generally, the function
 ```genmatrix()``` takes the following types of parameters: Parameters | Type |
 Values | :--- | :--- | :--- ```blocks``` | ```list[int]``` | List of positive
@@ -24,42 +24,41 @@
 | Positive integer specifying the number of individuals in the genomic matrix
 The generation of each locus in a VCF file tend to be linear in the parameter
 ```Npop```. For example, one genetic variant can take from 0.3 to 0.8 seconds
 to be generated/simulated when we set ```Npop=100000``` (this may vary
 depending on your machine). The estimated time complexity for an average
 machine is shown below. ![GitHub Logo](/time_complexity.png) The following
 script shows how to display the linkage disequilibirum correlations associated
-with the simulated data. ```python import matplotlib.pyplot as plt from
-HaploDynamics.HaploDX import genmatrix, create_vcfgz, display, LD_corr_matrix
-simulated_data = genmatrix(
-[20,5,20,35,30,15],strength=1,population=0.1,Npop=1000) create_vcfgz("genomic-
-data.simulation.v1",*simulated_data) rel, m, _ = LD_corr_matrix(simulated_data
-[0]) plt.imshow(display(rel,m)) plt.show() ``` The following plot is an example
-of the output that can be returned by the previous script when using 6 LD-
-blocks of 20kb each. ![alt text](http://www.normalesup.org/~tuyeras/node_diss/
-blg/blg_stat/img/LD_block_corr_strength_high.png) ## HaploDX Functions You can
-find a complete presentation (or in fact a thorough tutorial) of the
-**HaploDX** library on my personal webpage (here). Below is the list of all
-functions accessible from the library. It is recommended to first experiment
-with the functions presented in the [Data Generation](#data-generation)
-section. ### Population and Allele Frequency Spectrum Modeling ```python def
-stochastic_line(a: float,b: float,sigma: float) -> Callable[float,float] ```
-```python population_mut = stochastic_line(0.08,0.17,0.01) ``` ```python def
-afs_distribution(index: int,alpha: float = 4/30) -> float ``` ```python def
-afs_intervals(pick: float,alpha: float = 4/30) -> list[float] ``` ```python def
-afs_sample(alpha: float = 4/30) -> float ``` ```python def genotype_schema
-(alpha: float = 4/30) -> tuple[float,list[float]] ``` ```python def genotype
-(hwp: list[float],minor: int) -> tuple[int,int] ``` ```python gref = lambda g:
-g[0] if g[0] in [2,0] else g[1] ``` ```python def population_mld(t: float) -
-> tuple[float,float,float] ``` ### LD and HardyâWeinberg Principle Modeling
-```python def decay(initial: float,halfwidth: float,shift: float) -> Callable
-[float,float] ``` ```python def ref_alt_function(y: float,x: float) -> float
-``` ```python def alt_alt_function(y: float,z: float,x: float) -> float ```
-```python def amplifier(beta: float,p: float,q: float,s: float = 1) -> float
-``` ```python def lb_freq(beta: float,gamma: float,previous_freq:
+with the simulated data. ```python import matplotlib.pyplot as plt import
+HaploDynamics.HaploDX as hdx simulated_data = hdx.genmatrix(
+[20,5,20,35,30,15],strength=1,population=0.1,Npop=1000) hdx.create_vcfgz
+("genomic-data.simulation.v1",*simulated_data) rel, m, _ = hdx.LD_corr_matrix
+(simulated_data[0]) plt.imshow(hdx.display(rel,m)) plt.show() ``` The following
+plot is an example of the output that can be returned by the previous script
+when using 6 LD-blocks of 20kb each. ![alt text](http://www.normalesup.org/
+~tuyeras/node_diss/blg/blg_stat/img/LD_block_corr_strength_high.png) ## HaploDX
+Functions You can find a complete presentation (or in fact a thorough tutorial)
+of the **HaploDX** library on my personal webpage (here). Below is the list of
+all functions accessible from the library. It is recommended to first
+experiment with the functions presented in the [Data Generation](#data-
+generation) section. ### Population and Allele Frequency Spectrum Modeling
+```python def stochastic_line(a: float,b: float,sigma: float) -> Callable
+[float,float] ``` ```python population_mut = stochastic_line(0.08,0.17,0.01)
+``` ```python def afs_distribution(index: int,alpha: float = 4/30) -> float ```
+```python def afs_intervals(pick: float,alpha: float = 4/30) -> list[float] ```
+```python def afs_sample(alpha: float = 4/30) -> float ``` ```python def
+genotype_schema(alpha: float = 4/30) -> tuple[float,list[float]] ``` ```python
+def genotype(hwp: list[float],minor: int) -> tuple[int,int] ``` ```python gref
+= lambda g: g[0] if g[0] in [2,0] else g[1] ``` ```python def population_mld(t:
+float) -> tuple[float,float,float] ``` ### LD and HardyâWeinberg Principle
+Modeling ```python def decay(initial: float,halfwidth: float,shift: float) -
+> Callable[float,float] ``` ```python def ref_alt_function(y: float,x: float) -
+> float ``` ```python def alt_alt_function(y: float,z: float,x: float) -> float
+``` ```python def amplifier(beta: float,p: float,q: float,s: float = 1) -
+> float ``` ```python def lb_freq(beta: float,gamma: float,previous_freq:
 float,distance: float,shift: float) -> float ``` ```python def ub_freq(beta:
 float,gamma: float,previous_freq: float,distance: float,shift: float) -> float
 ``` ```python def linkage_disequilibrium(alpha: float,beta: float,gamma:
 float,strength: float = -1) -> Callable[float,Callabel[float,tuple
 [float,float]]] ``` ```python def cond_genotype_schema(previous_maf:
 float,distance: float,alpha: float,beta: float,gamma: float,strength: float = -
 1) -> tuple[float,list[float],float] ``` ### Data Generation ```python def
```

### Comparing `HaploDynamics-0.1b2/setup.py` & `HaploDynamics-0.1b3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
   name = 'HaploDynamics',
   packages=setuptools.find_packages(include=['HaploDX','Framework']),
-  version = 'v0.1-beta.2',
+  version = 'v0.1-beta.3',
   license='gpl-3.0',
   author = 'Remy Tuyeras',
   author_email = 'rtuyeras@gmail.com',
   description = 'A python library to develop genomic data simulators',
   long_description = long_description,
   long_description_content_type = "text/markdown",
   url = 'https://github.com/remytuyeras/HaploDynamics',
-  download_url = 'https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.2.tar.gz',
+  download_url = 'https://github.com/remytuyeras/HaploDynamics/archive/refs/tags/v0.1-beta.3.tar.gz',
   keywords = ['Simulator', 'Genomics', 'Genomic', 'Microarray','SNP chip','VCF', 'Linkage disequilibrium', 'Hardy-Weinberg equilibrium'],
   install_requires=['scipy'],
   classifiers=[
     'Development Status :: 4 - Beta',  #"3 - Alpha", "4 - Beta" or "5 - Production/Stable"
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'Topic :: Software Development :: Build Tools',
```

