# Comparing `tmp/varvamp-0.9.1.tar.gz` & `tmp/varvamp-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varvamp-0.9.1.tar", last modified: Mon Jul 31 14:23:15 2023, max compression
+gzip compressed data, was "varvamp-0.9.2.tar", last modified: Mon Aug  7 14:12:56 2023, max compression
```

## Comparing `varvamp-0.9.1.tar` & `varvamp-0.9.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:23:15.420872 varvamp-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-31 14:23:15.420872 varvamp-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-31 14:22:55.000000 varvamp-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 14:23:15.420872 varvamp-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-31 14:22:55.000000 varvamp-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:23:15.412872 varvamp-0.9.1/varvamp/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17440 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:23:15.420872 varvamp-0.9.1/varvamp/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/scripts/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/scripts/blast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/scripts/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/scripts/consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)    17960 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/scripts/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/scripts/param_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/scripts/primers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/scripts/qpcr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/scripts/regions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19760 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/scripts/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-07-31 14:22:55.000000 varvamp-0.9.1/varvamp/scripts/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:23:15.416872 varvamp-0.9.1/varvamp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-31 14:23:15.000000 varvamp-0.9.1/varvamp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-31 14:23:15.000000 varvamp-0.9.1/varvamp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 14:23:15.000000 varvamp-0.9.1/varvamp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-31 14:23:15.000000 varvamp-0.9.1/varvamp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 14:23:15.000000 varvamp-0.9.1/varvamp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-31 14:23:15.000000 varvamp-0.9.1/varvamp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 14:23:15.000000 varvamp-0.9.1/varvamp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:12:56.575465 varvamp-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-08-07 14:12:56.575465 varvamp-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-08-07 14:12:38.000000 varvamp-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 14:12:56.575465 varvamp-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-08-07 14:12:38.000000 varvamp-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:12:56.571465 varvamp-0.9.2/varvamp/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-07 14:12:38.000000 varvamp-0.9.2/varvamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-07 14:12:38.000000 varvamp-0.9.2/varvamp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-08-07 14:12:38.000000 varvamp-0.9.2/varvamp/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:12:56.575465 varvamp-0.9.2/varvamp/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 14:12:38.000000 varvamp-0.9.2/varvamp/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-08-07 14:12:38.000000 varvamp-0.9.2/varvamp/scripts/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-08-07 14:12:38.000000 varvamp-0.9.2/varvamp/scripts/blast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-08-07 14:12:38.000000 varvamp-0.9.2/varvamp/scripts/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-08-07 14:12:38.000000 varvamp-0.9.2/varvamp/scripts/consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19557 2023-08-07 14:12:38.000000 varvamp-0.9.2/varvamp/scripts/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-08-07 14:12:38.000000 varvamp-0.9.2/varvamp/scripts/param_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-08-07 14:12:38.000000 varvamp-0.9.2/varvamp/scripts/primers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-08-07 14:12:38.000000 varvamp-0.9.2/varvamp/scripts/qpcr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-08-07 14:12:38.000000 varvamp-0.9.2/varvamp/scripts/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19760 2023-08-07 14:12:38.000000 varvamp-0.9.2/varvamp/scripts/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-08-07 14:12:38.000000 varvamp-0.9.2/varvamp/scripts/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 14:12:56.571465 varvamp-0.9.2/varvamp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-08-07 14:12:56.000000 varvamp-0.9.2/varvamp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-07 14:12:56.000000 varvamp-0.9.2/varvamp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 14:12:56.000000 varvamp-0.9.2/varvamp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-07 14:12:56.000000 varvamp-0.9.2/varvamp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 14:12:56.000000 varvamp-0.9.2/varvamp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-07 14:12:56.000000 varvamp-0.9.2/varvamp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-07 14:12:56.000000 varvamp-0.9.2/varvamp.egg-info/top_level.txt
```

### Comparing `varvamp-0.9.1/PKG-INFO` & `varvamp-0.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varvamp
-Version: 0.9.1
+Version: 0.9.2
 Summary: Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses
 Home-page: https://github.com/jonas-fuchs/varVAMP
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
@@ -45,14 +45,15 @@
 
 # Documentation
 
 * [Installation](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/installation.md)
 * [Preparing the data](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/preparing_the_data.md)
 * [Usage](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/usage.md)
 * [Output](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/output.md)
+* [Wet-lab protocol](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/wet_lab_protocol.md)
 * [How it works](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/how_varvamp_works.md)
 * [FAQ](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/FAQ.md)
 
 ---
 
 **Important disclaimer:**
 *For the primer design, varVAMP uses [primer3](https://pypi.org/project/primer3-py/) to check if digested kmers of a sequence are potential primers. Some of the functions for this were adapted from [primalscheme](www.github.com/aresti/primalscheme) and I do not claim credit.*
```

### Comparing `varvamp-0.9.1/README.md` & `varvamp-0.9.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
 # Documentation
 
 * [Installation](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/installation.md)
 * [Preparing the data](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/preparing_the_data.md)
 * [Usage](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/usage.md)
 * [Output](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/output.md)
+* [Wet-lab protocol](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/wet_lab_protocol.md)
 * [How it works](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/how_varvamp_works.md)
 * [FAQ](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/FAQ.md)
 
 ---
 
 **Important disclaimer:**
 *For the primer design, varVAMP uses [primer3](https://pypi.org/project/primer3-py/) to check if digested kmers of a sequence are potential primers. Some of the functions for this were adapted from [primalscheme](www.github.com/aresti/primalscheme) and I do not claim credit.*
```

### Comparing `varvamp-0.9.1/setup.py` & `varvamp-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.9.1/varvamp/command.py` & `varvamp-0.9.2/varvamp/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 # BUILT-INS
 import sys
 import os
 import datetime
 import argparse
+import multiprocessing
 
 # varVAMP
 from varvamp.scripts import alignment
 from varvamp.scripts import config
 from varvamp.scripts import consensus
 from varvamp.scripts import regions
 from varvamp.scripts import logging
@@ -68,14 +69,30 @@
             "-a",
             "--n-ambig",
             metavar="",
             type=int,
             default=None,
             help="max number of ambiguous characters in a primer"
         )
+        par.add_argument(
+            "-db",
+            "--database",
+            help="location of the BLAST db",
+            metavar="None",
+            type=str,
+            default=None
+        )
+        par.add_argument(
+            "-th",
+            "--n-threads",
+            help="number of threads",
+            metavar="1",
+            type=int,
+            default=1
+        )
     for par in (SANGER_parser, TILED_parser):
         par.add_argument(
             "-ol",
             "--opt-length",
             help="optimal length of the amplicons",
             metavar="1000",
             type=int,
@@ -85,30 +102,14 @@
             "-ml",
             "--max-length",
             help="max length of the amplicons",
             metavar="1500",
             type=int,
             default=1500
         )
-        par.add_argument(
-            "-db",
-            "--database",
-            help="location of the BLAST db",
-            metavar="None",
-            type=str,
-            default=None
-        )
-        par.add_argument(
-            "-th",
-            "--n-threads",
-            help="number of threads for the BLAST search",
-            metavar="1",
-            type=int,
-            default=1
-        )
     TILED_parser.add_argument(
         "-o",
         "--overlap",
         type=int,
         metavar="100",
         default=100,
         help="min overlap of the amplicons"
@@ -169,14 +170,16 @@
     part of the workflow that is shared by all modes
     """
     # start varvamp
     logging.varvamp_progress(log_file, mode=args.mode)
 
     # read in alignment and preprocess
     preprocessed_alignment = alignment.preprocess(args.input[0])
+    # check alignment length distribution
+    logging.check_alignment_length(preprocessed_alignment, log_file)
 
     # estimate threshold or number of ambiguous bases if args were not supplied
     if args.threshold is None or args.n_ambig is None:
         args.threshold, args.n_ambig = param_estimation.get_parameters(preprocessed_alignment, args, log_file)
     if args.mode == "qpcr" and args.n_ambig >= 1 and args.pn_ambig is None:
         args.pn_ambig = args.n_ambig - 1
         with open(log_file, "a") as f:
@@ -193,15 +196,16 @@
         job="Checking config.",
         progress_text="config file passed"
     )
 
     # clean alignment of gaps
     alignment_cleaned, gaps_to_mask = alignment.process_alignment(
         preprocessed_alignment,
-        args.threshold
+        args.threshold,
+        args.n_threads
     )
     logging.varvamp_progress(
         log_file,
         progress=0.2,
         job="Preprocessing alignment and cleaning gaps.",
         progress_text=f"{len(gaps_to_mask)} gaps with {alignment.calculate_total_masked_gaps(gaps_to_mask)} nucleotides"
     )
@@ -302,22 +306,26 @@
         log_file,
         progress=0.8,
         job="Finding potential amplicons.",
         progress_text=f"{len(amplicons)} potential amplicons"
     )
 
     if args.database is not None:
-        amplicons, off_target_amplicons = blast.sanger_or_tiled_blast(
-            all_primers,
+        # create blast query
+        query_path = blast.create_BLAST_query(all_primers, amplicons, data_dir)
+        # perform primer blast
+        amplicons, off_target_amplicons = blast.primer_blast(
             data_dir,
             args.database,
+            query_path,
             amplicons,
             args.max_length,
             args.n_threads,
-            log_file
+            log_file,
+            mode="sanger_tiled"
         )
     else:
         off_target_amplicons = []
 
     return all_primers, amplicons, off_target_amplicons
 
 
@@ -381,15 +389,15 @@
             "\t - increase number of ambiguous nucleotides\n"
             "\t - relax primer settings (not recommended)\n",
             log_file
         )
     return amplicon_scheme
 
 
-def qpcr_workflow(args, alignment_cleaned, ambiguous_consensus, majority_consensus, left_primer_candidates, right_primer_candidates, log_file):
+def qpcr_workflow(args, data_dir, alignment_cleaned, ambiguous_consensus, majority_consensus, left_primer_candidates, right_primer_candidates, log_file):
     """
     part of the workflow specific for the tiled mode
     """
     # find regions for qPCR probes
     probe_regions = regions.find_regions(
         ambiguous_consensus,
         args.pn_ambig
@@ -432,30 +440,46 @@
         )
     logging.varvamp_progress(
         log_file,
         progress=0.8,
         job="Finding unique amplicons with probe.",
         progress_text=f"{len(qpcr_scheme_candidates)} unique amplicons with internal probe"
     )
-
+    # run blast if db is given
+    if args.database is not None:
+        # create blast query
+        query_path = blast.create_BLAST_query_qpcr(qpcr_scheme_candidates, data_dir)
+        # perform primer blast
+        amplicons, off_target_amplicons = blast.primer_blast(
+            data_dir,
+            args.database,
+            query_path,
+            qpcr_scheme_candidates,
+            config.QAMPLICON_LENGTH[1],
+            args.n_threads,
+            log_file,
+            mode="qpcr"
+        )
     # test amplicons for deltaG
-    final_schemes = qpcr.test_amplicon_deltaG(qpcr_scheme_candidates, majority_consensus, args.test_n, args.deltaG)
+    final_schemes = qpcr.test_amplicon_deltaG_parallel(qpcr_scheme_candidates, majority_consensus, args.test_n, args.deltaG, args.n_threads)
     if not final_schemes:
         logging.raise_error(
             "no qPCR amplicon passed the deltaG threshold\n",
             log_file,
             exit=True
         )
+    # report potential blast warnings
+    if args.database is not None:
+        blast.write_BLAST_warning(off_target_amplicons, final_schemes, log_file)
     logging.varvamp_progress(
         log_file,
         progress=0.9,
         job="Filtering amplicons for deltaG.",
         progress_text=f"{len(final_schemes)} non-overlapping qPCR schemes that passed deltaG cutoff"
     )
-
     return probe_regions, final_schemes
 
 
 def main(sysargs=sys.argv[1:]):
     """
     main varvamp workflow
     """
@@ -525,14 +549,15 @@
         )
         reporting.per_base_mismatch_plot(results_dir, amplicon_scheme, args.threshold)
 
     # QPCR mode
     if args.mode == "qpcr":
         probe_regions, final_schemes = qpcr_workflow(
             args,
+            data_dir,
             alignment_cleaned,
             ambiguous_consensus,
             majority_consensus,
             left_primer_candidates,
             right_primer_candidates,
             log_file
         )
```

### Comparing `varvamp-0.9.1/varvamp/scripts/alignment.py` & `varvamp-0.9.2/varvamp/scripts/alignment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 alignment preprocessing
 """
 
 # BUILT-INS
 import re
+import multiprocessing
 
 # varVAMP
 from varvamp.scripts import config
 
 # LIBS
 from Bio import AlignIO
 from Bio.Seq import Seq
@@ -42,38 +43,14 @@
         if "u" in seq:
             seq = seq.back_transcribe()
         preprocessed_alignment.append([sequence[0], str(seq)])
 
     return preprocessed_alignment
 
 
-def find_gaps_in_alignment(alignment):
-    """
-    find all gaps for each sequence in alignment
-    """
-    all_gaps = []
-
-    for seq in alignment:
-        # find all gaps for all sequences with regular expression -{min}
-        all_gaps.append(
-            [(gap.start(0), gap.end(0)-1) for gap in re.finditer(
-                "-{1,}", seq[1])]
-            )
-
-    return all_gaps
-
-
-def find_unique_gaps(all_gaps):
-    """
-    get all unique gaps
-    """
-    result = list(set(gaps for gap_list in all_gaps for gaps in gap_list))
-    return result
-
-
 def find_internal_gaps(unique_gaps, gap):
     """
     find all unique gaps that
     lie within the current gap
     """
     overlapping_gaps = []
 
@@ -93,55 +70,71 @@
                 continue
             if min(intersection) == unique_gap[0] and max(intersection)+1 == unique_gap[1]:
                 overlapping_gaps.append(unique_gap)
 
     return overlapping_gaps
 
 
-def create_gap_dictionary(unique_gaps, all_gaps):
+def find_overlapping_gaps_worker(gap_list, unique_gaps):
     """
-    creates a dictionary with gap counts.
-    counts also all overlapping gaps per gap.
+    Worker function to find overlapping gaps and count their occurrences.
     """
+    gap_dict_part = {}
+    for gap in gap_list:
+        overlapping_gaps = find_internal_gaps(unique_gaps, gap)
+        for overlapping_gap in overlapping_gaps:
+            if overlapping_gap in gap_dict_part:
+                gap_dict_part[overlapping_gap] += 1
+            else:
+                gap_dict_part[overlapping_gap] = 1
+    return gap_dict_part
 
-    gap_dict = {}
 
-    for gap_list in all_gaps:
-        for gap in gap_list:
-            overlapping_gaps = find_internal_gaps(unique_gaps, gap)
-            for overlapping_gap in overlapping_gaps:
-                if overlapping_gap in gap_dict:
-                    gap_dict[overlapping_gap] += 1
-                else:
-                    gap_dict[overlapping_gap] = 1
+def create_gap_dictionary(unique_gaps, all_gaps, n_threads):
+    """
+    Creates a dictionary with all gap counts.
+    Counts also all overlapping gaps per gap.
+    Uses multiprocessing for parallelization.
+    """
+
+    with multiprocessing.Pool(processes=n_threads) as pool:
+        results = pool.starmap(find_overlapping_gaps_worker, [(gap_list, unique_gaps) for gap_list in all_gaps])
+
+    gap_dict = {}
+    for gap_dict_part in results:
+        for gap, count in gap_dict_part.items():
+            if gap in gap_dict:
+                gap_dict[gap] += count
+            else:
+                gap_dict[gap] = count
 
     return gap_dict
 
 
+
 def find_gaps_to_mask(gap_dict, cutoff):
     """
     filters gaps for their freq cutoff.
     condenses final gaps if there is
     an overlap.
     """
     gaps_to_mask = []
     potential_gaps = []
+    opened_region = []
 
     # check for each region if it is covered
     # by enough sequences
     for gap in gap_dict:
         if gap_dict[gap] > cutoff:
             potential_gaps.append(gap)
 
     # sort by start and stop
     potential_gaps = sorted(potential_gaps)
 
     # get the min and max of overlapping gaps
-    opened_region = []
-    gaps_to_mask = []
     for i, region in enumerate(potential_gaps):
         region = list(region)
         if opened_region:
             # write the opened region if the start of the current region
             # > opened_region[stop] and the last still opened region
             if region[0] > opened_region[1] or i == len(potential_gaps)-1:
                 gaps_to_mask.append(opened_region)
@@ -199,25 +192,31 @@
             masked_seq = masked_seq + mask
 
         cleaned_alignment.append([sequence[0], masked_seq])
 
     return cleaned_alignment
 
 
-def process_alignment(preprocessed_alignment, threshold):
+def process_alignment(preprocessed_alignment, threshold, n_threads):
     """
     proprocesses alignment and cleans gaps
     """
-    gap_cutoff = len(preprocessed_alignment)*(1-threshold)
+    all_gaps = []
 
-    all_gaps = find_gaps_in_alignment(preprocessed_alignment)
-    unique_gaps = find_unique_gaps(all_gaps)
+    gap_cutoff = len(preprocessed_alignment)*(1-threshold)
+    for seq in preprocessed_alignment:
+        # find all gaps for all sequences with regular expression -{min}
+        all_gaps.append(
+            [(gap.start(0), gap.end(0) - 1) for gap in re.finditer(
+                "-{1,}", seq[1])]
+        )
+    unique_gaps = list(set(gaps for gap_list in all_gaps for gaps in gap_list))
 
     if unique_gaps:
-        gap_dic = create_gap_dictionary(unique_gaps, all_gaps)
+        gap_dic = create_gap_dictionary(unique_gaps, all_gaps, n_threads)
         gaps_to_mask = find_gaps_to_mask(gap_dic, gap_cutoff)
         if gaps_to_mask:
             alignment_cleaned = clean_gaps(
                 preprocessed_alignment, gaps_to_mask
             )
         else:
             alignment_cleaned = preprocessed_alignment
```

### Comparing `varvamp-0.9.1/varvamp/scripts/blast.py` & `varvamp-0.9.2/varvamp/scripts/blast.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 BLAST feature of varVAMP. Checks primers of potential amplicons for hits
 against a db and evals if hits are in proximity to potentially
 produce off-target amplicons.
 """
 
 # BUILT-INS
 import os
+import itertools
+import multiprocessing
 from shutil import which
 
 #LIBS
 import pandas as pd
 from Bio.Blast.Applications import NcbiblastnCommandline
 
 # varVAMP
@@ -23,27 +25,52 @@
     """
     if which("blastn") is not None:
         print("\nINFO: BLASTN is installed.")
     else:
         logging.raise_error("BLASTN is not installed", log_file, exit=True)
 
 
-def create_BLAST_query(all_primers, data_dir):
+def create_BLAST_query(all_primers, amplicons, data_dir):
     """
-    create a query for the BLAST search
+    create a query for the BLAST search (tiled, sanger mode)
     """
+    already_written = []
+
     query_path = os.path.join(data_dir, "BLAST_query.fasta")
     with open(query_path, "w") as query:
-        for strand in all_primers:
-            for primer in all_primers[strand]:
-                print(f">{primer}\n{all_primers[strand][primer][0]}", file=query)
+        for amp in amplicons:
+            fw_primer, rw_primer = amplicons[amp][2], amplicons[amp][3]
+            if fw_primer not in already_written:
+                print(f">{fw_primer}\n{all_primers['+'][fw_primer][0]}", file=query)
+                already_written.append(fw_primer)
+            if rw_primer not in already_written:
+                print(f">{rw_primer}\n{all_primers['-'][rw_primer][0]}", file=query)
+                already_written.append(rw_primer)
 
     return query_path
 
 
+def create_BLAST_query_qpcr(qpcr_scheme_candidates, data_dir):
+    """
+    create a query for the BLAST search (qpcr mode)
+    """
+    already_written = []
+
+    query_path = os.path.join(data_dir, "BLAST_query.fasta")
+    with open(query_path, "w") as query:
+        for amp in qpcr_scheme_candidates:
+            for primer_type in ["probe", "left", "right"]:
+                name = f"{primer_type}_{qpcr_scheme_candidates[amp][primer_type][1]}_{qpcr_scheme_candidates[amp][primer_type][2]}"
+                if name in already_written:
+                    continue
+                print(f">{name}\n{qpcr_scheme_candidates[amp][primer_type][0]}", file=query)
+                already_written.append(name)
+    return query_path
+
+
 def run_BLAST(query, blast_db, data_dir, n_threads):
     """
     runs a BLAST search on a search query.
     """
     basename = os.path.basename(os.path.normpath(query))
     blast_out = os.path.join(data_dir, f"{basename.strip('.fasta')}_result.tabular")
 
@@ -86,86 +113,124 @@
         ]
     # removes tabular output
     os.remove(blast_out)
 
     return(blast_df)
 
 
-def predict_non_specific_amplicons(amplicons, blast_df, max_length):
+def check_off_targets(df_amp_primers_sorted, max_length, primers):
     """
-    for a given primer pair, predict unspecific targets within a size
-    range and give these primers a high penalty.
+    determines off targets in subset blast df
     """
-    off_target_amp = []
+    combinations = list(itertools.combinations(primers, 2))
 
-    for amp in amplicons:
-        fw_primer = amplicons[amp][2]
-        rw_primer = amplicons[amp][3]
-        # subset df for primers
-        df_amp_primers = blast_df[blast_df["query"].isin([fw_primer, rw_primer])]
-        # sort by reference and ref start
-        df_amp_primers_sorted = df_amp_primers.sort_values(["ref", "ref_start"])
-        # iterate over ref for each primer pair
-        for ref in set(df_amp_primers_sorted["ref"]):
-            df_ref_subset = df_amp_primers_sorted[df_amp_primers_sorted["ref"] == ref]
-            # reindex to remember the correct index later on
-            df_ref_subset.reset_index(inplace=True, drop=True)
-            # ini the primer search
-            indices = []  # remember the index of the subset df
-            start = -float("inf")
-            off_target = False
-            for row in df_ref_subset.itertuples():
-                # for the current row check if start of the current batch is close enough
-                if row[8] - start <= config.BLAST_SIZE_MULTI * max_length:
-                    indices.append(row[0])
+    for ref in set(df_amp_primers_sorted["ref"]):
+        df_ref_subset = df_amp_primers_sorted[df_amp_primers_sorted["ref"] == ref]
+        # reindex to remember the correct index later on
+        df_ref_subset.reset_index(inplace=True, drop=True)
+        # ini the primer search
+        indices = []  # remember the index of the subset df
+        start = -float("inf")
+        for row in df_ref_subset.itertuples():
+            # for the current row check if start of the current batch is close enough
+            if row[8] - start <= config.BLAST_SIZE_MULTI * max_length:
+                indices.append(row[0])
+            else:
+                # reset start to the next element in the index list if list has more than
+                # one element
+                if len(indices) > 1:
+                    indices.pop(0)
+                    start = df_ref_subset.iloc[indices[0]]["ref_start"]
+                # else reset to the current row and empty index list
                 else:
-                    # reset start to the next element in the index list if list has more than
-                    # one element
-                    if len(indices) > 1:
-                        indices.pop(0)
-                        start = df_ref_subset.iloc[indices[0]]["ref_start"]
-                    # else reset to the current row and empty index list
-                    else:
-                        start = row[7]
-                        indices = []
-                # check if in the df subset is more than one primer
-                if len(set(df_ref_subset.iloc[indices]["query"])) <= 1:
-                    continue
-                # subset of df with potential off-targets
-                possible_off_targets = df_ref_subset.iloc[indices]
-                # check if fw and rw primers bind in different directions
-                direction_fw = set(possible_off_targets[possible_off_targets["query"] == fw_primer]["strand"])
-                direction_rw = set(possible_off_targets[possible_off_targets["query"] == rw_primer]["strand"])
+                    start = row[7]
+                    indices = []
+            # check if in the df subset is more than one primer
+            if len(set(df_ref_subset.iloc[indices]["query"])) <= 1:
+                continue
+            # subset of df with potential off-targets
+            possible_off_targets = df_ref_subset.iloc[indices]
+            # check if any two primers in scheme bind different directions
+            for combi in combinations:
+                direction_fw = set(possible_off_targets[possible_off_targets["query"] == combi[0]]["strand"])
+                direction_rw = set(possible_off_targets[possible_off_targets["query"] == combi[1]]["strand"])
                 # do we have one primer in subset that binds both directions or are the
                 # direction sets different? --> 2 different primers bind on the same chrom,
                 # are close enough and are in opposite direction ->[seq]<-
                 # >this classifies as an off-target<
                 if len(direction_fw) > 1 or len(direction_rw) > 1 or direction_fw != direction_rw:
-                    off_target = True
-                    break
-            if off_target:
-                amplicons[amp][5] = amplicons[amp][5] + config.BLAST_PENALTY
-                off_target_amp.append(amp)
-                break
+                    return True
+    return False
+
+
+def predict_non_specific_amplicons_worker(amp, blast_df, max_length, mode):
+    """
+    Worker function to predict unspecific targets for a single amplicon.
+    """
+    name, data = amp
+    # get correct primers
+    if mode == "sanger_tiled":
+        primers = [data[2], data[3]]
+    elif mode == "qpcr":
+        primers = []
+        for primer_type in ["probe", "left", "right"]:
+            primers.append(f"{primer_type}_{data[primer_type][1]}_{data[primer_type][2]}")
+    # subset df for primers
+    df_amp_primers = blast_df[blast_df["query"].isin(primers)]
+    # sort by reference and ref start
+    df_amp_primers_sorted = df_amp_primers.sort_values(["ref", "ref_start"])
+    # check for off-targets for specific primers
+    if check_off_targets(df_amp_primers_sorted, max_length, primers):
+        return name
+
+
+def predict_non_specific_amplicons(amplicons, blast_df, max_length, mode, n_threads):
+    """
+    Main function to predict unspecific targets within a size range and give
+    these primers a high penalty. Uses multiprocessing for parallelization.
+    """
+    off_targets = []
+    # process amplicons concurrently
+    with multiprocessing.Pool(processes=n_threads) as pool:
+        amp_items = amplicons.items()
+        results = pool.starmap(predict_non_specific_amplicons_worker, [(amp, blast_df, max_length, mode) for amp in amp_items])
+    # check results
+    for off_target in results:
+        if off_target is None:
+            continue
+        off_targets.append(off_target)
+        if mode == "sanger_tiled":
+            amplicons[off_target][5] = amplicons[off_target][5] + config.BLAST_PENALTY
+        elif mode == "qpcr":
+            amplicons[off_target]["score"][0] = amplicons[off_target]["score"][0] + config.BLAST_PENALTY
 
-    return(off_target_amp, amplicons)
+    return off_targets, amplicons
 
 
-def sanger_or_tiled_blast(all_primers, data_dir, db, amplicons, max_length, n_threads, log_file):
+def primer_blast(data_dir, db, query_path, amplicons, max_length, n_threads, log_file, mode):
     """
     performs the blast search for the sanger or tiled workflow
     """
     print("\n#### Starting varVAMP primerBLAST. ####\n")
-    print("Job_1: Creating BLAST query.")
-    query_path = create_BLAST_query(all_primers, data_dir)
-    print("Job_2: Running BLAST.")
-    blast_out = run_BLAST(query_path, db, data_dir, n_threads)
+    print("Running BLASTN...")
+    blast_out = run_BLAST(
+        query_path,
+        db,
+        data_dir,
+        n_threads
+    )
     blast_df = parse_and_filter_BLAST_output(blast_out)
-    print("Job_3: Predicting non-specific amplicons.")
-    off_target_amplicons, amplicons = predict_non_specific_amplicons(amplicons, blast_df, max_length)
+    print("Predicting non-specific amplicons...")
+    off_target_amplicons, amplicons = predict_non_specific_amplicons(
+        amplicons,
+        blast_df,
+        max_length,
+        mode,
+        n_threads
+    )
     success_text = f"varVAMP successfully predicted non-specific amplicons:\n\t> {len(off_target_amplicons)}/{len(amplicons)} amplicons could produce amplicons with the blast db.\n\t> raised their amplicon score by {config.BLAST_PENALTY}"
     print(success_text)
     with open(log_file, 'a') as f:
         print(
             f"\nBLAST results: {success_text}",
             file=f
         )
```

### Comparing `varvamp-0.9.1/varvamp/scripts/config.py` & `varvamp-0.9.2/varvamp/scripts/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     "outfmt": "6 qseqid sseqid qlen length mismatch gapopen sstart send sstrand",  # do NOT change
     "evalue": 5000,
     "reward": 1,
     "penalty": -1,
     "gapopen": 2,
     "gapextend": 1
 }
-BLAST_MAX_DIFF = 0.7  # allowed % differences between primer and BLAST hit
+BLAST_MAX_DIFF = 0.5  # min percent match between primer and BLAST hit (coverage and/or mismatches)
 BLAST_SIZE_MULTI = 2  # multiplier for the max_amp size of off targets (in relation to max amp size)
 BLAST_PENALTY = 50  # amplicon score increase -> considered only if no other possibilities
 
 # nucleotide definitions, do NOT change
 NUCS = set("atcg")
 AMBIG_NUCS = {
     "r": ["a", "g"],
```

### Comparing `varvamp-0.9.1/varvamp/scripts/consensus.py` & `varvamp-0.9.2/varvamp/scripts/consensus.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.9.1/varvamp/scripts/logging.py` & `varvamp-0.9.2/varvamp/scripts/logging.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 # BUILT-INS
 import sys
 import os
 import shutil
 import datetime
 import random
+import statistics
 
 # varVAMP
 from varvamp.scripts import config
 from varvamp import __version__
 
 
 def create_dir_structure(dir):
@@ -100,34 +101,34 @@
         )
     if args.n_ambig > 4:
         raise_error(
             "high number of ambiguous nucleotides in primer leads to a high "
             "degeneracy. Consider reducing.",
             log_file
         )
+    if args.database is not None:
+        if args.n_threads < 1:
+            raise_error(
+                "number of threads cannot be smaller than 1.",
+                log_file,
+                exit=True
+            )
     if args.mode in ("tiled", "sanger"):
         if args.opt_length > args.max_length:
             raise_error(
                 "optimal length can not be higher than the maximum amplicon length.",
                 log_file,
                 exit=True
             )
         if args.opt_length < 0 or args.max_length < 0:
             raise_error(
                 "amplicon lengths can not be negative.",
                 log_file,
                 exit=True
             )
-        if args.database is not None:
-            if args.n_threads < 1:
-                raise_error(
-                    "number of threads cannot be smaller than 1.",
-                    log_file,
-                    exit=True
-                )
     # SANGER specific warnings
     if args.mode == "sanger":
         if args.report_n < 1:
             raise_error(
                 "number of reported amplicons cannot be below 1.",
                 log_file,
                 exit=True
@@ -201,14 +202,49 @@
         if args.deltaG > 0:
             raise_error(
                 "setting the deltaG cutoff larger than 0 is not recommended!",
                 log_file
             )
 
 
+def check_alignment_length(preprocessed_alignment, log_file):
+    """
+    checks the sequence lengths of the alignment and reports a warning
+    if the length is larger or smaller than the mean +- 3std of all seqs
+    and at least 1 % diff to mean
+    """
+
+    all_seq_length, all_names = [], []
+    # count the length
+    for seq in preprocessed_alignment:
+        all_names.append(seq[0])
+        all_seq_length.append(len(seq[1].strip("-")))
+    # clac mean and std
+    mean_len, mean_std = statistics.mean(all_seq_length), statistics.stdev(all_seq_length)
+    # check for each seq if it is larger or smaller than the mean +-3std
+    # and is at least 1 % smaller or larger than the alignment mean
+    # (otherwise varvamp will report very small differences).
+    smaller_warning, larger_warning = [], []
+    for name, length in zip(all_names, all_seq_length):
+        if length <= mean_len-3*mean_std and length <= mean_len-mean_len*0.01:
+            smaller_warning.append(f"{name} ({length} nt)\n")
+        elif length >= mean_len+3*mean_std and length >= mean_len+mean_len*0.01:
+            larger_warning.append(f"{name} ({length} nt)\n")
+    # raise warning for non-empty lists
+    for warning, length_type in zip([larger_warning, smaller_warning], ["larger", "smaller"]):
+        if not warning:
+            continue
+        warning = "".join(warning)
+        raise_error(
+            f"The following sequences are considerably {length_type} than the alignment mean ({round(mean_len)} nt) and might cause signigicant trimming:\n{warning}",
+            log_file,
+            exit=False
+        )
+
+
 def confirm_config(args, log_file):
     """
     checks the config. raises error and warnings
     if nececarry. writes settings to log
     """
     error = False
```

### Comparing `varvamp-0.9.1/varvamp/scripts/param_estimation.py` & `varvamp-0.9.2/varvamp/scripts/param_estimation.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.9.1/varvamp/scripts/primers.py` & `varvamp-0.9.2/varvamp/scripts/primers.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.9.1/varvamp/scripts/qpcr.py` & `varvamp-0.9.2/varvamp/scripts/qpcr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 qPCR probe and amplicon design
 """
 
 # LIBS
 import seqfold
+import itertools
+import multiprocessing
 
 # varVAMP
 from varvamp.scripts import config
 from varvamp.scripts import primers
 
 def choose_probe_direction(seq):
     """
@@ -234,54 +236,61 @@
         }
     # and again sort by total score (left + right + probe)
     qpcr_scheme_candidates = dict(sorted(qpcr_scheme_candidates.items(), key=lambda x: x[1]["score"]))
 
     return qpcr_scheme_candidates
 
 
-def test_amplicon_deltaG(qpcr_schemes_candiadates, majority_consensus, n_to_test, deltaG_cutoff):
+def process_single_amplicon_deltaG(amplicon, majority_consensus):
     """
-    test all amplicon deltaGsfor the top n hits  at the lowest primer temperature
-    and filters if they fall below the cutoff. relies in seqfold. only consider
-    non-overlapping amplicons.
-
-    NOTE: this is computationally intensive. Therefore, it is not advisable to
-    test all hits for their deltaG.
+    Process a single amplicon to test its deltaG and apply filtering.
+    This function will be called concurrently by multiple threads.
+    """
+    name, data = amplicon
+    start = data["left"][1]
+    stop = data["right"][2]
+    seq = majority_consensus[start:stop]
+    seq = seq.replace("N", "")
+    seq = seq.replace("n", "")
+    amp_positions = list(range(start, stop + 1))
+    # check if the amplicon overlaps with an amplicon that was previously
+    # found and had a high enough deltaG
+    min_temp = min((primers.calc_temp(data["left"][0]),
+                    primers.calc_temp(data["right"][0])))
+    # calculate deltaG at the minimal primer temp
+    deltaG = seqfold.dg(seq, min_temp)
+
+    return deltaG, amp_positions, name
+
+
+def test_amplicon_deltaG_parallel(qpcr_schemes_candidates, majority_consensus, n_to_test, deltaG_cutoff, n_threads):
+    """
+    Test all amplicon deltaGs for the top n hits at the lowest primer temperature
+    and filters if they fall below the cutoff. Multiple processes are used
+    for processing amplicons in parallel.
     """
-
     final_schemes = {}
-    n = 0
-    passed_counter = 0
+    passed_counter = 0  # counter for re-naming amplicons that passed deltaG cutoff
     amplicon_set = set()
 
-    for amp in qpcr_schemes_candiadates:
-        start = qpcr_schemes_candiadates[amp]["left"][1]
-        stop = qpcr_schemes_candiadates[amp]["right"][2]
-        seq = majority_consensus[start:stop]
-        # delta G cannot be calculated if non-atcg chars are in the sequence, so
-        # delete any single Ns (small deletions) or ns (ambiguties) from seq
-        seq = seq.replace("N", "")
-        seq = seq.replace("n", "")
-        amp_positions = list(range(start, stop+1))
-        # check if the amplicon overlaps with an amplicon that was previously
-        # found and had a high enough deltaG
-        if any(x in amp_positions for x in amplicon_set):
-            continue
-        # did we check enough amplicons?
-        if n < n_to_test:
-            min_temp = min((primers.calc_temp(qpcr_schemes_candiadates[amp]["left"][0]), primers.calc_temp(qpcr_schemes_candiadates[amp]["right"][0])))
-            # calculate deltaG at the minimal primer temp
-            deltaG = seqfold.dg(seq, min_temp)
+    # Create a pool of processes to handle the concurrent processing
+    with multiprocessing.Pool(processes=n_threads) as pool:
+        # Create a list of the first n amplicon tuples for processing
+        amplicons = itertools.islice(qpcr_schemes_candidates.items(), n_to_test)
+        # process amplicons concurrently
+        results = pool.starmap(process_single_amplicon_deltaG, [(amp, majority_consensus) for amp in amplicons])
+        # Process the results
+        for deltaG, amp_positions, amp_name in results:
+            # check if the amplicon overlaps with an amplicon that was previously
+            # found and had a high enough deltaG
+            if any(x in amp_positions for x in amplicon_set):
+                continue
             # and if this passes cutoff make a dict entry and do not allow further
             # amplicons in that region (they will have a lower score)
             if deltaG > deltaG_cutoff:
                 new_name = f"QPCR_SCHEME_{passed_counter}"
-                final_schemes[new_name] = qpcr_schemes_candiadates[amp]
+                final_schemes[new_name] = qpcr_schemes_candidates[amp_name]
                 final_schemes[new_name]["deltaG"] = deltaG
                 amplicon_set.update(amp_positions)
                 passed_counter += 1
-            n += 1
-        # break if enough amplicons were checked
-        else:
-            break
 
     return final_schemes
```

### Comparing `varvamp-0.9.1/varvamp/scripts/regions.py` & `varvamp-0.9.2/varvamp/scripts/regions.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.9.1/varvamp/scripts/reporting.py` & `varvamp-0.9.2/varvamp/scripts/reporting.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.9.1/varvamp/scripts/scheme.py` & `varvamp-0.9.2/varvamp/scripts/scheme.py`

 * *Files identical despite different names*

### Comparing `varvamp-0.9.1/varvamp.egg-info/PKG-INFO` & `varvamp-0.9.2/varvamp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varvamp
-Version: 0.9.1
+Version: 0.9.2
 Summary: Variable VirusAMPlicons (varVAMP) is a tool to design primers for highly diverse viruses
 Home-page: https://github.com/jonas-fuchs/varVAMP
 Author: Dr. Jonas Fuchs
 Author-email: jonas.fuchs@uniklinik-freiburg.de
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.9
@@ -45,14 +45,15 @@
 
 # Documentation
 
 * [Installation](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/installation.md)
 * [Preparing the data](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/preparing_the_data.md)
 * [Usage](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/usage.md)
 * [Output](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/output.md)
+* [Wet-lab protocol](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/wet_lab_protocol.md)
 * [How it works](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/how_varvamp_works.md)
 * [FAQ](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/FAQ.md)
 
 ---
 
 **Important disclaimer:**
 *For the primer design, varVAMP uses [primer3](https://pypi.org/project/primer3-py/) to check if digested kmers of a sequence are potential primers. Some of the functions for this were adapted from [primalscheme](www.github.com/aresti/primalscheme) and I do not claim credit.*
```

### Comparing `varvamp-0.9.1/varvamp.egg-info/SOURCES.txt` & `varvamp-0.9.2/varvamp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

