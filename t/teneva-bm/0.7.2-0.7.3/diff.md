# Comparing `tmp/teneva_bm-0.7.2.tar.gz` & `tmp/teneva_bm-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teneva_bm-0.7.2.tar", last modified: Sun Aug  6 12:05:58 2023, max compression
+gzip compressed data, was "teneva_bm-0.7.3.tar", last modified: Sun Aug  6 12:32:04 2023, max compression
```

## Comparing `teneva_bm-0.7.2.tar` & `teneva_bm-0.7.3.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:05:58.877107 teneva_bm-0.7.2/
--rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:29:59.000000 teneva_bm-0.7.2/LICENSE.txt
--rw-r--r--   0 andrei     (501) staff       (20)       79 2023-07-27 07:17:23.000000 teneva_bm-0.7.2/MANIFEST.in
--rw-r--r--   0 andrei     (501) staff       (20)    19872 2023-08-06 12:05:58.877315 teneva_bm-0.7.2/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)    18611 2023-08-06 12:04:15.000000 teneva_bm-0.7.2/README.md
--rw-r--r--   0 andrei     (501) staff       (20)      899 2023-07-29 14:29:03.000000 teneva_bm-0.7.2/demo.py
--rw-r--r--   0 andrei     (501) staff       (20)       33 2023-07-29 13:15:53.000000 teneva_bm-0.7.2/requirements.txt
--rw-r--r--   0 andrei     (501) staff       (20)      107 2023-08-06 12:05:58.878231 teneva_bm-0.7.2/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)     2518 2023-07-16 14:04:06.000000 teneva_bm-0.7.2/setup.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:05:58.833621 teneva_bm-0.7.2/teneva_bm/
--rw-r--r--   0 andrei     (501) staff       (20)      211 2023-08-06 12:04:10.000000 teneva_bm-0.7.2/teneva_bm/__init__.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:05:58.844985 teneva_bm-0.7.2/teneva_bm/agent/
--rw-r--r--   0 andrei     (501) staff       (20)      452 2023-08-06 10:02:09.000000 teneva_bm-0.7.2/teneva_bm/agent/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     7615 2023-08-06 09:59:09.000000 teneva_bm-0.7.2/teneva_bm/agent/agent.py
--rw-r--r--   0 andrei     (501) staff       (20)     2076 2023-07-30 16:06:42.000000 teneva_bm-0.7.2/teneva_bm/agent/bm_agent_ant.py
--rw-r--r--   0 andrei     (501) staff       (20)     2114 2023-08-04 11:40:40.000000 teneva_bm-0.7.2/teneva_bm/agent/bm_agent_cheetah.py
--rw-r--r--   0 andrei     (501) staff       (20)     2092 2023-07-30 15:54:04.000000 teneva_bm-0.7.2/teneva_bm/agent/bm_agent_human.py
--rw-r--r--   0 andrei     (501) staff       (20)     2139 2023-07-30 15:53:56.000000 teneva_bm-0.7.2/teneva_bm/agent/bm_agent_human_stand.py
--rw-r--r--   0 andrei     (501) staff       (20)     7445 2023-08-06 09:58:29.000000 teneva_bm-0.7.2/teneva_bm/agent/bm_agent_lake.py
--rw-r--r--   0 andrei     (501) staff       (20)     2258 2023-08-06 11:17:21.000000 teneva_bm-0.7.2/teneva_bm/agent/bm_agent_lander.py
--rw-r--r--   0 andrei     (501) staff       (20)     2136 2023-07-30 16:47:47.000000 teneva_bm-0.7.2/teneva_bm/agent/bm_agent_pend_inv.py
--rw-r--r--   0 andrei     (501) staff       (20)     2185 2023-07-30 16:47:42.000000 teneva_bm-0.7.2/teneva_bm/agent/bm_agent_pend_inv_double.py
--rw-r--r--   0 andrei     (501) staff       (20)     2100 2023-08-04 11:48:23.000000 teneva_bm-0.7.2/teneva_bm/agent/bm_agent_reacher.py
--rw-r--r--   0 andrei     (501) staff       (20)     2288 2023-07-30 15:24:14.000000 teneva_bm-0.7.2/teneva_bm/agent/bm_agent_swimmer.py
--rw-r--r--   0 andrei     (501) staff       (20)     3323 2023-07-30 15:46:50.000000 teneva_bm-0.7.2/teneva_bm/agent/policy.py
--rw-r--r--   0 andrei     (501) staff       (20)    35400 2023-08-04 13:13:26.000000 teneva_bm-0.7.2/teneva_bm/bm.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:05:58.853047 teneva_bm-0.7.2/teneva_bm/func/
--rw-r--r--   0 andrei     (501) staff       (20)      516 2023-07-13 07:42:30.000000 teneva_bm-0.7.2/teneva_bm/func/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     3641 2023-08-02 10:12:25.000000 teneva_bm-0.7.2/teneva_bm/func/bm_func_ackley.py
--rw-r--r--   0 andrei     (501) staff       (20)     2301 2023-07-30 10:08:14.000000 teneva_bm-0.7.2/teneva_bm/func/bm_func_alpine.py
--rw-r--r--   0 andrei     (501) staff       (20)     2430 2023-07-30 10:52:13.000000 teneva_bm-0.7.2/teneva_bm/func/bm_func_dixon.py
--rw-r--r--   0 andrei     (501) staff       (20)     2295 2023-07-30 10:52:30.000000 teneva_bm-0.7.2/teneva_bm/func/bm_func_exp.py
--rw-r--r--   0 andrei     (501) staff       (20)     2746 2023-07-30 10:13:15.000000 teneva_bm-0.7.2/teneva_bm/func/bm_func_griewank.py
--rw-r--r--   0 andrei     (501) staff       (20)     3623 2023-08-02 10:10:43.000000 teneva_bm-0.7.2/teneva_bm/func/bm_func_michalewicz.py
--rw-r--r--   0 andrei     (501) staff       (20)     2421 2023-07-30 10:17:40.000000 teneva_bm-0.7.2/teneva_bm/func/bm_func_piston.py
--rw-r--r--   0 andrei     (501) staff       (20)     2478 2023-07-30 10:55:11.000000 teneva_bm-0.7.2/teneva_bm/func/bm_func_qing.py
--rw-r--r--   0 andrei     (501) staff       (20)     3130 2023-08-02 10:10:09.000000 teneva_bm-0.7.2/teneva_bm/func/bm_func_rastrigin.py
--rw-r--r--   0 andrei     (501) staff       (20)     3155 2023-07-30 10:56:44.000000 teneva_bm-0.7.2/teneva_bm/func/bm_func_rosenbrock.py
--rw-r--r--   0 andrei     (501) staff       (20)     2129 2023-07-30 10:56:51.000000 teneva_bm-0.7.2/teneva_bm/func/bm_func_schaffer.py
--rw-r--r--   0 andrei     (501) staff       (20)     3165 2023-08-02 10:10:07.000000 teneva_bm-0.7.2/teneva_bm/func/bm_func_schwefel.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:05:58.854750 teneva_bm-0.7.2/teneva_bm/hs/
--rw-r--r--   0 andrei     (501) staff       (20)       78 2023-07-17 21:02:17.000000 teneva_bm-0.7.2/teneva_bm/hs/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     1755 2023-07-30 11:13:53.000000 teneva_bm-0.7.2/teneva_bm/hs/bm_hs_func001.py
--rw-r--r--   0 andrei     (501) staff       (20)     2430 2023-07-30 11:26:02.000000 teneva_bm-0.7.2/teneva_bm/hs/bm_hs_func006.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:05:58.860406 teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/
--rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     2272 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/bm_hs007.py
--rw-r--r--   0 andrei     (501) staff       (20)     2459 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/bm_hs008.py
--rw-r--r--   0 andrei     (501) staff       (20)     2318 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/bm_hs009.py
--rw-r--r--   0 andrei     (501) staff       (20)     2266 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/bm_hs010.py
--rw-r--r--   0 andrei     (501) staff       (20)     2251 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/bm_hs011.py
--rw-r--r--   0 andrei     (501) staff       (20)     2376 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/bm_hs012.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:05:58.868365 teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/
--rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     1937 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py
--rw-r--r--   0 andrei     (501) staff       (20)     1857 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py
--rw-r--r--   0 andrei     (501) staff       (20)     1839 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py
--rw-r--r--   0 andrei     (501) staff       (20)     2197 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py
--rw-r--r--   0 andrei     (501) staff       (20)     2275 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py
--rw-r--r--   0 andrei     (501) staff       (20)     1929 2023-07-17 20:25:36.000000 teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:05:58.871395 teneva_bm-0.7.2/teneva_bm/odeoc/
--rw-r--r--   0 andrei     (501) staff       (20)       99 2023-07-30 11:32:37.000000 teneva_bm-0.7.2/teneva_bm/odeoc/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     4218 2023-08-02 10:06:50.000000 teneva_bm-0.7.2/teneva_bm/odeoc/bm_odeoc_simple.py
--rw-r--r--   0 andrei     (501) staff       (20)     2292 2023-07-30 11:37:44.000000 teneva_bm-0.7.2/teneva_bm/odeoc/bm_odeoc_simple_constr.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:05:58.874750 teneva_bm-0.7.2/teneva_bm/qubo/
--rw-r--r--   0 andrei     (501) staff       (20)      166 2023-07-22 15:44:37.000000 teneva_bm-0.7.2/teneva_bm/qubo/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     7111 2023-07-30 11:04:30.000000 teneva_bm-0.7.2/teneva_bm/qubo/bm_qubo_knap_det.py
--rw-r--r--   0 andrei     (501) staff       (20)     1834 2023-07-30 11:06:13.000000 teneva_bm-0.7.2/teneva_bm/qubo/bm_qubo_knap_quad.py
--rw-r--r--   0 andrei     (501) staff       (20)     2782 2023-08-06 12:03:27.000000 teneva_bm-0.7.2/teneva_bm/qubo/bm_qubo_maxcut.py
--rw-r--r--   0 andrei     (501) staff       (20)     2845 2023-08-06 12:01:41.000000 teneva_bm-0.7.2/teneva_bm/qubo/bm_qubo_mvc.py
--rw-r--r--   0 andrei     (501) staff       (20)     3377 2023-07-29 14:31:04.000000 teneva_bm-0.7.2/teneva_bm/teneva_bm_demo.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:05:58.876677 teneva_bm-0.7.2/teneva_bm/various/
--rw-r--r--   0 andrei     (501) staff       (20)      105 2023-07-13 07:41:21.000000 teneva_bm-0.7.2/teneva_bm/various/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     7774 2023-08-02 10:24:54.000000 teneva_bm-0.7.2/teneva_bm/various/bm_matmul.py
--rw-r--r--   0 andrei     (501) staff       (20)    12683 2023-08-02 10:23:16.000000 teneva_bm-0.7.2/teneva_bm/various/bm_topopt.py
--rw-r--r--   0 andrei     (501) staff       (20)     1867 2023-07-30 11:18:40.000000 teneva_bm-0.7.2/teneva_bm/various/bm_wall_simple.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:05:58.837409 teneva_bm-0.7.2/teneva_bm.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)    19872 2023-08-06 12:05:58.000000 teneva_bm-0.7.2/teneva_bm.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     2419 2023-08-06 12:05:58.000000 teneva_bm-0.7.2/teneva_bm.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2023-08-06 12:05:58.000000 teneva_bm-0.7.2/teneva_bm.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)       33 2023-08-06 12:05:58.000000 teneva_bm-0.7.2/teneva_bm.egg-info/requires.txt
--rw-r--r--   0 andrei     (501) staff       (20)       10 2023-08-06 12:05:58.000000 teneva_bm-0.7.2/teneva_bm.egg-info/top_level.txt
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:32:04.259304 teneva_bm-0.7.3/
+-rw-r--r--   0 andrei     (501) staff       (20)     1090 2023-02-25 19:29:59.000000 teneva_bm-0.7.3/LICENSE.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       79 2023-07-27 07:17:23.000000 teneva_bm-0.7.3/MANIFEST.in
+-rw-r--r--   0 andrei     (501) staff       (20)    19872 2023-08-06 12:32:04.259581 teneva_bm-0.7.3/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)    18611 2023-08-06 12:29:10.000000 teneva_bm-0.7.3/README.md
+-rw-r--r--   0 andrei     (501) staff       (20)      899 2023-07-29 14:29:03.000000 teneva_bm-0.7.3/demo.py
+-rw-r--r--   0 andrei     (501) staff       (20)       33 2023-07-29 13:15:53.000000 teneva_bm-0.7.3/requirements.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      107 2023-08-06 12:32:04.260793 teneva_bm-0.7.3/setup.cfg
+-rw-r--r--   0 andrei     (501) staff       (20)     2518 2023-07-16 14:04:06.000000 teneva_bm-0.7.3/setup.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:32:04.205938 teneva_bm-0.7.3/teneva_bm/
+-rw-r--r--   0 andrei     (501) staff       (20)      211 2023-08-06 12:29:03.000000 teneva_bm-0.7.3/teneva_bm/__init__.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:32:04.217263 teneva_bm-0.7.3/teneva_bm/agent/
+-rw-r--r--   0 andrei     (501) staff       (20)      452 2023-08-06 10:02:09.000000 teneva_bm-0.7.3/teneva_bm/agent/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7615 2023-08-06 09:59:09.000000 teneva_bm-0.7.3/teneva_bm/agent/agent.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2076 2023-07-30 16:06:42.000000 teneva_bm-0.7.3/teneva_bm/agent/bm_agent_ant.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2114 2023-08-04 11:40:40.000000 teneva_bm-0.7.3/teneva_bm/agent/bm_agent_cheetah.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2092 2023-07-30 15:54:04.000000 teneva_bm-0.7.3/teneva_bm/agent/bm_agent_human.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2139 2023-07-30 15:53:56.000000 teneva_bm-0.7.3/teneva_bm/agent/bm_agent_human_stand.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7445 2023-08-06 09:58:29.000000 teneva_bm-0.7.3/teneva_bm/agent/bm_agent_lake.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2258 2023-08-06 11:17:21.000000 teneva_bm-0.7.3/teneva_bm/agent/bm_agent_lander.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2136 2023-07-30 16:47:47.000000 teneva_bm-0.7.3/teneva_bm/agent/bm_agent_pend_inv.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2185 2023-07-30 16:47:42.000000 teneva_bm-0.7.3/teneva_bm/agent/bm_agent_pend_inv_double.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2100 2023-08-04 11:48:23.000000 teneva_bm-0.7.3/teneva_bm/agent/bm_agent_reacher.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2288 2023-07-30 15:24:14.000000 teneva_bm-0.7.3/teneva_bm/agent/bm_agent_swimmer.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3323 2023-07-30 15:46:50.000000 teneva_bm-0.7.3/teneva_bm/agent/policy.py
+-rw-r--r--   0 andrei     (501) staff       (20)    35400 2023-08-04 13:13:26.000000 teneva_bm-0.7.3/teneva_bm/bm.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:32:04.223256 teneva_bm-0.7.3/teneva_bm/func/
+-rw-r--r--   0 andrei     (501) staff       (20)      516 2023-07-13 07:42:30.000000 teneva_bm-0.7.3/teneva_bm/func/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3641 2023-08-02 10:12:25.000000 teneva_bm-0.7.3/teneva_bm/func/bm_func_ackley.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2301 2023-07-30 10:08:14.000000 teneva_bm-0.7.3/teneva_bm/func/bm_func_alpine.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2430 2023-07-30 10:52:13.000000 teneva_bm-0.7.3/teneva_bm/func/bm_func_dixon.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2295 2023-07-30 10:52:30.000000 teneva_bm-0.7.3/teneva_bm/func/bm_func_exp.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2746 2023-07-30 10:13:15.000000 teneva_bm-0.7.3/teneva_bm/func/bm_func_griewank.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3623 2023-08-02 10:10:43.000000 teneva_bm-0.7.3/teneva_bm/func/bm_func_michalewicz.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2421 2023-07-30 10:17:40.000000 teneva_bm-0.7.3/teneva_bm/func/bm_func_piston.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2478 2023-07-30 10:55:11.000000 teneva_bm-0.7.3/teneva_bm/func/bm_func_qing.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3130 2023-08-02 10:10:09.000000 teneva_bm-0.7.3/teneva_bm/func/bm_func_rastrigin.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3155 2023-07-30 10:56:44.000000 teneva_bm-0.7.3/teneva_bm/func/bm_func_rosenbrock.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2129 2023-07-30 10:56:51.000000 teneva_bm-0.7.3/teneva_bm/func/bm_func_schaffer.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3165 2023-08-02 10:10:07.000000 teneva_bm-0.7.3/teneva_bm/func/bm_func_schwefel.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:32:04.224561 teneva_bm-0.7.3/teneva_bm/hs/
+-rw-r--r--   0 andrei     (501) staff       (20)       78 2023-07-17 21:02:17.000000 teneva_bm-0.7.3/teneva_bm/hs/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1755 2023-07-30 11:13:53.000000 teneva_bm-0.7.3/teneva_bm/hs/bm_hs_func001.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2430 2023-07-30 11:26:02.000000 teneva_bm-0.7.3/teneva_bm/hs/bm_hs_func006.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:32:04.227928 teneva_bm-0.7.3/teneva_bm/hs/draft_constrained_functions/
+-rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.7.3/teneva_bm/hs/draft_constrained_functions/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2272 2023-07-17 20:25:36.000000 teneva_bm-0.7.3/teneva_bm/hs/draft_constrained_functions/bm_hs007.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2459 2023-07-17 20:25:36.000000 teneva_bm-0.7.3/teneva_bm/hs/draft_constrained_functions/bm_hs008.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2318 2023-07-17 20:25:36.000000 teneva_bm-0.7.3/teneva_bm/hs/draft_constrained_functions/bm_hs009.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2266 2023-07-17 20:25:36.000000 teneva_bm-0.7.3/teneva_bm/hs/draft_constrained_functions/bm_hs010.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2251 2023-07-17 20:25:36.000000 teneva_bm-0.7.3/teneva_bm/hs/draft_constrained_functions/bm_hs011.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2376 2023-07-17 20:25:36.000000 teneva_bm-0.7.3/teneva_bm/hs/draft_constrained_functions/bm_hs012.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:32:04.231816 teneva_bm-0.7.3/teneva_bm/hs/draft_unconstrained_functions/
+-rw-r--r--   0 andrei     (501) staff       (20)      209 2023-07-17 20:25:36.000000 teneva_bm-0.7.3/teneva_bm/hs/draft_unconstrained_functions/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1937 2023-07-17 20:25:36.000000 teneva_bm-0.7.3/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1857 2023-07-17 20:25:36.000000 teneva_bm-0.7.3/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1839 2023-07-17 20:25:36.000000 teneva_bm-0.7.3/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2197 2023-07-17 20:25:36.000000 teneva_bm-0.7.3/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2275 2023-07-17 20:25:36.000000 teneva_bm-0.7.3/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1929 2023-07-17 20:25:36.000000 teneva_bm-0.7.3/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:32:04.253600 teneva_bm-0.7.3/teneva_bm/odeoc/
+-rw-r--r--   0 andrei     (501) staff       (20)       99 2023-07-30 11:32:37.000000 teneva_bm-0.7.3/teneva_bm/odeoc/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     4218 2023-08-02 10:06:50.000000 teneva_bm-0.7.3/teneva_bm/odeoc/bm_odeoc_simple.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2292 2023-07-30 11:37:44.000000 teneva_bm-0.7.3/teneva_bm/odeoc/bm_odeoc_simple_constr.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:32:04.256634 teneva_bm-0.7.3/teneva_bm/qubo/
+-rw-r--r--   0 andrei     (501) staff       (20)      166 2023-07-22 15:44:37.000000 teneva_bm-0.7.3/teneva_bm/qubo/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7111 2023-07-30 11:04:30.000000 teneva_bm-0.7.3/teneva_bm/qubo/bm_qubo_knap_det.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1834 2023-07-30 11:06:13.000000 teneva_bm-0.7.3/teneva_bm/qubo/bm_qubo_knap_quad.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2961 2023-08-06 12:28:25.000000 teneva_bm-0.7.3/teneva_bm/qubo/bm_qubo_maxcut.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3024 2023-08-06 12:28:27.000000 teneva_bm-0.7.3/teneva_bm/qubo/bm_qubo_mvc.py
+-rw-r--r--   0 andrei     (501) staff       (20)     3377 2023-07-29 14:31:04.000000 teneva_bm-0.7.3/teneva_bm/teneva_bm_demo.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:32:04.258850 teneva_bm-0.7.3/teneva_bm/various/
+-rw-r--r--   0 andrei     (501) staff       (20)      105 2023-07-13 07:41:21.000000 teneva_bm-0.7.3/teneva_bm/various/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     7774 2023-08-02 10:24:54.000000 teneva_bm-0.7.3/teneva_bm/various/bm_matmul.py
+-rw-r--r--   0 andrei     (501) staff       (20)    12683 2023-08-02 10:23:16.000000 teneva_bm-0.7.3/teneva_bm/various/bm_topopt.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1867 2023-07-30 11:18:40.000000 teneva_bm-0.7.3/teneva_bm/various/bm_wall_simple.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-08-06 12:32:04.209411 teneva_bm-0.7.3/teneva_bm.egg-info/
+-rw-r--r--   0 andrei     (501) staff       (20)    19872 2023-08-06 12:32:04.000000 teneva_bm-0.7.3/teneva_bm.egg-info/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     2419 2023-08-06 12:32:04.000000 teneva_bm-0.7.3/teneva_bm.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        1 2023-08-06 12:32:04.000000 teneva_bm-0.7.3/teneva_bm.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       33 2023-08-06 12:32:04.000000 teneva_bm-0.7.3/teneva_bm.egg-info/requires.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       10 2023-08-06 12:32:04.000000 teneva_bm-0.7.3/teneva_bm.egg-info/top_level.txt
```

### Comparing `teneva_bm-0.7.2/LICENSE.txt` & `teneva_bm-0.7.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/PKG-INFO` & `teneva_bm-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teneva_bm
-Version: 0.7.2
+Version: 0.7.3
 Summary: Benchmarks library, based on the software product teneva, for testing multivariate approximation and optimization methods
 Home-page: https://github.com/AndreiChertkov/teneva_bm
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_bm
 Keywords: benchmarks approximation optimization multidimensional array multivariate function low-rank representation tensor train format TT-decomposition
@@ -32,15 +32,15 @@
 Benchmarks library, based on the software product [teneva](https://github.com/AndreiChertkov/teneva), for testing multidimensional approximation and optimization methods. Our benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
 1. The package can be installed via pip (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9):
     ```bash
-    pip install teneva_bm==0.7.2
+    pip install teneva_bm==0.7.3
     ```
     > The package can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and be installed by `python setup.py install` command from the root folder of the project.
 
 2. Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the script [install_all.py](https://github.com/AndreiChertkov/teneva_bm/blob/main/install_all.py) for existing [anaconda](https://www.anaconda.com) environment `ENV_NAME` (except the colab platform, where `env` flag should not be used):
     ```bash
     conda create --name ENV_NAME python=3.8 -y
     wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_all.py
```

### Comparing `teneva_bm-0.7.2/README.md` & `teneva_bm-0.7.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Benchmarks library, based on the software product [teneva](https://github.com/AndreiChertkov/teneva), for testing multidimensional approximation and optimization methods. Our benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
 1. The package can be installed via pip (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9):
     ```bash
-    pip install teneva_bm==0.7.2
+    pip install teneva_bm==0.7.3
     ```
     > The package can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and be installed by `python setup.py install` command from the root folder of the project.
 
 2. Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the script [install_all.py](https://github.com/AndreiChertkov/teneva_bm/blob/main/install_all.py) for existing [anaconda](https://www.anaconda.com) environment `ENV_NAME` (except the colab platform, where `env` flag should not be used):
     ```bash
     conda create --name ENV_NAME python=3.8 -y
     wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_all.py
```

### Comparing `teneva_bm-0.7.2/demo.py` & `teneva_bm-0.7.3/demo.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/setup.py` & `teneva_bm-0.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/agent/agent.py` & `teneva_bm-0.7.3/teneva_bm/agent/agent.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/agent/bm_agent_ant.py` & `teneva_bm-0.7.3/teneva_bm/agent/bm_agent_ant.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/agent/bm_agent_cheetah.py` & `teneva_bm-0.7.3/teneva_bm/agent/bm_agent_cheetah.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/agent/bm_agent_human.py` & `teneva_bm-0.7.3/teneva_bm/agent/bm_agent_human.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/agent/bm_agent_human_stand.py` & `teneva_bm-0.7.3/teneva_bm/agent/bm_agent_human_stand.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/agent/bm_agent_lake.py` & `teneva_bm-0.7.3/teneva_bm/agent/bm_agent_lake.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/agent/bm_agent_lander.py` & `teneva_bm-0.7.3/teneva_bm/agent/bm_agent_lander.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/agent/bm_agent_pend_inv.py` & `teneva_bm-0.7.3/teneva_bm/agent/bm_agent_pend_inv.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/agent/bm_agent_pend_inv_double.py` & `teneva_bm-0.7.3/teneva_bm/agent/bm_agent_pend_inv_double.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/agent/bm_agent_reacher.py` & `teneva_bm-0.7.3/teneva_bm/agent/bm_agent_reacher.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/agent/bm_agent_swimmer.py` & `teneva_bm-0.7.3/teneva_bm/agent/bm_agent_swimmer.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/agent/policy.py` & `teneva_bm-0.7.3/teneva_bm/agent/policy.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/bm.py` & `teneva_bm-0.7.3/teneva_bm/bm.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/func/__init__.py` & `teneva_bm-0.7.3/teneva_bm/func/__init__.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/func/bm_func_ackley.py` & `teneva_bm-0.7.3/teneva_bm/func/bm_func_ackley.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/func/bm_func_alpine.py` & `teneva_bm-0.7.3/teneva_bm/func/bm_func_alpine.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/func/bm_func_dixon.py` & `teneva_bm-0.7.3/teneva_bm/func/bm_func_dixon.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/func/bm_func_exp.py` & `teneva_bm-0.7.3/teneva_bm/func/bm_func_exp.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/func/bm_func_griewank.py` & `teneva_bm-0.7.3/teneva_bm/func/bm_func_griewank.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/func/bm_func_michalewicz.py` & `teneva_bm-0.7.3/teneva_bm/func/bm_func_michalewicz.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/func/bm_func_piston.py` & `teneva_bm-0.7.3/teneva_bm/func/bm_func_piston.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/func/bm_func_qing.py` & `teneva_bm-0.7.3/teneva_bm/func/bm_func_qing.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/func/bm_func_rastrigin.py` & `teneva_bm-0.7.3/teneva_bm/func/bm_func_rastrigin.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/func/bm_func_rosenbrock.py` & `teneva_bm-0.7.3/teneva_bm/func/bm_func_rosenbrock.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/func/bm_func_schaffer.py` & `teneva_bm-0.7.3/teneva_bm/func/bm_func_schaffer.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/func/bm_func_schwefel.py` & `teneva_bm-0.7.3/teneva_bm/func/bm_func_schwefel.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/hs/bm_hs_func001.py` & `teneva_bm-0.7.3/teneva_bm/hs/bm_hs_func001.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/hs/bm_hs_func006.py` & `teneva_bm-0.7.3/teneva_bm/hs/bm_hs_func006.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/bm_hs007.py` & `teneva_bm-0.7.3/teneva_bm/hs/draft_constrained_functions/bm_hs007.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/bm_hs008.py` & `teneva_bm-0.7.3/teneva_bm/hs/draft_constrained_functions/bm_hs008.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/bm_hs009.py` & `teneva_bm-0.7.3/teneva_bm/hs/draft_constrained_functions/bm_hs009.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/bm_hs010.py` & `teneva_bm-0.7.3/teneva_bm/hs/draft_constrained_functions/bm_hs010.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/bm_hs011.py` & `teneva_bm-0.7.3/teneva_bm/hs/draft_constrained_functions/bm_hs011.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/hs/draft_constrained_functions/bm_hs012.py` & `teneva_bm-0.7.3/teneva_bm/hs/draft_constrained_functions/bm_hs012.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py` & `teneva_bm-0.7.3/teneva_bm/hs/draft_unconstrained_functions/bm_hs002.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py` & `teneva_bm-0.7.3/teneva_bm/hs/draft_unconstrained_functions/bm_hs003.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py` & `teneva_bm-0.7.3/teneva_bm/hs/draft_unconstrained_functions/bm_hs004.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py` & `teneva_bm-0.7.3/teneva_bm/hs/draft_unconstrained_functions/bm_hs005.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py` & `teneva_bm-0.7.3/teneva_bm/hs/draft_unconstrained_functions/bm_hs038.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py` & `teneva_bm-0.7.3/teneva_bm/hs/draft_unconstrained_functions/bm_hs045.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/odeoc/bm_odeoc_simple.py` & `teneva_bm-0.7.3/teneva_bm/odeoc/bm_odeoc_simple.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/odeoc/bm_odeoc_simple_constr.py` & `teneva_bm-0.7.3/teneva_bm/odeoc/bm_odeoc_simple_constr.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/qubo/bm_qubo_knap_det.py` & `teneva_bm-0.7.3/teneva_bm/qubo/bm_qubo_knap_det.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/qubo/bm_qubo_knap_quad.py` & `teneva_bm-0.7.3/teneva_bm/qubo/bm_qubo_knap_quad.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/qubo/bm_qubo_maxcut.py` & `teneva_bm-0.7.3/teneva_bm/qubo/bm_qubo_maxcut.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 from teneva_bm import Bm
 
 
 DESC = """
     Quadratic unconstrained binary optimization (QUBO) Max-Cut problem
     represented as a discrete function. The dimension may be any (default
     is 100), and the mode size should be 2. The default value of the
-    probability of the connection in the graph if 0.5 (pcon). The benchmark
-    needs "networkx==3.0" and "qubogen==0.1.1" libraries.
+    probability of the connection in the graph if 0.5 (pcon=5).
+    The benchmark needs "networkx==3.0" and "qubogen==0.1.1" libraries.
 """
 
 
 class BmQuboMaxcut(Bm):
-    def __init__(self, d=100, n=2, name='QuboMaxcut', desc=DESC, pcon=0.5):
+    def __init__(self, d=100, n=2, name='QuboMaxcut', desc=DESC, pcon=5):
         super().__init__(d, n, name, desc)
 
         if not self.is_n_equal or self.n0 != 2:
             self.set_err('Mode size (n) should be "2"')
 
         if not with_networkx:
             msg = 'Need "networkx" module. For installation please run '
@@ -40,14 +40,18 @@
             self.set_err(msg)
 
         if not with_qubogen:
             msg = 'Need "qubogen" module. For installation please run '
             msg += '"pip install qubogen==0.1.1"'
             self.set_err(msg)
 
+        if not isinstance(pcon, int) or pcon < 1 or pcon > 9:
+            msg = 'Param "pcon" should be of int type and in range 1...9'
+            self.set_err(msg)
+
         self.pcon = pcon
 
     @property
     def identity(self):
         return ['d', 'pcon', 'seed']
 
     @property
@@ -59,22 +63,22 @@
         conf['pcon'] = self.pcon
         return conf
 
     def info(self, footer=''):
         text = ''
 
         text += 'Param pcon (connection probability)      : '
-        v = self.pcon
+        v = 0.1 * self.pcon
         text += f'{v:.6f}\n'
 
         return super().info(text+footer)
 
     def prep_bm(self):
         d = self.d
-        p = self.pcon
+        p = 0.1 * self.pcon
         graph = nx.fast_gnp_random_graph(n=d, p=p, seed=self.seed)
         edges = np.array(list([list(e) for e in graph.edges]))
         n_nodes = len(np.unique(np.array(edges).flatten()))
 
         g = qubogen.Graph(edges=edges, n_nodes=n_nodes)
         self._Q = qubogen.qubo_max_cut(g)
```

### Comparing `teneva_bm-0.7.2/teneva_bm/qubo/bm_qubo_mvc.py` & `teneva_bm-0.7.3/teneva_bm/qubo/bm_qubo_mvc.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 from teneva_bm import Bm
 
 
 DESC = """
     Quadratic unconstrained binary optimization (QUBO) Minimum Vertex Cover
     (MVC) problem represented as a discrete function. The dimension may be
     any (default is 100), and the mode size should be 2. The default value
-    of the probability of the connection in the graph if 0.5 (pcon).
+    of the probability of the connection in the graph if 0.5 (pcon=5).
     The benchmark needs "networkx==3.0" and "qubogen==0.1.1" libraries.
     TODO: fix inner bm name from "QuboMVC" to "QuboMvc".
 """
 
 
 class BmQuboMvc(Bm):
-    def __init__(self, d=100, n=2, name='QuboMVC', desc=DESC, pcon=0.5):
+    def __init__(self, d=100, n=2, name='QuboMVC', desc=DESC, pcon=5):
         super().__init__(d, n, name, desc)
 
         if not self.is_n_equal or self.n0 != 2:
             self.set_err('Mode size (n) should be "2"')
 
         if not with_networkx:
             msg = 'Need "networkx" module. For installation please run '
@@ -41,14 +41,18 @@
             self.set_err(msg)
 
         if not with_qubogen:
             msg = 'Need "qubogen" module. For installation please run '
             msg += '"pip install qubogen==0.1.1"'
             self.set_err(msg)
 
+        if not isinstance(pcon, int) or pcon < 1 or pcon > 9:
+            msg = 'Param "pcon" should be of int type and in range 1...9'
+            self.set_err(msg)
+
         self.pcon = pcon
 
     @property
     def identity(self):
         return ['d', 'pcon', 'seed']
 
     @property
@@ -60,22 +64,22 @@
         conf['pcon'] = self.pcon
         return conf
 
     def info(self, footer=''):
         text = ''
 
         text += 'Param pcon (connection probability)      : '
-        v = self.pcon
+        v = 0.1 * self.pcon
         text += f'{v:.6f}\n'
 
         return super().info(text+footer)
 
     def prep_bm(self):
         d = self.d
-        p = self.pcon
+        p = 0.1 * self.pcon
         graph = nx.fast_gnp_random_graph(n=d, p=p, seed=self.seed)
         edges = np.array(list([list(e) for e in graph.edges]))
         n_nodes = len(np.unique(np.array(edges).flatten()))
 
         g = qubogen.Graph(edges=edges, n_nodes=n_nodes)
         self._Q = qubogen.qubo_mvc(g)
```

### Comparing `teneva_bm-0.7.2/teneva_bm/teneva_bm_demo.py` & `teneva_bm-0.7.3/teneva_bm/teneva_bm_demo.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/various/bm_matmul.py` & `teneva_bm-0.7.3/teneva_bm/various/bm_matmul.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/various/bm_topopt.py` & `teneva_bm-0.7.3/teneva_bm/various/bm_topopt.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm/various/bm_wall_simple.py` & `teneva_bm-0.7.3/teneva_bm/various/bm_wall_simple.py`

 * *Files identical despite different names*

### Comparing `teneva_bm-0.7.2/teneva_bm.egg-info/PKG-INFO` & `teneva_bm-0.7.3/teneva_bm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teneva-bm
-Version: 0.7.2
+Version: 0.7.3
 Summary: Benchmarks library, based on the software product teneva, for testing multivariate approximation and optimization methods
 Home-page: https://github.com/AndreiChertkov/teneva_bm
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AndreiChertkov/teneva_bm
 Keywords: benchmarks approximation optimization multidimensional array multivariate function low-rank representation tensor train format TT-decomposition
@@ -32,15 +32,15 @@
 Benchmarks library, based on the software product [teneva](https://github.com/AndreiChertkov/teneva), for testing multidimensional approximation and optimization methods. Our benchmarks include both multidimensional data arrays and discretized functions of many variables.
 
 
 ## Installation
 
 1. The package can be installed via pip (it requires the [Python](https://www.python.org) programming language of the version 3.8 or 3.9):
     ```bash
-    pip install teneva_bm==0.7.2
+    pip install teneva_bm==0.7.3
     ```
     > The package can be also downloaded from the repository [teneva_bm](https://github.com/AndreiChertkov/teneva_bm) and be installed by `python setup.py install` command from the root folder of the project.
 
 2. Some benchmarks require additional installation of specialized libraries. The corresponding instructions are given in the description of each benchmark (see `DESC` string in the python files with benchmarks). Installation of all required libraries for all benchmarks can be done with the script [install_all.py](https://github.com/AndreiChertkov/teneva_bm/blob/main/install_all.py) for existing [anaconda](https://www.anaconda.com) environment `ENV_NAME` (except the colab platform, where `env` flag should not be used):
     ```bash
     conda create --name ENV_NAME python=3.8 -y
     wget https://raw.githubusercontent.com/AndreiChertkov/teneva_bm/main/install_all.py
```

### Comparing `teneva_bm-0.7.2/teneva_bm.egg-info/SOURCES.txt` & `teneva_bm-0.7.3/teneva_bm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

