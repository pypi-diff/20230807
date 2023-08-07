# Comparing `tmp/ydata-synthetic-1.2.0.tar.gz` & `tmp/ydata-synthetic-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ydata-synthetic-1.2.0.tar", last modified: Wed May 24 06:53:51 2023, max compression
+gzip compressed data, was "ydata-synthetic-1.3.0.tar", last modified: Mon Aug  7 11:15:28 2023, max compression
```

## Comparing `ydata-synthetic-1.2.0.tar` & `ydata-synthetic-1.3.0.tar`

### file list

```diff
@@ -1,101 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.696075 ydata-synthetic-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9582 2023-05-24 06:53:51.696075 ydata-synthetic-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7127 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-24 06:53:50.000000 ydata-synthetic-1.2.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)      206 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-24 06:53:51.696075 ydata-synthetic-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2424 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.688075 ydata-synthetic-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.688075 ydata-synthetic-1.2.0/src/ydata_synthetic/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/evaluation/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/evaluation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.688075 ydata-synthetic-1.2.0/src/ydata_synthetic/postprocessing/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/postprocessing/regular/
--rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/postprocessing/regular/inverse_preprocesser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5464 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/base_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/regular/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/regular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8210 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/regular/ctgan_processor.py
--rw-r--r--   0 runner    (1001) docker     (122)     4519 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/regular/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/timeseries/
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      577 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/timeseries/stock.py
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/timeseries/timeseries_processor.py
--rw-r--r--   0 runner    (1001) docker     (122)     1166 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/timeseries/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/
--rw-r--r--   0 runner    (1001) docker     (122)     4196 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/About.py
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/
--rw-r--r--   0 runner    (1001) docker     (122)     5723 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/1_Train_a_synthesizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2947 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/2_Generate_synthetic_data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/functions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      789 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/functions/generate.py
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/functions/load_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1843 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/functions/train.py
--rw-r--r--   0 runner    (1001) docker     (122)      363 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/run.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12365 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2849 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/
--rw-r--r--   0 runner    (1001) docker     (122)      115 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/cgan/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/cgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8358 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/cgan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/cramergan/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/cramergan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8740 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/cramergan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/ctgan/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/ctgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14122 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/ctgan/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     5343 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/ctgan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/cwgangp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/cwgangp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8917 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/cwgangp/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/dragan/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/dragan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7846 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/dragan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/gmm/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/gmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3804 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/gmm/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/vanillagan/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/vanillagan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/vanillagan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/wgan/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/wgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8119 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/wgan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/wgangp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/wgangp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8396 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/wgangp/model.py
--rw-r--r--   0 runner    (1001) docker     (122)      802 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/saving_keras.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.692075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/timeseries/
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.696075 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/timeseries/timegan/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/timeseries/timegan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13792 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/timeseries/timegan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.688075 ydata-synthetic-1.2.0/src/ydata_synthetic/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.696075 ydata-synthetic-1.2.0/src/ydata_synthetic/tests/custom_layers/
--rw-r--r--   0 runner    (1001) docker     (122)     3315 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_activation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2714 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.696075 ydata-synthetic-1.2.0/src/ydata_synthetic/tests/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (122)     3368 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/tests/preprocessing/test_regular_data_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.696075 ydata-synthetic-1.2.0/src/ydata_synthetic/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2050 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     4346 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/utils/gumbel_softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.696075 ydata-synthetic-1.2.0/src/ydata_synthetic/utils/misc/
--rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-05-24 06:53:43.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/utils/misc/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-05-24 06:53:51.000000 ydata-synthetic-1.2.0/src/ydata_synthetic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 06:53:51.688075 ydata-synthetic-1.2.0/src/ydata_synthetic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9582 2023-05-24 06:53:51.000000 ydata-synthetic-1.2.0/src/ydata_synthetic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3406 2023-05-24 06:53:51.000000 ydata-synthetic-1.2.0/src/ydata_synthetic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 06:53:51.000000 ydata-synthetic-1.2.0/src/ydata_synthetic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-05-24 06:53:51.000000 ydata-synthetic-1.2.0/src/ydata_synthetic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-24 06:53:51.000000 ydata-synthetic-1.2.0/src/ydata_synthetic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.691187 ydata-synthetic-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10357 2023-08-07 11:15:28.691187 ydata-synthetic-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7830 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-08-07 11:15:27.000000 ydata-synthetic-1.3.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      205 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-07 11:15:28.691187 ydata-synthetic-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2424 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.679186 ydata-synthetic-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.683186 ydata-synthetic-1.3.0/src/ydata_synthetic/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.683186 ydata-synthetic-1.3.0/src/ydata_synthetic/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/evaluation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.679186 ydata-synthetic-1.3.0/src/ydata_synthetic/postprocessing/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.683186 ydata-synthetic-1.3.0/src/ydata_synthetic/postprocessing/regular/
+-rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/postprocessing/regular/inverse_preprocesser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.683186 ydata-synthetic-1.3.0/src/ydata_synthetic/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5464 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/preprocessing/base_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.683186 ydata-synthetic-1.3.0/src/ydata_synthetic/preprocessing/regular/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/preprocessing/regular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8210 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/preprocessing/regular/ctgan_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4526 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/preprocessing/regular/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.683186 ydata-synthetic-1.3.0/src/ydata_synthetic/preprocessing/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/preprocessing/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8977 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/preprocessing/timeseries/doppelganger_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      577 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/preprocessing/timeseries/stock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/preprocessing/timeseries/timeseries_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1166 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/preprocessing/timeseries/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.683186 ydata-synthetic-1.3.0/src/ydata_synthetic/streamlit_app/
+-rw-r--r--   0 runner    (1001) docker     (122)     4196 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/streamlit_app/About.py
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/streamlit_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.683186 ydata-synthetic-1.3.0/src/ydata_synthetic/streamlit_app/pages/
+-rw-r--r--   0 runner    (1001) docker     (122)     5723 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/streamlit_app/pages/1_Train_a_synthesizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2947 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/streamlit_app/pages/2_Generate_synthetic_data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.687186 ydata-synthetic-1.3.0/src/ydata_synthetic/streamlit_app/pages/functions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/streamlit_app/pages/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      789 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/streamlit_app/pages/functions/generate.py
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/streamlit_app/pages/functions/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1843 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/streamlit_app/pages/functions/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)      363 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/streamlit_app/run.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.687186 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12965 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2849 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.687186 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.687186 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/cgan/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/cgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9612 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/cgan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.687186 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/cramergan/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/cramergan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10646 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/cramergan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.687186 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/ctgan/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/ctgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14122 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/ctgan/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5343 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/ctgan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.687186 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/cwgangp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/cwgangp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10283 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/cwgangp/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.687186 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/dragan/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/dragan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10062 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/dragan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.687186 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/gmm/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/gmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3804 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/gmm/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.687186 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/vanillagan/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/vanillagan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8162 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/vanillagan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.687186 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/wgan/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/wgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9741 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/wgan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.687186 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/wgangp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/wgangp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10518 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/wgangp/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      802 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/saving_keras.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.687186 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.687186 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/timeseries/doppelganger/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/timeseries/doppelganger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26557 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/timeseries/doppelganger/doppelganger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8177 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/timeseries/doppelganger/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19125 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/timeseries/doppelganger/network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/timeseries/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.687186 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/timeseries/timegan/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/timeseries/timegan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15136 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/timeseries/timegan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.683186 ydata-synthetic-1.3.0/src/ydata_synthetic/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.691187 ydata-synthetic-1.3.0/src/ydata_synthetic/tests/custom_layers/
+-rw-r--r--   0 runner    (1001) docker     (122)     3315 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_activation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2714 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.691187 ydata-synthetic-1.3.0/src/ydata_synthetic/tests/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (122)     3368 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/tests/preprocessing/test_regular_data_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.691187 ydata-synthetic-1.3.0/src/ydata_synthetic/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2050 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4346 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/utils/gumbel_softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.691187 ydata-synthetic-1.3.0/src/ydata_synthetic/utils/misc/
+-rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-08-07 11:15:23.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/utils/misc/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-08-07 11:15:28.000000 ydata-synthetic-1.3.0/src/ydata_synthetic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 11:15:28.683186 ydata-synthetic-1.3.0/src/ydata_synthetic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10357 2023-08-07 11:15:28.000000 ydata-synthetic-1.3.0/src/ydata_synthetic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3828 2023-08-07 11:15:28.000000 ydata-synthetic-1.3.0/src/ydata_synthetic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-07 11:15:28.000000 ydata-synthetic-1.3.0/src/ydata_synthetic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      335 2023-08-07 11:15:28.000000 ydata-synthetic-1.3.0/src/ydata_synthetic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-08-07 11:15:28.000000 ydata-synthetic-1.3.0/src/ydata_synthetic.egg-info/top_level.txt
```

### Comparing `ydata-synthetic-1.2.0/LICENSE` & `ydata-synthetic-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/PKG-INFO` & `ydata-synthetic-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ydata-synthetic
-Version: 1.2.0
+Version: 1.3.0
 Summary: Synthetic data generation methods with different synthetization methods.
 Home-page: https://github.com/ydataai/ydata-synthetic
 Author: YData
 Author-email: community@ydata.ai
 License: https://github.com/ydataai/ydata-synthetic/blob/master/LICENSE
 Description: ![](https://img.shields.io/github/workflow/status/ydataai/ydata-synthetic/prerelease)
         ![](https://img.shields.io/pypi/status/ydata-synthetic)
         [![](https://pepy.tech/badge/ydata-synthetic)](https://pypi.org/project/ydata-synthetic/)
         ![](https://img.shields.io/badge/python-3.9%20%7C%203.10-blue)
         [![](https://img.shields.io/pypi/v/ydata-synthetic)](https://pypi.org/project/ydata-synthetic/)
         ![](https://img.shields.io/github/license/ydataai/ydata-synthetic)
         
-        <p align="center"><img width="200" src="https://user-images.githubusercontent.com/3348134/177604157-11181f6c-57e5-44b1-8f6c-774edbba5512.png" alt="Synthetic Data Logo"></p>
+        <p align="center"><img width="300" src="https://assets.ydata.ai/oss/ydata-synthetic_black.png" alt="YData Synthetic Logo"></p>
         
-        Join us on [![Discord](https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/mw7xjJ7b7s)
+        Join us on [![Discord](https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white)](https://tiny.ydata.ai/dcai-ydata-synthetic)
         
         # YData Synthetic
         A package to generate synthetic tabular and time-series data leveraging the state of the art generative models.
         
         ## 🎊 The exciting features:
         > These are must try features when it comes to synthetic data generation:
           > - A new streamlit app that delivers the synthetic data generation experience with a UI interface. A low code experience for the quick generation of synthetic data
@@ -33,14 +33,19 @@
         ### Why Synthetic Data?
         Synthetic data can be used for many applications:
           - Privacy compliance for data-sharing and Machine Learning development
           - Remove bias
           - Balance datasets
           - Augment datasets
         
+        > **Looking for an end-to-end solution to Synthetic Data Generation?**<br>
+        > [YData Fabric](https://ydata.ai/products/synthetic_data) enables the generation of high-quality datasets within a full UI experience, from data preparation to synthetic data generation and evaluation.<br>
+        > Check out the [Community Version](https://ydata.ai/ydata-fabric-free-trial).
+        
+        
         # ydata-synthetic
         This repository contains material related with architectures and models for synthetic data, from Generative Adversarial Networks (GANs) to Gaussian Mixtures.
         The repo includes a full ecosystem for synthetic data generation, that includes different models for the generation of synthetic structure data and time-series.
         All the Deep Learning models are implemented leveraging Tensorflow 2.0.
         Several example Jupyter Notebooks and Python scripts are included, to show how to use the different architectures.
         
         Are you ready to learn more about synthetic data and the bext-practices for synthetic data generation?
@@ -119,23 +124,27 @@
           - [Cramer GAN (The Cramer Distance as a Solution to Biased Wasserstein Gradients)](https://arxiv.org/abs/1705.10743)
           - [CWGAN-GP (Conditional Wassertein GAN with Gradient Penalty)](https://cameronfabbri.github.io/papers/conditionalWGAN.pdf)
           - [CTGAN (Conditional Tabular GAN)](https://arxiv.org/pdf/1907.00503.pdf)
           - [Gaussian Mixture](https://towardsdatascience.com/gaussian-mixture-models-explained-6986aaf5a95)
         
         ### Sequential data
           - [TimeGAN](https://papers.nips.cc/paper/2019/file/c9efe5f26cd17ba6216bbe2a7d26d490-Paper.pdf)
+          - [DoppelGANger](https://dl.acm.org/doi/pdf/10.1145/3419394.3423643)
         
         ## Contributing
         We are open to collaboration! If you want to start contributing you only need to:
           1. Search for an issue in which you would like to work. Issues for newcomers are labeled with good first issue.
           2. Create a PR solving the issue.
           3. We would review every PRs and either accept or ask for revisions.
         
         ## Support
-        For support in using this library, please join our Discord server. Our Discord community is very friendly and great about quickly answering questions about the use and development of the library. [Click here to join our Discord community!](https://discord.com/invite/mw7xjJ7b7s)
+        For support in using this library, please join our Discord server. Our Discord community is very friendly and great about quickly answering questions about the use and development of the library. [Click here to join our Discord community!](https://tiny.ydata.ai/dcai-ydata-synthetic)
+        
+        ## FAQs
+        Have a question? Check out the [Frequently Asked Questions](https://ydata.ai/resources/10-most-asked-questions-on-ydata-synthetic) about `ydata-synthetic`. If you feel something is missing, feel free to [book a beary informal chat with us](https://meetings.hubspot.com/fabiana-clemente).
         
         ## License
         [MIT License](https://github.com/ydataai/ydata-synthetic/blob/master/LICENSE)
         
 Keywords: data science ydata
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ydata-synthetic-1.2.0/README.md` & `ydata-synthetic-1.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ![](https://img.shields.io/github/workflow/status/ydataai/ydata-synthetic/prerelease)
 ![](https://img.shields.io/pypi/status/ydata-synthetic)
 [![](https://pepy.tech/badge/ydata-synthetic)](https://pypi.org/project/ydata-synthetic/)
 ![](https://img.shields.io/badge/python-3.9%20%7C%203.10-blue)
 [![](https://img.shields.io/pypi/v/ydata-synthetic)](https://pypi.org/project/ydata-synthetic/)
 ![](https://img.shields.io/github/license/ydataai/ydata-synthetic)
 
-<p align="center"><img width="200" src="https://user-images.githubusercontent.com/3348134/177604157-11181f6c-57e5-44b1-8f6c-774edbba5512.png" alt="Synthetic Data Logo"></p>
+<p align="center"><img width="300" src="https://assets.ydata.ai/oss/ydata-synthetic_black.png" alt="YData Synthetic Logo"></p>
 
-Join us on [![Discord](https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/mw7xjJ7b7s)
+Join us on [![Discord](https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white)](https://tiny.ydata.ai/dcai-ydata-synthetic)
 
 # YData Synthetic
 A package to generate synthetic tabular and time-series data leveraging the state of the art generative models.
 
 ## 🎊 The exciting features:
 > These are must try features when it comes to synthetic data generation:
   > - A new streamlit app that delivers the synthetic data generation experience with a UI interface. A low code experience for the quick generation of synthetic data
@@ -25,14 +25,19 @@
 ### Why Synthetic Data?
 Synthetic data can be used for many applications:
   - Privacy compliance for data-sharing and Machine Learning development
   - Remove bias
   - Balance datasets
   - Augment datasets
 
+> **Looking for an end-to-end solution to Synthetic Data Generation?**<br>
+> [YData Fabric](https://ydata.ai/products/synthetic_data) enables the generation of high-quality datasets within a full UI experience, from data preparation to synthetic data generation and evaluation.<br>
+> Check out the [Community Version](https://ydata.ai/ydata-fabric-free-trial).
+
+
 # ydata-synthetic
 This repository contains material related with architectures and models for synthetic data, from Generative Adversarial Networks (GANs) to Gaussian Mixtures.
 The repo includes a full ecosystem for synthetic data generation, that includes different models for the generation of synthetic structure data and time-series.
 All the Deep Learning models are implemented leveraging Tensorflow 2.0.
 Several example Jupyter Notebooks and Python scripts are included, to show how to use the different architectures.
 
 Are you ready to learn more about synthetic data and the bext-practices for synthetic data generation?
@@ -111,19 +116,23 @@
   - [Cramer GAN (The Cramer Distance as a Solution to Biased Wasserstein Gradients)](https://arxiv.org/abs/1705.10743)
   - [CWGAN-GP (Conditional Wassertein GAN with Gradient Penalty)](https://cameronfabbri.github.io/papers/conditionalWGAN.pdf)
   - [CTGAN (Conditional Tabular GAN)](https://arxiv.org/pdf/1907.00503.pdf)
   - [Gaussian Mixture](https://towardsdatascience.com/gaussian-mixture-models-explained-6986aaf5a95)
 
 ### Sequential data
   - [TimeGAN](https://papers.nips.cc/paper/2019/file/c9efe5f26cd17ba6216bbe2a7d26d490-Paper.pdf)
+  - [DoppelGANger](https://dl.acm.org/doi/pdf/10.1145/3419394.3423643)
 
 ## Contributing
 We are open to collaboration! If you want to start contributing you only need to:
   1. Search for an issue in which you would like to work. Issues for newcomers are labeled with good first issue.
   2. Create a PR solving the issue.
   3. We would review every PRs and either accept or ask for revisions.
 
 ## Support
-For support in using this library, please join our Discord server. Our Discord community is very friendly and great about quickly answering questions about the use and development of the library. [Click here to join our Discord community!](https://discord.com/invite/mw7xjJ7b7s)
+For support in using this library, please join our Discord server. Our Discord community is very friendly and great about quickly answering questions about the use and development of the library. [Click here to join our Discord community!](https://tiny.ydata.ai/dcai-ydata-synthetic)
+
+## FAQs
+Have a question? Check out the [Frequently Asked Questions](https://ydata.ai/resources/10-most-asked-questions-on-ydata-synthetic) about `ydata-synthetic`. If you feel something is missing, feel free to [book a beary informal chat with us](https://meetings.hubspot.com/fabiana-clemente).
 
 ## License
 [MIT License](https://github.com/ydataai/ydata-synthetic/blob/master/LICENSE)
```

### Comparing `ydata-synthetic-1.2.0/setup.py` & `ydata-synthetic-1.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,14 @@
       package_dir={'':'src'},
       include_package_data=True,
       options={"bdist_wheel": {"universal": True}},
       install_requires=requirements,
       extras_require={
           "streamlit": [
               "streamlit==1.18.1",
-              "typing-extensions==3.10.0",
+              "typing-extensions>=3.10.0",
               "streamlit_pandas_profiling==0.1.3",
               "ydata-profiling==4.0.0",
               "ydata-sdk>=0.2.1"
           ],
       },
       )
```

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/postprocessing/regular/inverse_preprocesser.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/postprocessing/regular/inverse_preprocesser.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/base_processor.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/preprocessing/base_processor.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/regular/ctgan_processor.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/preprocessing/regular/ctgan_processor.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/regular/processor.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/preprocessing/regular/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
         self._types = X.dtypes
 
         self._num_pipeline = Pipeline([
             ("scaler", MinMaxScaler()),
         ])
         self._cat_pipeline = Pipeline([
-            ("encoder", OneHotEncoder(sparse=False, handle_unknown='ignore')),
+            ("encoder", OneHotEncoder(sparse_output=False, handle_unknown='ignore')),
         ])
 
         self.num_pipeline.fit(X[self.num_cols]) if self.num_cols else zeros([len(X), 0])
         self.cat_pipeline.fit(X[self.cat_cols]) if self.num_cols else zeros([len(X), 0])
 
         self._num_col_idx_ = len(self.num_pipeline.get_feature_names_out())
         self._cat_col_idx_ = self._num_col_idx_ + len(self.cat_pipeline.get_feature_names_out())
```

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/timeseries/stock.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/preprocessing/timeseries/stock.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/timeseries/timeseries_processor.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/preprocessing/timeseries/timeseries_processor.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/preprocessing/timeseries/utils.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/preprocessing/timeseries/utils.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/About.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/streamlit_app/About.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/1_Train_a_synthesizer.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/streamlit_app/pages/1_Train_a_synthesizer.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/2_Generate_synthetic_data.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/streamlit_app/pages/2_Generate_synthetic_data.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/functions/generate.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/streamlit_app/pages/functions/generate.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/functions/load_data.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/streamlit_app/pages/functions/load_data.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/streamlit_app/pages/functions/train.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/streamlit_app/pages/functions/train.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/base.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,29 +22,31 @@
 from typeguard import typechecked
 
 from ydata_synthetic.preprocessing.regular.processor import (
     RegularDataProcessor, RegularModels)
 from ydata_synthetic.preprocessing.timeseries.timeseries_processor import (
     TimeSeriesDataProcessor, TimeSeriesModels)
 from ydata_synthetic.preprocessing.regular.ctgan_processor import CTGANDataProcessor
+from ydata_synthetic.preprocessing.timeseries.doppelganger_processor import DoppelGANgerProcessor
 from ydata_synthetic.synthesizers.saving_keras import make_keras_picklable
 
 _model_parameters = ['batch_size', 'lr', 'betas', 'layers_dim', 'noise_dim',
                      'n_cols', 'seq_len', 'condition', 'n_critic', 'n_features', 
                      'tau_gs', 'generator_dims', 'critic_dims', 'l2_scale', 
-                     'latent_dim', 'gp_lambda', 'pac']
+                     'latent_dim', 'gp_lambda', 'pac', 'gamma']
 _model_parameters_df = [128, 1e-4, (None, None), 128, 264,
                         None, None, None, 1, None, 0.2, [256, 256], 
-                        [256, 256], 1e-6, 128, 10.0, 10]
+                        [256, 256], 1e-6, 128, 10.0, 10, 1]
 
 _train_parameters = ['cache_prefix', 'label_dim', 'epochs', 'sample_interval', 
-                     'labels', 'n_clusters', 'epsilon', 'log_frequency']
+                     'labels', 'n_clusters', 'epsilon', 'log_frequency', 
+                     'measurement_cols', 'sequence_length', 'number_sequences']
 
 ModelParameters = namedtuple('ModelParameters', _model_parameters, defaults=_model_parameters_df)
-TrainParameters = namedtuple('TrainParameters', _train_parameters, defaults=('', None, 300, 50, None, 10, 0.005, True))
+TrainParameters = namedtuple('TrainParameters', _train_parameters, defaults=('', None, 300, 50, None, 10, 0.005, True, None, 1, 1))
 
 @typechecked
 class BaseModel(ABC):
     """
     Abstract class for synthetic data generation nmodels
 
     The main methods are train (for fitting the synthesizer), save/load and sample (generating synthetic records).
@@ -141,14 +143,15 @@
         elif isinstance(lr,(list, tuple)):
             assert len(lr)==2, "Please provide a two values array for the learning rates or a float."
             self.g_lr=lr[0]
             self.d_lr=lr[1]
 
     def define_gan(self):
         """Define the trainable model components.
+
         Optionally validate model structure with mock inputs and initialize optimizers."""
         raise NotImplementedError
 
     @property
     def model_parameters(self):
         "Returns the parameters of the model."
         return self._model_parameters
@@ -160,81 +163,81 @@
 
     def fit(self,
               data: Union[DataFrame, array],
               num_cols: Optional[List[str]] = None,
               cat_cols: Optional[List[str]] = None,
               train_arguments: Optional[TrainParameters] = None) -> Union[DataFrame, array]:
         """
-        ### Description:
         Trains and fit a synthesizer model to a given input dataset.
 
-        ### Args:
-        `data` (Union[DataFrame, array]): Training data
-        `num_cols` (Optional[List[str]]) : List with the names of the categorical columns
-        `cat_cols` (Optional[List[str]]): List of names of categorical columns
-        `train_arguments` (Optional[TrainParameters]): Training parameters
+        Args:
+            data (Union[DataFrame, array]): Training data
+            num_cols (Optional[List[str]]) : List with the names of the categorical columns
+            cat_cols (Optional[List[str]]): List of names of categorical columns
+            train_arguments (Optional[TrainParameters]): Training parameters
 
-        ### Returns:
-        **self:** *object*
+        Returns:
             Fitted synthesizer
         """
         if self.__MODEL__ in RegularModels.__members__:
             self.processor = RegularDataProcessor(num_cols=num_cols, cat_cols=cat_cols).fit(data)
         elif self.__MODEL__ in TimeSeriesModels.__members__:
             self.processor = TimeSeriesDataProcessor(num_cols=num_cols, cat_cols=cat_cols).fit(data)
         elif self.__MODEL__ == CTGANDataProcessor.SUPPORTED_MODEL:
             n_clusters = train_arguments.n_clusters
             epsilon = train_arguments.epsilon
             self.processor = CTGANDataProcessor(n_clusters=n_clusters, epsilon=epsilon, 
                                                 num_cols=num_cols, cat_cols=cat_cols).fit(data)
+        elif self.__MODEL__ == DoppelGANgerProcessor.SUPPORTED_MODEL:
+            measurement_cols = train_arguments.measurement_cols
+            sequence_length = train_arguments.sequence_length
+            self.processor = DoppelGANgerProcessor(num_cols=num_cols, cat_cols=cat_cols,
+                                                   measurement_cols=measurement_cols,
+                                                   sequence_length=sequence_length).fit(data)
         else:
             print(f'A DataProcessor is not available for the {self.__MODEL__}.')
 
     def sample(self, n_samples: int):
         """
-        ### Description:
         Generates samples from the trained synthesizer.
 
-        ### Args:
-        `n_samples` (int): Number of rows to generated.
+        Args:
+            n_samples (int): Number of rows to generated.
 
-        ### Returns:
-        **synth_sample:** pandas.DataFrame, shape (n_samples, n_features)
-            Returns the generated synthetic samples.
+        Returns:
+            synth_sample (pandas.DataFrame): generated synthetic samples.
         """
         steps = n_samples // self.batch_size + 1
         data = []
         for _ in tqdm.trange(steps, desc='Synthetic data generation'):
             z = random.uniform([self.batch_size, self.noise_dim], dtype=tf.dtypes.float32)
             records = self.generator(z, training=False).numpy()
             data.append(records)
         return self.processor.inverse_transform(array(vstack(data)))
 
     def save(self, path):
         """
-        ### Description:
         Saves a synthesizer as a pickle.
 
-        ### Args:
-        `path` (str): Path to write the synthesizer as a pickle object.
+        Args:
+            path (str): Path to write the synthesizer as a pickle object.
         """
         #Save only the generator?
         if self.__MODEL__=='WGAN' or self.__MODEL__=='WGAN_GP' or self.__MODEL__=='CWGAN_GP':
             del self.critic
         make_keras_picklable()
         dump(self, path)
 
     @classmethod
     def load(cls, path):
         """
-        ### Description:
         Loads a saved synthesizer from a pickle.
 
-        ### Args:
-        `path` (str): Path to read the synthesizer pickle from.
+        Args:
+            path (str): Path to read the synthesizer pickle from.
         """
         gpu_devices = tfconfig.list_physical_devices('GPU')
         if len(gpu_devices) > 0:
             try:
                 tfconfig.experimental.set_memory_growth(gpu_devices[0], True)
             except (ValueError, RuntimeError):
                 # Invalid device or cannot modify virtual devices once initialized.
@@ -258,19 +261,20 @@
         assert all(unique_frac < 0.3), \
             f"The provided columns {label_cols} are not valid conditional columns due to high cardinality. Please revise your input."
 
     def _prep_fit(self, data: DataFrame, label_cols: List[str], num_cols: List[str], cat_cols: List[str]):
         """
             Validate and prepare the data for the training of a conditionalGAN architecture
         Args:
-            data:
-            label_cols:
-            num_cols:
-            cat_cols:
+            data: training data
+            label_cols: label columns
+            num_cols: numerical columns
+            cat_cols: categorical columns
         Returns:
+            data, label: preprocessed data and labels
         """
         # Validating the label columns
         self._validate_label_col(data, label_cols)
         self._col_order = data.columns
         self.label_col = label_cols
 
         # Separating labels from the rest of the data to fit the data processor
@@ -303,8 +307,8 @@
         ##Validate here if the cond_vector=label_dim
         condition = condition.reset_index(drop=True)
         n_samples = len(condition)
         z_dist = random.uniform(shape=(n_samples, self.noise_dim))
         records = self.generator([z_dist, condition], training=False)
         data = self.processor.inverse_transform(array(records))
         data = concat([condition, data], axis=1)
-        return data[self._col_order]
+        return data[self._col_order]
```

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/loss.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/loss.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/cgan/model.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/cgan/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,19 @@
     __MODEL__='CGAN'
 
     def __init__(self, model_parameters):
         self._col_order = None
         super().__init__(model_parameters)
 
     def define_gan(self, activation_info: Optional[NamedTuple] = None):
+        """Define the trainable model components.
+        
+        Args:
+            activation_info (Optional[NamedTuple]): Defaults to None
+        """
         self.generator = Generator(self.batch_size). \
             build_model(input_shape=(self.noise_dim,),
                         label_shape=(self.label_dim),
                         dim=self.layers_dim, data_dim=self.data_dim,
                         activation_info = activation_info, tau = self.tau)
 
         self.discriminator = Discriminator(self.batch_size). \
@@ -64,40 +69,50 @@
 
         # The combined model  (stacked generator and discriminator)
         # Trains the generator to fool the discriminator
         self._model = Model([noise, label], validity)
         self._model.compile(loss='binary_crossentropy', optimizer=g_optimizer)
 
     def _generate_noise(self):
-        "Gaussian noise for the generator input."
+        """Gaussian noise for the generator input."""
         while True:
             yield random.uniform(shape=(self.noise_dim,))
 
     def get_batch_noise(self):
-        "Create a batch iterator for the generator gaussian noise input."
+        """Create a batch iterator for the generator gaussian noise input."""
         return iter(tfdata.Dataset.from_generator(self._generate_noise, output_types=dtypes.float32)
                                 .batch(self.batch_size)
                                 .repeat())
 
     def get_data_batch(self, data, batch_size, seed=0):
-        "Produce real data batches from the passed data object."
+        """Produce real data batches from the passed data object.
+
+        Args:
+            data: real data.
+            batch_size: batch size.
+            seed (int, optional): Defaults to 0.
+
+        Returns:
+            data batch.
+        """
         start_i = (batch_size * seed) % len(data)
         stop_i = start_i + batch_size
         shuffle_seed = (batch_size * seed) // len(data)
         np.random.seed(shuffle_seed)
         data_ix = np.random.choice(data.shape[0], replace=False, size=len(data))  # wasteful to shuffle every time
         return data[data_ix[start_i: stop_i]]
 
     def fit(self,
             data: DataFrame,
             label_cols: List[str],
             train_arguments: TrainParameters,
             num_cols: List[str],
             cat_cols: List[str]):
-        """
+        """Trains and fit a synthesizer model to a given input dataset.
+
         Args:
             data: A pandas DataFrame with the data to be synthesized
             label_cols: The name of the column to be used as a label and condition for the training
             train_arguments: GAN training arguments.
             num_cols: List of columns of the data object to be handled as numerical
             cat_cols: List of columns of the data object to be handled as categorical
         """
@@ -148,28 +163,46 @@
             print("%d [D loss: %f, acc.: %.2f%%] [G loss: %f]" % (epoch, d_loss[0], 100 * d_loss[1], g_loss))
 
             # If at save interval => save model state and generated image samples
             if epoch % train_arguments.sample_interval == 0:
                 self._run_checkpoint(train_arguments, epoch, label)
 
     def _run_checkpoint(self, train_arguments, epoch, label):
-        "Run checkpoint. Store model state and generated samples."
+        """Run checkpoint and store model state and generated samples.
+
+        Args:
+            train_arguments:  GAN training arguments.
+            epoch: training epoch
+            label: deprecated
+        """
         if path.exists('./cache') is False:
             os.mkdir('./cache')
         model_checkpoint_base_name = './cache/' + train_arguments.cache_prefix + '_{}_model_weights_step_{}.h5'
         self.generator.save_weights(model_checkpoint_base_name.format('generator', epoch))
         self.discriminator.save_weights(model_checkpoint_base_name.format('discriminator', epoch))
 
 # pylint: disable=R0903
 class Generator():
     "Standard discrete conditional generator."
     def __init__(self, batch_size):
         self.batch_size = batch_size
 
     def build_model(self, input_shape, label_shape, dim, data_dim, activation_info: Optional[NamedTuple] = None, tau: Optional[float] = None):
+        """Create model components.
+
+        Args:
+            input_shape: input dimensionality.
+            label_shape: label dimensionality.
+            dim: hidden layers dimensions.
+            data_dim: Output dimensionality.
+            activation_info (Optional[NamedTuple]): Defaults to None
+            tau (Optional[float]): Gumbel-Softmax non-negative temperature. Defaults to None
+        Returns:
+            Generator model
+        """
         noise = Input(shape=input_shape, batch_size=self.batch_size)
         label_v = Input(shape=label_shape)
         x = concatenate([noise, label_v])
         x = Dense(dim, activation='relu')(x)
         x = Dense(dim * 2, activation='relu')(x)
         x = Dense(dim * 4, activation='relu')(x)
         x = Dense(data_dim)(x)
@@ -181,14 +214,24 @@
 # pylint: disable=R0903
 class Discriminator():
     "Standard discrete conditional discriminator."
     def __init__(self, batch_size):
         self.batch_size = batch_size
 
     def build_model(self, input_shape, label_shape, dim):
+        """Create model components.
+
+        Args:
+            input_shape: input dimensionality.
+            label_shape: labels dimenstionality.
+            dim: hidden layers size.
+
+        Returns:
+            Discriminator model
+        """
         events = Input(shape=input_shape, batch_size=self.batch_size)
         label = Input(shape=label_shape, batch_size=self.batch_size)
         input_ = concatenate([events, label])
         x = Dense(dim * 4, activation='relu')(input_)
         x = Dropout(0.1)(x)
         x = Dense(dim * 2, activation='relu')(x)
         x = Dropout(0.1)(x)
```

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/cramergan/model.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/cramergan/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,22 @@
 
         Based according to the WGAN paper - https://arxiv.org/pdf/1705.10743.pdf
         CramerGAN, a solution to biased Wassertein Gradients https://arxiv.org/abs/1705.10743"""
         self.gradient_penalty_weight = gradient_penalty_weight
         super().__init__(model_parameters)
 
     def define_gan(self, activation_info: Optional[NamedTuple] = None):
+        """Define the trainable model components.
+
+        Args:
+            activation_info (Optional[NamedTuple], optional): Defaults to None.
+
+        Returns:
+            (generator_optimizer, critic_optimizer): Generator and critic optimizers
+        """
         self.generator = Generator(self.batch_size). \
             build_model(input_shape=(self.noise_dim,), dim=self.layers_dim, data_dim=self.data_dim,
                         activation_info=activation_info, tau = self.tau)
 
         self.critic = Critic(self.batch_size). \
             build_model(input_shape=(self.data_dim,), dim=self.layers_dim)
 
@@ -45,22 +53,34 @@
         z = Input(shape=(self.noise_dim,), batch_size=self.batch_size)
         fake = self.generator(z)
         logits = self.critic(fake)
 
         return g_optimizer, c_optimizer
 
     def gradient_penalty(self, real, fake):
+        """Compute gradient penalty.
+        
+        Args:
+            real: real event.
+            fake: fake event.
+        Returns:
+            gradient_penalty.
+        """
         gp = gradient_penalty(self.f_crit, real, fake, mode=Mode.CRAMER)
         return gp
 
     def update_gradients(self, x, g_optimizer, c_optimizer):
         """Compute and apply the gradients for both the Generator and the Critic.
 
-        :param x: real data event
-        :return: generator gradients, critic gradients
+        Args:
+            x: real data event
+            g_optimizer: generator optimizer
+            c_optimizer: critic optimizer
+        Returns:
+            (critic loss, generator loss)
         """
         # Update the gradients of critic for n_critic times (Training the critic)
 
         ##New generator gradient_tape
         noise= tf.random.normal([x.shape[0], self.noise_dim], dtype=tf.dtypes.float32)
         noise2= tf.random.normal([x.shape[0], self.noise_dim], dtype=tf.dtypes.float32)
 
@@ -87,65 +107,95 @@
         )
 
         return c_loss, g_loss
 
     def g_lossfn(self, real, fake, fake2):
         """Compute generator loss function according to the CramerGAN paper.
 
-        :param real: A real sample
-        :param fake: A fake sample
-        :param fak2: A second fake sample
-        :return: Loss of the generator
+        Args:
+            real: A real sample
+            fake: A fake sample
+            fak2: A second fake sample
+
+        Returns:
+            Loss of the generator
         """
         g_loss = tf.norm(self.critic(real, training=True) - self.critic(fake, training=True), axis=1) + \
                  tf.norm(self.critic(real, training=True) - self.critic(fake2, training=True), axis=1) - \
                  tf.norm(self.critic(fake, training=True) - self.critic(fake2, training=True), axis=1)
         return tf.reduce_mean(g_loss)
 
     def f_crit(self, real, fake):
         """
-        Computes the critic distance function f between two samples
-        :param real: A real sample
-        :param fake: A fake sample
-        :return: Loss of the critic
+        Computes the critic distance function f between two samples.
+
+        Args:
+            real: A real sample
+            fake: A fake sample
+        Returns:
+            Loss of the critic
         """
         return tf.norm(self.critic(real, training=True) - self.critic(fake, training=True), axis=1) - tf.norm(self.critic(real, training=True), axis=1)
 
     def c_lossfn(self, real, fake, fake2):
-        """
-        :param real: A real sample
-        :param fake: A fake sample
-        :param fak2: A second fake sample
-        :return: Loss of the critic
+        """Compute the loss of the critic.
+
+        Args:
+            real: A real sample
+            fake: A fake sample
+            fake2: A second fake sample
+        
+        Returns:
+            Loss of the critic
         """
         f_real = self.f_crit(real, fake2)
         f_fake = self.f_crit(fake, fake2)
         loss_surrogate = f_real - f_fake
         gp = self.gradient_penalty(real, [fake, fake2])
         return tf.reduce_mean(- loss_surrogate + self.gradient_penalty_weight*gp)
 
     @staticmethod
     def get_data_batch(train, batch_size, seed=0):
+        """Get real data batches from the passed data object.
+
+        Args:
+            train: real data.
+            batch_size: batch size.
+            seed (int, optional):Defaults to 0.
+
+        Returns:
+            data batch.
+        """
         # np.random.seed(seed)
         # x = train.loc[ np.random.choice(train.index, batch_size) ].values
         # iterate through shuffled indices, so every sample gets covered evenly
         start_i = (batch_size * seed) % len(train)
         stop_i = start_i + batch_size
         shuffle_seed = (batch_size * seed) // len(train)
         np.random.seed(shuffle_seed)
         train_ix = np.random.choice(train.shape[0], replace=False, size=len(train))  # wasteful to shuffle every time
         train_ix = list(train_ix) + list(train_ix)  # duplicate to cover ranges past the end of the set
         return train[train_ix[start_i: stop_i]]
 
     def train_step(self, train_data, optimizers):
+        """Perform a training step.
+
+        Args:
+            train_data: training data
+            optimizers: generator and critic optimizers 
+
+        Returns:
+            (critic_loss, generator_loss): Critic and generator loss.
+        """
         critic_loss, g_loss = self.update_gradients(train_data, *optimizers)
         return critic_loss, g_loss
 
     def fit(self, data, train_arguments: TrainParameters, num_cols: List[str], cat_cols: List[str]):
-        """
+        """Fit a synthesizer model to a given input dataset.
+
         Args:
             data: A pandas DataFrame or a Numpy array with the data to be synthesized
             train_arguments: GAN training arguments.
             num_cols: List of columns of the data object to be handled as numerical
             cat_cols: List of columns of the data object to be handled as categorical
         """
         super().fit(data, num_cols, cat_cols)
@@ -174,31 +224,59 @@
                         self.generator.save_weights(model_checkpoint_base_name.format('generator', iteration))
                         self.critic.save_weights(model_checkpoint_base_name.format('critic', iteration))
                 print(f"Epoch: {epoch} | critic_loss: {c_loss} | gen_loss: {g_loss}")
 
 
 class Generator(tf.keras.Model):
     def __init__(self, batch_size):
-        """Simple generator with dense feedforward layers."""
+        """Simple generator with dense feedforward layers.
+
+        Args:
+            batch_size (int): batch size
+        """
         self.batch_size = batch_size
 
     def build_model(self, input_shape, dim, data_dim, activation_info: Optional[NamedTuple] = None, tau: Optional[float] = None):
+        """Create model components.
+
+        Args:
+            input_shape: input dimensionality.
+            dim: hidden layers dimensions.
+            data_dim: Output dimensionality.
+            activation_info (Optional[NamedTuple]): Defaults to None
+            tau (Optional[float]): Gumbel-Softmax non-negative temperature. Defaults to None
+        Returns:
+            Generator model
+        """
         input_ = Input(shape=input_shape, batch_size=self.batch_size)
         x = Dense(dim, activation='relu')(input_)
         x = Dense(dim * 2, activation='relu')(x)
         x = Dense(dim * 4, activation='relu')(x)
         x = Dense(data_dim, activation='softmax')(x)
         return Model(inputs=input_, outputs=x)
 
 class Critic(tf.keras.Model):
     def __init__(self, batch_size):
-        """Simple critic with dense feedforward and dropout layers."""
+        """Simple critic with dense feedforward and dropout layers.
+
+        Args:
+            batch_size (int): batch size
+        """
         self.batch_size = batch_size
 
     def build_model(self, input_shape, dim):
+        """Create model components.
+
+        Args:
+            input_shape: input dimensionality.
+            dim: hidden layers size.
+
+        Returns:
+            Critic model
+        """
         input_ = Input(shape=input_shape, batch_size=self.batch_size)
         x = Dense(dim * 4, activation='relu')(input_)
         x = Dropout(0.1)(x)
         x = Dense(dim * 2, activation='relu')(x)
         x = Dropout(0.1)(x)
         x = Dense(dim, activation='relu')(x)
         x = Dense(1)(x)
```

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/ctgan/model.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/ctgan/model.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/ctgan/utils.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/ctgan/utils.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/cwgangp/model.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/cwgangp/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,14 +36,19 @@
         """
         WGAN_GP.__init__(self, model_parameters,
                          n_generator=n_generator,
                          n_critic=n_critic,
                          gradient_penalty_weight=gradient_penalty_weight)
 
     def define_gan(self, activation_info: Optional[NamedTuple] = None):
+        """Define the trainable model components.
+        
+        Args:
+            activation_info (Optional[NamedTuple]): Defaults to None
+        """
         self.generator = Generator(self.batch_size). \
             build_model(input_shape=(self.noise_dim,),
                         label_shape=(self.label_dim, ),
                         dim=self.layers_dim,
                         data_dim=self.data_dim,
                         activation_info = activation_info,
                         tau = self.tau)
@@ -54,36 +59,61 @@
                         dim=self.layers_dim)
 
         g_optimizer = Adam(self.g_lr, beta_1=self.beta_1, beta_2=self.beta_2)
         c_optimizer = Adam(self.d_lr, beta_1=self.beta_1, beta_2=self.beta_2)
         return g_optimizer, c_optimizer
 
     def gradient_penalty(self, real, fake, label):
+        """Compute gradient penalty.
+        
+        Args:
+            real: real event.
+            fake: fake event.
+            label: ground truth.
+        Returns:
+            gradient_penalty
+        """
         epsilon = random.uniform([real.shape[0], 1], 0.0, 1.0, dtype=dtypes.float32)
         x_hat = epsilon * real + (1 - epsilon) * fake
         with GradientTape() as t:
             t.watch(x_hat)
             d_hat = self.critic([x_hat, label])
         gradients = t.gradient(d_hat, x_hat)
         ddx = sqrt(reduce_sum(gradients ** 2))
         d_regularizer = reduce_mean((ddx - 1.0) ** 2)
         return d_regularizer
 
     @staticmethod
     def get_data_batch(data, batch_size, seed=0):
-        "Produce real data batches from the passed data object."
+        """Produce real data batches from the passed data object.
+
+        Args:
+            train: real data.
+            batch_size: batch size.
+            seed (int, optional):Defaults to 0.
+
+        Returns:
+            data batch.
+        """
         start_i = (batch_size * seed) % len(data)
         stop_i = start_i + batch_size
         shuffle_seed = (batch_size * seed) // len(data)
         np.random.seed(shuffle_seed)
         data_ix = np.random.choice(data.shape[0], replace=False, size=len(data))  # wasteful to shuffle every time
         return dtypes.cast(data[data_ix[start_i: stop_i]], dtype=dtypes.float32)
 
     def c_lossfn(self, real):
-        "Forward pass on the critic and computes the loss."
+        """Compute the critic loss.
+
+        Args:
+            real: A real sample
+        
+        Returns:
+            Critic loss
+        """
         real, label = real
         # generating noise from a uniform distribution
         noise = random.uniform([real.shape[0], self.noise_dim], minval=0.999, maxval=1.0 , dtype=dtypes.float32)
         # run noise through generator
         fake = self.generator([noise, label])
         # discriminate x and x_gen
         logits_real = self.critic([real, label])
@@ -97,16 +127,18 @@
                   + gp * self.gradient_penalty_weight)
         return c_loss
 
     def g_lossfn(self, real):
         """
         Forward pass on the generator and computes the loss.
 
-        :param real: Data batch we are analyzing
-        :return: Loss of the generator
+        Args:
+            real: Data batch we are analyzing
+        Returns:
+            Generator loss
         """
         real, label = real
 
         # generating noise from a uniform distribution
         noise = random.uniform([real.shape[0], self.noise_dim], minval=0.0, maxval=0.001 ,dtype=dtypes.float32)
 
         fake = self.generator([noise, label])
@@ -160,32 +192,45 @@
                 ))
 
             # If at save interval => save model state and generated image samples
             if epoch % train_arguments.sample_interval == 0:
                 self._run_checkpoint(train_arguments, epoch)
 
     def _run_checkpoint(self, train_arguments, epoch):
-        "Run checkpoint. Store model state and generated samples."
+        "Run checkpoint and store model state and generated samples."
         if path.exists('./cache') is False:
             os.mkdir('./cache')
         model_checkpoint_base_name = './cache/' + train_arguments.cache_prefix + '_{}_model_weights_step_{}.h5'
         self.generator.save_weights(model_checkpoint_base_name.format('generator', epoch))
         self.critic.save_weights(model_checkpoint_base_name.format('critic', epoch))
 
 
 act_leakyr = LeakyReLU(alpha=0.2)
 # pylint: disable=R0903,D203
 class Generator():
-
     "Standard discrete conditional generator."
     def __init__(self, batch_size):
-        "Sets the properties of the generator."
+        """Sets the properties of the generator.
+
+        Args:
+            batch_size (int): batch size
+        """
         self.batch_size = batch_size
 
     def build_model(self, input_shape, label_shape, dim, data_dim, activation_info: Optional[NamedTuple] = None, tau: Optional[float] = None):
+        """Create model components.
+
+        Args:
+            input_shape: input dimensionality.
+            label_shape: label dimensionality.
+            dim: hidden layers dimensions.
+            data_dim: Output dimensionality.
+            activation_info (Optional[NamedTuple]): Defaults to None
+            tau (Optional[float]): Gumbel-Softmax non-negative temperature. Defaults to None
+        """
         noise = Input(shape=input_shape, batch_size=self.batch_size)
         label_v = Input(shape=label_shape)
         x = concatenate([noise, label_v])
         x = Dense(dim, activation=act_leakyr)(x)
         x = Dense(dim * 2, activation=act_leakyr)(x)
         x = Dense(dim * 4, activation=act_leakyr)(x)
         x = Dense(data_dim)(x)
@@ -196,15 +241,25 @@
 # pylint: disable=R0903,D203
 class Critic():
     "Conditional Critic."
     def __init__(self, batch_size):
         "Sets the properties of the critic."
         self.batch_size = batch_size
 
-    def build_model(self, input_shape, label_shape,dim):
+    def build_model(self, input_shape, label_shape, dim):
+        """Create model components.
+
+        Args:
+            input_shape: input dimensionality.
+            label_shape: label dimensionality.
+            dim: hidden layers size.
+
+        Returns:
+            Critic model
+        """
         events = Input(shape=input_shape, batch_size=self.batch_size)
         label = Input(shape=label_shape, batch_size=self.batch_size)
         input_ = concatenate([events, label])
         x = Dense(dim * 4, activation=act_leakyr)(input_)
         x = Dropout(0.1)(x)
         x = Dense(dim * 2, activation=act_leakyr)(x)
         x = Dropout(0.1)(x)
```

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/dragan/model.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/dragan/model.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,42 +16,68 @@
 from ....synthesizers.loss import Mode, gradient_penalty
 
 class DRAGAN(BaseGANModel):
 
     __MODEL__='DRAGAN'
 
     def __init__(self, model_parameters, n_discriminator, gradient_penalty_weight=10):
+        """DRAGAN model architecture implementation.
+
+        Args:
+            model_parameters:
+            n_discriminator:
+            gradient_penalty_weight (int, optional): Defaults to 10.
+        """
         # As recommended in DRAGAN paper - https://arxiv.org/abs/1705.07215
         self.n_discriminator = n_discriminator
         self.gradient_penalty_weight = gradient_penalty_weight
         super().__init__(model_parameters)
 
     def define_gan(self, col_transform_info: Optional[NamedTuple] = None):
+        """Define the trainable model components.
+
+        Args:
+            col_transform_info (Optional[NamedTuple], optional): Defaults to None.
+
+        Returns:
+            (generator_optimizer, discriminator_optimizer): Generator and discriminator optimizers
+        """
         # define generator/discriminator
         self.generator = Generator(self.batch_size). \
             build_model(input_shape=(self.noise_dim,), dim=self.layers_dim, data_dim=self.data_dim,
                         activation_info=col_transform_info, tau = self.tau)
 
         self.discriminator = Discriminator(self.batch_size). \
             build_model(input_shape=(self.data_dim,), dim=self.layers_dim)
 
         g_optimizer = Adam(self.g_lr, beta_1=self.beta_1, beta_2=self.beta_2, clipvalue=0.001)
         d_optimizer = Adam(self.d_lr, beta_1=self.beta_1, beta_2=self.beta_2, clipvalue=0.001)
         return g_optimizer, d_optimizer
 
     def gradient_penalty(self, real, fake):
+        """Compute gradient penalty.
+        
+        Args:
+            real: real event.
+            fake: fake event.
+        Returns:
+            gradient_penalty.
+        """
         gp = gradient_penalty(self.discriminator, real, fake, mode= Mode.DRAGAN)
         return gp
 
     def update_gradients(self, x, g_optimizer, d_optimizer):
-        """
-        Compute the gradients for both the Generator and the Discriminator
+        """Compute the gradients for Generator and Discriminator.
+
+        Args:
             x (tf.tensor): real data event
-            *_optimizer (tf.OptimizerV2): Optimizer for the * model
-        :return: generator gradients, discriminator gradients
+            g_optimizer (tf.OptimizerV2): Optimizer for the generator model
+            c_optimizer (tf.OptimizerV2): Optimizer for the discriminator model
+        Returns:
+            (discriminator loss, generator loss)
         """
         # Update the gradients of critic for n_critic times (Training the critic)
         for _ in range(self.n_discriminator):
             with tf.GradientTape() as d_tape:
                 d_loss = self.d_lossfn(x)
             # Get the gradients of the critic
             d_gradient = d_tape.gradient(d_loss, self.discriminator.trainable_variables)
@@ -71,16 +97,21 @@
         g_optimizer.apply_gradients(
             zip(gen_gradients, self.generator.trainable_variables)
         )
 
         return d_loss, gen_loss
 
     def d_lossfn(self, real):
-        """
-        Calculates the critic losses
+        """Calculates the critic losses.
+
+        Args:
+            real: real data examples.
+
+        Returns:
+            discriminator loss
         """
         noise = tf.random.normal((self.batch_size, self.noise_dim), dtype=tf.dtypes.float64)
         # run noise through generator
         fake = self.generator(noise)
         # discriminate x and x_gen
         logits_real = self.discriminator(real, training=True)
         logits_fake = self.discriminator(fake, training=True)
@@ -90,42 +121,63 @@
 
         # getting the loss of the discriminator.
         d_loss = (tf.reduce_mean(logits_fake)
                   - tf.reduce_mean(logits_real)
                   + gp * self.gradient_penalty_weight)
         return d_loss
 
-    # generator loss
     def g_lossfn(self, real):
-        """
-        Calculates the Generator losses
-        :param real: Data batch we are analyzing
-        :return: Loss of the generator
+        """Calculates the Generator losses.
+
+        Args:
+            real: real data.
+        Returns:
+            generator loss
         """
         # generating noise from a uniform distribution
         noise = tf.random.normal((real.shape[0], self.noise_dim), dtype=tf.float64)
 
         fake = self.generator(noise, training=True)
         logits_fake = self.discriminator(fake, training=True)
         g_loss = -tf.reduce_mean(logits_fake)
         return g_loss
 
     def get_data_batch(self, train, batch_size):
+        """Get real data batches from the passed data object.
+
+        Args:
+            train: real data.
+            batch_size: batch size.
+            seed (int, optional):Defaults to 0.
+
+        Returns:
+            data batch.
+        """
         buffer_size = len(train)
         #tensor_data = pd.concat([x_train, y_train], axis=1)
         train_loader = tf.data.Dataset.from_tensor_slices(train) \
             .batch(batch_size).shuffle(buffer_size)
         return train_loader
 
     def train_step(self, train_data, optimizers):
+        """Perform a training step.
+
+        Args:
+            train_data: training data
+            optimizers: generator and critic optimizers 
+
+        Returns:
+            (critic_loss, generator_loss): Critic and generator loss.
+        """
         d_loss, g_loss = self.update_gradients(train_data, *optimizers)
         return d_loss, g_loss
 
     def fit(self, data, train_arguments, num_cols, cat_cols):
-        """
+        """Fit a synthesizer model to a given input dataset.
+
         Args:
             data: A pandas DataFrame or a Numpy array with the data to be synthesized
             train_arguments: GAN training arguments.
             num_cols: List of columns of the data object to be handled as numerical
             cat_cols: List of columns of the data object to be handled as categorical
         """
         super().fit(data, num_cols, cat_cols)
@@ -158,31 +210,61 @@
                     model_checkpoint_base_name = './cache/' + train_arguments.cache_prefix + '_{}_model_weights_step_{}.h5'
                     self.generator.save_weights(model_checkpoint_base_name.format('generator', epoch))
                     self.discriminator.save_weights(model_checkpoint_base_name.format('discriminator', epoch))
 
 
 class Discriminator(Model):
     def __init__(self, batch_size):
+        """Simple discriminator with dense feedforward layers.
+
+        Args:
+            batch_size (int): batch size
+        """
         self.batch_size = batch_size
 
     def build_model(self, input_shape, dim):
+        """Create model components.
+
+        Args:
+            input_shape: input dimensionality.
+            dim: hidden layers size.
+
+        Returns:
+            Discriminator model
+        """
         input = Input(shape=input_shape, batch_size=self.batch_size)
         x = Dense(dim * 4, kernel_initializer=initializers.TruncatedNormal(mean=0., stddev=0.5), activation='relu')(input)
         x = Dropout(0.1)(x)
         x = Dense(dim * 2, activation='relu')(x)
         x = Dropout(0.1)(x)
         x = Dense(dim, activation='relu')(x)
         x = Dense(1, activation='sigmoid')(x)
         return Model(inputs=input, outputs=x)
 
 class Generator(Model):
     def __init__(self, batch_size):
+        """Simple generator with dense feedforward layers.
+
+        Args:
+            batch_size (int): batch size
+        """
         self.batch_size = batch_size
 
     def build_model(self, input_shape, dim, data_dim, activation_info: NamedTuple = None, tau: Optional[float] = None):
+        """Create model components.
+
+        Args:
+            input_shape: input dimensionality.
+            dim: hidden layers dimensions.
+            data_dim: Output dimensionality.
+            activation_info (Optional[NamedTuple]): Defaults to None
+            tau (Optional[float]): Gumbel-Softmax non-negative temperature. Defaults to None
+        Returns:
+            Generator model
+        """
         input = Input(shape=input_shape, batch_size = self.batch_size)
         x = Dense(dim, kernel_initializer=initializers.TruncatedNormal(mean=0., stddev=0.5), activation='relu')(input)
         x = Dense(dim * 2, activation='relu')(x)
         x = Dense(dim * 4, activation='relu')(x)
         x = Dense(data_dim)(x)
         #if activation_info:
         #    x = GumbelSoftmaxActivation(activation_info, tau=tau)(x)
```

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/gmm/model.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/gmm/model.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/model.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/model.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/vanillagan/model.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/vanillagan/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,22 @@
 
     __MODEL__='GAN'
 
     def __init__(self, model_parameters):
         super().__init__(model_parameters)
 
     def define_gan(self, activation_info: Optional[NamedTuple]):
+        """Define the trainable model components.
+
+        Args:
+            activation_info (Optional[NamedTuple], optional): Defaults to None.
+
+        Returns:
+            (generator_optimizer, critic_optimizer): Generator and critic optimizers
+        """
         self.generator = Generator(self.batch_size).\
             build_model(input_shape=(self.noise_dim,), dim=self.layers_dim, data_dim=self.data_dim,)
 
         self.discriminator = Discriminator(self.batch_size).\
             build_model(input_shape=(self.data_dim,), dim=self.layers_dim)
 
         g_optimizer = Adam(self.g_lr, beta_1=self.beta_1, beta_2=self.beta_2)
@@ -51,34 +59,45 @@
 
         # The combined model  (stacked generator and discriminator)
         # Trains the generator to fool the discriminator
         self._model = Model(z, validity)
         self._model.compile(loss='binary_crossentropy', optimizer=g_optimizer)
 
     def get_data_batch(self, train, batch_size, seed=0):
+        """Get real data batches from the passed data object.
+
+        Args:
+            train: real data
+            batch_size: batch size
+            seed (int, optional):Defaults to 0.
+
+        Returns:
+            data batch
+        """
         # # random sampling - some samples will have excessively low or high sampling, but easy to implement
         # np.random.seed(seed)
         # x = train.loc[ np.random.choice(train.index, batch_size) ].values
         # iterate through shuffled indices, so every sample gets covered evenly
 
         start_i = (batch_size * seed) % len(train)
         stop_i = start_i + batch_size
         shuffle_seed = (batch_size * seed) // len(train)
         np.random.seed(shuffle_seed)
         train_ix = np.random.choice(train.shape[0], replace=False, size=len(train))  # wasteful to shuffle every time
         train_ix = list(train_ix) + list(train_ix)  # duplicate to cover ranges past the end of the set
         return train[train_ix[start_i: stop_i]]
 
     def fit(self, data, train_arguments: TrainParameters, num_cols: List[str], cat_cols: List[str]):
-        """
+        """Fit a synthesizer model to a given input dataset.
+
         Args:
             data: A pandas DataFrame or a Numpy array with the data to be synthesized
             train_arguments: GAN training arguments.
-            num_cols: List of columns of the data object to be handled as numerical
-            cat_cols: List of columns of the data object to be handled as categorical
+            num_cols (List[str]): List of columns of the data object to be handled as numerical
+            cat_cols (List[str]): List of columns of the data object to be handled as categorical
         """
         super().fit(data, num_cols, cat_cols)
 
         processed_data = self.processor.transform(data)
         self.data_dim = processed_data.shape[1]
         self.define_gan(self.processor.col_transform_info)
 
@@ -128,29 +147,59 @@
                 z = tf.random.normal((432, self.noise_dim))
                 gen_data = self.generator(z)
                 print('generated_data')
 
 
 class Generator(tf.keras.Model):
     def __init__(self, batch_size):
+        """Simple generator with dense feedforward layers.
+
+        Args:
+            batch_size (int): batch size
+        """
         self.batch_size=batch_size
 
-    def build_model(self, input_shape, dim, data_dim):
+    def build_model(self, input_shape, dim, data_dim, activation_info: Optional[NamedTuple] = None, tau: Optional[float] = None):
+        """Create model components.
+
+        Args:
+            input_shape: input dimensionality.
+            dim: hidden layers dimensions.
+            data_dim: Output dimensionality.
+            activation_info (Optional[NamedTuple]): Defaults to None
+            tau (Optional[float]): Gumbel-Softmax non-negative temperature. Defaults to None
+        Returns:
+            Generator model
+        """
         input= Input(shape=input_shape, batch_size=self.batch_size)
         x = Dense(dim, activation='relu')(input)
         x = Dense(dim * 2, activation='relu')(x)
         x = Dense(dim * 4, activation='relu')(x)
         x = Dense(data_dim)(x)
         return Model(inputs=input, outputs=x)
 
 class Discriminator(tf.keras.Model):
     def __init__(self,batch_size):
+        """Simple discriminator with dense feedforward and dropout layers.
+
+        Args:
+            batch_size (int): batch size
+        """
         self.batch_size=batch_size
 
     def build_model(self, input_shape, dim):
+        """Create model components.
+
+        Args:
+            input_shape: input dimensionality.
+            dim: hidden layers size.
+
+        Returns:
+            Discriminator model
+        """
         input = Input(shape=input_shape, batch_size=self.batch_size)
         x = Dense(dim * 4, activation='relu')(input)
         x = Dropout(0.1)(x)
         x = Dense(dim * 2, activation='relu')(x)
         x = Dropout(0.1)(x)
         x = Dense(dim, activation='relu')(x)
         x = Dense(1, activation='sigmoid')(x)
```

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/wgan/model.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/wgan/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,17 +41,34 @@
         # As recommended in WGAN paper - https://arxiv.org/abs/1701.07875
         # WGAN-GP - WGAN with Gradient Penalty
         self.n_critic = n_critic
         self.clip_value = clip_value
         super().__init__(model_parameters)
 
     def wasserstein_loss(self, y_true, y_pred):
+        """Calculate wasserstein loss.
+
+        Args:
+            y_true: ground truth.
+            y_pred: predictions.
+
+        Returns:
+            wasserstein loss.
+        """
         return K.mean(y_true * y_pred)
 
     def define_gan(self, activation_info: Optional[NamedTuple] = None):
+        """Define the trainable model components.
+
+        Args:
+            activation_info (Optional[NamedTuple], optional): Defaults to None.
+
+        Returns:
+            (generator_optimizer, critic_optimizer): Generator and critic optimizers.
+        """
         self.generator = Generator(self.batch_size). \
             build_model(input_shape=(self.noise_dim,), dim=self.layers_dim, data_dim=self.data_dim,
                         activation_info=activation_info, tau = self.tau)
 
         self.critic = Critic(self.batch_size). \
             build_model(input_shape=(self.data_dim,), dim=self.layers_dim)
 
@@ -75,33 +92,44 @@
         # The combined model  (stacked generator and discriminator)
         # Trains the generator to fool the discriminator
         #For the WGAN model use the Wassertein loss
         self._model = Model(z, validity)
         self._model.compile(loss='binary_crossentropy', optimizer=optimizer)
 
     def get_data_batch(self, train, batch_size, seed=0):
+        """Get real data batches from the passed data object.
+
+        Args:
+            train: real data.
+            batch_size: batch size.
+            seed (int, optional):Defaults to 0.
+
+        Returns:
+            data batch.
+        """
         # np.random.seed(seed)
         # x = train.loc[ np.random.choice(train.index, batch_size) ].values
         # iterate through shuffled indices, so every sample gets covered evenly
         start_i = (batch_size * seed) % len(train)
         stop_i = start_i + batch_size
         shuffle_seed = (batch_size * seed) // len(train)
         np.random.seed(shuffle_seed)
         train_ix = np.random.choice(train.shape[0], replace=False, size=len(train))  # wasteful to shuffle every time
         train_ix = list(train_ix) + list(train_ix)  # duplicate to cover ranges past the end of the set
         return train[train_ix[start_i: stop_i]]
 
     def fit(self, data, train_arguments: TrainParameters, num_cols: List[str],
               cat_cols: List[str]):
-        """
+        """Fit a synthesizer model to a given input dataset.
+
         Args:
-            data: A pandas DataFrame or a Numpy array with the data to be synthesized
+            data: A pandas DataFrame or a Numpy array with the data to be synthesized.
             train_arguments: GAN training arguments.
-            num_cols: List of columns of the data object to be handled as numerical
-            cat_cols: List of columns of the data object to be handled as categorical
+            num_cols (List[str]): List of columns of the data object to be handled as numerical.
+            cat_cols (List[str]): List of columns of the data object to be handled as categorical.
         """
         super().fit(data, num_cols, cat_cols)
 
         processed_data = self.processor.transform(data)
         self.data_dim = processed_data.shape[1]
         self.define_gan(self.processor.col_transform_info)
 
@@ -154,31 +182,61 @@
                     model_checkpoint_base_name = './cache/' + train_arguments.cache_prefix + '_{}_model_weights_step_{}.h5'
                     self.generator.save_weights(model_checkpoint_base_name.format('generator', epoch))
                     self.critic.save_weights(model_checkpoint_base_name.format('critic', epoch))
 
 
 class Generator(tf.keras.Model):
     def __init__(self, batch_size):
+        """Simple generator with dense feedforward layers.
+
+        Args:
+            batch_size (int): batch size
+        """
         self.batch_size = batch_size
 
     def build_model(self, input_shape, dim, data_dim, activation_info: Optional[NamedTuple] = None, tau: Optional[float] = None):
+        """Create model components.
+
+        Args:
+            input_shape: input dimensionality.
+            dim: hidden layers dimensions.
+            data_dim: Output dimensionality.
+            activation_info (Optional[NamedTuple]): Defaults to None
+            tau (Optional[float]): Gumbel-Softmax non-negative temperature. Defaults to None
+        Returns:
+            Generator model
+        """
         input = Input(shape=input_shape, batch_size=self.batch_size)
         x = Dense(dim, activation='relu')(input)
         x = Dense(dim * 2, activation='relu')(x)
         x = Dense(dim * 4, activation='relu')(x)
         x = Dense(data_dim)(x)
         #if activation_info:
         #    x = GumbelSoftmaxActivation(activation_info, tau=tau)(x)
         return Model(inputs=input, outputs=x)
 
 class Critic(tf.keras.Model):
     def __init__(self, batch_size):
+        """Simple critic with dense feedforward and dropout layers.
+
+        Args:
+            batch_size (int): batch size
+        """
         self.batch_size = batch_size
 
     def build_model(self, input_shape, dim):
+        """Create model components.
+
+        Args:
+            input_shape: input dimensionality.
+            dim: hidden layers size.
+
+        Returns:
+            Critic model
+        """
         input = Input(shape=input_shape, batch_size=self.batch_size)
         x = Dense(dim * 4, activation='relu')(input)
         x = Dropout(0.1)(x)
         x = Dense(dim * 2, activation='relu')(x)
         x = Dropout(0.1)(x)
         x = Dense(dim, activation='relu')(x)
         x = Dense(1)(x)
```

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/regular/wgangp/model.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/regular/wgangp/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,42 +27,62 @@
         # WGAN-GP - WGAN with Gradient Penalty
         self.n_critic = n_critic
         self.n_generator = n_generator
         self.gradient_penalty_weight = gradient_penalty_weight
         super().__init__(model_parameters)
 
     def define_gan(self, activation_info: Optional[NamedTuple] = None):
+        """Define the trainable model components.
+
+        Args:
+            activation_info (Optional[NamedTuple], optional): Defaults to None.
+
+        Returns:
+            (generator_optimizer, critic_optimizer): Generator and critic optimizers.
+        """
         self.generator = Generator(self.batch_size). \
             build_model(input_shape=(self.noise_dim,), dim=self.layers_dim, data_dim=self.data_dim,
                         activation_info=activation_info, tau = self.tau)
 
         self.critic = Critic(self.batch_size). \
             build_model(input_shape=(self.data_dim,), dim=self.layers_dim)
 
         g_optimizer = Adam(self.g_lr, beta_1=self.beta_1, beta_2=self.beta_2)
         c_optimizer = Adam(self.d_lr, beta_1=self.beta_1, beta_2=self.beta_2)
         return g_optimizer, c_optimizer
 
     def gradient_penalty(self, real, fake):
+        """Compute gradient penalty.
+        
+        Args:
+            real: real event.
+            fake: fake event.
+        Returns:
+            gradient_penalty.
+        """
         epsilon = tf.random.uniform([real.shape[0], 1], minval=0.0, maxval=1.0, dtype=tf.dtypes.float32)
         x_hat = epsilon * real + (1 - epsilon) * fake
         with tf.GradientTape() as t:
             t.watch(x_hat)
             d_hat = self.critic(x_hat)
         gradients = t.gradient(d_hat, x_hat)
         ddx = tf.sqrt(tf.reduce_sum(gradients ** 2))
         d_regularizer = tf.reduce_mean((ddx - 1.0) ** 2)
         return d_regularizer
 
     @tf.function
     def update_gradients(self, x, g_optimizer, c_optimizer):
-        """
-        Compute the gradients for both the Generator and the Critic
-        :param x: real data event
-        :return: generator gradients, critic gradients
+        """Compute and apply the gradients for both the Generator and the Critic.
+
+        Args:
+            x: real data event
+            g_optimizer: generator optimizer
+            c_optimizer: critic optimizer
+        Returns:
+            (critic loss, generator loss)
         """
         for _ in range(self.n_critic):
             with tf.GradientTape() as d_tape:
                 critic_loss = self.c_lossfn(x)
             # Get the gradients of the critic
             d_gradient = d_tape.gradient(critic_loss, self.critic.trainable_variables)
             # Update the weights of the critic using the optimizer
@@ -81,16 +101,21 @@
             g_optimizer.apply_gradients(
                 zip(gen_gradients, self.generator.trainable_variables)
             )
 
         return critic_loss, gen_loss
 
     def c_lossfn(self, real):
-        """
-        passes through the network and computes the losses
+        """Compute critic loss.
+
+        Args:
+            real: real data
+
+        Returns:
+            critic loss
         """
         # generating noise from a uniform distribution
         noise = tf.random.normal([real.shape[0], self.noise_dim], dtype=tf.dtypes.float32)
         # run noise through generator
         fake = self.generator(noise)
         # discriminate x and x_gen
         logits_real = self.critic(real)
@@ -101,49 +126,75 @@
         # getting the loss of the critic.
         c_loss = (tf.reduce_mean(logits_fake)
                   - tf.reduce_mean(logits_real)
                   + gp * self.gradient_penalty_weight)
         return c_loss
 
     def g_lossfn(self, real):
-        """
-        :param real: Data batch we are analyzing
-        :return: Loss of the generator
+        """Compute generator loss.
+
+        Args:
+            real: A real sample
+            fake: A fake sample
+            fak2: A second fake sample
+
+        Returns:
+            Loss of the generator
         """
         # generating noise from a uniform distribution
         noise = tf.random.normal([real.shape[0], self.noise_dim], dtype=tf.dtypes.float32)
 
         fake = self.generator(noise)
         logits_fake = self.critic(fake)
         g_loss = -tf.reduce_mean(logits_fake)
         return g_loss
 
     def get_data_batch(self, train, batch_size, seed=0):
+        """Get real data batches from the passed data object.
+
+        Args:
+            train: real data.
+            batch_size: batch size.
+            seed (int, optional):Defaults to 0.
+
+        Returns:
+            data batch.
+        """
         # np.random.seed(seed)
         # x = train.loc[ np.random.choice(train.index, batch_size) ].values
         # iterate through shuffled indices, so every sample gets covered evenly
         start_i = (batch_size * seed) % len(train)
         stop_i = start_i + batch_size
         shuffle_seed = (batch_size * seed) // len(train)
         np.random.seed(shuffle_seed)
         train_ix = np.random.choice(train.shape[0], replace=False, size=len(train))  # wasteful to shuffle every time
         train_ix = list(train_ix) + list(train_ix)  # duplicate to cover ranges past the end of the set
         return train[train_ix[start_i: stop_i]]
 
     def train_step(self, train_data, optimizers):
+        """Perform a training step.
+
+        Args:
+            train_data: training data
+            optimizers: generator and critic optimizers 
+
+        Returns:
+            (critic_loss, generator_loss): Critic and generator loss.
+        """
         cri_loss, ge_loss = self.update_gradients(train_data, *optimizers)
         return cri_loss, ge_loss
 
     def fit(self, data, train_arguments: TrainParameters, num_cols: List[str], cat_cols: List[str]):
-        """
+        """Fit a synthesizer model to a given input dataset.
+
         Args:
-            data: A pandas DataFrame or a Numpy array with the data to be synthesized
+            data: A pandas DataFrame or a Numpy array with the data to be synthesized.
             train_arguments: GAN training arguments.
-            num_cols: List of columns of the data object to be handled as numerical
-            cat_cols: List of columns of the data object to be handled as categorical
+            num_cols (List[str]): List of columns of the data object to be handled as numerical.
+            cat_cols (List[str]): List of columns of the data object to be handled as categorical.
         """
         super().fit(data, num_cols, cat_cols)
 
         processed_data = self.processor.transform(data)
         self.data_dim = processed_data.shape[1]
         optimizers = self.define_gan(self.processor.col_transform_info)
 
@@ -171,31 +222,61 @@
                     model_checkpoint_base_name = './cache/' + train_arguments.cache_prefix + '_{}_model_weights_step_{}.h5'
                     self.generator.save_weights(model_checkpoint_base_name.format('generator', epoch))
                     self.critic.save_weights(model_checkpoint_base_name.format('critic', epoch))
 
 
 class Generator(tf.keras.Model):
     def __init__(self, batch_size):
+        """Simple generator with dense feedforward layers.
+
+        Args:
+            batch_size (int): batch size
+        """
         self.batch_size = batch_size
 
     def build_model(self, input_shape, dim, data_dim, activation_info: Optional[NamedTuple] = None, tau: Optional[float] = None):
+        """Create model components.
+
+        Args:
+            input_shape: input dimensionality.
+            dim: hidden layers dimensions.
+            data_dim: Output dimensionality.
+            activation_info (Optional[NamedTuple]): Defaults to None
+            tau (Optional[float]): Gumbel-Softmax non-negative temperature. Defaults to None
+        Returns:
+            Generator model
+        """
         input = Input(shape=input_shape, batch_size=self.batch_size)
         x = Dense(dim, activation='relu')(input)
         x = Dense(dim * 2, activation='relu')(x)
         x = Dense(dim * 4, activation='relu')(x)
         x = Dense(data_dim)(x)
         #if activation_info:
         #    x = GumbelSoftmaxActivation(activation_info, tau=tau)(x)
         return Model(inputs=input, outputs=x)
 
 class Critic(tf.keras.Model):
     def __init__(self, batch_size):
+        """Simple critic with dense feedforward and dropout layers.
+
+        Args:
+            batch_size (int): batch size
+        """
         self.batch_size = batch_size
 
     def build_model(self, input_shape, dim):
+        """Create model components.
+
+        Args:
+            input_shape: input dimensionality.
+            dim: hidden layers size.
+
+        Returns:
+            Critic model
+        """
         input = Input(shape=input_shape, batch_size=self.batch_size)
         x = Dense(dim * 4, activation='relu')(input)
         x = Dropout(0.1)(x)
         x = Dense(dim * 2, activation='relu')(x)
         x = Dropout(0.1)(x)
         x = Dense(dim, activation='relu')(x)
         x = Dense(1)(x)
```

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/saving_keras.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/saving_keras.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/synthesizers/timeseries/timegan/model.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/synthesizers/timeseries/timegan/model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """
     TimeGAN class implemented accordingly with:
     Original code can be found here: https://bitbucket.org/mvdschaar/mlforhealthlabpub/src/master/alg/timegan/
 """
-from tqdm import tqdm, trange
+from tqdm import tqdm
 import numpy as np
+from pandas import DataFrame
 
-from tensorflow import function, GradientTape, sqrt, abs, reduce_mean, ones_like, zeros_like, convert_to_tensor,float32
+from tensorflow import function, GradientTape, sqrt, abs, reduce_mean, ones_like, zeros_like, convert_to_tensor, float32
 from tensorflow import data as tfdata
 from tensorflow import nn
 from keras import (Model, Sequential, Input)
 from keras.layers import (GRU, LSTM, Dense)
 from keras.optimizers import Adam
 from keras.losses import (BinaryCrossentropy, MeanSquaredError)
 
-from ....synthesizers.base import BaseGANModel
+from ydata_synthetic.synthesizers.base import BaseGANModel, ModelParameters, TrainParameters
+from ydata_synthetic.preprocessing.timeseries.utils import real_data_loading
 
 def make_net(model, n_layers, hidden_units, output_units, net_type='GRU'):
     if net_type=='GRU':
         for i in range(n_layers):
             model.add(GRU(units=hidden_units,
                       return_sequences=True,
                       name=f'GRU_{i + 1}'))
@@ -31,22 +33,59 @@
                     activation='sigmoid',
                     name='OUT'))
     return model
 
 
 class TimeGAN(BaseGANModel):
 
-    __MODEL__='TimeGAN'
+    __MODEL__ = 'TimeGAN'
 
-    def __init__(self, model_parameters, hidden_dim, seq_len, n_seq, gamma):
-        self.seq_len=seq_len
-        self.n_seq=n_seq
-        self.hidden_dim=hidden_dim
-        self.gamma=gamma
+    def __init__(self, model_parameters: ModelParameters):
         super().__init__(model_parameters)
+        self.seq_len = None
+        self.n_seq = None
+        self.hidden_dim = model_parameters.latent_dim
+        self.gamma = model_parameters.gamma
+        self.num_cols = None
+
+    def fit(self, data: DataFrame,
+        train_arguments: TrainParameters,
+        num_cols: list[str] | None = None,
+        cat_cols: list[str] | None = None):
+        """
+        Fits the TimeGAN model.
+
+        Args:
+            data: A pandas DataFrame with the data to be synthesized.
+            train_arguments: TimeGAN training arguments.
+            num_cols: List of columns to be handled as numerical
+            cat_cols: List of columns to be handled as categorical
+        """
+        super().fit(data=data, num_cols=num_cols, cat_cols=cat_cols, train_arguments=train_arguments)
+        if cat_cols:
+            raise NotImplementedError("TimeGAN does not support categorical features.")
+        self.num_cols = num_cols
+        self.seq_len = train_arguments.sequence_length
+        self.n_seq = train_arguments.number_sequences
+        processed_data = real_data_loading(data[self.num_cols].values, seq_len=self.seq_len)
+        self.train(data=processed_data, train_steps=train_arguments.epochs)
+
+    def sample(self, n_samples: int):
+        """
+        Samples new data from the TimeGAN.
+
+        Args:
+            n_samples: Number of samples to be generated.
+        """
+        Z_ = next(self.get_batch_noise(size=n_samples))
+        records = self.generator(Z_)
+        data = []
+        for i in range(records.shape[0]):
+            data.append(DataFrame(records[i], columns=self.num_cols))
+        return data
 
     def define_gan(self):
         self.generator_aux=Generator(self.hidden_dim).build()
         self.supervisor=Supervisor(self.hidden_dim).build()
         self.discriminator=Discriminator(self.hidden_dim).build()
         self.recovery = Recovery(self.hidden_dim, self.n_seq).build()
         self.embedder = Embedder(self.hidden_dim).build()
@@ -216,17 +255,17 @@
                                 .shuffle(buffer_size=n_windows)
                                 .batch(self.batch_size).repeat())
 
     def _generate_noise(self):
         while True:
             yield np.random.uniform(low=0, high=1, size=(self.seq_len, self.n_seq))
 
-    def get_batch_noise(self):
+    def get_batch_noise(self, size=None):
         return iter(tfdata.Dataset.from_generator(self._generate_noise, output_types=float32)
-                                .batch(self.batch_size)
+                                .batch(self.batch_size if size is None else size)
                                 .repeat())
 
     def train(self, data, train_steps):
         # Assemble the model
         self.define_gan()
 
         ## Embedding network training
@@ -266,23 +305,14 @@
 
             X_ = next(self.get_batch_data(data, n_windows=len(data)))
             Z_ = next(self.get_batch_noise())
             step_d_loss = self.discriminator_loss(X_, Z_)
             if step_d_loss > 0.15:
                 step_d_loss = self.train_discriminator(X_, Z_, discriminator_opt)
 
-    def sample(self, n_samples):
-        steps = n_samples // self.batch_size + 1
-        data = []
-        for _ in trange(steps, desc='Synthetic data generation'):
-            Z_ = next(self.get_batch_noise())
-            records = self.generator(Z_)
-            data.append(records)
-        return np.array(np.vstack(data))
-
 
 class Generator(Model):
     def __init__(self, hidden_dim, net_type='GRU'):
         self.hidden_dim = hidden_dim
         self.net_type = net_type
 
     def build(self):
```

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_activation.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_activation.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_layer.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_layer.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/tests/preprocessing/test_regular_data_processor.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/tests/preprocessing/test_regular_data_processor.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/utils/cache.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/utils/gumbel_softmax.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/utils/gumbel_softmax.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic/utils/misc/colormaps.py` & `ydata-synthetic-1.3.0/src/ydata_synthetic/utils/misc/colormaps.py`

 * *Files identical despite different names*

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic.egg-info/PKG-INFO` & `ydata-synthetic-1.3.0/src/ydata_synthetic.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ydata-synthetic
-Version: 1.2.0
+Version: 1.3.0
 Summary: Synthetic data generation methods with different synthetization methods.
 Home-page: https://github.com/ydataai/ydata-synthetic
 Author: YData
 Author-email: community@ydata.ai
 License: https://github.com/ydataai/ydata-synthetic/blob/master/LICENSE
 Description: ![](https://img.shields.io/github/workflow/status/ydataai/ydata-synthetic/prerelease)
         ![](https://img.shields.io/pypi/status/ydata-synthetic)
         [![](https://pepy.tech/badge/ydata-synthetic)](https://pypi.org/project/ydata-synthetic/)
         ![](https://img.shields.io/badge/python-3.9%20%7C%203.10-blue)
         [![](https://img.shields.io/pypi/v/ydata-synthetic)](https://pypi.org/project/ydata-synthetic/)
         ![](https://img.shields.io/github/license/ydataai/ydata-synthetic)
         
-        <p align="center"><img width="200" src="https://user-images.githubusercontent.com/3348134/177604157-11181f6c-57e5-44b1-8f6c-774edbba5512.png" alt="Synthetic Data Logo"></p>
+        <p align="center"><img width="300" src="https://assets.ydata.ai/oss/ydata-synthetic_black.png" alt="YData Synthetic Logo"></p>
         
-        Join us on [![Discord](https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/mw7xjJ7b7s)
+        Join us on [![Discord](https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white)](https://tiny.ydata.ai/dcai-ydata-synthetic)
         
         # YData Synthetic
         A package to generate synthetic tabular and time-series data leveraging the state of the art generative models.
         
         ## 🎊 The exciting features:
         > These are must try features when it comes to synthetic data generation:
           > - A new streamlit app that delivers the synthetic data generation experience with a UI interface. A low code experience for the quick generation of synthetic data
@@ -33,14 +33,19 @@
         ### Why Synthetic Data?
         Synthetic data can be used for many applications:
           - Privacy compliance for data-sharing and Machine Learning development
           - Remove bias
           - Balance datasets
           - Augment datasets
         
+        > **Looking for an end-to-end solution to Synthetic Data Generation?**<br>
+        > [YData Fabric](https://ydata.ai/products/synthetic_data) enables the generation of high-quality datasets within a full UI experience, from data preparation to synthetic data generation and evaluation.<br>
+        > Check out the [Community Version](https://ydata.ai/ydata-fabric-free-trial).
+        
+        
         # ydata-synthetic
         This repository contains material related with architectures and models for synthetic data, from Generative Adversarial Networks (GANs) to Gaussian Mixtures.
         The repo includes a full ecosystem for synthetic data generation, that includes different models for the generation of synthetic structure data and time-series.
         All the Deep Learning models are implemented leveraging Tensorflow 2.0.
         Several example Jupyter Notebooks and Python scripts are included, to show how to use the different architectures.
         
         Are you ready to learn more about synthetic data and the bext-practices for synthetic data generation?
@@ -119,23 +124,27 @@
           - [Cramer GAN (The Cramer Distance as a Solution to Biased Wasserstein Gradients)](https://arxiv.org/abs/1705.10743)
           - [CWGAN-GP (Conditional Wassertein GAN with Gradient Penalty)](https://cameronfabbri.github.io/papers/conditionalWGAN.pdf)
           - [CTGAN (Conditional Tabular GAN)](https://arxiv.org/pdf/1907.00503.pdf)
           - [Gaussian Mixture](https://towardsdatascience.com/gaussian-mixture-models-explained-6986aaf5a95)
         
         ### Sequential data
           - [TimeGAN](https://papers.nips.cc/paper/2019/file/c9efe5f26cd17ba6216bbe2a7d26d490-Paper.pdf)
+          - [DoppelGANger](https://dl.acm.org/doi/pdf/10.1145/3419394.3423643)
         
         ## Contributing
         We are open to collaboration! If you want to start contributing you only need to:
           1. Search for an issue in which you would like to work. Issues for newcomers are labeled with good first issue.
           2. Create a PR solving the issue.
           3. We would review every PRs and either accept or ask for revisions.
         
         ## Support
-        For support in using this library, please join our Discord server. Our Discord community is very friendly and great about quickly answering questions about the use and development of the library. [Click here to join our Discord community!](https://discord.com/invite/mw7xjJ7b7s)
+        For support in using this library, please join our Discord server. Our Discord community is very friendly and great about quickly answering questions about the use and development of the library. [Click here to join our Discord community!](https://tiny.ydata.ai/dcai-ydata-synthetic)
+        
+        ## FAQs
+        Have a question? Check out the [Frequently Asked Questions](https://ydata.ai/resources/10-most-asked-questions-on-ydata-synthetic) about `ydata-synthetic`. If you feel something is missing, feel free to [book a beary informal chat with us](https://meetings.hubspot.com/fabiana-clemente).
         
         ## License
         [MIT License](https://github.com/ydataai/ydata-synthetic/blob/master/LICENSE)
         
 Keywords: data science ydata
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ydata-synthetic-1.2.0/src/ydata_synthetic.egg-info/SOURCES.txt` & `ydata-synthetic-1.3.0/src/ydata_synthetic.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 VERSION
+requirements-docs.txt
 requirements.txt
 setup.py
 src/ydata_synthetic/__init__.py
 src/ydata_synthetic/version.py
 src/ydata_synthetic.egg-info/PKG-INFO
 src/ydata_synthetic.egg-info/SOURCES.txt
 src/ydata_synthetic.egg-info/dependency_links.txt
@@ -15,14 +16,15 @@
 src/ydata_synthetic/postprocessing/regular/inverse_preprocesser.py
 src/ydata_synthetic/preprocessing/__init__.py
 src/ydata_synthetic/preprocessing/base_processor.py
 src/ydata_synthetic/preprocessing/regular/__init__.py
 src/ydata_synthetic/preprocessing/regular/ctgan_processor.py
 src/ydata_synthetic/preprocessing/regular/processor.py
 src/ydata_synthetic/preprocessing/timeseries/__init__.py
+src/ydata_synthetic/preprocessing/timeseries/doppelganger_processor.py
 src/ydata_synthetic/preprocessing/timeseries/stock.py
 src/ydata_synthetic/preprocessing/timeseries/timeseries_processor.py
 src/ydata_synthetic/preprocessing/timeseries/utils.py
 src/ydata_synthetic/streamlit_app/About.py
 src/ydata_synthetic/streamlit_app/__init__.py
 src/ydata_synthetic/streamlit_app/run.py
 src/ydata_synthetic/streamlit_app/pages/1_Train_a_synthesizer.py
@@ -53,14 +55,19 @@
 src/ydata_synthetic/synthesizers/regular/vanillagan/__init__.py
 src/ydata_synthetic/synthesizers/regular/vanillagan/model.py
 src/ydata_synthetic/synthesizers/regular/wgan/__init__.py
 src/ydata_synthetic/synthesizers/regular/wgan/model.py
 src/ydata_synthetic/synthesizers/regular/wgangp/__init__.py
 src/ydata_synthetic/synthesizers/regular/wgangp/model.py
 src/ydata_synthetic/synthesizers/timeseries/__init__.py
+src/ydata_synthetic/synthesizers/timeseries/model.py
+src/ydata_synthetic/synthesizers/timeseries/doppelganger/__init__.py
+src/ydata_synthetic/synthesizers/timeseries/doppelganger/doppelganger.py
+src/ydata_synthetic/synthesizers/timeseries/doppelganger/model.py
+src/ydata_synthetic/synthesizers/timeseries/doppelganger/network.py
 src/ydata_synthetic/synthesizers/timeseries/timegan/__init__.py
 src/ydata_synthetic/synthesizers/timeseries/timegan/model.py
 src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_activation.py
 src/ydata_synthetic/tests/custom_layers/test_gumbel_softmax_layer.py
 src/ydata_synthetic/tests/preprocessing/test_regular_data_processor.py
 src/ydata_synthetic/utils/__init__.py
 src/ydata_synthetic/utils/cache.py
```

