# Comparing `tmp/booze-tools-0.6.1.0.tar.gz` & `tmp/booze-tools-0.6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "booze-tools-0.6.1.0.tar", last modified: Sun Oct 30 03:16:16 2022, max compression
+gzip compressed data, was "booze-tools-0.6.2.0.tar", last modified: Mon Aug  7 06:44:43 2023, max compression
```

## Comparing `booze-tools-0.6.1.0.tar` & `booze-tools-0.6.2.0.tar`

### file list

```diff
@@ -1,54 +1,68 @@
-drwxrwxrwx   0        0        0        0 2022-10-30 03:16:16.173141 booze-tools-0.6.1.0/
--rw-rw-rw-   0        0        0     1089 2021-09-06 01:47:53.000000 booze-tools-0.6.1.0/LICENSE
--rw-rw-rw-   0        0        0     5133 2022-10-30 03:16:16.173141 booze-tools-0.6.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4530 2022-10-16 04:57:46.000000 booze-tools-0.6.1.0/README.md
-drwxrwxrwx   0        0        0        0 2022-10-30 03:16:16.041531 booze-tools-0.6.1.0/booze_tools.egg-info/
--rw-rw-rw-   0        0        0     5133 2022-10-30 03:16:15.000000 booze-tools-0.6.1.0/booze_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1340 2022-10-30 03:16:15.000000 booze-tools-0.6.1.0/booze_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-30 03:16:15.000000 booze-tools-0.6.1.0/booze_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-10-30 03:16:15.000000 booze-tools-0.6.1.0/booze_tools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-10-30 03:16:16.057157 booze-tools-0.6.1.0/boozetools/
--rw-rw-rw-   0        0        0        0 2021-09-06 01:47:53.000000 booze-tools-0.6.1.0/boozetools/__init__.py
--rw-rw-rw-   0        0        0     3200 2022-10-12 02:28:06.000000 booze-tools-0.6.1.0/boozetools/__main__.py
-drwxrwxrwx   0        0        0        0 2022-10-30 03:16:16.082114 booze-tools-0.6.1.0/boozetools/macroparse/
--rw-rw-rw-   0        0        0        0 2021-09-06 01:47:53.000000 booze-tools-0.6.1.0/boozetools/macroparse/__init__.py
--rw-rw-rw-   0        0        0    19641 2022-09-02 06:26:53.000000 booze-tools-0.6.1.0/boozetools/macroparse/compaction.py
--rw-rw-rw-   0        0        0    12388 2022-10-09 09:47:18.000000 booze-tools-0.6.1.0/boozetools/macroparse/compiler.py
--rw-rw-rw-   0        0        0     8690 2022-10-09 00:56:43.000000 booze-tools-0.6.1.0/boozetools/macroparse/expansion.py
--rw-rw-rw-   0        0        0    18321 2022-10-12 02:21:54.000000 booze-tools-0.6.1.0/boozetools/macroparse/grammar.py
--rw-rw-rw-   0        0        0      263 2022-10-09 00:56:43.000000 booze-tools-0.6.1.0/boozetools/macroparse/interface.py
--rw-rw-rw-   0        0        0     7822 2022-10-29 19:48:14.000000 booze-tools-0.6.1.0/boozetools/macroparse/runtime.py
--rw-rw-rw-   0        0        0    14239 2022-09-02 06:26:53.000000 booze-tools-0.6.1.0/boozetools/menagerie.py
-drwxrwxrwx   0        0        0        0 2022-10-30 03:16:16.122733 booze-tools-0.6.1.0/boozetools/parsing/
--rw-rw-rw-   0        0        0        0 2021-09-06 01:47:53.000000 booze-tools-0.6.1.0/boozetools/parsing/__init__.py
--rw-rw-rw-   0        0        0      191 2022-09-02 06:57:12.000000 booze-tools-0.6.1.0/boozetools/parsing/all_methods.py
--rw-rw-rw-   0        0        0    19975 2022-10-09 09:41:28.000000 booze-tools-0.6.1.0/boozetools/parsing/automata.py
--rw-rw-rw-   0        0        0    20020 2022-08-24 02:31:39.000000 booze-tools-0.6.1.0/boozetools/parsing/context_free.py
-drwxrwxrwx   0        0        0        0 2022-10-30 03:16:16.122733 booze-tools-0.6.1.0/boozetools/parsing/general/
--rw-rw-rw-   0        0        0        0 2021-09-06 01:47:53.000000 booze-tools-0.6.1.0/boozetools/parsing/general/__init__.py
--rw-rw-rw-   0        0        0     3875 2022-09-03 18:53:40.000000 booze-tools-0.6.1.0/boozetools/parsing/general/brute_force.py
--rw-rw-rw-   0        0        0     6018 2022-09-02 20:18:33.000000 booze-tools-0.6.1.0/boozetools/parsing/general/gss.py
--rw-rw-rw-   0        0        0     5684 2022-10-29 19:38:36.000000 booze-tools-0.6.1.0/boozetools/parsing/interface.py
--rw-rw-rw-   0        0        0     8889 2022-09-04 01:15:57.000000 booze-tools-0.6.1.0/boozetools/parsing/lalr.py
--rw-rw-rw-   0        0        0     3780 2022-08-15 04:08:38.000000 booze-tools-0.6.1.0/boozetools/parsing/lr0.py
--rw-rw-rw-   0        0        0    13063 2022-09-04 00:20:05.000000 booze-tools-0.6.1.0/boozetools/parsing/lr1.py
--rw-rw-rw-   0        0        0     4828 2022-10-09 09:41:28.000000 booze-tools-0.6.1.0/boozetools/parsing/miniparse.py
--rw-rw-rw-   0        0        0    15293 2022-10-09 09:16:27.000000 booze-tools-0.6.1.0/boozetools/parsing/shift_reduce.py
-drwxrwxrwx   0        0        0        0 2022-10-30 03:16:16.157520 booze-tools-0.6.1.0/boozetools/scanning/
--rw-rw-rw-   0        0        0        0 2021-09-06 01:47:53.000000 booze-tools-0.6.1.0/boozetools/scanning/__init__.py
--rw-rw-rw-   0        0        0     1611 2022-09-01 05:08:45.000000 booze-tools-0.6.1.0/boozetools/scanning/charclass.py
--rw-rw-rw-   0        0        0     6217 2022-09-02 22:19:32.000000 booze-tools-0.6.1.0/boozetools/scanning/charset.py
--rw-rw-rw-   0        0        0     4476 2022-10-08 23:33:20.000000 booze-tools-0.6.1.0/boozetools/scanning/engine.py
--rw-rw-rw-   0        0        0     7571 2022-09-01 05:47:11.000000 booze-tools-0.6.1.0/boozetools/scanning/finite.py
--rw-rw-rw-   0        0        0     2996 2022-09-02 20:25:18.000000 booze-tools-0.6.1.0/boozetools/scanning/interface.py
--rw-rw-rw-   0        0        0     4534 2022-09-04 01:32:37.000000 booze-tools-0.6.1.0/boozetools/scanning/miniscan.py
--rw-rw-rw-   0        0        0    22191 2022-09-04 01:52:37.000000 booze-tools-0.6.1.0/boozetools/scanning/regular.py
-drwxrwxrwx   0        0        0        0 2022-10-30 03:16:16.173141 booze-tools-0.6.1.0/boozetools/support/
--rw-rw-rw-   0        0        0        0 2021-09-06 01:47:53.000000 booze-tools-0.6.1.0/boozetools/support/__init__.py
--rw-rw-rw-   0        0        0     6636 2022-10-29 18:24:32.000000 booze-tools-0.6.1.0/boozetools/support/failureprone.py
--rw-rw-rw-   0        0        0     9164 2022-08-10 07:51:09.000000 booze-tools-0.6.1.0/boozetools/support/foundation.py
--rw-rw-rw-   0        0        0     1318 2022-08-14 04:36:14.000000 booze-tools-0.6.1.0/boozetools/support/pretty.py
--rw-rw-rw-   0        0        0     5762 2022-08-21 22:41:21.000000 booze-tools-0.6.1.0/boozetools/support/symtab.py
--rw-rw-rw-   0        0        0     7119 2022-09-04 02:17:04.000000 booze-tools-0.6.1.0/boozetools/support/treelang.py
--rw-rw-rw-   0        0        0       42 2022-10-30 03:16:16.173141 booze-tools-0.6.1.0/setup.cfg
--rw-rw-rw-   0        0        0      784 2022-10-30 03:15:42.000000 booze-tools-0.6.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:44:43.686386 booze-tools-0.6.2.0/
+-rw-rw-rw-   0        0        0     1089 2021-09-06 01:47:53.000000 booze-tools-0.6.2.0/LICENSE
+-rw-rw-rw-   0        0        0     5731 2023-08-07 06:44:43.686386 booze-tools-0.6.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5128 2023-08-02 04:04:59.000000 booze-tools-0.6.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 06:44:43.402882 booze-tools-0.6.2.0/booze_tools.egg-info/
+-rw-rw-rw-   0        0        0     5731 2023-08-07 06:44:43.000000 booze-tools-0.6.2.0/booze_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1662 2023-08-07 06:44:43.000000 booze-tools-0.6.2.0/booze_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 06:44:43.000000 booze-tools-0.6.2.0/booze_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-07 06:44:43.000000 booze-tools-0.6.2.0/booze_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 06:44:43.417899 booze-tools-0.6.2.0/boozetools/
+-rw-rw-rw-   0        0        0        0 2021-09-06 01:47:53.000000 booze-tools-0.6.2.0/boozetools/__init__.py
+-rw-rw-rw-   0        0        0     3714 2023-08-07 01:19:06.000000 booze-tools-0.6.2.0/boozetools/__main__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:44:43.456761 booze-tools-0.6.2.0/boozetools/macroparse/
+-rw-rw-rw-   0        0        0        0 2021-09-06 01:47:53.000000 booze-tools-0.6.2.0/boozetools/macroparse/__init__.py
+-rw-rw-rw-   0        0        0    19641 2022-09-02 06:26:53.000000 booze-tools-0.6.2.0/boozetools/macroparse/compaction.py
+-rw-rw-rw-   0        0        0    12709 2023-08-07 01:19:06.000000 booze-tools-0.6.2.0/boozetools/macroparse/compiler.py
+-rw-rw-rw-   0        0        0     8690 2022-10-09 00:56:43.000000 booze-tools-0.6.2.0/boozetools/macroparse/expansion.py
+-rw-rw-rw-   0        0        0    18516 2023-07-07 05:59:24.000000 booze-tools-0.6.2.0/boozetools/macroparse/grammar.py
+-rw-rw-rw-   0        0        0      263 2022-10-09 00:56:43.000000 booze-tools-0.6.2.0/boozetools/macroparse/interface.py
+-rw-rw-rw-   0        0        0     7822 2022-10-29 19:48:14.000000 booze-tools-0.6.2.0/boozetools/macroparse/runtime.py
+-rw-rw-rw-   0        0        0    22554 2023-08-06 02:58:32.000000 booze-tools-0.6.2.0/boozetools/menagerie.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:44:43.513057 booze-tools-0.6.2.0/boozetools/parsing/
+-rw-rw-rw-   0        0        0        0 2021-09-06 01:47:53.000000 booze-tools-0.6.2.0/boozetools/parsing/__init__.py
+-rw-rw-rw-   0        0        0      191 2023-08-07 00:53:07.000000 booze-tools-0.6.2.0/boozetools/parsing/all_methods.py
+-rw-rw-rw-   0        0        0    22013 2023-08-07 05:52:25.000000 booze-tools-0.6.2.0/boozetools/parsing/automata.py
+-rw-rw-rw-   0        0        0        0 2023-08-06 02:26:39.000000 booze-tools-0.6.2.0/boozetools/parsing/canonical.py
+-rw-rw-rw-   0        0        0    20050 2023-08-07 04:20:45.000000 booze-tools-0.6.2.0/boozetools/parsing/context_free.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:44:43.527148 booze-tools-0.6.2.0/boozetools/parsing/general/
+-rw-rw-rw-   0        0        0        0 2021-09-06 01:47:53.000000 booze-tools-0.6.2.0/boozetools/parsing/general/__init__.py
+-rw-rw-rw-   0        0        0     3875 2022-09-03 18:53:40.000000 booze-tools-0.6.2.0/boozetools/parsing/general/brute_force.py
+-rw-rw-rw-   0        0        0     6018 2022-09-02 20:18:33.000000 booze-tools-0.6.2.0/boozetools/parsing/general/gss.py
+-rw-rw-rw-   0        0        0     5684 2022-10-29 19:38:36.000000 booze-tools-0.6.2.0/boozetools/parsing/interface.py
+-rw-rw-rw-   0        0        0     8862 2023-08-07 05:04:45.000000 booze-tools-0.6.2.0/boozetools/parsing/lalr.py
+-rw-rw-rw-   0        0        0     4157 2023-08-06 07:28:56.000000 booze-tools-0.6.2.0/boozetools/parsing/lr0.py
+-rw-rw-rw-   0        0        0    10335 2023-08-07 06:08:16.000000 booze-tools-0.6.2.0/boozetools/parsing/lr1.py
+-rw-rw-rw-   0        0        0     4828 2022-10-09 09:41:28.000000 booze-tools-0.6.2.0/boozetools/parsing/miniparse.py
+-rw-rw-rw-   0        0        0    15293 2022-10-09 09:16:27.000000 booze-tools-0.6.2.0/boozetools/parsing/shift_reduce.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:44:43.577077 booze-tools-0.6.2.0/boozetools/scanning/
+-rw-rw-rw-   0        0        0        0 2021-09-06 01:47:53.000000 booze-tools-0.6.2.0/boozetools/scanning/__init__.py
+-rw-rw-rw-   0        0        0     1611 2022-09-01 05:08:45.000000 booze-tools-0.6.2.0/boozetools/scanning/charclass.py
+-rw-rw-rw-   0        0        0     6217 2022-09-02 22:19:32.000000 booze-tools-0.6.2.0/boozetools/scanning/charset.py
+-rw-rw-rw-   0        0        0     4476 2022-10-08 23:33:20.000000 booze-tools-0.6.2.0/boozetools/scanning/engine.py
+-rw-rw-rw-   0        0        0     7571 2022-09-01 05:47:11.000000 booze-tools-0.6.2.0/boozetools/scanning/finite.py
+-rw-rw-rw-   0        0        0     2996 2022-09-02 20:25:18.000000 booze-tools-0.6.2.0/boozetools/scanning/interface.py
+-rw-rw-rw-   0        0        0     4534 2022-09-04 01:32:37.000000 booze-tools-0.6.2.0/boozetools/scanning/miniscan.py
+-rw-rw-rw-   0        0        0    22191 2022-09-04 01:52:37.000000 booze-tools-0.6.2.0/boozetools/scanning/regular.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:44:43.615767 booze-tools-0.6.2.0/boozetools/support/
+-rw-rw-rw-   0        0        0        0 2021-09-06 01:47:53.000000 booze-tools-0.6.2.0/boozetools/support/__init__.py
+-rw-rw-rw-   0        0        0     6637 2023-05-05 07:02:54.000000 booze-tools-0.6.2.0/boozetools/support/failureprone.py
+-rw-rw-rw-   0        0        0     9164 2023-04-03 02:56:32.000000 booze-tools-0.6.2.0/boozetools/support/foundation.py
+-rw-rw-rw-   0        0        0     1318 2022-08-14 04:36:14.000000 booze-tools-0.6.2.0/boozetools/support/pretty.py
+-rw-rw-rw-   0        0        0     5762 2022-08-21 22:41:21.000000 booze-tools-0.6.2.0/boozetools/support/symtab.py
+-rw-rw-rw-   0        0        0     7119 2022-09-04 02:17:04.000000 booze-tools-0.6.2.0/boozetools/support/treelang.py
+-rw-rw-rw-   0        0        0       42 2023-08-07 06:44:43.687355 booze-tools-0.6.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      784 2023-08-07 06:37:16.000000 booze-tools-0.6.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:44:43.685389 booze-tools-0.6.2.0/tests/
+-rw-rw-rw-   0        0        0     4967 2022-09-04 01:52:37.000000 booze-tools-0.6.2.0/tests/test_bootstrap.py
+-rw-rw-rw-   0        0        0     1948 2021-09-06 01:47:53.000000 booze-tools-0.6.2.0/tests/test_charclass.py
+-rw-rw-rw-   0        0        0     5241 2022-09-03 03:07:50.000000 booze-tools-0.6.2.0/tests/test_deterministic.py
+-rw-rw-rw-   0        0        0     1809 2023-07-07 05:59:24.000000 booze-tools-0.6.2.0/tests/test_error_handling.py
+-rw-rw-rw-   0        0        0     7302 2023-08-06 04:14:24.000000 booze-tools-0.6.2.0/tests/test_examples.py
+-rw-rw-rw-   0        0        0      655 2021-09-20 06:03:44.000000 booze-tools-0.6.2.0/tests/test_foundation.py
+-rw-rw-rw-   0        0        0     5486 2023-08-07 04:20:45.000000 booze-tools-0.6.2.0/tests/test_generalized.py
+-rw-rw-rw-   0        0        0     1097 2023-08-02 07:14:31.000000 booze-tools-0.6.2.0/tests/test_lalr.py
+-rw-rw-rw-   0        0        0     1193 2022-09-02 06:05:18.000000 booze-tools-0.6.2.0/tests/test_miniparse.py
+-rw-rw-rw-   0        0        0     4835 2022-09-04 00:02:19.000000 booze-tools-0.6.2.0/tests/test_miniscan.py
+-rw-rw-rw-   0        0        0     2809 2022-09-02 20:05:39.000000 booze-tools-0.6.2.0/tests/test_regular.py
+-rw-rw-rw-   0        0        0     1232 2022-09-06 02:35:03.000000 booze-tools-0.6.2.0/tests/test_treelang.py
```

### Comparing `booze-tools-0.6.1.0/LICENSE` & `booze-tools-0.6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `booze-tools-0.6.1.0/PKG-INFO` & `booze-tools-0.6.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: booze-tools
-Version: 0.6.1.0
+Version: 0.6.2.0
 Summary: A panoply of tools for parsing, lexical analysis, and semantic processing
 Home-page: https://github.com/kjosib/booze-tools
 Author: Ian Kjos
 Author-email: kjosib@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
@@ -91,29 +91,42 @@
     * Transitive Closure
     * Visitor Pattern
     * Equivalence Classification
     * Hamming Distance
     * Breadth First Traversal
     * Various small array hacks
 
-The "minimal-LR(1)" algorithm used here is -- I believe -- provably minimal, even while it
-respects precedence and associativity declarations in the usual way. It is strongly inspired
-by the IELR(1) algorithm, but it is NOT exactly that algorithm. As far as I can tell it is a
-new contribution. As such, I would appreciate feedback respecting your results with it.
-
+The "minimal-LR(1)" algorithm used here is meant to create a *constructively minimal* number of
+parser states while respecting precedence and associativity declarations in the usual way.
+That means it can split states but does not (yet) attempt to merge them again afterwards.
+It is strongly inspired by the IELR(1) algorithm, but it is NOT exactly that algorithm.
+As far as I can tell it is a new contribution.
+As such, I would appreciate feedback respecting your results with it.
+
+* Caveat: See the status of issue 45 before using that mode.
+  Someone found a bug that sometimes yields LALR-like behavior.
+  I think the idea is probably sound but the execution is flawed.
+  Meanwhile, `%method CLR` in the *precedence* section will yield a full Knuth-style LR(1) table
+  which is guaranteed to be correct, even if probably larger than necessary.
 
 # Priorities?
 * These operate within a Python environment.
 * They have some features not found in other such tools.
 * Performance is accordingly not the top priority, but:
     * the profiler has been used to solve one or two problems,
     * if someone wants to play with the profiler they are welcome, and
     * contributions in that vein will be accepted as long as they are consistent with the higher priorities.
 
 # What Else?
 
 There are unit tests. They're not vast and imposing, but they exercise the interface both directly and via the example code.
 
+# Bibliography:
+
+* https://dl.acm.org/doi/pdf/10.1145/1780.1802
+
+I'll add links as I track them down.
+
 # Oh by the way..
 I'm NOT a [crack-pot](https://github.com/kjosib/booze-tools/blob/master/docs/P%20vs%20NP.md). Really I'm not.
```

### Comparing `booze-tools-0.6.1.0/README.md` & `booze-tools-0.6.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -74,27 +74,40 @@
     * Transitive Closure
     * Visitor Pattern
     * Equivalence Classification
     * Hamming Distance
     * Breadth First Traversal
     * Various small array hacks
 
-The "minimal-LR(1)" algorithm used here is -- I believe -- provably minimal, even while it
-respects precedence and associativity declarations in the usual way. It is strongly inspired
-by the IELR(1) algorithm, but it is NOT exactly that algorithm. As far as I can tell it is a
-new contribution. As such, I would appreciate feedback respecting your results with it.
-
+The "minimal-LR(1)" algorithm used here is meant to create a *constructively minimal* number of
+parser states while respecting precedence and associativity declarations in the usual way.
+That means it can split states but does not (yet) attempt to merge them again afterwards.
+It is strongly inspired by the IELR(1) algorithm, but it is NOT exactly that algorithm.
+As far as I can tell it is a new contribution.
+As such, I would appreciate feedback respecting your results with it.
+
+* Caveat: See the status of issue 45 before using that mode.
+  Someone found a bug that sometimes yields LALR-like behavior.
+  I think the idea is probably sound but the execution is flawed.
+  Meanwhile, `%method CLR` in the *precedence* section will yield a full Knuth-style LR(1) table
+  which is guaranteed to be correct, even if probably larger than necessary.
 
 # Priorities?
 * These operate within a Python environment.
 * They have some features not found in other such tools.
 * Performance is accordingly not the top priority, but:
     * the profiler has been used to solve one or two problems,
     * if someone wants to play with the profiler they are welcome, and
     * contributions in that vein will be accepted as long as they are consistent with the higher priorities.
 
 # What Else?
 
 There are unit tests. They're not vast and imposing, but they exercise the interface both directly and via the example code.
 
+# Bibliography:
+
+* https://dl.acm.org/doi/pdf/10.1145/1780.1802
+
+I'll add links as I track them down.
+
 # Oh by the way..
 I'm NOT a [crack-pot](https://github.com/kjosib/booze-tools/blob/master/docs/P%20vs%20NP.md). Really I'm not.
```

### Comparing `booze-tools-0.6.1.0/booze_tools.egg-info/PKG-INFO` & `booze-tools-0.6.2.0/booze_tools.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: booze-tools
-Version: 0.6.1.0
+Version: 0.6.2.0
 Summary: A panoply of tools for parsing, lexical analysis, and semantic processing
 Home-page: https://github.com/kjosib/booze-tools
 Author: Ian Kjos
 Author-email: kjosib@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
@@ -91,29 +91,42 @@
     * Transitive Closure
     * Visitor Pattern
     * Equivalence Classification
     * Hamming Distance
     * Breadth First Traversal
     * Various small array hacks
 
-The "minimal-LR(1)" algorithm used here is -- I believe -- provably minimal, even while it
-respects precedence and associativity declarations in the usual way. It is strongly inspired
-by the IELR(1) algorithm, but it is NOT exactly that algorithm. As far as I can tell it is a
-new contribution. As such, I would appreciate feedback respecting your results with it.
-
+The "minimal-LR(1)" algorithm used here is meant to create a *constructively minimal* number of
+parser states while respecting precedence and associativity declarations in the usual way.
+That means it can split states but does not (yet) attempt to merge them again afterwards.
+It is strongly inspired by the IELR(1) algorithm, but it is NOT exactly that algorithm.
+As far as I can tell it is a new contribution.
+As such, I would appreciate feedback respecting your results with it.
+
+* Caveat: See the status of issue 45 before using that mode.
+  Someone found a bug that sometimes yields LALR-like behavior.
+  I think the idea is probably sound but the execution is flawed.
+  Meanwhile, `%method CLR` in the *precedence* section will yield a full Knuth-style LR(1) table
+  which is guaranteed to be correct, even if probably larger than necessary.
 
 # Priorities?
 * These operate within a Python environment.
 * They have some features not found in other such tools.
 * Performance is accordingly not the top priority, but:
     * the profiler has been used to solve one or two problems,
     * if someone wants to play with the profiler they are welcome, and
     * contributions in that vein will be accepted as long as they are consistent with the higher priorities.
 
 # What Else?
 
 There are unit tests. They're not vast and imposing, but they exercise the interface both directly and via the example code.
 
+# Bibliography:
+
+* https://dl.acm.org/doi/pdf/10.1145/1780.1802
+
+I'll add links as I track them down.
+
 # Oh by the way..
 I'm NOT a [crack-pot](https://github.com/kjosib/booze-tools/blob/master/docs/P%20vs%20NP.md). Really I'm not.
```

### Comparing `booze-tools-0.6.1.0/boozetools/__main__.py` & `booze-tools-0.6.2.0/boozetools/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,42 +13,53 @@
 from boozetools.macroparse.compiler import compile_string
 from boozetools.macroparse.grammar import DefinitionError
 from boozetools.macroparse import compaction
 
 def parse_arguments():
 	parser = argparse.ArgumentParser(prog='py -m boozetools', description=__doc__,)
 	parser.add_argument('source_path', help='path to input file')
+	parser.add_argument("-m", "--method", help="Override the parse table generation method in the %method spec. (LR1, CLR, or LALR)")
 	parser.add_argument('-f', '--force', action='store_true', dest='force', help='allow to write over existing file')
 	parser.add_argument('-o', '--output', help='path to output file')
 	parser.add_argument('-i', '--indent', help='indent the JSON output for easier reading.', action='store_const', dest='indent', const=2, default=None)
 	parser.add_argument('--pretty', action='store_true', help='Display uncompressed tables in attractive grid format on STDOUT.')
 	parser.add_argument('--csv', action='store_true', help='Generate CSV versions of uncompressed tables, suitable for inspection.')
 	parser.add_argument('--dev', action='store_true', help='Operate in "development mode" -- which changes from time to time.')
 	parser.add_argument('--dot', action='store_true', help="Create a .dot file for visualizing the parser via the Graphviz package.")
 	parser.add_argument('-v', '--verbose', action='store_true', help="Squawk, mainly about the table compression stats.")
 	# if len(sys.argv) < 2: exit(parser.print_help())
 	return parser.parse_args()
 
+def _method(args):
+	if args.method:
+		from boozetools.parsing.all_methods import PARSE_TABLE_METHODS
+		try: return PARSE_TABLE_METHODS[args.method.upper()]
+		except KeyError: _err("No joy! Valid methods are: "+" ".join(PARSE_TABLE_METHODS.keys()) )
+
+def _err(msg):
+	print(msg, file=sys.stderr)
+	exit(1)
+
 def main(args):
 	if args.verbose: compaction.VERBOSE = True
 	stem, extension = os.path.splitext(args.source_path)
 	target_path = args.output or stem+'.automaton'
 	if os.path.exists(target_path) and not args.force:
-		print('Target file already exists and --force command-line argument was not given.', file=sys.stderr)
-		exit(1)
+		_err("Target file already exists and --force command-line argument was not given.")
 	with(open(args.source_path)) as fh:document = fh.read()
+	strict = not (args.pretty or args.csv or args.dot or args.dev)
 	try:
-		intermediate_form = compile_string(document)
+		intermediate_form = compile_string(document, strict, _method(args))
 		if args.dot: intermediate_form.make_dot_file(target_path+'.dot')
 		textbook_form = intermediate_form.determinize()
 	except DefinitionError as e:
-		print(e.args[0], file=sys.stderr)
-		exit(1)
+		_err(e.args[0])
 	else:
 		if args.pretty: textbook_form.pretty_print()
+		else: textbook_form.report_stats()
 		if args.csv: textbook_form.make_csv(target_path)
 		compact = textbook_form.as_compact_form(filename=os.path.basename(args.source_path))
 		if args.dev:
 			compact_goto = compact['parser']['goto']
 			for listname in ['row_index', 'col_index', 'quotient']:
 				print(listname+':', compact_goto[listname], len(compact_goto[listname]))
 			print('mark:', compact_goto['mark'], 'residue:', len(compact_goto['quotient'])-compact_goto['mark'])
```

### Comparing `booze-tools-0.6.1.0/boozetools/macroparse/compaction.py` & `booze-tools-0.6.2.0/boozetools/macroparse/compaction.py`

 * *Files identical despite different names*

### Comparing `booze-tools-0.6.1.0/boozetools/macroparse/compiler.py` & `booze-tools-0.6.2.0/boozetools/macroparse/compiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 """
 import re, os, collections
 from typing import NamedTuple, List
 from ..support import foundation, failureprone
 from ..parsing.context_free import ContextFreeGrammar
 from ..parsing.automata import DragonBookTable, ParsingStyle, GeneralizedStyle, DeterministicStyle, HFA, tabulate
-from ..parsing.all_methods import PARSE_TABLE_METHODS
 from ..scanning import finite, regular, charset
 from ..scanning.interface import INITIAL
 from . import grammar, compaction
 from .interface import ScanAction
 
 
 class TextBookForm:
@@ -63,52 +62,59 @@
 		if table.splits: form['splits'] = table.splits
 		return form
 	def pretty_print(self):
 		if self.dfa is not None:
 			self.dfa.stats()
 			self.dfa.display()
 		if self.parse_table is not None:
+			self.parse_table.stats()
 			self.parse_table.display()
+	def report_stats(self):
+		if self.dfa is not None:
+			self.dfa.stats()
+		if self.parse_table is not None:
+			self.parse_table.stats()
 	def make_csv(self, pathstem):
 		if self.dfa is not None:
 			self.dfa.make_csv(pathstem)
 		if self.parse_table is not None:
 			self.parse_table.make_csv(pathstem)
 
 class IntermediateForm(NamedTuple):
 	nfa: finite.NFA
 	scan_actions: List[ScanAction]
 	hfa: HFA
 	cfg: ContextFreeGrammar
 	parse_style:ParsingStyle
 	def determinize(self) -> TextBookForm:
 		dfa = self.nfa.subset_construction().minimize_states().minimize_alphabet() if self.nfa.states else None
-		return TextBookForm(dfa=dfa, scan_actions=self.scan_actions, parse_table=tabulate(self.hfa, self.cfg, style=self.parse_style))
+		parse_table = tabulate(self.hfa, self.cfg, style=self.parse_style)
+		return TextBookForm(dfa=dfa, scan_actions=self.scan_actions, parse_table=parse_table)
 	def make_dot_file(self, path): self.hfa.make_dot_file(path)
 
 
-def compile_string(document:str) -> IntermediateForm:
+def compile_string(document:str, strict:bool, method=None) -> IntermediateForm:
 	text = failureprone.SourceText(document)
-	return _compile_text(text)
+	return _compile_text(text, strict, method)
 
-def compile_file(pathname, *, verbose=False) -> dict:
+def compile_file(pathname, *, verbose=False, strict=True, method=None) -> dict:
 	with(open(pathname)) as fh:
 		text = failureprone.SourceText(fh.read(), filename=pathname)
-	intermediate_form = _compile_text(text)
+	intermediate_form = _compile_text(text, strict, method)
 	textbook_form = intermediate_form.determinize()
 	if verbose:
 		print("\n  -- ", pathname, " --")
 		textbook_form.pretty_print()
 	return textbook_form.as_compact_form(filename=os.path.basename(pathname))
 
 STRERROR = {
 	regular.VariableTrailingContextError: "Variable size for both stem and trailing context is not currently supported.",
 }
 
-def _compile_text(document:failureprone.SourceText) -> IntermediateForm:
+def _compile_text(document:failureprone.SourceText, strict:bool, method=None) -> IntermediateForm:
 	""" This has the job of reading the specification and building the textbook-form tables. """
 	# The approach is a sort of outside-in parse. The outermost layer concerns the overall markdown document format,
 	# which is dealt with in the main body of this routine prior to determinizing and serializing everything.
 	# Each major sub-language is line-oriented and interpreted with one of the following five subroutines:
 	
 	def handle_meta_exception(e: Exception, pattern_text:str):
 		if isinstance(e, regular.PatternError):
@@ -198,15 +204,15 @@
 				if t not in ebnf.plain_cfg.start:
 					ebnf.plain_cfg.start.append(t)
 			return productions
 		return None
 
 	# The context-free portion of the definition:
 	error_help = grammar.ErrorHelper(document.filename)
-	ebnf = grammar.EBNF_Definition(error_help)
+	ebnf = grammar.EBNF_Definition(error_help, strict)
 	
 	# The regular (finite-state) portion of the definition:
 	env = charset.mode_normal.new_child(document.filename or "text")
 	nfa = finite.NFA()
 	pending_patterns = collections.defaultdict(list) # Those awaiting an application of the `|` action...
 	scan_actions = [] # That of a regular-language rule entry is <message, parameter, trail, line_number>
 	current_pattern_group = None
@@ -242,16 +248,19 @@
 		elif current_line_text.strip().startswith('```'): in_code = True
 		else: continue
 	if in_code and section: raise grammar.DefinitionError("A code block fails to terminate before the end of the document.")
 	
 	# Compose the control tables. (Compaction is elsewhere. Serialization will be straight JSON via standard library.)
 	if condition_definitions: tie_conditions()
 	cfg = ebnf.sugarless_form()
-	hfa = ebnf.method(cfg)
-	style = GeneralizedStyle(len(hfa.graph)) if ebnf.is_nondeterministic else DeterministicStyle(False)
+	if method is None:
+		hfa = ebnf.method(cfg)
+	else:
+		hfa = method(cfg)
+	style = GeneralizedStyle(len(hfa.graph)) if ebnf.is_nondeterministic else DeterministicStyle(ebnf.is_strict)
 	return IntermediateForm(nfa=nfa, scan_actions=scan_actions, hfa=hfa, cfg=cfg, parse_style=style,)
 
 def encode_parse_rules(rules:list, constructors:list, origins:list) -> dict:
 	assert isinstance(rules, list), type(rules)
 	return {'rules': rules, 'line_number': origins, 'constructor': constructors, }
```

### Comparing `booze-tools-0.6.1.0/boozetools/macroparse/expansion.py` & `booze-tools-0.6.2.0/boozetools/macroparse/expansion.py`

 * *Files identical despite different names*

### Comparing `booze-tools-0.6.1.0/boozetools/macroparse/grammar.py` & `booze-tools-0.6.2.0/boozetools/macroparse/grammar.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from ..scanning.interface import ScannerBlocked
 from ..parsing import context_free, miniparse
 from ..parsing.interface import ParseError
 from ..parsing.all_methods import PARSE_TABLE_METHODS
 from ..support.failureprone import illustration
 
 NONDET = object()
+NONSTRICT = object()
 METHOD = object()
 VOID = object()
 VOID_SET = object()
 
 SET_PATTERNS = {
 	"upper" : lambda x: x.isalpha() and x.isupper(),
 	"lower" : lambda x: x.isalpha() and x.islower(),
@@ -210,14 +211,15 @@
 METAGRAMMAR.rule('symbol', 'topic')(Symbol)   # Topic symbol; gets its name fixed later.
 METAGRAMMAR.rule('symbol', 'name ( ' + list_of('actual_parameter', ',') + ' )')(MacroCall)
 
 # Sub-language: For specifying precedence and associativity rules:
 NAMES = one_or_more('name')
 METAGRAMMAR.rule('precedence', 'associativity '+one_or_more('terminal'))(None)
 METAGRAMMAR.rule('precedence', 'pragma_nondeterministic')(lambda : (NONDET, ()))
+METAGRAMMAR.rule('precedence', 'pragma_nonstrict')(lambda : (NONSTRICT, ()))
 @METAGRAMMAR.rule('precedence', 'pragma_method name')
 def parse_method(_, method):
 	try:
 		return METHOD, PARSE_TABLE_METHODS[method]
 	except KeyError:
 		error_message = "Unrecognized parse method %r. Options are %r." % (method, list(PARSE_TABLE_METHODS))
 		raise DefinitionError(error_message)
@@ -293,36 +295,38 @@
 			rewrite.install(ebnf, head, dict(zip(self.formals, args)))
 
 ### Grammar object:
 # Please note: The format of an action entry shall be the tuple <message_name, tuple-of-offsets, line_number>.
 # These are a pass-through into the ContextFreeGrammar and eventually the parse tables themselves.
 
 class EBNF_Definition:
-	def __init__(self, error_help:ErrorHelper):
+	def __init__(self, error_help:ErrorHelper, strict:bool):
 		self.plain_cfg = context_free.ContextFreeGrammar()
 		self.current_head = None # This bit of state facilitates the feature of beginning a line with an alternation symbol.
 		self.inferential_start = None # Use this to infer a start symbol if necessary.
 		self.macro_definitions = {} # name -> MacroDefinition
 		self.implementations = {} # canonical symbol -> line number of first elaboration
 		self.must_elaborate = []
 		self.error_help = error_help
 		self.is_nondeterministic = False
+		self.is_strict = strict
 		self.__void_symbols = set()
 		self.__void_sets = {self.__void_symbols.__contains__}
 		self.method = PARSE_TABLE_METHODS["LR1"]
 		self.__schedule = []
 	
 	def is_symbol_void(self, symbol:str):
 		return any(predicate(symbol) for predicate in self.__void_sets)
 	
 	def read_precedence_line(self, line:str, line_nr:int):
 		direction, symbols = self.error_help.parse(line, line_nr, 'precedence')
 		if direction is NONDET:
 			self.is_nondeterministic = True
 			self.method = PARSE_TABLE_METHODS["LALR"]
+		elif direction is NONSTRICT: self.is_strict = False
 		elif direction is METHOD: self.method = symbols
 		elif direction is VOID: self.__void_symbols.update(symbols)
 		elif direction is VOID_SET:
 			try: self.__void_sets.update(SET_PATTERNS[k.lower()] for k in symbols)
 			except KeyError: self.error_help.gripe_about(line, 10, "The only valid void_set patterns are %r"%(list(SET_PATTERNS)))
 		else: self.plain_cfg.assoc(direction, symbols)
```

### Comparing `booze-tools-0.6.1.0/boozetools/macroparse/runtime.py` & `booze-tools-0.6.2.0/boozetools/macroparse/runtime.py`

 * *Files identical despite different names*

### Comparing `booze-tools-0.6.1.0/boozetools/menagerie.py` & `booze-tools-0.6.2.0/boozetools/menagerie.py`

 * *Files 24% similar despite different names*

```diff
@@ -277,7 +277,181 @@
 				for l, r in zip(left_parts, right_parts):
 					print(' ' * (align - len(l)) + l + '  ' + pretty.DOT + '  ' + r)
 			for r in rule_ids:
 				rule = hfa.grammar.rules[r]
 				print("Do we reduce:  %s -> %s" % (rule.lhs, ' '.join(rule.rhs)))
 		if self.strict and self.conflicts: raise PurityError()
 
+###########
+#
+#  The old broken version of the minimal-LR1 thing
+
+
+def minimal_lr1(grammar: ContextFreeGrammar) -> HFA[LookAheadState]:
+	"""
+	This amounts to a hybrid of LALR and Canonical LR(1) in which only the conflicted
+	parts are reconsidered in greater detail. Details of the approach are in the
+	doc-comments for the `front` and `note_reduce` subroutines.
+
+	After poring over the IELR paper on several occasions, I believe there may yet be
+	some originality in this contribution. If anything, I have an argument why this
+	routine produces absolutely minimal tables: each output state has an absolutely
+	minimal set of "siblings" affiliated with a corresponding LALR state, because the
+	only thing distinguishing "siblings" is the correct final deterministic parse
+	action after the rule associated with a parse-item is recognized, and then only
+	for those (generally very few) tokens for which LALR does not figure it out. Also,
+	unit rule elimination is applied, and unreachable states (in light of conflict
+	resolutions) are never considered.
+	"""
+	
+	def front(symbol, follower, goto_transparent, iso_q):
+		"""
+		Return the list of parse-items which DIRECTLY follow from the given criteria.
+		In other words, these will be parse-items in position zero for the rules that
+		apply to nonterminal `symbol`.
+
+		`follower` may be `None` to mean "the non-conflicted portion of the reduce set,
+		or may be a specific reduce-set token.
+
+		`goto_transparent` means there is an epsilon-only path through any
+		remaining portion of the rule :param symbol: appeared in, so that reduce-set
+		conflicts should be propagated to these resulting parse-items.
+
+		`iso_q` is the ID number in the LR(0)/LALR graph corresponding to the
+		LR(1) state under construction.
+
+		The complexity here comes from how this algorithm threads the needle between
+		LALR-when-adequate and LR(1)-when-necessary.
+		"""
+		items = []
+		goto_q = lr0.graph[iso_q].shift[symbol]
+		goto_conflict = conflict_data[goto_q].tokens.keys()
+		for sub_rule_id, lr0_item in zip(grammar.symbol_rule_ids[symbol], pim.symbol_front[symbol]):
+			# Most of the smarts in this algorithm comes down to understanding what
+			# LALR found at the far end of each sub-production. We need to know which
+			# LR(0) state you reach after shifting the contents of that sub-rule.
+			# (Incidentally, the LALR construction also discovers this same information.)
+			reach = lr0.traverse(iso_q, grammar.rules[sub_rule_id].rhs)
+			if follower is None:  # We're coming from LALR-land:
+				items.append((lr0_item, None))
+				reach_conflict = conflict_data[reach].rules.get(sub_rule_id, EMPTY)
+				possible_follow = reach_conflict & successors[goto_q]
+				# Things get a bit weird for tokens that are ALSO conflicted in the
+				# goto state. Normally, we ignore them in this section; they'll come
+				# along expressly in another round through the algorithm as a split
+				# from the goto-state. However, in case of epsilon productions we
+				# must include those tokens lest the parse table may come out wrong.
+				if reach != iso_q: possible_follow -= goto_conflict
+				for token in possible_follow: items.append((lr0_item, token))
+			else:  # The canonical branch:
+				# GOTO-conflicted tokens will have resulted in canonical-style parse items.
+				# As with Canonical, they can follow a derivation only when the remainder
+				# of the current rule is "transparent", but this algorithm imposes the
+				# additional constraint regarding the token's contribution to a
+				# LALR-inadequacy in the "reach" state.
+				if follower in conflict_data[reach].tokens and goto_transparent:
+					assert follower in goto_conflict
+					items.append((lr0_item, follower))
+		return items
+	
+	def note_reduce(reduce, follower, rule_id, iso_q):
+		"""
+		There are two cases:
+
+		If the "follower" is `None`, it stands for the un-conflicted portion of the
+		corresponding LALR reduce-set.
+
+		Otherwise, the token MUST have earlier been implicated in a LALR-inadequacy
+		in this state (which fact we assert for good measure). Handle it the same as
+		Canonical-LR(1).
+
+		Incidentally, it is possible to reach a particular `reduce[follower]` list
+		more than once if and only if the follower is LALR-inadequate. Proof follows
+		from the fact that a given parse-item is visited at most once.
+		"""
+		if follower is None:
+			for t in terminal_sets[reduce_set_id[iso_q, rule_id]] - conflict_data[iso_q].rules[rule_id]:
+				assert t not in reduce
+				reduce[t] = [rule_id]
+		else:
+			assert follower in conflict_data[iso_q].rules[rule_id]
+			if follower in reduce:
+				assert rule_id not in reduce[follower]
+				reduce[follower].append(rule_id)
+			else:
+				reduce[follower] = [rule_id]
+	
+	def possible_next_terminals(iso_q):
+		union = set(terminal_sets[iso_q])
+		for rule_id in lr0.graph[iso_q].reduce:
+			union.update(terminal_sets[reduce_set_id[iso_q, rule_id]])
+		return union
+	
+	EMPTY = frozenset()
+	pim = ParseItemMap.from_grammar(grammar)
+	lr0 = lr0_construction(pim)  # This implicitly solves a lot of sub-problems.
+	terminal_sets, reduce_set_id = find_lalr_sets(lr0, grammar)
+	successors = [possible_next_terminals(iso_q) for iso_q in range(len(lr0.graph))]
+	# Later we need to know if a certain rule is implicated in an LALR conflict: if so, for which terminals?
+	# We also need to know if a state is conflicted with respect to a particular terminal.
+	conflict_data = find_conflicts(lr0.graph, {(q, r): terminal_sets[i] for (q, r), i in reduce_set_id.items()}, grammar)
+	
+	return abstract_lr1_construction(
+		pim, grammar,
+		front=front, note_reduce=note_reduce,
+		initial_follow=None,
+		lr0_catalog=lr0.bft.catalog,
+	)
+
+
+
+class ConflictData(NamedTuple):
+	tokens: dict[str, set[int]]  # The rules that conflict on this token
+	rules: dict[int, set[str]]  # The tokens that conflict on this rule.
+
+
+def find_conflicts(graph, reduce_sets, grammar) -> list[ConflictData]:
+	"""
+	This drives one of the central ideas of the Minimal-LR(1) algorithm:
+	Learn which tokens are involved in conflicts, and which rules contribute
+	to those conflicts for each token (as known to LALR).
+
+	Subtleties:
+
+	1. If an S/R conflict is DECLARED to shift, then it does not impugn the token,
+	   but the token still refers to the rule in case some other rule MAY reduce.
+
+	This routine (and the stuff that uses it) is coded with the idea that the
+	grammar may leave certain things deliberately non-deterministic. Wherever that
+	is the case, these algorithms will respect it.
+
+	2. There is a way to improve the treatment of R/R conflicts if it is known in
+	   advance that the table will be used deterministically, or if the R/R is
+	   resolved by rule precedence. It involves a pass over the LR(1) item cores
+	   considering the groups that eventually lead to a R/R conflict (they have the
+	   same suffix and follower): among those groups only the "winning" reduction
+	   item needs to stay in the core. This "normalizes" the LR(1) cores so that
+	   potentially fewer distinct ones might be generated.
+
+	Alas, idea #2 is not yet implemented. Complex R/R conflicts may still lead to
+	more states than strictly necessary for a deterministic table. In practice,
+	this is unlikely to be a real problem: deterministic tables are usually made
+	from grammars with few LALR conflicts, and in the non-deterministic case
+	nothing is wasted. Nevertheless, this remains an avenue for improvement.
+	"""
+	result = []
+	for q, state in enumerate(graph):
+		degree = Counter(state.shift.keys())  # This picks up some nonterminals but they do no harm.
+		for rule_id in state.reduce:
+			for token in reduce_sets[q, rule_id]:
+				prefer_shift = token in state.shift and grammar.decide_shift_reduce(token, rule_id) == RIGHT
+				if not prefer_shift: degree[token] += 1
+		conflicted_tokens = set(token for token, count in degree.items() if count > 1)
+		conflict = ConflictData({token: set() for token in conflicted_tokens}, {})
+		for rule_id in state.reduce:
+			contribution = conflicted_tokens & reduce_sets[q, rule_id]
+			conflict.rules[rule_id] = contribution
+			for token in contribution: conflict.tokens[token].add(rule_id)
+		result.append(conflict)
+	return result
+
+
```

### Comparing `booze-tools-0.6.1.0/boozetools/parsing/automata.py` & `booze-tools-0.6.2.0/boozetools/parsing/automata.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 The HFA class itself contains a trial-parse routine which exercises these constructions
 by determining whether they recognize a string as "in the language". It's great for testing
 and illustrates one method to perform a parallel-parse, but it does not bother to recover a
 parse tree or semantic value. Such things could be added, but preferably atop good means
 for persisting ambiguous parse tables.
 """
-import collections, sys
+import sys
 from pprint import pprint
 from typing import Iterable, TypeVar, Generic, Any
 from typing import NamedTuple
 from ..support import foundation, pretty
 from .interface import HandleFindingAutomaton, END_OF_TOKENS, ERROR_SYMBOL, ParseError
 from .context_free import ContextFreeGrammar, Rule, SemanticAction, LEFT, RIGHT, NONASSOC, BOGUS
 
@@ -104,59 +104,89 @@
 		
 		def reduce(stack, rule_id):
 			""" To perform a reduction, roll the stack to before the RHS and then shift the LHS. """
 			rule = rules[rule_id]
 			for i in range(len(rule.rhs)): stack = stack[1]
 			return self.graph[stack[0]].shift[rule.lhs], stack
 		
-		root = (initial, None)
-		alive = [root]
-		for lexeme in sentence:
-			next = []
+		def lock_step_parallel():
+			root = (initial, None)
+			alive = [root]
+			for lexeme in sentence:
+				subsequent = []
+				for stack in alive:
+					state = self.graph[stack[0]]
+					if lexeme in state.shift: subsequent.append((state.shift[lexeme], stack))
+					for rule_id in state.reductions_before(lexeme): alive.append(reduce(stack, rule_id))
+				alive = subsequent
+				if not alive: raise ParseError("Parser died midway at something ungrammatical.")
 			for stack in alive:
-				state = self.graph[stack[0]]
-				if lexeme in state.shift: next.append((state.shift[lexeme], stack))
-				for rule_id in state.reductions_before(lexeme): alive.append(reduce(stack, rule_id))
-			alive = next
-			if not alive: raise ParseError("Parser died midway at something ungrammatical.")
-		for stack in alive:
-			q = stack[0]
-			if q == accept: return True
-			for rule_id in self.graph[q].reductions_before(END_OF_TOKENS):
-				alive.append(reduce(stack, rule_id))
-		raise ParseError("Parser recognized a viable prefix, but not a complete sentence.")
+				q = stack[0]
+				if q == accept: return True
+				for rule_id in self.graph[q].reductions_before(END_OF_TOKENS):
+					alive.append(reduce(stack, rule_id))
+			raise ParseError("Parser recognized a viable prefix, but not a complete sentence.")
+		return lock_step_parallel()
 
+	def has_shift_reduce_conflict(self):
+		return any(state.has_shift_reduce_conflict() for state in self.graph)
+
+	def has_reduce_reduce_conflict(self):
+		return any(state.has_reduce_reduce_conflict() for state in self.graph)
 
 class LR0_State(NamedTuple):
 	"""
 	The LR(0) construction completely ignores right-context.
 	Therefore, an LR(0) state tracks which rules it may recognize,
 	but does not differentiate this information any further.
 	"""
 	shift: dict[str, int]  # symbol => state-id
 	reduce: list[int]  # rule-id
+	closure: set[int]  # set of parse-item index
 	
 	def reductions_before(self, lexeme):
 		""" Did I mention LR(0) doesn't worry about look-ahead? """
 		return self.reduce
 
+	def has_shift_reduce_conflict(self):
+		return bool(self.shift and self.reduce)
+	
+	def has_reduce_reduce_conflict(self):
+		return len(self.reduce)>1
+	
+	def has_conflict(self):
+		return self.has_shift_reduce_conflict() or self.has_reduce_reduce_conflict()
+
+	def is_adequate_reduce(self):
+		return len(self.reduce) == 1 and not self.shift
 
 class LookAheadState(NamedTuple):
 	"""
 	An LR(1) or LALR(1) table needs to take a token of right-context
 	into account when recognizing a rule. Therefore, the .reduce field
 	is a dictionary keyed by look-ahead token.
 	"""
 	shift: dict[str, int]  # symbol => state-id
-	reduce: dict[str, list[int]]  # LALR
+	reduce: dict[str, list[int]]  # symbol => list of rule_id
 	
 	def reductions_before(self, lexeme):
-		return self.reduce.get(lexeme, ())
-
+		if None in self.reduce:
+			assert len(self.reduce) == 1
+			return self.reduce[None]
+		else:
+			return self.reduce.get(lexeme, ())
 
+	def has_shift_reduce_conflict(self):
+		return bool(self.shift.keys() & self.reduce.keys())
+	
+	def has_reduce_reduce_conflict(self):
+		return any(len(r)>1 for r in self.reduce.values())
+	
+	def has_conflict(self):
+		return self.has_shift_reduce_conflict() or self.has_reduce_reduce_conflict()
 
 def reachable(step: dict, reduce: dict, grammar:ContextFreeGrammar) -> dict:
 	"""
 	This function exists so that parse-table construction algorithms can respect operator
 	precedence and associativity declarations in a grammar specification. It is a vital
 	part of minimal-LR1 mode, but it also works for LALR and canonical-LR1.
 	
@@ -170,15 +200,15 @@
 	defined. The code below should either behave sensibly or toss an exception.
 
 	The problem with the bizarre corner cases is they cannot be understood solely in terms
 	of actions the parser might (or might not) take in this state. If they come up, you
 	get a warning printed on STDERR but otherwise the operator-precedence declarations
 	are ignored in that instance.
 	
-	FIXME: This function should not perform I/O directly.
+	FIXME: This function ought not perform I/O directly.
 	"""
 	for token, rule_id_list in list(reduce.items()):
 		if token not in step: continue
 		decide = [grammar.decide_shift_reduce(token, rule_id) for rule_id in rule_id_list]
 		ways = set(decide)
 		assert BOGUS not in ways, "This is guaranteed by grammar.validate(...), called earlier."
 		if len(ways) == 1:
@@ -279,21 +309,26 @@
 	
 	def get_goto(self, state_id, nonterminal_id) -> int: return self.goto_matrix[state_id][nonterminal_id]
 	
 	def get_initial(self, language) -> int: return 0 if language is None else self.initial[language]
 	
 	def get_breadcrumb(self, state_id) -> str: return self.breadcrumbs[state_id]
 	
-	def display(self):
+	def stats(self):
 		size = len(self.action_matrix)
-		print('Action and Goto: (%d states)' % size)
+		print('Action and Goto: %d states' % size)
+		if self.splits:
+			print("%d nondeterministic splits" % len(self.splits))
+
+	def display(self):
+		mask = lambda xs:[x or "" for x in xs]
 		head = ['', ''] + self.terminals + [''] + self.nonterminals
 		body = []
 		for i, (b, a, g) in enumerate(zip(self.breadcrumbs, self.action_matrix, self.goto_matrix)):
-			body.append([i, b, *a, '', *g])
+			body.append([i, b, *mask(a), '', *mask(g)])
 		pretty.print_grid([head] + body)
 		if self.splits:
 			print("Splits:")
 			pprint(self.splits)
 	
 	def make_csv(self, pathstem):
 		""" Generate action and goto tables into CSV files suitable for inspection in a spreadsheet program. """
@@ -344,32 +379,38 @@
 		""" Called in all non-deterministic situations. """
 		raise NotImplementedError(type(self))
 	
 	def any_splits(self):
 		""" Return nothing, or a list of splits for use in non-deterministic parsing algorithms. """
 		raise NotImplementedError(type(self))
 
-	def report(self, hfa):
+	def report(self, hfa, rules):
 		""" Give user-feedback about any observed challenges. """
 		raise NotImplementedError(type(self))
 
 class DeterministicStyle(ParsingStyle):
 	
 	def __init__(self, strict:bool):
-		self.conflicts = collections.defaultdict(list)
-		self.strict = strict
+		self._conflict_rules = {}
+		self._conflict_shift = set()
+		self._strict = strict
 	
 	def decide_inadequacy(self, q:int, look_ahead: str, shift: int, rule_ids: Iterable, rules:list) -> int:
-		self.conflicts[q, look_ahead].extend(rule_ids)
-		return shift or encode_reduce(min(rule_ids))
+		key = (q, look_ahead)
+		self._conflict_rules[key] = rule_ids
+		if shift:
+			self._conflict_shift.add(key)
+			return shift
+		else:
+			return encode_reduce(min(rule_ids))
 	
 	def any_splits(self):
 		pass
 	
-	def report(self, hfa):
+	def report(self, hfa, rules):
 		"""
 		This function was originally intended as a way to visualize the branches of a conflict.
 		In its original form a bunch of context was available; I've gratuitously stripped that away
 		and now I want to break this down to the bits we actually need.
 		
 		BreadthFirstTraversal.traversal[x] was used to grab the core parse items in order to
 		visualize the state reached by shifting the lookahead token if that shift is viable.
@@ -377,23 +418,36 @@
 		
 		The "options" list contains numeric candidate ACTION instructions which are interpreted
 		in the usual way: This does represent a data-coupling, but one that's unlikely to change,
 		so I'm not too worried about it just now.
 		
 		In conclusion: Let the objects defined in automata.py format parse-states for human consumption.
 		"""
-		if not self.conflicts:
+		if not self._conflict_rules:
 			# print("Grammar specification is fully deterministic.")
 			pass
-		elif self.strict:
-			raise PurityError(self.conflicts)
 		else:
-			print("Grammar specification contains conflicts.")
-			print("Conflict reporting is presently undergoing an overhaul, but here's some diagnostic data:")
-			pprint(self.conflicts)
+			print(("  "+pretty.DOT)*20)
+			print(
+				"Grammar entails %d shift/reduce conflicts and %d reduce/reduce conflicts."%
+				(len(self._conflict_shift), len(self._conflict_rules) - len(self._conflict_shift)),
+			)
+			bft = hfa.bft
+			for key, rule_ids in sorted(self._conflict_rules.items()):
+				print()
+				(q, look_ahead) = key
+				print(' '.join(bft.breadcrumbs[k] for k in bft.shortest_path_to(q)[1:]), pretty.DOT, look_ahead)
+				if key in self._conflict_shift:
+					print("<shift>")
+				for rule_id in rule_ids:
+					print("\t\t\t",rules[rule_id])
+			print()
+			print(("  "+pretty.DOT)*20)
+			if self._strict:
+				raise PurityError(self._conflict_rules)
 
 class GeneralizedStyle(ParsingStyle):
 	
 	def __init__(self, splits_offset:int):
 		self.offset = splits_offset
 		self.splits = []
 	
@@ -402,15 +456,15 @@
 		if shift: split.append(shift)
 		for r in sorted(rule_ids, key=lambda i:len(rules[i].rhs)): split.append(-1-r)
 		return self.offset + foundation.allocate(self.splits, split)
 	
 	def any_splits(self):
 		return self.splits
 	
-	def report(self, hfa):
+	def report(self, hfa, rules):
 		print(len(self.splits), "non-deterministic situation(s) encountered.")
 
 
 def encode_reduce(rule_id:int) -> int:
 	""" See interface.HandleFindingAutomaton.get_action. """
 	return -1 - rule_id
 
@@ -429,35 +483,41 @@
 	"""
 	assert isinstance(grammar, ContextFreeGrammar), grammar
 	assert END_OF_TOKENS not in grammar.symbols
 	assert ERROR_SYMBOL not in grammar.symbol_rule_ids
 	terminals = [END_OF_TOKENS] + sorted(grammar.apparent_terminals())
 	translate = {t:i for i,t in enumerate(terminals)}
 	nonterminals = sorted(grammar.symbol_rule_ids.keys())
+	
 	##### Tabulate the states into dense matrices ACTION and GOTO:
 	action, goto, nonassoc_errors = [], [], set()
-	conflict = collections.defaultdict(set)
 	for q, state in enumerate(hfa.graph):
 		goto.append([state.shift.get(s, 0) for s in nonterminals])
-		action_row = [state.shift.get(s, 0) for s in terminals]
-		conflict.clear()
-		for symbol, rule_ids in state.reduce.items():
-			idx = translate[symbol]
-			shift = action_row[idx]
-			if rule_ids == ():
-				# This is how function `reachable(...)` communicates a non-association situation.
-				assert shift == 0
-				nonassoc_errors.add((q,idx))
-			elif shift == 0 and len(rule_ids) == 1:
-				action_row[idx] = encode_reduce(rule_ids[0])
-			else: action_row[idx] = style.decide_inadequacy(q, symbol, shift, rule_ids, grammar.rules)
+		if None in state.reduce:
+			assert len(state.reduce) == 1
+			assert len(state.reduce[None]) == 1, (q, state.reduce[None])
+			sole_action = encode_reduce(state.reduce[None][0])
+			action_row = [sole_action]  * len(terminals)
+		else:
+			action_row = [state.shift.get(s, 0) for s in terminals]
+			for symbol, rule_ids in state.reduce.items():
+				idx = translate[symbol]
+				shift = action_row[idx]
+				if rule_ids == ():
+					# This is how function `reachable(...)` communicates a non-association situation.
+					assert shift == 0
+					nonassoc_errors.add((q,idx))
+				elif shift == 0 and len(rule_ids) == 1:
+					action_row[idx] = encode_reduce(rule_ids[0])
+				else: action_row[idx] = style.decide_inadequacy(q, symbol, shift, rule_ids, grammar.rules)
 		action.append(action_row)
+	
 	for q, t in nonassoc_errors: action[q][t] = 0
 	for q in hfa.accept: action[q][0] = q
-	style.report(hfa)
+	style.report(hfa, grammar.rules)
 	return DragonBookTable(
 		initial=dict(zip(grammar.start, hfa.initial)),
 		action=action,
 		goto=goto,
 		nonassoc_errors=nonassoc_errors,
 		rules=grammar.rules,
 		terminals=terminals,
```

### Comparing `booze-tools-0.6.1.0/boozetools/parsing/context_free.py` & `booze-tools-0.6.2.0/boozetools/parsing/context_free.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,16 +76,16 @@
 	It might be nice to get a more complete read-out of problems, but that would mean
 	inventing some sort of document structure to talk about faults in grammars.
 	Then again, maybe that's in the pipeline.
 	"""
 	def rule_produces_bogon(self, rule, symbol):
 		raise Fault("Rule at %r produces bogus terminal(s) %r." % (rule.provenance, symbol))
 	
-	def epsilon_right_recursion(self, rule):
-		raise Fault("Rule at %r produces epsilon right-recursion."%rule.provenance)
+	def nullable_right_recursion(self, rule):
+		raise Fault("Rule at %r produces nullable right-recursion."%rule.provenance)
 	
 	def nonterminal_given_precedence(self, symbol):
 		raise Fault("Nonterminal %r included in precedence declaration."%symbol)
 	
 	def bad_prec_sym(self, rule):
 		raise Fault("Rule at %r has an explicit precedence-symbol without a defined precedence level.", rule.provenance)
 	
@@ -105,17 +105,17 @@
 		# FIXME: convey the location of the problem?
 		raise Fault("Symbol %r may be replaced by itself in a recursive loop."%symbol)
 
 	def mutual_recursive_loop(self, symbols):
 		# FIXME: convey the locations of the problematic rules?
 		raise Fault("Symbols %r may be replaced by one another in a mutually-recursive loop."%symbols)
 
-	def epsilon_mutual_recursion(self, symbols):
+	def mutual_nullable_recursion(self, symbols):
 		# FIXME: convey the locations of the problematic rules?
-		raise Fault("Symbols %r form a mutually-recursive epsilon loop."%symbols)
+		raise Fault("Symbols %r form a mutually-recursive nullable loop."%symbols)
 
 class SimpleFaultHandler(FaultHandler):
 	""" Protocols cannot be instantiated, so here's a simple way to get "raise for everything" behavior. """
 	pass
 
 
 class SemanticAction(NamedTuple):
@@ -310,17 +310,17 @@
 		return self.ops.decide_shift_reduce(symbol, self.rules[rule_id])
 	
 	def apparent_terminals(self) -> set:
 		""" Of all symbols mentioned, those without production rules are apparently terminal. """
 		# FIXME: This could be a pluggable strategy, and MAY be misplaced. Validation and table generation need to know.
 		return self.symbols - self.symbol_rule_ids.keys()
 	
-	def bipartite_closure(self, root_symbols) -> set:
+	def _bipartite_closure(self, root_symbols) -> set:
 		"""
-		The algorithm to find epsilon symbols and well-founded symbols is basically the same,
+		The algorithm to find nullable symbols and well-founded symbols is basically the same,
 		with different initial conditions. It's a bipartite propagation, alternating between
 		disjuncts (symbols) and conjuncts (rules). By factoring this out and focusing on the
 		graph structure of the problem (and also getting some sleep) a decent solution arose.
 		"""
 		# Structuring the problem in bipartite-graph form, as explained in the docstring.
 		# The transitive closure involves some stateful cleverness:
 		# Rely on the foundation library for proper abstraction:
@@ -330,40 +330,40 @@
 				remain[rule_id] -= 1
 				if remain[rule_id] == 0:
 					yield self.rules[rule_id].lhs
 		
 		remain = [len(rule.rhs) for rule in self.rules]
 		return foundation.transitive_closure(root_symbols, successors)
 	
-	def find_epsilon(self) -> set:
+	def find_nullable(self) -> set:
 		""" Which symbols may produce the empty string? """
-		return self.bipartite_closure(rule.lhs for rule in self.rules if not rule.rhs)
+		return self._bipartite_closure(rule.lhs for rule in self.rules if not rule.rhs)
 	
 	def find_first(self):
 		"""
 		Particularly the LL school of grammar processing uses first-sets.
 		These tables answer the question: For each nonterminal symbol,
 		what terminal symbols could it possibly start with?
 		
 		The FIRST set of a nonterminal is the union of the FIRST sets of each right-hand side.
-		Without epsilon symbols, the FIRST set of a right-hand side is that of its first symbol.
-		With them, you need to include all symbols up to the first non-epsilon symbol.
+		Without nullable symbols, the FIRST set of a right-hand side is that of its first symbol.
+		With them, you need to include all symbols up to the first non-nullable symbol.
 		
 		Anyway, this is a job for a strongly_connected_components,
 		in part because it also produces a topological sort which
 		allows for a quick determination of the level sets.
 		"""
 		
 		# Structure the problem as a graph, called ``first``
 		first = collections.defaultdict(set)
-		epsilon = self.find_epsilon()
+		nullable = self.find_nullable()
 		for rule in self.rules:
 			for symbol in rule.rhs:
 				first[rule.lhs].add(symbol)
-				if symbol not in epsilon: break
+				if symbol not in nullable: break
 		
 		# Gather up the answer in topological order:
 		for component in foundation.strongly_connected_components_hashable(first):
 			# All the members of a component share a first-set, here called ``f``.
 			f = set()
 			for symbol in component:  # Not sure about performance with large SCCs.
 				f.update(*(first[x] for x in first[symbol]))
@@ -376,22 +376,22 @@
 		Here, "well-founded" means "can possibly produce a finite sequence of terminals."
 		The opposite is called "ill-founded".
 
 		Here are two examples of ill-founded grammars:
 			S -> x S   -- This is ill-founded because there's always one more S.
 			A -> B y;  B -> A x     -- Similar, but with mutual recursion.
 
-		A terminal symbol is well-founded. So is an epsilon symbol, since zero is finite.
+		A terminal symbol is well-founded. So is a nullable symbol, since zero is finite.
 		A rule with only well-founded symbols in the right-hand side is well-founded.
 		A non-terminal symbol with at least one well-founded rule is well-founded.
 		Induction applies. That induction happens to be called ``bipartite_closure``.
 
 		A grammar with only well-founded symbols is well-founded.
 		"""
-		well_founded = self.bipartite_closure(self.apparent_terminals() | self.find_epsilon())
+		well_founded = self._bipartite_closure(self.apparent_terminals() | self.find_nullable())
 		ill_founded = self.symbol_rule_ids.keys() - well_founded
 		if ill_founded:
 			fault_handler.ill_founded_symbols(ill_founded)
 	
 	def assert_no_orphans(self, fault_handler:FaultHandler):
 		"""
 		Every symbol should be reachable from the start symbol(s).
@@ -411,29 +411,29 @@
 				if rule.lhs == rule.rhs[0]:
 					fault_handler.self_recursive_loop(rule.lhs)
 				else:
 					renames[rule.lhs].add(rule.rhs[0])
 		for component in foundation.strongly_connected_components_hashable(renames):
 			if len(component) > 1: fault_handler.mutual_recursive_loop(component)
 	
-	def assert_no_epsilon_loops(self, fault_handler:FaultHandler):
-		""" Epsilon Left-Self-Recursion is OK. All other recursive-epsilon-loops are pathological. """
-		epsilon = self.find_epsilon()
+	def assert_no_nullable_loops(self, fault_handler:FaultHandler):
+		""" Nullable Left-Self-Recursion is OK. All other recursive-nullable-loops are pathological. """
+		nullable = self.find_nullable()
 		reaches = collections.defaultdict(set)
 		for rule in self.rules:
-			epsilon_prefix = list(itertools.takewhile(epsilon.__contains__, rule.rhs))
-			if not epsilon_prefix: continue
-			if epsilon_prefix[0] == rule.lhs: epsilon_prefix.pop(0)
-			if rule.lhs in epsilon_prefix:
+			nullable_prefix = list(itertools.takewhile(nullable.__contains__, rule.rhs))
+			if not nullable_prefix: continue
+			if nullable_prefix[0] == rule.lhs: nullable_prefix.pop(0)
+			if rule.lhs in nullable_prefix:
 				# Somehow this case seems qualitatively different.
-				fault_handler.epsilon_right_recursion(rule)
-			reaches[rule.lhs].update(epsilon_prefix)
+				fault_handler.nullable_right_recursion(rule)
+			reaches[rule.lhs].update(nullable_prefix)
 		for component in foundation.strongly_connected_components_hashable(reaches):
 			if len(component) > 1:
-				fault_handler.epsilon_mutual_recursion(component)
+				fault_handler.mutual_nullable_recursion(component)
 	
 	def assert_no_duplicate_rules(self, fault_handler:FaultHandler):
 		for symbol, rule_ids in self.symbol_rule_ids.items():
 			inverse = collections.defaultdict(list)
 			for r in rule_ids:
 				inverse[tuple(self.rules[r].rhs)].append(r)
 			for rs in inverse.values():
@@ -445,12 +445,12 @@
 		Calls the fault handler with every identified fault. The default fault handler
 		raises an exception (derived from Fault, above) for the first error noticed.
 		"""
 		self.ops.validate(fault_handler, self.rules)
 		self.assert_well_founded(fault_handler)
 		self.assert_no_orphans(fault_handler)
 		self.assert_no_rename_loops(fault_handler)
-		self.assert_no_epsilon_loops(fault_handler)
+		self.assert_no_nullable_loops(fault_handler)
 		if not allow_duplicate_rules:
 			self.assert_no_duplicate_rules(fault_handler)
```

### Comparing `booze-tools-0.6.1.0/boozetools/parsing/general/brute_force.py` & `booze-tools-0.6.2.0/boozetools/parsing/general/brute_force.py`

 * *Files identical despite different names*

### Comparing `booze-tools-0.6.1.0/boozetools/parsing/general/gss.py` & `booze-tools-0.6.2.0/boozetools/parsing/general/gss.py`

 * *Files identical despite different names*

### Comparing `booze-tools-0.6.1.0/boozetools/parsing/interface.py` & `booze-tools-0.6.2.0/boozetools/parsing/interface.py`

 * *Files identical despite different names*

### Comparing `booze-tools-0.6.1.0/boozetools/parsing/lalr.py` & `booze-tools-0.6.2.0/boozetools/parsing/lalr.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 1. Chapter 9 of Parsing Techniques: a Practical Guide, by Dick Grune and Ceriel Jacobs.
 2. Source code to lemon.c parser generator. See [3] for one copy.
 3. Source code to lime.php parser generator. https://github.com/rvanvelzen/lime
 
 ================================================================================
 """
 
-from typing import NamedTuple
 from ..support.foundation import allocate, strongly_connected_components_by_tarjan
 from .interface import END_OF_TOKENS
 from .context_free import ContextFreeGrammar
 from .automata import HFA, LR0_State, LookAheadState, reachable
 from .lr0 import lr0_construction, ParseItemMap
 
 
@@ -104,18 +103,18 @@
 		2. terminal_sets[reduce_set_id[state_id, rule_id]] is the set of tokens which the LALR
 		   algorithm determines can trigger reduction.
 	"""
 	graph = lr0.graph
 	terminals = grammar.apparent_terminals()
 	
 	# Prepare to find first-sets:
-	epsilon = grammar.find_epsilon()
+	nullable = grammar.find_nullable()
 	terminal_sets = [terminals.intersection(node.shift) for node in graph]
 	for q in lr0.accept:terminal_sets[q].add(END_OF_TOKENS)
-	inbound = [[dst for symbol, dst in node.shift.items() if symbol in epsilon] for node in graph]
+	inbound = [[dst for symbol, dst in node.shift.items() if symbol in nullable] for node in graph]
 	
 	# Now do something about follow-sets and reduce-sets.
 	
 	# There is one follow-set for each nonterminal-edge in the graph.
 	# There is one reduce-set for each reducing parse-item in a parse-item-core.
 	# One must not confuse these two distinct ideas, lest one end up with NQ-LALR.
 	nonterminals = frozenset(grammar.symbol_rule_ids)
@@ -128,15 +127,15 @@
 		for symbol, q_dst in node.shift.items():
 			if symbol in nonterminals:
 				# A follow-set always contains the FIRST-set of the successor-state...
 				follow_set_id[q_src, symbol] = allocate(terminal_sets, set())
 				inbound.append([q_dst])
 	
 	# And, there is some kind of inclusion relation between them.
-	prefix, suffix = prepare_rule_affixes(grammar.rules, epsilon, nonterminals)
+	prefix, suffix = prepare_rule_affixes(grammar.rules, nullable, nonterminals)
 	for (q_src, lhs), src_fs_id in follow_set_id.items():
 		for rule_id in grammar.symbol_rule_ids[lhs]:
 			# A prefix of the RHS symbols does not "see" this follow-set:
 			q_mid = lr0.traverse(q_src, prefix[rule_id])
 			# Suffix symbols can "see" this follow-set, so they must be connected up:
 			for symbol in suffix[rule_id]:
 				inbound[follow_set_id[q_mid, symbol]].append(src_fs_id)
```

### Comparing `booze-tools-0.6.1.0/boozetools/parsing/lr0.py` & `booze-tools-0.6.2.0/boozetools/parsing/lr0.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,96 +1,103 @@
 """
 Of all the LR-style parsing methods, LR(0) is the least sophisticated and the easiest to understand.
 It's also the functional foundation for all the rest, so it makes sense to start reading here.
 """
 
-from typing import NamedTuple
+from typing import NamedTuple, Optional
 from collections import defaultdict
 
 from ..support.foundation import transitive_closure, BreadthFirstTraversal
 from .context_free import ContextFreeGrammar
 from .automata import HFA, LR0_State
 
+class ParseItem(NamedTuple):
+	""" It's quite handy to be able to work symbolically with parse-items. """
+	
+	next_symbol : Optional[str]  # None means end-of-rule.
+	rule_id : Optional[int]  # None means it's a pseudo-rule for the augmented grammar
+	offset : int
+
 class ParseItemMap(NamedTuple):
 	"""
 	The key to the whole LR genera is the notion of a parse-item (and subsets of them).
 	Normally, we think of a parse-item as a pair: a rule (or its ID, or its right-hand side)
 	crossed with an index into (or just past) that right-hand side. And this is well-enough.
 	However, it's an ungainly structure. I propose an alternative based on sentinels,
 	so that a small integer refers to a parse-item, and the next higher integer is the
 	successor parse-item. We index an array (symbol_at) to find the symbol at the dot,
 	or None for the end of a rule. Other mappings facilitate each step in the dance.
 	
 	There's a subtle idea lurking in here:
 	This structure is an interesting representation of all the rules in a context-free grammar.
 	With it, the fact that parse-items are also just numbers is ALMOST completely hidden.
 	"""
-	symbol_at : list[str]
-	rule_found : dict[int, int]
+	parse_items : list[ParseItem]
 	symbol_front : dict[str: list[int]]
 	language_front : list[int]
-	nr_rules : int
 	
 	@staticmethod
 	def from_grammar(grammar: ContextFreeGrammar):
-		
-		symbol_at, rule_found, language_front = [], {}, []
-		symbol_front = {N: [] for N in grammar.symbol_rule_ids}
+		parse_item = []
+		language_front = []
+		symbol_front = {nonterminal: [] for nonterminal in grammar.symbol_rule_ids}
 		
 		def plonk(where, rhs):
-			where.append(len(symbol_at))
-			symbol_at.extend(rhs)
-			rule_found[len(symbol_at)] = len(rule_found)
-			symbol_at.append(None)
+			where.append(len(parse_item))
+			for offset, symbol in enumerate(rhs):
+				parse_item.append(ParseItem(symbol, rule_id, offset))
+			parse_item.append(ParseItem(None, rule_id, len(rhs)))
 		
-		for rule in grammar.rules:
+		for rule_id, rule in enumerate(grammar.rules):
 			plonk(symbol_front[rule.lhs], rule.rhs)
 		
-		for symbol in grammar.start:
-			plonk(language_front, [symbol])
+		rule_id = None
+		for language in grammar.start:
+			plonk(language_front, [language])
 		
-		return ParseItemMap(symbol_at, rule_found, symbol_front, language_front, len(grammar.rules))
+		return ParseItemMap(parse_item, symbol_front, language_front)
 
 
 def lr0_construction(pim:ParseItemMap) -> HFA[LR0_State]:
 	"""
 	In broad strokes, this is a subset-construction with a sophisticated means
 	to identify successor-states. The keys (by which nodes are identified) are
 	core-sets of LR0 parse items. (See also _prepare_parse_items.)
 
 	Additionally, during the full-elaboration step in visiting a core, completed
 	parse-items correspond to a state's `reduce` entries. We don't worry about
 	look-ahead in this construction: hence the '0' in LR(0). The net result is
 	a compact table generated very quickly, but with somewhat limited power.
 	In practical systems, LR(0) is normally just a first step, but some few
 	grammars are deterministic in LR(0).
+	
+	Note that the core-item sets may be found at hfa.bft.traversal.
 	"""
 	
 	def build_state(core_item_set: frozenset):
-		def visit_parse_item(item):
-			next_symbol = symbol_at[item]
-			if next_symbol is None:
-				rule_id = rule_found[item]
-				if rule_id < nr_rules:
-					reduce.append(rule_id)
+		def visit_parse_item(i):
+			pi = parse_items[i]
+			if pi.next_symbol is None:
+				if pi.rule_id is not None:
+					reduce.append(pi.rule_id)
 			else:
-				shifted_cores[next_symbol].append(item + 1)
-				return symbol_front.get(next_symbol)
+				shifted_cores[pi.next_symbol].append(i + 1)
+				return symbol_front.get(pi.next_symbol)
 		
 		shifted_cores, reduce = defaultdict(list), []
-		transitive_closure(core_item_set, visit_parse_item)
+		closure = transitive_closure(core_item_set, visit_parse_item)
 		
 		shift = {
 			symbol: bft.lookup(frozenset(item_set), breadcrumb=symbol)
 			for symbol, item_set in shifted_cores.items()
 		}
-		graph.append(LR0_State(shift=shift, reduce=reduce))
+		graph.append(LR0_State(shift=shift, reduce=reduce, closure=closure))
 
-	symbol_at, rule_found, symbol_front, language_front, nr_rules = pim
+	parse_items, symbol_front, language_front = pim
 	
 	bft = BreadthFirstTraversal()
-	initial = [bft.lookup(frozenset([item])) for item in language_front]
+	initial = [bft.lookup(frozenset([item_index])) for item_index in language_front]
 	graph = []
 	bft.execute(build_state)
-	accept = [graph[qi].shift[symbol_at[item]] for item, qi in zip(language_front, initial)]
+	accept = [graph[qi].shift[parse_items[i].next_symbol] for i, qi in zip(language_front, initial)]
 	return HFA(graph=graph, initial=initial, accept=accept, bft=bft)
```

### Comparing `booze-tools-0.6.1.0/boozetools/parsing/miniparse.py` & `booze-tools-0.6.2.0/boozetools/parsing/miniparse.py`

 * *Files identical despite different names*

### Comparing `booze-tools-0.6.1.0/boozetools/parsing/shift_reduce.py` & `booze-tools-0.6.2.0/boozetools/parsing/shift_reduce.py`

 * *Files identical despite different names*

### Comparing `booze-tools-0.6.1.0/boozetools/scanning/charclass.py` & `booze-tools-0.6.2.0/boozetools/scanning/charclass.py`

 * *Files identical despite different names*

### Comparing `booze-tools-0.6.1.0/boozetools/scanning/charset.py` & `booze-tools-0.6.2.0/boozetools/scanning/charset.py`

 * *Files identical despite different names*

### Comparing `booze-tools-0.6.1.0/boozetools/scanning/engine.py` & `booze-tools-0.6.2.0/boozetools/scanning/engine.py`

 * *Files identical despite different names*

### Comparing `booze-tools-0.6.1.0/boozetools/scanning/finite.py` & `booze-tools-0.6.2.0/boozetools/scanning/finite.py`

 * *Files identical despite different names*

### Comparing `booze-tools-0.6.1.0/boozetools/scanning/interface.py` & `booze-tools-0.6.2.0/boozetools/scanning/interface.py`

 * *Files identical despite different names*

### Comparing `booze-tools-0.6.1.0/boozetools/scanning/miniscan.py` & `booze-tools-0.6.2.0/boozetools/scanning/miniscan.py`

 * *Files identical despite different names*

### Comparing `booze-tools-0.6.1.0/boozetools/scanning/regular.py` & `booze-tools-0.6.2.0/boozetools/scanning/regular.py`

 * *Files identical despite different names*

### Comparing `booze-tools-0.6.1.0/boozetools/support/failureprone.py` & `booze-tools-0.6.2.0/boozetools/support/failureprone.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 		This will generate a not-completely-terrible error report in text-only format.
 		The precise format is subject to change, but basically you should be able to
 		print this on stderr and not cry yourself to sleep.
 		
 		:param: "fetch" must be a function which takes a key (from the evidence dictionary)
 		and returns a corresponding SourceText object.
 		"""
-		lines = ["%s while %s: %s"%(self.severity.name, self.phase, self.description)]
+		lines = ["%s while %s: %s"%(self.severity.value, self.phase, self.description)]
 		for key, evidence in self.evidence.items():
 			source = fetch(key)
 			if source.filename:
 				lines.append("Excerpt from "+source.filename+" :")
 			for e in evidence:
 				row, col = source.find_row_col(e.slice.start)
 				single_line = source.line_of_text(row)
```

### Comparing `booze-tools-0.6.1.0/boozetools/support/foundation.py` & `booze-tools-0.6.2.0/boozetools/support/foundation.py`

 * *Files identical despite different names*

### Comparing `booze-tools-0.6.1.0/boozetools/support/pretty.py` & `booze-tools-0.6.2.0/boozetools/support/pretty.py`

 * *Files identical despite different names*

### Comparing `booze-tools-0.6.1.0/boozetools/support/symtab.py` & `booze-tools-0.6.2.0/boozetools/support/symtab.py`

 * *Files identical despite different names*

### Comparing `booze-tools-0.6.1.0/boozetools/support/treelang.py` & `booze-tools-0.6.2.0/boozetools/support/treelang.py`

 * *Files identical despite different names*

### Comparing `booze-tools-0.6.1.0/setup.py` & `booze-tools-0.6.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
 	name='booze-tools',
-	version='0.6.1.0',
+	version='0.6.2.0',
 	packages=[
 		'boozetools',
 		'boozetools.macroparse',
 		'boozetools.parsing',
 		'boozetools.parsing.general',
 		'boozetools.scanning',
 		'boozetools.support',
```

