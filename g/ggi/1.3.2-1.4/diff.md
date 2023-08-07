# Comparing `tmp/ggi-1.3.2.tar.gz` & `tmp/ggi-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Apr 11 02:40:59 2022, from Unix
+gzip compressed data, last modified: Mon Aug  7 17:05:42 2023, from Unix
```

## Comparing `ggi-1.3.2.tar` & `ggi-1.4.tar`

### file list

```diff
@@ -1,36 +1,34 @@
-drwxr-xr-x   0 ulises     (502) staff       (20)        0 2022-04-11 02:40:57.000000 ggi-1.3.2/
--rw-r--r--   0 ulises     (502) staff       (20)      252 2022-04-11 02:40:53.000000 ggi-1.3.2/PKG-INFO
-drwxr-xr-x   0 ulises     (502) staff       (20)        0 2022-04-11 02:40:57.000000 ggi-1.3.2/ext_bin/
--rw-r--r--   0 ulises     (502) staff       (20)     1073 2021-08-09 20:41:21.000000 ggi-1.3.2/LICENSE
-drwxr-xr-x   0 ulises     (502) staff       (20)        0 2022-04-11 02:40:53.000000 ggi-1.3.2/ggpy/
--rw-r--r--   0 ulises     (502) staff       (20)     1965 2022-03-14 22:47:54.000000 ggi-1.3.2/README.md
--rw-r--r--   0 ulises     (502) staff       (20)     1996 2022-04-11 02:40:32.000000 ggi-1.3.2/setup.py
-drwxr-xr-x   0 ulises     (502) staff       (20)        0 2022-04-11 02:40:53.000000 ggi-1.3.2/scripts/
--rw-r--r--   0 ulises     (502) staff       (20)       38 2022-04-11 02:40:53.000000 ggi-1.3.2/setup.cfg
--rw-r--r--   0 ulises     (502) staff       (20)     3268 2021-06-20 04:31:04.000000 ggi-1.3.2/scripts/root_groups.py
--rw-r--r--   0 ulises     (502) staff       (20)    15033 2022-04-10 23:42:15.000000 ggi-1.3.2/ggpy/classifier.py
--rw-r--r--   0 ulises     (502) staff       (20)        0 2021-05-22 00:43:28.000000 ggi-1.3.2/ggpy/__init__.py
--rw-r--r--   0 ulises     (502) staff       (20)    12350 2022-03-27 00:54:40.000000 ggi-1.3.2/ggpy/cli.py
--rw-r--r--   0 ulises     (502) staff       (20)     5960 2022-03-01 17:22:40.000000 ggi-1.3.2/ggpy/utils.py
--rw-r--r--   0 ulises     (502) staff       (20)    14163 2022-03-14 22:38:19.000000 ggi-1.3.2/ggpy/wrappers.py
--rw-r--r--   0 ulises     (502) staff       (20)    19385 2022-03-14 22:34:53.000000 ggi-1.3.2/ggpy/ggi.py
--rw-r--r--   0 ulises     (502) staff       (20)      120 2022-04-11 02:40:57.000000 ggi-1.3.2/ext_bin/._.DS_Store
--rw-r--r--   0 ulises     (502) staff       (20)     6148 2022-04-11 02:40:57.884655 ggi-1.3.2/ext_bin/.DS_Store
-drwxr-xr-x   0 ulises     (502) staff       (20)        0 2022-04-11 02:40:57.000000 ggi-1.3.2/ext_bin/consel/
-drwxr-xr-x   0 ulises     (502) staff       (20)        0 2022-04-11 02:40:57.000000 ggi-1.3.2/ext_bin/raxml/
--rwxr-xr-x   0 ulises     (502) staff       (20)  1569209 2022-04-11 02:40:57.000000 ggi-1.3.2/ext_bin/raxml/raxmlHPC-PTHREADS-SSE3.exe
--rwxr-xr-x   0 ulises     (502) staff       (20)  1060208 2022-04-11 02:40:57.000000 ggi-1.3.2/ext_bin/raxml/raxmlHPC-SSE3_Darwin_64bit
--rwxr-xr-x   0 ulises     (502) staff       (20)  1372480 2022-04-11 02:40:57.000000 ggi-1.3.2/ext_bin/raxml/raxmlHPC-SSE3.exe
--rwxr-xr-x   0 ulises     (502) staff       (20)  1133160 2022-04-11 02:40:57.000000 ggi-1.3.2/ext_bin/raxml/raxmlHPC-PTHREADS-SSE3_Darwin_64bit
--rwxr-xr-x   0 ulises     (502) staff       (20)  1247088 2022-04-11 02:40:57.000000 ggi-1.3.2/ext_bin/raxml/raxmlHPC-PTHREADS-SSE3_Linux_64bit
--rwxr-xr-x   0 ulises     (502) staff       (20)  1185960 2022-04-11 02:40:57.000000 ggi-1.3.2/ext_bin/raxml/raxmlHPC-SSE3_Linux_64bit
-drwxr-xr-x   0 ulises     (502) staff       (20)        0 2022-04-11 02:40:57.000000 ggi-1.3.2/ext_bin/consel/linux/
-drwxr-xr-x   0 ulises     (502) staff       (20)        0 2022-04-11 02:40:57.000000 ggi-1.3.2/ext_bin/consel/darwin/
--rwxr-xr-x   0 ulises     (502) staff       (20)   101280 2022-04-11 02:40:57.000000 ggi-1.3.2/ext_bin/consel/darwin/makermt
--rwxr-xr-x   0 ulises     (502) staff       (20)    76976 2022-04-11 02:40:57.000000 ggi-1.3.2/ext_bin/consel/darwin/seqmt
--rwxr-xr-x   0 ulises     (502) staff       (20)   166344 2022-04-11 02:40:57.000000 ggi-1.3.2/ext_bin/consel/darwin/consel
--rwxr-xr-x   0 ulises     (502) staff       (20)    76688 2022-04-11 02:40:57.000000 ggi-1.3.2/ext_bin/consel/darwin/catpv
--rwxr-xr-x   0 ulises     (502) staff       (20)    86320 2022-04-11 02:40:57.000000 ggi-1.3.2/ext_bin/consel/linux/makermt
--rwxr-xr-x   0 ulises     (502) staff       (20)    51288 2022-04-11 02:40:57.000000 ggi-1.3.2/ext_bin/consel/linux/seqmt
--rwxr-xr-x   0 ulises     (502) staff       (20)   176832 2022-04-11 02:40:57.000000 ggi-1.3.2/ext_bin/consel/linux/consel
--rwxr-xr-x   0 ulises     (502) staff       (20)    57856 2022-04-11 02:40:57.000000 ggi-1.3.2/ext_bin/consel/linux/catpv
+drwxr-xr-x   0 ulises     (502) staff       (20)        0 2023-08-07 17:05:41.000000 ggi-1.4/
+-rw-r--r--   0 ulises     (502) staff       (20)      250 2023-08-07 17:05:36.000000 ggi-1.4/PKG-INFO
+drwxr-xr-x   0 ulises     (502) staff       (20)        0 2023-08-07 17:05:41.000000 ggi-1.4/ext_bin/
+-rw-r--r--   0 ulises     (502) staff       (20)     1073 2023-08-07 16:48:59.000000 ggi-1.4/LICENSE
+drwxr-xr-x   0 ulises     (502) staff       (20)        0 2023-08-07 17:05:36.000000 ggi-1.4/ggpy/
+-rw-r--r--   0 ulises     (502) staff       (20)     1999 2023-08-07 17:03:54.000000 ggi-1.4/README.md
+-rw-r--r--   0 ulises     (502) staff       (20)     2011 2023-08-07 17:05:24.000000 ggi-1.4/setup.py
+drwxr-xr-x   0 ulises     (502) staff       (20)        0 2023-08-07 17:05:36.000000 ggi-1.4/scripts/
+-rw-r--r--   0 ulises     (502) staff       (20)       38 2023-08-07 17:05:36.000000 ggi-1.4/setup.cfg
+-rw-r--r--   0 ulises     (502) staff       (20)     3268 2023-08-07 16:48:59.000000 ggi-1.4/scripts/root_groups.py
+-rw-r--r--   0 ulises     (502) staff       (20)    15033 2023-08-07 16:48:59.000000 ggi-1.4/ggpy/classifier.py
+-rw-r--r--   0 ulises     (502) staff       (20)        0 2023-08-07 16:48:59.000000 ggi-1.4/ggpy/__init__.py
+-rw-r--r--   0 ulises     (502) staff       (20)    12559 2023-08-07 16:58:15.000000 ggi-1.4/ggpy/cli.py
+-rw-r--r--   0 ulises     (502) staff       (20)     5960 2023-08-07 16:48:59.000000 ggi-1.4/ggpy/utils.py
+-rw-r--r--   0 ulises     (502) staff       (20)    14163 2023-08-07 16:48:59.000000 ggi-1.4/ggpy/wrappers.py
+-rw-r--r--   0 ulises     (502) staff       (20)    19385 2023-08-07 16:48:59.000000 ggi-1.4/ggpy/ggi.py
+drwxr-xr-x   0 ulises     (502) staff       (20)        0 2023-08-07 17:05:41.000000 ggi-1.4/ext_bin/consel/
+drwxr-xr-x   0 ulises     (502) staff       (20)        0 2023-08-07 17:05:41.000000 ggi-1.4/ext_bin/raxml/
+-rwxr-xr-x   0 ulises     (502) staff       (20)  1569209 2023-08-07 17:05:41.000000 ggi-1.4/ext_bin/raxml/raxmlHPC-PTHREADS-SSE3.exe
+-rwxr-xr-x   0 ulises     (502) staff       (20)  1060208 2023-08-07 17:05:41.000000 ggi-1.4/ext_bin/raxml/raxmlHPC-SSE3_Darwin_64bit
+-rwxr-xr-x   0 ulises     (502) staff       (20)  1372480 2023-08-07 17:05:41.000000 ggi-1.4/ext_bin/raxml/raxmlHPC-SSE3.exe
+-rwxr-xr-x   0 ulises     (502) staff       (20)  1133160 2023-08-07 17:05:41.000000 ggi-1.4/ext_bin/raxml/raxmlHPC-PTHREADS-SSE3_Darwin_64bit
+-rwxr-xr-x   0 ulises     (502) staff       (20)  1247088 2023-08-07 17:05:41.000000 ggi-1.4/ext_bin/raxml/raxmlHPC-PTHREADS-SSE3_Linux_64bit
+-rwxr-xr-x   0 ulises     (502) staff       (20)  1185960 2023-08-07 17:05:41.000000 ggi-1.4/ext_bin/raxml/raxmlHPC-SSE3_Linux_64bit
+drwxr-xr-x   0 ulises     (502) staff       (20)        0 2023-08-07 17:05:41.000000 ggi-1.4/ext_bin/consel/linux/
+drwxr-xr-x   0 ulises     (502) staff       (20)        0 2023-08-07 17:05:41.000000 ggi-1.4/ext_bin/consel/darwin/
+-rwxr-xr-x   0 ulises     (502) staff       (20)   101280 2023-08-07 17:05:41.000000 ggi-1.4/ext_bin/consel/darwin/makermt
+-rwxr-xr-x   0 ulises     (502) staff       (20)    76976 2023-08-07 17:05:41.000000 ggi-1.4/ext_bin/consel/darwin/seqmt
+-rwxr-xr-x   0 ulises     (502) staff       (20)   166344 2023-08-07 17:05:41.000000 ggi-1.4/ext_bin/consel/darwin/consel
+-rwxr-xr-x   0 ulises     (502) staff       (20)    76688 2023-08-07 17:05:41.000000 ggi-1.4/ext_bin/consel/darwin/catpv
+-rwxr-xr-x   0 ulises     (502) staff       (20)    86320 2023-08-07 17:05:41.000000 ggi-1.4/ext_bin/consel/linux/makermt
+-rwxr-xr-x   0 ulises     (502) staff       (20)    51288 2023-08-07 17:05:41.000000 ggi-1.4/ext_bin/consel/linux/seqmt
+-rwxr-xr-x   0 ulises     (502) staff       (20)   176832 2023-08-07 17:05:41.000000 ggi-1.4/ext_bin/consel/linux/consel
+-rwxr-xr-x   0 ulises     (502) staff       (20)    57856 2023-08-07 17:05:41.000000 ggi-1.4/ext_bin/consel/linux/catpv
```

### Comparing `ggi-1.3.2/LICENSE` & `ggi-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ggi-1.3.2/README.md` & `ggi-1.4/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,55 @@
 # GGpy
 
-GGI automatization
+GGI automatization and feature extraction
 
 Software requierements:
 
 * pip
 * python3
 
 
 ## Installation
 
 It is advisable to install this package inside a [conda](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) or [python environment](https://docs.python.org/3/library/venv.html) if there are issues with system permissions.
 
 Using `pip`:
 
+<!-- # pip install numpy # needed for python<3.7 -->
+
 ```Bash
-pip install numpy # needed for python<3.7
 pip install ggi
 ```
 
-
 Using `git` and `pip` (Optional):
+<!-- python3 -m pip install numpy # needed for python<3.7 -->
 ```Bash
 git clone https://github.com/Ulises-Rosas/GGpy.git
 cd GGpy
-python3 -m pip install numpy # needed for python<3.7
 python3 -m pip install .
 ```
 
 ## Usage
 
 Main Command:
 
 ```Bash
 ggpy -h
 ```
 
 ```
 usage: ggpy [-h] {ggi,features,post} ...
 
-                                 GGI and Post-GGI
+                                 GGI and more
                                       
 
 positional arguments:
   {ggi,features,post}
     ggi                Gene-Genealogy Interrogation (GGI)
     features           Features from both alignment and tree information
-    post               Classification of GGI hypothesis based on features
 
 optional arguments:
   -h, --help           show this help message and exit
 ```
 ### GGI
 
 ```Bash
@@ -67,16 +66,16 @@
 
 Utilities
 
 * `root_groups.py` : Root groups at ggpy results
 
 ### Features
 
+Feature extraction from alignments and sequences
+
 ```Bash
 ggpy features -A [alignment file extension] -T [tree file extension]
 ```
+### TODO
 
-### post-GGI
+- Add a machine learning model to make a non-linear regression between labels from ggi and features
 
-```Bash
-ggpy post [ggi result] -f [features result] -c [comparison file]
-```
```

### Comparing `ggi-1.3.2/setup.py` & `ggi-1.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,27 +37,27 @@
     sys.stderr.flush()
     exit()
 
 
 dependencies = [
     "fishlifetraits>=0.5.0", # own package
     'dendropy==4.4.0',
-    'shap',
+    # 'shap',
     # 'joblib',
-    'xgboost',
-    'pandas',
-    'scikit-learn',
-    'matplotlib',
+    # 'xgboost==1.4.1',
+    # 'pandas',
+    # 'scikit-learn',
+    # 'matplotlib',
 ]
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(name = "ggi",
-      version = '1.3.2',
+      version = '1.4',
       maintainer = 'Ulises Rosas',
     #   long_description = readme,
     #   long_description_content_type = 'text/markdown',
       url ='https://github.com/Ulises-Rosas/GGpy',
       packages = ['ggpy'],
       package_data = {'ggpy': ['data/*']} ,
       data_files = [ ('bin', bins) ],
```

### Comparing `ggi-1.3.2/scripts/root_groups.py` & `ggi-1.4/scripts/root_groups.py`

 * *Files identical despite different names*

### Comparing `ggi-1.3.2/ggpy/classifier.py` & `ggi-1.4/ggpy/classifier.py`

 * *Files identical despite different names*

### Comparing `ggi-1.3.2/ggpy/cli.py` & `ggi-1.4/ggpy/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 # ITT_OUTFILENAME = "support_tt.tsv"
 # RF_OUTFILENAME = "RF_distance.tsv"
 
 parser = argparse.ArgumentParser( formatter_class = argparse.RawDescriptionHelpFormatter, 
                                       description = '''
-                                 GGI and Post-GGI
+                                    GGI and more
                                       ''')
 subparsers = parser.add_subparsers(help='', dest='subcommand')
 
 # ggi -------------------------------------------------------------------------
 ggi = subparsers.add_parser('ggi',
                              help = "Gene-Genealogy Interrogation (GGI)",
                              formatter_class = argparse.RawDescriptionHelpFormatter, 
@@ -142,15 +142,16 @@
 Examples:
 
     * Standard usage:
 
         $ %(prog)s -A [alignment file extension] -T [tree file extension]
 
             Where '-A' and '-T' indicate file extensions for alignments and 
-            trees, correspondingly.
+            trees, correspondingly. For each pair alignment and tree, extensions
+            are taken out and leftovers should match
 
 """)
 fstats.add_argument('-A','--aln',
                     metavar="ext",
                     type= str,
                     # required=True,
                     default=".fasta",
@@ -193,69 +194,69 @@
 fstats.add_argument('-n', '--threads',
                     metavar = "",
                     type    = int,
                     default = 1,
                     help    = '[Optional] number of cpus [Default = 1]')          
 # fstats -----------------------------------------------------------------------
 
-# post_ggi --------------------------------------------------------------------------
-post_ggi_sub = subparsers.add_parser('post', help = "Classification of GGI hypothesis based on features",
-                              formatter_class = argparse.RawDescriptionHelpFormatter, 
-                              description="""
+# # post_ggi --------------------------------------------------------------------------
+# post_ggi_sub = subparsers.add_parser('post', help = "Classification of GGI hypothesis based on features",
+#                               formatter_class = argparse.RawDescriptionHelpFormatter, 
+#                               description="""
                               
-                    Post-GGI
-Examples:
-
-    * Standard usage:
+#                     Post-GGI
+# Examples:
 
-        $ %(prog)s [ggi result] -f [features result] -c [comparison file]
-
-        note 1: feature file is obtained from the 'features' subcomand
-        note 2: comparison file is a CSV-formated file and it containts
-                pairs of tree ids from the ggi result file:
-
-                1,2
-                1,3
-                ...
-
-                In above example, hypothesis 1 and hypothesis 2 are compared,
-                then hypothesis 1 and hypothesis 3 are compared, and so on.
-
-""")
+#     * Standard usage:
 
-post_ggi_sub.add_argument('all_ggi_results',
-                      metavar = 'file',
-                      help='file from the "ggi" subcomand')
-post_ggi_sub.add_argument('-f','--features',
-                    metavar="",
-                    type= str,
-                    required=True,
-                    help='File with features of alignments and trees [Default: None]')
-post_ggi_sub.add_argument('-c','--comparisons',
-                    metavar="",
-                    type= str,
-                    required=True,
-                    help='File with hypothesis id to compare [Default: None]')
+#         $ %(prog)s [ggi result] -f [features result] -c [comparison file]
 
-post_ggi_sub.add_argument('-s','--suffix', 
-                        metavar="",
-                        type = str,
-                        default='post_ggi',
-                        help='[Optional] prefix name for outputs [Default = post_ggi]' )
-post_ggi_sub.add_argument('-l', '--ncols',
-                    metavar = "",
-                    type    = int,
-                    default = 3,
-                    help    = '[Optional] number of columns for plotting confusion matrices [Default = 3]') 
-post_ggi_sub.add_argument('-n', '--threads',
-                    metavar = "",
-                    type    = int,
-                    default = 1,
-                    help    = '[Optional] number of cpus [Default = 1]') 
-# post_ggi --------------------------------------------------------------------------
+#         note 1: feature file is obtained from the 'features' subcomand
+#         note 2: comparison file is a CSV-formated file and it containts
+#                 pairs of tree ids from the ggi result file:
+
+#                 1,2
+#                 1,3
+#                 ...
+
+#                 In above example, hypothesis 1 and hypothesis 2 are compared,
+#                 then hypothesis 1 and hypothesis 3 are compared, and so on.
+
+# """)
+
+# post_ggi_sub.add_argument('all_ggi_results',
+#                       metavar = 'file',
+#                       help='file from the "ggi" subcomand')
+# post_ggi_sub.add_argument('-f','--features',
+#                     metavar="",
+#                     type= str,
+#                     required=True,
+#                     help='File with features of alignments and trees [Default: None]')
+# post_ggi_sub.add_argument('-c','--comparisons',
+#                     metavar="",
+#                     type= str,
+#                     required=True,
+#                     help='File with hypothesis id to compare [Default: None]')
+
+# post_ggi_sub.add_argument('-s','--suffix', 
+#                         metavar="",
+#                         type = str,
+#                         default='post_ggi',
+#                         help='[Optional] prefix name for outputs [Default = post_ggi]' )
+# post_ggi_sub.add_argument('-l', '--ncols',
+#                     metavar = "",
+#                     type    = int,
+#                     default = 3,
+#                     help    = '[Optional] number of columns for plotting confusion matrices [Default = 3]') 
+# post_ggi_sub.add_argument('-n', '--threads',
+#                     metavar = "",
+#                     type    = int,
+#                     default = 1,
+#                     help    = '[Optional] number of cpus [Default = 1]') 
+# # post_ggi --------------------------------------------------------------------------
 
 
 def main():
 
     wholeargs = parser.parse_args()
 
     if wholeargs.subcommand == "ggi":
@@ -290,23 +291,23 @@
             groups_file    = None,
             codon_aware    = wholeargs.codon_aware,
             sym_tests      = False,
             threads        = wholeargs.threads,
             suffix         = wholeargs.suffix,
         ).write_stats()
 
-    elif wholeargs.subcommand == "post":
+    # elif wholeargs.subcommand == "post":
 
-        from ggpy.classifier import Post_ggi
+    #     from ggpy.classifier import Post_ggi
 
-        Post_ggi(
-            feature_file    = wholeargs.features,
-            all_ggi_results  = wholeargs.all_ggi_results,
-            file_comparisons = wholeargs.comparisons,
-            model_prefix     = wholeargs.suffix,
-            cnfx_ncols       = wholeargs.ncols,
-            threads          = wholeargs.threads
+    #     Post_ggi(
+    #         feature_file    = wholeargs.features,
+    #         all_ggi_results  = wholeargs.all_ggi_results,
+    #         file_comparisons = wholeargs.comparisons,
+    #         model_prefix     = wholeargs.suffix,
+    #         cnfx_ncols       = wholeargs.ncols,
+    #         threads          = wholeargs.threads
 
-        ).xgboost_iterator()
+    #     ).xgboost_iterator()
 
 if __name__ == "__main__":
     main()
```

### Comparing `ggi-1.3.2/ggpy/utils.py` & `ggi-1.4/ggpy/utils.py`

 * *Files identical despite different names*

### Comparing `ggi-1.3.2/ggpy/wrappers.py` & `ggi-1.4/ggpy/wrappers.py`

 * *Files identical despite different names*

### Comparing `ggi-1.3.2/ggpy/ggi.py` & `ggi-1.4/ggpy/ggi.py`

 * *Files identical despite different names*

### Comparing `ggi-1.3.2/ext_bin/raxml/raxmlHPC-PTHREADS-SSE3.exe` & `ggi-1.4/ext_bin/raxml/raxmlHPC-PTHREADS-SSE3.exe`

 * *Files identical despite different names*

### Comparing `ggi-1.3.2/ext_bin/raxml/raxmlHPC-SSE3_Darwin_64bit` & `ggi-1.4/ext_bin/raxml/raxmlHPC-SSE3_Darwin_64bit`

 * *Files identical despite different names*

### Comparing `ggi-1.3.2/ext_bin/raxml/raxmlHPC-SSE3.exe` & `ggi-1.4/ext_bin/raxml/raxmlHPC-SSE3.exe`

 * *Files identical despite different names*

### Comparing `ggi-1.3.2/ext_bin/raxml/raxmlHPC-PTHREADS-SSE3_Darwin_64bit` & `ggi-1.4/ext_bin/raxml/raxmlHPC-PTHREADS-SSE3_Darwin_64bit`

 * *Files identical despite different names*

### Comparing `ggi-1.3.2/ext_bin/raxml/raxmlHPC-PTHREADS-SSE3_Linux_64bit` & `ggi-1.4/ext_bin/raxml/raxmlHPC-PTHREADS-SSE3_Linux_64bit`

 * *Files identical despite different names*

### Comparing `ggi-1.3.2/ext_bin/raxml/raxmlHPC-SSE3_Linux_64bit` & `ggi-1.4/ext_bin/raxml/raxmlHPC-SSE3_Linux_64bit`

 * *Files identical despite different names*

### Comparing `ggi-1.3.2/ext_bin/consel/darwin/makermt` & `ggi-1.4/ext_bin/consel/darwin/makermt`

 * *Files identical despite different names*

### Comparing `ggi-1.3.2/ext_bin/consel/darwin/seqmt` & `ggi-1.4/ext_bin/consel/darwin/seqmt`

 * *Files identical despite different names*

### Comparing `ggi-1.3.2/ext_bin/consel/darwin/consel` & `ggi-1.4/ext_bin/consel/darwin/consel`

 * *Files identical despite different names*

### Comparing `ggi-1.3.2/ext_bin/consel/darwin/catpv` & `ggi-1.4/ext_bin/consel/darwin/catpv`

 * *Files identical despite different names*

### Comparing `ggi-1.3.2/ext_bin/consel/linux/makermt` & `ggi-1.4/ext_bin/consel/linux/makermt`

 * *Files identical despite different names*

### Comparing `ggi-1.3.2/ext_bin/consel/linux/seqmt` & `ggi-1.4/ext_bin/consel/linux/seqmt`

 * *Files identical despite different names*

### Comparing `ggi-1.3.2/ext_bin/consel/linux/consel` & `ggi-1.4/ext_bin/consel/linux/consel`

 * *Files identical despite different names*

### Comparing `ggi-1.3.2/ext_bin/consel/linux/catpv` & `ggi-1.4/ext_bin/consel/linux/catpv`

 * *Files identical despite different names*

