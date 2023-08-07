# Comparing `tmp/smltheory-0.1.4.tar.gz` & `tmp/smltheory-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smltheory-0.1.4.tar", max compression
+gzip compressed data, was "smltheory-0.1.5.tar", max compression
```

## Comparing `smltheory-0.1.4.tar` & `smltheory-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,21 @@
--rwxr-xr-x   0        0        0     1076 2023-08-01 20:38:18.331005 smltheory-0.1.4/LICENSE
--rw-r--r--   0        0        0      926 2023-08-02 15:34:34.623560 smltheory-0.1.4/README.md
--rw-r--r--   0        0        0      593 2023-08-04 22:39:19.169699 smltheory-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      410 2023-08-04 22:38:07.742434 smltheory-0.1.4/src/smltheory/__init__.py
--rw-r--r--   0        0        0     5122 2023-08-04 17:25:51.083724 smltheory-0.1.4/src/smltheory/bayes_decision.py
--rw-r--r--   0        0        0     4012 2023-08-03 14:23:13.848664 smltheory-0.1.4/src/smltheory/est_error.py
--rw-r--r--   0        0        0    12719 2023-08-03 20:10:07.529472 smltheory-0.1.4/src/smltheory/generate_data.py
--rw-r--r--   0        0        0     9449 2023-08-04 14:15:40.598616 smltheory-0.1.4/src/smltheory/gradient_descent.py
--rw-r--r--   0        0        0     9377 2023-08-04 16:14:40.063052 smltheory-0.1.4/src/smltheory/least_squares.py
--rw-r--r--   0        0        0    11041 2023-08-04 17:10:38.427385 smltheory-0.1.4/src/smltheory/opt_error.py
--rw-r--r--   0        0        0     7590 2023-08-04 17:04:40.592233 smltheory-0.1.4/src/smltheory/overfitting.py
--rw-r--r--   0        0        0    15886 2023-08-04 17:06:08.189243 smltheory-0.1.4/src/smltheory/trun_mvnt.py
--rw-r--r--   0        0        0     1518 1970-01-01 00:00:00.000000 smltheory-0.1.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1076 2023-08-01 20:38:18.331005 smltheory-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1041 2023-08-06 16:05:12.742227 smltheory-0.1.5/README.md
+-rw-r--r--   0        0        0      593 2023-08-07 21:21:59.684225 smltheory-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      444 2023-08-06 01:37:23.815152 smltheory-0.1.5/src/smltheory/__init__.py
+-rw-r--r--   0        0        0     6199 2023-08-06 01:58:07.279270 smltheory-0.1.5/src/smltheory/bayes_decision.py
+-rw-r--r--   0        0        0        0 2023-08-05 02:48:00.360490 smltheory-0.1.5/src/smltheory/data/__init__.py
+-rw-r--r--   0        0        0   589785 2023-08-05 03:48:26.746468 smltheory-0.1.5/src/smltheory/data/data_best_in_class.csv
+-rw-r--r--   0        0        0  5998151 2023-07-27 15:14:55.256898 smltheory-0.1.5/src/smltheory/data/data_bv_tradeoff.csv
+-rw-r--r--   0        0        0     8630 2023-08-05 03:18:12.360165 smltheory-0.1.5/src/smltheory/data/data_emp_loss.csv
+-rw-r--r--   0        0        0    23457 2023-07-16 02:37:58.154443 smltheory-0.1.5/src/smltheory/data/data_est_error.csv
+-rw-r--r--   0        0        0     8630 2023-08-05 03:18:38.737708 smltheory-0.1.5/src/smltheory/data/data_gen_error.csv
+-rw-r--r--   0        0        0    23158 2023-08-05 22:49:49.318878 smltheory-0.1.5/src/smltheory/data/data_opt_error_fast.csv
+-rw-r--r--   0        0        0     8557 2023-08-06 01:52:33.818341 smltheory-0.1.5/src/smltheory/datasets.py
+-rw-r--r--   0        0        0     3971 2023-08-06 01:52:33.804070 smltheory-0.1.5/src/smltheory/est_error.py
+-rw-r--r--   0        0        0    15895 2023-08-06 02:21:14.762431 smltheory-0.1.5/src/smltheory/generate_data.py
+-rw-r--r--   0        0        0     9449 2023-08-04 14:15:40.598616 smltheory-0.1.5/src/smltheory/gradient_descent.py
+-rw-r--r--   0        0        0     9377 2023-08-04 16:14:40.063052 smltheory-0.1.5/src/smltheory/least_squares.py
+-rw-r--r--   0        0        0    11006 2023-08-06 02:27:17.083759 smltheory-0.1.5/src/smltheory/opt_error.py
+-rw-r--r--   0        0        0     7610 2023-08-07 21:13:01.889018 smltheory-0.1.5/src/smltheory/overfitting.py
+-rw-r--r--   0        0        0    15886 2023-08-04 17:06:08.189243 smltheory-0.1.5/src/smltheory/trun_mvnt.py
+-rw-r--r--   0        0        0     1633 1970-01-01 00:00:00.000000 smltheory-0.1.5/PKG-INFO
```

### Comparing `smltheory-0.1.4/LICENSE` & `smltheory-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.4/README.md` & `smltheory-0.1.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,26 @@
-# sml_theory
+# smltheory
 
-Demonstrates propositions of supervised machine learning theories
+Demonstrates propositions of supervised machine learning theories.
 
 ## Installation
 
 ```bash
 $ pip install smltheory
 ```
 
 ## Usage
 
-`sml_theory` can be used to demonstrate propositions of
+`smltheory` can be used to demonstrate propositions of
 supervised machine learning theories. Specifically, the functions
 demonstrate the propositions of excess risk decomposition
 and the bias-variance tradeoff. 
 
-```python
-#compute Bayes risk 
-
-
-
-```
+For a demonstration of each supervised machine learning proposition, see 
+[whitepaper](https://sebastiansciarra.com/technical_content/understanding_ML). 
 
 
 
 
 ## Contributing
 
 Interested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.
```

### Comparing `smltheory-0.1.4/pyproject.toml` & `smltheory-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smltheory"
-version = "0.1.4"
+version = "0.1.5"
 description = "Demonstrates propositions of supervised machine learning theories"
 authors = ["Sebastian Sciarra"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
```

### Comparing `smltheory-0.1.4/src/smltheory/bayes_decision.py` & `smltheory-0.1.5/src/smltheory/bayes_decision.py`

 * *Files 26% similar despite different names*

```diff
@@ -35,26 +35,41 @@
      Returns
      -------
      bayes_features : pandas.core.frame.DataFrame
          A dataframe that contains features needed to compute Bayes decision function predictions
 
      See Also
      --------
+     generate_data.create_covariance_matrix()
      generate_data.generate_mult_trunc_normal()
 
      Examples
      ---------
      >>> mu=[5, 7]
      >>> sd=[1.2, 1.7]
      >>> rho_weather_winemaking =  0.35
-     >>> cov_matrix=generate_data.create_covariance_matrix(sd=sd, rho=rho_weather_winemaking)
-     >>>sample_size_gen_error = 150
-     >>> data_gen_error = generate_data.generate_mult_trunc_normal(cov_matrix=cov_matrix, sd=sd,
-                          mu=mu, sample_size=sample_size_gen_error)
+     >>> cov_matrix = create_covariance_matrix(sd=sd, rho=rho_weather_winemaking)
+     #generate data set
+     >>> sample_size_gen_error = 150
+     >>> data_gen_error = generate_mult_trunc_normal(cov_matrix=cov_matrix, mu=mu,
+     ... sample_size=sample_size_gen_error)
+     #compute features for Bayes decision function
      >>> compute_bayes_features(data=data_gen_error)
+          weather  winemaking_quality    weather  winemaking_quality          0
+     0    5.214258            6.655854  27.188488           44.300390  34.705340
+     1    5.459996            4.313195  29.811557           18.603650  23.550027
+     2    4.813125            8.830114  23.166172           77.970922  42.500444
+     3    5.499881            6.345226  30.248688           40.261895  34.897987
+     4    5.235549            8.265799  27.410970           68.323429  43.275991
+     ..        ...                 ...        ...                 ...        ...
+     145  6.020267            7.603160  36.243618           57.808035  45.773053
+     146  3.982080            7.635946  15.856965           58.307675  30.406952
+     147  5.654110            9.818515  31.968960           96.403227  55.514961
+     148  8.112048            6.618283  65.805322           43.801670  53.687829
+     149  3.384190            6.122903  11.452739           37.489943  20.721065
      """
 
     # Feature columns
     predictors = data[["weather", "winemaking_quality"]]
     bayes_features = pd.concat(objs=[predictors, predictors**2, predictors.prod(axis=1)], axis=1)
 
     return bayes_features
@@ -83,19 +98,22 @@
     generate_data.generate_mult_trunc_normal()
 
     Examples
     ---------
     >>> mu = [5, 7]
     >>> sd = [1.2, 1.7]
     >>> rho_weather_winemaking =  0.35
-    >>> cov_matrix = generate_data.create_covariance_matrix(sd=sd, rho=rho_weather_winemaking)
+    >>> cov_matrix = create_covariance_matrix(sd=sd, rho=rho_weather_winemaking)
+    #generate data set
     >>> sample_size_gen_error = 150
-    >>> data_gen_error = generate_data.generate_mult_trunc_normal(cov_matrix=cov_matrix, sd=sd,
-                         mu=mu, sample_size=sample_size_gen_error)
+    >>> data_gen_error = generate_mult_trunc_normal(cov_matrix=cov_matrix, mu=mu,
+    ... sample_size=sample_size_gen_error)
+    #compute intercept of Bayes decision function
     >>> compute_bayes_intercept(data=data_gen_error)
+    4.977118063990485
     """
 
     bayes_features = generate_bayes_features(data=data)
 
     # Intercept
     intercept = np.mean(data["wine_quality"]) - np.sum(provide_weights() * compute_rescaling_factor() *
                                                        np.mean(bayes_features, axis=0))
@@ -126,19 +144,21 @@
     generate_data.generate_mult_trunc_normal()
 
     Examples
     --------
     >>> mu = [5, 7]
     >>> sd = [1.2, 1.7]
     >>> rho_weather_winemaking =  0.35
-    >>> cov_matrix = generate_data.create_covariance_matrix(sd=sd, rho=rho_weather_winemaking)
+    >>> cov_matrix = create_covariance_matrix(sd=sd, rho=rho_weather_winemaking)
+    #generate data
     >>> sample_size_gen_error = 150
-    >>> data_gen_error = generate_data.generate_mult_trunc_normal(cov_matrix=cov_matrix, sd=sd,
-                         mu=mu, sample_size=sample_size_gen_error)
+    >>> data_gen_error = generate_mult_trunc_normal(cov_matrix=cov_matrix, mu=mu,
+    ... sample_size=sample_size_gen_error)
     >>> compute_bayes_risk(data=data_gen_error)
+    0.25105984029122547
     """
 
     bayes_features = generate_bayes_features(data=data)
 
     # Compute intercept
     intercept = compute_bayes_intercept(data=data)
```

### Comparing `smltheory-0.1.4/src/smltheory/est_error.py` & `smltheory-0.1.5/src/smltheory/est_error.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 In the excess risk decomposition setup, a constrained set of functions must be
 considered to reduce the incidence of overfitting. Because sample sizes are limited
 in practice, the best possible function in the constrained set of functions (i.e.,
 constrained empirical risk minimizer, :math:`f_\\mathcal{F}`) is unlikely to be obtained. Instead, an estimate
 of the constrained empirical risk minimizer will result and will have a larger
 generalization error than the constrained empirical risk minimizer. I call this estimate
 the sample risk minimizer, :math:`\\hat{f}_s`. This module computes the generalization error of the optimization risk
-minimizer. For more details, see whitepaper at `sebastiansciarra.com <https://sebastiansciarra.com/technical_content/understanding_ML>`_.
+minimizer. For more details, see whitepaper at
+ `sebastiansciarra.com <https://sebastiansciarra.com/technical_content/understanding_ML>`_.
 
 References
 ----------
 [1] Bottou, L. & Bousquet, O. (2007). The tradeoffs of large scale learning. InKoller, S.
 (Eds.), Advances in neural information processing systems.
 (pp. 161–168). Curran Associates, Inc. `bit.ly/3qo1xpI <bit.ly/3qo1xpI>`_.
 """
@@ -53,25 +54,26 @@
     generate_data.generate_mult_trunc_normal()
 
     Examples
     --------
     >>> mu = [5, 7]
     >>> sd = [1.2, 1.7]
     >>> rho_weather_winemaking =  0.35
-    >>> cov_matrix = generate_data.create_covariance_matrix(sd=sd, rho=rho_weather_winemaking)
+    >>> cov_matrix = create_covariance_matrix(sd=sd, rho=rho_weather_winemaking)
     >>> sample_size_gen_error = 150
-    >>> sample_size_data_best_in_class = 1e4
-
-    >>> data_best_in_class = generate_data.generate_mult_trunc_normal(cov_matrix = cov_matrix, mu = mu,
-                             sample_size=best_in_class_sample_size, seed=7)
-    >>> data_gen_error = generate_data.generate_mult_trunc_normal(cov_matrix=cov_matrix, sd=sd,
-                         mu=mu, sample_size=sample_size_gen_error, seed = 22)
-    >>> compute_sample_risk_gen_error(sample_size=50,
-                                     data_best_in_class=data_best_in_class,
-                                     data_gen_error=data_gen_error)
+    >>> sample_size_data_best_in_class = 500
+    #generate data sets
+    >>> data_best_in_class = generate_mult_trunc_normal(cov_matrix = cov_matrix, mu = mu,
+    ... sample_size=sample_size_data_best_in_class, seed=7)
+    >>> data_gen_error = generate_mult_trunc_normal(cov_matrix=cov_matrix, mu=mu,
+    ... sample_size=sample_size_gen_error, seed = 21)
+    #compute generalization error of sample risk minimizer
+    >>> compute_sample_risk_gen_error(sample_size=50, data_best_in_class=data_best_in_class,
+    ... data_gen_error=data_gen_error)
+    0.22130558411285997
 """
     # Use random_state to ensure reproducibility and prevent resampling from adding noise to estimates
     gen_errors = compute_all_emp_gen_errors(data_emp_loss=data_best_in_class.sample(n=sample_size, random_state=27),
                                             data_gen_error=data_gen_error,
                                             include_interactions=False,
                                             poly_order_range=poly_order_range)['gen_error']
```

### Comparing `smltheory-0.1.4/src/smltheory/generate_data.py` & `smltheory-0.1.5/src/smltheory/generate_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     --------
     weights: numpy.ndarray
         Weights of Bayes decision function.
 
     Examples
     --------
     >>> provide_weights()
+    array([ 0.3 ,  0.1 ,  0.07, -0.1 ,  0.1 ])
     """
 
     b_weight_weather = 0.3
     b_weight_winemaking = 0.1
     b_weight_weather_squared = 0.07
     b_weight_winemaking_squared = -0.1
     b_weight_weather_winemaking = 0.1
@@ -60,14 +61,15 @@
     --------
     old_upper_limit - old_lower_limit: numpy.float.64
         Old range of outcome variable.
 
     Examples
     --------
     >>> compute_old_scale_range()
+    27.63
     """
 
     # assume highest/lowest possible error scores are +-3 SDs
     old_lower_limit = np.dot(a=provide_weights(), b=np.array([1, 10, 1, 100, 10])) - 3 * 1.5
     old_upper_limit = np.dot(a=provide_weights(), b=np.array([10, 10, 100, 100, 100])) + 3 * 1.5
 
     return old_upper_limit - old_lower_limit
@@ -96,15 +98,16 @@
     Returns
     --------
     rescaling_factor: numpy.float64
         Factor for rescaling from old scale to new scale.
 
     Examples
     --------
-    >>> compute_rescaling_factor(new_upper_limit=5, new_lower_limit=10)
+    >>> compute_rescaling_factor(new_upper_limit=10, new_lower_limit=5)
+    0.18096272167933405
     """
     old_scale_range = compute_old_scale_range()
     new_scale_range = new_upper_limit - new_lower_limit
 
     rescaling_factor = new_scale_range / old_scale_range
 
     return rescaling_factor
@@ -144,15 +147,17 @@
 
     Examples
     --------
     >>> mu = [5, 7]
     >>> sd = [1.2, 1.7]
     #population correlation between weather and winemaking quality
     >>> rho_weather_winemaking =  0.35
-    >>> cov_matrix = create_covariance_matrix(sd = sd, rho =  rho_weather_winemaking)
+    >>> create_covariance_matrix(sd = sd, rho =  rho_weather_winemaking)
+    array([[1.2  , 0.714],
+            [0.714, 1.7  ]])
     """
 
     # Create a lower triangular matrix with zeros
     n = len(sd)
     cov_matrix = np.zeros((n, n))
 
     # Fill lower and upper triangles of covariance matrix
@@ -173,30 +178,58 @@
     original (or old) scale range. For more information, see whitepaper
     at `sebastiansciarra.com <https://sebastiansciarra.com/technical_content/understanding_ML>`_.
 
     Parameters
     ---------
     mu: pandas.core.frame.DataFrame
         Data set containing predictors (weather, winemaking quality) and outcome variable (wine quality).
+
     cov_matrix: int
         Upper limit of new scale.
+
     sample_size: int
-        New lower limit.
+        Sample size of for data set containing predictors.
+
     lower_limits: int
+        Lower limit of predictors.
+
     upper_limits: int
+        Upper limits of predictors.
+
     seed: int
+        Seed value for random number generator.
 
     Returns
     --------
     truncated_data:  pandas.core.frame.DataFrame
         Factor for rescaling from old scale to new scale.
 
     Examples
     --------
-    >>> compute_rescaling_factor(new_upper_limit=10, new_lower_limit=2)
+    >>> mu = [5, 7]
+    ... sd = [1.2, 1.7]
+    ... rho_weather_winemaking =  0.35
+    #generate covariance matrix
+    >>> cov_matrix = create_covariance_matrix(sd = sd, rho =  rho_weather_winemaking)
+    #genrate predictor data
+    generate_trunc_predictors(mu=mu, cov_matrix = cov_matrix, sample_size = 150)
+         weather  winemaking_quality
+    0    5.214258            6.655854
+    1    5.459996            4.313195
+    2    4.813125            8.830114
+    3    5.499881            6.345226
+    4    5.235549            8.265799
+    ..        ...                 ...
+    145  6.020267            7.603160
+    146  3.982080            7.635946
+    147  5.654110            9.818515
+    148  8.112048            6.618283
+    149  3.384190            6.122903
+
+    [150 rows x 2 columns]
     """
     # Upper and lower limits for variables
     lower_limits = np.repeat(lower_limits, len(mu))
     upper_limits = np.repeat(upper_limits, len(mu))
 
     # Generate samples from multivariate distribution
     sample_size = int(sample_size)
@@ -240,20 +273,33 @@
     generate_data.generate_trunc_predictors()
 
     Examples
     --------
     >>> mu = [5, 7]
     >>> sd = [1.2, 1.7]
     >>> rho_weather_winemaking =  0.35
-    >>> cov_matrix = generate_data.create_covariance_matrix(sd=sd, rho=rho_weather_winemaking)
-    >>> sample_size_gen_error = 150
-    >>> sample_size_data_best_in_class = 1e4
+    >>> cov_matrix = create_covariance_matrix(sd=sd, rho=rho_weather_winemaking)
+    #generate data and compute outcome variable
     >>> data = generate_trunc_predictors(mu=mu, cov_matrix=cov_matrix,
-    ... sample_size=sample_size, seed=27)
+    ... sample_size=150, seed=27)
     >>> compute_outcome_variable(data=data)
+              weather  winemaking_quality  wine_quality
+    0    5.214258            6.655854      4.496573
+    1    5.459996            4.313195      5.847665
+    2    4.813125            8.830114     -0.288320
+    3    5.499881            6.345226      0.672006
+    4    5.235549            8.265799     -0.912242
+    ..        ...                 ...           ...
+    145  6.020267            7.603160      4.538715
+    146  3.982080            7.635946      0.727746
+    147  5.654110            9.818515      0.327821
+    148  8.112048            6.618283      7.094816
+    149  3.384190            6.122903      0.930205
+
+    [150 rows x 3 columns]
     """
 
     feature_cols = pd.concat(objs=[data, data ** 2, data.prod(axis=1)], axis=1)
 
     # Error
     error = np.random.normal(loc=0, scale=1.5, size=data.shape[0])
 
@@ -281,15 +327,37 @@
     Returns
     --------
     data: pandas.core.frame.DataFrame
         Data set containing predictors (weather, winemaking quality) and rescaled outcome variable (wine quality).
 
     Examples
     --------
-    >>> compute_rescaling_factor(new_upper_limit=10, new_lower_limit=2)
+    >>> mu = [5, 7]
+    >>> sd = [1.2, 1.7]
+    >>> rho_weather_winemaking =  0.35
+    >>> cov_matrix = create_covariance_matrix(sd=sd, rho=rho_weather_winemaking)
+    #generate data and compute outcome variable
+    >>> data = generate_trunc_predictors(mu=mu, cov_matrix=cov_matrix,
+    ... sample_size=150, seed=27)
+    >>> data = compute_outcome_variable(data=data)
+    >>> rescale_outcome_variable(data=data)
+         weather  winemaking_quality  wine_quality
+    0    5.214258            6.655854      6.415822
+    1    5.459996            4.313195      6.855917
+    2    4.813125            8.830114      4.857225
+    3    5.499881            6.345226      5.170035
+    4    5.235549            8.265799      4.653993
+    ..        ...                 ...           ...
+    145  6.020267            7.603160      6.429549
+    146  3.982080            7.635946      5.188191
+    147  5.654110            9.818515      5.057922
+    148  8.112048            6.618283      7.262155
+    149  3.384190            6.122903      5.254139
+
+    [150 rows x 3 columns]
     """
     rescaling_factor = compute_rescaling_factor(new_upper_limit=new_upper_limit,
                                                 new_lower_limit=new_lower_limit)
     old_lower_limit = np.dot(a=provide_weights(), b=np.array([1, 10, 1, 100, 10])) - 3 * 1.5
     lower_limit_center = (data["wine_quality"] - old_lower_limit)
 
     data["wine_quality"] = pd.DataFrame(data=new_lower_limit + lower_limit_center * rescaling_factor,
@@ -298,16 +366,16 @@
     return data
 
 
 def generate_mult_trunc_normal(cov_matrix, mu, sample_size, seed=27):
     """Generates multivariate normal truncated data.
 
     Data for features (weather, winemaking quality) and outcome (wine quality) are generated according
-    to truncated normal distrib utions. For more details,see `
-    sebastiansciarra.com <https://sebastiansciarra.com/technical_content/understanding_ML>`_.
+    to truncated normal distrib utions. For more details, see `sebastiansciarra.com
+    <https://sebastiansciarra.com/technical_content/understanding_ML>`_.
 
     Parameters
     ----------
     cov_matrix: pandas.core.frame.DataFrame
         Data set containing predictors (weather, winemaking quality).
     mu: list
         Specifies population-level mean for features.
@@ -322,25 +390,37 @@
         Data set containing predictors (weather, winemaking quality) and outcome variable (wine quality),
         with data for the predictors and outcome rescaled on the desired range.
 
     See Also
     --------
     generate_data.generate_trunc_predictors()
     generate_data.compute_outcome_variable()
-    generate_data.rescale_outcome_variable
+
     Examples
     --------
     >>> mu = [5, 7]
     ... sd = [1.2, 1.7]
     ... rho_weather_winemaking =  0.35
     #generate covariance matrix
     >>> cov_matrix = create_covariance_matrix(sd=sd, rho=rho_weather_winemaking)
     #specify sample sizes for data sets
     >>> generate_mult_trunc_normal(cov_matrix=cov_matrix, mu=mu,
     ... sample_size=150, seed=27)
+         weather  winemaking_quality  wine_quality
+    0    5.214258            6.655854      6.415822
+    1    5.459996            4.313195      6.855917
+    2    4.813125            8.830114      4.857225
+    3    5.499881            6.345226      5.170035
+    4    5.235549            8.265799      4.653993
+    ..        ...                 ...           ...
+    145  6.020267            7.603160      6.429549
+    146  3.982080            7.635946      5.188191
+    147  5.654110            9.818515      5.057922
+    148  8.112048            6.618283      7.262155
+    149  3.384190            6.122903      5.254139
     """
     # generate predictors
     data_mult_trunc_normal = generate_trunc_predictors(mu=mu, cov_matrix=cov_matrix,
                                                        sample_size=sample_size, seed=seed)
 
     # generate outcome variable
     data_mult_trunc_normal = compute_outcome_variable(data=data_mult_trunc_normal)
```

### Comparing `smltheory-0.1.4/src/smltheory/gradient_descent.py` & `smltheory-0.1.5/src/smltheory/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.4/src/smltheory/least_squares.py` & `smltheory-0.1.5/src/smltheory/least_squares.py`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.4/src/smltheory/opt_error.py` & `smltheory-0.1.5/src/smltheory/opt_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,20 +67,20 @@
     >>> cov_matrix = create_covariance_matrix(sd=sd, rho=rho_weather_winemaking)
     #specify sample sizes for data sets
     >>> sample_size_gen_error = 150
     ... sample_size_data_best_in_class = 1e4
     #generate data sets
     >>> data_best_in_class = generate_mult_trunc_normal(cov_matrix = cov_matrix, mu = mu,
     ... sample_size=sample_size_data_best_in_class, seed=7)
-    >>> data_gen_error = generate_mult_trunc_normal(cov_matrix=cov_matrix, sd=sd,
-    ... mu=mu, sample_size=sample_size_gen_error, seed = 22
+    >>> data_gen_error = generate_mult_trunc_normal(cov_matrix=cov_matrix, mu=mu,
+    ... sample_size=sample_size_gen_error, seed = 22
     >>> data_sample = data_best_in_class.sample(n=50, random_state=27)
     #determine best polynomial model
-    >>> best_model_poly_order = determine_best_polynomial_model(data_sample=data_sample,
-    ... data_gen_error=data_gen_error)
+    >>> determine_best_polynomial_model(data_sample=data_sample, data_gen_error=data_gen_error)
+    2
     """
     # Use random_state to ensure reproducibility and prevent resampling from adding noise to estimates
     df_all_emp_gen_errors = compute_all_emp_gen_errors(data_emp_loss=data_sample,
                                                        data_gen_error=data_gen_error,
                                                        include_interactions=False,
                                                        poly_order_range=poly_order_range)
 
@@ -124,26 +124,27 @@
     #generate covariance matrix
     >>> cov_matrix = create_covariance_matrix(sd=sd, rho=rho_weather_winemaking)
     #specify sample sizes for data sets
     >>> sample_size_gen_error = 150
     ... sample_size_data_best_in_class = 1e4
     #generate data sets
     >>> data_best_in_class = generate_mult_trunc_normal(cov_matrix = cov_matrix, mu = mu,
-    ... sample_size=best_in_class_sample_size, seed=7)
-    >>> data_gen_error = generate_mult_trunc_normal(cov_matrix=cov_matrix, sd=sd,
-    ... mu=mu, sample_size=sample_size_gen_error, seed = 22
-    >>> data_sample = data_best_in_class.sample(n=sample_size, random_state=27)
+    ... sample_size=sample_size_data_best_in_class, seed=7)
+    >>> data_gen_error = generate_mult_trunc_normal(cov_matrix=cov_matrix, mu=mu,
+    ... sample_size=sample_size_gen_error, seed = 22)
+    >>> data_sample = data_best_in_class.sample(n=50, random_state=27)
     #determine best polynomial model
     >>> best_model_poly_order = determine_best_polynomial_model(data_sample=data_sample,
     ... data_gen_error=data_gen_error)
     #set initial guess for regression weights
     >>> opt_weights = np.random.uniform(low=0, high=1, size=2 * best_model_poly_order)
     #compute generalization error of optimization risk minimizer
-    >>> compute_opt_gen_error(opt_weights=opt_weights, poly_order=poly_order,
+    >>> compute_opt_gen_error(opt_weights=opt_weights, poly_order=best_model_poly_order,
     ... data_gen_error=data_gen_error)
+    451.0819816097045
     """
     # gather necessary components for matrix-matrix multiplications
     dict_data = extract_feature_outcome_data(data=data_gen_error, poly_order=poly_order)
     features = dict_data["features"]
     outcome = dict_data["outcome"].ravel()
 
     # compute predictions and generalization error
@@ -196,26 +197,27 @@
 
     Examples
     --------
     >>> mu = [5, 7]
     ... sd = [1.2, 1.7]
     ... rho_weather_winemaking =  0.35
     #generate covariance matrix
-    >>> cov_matrix = generate_data.create_covariance_matrix(sd=sd, rho=rho_weather_winemaking)
+    >>> cov_matrix = create_covariance_matrix(sd=sd, rho=rho_weather_winemaking)
     #specify sample sizes for data sets
     >>> sample_size_gen_error = 150
     ... sample_size_data_best_in_class = 1e4
     #generate data sets
-    >>> data_best_in_class = generate_data.generate_mult_trunc_normal(cov_matrix = cov_matrix, mu = mu,
+    >>> data_best_in_class = generate_mult_trunc_normal(cov_matrix = cov_matrix, mu = mu,
     ... sample_size=best_in_class_sample_size, seed=7)
-    >>> data_gen_error = generate_data.generate_mult_trunc_normal(cov_matrix=cov_matrix, sd=sd,
-    ... mu=mu, sample_size=sample_size_gen_error, seed = 22
+    >>> data_gen_error = generate_mult_trunc_normal(cov_matrix=cov_matrix, mu=mu,
+    ... sample_size=sample_size_gen_error, seed = 22
     #compute generalization error of optimization risk minimizer
     >>> get_opt_risk_min(sample_size = 50, data_best_in_class=data_best_in_class, data_gen_error=data_gen_error,
     ... num_iterations=500)
+    0.34195817817471824
     """
     # Step 1: Using empirical risk minimization to determine the polynomial model order that results in the lowest
     # empirical loss
     data_sample = data_best_in_class.sample(n=sample_size, random_state=27)
     best_model_poly_order = determine_best_polynomial_model(data_sample=data_sample,
                                                             data_gen_error=data_gen_error)
```

### Comparing `smltheory-0.1.4/src/smltheory/overfitting.py` & `smltheory-0.1.5/src/smltheory/overfitting.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 whitepaper at `sebastiansciarra.com <https://sebastiansciarra.com/technical_content/understanding_ML>`_.
 """
 
 import statsmodels.formula.api as smf
 from sklearn.metrics import mean_squared_error
 from functools import partial
 import pandas as pd
+import numpy as np
+
 
 
 def gen_poly_reg_eq(poly_order, include_interactions=False):
     """Generates equation for polynomial model of specified order.
 
     Parameters
     ----------
```

### Comparing `smltheory-0.1.4/src/smltheory/trun_mvnt.py` & `smltheory-0.1.5/src/smltheory/trun_mvnt.py`

 * *Files identical despite different names*

### Comparing `smltheory-0.1.4/PKG-INFO` & `smltheory-0.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 Metadata-Version: 2.1
 Name: smltheory
-Version: 0.1.4
+Version: 0.1.5
 Summary: Demonstrates propositions of supervised machine learning theories
 License: MIT
 Author: Sebastian Sciarra
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.3)
 Requires-Dist: scipy (>=1.11.1)
 Description-Content-Type: text/markdown
 
-# sml_theory
+# smltheory
 
-Demonstrates propositions of supervised machine learning theories
+Demonstrates propositions of supervised machine learning theories.
 
 ## Installation
 
 ```bash
 $ pip install smltheory
 ```
 
 ## Usage
 
-`sml_theory` can be used to demonstrate propositions of
+`smltheory` can be used to demonstrate propositions of
 supervised machine learning theories. Specifically, the functions
 demonstrate the propositions of excess risk decomposition
 and the bias-variance tradeoff. 
 
-```python
-#compute Bayes risk 
-
-
-
-```
+For a demonstration of each supervised machine learning proposition, see 
+[whitepaper](https://sebastiansciarra.com/technical_content/understanding_ML). 
 
 
 
 
 ## Contributing
 
 Interested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.
```

