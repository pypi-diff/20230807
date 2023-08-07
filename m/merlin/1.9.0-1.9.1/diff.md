# Comparing `tmp/merlin-1.9.0.tar.gz` & `tmp/merlin-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merlin-1.9.0.tar", last modified: Thu Dec 15 22:11:03 2022, max compression
+gzip compressed data, was "merlin-1.9.1.tar", last modified: Wed Dec 21 23:04:13 2022, max compression
```

## Comparing `merlin-1.9.0.tar` & `merlin-1.9.1.tar`

### file list

```diff
@@ -1,225 +1,227 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.047820 merlin-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2022-12-15 22:10:50.000000 merlin-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      220 2022-12-15 22:10:50.000000 merlin-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2022-12-15 22:11:03.047820 merlin-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2022-12-15 22:10:50.000000 merlin-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.015820 merlin-1.9.0/merlin/
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/ascii_art.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/celery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.019820 merlin-1.9.0/merlin/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.019820 merlin-1.9.0/merlin/common/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/common/abstracts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.019820 merlin-1.9.0/merlin/common/abstracts/enums/
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/common/abstracts/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/common/openfilelist.py
--rw-r--r--   0 runner    (1001) docker     (123)    12153 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/common/opennpylib.py
--rw-r--r--   0 runner    (1001) docker     (123)    12407 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/common/sample_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     7104 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/common/sample_index_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.019820 merlin-1.9.0/merlin/common/security/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/common/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/common/security/encrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/common/security/encrypt_backend_traffic.py
--rw-r--r--   0 runner    (1001) docker     (123)    23103 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/common/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/common/util_sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.019820 merlin-1.9.0/merlin/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/config/broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/config/celeryconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    10334 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/config/configfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/config/results_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.011820 merlin-1.9.0/merlin/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.019820 merlin-1.9.0/merlin/data/celery/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/data/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/data/celery/app.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/data/celery/app_redis.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/data/celery/app_test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.019820 merlin-1.9.0/merlin/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.023820 merlin-1.9.0/merlin/examples/dev_workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/dev_workflows/bad_format1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      397 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/dev_workflows/bad_format10.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      432 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/dev_workflows/bad_format11.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      247 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/dev_workflows/bad_format2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      250 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/dev_workflows/bad_format3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      518 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/dev_workflows/bad_format4.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      522 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/dev_workflows/bad_format5.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      526 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/dev_workflows/bad_format6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      522 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/dev_workflows/bad_format7.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      519 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/dev_workflows/bad_format8.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      381 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/dev_workflows/bad_format9.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/dev_workflows/full_format.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      173 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/dev_workflows/minimum_format.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/dev_workflows/no_description.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/dev_workflows/no_steps.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/dev_workflows/no_study.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/dev_workflows/restart.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      978 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/dev_workflows/restart_shell.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9896 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.015820 merlin-1.9.0/merlin/examples/workflows/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.023820 merlin-1.9.0/merlin/examples/workflows/feature_demo/
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/feature_demo/feature_demo.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/feature_demo/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.023820 merlin-1.9.0/merlin/examples/workflows/feature_demo/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/feature_demo/scripts/features.json
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/feature_demo/scripts/hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/feature_demo/scripts/pgen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.023820 merlin-1.9.0/merlin/examples/workflows/flux/
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/flux/flux_local.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/flux/flux_par.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/flux/flux_par_restart.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/flux/flux_test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/flux/paper.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/flux/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.027820 merlin-1.9.0/merlin/examples/workflows/flux/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3034 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/flux/scripts/flux_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/flux/scripts/hello.c
--rw-r--r--   0 runner    (1001) docker     (123)      969 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/flux/scripts/hello_sleep.c
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/flux/scripts/make_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/flux/scripts/paper_workers.sbatch
--rw-r--r--   0 runner    (1001) docker     (123)      666 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/flux/scripts/test_workers.sbatch
--rw-r--r--   0 runner    (1001) docker     (123)      655 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/flux/scripts/workers.bsub
--rw-r--r--   0 runner    (1001) docker     (123)      652 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/flux/scripts/workers.sbatch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.027820 merlin-1.9.0/merlin/examples/workflows/hello/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/hello/hello.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      750 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/hello/hello_samples.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      638 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/hello/make_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/hello/my_hello.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/hello/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.031820 merlin-1.9.0/merlin/examples/workflows/hpc_demo/
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/hpc_demo/cumulative_sample_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/hpc_demo/faker_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/hpc_demo/hpc_demo.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/hpc_demo/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/hpc_demo/sample_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/hpc_demo/sample_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.031820 merlin-1.9.0/merlin/examples/workflows/iterative_demo/
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/iterative_demo/cumulative_sample_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/iterative_demo/faker_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/iterative_demo/iterative_demo.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/iterative_demo/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/iterative_demo/sample_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/iterative_demo/sample_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.031820 merlin-1.9.0/merlin/examples/workflows/lsf/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/lsf/lsf_par.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/lsf/lsf_par_srun.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.031820 merlin-1.9.0/merlin/examples/workflows/lsf/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/lsf/scripts/hello.c
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/lsf/scripts/make_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.031820 merlin-1.9.0/merlin/examples/workflows/null_spec/
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/null_spec/null_chain.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/null_spec/null_spec.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/null_spec/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.035820 merlin-1.9.0/merlin/examples/workflows/null_spec/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/null_spec/scripts/launch_chain_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/null_spec/scripts/launch_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/null_spec/scripts/make_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/null_spec/scripts/read_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/null_spec/scripts/read_output_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/null_spec/scripts/submit.sbatch
--rw-r--r--   0 runner    (1001) docker     (123)      812 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/null_spec/scripts/submit_chain.sbatch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.035820 merlin-1.9.0/merlin/examples/workflows/openfoam_wf/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/openfoam_wf/openfoam_wf.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/openfoam_wf/openfoam_wf_template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/openfoam_wf/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.035820 merlin-1.9.0/merlin/examples/workflows/openfoam_wf/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/openfoam_wf/scripts/blockMesh_template.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/openfoam_wf/scripts/combine_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/openfoam_wf/scripts/learn.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/openfoam_wf/scripts/make_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/openfoam_wf/scripts/mesh_param_script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.035820 merlin-1.9.0/merlin/examples/workflows/openfoam_wf_no_docker/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/openfoam_wf_no_docker/openfoam_wf_no_docker.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/openfoam_wf_no_docker/openfoam_wf_no_docker_template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/openfoam_wf_no_docker/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.035820 merlin-1.9.0/merlin/examples/workflows/openfoam_wf_no_docker/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/openfoam_wf_no_docker/scripts/blockMesh_template.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/openfoam_wf_no_docker/scripts/combine_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/openfoam_wf_no_docker/scripts/learn.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/openfoam_wf_no_docker/scripts/make_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/openfoam_wf_no_docker/scripts/mesh_param_script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.039820 merlin-1.9.0/merlin/examples/workflows/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/optimization/optimization_basic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/optimization/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.039820 merlin-1.9.0/merlin/examples/workflows/optimization/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      953 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/optimization/scripts/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/optimization/scripts/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/optimization/scripts/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/optimization/scripts/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/optimization/template_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/optimization/template_optimization.temp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.039820 merlin-1.9.0/merlin/examples/workflows/remote_feature_demo/
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/remote_feature_demo/remote_feature_demo.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/remote_feature_demo/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.039820 merlin-1.9.0/merlin/examples/workflows/remote_feature_demo/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/remote_feature_demo/scripts/features.json
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/remote_feature_demo/scripts/hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/remote_feature_demo/scripts/pgen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.039820 merlin-1.9.0/merlin/examples/workflows/restart/
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/restart/restart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.039820 merlin-1.9.0/merlin/examples/workflows/restart/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/restart/scripts/make_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.039820 merlin-1.9.0/merlin/examples/workflows/restart_delay/
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/restart_delay/restart_delay.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.039820 merlin-1.9.0/merlin/examples/workflows/restart_delay/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/restart_delay/scripts/make_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.039820 merlin-1.9.0/merlin/examples/workflows/simple_chain/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/simple_chain/simple_chain.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.043820 merlin-1.9.0/merlin/examples/workflows/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/slurm/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.043820 merlin-1.9.0/merlin/examples/workflows/slurm/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/slurm/scripts/hello.c
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/slurm/scripts/make_samples.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      569 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/slurm/scripts/test_workers.sbatch
--rwxr-xr-x   0 runner    (1001) docker     (123)      556 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/slurm/scripts/workers.sbatch
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/slurm/slurm_par.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/slurm/slurm_par_restart.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      960 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/examples/workflows/slurm/slurm_test.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.043820 merlin-1.9.0/merlin/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/log_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    30123 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/merlin_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     9239 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.043820 merlin-1.9.0/merlin/server/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/server/docker.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      988 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/server/merlin_server.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      222 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/server/podman.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11799 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/server/server_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    14069 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/server/server_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    21429 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/server/server_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/server/singularity.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.043820 merlin-1.9.0/merlin/spec/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/spec/all_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/spec/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     8731 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/spec/expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/spec/override.py
--rw-r--r--   0 runner    (1001) docker     (123)    21265 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/spec/specification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.047820 merlin-1.9.0/merlin/study/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/study/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/study/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    16367 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/study/celeryadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/study/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)    17863 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/study/script_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10464 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/study/step.py
--rw-r--r--   0 runner    (1001) docker     (123)    20836 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/study/study.py
--rw-r--r--   0 runner    (1001) docker     (123)    15171 2022-12-15 22:10:50.000000 merlin-1.9.0/merlin/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.019820 merlin-1.9.0/merlin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2022-12-15 22:11:02.000000 merlin-1.9.0/merlin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2022-12-15 22:11:03.000000 merlin-1.9.0/merlin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 22:11:02.000000 merlin-1.9.0/merlin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-15 22:11:02.000000 merlin-1.9.0/merlin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 22:11:02.000000 merlin-1.9.0/merlin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      301 2022-12-15 22:11:02.000000 merlin-1.9.0/merlin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-15 22:11:02.000000 merlin-1.9.0/merlin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 22:11:03.047820 merlin-1.9.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2022-12-15 22:10:50.000000 merlin-1.9.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      199 2022-12-15 22:10:50.000000 merlin-1.9.0/requirements/release.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-15 22:10:50.000000 merlin-1.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      550 2022-12-15 22:11:03.047820 merlin-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2022-12-15 22:10:50.000000 merlin-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.075223 merlin-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2022-12-21 23:04:03.000000 merlin-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2022-12-21 23:04:03.000000 merlin-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2022-12-21 23:04:13.075223 merlin-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2022-12-21 23:04:03.000000 merlin-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.059223 merlin-1.9.1/merlin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/ascii_art.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/celery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.059223 merlin-1.9.1/merlin/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.059223 merlin-1.9.1/merlin/common/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/common/abstracts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.059223 merlin-1.9.1/merlin/common/abstracts/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/common/abstracts/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/common/openfilelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12153 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/common/opennpylib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12407 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/common/sample_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/common/sample_index_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.059223 merlin-1.9.1/merlin/common/security/
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/common/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/common/security/encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/common/security/encrypt_backend_traffic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23103 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/common/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/common/util_sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.059223 merlin-1.9.1/merlin/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9229 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/config/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/config/celeryconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10334 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/config/configfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/config/results_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.055223 merlin-1.9.1/merlin/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.063223 merlin-1.9.1/merlin/data/celery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/data/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/data/celery/app.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/data/celery/app_redis.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/data/celery/app_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.063223 merlin-1.9.1/merlin/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.063223 merlin-1.9.1/merlin/examples/dev_workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/dev_workflows/bad_format1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/dev_workflows/bad_format10.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/dev_workflows/bad_format11.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/dev_workflows/bad_format2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/dev_workflows/bad_format3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/dev_workflows/bad_format4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/dev_workflows/bad_format5.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/dev_workflows/bad_format6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/dev_workflows/bad_format7.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/dev_workflows/bad_format8.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/dev_workflows/bad_format9.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/dev_workflows/full_format.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/dev_workflows/minimum_format.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/dev_workflows/no_description.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/dev_workflows/no_steps.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/dev_workflows/no_study.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/dev_workflows/restart.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/dev_workflows/restart_shell.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9896 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.055223 merlin-1.9.1/merlin/examples/workflows/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.063223 merlin-1.9.1/merlin/examples/workflows/feature_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/feature_demo/feature_demo.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/feature_demo/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.063223 merlin-1.9.1/merlin/examples/workflows/feature_demo/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/feature_demo/scripts/features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/feature_demo/scripts/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/feature_demo/scripts/pgen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.063223 merlin-1.9.1/merlin/examples/workflows/flux/
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/flux/flux_local.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/flux/flux_par.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/flux/flux_par_restart.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/flux/flux_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/flux/paper.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/flux/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.067223 merlin-1.9.1/merlin/examples/workflows/flux/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3034 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/flux/scripts/flux_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/flux/scripts/hello.c
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/flux/scripts/hello_sleep.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/flux/scripts/make_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/flux/scripts/paper_workers.sbatch
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/flux/scripts/test_workers.sbatch
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/flux/scripts/workers.bsub
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/flux/scripts/workers.sbatch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.067223 merlin-1.9.1/merlin/examples/workflows/hello/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/hello/hello.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/hello/hello_samples.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/hello/make_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/hello/my_hello.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/hello/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.067223 merlin-1.9.1/merlin/examples/workflows/hpc_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/hpc_demo/cumulative_sample_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/hpc_demo/faker_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/hpc_demo/hpc_demo.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/hpc_demo/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/hpc_demo/sample_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/hpc_demo/sample_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.067223 merlin-1.9.1/merlin/examples/workflows/iterative_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/iterative_demo/cumulative_sample_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/iterative_demo/faker_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/iterative_demo/iterative_demo.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/iterative_demo/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/iterative_demo/sample_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/iterative_demo/sample_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.067223 merlin-1.9.1/merlin/examples/workflows/lsf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/lsf/lsf_par.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/lsf/lsf_par_srun.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.067223 merlin-1.9.1/merlin/examples/workflows/lsf/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/lsf/scripts/hello.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/lsf/scripts/make_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.067223 merlin-1.9.1/merlin/examples/workflows/null_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/null_spec/null_chain.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/null_spec/null_spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/null_spec/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.067223 merlin-1.9.1/merlin/examples/workflows/null_spec/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/null_spec/scripts/launch_chain_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/null_spec/scripts/launch_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/null_spec/scripts/make_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/null_spec/scripts/read_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/null_spec/scripts/read_output_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/null_spec/scripts/submit.sbatch
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/null_spec/scripts/submit_chain.sbatch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.067223 merlin-1.9.1/merlin/examples/workflows/openfoam_wf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/openfoam_wf/openfoam_wf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/openfoam_wf/openfoam_wf_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/openfoam_wf/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.071223 merlin-1.9.1/merlin/examples/workflows/openfoam_wf/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/openfoam_wf/scripts/blockMesh_template.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/openfoam_wf/scripts/combine_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/openfoam_wf/scripts/learn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/openfoam_wf/scripts/make_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/openfoam_wf/scripts/mesh_param_script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.071223 merlin-1.9.1/merlin/examples/workflows/openfoam_wf_no_docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/openfoam_wf_no_docker/openfoam_wf_no_docker.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/openfoam_wf_no_docker/openfoam_wf_no_docker_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/openfoam_wf_no_docker/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.071223 merlin-1.9.1/merlin/examples/workflows/openfoam_wf_no_docker/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/openfoam_wf_no_docker/scripts/blockMesh_template.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/openfoam_wf_no_docker/scripts/combine_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/openfoam_wf_no_docker/scripts/learn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/openfoam_wf_no_docker/scripts/make_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/openfoam_wf_no_docker/scripts/mesh_param_script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.071223 merlin-1.9.1/merlin/examples/workflows/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/optimization/optimization_basic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/optimization/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.071223 merlin-1.9.1/merlin/examples/workflows/optimization/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/optimization/scripts/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/optimization/scripts/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/optimization/scripts/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/optimization/scripts/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/optimization/template_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/optimization/template_optimization.temp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.071223 merlin-1.9.1/merlin/examples/workflows/remote_feature_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/remote_feature_demo/remote_feature_demo.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/remote_feature_demo/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.071223 merlin-1.9.1/merlin/examples/workflows/remote_feature_demo/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/remote_feature_demo/scripts/features.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/remote_feature_demo/scripts/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/remote_feature_demo/scripts/pgen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.071223 merlin-1.9.1/merlin/examples/workflows/restart/
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/restart/restart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.071223 merlin-1.9.1/merlin/examples/workflows/restart/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/restart/scripts/make_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.071223 merlin-1.9.1/merlin/examples/workflows/restart_delay/
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/restart_delay/restart_delay.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.071223 merlin-1.9.1/merlin/examples/workflows/restart_delay/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/restart_delay/scripts/make_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.071223 merlin-1.9.1/merlin/examples/workflows/simple_chain/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/simple_chain/simple_chain.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.071223 merlin-1.9.1/merlin/examples/workflows/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/slurm/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.071223 merlin-1.9.1/merlin/examples/workflows/slurm/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/slurm/scripts/hello.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/slurm/scripts/make_samples.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      569 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/slurm/scripts/test_workers.sbatch
+-rwxr-xr-x   0 runner    (1001) docker     (123)      556 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/slurm/scripts/workers.sbatch
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/slurm/slurm_par.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/slurm/slurm_par_restart.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/examples/workflows/slurm/slurm_test.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.075223 merlin-1.9.1/merlin/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/log_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30123 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/merlin_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9239 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.075223 merlin-1.9.1/merlin/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/server/docker.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/server/merlin_server.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/server/podman.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/server/server_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14487 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/server/server_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21429 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/server/server_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/server/singularity.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.075223 merlin-1.9.1/merlin/spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/spec/all_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/spec/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8731 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/spec/expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/spec/merlinspec.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/spec/override.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21265 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/spec/specification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.075223 merlin-1.9.1/merlin/study/
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/study/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/study/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16367 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/study/celeryadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/study/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17863 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/study/script_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10464 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/study/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20836 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/study/study.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15165 2022-12-21 23:04:03.000000 merlin-1.9.1/merlin/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.059223 merlin-1.9.1/merlin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2022-12-21 23:04:13.000000 merlin-1.9.1/merlin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2022-12-21 23:04:13.000000 merlin-1.9.1/merlin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 23:04:13.000000 merlin-1.9.1/merlin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-21 23:04:13.000000 merlin-1.9.1/merlin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 23:04:12.000000 merlin-1.9.1/merlin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2022-12-21 23:04:13.000000 merlin-1.9.1/merlin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-21 23:04:13.000000 merlin-1.9.1/merlin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 23:04:13.075223 merlin-1.9.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2022-12-21 23:04:03.000000 merlin-1.9.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2022-12-21 23:04:03.000000 merlin-1.9.1/requirements/release.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-21 23:04:03.000000 merlin-1.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2022-12-21 23:04:13.075223 merlin-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2022-12-21 23:04:03.000000 merlin-1.9.1/setup.py
```

### Comparing `merlin-1.9.0/LICENSE` & `merlin-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/PKG-INFO` & `merlin-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin
-Version: 1.9.0
+Version: 1.9.1
 Summary: The building blocks of workflows!
 Home-page: https://github.com/LLNL/merlin
 Author: Merlin Dev team
 Author-email: merlin@llnl.gov
 License: MIT
 Keywords: machine learning workflow
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `merlin-1.9.0/README.md` & `merlin-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/__init__.py` & `merlin-1.9.1/merlin/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -34,15 +34,15 @@
 This module contains the source code for Merlin.
 """
 
 import os
 import sys
 
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
 VERSION = __version__
 PATH_TO_PROJ = os.path.join(os.path.dirname(__file__), "")
 
 CLI_MOD = "merlin.main"
 
 
 def is_using_cli():
```

### Comparing `merlin-1.9.0/merlin/ascii_art.py` & `merlin-1.9.1/merlin/ascii_art.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/celery.py` & `merlin-1.9.1/merlin/celery.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/common/__init__.py` & `merlin-1.9.1/merlin/server/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/common/abstracts/__init__.py` & `merlin-1.9.1/merlin/common/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/common/abstracts/enums/__init__.py` & `merlin-1.9.1/merlin/common/abstracts/enums/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/common/openfilelist.py` & `merlin-1.9.1/merlin/common/openfilelist.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/common/opennpylib.py` & `merlin-1.9.1/merlin/common/opennpylib.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/common/sample_index.py` & `merlin-1.9.1/merlin/common/sample_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/common/sample_index_factory.py` & `merlin-1.9.1/merlin/common/sample_index_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/common/security/__init__.py` & `merlin-1.9.1/merlin/common/abstracts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/common/security/encrypt.py` & `merlin-1.9.1/merlin/common/security/encrypt.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/common/security/encrypt_backend_traffic.py` & `merlin-1.9.1/merlin/common/security/encrypt_backend_traffic.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/common/tasks.py` & `merlin-1.9.1/merlin/common/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/common/util_sampling.py` & `merlin-1.9.1/merlin/common/util_sampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/config/__init__.py` & `merlin-1.9.1/merlin/config/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/config/broker.py` & `merlin-1.9.1/merlin/config/broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/config/celeryconfig.py` & `merlin-1.9.1/merlin/config/celeryconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/config/configfile.py` & `merlin-1.9.1/merlin/config/configfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/config/results_backend.py` & `merlin-1.9.1/merlin/config/results_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/config/utils.py` & `merlin-1.9.1/merlin/config/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/data/celery/__init__.py` & `merlin-1.9.1/merlin/common/security/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/data/celery/app.yaml` & `merlin-1.9.1/merlin/data/celery/app.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/data/celery/app_redis.yaml` & `merlin-1.9.1/merlin/data/celery/app_redis.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/data/celery/app_test.yaml` & `merlin-1.9.1/merlin/data/celery/app_test.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/display.py` & `merlin-1.9.1/merlin/display.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/examples/__init__.py` & `merlin-1.9.1/merlin/data/celery/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/examples/dev_workflows/bad_format4.yaml` & `merlin-1.9.1/merlin/examples/dev_workflows/bad_format4.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/dev_workflows/bad_format5.yaml` & `merlin-1.9.1/merlin/examples/dev_workflows/bad_format5.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/dev_workflows/bad_format6.yaml` & `merlin-1.9.1/merlin/examples/dev_workflows/bad_format6.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/dev_workflows/bad_format7.yaml` & `merlin-1.9.1/merlin/examples/dev_workflows/bad_format7.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/dev_workflows/bad_format8.yaml` & `merlin-1.9.1/merlin/examples/dev_workflows/bad_format8.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/dev_workflows/full_format.yaml` & `merlin-1.9.1/merlin/examples/dev_workflows/full_format.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/dev_workflows/restart.yaml` & `merlin-1.9.1/merlin/examples/dev_workflows/restart.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/dev_workflows/restart_shell.yaml` & `merlin-1.9.1/merlin/examples/dev_workflows/restart_shell.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/examples.py` & `merlin-1.9.1/merlin/examples/examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/examples/generator.py` & `merlin-1.9.1/merlin/examples/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/examples/workflows/feature_demo/feature_demo.yaml` & `merlin-1.9.1/merlin/examples/workflows/feature_demo/feature_demo.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/feature_demo/scripts/hello_world.py` & `merlin-1.9.1/merlin/examples/workflows/feature_demo/scripts/hello_world.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/flux/flux_local.yaml` & `merlin-1.9.1/merlin/examples/workflows/flux/flux_local.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/flux/flux_par.yaml` & `merlin-1.9.1/merlin/examples/workflows/flux/flux_par.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/flux/flux_par_restart.yaml` & `merlin-1.9.1/merlin/examples/workflows/flux/flux_par_restart.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/flux/flux_test.yaml` & `merlin-1.9.1/merlin/examples/workflows/flux/flux_test.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/flux/paper.yaml` & `merlin-1.9.1/merlin/examples/workflows/flux/paper.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/flux/scripts/flux_info.py` & `merlin-1.9.1/merlin/examples/workflows/flux/scripts/flux_info.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/flux/scripts/hello.c` & `merlin-1.9.1/merlin/examples/workflows/flux/scripts/hello.c`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/flux/scripts/hello_sleep.c` & `merlin-1.9.1/merlin/examples/workflows/flux/scripts/hello_sleep.c`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/flux/scripts/make_samples.py` & `merlin-1.9.1/merlin/examples/workflows/flux/scripts/make_samples.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/flux/scripts/paper_workers.sbatch` & `merlin-1.9.1/merlin/examples/workflows/flux/scripts/paper_workers.sbatch`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/flux/scripts/test_workers.sbatch` & `merlin-1.9.1/merlin/examples/workflows/flux/scripts/test_workers.sbatch`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/flux/scripts/workers.bsub` & `merlin-1.9.1/merlin/examples/workflows/flux/scripts/workers.bsub`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/flux/scripts/workers.sbatch` & `merlin-1.9.1/merlin/examples/workflows/flux/scripts/workers.sbatch`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/hello/hello.yaml` & `merlin-1.9.1/merlin/examples/workflows/hello/hello.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/hello/hello_samples.yaml` & `merlin-1.9.1/merlin/examples/workflows/hello/hello_samples.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/hello/make_samples.py` & `merlin-1.9.1/merlin/examples/workflows/hello/make_samples.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/hpc_demo/cumulative_sample_processor.py` & `merlin-1.9.1/merlin/examples/workflows/hpc_demo/cumulative_sample_processor.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/hpc_demo/faker_sample.py` & `merlin-1.9.1/merlin/examples/workflows/hpc_demo/faker_sample.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/hpc_demo/hpc_demo.yaml` & `merlin-1.9.1/merlin/examples/workflows/hpc_demo/hpc_demo.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/hpc_demo/sample_collector.py` & `merlin-1.9.1/merlin/examples/workflows/hpc_demo/sample_collector.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/hpc_demo/sample_processor.py` & `merlin-1.9.1/merlin/examples/workflows/hpc_demo/sample_processor.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/iterative_demo/cumulative_sample_processor.py` & `merlin-1.9.1/merlin/examples/workflows/iterative_demo/cumulative_sample_processor.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/iterative_demo/faker_sample.py` & `merlin-1.9.1/merlin/examples/workflows/iterative_demo/faker_sample.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/iterative_demo/iterative_demo.yaml` & `merlin-1.9.1/merlin/examples/workflows/iterative_demo/iterative_demo.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/iterative_demo/sample_collector.py` & `merlin-1.9.1/merlin/examples/workflows/iterative_demo/sample_collector.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/iterative_demo/sample_processor.py` & `merlin-1.9.1/merlin/examples/workflows/iterative_demo/sample_processor.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/lsf/lsf_par.yaml` & `merlin-1.9.1/merlin/examples/workflows/lsf/lsf_par.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/lsf/lsf_par_srun.yaml` & `merlin-1.9.1/merlin/examples/workflows/lsf/lsf_par_srun.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/lsf/scripts/hello.c` & `merlin-1.9.1/merlin/examples/workflows/lsf/scripts/hello.c`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/lsf/scripts/make_samples.py` & `merlin-1.9.1/merlin/examples/workflows/lsf/scripts/make_samples.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/null_spec/null_chain.yaml` & `merlin-1.9.1/merlin/examples/workflows/null_spec/null_chain.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/null_spec/null_spec.yaml` & `merlin-1.9.1/merlin/examples/workflows/null_spec/null_spec.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/null_spec/scripts/launch_chain_job.py` & `merlin-1.9.1/merlin/examples/workflows/null_spec/scripts/launch_chain_job.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/null_spec/scripts/launch_jobs.py` & `merlin-1.9.1/merlin/examples/workflows/null_spec/scripts/launch_jobs.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/null_spec/scripts/read_output.py` & `merlin-1.9.1/merlin/examples/workflows/null_spec/scripts/read_output.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/null_spec/scripts/read_output_chain.py` & `merlin-1.9.1/merlin/examples/workflows/null_spec/scripts/read_output_chain.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/null_spec/scripts/submit.sbatch` & `merlin-1.9.1/merlin/examples/workflows/null_spec/scripts/submit.sbatch`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/null_spec/scripts/submit_chain.sbatch` & `merlin-1.9.1/merlin/examples/workflows/null_spec/scripts/submit_chain.sbatch`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/openfoam_wf/openfoam_wf.yaml` & `merlin-1.9.1/merlin/examples/workflows/openfoam_wf/openfoam_wf.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/openfoam_wf/openfoam_wf_template.yaml` & `merlin-1.9.1/merlin/examples/workflows/openfoam_wf/openfoam_wf_template.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/openfoam_wf/scripts/blockMesh_template.txt` & `merlin-1.9.1/merlin/examples/workflows/openfoam_wf/scripts/blockMesh_template.txt`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/openfoam_wf/scripts/combine_outputs.py` & `merlin-1.9.1/merlin/examples/workflows/openfoam_wf/scripts/combine_outputs.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/openfoam_wf/scripts/learn.py` & `merlin-1.9.1/merlin/examples/workflows/openfoam_wf/scripts/learn.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/openfoam_wf/scripts/make_samples.py` & `merlin-1.9.1/merlin/examples/workflows/openfoam_wf/scripts/make_samples.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/openfoam_wf/scripts/mesh_param_script.py` & `merlin-1.9.1/merlin/examples/workflows/openfoam_wf/scripts/mesh_param_script.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/openfoam_wf_no_docker/openfoam_wf_no_docker.yaml` & `merlin-1.9.1/merlin/examples/workflows/openfoam_wf_no_docker/openfoam_wf_no_docker.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/openfoam_wf_no_docker/openfoam_wf_no_docker_template.yaml` & `merlin-1.9.1/merlin/examples/workflows/openfoam_wf_no_docker/openfoam_wf_no_docker_template.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/openfoam_wf_no_docker/scripts/blockMesh_template.txt` & `merlin-1.9.1/merlin/examples/workflows/openfoam_wf_no_docker/scripts/blockMesh_template.txt`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/openfoam_wf_no_docker/scripts/combine_outputs.py` & `merlin-1.9.1/merlin/examples/workflows/openfoam_wf_no_docker/scripts/combine_outputs.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/openfoam_wf_no_docker/scripts/learn.py` & `merlin-1.9.1/merlin/examples/workflows/openfoam_wf_no_docker/scripts/learn.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/openfoam_wf_no_docker/scripts/make_samples.py` & `merlin-1.9.1/merlin/examples/workflows/openfoam_wf_no_docker/scripts/make_samples.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/openfoam_wf_no_docker/scripts/mesh_param_script.py` & `merlin-1.9.1/merlin/examples/workflows/openfoam_wf_no_docker/scripts/mesh_param_script.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/optimization/optimization_basic.yaml` & `merlin-1.9.1/merlin/examples/workflows/optimization/optimization_basic.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/optimization/scripts/collector.py` & `merlin-1.9.1/merlin/examples/workflows/optimization/scripts/collector.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/optimization/scripts/optimizer.py` & `merlin-1.9.1/merlin/examples/workflows/optimization/scripts/optimizer.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/optimization/scripts/test_functions.py` & `merlin-1.9.1/merlin/examples/workflows/optimization/scripts/test_functions.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/optimization/scripts/visualizer.py` & `merlin-1.9.1/merlin/examples/workflows/optimization/scripts/visualizer.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/optimization/template_config.py` & `merlin-1.9.1/merlin/examples/workflows/optimization/template_config.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/optimization/template_optimization.temp` & `merlin-1.9.1/merlin/examples/workflows/optimization/template_optimization.temp`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/remote_feature_demo/remote_feature_demo.yaml` & `merlin-1.9.1/merlin/examples/workflows/remote_feature_demo/remote_feature_demo.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/remote_feature_demo/scripts/hello_world.py` & `merlin-1.9.1/merlin/examples/workflows/remote_feature_demo/scripts/hello_world.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/remote_feature_demo/scripts/pgen.py` & `merlin-1.9.1/merlin/examples/workflows/remote_feature_demo/scripts/pgen.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/restart/restart.yaml` & `merlin-1.9.1/merlin/examples/workflows/restart/restart.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/restart/scripts/make_samples.py` & `merlin-1.9.1/merlin/examples/workflows/restart/scripts/make_samples.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/restart_delay/restart_delay.yaml` & `merlin-1.9.1/merlin/examples/workflows/restart_delay/restart_delay.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/restart_delay/scripts/make_samples.py` & `merlin-1.9.1/merlin/examples/workflows/restart_delay/scripts/make_samples.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/simple_chain/simple_chain.yaml` & `merlin-1.9.1/merlin/examples/workflows/simple_chain/simple_chain.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/slurm/scripts/hello.c` & `merlin-1.9.1/merlin/examples/workflows/slurm/scripts/hello.c`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/slurm/scripts/make_samples.py` & `merlin-1.9.1/merlin/examples/workflows/slurm/scripts/make_samples.py`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/slurm/scripts/test_workers.sbatch` & `merlin-1.9.1/merlin/examples/workflows/slurm/scripts/test_workers.sbatch`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/slurm/scripts/workers.sbatch` & `merlin-1.9.1/merlin/examples/workflows/slurm/scripts/workers.sbatch`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/slurm/slurm_par.yaml` & `merlin-1.9.1/merlin/examples/workflows/slurm/slurm_par.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/slurm/slurm_par_restart.yaml` & `merlin-1.9.1/merlin/examples/workflows/slurm/slurm_par_restart.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/examples/workflows/slurm/slurm_test.yaml` & `merlin-1.9.1/merlin/examples/workflows/slurm/slurm_test.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/exceptions/__init__.py` & `merlin-1.9.1/merlin/exceptions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/log_formatter.py` & `merlin-1.9.1/merlin/log_formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/main.py` & `merlin-1.9.1/merlin/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/merlin_templates.py` & `merlin-1.9.1/merlin/merlin_templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/router.py` & `merlin-1.9.1/merlin/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/server/merlin_server.yaml` & `merlin-1.9.1/merlin/server/merlin_server.yaml`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/merlin/server/server_commands.py` & `merlin-1.9.1/merlin/server/server_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/server/server_config.py` & `merlin-1.9.1/merlin/server/server_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -28,22 +28,27 @@
 # SOFTWARE.
 ###############################################################################
 
 import enum
 import logging
 import os
 import random
-import shutil
 import string
 import subprocess
 from io import BufferedReader
 from typing import Tuple
 
 import yaml
 
+
+try:
+    import importlib.resources as resources
+except ImportError:
+    import importlib_resources as resources
+
 from merlin.server.server_util import (
     CONTAINER_TYPES,
     MERLIN_CONFIG_DIR,
     MERLIN_SERVER_CONFIG,
     MERLIN_SERVER_SUBDIR,
     AppYaml,
     RedisConfig,
@@ -154,26 +159,30 @@
     for file in files:
         file_path = os.path.join(config_dir, file)
         if os.path.exists(file_path):
             LOG.info(f"{file} already exists.")
             continue
         LOG.info(f"Copying file {file} to configuration directory.")
         try:
-            shutil.copy(os.path.join(os.path.dirname(os.path.abspath(__file__)), file), config_dir)
+            with resources.path("merlin.server", file) as config_file:
+                with open(file_path, "w") as outfile, open(config_file, "r") as infile:
+                    outfile.write(infile.read())
         except OSError:
             LOG.error(f"Destination location {config_dir} is not writable.")
             return False
 
     # Load Merlin Server Configuration and apply it to app.yaml
-    with open(os.path.join(os.path.dirname(os.path.abspath(__file__)), MERLIN_SERVER_CONFIG)) as f:
-        main_server_config = yaml.load(f, yaml.Loader)
-        filename = LOCAL_APP_YAML if os.path.exists(LOCAL_APP_YAML) else AppYaml.default_filename
-        merlin_app_yaml = AppYaml(filename)
-        merlin_app_yaml.update_data(main_server_config)
-        merlin_app_yaml.write(filename)
+    with resources.path("merlin.server", MERLIN_SERVER_CONFIG) as merlin_server_config:
+        with open(merlin_server_config) as f:
+            main_server_config = yaml.load(f, yaml.Loader)
+            filename = LOCAL_APP_YAML if os.path.exists(LOCAL_APP_YAML) else AppYaml.default_filename
+            merlin_app_yaml = AppYaml(filename)
+            merlin_app_yaml.update_data(main_server_config)
+            merlin_app_yaml.write(filename)
+    LOG.info("Applying merlin server configuration to app.yaml")
 
     server_config = pull_server_config()
     if not server_config:
         LOG.error('Try to run "merlin server init" again to reinitialize values.')
         return False
 
     if not os.path.exists(server_config.container.get_config_dir()):
@@ -297,16 +306,17 @@
         )
     else:
         LOG.info(f"{image_path} already exists.")
 
     if not os.path.exists(os.path.join(config_dir, config_file)):
         LOG.info("Copying default redis configuration file.")
         try:
-            file_dir = os.path.dirname(os.path.abspath(__file__))
-            shutil.copy(os.path.join(file_dir, config_file), config_dir)
+            with resources.path("merlin.server", config_file) as file:
+                with open(os.path.join(config_dir, config_file), "w") as outfile, open(file, "r") as infile:
+                    outfile.write(infile.read())
         except OSError:
             LOG.error(f"Destination location {config_dir} is not writable.")
             return False
     else:
         LOG.info("Redis configuration file already exist.")
 
     return True
```

### Comparing `merlin-1.9.0/merlin/server/server_util.py` & `merlin-1.9.1/merlin/server/server_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/spec/__init__.py` & `merlin-1.9.1/merlin/examples/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/spec/all_keys.py` & `merlin-1.9.1/merlin/spec/all_keys.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/spec/defaults.py` & `merlin-1.9.1/merlin/spec/defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/spec/expansion.py` & `merlin-1.9.1/merlin/spec/expansion.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/spec/override.py` & `merlin-1.9.1/merlin/spec/override.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/spec/specification.py` & `merlin-1.9.1/merlin/spec/specification.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/study/__init__.py` & `merlin-1.9.1/merlin/spec/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/study/batch.py` & `merlin-1.9.1/merlin/study/batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/study/celeryadapter.py` & `merlin-1.9.1/merlin/study/celeryadapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/study/dag.py` & `merlin-1.9.1/merlin/study/dag.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/study/script_adapter.py` & `merlin-1.9.1/merlin/study/script_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/study/step.py` & `merlin-1.9.1/merlin/study/step.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/study/study.py` & `merlin-1.9.1/merlin/study/study.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `merlin-1.9.0/merlin/utils.py` & `merlin-1.9.1/merlin/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -236,17 +236,17 @@
         if array.ndim < ndmin:
             LOG.error(
                 f"Array in {filename} has fewer than the required \
                        minimum dimensions ({array.ndim} < {ndmin})!"
             )
     # Make sure text files load as strings with minimum number of dimensions
     elif protocol == "csv":
-        array = np.loadtxt(filename, delimiter=",", ndmin=ndmin, dtype=np.str)
+        array = np.loadtxt(filename, delimiter=",", ndmin=ndmin, dtype=str)
     elif protocol == "tab":
-        array = np.loadtxt(filename, ndmin=ndmin, dtype=np.str)
+        array = np.loadtxt(filename, ndmin=ndmin, dtype=str)
     else:
         raise TypeError(
             f"{protocol} is not a valid array file extension.\
                          Choices: {ARRAY_FILE_FORMATS}"
         )
 
     return array
```

### Comparing `merlin-1.9.0/merlin.egg-info/PKG-INFO` & `merlin-1.9.1/merlin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin
-Version: 1.9.0
+Version: 1.9.1
 Summary: The building blocks of workflows!
 Home-page: https://github.com/LLNL/merlin
 Author: Merlin Dev team
 Author-email: merlin@llnl.gov
 License: MIT
 Keywords: machine learning workflow
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `merlin-1.9.0/merlin.egg-info/SOURCES.txt` & `merlin-1.9.1/merlin.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -152,25 +152,27 @@
 merlin/examples/workflows/slurm/slurm_par_restart.yaml
 merlin/examples/workflows/slurm/slurm_test.yaml
 merlin/examples/workflows/slurm/scripts/hello.c
 merlin/examples/workflows/slurm/scripts/make_samples.py
 merlin/examples/workflows/slurm/scripts/test_workers.sbatch
 merlin/examples/workflows/slurm/scripts/workers.sbatch
 merlin/exceptions/__init__.py
+merlin/server/__init__.py
 merlin/server/docker.yaml
 merlin/server/merlin_server.yaml
 merlin/server/podman.yaml
 merlin/server/server_commands.py
 merlin/server/server_config.py
 merlin/server/server_util.py
 merlin/server/singularity.yaml
 merlin/spec/__init__.py
 merlin/spec/all_keys.py
 merlin/spec/defaults.py
 merlin/spec/expansion.py
+merlin/spec/merlinspec.json
 merlin/spec/override.py
 merlin/spec/specification.py
 merlin/study/__init__.py
 merlin/study/batch.py
 merlin/study/celeryadapter.py
 merlin/study/dag.py
 merlin/study/script_adapter.py
```

### Comparing `merlin-1.9.0/setup.cfg` & `merlin-1.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `merlin-1.9.0/setup.py` & `merlin-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2022, Lawrence Livermore National Security, LLC.
 # Produced at the Lawrence Livermore National Laboratory
 # Written by the Merlin dev team, listed in the CONTRIBUTORS file.
 # <merlin@llnl.gov>
 #
 # LLNL-CODE-797170
 # All rights reserved.
-# This file is part of Merlin, Version: 1.9.0.
+# This file is part of Merlin, Version: 1.9.1.
 #
 # For details, see https://github.com/LLNL/merlin.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

