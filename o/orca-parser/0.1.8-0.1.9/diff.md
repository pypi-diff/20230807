# Comparing `tmp/orca_parser-0.1.8-py2.py3-none-any.whl.zip` & `tmp/orca_parser-0.1.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7025 bytes, number of entries: 8
+Zip file size: 7242 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat     3325 b- defN 23-Jul-06 09:45 orca_parser/HessianTools.py
--rw-rw-rw-  2.0 fat    12317 b- defN 23-Aug-01 20:49 orca_parser/ORCAParse.py
+-rw-rw-rw-  2.0 fat    13289 b- defN 23-Aug-02 10:55 orca_parser/ORCAParse.py
 -rw-rw-rw-  2.0 fat      287 b- defN 23-Jul-06 09:50 orca_parser/__init__.py
--rw-rw-rw-  2.0 fat     1235 b- defN 23-Aug-01 20:50 orca_parser-0.1.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      482 b- defN 23-Aug-01 20:50 orca_parser-0.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Aug-01 20:50 orca_parser-0.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Aug-01 20:50 orca_parser-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      651 b- defN 23-Aug-01 20:50 orca_parser-0.1.8.dist-info/RECORD
-8 files, 18419 bytes uncompressed, 5889 bytes compressed:  68.0%
+-rw-rw-rw-  2.0 fat     1235 b- defN 23-Aug-02 10:57 orca_parser-0.1.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      482 b- defN 23-Aug-02 10:57 orca_parser-0.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Aug-02 10:57 orca_parser-0.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Aug-02 10:57 orca_parser-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      651 b- defN 23-Aug-02 10:57 orca_parser-0.1.9.dist-info/RECORD
+8 files, 19391 bytes uncompressed, 6106 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: orca_parser/ORCAParse.py
 Comment: 
 
 Filename: orca_parser/__init__.py
 Comment: 
 
-Filename: orca_parser-0.1.8.dist-info/LICENSE
+Filename: orca_parser-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: orca_parser-0.1.8.dist-info/METADATA
+Filename: orca_parser-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: orca_parser-0.1.8.dist-info/WHEEL
+Filename: orca_parser-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: orca_parser-0.1.8.dist-info/top_level.txt
+Filename: orca_parser-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: orca_parser-0.1.8.dist-info/RECORD
+Filename: orca_parser-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## orca_parser/ORCAParse.py

```diff
@@ -4,28 +4,32 @@
 
 @author: Alex
 """
 import numpy as np
 import ase, pandas
 from ase.io import read
 
-def readin(fname):
-    # ORCA sometimes makes output that is hard to parse, we will try to read it the quick way first
+
+
+def tricky_readin(fname):
+    # Frist try a linux / archie output
     try:
-        f = open(fname)
-        content = f.read()
-        f.close()
-        return content
+        with open(fname, "rb") as f:
+            content = f.read().decode("utf-8")
+        #print("Encoded as UTF-8")
     except:
-        content = ""
-        with open(fname, 'rb') as f:
-            for line in f:
-                content = content + line.decode("utf-8", errors='ignore') + "\n"
-        return content
-
+        # next try a winwdows 10/11 encoding
+        try:    
+            with open(fname, "rb") as f:
+                content = f.read().decode("utf-16")        
+            #print("Encoded as UTF-16")
+        except:
+            content = "Couldnt decode output file as utf-8 or utf-16"
+            print(content)
+    return content
 
 def fit_rms(ref_c,c):
     # move geometric center to the origin
     ref_trans = np.average(ref_c, axis=0)
     ref_c = ref_c - ref_trans
     c_trans = np.average(c, axis=0)
     c = c - c_trans
@@ -165,18 +169,30 @@
         if "out the resulting rotational entropy values for" in self.raw:
             symmetric_number = self.raw.split("Final Gibbs free energy         ...")[-2].split("out the resulting rotational entropy values for")[1]
             symmetric_number = symmetric_number.split("--------------------------------------------------------")[1]
             self.symmetry_number = symmetric_number.count("sn=")
         else:
             self.symmetry_number = 2
         
-        self.AllGibbs = [float(x.split("\n")[0].strip().split()[0]) for x in self.raw.split("Final Gibbs free energy         ...")[1:]]
-        self.Gibbs = float(self.raw.split("Final Gibbs free energy         ...")[-1].split("\n")[0].strip().split()[0])
-        self.entropies = [float(x.split("\n")[0].strip().split()[0]) for x in self.raw.split("Total enthalpy                    ...")[1:]]
-        self.enthalpies = [float(x.split("\n")[0].strip().split()[0]) for x in self.raw.split("Total entropy correction          ...")[1:]]
+        
+        frames = self.raw.split("GEOMETRY OPTIMIZATION CYCLE")
+        
+        self.AllGibbs = {}
+        self.entropies = {}
+        self.enthalpies = {}
+        for i, frame in enumerate(frames):
+            print("Frame:", i)
+            if "Final Gibbs free energy" in frame:
+                G = frame.split("Final Gibbs free energy         ...")[1].split("Eh")[0]
+                H = frame.split("Total enthalpy                    ...")[1].split("Eh")[0]
+                S = frame.split("Total entropy correction          ...")[1].split("Eh")[0]
+                self.AllGibbs[i] = float(G)
+                self.enthalpies[i] = float(H)
+                self.entropies[i] = float(S)
+        self.Gibbs = list(self.AllGibbs.values())[-1]
         
         
         
     def seconds(self):
         time_str = self.raw.split("TOTAL RUN TIME:")[1].strip().split()
         days = int(time_str[0])
         hours = int(time_str[2])
@@ -187,43 +203,46 @@
         hours = hours + (days*24)
         minutes = minutes + (hours*60)
         seconds = seconds + (minutes*60)
         seconds = seconds + (miliseconds/1000)
         return seconds
     
     def parse_input(self):
-        self.Z = int(round(float(self.raw.split("Sum of atomic charges:")[1].split("\n")[0])))
+        self.Z = int(round(float(self.raw.split("Sum of atomic charges")[1].split("\n")[0].replace(":", ""))))
         self.Multiplicity = int(round(float(self.raw.split("* xyz")[1].replace("file","").split("\n")[0].split()[1])))
         self.orca_version = self.raw.split("Program Version ")[1].split()[0]
         inp = self.raw.split("INPUT FILE")[1].split("****END OF INPUT****")[0]
         inp = inp.split("> !")[1].split("\n")[0]
         inp = inp.upper()
         inp = inp.replace("!", "")
         inp = inp.split()
         inp_dict = {"Job": None, 
                     "Freq": False,
                     "Solvation": "Gas",
                     "Dispersion": None,
                     "Charge": self.Z,
-                    "defgrid": None,
+                    "defgrid": "DEFGRID2", #default in orca 5
                     "def2/J": None,
+                    "RIJCOSX": None,
+                    "SlowConv": None,
+                    "SCF_conv_tol": None,
                     "Multiplicity": self.Multiplicity,
                     "orca_version": self.orca_version}
         i = 0
         while i < len(inp):
             inp[i] = inp[i].upper()
             if inp[i] in ["SP", "OPT"]:
                 inp_dict["Job"] = inp[i]
                 del inp[i]
                 continue
             elif "FREQ" in inp[i]:
                 inp_dict["Freq"] = True
                 del inp[i]
                 continue
-            elif inp[i] in ["B3LYP", "PBE"] or "WB9" in inp[i]:
+            elif inp[i] in ["B3LYP", "PBE"] or "WB9" in inp[i] or inp[i][:2] == "HF":
                 inp_dict["Functional"] = inp[i]
                 del inp[i]
                 continue
             elif "CPCM" in inp[i] or "SMD" in inp[i]:
                 inp_dict["Solvation"] = inp[i]
                 del inp[i]
                 continue
@@ -239,14 +258,26 @@
                 inp_dict["defgrid"] = inp[i]
                 del inp[i]
                 continue
             elif "DEF2/J" in inp[i]:
                 inp_dict["def2/J"] = True
                 del inp[i]
                 continue
+            elif inp[i] == "RIJCOSX":
+                inp_dict["RIJCOSX"] = True
+                del inp[i]
+                continue
+            elif "SLOWCONV" in inp[i]:
+                inp_dict["SLOWCONV"] = inp[i]
+                del inp[i]
+                continue
+            elif "SCF" in inp[i]:
+                inp_dict["SCF_conv_tol"] = inp[i]
+                del inp[i]
+                continue
             i+= 1
         return inp_dict
     
     def convergence(self):
         self.conv = dict()
         self.tol = dict()
         if "Geometry convergence" not in self.raw:
@@ -300,11 +331,12 @@
                 self.CD.append(float(line[2]))
                 self.R.append(float(line[3]))
     
     
     def __init__(self, fname, verbose = False):
         self.fname = fname
         self.verbose = verbose
-        self.raw = readin(fname)
+        self.raw = tricky_readin(fname)
         self.ValidateOutput()
         self.convergence()
-        self.TDDFT = False
+        self.TDDFT = False
+
```

## Comparing `orca_parser-0.1.8.dist-info/LICENSE` & `orca_parser-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `orca_parser-0.1.8.dist-info/RECORD` & `orca_parser-0.1.9.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 orca_parser/HessianTools.py,sha256=y936_LzZ3DGpnlElVQY96RtLPaKtRbEG5zPE4T-7VYY,3325
-orca_parser/ORCAParse.py,sha256=V0q-GYrY4iZhFeUJkPbjSDiJdYYp91uw8gTiQBpN_Mg,12317
+orca_parser/ORCAParse.py,sha256=3ydK8ZJayB4MX7SIu1xuWlS_gPu8wrUuXTipEw82dXA,13289
 orca_parser/__init__.py,sha256=MlYoARmgG3uEVqcMY6rIRRYLHm0-4rh6WiSVGx-ngK4,287
-orca_parser-0.1.8.dist-info/LICENSE,sha256=Q2ptU2E48gOsMzhYz_kqVovmJ5d1KzrblLyqD2_-fvY,1235
-orca_parser-0.1.8.dist-info/METADATA,sha256=Oa4RJkLvWSzTHi9-hu3e4fdyMucGFr31m2-wzcQciTc,482
-orca_parser-0.1.8.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-orca_parser-0.1.8.dist-info/top_level.txt,sha256=8n8h8nQznt6NRgMjI0VijQ6cY5Nu7A0UUuc1M-GHe40,12
-orca_parser-0.1.8.dist-info/RECORD,,
+orca_parser-0.1.9.dist-info/LICENSE,sha256=Q2ptU2E48gOsMzhYz_kqVovmJ5d1KzrblLyqD2_-fvY,1235
+orca_parser-0.1.9.dist-info/METADATA,sha256=sx3MWAvIqomdlRo0tX8oBDsdLDbAWSXfFV93yDtZ4eA,482
+orca_parser-0.1.9.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+orca_parser-0.1.9.dist-info/top_level.txt,sha256=8n8h8nQznt6NRgMjI0VijQ6cY5Nu7A0UUuc1M-GHe40,12
+orca_parser-0.1.9.dist-info/RECORD,,
```

