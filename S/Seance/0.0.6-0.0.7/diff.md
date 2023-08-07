# Comparing `tmp/Seance-0.0.6-py3-none-any.whl.zip` & `tmp/Seance-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 15839 bytes, number of entries: 16
+Zip file size: 16015 bytes, number of entries: 16
 -rw-rw-rw-  2.0 fat     2392 b- defN 23-Aug-02 14:22 Seance/Explainer.py
--rw-rw-rw-  2.0 fat    13078 b- defN 23-Aug-03 17:10 Seance/Forecaster.py
--rw-rw-rw-  2.0 fat    11395 b- defN 23-Jul-30 23:54 Seance/Optimizer.py
+-rw-rw-rw-  2.0 fat    13092 b- defN 23-Aug-07 01:58 Seance/Forecaster.py
+-rw-rw-rw-  2.0 fat    12090 b- defN 23-Aug-07 01:58 Seance/Optimizer.py
 -rw-rw-rw-  2.0 fat       27 b- defN 23-May-04 14:41 Seance/__init__.py
 -rw-rw-rw-  2.0 fat     3358 b- defN 23-May-18 13:18 Seance/Builder/PanelAxis.py
 -rw-rw-rw-  2.0 fat     3916 b- defN 23-Jul-06 20:13 Seance/Builder/PreProcess.py
--rw-rw-rw-  2.0 fat     6595 b- defN 23-May-31 15:17 Seance/Builder/Transformations.py
+-rw-rw-rw-  2.0 fat     6595 b- defN 23-Aug-07 01:49 Seance/Builder/Transformations.py
 -rw-rw-rw-  2.0 fat       27 b- defN 23-May-04 14:40 Seance/Builder/__init__.py
 -rw-rw-rw-  2.0 fat       27 b- defN 23-Jun-03 01:07 Seance/basis_functions/__init__.py
 -rw-rw-rw-  2.0 fat      845 b- defN 23-Jul-06 19:45 Seance/basis_functions/fourier_basis.py
 -rw-rw-rw-  2.0 fat     2834 b- defN 23-May-31 21:10 Seance/basis_functions/linear_basis.py
--rw-rw-rw-  2.0 fat     1087 b- defN 23-Aug-03 17:14 Seance-0.0.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2725 b- defN 23-Aug-03 17:14 Seance-0.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-03 17:14 Seance-0.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Aug-03 17:14 Seance-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1303 b- defN 23-Aug-03 17:14 Seance-0.0.6.dist-info/RECORD
-16 files, 49708 bytes uncompressed, 13691 bytes compressed:  72.5%
+-rw-rw-rw-  2.0 fat     1088 b- defN 23-Aug-07 01:59 Seance-0.0.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2725 b- defN 23-Aug-07 01:59 Seance-0.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-07 01:59 Seance-0.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Aug-07 01:59 Seance-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1303 b- defN 23-Aug-07 01:59 Seance-0.0.7.dist-info/RECORD
+16 files, 50418 bytes uncompressed, 13867 bytes compressed:  72.5%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: Seance/basis_functions/fourier_basis.py
 Comment: 
 
 Filename: Seance/basis_functions/linear_basis.py
 Comment: 
 
-Filename: Seance-0.0.6.dist-info/LICENSE
+Filename: Seance-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: Seance-0.0.6.dist-info/METADATA
+Filename: Seance-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: Seance-0.0.6.dist-info/WHEEL
+Filename: Seance-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: Seance-0.0.6.dist-info/top_level.txt
+Filename: Seance-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: Seance-0.0.6.dist-info/RECORD
+Filename: Seance-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Seance/Forecaster.py

```diff
@@ -115,15 +115,15 @@
             for i in self.seasonal_period:
                 fourier_basis = get_fourier_series(length=len(self.time_periods),
                                                    seasonal_period=i,
                                                    fourier_order=self.fourier_order)
                 column_names = [f'{i}_fourier_{j+1}' for j in range(2 * self.fourier_order)]
                 fourier_basis = pd.DataFrame(fourier_basis, columns=column_names)
                 seasonal_df.append(fourier_basis)
-            seasonal_df = pd.concat(seasonal_df)
+            seasonal_df = pd.concat(seasonal_df, axis=1)
             seasonal_df[date_column] = self.time_periods.values
             seasonal_df[date_column] = pd.to_datetime(seasonal_df[date_column]).dt.tz_localize(None)
             max_period = max(self.seasonal_period)
         else:
             max_period = None
 
         if differences is not None:
@@ -236,15 +236,15 @@
                 fourier_basis = get_future_fourier(forecast_horizon=forecast_horizon,
                                                    length=len(self.time_periods),
                                                    seasonal_period=i,
                                                    fourier_order=self.fourier_order)
                 column_names = [f'{i}_fourier_{j+1}' for j in range(2 * self.fourier_order)]
                 fourier_basis = pd.DataFrame(fourier_basis, columns=column_names).astype(float)
                 seasonal_df.append(fourier_basis)
-            seasonal_df = pd.concat(seasonal_df)
+            seasonal_df = pd.concat(seasonal_df, axis=1)
             seasonal_df[self.date_column] = full_dates.values
             pred_X = pred_X.merge(seasonal_df, on=self.date_column)
         if self.n_basis is not None and self.n_basis:
             basis = pred_X.groupby('Seance ID').apply(self.future_linear_basis)
             pred_X = pd.concat([pred_X, basis], axis=1)
         if self.seasonal_period is not None or (self.n_basis is not None and self.n_basis):
             self.dynamic_dfs = [pred_X]
@@ -264,8 +264,7 @@
         return predicted
 
     def plot_importance(self, max_num_features=20):
         lgb.plot_importance(self.mlforecast.models_[self.pred_col],
                             max_num_features=max_num_features)
         return
 
-
```

## Seance/Optimizer.py

```diff
@@ -37,18 +37,26 @@
                  max_bagging_pct=1.0,
                  min_feature_fraction=.6,
                  max_n_basis=25,
                  model='lightgbm',
                  timeout=None):
         self.df = df.sort_values([id_column, date_column])
         if isinstance(seasonal_period, list):
-            self.max_pulse = max(seasonal_period)
+            maxes = []
+            for i in seasonal_period:
+                if isinstance(i, list):
+                    maxes.append(max(i))
+                else:
+                    maxes.append(i)
+            self.max_pulse = max(maxes)
+            self.seasonal_period = seasonal_period
         else:
             self.max_pulse = seasonal_period
-        self.seasonal_period = seasonal_period
+            self.seasonal_period = [seasonal_period]
+
         self.n_folds = n_folds
         self.test_size = test_size
         self.n_trials = n_trials
         self.target_column = target_column
         self.date_column = date_column
         self.id_column = id_column
         self.timeout = timeout
@@ -81,42 +89,42 @@
         self.train_df = df[df['test_split'] == False]
         # self.train_df[self.date_column] = pd.to_datetime(self.train_df[self.date_column]).dt.
         self.test_df = df[df['test_split'] == True]
 
     def scorer(self, params, metric):
         scores = []
         # for train_index, test_index in cv_splits:
-        try:
-            model_obj = Forecaster()
-            model_obj.fit(self.train_df,
-                          target_column=self.target_column,
-                          date_column=self.date_column,
-                          id_column=self.id_column,
-                          freq=self.freq,
-                          categorical_columns=self.categorical_columns,
-                          model=self.model,
-                          **params)
-            predicted = model_obj.predict(self.test_size)
-            self.predicted = predicted
-            if len(predicted) != len(self.test_df):
-                print('Predicted not the same size as test set')
-    
-            if any(np.isnan(predicted[model_obj.pred_col])):
-                scores.append(np.inf)
-            else:
-                # predicted[self.date_column] = predicted[self.date_column].dt.tz_localize(None)
-                self.test_df[self.date_column] = self.test_df[self.date_column].dt.tz_localize(None)
-                self.cv_df = self.test_df[[self.id_column, self.date_column, self.target_column]].merge(predicted, on=[self.id_column, self.date_column])
-                if metric == 'mse':
-                    scores.append(mean_squared_error(self.cv_df[self.target_column].values, self.cv_df[model_obj.pred_col].values))
-                elif metric == 'smape':
-                    scores.append(self.cv_df.groupby(self.id_column).apply(grouped_smape, self.target_column, model_obj.pred_col))
-        except Exception as e:
-                scores.append(np.inf)
-                print(f'ERROR WHILE TUNING: {e}')
+        # try:
+        model_obj = Forecaster()
+        model_obj.fit(self.train_df,
+                      target_column=self.target_column,
+                      date_column=self.date_column,
+                      id_column=self.id_column,
+                      freq=self.freq,
+                      categorical_columns=self.categorical_columns,
+                      model=self.model,
+                      **params)
+        predicted = model_obj.predict(self.test_size)
+        self.predicted = predicted
+        if len(predicted) != len(self.test_df):
+            print('Predicted not the same size as test set')
+
+        if any(np.isnan(predicted[model_obj.pred_col])):
+            scores.append(np.inf)
+        else:
+            # predicted[self.date_column] = predicted[self.date_column].dt.tz_localize(None)
+            self.test_df[self.date_column] = self.test_df[self.date_column].dt.tz_localize(None)
+            self.cv_df = self.test_df[[self.id_column, self.date_column, self.target_column]].merge(predicted, on=[self.id_column, self.date_column])
+            if metric == 'mse':
+                scores.append(mean_squared_error(self.cv_df[self.target_column].values, self.cv_df[model_obj.pred_col].values))
+            elif metric == 'smape':
+                scores.append(self.cv_df.groupby(self.id_column).apply(grouped_smape, self.target_column, model_obj.pred_col))
+    # except Exception as e:
+        #         scores.append(np.inf)
+        #         print(f'ERROR WHILE TUNING: {e}')
         return np.mean(scores)
 
 
     def objective(self, trial):
         params = {
             "use_id": trial.suggest_categorical("use_id", [True, False]),
             "n_basis": trial.suggest_int("n_basis", 0, self.max_n_basis),
@@ -142,24 +150,32 @@
                             'bagging_freq': trial.suggest_int('bagging_freq', 0, 15),
                             "objective": trial.suggest_categorical("objective", ['regression', 'regression_l1'])
             })
         elif self.model == 'ridge':
             params.update({"alpha": trial.suggest_float("alpha", 1e-8, 1000.0)
                            })
         if self.seasonal_period:
-            params.update({'seasonal_period': trial.suggest_categorical("seasonal_period", [None, self.seasonal_period])})
+            if any(isinstance(period, list) for period in self.seasonal_period):
+                choices = self.seasonal_period.copy()
+                choices.append(None)
+                params.update({'seasonal_period': trial.suggest_categorical("seasonal_period", choices)})
+            else:
+                params.update({'seasonal_period': trial.suggest_categorical("seasonal_period", [None, self.seasonal_period])})
+
+            params.update({'fourier_order': trial.suggest_int("fourier_order", 3, 25)})
         if self.ar_lags is not None:
             params.update({'lags': trial.suggest_categorical("lags", self.ar_lags)})
         else:
             if self.seasonal_period:
                 params.update({'lags': trial.suggest_int(name="lags", low=1, high=self.max_pulse + 1)})
                 params['lags'] = list(range(1, params['lags']))
             else:
                 params.update({'lags': trial.suggest_int(name="lags", low=1, high=13)})
                 params['lags'] = list(range(1, params['lags']))
+
         score = self.scorer(params, self.metric)
         return score
 
     def callback(study, trial):
         if len(study.get_trials()) == 2:
             study.stop()
 
@@ -172,14 +188,15 @@
         best_params = study.best_params
         if best_params['lags'] == 1:
             best_params.update({'lags': [study.best_params['lags']]})
         elif isinstance(best_params['lags'], list):
             pass
         else:
             best_params.update({'lags': list(range(1, best_params['lags']))})
+        best_params.update({'model': self.model})
         return best_params, study
 
 #%%
 if __name__ == '__main__':
     import matplotlib.pyplot as plt
     # opt = Optimize(train_df[['V', 'Datetime', 'ID']],
     #             target_column='V',
@@ -193,21 +210,22 @@
     # best_params, study = opt.fit(seed=1)
     import time
     tic = time.perf_counter()
     opt = Optimize(train_df[['V', 'Datetime', 'ID']],
                 target_column='V',
                 date_column='Datetime',
                 id_column='ID',
-                freq='M',
+                freq='Q',
                 metric='smape',
-                seasonal_period=12,
+                scale_types=['none', 'minmax', 'standard'],
+                seasonal_period=[4],
                 model='lightgbm',
-                # ar_lags=[list(range(1, 4))],
-                test_size=26,
-                # n_trials=10,
+                # ar_lags=[[i] for i in [1,2,3,4,5,6,7,8,9,10,11,12]],
+                test_size=5,
+                n_trials=5,
                 timeout=60*60*3)
     best_params, study = opt.fit(seed=1)
     toc = time.perf_counter()
     print(toc - tic)
 
 #%%
     look = opt.test_df
```

## Comparing `Seance-0.0.6.dist-info/LICENSE` & `Seance-0.0.7.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

## Comparing `Seance-0.0.6.dist-info/METADATA` & `Seance-0.0.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Seance
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Wrapper around MLForecast.
 Home-page: https://github.com/tblume1992/Seance
 Author: Tyler Blume
 Author-email: tblume@mail.USF.edu
 Keywords: forecasting,time series,lightgbm,mlforecast
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `Seance-0.0.6.dist-info/RECORD` & `Seance-0.0.7.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Seance/Explainer.py,sha256=f_SHRq6cbtqKmU6wX3pO3WgRrD4xA-QHHEpG1LYcZ0o,2392
-Seance/Forecaster.py,sha256=p5baHpdIwWQnD6Qm3PyOPS9PFrfEcy9VuBhjOT8jUN4,13078
-Seance/Optimizer.py,sha256=6HcRxJMnROPNxMu7rU_F4XvN5UYDREFiyzYATus5epg,11395
+Seance/Forecaster.py,sha256=ZvR9t6XV6yzsnASB7UcHgSL1RBuAcGbeN_OQ1IG5JSw,13092
+Seance/Optimizer.py,sha256=GYSDtlFKUr1SW0NasWSHehJHEGUcuABX3qTAeqCv_Ig,12090
 Seance/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 Seance/Builder/PanelAxis.py,sha256=w5YYnDXgprHWUzCWcqqBEkV1xJ_6qLabzW_PIbQF9ZQ,3358
 Seance/Builder/PreProcess.py,sha256=lXDwzPEYw_01pDEB9533v60uqYJEQE7Jb12vjIxmWhA,3916
 Seance/Builder/Transformations.py,sha256=JY27tWWvxha2JXhVgOALQFJUhV-N2Hcmg2u9hhBSeaA,6595
 Seance/Builder/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 Seance/basis_functions/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 Seance/basis_functions/fourier_basis.py,sha256=8KePMSK7FGqu9t_mkir101B2OvJGZ-FY9kqepiJSCyw,845
 Seance/basis_functions/linear_basis.py,sha256=1RHj--VkbA4heV8QwzNE7a9O0-aPu3Br3EqLlcuUHWU,2834
-Seance-0.0.6.dist-info/LICENSE,sha256=Dk4ScfuH6m_hggBOkCWWWoKU4wkTVtAInrZB4yhn5HU,1087
-Seance-0.0.6.dist-info/METADATA,sha256=6RFVmAWjPpqaeoDHgXkqy7cMs7unZZZh6JlB5xXHFZI,2725
-Seance-0.0.6.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-Seance-0.0.6.dist-info/top_level.txt,sha256=NBiOB1gdtNGUu8k7LuJVpJoaNIhKeZK5izXE8-qbRc0,7
-Seance-0.0.6.dist-info/RECORD,,
+Seance-0.0.7.dist-info/LICENSE,sha256=aRf1taSiJ92tbFDjgbCzfr7RdH-sKYHFIqSRVxwSoBQ,1088
+Seance-0.0.7.dist-info/METADATA,sha256=Sw3kbZr3LJIfv6fVNjgj2CynxMEMd4sEJhD7bQ2X1ns,2725
+Seance-0.0.7.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+Seance-0.0.7.dist-info/top_level.txt,sha256=NBiOB1gdtNGUu8k7LuJVpJoaNIhKeZK5izXE8-qbRc0,7
+Seance-0.0.7.dist-info/RECORD,,
```

