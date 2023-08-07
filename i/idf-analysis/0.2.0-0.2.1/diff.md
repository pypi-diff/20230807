# Comparing `tmp/idf-analysis-0.2.0.tar.gz` & `tmp/idf-analysis-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idf-analysis-0.2.0.tar", last modified: Sat Aug  5 22:53:41 2023, max compression
+gzip compressed data, was "idf-analysis-0.2.1.tar", last modified: Mon Aug  7 13:15:13 2023, max compression
```

## Comparing `idf-analysis-0.2.0.tar` & `idf-analysis-0.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:53:41.463266 idf-analysis-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-05 22:53:27.000000 idf-analysis-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-05 22:53:27.000000 idf-analysis-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14780 2023-08-05 22:53:41.463266 idf-analysis-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13586 2023-08-05 22:53:27.000000 idf-analysis-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:53:41.459266 idf-analysis-0.2.0/idf_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-05 22:53:28.000000 idf-analysis-0.2.0/idf_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-05 22:53:27.000000 idf-analysis-0.2.0/idf_analysis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-05 22:53:27.000000 idf-analysis-0.2.0/idf_analysis/_console_script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:53:41.459266 idf-analysis-0.2.0/idf_analysis/approaches/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-05 22:53:27.000000 idf-analysis-0.2.0/idf_analysis/approaches/ATV-A_121.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-05 22:53:27.000000 idf-analysis-0.2.0/idf_analysis/approaches/KOSTRA.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-05 22:53:27.000000 idf-analysis-0.2.0/idf_analysis/approaches/convective_vs_advective.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-08-05 22:53:27.000000 idf-analysis-0.2.0/idf_analysis/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-08-05 22:53:27.000000 idf-analysis-0.2.0/idf_analysis/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-08-05 22:53:27.000000 idf-analysis-0.2.0/idf_analysis/event_series_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-08-05 22:53:27.000000 idf-analysis-0.2.0/idf_analysis/heavy_rainfall_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-08-05 22:53:27.000000 idf-analysis-0.2.0/idf_analysis/idf_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    34588 2023-08-05 22:53:27.000000 idf-analysis-0.2.0/idf_analysis/idf_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-08-05 22:53:27.000000 idf-analysis-0.2.0/idf_analysis/in_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-08-05 22:53:27.000000 idf-analysis-0.2.0/idf_analysis/interim_result_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-08-05 22:53:27.000000 idf-analysis-0.2.0/idf_analysis/little_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-08-05 22:53:27.000000 idf-analysis-0.2.0/idf_analysis/parameter_formulation_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-08-05 22:53:27.000000 idf-analysis-0.2.0/idf_analysis/parameter_formulations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-08-05 22:53:27.000000 idf-analysis-0.2.0/idf_analysis/plot_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-08-05 22:53:27.000000 idf-analysis-0.2.0/idf_analysis/sww_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-08-05 22:53:27.000000 idf-analysis-0.2.0/idf_analysis/synthetic_rainseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 22:53:41.459266 idf-analysis-0.2.0/idf_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14780 2023-08-05 22:53:41.000000 idf-analysis-0.2.0/idf_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-05 22:53:41.000000 idf-analysis-0.2.0/idf_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 22:53:41.000000 idf-analysis-0.2.0/idf_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-05 22:53:41.000000 idf-analysis-0.2.0/idf_analysis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-05 22:53:41.000000 idf-analysis-0.2.0/idf_analysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-05 22:53:41.000000 idf-analysis-0.2.0/idf_analysis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-08-05 22:53:27.000000 idf-analysis-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 22:53:41.463266 idf-analysis-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 22:53:27.000000 idf-analysis-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:15:13.536529 idf-analysis-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-08-07 13:15:05.000000 idf-analysis-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       98 2023-08-07 13:15:05.000000 idf-analysis-0.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    14780 2023-08-07 13:15:13.536529 idf-analysis-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13586 2023-08-07 13:15:05.000000 idf-analysis-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:15:13.532529 idf-analysis-0.2.1/idf_analysis/
+-rw-r--r--   0 root         (0) root         (0)      624 2023-08-07 13:15:06.000000 idf-analysis-0.2.1/idf_analysis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      245 2023-08-07 13:15:05.000000 idf-analysis-0.2.1/idf_analysis/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      254 2023-08-07 13:15:05.000000 idf-analysis-0.2.1/idf_analysis/_console_script.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:15:13.536529 idf-analysis-0.2.1/idf_analysis/approaches/
+-rw-r--r--   0 root         (0) root         (0)      283 2023-08-07 13:15:05.000000 idf-analysis-0.2.1/idf_analysis/approaches/ATV-A_121.yaml
+-rw-r--r--   0 root         (0) root         (0)      239 2023-08-07 13:15:05.000000 idf-analysis-0.2.1/idf_analysis/approaches/KOSTRA.yaml
+-rw-r--r--   0 root         (0) root         (0)      241 2023-08-07 13:15:05.000000 idf-analysis-0.2.1/idf_analysis/approaches/convective_vs_advective.yaml
+-rw-r--r--   0 root         (0) root         (0)     4309 2023-08-07 13:15:05.000000 idf-analysis-0.2.1/idf_analysis/arg_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-08-07 13:15:05.000000 idf-analysis-0.2.1/idf_analysis/definitions.py
+-rw-r--r--   0 root         (0) root         (0)     7365 2023-08-07 13:15:05.000000 idf-analysis-0.2.1/idf_analysis/event_series_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    23398 2023-08-07 13:15:05.000000 idf-analysis-0.2.1/idf_analysis/heavy_rainfall_index.py
+-rw-r--r--   0 root         (0) root         (0)    12272 2023-08-07 13:15:05.000000 idf-analysis-0.2.1/idf_analysis/idf_backend.py
+-rw-r--r--   0 root         (0) root         (0)    34651 2023-08-07 13:15:05.000000 idf-analysis-0.2.1/idf_analysis/idf_class.py
+-rw-r--r--   0 root         (0) root         (0)     2546 2023-08-07 13:15:05.000000 idf-analysis-0.2.1/idf_analysis/in_out.py
+-rw-r--r--   0 root         (0) root         (0)     5113 2023-08-07 13:15:05.000000 idf-analysis-0.2.1/idf_analysis/interim_result_plots.py
+-rw-r--r--   0 root         (0) root         (0)     6906 2023-08-07 13:15:05.000000 idf-analysis-0.2.1/idf_analysis/little_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     3953 2023-08-07 13:15:05.000000 idf-analysis-0.2.1/idf_analysis/parameter_formulation_class.py
+-rw-r--r--   0 root         (0) root         (0)     3750 2023-08-07 13:15:05.000000 idf-analysis-0.2.1/idf_analysis/parameter_formulations.py
+-rw-r--r--   0 root         (0) root         (0)     3656 2023-08-07 13:15:05.000000 idf-analysis-0.2.1/idf_analysis/plot_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     6639 2023-08-07 13:15:05.000000 idf-analysis-0.2.1/idf_analysis/sww_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4988 2023-08-07 13:15:05.000000 idf-analysis-0.2.1/idf_analysis/synthetic_rainseries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:15:13.532529 idf-analysis-0.2.1/idf_analysis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14780 2023-08-07 13:15:13.000000 idf-analysis-0.2.1/idf_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      931 2023-08-07 13:15:13.000000 idf-analysis-0.2.1/idf_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 13:15:13.000000 idf-analysis-0.2.1/idf_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-08-07 13:15:13.000000 idf-analysis-0.2.1/idf_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      147 2023-08-07 13:15:13.000000 idf-analysis-0.2.1/idf_analysis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-07 13:15:13.000000 idf-analysis-0.2.1/idf_analysis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2440 2023-08-07 13:15:05.000000 idf-analysis-0.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 13:15:13.536529 idf-analysis-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 13:15:05.000000 idf-analysis-0.2.1/setup.py
```

### Comparing `idf-analysis-0.2.0/LICENSE` & `idf-analysis-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.0/PKG-INFO` & `idf-analysis-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idf-analysis
-Version: 0.2.0
+Version: 0.2.1
 Summary: heavy rain as a function of the duration and the return period acc. to DWA-A 531 (2012)
 Author-email: Markus Pichler <markus.pichler@tugraz.at>
 License: MIT
 Project-URL: Documentation, https://markuspic.github.io/intensity_duration_frequency_analysis/
 Project-URL: Changelog, https://github.com/MarkusPic/intensity_duration_frequency_analysis/-/blob/master/CHANGELOG.md
 Project-URL: homepage, https://github.com/MarkusPic/intensity_duration_frequency_analysis
 Keywords: duration,analysis,rainfall,dwd,idf,measurement-data,precipitation,kostra,dwa,heavy-rain,intensity-duration-frequency,design-rainfall,duration-steps,return-period,dwa-a-531
```

### Comparing `idf-analysis-0.2.0/README.md` & `idf-analysis-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.0/idf_analysis/__init__.py` & `idf-analysis-0.2.1/idf_analysis/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = "Markus Pichler"
 __credits__ = ["Markus Pichler"]
 __maintainer__ = "Markus Pichler"
 __email__ = "markus.pichler@tugraz.at"
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 __license__ = "MIT"
 
 from .idf_class import IntensityDurationFrequencyAnalyse, SERIES, METHOD
 
 """
 Heavy rain as a function of the duration and the return period acc. to DWA-A 531 (2012)
```

### Comparing `idf-analysis-0.2.0/idf_analysis/arg_parser.py` & `idf-analysis-0.2.1/idf_analysis/arg_parser.py`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.0/idf_analysis/definitions.py` & `idf-analysis-0.2.1/idf_analysis/definitions.py`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.0/idf_analysis/event_series_analysis.py` & `idf-analysis-0.2.1/idf_analysis/event_series_analysis.py`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.0/idf_analysis/heavy_rainfall_index.py` & `idf-analysis-0.2.1/idf_analysis/heavy_rainfall_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,15 +373,15 @@
         ax.legend(handles[::-1], labels[::-1], bbox_to_anchor=(1.02, 1.), loc='upper left',
                   borderaxespad=0., title='SRI')
 
         fig = ax.get_figure()
 
         # cm_to_inch = 2.54
         # fig.set_size_inches(h=11 / cm_to_inch, w=25 / cm_to_inch)  # (11.69, 8.27)
-        fig.tight_layout()
+        # fig.tight_layout()
         return fig, ax
 
     ####################################################################################################################
     @property
     def sri_frame(self):
         """
         get the return periods over the whole time-series for the default duration steps.
```

### Comparing `idf-analysis-0.2.0/idf_analysis/idf_backend.py` & `idf-analysis-0.2.1/idf_analysis/idf_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,16 @@
                     params_dur[p] = _Formulation.from_dict(params_dur[p])  # init object
 
                 if params_dur[p].a is None or params_dur[p].b is None or param_mean is not None:
                     params_dur[p].fit(dur, values_series, param_mean=param_mean, duration_mean=duration_mean)
 
         # ----------------------------
         # balance_parameter_change
-        if params_mean is None:
+        # TODO only between Not linear ranges
+        if params_mean is None and (len(self.parameters_final) > 1):
             print('_balance_parameter_change')
             # the balance between the different duration ranges acc. to DWA-A 531 chap. 5.2.4
             duration_step = list(self.parameters_final.keys())[1]
             durations = np.array([duration_step - 0.001, duration_step + 0.001])
 
             # if the interim results end here
```

### Comparing `idf-analysis-0.2.0/idf_analysis/idf_class.py` & `idf-analysis-0.2.1/idf_analysis/idf_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -665,32 +665,34 @@
                                            unit=unit, column_name=column_name)
 
             # -------------------------------------
             fig.get_axes()[0].set_title(caption + '\n\n\n')
 
             # DIN A4
             fig.set_size_inches(w=8.27, h=11.69)
-            fig.tight_layout()
+            # fig.tight_layout()
             pdf.savefig(fig)
             plt.close(fig)
 
         pdf.close()
 
     def event_plot(self, event, durations=None, unit='mm', column_name='Precipitation', min_return_period=1., german_caption=False, max_duration=None):
         import matplotlib.pyplot as plt
         if isinstance(event, pd.Series):
             event = event.to_dict()
 
         plot_range = slice(event[COL.START] - pd.Timedelta(self._freq), event[COL.END] + pd.Timedelta(self._freq))
 
+        return_periods_frame = self.return_periods_frame[plot_range]
         if COL.MAX_PERIOD not in event:
-            return_periods_frame = self.return_periods_frame[plot_range]
             event[COL.MAX_PERIOD] = return_periods_frame.max().max()
             event[COL.MAX_PERIOD_DURATION] = return_periods_frame.max().idxmax()
 
+        sum_frame_event = self.rainfall_sum_frame[plot_range]
+
         ts = self.series[plot_range].resample(self._freq).sum().fillna(0).copy()
 
         # -------------------------------------
         fig = plt.figure()
 
         if event[COL.MAX_PERIOD] < min_return_period:
             rain_ax = fig.add_subplot(111)
@@ -737,15 +739,15 @@
 
         for _, event in tqdm(main_events.to_dict(orient='index').items()):
             fig, ax = self.return_period_event_figure(event)
 
             # -------------------------------------
             # DIN A4
             fig.set_size_inches(h=11.69 / 2, w=8.27)
-            fig.tight_layout()
+            # fig.tight_layout()
             pdf.savefig(fig)
             plt.close(fig)
 
         pdf.close()
 
     def return_period_event_figure(self, event):
         import matplotlib.pyplot as plt
```

### Comparing `idf-analysis-0.2.0/idf_analysis/in_out.py` & `idf-analysis-0.2.1/idf_analysis/in_out.py`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.0/idf_analysis/interim_result_plots.py` & `idf-analysis-0.2.1/idf_analysis/interim_result_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     # -----------------
     l1 = ax.legend(custom_lines, ['< 60 min', '> 60 min'], loc='best', title='max Duration')
     ax.add_artist(l1)
 
     # -----------------
     # DIN A4
     fig.set_size_inches(w=7, h=5)
-    fig.tight_layout()
+    # fig.tight_layout()
     fig.savefig(filename)
     plt.close(fig)
 
 
 def result_plot_v2(idf: IntensityDurationFrequencyAnalyse, filename, min_duration=5.0, max_duration=720.0, logx=False, show=False):
     duration_steps = np.arange(min_duration, max_duration + 1, 1)
     colors = ['r', 'g', 'b', 'y', 'm']
@@ -132,13 +132,13 @@
     #                                                 return_periods[len(return_periods) - 1],
     #                                                 parameter_1, parameter_2) + 10])
 
     fig = ax.get_figure()
 
     cm_to_inch = 2.54
     fig.set_size_inches(h=21 / cm_to_inch, w=29.7 / cm_to_inch)  # (11.69, 8.27)
-    fig.tight_layout()
+    # fig.tight_layout()
     fig.savefig(filename, dpi=260)
     plt.close(fig)
     if show:
         show_file(filename)
     return filename
```

### Comparing `idf-analysis-0.2.0/idf_analysis/little_helpers.py` & `idf-analysis-0.2.1/idf_analysis/little_helpers.py`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.0/idf_analysis/parameter_formulation_class.py` & `idf-analysis-0.2.1/idf_analysis/parameter_formulation_class.py`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.0/idf_analysis/parameter_formulations.py` & `idf-analysis-0.2.1/idf_analysis/parameter_formulations.py`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.0/idf_analysis/plot_helpers.py` & `idf-analysis-0.2.1/idf_analysis/plot_helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -91,9 +91,12 @@
     ax.grid(axis='y', which='major')
 
     ax.set_ylim(0, duration_size)
     ax.set_xticklabels([])
     from matplotlib.ticker import NullFormatter
     ax.xaxis.set_major_formatter(NullFormatter())
     # ax.axhline(0, color='k')
-    ax.axhline(duration_size / 2, color='k')
+    # ax.axhline(duration_size / 2, color='k')
+    # TODO
+    # (k)urzzeitige Summationen, d. h. der Dauerstufen von 5 Minuten bis 2 Stunden
+    # (m)ittelfristige Summationen, d. h. der Dauerstufen von 3 Stunden bis 3 Tagen.
     return ax
```

### Comparing `idf-analysis-0.2.0/idf_analysis/sww_utils.py` & `idf-analysis-0.2.1/idf_analysis/sww_utils.py`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.0/idf_analysis/synthetic_rainseries.py` & `idf-analysis-0.2.1/idf_analysis/synthetic_rainseries.py`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.0/idf_analysis.egg-info/PKG-INFO` & `idf-analysis-0.2.1/idf_analysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idf-analysis
-Version: 0.2.0
+Version: 0.2.1
 Summary: heavy rain as a function of the duration and the return period acc. to DWA-A 531 (2012)
 Author-email: Markus Pichler <markus.pichler@tugraz.at>
 License: MIT
 Project-URL: Documentation, https://markuspic.github.io/intensity_duration_frequency_analysis/
 Project-URL: Changelog, https://github.com/MarkusPic/intensity_duration_frequency_analysis/-/blob/master/CHANGELOG.md
 Project-URL: homepage, https://github.com/MarkusPic/intensity_duration_frequency_analysis
 Keywords: duration,analysis,rainfall,dwd,idf,measurement-data,precipitation,kostra,dwa,heavy-rain,intensity-duration-frequency,design-rainfall,duration-steps,return-period,dwa-a-531
```

### Comparing `idf-analysis-0.2.0/idf_analysis.egg-info/SOURCES.txt` & `idf-analysis-0.2.1/idf_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.0/pyproject.toml` & `idf-analysis-0.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -35,34 +35,38 @@
     "pyarrow"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 docs = ["sphinx", "nbsphinx", "recommonmark", "pydata_sphinx_theme", "ipython==8.5.0"]
 
-[tool.setuptools.dynamic]
-version = { attr = "idf_analysis.__version__" }
-
 [project.urls]
 Documentation = "https://markuspic.github.io/intensity_duration_frequency_analysis/"
 Changelog = "https://github.com/MarkusPic/intensity_duration_frequency_analysis/-/blob/master/CHANGELOG.md"
 homepage = "https://github.com/MarkusPic/intensity_duration_frequency_analysis"
 
+[project.scripts]
+idf_analysis = "idf_analysis._console_script:command_line_tool"
+
+[tool.setuptools.dynamic]
+version = { attr = "idf_analysis.__version__" }
+
 [tool.setuptools.packages.find]
-include = ['idf_analysis']
+include = ["idf_analysis", "idf_analysis.approaches"]
 #namespaces = false
 
 [tool.setuptools.package-data]
-#mypkg = ["*.txt"]
 "idf_analysis.approaches" = ["*.yaml"]
 
-[project.scripts]
-idf_analysis = "idf_analysis._console_script:command_line_tool"
-
 # https://github.com/python-semantic-release/python-semantic-release
 [tool.semantic_release]
 branch = "main"
 version_variables = ["idf_analysis/__init__.py:__version__",]
 major_on_zero = false
-upload_to_pypi = true
-hvcs = 'github'
-version_source = 'tag'
+build_command = "pip install -q build && python -m build"
+# https://docs.github.com/en/actions/managing-workflow-runs/skipping-workflow-runs
+# [skip actions]
+commit_message = "{version}\n\nAutomatically generated by python-semantic-release\n\n[skip actions]"
+
+[tool.semantic_release.publish]
+dist_glob_patterns = ["dist/*"]
+upload_to_vcs_release = true
```

