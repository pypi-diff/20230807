# Comparing `tmp/eef-data-0.52.tar.gz` & `tmp/eef-data-0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eef-data-0.52.tar", last modified: Wed Jul 19 00:21:04 2023, max compression
+gzip compressed data, was "eef-data-0.53.tar", last modified: Mon Aug  7 15:31:25 2023, max compression
```

## Comparing `eef-data-0.52.tar` & `eef-data-0.53.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-19 00:21:04.869304 eef-data-0.52/
--rw-rw-r--   0 linux     (1000) linux     (1000)     1073 2023-05-04 23:15:45.000000 eef-data-0.52/LICENSE
--rw-rw-r--   0 linux     (1000) linux     (1000)       41 2023-07-19 00:05:55.000000 eef-data-0.52/MANIFEST.in
--rw-rw-r--   0 linux     (1000) linux     (1000)    62840 2023-07-19 00:21:04.869304 eef-data-0.52/PKG-INFO
--rw-rw-r--   0 linux     (1000) linux     (1000)    64622 2023-07-18 23:21:55.000000 eef-data-0.52/README.md
--rwxrwxrwx   0 linux     (1000) linux     (1000)    62627 2023-07-18 23:33:52.000000 eef-data-0.52/README_package.md
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-19 00:21:04.869304 eef-data-0.52/eef_data.egg-info/
--rw-rw-r--   0 linux     (1000) linux     (1000)    62840 2023-07-19 00:21:04.000000 eef-data-0.52/eef_data.egg-info/PKG-INFO
--rw-rw-r--   0 linux     (1000) linux     (1000)      358 2023-07-19 00:21:04.000000 eef-data-0.52/eef_data.egg-info/SOURCES.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)        1 2023-07-19 00:21:04.000000 eef-data-0.52/eef_data.egg-info/dependency_links.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)       47 2023-07-19 00:21:04.000000 eef-data-0.52/eef_data.egg-info/entry_points.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)       78 2023-07-19 00:21:04.000000 eef-data-0.52/eef_data.egg-info/requires.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)        8 2023-07-19 00:21:04.000000 eef-data-0.52/eef_data.egg-info/top_level.txt
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-19 00:21:04.869304 eef-data-0.52/eefdata/
--rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:41.000000 eef-data-0.52/eefdata/__init__.py
--rw-rw-r--   0 linux     (1000) linux     (1000)   165256 2023-07-19 00:18:46.000000 eef-data-0.52/eefdata/app.py
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-07-19 00:21:04.869304 eef-data-0.52/eefdata/src/
--rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-03-17 12:41:42.000000 eef-data-0.52/eefdata/src/__init__.py
--rw-rw-r--   0 linux     (1000) linux     (1000)   151479 2023-07-18 18:50:53.000000 eef-data-0.52/eefdata/src/attributeIDs.py
--rw-rw-r--   0 linux     (1000) linux     (1000)   263012 2023-07-19 00:19:34.000000 eef-data-0.52/eefdata/src/funcs.py
--rw-rw-r--   0 linux     (1000) linux     (1000)       38 2023-07-19 00:21:04.869304 eef-data-0.52/setup.cfg
--rw-rw-r--   0 linux     (1000) linux     (1000)      771 2023-07-19 00:20:28.000000 eef-data-0.52/setup.py
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-08-07 15:31:25.792342 eef-data-0.53/
+-rw-rw-r--   0 linux     (1000) linux     (1000)     1073 2023-08-07 15:21:56.000000 eef-data-0.53/LICENSE
+-rw-rw-r--   0 linux     (1000) linux     (1000)       41 2023-08-07 15:21:56.000000 eef-data-0.53/MANIFEST.in
+-rw-rw-r--   0 linux     (1000) linux     (1000)    67256 2023-08-07 15:31:25.792342 eef-data-0.53/PKG-INFO
+-rw-rw-r--   0 linux     (1000) linux     (1000)    66890 2023-08-07 15:21:56.000000 eef-data-0.53/README.md
+-rwxrwxrwx   0 linux     (1000) linux     (1000)    67043 2023-08-07 15:30:14.000000 eef-data-0.53/README_package.md
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-08-07 15:31:25.788342 eef-data-0.53/eef_data.egg-info/
+-rw-rw-r--   0 linux     (1000) linux     (1000)    67256 2023-08-07 15:31:25.000000 eef-data-0.53/eef_data.egg-info/PKG-INFO
+-rw-rw-r--   0 linux     (1000) linux     (1000)      358 2023-08-07 15:31:25.000000 eef-data-0.53/eef_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)        1 2023-08-07 15:31:25.000000 eef-data-0.53/eef_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)       47 2023-08-07 15:31:25.000000 eef-data-0.53/eef_data.egg-info/entry_points.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)       78 2023-08-07 15:31:25.000000 eef-data-0.53/eef_data.egg-info/requires.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)        8 2023-08-07 15:31:25.000000 eef-data-0.53/eef_data.egg-info/top_level.txt
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-08-07 15:31:25.788342 eef-data-0.53/eefdata/
+-rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-08-07 15:21:56.000000 eef-data-0.53/eefdata/__init__.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)   182007 2023-08-07 15:21:56.000000 eef-data-0.53/eefdata/app.py
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2023-08-07 15:31:25.788342 eef-data-0.53/eefdata/src/
+-rw-rw-r--   0 linux     (1000) linux     (1000)        0 2023-08-07 15:21:56.000000 eef-data-0.53/eefdata/src/__init__.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)   151479 2023-08-07 15:21:56.000000 eef-data-0.53/eefdata/src/attributeIDs.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)   263357 2023-08-07 15:21:56.000000 eef-data-0.53/eefdata/src/funcs.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)       38 2023-08-07 15:31:25.792342 eef-data-0.53/setup.cfg
+-rw-rw-r--   0 linux     (1000) linux     (1000)      771 2023-08-07 15:28:26.000000 eef-data-0.53/setup.py
```

### Comparing `eef-data-0.52/LICENSE` & `eef-data-0.53/LICENSE`

 * *Files identical despite different names*

### Comparing `eef-data-0.52/PKG-INFO` & `eef-data-0.53/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eef-data
-Version: 0.52
+Version: 0.53
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.10.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -708,44 +708,42 @@
 | `URL`            | `raw`     | `url`            |
 | `Publisher`      | `raw`     | `publisher`      |
 | `City`           | `raw`     | `city`           |
 | `Institution`    | `raw`     | `institution`    |
 
 </details>
 
-## Custom Dataframe Selection
+## Custom Column Selection
 
-This dataframe consists of the data the user chooses from a pre-defined column list.
+Custom column selections consist of the data the user chooses from a pre-defined list of column options.
 
 | Data Type   | Description                           | Number of Columns   |
 | ----------- | ------------------------------------- | :-----------------: |
-|  `_raw`     | raw data as input by the data coders  | 119                 |
-|  `_ht`      | text highlighted from the manuscript  | 19                  |
-|  `_info`    | any 'user' entered info               | 19                  |
+|  `_raw`     | raw data as input by the data coders  | 127                 |
+|  `_ht`      | text highlighted from the manuscript  | 43                 |
+|  `_info`    | any 'user' entered info               | 43                  |
 | `_CLEAN`    | empty columns for data cleaning notes | 0                   |
-|             | **Total Number of Columns**           | **157**<sup>1</sup> |
+|             | **Total Number of Columns**           | **213**<sup>1</sup> |
 
-<sup>1</sup>157 is the maximum number of columns where are all data are selected.
+<sup>1</sup>213 is the maximum number of columns where are all data are selected.
 
 <details>
 <summary>Custom Dataframe Selection Column Summary</summary>
 
 | Variable                                    | Data Type | Column Name         |
 | ------------------------------------------- | --------- | ------------------- |
-| `Eppi ID`                                   | `raw`     | `id`                |
+| `Study ID`                                   | `raw`     | `id`                |
 | `Publication Author`                        | `raw`     | `pub_author`        |
 | `Publication Year`                          | `raw`     | `pub_year`          |
 | `Abstract`                                  | `raw`     | `abstract`          |
 | `Strand`                                    | `raw`     | `strand_raw`        |
 | `Country`                                   | `raw`     | `loc_country_raw`   |
 | `Publication Type (EPPI)`                   | `raw`     | `pub_eppi`          |
 | `Publication Type`                          | `raw`     | `pub_type_raw`      |
-| `Educational Setting`                       | `raw`     | `int_setting_raw`   |
 | `Participant Age`                           | `raw`     | `part_age_raw`      |
-| `REPLACE`                                   | `REPLACE` | `REPLACE`           |
 | `Ecological Validity`                       | `raw`     | `eco_valid_raw`     |
 | `Intervention Number of Schools (info)`     | `info`    | `school_treat_info` |
 | `Intervention Number of Schools (ht)`       | `ht`      | `school_treat_ht`   |
 | `Control Number of Schools (info)`          | `info`    | `school_cont_info`  |
 | `Control Number of Schools (ht)`            | `ht`      | `school_cont_ht`    |
 | `Total Number of Schools (info)`            | `info`    | `school_total_info` |
 | `Total Number of Schools (ht)`              | `ht`      | `school_total_ht`   |
@@ -795,30 +793,30 @@
 | `Reading Outcome Group1 Mean`               | `raw`  | `out_g1_mean_red`    |
 | `Reading Outcome Group1 SD`                 | `raw`  | `out_g1_sd_red`      |
 | `Reading Outcome Group2 N`                  | `raw`  | `out_g2_n_red`       |
 | `Reading Outcome Group2 Mean`               | `raw`  | `out_g2_mean_red`    |
 | `Reading Outcome Group2 SD`                 | `raw`  | `out_g2_sd_red`      |
 | `Reading Outcome Test Type`                 | `raw`  | `out_test_type_raw_red` |
 | `Reading Outcome Effect Size Type`          | `raw`  | `out_es_type_red`    |
-| `Writnig Outcome Title`                     | `raw`  | `out_tit_wri`        |
-| `Writnig Outcome Description`               | `raw`  | `out_desc_wri`       |
-| `Writnig Outcome Type`                      | `raw`  | `out_type_wri`       |
-| `Writnig Outcome SMD`                       | `raw`  | `smd_wri`            |
-| `Writnig Outcome SE`                        | `raw`  | `se_wri`             |
-| `Writnig Outcome CI (lower)`                | `raw`  | `ci_lower_wri`       |
-| `Writnig Outcome CI (upper)`                | `raw`  | `ci_upper_wri`       |
-| `Writnig Outcome Measure`                   | `raw`  | `out_measure_wri`    |
-| `Writnig Outcome Group1 N`                  | `raw`  | `out_g1_n_wri`       |
-| `Writnig Outcome Group1 Mean`               | `raw`  | `out_g1_mean_wri`    |
-| `Writnig Outcome Group1 SD`                 | `raw`  | `out_g1_sd_wri`      |
-| `Writnig Outcome Group2 N`                  | `raw`  | `out_g2_n_wri`       |
-| `Writnig Outcome Group2 Mean`               | `raw`  | `out_g2_mean_wri`    |
-| `Writnig Outcome Group2 SD`                 | `raw`  | `out_g2_sd_wri`      |
-| `Writnig Outcome Test Type`                 | `raw`  | `out_test_type_raw_wri` |
-| `Writnig Outcome Effect Size Type`          | `raw`  | `out_es_type_wri`    |
+| `Writing Outcome Title`                     | `raw`  | `out_tit_wri`        |
+| `Writing Outcome Description`               | `raw`  | `out_desc_wri`       |
+| `Writing Outcome Type`                      | `raw`  | `out_type_wri`       |
+| `Writing Outcome SMD`                       | `raw`  | `smd_wri`            |
+| `Writing Outcome SE`                        | `raw`  | `se_wri`             |
+| `Writing Outcome CI (lower)`                | `raw`  | `ci_lower_wri`       |
+| `Writing Outcome CI (upper)`                | `raw`  | `ci_upper_wri`       |
+| `Writing Outcome Measure`                   | `raw`  | `out_measure_wri`    |
+| `Writing Outcome Group1 N`                  | `raw`  | `out_g1_n_wri`       |
+| `Writing Outcome Group1 Mean`               | `raw`  | `out_g1_mean_wri`    |
+| `Writing Outcome Group1 SD`                 | `raw`  | `out_g1_sd_wri`      |
+| `Writing Outcome Group2 N`                  | `raw`  | `out_g2_n_wri`       |
+| `Writing Outcome Group2 Mean`               | `raw`  | `out_g2_mean_wri`    |
+| `Writing Outcome Group2 SD`                 | `raw`  | `out_g2_sd_wri`      |
+| `Writing Outcome Test Type`                 | `raw`  | `out_test_type_raw_wri` |
+| `Writing Outcome Effect Size Type`          | `raw`  | `out_es_type_wri`    |
 | `Math Outcome Title`                        | `raw`  | `out_tit_math`       |
 | `Math Outcome Description`                  | `raw`  | `out_desc_math`      |
 | `Math Outcome Type`                         | `raw`  | `out_type_math`      |
 | `Math Outcome SMD`                          | `raw`  | `smd_math`           |
 | `Math Outcome SE`                           | `raw`  | `se_math`            |
 | `Math Outcome CI (lower)`                   | `raw`  | `ci_lower_math`      |
 | `Math Outcome CI (upper)`                   | `raw`  | `ci_upper_math`      |
@@ -859,14 +857,20 @@
 | `FSM Outcome Group1 Mean`                   | `raw`  | `out_g1_mean_fsm`    |
 | `FSM Outcome Group1 SD`                     | `raw`  | `out_g1_sd_fsm`      |
 | `FSM Outcome Group2 N`                      | `raw`  | `out_g2_n_fsm`       |
 | `FSM Outcome Group2 Mean`                   | `raw`  | `out_g2_mean_fsm`    |
 | `FSM Outcome Group2 SD`                     | `raw`  | `out_g2_sd_fsm`      |
 | `FSM Outcome Test Type`                     | `raw`  | `out_test_type_raw_fsm` |
 | `FSM Outcome Effect Size Type`              | `raw`  | `out_es_type_fsm`    |
+| `Intervention Name (ht)`                     | `ht`  | `int_name_ht`   |
+| `Intervention Name (info)`                     | `info`  | `int_name_info`   |
+| `Intervention Description (ht)`                     | `ht`  | `int_desc_ht`   |
+| `Intervention Description (info)`                     | `info`  | `int_desc_info`   |
+| `Intervention Objective (ht)`                     | `ht`  | `int_objec_ht`   |
+| `Intervention Objective (info)`                     | `info`  | `int_objec_info`   |
 | `Intervention Training`                     | `raw`  | `int_training_raw`   |
 | `Intervention Training (ht)`                | `ht`   | `int_training_ht`    |
 | `Intervention Training (info)`              | `info` | `int_training_info`  |
 | `Intervention Approach`                     | `raw`  | `int_approach_raw`   |
 | `Intervention Approach (ht)`                | `ht`   | `int_approach_ht`    |
 | `Intervention Approach (info)`              | `info` | `int_approach_info`  |
 | `Digital Technology`                        | `raw`  | `digit_tech_raw`     |
@@ -884,13 +888,71 @@
 | `Intervention Duration (ht)`                | `ht`   | `int_dur_ht`         |
 | `Intervention Duration (info)`              | `info` | `int_dur_info`       |
 | `Intervention Length (ht)`                  | `ht`   | `int_leng_ht`        |
 | `Intervention Length (info)`                | `info` | `int_leng_info`      |
 | `Intervention Setting`                      | `raw`  | `int_setting_raw`    |
 | `Intervention Setting (ht)`                 | `ht`   | `int_setting_ht`     |
 | `Intervention Setting (info)`               | `info` | `int_setting_info`   |
+| `Intervention Focus`                      | `raw`  | `int_part_raw`    |
+| `Intervention Focus (ht)`                 | `ht`   | `int_part_ht`     |
+| `Intervention Focus (info)`               | `info` | `int_part_info`   |
+| `Intervention Detail`                      | `raw`  | `int_fidel_raw`    |
+| `Intervention Detail (ht)`                 | `ht`   | `int_fidel_ht`     |
+| `Intervention Detail (info)`               | `info` | `int_fidel_info`   |
+| `Intervention Cost`                      | `raw`  | `int_cost_raw`    |
+| `Intervention Cost (ht)`                 | `ht`   | `int_cost_ht`     |
+| `Intervention Cost (info)`               | `info` | `int_cost_info`   |
+| `Baseline Differences (raw)`              | `raw`  | `base_diff_raw`    |
+| `Baseline Differences (ht)`               | `ht`   | `base_diff_ht`     |
+| `Baseline Differences (info)`             | `info` | `base_diff_info`   |
+| `Comparability (raw)`              | `raw`  | `comp_anal_raw`    |
+| `Comparability (ht)`               | `ht`   | `comp_anal_ht`     |
+| `Comparability (info)`             | `info` | `comp_anal_info`   |
+| `Comparability Reported`              | `raw`  | `comp_var__raw`    |
+| `Comparability Reported (ht)`               | `ht`   | `comp_var__ht`     |
+| `Comparability Reported (info)`             | `info` | `comp_var__info`   |
+| `Which Comp Var Reported`              | `raw`  | `comp_var_rep_raw`    |
+| `Which Comp Var Reported (ht)`               | `ht`   | `comp_var_rep_ht`     |
+| `Which Comp Var Reported (info)`             | `info` | `comp_var_rep_info`   |
+| `Clustering`              | `raw`  | `clust_anal_raw`    |
+| `Clustering (ht)`               | `ht`   | `clust_anal_ht`     |
+| `Clustering (info)`             | `info` | `clust_anal_info`   |
+| `Student Gender`              | `raw`  | `part_gen_raw`    |
+| `Student Gender (ht)`               | `ht`   | `part_gen_ht`     |
+| `Student Gender (info)`             | `info` | `part_gen_info`   |
+| `Sample Size (ht)`               | `ht`   | `sample_analysed_ht`     |
+| `Sample Size (info)`             | `info` | `sample_analysed_info`   |
+| `Intervention Sample Size (ht)`             | `ht` | `base_n_treat_ht`   |
+| `Intervention Sample Size (info)`             | `info` | `base_n_treat_info`   |
+| `Control Sample Size (ht)`             | `ht` | `base_n_cont_ht`   |
+| `Control Sample Size (info)`             | `info` | `base_n_cont_info`   |
+| `Intervention 2 Sample Size (ht)`             | `ht` | `base_n_treat2_ht`   |
+| `Intervention 2 Sample Size (info)`             | `info` | `base_n_treat2_info`   |
+| `Intervention 3 Sample Size (ht)`             | `ht` | `base_n_treat3_ht`   |
+| `Intervention 3 Sample Size (info)`             | `info` | `base_n_treat3_info`   |
+| `Intervention Sample Size Analyzed (ht)`             | `ht` | `n_treat_ht`   |
+| `Intervention Sample Size Analyzed (info)`             | `info` | `n_treat_info`   |
+| `Control Sample Size Analyzed (ht)`             | `ht` | `n_cont_ht`   |
+| `Control Sample Size Analyzed (info)`             | `info` | `n_cont_info`   |
+| `Intervention 2 Sample Size Analyzed (ht)`             | `ht` | `n_treat2_ht`   |
+| `Intervention 2 Sample Size Analyzed (info)`             | `info` | `n_treat2_info`   |
+| `Control 2 Sample Size Analyzed (ht)`             | `ht` | `n_cont2_ht`   |
+| `Control 2 Sample Size  (info)`             | `info` | `n_cont2_info`   |
+| `Attrition Reported`             | `raw` | `attri_raw`   |
+| `Attrition Reported (ht)`             | `ht` | `attri_ht`   |
+| `Attrition Reported (info)`             | `info` | `attri_info`   |
+| `Treatment Group Attrition (ht)`             | `ht` | `attri_treat_ht`   |
+| `Treatment Group Attrition (info)`             | `info` | `attri_treat_info`   |
+| `Total % Attrition (ht)`             | `ht` | `attri_perc_ht`   |
+| `Total % Attrition (info)`             | `info` | `attri_perc_info`   |
+| `All`             | `*all columns` | `*all columns`   |
+
 </details>
 
+## Custom ID Selection
+
+This option produces all columns for one or more user entered EPPI ID's.
+
 ## License
 
 Distributed under the MIT License. See LICENSE for more information.
```

### Comparing `eef-data-0.52/README.md` & `eef-data-0.53/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -694,44 +694,42 @@
 | `URL`            | `raw`     | `url`            |
 | `Publisher`      | `raw`     | `publisher`      |
 | `City`           | `raw`     | `city`           |
 | `Institution`    | `raw`     | `institution`    |
 
 </details>
 
-## Custom Dataframe Selection
+## Custom Column Selection
 
-This dataframe consists of the data the user chooses from a pre-defined column list.
+Custom column selections consist of the data the user chooses from a pre-defined list of column options.
 
 | Data Type   | Description                           | Number of Columns   |
 | ----------- | ------------------------------------- | :-----------------: |
-|  `_raw`     | raw data as input by the data coders  | 119                 |
-|  `_ht`      | text highlighted from the manuscript  | 19                  |
-|  `_info`    | any 'user' entered info               | 19                  |
+|  `_raw`     | raw data as input by the data coders  | 127                 |
+|  `_ht`      | text highlighted from the manuscript  | 43                 |
+|  `_info`    | any 'user' entered info               | 43                  |
 | `_CLEAN`    | empty columns for data cleaning notes | 0                   |
-|             | **Total Number of Columns**           | **157**<sup>1</sup> |
+|             | **Total Number of Columns**           | **213**<sup>1</sup> |
 
-<sup>1</sup>157 is the maximum number of columns where are all data are selected.
+<sup>1</sup>213 is the maximum number of columns where are all data are selected.
 
 <details>
 <summary>Custom Dataframe Selection Column Summary</summary>
 
 | Variable                                    | Data Type | Column Name         |
 | ------------------------------------------- | --------- | ------------------- |
-| `Eppi ID`                                   | `raw`     | `id`                |
+| `Study ID`                                   | `raw`     | `id`                |
 | `Publication Author`                        | `raw`     | `pub_author`        |
 | `Publication Year`                          | `raw`     | `pub_year`          |
 | `Abstract`                                  | `raw`     | `abstract`          |
 | `Strand`                                    | `raw`     | `strand_raw`        |
 | `Country`                                   | `raw`     | `loc_country_raw`   |
 | `Publication Type (EPPI)`                   | `raw`     | `pub_eppi`          |
 | `Publication Type`                          | `raw`     | `pub_type_raw`      |
-| `Educational Setting`                       | `raw`     | `int_setting_raw`   |
 | `Participant Age`                           | `raw`     | `part_age_raw`      |
-| `REPLACE`                                   | `REPLACE` | `REPLACE`           |
 | `Ecological Validity`                       | `raw`     | `eco_valid_raw`     |
 | `Intervention Number of Schools (info)`     | `info`    | `school_treat_info` |
 | `Intervention Number of Schools (ht)`       | `ht`      | `school_treat_ht`   |
 | `Control Number of Schools (info)`          | `info`    | `school_cont_info`  |
 | `Control Number of Schools (ht)`            | `ht`      | `school_cont_ht`    |
 | `Total Number of Schools (info)`            | `info`    | `school_total_info` |
 | `Total Number of Schools (ht)`              | `ht`      | `school_total_ht`   |
@@ -781,30 +779,30 @@
 | `Reading Outcome Group1 Mean`               | `raw`  | `out_g1_mean_red`    |
 | `Reading Outcome Group1 SD`                 | `raw`  | `out_g1_sd_red`      |
 | `Reading Outcome Group2 N`                  | `raw`  | `out_g2_n_red`       |
 | `Reading Outcome Group2 Mean`               | `raw`  | `out_g2_mean_red`    |
 | `Reading Outcome Group2 SD`                 | `raw`  | `out_g2_sd_red`      |
 | `Reading Outcome Test Type`                 | `raw`  | `out_test_type_raw_red` |
 | `Reading Outcome Effect Size Type`          | `raw`  | `out_es_type_red`    |
-| `Writnig Outcome Title`                     | `raw`  | `out_tit_wri`        |
-| `Writnig Outcome Description`               | `raw`  | `out_desc_wri`       |
-| `Writnig Outcome Type`                      | `raw`  | `out_type_wri`       |
-| `Writnig Outcome SMD`                       | `raw`  | `smd_wri`            |
-| `Writnig Outcome SE`                        | `raw`  | `se_wri`             |
-| `Writnig Outcome CI (lower)`                | `raw`  | `ci_lower_wri`       |
-| `Writnig Outcome CI (upper)`                | `raw`  | `ci_upper_wri`       |
-| `Writnig Outcome Measure`                   | `raw`  | `out_measure_wri`    |
-| `Writnig Outcome Group1 N`                  | `raw`  | `out_g1_n_wri`       |
-| `Writnig Outcome Group1 Mean`               | `raw`  | `out_g1_mean_wri`    |
-| `Writnig Outcome Group1 SD`                 | `raw`  | `out_g1_sd_wri`      |
-| `Writnig Outcome Group2 N`                  | `raw`  | `out_g2_n_wri`       |
-| `Writnig Outcome Group2 Mean`               | `raw`  | `out_g2_mean_wri`    |
-| `Writnig Outcome Group2 SD`                 | `raw`  | `out_g2_sd_wri`      |
-| `Writnig Outcome Test Type`                 | `raw`  | `out_test_type_raw_wri` |
-| `Writnig Outcome Effect Size Type`          | `raw`  | `out_es_type_wri`    |
+| `Writing Outcome Title`                     | `raw`  | `out_tit_wri`        |
+| `Writing Outcome Description`               | `raw`  | `out_desc_wri`       |
+| `Writing Outcome Type`                      | `raw`  | `out_type_wri`       |
+| `Writing Outcome SMD`                       | `raw`  | `smd_wri`            |
+| `Writing Outcome SE`                        | `raw`  | `se_wri`             |
+| `Writing Outcome CI (lower)`                | `raw`  | `ci_lower_wri`       |
+| `Writing Outcome CI (upper)`                | `raw`  | `ci_upper_wri`       |
+| `Writing Outcome Measure`                   | `raw`  | `out_measure_wri`    |
+| `Writing Outcome Group1 N`                  | `raw`  | `out_g1_n_wri`       |
+| `Writing Outcome Group1 Mean`               | `raw`  | `out_g1_mean_wri`    |
+| `Writing Outcome Group1 SD`                 | `raw`  | `out_g1_sd_wri`      |
+| `Writing Outcome Group2 N`                  | `raw`  | `out_g2_n_wri`       |
+| `Writing Outcome Group2 Mean`               | `raw`  | `out_g2_mean_wri`    |
+| `Writing Outcome Group2 SD`                 | `raw`  | `out_g2_sd_wri`      |
+| `Writing Outcome Test Type`                 | `raw`  | `out_test_type_raw_wri` |
+| `Writing Outcome Effect Size Type`          | `raw`  | `out_es_type_wri`    |
 | `Math Outcome Title`                        | `raw`  | `out_tit_math`       |
 | `Math Outcome Description`                  | `raw`  | `out_desc_math`      |
 | `Math Outcome Type`                         | `raw`  | `out_type_math`      |
 | `Math Outcome SMD`                          | `raw`  | `smd_math`           |
 | `Math Outcome SE`                           | `raw`  | `se_math`            |
 | `Math Outcome CI (lower)`                   | `raw`  | `ci_lower_math`      |
 | `Math Outcome CI (upper)`                   | `raw`  | `ci_upper_math`      |
@@ -845,14 +843,20 @@
 | `FSM Outcome Group1 Mean`                   | `raw`  | `out_g1_mean_fsm`    |
 | `FSM Outcome Group1 SD`                     | `raw`  | `out_g1_sd_fsm`      |
 | `FSM Outcome Group2 N`                      | `raw`  | `out_g2_n_fsm`       |
 | `FSM Outcome Group2 Mean`                   | `raw`  | `out_g2_mean_fsm`    |
 | `FSM Outcome Group2 SD`                     | `raw`  | `out_g2_sd_fsm`      |
 | `FSM Outcome Test Type`                     | `raw`  | `out_test_type_raw_fsm` |
 | `FSM Outcome Effect Size Type`              | `raw`  | `out_es_type_fsm`    |
+| `Intervention Name (ht)`                     | `ht`  | `int_name_ht`   |
+| `Intervention Name (info)`                     | `info`  | `int_name_info`   |
+| `Intervention Description (ht)`                     | `ht`  | `int_desc_ht`   |
+| `Intervention Description (info)`                     | `info`  | `int_desc_info`   |
+| `Intervention Objective (ht)`                     | `ht`  | `int_objec_ht`   |
+| `Intervention Objective (info)`                     | `info`  | `int_objec_info`   |
 | `Intervention Training`                     | `raw`  | `int_training_raw`   |
 | `Intervention Training (ht)`                | `ht`   | `int_training_ht`    |
 | `Intervention Training (info)`              | `info` | `int_training_info`  |
 | `Intervention Approach`                     | `raw`  | `int_approach_raw`   |
 | `Intervention Approach (ht)`                | `ht`   | `int_approach_ht`    |
 | `Intervention Approach (info)`              | `info` | `int_approach_info`  |
 | `Digital Technology`                        | `raw`  | `digit_tech_raw`     |
@@ -885,27 +889,55 @@
 | `Intervention Cost (info)`               | `info` | `int_cost_info`   |
 | `Baseline Differences (raw)`              | `raw`  | `base_diff_raw`    |
 | `Baseline Differences (ht)`               | `ht`   | `base_diff_ht`     |
 | `Baseline Differences (info)`             | `info` | `base_diff_info`   |
 | `Comparability (raw)`              | `raw`  | `comp_anal_raw`    |
 | `Comparability (ht)`               | `ht`   | `comp_anal_ht`     |
 | `Comparability (info)`             | `info` | `comp_anal_info`   |
-| `Comparability Reported (raw)`              | `raw`  | `comp_var__raw`    |
+| `Comparability Reported`              | `raw`  | `comp_var__raw`    |
 | `Comparability Reported (ht)`               | `ht`   | `comp_var__ht`     |
 | `Comparability Reported (info)`             | `info` | `comp_var__info`   |
-| `Which Comp Var Reported (raw)`              | `raw`  | `comp_var_rep_raw`    |
+| `Which Comp Var Reported`              | `raw`  | `comp_var_rep_raw`    |
 | `Which Comp Var Reported (ht)`               | `ht`   | `comp_var_rep_ht`     |
 | `Which Comp Var Reported (info)`             | `info` | `comp_var_rep_info`   |
-| `Clustering (raw)`              | `raw`  | `clust_anal_raw`    |
+| `Clustering`              | `raw`  | `clust_anal_raw`    |
 | `Clustering (ht)`               | `ht`   | `clust_anal_ht`     |
 | `Clustering (info)`             | `info` | `clust_anal_info`   |
-| `Student Gender (raw)`              | `raw`  | `part_gen_raw`    |
+| `Student Gender`              | `raw`  | `part_gen_raw`    |
 | `Student Gender (ht)`               | `ht`   | `part_gen_ht`     |
 | `Student Gender (info)`             | `info` | `part_gen_info`   |
 | `Sample Size (ht)`               | `ht`   | `sample_analysed_ht`     |
 | `Sample Size (info)`             | `info` | `sample_analysed_info`   |
+| `Intervention Sample Size (ht)`             | `ht` | `base_n_treat_ht`   |
+| `Intervention Sample Size (info)`             | `info` | `base_n_treat_info`   |
+| `Control Sample Size (ht)`             | `ht` | `base_n_cont_ht`   |
+| `Control Sample Size (info)`             | `info` | `base_n_cont_info`   |
+| `Intervention 2 Sample Size (ht)`             | `ht` | `base_n_treat2_ht`   |
+| `Intervention 2 Sample Size (info)`             | `info` | `base_n_treat2_info`   |
+| `Intervention 3 Sample Size (ht)`             | `ht` | `base_n_treat3_ht`   |
+| `Intervention 3 Sample Size (info)`             | `info` | `base_n_treat3_info`   |
+| `Intervention Sample Size Analyzed (ht)`             | `ht` | `n_treat_ht`   |
+| `Intervention Sample Size Analyzed (info)`             | `info` | `n_treat_info`   |
+| `Control Sample Size Analyzed (ht)`             | `ht` | `n_cont_ht`   |
+| `Control Sample Size Analyzed (info)`             | `info` | `n_cont_info`   |
+| `Intervention 2 Sample Size Analyzed (ht)`             | `ht` | `n_treat2_ht`   |
+| `Intervention 2 Sample Size Analyzed (info)`             | `info` | `n_treat2_info`   |
+| `Control 2 Sample Size Analyzed (ht)`             | `ht` | `n_cont2_ht`   |
+| `Control 2 Sample Size  (info)`             | `info` | `n_cont2_info`   |
+| `Attrition Reported`             | `raw` | `attri_raw`   |
+| `Attrition Reported (ht)`             | `ht` | `attri_ht`   |
+| `Attrition Reported (info)`             | `info` | `attri_info`   |
+| `Treatment Group Attrition (ht)`             | `ht` | `attri_treat_ht`   |
+| `Treatment Group Attrition (info)`             | `info` | `attri_treat_info`   |
+| `Total % Attrition (ht)`             | `ht` | `attri_perc_ht`   |
+| `Total % Attrition (info)`             | `info` | `attri_perc_info`   |
+| `All`             | `*all columns` | `*all columns`   |
 
 </details>
 
+## Custom ID Selection
+
+This option produces all columns for one or more user entered EPPI ID's.
+
 ## License
 
 Distributed under the MIT License. See LICENSE for more information.
```

### Comparing `eef-data-0.52/README_package.md` & `eef-data-0.53/README_package.md`

 * *Files 4% similar despite different names*

```diff
@@ -697,44 +697,42 @@
 | `URL`            | `raw`     | `url`            |
 | `Publisher`      | `raw`     | `publisher`      |
 | `City`           | `raw`     | `city`           |
 | `Institution`    | `raw`     | `institution`    |
 
 </details>
 
-## Custom Dataframe Selection
+## Custom Column Selection
 
-This dataframe consists of the data the user chooses from a pre-defined column list.
+Custom column selections consist of the data the user chooses from a pre-defined list of column options.
 
 | Data Type   | Description                           | Number of Columns   |
 | ----------- | ------------------------------------- | :-----------------: |
-|  `_raw`     | raw data as input by the data coders  | 119                 |
-|  `_ht`      | text highlighted from the manuscript  | 19                  |
-|  `_info`    | any 'user' entered info               | 19                  |
+|  `_raw`     | raw data as input by the data coders  | 127                 |
+|  `_ht`      | text highlighted from the manuscript  | 43                 |
+|  `_info`    | any 'user' entered info               | 43                  |
 | `_CLEAN`    | empty columns for data cleaning notes | 0                   |
-|             | **Total Number of Columns**           | **157**<sup>1</sup> |
+|             | **Total Number of Columns**           | **213**<sup>1</sup> |
 
-<sup>1</sup>157 is the maximum number of columns where are all data are selected.
+<sup>1</sup>213 is the maximum number of columns where are all data are selected.
 
 <details>
 <summary>Custom Dataframe Selection Column Summary</summary>
 
 | Variable                                    | Data Type | Column Name         |
 | ------------------------------------------- | --------- | ------------------- |
-| `Eppi ID`                                   | `raw`     | `id`                |
+| `Study ID`                                   | `raw`     | `id`                |
 | `Publication Author`                        | `raw`     | `pub_author`        |
 | `Publication Year`                          | `raw`     | `pub_year`          |
 | `Abstract`                                  | `raw`     | `abstract`          |
 | `Strand`                                    | `raw`     | `strand_raw`        |
 | `Country`                                   | `raw`     | `loc_country_raw`   |
 | `Publication Type (EPPI)`                   | `raw`     | `pub_eppi`          |
 | `Publication Type`                          | `raw`     | `pub_type_raw`      |
-| `Educational Setting`                       | `raw`     | `int_setting_raw`   |
 | `Participant Age`                           | `raw`     | `part_age_raw`      |
-| `REPLACE`                                   | `REPLACE` | `REPLACE`           |
 | `Ecological Validity`                       | `raw`     | `eco_valid_raw`     |
 | `Intervention Number of Schools (info)`     | `info`    | `school_treat_info` |
 | `Intervention Number of Schools (ht)`       | `ht`      | `school_treat_ht`   |
 | `Control Number of Schools (info)`          | `info`    | `school_cont_info`  |
 | `Control Number of Schools (ht)`            | `ht`      | `school_cont_ht`    |
 | `Total Number of Schools (info)`            | `info`    | `school_total_info` |
 | `Total Number of Schools (ht)`              | `ht`      | `school_total_ht`   |
@@ -784,30 +782,30 @@
 | `Reading Outcome Group1 Mean`               | `raw`  | `out_g1_mean_red`    |
 | `Reading Outcome Group1 SD`                 | `raw`  | `out_g1_sd_red`      |
 | `Reading Outcome Group2 N`                  | `raw`  | `out_g2_n_red`       |
 | `Reading Outcome Group2 Mean`               | `raw`  | `out_g2_mean_red`    |
 | `Reading Outcome Group2 SD`                 | `raw`  | `out_g2_sd_red`      |
 | `Reading Outcome Test Type`                 | `raw`  | `out_test_type_raw_red` |
 | `Reading Outcome Effect Size Type`          | `raw`  | `out_es_type_red`    |
-| `Writnig Outcome Title`                     | `raw`  | `out_tit_wri`        |
-| `Writnig Outcome Description`               | `raw`  | `out_desc_wri`       |
-| `Writnig Outcome Type`                      | `raw`  | `out_type_wri`       |
-| `Writnig Outcome SMD`                       | `raw`  | `smd_wri`            |
-| `Writnig Outcome SE`                        | `raw`  | `se_wri`             |
-| `Writnig Outcome CI (lower)`                | `raw`  | `ci_lower_wri`       |
-| `Writnig Outcome CI (upper)`                | `raw`  | `ci_upper_wri`       |
-| `Writnig Outcome Measure`                   | `raw`  | `out_measure_wri`    |
-| `Writnig Outcome Group1 N`                  | `raw`  | `out_g1_n_wri`       |
-| `Writnig Outcome Group1 Mean`               | `raw`  | `out_g1_mean_wri`    |
-| `Writnig Outcome Group1 SD`                 | `raw`  | `out_g1_sd_wri`      |
-| `Writnig Outcome Group2 N`                  | `raw`  | `out_g2_n_wri`       |
-| `Writnig Outcome Group2 Mean`               | `raw`  | `out_g2_mean_wri`    |
-| `Writnig Outcome Group2 SD`                 | `raw`  | `out_g2_sd_wri`      |
-| `Writnig Outcome Test Type`                 | `raw`  | `out_test_type_raw_wri` |
-| `Writnig Outcome Effect Size Type`          | `raw`  | `out_es_type_wri`    |
+| `Writing Outcome Title`                     | `raw`  | `out_tit_wri`        |
+| `Writing Outcome Description`               | `raw`  | `out_desc_wri`       |
+| `Writing Outcome Type`                      | `raw`  | `out_type_wri`       |
+| `Writing Outcome SMD`                       | `raw`  | `smd_wri`            |
+| `Writing Outcome SE`                        | `raw`  | `se_wri`             |
+| `Writing Outcome CI (lower)`                | `raw`  | `ci_lower_wri`       |
+| `Writing Outcome CI (upper)`                | `raw`  | `ci_upper_wri`       |
+| `Writing Outcome Measure`                   | `raw`  | `out_measure_wri`    |
+| `Writing Outcome Group1 N`                  | `raw`  | `out_g1_n_wri`       |
+| `Writing Outcome Group1 Mean`               | `raw`  | `out_g1_mean_wri`    |
+| `Writing Outcome Group1 SD`                 | `raw`  | `out_g1_sd_wri`      |
+| `Writing Outcome Group2 N`                  | `raw`  | `out_g2_n_wri`       |
+| `Writing Outcome Group2 Mean`               | `raw`  | `out_g2_mean_wri`    |
+| `Writing Outcome Group2 SD`                 | `raw`  | `out_g2_sd_wri`      |
+| `Writing Outcome Test Type`                 | `raw`  | `out_test_type_raw_wri` |
+| `Writing Outcome Effect Size Type`          | `raw`  | `out_es_type_wri`    |
 | `Math Outcome Title`                        | `raw`  | `out_tit_math`       |
 | `Math Outcome Description`                  | `raw`  | `out_desc_math`      |
 | `Math Outcome Type`                         | `raw`  | `out_type_math`      |
 | `Math Outcome SMD`                          | `raw`  | `smd_math`           |
 | `Math Outcome SE`                           | `raw`  | `se_math`            |
 | `Math Outcome CI (lower)`                   | `raw`  | `ci_lower_math`      |
 | `Math Outcome CI (upper)`                   | `raw`  | `ci_upper_math`      |
@@ -848,14 +846,20 @@
 | `FSM Outcome Group1 Mean`                   | `raw`  | `out_g1_mean_fsm`    |
 | `FSM Outcome Group1 SD`                     | `raw`  | `out_g1_sd_fsm`      |
 | `FSM Outcome Group2 N`                      | `raw`  | `out_g2_n_fsm`       |
 | `FSM Outcome Group2 Mean`                   | `raw`  | `out_g2_mean_fsm`    |
 | `FSM Outcome Group2 SD`                     | `raw`  | `out_g2_sd_fsm`      |
 | `FSM Outcome Test Type`                     | `raw`  | `out_test_type_raw_fsm` |
 | `FSM Outcome Effect Size Type`              | `raw`  | `out_es_type_fsm`    |
+| `Intervention Name (ht)`                     | `ht`  | `int_name_ht`   |
+| `Intervention Name (info)`                     | `info`  | `int_name_info`   |
+| `Intervention Description (ht)`                     | `ht`  | `int_desc_ht`   |
+| `Intervention Description (info)`                     | `info`  | `int_desc_info`   |
+| `Intervention Objective (ht)`                     | `ht`  | `int_objec_ht`   |
+| `Intervention Objective (info)`                     | `info`  | `int_objec_info`   |
 | `Intervention Training`                     | `raw`  | `int_training_raw`   |
 | `Intervention Training (ht)`                | `ht`   | `int_training_ht`    |
 | `Intervention Training (info)`              | `info` | `int_training_info`  |
 | `Intervention Approach`                     | `raw`  | `int_approach_raw`   |
 | `Intervention Approach (ht)`                | `ht`   | `int_approach_ht`    |
 | `Intervention Approach (info)`              | `info` | `int_approach_info`  |
 | `Digital Technology`                        | `raw`  | `digit_tech_raw`     |
@@ -873,12 +877,70 @@
 | `Intervention Duration (ht)`                | `ht`   | `int_dur_ht`         |
 | `Intervention Duration (info)`              | `info` | `int_dur_info`       |
 | `Intervention Length (ht)`                  | `ht`   | `int_leng_ht`        |
 | `Intervention Length (info)`                | `info` | `int_leng_info`      |
 | `Intervention Setting`                      | `raw`  | `int_setting_raw`    |
 | `Intervention Setting (ht)`                 | `ht`   | `int_setting_ht`     |
 | `Intervention Setting (info)`               | `info` | `int_setting_info`   |
+| `Intervention Focus`                      | `raw`  | `int_part_raw`    |
+| `Intervention Focus (ht)`                 | `ht`   | `int_part_ht`     |
+| `Intervention Focus (info)`               | `info` | `int_part_info`   |
+| `Intervention Detail`                      | `raw`  | `int_fidel_raw`    |
+| `Intervention Detail (ht)`                 | `ht`   | `int_fidel_ht`     |
+| `Intervention Detail (info)`               | `info` | `int_fidel_info`   |
+| `Intervention Cost`                      | `raw`  | `int_cost_raw`    |
+| `Intervention Cost (ht)`                 | `ht`   | `int_cost_ht`     |
+| `Intervention Cost (info)`               | `info` | `int_cost_info`   |
+| `Baseline Differences (raw)`              | `raw`  | `base_diff_raw`    |
+| `Baseline Differences (ht)`               | `ht`   | `base_diff_ht`     |
+| `Baseline Differences (info)`             | `info` | `base_diff_info`   |
+| `Comparability (raw)`              | `raw`  | `comp_anal_raw`    |
+| `Comparability (ht)`               | `ht`   | `comp_anal_ht`     |
+| `Comparability (info)`             | `info` | `comp_anal_info`   |
+| `Comparability Reported`              | `raw`  | `comp_var__raw`    |
+| `Comparability Reported (ht)`               | `ht`   | `comp_var__ht`     |
+| `Comparability Reported (info)`             | `info` | `comp_var__info`   |
+| `Which Comp Var Reported`              | `raw`  | `comp_var_rep_raw`    |
+| `Which Comp Var Reported (ht)`               | `ht`   | `comp_var_rep_ht`     |
+| `Which Comp Var Reported (info)`             | `info` | `comp_var_rep_info`   |
+| `Clustering`              | `raw`  | `clust_anal_raw`    |
+| `Clustering (ht)`               | `ht`   | `clust_anal_ht`     |
+| `Clustering (info)`             | `info` | `clust_anal_info`   |
+| `Student Gender`              | `raw`  | `part_gen_raw`    |
+| `Student Gender (ht)`               | `ht`   | `part_gen_ht`     |
+| `Student Gender (info)`             | `info` | `part_gen_info`   |
+| `Sample Size (ht)`               | `ht`   | `sample_analysed_ht`     |
+| `Sample Size (info)`             | `info` | `sample_analysed_info`   |
+| `Intervention Sample Size (ht)`             | `ht` | `base_n_treat_ht`   |
+| `Intervention Sample Size (info)`             | `info` | `base_n_treat_info`   |
+| `Control Sample Size (ht)`             | `ht` | `base_n_cont_ht`   |
+| `Control Sample Size (info)`             | `info` | `base_n_cont_info`   |
+| `Intervention 2 Sample Size (ht)`             | `ht` | `base_n_treat2_ht`   |
+| `Intervention 2 Sample Size (info)`             | `info` | `base_n_treat2_info`   |
+| `Intervention 3 Sample Size (ht)`             | `ht` | `base_n_treat3_ht`   |
+| `Intervention 3 Sample Size (info)`             | `info` | `base_n_treat3_info`   |
+| `Intervention Sample Size Analyzed (ht)`             | `ht` | `n_treat_ht`   |
+| `Intervention Sample Size Analyzed (info)`             | `info` | `n_treat_info`   |
+| `Control Sample Size Analyzed (ht)`             | `ht` | `n_cont_ht`   |
+| `Control Sample Size Analyzed (info)`             | `info` | `n_cont_info`   |
+| `Intervention 2 Sample Size Analyzed (ht)`             | `ht` | `n_treat2_ht`   |
+| `Intervention 2 Sample Size Analyzed (info)`             | `info` | `n_treat2_info`   |
+| `Control 2 Sample Size Analyzed (ht)`             | `ht` | `n_cont2_ht`   |
+| `Control 2 Sample Size  (info)`             | `info` | `n_cont2_info`   |
+| `Attrition Reported`             | `raw` | `attri_raw`   |
+| `Attrition Reported (ht)`             | `ht` | `attri_ht`   |
+| `Attrition Reported (info)`             | `info` | `attri_info`   |
+| `Treatment Group Attrition (ht)`             | `ht` | `attri_treat_ht`   |
+| `Treatment Group Attrition (info)`             | `info` | `attri_treat_info`   |
+| `Total % Attrition (ht)`             | `ht` | `attri_perc_ht`   |
+| `Total % Attrition (info)`             | `info` | `attri_perc_info`   |
+| `All`             | `*all columns` | `*all columns`   |
+
 </details>
 
+## Custom ID Selection
+
+This option produces all columns for one or more user entered EPPI ID's.
+
 ## License
 
 Distributed under the MIT License. See LICENSE for more information.
```

### Comparing `eef-data-0.52/eef_data.egg-info/PKG-INFO` & `eef-data-0.53/eef_data.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eef-data
-Version: 0.52
+Version: 0.53
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.10.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -708,44 +708,42 @@
 | `URL`            | `raw`     | `url`            |
 | `Publisher`      | `raw`     | `publisher`      |
 | `City`           | `raw`     | `city`           |
 | `Institution`    | `raw`     | `institution`    |
 
 </details>
 
-## Custom Dataframe Selection
+## Custom Column Selection
 
-This dataframe consists of the data the user chooses from a pre-defined column list.
+Custom column selections consist of the data the user chooses from a pre-defined list of column options.
 
 | Data Type   | Description                           | Number of Columns   |
 | ----------- | ------------------------------------- | :-----------------: |
-|  `_raw`     | raw data as input by the data coders  | 119                 |
-|  `_ht`      | text highlighted from the manuscript  | 19                  |
-|  `_info`    | any 'user' entered info               | 19                  |
+|  `_raw`     | raw data as input by the data coders  | 127                 |
+|  `_ht`      | text highlighted from the manuscript  | 43                 |
+|  `_info`    | any 'user' entered info               | 43                  |
 | `_CLEAN`    | empty columns for data cleaning notes | 0                   |
-|             | **Total Number of Columns**           | **157**<sup>1</sup> |
+|             | **Total Number of Columns**           | **213**<sup>1</sup> |
 
-<sup>1</sup>157 is the maximum number of columns where are all data are selected.
+<sup>1</sup>213 is the maximum number of columns where are all data are selected.
 
 <details>
 <summary>Custom Dataframe Selection Column Summary</summary>
 
 | Variable                                    | Data Type | Column Name         |
 | ------------------------------------------- | --------- | ------------------- |
-| `Eppi ID`                                   | `raw`     | `id`                |
+| `Study ID`                                   | `raw`     | `id`                |
 | `Publication Author`                        | `raw`     | `pub_author`        |
 | `Publication Year`                          | `raw`     | `pub_year`          |
 | `Abstract`                                  | `raw`     | `abstract`          |
 | `Strand`                                    | `raw`     | `strand_raw`        |
 | `Country`                                   | `raw`     | `loc_country_raw`   |
 | `Publication Type (EPPI)`                   | `raw`     | `pub_eppi`          |
 | `Publication Type`                          | `raw`     | `pub_type_raw`      |
-| `Educational Setting`                       | `raw`     | `int_setting_raw`   |
 | `Participant Age`                           | `raw`     | `part_age_raw`      |
-| `REPLACE`                                   | `REPLACE` | `REPLACE`           |
 | `Ecological Validity`                       | `raw`     | `eco_valid_raw`     |
 | `Intervention Number of Schools (info)`     | `info`    | `school_treat_info` |
 | `Intervention Number of Schools (ht)`       | `ht`      | `school_treat_ht`   |
 | `Control Number of Schools (info)`          | `info`    | `school_cont_info`  |
 | `Control Number of Schools (ht)`            | `ht`      | `school_cont_ht`    |
 | `Total Number of Schools (info)`            | `info`    | `school_total_info` |
 | `Total Number of Schools (ht)`              | `ht`      | `school_total_ht`   |
@@ -795,30 +793,30 @@
 | `Reading Outcome Group1 Mean`               | `raw`  | `out_g1_mean_red`    |
 | `Reading Outcome Group1 SD`                 | `raw`  | `out_g1_sd_red`      |
 | `Reading Outcome Group2 N`                  | `raw`  | `out_g2_n_red`       |
 | `Reading Outcome Group2 Mean`               | `raw`  | `out_g2_mean_red`    |
 | `Reading Outcome Group2 SD`                 | `raw`  | `out_g2_sd_red`      |
 | `Reading Outcome Test Type`                 | `raw`  | `out_test_type_raw_red` |
 | `Reading Outcome Effect Size Type`          | `raw`  | `out_es_type_red`    |
-| `Writnig Outcome Title`                     | `raw`  | `out_tit_wri`        |
-| `Writnig Outcome Description`               | `raw`  | `out_desc_wri`       |
-| `Writnig Outcome Type`                      | `raw`  | `out_type_wri`       |
-| `Writnig Outcome SMD`                       | `raw`  | `smd_wri`            |
-| `Writnig Outcome SE`                        | `raw`  | `se_wri`             |
-| `Writnig Outcome CI (lower)`                | `raw`  | `ci_lower_wri`       |
-| `Writnig Outcome CI (upper)`                | `raw`  | `ci_upper_wri`       |
-| `Writnig Outcome Measure`                   | `raw`  | `out_measure_wri`    |
-| `Writnig Outcome Group1 N`                  | `raw`  | `out_g1_n_wri`       |
-| `Writnig Outcome Group1 Mean`               | `raw`  | `out_g1_mean_wri`    |
-| `Writnig Outcome Group1 SD`                 | `raw`  | `out_g1_sd_wri`      |
-| `Writnig Outcome Group2 N`                  | `raw`  | `out_g2_n_wri`       |
-| `Writnig Outcome Group2 Mean`               | `raw`  | `out_g2_mean_wri`    |
-| `Writnig Outcome Group2 SD`                 | `raw`  | `out_g2_sd_wri`      |
-| `Writnig Outcome Test Type`                 | `raw`  | `out_test_type_raw_wri` |
-| `Writnig Outcome Effect Size Type`          | `raw`  | `out_es_type_wri`    |
+| `Writing Outcome Title`                     | `raw`  | `out_tit_wri`        |
+| `Writing Outcome Description`               | `raw`  | `out_desc_wri`       |
+| `Writing Outcome Type`                      | `raw`  | `out_type_wri`       |
+| `Writing Outcome SMD`                       | `raw`  | `smd_wri`            |
+| `Writing Outcome SE`                        | `raw`  | `se_wri`             |
+| `Writing Outcome CI (lower)`                | `raw`  | `ci_lower_wri`       |
+| `Writing Outcome CI (upper)`                | `raw`  | `ci_upper_wri`       |
+| `Writing Outcome Measure`                   | `raw`  | `out_measure_wri`    |
+| `Writing Outcome Group1 N`                  | `raw`  | `out_g1_n_wri`       |
+| `Writing Outcome Group1 Mean`               | `raw`  | `out_g1_mean_wri`    |
+| `Writing Outcome Group1 SD`                 | `raw`  | `out_g1_sd_wri`      |
+| `Writing Outcome Group2 N`                  | `raw`  | `out_g2_n_wri`       |
+| `Writing Outcome Group2 Mean`               | `raw`  | `out_g2_mean_wri`    |
+| `Writing Outcome Group2 SD`                 | `raw`  | `out_g2_sd_wri`      |
+| `Writing Outcome Test Type`                 | `raw`  | `out_test_type_raw_wri` |
+| `Writing Outcome Effect Size Type`          | `raw`  | `out_es_type_wri`    |
 | `Math Outcome Title`                        | `raw`  | `out_tit_math`       |
 | `Math Outcome Description`                  | `raw`  | `out_desc_math`      |
 | `Math Outcome Type`                         | `raw`  | `out_type_math`      |
 | `Math Outcome SMD`                          | `raw`  | `smd_math`           |
 | `Math Outcome SE`                           | `raw`  | `se_math`            |
 | `Math Outcome CI (lower)`                   | `raw`  | `ci_lower_math`      |
 | `Math Outcome CI (upper)`                   | `raw`  | `ci_upper_math`      |
@@ -859,14 +857,20 @@
 | `FSM Outcome Group1 Mean`                   | `raw`  | `out_g1_mean_fsm`    |
 | `FSM Outcome Group1 SD`                     | `raw`  | `out_g1_sd_fsm`      |
 | `FSM Outcome Group2 N`                      | `raw`  | `out_g2_n_fsm`       |
 | `FSM Outcome Group2 Mean`                   | `raw`  | `out_g2_mean_fsm`    |
 | `FSM Outcome Group2 SD`                     | `raw`  | `out_g2_sd_fsm`      |
 | `FSM Outcome Test Type`                     | `raw`  | `out_test_type_raw_fsm` |
 | `FSM Outcome Effect Size Type`              | `raw`  | `out_es_type_fsm`    |
+| `Intervention Name (ht)`                     | `ht`  | `int_name_ht`   |
+| `Intervention Name (info)`                     | `info`  | `int_name_info`   |
+| `Intervention Description (ht)`                     | `ht`  | `int_desc_ht`   |
+| `Intervention Description (info)`                     | `info`  | `int_desc_info`   |
+| `Intervention Objective (ht)`                     | `ht`  | `int_objec_ht`   |
+| `Intervention Objective (info)`                     | `info`  | `int_objec_info`   |
 | `Intervention Training`                     | `raw`  | `int_training_raw`   |
 | `Intervention Training (ht)`                | `ht`   | `int_training_ht`    |
 | `Intervention Training (info)`              | `info` | `int_training_info`  |
 | `Intervention Approach`                     | `raw`  | `int_approach_raw`   |
 | `Intervention Approach (ht)`                | `ht`   | `int_approach_ht`    |
 | `Intervention Approach (info)`              | `info` | `int_approach_info`  |
 | `Digital Technology`                        | `raw`  | `digit_tech_raw`     |
@@ -884,13 +888,71 @@
 | `Intervention Duration (ht)`                | `ht`   | `int_dur_ht`         |
 | `Intervention Duration (info)`              | `info` | `int_dur_info`       |
 | `Intervention Length (ht)`                  | `ht`   | `int_leng_ht`        |
 | `Intervention Length (info)`                | `info` | `int_leng_info`      |
 | `Intervention Setting`                      | `raw`  | `int_setting_raw`    |
 | `Intervention Setting (ht)`                 | `ht`   | `int_setting_ht`     |
 | `Intervention Setting (info)`               | `info` | `int_setting_info`   |
+| `Intervention Focus`                      | `raw`  | `int_part_raw`    |
+| `Intervention Focus (ht)`                 | `ht`   | `int_part_ht`     |
+| `Intervention Focus (info)`               | `info` | `int_part_info`   |
+| `Intervention Detail`                      | `raw`  | `int_fidel_raw`    |
+| `Intervention Detail (ht)`                 | `ht`   | `int_fidel_ht`     |
+| `Intervention Detail (info)`               | `info` | `int_fidel_info`   |
+| `Intervention Cost`                      | `raw`  | `int_cost_raw`    |
+| `Intervention Cost (ht)`                 | `ht`   | `int_cost_ht`     |
+| `Intervention Cost (info)`               | `info` | `int_cost_info`   |
+| `Baseline Differences (raw)`              | `raw`  | `base_diff_raw`    |
+| `Baseline Differences (ht)`               | `ht`   | `base_diff_ht`     |
+| `Baseline Differences (info)`             | `info` | `base_diff_info`   |
+| `Comparability (raw)`              | `raw`  | `comp_anal_raw`    |
+| `Comparability (ht)`               | `ht`   | `comp_anal_ht`     |
+| `Comparability (info)`             | `info` | `comp_anal_info`   |
+| `Comparability Reported`              | `raw`  | `comp_var__raw`    |
+| `Comparability Reported (ht)`               | `ht`   | `comp_var__ht`     |
+| `Comparability Reported (info)`             | `info` | `comp_var__info`   |
+| `Which Comp Var Reported`              | `raw`  | `comp_var_rep_raw`    |
+| `Which Comp Var Reported (ht)`               | `ht`   | `comp_var_rep_ht`     |
+| `Which Comp Var Reported (info)`             | `info` | `comp_var_rep_info`   |
+| `Clustering`              | `raw`  | `clust_anal_raw`    |
+| `Clustering (ht)`               | `ht`   | `clust_anal_ht`     |
+| `Clustering (info)`             | `info` | `clust_anal_info`   |
+| `Student Gender`              | `raw`  | `part_gen_raw`    |
+| `Student Gender (ht)`               | `ht`   | `part_gen_ht`     |
+| `Student Gender (info)`             | `info` | `part_gen_info`   |
+| `Sample Size (ht)`               | `ht`   | `sample_analysed_ht`     |
+| `Sample Size (info)`             | `info` | `sample_analysed_info`   |
+| `Intervention Sample Size (ht)`             | `ht` | `base_n_treat_ht`   |
+| `Intervention Sample Size (info)`             | `info` | `base_n_treat_info`   |
+| `Control Sample Size (ht)`             | `ht` | `base_n_cont_ht`   |
+| `Control Sample Size (info)`             | `info` | `base_n_cont_info`   |
+| `Intervention 2 Sample Size (ht)`             | `ht` | `base_n_treat2_ht`   |
+| `Intervention 2 Sample Size (info)`             | `info` | `base_n_treat2_info`   |
+| `Intervention 3 Sample Size (ht)`             | `ht` | `base_n_treat3_ht`   |
+| `Intervention 3 Sample Size (info)`             | `info` | `base_n_treat3_info`   |
+| `Intervention Sample Size Analyzed (ht)`             | `ht` | `n_treat_ht`   |
+| `Intervention Sample Size Analyzed (info)`             | `info` | `n_treat_info`   |
+| `Control Sample Size Analyzed (ht)`             | `ht` | `n_cont_ht`   |
+| `Control Sample Size Analyzed (info)`             | `info` | `n_cont_info`   |
+| `Intervention 2 Sample Size Analyzed (ht)`             | `ht` | `n_treat2_ht`   |
+| `Intervention 2 Sample Size Analyzed (info)`             | `info` | `n_treat2_info`   |
+| `Control 2 Sample Size Analyzed (ht)`             | `ht` | `n_cont2_ht`   |
+| `Control 2 Sample Size  (info)`             | `info` | `n_cont2_info`   |
+| `Attrition Reported`             | `raw` | `attri_raw`   |
+| `Attrition Reported (ht)`             | `ht` | `attri_ht`   |
+| `Attrition Reported (info)`             | `info` | `attri_info`   |
+| `Treatment Group Attrition (ht)`             | `ht` | `attri_treat_ht`   |
+| `Treatment Group Attrition (info)`             | `info` | `attri_treat_info`   |
+| `Total % Attrition (ht)`             | `ht` | `attri_perc_ht`   |
+| `Total % Attrition (info)`             | `info` | `attri_perc_info`   |
+| `All`             | `*all columns` | `*all columns`   |
+
 </details>
 
+## Custom ID Selection
+
+This option produces all columns for one or more user entered EPPI ID's.
+
 ## License
 
 Distributed under the MIT License. See LICENSE for more information.
```

### Comparing `eef-data-0.52/eefdata/app.py` & `eef-data-0.53/eefdata/app.py`

 * *Files 23% similar despite different names*

```diff
@@ -37,27 +37,25 @@
     dataframe_11_output_display,
     input_file_info_display,
     main_menu_display,
     main_menu_display1,
 )
 
 # table1 
-row_styles1 = ["#FFFFFF"] * 36
+row_styles1 = ["#FFFFFF"] * 34
 row_data_list1 = [
     "Study ID", 
     "Author", 
     "Year", 
     "Abstract", 
     "Admin Strand",
     "Country", 
     "Publication Type EPPI", 
     "Publication Type",
-    "Educational Setting", 
     "Student Age",
-    "Strand",
     "Ecological Validity",
     "Number of Schools Int (info)",
     "Number of Schools Int (ht)",
     "Number of Schools Ctrl (info)",
     "Number of Schools Ctrl (ht)",
     "Number of Schools Total (info)",
     "Number of Schools Total (ht)",
@@ -199,15 +197,15 @@
                         title_style=table_title_style,                  
     )
 
     main_table3.add_column("", header_style=header_style, style=column_style, width=3)
     main_table3.add_column("Outcome Specific Data", header_style=header_style, style=column_style, width=30)
 
     for idx, row_data in enumerate(row_data_list2, start=1):
-        main_table3.add_row(f"{idx+36}", row_data, style=row_styles2[idx - 1])
+        main_table3.add_row(f"{idx+34}", row_data, style=row_styles2[idx - 1])
     
     return main_table3
 
 # table1 
 row_styles3 = ["#FFFFFF"] * 48
 row_data_list3 = [
 
@@ -288,15 +286,15 @@
                         title_style=table_title_style,                  
     )
 
     main_table4.add_column("", header_style=header_style, style=column_style, width=3)
     main_table4.add_column("Outcome Specific Data", header_style=header_style, style=column_style, width=30)
 
     for idx, row_data in enumerate(row_data_list3, start=1):
-        main_table4.add_row(f"{idx+84}", row_data, style=row_styles3[idx - 1])
+        main_table4.add_row(f"{idx+82}", row_data, style=row_styles3[idx - 1])
     
     return main_table4
 
 # table1 
 row_styles4 = ["#FFFFFF"] * 49
 row_data_list4 = [
     "Intervention Name (ht)",
@@ -377,20 +375,20 @@
                         title_style=table_title_style,                  
     )
 
     main_table5.add_column("", header_style=header_style, style=column_style, width=3)
     main_table5.add_column("Intervention Details", header_style=header_style, style=column_style, width=31)
 
     for idx, row_data in enumerate(row_data_list4, start=1):
-        main_table5.add_row(f"{idx+132}", row_data, style=row_styles4[idx - 1])
+        main_table5.add_row(f"{idx+130}", row_data, style=row_styles4[idx - 1])
     
     return main_table5
 
 # table1 
-row_styles5 = ["#FFFFFF"] * 34
+row_styles5 = ["#FFFFFF"] * 35
 row_data_list5 = [
     "Which Comp Var Reported (raw)",
     "Which Comp Var Reported (ht)",
     "Which Comp Var Reported (info)",
     "Clustering (raw)",
     "Clustering (ht)",
     "Clustering (info)",
@@ -418,14 +416,15 @@
     "Attrition Reported (raw)",
     "Attrition Reported (ht)",
     "Attrition Reported (info)",
     "Treatment Group Attrition (ht)",
     "Treatment Group Attrition (info)",
     "Total % Attrition (ht)",
     "Total % Attrition (info)",
+    "ALL"
 ]
 
 def intervention_vars_4():
     """
     Displays a Rich list of [toolkit]'outcome' variables for the custom data frame builder
     - Outcome Titlepanel5
     - Outcome Description
@@ -451,15 +450,15 @@
                         title_style=table_title_style,                  
     )
 
     main_table6.add_column("", header_style=header_style, style=column_style, width=3)
     main_table6.add_column("Intervention Details", header_style=header_style, style=column_style, width=42)
 
     for idx, row_data in enumerate(row_data_list5, start=1):
-        main_table6.add_row(f"{idx+181}", row_data, style=row_styles5[idx - 1])
+        main_table6.add_row(f"{idx+179}", row_data, style=row_styles5[idx - 1])
     
     return main_table6
 
 def get_user_input():
     while True:
         try:
             data_cleaning_option = Prompt.ask("Enter an option from the Main Menu")
@@ -659,2001 +658,1944 @@
                 
                 df = CustomFrames(json_extractor)
 
                 used_options = []
 
                 # Compile list of invidividual data frames
                 dataframes=[]
+                all_df = pd.DataFrame()
+
+                df_outcomes = DataFrameCompilation(json_extractor)
+                df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
 
                 custom=True
                 while custom==True:
                     try:
                         console.print("\nAdd variables to your data frame or 0 to Save file and exit")
                         num = int(Prompt.ask("Selection"))
-                        if num < 0 or num > 2010:
+                        if num < 0 or num > 2020:
                             raise ValueError
                     except ValueError:
-                        print("Error: invalid input. Please enter a number from 0 to 2010.\n")
+                        print("Error: invalid input. Please enter a number from 0 to 2020.\n")
                         continue
 
                     match num:
                         case 0:
                             run_program=False
                             break
                         case 1: 
                             if "id" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                eppiid_df = df.data_extraction.retrieve_metadata("ItemId", "id")
-                                dataframes.append(eppiid_df)
+                                all_df["id"] = df.data_extraction.retrieve_metadata("ItemId", "id")
                                 used_options.append("id")
                             else:
                                 print("You have already selected this option!")
                         case 2: 
                             if "pub_author" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                author_df = df.data_extraction.retrieve_metadata("ShortTitle", "pub_author")
-                                dataframes.append(author_df)
+                                all_df["pub_author"] = df.data_extraction.retrieve_metadata("ShortTitle", "pub_author")
                                 used_options.append("pub_author")
                             else:
                                 print("You have already selected this option!")
                         case 3: 
                             if "pub_year" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                year_df = df.data_extraction.retrieve_metadata("Year", "pub_year")
-                                dataframes.append(year_df)
+                                all_df["pub_year"] = df.data_extraction.retrieve_metadata("Year", "pub_year")
                                 used_options.append("pub_year")
                             else:
                                 print("You have already selected this option!")
                         case 4:
                             if "abstract" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                abstract_df = df.data_extraction.retrieve_metadata("Abstract", "abstract")
-                                dataframes.append(abstract_df)
+                                all_df["abstract"] = df.data_extraction.retrieve_metadata("Abstract", "abstract")
                                 used_options.append("abstract")
                             else:
                                 print("You have already selected this option!")
                         case 5: 
                             if "strand_raw" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                admin_strand_df = df.data_extraction.retrieve_data(admin_strand_output, "strand_raw")
-                                dataframes.append(admin_strand_df)
+                                all_df["strand_raw"] = df.data_extraction.retrieve_data(admin_strand_output, "strand_raw")
                                 used_options.append("strand_raw")
                             else:
                                 print("You have already selected this option!")
                         case 6:
                             if "loc_country_raw" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                country_df = df.data_extraction.retrieve_data(countries, "loc_country_raw")
-                                dataframes.append(country_df)
+                                all_df["loc_country_raw"] = df.data_extraction.retrieve_data(countries, "loc_country_raw")
                                 used_options.append("loc_country_raw")
                             else:
                                 print("You have already selected this option!")
                         case 7: 
                             if "pub_eppi" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                pubtype_eppi_df = df.data_extraction.retrieve_metadata("TypeName", "pub_eppi")
-                                dataframes.append(pubtype_eppi_df)
+                                all_df["pub_eppi"] = df.data_extraction.retrieve_metadata("TypeName", "pub_eppi")
                                 used_options.append("pub_eppi")
                             else:
                                 print("You have already selected this option!")
                         case 8: 
                             if "pub_type_raw" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                pub_type_data = df.data_extraction.retrieve_data(publication_type_output, "pub_type_raw")
-                                dataframes.append(pub_type_data)
+                                all_df["pub_type_raw"] = df.data_extraction.retrieve_data(publication_type_output, "pub_type_raw")
                                 used_options.append("pub_type_raw")
                             else:
                                 print("You have already selected this option!")
                         case 9: 
-                            if "int_setting_raw" not in used_options:
-                                row_styles1[num - 1] = highlight_style
-                                edu_setting_data = df.data_extraction.retrieve_data(edu_setting_output, "int_setting_raw")
-                                dataframes.append(edu_setting_data)
-                                used_options.append("int_setting_raw")
-                            else:
-                                print("You have already selected this option!")
-                        case 10: 
                             if "part_age_raw" not in used_options:
                                 row_styles1[num - 1] = highlight_style
                                 student_age_data = df.data_extraction.retrieve_data(student_age_output, "part_age_raw")
-                                dataframes.append(student_age_data)
                                 used_options.append("part_age_raw")
                             else:
                                 print("You have already selected this option!")
-                        case 11: 
-                            if "strand_raw" not in used_options:
-                                row_styles1[num - 1] = highlight_style
-                                admin_strand_data = df.data_extraction.retrieve_data(admin_strand_output, "strand_raw")
-                                dataframes.append(admin_strand_data)
-                                used_options.append("strand_raw")
-                            else:
-                                print("You have already selected this option!")
-                        case 12: 
+                        case 10: 
                             if "eco_valid_raw" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                eco_valid_raw = df.data_extraction.retrieve_data(study_realism_output, "eco_valid_raw")
-                                dataframes.append(eco_valid_raw)
+                                all_df["eco_valid_raw"] = df.data_extraction.retrieve_data(study_realism_output, "eco_valid_raw")
                                 used_options.append("eco_valid_raw")
                             else:
                                 print("You have already selected this option!")
                         #/*************************/#
                         #/     NUMBER OF SCHOOLS   /#
                         #/*************************/#
-                        case 13: 
+                        case 11: 
                             if "school_treat_info" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                number_of_school_int_info = df.data_extraction.retrieve_info(number_of_schools_intervention_output, "school_treat_info")
-                                dataframes.append(number_of_school_int_info)
+                                all_df["school_treat_info"] = df.data_extraction.retrieve_info(number_of_schools_intervention_output, "school_treat_info")
                                 used_options.append("school_treat_info")
                             else:
                                 print("You have already selected this option!")
-                        case 14: 
+                        case 12: 
                             if "school_treat_ht" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                number_of_school_int_ht = df.data_extraction.retrieve_ht(number_of_schools_intervention_output, "school_treat_ht")
-                                dataframes.append(number_of_school_int_ht)
+                                all_df["school_treat_ht"] = df.data_extraction.retrieve_ht(number_of_schools_intervention_output, "school_treat_ht")
                                 used_options.append("school_treat_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 15: 
+                        case 13: 
                             if "school_cont_info" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                number_of_school_control_info = df.data_extraction.retrieve_info(number_of_schools_control_output, "school_cont_info")
-                                dataframes.append(number_of_school_control_info)
+                                all_df["school_cont_info"] = df.data_extraction.retrieve_info(number_of_schools_control_output, "school_cont_info")
                                 used_options.append("school_cont_info")
                             else:
                                 print("You have already selected this option!")
-                        case 16: 
+                        case 14: 
                             if "school_cont_ht" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                number_of_school_control_ht = df.data_extraction.retrieve_ht(number_of_schools_control_output, "school_cont_ht")
-                                dataframes.append(number_of_school_int_ht)
+                                all_df["school_cont_ht"] = df.data_extraction.retrieve_ht(number_of_schools_control_output, "school_cont_ht")
                                 used_options.append("school_cont_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 17: 
+                        case 15: 
                             if "school_total_info" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                number_of_school_total_info = df.data_extraction.retrieve_info(number_of_schools_total_output, "school_total_info")
-                                dataframes.append(number_of_school_total_info)
+                                all_df["school_total_info"] = df.data_extraction.retrieve_info(number_of_schools_total_output, "school_total_info")
                                 used_options.append("school_total_info")
                             else:
                                 print("You have already selected this option!")
-                        case 18: 
+                        case 16: 
                             if "school_total_ht" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                number_of_school_total_ht = df.data_extraction.retrieve_ht(number_of_schools_total_output, "school_total_ht")
-                                dataframes.append(number_of_school_total_ht)
+                                all_df["school_total_ht"] = df.data_extraction.retrieve_ht(number_of_schools_total_output, "school_total_ht")
                                 used_options.append("school_total_ht")
                             else:
                                 print("You have already selected this option!")
                         #/*************************/#
                         #/    NUMBER OF CLASSES    /#
                         #/*************************/#
-                        case 19: 
+                        case 17: 
                             if "class_treat_info" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                number_of_classes_int_info = df.data_extraction.retrieve_info(num_of_class_int_output, "class_treat_info")
-                                dataframes.append(number_of_classes_int_info)
+                                all_df["class_treat_info"] = df.data_extraction.retrieve_info(num_of_class_int_output, "class_treat_info")
                                 used_options.append("class_treat_info")
                             else:
                                 print("You have already selected this option!")
-                        case 20: 
+                        case 18: 
                             if "class_treat_ht" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                number_of_classes_int_ht = df.data_extraction.retrieve_ht(num_of_class_int_output, "class_treat_ht")
-                                dataframes.append(number_of_classes_int_ht)
+                                all_df["class_treat_ht"] = df.data_extraction.retrieve_ht(num_of_class_int_output, "class_treat_ht")
                                 used_options.append("class_treat_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 21: 
+                        case 19: 
                             if "class_cont_info" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                number_of_classes_control_info = df.data_extraction.retrieve_info(num_of_class_cont_output, "class_cont_info")
-                                dataframes.append(number_of_classes_control_info)
+                                all_df["class_cont_info"] = df.data_extraction.retrieve_info(num_of_class_cont_output, "class_cont_info")
                                 used_options.append("class_cont_info")
                             else:
                                 print("You have already selected this option!")
-                        case 22: 
+                        case 20: 
                             if "class_cont_ht" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                number_of_classes_control_ht = df.data_extraction.retrieve_ht(num_of_class_cont_output, "class_cont_ht")
-                                dataframes.append(number_of_classes_control_ht)
+                                all_df["class_cont_ht"] = df.data_extraction.retrieve_ht(num_of_class_cont_output, "class_cont_ht")
                                 used_options.append("class_cont_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 23: 
+                        case 21: 
                             if "class_total_info" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                number_of_classes_total_info = df.data_extraction.retrieve_info(num_of_class_tot_output, "class_total_info")
-                                dataframes.append(number_of_classes_total_info)
+                                all_df["class_total_info"] = df.data_extraction.retrieve_info(num_of_class_tot_output, "class_total_info")
                                 used_options.append("class_total_info")
                             else:
                                 print("You have already selected this option!")
-                        case 24: 
+                        case 22: 
                             if "class_total_ht" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                number_of_classes_total_ht = df.data_extraction.retrieve_ht(num_of_class_tot_output, "class_total_ht")
-                                dataframes.append(number_of_classes_total_ht)
+                                all_df["class_total_ht"] = df.data_extraction.retrieve_ht(num_of_class_tot_output, "class_total_ht")
                                 used_options.append("class_total_ht")
                             else:
                                 print("You have already selected this option!")
                         #/****************************/#
                         #/   PARTICIPANT ASSIGNMENT   /#
                         #/****************************/#
-                        case 25: 
+                        case 23: 
                             if "part_assig_raw" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                part_assig_data = df.data_extraction.retrieve_data(part_assign_output, "part_assig_raw")
-                                dataframes.append(part_assig_data)
+                                all_df["part_assig_raw"] = df.data_extraction.retrieve_data(part_assign_output, "part_assig_raw")
                                 used_options.append("part_assig_raw")
                             else:
                                 print("You have already selected this option!")
-                        case 26: 
+                        case 24: 
                             if "part_assig_ht" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                part_assig_ht = df.data_extraction.retrieve_ht(part_assign_output, "part_assig_ht")
-                                dataframes.append(part_assig_ht)
+                                all_df["part_assig_ht"] = df.data_extraction.retrieve_ht(part_assign_output, "part_assig_ht")
                                 used_options.append("part_assig_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 27: 
+                        case 25: 
                             if "part_assig_info" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                part_assig_info = df.data_extraction.retrieve_info(part_assign_output, "part_assig_info")
-                                dataframes.append(part_assig_ht)
+                                all_df["part_assig_info"] = df.data_extraction.retrieve_info(part_assign_output, "part_assig_info")
                                 used_options.append("part_assig_info")
                             else:
                                 print("You have already selected this option!")
                         #/*************************/#
                         #/   LEVEL OF ASSIGNMENT   /#
                         #/*************************/#
-                        case 28: 
+                        case 26: 
                             if "level_assig_raw" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                level_of_assign_data = df.data_extraction.retrieve_data(level_of_assignment_output, "level_assig_raw")
-                                dataframes.append(level_of_assign_data)
+                                all_df["level_assig_raw"] = df.data_extraction.retrieve_data(level_of_assignment_output, "level_assig_raw")
                                 used_options.append("level_assig_raw")
                             else:
                                 print("You have already selected this option!")
-                        case 29: 
+                        case 27: 
                             if "level_assig_ht" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                level_of_assign_ht = df.data_extraction.retrieve_ht(level_of_assignment_output, "level_assig_ht")
-                                dataframes.append(level_of_assign_ht)
+                                all_df["level_assig_ht"] = df.data_extraction.retrieve_ht(level_of_assignment_output, "level_assig_ht")
                                 used_options.append("level_assig_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 30: 
+                        case 28: 
                             if "level_assig_info" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                level_of_assign_info = df.data_extraction.retrieve_info(level_of_assignment_output, "level_assig_info")
-                                dataframes.append(level_of_assign_info)
+                                all_df["level_assig_info"] = df.data_extraction.retrieve_info(level_of_assignment_output, "level_assig_info")
                                 used_options.append("level_assig_info")
                             else:
                                 print("You have already selected this option!")
                         #/**********************/#
                         #/     STUDY DESIGN     /#
                         #/**********************/#
-                        case 31: 
+                        case 29: 
                             if "int_desig_raw" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                study_design_data = df.data_extraction.retrieve_data(study_design_output, "int_desig_raw")
-                                dataframes.append(study_design_data)
+                                all_df["int_design_raw"] = df.data_extraction.retrieve_data(study_design_output, "int_desig_raw")
                                 used_options.append("int_desig_raw")
                             else:
                                 print("You have already selected this option!")
-                        case 32: 
+                        case 30: 
                             if "int_design_ht" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                study_design_ht = df.data_extraction.retrieve_ht(study_design_output, "int_design_ht")
-                                dataframes.append(study_design_ht)
+                                all_df["int_design_ht"] = df.data_extraction.retrieve_ht(study_design_output, "int_design_ht")
                                 used_options.append("int_design_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 33: 
+                        case 31: 
                             if "int_design_info" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                study_design_info = df.data_extraction.retrieve_info(study_design_output, "int_design_info")
-                                dataframes.append(study_design_info)
+                                all_df["int_design_info"] = df.data_extraction.retrieve_info(study_design_output, "int_design_info")
                                 used_options.append("int_design_info")
                             else:
                                 print("You have already selected this option!")
                         #/**********************/#
                         #/     RANDOMISATION    /#
                         #/**********************/#
-                        case 34: 
+                        case 32: 
                             if "rand_raw" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                rand_data = df.data_extraction.retrieve_data(randomisation_details, "rand_raw")
-                                dataframes.append(rand_data)
+                                all_df["rand_raw"] = df.data_extraction.retrieve_data(randomisation_details, "rand_raw")
                                 used_options.append("rand_raw")
                             else:
                                 print("You have already selected this option!")
-                        case 35: 
+                        case 33: 
                             if "rand_ht" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                rand_ht = df.data_extraction.retrieve_ht(randomisation_details, "rand_ht")
-                                dataframes.append(rand_ht)
+                                all_df["rand_ht"] = df.data_extraction.retrieve_ht(randomisation_details, "rand_ht")
                                 used_options.append("rand_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 36: 
+                        case 34: 
                             if "rand_info" not in used_options:
                                 row_styles1[num - 1] = highlight_style
-                                rand_info = df.data_extraction.retrieve_info(randomisation_details, "rand_info")
-                                dataframes.append(rand_info)
+                                all_df["rand_info"] = df.data_extraction.retrieve_info(randomisation_details, "rand_info")
                                 used_options.append("rand_info")
                             else:
                                 print("You have already selected this option!")
                         #/*************************/#
                         #/ TOOLKIT PRIMARY OUTCOME /#
                         #/*************************/#
+                        case 35:
+                            if "out_tit_tool" not in used_options:
+                                row_styles2[num - 35] = highlight_style
+                                all_df["out_tit_tool"] = df_out.out_tit_tool
+                                used_options.append("out_tit_tool")
+                            else:
+                                print("You have already selected this option!")
+                        case 36:
+                            if "out_desc_tool" not in used_options:
+                                row_styles2[num - 35] = highlight_style
+                                all_df["out_desc_tool"] =  df_out.out_desc_tool
+                                used_options.append("out_desc_tool")
+                            else:
+                                print("You have already selected this option!")
                         case 37:
-                                if "out_tit_tool" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_tit_tool = df_out.out_tit_tool
-                                    dataframes.append(df_out_tit_tool)
-                                    used_options.append("out_tit_tool")
-                                else:
-                                    print("You have already selected this option!")
+                            if "out_type_tool" not in used_options:
+                                row_styles2[num - 35] = highlight_style
+
+                                all_df["out_type_tool"] = df_out.out_type_tool
+                                used_options.append("out_type_tool")
+                            else:
+                                print("You have already selected this option!")
                         case 38:
-                                if "out_desc_tool" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_desc_tool = df_out.out_desc_tool
-                                    dataframes.append(df_out_desc_tool)
-                                    used_options.append("out_desc_tool")
-                                else:
-                                    print("You have already selected this option!")
-                        case 39:
-                                if "out_type_tool" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_type_tool = df_out.out_type_tool
-                                    dataframes.append(df_out_type_tool)
-                                    used_options.append("out_type_tool")
-                                else:
-                                    print("You have already selected this option!")
+                            if "smd_tool" not in used_options:
+                                row_styles2[num - 35] = highlight_style
+                                all_df["smd_tool"] = df_out.smd_tool
+                                used_options.append("smd_tool")
+                            else:
+                                print("You have already selected this option!")
+                        case 49:
+                            if "se_tool" not in used_options:
+                                row_styles2[num - 35] = highlight_style
+                                all_df["se_tool"] = df_out.se_tool
+                                used_options.append("se_tool")
+                            else:
+                                print("You have already selected this option!")
                         case 40:
-                                if "smd_tool" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_smd_tool = df_out.smd_tool
-                                    dataframes.append(df_smd_tool)
-                                    used_options.append("smd_tool")
-                                else:
-                                    print("You have already selected this option!")
+                            if "ci_lower_tool" not in used_options:
+                                row_styles2[num - 35] = highlight_style
+                                all_df["ci_lower_tool"] = df_out.ci_lower_tool
+                                used_options.append("ci_lower_tool")
+                            else:
+                                print("You have already selected this option!")
                         case 41:
-                                if "se_tool" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_se_tool = df_out.se_tool
-                                    dataframes.append(df_se_tool)
-                                    used_options.append("se_tool")
-                                else:
-                                    print("You have already selected this option!")
+                            if "ci_upper_tool" not in used_options:
+                                row_styles2[num - 35] = highlight_style
+                                all_df["ci_upper_tool"] = df_out.ci_upper_tool
+                                used_options.append("ci_upper_tool")
+                            else:
+                                print("You have already selected this option!")
                         case 42:
-                                if "ci_lower_tool" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_ci_lower_tool = df_out.ci_lower_tool
-                                    dataframes.append(df_ci_lower_tool)
-                                    used_options.append("ci_lower_tool")
-                                else:
-                                    print("You have already selected this option!")
+                            if "out_measure_tool" not in used_options:
+                                row_styles2[num - 35] = highlight_style
+                                all_df["out_measure_tool"] = df_out.out_measure_tool
+                                used_options.append("out_measure_tool")
+                            else:
+                                print("You have already selected this option!")
                         case 43:
-                                if "ci_upper_tool" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_ci_upper_tool = df_out.ci_upper_tool
-                                    dataframes.append(df_ci_upper_tool)
-                                    used_options.append("ci_upper_tool")
-                                else:
-                                    print("You have already selected this option!")
+                            if "out_g1_n_tool" not in used_options:
+                                row_styles2[num - 35] = highlight_style
+                                all_df["out_g1_n_tool"] = df_out.out_g1_n_tool
+                                used_options.append("out_g1_n_tool")
+                            else:
+                                print("You have already selected this option!")
                         case 44:
-                                if "out_measure_tool" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_measure_tool = df_out.out_measure_tool
-                                    dataframes.append(df_out_measure_tool)
-                                    used_options.append("out_measure_tool")
-                                else:
-                                    print("You have already selected this option!")
+                            if "out_g1_mean_tool" not in used_options:
+                                row_styles2[num - 35] = highlight_style
+                                all_df["out_g1_mean_tool"] = df_out.out_g1_mean_tool
+                                used_options.append("out_g1_mean_tool")
+                            else:
+                                print("You have already selected this option!")
                         case 45:
-                                if "out_g1_n_tool" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g1_n_tool = df_out.out_g1_n_tool
-                                    dataframes.append(df_g1_n_tool)
-                                    used_options.append("out_g1_n_tool")
-                                else:
-                                    print("You have already selected this option!")
+                            if "out_g1_sd_tool" not in used_options:
+                                row_styles2[num - 35] = highlight_style
+                                all_df["out_g1_sd_tool"] = df_out.out_g1_sd_tool
+                                used_options.append("out_g1_sd_tool")
+                            else:
+                                print("You have already selected this option!")
                         case 46:
-                                if "out_g1_mean_tool" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g1_mean_tool = df_out.out_g1_mean_tool
-                                    dataframes.append(df_g1_mean_tool)
-                                    used_options.append("out_g1_mean_tool")
-                                else:
-                                    print("You have already selected this option!")
+                            if "out_g2_n_tool" not in used_options:
+                                row_styles2[num - 35] = highlight_style
+                                all_df["out_g2_n_tool"] = df_out.out_g2_n_tool
+                                used_options.append("out_g2_n_tool")
+                            else:
+                                print("You have already selected this option!")
                         case 47:
-                                if "out_g1_sd_tool" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g1_sd_tool = df_out.out_g1_sd_tool
-                                    dataframes.append(df_g1_sd_tool)
-                                    used_options.append("out_g1_sd_tool")
-                                else:
-                                    print("You have already selected this option!")
+                            if "out_g2_mean_tool" not in used_options:
+                                row_styles2[num - 35] = highlight_style
+                                all_df["out_g2_mean_tool"] = df_out.out_g2_mean_tool
+                                used_options.append("out_g2_mean_tool")
+                            else:
+                                print("You have already selected this option!")
                         case 48:
-                                if "out_g2_n_tool" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g2_n_tool = df_out.out_g2_n_tool
-                                    dataframes.append(df_g2_n_tool)
-                                    used_options.append("out_g2_n_tool")
-                                else:
-                                    print("You have already selected this option!")
+                            if "out_g2_sd_tool" not in used_options:
+                                row_styles2[num - 35] = highlight_style
+                                all_df["out_g2_sd_tool"] = df_out.out_g2_sd_tool
+                                used_options.append("out_g2_sd_tool")
+                            else:
+                                print("You have already selected this option!")
                         case 49:
-                                if "out_g2_mean_tool" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g2_mean_tool = df_out.out_g2_mean_tool
-                                    dataframes.append(df_g2_mean_tool)
-                                    used_options.append("out_g2_mean_tool")
-                                else:
-                                    print("You have already selected this option!")
+                            if "out_test_type_raw_" not in used_options:
+                                row_styles2[num - 35] = highlight_style
+                                all_df["out_test_type_raw_"] = df_out.out_test_type_raw_tool
+                                used_options.append("out_test_type_raw_")
+                            else:
+                                print("You have already selected this option!")
                         case 50:
-                                if "out_g2_sd_tool" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g2_sd_tool = df_out.out_g2_sd_tool
-                                    dataframes.append(df_g2_sd_tool)
-                                    used_options.append("out_g2_sd_tool")
-                                else:
-                                    print("You have already selected this option!")
-                        case 51:
-                                if "out_test_type_raw_" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_test_type = df_out.out_test_type_raw_tool
-                                    dataframes.append(df_out_test_type)
-                                    used_options.append("out_test_type_raw_")
-                                else:
-                                    print("You have already selected this option!")
-                        case 52:
-                                if "out_es_type_tool" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_es_type = df_out.out_es_type_tool
-                                    dataframes.append(df_out_es_type)
-                                    used_options.append("out_es_type_tool")
-                                else:
-                                    print("You have already selected this option!")
+                            if "out_es_type_tool" not in used_options:
+                                row_styles2[num - 35] = highlight_style
+                                all_df["out_es_type_tool"] = df_out.out_es_type_tool
+                                used_options.append("out_es_type_tool")
+                            else:
+                                print("You have already selected this option!")
                         #/*************************/#
                         #/     READING OUTCOME     /#
                         #/*************************/#
-                        case 53:
+                        case 51:
                                 if "out_tit_red" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_tit_red = df_out.out_tit_red
-                                    dataframes.append(df_out_tit_red)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["out_tit_red"] = df_out.out_tit_red
                                     used_options.append("out_tit_red")
                                 else:
                                     print("You have already selected this option!")
-                        case 54:
+                        case 52:
                                 if "out_desc_red" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_desc_red = df_out.out_desc_red
-                                    dataframes.append(df_out_desc_red)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["out_desc_red"] = df_out.out_desc_red
                                     used_options.append("out_desc_red")
                                 else:
                                     print("You have already selected this option!")
-                        case 55:
+                        case 53:
                                 if "out_type_red" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_type_red = df_out.out_type_red
-                                    dataframes.append(df_out_type_red)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["out_type_red"] = df_out.out_type_red
                                     used_options.append("out_type_red")
                                 else:
                                     print("You have already selected this option!")
-                        case 56:
+                        case 54:
                                 if "smd_red" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_smd_red = df_out.smd_red
-                                    dataframes.append(df_smd_red)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["smd_red"] = df_out.smd_red
                                     used_options.append("smd_red")
                                 else:
                                     print("You have already selected this option!")
-                        case 57:
+                        case 55:
                                 if "se_red" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_se_red = df_out.se_red
-                                    dataframes.append(df_se_red)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["se_red"] = df_out.se_red
                                     used_options.append("se_red")
                                 else:
                                     print("You have already selected this option!")
-                        case 58:
+                        case 56:
                                 if "ci_lower_red" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_ci_lower_red = df_out.ci_lower_red
-                                    dataframes.append(df_ci_lower_red)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["ci_lower_red"] = df_out.ci_lower_red
                                     used_options.append("ci_lower_red")
                                 else:
                                     print("You have already selected this option!")
-                        case 59:
+                        case 57:
                                 if "ci_upper_red" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_ci_upper_red = df_out.ci_upper_red
-                                    dataframes.append(df_ci_upper_red)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["ci_upper_red"] = df_out.ci_upper_red
                                     used_options.append("ci_upper_red")
                                 else:
                                     print("You have already selected this option!")
-                        case 60:
+                        case 58:
                                 if "out_measure_red" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_measure_red = df_out.out_measure_red
-                                    dataframes.append(df_out_measure_red)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["out_measure_red"] = df_out.out_measure_red
                                     used_options.append("out_measure_red")
                                 else:
                                     print("You have already selected this option!")
-                        case 61:
+                        case 59:
                                 if "out_g1_n_red" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g1_n_red = df_out.out_g1_n_red
-                                    dataframes.append(df_g1_n_red)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["out_g1_n_red"] = df_out.out_g1_n_red
                                     used_options.append("out_g1_n_red")
                                 else:
                                     print("You have already selected this option!")
-                        case 62:
+                        case 60:
                                 if "out_g1_mean_red" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g1_mean_red = df_out.out_g1_mean_red
-                                    dataframes.append(df_g1_mean_red)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["out_g1_mean_red"] = df_out.out_g1_mean_red
                                     used_options.append("out_g1_mean_red")
                                 else:
                                     print("You have already selected this option!")
-                        case 63:
+                        case 61:
                                 if "out_g1_sd_red" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g1_sd_red = df_out.out_g1_sd_red
-                                    dataframes.append(df_g1_sd_red)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["out_g1_sd_red"] = df_out.out_g1_sd_red
                                     used_options.append("out_g1_sd_red")
                                 else:
                                     print("You have already selected this option!")
-                        case 64:
+                        case 62:
                                 if "out_g2_n_red" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g2_n_red = df_out.out_g2_n_red
-                                    dataframes.append(df_g2_n_red)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["out_g2_n_red"] = df_out.out_g2_n_red
                                     used_options.append("out_g2_n_red")
                                 else:
                                     print("You have already selected this option!")
-                        case 65:
+                        case 63:
                                 if "out_g2_mean_red" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g2_mean_red = df_out.out_g2_mean_red
-                                    dataframes.append(df_g2_mean_red)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["out_g2_mean_red"] = df_out.out_g2_mean_red
                                     used_options.append("out_g2_mean_red")
                                 else:
                                     print("You have already selected this option!")
-                        case 66:
+                        case 64:
                                 if "out_g2_sd_red" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g2_sd_red = df_out.out_g2_sd_red
-                                    dataframes.append(df_g2_sd_red)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["out_g2_sd_red"] = df_out.out_g2_sd_red
                                     used_options.append("out_g2_sd_red")
                                 else:
                                     print("You have already selected this option!")
-                        case 67:
+                        case 65:
                                 if "out_test_type_raw_red" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_test_type_red = df_out.out_test_type_raw_red
-                                    dataframes.append(df_out_test_type_red)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["out_test_type_raw_red"] = df_out.out_test_type_raw_red
                                     used_options.append("out_test_type_raw_red")
                                 else:
                                     print("You have already selected this option!")
-                        case 68:
+                        case 66:
                                 if "out_es_type_red" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_es_type_red = df_out.out_es_type_red
-                                    dataframes.append(df_out_es_type_red)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["out_es_type_red"] = df_out.out_es_type_red
                                     used_options.append("out_es_type_red")
                                 else:
                                     print("You have already selected this option!")
                         #/*************************/#
                         #/     WRITING OUTCOME     /#
                         #/*************************/#
-                        case 69:
+                        case 67:
                                 if "out_tit_wri" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_tit_wri = df_out.out_tit_wri
-                                    dataframes.append(df_out_tit_wri)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["out_tit_wri"] = df_out.out_tit_wri
                                     used_options.append("out_tit_wri")
                                 else:
                                     print("You have already selected this option!")
-                        case 70:
+                        case 68:
                                 if "out_desc_wri" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_desc_wri = df_out.out_desc_wri
-                                    dataframes.append(df_out_desc_wri)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["out_desc_wri"] = df_out.out_desc_wri
                                     used_options.append("out_desc_wri")
                                 else:
                                     print("You have already selected this option!")
-                        case 71:
+                        case 69:
                                 if "out_type_wri" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_type_wri = df_out.out_type_wri
-                                    dataframes.append(df_out_type_wri)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["out_type_wri"] = df_out.out_type_wri
                                     used_options.append("out_type_wri")
                                 else:
                                     print("You have already selected this option!")
-                        case 72:
+                        case 70:
                                 if "smd_wri" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_smd_wri = df_out.smd_wri
-                                    dataframes.append(df_smd_wri)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["smd_wri"] = df_out.smd_wri
                                     used_options.append("smd_wri")
                                 else:
                                     print("You have already selected this option!")
-                        case 73:
+                        case 71:
                                 if "se_wri" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_se_wri = df_out.se_wri
-                                    dataframes.append(df_se_wri)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["se_wri"] = df_out.se_wri
                                     used_options.append("se_wri")
                                 else:
                                     print("You have already selected this option!")
-                        case 74:
+                        case 72:
                                 if "ci_lower_wri" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_ci_lower_wri = df_out.ci_lower_wri
-                                    dataframes.append(df_ci_lower_wri)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["ci_lower_wri"] = df_out.ci_lower_wri
                                     used_options.append("ci_lower_wri")
                                 else:
                                     print("You have already selected this option!")
-                        case 75:
+                        case 73:
                                 if "ci_upper_wri" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_ci_upper_wri = df_out.ci_upper_wri
-                                    dataframes.append(df_ci_upper_wri)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["ci_upper_wri"] = df_out.ci_upper_wri
                                     used_options.append("ci_upper_wri")
                                 else:
                                     print("You have already selected this option!")
-                        case 76:
+                        case 74:
                                 if "out_measure_wri" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_measure_wri = df_out.out_measure_wri
-                                    dataframes.append(df_out_measure_wri)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["out_measure_wri"] = df_out.out_measure_wri
                                     used_options.append("out_measure_wri")
                                 else:
                                     print("You have already selected this option!")
-                        case 77:
+                        case 75:
                                 if "out_g1_n_wri" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g1_n_wri = df_out.out_g1_n_wri
-                                    dataframes.append(df_g1_n_wri)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["out_g1_n_wri"] = df_out.out_g1_n_wri
                                     used_options.append("out_g1_n_wri")
                                 else:
                                     print("You have already selected this option!")
-                        case 78:
+                        case 76:
                                 if "out_g1_mean_wri" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g1_mean_wri = df_out.out_g1_mean_wri
-                                    dataframes.append(df_g1_mean_wri)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["out_g1_mean_wri"] = df_out.out_g1_mean_wri
                                     used_options.append("out_g1_mean_wri")
                                 else:
                                     print("You have already selected this option!")
-                        case 79:
+                        case 77:
                                 if "out_g1_sd_wri" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g1_sd_wri = df_out.out_g1_sd_wri
-                                    dataframes.append(df_g1_sd_wri)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["out_g1_sd_wri"] = df_out.out_g1_sd_wri
                                     used_options.append("out_g1_sd_wri")
                                 else:
                                     print("You have already selected this option!")
-                        case 80:
+                        case 78:
                                 if "out_g2_n_wri" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g2_n_wri = df_out.out_g2_n_wri
-                                    dataframes.append(df_g2_n_wri)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["out_g2_n_wri"] = df_out.out_g2_n_wri
                                     used_options.append("out_g2_n_wri")
                                 else:
                                     print("You have already selected this option!")
-                        case 81:
+                        case 79:
                                 if "out_g2_mean_wri" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g2_mean_wri = df_out.out_g2_mean_wri
-                                    dataframes.append(df_g2_mean_wri)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["out_g2_mean_wri"] = df_out.out_g2_mean_wri
                                     used_options.append("out_g2_mean_wri")
                                 else:
                                     print("You have already selected this option!")
-                        case 82:
+                        case 80:
                                 if "out_g2_sd_wri" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g2_sd_wri = df_out.out_g2_sd_wri
-                                    dataframes.append(df_g2_sd_wri)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["out_g2_sd_wri"] = df_out.out_g2_sd_wri
                                     used_options.append("out_g2_sd_wri")
                                 else:
                                     print("You have already selected this option!")
-                        case 83:
+                        case 81:
                                 if "out_test_type_raw_wri" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_test_type_wri = df_out.out_test_type_raw_wri
-                                    dataframes.append(df_out_test_type_wri)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["out_test_type_raw_wri"] = df_out.out_test_type_raw_wri
                                     used_options.append("out_test_type_raw_wri")
                                 else:
                                     print("You have already selected this option!")
-                        case 84:
+                        case 82:
                                 if "out_es_type_wri" not in used_options:
-                                    row_styles2[num - 37] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_es_type_wri = df_out.out_es_type_wri
-                                    dataframes.append(df_out_es_type_wri)
+                                    row_styles2[num - 35] = highlight_style
+                                    all_df["out_es_type_wri"] = df_out.out_es_type_wri
                                     used_options.append("out_es_type_wri")
                                 else:
                                     print("You have already selected this option!")
                         #/*************************/#
                         #/        MATH OUTCOME     /#
                         #/*************************/#
-                        case 85:
+                        case 83:
                                 if "out_tit_math" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_tit_math = df_out.out_tit_math
-                                    dataframes.append(df_out_tit_math)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["out_tit_math"] = df_out.out_tit_math
                                     used_options.append("out_tit_math")
                                 else:
                                     print("You have already selected this option!")
-                        case 86:
+                        case 84:
                                 if "out_desc_math" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_desc_math = df_out.out_desc_math
-                                    dataframes.append(df_out_desc_math)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["out_desc_math"] = df_out.out_desc_math
                                     used_options.append("out_desc_math")
                                 else:
                                     print("You have already selected this option!")
-                        case 87:
+                        case 85:
                                 if "out_type_math" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_type_math = df_out.out_type_math
-                                    dataframes.append(df_out_type_math)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["out_type_math"] = df_out.out_type_math
                                     used_options.append("out_type_math")
                                 else:
                                     print("You have already selected this option!")
-                        case 88:
+                        case 86:
                                 if "smd_math" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_smd_math = df_out.smd_math
-                                    dataframes.append(df_smd_math)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["smd_math"] = df_out.smd_math
                                     used_options.append("smd_math")
                                 else:
                                     print("You have already selected this option!")
-                        case 89:
+                        case 87:
                                 if "se_math" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_se_math = df_out.se_math
-                                    dataframes.append(df_se_math)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["se_math"] = df_out.se_math
                                     used_options.append("se_math")
                                 else:
                                     print("You have already selected this option!")
-                        case 90:
+                        case 88:
                                 if "ci_lower_math" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_ci_lower_math = df_out.ci_lower_math
-                                    dataframes.append(df_ci_lower_math)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["ci_lower_math"] = df_out.ci_lower_math
                                     used_options.append("ci_lower_math")
                                 else:
                                     print("You have already selected this option!")
-                        case 91:
+                        case 89:
                                 if "ci_upper_math" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_ci_upper_math = df_out.ci_upper_math
-                                    dataframes.append(df_ci_upper_math)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["ci_upper_math"] = df_out.ci_upper_math
                                     used_options.append("ci_upper_math")
                                 else:
                                     print("You have already selected this option!")
-                        case 92:
+                        case 90:
                                 if "out_measure_math" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_measure_math = df_out.out_measure_math
-                                    dataframes.append(df_out_measure_math)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["out_measure_math"] = df_out.out_measure_math
                                     used_options.append("out_measure_math")
                                 else:
                                     print("You have already selected this option!")
-                        case 93:
+                        case 91:
                                 if "out_g1_n_math" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g1_n_math = df_out.out_g1_n_math
-                                    dataframes.append(df_g1_n_math)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["out_g1_n_math"] = df_out.out_g1_n_math
                                     used_options.append("out_g1_n_math")
                                 else:
                                     print("You have already selected this option!")
-                        case 94:
+                        case 92:
                                 if "out_g1_mean_math" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g1_mean_math = df_out.out_g1_mean_math
-                                    dataframes.append(df_g1_mean_math)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["out_g1_mean_math"] = df_out.out_g1_mean_math
                                     used_options.append("out_g1_mean_math")
                                 else:
                                     print("You have already selected this option!")
-                        case 95:
+                        case 93:
                                 if "out_g1_sd_math" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g1_sd_math = df_out.out_g1_sd_math
-                                    dataframes.append(df_g1_sd_math)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["out_g1_sd_math"] = df_out.out_g1_sd_math
                                     used_options.append("out_g1_sd_math")
                                 else:
                                     print("You have already selected this option!")
-                        case 96:
+                        case 94:
                                 if "out_g2_n_math" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g2_n_math = df_out.out_g2_n_math
-                                    dataframes.append(df_g2_n_math)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["out_g2_n_math"] = df_out.out_g2_n_math
                                     used_options.append("out_g2_n_math")
                                 else:
                                     print("You have already selected this option!")
-                        case 97:
+                        case 95:
                                 if "out_g2_mean_math" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g2_mean_math = df_out.out_g2_mean_math
-                                    dataframes.append(df_g2_mean_math)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["out_g2_mean_math"] = df_out.out_g2_mean_math
                                     used_options.append("out_g2_mean_math")
                                 else:
                                     print("You have already selected this option!")
-                        case 98:
+                        case 96:
                                 if "out_g2_sd_math" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g2_sd_math = df_out.out_g2_sd_math
-                                    dataframes.append(df_g2_sd_math)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["out_g2_sd_math"] = df_out.out_g2_sd_math
                                     used_options.append("out_g2_sd_math")
                                 else:
                                     print("You have already selected this option!")
-                        case 99:
+                        case 97:
                                 if "out_test_type_raw_math" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_test_type_math = df_out.out_test_type_raw_math
-                                    dataframes.append(df_out_test_type_math)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["out_test_type_raw_math"] = df_out.out_test_type_raw_math
                                     used_options.append("out_test_type_raw_math")
                                 else:
                                     print("You have already selected this option!")
-                        case 100:
+                        case 98:
                                 if "out_es_type_math" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_es_type_math = df_out.out_es_type_math
-                                    dataframes.append(df_out_es_type_math)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["out_es_type_math"] = df_out.out_es_type_math
                                     used_options.append("out_es_type_math")
                                 else:
                                     print("You have already selected this option!")
                         #/*************************/#
                         #/     SCIENCE OUTCOME     /#
                         #/*************************/#
-                        case 101:
+                        case 99:
                                 if "out_tit_sci" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_tit_sci = df_out.out_tit_sci
-                                    dataframes.append(df_out_tit_sci)
+                                    row_styles3[num - 83] = highlight_style
+
+                                    all_df["out_tit_sci"] = df_out.out_tit_sci
                                     used_options.append("out_tit_sci")
                                 else:
                                     print("You have already selected this option!")
-                        case 102:
+                        case 100:
                                 if "out_desc_sci" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_desc_sci = df_out.out_desc_sci
-                                    dataframes.append(df_out_desc_sci)
+                                    row_styles3[num - 83] = highlight_style
+
+                                    all_df["out_desc_sci"] = df_out.out_desc_sci
                                     used_options.append("out_desc_sci")
                                 else:
                                     print("You have already selected this option!")
-                        case 103:
+                        case 101:
                                 if "out_type_sci" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_type_sci = df_out.out_type_sci
-                                    dataframes.append(df_out_type_sci)
+                                    row_styles3[num - 83] = highlight_style
+
+                                    all_df["out_type_sci"] = df_out.out_type_sci
                                     used_options.append("out_type_sci")
                                 else:
                                     print("You have already selected this option!")
-                        case 104:
+                        case 102:
                                 if "smd_sci" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_smd_sci = df_out.smd_sci
-                                    dataframes.append(df_smd_sci)
+                                    row_styles3[num - 83] = highlight_style
+
+                                    all_df["smd_sci"] = df_out.smd_sci
                                     used_options.append("smd_sci")
                                 else:
                                     print("You have already selected this option!")
-                        case 105:
+                        case 103:
                                 if "se_sci" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_se_sci = df_out.se_sci
-                                    dataframes.append(df_se_sci)
+                                    row_styles3[num - 83] = highlight_style
+
+                                    all_df["se_sci"] = df_out.se_sci
                                     used_options.append("se_sci")
                                 else:
                                     print("You have already selected this option!")
-                        case 106:
+                        case 104:
                                 if "ci_lower_sci" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_ci_lower_sci = df_out.ci_lower_sci
-                                    dataframes.append(df_ci_lower_sci)
+                                    row_styles3[num - 83] = highlight_style
+
+                                    all_df["ci_lower_sci"] = df_out.ci_lower_sci
                                     used_options.append("ci_lower_sci")
                                 else:
                                     print("You have already selected this option!")
-                        case 107:
+                        case 105:
                                 if "ci_upper_sci" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_ci_upper_sci = df_out.ci_upper_sci
-                                    dataframes.append(df_ci_upper_sci)
+                                    row_styles3[num - 83] = highlight_style
+
+                                    all_df["ci_upper_sci"] = df_out.ci_upper_sci
                                     used_options.append("ci_upper_sci")
                                 else:
                                     print("You have already selected this option!")
-                        case 108:
+                        case 106:
                                 if "out_measure_sci" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_measure_sci = df_out.out_measure_sci
-                                    dataframes.append(df_out_measure_sci)
+                                    row_styles3[num - 83] = highlight_style
+
+                                    all_df["out_measure_sci"] = df_out.out_measure_sci
                                     used_options.append("out_measure_sci")
                                 else:
                                     print("You have already selected this option!")
-                        case 109:
+                        case 107:
                                 if "out_g1_n_sci" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g1_n_sci = df_out.out_g1_n_sci
-                                    dataframes.append(df_g1_n_sci)
+                                    row_styles3[num - 83] = highlight_style
+
+                                    all_df["out_g1_n_sci"] = df_out.out_g1_n_sci
                                     used_options.append("out_g1_n_sci")
                                 else:
                                     print("You have already selected this option!")
-                        case 110:
+                        case 108:
                                 if "out_g1_mean_sci" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g1_mean_sci = df_out.out_g1_mean_sci
-                                    dataframes.append(df_g1_mean_sci)
+                                    row_styles3[num - 83] = highlight_style
+
+                                    all_df["out_g1_mean_sci"] = df_out.out_g1_mean_sci
                                     used_options.append("out_g1_mean_sci")
                                 else:
                                     print("You have already selected this option!")
-                        case 111:
+                        case 109:
                                 if "out_g1_sd_sci" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g1_sd_sci = df_out.out_g1_sd_sci
-                                    dataframes.append(df_g1_sd_sci)
+                                    row_styles3[num - 83] = highlight_style
+
+                                    all_df["out_g1_sd_sci"] = df_out.out_g1_sd_sci
                                     used_options.append("out_g1_sd_sci")
                                 else:
                                     print("You have already selected this option!")
-                        case 112:
+                        case 110:
                                 if "out_g2_n_sci" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g2_n_sci = df_out.out_g2_n_sci
-                                    dataframes.append(df_g2_n_sci)
+                                    row_styles3[num - 83] = highlight_style
+
+                                    all_df["out_g2_n_sci"] = df_out.out_g2_n_sci
                                     used_options.append("out_g2_n_sci")
                                 else:
                                     print("You have already selected this option!")
-                        case 113:
+                        case 111:
                                 if "out_g2_mean_sci" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g2_mean_sci = df_out.out_g2_mean_sci
-                                    dataframes.append(df_g2_mean_sci)
+                                    row_styles3[num - 83] = highlight_style
+
+                                    all_df["out_g2_mean_sci"] = df_out.out_g2_mean_sci
                                     used_options.append("out_g2_mean_sci")
                                 else:
                                     print("You have already selected this option!")
-                        case 114:
+                        case 112:
                                 if "out_g2_sd_sci" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g2_sd_sci = df_out.out_g2_sd_sci
-                                    dataframes.append(df_g2_sd_sci)
+                                    row_styles3[num - 83] = highlight_style
+
+                                    all_df["out_g2_sd_sci"] = df_out.out_g2_sd_sci
                                     used_options.append("out_g2_sd_sci")
                                 else:
                                     print("You have already selected this option!")
-                        case 115:
+                        case 113:
                                 if "out_test_type_raw_sci" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_test_type_sci = df_out.out_test_type_raw_sci
-                                    dataframes.append(df_out_test_type_sci)
+                                    row_styles3[num - 83] = highlight_style
+
+                                    all_df["out_test_type_raw_sci"] = df_out.out_test_type_raw_sci
                                     used_options.append("out_test_type_raw_sci")
                                 else:
                                     print("You have already selected this option!")
-                        case 116:
+                        case 114:
                                 if "out_es_type_sci" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_es_type_sci = df_out.out_es_type_sci
-                                    dataframes.append(df_out_es_type_sci)
+                                    row_styles3[num - 83] = highlight_style
+
+                                    all_df["out_es_type_sci"] = df_out.out_es_type_sci
                                     used_options.append("out_es_type_sci")
                                 else:
                                     print("You have already selected this option!")
                         #/*************************/#
                         #/        FSM OUTCOME      /#
                         #/*************************/#
-                        case 117:
+                        case 115:
                                 if "out_tit_fsm" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_tit_fsm = df_out.out_tit_fsm
-                                    dataframes.append(df_out_tit_fsm)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["out_tit_fsm"] = df_out.out_tit_fsm
                                     used_options.append("out_tit_fsm")
                                 else:
                                     print("You have already selected this option!")
-                        case 118:
+                        case 116:
                                 if "out_desc_fsm" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_desc_fsm = df_out.out_desc_fsm
-                                    dataframes.append(df_out_desc_fsm)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["out_desc_fsm"] = df_out.out_desc_fsm
                                     used_options.append("out_desc_fsm")
                                 else:
                                     print("You have already selected this option!")
-                        case 119:
+                        case 117:
                                 if "out_type_fsm" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_type_fsm = df_out.out_type_fsm
-                                    dataframes.append(df_out_type_fsm)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["out_type_fsm"] = df_out.out_type_fsm
                                     used_options.append("out_type_fsm")
                                 else:
                                     print("You have already selected this option!")
-                        case 120:
+                        case 118:
                                 if "smd_fsm" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_smd_fsm = df_out.smd_fsm
-                                    dataframes.append(df_smd_fsm)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["smd_fsm"] = df_out.smd_fsm
                                     used_options.append("smd_fsm")
                                 else:
                                     print("You have already selected this option!")
-                        case 121:
+                        case 119:
                                 if "se_fsm" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_se_fsm = df_out.se_fsm
-                                    dataframes.append(df_se_fsm)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["se_fsm"] = df_out.se_fsm
                                     used_options.append("se_fsm")
                                 else:
                                     print("You have already selected this option!")
-                        case 122:
+                        case 120:
                                 if "ci_lower_fsm" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_ci_lower_fsm = df_out.ci_lower_fsm
-                                    dataframes.append(df_ci_lower_fsm)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["ci_lower_fsm"] = df_out.ci_lower_fsm
                                     used_options.append("ci_lower_fsm")
                                 else:
                                     print("You have already selected this option!")
-                        case 123:
+                        case 121:
                                 if "ci_upper_fsm" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_ci_upper_fsm = df_out.ci_upper_fsm
-                                    dataframes.append(df_ci_upper_fsm)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["ci_upper_fsm"] = df_out.ci_upper_fsm
                                     used_options.append("ci_upper_fsm")
                                 else:
                                     print("You have already selected this option!")
-                        case 124:
+                        case 122:
                                 if "out_measure_fsm" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_measure_fsm = df_out.out_measure_fsm
-                                    dataframes.append(df_out_measure_fsm)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["out_measure_fsm"] = df_out.out_measure_fsm
                                     used_options.append("out_measure_fsm")
                                 else:
                                     print("You have already selected this option!")
-                        case 125:
+                        case 123:
                                 if "out_g1_n_fsm" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g1_n_fsm = df_out.out_g1_n_fsm
-                                    dataframes.append(df_g1_n_fsm)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["out_g1_n_fsm"] = df_out.out_g1_n_fsm
                                     used_options.append("out_g1_n_fsm")
                                 else:
                                     print("You have already selected this option!")
-                        case 126:
+                        case 124:
                                 if "out_g1_mean_fsm" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g1_mean_fsm = df_out.out_g1_mean_fsm
-                                    dataframes.append(df_g1_mean_fsm)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["out_g1_mean_fsm"] = df_out.out_g1_mean_fsm
                                     used_options.append("out_g1_mean_fsm")
                                 else:
                                     print("You have already selected this option!")
-                        case 127:
+                        case 125:
                                 if "out_g1_sd_fsm" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g1_sd_fsm = df_out.out_g1_sd_fsm
-                                    dataframes.append(df_g1_sd_fsm)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["out_g1_sd_fsm"] = df_out.out_g1_sd_fsm
                                     used_options.append("out_g1_sd_fsm")
                                 else:
                                     print("You have already selected this option!")
-                        case 128:
+                        case 126:
                                 if "out_g2_n_fsm" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g2_n_fsm = df_out.out_g2_n_fsm
-                                    dataframes.append(df_g2_n_fsm)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["out_g2_n_fsm"] = df_out.out_g2_n_fsm
                                     used_options.append("out_g2_n_fsm")
                                 else:
                                     print("You have already selected this option!")
-                        case 129:
+                        case 127:
                                 if "out_g2_mean_fsm" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g2_mean_fsm = df_out.out_g2_mean_fsm
-                                    dataframes.append(df_g2_mean_fsm)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["out_g2_mean_fsm"] = df_out.out_g2_mean_fsm
                                     used_options.append("out_g2_mean_fsm")
                                 else:
                                     print("You have already selected this option!")
-                        case 130:
+                        case 128:
                                 if "out_g2_sd_fsm" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_g2_sd_fsm = df_out.out_g2_sd_fsm
-                                    dataframes.append(df_g2_sd_fsm)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["out_g2_sd_fsm"] = df_out.out_g2_sd_fsm
                                     used_options.append("out_g2_sd_fsm")
                                 else:
                                     print("You have already selected this option!")
-                        case 131:
+                        case 129:
                                 if "out_test_type_raw_fsm" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_test_type_fsm = df_out.out_test_type_raw_fsm
-                                    dataframes.append(df_out_test_type_fsm)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["out_test_type_raw_fsm"] = df_out.out_test_type_raw_fsm
                                     used_options.append("out_test_type_raw_fsm")
                                 else:
                                     print("You have already selected this option!")
-                        case 132:
+                        case 130:
                                 if "out_es_type_fsm" not in used_options:
-                                    row_styles3[num - 85] = highlight_style
-                                    df_outcomes = DataFrameCompilation(json_extractor)
-                                    df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
-                                    df_out_es_type_fsm = df_out.out_es_type_fsm
-                                    dataframes.append(df_out_es_type_fsm)
+                                    row_styles3[num - 83] = highlight_style
+                                    all_df["out_es_type_fsm"] = df_out.out_es_type_fsm
                                     used_options.append("out_es_type_fsm")
                                 else:
                                     print("You have already selected this option!")
                         #/*****************************/#
                         #/     INTERVENTION DETAILS    /#
                         #/*****************************/#
-                        case 133: 
+                        case 131: 
                             if "intervention_name_ht" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                intervention_name_ht = df.data_extraction.retrieve_ht(int_name_output, "intervention_name_ht")
-                                dataframes.append(intervention_name_ht)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_name_ht"] = df.data_extraction.retrieve_ht(int_name_output, "intervention_name_ht")
                                 used_options.append("intervention_name_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 134: 
+                        case 132: 
                             if "int_name_info" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                intervention_name_info = df.data_extraction.retrieve_info(int_name_output, "int_name_info")
-                                dataframes.append(intervention_name_info)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_name_info"] = df.data_extraction.retrieve_info(int_name_output, "int_name_info")
                                 used_options.append("int_name_info")
                             else:
                                 print("You have already selected this option!")
-                        case 135: 
+                        case 133: 
                             if "intervention_desc_ht" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                intervention_desc_ht = df.data_extraction.retrieve_ht(intervention_description_output, "intervention_desc_ht")
-                                dataframes.append(intervention_desc_ht)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_desc_ht"] = df.data_extraction.retrieve_ht(intervention_description_output, "intervention_desc_ht")
                                 used_options.append("intervention_desc_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 136: 
+                        case 134: 
                             if "intervention_desc_info" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                intervention_desc_info = df.data_extraction.retrieve_info(intervention_description_output, "intervention_desc_info")
-                                dataframes.append(intervention_desc_info)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_desc_info"] = df.data_extraction.retrieve_info(intervention_description_output, "intervention_desc_info")
                                 used_options.append("intervention_desc_info")
                             else:
                                 print("You have already selected this option!")
-                        case 137: 
+                        case 135: 
                             if "intervention_objec_ht" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                intervention_desc_ht = df.data_extraction.retrieve_ht(intervention_objectives_output, "intervention_objec_ht")
-                                dataframes.append(intervention_desc_ht)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_objec_ht"] = df.data_extraction.retrieve_ht(intervention_objectives_output, "intervention_objec_ht")
                                 used_options.append("intervention_objec_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 138: 
+                        case 136: 
                             if "intervention_objec_info" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                intervention_desc_info = df.data_extraction.retrieve_info(intervention_objectives_output, "intervention_objec_info")
-                                dataframes.append(intervention_desc_info)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_objec_info"] = df.data_extraction.retrieve_info(intervention_objectives_output, "intervention_objec_info")
                                 used_options.append("intervention_objec_info")
                             else:
                                 print("You have already selected this option!")
-                        case 139: 
+                        case 137: 
                             if "int_training_raw" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                intervention_training_prov_data = df.data_extraction.retrieve_data(int_training_provided_output, "int_training_raw")
-                                dataframes.append(intervention_training_prov_data)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_training_raw"] = df.data_extraction.retrieve_data(int_training_provided_output, "int_training_raw")
                                 used_options.append("int_training_raw")
                             else:
                                 print("You have already selected this option!")
-                        case 140: 
+                        case 138: 
                             if "int_training_ht" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                intervention_training_prov_ht = df.data_extraction.retrieve_ht(int_training_provided_output, "int_training_ht")
-                                dataframes.append(intervention_training_prov_ht)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_training_ht"] = df.data_extraction.retrieve_ht(int_training_provided_output, "int_training_ht")
                                 used_options.append("int_training_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 141: 
+                        case 139: 
                             if "int_training_info" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                intervention_training_prov_info = df.data_extraction.retrieve_info(int_training_provided_output, "int_training_info")
-                                dataframes.append(intervention_training_prov_info)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_training_info"] = df.data_extraction.retrieve_info(int_training_provided_output, "int_training_info")
                                 used_options.append("int_training_info")
                             else:
                                 print("You have already selected this option!")
-                        case 142: 
+                        case 140: 
                             if "int_approach_raw" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                intervention_teaching_app_data = df.data_extraction.retrieve_data(intervention_teaching_approach, "int_approach_raw")
-                                dataframes.append(intervention_teaching_app_data)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_approach_raw"] = df.data_extraction.retrieve_data(intervention_teaching_approach, "int_approach_raw")
                                 used_options.append("int_approach_raw")
                             else:
                                 print("You have already selected this option!")
-                        case 143: 
+                        case 141: 
                             if "int_approach_ht" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                intervention_training_prov_ht = df.data_extraction.retrieve_ht(intervention_teaching_approach, "int_approach_ht")
-                                dataframes.append(intervention_training_prov_ht)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_approach_ht"] = df.data_extraction.retrieve_ht(intervention_teaching_approach, "int_approach_ht")
                                 used_options.append("int_approach_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 144: 
+                        case 142: 
                             if "int_approach_info" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                intervention_training_prov_info = df.data_extraction.retrieve_info(intervention_teaching_approach, "int_approach_info")
-                                dataframes.append(intervention_training_prov_info)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_approach_info"] = df.data_extraction.retrieve_info(intervention_teaching_approach, "int_approach_info")
                                 used_options.append("int_approach_info")
                             else:
                                 print("You have already selected this option!")
-                        case 145: 
+                        case 143: 
                             if "digit_tech_raw" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                digit_tech_data = df.data_extraction.retrieve_data(int_appr_dig_tech, "digit_tech_raw")
-                                dataframes.append(digit_tech_data)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["digit_tech_raw"] = df.data_extraction.retrieve_data(int_appr_dig_tech, "digit_tech_raw")
                                 used_options.append("digit_tech_raw")
                             else:
                                 print("You have already selected this option!")
-                        case 146: 
+                        case 144: 
                             if "digit_tech_ht" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                digit_tech_ht = df.data_extraction.retrieve_ht(int_appr_dig_tech, "digit_tech_ht")
-                                dataframes.append(digit_tech_ht)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["digit_tech_ht"] = df.data_extraction.retrieve_ht(int_appr_dig_tech, "digit_tech_ht")
                                 used_options.append("digit_tech_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 147: 
+                        case 145: 
                             if "digit_tech_info" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                digit_tech_info = df.data_extraction.retrieve_info(int_appr_dig_tech, "digit_tech_info")
-                                dataframes.append(digit_tech_info)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["digit_tech_info"] = df.data_extraction.retrieve_info(int_appr_dig_tech, "digit_tech_info")
                                 used_options.append("digit_tech_info")
                             else:
                                 print("You have already selected this option!")
-                        case 148: 
+                        case 146: 
                             if "parent_partic_raw" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                par_eng_data = df.data_extraction.retrieve_data(int_appr_par_or_comm_vol, "parent_partic_raw")
-                                dataframes.append(par_eng_data)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["parent_partic_raw"] = df.data_extraction.retrieve_data(int_appr_par_or_comm_vol, "parent_partic_raw")
                                 used_options.append("parent_partic_raw")
                             else:
                                 print("You have already selected this option!")
-                        case 149: 
+                        case 147: 
                             if "parent_partic_ht" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                par_eng_ht = df.data_extraction.retrieve_ht(int_appr_par_or_comm_vol, "parent_partic_ht")
-                                dataframes.append(par_eng_ht)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["parent_partic_ht"] = df.data_extraction.retrieve_ht(int_appr_par_or_comm_vol, "parent_partic_ht")
                                 used_options.append("parent_partic_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 150: 
+                        case 148: 
                             if "parent_partic_info" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                par_eng_info = df.data_extraction.retrieve_info(int_appr_par_or_comm_vol, "parent_partic_info")
-                                dataframes.append(par_eng_info)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["parent_partic_info"] = df.data_extraction.retrieve_info(int_appr_par_or_comm_vol, "parent_partic_info")
                                 used_options.append("parent_partic_info")
                             else:
                                 print("You have already selected this option!")
-                        case 151: 
+                        case 149: 
                             if "int_when_raw" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                intervention_time_data = df.data_extraction.retrieve_data(intervention_time_output, "int_when_raw")
-                                dataframes.append(intervention_time_data)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_when_raw"] = df.data_extraction.retrieve_data(intervention_time_output, "int_when_raw")
                                 used_options.append("int_when_raw")
                             else:
                                 print("You have already selected this option!")
-                        case 152: 
+                        case 150: 
                             if "int_when_ht" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                intervention_time_ht = df.data_extraction.retrieve_ht(intervention_time_output, "int_when_ht")
-                                dataframes.append(intervention_time_ht)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_when_ht"] = df.data_extraction.retrieve_ht(intervention_time_output, "int_when_ht")
                                 used_options.append("int_when_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 153: 
+                        case 151: 
                             if "int_when_info" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                intervention_time_info = df.data_extraction.retrieve_info(intervention_time_output, "int_when_info")
-                                dataframes.append(intervention_time_info)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_when_info"] = df.data_extraction.retrieve_info(intervention_time_output, "int_when_info")
                                 used_options.append("int_when_info")
                             else:
                                 print("You have already selected this option!")
-                        case 154: 
+                        case 152: 
                             if "int_who_raw" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                intervention_delivery_data = df.data_extraction.retrieve_data(intervention_delivery_output, "int_who_raw")
-                                dataframes.append(intervention_delivery_data)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_who_raw"] = df.data_extraction.retrieve_data(intervention_delivery_output, "int_who_raw")
                                 used_options.append("int_who_raw")
                             else:
                                 print("You have already selected this option!")
-                        case 155: 
+                        case 153: 
                             if "int_who_ht" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                intervention_delivery_ht = df.data_extraction.retrieve_ht(intervention_delivery_output, "int_who_ht")
-                                dataframes.append(intervention_delivery_ht)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_who_ht"] = df.data_extraction.retrieve_ht(intervention_delivery_output, "int_who_ht")
                                 used_options.append("int_who_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 156: 
+                        case 154: 
                             if "int_who_info" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                intervention_delivery_info = df.data_extraction.retrieve_info(intervention_delivery_output, "int_who_info")
-                                dataframes.append(intervention_delivery_info)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_who_info"] = df.data_extraction.retrieve_info(intervention_delivery_output, "int_who_info")
                                 used_options.append("int_who_info")
                             else:
                                 print("You have already selected this option!")
-                        case 157: 
+                        case 155: 
                             if "int_dur_ht" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                intervention_duration_ht = df.data_extraction.retrieve_ht(int_dur_output, "int_dur_ht")
-                                dataframes.append(intervention_duration_ht)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_dur_ht"] = df.data_extraction.retrieve_ht(int_dur_output, "int_dur_ht")
                                 used_options.append("int_dur_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 158: 
+                        case 156: 
                             if "int_dur_info" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                intervention_duration_info = df.data_extraction.retrieve_info(int_dur_output, "int_dur_info")
-                                dataframes.append(intervention_duration_info)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_dur_info"] = df.data_extraction.retrieve_info(int_dur_output, "int_dur_info")
                                 used_options.append("int_dur_info")
                             else:
                                 print("You have already selected this option!")
-                        case 159: 
+                        case 157: 
                             if "int_leng_ht" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                intervention_duration_ht = df.data_extraction.retrieve_ht(intervention_session_length_output, "int_leng_ht")
-                                dataframes.append(intervention_duration_ht)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_leng_ht"] = df.data_extraction.retrieve_ht(intervention_session_length_output, "int_leng_ht")
                                 used_options.append("int_leng_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 160: 
+                        case 158: 
                             if "int_leng_info" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                intervention_sess_length_info = df.data_extraction.retrieve_info(intervention_session_length_output, "int_leng_info")
-                                dataframes.append(intervention_sess_length_info)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_leng_info"] = df.data_extraction.retrieve_info(intervention_session_length_output, "int_leng_info")
                                 used_options.append("int_leng_info")
                             else:
                                 print("You have already selected this option!")
-                        case 161: 
+                        case 159: 
                             if "int_setting_raw" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                edu_setting_data = df.data_extraction.retrieve_info(edu_setting_output, "int_setting_raw")
-                                dataframes.append(edu_setting_data)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_setting_raw"] = df.data_extraction.retrieve_info(edu_setting_output, "int_setting_raw")
                                 used_options.append("int_setting_raw")
                             else:
                                 print("You have already selected this option!")
-                        case 162: 
+                        case 160: 
                             if "int_setting_ht" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                edu_setting_ht = df.data_extraction.retrieve_ht(edu_setting_output, "int_setting_ht")
-                                dataframes.append(edu_setting_ht)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_setting_ht"] = df.data_extraction.retrieve_ht(edu_setting_output, "int_setting_ht")
                                 used_options.append("int_setting_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 163: 
+                        case 161: 
                             if "int_setting_info" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                edu_setting_info = df.data_extraction.retrieve_info(edu_setting_output, "int_setting_info")
-                                dataframes.append(edu_setting_info)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_setting_info"] = df.data_extraction.retrieve_info(edu_setting_output, "int_setting_info")
                                 used_options.append("int_setting_info")
                             else:
                                 print("You have already selected this option!")
-                        case 164: 
+                        case 162: 
                             if "int_part_raw" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                int_focus = df.data_extraction.retrieve_info(int_focus_output, "int_part_raw")
-                                dataframes.append(int_focus)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_part_raw"] = df.data_extraction.retrieve_info(int_focus_output, "int_part_raw")
                                 used_options.append("int_part_raw")
                             else:
                                 print("You have already selected this option!")
-                        case 165: 
+                        case 163: 
                             if "int_part_ht" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                int_focus_ht = df.data_extraction.retrieve_info(int_focus_output, "int_part_ht")
-                                dataframes.append(int_focus_ht)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_part_ht"] = df.data_extraction.retrieve_info(int_focus_output, "int_part_ht")
                                 used_options.append("int_part_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 166: 
+                        case 164: 
                             if "int_part_info" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                int_focus_info = df.data_extraction.retrieve_info(int_focus_output, "int_part_info")
-                                dataframes.append(int_focus_info)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_part_info"] = df.data_extraction.retrieve_info(int_focus_output, "int_part_info")
                                 used_options.append("int_part_info")
                             else:
                                 print("You have already selected this option!")
-                        case 167: 
+                        case 165: 
                             if "int_fidel_raw" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                int_fidel = df.data_extraction.retrieve_data(int_impl_details, "int_fidel_raw")
-                                dataframes.append(int_fidel)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_fidel_raw"] = df.data_extraction.retrieve_data(int_impl_details, "int_fidel_raw")
                                 used_options.append("int_fidel_raw")
                             else:
                                 print("You have already selected this option!")
-                        case 168: 
+                        case 166: 
                             if "int_fidel_ht" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                int_fidel_ht = df.data_extraction.retrieve_ht(int_impl_details, "int_fidel_ht")
-                                dataframes.append(int_fidel_ht)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_fidel_ht"] = df.data_extraction.retrieve_ht(int_impl_details, "int_fidel_ht")
                                 used_options.append("int_fidel_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 169: 
+                        case 167: 
                             if "int_fidel_info" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                int_fidel_ht_info = df.data_extraction.retrieve_info(int_impl_details, "int_fidel_info")
-                                dataframes.append(int_fidel_ht_info)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_fidel_info"] = df.data_extraction.retrieve_info(int_impl_details, "int_fidel_info")
                                 used_options.append("int_fidel_info")
                             else:
                                 print("You have already selected this option!")
-                        case 170: 
+                        case 168: 
                             if "int_cost_raw" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                int_cost = df.data_extraction.retrieve_data(int_costs_reported, "int_cost_raw")
-                                dataframes.append(int_cost)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_cost_raw"] = df.data_extraction.retrieve_data(int_costs_reported, "int_cost_raw")
                                 used_options.append("int_cost_raw")
                             else:
                                 print("You have already selected this option!")
-                        case 171: 
+                        case 169: 
                             if "int_cost_ht" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                int_cost_ht = df.data_extraction.retrieve_ht(int_costs_reported, "int_cost_ht")
-                                dataframes.append(int_cost_ht)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_cost_ht"] = df.data_extraction.retrieve_ht(int_costs_reported, "int_cost_ht")
                                 used_options.append("int_cost_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 172: 
+                        case 170: 
                             if "int_cost_info" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                int_cost_info = df.data_extraction.retrieve_info(int_costs_reported, "int_cost_info")
-                                dataframes.append(int_cost_info)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["int_cost_info"] = df.data_extraction.retrieve_info(int_costs_reported, "int_cost_info")
                                 used_options.append("int_cost_info")
                             else:
                                 print("You have already selected this option!")
-                        case 173: 
+                        case 171: 
                             if "base_diff_raw" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                base_diff = df.data_extraction.retrieve_data(baseline_diff_output, "base_diff_raw")
-                                dataframes.append(base_diff)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["base_diff_raw"] = df.data_extraction.retrieve_data(baseline_diff_output, "base_diff_raw")
                                 used_options.append("base_diff_raw")
                             else:
                                 print("You have already selected this option!")
-                        case 174: 
+                        case 172: 
                             if "base_diff_ht" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                base_diff_ht = df.data_extraction.retrieve_ht(baseline_diff_output, "base_diff_ht")
-                                dataframes.append(base_diff_ht)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["base_diff_ht"] = df.data_extraction.retrieve_ht(baseline_diff_output, "base_diff_ht")
                                 used_options.append("base_diff_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 175: 
+                        case 173: 
                             if "base_diff_info" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                base_diff_info = df.data_extraction.retrieve_info(baseline_diff_output, "base_diff_info")
-                                dataframes.append(base_diff_info)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["base_diff_info"] = df.data_extraction.retrieve_info(baseline_diff_output, "base_diff_info")
                                 used_options.append("base_diff_info")
                             else:
                                 print("You have already selected this option!")
-                        case 176: 
+                        case 174: 
                             if "comp_anal_raw" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                comp_anal = df.data_extraction.retrieve_data(comparability_output, "comp_anal_raw")
-                                dataframes.append(comp_anal)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["comp_anal_raw"] = df.data_extraction.retrieve_data(comparability_output, "comp_anal_raw")
                                 used_options.append("comp_anal_raw")
                             else:
                                 print("You have already selected this option!")
-                        case 177: 
+                        case 175: 
                             if "comp_anal_ht" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                comp_anal_ht = df.data_extraction.retrieve_ht(comparability_output, "comp_anal_ht")
-                                dataframes.append(comp_anal_ht)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["comp_anal_ht"] = df.data_extraction.retrieve_ht(comparability_output, "comp_anal_ht")
                                 used_options.append("comp_anal_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 178: 
+                        case 176: 
                             if "comp_anal_info" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                comp_anal_info = df.data_extraction.retrieve_info(comparability_output, "comp_anal_info")
-                                dataframes.append(comp_anal_info)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["comp_anal_info"] = df.data_extraction.retrieve_info(comparability_output, "comp_anal_info")
                                 used_options.append("comp_anal_info")
                             else:
                                 print("You have already selected this option!")
-                        case 179: 
+                        case 177: 
                             if "comp_var__raw" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                comp_var = df.data_extraction.retrieve_data(comp_vars_rep, "comp_var__raw")
-                                dataframes.append(comp_var)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["comp_var__raw"] = df.data_extraction.retrieve_data(comp_vars_rep, "comp_var__raw")
                                 used_options.append("comp_var__raw")
                             else:
                                 print("You have already selected this option!")
-                        case 180: 
+                        case 178: 
                             if "comp_var__ht" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                comp_var_ht = df.data_extraction.retrieve_ht(comp_vars_rep, "comp_var__ht")
-                                dataframes.append(comp_var_ht)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["comp_var__ht"] = df.data_extraction.retrieve_ht(comp_vars_rep, "comp_var__ht")
                                 used_options.append("comp_var__ht")
                             else:
                                 print("You have already selected this option!")
-                        case 181: 
+                        case 179: 
                             if "comp_var__info" not in used_options:
-                                row_styles4[num - 133] = highlight_style
-                                comp_var_info = df.data_extraction.retrieve_info(comp_vars_rep, "comp_var__info")
-                                dataframes.append(comp_var_info)
+                                row_styles4[num - 131] = highlight_style
+                                all_df["comp_var__info"] = df.data_extraction.retrieve_info(comp_vars_rep, "comp_var__info")
                                 used_options.append("comp_var__info")
                             else:
                                 print("You have already selected this option!")
-                        case 182: 
+                        case 180: 
                             if "comp_var_rep_raw" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                comp_var_rep = df.data_extraction.retrieve_data(which_comp_vars_rep_output, "comp_var_rep_raw")
-                                dataframes.append(comp_var_rep)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["comp_var_rep_raw"] = df.data_extraction.retrieve_data(which_comp_vars_rep_output, "comp_var_rep_raw")
                                 used_options.append("comp_var_rep_raw")
                             else:
                                 print("You have already selected this option!")
-                        case 183: 
+                        case 181: 
                             if "comp_var_rep_ht" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                comp_var_rep_ht = df.data_extraction.retrieve_ht(which_comp_vars_rep_output, "comp_var_rep_ht")
-                                dataframes.append(comp_var_rep_ht)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["comp_var_rep_ht"] = df.data_extraction.retrieve_ht(which_comp_vars_rep_output, "comp_var_rep_ht")
                                 used_options.append("comp_var_rep_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 184: 
+                        case 182: 
                             if "comp_var_rep_info" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                comp_var_rep_info = df.data_extraction.retrieve_info(which_comp_vars_rep_output, "comp_var_rep_info")
-                                dataframes.append(comp_var_rep_info)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["comp_var_rep_info"] = df.data_extraction.retrieve_info(which_comp_vars_rep_output, "comp_var_rep_info")
                                 used_options.append("comp_var_rep_info")
                             else:
                                 print("You have already selected this option!")
                         # CLUSTERING
-                        case 185: 
+                        case 183: 
                             if "clust_anal_raw" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                clustering = df.data_extraction.retrieve_data(clustering_output, "clust_anal_raw")
-                                dataframes.append(clustering)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["clust_anal_raw"] = df.data_extraction.retrieve_data(clustering_output, "clust_anal_raw")
                                 used_options.append("clust_anal_raw")
                             else:
                                 print("You have already selected this option!")
-                        case 186: 
+                        case 184: 
                             if "clust_anal_ht" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                clustering_ht = df.data_extraction.retrieve_ht(clustering_output, "clust_anal_ht")
-                                dataframes.append(clustering_ht)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["clust_anal_ht"] = df.data_extraction.retrieve_ht(clustering_output, "clust_anal_ht")
                                 used_options.append("clust_anal_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 187: 
+                        case 185: 
                             if "clust_anal_info" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                clustering_info = df.data_extraction.retrieve_info(clustering_output, "clust_anal_info")
-                                dataframes.append(clustering_info)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["clust_anal_info"] = df.data_extraction.retrieve_info(clustering_output, "clust_anal_info")
                                 used_options.append("clust_anal_info")
                             else:
                                 print("You have already selected this option!")
                         # STUDENT GENDER
-                        case 188: 
+                        case 186: 
                             if "part_gen_raw" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                gender = df.data_extraction.retrieve_data(student_gender, "part_gen_raw")
-                                dataframes.append(gender)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["part_gen_raw"] = df.data_extraction.retrieve_data(student_gender, "part_gen_raw")
                                 used_options.append("part_gen_raw")
                             else:
                                 print("You have already selected this option!")
-                        case 189: 
+                        case 187: 
                             if "part_gen_ht" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                gender_ht = df.data_extraction.retrieve_ht(student_gender, "part_gen_ht")
-                                dataframes.append(gender_ht)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["part_gen_ht"] = df.data_extraction.retrieve_ht(student_gender, "part_gen_ht")
                                 used_options.append("part_gen_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 190: 
+                        case 188: 
                             if "part_gen_info" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                gender_info = df.data_extraction.retrieve_info(student_gender, "part_gen_info")
-                                dataframes.append(gender_info)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["part_gen_info"] = df.data_extraction.retrieve_info(student_gender, "part_gen_info")
                                 used_options.append("part_gen_info")
                             else:
                                 print("You have already selected this option!")
                         # SAMPLE SIZE
-                        case 191: 
+                        case 189: 
                             if "sample_analysed_ht" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                sample_size_ht = df.data_extraction.retrieve_ht(sample_size_output, "sample_analysed_ht")
-                                dataframes.append(sample_size_ht)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["sample_analysed_ht"] = df.data_extraction.retrieve_ht(sample_size_output, "sample_analysed_ht")
                                 used_options.append("sample_analysed_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 192: 
+                        case 190: 
                             if "sample_analysed_info" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                sample_size_info = df.data_extraction.retrieve_info(sample_size_output, "sample_analysed_info")
-                                dataframes.append(sample_size_info)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["sample_analysed_info"] = df.data_extraction.retrieve_info(sample_size_output, "sample_analysed_info")
                                 used_options.append("sample_analysed_info")
                             else:
                                 print("You have already selected this option!")
                         # INTERVENTION SAMPLE SIZE
-                        case 193: 
+                        case 191: 
                             if "base_n_treat_ht" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                sample_size_int_ht = df.data_extraction.retrieve_ht(sample_size_intervention_output, "base_n_treat_ht")
-                                dataframes.append(sample_size_int_ht)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["base_n_treat_ht"] = df.data_extraction.retrieve_ht(sample_size_intervention_output, "base_n_treat_ht")
                                 used_options.append("base_n_treat_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 194: 
+                        case 192: 
                             if "base_n_treat_info" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                sample_size_int_info = df.data_extraction.retrieve_info(sample_size_intervention_output, "base_n_treat_info")
-                                dataframes.append(sample_size_int_info)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["base_n_treat_info"] = df.data_extraction.retrieve_info(sample_size_intervention_output, "base_n_treat_info")
                                 used_options.append("base_n_treat_info")
                             else:
                                 print("You have already selected this option!")
                         # CONTROL SAMPLE SIZE
-                        case 195: 
+                        case 193: 
                             if "base_n_cont_ht" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                sample_size_cont_ht = df.data_extraction.retrieve_ht(sample_size_control_output, "base_n_cont_ht")
-                                dataframes.append(sample_size_cont_ht)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["base_n_cont_ht"] = df.data_extraction.retrieve_ht(sample_size_control_output, "base_n_cont_ht")
                                 used_options.append("base_n_cont_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 196: 
+                        case 194: 
                             if "base_n_cont_info" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                sample_size_cont_info = df.data_extraction.retrieve_info(sample_size_control_output, "base_n_cont_info")
-                                dataframes.append(sample_size_cont_info)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["base_n_cont_info"] = df.data_extraction.retrieve_info(sample_size_control_output, "base_n_cont_info")
                                 used_options.append("base_n_cont_info")
                             else:
                                 print("You have already selected this option!")
                         # INTERVENTION 2 SAMPLE SIZE
-                        case 197: 
+                        case 195: 
                             if "base_n_treat2_ht" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                sample_size_int2_ht = df.data_extraction.retrieve_ht(sample_size_second_intervention_output, "base_n_treat2_ht")
-                                dataframes.append(sample_size_int2_ht)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["base_n_treat2_ht"] = df.data_extraction.retrieve_ht(sample_size_second_intervention_output, "base_n_treat2_ht")
                                 used_options.append("base_n_treat2_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 198: 
+                        case 196: 
                             if "base_n_treat2_info" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                sample_size_int2_info = df.data_extraction.retrieve_info(sample_size_second_intervention_output, "base_n_treat2_info")
-                                dataframes.append(sample_size_int2_info)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["base_n_treat2_info"] = df.data_extraction.retrieve_info(sample_size_second_intervention_output, "base_n_treat2_info")
                                 used_options.append("base_n_treat2_info")
                             else:
                                 print("You have already selected this option!")
                         # INTERVENTION 3 SAMPLE SIZE
-                        case 199: 
+                        case 197: 
                             if "base_n_treat3_ht" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                sample_size_int3_ht = df.data_extraction.retrieve_ht(sample_size_third_intervention_output, "base_n_treat3_ht")
-                                dataframes.append(sample_size_int3_ht)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["base_n_treat3_ht"] = df.data_extraction.retrieve_ht(sample_size_third_intervention_output, "base_n_treat3_ht")
                                 used_options.append("base_n_treat3_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 200: 
+                        case 198: 
                             if "base_n_treat3_info" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                sample_size_int3_info = df.data_extraction.retrieve_info(sample_size_third_intervention_output, "base_n_treat3_info")
-                                dataframes.append(sample_size_int3_info)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["base_n_treat3_info"] = df.data_extraction.retrieve_info(sample_size_third_intervention_output, "base_n_treat3_info")
                                 used_options.append("base_n_treat3_info")
                             else:
                                 print("You have already selected this option!") 
                         # INTERVENTION SAMPLE SIZE ANALYSED
-                        case 201: 
+                        case 199: 
                             if "n_treat_ht" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                sameple_size_int_anal_ht = df.data_extraction.retrieve_ht(samp_size_anal_int_output, "n_treat_ht")
-                                dataframes.append(sameple_size_int_anal_ht)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["n_treat_ht"] = df.data_extraction.retrieve_ht(samp_size_anal_int_output, "n_treat_ht")
                                 used_options.append("n_treat_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 202: 
+                        case 200: 
                             if "n_treat_info" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                sameple_size_int_anal_info = df.data_extraction.retrieve_info(samp_size_anal_int_output, "n_treat_info")
-                                dataframes.append(sameple_size_int_anal_info)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["n_treat_info"] = df.data_extraction.retrieve_info(samp_size_anal_int_output, "n_treat_info")
                                 used_options.append("n_treat_info")
                             else:
                                 print("You have already selected this option!") 
                         # CONTROL SAMPLE SIZE ANALYSED
-                        case 203: 
+                        case 201: 
                             if "n_cont_ht" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                sameple_size_cont_anal_ht = df.data_extraction.retrieve_ht(samp_size_anal_cont_output, "n_cont_ht")
-                                dataframes.append(sameple_size_cont_anal_ht)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["n_cont_ht"] = df.data_extraction.retrieve_ht(samp_size_anal_cont_output, "n_cont_ht")
                                 used_options.append("n_cont_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 204: 
+                        case 202: 
                             if "n_cont_info" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                sameple_size_cont_anal_info = df.data_extraction.retrieve_info(samp_size_anal_cont_output, "n_cont_info")
-                                dataframes.append(sameple_size_cont_anal_info)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["n_cont_info"] = df.data_extraction.retrieve_info(samp_size_anal_cont_output, "n_cont_info")
                                 used_options.append("n_cont_info")
                             else:
                                 print("You have already selected this option!") 
                         # INTERVENTION 2 SAMPLE SIZE ANALYSED
-                        case 205: 
+                        case 203: 
                             if "n_treat2_ht" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                sameple_size_int2_anal_ht = df.data_extraction.retrieve_ht(samp_size_anal_sec_int_output, "n_treat2_ht")
-                                dataframes.append(sameple_size_int2_anal_ht)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["n_treat2_ht"] = df.data_extraction.retrieve_ht(samp_size_anal_sec_int_output, "n_treat2_ht")
                                 used_options.append("n_treat2_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 206: 
+                        case 204: 
                             if "n_treat2_info" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                sameple_size_int2_anal_info = df.data_extraction.retrieve_info(samp_size_anal_sec_int_output, "n_treat2_info")
-                                dataframes.append(sameple_size_int2_anal_info)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["n_treat2_info"] = df.data_extraction.retrieve_info(samp_size_anal_sec_int_output, "n_treat2_info")
                                 used_options.append("n_treat2_info")
                             else:
                                 print("You have already selected this option!") 
                         # CONTROL 2 SAMPLE SIZE ANALYSED
-                        case 207: 
+                        case 205: 
                             if "n_cont2_ht" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                sameple_size_contr2_anal_ht = df.data_extraction.retrieve_ht(samp_size_anal_sec_cont_output, "n_cont2_ht")
-                                dataframes.append(sameple_size_contr2_anal_ht)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["n_cont2_ht"] = df.data_extraction.retrieve_ht(samp_size_anal_sec_cont_output, "n_cont2_ht")
                                 used_options.append("n_cont2_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 208: 
+                        case 206: 
                             if "n_cont2_info" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                sameple_size_contr2_anal_info = df.data_extraction.retrieve_info(samp_size_anal_sec_cont_output, "n_cont2_info")
-                                dataframes.append(sameple_size_contr2_anal_info)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["n_cont2_info"] = df.data_extraction.retrieve_info(samp_size_anal_sec_cont_output, "n_cont2_info")
                                 used_options.append("n_cont2_info")
                             else:
                                 print("You have already selected this option!") 
                         # ATTRITION REPORTED
-                        case 209: 
+                        case 207: 
                             if "attri_raw" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                attrition = df.data_extraction.retrieve_data(attr_dropout_rep_output, "attri_raw")
-                                dataframes.append(attrition)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["attri_raw"] = df.data_extraction.retrieve_data(attr_dropout_rep_output, "attri_raw")
                                 used_options.append("attri_raw")
                             else:
                                 print("You have already selected this option!")
-                        case 210: 
+                        case 208: 
                             if "attri_ht" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                attrition_ht = df.data_extraction.retrieve_ht(attr_dropout_rep_output, "attri_ht")
-                                dataframes.append(attrition_ht)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["attri_ht"] = df.data_extraction.retrieve_ht(attr_dropout_rep_output, "attri_ht")
                                 used_options.append("attri_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 211: 
+                        case 209: 
                             if "attri_info" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                attrition_info = df.data_extraction.retrieve_info(attr_dropout_rep_output, "attri_info")
-                                dataframes.append(attrition_info)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["attri_info"] = df.data_extraction.retrieve_info(attr_dropout_rep_output, "attri_info")
                                 used_options.append("attri_info")
                             else:
                                 print("You have already selected this option!")
                         # ATTRITION TREATMENT GROUP
-                        case 212: 
+                        case 210: 
                             if "attri_treat_ht" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                attrition_treat_ht = df.data_extraction.retrieve_ht(treat_grp_attr, "attri_treat_ht")
-                                dataframes.append(attrition_treat_ht)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["attri_treat_ht"] = df.data_extraction.retrieve_ht(treat_grp_attr, "attri_treat_ht")
                                 used_options.append("attri_treat_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 213: 
+                        case 211: 
                             if "attri_treat_info" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                attrition_treat_info = df.data_extraction.retrieve_info(treat_grp_attr, "attri_treat_info")
-                                dataframes.append(attrition_treat_info)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["attri_treat_info"] = df.data_extraction.retrieve_info(treat_grp_attr, "attri_treat_info")
                                 used_options.append("attri_treat_info")
                             else:
                                 print("You have already selected this option!") 
                         # TOTAL % ATTRITION
-                        case 214: 
+                        case 212: 
                             if "attri_perc_ht" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                total_perc_attr_ht = df.data_extraction.retrieve_ht(overall_perc_attr, "attri_perc_ht")
-                                dataframes.append(total_perc_attr_ht)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["attri_perc_ht"] = df.data_extraction.retrieve_ht(overall_perc_attr, "attri_perc_ht")
                                 used_options.append("attri_perc_ht")
                             else:
                                 print("You have already selected this option!")
-                        case 215: 
+                        case 213: 
                             if "attri_perc_info" not in used_options:
-                                row_styles5[num - 182] = highlight_style
-                                total_perc_attr_info = df.data_extraction.retrieve_info(overall_perc_attr, "attri_perc_info")
-                                dataframes.append(total_perc_attr_info)
+                                row_styles5[num - 180] = highlight_style
+                                all_df["attri_perc_info"] = df.data_extraction.retrieve_info(overall_perc_attr, "attri_perc_info")
                                 used_options.append("attri_perc_info")
                             else:
                                 print("You have already selected this option!") 
-                        case _:
-                            print("Error: invalid option selected")
-                    
+                        case 214:
+                            console.print("Compiling..")
+
+                            row_styles5[num - 180] = highlight_style
+                                
+                            all_df["id"] = df.data_extraction.retrieve_metadata("ItemId", "id")
+                            all_df["pub_author"] = df.data_extraction.retrieve_metadata("ShortTitle", "pub_author")
+                            all_df["pub_year"] = df.data_extraction.retrieve_metadata("Year", "pub_year")
+                            all_df["abstract"] = df.data_extraction.retrieve_metadata("Abstract", "abstract")
+                            all_df["strand_raw"] = df.data_extraction.retrieve_data(admin_strand_output, "strand_raw")
+                            all_df["loc_country_raw"] = df.data_extraction.retrieve_data(countries, "loc_country_raw")
+                            all_df["pub_eppi"] = df.data_extraction.retrieve_metadata("TypeName", "pub_eppi")
+                            all_df["pub_type_raw"] = df.data_extraction.retrieve_data(publication_type_output, "pub_type_raw")
+                            all_df["part_age_raw"] = df.data_extraction.retrieve_data(student_age_output, "part_age_raw")
+                            all_df["eco_valid_raw"] = df.data_extraction.retrieve_data(study_realism_output, "eco_valid_raw")
+                            
+                            #/*************************/#
+                            #/     NUMBER OF SCHOOLS   /#
+                            #/*************************/#
+        
+                            all_df["school_treat_info"] = df.data_extraction.retrieve_info(number_of_schools_intervention_output, "school_treat_info")
+                            all_df["school_treat_ht"] = df.data_extraction.retrieve_ht(number_of_schools_intervention_output, "school_treat_ht")
+                            all_df["school_cont_info"] = df.data_extraction.retrieve_info(number_of_schools_control_output, "school_cont_info")
+                            all_df["school_cont_ht"] = df.data_extraction.retrieve_ht(number_of_schools_control_output, "school_cont_ht")
+                            all_df["school_total_info"] = df.data_extraction.retrieve_info(number_of_schools_total_output, "school_total_info")
+                            all_df["school_total_ht"] = df.data_extraction.retrieve_ht(number_of_schools_total_output, "school_total_ht")
+                            
+                            
+                            #/*************************/#
+                            #/    NUMBER OF CLASSES    /#
+                            #/*************************/#
+                            
+                            all_df["class_treat_info"] = df.data_extraction.retrieve_info(num_of_class_int_output, "class_treat_info")
+                            all_df["class_treat_ht"] = df.data_extraction.retrieve_ht(num_of_class_int_output, "class_treat_ht")
+                            all_df["class_cont_info"] = df.data_extraction.retrieve_info(num_of_class_cont_output, "class_cont_info")
+                            all_df["class_cont_ht"] = df.data_extraction.retrieve_ht(num_of_class_cont_output, "class_cont_ht")
+                            all_df["class_total_info"] = df.data_extraction.retrieve_info(num_of_class_tot_output, "class_total_info")
+                            all_df["class_total_ht"] = df.data_extraction.retrieve_ht(num_of_class_tot_output, "class_total_ht")
+                            
+                            #/****************************/#
+                            #/   PARTICIPANT ASSIGNMENT   /#
+                            #/****************************/#
+                            
+                            all_df["part_assig_raw"] = df.data_extraction.retrieve_data(part_assign_output, "part_assig_raw")
+                            all_df["part_assig_ht"] = df.data_extraction.retrieve_ht(part_assign_output, "part_assig_ht")
+                            all_df["part_assig_info"] = df.data_extraction.retrieve_info(part_assign_output, "part_assig_info")
+                        
+                            #/*************************/#
+                            #/   LEVEL OF ASSIGNMENT   /#
+                            #/*************************/#
+                            
+                            all_df["level_assig_raw"] = df.data_extraction.retrieve_data(level_of_assignment_output, "level_assig_raw")
+                            all_df["level_assig_ht"] = df.data_extraction.retrieve_ht(level_of_assignment_output, "level_assig_ht")
+                            all_df["level_assig_info"] = df.data_extraction.retrieve_info(level_of_assignment_output, "level_assig_info")
+                            
+                            #/**********************/#
+                            #/     STUDY DESIGN     /#
+                            #/**********************/#
+                            
+                            all_df["int_design_raw"] = df.data_extraction.retrieve_data(study_design_output, "int_desig_raw")
+                            all_df["int_design_ht"] = df.data_extraction.retrieve_ht(study_design_output, "int_design_ht")
+                            all_df["int_design_info"] = df.data_extraction.retrieve_info(study_design_output, "int_design_info")
+
+                            #/**********************/#
+                            #/     RANDOMISATION    /#
+                            #/**********************/#
                     
-                    if dataframes:
-                        all_df = pd.concat(dataframes, axis=1)
+                            all_df["rand_raw"] = df.data_extraction.retrieve_data(randomisation_details, "rand_raw")
+                            all_df["rand_ht"] = df.data_extraction.retrieve_ht(randomisation_details, "rand_ht")
+                            all_df["rand_info"] = df.data_extraction.retrieve_info(randomisation_details, "rand_info")
+
+                            #/*************************/#
+                            #/ TOOLKIT PRIMARY OUTCOME /#
+                            #/*************************/#
+
+                            df_outcomes = DataFrameCompilation(json_extractor)
+                            df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
+
+                            all_df["out_tit_tool"] = df_out.out_tit_tool
+                            all_df["out_desc_tool"] = df_out.out_desc_tool
+                            all_df["out_type_tool"] = df_out.out_type_tool
+                            all_df["out_smd_tool"] = df_out.smd_tool
+                            all_df["out_se_tool"] = df_out.se_tool
+                            all_df["out_ci_lower_tool"] = df_out.ci_lower_tool
+                            all_df["out_ci_upper_tool"] = df_out.ci_upper_tool
+                            all_df["out_measure_tool"] = df_out.out_measure_tool
+                            all_df["out_g1_n_tool"] = df_out.out_g1_n_tool
+                            all_df["out_g1_mean_tool"] = df_out.out_g1_mean_tool
+                            all_df["out_g1_sd_tool"] = df_out.out_g1_sd_tool
+                            all_df["out_g2_n_tool"] = df_out.out_g2_n_tool
+                            all_df["out_g2_mean_tool"] = df_out.out_g2_mean_tool
+                            all_df["out_g2_sd_tool"] = df_out.out_g2_sd_tool
+                            all_df["out_test_type_raw_tool"] = df_out.out_test_type_raw_tool
+                            all_df["out_es_type_tool"] = df_out.out_es_type_tool
+
+                            #/*************************/#
+                            #/     READING OUTCOME     /#
+                            #/*************************/#
+
+                            all_df["out_tit_red"] = df_out.out_tit_red
+                            all_df["out_desc_red"] = df_out.out_desc_red
+                            all_df["out_type_red"] = df_out.out_type_red
+                            all_df["out_smd_red"] = df_out.smd_red
+                            all_df["out_se_red"] = df_out.se_red
+                            all_df["out_ci_lower_red"] = df_out.ci_lower_red
+                            all_df["out_ci_upper_red"] = df_out.ci_upper_red
+                            all_df["out_measure_red"] = df_out.out_measure_red
+                            all_df["out_g1_n_red"] = df_out.out_g1_n_red
+                            all_df["out_g1_mean_red"] = df_out.out_g1_mean_red
+                            all_df["out_g1_sd_red"] = df_out.out_g1_sd_red
+                            all_df["out_g2_n_red"] = df_out.out_g2_n_red
+                            all_df["out_g2_mean_red"] = df_out.out_g2_mean_red
+                            all_df["out_g2_sd_red"] = df_out.out_g2_sd_red
+                            all_df["out_test_type_raw_red"] = df_out.out_test_type_raw_red
+                            all_df["out_es_type_red"] = df_out.out_es_type_red
+
+                            #/*************************/#
+                            #/     WRITING OUTCOME     /#
+                            #/*************************/#
+
+                            all_df["out_tit_wri"] = df_out.out_tit_wri
+                            all_df["out_desc_wri"] = df_out.out_desc_wri
+                            all_df["out_type_wri"] = df_out.out_type_wri
+                            all_df["out_smd_wri"] = df_out.smd_wri
+                            all_df["out_se_wri"] = df_out.se_wri
+                            all_df["out_ci_lower_wri"] = df_out.ci_lower_wri
+                            all_df["out_ci_upper_wri"] = df_out.ci_upper_wri
+                            all_df["out_measure_wri"] = df_out.out_measure_wri
+                            all_df["out_g1_n_wri"] = df_out.out_g1_n_wri
+                            all_df["out_g1_mean_wri"] = df_out.out_g1_mean_wri
+                            all_df["out_g1_sd_wri"] = df_out.out_g1_sd_wri
+                            all_df["out_g2_n_wri"] = df_out.out_g2_n_wri
+                            all_df["out_g2_mean_wri"] = df_out.out_g2_mean_wri
+                            all_df["out_g2_sd_wri"] = df_out.out_g2_sd_wri
+                            all_df["out_test_type_raw_wri"] = df_out.out_test_type_raw_wri
+                            all_df["out_es_type_wri"] = df_out.out_es_type_wri
+
+                            #/*************************/#
+                            #/        MATH OUTCOME     /#
+                            #/*************************/#
+
+                            all_df["out_tit_math"] = df_out.out_tit_math
+                            all_df["out_desc_math"] = df_out.out_desc_math
+                            all_df["out_type_math"] = df_out.out_type_math
+                            all_df["out_smd_math"] = df_out.smd_math
+                            all_df["out_se_math"] = df_out.se_math
+                            all_df["out_ci_lower_math"] = df_out.ci_lower_math
+                            all_df["out_ci_upper_math"] = df_out.ci_upper_math
+                            all_df["out_measure_math"] = df_out.out_measure_math
+                            all_df["out_g1_n_math"] = df_out.out_g1_n_math
+                            all_df["out_g1_mean_math"] = df_out.out_g1_mean_math
+                            all_df["out_g1_sd_math"] = df_out.out_g1_sd_math
+                            all_df["out_g2_n_math"] = df_out.out_g2_n_math
+                            all_df["out_g2_mean_math"] = df_out.out_g2_mean_math
+                            all_df["out_g2_sd_math"] = df_out.out_g2_sd_math
+                            all_df["out_test_type_raw_math"] = df_out.out_test_type_raw_math
+                            all_df["out_es_type_math"] = df_out.out_es_type_math
+
+                            #/*************************/#
+                            #/     SCIENCE OUTCOME     /#
+                            #/*************************/#
+
+                            all_df["out_tit_sci"] = df_out.out_tit_sci
+                            all_df["out_desc_sci"] = df_out.out_desc_sci
+                            all_df["out_type_sci"] = df_out.out_type_sci
+                            all_df["out_smd_sci"] = df_out.smd_sci
+                            all_df["out_se_sci"] = df_out.se_sci
+                            all_df["out_ci_lower_sci"] = df_out.ci_lower_sci
+                            all_df["out_ci_upper_sci"] = df_out.ci_upper_sci
+                            all_df["out_measure_sci"] = df_out.out_measure_sci
+                            all_df["out_g1_n_sci"] = df_out.out_g1_n_sci
+                            all_df["out_g1_mean_sci"] = df_out.out_g1_mean_sci
+                            all_df["out_g1_sd_sci"] = df_out.out_g1_sd_sci
+                            all_df["out_g2_n_sci"] = df_out.out_g2_n_sci
+                            all_df["out_g2_mean_sci"] = df_out.out_g2_mean_sci
+                            all_df["out_g2_sd_sci"] = df_out.out_g2_sd_sci
+                            all_df["out_test_type_raw_sci"] = df_out.out_test_type_raw_sci
+                            all_df["out_es_type_sci"] = df_out.out_es_type_sci
+
+                            #/*************************/#
+                            #/        FSM OUTCOME      /#
+                            #/*************************/#
+
+                            all_df["out_tit_fsm"] = df_out.out_tit_fsm
+                            all_df["out_desc_fsm"] = df_out.out_desc_fsm
+                            all_df["out_type_fsm"] = df_out.out_type_fsm
+                            all_df["out_smd_fsm"] = df_out.smd_fsm
+                            all_df["out_se_fsm"] = df_out.se_fsm
+                            all_df["out_ci_lower_fsm"] = df_out.ci_lower_fsm
+                            all_df["out_ci_upper_fsm"] = df_out.ci_upper_fsm
+                            all_df["out_measure_fsm"] = df_out.out_measure_fsm
+                            all_df["out_g1_n_fsm"] = df_out.out_g1_n_fsm
+                            all_df["out_g1_mean_fsm"] = df_out.out_g1_mean_fsm
+                            all_df["out_g1_sd_fsm"] = df_out.out_g1_sd_fsm
+                            all_df["out_g2_n_fsm"] = df_out.out_g2_n_fsm
+                            all_df["out_g2_mean_fsm"] = df_out.out_g2_mean_fsm
+                            all_df["out_g2_sd_fsm"] = df_out.out_g2_sd_fsm
+                            all_df["out_test_type_raw_fsm"] = df_out.out_test_type_raw_fsm
+                            all_df["out_es_type_fsm"] = df_out.out_es_type_fsm
+
+                            #/*****************************/#
+                            #/     INTERVENTION DETAILS    /#
+                            #/*****************************/#
+                            
+                            all_df["intervention_name_ht"] = df.data_extraction.retrieve_ht(int_name_output, "intervention_name_ht")
+                            all_df["int_name_info"] = df.data_extraction.retrieve_info(int_name_output, "int_name_info")
+
+                            all_df["intervention_desc_ht"] = df.data_extraction.retrieve_ht(intervention_description_output, "intervention_desc_ht")
+                            all_df["intervention_desc_info"] = df.data_extraction.retrieve_info(intervention_description_output, "intervention_desc_info")
+
+                            all_df["intervention_objec_ht"] = df.data_extraction.retrieve_ht(intervention_objectives_output, "intervention_objec_ht")
+                            all_df["intervention_objec_info"] = df.data_extraction.retrieve_info(intervention_objectives_output, "intervention_objec_info")
+
+                            all_df["int_training_raw"] = df.data_extraction.retrieve_data(int_training_provided_output, "int_training_raw")
+                            all_df["int_training_ht"] = df.data_extraction.retrieve_ht(int_training_provided_output, "int_training_ht")
+                            all_df["int_training_info"] = df.data_extraction.retrieve_info(int_training_provided_output, "int_training_info")
+
+                            all_df["int_approach_raw"] = df.data_extraction.retrieve_data(intervention_teaching_approach, "int_approach_raw")
+                            all_df["int_approach_ht"] = df.data_extraction.retrieve_ht(intervention_teaching_approach, "int_approach_ht")
+                            all_df["int_approach_info"] = df.data_extraction.retrieve_info(intervention_teaching_approach, "int_approach_info")
+
+                            all_df["digit_tech_raw"] = df.data_extraction.retrieve_data(int_appr_dig_tech, "digit_tech_raw")
+                            all_df["digit_tech_ht"] = df.data_extraction.retrieve_ht(int_appr_dig_tech, "digit_tech_ht")
+                            all_df["digit_tech_info"] = df.data_extraction.retrieve_info(int_appr_dig_tech, "digit_tech_info")
+
+                            all_df["parent_partic_raw"] = df.data_extraction.retrieve_data(int_appr_par_or_comm_vol, "parent_partic_raw")
+                            all_df["parent_partic_ht"] = df.data_extraction.retrieve_ht(int_appr_par_or_comm_vol, "parent_partic_ht")
+                            all_df["parent_partic_info"] = df.data_extraction.retrieve_info(int_appr_par_or_comm_vol, "parent_partic_info")
+
+                            all_df["int_when_raw"] = df.data_extraction.retrieve_data(intervention_time_output, "int_when_raw")
+                            all_df["int_when_ht"] = df.data_extraction.retrieve_ht(intervention_time_output, "int_when_ht")
+                            all_df["int_when_info"] = df.data_extraction.retrieve_info(intervention_time_output, "int_when_info")
+
+                            all_df["int_who_raw"] = df.data_extraction.retrieve_data(intervention_delivery_output, "int_who_raw")
+                            all_df["int_who_ht"] = df.data_extraction.retrieve_ht(intervention_delivery_output, "int_who_ht")
+                            all_df["int_who_info"] = df.data_extraction.retrieve_info(intervention_delivery_output, "int_who_info")
+
+                            all_df["int_dur_ht"] = df.data_extraction.retrieve_ht(int_dur_output, "int_dur_ht")
+                            all_df["int_dur_info"] = df.data_extraction.retrieve_info(int_dur_output, "int_dur_info")
+
+                            all_df["int_leng_ht"] = df.data_extraction.retrieve_ht(intervention_session_length_output, "int_leng_ht")
+                            all_df["int_leng_info"] = df.data_extraction.retrieve_info(intervention_session_length_output, "int_leng_info")
+
+                            all_df["int_setting_raw"] = df.data_extraction.retrieve_info(edu_setting_output, "int_setting_raw")
+                            all_df["int_setting_ht"] = df.data_extraction.retrieve_ht(edu_setting_output, "int_setting_ht")
+                            all_df["int_setting_info"] = df.data_extraction.retrieve_info(edu_setting_output, "int_setting_info")
+
+                            all_df["int_part_raw"] = df.data_extraction.retrieve_info(int_focus_output, "int_part_raw")
+                            all_df["int_part_ht"] = df.data_extraction.retrieve_info(int_focus_output, "int_part_ht")
+                            all_df["int_part_info"] = df.data_extraction.retrieve_info(int_focus_output, "int_part_info")
+
+                            all_df["int_fidel_raw"] = df.data_extraction.retrieve_data(int_impl_details, "int_fidel_raw")
+                            all_df["int_fidel_ht"] = df.data_extraction.retrieve_ht(int_impl_details, "int_fidel_ht")
+                            all_df["int_fidel_info"] = df.data_extraction.retrieve_info(int_impl_details, "int_fidel_info")
+
+                            all_df["int_cost_raw"] = df.data_extraction.retrieve_data(int_costs_reported, "int_cost_raw")
+                            all_df["int_cost_ht"] = df.data_extraction.retrieve_ht(int_costs_reported, "int_cost_ht")
+                            all_df["int_cost_info"] = df.data_extraction.retrieve_info(int_costs_reported, "int_cost_info")
+
+                            all_df["base_diff_raw"] = df.data_extraction.retrieve_data(baseline_diff_output, "base_diff_raw")
+                            all_df["base_diff_ht"] = df.data_extraction.retrieve_ht(baseline_diff_output, "base_diff_ht")
+                            all_df["base_diff_info"] = df.data_extraction.retrieve_info(baseline_diff_output, "base_diff_info")
+
+                            all_df["comp_anal_raw"] = df.data_extraction.retrieve_data(comparability_output, "comp_anal_raw")
+                            all_df["comp_anal_ht"] = df.data_extraction.retrieve_ht(comparability_output, "comp_anal_ht")
+                            all_df["comp_anal_info"] = df.data_extraction.retrieve_info(comparability_output, "comp_anal_info")
+
+                            all_df["comp_var__raw"] = df.data_extraction.retrieve_data(comp_vars_rep, "comp_var__raw")
+                            all_df["comp_var__ht"] = df.data_extraction.retrieve_ht(comp_vars_rep, "comp_var__ht")
+                            all_df["comp_var__info"] = df.data_extraction.retrieve_info(comp_vars_rep, "comp_var__info")
+
+                            all_df["comp_var_rep_raw"] = df.data_extraction.retrieve_data(which_comp_vars_rep_output, "comp_var_rep_raw")
+                            all_df["comp_var_rep_ht"] = df.data_extraction.retrieve_ht(which_comp_vars_rep_output, "comp_var_rep_ht")
+                            all_df["comp_var_rep_info"] = df.data_extraction.retrieve_info(which_comp_vars_rep_output, "comp_var_rep_info")
+
+                            # CLUSTERING
+                            
+                            all_df["clust_anal_raw"] = df.data_extraction.retrieve_data(clustering_output, "clust_anal_raw")
+                            all_df["clust_anal_ht"] = df.data_extraction.retrieve_ht(clustering_output, "clust_anal_ht")
+                            all_df["clust_anal_info"] = df.data_extraction.retrieve_info(clustering_output, "clust_anal_info")
+                                                        
+                            # STUDENT GENDER
+                            
+                            all_df["part_gen_raw"] = df.data_extraction.retrieve_data(student_gender, "part_gen_raw")
+                            all_df["part_gen_ht"] = df.data_extraction.retrieve_ht(student_gender, "part_gen_ht")
+                            all_df["part_gen_info"] = df.data_extraction.retrieve_info(student_gender, "part_gen_info")
+                            
+                            # SAMPLE SIZE
+                            
+                            all_df["sample_analysed_ht"] = df.data_extraction.retrieve_ht(sample_size_output, "sample_analysed_ht")
+                            all_df["sample_analysed_info"] = df.data_extraction.retrieve_info(sample_size_output, "sample_analysed_info")
+                                                    
+                            # INTERVENTION SAMPLE SIZE
+                            
+                            all_df["base_n_treat_ht"] = df.data_extraction.retrieve_ht(sample_size_intervention_output, "base_n_treat_ht")
+                            all_df["base_n_treat_info"] = df.data_extraction.retrieve_info(sample_size_intervention_output, "base_n_treat_info")
+                        
+                            # CONTROL SAMPLE SIZE
+                            
+                            all_df["base_n_cont_ht"] = df.data_extraction.retrieve_ht(sample_size_control_output, "base_n_cont_ht")
+                            all_df["base_n_cont_info"] = df.data_extraction.retrieve_info(sample_size_control_output, "base_n_cont_info")
+                        
+                            # INTERVENTION 2 SAMPLE SIZE
+                            
+                            all_df["base_n_treat2_ht"] = df.data_extraction.retrieve_ht(sample_size_second_intervention_output, "base_n_treat2_ht")
+                            all_df["base_n_treat2_info"] = df.data_extraction.retrieve_info(sample_size_second_intervention_output, "base_n_treat2_info")
+                        
+                            # INTERVENTION 3 SAMPLE SIZE
+                            
+                            all_df["base_n_treat3_ht"] = df.data_extraction.retrieve_ht(sample_size_third_intervention_output, "base_n_treat3_ht")
+                            all_df["base_n_treat3_info"] = df.data_extraction.retrieve_info(sample_size_third_intervention_output, "base_n_treat3_info")
+                        
+                            # INTERVENTION SAMPLE SIZE ANALYSED
+                            
+                            all_df["n_treat_ht"] = df.data_extraction.retrieve_ht(samp_size_anal_int_output, "n_treat_ht")
+                            all_df["n_treat_info"] = df.data_extraction.retrieve_info(samp_size_anal_int_output, "n_treat_info")
+                            
+                            # CONTROL SAMPLE SIZE ANALYSED
+                            
+                            all_df["n_cont_ht"] = df.data_extraction.retrieve_ht(samp_size_anal_cont_output, "n_cont_ht")
+                            all_df["n_cont_info"] = df.data_extraction.retrieve_info(samp_size_anal_cont_output, "n_cont_info")
+
+                            # INTERVENTION 2 SAMPLE SIZE ANALYSED
+                            
+                            all_df["n_treat2_ht"] = df.data_extraction.retrieve_ht(samp_size_anal_sec_int_output, "n_treat2_ht")
+                            all_df["n_treat2_info"] = df.data_extraction.retrieve_info(samp_size_anal_sec_int_output, "n_treat2_info")
+                            
+                            # CONTROL 2 SAMPLE SIZE ANALYSED
+                            
+                            all_df["n_cont2_ht"] = df.data_extraction.retrieve_ht(samp_size_anal_sec_cont_output, "n_cont2_ht")
+                            all_df["n_cont2_info"] = df.data_extraction.retrieve_info(samp_size_anal_sec_cont_output, "n_cont2_info")
+                            
+                            # ATTRITION REPORTED
+                            
+                            all_df["attri_raw"] = df.data_extraction.retrieve_data(attr_dropout_rep_output, "attri_raw")
+                            all_df["attri_ht"] = df.data_extraction.retrieve_ht(attr_dropout_rep_output, "attri_ht")
+                            all_df["attri_info"] = df.data_extraction.retrieve_info(attr_dropout_rep_output, "attri_info")
+                        
+                            # ATTRITION TREATMENT GROUP
+                            
+                            all_df["attri_treat_ht"] = df.data_extraction.retrieve_ht(treat_grp_attr, "attri_treat_ht")
+                            all_df["attri_treat_info"] = df.data_extraction.retrieve_info(treat_grp_attr, "attri_treat_info")
+                        
+                            # TOTAL % ATTRITION
+
+                            all_df["attri_perc_ht"] = df.data_extraction.retrieve_ht(overall_perc_attr, "attri_perc_ht")
+                            all_df["attri_perc_info"] = df.data_extraction.retrieve_info(overall_perc_attr, "attri_perc_info")
+
+                    if not all_df.empty:
                         console = Console()
                         main_table2 = custom_general_vars1()
                         main_table3 = custom_outcome_vars_1()
                         main_table4 = custom_outcome_vars_2()
                         main_table5 = intervention_vars_3()
                         main_table6 = intervention_vars_4()
                         console.clear()
@@ -2673,24 +2615,425 @@
                                       style=custom_style_outer, 
                                       border_style="#FFFFFF",
                                       width=250)
                         console.clear()
                         # Print the panel
                         console.print(panel)
 
-                if dataframes:
+                if not all_df.empty:
                     import datetime 
                     current_datetime = datetime.datetime.now()
-                    all_df = pd.concat(dataframes, axis=1)
                     console.print("\n[bold]Custom dataframe saved here..[/bold]\n")
 
                     outfile1 = df.data_extraction.save_dataframe(all_df, f"_{current_datetime.strftime('%Y-%m-%d_%H-%M-%S')}_Custom.csv", custom_info=True)
 
                     outfile1=str(outfile1)
                     outfile1=outfile1
                     console.print(outfile1 + "\n")
                 else: 
                     console.print("No data selected, thanks for using the EEF Teaching and Learning Toolkit Extractor.")
                 
+            case 12:
+
+                print("Compiling..")
+
+                all_df = pd.DataFrame()
+
+                df = CustomFrames(json_extractor)
+
+                all_df["id"] = df.data_extraction.retrieve_metadata("ItemId", "id")
+                all_df["pub_author"] = df.data_extraction.retrieve_metadata("ShortTitle", "pub_author")
+                all_df["pub_year"] = df.data_extraction.retrieve_metadata("Year", "pub_year")
+                all_df["abstract"] = df.data_extraction.retrieve_metadata("Abstract", "abstract")
+                all_df["strand_raw"] = df.data_extraction.retrieve_data(admin_strand_output, "strand_raw")
+                all_df["loc_country_raw"] = df.data_extraction.retrieve_data(countries, "loc_country_raw")
+                all_df["pub_eppi"] = df.data_extraction.retrieve_metadata("TypeName", "pub_eppi")
+                all_df["pub_type_raw"] = df.data_extraction.retrieve_data(publication_type_output, "pub_type_raw")
+                all_df["part_age_raw"] = df.data_extraction.retrieve_data(student_age_output, "part_age_raw")
+                all_df["eco_valid_raw"] = df.data_extraction.retrieve_data(study_realism_output, "eco_valid_raw")
+
+                #/*************************/#
+                #/     NUMBER OF SCHOOLS   /#
+                #/*************************/#
+        
+                all_df["school_treat_info"] = df.data_extraction.retrieve_info(number_of_schools_intervention_output, "school_treat_info")
+                all_df["school_treat_ht"] = df.data_extraction.retrieve_ht(number_of_schools_intervention_output, "school_treat_ht")
+                all_df["school_cont_info"] = df.data_extraction.retrieve_info(number_of_schools_control_output, "school_cont_info")
+                all_df["school_cont_ht"] = df.data_extraction.retrieve_ht(number_of_schools_control_output, "school_cont_ht")
+                all_df["school_total_info"] = df.data_extraction.retrieve_info(number_of_schools_total_output, "school_total_info")
+                all_df["school_total_ht"] = df.data_extraction.retrieve_ht(number_of_schools_total_output, "school_total_ht")
+                
+                
+                #/*************************/#
+                #/    NUMBER OF CLASSES    /#
+                #/*************************/#
+                
+                all_df["class_treat_info"] = df.data_extraction.retrieve_info(num_of_class_int_output, "class_treat_info")
+                all_df["class_treat_ht"] = df.data_extraction.retrieve_ht(num_of_class_int_output, "class_treat_ht")
+                all_df["class_cont_info"] = df.data_extraction.retrieve_info(num_of_class_cont_output, "class_cont_info")
+                all_df["class_cont_ht"] = df.data_extraction.retrieve_ht(num_of_class_cont_output, "class_cont_ht")
+                all_df["class_total_info"] = df.data_extraction.retrieve_info(num_of_class_tot_output, "class_total_info")
+                all_df["class_total_ht"] = df.data_extraction.retrieve_ht(num_of_class_tot_output, "class_total_ht")
+                
+                #/****************************/#
+                #/   PARTICIPANT ASSIGNMENT   /#
+                #/****************************/#
+                
+                all_df["part_assig_raw"] = df.data_extraction.retrieve_data(part_assign_output, "part_assig_raw")
+                all_df["part_assig_ht"] = df.data_extraction.retrieve_ht(part_assign_output, "part_assig_ht")
+                all_df["part_assig_info"] = df.data_extraction.retrieve_info(part_assign_output, "part_assig_info")
+            
+                #/*************************/#
+                #/   LEVEL OF ASSIGNMENT   /#
+                #/*************************/#
+                
+                all_df["level_assig_raw"] = df.data_extraction.retrieve_data(level_of_assignment_output, "level_assig_raw")
+                all_df["level_assig_ht"] = df.data_extraction.retrieve_ht(level_of_assignment_output, "level_assig_ht")
+                all_df["level_assig_info"] = df.data_extraction.retrieve_info(level_of_assignment_output, "level_assig_info")
+                
+                #/**********************/#
+                #/     STUDY DESIGN     /#
+                #/**********************/#
+                
+                all_df["int_design_raw"] = df.data_extraction.retrieve_data(study_design_output, "int_desig_raw")
+                all_df["int_design_ht"] = df.data_extraction.retrieve_ht(study_design_output, "int_design_ht")
+                all_df["int_design_info"] = df.data_extraction.retrieve_info(study_design_output, "int_design_info")
+
+                #/**********************/#
+                #/     RANDOMISATION    /#
+                #/**********************/#
+        
+                all_df["rand_raw"] = df.data_extraction.retrieve_data(randomisation_details, "rand_raw")
+                all_df["rand_ht"] = df.data_extraction.retrieve_ht(randomisation_details, "rand_ht")
+                all_df["rand_info"] = df.data_extraction.retrieve_info(randomisation_details, "rand_info")
+
+                #/*************************/#
+                #/ TOOLKIT PRIMARY OUTCOME /#
+                #/*************************/#
+
+                df_outcomes = DataFrameCompilation(json_extractor)
+                df_out, _ = df_outcomes.make_dataframe_5(save_file=False, clean_cols=False, verbose=False)
+
+                all_df["out_tit_tool"] = df_out.out_tit_tool
+                all_df["out_desc_tool"] = df_out.out_desc_tool
+                all_df["out_type_tool"] = df_out.out_type_tool
+                all_df["out_smd_tool"] = df_out.smd_tool
+                all_df["out_se_tool"] = df_out.se_tool
+                all_df["out_ci_lower_tool"] = df_out.ci_lower_tool
+                all_df["out_ci_upper_tool"] = df_out.ci_upper_tool
+                all_df["out_measure_tool"] = df_out.out_measure_tool
+                all_df["out_g1_n_tool"] = df_out.out_g1_n_tool
+                all_df["out_g1_mean_tool"] = df_out.out_g1_mean_tool
+                all_df["out_g1_sd_tool"] = df_out.out_g1_sd_tool
+                all_df["out_g2_n_tool"] = df_out.out_g2_n_tool
+                all_df["out_g2_mean_tool"] = df_out.out_g2_mean_tool
+                all_df["out_g2_sd_tool"] = df_out.out_g2_sd_tool
+                all_df["out_test_type_raw_tool"] = df_out.out_test_type_raw_tool
+                all_df["out_es_type_tool"] = df_out.out_es_type_tool
+
+                #/*************************/#
+                #/     READING OUTCOME     /#
+                #/*************************/#
+
+                all_df["out_tit_red"] = df_out.out_tit_red
+                all_df["out_desc_red"] = df_out.out_desc_red
+                all_df["out_type_red"] = df_out.out_type_red
+                all_df["out_smd_red"] = df_out.smd_red
+                all_df["out_se_red"] = df_out.se_red
+                all_df["out_ci_lower_red"] = df_out.ci_lower_red
+                all_df["out_ci_upper_red"] = df_out.ci_upper_red
+                all_df["out_measure_red"] = df_out.out_measure_red
+                all_df["out_g1_n_red"] = df_out.out_g1_n_red
+                all_df["out_g1_mean_red"] = df_out.out_g1_mean_red
+                all_df["out_g1_sd_red"] = df_out.out_g1_sd_red
+                all_df["out_g2_n_red"] = df_out.out_g2_n_red
+                all_df["out_g2_mean_red"] = df_out.out_g2_mean_red
+                all_df["out_g2_sd_red"] = df_out.out_g2_sd_red
+                all_df["out_test_type_raw_red"] = df_out.out_test_type_raw_red
+                all_df["out_es_type_red"] = df_out.out_es_type_red
+
+                #/*************************/#
+                #/     WRITING OUTCOME     /#
+                #/*************************/#
+
+                all_df["out_tit_wri"] = df_out.out_tit_wri
+                all_df["out_desc_wri"] = df_out.out_desc_wri
+                all_df["out_type_wri"] = df_out.out_type_wri
+                all_df["out_smd_wri"] = df_out.smd_wri
+                all_df["out_se_wri"] = df_out.se_wri
+                all_df["out_ci_lower_wri"] = df_out.ci_lower_wri
+                all_df["out_ci_upper_wri"] = df_out.ci_upper_wri
+                all_df["out_measure_wri"] = df_out.out_measure_wri
+                all_df["out_g1_n_wri"] = df_out.out_g1_n_wri
+                all_df["out_g1_mean_wri"] = df_out.out_g1_mean_wri
+                all_df["out_g1_sd_wri"] = df_out.out_g1_sd_wri
+                all_df["out_g2_n_wri"] = df_out.out_g2_n_wri
+                all_df["out_g2_mean_wri"] = df_out.out_g2_mean_wri
+                all_df["out_g2_sd_wri"] = df_out.out_g2_sd_wri
+                all_df["out_test_type_raw_wri"] = df_out.out_test_type_raw_wri
+                all_df["out_es_type_wri"] = df_out.out_es_type_wri
+
+                #/*************************/#
+                #/        MATH OUTCOME     /#
+                #/*************************/#
+
+                all_df["out_tit_math"] = df_out.out_tit_math
+                all_df["out_desc_math"] = df_out.out_desc_math
+                all_df["out_type_math"] = df_out.out_type_math
+                all_df["out_smd_math"] = df_out.smd_math
+                all_df["out_se_math"] = df_out.se_math
+                all_df["out_ci_lower_math"] = df_out.ci_lower_math
+                all_df["out_ci_upper_math"] = df_out.ci_upper_math
+                all_df["out_measure_math"] = df_out.out_measure_math
+                all_df["out_g1_n_math"] = df_out.out_g1_n_math
+                all_df["out_g1_mean_math"] = df_out.out_g1_mean_math
+                all_df["out_g1_sd_math"] = df_out.out_g1_sd_math
+                all_df["out_g2_n_math"] = df_out.out_g2_n_math
+                all_df["out_g2_mean_math"] = df_out.out_g2_mean_math
+                all_df["out_g2_sd_math"] = df_out.out_g2_sd_math
+                all_df["out_test_type_raw_math"] = df_out.out_test_type_raw_math
+                all_df["out_es_type_math"] = df_out.out_es_type_math
+
+                #/*************************/#
+                #/     SCIENCE OUTCOME     /#
+                #/*************************/#
+
+                all_df["out_tit_sci"] = df_out.out_tit_sci
+                all_df["out_desc_sci"] = df_out.out_desc_sci
+                all_df["out_type_sci"] = df_out.out_type_sci
+                all_df["out_smd_sci"] = df_out.smd_sci
+                all_df["out_se_sci"] = df_out.se_sci
+                all_df["out_ci_lower_sci"] = df_out.ci_lower_sci
+                all_df["out_ci_upper_sci"] = df_out.ci_upper_sci
+                all_df["out_measure_sci"] = df_out.out_measure_sci
+                all_df["out_g1_n_sci"] = df_out.out_g1_n_sci
+                all_df["out_g1_mean_sci"] = df_out.out_g1_mean_sci
+                all_df["out_g1_sd_sci"] = df_out.out_g1_sd_sci
+                all_df["out_g2_n_sci"] = df_out.out_g2_n_sci
+                all_df["out_g2_mean_sci"] = df_out.out_g2_mean_sci
+                all_df["out_g2_sd_sci"] = df_out.out_g2_sd_sci
+                all_df["out_test_type_raw_sci"] = df_out.out_test_type_raw_sci
+                all_df["out_es_type_sci"] = df_out.out_es_type_sci
+
+                #/*************************/#
+                #/        FSM OUTCOME      /#
+                #/*************************/#
+
+                all_df["out_tit_fsm"] = df_out.out_tit_fsm
+                all_df["out_desc_fsm"] = df_out.out_desc_fsm
+                all_df["out_type_fsm"] = df_out.out_type_fsm
+                all_df["out_smd_fsm"] = df_out.smd_fsm
+                all_df["out_se_fsm"] = df_out.se_fsm
+                all_df["out_ci_lower_fsm"] = df_out.ci_lower_fsm
+                all_df["out_ci_upper_fsm"] = df_out.ci_upper_fsm
+                all_df["out_measure_fsm"] = df_out.out_measure_fsm
+                all_df["out_g1_n_fsm"] = df_out.out_g1_n_fsm
+                all_df["out_g1_mean_fsm"] = df_out.out_g1_mean_fsm
+                all_df["out_g1_sd_fsm"] = df_out.out_g1_sd_fsm
+                all_df["out_g2_n_fsm"] = df_out.out_g2_n_fsm
+                all_df["out_g2_mean_fsm"] = df_out.out_g2_mean_fsm
+                all_df["out_g2_sd_fsm"] = df_out.out_g2_sd_fsm
+                all_df["out_test_type_raw_fsm"] = df_out.out_test_type_raw_fsm
+                all_df["out_es_type_fsm"] = df_out.out_es_type_fsm
+
+                #/*****************************/#
+                #/     INTERVENTION DETAILS    /#
+                #/*****************************/#
+                
+                all_df["intervention_name_ht"] = df.data_extraction.retrieve_ht(int_name_output, "intervention_name_ht")
+                all_df["int_name_info"] = df.data_extraction.retrieve_info(int_name_output, "int_name_info")
+
+                all_df["intervention_desc_ht"] = df.data_extraction.retrieve_ht(intervention_description_output, "intervention_desc_ht")
+                all_df["intervention_desc_info"] = df.data_extraction.retrieve_info(intervention_description_output, "intervention_desc_info")
+
+                all_df["intervention_objec_ht"] = df.data_extraction.retrieve_ht(intervention_objectives_output, "intervention_objec_ht")
+                all_df["intervention_objec_info"] = df.data_extraction.retrieve_info(intervention_objectives_output, "intervention_objec_info")
+
+                all_df["int_training_raw"] = df.data_extraction.retrieve_data(int_training_provided_output, "int_training_raw")
+                all_df["int_training_ht"] = df.data_extraction.retrieve_ht(int_training_provided_output, "int_training_ht")
+                all_df["int_training_info"] = df.data_extraction.retrieve_info(int_training_provided_output, "int_training_info")
+
+                all_df["int_approach_raw"] = df.data_extraction.retrieve_data(intervention_teaching_approach, "int_approach_raw")
+                all_df["int_approach_ht"] = df.data_extraction.retrieve_ht(intervention_teaching_approach, "int_approach_ht")
+                all_df["int_approach_info"] = df.data_extraction.retrieve_info(intervention_teaching_approach, "int_approach_info")
+
+                all_df["digit_tech_raw"] = df.data_extraction.retrieve_data(int_appr_dig_tech, "digit_tech_raw")
+                all_df["digit_tech_ht"] = df.data_extraction.retrieve_ht(int_appr_dig_tech, "digit_tech_ht")
+                all_df["digit_tech_info"] = df.data_extraction.retrieve_info(int_appr_dig_tech, "digit_tech_info")
+
+                all_df["parent_partic_raw"] = df.data_extraction.retrieve_data(int_appr_par_or_comm_vol, "parent_partic_raw")
+                all_df["parent_partic_ht"] = df.data_extraction.retrieve_ht(int_appr_par_or_comm_vol, "parent_partic_ht")
+                all_df["parent_partic_info"] = df.data_extraction.retrieve_info(int_appr_par_or_comm_vol, "parent_partic_info")
+
+                all_df["int_when_raw"] = df.data_extraction.retrieve_data(intervention_time_output, "int_when_raw")
+                all_df["int_when_ht"] = df.data_extraction.retrieve_ht(intervention_time_output, "int_when_ht")
+                all_df["int_when_info"] = df.data_extraction.retrieve_info(intervention_time_output, "int_when_info")
+
+                all_df["int_who_raw"] = df.data_extraction.retrieve_data(intervention_delivery_output, "int_who_raw")
+                all_df["int_who_ht"] = df.data_extraction.retrieve_ht(intervention_delivery_output, "int_who_ht")
+                all_df["int_who_info"] = df.data_extraction.retrieve_info(intervention_delivery_output, "int_who_info")
+
+                all_df["int_dur_ht"] = df.data_extraction.retrieve_ht(int_dur_output, "int_dur_ht")
+                all_df["int_dur_info"] = df.data_extraction.retrieve_info(int_dur_output, "int_dur_info")
+
+                all_df["int_leng_ht"] = df.data_extraction.retrieve_ht(intervention_session_length_output, "int_leng_ht")
+                all_df["int_leng_info"] = df.data_extraction.retrieve_info(intervention_session_length_output, "int_leng_info")
+
+                all_df["int_setting_raw"] = df.data_extraction.retrieve_info(edu_setting_output, "int_setting_raw")
+                all_df["int_setting_ht"] = df.data_extraction.retrieve_ht(edu_setting_output, "int_setting_ht")
+                all_df["int_setting_info"] = df.data_extraction.retrieve_info(edu_setting_output, "int_setting_info")
+
+                all_df["int_part_raw"] = df.data_extraction.retrieve_info(int_focus_output, "int_part_raw")
+                all_df["int_part_ht"] = df.data_extraction.retrieve_info(int_focus_output, "int_part_ht")
+                all_df["int_part_info"] = df.data_extraction.retrieve_info(int_focus_output, "int_part_info")
+
+                all_df["int_fidel_raw"] = df.data_extraction.retrieve_data(int_impl_details, "int_fidel_raw")
+                all_df["int_fidel_ht"] = df.data_extraction.retrieve_ht(int_impl_details, "int_fidel_ht")
+                all_df["int_fidel_info"] = df.data_extraction.retrieve_info(int_impl_details, "int_fidel_info")
+
+                all_df["int_cost_raw"] = df.data_extraction.retrieve_data(int_costs_reported, "int_cost_raw")
+                all_df["int_cost_ht"] = df.data_extraction.retrieve_ht(int_costs_reported, "int_cost_ht")
+                all_df["int_cost_info"] = df.data_extraction.retrieve_info(int_costs_reported, "int_cost_info")
+
+                all_df["base_diff_raw"] = df.data_extraction.retrieve_data(baseline_diff_output, "base_diff_raw")
+                all_df["base_diff_ht"] = df.data_extraction.retrieve_ht(baseline_diff_output, "base_diff_ht")
+                all_df["base_diff_info"] = df.data_extraction.retrieve_info(baseline_diff_output, "base_diff_info")
+
+                all_df["comp_anal_raw"] = df.data_extraction.retrieve_data(comparability_output, "comp_anal_raw")
+                all_df["comp_anal_ht"] = df.data_extraction.retrieve_ht(comparability_output, "comp_anal_ht")
+                all_df["comp_anal_info"] = df.data_extraction.retrieve_info(comparability_output, "comp_anal_info")
+
+                all_df["comp_var__raw"] = df.data_extraction.retrieve_data(comp_vars_rep, "comp_var__raw")
+                all_df["comp_var__ht"] = df.data_extraction.retrieve_ht(comp_vars_rep, "comp_var__ht")
+                all_df["comp_var__info"] = df.data_extraction.retrieve_info(comp_vars_rep, "comp_var__info")
+
+                all_df["comp_var_rep_raw"] = df.data_extraction.retrieve_data(which_comp_vars_rep_output, "comp_var_rep_raw")
+                all_df["comp_var_rep_ht"] = df.data_extraction.retrieve_ht(which_comp_vars_rep_output, "comp_var_rep_ht")
+                all_df["comp_var_rep_info"] = df.data_extraction.retrieve_info(which_comp_vars_rep_output, "comp_var_rep_info")
+
+                # CLUSTERING
+                
+                all_df["clust_anal_raw"] = df.data_extraction.retrieve_data(clustering_output, "clust_anal_raw")
+                all_df["clust_anal_ht"] = df.data_extraction.retrieve_ht(clustering_output, "clust_anal_ht")
+                all_df["clust_anal_info"] = df.data_extraction.retrieve_info(clustering_output, "clust_anal_info")
+                                            
+                # STUDENT GENDER
+                
+                all_df["part_gen_raw"] = df.data_extraction.retrieve_data(student_gender, "part_gen_raw")
+                all_df["part_gen_ht"] = df.data_extraction.retrieve_ht(student_gender, "part_gen_ht")
+                all_df["part_gen_info"] = df.data_extraction.retrieve_info(student_gender, "part_gen_info")
+                
+                # SAMPLE SIZE
+                
+                all_df["sample_analysed_ht"] = df.data_extraction.retrieve_ht(sample_size_output, "sample_analysed_ht")
+                all_df["sample_analysed_info"] = df.data_extraction.retrieve_info(sample_size_output, "sample_analysed_info")
+                                        
+                # INTERVENTION SAMPLE SIZE
+                
+                all_df["base_n_treat_ht"] = df.data_extraction.retrieve_ht(sample_size_intervention_output, "base_n_treat_ht")
+                all_df["base_n_treat_info"] = df.data_extraction.retrieve_info(sample_size_intervention_output, "base_n_treat_info")
+            
+                # CONTROL SAMPLE SIZE
+                
+                all_df["base_n_cont_ht"] = df.data_extraction.retrieve_ht(sample_size_control_output, "base_n_cont_ht")
+                all_df["base_n_cont_info"] = df.data_extraction.retrieve_info(sample_size_control_output, "base_n_cont_info")
+            
+                # INTERVENTION 2 SAMPLE SIZE
+                
+                all_df["base_n_treat2_ht"] = df.data_extraction.retrieve_ht(sample_size_second_intervention_output, "base_n_treat2_ht")
+                all_df["base_n_treat2_info"] = df.data_extraction.retrieve_info(sample_size_second_intervention_output, "base_n_treat2_info")
+            
+                # INTERVENTION 3 SAMPLE SIZE
+                
+                all_df["base_n_treat3_ht"] = df.data_extraction.retrieve_ht(sample_size_third_intervention_output, "base_n_treat3_ht")
+                all_df["base_n_treat3_info"] = df.data_extraction.retrieve_info(sample_size_third_intervention_output, "base_n_treat3_info")
+            
+                # INTERVENTION SAMPLE SIZE ANALYSED
+                
+                all_df["n_treat_ht"] = df.data_extraction.retrieve_ht(samp_size_anal_int_output, "n_treat_ht")
+                all_df["n_treat_info"] = df.data_extraction.retrieve_info(samp_size_anal_int_output, "n_treat_info")
+                
+                # CONTROL SAMPLE SIZE ANALYSED
+                
+                all_df["n_cont_ht"] = df.data_extraction.retrieve_ht(samp_size_anal_cont_output, "n_cont_ht")
+                all_df["n_cont_info"] = df.data_extraction.retrieve_info(samp_size_anal_cont_output, "n_cont_info")
+
+                # INTERVENTION 2 SAMPLE SIZE ANALYSED
+                
+                all_df["n_treat2_ht"] = df.data_extraction.retrieve_ht(samp_size_anal_sec_int_output, "n_treat2_ht")
+                all_df["n_treat2_info"] = df.data_extraction.retrieve_info(samp_size_anal_sec_int_output, "n_treat2_info")
+                
+                # CONTROL 2 SAMPLE SIZE ANALYSED
+                
+                all_df["n_cont2_ht"] = df.data_extraction.retrieve_ht(samp_size_anal_sec_cont_output, "n_cont2_ht")
+                all_df["n_cont2_info"] = df.data_extraction.retrieve_info(samp_size_anal_sec_cont_output, "n_cont2_info")
+                
+                # ATTRITION REPORTED
+                
+                all_df["attri_raw"] = df.data_extraction.retrieve_data(attr_dropout_rep_output, "attri_raw")
+                all_df["attri_ht"] = df.data_extraction.retrieve_ht(attr_dropout_rep_output, "attri_ht")
+                all_df["attri_info"] = df.data_extraction.retrieve_info(attr_dropout_rep_output, "attri_info")
+            
+                # ATTRITION TREATMENT GROUP
+                
+                all_df["attri_treat_ht"] = df.data_extraction.retrieve_ht(treat_grp_attr, "attri_treat_ht")
+                all_df["attri_treat_info"] = df.data_extraction.retrieve_info(treat_grp_attr, "attri_treat_info")
+            
+                # TOTAL % ATTRITION
+
+                all_df["attri_perc_ht"] = df.data_extraction.retrieve_ht(overall_perc_attr, "attri_perc_ht")
+                all_df["attri_perc_info"] = df.data_extraction.retrieve_info(overall_perc_attr, "attri_perc_info")
+                #dataframes.append(df_out_tit_tool)
+
+                #all_df = pd.concat(dataframes, axis=1)
+
+                new_df = pd.DataFrame()
+
+                added_ids = []
+
+                while True:
+                    user_id = input("Enter EPPI ID (or 'q' to finish): ")
+                    
+                    if user_id.lower() == 'q':
+                        break
+
+                    try:
+                        user_id = int(user_id)
+                    except ValueError:
+                        print("The ID you entered is not an integer. Please enter a valid ID.")
+                        continue
+
+                    # Filter the row from DataFrame
+                    filtered_df = all_df.loc[all_df['id'] == user_id]
+
+                    # If there is no such ID in the DataFrame, print an error message
+                    if filtered_df.empty:
+                        print(f"No data found for ID {user_id}")
+                    else:
+                        # Append the filtered row to the new DataFrame
+                        new_df = new_df.append(filtered_df)
+                        # Append the added ID to the list
+                        added_ids.append(user_id)
+                        # Print the list of added IDs
+                        print(f"Added ID: {user_id}: {filtered_df['pub_author'].values[0]}")
 
+                if not new_df.empty:
+                    console = Console()
+                    import datetime 
+                    current_datetime = datetime.datetime.now()
+                    console.print("\n[bold]Custom dataframe saved here..[/bold]\n")
+
+                    outfile1 = df.data_extraction.save_dataframe(new_df, f"_{current_datetime.strftime('%Y-%m-%d_%H-%M-%S')}_Custom.csv", custom_info=True)
+
+                    outfile1=str(outfile1)
+                    outfile1=outfile1
+                    console.print(outfile1 + "\n")
+                else: 
+                    console = Console()
+                    console.print("No data selected, thanks for using the EEF Teaching and Learning Toolkit Extractor.")
+                break
+
+
+
+                
 if __name__ == "__main__":
     main()
```

### Comparing `eef-data-0.52/eefdata/src/attributeIDs.py` & `eef-data-0.53/eefdata/src/attributeIDs.py`

 * *Files identical despite different names*

### Comparing `eef-data-0.52/eefdata/src/funcs.py` & `eef-data-0.53/eefdata/src/funcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -15386,1054 +15386,1075 @@
 0003c190: 222c 2020 2249 6e74 2054 7265 6174 2047  ",  "Int Treat G
 0003c1a0: 7270 2050 7265 2d74 6573 7420 4d65 616e  rp Pre-test Mean
 0003c1b0: 2f53 4422 2c20 2022 5374 616e 6461 7264  /SD",  "Standard
 0003c1c0: 2045 7272 6f72 2229 0a20 2020 206d 6169   Error").    mai
 0003c1d0: 6e5f 7461 626c 6532 2e61 6464 5f72 6f77  n_table2.add_row
 0003c1e0: 2822 4564 7563 6174 696f 6e61 6c20 5365  ("Educational Se
 0003c1f0: 7474 696e 6722 2c20 2249 6e74 204f 7267  tting", "Int Org
-0003c200: 616e 6973 6174 696f 2054 7970 6522 2c20  anisatio Type", 
-0003c210: 2022 496e 7420 5472 6561 7420 5361 6d70   "Int Treat Samp
-0003c220: 6c65 2053 697a 6522 2c20 2022 496e 7420  le Size",  "Int 
-0003c230: 5472 6561 7420 4772 7020 506f 7374 2d74  Treat Grp Post-t
-0003c240: 6573 7420 4d65 616e 2f53 4422 2c20 2022  est Mean/SD",  "
-0003c250: 436f 6e66 6964 656e 6365 2049 6e74 6572  Confidence Inter
-0003c260: 7661 6c20 286c 6229 2229 0a20 2020 206d  val (lb)").    m
-0003c270: 6169 6e5f 7461 626c 6532 2e61 6464 5f72  ain_table2.add_r
-0003c280: 6f77 2822 4563 6f6c 6f67 6963 616c 2056  ow("Ecological V
-0003c290: 616c 6964 6974 7922 2c20 2249 6e74 2054  alidity", "Int T
-0003c2a0: 7261 696e 696e 6722 2c20 2022 496e 7420  raining",  "Int 
-0003c2b0: 436f 6e74 2053 616d 706c 6520 5369 7a65  Cont Sample Size
-0003c2c0: 222c 2020 2249 6e74 2054 7265 6174 2047  ",  "Int Treat G
-0003c2d0: 7270 2047 6169 6e20 5363 6f72 6520 4d65  rp Gain Score Me
-0003c2e0: 616e 2f53 4422 2c20 2022 436f 6e66 6964  an/SD",  "Confid
-0003c2f0: 656e 6365 2049 6e74 6572 7661 6c20 2875  ence Interval (u
-0003c300: 6229 2229 0a20 2020 206d 6169 6e5f 7461  b)").    main_ta
-0003c310: 626c 6532 2e61 6464 5f72 6f77 2822 5374  ble2.add_row("St
-0003c320: 7564 656e 7420 4167 6522 2c20 2022 496e  udent Age",  "In
-0003c330: 7420 466f 6375 7322 2c20 2022 496e 7420  t Focus",  "Int 
-0003c340: 5472 6561 7420 4772 7032 2053 616d 706c  Treat Grp2 Sampl
-0003c350: 6520 5369 7a65 222c 2020 2249 6e74 2054  e Size",  "Int T
-0003c360: 7265 6174 2047 7270 2041 6e79 204f 7468  reat Grp Any Oth
-0003c370: 6572 2049 6e66 6f22 2c20 2022 4f75 7463  er Info",  "Outc
-0003c380: 6f6d 6522 290a 2020 2020 6d61 696e 5f74  ome").    main_t
-0003c390: 6162 6c65 322e 6164 645f 726f 7728 224e  able2.add_row("N
-0003c3a0: 756d 6265 7220 6f66 2053 6368 6f6f 6c73  umber of Schools
-0003c3b0: 222c 2020 2249 6e74 2054 6561 6368 696e  ",  "Int Teachin
-0003c3c0: 6720 4170 7072 6f61 6368 222c 2020 2249  g Approach",  "I
-0003c3d0: 6e74 2054 7265 6174 2047 7270 3320 5361  nt Treat Grp3 Sa
-0003c3e0: 6d70 6c65 2053 697a 6522 2c20 2022 496e  mple Size",  "In
-0003c3f0: 7420 436f 6e74 2047 7270 204e 756d 6265  t Cont Grp Numbe
-0003c400: 7222 2c20 2022 5361 6d70 6c65 2229 0a20  r",  "Sample"). 
-0003c410: 2020 206d 6169 6e5f 7461 626c 6532 2e61     main_table2.a
-0003c420: 6464 5f72 6f77 2822 4e75 6d62 6572 206f  dd_row("Number o
-0003c430: 6620 436c 6173 7365 7322 2c20 2022 496e  f Classes",  "In
-0003c440: 7420 496e 636c 7573 696f 6e22 2c20 2022  t Inclusion",  "
-0003c450: 496e 7420 5472 6561 7420 5361 6d70 6c65  Int Treat Sample
-0003c460: 2053 697a 6520 416e 616c 797a 6564 222c   Size Analyzed",
-0003c470: 2020 2249 6e74 2043 6f6e 7420 4772 7020    "Int Cont Grp 
-0003c480: 5072 652d 7465 7374 204d 6561 6e2f 5344  Pre-test Mean/SD
-0003c490: 222c 2020 224f 7574 636f 6d65 2043 6f6d  ",  "Outcome Com
-0003c4a0: 7061 7269 736f 6e22 290a 2020 2020 6d61  parison").    ma
-0003c4b0: 696e 5f74 6162 6c65 322e 6164 645f 726f  in_table2.add_ro
-0003c4c0: 7728 2254 7265 6174 6d65 6e74 2047 726f  w("Treatment Gro
-0003c4d0: 7570 222c 2020 2249 6e74 2054 696d 6522  up",  "Int Time"
-0003c4e0: 2c20 2022 496e 7420 436f 6e74 2053 616d  ,  "Int Cont Sam
-0003c4f0: 706c 6520 5369 7a65 2041 6e61 6c79 7a65  ple Size Analyze
-0003c500: 6422 2c20 2022 496e 7420 436f 6e74 2047  d",  "Int Cont G
-0003c510: 7270 2050 6f73 742d 7465 7374 204d 6561  rp Post-test Mea
-0003c520: 6e2f 5344 222c 2020 2245 6666 6563 7420  n/SD",  "Effect 
-0003c530: 5369 7a65 2054 7970 6522 290a 2020 2020  Size Type").    
-0003c540: 6d61 696e 5f74 6162 6c65 322e 6164 645f  main_table2.add_
-0003c550: 726f 7728 2250 6172 7469 6369 7061 6e74  row("Participant
-0003c560: 2041 7373 6967 6e6d 656e 7422 2c20 2022   Assignment",  "
-0003c570: 496e 7420 4465 6c69 7665 7279 222c 2020  Int Delivery",  
-0003c580: 2249 6e74 2054 7265 6174 2047 7270 3220  "Int Treat Grp2 
-0003c590: 5361 6d70 6c65 2053 697a 6520 416e 616c  Sample Size Anal
-0003c5a0: 797a 6564 222c 2020 2249 6e74 2043 6f6e  yzed",  "Int Con
-0003c5b0: 7420 4772 7020 4761 696e 2053 636f 7265  t Grp Gain Score
-0003c5c0: 204d 6561 6e2f 5344 222c 2020 224f 7574   Mean/SD",  "Out
-0003c5d0: 636f 6d65 204d 6561 7375 7265 2229 0a20  come Measure"). 
-0003c5e0: 2020 206d 6169 6e5f 7461 626c 6532 2e61     main_table2.a
-0003c5f0: 6464 5f72 6f77 2822 4c65 7665 6c20 6f66  dd_row("Level of
-0003c600: 2041 7373 6967 6e6d 656e 7422 2c20 2249   Assignment", "I
-0003c610: 6e74 2044 7572 6174 696f 6e22 2c20 2022  nt Duration",  "
-0003c620: 496e 7420 436f 6e74 2047 7270 3220 5361  Int Cont Grp2 Sa
-0003c630: 6d70 6c65 2053 697a 6520 416e 616c 797a  mple Size Analyz
-0003c640: 6564 222c 2020 2249 6e74 2043 6f6e 7420  ed",  "Int Cont 
-0003c650: 4772 7020 416e 7920 4f74 6865 7220 496e  Grp Any Other In
-0003c660: 666f 222c 2020 224f 7574 636f 6d65 2054  fo",  "Outcome T
-0003c670: 6974 6c65 2229 0a20 2020 206d 6169 6e5f  itle").    main_
-0003c680: 7461 626c 6532 2e61 6464 5f72 6f77 2822  table2.add_row("
-0003c690: 5374 7564 7920 4465 7369 676e 222c 2022  Study Design", "
-0003c6a0: 496e 7420 4672 6571 7565 6e63 7922 2c20  Int Frequency", 
-0003c6b0: 2022 4174 7472 6974 696f 6e20 5265 706f   "Attrition Repo
-0003c6c0: 7274 6564 222c 2020 2249 6e74 2054 7265  rted",  "Int Tre
-0003c6d0: 6174 2047 7270 3220 4e75 6d62 6572 222c  at Grp2 Number",
-0003c6e0: 2020 2247 726f 7570 3120 4e22 290a 2020    "Group1 N").  
-0003c6f0: 2020 6d61 696e 5f74 6162 6c65 322e 6164    main_table2.ad
-0003c700: 645f 726f 7728 2022 5261 6e64 6f6d 6973  d_row( "Randomis
-0003c710: 6174 696f 6e22 2c20 2022 496e 7420 5365  ation",  "Int Se
-0003c720: 7373 696f 6e20 4c65 6e67 7468 222c 2020  ssion Length",  
-0003c730: 2241 7474 7269 7469 6f6e 2054 7265 6174  "Attrition Treat
-0003c740: 2047 7270 222c 2020 2249 6e74 2054 7265   Grp",  "Int Tre
-0003c750: 6174 2047 7270 3220 5072 652d 7465 7374  at Grp2 Pre-test
-0003c760: 204d 6561 6e2f 5344 222c 2020 2247 726f   Mean/SD",  "Gro
-0003c770: 7570 3220 4e22 290a 2020 2020 6d61 696e  up2 N").    main
-0003c780: 5f74 6162 6c65 322e 6164 645f 726f 7728  _table2.add_row(
-0003c790: 224f 7468 6572 204f 7574 636f 6d65 7322  "Other Outcomes"
-0003c7a0: 2c20 2022 496e 7420 4465 7461 696c 222c  ,  "Int Detail",
-0003c7b0: 2020 2241 7474 7269 7469 6f6e 2054 6f74    "Attrition Tot
-0003c7c0: 616c 2028 2529 222c 2020 2249 6e74 2054  al (%)",  "Int T
-0003c7d0: 7265 6174 2047 7270 3220 506f 7374 2d74  reat Grp2 Post-t
-0003c7e0: 6573 7420 4d65 616e 2f53 4422 2c20 2022  est Mean/SD",  "
-0003c7f0: 4772 6f75 7031 204d 6561 6e22 290a 2020  Group1 Mean").  
-0003c800: 2020 6d61 696e 5f74 6162 6c65 322e 6164    main_table2.ad
-0003c810: 645f 726f 7728 2241 6464 6974 696f 6e61  d_row("Additiona
-0003c820: 6c20 4f75 7463 6f6d 6573 222c 2020 2249  l Outcomes",  "I
-0003c830: 6e74 2043 6f73 7473 222c 2022 222c 2022  nt Costs", "", "
-0003c840: 496e 7420 5472 6561 7420 4772 7032 2047  Int Treat Grp2 G
-0003c850: 6169 6e20 5363 6f72 6520 4d65 616e 2f53  ain Score Mean/S
-0003c860: 4422 2c20 2247 726f 7570 3220 4d65 616e  D", "Group2 Mean
-0003c870: 2229 0a20 2020 206d 6169 6e5f 7461 626c  ").    main_tabl
-0003c880: 6532 2e61 6464 5f72 6f77 2822 4f74 6865  e2.add_row("Othe
-0003c890: 7220 5061 7274 6963 6970 616e 7473 204f  r Participants O
-0003c8a0: 7574 636f 6d65 7322 2c20 2249 6e74 2045  utcomes", "Int E
-0003c8b0: 7661 6c75 6174 696f 6e22 2c20 2022 222c  valuation",  "",
-0003c8c0: 2020 2022 496e 7420 5472 6561 7420 4772     "Int Treat Gr
-0003c8d0: 7032 2041 6e79 204f 7468 6572 2049 6e66  p2 Any Other Inf
-0003c8e0: 6f22 2c20 2247 726f 7570 3120 5344 2229  o", "Group1 SD")
-0003c8f0: 0a20 2020 206d 6169 6e5f 7461 626c 6532  .    main_table2
-0003c900: 2e61 6464 5f72 6f77 2822 222c 2020 2242  .add_row("",  "B
-0003c910: 6173 656c 696e 6520 4469 6666 6572 656e  aseline Differen
-0003c920: 6365 7322 2c20 2222 2c20 2022 496e 7420  ces", "",  "Int 
-0003c930: 436f 6e74 2047 7270 3220 4e75 6d62 6572  Cont Grp2 Number
-0003c940: 222c 2020 2247 726f 7570 3220 5344 2229  ",  "Group2 SD")
-0003c950: 0a20 2020 206d 6169 6e5f 7461 626c 6532  .    main_table2
-0003c960: 2e61 6464 5f72 6f77 2822 222c 2022 436f  .add_row("", "Co
-0003c970: 6d70 7574 6174 696f 6e61 6c20 416e 616c  mputational Anal
-0003c980: 7973 6973 222c 2020 2222 2c20 2249 6e74  ysis",  "", "Int
-0003c990: 2043 6f6e 7420 4772 7032 2050 7265 2d74   Cont Grp2 Pre-t
-0003c9a0: 6573 7420 4d65 616e 2f53 4422 2c20 2022  est Mean/SD",  "
-0003c9b0: 4f75 7463 6f6d 6520 4465 7363 7269 7074  Outcome Descript
-0003c9c0: 696f 6e22 290a 2020 2020 6d61 696e 5f74  ion").    main_t
-0003c9d0: 6162 6c65 322e 6164 645f 726f 7728 2222  able2.add_row(""
-0003c9e0: 2c20 2022 436f 6d70 6172 6162 696c 6974  ,  "Comparabilit
-0003c9f0: 7920 5661 7269 6162 6c65 7320 5265 706f  y Variables Repo
-0003ca00: 7274 6564 222c 2020 2222 2c20 2249 6e74  rted",  "", "Int
-0003ca10: 2043 6f6e 7420 4772 7032 2050 6f73 742d   Cont Grp2 Post-
-0003ca20: 7465 7374 204d 6561 6e2f 5344 222c 2020  test Mean/SD",  
-0003ca30: 2254 6573 7420 5479 7065 204f 7574 636f  "Test Type Outco
-0003ca40: 6d65 2229 0a20 2020 206d 6169 6e5f 7461  me").    main_ta
-0003ca50: 626c 6532 2e61 6464 5f72 6f77 2822 222c  ble2.add_row("",
-0003ca60: 2020 2243 6c75 7374 6572 696e 6722 2c20    "Clustering", 
-0003ca70: 2022 222c 2022 496e 7420 436f 6e74 2047   "", "Int Cont G
-0003ca80: 7270 3220 4761 696e 2053 636f 7265 204d  rp2 Gain Score M
-0003ca90: 6561 6e2f 5344 222c 2022 2229 0a20 2020  ean/SD", "").   
-0003caa0: 206d 6169 6e5f 7461 626c 6532 2e61 6464   main_table2.add
-0003cab0: 5f72 6f77 2822 222c 2020 2222 2c20 2222  _row("",  "", ""
-0003cac0: 2c20 2022 496e 7420 436f 6e74 2047 7270  ,  "Int Cont Grp
-0003cad0: 3220 416e 7920 4f74 6865 7220 496e 666f  2 Any Other Info
-0003cae0: 222c 2022 2229 0a20 2020 206d 6169 6e5f  ", "").    main_
-0003caf0: 7461 626c 6532 2e61 6464 5f72 6f77 2822  table2.add_row("
-0003cb00: 222c 2020 2222 2c20 2222 2c20 2022 466f  ",  "", "",  "Fo
-0003cb10: 6c6c 6f77 2d75 7020 496e 666f 726d 6174  llow-up Informat
-0003cb20: 696f 6e22 2c20 2222 290a 2020 2020 6d61  ion", "").    ma
-0003cb30: 696e 5f74 6162 6c65 322e 666f 6f74 6572  in_table2.footer
-0003cb40: 203d 2022 5468 6973 2069 7320 7468 6520   = "This is the 
-0003cb50: 666f 6f74 6572 2e22 0a20 2020 2072 6574  footer.".    ret
-0003cb60: 7572 6e20 6d61 696e 5f74 6162 6c65 320a  urn main_table2.
-0003cb70: 0a0a 6465 6620 6469 7370 6c61 795f 6d61  ..def display_ma
-0003cb80: 696e 5f6d 656e 7528 293a 0a20 2020 2074  in_menu():.    t
-0003cb90: 6162 6c65 5f74 6974 6c65 5f73 7479 6c65  able_title_style
-0003cba0: 203d 2053 7479 6c65 2869 7461 6c69 633d   = Style(italic=
-0003cbb0: 4661 6c73 652c 2062 6763 6f6c 6f72 3d4e  False, bgcolor=N
-0003cbc0: 6f6e 652c 2063 6f6c 6f72 3d22 2366 6335  one, color="#fc5
-0003cbd0: 3432 3422 2c20 626f 6c64 3d54 7275 6529  424", bold=True)
-0003cbe0: 0a20 2020 2068 6561 6465 725f 7374 796c  .    header_styl
-0003cbf0: 6520 3d20 5374 796c 6528 6974 616c 6963  e = Style(italic
-0003cc00: 3d46 616c 7365 2c20 6267 636f 6c6f 723d  =False, bgcolor=
-0003cc10: 2223 6663 3534 3234 222c 2063 6f6c 6f72  "#fc5424", color
-0003cc20: 3d57 4849 5445 2c20 626f 6c64 3d54 7275  =WHITE, bold=Tru
-0003cc30: 6529 0a20 2020 2063 6f6c 756d 6e5f 7374  e).    column_st
-0003cc40: 796c 6520 3d20 5374 796c 6528 6267 636f  yle = Style(bgco
-0003cc50: 6c6f 723d 4752 4559 2c20 636f 6c6f 723d  lor=GREY, color=
-0003cc60: 5748 4954 452c 2062 6f6c 643d 4661 6c73  WHITE, bold=Fals
-0003cc70: 6529 200a 0a20 2020 206d 6169 6e5f 7461  e) ..    main_ta
-0003cc80: 626c 6520 3d20 5461 626c 6528 7368 6f77  ble = Table(show
-0003cc90: 5f68 6561 6465 723d 5472 7565 2c0a 2020  _header=True,.  
+0003c200: 616e 6973 6174 696f 6e20 5479 7065 222c  anisation Type",
+0003c210: 2020 2249 6e74 2054 7265 6174 2053 616d    "Int Treat Sam
+0003c220: 706c 6520 5369 7a65 222c 2020 2249 6e74  ple Size",  "Int
+0003c230: 2054 7265 6174 2047 7270 2050 6f73 742d   Treat Grp Post-
+0003c240: 7465 7374 204d 6561 6e2f 5344 222c 2020  test Mean/SD",  
+0003c250: 2243 6f6e 6669 6465 6e63 6520 496e 7465  "Confidence Inte
+0003c260: 7276 616c 2028 6c62 2922 290a 2020 2020  rval (lb)").    
+0003c270: 6d61 696e 5f74 6162 6c65 322e 6164 645f  main_table2.add_
+0003c280: 726f 7728 2245 636f 6c6f 6769 6361 6c20  row("Ecological 
+0003c290: 5661 6c69 6469 7479 222c 2022 496e 7420  Validity", "Int 
+0003c2a0: 5472 6169 6e69 6e67 222c 2020 2249 6e74  Training",  "Int
+0003c2b0: 2043 6f6e 7420 5361 6d70 6c65 2053 697a   Cont Sample Siz
+0003c2c0: 6522 2c20 2022 496e 7420 5472 6561 7420  e",  "Int Treat 
+0003c2d0: 4772 7020 4761 696e 2053 636f 7265 204d  Grp Gain Score M
+0003c2e0: 6561 6e2f 5344 222c 2020 2243 6f6e 6669  ean/SD",  "Confi
+0003c2f0: 6465 6e63 6520 496e 7465 7276 616c 2028  dence Interval (
+0003c300: 7562 2922 290a 2020 2020 6d61 696e 5f74  ub)").    main_t
+0003c310: 6162 6c65 322e 6164 645f 726f 7728 2253  able2.add_row("S
+0003c320: 7475 6465 6e74 2041 6765 222c 2020 2249  tudent Age",  "I
+0003c330: 6e74 2046 6f63 7573 222c 2020 2249 6e74  nt Focus",  "Int
+0003c340: 2054 7265 6174 2047 7270 3220 5361 6d70   Treat Grp2 Samp
+0003c350: 6c65 2053 697a 6522 2c20 2022 496e 7420  le Size",  "Int 
+0003c360: 5472 6561 7420 4772 7020 416e 7920 4f74  Treat Grp Any Ot
+0003c370: 6865 7220 496e 666f 222c 2020 224f 7574  her Info",  "Out
+0003c380: 636f 6d65 2229 0a20 2020 206d 6169 6e5f  come").    main_
+0003c390: 7461 626c 6532 2e61 6464 5f72 6f77 2822  table2.add_row("
+0003c3a0: 4e75 6d62 6572 206f 6620 5363 686f 6f6c  Number of School
+0003c3b0: 7322 2c20 2022 496e 7420 5465 6163 6869  s",  "Int Teachi
+0003c3c0: 6e67 2041 7070 726f 6163 6822 2c20 2022  ng Approach",  "
+0003c3d0: 496e 7420 5472 6561 7420 4772 7033 2053  Int Treat Grp3 S
+0003c3e0: 616d 706c 6520 5369 7a65 222c 2020 2249  ample Size",  "I
+0003c3f0: 6e74 2043 6f6e 7420 4772 7020 4e75 6d62  nt Cont Grp Numb
+0003c400: 6572 222c 2020 2253 616d 706c 6522 290a  er",  "Sample").
+0003c410: 2020 2020 6d61 696e 5f74 6162 6c65 322e      main_table2.
+0003c420: 6164 645f 726f 7728 224e 756d 6265 7220  add_row("Number 
+0003c430: 6f66 2043 6c61 7373 6573 222c 2020 2249  of Classes",  "I
+0003c440: 6e74 2049 6e63 6c75 7369 6f6e 222c 2020  nt Inclusion",  
+0003c450: 2249 6e74 2054 7265 6174 2053 616d 706c  "Int Treat Sampl
+0003c460: 6520 5369 7a65 2041 6e61 6c79 7a65 6422  e Size Analyzed"
+0003c470: 2c20 2022 496e 7420 436f 6e74 2047 7270  ,  "Int Cont Grp
+0003c480: 2050 7265 2d74 6573 7420 4d65 616e 2f53   Pre-test Mean/S
+0003c490: 4422 2c20 2022 4f75 7463 6f6d 6520 436f  D",  "Outcome Co
+0003c4a0: 6d70 6172 6973 6f6e 2229 0a20 2020 206d  mparison").    m
+0003c4b0: 6169 6e5f 7461 626c 6532 2e61 6464 5f72  ain_table2.add_r
+0003c4c0: 6f77 2822 5472 6561 746d 656e 7420 4772  ow("Treatment Gr
+0003c4d0: 6f75 7022 2c20 2022 496e 7420 5469 6d65  oup",  "Int Time
+0003c4e0: 222c 2020 2249 6e74 2043 6f6e 7420 5361  ",  "Int Cont Sa
+0003c4f0: 6d70 6c65 2053 697a 6520 416e 616c 797a  mple Size Analyz
+0003c500: 6564 222c 2020 2249 6e74 2043 6f6e 7420  ed",  "Int Cont 
+0003c510: 4772 7020 506f 7374 2d74 6573 7420 4d65  Grp Post-test Me
+0003c520: 616e 2f53 4422 2c20 2022 4566 6665 6374  an/SD",  "Effect
+0003c530: 2053 697a 6520 5479 7065 2229 0a20 2020   Size Type").   
+0003c540: 206d 6169 6e5f 7461 626c 6532 2e61 6464   main_table2.add
+0003c550: 5f72 6f77 2822 5061 7274 6963 6970 616e  _row("Participan
+0003c560: 7420 4173 7369 676e 6d65 6e74 222c 2020  t Assignment",  
+0003c570: 2249 6e74 2044 656c 6976 6572 7922 2c20  "Int Delivery", 
+0003c580: 2022 496e 7420 5472 6561 7420 4772 7032   "Int Treat Grp2
+0003c590: 2053 616d 706c 6520 5369 7a65 2041 6e61   Sample Size Ana
+0003c5a0: 6c79 7a65 6422 2c20 2022 496e 7420 436f  lyzed",  "Int Co
+0003c5b0: 6e74 2047 7270 2047 6169 6e20 5363 6f72  nt Grp Gain Scor
+0003c5c0: 6520 4d65 616e 2f53 4422 2c20 2022 4f75  e Mean/SD",  "Ou
+0003c5d0: 7463 6f6d 6520 4d65 6173 7572 6522 290a  tcome Measure").
+0003c5e0: 2020 2020 6d61 696e 5f74 6162 6c65 322e      main_table2.
+0003c5f0: 6164 645f 726f 7728 224c 6576 656c 206f  add_row("Level o
+0003c600: 6620 4173 7369 676e 6d65 6e74 222c 2022  f Assignment", "
+0003c610: 496e 7420 4475 7261 7469 6f6e 222c 2020  Int Duration",  
+0003c620: 2249 6e74 2043 6f6e 7420 4772 7032 2053  "Int Cont Grp2 S
+0003c630: 616d 706c 6520 5369 7a65 2041 6e61 6c79  ample Size Analy
+0003c640: 7a65 6422 2c20 2022 496e 7420 436f 6e74  zed",  "Int Cont
+0003c650: 2047 7270 2041 6e79 204f 7468 6572 2049   Grp Any Other I
+0003c660: 6e66 6f22 2c20 2022 4f75 7463 6f6d 6520  nfo",  "Outcome 
+0003c670: 5469 746c 6522 290a 2020 2020 6d61 696e  Title").    main
+0003c680: 5f74 6162 6c65 322e 6164 645f 726f 7728  _table2.add_row(
+0003c690: 2253 7475 6479 2044 6573 6967 6e22 2c20  "Study Design", 
+0003c6a0: 2249 6e74 2046 7265 7175 656e 6379 222c  "Int Frequency",
+0003c6b0: 2020 2241 7474 7269 7469 6f6e 2052 6570    "Attrition Rep
+0003c6c0: 6f72 7465 6422 2c20 2022 496e 7420 5472  orted",  "Int Tr
+0003c6d0: 6561 7420 4772 7032 204e 756d 6265 7222  eat Grp2 Number"
+0003c6e0: 2c20 2022 4772 6f75 7031 204e 2229 0a20  ,  "Group1 N"). 
+0003c6f0: 2020 206d 6169 6e5f 7461 626c 6532 2e61     main_table2.a
+0003c700: 6464 5f72 6f77 2820 2252 616e 646f 6d69  dd_row( "Randomi
+0003c710: 7361 7469 6f6e 222c 2020 2249 6e74 2053  sation",  "Int S
+0003c720: 6573 7369 6f6e 204c 656e 6774 6822 2c20  ession Length", 
+0003c730: 2022 4174 7472 6974 696f 6e20 5472 6561   "Attrition Trea
+0003c740: 7420 4772 7022 2c20 2022 496e 7420 5472  t Grp",  "Int Tr
+0003c750: 6561 7420 4772 7032 2050 7265 2d74 6573  eat Grp2 Pre-tes
+0003c760: 7420 4d65 616e 2f53 4422 2c20 2022 4772  t Mean/SD",  "Gr
+0003c770: 6f75 7032 204e 2229 0a20 2020 206d 6169  oup2 N").    mai
+0003c780: 6e5f 7461 626c 6532 2e61 6464 5f72 6f77  n_table2.add_row
+0003c790: 2822 4f74 6865 7220 4f75 7463 6f6d 6573  ("Other Outcomes
+0003c7a0: 222c 2020 2249 6e74 2044 6574 6169 6c22  ",  "Int Detail"
+0003c7b0: 2c20 2022 4174 7472 6974 696f 6e20 546f  ,  "Attrition To
+0003c7c0: 7461 6c20 2825 2922 2c20 2022 496e 7420  tal (%)",  "Int 
+0003c7d0: 5472 6561 7420 4772 7032 2050 6f73 742d  Treat Grp2 Post-
+0003c7e0: 7465 7374 204d 6561 6e2f 5344 222c 2020  test Mean/SD",  
+0003c7f0: 2247 726f 7570 3120 4d65 616e 2229 0a20  "Group1 Mean"). 
+0003c800: 2020 206d 6169 6e5f 7461 626c 6532 2e61     main_table2.a
+0003c810: 6464 5f72 6f77 2822 4164 6469 7469 6f6e  dd_row("Addition
+0003c820: 616c 204f 7574 636f 6d65 7322 2c20 2022  al Outcomes",  "
+0003c830: 496e 7420 436f 7374 7322 2c20 2222 2c20  Int Costs", "", 
+0003c840: 2249 6e74 2054 7265 6174 2047 7270 3220  "Int Treat Grp2 
+0003c850: 4761 696e 2053 636f 7265 204d 6561 6e2f  Gain Score Mean/
+0003c860: 5344 222c 2022 4772 6f75 7032 204d 6561  SD", "Group2 Mea
+0003c870: 6e22 290a 2020 2020 6d61 696e 5f74 6162  n").    main_tab
+0003c880: 6c65 322e 6164 645f 726f 7728 224f 7468  le2.add_row("Oth
+0003c890: 6572 2050 6172 7469 6369 7061 6e74 7320  er Participants 
+0003c8a0: 4f75 7463 6f6d 6573 222c 2022 496e 7420  Outcomes", "Int 
+0003c8b0: 4576 616c 7561 7469 6f6e 222c 2020 2222  Evaluation",  ""
+0003c8c0: 2c20 2020 2249 6e74 2054 7265 6174 2047  ,   "Int Treat G
+0003c8d0: 7270 3220 416e 7920 4f74 6865 7220 496e  rp2 Any Other In
+0003c8e0: 666f 222c 2022 4772 6f75 7031 2053 4422  fo", "Group1 SD"
+0003c8f0: 290a 2020 2020 6d61 696e 5f74 6162 6c65  ).    main_table
+0003c900: 322e 6164 645f 726f 7728 2222 2c20 2022  2.add_row("",  "
+0003c910: 4261 7365 6c69 6e65 2044 6966 6665 7265  Baseline Differe
+0003c920: 6e63 6573 222c 2022 222c 2020 2249 6e74  nces", "",  "Int
+0003c930: 2043 6f6e 7420 4772 7032 204e 756d 6265   Cont Grp2 Numbe
+0003c940: 7222 2c20 2022 4772 6f75 7032 2053 4422  r",  "Group2 SD"
+0003c950: 290a 2020 2020 6d61 696e 5f74 6162 6c65  ).    main_table
+0003c960: 322e 6164 645f 726f 7728 2222 2c20 2243  2.add_row("", "C
+0003c970: 6f6d 7075 7461 7469 6f6e 616c 2041 6e61  omputational Ana
+0003c980: 6c79 7369 7322 2c20 2022 222c 2022 496e  lysis",  "", "In
+0003c990: 7420 436f 6e74 2047 7270 3220 5072 652d  t Cont Grp2 Pre-
+0003c9a0: 7465 7374 204d 6561 6e2f 5344 222c 2020  test Mean/SD",  
+0003c9b0: 224f 7574 636f 6d65 2044 6573 6372 6970  "Outcome Descrip
+0003c9c0: 7469 6f6e 2229 0a20 2020 206d 6169 6e5f  tion").    main_
+0003c9d0: 7461 626c 6532 2e61 6464 5f72 6f77 2822  table2.add_row("
+0003c9e0: 222c 2020 2243 6f6d 7061 7261 6269 6c69  ",  "Comparabili
+0003c9f0: 7479 2056 6172 6961 626c 6573 2052 6570  ty Variables Rep
+0003ca00: 6f72 7465 6422 2c20 2022 222c 2022 496e  orted",  "", "In
+0003ca10: 7420 436f 6e74 2047 7270 3220 506f 7374  t Cont Grp2 Post
+0003ca20: 2d74 6573 7420 4d65 616e 2f53 4422 2c20  -test Mean/SD", 
+0003ca30: 2022 5465 7374 2054 7970 6520 4f75 7463   "Test Type Outc
+0003ca40: 6f6d 6522 290a 2020 2020 6d61 696e 5f74  ome").    main_t
+0003ca50: 6162 6c65 322e 6164 645f 726f 7728 2222  able2.add_row(""
+0003ca60: 2c20 2022 436c 7573 7465 7269 6e67 222c  ,  "Clustering",
+0003ca70: 2020 2222 2c20 2249 6e74 2043 6f6e 7420    "", "Int Cont 
+0003ca80: 4772 7032 2047 6169 6e20 5363 6f72 6520  Grp2 Gain Score 
+0003ca90: 4d65 616e 2f53 4422 2c20 2222 290a 2020  Mean/SD", "").  
+0003caa0: 2020 6d61 696e 5f74 6162 6c65 322e 6164    main_table2.ad
+0003cab0: 645f 726f 7728 2222 2c20 2022 222c 2022  d_row("",  "", "
+0003cac0: 222c 2020 2249 6e74 2043 6f6e 7420 4772  ",  "Int Cont Gr
+0003cad0: 7032 2041 6e79 204f 7468 6572 2049 6e66  p2 Any Other Inf
+0003cae0: 6f22 2c20 2222 290a 2020 2020 6d61 696e  o", "").    main
+0003caf0: 5f74 6162 6c65 322e 6164 645f 726f 7728  _table2.add_row(
+0003cb00: 2222 2c20 2022 222c 2022 222c 2020 2246  "",  "", "",  "F
+0003cb10: 6f6c 6c6f 772d 7570 2049 6e66 6f72 6d61  ollow-up Informa
+0003cb20: 7469 6f6e 222c 2022 2229 0a20 2020 206d  tion", "").    m
+0003cb30: 6169 6e5f 7461 626c 6532 2e66 6f6f 7465  ain_table2.foote
+0003cb40: 7220 3d20 2254 6869 7320 6973 2074 6865  r = "This is the
+0003cb50: 2066 6f6f 7465 722e 220a 2020 2020 7265   footer.".    re
+0003cb60: 7475 726e 206d 6169 6e5f 7461 626c 6532  turn main_table2
+0003cb70: 0a0a 0a64 6566 2064 6973 706c 6179 5f6d  ...def display_m
+0003cb80: 6169 6e5f 6d65 6e75 2829 3a0a 2020 2020  ain_menu():.    
+0003cb90: 7461 626c 655f 7469 746c 655f 7374 796c  table_title_styl
+0003cba0: 6520 3d20 5374 796c 6528 6974 616c 6963  e = Style(italic
+0003cbb0: 3d46 616c 7365 2c20 6267 636f 6c6f 723d  =False, bgcolor=
+0003cbc0: 4e6f 6e65 2c20 636f 6c6f 723d 2223 6663  None, color="#fc
+0003cbd0: 3534 3234 222c 2062 6f6c 643d 5472 7565  5424", bold=True
+0003cbe0: 290a 2020 2020 6865 6164 6572 5f73 7479  ).    header_sty
+0003cbf0: 6c65 203d 2053 7479 6c65 2869 7461 6c69  le = Style(itali
+0003cc00: 633d 4661 6c73 652c 2062 6763 6f6c 6f72  c=False, bgcolor
+0003cc10: 3d22 2366 6335 3432 3422 2c20 636f 6c6f  ="#fc5424", colo
+0003cc20: 723d 5748 4954 452c 2062 6f6c 643d 5472  r=WHITE, bold=Tr
+0003cc30: 7565 290a 2020 2020 636f 6c75 6d6e 5f73  ue).    column_s
+0003cc40: 7479 6c65 203d 2053 7479 6c65 2862 6763  tyle = Style(bgc
+0003cc50: 6f6c 6f72 3d47 5245 592c 2063 6f6c 6f72  olor=GREY, color
+0003cc60: 3d57 4849 5445 2c20 626f 6c64 3d46 616c  =WHITE, bold=Fal
+0003cc70: 7365 2920 0a0a 2020 2020 6d61 696e 5f74  se) ..    main_t
+0003cc80: 6162 6c65 203d 2054 6162 6c65 2873 686f  able = Table(sho
+0003cc90: 775f 6865 6164 6572 3d54 7275 652c 0a20  w_header=True,. 
 0003cca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003ccb0: 2020 2020 2068 6967 686c 6967 6874 3d46       highlight=F
-0003ccc0: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-0003ccd0: 2020 2020 2020 2020 2020 2020 2074 6974               tit
-0003cce0: 6c65 3d4e 6f6e 652c 0a20 2020 2020 2020  le=None,.       
+0003ccb0: 2020 2020 2020 6869 6768 6c69 6768 743d        highlight=
+0003ccc0: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
+0003ccd0: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+0003cce0: 746c 653d 4e6f 6e65 2c0a 2020 2020 2020  tle=None,.      
 0003ccf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003cd00: 7469 746c 655f 7374 796c 653d 7461 626c  title_style=tabl
-0003cd10: 655f 7469 746c 655f 7374 796c 652c 0a20  e_title_style,. 
+0003cd00: 2074 6974 6c65 5f73 7479 6c65 3d74 6162   title_style=tab
+0003cd10: 6c65 5f74 6974 6c65 5f73 7479 6c65 2c0a  le_title_style,.
 0003cd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003cd30: 2020 2020 2020 626f 783d 626f 782e 5349        box=box.SI
-0003cd40: 4d50 4c45 290a 0a20 2020 2073 656c 6563  MPLE)..    selec
-0003cd50: 7469 6f6e 5f73 7479 6c65 203d 2053 7479  tion_style = Sty
-0003cd60: 6c65 2869 7461 6c69 633d 4661 6c73 652c  le(italic=False,
-0003cd70: 2062 6763 6f6c 6f72 3d47 5245 592c 2063   bgcolor=GREY, c
-0003cd80: 6f6c 6f72 3d22 2366 6335 3432 3422 2c20  olor="#fc5424", 
-0003cd90: 626f 6c64 3d54 7275 6529 0a20 2020 2064  bold=True).    d
-0003cda0: 6573 6372 6970 7469 6f6e 5f73 7479 6c65  escription_style
-0003cdb0: 203d 2053 7479 6c65 2869 7461 6c69 633d   = Style(italic=
-0003cdc0: 4661 6c73 652c 2062 6763 6f6c 6f72 3d47  False, bgcolor=G
-0003cdd0: 5245 592c 2063 6f6c 6f72 3d22 2366 6335  REY, color="#fc5
-0003cde0: 3432 3422 2c20 626f 6c64 3d54 7275 6529  424", bold=True)
-0003cdf0: 0a0a 2020 2020 6d61 696e 5f74 6162 6c65  ..    main_table
-0003ce00: 2e61 6464 5f63 6f6c 756d 6e28 2253 656c  .add_column("Sel
-0003ce10: 6563 7469 6f6e 222c 2068 6561 6465 725f  ection", header_
-0003ce20: 7374 796c 653d 7365 6c65 6374 696f 6e5f  style=selection_
-0003ce30: 7374 796c 652c 2073 7479 6c65 3d63 6f6c  style, style=col
-0003ce40: 756d 6e5f 7374 796c 6529 0a20 2020 206d  umn_style).    m
-0003ce50: 6169 6e5f 7461 626c 652e 6164 645f 636f  ain_table.add_co
-0003ce60: 6c75 6d6e 2822 4465 7363 7269 7074 696f  lumn("Descriptio
-0003ce70: 6e22 2c20 6865 6164 6572 5f73 7479 6c65  n", header_style
-0003ce80: 3d64 6573 6372 6970 7469 6f6e 5f73 7479  =description_sty
-0003ce90: 6c65 2c20 7374 796c 653d 636f 6c75 6d6e  le, style=column
-0003cea0: 5f73 7479 6c65 290a 0a20 2020 206d 6169  _style)..    mai
-0003ceb0: 6e5f 7461 626c 652e 6164 645f 726f 7728  n_table.add_row(
-0003cec0: 2220 312e 2044 6174 6166 7261 6d65 2031  " 1. Dataframe 1
-0003ced0: 222c 2020 2020 2020 2253 7475 6479 2c20  ",      "Study, 
-0003cee0: 5265 7365 6172 6368 2026 2044 6573 6967  Research & Desig
-0003cef0: 6e20 5661 7269 6162 6c65 7322 290a 2020  n Variables").  
-0003cf00: 2020 6d61 696e 5f74 6162 6c65 2e61 6464    main_table.add
-0003cf10: 5f72 6f77 2822 2032 2e20 4461 7461 6672  _row(" 2. Datafr
-0003cf20: 616d 6520 3222 2c20 2020 2020 2022 496e  ame 2",      "In
-0003cf30: 7465 7276 656e 7469 6f6e 2044 6574 6169  tervention Detai
-0003cf40: 6c73 2229 0a20 2020 206d 6169 6e5f 7461  ls").    main_ta
-0003cf50: 626c 652e 6164 645f 726f 7728 2220 332e  ble.add_row(" 3.
-0003cf60: 2053 616d 706c 6520 5369 7a65 222c 2020   Sample Size",  
-0003cf70: 2020 2020 2253 616d 706c 6520 7369 7a65      "Sample size
-0003cf80: 2076 6172 6961 626c 6573 2229 0a20 2020   variables").   
-0003cf90: 206d 6169 6e5f 7461 626c 652e 6164 645f   main_table.add_
-0003cfa0: 726f 7728 2220 342e 2045 6666 6563 7420  row(" 4. Effect 
-0003cfb0: 5369 7a65 2041 222c 2020 2020 2244 6573  Size A",    "Des
-0003cfc0: 6372 6970 7469 7665 2053 7461 7469 7374  criptive Statist
-0003cfd0: 6963 7322 290a 2020 2020 6d61 696e 5f74  ics").    main_t
-0003cfe0: 6162 6c65 2e61 6464 5f72 6f77 2822 2035  able.add_row(" 5
-0003cff0: 2e20 4566 6665 6374 2053 697a 6520 4222  . Effect Size B"
-0003d000: 2c20 2020 2022 4f75 7463 6f6d 6520 4465  ,    "Outcome De
-0003d010: 7461 696c 7322 290a 2020 2020 6d61 696e  tails").    main
-0003d020: 5f74 6162 6c65 2e61 6464 5f72 6f77 2822  _table.add_row("
-0003d030: 2036 2e20 4461 7461 2041 6e61 6c79 7369   6. Data Analysi
-0003d040: 7322 2c20 2020 2022 4b65 7920 7661 7269  s",    "Key vari
-0003d050: 6162 6c65 7320 666f 7220 6461 7461 2061  ables for data a
-0003d060: 6e61 6c79 7369 7322 290a 2020 2020 6d61  nalysis").    ma
-0003d070: 696e 5f74 6162 6c65 2e61 6464 5f72 6f77  in_table.add_row
-0003d080: 2822 2037 2e20 4f75 7463 6f6d 6520 4461  (" 7. Outcome Da
-0003d090: 7461 222c 2020 2020 2022 5261 7720 6f75  ta",     "Raw ou
-0003d0a0: 7463 6f6d 6520 6461 7461 2229 0a20 2020  tcome data").   
-0003d0b0: 206d 6169 6e5f 7461 626c 652e 6164 645f   main_table.add_
-0003d0c0: 726f 7728 2220 382e 2053 7475 6479 2053  row(" 8. Study S
-0003d0d0: 6563 7572 6974 7922 2c20 2020 2020 2253  ecurity",     "S
-0003d0e0: 7475 6479 2053 6563 7572 6974 7920 6361  tudy Security ca
-0003d0f0: 6c63 756c 6174 696f 6e73 2229 0a20 2020  lculations").   
-0003d100: 206d 6169 6e5f 7461 626c 652e 6164 645f   main_table.add_
-0003d110: 726f 7728 2220 392e 2050 6164 6c6f 636b  row(" 9. Padlock
-0003d120: 7322 2c20 2020 2020 2020 2253 7472 616e  s",       "Stran
-0003d130: 6420 6c65 7665 6c20 7061 646c 6f63 6b20  d level padlock 
-0003d140: 6461 7461 2229 0a20 2020 206d 6169 6e5f  data").    main_
-0003d150: 7461 626c 652e 6164 645f 726f 7728 2231  table.add_row("1
-0003d160: 302e 2052 6566 6572 656e 6365 7322 2c20  0. References", 
-0003d170: 2020 2020 2244 6174 6120 666f 7220 636f      "Data for co
-0003d180: 6e73 7472 7563 7469 6e67 2073 7475 6479  nstructing study
-0003d190: 2072 6566 6572 656e 6365 7322 290a 2020   references").  
-0003d1a0: 2020 6d61 696e 5f74 6162 6c65 2e61 6464    main_table.add
-0003d1b0: 5f72 6f77 2822 3131 2e20 4375 7374 6f6d  _row("11. Custom
-0003d1c0: 2053 656c 6563 7469 6f6e 222c 2022 5365   Selection", "Se
-0003d1d0: 6c65 6374 2079 6f75 7220 6f77 6e20 6375  lect your own cu
-0003d1e0: 7374 6f6d 2064 6174 6120 6672 616d 6522  stom data frame"
-0003d1f0: 290a 0a20 2020 206d 6169 6e5f 7461 626c  )..    main_tabl
-0003d200: 652e 6164 645f 726f 7728 2222 2c20 2222  e.add_row("", ""
-0003d210: 290a 0a20 2020 206d 6169 6e5f 7461 626c  )..    main_tabl
-0003d220: 652e 6164 645f 726f 7728 2220 302e 2045  e.add_row(" 0. E
-0003d230: 5849 5422 2c20 2222 290a 2020 2020 7265  XIT", "").    re
-0003d240: 7475 726e 206d 6169 6e5f 7461 626c 650a  turn main_table.
-0003d250: 0a0a 6465 6620 6461 7461 6672 616d 655f  ..def dataframe_
-0003d260: 315f 6f75 7470 7574 5f64 6973 706c 6179  1_output_display
-0003d270: 2866 756e 6374 696f 6e73 2c20 6f75 7466  (functions, outf
-0003d280: 696c 6529 3a0a 2020 2020 636f 6e73 6f6c  ile):.    consol
-0003d290: 6520 3d20 436f 6e73 6f6c 6528 290a 2020  e = Console().  
-0003d2a0: 2020 6375 7374 6f6d 5f73 7479 6c65 5f64    custom_style_d
-0003d2b0: 6631 203d 2053 7479 6c65 2862 6763 6f6c  f1 = Style(bgcol
-0003d2c0: 6f72 3d47 5245 5929 0a0a 2020 2020 6466  or=GREY)..    df
-0003d2d0: 315f 7461 626c 6520 3d20 5461 626c 6528  1_table = Table(
-0003d2e0: 7368 6f77 5f68 6561 6465 723d 5472 7565  show_header=True
-0003d2f0: 2c20 0a20 2020 2020 2020 2020 2020 2020  , .             
-0003d300: 2020 2020 2020 2020 2073 7479 6c65 3d63           style=c
-0003d310: 7573 746f 6d5f 7374 796c 655f 6466 312c  ustom_style_df1,
-0003d320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0003d330: 2020 2020 2020 2074 6974 6c65 3d4e 6f6e         title=Non
-0003d340: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0003d350: 2020 2020 2020 2020 2073 6166 655f 626f           safe_bo
-0003d360: 783d 4661 6c73 652c 0a20 2020 2020 2020  x=False,.       
-0003d370: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0003d380: 6f78 3d62 6f78 2e53 494d 504c 4529 0a0a  ox=box.SIMPLE)..
-0003d390: 2020 2020 6466 315f 7461 626c 652e 6164      df1_table.ad
-0003d3a0: 645f 636f 6c75 6d6e 2822 5365 6c65 6374  d_column("Select
-0003d3b0: 696f 6e22 2c20 6a75 7374 6966 793d 2263  ion", justify="c
-0003d3c0: 656e 7465 7222 2c20 6865 6164 6572 5f73  enter", header_s
-0003d3d0: 7479 6c65 3d22 2366 6335 3432 3422 290a  tyle="#fc5424").
-0003d3e0: 2020 2020 6466 315f 7461 626c 652e 6164      df1_table.ad
-0003d3f0: 645f 636f 6c75 6d6e 2822 4f75 7470 7574  d_column("Output
-0003d400: 2064 6972 6563 746f 7279 222c 206a 7573   directory", jus
-0003d410: 7469 6679 3d22 6c65 6674 222c 2068 6561  tify="left", hea
-0003d420: 6465 725f 7374 796c 653d 2223 6663 3534  der_style="#fc54
-0003d430: 3234 2229 0a20 2020 2064 6631 5f74 6162  24").    df1_tab
-0003d440: 6c65 2e61 6464 5f72 6f77 2822 4461 7461  le.add_row("Data
-0003d450: 6672 616d 6520 3122 2c20 6f75 7466 696c  frame 1", outfil
-0003d460: 652c 2073 7479 6c65 3d57 4849 5445 290a  e, style=WHITE).
-0003d470: 0a20 2020 2072 6574 7572 6e20 6466 315f  .    return df1_
-0003d480: 7461 626c 650a 0a0a 6465 6620 6461 7461  table...def data
-0003d490: 6672 616d 655f 325f 6f75 7470 7574 5f64  frame_2_output_d
-0003d4a0: 6973 706c 6179 2866 756e 6374 696f 6e73  isplay(functions
-0003d4b0: 2c20 6f75 7466 696c 6529 3a0a 2020 2020  , outfile):.    
-0003d4c0: 636f 6e73 6f6c 6520 3d20 436f 6e73 6f6c  console = Consol
-0003d4d0: 6528 290a 2020 2020 6375 7374 6f6d 5f73  e().    custom_s
-0003d4e0: 7479 6c65 5f64 6631 203d 2053 7479 6c65  tyle_df1 = Style
-0003d4f0: 2862 6763 6f6c 6f72 3d47 5245 5929 0a0a  (bgcolor=GREY)..
-0003d500: 2020 2020 6466 325f 7461 626c 6520 3d20      df2_table = 
-0003d510: 5461 626c 6528 7368 6f77 5f68 6561 6465  Table(show_heade
-0003d520: 723d 5472 7565 2c20 0a20 2020 2020 2020  r=True, .       
-0003d530: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0003d540: 7479 6c65 3d63 7573 746f 6d5f 7374 796c  tyle=custom_styl
-0003d550: 655f 6466 312c 0a20 2020 2020 2020 2020  e_df1,.         
-0003d560: 2020 2020 2020 2020 2020 2020 2074 6974               tit
-0003d570: 6c65 3d4e 6f6e 652c 0a20 2020 2020 2020  le=None,.       
-0003d580: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0003d590: 6166 655f 626f 783d 4661 6c73 652c 0a20  afe_box=False,. 
-0003d5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003d5b0: 2020 2020 2062 6f78 3d62 6f78 2e53 494d       box=box.SIM
-0003d5c0: 504c 4529 0a0a 2020 2020 6466 325f 7461  PLE)..    df2_ta
-0003d5d0: 626c 652e 6164 645f 636f 6c75 6d6e 2822  ble.add_column("
-0003d5e0: 5365 6c65 6374 696f 6e22 2c20 6a75 7374  Selection", just
-0003d5f0: 6966 793d 2263 656e 7465 7222 2c20 6865  ify="center", he
-0003d600: 6164 6572 5f73 7479 6c65 3d22 2366 6335  ader_style="#fc5
-0003d610: 3432 3422 290a 2020 2020 6466 325f 7461  424").    df2_ta
-0003d620: 626c 652e 6164 645f 636f 6c75 6d6e 2822  ble.add_column("
-0003d630: 4f75 7470 7574 2064 6972 6563 746f 7279  Output directory
-0003d640: 222c 206a 7573 7469 6679 3d22 6c65 6674  ", justify="left
-0003d650: 222c 2068 6561 6465 725f 7374 796c 653d  ", header_style=
-0003d660: 5748 4954 4529 0a20 2020 2064 6632 5f74  WHITE).    df2_t
-0003d670: 6162 6c65 2e61 6464 5f72 6f77 2822 4461  able.add_row("Da
-0003d680: 7461 6672 616d 6520 3222 2c20 6f75 7466  taframe 2", outf
-0003d690: 696c 652c 2073 7479 6c65 3d57 4849 5445  ile, style=WHITE
-0003d6a0: 290a 0a20 2020 2072 6574 7572 6e20 6466  )..    return df
-0003d6b0: 325f 7461 626c 650a 0a0a 6465 6620 6461  2_table...def da
-0003d6c0: 7461 6672 616d 655f 335f 6f75 7470 7574  taframe_3_output
-0003d6d0: 5f64 6973 706c 6179 2866 756e 6374 696f  _display(functio
-0003d6e0: 6e73 2c20 6f75 7466 696c 6529 3a0a 2020  ns, outfile):.  
-0003d6f0: 2020 636f 6e73 6f6c 6520 3d20 436f 6e73    console = Cons
-0003d700: 6f6c 6528 290a 2020 2020 6375 7374 6f6d  ole().    custom
-0003d710: 5f73 7479 6c65 5f64 6631 203d 2053 7479  _style_df1 = Sty
-0003d720: 6c65 2862 6763 6f6c 6f72 3d47 5245 5929  le(bgcolor=GREY)
-0003d730: 0a0a 2020 2020 6466 335f 7461 626c 6520  ..    df3_table 
-0003d740: 3d20 5461 626c 6528 7368 6f77 5f68 6561  = Table(show_hea
-0003d750: 6465 723d 5472 7565 2c20 0a20 2020 2020  der=True, .     
-0003d760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003d770: 2073 7479 6c65 3d63 7573 746f 6d5f 7374   style=custom_st
-0003d780: 796c 655f 6466 312c 0a20 2020 2020 2020  yle_df1,.       
-0003d790: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0003d7a0: 6974 6c65 3d4e 6f6e 652c 0a20 2020 2020  itle=None,.     
-0003d7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003d7c0: 2073 6166 655f 626f 783d 4661 6c73 652c   safe_box=False,
-0003d7d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0003d7e0: 2020 2020 2020 2062 6f78 3d62 6f78 2e53         box=box.S
-0003d7f0: 494d 504c 4529 0a0a 2020 2020 6466 335f  IMPLE)..    df3_
-0003d800: 7461 626c 652e 6164 645f 636f 6c75 6d6e  table.add_column
-0003d810: 2822 5365 6c65 6374 696f 6e22 2c20 6a75  ("Selection", ju
-0003d820: 7374 6966 793d 2263 656e 7465 7222 2c20  stify="center", 
-0003d830: 6865 6164 6572 5f73 7479 6c65 3d22 2366  header_style="#f
-0003d840: 6335 3432 3422 290a 2020 2020 6466 335f  c5424").    df3_
-0003d850: 7461 626c 652e 6164 645f 636f 6c75 6d6e  table.add_column
-0003d860: 2822 4f75 7470 7574 2064 6972 6563 746f  ("Output directo
-0003d870: 7279 222c 206a 7573 7469 6679 3d22 6c65  ry", justify="le
-0003d880: 6674 222c 2068 6561 6465 725f 7374 796c  ft", header_styl
-0003d890: 653d 5748 4954 4529 0a20 2020 2064 6633  e=WHITE).    df3
-0003d8a0: 5f74 6162 6c65 2e61 6464 5f72 6f77 2822  _table.add_row("
-0003d8b0: 5361 6d70 6c65 2053 697a 6522 2c20 6f75  Sample Size", ou
-0003d8c0: 7466 696c 652c 2073 7479 6c65 3d57 4849  tfile, style=WHI
-0003d8d0: 5445 290a 0a20 2020 2072 6574 7572 6e20  TE)..    return 
-0003d8e0: 6466 335f 7461 626c 650a 0a0a 6465 6620  df3_table...def 
-0003d8f0: 6461 7461 6672 616d 655f 345f 6f75 7470  dataframe_4_outp
-0003d900: 7574 5f64 6973 706c 6179 2866 756e 6374  ut_display(funct
-0003d910: 696f 6e73 2c20 6f75 7466 696c 6529 3a0a  ions, outfile):.
-0003d920: 2020 2020 636f 6e73 6f6c 6520 3d20 436f      console = Co
-0003d930: 6e73 6f6c 6528 290a 2020 2020 6375 7374  nsole().    cust
-0003d940: 6f6d 5f73 7479 6c65 5f64 6631 203d 2053  om_style_df1 = S
-0003d950: 7479 6c65 2862 6763 6f6c 6f72 3d47 5245  tyle(bgcolor=GRE
-0003d960: 5929 0a0a 2020 2020 6466 345f 7461 626c  Y)..    df4_tabl
-0003d970: 6520 3d20 5461 626c 6528 7368 6f77 5f68  e = Table(show_h
-0003d980: 6561 6465 723d 5472 7565 2c20 0a20 2020  eader=True, .   
-0003d990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003d9a0: 2020 2073 7479 6c65 3d63 7573 746f 6d5f     style=custom_
-0003d9b0: 7374 796c 655f 6466 312c 0a20 2020 2020  style_df1,.     
-0003d9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003d9d0: 2074 6974 6c65 3d4e 6f6e 652c 0a20 2020   title=None,.   
-0003d9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003d9f0: 2020 2073 6166 655f 626f 783d 4661 6c73     safe_box=Fals
-0003da00: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0003da10: 2020 2020 2020 2020 2062 6f78 3d62 6f78           box=box
-0003da20: 2e53 494d 504c 4529 0a0a 2020 2020 6466  .SIMPLE)..    df
-0003da30: 345f 7461 626c 652e 6164 645f 636f 6c75  4_table.add_colu
-0003da40: 6d6e 2822 5365 6c65 6374 696f 6e22 2c20  mn("Selection", 
-0003da50: 6a75 7374 6966 793d 2263 656e 7465 7222  justify="center"
-0003da60: 2c20 6865 6164 6572 5f73 7479 6c65 3d22  , header_style="
-0003da70: 2366 6335 3432 3422 290a 2020 2020 6466  #fc5424").    df
-0003da80: 345f 7461 626c 652e 6164 645f 636f 6c75  4_table.add_colu
-0003da90: 6d6e 2822 4f75 7470 7574 2064 6972 6563  mn("Output direc
-0003daa0: 746f 7279 222c 206a 7573 7469 6679 3d22  tory", justify="
-0003dab0: 6c65 6674 222c 2068 6561 6465 725f 7374  left", header_st
-0003dac0: 796c 653d 5748 4954 4529 0a20 2020 2064  yle=WHITE).    d
-0003dad0: 6634 5f74 6162 6c65 2e61 6464 5f72 6f77  f4_table.add_row
-0003dae0: 2822 4566 6665 6374 2053 697a 6520 4122  ("Effect Size A"
-0003daf0: 2c20 6f75 7466 696c 652c 2073 7479 6c65  , outfile, style
-0003db00: 3d57 4849 5445 290a 0a20 2020 2072 6574  =WHITE)..    ret
-0003db10: 7572 6e20 6466 345f 7461 626c 650a 0a0a  urn df4_table...
-0003db20: 6465 6620 6461 7461 6672 616d 655f 355f  def dataframe_5_
-0003db30: 6f75 7470 7574 5f64 6973 706c 6179 2866  output_display(f
-0003db40: 756e 6374 696f 6e73 2c20 6f75 7466 696c  unctions, outfil
-0003db50: 6529 3a0a 2020 2020 636f 6e73 6f6c 6520  e):.    console 
-0003db60: 3d20 436f 6e73 6f6c 6528 290a 2020 2020  = Console().    
-0003db70: 6375 7374 6f6d 5f73 7479 6c65 5f64 6631  custom_style_df1
-0003db80: 203d 2053 7479 6c65 2862 6763 6f6c 6f72   = Style(bgcolor
-0003db90: 3d47 5245 5929 0a0a 2020 2020 6466 355f  =GREY)..    df5_
-0003dba0: 7461 626c 6520 3d20 5461 626c 6528 7368  table = Table(sh
-0003dbb0: 6f77 5f68 6561 6465 723d 5472 7565 2c20  ow_header=True, 
-0003dbc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0003dbd0: 2020 2020 2020 2073 7479 6c65 3d63 7573         style=cus
-0003dbe0: 746f 6d5f 7374 796c 655f 6466 312c 0a20  tom_style_df1,. 
-0003dbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003dc00: 2020 2020 2074 6974 6c65 3d4e 6f6e 652c       title=None,
-0003dc10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0003dc20: 2020 2020 2020 2073 6166 655f 626f 783d         safe_box=
-0003dc30: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
-0003dc40: 2020 2020 2020 2020 2020 2020 2062 6f78               box
-0003dc50: 3d62 6f78 2e53 494d 504c 4529 0a0a 2020  =box.SIMPLE)..  
-0003dc60: 2020 6466 355f 7461 626c 652e 6164 645f    df5_table.add_
-0003dc70: 636f 6c75 6d6e 2822 5365 6c65 6374 696f  column("Selectio
-0003dc80: 6e22 2c20 6a75 7374 6966 793d 2263 656e  n", justify="cen
-0003dc90: 7465 7222 2c20 6865 6164 6572 5f73 7479  ter", header_sty
-0003dca0: 6c65 3d22 2366 6335 3432 3422 290a 2020  le="#fc5424").  
-0003dcb0: 2020 6466 355f 7461 626c 652e 6164 645f    df5_table.add_
-0003dcc0: 636f 6c75 6d6e 2822 4f75 7470 7574 2064  column("Output d
-0003dcd0: 6972 6563 746f 7279 222c 206a 7573 7469  irectory", justi
-0003dce0: 6679 3d22 6c65 6674 222c 2068 6561 6465  fy="left", heade
-0003dcf0: 725f 7374 796c 653d 5748 4954 4529 0a20  r_style=WHITE). 
-0003dd00: 2020 2064 6635 5f74 6162 6c65 2e61 6464     df5_table.add
-0003dd10: 5f72 6f77 2822 4566 6665 6374 2053 697a  _row("Effect Siz
-0003dd20: 6520 4222 2c20 6f75 7466 696c 652c 2073  e B", outfile, s
-0003dd30: 7479 6c65 3d57 4849 5445 290a 0a20 2020  tyle=WHITE)..   
-0003dd40: 2072 6574 7572 6e20 6466 355f 7461 626c   return df5_tabl
-0003dd50: 650a 0a0a 6465 6620 6461 7461 6672 616d  e...def datafram
-0003dd60: 655f 365f 6f75 7470 7574 5f64 6973 706c  e_6_output_displ
-0003dd70: 6179 2866 756e 6374 696f 6e73 2c20 6f75  ay(functions, ou
-0003dd80: 7466 696c 6529 3a0a 2020 2020 636f 6e73  tfile):.    cons
-0003dd90: 6f6c 6520 3d20 436f 6e73 6f6c 6528 290a  ole = Console().
-0003dda0: 2020 2020 6375 7374 6f6d 5f73 7479 6c65      custom_style
-0003ddb0: 5f64 6631 203d 2053 7479 6c65 2862 6763  _df1 = Style(bgc
-0003ddc0: 6f6c 6f72 3d47 5245 5929 0a0a 2020 2020  olor=GREY)..    
-0003ddd0: 6466 365f 7461 626c 6520 3d20 5461 626c  df6_table = Tabl
-0003dde0: 6528 7368 6f77 5f68 6561 6465 723d 5472  e(show_header=Tr
-0003ddf0: 7565 2c20 0a20 2020 2020 2020 2020 2020  ue, .           
-0003de00: 2020 2020 2020 2020 2020 2073 7479 6c65             style
-0003de10: 3d63 7573 746f 6d5f 7374 796c 655f 6466  =custom_style_df
-0003de20: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-0003de30: 2020 2020 2020 2020 2074 6974 6c65 3d4e           title=N
-0003de40: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-0003de50: 2020 2020 2020 2020 2020 2073 6166 655f             safe_
-0003de60: 626f 783d 4661 6c73 652c 0a20 2020 2020  box=False,.     
-0003de70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003de80: 2062 6f78 3d62 6f78 2e53 494d 504c 4529   box=box.SIMPLE)
-0003de90: 0a0a 2020 2020 6466 365f 7461 626c 652e  ..    df6_table.
-0003dea0: 6164 645f 636f 6c75 6d6e 2822 5365 6c65  add_column("Sele
-0003deb0: 6374 696f 6e22 2c20 6a75 7374 6966 793d  ction", justify=
-0003dec0: 2263 656e 7465 7222 2c20 6865 6164 6572  "center", header
-0003ded0: 5f73 7479 6c65 3d22 2366 6335 3432 3422  _style="#fc5424"
-0003dee0: 290a 2020 2020 6466 365f 7461 626c 652e  ).    df6_table.
-0003def0: 6164 645f 636f 6c75 6d6e 2822 4f75 7470  add_column("Outp
-0003df00: 7574 2064 6972 6563 746f 7279 222c 206a  ut directory", j
-0003df10: 7573 7469 6679 3d22 6c65 6674 222c 2068  ustify="left", h
-0003df20: 6561 6465 725f 7374 796c 653d 2223 6663  eader_style="#fc
-0003df30: 3534 3234 2229 0a20 2020 2064 6636 5f74  5424").    df6_t
-0003df40: 6162 6c65 2e61 6464 5f72 6f77 2822 4d61  able.add_row("Ma
-0003df50: 696e 2041 6e61 6c79 7369 7322 2c20 6f75  in Analysis", ou
-0003df60: 7466 696c 652c 2073 7479 6c65 3d57 4849  tfile, style=WHI
-0003df70: 5445 290a 0a20 2020 2072 6574 7572 6e20  TE)..    return 
-0003df80: 6466 365f 7461 626c 650a 0a0a 6465 6620  df6_table...def 
-0003df90: 6461 7461 6672 616d 655f 375f 6f75 7470  dataframe_7_outp
-0003dfa0: 7574 5f64 6973 706c 6179 2866 756e 6374  ut_display(funct
-0003dfb0: 696f 6e73 2c20 6f75 7466 696c 6529 3a0a  ions, outfile):.
-0003dfc0: 2020 2020 636f 6e73 6f6c 6520 3d20 436f      console = Co
-0003dfd0: 6e73 6f6c 6528 290a 2020 2020 6375 7374  nsole().    cust
-0003dfe0: 6f6d 5f73 7479 6c65 5f64 6631 203d 2053  om_style_df1 = S
-0003dff0: 7479 6c65 2862 6763 6f6c 6f72 3d47 5245  tyle(bgcolor=GRE
-0003e000: 5929 0a0a 2020 2020 6466 375f 7461 626c  Y)..    df7_tabl
-0003e010: 6520 3d20 5461 626c 6528 7368 6f77 5f68  e = Table(show_h
-0003e020: 6561 6465 723d 5472 7565 2c20 0a20 2020  eader=True, .   
-0003e030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003e040: 2020 2073 7479 6c65 3d63 7573 746f 6d5f     style=custom_
-0003e050: 7374 796c 655f 6466 312c 0a20 2020 2020  style_df1,.     
-0003e060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003e070: 2074 6974 6c65 3d4e 6f6e 652c 0a20 2020   title=None,.   
-0003e080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003e090: 2020 2073 6166 655f 626f 783d 4661 6c73     safe_box=Fals
-0003e0a0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0003e0b0: 2020 2020 2020 2020 2062 6f78 3d62 6f78           box=box
-0003e0c0: 2e53 494d 504c 4529 0a0a 2020 2020 6466  .SIMPLE)..    df
-0003e0d0: 375f 7461 626c 652e 6164 645f 636f 6c75  7_table.add_colu
-0003e0e0: 6d6e 2822 5365 6c65 6374 696f 6e22 2c20  mn("Selection", 
-0003e0f0: 6a75 7374 6966 793d 2263 656e 7465 7222  justify="center"
-0003e100: 2c20 6865 6164 6572 5f73 7479 6c65 3d22  , header_style="
-0003e110: 2366 6335 3432 3422 290a 2020 2020 6466  #fc5424").    df
-0003e120: 375f 7461 626c 652e 6164 645f 636f 6c75  7_table.add_colu
-0003e130: 6d6e 2822 4f75 7470 7574 2064 6972 6563  mn("Output direc
-0003e140: 746f 7279 222c 206a 7573 7469 6679 3d22  tory", justify="
-0003e150: 6c65 6674 222c 2068 6561 6465 725f 7374  left", header_st
-0003e160: 796c 653d 2223 6663 3534 3234 2229 0a20  yle="#fc5424"). 
-0003e170: 2020 2064 6637 5f74 6162 6c65 2e61 6464     df7_table.add
-0003e180: 5f72 6f77 2822 4f75 7463 6f6d 6520 4461  _row("Outcome Da
-0003e190: 7461 222c 206f 7574 6669 6c65 2c20 7374  ta", outfile, st
-0003e1a0: 796c 653d 5748 4954 4529 0a0a 2020 2020  yle=WHITE)..    
-0003e1b0: 7265 7475 726e 2064 6637 5f74 6162 6c65  return df7_table
-0003e1c0: 0a0a 6465 6620 6461 7461 6672 616d 655f  ..def dataframe_
-0003e1d0: 385f 6f75 7470 7574 5f64 6973 706c 6179  8_output_display
-0003e1e0: 2866 756e 6374 696f 6e73 2c20 6f75 7466  (functions, outf
-0003e1f0: 696c 6529 3a0a 2020 2020 636f 6e73 6f6c  ile):.    consol
-0003e200: 6520 3d20 436f 6e73 6f6c 6528 290a 2020  e = Console().  
-0003e210: 2020 6375 7374 6f6d 5f73 7479 6c65 5f64    custom_style_d
-0003e220: 6631 203d 2053 7479 6c65 2862 6763 6f6c  f1 = Style(bgcol
-0003e230: 6f72 3d47 5245 5929 0a0a 2020 2020 6466  or=GREY)..    df
-0003e240: 385f 7461 626c 6520 3d20 5461 626c 6528  8_table = Table(
-0003e250: 7368 6f77 5f68 6561 6465 723d 5472 7565  show_header=True
-0003e260: 2c20 0a20 2020 2020 2020 2020 2020 2020  , .             
-0003e270: 2020 2020 2020 2020 2073 7479 6c65 3d63           style=c
-0003e280: 7573 746f 6d5f 7374 796c 655f 6466 312c  ustom_style_df1,
-0003e290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0003e2a0: 2020 2020 2020 2074 6974 6c65 3d4e 6f6e         title=Non
-0003e2b0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0003e2c0: 2020 2020 2020 2020 2073 6166 655f 626f           safe_bo
-0003e2d0: 783d 4661 6c73 652c 0a20 2020 2020 2020  x=False,.       
-0003e2e0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0003e2f0: 6f78 3d62 6f78 2e53 494d 504c 4529 0a0a  ox=box.SIMPLE)..
-0003e300: 2020 2020 6466 385f 7461 626c 652e 6164      df8_table.ad
-0003e310: 645f 636f 6c75 6d6e 2822 5365 6c65 6374  d_column("Select
-0003e320: 696f 6e22 2c20 6a75 7374 6966 793d 2263  ion", justify="c
-0003e330: 656e 7465 7222 2c20 6865 6164 6572 5f73  enter", header_s
-0003e340: 7479 6c65 3d22 2366 6335 3432 3422 290a  tyle="#fc5424").
-0003e350: 2020 2020 6466 385f 7461 626c 652e 6164      df8_table.ad
-0003e360: 645f 636f 6c75 6d6e 2822 4f75 7470 7574  d_column("Output
-0003e370: 2064 6972 6563 746f 7279 222c 206a 7573   directory", jus
-0003e380: 7469 6679 3d22 6c65 6674 222c 2068 6561  tify="left", hea
-0003e390: 6465 725f 7374 796c 653d 2223 6663 3534  der_style="#fc54
-0003e3a0: 3234 2229 0a20 2020 2064 6638 5f74 6162  24").    df8_tab
-0003e3b0: 6c65 2e61 6464 5f72 6f77 2822 5374 7564  le.add_row("Stud
-0003e3c0: 7920 5365 6375 7269 7479 222c 206f 7574  y Security", out
-0003e3d0: 6669 6c65 2c20 7374 796c 653d 5748 4954  file, style=WHIT
-0003e3e0: 4529 0a0a 2020 2020 7265 7475 726e 2064  E)..    return d
-0003e3f0: 6638 5f74 6162 6c65 0a0a 6465 6620 6461  f8_table..def da
-0003e400: 7461 6672 616d 655f 395f 6f75 7470 7574  taframe_9_output
-0003e410: 5f64 6973 706c 6179 2866 756e 6374 696f  _display(functio
-0003e420: 6e73 2c20 6f75 7466 696c 6529 3a0a 2020  ns, outfile):.  
-0003e430: 2020 636f 6e73 6f6c 6520 3d20 436f 6e73    console = Cons
-0003e440: 6f6c 6528 290a 2020 2020 6375 7374 6f6d  ole().    custom
-0003e450: 5f73 7479 6c65 5f64 6631 203d 2053 7479  _style_df1 = Sty
-0003e460: 6c65 2862 6763 6f6c 6f72 3d47 5245 5929  le(bgcolor=GREY)
-0003e470: 0a0a 2020 2020 6466 395f 7461 626c 6520  ..    df9_table 
-0003e480: 3d20 5461 626c 6528 7368 6f77 5f68 6561  = Table(show_hea
-0003e490: 6465 723d 5472 7565 2c20 0a20 2020 2020  der=True, .     
-0003e4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003e4b0: 2073 7479 6c65 3d63 7573 746f 6d5f 7374   style=custom_st
-0003e4c0: 796c 655f 6466 312c 0a20 2020 2020 2020  yle_df1,.       
-0003e4d0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0003e4e0: 6974 6c65 3d4e 6f6e 652c 0a20 2020 2020  itle=None,.     
-0003e4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003e500: 2073 6166 655f 626f 783d 4661 6c73 652c   safe_box=False,
-0003e510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0003e520: 2020 2020 2020 2062 6f78 3d62 6f78 2e53         box=box.S
-0003e530: 494d 504c 4529 0a0a 2020 2020 6466 395f  IMPLE)..    df9_
-0003e540: 7461 626c 652e 6164 645f 636f 6c75 6d6e  table.add_column
-0003e550: 2822 5365 6c65 6374 696f 6e22 2c20 6a75  ("Selection", ju
-0003e560: 7374 6966 793d 2263 656e 7465 7222 2c20  stify="center", 
-0003e570: 6865 6164 6572 5f73 7479 6c65 3d22 2366  header_style="#f
-0003e580: 6335 3432 3422 290a 2020 2020 6466 395f  c5424").    df9_
-0003e590: 7461 626c 652e 6164 645f 636f 6c75 6d6e  table.add_column
-0003e5a0: 2822 4f75 7470 7574 2064 6972 6563 746f  ("Output directo
-0003e5b0: 7279 222c 206a 7573 7469 6679 3d22 6c65  ry", justify="le
-0003e5c0: 6674 222c 2068 6561 6465 725f 7374 796c  ft", header_styl
-0003e5d0: 653d 2223 6663 3534 3234 2229 0a20 2020  e="#fc5424").   
-0003e5e0: 2064 6639 5f74 6162 6c65 2e61 6464 5f72   df9_table.add_r
-0003e5f0: 6f77 2822 5061 646c 6f63 6b73 222c 206f  ow("Padlocks", o
-0003e600: 7574 6669 6c65 2c20 7374 796c 653d 5748  utfile, style=WH
-0003e610: 4954 4529 0a0a 2020 2020 7265 7475 726e  ITE)..    return
-0003e620: 2064 6639 5f74 6162 6c65 0a0a 6465 6620   df9_table..def 
-0003e630: 6461 7461 6672 616d 655f 3130 5f6f 7574  dataframe_10_out
-0003e640: 7075 745f 6469 7370 6c61 7928 6675 6e63  put_display(func
-0003e650: 7469 6f6e 732c 206f 7574 6669 6c65 293a  tions, outfile):
-0003e660: 0a20 2020 2063 6f6e 736f 6c65 203d 2043  .    console = C
-0003e670: 6f6e 736f 6c65 2829 0a20 2020 2063 7573  onsole().    cus
-0003e680: 746f 6d5f 7374 796c 655f 6466 3120 3d20  tom_style_df1 = 
-0003e690: 5374 796c 6528 6267 636f 6c6f 723d 4752  Style(bgcolor=GR
-0003e6a0: 4559 290a 0a20 2020 2064 6631 305f 7461  EY)..    df10_ta
-0003e6b0: 626c 6520 3d20 5461 626c 6528 7368 6f77  ble = Table(show
-0003e6c0: 5f68 6561 6465 723d 5472 7565 2c20 0a20  _header=True, . 
-0003e6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003e6e0: 2020 2020 2073 7479 6c65 3d63 7573 746f       style=custo
-0003e6f0: 6d5f 7374 796c 655f 6466 312c 0a20 2020  m_style_df1,.   
-0003e700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003e710: 2020 2074 6974 6c65 3d4e 6f6e 652c 0a20     title=None,. 
-0003e720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003e730: 2020 2020 2073 6166 655f 626f 783d 4661       safe_box=Fa
-0003e740: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
-0003e750: 2020 2020 2020 2020 2020 2062 6f78 3d62             box=b
-0003e760: 6f78 2e53 494d 504c 4529 0a0a 2020 2020  ox.SIMPLE)..    
-0003e770: 6466 3130 5f74 6162 6c65 2e61 6464 5f63  df10_table.add_c
-0003e780: 6f6c 756d 6e28 2253 656c 6563 7469 6f6e  olumn("Selection
-0003e790: 222c 206a 7573 7469 6679 3d22 6365 6e74  ", justify="cent
-0003e7a0: 6572 222c 2068 6561 6465 725f 7374 796c  er", header_styl
-0003e7b0: 653d 2223 6663 3534 3234 2229 0a20 2020  e="#fc5424").   
-0003e7c0: 2064 6631 305f 7461 626c 652e 6164 645f   df10_table.add_
-0003e7d0: 636f 6c75 6d6e 2822 4f75 7470 7574 2064  column("Output d
-0003e7e0: 6972 6563 746f 7279 222c 206a 7573 7469  irectory", justi
-0003e7f0: 6679 3d22 6c65 6674 222c 2068 6561 6465  fy="left", heade
-0003e800: 725f 7374 796c 653d 2223 6663 3534 3234  r_style="#fc5424
-0003e810: 2229 0a20 2020 2064 6631 305f 7461 626c  ").    df10_tabl
-0003e820: 652e 6164 645f 726f 7728 2252 6566 6572  e.add_row("Refer
-0003e830: 656e 6365 7322 2c20 6f75 7466 696c 652c  ences", outfile,
-0003e840: 2073 7479 6c65 3d57 4849 5445 290a 0a20   style=WHITE).. 
-0003e850: 2020 2072 6574 7572 6e20 6466 3130 5f74     return df10_t
-0003e860: 6162 6c65 0a0a 6465 6620 6461 7461 6672  able..def datafr
-0003e870: 616d 655f 3131 5f6f 7574 7075 745f 6469  ame_11_output_di
-0003e880: 7370 6c61 7928 6675 6e63 7469 6f6e 732c  splay(functions,
-0003e890: 206f 7574 6669 6c65 293a 0a20 2020 2063   outfile):.    c
-0003e8a0: 6f6e 736f 6c65 203d 2043 6f6e 736f 6c65  onsole = Console
-0003e8b0: 2829 0a20 2020 2063 7573 746f 6d5f 7374  ().    custom_st
-0003e8c0: 796c 655f 6466 3120 3d20 5374 796c 6528  yle_df1 = Style(
-0003e8d0: 6267 636f 6c6f 723d 4752 4559 290a 0a20  bgcolor=GREY).. 
-0003e8e0: 2020 2064 6631 315f 7461 626c 6520 3d20     df11_table = 
-0003e8f0: 5461 626c 6528 7368 6f77 5f68 6561 6465  Table(show_heade
-0003e900: 723d 5472 7565 2c20 0a20 2020 2020 2020  r=True, .       
-0003e910: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0003e920: 7479 6c65 3d63 7573 746f 6d5f 7374 796c  tyle=custom_styl
-0003e930: 655f 6466 312c 0a20 2020 2020 2020 2020  e_df1,.         
-0003e940: 2020 2020 2020 2020 2020 2020 2074 6974               tit
-0003e950: 6c65 3d4e 6f6e 652c 0a20 2020 2020 2020  le=None,.       
-0003e960: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0003e970: 6166 655f 626f 783d 4661 6c73 652c 0a20  afe_box=False,. 
-0003e980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003e990: 2020 2020 2062 6f78 3d62 6f78 2e53 494d       box=box.SIM
-0003e9a0: 504c 4529 0a0a 2020 2020 6466 3131 5f74  PLE)..    df11_t
-0003e9b0: 6162 6c65 2e61 6464 5f63 6f6c 756d 6e28  able.add_column(
-0003e9c0: 2253 656c 6563 7469 6f6e 222c 206a 7573  "Selection", jus
-0003e9d0: 7469 6679 3d22 6365 6e74 6572 222c 2068  tify="center", h
-0003e9e0: 6561 6465 725f 7374 796c 653d 2223 6663  eader_style="#fc
-0003e9f0: 3534 3234 2229 0a20 2020 2064 6631 315f  5424").    df11_
-0003ea00: 7461 626c 652e 6164 645f 636f 6c75 6d6e  table.add_column
-0003ea10: 2822 4f75 7470 7574 2064 6972 6563 746f  ("Output directo
-0003ea20: 7279 222c 206a 7573 7469 6679 3d22 6c65  ry", justify="le
-0003ea30: 6674 222c 2068 6561 6465 725f 7374 796c  ft", header_styl
-0003ea40: 653d 2223 6663 3534 3234 2229 0a20 2020  e="#fc5424").   
-0003ea50: 2064 6631 315f 7461 626c 652e 6164 645f   df11_table.add_
-0003ea60: 726f 7728 2243 7573 746f 6d22 2c20 6f75  row("Custom", ou
-0003ea70: 7466 696c 652c 2073 7479 6c65 3d57 4849  tfile, style=WHI
-0003ea80: 5445 290a 0a20 2020 2072 6574 7572 6e20  TE)..    return 
-0003ea90: 6466 3131 5f74 6162 6c65 0a0a 6465 6620  df11_table..def 
-0003eaa0: 6372 6561 7465 5f6f 7574 7075 745f 6469  create_output_di
-0003eab0: 7370 6c61 795f 7461 626c 6528 6461 7461  splay_table(data
-0003eac0: 6672 616d 655f 6e61 6d65 2c20 6f75 7466  frame_name, outf
-0003ead0: 696c 6529 3a0a 2020 2020 636f 6e73 6f6c  ile):.    consol
-0003eae0: 6520 3d20 436f 6e73 6f6c 6528 290a 2020  e = Console().  
-0003eaf0: 2020 6375 7374 6f6d 5f73 7479 6c65 5f64    custom_style_d
-0003eb00: 6631 203d 2053 7479 6c65 2862 6763 6f6c  f1 = Style(bgcol
-0003eb10: 6f72 3d47 5245 5929 0a0a 2020 2020 6466  or=GREY)..    df
-0003eb20: 5f74 6162 6c65 203d 2054 6162 6c65 2873  _table = Table(s
-0003eb30: 686f 775f 6865 6164 6572 3d54 7275 652c  how_header=True,
-0003eb40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0003eb50: 2020 2020 2020 7374 796c 653d 6375 7374        style=cust
-0003eb60: 6f6d 5f73 7479 6c65 5f64 6631 2c0a 2020  om_style_df1,.  
-0003eb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003eb80: 2020 2074 6974 6c65 3d4e 6f6e 652c 0a20     title=None,. 
-0003eb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003eba0: 2020 2020 7361 6665 5f62 6f78 3d46 616c      safe_box=Fal
-0003ebb0: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-0003ebc0: 2020 2020 2020 2020 2062 6f78 3d62 6f78           box=box
-0003ebd0: 2e53 494d 504c 4529 0a0a 2020 2020 6466  .SIMPLE)..    df
-0003ebe0: 5f74 6162 6c65 2e61 6464 5f63 6f6c 756d  _table.add_colum
-0003ebf0: 6e28 2253 656c 6563 7469 6f6e 222c 206a  n("Selection", j
-0003ec00: 7573 7469 6679 3d22 6365 6e74 6572 222c  ustify="center",
-0003ec10: 2068 6561 6465 725f 7374 796c 653d 2223   header_style="#
-0003ec20: 6663 3534 3234 2229 0a20 2020 2064 665f  fc5424").    df_
-0003ec30: 7461 626c 652e 6164 645f 636f 6c75 6d6e  table.add_column
-0003ec40: 2822 4f75 7470 7574 2064 6972 6563 746f  ("Output directo
-0003ec50: 7279 222c 206a 7573 7469 6679 3d22 6c65  ry", justify="le
-0003ec60: 6674 222c 2068 6561 6465 725f 7374 796c  ft", header_styl
-0003ec70: 653d 2223 6663 3534 3234 2229 0a20 2020  e="#fc5424").   
-0003ec80: 2064 665f 7461 626c 652e 6164 645f 726f   df_table.add_ro
-0003ec90: 7728 6461 7461 6672 616d 655f 6e61 6d65  w(dataframe_name
-0003eca0: 2c20 6f75 7466 696c 652c 2073 7479 6c65  , outfile, style
-0003ecb0: 3d57 4849 5445 290a 0a20 2020 2072 6574  =WHITE)..    ret
-0003ecc0: 7572 6e20 6466 5f74 6162 6c65 0a0a 0a64  urn df_table...d
-0003ecd0: 6566 2069 6e70 7574 5f66 696c 655f 696e  ef input_file_in
-0003ece0: 666f 5f64 6973 706c 6179 2864 6174 615f  fo_display(data_
-0003ecf0: 6669 6c65 293a 0a0a 2020 2020 7461 626c  file):..    tabl
-0003ed00: 655f 7469 746c 655f 7374 796c 6520 3d20  e_title_style = 
-0003ed10: 5374 796c 6528 6974 616c 6963 3d46 616c  Style(italic=Fal
-0003ed20: 7365 2c20 6267 636f 6c6f 723d 4752 4559  se, bgcolor=GREY
-0003ed30: 2c20 636f 6c6f 723d 5748 4954 452c 2062  , color=WHITE, b
-0003ed40: 6f6c 643d 5472 7565 290a 2020 2020 6865  old=True).    he
-0003ed50: 6164 6572 5f73 7479 6c65 203d 2053 7479  ader_style = Sty
-0003ed60: 6c65 2869 7461 6c69 633d 4661 6c73 652c  le(italic=False,
-0003ed70: 2062 6763 6f6c 6f72 3d47 5245 592c 2063   bgcolor=GREY, c
-0003ed80: 6f6c 6f72 3d22 2366 6335 3432 3422 2c20  olor="#fc5424", 
-0003ed90: 626f 6c64 3d54 7275 6529 0a20 2020 2063  bold=True).    c
-0003eda0: 6f6c 756d 6e5f 7374 796c 6520 3d20 5374  olumn_style = St
-0003edb0: 796c 6528 6267 636f 6c6f 723d 4752 4559  yle(bgcolor=GREY
-0003edc0: 2c20 636f 6c6f 723d 5748 4954 4529 200a  , color=WHITE) .
-0003edd0: 0a20 2020 2066 696c 655f 696e 666f 5f74  .    file_info_t
-0003ede0: 6162 6c65 203d 2054 6162 6c65 2873 686f  able = Table(sho
-0003edf0: 775f 6865 6164 6572 3d54 7275 652c 0a20  w_header=True,. 
-0003ee00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003ee10: 2020 2020 2020 6869 6768 6c69 6768 743d        highlight=
-0003ee20: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
-0003ee30: 2020 2020 2020 2020 2020 2020 2020 7469                ti
-0003ee40: 746c 653d 4e6f 6e65 2c0a 2020 2020 2020  tle=None,.      
-0003ee50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003ee60: 2074 6974 6c65 5f73 7479 6c65 3d74 6162   title_style=tab
-0003ee70: 6c65 5f74 6974 6c65 5f73 7479 6c65 2c0a  le_title_style,.
-0003ee80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0003ee90: 2020 2020 2020 2062 6f78 3d62 6f78 2e53         box=box.S
-0003eea0: 494d 504c 4529 0a20 2020 200a 2020 2020  IMPLE).    .    
-0003eeb0: 6669 6c65 5f69 6e66 6f5f 7461 626c 652e  file_info_table.
-0003eec0: 6164 645f 636f 6c75 6d6e 2822 596f 7572  add_column("Your
-0003eed0: 2069 6e70 7574 2066 696c 6522 2c20 6865   input file", he
-0003eee0: 6164 6572 5f73 7479 6c65 3d68 6561 6465  ader_style=heade
-0003eef0: 725f 7374 796c 652c 2073 7479 6c65 3d63  r_style, style=c
-0003ef00: 6f6c 756d 6e5f 7374 796c 6529 0a20 2020  olumn_style).   
-0003ef10: 2066 696c 655f 696e 666f 5f74 6162 6c65   file_info_table
-0003ef20: 2e61 6464 5f72 6f77 2864 6174 615f 6669  .add_row(data_fi
-0003ef30: 6c65 290a 2020 2020 7265 7475 726e 2066  le).    return f
-0003ef40: 696c 655f 696e 666f 5f74 6162 6c65 0a0a  ile_info_table..
-0003ef50: 6465 6620 6d61 696e 5f6d 656e 755f 6469  def main_menu_di
-0003ef60: 7370 6c61 7928 293a 0a20 2020 2063 6f6e  splay():.    con
-0003ef70: 736f 6c65 203d 2043 6f6e 736f 6c65 2829  sole = Console()
-0003ef80: 0a20 2020 2023 6461 7461 5f63 6c65 616e  .    #data_clean
-0003ef90: 696e 675f 7661 725f 7461 626c 6520 3d20  ing_var_table = 
-0003efa0: 6461 7461 5f63 6c65 616e 696e 675f 636f  data_cleaning_co
-0003efb0: 6c5f 6272 6561 6b64 6f77 6e28 290a 2020  l_breakdown().  
-0003efc0: 2020 6d61 696e 5f6d 656e 755f 7461 626c    main_menu_tabl
-0003efd0: 6520 3d20 6469 7370 6c61 795f 6d61 696e  e = display_main
-0003efe0: 5f6d 656e 7528 290a 2020 2020 6461 7461  _menu().    data
-0003eff0: 6669 6c65 5f69 6e66 6f5f 7461 626c 6520  file_info_table 
-0003f000: 3d20 696e 7075 745f 6669 6c65 5f69 6e66  = input_file_inf
-0003f010: 6f5f 6469 7370 6c61 7928 6461 7461 5f66  o_display(data_f
-0003f020: 696c 6529 0a0a 2020 2020 6375 7374 6f6d  ile)..    custom
-0003f030: 5f73 7479 6c65 5f6d 6169 6e20 3d20 5374  _style_main = St
-0003f040: 796c 6528 6267 636f 6c6f 723d 4752 4559  yle(bgcolor=GREY
-0003f050: 290a 2020 2020 6375 7374 6f6d 5f73 7479  ).    custom_sty
-0003f060: 6c65 5f66 696c 655f 6465 7461 696c 7320  le_file_details 
-0003f070: 3d20 5374 796c 6528 6267 636f 6c6f 723d  = Style(bgcolor=
-0003f080: 4752 4559 290a 2020 2020 6375 7374 6f6d  GREY).    custom
-0003f090: 5f73 7479 6c65 5f63 6c65 616e 696e 675f  _style_cleaning_
-0003f0a0: 696e 666f 203d 2053 7479 6c65 2862 6763  info = Style(bgc
-0003f0b0: 6f6c 6f72 3d47 5245 5929 0a0a 2020 2020  olor=GREY)..    
-0003f0c0: 636f 6e74 6169 6e65 725f 7469 746c 6520  container_title 
-0003f0d0: 3d20 636f 6e73 6f6c 652e 7265 6e64 6572  = console.render
-0003f0e0: 5f73 7472 2822 5b62 6f6c 6420 7768 6974  _str("[bold whit
-0003f0f0: 655d 4545 4620 4461 7461 2045 7874 7261  e]EEF Data Extra
-0003f100: 6374 6f72 5b2f 626f 6c64 2077 6869 7465  ctor[/bold white
-0003f110: 5d22 290a 0a20 2020 2074 6f70 5f74 6974  ]")..    top_tit
-0003f120: 6c65 203d 2063 6f6e 736f 6c65 2e72 656e  le = console.ren
-0003f130: 6465 725f 7374 7228 225b 626f 6c64 2077  der_str("[bold w
-0003f140: 6869 7465 5d57 656c 636f 6d65 5b2f 626f  hite]Welcome[/bo
-0003f150: 6c64 2077 6869 7465 5d22 290a 2020 2020  ld white]").    
-0003f160: 7469 746c 6531 203d 2063 6f6e 736f 6c65  title1 = console
-0003f170: 2e72 656e 6465 725f 7374 7228 225b 626f  .render_str("[bo
-0003f180: 6c64 2077 6869 7465 5d4d 6169 6e20 4d65  ld white]Main Me
-0003f190: 6e75 5b2f 626f 6c64 2077 6869 7465 5d22  nu[/bold white]"
-0003f1a0: 290a 2020 2020 7469 746c 6532 203d 2063  ).    title2 = c
-0003f1b0: 6f6e 736f 6c65 2e72 656e 6465 725f 7374  onsole.render_st
-0003f1c0: 7228 225b 626f 6c64 2077 6869 7465 5d44  r("[bold white]D
-0003f1d0: 6174 6120 4669 6c65 2044 6574 6169 6c73  ata File Details
-0003f1e0: 5b2f 626f 6c64 2077 6869 7465 5d22 290a  [/bold white]").
-0003f1f0: 0a20 2020 2023 2053 6574 2074 6578 7420  .    # Set text 
-0003f200: 666f 7220 746f 7020 7061 6e65 6c20 6f66  for top panel of
-0003f210: 206d 6169 6e20 6d65 6e75 0a20 2020 2074   main menu.    t
-0003f220: 6f70 5f70 616e 656c 5f74 6578 7420 3d20  op_panel_text = 
-0003f230: 280a 2020 2020 2020 2020 225b 2346 4646  (.        "[#FFF
-0003f240: 4646 465d 5765 6c63 6f6d 6520 746f 2074  FFF]Welcome to t
-0003f250: 6865 2045 4546 2044 6174 6120 4578 7472  he EEF Data Extr
-0003f260: 6163 746f 722e 2055 7365 2074 6865 5b2f  actor. Use the[/
-0003f270: 2346 4646 4646 465d 2022 0a20 2020 2020  #FFFFFF] ".     
-0003f280: 2020 2022 5b62 6f6c 6420 2366 6335 3432     "[bold #fc542
-0003f290: 345d 4d61 696e 204d 656e 755b 2f62 6f6c  4]Main Menu[/bol
-0003f2a0: 6420 2366 6335 3432 345d 205b 2346 4646  d #fc5424] [#FFF
-0003f2b0: 4646 465d 746f 2067 656e 6572 6174 6520  FFF]to generate 
-0003f2c0: 7661 7269 6f75 7320 6461 7461 6672 616d  various datafram
-0003f2d0: 6573 2063 6f6e 7461 696e 696e 6720 6461  es containing da
-0003f2e0: 7461 2065 7874 7261 6374 6564 2022 0a20  ta extracted ". 
-0003f2f0: 2020 2020 2020 2022 6672 6f6d 2061 6e20         "from an 
-0003f300: 696e 7075 7420 5b62 6f6c 6420 2366 6335  input [bold #fc5
-0003f310: 3432 345d 4a53 4f4e 5b2f 626f 6c64 2023  424]JSON[/bold #
-0003f320: 6663 3534 3234 5d20 5b23 4646 4646 4646  fc5424] [#FFFFFF
-0003f330: 5d64 6174 6166 696c 6520 7072 6f64 7563  ]datafile produc
-0003f340: 6564 2062 7920 7468 6520 4545 4620 4564  ed by the EEF Ed
-0003f350: 7563 6174 696f 6e20 4576 6964 656e 6365  ucation Evidence
-0003f360: 2022 0a20 2020 2020 2020 2022 4461 7461   ".        "Data
-0003f370: 6261 7365 2e5c 6e5c 6e5b 626f 6c64 2023  base.\n\n[bold #
-0003f380: 6663 3534 3234 5d4f 7074 696f 6e73 2031  fc5424]Options 1
-0003f390: 2d35 5b2f 626f 6c64 2023 6663 3534 3234  -5[/bold #fc5424
-0003f3a0: 5d20 5b23 4646 4646 4646 5d69 6e63 6c75  ] [#FFFFFF]inclu
-0003f3b0: 6465 206f 7572 206f 776e 2063 7573 746f  de our own custo
-0003f3c0: 6d20 6461 7461 6672 616d 6573 2022 0a20  m dataframes ". 
-0003f3d0: 2020 2020 2020 2022 666f 7220 6461 7461         "for data
-0003f3e0: 2063 6c65 616e 696e 6720 7072 696f 7220   cleaning prior 
-0003f3f0: 746f 2061 6e61 6c79 7369 732e 5b2f 2346  to analysis.[/#F
-0003f400: 4646 4646 465d 205b 626f 6c64 2023 6663  FFFFF] [bold #fc
-0003f410: 3534 3234 5d4f 7074 696f 6e20 365b 2f62  5424]Option 6[/b
-0003f420: 6f6c 6420 2366 6335 3432 345d 205b 2346  old #fc5424] [#F
-0003f430: 4646 4646 465d 6765 6e65 7261 7465 7320  FFFFF]generates 
-0003f440: 7468 6520 220a 2020 2020 2020 2020 2266  the ".        "f
-0003f450: 696e 616c 2064 6174 6166 7261 6d65 2873  inal dataframe(s
-0003f460: 2920 7573 6564 2069 6e20 6f75 7220 6d65  ) used in our me
-0003f470: 7461 2d61 6e61 6c79 7365 732e 205b 626f  ta-analyses. [bo
-0003f480: 6c64 2023 6663 3534 3234 5d4f 7074 696f  ld #fc5424]Optio
-0003f490: 6e20 375b 2f62 6f6c 6420 2366 6335 3432  n 7[/bold #fc542
-0003f4a0: 345d 2070 726f 6475 6365 7320 7261 7720  4] produces raw 
-0003f4b0: 2875 6e6f 7264 6572 6564 2920 220a 2020  (unordered) ".  
-0003f4c0: 2020 2020 2020 226f 7574 636f 6d65 2064        "outcome d
-0003f4d0: 6174 612e 205b 626f 6c64 2023 6663 3534  ata. [bold #fc54
-0003f4e0: 3234 5d4f 7074 696f 6e20 385b 2f62 6f6c  24]Option 8[/bol
-0003f4f0: 6420 2366 6335 3432 345d 2070 726f 6475  d #fc5424] produ
-0003f500: 6365 7320 6120 6265 7370 6f6b 6520 7374  ces a bespoke st
-0003f510: 7564 7920 7365 6375 7269 7479 2064 6174  udy security dat
-0003f520: 6166 7261 6d65 2e20 220a 2020 2020 2020  aframe. ".      
-0003f530: 2020 225b 2f23 4646 4646 4646 5d5b 626f    "[/#FFFFFF][bo
-0003f540: 6c64 2023 6663 3534 3234 5d4f 7074 696f  ld #fc5424]Optio
-0003f550: 6e20 395b 2f62 6f6c 6420 2366 6335 3432  n 9[/bold #fc542
-0003f560: 345d 2070 726f 6475 6365 7320 6120 7374  4] produces a st
-0003f570: 7261 6e64 2d6c 6576 656c 2027 7061 646c  rand-level 'padl
-0003f580: 6f63 6b73 2720 6461 7461 6672 616d 652e  ocks' dataframe.
-0003f590: 205b 626f 6c64 2023 6663 3534 3234 5d4f   [bold #fc5424]O
-0003f5a0: 7074 696f 6e20 3130 5b2f 626f 6c64 2023  ption 10[/bold #
-0003f5b0: 6663 3534 3234 5d20 5b23 4646 4646 4646  fc5424] [#FFFFFF
-0003f5c0: 5d63 6f6d 7069 6c65 7320 220a 2020 2020  ]compiles ".    
-0003f5d0: 2020 2020 2274 6865 206e 6563 6573 7361      "the necessa
-0003f5e0: 7279 2064 6174 6120 666f 7220 636f 6e73  ry data for cons
-0003f5f0: 7472 7563 7469 6e67 2073 7475 6479 2072  tructing study r
-0003f600: 6566 6572 656e 6365 732e 2046 696e 616c  eferences. Final
-0003f610: 6c79 2c20 5b2f 2346 4646 4646 465d 5b62  ly, [/#FFFFFF][b
-0003f620: 6f6c 6420 2366 6335 3432 345d 4f70 7469  old #fc5424]Opti
-0003f630: 6f6e 2031 315b 2f62 6f6c 6420 2366 6335  on 11[/bold #fc5
-0003f640: 3432 345d 2022 0a20 2020 2020 2020 2022  424] ".        "
-0003f650: 5b23 4646 4646 4646 5d61 6c6c 6f77 7320  [#FFFFFF]allows 
-0003f660: 796f 7520 746f 2063 7265 6174 6520 796f  you to create yo
-0003f670: 7572 206f 776e 2063 7573 746f 6d20 7661  ur own custom va
-0003f680: 7269 6162 6c65 2064 6174 6166 7261 6d65  riable dataframe
-0003f690: 2e5b 2f23 4646 4646 4646 5d22 0a20 2020  .[/#FFFFFF]".   
-0003f6a0: 2029 0a20 2020 2074 6f70 5f6d 656e 755f   ).    top_menu_
-0003f6b0: 7374 796c 6520 3d20 5374 796c 6528 6267  style = Style(bg
-0003f6c0: 636f 6c6f 723d 4752 4559 290a 0a20 2020  color=GREY)..   
-0003f6d0: 2023 2063 7265 6174 6520 7468 6520 7061   # create the pa
-0003f6e0: 6e65 6c20 7769 7468 2074 6865 2074 6578  nel with the tex
-0003f6f0: 740a 2020 2020 746f 705f 7061 6e65 6c20  t.    top_panel 
-0003f700: 3d20 5061 6e65 6c28 0a20 2020 2020 2020  = Panel(.       
-0003f710: 2074 6f70 5f70 616e 656c 5f74 6578 742c   top_panel_text,
-0003f720: 0a20 2020 2020 2020 2074 6974 6c65 3d74  .        title=t
-0003f730: 6f70 5f74 6974 6c65 2c20 0a20 2020 2020  op_title, .     
-0003f740: 2020 2062 6f72 6465 725f 7374 796c 653d     border_style=
-0003f750: 2262 6f6c 6420 7768 6974 6522 2c0a 2020  "bold white",.  
-0003f760: 2020 2020 2020 7469 746c 655f 616c 6967        title_alig
-0003f770: 6e3d 226c 6566 7422 2c0a 2020 2020 2020  n="left",.      
-0003f780: 2020 7374 796c 653d 746f 705f 6d65 6e75    style=top_menu
-0003f790: 5f73 7479 6c65 2c0a 2020 2020 2020 2020  _style,.        
-0003f7a0: 7061 6464 696e 673d 2831 2c20 3229 2c0a  padding=(1, 2),.
-0003f7b0: 2020 2020 2020 2020 7769 6474 683d 3132          width=12
-0003f7c0: 302c 0a20 2020 2029 0a0a 2020 2020 7061  0,.    )..    pa
-0003f7d0: 6e65 6c31 203d 2050 616e 656c 2e66 6974  nel1 = Panel.fit
-0003f7e0: 280a 2020 2020 2020 2020 6d61 696e 5f6d  (.        main_m
-0003f7f0: 656e 755f 7461 626c 652c 0a20 2020 2020  enu_table,.     
-0003f800: 2020 2074 6974 6c65 3d74 6974 6c65 312c     title=title1,
-0003f810: 0a20 2020 2020 2020 2062 6f72 6465 725f  .        border_
-0003f820: 7374 796c 653d 2262 6f6c 6420 7768 6974  style="bold whit
-0003f830: 6522 2c0a 2020 2020 2020 2020 7374 796c  e",.        styl
-0003f840: 653d 6375 7374 6f6d 5f73 7479 6c65 5f6d  e=custom_style_m
-0003f850: 6169 6e2c 0a20 2020 2020 2020 2074 6974  ain,.        tit
-0003f860: 6c65 5f61 6c69 676e 3d22 6c65 6674 222c  le_align="left",
-0003f870: 0a20 2020 2020 2020 2070 6164 6469 6e67  .        padding
-0003f880: 3d28 312c 2032 292c 0a20 2020 2020 2020  =(1, 2),.       
-0003f890: 2077 6964 7468 3d31 3230 2c0a 2020 2020   width=120,.    
-0003f8a0: 290a 0a20 2020 2070 616e 656c 3220 3d20  )..    panel2 = 
-0003f8b0: 5061 6e65 6c2e 6669 7428 0a20 2020 2020  Panel.fit(.     
-0003f8c0: 2020 2064 6174 6166 696c 655f 696e 666f     datafile_info
-0003f8d0: 5f74 6162 6c65 2c0a 2020 2020 2020 2020  _table,.        
-0003f8e0: 7469 746c 653d 7469 746c 6532 2c0a 2020  title=title2,.  
-0003f8f0: 2020 2020 2020 626f 7264 6572 5f73 7479        border_sty
-0003f900: 6c65 3d22 626f 6c64 2077 6869 7465 222c  le="bold white",
-0003f910: 0a20 2020 2020 2020 2073 7479 6c65 3d63  .        style=c
-0003f920: 7573 746f 6d5f 7374 796c 655f 6669 6c65  ustom_style_file
-0003f930: 5f64 6574 6169 6c73 2c0a 2020 2020 2020  _details,.      
-0003f940: 2020 7469 746c 655f 616c 6967 6e3d 226c    title_align="l
-0003f950: 6566 7422 2c0a 2020 2020 2020 2020 7061  eft",.        pa
-0003f960: 6464 696e 673d 2831 2c20 3229 2c0a 2020  dding=(1, 2),.  
-0003f970: 2020 2020 2020 7769 6474 683d 3132 302c        width=120,
-0003f980: 0a20 2020 2029 0a0a 2020 2020 2320 636f  .    )..    # co
-0003f990: 6d62 696e 6520 7468 6520 7465 7874 2070  mbine the text p
-0003f9a0: 616e 656c 2061 6e64 2070 616e 656c 7320  anel and panels 
-0003f9b0: 696e 746f 2061 206e 6577 2063 6f6c 756d  into a new colum
-0003f9c0: 6e0a 2020 2020 636f 6c75 6d6e 5f63 6f6d  n.    column_com
-0003f9d0: 6269 6e65 6420 3d20 436f 6c75 6d6e 7328  bined = Columns(
-0003f9e0: 5b74 6f70 5f70 616e 656c 2c20 7061 6e65  [top_panel, pane
-0003f9f0: 6c31 2c20 7061 6e65 6c32 5d2c 2065 7175  l1, panel2], equ
-0003fa00: 616c 3d46 616c 7365 290a 0a20 2020 2023  al=False)..    #
-0003fa10: 2063 7265 6174 6520 7468 6520 6c61 796f   create the layo
-0003fa20: 7574 2077 6974 6820 7468 6520 636f 6d62  ut with the comb
-0003fa30: 696e 6564 2063 6f6c 756d 6e0a 2020 2020  ined column.    
-0003fa40: 6c61 796f 7574 203d 204c 6179 6f75 7428  layout = Layout(
-0003fa50: 636f 6c75 6d6e 5f63 6f6d 6269 6e65 6429  column_combined)
-0003fa60: 0a0a 2020 2020 7061 6e65 6c20 3d20 5061  ..    panel = Pa
-0003fa70: 6e65 6c28 0a20 2020 2020 2020 206c 6179  nel(.        lay
-0003fa80: 6f75 742c 0a20 2020 2020 2020 2074 6974  out,.        tit
-0003fa90: 6c65 3d63 6f6e 7461 696e 6572 5f74 6974  le=container_tit
-0003faa0: 6c65 2c0a 2020 2020 2020 2020 626f 7264  le,.        bord
-0003fab0: 6572 5f73 7479 6c65 3d22 626f 6c64 2077  er_style="bold w
-0003fac0: 6869 7465 222c 0a20 2020 2020 2020 2070  hite",.        p
-0003fad0: 6164 6469 6e67 3d28 312c 2032 292c 0a20  adding=(1, 2),. 
-0003fae0: 2020 2020 2020 2074 6974 6c65 5f61 6c69         title_ali
-0003faf0: 676e 3d22 6365 6e74 6572 222c 0a20 2020  gn="center",.   
-0003fb00: 2020 2020 2073 7479 6c65 3d63 7573 746f       style=custo
-0003fb10: 6d5f 7374 796c 655f 6d61 696e 2c0a 2020  m_style_main,.  
-0003fb20: 2020 2020 2020 6865 6967 6874 3d34 362c        height=46,
-0003fb30: 0a20 2020 2020 2020 2077 6964 7468 3d31  .        width=1
-0003fb40: 3230 2c0a 2020 2020 290a 0a20 2020 2063  20,.    )..    c
-0003fb50: 6f6e 736f 6c65 2e63 6c65 6172 2829 0a20  onsole.clear(). 
-0003fb60: 2020 2063 6f6e 736f 6c65 2e70 7269 6e74     console.print
-0003fb70: 2870 616e 656c 290a 2020 2020 7072 696e  (panel).    prin
-0003fb80: 7428 225c 6e22 290a 0a0a 6465 6620 6d61  t("\n")...def ma
-0003fb90: 696e 5f6d 656e 755f 6469 7370 6c61 7931  in_menu_display1
-0003fba0: 2866 756e 6374 696f 6e73 2c20 6f75 7466  (functions, outf
-0003fbb0: 696c 6531 2c20 6466 5f64 6973 706c 6179  ile1, df_display
-0003fbc0: 293a 0a0a 2020 2020 636f 6e73 6f6c 6520  ):..    console 
-0003fbd0: 3d20 436f 6e73 6f6c 6528 290a 2020 2020  = Console().    
-0003fbe0: 6f75 7470 7574 5f66 696c 655f 696e 666f  output_file_info
-0003fbf0: 203d 2064 665f 6469 7370 6c61 7928 6675   = df_display(fu
-0003fc00: 6e63 7469 6f6e 732c 206f 7574 6669 6c65  nctions, outfile
-0003fc10: 3129 0a20 2020 206d 6169 6e5f 6d65 6e75  1).    main_menu
-0003fc20: 5f74 6162 6c65 203d 2064 6973 706c 6179  _table = display
-0003fc30: 5f6d 6169 6e5f 6d65 6e75 2829 0a20 2020  _main_menu().   
-0003fc40: 2064 6174 6166 696c 655f 696e 666f 5f74   datafile_info_t
-0003fc50: 6162 6c65 203d 2069 6e70 7574 5f66 696c  able = input_fil
-0003fc60: 655f 696e 666f 5f64 6973 706c 6179 2864  e_info_display(d
-0003fc70: 6174 615f 6669 6c65 290a 0a20 2020 2063  ata_file)..    c
-0003fc80: 7573 746f 6d5f 7374 796c 655f 6d61 696e  ustom_style_main
-0003fc90: 203d 2053 7479 6c65 2862 6763 6f6c 6f72   = Style(bgcolor
-0003fca0: 3d47 5245 5929 0a20 2020 2063 7573 746f  =GREY).    custo
-0003fcb0: 6d5f 7374 796c 655f 6669 6c65 5f64 6574  m_style_file_det
-0003fcc0: 6169 6c73 203d 2053 7479 6c65 2862 6763  ails = Style(bgc
-0003fcd0: 6f6c 6f72 3d47 5245 5929 0a20 2020 2063  olor=GREY).    c
-0003fce0: 7573 746f 6d5f 7374 796c 655f 636c 6561  ustom_style_clea
-0003fcf0: 6e69 6e67 5f69 6e66 6f20 3d20 5374 796c  ning_info = Styl
-0003fd00: 6528 6267 636f 6c6f 723d 4752 4559 290a  e(bgcolor=GREY).
-0003fd10: 0a20 2020 2074 6974 6c65 3120 3d20 636f  .    title1 = co
-0003fd20: 6e73 6f6c 652e 7265 6e64 6572 5f73 7472  nsole.render_str
-0003fd30: 2822 5b62 6f6c 6420 7768 6974 655d 4d61  ("[bold white]Ma
-0003fd40: 696e 204d 656e 755b 2f62 6f6c 6420 7768  in Menu[/bold wh
-0003fd50: 6974 655d 2229 0a20 2020 2074 6974 6c65  ite]").    title
-0003fd60: 3220 3d20 636f 6e73 6f6c 652e 7265 6e64  2 = console.rend
-0003fd70: 6572 5f73 7472 2822 5b62 6f6c 6420 7768  er_str("[bold wh
-0003fd80: 6974 655d 4461 7461 2046 696c 6520 4465  ite]Data File De
-0003fd90: 7461 696c 735b 2f62 6f6c 6420 7768 6974  tails[/bold whit
-0003fda0: 655d 2229 0a20 2020 2074 6974 6c65 3320  e]").    title3 
-0003fdb0: 3d20 636f 6e73 6f6c 652e 7265 6e64 6572  = console.render
-0003fdc0: 5f73 7472 2822 5b62 6f6c 6420 7768 6974  _str("[bold whit
-0003fdd0: 655d 4f75 7470 7574 2046 696c 6573 5b2f  e]Output Files[/
-0003fde0: 626f 6c64 2077 6869 7465 5d22 290a 0a20  bold white]").. 
-0003fdf0: 2020 2070 616e 656c 3161 203d 2050 616e     panel1a = Pan
-0003fe00: 656c 2e66 6974 280a 2020 2020 2020 2020  el.fit(.        
-0003fe10: 6d61 696e 5f6d 656e 755f 7461 626c 652c  main_menu_table,
-0003fe20: 0a20 2020 2020 2020 2074 6974 6c65 3d74  .        title=t
-0003fe30: 6974 6c65 312c 0a20 2020 2020 2020 2062  itle1,.        b
-0003fe40: 6f72 6465 725f 7374 796c 653d 2262 6f6c  order_style="bol
-0003fe50: 6420 7768 6974 6522 2c0a 2020 2020 2020  d white",.      
-0003fe60: 2020 7374 796c 653d 6375 7374 6f6d 5f73    style=custom_s
-0003fe70: 7479 6c65 5f6d 6169 6e2c 0a20 2020 2020  tyle_main,.     
-0003fe80: 2020 2074 6974 6c65 5f61 6c69 676e 3d22     title_align="
-0003fe90: 6c65 6674 222c 0a20 2020 2020 2020 2070  left",.        p
-0003fea0: 6164 6469 6e67 3d28 312c 2032 292c 0a20  adding=(1, 2),. 
-0003feb0: 2020 2029 0a20 2020 2070 616e 656c 3162     ).    panel1b
-0003fec0: 203d 2050 616e 656c 2e66 6974 280a 2020   = Panel.fit(.  
-0003fed0: 2020 2020 2020 6461 7461 6669 6c65 5f69        datafile_i
-0003fee0: 6e66 6f5f 7461 626c 652c 0a20 2020 2020  nfo_table,.     
-0003fef0: 2020 2074 6974 6c65 3d74 6974 6c65 322c     title=title2,
-0003ff00: 0a20 2020 2020 2020 2062 6f72 6465 725f  .        border_
-0003ff10: 7374 796c 653d 2262 6f6c 6420 7768 6974  style="bold whit
-0003ff20: 6522 2c0a 2020 2020 2020 2020 7374 796c  e",.        styl
-0003ff30: 653d 6375 7374 6f6d 5f73 7479 6c65 5f66  e=custom_style_f
-0003ff40: 696c 655f 6465 7461 696c 732c 0a20 2020  ile_details,.   
-0003ff50: 2020 2020 2074 6974 6c65 5f61 6c69 676e       title_align
-0003ff60: 3d22 6c65 6674 222c 0a20 2020 2020 2020  ="left",.       
-0003ff70: 2070 6164 6469 6e67 3d28 312c 2032 292c   padding=(1, 2),
-0003ff80: 0a20 2020 2029 0a0a 2020 2020 7061 6e65  .    )..    pane
-0003ff90: 6c32 203d 2050 616e 656c 2e66 6974 280a  l2 = Panel.fit(.
-0003ffa0: 2020 2020 2020 2020 6f75 7470 7574 5f66          output_f
-0003ffb0: 696c 655f 696e 666f 2c0a 2020 2020 2020  ile_info,.      
-0003ffc0: 2020 7469 746c 653d 7469 746c 6533 2c0a    title=title3,.
-0003ffd0: 2020 2020 2020 2020 626f 7264 6572 5f73          border_s
-0003ffe0: 7479 6c65 3d22 626f 6c64 2077 6869 7465  tyle="bold white
-0003fff0: 222c 0a20 2020 2020 2020 2073 7479 6c65  ",.        style
-00040000: 3d63 7573 746f 6d5f 7374 796c 655f 636c  =custom_style_cl
-00040010: 6561 6e69 6e67 5f69 6e66 6f2c 0a20 2020  eaning_info,.   
-00040020: 2020 2020 2074 6974 6c65 5f61 6c69 676e       title_align
-00040030: 3d22 6c65 6674 222c 0a20 2020 2020 2020  ="left",.       
-00040040: 2070 6164 6469 6e67 3d28 312c 2032 292c   padding=(1, 2),
-00040050: 0a20 2020 2029 0a20 2020 2023 2063 7265  .    ).    # cre
-00040060: 6174 6520 7468 6520 6669 7273 7420 726f  ate the first ro
-00040070: 7720 6f66 2063 6f6c 756d 6e73 0a20 2020  w of columns.   
-00040080: 2072 6f77 3120 3d20 436f 6c75 6d6e 7328   row1 = Columns(
-00040090: 5b70 616e 656c 3161 5d2c 2065 7175 616c  [panel1a], equal
-000400a0: 3d46 616c 7365 290a 0a20 2020 2072 6f77  =False)..    row
-000400b0: 3162 203d 2043 6f6c 756d 6e73 285b 7061  1b = Columns([pa
-000400c0: 6e65 6c31 625d 2c20 6571 7561 6c3d 4661  nel1b], equal=Fa
-000400d0: 6c73 6529 0a0a 2020 2020 2320 6372 6561  lse)..    # crea
-000400e0: 7465 2074 6865 2073 6563 6f6e 6420 726f  te the second ro
-000400f0: 7720 6f66 2063 6f6c 756d 6e73 0a20 2020  w of columns.   
-00040100: 2072 6f77 3220 3d20 436f 6c75 6d6e 7328   row2 = Columns(
-00040110: 5b70 616e 656c 325d 2c20 6571 7561 6c3d  [panel2], equal=
-00040120: 4661 6c73 6529 0a0a 2020 2020 2320 6372  False)..    # cr
-00040130: 6561 7465 2074 6865 206c 6179 6f75 7420  eate the layout 
-00040140: 7769 7468 2074 6865 2070 616e 656c 730a  with the panels.
-00040150: 2020 2020 6c61 796f 7574 203d 2043 6f6c      layout = Col
-00040160: 756d 6e73 285b 726f 7731 2c20 726f 7731  umns([row1, row1
-00040170: 622c 2072 6f77 325d 2c20 6571 7561 6c3d  b, row2], equal=
-00040180: 4661 6c73 6529 0a0a 2020 2020 7061 6e65  False)..    pane
-00040190: 6c20 3d20 5061 6e65 6c28 0a20 2020 2020  l = Panel(.     
-000401a0: 2020 206c 6179 6f75 742c 200a 2020 2020     layout, .    
-000401b0: 2020 2020 7469 746c 653d 2245 4546 2054      title="EEF T
-000401c0: 6561 6368 696e 6720 616e 6420 4c65 6172  eaching and Lear
-000401d0: 6e69 6e67 2054 6f6f 6c6b 6974 2044 6174  ning Toolkit Dat
-000401e0: 6120 4578 7472 6163 746f 7222 2c20 0a20  a Extractor", . 
-000401f0: 2020 2020 2020 2062 6f72 6465 725f 7374         border_st
-00040200: 796c 653d 2262 6f6c 6420 7768 6974 6522  yle="bold white"
-00040210: 2c20 0a20 2020 2020 2020 2070 6164 6469  , .        paddi
-00040220: 6e67 3d28 312c 2032 292c 200a 2020 2020  ng=(1, 2), .    
-00040230: 2020 2020 7469 746c 655f 616c 6967 6e3d      title_align=
-00040240: 226c 6566 7422 2c0a 2020 2020 2020 2020  "left",.        
-00040250: 7374 796c 653d 6375 7374 6f6d 5f73 7479  style=custom_sty
-00040260: 6c65 5f6d 6169 6e2c 0a20 2020 2020 2020  le_main,.       
-00040270: 2077 6964 7468 3d31 3230 2c0a 2020 2020   width=120,.    
-00040280: 2020 2020 6865 6967 6874 3d34 3429 0a0a      height=44)..
-00040290: 2020 2020 636f 6e73 6f6c 652e 636c 6561      console.clea
-000402a0: 7228 290a 2020 2020 636f 6e73 6f6c 652e  r().    console.
-000402b0: 7072 696e 7428 7061 6e65 6c29 0a20 2020  print(panel).   
-000402c0: 2070 7269 6e74 2822 5c6e 2229 0a0a 7061   print("\n")..pa
-000402d0: 7468 5f63 6f6d 706c 6574 6572 203d 2050  th_completer = P
-000402e0: 6174 6843 6f6d 706c 6574 6572 2829 0a64  athCompleter().d
-000402f0: 6174 615f 6669 6c65 203d 2070 726f 6d70  ata_file = promp
-00040300: 7428 2753 656c 6563 7420 796f 7572 2064  t('Select your d
-00040310: 6174 6120 6669 6c65 3a20 272c 2063 6f6d  ata file: ', com
-00040320: 706c 6574 6572 3d70 6174 685f 636f 6d70  pleter=path_comp
-00040330: 6c65 7465 7229 0a6a 736f 6e5f 6578 7472  leter).json_extr
-00040340: 6163 746f 7220 3d20 4a53 4f4e 4461 7461  actor = JSONData
-00040350: 4578 7472 6163 746f 7228 6461 7461 5f66  Extractor(data_f
-00040360: 696c 6529                                ile)
+0003cd30: 2020 2020 2020 2062 6f78 3d62 6f78 2e53         box=box.S
+0003cd40: 494d 504c 4529 0a0a 2020 2020 7365 6c65  IMPLE)..    sele
+0003cd50: 6374 696f 6e5f 7374 796c 6520 3d20 5374  ction_style = St
+0003cd60: 796c 6528 6974 616c 6963 3d46 616c 7365  yle(italic=False
+0003cd70: 2c20 6267 636f 6c6f 723d 4752 4559 2c20  , bgcolor=GREY, 
+0003cd80: 636f 6c6f 723d 2223 6663 3534 3234 222c  color="#fc5424",
+0003cd90: 2062 6f6c 643d 5472 7565 290a 2020 2020   bold=True).    
+0003cda0: 6465 7363 7269 7074 696f 6e5f 7374 796c  description_styl
+0003cdb0: 6520 3d20 5374 796c 6528 6974 616c 6963  e = Style(italic
+0003cdc0: 3d46 616c 7365 2c20 6267 636f 6c6f 723d  =False, bgcolor=
+0003cdd0: 4752 4559 2c20 636f 6c6f 723d 2223 6663  GREY, color="#fc
+0003cde0: 3534 3234 222c 2062 6f6c 643d 5472 7565  5424", bold=True
+0003cdf0: 290a 0a20 2020 206d 6169 6e5f 7461 626c  )..    main_tabl
+0003ce00: 652e 6164 645f 636f 6c75 6d6e 2822 5365  e.add_column("Se
+0003ce10: 6c65 6374 696f 6e22 2c20 6865 6164 6572  lection", header
+0003ce20: 5f73 7479 6c65 3d73 656c 6563 7469 6f6e  _style=selection
+0003ce30: 5f73 7479 6c65 2c20 7374 796c 653d 636f  _style, style=co
+0003ce40: 6c75 6d6e 5f73 7479 6c65 290a 2020 2020  lumn_style).    
+0003ce50: 6d61 696e 5f74 6162 6c65 2e61 6464 5f63  main_table.add_c
+0003ce60: 6f6c 756d 6e28 2244 6573 6372 6970 7469  olumn("Descripti
+0003ce70: 6f6e 222c 2068 6561 6465 725f 7374 796c  on", header_styl
+0003ce80: 653d 6465 7363 7269 7074 696f 6e5f 7374  e=description_st
+0003ce90: 796c 652c 2073 7479 6c65 3d63 6f6c 756d  yle, style=colum
+0003cea0: 6e5f 7374 796c 6529 0a0a 2020 2020 6d61  n_style)..    ma
+0003ceb0: 696e 5f74 6162 6c65 2e61 6464 5f72 6f77  in_table.add_row
+0003cec0: 2822 2031 2e20 4461 7461 6672 616d 6520  (" 1. Dataframe 
+0003ced0: 3122 2c20 2020 2020 2022 5374 7564 792c  1",      "Study,
+0003cee0: 2052 6573 6561 7263 6820 2620 4465 7369   Research & Desi
+0003cef0: 676e 2056 6172 6961 626c 6573 2229 0a20  gn Variables"). 
+0003cf00: 2020 206d 6169 6e5f 7461 626c 652e 6164     main_table.ad
+0003cf10: 645f 726f 7728 2220 322e 2044 6174 6166  d_row(" 2. Dataf
+0003cf20: 7261 6d65 2032 222c 2020 2020 2020 2249  rame 2",      "I
+0003cf30: 6e74 6572 7665 6e74 696f 6e20 4465 7461  ntervention Deta
+0003cf40: 696c 7322 290a 2020 2020 6d61 696e 5f74  ils").    main_t
+0003cf50: 6162 6c65 2e61 6464 5f72 6f77 2822 2033  able.add_row(" 3
+0003cf60: 2e20 5361 6d70 6c65 2053 697a 6522 2c20  . Sample Size", 
+0003cf70: 2020 2020 2022 5361 6d70 6c65 2073 697a       "Sample siz
+0003cf80: 6520 7661 7269 6162 6c65 7322 290a 2020  e variables").  
+0003cf90: 2020 6d61 696e 5f74 6162 6c65 2e61 6464    main_table.add
+0003cfa0: 5f72 6f77 2822 2034 2e20 4566 6665 6374  _row(" 4. Effect
+0003cfb0: 2053 697a 6520 4122 2c20 2020 2022 4465   Size A",    "De
+0003cfc0: 7363 7269 7074 6976 6520 5374 6174 6973  scriptive Statis
+0003cfd0: 7469 6373 2229 0a20 2020 206d 6169 6e5f  tics").    main_
+0003cfe0: 7461 626c 652e 6164 645f 726f 7728 2220  table.add_row(" 
+0003cff0: 352e 2045 6666 6563 7420 5369 7a65 2042  5. Effect Size B
+0003d000: 222c 2020 2020 224f 7574 636f 6d65 2044  ",    "Outcome D
+0003d010: 6574 6169 6c73 2229 0a20 2020 206d 6169  etails").    mai
+0003d020: 6e5f 7461 626c 652e 6164 645f 726f 7728  n_table.add_row(
+0003d030: 2220 362e 2044 6174 6120 416e 616c 7973  " 6. Data Analys
+0003d040: 6973 222c 2020 2020 224b 6579 2076 6172  is",    "Key var
+0003d050: 6961 626c 6573 2066 6f72 2064 6174 6120  iables for data 
+0003d060: 616e 616c 7973 6973 2229 0a20 2020 206d  analysis").    m
+0003d070: 6169 6e5f 7461 626c 652e 6164 645f 726f  ain_table.add_ro
+0003d080: 7728 2220 372e 204f 7574 636f 6d65 2044  w(" 7. Outcome D
+0003d090: 6174 6122 2c20 2020 2020 2252 6177 206f  ata",     "Raw o
+0003d0a0: 7574 636f 6d65 2064 6174 6122 290a 2020  utcome data").  
+0003d0b0: 2020 6d61 696e 5f74 6162 6c65 2e61 6464    main_table.add
+0003d0c0: 5f72 6f77 2822 2038 2e20 5374 7564 7920  _row(" 8. Study 
+0003d0d0: 5365 6375 7269 7479 222c 2020 2020 2022  Security",     "
+0003d0e0: 5374 7564 7920 5365 6375 7269 7479 2063  Study Security c
+0003d0f0: 616c 6375 6c61 7469 6f6e 7322 290a 2020  alculations").  
+0003d100: 2020 6d61 696e 5f74 6162 6c65 2e61 6464    main_table.add
+0003d110: 5f72 6f77 2822 2039 2e20 5061 646c 6f63  _row(" 9. Padloc
+0003d120: 6b73 222c 2020 2020 2020 2022 5374 7261  ks",       "Stra
+0003d130: 6e64 206c 6576 656c 2070 6164 6c6f 636b  nd level padlock
+0003d140: 2064 6174 6122 290a 2020 2020 6d61 696e   data").    main
+0003d150: 5f74 6162 6c65 2e61 6464 5f72 6f77 2822  _table.add_row("
+0003d160: 3130 2e20 5265 6665 7265 6e63 6573 222c  10. References",
+0003d170: 2020 2020 2022 4461 7461 2066 6f72 2063       "Data for c
+0003d180: 6f6e 7374 7275 6374 696e 6720 7374 7564  onstructing stud
+0003d190: 7920 7265 6665 7265 6e63 6573 2229 0a20  y references"). 
+0003d1a0: 2020 206d 6169 6e5f 7461 626c 652e 6164     main_table.ad
+0003d1b0: 645f 726f 7728 2231 312e 2043 6f6c 756d  d_row("11. Colum
+0003d1c0: 6e20 5365 6c65 6374 696f 6e22 2c20 2243  n Selection", "C
+0003d1d0: 7573 746f 6d20 636f 6c75 6d6e 2073 656c  ustom column sel
+0003d1e0: 6563 7469 6f6e 2229 0a20 2020 206d 6169  ection").    mai
+0003d1f0: 6e5f 7461 626c 652e 6164 645f 726f 7728  n_table.add_row(
+0003d200: 2231 322e 2053 7475 6479 2053 656c 6563  "12. Study Selec
+0003d210: 7469 6f6e 222c 2022 4375 7374 6f6d 2049  tion", "Custom I
+0003d220: 4420 7365 6c65 6374 696f 6e22 290a 0a20  D selection").. 
+0003d230: 2020 206d 6169 6e5f 7461 626c 652e 6164     main_table.ad
+0003d240: 645f 726f 7728 2222 2c20 2222 290a 0a20  d_row("", "").. 
+0003d250: 2020 206d 6169 6e5f 7461 626c 652e 6164     main_table.ad
+0003d260: 645f 726f 7728 2220 302e 2045 5849 5422  d_row(" 0. EXIT"
+0003d270: 2c20 2222 290a 2020 2020 7265 7475 726e  , "").    return
+0003d280: 206d 6169 6e5f 7461 626c 650a 0a0a 6465   main_table...de
+0003d290: 6620 6461 7461 6672 616d 655f 315f 6f75  f dataframe_1_ou
+0003d2a0: 7470 7574 5f64 6973 706c 6179 2866 756e  tput_display(fun
+0003d2b0: 6374 696f 6e73 2c20 6f75 7466 696c 6529  ctions, outfile)
+0003d2c0: 3a0a 2020 2020 636f 6e73 6f6c 6520 3d20  :.    console = 
+0003d2d0: 436f 6e73 6f6c 6528 290a 2020 2020 6375  Console().    cu
+0003d2e0: 7374 6f6d 5f73 7479 6c65 5f64 6631 203d  stom_style_df1 =
+0003d2f0: 2053 7479 6c65 2862 6763 6f6c 6f72 3d47   Style(bgcolor=G
+0003d300: 5245 5929 0a0a 2020 2020 6466 315f 7461  REY)..    df1_ta
+0003d310: 626c 6520 3d20 5461 626c 6528 7368 6f77  ble = Table(show
+0003d320: 5f68 6561 6465 723d 5472 7565 2c20 0a20  _header=True, . 
+0003d330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003d340: 2020 2020 2073 7479 6c65 3d63 7573 746f       style=custo
+0003d350: 6d5f 7374 796c 655f 6466 312c 0a20 2020  m_style_df1,.   
+0003d360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003d370: 2020 2074 6974 6c65 3d4e 6f6e 652c 0a20     title=None,. 
+0003d380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003d390: 2020 2020 2073 6166 655f 626f 783d 4661       safe_box=Fa
+0003d3a0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+0003d3b0: 2020 2020 2020 2020 2020 2062 6f78 3d62             box=b
+0003d3c0: 6f78 2e53 494d 504c 4529 0a0a 2020 2020  ox.SIMPLE)..    
+0003d3d0: 6466 315f 7461 626c 652e 6164 645f 636f  df1_table.add_co
+0003d3e0: 6c75 6d6e 2822 5365 6c65 6374 696f 6e22  lumn("Selection"
+0003d3f0: 2c20 6a75 7374 6966 793d 2263 656e 7465  , justify="cente
+0003d400: 7222 2c20 6865 6164 6572 5f73 7479 6c65  r", header_style
+0003d410: 3d22 2366 6335 3432 3422 290a 2020 2020  ="#fc5424").    
+0003d420: 6466 315f 7461 626c 652e 6164 645f 636f  df1_table.add_co
+0003d430: 6c75 6d6e 2822 4f75 7470 7574 2064 6972  lumn("Output dir
+0003d440: 6563 746f 7279 222c 206a 7573 7469 6679  ectory", justify
+0003d450: 3d22 6c65 6674 222c 2068 6561 6465 725f  ="left", header_
+0003d460: 7374 796c 653d 2223 6663 3534 3234 2229  style="#fc5424")
+0003d470: 0a20 2020 2064 6631 5f74 6162 6c65 2e61  .    df1_table.a
+0003d480: 6464 5f72 6f77 2822 4461 7461 6672 616d  dd_row("Datafram
+0003d490: 6520 3122 2c20 6f75 7466 696c 652c 2073  e 1", outfile, s
+0003d4a0: 7479 6c65 3d57 4849 5445 290a 0a20 2020  tyle=WHITE)..   
+0003d4b0: 2072 6574 7572 6e20 6466 315f 7461 626c   return df1_tabl
+0003d4c0: 650a 0a0a 6465 6620 6461 7461 6672 616d  e...def datafram
+0003d4d0: 655f 325f 6f75 7470 7574 5f64 6973 706c  e_2_output_displ
+0003d4e0: 6179 2866 756e 6374 696f 6e73 2c20 6f75  ay(functions, ou
+0003d4f0: 7466 696c 6529 3a0a 2020 2020 636f 6e73  tfile):.    cons
+0003d500: 6f6c 6520 3d20 436f 6e73 6f6c 6528 290a  ole = Console().
+0003d510: 2020 2020 6375 7374 6f6d 5f73 7479 6c65      custom_style
+0003d520: 5f64 6631 203d 2053 7479 6c65 2862 6763  _df1 = Style(bgc
+0003d530: 6f6c 6f72 3d47 5245 5929 0a0a 2020 2020  olor=GREY)..    
+0003d540: 6466 325f 7461 626c 6520 3d20 5461 626c  df2_table = Tabl
+0003d550: 6528 7368 6f77 5f68 6561 6465 723d 5472  e(show_header=Tr
+0003d560: 7565 2c20 0a20 2020 2020 2020 2020 2020  ue, .           
+0003d570: 2020 2020 2020 2020 2020 2073 7479 6c65             style
+0003d580: 3d63 7573 746f 6d5f 7374 796c 655f 6466  =custom_style_df
+0003d590: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
+0003d5a0: 2020 2020 2020 2020 2074 6974 6c65 3d4e           title=N
+0003d5b0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+0003d5c0: 2020 2020 2020 2020 2020 2073 6166 655f             safe_
+0003d5d0: 626f 783d 4661 6c73 652c 0a20 2020 2020  box=False,.     
+0003d5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003d5f0: 2062 6f78 3d62 6f78 2e53 494d 504c 4529   box=box.SIMPLE)
+0003d600: 0a0a 2020 2020 6466 325f 7461 626c 652e  ..    df2_table.
+0003d610: 6164 645f 636f 6c75 6d6e 2822 5365 6c65  add_column("Sele
+0003d620: 6374 696f 6e22 2c20 6a75 7374 6966 793d  ction", justify=
+0003d630: 2263 656e 7465 7222 2c20 6865 6164 6572  "center", header
+0003d640: 5f73 7479 6c65 3d22 2366 6335 3432 3422  _style="#fc5424"
+0003d650: 290a 2020 2020 6466 325f 7461 626c 652e  ).    df2_table.
+0003d660: 6164 645f 636f 6c75 6d6e 2822 4f75 7470  add_column("Outp
+0003d670: 7574 2064 6972 6563 746f 7279 222c 206a  ut directory", j
+0003d680: 7573 7469 6679 3d22 6c65 6674 222c 2068  ustify="left", h
+0003d690: 6561 6465 725f 7374 796c 653d 5748 4954  eader_style=WHIT
+0003d6a0: 4529 0a20 2020 2064 6632 5f74 6162 6c65  E).    df2_table
+0003d6b0: 2e61 6464 5f72 6f77 2822 4461 7461 6672  .add_row("Datafr
+0003d6c0: 616d 6520 3222 2c20 6f75 7466 696c 652c  ame 2", outfile,
+0003d6d0: 2073 7479 6c65 3d57 4849 5445 290a 0a20   style=WHITE).. 
+0003d6e0: 2020 2072 6574 7572 6e20 6466 325f 7461     return df2_ta
+0003d6f0: 626c 650a 0a0a 6465 6620 6461 7461 6672  ble...def datafr
+0003d700: 616d 655f 335f 6f75 7470 7574 5f64 6973  ame_3_output_dis
+0003d710: 706c 6179 2866 756e 6374 696f 6e73 2c20  play(functions, 
+0003d720: 6f75 7466 696c 6529 3a0a 2020 2020 636f  outfile):.    co
+0003d730: 6e73 6f6c 6520 3d20 436f 6e73 6f6c 6528  nsole = Console(
+0003d740: 290a 2020 2020 6375 7374 6f6d 5f73 7479  ).    custom_sty
+0003d750: 6c65 5f64 6631 203d 2053 7479 6c65 2862  le_df1 = Style(b
+0003d760: 6763 6f6c 6f72 3d47 5245 5929 0a0a 2020  gcolor=GREY)..  
+0003d770: 2020 6466 335f 7461 626c 6520 3d20 5461    df3_table = Ta
+0003d780: 626c 6528 7368 6f77 5f68 6561 6465 723d  ble(show_header=
+0003d790: 5472 7565 2c20 0a20 2020 2020 2020 2020  True, .         
+0003d7a0: 2020 2020 2020 2020 2020 2020 2073 7479               sty
+0003d7b0: 6c65 3d63 7573 746f 6d5f 7374 796c 655f  le=custom_style_
+0003d7c0: 6466 312c 0a20 2020 2020 2020 2020 2020  df1,.           
+0003d7d0: 2020 2020 2020 2020 2020 2074 6974 6c65             title
+0003d7e0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+0003d7f0: 2020 2020 2020 2020 2020 2020 2073 6166               saf
+0003d800: 655f 626f 783d 4661 6c73 652c 0a20 2020  e_box=False,.   
+0003d810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003d820: 2020 2062 6f78 3d62 6f78 2e53 494d 504c     box=box.SIMPL
+0003d830: 4529 0a0a 2020 2020 6466 335f 7461 626c  E)..    df3_tabl
+0003d840: 652e 6164 645f 636f 6c75 6d6e 2822 5365  e.add_column("Se
+0003d850: 6c65 6374 696f 6e22 2c20 6a75 7374 6966  lection", justif
+0003d860: 793d 2263 656e 7465 7222 2c20 6865 6164  y="center", head
+0003d870: 6572 5f73 7479 6c65 3d22 2366 6335 3432  er_style="#fc542
+0003d880: 3422 290a 2020 2020 6466 335f 7461 626c  4").    df3_tabl
+0003d890: 652e 6164 645f 636f 6c75 6d6e 2822 4f75  e.add_column("Ou
+0003d8a0: 7470 7574 2064 6972 6563 746f 7279 222c  tput directory",
+0003d8b0: 206a 7573 7469 6679 3d22 6c65 6674 222c   justify="left",
+0003d8c0: 2068 6561 6465 725f 7374 796c 653d 5748   header_style=WH
+0003d8d0: 4954 4529 0a20 2020 2064 6633 5f74 6162  ITE).    df3_tab
+0003d8e0: 6c65 2e61 6464 5f72 6f77 2822 5361 6d70  le.add_row("Samp
+0003d8f0: 6c65 2053 697a 6522 2c20 6f75 7466 696c  le Size", outfil
+0003d900: 652c 2073 7479 6c65 3d57 4849 5445 290a  e, style=WHITE).
+0003d910: 0a20 2020 2072 6574 7572 6e20 6466 335f  .    return df3_
+0003d920: 7461 626c 650a 0a0a 6465 6620 6461 7461  table...def data
+0003d930: 6672 616d 655f 345f 6f75 7470 7574 5f64  frame_4_output_d
+0003d940: 6973 706c 6179 2866 756e 6374 696f 6e73  isplay(functions
+0003d950: 2c20 6f75 7466 696c 6529 3a0a 2020 2020  , outfile):.    
+0003d960: 636f 6e73 6f6c 6520 3d20 436f 6e73 6f6c  console = Consol
+0003d970: 6528 290a 2020 2020 6375 7374 6f6d 5f73  e().    custom_s
+0003d980: 7479 6c65 5f64 6631 203d 2053 7479 6c65  tyle_df1 = Style
+0003d990: 2862 6763 6f6c 6f72 3d47 5245 5929 0a0a  (bgcolor=GREY)..
+0003d9a0: 2020 2020 6466 345f 7461 626c 6520 3d20      df4_table = 
+0003d9b0: 5461 626c 6528 7368 6f77 5f68 6561 6465  Table(show_heade
+0003d9c0: 723d 5472 7565 2c20 0a20 2020 2020 2020  r=True, .       
+0003d9d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0003d9e0: 7479 6c65 3d63 7573 746f 6d5f 7374 796c  tyle=custom_styl
+0003d9f0: 655f 6466 312c 0a20 2020 2020 2020 2020  e_df1,.         
+0003da00: 2020 2020 2020 2020 2020 2020 2074 6974               tit
+0003da10: 6c65 3d4e 6f6e 652c 0a20 2020 2020 2020  le=None,.       
+0003da20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0003da30: 6166 655f 626f 783d 4661 6c73 652c 0a20  afe_box=False,. 
+0003da40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003da50: 2020 2020 2062 6f78 3d62 6f78 2e53 494d       box=box.SIM
+0003da60: 504c 4529 0a0a 2020 2020 6466 345f 7461  PLE)..    df4_ta
+0003da70: 626c 652e 6164 645f 636f 6c75 6d6e 2822  ble.add_column("
+0003da80: 5365 6c65 6374 696f 6e22 2c20 6a75 7374  Selection", just
+0003da90: 6966 793d 2263 656e 7465 7222 2c20 6865  ify="center", he
+0003daa0: 6164 6572 5f73 7479 6c65 3d22 2366 6335  ader_style="#fc5
+0003dab0: 3432 3422 290a 2020 2020 6466 345f 7461  424").    df4_ta
+0003dac0: 626c 652e 6164 645f 636f 6c75 6d6e 2822  ble.add_column("
+0003dad0: 4f75 7470 7574 2064 6972 6563 746f 7279  Output directory
+0003dae0: 222c 206a 7573 7469 6679 3d22 6c65 6674  ", justify="left
+0003daf0: 222c 2068 6561 6465 725f 7374 796c 653d  ", header_style=
+0003db00: 5748 4954 4529 0a20 2020 2064 6634 5f74  WHITE).    df4_t
+0003db10: 6162 6c65 2e61 6464 5f72 6f77 2822 4566  able.add_row("Ef
+0003db20: 6665 6374 2053 697a 6520 4122 2c20 6f75  fect Size A", ou
+0003db30: 7466 696c 652c 2073 7479 6c65 3d57 4849  tfile, style=WHI
+0003db40: 5445 290a 0a20 2020 2072 6574 7572 6e20  TE)..    return 
+0003db50: 6466 345f 7461 626c 650a 0a0a 6465 6620  df4_table...def 
+0003db60: 6461 7461 6672 616d 655f 355f 6f75 7470  dataframe_5_outp
+0003db70: 7574 5f64 6973 706c 6179 2866 756e 6374  ut_display(funct
+0003db80: 696f 6e73 2c20 6f75 7466 696c 6529 3a0a  ions, outfile):.
+0003db90: 2020 2020 636f 6e73 6f6c 6520 3d20 436f      console = Co
+0003dba0: 6e73 6f6c 6528 290a 2020 2020 6375 7374  nsole().    cust
+0003dbb0: 6f6d 5f73 7479 6c65 5f64 6631 203d 2053  om_style_df1 = S
+0003dbc0: 7479 6c65 2862 6763 6f6c 6f72 3d47 5245  tyle(bgcolor=GRE
+0003dbd0: 5929 0a0a 2020 2020 6466 355f 7461 626c  Y)..    df5_tabl
+0003dbe0: 6520 3d20 5461 626c 6528 7368 6f77 5f68  e = Table(show_h
+0003dbf0: 6561 6465 723d 5472 7565 2c20 0a20 2020  eader=True, .   
+0003dc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003dc10: 2020 2073 7479 6c65 3d63 7573 746f 6d5f     style=custom_
+0003dc20: 7374 796c 655f 6466 312c 0a20 2020 2020  style_df1,.     
+0003dc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003dc40: 2074 6974 6c65 3d4e 6f6e 652c 0a20 2020   title=None,.   
+0003dc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003dc60: 2020 2073 6166 655f 626f 783d 4661 6c73     safe_box=Fals
+0003dc70: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0003dc80: 2020 2020 2020 2020 2062 6f78 3d62 6f78           box=box
+0003dc90: 2e53 494d 504c 4529 0a0a 2020 2020 6466  .SIMPLE)..    df
+0003dca0: 355f 7461 626c 652e 6164 645f 636f 6c75  5_table.add_colu
+0003dcb0: 6d6e 2822 5365 6c65 6374 696f 6e22 2c20  mn("Selection", 
+0003dcc0: 6a75 7374 6966 793d 2263 656e 7465 7222  justify="center"
+0003dcd0: 2c20 6865 6164 6572 5f73 7479 6c65 3d22  , header_style="
+0003dce0: 2366 6335 3432 3422 290a 2020 2020 6466  #fc5424").    df
+0003dcf0: 355f 7461 626c 652e 6164 645f 636f 6c75  5_table.add_colu
+0003dd00: 6d6e 2822 4f75 7470 7574 2064 6972 6563  mn("Output direc
+0003dd10: 746f 7279 222c 206a 7573 7469 6679 3d22  tory", justify="
+0003dd20: 6c65 6674 222c 2068 6561 6465 725f 7374  left", header_st
+0003dd30: 796c 653d 5748 4954 4529 0a20 2020 2064  yle=WHITE).    d
+0003dd40: 6635 5f74 6162 6c65 2e61 6464 5f72 6f77  f5_table.add_row
+0003dd50: 2822 4566 6665 6374 2053 697a 6520 4222  ("Effect Size B"
+0003dd60: 2c20 6f75 7466 696c 652c 2073 7479 6c65  , outfile, style
+0003dd70: 3d57 4849 5445 290a 0a20 2020 2072 6574  =WHITE)..    ret
+0003dd80: 7572 6e20 6466 355f 7461 626c 650a 0a0a  urn df5_table...
+0003dd90: 6465 6620 6461 7461 6672 616d 655f 365f  def dataframe_6_
+0003dda0: 6f75 7470 7574 5f64 6973 706c 6179 2866  output_display(f
+0003ddb0: 756e 6374 696f 6e73 2c20 6f75 7466 696c  unctions, outfil
+0003ddc0: 6529 3a0a 2020 2020 636f 6e73 6f6c 6520  e):.    console 
+0003ddd0: 3d20 436f 6e73 6f6c 6528 290a 2020 2020  = Console().    
+0003dde0: 6375 7374 6f6d 5f73 7479 6c65 5f64 6631  custom_style_df1
+0003ddf0: 203d 2053 7479 6c65 2862 6763 6f6c 6f72   = Style(bgcolor
+0003de00: 3d47 5245 5929 0a0a 2020 2020 6466 365f  =GREY)..    df6_
+0003de10: 7461 626c 6520 3d20 5461 626c 6528 7368  table = Table(sh
+0003de20: 6f77 5f68 6561 6465 723d 5472 7565 2c20  ow_header=True, 
+0003de30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0003de40: 2020 2020 2020 2073 7479 6c65 3d63 7573         style=cus
+0003de50: 746f 6d5f 7374 796c 655f 6466 312c 0a20  tom_style_df1,. 
+0003de60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003de70: 2020 2020 2074 6974 6c65 3d4e 6f6e 652c       title=None,
+0003de80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0003de90: 2020 2020 2020 2073 6166 655f 626f 783d         safe_box=
+0003dea0: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
+0003deb0: 2020 2020 2020 2020 2020 2020 2062 6f78               box
+0003dec0: 3d62 6f78 2e53 494d 504c 4529 0a0a 2020  =box.SIMPLE)..  
+0003ded0: 2020 6466 365f 7461 626c 652e 6164 645f    df6_table.add_
+0003dee0: 636f 6c75 6d6e 2822 5365 6c65 6374 696f  column("Selectio
+0003def0: 6e22 2c20 6a75 7374 6966 793d 2263 656e  n", justify="cen
+0003df00: 7465 7222 2c20 6865 6164 6572 5f73 7479  ter", header_sty
+0003df10: 6c65 3d22 2366 6335 3432 3422 290a 2020  le="#fc5424").  
+0003df20: 2020 6466 365f 7461 626c 652e 6164 645f    df6_table.add_
+0003df30: 636f 6c75 6d6e 2822 4f75 7470 7574 2064  column("Output d
+0003df40: 6972 6563 746f 7279 222c 206a 7573 7469  irectory", justi
+0003df50: 6679 3d22 6c65 6674 222c 2068 6561 6465  fy="left", heade
+0003df60: 725f 7374 796c 653d 2223 6663 3534 3234  r_style="#fc5424
+0003df70: 2229 0a20 2020 2064 6636 5f74 6162 6c65  ").    df6_table
+0003df80: 2e61 6464 5f72 6f77 2822 4d61 696e 2041  .add_row("Main A
+0003df90: 6e61 6c79 7369 7322 2c20 6f75 7466 696c  nalysis", outfil
+0003dfa0: 652c 2073 7479 6c65 3d57 4849 5445 290a  e, style=WHITE).
+0003dfb0: 0a20 2020 2072 6574 7572 6e20 6466 365f  .    return df6_
+0003dfc0: 7461 626c 650a 0a0a 6465 6620 6461 7461  table...def data
+0003dfd0: 6672 616d 655f 375f 6f75 7470 7574 5f64  frame_7_output_d
+0003dfe0: 6973 706c 6179 2866 756e 6374 696f 6e73  isplay(functions
+0003dff0: 2c20 6f75 7466 696c 6529 3a0a 2020 2020  , outfile):.    
+0003e000: 636f 6e73 6f6c 6520 3d20 436f 6e73 6f6c  console = Consol
+0003e010: 6528 290a 2020 2020 6375 7374 6f6d 5f73  e().    custom_s
+0003e020: 7479 6c65 5f64 6631 203d 2053 7479 6c65  tyle_df1 = Style
+0003e030: 2862 6763 6f6c 6f72 3d47 5245 5929 0a0a  (bgcolor=GREY)..
+0003e040: 2020 2020 6466 375f 7461 626c 6520 3d20      df7_table = 
+0003e050: 5461 626c 6528 7368 6f77 5f68 6561 6465  Table(show_heade
+0003e060: 723d 5472 7565 2c20 0a20 2020 2020 2020  r=True, .       
+0003e070: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0003e080: 7479 6c65 3d63 7573 746f 6d5f 7374 796c  tyle=custom_styl
+0003e090: 655f 6466 312c 0a20 2020 2020 2020 2020  e_df1,.         
+0003e0a0: 2020 2020 2020 2020 2020 2020 2074 6974               tit
+0003e0b0: 6c65 3d4e 6f6e 652c 0a20 2020 2020 2020  le=None,.       
+0003e0c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0003e0d0: 6166 655f 626f 783d 4661 6c73 652c 0a20  afe_box=False,. 
+0003e0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003e0f0: 2020 2020 2062 6f78 3d62 6f78 2e53 494d       box=box.SIM
+0003e100: 504c 4529 0a0a 2020 2020 6466 375f 7461  PLE)..    df7_ta
+0003e110: 626c 652e 6164 645f 636f 6c75 6d6e 2822  ble.add_column("
+0003e120: 5365 6c65 6374 696f 6e22 2c20 6a75 7374  Selection", just
+0003e130: 6966 793d 2263 656e 7465 7222 2c20 6865  ify="center", he
+0003e140: 6164 6572 5f73 7479 6c65 3d22 2366 6335  ader_style="#fc5
+0003e150: 3432 3422 290a 2020 2020 6466 375f 7461  424").    df7_ta
+0003e160: 626c 652e 6164 645f 636f 6c75 6d6e 2822  ble.add_column("
+0003e170: 4f75 7470 7574 2064 6972 6563 746f 7279  Output directory
+0003e180: 222c 206a 7573 7469 6679 3d22 6c65 6674  ", justify="left
+0003e190: 222c 2068 6561 6465 725f 7374 796c 653d  ", header_style=
+0003e1a0: 2223 6663 3534 3234 2229 0a20 2020 2064  "#fc5424").    d
+0003e1b0: 6637 5f74 6162 6c65 2e61 6464 5f72 6f77  f7_table.add_row
+0003e1c0: 2822 4f75 7463 6f6d 6520 4461 7461 222c  ("Outcome Data",
+0003e1d0: 206f 7574 6669 6c65 2c20 7374 796c 653d   outfile, style=
+0003e1e0: 5748 4954 4529 0a0a 2020 2020 7265 7475  WHITE)..    retu
+0003e1f0: 726e 2064 6637 5f74 6162 6c65 0a0a 6465  rn df7_table..de
+0003e200: 6620 6461 7461 6672 616d 655f 385f 6f75  f dataframe_8_ou
+0003e210: 7470 7574 5f64 6973 706c 6179 2866 756e  tput_display(fun
+0003e220: 6374 696f 6e73 2c20 6f75 7466 696c 6529  ctions, outfile)
+0003e230: 3a0a 2020 2020 636f 6e73 6f6c 6520 3d20  :.    console = 
+0003e240: 436f 6e73 6f6c 6528 290a 2020 2020 6375  Console().    cu
+0003e250: 7374 6f6d 5f73 7479 6c65 5f64 6631 203d  stom_style_df1 =
+0003e260: 2053 7479 6c65 2862 6763 6f6c 6f72 3d47   Style(bgcolor=G
+0003e270: 5245 5929 0a0a 2020 2020 6466 385f 7461  REY)..    df8_ta
+0003e280: 626c 6520 3d20 5461 626c 6528 7368 6f77  ble = Table(show
+0003e290: 5f68 6561 6465 723d 5472 7565 2c20 0a20  _header=True, . 
+0003e2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003e2b0: 2020 2020 2073 7479 6c65 3d63 7573 746f       style=custo
+0003e2c0: 6d5f 7374 796c 655f 6466 312c 0a20 2020  m_style_df1,.   
+0003e2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003e2e0: 2020 2074 6974 6c65 3d4e 6f6e 652c 0a20     title=None,. 
+0003e2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003e300: 2020 2020 2073 6166 655f 626f 783d 4661       safe_box=Fa
+0003e310: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+0003e320: 2020 2020 2020 2020 2020 2062 6f78 3d62             box=b
+0003e330: 6f78 2e53 494d 504c 4529 0a0a 2020 2020  ox.SIMPLE)..    
+0003e340: 6466 385f 7461 626c 652e 6164 645f 636f  df8_table.add_co
+0003e350: 6c75 6d6e 2822 5365 6c65 6374 696f 6e22  lumn("Selection"
+0003e360: 2c20 6a75 7374 6966 793d 2263 656e 7465  , justify="cente
+0003e370: 7222 2c20 6865 6164 6572 5f73 7479 6c65  r", header_style
+0003e380: 3d22 2366 6335 3432 3422 290a 2020 2020  ="#fc5424").    
+0003e390: 6466 385f 7461 626c 652e 6164 645f 636f  df8_table.add_co
+0003e3a0: 6c75 6d6e 2822 4f75 7470 7574 2064 6972  lumn("Output dir
+0003e3b0: 6563 746f 7279 222c 206a 7573 7469 6679  ectory", justify
+0003e3c0: 3d22 6c65 6674 222c 2068 6561 6465 725f  ="left", header_
+0003e3d0: 7374 796c 653d 2223 6663 3534 3234 2229  style="#fc5424")
+0003e3e0: 0a20 2020 2064 6638 5f74 6162 6c65 2e61  .    df8_table.a
+0003e3f0: 6464 5f72 6f77 2822 5374 7564 7920 5365  dd_row("Study Se
+0003e400: 6375 7269 7479 222c 206f 7574 6669 6c65  curity", outfile
+0003e410: 2c20 7374 796c 653d 5748 4954 4529 0a0a  , style=WHITE)..
+0003e420: 2020 2020 7265 7475 726e 2064 6638 5f74      return df8_t
+0003e430: 6162 6c65 0a0a 6465 6620 6461 7461 6672  able..def datafr
+0003e440: 616d 655f 395f 6f75 7470 7574 5f64 6973  ame_9_output_dis
+0003e450: 706c 6179 2866 756e 6374 696f 6e73 2c20  play(functions, 
+0003e460: 6f75 7466 696c 6529 3a0a 2020 2020 636f  outfile):.    co
+0003e470: 6e73 6f6c 6520 3d20 436f 6e73 6f6c 6528  nsole = Console(
+0003e480: 290a 2020 2020 6375 7374 6f6d 5f73 7479  ).    custom_sty
+0003e490: 6c65 5f64 6631 203d 2053 7479 6c65 2862  le_df1 = Style(b
+0003e4a0: 6763 6f6c 6f72 3d47 5245 5929 0a0a 2020  gcolor=GREY)..  
+0003e4b0: 2020 6466 395f 7461 626c 6520 3d20 5461    df9_table = Ta
+0003e4c0: 626c 6528 7368 6f77 5f68 6561 6465 723d  ble(show_header=
+0003e4d0: 5472 7565 2c20 0a20 2020 2020 2020 2020  True, .         
+0003e4e0: 2020 2020 2020 2020 2020 2020 2073 7479               sty
+0003e4f0: 6c65 3d63 7573 746f 6d5f 7374 796c 655f  le=custom_style_
+0003e500: 6466 312c 0a20 2020 2020 2020 2020 2020  df1,.           
+0003e510: 2020 2020 2020 2020 2020 2074 6974 6c65             title
+0003e520: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+0003e530: 2020 2020 2020 2020 2020 2020 2073 6166               saf
+0003e540: 655f 626f 783d 4661 6c73 652c 0a20 2020  e_box=False,.   
+0003e550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003e560: 2020 2062 6f78 3d62 6f78 2e53 494d 504c     box=box.SIMPL
+0003e570: 4529 0a0a 2020 2020 6466 395f 7461 626c  E)..    df9_tabl
+0003e580: 652e 6164 645f 636f 6c75 6d6e 2822 5365  e.add_column("Se
+0003e590: 6c65 6374 696f 6e22 2c20 6a75 7374 6966  lection", justif
+0003e5a0: 793d 2263 656e 7465 7222 2c20 6865 6164  y="center", head
+0003e5b0: 6572 5f73 7479 6c65 3d22 2366 6335 3432  er_style="#fc542
+0003e5c0: 3422 290a 2020 2020 6466 395f 7461 626c  4").    df9_tabl
+0003e5d0: 652e 6164 645f 636f 6c75 6d6e 2822 4f75  e.add_column("Ou
+0003e5e0: 7470 7574 2064 6972 6563 746f 7279 222c  tput directory",
+0003e5f0: 206a 7573 7469 6679 3d22 6c65 6674 222c   justify="left",
+0003e600: 2068 6561 6465 725f 7374 796c 653d 2223   header_style="#
+0003e610: 6663 3534 3234 2229 0a20 2020 2064 6639  fc5424").    df9
+0003e620: 5f74 6162 6c65 2e61 6464 5f72 6f77 2822  _table.add_row("
+0003e630: 5061 646c 6f63 6b73 222c 206f 7574 6669  Padlocks", outfi
+0003e640: 6c65 2c20 7374 796c 653d 5748 4954 4529  le, style=WHITE)
+0003e650: 0a0a 2020 2020 7265 7475 726e 2064 6639  ..    return df9
+0003e660: 5f74 6162 6c65 0a0a 6465 6620 6461 7461  _table..def data
+0003e670: 6672 616d 655f 3130 5f6f 7574 7075 745f  frame_10_output_
+0003e680: 6469 7370 6c61 7928 6675 6e63 7469 6f6e  display(function
+0003e690: 732c 206f 7574 6669 6c65 293a 0a20 2020  s, outfile):.   
+0003e6a0: 2063 6f6e 736f 6c65 203d 2043 6f6e 736f   console = Conso
+0003e6b0: 6c65 2829 0a20 2020 2063 7573 746f 6d5f  le().    custom_
+0003e6c0: 7374 796c 655f 6466 3120 3d20 5374 796c  style_df1 = Styl
+0003e6d0: 6528 6267 636f 6c6f 723d 4752 4559 290a  e(bgcolor=GREY).
+0003e6e0: 0a20 2020 2064 6631 305f 7461 626c 6520  .    df10_table 
+0003e6f0: 3d20 5461 626c 6528 7368 6f77 5f68 6561  = Table(show_hea
+0003e700: 6465 723d 5472 7565 2c20 0a20 2020 2020  der=True, .     
+0003e710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003e720: 2073 7479 6c65 3d63 7573 746f 6d5f 7374   style=custom_st
+0003e730: 796c 655f 6466 312c 0a20 2020 2020 2020  yle_df1,.       
+0003e740: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0003e750: 6974 6c65 3d4e 6f6e 652c 0a20 2020 2020  itle=None,.     
+0003e760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003e770: 2073 6166 655f 626f 783d 4661 6c73 652c   safe_box=False,
+0003e780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0003e790: 2020 2020 2020 2062 6f78 3d62 6f78 2e53         box=box.S
+0003e7a0: 494d 504c 4529 0a0a 2020 2020 6466 3130  IMPLE)..    df10
+0003e7b0: 5f74 6162 6c65 2e61 6464 5f63 6f6c 756d  _table.add_colum
+0003e7c0: 6e28 2253 656c 6563 7469 6f6e 222c 206a  n("Selection", j
+0003e7d0: 7573 7469 6679 3d22 6365 6e74 6572 222c  ustify="center",
+0003e7e0: 2068 6561 6465 725f 7374 796c 653d 2223   header_style="#
+0003e7f0: 6663 3534 3234 2229 0a20 2020 2064 6631  fc5424").    df1
+0003e800: 305f 7461 626c 652e 6164 645f 636f 6c75  0_table.add_colu
+0003e810: 6d6e 2822 4f75 7470 7574 2064 6972 6563  mn("Output direc
+0003e820: 746f 7279 222c 206a 7573 7469 6679 3d22  tory", justify="
+0003e830: 6c65 6674 222c 2068 6561 6465 725f 7374  left", header_st
+0003e840: 796c 653d 2223 6663 3534 3234 2229 0a20  yle="#fc5424"). 
+0003e850: 2020 2064 6631 305f 7461 626c 652e 6164     df10_table.ad
+0003e860: 645f 726f 7728 2252 6566 6572 656e 6365  d_row("Reference
+0003e870: 7322 2c20 6f75 7466 696c 652c 2073 7479  s", outfile, sty
+0003e880: 6c65 3d57 4849 5445 290a 0a20 2020 2072  le=WHITE)..    r
+0003e890: 6574 7572 6e20 6466 3130 5f74 6162 6c65  eturn df10_table
+0003e8a0: 0a0a 6465 6620 6461 7461 6672 616d 655f  ..def dataframe_
+0003e8b0: 3131 5f6f 7574 7075 745f 6469 7370 6c61  11_output_displa
+0003e8c0: 7928 6675 6e63 7469 6f6e 732c 206f 7574  y(functions, out
+0003e8d0: 6669 6c65 293a 0a20 2020 2063 6f6e 736f  file):.    conso
+0003e8e0: 6c65 203d 2043 6f6e 736f 6c65 2829 0a20  le = Console(). 
+0003e8f0: 2020 2063 7573 746f 6d5f 7374 796c 655f     custom_style_
+0003e900: 6466 3120 3d20 5374 796c 6528 6267 636f  df1 = Style(bgco
+0003e910: 6c6f 723d 4752 4559 290a 0a20 2020 2064  lor=GREY)..    d
+0003e920: 6631 315f 7461 626c 6520 3d20 5461 626c  f11_table = Tabl
+0003e930: 6528 7368 6f77 5f68 6561 6465 723d 5472  e(show_header=Tr
+0003e940: 7565 2c20 0a20 2020 2020 2020 2020 2020  ue, .           
+0003e950: 2020 2020 2020 2020 2020 2073 7479 6c65             style
+0003e960: 3d63 7573 746f 6d5f 7374 796c 655f 6466  =custom_style_df
+0003e970: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
+0003e980: 2020 2020 2020 2020 2074 6974 6c65 3d4e           title=N
+0003e990: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+0003e9a0: 2020 2020 2020 2020 2020 2073 6166 655f             safe_
+0003e9b0: 626f 783d 4661 6c73 652c 0a20 2020 2020  box=False,.     
+0003e9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003e9d0: 2062 6f78 3d62 6f78 2e53 494d 504c 4529   box=box.SIMPLE)
+0003e9e0: 0a0a 2020 2020 6466 3131 5f74 6162 6c65  ..    df11_table
+0003e9f0: 2e61 6464 5f63 6f6c 756d 6e28 2253 656c  .add_column("Sel
+0003ea00: 6563 7469 6f6e 222c 206a 7573 7469 6679  ection", justify
+0003ea10: 3d22 6365 6e74 6572 222c 2068 6561 6465  ="center", heade
+0003ea20: 725f 7374 796c 653d 2223 6663 3534 3234  r_style="#fc5424
+0003ea30: 2229 0a20 2020 2064 6631 315f 7461 626c  ").    df11_tabl
+0003ea40: 652e 6164 645f 636f 6c75 6d6e 2822 4f75  e.add_column("Ou
+0003ea50: 7470 7574 2064 6972 6563 746f 7279 222c  tput directory",
+0003ea60: 206a 7573 7469 6679 3d22 6c65 6674 222c   justify="left",
+0003ea70: 2068 6561 6465 725f 7374 796c 653d 2223   header_style="#
+0003ea80: 6663 3534 3234 2229 0a20 2020 2064 6631  fc5424").    df1
+0003ea90: 315f 7461 626c 652e 6164 645f 726f 7728  1_table.add_row(
+0003eaa0: 2243 7573 746f 6d22 2c20 6f75 7466 696c  "Custom", outfil
+0003eab0: 652c 2073 7479 6c65 3d57 4849 5445 290a  e, style=WHITE).
+0003eac0: 0a20 2020 2072 6574 7572 6e20 6466 3131  .    return df11
+0003ead0: 5f74 6162 6c65 0a0a 6465 6620 6372 6561  _table..def crea
+0003eae0: 7465 5f6f 7574 7075 745f 6469 7370 6c61  te_output_displa
+0003eaf0: 795f 7461 626c 6528 6461 7461 6672 616d  y_table(datafram
+0003eb00: 655f 6e61 6d65 2c20 6f75 7466 696c 6529  e_name, outfile)
+0003eb10: 3a0a 2020 2020 636f 6e73 6f6c 6520 3d20  :.    console = 
+0003eb20: 436f 6e73 6f6c 6528 290a 2020 2020 6375  Console().    cu
+0003eb30: 7374 6f6d 5f73 7479 6c65 5f64 6631 203d  stom_style_df1 =
+0003eb40: 2053 7479 6c65 2862 6763 6f6c 6f72 3d47   Style(bgcolor=G
+0003eb50: 5245 5929 0a0a 2020 2020 6466 5f74 6162  REY)..    df_tab
+0003eb60: 6c65 203d 2054 6162 6c65 2873 686f 775f  le = Table(show_
+0003eb70: 6865 6164 6572 3d54 7275 652c 0a20 2020  header=True,.   
+0003eb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003eb90: 2020 7374 796c 653d 6375 7374 6f6d 5f73    style=custom_s
+0003eba0: 7479 6c65 5f64 6631 2c0a 2020 2020 2020  tyle_df1,.      
+0003ebb0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0003ebc0: 6974 6c65 3d4e 6f6e 652c 0a20 2020 2020  itle=None,.     
+0003ebd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003ebe0: 7361 6665 5f62 6f78 3d46 616c 7365 2c0a  safe_box=False,.
+0003ebf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003ec00: 2020 2020 2062 6f78 3d62 6f78 2e53 494d       box=box.SIM
+0003ec10: 504c 4529 0a0a 2020 2020 6466 5f74 6162  PLE)..    df_tab
+0003ec20: 6c65 2e61 6464 5f63 6f6c 756d 6e28 2253  le.add_column("S
+0003ec30: 656c 6563 7469 6f6e 222c 206a 7573 7469  election", justi
+0003ec40: 6679 3d22 6365 6e74 6572 222c 2068 6561  fy="center", hea
+0003ec50: 6465 725f 7374 796c 653d 2223 6663 3534  der_style="#fc54
+0003ec60: 3234 2229 0a20 2020 2064 665f 7461 626c  24").    df_tabl
+0003ec70: 652e 6164 645f 636f 6c75 6d6e 2822 4f75  e.add_column("Ou
+0003ec80: 7470 7574 2064 6972 6563 746f 7279 222c  tput directory",
+0003ec90: 206a 7573 7469 6679 3d22 6c65 6674 222c   justify="left",
+0003eca0: 2068 6561 6465 725f 7374 796c 653d 2223   header_style="#
+0003ecb0: 6663 3534 3234 2229 0a20 2020 2064 665f  fc5424").    df_
+0003ecc0: 7461 626c 652e 6164 645f 726f 7728 6461  table.add_row(da
+0003ecd0: 7461 6672 616d 655f 6e61 6d65 2c20 6f75  taframe_name, ou
+0003ece0: 7466 696c 652c 2073 7479 6c65 3d57 4849  tfile, style=WHI
+0003ecf0: 5445 290a 0a20 2020 2072 6574 7572 6e20  TE)..    return 
+0003ed00: 6466 5f74 6162 6c65 0a0a 0a64 6566 2069  df_table...def i
+0003ed10: 6e70 7574 5f66 696c 655f 696e 666f 5f64  nput_file_info_d
+0003ed20: 6973 706c 6179 2864 6174 615f 6669 6c65  isplay(data_file
+0003ed30: 293a 0a0a 2020 2020 7461 626c 655f 7469  ):..    table_ti
+0003ed40: 746c 655f 7374 796c 6520 3d20 5374 796c  tle_style = Styl
+0003ed50: 6528 6974 616c 6963 3d46 616c 7365 2c20  e(italic=False, 
+0003ed60: 6267 636f 6c6f 723d 4752 4559 2c20 636f  bgcolor=GREY, co
+0003ed70: 6c6f 723d 5748 4954 452c 2062 6f6c 643d  lor=WHITE, bold=
+0003ed80: 5472 7565 290a 2020 2020 6865 6164 6572  True).    header
+0003ed90: 5f73 7479 6c65 203d 2053 7479 6c65 2869  _style = Style(i
+0003eda0: 7461 6c69 633d 4661 6c73 652c 2062 6763  talic=False, bgc
+0003edb0: 6f6c 6f72 3d47 5245 592c 2063 6f6c 6f72  olor=GREY, color
+0003edc0: 3d22 2366 6335 3432 3422 2c20 626f 6c64  ="#fc5424", bold
+0003edd0: 3d54 7275 6529 0a20 2020 2063 6f6c 756d  =True).    colum
+0003ede0: 6e5f 7374 796c 6520 3d20 5374 796c 6528  n_style = Style(
+0003edf0: 6267 636f 6c6f 723d 4752 4559 2c20 636f  bgcolor=GREY, co
+0003ee00: 6c6f 723d 5748 4954 4529 200a 0a20 2020  lor=WHITE) ..   
+0003ee10: 2066 696c 655f 696e 666f 5f74 6162 6c65   file_info_table
+0003ee20: 203d 2054 6162 6c65 2873 686f 775f 6865   = Table(show_he
+0003ee30: 6164 6572 3d54 7275 652c 0a20 2020 2020  ader=True,.     
+0003ee40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003ee50: 2020 6869 6768 6c69 6768 743d 4661 6c73    highlight=Fals
+0003ee60: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0003ee70: 2020 2020 2020 2020 2020 7469 746c 653d            title=
+0003ee80: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+0003ee90: 2020 2020 2020 2020 2020 2020 2074 6974               tit
+0003eea0: 6c65 5f73 7479 6c65 3d74 6162 6c65 5f74  le_style=table_t
+0003eeb0: 6974 6c65 5f73 7479 6c65 2c0a 2020 2020  itle_style,.    
+0003eec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003eed0: 2020 2062 6f78 3d62 6f78 2e53 494d 504c     box=box.SIMPL
+0003eee0: 4529 0a20 2020 200a 2020 2020 6669 6c65  E).    .    file
+0003eef0: 5f69 6e66 6f5f 7461 626c 652e 6164 645f  _info_table.add_
+0003ef00: 636f 6c75 6d6e 2822 596f 7572 2069 6e70  column("Your inp
+0003ef10: 7574 2066 696c 6522 2c20 6865 6164 6572  ut file", header
+0003ef20: 5f73 7479 6c65 3d68 6561 6465 725f 7374  _style=header_st
+0003ef30: 796c 652c 2073 7479 6c65 3d63 6f6c 756d  yle, style=colum
+0003ef40: 6e5f 7374 796c 6529 0a20 2020 2066 696c  n_style).    fil
+0003ef50: 655f 696e 666f 5f74 6162 6c65 2e61 6464  e_info_table.add
+0003ef60: 5f72 6f77 2864 6174 615f 6669 6c65 290a  _row(data_file).
+0003ef70: 2020 2020 7265 7475 726e 2066 696c 655f      return file_
+0003ef80: 696e 666f 5f74 6162 6c65 0a0a 6465 6620  info_table..def 
+0003ef90: 6d61 696e 5f6d 656e 755f 6469 7370 6c61  main_menu_displa
+0003efa0: 7928 293a 0a20 2020 2063 6f6e 736f 6c65  y():.    console
+0003efb0: 203d 2043 6f6e 736f 6c65 2829 0a20 2020   = Console().   
+0003efc0: 2023 6461 7461 5f63 6c65 616e 696e 675f   #data_cleaning_
+0003efd0: 7661 725f 7461 626c 6520 3d20 6461 7461  var_table = data
+0003efe0: 5f63 6c65 616e 696e 675f 636f 6c5f 6272  _cleaning_col_br
+0003eff0: 6561 6b64 6f77 6e28 290a 2020 2020 6d61  eakdown().    ma
+0003f000: 696e 5f6d 656e 755f 7461 626c 6520 3d20  in_menu_table = 
+0003f010: 6469 7370 6c61 795f 6d61 696e 5f6d 656e  display_main_men
+0003f020: 7528 290a 2020 2020 6461 7461 6669 6c65  u().    datafile
+0003f030: 5f69 6e66 6f5f 7461 626c 6520 3d20 696e  _info_table = in
+0003f040: 7075 745f 6669 6c65 5f69 6e66 6f5f 6469  put_file_info_di
+0003f050: 7370 6c61 7928 6461 7461 5f66 696c 6529  splay(data_file)
+0003f060: 0a0a 2020 2020 6375 7374 6f6d 5f73 7479  ..    custom_sty
+0003f070: 6c65 5f6d 6169 6e20 3d20 5374 796c 6528  le_main = Style(
+0003f080: 6267 636f 6c6f 723d 4752 4559 290a 2020  bgcolor=GREY).  
+0003f090: 2020 6375 7374 6f6d 5f73 7479 6c65 5f66    custom_style_f
+0003f0a0: 696c 655f 6465 7461 696c 7320 3d20 5374  ile_details = St
+0003f0b0: 796c 6528 6267 636f 6c6f 723d 4752 4559  yle(bgcolor=GREY
+0003f0c0: 290a 2020 2020 6375 7374 6f6d 5f73 7479  ).    custom_sty
+0003f0d0: 6c65 5f63 6c65 616e 696e 675f 696e 666f  le_cleaning_info
+0003f0e0: 203d 2053 7479 6c65 2862 6763 6f6c 6f72   = Style(bgcolor
+0003f0f0: 3d47 5245 5929 0a0a 2020 2020 636f 6e74  =GREY)..    cont
+0003f100: 6169 6e65 725f 7469 746c 6520 3d20 636f  ainer_title = co
+0003f110: 6e73 6f6c 652e 7265 6e64 6572 5f73 7472  nsole.render_str
+0003f120: 2822 5b62 6f6c 6420 7768 6974 655d 4545  ("[bold white]EE
+0003f130: 4620 4461 7461 2045 7874 7261 6374 6f72  F Data Extractor
+0003f140: 5b2f 626f 6c64 2077 6869 7465 5d22 290a  [/bold white]").
+0003f150: 0a20 2020 2074 6f70 5f74 6974 6c65 203d  .    top_title =
+0003f160: 2063 6f6e 736f 6c65 2e72 656e 6465 725f   console.render_
+0003f170: 7374 7228 225b 626f 6c64 2077 6869 7465  str("[bold white
+0003f180: 5d57 656c 636f 6d65 5b2f 626f 6c64 2077  ]Welcome[/bold w
+0003f190: 6869 7465 5d22 290a 2020 2020 7469 746c  hite]").    titl
+0003f1a0: 6531 203d 2063 6f6e 736f 6c65 2e72 656e  e1 = console.ren
+0003f1b0: 6465 725f 7374 7228 225b 626f 6c64 2077  der_str("[bold w
+0003f1c0: 6869 7465 5d4d 6169 6e20 4d65 6e75 5b2f  hite]Main Menu[/
+0003f1d0: 626f 6c64 2077 6869 7465 5d22 290a 2020  bold white]").  
+0003f1e0: 2020 7469 746c 6532 203d 2063 6f6e 736f    title2 = conso
+0003f1f0: 6c65 2e72 656e 6465 725f 7374 7228 225b  le.render_str("[
+0003f200: 626f 6c64 2077 6869 7465 5d44 6174 6120  bold white]Data 
+0003f210: 4669 6c65 2044 6574 6169 6c73 5b2f 626f  File Details[/bo
+0003f220: 6c64 2077 6869 7465 5d22 290a 0a20 2020  ld white]")..   
+0003f230: 2023 2053 6574 2074 6578 7420 666f 7220   # Set text for 
+0003f240: 746f 7020 7061 6e65 6c20 6f66 206d 6169  top panel of mai
+0003f250: 6e20 6d65 6e75 0a20 2020 2074 6f70 5f70  n menu.    top_p
+0003f260: 616e 656c 5f74 6578 7420 3d20 280a 2020  anel_text = (.  
+0003f270: 2020 2020 2020 225b 2346 4646 4646 465d        "[#FFFFFF]
+0003f280: 5765 6c63 6f6d 6520 746f 2074 6865 2045  Welcome to the E
+0003f290: 4546 2044 6174 6120 4578 7472 6163 746f  EF Data Extracto
+0003f2a0: 722e 2055 7365 2074 6865 5b2f 2346 4646  r. Use the[/#FFF
+0003f2b0: 4646 465d 2022 0a20 2020 2020 2020 2022  FFF] ".        "
+0003f2c0: 5b62 6f6c 6420 2366 6335 3432 345d 4d61  [bold #fc5424]Ma
+0003f2d0: 696e 204d 656e 755b 2f62 6f6c 6420 2366  in Menu[/bold #f
+0003f2e0: 6335 3432 345d 205b 2346 4646 4646 465d  c5424] [#FFFFFF]
+0003f2f0: 746f 2067 656e 6572 6174 6520 7661 7269  to generate vari
+0003f300: 6f75 7320 6461 7461 6672 616d 6573 2063  ous dataframes c
+0003f310: 6f6e 7461 696e 696e 6720 6461 7461 2065  ontaining data e
+0003f320: 7874 7261 6374 6564 2022 0a20 2020 2020  xtracted ".     
+0003f330: 2020 2022 6672 6f6d 2061 6e20 696e 7075     "from an inpu
+0003f340: 7420 5b62 6f6c 6420 2366 6335 3432 345d  t [bold #fc5424]
+0003f350: 4a53 4f4e 5b2f 626f 6c64 2023 6663 3534  JSON[/bold #fc54
+0003f360: 3234 5d20 5b23 4646 4646 4646 5d64 6174  24] [#FFFFFF]dat
+0003f370: 6166 696c 6520 7072 6f64 7563 6564 2062  afile produced b
+0003f380: 7920 7468 6520 4545 4620 4564 7563 6174  y the EEF Educat
+0003f390: 696f 6e20 4576 6964 656e 6365 2022 0a20  ion Evidence ". 
+0003f3a0: 2020 2020 2020 2022 4461 7461 6261 7365         "Database
+0003f3b0: 2e5c 6e5c 6e5b 626f 6c64 2023 6663 3534  .\n\n[bold #fc54
+0003f3c0: 3234 5d4f 7074 696f 6e73 2031 2d35 5b2f  24]Options 1-5[/
+0003f3d0: 626f 6c64 2023 6663 3534 3234 5d20 5b23  bold #fc5424] [#
+0003f3e0: 4646 4646 4646 5d69 6e63 6c75 6465 206f  FFFFFF]include o
+0003f3f0: 7572 206f 776e 2063 7573 746f 6d20 6461  ur own custom da
+0003f400: 7461 6672 616d 6573 2022 0a20 2020 2020  taframes ".     
+0003f410: 2020 2022 666f 7220 6461 7461 2063 6c65     "for data cle
+0003f420: 616e 696e 6720 7072 696f 7220 746f 2061  aning prior to a
+0003f430: 6e61 6c79 7369 732e 5b2f 2346 4646 4646  nalysis.[/#FFFFF
+0003f440: 465d 205b 626f 6c64 2023 6663 3534 3234  F] [bold #fc5424
+0003f450: 5d4f 7074 696f 6e20 365b 2f62 6f6c 6420  ]Option 6[/bold 
+0003f460: 2366 6335 3432 345d 205b 2346 4646 4646  #fc5424] [#FFFFF
+0003f470: 465d 6765 6e65 7261 7465 7320 7468 6520  F]generates the 
+0003f480: 220a 2020 2020 2020 2020 2266 696e 616c  ".        "final
+0003f490: 2064 6174 6166 7261 6d65 2873 2920 7573   dataframe(s) us
+0003f4a0: 6564 2069 6e20 6f75 7220 6d65 7461 2d61  ed in our meta-a
+0003f4b0: 6e61 6c79 7365 732e 205b 626f 6c64 2023  nalyses. [bold #
+0003f4c0: 6663 3534 3234 5d4f 7074 696f 6e20 375b  fc5424]Option 7[
+0003f4d0: 2f62 6f6c 6420 2366 6335 3432 345d 2070  /bold #fc5424] p
+0003f4e0: 726f 6475 6365 7320 7261 7720 2875 6e6f  roduces raw (uno
+0003f4f0: 7264 6572 6564 2920 220a 2020 2020 2020  rdered) ".      
+0003f500: 2020 226f 7574 636f 6d65 2064 6174 612e    "outcome data.
+0003f510: 205b 626f 6c64 2023 6663 3534 3234 5d4f   [bold #fc5424]O
+0003f520: 7074 696f 6e20 385b 2f62 6f6c 6420 2366  ption 8[/bold #f
+0003f530: 6335 3432 345d 2070 726f 6475 6365 7320  c5424] produces 
+0003f540: 6120 6265 7370 6f6b 6520 7374 7564 7920  a bespoke study 
+0003f550: 7365 6375 7269 7479 2064 6174 6166 7261  security datafra
+0003f560: 6d65 2e20 220a 2020 2020 2020 2020 225b  me. ".        "[
+0003f570: 2f23 4646 4646 4646 5d5b 626f 6c64 2023  /#FFFFFF][bold #
+0003f580: 6663 3534 3234 5d4f 7074 696f 6e20 395b  fc5424]Option 9[
+0003f590: 2f62 6f6c 6420 2366 6335 3432 345d 2070  /bold #fc5424] p
+0003f5a0: 726f 6475 6365 7320 6120 7374 7261 6e64  roduces a strand
+0003f5b0: 2d6c 6576 656c 2027 7061 646c 6f63 6b73  -level 'padlocks
+0003f5c0: 2720 6461 7461 6672 616d 652e 205b 626f  ' dataframe. [bo
+0003f5d0: 6c64 2023 6663 3534 3234 5d4f 7074 696f  ld #fc5424]Optio
+0003f5e0: 6e20 3130 5b2f 626f 6c64 2023 6663 3534  n 10[/bold #fc54
+0003f5f0: 3234 5d20 5b23 4646 4646 4646 5d63 6f6d  24] [#FFFFFF]com
+0003f600: 7069 6c65 7320 220a 2020 2020 2020 2020  piles ".        
+0003f610: 2274 6865 206e 6563 6573 7361 7279 2064  "the necessary d
+0003f620: 6174 6120 666f 7220 636f 6e73 7472 7563  ata for construc
+0003f630: 7469 6e67 2073 7475 6479 2072 6566 6572  ting study refer
+0003f640: 656e 6365 732e 2046 696e 616c 6c79 2c20  ences. Finally, 
+0003f650: 5b2f 2346 4646 4646 465d 5b62 6f6c 6420  [/#FFFFFF][bold 
+0003f660: 2366 6335 3432 345d 4f70 7469 6f6e 2031  #fc5424]Option 1
+0003f670: 315b 2f62 6f6c 6420 2366 6335 3432 345d  1[/bold #fc5424]
+0003f680: 2022 0a20 2020 2020 2020 2022 5b23 4646   ".        "[#FF
+0003f690: 4646 4646 5d61 6c6c 6f77 7320 796f 7520  FFFF]allows you 
+0003f6a0: 746f 2063 7265 6174 6520 796f 7572 206f  to create your o
+0003f6b0: 776e 2063 7573 746f 6d20 636f 6c75 6d6e  wn custom column
+0003f6c0: 2064 6174 6166 7261 6d65 2c5b 2f23 4646   dataframe,[/#FF
+0003f6d0: 4646 4646 5d20 616e 6420 5b62 6f6c 6420  FFFF] and [bold 
+0003f6e0: 2366 6335 3432 345d 6f70 7469 6f6e 2031  #fc5424]option 1
+0003f6f0: 325b 2f62 6f6c 6420 2366 6335 3432 345d  2[/bold #fc5424]
+0003f700: 2061 6c6c 6f77 7320 796f 7520 746f 2063   allows you to c
+0003f710: 7265 6174 6520 796f 7572 206f 776e 2022  reate your own "
+0003f720: 0a20 2020 2020 2020 2022 696e 6469 7669  .        "indivi
+0003f730: 6475 616c 2073 7475 6479 2064 6174 6166  dual study dataf
+0003f740: 7261 6d65 2e22 0a20 2020 2029 0a20 2020  rame.".    ).   
+0003f750: 2074 6f70 5f6d 656e 755f 7374 796c 6520   top_menu_style 
+0003f760: 3d20 5374 796c 6528 6267 636f 6c6f 723d  = Style(bgcolor=
+0003f770: 4752 4559 290a 0a20 2020 2023 2063 7265  GREY)..    # cre
+0003f780: 6174 6520 7468 6520 7061 6e65 6c20 7769  ate the panel wi
+0003f790: 7468 2074 6865 2074 6578 740a 2020 2020  th the text.    
+0003f7a0: 746f 705f 7061 6e65 6c20 3d20 5061 6e65  top_panel = Pane
+0003f7b0: 6c28 0a20 2020 2020 2020 2074 6f70 5f70  l(.        top_p
+0003f7c0: 616e 656c 5f74 6578 742c 0a20 2020 2020  anel_text,.     
+0003f7d0: 2020 2074 6974 6c65 3d74 6f70 5f74 6974     title=top_tit
+0003f7e0: 6c65 2c20 0a20 2020 2020 2020 2062 6f72  le, .        bor
+0003f7f0: 6465 725f 7374 796c 653d 2262 6f6c 6420  der_style="bold 
+0003f800: 7768 6974 6522 2c0a 2020 2020 2020 2020  white",.        
+0003f810: 7469 746c 655f 616c 6967 6e3d 226c 6566  title_align="lef
+0003f820: 7422 2c0a 2020 2020 2020 2020 7374 796c  t",.        styl
+0003f830: 653d 746f 705f 6d65 6e75 5f73 7479 6c65  e=top_menu_style
+0003f840: 2c0a 2020 2020 2020 2020 7061 6464 696e  ,.        paddin
+0003f850: 673d 2831 2c20 3229 2c0a 2020 2020 2020  g=(1, 2),.      
+0003f860: 2020 7769 6474 683d 3132 302c 0a20 2020    width=120,.   
+0003f870: 2029 0a0a 2020 2020 7061 6e65 6c31 203d   )..    panel1 =
+0003f880: 2050 616e 656c 2e66 6974 280a 2020 2020   Panel.fit(.    
+0003f890: 2020 2020 6d61 696e 5f6d 656e 755f 7461      main_menu_ta
+0003f8a0: 626c 652c 0a20 2020 2020 2020 2074 6974  ble,.        tit
+0003f8b0: 6c65 3d74 6974 6c65 312c 0a20 2020 2020  le=title1,.     
+0003f8c0: 2020 2062 6f72 6465 725f 7374 796c 653d     border_style=
+0003f8d0: 2262 6f6c 6420 7768 6974 6522 2c0a 2020  "bold white",.  
+0003f8e0: 2020 2020 2020 7374 796c 653d 6375 7374        style=cust
+0003f8f0: 6f6d 5f73 7479 6c65 5f6d 6169 6e2c 0a20  om_style_main,. 
+0003f900: 2020 2020 2020 2074 6974 6c65 5f61 6c69         title_ali
+0003f910: 676e 3d22 6c65 6674 222c 0a20 2020 2020  gn="left",.     
+0003f920: 2020 2070 6164 6469 6e67 3d28 312c 2032     padding=(1, 2
+0003f930: 292c 0a20 2020 2020 2020 2077 6964 7468  ),.        width
+0003f940: 3d31 3230 2c0a 2020 2020 290a 0a20 2020  =120,.    )..   
+0003f950: 2070 616e 656c 3220 3d20 5061 6e65 6c2e   panel2 = Panel.
+0003f960: 6669 7428 0a20 2020 2020 2020 2064 6174  fit(.        dat
+0003f970: 6166 696c 655f 696e 666f 5f74 6162 6c65  afile_info_table
+0003f980: 2c0a 2020 2020 2020 2020 7469 746c 653d  ,.        title=
+0003f990: 7469 746c 6532 2c0a 2020 2020 2020 2020  title2,.        
+0003f9a0: 626f 7264 6572 5f73 7479 6c65 3d22 626f  border_style="bo
+0003f9b0: 6c64 2077 6869 7465 222c 0a20 2020 2020  ld white",.     
+0003f9c0: 2020 2073 7479 6c65 3d63 7573 746f 6d5f     style=custom_
+0003f9d0: 7374 796c 655f 6669 6c65 5f64 6574 6169  style_file_detai
+0003f9e0: 6c73 2c0a 2020 2020 2020 2020 7469 746c  ls,.        titl
+0003f9f0: 655f 616c 6967 6e3d 226c 6566 7422 2c0a  e_align="left",.
+0003fa00: 2020 2020 2020 2020 7061 6464 696e 673d          padding=
+0003fa10: 2831 2c20 3229 2c0a 2020 2020 2020 2020  (1, 2),.        
+0003fa20: 7769 6474 683d 3132 302c 0a20 2020 2029  width=120,.    )
+0003fa30: 0a0a 2020 2020 2320 636f 6d62 696e 6520  ..    # combine 
+0003fa40: 7468 6520 7465 7874 2070 616e 656c 2061  the text panel a
+0003fa50: 6e64 2070 616e 656c 7320 696e 746f 2061  nd panels into a
+0003fa60: 206e 6577 2063 6f6c 756d 6e0a 2020 2020   new column.    
+0003fa70: 636f 6c75 6d6e 5f63 6f6d 6269 6e65 6420  column_combined 
+0003fa80: 3d20 436f 6c75 6d6e 7328 5b74 6f70 5f70  = Columns([top_p
+0003fa90: 616e 656c 2c20 7061 6e65 6c31 2c20 7061  anel, panel1, pa
+0003faa0: 6e65 6c32 5d2c 2065 7175 616c 3d46 616c  nel2], equal=Fal
+0003fab0: 7365 290a 0a20 2020 2023 2063 7265 6174  se)..    # creat
+0003fac0: 6520 7468 6520 6c61 796f 7574 2077 6974  e the layout wit
+0003fad0: 6820 7468 6520 636f 6d62 696e 6564 2063  h the combined c
+0003fae0: 6f6c 756d 6e0a 2020 2020 6c61 796f 7574  olumn.    layout
+0003faf0: 203d 204c 6179 6f75 7428 636f 6c75 6d6e   = Layout(column
+0003fb00: 5f63 6f6d 6269 6e65 6429 0a0a 2020 2020  _combined)..    
+0003fb10: 7061 6e65 6c20 3d20 5061 6e65 6c28 0a20  panel = Panel(. 
+0003fb20: 2020 2020 2020 206c 6179 6f75 742c 0a20         layout,. 
+0003fb30: 2020 2020 2020 2074 6974 6c65 3d63 6f6e         title=con
+0003fb40: 7461 696e 6572 5f74 6974 6c65 2c0a 2020  tainer_title,.  
+0003fb50: 2020 2020 2020 626f 7264 6572 5f73 7479        border_sty
+0003fb60: 6c65 3d22 626f 6c64 2077 6869 7465 222c  le="bold white",
+0003fb70: 0a20 2020 2020 2020 2070 6164 6469 6e67  .        padding
+0003fb80: 3d28 312c 2032 292c 0a20 2020 2020 2020  =(1, 2),.       
+0003fb90: 2074 6974 6c65 5f61 6c69 676e 3d22 6365   title_align="ce
+0003fba0: 6e74 6572 222c 0a20 2020 2020 2020 2073  nter",.        s
+0003fbb0: 7479 6c65 3d63 7573 746f 6d5f 7374 796c  tyle=custom_styl
+0003fbc0: 655f 6d61 696e 2c0a 2020 2020 2020 2020  e_main,.        
+0003fbd0: 6865 6967 6874 3d34 372c 0a20 2020 2020  height=47,.     
+0003fbe0: 2020 2077 6964 7468 3d31 3230 2c0a 2020     width=120,.  
+0003fbf0: 2020 290a 0a20 2020 2063 6f6e 736f 6c65    )..    console
+0003fc00: 2e63 6c65 6172 2829 0a20 2020 2063 6f6e  .clear().    con
+0003fc10: 736f 6c65 2e70 7269 6e74 2870 616e 656c  sole.print(panel
+0003fc20: 290a 2020 2020 7072 696e 7428 225c 6e22  ).    print("\n"
+0003fc30: 290a 0a0a 6465 6620 6d61 696e 5f6d 656e  )...def main_men
+0003fc40: 755f 6469 7370 6c61 7931 2866 756e 6374  u_display1(funct
+0003fc50: 696f 6e73 2c20 6f75 7466 696c 6531 2c20  ions, outfile1, 
+0003fc60: 6466 5f64 6973 706c 6179 293a 0a0a 2020  df_display):..  
+0003fc70: 2020 636f 6e73 6f6c 6520 3d20 436f 6e73    console = Cons
+0003fc80: 6f6c 6528 290a 2020 2020 6f75 7470 7574  ole().    output
+0003fc90: 5f66 696c 655f 696e 666f 203d 2064 665f  _file_info = df_
+0003fca0: 6469 7370 6c61 7928 6675 6e63 7469 6f6e  display(function
+0003fcb0: 732c 206f 7574 6669 6c65 3129 0a20 2020  s, outfile1).   
+0003fcc0: 206d 6169 6e5f 6d65 6e75 5f74 6162 6c65   main_menu_table
+0003fcd0: 203d 2064 6973 706c 6179 5f6d 6169 6e5f   = display_main_
+0003fce0: 6d65 6e75 2829 0a20 2020 2064 6174 6166  menu().    dataf
+0003fcf0: 696c 655f 696e 666f 5f74 6162 6c65 203d  ile_info_table =
+0003fd00: 2069 6e70 7574 5f66 696c 655f 696e 666f   input_file_info
+0003fd10: 5f64 6973 706c 6179 2864 6174 615f 6669  _display(data_fi
+0003fd20: 6c65 290a 0a20 2020 2063 7573 746f 6d5f  le)..    custom_
+0003fd30: 7374 796c 655f 6d61 696e 203d 2053 7479  style_main = Sty
+0003fd40: 6c65 2862 6763 6f6c 6f72 3d47 5245 5929  le(bgcolor=GREY)
+0003fd50: 0a20 2020 2063 7573 746f 6d5f 7374 796c  .    custom_styl
+0003fd60: 655f 6669 6c65 5f64 6574 6169 6c73 203d  e_file_details =
+0003fd70: 2053 7479 6c65 2862 6763 6f6c 6f72 3d47   Style(bgcolor=G
+0003fd80: 5245 5929 0a20 2020 2063 7573 746f 6d5f  REY).    custom_
+0003fd90: 7374 796c 655f 636c 6561 6e69 6e67 5f69  style_cleaning_i
+0003fda0: 6e66 6f20 3d20 5374 796c 6528 6267 636f  nfo = Style(bgco
+0003fdb0: 6c6f 723d 4752 4559 290a 0a20 2020 2074  lor=GREY)..    t
+0003fdc0: 6974 6c65 3120 3d20 636f 6e73 6f6c 652e  itle1 = console.
+0003fdd0: 7265 6e64 6572 5f73 7472 2822 5b62 6f6c  render_str("[bol
+0003fde0: 6420 7768 6974 655d 4d61 696e 204d 656e  d white]Main Men
+0003fdf0: 755b 2f62 6f6c 6420 7768 6974 655d 2229  u[/bold white]")
+0003fe00: 0a20 2020 2074 6974 6c65 3220 3d20 636f  .    title2 = co
+0003fe10: 6e73 6f6c 652e 7265 6e64 6572 5f73 7472  nsole.render_str
+0003fe20: 2822 5b62 6f6c 6420 7768 6974 655d 4461  ("[bold white]Da
+0003fe30: 7461 2046 696c 6520 4465 7461 696c 735b  ta File Details[
+0003fe40: 2f62 6f6c 6420 7768 6974 655d 2229 0a20  /bold white]"). 
+0003fe50: 2020 2074 6974 6c65 3320 3d20 636f 6e73     title3 = cons
+0003fe60: 6f6c 652e 7265 6e64 6572 5f73 7472 2822  ole.render_str("
+0003fe70: 5b62 6f6c 6420 7768 6974 655d 4f75 7470  [bold white]Outp
+0003fe80: 7574 2046 696c 6573 5b2f 626f 6c64 2077  ut Files[/bold w
+0003fe90: 6869 7465 5d22 290a 0a20 2020 2070 616e  hite]")..    pan
+0003fea0: 656c 3161 203d 2050 616e 656c 2e66 6974  el1a = Panel.fit
+0003feb0: 280a 2020 2020 2020 2020 6d61 696e 5f6d  (.        main_m
+0003fec0: 656e 755f 7461 626c 652c 0a20 2020 2020  enu_table,.     
+0003fed0: 2020 2074 6974 6c65 3d74 6974 6c65 312c     title=title1,
+0003fee0: 0a20 2020 2020 2020 2062 6f72 6465 725f  .        border_
+0003fef0: 7374 796c 653d 2262 6f6c 6420 7768 6974  style="bold whit
+0003ff00: 6522 2c0a 2020 2020 2020 2020 7374 796c  e",.        styl
+0003ff10: 653d 6375 7374 6f6d 5f73 7479 6c65 5f6d  e=custom_style_m
+0003ff20: 6169 6e2c 0a20 2020 2020 2020 2074 6974  ain,.        tit
+0003ff30: 6c65 5f61 6c69 676e 3d22 6c65 6674 222c  le_align="left",
+0003ff40: 0a20 2020 2020 2020 2070 6164 6469 6e67  .        padding
+0003ff50: 3d28 312c 2032 292c 0a20 2020 2029 0a20  =(1, 2),.    ). 
+0003ff60: 2020 2070 616e 656c 3162 203d 2050 616e     panel1b = Pan
+0003ff70: 656c 2e66 6974 280a 2020 2020 2020 2020  el.fit(.        
+0003ff80: 6461 7461 6669 6c65 5f69 6e66 6f5f 7461  datafile_info_ta
+0003ff90: 626c 652c 0a20 2020 2020 2020 2074 6974  ble,.        tit
+0003ffa0: 6c65 3d74 6974 6c65 322c 0a20 2020 2020  le=title2,.     
+0003ffb0: 2020 2062 6f72 6465 725f 7374 796c 653d     border_style=
+0003ffc0: 2262 6f6c 6420 7768 6974 6522 2c0a 2020  "bold white",.  
+0003ffd0: 2020 2020 2020 7374 796c 653d 6375 7374        style=cust
+0003ffe0: 6f6d 5f73 7479 6c65 5f66 696c 655f 6465  om_style_file_de
+0003fff0: 7461 696c 732c 0a20 2020 2020 2020 2074  tails,.        t
+00040000: 6974 6c65 5f61 6c69 676e 3d22 6c65 6674  itle_align="left
+00040010: 222c 0a20 2020 2020 2020 2070 6164 6469  ",.        paddi
+00040020: 6e67 3d28 312c 2032 292c 0a20 2020 2029  ng=(1, 2),.    )
+00040030: 0a0a 2020 2020 7061 6e65 6c32 203d 2050  ..    panel2 = P
+00040040: 616e 656c 2e66 6974 280a 2020 2020 2020  anel.fit(.      
+00040050: 2020 6f75 7470 7574 5f66 696c 655f 696e    output_file_in
+00040060: 666f 2c0a 2020 2020 2020 2020 7469 746c  fo,.        titl
+00040070: 653d 7469 746c 6533 2c0a 2020 2020 2020  e=title3,.      
+00040080: 2020 626f 7264 6572 5f73 7479 6c65 3d22    border_style="
+00040090: 626f 6c64 2077 6869 7465 222c 0a20 2020  bold white",.   
+000400a0: 2020 2020 2073 7479 6c65 3d63 7573 746f       style=custo
+000400b0: 6d5f 7374 796c 655f 636c 6561 6e69 6e67  m_style_cleaning
+000400c0: 5f69 6e66 6f2c 0a20 2020 2020 2020 2074  _info,.        t
+000400d0: 6974 6c65 5f61 6c69 676e 3d22 6c65 6674  itle_align="left
+000400e0: 222c 0a20 2020 2020 2020 2070 6164 6469  ",.        paddi
+000400f0: 6e67 3d28 312c 2032 292c 0a20 2020 2029  ng=(1, 2),.    )
+00040100: 0a20 2020 2023 2063 7265 6174 6520 7468  .    # create th
+00040110: 6520 6669 7273 7420 726f 7720 6f66 2063  e first row of c
+00040120: 6f6c 756d 6e73 0a20 2020 2072 6f77 3120  olumns.    row1 
+00040130: 3d20 436f 6c75 6d6e 7328 5b70 616e 656c  = Columns([panel
+00040140: 3161 5d2c 2065 7175 616c 3d46 616c 7365  1a], equal=False
+00040150: 290a 0a20 2020 2072 6f77 3162 203d 2043  )..    row1b = C
+00040160: 6f6c 756d 6e73 285b 7061 6e65 6c31 625d  olumns([panel1b]
+00040170: 2c20 6571 7561 6c3d 4661 6c73 6529 0a0a  , equal=False)..
+00040180: 2020 2020 2320 6372 6561 7465 2074 6865      # create the
+00040190: 2073 6563 6f6e 6420 726f 7720 6f66 2063   second row of c
+000401a0: 6f6c 756d 6e73 0a20 2020 2072 6f77 3220  olumns.    row2 
+000401b0: 3d20 436f 6c75 6d6e 7328 5b70 616e 656c  = Columns([panel
+000401c0: 325d 2c20 6571 7561 6c3d 4661 6c73 6529  2], equal=False)
+000401d0: 0a0a 2020 2020 2320 6372 6561 7465 2074  ..    # create t
+000401e0: 6865 206c 6179 6f75 7420 7769 7468 2074  he layout with t
+000401f0: 6865 2070 616e 656c 730a 2020 2020 6c61  he panels.    la
+00040200: 796f 7574 203d 2043 6f6c 756d 6e73 285b  yout = Columns([
+00040210: 726f 7731 2c20 726f 7731 622c 2072 6f77  row1, row1b, row
+00040220: 325d 2c20 6571 7561 6c3d 4661 6c73 6529  2], equal=False)
+00040230: 0a0a 2020 2020 7061 6e65 6c20 3d20 5061  ..    panel = Pa
+00040240: 6e65 6c28 0a20 2020 2020 2020 206c 6179  nel(.        lay
+00040250: 6f75 742c 200a 2020 2020 2020 2020 7469  out, .        ti
+00040260: 746c 653d 2245 4546 2054 6561 6368 696e  tle="EEF Teachin
+00040270: 6720 616e 6420 4c65 6172 6e69 6e67 2054  g and Learning T
+00040280: 6f6f 6c6b 6974 2044 6174 6120 4578 7472  oolkit Data Extr
+00040290: 6163 746f 7222 2c20 0a20 2020 2020 2020  actor", .       
+000402a0: 2062 6f72 6465 725f 7374 796c 653d 2262   border_style="b
+000402b0: 6f6c 6420 7768 6974 6522 2c20 0a20 2020  old white", .   
+000402c0: 2020 2020 2070 6164 6469 6e67 3d28 312c       padding=(1,
+000402d0: 2032 292c 200a 2020 2020 2020 2020 7469   2), .        ti
+000402e0: 746c 655f 616c 6967 6e3d 226c 6566 7422  tle_align="left"
+000402f0: 2c0a 2020 2020 2020 2020 7374 796c 653d  ,.        style=
+00040300: 6375 7374 6f6d 5f73 7479 6c65 5f6d 6169  custom_style_mai
+00040310: 6e2c 0a20 2020 2020 2020 2077 6964 7468  n,.        width
+00040320: 3d31 3230 2c0a 2020 2020 2020 2020 6865  =120,.        he
+00040330: 6967 6874 3d34 3429 0a0a 2020 2020 636f  ight=44)..    co
+00040340: 6e73 6f6c 652e 636c 6561 7228 290a 2020  nsole.clear().  
+00040350: 2020 636f 6e73 6f6c 652e 7072 696e 7428    console.print(
+00040360: 7061 6e65 6c29 0a20 2020 2070 7269 6e74  panel).    print
+00040370: 2822 5c6e 2229 0a0a 7061 7468 5f63 6f6d  ("\n")..path_com
+00040380: 706c 6574 6572 203d 2050 6174 6843 6f6d  pleter = PathCom
+00040390: 706c 6574 6572 2829 0a0a 0a77 6869 6c65  pleter()...while
+000403a0: 2054 7275 653a 0a20 2020 2064 6174 615f   True:.    data_
+000403b0: 6669 6c65 203d 2070 726f 6d70 7428 2753  file = prompt('S
+000403c0: 656c 6563 7420 796f 7572 2064 6174 6120  elect your data 
+000403d0: 6669 6c65 3a20 272c 2063 6f6d 706c 6574  file: ', complet
+000403e0: 6572 3d70 6174 685f 636f 6d70 6c65 7465  er=path_complete
+000403f0: 7229 0a20 2020 2069 6620 6f73 2e70 6174  r).    if os.pat
+00040400: 682e 6973 6669 6c65 2864 6174 615f 6669  h.isfile(data_fi
+00040410: 6c65 2920 616e 6420 6461 7461 5f66 696c  le) and data_fil
+00040420: 652e 656e 6473 7769 7468 2827 2e6a 736f  e.endswith('.jso
+00040430: 6e27 293a 0a20 2020 2020 2020 2062 7265  n'):.        bre
+00040440: 616b 0a20 2020 2065 6c73 653a 0a20 2020  ak.    else:.   
+00040450: 2020 2020 2070 7269 6e74 2827 496e 7661       print('Inva
+00040460: 6c69 6420 6669 6c65 2e20 506c 6561 7365  lid file. Please
+00040470: 2065 6e74 6572 2061 2076 616c 6964 202e   enter a valid .
+00040480: 6a73 6f6e 2066 696c 652e 2729 0a0a 0a0a  json file.')....
+00040490: 6a73 6f6e 5f65 7874 7261 6374 6f72 203d  json_extractor =
+000404a0: 204a 534f 4e44 6174 6145 7874 7261 6374   JSONDataExtract
+000404b0: 6f72 2864 6174 615f 6669 6c65 29         or(data_file)
```

### Comparing `eef-data-0.52/setup.py` & `eef-data-0.53/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README_package.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='eef-data',
-    version='0.52',  # Remember to increment the version number
+    version='0.53',  # Remember to increment the version number
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'numpy==1.22.0',
         'pandas==1.5.0',
         'prompt_toolkit==3.0.30',
         'rich==12.4.4',
```

