# Comparing `tmp/kubeflow-training-1.6.0rc0.tar.gz` & `tmp/kubeflow-training-1.7.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kubeflow-training-1.6.0rc0.tar", last modified: Thu Jan 26 11:54:55 2023, max compression
+gzip compressed data, was "kubeflow-training-1.7.0rc0.tar", last modified: Mon Aug  7 13:02:53 2023, max compression
```

## Comparing `kubeflow-training-1.6.0rc0.tar` & `kubeflow-training-1.7.0rc0.tar`

### file list

```diff
@@ -1,97 +1,98 @@
-drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-01-26 11:54:55.000000 kubeflow-training-1.6.0rc0/
--rw-r--r--   0 johnu.george   (502) staff       (20)     1183 2023-01-26 11:54:55.000000 kubeflow-training-1.6.0rc0/PKG-INFO
--rw-r--r--   0 johnu.george   (502) staff       (20)     4555 2023-01-23 05:25:04.000000 kubeflow-training-1.6.0rc0/README.md
-drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-01-26 11:54:55.000000 kubeflow-training-1.6.0rc0/kubeflow/
--rw-r--r--   0 johnu.george   (502) staff       (20)       64 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/__init__.py
-drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-01-26 11:54:55.000000 kubeflow-training-1.6.0rc0/kubeflow/training/
--rw-r--r--   0 johnu.george   (502) staff       (20)     3142 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/__init__.py
-drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-01-26 11:54:55.000000 kubeflow-training-1.6.0rc0/kubeflow/training/api/
--rw-r--r--   0 johnu.george   (502) staff       (20)       87 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/api/__init__.py
--rw-r--r--   0 johnu.george   (502) staff       (20)    59037 2023-01-25 15:22:47.000000 kubeflow-training-1.6.0rc0/kubeflow/training/api/training_client.py
--rw-r--r--   0 johnu.george   (502) staff       (20)    26198 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/api_client.py
--rw-r--r--   0 johnu.george   (502) staff       (20)    12393 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/configuration.py
-drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-01-26 11:54:55.000000 kubeflow-training-1.6.0rc0/kubeflow/training/constants/
--rw-r--r--   0 johnu.george   (502) staff       (20)      576 2022-11-02 15:55:46.000000 kubeflow-training-1.6.0rc0/kubeflow/training/constants/__init__.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3426 2023-01-25 15:22:47.000000 kubeflow-training-1.6.0rc0/kubeflow/training/constants/constants.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3728 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/exceptions.py
-drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-01-26 11:54:55.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/
--rw-r--r--   0 johnu.george   (502) staff       (20)     2681 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/__init__.py
--rw-r--r--   0 johnu.george   (502) staff       (20)    13868 2023-01-26 11:43:25.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_elastic_policy.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7298 2023-01-26 11:43:25.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_mpi_job.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     6884 2023-01-26 11:43:25.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_mpi_job_list.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7988 2023-01-26 11:43:25.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_mpi_job_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7271 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_mx_job.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     6861 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_mx_job_list.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     6291 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_mx_job_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7822 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_elastic_policy.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7379 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_job.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7037 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_job_list.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     6150 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_job_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7406 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_py_torch_job.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7062 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_py_torch_job_list.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     6177 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_py_torch_job_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3887 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_rdzv_conf.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7271 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_tf_job.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     6937 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_tf_job_list.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7195 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_tf_job_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7406 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_xg_boost_job.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     6976 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_xg_boost_job_list.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     4750 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_xg_boost_job_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7733 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/v1_job_condition.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7368 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/v1_job_status.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     5279 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/v1_replica_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     6893 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/v1_replica_status.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     8170 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/v1_run_policy.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     6677 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/models/v1_scheduling_policy.py
--rw-r--r--   0 johnu.george   (502) staff       (20)    12263 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/kubeflow/training/rest.py
-drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-01-26 11:54:55.000000 kubeflow-training-1.6.0rc0/kubeflow/training/utils/
--rw-r--r--   0 johnu.george   (502) staff       (20)      576 2022-11-02 15:55:46.000000 kubeflow-training-1.6.0rc0/kubeflow/training/utils/__init__.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     9592 2023-01-25 15:22:47.000000 kubeflow-training-1.6.0rc0/kubeflow/training/utils/utils.py
-drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-01-26 11:54:55.000000 kubeflow-training-1.6.0rc0/kubeflow_training.egg-info/
--rw-r--r--   0 johnu.george   (502) staff       (20)     1183 2023-01-26 11:54:55.000000 kubeflow-training-1.6.0rc0/kubeflow_training.egg-info/PKG-INFO
--rw-r--r--   0 johnu.george   (502) staff       (20)     3502 2023-01-26 11:54:55.000000 kubeflow-training-1.6.0rc0/kubeflow_training.egg-info/SOURCES.txt
--rw-r--r--   0 johnu.george   (502) staff       (20)        1 2023-01-26 11:54:55.000000 kubeflow-training-1.6.0rc0/kubeflow_training.egg-info/dependency_links.txt
--rw-r--r--   0 johnu.george   (502) staff       (20)        1 2023-01-26 11:54:55.000000 kubeflow-training-1.6.0rc0/kubeflow_training.egg-info/not-zip-safe
--rw-r--r--   0 johnu.george   (502) staff       (20)      135 2023-01-26 11:54:55.000000 kubeflow-training-1.6.0rc0/kubeflow_training.egg-info/requires.txt
--rw-r--r--   0 johnu.george   (502) staff       (20)       14 2023-01-26 11:54:55.000000 kubeflow-training-1.6.0rc0/kubeflow_training.egg-info/top_level.txt
--rw-r--r--   0 johnu.george   (502) staff       (20)       38 2023-01-26 11:54:55.000000 kubeflow-training-1.6.0rc0/setup.cfg
--rw-r--r--   0 johnu.george   (502) staff       (20)     2256 2023-01-25 19:10:34.000000 kubeflow-training-1.6.0rc0/setup.py
-drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-01-26 11:54:55.000000 kubeflow-training-1.6.0rc0/test/
--rw-r--r--   0 johnu.george   (502) staff       (20)        0 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/__init__.py
-drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-01-26 11:54:55.000000 kubeflow-training-1.6.0rc0/test/e2e/
--rw-r--r--   0 johnu.george   (502) staff       (20)        0 2022-11-02 15:55:46.000000 kubeflow-training-1.6.0rc0/test/e2e/__init__.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     1004 2023-01-25 15:22:47.000000 kubeflow-training-1.6.0rc0/test/e2e/constants.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     5956 2023-01-25 15:22:47.000000 kubeflow-training-1.6.0rc0/test/e2e/test_e2e_mpijob.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     6927 2023-01-25 15:22:47.000000 kubeflow-training-1.6.0rc0/test/e2e/test_e2e_mxjob.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     4697 2023-01-25 15:22:47.000000 kubeflow-training-1.6.0rc0/test/e2e/test_e2e_paddlejob.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     5185 2023-01-25 15:22:47.000000 kubeflow-training-1.6.0rc0/test/e2e/test_e2e_pytorchjob.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     4657 2023-01-25 15:22:47.000000 kubeflow-training-1.6.0rc0/test/e2e/test_e2e_tfjob.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     5410 2023-01-25 15:22:47.000000 kubeflow-training-1.6.0rc0/test/e2e/test_e2e_xgboostjob.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     2956 2023-01-25 15:22:47.000000 kubeflow-training-1.6.0rc0/test/e2e/utils.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     2077 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_elastic_policy.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3535 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_mpi_job.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     6792 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_mpi_job_list.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     2641 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_mpi_job_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3426 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_mx_job.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     6549 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_mx_job_list.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3172 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_mx_job_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     1736 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_paddle_elastic_policy.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3790 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_paddle_job.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     7345 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_paddle_job_list.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3476 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_paddle_job_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     4291 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_py_torch_job.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     8516 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_py_torch_job_list.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3931 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_py_torch_job_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     1486 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_rdzv_conf.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3483 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_tf_job.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     6679 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_tf_job_list.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3193 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_tf_job_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3458 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_xg_boost_job.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     6562 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_xg_boost_job_list.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     3166 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_xg_boost_job_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     1616 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_v1_job_condition.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     2762 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_v1_job_status.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     1441 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_v1_replica_spec.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     1524 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_v1_replica_status.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     1821 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_v1_run_policy.py
--rw-r--r--   0 johnu.george   (502) staff       (20)     1636 2023-01-26 11:43:26.000000 kubeflow-training-1.6.0rc0/test/test_v1_scheduling_policy.py
+drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-08-07 13:02:53.053903 kubeflow-training-1.7.0rc0/
+-rw-r--r--   0 johnu.george   (502) staff       (20)     1172 2023-08-07 13:02:53.053446 kubeflow-training-1.7.0rc0/PKG-INFO
+-rw-r--r--   0 johnu.george   (502) staff       (20)     4650 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/README.md
+drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-08-07 13:02:52.936905 kubeflow-training-1.7.0rc0/kubeflow/
+-rw-r--r--   0 johnu.george   (502) staff       (20)       64 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/__init__.py
+drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-08-07 13:02:52.942718 kubeflow-training-1.7.0rc0/kubeflow/training/
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3289 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/__init__.py
+drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-08-07 13:02:52.944333 kubeflow-training-1.7.0rc0/kubeflow/training/api/
+-rw-r--r--   0 johnu.george   (502) staff       (20)       87 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/api/__init__.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)    59023 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/kubeflow/training/api/training_client.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)    26201 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/api_client.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)    12396 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/configuration.py
+drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-08-07 13:02:52.946778 kubeflow-training-1.7.0rc0/kubeflow/training/constants/
+-rw-r--r--   0 johnu.george   (502) staff       (20)      576 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/kubeflow/training/constants/__init__.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3478 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/kubeflow/training/constants/constants.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3728 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/exceptions.py
+drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-08-07 13:02:52.991722 kubeflow-training-1.7.0rc0/kubeflow/training/models/
+-rw-r--r--   0 johnu.george   (502) staff       (20)     2825 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/__init__.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)    14020 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_elastic_policy.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     8041 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_job_condition.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7372 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_job_status.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7331 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_mpi_job.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     6884 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_mpi_job_list.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     8054 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_mpi_job_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7304 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_mx_job.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     6861 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_mx_job_list.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     6267 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_mx_job_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7822 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_elastic_policy.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7412 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_job.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7037 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_job_list.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     6216 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_job_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7439 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_py_torch_job.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7062 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_py_torch_job_list.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7550 2023-08-07 07:02:03.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_py_torch_job_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3887 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_rdzv_conf.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     5455 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_replica_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7157 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_replica_status.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)    10117 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_run_policy.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     6941 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_scheduling_policy.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7304 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_tf_job.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     6937 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_tf_job_list.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7261 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_tf_job_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7439 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_xg_boost_job.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     6976 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_xg_boost_job_list.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     4816 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_xg_boost_job_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)    12263 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/kubeflow/training/rest.py
+drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-08-07 13:02:52.995394 kubeflow-training-1.7.0rc0/kubeflow/training/utils/
+-rw-r--r--   0 johnu.george   (502) staff       (20)      576 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/kubeflow/training/utils/__init__.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     9600 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/kubeflow/training/utils/utils.py
+drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-08-07 13:02:53.000849 kubeflow-training-1.7.0rc0/kubeflow_training.egg-info/
+-rw-r--r--   0 johnu.george   (502) staff       (20)     1172 2023-08-07 13:02:52.000000 kubeflow-training-1.7.0rc0/kubeflow_training.egg-info/PKG-INFO
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3675 2023-08-07 13:02:52.000000 kubeflow-training-1.7.0rc0/kubeflow_training.egg-info/SOURCES.txt
+-rw-r--r--   0 johnu.george   (502) staff       (20)        1 2023-08-07 13:02:52.000000 kubeflow-training-1.7.0rc0/kubeflow_training.egg-info/dependency_links.txt
+-rw-r--r--   0 johnu.george   (502) staff       (20)        1 2023-08-07 13:02:52.000000 kubeflow-training-1.7.0rc0/kubeflow_training.egg-info/not-zip-safe
+-rw-r--r--   0 johnu.george   (502) staff       (20)      135 2023-08-07 13:02:52.000000 kubeflow-training-1.7.0rc0/kubeflow_training.egg-info/requires.txt
+-rw-r--r--   0 johnu.george   (502) staff       (20)       14 2023-08-07 13:02:52.000000 kubeflow-training-1.7.0rc0/kubeflow_training.egg-info/top_level.txt
+-rw-r--r--   0 johnu.george   (502) staff       (20)       38 2023-08-07 13:02:53.054072 kubeflow-training-1.7.0rc0/setup.cfg
+-rw-r--r--   0 johnu.george   (502) staff       (20)     2256 2023-08-07 07:01:49.000000 kubeflow-training-1.7.0rc0/setup.py
+drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-08-07 13:02:53.026085 kubeflow-training-1.7.0rc0/test/
+-rw-r--r--   0 johnu.george   (502) staff       (20)        0 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/__init__.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)      213 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/conftest.py
+drwxr-xr-x   0 johnu.george   (502) staff       (20)        0 2023-08-07 13:02:53.052162 kubeflow-training-1.7.0rc0/test/e2e/
+-rw-r--r--   0 johnu.george   (502) staff       (20)        0 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/test/e2e/__init__.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     1004 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/test/e2e/constants.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     6838 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/test/e2e/test_e2e_mpijob.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     8176 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/test/e2e/test_e2e_mxjob.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     5227 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/test/e2e/test_e2e_paddlejob.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     6033 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/test/e2e/test_e2e_pytorchjob.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     5188 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/test/e2e/test_e2e_tfjob.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     6232 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/test/e2e/test_e2e_xgboostjob.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3180 2023-08-07 05:36:49.000000 kubeflow-training-1.7.0rc0/test/e2e/utils.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     2077 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_elastic_policy.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     1741 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_job_condition.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     2308 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_job_status.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3820 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_mpi_job.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7378 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_mpi_job_list.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     2841 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_mpi_job_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3711 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_mx_job.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7135 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_mx_job_list.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3492 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_mx_job_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     1736 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_paddle_elastic_policy.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     4075 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_paddle_job.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7931 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_paddle_job_list.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3796 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_paddle_job_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     4619 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_py_torch_job.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     9204 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_py_torch_job_list.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     4290 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_py_torch_job_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     1486 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_rdzv_conf.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     1566 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_replica_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     1649 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_replica_status.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     2024 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_run_policy.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     1761 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_scheduling_policy.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3768 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_tf_job.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7265 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_tf_job_list.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3513 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_tf_job_spec.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3743 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_xg_boost_job.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     7148 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_xg_boost_job_list.py
+-rw-r--r--   0 johnu.george   (502) staff       (20)     3486 2023-08-07 07:02:04.000000 kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_xg_boost_job_spec.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `kubeflow-training-1.6.0rc0/PKG-INFO` & `kubeflow-training-1.7.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: kubeflow-training
-Version: 1.6.0rc0
+Version: 1.7.0rc0
 Summary: Training Operator Python SDK
 Home-page: https://github.com/kubeflow/training-operator/sdk/python
 Author: Kubeflow Authors
 Author-email: hejinchi@cn.ibm.com
 License: Apache License Version 2.0
-Description: Training Operator Python SDK
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
@@ -21,7 +20,10 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: test
+
+Training Operator Python SDK
+
```

### Comparing `kubeflow-training-1.6.0rc0/README.md` & `kubeflow-training-1.7.0rc0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -77,7 +77,15 @@
  - [V1SchedulingPolicy](docs/V1SchedulingPolicy.md)
  - [V1TFJob](docs/KubeflowOrgV1TFJob.md)
  - [V1TFJobList](docs/KubeflowOrgV1TFJobList.md)
  - [V1TFJobSpec](docs/KubeflowOrgV1TFJobSpec.md)
  - [V1XGBoostJob](docs/KubeflowOrgV1XGBoostJob.md)
  - [V1XGBoostJobList](docs/KubeflowOrgV1XGBoostJobList.md)
  - [V1XGBoostJobSpec](docs/KubeflowOrgV1XGBoostJobSpec.md)
+
+
+## Building conformance tests
+
+Run
+```
+docker build . -f Dockerfile.conformance -t <tag>
+```
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/__init__.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,56 +3,56 @@
 # flake8: noqa
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.5.0"
+__version__ = "1.7.0rc0"
 
 # import apis into sdk package
 
 # import ApiClient
 from kubeflow.training.api_client import ApiClient
 from kubeflow.training.configuration import Configuration
 from kubeflow.training.exceptions import OpenApiException
 from kubeflow.training.exceptions import ApiTypeError
 from kubeflow.training.exceptions import ApiValueError
 from kubeflow.training.exceptions import ApiKeyError
 from kubeflow.training.exceptions import ApiException
 # import models into sdk package
 from kubeflow.training.models.kubeflow_org_v1_elastic_policy import KubeflowOrgV1ElasticPolicy
+from kubeflow.training.models.kubeflow_org_v1_job_condition import KubeflowOrgV1JobCondition
+from kubeflow.training.models.kubeflow_org_v1_job_status import KubeflowOrgV1JobStatus
 from kubeflow.training.models.kubeflow_org_v1_mpi_job import KubeflowOrgV1MPIJob
 from kubeflow.training.models.kubeflow_org_v1_mpi_job_list import KubeflowOrgV1MPIJobList
 from kubeflow.training.models.kubeflow_org_v1_mpi_job_spec import KubeflowOrgV1MPIJobSpec
 from kubeflow.training.models.kubeflow_org_v1_mx_job import KubeflowOrgV1MXJob
 from kubeflow.training.models.kubeflow_org_v1_mx_job_list import KubeflowOrgV1MXJobList
 from kubeflow.training.models.kubeflow_org_v1_mx_job_spec import KubeflowOrgV1MXJobSpec
 from kubeflow.training.models.kubeflow_org_v1_paddle_elastic_policy import KubeflowOrgV1PaddleElasticPolicy
 from kubeflow.training.models.kubeflow_org_v1_paddle_job import KubeflowOrgV1PaddleJob
 from kubeflow.training.models.kubeflow_org_v1_paddle_job_list import KubeflowOrgV1PaddleJobList
 from kubeflow.training.models.kubeflow_org_v1_paddle_job_spec import KubeflowOrgV1PaddleJobSpec
 from kubeflow.training.models.kubeflow_org_v1_py_torch_job import KubeflowOrgV1PyTorchJob
 from kubeflow.training.models.kubeflow_org_v1_py_torch_job_list import KubeflowOrgV1PyTorchJobList
 from kubeflow.training.models.kubeflow_org_v1_py_torch_job_spec import KubeflowOrgV1PyTorchJobSpec
 from kubeflow.training.models.kubeflow_org_v1_rdzv_conf import KubeflowOrgV1RDZVConf
+from kubeflow.training.models.kubeflow_org_v1_replica_spec import KubeflowOrgV1ReplicaSpec
+from kubeflow.training.models.kubeflow_org_v1_replica_status import KubeflowOrgV1ReplicaStatus
+from kubeflow.training.models.kubeflow_org_v1_run_policy import KubeflowOrgV1RunPolicy
+from kubeflow.training.models.kubeflow_org_v1_scheduling_policy import KubeflowOrgV1SchedulingPolicy
 from kubeflow.training.models.kubeflow_org_v1_tf_job import KubeflowOrgV1TFJob
 from kubeflow.training.models.kubeflow_org_v1_tf_job_list import KubeflowOrgV1TFJobList
 from kubeflow.training.models.kubeflow_org_v1_tf_job_spec import KubeflowOrgV1TFJobSpec
 from kubeflow.training.models.kubeflow_org_v1_xg_boost_job import KubeflowOrgV1XGBoostJob
 from kubeflow.training.models.kubeflow_org_v1_xg_boost_job_list import KubeflowOrgV1XGBoostJobList
 from kubeflow.training.models.kubeflow_org_v1_xg_boost_job_spec import KubeflowOrgV1XGBoostJobSpec
-from kubeflow.training.models.v1_job_condition import V1JobCondition
-from kubeflow.training.models.v1_job_status import V1JobStatus
-from kubeflow.training.models.v1_replica_spec import V1ReplicaSpec
-from kubeflow.training.models.v1_replica_status import V1ReplicaStatus
-from kubeflow.training.models.v1_run_policy import V1RunPolicy
-from kubeflow.training.models.v1_scheduling_policy import V1SchedulingPolicy
 
 from kubeflow.training.api.training_client import TrainingClient
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/api/training_client.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/api/training_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -573,15 +573,15 @@
                 try:
                     pod_logs = self.core_api.read_namespaced_pod_log(
                         pod, namespace, container=container
                     )
                     logging.info("The logs of pod %s:\n %s", pod, pod_logs)
                 except Exception:
                     raise RuntimeError(
-                        f"Failed to read logs for pod {namespace}/{pod.metadata.name}"
+                        f"Failed to read logs for pod {namespace}/{pod}"
                     )
 
     # ------------------------------------------------------------------------ #
     # TFJob Training Client APIs.
     # ------------------------------------------------------------------------ #
     def create_tfjob(
         self,
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/api_client.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
 import datetime
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.5.0/python'
+        self.user_agent = 'OpenAPI-Generator/1.7.0rc0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/configuration.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import copy
@@ -320,16 +320,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: v1.6.0rc0\n"\
-               "SDK Package Version: 1.5.0".\
+               "Version of the API: v1.7.0rc0\n"\
+               "SDK Package Version: 1.7.0rc0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/constants/__init__.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/constants/constants.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/constants/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 # How long to wait in seconds for requests to the Kubernetes API Server.
 DEFAULT_TIMEOUT = 120
 
 # Common constants.
 KUBEFLOW_GROUP = "kubeflow.org"
 OPERATOR_VERSION = "v1"
+ISTIO_SIDECAR_INJECTION = "sidecar.istio.io/inject"
 
 # Training Job conditions.
 JOB_CONDITION_CREATED = "Created"
 JOB_CONDITION_RUNNING = "Running"
 JOB_CONDITION_RESTARTING = "Restarting"
 JOB_CONDITION_SUCCEEDED = "Succeeded"
 JOB_CONDITION_FAILED = "Failed"
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/exceptions.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/__init__.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,45 +2,45 @@
 
 # flake8: noqa
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # Import Kubernetes models.
 from kubernetes.client import *
 
 # import models into model package
 from kubeflow.training.models.kubeflow_org_v1_elastic_policy import KubeflowOrgV1ElasticPolicy
+from kubeflow.training.models.kubeflow_org_v1_job_condition import KubeflowOrgV1JobCondition
+from kubeflow.training.models.kubeflow_org_v1_job_status import KubeflowOrgV1JobStatus
 from kubeflow.training.models.kubeflow_org_v1_mpi_job import KubeflowOrgV1MPIJob
 from kubeflow.training.models.kubeflow_org_v1_mpi_job_list import KubeflowOrgV1MPIJobList
 from kubeflow.training.models.kubeflow_org_v1_mpi_job_spec import KubeflowOrgV1MPIJobSpec
 from kubeflow.training.models.kubeflow_org_v1_mx_job import KubeflowOrgV1MXJob
 from kubeflow.training.models.kubeflow_org_v1_mx_job_list import KubeflowOrgV1MXJobList
 from kubeflow.training.models.kubeflow_org_v1_mx_job_spec import KubeflowOrgV1MXJobSpec
 from kubeflow.training.models.kubeflow_org_v1_paddle_elastic_policy import KubeflowOrgV1PaddleElasticPolicy
 from kubeflow.training.models.kubeflow_org_v1_paddle_job import KubeflowOrgV1PaddleJob
 from kubeflow.training.models.kubeflow_org_v1_paddle_job_list import KubeflowOrgV1PaddleJobList
 from kubeflow.training.models.kubeflow_org_v1_paddle_job_spec import KubeflowOrgV1PaddleJobSpec
 from kubeflow.training.models.kubeflow_org_v1_py_torch_job import KubeflowOrgV1PyTorchJob
 from kubeflow.training.models.kubeflow_org_v1_py_torch_job_list import KubeflowOrgV1PyTorchJobList
 from kubeflow.training.models.kubeflow_org_v1_py_torch_job_spec import KubeflowOrgV1PyTorchJobSpec
 from kubeflow.training.models.kubeflow_org_v1_rdzv_conf import KubeflowOrgV1RDZVConf
+from kubeflow.training.models.kubeflow_org_v1_replica_spec import KubeflowOrgV1ReplicaSpec
+from kubeflow.training.models.kubeflow_org_v1_replica_status import KubeflowOrgV1ReplicaStatus
+from kubeflow.training.models.kubeflow_org_v1_run_policy import KubeflowOrgV1RunPolicy
+from kubeflow.training.models.kubeflow_org_v1_scheduling_policy import KubeflowOrgV1SchedulingPolicy
 from kubeflow.training.models.kubeflow_org_v1_tf_job import KubeflowOrgV1TFJob
 from kubeflow.training.models.kubeflow_org_v1_tf_job_list import KubeflowOrgV1TFJobList
 from kubeflow.training.models.kubeflow_org_v1_tf_job_spec import KubeflowOrgV1TFJobSpec
 from kubeflow.training.models.kubeflow_org_v1_xg_boost_job import KubeflowOrgV1XGBoostJob
 from kubeflow.training.models.kubeflow_org_v1_xg_boost_job_list import KubeflowOrgV1XGBoostJobList
 from kubeflow.training.models.kubeflow_org_v1_xg_boost_job_spec import KubeflowOrgV1XGBoostJobSpec
-from kubeflow.training.models.v1_job_condition import V1JobCondition
-from kubeflow.training.models.v1_job_status import V1JobStatus
-from kubeflow.training.models.v1_replica_spec import V1ReplicaSpec
-from kubeflow.training.models.v1_replica_status import V1ReplicaStatus
-from kubeflow.training.models.v1_run_policy import V1RunPolicy
-from kubeflow.training.models.v1_scheduling_policy import V1SchedulingPolicy
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_elastic_policy.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_elastic_policy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -192,26 +192,26 @@
 
         self._min_replicas = min_replicas
 
     @property
     def n_proc_per_node(self):
         """Gets the n_proc_per_node of this KubeflowOrgV1ElasticPolicy.  # noqa: E501
 
-        Number of workers per node; supported values: [auto, cpu, gpu, int].  # noqa: E501
+        Number of workers per node; supported values: [auto, cpu, gpu, int]. Deprecated: This API is deprecated in v1.7+ Use .spec.nprocPerNode instead.  # noqa: E501
 
         :return: The n_proc_per_node of this KubeflowOrgV1ElasticPolicy.  # noqa: E501
         :rtype: int
         """
         return self._n_proc_per_node
 
     @n_proc_per_node.setter
     def n_proc_per_node(self, n_proc_per_node):
         """Sets the n_proc_per_node of this KubeflowOrgV1ElasticPolicy.
 
-        Number of workers per node; supported values: [auto, cpu, gpu, int].  # noqa: E501
+        Number of workers per node; supported values: [auto, cpu, gpu, int]. Deprecated: This API is deprecated in v1.7+ Use .spec.nprocPerNode instead.  # noqa: E501
 
         :param n_proc_per_node: The n_proc_per_node of this KubeflowOrgV1ElasticPolicy.  # noqa: E501
         :type: int
         """
 
         self._n_proc_per_node = n_proc_per_node
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_mpi_job.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_mpi_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -33,15 +33,15 @@
                             and the value is json key in definition.
     """
     openapi_types = {
         'api_version': 'str',
         'kind': 'str',
         'metadata': 'V1ObjectMeta',
         'spec': 'KubeflowOrgV1MPIJobSpec',
-        'status': 'V1JobStatus'
+        'status': 'KubeflowOrgV1JobStatus'
     }
 
     attribute_map = {
         'api_version': 'apiVersion',
         'kind': 'kind',
         'metadata': 'metadata',
         'spec': 'spec',
@@ -162,25 +162,25 @@
 
     @property
     def status(self):
         """Gets the status of this KubeflowOrgV1MPIJob.  # noqa: E501
 
 
         :return: The status of this KubeflowOrgV1MPIJob.  # noqa: E501
-        :rtype: V1JobStatus
+        :rtype: KubeflowOrgV1JobStatus
         """
         return self._status
 
     @status.setter
     def status(self, status):
         """Sets the status of this KubeflowOrgV1MPIJob.
 
 
         :param status: The status of this KubeflowOrgV1MPIJob.  # noqa: E501
-        :type: V1JobStatus
+        :type: KubeflowOrgV1JobStatus
         """
 
         self._status = status
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_mpi_job_list.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_mpi_job_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_mpi_job_spec.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_mpi_job_spec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -31,16 +31,16 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'clean_pod_policy': 'str',
         'main_container': 'str',
-        'mpi_replica_specs': 'dict(str, V1ReplicaSpec)',
-        'run_policy': 'V1RunPolicy',
+        'mpi_replica_specs': 'dict(str, KubeflowOrgV1ReplicaSpec)',
+        'run_policy': 'KubeflowOrgV1RunPolicy',
         'slots_per_worker': 'int'
     }
 
     attribute_map = {
         'clean_pod_policy': 'cleanPodPolicy',
         'main_container': 'mainContainer',
         'mpi_replica_specs': 'mpiReplicaSpecs',
@@ -120,49 +120,49 @@
     @property
     def mpi_replica_specs(self):
         """Gets the mpi_replica_specs of this KubeflowOrgV1MPIJobSpec.  # noqa: E501
 
         `MPIReplicaSpecs` contains maps from `MPIReplicaType` to `ReplicaSpec` that specify the MPI replicas to run.  # noqa: E501
 
         :return: The mpi_replica_specs of this KubeflowOrgV1MPIJobSpec.  # noqa: E501
-        :rtype: dict(str, V1ReplicaSpec)
+        :rtype: dict(str, KubeflowOrgV1ReplicaSpec)
         """
         return self._mpi_replica_specs
 
     @mpi_replica_specs.setter
     def mpi_replica_specs(self, mpi_replica_specs):
         """Sets the mpi_replica_specs of this KubeflowOrgV1MPIJobSpec.
 
         `MPIReplicaSpecs` contains maps from `MPIReplicaType` to `ReplicaSpec` that specify the MPI replicas to run.  # noqa: E501
 
         :param mpi_replica_specs: The mpi_replica_specs of this KubeflowOrgV1MPIJobSpec.  # noqa: E501
-        :type: dict(str, V1ReplicaSpec)
+        :type: dict(str, KubeflowOrgV1ReplicaSpec)
         """
         if self.local_vars_configuration.client_side_validation and mpi_replica_specs is None:  # noqa: E501
             raise ValueError("Invalid value for `mpi_replica_specs`, must not be `None`")  # noqa: E501
 
         self._mpi_replica_specs = mpi_replica_specs
 
     @property
     def run_policy(self):
         """Gets the run_policy of this KubeflowOrgV1MPIJobSpec.  # noqa: E501
 
 
         :return: The run_policy of this KubeflowOrgV1MPIJobSpec.  # noqa: E501
-        :rtype: V1RunPolicy
+        :rtype: KubeflowOrgV1RunPolicy
         """
         return self._run_policy
 
     @run_policy.setter
     def run_policy(self, run_policy):
         """Sets the run_policy of this KubeflowOrgV1MPIJobSpec.
 
 
         :param run_policy: The run_policy of this KubeflowOrgV1MPIJobSpec.  # noqa: E501
-        :type: V1RunPolicy
+        :type: KubeflowOrgV1RunPolicy
         """
 
         self._run_policy = run_policy
 
     @property
     def slots_per_worker(self):
         """Gets the slots_per_worker of this KubeflowOrgV1MPIJobSpec.  # noqa: E501
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_mx_job.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_mx_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -33,15 +33,15 @@
                             and the value is json key in definition.
     """
     openapi_types = {
         'api_version': 'str',
         'kind': 'str',
         'metadata': 'V1ObjectMeta',
         'spec': 'KubeflowOrgV1MXJobSpec',
-        'status': 'V1JobStatus'
+        'status': 'KubeflowOrgV1JobStatus'
     }
 
     attribute_map = {
         'api_version': 'apiVersion',
         'kind': 'kind',
         'metadata': 'metadata',
         'spec': 'spec',
@@ -162,25 +162,25 @@
 
     @property
     def status(self):
         """Gets the status of this KubeflowOrgV1MXJob.  # noqa: E501
 
 
         :return: The status of this KubeflowOrgV1MXJob.  # noqa: E501
-        :rtype: V1JobStatus
+        :rtype: KubeflowOrgV1JobStatus
         """
         return self._status
 
     @status.setter
     def status(self, status):
         """Sets the status of this KubeflowOrgV1MXJob.
 
 
         :param status: The status of this KubeflowOrgV1MXJob.  # noqa: E501
-        :type: V1JobStatus
+        :type: KubeflowOrgV1JobStatus
         """
 
         self._status = status
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_mx_job_list.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_mx_job_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_mx_job_spec.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_mx_job_spec.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -30,16 +30,16 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'job_mode': 'str',
-        'mx_replica_specs': 'dict(str, V1ReplicaSpec)',
-        'run_policy': 'V1RunPolicy'
+        'mx_replica_specs': 'dict(str, KubeflowOrgV1ReplicaSpec)',
+        'run_policy': 'KubeflowOrgV1RunPolicy'
     }
 
     attribute_map = {
         'job_mode': 'jobMode',
         'mx_replica_specs': 'mxReplicaSpecs',
         'run_policy': 'runPolicy'
     }
@@ -84,52 +84,52 @@
 
         self._job_mode = job_mode
 
     @property
     def mx_replica_specs(self):
         """Gets the mx_replica_specs of this KubeflowOrgV1MXJobSpec.  # noqa: E501
 
-        MXReplicaSpecs is map of commonv1.ReplicaType and commonv1.ReplicaSpec specifies the MX replicas to run. For example,   {     \"Scheduler\": commonv1.ReplicaSpec,     \"Server\": commonv1.ReplicaSpec,     \"Worker\": commonv1.ReplicaSpec,   }  # noqa: E501
+        MXReplicaSpecs is map of ReplicaType and ReplicaSpec specifies the MX replicas to run. For example,   {     \"Scheduler\": ReplicaSpec,     \"Server\": ReplicaSpec,     \"Worker\": ReplicaSpec,   }  # noqa: E501
 
         :return: The mx_replica_specs of this KubeflowOrgV1MXJobSpec.  # noqa: E501
-        :rtype: dict(str, V1ReplicaSpec)
+        :rtype: dict(str, KubeflowOrgV1ReplicaSpec)
         """
         return self._mx_replica_specs
 
     @mx_replica_specs.setter
     def mx_replica_specs(self, mx_replica_specs):
         """Sets the mx_replica_specs of this KubeflowOrgV1MXJobSpec.
 
-        MXReplicaSpecs is map of commonv1.ReplicaType and commonv1.ReplicaSpec specifies the MX replicas to run. For example,   {     \"Scheduler\": commonv1.ReplicaSpec,     \"Server\": commonv1.ReplicaSpec,     \"Worker\": commonv1.ReplicaSpec,   }  # noqa: E501
+        MXReplicaSpecs is map of ReplicaType and ReplicaSpec specifies the MX replicas to run. For example,   {     \"Scheduler\": ReplicaSpec,     \"Server\": ReplicaSpec,     \"Worker\": ReplicaSpec,   }  # noqa: E501
 
         :param mx_replica_specs: The mx_replica_specs of this KubeflowOrgV1MXJobSpec.  # noqa: E501
-        :type: dict(str, V1ReplicaSpec)
+        :type: dict(str, KubeflowOrgV1ReplicaSpec)
         """
         if self.local_vars_configuration.client_side_validation and mx_replica_specs is None:  # noqa: E501
             raise ValueError("Invalid value for `mx_replica_specs`, must not be `None`")  # noqa: E501
 
         self._mx_replica_specs = mx_replica_specs
 
     @property
     def run_policy(self):
         """Gets the run_policy of this KubeflowOrgV1MXJobSpec.  # noqa: E501
 
 
         :return: The run_policy of this KubeflowOrgV1MXJobSpec.  # noqa: E501
-        :rtype: V1RunPolicy
+        :rtype: KubeflowOrgV1RunPolicy
         """
         return self._run_policy
 
     @run_policy.setter
     def run_policy(self, run_policy):
         """Sets the run_policy of this KubeflowOrgV1MXJobSpec.
 
 
         :param run_policy: The run_policy of this KubeflowOrgV1MXJobSpec.  # noqa: E501
-        :type: V1RunPolicy
+        :type: KubeflowOrgV1RunPolicy
         """
         if self.local_vars_configuration.client_side_validation and run_policy is None:  # noqa: E501
             raise ValueError("Invalid value for `run_policy`, must not be `None`")  # noqa: E501
 
         self._run_policy = run_policy
 
     def to_dict(self):
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_elastic_policy.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_elastic_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_job.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -33,15 +33,15 @@
                             and the value is json key in definition.
     """
     openapi_types = {
         'api_version': 'str',
         'kind': 'str',
         'metadata': 'V1ObjectMeta',
         'spec': 'KubeflowOrgV1PaddleJobSpec',
-        'status': 'V1JobStatus'
+        'status': 'KubeflowOrgV1JobStatus'
     }
 
     attribute_map = {
         'api_version': 'apiVersion',
         'kind': 'kind',
         'metadata': 'metadata',
         'spec': 'spec',
@@ -162,25 +162,25 @@
 
     @property
     def status(self):
         """Gets the status of this KubeflowOrgV1PaddleJob.  # noqa: E501
 
 
         :return: The status of this KubeflowOrgV1PaddleJob.  # noqa: E501
-        :rtype: V1JobStatus
+        :rtype: KubeflowOrgV1JobStatus
         """
         return self._status
 
     @status.setter
     def status(self, status):
         """Sets the status of this KubeflowOrgV1PaddleJob.
 
 
         :param status: The status of this KubeflowOrgV1PaddleJob.  # noqa: E501
-        :type: V1JobStatus
+        :type: KubeflowOrgV1JobStatus
         """
 
         self._status = status
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_job_list.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_job_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_job_spec.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_paddle_job_spec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -30,16 +30,16 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'elastic_policy': 'KubeflowOrgV1PaddleElasticPolicy',
-        'paddle_replica_specs': 'dict(str, V1ReplicaSpec)',
-        'run_policy': 'V1RunPolicy'
+        'paddle_replica_specs': 'dict(str, KubeflowOrgV1ReplicaSpec)',
+        'run_policy': 'KubeflowOrgV1RunPolicy'
     }
 
     attribute_map = {
         'elastic_policy': 'elasticPolicy',
         'paddle_replica_specs': 'paddleReplicaSpecs',
         'run_policy': 'runPolicy'
     }
@@ -84,49 +84,49 @@
     @property
     def paddle_replica_specs(self):
         """Gets the paddle_replica_specs of this KubeflowOrgV1PaddleJobSpec.  # noqa: E501
 
         A map of PaddleReplicaType (type) to ReplicaSpec (value). Specifies the Paddle cluster configuration. For example,   {     \"Master\": PaddleReplicaSpec,     \"Worker\": PaddleReplicaSpec,   }  # noqa: E501
 
         :return: The paddle_replica_specs of this KubeflowOrgV1PaddleJobSpec.  # noqa: E501
-        :rtype: dict(str, V1ReplicaSpec)
+        :rtype: dict(str, KubeflowOrgV1ReplicaSpec)
         """
         return self._paddle_replica_specs
 
     @paddle_replica_specs.setter
     def paddle_replica_specs(self, paddle_replica_specs):
         """Sets the paddle_replica_specs of this KubeflowOrgV1PaddleJobSpec.
 
         A map of PaddleReplicaType (type) to ReplicaSpec (value). Specifies the Paddle cluster configuration. For example,   {     \"Master\": PaddleReplicaSpec,     \"Worker\": PaddleReplicaSpec,   }  # noqa: E501
 
         :param paddle_replica_specs: The paddle_replica_specs of this KubeflowOrgV1PaddleJobSpec.  # noqa: E501
-        :type: dict(str, V1ReplicaSpec)
+        :type: dict(str, KubeflowOrgV1ReplicaSpec)
         """
         if self.local_vars_configuration.client_side_validation and paddle_replica_specs is None:  # noqa: E501
             raise ValueError("Invalid value for `paddle_replica_specs`, must not be `None`")  # noqa: E501
 
         self._paddle_replica_specs = paddle_replica_specs
 
     @property
     def run_policy(self):
         """Gets the run_policy of this KubeflowOrgV1PaddleJobSpec.  # noqa: E501
 
 
         :return: The run_policy of this KubeflowOrgV1PaddleJobSpec.  # noqa: E501
-        :rtype: V1RunPolicy
+        :rtype: KubeflowOrgV1RunPolicy
         """
         return self._run_policy
 
     @run_policy.setter
     def run_policy(self, run_policy):
         """Sets the run_policy of this KubeflowOrgV1PaddleJobSpec.
 
 
         :param run_policy: The run_policy of this KubeflowOrgV1PaddleJobSpec.  # noqa: E501
-        :type: V1RunPolicy
+        :type: KubeflowOrgV1RunPolicy
         """
         if self.local_vars_configuration.client_side_validation and run_policy is None:  # noqa: E501
             raise ValueError("Invalid value for `run_policy`, must not be `None`")  # noqa: E501
 
         self._run_policy = run_policy
 
     def to_dict(self):
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_py_torch_job.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_py_torch_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -33,15 +33,15 @@
                             and the value is json key in definition.
     """
     openapi_types = {
         'api_version': 'str',
         'kind': 'str',
         'metadata': 'V1ObjectMeta',
         'spec': 'KubeflowOrgV1PyTorchJobSpec',
-        'status': 'V1JobStatus'
+        'status': 'KubeflowOrgV1JobStatus'
     }
 
     attribute_map = {
         'api_version': 'apiVersion',
         'kind': 'kind',
         'metadata': 'metadata',
         'spec': 'spec',
@@ -162,25 +162,25 @@
 
     @property
     def status(self):
         """Gets the status of this KubeflowOrgV1PyTorchJob.  # noqa: E501
 
 
         :return: The status of this KubeflowOrgV1PyTorchJob.  # noqa: E501
-        :rtype: V1JobStatus
+        :rtype: KubeflowOrgV1JobStatus
         """
         return self._status
 
     @status.setter
     def status(self, status):
         """Sets the status of this KubeflowOrgV1PyTorchJob.
 
 
         :param status: The status of this KubeflowOrgV1PyTorchJob.  # noqa: E501
-        :type: V1JobStatus
+        :type: KubeflowOrgV1JobStatus
         """
 
         self._status = status
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_py_torch_job_list.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_py_torch_job_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_rdzv_conf.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_rdzv_conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_tf_job.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_tf_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -33,15 +33,15 @@
                             and the value is json key in definition.
     """
     openapi_types = {
         'api_version': 'str',
         'kind': 'str',
         'metadata': 'V1ObjectMeta',
         'spec': 'KubeflowOrgV1TFJobSpec',
-        'status': 'V1JobStatus'
+        'status': 'KubeflowOrgV1JobStatus'
     }
 
     attribute_map = {
         'api_version': 'apiVersion',
         'kind': 'kind',
         'metadata': 'metadata',
         'spec': 'spec',
@@ -162,25 +162,25 @@
 
     @property
     def status(self):
         """Gets the status of this KubeflowOrgV1TFJob.  # noqa: E501
 
 
         :return: The status of this KubeflowOrgV1TFJob.  # noqa: E501
-        :rtype: V1JobStatus
+        :rtype: KubeflowOrgV1JobStatus
         """
         return self._status
 
     @status.setter
     def status(self, status):
         """Sets the status of this KubeflowOrgV1TFJob.
 
 
         :param status: The status of this KubeflowOrgV1TFJob.  # noqa: E501
-        :type: V1JobStatus
+        :type: KubeflowOrgV1JobStatus
         """
 
         self._status = status
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_tf_job_list.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_tf_job_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_tf_job_spec.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_tf_job_spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -30,17 +30,17 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'enable_dynamic_worker': 'bool',
-        'run_policy': 'V1RunPolicy',
+        'run_policy': 'KubeflowOrgV1RunPolicy',
         'success_policy': 'str',
-        'tf_replica_specs': 'dict(str, V1ReplicaSpec)'
+        'tf_replica_specs': 'dict(str, KubeflowOrgV1ReplicaSpec)'
     }
 
     attribute_map = {
         'enable_dynamic_worker': 'enableDynamicWorker',
         'run_policy': 'runPolicy',
         'success_policy': 'successPolicy',
         'tf_replica_specs': 'tfReplicaSpecs'
@@ -90,25 +90,25 @@
 
     @property
     def run_policy(self):
         """Gets the run_policy of this KubeflowOrgV1TFJobSpec.  # noqa: E501
 
 
         :return: The run_policy of this KubeflowOrgV1TFJobSpec.  # noqa: E501
-        :rtype: V1RunPolicy
+        :rtype: KubeflowOrgV1RunPolicy
         """
         return self._run_policy
 
     @run_policy.setter
     def run_policy(self, run_policy):
         """Sets the run_policy of this KubeflowOrgV1TFJobSpec.
 
 
         :param run_policy: The run_policy of this KubeflowOrgV1TFJobSpec.  # noqa: E501
-        :type: V1RunPolicy
+        :type: KubeflowOrgV1RunPolicy
         """
         if self.local_vars_configuration.client_side_validation and run_policy is None:  # noqa: E501
             raise ValueError("Invalid value for `run_policy`, must not be `None`")  # noqa: E501
 
         self._run_policy = run_policy
 
     @property
@@ -137,26 +137,26 @@
     @property
     def tf_replica_specs(self):
         """Gets the tf_replica_specs of this KubeflowOrgV1TFJobSpec.  # noqa: E501
 
         A map of TFReplicaType (type) to ReplicaSpec (value). Specifies the TF cluster configuration. For example,   {     \"PS\": ReplicaSpec,     \"Worker\": ReplicaSpec,   }  # noqa: E501
 
         :return: The tf_replica_specs of this KubeflowOrgV1TFJobSpec.  # noqa: E501
-        :rtype: dict(str, V1ReplicaSpec)
+        :rtype: dict(str, KubeflowOrgV1ReplicaSpec)
         """
         return self._tf_replica_specs
 
     @tf_replica_specs.setter
     def tf_replica_specs(self, tf_replica_specs):
         """Sets the tf_replica_specs of this KubeflowOrgV1TFJobSpec.
 
         A map of TFReplicaType (type) to ReplicaSpec (value). Specifies the TF cluster configuration. For example,   {     \"PS\": ReplicaSpec,     \"Worker\": ReplicaSpec,   }  # noqa: E501
 
         :param tf_replica_specs: The tf_replica_specs of this KubeflowOrgV1TFJobSpec.  # noqa: E501
-        :type: dict(str, V1ReplicaSpec)
+        :type: dict(str, KubeflowOrgV1ReplicaSpec)
         """
         if self.local_vars_configuration.client_side_validation and tf_replica_specs is None:  # noqa: E501
             raise ValueError("Invalid value for `tf_replica_specs`, must not be `None`")  # noqa: E501
 
         self._tf_replica_specs = tf_replica_specs
 
     def to_dict(self):
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_xg_boost_job.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_xg_boost_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -33,15 +33,15 @@
                             and the value is json key in definition.
     """
     openapi_types = {
         'api_version': 'str',
         'kind': 'str',
         'metadata': 'V1ObjectMeta',
         'spec': 'KubeflowOrgV1XGBoostJobSpec',
-        'status': 'V1JobStatus'
+        'status': 'KubeflowOrgV1JobStatus'
     }
 
     attribute_map = {
         'api_version': 'apiVersion',
         'kind': 'kind',
         'metadata': 'metadata',
         'spec': 'spec',
@@ -162,25 +162,25 @@
 
     @property
     def status(self):
         """Gets the status of this KubeflowOrgV1XGBoostJob.  # noqa: E501
 
 
         :return: The status of this KubeflowOrgV1XGBoostJob.  # noqa: E501
-        :rtype: V1JobStatus
+        :rtype: KubeflowOrgV1JobStatus
         """
         return self._status
 
     @status.setter
     def status(self, status):
         """Sets the status of this KubeflowOrgV1XGBoostJob.
 
 
         :param status: The status of this KubeflowOrgV1XGBoostJob.  # noqa: E501
-        :type: V1JobStatus
+        :type: KubeflowOrgV1JobStatus
         """
 
         self._status = status
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_xg_boost_job_list.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_xg_boost_job_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/kubeflow_org_v1_xg_boost_job_spec.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_xg_boost_job_spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -29,16 +29,16 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'run_policy': 'V1RunPolicy',
-        'xgb_replica_specs': 'dict(str, V1ReplicaSpec)'
+        'run_policy': 'KubeflowOrgV1RunPolicy',
+        'xgb_replica_specs': 'dict(str, KubeflowOrgV1ReplicaSpec)'
     }
 
     attribute_map = {
         'run_policy': 'runPolicy',
         'xgb_replica_specs': 'xgbReplicaSpecs'
     }
 
@@ -57,48 +57,48 @@
 
     @property
     def run_policy(self):
         """Gets the run_policy of this KubeflowOrgV1XGBoostJobSpec.  # noqa: E501
 
 
         :return: The run_policy of this KubeflowOrgV1XGBoostJobSpec.  # noqa: E501
-        :rtype: V1RunPolicy
+        :rtype: KubeflowOrgV1RunPolicy
         """
         return self._run_policy
 
     @run_policy.setter
     def run_policy(self, run_policy):
         """Sets the run_policy of this KubeflowOrgV1XGBoostJobSpec.
 
 
         :param run_policy: The run_policy of this KubeflowOrgV1XGBoostJobSpec.  # noqa: E501
-        :type: V1RunPolicy
+        :type: KubeflowOrgV1RunPolicy
         """
         if self.local_vars_configuration.client_side_validation and run_policy is None:  # noqa: E501
             raise ValueError("Invalid value for `run_policy`, must not be `None`")  # noqa: E501
 
         self._run_policy = run_policy
 
     @property
     def xgb_replica_specs(self):
         """Gets the xgb_replica_specs of this KubeflowOrgV1XGBoostJobSpec.  # noqa: E501
 
 
         :return: The xgb_replica_specs of this KubeflowOrgV1XGBoostJobSpec.  # noqa: E501
-        :rtype: dict(str, V1ReplicaSpec)
+        :rtype: dict(str, KubeflowOrgV1ReplicaSpec)
         """
         return self._xgb_replica_specs
 
     @xgb_replica_specs.setter
     def xgb_replica_specs(self, xgb_replica_specs):
         """Sets the xgb_replica_specs of this KubeflowOrgV1XGBoostJobSpec.
 
 
         :param xgb_replica_specs: The xgb_replica_specs of this KubeflowOrgV1XGBoostJobSpec.  # noqa: E501
-        :type: dict(str, V1ReplicaSpec)
+        :type: dict(str, KubeflowOrgV1ReplicaSpec)
         """
         if self.local_vars_configuration.client_side_validation and xgb_replica_specs is None:  # noqa: E501
             raise ValueError("Invalid value for `xgb_replica_specs`, must not be `None`")  # noqa: E501
 
         self._xgb_replica_specs = xgb_replica_specs
 
     def to_dict(self):
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/v1_job_condition.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_job_condition.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from kubeflow.training.configuration import Configuration
 
 
-class V1JobCondition(object):
+class KubeflowOrgV1JobCondition(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -47,15 +47,15 @@
         'message': 'message',
         'reason': 'reason',
         'status': 'status',
         'type': 'type'
     }
 
     def __init__(self, last_transition_time=None, last_update_time=None, message=None, reason=None, status='', type='', local_vars_configuration=None):  # noqa: E501
-        """V1JobCondition - a model defined in OpenAPI"""  # noqa: E501
+        """KubeflowOrgV1JobCondition - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._last_transition_time = None
         self._last_update_time = None
         self._message = None
@@ -73,143 +73,143 @@
         if reason is not None:
             self.reason = reason
         self.status = status
         self.type = type
 
     @property
     def last_transition_time(self):
-        """Gets the last_transition_time of this V1JobCondition.  # noqa: E501
+        """Gets the last_transition_time of this KubeflowOrgV1JobCondition.  # noqa: E501
 
 
-        :return: The last_transition_time of this V1JobCondition.  # noqa: E501
+        :return: The last_transition_time of this KubeflowOrgV1JobCondition.  # noqa: E501
         :rtype: datetime
         """
         return self._last_transition_time
 
     @last_transition_time.setter
     def last_transition_time(self, last_transition_time):
-        """Sets the last_transition_time of this V1JobCondition.
+        """Sets the last_transition_time of this KubeflowOrgV1JobCondition.
 
 
-        :param last_transition_time: The last_transition_time of this V1JobCondition.  # noqa: E501
+        :param last_transition_time: The last_transition_time of this KubeflowOrgV1JobCondition.  # noqa: E501
         :type: datetime
         """
 
         self._last_transition_time = last_transition_time
 
     @property
     def last_update_time(self):
-        """Gets the last_update_time of this V1JobCondition.  # noqa: E501
+        """Gets the last_update_time of this KubeflowOrgV1JobCondition.  # noqa: E501
 
 
-        :return: The last_update_time of this V1JobCondition.  # noqa: E501
+        :return: The last_update_time of this KubeflowOrgV1JobCondition.  # noqa: E501
         :rtype: datetime
         """
         return self._last_update_time
 
     @last_update_time.setter
     def last_update_time(self, last_update_time):
-        """Sets the last_update_time of this V1JobCondition.
+        """Sets the last_update_time of this KubeflowOrgV1JobCondition.
 
 
-        :param last_update_time: The last_update_time of this V1JobCondition.  # noqa: E501
+        :param last_update_time: The last_update_time of this KubeflowOrgV1JobCondition.  # noqa: E501
         :type: datetime
         """
 
         self._last_update_time = last_update_time
 
     @property
     def message(self):
-        """Gets the message of this V1JobCondition.  # noqa: E501
+        """Gets the message of this KubeflowOrgV1JobCondition.  # noqa: E501
 
         A human readable message indicating details about the transition.  # noqa: E501
 
-        :return: The message of this V1JobCondition.  # noqa: E501
+        :return: The message of this KubeflowOrgV1JobCondition.  # noqa: E501
         :rtype: str
         """
         return self._message
 
     @message.setter
     def message(self, message):
-        """Sets the message of this V1JobCondition.
+        """Sets the message of this KubeflowOrgV1JobCondition.
 
         A human readable message indicating details about the transition.  # noqa: E501
 
-        :param message: The message of this V1JobCondition.  # noqa: E501
+        :param message: The message of this KubeflowOrgV1JobCondition.  # noqa: E501
         :type: str
         """
 
         self._message = message
 
     @property
     def reason(self):
-        """Gets the reason of this V1JobCondition.  # noqa: E501
+        """Gets the reason of this KubeflowOrgV1JobCondition.  # noqa: E501
 
         The reason for the condition's last transition.  # noqa: E501
 
-        :return: The reason of this V1JobCondition.  # noqa: E501
+        :return: The reason of this KubeflowOrgV1JobCondition.  # noqa: E501
         :rtype: str
         """
         return self._reason
 
     @reason.setter
     def reason(self, reason):
-        """Sets the reason of this V1JobCondition.
+        """Sets the reason of this KubeflowOrgV1JobCondition.
 
         The reason for the condition's last transition.  # noqa: E501
 
-        :param reason: The reason of this V1JobCondition.  # noqa: E501
+        :param reason: The reason of this KubeflowOrgV1JobCondition.  # noqa: E501
         :type: str
         """
 
         self._reason = reason
 
     @property
     def status(self):
-        """Gets the status of this V1JobCondition.  # noqa: E501
+        """Gets the status of this KubeflowOrgV1JobCondition.  # noqa: E501
 
         Status of the condition, one of True, False, Unknown.  # noqa: E501
 
-        :return: The status of this V1JobCondition.  # noqa: E501
+        :return: The status of this KubeflowOrgV1JobCondition.  # noqa: E501
         :rtype: str
         """
         return self._status
 
     @status.setter
     def status(self, status):
-        """Sets the status of this V1JobCondition.
+        """Sets the status of this KubeflowOrgV1JobCondition.
 
         Status of the condition, one of True, False, Unknown.  # noqa: E501
 
-        :param status: The status of this V1JobCondition.  # noqa: E501
+        :param status: The status of this KubeflowOrgV1JobCondition.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and status is None:  # noqa: E501
             raise ValueError("Invalid value for `status`, must not be `None`")  # noqa: E501
 
         self._status = status
 
     @property
     def type(self):
-        """Gets the type of this V1JobCondition.  # noqa: E501
+        """Gets the type of this KubeflowOrgV1JobCondition.  # noqa: E501
 
         Type of job condition.  # noqa: E501
 
-        :return: The type of this V1JobCondition.  # noqa: E501
+        :return: The type of this KubeflowOrgV1JobCondition.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
-        """Sets the type of this V1JobCondition.
+        """Sets the type of this KubeflowOrgV1JobCondition.
 
         Type of job condition.  # noqa: E501
 
-        :param type: The type of this V1JobCondition.  # noqa: E501
+        :param type: The type of this KubeflowOrgV1JobCondition.  # noqa: E501
         :type: str
         """
         if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
             raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
 
         self._type = type
 
@@ -243,18 +243,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1JobCondition):
+        if not isinstance(other, KubeflowOrgV1JobCondition):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V1JobCondition):
+        if not isinstance(other, KubeflowOrgV1JobCondition):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/v1_job_status.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_job_status.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from kubeflow.training.configuration import Configuration
 
 
-class V1JobStatus(object):
+class KubeflowOrgV1JobStatus(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -30,158 +30,156 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'completion_time': 'datetime',
-        'conditions': 'list[V1JobCondition]',
+        'conditions': 'list[KubeflowOrgV1JobCondition]',
         'last_reconcile_time': 'datetime',
-        'replica_statuses': 'dict(str, V1ReplicaStatus)',
+        'replica_statuses': 'dict(str, KubeflowOrgV1ReplicaStatus)',
         'start_time': 'datetime'
     }
 
     attribute_map = {
         'completion_time': 'completionTime',
         'conditions': 'conditions',
         'last_reconcile_time': 'lastReconcileTime',
         'replica_statuses': 'replicaStatuses',
         'start_time': 'startTime'
     }
 
     def __init__(self, completion_time=None, conditions=None, last_reconcile_time=None, replica_statuses=None, start_time=None, local_vars_configuration=None):  # noqa: E501
-        """V1JobStatus - a model defined in OpenAPI"""  # noqa: E501
+        """KubeflowOrgV1JobStatus - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._completion_time = None
         self._conditions = None
         self._last_reconcile_time = None
         self._replica_statuses = None
         self._start_time = None
         self.discriminator = None
 
         if completion_time is not None:
             self.completion_time = completion_time
-        self.conditions = conditions
+        if conditions is not None:
+            self.conditions = conditions
         if last_reconcile_time is not None:
             self.last_reconcile_time = last_reconcile_time
-        self.replica_statuses = replica_statuses
+        if replica_statuses is not None:
+            self.replica_statuses = replica_statuses
         if start_time is not None:
             self.start_time = start_time
 
     @property
     def completion_time(self):
-        """Gets the completion_time of this V1JobStatus.  # noqa: E501
+        """Gets the completion_time of this KubeflowOrgV1JobStatus.  # noqa: E501
 
 
-        :return: The completion_time of this V1JobStatus.  # noqa: E501
+        :return: The completion_time of this KubeflowOrgV1JobStatus.  # noqa: E501
         :rtype: datetime
         """
         return self._completion_time
 
     @completion_time.setter
     def completion_time(self, completion_time):
-        """Sets the completion_time of this V1JobStatus.
+        """Sets the completion_time of this KubeflowOrgV1JobStatus.
 
 
-        :param completion_time: The completion_time of this V1JobStatus.  # noqa: E501
+        :param completion_time: The completion_time of this KubeflowOrgV1JobStatus.  # noqa: E501
         :type: datetime
         """
 
         self._completion_time = completion_time
 
     @property
     def conditions(self):
-        """Gets the conditions of this V1JobStatus.  # noqa: E501
+        """Gets the conditions of this KubeflowOrgV1JobStatus.  # noqa: E501
 
         Conditions is an array of current observed job conditions.  # noqa: E501
 
-        :return: The conditions of this V1JobStatus.  # noqa: E501
-        :rtype: list[V1JobCondition]
+        :return: The conditions of this KubeflowOrgV1JobStatus.  # noqa: E501
+        :rtype: list[KubeflowOrgV1JobCondition]
         """
         return self._conditions
 
     @conditions.setter
     def conditions(self, conditions):
-        """Sets the conditions of this V1JobStatus.
+        """Sets the conditions of this KubeflowOrgV1JobStatus.
 
         Conditions is an array of current observed job conditions.  # noqa: E501
 
-        :param conditions: The conditions of this V1JobStatus.  # noqa: E501
-        :type: list[V1JobCondition]
+        :param conditions: The conditions of this KubeflowOrgV1JobStatus.  # noqa: E501
+        :type: list[KubeflowOrgV1JobCondition]
         """
-        if self.local_vars_configuration.client_side_validation and conditions is None:  # noqa: E501
-            raise ValueError("Invalid value for `conditions`, must not be `None`")  # noqa: E501
 
         self._conditions = conditions
 
     @property
     def last_reconcile_time(self):
-        """Gets the last_reconcile_time of this V1JobStatus.  # noqa: E501
+        """Gets the last_reconcile_time of this KubeflowOrgV1JobStatus.  # noqa: E501
 
 
-        :return: The last_reconcile_time of this V1JobStatus.  # noqa: E501
+        :return: The last_reconcile_time of this KubeflowOrgV1JobStatus.  # noqa: E501
         :rtype: datetime
         """
         return self._last_reconcile_time
 
     @last_reconcile_time.setter
     def last_reconcile_time(self, last_reconcile_time):
-        """Sets the last_reconcile_time of this V1JobStatus.
+        """Sets the last_reconcile_time of this KubeflowOrgV1JobStatus.
 
 
-        :param last_reconcile_time: The last_reconcile_time of this V1JobStatus.  # noqa: E501
+        :param last_reconcile_time: The last_reconcile_time of this KubeflowOrgV1JobStatus.  # noqa: E501
         :type: datetime
         """
 
         self._last_reconcile_time = last_reconcile_time
 
     @property
     def replica_statuses(self):
-        """Gets the replica_statuses of this V1JobStatus.  # noqa: E501
+        """Gets the replica_statuses of this KubeflowOrgV1JobStatus.  # noqa: E501
 
         ReplicaStatuses is map of ReplicaType and ReplicaStatus, specifies the status of each replica.  # noqa: E501
 
-        :return: The replica_statuses of this V1JobStatus.  # noqa: E501
-        :rtype: dict(str, V1ReplicaStatus)
+        :return: The replica_statuses of this KubeflowOrgV1JobStatus.  # noqa: E501
+        :rtype: dict(str, KubeflowOrgV1ReplicaStatus)
         """
         return self._replica_statuses
 
     @replica_statuses.setter
     def replica_statuses(self, replica_statuses):
-        """Sets the replica_statuses of this V1JobStatus.
+        """Sets the replica_statuses of this KubeflowOrgV1JobStatus.
 
         ReplicaStatuses is map of ReplicaType and ReplicaStatus, specifies the status of each replica.  # noqa: E501
 
-        :param replica_statuses: The replica_statuses of this V1JobStatus.  # noqa: E501
-        :type: dict(str, V1ReplicaStatus)
+        :param replica_statuses: The replica_statuses of this KubeflowOrgV1JobStatus.  # noqa: E501
+        :type: dict(str, KubeflowOrgV1ReplicaStatus)
         """
-        if self.local_vars_configuration.client_side_validation and replica_statuses is None:  # noqa: E501
-            raise ValueError("Invalid value for `replica_statuses`, must not be `None`")  # noqa: E501
 
         self._replica_statuses = replica_statuses
 
     @property
     def start_time(self):
-        """Gets the start_time of this V1JobStatus.  # noqa: E501
+        """Gets the start_time of this KubeflowOrgV1JobStatus.  # noqa: E501
 
 
-        :return: The start_time of this V1JobStatus.  # noqa: E501
+        :return: The start_time of this KubeflowOrgV1JobStatus.  # noqa: E501
         :rtype: datetime
         """
         return self._start_time
 
     @start_time.setter
     def start_time(self, start_time):
-        """Sets the start_time of this V1JobStatus.
+        """Sets the start_time of this KubeflowOrgV1JobStatus.
 
 
-        :param start_time: The start_time of this V1JobStatus.  # noqa: E501
+        :param start_time: The start_time of this KubeflowOrgV1JobStatus.  # noqa: E501
         :type: datetime
         """
 
         self._start_time = start_time
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -213,18 +211,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1JobStatus):
+        if not isinstance(other, KubeflowOrgV1JobStatus):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V1JobStatus):
+        if not isinstance(other, KubeflowOrgV1JobStatus):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/v1_replica_spec.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_replica_spec.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from kubeflow.training.configuration import Configuration
 
 
-class V1ReplicaSpec(object):
+class KubeflowOrgV1ReplicaSpec(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -41,15 +41,15 @@
     attribute_map = {
         'replicas': 'replicas',
         'restart_policy': 'restartPolicy',
         'template': 'template'
     }
 
     def __init__(self, replicas=None, restart_policy=None, template=None, local_vars_configuration=None):  # noqa: E501
-        """V1ReplicaSpec - a model defined in OpenAPI"""  # noqa: E501
+        """KubeflowOrgV1ReplicaSpec - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._replicas = None
         self._restart_policy = None
         self._template = None
@@ -60,74 +60,74 @@
         if restart_policy is not None:
             self.restart_policy = restart_policy
         if template is not None:
             self.template = template
 
     @property
     def replicas(self):
-        """Gets the replicas of this V1ReplicaSpec.  # noqa: E501
+        """Gets the replicas of this KubeflowOrgV1ReplicaSpec.  # noqa: E501
 
         Replicas is the desired number of replicas of the given template. If unspecified, defaults to 1.  # noqa: E501
 
-        :return: The replicas of this V1ReplicaSpec.  # noqa: E501
+        :return: The replicas of this KubeflowOrgV1ReplicaSpec.  # noqa: E501
         :rtype: int
         """
         return self._replicas
 
     @replicas.setter
     def replicas(self, replicas):
-        """Sets the replicas of this V1ReplicaSpec.
+        """Sets the replicas of this KubeflowOrgV1ReplicaSpec.
 
         Replicas is the desired number of replicas of the given template. If unspecified, defaults to 1.  # noqa: E501
 
-        :param replicas: The replicas of this V1ReplicaSpec.  # noqa: E501
+        :param replicas: The replicas of this KubeflowOrgV1ReplicaSpec.  # noqa: E501
         :type: int
         """
 
         self._replicas = replicas
 
     @property
     def restart_policy(self):
-        """Gets the restart_policy of this V1ReplicaSpec.  # noqa: E501
+        """Gets the restart_policy of this KubeflowOrgV1ReplicaSpec.  # noqa: E501
 
         Restart policy for all replicas within the job. One of Always, OnFailure, Never and ExitCode. Default to Never.  # noqa: E501
 
-        :return: The restart_policy of this V1ReplicaSpec.  # noqa: E501
+        :return: The restart_policy of this KubeflowOrgV1ReplicaSpec.  # noqa: E501
         :rtype: str
         """
         return self._restart_policy
 
     @restart_policy.setter
     def restart_policy(self, restart_policy):
-        """Sets the restart_policy of this V1ReplicaSpec.
+        """Sets the restart_policy of this KubeflowOrgV1ReplicaSpec.
 
         Restart policy for all replicas within the job. One of Always, OnFailure, Never and ExitCode. Default to Never.  # noqa: E501
 
-        :param restart_policy: The restart_policy of this V1ReplicaSpec.  # noqa: E501
+        :param restart_policy: The restart_policy of this KubeflowOrgV1ReplicaSpec.  # noqa: E501
         :type: str
         """
 
         self._restart_policy = restart_policy
 
     @property
     def template(self):
-        """Gets the template of this V1ReplicaSpec.  # noqa: E501
+        """Gets the template of this KubeflowOrgV1ReplicaSpec.  # noqa: E501
 
 
-        :return: The template of this V1ReplicaSpec.  # noqa: E501
+        :return: The template of this KubeflowOrgV1ReplicaSpec.  # noqa: E501
         :rtype: V1PodTemplateSpec
         """
         return self._template
 
     @template.setter
     def template(self, template):
-        """Sets the template of this V1ReplicaSpec.
+        """Sets the template of this KubeflowOrgV1ReplicaSpec.
 
 
-        :param template: The template of this V1ReplicaSpec.  # noqa: E501
+        :param template: The template of this KubeflowOrgV1ReplicaSpec.  # noqa: E501
         :type: V1PodTemplateSpec
         """
 
         self._template = template
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -159,18 +159,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1ReplicaSpec):
+        if not isinstance(other, KubeflowOrgV1ReplicaSpec):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V1ReplicaSpec):
+        if not isinstance(other, KubeflowOrgV1ReplicaSpec):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/v1_replica_status.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_replica_status.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from kubeflow.training.configuration import Configuration
 
 
-class V1ReplicaStatus(object):
+class KubeflowOrgV1ReplicaStatus(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -45,15 +45,15 @@
         'failed': 'failed',
         'label_selector': 'labelSelector',
         'selector': 'selector',
         'succeeded': 'succeeded'
     }
 
     def __init__(self, active=None, failed=None, label_selector=None, selector=None, succeeded=None, local_vars_configuration=None):  # noqa: E501
-        """V1ReplicaStatus - a model defined in OpenAPI"""  # noqa: E501
+        """KubeflowOrgV1ReplicaStatus - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._active = None
         self._failed = None
         self._label_selector = None
@@ -70,120 +70,120 @@
         if selector is not None:
             self.selector = selector
         if succeeded is not None:
             self.succeeded = succeeded
 
     @property
     def active(self):
-        """Gets the active of this V1ReplicaStatus.  # noqa: E501
+        """Gets the active of this KubeflowOrgV1ReplicaStatus.  # noqa: E501
 
         The number of actively running pods.  # noqa: E501
 
-        :return: The active of this V1ReplicaStatus.  # noqa: E501
+        :return: The active of this KubeflowOrgV1ReplicaStatus.  # noqa: E501
         :rtype: int
         """
         return self._active
 
     @active.setter
     def active(self, active):
-        """Sets the active of this V1ReplicaStatus.
+        """Sets the active of this KubeflowOrgV1ReplicaStatus.
 
         The number of actively running pods.  # noqa: E501
 
-        :param active: The active of this V1ReplicaStatus.  # noqa: E501
+        :param active: The active of this KubeflowOrgV1ReplicaStatus.  # noqa: E501
         :type: int
         """
 
         self._active = active
 
     @property
     def failed(self):
-        """Gets the failed of this V1ReplicaStatus.  # noqa: E501
+        """Gets the failed of this KubeflowOrgV1ReplicaStatus.  # noqa: E501
 
         The number of pods which reached phase Failed.  # noqa: E501
 
-        :return: The failed of this V1ReplicaStatus.  # noqa: E501
+        :return: The failed of this KubeflowOrgV1ReplicaStatus.  # noqa: E501
         :rtype: int
         """
         return self._failed
 
     @failed.setter
     def failed(self, failed):
-        """Sets the failed of this V1ReplicaStatus.
+        """Sets the failed of this KubeflowOrgV1ReplicaStatus.
 
         The number of pods which reached phase Failed.  # noqa: E501
 
-        :param failed: The failed of this V1ReplicaStatus.  # noqa: E501
+        :param failed: The failed of this KubeflowOrgV1ReplicaStatus.  # noqa: E501
         :type: int
         """
 
         self._failed = failed
 
     @property
     def label_selector(self):
-        """Gets the label_selector of this V1ReplicaStatus.  # noqa: E501
+        """Gets the label_selector of this KubeflowOrgV1ReplicaStatus.  # noqa: E501
 
 
-        :return: The label_selector of this V1ReplicaStatus.  # noqa: E501
+        :return: The label_selector of this KubeflowOrgV1ReplicaStatus.  # noqa: E501
         :rtype: V1LabelSelector
         """
         return self._label_selector
 
     @label_selector.setter
     def label_selector(self, label_selector):
-        """Sets the label_selector of this V1ReplicaStatus.
+        """Sets the label_selector of this KubeflowOrgV1ReplicaStatus.
 
 
-        :param label_selector: The label_selector of this V1ReplicaStatus.  # noqa: E501
+        :param label_selector: The label_selector of this KubeflowOrgV1ReplicaStatus.  # noqa: E501
         :type: V1LabelSelector
         """
 
         self._label_selector = label_selector
 
     @property
     def selector(self):
-        """Gets the selector of this V1ReplicaStatus.  # noqa: E501
+        """Gets the selector of this KubeflowOrgV1ReplicaStatus.  # noqa: E501
 
         A Selector is a label query over a set of resources. The result of matchLabels and matchExpressions are ANDed. An empty Selector matches all objects. A null Selector matches no objects.  # noqa: E501
 
-        :return: The selector of this V1ReplicaStatus.  # noqa: E501
+        :return: The selector of this KubeflowOrgV1ReplicaStatus.  # noqa: E501
         :rtype: str
         """
         return self._selector
 
     @selector.setter
     def selector(self, selector):
-        """Sets the selector of this V1ReplicaStatus.
+        """Sets the selector of this KubeflowOrgV1ReplicaStatus.
 
         A Selector is a label query over a set of resources. The result of matchLabels and matchExpressions are ANDed. An empty Selector matches all objects. A null Selector matches no objects.  # noqa: E501
 
-        :param selector: The selector of this V1ReplicaStatus.  # noqa: E501
+        :param selector: The selector of this KubeflowOrgV1ReplicaStatus.  # noqa: E501
         :type: str
         """
 
         self._selector = selector
 
     @property
     def succeeded(self):
-        """Gets the succeeded of this V1ReplicaStatus.  # noqa: E501
+        """Gets the succeeded of this KubeflowOrgV1ReplicaStatus.  # noqa: E501
 
         The number of pods which reached phase Succeeded.  # noqa: E501
 
-        :return: The succeeded of this V1ReplicaStatus.  # noqa: E501
+        :return: The succeeded of this KubeflowOrgV1ReplicaStatus.  # noqa: E501
         :rtype: int
         """
         return self._succeeded
 
     @succeeded.setter
     def succeeded(self, succeeded):
-        """Sets the succeeded of this V1ReplicaStatus.
+        """Sets the succeeded of this KubeflowOrgV1ReplicaStatus.
 
         The number of pods which reached phase Succeeded.  # noqa: E501
 
-        :param succeeded: The succeeded of this V1ReplicaStatus.  # noqa: E501
+        :param succeeded: The succeeded of this KubeflowOrgV1ReplicaStatus.  # noqa: E501
         :type: int
         """
 
         self._succeeded = succeeded
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -215,18 +215,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1ReplicaStatus):
+        if not isinstance(other, KubeflowOrgV1ReplicaStatus):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V1ReplicaStatus):
+        if not isinstance(other, KubeflowOrgV1ReplicaStatus):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/models/v1_run_policy.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/models/kubeflow_org_v1_scheduling_policy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,193 +1,185 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from kubeflow.training.configuration import Configuration
 
 
-class V1RunPolicy(object):
+class KubeflowOrgV1SchedulingPolicy(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'active_deadline_seconds': 'int',
-        'backoff_limit': 'int',
-        'clean_pod_policy': 'str',
-        'scheduling_policy': 'V1SchedulingPolicy',
-        'ttl_seconds_after_finished': 'int'
+        'min_available': 'int',
+        'min_resources': 'dict(str, Quantity)',
+        'priority_class': 'str',
+        'queue': 'str',
+        'schedule_timeout_seconds': 'int'
     }
 
     attribute_map = {
-        'active_deadline_seconds': 'activeDeadlineSeconds',
-        'backoff_limit': 'backoffLimit',
-        'clean_pod_policy': 'cleanPodPolicy',
-        'scheduling_policy': 'schedulingPolicy',
-        'ttl_seconds_after_finished': 'ttlSecondsAfterFinished'
+        'min_available': 'minAvailable',
+        'min_resources': 'minResources',
+        'priority_class': 'priorityClass',
+        'queue': 'queue',
+        'schedule_timeout_seconds': 'scheduleTimeoutSeconds'
     }
 
-    def __init__(self, active_deadline_seconds=None, backoff_limit=None, clean_pod_policy=None, scheduling_policy=None, ttl_seconds_after_finished=None, local_vars_configuration=None):  # noqa: E501
-        """V1RunPolicy - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, min_available=None, min_resources=None, priority_class=None, queue=None, schedule_timeout_seconds=None, local_vars_configuration=None):  # noqa: E501
+        """KubeflowOrgV1SchedulingPolicy - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._active_deadline_seconds = None
-        self._backoff_limit = None
-        self._clean_pod_policy = None
-        self._scheduling_policy = None
-        self._ttl_seconds_after_finished = None
+        self._min_available = None
+        self._min_resources = None
+        self._priority_class = None
+        self._queue = None
+        self._schedule_timeout_seconds = None
         self.discriminator = None
 
-        if active_deadline_seconds is not None:
-            self.active_deadline_seconds = active_deadline_seconds
-        if backoff_limit is not None:
-            self.backoff_limit = backoff_limit
-        if clean_pod_policy is not None:
-            self.clean_pod_policy = clean_pod_policy
-        if scheduling_policy is not None:
-            self.scheduling_policy = scheduling_policy
-        if ttl_seconds_after_finished is not None:
-            self.ttl_seconds_after_finished = ttl_seconds_after_finished
+        if min_available is not None:
+            self.min_available = min_available
+        if min_resources is not None:
+            self.min_resources = min_resources
+        if priority_class is not None:
+            self.priority_class = priority_class
+        if queue is not None:
+            self.queue = queue
+        if schedule_timeout_seconds is not None:
+            self.schedule_timeout_seconds = schedule_timeout_seconds
 
     @property
-    def active_deadline_seconds(self):
-        """Gets the active_deadline_seconds of this V1RunPolicy.  # noqa: E501
+    def min_available(self):
+        """Gets the min_available of this KubeflowOrgV1SchedulingPolicy.  # noqa: E501
 
-        Specifies the duration in seconds relative to the startTime that the job may be active before the system tries to terminate it; value must be positive integer.  # noqa: E501
 
-        :return: The active_deadline_seconds of this V1RunPolicy.  # noqa: E501
+        :return: The min_available of this KubeflowOrgV1SchedulingPolicy.  # noqa: E501
         :rtype: int
         """
-        return self._active_deadline_seconds
+        return self._min_available
 
-    @active_deadline_seconds.setter
-    def active_deadline_seconds(self, active_deadline_seconds):
-        """Sets the active_deadline_seconds of this V1RunPolicy.
+    @min_available.setter
+    def min_available(self, min_available):
+        """Sets the min_available of this KubeflowOrgV1SchedulingPolicy.
 
-        Specifies the duration in seconds relative to the startTime that the job may be active before the system tries to terminate it; value must be positive integer.  # noqa: E501
 
-        :param active_deadline_seconds: The active_deadline_seconds of this V1RunPolicy.  # noqa: E501
+        :param min_available: The min_available of this KubeflowOrgV1SchedulingPolicy.  # noqa: E501
         :type: int
         """
 
-        self._active_deadline_seconds = active_deadline_seconds
+        self._min_available = min_available
 
     @property
-    def backoff_limit(self):
-        """Gets the backoff_limit of this V1RunPolicy.  # noqa: E501
+    def min_resources(self):
+        """Gets the min_resources of this KubeflowOrgV1SchedulingPolicy.  # noqa: E501
 
-        Optional number of retries before marking this job failed.  # noqa: E501
 
-        :return: The backoff_limit of this V1RunPolicy.  # noqa: E501
-        :rtype: int
+        :return: The min_resources of this KubeflowOrgV1SchedulingPolicy.  # noqa: E501
+        :rtype: dict(str, Quantity)
         """
-        return self._backoff_limit
+        return self._min_resources
 
-    @backoff_limit.setter
-    def backoff_limit(self, backoff_limit):
-        """Sets the backoff_limit of this V1RunPolicy.
+    @min_resources.setter
+    def min_resources(self, min_resources):
+        """Sets the min_resources of this KubeflowOrgV1SchedulingPolicy.
 
-        Optional number of retries before marking this job failed.  # noqa: E501
 
-        :param backoff_limit: The backoff_limit of this V1RunPolicy.  # noqa: E501
-        :type: int
+        :param min_resources: The min_resources of this KubeflowOrgV1SchedulingPolicy.  # noqa: E501
+        :type: dict(str, Quantity)
         """
 
-        self._backoff_limit = backoff_limit
+        self._min_resources = min_resources
 
     @property
-    def clean_pod_policy(self):
-        """Gets the clean_pod_policy of this V1RunPolicy.  # noqa: E501
+    def priority_class(self):
+        """Gets the priority_class of this KubeflowOrgV1SchedulingPolicy.  # noqa: E501
 
-        CleanPodPolicy defines the policy to kill pods after the job completes. Default to Running.  # noqa: E501
 
-        :return: The clean_pod_policy of this V1RunPolicy.  # noqa: E501
+        :return: The priority_class of this KubeflowOrgV1SchedulingPolicy.  # noqa: E501
         :rtype: str
         """
-        return self._clean_pod_policy
+        return self._priority_class
 
-    @clean_pod_policy.setter
-    def clean_pod_policy(self, clean_pod_policy):
-        """Sets the clean_pod_policy of this V1RunPolicy.
+    @priority_class.setter
+    def priority_class(self, priority_class):
+        """Sets the priority_class of this KubeflowOrgV1SchedulingPolicy.
 
-        CleanPodPolicy defines the policy to kill pods after the job completes. Default to Running.  # noqa: E501
 
-        :param clean_pod_policy: The clean_pod_policy of this V1RunPolicy.  # noqa: E501
+        :param priority_class: The priority_class of this KubeflowOrgV1SchedulingPolicy.  # noqa: E501
         :type: str
         """
 
-        self._clean_pod_policy = clean_pod_policy
+        self._priority_class = priority_class
 
     @property
-    def scheduling_policy(self):
-        """Gets the scheduling_policy of this V1RunPolicy.  # noqa: E501
+    def queue(self):
+        """Gets the queue of this KubeflowOrgV1SchedulingPolicy.  # noqa: E501
 
 
-        :return: The scheduling_policy of this V1RunPolicy.  # noqa: E501
-        :rtype: V1SchedulingPolicy
+        :return: The queue of this KubeflowOrgV1SchedulingPolicy.  # noqa: E501
+        :rtype: str
         """
-        return self._scheduling_policy
+        return self._queue
 
-    @scheduling_policy.setter
-    def scheduling_policy(self, scheduling_policy):
-        """Sets the scheduling_policy of this V1RunPolicy.
+    @queue.setter
+    def queue(self, queue):
+        """Sets the queue of this KubeflowOrgV1SchedulingPolicy.
 
 
-        :param scheduling_policy: The scheduling_policy of this V1RunPolicy.  # noqa: E501
-        :type: V1SchedulingPolicy
+        :param queue: The queue of this KubeflowOrgV1SchedulingPolicy.  # noqa: E501
+        :type: str
         """
 
-        self._scheduling_policy = scheduling_policy
+        self._queue = queue
 
     @property
-    def ttl_seconds_after_finished(self):
-        """Gets the ttl_seconds_after_finished of this V1RunPolicy.  # noqa: E501
+    def schedule_timeout_seconds(self):
+        """Gets the schedule_timeout_seconds of this KubeflowOrgV1SchedulingPolicy.  # noqa: E501
 
-        TTLSecondsAfterFinished is the TTL to clean up jobs. It may take extra ReconcilePeriod seconds for the cleanup, since reconcile gets called periodically. Default to infinite.  # noqa: E501
 
-        :return: The ttl_seconds_after_finished of this V1RunPolicy.  # noqa: E501
+        :return: The schedule_timeout_seconds of this KubeflowOrgV1SchedulingPolicy.  # noqa: E501
         :rtype: int
         """
-        return self._ttl_seconds_after_finished
+        return self._schedule_timeout_seconds
 
-    @ttl_seconds_after_finished.setter
-    def ttl_seconds_after_finished(self, ttl_seconds_after_finished):
-        """Sets the ttl_seconds_after_finished of this V1RunPolicy.
+    @schedule_timeout_seconds.setter
+    def schedule_timeout_seconds(self, schedule_timeout_seconds):
+        """Sets the schedule_timeout_seconds of this KubeflowOrgV1SchedulingPolicy.
 
-        TTLSecondsAfterFinished is the TTL to clean up jobs. It may take extra ReconcilePeriod seconds for the cleanup, since reconcile gets called periodically. Default to infinite.  # noqa: E501
 
-        :param ttl_seconds_after_finished: The ttl_seconds_after_finished of this V1RunPolicy.  # noqa: E501
+        :param schedule_timeout_seconds: The schedule_timeout_seconds of this KubeflowOrgV1SchedulingPolicy.  # noqa: E501
         :type: int
         """
 
-        self._ttl_seconds_after_finished = ttl_seconds_after_finished
+        self._schedule_timeout_seconds = schedule_timeout_seconds
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -215,18 +207,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1RunPolicy):
+        if not isinstance(other, KubeflowOrgV1SchedulingPolicy):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, V1RunPolicy):
+        if not isinstance(other, KubeflowOrgV1SchedulingPolicy):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/rest.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import io
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/utils/__init__.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kubeflow-training-1.6.0rc0/kubeflow/training/utils/utils.py` & `kubeflow-training-1.7.0rc0/kubeflow/training/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,15 +318,15 @@
         exec_script = (
             get_script_for_python_packages(packages_to_install, pip_index_url)
             + exec_script
         )
 
     # Create Pod template spec.
     pod_template_spec = client.V1PodTemplateSpec(
-        metadata=client.V1ObjectMeta(annotations={"sidecar.istio.io/inject": "false"}),
+        metadata=client.V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
         spec=client.V1PodSpec(
             containers=[
                 client.V1Container(
                     name=container_name,
                     image=base_image,
                     command=["bash", "-c"],
                     args=[exec_script],
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow_training.egg-info/PKG-INFO` & `kubeflow-training-1.7.0rc0/kubeflow_training.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: kubeflow-training
-Version: 1.6.0rc0
+Version: 1.7.0rc0
 Summary: Training Operator Python SDK
 Home-page: https://github.com/kubeflow/training-operator/sdk/python
 Author: Kubeflow Authors
 Author-email: hejinchi@cn.ibm.com
 License: Apache License Version 2.0
-Description: Training Operator Python SDK
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
@@ -21,7 +20,10 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: test
+
+Training Operator Python SDK
+
```

### Comparing `kubeflow-training-1.6.0rc0/kubeflow_training.egg-info/SOURCES.txt` & `kubeflow-training-1.7.0rc0/kubeflow_training.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,76 +8,77 @@
 kubeflow/training/rest.py
 kubeflow/training/api/__init__.py
 kubeflow/training/api/training_client.py
 kubeflow/training/constants/__init__.py
 kubeflow/training/constants/constants.py
 kubeflow/training/models/__init__.py
 kubeflow/training/models/kubeflow_org_v1_elastic_policy.py
+kubeflow/training/models/kubeflow_org_v1_job_condition.py
+kubeflow/training/models/kubeflow_org_v1_job_status.py
 kubeflow/training/models/kubeflow_org_v1_mpi_job.py
 kubeflow/training/models/kubeflow_org_v1_mpi_job_list.py
 kubeflow/training/models/kubeflow_org_v1_mpi_job_spec.py
 kubeflow/training/models/kubeflow_org_v1_mx_job.py
 kubeflow/training/models/kubeflow_org_v1_mx_job_list.py
 kubeflow/training/models/kubeflow_org_v1_mx_job_spec.py
 kubeflow/training/models/kubeflow_org_v1_paddle_elastic_policy.py
 kubeflow/training/models/kubeflow_org_v1_paddle_job.py
 kubeflow/training/models/kubeflow_org_v1_paddle_job_list.py
 kubeflow/training/models/kubeflow_org_v1_paddle_job_spec.py
 kubeflow/training/models/kubeflow_org_v1_py_torch_job.py
 kubeflow/training/models/kubeflow_org_v1_py_torch_job_list.py
 kubeflow/training/models/kubeflow_org_v1_py_torch_job_spec.py
 kubeflow/training/models/kubeflow_org_v1_rdzv_conf.py
+kubeflow/training/models/kubeflow_org_v1_replica_spec.py
+kubeflow/training/models/kubeflow_org_v1_replica_status.py
+kubeflow/training/models/kubeflow_org_v1_run_policy.py
+kubeflow/training/models/kubeflow_org_v1_scheduling_policy.py
 kubeflow/training/models/kubeflow_org_v1_tf_job.py
 kubeflow/training/models/kubeflow_org_v1_tf_job_list.py
 kubeflow/training/models/kubeflow_org_v1_tf_job_spec.py
 kubeflow/training/models/kubeflow_org_v1_xg_boost_job.py
 kubeflow/training/models/kubeflow_org_v1_xg_boost_job_list.py
 kubeflow/training/models/kubeflow_org_v1_xg_boost_job_spec.py
-kubeflow/training/models/v1_job_condition.py
-kubeflow/training/models/v1_job_status.py
-kubeflow/training/models/v1_replica_spec.py
-kubeflow/training/models/v1_replica_status.py
-kubeflow/training/models/v1_run_policy.py
-kubeflow/training/models/v1_scheduling_policy.py
 kubeflow/training/utils/__init__.py
 kubeflow/training/utils/utils.py
 kubeflow_training.egg-info/PKG-INFO
 kubeflow_training.egg-info/SOURCES.txt
 kubeflow_training.egg-info/dependency_links.txt
 kubeflow_training.egg-info/not-zip-safe
 kubeflow_training.egg-info/requires.txt
 kubeflow_training.egg-info/top_level.txt
 test/__init__.py
+test/conftest.py
 test/test_kubeflow_org_v1_elastic_policy.py
+test/test_kubeflow_org_v1_job_condition.py
+test/test_kubeflow_org_v1_job_status.py
 test/test_kubeflow_org_v1_mpi_job.py
 test/test_kubeflow_org_v1_mpi_job_list.py
 test/test_kubeflow_org_v1_mpi_job_spec.py
 test/test_kubeflow_org_v1_mx_job.py
 test/test_kubeflow_org_v1_mx_job_list.py
 test/test_kubeflow_org_v1_mx_job_spec.py
 test/test_kubeflow_org_v1_paddle_elastic_policy.py
 test/test_kubeflow_org_v1_paddle_job.py
 test/test_kubeflow_org_v1_paddle_job_list.py
 test/test_kubeflow_org_v1_paddle_job_spec.py
 test/test_kubeflow_org_v1_py_torch_job.py
 test/test_kubeflow_org_v1_py_torch_job_list.py
 test/test_kubeflow_org_v1_py_torch_job_spec.py
 test/test_kubeflow_org_v1_rdzv_conf.py
+test/test_kubeflow_org_v1_replica_spec.py
+test/test_kubeflow_org_v1_replica_status.py
+test/test_kubeflow_org_v1_run_policy.py
+test/test_kubeflow_org_v1_scheduling_policy.py
 test/test_kubeflow_org_v1_tf_job.py
 test/test_kubeflow_org_v1_tf_job_list.py
 test/test_kubeflow_org_v1_tf_job_spec.py
 test/test_kubeflow_org_v1_xg_boost_job.py
 test/test_kubeflow_org_v1_xg_boost_job_list.py
 test/test_kubeflow_org_v1_xg_boost_job_spec.py
-test/test_v1_job_condition.py
-test/test_v1_job_status.py
-test/test_v1_replica_spec.py
-test/test_v1_replica_status.py
-test/test_v1_run_policy.py
-test/test_v1_scheduling_policy.py
 test/e2e/__init__.py
 test/e2e/constants.py
 test/e2e/test_e2e_mpijob.py
 test/e2e/test_e2e_mxjob.py
 test/e2e/test_e2e_paddlejob.py
 test/e2e/test_e2e_pytorchjob.py
 test/e2e/test_e2e_tfjob.py
```

### Comparing `kubeflow-training-1.6.0rc0/setup.py` & `kubeflow-training-1.7.0rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "urllib3>=1.15.1",
     "kubernetes>=23.6.0",
     "retrying>=1.3.3",
 ]
 
 setuptools.setup(
     name="kubeflow-training",
-    version="1.6.0rc0",
+    version="1.7.0rc0",
     author="Kubeflow Authors",
     author_email="hejinchi@cn.ibm.com",
     license="Apache License Version 2.0",
     url="https://github.com/kubeflow/training-operator/sdk/python",
     description="Training Operator Python SDK",
     long_description="Training Operator Python SDK",
     packages=setuptools.find_packages(include=("kubeflow*")),
```

### Comparing `kubeflow-training-1.6.0rc0/test/e2e/constants.py` & `kubeflow-training-1.7.0rc0/test/e2e/constants.py`

 * *Files identical despite different names*

### Comparing `kubeflow-training-1.6.0rc0/test/e2e/test_e2e_mpijob.py` & `kubeflow-training-1.7.0rc0/test/e2e/test_e2e_pytorchjob.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,181 +11,160 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import logging
 import pytest
-from typing import Tuple
 
 from kubernetes.client import V1PodTemplateSpec
 from kubernetes.client import V1ObjectMeta
 from kubernetes.client import V1PodSpec
 from kubernetes.client import V1Container
+from kubernetes.client import V1ResourceRequirements
 
 from kubeflow.training import TrainingClient
-from kubeflow.training import V1ReplicaSpec
-from kubeflow.training import KubeflowOrgV1MPIJob
-from kubeflow.training import KubeflowOrgV1MPIJobSpec
-from kubeflow.training import V1RunPolicy
-from kubeflow.training import V1SchedulingPolicy
+from kubeflow.training import KubeflowOrgV1ReplicaSpec
+from kubeflow.training import KubeflowOrgV1PyTorchJob
+from kubeflow.training import KubeflowOrgV1PyTorchJobSpec
+from kubeflow.training import KubeflowOrgV1RunPolicy
+from kubeflow.training import KubeflowOrgV1SchedulingPolicy
 from kubeflow.training.constants import constants
 
 from test.e2e.utils import verify_job_e2e, verify_unschedulable_job_e2e, get_pod_spec_scheduler_name
 from test.e2e.constants import TEST_GANG_SCHEDULER_NAME_ENV_KEY
 from test.e2e.constants import GANG_SCHEDULERS, NONE_GANG_SCHEDULERS
 
 logging.basicConfig(format="%(message)s")
 logging.getLogger().setLevel(logging.INFO)
 
-TRAINING_CLIENT = TrainingClient(config_file=os.getenv("KUBECONFIG", "~/.kube/config"))
-JOB_NAME = "mpijob-mxnet-ci-test"
-JOB_NAMESPACE = "default"
-CONTAINER_NAME = "mpi"
+TRAINING_CLIENT = TrainingClient()
+JOB_NAME = "pytorchjob-mnist-ci-test"
+CONTAINER_NAME = "pytorch"
 GANG_SCHEDULER_NAME = os.getenv(TEST_GANG_SCHEDULER_NAME_ENV_KEY)
 
 
 @pytest.mark.skipif(
     GANG_SCHEDULER_NAME in NONE_GANG_SCHEDULERS, reason="For gang-scheduling",
 )
-def test_sdk_e2e_with_gang_scheduling():
-    launcher_container, worker_container = generate_containers()
+def test_sdk_e2e_with_gang_scheduling(job_namespace):
+    container = generate_container()
 
-    launcher = V1ReplicaSpec(
+    master = KubeflowOrgV1ReplicaSpec(
         replicas=1,
-        restart_policy="Never",
-        template=V1PodTemplateSpec(spec=V1PodSpec(
-            containers=[launcher_container],
-            scheduler_name=get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
-        )),
+        restart_policy="OnFailure",
+        template=V1PodTemplateSpec(
+            metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
+            spec=V1PodSpec(
+                scheduler_name=get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
+                containers=[container],
+            )
+        ),
     )
 
-    worker = V1ReplicaSpec(
+    worker = KubeflowOrgV1ReplicaSpec(
         replicas=1,
-        restart_policy="Never",
-        template=V1PodTemplateSpec(spec=V1PodSpec(
-            containers=[worker_container],
-            scheduler_name=get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
-        )),
+        restart_policy="OnFailure",
+        template=V1PodTemplateSpec(
+            metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
+            spec=V1PodSpec(
+                scheduler_name=get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
+                containers=[container],
+            )
+        ),
     )
 
-    mpijob = generate_mpijob(launcher, worker, V1SchedulingPolicy(min_available=10))
-    patched_mpijob = generate_mpijob(launcher, worker, V1SchedulingPolicy(min_available=2))
-
-    TRAINING_CLIENT.create_mpijob(mpijob, JOB_NAMESPACE)
-    logging.info(f"List of created {constants.MPIJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_mpijobs(JOB_NAMESPACE))
+    unschedulable_pytorchjob = generate_pytorchjob(master, worker, KubeflowOrgV1SchedulingPolicy(min_available=10), job_namespace)
+    schedulable_pytorchjob = generate_pytorchjob(master, worker, KubeflowOrgV1SchedulingPolicy(min_available=2), job_namespace)
+
+    TRAINING_CLIENT.create_pytorchjob(unschedulable_pytorchjob, job_namespace)
+    logging.info(f"List of created {constants.PYTORCHJOB_KIND}s")
+    logging.info(TRAINING_CLIENT.list_pytorchjobs(job_namespace))
 
     verify_unschedulable_job_e2e(
         TRAINING_CLIENT,
         JOB_NAME,
-        JOB_NAMESPACE,
-        constants.MPIJOB_KIND,
+        job_namespace,
+        constants.PYTORCHJOB_KIND,
     )
 
-    TRAINING_CLIENT.patch_mpijob(patched_mpijob, JOB_NAME, JOB_NAMESPACE)
-    logging.info(f"List of patched {constants.MPIJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_mpijobs(JOB_NAMESPACE))
+    TRAINING_CLIENT.patch_pytorchjob(schedulable_pytorchjob, JOB_NAME, job_namespace)
+    logging.info(f"List of patched {constants.PYTORCHJOB_KIND}s")
+    logging.info(TRAINING_CLIENT.list_pytorchjobs(job_namespace))
 
     verify_job_e2e(
         TRAINING_CLIENT,
         JOB_NAME,
-        JOB_NAMESPACE,
-        constants.MPIJOB_KIND,
+        job_namespace,
+        constants.PYTORCHJOB_KIND,
         CONTAINER_NAME,
+        timeout=900,
     )
 
-    TRAINING_CLIENT.delete_mpijob(JOB_NAME, JOB_NAMESPACE)
+    TRAINING_CLIENT.delete_pytorchjob(JOB_NAME, job_namespace)
 
 
 @pytest.mark.skipif(
     GANG_SCHEDULER_NAME in GANG_SCHEDULERS, reason="For plain scheduling",
 )
-def test_sdk_e2e():
-    launcher_container, worker_container = generate_containers()
+def test_sdk_e2e(job_namespace):
+    container = generate_container()
 
-    launcher = V1ReplicaSpec(
+    master = KubeflowOrgV1ReplicaSpec(
         replicas=1,
-        restart_policy="Never",
-        template=V1PodTemplateSpec(spec=V1PodSpec(containers=[launcher_container])),
+        restart_policy="OnFailure",
+        template=V1PodTemplateSpec(metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
+                                   spec=V1PodSpec(containers=[container])),
     )
 
-    worker = V1ReplicaSpec(
+    worker = KubeflowOrgV1ReplicaSpec(
         replicas=1,
-        restart_policy="Never",
-        template=V1PodTemplateSpec(spec=V1PodSpec(containers=[worker_container])),
+        restart_policy="OnFailure",
+        template=V1PodTemplateSpec(metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
+                                   spec=V1PodSpec(containers=[container])),
     )
 
-    mpijob = generate_mpijob(launcher, worker, None)
+    pytorchjob = generate_pytorchjob(master, worker, job_namespace=job_namespace)
 
-    TRAINING_CLIENT.create_mpijob(mpijob, JOB_NAMESPACE)
-    logging.info(f"List of created {constants.MPIJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_mpijobs(JOB_NAMESPACE))
+    TRAINING_CLIENT.create_pytorchjob(pytorchjob, job_namespace)
+    logging.info(f"List of created {constants.PYTORCHJOB_KIND}s")
+    logging.info(TRAINING_CLIENT.list_pytorchjobs(job_namespace))
 
     verify_job_e2e(
         TRAINING_CLIENT,
         JOB_NAME,
-        JOB_NAMESPACE,
-        constants.MPIJOB_KIND,
+        job_namespace,
+        constants.PYTORCHJOB_KIND,
         CONTAINER_NAME,
+        timeout=900,
     )
 
-    TRAINING_CLIENT.delete_mpijob(JOB_NAME, JOB_NAMESPACE)
+    TRAINING_CLIENT.delete_pytorchjob(JOB_NAME, job_namespace)
 
 
-def generate_mpijob(
-    launcher: V1ReplicaSpec,
-    worker: V1ReplicaSpec,
-    scheduling_policy: V1SchedulingPolicy = None,
-) -> KubeflowOrgV1MPIJob:
-    return KubeflowOrgV1MPIJob(
+def generate_pytorchjob(
+    master: KubeflowOrgV1ReplicaSpec,
+    worker: KubeflowOrgV1ReplicaSpec,
+    scheduling_policy: KubeflowOrgV1SchedulingPolicy = None,
+    job_namespace: str = "default",
+) -> KubeflowOrgV1PyTorchJob:
+    return KubeflowOrgV1PyTorchJob(
         api_version="kubeflow.org/v1",
-        kind="MPIJob",
-        metadata=V1ObjectMeta(name=JOB_NAME, namespace=JOB_NAMESPACE),
-        spec=KubeflowOrgV1MPIJobSpec(
-            slots_per_worker=1,
-            run_policy=V1RunPolicy(
+        kind="PyTorchJob",
+        metadata=V1ObjectMeta(name=JOB_NAME, namespace=job_namespace),
+        spec=KubeflowOrgV1PyTorchJobSpec(
+            run_policy=KubeflowOrgV1RunPolicy(
                 clean_pod_policy="None",
                 scheduling_policy=scheduling_policy,
             ),
-            mpi_replica_specs={"Launcher": launcher, "Worker": worker},
+            pytorch_replica_specs={"Master": master, "Worker": worker},
         ),
     )
 
 
-def generate_containers() -> Tuple[V1Container, V1Container]:
-    launcher_container = V1Container(
+def generate_container() -> V1Container:
+    return V1Container(
         name=CONTAINER_NAME,
-        image="horovod/horovod:0.20.0-tf2.3.0-torch1.6.0-mxnet1.5.0-py3.7-cpu",
-        command=["mpirun"],
-        args=[
-            "-np",
-            "1",
-            "--allow-run-as-root",
-            "-bind-to",
-            "none",
-            "-map-by",
-            "slot",
-            "-x",
-            "LD_LIBRARY_PATH",
-            "-x",
-            "PATH",
-            "-mca",
-            "pml",
-            "ob1",
-            "-mca",
-            "btl",
-            "^openib",
-            # "python", "/examples/tensorflow2_mnist.py"]
-            "python",
-            "/examples/pytorch_mnist.py",
-            "--epochs",
-            "1",
-        ],
-    )
-
-    worker_container = V1Container(
-        name="mpi",
-        image="horovod/horovod:0.20.0-tf2.3.0-torch1.6.0-mxnet1.5.0-py3.7-cpu",
+        image="gcr.io/kubeflow-ci/pytorch-dist-mnist-test:v1.0",
+        args=["--backend", "gloo"],
+        resources=V1ResourceRequirements(limits={"memory": "1Gi", "cpu": "0.4"}),
     )
-
-    return launcher_container, worker_container
```

### Comparing `kubeflow-training-1.6.0rc0/test/e2e/test_e2e_mxjob.py` & `kubeflow-training-1.7.0rc0/test/e2e/test_e2e_mxjob.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,153 +18,166 @@
 from typing import Tuple
 
 from kubernetes.client import V1PodTemplateSpec
 from kubernetes.client import V1ObjectMeta
 from kubernetes.client import V1PodSpec
 from kubernetes.client import V1Container
 from kubernetes.client import V1ContainerPort
+from kubernetes.client import V1ResourceRequirements
 
 from kubeflow.training import TrainingClient
-from kubeflow.training import V1ReplicaSpec
+from kubeflow.training import KubeflowOrgV1ReplicaSpec
 from kubeflow.training import KubeflowOrgV1MXJob
 from kubeflow.training import KubeflowOrgV1MXJobSpec
-from kubeflow.training import V1RunPolicy
-from kubeflow.training import V1SchedulingPolicy
+from kubeflow.training import KubeflowOrgV1RunPolicy
+from kubeflow.training import KubeflowOrgV1SchedulingPolicy
 from kubeflow.training.constants import constants
 
 from test.e2e.utils import verify_job_e2e, verify_unschedulable_job_e2e, get_pod_spec_scheduler_name
 from test.e2e.constants import TEST_GANG_SCHEDULER_NAME_ENV_KEY
 from test.e2e.constants import GANG_SCHEDULERS, NONE_GANG_SCHEDULERS
 
 logging.basicConfig(format="%(message)s")
 logging.getLogger().setLevel(logging.INFO)
 
-TRAINING_CLIENT = TrainingClient(config_file=os.getenv("KUBECONFIG", "~/.kube/config"))
+TRAINING_CLIENT = TrainingClient()
 JOB_NAME = "mxjob-mnist-ci-test"
-JOB_NAMESPACE = "default"
 CONTAINER_NAME = "mxnet"
 GANG_SCHEDULER_NAME = os.getenv(TEST_GANG_SCHEDULER_NAME_ENV_KEY)
 
 
 @pytest.mark.skipif(
     GANG_SCHEDULER_NAME in NONE_GANG_SCHEDULERS, reason="For gang-scheduling",
 )
-def test_sdk_e2e_with_gang_scheduling():
+def test_sdk_e2e_with_gang_scheduling(job_namespace):
     worker_container, server_container, scheduler_container = generate_containers()
 
-    worker = V1ReplicaSpec(
+    worker = KubeflowOrgV1ReplicaSpec(
         replicas=1,
         restart_policy="Never",
-        template=V1PodTemplateSpec(spec=V1PodSpec(
-            containers=[worker_container],
-            scheduler_name=get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
-        )),
+        template=V1PodTemplateSpec(
+            metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
+            spec=V1PodSpec(
+                containers=[worker_container],
+                scheduler_name=get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
+            )
+        ),
     )
 
-    server = V1ReplicaSpec(
+    server = KubeflowOrgV1ReplicaSpec(
         replicas=1,
         restart_policy="Never",
-        template=V1PodTemplateSpec(spec=V1PodSpec(
-            containers=[server_container],
-            scheduler_name=get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
-        )),
+        template=V1PodTemplateSpec(
+            metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
+            spec=V1PodSpec(
+                containers=[server_container],
+                scheduler_name=get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
+            )
+        ),
     )
 
-    scheduler = V1ReplicaSpec(
+    scheduler = KubeflowOrgV1ReplicaSpec(
         replicas=1,
         restart_policy="Never",
-        template=V1PodTemplateSpec(spec=V1PodSpec(
-            containers=[scheduler_container],
-            scheduler_name=get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
-        )),
+        template=V1PodTemplateSpec(
+            metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
+            spec=V1PodSpec(
+                containers=[scheduler_container],
+                scheduler_name=get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
+            )
+        ),
     )
 
-    unschedulable_mxjob = generate_mxjob(scheduler, server, worker, V1SchedulingPolicy(min_available=10))
-    schedulable_mxjob = generate_mxjob(scheduler, server, worker, V1SchedulingPolicy(min_available=3))
+    unschedulable_mxjob = generate_mxjob(scheduler, server, worker, KubeflowOrgV1SchedulingPolicy(min_available=10), job_namespace)
+    schedulable_mxjob = generate_mxjob(scheduler, server, worker, KubeflowOrgV1SchedulingPolicy(min_available=3), job_namespace)
 
-    TRAINING_CLIENT.create_mxjob(unschedulable_mxjob, JOB_NAMESPACE)
+    TRAINING_CLIENT.create_mxjob(unschedulable_mxjob, job_namespace)
     logging.info(f"List of created {constants.MXJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_mxjobs(JOB_NAMESPACE))
+    logging.info(TRAINING_CLIENT.list_mxjobs(job_namespace))
 
     verify_unschedulable_job_e2e(
         TRAINING_CLIENT,
         JOB_NAME,
-        JOB_NAMESPACE,
+        job_namespace,
         constants.MXJOB_KIND,
     )
 
-    TRAINING_CLIENT.patch_mxjob(schedulable_mxjob, JOB_NAME, JOB_NAMESPACE)
+    TRAINING_CLIENT.patch_mxjob(schedulable_mxjob, JOB_NAME, job_namespace)
     logging.info(f"List of patched {constants.MXJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_mxjobs(JOB_NAMESPACE))
+    logging.info(TRAINING_CLIENT.list_mxjobs(job_namespace))
 
     verify_job_e2e(
         TRAINING_CLIENT,
         JOB_NAME,
-        JOB_NAMESPACE,
+        job_namespace,
         constants.MXJOB_KIND,
         CONTAINER_NAME,
     )
 
-    TRAINING_CLIENT.delete_mxjob(JOB_NAME, JOB_NAMESPACE)
+    TRAINING_CLIENT.delete_mxjob(JOB_NAME, job_namespace)
 
 
 @pytest.mark.skipif(
     GANG_SCHEDULER_NAME in GANG_SCHEDULERS, reason="For plain scheduling",
 )
-def test_sdk_e2e():
+def test_sdk_e2e(job_namespace):
     worker_container, server_container, scheduler_container = generate_containers()
 
-    worker = V1ReplicaSpec(
+    worker = KubeflowOrgV1ReplicaSpec(
         replicas=1,
         restart_policy="Never",
-        template=V1PodTemplateSpec(spec=V1PodSpec(containers=[worker_container])),
+        template=V1PodTemplateSpec(metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
+                                   spec=V1PodSpec(containers=[worker_container])),
     )
 
-    server = V1ReplicaSpec(
+    server = KubeflowOrgV1ReplicaSpec(
         replicas=1,
         restart_policy="Never",
-        template=V1PodTemplateSpec(spec=V1PodSpec(containers=[server_container])),
+        template=V1PodTemplateSpec(metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
+                                   spec=V1PodSpec(containers=[server_container])),
     )
 
-    scheduler = V1ReplicaSpec(
+    scheduler = KubeflowOrgV1ReplicaSpec(
         replicas=1,
         restart_policy="Never",
-        template=V1PodTemplateSpec(spec=V1PodSpec(containers=[scheduler_container])),
+        template=V1PodTemplateSpec(metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
+                                   spec=V1PodSpec(containers=[scheduler_container])),
     )
 
-    mxjob = generate_mxjob(scheduler, server, worker)
+    mxjob = generate_mxjob(scheduler, server, worker, job_namespace=job_namespace)
 
-    TRAINING_CLIENT.create_mxjob(mxjob, JOB_NAMESPACE)
+    TRAINING_CLIENT.create_mxjob(mxjob, job_namespace)
     logging.info(f"List of created {constants.MXJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_mxjobs(JOB_NAMESPACE))
+    logging.info(TRAINING_CLIENT.list_mxjobs(job_namespace))
 
     verify_job_e2e(
         TRAINING_CLIENT,
         JOB_NAME,
-        JOB_NAMESPACE,
+        job_namespace,
         constants.MXJOB_KIND,
         CONTAINER_NAME,
     )
 
-    TRAINING_CLIENT.delete_mxjob(JOB_NAME, JOB_NAMESPACE)
+    TRAINING_CLIENT.delete_mxjob(JOB_NAME, job_namespace)
 
 
 def generate_mxjob(
-    scheduler: V1ReplicaSpec,
-    server: V1ReplicaSpec,
-    worker: V1ReplicaSpec,
-    scheduling_policy: V1SchedulingPolicy = None,
+    scheduler: KubeflowOrgV1ReplicaSpec,
+    server: KubeflowOrgV1ReplicaSpec,
+    worker: KubeflowOrgV1ReplicaSpec,
+    scheduling_policy: KubeflowOrgV1SchedulingPolicy = None,
+    job_namespace: str = "default",
 ) -> KubeflowOrgV1MXJob:
     return KubeflowOrgV1MXJob(
         api_version="kubeflow.org/v1",
         kind="MXJob",
-        metadata=V1ObjectMeta(name=JOB_NAME, namespace=JOB_NAMESPACE),
+        metadata=V1ObjectMeta(name=JOB_NAME, namespace=job_namespace),
         spec=KubeflowOrgV1MXJobSpec(
             job_mode="MXTrain",
-            run_policy=V1RunPolicy(
+            run_policy=KubeflowOrgV1RunPolicy(
                 clean_pod_policy="None",
                 scheduling_policy=scheduling_policy,
             ),
             mx_replica_specs={
                 "Scheduler": scheduler,
                 "Server": server,
                 "Worker": worker,
@@ -185,24 +198,27 @@
             "1",
             "--num-examples",
             "1000",
             "--kv-store",
             "dist_sync",
         ],
         ports=[V1ContainerPort(container_port=9991, name="mxjob-port")],
+        resources=V1ResourceRequirements(limits={"memory": "1Gi", "cpu": "0.25"}),
     )
 
     server_container = V1Container(
         name=CONTAINER_NAME,
         # TODO (tenzen-y): Replace the below image with the kubeflow hosted image
         image="docker.io/johnugeorge/mxnet:1.9.1_cpu_py3",
         ports=[V1ContainerPort(container_port=9991, name="mxjob-port")],
+        resources=V1ResourceRequirements(limits={"memory": "1Gi", "cpu": "0.25"}),
     )
 
     scheduler_container = V1Container(
         name=CONTAINER_NAME,
         # TODO (tenzen-y): Replace the below image with the kubeflow hosted image
         image="docker.io/johnugeorge/mxnet:1.9.1_cpu_py3",
         ports=[V1ContainerPort(container_port=9991, name="mxjob-port")],
+        resources=V1ResourceRequirements(limits={"memory": "1Gi", "cpu": "0.25"}),
     )
 
     return worker_container, server_container, scheduler_container
```

### Comparing `kubeflow-training-1.6.0rc0/test/e2e/test_e2e_paddlejob.py` & `kubeflow-training-1.7.0rc0/test/e2e/test_e2e_paddlejob.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,128 +16,134 @@
 import logging
 import pytest
 
 from kubernetes.client import V1PodTemplateSpec
 from kubernetes.client import V1ObjectMeta
 from kubernetes.client import V1PodSpec
 from kubernetes.client import V1Container
+from kubernetes.client import V1ResourceRequirements
 
 from kubeflow.training import TrainingClient
-from kubeflow.training import V1ReplicaSpec
+from kubeflow.training import KubeflowOrgV1ReplicaSpec
 from kubeflow.training import KubeflowOrgV1PaddleJob
 from kubeflow.training import KubeflowOrgV1PaddleJobSpec
-from kubeflow.training import V1RunPolicy
-from kubeflow.training import V1SchedulingPolicy
+from kubeflow.training import KubeflowOrgV1RunPolicy
+from kubeflow.training import KubeflowOrgV1SchedulingPolicy
 from kubeflow.training.constants import constants
 
 from test.e2e.utils import verify_job_e2e, verify_unschedulable_job_e2e, get_pod_spec_scheduler_name
 from test.e2e.constants import TEST_GANG_SCHEDULER_NAME_ENV_KEY
 from test.e2e.constants import GANG_SCHEDULERS, NONE_GANG_SCHEDULERS
 
 logging.basicConfig(format="%(message)s")
 logging.getLogger().setLevel(logging.INFO)
 
-TRAINING_CLIENT = TrainingClient(config_file=os.getenv("KUBECONFIG", "~/.kube/config"))
+TRAINING_CLIENT = TrainingClient()
 JOB_NAME = "paddlejob-cpu-ci-test"
-JOB_NAMESPACE = "default"
 CONTAINER_NAME = "paddle"
 GANG_SCHEDULER_NAME = os.getenv(TEST_GANG_SCHEDULER_NAME_ENV_KEY)
 
 
 @pytest.mark.skipif(
     GANG_SCHEDULER_NAME in NONE_GANG_SCHEDULERS, reason="For gang-scheduling",
 )
-def test_sdk_e2e_with_gang_scheduling():
+def test_sdk_e2e_with_gang_scheduling(job_namespace):
     container = generate_container()
 
-    worker = V1ReplicaSpec(
+    worker = KubeflowOrgV1ReplicaSpec(
         replicas=2,
         restart_policy="OnFailure",
-        template=V1PodTemplateSpec(spec=V1PodSpec(
-            scheduler_name=get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
-            containers=[container],
-        )),
+        template=V1PodTemplateSpec(
+            metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
+            spec=V1PodSpec(
+                scheduler_name=get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
+                containers=[container],
+            )
+        ),
     )
 
-    unschedulable_paddlejob = generate_paddlejob(worker, V1SchedulingPolicy(min_available=10))
-    schedulable_paddlejob = generate_paddlejob(worker, V1SchedulingPolicy(min_available=2))
+    unschedulable_paddlejob = generate_paddlejob(worker, KubeflowOrgV1SchedulingPolicy(min_available=10), job_namespace)
+    schedulable_paddlejob = generate_paddlejob(worker, KubeflowOrgV1SchedulingPolicy(min_available=2), job_namespace)
 
-    TRAINING_CLIENT.create_paddlejob(unschedulable_paddlejob, JOB_NAMESPACE)
+    TRAINING_CLIENT.create_paddlejob(unschedulable_paddlejob, job_namespace)
     logging.info(f"List of created {constants.PADDLEJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_paddlejobs(JOB_NAMESPACE))
+    logging.info(TRAINING_CLIENT.list_paddlejobs(job_namespace))
 
     verify_unschedulable_job_e2e(
         TRAINING_CLIENT,
         JOB_NAME,
-        JOB_NAMESPACE,
+        job_namespace,
         constants.PADDLEJOB_KIND,
     )
 
-    TRAINING_CLIENT.patch_paddlejob(schedulable_paddlejob, JOB_NAME, JOB_NAMESPACE)
+    TRAINING_CLIENT.patch_paddlejob(schedulable_paddlejob, JOB_NAME, job_namespace)
     logging.info(f"List of patched {constants.PADDLEJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_paddlejobs(JOB_NAMESPACE))
+    logging.info(TRAINING_CLIENT.list_paddlejobs(job_namespace))
 
     verify_job_e2e(
         TRAINING_CLIENT,
         JOB_NAME,
-        JOB_NAMESPACE,
+        job_namespace,
         constants.PADDLEJOB_KIND,
         CONTAINER_NAME,
     )
 
-    TRAINING_CLIENT.delete_paddlejob(JOB_NAME, JOB_NAMESPACE)
+    TRAINING_CLIENT.delete_paddlejob(JOB_NAME, job_namespace)
 
 
 @pytest.mark.skipif(
     GANG_SCHEDULER_NAME in GANG_SCHEDULERS, reason="For plain scheduling",
 )
-def test_sdk_e2e():
+def test_sdk_e2e(job_namespace):
     container = generate_container()
 
-    worker = V1ReplicaSpec(
+    worker = KubeflowOrgV1ReplicaSpec(
         replicas=2,
         restart_policy="OnFailure",
-        template=V1PodTemplateSpec(spec=V1PodSpec(containers=[container])),
+        template=V1PodTemplateSpec(metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
+                                   spec=V1PodSpec(containers=[container])),
     )
 
-    paddlejob = generate_paddlejob(worker)
+    paddlejob = generate_paddlejob(worker, job_namespace=job_namespace)
 
-    TRAINING_CLIENT.create_paddlejob(paddlejob, JOB_NAMESPACE)
+    TRAINING_CLIENT.create_paddlejob(paddlejob, job_namespace)
     logging.info(f"List of created {constants.PADDLEJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_paddlejobs(JOB_NAMESPACE))
+    logging.info(TRAINING_CLIENT.list_paddlejobs(job_namespace))
 
     verify_job_e2e(
         TRAINING_CLIENT,
         JOB_NAME,
-        JOB_NAMESPACE,
+        job_namespace,
         constants.PADDLEJOB_KIND,
         CONTAINER_NAME,
     )
 
-    TRAINING_CLIENT.delete_paddlejob(JOB_NAME, JOB_NAMESPACE)
+    TRAINING_CLIENT.delete_paddlejob(JOB_NAME, job_namespace)
 
 
 def generate_paddlejob(
-    worker: V1ReplicaSpec,
-    scheduling_policy: V1SchedulingPolicy = None,
+    worker: KubeflowOrgV1ReplicaSpec,
+    scheduling_policy: KubeflowOrgV1SchedulingPolicy = None,
+    job_namespace: str = "default",
 ) -> KubeflowOrgV1PaddleJob:
     return KubeflowOrgV1PaddleJob(
         api_version="kubeflow.org/v1",
         kind="PaddleJob",
-        metadata=V1ObjectMeta(name=JOB_NAME, namespace=JOB_NAMESPACE),
+        metadata=V1ObjectMeta(name=JOB_NAME, namespace=job_namespace),
         spec=KubeflowOrgV1PaddleJobSpec(
-            run_policy=V1RunPolicy(
+            run_policy=KubeflowOrgV1RunPolicy(
                 scheduling_policy=scheduling_policy,
                 clean_pod_policy="None",
             ),
             paddle_replica_specs={"Worker": worker},
         ),
     )
 
 
 def generate_container() -> V1Container:
     return V1Container(
         name=CONTAINER_NAME,
         image="docker.io/paddlepaddle/paddle:2.4.0rc0-cpu",
         command=["python"],
         args=["-m", "paddle.distributed.launch", "run_check"],
+        resources=V1ResourceRequirements(limits={"memory": "1Gi", "cpu": "0.4"}),
     )
```

### Comparing `kubeflow-training-1.6.0rc0/test/e2e/test_e2e_tfjob.py` & `kubeflow-training-1.7.0rc0/test/e2e/test_e2e_tfjob.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,116 +16,121 @@
 import logging
 import pytest
 
 from kubernetes.client import V1PodTemplateSpec
 from kubernetes.client import V1ObjectMeta
 from kubernetes.client import V1PodSpec
 from kubernetes.client import V1Container
+from kubernetes.client import V1ResourceRequirements
 
 from kubeflow.training import TrainingClient
-from kubeflow.training import V1ReplicaSpec
-from kubeflow.training import V1RunPolicy
+from kubeflow.training import KubeflowOrgV1ReplicaSpec
+from kubeflow.training import KubeflowOrgV1RunPolicy
 from kubeflow.training import KubeflowOrgV1TFJob
 from kubeflow.training import KubeflowOrgV1TFJobSpec
-from kubeflow.training import V1SchedulingPolicy
+from kubeflow.training import KubeflowOrgV1SchedulingPolicy
 from kubeflow.training.constants import constants
 
 from test.e2e.utils import verify_job_e2e, verify_unschedulable_job_e2e, get_pod_spec_scheduler_name
 from test.e2e.constants import TEST_GANG_SCHEDULER_NAME_ENV_KEY
 from test.e2e.constants import GANG_SCHEDULERS, NONE_GANG_SCHEDULERS
 
 logging.basicConfig(format="%(message)s")
 logging.getLogger().setLevel(logging.INFO)
 
-TRAINING_CLIENT = TrainingClient(config_file=os.getenv("KUBECONFIG", "~/.kube/config"))
+TRAINING_CLIENT = TrainingClient()
 JOB_NAME = "tfjob-mnist-ci-test"
-JOB_NAMESPACE = "default"
 CONTAINER_NAME = "tensorflow"
 GANG_SCHEDULER_NAME = os.getenv(TEST_GANG_SCHEDULER_NAME_ENV_KEY)
 
 
 @pytest.mark.skipif(
     GANG_SCHEDULER_NAME in NONE_GANG_SCHEDULERS, reason="For gang-scheduling",
 )
-def test_sdk_e2e_with_gang_scheduling():
+def test_sdk_e2e_with_gang_scheduling(job_namespace):
     container = generate_container()
 
-    worker = V1ReplicaSpec(
+    worker = KubeflowOrgV1ReplicaSpec(
         replicas=1,
         restart_policy="Never",
-        template=V1PodTemplateSpec(spec=V1PodSpec(
-            containers=[container],
-            scheduler_name=get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
-        )),
+        template=V1PodTemplateSpec(
+            metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
+            spec=V1PodSpec(
+                containers=[container],
+                scheduler_name=get_pod_spec_scheduler_name(GANG_SCHEDULER_NAME),
+            )
+        ),
     )
 
-    unschedulable_tfjob = generate_tfjob(worker, V1SchedulingPolicy(min_available=10))
-    schedulable_tfjob = generate_tfjob(worker, V1SchedulingPolicy(min_available=1))
+    unschedulable_tfjob = generate_tfjob(worker, KubeflowOrgV1SchedulingPolicy(min_available=10), job_namespace)
+    schedulable_tfjob = generate_tfjob(worker, KubeflowOrgV1SchedulingPolicy(min_available=1), job_namespace)
 
-    TRAINING_CLIENT.create_tfjob(unschedulable_tfjob, JOB_NAMESPACE)
+    TRAINING_CLIENT.create_tfjob(unschedulable_tfjob, job_namespace)
     logging.info(f"List of created {constants.TFJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_tfjobs(JOB_NAMESPACE))
+    logging.info(TRAINING_CLIENT.list_tfjobs(job_namespace))
 
     verify_unschedulable_job_e2e(
         TRAINING_CLIENT,
         JOB_NAME,
-        JOB_NAMESPACE,
+        job_namespace,
         constants.TFJOB_KIND,
     )
 
-    TRAINING_CLIENT.patch_tfjob(schedulable_tfjob, JOB_NAME, JOB_NAMESPACE)
+    TRAINING_CLIENT.patch_tfjob(schedulable_tfjob, JOB_NAME, job_namespace)
     logging.info(f"List of patched {constants.TFJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_tfjobs(JOB_NAMESPACE))
+    logging.info(TRAINING_CLIENT.list_tfjobs(job_namespace))
 
     verify_job_e2e(
         TRAINING_CLIENT,
         JOB_NAME,
-        JOB_NAMESPACE,
+        job_namespace,
         constants.TFJOB_KIND,
         CONTAINER_NAME,
     )
 
-    TRAINING_CLIENT.delete_tfjob(JOB_NAME, JOB_NAMESPACE)
+    TRAINING_CLIENT.delete_tfjob(JOB_NAME, job_namespace)
 
 
 @pytest.mark.skipif(
     GANG_SCHEDULER_NAME in GANG_SCHEDULERS, reason="For plain scheduling",
 )
-def test_sdk_e2e():
+def test_sdk_e2e(job_namespace):
     container = generate_container()
 
-    worker = V1ReplicaSpec(
+    worker = KubeflowOrgV1ReplicaSpec(
         replicas=1,
         restart_policy="Never",
-        template=V1PodTemplateSpec(spec=V1PodSpec(containers=[container])),
+        template=V1PodTemplateSpec(metadata=V1ObjectMeta(annotations={constants.ISTIO_SIDECAR_INJECTION: "false"}),
+                                   spec=V1PodSpec(containers=[container])),
     )
 
-    tfjob = generate_tfjob(worker)
+    tfjob = generate_tfjob(worker, job_namespace=job_namespace)
 
-    TRAINING_CLIENT.create_tfjob(tfjob, JOB_NAMESPACE)
+    TRAINING_CLIENT.create_tfjob(tfjob, job_namespace)
     logging.info(f"List of created {constants.TFJOB_KIND}s")
-    logging.info(TRAINING_CLIENT.list_tfjobs(JOB_NAMESPACE))
+    logging.info(TRAINING_CLIENT.list_tfjobs(job_namespace))
 
     verify_job_e2e(
-        TRAINING_CLIENT, JOB_NAME, JOB_NAMESPACE, constants.TFJOB_KIND, CONTAINER_NAME,
+        TRAINING_CLIENT, JOB_NAME, job_namespace, constants.TFJOB_KIND, CONTAINER_NAME,
     )
 
-    TRAINING_CLIENT.delete_tfjob(JOB_NAME, JOB_NAMESPACE)
+    TRAINING_CLIENT.delete_tfjob(JOB_NAME, job_namespace)
 
 
 def generate_tfjob(
-    worker: V1ReplicaSpec,
-    scheduling_policy: V1SchedulingPolicy = None,
+    worker: KubeflowOrgV1ReplicaSpec,
+    scheduling_policy: KubeflowOrgV1SchedulingPolicy = None,
+    job_namespace: str = "default",
 ) -> KubeflowOrgV1TFJob:
     return KubeflowOrgV1TFJob(
         api_version="kubeflow.org/v1",
         kind="TFJob",
-        metadata=V1ObjectMeta(name=JOB_NAME, namespace=JOB_NAMESPACE),
+        metadata=V1ObjectMeta(name=JOB_NAME, namespace=job_namespace),
         spec=KubeflowOrgV1TFJobSpec(
-            run_policy=V1RunPolicy(
+            run_policy=KubeflowOrgV1RunPolicy(
                 clean_pod_policy="None",
                 scheduling_policy=scheduling_policy,
             ),
             tf_replica_specs={"Worker": worker},
         ),
     )
 
@@ -137,8 +142,9 @@
         command=[
             "python",
             "/var/tf_mnist/mnist_with_summaries.py",
             "--log_dir=/train/logs",
             "--learning_rate=0.01",
             "--batch_size=150",
         ],
+        resources=V1ResourceRequirements(limits={"memory": "2Gi", "cpu": "0.75"}),
     )
```

### Comparing `kubeflow-training-1.6.0rc0/test/e2e/utils.py` & `kubeflow-training-1.7.0rc0/test/e2e/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import time
 
 from kubeflow.training import TrainingClient
 from kubeflow.training.constants import constants
 from test.e2e.constants import TEST_GANG_SCHEDULER_NAME_SCHEDULER_PLUGINS
 from test.e2e.constants import DEFAULT_SCHEDULER_PLUGINS_NAME
 from test.e2e.constants import TEST_GANG_SCHEDULER_NAME_VOLCANO
 
@@ -13,32 +14,37 @@
 def verify_unschedulable_job_e2e(
     client: TrainingClient, name: str, namespace: str, job_kind: str
 ):
     """Verify unschedulable Training Job e2e test."""
     logging.info(f"\n\n\n{job_kind} is creating")
     client.wait_for_job_conditions(name, namespace, job_kind, {constants.JOB_CONDITION_CREATED})
 
-    # Job should have Created conditions.
-    conditions = client.get_job_conditions(name, namespace, job_kind)
-    if len(conditions) != 1:
-        raise Exception(f"{job_kind} conditions are invalid: {conditions}")
+    logging.info("Checking 3 times that pods are not scheduled")
+    for num in range(3):
+        logging.info(f"Number of attempts: {int(num)+1}/3")
+        # Job should have a Created condition.
+        if not client.is_job_created(name, namespace, job_kind):
+            raise Exception(f"{job_kind} should be in Created condition")
+
+        # Job shouldn't have a Running condition.
+        if client.is_job_running(name, namespace, job_kind):
+            raise Exception(f"{job_kind} shouldn't be in Running condition")
 
-    # Job should have correct conditions.
-    if not client.is_job_created(name, namespace, job_kind):
-        raise Exception(f"{job_kind} should be in Created condition")
+        logging.info("Sleeping 5 seconds...")
+        time.sleep(5)
 
 
 def verify_job_e2e(
-    client: TrainingClient, name: str, namespace: str, job_kind: str, container: str
+    client: TrainingClient, name: str, namespace: str, job_kind: str, container: str, timeout: int = 600
 ):
     """Verify Training Job e2e test."""
 
     # Wait until Job is Succeeded.
     logging.info(f"\n\n\n{job_kind} is running")
-    client.wait_for_job_conditions(name, namespace, job_kind)
+    client.wait_for_job_conditions(name, namespace, job_kind, timeout=timeout)
 
     # Job should have Created, Running, and Succeeded conditions.
     conditions = client.get_job_conditions(name, namespace, job_kind)
     if len(conditions) != 3:
         raise Exception(f"{job_kind} conditions are invalid: {conditions}")
 
     # Job should have correct conditions.
@@ -65,12 +71,11 @@
     logging.info(f"\n\n\n{job_kind} logs")
     client.get_job_logs(name, namespace, container=container)
 
 
 def get_pod_spec_scheduler_name(gang_scheduler_name: str) -> str:
     if gang_scheduler_name == TEST_GANG_SCHEDULER_NAME_SCHEDULER_PLUGINS:
         return DEFAULT_SCHEDULER_PLUGINS_NAME
-    # TODO (tenzen-y): Implement E2E tests using volcano.
     elif gang_scheduler_name == TEST_GANG_SCHEDULER_NAME_VOLCANO:
-        return ""
+        return TEST_GANG_SCHEDULER_NAME_VOLCANO
 
     return ""
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_elastic_policy.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_elastic_policy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_mpi_job.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_mpi_job.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -39,47 +39,48 @@
                 api_version = '0', 
                 kind = '0', 
                 metadata = None, 
                 spec = kubeflow_org_v1_mpi_job_spec.KubeflowOrgV1MPIJobSpec(
                     clean_pod_policy = '0', 
                     main_container = '0', 
                     mpi_replica_specs = {
-                        'key' : V1ReplicaSpec(
+                        'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
                             replicas = 56, 
                             restart_policy = '0', 
                             template = None, )
                         }, 
-                    run_policy = V1RunPolicy(
+                    run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                         active_deadline_seconds = 56, 
                         backoff_limit = 56, 
                         clean_pod_policy = '0', 
-                        scheduling_policy = V1SchedulingPolicy(
+                        scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                             min_available = 56, 
                             min_resources = {
                                 'key' : None
                                 }, 
                             priority_class = '0', 
                             queue = '0', 
                             schedule_timeout_seconds = 56, ), 
+                        suspend = True, 
                         ttl_seconds_after_finished = 56, ), 
                     slots_per_worker = 56, ), 
-                status = V1JobStatus(
+                status = kubeflow_org_v1_job_status.KubeflowOrgV1JobStatus(
                     completion_time = None, 
                     conditions = [
-                        V1JobCondition(
+                        kubeflow_org_v1_job_condition.KubeflowOrgV1JobCondition(
                             last_transition_time = None, 
                             last_update_time = None, 
                             message = '0', 
                             reason = '0', 
                             status = '0', 
                             type = '0', )
                         ], 
                     last_reconcile_time = None, 
                     replica_statuses = {
-                        'key' : V1ReplicaStatus(
+                        'key' : kubeflow_org_v1_replica_status.KubeflowOrgV1ReplicaStatus(
                             active = 56, 
                             failed = 56, 
                             label_selector = None, 
                             selector = '0', 
                             succeeded = 56, )
                         }, 
                     start_time = None, )
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_mpi_job_list.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_tf_job_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,154 +1,154 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 from kubeflow.training.models import *
-from kubeflow.training.models.kubeflow_org_v1_mpi_job_list import KubeflowOrgV1MPIJobList  # noqa: E501
+from kubeflow.training.models.kubeflow_org_v1_tf_job_list import KubeflowOrgV1TFJobList  # noqa: E501
 from kubeflow.training.rest import ApiException
 
-class TestKubeflowOrgV1MPIJobList(unittest.TestCase):
-    """KubeflowOrgV1MPIJobList unit test stubs"""
+class TestKubeflowOrgV1TFJobList(unittest.TestCase):
+    """KubeflowOrgV1TFJobList unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test KubeflowOrgV1MPIJobList
+        """Test KubeflowOrgV1TFJobList
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kubeflow.training.models.kubeflow_org_v1_mpi_job_list.KubeflowOrgV1MPIJobList()  # noqa: E501
+        # model = kubeflow.training.models.kubeflow_org_v1_tf_job_list.KubeflowOrgV1TFJobList()  # noqa: E501
         if include_optional :
-            return KubeflowOrgV1MPIJobList(
+            return KubeflowOrgV1TFJobList(
                 api_version = '0', 
                 items = [
-                    kubeflow_org_v1_mpi_job.KubeflowOrgV1MPIJob(
+                    kubeflow_org_v1_tf_job.KubeflowOrgV1TFJob(
                         api_version = '0', 
                         kind = '0', 
                         metadata = None, 
-                        spec = kubeflow_org_v1_mpi_job_spec.KubeflowOrgV1MPIJobSpec(
-                            clean_pod_policy = '0', 
-                            main_container = '0', 
-                            mpi_replica_specs = {
-                                'key' : V1ReplicaSpec(
-                                    replicas = 56, 
-                                    restart_policy = '0', 
-                                    template = None, )
-                                }, 
-                            run_policy = V1RunPolicy(
+                        spec = kubeflow_org_v1_tf_job_spec.KubeflowOrgV1TFJobSpec(
+                            enable_dynamic_worker = True, 
+                            run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                                 active_deadline_seconds = 56, 
                                 backoff_limit = 56, 
                                 clean_pod_policy = '0', 
-                                scheduling_policy = V1SchedulingPolicy(
+                                scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                                     min_available = 56, 
                                     min_resources = {
                                         'key' : None
                                         }, 
                                     priority_class = '0', 
                                     queue = '0', 
                                     schedule_timeout_seconds = 56, ), 
+                                suspend = True, 
                                 ttl_seconds_after_finished = 56, ), 
-                            slots_per_worker = 56, ), 
-                        status = V1JobStatus(
+                            success_policy = '0', 
+                            tf_replica_specs = {
+                                'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
+                                    replicas = 56, 
+                                    restart_policy = '0', 
+                                    template = None, )
+                                }, ), 
+                        status = kubeflow_org_v1_job_status.KubeflowOrgV1JobStatus(
                             completion_time = None, 
                             conditions = [
-                                V1JobCondition(
+                                kubeflow_org_v1_job_condition.KubeflowOrgV1JobCondition(
                                     last_transition_time = None, 
                                     last_update_time = None, 
                                     message = '0', 
                                     reason = '0', 
                                     status = '0', 
                                     type = '0', )
                                 ], 
                             last_reconcile_time = None, 
                             replica_statuses = {
-                                'key' : V1ReplicaStatus(
+                                'key' : kubeflow_org_v1_replica_status.KubeflowOrgV1ReplicaStatus(
                                     active = 56, 
                                     failed = 56, 
                                     label_selector = None, 
                                     selector = '0', 
                                     succeeded = 56, )
                                 }, 
                             start_time = None, ), )
                     ], 
                 kind = '0', 
                 metadata = None
             )
         else :
-            return KubeflowOrgV1MPIJobList(
+            return KubeflowOrgV1TFJobList(
                 items = [
-                    kubeflow_org_v1_mpi_job.KubeflowOrgV1MPIJob(
+                    kubeflow_org_v1_tf_job.KubeflowOrgV1TFJob(
                         api_version = '0', 
                         kind = '0', 
                         metadata = None, 
-                        spec = kubeflow_org_v1_mpi_job_spec.KubeflowOrgV1MPIJobSpec(
-                            clean_pod_policy = '0', 
-                            main_container = '0', 
-                            mpi_replica_specs = {
-                                'key' : V1ReplicaSpec(
-                                    replicas = 56, 
-                                    restart_policy = '0', 
-                                    template = None, )
-                                }, 
-                            run_policy = V1RunPolicy(
+                        spec = kubeflow_org_v1_tf_job_spec.KubeflowOrgV1TFJobSpec(
+                            enable_dynamic_worker = True, 
+                            run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                                 active_deadline_seconds = 56, 
                                 backoff_limit = 56, 
                                 clean_pod_policy = '0', 
-                                scheduling_policy = V1SchedulingPolicy(
+                                scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                                     min_available = 56, 
                                     min_resources = {
                                         'key' : None
                                         }, 
                                     priority_class = '0', 
                                     queue = '0', 
                                     schedule_timeout_seconds = 56, ), 
+                                suspend = True, 
                                 ttl_seconds_after_finished = 56, ), 
-                            slots_per_worker = 56, ), 
-                        status = V1JobStatus(
+                            success_policy = '0', 
+                            tf_replica_specs = {
+                                'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
+                                    replicas = 56, 
+                                    restart_policy = '0', 
+                                    template = None, )
+                                }, ), 
+                        status = kubeflow_org_v1_job_status.KubeflowOrgV1JobStatus(
                             completion_time = None, 
                             conditions = [
-                                V1JobCondition(
+                                kubeflow_org_v1_job_condition.KubeflowOrgV1JobCondition(
                                     last_transition_time = None, 
                                     last_update_time = None, 
                                     message = '0', 
                                     reason = '0', 
                                     status = '0', 
                                     type = '0', )
                                 ], 
                             last_reconcile_time = None, 
                             replica_statuses = {
-                                'key' : V1ReplicaStatus(
+                                'key' : kubeflow_org_v1_replica_status.KubeflowOrgV1ReplicaStatus(
                                     active = 56, 
                                     failed = 56, 
                                     label_selector = None, 
                                     selector = '0', 
                                     succeeded = 56, )
                                 }, 
                             start_time = None, ), )
                     ],
         )
 
-    def testKubeflowOrgV1MPIJobList(self):
-        """Test KubeflowOrgV1MPIJobList"""
+    def testKubeflowOrgV1TFJobList(self):
+        """Test KubeflowOrgV1TFJobList"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_mpi_job_spec.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_run_policy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,64 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 from kubeflow.training.models import *
-from kubeflow.training.models.kubeflow_org_v1_mpi_job_spec import KubeflowOrgV1MPIJobSpec  # noqa: E501
+from kubeflow.training.models.kubeflow_org_v1_run_policy import KubeflowOrgV1RunPolicy  # noqa: E501
 from kubeflow.training.rest import ApiException
 
-class TestKubeflowOrgV1MPIJobSpec(unittest.TestCase):
-    """KubeflowOrgV1MPIJobSpec unit test stubs"""
+class TestKubeflowOrgV1RunPolicy(unittest.TestCase):
+    """KubeflowOrgV1RunPolicy unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test KubeflowOrgV1MPIJobSpec
+        """Test KubeflowOrgV1RunPolicy
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kubeflow.training.models.kubeflow_org_v1_mpi_job_spec.KubeflowOrgV1MPIJobSpec()  # noqa: E501
+        # model = kubeflow.training.models.kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy()  # noqa: E501
         if include_optional :
-            return KubeflowOrgV1MPIJobSpec(
+            return KubeflowOrgV1RunPolicy(
+                active_deadline_seconds = 56, 
+                backoff_limit = 56, 
                 clean_pod_policy = '0', 
-                main_container = '0', 
-                mpi_replica_specs = {
-                    'key' : V1ReplicaSpec(
-                        replicas = 56, 
-                        restart_policy = '0', 
-                        template = None, )
-                    }, 
-                run_policy = V1RunPolicy(
-                    active_deadline_seconds = 56, 
-                    backoff_limit = 56, 
-                    clean_pod_policy = '0', 
-                    scheduling_policy = V1SchedulingPolicy(
-                        min_available = 56, 
-                        min_resources = {
-                            'key' : None
-                            }, 
-                        priority_class = '0', 
-                        queue = '0', 
-                        schedule_timeout_seconds = 56, ), 
-                    ttl_seconds_after_finished = 56, ), 
-                slots_per_worker = 56
+                scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
+                    min_available = 56, 
+                    min_resources = {
+                        'key' : None
+                        }, 
+                    priority_class = '0', 
+                    queue = '0', 
+                    schedule_timeout_seconds = 56, ), 
+                suspend = True, 
+                ttl_seconds_after_finished = 56
             )
         else :
-            return KubeflowOrgV1MPIJobSpec(
-                mpi_replica_specs = {
-                    'key' : V1ReplicaSpec(
-                        replicas = 56, 
-                        restart_policy = '0', 
-                        template = None, )
-                    },
+            return KubeflowOrgV1RunPolicy(
         )
 
-    def testKubeflowOrgV1MPIJobSpec(self):
-        """Test KubeflowOrgV1MPIJobSpec"""
+    def testKubeflowOrgV1RunPolicy(self):
+        """Test KubeflowOrgV1RunPolicy"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_mx_job.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_mx_job.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -38,46 +38,47 @@
             return KubeflowOrgV1MXJob(
                 api_version = '0', 
                 kind = '0', 
                 metadata = None, 
                 spec = kubeflow_org_v1_mx_job_spec.KubeflowOrgV1MXJobSpec(
                     job_mode = '0', 
                     mx_replica_specs = {
-                        'key' : V1ReplicaSpec(
+                        'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
                             replicas = 56, 
                             restart_policy = '0', 
                             template = None, )
                         }, 
-                    run_policy = V1RunPolicy(
+                    run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                         active_deadline_seconds = 56, 
                         backoff_limit = 56, 
                         clean_pod_policy = '0', 
-                        scheduling_policy = V1SchedulingPolicy(
+                        scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                             min_available = 56, 
                             min_resources = {
                                 'key' : None
                                 }, 
                             priority_class = '0', 
                             queue = '0', 
                             schedule_timeout_seconds = 56, ), 
+                        suspend = True, 
                         ttl_seconds_after_finished = 56, ), ), 
-                status = V1JobStatus(
+                status = kubeflow_org_v1_job_status.KubeflowOrgV1JobStatus(
                     completion_time = None, 
                     conditions = [
-                        V1JobCondition(
+                        kubeflow_org_v1_job_condition.KubeflowOrgV1JobCondition(
                             last_transition_time = None, 
                             last_update_time = None, 
                             message = '0', 
                             reason = '0', 
                             status = '0', 
                             type = '0', )
                         ], 
                     last_reconcile_time = None, 
                     replica_statuses = {
-                        'key' : V1ReplicaStatus(
+                        'key' : kubeflow_org_v1_replica_status.KubeflowOrgV1ReplicaStatus(
                             active = 56, 
                             failed = 56, 
                             label_selector = None, 
                             selector = '0', 
                             succeeded = 56, )
                         }, 
                     start_time = None, )
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_mx_job_list.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_xg_boost_job_list.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,150 +1,150 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 from kubeflow.training.models import *
-from kubeflow.training.models.kubeflow_org_v1_mx_job_list import KubeflowOrgV1MXJobList  # noqa: E501
+from kubeflow.training.models.kubeflow_org_v1_xg_boost_job_list import KubeflowOrgV1XGBoostJobList  # noqa: E501
 from kubeflow.training.rest import ApiException
 
-class TestKubeflowOrgV1MXJobList(unittest.TestCase):
-    """KubeflowOrgV1MXJobList unit test stubs"""
+class TestKubeflowOrgV1XGBoostJobList(unittest.TestCase):
+    """KubeflowOrgV1XGBoostJobList unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test KubeflowOrgV1MXJobList
+        """Test KubeflowOrgV1XGBoostJobList
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kubeflow.training.models.kubeflow_org_v1_mx_job_list.KubeflowOrgV1MXJobList()  # noqa: E501
+        # model = kubeflow.training.models.kubeflow_org_v1_xg_boost_job_list.KubeflowOrgV1XGBoostJobList()  # noqa: E501
         if include_optional :
-            return KubeflowOrgV1MXJobList(
+            return KubeflowOrgV1XGBoostJobList(
                 api_version = '0', 
                 items = [
-                    kubeflow_org_v1_mx_job.KubeflowOrgV1MXJob(
+                    kubeflow_org_v1_xg_boost_job.KubeflowOrgV1XGBoostJob(
                         api_version = '0', 
                         kind = '0', 
                         metadata = None, 
-                        spec = kubeflow_org_v1_mx_job_spec.KubeflowOrgV1MXJobSpec(
-                            job_mode = '0', 
-                            mx_replica_specs = {
-                                'key' : V1ReplicaSpec(
-                                    replicas = 56, 
-                                    restart_policy = '0', 
-                                    template = None, )
-                                }, 
-                            run_policy = V1RunPolicy(
+                        spec = kubeflow_org_v1_xg_boost_job_spec.KubeflowOrgV1XGBoostJobSpec(
+                            run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                                 active_deadline_seconds = 56, 
                                 backoff_limit = 56, 
                                 clean_pod_policy = '0', 
-                                scheduling_policy = V1SchedulingPolicy(
+                                scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                                     min_available = 56, 
                                     min_resources = {
                                         'key' : None
                                         }, 
                                     priority_class = '0', 
                                     queue = '0', 
                                     schedule_timeout_seconds = 56, ), 
-                                ttl_seconds_after_finished = 56, ), ), 
-                        status = V1JobStatus(
+                                suspend = True, 
+                                ttl_seconds_after_finished = 56, ), 
+                            xgb_replica_specs = {
+                                'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
+                                    replicas = 56, 
+                                    restart_policy = '0', 
+                                    template = None, )
+                                }, ), 
+                        status = kubeflow_org_v1_job_status.KubeflowOrgV1JobStatus(
                             completion_time = None, 
                             conditions = [
-                                V1JobCondition(
+                                kubeflow_org_v1_job_condition.KubeflowOrgV1JobCondition(
                                     last_transition_time = None, 
                                     last_update_time = None, 
                                     message = '0', 
                                     reason = '0', 
                                     status = '0', 
                                     type = '0', )
                                 ], 
                             last_reconcile_time = None, 
                             replica_statuses = {
-                                'key' : V1ReplicaStatus(
+                                'key' : kubeflow_org_v1_replica_status.KubeflowOrgV1ReplicaStatus(
                                     active = 56, 
                                     failed = 56, 
                                     label_selector = None, 
                                     selector = '0', 
                                     succeeded = 56, )
                                 }, 
                             start_time = None, ), )
                     ], 
                 kind = '0', 
                 metadata = None
             )
         else :
-            return KubeflowOrgV1MXJobList(
+            return KubeflowOrgV1XGBoostJobList(
                 items = [
-                    kubeflow_org_v1_mx_job.KubeflowOrgV1MXJob(
+                    kubeflow_org_v1_xg_boost_job.KubeflowOrgV1XGBoostJob(
                         api_version = '0', 
                         kind = '0', 
                         metadata = None, 
-                        spec = kubeflow_org_v1_mx_job_spec.KubeflowOrgV1MXJobSpec(
-                            job_mode = '0', 
-                            mx_replica_specs = {
-                                'key' : V1ReplicaSpec(
-                                    replicas = 56, 
-                                    restart_policy = '0', 
-                                    template = None, )
-                                }, 
-                            run_policy = V1RunPolicy(
+                        spec = kubeflow_org_v1_xg_boost_job_spec.KubeflowOrgV1XGBoostJobSpec(
+                            run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                                 active_deadline_seconds = 56, 
                                 backoff_limit = 56, 
                                 clean_pod_policy = '0', 
-                                scheduling_policy = V1SchedulingPolicy(
+                                scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                                     min_available = 56, 
                                     min_resources = {
                                         'key' : None
                                         }, 
                                     priority_class = '0', 
                                     queue = '0', 
                                     schedule_timeout_seconds = 56, ), 
-                                ttl_seconds_after_finished = 56, ), ), 
-                        status = V1JobStatus(
+                                suspend = True, 
+                                ttl_seconds_after_finished = 56, ), 
+                            xgb_replica_specs = {
+                                'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
+                                    replicas = 56, 
+                                    restart_policy = '0', 
+                                    template = None, )
+                                }, ), 
+                        status = kubeflow_org_v1_job_status.KubeflowOrgV1JobStatus(
                             completion_time = None, 
                             conditions = [
-                                V1JobCondition(
+                                kubeflow_org_v1_job_condition.KubeflowOrgV1JobCondition(
                                     last_transition_time = None, 
                                     last_update_time = None, 
                                     message = '0', 
                                     reason = '0', 
                                     status = '0', 
                                     type = '0', )
                                 ], 
                             last_reconcile_time = None, 
                             replica_statuses = {
-                                'key' : V1ReplicaStatus(
+                                'key' : kubeflow_org_v1_replica_status.KubeflowOrgV1ReplicaStatus(
                                     active = 56, 
                                     failed = 56, 
                                     label_selector = None, 
                                     selector = '0', 
                                     succeeded = 56, )
                                 }, 
                             start_time = None, ), )
                     ],
         )
 
-    def testKubeflowOrgV1MXJobList(self):
-        """Test KubeflowOrgV1MXJobList"""
+    def testKubeflowOrgV1XGBoostJobList(self):
+        """Test KubeflowOrgV1XGBoostJobList"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_mx_job_spec.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_mx_job_spec.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -34,54 +34,56 @@
             params are included, when True both required and
             optional params are included """
         # model = kubeflow.training.models.kubeflow_org_v1_mx_job_spec.KubeflowOrgV1MXJobSpec()  # noqa: E501
         if include_optional :
             return KubeflowOrgV1MXJobSpec(
                 job_mode = '0', 
                 mx_replica_specs = {
-                    'key' : V1ReplicaSpec(
+                    'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
                         replicas = 56, 
                         restart_policy = '0', 
                         template = None, )
                     }, 
-                run_policy = V1RunPolicy(
+                run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                     active_deadline_seconds = 56, 
                     backoff_limit = 56, 
                     clean_pod_policy = '0', 
-                    scheduling_policy = V1SchedulingPolicy(
+                    scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                         min_available = 56, 
                         min_resources = {
                             'key' : None
                             }, 
                         priority_class = '0', 
                         queue = '0', 
                         schedule_timeout_seconds = 56, ), 
+                    suspend = True, 
                     ttl_seconds_after_finished = 56, )
             )
         else :
             return KubeflowOrgV1MXJobSpec(
                 job_mode = '0',
                 mx_replica_specs = {
-                    'key' : V1ReplicaSpec(
+                    'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
                         replicas = 56, 
                         restart_policy = '0', 
                         template = None, )
                     },
-                run_policy = V1RunPolicy(
+                run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                     active_deadline_seconds = 56, 
                     backoff_limit = 56, 
                     clean_pod_policy = '0', 
-                    scheduling_policy = V1SchedulingPolicy(
+                    scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                         min_available = 56, 
                         min_resources = {
                             'key' : None
                             }, 
                         priority_class = '0', 
                         queue = '0', 
                         schedule_timeout_seconds = 56, ), 
+                    suspend = True, 
                     ttl_seconds_after_finished = 56, ),
         )
 
     def testKubeflowOrgV1MXJobSpec(self):
         """Test KubeflowOrgV1MXJobSpec"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_paddle_elastic_policy.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_paddle_elastic_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_paddle_job.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_paddle_job.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -44,46 +44,47 @@
                         max_replicas = 56, 
                         max_restarts = 56, 
                         metrics = [
                             None
                             ], 
                         min_replicas = 56, ), 
                     paddle_replica_specs = {
-                        'key' : V1ReplicaSpec(
+                        'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
                             replicas = 56, 
                             restart_policy = '0', 
                             template = None, )
                         }, 
-                    run_policy = V1RunPolicy(
+                    run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                         active_deadline_seconds = 56, 
                         backoff_limit = 56, 
                         clean_pod_policy = '0', 
-                        scheduling_policy = V1SchedulingPolicy(
+                        scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                             min_available = 56, 
                             min_resources = {
                                 'key' : None
                                 }, 
                             priority_class = '0', 
                             queue = '0', 
                             schedule_timeout_seconds = 56, ), 
+                        suspend = True, 
                         ttl_seconds_after_finished = 56, ), ), 
-                status = V1JobStatus(
+                status = kubeflow_org_v1_job_status.KubeflowOrgV1JobStatus(
                     completion_time = None, 
                     conditions = [
-                        V1JobCondition(
+                        kubeflow_org_v1_job_condition.KubeflowOrgV1JobCondition(
                             last_transition_time = None, 
                             last_update_time = None, 
                             message = '0', 
                             reason = '0', 
                             status = '0', 
                             type = '0', )
                         ], 
                     last_reconcile_time = None, 
                     replica_statuses = {
-                        'key' : V1ReplicaStatus(
+                        'key' : kubeflow_org_v1_replica_status.KubeflowOrgV1ReplicaStatus(
                             active = 56, 
                             failed = 56, 
                             label_selector = None, 
                             selector = '0', 
                             succeeded = 56, )
                         }, 
                     start_time = None, )
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_paddle_job_list.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_mpi_job_list.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,162 +1,156 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 from kubeflow.training.models import *
-from kubeflow.training.models.kubeflow_org_v1_paddle_job_list import KubeflowOrgV1PaddleJobList  # noqa: E501
+from kubeflow.training.models.kubeflow_org_v1_mpi_job_list import KubeflowOrgV1MPIJobList  # noqa: E501
 from kubeflow.training.rest import ApiException
 
-class TestKubeflowOrgV1PaddleJobList(unittest.TestCase):
-    """KubeflowOrgV1PaddleJobList unit test stubs"""
+class TestKubeflowOrgV1MPIJobList(unittest.TestCase):
+    """KubeflowOrgV1MPIJobList unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test KubeflowOrgV1PaddleJobList
+        """Test KubeflowOrgV1MPIJobList
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kubeflow.training.models.kubeflow_org_v1_paddle_job_list.KubeflowOrgV1PaddleJobList()  # noqa: E501
+        # model = kubeflow.training.models.kubeflow_org_v1_mpi_job_list.KubeflowOrgV1MPIJobList()  # noqa: E501
         if include_optional :
-            return KubeflowOrgV1PaddleJobList(
+            return KubeflowOrgV1MPIJobList(
                 api_version = '0', 
                 items = [
-                    kubeflow_org_v1_paddle_job.KubeflowOrgV1PaddleJob(
+                    kubeflow_org_v1_mpi_job.KubeflowOrgV1MPIJob(
                         api_version = '0', 
                         kind = '0', 
                         metadata = None, 
-                        spec = kubeflow_org_v1_paddle_job_spec.KubeflowOrgV1PaddleJobSpec(
-                            elastic_policy = kubeflow_org_v1_paddle_elastic_policy.KubeflowOrgV1PaddleElasticPolicy(
-                                max_replicas = 56, 
-                                max_restarts = 56, 
-                                metrics = [
-                                    None
-                                    ], 
-                                min_replicas = 56, ), 
-                            paddle_replica_specs = {
-                                'key' : V1ReplicaSpec(
+                        spec = kubeflow_org_v1_mpi_job_spec.KubeflowOrgV1MPIJobSpec(
+                            clean_pod_policy = '0', 
+                            main_container = '0', 
+                            mpi_replica_specs = {
+                                'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
                                     replicas = 56, 
                                     restart_policy = '0', 
                                     template = None, )
                                 }, 
-                            run_policy = V1RunPolicy(
+                            run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                                 active_deadline_seconds = 56, 
                                 backoff_limit = 56, 
                                 clean_pod_policy = '0', 
-                                scheduling_policy = V1SchedulingPolicy(
+                                scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                                     min_available = 56, 
                                     min_resources = {
                                         'key' : None
                                         }, 
                                     priority_class = '0', 
                                     queue = '0', 
                                     schedule_timeout_seconds = 56, ), 
-                                ttl_seconds_after_finished = 56, ), ), 
-                        status = V1JobStatus(
+                                suspend = True, 
+                                ttl_seconds_after_finished = 56, ), 
+                            slots_per_worker = 56, ), 
+                        status = kubeflow_org_v1_job_status.KubeflowOrgV1JobStatus(
                             completion_time = None, 
                             conditions = [
-                                V1JobCondition(
+                                kubeflow_org_v1_job_condition.KubeflowOrgV1JobCondition(
                                     last_transition_time = None, 
                                     last_update_time = None, 
                                     message = '0', 
                                     reason = '0', 
                                     status = '0', 
                                     type = '0', )
                                 ], 
                             last_reconcile_time = None, 
                             replica_statuses = {
-                                'key' : V1ReplicaStatus(
+                                'key' : kubeflow_org_v1_replica_status.KubeflowOrgV1ReplicaStatus(
                                     active = 56, 
                                     failed = 56, 
                                     label_selector = None, 
                                     selector = '0', 
                                     succeeded = 56, )
                                 }, 
                             start_time = None, ), )
                     ], 
                 kind = '0', 
                 metadata = None
             )
         else :
-            return KubeflowOrgV1PaddleJobList(
+            return KubeflowOrgV1MPIJobList(
                 items = [
-                    kubeflow_org_v1_paddle_job.KubeflowOrgV1PaddleJob(
+                    kubeflow_org_v1_mpi_job.KubeflowOrgV1MPIJob(
                         api_version = '0', 
                         kind = '0', 
                         metadata = None, 
-                        spec = kubeflow_org_v1_paddle_job_spec.KubeflowOrgV1PaddleJobSpec(
-                            elastic_policy = kubeflow_org_v1_paddle_elastic_policy.KubeflowOrgV1PaddleElasticPolicy(
-                                max_replicas = 56, 
-                                max_restarts = 56, 
-                                metrics = [
-                                    None
-                                    ], 
-                                min_replicas = 56, ), 
-                            paddle_replica_specs = {
-                                'key' : V1ReplicaSpec(
+                        spec = kubeflow_org_v1_mpi_job_spec.KubeflowOrgV1MPIJobSpec(
+                            clean_pod_policy = '0', 
+                            main_container = '0', 
+                            mpi_replica_specs = {
+                                'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
                                     replicas = 56, 
                                     restart_policy = '0', 
                                     template = None, )
                                 }, 
-                            run_policy = V1RunPolicy(
+                            run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                                 active_deadline_seconds = 56, 
                                 backoff_limit = 56, 
                                 clean_pod_policy = '0', 
-                                scheduling_policy = V1SchedulingPolicy(
+                                scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                                     min_available = 56, 
                                     min_resources = {
                                         'key' : None
                                         }, 
                                     priority_class = '0', 
                                     queue = '0', 
                                     schedule_timeout_seconds = 56, ), 
-                                ttl_seconds_after_finished = 56, ), ), 
-                        status = V1JobStatus(
+                                suspend = True, 
+                                ttl_seconds_after_finished = 56, ), 
+                            slots_per_worker = 56, ), 
+                        status = kubeflow_org_v1_job_status.KubeflowOrgV1JobStatus(
                             completion_time = None, 
                             conditions = [
-                                V1JobCondition(
+                                kubeflow_org_v1_job_condition.KubeflowOrgV1JobCondition(
                                     last_transition_time = None, 
                                     last_update_time = None, 
                                     message = '0', 
                                     reason = '0', 
                                     status = '0', 
                                     type = '0', )
                                 ], 
                             last_reconcile_time = None, 
                             replica_statuses = {
-                                'key' : V1ReplicaStatus(
+                                'key' : kubeflow_org_v1_replica_status.KubeflowOrgV1ReplicaStatus(
                                     active = 56, 
                                     failed = 56, 
                                     label_selector = None, 
                                     selector = '0', 
                                     succeeded = 56, )
                                 }, 
                             start_time = None, ), )
                     ],
         )
 
-    def testKubeflowOrgV1PaddleJobList(self):
-        """Test KubeflowOrgV1PaddleJobList"""
+    def testKubeflowOrgV1MPIJobList(self):
+        """Test KubeflowOrgV1MPIJobList"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_paddle_job_spec.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_paddle_job_spec.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -40,53 +40,55 @@
                     max_replicas = 56, 
                     max_restarts = 56, 
                     metrics = [
                         None
                         ], 
                     min_replicas = 56, ), 
                 paddle_replica_specs = {
-                    'key' : V1ReplicaSpec(
+                    'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
                         replicas = 56, 
                         restart_policy = '0', 
                         template = None, )
                     }, 
-                run_policy = V1RunPolicy(
+                run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                     active_deadline_seconds = 56, 
                     backoff_limit = 56, 
                     clean_pod_policy = '0', 
-                    scheduling_policy = V1SchedulingPolicy(
+                    scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                         min_available = 56, 
                         min_resources = {
                             'key' : None
                             }, 
                         priority_class = '0', 
                         queue = '0', 
                         schedule_timeout_seconds = 56, ), 
+                    suspend = True, 
                     ttl_seconds_after_finished = 56, )
             )
         else :
             return KubeflowOrgV1PaddleJobSpec(
                 paddle_replica_specs = {
-                    'key' : V1ReplicaSpec(
+                    'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
                         replicas = 56, 
                         restart_policy = '0', 
                         template = None, )
                     },
-                run_policy = V1RunPolicy(
+                run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                     active_deadline_seconds = 56, 
                     backoff_limit = 56, 
                     clean_pod_policy = '0', 
-                    scheduling_policy = V1SchedulingPolicy(
+                    scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                         min_available = 56, 
                         min_resources = {
                             'key' : None
                             }, 
                         priority_class = '0', 
                         queue = '0', 
                         schedule_timeout_seconds = 56, ), 
+                    suspend = True, 
                     ttl_seconds_after_finished = 56, ),
         )
 
     def testKubeflowOrgV1PaddleJobSpec(self):
         """Test KubeflowOrgV1PaddleJobSpec"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_py_torch_job.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_py_torch_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -54,47 +54,49 @@
                                 key = '0', 
                                 value = '0', )
                             ], 
                         rdzv_host = '0', 
                         rdzv_id = '0', 
                         rdzv_port = 56, 
                         standalone = True, ), 
+                    nproc_per_node = '0', 
                     pytorch_replica_specs = {
-                        'key' : V1ReplicaSpec(
+                        'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
                             replicas = 56, 
                             restart_policy = '0', 
                             template = None, )
                         }, 
-                    run_policy = V1RunPolicy(
+                    run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                         active_deadline_seconds = 56, 
                         backoff_limit = 56, 
                         clean_pod_policy = '0', 
-                        scheduling_policy = V1SchedulingPolicy(
+                        scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                             min_available = 56, 
                             min_resources = {
                                 'key' : None
                                 }, 
                             priority_class = '0', 
                             queue = '0', 
                             schedule_timeout_seconds = 56, ), 
+                        suspend = True, 
                         ttl_seconds_after_finished = 56, ), ), 
-                status = V1JobStatus(
+                status = kubeflow_org_v1_job_status.KubeflowOrgV1JobStatus(
                     completion_time = None, 
                     conditions = [
-                        V1JobCondition(
+                        kubeflow_org_v1_job_condition.KubeflowOrgV1JobCondition(
                             last_transition_time = None, 
                             last_update_time = None, 
                             message = '0', 
                             reason = '0', 
                             status = '0', 
                             type = '0', )
                         ], 
                     last_reconcile_time = None, 
                     replica_statuses = {
-                        'key' : V1ReplicaStatus(
+                        'key' : kubeflow_org_v1_replica_status.KubeflowOrgV1ReplicaStatus(
                             active = 56, 
                             failed = 56, 
                             label_selector = None, 
                             selector = '0', 
                             succeeded = 56, )
                         }, 
                     start_time = None, )
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_py_torch_job_list.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_py_torch_job_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -57,47 +57,49 @@
                                         key = '0', 
                                         value = '0', )
                                     ], 
                                 rdzv_host = '0', 
                                 rdzv_id = '0', 
                                 rdzv_port = 56, 
                                 standalone = True, ), 
+                            nproc_per_node = '0', 
                             pytorch_replica_specs = {
-                                'key' : V1ReplicaSpec(
+                                'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
                                     replicas = 56, 
                                     restart_policy = '0', 
                                     template = None, )
                                 }, 
-                            run_policy = V1RunPolicy(
+                            run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                                 active_deadline_seconds = 56, 
                                 backoff_limit = 56, 
                                 clean_pod_policy = '0', 
-                                scheduling_policy = V1SchedulingPolicy(
+                                scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                                     min_available = 56, 
                                     min_resources = {
                                         'key' : None
                                         }, 
                                     priority_class = '0', 
                                     queue = '0', 
                                     schedule_timeout_seconds = 56, ), 
+                                suspend = True, 
                                 ttl_seconds_after_finished = 56, ), ), 
-                        status = V1JobStatus(
+                        status = kubeflow_org_v1_job_status.KubeflowOrgV1JobStatus(
                             completion_time = None, 
                             conditions = [
-                                V1JobCondition(
+                                kubeflow_org_v1_job_condition.KubeflowOrgV1JobCondition(
                                     last_transition_time = None, 
                                     last_update_time = None, 
                                     message = '0', 
                                     reason = '0', 
                                     status = '0', 
                                     type = '0', )
                                 ], 
                             last_reconcile_time = None, 
                             replica_statuses = {
-                                'key' : V1ReplicaStatus(
+                                'key' : kubeflow_org_v1_replica_status.KubeflowOrgV1ReplicaStatus(
                                     active = 56, 
                                     failed = 56, 
                                     label_selector = None, 
                                     selector = '0', 
                                     succeeded = 56, )
                                 }, 
                             start_time = None, ), )
@@ -127,47 +129,49 @@
                                         key = '0', 
                                         value = '0', )
                                     ], 
                                 rdzv_host = '0', 
                                 rdzv_id = '0', 
                                 rdzv_port = 56, 
                                 standalone = True, ), 
+                            nproc_per_node = '0', 
                             pytorch_replica_specs = {
-                                'key' : V1ReplicaSpec(
+                                'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
                                     replicas = 56, 
                                     restart_policy = '0', 
                                     template = None, )
                                 }, 
-                            run_policy = V1RunPolicy(
+                            run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                                 active_deadline_seconds = 56, 
                                 backoff_limit = 56, 
                                 clean_pod_policy = '0', 
-                                scheduling_policy = V1SchedulingPolicy(
+                                scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                                     min_available = 56, 
                                     min_resources = {
                                         'key' : None
                                         }, 
                                     priority_class = '0', 
                                     queue = '0', 
                                     schedule_timeout_seconds = 56, ), 
+                                suspend = True, 
                                 ttl_seconds_after_finished = 56, ), ), 
-                        status = V1JobStatus(
+                        status = kubeflow_org_v1_job_status.KubeflowOrgV1JobStatus(
                             completion_time = None, 
                             conditions = [
-                                V1JobCondition(
+                                kubeflow_org_v1_job_condition.KubeflowOrgV1JobCondition(
                                     last_transition_time = None, 
                                     last_update_time = None, 
                                     message = '0', 
                                     reason = '0', 
                                     status = '0', 
                                     type = '0', )
                                 ], 
                             last_reconcile_time = None, 
                             replica_statuses = {
-                                'key' : V1ReplicaStatus(
+                                'key' : kubeflow_org_v1_replica_status.KubeflowOrgV1ReplicaStatus(
                                     active = 56, 
                                     failed = 56, 
                                     label_selector = None, 
                                     selector = '0', 
                                     succeeded = 56, )
                                 }, 
                             start_time = None, ), )
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_py_torch_job_spec.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_py_torch_job_spec.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -50,54 +50,57 @@
                             key = '0', 
                             value = '0', )
                         ], 
                     rdzv_host = '0', 
                     rdzv_id = '0', 
                     rdzv_port = 56, 
                     standalone = True, ), 
+                nproc_per_node = '0', 
                 pytorch_replica_specs = {
-                    'key' : V1ReplicaSpec(
+                    'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
                         replicas = 56, 
                         restart_policy = '0', 
                         template = None, )
                     }, 
-                run_policy = V1RunPolicy(
+                run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                     active_deadline_seconds = 56, 
                     backoff_limit = 56, 
                     clean_pod_policy = '0', 
-                    scheduling_policy = V1SchedulingPolicy(
+                    scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                         min_available = 56, 
                         min_resources = {
                             'key' : None
                             }, 
                         priority_class = '0', 
                         queue = '0', 
                         schedule_timeout_seconds = 56, ), 
+                    suspend = True, 
                     ttl_seconds_after_finished = 56, )
             )
         else :
             return KubeflowOrgV1PyTorchJobSpec(
                 pytorch_replica_specs = {
-                    'key' : V1ReplicaSpec(
+                    'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
                         replicas = 56, 
                         restart_policy = '0', 
                         template = None, )
                     },
-                run_policy = V1RunPolicy(
+                run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                     active_deadline_seconds = 56, 
                     backoff_limit = 56, 
                     clean_pod_policy = '0', 
-                    scheduling_policy = V1SchedulingPolicy(
+                    scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                         min_available = 56, 
                         min_resources = {
                             'key' : None
                             }, 
                         priority_class = '0', 
                         queue = '0', 
                         schedule_timeout_seconds = 56, ), 
+                    suspend = True, 
                     ttl_seconds_after_finished = 56, ),
         )
 
     def testKubeflowOrgV1PyTorchJobSpec(self):
         """Test KubeflowOrgV1PyTorchJobSpec"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_rdzv_conf.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_rdzv_conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_tf_job.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_tf_job.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -37,48 +37,49 @@
         if include_optional :
             return KubeflowOrgV1TFJob(
                 api_version = '0', 
                 kind = '0', 
                 metadata = None, 
                 spec = kubeflow_org_v1_tf_job_spec.KubeflowOrgV1TFJobSpec(
                     enable_dynamic_worker = True, 
-                    run_policy = V1RunPolicy(
+                    run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                         active_deadline_seconds = 56, 
                         backoff_limit = 56, 
                         clean_pod_policy = '0', 
-                        scheduling_policy = V1SchedulingPolicy(
+                        scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                             min_available = 56, 
                             min_resources = {
                                 'key' : None
                                 }, 
                             priority_class = '0', 
                             queue = '0', 
                             schedule_timeout_seconds = 56, ), 
+                        suspend = True, 
                         ttl_seconds_after_finished = 56, ), 
                     success_policy = '0', 
                     tf_replica_specs = {
-                        'key' : V1ReplicaSpec(
+                        'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
                             replicas = 56, 
                             restart_policy = '0', 
                             template = None, )
                         }, ), 
-                status = V1JobStatus(
+                status = kubeflow_org_v1_job_status.KubeflowOrgV1JobStatus(
                     completion_time = None, 
                     conditions = [
-                        V1JobCondition(
+                        kubeflow_org_v1_job_condition.KubeflowOrgV1JobCondition(
                             last_transition_time = None, 
                             last_update_time = None, 
                             message = '0', 
                             reason = '0', 
                             status = '0', 
                             type = '0', )
                         ], 
                     last_reconcile_time = None, 
                     replica_statuses = {
-                        'key' : V1ReplicaStatus(
+                        'key' : kubeflow_org_v1_replica_status.KubeflowOrgV1ReplicaStatus(
                             active = 56, 
                             failed = 56, 
                             label_selector = None, 
                             selector = '0', 
                             succeeded = 56, )
                         }, 
                     start_time = None, )
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_tf_job_list.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_mx_job_list.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,152 +1,152 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 from kubeflow.training.models import *
-from kubeflow.training.models.kubeflow_org_v1_tf_job_list import KubeflowOrgV1TFJobList  # noqa: E501
+from kubeflow.training.models.kubeflow_org_v1_mx_job_list import KubeflowOrgV1MXJobList  # noqa: E501
 from kubeflow.training.rest import ApiException
 
-class TestKubeflowOrgV1TFJobList(unittest.TestCase):
-    """KubeflowOrgV1TFJobList unit test stubs"""
+class TestKubeflowOrgV1MXJobList(unittest.TestCase):
+    """KubeflowOrgV1MXJobList unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test KubeflowOrgV1TFJobList
+        """Test KubeflowOrgV1MXJobList
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kubeflow.training.models.kubeflow_org_v1_tf_job_list.KubeflowOrgV1TFJobList()  # noqa: E501
+        # model = kubeflow.training.models.kubeflow_org_v1_mx_job_list.KubeflowOrgV1MXJobList()  # noqa: E501
         if include_optional :
-            return KubeflowOrgV1TFJobList(
+            return KubeflowOrgV1MXJobList(
                 api_version = '0', 
                 items = [
-                    kubeflow_org_v1_tf_job.KubeflowOrgV1TFJob(
+                    kubeflow_org_v1_mx_job.KubeflowOrgV1MXJob(
                         api_version = '0', 
                         kind = '0', 
                         metadata = None, 
-                        spec = kubeflow_org_v1_tf_job_spec.KubeflowOrgV1TFJobSpec(
-                            enable_dynamic_worker = True, 
-                            run_policy = V1RunPolicy(
+                        spec = kubeflow_org_v1_mx_job_spec.KubeflowOrgV1MXJobSpec(
+                            job_mode = '0', 
+                            mx_replica_specs = {
+                                'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
+                                    replicas = 56, 
+                                    restart_policy = '0', 
+                                    template = None, )
+                                }, 
+                            run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                                 active_deadline_seconds = 56, 
                                 backoff_limit = 56, 
                                 clean_pod_policy = '0', 
-                                scheduling_policy = V1SchedulingPolicy(
+                                scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                                     min_available = 56, 
                                     min_resources = {
                                         'key' : None
                                         }, 
                                     priority_class = '0', 
                                     queue = '0', 
                                     schedule_timeout_seconds = 56, ), 
-                                ttl_seconds_after_finished = 56, ), 
-                            success_policy = '0', 
-                            tf_replica_specs = {
-                                'key' : V1ReplicaSpec(
-                                    replicas = 56, 
-                                    restart_policy = '0', 
-                                    template = None, )
-                                }, ), 
-                        status = V1JobStatus(
+                                suspend = True, 
+                                ttl_seconds_after_finished = 56, ), ), 
+                        status = kubeflow_org_v1_job_status.KubeflowOrgV1JobStatus(
                             completion_time = None, 
                             conditions = [
-                                V1JobCondition(
+                                kubeflow_org_v1_job_condition.KubeflowOrgV1JobCondition(
                                     last_transition_time = None, 
                                     last_update_time = None, 
                                     message = '0', 
                                     reason = '0', 
                                     status = '0', 
                                     type = '0', )
                                 ], 
                             last_reconcile_time = None, 
                             replica_statuses = {
-                                'key' : V1ReplicaStatus(
+                                'key' : kubeflow_org_v1_replica_status.KubeflowOrgV1ReplicaStatus(
                                     active = 56, 
                                     failed = 56, 
                                     label_selector = None, 
                                     selector = '0', 
                                     succeeded = 56, )
                                 }, 
                             start_time = None, ), )
                     ], 
                 kind = '0', 
                 metadata = None
             )
         else :
-            return KubeflowOrgV1TFJobList(
+            return KubeflowOrgV1MXJobList(
                 items = [
-                    kubeflow_org_v1_tf_job.KubeflowOrgV1TFJob(
+                    kubeflow_org_v1_mx_job.KubeflowOrgV1MXJob(
                         api_version = '0', 
                         kind = '0', 
                         metadata = None, 
-                        spec = kubeflow_org_v1_tf_job_spec.KubeflowOrgV1TFJobSpec(
-                            enable_dynamic_worker = True, 
-                            run_policy = V1RunPolicy(
+                        spec = kubeflow_org_v1_mx_job_spec.KubeflowOrgV1MXJobSpec(
+                            job_mode = '0', 
+                            mx_replica_specs = {
+                                'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
+                                    replicas = 56, 
+                                    restart_policy = '0', 
+                                    template = None, )
+                                }, 
+                            run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                                 active_deadline_seconds = 56, 
                                 backoff_limit = 56, 
                                 clean_pod_policy = '0', 
-                                scheduling_policy = V1SchedulingPolicy(
+                                scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                                     min_available = 56, 
                                     min_resources = {
                                         'key' : None
                                         }, 
                                     priority_class = '0', 
                                     queue = '0', 
                                     schedule_timeout_seconds = 56, ), 
-                                ttl_seconds_after_finished = 56, ), 
-                            success_policy = '0', 
-                            tf_replica_specs = {
-                                'key' : V1ReplicaSpec(
-                                    replicas = 56, 
-                                    restart_policy = '0', 
-                                    template = None, )
-                                }, ), 
-                        status = V1JobStatus(
+                                suspend = True, 
+                                ttl_seconds_after_finished = 56, ), ), 
+                        status = kubeflow_org_v1_job_status.KubeflowOrgV1JobStatus(
                             completion_time = None, 
                             conditions = [
-                                V1JobCondition(
+                                kubeflow_org_v1_job_condition.KubeflowOrgV1JobCondition(
                                     last_transition_time = None, 
                                     last_update_time = None, 
                                     message = '0', 
                                     reason = '0', 
                                     status = '0', 
                                     type = '0', )
                                 ], 
                             last_reconcile_time = None, 
                             replica_statuses = {
-                                'key' : V1ReplicaStatus(
+                                'key' : kubeflow_org_v1_replica_status.KubeflowOrgV1ReplicaStatus(
                                     active = 56, 
                                     failed = 56, 
                                     label_selector = None, 
                                     selector = '0', 
                                     succeeded = 56, )
                                 }, 
                             start_time = None, ), )
                     ],
         )
 
-    def testKubeflowOrgV1TFJobList(self):
-        """Test KubeflowOrgV1TFJobList"""
+    def testKubeflowOrgV1MXJobList(self):
+        """Test KubeflowOrgV1MXJobList"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_tf_job_spec.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_tf_job_spec.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -33,52 +33,54 @@
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = kubeflow.training.models.kubeflow_org_v1_tf_job_spec.KubeflowOrgV1TFJobSpec()  # noqa: E501
         if include_optional :
             return KubeflowOrgV1TFJobSpec(
                 enable_dynamic_worker = True, 
-                run_policy = V1RunPolicy(
+                run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                     active_deadline_seconds = 56, 
                     backoff_limit = 56, 
                     clean_pod_policy = '0', 
-                    scheduling_policy = V1SchedulingPolicy(
+                    scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                         min_available = 56, 
                         min_resources = {
                             'key' : None
                             }, 
                         priority_class = '0', 
                         queue = '0', 
                         schedule_timeout_seconds = 56, ), 
+                    suspend = True, 
                     ttl_seconds_after_finished = 56, ), 
                 success_policy = '0', 
                 tf_replica_specs = {
-                    'key' : V1ReplicaSpec(
+                    'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
                         replicas = 56, 
                         restart_policy = '0', 
                         template = None, )
                     }
             )
         else :
             return KubeflowOrgV1TFJobSpec(
-                run_policy = V1RunPolicy(
+                run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                     active_deadline_seconds = 56, 
                     backoff_limit = 56, 
                     clean_pod_policy = '0', 
-                    scheduling_policy = V1SchedulingPolicy(
+                    scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                         min_available = 56, 
                         min_resources = {
                             'key' : None
                             }, 
                         priority_class = '0', 
                         queue = '0', 
                         schedule_timeout_seconds = 56, ), 
+                    suspend = True, 
                     ttl_seconds_after_finished = 56, ),
                 tf_replica_specs = {
-                    'key' : V1ReplicaSpec(
+                    'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
                         replicas = 56, 
                         restart_policy = '0', 
                         template = None, )
                     },
         )
 
     def testKubeflowOrgV1TFJobSpec(self):
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_xg_boost_job.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_xg_boost_job.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -36,47 +36,48 @@
         # model = kubeflow.training.models.kubeflow_org_v1_xg_boost_job.KubeflowOrgV1XGBoostJob()  # noqa: E501
         if include_optional :
             return KubeflowOrgV1XGBoostJob(
                 api_version = '0', 
                 kind = '0', 
                 metadata = None, 
                 spec = kubeflow_org_v1_xg_boost_job_spec.KubeflowOrgV1XGBoostJobSpec(
-                    run_policy = V1RunPolicy(
+                    run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                         active_deadline_seconds = 56, 
                         backoff_limit = 56, 
                         clean_pod_policy = '0', 
-                        scheduling_policy = V1SchedulingPolicy(
+                        scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                             min_available = 56, 
                             min_resources = {
                                 'key' : None
                                 }, 
                             priority_class = '0', 
                             queue = '0', 
                             schedule_timeout_seconds = 56, ), 
+                        suspend = True, 
                         ttl_seconds_after_finished = 56, ), 
                     xgb_replica_specs = {
-                        'key' : V1ReplicaSpec(
+                        'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
                             replicas = 56, 
                             restart_policy = '0', 
                             template = None, )
                         }, ), 
-                status = V1JobStatus(
+                status = kubeflow_org_v1_job_status.KubeflowOrgV1JobStatus(
                     completion_time = None, 
                     conditions = [
-                        V1JobCondition(
+                        kubeflow_org_v1_job_condition.KubeflowOrgV1JobCondition(
                             last_transition_time = None, 
                             last_update_time = None, 
                             message = '0', 
                             reason = '0', 
                             status = '0', 
                             type = '0', )
                         ], 
                     last_reconcile_time = None, 
                     replica_statuses = {
-                        'key' : V1ReplicaStatus(
+                        'key' : kubeflow_org_v1_replica_status.KubeflowOrgV1ReplicaStatus(
                             active = 56, 
                             failed = 56, 
                             label_selector = None, 
                             selector = '0', 
                             succeeded = 56, )
                         }, 
                     start_time = None, )
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_kubeflow_org_v1_xg_boost_job_spec.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_xg_boost_job_spec.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
@@ -32,51 +32,53 @@
         """Test KubeflowOrgV1XGBoostJobSpec
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = kubeflow.training.models.kubeflow_org_v1_xg_boost_job_spec.KubeflowOrgV1XGBoostJobSpec()  # noqa: E501
         if include_optional :
             return KubeflowOrgV1XGBoostJobSpec(
-                run_policy = V1RunPolicy(
+                run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                     active_deadline_seconds = 56, 
                     backoff_limit = 56, 
                     clean_pod_policy = '0', 
-                    scheduling_policy = V1SchedulingPolicy(
+                    scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                         min_available = 56, 
                         min_resources = {
                             'key' : None
                             }, 
                         priority_class = '0', 
                         queue = '0', 
                         schedule_timeout_seconds = 56, ), 
+                    suspend = True, 
                     ttl_seconds_after_finished = 56, ), 
                 xgb_replica_specs = {
-                    'key' : V1ReplicaSpec(
+                    'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
                         replicas = 56, 
                         restart_policy = '0', 
                         template = None, )
                     }
             )
         else :
             return KubeflowOrgV1XGBoostJobSpec(
-                run_policy = V1RunPolicy(
+                run_policy = kubeflow_org_v1_run_policy.KubeflowOrgV1RunPolicy(
                     active_deadline_seconds = 56, 
                     backoff_limit = 56, 
                     clean_pod_policy = '0', 
-                    scheduling_policy = V1SchedulingPolicy(
+                    scheduling_policy = kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy(
                         min_available = 56, 
                         min_resources = {
                             'key' : None
                             }, 
                         priority_class = '0', 
                         queue = '0', 
                         schedule_timeout_seconds = 56, ), 
+                    suspend = True, 
                     ttl_seconds_after_finished = 56, ),
                 xgb_replica_specs = {
-                    'key' : V1ReplicaSpec(
+                    'key' : kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec(
                         replicas = 56, 
                         restart_policy = '0', 
                         template = None, )
                     },
         )
 
     def testKubeflowOrgV1XGBoostJobSpec(self):
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_v1_job_condition.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_job_condition.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 from kubeflow.training.models import *
-from kubeflow.training.models.v1_job_condition import V1JobCondition  # noqa: E501
+from kubeflow.training.models.kubeflow_org_v1_job_condition import KubeflowOrgV1JobCondition  # noqa: E501
 from kubeflow.training.rest import ApiException
 
-class TestV1JobCondition(unittest.TestCase):
-    """V1JobCondition unit test stubs"""
+class TestKubeflowOrgV1JobCondition(unittest.TestCase):
+    """KubeflowOrgV1JobCondition unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1JobCondition
+        """Test KubeflowOrgV1JobCondition
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kubeflow.training.models.v1_job_condition.V1JobCondition()  # noqa: E501
+        # model = kubeflow.training.models.kubeflow_org_v1_job_condition.KubeflowOrgV1JobCondition()  # noqa: E501
         if include_optional :
-            return V1JobCondition(
+            return KubeflowOrgV1JobCondition(
                 last_transition_time = None, 
                 last_update_time = None, 
                 message = '0', 
                 reason = '0', 
                 status = '0', 
                 type = '0'
             )
         else :
-            return V1JobCondition(
+            return KubeflowOrgV1JobCondition(
                 status = '0',
                 type = '0',
         )
 
-    def testV1JobCondition(self):
-        """Test V1JobCondition"""
+    def testKubeflowOrgV1JobCondition(self):
+        """Test KubeflowOrgV1JobCondition"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_v1_job_status.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_job_status.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,88 +1,71 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 from kubeflow.training.models import *
-from kubeflow.training.models.v1_job_status import V1JobStatus  # noqa: E501
+from kubeflow.training.models.kubeflow_org_v1_job_status import KubeflowOrgV1JobStatus  # noqa: E501
 from kubeflow.training.rest import ApiException
 
-class TestV1JobStatus(unittest.TestCase):
-    """V1JobStatus unit test stubs"""
+class TestKubeflowOrgV1JobStatus(unittest.TestCase):
+    """KubeflowOrgV1JobStatus unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1JobStatus
+        """Test KubeflowOrgV1JobStatus
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kubeflow.training.models.v1_job_status.V1JobStatus()  # noqa: E501
+        # model = kubeflow.training.models.kubeflow_org_v1_job_status.KubeflowOrgV1JobStatus()  # noqa: E501
         if include_optional :
-            return V1JobStatus(
+            return KubeflowOrgV1JobStatus(
                 completion_time = None, 
                 conditions = [
-                    V1JobCondition(
+                    kubeflow_org_v1_job_condition.KubeflowOrgV1JobCondition(
                         last_transition_time = None, 
                         last_update_time = None, 
                         message = '0', 
                         reason = '0', 
                         status = '0', 
                         type = '0', )
                     ], 
                 last_reconcile_time = None, 
                 replica_statuses = {
-                    'key' : V1ReplicaStatus(
+                    'key' : kubeflow_org_v1_replica_status.KubeflowOrgV1ReplicaStatus(
                         active = 56, 
                         failed = 56, 
                         label_selector = None, 
                         selector = '0', 
                         succeeded = 56, )
                     }, 
                 start_time = None
             )
         else :
-            return V1JobStatus(
-                conditions = [
-                    V1JobCondition(
-                        last_transition_time = None, 
-                        last_update_time = None, 
-                        message = '0', 
-                        reason = '0', 
-                        status = '0', 
-                        type = '0', )
-                    ],
-                replica_statuses = {
-                    'key' : V1ReplicaStatus(
-                        active = 56, 
-                        failed = 56, 
-                        label_selector = None, 
-                        selector = '0', 
-                        succeeded = 56, )
-                    },
+            return KubeflowOrgV1JobStatus(
         )
 
-    def testV1JobStatus(self):
-        """Test V1JobStatus"""
+    def testKubeflowOrgV1JobStatus(self):
+        """Test KubeflowOrgV1JobStatus"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_v1_replica_spec.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_replica_spec.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 from kubeflow.training.models import *
-from kubeflow.training.models.v1_replica_spec import V1ReplicaSpec  # noqa: E501
+from kubeflow.training.models.kubeflow_org_v1_replica_spec import KubeflowOrgV1ReplicaSpec  # noqa: E501
 from kubeflow.training.rest import ApiException
 
-class TestV1ReplicaSpec(unittest.TestCase):
-    """V1ReplicaSpec unit test stubs"""
+class TestKubeflowOrgV1ReplicaSpec(unittest.TestCase):
+    """KubeflowOrgV1ReplicaSpec unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1ReplicaSpec
+        """Test KubeflowOrgV1ReplicaSpec
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kubeflow.training.models.v1_replica_spec.V1ReplicaSpec()  # noqa: E501
+        # model = kubeflow.training.models.kubeflow_org_v1_replica_spec.KubeflowOrgV1ReplicaSpec()  # noqa: E501
         if include_optional :
-            return V1ReplicaSpec(
+            return KubeflowOrgV1ReplicaSpec(
                 replicas = 56, 
                 restart_policy = '0', 
                 template = None
             )
         else :
-            return V1ReplicaSpec(
+            return KubeflowOrgV1ReplicaSpec(
         )
 
-    def testV1ReplicaSpec(self):
-        """Test V1ReplicaSpec"""
+    def testKubeflowOrgV1ReplicaSpec(self):
+        """Test KubeflowOrgV1ReplicaSpec"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_v1_replica_status.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_replica_status.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 from kubeflow.training.models import *
-from kubeflow.training.models.v1_replica_status import V1ReplicaStatus  # noqa: E501
+from kubeflow.training.models.kubeflow_org_v1_replica_status import KubeflowOrgV1ReplicaStatus  # noqa: E501
 from kubeflow.training.rest import ApiException
 
-class TestV1ReplicaStatus(unittest.TestCase):
-    """V1ReplicaStatus unit test stubs"""
+class TestKubeflowOrgV1ReplicaStatus(unittest.TestCase):
+    """KubeflowOrgV1ReplicaStatus unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1ReplicaStatus
+        """Test KubeflowOrgV1ReplicaStatus
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kubeflow.training.models.v1_replica_status.V1ReplicaStatus()  # noqa: E501
+        # model = kubeflow.training.models.kubeflow_org_v1_replica_status.KubeflowOrgV1ReplicaStatus()  # noqa: E501
         if include_optional :
-            return V1ReplicaStatus(
+            return KubeflowOrgV1ReplicaStatus(
                 active = 56, 
                 failed = 56, 
                 label_selector = None, 
                 selector = '0', 
                 succeeded = 56
             )
         else :
-            return V1ReplicaStatus(
+            return KubeflowOrgV1ReplicaStatus(
         )
 
-    def testV1ReplicaStatus(self):
-        """Test V1ReplicaStatus"""
+    def testKubeflowOrgV1ReplicaStatus(self):
+        """Test KubeflowOrgV1ReplicaStatus"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kubeflow-training-1.6.0rc0/test/test_v1_run_policy.py` & `kubeflow-training-1.7.0rc0/test/test_kubeflow_org_v1_scheduling_policy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,58 @@
 # coding: utf-8
 
 """
     Kubeflow Training SDK
 
     Python SDK for Kubeflow Training  # noqa: E501
 
-    The version of the OpenAPI document: v1.6.0rc0
+    The version of the OpenAPI document: v1.7.0rc0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 from kubeflow.training.models import *
-from kubeflow.training.models.v1_run_policy import V1RunPolicy  # noqa: E501
+from kubeflow.training.models.kubeflow_org_v1_scheduling_policy import KubeflowOrgV1SchedulingPolicy  # noqa: E501
 from kubeflow.training.rest import ApiException
 
-class TestV1RunPolicy(unittest.TestCase):
-    """V1RunPolicy unit test stubs"""
+class TestKubeflowOrgV1SchedulingPolicy(unittest.TestCase):
+    """KubeflowOrgV1SchedulingPolicy unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test V1RunPolicy
+        """Test KubeflowOrgV1SchedulingPolicy
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = kubeflow.training.models.v1_run_policy.V1RunPolicy()  # noqa: E501
+        # model = kubeflow.training.models.kubeflow_org_v1_scheduling_policy.KubeflowOrgV1SchedulingPolicy()  # noqa: E501
         if include_optional :
-            return V1RunPolicy(
-                active_deadline_seconds = 56, 
-                backoff_limit = 56, 
-                clean_pod_policy = '0', 
-                scheduling_policy = V1SchedulingPolicy(
-                    min_available = 56, 
-                    min_resources = {
-                        'key' : None
-                        }, 
-                    priority_class = '0', 
-                    queue = '0', 
-                    schedule_timeout_seconds = 56, ), 
-                ttl_seconds_after_finished = 56
+            return KubeflowOrgV1SchedulingPolicy(
+                min_available = 56, 
+                min_resources = {
+                    'key' : None
+                    }, 
+                priority_class = '0', 
+                queue = '0', 
+                schedule_timeout_seconds = 56
             )
         else :
-            return V1RunPolicy(
+            return KubeflowOrgV1SchedulingPolicy(
         )
 
-    def testV1RunPolicy(self):
-        """Test V1RunPolicy"""
+    def testKubeflowOrgV1SchedulingPolicy(self):
+        """Test KubeflowOrgV1SchedulingPolicy"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

