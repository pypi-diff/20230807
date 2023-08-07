# Comparing `tmp/waafle-0.1.0.dev0.tar.gz` & `tmp/waafle-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/waafle-0.1.0.dev0.tar", last modified: Thu Jun 20 19:49:50 2019, max compression
+gzip compressed data, was "dist/waafle-1.0.0.tar", last modified: Mon Aug  7 16:29:49 2023, max compression
```

## Comparing `waafle-0.1.0.dev0.tar` & `waafle-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 efranzosa  (1000) efranzosa  (1000)        0 2019-06-20 19:49:50.000000 waafle-0.1.0.dev0/
--rw-rw-r--   0 efranzosa  (1000) efranzosa  (1000)     1022 2019-06-20 19:45:58.000000 waafle-0.1.0.dev0/setup.py
--rw-rw-r--   0 efranzosa  (1000) efranzosa  (1000)    18125 2019-06-20 19:49:50.000000 waafle-0.1.0.dev0/PKG-INFO
-drwxrwxr-x   0 efranzosa  (1000) efranzosa  (1000)        0 2019-06-20 19:49:50.000000 waafle-0.1.0.dev0/waafle/
--rwxrwxr-x   0 efranzosa  (1000) efranzosa  (1000)    36169 2019-06-13 16:54:24.000000 waafle-0.1.0.dev0/waafle/waafle_orgscorer.py
--rwxrwxr-x   0 efranzosa  (1000) efranzosa  (1000)     6174 2019-06-17 19:35:30.000000 waafle-0.1.0.dev0/waafle/waafle_qc.py
--rwxrwxr-x   0 efranzosa  (1000) efranzosa  (1000)       28 2018-04-06 19:40:42.000000 waafle-0.1.0.dev0/waafle/__init__.py
--rwxrwxr-x   0 efranzosa  (1000) efranzosa  (1000)    15479 2019-06-13 16:54:33.000000 waafle-0.1.0.dev0/waafle/waafle_junctions.py
--rwxrwxr-x   0 efranzosa  (1000) efranzosa  (1000)    19487 2019-06-17 19:03:11.000000 waafle-0.1.0.dev0/waafle/utils.py
--rwxrwxr-x   0 efranzosa  (1000) efranzosa  (1000)     3734 2019-06-13 16:54:06.000000 waafle-0.1.0.dev0/waafle/waafle_search.py
--rwxrwxr-x   0 efranzosa  (1000) efranzosa  (1000)     7683 2019-06-13 16:54:40.000000 waafle-0.1.0.dev0/waafle/waafle_genecaller.py
-drwxrwxr-x   0 efranzosa  (1000) efranzosa  (1000)        0 2019-06-20 19:49:50.000000 waafle-0.1.0.dev0/waafle.egg-info/
--rw-rw-r--   0 efranzosa  (1000) efranzosa  (1000)        1 2019-06-20 19:49:50.000000 waafle-0.1.0.dev0/waafle.egg-info/dependency_links.txt
--rw-rw-r--   0 efranzosa  (1000) efranzosa  (1000)      241 2019-06-20 19:49:50.000000 waafle-0.1.0.dev0/waafle.egg-info/entry_points.txt
--rw-rw-r--   0 efranzosa  (1000) efranzosa  (1000)    18125 2019-06-20 19:49:50.000000 waafle-0.1.0.dev0/waafle.egg-info/PKG-INFO
--rw-rw-r--   0 efranzosa  (1000) efranzosa  (1000)       14 2019-06-20 19:49:50.000000 waafle-0.1.0.dev0/waafle.egg-info/requires.txt
--rw-rw-r--   0 efranzosa  (1000) efranzosa  (1000)      361 2019-06-20 19:49:50.000000 waafle-0.1.0.dev0/waafle.egg-info/SOURCES.txt
--rw-rw-r--   0 efranzosa  (1000) efranzosa  (1000)        7 2019-06-20 19:49:50.000000 waafle-0.1.0.dev0/waafle.egg-info/top_level.txt
--rw-rw-r--   0 efranzosa  (1000) efranzosa  (1000)    15643 2019-06-20 18:46:24.000000 waafle-0.1.0.dev0/README.md
--rw-rw-r--   0 efranzosa  (1000) efranzosa  (1000)       38 2019-06-20 19:49:50.000000 waafle-0.1.0.dev0/setup.cfg
+drwxr-xr-x   0 sam1389    (501) staff       (20)        0 2023-08-07 16:29:49.000000 waafle-1.0.0/
+-rw-r--r--   0 sam1389    (501) staff       (20)    18972 2023-08-07 16:29:49.000000 waafle-1.0.0/PKG-INFO
+-rw-r--r--   0 sam1389    (501) staff       (20)    16423 2023-08-07 16:19:04.000000 waafle-1.0.0/README.md
+-rw-r--r--   0 sam1389    (501) staff       (20)       38 2023-08-07 16:29:49.000000 waafle-1.0.0/setup.cfg
+-rw-r--r--   0 sam1389    (501) staff       (20)     1020 2023-08-07 16:19:04.000000 waafle-1.0.0/setup.py
+drwxr-xr-x   0 sam1389    (501) staff       (20)        0 2023-08-07 16:29:49.000000 waafle-1.0.0/waafle/
+-rwxr-xr-x   0 sam1389    (501) staff       (20)       28 2023-08-07 16:19:04.000000 waafle-1.0.0/waafle/__init__.py
+-rwxr-xr-x   0 sam1389    (501) staff       (20)    19488 2023-08-07 16:19:04.000000 waafle-1.0.0/waafle/utils.py
+-rwxr-xr-x   0 sam1389    (501) staff       (20)     7683 2023-08-07 16:19:04.000000 waafle-1.0.0/waafle/waafle_genecaller.py
+-rwxr-xr-x   0 sam1389    (501) staff       (20)    15479 2023-08-07 16:19:04.000000 waafle-1.0.0/waafle/waafle_junctions.py
+-rwxr-xr-x   0 sam1389    (501) staff       (20)    36239 2023-08-07 16:19:04.000000 waafle-1.0.0/waafle/waafle_orgscorer.py
+-rwxr-xr-x   0 sam1389    (501) staff       (20)     6174 2023-08-07 16:19:04.000000 waafle-1.0.0/waafle/waafle_qc.py
+-rwxr-xr-x   0 sam1389    (501) staff       (20)     3734 2023-08-07 16:19:04.000000 waafle-1.0.0/waafle/waafle_search.py
+drwxr-xr-x   0 sam1389    (501) staff       (20)        0 2023-08-07 16:29:49.000000 waafle-1.0.0/waafle.egg-info/
+-rw-r--r--   0 sam1389    (501) staff       (20)    18972 2023-08-07 16:29:49.000000 waafle-1.0.0/waafle.egg-info/PKG-INFO
+-rw-r--r--   0 sam1389    (501) staff       (20)      361 2023-08-07 16:29:49.000000 waafle-1.0.0/waafle.egg-info/SOURCES.txt
+-rw-r--r--   0 sam1389    (501) staff       (20)        1 2023-08-07 16:29:49.000000 waafle-1.0.0/waafle.egg-info/dependency_links.txt
+-rw-r--r--   0 sam1389    (501) staff       (20)      241 2023-08-07 16:29:49.000000 waafle-1.0.0/waafle.egg-info/entry_points.txt
+-rw-r--r--   0 sam1389    (501) staff       (20)       14 2023-08-07 16:29:49.000000 waafle-1.0.0/waafle.egg-info/requires.txt
+-rw-r--r--   0 sam1389    (501) staff       (20)        7 2023-08-07 16:29:49.000000 waafle-1.0.0/waafle.egg-info/top_level.txt
```

### Comparing `waafle-0.1.0.dev0/setup.py` & `waafle-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
 with open( "README.md" ) as fh:
-    long_description = fh.read( )
+    long_description = fh.read( ) 
 
 setuptools.setup(
     name = "waafle",
-    version = "0.1.0dev",
+    version = "1.0.0",
     author = "Eric Franzosa",
     author_email = "franzosa@hsph.harvard.edu",
     license = "MIT",
-    description = "WAAFLE: a Workflow to Annotate Assemblies and find LGT Events",
+    description = "WAAFLE: a Workflow to Annotate Assemblies and Find LGT Events",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://huttenhower.sph.harvard.edu/waafle",
     packages = setuptools.find_packages( ),
     classifiers = [
         "Programming Language :: Python",
     ],
```

### Comparing `waafle-0.1.0.dev0/PKG-INFO` & `waafle-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 Metadata-Version: 2.1
 Name: waafle
-Version: 0.1.0.dev0
-Summary: WAAFLE: a Workflow to Annotate Assemblies and find LGT Events
+Version: 1.0.0
+Summary: WAAFLE: a Workflow to Annotate Assemblies and Find LGT Events
 Home-page: https://huttenhower.sph.harvard.edu/waafle
 Author: Eric Franzosa
 Author-email: franzosa@hsph.harvard.edu
 License: MIT
 Description: # WAAFLE
         
-        **WAAFLE** (a **W**orkflow to **A**nnotate **A**ssemblies and **F**ind **L**GT Events) is a method for finding novel LGT (Lateral Gene Transfer) events in assembled metagenomes, including those from human microbiomes. WAAFLE was developed in the [Huttenhower Lab](http://huttenhower.sph.harvard.edu) at the Harvard T.H. Chan School of Public Health by **Tiffany Hsu** and **Eric A. Franzosa**. Please direct questions to the [WAAFLE user group](waafle-users@googlegroups.com).
+        **WAAFLE** (a **W**orkflow to **A**nnotate **A**ssemblies and **F**ind **L**GT Events) is a method for finding novel LGT (Lateral Gene Transfer) events in assembled metagenomes, including those from human microbiomes.Please direct questions to the [bioBakery Support Forum in WAAFLE category](https://forum.biobakery.org/c/Microbial-community-profiling/WAAFLE).
         
-        [TOC]
         
         ## Citation
+        The WAAFLE manuscript has been submitted!
         
-        |Tiffany Y. Hsu, Eric A. Franzosa, Dennis Wong, Chengwei Luo, Robert G. Beiko, Morgan Langille, Curtis Huttenhower. *The landscape of novel lateral gene transfer events in the human microbiome.* (In prep.)|
-        |-|
+        Tiffany Y. Hsu*, Etienne Nzabarushimana*, Dennis Wong, Chengwei Luo, Robert G. Beiko, Morgan Langille, Curtis Huttenhower, Long H. Nguyen**, Eric A. Franzosa**.
+        
+        <h4> Profiling novel lateral gene transfer events in the human microbiome. (Submitted.) </h4>
+        
+        ```
+        [* = co-lead; ** = co-supervised]
+        ```
+        In the meantime, if you use WAAFLE in your work, please cite the WAAFLE repository on GitHub: https://github.com/biobakery/waafle.
         
-        (*While WAAFLE is not yet published, if you use WAAFLE or the datasets provided below in your work, please cite this website:* http://huttenhower.sph.harvard.edu/waafle.)
         ## Installation
         
         Install the WAAFLE software and Python dependencies with `pip`:
         
         ```
         $ pip install waafle
         ```
         
-        You can also clone the WAAFLE package from bitbucket with mercurial (`hg`):
+        You can also clone the WAAFLE package from Github:
         
         ```
-        $ hg clone https://bitbucket.org/biobakery/waafle
+        $ git clone https://github.com/biobakery/waafle.git
         ```
         
         Or download and inflate WAAFLE package directly:
         
         ```
-        $ wget https://bitbucket.org/biobakery/waafle/get/default.zip
-        $ unzip default.zip
+        $ wget https://github.com/biobakery/waafle/archive/master.zip
+        $ unzip master.zip
         ```
         
         ## Software requirements
         
         * Python 3+ or 2.7+
         * Python `numpy` (tested with v1.13.3)
         * [NCBI BLAST+](https://blast.ncbi.nlm.nih.gov/Blast.cgi?CMD=Web&PAGE_TYPE=BlastDocs&DOC_TYPE=Download) (tested with v2.6.0)
@@ -57,22 +62,22 @@
         
         An individual WAAFLE run requires one or two non-fixed inputs: 1) a file containing **metagenomic contigs** and (optionally) 2) a GFF file describing **gene/ORF coordinates** along those contigs.
         
         ### Input contigs (required)
         
         Contigs should be provided as nucleotide sequences in FASTA format. Contigs are expected to have unique, BLAST-compatible headers. WAAFLE is optimized for working with fragmentary contigs from partially assembled metagenomes (spanning 2-20 genes, or roughly 1-20 kb). WAAFLE is not optimized to work with extremely long contigs (100s of kbs), scaffolds, or closed genomes. The WAAFLE developers recommend [MEGAHIT](https://github.com/voutcn/megahit) as a general-purpose metagenomic assembler.
         
-        * [A sample contigs input file](https://bitbucket.org/biobakery/waafle/raw/tip/demo/input/demo_contigs.fna)
+        * [A sample contigs input file](https://github.com/biobakery/waafle/blob/master/demo/input/demo_contigs.fna)
         
         ### Input ORF calls (optional)
         
         2) The optional GFF file, if provided, should conform to the [GFF format]([https://useast.ensembl.org/info/website/upload/gff.html). The WAAFLE developers recommend [Prodigal](https://github.com/hyattpd/Prodigal) as a general-purpose ORF caller with GFF output.
         
-        * [A sample GFF file produced by WAAFLE](https://bitbucket.org/biobakery/waafle/src/default/demo/output/demo_contigs.gff)
-        * [A sample GFF file produced by Prodigal](https://bitbucket.org/biobakery/waafle/src/default/demo/output_prodigal/demo_contigs.gff)
+        * [A sample GFF file produced by WAAFLE](https://github.com/biobakery/waafle/blob/master/demo/output/demo_contigs.gff)
+        * [A sample GFF file produced by Prodigal](https://github.com/biobakery/waafle/blob/master/demo/output_prodigal/demo_contigs.prodigal.gff)
         
         ## Performing a WAAFLE analysis
         
         Analyzing a set of contigs with WAAFLE consistent of three steps, one of which is optional. These three steps are carried out by three independent scripts: `waafle_search`, `waafle_genecaller` (optional), and `waafle_orgscorer`.
         
         ### Step 1 (required): running `waafle_search`
         
@@ -267,10 +272,14 @@
         
         The following properties of the taxonomy file are optional:
         
         * Additional taxa *below* the level of the taxa in the sequence file can be included in the taxonomy file. For example, a species-level sequence database could contain isolate genomes as children of the species-level clades in the taxonomy file. (WAAFLE can use such entries as "leaf support" for LGT events.)
         
         * We recommend prefixing taxonomic clades to indicate their level. For example, `g__Homo` identifies *Homo* as a genus above.
         
+        ## Contributions ##
+        This work was supported by the National Institutes of Health grants U54DE023798 (CH), R24DK110499 (CH), and K23DK125838 (LHN), the American Gastroenterological Association Research Foundation’s Research Scholars Award (LHN), and the Crohn’s and Colitis Foundation Career Development Award (LHN). The content is solely the responsibility of the authors and does not necessarily represent the official views of the NIH. We thank April Pawluk, Kelsey N. Thompson, Kristen Curry, and Todd Treangen for comments on the manuscript and helpful discussions. We also acknowledge Monia Michaud, Casey Dulong, and Yan Yan for their help with validation experiments. Computational work was conducted on the FASRC Cannon cluster supported by the FAS Division of Science Research Computing Group at Harvard University.
+        
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `waafle-0.1.0.dev0/waafle/waafle_orgscorer.py` & `waafle-1.0.0/waafle/waafle_orgscorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 """
 This module is a part of:
 WAAFLE, a [W]orkflow to [A]nnotate [A]ssemblies and [F]ind [L]GT [E]vents
 
-Copyright (c) 2019 Harvard T.H. Chan School of Public Health
+Copyright (c) 2023 Harvard T.H. Chan School of Public Health
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -166,15 +166,15 @@
         metavar="<path>",
         help="directory for writing output files\n[default: .]",
         )
     g.add_argument(
         "--basename",
         default=None,
         metavar="<str>",
-        help="basename for output files\n[default: derived from input]",
+        help="basename for output files\n[default: derived from contigs file]",
         )
     g.add_argument(
         "--write-details",
         action="store_true",
         help="make an additional output file with per-gene clade scores\n[default: off]",
         )
     g.add_argument(
@@ -811,16 +811,14 @@
                 }
             wu.write_rowdict( rowdict, c_formats["details"], details )
 
 def write_main_output_files( contigs, taxonomy, args ):
 
     # open output file handles
     wu.say( "Initializing outputs." )
-    if args.basename is None:
-        args.basename = os.path.split( args.blastout )[1].split( "." )[0]
     handles = {}
     for option in ["lgt", "no_lgt", "unclassified"]:
         file_name = ".".join( [args.basename, option, "tsv"] )
         handles[option] = open( os.path.join( args.outdir, file_name ), "w" )
 
     # determine possible function annotation systems
     systems = set( )
@@ -922,14 +920,18 @@
     for contig_name, loci in wu.iter_contig_loci( args.gff, attach_annotations=False ):
         if contig_name not in contigs:
             wu.say( "  Unknown contig in <gff> file", contig_name )
             continue
         C = contigs[contig_name]
         C.attach_loci( loci )
 
+    # check basename in preparation for writing output
+    if args.basename is None:
+        args.basename = os.path.split( args.contigs )[1].split( "." )[0]
+        
     # prepare details file
     details = None
     if args.write_details:
         details = wu.try_open( os.path.join( 
                 args.outdir, args.basename + ".details.tsv.gz" ), "w" )
         # headers
         wu.write_rowdict( None, c_formats["details"], file=details )
```

### Comparing `waafle-0.1.0.dev0/waafle/waafle_qc.py` & `waafle-1.0.0/waafle/waafle_qc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 """
 This module is a part of:
 WAAFLE, a [W]orkflow to [A]nnotate [A]ssemblies and [F]ind [L]GT [E]vents
 
-Copyright (c) 2019 Harvard T.H. Chan School of Public Health
+Copyright (c) 2023 Harvard T.H. Chan School of Public Health
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `waafle-0.1.0.dev0/waafle/waafle_junctions.py` & `waafle-1.0.0/waafle/waafle_junctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 """
 This module is a part of:
 WAAFLE, a [W]orkflow to [A]nnotate [A]ssemblies and [F]ind [L]GT [E]vents
 
-Copyright (c) 2019 Harvard T.H. Chan School of Public Health
+Copyright (c) 2023 Harvard T.H. Chan School of Public Health
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `waafle-0.1.0.dev0/waafle/utils.py` & `waafle-1.0.0/waafle/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
-"""
+""" 
 This module is a part of:
 WAAFLE, a [W]orkflow to [A]nnotate [A]ssemblies and [F]ind [L]GT [E]vents
 
-Copyright (c) 2019 Harvard T.H. Chan School of Public Health
+Copyright (c) 2023 Harvard T.H. Chan School of Public Health
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `waafle-0.1.0.dev0/waafle/waafle_search.py` & `waafle-1.0.0/waafle/waafle_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 """
 This module is a part of:
 WAAFLE, a [W]orkflow to [A]nnotate [A]ssemblies and [F]ind [L]GT [E]vents
 
-Copyright (c) 2019 Harvard T.H. Chan School of Public Health
+Copyright (c) 2023 Harvard T.H. Chan School of Public Health
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `waafle-0.1.0.dev0/waafle/waafle_genecaller.py` & `waafle-1.0.0/waafle/waafle_genecaller.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 """
 This module is a part of:
 WAAFLE, a [W]orkflow to [A]nnotate [A]ssemblies and [F]ind [L]GT [E]vents
 
-Copyright (c) 2019 Harvard T.H. Chan School of Public Health
+Copyright (c) 2023 Harvard T.H. Chan School of Public Health
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `waafle-0.1.0.dev0/waafle.egg-info/PKG-INFO` & `waafle-1.0.0/waafle.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 Metadata-Version: 2.1
 Name: waafle
-Version: 0.1.0.dev0
-Summary: WAAFLE: a Workflow to Annotate Assemblies and find LGT Events
+Version: 1.0.0
+Summary: WAAFLE: a Workflow to Annotate Assemblies and Find LGT Events
 Home-page: https://huttenhower.sph.harvard.edu/waafle
 Author: Eric Franzosa
 Author-email: franzosa@hsph.harvard.edu
 License: MIT
 Description: # WAAFLE
         
-        **WAAFLE** (a **W**orkflow to **A**nnotate **A**ssemblies and **F**ind **L**GT Events) is a method for finding novel LGT (Lateral Gene Transfer) events in assembled metagenomes, including those from human microbiomes. WAAFLE was developed in the [Huttenhower Lab](http://huttenhower.sph.harvard.edu) at the Harvard T.H. Chan School of Public Health by **Tiffany Hsu** and **Eric A. Franzosa**. Please direct questions to the [WAAFLE user group](waafle-users@googlegroups.com).
+        **WAAFLE** (a **W**orkflow to **A**nnotate **A**ssemblies and **F**ind **L**GT Events) is a method for finding novel LGT (Lateral Gene Transfer) events in assembled metagenomes, including those from human microbiomes.Please direct questions to the [bioBakery Support Forum in WAAFLE category](https://forum.biobakery.org/c/Microbial-community-profiling/WAAFLE).
         
-        [TOC]
         
         ## Citation
+        The WAAFLE manuscript has been submitted!
         
-        |Tiffany Y. Hsu, Eric A. Franzosa, Dennis Wong, Chengwei Luo, Robert G. Beiko, Morgan Langille, Curtis Huttenhower. *The landscape of novel lateral gene transfer events in the human microbiome.* (In prep.)|
-        |-|
+        Tiffany Y. Hsu*, Etienne Nzabarushimana*, Dennis Wong, Chengwei Luo, Robert G. Beiko, Morgan Langille, Curtis Huttenhower, Long H. Nguyen**, Eric A. Franzosa**.
+        
+        <h4> Profiling novel lateral gene transfer events in the human microbiome. (Submitted.) </h4>
+        
+        ```
+        [* = co-lead; ** = co-supervised]
+        ```
+        In the meantime, if you use WAAFLE in your work, please cite the WAAFLE repository on GitHub: https://github.com/biobakery/waafle.
         
-        (*While WAAFLE is not yet published, if you use WAAFLE or the datasets provided below in your work, please cite this website:* http://huttenhower.sph.harvard.edu/waafle.)
         ## Installation
         
         Install the WAAFLE software and Python dependencies with `pip`:
         
         ```
         $ pip install waafle
         ```
         
-        You can also clone the WAAFLE package from bitbucket with mercurial (`hg`):
+        You can also clone the WAAFLE package from Github:
         
         ```
-        $ hg clone https://bitbucket.org/biobakery/waafle
+        $ git clone https://github.com/biobakery/waafle.git
         ```
         
         Or download and inflate WAAFLE package directly:
         
         ```
-        $ wget https://bitbucket.org/biobakery/waafle/get/default.zip
-        $ unzip default.zip
+        $ wget https://github.com/biobakery/waafle/archive/master.zip
+        $ unzip master.zip
         ```
         
         ## Software requirements
         
         * Python 3+ or 2.7+
         * Python `numpy` (tested with v1.13.3)
         * [NCBI BLAST+](https://blast.ncbi.nlm.nih.gov/Blast.cgi?CMD=Web&PAGE_TYPE=BlastDocs&DOC_TYPE=Download) (tested with v2.6.0)
@@ -57,22 +62,22 @@
         
         An individual WAAFLE run requires one or two non-fixed inputs: 1) a file containing **metagenomic contigs** and (optionally) 2) a GFF file describing **gene/ORF coordinates** along those contigs.
         
         ### Input contigs (required)
         
         Contigs should be provided as nucleotide sequences in FASTA format. Contigs are expected to have unique, BLAST-compatible headers. WAAFLE is optimized for working with fragmentary contigs from partially assembled metagenomes (spanning 2-20 genes, or roughly 1-20 kb). WAAFLE is not optimized to work with extremely long contigs (100s of kbs), scaffolds, or closed genomes. The WAAFLE developers recommend [MEGAHIT](https://github.com/voutcn/megahit) as a general-purpose metagenomic assembler.
         
-        * [A sample contigs input file](https://bitbucket.org/biobakery/waafle/raw/tip/demo/input/demo_contigs.fna)
+        * [A sample contigs input file](https://github.com/biobakery/waafle/blob/master/demo/input/demo_contigs.fna)
         
         ### Input ORF calls (optional)
         
         2) The optional GFF file, if provided, should conform to the [GFF format]([https://useast.ensembl.org/info/website/upload/gff.html). The WAAFLE developers recommend [Prodigal](https://github.com/hyattpd/Prodigal) as a general-purpose ORF caller with GFF output.
         
-        * [A sample GFF file produced by WAAFLE](https://bitbucket.org/biobakery/waafle/src/default/demo/output/demo_contigs.gff)
-        * [A sample GFF file produced by Prodigal](https://bitbucket.org/biobakery/waafle/src/default/demo/output_prodigal/demo_contigs.gff)
+        * [A sample GFF file produced by WAAFLE](https://github.com/biobakery/waafle/blob/master/demo/output/demo_contigs.gff)
+        * [A sample GFF file produced by Prodigal](https://github.com/biobakery/waafle/blob/master/demo/output_prodigal/demo_contigs.prodigal.gff)
         
         ## Performing a WAAFLE analysis
         
         Analyzing a set of contigs with WAAFLE consistent of three steps, one of which is optional. These three steps are carried out by three independent scripts: `waafle_search`, `waafle_genecaller` (optional), and `waafle_orgscorer`.
         
         ### Step 1 (required): running `waafle_search`
         
@@ -267,10 +272,14 @@
         
         The following properties of the taxonomy file are optional:
         
         * Additional taxa *below* the level of the taxa in the sequence file can be included in the taxonomy file. For example, a species-level sequence database could contain isolate genomes as children of the species-level clades in the taxonomy file. (WAAFLE can use such entries as "leaf support" for LGT events.)
         
         * We recommend prefixing taxonomic clades to indicate their level. For example, `g__Homo` identifies *Homo* as a genus above.
         
+        ## Contributions ##
+        This work was supported by the National Institutes of Health grants U54DE023798 (CH), R24DK110499 (CH), and K23DK125838 (LHN), the American Gastroenterological Association Research Foundation’s Research Scholars Award (LHN), and the Crohn’s and Colitis Foundation Career Development Award (LHN). The content is solely the responsibility of the authors and does not necessarily represent the official views of the NIH. We thank April Pawluk, Kelsey N. Thompson, Kristen Curry, and Todd Treangen for comments on the manuscript and helpful discussions. We also acknowledge Monia Michaud, Casey Dulong, and Yan Yan for their help with validation experiments. Computational work was conducted on the FASRC Cannon cluster supported by the FAS Division of Science Research Computing Group at Harvard University.
+        
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `waafle-0.1.0.dev0/README.md` & `waafle-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 # WAAFLE
 
-**WAAFLE** (a **W**orkflow to **A**nnotate **A**ssemblies and **F**ind **L**GT Events) is a method for finding novel LGT (Lateral Gene Transfer) events in assembled metagenomes, including those from human microbiomes. WAAFLE was developed in the [Huttenhower Lab](http://huttenhower.sph.harvard.edu) at the Harvard T.H. Chan School of Public Health by **Tiffany Hsu** and **Eric A. Franzosa**. Please direct questions to the [WAAFLE user group](waafle-users@googlegroups.com).
+**WAAFLE** (a **W**orkflow to **A**nnotate **A**ssemblies and **F**ind **L**GT Events) is a method for finding novel LGT (Lateral Gene Transfer) events in assembled metagenomes, including those from human microbiomes.Please direct questions to the [bioBakery Support Forum in WAAFLE category](https://forum.biobakery.org/c/Microbial-community-profiling/WAAFLE).
 
-[TOC]
 
 ## Citation
+The WAAFLE manuscript has been submitted!
 
-|Tiffany Y. Hsu, Eric A. Franzosa, Dennis Wong, Chengwei Luo, Robert G. Beiko, Morgan Langille, Curtis Huttenhower. *The landscape of novel lateral gene transfer events in the human microbiome.* (In prep.)|
-|-|
+Tiffany Y. Hsu*, Etienne Nzabarushimana*, Dennis Wong, Chengwei Luo, Robert G. Beiko, Morgan Langille, Curtis Huttenhower, Long H. Nguyen**, Eric A. Franzosa**.
+
+<h4> Profiling novel lateral gene transfer events in the human microbiome. (Submitted.) </h4>
+
+```
+[* = co-lead; ** = co-supervised]
+```
+In the meantime, if you use WAAFLE in your work, please cite the WAAFLE repository on GitHub: https://github.com/biobakery/waafle.
 
-(*While WAAFLE is not yet published, if you use WAAFLE or the datasets provided below in your work, please cite this website:* http://huttenhower.sph.harvard.edu/waafle.)
 ## Installation
 
 Install the WAAFLE software and Python dependencies with `pip`:
 
 ```
 $ pip install waafle
 ```
 
-You can also clone the WAAFLE package from bitbucket with mercurial (`hg`):
+You can also clone the WAAFLE package from Github:
 
 ```
-$ hg clone https://bitbucket.org/biobakery/waafle
+$ git clone https://github.com/biobakery/waafle.git
 ```
 
 Or download and inflate WAAFLE package directly:
 
 ```
-$ wget https://bitbucket.org/biobakery/waafle/get/default.zip
-$ unzip default.zip
+$ wget https://github.com/biobakery/waafle/archive/master.zip
+$ unzip master.zip
 ```
 
 ## Software requirements
 
 * Python 3+ or 2.7+
 * Python `numpy` (tested with v1.13.3)
 * [NCBI BLAST+](https://blast.ncbi.nlm.nih.gov/Blast.cgi?CMD=Web&PAGE_TYPE=BlastDocs&DOC_TYPE=Download) (tested with v2.6.0)
@@ -49,22 +54,22 @@
 
 An individual WAAFLE run requires one or two non-fixed inputs: 1) a file containing **metagenomic contigs** and (optionally) 2) a GFF file describing **gene/ORF coordinates** along those contigs.
 
 ### Input contigs (required)
 
 Contigs should be provided as nucleotide sequences in FASTA format. Contigs are expected to have unique, BLAST-compatible headers. WAAFLE is optimized for working with fragmentary contigs from partially assembled metagenomes (spanning 2-20 genes, or roughly 1-20 kb). WAAFLE is not optimized to work with extremely long contigs (100s of kbs), scaffolds, or closed genomes. The WAAFLE developers recommend [MEGAHIT](https://github.com/voutcn/megahit) as a general-purpose metagenomic assembler.
 
-* [A sample contigs input file](https://bitbucket.org/biobakery/waafle/raw/tip/demo/input/demo_contigs.fna)
+* [A sample contigs input file](https://github.com/biobakery/waafle/blob/master/demo/input/demo_contigs.fna)
 
 ### Input ORF calls (optional)
 
 2) The optional GFF file, if provided, should conform to the [GFF format]([https://useast.ensembl.org/info/website/upload/gff.html). The WAAFLE developers recommend [Prodigal](https://github.com/hyattpd/Prodigal) as a general-purpose ORF caller with GFF output.
 
-* [A sample GFF file produced by WAAFLE](https://bitbucket.org/biobakery/waafle/src/default/demo/output/demo_contigs.gff)
-* [A sample GFF file produced by Prodigal](https://bitbucket.org/biobakery/waafle/src/default/demo/output_prodigal/demo_contigs.gff)
+* [A sample GFF file produced by WAAFLE](https://github.com/biobakery/waafle/blob/master/demo/output/demo_contigs.gff)
+* [A sample GFF file produced by Prodigal](https://github.com/biobakery/waafle/blob/master/demo/output_prodigal/demo_contigs.prodigal.gff)
 
 ## Performing a WAAFLE analysis
 
 Analyzing a set of contigs with WAAFLE consistent of three steps, one of which is optional. These three steps are carried out by three independent scripts: `waafle_search`, `waafle_genecaller` (optional), and `waafle_orgscorer`.
 
 ### Step 1 (required): running `waafle_search`
 
@@ -258,7 +263,11 @@
 * All taxon names/IDs used in the sequence database must be the same distance from the root.
 
 The following properties of the taxonomy file are optional:
 
 * Additional taxa *below* the level of the taxa in the sequence file can be included in the taxonomy file. For example, a species-level sequence database could contain isolate genomes as children of the species-level clades in the taxonomy file. (WAAFLE can use such entries as "leaf support" for LGT events.)
 
 * We recommend prefixing taxonomic clades to indicate their level. For example, `g__Homo` identifies *Homo* as a genus above.
+
+## Contributions ##
+This work was supported by the National Institutes of Health grants U54DE023798 (CH), R24DK110499 (CH), and K23DK125838 (LHN), the American Gastroenterological Association Research Foundation’s Research Scholars Award (LHN), and the Crohn’s and Colitis Foundation Career Development Award (LHN). The content is solely the responsibility of the authors and does not necessarily represent the official views of the NIH. We thank April Pawluk, Kelsey N. Thompson, Kristen Curry, and Todd Treangen for comments on the manuscript and helpful discussions. We also acknowledge Monia Michaud, Casey Dulong, and Yan Yan for their help with validation experiments. Computational work was conducted on the FASRC Cannon cluster supported by the FAS Division of Science Research Computing Group at Harvard University.
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

