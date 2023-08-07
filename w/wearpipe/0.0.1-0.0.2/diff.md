# Comparing `tmp/wearpipe-0.0.1.tar.gz` & `tmp/wearpipe-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wearpipe-0.0.1.tar", last modified: Fri Aug  4 16:48:05 2023, max compression
+gzip compressed data, was "wearpipe-0.0.2.tar", last modified: Mon Aug  7 15:22:34 2023, max compression
```

## Comparing `wearpipe-0.0.1.tar` & `wearpipe-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 16:48:05.158270 wearpipe-0.0.1/
--rw-rw-rw-   0        0        0        0 2023-08-04 15:13:48.000000 wearpipe-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      311 2023-08-04 16:48:05.157272 wearpipe-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-08-04 15:14:11.000000 wearpipe-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-08-04 16:48:05.158270 wearpipe-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      494 2023-08-04 16:45:34.000000 wearpipe-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:48:05.133978 wearpipe-0.0.1/wearpipe/
--rw-rw-rw-   0        0        0      100 2023-08-04 16:47:19.000000 wearpipe-0.0.1/wearpipe/__init__.py
--rw-rw-rw-   0        0        0     6568 2023-08-04 16:15:40.000000 wearpipe-0.0.1/wearpipe/wearpipe.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:48:05.156304 wearpipe-0.0.1/wearpipe.egg-info/
--rw-rw-rw-   0        0        0      311 2023-08-04 16:48:04.000000 wearpipe-0.0.1/wearpipe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-08-04 16:48:05.000000 wearpipe-0.0.1/wearpipe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 16:48:04.000000 wearpipe-0.0.1/wearpipe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-08-04 16:48:04.000000 wearpipe-0.0.1/wearpipe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-04 16:48:04.000000 wearpipe-0.0.1/wearpipe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 15:22:34.838401 wearpipe-0.0.2/
+-rw-rw-rw-   0        0        0        0 2023-08-04 15:13:48.000000 wearpipe-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      311 2023-08-07 15:22:34.837405 wearpipe-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-08-04 15:14:11.000000 wearpipe-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-07 15:22:34.838401 wearpipe-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      494 2023-08-07 15:22:29.000000 wearpipe-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 15:22:34.821104 wearpipe-0.0.2/wearpipe/
+-rw-rw-rw-   0        0        0      100 2023-08-04 16:47:19.000000 wearpipe-0.0.2/wearpipe/__init__.py
+-rw-rw-rw-   0        0        0     6770 2023-08-07 15:21:34.000000 wearpipe-0.0.2/wearpipe/wearpipe.py
+drwxrwxrwx   0        0        0        0 2023-08-07 15:22:34.836407 wearpipe-0.0.2/wearpipe.egg-info/
+-rw-rw-rw-   0        0        0      311 2023-08-07 15:22:34.000000 wearpipe-0.0.2/wearpipe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-08-07 15:22:34.000000 wearpipe-0.0.2/wearpipe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 15:22:34.000000 wearpipe-0.0.2/wearpipe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-08-07 15:22:34.000000 wearpipe-0.0.2/wearpipe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-07 15:22:34.000000 wearpipe-0.0.2/wearpipe.egg-info/top_level.txt
```

### Comparing `wearpipe-0.0.1/wearpipe/wearpipe.py` & `wearpipe-0.0.2/wearpipe/wearpipe.py`

 * *Files 9% similar despite different names*

```diff
@@ -68,37 +68,42 @@
     Parameters:
     df: DataFrame, the original data.
     feature_columns: list, the names of the feature columns.
     model: Keras model, the trained LSTM model.
     le: LabelEncoder, the label encoder used during training.
 
     Returns:
-    df: DataFrame, the original DataFrame with an additional column for the model's predictions.
+    df: DataFrame, the original DataFrame with additional columns for the model's predictions and their confidence.
     """
 
     # Extract features
     features = df[feature_columns].values
 
     # Reshape input to be 3D [samples, timesteps, features]
     features = features.reshape((features.shape[0], 1, features.shape[1]))
     
     # Make predictions
     predictions = model.predict(features)
     predictions_classes = np.argmax(predictions, axis=1)
     
+    # Compute prediction confidences
+    prediction_confidences = np.max(predictions, axis=1)
+    
     # Transform class indices back into original labels
     predictions_labels = le.inverse_transform(predictions_classes)
     
-    # Add predictions to original DataFrame
+    # Add predictions and their confidence to original DataFrame
     df['Predictions'] = predictions_labels
+    df['Prediction_Confidence'] = prediction_confidences
 
     return df
 
 
 
+
 def choi_non_wear(df, accx, accy, accz, sampling_rate, non_wear_time_threshold=60, std_threshold=0.013, range_threshold=0.05):
     """
     Parameters:
     df: DataFrame, the original data.
     sampling_rate: int, the number of data points per minute.
     non_wear_time_threshold: int, the time threshold (in minutes) to detect non-wear.
     std_threshold: int, the standard deviation threshold to detect non-wear.
```

