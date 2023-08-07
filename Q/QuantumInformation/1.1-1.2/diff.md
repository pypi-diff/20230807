# Comparing `tmp/QuantumInformation-1.1.tar.gz` & `tmp/QuantumInformation-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuantumInformation-1.1.tar", last modified: Sat Jan 15 07:24:53 2022, max compression
+gzip compressed data, was "QuantumInformation-1.2.tar", last modified: Mon Aug  7 14:37:12 2023, max compression
```

## Comparing `QuantumInformation-1.1.tar` & `QuantumInformation-1.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxr-x   0 pranay    (1000) pranay    (1000)        0 2022-01-15 07:24:53.254772 QuantumInformation-1.1/
--rw-rw-r--   0 pranay    (1000) pranay    (1000)     2505 2022-01-15 07:24:53.254772 QuantumInformation-1.1/PKG-INFO
-drwxrwxr-x   0 pranay    (1000) pranay    (1000)        0 2022-01-15 07:24:53.254772 QuantumInformation-1.1/QuantumInformation/
--rw-r--r--   0 pranay    (1000) pranay    (1000)     7169 2020-11-03 06:29:30.000000 QuantumInformation-1.1/QuantumInformation/RecurNum.py
--rw-r--r--   0 pranay    (1000) pranay    (1000)      343 2021-03-23 08:34:42.000000 QuantumInformation-1.1/QuantumInformation/__init__.py
--rw-r--r--   0 pranay    (1000) pranay    (1000)     7698 2021-12-27 09:17:26.000000 QuantumInformation-1.1/QuantumInformation/chap2_nutsboltsquantum.py
--rw-r--r--   0 pranay    (1000) pranay    (1000)    19128 2022-01-11 14:34:15.000000 QuantumInformation-1.1/QuantumInformation/chap3_linearalgebra.py
--rw-r--r--   0 pranay    (1000) pranay    (1000)    18397 2021-12-30 08:10:52.000000 QuantumInformation-1.1/QuantumInformation/chap4_quantumtools.py
--rw-r--r--   0 pranay    (1000) pranay    (1000)    26358 2022-01-09 06:28:57.000000 QuantumInformation-1.1/QuantumInformation/chap5_partial_quantumentanglement.py
--rw-r--r--   0 pranay    (1000) pranay    (1000)    26354 2021-12-28 10:34:17.000000 QuantumInformation-1.1/QuantumInformation/chap6_hamiltonians.py
--rw-r--r--   0 pranay    (1000) pranay    (1000)    11522 2021-12-30 09:56:43.000000 QuantumInformation-1.1/QuantumInformation/chap7_randommatrix.py
-drwxrwxr-x   0 pranay    (1000) pranay    (1000)        0 2022-01-15 07:24:53.254772 QuantumInformation-1.1/QuantumInformation.egg-info/
--rw-rw-r--   0 pranay    (1000) pranay    (1000)     2505 2022-01-15 07:24:53.000000 QuantumInformation-1.1/QuantumInformation.egg-info/PKG-INFO
--rw-rw-r--   0 pranay    (1000) pranay    (1000)      545 2022-01-15 07:24:53.000000 QuantumInformation-1.1/QuantumInformation.egg-info/SOURCES.txt
--rw-rw-r--   0 pranay    (1000) pranay    (1000)        1 2022-01-15 07:24:53.000000 QuantumInformation-1.1/QuantumInformation.egg-info/dependency_links.txt
--rw-rw-r--   0 pranay    (1000) pranay    (1000)        1 2022-01-15 07:24:53.000000 QuantumInformation-1.1/QuantumInformation.egg-info/not-zip-safe
--rw-rw-r--   0 pranay    (1000) pranay    (1000)       19 2022-01-15 07:24:53.000000 QuantumInformation-1.1/QuantumInformation.egg-info/top_level.txt
--rw-rw-r--   0 pranay    (1000) pranay    (1000)       38 2022-01-15 07:24:53.254772 QuantumInformation-1.1/setup.cfg
--rw-rw-r--   0 pranay    (1000) pranay    (1000)      543 2022-01-15 07:22:31.000000 QuantumInformation-1.1/setup.py
+drwxrwxr-x   0 pranay-ubuntu  (1000) pranay-ubuntu  (1000)        0 2023-08-07 14:37:12.713844 QuantumInformation-1.2/
+-rw-rw-r--   0 pranay-ubuntu  (1000) pranay-ubuntu  (1000)     2721 2023-08-07 14:37:12.713844 QuantumInformation-1.2/PKG-INFO
+drwxrwxr-x   0 pranay-ubuntu  (1000) pranay-ubuntu  (1000)        0 2023-08-07 14:37:12.713844 QuantumInformation-1.2/QuantumInformation/
+-rw-rw-r--   0 pranay-ubuntu  (1000) pranay-ubuntu  (1000)     6887 2022-06-16 16:06:49.000000 QuantumInformation-1.2/QuantumInformation/RecurNum.py
+-rw-rw-r--   0 pranay-ubuntu  (1000) pranay-ubuntu  (1000)      343 2022-06-16 16:06:49.000000 QuantumInformation-1.2/QuantumInformation/__init__.py
+-rw-rw-r--   0 pranay-ubuntu  (1000) pranay-ubuntu  (1000)     7729 2022-06-16 16:06:49.000000 QuantumInformation-1.2/QuantumInformation/chap2_nutsboltsquantum.py
+-rw-rw-r--   0 pranay-ubuntu  (1000) pranay-ubuntu  (1000)    19158 2022-06-16 16:06:49.000000 QuantumInformation-1.2/QuantumInformation/chap3_linearalgebra.py
+-rw-rw-r--   0 pranay-ubuntu  (1000) pranay-ubuntu  (1000)    18428 2022-06-16 16:06:49.000000 QuantumInformation-1.2/QuantumInformation/chap4_quantumtools.py
+-rw-rw-r--   0 pranay-ubuntu  (1000) pranay-ubuntu  (1000)    26387 2022-06-16 16:06:49.000000 QuantumInformation-1.2/QuantumInformation/chap5_partial_quantumentanglement.py
+-rw-rw-r--   0 pranay-ubuntu  (1000) pranay-ubuntu  (1000)    26382 2022-06-16 16:06:49.000000 QuantumInformation-1.2/QuantumInformation/chap6_hamiltonians.py
+-rw-rw-r--   0 pranay-ubuntu  (1000) pranay-ubuntu  (1000)    11552 2022-06-16 16:06:49.000000 QuantumInformation-1.2/QuantumInformation/chap7_randommatrix.py
+drwxrwxr-x   0 pranay-ubuntu  (1000) pranay-ubuntu  (1000)        0 2023-08-07 14:37:12.713844 QuantumInformation-1.2/QuantumInformation.egg-info/
+-rw-rw-r--   0 pranay-ubuntu  (1000) pranay-ubuntu  (1000)     2721 2023-08-07 14:37:12.000000 QuantumInformation-1.2/QuantumInformation.egg-info/PKG-INFO
+-rw-rw-r--   0 pranay-ubuntu  (1000) pranay-ubuntu  (1000)      596 2023-08-07 14:37:12.000000 QuantumInformation-1.2/QuantumInformation.egg-info/SOURCES.txt
+-rw-rw-r--   0 pranay-ubuntu  (1000) pranay-ubuntu  (1000)        1 2023-08-07 14:37:12.000000 QuantumInformation-1.2/QuantumInformation.egg-info/dependency_links.txt
+-rw-rw-r--   0 pranay-ubuntu  (1000) pranay-ubuntu  (1000)        1 2023-08-07 14:05:38.000000 QuantumInformation-1.2/QuantumInformation.egg-info/not-zip-safe
+-rw-rw-r--   0 pranay-ubuntu  (1000) pranay-ubuntu  (1000)       60 2023-08-07 14:37:12.000000 QuantumInformation-1.2/QuantumInformation.egg-info/requires.txt
+-rw-rw-r--   0 pranay-ubuntu  (1000) pranay-ubuntu  (1000)       19 2023-08-07 14:37:12.000000 QuantumInformation-1.2/QuantumInformation.egg-info/top_level.txt
+-rw-rw-r--   0 pranay-ubuntu  (1000) pranay-ubuntu  (1000)     2475 2022-06-16 16:06:49.000000 QuantumInformation-1.2/README.md
+-rw-rw-r--   0 pranay-ubuntu  (1000) pranay-ubuntu  (1000)       38 2023-08-07 14:37:12.713844 QuantumInformation-1.2/setup.cfg
+-rw-rw-r--   0 pranay-ubuntu  (1000) pranay-ubuntu  (1000)      693 2023-08-07 14:36:47.000000 QuantumInformation-1.2/setup.py
```

### Comparing `QuantumInformation-1.1/PKG-INFO` & `QuantumInformation-1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 Metadata-Version: 2.1
 Name: QuantumInformation
-Version: 1.1
+Version: 1.2
 Summary: Quantum Information and Computation package
-Home-page: UNKNOWN
 Author: M. S. Ramkarthik and Pranay Barkataki
-License: UNKNOWN
-Platform: UNKNOWN
+Requires-Python: >= 3.7.9
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 
 # QuantumInformation package
-This package contains numerous numerical methods for various quantum information and computation problems. The explanation of each of the numerical methods are explained in detail in the following book, ***"An Object Oriented Python Cookbook for Quantum Information Theory and Quantum Computing"***. The book contains more than 100 numerical routines in python and it will be extremely useful for a practising physicist, both theoretical and experimentl, working in the areas of quantum information theory, quantum computing, quantum entanglement and also on condensed matter quantum many-body spin half chains. We also remark here that, there is a chapter devoted to numerical linear algebra procedures and a final chapter on random states and matrices too. We can safely and humbly say that, the computational libraries cover a wide spectrum of topics. The hyperlink to buy the book will soon be updated, stay tuned.
+This package contains numerous numerical methods for various quantum information and computation problems. The explanation of each of the numerical methods are explained in detail in the following book, ***"An Object Oriented Python Cookbook for Quantum Information Theory and Quantum Computing"***. The book contains more than 100 numerical routines in python and it will be extremely useful for a practising physicist, both theoretical and experimentl, working in the areas of quantum information theory, quantum computing, quantum entanglement and also on condensed matter quantum many-body spin half chains. We also remark here that, there is a chapter devoted to numerical linear algebra procedures and a final chapter on random states and matrices too. We can safely and humbly say that, the computational libraries cover a wide spectrum of topics. You can easily buy the book by clicking [here](https://www.routledge.com/An-Object-Oriented-Python-Cookbook-in-Quantum-Information-Theory-and-Quantum/Ramkarthik-Barkataki/p/book/9781032256078)
+
+![alt text](https://github.com/pranay1990/QuantumInformation/blob/main/python%20book%20image.jpg)
 
 ## Files
 
 The functionality of each module is extensively discussed in the book.
 
 ## Installation
 Type the following command in the terminal of Linux or the command prompt of Windows, in order to install the package in your local computer.
 
 **pip install QuantumInformation**
 
 ## License
-Copyright 2021 CRC Press
+Copyright 2023 CRC Press
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, distribute, sublicense, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 ***THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.***
-
-
-
-
```

### Comparing `QuantumInformation-1.1/QuantumInformation/RecurNum.py` & `QuantumInformation-1.2/QuantumInformation/RecurNum.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Created on Mon Jul 15 18:26:57 2019
 
-@author: Pranay Barkataki and Payal Dineshbhai Solanki
+@authors: Dr. M. S. Ramkarthik and Dr. Pranay Barkataki
 """
 
 def recur_comb_add(mylist,vec,icount,sum2):
     lenvec=len(vec)
     if icount<=lenvec-1:
         for j in range(icount,lenvec):
             sum3=sum2+vec[j]
@@ -13,19 +13,15 @@
             mylist.append(sum3)
             recur_comb_add(mylist,vec,j+1,sum3)
             if j==lenvec:
                 return()
     if icount==lenvec:
         return()
 
-"""
-Created on Sun Aug  4 21:11:55 2019
 
-@authors: Pranay Barkataki
-"""
 def RecurChainRL1(row,tot_spins,icount,mylist,shift):
     len_row=len(row)
     if icount<len_row:
         for x in range(icount,len_row):
             row2=row.copy()
             if x>=0:
                 row2[x]=1
@@ -58,19 +54,15 @@
             if x<len_row-1 and x!=-1:    
                 RecurChainRL1(row2,tot_spins,x+1,mylist,shift)
             if x==len_row-1:
                 return()
     if icount >= len_row:
         return()
 
-"""
-Created on Sun Aug  7 14:19:31 2019
 
-@authors: Pranay Barkataki
-"""
 def RecurChainRL2(row,tot_spins,icount,mylist,shift):
     len_row=len(row)
     if icount<len_row:
         for x in range(icount,len_row):
             row2=row.copy()
             if x>=0:
                 row2[x]=1
@@ -116,19 +108,15 @@
             if x<len_row-1 and x!=-1:    
                 RecurChainRL2(row2,tot_spins,x+1,mylist,shift)
             if x==len_row-1:
                 return()
     if icount >= len_row:
         return()
         
-"""
-Created on Sun Aug  7 23:09:23 2019
 
-@authors: Pranay Barkataki
-"""
 def RecurChainRL3(row,tot_spins,icount,mylist,shift):
     len_row=len(row)
     if icount<len_row:
         for x in range(icount,len_row):
             row2=row.copy()
             if x>=0:
                 row2[x]=1
@@ -161,19 +149,15 @@
             if x<len_row-1 and x!=-1:    
                 RecurChainRL3(row2,tot_spins,x+1,mylist,shift)
             if x==len_row-1:
                 return()
     if icount >= len_row:
         return()
 
-"""
-Created on Sun Aug  7 14:19:31 2019
 
-@authors: Pranay Barkataki
-"""
 def RecurChainRL4(row,tot_spins,icount,mylist,shift):
     len_row=len(row)
     if icount<len_row:
         for x in range(icount,len_row):
             row2=row.copy()
             if x>=0:
                 row2[x]=1
@@ -217,8 +201,8 @@
                     mylist.append(-sumr)
                     #print(sumr)
             if x<len_row-1 and x!=-1:    
                 RecurChainRL4(row2,tot_spins,x+1,mylist,shift)
             if x==len_row-1:
                 return()
     if icount >= len_row:
-        return()
+        return()
```

### Comparing `QuantumInformation-1.1/QuantumInformation/chap2_nutsboltsquantum.py` & `QuantumInformation-1.2/QuantumInformation/chap2_nutsboltsquantum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Sat Jan 23 2021
 
-@author: pranay barkataki
+@authors: Dr. M. S. Ramkarthik and Dr. Pranay Barkataki
 """
 
 import numpy as np
 import math
 
 class QuantumMechanics:
     
@@ -240,8 +240,8 @@
 
 
 
 
 
 
 
-    
+
```

### Comparing `QuantumInformation-1.1/QuantumInformation/chap3_linearalgebra.py` & `QuantumInformation-1.2/QuantumInformation/chap3_linearalgebra.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Created on Wed Nov  4 
 
-@author: pranay barkataki
+@authors: Dr. M. S. Ramkarthik and Dr. Pranay Barkataki
 """
 import numpy as np
 import math
 import cmath
 import scipy.linalg.lapack as la
```

### Comparing `QuantumInformation-1.1/QuantumInformation/chap4_quantumtools.py` & `QuantumInformation-1.2/QuantumInformation/chap4_quantumtools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Tue Mar  2 11:35:07 2021
 
-@author: pranay barkataki
+@authors: Dr. M. S. Ramkarthik and Dr. Pranay Barkataki
 """
 
 import numpy as np
 import math
 import cmath
 from QuantumInformation import RecurNum
 from QuantumInformation import QuantumMechanics as QM
@@ -565,8 +565,8 @@
         
     
 
         
         
         
         
-        
+
```

### Comparing `QuantumInformation-1.1/QuantumInformation/chap5_partial_quantumentanglement.py` & `QuantumInformation-1.2/QuantumInformation/chap5_partial_quantumentanglement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Created on Thu Aug 22 19:18:53 2019
 
-@author: Pranay Barkataki 
+@authors: Dr. M. S. Ramkarthik and Dr. Pranay Barkataki
 """
 
 import numpy as np
 import math
 from QuantumInformation import RecurNum
 from QuantumInformation import LinearAlgebra as LA
 from QuantumInformation import QuantumMechanics as QM
```

### Comparing `QuantumInformation-1.1/QuantumInformation/chap6_hamiltonians.py` & `QuantumInformation-1.2/QuantumInformation/chap6_hamiltonians.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Created on Sun Jul  7 17:42:28 2019
 
-@authors: Pranay Barkataki 
+@authors: Dr. M. S. Ramkarthik and Dr. Pranay Barkataki
 
 Nth neighbor inhomogeneous spin interaction Hamiltonian with periodic boundary 
 condition
 """
 import numpy as np
 from QuantumInformation import QuantumMechanics as QM
 qobj=QM()
```

### Comparing `QuantumInformation-1.1/QuantumInformation/chap7_randommatrix.py` & `QuantumInformation-1.2/QuantumInformation/chap7_randommatrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Created on Thu Aug 22 19:18:53 2019
 
-@author: Pranay Barkataki 
+@authors: Dr. M. S. Ramkarthik and Dr. Pranay Barkataki
 """
 #import scipy.linalg.lapack as la
 import numpy as np
 import re
 
 class QRandom:
     def __init__(self):
@@ -312,8 +312,8 @@
         
         
         
         
         
         
         
-    
+
```

### Comparing `QuantumInformation-1.1/QuantumInformation.egg-info/PKG-INFO` & `QuantumInformation-1.2/QuantumInformation.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 Metadata-Version: 2.1
 Name: QuantumInformation
-Version: 1.1
+Version: 1.2
 Summary: Quantum Information and Computation package
-Home-page: UNKNOWN
 Author: M. S. Ramkarthik and Pranay Barkataki
-License: UNKNOWN
-Platform: UNKNOWN
+Requires-Python: >= 3.7.9
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 
 # QuantumInformation package
-This package contains numerous numerical methods for various quantum information and computation problems. The explanation of each of the numerical methods are explained in detail in the following book, ***"An Object Oriented Python Cookbook for Quantum Information Theory and Quantum Computing"***. The book contains more than 100 numerical routines in python and it will be extremely useful for a practising physicist, both theoretical and experimentl, working in the areas of quantum information theory, quantum computing, quantum entanglement and also on condensed matter quantum many-body spin half chains. We also remark here that, there is a chapter devoted to numerical linear algebra procedures and a final chapter on random states and matrices too. We can safely and humbly say that, the computational libraries cover a wide spectrum of topics. The hyperlink to buy the book will soon be updated, stay tuned.
+This package contains numerous numerical methods for various quantum information and computation problems. The explanation of each of the numerical methods are explained in detail in the following book, ***"An Object Oriented Python Cookbook for Quantum Information Theory and Quantum Computing"***. The book contains more than 100 numerical routines in python and it will be extremely useful for a practising physicist, both theoretical and experimentl, working in the areas of quantum information theory, quantum computing, quantum entanglement and also on condensed matter quantum many-body spin half chains. We also remark here that, there is a chapter devoted to numerical linear algebra procedures and a final chapter on random states and matrices too. We can safely and humbly say that, the computational libraries cover a wide spectrum of topics. You can easily buy the book by clicking [here](https://www.routledge.com/An-Object-Oriented-Python-Cookbook-in-Quantum-Information-Theory-and-Quantum/Ramkarthik-Barkataki/p/book/9781032256078)
+
+![alt text](https://github.com/pranay1990/QuantumInformation/blob/main/python%20book%20image.jpg)
 
 ## Files
 
 The functionality of each module is extensively discussed in the book.
 
 ## Installation
 Type the following command in the terminal of Linux or the command prompt of Windows, in order to install the package in your local computer.
 
 **pip install QuantumInformation**
 
 ## License
-Copyright 2021 CRC Press
+Copyright 2023 CRC Press
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, distribute, sublicense, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 ***THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.***
-
-
-
-
```

### Comparing `QuantumInformation-1.1/QuantumInformation.egg-info/SOURCES.txt` & `QuantumInformation-1.2/QuantumInformation.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+README.md
 setup.py
 QuantumInformation/RecurNum.py
 QuantumInformation/__init__.py
 QuantumInformation/chap2_nutsboltsquantum.py
 QuantumInformation/chap3_linearalgebra.py
 QuantumInformation/chap4_quantumtools.py
 QuantumInformation/chap5_partial_quantumentanglement.py
 QuantumInformation/chap6_hamiltonians.py
 QuantumInformation/chap7_randommatrix.py
 QuantumInformation.egg-info/PKG-INFO
 QuantumInformation.egg-info/SOURCES.txt
 QuantumInformation.egg-info/dependency_links.txt
 QuantumInformation.egg-info/not-zip-safe
+QuantumInformation.egg-info/requires.txt
 QuantumInformation.egg-info/top_level.txt
```

### Comparing `QuantumInformation-1.1/setup.py` & `QuantumInformation-1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from setuptools import setup
 
 from pathlib import Path
 this_directory = Path(__file__).parent
-long_description = (this_directory / "QuantumInformation/README.md").read_text()
+long_description = (this_directory / "README.md").read_text()
 
 setup(name="QuantumInformation",
-     version='1.1',
+     version='1.2',
      description='Quantum Information and Computation package',
      author = 'M. S. Ramkarthik and Pranay Barkataki',
      email = 'pranay.barkataki@gmail.com',
      packages=['QuantumInformation'],
      long_description=long_description,
      long_description_content_type='text/markdown',
-     zip_safe=False) 
+     zip_safe=False, 
+     install_requires = ["numpy >= 1.25.2", "scipy >= 1.11.1"],
+     extras_require = {"dev": ["pytest >= 7.0", "twine >= 4.0.2"]}, 
+     python_requires = ">= 3.7.9")
```

