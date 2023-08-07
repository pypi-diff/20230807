# Comparing `tmp/cybotrade-indicators-0.0.4.tar.gz` & `tmp/cybotrade-indicators-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybotrade-indicators-0.0.4.tar", last modified: Fri Aug  4 09:44:40 2023, max compression
+gzip compressed data, was "cybotrade-indicators-0.0.5.tar", last modified: Mon Aug  7 08:14:15 2023, max compression
```

## Comparing `cybotrade-indicators-0.0.4.tar` & `cybotrade-indicators-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-08-04 09:44:40.215543 cybotrade-indicators-0.0.4/
--rw-r--r--   0 marcus     (501) staff       (20)      433 2023-07-25 20:08:51.000000 cybotrade-indicators-0.0.4/AUTHORS
--rw-r--r--   0 marcus     (501) staff       (20)     7650 2023-07-25 20:08:38.000000 cybotrade-indicators-0.0.4/LICENSE
--rw-r--r--   0 marcus     (501) staff       (20)      238 2023-07-26 03:00:01.000000 cybotrade-indicators-0.0.4/MANIFEST.in
--rw-r--r--   0 marcus     (501) staff       (20)     3493 2023-08-04 09:44:40.215349 cybotrade-indicators-0.0.4/PKG-INFO
--rw-r--r--   0 marcus     (501) staff       (20)     2818 2023-07-25 20:06:26.000000 cybotrade-indicators-0.0.4/README.md
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-08-04 09:44:40.195197 cybotrade-indicators-0.0.4/external/
--rw-r--r--   0 marcus     (501) staff       (20)    53547 2023-07-25 10:32:29.000000 cybotrade-indicators-0.0.4/external/indicators.h
--rw-r--r--   0 marcus     (501) staff       (20)   419813 2023-08-04 09:22:41.000000 cybotrade-indicators-0.0.4/external/tiamalgamation.c
--rw-r--r--   0 marcus     (501) staff       (20)      920 2023-08-04 09:43:44.000000 cybotrade-indicators-0.0.4/pyproject.toml
--rw-r--r--   0 marcus     (501) staff       (20)       38 2023-08-04 09:44:40.215608 cybotrade-indicators-0.0.4/setup.cfg
--rw-r--r--   0 marcus     (501) staff       (20)      370 2023-07-25 19:18:28.000000 cybotrade-indicators-0.0.4/setup.py
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-08-04 09:44:40.190969 cybotrade-indicators-0.0.4/src/
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-08-04 09:44:40.213216 cybotrade-indicators-0.0.4/src/cybotrade_indicators/
--rw-r--r--   0 marcus     (501) staff       (20)  4146665 2023-08-04 09:35:32.000000 cybotrade-indicators-0.0.4/src/cybotrade_indicators/__init__.c
--rw-r--r--   0 marcus     (501) staff       (20)    24376 2023-07-25 19:55:33.000000 cybotrade-indicators-0.0.4/src/cybotrade_indicators/__init__.pyi
--rw-r--r--   0 marcus     (501) staff       (20)    56715 2023-07-25 19:55:33.000000 cybotrade-indicators-0.0.4/src/cybotrade_indicators/__init__.pyx
--rw-r--r--   0 marcus     (501) staff       (20)     1817 2023-07-25 19:17:58.000000 cybotrade-indicators-0.0.4/src/cybotrade_indicators/indicators.pxd
--rw-r--r--   0 marcus     (501) staff       (20)        0 2023-07-25 20:15:15.000000 cybotrade-indicators-0.0.4/src/cybotrade_indicators/py.typed
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-08-04 09:44:40.214475 cybotrade-indicators-0.0.4/src/cybotrade_indicators.egg-info/
--rw-r--r--   0 marcus     (501) staff       (20)     3493 2023-08-04 09:44:40.000000 cybotrade-indicators-0.0.4/src/cybotrade_indicators.egg-info/PKG-INFO
--rw-r--r--   0 marcus     (501) staff       (20)      548 2023-08-04 09:44:40.000000 cybotrade-indicators-0.0.4/src/cybotrade_indicators.egg-info/SOURCES.txt
--rw-r--r--   0 marcus     (501) staff       (20)        1 2023-08-04 09:44:40.000000 cybotrade-indicators-0.0.4/src/cybotrade_indicators.egg-info/dependency_links.txt
--rw-r--r--   0 marcus     (501) staff       (20)       30 2023-08-04 09:44:40.000000 cybotrade-indicators-0.0.4/src/cybotrade_indicators.egg-info/requires.txt
--rw-r--r--   0 marcus     (501) staff       (20)       21 2023-08-04 09:44:40.000000 cybotrade-indicators-0.0.4/src/cybotrade_indicators.egg-info/top_level.txt
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-08-04 09:44:40.214673 cybotrade-indicators-0.0.4/tests/
--rw-r--r--   0 marcus     (501) staff       (20)     2219 2023-07-25 19:35:10.000000 cybotrade-indicators-0.0.4/tests/test.py
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-08-07 08:14:15.365749 cybotrade-indicators-0.0.5/
+-rw-r--r--   0 marcus     (501) staff       (20)      433 2023-07-25 20:08:51.000000 cybotrade-indicators-0.0.5/AUTHORS
+-rw-r--r--   0 marcus     (501) staff       (20)     7650 2023-07-25 20:08:38.000000 cybotrade-indicators-0.0.5/LICENSE
+-rw-r--r--   0 marcus     (501) staff       (20)      238 2023-07-26 03:00:01.000000 cybotrade-indicators-0.0.5/MANIFEST.in
+-rw-r--r--   0 marcus     (501) staff       (20)     3493 2023-08-07 08:14:15.365611 cybotrade-indicators-0.0.5/PKG-INFO
+-rw-r--r--   0 marcus     (501) staff       (20)     2818 2023-07-25 20:06:26.000000 cybotrade-indicators-0.0.5/README.md
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-08-07 08:14:15.357283 cybotrade-indicators-0.0.5/external/
+-rw-r--r--   0 marcus     (501) staff       (20)    53547 2023-07-25 10:32:29.000000 cybotrade-indicators-0.0.5/external/indicators.h
+-rw-r--r--   0 marcus     (501) staff       (20)   418929 2023-08-07 08:03:01.000000 cybotrade-indicators-0.0.5/external/tiamalgamation.c
+-rw-r--r--   0 marcus     (501) staff       (20)      920 2023-08-07 08:06:24.000000 cybotrade-indicators-0.0.5/pyproject.toml
+-rw-r--r--   0 marcus     (501) staff       (20)       38 2023-08-07 08:14:15.365801 cybotrade-indicators-0.0.5/setup.cfg
+-rw-r--r--   0 marcus     (501) staff       (20)      370 2023-07-25 19:18:28.000000 cybotrade-indicators-0.0.5/setup.py
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-08-07 08:14:15.354897 cybotrade-indicators-0.0.5/src/
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-08-07 08:14:15.364156 cybotrade-indicators-0.0.5/src/cybotrade_indicators/
+-rw-r--r--   0 marcus     (501) staff       (20)  4149617 2023-08-07 07:59:19.000000 cybotrade-indicators-0.0.5/src/cybotrade_indicators/__init__.c
+-rw-r--r--   0 marcus     (501) staff       (20)    24376 2023-07-25 19:55:33.000000 cybotrade-indicators-0.0.5/src/cybotrade_indicators/__init__.pyi
+-rw-r--r--   0 marcus     (501) staff       (20)    56715 2023-07-25 19:55:33.000000 cybotrade-indicators-0.0.5/src/cybotrade_indicators/__init__.pyx
+-rw-r--r--   0 marcus     (501) staff       (20)     1817 2023-07-25 19:17:58.000000 cybotrade-indicators-0.0.5/src/cybotrade_indicators/indicators.pxd
+-rw-r--r--   0 marcus     (501) staff       (20)        0 2023-07-25 20:15:15.000000 cybotrade-indicators-0.0.5/src/cybotrade_indicators/py.typed
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-08-07 08:14:15.364799 cybotrade-indicators-0.0.5/src/cybotrade_indicators.egg-info/
+-rw-r--r--   0 marcus     (501) staff       (20)     3493 2023-08-07 08:14:15.000000 cybotrade-indicators-0.0.5/src/cybotrade_indicators.egg-info/PKG-INFO
+-rw-r--r--   0 marcus     (501) staff       (20)      548 2023-08-07 08:14:15.000000 cybotrade-indicators-0.0.5/src/cybotrade_indicators.egg-info/SOURCES.txt
+-rw-r--r--   0 marcus     (501) staff       (20)        1 2023-08-07 08:14:15.000000 cybotrade-indicators-0.0.5/src/cybotrade_indicators.egg-info/dependency_links.txt
+-rw-r--r--   0 marcus     (501) staff       (20)       30 2023-08-07 08:14:15.000000 cybotrade-indicators-0.0.5/src/cybotrade_indicators.egg-info/requires.txt
+-rw-r--r--   0 marcus     (501) staff       (20)       21 2023-08-07 08:14:15.000000 cybotrade-indicators-0.0.5/src/cybotrade_indicators.egg-info/top_level.txt
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-08-07 08:14:15.364925 cybotrade-indicators-0.0.5/tests/
+-rw-r--r--   0 marcus     (501) staff       (20)     2219 2023-07-25 19:35:10.000000 cybotrade-indicators-0.0.5/tests/test.py
```

### Comparing `cybotrade-indicators-0.0.4/LICENSE` & `cybotrade-indicators-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cybotrade-indicators-0.0.4/PKG-INFO` & `cybotrade-indicators-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybotrade-indicators
-Version: 0.0.4
+Version: 0.0.5
 Summary: This library provides a set of technical analysis indicators that can be used to craft trading strategies.
 Author-email: Marcus Lee <marcuslee@balaenaquant.com>, Lee Ze Lim <zelim@balaenaquant.com>
 Project-URL: Homepage, https://app.cybotrade.rs
 Project-URL: Documentation, https://docs.cybotrade.rs
 Project-URL: Repository, https://github.com/cybotrade/cybotrade-indicators
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cybotrade-indicators-0.0.4/README.md` & `cybotrade-indicators-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cybotrade-indicators-0.0.4/external/indicators.h` & `cybotrade-indicators-0.0.5/external/indicators.h`

 * *Files identical despite different names*

### Comparing `cybotrade-indicators-0.0.4/external/tiamalgamation.c` & `cybotrade-indicators-0.0.5/external/tiamalgamation.c`

 * *Files 1% similar despite different names*

```diff
@@ -31,29 +31,29 @@
 #ifndef __TI_INDICATORS_H__
 #define __TI_INDICATORS_H__
 
 
 /*
  *
  * Version 0.9.2
- * Header Build 1688954421
+ * Header Build 1691395352
  *
  */
 
 /*
  *
  * This file is generated. Do not modify directly.
  *
  */
 
 
 
 
 #define TI_VERSION "0.9.2"
-#define TI_BUILD 1688954421
+#define TI_BUILD 1691395352
 
 
 
 #ifndef TI_SKIP_SYSTEM_HEADERS
 #include <assert.h>
 #include <math.h>
 #include <stdlib.h>
@@ -128,17 +128,17 @@
 typedef struct ti_indicator_info {
   const char *name;
   const char *full_name;
   ti_indicator_start_function start;
   ti_indicator_function indicator;
   ti_indicator_function indicator_ref;
   int type, inputs, options, outputs;
-  const char *input_names[TI_MAXINDPARAMS + 1];
-  const char *option_names[TI_MAXINDPARAMS + 1];
-  const char *output_names[TI_MAXINDPARAMS + 1];
+  const char *input_names[TI_MAXINDPARAMS];
+  const char *option_names[TI_MAXINDPARAMS];
+  const char *output_names[TI_MAXINDPARAMS];
   ti_indicator_stream_new stream_new;
   ti_indicator_stream_run stream_run;
   ti_indicator_stream_free stream_free;
 } ti_indicator_info;
 
 /*Complete array of all indicators. Last element is 0,0,0,0...*/
 extern ti_indicator_info ti_indicators[];
@@ -1372,29 +1372,29 @@
 #define __TC_CANDLES_H__
 
 
 
 /*
  *
  * Version 0.9.2
- * Header Build 1688954421
+ * Header Build 1691395352
  *
  */
 
 /*
  *
  * This file is generated. Do not modify directly.
  *
  */
 
 
 
 
 #define TC_VERSION "0.9.2"
-#define TC_BUILD 1688954421
+#define TC_BUILD 1691395352
 
 
 
 
 #ifndef TI_SKIP_SYSTEM_HEADERS
 #include <stdint.h>
 #endif
@@ -6021,93 +6021,97 @@
   free(filter_ph_div_data);
   free(filter_pl_index);
   free(filter_pl_div_data);
   return TI_OKAY;
 }
 int ti_sin_start(TI_REAL const *options) { (void)options; return 0; } int ti_sin(int size, TI_REAL const *const *inputs, TI_REAL const *options, TI_REAL *const *outputs) { const TI_REAL *in1 = inputs[0]; (void)options; TI_REAL *output = outputs[0]; int i; for (i = 0; i < size; ++i) { output[i] = (sin(in1[i])); } return TI_OKAY; }
 int ti_sinh_start(TI_REAL const *options) { (void)options; return 0; } int ti_sinh(int size, TI_REAL const *const *inputs, TI_REAL const *options, TI_REAL *const *outputs) { const TI_REAL *in1 = inputs[0]; (void)options; TI_REAL *output = outputs[0]; int i; for (i = 0; i < size; ++i) { output[i] = (sinh(in1[i])); } return TI_OKAY; }
-int ti_sma_start(TI_REAL const *options) {
-    return (int)options[0]-1;
-}
-int ti_sma(int size, TI_REAL const *const *inputs, TI_REAL const *options, TI_REAL *const *outputs) {
-    const TI_REAL *input = inputs[0];
-    const int period = (int)options[0];
-    TI_REAL *output = outputs[0];
-    const TI_REAL scale = 1.0 / period;
-    if (period < 1) return TI_INVALID_OPTION;
-    if (size <= ti_sma_start(options)) return TI_OKAY;
-    TI_REAL sum = 0;
-    int i;
-    for (i = 0; i < period; ++i) {
-        sum += input[i];
-    }
-    *output++ = sum * scale;
-    for (i = period; i < size; ++i) {
-        sum += input[i];
-        sum -= input[i-period];
-        *output++ = sum * scale;
-    }
-    assert(output - outputs[0] == size - ti_sma_start(options));
+
+int ti_sma_start(TI_REAL const *options) { return (int)options[0] - 1; }
+int ti_sma(int size, TI_REAL const *const *inputs, TI_REAL const *options,
+           TI_REAL *const *outputs) {
+  const TI_REAL *input = inputs[0];
+  const int period = (int)options[0];
+  TI_REAL *output = outputs[0];
+  const TI_REAL scale = 1.0 / period;
+  if (period < 1)
+    return TI_INVALID_OPTION;
+  if (size <= ti_sma_start(options))
     return TI_OKAY;
+  TI_REAL sum = 0;
+  int i;
+  for (i = 0; i < period; ++i) {
+    sum += input[i];
+  }
+  *output++ = sum * scale;
+  for (i = period; i < size; ++i) {
+    sum += input[i];
+    sum -= input[i - period];
+    *output++ = sum * scale;
+  }
+  assert(output - outputs[0] == size - ti_sma_start(options));
+  return TI_OKAY;
 }
 typedef struct ti_stream_sma {
-    int index;
-    int progress;
-    int period;
-    TI_REAL per;
-    TI_REAL sum;
-    int buffer_idx;
-    TI_REAL buffer[];
+  int index;
+  int progress;
+  int period;
+  TI_REAL per;
+  TI_REAL sum;
+  int buffer_idx;
+  TI_REAL buffer[];
 } ti_stream_sma;
 int ti_sma_stream_new(TI_REAL const *options, ti_stream **stream_in) {
-    ti_stream_sma **stream = (ti_stream_sma**)stream_in;
-    int period = (int)options[0];
-    if (period < 1) return TI_INVALID_OPTION;
-    *stream = malloc(sizeof(ti_stream_sma) + sizeof(TI_REAL) * period);
-    if (!stream) {
-        return TI_OUT_OF_MEMORY;
-    }
-    (*stream)->index = TI_INDICATOR_SMA_INDEX;
-    (*stream)->progress = -ti_sma_start(options);
-    (*stream)->period = period;
-    (*stream)->per = 1. / period;
-    (*stream)->sum = 0.;
-    (*stream)->buffer_idx = -1;
-    return TI_OKAY;
-}
-int ti_sma_stream_run(ti_stream *stream_in, int size, TI_REAL const *const *inputs, TI_REAL *const *outputs) {
-    ti_stream_sma *stream = (ti_stream_sma*)stream_in;
-    int progress = stream->progress;
-    const TI_REAL *real = inputs[0];
-    int period = stream->period;
-    TI_REAL *sma = outputs[0];
-    TI_REAL per = stream->per;
-    TI_REAL sum = stream->sum;
-    int buffer_idx = stream->buffer_idx;
-    TI_REAL *buffer = stream->buffer;
-    if (progress == -period + 1) {} else {}
-    int i;
-    for (i = 0; progress < 1 && i < size; ++i, ++progress) {
-        { ++buffer_idx; sum += buffer[buffer_idx] = real[i] * per; };
-    }
-    if (i > 0 && progress == 1) {
-        *sma++ = sum;
-    }
-    for (; i < size; ++i, ++progress) {
-        { ++buffer_idx; if (buffer_idx == period) { buffer_idx = 0; } sum -= buffer[buffer_idx]; sum += buffer[buffer_idx] = real[i] * per; };
-        *sma++ = sum;
-    }
-    stream->progress = progress;
-    stream->sum = sum;
-    stream->buffer_idx = buffer_idx;
-    return TI_OKAY;
+  ti_stream_sma **stream = (ti_stream_sma **)stream_in;
+  int period = (int)options[0];
+  if (period < 1)
+    return TI_INVALID_OPTION;
+  *stream = malloc(sizeof(ti_stream_sma) + sizeof(TI_REAL) * period);
+  if (!stream) {
+    return TI_OUT_OF_MEMORY;
+  }
+  (*stream)->index = TI_INDICATOR_SMA_INDEX;
+  (*stream)->progress = -ti_sma_start(options);
+  (*stream)->period = period;
+  (*stream)->per = 1. / period;
+  (*stream)->sum = 0.;
+  (*stream)->buffer_idx = -1;
+  return TI_OKAY;
 }
-void ti_sma_stream_free(ti_stream *stream) {
-    free(stream);
+int ti_sma_stream_run(ti_stream *stream_in, int size,
+                      TI_REAL const *const *inputs, TI_REAL *const *outputs) {
+  ti_stream_sma *stream = (ti_stream_sma *)stream_in;
+  int progress = stream->progress;
+  const TI_REAL *real = inputs[0];
+  int period = stream->period;
+  TI_REAL *sma = outputs[0];
+  TI_REAL per = stream->per;
+  TI_REAL sum = stream->sum;
+  int buffer_idx = stream->buffer_idx;
+  TI_REAL *buffer = stream->buffer;
+  if (progress == -period + 1) {
+  } else {
+  }
+  int i;
+  for (i = 0; progress < 1 && i < size; ++i, ++progress) {
+    { ++buffer_idx; sum += buffer[buffer_idx] = real[i] * per; };
+  }
+  if (i > 0 && progress == 1) {
+    *sma++ = sum;
+  }
+  for (; i < size; ++i, ++progress) {
+    { ++buffer_idx; if (buffer_idx == period) { buffer_idx = 0; } sum -= buffer[buffer_idx]; sum += buffer[buffer_idx] = real[i] * per; };
+    *sma++ = sum;
+  }
+  stream->progress = progress;
+  stream->sum = sum;
+  stream->buffer_idx = buffer_idx;
+  return TI_OKAY;
 }
+void ti_sma_stream_free(ti_stream *stream) { free(stream); }
 int ti_sqrt_start(TI_REAL const *options) { (void)options; return 0; } int ti_sqrt(int size, TI_REAL const *const *inputs, TI_REAL const *options, TI_REAL *const *outputs) { const TI_REAL *in1 = inputs[0]; (void)options; TI_REAL *output = outputs[0]; int i; for (i = 0; i < size; ++i) { output[i] = (sqrt(in1[i])); } return TI_OKAY; }
 double max_value(double arr[], int n);
 double min_value(double arr[], int n);
 double not_zero(double x, double y);
 void slice_index(int const *const *inputs, int start_index, int end_index,
                  int input_size, int *const *outputs);
 void slice_array(double const *const *inputs, int start_index, int end_index,
@@ -8692,15 +8696,15 @@
 }
 void ti_buffer_free(ti_buffer *buffer) {
     free(buffer);
 }
 const char* ti_version(void) {return TI_VERSION;}
 long int ti_build(void) {return TI_BUILD;}
 int ti_indicator_count(void) {return TI_INDICATOR_COUNT;}
-struct ti_indicator_info ti_indicators[] = { {"abs", "Vector Absolute Value", ti_abs_start, ti_abs, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real",0}, {"",0}, {"abs",0}, 0, 0, 0}, {"acos", "Vector Arccosine", ti_acos_start, ti_acos, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real",0}, {"",0}, {"acos",0}, 0, 0, 0}, {"ad", "Accumulation/Distribution Line", ti_ad_start, ti_ad, 0, TI_TYPE_INDICATOR, 4, 0, 1, {"high","low","close","volume",0}, {"",0}, {"ad",0}, 0, 0, 0}, {"add", "Vector Addition", ti_add_start, ti_add, 0, TI_TYPE_SIMPLE, 2, 0, 1, {"value_one","value_two",0}, {"",0}, {"add",0}, 0, 0, 0}, {"adosc", "Accumulation/Distribution Oscillator", ti_adosc_start, ti_adosc, 0, TI_TYPE_INDICATOR, 4, 2, 1, {"high","low","close","volume",0}, {"short_period","long_period",0}, {"adosc",0}, 0, 0, 0}, {"adx", "Average Directional Movement Index", ti_adx_start, ti_adx, 0, TI_TYPE_INDICATOR, 2, 1, 1, {"high","low",0}, {"period[14]",0}, {"adx",0}, 0, 0, 0}, {"adxr", "Average Directional Movement Rating", ti_adxr_start, ti_adxr, 0, TI_TYPE_INDICATOR, 2, 1, 1, {"high","low",0}, {"period",0}, {"adxr",0}, 0, 0, 0}, {"andean_osc", "Andean Osc", ti_andean_osc_start, ti_andean_osc, 0, TI_TYPE_OVERLAY, 2, 2, 3, {"open","close",0}, {"period[50]","signal_length[9]",0}, {"?bull_data","?bear_data","ao_data",0}, 0, 0, 0}, {"ao", "Awesome Oscillator", ti_ao_start, ti_ao, 0, TI_TYPE_INDICATOR, 2, 0, 1, {"high","low",0}, {"",0}, {"ao",0}, 0, 0, 0}, {"apo", "Absolute Price Oscillator", ti_apo_start, ti_apo, 0, TI_TYPE_INDICATOR, 1, 2, 1, {"real",0}, {"short_period","long_period",0}, {"apo",0}, 0, 0, 0}, {"aroon", "Aroon", ti_aroon_start, ti_aroon, 0, TI_TYPE_INDICATOR, 2, 1, 2, {"high","low",0}, {"period",0}, {"aroon_down","aroon_up",0}, 0, 0, 0}, {"aroonosc", "Aroon Oscillator", ti_aroonosc_start, ti_aroonosc, 0, TI_TYPE_INDICATOR, 2, 1, 1, {"high","low",0}, {"period",0}, {"aroonosc",0}, 0, 0, 0}, {"asin", "Vector Arcsine", ti_asin_start, ti_asin, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real",0}, {"",0}, {"asin",0}, 0, 0, 0}, {"atan", "Vector Arctangent", ti_atan_start, ti_atan, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real",0}, {"",0}, {"atan",0}, 0, 0, 0}, {"atr", "Average True Range", ti_atr_start, ti_atr, ti_atr_ref, TI_TYPE_INDICATOR, 3, 1, 1, {"high","low","close",0}, {"period[14]",0}, {"atr",0}, ti_atr_stream_new, ti_atr_stream_run, ti_atr_stream_free}, {"avgprice", "Average Price", ti_avgprice_start, ti_avgprice, 0, TI_TYPE_OVERLAY, 4, 0, 1, {"open","high","low","close",0}, {"",0}, {"avgprice",0}, 0, 0, 0}, {"bbands", "Bollinger Bands", ti_bbands_start, ti_bbands, 0, TI_TYPE_OVERLAY, 1, 2, 3, {"real",0}, {"period[20]","stddev[2]",0}, {"bbands_lower(ohlcv)","bbands_middle(ohlcv)","bbands_upper(ohlcv)",0}, 0, 0, 0}, {"boom_pro", "Boom Pro", ti_boom_pro_start, ti_boom_pro, 0, TI_TYPE_OVERLAY, 1, 5, 2, {"close",0}, {"lp_period_one[6]","k1_quotient[0]","trig_no[2]","lp_period_two[27]","k22_eot[0.3]",0}, {"trigger(ohlc)","q4(ohlc)",0}, 0, 0, 0}, {"bop", "Balance of Power", ti_bop_start, ti_bop, 0, TI_TYPE_INDICATOR, 4, 0, 1, {"open","high","low","close",0}, {"",0}, {"bop",0}, 0, 0, 0}, {"braid_filter", "Braid Filter", ti_braid_filter_start, ti_braid_filter, 0, TI_TYPE_OVERLAY, 4, 4, 3, {"open","high","low","close",0}, {"ma01_length[3]","ma02_length[7]","ma03_length[14]","pips_min_sep_percent[40]",0}, {"?dif","?atr_filter","bar_color",0}, 0, 0, 0}, {"cci", "Commodity Channel Index", ti_cci_start, ti_cci, 0, TI_TYPE_INDICATOR, 3, 1, 1, {"high","low","close",0}, {"period[20]",0}, {"cci",0}, 0, 0, 0}, {"ceil", "Vector Ceiling", ti_ceil_start, ti_ceil, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real",0}, {"",0}, {"ceil",0}, 0, 0, 0}, {"chaikin_vol", "Chaikin Volatility", ti_chaikin_vol_start, ti_chaikin_vol, 0, TI_TYPE_OVERLAY, 2, 2, 1, {"high","low",0}, {"ema_period[7]","roc_period[14]",0}, {"cvi",0}, 0, 0, 0}, {"chandelier_exit", "Chandelier Exit", ti_chandelier_exit_start, ti_chandelier_exit, 0, TI_TYPE_OVERLAY, 3, 2, 1, {"high","low","close",0}, {"period[22]","atr_multiplier[3]",0}, {"buy_sell_signal",0}, 0, 0, 0}, {"cm_ema_trendbars", "CM EMA TRENDBARS", ti_cm_ema_trendbars_start, ti_cm_ema_trendbars, 0, TI_TYPE_OVERLAY, 3, 1, 2, {"high","low","close",0}, {"ema_length[34]",0}, {"?usdema(ohlc)","bar_color",0}, 0, 0, 0}, {"cmo", "Chande Momentum Oscillator", ti_cmo_start, ti_cmo, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real",0}, {"period",0}, {"cmo",0}, 0, 0, 0}, {"cos", "Vector Cosine", ti_cos_start, ti_cos, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real",0}, {"",0}, {"cos",0}, 0, 0, 0}, {"cosh", "Vector Hyperbolic Cosine", ti_cosh_start, ti_cosh, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real",0}, {"",0}, {"cosh",0}, 0, 0, 0}, {"crossany", "Crossany", ti_crossany_start, ti_crossany, 0, TI_TYPE_MATH, 2, 0, 1, {"value_one","value_two",0}, {"",0}, {"crossany",0}, 0, 0, 0}, {"crossover", "Crossover", ti_crossover_start, ti_crossover, 0, TI_TYPE_MATH, 2, 0, 1, {"value_one","value_two",0}, {"",0}, {"crossover",0}, 0, 0, 0}, {"cvi", "Chaikins Volatility", ti_cvi_start, ti_cvi, 0, TI_TYPE_INDICATOR, 2, 1, 1, {"high","low",0}, {"period",0}, {"cvi",0}, 0, 0, 0}, {"decay", "Linear Decay", ti_decay_start, ti_decay, 0, TI_TYPE_MATH, 1, 1, 1, {"real",0}, {"period",0}, {"decay",0}, 0, 0, 0}, {"dema", "Double Exponential Moving Average", ti_dema_start, ti_dema, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"real",0}, {"period[9]",0}, {"dema(ohlcv)",0}, 0, 0, 0}, {"di", "Directional Indicator", ti_di_start, ti_di, 0, TI_TYPE_INDICATOR, 3, 1, 2, {"high","low","close",0}, {"period",0}, {"plus_di","minus_di",0}, 0, 0, 0}, {"di_dx", "DI-DX", ti_di_dx_start, ti_di_dx, 0, TI_TYPE_INDICATOR, 3, 1, 3, {"high","low","close",0}, {"period[14]",0}, {"?dx","di_plus","di_minus",0}, 0, 0, 0}, {"div", "Vector Division", ti_div_start, ti_div, 0, TI_TYPE_SIMPLE, 2, 0, 1, {"value_one","value_two",0}, {"",0}, {"div",0}, 0, 0, 0}, {"dm", "Directional Movement", ti_dm_start, ti_dm, 0, TI_TYPE_INDICATOR, 2, 1, 2, {"high","low",0}, {"period",0}, {"plus_dm","minus_dm",0}, 0, 0, 0}, {"dpo", "Detrended Price Oscillator", ti_dpo_start, ti_dpo, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real",0}, {"period",0}, {"dpo",0}, 0, 0, 0}, {"dx", "Directional Movement Index", ti_dx_start, ti_dx, 0, TI_TYPE_INDICATOR, 2, 1, 1, {"high","low",0}, {"period[14]",0}, {"dx",0}, 0, 0, 0}, {"edecay", "Exponential Decay", ti_edecay_start, ti_edecay, 0, TI_TYPE_MATH, 1, 1, 1, {"real",0}, {"period",0}, {"edecay",0}, 0, 0, 0}, {"ema", "Exponential Moving Average", ti_ema_start, ti_ema, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"real",0}, {"period[9]",0}, {"ema(ohlcv)",0}, 0, 0, 0}, {"emv", "Ease of Movement", ti_emv_start, ti_emv, 0, TI_TYPE_INDICATOR, 3, 0, 1, {"high","low","volume",0}, {"",0}, {"emv",0}, 0, 0, 0}, {"exp", "Vector Exponential", ti_exp_start, ti_exp, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real",0}, {"",0}, {"exp",0}, 0, 0, 0}, {"floor", "Vector Floor", ti_floor_start, ti_floor, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real",0}, {"",0}, {"floor",0}, 0, 0, 0}, {"fosc", "Forecast Oscillator", ti_fosc_start, ti_fosc, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real",0}, {"period",0}, {"fosc",0}, 0, 0, 0}, {"ha", "Heikin-Ashi", ti_ha_start, ti_ha, 0, TI_TYPE_SIMPLE, 4, 0, 4, {"open","high","low","close",0}, {"",0}, {"ha_open","ha_high","ha_low","ha_close",0}, 0, 0, 0}, {"half_trend", "Half Trend", ti_half_trend_start, ti_half_trend, 0, TI_TYPE_OVERLAY, 3, 3, 2, {"high","low","close",0}, {"amplitude[2]","channel_deviation[2]","atr_length[100]",0}, {"?ht(ohlc)","bar_color",0}, 0, 0, 0}, {"heatmap_vol", "Heatmap Volume", ti_heatmap_vol_start, ti_heatmap_vol, 0, TI_TYPE_OVERLAY, 1, 6, 1, {"volume",0}, {"length[610]","std_length[610]","threshold_extra_high[4]","threshold_high[2.5]","threshold_medium[1]","threshold_normal[-0.5]",0}, {"heatmap_level",0}, 0, 0, 0}, {"hlc3", "HLC3", ti_hlc3_start, ti_hlc3, 0, TI_TYPE_MATH, 3, 0, 1, {"high","low","close",0}, {"",0}, {"hlc3_data",0}, 0, 0, 0}, {"hma", "Hull Moving Average", ti_hma_start, ti_hma, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"real",0}, {"period[9]",0}, {"hma(ohlcv)",0}, 0, 0, 0}, {"hull_suite", "Hull Suite", ti_hull_suite_start, ti_hull_suite, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"close",0}, {"hma_length[55]",0}, {"bar_color",0}, 0, 0, 0}, {"insidebar", "Inside Bar", ti_insidebar_start, ti_insidebar, 0, TI_TYPE_INDICATOR, 4, 0, 1, {"open","high","low","close",0}, {"",0}, {"buy_sell_signal",0}, 0, 0, 0}, {"kama", "Kaufman Adaptive Moving Average", ti_kama_start, ti_kama, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"real",0}, {"period",0}, {"kama",0}, 0, 0, 0}, {"kvo", "Klinger Volume Oscillator", ti_kvo_start, ti_kvo, 0, TI_TYPE_INDICATOR, 4, 2, 1, {"high","low","close","volume",0}, {"short_period","long_period",0}, {"kvo",0}, 0, 0, 0}, {"lag", "Lag", ti_lag_start, ti_lag, 0, TI_TYPE_MATH, 1, 1, 1, {"real",0}, {"period",0}, {"lag",0}, 0, 0, 0}, {"linreg", "Linear Regression", ti_linreg_start, ti_linreg, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"real",0}, {"period[100]",0}, {"linreg(ohlcv)",0}, 0, 0, 0}, {"linregintercept", "Linear Regression Intercept", ti_linregintercept_start, ti_linregintercept, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real",0}, {"period",0}, {"linregintercept",0}, 0, 0, 0}, {"linregslope", "Linear Regression Slope", ti_linregslope_start, ti_linregslope, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real",0}, {"period",0}, {"linregslope",0}, 0, 0, 0}, {"ln", "Vector Natural Log", ti_ln_start, ti_ln, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real",0}, {"",0}, {"ln",0}, 0, 0, 0}, {"log10", "Vector Base-10 Log", ti_log10_start, ti_log10, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real",0}, {"",0}, {"log10",0}, 0, 0, 0}, {"macd", "Moving Average Convergence/Divergence", ti_macd_start, ti_macd, 0, TI_TYPE_INDICATOR, 1, 3, 3, {"real",0}, {"short_period[12]","long_period[26]","signal_period[9]",0}, {"macd","macd_signal","?macd_histogram",0}, 0, 0, 0}, {"macd_fastline_divergence", "MACD Fastline Divergence", ti_macd_fastline_divergence_start, ti_macd_fastline_divergence, 0, TI_TYPE_OVERLAY, 3, 3, 2, {"high","low","close",0}, {"fast_length[12]","slow_length[26]","signal_length[9]",0}, {"bull","bear",0}, 0, 0, 0}, {"macd_hist_divergence", "MACD Hist Divergence", ti_macd_hist_divergence_start, ti_macd_hist_divergence, 0, TI_TYPE_OVERLAY, 3, 3, 2, {"high","low","close",0}, {"fast_length[12]","slow_length[26]","signal_length[9]",0}, {"bull","bear",0}, 0, 0, 0}, {"marketfi", "Market Facilitation Index", ti_marketfi_start, ti_marketfi, 0, TI_TYPE_INDICATOR, 3, 0, 1, {"high","low","volume",0}, {"",0}, {"marketfi",0}, 0, 0, 0}, {"mass", "Mass Index", ti_mass_start, ti_mass, 0, TI_TYPE_INDICATOR, 2, 1, 1, {"high","low",0}, {"period",0}, {"mass",0}, 0, 0, 0}, {"max", "Maximum In Period", ti_max_start, ti_max, ti_max_ref, TI_TYPE_MATH, 1, 1, 1, {"real",0}, {"period",0}, {"max",0}, 0, 0, 0}, {"md", "Mean Deviation Over Period", ti_md_start, ti_md, 0, TI_TYPE_MATH, 1, 1, 1, {"real",0}, {"period",0}, {"md",0}, 0, 0, 0}, {"medprice", "Median Price", ti_medprice_start, ti_medprice, 0, TI_TYPE_OVERLAY, 2, 0, 1, {"high","low",0}, {"",0}, {"medprice",0}, 0, 0, 0}, {"mfi", "Money Flow Index", ti_mfi_start, ti_mfi, 0, TI_TYPE_INDICATOR, 4, 1, 1, {"high","low","close","volume",0}, {"period[14]",0}, {"mfi",0}, 0, 0, 0}, {"min", "Minimum In Period", ti_min_start, ti_min, ti_min_ref, TI_TYPE_MATH, 1, 1, 1, {"real",0}, {"period",0}, {"min",0}, 0, 0, 0}, {"mobo_band", "Mobo Band", ti_mobo_band_start, ti_mobo_band, 0, TI_TYPE_OVERLAY, 2, 4, 1, {"high","low",0}, {"dpo_length[13]","mobo_length[10]","num_dev_down[-0.8]","num_dev_up[0.8]",0}, {"buy_sell_signal",0}, 0, 0, 0}, {"mom", "Momentum", ti_mom_start, ti_mom, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real",0}, {"period",0}, {"mom",0}, 0, 0, 0}, {"mul", "Vector Multiplication", ti_mul_start, ti_mul, 0, TI_TYPE_SIMPLE, 2, 0, 1, {"value_one","value_two",0}, {"",0}, {"mul",0}, 0, 0, 0}, {"natr", "Normalized Average True Range", ti_natr_start, ti_natr, 0, TI_TYPE_INDICATOR, 3, 1, 1, {"high","low","close",0}, {"period[14]",0}, {"natr",0}, 0, 0, 0}, {"price", "Compare Price", ti_price_start, ti_price, 0, TI_TYPE_INDICATOR, 1, 0, 1, {"value(ohlc)",0}, {"",0}, {"price",0}, 0, 0, 0}, {"psar", "PSAR", ti_psar_start, ti_psar, 0, TI_TYPE_INDICATOR, 3, 3, 1, {"high","low","close",0}, {"accel_start[0.02]","accel_step[0.02]","accel_max[0.2]",0}, {"psar(ohlc)",0}, 0, 0, 0}, {"qqe_mod", "QQE Mod", ti_qqe_mod_start, ti_qqe_mod, 0, TI_TYPE_OVERLAY, 1, 10, 2, {"close",0}, {"rsi_length_one[6]","rsi_smoothing_one[5]","qqe_factor_one[3]","threshold_one[3]","rsi_length_two[6]","rsi_smoothing_two[5]","qqe_factor_two[1.61]","threshold_two[3]","bollinger_length[50]","qqe_multiplier[0.35]",0}, {"bar_color_one","bar_color_two",0}, 0, 0, 0}, {"roc", "Rate of Change", ti_roc_start, ti_roc, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real",0}, {"period",0}, {"roc",0}, 0, 0, 0}, {"rocr", "Rate of Change Ratio", ti_rocr_start, ti_rocr, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real",0}, {"period",0}, {"rocr",0}, 0, 0, 0}, {"round", "Vector Round", ti_round_start, ti_round, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real",0}, {"",0}, {"round",0}, 0, 0, 0}, {"rsi", "Relative Strength Index", ti_rsi_start, ti_rsi, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real",0}, {"period[14]",0}, {"rsi",0}, 0, 0, 0}, {"rsi_divergence", "Relative Strength Index Divergence", ti_rsi_divergence_start, ti_rsi_divergence, 0, TI_TYPE_OVERLAY, 3, 3, 2, {"high","low","close",0}, {"left_bar[6]","right_bar[2]","rsi_length[14]",0}, {"bull","bear",0}, 0, 0, 0}, {"rvi", "Relative Volatility Index", ti_rvi_start, ti_rvi, 0, TI_TYPE_OVERLAY, 1, 2, 1, {"close",0}, {"std_length[10]","ema_length[14]",0}, {"rvi",0}, 0, 0, 0}, {"rvi_divergence", "Relative Volatility Index Divergence", ti_rvi_divergence_start, ti_rvi_divergence, 0, TI_TYPE_OVERLAY, 3, 4, 2, {"high","low","close",0}, {"left_bar[6]","right_bar[2]","std_length[12]","ema_length[14]",0}, {"bull","bear",0}, 0, 0, 0}, {"sin", "Vector Sine", ti_sin_start, ti_sin, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real",0}, {"",0}, {"sin",0}, 0, 0, 0}, {"sinh", "Vector Hyperbolic Sine", ti_sinh_start, ti_sinh, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real",0}, {"",0}, {"sinh",0}, 0, 0, 0}, {"sma", "Simple Moving Average", ti_sma_start, ti_sma, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"real",0}, {"period[7]",0}, {"sma(ohlcv)",0}, ti_sma_stream_new, ti_sma_stream_run, ti_sma_stream_free}, {"sqrt", "Vector Square Root", ti_sqrt_start, ti_sqrt, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real",0}, {"",0}, {"sqrt",0}, 0, 0, 0}, {"ssl", "SSL", ti_ssl_start, ti_ssl, 0, TI_TYPE_OVERLAY, 3, 2, 6, {"high","low","close",0}, {"ma_length[60]","ssl3_length[15]",0}, {"?bbmc(ohlc)","bar_color","?up_erk(ohlc)","?low_erk(ohlc)","?cross_long","?cross_short",0}, 0, 0, 0}, {"stc", "STC", ti_stc_start, ti_stc, 0, TI_TYPE_OVERLAY, 1, 4, 2, {"close",0}, {"length[12]","fast_length[26]","slow_length[50]","aaa[0.5]",0}, {"?stc","bar_color",0}, 0, 0, 0}, {"stddev", "Standard Deviation Over Period", ti_stddev_start, ti_stddev, 0, TI_TYPE_MATH, 1, 1, 1, {"real",0}, {"period",0}, {"stddev",0}, 0, 0, 0}, {"stderr", "Standard Error Over Period", ti_stderr_start, ti_stderr, 0, TI_TYPE_MATH, 1, 1, 1, {"real",0}, {"period",0}, {"stderr",0}, 0, 0, 0}, {"stoch", "Stochastic Oscillator", ti_stoch_start, ti_stoch, 0, TI_TYPE_INDICATOR, 3, 3, 2, {"high","low","close",0}, {"k_period[14]","k_slowing_period[1]","d_period[3]",0}, {"stoch_k","stoch_d",0}, 0, 0, 0}, {"stoch_divergence", "Stochastic Divergence", ti_stoch_divergence_start, ti_stoch_divergence, 0, TI_TYPE_OVERLAY, 3, 5, 2, {"high","low","close",0}, {"left_bar[6]","right_bar[2]","stk_length[14]","smooth_length[3]","sma_length[3]",0}, {"bull","bear",0}, 0, 0, 0}, {"stoch_rsi", "Stoch Rsi", ti_stoch_rsi_start, ti_stoch_rsi, 0, TI_TYPE_OVERLAY, 1, 4, 2, {"close",0}, {"smoothk[3]","smoothd[3]","rsi_period[14]","stoch_period[14]",0}, {"stoch_k","stoch_d",0}, 0, 0, 0}, {"stochrsi", "Stochastic RSI", ti_stochrsi_start, ti_stochrsi, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real",0}, {"period[14]",0}, {"stochrsi",0}, 0, 0, 0}, {"sub", "Vector Subtraction", ti_sub_start, ti_sub, 0, TI_TYPE_SIMPLE, 2, 0, 1, {"value_one","value_two",0}, {"",0}, {"sub",0}, 0, 0, 0}, {"sum", "Sum Over Period", ti_sum_start, ti_sum, 0, TI_TYPE_MATH, 1, 1, 1, {"real",0}, {"period",0}, {"sum",0}, 0, 0, 0}, {"sup_and_res", "Support and Resistance", ti_sup_and_res_start, ti_sup_and_res, 0, TI_TYPE_OVERLAY, 1, 4, 16, {"close",0}, {"left_bar[200]","right_bar_one[20]","right_bar_two[5]","hma_length[9]",0}, {"buy_one","buy_two","buy_three","buy_four","buy_five","buy_six","buy_seven","buy_eight","sell_one","sell_two","sell_three","sell_four","sell_five","sell_six","sell_seven","sell_eight",0}, 0, 0, 0}, {"supertrend", "Supertrend", ti_supertrend_start, ti_supertrend, 0, TI_TYPE_OVERLAY, 3, 2, 4, {"high","low","close",0}, {"period[34]","factor[3]",0}, {"?supertrend(ohlc)","?direction","bar_color","buy_sell_signal",0}, 0, 0, 0}, {"tan", "Vector Tangent", ti_tan_start, ti_tan, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real",0}, {"",0}, {"tan",0}, 0, 0, 0}, {"tanh", "Vector Hyperbolic Tangent", ti_tanh_start, ti_tanh, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real",0}, {"",0}, {"tanh",0}, 0, 0, 0}, {"tema", "Triple Exponential Moving Average", ti_tema_start, ti_tema, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"real",0}, {"period[9]",0}, {"tema(ohlcv)",0}, 0, 0, 0}, {"todeg", "Vector Degree Conversion", ti_todeg_start, ti_todeg, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real",0}, {"",0}, {"degrees",0}, 0, 0, 0}, {"torad", "Vector Radian Conversion", ti_torad_start, ti_torad, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real",0}, {"",0}, {"radians",0}, 0, 0, 0}, {"tr", "True Range", ti_tr_start, ti_tr, 0, TI_TYPE_INDICATOR, 3, 0, 1, {"high","low","close",0}, {"",0}, {"tr",0}, 0, 0, 0}, {"trima", "Triangular Moving Average", ti_trima_start, ti_trima, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"real",0}, {"period[20]",0}, {"trima(ohlcv)",0}, 0, 0, 0}, {"trix", "Trix", ti_trix_start, ti_trix, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real",0}, {"period",0}, {"trix",0}, 0, 0, 0}, {"trunc", "Vector Truncate", ti_trunc_start, ti_trunc, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real",0}, {"",0}, {"trunc",0}, 0, 0, 0}, {"tsf", "Time Series Forecast", ti_tsf_start, ti_tsf, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"real",0}, {"period",0}, {"tsf",0}, 0, 0, 0}, {"typprice", "Typical Price", ti_typprice_start, ti_typprice, 0, TI_TYPE_OVERLAY, 3, 0, 1, {"high","low","close",0}, {"",0}, {"typprice",0}, 0, 0, 0}, {"ultosc", "Ultimate Oscillator", ti_ultosc_start, ti_ultosc, 0, TI_TYPE_INDICATOR, 3, 3, 1, {"high","low","close",0}, {"short_period","medium_period","long_period",0}, {"ultosc",0}, 0, 0, 0}, {"unshift", "Unshift", ti_unshift_start, ti_unshift, 0, TI_TYPE_SIMPLE, 1, 2, 1, {"value",0}, {"default_value","length",0}, {"unshifted_value",0}, 0, 0, 0}, {"ut_bot", "UT Bot Alert", ti_ut_bot_start, ti_ut_bot, 0, TI_TYPE_OVERLAY, 3, 2, 1, {"high","low","close",0}, {"atr_period[10]","sensitivity[1]",0}, {"buy_sell_signal",0}, 0, 0, 0}, {"var", "Variance Over Period", ti_var_start, ti_var, 0, TI_TYPE_MATH, 1, 1, 1, {"real",0}, {"period",0}, {"var",0}, 0, 0, 0}, {"vhf", "Vertical Horizontal Filter", ti_vhf_start, ti_vhf, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real",0}, {"period",0}, {"vhf",0}, 0, 0, 0}, {"volatility", "Annualized Historical Volatility", ti_volatility_start, ti_volatility, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real",0}, {"period",0}, {"volatility",0}, 0, 0, 0}, {"volatility_oscillator", "Volatility Oscillator", ti_volatility_oscillator_start, ti_volatility_oscillator, 0, TI_TYPE_OVERLAY, 2, 1, 3, {"open","close",0}, {"length[100]",0}, {"spike_line","upper_line","lower_line",0}, 0, 0, 0}, {"vosc", "Volume Oscillator", ti_vosc_start, ti_vosc, 0, TI_TYPE_INDICATOR, 1, 2, 1, {"volume",0}, {"short_period","long_period",0}, {"vosc",0}, 0, 0, 0}, {"vu_man_chu_swing", "VU Man Chu Swing", ti_vu_man_chu_swing_start, ti_vu_man_chu_swing, 0, TI_TYPE_OVERLAY, 1, 2, 2, {"close",0}, {"swing_period[20]","swing_multiplier[3.5]",0}, {"buy_sell_signal_long","buy_sell_signal_short",0}, 0, 0, 0}, {"vwma", "Volume Weighted Moving Average", ti_vwma_start, ti_vwma, 0, TI_TYPE_OVERLAY, 2, 1, 1, {"close","volume",0}, {"period[20]",0}, {"vwma(v)",0}, 0, 0, 0}, {"wad", "Williams Accumulation/Distribution", ti_wad_start, ti_wad, 0, TI_TYPE_INDICATOR, 3, 0, 1, {"high","low","close",0}, {"",0}, {"wad",0}, 0, 0, 0}, {"waddah", "Waddah", ti_waddah_start, ti_waddah, 0, TI_TYPE_OVERLAY, 1, 6, 4, {"close",0}, {"fast_length[20]","slow_length[40]","signal_length[9]","bb_length[20]","multiplier[2]","sensitivity[150]",0}, {"?t","e","trend_up","trend_down",0}, 0, 0, 0}, {"wavetrend", "Wavetrend", ti_wavetrend_start, ti_wavetrend, 0, TI_TYPE_OVERLAY, 3, 2, 2, {"high","low","close",0}, {"period_one[9]","period_two[12]",0}, {"wavetrend_one","wavetrend_two",0}, 0, 0, 0}, {"wcprice", "Weighted Close Price", ti_wcprice_start, ti_wcprice, 0, TI_TYPE_OVERLAY, 3, 0, 1, {"high","low","close",0}, {"",0}, {"wcprice",0}, 0, 0, 0}, {"wilders", "Wilders Smoothing", ti_wilders_start, ti_wilders, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"real",0}, {"period",0}, {"wilders",0}, 0, 0, 0}, {"willr", "Williams %R", ti_willr_start, ti_willr, 0, TI_TYPE_INDICATOR, 3, 1, 1, {"high","low","close",0}, {"period",0}, {"willr",0}, 0, 0, 0}, {"wma", "Weighted Moving Average", ti_wma_start, ti_wma, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"real",0}, {"period[9]",0}, {"wma(ohlcv)",0}, 0, 0, 0}, {"zlema", "Zero-Lag Exponential Moving Average", ti_zlema_start, ti_zlema, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"real",0}, {"period",0}, {"zlema(ohlcv)",0}, 0, 0, 0}, {0,0,0,0,0,0,0,0,0,{0,0},{0,0},{0,0},0,0,0}};
+struct ti_indicator_info ti_indicators[] = { {"abs", "Vector Absolute Value", ti_abs_start, ti_abs, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real"}, {""}, {"abs"}, 0, 0, 0}, {"acos", "Vector Arccosine", ti_acos_start, ti_acos, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real"}, {""}, {"acos"}, 0, 0, 0}, {"ad", "Accumulation/Distribution Line", ti_ad_start, ti_ad, 0, TI_TYPE_INDICATOR, 4, 0, 1, {"high","low","close","volume"}, {""}, {"ad"}, 0, 0, 0}, {"add", "Vector Addition", ti_add_start, ti_add, 0, TI_TYPE_SIMPLE, 2, 0, 1, {"value_one","value_two"}, {""}, {"add"}, 0, 0, 0}, {"adosc", "Accumulation/Distribution Oscillator", ti_adosc_start, ti_adosc, 0, TI_TYPE_INDICATOR, 4, 2, 1, {"high","low","close","volume"}, {"short_period","long_period"}, {"adosc"}, 0, 0, 0}, {"adx", "Average Directional Movement Index", ti_adx_start, ti_adx, 0, TI_TYPE_INDICATOR, 2, 1, 1, {"high","low"}, {"period[14]"}, {"adx"}, 0, 0, 0}, {"adxr", "Average Directional Movement Rating", ti_adxr_start, ti_adxr, 0, TI_TYPE_INDICATOR, 2, 1, 1, {"high","low"}, {"period"}, {"adxr"}, 0, 0, 0}, {"andean_osc", "Andean Osc", ti_andean_osc_start, ti_andean_osc, 0, TI_TYPE_OVERLAY, 2, 2, 3, {"open","close"}, {"period[50]","signal_length[9]"}, {"?bull_data","?bear_data","ao_data"}, 0, 0, 0}, {"ao", "Awesome Oscillator", ti_ao_start, ti_ao, 0, TI_TYPE_INDICATOR, 2, 0, 1, {"high","low"}, {""}, {"ao"}, 0, 0, 0}, {"apo", "Absolute Price Oscillator", ti_apo_start, ti_apo, 0, TI_TYPE_INDICATOR, 1, 2, 1, {"real"}, {"short_period","long_period"}, {"apo"}, 0, 0, 0}, {"aroon", "Aroon", ti_aroon_start, ti_aroon, 0, TI_TYPE_INDICATOR, 2, 1, 2, {"high","low"}, {"period"}, {"aroon_down","aroon_up"}, 0, 0, 0}, {"aroonosc", "Aroon Oscillator", ti_aroonosc_start, ti_aroonosc, 0, TI_TYPE_INDICATOR, 2, 1, 1, {"high","low"}, {"period"}, {"aroonosc"}, 0, 0, 0}, {"asin", "Vector Arcsine", ti_asin_start, ti_asin, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real"}, {""}, {"asin"}, 0, 0, 0}, {"atan", "Vector Arctangent", ti_atan_start, ti_atan, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real"}, {""}, {"atan"}, 0, 0, 0}, {"atr", "Average True Range", ti_atr_start, ti_atr, ti_atr_ref, TI_TYPE_INDICATOR, 3, 1, 1, {"high","low","close"}, {"period[14]"}, {"atr"}, ti_atr_stream_new, ti_atr_stream_run, ti_atr_stream_free}, {"avgprice", "Average Price", ti_avgprice_start, ti_avgprice, 0, TI_TYPE_OVERLAY, 4, 0, 1, {"open","high","low","close"}, {""}, {"avgprice"}, 0, 0, 0}, {"bbands", "Bollinger Bands", ti_bbands_start, ti_bbands, 0, TI_TYPE_OVERLAY, 1, 2, 3, {"real"}, {"period[20]","stddev[2]"}, {"bbands_lower(ohlcv)","bbands_middle(ohlcv)","bbands_upper(ohlcv)"}, 0, 0, 0}, {"boom_pro", "Boom Pro", ti_boom_pro_start, ti_boom_pro, 0, TI_TYPE_OVERLAY, 1, 5, 2, {"close"}, {"lp_period_one[6]","k1_quotient[0]","trig_no[2]","lp_period_two[27]","k22_eot[0.3]"}, {"trigger(ohlc)","q4(ohlc)"}, 0, 0, 0}, {"bop", "Balance of Power", ti_bop_start, ti_bop, 0, TI_TYPE_INDICATOR, 4, 0, 1, {"open","high","low","close"}, {""}, {"bop"}, 0, 0, 0}, {"braid_filter", "Braid Filter", ti_braid_filter_start, ti_braid_filter, 0, TI_TYPE_OVERLAY, 4, 4, 3, {"open","high","low","close"}, {"ma01_length[3]","ma02_length[7]","ma03_length[14]","pips_min_sep_percent[40]"}, {"?dif","?atr_filter","bar_color"}, 0, 0, 0}, {"cci", "Commodity Channel Index", ti_cci_start, ti_cci, 0, TI_TYPE_INDICATOR, 3, 1, 1, {"high","low","close"}, {"period[20]"}, {"cci"}, 0, 0, 0}, {"ceil", "Vector Ceiling", ti_ceil_start, ti_ceil, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real"}, {""}, {"ceil"}, 0, 0, 0}, {"chaikin_vol", "Chaikin Volatility", ti_chaikin_vol_start, ti_chaikin_vol, 0, TI_TYPE_OVERLAY, 2, 2, 1, {"high","low"}, {"ema_period[7]","roc_period[14]"}, {"cvi"}, 0, 0, 0}, {"chandelier_exit", "Chandelier Exit", ti_chandelier_exit_start, ti_chandelier_exit, 0, TI_TYPE_OVERLAY, 3, 2, 1, {"high","low","close"}, {"period[22]","atr_multiplier[3]"}, {"buy_sell_signal"}, 0, 0, 0}, {"cm_ema_trendbars", "CM EMA TRENDBARS", ti_cm_ema_trendbars_start, ti_cm_ema_trendbars, 0, TI_TYPE_OVERLAY, 3, 1, 2, {"high","low","close"}, {"ema_length[34]"}, {"?usdema(ohlc)","bar_color"}, 0, 0, 0}, {"cmo", "Chande Momentum Oscillator", ti_cmo_start, ti_cmo, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real"}, {"period"}, {"cmo"}, 0, 0, 0}, {"cos", "Vector Cosine", ti_cos_start, ti_cos, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real"}, {""}, {"cos"}, 0, 0, 0}, {"cosh", "Vector Hyperbolic Cosine", ti_cosh_start, ti_cosh, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real"}, {""}, {"cosh"}, 0, 0, 0}, {"crossany", "Crossany", ti_crossany_start, ti_crossany, 0, TI_TYPE_MATH, 2, 0, 1, {"value_one","value_two"}, {""}, {"crossany"}, 0, 0, 0}, {"crossover", "Crossover", ti_crossover_start, ti_crossover, 0, TI_TYPE_MATH, 2, 0, 1, {"value_one","value_two"}, {""}, {"crossover"}, 0, 0, 0}, {"cvi", "Chaikins Volatility", ti_cvi_start, ti_cvi, 0, TI_TYPE_INDICATOR, 2, 1, 1, {"high","low"}, {"period"}, {"cvi"}, 0, 0, 0}, {"decay", "Linear Decay", ti_decay_start, ti_decay, 0, TI_TYPE_MATH, 1, 1, 1, {"real"}, {"period"}, {"decay"}, 0, 0, 0}, {"dema", "Double Exponential Moving Average", ti_dema_start, ti_dema, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"real"}, {"period[9]"}, {"dema(ohlcv)"}, 0, 0, 0}, {"di", "Directional Indicator", ti_di_start, ti_di, 0, TI_TYPE_INDICATOR, 3, 1, 2, {"high","low","close"}, {"period"}, {"plus_di","minus_di"}, 0, 0, 0}, {"di_dx", "DI-DX", ti_di_dx_start, ti_di_dx, 0, TI_TYPE_INDICATOR, 3, 1, 3, {"high","low","close"}, {"period[14]"}, {"?dx","di_plus","di_minus"}, 0, 0, 0}, {"div", "Vector Division", ti_div_start, ti_div, 0, TI_TYPE_SIMPLE, 2, 0, 1, {"value_one","value_two"}, {""}, {"div"}, 0, 0, 0}, {"dm", "Directional Movement", ti_dm_start, ti_dm, 0, TI_TYPE_INDICATOR, 2, 1, 2, {"high","low"}, {"period"}, {"plus_dm","minus_dm"}, 0, 0, 0}, {"dpo", "Detrended Price Oscillator", ti_dpo_start, ti_dpo, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real"}, {"period"}, {"dpo"}, 0, 0, 0}, {"dx", "Directional Movement Index", ti_dx_start, ti_dx, 0, TI_TYPE_INDICATOR, 2, 1, 1, {"high","low"}, {"period[14]"}, {"dx"}, 0, 0, 0}, {"edecay", "Exponential Decay", ti_edecay_start, ti_edecay, 0, TI_TYPE_MATH, 1, 1, 1, {"real"}, {"period"}, {"edecay"}, 0, 0, 0}, {"ema", "Exponential Moving Average", ti_ema_start, ti_ema, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"real"}, {"period[9]"}, {"ema(ohlcv)"}, 0, 0, 0}, {"emv", "Ease of Movement", ti_emv_start, ti_emv, 0, TI_TYPE_INDICATOR, 3, 0, 1, {"high","low","volume"}, {""}, {"emv"}, 0, 0, 0}, {"exp", "Vector Exponential", ti_exp_start, ti_exp, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real"}, {""}, {"exp"}, 0, 0, 0}, {"floor", "Vector Floor", ti_floor_start, ti_floor, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real"}, {""}, {"floor"}, 0, 0, 0}, {"fosc", "Forecast Oscillator", ti_fosc_start, ti_fosc, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real"}, {"period"}, {"fosc"}, 0, 0, 0}, {"ha", "Heikin-Ashi", ti_ha_start, ti_ha, 0, TI_TYPE_SIMPLE, 4, 0, 4, {"open","high","low","close"}, {""}, {"ha_open","ha_high","ha_low","ha_close"}, 0, 0, 0}, {"half_trend", "Half Trend", ti_half_trend_start, ti_half_trend, 0, TI_TYPE_OVERLAY, 3, 3, 2, {"high","low","close"}, {"amplitude[2]","channel_deviation[2]","atr_length[100]"}, {"?ht(ohlc)","bar_color"}, 0, 0, 0}, {"heatmap_vol", "Heatmap Volume", ti_heatmap_vol_start, ti_heatmap_vol, 0, TI_TYPE_OVERLAY, 1, 6, 1, {"volume"}, {"length[610]","std_length[610]","threshold_extra_high[4]","threshold_high[2.5]","threshold_medium[1]","threshold_normal[-0.5]"}, {"heatmap_level"}, 0, 0, 0}, {"hlc3", "HLC3", ti_hlc3_start, ti_hlc3, 0, TI_TYPE_MATH, 3, 0, 1, {"high","low","close"}, {""}, {"hlc3_data"}, 0, 0, 0}, {"hma", "Hull Moving Average", ti_hma_start, ti_hma, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"real"}, {"period[9]"}, {"hma(ohlcv)"}, 0, 0, 0}, {"hull_suite", "Hull Suite", ti_hull_suite_start, ti_hull_suite, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"close"}, {"hma_length[55]"}, {"bar_color"}, 0, 0, 0}, {"insidebar", "Inside Bar", ti_insidebar_start, ti_insidebar, 0, TI_TYPE_INDICATOR, 4, 0, 1, {"open","high","low","close"}, {""}, {"buy_sell_signal"}, 0, 0, 0}, {"kama", "Kaufman Adaptive Moving Average", ti_kama_start, ti_kama, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"real"}, {"period"}, {"kama"}, 0, 0, 0}, {"kvo", "Klinger Volume Oscillator", ti_kvo_start, ti_kvo, 0, TI_TYPE_INDICATOR, 4, 2, 1, {"high","low","close","volume"}, {"short_period","long_period"}, {"kvo"}, 0, 0, 0}, {"lag", "Lag", ti_lag_start, ti_lag, 0, TI_TYPE_MATH, 1, 1, 1, {"real"}, {"period"}, {"lag"}, 0, 0, 0}, {"linreg", "Linear Regression", ti_linreg_start, ti_linreg, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"real"}, {"period[100]"}, {"linreg(ohlcv)"}, 0, 0, 0}, {"linregintercept", "Linear Regression Intercept", ti_linregintercept_start, ti_linregintercept, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real"}, {"period"}, {"linregintercept"}, 0, 0, 0}, {"linregslope", "Linear Regression Slope", ti_linregslope_start, ti_linregslope, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real"}, {"period"}, {"linregslope"}, 0, 0, 0}, {"ln", "Vector Natural Log", ti_ln_start, ti_ln, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real"}, {""}, {"ln"}, 0, 0, 0}, {"log10", "Vector Base-10 Log", ti_log10_start, ti_log10, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real"}, {""}, {"log10"}, 0, 0, 0}, {"macd", "Moving Average Convergence/Divergence", ti_macd_start, ti_macd, 0, TI_TYPE_INDICATOR, 1, 3, 3, {"real"}, {"short_period[12]","long_period[26]","signal_period[9]"}, {"macd","macd_signal","?macd_histogram"}, 0, 0, 0}, {"macd_fastline_divergence", "MACD Fastline Divergence", ti_macd_fastline_divergence_start, ti_macd_fastline_divergence, 0, TI_TYPE_OVERLAY, 3, 3, 2, {"high","low","close"}, {"fast_length[12]","slow_length[26]","signal_length[9]"}, {"bull","bear"}, 0, 0, 0}, {"macd_hist_divergence", "MACD Hist Divergence", ti_macd_hist_divergence_start, ti_macd_hist_divergence, 0, TI_TYPE_OVERLAY, 3, 3, 2, {"high","low","close"}, {"fast_length[12]","slow_length[26]","signal_length[9]"}, {"bull","bear"}, 0, 0, 0}, {"marketfi", "Market Facilitation Index", ti_marketfi_start, ti_marketfi, 0, TI_TYPE_INDICATOR, 3, 0, 1, {"high","low","volume"}, {""}, {"marketfi"}, 0, 0, 0}, {"mass", "Mass Index", ti_mass_start, ti_mass, 0, TI_TYPE_INDICATOR, 2, 1, 1, {"high","low"}, {"period"}, {"mass"}, 0, 0, 0}, {"max", "Maximum In Period", ti_max_start, ti_max, ti_max_ref, TI_TYPE_MATH, 1, 1, 1, {"real"}, {"period"}, {"max"}, 0, 0, 0}, {"md", "Mean Deviation Over Period", ti_md_start, ti_md, 0, TI_TYPE_MATH, 1, 1, 1, {"real"}, {"period"}, {"md"}, 0, 0, 0}, {"medprice", "Median Price", ti_medprice_start, ti_medprice, 0, TI_TYPE_OVERLAY, 2, 0, 1, {"high","low"}, {""}, {"medprice"}, 0, 0, 0}, {"mfi", "Money Flow Index", ti_mfi_start, ti_mfi, 0, TI_TYPE_INDICATOR, 4, 1, 1, {"high","low","close","volume"}, {"period[14]"}, {"mfi"}, 0, 0, 0}, {"min", "Minimum In Period", ti_min_start, ti_min, ti_min_ref, TI_TYPE_MATH, 1, 1, 1, {"real"}, {"period"}, {"min"}, 0, 0, 0}, {"mobo_band", "Mobo Band", ti_mobo_band_start, ti_mobo_band, 0, TI_TYPE_OVERLAY, 2, 4, 1, {"high","low"}, {"dpo_length[13]","mobo_length[10]","num_dev_down[-0.8]","num_dev_up[0.8]"}, {"buy_sell_signal"}, 0, 0, 0}, {"mom", "Momentum", ti_mom_start, ti_mom, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real"}, {"period"}, {"mom"}, 0, 0, 0}, {"mul", "Vector Multiplication", ti_mul_start, ti_mul, 0, TI_TYPE_SIMPLE, 2, 0, 1, {"value_one","value_two"}, {""}, {"mul"}, 0, 0, 0}, {"natr", "Normalized Average True Range", ti_natr_start, ti_natr, 0, TI_TYPE_INDICATOR, 3, 1, 1, {"high","low","close"}, {"period[14]"}, {"natr"}, 0, 0, 0}, {"price", "Compare Price", ti_price_start, ti_price, 0, TI_TYPE_INDICATOR, 1, 0, 1, {"value(ohlc)"}, {""}, {"price"}, 0, 0, 0}, {"psar", "PSAR", ti_psar_start, ti_psar, 0, TI_TYPE_INDICATOR, 3, 3, 1, {"high","low","close"}, {"accel_start[0.02]","accel_step[0.02]","accel_max[0.2]"}, {"psar(ohlc)"}, 0, 0, 0}, {"qqe_mod", "QQE Mod", ti_qqe_mod_start, ti_qqe_mod, 0, TI_TYPE_OVERLAY, 1, 10, 2, {"close"}, {"rsi_length_one[6]","rsi_smoothing_one[5]","qqe_factor_one[3]","threshold_one[3]","rsi_length_two[6]","rsi_smoothing_two[5]","qqe_factor_two[1.61]","threshold_two[3]","bollinger_length[50]","qqe_multiplier[0.35]"}, {"bar_color_one","bar_color_two"}, 0, 0, 0}, {"roc", "Rate of Change", ti_roc_start, ti_roc, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real"}, {"period"}, {"roc"}, 0, 0, 0}, {"rocr", "Rate of Change Ratio", ti_rocr_start, ti_rocr, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real"}, {"period"}, {"rocr"}, 0, 0, 0}, {"round", "Vector Round", ti_round_start, ti_round, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real"}, {""}, {"round"}, 0, 0, 0}, {"rsi", "Relative Strength Index", ti_rsi_start, ti_rsi, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real"}, {"period[14]"}, {"rsi"}, 0, 0, 0}, {"rsi_divergence", "Relative Strength Index Divergence", ti_rsi_divergence_start, ti_rsi_divergence, 0, TI_TYPE_OVERLAY, 3, 3, 2, {"high","low","close"}, {"left_bar[6]","right_bar[2]","rsi_length[14]"}, {"bull","bear"}, 0, 0, 0}, {"rvi", "Relative Volatility Index", ti_rvi_start, ti_rvi, 0, TI_TYPE_OVERLAY, 1, 2, 1, {"close"}, {"std_length[10]","ema_length[14]"}, {"rvi"}, 0, 0, 0}, {"rvi_divergence", "Relative Volatility Index Divergence", ti_rvi_divergence_start, ti_rvi_divergence, 0, TI_TYPE_OVERLAY, 3, 4, 2, {"high","low","close"}, {"left_bar[6]","right_bar[2]","std_length[12]","ema_length[14]"}, {"bull","bear"}, 0, 0, 0}, {"sin", "Vector Sine", ti_sin_start, ti_sin, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real"}, {""}, {"sin"}, 0, 0, 0}, {"sinh", "Vector Hyperbolic Sine", ti_sinh_start, ti_sinh, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real"}, {""}, {"sinh"}, 0, 0, 0}, {"sma", "Simple Moving Average", ti_sma_start, ti_sma, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"real"}, {"period[7]"}, {"sma(ohlcv)"}, ti_sma_stream_new, ti_sma_stream_run, ti_sma_stream_free}, {"sqrt", "Vector Square Root", ti_sqrt_start, ti_sqrt, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real"}, {""}, {"sqrt"}, 0, 0, 0}, {"ssl", "SSL", ti_ssl_start, ti_ssl, 0, TI_TYPE_OVERLAY, 3, 2, 6, {"high","low","close"}, {"ma_length[60]","ssl3_length[15]"}, {"?bbmc(ohlc)","bar_color","?up_erk(ohlc)","?low_erk(ohlc)","?cross_long","?cross_short"}, 0, 0, 0}, {"stc", "STC", ti_stc_start, ti_stc, 0, TI_TYPE_OVERLAY, 1, 4, 2, {"close"}, {"length[12]","fast_length[26]","slow_length[50]","aaa[0.5]"}, {"?stc","bar_color"}, 0, 0, 0}, {"stddev", "Standard Deviation Over Period", ti_stddev_start, ti_stddev, 0, TI_TYPE_MATH, 1, 1, 1, {"real"}, {"period"}, {"stddev"}, 0, 0, 0}, {"stderr", "Standard Error Over Period", ti_stderr_start, ti_stderr, 0, TI_TYPE_MATH, 1, 1, 1, {"real"}, {"period"}, {"stderr"}, 0, 0, 0}, {"stoch", "Stochastic Oscillator", ti_stoch_start, ti_stoch, 0, TI_TYPE_INDICATOR, 3, 3, 2, {"high","low","close"}, {"k_period[14]","k_slowing_period[1]","d_period[3]"}, {"stoch_k","stoch_d"}, 0, 0, 0}, {"stoch_divergence", "Stochastic Divergence", ti_stoch_divergence_start, ti_stoch_divergence, 0, TI_TYPE_OVERLAY, 3, 5, 2, {"high","low","close"}, {"left_bar[6]","right_bar[2]","stk_length[14]","smooth_length[3]","sma_length[3]"}, {"bull","bear"}, 0, 0, 0}, {"stoch_rsi", "Stoch Rsi", ti_stoch_rsi_start, ti_stoch_rsi, 0, TI_TYPE_OVERLAY, 1, 4, 2, {"close"}, {"smoothk[3]","smoothd[3]","rsi_period[14]","stoch_period[14]"}, {"stoch_k","stoch_d"}, 0, 0, 0}, {"stochrsi", "Stochastic RSI", ti_stochrsi_start, ti_stochrsi, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real"}, {"period[14]"}, {"stochrsi"}, 0, 0, 0}, {"sub", "Vector Subtraction", ti_sub_start, ti_sub, 0, TI_TYPE_SIMPLE, 2, 0, 1, {"value_one","value_two"}, {""}, {"sub"}, 0, 0, 0}, {"sum", "Sum Over Period", ti_sum_start, ti_sum, 0, TI_TYPE_MATH, 1, 1, 1, {"real"}, {"period"}, {"sum"}, 0, 0, 0}, {"sup_and_res", "Support and Resistance", ti_sup_and_res_start, ti_sup_and_res, 0, TI_TYPE_OVERLAY, 1, 4, 16, {"close"}, {"left_bar[200]","right_bar_one[20]","right_bar_two[5]","hma_length[9]"}, {"buy_one","buy_two","buy_three","buy_four","buy_five","buy_six","buy_seven","buy_eight","sell_one","sell_two","sell_three","sell_four","sell_five","sell_six","sell_seven","sell_eight"}, 0, 0, 0}, {"supertrend", "Supertrend", ti_supertrend_start, ti_supertrend, 0, TI_TYPE_OVERLAY, 3, 2, 4, {"high","low","close"}, {"period[34]","factor[3]"}, {"?supertrend(ohlc)","?direction","bar_color","buy_sell_signal"}, 0, 0, 0}, {"tan", "Vector Tangent", ti_tan_start, ti_tan, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real"}, {""}, {"tan"}, 0, 0, 0}, {"tanh", "Vector Hyperbolic Tangent", ti_tanh_start, ti_tanh, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real"}, {""}, {"tanh"}, 0, 0, 0}, {"tema", "Triple Exponential Moving Average", ti_tema_start, ti_tema, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"real"}, {"period[9]"}, {"tema(ohlcv)"}, 0, 0, 0}, {"todeg", "Vector Degree Conversion", ti_todeg_start, ti_todeg, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real"}, {""}, {"degrees"}, 0, 0, 0}, {"torad", "Vector Radian Conversion", ti_torad_start, ti_torad, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real"}, {""}, {"radians"}, 0, 0, 0}, {"tr", "True Range", ti_tr_start, ti_tr, 0, TI_TYPE_INDICATOR, 3, 0, 1, {"high","low","close"}, {""}, {"tr"}, 0, 0, 0}, {"trima", "Triangular Moving Average", ti_trima_start, ti_trima, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"real"}, {"period[20]"}, {"trima(ohlcv)"}, 0, 0, 0}, {"trix", "Trix", ti_trix_start, ti_trix, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real"}, {"period"}, {"trix"}, 0, 0, 0}, {"trunc", "Vector Truncate", ti_trunc_start, ti_trunc, 0, TI_TYPE_SIMPLE, 1, 0, 1, {"real"}, {""}, {"trunc"}, 0, 0, 0}, {"tsf", "Time Series Forecast", ti_tsf_start, ti_tsf, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"real"}, {"period"}, {"tsf"}, 0, 0, 0}, {"typprice", "Typical Price", ti_typprice_start, ti_typprice, 0, TI_TYPE_OVERLAY, 3, 0, 1, {"high","low","close"}, {""}, {"typprice"}, 0, 0, 0}, {"ultosc", "Ultimate Oscillator", ti_ultosc_start, ti_ultosc, 0, TI_TYPE_INDICATOR, 3, 3, 1, {"high","low","close"}, {"short_period","medium_period","long_period"}, {"ultosc"}, 0, 0, 0}, {"unshift", "Unshift", ti_unshift_start, ti_unshift, 0, TI_TYPE_SIMPLE, 1, 2, 1, {"value"}, {"default_value","length"}, {"unshifted_value"}, 0, 0, 0}, {"ut_bot", "UT Bot Alert", ti_ut_bot_start, ti_ut_bot, 0, TI_TYPE_OVERLAY, 3, 2, 1, {"high","low","close"}, {"atr_period[10]","sensitivity[1]"}, {"buy_sell_signal"}, 0, 0, 0}, {"var", "Variance Over Period", ti_var_start, ti_var, 0, TI_TYPE_MATH, 1, 1, 1, {"real"}, {"period"}, {"var"}, 0, 0, 0}, {"vhf", "Vertical Horizontal Filter", ti_vhf_start, ti_vhf, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real"}, {"period"}, {"vhf"}, 0, 0, 0}, {"volatility", "Annualized Historical Volatility", ti_volatility_start, ti_volatility, 0, TI_TYPE_INDICATOR, 1, 1, 1, {"real"}, {"period"}, {"volatility"}, 0, 0, 0}, {"volatility_oscillator", "Volatility Oscillator", ti_volatility_oscillator_start, ti_volatility_oscillator, 0, TI_TYPE_OVERLAY, 2, 1, 3, {"open","close"}, {"length[100]"}, {"spike_line","upper_line","lower_line"}, 0, 0, 0}, {"vosc", "Volume Oscillator", ti_vosc_start, ti_vosc, 0, TI_TYPE_INDICATOR, 1, 2, 1, {"volume"}, {"short_period","long_period"}, {"vosc"}, 0, 0, 0}, {"vu_man_chu_swing", "VU Man Chu Swing", ti_vu_man_chu_swing_start, ti_vu_man_chu_swing, 0, TI_TYPE_OVERLAY, 1, 2, 2, {"close"}, {"swing_period[20]","swing_multiplier[3.5]"}, {"buy_sell_signal_long","buy_sell_signal_short"}, 0, 0, 0}, {"vwma", "Volume Weighted Moving Average", ti_vwma_start, ti_vwma, 0, TI_TYPE_OVERLAY, 2, 1, 1, {"close","volume"}, {"period[20]"}, {"vwma(v)"}, 0, 0, 0}, {"wad", "Williams Accumulation/Distribution", ti_wad_start, ti_wad, 0, TI_TYPE_INDICATOR, 3, 0, 1, {"high","low","close"}, {""}, {"wad"}, 0, 0, 0}, {"waddah", "Waddah", ti_waddah_start, ti_waddah, 0, TI_TYPE_OVERLAY, 1, 6, 4, {"close"}, {"fast_length[20]","slow_length[40]","signal_length[9]","bb_length[20]","multiplier[2]","sensitivity[150]"}, {"?t","e","trend_up","trend_down"}, 0, 0, 0}, {"wavetrend", "Wavetrend", ti_wavetrend_start, ti_wavetrend, 0, TI_TYPE_OVERLAY, 3, 2, 2, {"high","low","close"}, {"period_one[9]","period_two[12]"}, {"wavetrend_one","wavetrend_two"}, 0, 0, 0}, {"wcprice", "Weighted Close Price", ti_wcprice_start, ti_wcprice, 0, TI_TYPE_OVERLAY, 3, 0, 1, {"high","low","close"}, {""}, {"wcprice"}, 0, 0, 0}, {"wilders", "Wilders Smoothing", ti_wilders_start, ti_wilders, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"real"}, {"period"}, {"wilders"}, 0, 0, 0}, {"willr", "Williams %R", ti_willr_start, ti_willr, 0, TI_TYPE_INDICATOR, 3, 1, 1, {"high","low","close"}, {"period"}, {"willr"}, 0, 0, 0}, {"wma", "Weighted Moving Average", ti_wma_start, ti_wma, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"real"}, {"period[9]"}, {"wma(ohlcv)"}, 0, 0, 0}, {"zlema", "Zero-Lag Exponential Moving Average", ti_zlema_start, ti_zlema, 0, TI_TYPE_OVERLAY, 1, 1, 1, {"real"}, {"period"}, {"zlema(ohlcv)"}, 0, 0, 0}, {0,0,0,0,0,0,0,0,0,{0,0},{0,0},{0,0},0,0,0}};
 struct ti_stream {
     int index;
     int progress;
 };
 int ti_stream_run(ti_stream *stream, int size, TI_REAL const *const *inputs, TI_REAL *const *outputs) {
     return ti_indicators[stream->index].stream_run(stream, size, inputs, outputs);
 }
```

### Comparing `cybotrade-indicators-0.0.4/pyproject.toml` & `cybotrade-indicators-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "cybotrade-indicators"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name = "Marcus Lee", email = "marcuslee@balaenaquant.com" },
     { name = "Lee Ze Lim", email = "zelim@balaenaquant.com" },
 ]
 description = "This library provides a set of technical analysis indicators that can be used to craft trading strategies."
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `cybotrade-indicators-0.0.4/src/cybotrade_indicators/__init__.c` & `cybotrade-indicators-0.0.5/src/cybotrade_indicators/__init__.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 /* Generated by Cython 3.0.0 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "external/indicators.h"
         ],
         "include_dirs": [
             "external",
             "src/cybotrade_indicators",
-            "/opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/core/include"
+            "/private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/core/include"
         ],
         "name": "cybotrade_indicators",
         "sources": [
             "src/cybotrade_indicators/__init__.pyx",
             "external/tiamalgamation.c"
         ]
     },
@@ -1438,177 +1438,177 @@
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1638,42 +1638,42 @@
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_obj_20cybotrade_indicators__Indicator;
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -6541,261 +6541,261 @@
 #define __pyx_codeobj__304 __pyx_mstate_global->__pyx_codeobj__304
 #define __pyx_codeobj__305 __pyx_mstate_global->__pyx_codeobj__305
 #define __pyx_codeobj__307 __pyx_mstate_global->__pyx_codeobj__307
 #define __pyx_codeobj__309 __pyx_mstate_global->__pyx_codeobj__309
 #define __pyx_codeobj__310 __pyx_mstate_global->__pyx_codeobj__310
 /* #### Code section: module_code ### */
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 0);
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -6804,29 +6804,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -6837,15 +6837,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -6854,29 +6854,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -6887,15 +6887,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6904,29 +6904,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6937,15 +6937,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6954,29 +6954,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6987,15 +6987,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7004,29 +7004,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7037,89 +7037,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -7127,33 +7127,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 969, __pyx_L1_error)
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -7161,96 +7161,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+    /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7266,15 +7266,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -7282,68 +7282,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 981, __pyx_L3_error)
 
-      /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+      /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+    /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 982, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 983, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+    /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -7351,15 +7351,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7374,15 +7374,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7398,15 +7398,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7414,68 +7414,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 987, __pyx_L3_error)
 
-      /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+    /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 988, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 989, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -7483,15 +7483,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7506,15 +7506,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7530,15 +7530,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7546,68 +7546,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 993, __pyx_L3_error)
 
-      /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+    /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 994, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 995, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -7615,15 +7615,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7638,176 +7638,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1010
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1010
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1025
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1025
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1035
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1035
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1042
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+/* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1049
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -33910,26 +33910,26 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(2, 983, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../../../../private/var/folders/cy/y258_d912z3brmw5dgncgqbr0000gn/T/pip-build-env-44btj9_c/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(2, 989, __pyx_L1_error)
```

### Comparing `cybotrade-indicators-0.0.4/src/cybotrade_indicators/__init__.pyi` & `cybotrade-indicators-0.0.5/src/cybotrade_indicators/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cybotrade-indicators-0.0.4/src/cybotrade_indicators/__init__.pyx` & `cybotrade-indicators-0.0.5/src/cybotrade_indicators/__init__.pyx`

 * *Files identical despite different names*

### Comparing `cybotrade-indicators-0.0.4/src/cybotrade_indicators/indicators.pxd` & `cybotrade-indicators-0.0.5/src/cybotrade_indicators/indicators.pxd`

 * *Files identical despite different names*

### Comparing `cybotrade-indicators-0.0.4/src/cybotrade_indicators.egg-info/PKG-INFO` & `cybotrade-indicators-0.0.5/src/cybotrade_indicators.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybotrade-indicators
-Version: 0.0.4
+Version: 0.0.5
 Summary: This library provides a set of technical analysis indicators that can be used to craft trading strategies.
 Author-email: Marcus Lee <marcuslee@balaenaquant.com>, Lee Ze Lim <zelim@balaenaquant.com>
 Project-URL: Homepage, https://app.cybotrade.rs
 Project-URL: Documentation, https://docs.cybotrade.rs
 Project-URL: Repository, https://github.com/cybotrade/cybotrade-indicators
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cybotrade-indicators-0.0.4/src/cybotrade_indicators.egg-info/SOURCES.txt` & `cybotrade-indicators-0.0.5/src/cybotrade_indicators.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cybotrade-indicators-0.0.4/tests/test.py` & `cybotrade-indicators-0.0.5/tests/test.py`

 * *Files identical despite different names*

