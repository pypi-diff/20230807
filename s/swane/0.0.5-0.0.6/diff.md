# Comparing `tmp/swane-0.0.5.tar.gz` & `tmp/swane-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swane-0.0.5.tar", last modified: Sun Apr 16 17:02:37 2023, max compression
+gzip compressed data, was "swane-0.0.6.tar", last modified: Mon Aug  7 15:05:13 2023, max compression
```

## Comparing `swane-0.0.5.tar` & `swane-0.0.6.tar`

### file list

```diff
@@ -1,91 +1,95 @@
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-16 17:02:37.781633 swane-0.0.5/
--rw-rw-r--   0 mau       (1000) mau       (1000)     1976 2023-03-29 17:07:54.000000 swane-0.0.5/LICENSE
--rw-rw-r--   0 mau       (1000) mau       (1000)      184 2023-03-29 17:07:54.000000 swane-0.0.5/MANIFEST.in
--rw-rw-r--   0 mau       (1000) mau       (1000)      427 2023-04-16 17:02:37.781633 swane-0.0.5/PKG-INFO
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.5/README.md
--rw-rw-r--   0 mau       (1000) mau       (1000)       38 2023-04-16 17:02:37.781633 swane-0.0.5/setup.cfg
--rw-rw-r--   0 mau       (1000) mau       (1000)     1202 2023-04-11 08:22:48.000000 swane-0.0.5/setup.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-16 17:02:37.765633 swane-0.0.5/swane/
--rw-rw-r--   0 mau       (1000) mau       (1000)       50 2023-04-16 17:02:08.000000 swane-0.0.5/swane/__init__.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1827 2023-03-29 17:07:54.000000 swane-0.0.5/swane/__main__.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-16 17:02:37.765633 swane-0.0.5/swane/nipype_pipeline/
--rw-rw-r--   0 mau       (1000) mau       (1000)    18408 2023-04-15 15:05:28.000000 swane-0.0.5/swane/nipype_pipeline/MainWorkflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.5/swane/nipype_pipeline/__init__.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-16 17:02:37.765633 swane-0.0.5/swane/nipype_pipeline/engine/
--rw-rw-r--   0 mau       (1000) mau       (1000)     7906 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/engine/CustomWorkflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2795 2023-04-16 08:37:06.000000 swane-0.0.5/swane/nipype_pipeline/engine/MonitoredMultiProcPlugin.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      405 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/engine/NodeListEntry.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.5/swane/nipype_pipeline/engine/__init__.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-16 17:02:37.773633 swane-0.0.5/swane/nipype_pipeline/nodes/
--rw-rw-r--   0 mau       (1000) mau       (1000)     2537 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/AsymmetryIndex.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2263 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/CustomBEDPOSTX5.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1245 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/CustomDcm2niix.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      489 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/CustomDilateImage.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      661 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/CustomLabel2Vol.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      923 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/CustomProbTrackX2.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2356 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/CustomSliceTimer.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2737 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/DOmapOutliersMask.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2437 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/DeleteVolumes.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     4520 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/FMRIGenSpec.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2506 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/ForceOrient.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      458 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/FslCluster.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1600 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/FslNVols.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1601 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/GetNiftiTR.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1650 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/MergeTargets.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1849 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/Orient.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1400 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/RandomSeedGenerator.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2741 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/SegmentHA.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     3247 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/SumMultiTracks.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     3025 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/ThrROI.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2378 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/VenousCheck.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2703 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/Zscore.py
--rw-rw-r--   0 mau       (1000) mau       (1000)       25 2023-03-29 17:07:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/__init__.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      178 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/utils.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-16 17:02:37.777633 swane-0.0.5/swane/nipype_pipeline/workflows/
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.5/swane/nipype_pipeline/workflows/__init__.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    13690 2023-03-31 12:25:20.000000 swane-0.0.5/swane/nipype_pipeline/workflows/domap_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     7922 2023-04-04 03:17:58.000000 swane-0.0.5/swane/nipype_pipeline/workflows/dti_preproc_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     7690 2023-04-01 08:02:25.000000 swane-0.0.5/swane/nipype_pipeline/workflows/freesurfer_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    10956 2023-04-04 03:17:58.000000 swane-0.0.5/swane/nipype_pipeline/workflows/func_map_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     3504 2023-04-02 08:01:53.000000 swane-0.0.5/swane/nipype_pipeline/workflows/linear_reg_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     3142 2023-03-29 20:08:41.000000 swane-0.0.5/swane/nipype_pipeline/workflows/nonlinear_reg_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2180 2023-04-02 07:46:38.000000 swane-0.0.5/swane/nipype_pipeline/workflows/ref_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    19603 2023-04-02 08:03:23.000000 swane-0.0.5/swane/nipype_pipeline/workflows/task_fMRI_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    13745 2023-04-01 08:02:25.000000 swane-0.0.5/swane/nipype_pipeline/workflows/tractography_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     6335 2023-04-02 08:03:52.000000 swane-0.0.5/swane/nipype_pipeline/workflows/venous_workflow.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-16 17:02:37.777633 swane-0.0.5/swane/slicer/
--rw-rw-r--   0 mau       (1000) mau       (1000)     1930 2023-04-15 15:05:28.000000 swane-0.0.5/swane/slicer/SlicerCheckWorker.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1331 2023-04-15 15:05:28.000000 swane-0.0.5/swane/slicer/SlicerExportWorker.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.5/swane/slicer/__init__.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      302 2023-04-15 15:05:28.000000 swane-0.0.5/swane/slicer/slicer_script_freesurfer_module_check.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    11931 2023-04-15 15:05:28.000000 swane-0.0.5/swane/slicer/slicer_script_result.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    12030 2023-04-15 15:05:28.000000 swane-0.0.5/swane/strings.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-16 17:02:37.777633 swane-0.0.5/swane/ui/
--rw-rw-r--   0 mau       (1000) mau       (1000)     1378 2023-03-31 12:13:49.000000 swane-0.0.5/swane/ui/CustomTreeWidgetItem.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    18206 2023-04-05 07:58:18.000000 swane-0.0.5/swane/ui/MainWindow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      844 2023-03-29 17:07:54.000000 swane-0.0.5/swane/ui/PersistentProgressDialog.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    19160 2023-03-29 20:42:46.000000 swane-0.0.5/swane/ui/PreferencesWindow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    33778 2023-04-16 08:37:06.000000 swane-0.0.5/swane/ui/PtTab.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1001 2023-03-29 17:07:54.000000 swane-0.0.5/swane/ui/VerticalScrollArea.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.5/swane/ui/__init__.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-16 17:02:37.781633 swane-0.0.5/swane/ui/workers/
--rw-rw-r--   0 mau       (1000) mau       (1000)     4152 2023-03-29 17:07:54.000000 swane-0.0.5/swane/ui/workers/DicomSearchWorker.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      725 2023-03-29 17:07:54.000000 swane-0.0.5/swane/ui/workers/WorkflowGeneratorWorker.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      631 2023-03-29 17:07:54.000000 swane-0.0.5/swane/ui/workers/WorkflowMonitorWorker.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     3829 2023-04-16 08:37:06.000000 swane-0.0.5/swane/ui/workers/WorkflowProcess.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.5/swane/ui/workers/__init__.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-16 17:02:37.781633 swane-0.0.5/swane/utils/
--rw-rw-r--   0 mau       (1000) mau       (1000)     9139 2023-03-30 16:32:11.000000 swane-0.0.5/swane/utils/ConfigManager.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2514 2023-03-30 17:00:25.000000 swane-0.0.5/swane/utils/DataInput.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     5568 2023-03-29 17:07:54.000000 swane-0.0.5/swane/utils/PreferenceEntry.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.5/swane/utils/__init__.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1749 2023-03-29 17:07:54.000000 swane-0.0.5/swane/utils/check_dependency.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     3267 2023-03-29 17:07:54.000000 swane-0.0.5/swane/utils/fsl_conflict_handler.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     4385 2023-04-11 10:17:10.000000 swane-0.0.5/swane/utils/shortcut_manager.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-16 17:02:37.765633 swane-0.0.5/swane.egg-info/
--rw-rw-r--   0 mau       (1000) mau       (1000)      427 2023-04-16 17:02:37.000000 swane-0.0.5/swane.egg-info/PKG-INFO
--rw-rw-r--   0 mau       (1000) mau       (1000)     2939 2023-04-16 17:02:37.000000 swane-0.0.5/swane.egg-info/SOURCES.txt
--rw-rw-r--   0 mau       (1000) mau       (1000)        1 2023-04-16 17:02:37.000000 swane-0.0.5/swane.egg-info/dependency_links.txt
--rw-rw-r--   0 mau       (1000) mau       (1000)       42 2023-04-16 17:02:37.000000 swane-0.0.5/swane.egg-info/entry_points.txt
--rw-rw-r--   0 mau       (1000) mau       (1000)      109 2023-04-16 17:02:37.000000 swane-0.0.5/swane.egg-info/requires.txt
--rw-rw-r--   0 mau       (1000) mau       (1000)        6 2023-04-16 17:02:37.000000 swane-0.0.5/swane.egg-info/top_level.txt
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-08-07 15:05:13.622750 swane-0.0.6/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1976 2023-03-29 17:07:54.000000 swane-0.0.6/LICENSE
+-rw-rw-r--   0 mau       (1000) mau       (1000)      184 2023-03-29 17:07:54.000000 swane-0.0.6/MANIFEST.in
+-rw-rw-r--   0 mau       (1000) mau       (1000)      427 2023-08-07 15:05:13.622750 swane-0.0.6/PKG-INFO
+-rw-rw-r--   0 mau       (1000) mau       (1000)     7360 2023-08-07 13:21:41.000000 swane-0.0.6/README.md
+-rw-rw-r--   0 mau       (1000) mau       (1000)       38 2023-08-07 15:05:13.626750 swane-0.0.6/setup.cfg
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1258 2023-08-07 15:03:55.000000 swane-0.0.6/setup.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-08-07 15:05:13.618750 swane-0.0.6/swane/
+-rw-rw-r--   0 mau       (1000) mau       (1000)       46 2023-08-07 15:05:08.000000 swane-0.0.6/swane/__init__.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2068 2023-04-29 14:28:42.000000 swane-0.0.6/swane/__main__.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-08-07 15:05:13.618750 swane-0.0.6/swane/nipype_pipeline/
+-rw-rw-r--   0 mau       (1000) mau       (1000)    18907 2023-08-07 13:21:41.000000 swane-0.0.6/swane/nipype_pipeline/MainWorkflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.6/swane/nipype_pipeline/__init__.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-08-07 15:05:13.618750 swane-0.0.6/swane/nipype_pipeline/engine/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     7906 2023-06-11 04:41:26.000000 swane-0.0.6/swane/nipype_pipeline/engine/CustomWorkflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2795 2023-04-16 08:37:06.000000 swane-0.0.6/swane/nipype_pipeline/engine/MonitoredMultiProcPlugin.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      405 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/engine/NodeListEntry.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.6/swane/nipype_pipeline/engine/__init__.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-08-07 15:05:13.622750 swane-0.0.6/swane/nipype_pipeline/nodes/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2537 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/AsymmetryIndex.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2263 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/CustomBEDPOSTX5.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1477 2023-06-12 13:39:18.000000 swane-0.0.6/swane/nipype_pipeline/nodes/CustomDcm2niix.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      489 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/CustomDilateImage.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      661 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/CustomLabel2Vol.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      923 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/CustomProbTrackX2.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2356 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/CustomSliceTimer.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2437 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/DeleteVolumes.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2737 2023-08-07 13:21:41.000000 swane-0.0.6/swane/nipype_pipeline/nodes/FLAT1OutliersMask.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     4520 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/FMRIGenSpec.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2506 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/ForceOrient.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      458 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/FslCluster.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1600 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/FslNVols.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1601 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/GetNiftiTR.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1650 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/MergeTargets.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1849 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/Orient.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1400 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/RandomSeedGenerator.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2741 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/SegmentHA.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3247 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/SumMultiTracks.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1292 2023-05-29 14:38:12.000000 swane-0.0.6/swane/nipype_pipeline/nodes/SumMultiVols.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1580 2023-05-29 14:38:12.000000 swane-0.0.6/swane/nipype_pipeline/nodes/TTest.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3025 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/ThrROI.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2378 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/VenousCheck.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2703 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/Zscore.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)       25 2023-03-29 17:07:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/__init__.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      178 2023-04-06 16:01:54.000000 swane-0.0.6/swane/nipype_pipeline/nodes/utils.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-08-07 15:05:13.622750 swane-0.0.6/swane/nipype_pipeline/workflows/
+-rw-rw-r--   0 mau       (1000) mau       (1000)    14190 2023-08-07 13:21:41.000000 swane-0.0.6/swane/nipype_pipeline/workflows/FLAT1_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.6/swane/nipype_pipeline/workflows/__init__.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     7912 2023-08-07 13:21:41.000000 swane-0.0.6/swane/nipype_pipeline/workflows/dti_preproc_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    11783 2023-05-29 14:38:12.000000 swane-0.0.6/swane/nipype_pipeline/workflows/freesurfer_asymmetry_index_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     8381 2023-05-29 06:41:18.000000 swane-0.0.6/swane/nipype_pipeline/workflows/freesurfer_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    10956 2023-04-04 03:17:58.000000 swane-0.0.6/swane/nipype_pipeline/workflows/func_map_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3504 2023-04-02 08:01:53.000000 swane-0.0.6/swane/nipype_pipeline/workflows/linear_reg_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3132 2023-08-07 13:21:41.000000 swane-0.0.6/swane/nipype_pipeline/workflows/nonlinear_reg_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2180 2023-04-02 07:46:38.000000 swane-0.0.6/swane/nipype_pipeline/workflows/ref_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    19604 2023-07-13 09:03:26.000000 swane-0.0.6/swane/nipype_pipeline/workflows/task_fMRI_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    13725 2023-08-07 13:21:41.000000 swane-0.0.6/swane/nipype_pipeline/workflows/tractography_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     6335 2023-04-02 08:03:52.000000 swane-0.0.6/swane/nipype_pipeline/workflows/venous_workflow.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-08-07 15:05:13.622750 swane-0.0.6/swane/slicer/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2971 2023-05-19 05:29:53.000000 swane-0.0.6/swane/slicer/SlicerCheckWorker.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1331 2023-04-15 15:05:28.000000 swane-0.0.6/swane/slicer/SlicerExportWorker.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.6/swane/slicer/__init__.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      302 2023-04-15 15:05:28.000000 swane-0.0.6/swane/slicer/slicer_script_freesurfer_module_check.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    12647 2023-08-07 13:21:41.000000 swane-0.0.6/swane/slicer/slicer_script_result.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    12511 2023-08-07 13:21:41.000000 swane-0.0.6/swane/strings.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-08-07 15:05:13.622750 swane-0.0.6/swane/ui/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2309 2023-05-11 14:49:48.000000 swane-0.0.6/swane/ui/CustomTreeWidgetItem.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    25003 2023-08-07 14:58:34.000000 swane-0.0.6/swane/ui/MainWindow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      950 2023-05-19 04:43:57.000000 swane-0.0.6/swane/ui/PersistentProgressDialog.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    19245 2023-08-07 13:21:41.000000 swane-0.0.6/swane/ui/PreferencesWindow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    43097 2023-08-07 14:11:31.000000 swane-0.0.6/swane/ui/PtTab.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1119 2023-05-19 04:43:57.000000 swane-0.0.6/swane/ui/VerticalScrollArea.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.6/swane/ui/__init__.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-08-07 15:05:13.622750 swane-0.0.6/swane/ui/workers/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     4152 2023-03-29 17:07:54.000000 swane-0.0.6/swane/ui/workers/DicomSearchWorker.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      725 2023-03-29 17:07:54.000000 swane-0.0.6/swane/ui/workers/WorkflowGeneratorWorker.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      631 2023-03-29 17:07:54.000000 swane-0.0.6/swane/ui/workers/WorkflowMonitorWorker.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3829 2023-04-16 08:37:06.000000 swane-0.0.6/swane/ui/workers/WorkflowProcess.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.6/swane/ui/workers/__init__.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-08-07 15:05:13.622750 swane-0.0.6/swane/utils/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     9139 2023-08-07 13:21:41.000000 swane-0.0.6/swane/utils/ConfigManager.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     4390 2023-08-07 13:21:41.000000 swane-0.0.6/swane/utils/DataInput.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     5698 2023-05-19 04:55:32.000000 swane-0.0.6/swane/utils/PreferenceEntry.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.6/swane/utils/__init__.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1749 2023-03-29 17:07:54.000000 swane-0.0.6/swane/utils/check_dependency.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3267 2023-03-29 17:07:54.000000 swane-0.0.6/swane/utils/fsl_conflict_handler.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1429 2023-08-07 14:10:46.000000 swane-0.0.6/swane/utils/print_error.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     4385 2023-04-11 10:17:10.000000 swane-0.0.6/swane/utils/shortcut_manager.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-08-07 15:05:13.618750 swane-0.0.6/swane.egg-info/
+-rw-rw-r--   0 mau       (1000) mau       (1000)      427 2023-08-07 15:05:13.000000 swane-0.0.6/swane.egg-info/PKG-INFO
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3118 2023-08-07 15:05:13.000000 swane-0.0.6/swane.egg-info/SOURCES.txt
+-rw-rw-r--   0 mau       (1000) mau       (1000)        1 2023-08-07 15:05:13.000000 swane-0.0.6/swane.egg-info/dependency_links.txt
+-rw-rw-r--   0 mau       (1000) mau       (1000)       42 2023-08-07 15:05:13.000000 swane-0.0.6/swane.egg-info/entry_points.txt
+-rw-rw-r--   0 mau       (1000) mau       (1000)      165 2023-08-07 15:05:13.000000 swane-0.0.6/swane.egg-info/requires.txt
+-rw-rw-r--   0 mau       (1000) mau       (1000)        6 2023-08-07 15:05:13.000000 swane-0.0.6/swane.egg-info/top_level.txt
```

### Comparing `swane-0.0.5/LICENSE` & `swane-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/setup.py` & `swane-0.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,23 +20,23 @@
           "License :: OSI Approved :: MIT License",
           "Operating System :: MacOS",
           "Operating System :: POSIX :: Linux",
       ],
       license='MIT',
       install_requires=[
           "networkx<3",
-          "nipype",
-          "Pyside6",
-          "pydicom",
-          "configparser",
-          "psutil",
-          "pyshortcuts",
+          "nipype==1.8.6",
+          "Pyside6==6.4.3",
+          "pydicom==2.3.1",
+          "configparser==5.3.0",
+          "psutil==5.9.4",
+          "pyshortcuts==1.8.3",
           "swane_supplement>=0.1.2",
-          "matplotlib",
-          "nibabel"
+          "matplotlib==3.5.2",
+          "nibabel==5.0.0"
       ],
       python_requires=">=3.7",
       entry_points={
           'gui_scripts': [
               "swane = swane.__main__:main"
           ]
       }
```

### Comparing `swane-0.0.5/swane/__main__.py` & `swane-0.0.6/swane/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,48 +9,53 @@
     import swane_supplement
     from PySide6.QtWidgets import QApplication, QMessageBox
     from PySide6.QtGui import QIcon, QPixmap
     from swane.ui.MainWindow import MainWindow
     from swane.utils.ConfigManager import ConfigManager
     from swane import EXIT_CODE_REBOOT
 
+    # Exit Code definition for automatic reboot
     current_exit_code = EXIT_CODE_REBOOT
 
     while current_exit_code == EXIT_CODE_REBOOT:
-
+        
+        # Singleton for SWANe application
         if not QApplication.instance():
             app = QApplication(sys.argv)
         else:
             app = QApplication.instance()
 
+        # SWANe Icon definition
         app.setWindowIcon(QIcon(QPixmap(swane_supplement.appIcon_file)))
+        # SWANe App Name definition
         app.setApplicationDisplayName(strings.APPNAME)
-
+        
+        # SWANe Configuration loading
         global_config = ConfigManager()
 
-        # single instance check
+        # Guard to prevent multiple SWANe instances launch
         last_pid = global_config.getint('MAIN', 'lastPID')
         if last_pid != os.getpid():
             try:
                 psutil.Process(last_pid)
                 msg_box = QMessageBox()
-                msg_box.setText("Another instance of " + strings.APPNAME + " is already running!")
+                msg_box.setText(strings.main_multiple_instances_error)
                 msg_box.exec()
                 break
 
             except (psutil.NoSuchProcess, ValueError):
                 global_config['MAIN']['lastPID'] = str(os.getpid())
                 global_config.save()
 
-        # save MainWindow in a var to keep in memory and prevent crash
+        # MainWindow in a varariable to prenvent garbage collector deletion (might cause crash)
         widget = MainWindow(global_config)
         widget.setWindowIcon(QIcon(QPixmap(swane_supplement.appIcon_file)))
         current_exit_code = app.exec()
 
     sys.exit(current_exit_code)
 
 
 if __name__ == "__main__":
 
-    # before gui execution check for fsl/python/freesurfer error
+    # Before GUI execution check for fsl/python/freesurfer error
     if fsl_conflict_check():
         main()
```

### Comparing `swane-0.0.5/swane/nipype_pipeline/MainWorkflow.py` & `swane-0.0.6/swane/nipype_pipeline/MainWorkflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from swane.nipype_pipeline.engine.CustomWorkflow import CustomWorkflow
 
 from swane.nipype_pipeline.workflows.linear_reg_workflow import linear_reg_workflow
 from swane.nipype_pipeline.workflows.task_fMRI_workflow import task_fMRI_workflow
 from swane.nipype_pipeline.workflows.nonlinear_reg_workflow import nonlinear_reg_workflow
 from swane.nipype_pipeline.workflows.ref_workflow import ref_workflow
 from swane.nipype_pipeline.workflows.freesurfer_workflow import freesurfer_workflow
-from swane.nipype_pipeline.workflows.domap_workflow import domap_workflow
+from swane.nipype_pipeline.workflows.FLAT1_workflow import FLAT1_workflow
 from swane.nipype_pipeline.workflows.func_map_workflow import func_map_workflow
 from swane.nipype_pipeline.workflows.venous_workflow import venous_workflow
 from swane.nipype_pipeline.workflows.dti_preproc_workflow import dti_preproc_workflow
 from swane.nipype_pipeline.workflows.tractography_workflow import tractography_workflow, SIDES
 
 
 DEBUG = False
@@ -49,16 +49,16 @@
         
         if not data_input_list.is_ref_loaded:
             return
 
         # Check for FreeSurfer requirement and request
         is_freesurfer = pt_config.is_freesurfer() and pt_config.get_pt_wf_freesurfer()
         is_hippo_amyg_labels = pt_config.is_freesurfer_matlab() and pt_config.get_pt_wf_hippo()
-        # Check for DOMap requirement and request
-        is_domap = pt_config.getboolean('WF_OPTION', 'DOmap') and data_input_list[DataInputList.FLAIR3D].loaded
+        # Check for FLAT1 requirement and request
+        is_FLAT1 = pt_config.getboolean('WF_OPTION', 'FLAT1') and data_input_list[DataInputList.FLAIR3D].loaded
         # Check for Asymmetry Index request
         is_ai = pt_config.getboolean('WF_OPTION', 'ai')
         # Check for Tractography request
         is_tractography = pt_config.getboolean('WF_OPTION', 'tractography')
 
         # Core management
         self.max_cpu = global_config.getint('MAIN', 'maxPtCPU')
@@ -115,36 +115,36 @@
             flair_inputnode.inputs.frac = 0.5
             flair_inputnode.inputs.crop = True
             flair_inputnode.inputs.output_name = "r-flair_brain.nii.gz"
             self.connect(t1, "outputnode.ref_brain", flair, "inputnode.reference")
 
             flair.sink_result(self.base_dir, "outputnode", 'registered_file', self.SCENE_DIR)
 
-        if is_domap:
-            # Non linear registration to MNI1mm Atlas for DOmap
+        if is_FLAT1:
+            # Non linear registration to MNI1mm Atlas for FLAT1
             mni1 = nonlinear_reg_workflow("mni1")
             mni1.long_name = "MNI atlas registration"
 
             mni1_inputnode = mni1.get_node("inputnode")
             mni1_path = abspath(os.path.join(os.environ["FSLDIR"], 'data/standard/MNI152_T1_1mm_brain.nii.gz'))
             mni1_inputnode.inputs.atlas = mni1_path
             self.connect(t1, "outputnode.ref_brain", mni1, "inputnode.in_file")
 
-            # DOmap analysis
-            domap = domap_workflow("DOmap", mni1_path)
-            domap.long_name = "DOmap analysis"
-
-            self.connect(t1, "outputnode.ref_brain", domap, "inputnode.ref_brain")
-            self.connect(flair, "outputnode.registered_file", domap, "inputnode.flair_brain")
-            self.connect(mni1, "outputnode.fieldcoeff_file", domap, "inputnode.ref_2_mni1_warp")
-            self.connect(mni1, "outputnode.inverse_warp", domap, "inputnode.ref_2_mni1_inverse_warp")
-
-            domap.sink_result(self.base_dir, "outputnode", "extension_z", self.SCENE_DIR)
-            domap.sink_result(self.base_dir, "outputnode", "junction_z", self.SCENE_DIR)
-            domap.sink_result(self.base_dir, "outputnode", "binary_flair", self.SCENE_DIR)
+            # FLAT1 analysis
+            FLAT1 = FLAT1_workflow("FLAT1", mni1_path)
+            FLAT1.long_name = "FLAT1 analysis"
+
+            self.connect(t1, "outputnode.ref_brain", FLAT1, "inputnode.ref_brain")
+            self.connect(flair, "outputnode.registered_file", FLAT1, "inputnode.flair_brain")
+            self.connect(mni1, "outputnode.fieldcoeff_file", FLAT1, "inputnode.ref_2_mni1_warp")
+            self.connect(mni1, "outputnode.inverse_warp", FLAT1, "inputnode.ref_2_mni1_inverse_warp")
+
+            FLAT1.sink_result(self.base_dir, "outputnode", "extension_z", self.SCENE_DIR)
+            FLAT1.sink_result(self.base_dir, "outputnode", "junction_z", self.SCENE_DIR)
+            FLAT1.sink_result(self.base_dir, "outputnode", "binary_flair", self.SCENE_DIR)
 
         for plane in DataInputList.PLANES:
             if DataInputList.FLAIR2D+'_%s' % plane in data_input_list and data_input_list[DataInputList.FLAIR2D+'_%s' % plane].loaded:
                 flair_dir = data_input_list.get_dicom_dir(DataInputList.FLAIR2D+'_%s' % plane)
                 flair2d = linear_reg_workflow(data_input_list[DataInputList.FLAIR2D+'_%s' % plane].wf_name, flair_dir, is_volumetric=False)
                 flair2d.long_name = "2D %s FLAIR analysis" % plane
                 self.add_nodes([flair2d])
@@ -222,14 +222,20 @@
 
                 pet.sink_result(self.base_dir, "outputnode", 'surf_lh', self.SCENE_DIR)
                 pet.sink_result(self.base_dir, "outputnode", 'surf_rh', self.SCENE_DIR)
                 pet.sink_result(self.base_dir, "outputnode", 'zscore', self.SCENE_DIR)
                 pet.sink_result(self.base_dir, "outputnode", 'zscore_surf_lh', self.SCENE_DIR)
                 pet.sink_result(self.base_dir, "outputnode", 'zscore_surf_rh', self.SCENE_DIR)
 
+                # TODO work in progress for segmentation based asymmetry study
+                # from swane.nipype_pipeline.workflows.freesurfer_asymmetry_index_workflow import freesurfer_asymmetry_index_workflow
+                # pet_ai = freesurfer_asymmetry_index_workflow(name="pet_ai")
+                # self.connect(pet, "outputnode.registered_file", pet_ai, "inputnode.in_file")
+                # self.connect(freesurfer, "outputnode.vol_label_file_nii", pet_ai, "inputnode.seg_file")
+
             if is_ai:
                 self.connect(sym, 'outputnode.fieldcoeff_file', pet, 'inputnode.ref_2_sym_warp')
                 self.connect(sym, 'outputnode.inverse_warp', pet, 'inputnode.ref_2_sym_invwarp')
 
                 pet.sink_result(self.base_dir, "outputnode", 'ai', self.SCENE_DIR)
 
                 if is_freesurfer:
```

### Comparing `swane-0.0.5/swane/nipype_pipeline/engine/CustomWorkflow.py` & `swane-0.0.6/swane/nipype_pipeline/engine/CustomWorkflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/nipype_pipeline/engine/MonitoredMultiProcPlugin.py` & `swane-0.0.6/swane/nipype_pipeline/engine/MonitoredMultiProcPlugin.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/nipype_pipeline/nodes/AsymmetryIndex.py` & `swane-0.0.6/swane/nipype_pipeline/nodes/AsymmetryIndex.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/nipype_pipeline/nodes/CustomBEDPOSTX5.py` & `swane-0.0.6/swane/nipype_pipeline/nodes/CustomBEDPOSTX5.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/nipype_pipeline/nodes/CustomDcm2niix.py` & `swane-0.0.6/swane/nipype_pipeline/nodes/CustomDcm2niix.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,8 +26,12 @@
 
     def _run_interface(self, runtime):
         self.inputs.args = "-w 1"
         runtime = super(CustomDcm2niix, self)._run_interface(runtime)
         if self.inputs.crop is True and len(self.output_files) > 0 and os.path.exists(self.output_files[0].replace(".nii.gz", "_Crop_1.nii.gz")):
             os.remove(self.output_files[0])
             os.rename(self.output_files[0].replace(".nii.gz", "_Crop_1.nii.gz"), self.output_files[0])
+            
+        # in mosaic conversion nipype misread dcm2niix output and generate a duplicate list of results
+        # next line remove duplicates from output files array
+        self.output_files = [*set(self.output_files)]
         return runtime
```

### Comparing `swane-0.0.5/swane/nipype_pipeline/nodes/CustomLabel2Vol.py` & `swane-0.0.6/swane/nipype_pipeline/nodes/CustomLabel2Vol.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/nipype_pipeline/nodes/CustomProbTrackX2.py` & `swane-0.0.6/swane/nipype_pipeline/nodes/CustomProbTrackX2.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/nipype_pipeline/nodes/CustomSliceTimer.py` & `swane-0.0.6/swane/nipype_pipeline/nodes/CustomSliceTimer.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/nipype_pipeline/nodes/DOmapOutliersMask.py` & `swane-0.0.6/swane/nipype_pipeline/nodes/FLAT1OutliersMask.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 import shutil
 from nipype.interfaces.fsl import (BinaryMaths, UnaryMaths, ImageStats, Threshold)
 from os.path import abspath
 import math
 from nipype.interfaces.base import (BaseInterface, BaseInterfaceInputSpec, TraitedSpec, File, isdefined)
 
 
-# nodo per rimozione outliers nel DOmap
+# nodo per rimozione outliers nel FLAT1
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterfaceInputSpec)  -*-
-class DOmapOutliersMaskInputSpec(BaseInterfaceInputSpec):
+class FLAT1OutliersMaskInputSpec(BaseInterfaceInputSpec):
     in_file = File(exists=True, mandatory=True, desc='the input image')
     mask_file = File(exists=True, mandatory=True, desc='the original mask image')
     out_file = File(desc='the output mask name')
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.TraitedSpec)  -*-
-class DOmapOutliersMaskOutputSpec(TraitedSpec):
+class FLAT1OutliersMaskOutputSpec(TraitedSpec):
     out_file = File(exists=True, desc='the output image')
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterface)  -*-
-class DOmapOutliersMask(BaseInterface):
+class FLAT1OutliersMask(BaseInterface):
     """
-    Creates a mask that can be used to remove the outliers in DOmap workflow.
+    Creates a mask that can be used to remove the outliers in FLAT1 workflow.
 
     """
     
-    input_spec = DOmapOutliersMaskInputSpec
-    output_spec = DOmapOutliersMaskOutputSpec
+    input_spec = FLAT1OutliersMaskInputSpec
+    output_spec = FLAT1OutliersMaskOutputSpec
 
     def _run_interface(self, runtime):
         self.inputs.out_file = self._gen_outfilename()
 
         mean = ImageStats()
         mean.inputs.in_file = self.inputs.in_file
         mean.inputs.op_string = "-M"
```

### Comparing `swane-0.0.5/swane/nipype_pipeline/nodes/DeleteVolumes.py` & `swane-0.0.6/swane/nipype_pipeline/nodes/DeleteVolumes.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/nipype_pipeline/nodes/FMRIGenSpec.py` & `swane-0.0.6/swane/nipype_pipeline/nodes/FMRIGenSpec.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/nipype_pipeline/nodes/ForceOrient.py` & `swane-0.0.6/swane/nipype_pipeline/nodes/ForceOrient.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/nipype_pipeline/nodes/FslNVols.py` & `swane-0.0.6/swane/nipype_pipeline/nodes/FslNVols.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/nipype_pipeline/nodes/GetNiftiTR.py` & `swane-0.0.6/swane/nipype_pipeline/nodes/GetNiftiTR.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/nipype_pipeline/nodes/MergeTargets.py` & `swane-0.0.6/swane/nipype_pipeline/nodes/MergeTargets.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/nipype_pipeline/nodes/Orient.py` & `swane-0.0.6/swane/nipype_pipeline/nodes/Orient.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/nipype_pipeline/nodes/RandomSeedGenerator.py` & `swane-0.0.6/swane/nipype_pipeline/nodes/RandomSeedGenerator.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/nipype_pipeline/nodes/SegmentHA.py` & `swane-0.0.6/swane/nipype_pipeline/nodes/SegmentHA.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/nipype_pipeline/nodes/SumMultiTracks.py` & `swane-0.0.6/swane/nipype_pipeline/nodes/SumMultiTracks.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/nipype_pipeline/nodes/ThrROI.py` & `swane-0.0.6/swane/nipype_pipeline/nodes/ThrROI.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/nipype_pipeline/nodes/VenousCheck.py` & `swane-0.0.6/swane/nipype_pipeline/nodes/VenousCheck.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/nipype_pipeline/nodes/Zscore.py` & `swane-0.0.6/swane/nipype_pipeline/nodes/Zscore.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/nipype_pipeline/workflows/domap_workflow.py` & `swane-0.0.6/swane/nipype_pipeline/workflows/FLAT1_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from nipype.interfaces.fsl import (ApplyWarp, ApplyMask, BinaryMaths, FAST, ImageStats, )
 from nipype.pipeline.engine import Node
 
 from swane.nipype_pipeline.nodes.utils import getn
 from swane.nipype_pipeline.engine.CustomWorkflow import CustomWorkflow
 from swane.nipype_pipeline.nodes.ThrROI import ThrROI
 from swane.nipype_pipeline.nodes.CustomDilateImage import CustomDilateImage
-from swane.nipype_pipeline.nodes.DOmapOutliersMask import DOmapOutliersMask
+from swane.nipype_pipeline.nodes.FLAT1OutliersMask import FLAT1OutliersMask
 
 from nipype.interfaces.utility import IdentityInterface
 
 
-def domap_workflow(name: str, mni1_dir: str, base_dir: str = "/")  -> CustomWorkflow:
+def FLAT1_workflow(name: str, mni1_dir: str, base_dir: str = "/")  -> CustomWorkflow:
     """
     Creation of a junction and extension z-score map based on T13D, FLAIR3D and
     a mean template.
 
     Parameters
     ----------
     name : str
@@ -36,22 +36,29 @@
         Nonlinear registration warp from T13D reference space to MNI1 atlas.
     ref_2_mni1_inverse_warp : path
         Nonlinear registration inverse warp from MNI1 atlas space to T13D reference.
         
     Returns
     -------
     workflow : CustomWorkflow
-        The domap workflow.
+        The FLAT1 workflow.
         
     Output Node Fields
     ----------
     extension_z : path
         Extension z-score map in T13D reference space.
+        Based on:
+        - Pascher et al. - Automated morphometric MRI analysis for the detection of PNH - Epilepsia 2013
     junction_z : path
         Junction z-score map in T13D reference space.
+        Based on:
+        - Huppertz et al. - Enhanced visualization of blurred gray-white matter junctions in focal cortical
+                            dysplasia by voxel-based 3D MRI analysis - Epilepsy Res 2005
+        - Huppertz et al. - Voxel-based 3D MRI analysis helps to detect subtle forms of subcortical band
+                            heterotopia - Epilepsia 2008
     binary_flair : path
         Divided image FLAIR/T13D.
 
     """
     
     workflow = CustomWorkflow(name=name, base_dir=base_dir)
 
@@ -110,15 +117,15 @@
     flair_div_ref = Node(BinaryMaths(), name="%s_flairDIVref" % name)
     flair_div_ref.long_name = "Flair/T1 normalization"
     flair_div_ref.inputs.operation = "div"
     workflow.connect(flair_2_mni1, "out_file", flair_div_ref, "in_file")
     workflow.connect(restore_2_mni1, "out_file", flair_div_ref, "operand_file")
 
     # NODE 7: Outliers removal from mask
-    outliers_mask = Node(DOmapOutliersMask(), name="%s_outliers_mask" % name)
+    outliers_mask = Node(FLAT1OutliersMask(), name="%s_outliers_mask" % name)
     outliers_mask.inputs.mask_file = swane_supplement.cortex_mas
     workflow.connect(flair_div_ref, "out_file", outliers_mask, "in_file")
 
     # NODE 8: Cerebellum removal from divided image
     cortex_mask = Node(ApplyMask(), name="%s_cortexMask" % name)
     cortex_mask.long_name = "outliers %s"
     workflow.connect(outliers_mask, "out_file", cortex_mask, "mask_file")
@@ -145,21 +152,21 @@
     # NODE 12: Mean calculation for white matter
     wm_mean = Node(ImageStats(), name="%s_wm_mean" % name)
     wm_mean.long_name = "White matter mean value calculation"
     wm_mean.inputs.op_string = "-M"
     workflow.connect(wm_mask, "out_file", wm_mean, "in_file")
 
     # TODO parametri per ora inutilizzati. Valutare in futuro la loro implementazione
-    # DOmap_gm_std = Node(ImageStats(), name="%s_gm_std")
-    # DOmap_gm_std.inputs.op_string="-S"
-    # workflow.connect(DOmap_gmMask,"out_file",DOmap_gm_std,"in_file")
-
-    # DOmap_wm_std = Node(ImageStats(), name="%s_wm_std")
-    # DOmap_wm_std.inputs.op_string="-S"
-    # workflow.connect(DOmap_wmMask,"out_file",DOmap_wm_std,"in_file")
+    # FLAT1_gm_std = Node(ImageStats(), name="%s_gm_std")
+    # FLAT1_gm_std.inputs.op_string="-S"
+    # workflow.connect(FLAT1_gmMask,"out_file",FLAT1_gm_std,"in_file")
+
+    # FLAT1_wm_std = Node(ImageStats(), name="%s_wm_std")
+    # FLAT1_wm_std.inputs.op_string="-S"
+    # workflow.connect(FLAT1_wmMask,"out_file",FLAT1_wm_std,"in_file")
 
     # NODE 13: Mask generation with values between mean white matter and mean gray matter values
     binary_flair = Node(ThrROI(), name='%s_binaryFLAIR' % name)
     binary_flair.long_name = "Mean based masking"
     binary_flair.inputs.out_file = "binary_flair.nii.gz"
     workflow.connect(cortex_mask, "out_file", binary_flair, "in_file")
     workflow.connect(gm_mean, "out_stat", binary_flair, "seg_val_max")
```

### Comparing `swane-0.0.5/swane/nipype_pipeline/workflows/dti_preproc_workflow.py` & `swane-0.0.6/swane/nipype_pipeline/workflows/dti_preproc_workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         mni_2_ref_flirt.inputs.cost = "corratio"
         mni_2_ref_flirt.inputs.out_matrix_file = "mni_2_ref.mat"
         mni_2_ref_flirt.inputs.in_file = mni_dir
         workflow.add_nodes([mni_2_ref_flirt])
         workflow.connect(inputnode, 'ref_brain', mni_2_ref_flirt, 'reference')
 
         # NODE 2: Nonlinear registration
-        mni_2_ref_fnirt = Node(FNIRT(), name='mni_2_ref_fnirt', mem_gb=7)
+        mni_2_ref_fnirt = Node(FNIRT(), name='mni_2_ref_fnirt')
         mni_2_ref_fnirt.long_name = "atlas %s to diffusion space"
         mni_2_ref_fnirt.inputs.fieldcoeff_file = True
         mni_2_ref_fnirt.inputs.in_file = mni_dir
         workflow.connect(mni_2_ref_flirt, "out_matrix_file", mni_2_ref_fnirt, "affine_file")
         workflow.connect(inputnode, 'ref_brain', mni_2_ref_fnirt, 'ref_file')
 
         # NODE 8: Bayesian estimation of diffusion parameters
```

### Comparing `swane-0.0.5/swane/nipype_pipeline/workflows/freesurfer_workflow.py` & `swane-0.0.6/swane/nipype_pipeline/workflows/freesurfer_workflow.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,26 +71,40 @@
     inputnode = Node(
         IdentityInterface(fields=['max_node_cpu', 'ref', 'subjects_dir']),
         name='inputnode')
     
     # Output Node
     outputnode = Node(
         IdentityInterface(fields=['subject_id', 'subjects_dir', 'bgtROI', 'wmROI',
-                                  'pial', 'white', 'vol_label_file', 'lh_hippoAmygLabels',
+                                  'pial', 'white', 'vol_label_file', 'vol_label_file_nii', 'lh_hippoAmygLabels',
                                   'rh_hippoAmygLabels']),
         name='outputnode')
 
+    def check_fov_dim(nifti):
+        import subprocess
+        for x in range(1, 4, 1):
+            cmd = "echo $( echo $(fslval " + nifti + " dim" + str(x) + ") \\* $(fslval " + nifti + " pixdim" + str(x) + ") | bc)"
+            output = subprocess.run(cmd, shell=True, stdout=subprocess.PIPE).stdout.decode('utf-8')
+            try:
+                fovdim = float(output)
+                if fovdim > 256:
+                    return "-cw256"
+            except:
+                pass
+        return ""
+
     # NODE 1: Freesurfer cortical reconstruction process
     reconAll = Node(ReconAll(), name='reconAll')
     reconAll.inputs.subject_id = FS_DIR
     reconAll.inputs.parallel = True
     reconAll.inputs.directive = 'all'
     workflow.add_nodes([reconAll])
     workflow.connect(inputnode, "max_node_cpu", reconAll, "openmp")
     workflow.connect(inputnode, "ref", reconAll, "T1_files")
+    workflow.connect(inputnode, ('ref', check_fov_dim), reconAll, 'flags')
     workflow.connect(inputnode, "subjects_dir", reconAll, "subjects_dir")
 
     # NODE 2: Aparcaseg linear transformation in reference space
     aparaseg2Volmgz = Node(CustomLabel2Vol(), name="aparaseg2Volmgz")
     aparaseg2Volmgz.long_name = "label %s to reference space"
     aparaseg2Volmgz.inputs.vol_label_file = "./r-aparc_aseg.mgz"
     workflow.connect(reconAll, "rawavg", aparaseg2Volmgz, "template_file")
@@ -102,14 +116,15 @@
     # NODE 3: Aparcaseg conversion mgz -> nifti
     aparaseg2Volnii = Node(CustomLabel2Vol(), name="aparaseg2Volnii")
     aparaseg2Volnii.long_name = "label Nifti conversion"
     aparaseg2Volnii.inputs.vol_label_file = "r-aparc_aseg.nii.gz"
     workflow.connect(reconAll, "rawavg", aparaseg2Volnii, "template_file")
     workflow.connect([(reconAll, aparaseg2Volnii, [(('aparc_aseg', getn, 0), 'reg_header')])])
     workflow.connect([(reconAll, aparaseg2Volnii, [(('aparc_aseg', getn, 0), 'seg_file')])])
+    workflow.connect(aparaseg2Volnii, "vol_label_file", outputnode, "vol_label_file_nii")
 
     # NODE 4: Left cerebral white matter binary ROI
     lhwmROI = Node(ThrROI(), name='lhwmROI')
     lhwmROI.long_name = "Lh white matter ROI"
     lhwmROI.inputs.seg_val_min = 2
     lhwmROI.inputs.seg_val_max = 2
     lhwmROI.inputs.out_file = "lhwmROI.nii.gz"
```

### Comparing `swane-0.0.5/swane/nipype_pipeline/workflows/func_map_workflow.py` & `swane-0.0.6/swane/nipype_pipeline/workflows/func_map_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/nipype_pipeline/workflows/linear_reg_workflow.py` & `swane-0.0.6/swane/nipype_pipeline/workflows/linear_reg_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/nipype_pipeline/workflows/nonlinear_reg_workflow.py` & `swane-0.0.6/swane/nipype_pipeline/workflows/nonlinear_reg_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     flirt.inputs.cost = "corratio"
     flirt.inputs.out_matrix_file = "ref_2_%s.mat" % name
     workflow.add_nodes([flirt])
     workflow.connect(inputnode, 'in_file', flirt, 'in_file')
     workflow.connect(inputnode, 'atlas', flirt, 'reference')
 
     # NODE 2: Nonlinear registration
-    fnirt = Node(FNIRT(), name='ref_2_%s_fnirt' % name, mem_gb=7)
+    fnirt = Node(FNIRT(), name='ref_2_%s_fnirt' % name)
     fnirt.long_name = "%s to atlas"
     fnirt.inputs.fieldcoeff_file = True
     workflow.connect(flirt, "out_matrix_file", fnirt, "affine_file")
     workflow.connect(inputnode, 'in_file', fnirt, 'in_file')
     workflow.connect(inputnode, 'atlas', fnirt, 'ref_file')
 
     # NODE 3: Inverse matrix
```

### Comparing `swane-0.0.5/swane/nipype_pipeline/workflows/ref_workflow.py` & `swane-0.0.6/swane/nipype_pipeline/workflows/ref_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/nipype_pipeline/workflows/task_fMRI_workflow.py` & `swane-0.0.6/swane/nipype_pipeline/workflows/task_fMRI_workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,15 +395,15 @@
         maskfunc4.inputs.suffix = '_mask'
         maskfunc4.inputs.op_string = '-mas'
         workflow.connect(results_select, 'zstat', maskfunc4, 'in_file')
         workflow.connect(dilatemask, 'out_file', maskfunc4, 'in_file2')
 
         # NODE 36: Perform clustering on statistical output
         cluster = Node(FslCluster(), name="%s_cluster_%d" % (name, cont))
-        cluster.long_name = "contrast " + str(cont) + " %"
+        cluster.long_name = "contrast " + str(cont) + " %s"
         cluster.inputs.threshold = 3.1
         cluster.inputs.connectivity = 26
         cluster.inputs.pthreshold = 0.05
         cluster.inputs.out_localmax_txt_file = True
 
         # Function to generate the name for the file of output cluster
         def cluster_file_name(contrasts, run_name, x):
```

### Comparing `swane-0.0.5/swane/nipype_pipeline/workflows/tractography_workflow.py` & `swane-0.0.6/swane/nipype_pipeline/workflows/tractography_workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         targets_bin.long_name = side + " target ROIs binarization"
         targets_bin.inputs.op_string = "-thr 0.1 -bin"
         targets_bin.inputs.out_data_type = "char"
         targets_bin.inputs.suffix = "_bin"
         workflow.connect(targets_2_ref, "out_file", targets_bin, "in_file")
         
         # NODE 10: Tractography
-        probtrackx = MapNode(CustomProbTrackX2(), name="probtrackx_%s_%s" % (name, side), iterfield=["rseed"], mem_gb=4)
+        probtrackx = MapNode(CustomProbTrackX2(), name="probtrackx_%s_%s" % (name, side), iterfield=["rseed"])
         probtrackx.long_name = side + " %s"
         probtrackx.inputs.n_samples = n_samples
         probtrackx.inputs.loop_check = True
         probtrackx.inputs.wayorder = is_wayorder
         probtrackx.inputs.rand_fib = 1
         probtrackx.inputs.sample_random_points = 1
         # TODO argomento --ompl che fa??
@@ -186,15 +186,15 @@
             workflow.connect(merge_targets, "out_file", probtrackx, "waypoints")
         else:
             workflow.connect(targets_bin, "out_file", probtrackx, "waypoints")
         
         # Check if inverted run is required in protocol
         if is_invert:
             # NODE 11: Inverted tractography
-            probtrackx_inverted = MapNode(CustomProbTrackX2(), name="probtrackx_inverted_%s_%s" % (name, side), iterfield=["rseed"], mem_gb=4)
+            probtrackx_inverted = MapNode(CustomProbTrackX2(), name="probtrackx_inverted_%s_%s" % (name, side), iterfield=["rseed"])
             probtrackx_inverted.long_name = side + " inverse %s"
             probtrackx_inverted.inputs.n_samples = n_samples
             probtrackx_inverted.inputs.loop_check = True
             probtrackx_inverted.inputs.wayorder = is_wayorder
             probtrackx_inverted.inputs.rand_fib = 1
             probtrackx_inverted.inputs.sample_random_points = 1
             probtrackx_inverted.inputs.opd = True
```

### Comparing `swane-0.0.5/swane/nipype_pipeline/workflows/venous_workflow.py` & `swane-0.0.6/swane/nipype_pipeline/workflows/venous_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/slicer/SlicerExportWorker.py` & `swane-0.0.6/swane/slicer/SlicerExportWorker.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/slicer/slicer_script_result.py` & `swane-0.0.6/swane/slicer/slicer_script_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # slicerpython script for module checking
 # Warning: slicer library is not required beacuse the script is executed in Slicer environment
 
 import sys
 import os
 import subprocess
 
-def load_anat(scene_dir: str, volume_name: str):
+def load_anat(scene_dir: str, volume_name: str, color_node_ID: str = None):
     """
     Creates a scalar node from a NIFTI file.
 
     Parameters
     ----------
     scene_dir : str
         The scene directory.
     volume_name : str
         The NIFTI file name (without extension).
+    color_node_ID : str, optional
+        The colorNodeID to apply to Slicer node. The default is None.
 
     Returns
     -------
     node : MRMLCore.vtkMRMLScalarVolumeNode
         The scalar node generated from the NIFTI file.
 
     """
@@ -27,14 +29,18 @@
     node = None
     if os.path.exists(file):
         try:
             print("SLICERLOADER: Loading " + volume_name)
             node = slicer.util.loadVolume(file)
         except:
             pass
+
+        if node is not None and color_node_ID is not None:
+            node.GetDisplayNode().SetAndObserveColorNodeID(color_node_ID)
+            return
         
     return node
 
 
 def lesion_segment(scene_dir: str):
     """
     Prepares an empty segment for optional manual segmentation.
@@ -186,15 +192,15 @@
 
     overlays = ['pet_surf', 'pet_ai_surf', 'pet_zscore_surf', 'asl_surf', 'asl_ai_surf', 'asl_zscore_surf']
     for overlay in overlays:
         load_freesurfer_overlay(scene_dir, overlay + "_lh.mgz", lh_pial)
         load_freesurfer_overlay(scene_dir, overlay + "_rh.mgz", rh_pial)
 
 
-def load_vein(scene_dir: str, remove_vein: bool=False):
+def load_vein(scene_dir: str, remove_vein: bool = False):
     """
     Loads the veins files and creates their 3d model.
 
     Parameters
     ----------
     scene_dir : str
         The scene directory.
@@ -238,27 +244,27 @@
     my_storage_node.SetFileName(os.path.join(scene_dir, "veins.vtk"))
     my_storage_node.WriteData(vein_model)
     
     if remove_vein:
         slicer.mrmlScene.RemoveNode(vein_node)
 
 
-def tract_model(segmentation_node, dti_dir: str, tract: str, side: str):
+def tract_model(segmentation_node, dti_dir: str, tract: [], side: str):
     """
     Creates the 3d model of a tract.
 
     Parameters
     ----------
     #TODO verificare tipo
     segmentation_node : TYPE
         DESCRIPTION.
     dti_dir : str
         The DTI directory.
-    tract : str
-        The name of the tract.
+    tract : []
+        The array with the tract information.
     side : str
         The side of the tract:
             - LH for left side
             - RH for right side
 
     Returns
     -------
@@ -329,18 +335,15 @@
     
     fmri_path = os.path.join(scene_dir, "fMRI")
     if not os.path.exists(fmri_path):
         return
     print("SLICERLOADER: Loading fMRI")
     for file in os.listdir(fmri_path):
         if file.endswith('.nii.gz'):
-            func_node = load_anat(fmri_path, file.replace(".nii.gz", ""))
-            if func_node is not None:
-                func_node.GetDisplayNode().SetAndObserveColorNodeID('vtkMRMLPETProceduralColorNodePET-Rainbow2')
-
+            func_node = load_anat(fmri_path, file.replace(".nii.gz", ""), 'vtkMRMLPETProceduralColorNodePET-Rainbow2')
 
 def main_tract(dti_dir: str, scene_dir: str):
     sides = ["rh", "lh"]
     tracts = [
         {"name": "cst", "thr": "500", "color": [0, 1, 0]},
         {"name": "af", "thr": "1500", "color": [1, 0, 1]},
         {"name": "or", "thr": "500", "color": [1, 1, 0]}
@@ -375,21 +378,31 @@
 
         dtiDir = os.path.join(sceneDir, "dti")
         if os.path.isdir(dtiDir):
             main_tract(dtiDir, sceneDir)
 
         lesion_segment(sceneDir)
 
-        baseList = ['ref_brain', 'r-flair_brain', 'r-mdc_brain', 'r-pet', 'r-pet_ai', 'r-pet_zscore', 'r-asl',
-                    'r-asl_ai', 'r-asl_zscore', 'r-FA', 'r-flair2d_tra_brain', 'r-flair2d_cor_brain',
+        baseList = ['ref_brain', 'r-flair_brain', 'r-mdc_brain', 'r-FA', 'r-flair2d_tra_brain', 'r-flair2d_cor_brain',
                     'r-flair2d_sag_brain', 'r-binary_flair', 'r-junction_z', 'r-extension_z']
 
         for volume in baseList:
             load_anat(sceneDir, volume)
 
+        colorList = [('r-asl_ai', 'vtkMRMLColorTableNodeFileDivergingBlueRed.txt'),
+                     ('r-pet_ai', 'vtkMRMLColorTableNodeFileDivergingBlueRed.txt'),
+                     ('r-pet', 'vtkMRMLColorTableNodeFileColdToHotRainbow.txt'),
+                     ('r-pet_zscore', 'vtkMRMLColorTableNodeFileColdToHotRainbow.txt'),
+                     ('r-asl', 'vtkMRMLColorTableNodeFileColdToHotRainbow.txt'),
+                     ('r-asl_zscore', 'vtkMRMLColorTableNodeFileColdToHotRainbow.txt'),
+                     ]
+
+        for volume in colorList:
+            load_anat(sceneDir, volume[0], volume[1])
+
         load_fmri(sceneDir)
 
         load_vein(sceneDir)
 
         load_freesurfer(sceneDir, refNode)
 
         ext = "mrb"
```

### Comparing `swane-0.0.5/swane/strings.py` & `swane-0.0.6/swane/strings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,25 @@
+# General
 APPNAME = "SWANe"
 app_acronym = "Standardized Workflow for Advanced Neuroimaging in Epilepsy"
 EXECBUTTONTEXT = "Execute " + APPNAME + " Workflow"
 EXECBUTTONTEXT_STOP = "Stop " + APPNAME + " Workflow"
 GENBUTTONTEXT = "Generate " + APPNAME + " Workflow"
 PTCONFIGBUTTONTEXT = "Workflow preferences"
 
-mainwindow_chose_working_dir = "Choose the main working directory before start to use this application"
-mainwindow_chose_working_dir_title = 'Select the main working directory'
+# Main
+main_multiple_instances_error = "Another instance of " + APPNAME + " is already running!"
+
+# Main Window
+mainwindow_choose_working_dir = "Choose the main working directory before start to use this application"
+mainwindow_working_dir_space_error = "Blank spaces are not allowed in main working dir name or in its parent folder name"
+mainwindow_choose_working_dir_title = 'Select the main working directory'
 mainwindow_select_pt_folder = 'Select a patient folder'
 mainwindow_ptfolder_outside_workingdir_error = "The selected folder is not in " + APPNAME + " main working directory!"
+mainwindow_ptfolder_with_blank_spaces_error = "The selected folder name contains blank spaces!"
 mainwindow_pt_already_loaded_error = "The selected patient was already loaded in " + APPNAME + "!"
 mainwindow_invalid_folder_error = "The selected folder does not contains valid patient data!"
 mainwindow_force_dir_update = "If you are SURE you selected a patient folder, " + APPNAME + "can try to update " \
                               "it.\nDo you want to update selected patient folder?"
 mainwindow_max_pt_error = "Max patient tab limit reached!"
 mainwindow_new_pt_name = 'Write the name of the new patient:'
 mainwindow_new_pt_title = 'New patient'
@@ -35,31 +42,32 @@
 mainwindow_home_label5 = "\nExternal mandatory dependencies:"
 mainwindow_home_label6 = "\nExternal recommended dependencies:"
 mainwindow_home_label7 = "\nExternal optional dependencies:"
 
 mainwindow_dep_slicer_src = "Searching Slicer installation..."
 mainwindow_dep_slicer_found = "Slicer detected"
 mainwindow_pref_disabled_error = "Prefecences disabled during workflow execution!"
+aboutwindow_python_libs = "Python libraries dependencies: configparser, logging, matplotlib, nipype, pydicom, " \
+                          "pyshortcuts, PySide6, psutil"
 
+# Menu
 menu_load_pt = "Load existing patient"
 menu_load_pt_tip = "Load patient data from the main working directory"
 menu_new_pt = "Create new patient"
 menu_new_pt_tip = "Add a new patient in the main working directory"
 menu_exit = "Exit " + APPNAME
 menu_pref = "Preferences"
 menu_pref_tip = "Edit " + APPNAME + " preferences"
 menu_shortcut = "Toggle shortcuts"
 menu_about = "About " + APPNAME + "..."
 menu_file_name = "File"
 menu_tools_name = "Tools"
 menu_help_name = "Help"
 
-aboutwindow_python_libs = "Python libraries dependencies: configparser, logging, matplotlib, nipype, pydicom, " \
-                          "pyshortcuts, PySide6, psutil"
-
+# Patient Tab
 pttab_data_tab_name = "Data load"
 pttab_wf_tab_name = "Workflow execution"
 pttab_results_tab_name = "Results export"
 pttab_wf_executed = APPNAME + " Workflow executed!"
 pttab_wf_executed_with_error = APPNAME + " Workflow finished. Error occurred!"
 pttab_import_button = "Import"
 pttab_clear_button = "Clear"
@@ -74,74 +82,70 @@
 pttab_select_dicom_folder = 'Select a folder to scan for DICOM files'
 pttab_no_dicom_error = "No DICOM file in "
 pttab_multi_pt_error = "Dicom file from more than one patient in "
 pttab_multi_exam_error = "DICOM file from more than one examination in "
 pttab_multi_series_error = "DICOM file from more than one series in "
 pttab_missing_fsl_error = "FSL is required to generate " + APPNAME + " Workflow!"
 pttab_wf_gen_error = "Error generating the Workflow!"
-pttab_old_wf_found = "A previous execution of " + APPNAME + """ was detected. Do you want to resume execution or start 
-a new one?"""
+pttab_old_wf_found = "This patient has already been analyzed by " + APPNAME + """. Do you want to resume the previous analysis? If you want to delete all
+previous analyses and start over press NO, otherwise press YES"""
 pttab_old_wf_resume = "Resume execution"
 pttab_old_wf_reset = "New execution"
 pttab_old_fs_found = "An existing FreeSurfer folder was detected. Do you want to keep or delete the existing folder?"
 pttab_old_fs_resume = "Keep folder"
 pttab_old_fs_reset = "Delete folder"
 pttab_wf_stop = "Do you REALLY want to stop " + APPNAME + " Workflow execution?"
 pttab_results_button = "Export results into Slicer scene"
 pttab_exporting_start = "Exporting results into Slicer scene...\nLoading Slicer environment"
 pttab_exporting_prefix = "Exporting results into Slicer scene...\n"
 pttab_dicom_clearing = "Clearing DICOM files in: "
 pttab_wf_insufficient_resources = "Insufficient system resources (RAM or CPU) to execute workflows"
 
+# Preference Window
 pref_window_title_global = APPNAME + ' - Preferences'
 pref_window_title_user = ' - Workflow preferences'
-
 pref_window_global_box_title = "Global settings"
 pref_window_global_box_mwd = "Main working directory"
 pref_window_global_box_slicer = "3D Slicer path"
 pref_window_global_box_default_wf = "Default workflow"
 pref_window_global_box_default_task = "Default fMRI taks duration"
 pref_window_global_box_pt_limit = "Patient tab limit"
 pref_window_global_box_cpu_limit = "CPU per Patient limit"
 pref_window_global_box_default_ext = "Slicer scene extension"
-
 pref_window_global_box_optional_title = "Optional series settings"
-
 pref_window_wf_box_title = "Workflow settings"
-pref_window_wf_box_reconall = "FreeSurfer analisys"
+pref_window_wf_box_reconall = "FreeSurfer analysis"
 pref_window_wf_box_reconall_disabled_tip = "FreeSurfer not detected"
 pref_window_wf_box_hippo = "FreeSurfer hippocampal subfields"
 pref_window_wf_box_hippo_disabled_tip = "Matlab Runtime not detected"
 pref_window_wf_box_ai = "Asymmetry Index map for ASL and PET"
-pref_window_wf_box_domap = "DOmap analisys"
+pref_window_wf_box_FLAT1 = "FLAT1 analysis"
 pref_window_wf_box_tractography = "DTI tractography"
 pref_window_wf_box_missing_flair3d = "3D Flair missing"
 pref_window_wf_box_missing_dti = "DTI missing"
 pref_window_wf_box_missing_ai = "Asymmetry Index maps can be generated for PET or ASL data"
-
 pref_window_fmri_box_task_a_name = "Task A name"
 pref_window_fmri_box_task_b_name = "Task B name"
 pref_window_fmri_box_task_duration = "Task duration (sec)"
 pref_window_fmri_box_rest_duration = "Rest duration (sec)"
 pref_window_fmri_box_tr = "TR (sec)"
 pref_window_fmri_box_vols = "Number of EPI runs"
 pref_window_fmri_box_st = "Slice timing"
 pref_window_fmri_box_blockdesign = "Block design"
 pref_window_fmri_box_del_start_vols = "Delete start volumes"
 pref_window_fmri_box_del_end_vols = "Delete end volumes"
-
 pref_window_tract_box_title = "Tractography settings"
-
 pref_window_save_button = "Save preferences"
 pref_window_save_restart_button = "Save preferences (" + APPNAME + " will close and restart)"
 pref_window_discard_button = "Discard changes"
 pref_window_dir_error = "Directory does not exists!"
 pref_window_file_error = "File does not exists!"
 pref_window_select_slicer = "Select 3D Slicer executable"
 
+# Workflow
 check_dep_dcm2niix_error = "dcm2niix not detected (<a href='https://github.com/rordenlab/dcm2niix#Install" \
                            "'>installation info</a>)"
 check_dep_dcm2niix_found = "dcm2niix detected (%s)"
 check_dep_fsl_error = "FSL not detected (<a href='https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/FslInstallation" \
                       "'>installation info</a>)"
 check_dep_fsl_found = "FSL detected (%s)"
 check_dep_fs_found = "FreeSurfer detected (%s)"
@@ -168,14 +172,15 @@
                     " you can exit " + APPNAME + " and fix your configuration manually adding this line to your " \
                     "configuration file:"
 fsl_python_error_fix = "Fix error and Restart"
 fsl_python_error_restart = "Restart with system Python"
 fsl_python_error_exit = "Copy fix line and Exit"
 generic_shell_file = "your shell configuration"
 
+# Nodes
 node_names = {}
 node_names["CustomDcm2niix"] = "nifti conversion"
 node_names["ForceOrient"] = "standard orientation"
 node_names["BET"] = "scalp removal"
 node_names["FLIRT"] = "linear registration"
 node_names["ApplyXFM"] = "linear transformation"
 node_names["FNIRT"] = "nonlinear registration"
@@ -200,8 +205,8 @@
 node_names["Level1Design"] = "FEAT files generation"
 node_names["FEATModel"] = "design file generation"
 node_names["FILMGLS"] = "General-Linear-Model estimation"
 node_names["SmoothEstimate"] = "smoothness estimation"
 node_names["FslCluster"] = "cluster extraction"
 node_names["SampleToSurface"] = "surface projection"
 node_names["FAST"] = "Tissue segmentation"
-node_names["DOmapOutliersMask"] = "outliers mask generation"
+node_names["FLAT1OutliersMask"] = "outliers mask generation"
```

### Comparing `swane-0.0.5/swane/ui/CustomTreeWidgetItem.py` & `swane-0.0.6/swane/ui/CustomTreeWidgetItem.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,94 @@
 from PySide6.QtWidgets import QWidget, QLabel, QHBoxLayout, QTreeWidgetItem, QSpacerItem
 from PySide6.QtSvgWidgets import QSvgWidget
 
 
 class CustomTreeWidgetItem(QTreeWidgetItem):
+    """
+    Custom implementation of PySide QTreeWidgetItem to define the Workflows Tree items.
+
+    """
 
     def __init__(self, parent, tree, text, art=None):
         super(CustomTreeWidgetItem, self).__init__(parent)
         
         self.widget = QWidget()
         self.widget.setLayout(QHBoxLayout())
         self.artLabel = QSvgWidget()
         self.artLabel.setFixedWidth(26)
         self.artLabel.setFixedHeight(26)
-        self.setArt(art)
+        self.set_art(art)
         self.textLabel = QLabel(text)
         self.resize_text_label()
         
         self.widget.layout().addWidget(self.artLabel)
         self.widget.layout().addWidget(self.textLabel)
         self.widget.layout().addSpacerItem(QSpacerItem(25, 0))
 
         tree.setItemWidget(self, 0, self.widget)
         
         self.completed = False
         self.art = None
+
+    def setText(self, text: str):
+        """
+        Set the tree item text.
+
+        Parameters
+        ----------
+        text : str
+            The item text.
+
+        Returns
+        -------
+        None.
+
+        """
         
-    def setText(self, text):
         self.textLabel.setText(text)
         self.resize_text_label()
 
     def resize_text_label(self):
+        """
+        Resize the tree item label.
+        Allow the horizontal scroll when expanding subsection.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         self.textLabel.setMinimumWidth(self.textLabel.fontMetrics().boundingRect(self.textLabel.text()).width() + 10)
         
-    def getText(self):
+    def get_text(self) -> str:
+        """
+        Get the tree item text from its label.
+
+        Returns
+        -------
+        str
+            The item text.
+
+        """
+        
         return self.textLabel.text()
     
-    def setArt(self, art):
+    def set_art(self, art: str):
+        """
+        Set the icon of the tree item.
+
+        Parameters
+        ----------
+        art : str
+            The icon path of the tree item.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         self.art = art
+        
         if art is not None:
             self.artLabel.load(art)
```

### Comparing `swane-0.0.5/swane/ui/MainWindow.py` & `swane-0.0.6/swane/ui/MainWindow.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,65 @@
 from PySide6.QtWidgets import (QMainWindow, QMessageBox, QFileDialog, QInputDialog,
                                QLineEdit, QTabWidget, QGridLayout, QLabel, QSizePolicy,
                                QSpacerItem, QWidget, QTabBar, QDialog)
 from swane.utils.check_dependency import (check_dcm2niix, check_fsl, check_freesurfer,
                                           check_graphviz)
-from PySide6.QtGui import QAction, QIcon, QPixmap, QFont
+from PySide6.QtGui import QAction, QIcon, QPixmap, QFont, QCloseEvent
 from PySide6.QtCore import QCoreApplication, QThreadPool
 from PySide6.QtSvgWidgets import QSvgWidget
 import os
+import sys
 
 from swane.ui.PtTab import PtTab
 from swane.ui.PreferencesWindow import PreferencesWindow
 import swane_supplement
 from swane import __version__, EXIT_CODE_REBOOT, strings
 from swane.utils.DataInput import DataInputList
 from swane.utils.shortcut_manager import shortcut_manager
 from swane.slicer.SlicerCheckWorker import SlicerCheckWorker
 
 
 class MainWindow(QMainWindow):
-    ptDirPath = ""
-    tabWidget = None
+    """
+    Custom implementation of PySide QMainWindow to define SWANe GUI.
 
+    """
+       
     def __init__(self, global_config):
 
+        # GUI configuration setting
         self.global_config = global_config
-
+        
         super(MainWindow, self).__init__()
+        
+        # GUI Icons setting
         self.setWindowIcon(QIcon(QPixmap(swane_supplement.appIcon_file)))
-
         self.OK_ICON_FILE = swane_supplement.okIcon_file
         self.ERROR_ICON_FILE = swane_supplement.errorIcon_file
         self.WARNING_ICON_FILE = swane_supplement.warnIcon_file
         self.LOADING_MOVIE_FILE = swane_supplement.loadingMovie_file
         self.VOID_SVG_FILE = swane_supplement.voidsvg_file
-
         self.OK_ICON = QPixmap(self.OK_ICON_FILE)
         self.ERROR_ICON = QPixmap(self.ERROR_ICON_FILE)
         self.WARNING_ICON = QPixmap(self.WARNING_ICON_FILE)
 
+        # Patient folder configuration checking
         while self.global_config.get_patients_folder() == "" or not os.path.exists(
                 self.global_config.get_patients_folder()):
             msg_box = QMessageBox()
-            msg_box.setText(strings.mainwindow_chose_working_dir)
+            msg_box.setText(strings.mainwindow_choose_working_dir)
             msg_box.exec()
             self.set_patients_folder()
 
+        # Patient folder configuration setting
         os.chdir(self.global_config.get_patients_folder())
 
         self.initialize_ui()
 
-        # controllo che eventuali shortcut salvati esistano
+        # SWANe launching icon checking
         if self.global_config.get_shortcut_path() != '':
             targets = self.global_config.get_shortcut_path().split("|")
             new_path = ''
             change = False
             for fil in targets:
                 if strings.APPNAME in fil and os.path.exists(fil):
                     if new_path != '':
@@ -61,96 +67,171 @@
                     new_path = new_path + fil
                 else:
                     change = True
             if change:
                 self.global_config.set_shortcut_path(new_path)
                 self.global_config.save()
 
-    def open_pt_dir(self, folder_path):
+    def open_pt_dir(self, folder_path: str):
+        """
+        Load a checked and valid patient folder.
+
+        Parameters
+        ----------
+        folder_path : str
+            The patient folder path.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         this_tab = PtTab(self.global_config, folder_path,
                          self, parent=self.main_tab)
         this_tab.set_main_window(self)
         self.pt_tabs_array.append(this_tab)
 
         self.main_tab.addTab(this_tab, os.path.basename(folder_path))
         self.main_tab.setCurrentWidget(this_tab)
+        
         this_tab.load_pt()
 
-    def check_pt_limit(self):
+    def check_pt_limit(self) -> bool:
+        """
+        Check if SWANe can open another patient tab without overcome the limit set by configuration.
+
+        Returns
+        -------
+        bool
+            True if SWANe can load another tab, otherwise False.
+
+        """
+        
         max_pt = self.global_config.get_max_pt()
         if max_pt <= 0:
             return True
         if len(self.pt_tabs_array) >= max_pt:
             msg_box = QMessageBox()
             msg_box.setIcon(QMessageBox.Icon.Warning)
             msg_box.setText(strings.mainwindow_max_pt_error)
             msg_box.exec()
             return False
         return True
 
     def search_pt_dir(self):
+        """
+        Try to open a patient directory
+
+        Returns
+        -------
+        None.
+
+        """
+        
+        # Guard to avoid the opening of patient tabs greater than the maximum allowed
         if not self.check_pt_limit():
             return
 
+        # Open the directory selection dialog 
         file_dialog = QFileDialog()
         file_dialog.setDirectory(self.global_config.get_patients_folder())
         folder_path = file_dialog.getExistingDirectory(self, strings.mainwindow_select_pt_folder)
         if not os.path.exists(folder_path):
             return
 
+        # Guard to avoid the opening a directory containing blank spaces
+        if ' ' in folder_path:
+            msg_box = QMessageBox()
+            msg_box.setIcon(QMessageBox.Icon.Critical)
+            msg_box.setText(strings.mainwindow_ptfolder_with_blank_spaces_error)
+            msg_box.exec()
+            return
+
+
+        # Guard to avoid the opening of a directory outside the main patient folder
         if not os.path.abspath(folder_path).startswith(
                 os.path.abspath(self.global_config.get_patients_folder()) + os.sep):
             msg_box = QMessageBox()
             msg_box.setIcon(QMessageBox.Icon.Critical)
             msg_box.setText(strings.mainwindow_ptfolder_outside_workingdir_error)
             msg_box.exec()
             return
 
+        # Guard to avoid an already loaded patient directory
         for pt in self.pt_tabs_array:
             if pt.pt_folder == folder_path:
                 msg_box = QMessageBox()
                 msg_box.setIcon(QMessageBox.Icon.Warning)
                 msg_box.setText(strings.mainwindow_pt_already_loaded_error)
                 msg_box.exec()
                 return
 
+        # Check if selected folder is a valid patient folder
         if not self.check_pt_dir(folder_path):
             msg_box = QMessageBox()
             msg_box.setIcon(QMessageBox.Icon.Warning)
             msg_box.setText(strings.mainwindow_invalid_folder_error)
             msg_box.exec()
 
             msg_box2 = QMessageBox()
             msg_box2.setText(strings.mainwindow_force_dir_update)
             msg_box2.setIcon(QMessageBox.Icon.Question)
             msg_box2.setStandardButtons(QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No)
             msg_box2.button(QMessageBox.StandardButton.Yes).setText("Yes")
             msg_box2.button(QMessageBox.StandardButton.No).setText("No")
             msg_box2.setDefaultButton(QMessageBox.StandardButton.No)
             ret = msg_box2.exec()
+            
+            # A patient folder has a predefined folder tree.
+            # SWANe recognizes a patient folder checking its subfolders.
+            # If a selected folder is not valid, the user may force its conversion into a patient folder.
             if ret == QMessageBox.StandardButton.Yes:
                 self.update_pt_dir(folder_path)
             else:
                 return
+            
         self.open_pt_dir(folder_path)
 
-    def get_suggested_patient_name(self):
+    def get_suggested_patient_name(self) -> str:
+        """
+        Get a default name for the patient folder based the existing patient folders into the main patient directory.
+
+        Returns
+        -------
+        str
+            The suggested patient folder name.
+
+        """
+        
         import re
+        
         regex = re.compile('^' + self.global_config.get_patientsprefix() + '\d+$')
         file_list = []
+        
         for this_dir in os.listdir(self.global_config.get_patients_folder()):
             if regex.match(this_dir):
                 file_list.append(
                     int(this_dir.replace(self.global_config.get_patientsprefix(), "")))
 
         if len(file_list) == 0:
             return self.global_config.get_patientsprefix() + "1"
+        
         return self.global_config.get_patientsprefix() + str(max(file_list) + 1)
 
-    def chose_new_pt_dir(self):
+    def choose_new_pt_dir(self):
+        """
+        Create a new patient folder. The user must specify its name.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         if not self.check_pt_limit():
             return
 
         text, ok = QInputDialog.getText(self, strings.mainwindow_new_pt_title, strings.mainwindow_new_pt_name,
                                         QLineEdit.EchoMode.Normal, self.get_suggested_patient_name())
 
         if not ok:
@@ -166,25 +247,57 @@
 
         if os.path.exists(os.path.join(self.global_config.get_patients_folder(), pt_name)):
             msg_box = QMessageBox()
             msg_box.setText(strings.mainwindow_pt_exists_error + pt_name)
             msg_box.exec()
             return
 
-        self.create_new_pt_dir(pt_name)
+        self.create_new_pt_dir(pt_name.replace(" ", "_"))
 
     def set_patients_folder(self):
-        folder_path = QFileDialog.getExistingDirectory(self, strings.mainwindow_chose_working_dir_title)
+        """
+        Generates the OS directory selection dialog to set the default patient folder
+
+        Returns
+        -------
+        None.
+
+        """
+        
+        folder_path = QFileDialog.getExistingDirectory(self, strings.mainwindow_choose_working_dir_title)
+        
         if not os.path.exists(folder_path):
             return
+
+        if ' ' in folder_path:
+            msg_box = QMessageBox()
+            msg_box.setText(strings.mainwindow_working_dir_space_error)
+            msg_box.exec()
+            return
+        
         self.global_config.set_patients_folder(os.path.abspath(folder_path))
         self.global_config.save()
+        
         os.chdir(folder_path)
 
-    def create_new_pt_dir(self, pt_name):
+    def create_new_pt_dir(self, pt_name: str):
+        """
+        Create a new patient folder and subfolders.
+
+        Parameters
+        ----------
+        pt_name : str
+            The patient folder name.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         base_folder = os.path.abspath(os.path.join(
             self.global_config.get_patients_folder(), pt_name))
 
         dicom_folder = os.path.join(base_folder, self.global_config.get_default_dicom_folder())
 
         for data_input in DataInputList().values():
             os.makedirs(os.path.join(
@@ -192,51 +305,123 @@
 
         msg_box = QMessageBox()
         msg_box.setText(strings.mainwindow_new_pt_created + base_folder)
         msg_box.exec()
 
         self.open_pt_dir(base_folder)
 
-    def check_pt_dir(self, dir_path):
+    def check_pt_dir(self, dir_path: str) -> bool:
+        """
+        Check if a directory is a valid patient folder
+
+        Parameters
+        ----------
+        dir_path : str
+            The directory path to check.
+
+        Returns
+        -------
+        bool
+            True if the directory is a valid patient folder, otherwise False.
+
+        """
+        
         for data_input in DataInputList().values():
             if not os.path.exists(os.path.join(dir_path, self.global_config.get_default_dicom_folder(), data_input.name)):
                 return False
+            
         return True
 
-    def update_pt_dir(self, dir_path):
-        for folder in self.global_config.get_default_folders():
-            if not os.path.exists(os.path.join(dir_path, self.global_config.get_default_folders()[folder])):
-                os.makedirs(os.path.join(
-                    dir_path, self.global_config.get_default_folders()[folder]), exist_ok=True)
+    def update_pt_dir(self, dir_path: str):
+        """
+        Update an existing folder with the patient subfolder structure.
+
+        Parameters
+        ----------
+        dir_path : str
+            The directory path to update into a patient folder.
+
+        Returns
+        -------
+        None.
+
+        """
+
+        for data_input in DataInputList().values():
+            if not os.path.exists(
+                    os.path.join(dir_path, self.global_config.get_default_dicom_folder(), data_input.name)):
+                os.makedirs(os.path.join(dir_path, self.global_config.get_default_dicom_folder(), data_input.name),
+                            exist_ok=True)
 
     def edit_config(self):
+        """
+        Open the Global Preferences Window.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         if self.check_running_workflows():
             msg_box = QMessageBox()
             msg_box.setText(strings.mainwindow_pref_disabled_error)
             msg_box.exec()
             return
+        
         preference_window = PreferencesWindow(self.global_config, self)
         ret = preference_window.exec()
+        
         if ret == EXIT_CODE_REBOOT:
             self.close()
             QCoreApplication.exit(EXIT_CODE_REBOOT)
+            
         if ret != 0:
             self.reset_workflows()
 
-    def check_running_workflows(self):
+    def check_running_workflows(self) -> bool:
+        """
+        Check if SWANe is executing a workflow in any open Patients tab.
+
+        Returns
+        -------
+        bool
+            True if SWANe is executing a workflow, otherwise False.
+
+        """
+        
         for pt in self.pt_tabs_array:
             if pt.is_workflow_process_alive():
                 return True
+            
         return False
 
     def reset_workflows(self):
+        """
+        Reset all the generated workflows that are not already running.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         for pt in self.pt_tabs_array:
             pt.reset_workflow()
 
     def about(self):
+        """
+        Open the About Window.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         about_dialog = QDialog(parent=self)
         layout = QGridLayout()
 
         bold_font = QFont()
         bold_font.setBold(True)
         title_font = QFont()
         title_font.setBold(True)
@@ -261,101 +446,153 @@
 
         layout.addWidget(label_about_icon, 0, 0, 3, 1)
 
         about_dialog.setLayout(layout)
         about_dialog.exec()
 
     def initialize_ui(self):
+        """
+        Generates the SWANE GUI
+
+        Returns
+        -------
+        None.
+
+        """
+        
         self.resize(800, 600)
         self.setWindowTitle(strings.APPNAME + " - " + strings.app_acronym)
 
         self.statusBar().showMessage('')
 
+        # Buttons definition
         button_action = QAction(QIcon.fromTheme(
             "document-open"), strings.menu_load_pt, self)
         button_action.setStatusTip(strings.menu_load_pt_tip)
         button_action.triggered.connect(self.search_pt_dir)
 
         button_action2 = QAction(QIcon.fromTheme(
             "document-new"), strings.menu_new_pt, self)
         button_action2.setStatusTip(strings.menu_new_pt_tip)
-        button_action2.triggered.connect(self.chose_new_pt_dir)
+        button_action2.triggered.connect(self.choose_new_pt_dir)
 
         button_action3 = QAction(QIcon.fromTheme(
             "application-exit"), strings.menu_exit, self)
         button_action3.triggered.connect(self.close)
 
         button_action4 = QAction(QIcon.fromTheme(
             "preferences-other"), strings.menu_pref, self)
         button_action4.setStatusTip(strings.menu_pref_tip)
         button_action4.triggered.connect(self.edit_config)
 
         button_action6 = QAction(strings.menu_about, self)
         button_action6.triggered.connect(self.about)
 
+        # Menu definition and population
         menu = self.menuBar()
         menu.setNativeMenuBar(False)
         file_menu = menu.addMenu(strings.menu_file_name)
         file_menu.addAction(button_action)
         file_menu.addAction(button_action2)
         file_menu.addAction(button_action3)
         tool_menu = menu.addMenu(strings.menu_tools_name)
         tool_menu.addAction(button_action4)
-        button_action5 = QAction(strings.menu_shortcut, self)
-        button_action5.triggered.connect(lambda checked=None, global_config=self.global_config: shortcut_manager(global_config))
+        if sys.platform != "darwin":
+            button_action5 = QAction(strings.menu_shortcut, self)
+            button_action5.triggered.connect(lambda checked=None, global_config=self.global_config: shortcut_manager(global_config))
 
-        tool_menu.addAction(button_action5)
+            tool_menu.addAction(button_action5)
         help_menu = menu.addMenu(strings.menu_help_name)
         help_menu.addAction(button_action6)
-
+        
+        # Tab definition
         self.main_tab = QTabWidget(parent=self)
         self.main_tab.setTabsClosable(True)
         self.main_tab.tabCloseRequested.connect(self.close_pt)
         self.setCentralWidget(self.main_tab)
         self.homeTab = QWidget()
-
         self.main_tab.addTab(self.homeTab, strings.mainwindow_home_tab_name)
 
-        # rimozione tasto chiusura da tab home, a destra o sinistra in base allo stile
+        # Tab closing option disabled
         self.main_tab.tabBar().setTabButton(0, QTabBar.ButtonPosition.LeftSide, None)
         self.main_tab.tabBar().setTabButton(0, QTabBar.ButtonPosition.RightSide, None)
-
+        
+        # Home Tab definition
         self.home_tab_ui()
-
+        
         self.pt_tabs_array = []
 
         self.show()
 
-    def close_pt(self, index):
-        if index == -1:
+    def close_pt(self, index: int):
+        """
+        Handle the PySide tab closing event for the Patient tab.
+
+        Parameters
+        ----------
+        index : int
+            The patient tab index into the GUI.
+
+        Returns
+        -------
+        None.
+
+        """
+        
+        # Guard to prevent the Home Tab closing
+        if index <= 0:
             return
 
         tab_item = self.main_tab.widget(index)
         if tab_item.is_workflow_process_alive():
             msg_box = QMessageBox()
             msg_box.setText(strings.mainwindow_wf_executing_error_1)
             msg_box.exec()
             return
 
-        tab_item.close_routine()
+        tab_item.pt_config.save()
+        
         self.pt_tabs_array.remove(tab_item)
         self.main_tab.removeTab(index)
+        
         tab_item = None
 
-    def closeEvent(self, event):
-        # evito la chiusura se il wf è in esecuzione
+    def closeEvent(self, event: QCloseEvent):
+        """
+        Prevent the closing of a running workflow tab
+
+        Parameters
+        ----------
+        event : QCloseEvent
+            PySide QCloseEvent.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         if not self.check_running_workflows():
-            return super(MainWindow, self).closeEvent(event)
+            event.accept()
         else:
             msg_box = QMessageBox()
             msg_box.setText(strings.mainwindow_wf_executing_error_2)
             msg_box.exec()
             event.ignore()
 
     def home_tab_ui(self):
+        """
+        Generates the Home Tab layout
+
+        Returns
+        -------
+        None.
+
+        """
+        
         layout = QGridLayout()
 
         bold_font = QFont()
         bold_font.setBold(True)
         title_font = QFont()
         title_font.setBold(True)
         title_font.setPointSize(title_font.pointSize() * 1.5)
@@ -375,14 +612,15 @@
         layout.addWidget(label_welcome2, x, 0, 1, 2)
         x += 1
         layout.addWidget(label_welcome3, x, 0, 1, 2)
         x += 1
         layout.addWidget(label_welcome4, x, 0, 1, 2)
         x += 1
 
+        # Main window dependency check
         label_main_dep = QLabel(strings.mainwindow_home_label5)
         label_main_dep.setSizePolicy(QSizePolicy.Minimum, QSizePolicy.Minimum)
         label_main_dep.setFont(bold_font)
         layout.addWidget(label_main_dep, x, 0, 1, 2)
         x += 1
 
         msg, self.dcm2niix = check_dcm2niix()
@@ -396,28 +634,39 @@
         label_main_dep.setFont(bold_font)
         layout.addWidget(label_main_dep, x, 0, 1, 2)
         x += 1
 
         msg, self.freesurfer = check_freesurfer()
         x = self.add_home_entry(layout, msg, self.freesurfer[0], x)
 
-        if self.global_config.get_slicer_path() == '' or not os.path.exists(self.global_config.get_slicer_path()):
+        check_slicer = False
+        current_slicer_path = self.global_config.get_slicer_path()
+        if current_slicer_path == '':
+            check_slicer = True
+        elif current_slicer_path[0] == "*":
+            current_slicer_path = current_slicer_path[1:]
+            check_slicer = True
+
+        if not os.path.exists(current_slicer_path):
+            current_slicer_path = ''
+
+        if check_slicer:
             self.slicerlabel_icon = QSvgWidget()
             self.slicerlabel_icon.setFixedSize(25, 25)
             self.slicerlabel_icon.load(self.LOADING_MOVIE_FILE)
             layout.addWidget(self.slicerlabel_icon, x, 0)
             self.slicerlabel = QLabel(strings.mainwindow_dep_slicer_src)
             self.slicerlabel.setOpenExternalLinks(True)
             self.slicerlabel.setSizePolicy(
                 QSizePolicy.Minimum, QSizePolicy.Minimum)
             layout.addWidget(self.slicerlabel, x, 1)
             x += 1
 
             self.global_config.set_slicer_path('')
-            check_slicer_work = SlicerCheckWorker(parent=self)
+            check_slicer_work = SlicerCheckWorker(current_slicer_path, parent=self)
             check_slicer_work.signal.slicer.connect(self.slicer_row)
             QThreadPool.globalInstance().start(check_slicer_work)
         else:
             self.add_home_entry(layout, strings.mainwindow_dep_slicer_found, True, x)
         x += 1
 
         label_main_dep = QLabel(strings.mainwindow_home_label7)
@@ -431,30 +680,75 @@
 
         vertical_spacer = QSpacerItem(
             20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
         layout.addItem(vertical_spacer, x, 0, 1, 2)
 
         self.homeTab.setLayout(layout)
 
-    def add_home_entry(self, gridlayout, msg, icon, x):
+    def add_home_entry(self, gridlayout: QGridLayout, msg: str, icon: bool, x: int) -> int:
+        """
+        Generates a dependency check label, adding it to an existing layout
+
+        Parameters
+        ----------
+        gridlayout : QGridLayout
+            The layout to populate with the generated label.
+        msg : str
+            The label text.
+        icon : bool
+            The label check icon.
+        x : int
+            The starting grid layout row index.
+
+        Returns
+        -------
+        int
+            The next grid layout row index.
+
+        """
+        
         label_icon = QLabel()
         label_icon.setFixedSize(25, 25)
         label_icon.setScaledContents(True)
+        
         if icon:
             label_icon.setPixmap(self.OK_ICON)
         else:
             label_icon.setPixmap(self.ERROR_ICON)
+            
         gridlayout.addWidget(label_icon, x, 0)
         label = QLabel(msg)
         label.setOpenExternalLinks(True)
         label.setSizePolicy(QSizePolicy.Minimum, QSizePolicy.Minimum)
         gridlayout.addWidget(label, x, 1)
+        
         return x + 1
 
-    def slicer_row(self, cmd, msg, found):
+    def slicer_row(self, slicer_path: str, msg: str, found: bool):
+        """
+        Generates the Slicer dependency check label and path, if 3D Slicer is found.
+
+        Parameters
+        ----------
+        slicer_path : str
+            The local 3D Slicer path.
+        msg : str
+            The label message.
+        found : bool
+            True if 3d Slicer has been found locally, otherwise False.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         if found:
-            self.global_config.set_slicer_path(cmd)
+            self.global_config.set_slicer_path(slicer_path)
             self.global_config.save()
             self.slicerlabel_icon.load(self.OK_ICON_FILE)
         else:
+            self.global_config.set_slicer_path('')
+            self.global_config.save()
             self.slicerlabel_icon.load(self.ERROR_ICON_FILE)
+            
         self.slicerlabel.setText(msg)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `swane-0.0.5/swane/ui/PersistentProgressDialog.py` & `swane-0.0.6/swane/ui/PersistentProgressDialog.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from PySide6.QtWidgets import QProgressDialog
 from PySide6.QtCore import Qt
 
 
 class PersistentProgressDialog(QProgressDialog):
+    """
+    Custom implementation of PySide QProgressDialog to define a non-closable window.
+
+    """
 
     def __init__(self, label_text, minimum, maximum, parent=None):
         super(PersistentProgressDialog, self).__init__(label_text, None, minimum, maximum, parent, Qt.WindowFlags())
         self.setWindowFlags(self.windowFlags() & ~Qt.WindowCloseButtonHint)
         self.setWindowModality(Qt.WindowModal)
         self.setMinimumDuration(0)
```

### Comparing `swane-0.0.5/swane/ui/PreferencesWindow.py` & `swane-0.0.6/swane/ui/PreferencesWindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,22 +61,22 @@
             x = 0
 
             category = "MAIN"
 
             self.new_inputs[x] = PreferenceEntry(category, 'patientsfolder', my_config, PreferenceEntry.DIRECTORY,
                                                  parent=self)
             self.new_inputs[x].set_label_text(strings.pref_window_global_box_mwd)
-            self.new_inputs[x].set_box_text(strings.mainwindow_chose_working_dir_title)
+            self.new_inputs[x].set_box_text(strings.mainwindow_choose_working_dir_title)
             self.new_inputs[x].restart = True
             grid1.addWidget(self.new_inputs[x].label, x, 0)
             grid1.addWidget(self.new_inputs[x].input_field, x, 1)
             grid1.addWidget(self.new_inputs[x].button, x, 2)
             x += 1
 
-            self.new_inputs[x] = PreferenceEntry(category, 'slicerPath', my_config, PreferenceEntry.FILE, parent=self)
+            self.new_inputs[x] = PreferenceEntry(category, 'slicerPath', my_config, PreferenceEntry.FILE, parent=self, validate_on_change=True)
             self.new_inputs[x].set_label_text(strings.pref_window_global_box_slicer)
             self.new_inputs[x].set_box_text(strings.pref_window_select_slicer)
             self.new_inputs[x].restart = True
             grid1.addWidget(self.new_inputs[x].label, x, 0)
             grid1.addWidget(self.new_inputs[x].input_field, x, 1)
             grid1.addWidget(self.new_inputs[x].button, x, 2)
             x += 1
@@ -173,16 +173,16 @@
             self.new_inputs[x].set_label_text(strings.pref_window_wf_box_ai)
             if not data_input_list[DataInputList.ASL].loaded and not data_input_list[DataInputList.PET].loaded:
                 self.new_inputs[x].disable(strings.pref_window_wf_box_missing_ai)
             grid2.addWidget(self.new_inputs[x].input_field, x, 0)
             grid2.addWidget(self.new_inputs[x].label, x, 1)
             x += 1
 
-            self.new_inputs[x] = PreferenceEntry(category, 'domap', my_config, PreferenceEntry.CHECKBOX, parent=self)
-            self.new_inputs[x].set_label_text(strings.pref_window_wf_box_domap)
+            self.new_inputs[x] = PreferenceEntry(category, 'FLAT1', my_config, PreferenceEntry.CHECKBOX, parent=self)
+            self.new_inputs[x].set_label_text(strings.pref_window_wf_box_FLAT1)
             if not data_input_list[DataInputList.FLAIR3D].loaded:
                 self.new_inputs[x].disable(strings.pref_window_wf_box_missing_flair3d)
             grid2.addWidget(self.new_inputs[x].input_field, x, 0)
             grid2.addWidget(self.new_inputs[x].label, x, 1)
             x += 1
 
             self.new_inputs[x] = PreferenceEntry(category, 'tractography', my_config, PreferenceEntry.CHECKBOX,
@@ -318,51 +318,51 @@
         if not self.my_config.global_config:
             middle_layout.addWidget(self.saveButton)
             middle_layout.addWidget(discard_button)
             layout.addWidget(dx_pane)
 
         self.setLayout(layout)
 
-    def chose_dir(self, edit, message):
-        folder_path = QFileDialog.getExistingDirectory(self, message)
-        if not os.path.exists(folder_path):
-            msg_box = QMessageBox()
-            msg_box.setIcon(QMessageBox.Icon.NoIcon)
-            msg_box.setText(strings.pref_window_dir_error)
-            msg_box.exec()
-            return
-        edit.setText(folder_path)
-        self.set_restart()
-
-    def chose_file(self, edit, message):
-        file_path, _ = QFileDialog.getOpenFileName(self, message)
-        if not os.path.exists(file_path):
-            msg_box = QMessageBox()
-            msg_box.setIcon(QMessageBox.Icon.NoIcon)
-            msg_box.setText(strings.pref_window_file_error)
-            msg_box.exec()
-            return
-        edit.setText(file_path)
-        self.set_restart()
+    # def choose_dir(self, edit, message):
+    #     folder_path = QFileDialog.getExistingDirectory(self, message)
+    #     if not os.path.exists(folder_path):
+    #         msg_box = QMessageBox()
+    #         msg_box.setIcon(QMessageBox.Icon.NoIcon)
+    #         msg_box.setText(strings.pref_window_dir_error)
+    #         msg_box.exec()
+    #         return
+    #     edit.setText(folder_path)
+    #     self.set_restart()
+    #
+    # def choose_file(self, edit, message):
+    #     file_path, _ = QFileDialog.getOpenFileName(self, message)
+    #     if not os.path.exists(file_path):
+    #         msg_box = QMessageBox()
+    #         msg_box.setIcon(QMessageBox.Icon.NoIcon)
+    #         msg_box.setText(strings.pref_window_file_error)
+    #         msg_box.exec()
+    #         return
+    #     edit.setText(file_path)
+    #     self.set_restart()
 
     def freesurfer_changed(self, checked, hippo_index):
         if not checked or not self.my_config.is_freesurfer_matlab():
             self.new_inputs[hippo_index].disable()
         elif self.my_config.is_freesurfer_matlab():
             self.new_inputs[hippo_index].enable()
 
     def tractography_changed(self, checked):
         self.group_box3.setEnabled(checked)
 
-    @staticmethod
-    def set_checkbox(checkbox, value):
-        if value:
-            checkbox.setCheckState(Qt.Checked)
-        else:
-            checkbox.setCheckState(Qt.Unchecked)
+    # @staticmethod
+    # def set_checkbox(checkbox, value):
+    #     if value:
+    #         checkbox.setCheckState(Qt.Checked)
+    #     else:
+    #         checkbox.setCheckState(Qt.Unchecked)
 
     def set_restart(self):
         self.restart = True
         self.saveButton.setText(strings.pref_window_save_restart_button)
 
     def save_preferences(self):
```

### Comparing `swane-0.0.5/swane/ui/PtTab.py` & `swane-0.0.6/swane/ui/PtTab.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,14 +28,19 @@
 from swane.ui.workers.DicomSearchWorker import DicomSearchWorker
 from swane.nipype_pipeline.workflows.freesurfer_workflow import FS_DIR
 from swane.utils.DataInput import DataInput, DataInputList
 from swane.nipype_pipeline.engine.MonitoredMultiProcPlugin import MonitoredMultiProcPlugin
 
 
 class PtTab(QTabWidget):
+    """
+    Custom implementation of PySide QTabWidget to define a patient tab widget.
+
+    """
+    
     DATATAB = 0
     EXECTAB = 1
     RESULTTAB = 2
     GRAPH_DIR_NAME = "graph"
     GRAPH_FILE_PREFIX = "graph_"
     GRAPH_FILE_EXT = "svg"
     GRAPH_TYPE = "colored"
@@ -72,111 +77,182 @@
         self.exec_tab_ui()
         self.slicer_tab_ui()
 
         self.setTabEnabled(PtTab.EXECTAB, False)
         self.setTabEnabled(PtTab.RESULTTAB, False)
 
     def set_main_window(self, main_window):
+        """
+        Set the Main Window.
+
+        Parameters
+        ----------
+        main_window : MainWindow
+            The Main Window.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         self.main_window = main_window
 
-    def update_node_list(self, msg):
+    def update_node_list(self, msg: str):
+        """
+        Searches for the node linked to the msg arg.
+        Uses the parsed msng arg to update the node status.
+
+        Parameters
+        ----------
+        msg : str
+            Workflow Monitor Worker message to parse.
+
+        Returns
+        -------
+        None.
 
+        """
+        
         if msg == WorkflowMonitorWorker.STOP:
             errors = False
             for key in self.node_list.keys():
                 self.node_list[key].node_holder.setExpanded(False)
                 if not self.node_list[key].node_holder.completed:
                     errors = True
                     for subkey in self.node_list[key].node_list.keys():
                         if self.node_list[key].node_list[subkey].node_holder.art == self.main_window.ERROR_ICON_FILE:
-                            self.node_list[key].node_holder.setArt(self.main_window.ERROR_ICON_FILE)
+                            self.node_list[key].node_holder.set_art(self.main_window.ERROR_ICON_FILE)
                             break
 
             self.setTabEnabled(PtTab.DATATAB, True)
+            
             if errors:
                 self.exec_button.setText(strings.pttab_wf_executed_with_error)
                 self.node_button.setEnabled(True)
             else:
                 self.exec_button.setText(strings.pttab_wf_executed)
+                
             self.exec_button.setEnabled(False)
             self.enable_tab_if_result_dir()
+            
             return
 
+        # TODO - To be implemented for RAM usage info by each workflow
         # if msg == WorkflowProcess.WORKFLOW_INSUFFICIENT_RESOURCES:
         #     msg_box = QMessageBox()
         #     msg_box.setText(strings.pttab_wf_insufficient_resources)
         #     msg_box.exec()
 
         split = msg.split(PtTab.NODE_MSG_DIVIDER)
 
-        # Every message starts by "nipype_pt_x.", remove that
+        # For every message starts by "nipype_pt_x.", remove the prefix
         split.pop(0)
 
         # Remaining message must be like: workflow_name.node_name.message_type
         if len(split) < 3:
             return
 
         if split[2] == MonitoredMultiProcPlugin.NODE_STARTED:
             icon = self.main_window.LOADING_MOVIE_FILE
         elif split[2] == MonitoredMultiProcPlugin.NODE_COMPLETED:
             icon = self.main_window.OK_ICON_FILE
         else:
             icon = self.main_window.ERROR_ICON_FILE
 
-        self.node_list[split[0]].node_list[split[1]].node_holder.setArt(icon)
+        self.node_list[split[0]].node_list[split[1]].node_holder.set_art(icon)
 
         self.node_list[split[0]].node_holder.setExpanded(True)
 
         if icon == self.main_window.OK_ICON_FILE:
             completed = True
             for key in self.node_list[split[0]].node_list.keys():
                 if self.node_list[split[0]].node_list[key].node_holder.art != self.main_window.OK_ICON_FILE:
                     completed = False
                     break
             if completed:
-                self.node_list[split[0]].node_holder.setArt(self.main_window.OK_ICON_FILE)
+                self.node_list[split[0]].node_holder.set_art(self.main_window.OK_ICON_FILE)
                 self.node_list[split[0]].node_holder.setExpanded(False)
                 self.node_list[split[0]].node_holder.completed = True
 
     def remove_running_icon(self):
+        """
+        Remove all the loading icons from the series labels.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         for key1 in self.node_list.keys():
             for key2 in self.node_list[key1].node_list.keys():
                 if self.node_list[key1].node_list[key2].node_holder.art == self.main_window.LOADING_MOVIE_FILE:
-                    self.node_list[key1].node_list[key2].node_holder.setArt(self.main_window.VOID_SVG_FILE)
+                    self.node_list[key1].node_list[key2].node_holder.set_art(self.main_window.VOID_SVG_FILE)
 
     def start_gen_wf_thread(self):
-        # questa funzione serve a generare il wf in un thread a pare durante il caricamento del pz
-        # la prima generazione del wf può essere lunga perchè c'è il primo import delle librerie
-        # l'operazione è quasi istantanea le volte successive
-        # in caso di nuova generazione del wf viene effettuato sul thread principale
-        # questa funzione crea volo la variabile senza le nodi e le connessioni basati su preferenze e serie caricate
+        """
+        Generates the workflow object in its thread during the patient loading.
+        The first workflow generation can be heavy because SWANe needs to load nypipe modules.
+        If repeated, the operation is faster and therefore executed in the main thread.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         if not self.main_window.fsl:
             return
+        
         workflow_generator_work = WorkflowGeneratorWorker(self.pt_folder)
         workflow_generator_work.signal.workflow.connect(self.set_wf)
         QThreadPool.globalInstance().start(workflow_generator_work)
 
-    def set_wf(self, wf):
+    def set_wf(self, wf: MainWorkflow):
+        """
+        Saves the specified workflow into Main Thread and updates the UI.
+
+        Parameters
+        ----------
+        wf : MainWorkflow
+            The workflow passed to the Main Thread.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         self.workflow = wf
 
         try:
             self.node_button.setEnabled(True)
             self.wf_type_combo.setEnabled(True)
             self.pt_config_button.setEnabled(True)
 
             self.enable_exec_tab()
 
         except AttributeError:
             pass
 
     def data_tab_ui(self):
-        # LAYOUT ORIZZONTALE
+        """
+        Generates the Data tab UI.
+
+        Returns
+        -------
+        None.
+
+        """
+        
+        # Horizontal Layout
         layout = QHBoxLayout()
 
-        # PRIMA COLONNA: LISTA DEGLI INPUT
+        # First Column: INPUT LIST
         scroll_area = VerticalScrollArea()
         folder_layout = QGridLayout()
         scroll_area.m_scrollAreaWidgetContents.setLayout(folder_layout)
 
         bold_font = QFont()
         bold_font.setBold(True)
         x = 0
@@ -187,22 +263,25 @@
 
         for data_input in self.data_input_list.values():
 
             if data_input.optional and not self.global_config.is_optional_series_enabled(data_input.name):
                 remove_list.append(data_input.name)
                 continue
 
-            # TODO gestire serie opzionali
             self.input_report[data_input.name] = [QSvgWidget(self),
                                              QLabel(data_input.label),
                                              QLabel(""),
                                              QPushButton(strings.pttab_import_button),
                                              QPushButton(strings.pttab_clear_button)]
             self.input_report[data_input.name][0].load(self.main_window.ERROR_ICON_FILE)
             self.input_report[data_input.name][0].setFixedSize(25, 25)
+            if data_input.tooltip != "":
+                # Add tooltips and append ⓘ character to label
+                self.input_report[data_input.name][1].setText(data_input.label+" \u24D8")
+                self.input_report[data_input.name][1].setToolTip(data_input.tooltip)
             self.input_report[data_input.name][1].setFont(bold_font)
             self.input_report[data_input.name][1].setAlignment(Qt.AlignLeft | Qt.AlignBottom)
             self.input_report[data_input.name][2].setAlignment(Qt.AlignLeft | Qt.AlignTop)
             self.input_report[data_input.name][2].setStyleSheet("margin-bottom: 20px")
             self.input_report[data_input.name][3].setEnabled(False)
             self.input_report[data_input.name][3].clicked.connect(
                 lambda checked=None, z=data_input.name: self.dicom_import_to_folder(z))
@@ -220,32 +299,46 @@
 
             folder_layout.addWidget(self.input_report[data_input.name][2], (x * 2) + 1, 1, 1, 3)
             x += 1
 
         for to_remove in remove_list:
             self.data_input_list.pop(to_remove)
 
-        # SECONDA COLONNA: LISTA SERIE DA IMPORTARE
+        # Second Column: Series to be imported
         import_group_box = QGroupBox()
         import_layout = QVBoxLayout()
         import_group_box.setLayout(import_layout)
 
         scan_dicom_folder_button = QPushButton(strings.pttab_scan_dicom_button)
         scan_dicom_folder_button.clicked.connect(self.scan_dicom_folder)
 
         self.importable_series_list = QListWidget()
         import_layout.addWidget(scan_dicom_folder_button)
         import_layout.addWidget(self.importable_series_list)
 
-        # AGGIUNGO LE COLONNE AL LAYOUT PRINCIPALE
+        # Adding data_input columns to Main Layout
         layout.addWidget(scroll_area, stretch=1)
         layout.addWidget(import_group_box, stretch=1)
         self.data_tab.setLayout(layout)
 
-    def dicom_import_to_folder(self, input_name):
+    def dicom_import_to_folder(self, input_name: str):
+        """
+        Copies the files inside the selected folder in the input list into the folder specified by input_name var.
+
+        Parameters
+        ----------
+        input_name : str
+            The name of the series to which couple the selected file.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         if self.importable_series_list.currentRow() == -1:
             msg_box = QMessageBox()
             msg_box.setText(strings.pttab_selected_series_error)
             msg_box.exec()
             return
 
         import shutil
@@ -257,38 +350,51 @@
             msg_box = QMessageBox()
             msg_box.setText(strings.pttab_wrong_type_check_msg % (found_mod, self.data_input_list[input_name].image_modality))
             msg_box.setText(strings.pttab_wrong_type_check)
             msg_box.setIcon(QMessageBox.Icon.Warning)
             msg_box.setStandardButtons(QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No)
             msg_box.setDefaultButton(QMessageBox.StandardButton.No)
             ret = msg_box.exec()
+            
             if ret == QMessageBox.StandardButton.No:
                 return
 
         copy_list = self.final_series_list[self.importable_series_list.currentRow()][1]
 
         progress = PersistentProgressDialog(strings.pttab_dicom_copy, 0, len(copy_list) + 1, self)
         progress.show()
 
         self.input_report[input_name][0].load(self.main_window.LOADING_MOVIE_FILE)
 
         for thisFile in copy_list:
             if not os.path.isfile(thisFile):
                 continue
+            
             shutil.copy(thisFile, dest_path)
             progress.increase_value(1)
 
         progress.setRange(0, 0)
         progress.setLabelText(strings.pttab_dicom_check)
 
         self.check_input_folder(input_name, progress)
         self.reset_workflow()
 
     def scan_dicom_folder(self):
+        """
+        Opens a folder dialog window to select the DICOM files folder to import.
+        Scans the folder in a new thread.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         folder_path = QFileDialog.getExistingDirectory(self, strings.pttab_select_dicom_folder)
+        
         if not os.path.exists(folder_path):
             return
 
         dicom_src_work = DicomSearchWorker(folder_path)
         dicom_src_work.load_dir()
 
         if dicom_src_work.get_files_len() > 0:
@@ -303,17 +409,26 @@
 
         else:
             msg_box = QMessageBox()
             msg_box.setText(strings.pttab_no_dicom_error + folder_path)
             msg_box.exec()
 
     def exec_tab_ui(self):
+        """
+        Generates the Execute Workflow tab UI.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         layout = QGridLayout()
 
-        # PRIMA COLONNA: node list
+        # First Column: NODE LIST
         self.wf_type_combo = QComboBox(self)
 
         for index, label in enumerate(ConfigManager.WORKFLOW_TYPES):
             self.wf_type_combo.insertItem(index, label)
 
         layout.addWidget(self.wf_type_combo, 0, 0)
 
@@ -333,16 +448,15 @@
         self.node_list_treeWidget.header().setStretchLastSection(False)
         self.node_list_treeWidget.setHorizontalScrollBarPolicy(Qt.ScrollBarAsNeeded)
         self.node_list_treeWidget.horizontalScrollBar().setEnabled(True)
 
         layout.addWidget(self.node_list_treeWidget, 2, 0)
         self.node_list_treeWidget.itemClicked.connect(self.tree_item_clicked)
 
-        # SECONDA COLONNA: graph monitor
-
+        # Second Column: Graphviz Graph Layout
         self.pt_config_button = QPushButton(strings.PTCONFIGBUTTONTEXT)
         self.pt_config_button.clicked.connect(self.edit_pt_config)
         layout.addWidget(self.pt_config_button, 0, 1)
 
         self.exec_button = QPushButton(strings.EXECBUTTONTEXT)
         self.exec_button.clicked.connect(self.start_workflow_thread)
         self.exec_button.setEnabled(False)
@@ -350,189 +464,342 @@
         layout.addWidget(self.exec_button, 1, 1)
         self.exec_graph = QSvgWidget()
         layout.addWidget(self.exec_graph, 2, 1)
 
         self.exec_tab.setLayout(layout)
 
     def edit_pt_config(self):
+        """
+        Opens the Patient Preference Window.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         preference_window = PreferencesWindow(self.pt_config, self.data_input_list, self)
         ret = preference_window.exec()
         if ret != 0:
             self.reset_workflow()
 
-    def on_wf_type_changed(self, index):
+    def on_wf_type_changed(self, index: int):
+        """
+        Updates the workflow at workflow type combo change.
+
+        Parameters
+        ----------
+        index : int
+            The new selected value from the Execution tab workflow type combo.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         self.pt_config.set_wf_option(index)
         self.pt_config.save()
         self.reset_workflow()
 
     def gen_wf(self):
+        """
+        Generates and populates the Main Workflow.
+        Shows the node list into the UI.
+        Generates the graphviz analysis graphs on a new thread.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         if not self.main_window.fsl:
             error_dialog = QErrorMessage(parent=self)
             error_dialog.showMessage(strings.pttab_missing_fsl_error)
             return
 
+        # Main Workflow generation
         if self.workflow is None:
             self.workflow = MainWorkflow(name=self.pt_name + WorkflowGeneratorWorker.WF_DIR_SUFFIX, base_dir=self.pt_folder)
-
+        
+        # Node List population
         try:
             self.workflow.add_input_folders(self.global_config, self.pt_config, self.data_input_list)
         except:
             error_dialog = QErrorMessage(parent=self)
             error_dialog.showMessage(strings.pttab_wf_gen_error)
             traceback.print_exc()
             # TODO: generiamo un file crash nella cartella log?
             return
+        
         self.node_list = self.workflow.get_node_array()
         self.node_list_treeWidget.clear()
 
         graph_dir = os.path.join(self.pt_folder, PtTab.GRAPH_DIR_NAME)
         shutil.rmtree(graph_dir, ignore_errors=True)
         os.mkdir(graph_dir)
-
+        
+        # Graphviz analysis graphs drawing
         for node in self.node_list.keys():
             self.node_list[node].node_holder = CustomTreeWidgetItem(self.node_list_treeWidget, self.node_list_treeWidget, self.node_list[node].long_name)
             if len(self.node_list[node].node_list.keys()) > 0:
                 if self.main_window.graphviz:
                     graph_name = self.node_list[node].long_name.lower().replace(" ", "_")
                     thread = Thread(target=self.workflow.get_node(node).write_graph,
                                     kwargs={'graph2use': self.GRAPH_TYPE, 'format': PtTab.GRAPH_FILE_EXT,
                                             'dotfilename': os.path.join(graph_dir,
                                                                         PtTab.GRAPH_FILE_PREFIX + graph_name + '.dot')})
                     thread.start()
+                    
                 for sub_node in self.node_list[node].node_list.keys():
                     self.node_list[node].node_list[sub_node].node_holder = CustomTreeWidgetItem(self.node_list[node].node_holder, self.node_list_treeWidget, self.node_list[node].node_list[sub_node].long_name)
+        
+        # UI updating
         self.exec_button.setEnabled(True)
         self.exec_button.setText(strings.EXECBUTTONTEXT)
         self.node_button.setEnabled(False)
 
-    def tree_item_clicked(self, item, col):
+    def tree_item_clicked(self, item, col: int):
+        """
+        Listener for the QTreeWidget Items.
+        Shows the clicked analysis graphviz graph.
+
+        Parameters
+        ----------
+        item : QTreeWidget Item
+            The QTreeWidget item clicked.
+        col : int
+            The QTreeWidget column.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         if self.main_window.graphviz and item.parent() is None:
-            file = os.path.join(self.pt_folder, PtTab.GRAPH_DIR_NAME, PtTab.GRAPH_FILE_PREFIX + item.getText().lower().replace(" ", "_") + '.'
+            file = os.path.join(self.pt_folder, PtTab.GRAPH_DIR_NAME, PtTab.GRAPH_FILE_PREFIX + item.get_text().lower().replace(" ", "_") + '.'
                                 + PtTab.GRAPH_FILE_EXT)
             self.exec_graph.load(file)
             self.exec_graph.renderer().setAspectRatioMode(Qt.AspectRatioMode.KeepAspectRatio)
 
     @staticmethod
     def no_close_event(event):
+        """
+        Used to prevent the user to close a dialog.
+
+        Parameters
+        ----------
+        event : TYPE
+            The event to ignore.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         event.ignore()
 
-    def is_workflow_process_alive(self):
+    def is_workflow_process_alive(self) -> bool:
+        """
+        Checks if a workflow is in execution.
+
+        Returns
+        -------
+        bool
+            True if the workflow is executing, elsewise False.
+
+        """
+        
         try:
             if self.workflow_process is None:
                 return False
+            
             return self.workflow_process.is_alive()
+        
         except AttributeError:
             return False
 
     def start_workflow_thread(self):
+        """
+        If the workflow is not started, executes it.
+        If the workflow is executing, kills it.
+
+        Returns
+        -------
+        None.
+
+        """
+        
+        # Workflow not started
         if not self.is_workflow_process_alive():
             workflow_dir = os.path.join(self.pt_folder, self.pt_name + WorkflowGeneratorWorker.WF_DIR_SUFFIX)
+            # Checks for a previous workflow execution
             if os.path.exists(workflow_dir):
+                # If yes, asks for workflow resume or reset
                 msg_box = QMessageBox()
                 msg_box.setText(strings.pttab_old_wf_found)
                 msg_box.setIcon(QMessageBox.Icon.Question)
                 msg_box.setStandardButtons(QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No)
                 msg_box.button(QMessageBox.StandardButton.Yes).setText(strings.pttab_old_wf_resume)
                 msg_box.button(QMessageBox.StandardButton.No).setText(strings.pttab_old_wf_reset)
                 msg_box.setDefaultButton(QMessageBox.StandardButton.Yes)
                 msg_box.setWindowFlags(Qt.CustomizeWindowHint | Qt.WindowTitleHint)
                 msg_box.closeEvent = self.no_close_event
                 ret = msg_box.exec()
+                
                 if ret == QMessageBox.StandardButton.No:
                     shutil.rmtree(workflow_dir, ignore_errors=True)
 
             fsdir = os.path.join(self.pt_folder, FS_DIR)
+            # Checks for a previous workflow FreeSurfer execution
             if self.pt_config.get_pt_wf_freesurfer() and os.path.exists(fsdir):
+                # If yes, asks for workflow resume or reset
                 msg_box = QMessageBox()
                 msg_box.setText(strings.pttab_old_fs_found)
                 msg_box.setIcon(QMessageBox.Icon.Question)
                 msg_box.setStandardButtons(QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No)
                 msg_box.button(QMessageBox.StandardButton.Yes).setText(strings.pttab_old_fs_resume)
                 msg_box.button(QMessageBox.StandardButton.No).setText(strings.pttab_old_fs_reset)
                 msg_box.setDefaultButton(QMessageBox.StandardButton.Yes)
                 msg_box.setWindowFlags(Qt.CustomizeWindowHint | Qt.WindowTitleHint)
                 msg_box.closeEvent = self.no_close_event
                 ret = msg_box.exec()
+                
                 if ret == QMessageBox.StandardButton.No:
                     shutil.rmtree(fsdir, ignore_errors=True)
 
             queue = Queue(maxsize=500)
-
+            
+            # Generates a Monitor Worker to receive workflows notifications
             workflow_monitor_work = WorkflowMonitorWorker(queue)
             workflow_monitor_work.signal.log_msg.connect(self.update_node_list)
             QThreadPool.globalInstance().start(workflow_monitor_work)
-
+            
+            # Starts the workflow on a new process
             self.workflow_process = WorkflowProcess(self.pt_name, self.workflow, queue)
             self.workflow_process.start()
-
+            
+            # UI updating
             self.exec_button.setText(strings.EXECBUTTONTEXT_STOP)
             self.setTabEnabled(PtTab.DATATAB, False)
             self.setTabEnabled(PtTab.RESULTTAB, False)
             self.wf_type_combo.setEnabled(False)
             self.pt_config_button.setEnabled(False)
 
+        # Workflow executing
         else:
+            # Asks for workflow kill confirmation
             msg_box = QMessageBox()
             msg_box.setText(strings.pttab_wf_stop)
             msg_box.setIcon(QMessageBox.Icon.Question)
             msg_box.setStandardButtons(QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No)
             msg_box.setDefaultButton(QMessageBox.StandardButton.No)
             msg_box.closeEvent = self.no_close_event
             ret = msg_box.exec()
+            
             if ret == QMessageBox.StandardButton.No:
                 return
-
+            
+            # Workflow killing
             self.workflow_process.stop_event.set()
-
+            
+            # UI updating
             self.remove_running_icon()
             self.exec_button.setText(strings.EXECBUTTONTEXT)
             self.setTabEnabled(PtTab.DATATAB, True)
             self.reset_workflow(force=True)
             self.enable_tab_if_result_dir()
 
     def slicer_tab_ui(self):
+        """
+        Generates the Results tab UI.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         slicer_tab_layout = QGridLayout()
         self.slicer_tab.setLayout(slicer_tab_layout)
 
         self.export_results_button = QPushButton(strings.pttab_results_button)
         self.export_results_button.clicked.connect(self.slicer_thread)
         self.export_results_button.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
+        
         if self.global_config.get_slicer_path() == '' or not os.path.exists(self.global_config.get_slicer_path()):
             self.export_results_button.setEnabled(False)
         slicer_tab_layout.addWidget(self.export_results_button, 0, 0)
 
         self.results_model = QFileSystemModel()
         self.result_tree = QTreeView(parent=self)
         self.result_tree.setModel(self.results_model)
 
         slicer_tab_layout.addWidget(self.result_tree, 1, 0)
 
     def slicer_thread(self):
+        """
+        Exports the workflow results into 3D Slicer using a new thread.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         progress = PersistentProgressDialog(strings.pttab_exporting_start, 0, 0, parent=self)
         progress.show()
 
         slicer_thread = SlicerExportWorker(self.global_config.get_slicer_path(), self.pt_folder,
                                            self.global_config.get_slicer_scene_ext(), parent=self)
         slicer_thread.signal.export.connect(lambda msg: self.slicer_thread_signal(msg, progress))
         QThreadPool.globalInstance().start(slicer_thread)
 
-    def slicer_thread_signal(self, msg, progress):
+    def slicer_thread_signal(self, msg: str, progress: PersistentProgressDialog):
+        """
+        Updates the Progress Dialog text to inform the user of the loading status.
+
+        Parameters
+        ----------
+        msg : str
+            The loading text.
+        progress : PersistentProgressDialog
+            The Progress Dialog.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         if msg == SlicerExportWorker.END_MSG:
             progress.done(1)
         else:
             progress.setLabelText(strings.pttab_exporting_prefix + msg)
 
     def load_pt(self):
+        """
+        Loads the Patient configuration and folder.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         dicom_scanners = {}
         total_files = 0
 
-        # importo la configurazione del tipo di nipype_pipeline
+        # Config import absed on nipype_pipeline
         self.pt_config = ConfigManager(self.pt_folder, self.main_window.freesurfer)
         self.wf_type_combo.setCurrentIndex(self.pt_config.get_pt_wf_type())
-        # BISOGNA DICHIRARE QUI LA FUNZIONE ONCHANGED ALTRIMENTI RESETTA IL WF AL DEFAULT AL CARICAMENTO DEL PAZIENTE
+        # Set after patient loading to prevent the onchanged fire on previous line command
         self.wf_type_combo.currentIndexChanged.connect(self.on_wf_type_changed)
 
         for data_input in self.data_input_list.values():
             input_name = data_input.name
             dicom_scanners[input_name] = self.check_input_folder_step1(input_name)
             total_files = total_files + dicom_scanners[input_name].get_files_len()
 
@@ -549,144 +816,272 @@
             self.check_input_folder_step2(input_name, dicom_scanners[input_name], progress)
             self.directory_watcher.addPath(
                 os.path.join(self.pt_folder, self.global_config.get_default_dicom_folder(), input_name))
 
         self.setTabEnabled(PtTab.DATATAB, True)
         self.setCurrentWidget(self.data_tab)
 
-        # svuoto la lista delle serie importabili
         self.importable_series_list.clear()
-        # reset del nipype_pipeline
         self.reset_workflow()
 
         self.enable_tab_if_result_dir()
 
     def enable_tab_if_result_dir(self):
+        """
+        Enables Results tab, if any.
+
+        Returns
+        -------
+        None.
+
+        """
         scene_dir = os.path.join(self.pt_folder, MainWorkflow.SCENE_DIR)
+        
         if os.path.exists(scene_dir):
             self.setTabEnabled(PtTab.RESULTTAB, True)
             self.results_model.setRootPath(scene_dir)
             index_root = self.results_model.index(self.results_model.rootPath())
             self.result_tree.setRootIndex(index_root)
         else:
             self.setTabEnabled(PtTab.RESULTTAB, False)
 
-    def check_input_folder_step1(self, input_name):
+    def check_input_folder_step1(self, input_name: str) -> DicomSearchWorker:
+        """
+        Generates a Worker that scan the series folder in search for DICOM files.
+
+        Parameters
+        ----------
+        input_name : str
+            The series folder name to check.
+
+        Returns
+        -------
+        dicom_src_work : DicomSearchWorker
+            The DICOM Search Worker.
+
+        """
+        
         src_path = os.path.join(self.pt_folder,
                                 self.global_config.get_default_dicom_folder(), input_name)
         dicom_src_work = DicomSearchWorker(src_path)
         dicom_src_work.load_dir()
+        
         return dicom_src_work
 
-    def check_input_folder_step2(self, input_name, dicom_src_work, progress=None):
+    def check_input_folder_step2(self, input_name: str, dicom_src_work: DicomSearchWorker, progress: PersistentProgressDialog=None):
+        """
+        Starts the DICOM files scan Worker into the series folder on a new thread.
+
+        Parameters
+        ----------
+        input_name : str
+            The series folder name to check.
+        dicom_src_work : DicomSearchWorker
+            The DICOM Search Worker.
+        progress : PersistentProgressDialog, optional
+            The progress dialog. The default is None.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         dicom_src_work.signal.sig_finish.connect(lambda src, name=input_name: self.check_input_folder_step3(name, src))
+        
         if progress is not None:
             if progress.maximum() == 0:
                 progress.setMaximum(dicom_src_work.get_files_len())
             dicom_src_work.signal.sig_loop.connect(lambda i: progress.increase_value(i))
+            
         QThreadPool.globalInstance().start(dicom_src_work)
 
-    def check_input_folder_step3(self, input_name, dicom_src_work):
+    def check_input_folder_step3(self, input_name: str, dicom_src_work: DicomSearchWorker):
+        """
+        Updates SWANe UI at the end of the DICOM files scan Worker execution for a patient.
+
+        Parameters
+        ----------
+        input_name : str
+            The series folder name to check.
+        dicom_src_work : DicomSearchWorker
+            The DICOM Search Worker.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         src_path = dicom_src_work.dicom_dir
         pt_list = dicom_src_work.get_patient_list()
 
         if len(pt_list) == 0:
             self.set_error(input_name, strings.pttab_no_dicom_error + src_path)
             return
 
         if len(pt_list) > 1:
             self.set_warn(input_name, strings.pttab_multi_pt_error + src_path)
             return
+        
         exam_list = dicom_src_work.get_exam_list(pt_list[0])
+        
         if len(exam_list) != 1:
             self.set_warn(input_name, strings.pttab_multi_exam_error + src_path)
             return
+        
         series_list = dicom_src_work.get_series_list(pt_list[0], exam_list[0])
+        
         if len(series_list) != 1:
             self.set_warn(input_name, strings.pttab_multi_series_error + src_path)
             return
 
         image_list = dicom_src_work.get_series_files(pt_list[0], exam_list[0], series_list[0])
         ds = pydicom.read_file(image_list[0], force=True)
         mod = ds.Modality
+        
         if mod in DataInput.IMAGE_MODALITY_RENAME_LIST:
             mod = DataInput.IMAGE_MODALITY_RENAME_LIST[mod]
+            
         self.set_ok(input_name, str(ds.PatientName) + "-" + mod + "-" + ds.SeriesDescription + ": " + str(
             len(image_list)) + " images")
 
         self.data_input_list[input_name].loaded = True
 
         self.enable_exec_tab()
 
-    def check_input_folder(self, input_name, progress=None):
+    def check_input_folder(self, input_name: str, progress: PersistentProgressDialog=None):
+        """
+        Checks if the series folder labelled input_name contains DICOM files.
+        If PersistentProgressDialog is not None, it will be used to show the scan progress.
+
+        Parameters
+        ----------
+        input_name : str
+            The series folder name to check.
+        progress : PersistentProgressDialog, optional
+            The progress dialog. The default is None.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         dicom_src_work = self.check_input_folder_step1(input_name)
         self.check_input_folder_step2(input_name, dicom_src_work, progress)
 
-    def clear_import_folder(self, input_name):
+    def clear_import_folder(self, input_name: str):
+        """
+        Clears the patient series folder.
+
+        Parameters
+        ----------
+        input_name : str
+            The series folder name to clear.
+
+        Returns
+        -------
+        None.
+
+        """
 
         src_path = os.path.join(self.pt_folder,
                                 self.global_config.get_default_dicom_folder(), input_name)
 
         progress = PersistentProgressDialog(strings.pttab_dicom_clearing + src_path, 0, 0, self)
         progress.show()
 
         import shutil
         shutil.rmtree(src_path, ignore_errors=True)
         os.makedirs(src_path, exist_ok=True)
 
-        # reset dei wf in caso di cambio immagini
+        # Reset the workflows related to the deleted DICOM images
         src_path = os.path.join(self.pt_folder, self.pt_name + WorkflowGeneratorWorker.WF_DIR_SUFFIX,
                                 self.data_input_list[input_name].wf_name)
         shutil.rmtree(src_path, ignore_errors=True)
 
         self.set_error(input_name, strings.pttab_no_dicom_error + src_path)
         self.data_input_list[input_name].loaded = False
         self.enable_exec_tab()
 
         progress.accept()
+        
         self.reset_workflow()
 
-    def reset_workflow(self, force=False):
-        # l'argomento dir viene passato dal filesystemwatcher ma non viene utilizzata (valutare se forzare un reload delle cartelle modificate)
-        # SE il wf è già resettato oppure è in esecuzione non faccio nulla (in caso di funzione innescata dal filesystemwatcher)
+    def reset_workflow(self, force: bool=False):
+        """
+        Set the workflow var to None.
+        Resets the UI.
+        Works only if the worklow is not in execution or if force var is True.
+
+        Parameters
+        ----------
+        force : bool, optional
+            Force the usage of this function during workflow execution. The default is False.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         if self.workflow is None:
             return
         if not force and self.is_workflow_process_alive():
             return
 
         self.workflow = None
         self.node_list_treeWidget.clear()
         self.exec_graph.load(self.main_window.VOID_SVG_FILE)
         self.exec_button.setEnabled(False)
         self.exec_button.setText(strings.EXECBUTTONTEXT)
         self.node_button.setEnabled(True)
         self.wf_type_combo.setEnabled(True)
         self.pt_config_button.setEnabled(True)
 
-    def show_scan_result(self, dicom_src_work):
+    def show_scan_result(self, dicom_src_work: DicomSearchWorker):
+        """
+        Updates importable series list using DICOM Search Worker results.
+
+        Parameters
+        ----------
+        dicom_src_work : DicomSearchWorker
+            The DICOM Search Worker.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         folder_path = dicom_src_work.dicom_dir
         pt_list = dicom_src_work.get_patient_list()
 
         if len(pt_list) == 0:
             msg_box = QMessageBox()
             msg_box.setText(strings.pttab_no_dicom_error + folder_path)
             msg_box.exec()
             return
+        
         if len(pt_list) > 1:
             msg_box = QMessageBox()
             msg_box.setText(strings.pttab_multi_pt_error + folder_path)
             msg_box.exec()
             return
+        
         exam_list = dicom_src_work.get_exam_list(pt_list[0])
+        
         for exam in exam_list:
             series_list = dicom_src_work.get_series_list(pt_list[0], exam)
             for series in series_list:
                 image_list = dicom_src_work.get_series_files(pt_list[0], exam, series)
                 ds = pydicom.read_file(image_list[0], force=True)
-                # non mostro le serie troppo corte (survey ecc) a meno che non siano mosaici
+                
+                # Excludes series with less than 10 images unless they are siemens mosaics series
                 if len(image_list) < 10 and hasattr(ds, 'ImageType') and "MOSAIC" not in ds.ImageType:
                     continue
 
                 mod = ds.Modality
 
                 if mod in DataInput.IMAGE_MODALITY_RENAME_LIST:
                     mod = DataInput.IMAGE_MODALITY_RENAME_LIST[mod]
@@ -695,37 +1090,91 @@
                     [str(ds.PatientName) + "-" + mod + "-" + ds.SeriesDescription + ": " + str(
                         len(image_list)) + " images", image_list])
                 del image_list
 
         for series in self.final_series_list:
             self.importable_series_list.addItem(series[0])
 
-    def set_warn(self, input_name, msg):
+    def set_warn(self, input_name: str, msg: str):
+        """
+        Set a warning message and icon near a series label.
+
+        Parameters
+        ----------
+        input_name : str
+            The series label.
+        msg : str
+            The warning message.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         self.input_report[input_name][0].load(self.main_window.WARNING_ICON_FILE)
         self.input_report[input_name][0].setFixedSize(25, 25)
         self.input_report[input_name][0].setToolTip(msg)
         self.input_report[input_name][3].setEnabled(False)
         self.input_report[input_name][4].setEnabled(True)
         self.input_report[input_name][2].setText("")
 
-    def set_error(self, input_name, msg):
+    def set_error(self, input_name: str, msg: str):
+        """
+        Set an error message and icon near a series label.
+
+        Parameters
+        ----------
+        input_name : str
+            The series label.
+        msg : str
+            The error message.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         self.input_report[input_name][0].load(self.main_window.ERROR_ICON_FILE)
         self.input_report[input_name][0].setFixedSize(25, 25)
         self.input_report[input_name][0].setToolTip(msg)
         self.input_report[input_name][3].setEnabled(True)
         self.input_report[input_name][4].setEnabled(False)
         self.input_report[input_name][2].setText("")
 
-    def set_ok(self, input_name, msg):
+    def set_ok(self, input_name: str, msg: str):
+        """
+        Set a success message and icon near a series label.
+
+        Parameters
+        ----------
+        input_name : str
+            The series label.
+        msg : str
+            The success message.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         self.input_report[input_name][0].load(self.main_window.OK_ICON_FILE)
         self.input_report[input_name][0].setFixedSize(25, 25)
         self.input_report[input_name][0].setToolTip("")
         self.input_report[input_name][3].setEnabled(False)
         self.input_report[input_name][4].setEnabled(True)
         self.input_report[input_name][2].setText(msg)
 
-    def close_routine(self):
-        self.pt_config.save()
-
     def enable_exec_tab(self):
+        """
+        Enables the Execute Workflow tab into the UI.
+
+        Returns
+        -------
+        None.
+
+        """
+        
         enable = self.data_input_list.is_ref_loaded() and self.main_window.fsl and self.main_window.dcm2niix
         self.setTabEnabled(PtTab.EXECTAB, enable)
```

### Comparing `swane-0.0.5/swane/ui/VerticalScrollArea.py` & `swane-0.0.6/swane/ui/VerticalScrollArea.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from PySide6.QtWidgets import QScrollArea, QGroupBox, QSizePolicy
 from PySide6.QtCore import Qt, QEvent
 
 
 class VerticalScrollArea(QScrollArea):
+    """
+    Custom implementation of PySide QScrollArea to define a dynamic width scrollable area.
+
+    """
+    
     def __init__(self, parent=None):
         super(VerticalScrollArea, self).__init__(parent)
         self.setWidgetResizable(True)
         self.setHorizontalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
         self.setVerticalScrollBarPolicy(Qt.ScrollBarAsNeeded)
         self.m_scrollAreaWidgetContents = QGroupBox(self)
         self.m_scrollAreaWidgetContents.setSizePolicy(QSizePolicy.Preferred, QSizePolicy.Preferred)
```

### Comparing `swane-0.0.5/swane/ui/workers/DicomSearchWorker.py` & `swane-0.0.6/swane/ui/workers/DicomSearchWorker.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/ui/workers/WorkflowGeneratorWorker.py` & `swane-0.0.6/swane/ui/workers/WorkflowGeneratorWorker.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/ui/workers/WorkflowMonitorWorker.py` & `swane-0.0.6/swane/ui/workers/WorkflowMonitorWorker.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/ui/workers/WorkflowProcess.py` & `swane-0.0.6/swane/ui/workers/WorkflowProcess.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/utils/ConfigManager.py` & `swane-0.0.6/swane/utils/ConfigManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
               "fa": ['Frontal Aslant', 'false', 0],
               "fma": ['Forceps Major', 'false', 0],
               "fmi": ['Forceps Minor', 'false', 0],
               "fx": ['Fornix', 'false', 0],
               "ilf": ['Inferior Longitudinal Fasciculus', 'false', 0],
               "ifo": ['Inferior Fronto-Occipital Fasciculus', 'false', 0],
               "mcp": ['Middle Cerebellar Peduncle', 'false', 0],
-              "mdlf": ['Middle Longitudinal Fasciculuc', 'false', 0],
+              "mdlf": ['Middle Longitudinal Fasciculus', 'false', 0],
               "or": ['Optic Radiation', 'true', 0],
               "str": ['Superior Thalamic Radiation', 'false', 0],
               "ac": ['Anterior Commissure', 'false', 0],
               "uf": ['Uncinate Fasciculus', 'false', 0],
               "vof": ['Vertical Occipital Fasciculus', 'false', 0],
               "null": ['Vertical Occipital Fasciculus', 'false', 0],
               }
@@ -60,23 +60,23 @@
 
 
     DEFAULT_WF = {}
     DEFAULT_WF['0'] = {
         'wftype': '0',
         'freesurfer': 'true',
         'hippoAmygLabels': 'false',
-        'domap': 'false',
+        'FLAT1': 'false',
         'ai': 'false',
         'tractography': 'true',
     }
     DEFAULT_WF['1'] = {
         'wftype': '1',
         'freesurfer': 'true',
         'hippoAmygLabels': 'true',
-        'domap': 'true',
+        'FLAT1': 'true',
         'ai': 'true',
         'tractography': 'false',
     }
 
     def __init__(self, pt_folder=None, freesurfer=None):
         super(ConfigManager, self).__init__()
```

### Comparing `swane-0.0.5/swane/utils/PreferenceEntry.py` & `swane-0.0.6/swane/utils/PreferenceEntry.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,28 +14,29 @@
     TEXT = 0
     NUMBER = 1
     CHECKBOX = 2
     COMBO = 3
     FILE = 4
     DIRECTORY = 5
 
-    def __init__(self, category, key, my_config, input_type=TEXT, parent=None, populate_combo=None):
+    def __init__(self, category, key, my_config, input_type=TEXT, parent=None, populate_combo=None, validate_on_change=False):
         self.restart = False
         self.category = category
         self.key = key
         self.input_type = input_type
         self.label = QLabel()
         self.label.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Minimum)
         self.input_field, self.button = self.gen_input_field()
         if input_type == PreferenceEntry.COMBO and populate_combo is not None:
             self.populate_combo(populate_combo)
         self.set_value_from_config(my_config)
         self.box_text = ''
         self.parent = parent
         self.changed = False
+        self.validate_on_change = validate_on_change
 
     def set_label_text(self, text):
         self.label.setText(text)
 
     def set_box_text(self, text):
         self.box_text = text
 
@@ -62,20 +63,19 @@
 
         if self.input_type == PreferenceEntry.FILE or self.input_type == PreferenceEntry.DIRECTORY:
             field.setReadOnly(True)
             button = QPushButton()
             pixmap = getattr(QStyle, "SP_DirOpenIcon")
             icon_open_dir = button.style().standardIcon(pixmap)
             button.setIcon(icon_open_dir)
-            button.clicked.connect(self.chose_file)
+            button.clicked.connect(self.choose_file)
 
         return field, button
 
-    def chose_file(self, parent):
-        print("mah")
+    def choose_file(self):
         if self.input_type == PreferenceEntry.FILE:
             file_path, _ = QFileDialog.getOpenFileName(parent=self.parent, caption=self.box_text)
             error = strings.pref_window_file_error
         elif self.input_type == PreferenceEntry.DIRECTORY:
             file_path = QFileDialog.getExistingDirectory(parent=self.parent, caption=self.box_text)
             error = strings.pref_window_dir_error
         else:
@@ -86,14 +86,18 @@
 
         if not os.path.exists(file_path):
             msg_box = QMessageBox()
             msg_box.setIcon(QMessageBox.Warning)
             msg_box.setText(error)
             msg_box.exec()
             return
+
+        if self.validate_on_change:
+            file_path = "*" + file_path
+
         self.set_value(file_path)
 
     def populate_combo(self, items):
         if self.input_type != PreferenceEntry.COMBO:
             return
         for index, label in enumerate(items):
             self.input_field.insertItem(index, label)
```

### Comparing `swane-0.0.5/swane/utils/check_dependency.py` & `swane-0.0.6/swane/utils/check_dependency.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/utils/fsl_conflict_handler.py` & `swane-0.0.6/swane/utils/fsl_conflict_handler.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane/utils/shortcut_manager.py` & `swane-0.0.6/swane/utils/shortcut_manager.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.5/swane.egg-info/SOURCES.txt` & `swane-0.0.6/swane.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,34 +20,37 @@
 swane/nipype_pipeline/nodes/AsymmetryIndex.py
 swane/nipype_pipeline/nodes/CustomBEDPOSTX5.py
 swane/nipype_pipeline/nodes/CustomDcm2niix.py
 swane/nipype_pipeline/nodes/CustomDilateImage.py
 swane/nipype_pipeline/nodes/CustomLabel2Vol.py
 swane/nipype_pipeline/nodes/CustomProbTrackX2.py
 swane/nipype_pipeline/nodes/CustomSliceTimer.py
-swane/nipype_pipeline/nodes/DOmapOutliersMask.py
 swane/nipype_pipeline/nodes/DeleteVolumes.py
+swane/nipype_pipeline/nodes/FLAT1OutliersMask.py
 swane/nipype_pipeline/nodes/FMRIGenSpec.py
 swane/nipype_pipeline/nodes/ForceOrient.py
 swane/nipype_pipeline/nodes/FslCluster.py
 swane/nipype_pipeline/nodes/FslNVols.py
 swane/nipype_pipeline/nodes/GetNiftiTR.py
 swane/nipype_pipeline/nodes/MergeTargets.py
 swane/nipype_pipeline/nodes/Orient.py
 swane/nipype_pipeline/nodes/RandomSeedGenerator.py
 swane/nipype_pipeline/nodes/SegmentHA.py
 swane/nipype_pipeline/nodes/SumMultiTracks.py
+swane/nipype_pipeline/nodes/SumMultiVols.py
+swane/nipype_pipeline/nodes/TTest.py
 swane/nipype_pipeline/nodes/ThrROI.py
 swane/nipype_pipeline/nodes/VenousCheck.py
 swane/nipype_pipeline/nodes/Zscore.py
 swane/nipype_pipeline/nodes/__init__.py
 swane/nipype_pipeline/nodes/utils.py
+swane/nipype_pipeline/workflows/FLAT1_workflow.py
 swane/nipype_pipeline/workflows/__init__.py
-swane/nipype_pipeline/workflows/domap_workflow.py
 swane/nipype_pipeline/workflows/dti_preproc_workflow.py
+swane/nipype_pipeline/workflows/freesurfer_asymmetry_index_workflow.py
 swane/nipype_pipeline/workflows/freesurfer_workflow.py
 swane/nipype_pipeline/workflows/func_map_workflow.py
 swane/nipype_pipeline/workflows/linear_reg_workflow.py
 swane/nipype_pipeline/workflows/nonlinear_reg_workflow.py
 swane/nipype_pipeline/workflows/ref_workflow.py
 swane/nipype_pipeline/workflows/task_fMRI_workflow.py
 swane/nipype_pipeline/workflows/tractography_workflow.py
@@ -71,8 +74,9 @@
 swane/ui/workers/__init__.py
 swane/utils/ConfigManager.py
 swane/utils/DataInput.py
 swane/utils/PreferenceEntry.py
 swane/utils/__init__.py
 swane/utils/check_dependency.py
 swane/utils/fsl_conflict_handler.py
+swane/utils/print_error.py
 swane/utils/shortcut_manager.py
```

