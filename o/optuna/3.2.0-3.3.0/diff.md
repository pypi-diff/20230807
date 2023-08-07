# Comparing `tmp/optuna-3.2.0.tar.gz` & `tmp/optuna-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optuna-3.2.0.tar", last modified: Tue May 30 06:00:24 2023, max compression
+gzip compressed data, was "optuna-3.3.0.tar", last modified: Mon Aug  7 07:14:14 2023, max compression
```

## Comparing `optuna-3.2.0.tar` & `optuna-3.3.0.tar`

### file list

```diff
@@ -1,253 +1,266 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.305794 optuna-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-30 06:00:03.000000 optuna-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 06:00:03.000000 optuna-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13543 2023-05-30 06:00:24.305794 optuna-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-05-30 06:00:03.000000 optuna-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.281793 optuna-3.2.0/optuna/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/_convert_positional_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/_experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.281793 optuna-3.2.0/optuna/_hypervolume/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/_hypervolume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/_hypervolume/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/_hypervolume/hssp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/_hypervolume/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/_hypervolume/wfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    12143 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    36886 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    28140 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.281793 optuna-3.2.0/optuna/importance/
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/importance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/importance/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.281793 optuna-3.2.0/optuna/importance/_fanova/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/importance/_fanova/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/importance/_fanova/_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/importance/_fanova/_fanova.py
--rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/importance/_fanova/_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/importance/_mean_decrease_impurity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.285794 optuna-3.2.0/optuna/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.285794 optuna-3.2.0/optuna/integration/_lightgbm_tuner/
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/_lightgbm_tuner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/_lightgbm_tuner/alias.py
--rw-r--r--   0 runner    (1001) docker     (123)    43823 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/_lightgbm_tuner/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/_lightgbm_tuner/sklearn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.285794 optuna-3.2.0/optuna/integration/allennlp/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/allennlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27848 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/botorch.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/catalyst.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/catboost.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/chainer.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/chainermn.py
--rw-r--r--   0 runner    (1001) docker     (123)    20578 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/cma.py
--rw-r--r--   0 runner    (1001) docker     (123)    27465 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/fastaiv1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/fastaiv2.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/mxnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12340 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/pytorch_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/pytorch_ignite.py
--rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/pytorch_lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/shap.py
--rw-r--r--   0 runner    (1001) docker     (123)    31393 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)    13925 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/skopt.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/skorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/tfkeras.py
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/wandb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/integration/xgboost.py
--rw-r--r--   0 runner    (1001) docker     (123)    10452 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.285794 optuna-3.2.0/optuna/multi_objective/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/multi_objective/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.289794 optuna-3.2.0/optuna/multi_objective/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/multi_objective/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/multi_objective/samplers/_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/multi_objective/samplers/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/multi_objective/samplers/_motpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    13788 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/multi_objective/samplers/_nsga2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/multi_objective/samplers/_random.py
--rw-r--r--   0 runner    (1001) docker     (123)    17554 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/multi_objective/study.py
--rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/multi_objective/trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.289794 optuna-3.2.0/optuna/multi_objective/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/multi_objective/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/multi_objective/visualization/_pareto_front.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/progress_bar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.289794 optuna-3.2.0/optuna/pruners/
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/pruners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/pruners/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/pruners/_hyperband.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/pruners/_median.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/pruners/_nop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/pruners/_patient.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/pruners/_percentile.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/pruners/_successive_halving.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/pruners/_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.289794 optuna-3.2.0/optuna/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_brute_force.py
--rw-r--r--   0 runner    (1001) docker     (123)    31522 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_cmaes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    26431 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_nsgaiii.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_partial_fixed.py
--rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_qmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.289794 optuna-3.2.0/optuna/samplers/_search_space/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_search_space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_search_space/intersection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.293794 optuna-3.2.0/optuna/samplers/_tpe/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_tpe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_tpe/_erf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_tpe/_truncnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_tpe/multi_objective_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_tpe/parzen_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_tpe/probability_distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)    34490 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/_tpe/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.293794 optuna-3.2.0/optuna/samplers/nsgaii/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/nsgaii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/nsgaii/_crossover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.293794 optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_blxalpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_sbx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_spx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_undx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_uniform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_vsbx.py
--rw-r--r--   0 runner    (1001) docker     (123)    22070 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/samplers/nsgaii/_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.293794 optuna-3.2.0/optuna/search_space/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/search_space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/search_space/group_decomposed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/search_space/intersection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.293794 optuna-3.2.0/optuna/storages/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19283 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_cached_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14429 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_in_memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.293794 optuna-3.2.0/optuna/storages/_journal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_journal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_journal/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_journal/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_journal/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)    25886 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_journal/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.293794 optuna-3.2.0/optuna/storages/_rdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.293794 optuna-3.2.0/optuna/storages/_rdb/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.297794 optuna-3.2.0/optuna/storages/_rdb/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v0.9.0.a.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v1.2.0.a.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v1.3.0.a.py
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v2.4.0.a.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v2.6.0.a_.py
--rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v3.0.0.a.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v3.0.0.b.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v3.0.0.c.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v3.0.0.d.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v3.2.0.a_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)    19476 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    48100 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/storages/_rdb/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.297794 optuna-3.2.0/optuna/study/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/study/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/study/_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/study/_frozen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/study/_multi_objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/study/_optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/study/_study_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/study/_study_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/study/_tell.py
--rw-r--r--   0 runner    (1001) docker     (123)    55112 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/study/study.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.297794 optuna-3.2.0/optuna/terminator/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/terminator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/terminator/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/terminator/erroreval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.297794 optuna-3.2.0/optuna/terminator/improvement/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/terminator/improvement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/terminator/improvement/_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/terminator/improvement/evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.297794 optuna-3.2.0/optuna/terminator/improvement/gp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/terminator/improvement/gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/terminator/improvement/gp/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/terminator/improvement/gp/botorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/terminator/terminator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.301794 optuna-3.2.0/optuna/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/testing/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/testing/objectives.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/testing/pruners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/testing/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/testing/storages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/testing/tempfile_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/testing/threading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/testing/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.301794 optuna-3.2.0/optuna/trial/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/trial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/trial/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/trial/_fixed.py
--rw-r--r--   0 runner    (1001) docker     (123)    19949 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/trial/_frozen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/trial/_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    29610 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/trial/_trial.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.301794 optuna-3.2.0/optuna/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13508 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_edf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_intermediate_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_optimization_history.py
--rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_parallel_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_param_importances.py
--rw-r--r--   0 runner    (1001) docker     (123)    17911 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_pareto_front.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_plotly_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    13138 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_terminator_improvement.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.305794 optuna-3.2.0/optuna/visualization/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_edf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_intermediate_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_matplotlib_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_optimization_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_parallel_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_param_importances.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_pareto_front.py
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_terminator_improvement.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-30 06:00:03.000000 optuna-3.2.0/optuna/visualization/matplotlib/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.281793 optuna-3.2.0/optuna.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13543 2023-05-30 06:00:24.000000 optuna-3.2.0/optuna.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-05-30 06:00:24.000000 optuna-3.2.0/optuna.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:00:24.000000 optuna-3.2.0/optuna.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-30 06:00:24.000000 optuna-3.2.0/optuna.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-30 06:00:24.000000 optuna-3.2.0/optuna.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 06:00:24.000000 optuna-3.2.0/optuna.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-30 06:00:03.000000 optuna-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-30 06:00:24.305794 optuna-3.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:00:24.305794 optuna-3.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-30 06:00:03.000000 optuna-3.2.0/tests/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    55669 2023-05-30 06:00:03.000000 optuna-3.2.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-30 06:00:03.000000 optuna-3.2.0/tests/test_convert_positional_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-05-30 06:00:03.000000 optuna-3.2.0/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)    23658 2023-05-30 06:00:03.000000 optuna-3.2.0/tests/test_distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-30 06:00:03.000000 optuna-3.2.0/tests/test_experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-30 06:00:03.000000 optuna-3.2.0/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-30 06:00:03.000000 optuna-3.2.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-30 06:00:03.000000 optuna-3.2.0/tests/test_multi_objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-05-30 06:00:03.000000 optuna-3.2.0/tests/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.113889 optuna-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-08-07 07:13:36.000000 optuna-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 07:13:36.000000 optuna-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13543 2023-08-07 07:14:14.113889 optuna-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-08-07 07:13:36.000000 optuna-3.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.069889 optuna-3.3.0/optuna/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/_convert_positional_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/_experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.069889 optuna-3.3.0/optuna/_hypervolume/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/_hypervolume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/_hypervolume/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/_hypervolume/hssp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/_hypervolume/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/_hypervolume/wfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12143 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.073889 optuna-3.3.0/optuna/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/artifacts/_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/artifacts/_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/artifacts/_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/artifacts/_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/artifacts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38354 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28140 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.073889 optuna-3.3.0/optuna/importance/
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/importance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/importance/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.073889 optuna-3.3.0/optuna/importance/_fanova/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/importance/_fanova/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/importance/_fanova/_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/importance/_fanova/_fanova.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/importance/_fanova/_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/importance/_mean_decrease_impurity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.081889 optuna-3.3.0/optuna/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.081889 optuna-3.3.0/optuna/integration/_lightgbm_tuner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/_lightgbm_tuner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/_lightgbm_tuner/alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45346 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/_lightgbm_tuner/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/_lightgbm_tuner/sklearn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.081889 optuna-3.3.0/optuna/integration/allennlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/allennlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34022 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/botorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/catalyst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/catboost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/chainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/chainermn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20578 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/cma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27465 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/fastaiv1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/fastaiv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/mxnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12340 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/pytorch_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/pytorch_ignite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/pytorch_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/shap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32582 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13925 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/skopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/skorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/tfkeras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/wandb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/integration/xgboost.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10452 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.081889 optuna-3.3.0/optuna/multi_objective/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/multi_objective/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.081889 optuna-3.3.0/optuna/multi_objective/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/multi_objective/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/multi_objective/samplers/_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/multi_objective/samplers/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/multi_objective/samplers/_motpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13788 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/multi_objective/samplers/_nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/multi_objective/samplers/_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17554 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/multi_objective/study.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/multi_objective/trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.085889 optuna-3.3.0/optuna/multi_objective/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/multi_objective/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/multi_objective/visualization/_pareto_front.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/progress_bar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.085889 optuna-3.3.0/optuna/pruners/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/pruners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/pruners/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/pruners/_hyperband.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/pruners/_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/pruners/_nop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/pruners/_patient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/pruners/_percentile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/pruners/_successive_halving.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/pruners/_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.089889 optuna-3.3.0/optuna/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/_brute_force.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32897 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/_cmaes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25190 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/_nsgaiii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/_partial_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/_qmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/_random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.089889 optuna-3.3.0/optuna/samplers/_search_space/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/_search_space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/_search_space/intersection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.089889 optuna-3.3.0/optuna/samplers/_tpe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/_tpe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/_tpe/_erf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/_tpe/_truncnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/_tpe/multi_objective_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/_tpe/parzen_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/_tpe/probability_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32884 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/_tpe/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.089889 optuna-3.3.0/optuna/samplers/nsgaii/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/nsgaii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/nsgaii/_after_trial_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/nsgaii/_child_generation_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/nsgaii/_crossover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.093889 optuna-3.3.0/optuna/samplers/nsgaii/_crossovers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/nsgaii/_crossovers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/nsgaii/_crossovers/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/nsgaii/_crossovers/_blxalpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/nsgaii/_crossovers/_sbx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/nsgaii/_crossovers/_spx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/nsgaii/_crossovers/_undx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/nsgaii/_crossovers/_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/nsgaii/_crossovers/_vsbx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/nsgaii/_dominates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/nsgaii/_elite_population_selection_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15941 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/samplers/nsgaii/_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.093889 optuna-3.3.0/optuna/search_space/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/search_space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/search_space/group_decomposed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/search_space/intersection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.093889 optuna-3.3.0/optuna/storages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19283 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_cached_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14377 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_in_memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.093889 optuna-3.3.0/optuna/storages/_journal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_journal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_journal/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_journal/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_journal/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25886 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_journal/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.097889 optuna-3.3.0/optuna/storages/_rdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_rdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.097889 optuna-3.3.0/optuna/storages/_rdb/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_rdb/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_rdb/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.097889 optuna-3.3.0/optuna/storages/_rdb/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_rdb/alembic/versions/v0.9.0.a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_rdb/alembic/versions/v1.2.0.a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_rdb/alembic/versions/v1.3.0.a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_rdb/alembic/versions/v2.4.0.a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_rdb/alembic/versions/v2.6.0.a_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_rdb/alembic/versions/v3.0.0.a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_rdb/alembic/versions/v3.0.0.b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_rdb/alembic/versions/v3.0.0.c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_rdb/alembic/versions/v3.0.0.d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_rdb/alembic/versions/v3.2.0.a_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_rdb/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    19476 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_rdb/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48189 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/storages/_rdb/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.101889 optuna-3.3.0/optuna/study/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/study/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/study/_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/study/_frozen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/study/_multi_objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/study/_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/study/_study_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/study/_study_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/study/_tell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55080 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/study/study.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.101889 optuna-3.3.0/optuna/terminator/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/terminator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/terminator/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/terminator/erroreval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.101889 optuna-3.3.0/optuna/terminator/improvement/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/terminator/improvement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/terminator/improvement/_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/terminator/improvement/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.101889 optuna-3.3.0/optuna/terminator/improvement/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/terminator/improvement/gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/terminator/improvement/gp/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/terminator/improvement/gp/botorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/terminator/terminator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.105889 optuna-3.3.0/optuna/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/testing/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/testing/objectives.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/testing/pruners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/testing/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/testing/storages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/testing/tempfile_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/testing/threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/testing/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.105889 optuna-3.3.0/optuna/trial/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/trial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/trial/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/trial/_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19949 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/trial/_frozen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/trial/_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29550 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/trial/_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.109889 optuna-3.3.0/optuna/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14077 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/_edf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/_hypervolume_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/_intermediate_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/_optimization_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/_parallel_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/_param_importances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17913 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/_pareto_front.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/_plotly_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13138 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/_terminator_improvement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/_timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.113889 optuna-3.3.0/optuna/visualization/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/matplotlib/_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/matplotlib/_edf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/matplotlib/_hypervolume_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/matplotlib/_intermediate_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/matplotlib/_matplotlib_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/matplotlib/_optimization_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/matplotlib/_parallel_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/matplotlib/_param_importances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/matplotlib/_pareto_front.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/matplotlib/_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/matplotlib/_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/matplotlib/_terminator_improvement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/matplotlib/_timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-08-07 07:13:36.000000 optuna-3.3.0/optuna/visualization/matplotlib/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.069889 optuna-3.3.0/optuna.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13543 2023-08-07 07:14:14.000000 optuna-3.3.0/optuna.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-08-07 07:14:14.000000 optuna-3.3.0/optuna.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 07:14:14.000000 optuna-3.3.0/optuna.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-07 07:14:14.000000 optuna-3.3.0/optuna.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-07 07:14:14.000000 optuna-3.3.0/optuna.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-07 07:14:14.000000 optuna-3.3.0/optuna.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-08-07 07:13:36.000000 optuna-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-07 07:14:14.117889 optuna-3.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 07:14:14.113889 optuna-3.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-07 07:13:36.000000 optuna-3.3.0/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58314 2023-08-07 07:13:36.000000 optuna-3.3.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-08-07 07:13:36.000000 optuna-3.3.0/tests/test_convert_positional_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-08-07 07:13:36.000000 optuna-3.3.0/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23658 2023-08-07 07:13:36.000000 optuna-3.3.0/tests/test_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-08-07 07:13:36.000000 optuna-3.3.0/tests/test_experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-07 07:13:36.000000 optuna-3.3.0/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-08-07 07:13:36.000000 optuna-3.3.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-08-07 07:13:36.000000 optuna-3.3.0/tests/test_multi_objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-08-07 07:13:36.000000 optuna-3.3.0/tests/test_transform.py
```

### Comparing `optuna-3.2.0/LICENSE` & `optuna-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/PKG-INFO` & `optuna-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optuna
-Version: 3.2.0
+Version: 3.3.0
 Summary: A hyperparameter optimization framework
 Author: Takuya Akiba
 Author-email: akiba@preferred.jp
 License: MIT License
         
         Copyright (c) 2018 Preferred Networks, Inc.
```

### Comparing `optuna-3.2.0/README.md` & `optuna-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/__init__.py` & `optuna-3.3.0/optuna/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 
 __all__ = [
     "Study",
     "Trial",
     "TrialPruned",
     "__version__",
+    "artifacts",
     "copy_study",
     "create_study",
     "create_trial",
     "delete_study",
     "distributions",
     "exceptions",
     "get_all_study_summaries",
@@ -47,9 +48,10 @@
     "study",
     "trial",
     "version",
     "visualization",
 ]
 
 
+artifacts = _LazyImport("optuna.artifacts")
 importance = _LazyImport("optuna.importance")
 visualization = _LazyImport("optuna.visualization")
```

### Comparing `optuna-3.2.0/optuna/_callbacks.py` & `optuna-3.3.0/optuna/_callbacks.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/_convert_positional_args.py` & `optuna-3.3.0/optuna/_convert_positional_args.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/_deprecated.py` & `optuna-3.3.0/optuna/_deprecated.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/_experimental.py` & `optuna-3.3.0/optuna/_experimental.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/_hypervolume/base.py` & `optuna-3.3.0/optuna/_hypervolume/base.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/_hypervolume/hssp.py` & `optuna-3.3.0/optuna/_hypervolume/hssp.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/_hypervolume/utils.py` & `optuna-3.3.0/optuna/_hypervolume/utils.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/_hypervolume/wfg.py` & `optuna-3.3.0/optuna/_hypervolume/wfg.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/_imports.py` & `optuna-3.3.0/optuna/_imports.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/_transform.py` & `optuna-3.3.0/optuna/_transform.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/cli.py` & `optuna-3.3.0/optuna/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,20 +17,25 @@
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Type
 from typing import Union
 import warnings
 
+import sqlalchemy.exc
 import yaml
 
 import optuna
 from optuna._imports import _LazyImport
 from optuna.exceptions import CLIUsageError
 from optuna.exceptions import ExperimentalWarning
+from optuna.storages import BaseStorage
+from optuna.storages import JournalFileStorage
+from optuna.storages import JournalRedisStorage
+from optuna.storages import JournalStorage
 from optuna.storages import RDBStorage
 from optuna.trial import TrialState
 
 
 _dataframe = _LazyImport("optuna.study._dataframe")
 
 _DATETIME_FORMAT = "%Y-%m-%d %H:%M:%S"
@@ -47,14 +52,35 @@
             " is an experimental feature. The interface can change in the future.",
             ExperimentalWarning,
         )
         return env_storage
     raise CLIUsageError("Storage URL is not specified.")
 
 
+def _get_storage(storage_url: Optional[str], storage_class: Optional[str]) -> BaseStorage:
+    storage_url = _check_storage_url(storage_url)
+    if storage_class:
+        if storage_class == JournalRedisStorage.__name__:
+            return JournalStorage(JournalRedisStorage(storage_url))
+        if storage_class == JournalFileStorage.__name__:
+            return JournalStorage(JournalFileStorage(storage_url))
+        if storage_class == RDBStorage.__name__:
+            return RDBStorage(storage_url)
+        raise CLIUsageError("Unsupported storage class")
+
+    if storage_url.startswith("redis"):
+        return JournalStorage(JournalRedisStorage(storage_url))
+    if os.path.isfile(storage_url):
+        return JournalStorage(JournalFileStorage(storage_url))
+    try:
+        return RDBStorage(storage_url)
+    except sqlalchemy.exc.ArgumentError:
+        raise CLIUsageError("Failed to guess storage class from storage_url")
+
+
 def _format_value(value: Any) -> Any:
     #  Format value that can be serialized to JSON or YAML.
     if value is None or isinstance(value, (int, float)):
         return value
     elif isinstance(value, datetime.datetime):
         return value.strftime(_DATETIME_FORMAT)
     elif isinstance(value, list):
@@ -289,16 +315,15 @@
             help="Set directions of optimization to a new study."
             " Put whitespace between directions. Each direction should be"
             ' either "minimize" or "maximize".',
             nargs="+",
         )
 
     def take_action(self, parsed_args: Namespace) -> int:
-        storage_url = _check_storage_url(parsed_args.storage)
-        storage = optuna.storages.get_storage(storage_url)
+        storage = _get_storage(parsed_args.storage, parsed_args.storage_class)
         study_name = optuna.create_study(
             storage=storage,
             study_name=parsed_args.study_name,
             direction=parsed_args.direction,
             directions=parsed_args.directions,
             load_if_exists=parsed_args.skip_if_exists,
         ).study_name
@@ -309,16 +334,15 @@
 class _DeleteStudy(_BaseCommand):
     """Delete a specified study."""
 
     def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument("--study-name", default=None, help="The name of the study to delete.")
 
     def take_action(self, parsed_args: Namespace) -> int:
-        storage_url = _check_storage_url(parsed_args.storage)
-        storage = optuna.storages.get_storage(storage_url)
+        storage = _get_storage(parsed_args.storage, parsed_args.storage_class)
         study_id = storage.get_study_id_from_name(parsed_args.study_name)
         storage.delete_study(study_id)
         return 0
 
 
 class _StudySetUserAttribute(_BaseCommand):
     """Set a user attribute to a study."""
@@ -332,27 +356,27 @@
             default=None,
             help="The name of the study to set the user attribute to.",
         )
         parser.add_argument("--key", "-k", required=True, help="Key of the user attribute.")
         parser.add_argument("--value", required=True, help="Value to be set.")
 
     def take_action(self, parsed_args: Namespace) -> int:
-        storage_url = _check_storage_url(parsed_args.storage)
+        storage = _get_storage(parsed_args.storage, parsed_args.storage_class)
 
         if parsed_args.study and parsed_args.study_name:
             raise ValueError(
                 "Both `--study-name` and the deprecated `--study` was specified. "
                 "Please remove the `--study` flag."
             )
         elif parsed_args.study:
             message = "The use of `--study` is deprecated. Please use `--study-name` instead."
             warnings.warn(message, FutureWarning)
-            study = optuna.load_study(storage=storage_url, study_name=parsed_args.study)
+            study = optuna.load_study(storage=storage, study_name=parsed_args.study)
         elif parsed_args.study_name:
-            study = optuna.load_study(storage=storage_url, study_name=parsed_args.study_name)
+            study = optuna.load_study(storage=storage, study_name=parsed_args.study_name)
         else:
             raise ValueError("Missing study name. Please use `--study-name`.")
 
         study.set_user_attr(parsed_args.key, parsed_args.value)
 
         self.logger.info("Attribute successfully written.")
         return 0
@@ -381,16 +405,16 @@
             "--flatten",
             default=False,
             action="store_true",
             help="Flatten nested columns such as directions.",
         )
 
     def take_action(self, parsed_args: Namespace) -> int:
-        storage_url = _check_storage_url(parsed_args.storage)
-        summaries = optuna.get_all_study_summaries(storage_url, include_best_trial=False)
+        storage = _get_storage(parsed_args.storage, parsed_args.storage_class)
+        summaries = optuna.get_all_study_summaries(storage, include_best_trial=False)
 
         records = []
         for s in summaries:
             start = (
                 s.datetime_start.strftime(_DATETIME_FORMAT)
                 if s.datetime_start is not None
                 else None
@@ -440,16 +464,16 @@
 
     def take_action(self, parsed_args: Namespace) -> int:
         warnings.warn(
             "'trials' is an experimental CLI command. The interface can change in the future.",
             ExperimentalWarning,
         )
 
-        storage_url = _check_storage_url(parsed_args.storage)
-        study = optuna.load_study(storage=storage_url, study_name=parsed_args.study_name)
+        storage = _get_storage(parsed_args.storage, parsed_args.storage_class)
+        study = optuna.load_study(storage=storage, study_name=parsed_args.study_name)
         attrs = (
             "number",
             "value" if not study._is_multi_objective() else "values",
             "datetime_start",
             "datetime_complete",
             "duration",
             "params",
@@ -490,16 +514,16 @@
 
     def take_action(self, parsed_args: Namespace) -> int:
         warnings.warn(
             "'best-trial' is an experimental CLI command. The interface can change in the future.",
             ExperimentalWarning,
         )
 
-        storage_url = _check_storage_url(parsed_args.storage)
-        study = optuna.load_study(storage=storage_url, study_name=parsed_args.study_name)
+        storage = _get_storage(parsed_args.storage, parsed_args.storage_class)
+        study = optuna.load_study(storage=storage, study_name=parsed_args.study_name)
         attrs = (
             "number",
             "value" if not study._is_multi_objective() else "values",
             "datetime_start",
             "datetime_complete",
             "duration",
             "params",
@@ -544,16 +568,16 @@
     def take_action(self, parsed_args: Namespace) -> int:
         warnings.warn(
             "'best-trials' is an experimental CLI command. The interface can change in the "
             "future.",
             ExperimentalWarning,
         )
 
-        storage_url = _check_storage_url(parsed_args.storage)
-        study = optuna.load_study(storage=storage_url, study_name=parsed_args.study_name)
+        storage = _get_storage(parsed_args.storage, parsed_args.storage_class)
+        study = optuna.load_study(storage=storage, study_name=parsed_args.study_name)
         best_trials = [trial.number for trial in study.best_trials]
         attrs = (
             "number",
             "value" if not study._is_multi_objective() else "values",
             "datetime_start",
             "datetime_complete",
             "duration",
@@ -609,27 +633,27 @@
     def take_action(self, parsed_args: Namespace) -> int:
         message = (
             "The use of the `study optimize` command is deprecated. Please execute your Python "
             "script directly instead."
         )
         warnings.warn(message, FutureWarning)
 
-        storage_url = _check_storage_url(parsed_args.storage)
+        storage = _get_storage(parsed_args.storage, parsed_args.storage_class)
 
         if parsed_args.study and parsed_args.study_name:
             raise ValueError(
                 "Both `--study-name` and the deprecated `--study` was specified. "
                 "Please remove the `--study` flag."
             )
         elif parsed_args.study:
             message = "The use of `--study` is deprecated. Please use `--study-name` instead."
             warnings.warn(message, FutureWarning)
-            study = optuna.load_study(storage=storage_url, study_name=parsed_args.study)
+            study = optuna.load_study(storage=storage, study_name=parsed_args.study)
         elif parsed_args.study_name:
-            study = optuna.load_study(storage=storage_url, study_name=parsed_args.study_name)
+            study = optuna.load_study(storage=storage, study_name=parsed_args.study_name)
         else:
             raise ValueError("Missing study name. Please use `--study-name`.")
 
         # We force enabling the debug flag. As we are going to execute user codes, we want to show
         # exception stack traces by default.
         parsed_args.debug = True
 
@@ -652,22 +676,25 @@
             timeout=parsed_args.timeout,
             n_jobs=parsed_args.n_jobs,
         )
         return 0
 
 
 class _StorageUpgrade(_BaseCommand):
-    """Upgrade the schema of a storage."""
+    """Upgrade the schema of an RDB storage."""
 
     def take_action(self, parsed_args: Namespace) -> int:
         storage_url = _check_storage_url(parsed_args.storage)
-        if storage_url.startswith("redis"):
-            self.logger.info("This storage does not support upgrade yet.")
+        try:
+            storage = RDBStorage(
+                storage_url, skip_compatibility_check=True, skip_table_creation=True
+            )
+        except sqlalchemy.exc.ArgumentError:
+            self.logger.error("Invalid RDBStorage URL.")
             return 1
-        storage = RDBStorage(storage_url, skip_compatibility_check=True, skip_table_creation=True)
         current_version = storage.get_current_version()
         head_version = storage.get_head_version()
         known_versions = storage.get_all_versions()
         if current_version == head_version:
             self.logger.info("This storage is up-to-date.")
         elif current_version in known_versions:
             self.logger.info("Upgrading the storage schema to the latest version.")
@@ -737,18 +764,18 @@
 
     def take_action(self, parsed_args: Namespace) -> int:
         warnings.warn(
             "'ask' is an experimental CLI command. The interface can change in the future.",
             ExperimentalWarning,
         )
 
-        storage_url = _check_storage_url(parsed_args.storage)
+        storage = _get_storage(parsed_args.storage, parsed_args.storage_class)
 
         create_study_kwargs = {
-            "storage": storage_url,
+            "storage": storage,
             "study_name": parsed_args.study_name,
             "direction": parsed_args.direction,
             "directions": parsed_args.directions,
             "load_if_exists": True,
         }
 
         if parsed_args.direction is not None or parsed_args.directions is not None:
@@ -855,18 +882,18 @@
 
     def take_action(self, parsed_args: Namespace) -> int:
         warnings.warn(
             "'tell' is an experimental CLI command. The interface can change in the future.",
             ExperimentalWarning,
         )
 
-        storage_url = _check_storage_url(parsed_args.storage)
+        storage = _get_storage(parsed_args.storage, parsed_args.storage_class)
 
         study = optuna.load_study(
-            storage=storage_url,
+            storage=storage,
             study_name=parsed_args.study_name,
         )
 
         if parsed_args.state is not None:
             state: Optional[TrialState] = TrialState[parsed_args.state.upper()]
         else:
             state = None
@@ -906,14 +933,24 @@
         "--storage",
         default=None,
         help=(
             "DB URL. (e.g. sqlite:///example.db) "
             "Also can be specified via OPTUNA_STORAGE environment variable."
         ),
     )
+    parser.add_argument(
+        "--storage-class",
+        help="Storage class hint (e.g. JournalFileStorage)",
+        default=None,
+        choices=[
+            RDBStorage.__name__,
+            JournalFileStorage.__name__,
+            JournalRedisStorage.__name__,
+        ],
+    )
     verbose_group = parser.add_mutually_exclusive_group()
     verbose_group.add_argument(
         "-v",
         "--verbose",
         action="count",
         dest="verbose_level",
         default=1,
```

### Comparing `optuna-3.2.0/optuna/distributions.py` & `optuna-3.3.0/optuna/distributions.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/exceptions.py` & `optuna-3.3.0/optuna/exceptions.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/importance/__init__.py` & `optuna-3.3.0/optuna/importance/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from collections import OrderedDict
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 import warnings
 
 from optuna.exceptions import ExperimentalWarning
@@ -31,16 +30,15 @@
 ) -> Dict[str, float]:
     """Evaluate parameter importances based on completed trials in the given study.
 
     The parameter importances are returned as a dictionary where the keys consist of parameter
     names and their values importances.
     The importances are represented by non-negative floating point numbers, where higher values
     mean that the parameters are more important.
-    The returned dictionary is of type :class:`collections.OrderedDict` and is ordered by
-    its values in a descending order.
+    The returned dictionary is ordered by its values in a descending order.
     By default, the sum of the importance values are normalized to 1.0.
 
     If ``params`` is :obj:`None`, all parameter that are present in all of the completed trials are
     assessed.
     This implies that conditional parameters will be excluded from the evaluation.
     To assess the importances of conditional parameters, a :obj:`list` of parameter names can be
     specified via ``params``.
@@ -86,32 +84,31 @@
 
             .. note::
                 Added in v3.0.0 as an experimental feature. The interface may change in newer
                 versions without prior notice. See
                 https://github.com/optuna/optuna/releases/tag/v3.0.0.
 
     Returns:
-        An :class:`collections.OrderedDict` where the keys are parameter names and the values are
-        assessed importances.
+        A :obj:`dict` where the keys are parameter names and the values are assessed importances.
 
     """
     if evaluator is None:
         evaluator = FanovaImportanceEvaluator()
 
     if not isinstance(evaluator, BaseImportanceEvaluator):
         raise TypeError("Evaluator must be a subclass of BaseImportanceEvaluator.")
 
     res = evaluator.evaluate(study, params=params, target=target)
     if normalize:
         s = sum(res.values())
         if s == 0.0:
             n_params = len(res)
-            return OrderedDict((param, 1.0 / n_params) for param in res.keys())
+            return dict((param, 1.0 / n_params) for param in res.keys())
         else:
-            return OrderedDict((param, value / s) for (param, value) in res.items())
+            return dict((param, value / s) for (param, value) in res.items())
     else:
         warnings.warn(
             "`normalize` option is an experimental feature."
             " The interface can change in the future.",
             ExperimentalWarning,
         )
         return res
```

### Comparing `optuna-3.2.0/optuna/importance/_base.py` & `optuna-3.3.0/optuna/importance/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import abc
-from collections import OrderedDict
 from typing import Callable
 from typing import cast
 from typing import Collection
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
@@ -55,28 +54,28 @@
 
                 .. note::
                     Specify this argument if ``study`` is being used for multi-objective
                     optimization. For example, to get the hyperparameter importance of the first
                     objective, use ``target=lambda t: t.values[0]`` for the target parameter.
 
         Returns:
-            An :class:`collections.OrderedDict` where the keys are parameter names and the values
-            are assessed importances.
+            A :obj:`dict` where the keys are parameter names and the values are assessed
+            importances.
 
         """
         # TODO(hvy): Reconsider the interface as logic might violate DRY among multiple evaluators.
         raise NotImplementedError
 
 
 def _get_distributions(study: Study, params: Optional[List[str]]) -> Dict[str, BaseDistribution]:
     completed_trials = study.get_trials(deepcopy=False, states=(TrialState.COMPLETE,))
     _check_evaluate_args(completed_trials, params)
 
     if params is None:
-        return intersection_search_space(study.get_trials(deepcopy=False), ordered_dict=True)
+        return intersection_search_space(study.get_trials(deepcopy=False))
 
     # New temporary required to pass mypy. Seems like a bug.
     params_not_none = params
     assert params_not_none is not None
 
     # Compute the search space based on the subset of trials containing all parameters.
     distributions = None
@@ -100,15 +99,15 @@
         ):
             raise ValueError(
                 "Parameters importances cannot be assessed with dynamic search spaces if "
                 "parameters are specified. Specified parameters: {}.".format(params)
             )
 
     assert distributions is not None  # Required to pass mypy.
-    distributions = OrderedDict(
+    distributions = dict(
         sorted(distributions.items(), key=lambda name_and_distribution: name_and_distribution[0])
     )
     return distributions
 
 
 def _check_evaluate_args(completed_trials: List[FrozenTrial], params: Optional[List[str]]) -> None:
     if len(completed_trials) == 0:
@@ -168,14 +167,14 @@
 def _get_target_values(
     trials: List[FrozenTrial], target: Optional[Callable[[FrozenTrial], float]]
 ) -> numpy.ndarray:
     return numpy.array([target(trial) if target is not None else trial.value for trial in trials])
 
 
 def _sort_dict_by_importance(param_importances: Dict[str, float]) -> Dict[str, float]:
-    return OrderedDict(
+    return dict(
         reversed(
             sorted(
                 param_importances.items(), key=lambda name_and_importance: name_and_importance[1]
             )
         )
     )
```

### Comparing `optuna-3.2.0/optuna/importance/_fanova/_evaluator.py` & `optuna-3.3.0/optuna/importance/_fanova/_evaluator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from collections import OrderedDict
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 
 import numpy
 
@@ -102,15 +101,15 @@
             name: dist for name, dist in distributions.items() if not dist.single()
         }
         single_distributions = {
             name: dist for name, dist in distributions.items() if dist.single()
         }
 
         if len(non_single_distributions) == 0:
-            return OrderedDict()
+            return {}
 
         trials: List[FrozenTrial] = _get_filtered_trials(study, params=params, target=target)
 
         trans = _SearchSpaceTransform(
             non_single_distributions, transform_log=False, transform_step=False
         )
```

### Comparing `optuna-3.2.0/optuna/importance/_fanova/_fanova.py` & `optuna-3.3.0/optuna/importance/_fanova/_fanova.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/importance/_fanova/_tree.py` & `optuna-3.3.0/optuna/importance/_fanova/_tree.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/importance/_mean_decrease_impurity.py` & `optuna-3.3.0/optuna/importance/_mean_decrease_impurity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from collections import OrderedDict
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 
 import numpy
 
@@ -76,15 +75,15 @@
             )
 
         distributions = _get_distributions(study, params=params)
         if params is None:
             params = list(distributions.keys())
         assert params is not None
         if len(params) == 0:
-            return OrderedDict()
+            return {}
 
         trials: List[FrozenTrial] = _get_filtered_trials(study, params=params, target=target)
         trans = _SearchSpaceTransform(distributions, transform_log=False, transform_step=False)
         trans_params: numpy.ndarray = _get_trans_params(trials, trans)
         target_values: numpy.ndarray = _get_target_values(trials, target)
 
         forest = self._forest
```

### Comparing `optuna-3.2.0/optuna/integration/__init__.py` & `optuna-3.3.0/optuna/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/integration/_lightgbm_tuner/__init__.py` & `optuna-3.3.0/optuna/integration/_lightgbm_tuner/__init__.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/integration/_lightgbm_tuner/alias.py` & `optuna-3.3.0/optuna/integration/_lightgbm_tuner/alias.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/integration/_lightgbm_tuner/optimize.py` & `optuna-3.3.0/optuna/integration/_lightgbm_tuner/optimize.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
+from __future__ import annotations
+
 import abc
+from collections.abc import Callable
+from collections.abc import Container
+from collections.abc import Generator
+from collections.abc import Iterator
 import copy
 import json
 import os
 import pickle
 import time
 from typing import Any
-from typing import Callable
 from typing import cast
-from typing import Container
-from typing import Dict
-from typing import Generator
-from typing import Iterator
 from typing import List
-from typing import Optional
 from typing import Tuple
 from typing import Union
 import warnings
 
 import numpy as np
 import tqdm
 
@@ -60,16 +60,16 @@
 
 _logger = optuna.logging.get_logger(__name__)
 
 
 class _BaseTuner:
     def __init__(
         self,
-        lgbm_params: Optional[Dict[str, Any]] = None,
-        lgbm_kwargs: Optional[Dict[str, Any]] = None,
+        lgbm_params: dict[str, Any] | None = None,
+        lgbm_kwargs: dict[str, Any] | None = None,
     ) -> None:
         # Handling alias metrics.
         if lgbm_params is not None:
             _handling_alias_metrics(lgbm_params)
 
         self.lgbm_params = lgbm_params or {}
         self.lgbm_kwargs = lgbm_kwargs or {}
@@ -88,15 +88,15 @@
             raise NotImplementedError
         metric = self._metric_with_eval_at(metric)
 
         return metric
 
     def _get_booster_best_score(self, booster: "lgb.Booster") -> float:
         metric = self._get_metric_for_objective()
-        valid_sets: Optional[VALID_SET_TYPE] = self.lgbm_kwargs.get("valid_sets")
+        valid_sets: VALID_SET_TYPE | None = self.lgbm_kwargs.get("valid_sets")
 
         if self.lgbm_kwargs.get("valid_names") is not None:
             if type(self.lgbm_kwargs["valid_names"]) is str:
                 valid_name = self.lgbm_kwargs["valid_names"]
             elif type(self.lgbm_kwargs["valid_names"]) in [list, tuple]:
                 valid_name = self.lgbm_kwargs["valid_names"][-1]
             else:
@@ -151,32 +151,34 @@
 
 
 class _OptunaObjective(_BaseTuner):
     """Objective for hyperparameter-tuning with Optuna."""
 
     def __init__(
         self,
-        target_param_names: List[str],
-        lgbm_params: Dict[str, Any],
+        target_param_names: list[str],
+        lgbm_params: dict[str, Any],
         train_set: "lgb.Dataset",
-        lgbm_kwargs: Dict[str, Any],
+        lgbm_kwargs: dict[str, Any],
         best_score: float,
         step_name: str,
-        model_dir: Optional[str],
-        pbar: Optional[tqdm.tqdm] = None,
+        model_dir: str | None,
+        pbar: tqdm.tqdm | None = None,
     ):
         self.target_param_names = target_param_names
         self.pbar = pbar
         self.lgbm_params = lgbm_params
         self.lgbm_kwargs = lgbm_kwargs
         self.train_set = train_set
 
         self.trial_count = 0
         self.best_score = best_score
-        self.best_booster_with_trial_number: Optional[Tuple["lgb.Booster", int]] = None
+        self.best_booster_with_trial_number: tuple[
+            "lgb.Booster" | "lgb.CVBooster", int
+        ] | None = None
         self.step_name = step_name
         self.model_dir = model_dir
 
         self._check_target_names_supported()
         self.pbar_fmt = "{}, val_score: {:.6f}"
 
     def _check_target_names_supported(self) -> None:
@@ -275,37 +277,44 @@
 
         self.trial_count += 1
 
 
 class _OptunaObjectiveCV(_OptunaObjective):
     def __init__(
         self,
-        target_param_names: List[str],
-        lgbm_params: Dict[str, Any],
+        target_param_names: list[str],
+        lgbm_params: dict[str, Any],
         train_set: "lgb.Dataset",
-        lgbm_kwargs: Dict[str, Any],
+        lgbm_kwargs: dict[str, Any],
         best_score: float,
         step_name: str,
-        model_dir: Optional[str],
-        pbar: Optional[tqdm.tqdm] = None,
+        model_dir: str | None,
+        pbar: tqdm.tqdm | None = None,
     ):
         super().__init__(
             target_param_names,
             lgbm_params,
             train_set,
             lgbm_kwargs,
             best_score,
             step_name,
             model_dir,
             pbar=pbar,
         )
 
-    def _get_cv_scores(self, cv_results: Dict[str, List[float]]) -> List[float]:
+    def _get_cv_scores(self, cv_results: dict[str, list[float] | "lgb.CVBooster"]) -> list[float]:
         metric = self._get_metric_for_objective()
-        val_scores = cv_results["{}-mean".format(metric)]
+        metric_key = f"{metric}-mean"
+        # The prefix "valid " is added to metric name since LightGBM v4.0.0.
+        val_scores = (
+            cv_results[metric_key]
+            if metric_key in cv_results
+            else cv_results["valid " + metric_key]
+        )
+        assert not isinstance(val_scores, lgb.CVBooster)
         return val_scores
 
     def __call__(self, trial: optuna.trial.Trial) -> float:
         self._preprocess(trial)
 
         start_time = time.time()
         train_set = copy.copy(self.train_set)
@@ -318,20 +327,22 @@
 
         if self.model_dir is not None and self.lgbm_kwargs.get("return_cvbooster"):
             path = os.path.join(self.model_dir, "{}.pkl".format(trial.number))
             with open(path, "wb") as fout:
                 # At version `lightgbm==3.0.0`, :class:`lightgbm.CVBooster` does not
                 # have `__getstate__` which is required for pickle serialization.
                 cvbooster = cv_results["cvbooster"]
+                assert isinstance(cvbooster, lgb.CVBooster)
                 pickle.dump((cvbooster.boosters, cvbooster.best_iteration), fout)
             _logger.info("The booster of trial#{} was saved as {}.".format(trial.number, path))
 
         if self.compare_validation_metrics(val_score, self.best_score):
             self.best_score = val_score
             if self.lgbm_kwargs.get("return_cvbooster"):
+                assert not isinstance(cv_results["cvbooster"], list)
                 self.best_booster_with_trial_number = (cv_results["cvbooster"], trial.number)
 
         self._postprocess(trial, elapsed_secs, average_iteration_time)
 
         return val_score
 
 
@@ -341,62 +352,73 @@
     This class has common attributes and methods of
     :class:`~optuna.integration.lightgbm.LightGBMTuner` and
     :class:`~optuna.integration.lightgbm.LightGBMTunerCV`.
     """
 
     def __init__(
         self,
-        params: Dict[str, Any],
+        params: dict[str, Any],
         train_set: "lgb.Dataset",
+        callbacks: list[Callable[..., Any]],
         num_boost_round: int = 1000,
-        fobj: Optional[Callable[..., Any]] = None,
-        feval: Optional[Callable[..., Any]] = None,
+        fobj: Callable[..., Any] | None = None,
+        feval: Callable[..., Any] | None = None,
         feature_name: str = "auto",
         categorical_feature: str = "auto",
-        early_stopping_rounds: Optional[int] = None,
-        verbose_eval: Optional[Union[bool, int, str]] = None,
-        callbacks: Optional[List[Callable[..., Any]]] = None,
-        time_budget: Optional[int] = None,
-        sample_size: Optional[int] = None,
-        study: Optional[optuna.study.Study] = None,
-        optuna_callbacks: Optional[List[Callable[[Study, FrozenTrial], None]]] = None,
-        verbosity: Optional[int] = None,
+        early_stopping_rounds: int | None = None,
+        verbose_eval: bool | int | str | None = None,
+        time_budget: int | None = None,
+        sample_size: int | None = None,
+        study: optuna.study.Study | None = None,
+        optuna_callbacks: list[Callable[[Study, FrozenTrial], None]] | None = None,
+        verbosity: int | None = None,
         show_progress_bar: bool = True,
-        model_dir: Optional[str] = None,
+        model_dir: str | None = None,
         *,
-        optuna_seed: Optional[int] = None,
+        optuna_seed: int | None = None,
     ) -> None:
         _imports.check()
 
         params = copy.deepcopy(params)
+        if fobj is not None:
+            if "objective" not in params:
+                params["objective"] = fobj
+            else:
+                warnings.warn(
+                    "Objective function is specified by param['objective'] and therefore `fobj`"
+                    " will be ignored.",
+                    UserWarning,
+                )
 
         # Handling alias metrics.
         _handling_alias_metrics(params)
 
+        if early_stopping_rounds is not None:
+            callbacks.append(
+                lgb.early_stopping(
+                    stopping_rounds=early_stopping_rounds, verbose=bool(verbose_eval)
+                )
+            )
+
         args = [params, train_set]
-        kwargs: Dict[str, Any] = dict(
+        kwargs: dict[str, Any] = dict(
             num_boost_round=num_boost_round,
-            fobj=fobj,
             feval=feval,
             feature_name=feature_name,
             categorical_feature=categorical_feature,
-            early_stopping_rounds=early_stopping_rounds,
-            verbose_eval=verbose_eval,
             callbacks=callbacks,
             time_budget=time_budget,
             sample_size=sample_size,
             verbosity=verbosity,
             show_progress_bar=show_progress_bar,
         )
         self._parse_args(*args, **kwargs)
-        self._start_time: Optional[float] = None
+        self._start_time: float | None = None
         self._optuna_callbacks = optuna_callbacks
-        self._best_booster_with_trial_number: Optional[
-            Tuple[Union[lgb.Booster, lgb.CVBooster], int]
-        ] = None
+        self._best_booster_with_trial_number: tuple[lgb.Booster | lgb.CVBooster, int] | None = None
         self._model_dir = model_dir
         self._optuna_seed = optuna_seed
 
         # Should not alter data since `min_data_in_leaf` is tuned.
         # https://lightgbm.readthedocs.io/en/latest/Parameters.html#feature_pre_filter
         if self.lgbm_params.get("feature_pre_filter", False):
             warnings.warn(
@@ -445,63 +467,25 @@
         try:
             return self.study.best_value
         except ValueError:
             # Return the default score because no trials have completed.
             return -np.inf if self.higher_is_better() else np.inf
 
     @property
-    def best_params(self) -> Dict[str, Any]:
+    def best_params(self) -> dict[str, Any]:
         """Return parameters of the best booster."""
         try:
             return json.loads(self.study.best_trial.system_attrs[_LGBM_PARAMS_KEY])
         except ValueError:
             # Return the default score because no trials have completed.
             params = copy.deepcopy(_DEFAULT_LIGHTGBM_PARAMETERS)
             # self.lgbm_params may contain parameters given by users.
             params.update(self.lgbm_params)
             return params
 
-    def get_best_booster(self) -> "lgb.Booster":
-        """Return the best booster.
-
-        If the best booster cannot be found, :class:`ValueError` will be raised. To prevent the
-        errors, please save boosters by specifying the ``model_dir`` argument of
-        :meth:`~optuna.integration.lightgbm.LightGBMTuner.__init__`,
-        when you resume tuning or you run tuning in parallel.
-        """
-        if self._best_booster_with_trial_number is not None:
-            if self._best_booster_with_trial_number[1] == self.study.best_trial.number:
-                return self._best_booster_with_trial_number[0]
-        if len(self.study.trials) == 0:
-            raise ValueError("The best booster is not available because no trials completed.")
-
-        # The best booster exists, but this instance does not have it.
-        # This may be due to resuming or parallelization.
-        if self._model_dir is None:
-            raise ValueError(
-                "The best booster cannot be found. It may be found in the other processes due to "
-                "resuming or distributed computing. Please set the `model_dir` argument of "
-                "`LightGBMTuner.__init__` and make sure that boosters are shared with all "
-                "processes."
-            )
-
-        best_trial = self.study.best_trial
-        path = os.path.join(self._model_dir, "{}.pkl".format(best_trial.number))
-        if not os.path.exists(path):
-            raise ValueError(
-                "The best booster cannot be found in {}. If you execute `LightGBMTuner` in "
-                "distributed environment, please use network file system (e.g., NFS) to share "
-                "models with multiple workers.".format(self._model_dir)
-            )
-
-        with open(path, "rb") as fin:
-            booster = pickle.load(fin)
-
-        return booster
-
     def _parse_args(self, *args: Any, **kwargs: Any) -> None:
         self.auto_options = {
             option_name: kwargs.get(option_name)
             for option_name in ["time_budget", "sample_size", "verbosity", "show_progress_bar"]
         }
 
         # Split options.
@@ -553,15 +537,15 @@
             idx_list = offset + np.arange(self.auto_options["sample_size"])
             self.train_subset = self.train_set.subset(idx_list)
 
     def tune_feature_fraction(self, n_trials: int = 7) -> None:
         param_name = "feature_fraction"
         param_values = np.linspace(0.4, 1.0, n_trials).tolist()
 
-        sampler = optuna.samplers.GridSampler({param_name: param_values})
+        sampler = optuna.samplers.GridSampler({param_name: param_values}, seed=self._optuna_seed)
         self._tune_params([param_name], len(param_values), sampler, "feature_fraction")
 
     def tune_num_leaves(self, n_trials: int = 20) -> None:
         self._tune_params(
             ["num_leaves"],
             n_trials,
             optuna.samplers.TPESampler(seed=self._optuna_seed),
@@ -580,35 +564,35 @@
         param_name = "feature_fraction"
         best_feature_fraction = self.best_params[param_name]
         param_values = np.linspace(
             best_feature_fraction - 0.08, best_feature_fraction + 0.08, n_trials
         ).tolist()
         param_values = [val for val in param_values if val >= 0.4 and val <= 1.0]
 
-        sampler = optuna.samplers.GridSampler({param_name: param_values})
+        sampler = optuna.samplers.GridSampler({param_name: param_values}, seed=self._optuna_seed)
         self._tune_params([param_name], len(param_values), sampler, "feature_fraction_stage2")
 
     def tune_regularization_factors(self, n_trials: int = 20) -> None:
         self._tune_params(
             ["lambda_l1", "lambda_l2"],
             n_trials,
             optuna.samplers.TPESampler(seed=self._optuna_seed),
             "regularization_factors",
         )
 
     def tune_min_data_in_leaf(self) -> None:
         param_name = "min_child_samples"
         param_values = [5, 10, 25, 50, 100]
 
-        sampler = optuna.samplers.GridSampler({param_name: param_values})
+        sampler = optuna.samplers.GridSampler({param_name: param_values}, seed=self._optuna_seed)
         self._tune_params([param_name], len(param_values), sampler, "min_data_in_leaf")
 
     def _tune_params(
         self,
-        target_param_names: List[str],
+        target_param_names: list[str],
         n_trials: int,
         sampler: optuna.samplers.BaseSampler,
         step_name: str,
     ) -> _OptunaObjective:
         pbar = (
             tqdm.tqdm(total=n_trials, ascii=True)
             if self.auto_options["show_progress_bar"]
@@ -657,18 +641,18 @@
             self._best_booster_with_trial_number = objective.best_booster_with_trial_number
 
         return objective
 
     @abc.abstractmethod
     def _create_objective(
         self,
-        target_param_names: List[str],
+        target_param_names: list[str],
         train_set: "lgb.Dataset",
         step_name: str,
-        pbar: Optional[tqdm.tqdm],
+        pbar: tqdm.tqdm | None,
     ) -> _OptunaObjective:
         raise NotImplementedError
 
     def _create_stepwise_study(
         self, study: "optuna.study.Study", step_name: str
     ) -> "optuna.study.Study":
         # This class is assumed to be passed to a sampler and a pruner corresponding to the step.
@@ -681,16 +665,16 @@
                     pruner=study.pruner,
                 )
                 self._step_name = step_name
 
             def get_trials(
                 self,
                 deepcopy: bool = True,
-                states: Optional[Container[TrialState]] = None,
-            ) -> List[optuna.trial.FrozenTrial]:
+                states: Container[TrialState] | None = None,
+            ) -> list[optuna.trial.FrozenTrial]:
                 trials = super()._get_trials(deepcopy=deepcopy, states=states)
                 return [t for t in trials if t.system_attrs.get(_STEP_NAME_KEY) == self._step_name]
 
             @property
             def best_trial(self) -> optuna.trial.FrozenTrial:
                 """Return the best trial in the study.
 
@@ -785,89 +769,141 @@
     .. _lightgbm.train(): https://lightgbm.readthedocs.io/en/latest/pythonapi/lightgbm.train.html
     .. _LightGBM's verbosity: https://lightgbm.readthedocs.io/en/latest/Parameters.html#verbosity
     .. _deterministic: https://lightgbm.readthedocs.io/en/latest/Parameters.html#deterministic
     """
 
     def __init__(
         self,
-        params: Dict[str, Any],
+        params: dict[str, Any],
         train_set: "lgb.Dataset",
         num_boost_round: int = 1000,
-        valid_sets: Optional["VALID_SET_TYPE"] = None,
-        valid_names: Optional[Any] = None,
-        fobj: Optional[Callable[..., Any]] = None,
-        feval: Optional[Callable[..., Any]] = None,
+        valid_sets: "VALID_SET_TYPE" | None = None,
+        valid_names: Any | None = None,
+        fobj: Callable[..., Any] | None = None,
+        feval: Callable[..., Any] | None = None,
         feature_name: str = "auto",
         categorical_feature: str = "auto",
-        early_stopping_rounds: Optional[int] = None,
-        evals_result: Optional[Dict[Any, Any]] = None,
-        verbose_eval: Optional[Union[bool, int, str]] = "warn",
-        learning_rates: Optional[List[float]] = None,
+        early_stopping_rounds: int | None = None,
+        evals_result: dict[Any, Any] | None = None,
+        verbose_eval: bool | int | str | None = "warn",
+        learning_rates: list[float] | None = None,
         keep_training_booster: bool = False,
-        callbacks: Optional[List[Callable[..., Any]]] = None,
-        time_budget: Optional[int] = None,
-        sample_size: Optional[int] = None,
-        study: Optional[optuna.study.Study] = None,
-        optuna_callbacks: Optional[List[Callable[[Study, FrozenTrial], None]]] = None,
-        model_dir: Optional[str] = None,
-        verbosity: Optional[int] = None,
+        callbacks: list[Callable[..., Any]] | None = None,
+        time_budget: int | None = None,
+        sample_size: int | None = None,
+        study: optuna.study.Study | None = None,
+        optuna_callbacks: list[Callable[[Study, FrozenTrial], None]] | None = None,
+        model_dir: str | None = None,
+        verbosity: int | None = None,
         show_progress_bar: bool = True,
         *,
-        optuna_seed: Optional[int] = None,
+        optuna_seed: int | None = None,
     ) -> None:
+        if callbacks is None:
+            callbacks = []
+
+        if evals_result is not None:
+            callbacks.append(lgb.record_evaluation(evals_result))
+
+        if learning_rates is not None:
+            callbacks.append(lgb.reset_parameter(learning_rate=learning_rates))
+
+        if verbose_eval == "warn":
+            verbose_eval = False if callbacks else True
+        if verbose_eval is True:
+            callbacks.append(lgb.log_evaluation())
+        elif isinstance(verbose_eval, int):
+            callbacks.append(lgb.log_evaluation(verbose_eval))
+
         super().__init__(
             params,
             train_set,
+            callbacks=callbacks,
             num_boost_round=num_boost_round,
             fobj=fobj,
             feval=feval,
             feature_name=feature_name,
             categorical_feature=categorical_feature,
             early_stopping_rounds=early_stopping_rounds,
             verbose_eval=verbose_eval,
-            callbacks=callbacks,
             time_budget=time_budget,
             sample_size=sample_size,
             study=study,
             optuna_callbacks=optuna_callbacks,
             verbosity=verbosity,
             show_progress_bar=show_progress_bar,
             model_dir=model_dir,
             optuna_seed=optuna_seed,
         )
 
         self.lgbm_kwargs["valid_sets"] = valid_sets
         self.lgbm_kwargs["valid_names"] = valid_names
-        self.lgbm_kwargs["evals_result"] = evals_result
-        self.lgbm_kwargs["learning_rates"] = learning_rates
         self.lgbm_kwargs["keep_training_booster"] = keep_training_booster
 
-        self._best_booster_with_trial_number: Optional[Tuple[lgb.Booster, int]] = None
+        self._best_booster_with_trial_number: tuple[lgb.Booster, int] | None = None
 
         if valid_sets is None:
             raise ValueError("`valid_sets` is required.")
 
     def _create_objective(
         self,
-        target_param_names: List[str],
+        target_param_names: list[str],
         train_set: "lgb.Dataset",
         step_name: str,
-        pbar: Optional[tqdm.tqdm],
+        pbar: tqdm.tqdm | None,
     ) -> _OptunaObjective:
         return _OptunaObjective(
             target_param_names,
             self.lgbm_params,
             train_set,
             self.lgbm_kwargs,
             self.best_score,
             step_name=step_name,
             model_dir=self._model_dir,
             pbar=pbar,
         )
 
+    def get_best_booster(self) -> "lgb.Booster":
+        """Return the best booster.
+
+        If the best booster cannot be found, :class:`ValueError` will be raised. To prevent the
+        errors, please save boosters by specifying the ``model_dir`` argument of
+        :meth:`~optuna.integration.lightgbm.LightGBMTuner.__init__`,
+        when you resume tuning or you run tuning in parallel.
+        """
+        if self._best_booster_with_trial_number is not None:
+            if self._best_booster_with_trial_number[1] == self.study.best_trial.number:
+                return self._best_booster_with_trial_number[0]
+        if len(self.study.trials) == 0:
+            raise ValueError("The best booster is not available because no trials completed.")
+
+        # The best booster exists, but this instance does not have it.
+        # This may be due to resuming or parallelization.
+        if self._model_dir is None:
+            raise ValueError(
+                "The best booster cannot be found. It may be found in the other processes due to "
+                "resuming or distributed computing. Please set the `model_dir` argument of "
+                "`LightGBMTuner.__init__` and make sure that boosters are shared with all "
+                "processes."
+            )
+
+        best_trial = self.study.best_trial
+        path = os.path.join(self._model_dir, "{}.pkl".format(best_trial.number))
+        if not os.path.exists(path):
+            raise ValueError(
+                "The best booster cannot be found in {}. If you execute `LightGBMTuner` in "
+                "distributed environment, please use network file system (e.g., NFS) to share "
+                "models with multiple workers.".format(self._model_dir)
+            )
+
+        with open(path, "rb") as fin:
+            booster = pickle.load(fin)
+
+        return booster
+
 
 class LightGBMTunerCV(_LightGBMBaseTuner):
     """Hyperparameter tuner for LightGBM with cross-validation.
 
     It employs the same stepwise approach as
     :class:`~optuna.integration.lightgbm.LightGBMTuner`.
     :class:`~optuna.integration.lightgbm.LightGBMTunerCV` invokes `lightgbm.cv()`_ to train
@@ -942,84 +978,88 @@
     .. _lightgbm.cv(): https://lightgbm.readthedocs.io/en/latest/pythonapi/lightgbm.cv.html
     .. _LightGBM's verbosity: https://lightgbm.readthedocs.io/en/latest/Parameters.html#verbosity
     .. _deterministic: https://lightgbm.readthedocs.io/en/latest/Parameters.html#deterministic
     """
 
     def __init__(
         self,
-        params: Dict[str, Any],
+        params: dict[str, Any],
         train_set: "lgb.Dataset",
         num_boost_round: int = 1000,
-        folds: Optional[
-            Union[
-                Generator[Tuple[int, int], None, None],
-                Iterator[Tuple[int, int]],
-                "BaseCrossValidator",
-            ]
-        ] = None,
+        folds: Generator[tuple[int, int], None, None]
+        | Iterator[tuple[int, int]]
+        | "BaseCrossValidator"
+        | None = None,
         nfold: int = 5,
         stratified: bool = True,
         shuffle: bool = True,
-        fobj: Optional[Callable[..., Any]] = None,
-        feval: Optional[Callable[..., Any]] = None,
+        fobj: Callable[..., Any] | None = None,
+        feval: Callable[..., Any] | None = None,
         feature_name: str = "auto",
         categorical_feature: str = "auto",
-        early_stopping_rounds: Optional[int] = None,
-        fpreproc: Optional[Callable[..., Any]] = None,
-        verbose_eval: Optional[Union[bool, int]] = None,
+        early_stopping_rounds: int | None = None,
+        fpreproc: Callable[..., Any] | None = None,
+        verbose_eval: bool | int | None = None,
         show_stdv: bool = True,
         seed: int = 0,
-        callbacks: Optional[List[Callable[..., Any]]] = None,
-        time_budget: Optional[int] = None,
-        sample_size: Optional[int] = None,
-        study: Optional[optuna.study.Study] = None,
-        optuna_callbacks: Optional[List[Callable[[Study, FrozenTrial], None]]] = None,
-        verbosity: Optional[int] = None,
+        callbacks: list[Callable[..., Any]] | None = None,
+        time_budget: int | None = None,
+        sample_size: int | None = None,
+        study: optuna.study.Study | None = None,
+        optuna_callbacks: list[Callable[[Study, FrozenTrial], None]] | None = None,
+        verbosity: int | None = None,
         show_progress_bar: bool = True,
-        model_dir: Optional[str] = None,
+        model_dir: str | None = None,
         return_cvbooster: bool = False,
         *,
-        optuna_seed: Optional[int] = None,
+        optuna_seed: int | None = None,
     ) -> None:
+        if callbacks is None:
+            callbacks = []
+
+        if verbose_eval is True:
+            callbacks.append(lgb.log_evaluation(show_stdv=show_stdv))
+        elif isinstance(verbose_eval, int):
+            callbacks.append(lgb.log_evaluation(period=verbose_eval, show_stdv=show_stdv))
+
         super().__init__(
             params,
             train_set,
-            num_boost_round,
+            callbacks=callbacks,
+            num_boost_round=num_boost_round,
             fobj=fobj,
             feval=feval,
             feature_name=feature_name,
             categorical_feature=categorical_feature,
             early_stopping_rounds=early_stopping_rounds,
             verbose_eval=verbose_eval,
-            callbacks=callbacks,
             time_budget=time_budget,
             sample_size=sample_size,
             study=study,
             optuna_callbacks=optuna_callbacks,
             verbosity=verbosity,
             show_progress_bar=show_progress_bar,
             model_dir=model_dir,
             optuna_seed=optuna_seed,
         )
 
         self.lgbm_kwargs["folds"] = folds
         self.lgbm_kwargs["nfold"] = nfold
         self.lgbm_kwargs["stratified"] = stratified
         self.lgbm_kwargs["shuffle"] = shuffle
-        self.lgbm_kwargs["show_stdv"] = show_stdv
         self.lgbm_kwargs["seed"] = seed
         self.lgbm_kwargs["fpreproc"] = fpreproc
         self.lgbm_kwargs["return_cvbooster"] = return_cvbooster
 
     def _create_objective(
         self,
-        target_param_names: List[str],
+        target_param_names: list[str],
         train_set: "lgb.Dataset",
         step_name: str,
-        pbar: Optional[tqdm.tqdm],
+        pbar: tqdm.tqdm | None,
     ) -> _OptunaObjective:
         return _OptunaObjectiveCV(
             target_param_names,
             self.lgbm_params,
             train_set,
             self.lgbm_kwargs,
             self.best_score,
@@ -1039,14 +1079,15 @@
         """
         if self.lgbm_kwargs.get("return_cvbooster") is not True:
             raise ValueError(
                 "LightGBMTunerCV requires `return_cvbooster=True` for method `get_best_booster()`."
             )
         if self._best_booster_with_trial_number is not None:
             if self._best_booster_with_trial_number[1] == self.study.best_trial.number:
+                assert isinstance(self._best_booster_with_trial_number[0], lgb.CVBooster)
                 return self._best_booster_with_trial_number[0]
         if len(self.study.trials) == 0:
             raise ValueError("The best booster is not available because no trials completed.")
 
         # The best booster exists, but this instance does not have it.
         # This may be due to resuming or parallelization.
         if self._model_dir is None:
```

### Comparing `optuna-3.2.0/optuna/integration/_lightgbm_tuner/sklearn.py` & `optuna-3.3.0/optuna/integration/_lightgbm_tuner/sklearn.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/integration/botorch.py` & `optuna-3.3.0/optuna/integration/botorch.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from collections import OrderedDict
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Optional
 from typing import Sequence
 from typing import Union
 import warnings
@@ -25,14 +24,15 @@
 from optuna.study import StudyDirection
 from optuna.trial import FrozenTrial
 from optuna.trial import TrialState
 
 
 with try_import() as _imports:
     from botorch.acquisition.monte_carlo import qExpectedImprovement
+    from botorch.acquisition.monte_carlo import qNoisyExpectedImprovement
     from botorch.acquisition.multi_objective import monte_carlo
     from botorch.acquisition.multi_objective.objective import IdentityMCMultiOutputObjective
     from botorch.acquisition.objective import ConstrainedMCObjective
     from botorch.acquisition.objective import GenericMCObjective
     from botorch.models import SingleTaskGP
     from botorch.models.transforms.outcome import Standardize
     from botorch.optim import optimize_acqf
@@ -59,27 +59,120 @@
     from botorch.utils.transforms import unnormalize
     from gpytorch.mlls import ExactMarginalLogLikelihood
     import torch
 
 
 _logger = logging.get_logger(__name__)
 
+with try_import() as _imports_logei:
+    from botorch.acquisition.analytic import LogExpectedImprovement
+
+
+@experimental_func("3.3.0")
+def logei_candidates_func(
+    train_x: "torch.Tensor",
+    train_obj: "torch.Tensor",
+    train_con: Optional["torch.Tensor"],
+    bounds: "torch.Tensor",
+    pending_x: Optional["torch.Tensor"],
+) -> "torch.Tensor":
+    """Log Expected Improvement (LogEI).
+
+    The default value of ``candidates_func`` in :class:`~optuna.integration.BoTorchSampler`
+    with single-objective optimization for non-constrained problems.
+
+    Args:
+        train_x:
+            Previous parameter configurations. A ``torch.Tensor`` of shape
+            ``(n_trials, n_params)``. ``n_trials`` is the number of already observed trials
+            and ``n_params`` is the number of parameters. ``n_params`` may be larger than the
+            actual number of parameters if categorical parameters are included in the search
+            space, since these parameters are one-hot encoded.
+            Values are not normalized.
+        train_obj:
+            Previously observed objectives. A ``torch.Tensor`` of shape
+            ``(n_trials, n_objectives)``. ``n_trials`` is identical to that of ``train_x``.
+            ``n_objectives`` is the number of objectives. Observations are not normalized.
+        train_con:
+            Objective constraints. This option is not supported in ``logei_candidates_func`` and
+            must be :obj:`None`.
+        bounds:
+            Search space bounds. A ``torch.Tensor`` of shape ``(2, n_params)``. ``n_params`` is
+            identical to that of ``train_x``. The first and the second rows correspond to the
+            lower and upper bounds for each parameter respectively.
+        pending_x:
+            Pending parameter configurations. A ``torch.Tensor`` of shape
+            ``(n_pending, n_params)``. ``n_pending`` is the number of the trials which are already
+            suggested all their parameters but have not completed their evaluation, and
+            ``n_params`` is identical to that of ``train_x``.
+
+    Returns:
+        Next set of candidates. Usually the return value of BoTorch's ``optimize_acqf``.
+
+    """
+
+    # We need botorch >=0.8.1 for LogExpectedImprovement.
+    if not _imports_logei.is_successful():
+        raise ImportError(
+            "logei_candidates_func requires botorch >=0.8.1. "
+            "Please upgrade botorch or use qei_candidates_func as candidates_func instead."
+        )
+
+    if train_obj.size(-1) != 1:
+        raise ValueError("Objective may only contain single values with logEI.")
+    if train_con is not None:
+        raise ValueError(
+            "Constraint is not supported with logei_candidates_func. "
+            + "Please use qei_candidates_func instead."
+        )
+    else:
+        train_y = train_obj
+        best_f = train_obj.max()
+
+    train_x = normalize(train_x, bounds=bounds)
+
+    model = SingleTaskGP(train_x, train_y, outcome_transform=Standardize(m=train_y.size(-1)))
+    mll = ExactMarginalLogLikelihood(model.likelihood, model)
+    fit_gpytorch_mll(mll)
+
+    acqf = LogExpectedImprovement(
+        model=model,
+        best_f=best_f,
+    )
+
+    standard_bounds = torch.zeros_like(bounds)
+    standard_bounds[1] = 1
+
+    candidates, _ = optimize_acqf(
+        acq_function=acqf,
+        bounds=standard_bounds,
+        q=1,
+        num_restarts=10,
+        raw_samples=512,
+        options={"batch_limit": 5, "maxiter": 200},
+        sequential=True,
+    )
+
+    candidates = unnormalize(candidates.detach(), bounds=bounds)
+
+    return candidates
+
 
 @experimental_func("2.4.0")
 def qei_candidates_func(
     train_x: "torch.Tensor",
     train_obj: "torch.Tensor",
     train_con: Optional["torch.Tensor"],
     bounds: "torch.Tensor",
     pending_x: Optional["torch.Tensor"],
 ) -> "torch.Tensor":
     """Quasi MC-based batch Expected Improvement (qEI).
 
     The default value of ``candidates_func`` in :class:`~optuna.integration.BoTorchSampler`
-    with single-objective optimization.
+    with single-objective optimization for constrained problems.
 
     Args:
         train_x:
             Previous parameter configurations. A ``torch.Tensor`` of shape
             ``(n_trials, n_params)``. ``n_trials`` is the number of already observed trials
             and ``n_params`` is the number of parameters. ``n_params`` may be larger than the
             actual number of parameters if categorical parameters are included in the search
@@ -169,14 +262,82 @@
     )
 
     candidates = unnormalize(candidates.detach(), bounds=bounds)
 
     return candidates
 
 
+@experimental_func("3.3.0")
+def qnei_candidates_func(
+    train_x: "torch.Tensor",
+    train_obj: "torch.Tensor",
+    train_con: Optional["torch.Tensor"],
+    bounds: "torch.Tensor",
+    pending_x: Optional["torch.Tensor"],
+) -> "torch.Tensor":
+    """Quasi MC-based batch Noisy Expected Improvement (qNEI).
+
+    This function may perform better than qEI (`qei_candidates_func`) when
+    the evaluated values of objective function are noisy.
+
+    .. seealso::
+        :func:`~optuna.integration.botorch.qei_candidates_func` for argument and return value
+        descriptions.
+    """
+    if train_obj.size(-1) != 1:
+        raise ValueError("Objective may only contain single values with qNEI.")
+    if train_con is not None:
+        train_y = torch.cat([train_obj, train_con], dim=-1)
+
+        n_constraints = train_con.size(1)
+        objective = ConstrainedMCObjective(
+            objective=lambda Z: Z[..., 0],
+            constraints=[
+                (lambda Z, i=i: Z[..., -n_constraints + i]) for i in range(n_constraints)
+            ],
+        )
+    else:
+        train_y = train_obj
+
+        objective = None  # Using the default identity objective.
+
+    train_x = normalize(train_x, bounds=bounds)
+    if pending_x is not None:
+        pending_x = normalize(pending_x, bounds=bounds)
+
+    model = SingleTaskGP(train_x, train_y, outcome_transform=Standardize(m=train_y.size(-1)))
+    mll = ExactMarginalLogLikelihood(model.likelihood, model)
+    fit_gpytorch_mll(mll)
+
+    acqf = qNoisyExpectedImprovement(
+        model=model,
+        X_baseline=train_x,
+        sampler=_get_sobol_qmc_normal_sampler(256),
+        objective=objective,
+        X_pending=pending_x,
+    )
+
+    standard_bounds = torch.zeros_like(bounds)
+    standard_bounds[1] = 1
+
+    candidates, _ = optimize_acqf(
+        acq_function=acqf,
+        bounds=standard_bounds,
+        q=1,
+        num_restarts=10,
+        raw_samples=512,
+        options={"batch_limit": 5, "maxiter": 200},
+        sequential=True,
+    )
+
+    candidates = unnormalize(candidates.detach(), bounds=bounds)
+
+    return candidates
+
+
 @experimental_func("2.4.0")
 def qehvi_candidates_func(
     train_x: "torch.Tensor",
     train_obj: "torch.Tensor",
     train_con: Optional["torch.Tensor"],
     bounds: "torch.Tensor",
     pending_x: Optional["torch.Tensor"],
@@ -264,15 +425,15 @@
 def qnehvi_candidates_func(
     train_x: "torch.Tensor",
     train_obj: "torch.Tensor",
     train_con: Optional["torch.Tensor"],
     bounds: "torch.Tensor",
     pending_x: Optional["torch.Tensor"],
 ) -> "torch.Tensor":
-    """Quasi MC-based batch Expected Noisy Hypervolume Improvement (qNEHVI).
+    """Quasi MC-based batch Noisy Expected Hypervolume Improvement (qNEHVI).
 
     According to Botorch/Ax documentation,
     this function may perform better than qEHVI (`qehvi_candidates_func`).
     (cf. https://botorch.org/tutorials/constrained_multi_objective_bo )
 
     .. seealso::
         :func:`~optuna.integration.botorch.qei_candidates_func` for argument and return value
@@ -415,30 +576,34 @@
     candidates = unnormalize(candidates.detach(), bounds=bounds)
 
     return candidates
 
 
 def _get_default_candidates_func(
     n_objectives: int,
+    has_constraint: bool,
+    consider_running_trials: bool,
 ) -> Callable[
     [
         "torch.Tensor",
         "torch.Tensor",
         Optional["torch.Tensor"],
         "torch.Tensor",
         Optional["torch.Tensor"],
     ],
     "torch.Tensor",
 ]:
     if n_objectives > 3:
         return qparego_candidates_func
     elif n_objectives > 1:
         return qehvi_candidates_func
-    else:
+    elif has_constraint or consider_running_trials:
         return qei_candidates_func
+    else:
+        return logei_candidates_func
 
 
 @experimental_class("2.4.0")
 class BoTorchSampler(BaseSampler):
     """A sampler that uses BoTorch, a Bayesian optimization library built on top of PyTorch.
 
     This sampler allows using BoTorch's optimization algorithms from Optuna to suggest parameter
@@ -463,16 +628,19 @@
             An optional function that suggests the next candidates. It must take the training
             data, the objectives, the constraints, the search space bounds and return the next
             candidates. The arguments are of type ``torch.Tensor``. The return value must be a
             ``torch.Tensor``. However, if ``constraints_func`` is omitted, constraints will be
             :obj:`None`. For any constraints that failed to compute, the tensor will contain
             NaN.
 
-            If omitted, it is determined automatically based on the number of objectives. If the
-            number of objectives is one, Quasi MC-based batch Expected Improvement (qEI) is used.
+            If omitted, it is determined automatically based on the number of objectives and
+            whether a constraint is specified. If the
+            number of objectives is one and no constraint is specified, log-Expected Improvement
+            is used. If constraints are specified, quasi MC-based batch Expected Improvement
+            (qEI) is used.
             If the number of objectives is either two or three, Quasi MC-based
             batch Expected Hypervolume Improvement (qEHVI) is used. Otherwise, for larger number
             of objectives, the faster Quasi MC-based extended ParEGO (qParEGO) is used.
 
             The function should assume *maximization* of the objective.
 
             .. seealso::
@@ -518,15 +686,15 @@
                     Optional["torch.Tensor"],
                 ],
                 "torch.Tensor",
             ]
         ] = None,
         constraints_func: Optional[Callable[[FrozenTrial], Sequence[float]]] = None,
         n_startup_trials: int = 10,
-        consider_running_trials: bool = True,
+        consider_running_trials: bool = False,
         independent_sampler: Optional[BaseSampler] = None,
         seed: Optional[int] = None,
         device: Optional["torch.device"] = None,
     ):
         _imports.check()
 
         self._candidates_func = candidates_func
@@ -548,16 +716,16 @@
         if self._study_id is None:
             self._study_id = study._study_id
         if self._study_id != study._study_id:
             # Note that the check below is meaningless when `InMemoryStorage` is used
             # because `InMemoryStorage.create_new_study` always returns the same study ID.
             raise RuntimeError("BoTorchSampler cannot handle multiple studies.")
 
-        search_space: Dict[str, BaseDistribution] = OrderedDict()
-        for name, distribution in self._search_space.calculate(study, ordered_dict=True).items():
+        search_space: Dict[str, BaseDistribution] = {}
+        for name, distribution in self._search_space.calculate(study).items():
             if distribution.single():
                 # built-in `candidates_func` cannot handle distributions that contain just a
                 # single value, so we skip them. Note that the parameter values for such
                 # distributions are sampled in `Trial`.
                 continue
             search_space[name] = distribution
 
@@ -565,15 +733,15 @@
 
     def sample_relative(
         self,
         study: Study,
         trial: FrozenTrial,
         search_space: Dict[str, BaseDistribution],
     ) -> Dict[str, Any]:
-        assert isinstance(search_space, OrderedDict)
+        assert isinstance(search_space, dict)
 
         if len(search_space) == 0:
             return {}
 
         completed_trials = study.get_trials(deepcopy=False, states=(TrialState.COMPLETE,))
         running_trials = [
             t for t in study.get_trials(deepcopy=False, states=(TrialState.RUNNING,)) if t != trial
@@ -650,15 +818,19 @@
 
         if con is not None:
             if con.dim() == 1:
                 con.unsqueeze_(-1)
         bounds.transpose_(0, 1)
 
         if self._candidates_func is None:
-            self._candidates_func = _get_default_candidates_func(n_objectives=n_objectives)
+            self._candidates_func = _get_default_candidates_func(
+                n_objectives=n_objectives,
+                has_constraint=con is not None,
+                consider_running_trials=self._consider_running_trials,
+            )
 
         completed_values = values[:n_completed_trials]
         completed_params = params[:n_completed_trials]
         if self._consider_running_trials:
             running_params = params[n_completed_trials:]
             running_params = running_params[~torch.isnan(running_params).any(dim=1)]
         else:
```

### Comparing `optuna-3.2.0/optuna/integration/catboost.py` & `optuna-3.3.0/optuna/integration/catboost.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/integration/cma.py` & `optuna-3.3.0/optuna/integration/cma.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/integration/dask.py` & `optuna-3.3.0/optuna/integration/dask.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/integration/fastaiv1.py` & `optuna-3.3.0/optuna/integration/fastaiv1.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/integration/fastaiv2.py` & `optuna-3.3.0/optuna/integration/fastaiv2.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/integration/lightgbm.py` & `optuna-3.3.0/optuna/integration/lightgbm.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,18 @@
         self._report_interval = report_interval
 
     def _find_evaluation_result(
         self, target_valid_name: str, env: "CallbackEnv"
     ) -> Optional[List]:
         for evaluation_result in env.evaluation_result_list:
             valid_name, metric, current_score, is_higher_better = evaluation_result[:4]
-            if valid_name != target_valid_name or metric != self._metric:
+            # The prefix "valid " is added to metric name since LightGBM v4.0.0.
+            if valid_name != target_valid_name or (
+                metric != "valid " + self._metric and metric != self._metric
+            ):
                 continue
 
             return evaluation_result
 
         return None
 
     def __call__(self, env: "CallbackEnv") -> None:
```

### Comparing `optuna-3.2.0/optuna/integration/mlflow.py` & `optuna-3.3.0/optuna/integration/mlflow.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/integration/pytorch_distributed.py` & `optuna-3.3.0/optuna/integration/pytorch_distributed.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/integration/pytorch_ignite.py` & `optuna-3.3.0/optuna/integration/pytorch_ignite.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/integration/pytorch_lightning.py` & `optuna-3.3.0/optuna/integration/pytorch_lightning.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/integration/shap.py` & `optuna-3.3.0/optuna/integration/shap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from collections import OrderedDict
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 
 import numpy as np
 
@@ -78,15 +77,15 @@
             )
 
         distributions = _get_distributions(study, params=params)
         if params is None:
             params = list(distributions.keys())
         assert params is not None
         if len(params) == 0:
-            return OrderedDict()
+            return {}
 
         trials: List[FrozenTrial] = _get_filtered_trials(study, params=params, target=target)
         trans = _SearchSpaceTransform(distributions, transform_log=False, transform_step=False)
         trans_params: np.ndarray = _get_trans_params(trials, trans)
         target_values: np.ndarray = _get_target_values(trials, target)
 
         forest = self._forest
```

### Comparing `optuna-3.2.0/optuna/integration/sklearn.py` & `optuna-3.3.0/optuna/integration/sklearn.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,25 +211,39 @@
         params = self._get_params(trial)
 
         estimator.set_params(**params)
 
         if self.enable_pruning:
             scores = self._cross_validate_with_pruning(trial, estimator)
         else:
-            scores = cross_validate(
-                estimator,
-                self.X,
-                self.y,
-                cv=self.cv,
-                error_score=self.error_score,
-                fit_params=self.fit_params,
-                groups=self.groups,
-                return_train_score=self.return_train_score,
-                scoring=self.scoring,
-            )
+            try:
+                scores = cross_validate(
+                    estimator,
+                    self.X,
+                    self.y,
+                    cv=self.cv,
+                    error_score=self.error_score,
+                    fit_params=self.fit_params,
+                    groups=self.groups,
+                    return_train_score=self.return_train_score,
+                    scoring=self.scoring,
+                )
+            except ValueError:
+                n_splits = self.cv.get_n_splits(self.X, self.y, self.groups)
+                fit_time = np.array([np.nan] * n_splits)
+                score_time = np.array([np.nan] * n_splits)
+                test_score = np.array(
+                    [self.error_score if self.error_score is not None else np.nan] * n_splits
+                )
+
+                scores = {
+                    "fit_time": fit_time,
+                    "score_time": score_time,
+                    "test_score": test_score,
+                }
 
         self._store_scores(trial, scores)
 
         return trial.user_attrs["mean_test_score"]
 
     def _cross_validate_with_pruning(
         self, trial: Trial, estimator: "sklearn.base.BaseEstimator"
@@ -508,15 +522,15 @@
     def _estimator_type(self) -> str:
         return self.estimator._estimator_type
 
     @property
     def best_index_(self) -> int:
         """Trial number which corresponds to the best candidate parameter setting.
 
-        Retuned value is equivant to ``optuna_search.best_trial_.number``.
+        Returned value is equivalent to ``optuna_search.best_trial_.number``.
         """
 
         return self.best_trial_.number
 
     @property
     def best_params_(self) -> Dict[str, Any]:
         """Parameters of the best trial in the :class:`~optuna.study.Study`."""
@@ -546,14 +560,28 @@
         """Class labels."""
 
         self._check_is_fitted()
 
         return self.best_estimator_.classes_
 
     @property
+    def cv_results_(self) -> Dict[str, Any]:
+        """A dictionary mapping a metric name to a list of
+        Cross-Validation results of all trials."""
+        cv_results_dict_in_list = [trial_.user_attrs for trial_ in self.trials_]
+        if len(cv_results_dict_in_list) == 0:
+            cv_results_list_in_dict = {}
+        else:
+            cv_results_list_in_dict = {
+                key: [dict_[key] for dict_ in cv_results_dict_in_list]
+                for key in cv_results_dict_in_list[0]
+            }
+        return cv_results_list_in_dict
+
+    @property
     def n_trials_(self) -> int:
         """Actual number of trials."""
 
         return len(self.trials_)
 
     @property
     def trials_(self) -> List[FrozenTrial]:
@@ -881,15 +909,15 @@
             objective,
             n_jobs=self.n_jobs,
             n_trials=self.n_trials,
             timeout=self.timeout,
             callbacks=self.callbacks,
         )
 
-        _logger.info("Finished hyperparemeter search!")
+        _logger.info("Finished hyperparameter search!")
 
         if self.refit:
             self._refit(X, y, **fit_params)
 
         _logger.setLevel(old_level)
 
         return self
```

### Comparing `optuna-3.2.0/optuna/integration/skopt.py` & `optuna-3.3.0/optuna/integration/skopt.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/integration/tensorboard.py` & `optuna-3.3.0/optuna/integration/tensorboard.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/integration/wandb.py` & `optuna-3.3.0/optuna/integration/wandb.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/integration/xgboost.py` & `optuna-3.3.0/optuna/integration/xgboost.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/logging.py` & `optuna-3.3.0/optuna/logging.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/multi_objective/samplers/__init__.py` & `optuna-3.3.0/optuna/multi_objective/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/multi_objective/samplers/_adapter.py` & `optuna-3.3.0/optuna/multi_objective/samplers/_adapter.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/multi_objective/samplers/_base.py` & `optuna-3.3.0/optuna/multi_objective/samplers/_base.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/multi_objective/samplers/_motpe.py` & `optuna-3.3.0/optuna/multi_objective/samplers/_motpe.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/multi_objective/samplers/_nsga2.py` & `optuna-3.3.0/optuna/multi_objective/samplers/_nsga2.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/multi_objective/samplers/_random.py` & `optuna-3.3.0/optuna/multi_objective/samplers/_random.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/multi_objective/study.py` & `optuna-3.3.0/optuna/multi_objective/study.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/multi_objective/trial.py` & `optuna-3.3.0/optuna/multi_objective/trial.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/multi_objective/visualization/_pareto_front.py` & `optuna-3.3.0/optuna/multi_objective/visualization/_pareto_front.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/progress_bar.py` & `optuna-3.3.0/optuna/progress_bar.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 from typing import Any
 from typing import Optional
 from typing import TYPE_CHECKING
+import warnings
 
 from tqdm.auto import tqdm
 
 from optuna import logging as optuna_logging
 
 
 if TYPE_CHECKING:
@@ -41,14 +42,17 @@
 
     def __init__(
         self,
         is_valid: bool,
         n_trials: Optional[int] = None,
         timeout: Optional[float] = None,
     ) -> None:
+        if is_valid and n_trials is None and timeout is None:
+            warnings.warn("Progress bar won't be displayed because n_trials and timeout are None.")
+
         self._is_valid = is_valid and (n_trials or timeout) is not None
         self._n_trials = n_trials
         self._timeout = timeout
         self._last_elapsed_seconds = 0.0
 
         if self._is_valid:
             if self._n_trials is not None:
```

### Comparing `optuna-3.2.0/optuna/pruners/__init__.py` & `optuna-3.3.0/optuna/pruners/__init__.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/pruners/_base.py` & `optuna-3.3.0/optuna/pruners/_base.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/pruners/_hyperband.py` & `optuna-3.3.0/optuna/pruners/_hyperband.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/pruners/_median.py` & `optuna-3.3.0/optuna/pruners/_median.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/pruners/_nop.py` & `optuna-3.3.0/optuna/pruners/_nop.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/pruners/_patient.py` & `optuna-3.3.0/optuna/pruners/_patient.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/pruners/_percentile.py` & `optuna-3.3.0/optuna/pruners/_percentile.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/pruners/_successive_halving.py` & `optuna-3.3.0/optuna/pruners/_successive_halving.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/pruners/_threshold.py` & `optuna-3.3.0/optuna/pruners/_threshold.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/samplers/__init__.py` & `optuna-3.3.0/optuna/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/samplers/_base.py` & `optuna-3.3.0/optuna/samplers/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,14 +144,36 @@
         Returns:
             A parameter value.
 
         """
 
         raise NotImplementedError
 
+    def before_trial(self, study: Study, trial: FrozenTrial) -> None:
+        """Trial pre-processing.
+
+        This method is called before the objective function is called and right after the trial is
+        instantiated. More precisely, this method is called during trial initialization, just
+        before the :func:`~optuna.samplers.BaseSampler.infer_relative_search_space` call. In other
+        words, it is responsible for pre-processing that should be done before inferring the search
+        space.
+
+        .. note::
+            Added in v3.3.0 as an experimental feature. The interface may change in newer versions
+            without prior notice. See https://github.com/optuna/optuna/releases/tag/v3.3.0.
+
+        Args:
+            study:
+                Target study object.
+            trial:
+                Target trial object.
+        """
+
+        pass
+
     def after_trial(
         self,
         study: Study,
         trial: FrozenTrial,
         state: TrialState,
         values: Optional[Sequence[float]],
     ) -> None:
```

### Comparing `optuna-3.2.0/optuna/samplers/_brute_force.py` & `optuna-3.3.0/optuna/samplers/_brute_force.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,17 @@
         param_name: str,
         param_distribution: BaseDistribution,
     ) -> Any:
         trials = study.get_trials(
             deepcopy=False,
             states=(
                 TrialState.COMPLETE,
+                TrialState.PRUNED,
                 TrialState.RUNNING,
+                TrialState.FAIL,
             ),
         )
         tree = self._build_tree((t for t in trials if t.number != trial.number), trial.params)
         candidates = _enumerate_candidates(param_distribution)
         tree.expand(param_name, candidates)
         if tree.count_unexpanded() == 0:
             return param_distribution.to_external_repr(self._rng.choice(candidates))
@@ -203,15 +205,17 @@
         state: TrialState,
         values: Optional[Sequence[float]],
     ) -> None:
         trials = study.get_trials(
             deepcopy=False,
             states=(
                 TrialState.COMPLETE,
+                TrialState.PRUNED,
                 TrialState.RUNNING,
+                TrialState.FAIL,
             ),
         )
         tree = self._build_tree(
             (
                 t
                 if t.number != trial.number
                 else create_trial(
```

### Comparing `optuna-3.2.0/optuna/samplers/_cmaes.py` & `optuna-3.3.0/optuna/samplers/_cmaes.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,17 @@
       <https://hal.inria.fr/inria-00287367/document>`_
     - `Masahiro Nomura, Shuhei Watanabe, Youhei Akimoto, Yoshihiko Ozaki, Masaki Onishi.
       Warm Starting CMA-ES for Hyperparameter Optimization, AAAI. 2021.
       <https://arxiv.org/abs/2012.06932>`_
     - `R. Hamano, S. Saito, M. Nomura, S. Shirakawa. CMA-ES with Margin: Lower-Bounding Marginal
       Probability for Mixed-Integer Black-Box Optimization, GECCO. 2022.
       <https://arxiv.org/abs/2205.13482>`_
+    - `M. Nomura, Y. Akimoto, I. Ono. CMA-ES with Learning Rate Adaptation: Can CMA-ES with
+      Default Population Size Solve Multimodal and Noisy Problems?, GECCO. 2023.
+      <https://arxiv.org/abs/2304.03473>`_
 
     .. seealso::
         You can also use :class:`optuna.integration.PyCmaSampler` which is a sampler using cma
         library as the backend.
 
     Args:
 
@@ -214,14 +217,26 @@
             Currently, this option cannot be used with ``use_separable_cma=True``.
 
             .. note::
                 Added in v3.1.0 as an experimental feature. The interface may change in newer
                 versions without prior notice. See
                 https://github.com/optuna/optuna/releases/tag/v3.1.0.
 
+        lr_adapt:
+            If this is :obj:`True`, CMA-ES with learning rate adaptation is used.
+            This algorithm focuses on working well on multimodal and/or noisy problems
+            with default settings.
+            Currently, this option cannot be used with ``use_separable_cma=True`` or
+            ``with_margin=True``.
+
+            .. note::
+                Added in v3.3.0 or later, as an experimental feature.
+                The interface may change in newer versions without prior notice. See
+                https://github.com/optuna/optuna/releases/tag/v3.3.0.
+
         source_trials:
             This option is for Warm Starting CMA-ES, a method to transfer prior knowledge on
             similar HPO tasks through the initialization of CMA-ES. This method estimates a
             promising distribution from ``source_trials`` and generates the parameter of
             multivariate gaussian distribution. Please note that it is prohibited to use
             ``x0``, ``sigma0``, or ``use_separable_cma`` argument together.
 
@@ -243,14 +258,15 @@
         *,
         consider_pruned_trials: bool = False,
         restart_strategy: Optional[str] = None,
         popsize: Optional[int] = None,
         inc_popsize: int = 2,
         use_separable_cma: bool = False,
         with_margin: bool = False,
+        lr_adapt: bool = False,
         source_trials: Optional[List[FrozenTrial]] = None,
     ) -> None:
         self._x0 = x0
         self._sigma0 = sigma0
         self._independent_sampler = independent_sampler or optuna.samplers.RandomSampler(seed=seed)
         self._n_startup_trials = n_startup_trials
         self._warn_independent_sampling = warn_independent_sampling
@@ -258,14 +274,15 @@
         self._search_space = IntersectionSearchSpace()
         self._consider_pruned_trials = consider_pruned_trials
         self._restart_strategy = restart_strategy
         self._initial_popsize = popsize
         self._inc_popsize = inc_popsize
         self._use_separable_cma = use_separable_cma
         self._with_margin = with_margin
+        self._lr_adapt = lr_adapt
         self._source_trials = source_trials
 
         if self._restart_strategy:
             warnings.warn(
                 "`restart_strategy` option is an experimental feature."
                 " The interface can change in the future.",
                 ExperimentalWarning,
@@ -295,26 +312,39 @@
         if self._with_margin:
             warnings.warn(
                 "`with_margin` option is an experimental feature."
                 " The interface can change in the future.",
                 ExperimentalWarning,
             )
 
+        if self._lr_adapt:
+            warnings.warn(
+                "`lr_adapt` option is an experimental feature."
+                " The interface can change in the future.",
+                ExperimentalWarning,
+            )
+
         if source_trials is not None and (x0 is not None or sigma0 is not None):
             raise ValueError(
                 "It is prohibited to pass `source_trials` argument when "
                 "x0 or sigma0 is specified."
             )
 
         # TODO(c-bata): Support WS-sep-CMA-ES.
         if source_trials is not None and use_separable_cma:
             raise ValueError(
                 "It is prohibited to pass `source_trials` argument when using separable CMA-ES."
             )
 
+        if lr_adapt and (use_separable_cma or with_margin):
+            raise ValueError(
+                "It is prohibited to pass `use_separable_cma` or `with_margin` argument when "
+                "using `lr_adapt`."
+            )
+
         if restart_strategy not in (
             "ipop",
             "bipop",
             None,
         ):
             raise ValueError(
                 "restart_strategy={} is unsupported. "
@@ -686,14 +716,15 @@
             mean=mean,
             sigma=sigma0,
             cov=cov,
             bounds=trans.bounds,
             seed=self._cma_rng.randint(1, 2**31 - 2),
             n_max_resampling=10 * n_dimension,
             population_size=population_size,
+            lr_adapt=self._lr_adapt,
         )
 
     def sample_independent(
         self,
         study: "optuna.Study",
         trial: "optuna.trial.FrozenTrial",
         param_name: str,
```

### Comparing `optuna-3.2.0/optuna/samplers/_grid.py` & `optuna-3.3.0/optuna/samplers/_grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import collections
 import itertools
 from numbers import Real
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Mapping
 from typing import Optional
@@ -102,15 +101,15 @@
     def __init__(
         self, search_space: Mapping[str, Sequence[GridValueType]], seed: Optional[int] = None
     ) -> None:
         for param_name, param_values in search_space.items():
             for value in param_values:
                 self._check_value(param_name, value)
 
-        self._search_space = collections.OrderedDict()
+        self._search_space = {}
         for param_name, param_values in sorted(search_space.items()):
             self._search_space[param_name] = list(param_values)
 
         self._all_grids = list(itertools.product(*self._search_space.values()))
         self._param_names = sorted(search_space.keys())
         self._n_min_trials = len(self._all_grids)
         self._rng = np.random.RandomState(seed)
```

### Comparing `optuna-3.2.0/optuna/samplers/_nsgaiii.py` & `optuna-3.3.0/optuna/samplers/_nsgaiii.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 from __future__ import annotations
 
 from collections import defaultdict
+from collections.abc import Callable
+from collections.abc import Sequence
 import hashlib
 import itertools
 import math
 from typing import Any
-from typing import Callable
-from typing import Sequence
-import warnings
 
 import numpy as np
 
 import optuna
 from optuna._experimental import experimental_class
 from optuna.distributions import BaseDistribution
-from optuna.exceptions import ExperimentalWarning
-from optuna.samplers._base import _process_constraints_after_trial
 from optuna.samplers._base import BaseSampler
 from optuna.samplers._random import RandomSampler
-from optuna.samplers._search_space import IntersectionSearchSpace
-from optuna.samplers.nsgaii._crossover import perform_crossover
+from optuna.samplers.nsgaii._after_trial_strategy import NSGAIIAfterTrialStrategy
+from optuna.samplers.nsgaii._child_generation_strategy import NSGAIIChildGenerationStrategy
 from optuna.samplers.nsgaii._crossovers._base import BaseCrossover
 from optuna.samplers.nsgaii._crossovers._uniform import UniformCrossover
-from optuna.samplers.nsgaii._sampler import _constrained_dominates
-from optuna.samplers.nsgaii._sampler import _fast_non_dominated_sort
+from optuna.samplers.nsgaii._dominates import _constrained_dominates
+from optuna.samplers.nsgaii._dominates import _validate_constraints
+from optuna.samplers.nsgaii._elite_population_selection_strategy import _fast_non_dominated_sort
+from optuna.search_space import IntersectionSearchSpace
 from optuna.study import Study
 from optuna.study._multi_objective import _dominates
 from optuna.trial import FrozenTrial
 from optuna.trial import TrialState
 
 
 # Define key names of `Trial.system_attrs`.
 _GENERATION_KEY = "nsga3:generation"
 _POPULATION_CACHE_KEY_PREFIX = "nsga3:population"
+
 # Define a coefficient for scaling intervals, used in _filter_inf() to replace +-inf.
 _COEF = 3
 
 
 @experimental_class("3.2.0")
 class NSGAIIISampler(BaseSampler):
     """Multi-objective sampler using the NSGA-III algorithm.
@@ -61,65 +61,54 @@
             After non-dominated sort, who out of borderline front are going to survived is
             determined according to how sparse the closest reference point of each individual is.
             In the default setting the algorithm uses `uniformly` spread points to diversify the
             result. It is also possible to reflect your `preferences` by giving an arbitrary set of
             `target` points since the algorithm prioritizes individuals around reference points.
 
         dividing_parameter:
-            An parameter to determine the density of default reference points. This parameter
+            A parameter to determine the density of default reference points. This parameter
             determines how many divisions are made between reference points on each axis. The
             smaller this value is, the less reference points you have. The default value is 3.
             Note that this parameter is not used when ``reference_points`` is not :obj:`None`.
 
     .. note::
         Other parameters than ``reference_points`` and ``dividing_parameter`` are the same as
-        :class:`~optuna.samplers.nsgaii.NSGAIISampler`.
+        :class:`~optuna.samplers.NSGAIISampler`.
 
     """
 
     def __init__(
         self,
+        *,
         population_size: int = 50,
         mutation_prob: float | None = None,
         crossover: BaseCrossover | None = None,
         crossover_prob: float = 0.9,
         swapping_prob: float = 0.5,
         seed: int | None = None,
         constraints_func: Callable[[FrozenTrial], Sequence[float]] | None = None,
         reference_points: np.ndarray | None = None,
         dividing_parameter: int = 3,
+        child_generation_strategy: Callable[
+            [Study, dict[str, BaseDistribution], list[FrozenTrial]], dict[str, Any]
+        ]
+        | None = None,
+        after_trial_strategy: Callable[
+            [Study, FrozenTrial, TrialState, Sequence[float] | None], None
+        ]
+        | None = None,
     ) -> None:
         # TODO(ohta): Reconsider the default value of each parameter.
 
-        if not isinstance(population_size, int):
-            raise TypeError("`population_size` must be an integer value.")
-
         if population_size < 2:
             raise ValueError("`population_size` must be greater than or equal to 2.")
 
-        if not (mutation_prob is None or 0.0 <= mutation_prob <= 1.0):
-            raise ValueError(
-                "`mutation_prob` must be None or a float value within the range [0.0, 1.0]."
-            )
-
-        if not (0.0 <= crossover_prob <= 1.0):
-            raise ValueError("`crossover_prob` must be a float value within the range [0.0, 1.0].")
-
-        if not (0.0 <= swapping_prob <= 1.0):
-            raise ValueError("`swapping_prob` must be a float value within the range [0.0, 1.0].")
-
-        if constraints_func is not None:
-            warnings.warn(
-                "The constraints_func option is an experimental feature."
-                " The interface can change in the future.",
-                ExperimentalWarning,
-            )
-
         if crossover is None:
             crossover = UniformCrossover(swapping_prob)
+
         if not isinstance(crossover, BaseCrossover):
             raise ValueError(
                 f"'{crossover}' is not a valid crossover."
                 " For valid crossovers see"
                 " https://optuna.readthedocs.io/en/stable/reference/samplers.html."
             )
 
@@ -127,24 +116,34 @@
             raise ValueError(
                 f"Using {crossover},"
                 f" the population size should be greater than or equal to {crossover.n_parents}."
                 f" The specified `population_size` is {population_size}."
             )
 
         self._population_size = population_size
-        self._mutation_prob = mutation_prob
-        self._crossover = crossover
-        self._crossover_prob = crossover_prob
-        self._swapping_prob = swapping_prob
         self._random_sampler = RandomSampler(seed=seed)
         self._rng = np.random.RandomState(seed)
         self._constraints_func = constraints_func
         self._reference_points = reference_points
         self._dividing_parameter = dividing_parameter
         self._search_space = IntersectionSearchSpace()
+        self._child_generation_strategy = (
+            child_generation_strategy
+            or NSGAIIChildGenerationStrategy(
+                crossover_prob=crossover_prob,
+                mutation_prob=mutation_prob,
+                swapping_prob=swapping_prob,
+                crossover=crossover,
+                constraints_func=constraints_func,
+                seed=seed,
+            )
+        )
+        self._after_trial_strategy = after_trial_strategy or NSGAIIAfterTrialStrategy(
+            constraints_func=constraints_func
+        )
 
     def reseed_rng(self) -> None:
         self._random_sampler.reseed_rng()
         self._rng.seed()
 
     def infer_relative_search_space(
         self, study: Study, trial: FrozenTrial
@@ -163,51 +162,22 @@
     def sample_relative(
         self,
         study: Study,
         trial: FrozenTrial,
         search_space: dict[str, BaseDistribution],
     ) -> dict[str, Any]:
         parent_generation, parent_population = self._collect_parent_population(study)
-        trial_id = trial._trial_id
 
         generation = parent_generation + 1
-        study._storage.set_trial_system_attr(trial_id, _GENERATION_KEY, generation)
-
-        dominates_func = _dominates if self._constraints_func is None else _constrained_dominates
-
-        if parent_generation >= 0:
-            # We choose a child based on the specified crossover method.
-            if self._rng.rand() < self._crossover_prob:
-                child_params = perform_crossover(
-                    self._crossover,
-                    study,
-                    parent_population,
-                    search_space,
-                    self._rng,
-                    self._swapping_prob,
-                    dominates_func,
-                )
-            else:
-                parent_population_size = len(parent_population)
-                parent_params = parent_population[self._rng.choice(parent_population_size)].params
-                child_params = {name: parent_params[name] for name in search_space.keys()}
-
-            n_params = len(child_params)
-            if self._mutation_prob is None:
-                mutation_prob = 1.0 / max(1.0, n_params)
-            else:
-                mutation_prob = self._mutation_prob
+        study._storage.set_trial_system_attr(trial._trial_id, _GENERATION_KEY, generation)
 
-            params = {}
-            for param_name in child_params.keys():
-                if self._rng.rand() >= mutation_prob:
-                    params[param_name] = child_params[param_name]
-            return params
+        if parent_generation < 0:
+            return {}
 
-        return {}
+        return self._child_generation_strategy(study, search_space, parent_population)
 
     def sample_independent(
         self,
         study: Study,
         trial: FrozenTrial,
         param_name: str,
         param_distribution: BaseDistribution,
@@ -295,18 +265,19 @@
             parent_population = population
 
         return parent_generation, parent_population
 
     def _select_elite_population(
         self, study: Study, population: list[FrozenTrial]
     ) -> list[FrozenTrial]:
+        _validate_constraints(population, self._constraints_func)
+
+        dominates = _dominates if self._constraints_func is None else _constrained_dominates
+        population_per_rank = _fast_non_dominated_sort(population, study.directions, dominates)
         elite_population: list[FrozenTrial] = []
-        population_per_rank = _fast_non_dominated_sort(
-            population, study.directions, self._constraints_func
-        )
         for population in population_per_rank:
             if len(elite_population) + len(population) < self._population_size:
                 elite_population.extend(population)
             else:
                 n_objectives = len(study.directions)
                 # Construct reference points in the first run.
                 if self._reference_points is None:
@@ -348,16 +319,15 @@
         self,
         study: Study,
         trial: FrozenTrial,
         state: TrialState,
         values: Sequence[float] | None,
     ) -> None:
         assert state in [TrialState.COMPLETE, TrialState.FAIL, TrialState.PRUNED]
-        if self._constraints_func is not None:
-            _process_constraints_after_trial(self._constraints_func, study, trial, state)
+        self._after_trial_strategy(study, trial, state, values)
         self._random_sampler.after_trial(study, trial, state, values)
 
 
 # TODO(Shinichi) Replace with math.comb after support for python3.7 is deprecated.
 # This function calculates n multi-choose k, which is the total number of combinations with
 # repetition of size k from n items. This is equally re-written as math.comb(n+k-1, k)
 def _multi_choose(n: int, k: int) -> int:
```

### Comparing `optuna-3.2.0/optuna/samplers/_partial_fixed.py` & `optuna-3.3.0/optuna/samplers/_partial_fixed.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/samplers/_qmc.py` & `optuna-3.3.0/optuna/samplers/_qmc.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/samplers/_random.py` & `optuna-3.3.0/optuna/samplers/_random.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/samplers/_search_space/intersection.py` & `optuna-3.3.0/optuna/samplers/_search_space/intersection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from collections import OrderedDict
 import copy
 from typing import Dict
 from typing import Optional
 
 import optuna
 from optuna._deprecated import deprecated_class
 from optuna._deprecated import deprecated_func
@@ -47,16 +46,16 @@
         Args:
             study:
                 A study with completed trials. The same study must be passed for one instance
                 of this class through its lifetime.
             ordered_dict:
                 A boolean flag determining the return type.
                 If :obj:`False`, the returned object will be a :obj:`dict`.
-                If :obj:`True`, the returned object will be an :obj:`collections.OrderedDict`
-                sorted by keys, i.e. parameter names.
+                If :obj:`True`, the returned object will be a :obj:`dict` sorted by keys, i.e.
+                parameter names.
 
         Returns:
             A dictionary containing the parameter names and parameter's distributions.
 
         """
 
         if self._study_id is None:
@@ -97,15 +96,15 @@
                 if trial.distributions.get(name) == distribution
             }
 
         self._cursor = next_cursor
         search_space = self._search_space or {}
 
         if ordered_dict:
-            search_space = OrderedDict(sorted(search_space.items(), key=lambda x: x[0]))
+            search_space = dict(sorted(search_space.items(), key=lambda x: x[0]))
 
         return copy.deepcopy(search_space)
 
 
 @deprecated_func(
     "3.2.0",
     "4.0.0",
@@ -130,16 +129,16 @@
 
     Args:
         study:
             A study with completed trials.
         ordered_dict:
             A boolean flag determining the return type.
             If :obj:`False`, the returned object will be a :obj:`dict`.
-            If :obj:`True`, the returned object will be an :obj:`collections.OrderedDict` sorted by
-            keys, i.e. parameter names.
+            If :obj:`True`, the returned object will be a :obj:`dict` sorted by keys, i.e.
+            parameter names.
         include_pruned:
             Whether pruned trials should be included in the search space.
 
     Returns:
         A dictionary containing the parameter names and parameter's distributions.
     """
```

### Comparing `optuna-3.2.0/optuna/samplers/_tpe/_erf.py` & `optuna-3.3.0/optuna/samplers/_tpe/_erf.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,71 +34,79 @@
 # Coefficients for approximation to erf on [0,0.84375]
 
 pp0 = 1.28379167095512558561e-01
 pp1 = -3.25042107247001499370e-01
 pp2 = -2.84817495755985104766e-02
 pp3 = -5.77027029648944159157e-03
 pp4 = -2.37630166566501626084e-05
+pp = Polynomial([pp0, pp1, pp2, pp3, pp4])
 qq1 = 3.97917223959155352819e-01
 qq2 = 6.50222499887672944485e-02
 qq3 = 5.08130628187576562776e-03
 qq4 = 1.32494738004321644526e-04
 qq5 = -3.96022827877536812320e-06
+qq = Polynomial([one, qq1, qq2, qq3, qq4, qq5])
 
 # Coefficients for approximation to erf in [0.84375,1.25]
 
 pa0 = -2.36211856075265944077e-03
 pa1 = 4.14856118683748331666e-01
 pa2 = -3.72207876035701323847e-01
 pa3 = 3.18346619901161753674e-01
 pa4 = -1.10894694282396677476e-01
 pa5 = 3.54783043256182359371e-02
 pa6 = -2.16637559486879084300e-03
+pa = Polynomial([pa0, pa1, pa2, pa3, pa4, pa5, pa6])
 qa1 = 1.06420880400844228286e-01
 qa2 = 5.40397917702171048937e-01
 qa3 = 7.18286544141962662868e-02
 qa4 = 1.26171219808761642112e-01
 qa5 = 1.36370839120290507362e-02
 qa6 = 1.19844998467991074170e-02
+qa = Polynomial([one, qa1, qa2, qa3, qa4, qa5, qa6])
 
 # Coefficients for approximation to erfc in [1.25,1/0.35]
 
 ra0 = -9.86494403484714822705e-03
 ra1 = -6.93858572707181764372e-01
 ra2 = -1.05586262253232909814e01
 ra3 = -6.23753324503260060396e01
 ra4 = -1.62396669462573470355e02
 ra5 = -1.84605092906711035994e02
 ra6 = -8.12874355063065934246e01
 ra7 = -9.81432934416914548592e00
+ra = Polynomial([ra0, ra1, ra2, ra3, ra4, ra5, ra6, ra7])
 sa1 = 1.96512716674392571292e01
 sa2 = 1.37657754143519042600e02
 sa3 = 4.34565877475229228821e02
 sa4 = 6.45387271733267880336e02
 sa5 = 4.29008140027567833386e02
 sa6 = 1.08635005541779435134e02
 sa7 = 6.57024977031928170135e00
 sa8 = -6.04244152148580987438e-02
+sa = Polynomial([one, sa1, sa2, sa3, sa4, sa5, sa6, sa7, sa8])
 
 # Coefficients for approximation to erfc in [1/.35,28]
 
 rb0 = -9.86494292470009928597e-03
 rb1 = -7.99283237680523006574e-01
 rb2 = -1.77579549177547519889e01
 rb3 = -1.60636384855821916062e02
 rb4 = -6.37566443368389627722e02
 rb5 = -1.02509513161107724954e03
 rb6 = -4.83519191608651397019e02
+rb = Polynomial([rb0, rb1, rb2, rb3, rb4, rb5, rb6])
 sb1 = 3.03380607434824582924e01
 sb2 = 3.25792512996573918826e02
 sb3 = 1.53672958608443695994e03
 sb4 = 3.19985821950859553908e03
 sb5 = 2.55305040643316442583e03
 sb6 = 4.74528541206955367215e02
 sb7 = -2.24409524465858183362e01
+sb = Polynomial([one, sb1, sb2, sb3, sb4, sb5, sb6, sb7])
 
 
 def erf(x: np.ndarray) -> np.ndarray:
     a = np.abs(x)
 
     case_nan = np.isnan(x)
     case_posinf = np.isposinf(x)
@@ -111,53 +119,47 @@
     case_big = a >= 6
 
     def calc_case_tiny(x: np.ndarray) -> np.ndarray:
         return x + efx * x
 
     def calc_case_small1(x: np.ndarray) -> np.ndarray:
         z = x * x
-        r = Polynomial([pp0, pp1, pp2, pp3, pp4])(z)  # type: ignore[no-untyped-call]
-        s = Polynomial([one, qq1, qq2, qq3, qq4, qq5])(z)  # type: ignore[no-untyped-call]
+        r = pp(z)
+        s = qq(z)
         y = r / s
         return x + x * y
 
     def calc_case_small2(x: np.ndarray) -> np.ndarray:
         s = np.abs(x) - one
-        P = Polynomial([pa0, pa1, pa2, pa3, pa4, pa5, pa6])(s)  # type: ignore[no-untyped-call]
-        Q = Polynomial([one, qa1, qa2, qa3, qa4, qa5, qa6])(s)  # type: ignore[no-untyped-call]
+        P = pa(s)
+        Q = qa(s)
         absout = erx + P / Q
         return absout * np.sign(x)
 
     def calc_case_med1(x: np.ndarray) -> np.ndarray:
         sign = np.sign(x)
         x = np.abs(x)
         s = one / (x * x)
-        R = Polynomial([ra0, ra1, ra2, ra3, ra4, ra5, ra6, ra7])(  # type: ignore[no-untyped-call]
-            s
-        )
-        S = Polynomial(  # type: ignore[no-untyped-call]
-            [one, sa1, sa2, sa3, sa4, sa5, sa6, sa7, sa8]
-        )(s)
+        R = ra(s)
+        S = sa(s)
         # the following 3 lines are omitted for the following reasons:
         # (1) there are no easy way to implement SET_LOW_WORD equivalent method in NumPy
         # (2) we don't need very high accuracy in our use case.
         # z = x
         # SET_LOW_WORD(z, 0)
         # r = np.exp(-z * z - 0.5625) * np.exp((z - x) * (z + x) + R / S)
         r = np.exp(-x * x - 0.5625) * np.exp(R / S)
         return (one - r / x) * sign
 
     def calc_case_med2(x: np.ndarray) -> np.ndarray:
         sign = np.sign(x)
         x = np.abs(x)
         s = one / (x * x)
-        R = Polynomial([rb0, rb1, rb2, rb3, rb4, rb5, rb6])(s)  # type: ignore[no-untyped-call]
-        S = Polynomial([one, sb1, sb2, sb3, sb4, sb5, sb6, sb7])(  # type: ignore[no-untyped-call]
-            s
-        )
+        R = rb(s)
+        S = sb(s)
         # z = x
         # SET_LOW_WORD(z, 0)
         # r = np.exp(-z * z - 0.5625) * np.exp((z - x) * (z + x) + R / S)
         r = np.exp(-x * x - 0.5625) * np.exp(R / S)
         return (one - r / x) * sign
 
     def calc_case_big(x: np.ndarray) -> np.ndarray:
```

### Comparing `optuna-3.2.0/optuna/samplers/_tpe/_truncnorm.py` & `optuna-3.3.0/optuna/samplers/_tpe/_truncnorm.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
     b: Union[np.ndarray, float],
     loc: Union[np.ndarray, float] = 0,
     scale: Union[np.ndarray, float] = 1,
 ) -> np.ndarray:
     x = (x - loc) / scale
 
     x, a, b = np.atleast_1d(x, a, b)
-    x, a, b = np.broadcast_arrays(x, a, b)
 
     out = _norm_logpdf(x) - _log_gauss_mass(a, b)
 
+    x, a, b = np.broadcast_arrays(x, a, b)
     out[(x < a) | (b < x)] = -np.inf
     out[a == b] = math.nan
 
     return out
```

### Comparing `optuna-3.2.0/optuna/samplers/_tpe/multi_objective_sampler.py` & `optuna-3.3.0/optuna/samplers/_tpe/multi_objective_sampler.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/samplers/_tpe/parzen_estimator.py` & `optuna-3.3.0/optuna/samplers/_tpe/parzen_estimator.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/samplers/_tpe/probability_distributions.py` & `optuna-3.3.0/optuna/samplers/_tpe/probability_distributions.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/samplers/_tpe/sampler.py` & `optuna-3.3.0/optuna/samplers/_tpe/sampler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from __future__ import annotations
+
 import math
 from typing import Any
 from typing import Callable
-from typing import Container
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 import warnings
@@ -252,19 +253,17 @@
             consider_prior,
             prior_weight,
             consider_magic_clip,
             consider_endpoints,
             weights,
             multivariate,
         )
-        self._prior_weight = prior_weight
         self._n_startup_trials = n_startup_trials
         self._n_ei_candidates = n_ei_candidates
         self._gamma = gamma
-        self._weights = weights
 
         self._warn_independent_sampling = warn_independent_sampling
         self._rng = np.random.RandomState(seed)
         self._random_sampler = RandomSampler(seed=seed)
 
         self._multivariate = multivariate
         self._group = group
@@ -333,29 +332,14 @@
         for name, distribution in self._search_space.calculate(study).items():
             if distribution.single():
                 continue
             search_space[name] = distribution
 
         return search_space
 
-    def _log_independent_sampling(
-        self, n_complete_trials: int, trial: FrozenTrial, param_name: str
-    ) -> None:
-        if self._warn_independent_sampling and self._multivariate:
-            # The first trial samples independently.
-            if n_complete_trials >= max(self._n_startup_trials, 1):
-                _logger.warning(
-                    f"The parameter '{param_name}' in trial#{trial.number} is sampled "
-                    "independently instead of being sampled by multivariate TPE sampler. "
-                    "(optimization performance may be degraded). "
-                    "You can suppress this warning by setting `warn_independent_sampling` "
-                    "to `False` in the constructor of `TPESampler`, "
-                    "if this independent sampling is intended behavior."
-                )
-
     def sample_relative(
         self, study: Study, trial: FrozenTrial, search_space: Dict[str, BaseDistribution]
     ) -> Dict[str, Any]:
         if self._group:
             assert self._search_space_group is not None
             params = {}
             for sub_space in self._search_space_group.search_spaces:
@@ -371,116 +355,115 @@
 
     def _sample_relative(
         self, study: Study, trial: FrozenTrial, search_space: Dict[str, BaseDistribution]
     ) -> Dict[str, Any]:
         if search_space == {}:
             return {}
 
-        param_names = list(search_space.keys())
-        values, scores, violations = _get_observation_pairs(
-            study,
-            param_names,
-            self._constant_liar,
-            self._constraints_func is not None,
-        )
-
+        states = (TrialState.COMPLETE, TrialState.PRUNED)
+        trials = study._get_trials(deepcopy=False, states=states, use_cache=True)
         # If the number of samples is insufficient, we run random trial.
-        n = sum(s < float("inf") for s, v in scores)  # Ignore running trials.
-        if n < self._n_startup_trials:
+        if len(trials) < self._n_startup_trials:
             return {}
 
-        # We divide data into below and above.
-        indices_below, indices_above = _split_observation_pairs(scores, self._gamma(n), violations)
-        # `None` items are intentionally converted to `nan` and then filtered out.
-        # For `nan` conversion, the dtype must be float.
-        # `None` items appear when `group=True` or `constant_liar=True`.
-        config_values = {k: np.asarray(v, dtype=float) for k, v in values.items()}
-        param_mask = np.all(~np.isnan(list(config_values.values())), axis=0)
-        param_mask_below, param_mask_above = param_mask[indices_below], param_mask[indices_above]
-        below = {k: v[indices_below[param_mask_below]] for k, v in config_values.items()}
-        above = {k: v[indices_above[param_mask_above]] for k, v in config_values.items()}
-
-        # We then sample by maximizing log likelihood ratio.
-        if study._is_multi_objective():
-            weights_below = _calculate_weights_below_for_multi_objective(
-                scores, indices_below, violations
-            )[param_mask_below]
-            mpe_below = _ParzenEstimator(
-                below, search_space, self._parzen_estimator_parameters, weights_below
-            )
-        else:
-            mpe_below = _ParzenEstimator(below, search_space, self._parzen_estimator_parameters)
-        mpe_above = _ParzenEstimator(above, search_space, self._parzen_estimator_parameters)
-        samples_below = mpe_below.sample(self._rng, self._n_ei_candidates)
-        log_likelihoods_below = mpe_below.log_pdf(samples_below)
-        log_likelihoods_above = mpe_above.log_pdf(samples_below)
-        ret = TPESampler._compare(samples_below, log_likelihoods_below, log_likelihoods_above)
-
-        for param_name, dist in search_space.items():
-            ret[param_name] = dist.to_external_repr(ret[param_name])
-
-        return ret
+        return self._sample(study, trial, search_space)
 
     def sample_independent(
         self,
         study: Study,
         trial: FrozenTrial,
         param_name: str,
         param_distribution: BaseDistribution,
     ) -> Any:
-        values, scores, violations = _get_observation_pairs(
+        states = (TrialState.COMPLETE, TrialState.PRUNED)
+        trials = study._get_trials(deepcopy=False, states=states, use_cache=True)
+
+        # If the number of samples is insufficient, we run random trial.
+        if len(trials) < self._n_startup_trials:
+            return self._random_sampler.sample_independent(
+                study, trial, param_name, param_distribution
+            )
+
+        if self._warn_independent_sampling and self._multivariate:
+            # Avoid independent warning at the first sampling of `param_name`.
+            if any(param_name in trial.params for trial in trials):
+                _logger.warning(
+                    f"The parameter '{param_name}' in trial#{trial.number} is sampled "
+                    "independently instead of being sampled by multivariate TPE sampler. "
+                    "(optimization performance may be degraded). "
+                    "You can suppress this warning by setting `warn_independent_sampling` "
+                    "to `False` in the constructor of `TPESampler`, "
+                    "if this independent sampling is intended behavior."
+                )
+
+        return self._sample(study, trial, {param_name: param_distribution})[param_name]
+
+    def _get_internal_repr(
+        self, trials: list[FrozenTrial], search_space: dict[str, BaseDistribution]
+    ) -> dict[str, np.ndarray]:
+        values: dict[str, list[float]] = {param_name: [] for param_name in search_space}
+        for trial in trials:
+            if all((param_name in trial.params) for param_name in search_space):
+                for param_name in search_space:
+                    param = trial.params[param_name]
+                    distribution = trial.distributions[param_name]
+                    values[param_name].append(distribution.to_internal_repr(param))
+        return {k: np.asarray(v) for k, v in values.items()}
+
+    def _sample(
+        self, study: Study, trial: FrozenTrial, search_space: Dict[str, BaseDistribution]
+    ) -> Dict[str, Any]:
+        if self._constant_liar and not study._is_multi_objective():
+            states = [TrialState.COMPLETE, TrialState.PRUNED, TrialState.RUNNING]
+        else:
+            states = [TrialState.COMPLETE, TrialState.PRUNED]
+        use_cache = not self._constant_liar
+        trials = study._get_trials(deepcopy=False, states=states, use_cache=use_cache)
+
+        scores, violations = _get_observation_pairs(
             study,
-            [param_name],
-            self._constant_liar,
+            trials,
             self._constraints_func is not None,
         )
 
         n = sum(s < float("inf") for s, v in scores)  # Ignore running trials.
 
-        # Avoid independent warning at the first sampling of `param_name` when `group=True`.
-        if any(param is not None for param in values[param_name]):
-            self._log_independent_sampling(n, trial, param_name)
-
-        if n < self._n_startup_trials:
-            return self._random_sampler.sample_independent(
-                study, trial, param_name, param_distribution
-            )
-
+        # We divide data into below and above.
         indices_below, indices_above = _split_observation_pairs(scores, self._gamma(n), violations)
-        # `None` items are intentionally converted to `nan` and then filtered out.
-        # For `nan` conversion, the dtype must be float.
-        config_value = np.asarray(values[param_name], dtype=float)
-        param_mask = ~np.isnan(config_value)
-        param_mask_below, param_mask_above = param_mask[indices_below], param_mask[indices_above]
-        below = {param_name: config_value[indices_below[param_mask_below]]}
-        above = {param_name: config_value[indices_above[param_mask_above]]}
 
+        below_trials = np.asarray(trials, dtype=object)[indices_below].tolist()
+        above_trials = np.asarray(trials, dtype=object)[indices_above].tolist()
+        below = self._get_internal_repr(below_trials, search_space)
+        above = self._get_internal_repr(above_trials, search_space)
+
+        # We then sample by maximizing log likelihood ratio.
         if study._is_multi_objective():
+            param_mask_below = []
+            for trial in below_trials:
+                param_mask_below.append(
+                    all((param_name in trial.params) for param_name in search_space)
+                )
             weights_below = _calculate_weights_below_for_multi_objective(
-                scores, indices_below, violations
+                study, below_trials, self._constraints_func
             )[param_mask_below]
             mpe_below = _ParzenEstimator(
-                below,
-                {param_name: param_distribution},
-                self._parzen_estimator_parameters,
-                weights_below,
+                below, search_space, self._parzen_estimator_parameters, weights_below
             )
         else:
-            mpe_below = _ParzenEstimator(
-                below, {param_name: param_distribution}, self._parzen_estimator_parameters
-            )
-        mpe_above = _ParzenEstimator(
-            above, {param_name: param_distribution}, self._parzen_estimator_parameters
-        )
+            mpe_below = _ParzenEstimator(below, search_space, self._parzen_estimator_parameters)
+        mpe_above = _ParzenEstimator(above, search_space, self._parzen_estimator_parameters)
         samples_below = mpe_below.sample(self._rng, self._n_ei_candidates)
         log_likelihoods_below = mpe_below.log_pdf(samples_below)
         log_likelihoods_above = mpe_above.log_pdf(samples_below)
         ret = TPESampler._compare(samples_below, log_likelihoods_below, log_likelihoods_above)
 
-        return param_distribution.to_external_repr(ret[param_name])
+        for param_name, dist in search_space.items():
+            ret[param_name] = dist.to_external_repr(ret[param_name])
+
+        return ret
 
     @classmethod
     def _compare(
         cls,
         samples: Dict[str, np.ndarray],
         log_l: np.ndarray,
         log_g: np.ndarray,
@@ -571,22 +554,17 @@
         ranks[(counts == 0) & (ranks == -1)] = rank
         rank += 1
     return ranks
 
 
 def _get_observation_pairs(
     study: Study,
-    param_names: List[str],
-    constant_liar: bool = False,  # TODO(hvy): Remove default value and fix unit tests.
+    trials: list[FrozenTrial],
     constraints_enabled: bool = False,
-) -> Tuple[
-    Dict[str, List[Optional[float]]],
-    List[Tuple[float, List[float]]],
-    Optional[List[float]],
-]:
+) -> tuple[list[tuple[float, list[float]]], list[float] | None]:
     """Get observation pairs from the study.
 
     This function collects observation pairs from the complete or pruned trials of the study.
     In addition, if ``constant_liar`` is :obj:`True`, the running trials are considered.
     The values for trials that don't contain the parameter in the ``param_names`` are skipped.
 
     An observation pair fundamentally consists of a parameter value and an objective value.
@@ -608,61 +586,39 @@
     signs = []
     for d in study.directions:
         if d == StudyDirection.MINIMIZE:
             signs.append(1)
         else:
             signs.append(-1)
 
-    states: Container[TrialState]
-    if constant_liar:
-        states = (TrialState.COMPLETE, TrialState.PRUNED, TrialState.RUNNING)
-    else:
-        states = (TrialState.COMPLETE, TrialState.PRUNED)
-
     scores = []
-    values: Dict[str, List[Optional[float]]] = {param_name: [] for param_name in param_names}
     violations: Optional[List[float]] = [] if constraints_enabled else None
-    for trial in study._get_trials(deepcopy=False, states=states, use_cache=not constant_liar):
+    for trial in trials:
         # We extract score from the trial.
         if trial.state is TrialState.COMPLETE:
-            if trial.values is None:
-                continue
+            assert trial.values is not None
             score = (-float("inf"), [sign * v for sign, v in zip(signs, trial.values)])
         elif trial.state is TrialState.PRUNED:
-            if study._is_multi_objective():
-                continue
+            assert not study._is_multi_objective()
 
             if len(trial.intermediate_values) > 0:
                 step, intermediate_value = max(trial.intermediate_values.items())
                 if math.isnan(intermediate_value):
                     score = (-step, [float("inf")])
                 else:
                     score = (-step, [signs[0] * intermediate_value])
             else:
                 score = (1, [0.0])
         elif trial.state is TrialState.RUNNING:
-            if study._is_multi_objective():
-                continue
-
-            assert constant_liar
+            assert not study._is_multi_objective()
             score = (float("inf"), [signs[0] * float("inf")])
         else:
             assert False
         scores.append(score)
 
-        # We extract param_value from the trial.
-        for param_name in param_names:
-            param_value: Optional[float]
-            if param_name in trial.params:
-                distribution = trial.distributions[param_name]
-                param_value = distribution.to_internal_repr(trial.params[param_name])
-            else:
-                param_value = None
-            values[param_name].append(param_value)
-
         if constraints_enabled:
             assert violations is not None
             if trial.state != TrialState.RUNNING:
                 constraint = trial.system_attrs.get(_CONSTRAINTS_KEY)
                 if constraint is None:
                     warnings.warn(
                         f"Trial {trial.number} does not have constraint values."
@@ -672,15 +628,15 @@
                 else:
                     # Violation values of infeasible dimensions are summed up.
                     violation = sum(v for v in constraint if v > 0)
                 violations.append(violation)
             else:
                 violations.append(float("inf"))
 
-    return values, scores, violations
+    return scores, violations
 
 
 def _split_observation_pairs(
     loss_vals: List[Tuple[float, List[float]]],
     n_below: int,
     violations: Optional[List[float]],
 ) -> Tuple[np.ndarray, np.ndarray]:
@@ -758,26 +714,34 @@
 
         indices_above = np.setdiff1d(indices, indices_below)
 
     return indices_below, indices_above
 
 
 def _calculate_weights_below_for_multi_objective(
-    loss_vals: List[Tuple[float, List[float]]],
-    indices: np.ndarray,
-    violations: Optional[List[float]],
+    study: Study,
+    below_trials: list[FrozenTrial],
+    constraints_func: Callable[[FrozenTrial], Sequence[float]] | None,
 ) -> np.ndarray:
-    if violations is None:
-        feasible_mask = np.ones(len(indices), dtype=bool)
-    else:
+    loss_vals = []
+    feasible_mask = np.ones(len(below_trials), dtype=bool)
+    for i, trial in enumerate(below_trials):
         # Hypervolume contributions are calculated only using feasible trials.
-        feasible_mask = np.array(violations, dtype=float)[indices] == 0
-
-    # Multi-objective TPE does not support pruning, so it ignores the ``step``.
-    lvals = np.asarray([v for _, v in loss_vals])[indices[feasible_mask]]
+        if constraints_func is not None:
+            if any(constraint > 0 for constraint in constraints_func(trial)):
+                feasible_mask[i] = False
+                continue
+        values = []
+        for value, direction in zip(trial.values, study.directions):
+            if direction == StudyDirection.MINIMIZE:
+                values.append(value)
+            else:
+                values.append(-value)
+        loss_vals.append(values)
+    lvals = np.asarray(loss_vals, dtype=float)
 
     # Calculate weights based on hypervolume contributions.
     n_below = len(lvals)
     weights_below: np.ndarray
     if n_below == 0:
         weights_below = np.asarray([])
     elif n_below == 1:
@@ -791,10 +755,10 @@
         contributions = np.asarray(
             [hv - WFG().compute(lvals[indices_mat[i]], reference_point) for i in range(n_below)]
         )
         contributions += EPS
         weights_below = np.clip(contributions / np.max(contributions), 0, 1)
 
     # For now, EPS weight is assigned to infeasible trials.
-    weights_below_all = np.full(len(indices), EPS)
+    weights_below_all = np.full(len(below_trials), EPS)
     weights_below_all[feasible_mask] = weights_below
     return weights_below_all
```

### Comparing `optuna-3.2.0/optuna/samplers/nsgaii/__init__.py` & `optuna-3.3.0/optuna/samplers/nsgaii/__init__.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/samplers/nsgaii/_crossover.py` & `optuna-3.3.0/optuna/samplers/nsgaii/_crossover.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_base.py` & `optuna-3.3.0/optuna/samplers/nsgaii/_crossovers/_base.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_blxalpha.py` & `optuna-3.3.0/optuna/samplers/nsgaii/_crossovers/_blxalpha.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_sbx.py` & `optuna-3.3.0/optuna/samplers/nsgaii/_crossovers/_sbx.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_spx.py` & `optuna-3.3.0/optuna/samplers/nsgaii/_crossovers/_spx.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_undx.py` & `optuna-3.3.0/optuna/samplers/nsgaii/_crossovers/_undx.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_uniform.py` & `optuna-3.3.0/optuna/samplers/nsgaii/_crossovers/_uniform.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,16 @@
         swapping_prob:
             Probability of swapping each parameter of the parents during crossover.
     """
 
     n_parents = 2
 
     def __init__(self, swapping_prob: float = 0.5) -> None:
+        if not (0.0 <= swapping_prob <= 1.0):
+            raise ValueError("`swapping_prob` must be a float value within the range [0.0, 1.0].")
         self._swapping_prob = swapping_prob
 
     def crossover(
         self,
         parents_params: np.ndarray,
         rng: np.random.RandomState,
         study: Study,
```

### Comparing `optuna-3.2.0/optuna/samplers/nsgaii/_crossovers/_vsbx.py` & `optuna-3.3.0/optuna/samplers/nsgaii/_crossovers/_vsbx.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/samplers/nsgaii/_sampler.py` & `optuna-3.3.0/optuna/samplers/nsgaii/_sampler.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,32 @@
+from __future__ import annotations
+
 from collections import defaultdict
+from collections.abc import Callable
+from collections.abc import Sequence
 import hashlib
-import itertools
 from typing import Any
-from typing import Callable
-from typing import cast
-from typing import DefaultDict
-from typing import Dict
-from typing import List
-from typing import Optional
-from typing import Sequence
-from typing import Tuple
 import warnings
 
 import numpy as np
 
 import optuna
 from optuna.distributions import BaseDistribution
 from optuna.exceptions import ExperimentalWarning
-from optuna.samplers._base import _CONSTRAINTS_KEY
-from optuna.samplers._base import _process_constraints_after_trial
 from optuna.samplers._base import BaseSampler
 from optuna.samplers._random import RandomSampler
-from optuna.samplers.nsgaii._crossover import perform_crossover
+from optuna.samplers.nsgaii._after_trial_strategy import NSGAIIAfterTrialStrategy
+from optuna.samplers.nsgaii._child_generation_strategy import NSGAIIChildGenerationStrategy
 from optuna.samplers.nsgaii._crossovers._base import BaseCrossover
 from optuna.samplers.nsgaii._crossovers._uniform import UniformCrossover
+from optuna.samplers.nsgaii._elite_population_selection_strategy import (
+    NSGAIIElitePopulationSelectionStrategy,
+)
 from optuna.search_space import IntersectionSearchSpace
 from optuna.study import Study
-from optuna.study import StudyDirection
-from optuna.study._multi_objective import _dominates
 from optuna.trial import FrozenTrial
 from optuna.trial import TrialState
 
 
 # Define key names of `Trial.system_attrs`.
 _GENERATION_KEY = "nsga2:generation"
 _POPULATION_CACHE_KEY_PREFIX = "nsga2:population"
@@ -104,141 +99,174 @@
             3. Trial x and y are feasible and trial x dominates trial y.
 
             .. note::
                 Added in v2.5.0 as an experimental feature. The interface may change in newer
                 versions without prior notice. See
                 https://github.com/optuna/optuna/releases/tag/v2.5.0.
 
+        elite_population_selection_strategy:
+            The selection strategy for determining the individuals to survive from the current
+            population pool. Default to :obj:`None`.
+
+            .. note::
+                The arguments ``elite_population_selection_strategy`` was added in v3.3.0 as an
+                experimental feature. The interface may change in newer versions without prior
+                notice.
+                See https://github.com/optuna/optuna/releases/tag/v3.3.0.
+
+        child_generation_strategy:
+            The strategy for generating child parameters from parent trials. Defaults to
+            :obj:`None`.
+
+            .. note::
+                The arguments ``child_generation_strategy`` was added in v3.3.0 as an experimental
+                feature. The interface may change in newer versions without prior notice.
+                See https://github.com/optuna/optuna/releases/tag/v3.3.0.
+
+        after_trial_strategy:
+            A set of procedure to be conducted after each trial. Defaults to :obj:`None`.
+
+            .. note::
+                The arguments ``after_trial_strategy`` was added in v3.3.0 as an experimental
+                feature. The interface may change in newer versions without prior notice.
+                See https://github.com/optuna/optuna/releases/tag/v3.3.0.
     """
 
     def __init__(
         self,
         *,
         population_size: int = 50,
-        mutation_prob: Optional[float] = None,
-        crossover: Optional[BaseCrossover] = None,
+        mutation_prob: float | None = None,
+        crossover: BaseCrossover | None = None,
         crossover_prob: float = 0.9,
         swapping_prob: float = 0.5,
-        seed: Optional[int] = None,
-        constraints_func: Optional[Callable[[FrozenTrial], Sequence[float]]] = None,
+        seed: int | None = None,
+        constraints_func: Callable[[FrozenTrial], Sequence[float]] | None = None,
+        elite_population_selection_strategy: Callable[
+            [Study, list[FrozenTrial]], list[FrozenTrial]
+        ]
+        | None = None,
+        child_generation_strategy: Callable[
+            [Study, dict[str, BaseDistribution], list[FrozenTrial]], dict[str, Any]
+        ]
+        | None = None,
+        after_trial_strategy: Callable[
+            [Study, FrozenTrial, TrialState, Sequence[float] | None], None
+        ]
+        | None = None,
     ) -> None:
         # TODO(ohta): Reconsider the default value of each parameter.
 
-        if not isinstance(population_size, int):
-            raise TypeError("`population_size` must be an integer value.")
-
         if population_size < 2:
             raise ValueError("`population_size` must be greater than or equal to 2.")
 
-        if not (mutation_prob is None or 0.0 <= mutation_prob <= 1.0):
-            raise ValueError(
-                "`mutation_prob` must be None or a float value within the range [0.0, 1.0]."
+        if constraints_func is not None:
+            warnings.warn(
+                "The constraints_func option is an experimental feature."
+                " The interface can change in the future.",
+                ExperimentalWarning,
+            )
+        if after_trial_strategy is not None:
+            warnings.warn(
+                "The after_trial_strategy option is an experimental feature."
+                " The interface can change in the future.",
+                ExperimentalWarning,
             )
 
-        if not (0.0 <= crossover_prob <= 1.0):
-            raise ValueError("`crossover_prob` must be a float value within the range [0.0, 1.0].")
-
-        if not (0.0 <= swapping_prob <= 1.0):
-            raise ValueError("`swapping_prob` must be a float value within the range [0.0, 1.0].")
+        if child_generation_strategy is not None:
+            warnings.warn(
+                "The child_generation_strategy option is an experimental feature."
+                " The interface can change in the future.",
+                ExperimentalWarning,
+            )
 
-        if constraints_func is not None:
+        if elite_population_selection_strategy is not None:
             warnings.warn(
-                "The constraints_func option is an experimental feature."
+                "The elite_population_selection_strategy option is an experimental feature."
                 " The interface can change in the future.",
                 ExperimentalWarning,
             )
 
         if crossover is None:
             crossover = UniformCrossover(swapping_prob)
 
         if not isinstance(crossover, BaseCrossover):
             raise ValueError(
                 f"'{crossover}' is not a valid crossover."
                 " For valid crossovers see"
                 " https://optuna.readthedocs.io/en/stable/reference/samplers.html."
             )
+
         if population_size < crossover.n_parents:
             raise ValueError(
                 f"Using {crossover},"
                 f" the population size should be greater than or equal to {crossover.n_parents}."
                 f" The specified `population_size` is {population_size}."
             )
 
         self._population_size = population_size
-        self._mutation_prob = mutation_prob
-        self._crossover = crossover
-        self._crossover_prob = crossover_prob
-        self._swapping_prob = swapping_prob
         self._random_sampler = RandomSampler(seed=seed)
         self._rng = np.random.RandomState(seed)
         self._constraints_func = constraints_func
         self._search_space = IntersectionSearchSpace()
 
+        self._elite_population_selection_strategy = (
+            elite_population_selection_strategy
+            or NSGAIIElitePopulationSelectionStrategy(
+                population_size=population_size, constraints_func=constraints_func
+            )
+        )
+        self._child_generation_strategy = (
+            child_generation_strategy
+            or NSGAIIChildGenerationStrategy(
+                crossover_prob=crossover_prob,
+                mutation_prob=mutation_prob,
+                swapping_prob=swapping_prob,
+                crossover=crossover,
+                constraints_func=constraints_func,
+                seed=seed,
+            )
+        )
+        self._after_trial_strategy = after_trial_strategy or NSGAIIAfterTrialStrategy(
+            constraints_func=constraints_func
+        )
+
     def reseed_rng(self) -> None:
         self._random_sampler.reseed_rng()
         self._rng.seed()
 
     def infer_relative_search_space(
         self, study: Study, trial: FrozenTrial
-    ) -> Dict[str, BaseDistribution]:
-        search_space: Dict[str, BaseDistribution] = {}
+    ) -> dict[str, BaseDistribution]:
+        search_space: dict[str, BaseDistribution] = {}
         for name, distribution in self._search_space.calculate(study).items():
             if distribution.single():
                 # The `untransform` method of `optuna._transform._SearchSpaceTransform`
                 # does not assume a single value,
                 # so single value objects are not sampled with the `sample_relative` method,
                 # but with the `sample_independent` method.
                 continue
             search_space[name] = distribution
         return search_space
 
     def sample_relative(
         self,
         study: Study,
         trial: FrozenTrial,
-        search_space: Dict[str, BaseDistribution],
-    ) -> Dict[str, Any]:
+        search_space: dict[str, BaseDistribution],
+    ) -> dict[str, Any]:
         parent_generation, parent_population = self._collect_parent_population(study)
-        trial_id = trial._trial_id
 
         generation = parent_generation + 1
-        study._storage.set_trial_system_attr(trial_id, _GENERATION_KEY, generation)
+        study._storage.set_trial_system_attr(trial._trial_id, _GENERATION_KEY, generation)
 
-        dominates_func = _dominates if self._constraints_func is None else _constrained_dominates
+        if parent_generation < 0:
+            return {}
 
-        if parent_generation >= 0:
-            # We choose a child based on the specified crossover method.
-            if self._rng.rand() < self._crossover_prob:
-                child_params = perform_crossover(
-                    self._crossover,
-                    study,
-                    parent_population,
-                    search_space,
-                    self._rng,
-                    self._swapping_prob,
-                    dominates_func,
-                )
-            else:
-                parent_population_size = len(parent_population)
-                parent_params = parent_population[self._rng.choice(parent_population_size)].params
-                child_params = {name: parent_params[name] for name in search_space.keys()}
-
-            n_params = len(child_params)
-            if self._mutation_prob is None:
-                mutation_prob = 1.0 / max(1.0, n_params)
-            else:
-                mutation_prob = self._mutation_prob
-
-            params = {}
-            for param_name in child_params.keys():
-                if self._rng.rand() >= mutation_prob:
-                    params[param_name] = child_params[param_name]
-            return params
-
-        return {}
+        return self._child_generation_strategy(study, search_space, parent_population)
 
     def sample_independent(
         self,
         study: Study,
         trial: FrozenTrial,
         param_name: str,
         param_distribution: BaseDistribution,
@@ -248,15 +276,15 @@
         # 2. A parameter to mutate.
         # 3. A parameter excluded from the intersection search space.
 
         return self._random_sampler.sample_independent(
             study, trial, param_name, param_distribution
         )
 
-    def _collect_parent_population(self, study: Study) -> Tuple[int, List[FrozenTrial]]:
+    def _collect_parent_population(self, study: Study) -> tuple[int, list[FrozenTrial]]:
         trials = study._get_trials(deepcopy=False, use_cache=True)
 
         generation_to_runnings = defaultdict(list)
         generation_to_population = defaultdict(list)
         for trial in trials:
             if _GENERATION_KEY not in trial.system_attrs:
                 continue
@@ -267,15 +295,15 @@
                     generation_to_runnings[generation].append(trial)
                 continue
 
             # Do not use trials whose states are not COMPLETE, or `constraint` will be unavailable.
             generation_to_population[generation].append(trial)
 
         hasher = hashlib.sha256()
-        parent_population: List[FrozenTrial] = []
+        parent_population: list[FrozenTrial] = []
         parent_generation = -1
         while True:
             generation = parent_generation + 1
             population = generation_to_population[generation]
 
             # Under multi-worker settings, the population size might become larger than
             # `self._population_size`.
@@ -305,15 +333,15 @@
                 cache_key, (-1, [])
             )
             if cached_generation >= generation:
                 generation = cached_generation
                 population = [trials[n] for n in cached_population_numbers]
             else:
                 population.extend(parent_population)
-                population = self._select_elite_population(study, population)
+                population = self._elite_population_selection_strategy(study, population)
 
                 # To reduce the number of system attribute entries,
                 # we cache the population information only if there are no running trials
                 # (i.e., the information of the population has been fixed).
                 # Usually, if there are no too delayed running trials, the single entry
                 # will be used.
                 if len(generation_to_runnings[generation]) == 0:
@@ -323,217 +351,17 @@
                     )
 
             parent_generation = generation
             parent_population = population
 
         return parent_generation, parent_population
 
-    def _select_elite_population(
-        self, study: Study, population: List[FrozenTrial]
-    ) -> List[FrozenTrial]:
-        elite_population: List[FrozenTrial] = []
-        population_per_rank = _fast_non_dominated_sort(
-            population, study.directions, self._constraints_func
-        )
-        for population in population_per_rank:
-            if len(elite_population) + len(population) < self._population_size:
-                elite_population.extend(population)
-            else:
-                n = self._population_size - len(elite_population)
-                _crowding_distance_sort(population)
-                elite_population.extend(population[:n])
-                break
-
-        return elite_population
-
     def after_trial(
         self,
         study: Study,
         trial: FrozenTrial,
         state: TrialState,
-        values: Optional[Sequence[float]],
+        values: Sequence[float] | None,
     ) -> None:
         assert state in [TrialState.COMPLETE, TrialState.FAIL, TrialState.PRUNED]
-        if self._constraints_func is not None:
-            _process_constraints_after_trial(self._constraints_func, study, trial, state)
+        self._after_trial_strategy(study, trial, state, values)
         self._random_sampler.after_trial(study, trial, state, values)
-
-
-def _calc_crowding_distance(population: List[FrozenTrial]) -> DefaultDict[int, float]:
-    """Calculates the crowding distance of population.
-
-    We define the crowding distance as the summation of the crowding distance of each dimension
-    of value calculated as follows:
-
-    * If all values in that dimension are the same, i.e., [1, 1, 1] or [inf, inf],
-      the crowding distances of all trials in that dimension are zero.
-    * Otherwise, the crowding distances of that dimension is the difference between
-      two nearest values besides that value, one above and one below, divided by the difference
-      between the maximal and minimal finite value of that dimension. Please note that:
-        * the nearest value below the minimum is considered to be -inf and the
-          nearest value above the maximum is considered to be inf, and
-        * inf - inf and (-inf) - (-inf) is considered to be zero.
-    """
-
-    manhattan_distances: DefaultDict[int, float] = defaultdict(float)
-    if len(population) == 0:
-        return manhattan_distances
-
-    for i in range(len(population[0].values)):
-        population.sort(key=lambda x: cast(float, x.values[i]))
-
-        # If population have the same values[i], ignore that value.
-        if population[0].values[i] == population[-1].values[i]:
-            continue
-
-        vs = (
-            [-float("inf")]
-            + [cast(List[float], population[j].values)[i] for j in range(len(population))]
-            + [float("inf")]
-        )
-
-        # Smallest finite value.
-        v_min = next(x for x in vs if x != -float("inf"))
-
-        # Largest finite value.
-        v_max = next(x for x in reversed(vs) if x != float("inf"))
-
-        width = v_max - v_min
-        if width <= 0:
-            # width == 0 or width == -inf
-            width = 1.0
-
-        for j in range(len(population)):
-            # inf - inf and (-inf) - (-inf) is considered to be zero.
-            gap = 0.0 if vs[j] == vs[j + 2] else vs[j + 2] - vs[j]
-            manhattan_distances[population[j].number] += gap / width
-    return manhattan_distances
-
-
-def _crowding_distance_sort(population: List[FrozenTrial]) -> None:
-    manhattan_distances = _calc_crowding_distance(population)
-    population.sort(key=lambda x: manhattan_distances[x.number])
-    population.reverse()
-
-
-def _constrained_dominates(
-    trial0: FrozenTrial, trial1: FrozenTrial, directions: Sequence[StudyDirection]
-) -> bool:
-    """Checks constrained-domination.
-
-    A trial x is said to constrained-dominate a trial y, if any of the following conditions is
-    true:
-    1) Trial x is feasible and trial y is not.
-    2) Trial x and y are both infeasible, but solution x has a smaller overall constraint
-    violation.
-    3) Trial x and y are feasible and trial x dominates trial y.
-    """
-
-    constraints0 = trial0.system_attrs.get(_CONSTRAINTS_KEY)
-    constraints1 = trial1.system_attrs.get(_CONSTRAINTS_KEY)
-
-    if constraints0 is None:
-        warnings.warn(
-            f"Trial {trial0.number} does not have constraint values."
-            " It will be dominated by the other trials."
-        )
-
-    if constraints1 is None:
-        warnings.warn(
-            f"Trial {trial1.number} does not have constraint values."
-            " It will be dominated by the other trials."
-        )
-
-    if constraints0 is None and constraints1 is None:
-        # Neither Trial x nor y has constraints values
-        return _dominates(trial0, trial1, directions)
-
-    if constraints0 is not None and constraints1 is None:
-        # Trial x has constraint values, but y doesn't.
-        return True
-
-    if constraints0 is None and constraints1 is not None:
-        # If Trial y has constraint values, but x doesn't.
-        return False
-
-    assert isinstance(constraints0, (list, tuple))
-    assert isinstance(constraints1, (list, tuple))
-
-    if len(constraints0) != len(constraints1):
-        raise ValueError("Trials with different numbers of constraints cannot be compared.")
-
-    if trial0.state != TrialState.COMPLETE:
-        return False
-
-    if trial1.state != TrialState.COMPLETE:
-        return True
-
-    satisfy_constraints0 = all(v <= 0 for v in constraints0)
-    satisfy_constraints1 = all(v <= 0 for v in constraints1)
-
-    if satisfy_constraints0 and satisfy_constraints1:
-        # Both trials satisfy the constraints.
-        return _dominates(trial0, trial1, directions)
-
-    if satisfy_constraints0:
-        # trial0 satisfies the constraints, but trial1 violates them.
-        return True
-
-    if satisfy_constraints1:
-        # trial1 satisfies the constraints, but trial0 violates them.
-        return False
-
-    # Both trials violate the constraints.
-    violation0 = sum(v for v in constraints0 if v > 0)
-    violation1 = sum(v for v in constraints1 if v > 0)
-    return violation0 < violation1
-
-
-def _fast_non_dominated_sort(
-    population: List[FrozenTrial],
-    directions: List[optuna.study.StudyDirection],
-    constraints_func: Optional[Callable[[FrozenTrial], Sequence[float]]] = None,
-) -> List[List[FrozenTrial]]:
-    if constraints_func is not None:
-        for _trial in population:
-            _constraints = _trial.system_attrs.get(_CONSTRAINTS_KEY)
-            if _constraints is None:
-                continue
-            if np.any(np.isnan(np.array(_constraints))):
-                raise ValueError("NaN is not acceptable as constraint value.")
-
-    dominated_count: DefaultDict[int, int] = defaultdict(int)
-    dominates_list = defaultdict(list)
-
-    dominates = _dominates if constraints_func is None else _constrained_dominates
-
-    for p, q in itertools.combinations(population, 2):
-        if dominates(p, q, directions):
-            dominates_list[p.number].append(q.number)
-            dominated_count[q.number] += 1
-        elif dominates(q, p, directions):
-            dominates_list[q.number].append(p.number)
-            dominated_count[p.number] += 1
-
-    population_per_rank = []
-    while population:
-        non_dominated_population = []
-        i = 0
-        while i < len(population):
-            if dominated_count[population[i].number] == 0:
-                individual = population[i]
-                if i == len(population) - 1:
-                    population.pop()
-                else:
-                    population[i] = population.pop()
-                non_dominated_population.append(individual)
-            else:
-                i += 1
-
-        for x in non_dominated_population:
-            for y in dominates_list[x.number]:
-                dominated_count[y] -= 1
-
-        assert non_dominated_population
-        population_per_rank.append(non_dominated_population)
-
-    return population_per_rank
```

### Comparing `optuna-3.2.0/optuna/search_space/group_decomposed.py` & `optuna-3.3.0/optuna/search_space/group_decomposed.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/search_space/intersection.py` & `optuna-3.3.0/optuna/search_space/intersection.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-from collections import OrderedDict
 import copy
 from typing import Dict
 from typing import Tuple
 
 import optuna
 from optuna.distributions import BaseDistribution
 from optuna.study import Study
@@ -73,29 +72,25 @@
     def __init__(self, include_pruned: bool = False) -> None:
         self._cached_trial_number: int = -1
         self._search_space: Dict[str, BaseDistribution] | None = None
         self._study_id: int | None = None
 
         self._include_pruned = include_pruned
 
-    def calculate(self, study: Study, ordered_dict: bool = False) -> Dict[str, BaseDistribution]:
+    def calculate(self, study: Study) -> Dict[str, BaseDistribution]:
         """Returns the intersection search space of the :class:`~optuna.study.Study`.
 
         Args:
             study:
                 A study with completed trials. The same study must be passed for one instance
                 of this class through its lifetime.
-            ordered_dict:
-                A boolean flag determining the return type.
-                If :obj:`False`, the returned object will be a :obj:`dict`.
-                If :obj:`True`, the returned object will be an :obj:`collections.OrderedDict`
-                sorted by keys, i.e. parameter names.
 
         Returns:
-            A dictionary containing the parameter names and parameter's distributions.
+            A dictionary containing the parameter names and parameter's distributions sorted by
+            parameter names.
         """
 
         if self._study_id is None:
             self._study_id = study._study_id
         else:
             # Note that the check below is meaningless when `InMemoryStorage` is used
             # because `InMemoryStorage.create_new_study` always returns the same study ID.
@@ -105,24 +100,20 @@
         self._search_space, self._cached_trial_number = _calculate(
             study.get_trials(deepcopy=False),
             self._include_pruned,
             self._search_space,
             self._cached_trial_number,
         )
         search_space = self._search_space or {}
-
-        if ordered_dict:
-            search_space = OrderedDict(sorted(search_space.items(), key=lambda x: x[0]))
-
+        search_space = dict(sorted(search_space.items(), key=lambda x: x[0]))
         return copy.deepcopy(search_space)
 
 
 def intersection_search_space(
     trials: list[optuna.trial.FrozenTrial],
-    ordered_dict: bool = False,
     include_pruned: bool = False,
 ) -> Dict[str, BaseDistribution]:
     """Return the intersection search space of the given trials.
 
     Intersection search space contains the intersection of parameter distributions that have been
     suggested in the completed trials of the study so far.
     If there are multiple parameters that have the same name but different distributions,
@@ -133,26 +124,19 @@
         :class:`~optuna.search_space.IntersectionSearchSpace` provides the same functionality with
         a much faster way. Please consider using it if you want to reduce execution time
         as much as possible.
 
     Args:
         trials:
             A list of trials.
-        ordered_dict:
-            A boolean flag determining the return type.
-            If :obj:`False`, the returned object will be a :obj:`dict`.
-            If :obj:`True`, the returned object will be an :obj:`collections.OrderedDict` sorted by
-            keys, i.e. parameter names.
         include_pruned:
             Whether pruned trials should be included in the search space.
 
     Returns:
-        A dictionary containing the parameter names and parameter's distributions.
+        A dictionary containing the parameter names and parameter's distributions sorted by
+        parameter names.
     """
 
     search_space, _ = _calculate(trials, include_pruned)
     search_space = search_space or {}
-
-    if ordered_dict:
-        search_space = OrderedDict(sorted(search_space.items(), key=lambda x: x[0]))
-
+    search_space = dict(sorted(search_space.items(), key=lambda x: x[0]))
     return search_space
```

### Comparing `optuna-3.2.0/optuna/storages/__init__.py` & `optuna-3.3.0/optuna/storages/__init__.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/storages/_base.py` & `optuna-3.3.0/optuna/storages/_base.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/storages/_cached_storage.py` & `optuna-3.3.0/optuna/storages/_cached_storage.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/storages/_heartbeat.py` & `optuna-3.3.0/optuna/storages/_heartbeat.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/storages/_in_memory.py` & `optuna-3.3.0/optuna/storages/_in_memory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import copy
 from datetime import datetime
 import threading
 from typing import Any
 from typing import Container
 from typing import Dict
-from typing import Iterator
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
-from typing import Union
 import uuid
 
 import optuna
 from optuna import distributions  # NOQA
 from optuna._typing import JSONSerializable
 from optuna.exceptions import DuplicatedStudyError
 from optuna.storages import BaseStorage
@@ -358,24 +356,23 @@
         study_id: int,
         deepcopy: bool = True,
         states: Optional[Container[TrialState]] = None,
     ) -> List[FrozenTrial]:
         with self._lock:
             self._check_study_id(study_id)
 
-            trials: Union[List[FrozenTrial], Iterator[FrozenTrial]] = self._studies[
-                study_id
-            ].trials
+            trials = self._studies[study_id].trials
             if states is not None:
-                trials = filter(lambda t: t.state in states, trials)
+                trials = [t for t in trials if t.state in states]
 
             if deepcopy:
-                trials = copy.deepcopy(list(trials))
+                trials = copy.deepcopy(trials)
             else:
-                trials = list(trials)
+                # This copy is required for the replacing trick in `set_trial_xxx`.
+                trials = copy.copy(trials)
 
         return trials
 
     def _check_study_id(self, study_id: int) -> None:
         if study_id not in self._studies:
             raise KeyError("No study with study_id {} exists.".format(study_id))
```

### Comparing `optuna-3.2.0/optuna/storages/_journal/base.py` & `optuna-3.3.0/optuna/storages/_journal/base.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/storages/_journal/file.py` & `optuna-3.3.0/optuna/storages/_journal/file.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/storages/_journal/redis.py` & `optuna-3.3.0/optuna/storages/_journal/redis.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/storages/_journal/storage.py` & `optuna-3.3.0/optuna/storages/_journal/storage.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/storages/_rdb/alembic/env.py` & `optuna-3.3.0/optuna/storages/_rdb/alembic/env.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v0.9.0.a.py` & `optuna-3.3.0/optuna/storages/_rdb/alembic/versions/v0.9.0.a.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v1.2.0.a.py` & `optuna-3.3.0/optuna/storages/_rdb/alembic/versions/v1.2.0.a.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v1.3.0.a.py` & `optuna-3.3.0/optuna/storages/_rdb/alembic/versions/v1.3.0.a.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v2.4.0.a.py` & `optuna-3.3.0/optuna/storages/_rdb/alembic/versions/v2.4.0.a.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v2.6.0.a_.py` & `optuna-3.3.0/optuna/storages/_rdb/alembic/versions/v2.6.0.a_.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v3.0.0.a.py` & `optuna-3.3.0/optuna/storages/_rdb/alembic/versions/v3.0.0.a.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v3.0.0.b.py` & `optuna-3.3.0/optuna/storages/_rdb/alembic/versions/v3.0.0.b.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v3.0.0.c.py` & `optuna-3.3.0/optuna/storages/_rdb/alembic/versions/v3.0.0.c.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v3.0.0.d.py` & `optuna-3.3.0/optuna/storages/_rdb/alembic/versions/v3.0.0.d.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/storages/_rdb/alembic/versions/v3.2.0.a_.py` & `optuna-3.3.0/optuna/storages/_rdb/alembic/versions/v3.2.0.a_.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/storages/_rdb/alembic.ini` & `optuna-3.3.0/optuna/storages/_rdb/alembic.ini`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/storages/_rdb/models.py` & `optuna-3.3.0/optuna/storages/_rdb/models.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/storages/_rdb/storage.py` & `optuna-3.3.0/optuna/storages/_rdb/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from collections import defaultdict
 from contextlib import contextmanager
 import copy
 from datetime import datetime
 import json
 import logging
 import os
@@ -859,30 +861,32 @@
             for value_model in trial.values:
                 values[value_model.objective] = TrialValueModel.stored_repr_to_value(
                     value_model.value, value_model.value_type
                 )
         else:
             values = None
 
+        params = sorted(trial.params, key=lambda p: p.param_id)
+
         return FrozenTrial(
             number=trial.number,
             state=trial.state,
             value=None,
             values=values,
             datetime_start=trial.datetime_start,
             datetime_complete=trial.datetime_complete,
             params={
                 p.param_name: distributions.json_to_distribution(
                     p.distribution_json
                 ).to_external_repr(p.param_value)
-                for p in trial.params
+                for p in params
             },
             distributions={
                 p.param_name: distributions.json_to_distribution(p.distribution_json)
-                for p in trial.params
+                for p in params
             },
             user_attrs={attr.key: json.loads(attr.value_json) for attr in trial.user_attributes},
             system_attrs={
                 attr.key: json.loads(attr.value_json) for attr in trial.system_attributes
             },
             intermediate_values={
                 v.step: models.TrialIntermediateValueModel.stored_repr_to_intermediate_value(
```

### Comparing `optuna-3.2.0/optuna/study/__init__.py` & `optuna-3.3.0/optuna/study/__init__.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/study/_dataframe.py` & `optuna-3.3.0/optuna/study/_dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 __all__ = ["pd"]
 
 
 def _create_records_and_aggregate_column(
     study: "optuna.Study", attrs: Tuple[str, ...]
 ) -> Tuple[List[Dict[Tuple[str, str], Any]], List[Tuple[str, str]]]:
-    attrs_to_df_columns: Dict[str, str] = collections.OrderedDict()
+    attrs_to_df_columns: Dict[str, str] = {}
     for attr in attrs:
         if attr.startswith("_"):
             # Python conventional underscores are omitted in the dataframe.
             df_column = attr[1:]
         else:
             df_column = attr
         attrs_to_df_columns[attr] = df_column
```

### Comparing `optuna-3.2.0/optuna/study/_frozen.py` & `optuna-3.3.0/optuna/study/_frozen.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/study/_multi_objective.py` & `optuna-3.3.0/optuna/study/_multi_objective.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/study/_optimize.py` & `optuna-3.3.0/optuna/study/_optimize.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/study/_study_summary.py` & `optuna-3.3.0/optuna/study/_study_summary.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/study/_tell.py` & `optuna-3.3.0/optuna/study/_tell.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,23 +61,23 @@
 def _check_values_are_feasible(study: "optuna.Study", values: Sequence[float]) -> Optional[str]:
     for v in values:
         # TODO(Imamura): Construct error message taking into account all values and do not early
         # return `value` is assumed to be ignored on failure so we can set it to any value.
         try:
             float(v)
         except (ValueError, TypeError):
-            return f"The value {repr(v)} could not be cast to float."
+            return f"The value {repr(v)} could not be cast to float"
 
         if math.isnan(v):
-            return f"The value {v} is not acceptable."
+            return f"The value {v} is not acceptable"
 
     if len(study.directions) != len(values):
         return (
             f"The number of the values {len(values)} did not match the number of the objectives "
-            f"{len(study.directions)}."
+            f"{len(study.directions)}"
         )
 
     return None
 
 
 def _tell_with_warning(
     study: "optuna.Study",
```

### Comparing `optuna-3.2.0/optuna/study/study.py` & `optuna-3.3.0/optuna/study/study.py`

 * *Files 0% similar despite different names*

```diff
@@ -435,15 +435,14 @@
                 when ``n_trials`` is :obj:`None`, ``timeout`` is not :obj:`None`, and
                 ``n_jobs`` :math:`\\ne 1`.
 
         Raises:
             RuntimeError:
                 If nested invocation of this method occurs.
         """
-
         _optimize(
             study=self,
             func=func,
             n_trials=n_trials,
             timeout=timeout,
             n_jobs=n_jobs,
             catch=tuple(catch) if isinstance(catch, Iterable) else (catch,),
@@ -1003,17 +1002,15 @@
             The names set by this method are used in :meth:`~optuna.study.Study.trials_dataframe`
             and :func:`~optuna.visualization.plot_pareto_front`.
 
         Args:
             metric_names: A list of metric names for the objective function.
         """
         if len(self.directions) != len(metric_names):
-            raise ValueError(
-                "The number of objectives must match thhe length of the metric names."
-            )
+            raise ValueError("The number of objectives must match the length of the metric names.")
 
         self._storage.set_study_system_attr(
             self._study_id, _SYSTEM_ATTR_METRIC_NAMES, metric_names
         )
 
     def _is_multi_objective(self) -> bool:
         """Return :obj:`True` if the study has multiple objectives.
```

### Comparing `optuna-3.2.0/optuna/terminator/__init__.py` & `optuna-3.3.0/optuna/terminator/__init__.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/terminator/callback.py` & `optuna-3.3.0/optuna/terminator/callback.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     so that it can be used with the :func:`~optuna.study.Study.optimize` method.
 
     Args:
         terminator:
             A terminator object which determines whether to terminate the optimization by
             assessing the room for optimization and statistical error. Defaults to a
             :class:`~optuna.terminator.Terminator` object with default
-            improvement_evaluator and error_evaluator.
+            ``improvement_evaluator`` and ``error_evaluator``.
 
     Example:
 
         .. testcode::
 
             from sklearn.datasets import load_wine
             from sklearn.ensemble import RandomForestClassifier
```

### Comparing `optuna-3.2.0/optuna/terminator/erroreval.py` & `optuna-3.3.0/optuna/terminator/erroreval.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         trials: list[FrozenTrial],
         study_direction: StudyDirection,
     ) -> float:
         """Evaluate the statistical error of the objective function based on cross-validation.
 
         Args:
             trials:
-                A list of trials to consider. The best trial in `trials` is used to compute the
+                A list of trials to consider. The best trial in ``trials`` is used to compute the
                 statistical error.
 
             study_direction:
                 The direction of the study.
 
         Returns:
             A float representing the statistical error of the objective function.
```

### Comparing `optuna-3.2.0/optuna/terminator/improvement/_preprocessing.py` & `optuna-3.3.0/optuna/terminator/improvement/_preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,15 +203,15 @@
         self._rng = np.random.RandomState()
 
     def apply(
         self,
         trials: List[optuna.trial.FrozenTrial],
         study_direction: Optional[optuna.study.StudyDirection],
     ) -> List[optuna.trial.FrozenTrial]:
-        search_space = intersection_search_space(trials, ordered_dict=True)
+        search_space = intersection_search_space(trials)
 
         additional_trials = []
         for _ in range(self._n_additional_trials):
             params = {}
             for param_name, distribution in search_space.items():
                 trans = _SearchSpaceTransform({param_name: distribution})
                 trans_params = self._rng.uniform(trans.bounds[:, 0], trans.bounds[:, 1])
```

### Comparing `optuna-3.2.0/optuna/terminator/improvement/evaluator.py` & `optuna-3.3.0/optuna/terminator/improvement/evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         return PreprocessingPipeline(processes)
 
     def evaluate(
         self,
         trials: List[FrozenTrial],
         study_direction: StudyDirection,
     ) -> float:
-        search_space = intersection_search_space(trials, ordered_dict=True)
+        search_space = intersection_search_space(trials)
         self._validate_input(trials, search_space)
 
         fit_trials = self.get_preprocessing().apply(trials, study_direction)
         lcb_trials = self.get_preprocessing(add_random_inputs=True).apply(trials, study_direction)
 
         n_params = len(search_space)
         n_trials = len(fit_trials)
```

### Comparing `optuna-3.2.0/optuna/terminator/improvement/gp/base.py` & `optuna-3.3.0/optuna/terminator/improvement/gp/base.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/terminator/improvement/gp/botorch.py` & `optuna-3.3.0/optuna/terminator/improvement/gp/botorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
     This function assumes the following condition for input trials:
     - any categorical param is converted to a float or int one;
     - log is unscaled for any float/int distribution;
     - the state is COMPLETE for any trial;
     - direction is MINIMIZE for any trial.
     """
-    search_space = intersection_search_space(trials, ordered_dict=True)
+    search_space = intersection_search_space(trials)
     sorted_params = sorted(search_space.keys())
 
     x = []
     for trial in trials:
         assert trial.state == TrialState.COMPLETE
         x_row = []
         for param in sorted_params:
```

### Comparing `optuna-3.2.0/optuna/terminator/terminator.py` & `optuna-3.3.0/optuna/terminator/terminator.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                 study.tell(trial, value)
 
                 if trial.number > min_n_trials and terminator.should_terminate(study):
                     logging.info("Terminated by Optuna Terminator!")
                     break
 
     .. seealso::
-        Please refer to :class:`~optuna.terminator.TerminationCallback` for how to use
+        Please refer to :class:`~optuna.terminator.TerminatorCallback` for how to use
         the terminator mechanism with the :func:`~optuna.study.Study.optimize` method.
 
     """
 
     def __init__(
         self,
         improvement_evaluator: Optional[BaseImprovementEvaluator] = None,
```

### Comparing `optuna-3.2.0/optuna/testing/samplers.py` & `optuna-3.3.0/optuna/testing/samplers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,30 @@
+from __future__ import annotations
+
 from typing import Any
-from typing import Dict
 
 import optuna
 from optuna.distributions import BaseDistribution
 
 
 class DeterministicSampler(optuna.samplers.BaseSampler):
-    def __init__(self, params: Dict[str, Any]) -> None:
+    def __init__(self, params: dict[str, Any]) -> None:
         self.params = params
 
     def infer_relative_search_space(
         self, study: "optuna.study.Study", trial: "optuna.trial.FrozenTrial"
-    ) -> Dict[str, BaseDistribution]:
+    ) -> dict[str, BaseDistribution]:
         return {}
 
     def sample_relative(
         self,
         study: "optuna.study.Study",
         trial: "optuna.trial.FrozenTrial",
-        search_space: Dict[str, BaseDistribution],
-    ) -> Dict[str, Any]:
+        search_space: dict[str, BaseDistribution],
+    ) -> dict[str, Any]:
         return {}
 
     def sample_independent(
         self,
         study: "optuna.study.Study",
         trial: "optuna.trial.FrozenTrial",
         param_name: str,
@@ -35,16 +36,16 @@
 
 
 class FirstTrialOnlyRandomSampler(optuna.samplers.RandomSampler):
     def sample_relative(
         self,
         study: "optuna.study.Study",
         trial: "optuna.trial.FrozenTrial",
-        search_space: Dict[str, BaseDistribution],
-    ) -> Dict[str, float]:
+        search_space: dict[str, BaseDistribution],
+    ) -> dict[str, float]:
         if len(study.trials) > 1:
             raise RuntimeError("`FirstTrialOnlyRandomSampler` only works on the first trial.")
 
         return super(FirstTrialOnlyRandomSampler, self).sample_relative(study, trial, search_space)
 
     def sample_independent(
         self,
```

### Comparing `optuna-3.2.0/optuna/testing/storages.py` & `optuna-3.3.0/optuna/testing/storages.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from __future__ import annotations
 
 import sys
 from types import TracebackType
 from typing import Any
 from typing import IO
-from typing import Optional
-from typing import Type
-from typing import Union
 
 import fakeredis
 import pytest
 
 import optuna
 from optuna.storages import JournalFileStorage
 from optuna.testing.tempfile_pool import NamedTemporaryFilePool
@@ -48,26 +45,26 @@
 SQLITE3_TIMEOUT = 300
 
 
 class StorageSupplier:
     def __init__(self, storage_specifier: str, **kwargs: Any) -> None:
         self.storage_specifier = storage_specifier
         self.extra_args = kwargs
-        self.dask_client: Optional["distributed.Client"] = None
+        self.dask_client: "distributed.Client" | None = None
         self.tempfile: IO[Any] | None = None
 
     def __enter__(
         self,
-    ) -> Union[
-        optuna.storages.InMemoryStorage,
-        optuna.storages._CachedStorage,
-        optuna.storages.RDBStorage,
-        optuna.storages.JournalStorage,
-        "optuna.integration.DaskStorage",
-    ]:
+    ) -> (
+        optuna.storages.InMemoryStorage
+        | optuna.storages._CachedStorage
+        | optuna.storages.RDBStorage
+        | optuna.storages.JournalStorage
+        | "optuna.integration.DaskStorage"
+    ):
         if self.storage_specifier == "inmemory":
             if len(self.extra_args) > 0:
                 raise ValueError("InMemoryStorage does not accept any arguments!")
             return optuna.storages.InMemoryStorage()
         elif "sqlite" in self.storage_specifier:
             self.tempfile = NamedTemporaryFilePool().tempfile()
             url = "sqlite:///{}".format(self.tempfile.name)
@@ -95,15 +92,15 @@
             self.dask_client = distributed.Client()  # type: ignore[no-untyped-call]
 
             return optuna.integration.DaskStorage(client=self.dask_client, **self.extra_args)
         else:
             assert False
 
     def __exit__(
-        self, exc_type: Type[BaseException], exc_val: BaseException, exc_tb: TracebackType
+        self, exc_type: type[BaseException], exc_val: BaseException, exc_tb: TracebackType
     ) -> None:
         if self.tempfile:
             self.tempfile.close()
 
         if self.dask_client:
             self.dask_client.shutdown()  # type: ignore[no-untyped-call]
             self.dask_client.close()  # type: ignore[no-untyped-call]
```

### Comparing `optuna-3.2.0/optuna/testing/tempfile_pool.py` & `optuna-3.3.0/optuna/testing/tempfile_pool.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,20 +6,18 @@
 import atexit
 import gc
 import os
 import tempfile
 from types import TracebackType
 from typing import Any
 from typing import IO
-from typing import List
-from typing import Type
 
 
 class NamedTemporaryFilePool:
-    tempfile_pool: List[IO[Any]] = []
+    tempfile_pool: list[IO[Any]] = []
 
     def __new__(cls, **kwargs: Any) -> "NamedTemporaryFilePool":
         if not hasattr(cls, "_instance"):
             cls._instance = super(NamedTemporaryFilePool, cls).__new__(cls)
             atexit.register(cls._instance.cleanup)
         return cls._instance
 
@@ -37,12 +35,12 @@
             os.unlink(i.name)
 
     def __enter__(self) -> IO[Any]:
         return self.tempfile()
 
     def __exit__(
         self,
-        exc_type: Type[BaseException],
+        exc_type: type[BaseException],
         exc_val: BaseException,
         exc_tb: TracebackType,
     ) -> None:
         self._tempfile.close()
```

### Comparing `optuna-3.2.0/optuna/testing/threading.py` & `optuna-3.3.0/optuna/testing/threading.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
+from __future__ import annotations
+
 import threading
 from typing import Any
 from typing import Callable
-from typing import Optional
-from typing import Tuple
 
 
 class _TestableThread(threading.Thread):
-    def __init__(self, target: Callable[..., Any], args: Tuple):
+    def __init__(self, target: Callable[..., Any], args: tuple):
         threading.Thread.__init__(self, target=target, args=args)
-        self.exc: Optional[BaseException] = None
+        self.exc: BaseException | None = None
 
     def run(self) -> None:
         try:
             threading.Thread.run(self)
         except BaseException as e:
             self.exc = e
 
-    def join(self, timeout: Optional[float] = None) -> None:
+    def join(self, timeout: float | None = None) -> None:
         super(_TestableThread, self).join(timeout)
         if self.exc:
             raise self.exc
```

### Comparing `optuna-3.2.0/optuna/testing/visualization.py` & `optuna-3.3.0/optuna/testing/visualization.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/trial/_base.py` & `optuna-3.3.0/optuna/trial/_base.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/trial/_fixed.py` & `optuna-3.3.0/optuna/trial/_fixed.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/trial/_frozen.py` & `optuna-3.3.0/optuna/trial/_frozen.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/trial/_state.py` & `optuna-3.3.0/optuna/trial/_state.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/trial/_trial.py` & `optuna-3.3.0/optuna/trial/_trial.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,21 +47,21 @@
 
     """
 
     def __init__(self, study: "optuna.study.Study", trial_id: int) -> None:
         self.study = study
         self._trial_id = trial_id
 
-        # TODO(Yanase): Remove _study_id attribute, and use study._study_id instead.
-        self._study_id = self.study._study_id
         self.storage = self.study._storage
 
         self._cached_frozen_trial = self.storage.get_trial(self._trial_id)
         study = pruners._filter_study(self.study, self._cached_frozen_trial)
 
+        self.study.sampler.before_trial(study, self._cached_frozen_trial)
+
         self.relative_search_space = self.study.sampler.infer_relative_search_space(
             study, self._cached_frozen_trial
         )
         self._relative_params: Optional[Dict[str, Any]] = None
         self._fixed_params = self._cached_frozen_trial.system_attrs.get("fixed_params", {})
 
     @property
@@ -683,15 +683,15 @@
                 "uses the values of the first call and ignores all following. "
                 "Using these values: {}".format(name, old_distribution._asdict()),
                 RuntimeWarning,
             )
 
     def _get_latest_trial(self) -> FrozenTrial:
         # TODO(eukaryo): Remove this method after `system_attrs` property is removed.
-        latest_trial = copy.deepcopy(self._cached_frozen_trial)
+        latest_trial = copy.copy(self._cached_frozen_trial)
         latest_trial.system_attrs = _LazyTrialSystemAttrs(  # type: ignore[assignment]
             self._trial_id, self.storage
         )
         return latest_trial
 
     @property
     def params(self) -> Dict[str, Any]:
```

### Comparing `optuna-3.2.0/optuna/visualization/__init__.py` & `optuna-3.3.0/optuna/visualization/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from optuna.visualization import matplotlib
 from optuna.visualization._contour import plot_contour
 from optuna.visualization._edf import plot_edf
+from optuna.visualization._hypervolume_history import plot_hypervolume_history
 from optuna.visualization._intermediate_values import plot_intermediate_values
 from optuna.visualization._optimization_history import plot_optimization_history
 from optuna.visualization._parallel_coordinate import plot_parallel_coordinate
 from optuna.visualization._param_importances import plot_param_importances
 from optuna.visualization._pareto_front import plot_pareto_front
 from optuna.visualization._rank import plot_rank
 from optuna.visualization._slice import plot_slice
@@ -14,14 +15,15 @@
 
 
 __all__ = [
     "is_available",
     "matplotlib",
     "plot_contour",
     "plot_edf",
+    "plot_hypervolume_history",
     "plot_intermediate_values",
     "plot_optimization_history",
     "plot_parallel_coordinate",
     "plot_param_importances",
     "plot_pareto_front",
     "plot_slice",
     "plot_rank",
```

### Comparing `optuna-3.2.0/optuna/visualization/_contour.py` & `optuna-3.3.0/optuna/visualization/_contour.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import math
 from typing import Callable
 from typing import NamedTuple
 
 from optuna.logging import get_logger
 from optuna.study import Study
+from optuna.study import StudyDirection
 from optuna.trial import FrozenTrial
 from optuna.trial import TrialState
 from optuna.visualization._plotly_imports import _imports
 from optuna.visualization._utils import _check_plot_args
 from optuna.visualization._utils import _filter_nonfinite
 from optuna.visualization._utils import _is_log_scale
 from optuna.visualization._utils import _is_numerical
@@ -263,35 +264,36 @@
                 raise ValueError("Parameter {} does not exist in your study.".format(input_p_name))
         sorted_params = sorted(set(params))
 
     sub_plot_infos: list[list[_SubContourInfo]]
     if len(sorted_params) == 2:
         x_param = sorted_params[0]
         y_param = sorted_params[1]
-        sub_plot_info = _get_contour_subplot_info(trials, x_param, y_param, target)
+        sub_plot_info = _get_contour_subplot_info(study, trials, x_param, y_param, target)
         sub_plot_infos = [[sub_plot_info]]
     else:
         sub_plot_infos = []
         for i, y_param in enumerate(sorted_params):
             sub_plot_infos.append([])
             for x_param in sorted_params:
-                sub_plot_info = _get_contour_subplot_info(trials, x_param, y_param, target)
+                sub_plot_info = _get_contour_subplot_info(study, trials, x_param, y_param, target)
                 sub_plot_infos[i].append(sub_plot_info)
 
     reverse_scale = _is_reverse_scale(study, target)
 
     return _ContourInfo(
         sorted_params=sorted_params,
         sub_plot_infos=sub_plot_infos,
         reverse_scale=reverse_scale,
         target_name=target_name,
     )
 
 
 def _get_contour_subplot_info(
+    study: Study,
     trials: list[FrozenTrial],
     x_param: str,
     y_param: str,
     target: Callable[[FrozenTrial], float] | None,
 ) -> _SubContourInfo:
     xaxis = _get_axis_info(trials, x_param)
     yaxis = _get_axis_info(trials, y_param)
@@ -302,15 +304,15 @@
     if len(xaxis.indices) < 2:
         _logger.warning("Param {} unique value length is less than 2.".format(x_param))
         return _SubContourInfo(xaxis=xaxis, yaxis=yaxis, z_values={})
     if len(yaxis.indices) < 2:
         _logger.warning("Param {} unique value length is less than 2.".format(y_param))
         return _SubContourInfo(xaxis=xaxis, yaxis=yaxis, z_values={})
 
-    z_values = {}
+    z_values: dict[tuple[int, int], float] = {}
     for i, trial in enumerate(trials):
         if x_param not in trial.params or y_param not in trial.params:
             continue
         x_value = xaxis.values[i]
         y_value = yaxis.values[i]
         assert x_value is not None
         assert y_value is not None
@@ -319,15 +321,25 @@
 
         if target is None:
             value = trial.value
         else:
             value = target(trial)
         assert value is not None
 
-        z_values[(x_i, y_i)] = value
+        existing = z_values.get((x_i, y_i))
+        if existing is None or target is not None:
+            # When target function is present, we can't be sure what the z-value
+            # represents and therefore we don't know how to select the best one.
+            z_values[(x_i, y_i)] = value
+        else:
+            z_values[(x_i, y_i)] = (
+                min(existing, value)
+                if study.direction is StudyDirection.MINIMIZE
+                else max(existing, value)
+            )
 
     return _SubContourInfo(xaxis=xaxis, yaxis=yaxis, z_values=z_values)
 
 
 def _get_axis_info(trials: list[FrozenTrial], param_name: str) -> _AxisInfo:
     values: list[str | float | None]
     if _is_numerical(trials, param_name):
```

### Comparing `optuna-3.2.0/optuna/visualization/_edf.py` & `optuna-3.3.0/optuna/visualization/_edf.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/visualization/_intermediate_values.py` & `optuna-3.3.0/optuna/visualization/_intermediate_values.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/visualization/_optimization_history.py` & `optuna-3.3.0/optuna/visualization/_slice.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,132 +1,143 @@
 from __future__ import annotations
 
+from typing import Any
 from typing import Callable
 from typing import cast
 from typing import NamedTuple
-from typing import Sequence
-
-import numpy as np
 
+from optuna.distributions import CategoricalChoiceType
+from optuna.distributions import CategoricalDistribution
 from optuna.logging import get_logger
 from optuna.study import Study
-from optuna.study._study_direction import StudyDirection
 from optuna.trial import FrozenTrial
 from optuna.trial import TrialState
 from optuna.visualization._plotly_imports import _imports
 from optuna.visualization._utils import _check_plot_args
+from optuna.visualization._utils import _filter_nonfinite
+from optuna.visualization._utils import _is_log_scale
 
 
 if _imports.is_successful():
     from optuna.visualization._plotly_imports import go
+    from optuna.visualization._plotly_imports import make_subplots
+    from optuna.visualization._plotly_imports import Scatter
+    from optuna.visualization._utils import COLOR_SCALE
 
 _logger = get_logger(__name__)
 
 
-class _ValuesInfo(NamedTuple):
-    values: list[float]
-    stds: list[float] | None
-    label_name: str
+class _SliceSubplotInfo(NamedTuple):
+    param_name: str
+    x: list[Any]
+    y: list[float]
+    trial_numbers: list[int]
+    is_log: bool
+    is_numerical: bool
+    x_labels: tuple[CategoricalChoiceType, ...] | None
+
 
+class _SlicePlotInfo(NamedTuple):
+    target_name: str
+    subplots: list[_SliceSubplotInfo]
 
-class _OptimizationHistoryInfo(NamedTuple):
-    trial_numbers: list[int]
-    values_info: _ValuesInfo
-    best_values_info: _ValuesInfo | None
 
+def _get_slice_subplot_info(
+    trials: list[FrozenTrial],
+    param: str,
+    target: Callable[[FrozenTrial], float] | None,
+    log_scale: bool,
+    numerical: bool,
+    x_labels: tuple[CategoricalChoiceType, ...] | None,
+) -> _SliceSubplotInfo:
+    if target is None:
+
+        def _target(t: FrozenTrial) -> float:
+            return cast(float, t.value)
+
+        target = _target
 
-def _get_optimization_history_info_list(
-    study: Study | Sequence[Study],
+    return _SliceSubplotInfo(
+        param_name=param,
+        x=[t.params[param] for t in trials if param in t.params],
+        y=[target(t) for t in trials if param in t.params],
+        trial_numbers=[t.number for t in trials if param in t.params],
+        is_log=log_scale,
+        is_numerical=numerical,
+        x_labels=x_labels,
+    )
+
+
+def _get_slice_plot_info(
+    study: Study,
+    params: list[str] | None,
     target: Callable[[FrozenTrial], float] | None,
     target_name: str,
-    error_bar: bool,
-) -> list[_OptimizationHistoryInfo]:
+) -> _SlicePlotInfo:
     _check_plot_args(study, target, target_name)
-    if isinstance(study, Study):
-        studies = [study]
-    else:
-        studies = list(study)
 
-    info_list: list[_OptimizationHistoryInfo] = []
-    for study in studies:
-        trials = study.get_trials(states=(TrialState.COMPLETE,))
-        label_name = target_name if len(studies) == 1 else f"{target_name} of {study.study_name}"
-        if target is not None:
-            values = [target(t) for t in trials]
-            # We don't calculate best for user-defined target function since we cannot tell
-            # which direction is better.
-            best_values_info: _ValuesInfo | None = None
-        else:
-            values = [cast(float, t.value) for t in trials]
-            if study.direction == StudyDirection.MINIMIZE:
-                best_values = list(np.minimum.accumulate(values))
-            else:
-                best_values = list(np.maximum.accumulate(values))
-            best_label_name = (
-                "Best Value" if len(studies) == 1 else f"Best Value of {study.study_name}"
-            )
-            best_values_info = _ValuesInfo(best_values, None, best_label_name)
-        info_list.append(
-            _OptimizationHistoryInfo(
-                trial_numbers=[t.number for t in trials],
-                values_info=_ValuesInfo(values, None, label_name),
-                best_values_info=best_values_info,
-            )
-        )
-
-    if len(info_list) == 0:
-        _logger.warning("There are no studies.")
+    trials = _filter_nonfinite(
+        study.get_trials(deepcopy=False, states=(TrialState.COMPLETE,)), target=target
+    )
 
-    if sum(len(info.trial_numbers) for info in info_list) == 0:
-        _logger.warning("There are no complete trials.")
-        info_list.clear()
-
-    if not error_bar:
-        return info_list
-
-    # When error_bar=True, a list of 0 or 1 element is returned.
-    if len(info_list) == 0:
-        return []
-    all_trial_numbers = [number for info in info_list for number in info.trial_numbers]
-    max_num_trial = max(all_trial_numbers) + 1
-
-    def _aggregate(label_name: str, use_best_value: bool) -> tuple[list[int], _ValuesInfo]:
-        # Calculate mean and std of values for each trial number.
-        values: list[list[float]] = [[] for _ in range(max_num_trial)]
-        assert info_list is not None
-        for trial_numbers, values_info, best_values_info in info_list:
-            if use_best_value:
-                assert best_values_info is not None
-                values_info = best_values_info
-            for trial_number, value in zip(trial_numbers, values_info.values):
-                values[trial_number].append(value)
-        trial_numbers_union = [i for i in range(max_num_trial) if len(values[i]) > 0]
-        value_means = [np.mean(v).item() for v in values if len(v) > 0]
-        value_stds = [np.std(v).item() for v in values if len(v) > 0]
-        return trial_numbers_union, _ValuesInfo(value_means, value_stds, label_name)
+    if len(trials) == 0:
+        _logger.warning("Your study does not have any completed trials.")
+        return _SlicePlotInfo(target_name, [])
+
+    all_params = {p_name for t in trials for p_name in t.params.keys()}
+
+    distributions = {}
+    for trial in trials:
+        for param_name, distribution in trial.distributions.items():
+            if param_name not in distributions:
+                distributions[param_name] = distribution
+
+    x_labels = {}
+    for param_name, distribution in distributions.items():
+        if isinstance(distribution, CategoricalDistribution):
+            x_labels[param_name] = distribution.choices
 
-    eb_trial_numbers, eb_values_info = _aggregate(target_name, False)
-    eb_best_values_info: _ValuesInfo | None = None
-    if target is None:
-        _, eb_best_values_info = _aggregate("Best Value", True)
-    return [_OptimizationHistoryInfo(eb_trial_numbers, eb_values_info, eb_best_values_info)]
+    if params is None:
+        sorted_params = sorted(all_params)
+    else:
+        for input_p_name in params:
+            if input_p_name not in all_params:
+                raise ValueError(f"Parameter {input_p_name} does not exist in your study.")
+        sorted_params = sorted(set(params))
+
+    return _SlicePlotInfo(
+        target_name=target_name,
+        subplots=[
+            _get_slice_subplot_info(
+                trials=trials,
+                param=param,
+                target=target,
+                log_scale=_is_log_scale(trials, param),
+                numerical=not isinstance(distributions[param], CategoricalDistribution),
+                x_labels=x_labels.get(param),
+            )
+            for param in sorted_params
+        ],
+    )
 
 
-def plot_optimization_history(
-    study: Study | Sequence[Study],
+def plot_slice(
+    study: Study,
+    params: list[str] | None = None,
     *,
     target: Callable[[FrozenTrial], float] | None = None,
     target_name: str = "Objective Value",
-    error_bar: bool = False,
 ) -> "go.Figure":
-    """Plot optimization history of all trials in a study.
+    """Plot the parameter relationship as slice plot in a study.
+
+    Note that, if a parameter contains missing values, a trial with missing values is not plotted.
 
     Example:
 
-        The following code snippet shows how to plot optimization history.
+        The following code snippet shows how to plot the parameter relationship as slice plot.
 
         .. plotly::
 
             import optuna
 
 
             def objective(trial):
@@ -135,93 +146,97 @@
                 return x ** 2 + y
 
 
             sampler = optuna.samplers.TPESampler(seed=10)
             study = optuna.create_study(sampler=sampler)
             study.optimize(objective, n_trials=10)
 
-            fig = optuna.visualization.plot_optimization_history(study)
+            fig = optuna.visualization.plot_slice(study, params=["x", "y"])
             fig.show()
 
     Args:
         study:
             A :class:`~optuna.study.Study` object whose trials are plotted for their target values.
-            You can pass multiple studies if you want to compare those optimization histories.
+        params:
+            Parameter list to visualize. The default is all parameters.
         target:
             A function to specify the value to display. If it is :obj:`None` and ``study`` is being
             used for single-objective optimization, the objective values are plotted.
 
             .. note::
                 Specify this argument if ``study`` is being used for multi-objective optimization.
         target_name:
-            Target's name to display on the axis label and the legend.
-        error_bar:
-            A flag to show the error bar.
+            Target's name to display on the axis label.
 
     Returns:
         A :class:`plotly.graph_objs.Figure` object.
     """
 
     _imports.check()
+    return _get_slice_plot(_get_slice_plot_info(study, params, target, target_name))
 
-    info_list = _get_optimization_history_info_list(study, target, target_name, error_bar)
-    return _get_optimization_history_plot(info_list, target_name)
-
-
-def _get_optimization_history_plot(
-    info_list: list[_OptimizationHistoryInfo],
-    target_name: str,
-) -> "go.Figure":
-    layout = go.Layout(
-        title="Optimization History Plot",
-        xaxis={"title": "Trial"},
-        yaxis={"title": target_name},
-    )
 
-    traces = []
-    for trial_numbers, values_info, best_values_info in info_list:
-        if values_info.stds is None:
-            error_y = None
-        else:
-            error_y = {"type": "data", "array": values_info.stds, "visible": True}
-        traces.append(
-            go.Scatter(
-                x=trial_numbers,
-                y=values_info.values,
-                error_y=error_y,
-                mode="markers",
-                name=values_info.label_name,
-            )
-        )
+def _get_slice_plot(info: _SlicePlotInfo) -> "go.Figure":
+    layout = go.Layout(title="Slice Plot")
 
-        if best_values_info is not None:
-            traces.append(
-                go.Scatter(
-                    x=trial_numbers,
-                    y=best_values_info.values,
-                    name=best_values_info.label_name,
-                )
+    if len(info.subplots) == 0:
+        return go.Figure(data=[], layout=layout)
+    elif len(info.subplots) == 1:
+        figure = go.Figure(data=[_generate_slice_subplot(info.subplots[0])], layout=layout)
+        figure.update_xaxes(title_text=info.subplots[0].param_name)
+        figure.update_yaxes(title_text=info.target_name)
+        if not info.subplots[0].is_numerical:
+            figure.update_xaxes(
+                type="category", categoryorder="array", categoryarray=info.subplots[0].x_labels
             )
-            if best_values_info.stds is not None:
-                upper = np.array(best_values_info.values) + np.array(best_values_info.stds)
-                traces.append(
-                    go.Scatter(
-                        x=trial_numbers,
-                        y=upper,
-                        mode="lines",
-                        line=dict(width=0.01),
-                        showlegend=False,
-                    )
-                )
-                lower = np.array(best_values_info.values) - np.array(best_values_info.stds)
-                traces.append(
-                    go.Scatter(
-                        x=trial_numbers,
-                        y=lower,
-                        mode="none",
-                        showlegend=False,
-                        fill="tonexty",
-                        fillcolor="rgba(255,0,0,0.2)",
-                    )
+        elif info.subplots[0].is_log:
+            figure.update_xaxes(type="log")
+    else:
+        figure = make_subplots(rows=1, cols=len(info.subplots), shared_yaxes=True)
+        figure.update_layout(layout)
+        showscale = True  # showscale option only needs to be specified once.
+        for column_index, subplot_info in enumerate(info.subplots, start=1):
+            trace = _generate_slice_subplot(subplot_info)
+            trace.update(marker={"showscale": showscale})  # showscale's default is True.
+            if showscale:
+                showscale = False
+            figure.add_trace(trace, row=1, col=column_index)
+            figure.update_xaxes(title_text=subplot_info.param_name, row=1, col=column_index)
+            if column_index == 1:
+                figure.update_yaxes(title_text=info.target_name, row=1, col=column_index)
+            if not subplot_info.is_numerical:
+                figure.update_xaxes(
+                    type="category",
+                    categoryorder="array",
+                    categoryarray=subplot_info.x_labels,
+                    row=1,
+                    col=column_index,
                 )
-
-    return go.Figure(data=traces, layout=layout)
+            elif subplot_info.is_log:
+                figure.update_xaxes(type="log", row=1, col=column_index)
+        if len(info.subplots) > 3:
+            # Ensure that each subplot has a minimum width without relying on autusizing.
+            figure.update_layout(width=300 * len(info.subplots))
+
+    return figure
+
+
+def _generate_slice_subplot(subplot_info: _SliceSubplotInfo) -> "Scatter":
+    x = [x if x is not None else "None" for x in subplot_info.x]
+    y = [y if y is not None else "None" for y in subplot_info.y]
+
+    return go.Scatter(
+        x=x,
+        y=y,
+        mode="markers",
+        marker={
+            "line": {"width": 0.5, "color": "Grey"},
+            "color": subplot_info.trial_numbers,
+            "colorscale": COLOR_SCALE,
+            "colorbar": {
+                "title": "Trial",
+                "x": 1.0,  # Offset the colorbar position with a fixed width `xpad`.
+                "xpad": 40,
+            },
+        },
+        showlegend=False,
+    )
```

### Comparing `optuna-3.2.0/optuna/visualization/_parallel_coordinate.py` & `optuna-3.3.0/optuna/visualization/_parallel_coordinate.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/visualization/_param_importances.py` & `optuna-3.3.0/optuna/visualization/_param_importances.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-from collections import OrderedDict
 from typing import Callable
 from typing import NamedTuple
 
 import optuna
 from optuna.distributions import BaseDistribution
 from optuna.importance._base import BaseImportanceEvaluator
 from optuna.logging import get_logger
@@ -54,15 +53,15 @@
             target_name=target_name,
         )
 
     importances = optuna.importance.get_param_importances(
         study, evaluator=evaluator, params=params, target=target
     )
 
-    importances = OrderedDict(reversed(list(importances.items())))
+    importances = dict(reversed(list(importances.items())))
     importance_values = list(importances.values())
     param_names = list(importances.keys())
     importance_labels = [f"{val:.2f}" if val >= 0.01 else "<0.01" for val in importance_values]
 
     return _ImportancesInfo(
         importance_values=importance_values,
         param_names=param_names,
```

### Comparing `optuna-3.2.0/optuna/visualization/_pareto_front.py` & `optuna-3.3.0/optuna/visualization/_pareto_front.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             )
 
             fig.show()
 
     Args:
         study:
             A :class:`~optuna.study.Study` object whose trials are plotted for their objective
-            values. ``study.n_objectives`` must be either 2 or 3 when ``targets`` is :obj:`None`.
+            values. The number of objectives must be either 2 or 3 when ``targets`` is :obj:`None`.
         target_names:
             Objective name list used as the axis titles. If :obj:`None` is specified,
             "Objective {objective_index}" is used instead. If ``targets`` is specified
             for a study that does not contain any completed trial,
             ``target_name`` must be specified.
         include_dominated_trials:
             A flag to include all dominated trial's objective values.
```

### Comparing `optuna-3.2.0/optuna/visualization/_plotly_imports.py` & `optuna-3.3.0/optuna/visualization/_plotly_imports.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/visualization/_rank.py` & `optuna-3.3.0/optuna/visualization/_rank.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/visualization/_terminator_improvement.py` & `optuna-3.3.0/optuna/visualization/_terminator_improvement.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,18 +39,18 @@
     improvement_evaluator: BaseImprovementEvaluator | None = None,
     error_evaluator: BaseErrorEvaluator | None = None,
     min_n_trials: int = DEFAULT_MIN_N_TRIALS,
 ) -> "go.Figure":
     """Plot the potentials for future objective improvement.
 
     This function visualizes the objective improvement potentials, evaluated
-    with `improvement_evaluator`.
+    with ``improvement_evaluator``.
     It helps to determine whether we should continue the optimization or not.
     You can also plot the error evaluated with
-    `error_evaluator` if the `plot_error` argument is set to :obj:`True`.
+    ``error_evaluator`` if the ``plot_error`` argument is set to :obj:`True`.
     Note that this function may take some time to compute
     the improvement potentials.
 
     Example:
 
         The following code snippet shows how to plot improvement potentials,
         together with cross-validation errors.
@@ -90,15 +90,15 @@
 
     Args:
         study:
             A :class:`~optuna.study.Study` object whose trials are plotted
             for their improvement.
         plot_error:
             A flag to show the error. If it is set to :obj:`True`, errors
-            evaluated by `error_evaluator` are also plotted as line graph.
+            evaluated by ``error_evaluator`` are also plotted as line graph.
             Defaults to :obj:`False`.
         improvement_evaluator:
             An object that evaluates the improvement of the objective function.
             Defaults to :class:`~optuna.terminator.RegretBoundEvaluator`.
         error_evaluator:
             An object that evaluates the error inherent in the objective function.
             Defaults to :class:`~optuna.terminator.CrossValidationErrorEvaluator`.
```

### Comparing `optuna-3.2.0/optuna/visualization/_timeline.py` & `optuna-3.3.0/optuna/visualization/_timeline.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/visualization/_utils.py` & `optuna-3.3.0/optuna/visualization/_utils.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/visualization/matplotlib/__init__.py` & `optuna-3.3.0/optuna/visualization/matplotlib/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from optuna.visualization.matplotlib._contour import plot_contour
 from optuna.visualization.matplotlib._edf import plot_edf
+from optuna.visualization.matplotlib._hypervolume_history import plot_hypervolume_history
 from optuna.visualization.matplotlib._intermediate_values import plot_intermediate_values
 from optuna.visualization.matplotlib._optimization_history import plot_optimization_history
 from optuna.visualization.matplotlib._parallel_coordinate import plot_parallel_coordinate
 from optuna.visualization.matplotlib._param_importances import plot_param_importances
 from optuna.visualization.matplotlib._pareto_front import plot_pareto_front
 from optuna.visualization.matplotlib._rank import plot_rank
 from optuna.visualization.matplotlib._slice import plot_slice
@@ -13,14 +14,15 @@
 
 
 __all__ = [
     "is_available",
     "plot_contour",
     "plot_edf",
     "plot_intermediate_values",
+    "plot_hypervolume_history",
     "plot_optimization_history",
     "plot_parallel_coordinate",
     "plot_param_importances",
     "plot_pareto_front",
     "plot_rank",
     "plot_slice",
     "plot_terminator_improvement",
```

### Comparing `optuna-3.2.0/optuna/visualization/matplotlib/_contour.py` & `optuna-3.3.0/optuna/visualization/matplotlib/_contour.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/visualization/matplotlib/_edf.py` & `optuna-3.3.0/optuna/visualization/matplotlib/_edf.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/visualization/matplotlib/_intermediate_values.py` & `optuna-3.3.0/optuna/visualization/matplotlib/_intermediate_values.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/visualization/matplotlib/_matplotlib_imports.py` & `optuna-3.3.0/optuna/visualization/matplotlib/_matplotlib_imports.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/visualization/matplotlib/_optimization_history.py` & `optuna-3.3.0/optuna/visualization/matplotlib/_param_importances.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,137 +1,135 @@
 from __future__ import annotations
 
 from typing import Callable
-from typing import Sequence
 
 import numpy as np
 
 from optuna._experimental import experimental_func
+from optuna.importance._base import BaseImportanceEvaluator
+from optuna.logging import get_logger
 from optuna.study import Study
 from optuna.trial import FrozenTrial
-from optuna.visualization._optimization_history import _get_optimization_history_info_list
-from optuna.visualization._optimization_history import _OptimizationHistoryInfo
+from optuna.visualization._param_importances import _get_importances_info
+from optuna.visualization._param_importances import _ImportancesInfo
 from optuna.visualization.matplotlib._matplotlib_imports import _imports
 
 
 if _imports.is_successful():
     from optuna.visualization.matplotlib._matplotlib_imports import Axes
     from optuna.visualization.matplotlib._matplotlib_imports import plt
 
 
+_logger = get_logger(__name__)
+
+
+AXES_PADDING_RATIO = 1.05
+
+
 @experimental_func("2.2.0")
-def plot_optimization_history(
-    study: Study | Sequence[Study],
+def plot_param_importances(
+    study: Study,
+    evaluator: BaseImportanceEvaluator | None = None,
+    params: list[str] | None = None,
     *,
     target: Callable[[FrozenTrial], float] | None = None,
     target_name: str = "Objective Value",
-    error_bar: bool = False,
 ) -> "Axes":
-    """Plot optimization history of all trials in a study with Matplotlib.
+    """Plot hyperparameter importances with Matplotlib.
 
     .. seealso::
-        Please refer to :func:`optuna.visualization.plot_optimization_history` for an example.
+        Please refer to :func:`optuna.visualization.plot_param_importances` for an example.
 
     Example:
 
-        The following code snippet shows how to plot optimization history.
+        The following code snippet shows how to plot hyperparameter importances.
 
         .. plot::
 
             import optuna
-            import matplotlib.pyplot as plt
 
 
             def objective(trial):
-                x = trial.suggest_float("x", -100, 100)
-                y = trial.suggest_categorical("y", [-1, 0, 1])
-                return x ** 2 + y
+                x = trial.suggest_int("x", 0, 2)
+                y = trial.suggest_float("y", -1.0, 1.0)
+                z = trial.suggest_float("z", 0.0, 1.5)
+                return x ** 2 + y ** 3 - z ** 4
+
 
-            sampler = optuna.samplers.TPESampler(seed=10)
+            sampler = optuna.samplers.RandomSampler(seed=10)
             study = optuna.create_study(sampler=sampler)
-            study.optimize(objective, n_trials=10)
+            study.optimize(objective, n_trials=100)
 
-            optuna.visualization.matplotlib.plot_optimization_history(study)
-            plt.tight_layout()
+            optuna.visualization.matplotlib.plot_param_importances(study)
 
-        .. note::
-            You need to adjust the size of the plot by yourself using ``plt.tight_layout()`` or
-            ``plt.savefig(IMAGE_NAME, bbox_inches='tight')``.
     Args:
         study:
-            A :class:`~optuna.study.Study` object whose trials are plotted for their target values.
-            You can pass multiple studies if you want to compare those optimization histories.
-
+            An optimized study.
+        evaluator:
+            An importance evaluator object that specifies which algorithm to base the importance
+            assessment on.
+            Defaults to
+            :class:`~optuna.importance.FanovaImportanceEvaluator`.
+        params:
+            A list of names of parameters to assess.
+            If :obj:`None`, all parameters that are present in all of the completed trials are
+            assessed.
         target:
             A function to specify the value to display. If it is :obj:`None` and ``study`` is being
             used for single-objective optimization, the objective values are plotted.
 
             .. note::
-                Specify this argument if ``study`` is being used for multi-objective optimization.
+                Specify this argument if ``study`` is being used for multi-objective
+                optimization. For example, to get the hyperparameter importance of the first
+                objective, use ``target=lambda t: t.values[0]`` for the target parameter.
         target_name:
-            Target's name to display on the axis label and the legend.
-
-        error_bar:
-            A flag to show the error bar.
+            Target's name to display on the axis label.
 
     Returns:
         A :class:`matplotlib.axes.Axes` object.
     """
 
     _imports.check()
 
-    info_list = _get_optimization_history_info_list(study, target, target_name, error_bar)
-    return _get_optimization_history_plot(info_list, target_name)
+    importances_info = _get_importances_info(study, evaluator, params, target, target_name)
+    return _get_importances_plot(importances_info)
 
 
-def _get_optimization_history_plot(
-    info_list: list[_OptimizationHistoryInfo],
-    target_name: str,
-) -> "Axes":
+def _get_importances_plot(info: _ImportancesInfo) -> "Axes":
     # Set up the graph style.
     plt.style.use("ggplot")  # Use ggplot style sheet for similar outputs to plotly.
-    _, ax = plt.subplots()
-    ax.set_title("Optimization History Plot")
-    ax.set_xlabel("Trial")
-    ax.set_ylabel(target_name)
-    cmap = plt.get_cmap("tab10")  # Use tab10 colormap for similar outputs to plotly.
-
-    for i, (trial_numbers, values_info, best_values_info) in enumerate(info_list):
-        if values_info.stds is not None:
-            plt.errorbar(
-                x=trial_numbers,
-                y=values_info.values,
-                yerr=values_info.stds,
-                capsize=5,
-                fmt="o",
-                color="tab:blue",
-            )
-        ax.scatter(
-            x=trial_numbers,
-            y=values_info.values,
-            color=cmap(0) if len(info_list) == 1 else cmap(2 * i),
-            alpha=1,
-            label=values_info.label_name,
-        )
-
-        if best_values_info is not None:
-            ax.plot(
-                trial_numbers,
-                best_values_info.values,
-                marker="o",
-                color=cmap(3) if len(info_list) == 1 else cmap(2 * i + 1),
-                alpha=0.5,
-                label=best_values_info.label_name,
-            )
-            if best_values_info.stds is not None:
-                lower = np.array(best_values_info.values) - np.array(best_values_info.stds)
-                upper = np.array(best_values_info.values) + np.array(best_values_info.stds)
-                ax.fill_between(
-                    x=trial_numbers,
-                    y1=lower,
-                    y2=upper,
-                    color="tab:red",
-                    alpha=0.4,
-                )
-            ax.legend()
-    plt.legend(bbox_to_anchor=(1.05, 1.0), loc="upper left")
+    fig, ax = plt.subplots()
+    ax.set_title("Hyperparameter Importances")
+    ax.set_xlabel(f"Importance for {info.target_name}")
+    ax.set_ylabel("Hyperparameter")
+
+    param_names = info.param_names
+    pos = np.arange(len(param_names))
+    importance_values = info.importance_values
+
+    if len(importance_values) == 0:
+        return ax
+
+    # Draw horizontal bars.
+    ax.barh(
+        pos,
+        importance_values,
+        align="center",
+        color=plt.get_cmap("tab20c")(0),
+        tick_label=param_names,
+    )
+
+    renderer = fig.canvas.get_renderer()
+    for idx, (val, label) in enumerate(zip(importance_values, info.importance_labels)):
+        text = ax.text(val, idx, label, va="center")
+
+        # Sometimes horizontal axis needs to be re-scaled
+        # to avoid text going over plot area.
+        bbox = text.get_window_extent(renderer)
+        bbox = bbox.transformed(ax.transData.inverted())
+        _, plot_xmax = ax.get_xlim()
+        bbox_xmax = bbox.xmax
+
+        if bbox_xmax > plot_xmax:
+            ax.set_xlim(xmax=AXES_PADDING_RATIO * bbox_xmax)
+
     return ax
```

### Comparing `optuna-3.2.0/optuna/visualization/matplotlib/_parallel_coordinate.py` & `optuna-3.3.0/optuna/visualization/matplotlib/_parallel_coordinate.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/visualization/matplotlib/_param_importances.py` & `optuna-3.3.0/optuna/visualization/matplotlib/_rank.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,135 +1,156 @@
 from __future__ import annotations
 
 from typing import Callable
 
-import numpy as np
-
 from optuna._experimental import experimental_func
-from optuna.importance._base import BaseImportanceEvaluator
 from optuna.logging import get_logger
 from optuna.study import Study
 from optuna.trial import FrozenTrial
-from optuna.visualization._param_importances import _get_importances_info
-from optuna.visualization._param_importances import _ImportancesInfo
+from optuna.visualization._rank import _get_rank_info
+from optuna.visualization._rank import _get_tick_info
+from optuna.visualization._rank import _RankPlotInfo
+from optuna.visualization._rank import _RankSubplotInfo
 from optuna.visualization.matplotlib._matplotlib_imports import _imports
 
 
 if _imports.is_successful():
     from optuna.visualization.matplotlib._matplotlib_imports import Axes
+    from optuna.visualization.matplotlib._matplotlib_imports import PathCollection
     from optuna.visualization.matplotlib._matplotlib_imports import plt
 
 
 _logger = get_logger(__name__)
 
 
-AXES_PADDING_RATIO = 1.05
-
-
-@experimental_func("2.2.0")
-def plot_param_importances(
+@experimental_func("3.2.0")
+def plot_rank(
     study: Study,
-    evaluator: BaseImportanceEvaluator | None = None,
     params: list[str] | None = None,
     *,
     target: Callable[[FrozenTrial], float] | None = None,
     target_name: str = "Objective Value",
 ) -> "Axes":
-    """Plot hyperparameter importances with Matplotlib.
+    """Plot parameter relations as scatter plots with colors indicating ranks of target value.
+
+    Note that trials missing the specified parameters will not be plotted.
 
     .. seealso::
-        Please refer to :func:`optuna.visualization.plot_param_importances` for an example.
+        Please refer to :func:`optuna.visualization.plot_rank` for an example.
+
+    Warnings:
+        Output figures of this Matplotlib-based
+        :func:`~optuna.visualization.matplotlib.plot_rank` function would be different from
+        those of the Plotly-based :func:`~optuna.visualization.plot_rank`.
 
     Example:
 
-        The following code snippet shows how to plot hyperparameter importances.
+        The following code snippet shows how to plot the parameter relationship as a rank plot.
 
         .. plot::
 
             import optuna
 
 
             def objective(trial):
-                x = trial.suggest_int("x", 0, 2)
-                y = trial.suggest_float("y", -1.0, 1.0)
-                z = trial.suggest_float("z", 0.0, 1.5)
-                return x ** 2 + y ** 3 - z ** 4
+                x = trial.suggest_float("x", -100, 100)
+                y = trial.suggest_categorical("y", [-1, 0, 1])
+                return x ** 2 + y
 
 
-            sampler = optuna.samplers.RandomSampler(seed=10)
+            sampler = optuna.samplers.TPESampler(seed=10)
             study = optuna.create_study(sampler=sampler)
-            study.optimize(objective, n_trials=100)
+            study.optimize(objective, n_trials=30)
 
-            optuna.visualization.matplotlib.plot_param_importances(study)
+            optuna.visualization.matplotlib.plot_rank(study, params=["x", "y"])
 
     Args:
         study:
-            An optimized study.
-        evaluator:
-            An importance evaluator object that specifies which algorithm to base the importance
-            assessment on.
-            Defaults to
-            :class:`~optuna.importance.FanovaImportanceEvaluator`.
+            A :class:`~optuna.study.Study` object whose trials are plotted for their target values.
         params:
-            A list of names of parameters to assess.
-            If :obj:`None`, all parameters that are present in all of the completed trials are
-            assessed.
+            Parameter list to visualize. The default is all parameters.
         target:
             A function to specify the value to display. If it is :obj:`None` and ``study`` is being
             used for single-objective optimization, the objective values are plotted.
 
             .. note::
-                Specify this argument if ``study`` is being used for multi-objective
-                optimization. For example, to get the hyperparameter importance of the first
-                objective, use ``target=lambda t: t.values[0]`` for the target parameter.
+                Specify this argument if ``study`` is being used for multi-objective optimization.
         target_name:
-            Target's name to display on the axis label.
+            Target's name to display on the color bar.
 
     Returns:
         A :class:`matplotlib.axes.Axes` object.
     """
 
     _imports.check()
+    _logger.warning(
+        "Output figures of this Matplotlib-based `plot_rank` function would be different from "
+        "those of the Plotly-based `plot_rank`."
+    )
+    info = _get_rank_info(study, params, target, target_name)
+    return _get_rank_plot(info)
 
-    importances_info = _get_importances_info(study, evaluator, params, target, target_name)
-    return _get_importances_plot(importances_info)
 
+def _get_rank_plot(
+    info: _RankPlotInfo,
+) -> "Axes":
+    params = info.params
+    sub_plot_infos = info.sub_plot_infos
 
-def _get_importances_plot(info: _ImportancesInfo) -> "Axes":
-    # Set up the graph style.
     plt.style.use("ggplot")  # Use ggplot style sheet for similar outputs to plotly.
-    fig, ax = plt.subplots()
-    ax.set_title("Hyperparameter Importances")
-    ax.set_xlabel(f"Importance for {info.target_name}")
-    ax.set_ylabel("Hyperparameter")
-
-    param_names = info.param_names
-    pos = np.arange(len(param_names))
-    importance_values = info.importance_values
 
-    if len(importance_values) == 0:
-        return ax
+    title = f"Rank ({info.target_name})"
 
-    # Draw horizontal bars.
-    ax.barh(
-        pos,
-        importance_values,
-        align="center",
-        color=plt.get_cmap("tab20c")(0),
-        tick_label=param_names,
-    )
+    n_params = len(params)
+    if n_params == 0:
+        _, ax = plt.subplots()
+        ax.set_title(title)
+        return ax
+    if n_params == 1 or n_params == 2:
+        fig, axs = plt.subplots()
+        axs.set_title(title)
+        pc = _add_rank_subplot(axs, sub_plot_infos[0][0])
+    else:
+        fig, axs = plt.subplots(n_params, n_params)
+        fig.suptitle(title)
+
+        for x_i in range(n_params):
+            for y_i in range(n_params):
+                ax = axs[x_i, y_i]
+                # Set the x or y label only if the subplot is in the edge of the overall figure.
+                pc = _add_rank_subplot(
+                    ax,
+                    sub_plot_infos[x_i][y_i],
+                    set_x_label=x_i == (n_params - 1),
+                    set_y_label=y_i == 0,
+                )
+
+    tick_info = _get_tick_info(info.zs)
+
+    cbar = fig.colorbar(pc, ax=axs, ticks=tick_info.coloridxs, cmap=plt.get_cmap("RdYlBu_r"))
+    cbar.ax.set_yticklabels(tick_info.text)
+    cbar.outline.set_edgecolor("gray")
+    return axs
+
+
+def _add_rank_subplot(
+    ax: "Axes", info: _RankSubplotInfo, set_x_label: bool = True, set_y_label: bool = True
+) -> "PathCollection":
+    if set_x_label:
+        ax.set_xlabel(info.xaxis.name)
+    if set_y_label:
+        ax.set_ylabel(info.yaxis.name)
+
+    if not info.xaxis.is_cat:
+        ax.set_xlim(info.xaxis.range[0], info.xaxis.range[1])
+    if not info.yaxis.is_cat:
+        ax.set_ylim(info.yaxis.range[0], info.yaxis.range[1])
 
-    renderer = fig.canvas.get_renderer()
-    for idx, (val, label) in enumerate(zip(importance_values, info.importance_labels)):
-        text = ax.text(val, idx, label, va="center")
-
-        # Sometimes horizontal axis needs to be re-scaled
-        # to avoid text going over plot area.
-        bbox = text.get_window_extent(renderer)
-        bbox = bbox.transformed(ax.transData.inverted())
-        _, plot_xmax = ax.get_xlim()
-        bbox_xmax = bbox.xmax
+    if info.xaxis.is_log:
+        ax.set_xscale("log")
 
-        if bbox_xmax > plot_xmax:
-            ax.set_xlim(xmax=AXES_PADDING_RATIO * bbox_xmax)
+    if info.yaxis.is_log:
+        ax.set_yscale("log")
 
-    return ax
+    return ax.scatter(
+        x=info.xs, y=info.ys, c=info.color_idxs, cmap=plt.get_cmap("RdYlBu_r"), edgecolors="grey"
+    )
```

### Comparing `optuna-3.2.0/optuna/visualization/matplotlib/_pareto_front.py` & `optuna-3.3.0/optuna/visualization/matplotlib/_pareto_front.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             non-best, and infeasible. Categories are shown in different colors. Here, whether a
             trial is best (on Pareto front) or not is determined ignoring all infeasible trials.
         targets:
             A function that returns a tuple of target values to display.
             The argument to this function is :class:`~optuna.trial.FrozenTrial`.
             ``targets`` must be :obj:`None` or return 2 or 3 values.
             ``axis_order`` and ``targets`` cannot be used at the same time.
-            If ``study.n_objectives`` is neither 2 nor 3, ``targets`` must be specified.
+            If the number of objectives is neither 2 nor 3, ``targets`` must be specified.
 
             .. note::
                 Added in v3.0.0 as an experimental feature. The interface may change in newer
                 versions without prior notice.
                 See https://github.com/optuna/optuna/releases/tag/v3.0.0.
 
     Returns:
```

### Comparing `optuna-3.2.0/optuna/visualization/matplotlib/_rank.py` & `optuna-3.3.0/optuna/visualization/matplotlib/_slice.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,156 +1,178 @@
 from __future__ import annotations
 
+from collections import defaultdict
+import math
+from typing import Any
 from typing import Callable
 
 from optuna._experimental import experimental_func
-from optuna.logging import get_logger
 from optuna.study import Study
 from optuna.trial import FrozenTrial
-from optuna.visualization._rank import _get_rank_info
-from optuna.visualization._rank import _get_tick_info
-from optuna.visualization._rank import _RankPlotInfo
-from optuna.visualization._rank import _RankSubplotInfo
+from optuna.visualization._slice import _get_slice_plot_info
+from optuna.visualization._slice import _SlicePlotInfo
+from optuna.visualization._slice import _SliceSubplotInfo
 from optuna.visualization.matplotlib._matplotlib_imports import _imports
 
 
 if _imports.is_successful():
     from optuna.visualization.matplotlib._matplotlib_imports import Axes
+    from optuna.visualization.matplotlib._matplotlib_imports import Colormap
+    from optuna.visualization.matplotlib._matplotlib_imports import matplotlib
     from optuna.visualization.matplotlib._matplotlib_imports import PathCollection
     from optuna.visualization.matplotlib._matplotlib_imports import plt
 
 
-_logger = get_logger(__name__)
-
-
-@experimental_func("3.2.0")
-def plot_rank(
+@experimental_func("2.2.0")
+def plot_slice(
     study: Study,
     params: list[str] | None = None,
     *,
     target: Callable[[FrozenTrial], float] | None = None,
     target_name: str = "Objective Value",
 ) -> "Axes":
-    """Plot parameter relations as scatter plots with colors indicating ranks of target value.
-
-    Note that trials missing the specified parameters will not be plotted.
+    """Plot the parameter relationship as slice plot in a study with Matplotlib.
 
     .. seealso::
-        Please refer to :func:`optuna.visualization.plot_rank` for an example.
-
-    Warnings:
-        Output figures of this Matplotlib-based
-        :func:`~optuna.visualization.matplotlib.plot_rank` function would be different from
-        those of the Plotly-based :func:`~optuna.visualization.plot_rank`.
+        Please refer to :func:`optuna.visualization.plot_slice` for an example.
 
     Example:
 
-        The following code snippet shows how to plot the parameter relationship as a rank plot.
+        The following code snippet shows how to plot the parameter relationship as slice plot.
 
         .. plot::
 
             import optuna
 
 
             def objective(trial):
                 x = trial.suggest_float("x", -100, 100)
                 y = trial.suggest_categorical("y", [-1, 0, 1])
                 return x ** 2 + y
 
 
             sampler = optuna.samplers.TPESampler(seed=10)
             study = optuna.create_study(sampler=sampler)
-            study.optimize(objective, n_trials=30)
+            study.optimize(objective, n_trials=10)
 
-            optuna.visualization.matplotlib.plot_rank(study, params=["x", "y"])
+            optuna.visualization.matplotlib.plot_slice(study, params=["x", "y"])
 
     Args:
         study:
             A :class:`~optuna.study.Study` object whose trials are plotted for their target values.
         params:
             Parameter list to visualize. The default is all parameters.
         target:
             A function to specify the value to display. If it is :obj:`None` and ``study`` is being
             used for single-objective optimization, the objective values are plotted.
 
             .. note::
                 Specify this argument if ``study`` is being used for multi-objective optimization.
         target_name:
-            Target's name to display on the color bar.
+            Target's name to display on the axis label.
+
 
     Returns:
         A :class:`matplotlib.axes.Axes` object.
     """
 
     _imports.check()
-    _logger.warning(
-        "Output figures of this Matplotlib-based `plot_rank` function would be different from "
-        "those of the Plotly-based `plot_rank`."
-    )
-    info = _get_rank_info(study, params, target, target_name)
-    return _get_rank_plot(info)
+    return _get_slice_plot(_get_slice_plot_info(study, params, target, target_name))
 
 
-def _get_rank_plot(
-    info: _RankPlotInfo,
-) -> "Axes":
-    params = info.params
-    sub_plot_infos = info.sub_plot_infos
+def _get_slice_plot(info: _SlicePlotInfo) -> "Axes":
+    if len(info.subplots) == 0:
+        _, ax = plt.subplots()
+        return ax
 
+    # Set up the graph style.
+    cmap = plt.get_cmap("Blues")
+    padding_ratio = 0.05
     plt.style.use("ggplot")  # Use ggplot style sheet for similar outputs to plotly.
 
-    title = f"Rank ({info.target_name})"
-
-    n_params = len(params)
-    if n_params == 0:
-        _, ax = plt.subplots()
-        ax.set_title(title)
-        return ax
-    if n_params == 1 or n_params == 2:
+    if len(info.subplots) == 1:
+        # Set up the graph style.
         fig, axs = plt.subplots()
-        axs.set_title(title)
-        pc = _add_rank_subplot(axs, sub_plot_infos[0][0])
+        axs.set_title("Slice Plot")
+
+        # Draw a scatter plot.
+        sc = _generate_slice_subplot(info.subplots[0], axs, cmap, padding_ratio, info.target_name)
     else:
-        fig, axs = plt.subplots(n_params, n_params)
-        fig.suptitle(title)
+        # Set up the graph style.
+        min_figwidth = matplotlib.rcParams["figure.figsize"][0] / 2
+        fighight = matplotlib.rcParams["figure.figsize"][1]
+        # Ensure that each subplot has a minimum width without relying on auto-sizing.
+        fig, axs = plt.subplots(
+            1,
+            len(info.subplots),
+            sharey=True,
+            figsize=(min_figwidth * len(info.subplots), fighight),
+        )
+        fig.suptitle("Slice Plot")
+
+        # Draw scatter plots.
+        for i, subplot in enumerate(info.subplots):
+            ax = axs[i]
+            sc = _generate_slice_subplot(subplot, ax, cmap, padding_ratio, info.target_name)
+
+    axcb = fig.colorbar(sc, ax=axs)
+    axcb.set_label("Trial")
 
-        for x_i in range(n_params):
-            for y_i in range(n_params):
-                ax = axs[x_i, y_i]
-                # Set the x or y label only if the subplot is in the edge of the overall figure.
-                pc = _add_rank_subplot(
-                    ax,
-                    sub_plot_infos[x_i][y_i],
-                    set_x_label=x_i == (n_params - 1),
-                    set_y_label=y_i == 0,
-                )
-
-    tick_info = _get_tick_info(info.zs)
-
-    cbar = fig.colorbar(pc, ax=axs, ticks=tick_info.coloridxs, cmap=plt.get_cmap("RdYlBu_r"))
-    cbar.ax.set_yticklabels(tick_info.text)
-    cbar.outline.set_edgecolor("gray")
     return axs
 
 
-def _add_rank_subplot(
-    ax: "Axes", info: _RankSubplotInfo, set_x_label: bool = True, set_y_label: bool = True
+def _generate_slice_subplot(
+    subplot_info: _SliceSubplotInfo,
+    ax: "Axes",
+    cmap: "Colormap",
+    padding_ratio: float,
+    target_name: str,
 ) -> "PathCollection":
-    if set_x_label:
-        ax.set_xlabel(info.xaxis.name)
-    if set_y_label:
-        ax.set_ylabel(info.yaxis.name)
-
-    if not info.xaxis.is_cat:
-        ax.set_xlim(info.xaxis.range[0], info.xaxis.range[1])
-    if not info.yaxis.is_cat:
-        ax.set_ylim(info.yaxis.range[0], info.yaxis.range[1])
-
-    if info.xaxis.is_log:
+    ax.set(xlabel=subplot_info.param_name, ylabel=target_name)
+    scale = None
+    if subplot_info.is_log:
         ax.set_xscale("log")
-
-    if info.yaxis.is_log:
-        ax.set_yscale("log")
-
-    return ax.scatter(
-        x=info.xs, y=info.ys, c=info.color_idxs, cmap=plt.get_cmap("RdYlBu_r"), edgecolors="grey"
-    )
+        scale = "log"
+    if subplot_info.is_numerical:
+        x_values = subplot_info.x
+        y_values = subplot_info.y
+        c_values = subplot_info.trial_numbers
+    else:
+        x_values = []
+        y_values = []
+        c_values = []
+        assert subplot_info.x_labels is not None
+        points_dict = defaultdict(list)
+        for x, y, number in zip(subplot_info.x, subplot_info.y, subplot_info.trial_numbers):
+            points_dict[x].append((y, number))
+        for x_label in subplot_info.x_labels:
+            for y, number in points_dict[x_label]:
+                x_values.append(str(x_label))
+                y_values.append(y)
+                c_values.append(number)
+        scale = "categorical"
+    xlim = _calc_lim_with_padding(x_values, padding_ratio, scale)
+    ax.set_xlim(xlim[0], xlim[1])
+    sc = ax.scatter(x_values, y_values, c=c_values, cmap=cmap, edgecolors="grey")
+    ax.label_outer()
+
+    return sc
+
+
+def _calc_lim_with_padding(
+    values: list[Any], padding_ratio: float, scale: str | None
+) -> tuple[float, float]:
+    value_max = max(values)
+    value_min = min(values)
+    if scale == "log":
+        padding = (math.log10(value_max) - math.log10(value_min)) * padding_ratio
+        return (
+            math.pow(10, math.log10(value_min) - padding),
+            math.pow(10, math.log10(value_max) + padding),
+        )
+    elif scale == "categorical":
+        width = len(set(values)) - 1
+        padding = width * padding_ratio
+        return -padding, width + padding
+    else:
+        padding = (value_max - value_min) * padding_ratio
+        return value_min - padding, value_max + padding
```

### Comparing `optuna-3.2.0/optuna/visualization/matplotlib/_terminator_improvement.py` & `optuna-3.3.0/optuna/visualization/matplotlib/_terminator_improvement.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,18 +30,18 @@
     improvement_evaluator: BaseImprovementEvaluator | None = None,
     error_evaluator: BaseErrorEvaluator | None = None,
     min_n_trials: int = DEFAULT_MIN_N_TRIALS,
 ) -> "Axes":
     """Plot the potentials for future objective improvement.
 
     This function visualizes the objective improvement potentials, evaluated
-    with `improvement_evaluator`.
+    with ``improvement_evaluator``.
     It helps to determine whether we should continue the optimization or not.
     You can also plot the error evaluated with
-    `error_evaluator` if the `plot_error` argument is set to :obj:`True`.
+    ``error_evaluator`` if the ``plot_error`` argument is set to :obj:`True`.
     Note that this function may take some time to compute
     the improvement potentials.
 
     .. seealso::
         Please refer to :func:`optuna.visualization.plot_terminator_improvement`.
 
     Example:
@@ -79,15 +79,15 @@
             plot_terminator_improvement(study, plot_error=True)
 
     Args:
         study:
             A :class:`~optuna.study.Study` object whose trials are plotted for their improvement.
         plot_error:
             A flag to show the error. If it is set to :obj:`True`, errors
-            evaluated by `error_evaluator` are also plotted as line graph.
+            evaluated by ``error_evaluator`` are also plotted as line graph.
             Defaults to :obj:`False`.
         improvement_evaluator:
             An object that evaluates the improvement of the objective function.
             Default to :class:`~optuna.terminator.RegretBoundEvaluator`.
         error_evaluator:
             An object that evaluates the error inherent in the objective function.
             Default to :class:`~optuna.terminator.CrossValidationErrorEvaluator`.
```

### Comparing `optuna-3.2.0/optuna/visualization/matplotlib/_timeline.py` & `optuna-3.3.0/optuna/visualization/matplotlib/_timeline.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna/visualization/matplotlib/_utils.py` & `optuna-3.3.0/optuna/visualization/matplotlib/_utils.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/optuna.egg-info/PKG-INFO` & `optuna-3.3.0/optuna.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optuna
-Version: 3.2.0
+Version: 3.3.0
 Summary: A hyperparameter optimization framework
 Author: Takuya Akiba
 Author-email: akiba@preferred.jp
 License: MIT License
         
         Copyright (c) 2018 Preferred Networks, Inc.
```

### Comparing `optuna-3.2.0/optuna.egg-info/SOURCES.txt` & `optuna-3.3.0/optuna.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,20 @@
 optuna.egg-info/requires.txt
 optuna.egg-info/top_level.txt
 optuna/_hypervolume/__init__.py
 optuna/_hypervolume/base.py
 optuna/_hypervolume/hssp.py
 optuna/_hypervolume/utils.py
 optuna/_hypervolume/wfg.py
+optuna/artifacts/__init__.py
+optuna/artifacts/_boto3.py
+optuna/artifacts/_filesystem.py
+optuna/artifacts/_protocol.py
+optuna/artifacts/_upload.py
+optuna/artifacts/exceptions.py
 optuna/importance/__init__.py
 optuna/importance/_base.py
 optuna/importance/_mean_decrease_impurity.py
 optuna/importance/_fanova/__init__.py
 optuna/importance/_fanova/_evaluator.py
 optuna/importance/_fanova/_fanova.py
 optuna/importance/_fanova/_tree.py
@@ -102,15 +108,19 @@
 optuna/samplers/_tpe/_erf.py
 optuna/samplers/_tpe/_truncnorm.py
 optuna/samplers/_tpe/multi_objective_sampler.py
 optuna/samplers/_tpe/parzen_estimator.py
 optuna/samplers/_tpe/probability_distributions.py
 optuna/samplers/_tpe/sampler.py
 optuna/samplers/nsgaii/__init__.py
+optuna/samplers/nsgaii/_after_trial_strategy.py
+optuna/samplers/nsgaii/_child_generation_strategy.py
 optuna/samplers/nsgaii/_crossover.py
+optuna/samplers/nsgaii/_dominates.py
+optuna/samplers/nsgaii/_elite_population_selection_strategy.py
 optuna/samplers/nsgaii/_sampler.py
 optuna/samplers/nsgaii/_crossovers/__init__.py
 optuna/samplers/nsgaii/_crossovers/_base.py
 optuna/samplers/nsgaii/_crossovers/_blxalpha.py
 optuna/samplers/nsgaii/_crossovers/_sbx.py
 optuna/samplers/nsgaii/_crossovers/_spx.py
 optuna/samplers/nsgaii/_crossovers/_undx.py
@@ -178,28 +188,30 @@
 optuna/trial/_fixed.py
 optuna/trial/_frozen.py
 optuna/trial/_state.py
 optuna/trial/_trial.py
 optuna/visualization/__init__.py
 optuna/visualization/_contour.py
 optuna/visualization/_edf.py
+optuna/visualization/_hypervolume_history.py
 optuna/visualization/_intermediate_values.py
 optuna/visualization/_optimization_history.py
 optuna/visualization/_parallel_coordinate.py
 optuna/visualization/_param_importances.py
 optuna/visualization/_pareto_front.py
 optuna/visualization/_plotly_imports.py
 optuna/visualization/_rank.py
 optuna/visualization/_slice.py
 optuna/visualization/_terminator_improvement.py
 optuna/visualization/_timeline.py
 optuna/visualization/_utils.py
 optuna/visualization/matplotlib/__init__.py
 optuna/visualization/matplotlib/_contour.py
 optuna/visualization/matplotlib/_edf.py
+optuna/visualization/matplotlib/_hypervolume_history.py
 optuna/visualization/matplotlib/_intermediate_values.py
 optuna/visualization/matplotlib/_matplotlib_imports.py
 optuna/visualization/matplotlib/_optimization_history.py
 optuna/visualization/matplotlib/_parallel_coordinate.py
 optuna/visualization/matplotlib/_param_importances.py
 optuna/visualization/matplotlib/_pareto_front.py
 optuna/visualization/matplotlib/_rank.py
```

### Comparing `optuna-3.2.0/optuna.egg-info/requires.txt` & `optuna-3.3.0/optuna.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 alembic>=1.5.0
-cmaes>=0.9.1
+cmaes>=0.10.0
 colorlog
 numpy
 packaging>=20.0
 sqlalchemy>=1.3.0
 tqdm
 PyYAML
 
@@ -16,14 +16,15 @@
 
 [checking]
 black
 blackdoc
 flake8
 isort
 mypy
+mypy_boto3_s3
 types-PyYAML
 types-redis
 types-setuptools
 types-tqdm
 typing_extensions>=3.10.0.0
 
 [document]
@@ -39,57 +40,56 @@
 plotly>=4.9.0
 scikit-learn
 scikit-optimize
 sphinx
 sphinx-copybutton
 sphinx-gallery
 sphinx-plotly-directive
-sphinx_rtd_theme
+sphinx_rtd_theme>=1.2.0
 torch
 torchaudio
 torchvision
 
 [integration]
+botorch>=0.4.0
 cma
 distributed
-mlflow
-pandas
-scikit-learn>=0.24.2
-wandb
-xgboost
-
-[integration:python_version < "3.11"]
-botorch>=0.4.0
 fastai
 lightgbm
-mxnet
+mlflow
+pandas
 pytorch-ignite
 pytorch-lightning>=1.6.0
+scikit-learn>=0.24.2
 scikit-optimize
 shap
 tensorflow
 torch
 torchaudio
 torchvision
+wandb
+xgboost
 
 [integration:sys_platform != "darwin"]
 catboost>=0.26
 
 [integration:sys_platform == "darwin"]
 catboost<1.2,>=0.26
 
 [optional]
+boto3
 botorch
 matplotlib!=3.6.0
 pandas
 plotly>=4.9.0
 redis
 scikit-learn>=0.24.2
 
 [test]
 coverage
 fakeredis[lua]
 kaleido
+moto
 pytest
 
 [test:python_version >= "3.8"]
 scipy>=1.9.2
```

### Comparing `optuna-3.2.0/pyproject.toml` & `optuna-3.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 requires-python = ">=3.7"
 dependencies = [
   "alembic>=1.5.0",
-  "cmaes>=0.9.1",
+  "cmaes>=0.10.0",
   "colorlog",
   "numpy",
   "packaging>=20.0",
   "sqlalchemy>=1.3.0",
   "tqdm",
   "PyYAML",  # Only used in `optuna/cli.py`.
 ]
@@ -53,14 +53,15 @@
 ]
 checking = [
     "black",
     "blackdoc",
     "flake8",
     "isort",
     "mypy",
+    "mypy_boto3_s3",
     "types-PyYAML",
     "types-redis",
     "types-setuptools",
     "types-tqdm",
     "typing_extensions>=3.10.0.0",
 ]
 document = [
@@ -76,55 +77,56 @@
     "plotly>=4.9.0",  # optuna/visualization.
     "scikit-learn",
     "scikit-optimize",
     "sphinx",
     "sphinx-copybutton",
     "sphinx-gallery",
     "sphinx-plotly-directive",
-    "sphinx_rtd_theme",
+    "sphinx_rtd_theme>=1.2.0",
     "torch",
     "torchaudio",
     "torchvision",
 ]
 integration = [
-    "botorch>=0.4.0; python_version<'3.11'",
+    "botorch>=0.4.0",
     "catboost>=0.26; sys_platform!='darwin'",
     "catboost>=0.26,<1.2; sys_platform=='darwin'",
     "cma",
     "distributed",
-    "fastai; python_version<'3.11'",
-    "lightgbm; python_version<'3.11'",
+    "fastai",
+    "lightgbm",
     "mlflow",
-    "mxnet; python_version<'3.11'",
     "pandas",
-    "pytorch-ignite; python_version<'3.11'",
-    "pytorch-lightning>=1.6.0; python_version<'3.11'",
+    "pytorch-ignite",
+    "pytorch-lightning>=1.6.0",
     "scikit-learn>=0.24.2",
-    "scikit-optimize; python_version<'3.11'",
-    "shap; python_version<'3.11'",
-    "tensorflow; python_version<'3.11'",
-    "torch; python_version<'3.11'",
-    "torchaudio; python_version<'3.11'",
-    "torchvision; python_version<'3.11'",
+    "scikit-optimize",
+    "shap",
+    "tensorflow",
+    "torch",
+    "torchaudio",
+    "torchvision",
     "wandb",
     "xgboost",
 ]
 optional = [
-    "botorch",  # optuna/terminator/gp/botorch
-    "matplotlib!=3.6.0",  # optuna/visualization/matplotlib
-    "pandas",  # optuna/study.py
+    "boto3",  # optuna/artifacts/_boto3.py.
+    "botorch",  # optuna/terminator/gp/botorch.
+    "matplotlib!=3.6.0",  # optuna/visualization/matplotlib.
+    "pandas",  # optuna/study.py.
     "plotly>=4.9.0",  # optuna/visualization.
     "redis",  # optuna/storages/redis.py.
     "scikit-learn>=0.24.2",
     # optuna/visualization/param_importances.py.
 ]
 test = [
     "coverage",
     "fakeredis[lua]",
     "kaleido",
+    "moto",
     "pytest",
     "scipy>=1.9.2; python_version>='3.8'",
 ]
 
 [project.urls]
 homepage = "https://optuna.org/"
 repository = "https://github.com/optuna/optuna"
```

### Comparing `optuna-3.2.0/setup.cfg` & `optuna-3.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/tests/test_callbacks.py` & `optuna-3.3.0/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/tests/test_cli.py` & `optuna-3.3.0/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,35 @@
-from collections import OrderedDict
 import json
 import os
+import platform
 import re
 import subprocess
 from subprocess import CalledProcessError
+import tempfile
 from typing import Any
 from typing import Callable
 from typing import Optional
 from typing import Tuple
+from unittest.mock import MagicMock
 from unittest.mock import patch
 
+import fakeredis
 import numpy as np
 from pandas import Timedelta
 from pandas import Timestamp
 import pytest
 import yaml
 
 import optuna
 import optuna.cli
 from optuna.exceptions import CLIUsageError
 from optuna.exceptions import ExperimentalWarning
+from optuna.storages import JournalFileStorage
+from optuna.storages import JournalRedisStorage
+from optuna.storages import JournalStorage
 from optuna.storages import RDBStorage
 from optuna.storages._base import DEFAULT_STUDY_NAME_PREFIX
 from optuna.study import StudyDirection
 from optuna.testing.storages import StorageSupplier
 from optuna.testing.tempfile_pool import NamedTemporaryFilePool
 from optuna.trial import Trial
 from optuna.trial import TrialState
@@ -71,15 +77,15 @@
         assert all(len(rows[0]) == len(row) for row in rows)
         # Check ruled lines.
         assert rows[0] == rows[2] == rows[-1]
 
         keys = [r.strip() for r in rows[1].split("|")[1:-1]]
         ret = []
         for record in rows[3:-1]:
-            attrs = OrderedDict()
+            attrs = {}
             for key, attr in zip(keys, record.split("|")[1:-1]):
                 attrs[key] = attr.strip()
             ret.append(attrs)
         return ret
     elif output_format == "json":
         return json.loads(output)
     elif output_format == "yaml":
@@ -1045,14 +1051,59 @@
         with patch.dict("optuna.cli.os.environ", {"OPTUNA_STORAGE": "sqlite:///args.db"}):
             optuna.cli._check_storage_url(None)
 
     with pytest.raises(CLIUsageError):
         optuna.cli._check_storage_url(None)
 
 
+@pytest.mark.skipif(platform.system() == "Windows", reason="Skip on Windows")
+@patch("optuna.storages._journal.redis.redis")
+def test_get_storage_without_storage_class(mock_redis: MagicMock) -> None:
+    with tempfile.NamedTemporaryFile(suffix=".db") as fp:
+        storage = optuna.cli._get_storage(f"sqlite:///{fp.name}", storage_class=None)
+        assert isinstance(storage, RDBStorage)
+
+    with tempfile.NamedTemporaryFile(suffix=".log") as fp:
+        storage = optuna.cli._get_storage(fp.name, storage_class=None)
+        assert isinstance(storage, JournalStorage)
+        assert isinstance(storage._backend, JournalFileStorage)
+
+    mock_redis.Redis = fakeredis.FakeRedis
+    storage = optuna.cli._get_storage("redis://localhost:6379", storage_class=None)
+    assert isinstance(storage, JournalStorage)
+    assert isinstance(storage._backend, JournalRedisStorage)
+
+    with pytest.raises(CLIUsageError):
+        optuna.cli._get_storage("./file-not-found.log", storage_class=None)
+
+
+@pytest.mark.skipif(platform.system() == "Windows", reason="Skip on Windows")
+@patch("optuna.storages._journal.redis.redis")
+def test_get_storage_with_storage_class(mock_redis: MagicMock) -> None:
+    with tempfile.NamedTemporaryFile(suffix=".db") as fp:
+        storage = optuna.cli._get_storage(f"sqlite:///{fp.name}", storage_class=None)
+        assert isinstance(storage, RDBStorage)
+
+    with tempfile.NamedTemporaryFile(suffix=".log") as fp:
+        storage = optuna.cli._get_storage(fp.name, storage_class="JournalFileStorage")
+        assert isinstance(storage, JournalStorage)
+        assert isinstance(storage._backend, JournalFileStorage)
+
+    mock_redis.Redis = fakeredis.FakeRedis
+    storage = optuna.cli._get_storage(
+        "redis:///localhost:6379", storage_class="JournalRedisStorage"
+    )
+    assert isinstance(storage, JournalStorage)
+    assert isinstance(storage._backend, JournalRedisStorage)
+
+    with pytest.raises(CLIUsageError):
+        with tempfile.NamedTemporaryFile(suffix=".db") as fp:
+            optuna.cli._get_storage(f"sqlite:///{fp.name}", storage_class="InMemoryStorage")
+
+
 @pytest.mark.skip_coverage
 def test_storage_upgrade_command() -> None:
     with StorageSupplier("sqlite") as storage:
         assert isinstance(storage, RDBStorage)
         storage_url = str(storage.engine.url)
 
         command = ["optuna", "storage", "upgrade"]
@@ -1063,14 +1114,24 @@
             )
 
         command.extend(["--storage", storage_url])
         subprocess.check_call(command)
 
 
 @pytest.mark.skip_coverage
+def test_storage_upgrade_command_with_invalid_url() -> None:
+    with StorageSupplier("sqlite") as storage:
+        assert isinstance(storage, RDBStorage)
+
+        command = ["optuna", "storage", "upgrade", "--storage", "invalid-storage-url"]
+        with pytest.raises(CalledProcessError):
+            subprocess.check_call(command)
+
+
+@pytest.mark.skip_coverage
 @pytest.mark.parametrize(
     "direction,directions,sampler,sampler_kwargs,output_format",
     [
         (None, None, None, None, None),
         ("minimize", None, None, None, None),
         (None, "minimize maximize", None, None, None),
         (None, None, "RandomSampler", None, None),
```

### Comparing `optuna-3.2.0/tests/test_convert_positional_args.py` & `optuna-3.3.0/tests/test_convert_positional_args.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/tests/test_deprecated.py` & `optuna-3.3.0/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/tests/test_distributions.py` & `optuna-3.3.0/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/tests/test_experimental.py` & `optuna-3.3.0/tests/test_experimental.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/tests/test_imports.py` & `optuna-3.3.0/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/tests/test_logging.py` & `optuna-3.3.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/tests/test_multi_objective.py` & `optuna-3.3.0/tests/test_multi_objective.py`

 * *Files identical despite different names*

### Comparing `optuna-3.2.0/tests/test_transform.py` & `optuna-3.3.0/tests/test_transform.py`

 * *Files identical despite different names*

