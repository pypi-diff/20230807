# Comparing `tmp/noisepy_seis-0.9.6.tar.gz` & `tmp/noisepy_seis-0.9.61.tar.gz`

## Comparing `noisepy_seis-0.9.6.tar` & `noisepy_seis-0.9.61.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11683 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/S0A_download_ASDF_MPI.py
--rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/S0B_to_ASDF.py
--rw-r--r--   0        0        0    12766 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/S1_fft_cc_MPI.py
--rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/S2_stacking.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/_version.py
--rw-r--r--   0        0        0    10254 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/asdfstore.py
--rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/channelcatalog.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/constants.py
--rw-r--r--   0        0        0     9931 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/datatypes.py
--rw-r--r--   0        0        0     8720 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/main.py
--rw-r--r--   0        0        0   113005 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/noise_module.py
--rw-r--r--   0        0        0    34841 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/plotting_modules.py
--rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/pnwstore.py
--rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/scedc_s3store.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/scheduler.py
--rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/stores.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/utils.py
--rw-r--r--   0        0        0     7705 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/zarrstore.py
--rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/application_modules/comp_stacking.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/application_modules/dispersion_analysis.py
--rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/application_modules/measure_dvv.py
--rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/src/noisepy/seis/application_modules/write_sac.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/LICENSE
--rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/README.md
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/pyproject.toml
--rw-r--r--   0        0        0    10729 2020-02-02 00:00:00.000000 noisepy_seis-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0    11683 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/src/noisepy/seis/S0A_download_ASDF_MPI.py
+-rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/src/noisepy/seis/S0B_to_ASDF.py
+-rw-r--r--   0        0        0    14150 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/src/noisepy/seis/S1_fft_cc_MPI.py
+-rw-r--r--   0        0        0    11676 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/src/noisepy/seis/S2_stacking.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/src/noisepy/seis/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/src/noisepy/seis/_version.py
+-rw-r--r--   0        0        0    10254 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/src/noisepy/seis/asdfstore.py
+-rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/src/noisepy/seis/channelcatalog.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/src/noisepy/seis/constants.py
+-rw-r--r--   0        0        0    10154 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/src/noisepy/seis/datatypes.py
+-rw-r--r--   0        0        0     8720 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/src/noisepy/seis/main.py
+-rw-r--r--   0        0        0   112813 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/src/noisepy/seis/noise_module.py
+-rw-r--r--   0        0        0    35014 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/src/noisepy/seis/plotting_modules.py
+-rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/src/noisepy/seis/pnwstore.py
+-rw-r--r--   0        0        0     5765 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/src/noisepy/seis/scedc_s3store.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/src/noisepy/seis/scheduler.py
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/src/noisepy/seis/stores.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/src/noisepy/seis/utils.py
+-rw-r--r--   0        0        0     7705 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/src/noisepy/seis/zarrstore.py
+-rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/src/noisepy/seis/application_modules/comp_stacking.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/src/noisepy/seis/application_modules/dispersion_analysis.py
+-rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/src/noisepy/seis/application_modules/measure_dvv.py
+-rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/src/noisepy/seis/application_modules/write_sac.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/LICENSE
+-rw-r--r--   0        0        0     8118 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/README.md
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/pyproject.toml
+-rw-r--r--   0        0        0    10930 2020-02-02 00:00:00.000000 noisepy_seis-0.9.61/PKG-INFO
```

### Comparing `noisepy_seis-0.9.6/src/noisepy/seis/S0A_download_ASDF_MPI.py` & `noisepy_seis-0.9.61/src/noisepy/seis/S0A_download_ASDF_MPI.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.6/src/noisepy/seis/S0B_to_ASDF.py` & `noisepy_seis-0.9.61/src/noisepy/seis/S0B_to_ASDF.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.6/src/noisepy/seis/S1_fft_cc_MPI.py` & `noisepy_seis-0.9.61/src/noisepy/seis/S1_fft_cc_MPI.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import gc
 import logging
 import sys
 import time
 from collections import OrderedDict
 from concurrent.futures import Executor, ThreadPoolExecutor, as_completed
-from typing import Dict, List, Tuple
+from typing import Callable, Dict, List, Tuple
 
 import numpy as np
 import obspy
 from datetimerange import DateTimeRange
 from scipy.fftpack.helper import next_fast_len
 
 from . import noise_module
@@ -48,22 +48,32 @@
 
 
 def cross_correlate(
     raw_store: RawDataStore,
     fft_params: ConfigParameters,
     cc_store: CrossCorrelationDataStore,
     scheduler: Scheduler = SingleNodeScheduler(),
+    pair_filter: Callable[[Channel, Channel], bool] = lambda src, rec: True,
 ):
     """
     Perform the cross-correlation analysis
 
     Args:
         raw_store: Store to load data from
         fft_params: Parameters for the FFT calculations
         cc_store: Store for saving cross correlations
+        scheduler: Scheduler to use for parallelization
+        pair_filter: Function to decide whether a pair of channels should be used or not. E.g.
+
+        .. code-block:: python
+
+            def filter_by_lat(s: Channel, d: Channel) -> bool:
+                return abs(s.station.lat - d.station.lat) > 0.1
+
+            cross_correlate(..., pair_filter=filter_by_lat)
     """
 
     executor = ThreadPoolExecutor()
     tlog = TimeLogger(logger, logging.INFO)
     t_s1_total = tlog.reset()
 
     def init() -> List:
@@ -90,15 +100,17 @@
         all_channels = raw_store.get_channels(ts)
         error_if(
             not all(map(lambda c: c.station.valid(), all_channels)),
             "The stations don't have their lat/lon/elev properties populated. Problem with the ChannelCatalog used?",
         )
 
         tlog.log("get channels")
-        ch_data_tuples = _read_channels(executor, ts, raw_store, all_channels, fft_params.samp_freq)
+        ch_data_tuples = _read_channels(
+            executor, ts, raw_store, all_channels, fft_params.samp_freq, fft_params.single_freq
+        )
         # only the channels we are using
 
         if len(ch_data_tuples) == 0:
             logger.warning(f"No data available for {ts}")
             continue
 
         channels = list(zip(*ch_data_tuples))[0]
@@ -119,31 +131,40 @@
         fft_refs = [executor.submit(compute_fft, fft_params, chd[1]) for chd in ch_data_tuples]
         fft_datas = _get_results(fft_refs)
         for ix_ch, fft_data in enumerate(fft_datas):
             if fft_data.fft.size > 0:
                 ffts[ix_ch] = fft_data
             else:
                 logger.warning(f"No data available for channel '{channels[ix_ch]}', skipped")
-        Nfft = fft_data.length
         tlog.log("Compute FFTs")
+        Nfft = max(map(lambda d: d.length, fft_datas))
+        if Nfft == 0:
+            logger.error(f"No FFT data available for any channel in {ts}, skipping")
+            continue
 
         if len(ffts) != nchannels:
             logger.warning("it seems some stations miss data in download step, but it is OKAY!")
 
         tasks = []
 
         # # ###########PERFORM CROSS-CORRELATION##################
         for iiS in range(nchannels):
             for iiR in range(iiS, nchannels):
                 src_chan = channels[iiS]
                 rec_chan = channels[iiR]
+                if not pair_filter(src_chan, rec_chan):
+                    continue
                 if fft_params.acorr_only:
                     if src_chan.station != rec_chan.station:
                         continue
+                if iiS not in ffts:
+                    logger.warning(f"No FFT data available for channel '{src_chan}', skipped")
+                    continue
                 if iiR not in ffts:
+                    logger.warning(f"No FFT data available for channel '{rec_chan}', skipped")
                     continue
                 t = executor.submit(cross_correlation, fft_params, iiS, iiR, channels, ffts, Nfft)
                 tasks.append(t)
 
         t_append = 0
         for t in as_completed(tasks):
             # Use as_completed so we can start saving results to the store
@@ -296,39 +317,47 @@
     std = trace_stdS
     fft_time = dataS_t
     del trace_stdS, dataS_t, dataS, source_white, data
     return NoiseFFT(fft, std, fft_time, N, Nfft)
 
 
 def _read_channels(
-    executor: Executor, ts: DateTimeRange, store: RawDataStore, channels: List[Channel], samp_freq: int
+    executor: Executor,
+    ts: DateTimeRange,
+    store: RawDataStore,
+    channels: List[Channel],
+    samp_freq: int,
+    single_freq: bool = True,
 ) -> List[Tuple[Channel, ChannelData]]:
     ch_data_refs = [executor.submit(store.read_data, ts, ch) for ch in channels]
     ch_data = _get_results(ch_data_refs)
     tuples = list(zip(channels, ch_data))
-    return _filter_channel_data(tuples, samp_freq)
+    return _filter_channel_data(tuples, samp_freq, single_freq)
 
 
 def _filter_channel_data(
-    tuples: List[Tuple[Channel, ChannelData]], samp_freq: int
+    tuples: List[Tuple[Channel, ChannelData]], samp_freq: int, single_freq: bool = True
 ) -> List[Tuple[Channel, ChannelData]]:
     frequencies = set(t[1].sampling_rate for t in tuples)
     frequencies = list(filter(lambda f: f >= samp_freq, frequencies))
     if len(frequencies) == 0:
         logging.warning(f"No data available with sampling frequency >= {samp_freq}")
         return []
-    closest_freq = min(
-        frequencies,
-        key=lambda f: max(f - samp_freq, 0),
-    )
-    filtered_tuples = list(filter(lambda tup: tup[1].sampling_rate == closest_freq, tuples))
-    logger.info(
-        f"Picked {closest_freq} as the closest sampling frequence to {samp_freq}. "
-        f"Filtered to {len(filtered_tuples)}/{len(tuples)} channels"
-    )
+    if single_freq:
+        closest_freq = min(
+            frequencies,
+            key=lambda f: max(f - samp_freq, 0),
+        )
+        logger.info(f"Picked {closest_freq} as the closest sampling frequence to {samp_freq}. ")
+        filtered_tuples = list(filter(lambda tup: tup[1].sampling_rate == closest_freq, tuples))
+        logger.info(f"Filtered to {len(filtered_tuples)}/{len(tuples)} channels with sampling rate == {closest_freq}")
+    else:
+        filtered_tuples = list(filter(lambda tup: tup[1].sampling_rate >= samp_freq, tuples))
+        logger.info(f"Filtered to {len(filtered_tuples)}/{len(tuples)} channels with sampling rate >= {samp_freq}")
+
     return filtered_tuples
 
 
 def check_memory(params: ConfigParameters, nsta: int) -> int:
     # maximum memory allowed per core in GB
     MAX_MEM = 4.0
     # crude estimation on memory needs (assume float32)
```

### Comparing `noisepy_seis-0.9.6/src/noisepy/seis/S2_stacking.py` & `noisepy_seis-0.9.61/src/noisepy/seis/S2_stacking.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import sys
 import time
 from concurrent.futures import ProcessPoolExecutor
+from multiprocessing import get_context
 from typing import Any, Dict, List, Tuple
 
 import numpy as np
 import pandas as pd
 from datetimerange import DateTimeRange
 
 from noisepy.seis.datatypes import ConfigParameters, StackMethod, Station
@@ -46,15 +47,16 @@
 
 def stack(
     cc_store: CrossCorrelationDataStore,
     stack_store: StackStore,
     fft_params: ConfigParameters,
     scheduler: Scheduler = SingleNodeScheduler(),
 ):
-    executor = ProcessPoolExecutor()
+    # Use 'spawn' to avoid issues with multiprocessing on linux and 'fork'
+    executor = ProcessPoolExecutor(mp_context=get_context("spawn"))
     tlog = TimeLogger(logger=logger, level=logging.INFO)
     t_tot = tlog.reset()
 
     def initializer():
         timespans = cc_store.get_timespans()
         pairs_all = cc_store.get_station_pairs()
         logger.info(f"Station pairs: {pairs_all}")
```

### Comparing `noisepy_seis-0.9.6/src/noisepy/seis/__init__.py` & `noisepy_seis-0.9.61/src/noisepy/seis/__init__.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.6/src/noisepy/seis/asdfstore.py` & `noisepy_seis-0.9.61/src/noisepy/seis/asdfstore.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.6/src/noisepy/seis/channelcatalog.py` & `noisepy_seis-0.9.61/src/noisepy/seis/channelcatalog.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.6/src/noisepy/seis/datatypes.py` & `noisepy_seis-0.9.61/src/noisepy/seis/datatypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,20 @@
 class ConfigParameters(BaseModel):
     model_config = ConfigDict(validate_default=True)
 
     client_url_key: str = "SCEDC"
     start_date: datetime = Field(default=datetime(2019, 1, 1))
     end_date: datetime = Field(default=datetime(2019, 1, 2))
     samp_freq: float = Field(default=20.0)  # TODO: change this samp_freq for the obspy "sampling_rate"
+    single_freq: bool = Field(
+        default=True,
+        description="Filter to only data sampled at ONE frequency (the closest >= to samp_freq). "
+        "If False, it will use all data sample at >=samp_freq",
+    )
+
     cc_len: float = Field(default=1800.0, description="basic unit of data length for fft (sec)")
     # download params.
     # Targeted region/station information: only needed when down_list is False
     lamin: float = Field(default=31.0, description="Download: minimum latitude")
     lamax: float = Field(default=36.0, description="Download: maximum latitude")
     lomin: float = Field(default=-122.0, description="Download: minimum longitude")
     lomax: float = Field(default=-115.0, description="Download: maximum longitude")
```

### Comparing `noisepy_seis-0.9.6/src/noisepy/seis/main.py` & `noisepy_seis-0.9.61/src/noisepy/seis/main.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.6/src/noisepy/seis/noise_module.py` & `noisepy_seis-0.9.61/src/noisepy/seis/noise_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -1238,5826 +1238,5814 @@
 00004d50: 0a20 2020 2064 6174 6153 203d 2064 6574  .    dataS = det
 00004d60: 7265 6e64 2864 6174 6153 290a 2020 2020  rend(dataS).    
 00004d70: 6461 7461 5320 3d20 7461 7065 7228 6461  dataS = taper(da
 00004d80: 7461 5329 0a0a 2020 2020 7265 7475 726e  taS)..    return
 00004d90: 2074 7261 6365 5f73 7464 532c 2064 6174   trace_stdS, dat
 00004da0: 6153 5f74 2c20 6461 7461 530a 0a0a 6465  aS_t, dataS...de
 00004db0: 6620 6e6f 6973 655f 7072 6f63 6573 7369  f noise_processi
-00004dc0: 6e67 2866 6674 5f70 6172 612c 2064 6174  ng(fft_para, dat
-00004dd0: 6153 293a 0a20 2020 2022 2222 0a20 2020  aS):.    """.   
-00004de0: 2074 6869 7320 6675 6e63 7469 6f6e 2070   this function p
-00004df0: 6572 666f 726d 7320 7469 6d65 2064 6f6d  erforms time dom
-00004e00: 6169 6e20 616e 6420 6672 6571 7565 6e63  ain and frequenc
-00004e10: 7920 646f 6d61 696e 206e 6f72 6d61 6c69  y domain normali
-00004e20: 7a61 7469 6f6e 2069 6620 6e65 6564 6564  zation if needed
-00004e30: 2e20 696e 2072 6561 6c20 6361 7365 2c20  . in real case, 
-00004e40: 7765 2070 7265 6665 7220 7573 6520 696e  we prefer use in
-00004e50: 636c 7564 650a 2020 2020 7468 6520 6e6f  clude.    the no
-00004e60: 726d 616c 697a 6174 696f 6e20 696e 2074  rmalization in t
-00004e70: 6865 2063 726f 7373 2d63 6f72 7265 616c  he cross-correal
-00004e80: 7469 6f6e 2073 7465 7073 2062 7920 7365  tion steps by se
-00004e90: 6c65 6374 696e 6720 636f 6865 7265 6e63  lecting coherenc
-00004ea0: 7920 6f72 2064 6563 6f6e 0a20 2020 2028  y or decon.    (
-00004eb0: 5072 6965 746f 2065 7420 616c 2c20 3230  Prieto et al, 20
-00004ec0: 3038 2c20 3230 3039 3b20 4465 6e6f 6c6c  08, 2009; Denoll
-00004ed0: 6520 6574 2061 6c2c 2032 3031 3329 0a20  e et al, 2013). 
-00004ee0: 2020 2050 4152 4d41 4554 4552 533a 0a20     PARMAETERS:. 
-00004ef0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
-00004f00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
-00004f10: 6666 745f 7061 7261 3a20 6469 6374 696f  fft_para: dictio
-00004f20: 6e61 7279 2063 6f6e 7461 696e 696e 6720  nary containing 
-00004f30: 616c 6c20 7573 6566 756c 2076 6172 6961  all useful varia
-00004f40: 626c 6573 2075 7365 6420 666f 7220 6666  bles used for ff
-00004f50: 7420 616e 6420 6363 0a20 2020 2064 6174  t and cc.    dat
-00004f60: 6153 3a20 3244 206d 6174 7269 7820 6f66  aS: 2D matrix of
-00004f70: 2061 6c6c 2073 6567 6d65 6e74 6564 206e   all segmented n
-00004f80: 6f69 7365 2064 6174 610a 2020 2020 2320  oise data.    # 
-00004f90: 4f55 5450 5554 2056 4152 4941 424c 4553  OUTPUT VARIABLES
-00004fa0: 3a0a 2020 2020 736f 7572 6365 5f77 6869  :.    source_whi
-00004fb0: 7465 3a20 3244 206d 6174 7269 7820 6f66  te: 2D matrix of
-00004fc0: 2064 6174 6120 7370 6563 7472 610a 2020   data spectra.  
-00004fd0: 2020 2222 220a 2020 2020 2320 6c6f 6164    """.    # load
-00004fe0: 2070 6172 616d 6574 6572 7320 6669 7273   parameters firs
-00004ff0: 740a 2020 2020 7469 6d65 5f6e 6f72 6d20  t.    time_norm 
-00005000: 3d20 6666 745f 7061 7261 5b22 7469 6d65  = fft_para["time
-00005010: 5f6e 6f72 6d22 5d0a 2020 2020 6672 6571  _norm"].    freq
-00005020: 5f6e 6f72 6d20 3d20 6666 745f 7061 7261  _norm = fft_para
-00005030: 5b22 6672 6571 5f6e 6f72 6d22 5d0a 2020  ["freq_norm"].  
-00005040: 2020 736d 6f6f 7468 5f4e 203d 2066 6674    smooth_N = fft
-00005050: 5f70 6172 615b 2273 6d6f 6f74 685f 4e22  _para["smooth_N"
-00005060: 5d0a 2020 2020 4e20 3d20 6461 7461 532e  ].    N = dataS.
-00005070: 7368 6170 655b 305d 0a0a 2020 2020 2320  shape[0]..    # 
-00005080: 2d2d 2d2d 2d2d 746f 206e 6f72 6d61 6c69  ------to normali
-00005090: 7a65 2069 6e20 7469 6d65 206f 7220 6e6f  ze in time or no
-000050a0: 742d 2d2d 2d2d 2d0a 2020 2020 6966 2074  t------.    if t
-000050b0: 696d 655f 6e6f 726d 2021 3d20 226e 6f22  ime_norm != "no"
-000050c0: 3a0a 2020 2020 2020 2020 6966 2074 696d  :.        if tim
-000050d0: 655f 6e6f 726d 203d 3d20 226f 6e65 5f62  e_norm == "one_b
-000050e0: 6974 223a 2020 2320 7369 676e 206e 6f72  it":  # sign nor
-000050f0: 6d61 6c69 7a61 7469 6f6e 0a20 2020 2020  malization.     
-00005100: 2020 2020 2020 2077 6869 7465 203d 206e         white = n
-00005110: 702e 7369 676e 2864 6174 6153 290a 2020  p.sign(dataS).  
-00005120: 2020 2020 2020 656c 6966 2074 696d 655f        elif time_
-00005130: 6e6f 726d 203d 3d20 2272 6d61 223a 2020  norm == "rma":  
-00005140: 2320 7275 6e6e 696e 6720 6d65 616e 3a20  # running mean: 
-00005150: 6e6f 726d 616c 697a 6174 696f 6e20 6f76  normalization ov
-00005160: 6572 2073 6d6f 6f74 6865 6420 6162 736f  er smoothed abso
-00005170: 6c75 7465 2061 7665 7261 6765 0a20 2020  lute average.   
-00005180: 2020 2020 2020 2020 2077 6869 7465 203d           white =
-00005190: 206e 702e 7a65 726f 7328 7368 6170 653d   np.zeros(shape=
-000051a0: 6461 7461 532e 7368 6170 652c 2064 7479  dataS.shape, dty
-000051b0: 7065 3d64 6174 6153 2e64 7479 7065 290a  pe=dataS.dtype).
-000051c0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000051d0: 6b6b 6b20 696e 2072 616e 6765 284e 293a  kkk in range(N):
-000051e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000051f0: 2077 6869 7465 5b6b 6b6b 2c20 3a5d 203d   white[kkk, :] =
-00005200: 2064 6174 6153 5b6b 6b6b 2c20 3a5d 202f   dataS[kkk, :] /
-00005210: 206d 6f76 696e 675f 6176 6528 6e70 2e61   moving_ave(np.a
-00005220: 6273 2864 6174 6153 5b6b 6b6b 2c20 3a5d  bs(dataS[kkk, :]
-00005230: 292c 2073 6d6f 6f74 685f 4e29 0a0a 2020  ), smooth_N)..  
-00005240: 2020 656c 7365 3a20 2023 2064 6f6e 2774    else:  # don't
-00005250: 206e 6f72 6d61 6c69 7a65 0a20 2020 2020   normalize.     
-00005260: 2020 2077 6869 7465 203d 2064 6174 6153     white = dataS
-00005270: 0a0a 2020 2020 2320 2d2d 2d2d 2d74 6f20  ..    # -----to 
-00005280: 7768 6974 656e 206f 7220 6e6f 742d 2d2d  whiten or not---
-00005290: 2d2d 2d0a 2020 2020 6966 2066 7265 715f  ---.    if freq_
-000052a0: 6e6f 726d 2021 3d20 226e 6f22 3a0a 2020  norm != "no":.  
-000052b0: 2020 2020 2020 736f 7572 6365 5f77 6869        source_whi
-000052c0: 7465 203d 2077 6869 7465 6e28 7768 6974  te = whiten(whit
-000052d0: 652c 2066 6674 5f70 6172 6129 2020 2320  e, fft_para)  # 
-000052e0: 7768 6974 656e 2061 6e64 2072 6574 7572  whiten and retur
-000052f0: 6e20 4646 540a 2020 2020 656c 7365 3a0a  n FFT.    else:.
-00005300: 2020 2020 2020 2020 4e66 6674 203d 2069          Nfft = i
-00005310: 6e74 286e 6578 745f 6661 7374 5f6c 656e  nt(next_fast_len
-00005320: 2869 6e74 2864 6174 6153 2e73 6861 7065  (int(dataS.shape
-00005330: 5b31 5d29 2929 0a20 2020 2020 2020 2073  [1]))).        s
-00005340: 6f75 7263 655f 7768 6974 6520 3d20 7363  ource_white = sc
-00005350: 6970 792e 6666 7470 6163 6b2e 6666 7428  ipy.fftpack.fft(
-00005360: 7768 6974 652c 204e 6666 742c 2061 7869  white, Nfft, axi
-00005370: 733d 3129 2020 2320 7265 7475 726e 2046  s=1)  # return F
-00005380: 4654 0a0a 2020 2020 7265 7475 726e 2073  FT..    return s
-00005390: 6f75 7263 655f 7768 6974 650a 0a0a 6465  ource_white...de
-000053a0: 6620 736d 6f6f 7468 5f73 6f75 7263 655f  f smooth_source_
-000053b0: 7370 6563 7428 6363 5f70 6172 612c 2066  spect(cc_para, f
-000053c0: 6674 3129 3a0a 2020 2020 2222 220a 2020  ft1):.    """.  
-000053d0: 2020 7468 6973 2066 756e 6374 696f 6e20    this function 
-000053e0: 736d 6f6f 7468 6573 2061 6d70 6c69 7475  smoothes amplitu
-000053f0: 6465 2073 7065 6374 7275 6d20 6f66 2074  de spectrum of t
-00005400: 6865 2032 4420 7370 6563 7472 616c 206d  he 2D spectral m
-00005410: 6174 7269 782e 2028 7573 6564 2069 6e20  atrix. (used in 
-00005420: 5331 290a 2020 2020 5041 5241 4d45 5445  S1).    PARAMETE
-00005430: 5253 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  RS:.    --------
-00005440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-00005450: 2020 6363 5f70 6172 613a 2064 6963 7469    cc_para: dicti
-00005460: 6f6e 6172 7920 636f 6e74 6169 6e69 6e67  onary containing
-00005470: 2075 7365 6675 6c20 6363 2070 6172 616d   useful cc param
-00005480: 6574 6572 730a 2020 2020 6666 7431 3a20  eters.    fft1: 
-00005490: 2020 2073 6f75 7263 6520 7370 6563 7472     source spectr
-000054a0: 756d 206d 6174 7269 780a 0a20 2020 2052  um matrix..    R
-000054b0: 4554 5552 4e53 3a0a 2020 2020 2d2d 2d2d  ETURNS:.    ----
-000054c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000054d0: 2d0a 2020 2020 7366 6674 313a 2063 6f6d  -.    sfft1: com
-000054e0: 706c 6578 206e 756d 7079 2061 7272 6179  plex numpy array
-000054f0: 2077 6974 6820 6e6f 726d 616c 697a 6564   with normalized
-00005500: 2073 7065 6374 7275 6d0a 2020 2020 2222   spectrum.    ""
-00005510: 220a 2020 2020 6363 5f6d 6574 686f 6420  ".    cc_method 
-00005520: 3d20 6363 5f70 6172 615b 2263 635f 6d65  = cc_para["cc_me
-00005530: 7468 6f64 225d 0a20 2020 2073 6d6f 6f74  thod"].    smoot
-00005540: 6873 7065 6374 5f4e 203d 2063 635f 7061  hspect_N = cc_pa
-00005550: 7261 5b22 736d 6f6f 7468 7370 6563 745f  ra["smoothspect_
-00005560: 4e22 5d0a 0a20 2020 2069 6620 6363 5f6d  N"]..    if cc_m
-00005570: 6574 686f 6420 3d3d 2022 6465 636f 6e76  ethod == "deconv
-00005580: 223a 0a20 2020 2020 2020 2023 202d 2d2d  ":.        # ---
-00005590: 2d2d 6e6f 726d 616c 697a 6520 7369 6e67  --normalize sing
-000055a0: 6c65 2d73 7461 7469 6f6e 2063 6320 746f  le-station cc to
-000055b0: 207a 2063 6f6d 706f 6e65 6e74 2d2d 2d2d   z component----
-000055c0: 2d0a 2020 2020 2020 2020 7465 6d70 203d  -.        temp =
-000055d0: 206d 6f76 696e 675f 6176 6528 6e70 2e61   moving_ave(np.a
-000055e0: 6273 2866 6674 3129 2c20 736d 6f6f 7468  bs(fft1), smooth
-000055f0: 7370 6563 745f 4e29 0a20 2020 2020 2020  spect_N).       
-00005600: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00005610: 2020 7366 6674 3120 3d20 6e70 2e63 6f6e    sfft1 = np.con
-00005620: 6a28 6666 7431 2920 2f20 7465 6d70 2a2a  j(fft1) / temp**
-00005630: 320a 2020 2020 2020 2020 6578 6365 7074  2.        except
-00005640: 2045 7863 6570 7469 6f6e 3a0a 2020 2020   Exception:.    
-00005650: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00005660: 6c75 6545 7272 6f72 2822 736d 6f6f 7468  lueError("smooth
-00005670: 6564 2073 7065 6374 7275 6d20 6861 7320  ed spectrum has 
-00005680: 7a65 726f 2076 616c 7565 7322 290a 0a20  zero values").. 
-00005690: 2020 2065 6c69 6620 6363 5f6d 6574 686f     elif cc_metho
-000056a0: 6420 3d3d 2022 636f 6865 7265 6e63 7922  d == "coherency"
-000056b0: 3a0a 2020 2020 2020 2020 7465 6d70 203d  :.        temp =
-000056c0: 206d 6f76 696e 675f 6176 6528 6e70 2e61   moving_ave(np.a
-000056d0: 6273 2866 6674 3129 2c20 736d 6f6f 7468  bs(fft1), smooth
-000056e0: 7370 6563 745f 4e29 0a20 2020 2020 2020  spect_N).       
-000056f0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00005700: 2020 7366 6674 3120 3d20 6e70 2e63 6f6e    sfft1 = np.con
-00005710: 6a28 6666 7431 2920 2f20 7465 6d70 0a20  j(fft1) / temp. 
-00005720: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-00005730: 6365 7074 696f 6e3a 0a20 2020 2020 2020  ception:.       
-00005740: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00005750: 4572 726f 7228 2273 6d6f 6f74 6865 6420  Error("smoothed 
-00005760: 7370 6563 7472 756d 2068 6173 207a 6572  spectrum has zer
-00005770: 6f20 7661 6c75 6573 2229 0a0a 2020 2020  o values")..    
-00005780: 656c 6966 2063 635f 6d65 7468 6f64 203d  elif cc_method =
-00005790: 3d20 2278 636f 7272 223a 0a20 2020 2020  = "xcorr":.     
-000057a0: 2020 2073 6666 7431 203d 206e 702e 636f     sfft1 = np.co
-000057b0: 6e6a 2866 6674 3129 0a0a 2020 2020 656c  nj(fft1)..    el
-000057c0: 7365 3a0a 2020 2020 2020 2020 7261 6973  se:.        rais
-000057d0: 6520 5661 6c75 6545 7272 6f72 2822 6e6f  e ValueError("no
-000057e0: 2063 6f72 7265 6374 696f 6e20 636f 7272   correction corr
-000057f0: 656c 6174 696f 6e20 6d65 7468 6f64 2069  elation method i
-00005800: 7320 7365 6c65 6374 6564 2061 7420 4c35  s selected at L5
-00005810: 3922 290a 0a20 2020 2072 6574 7572 6e20  9")..    return 
-00005820: 7366 6674 310a 0a0a 6465 6620 636f 7272  sfft1...def corr
-00005830: 656c 6174 6528 6666 7431 5f73 6d6f 6f74  elate(fft1_smoot
-00005840: 6865 645f 6162 732c 2066 6674 322c 2044  hed_abs, fft2, D
-00005850: 2c20 4e66 6674 2c20 6461 7461 535f 7429  , Nfft, dataS_t)
-00005860: 3a0a 2020 2020 2222 220a 2020 2020 7468  :.    """.    th
-00005870: 6973 2066 756e 6374 696f 6e20 646f 6573  is function does
-00005880: 2074 6865 2063 726f 7373 2d63 6f72 7265   the cross-corre
-00005890: 6c61 7469 6f6e 2069 6e20 6672 6571 2064  lation in freq d
-000058a0: 6f6d 6169 6e20 616e 6420 6861 7320 7468  omain and has th
-000058b0: 6520 6f70 7469 6f6e 2074 6f20 6b65 6570  e option to keep
-000058c0: 2073 7562 2d73 7461 636b 7320 6f66 0a20   sub-stacks of. 
-000058d0: 2020 2074 6865 2063 726f 7373 2d63 6f72     the cross-cor
-000058e0: 7265 6c61 7469 6f6e 2069 6620 6e65 6564  relation if need
-000058f0: 6564 2e20 6974 2074 616b 6573 2061 6476  ed. it takes adv
-00005900: 616e 7461 6765 206f 6620 7468 6520 6c69  antage of the li
-00005910: 6e65 6172 2072 656c 6174 696f 6e73 6869  near relationshi
-00005920: 7020 6f66 2069 6666 742c 2073 6f20 7468  p of ifft, so th
-00005930: 6174 0a20 2020 2073 7461 636b 696e 6720  at.    stacking 
-00005940: 6973 2070 6572 666f 726d 6564 2069 6e20  is performed in 
-00005950: 7370 6563 7472 756d 2064 6f6d 6169 6e20  spectrum domain 
-00005960: 6669 7273 7420 746f 2072 6564 7563 6520  first to reduce 
-00005970: 7468 6520 746f 7461 6c20 6e75 6d62 6572  the total number
-00005980: 206f 6620 6966 6674 2e20 2875 7365 6420   of ifft. (used 
-00005990: 696e 2053 3129 0a20 2020 2050 4152 414d  in S1).    PARAM
-000059a0: 4554 4552 533a 0a20 2020 202d 2d2d 2d2d  ETERS:.    -----
-000059b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000059c0: 0a20 2020 2066 6674 315f 736d 6f6f 7468  .    fft1_smooth
-000059d0: 6564 5f61 6273 3a20 736d 6f6f 7468 6564  ed_abs: smoothed
-000059e0: 2070 6f77 6572 2073 7065 6374 7261 6c20   power spectral 
-000059f0: 6465 6e73 6974 7920 6f66 2074 6865 2046  density of the F
-00005a00: 4654 2066 6f72 2074 6865 2073 6f75 7263  FT for the sourc
-00005a10: 6520 7374 6174 696f 6e0a 2020 2020 6666  e station.    ff
-00005a20: 7432 3a20 7261 7720 4646 5420 7370 6563  t2: raw FFT spec
-00005a30: 7472 756d 206f 6620 7468 6520 7265 6365  trum of the rece
-00005a40: 6976 6572 2073 7461 7469 6f6e 0a20 2020  iver station.   
-00005a50: 2044 3a20 6469 6374 696f 6e61 7279 2063   D: dictionary c
-00005a60: 6f6e 7461 696e 696e 6720 666f 6c6c 6f77  ontaining follow
-00005a70: 696e 6720 7061 7261 6d65 7465 7273 3a0a  ing parameters:.
-00005a80: 2020 2020 2020 2020 6d61 786c 6167 3a20          maxlag: 
-00005a90: 206d 6178 696d 756d 206c 6167 7320 746f   maximum lags to
-00005aa0: 206b 6565 7020 696e 2074 6865 2063 726f   keep in the cro
-00005ab0: 7373 2063 6f72 7265 6c61 7469 6f6e 0a20  ss correlation. 
-00005ac0: 2020 2020 2020 2064 743a 2020 2020 2020         dt:      
-00005ad0: 7361 6d70 6c69 6e67 2072 6174 6520 2869  sampling rate (i
-00005ae0: 6e20 7329 0a20 2020 2020 2020 206e 7769  n s).        nwi
-00005af0: 6e3a 2020 2020 6e75 6d62 6572 206f 6620  n:    number of 
-00005b00: 7365 676d 656e 7473 2069 6e20 7468 6520  segments in the 
-00005b10: 3244 206d 6174 7269 780a 2020 2020 2020  2D matrix.      
-00005b20: 2020 6d65 7468 6f64 3a20 2063 726f 7373    method:  cross
-00005b30: 2d63 6f72 7265 6c61 7469 6f6e 206d 6574  -correlation met
-00005b40: 686f 6473 2073 656c 6563 7465 6420 6279  hods selected by
-00005b50: 2074 6865 2075 7365 720a 2020 2020 2020   the user.      
-00005b60: 2020 6672 6571 6d69 6e3a 206d 696e 696d    freqmin: minim
-00005b70: 756d 2066 7265 7175 656e 6379 2028 487a  um frequency (Hz
-00005b80: 290a 2020 2020 2020 2020 6672 6571 6d61  ).        freqma
-00005b90: 783a 206d 6178 696d 756d 2066 7265 7175  x: maximum frequ
-00005ba0: 656e 6379 2028 487a 290a 2020 2020 4e66  ency (Hz).    Nf
-00005bb0: 6674 3a20 2020 206e 756d 6265 7220 6f66  ft:    number of
-00005bc0: 2066 7265 7175 656e 6379 2070 6f69 6e74   frequency point
-00005bd0: 7320 666f 7220 6966 6674 0a20 2020 2064  s for ifft.    d
-00005be0: 6174 6153 5f74 3a20 6d61 7472 6978 206f  ataS_t: matrix o
-00005bf0: 6620 6461 7465 7469 6d65 206f 626a 6563  f datetime objec
-00005c00: 742e 0a0a 2020 2020 5245 5455 524e 533a  t...    RETURNS:
-00005c10: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
-00005c20: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2073  ----------.    s
-00005c30: 5f63 6f72 723a 2031 4420 6f72 2032 4420  _corr: 1D or 2D 
-00005c40: 6d61 7472 6978 206f 6620 7468 6520 6176  matrix of the av
-00005c50: 6572 6167 6564 206f 7220 7375 622d 7374  eraged or sub-st
-00005c60: 6163 6b73 206f 6620 6372 6f73 732d 636f  acks of cross-co
-00005c70: 7272 656c 6174 696f 6e20 6675 6e63 7469  rrelation functi
-00005c80: 6f6e 7320 696e 2074 696d 6520 646f 6d61  ons in time doma
-00005c90: 696e 0a20 2020 2074 5f63 6f72 723a 2074  in.    t_corr: t
-00005ca0: 696d 6573 7461 6d70 2066 6f72 2065 6163  imestamp for eac
-00005cb0: 6820 7375 622d 7374 6163 6b20 6f72 2061  h sub-stack or a
-00005cc0: 7665 7261 6765 6420 6675 6e63 7469 6f6e  veraged function
-00005cd0: 0a20 2020 206e 5f63 6f72 723a 206e 756d  .    n_corr: num
-00005ce0: 6265 7220 6f66 2069 6e63 6c75 6465 6420  ber of included 
-00005cf0: 7365 676d 656e 7473 2066 6f72 2065 6163  segments for eac
-00005d00: 6820 7375 622d 7374 6163 6b20 6f72 2061  h sub-stack or a
-00005d10: 7665 7261 6765 6420 6675 6e63 7469 6f6e  veraged function
-00005d20: 0a0a 2020 2020 4d4f 4449 4649 4341 5449  ..    MODIFICATI
-00005d30: 4f4e 533a 0a20 2020 202d 2d2d 2d2d 2d2d  ONS:.    -------
-00005d40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
-00005d50: 2020 206f 7574 7075 7420 7468 6520 6c69     output the li
-00005d60: 6e65 6172 2073 7461 636b 206f 6620 6561  near stack of ea
-00005d70: 6368 2074 696d 6520 6368 756e 6b20 6576  ch time chunk ev
-00005d80: 656e 2077 6865 6e20 7375 6273 7461 636b  en when substack
-00005d90: 2069 7320 7365 6c65 6374 6564 2028 6279   is selected (by
-00005da0: 2043 6865 6e67 7869 6e20 4041 7567 3230   Chengxin @Aug20
-00005db0: 3230 290a 2020 2020 2222 220a 2020 2020  20).    """.    
-00005dc0: 2320 2d2d 2d2d 6c6f 6164 2070 6172 616d  # ----load param
-00005dd0: 7465 7273 2d2d 2d2d 0a20 2020 2064 7420  ters----.    dt 
-00005de0: 3d20 445b 2264 7422 5d0a 2020 2020 6d61  = D["dt"].    ma
-00005df0: 786c 6167 203d 2044 5b22 6d61 786c 6167  xlag = D["maxlag
-00005e00: 225d 0a20 2020 206d 6574 686f 6420 3d20  "].    method = 
-00005e10: 445b 2263 635f 6d65 7468 6f64 225d 0a20  D["cc_method"]. 
-00005e20: 2020 2063 635f 6c65 6e20 3d20 445b 2263     cc_len = D["c
-00005e30: 635f 6c65 6e22 5d0a 2020 2020 7375 6273  c_len"].    subs
-00005e40: 7461 636b 203d 2044 5b22 7375 6273 7461  tack = D["substa
-00005e50: 636b 225d 0a20 2020 2073 7562 7374 6163  ck"].    substac
-00005e60: 6b5f 6c65 6e20 3d20 445b 2273 7562 7374  k_len = D["subst
-00005e70: 6163 6b5f 6c65 6e22 5d0a 2020 2020 736d  ack_len"].    sm
-00005e80: 6f6f 7468 7370 6563 745f 4e20 3d20 445b  oothspect_N = D[
-00005e90: 2273 6d6f 6f74 6873 7065 6374 5f4e 225d  "smoothspect_N"]
-00005ea0: 0a0a 2020 2020 6e77 696e 203d 2066 6674  ..    nwin = fft
-00005eb0: 315f 736d 6f6f 7468 6564 5f61 6273 2e73  1_smoothed_abs.s
-00005ec0: 6861 7065 5b30 5d0a 2020 2020 4e66 6674  hape[0].    Nfft
-00005ed0: 3220 3d20 6666 7431 5f73 6d6f 6f74 6865  2 = fft1_smoothe
-00005ee0: 645f 6162 732e 7368 6170 655b 315d 0a0a  d_abs.shape[1]..
-00005ef0: 2020 2020 2320 2d2d 2d2d 2d2d 636f 6e76      # ------conv
-00005f00: 6572 7420 616c 6c20 3244 2061 7272 6179  ert all 2D array
-00005f10: 7320 696e 746f 2031 4420 746f 2073 7065  s into 1D to spe
-00005f20: 6564 2075 702d 2d2d 2d2d 2d2d 2d0a 2020  ed up--------.  
-00005f30: 2020 636f 7272 203d 206e 702e 7a65 726f    corr = np.zero
-00005f40: 7328 6e77 696e 202a 204e 6666 7432 2c20  s(nwin * Nfft2, 
-00005f50: 6474 7970 653d 6e70 2e63 6f6d 706c 6578  dtype=np.complex
-00005f60: 3634 290a 2020 2020 636f 7272 203d 2066  64).    corr = f
-00005f70: 6674 315f 736d 6f6f 7468 6564 5f61 6273  ft1_smoothed_abs
-00005f80: 2e72 6573 6861 7065 280a 2020 2020 2020  .reshape(.      
-00005f90: 2020 6666 7431 5f73 6d6f 6f74 6865 645f    fft1_smoothed_
-00005fa0: 6162 732e 7369 7a65 2c0a 2020 2020 2920  abs.size,.    ) 
-00005fb0: 2a20 6666 7432 2e72 6573 6861 7065 280a  * fft2.reshape(.
-00005fc0: 2020 2020 2020 2020 6666 7432 2e73 697a          fft2.siz
-00005fd0: 652c 0a20 2020 2029 0a0a 2020 2020 6966  e,.    )..    if
-00005fe0: 206d 6574 686f 6420 3d3d 2022 636f 6865   method == "cohe
-00005ff0: 7265 6e63 7922 3a0a 2020 2020 2020 2020  rency":.        
-00006000: 7465 6d70 203d 206d 6f76 696e 675f 6176  temp = moving_av
-00006010: 6528 0a20 2020 2020 2020 2020 2020 206e  e(.            n
-00006020: 702e 6162 7328 0a20 2020 2020 2020 2020  p.abs(.         
-00006030: 2020 2020 2020 2066 6674 322e 7265 7368         fft2.resh
-00006040: 6170 6528 0a20 2020 2020 2020 2020 2020  ape(.           
-00006050: 2020 2020 2020 2020 2066 6674 322e 7369           fft2.si
-00006060: 7a65 2c0a 2020 2020 2020 2020 2020 2020  ze,.            
-00006070: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00006080: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-00006090: 2073 6d6f 6f74 6873 7065 6374 5f4e 2c0a   smoothspect_N,.
-000060a0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000060b0: 2020 636f 7272 202f 3d20 7465 6d70 0a20    corr /= temp. 
-000060c0: 2020 2063 6f72 7220 3d20 636f 7272 2e72     corr = corr.r
-000060d0: 6573 6861 7065 286e 7769 6e2c 204e 6666  eshape(nwin, Nff
-000060e0: 7432 290a 0a20 2020 2069 6620 7375 6273  t2)..    if subs
-000060f0: 7461 636b 3a0a 2020 2020 2020 2020 6966  tack:.        if
-00006100: 2073 7562 7374 6163 6b5f 6c65 6e20 3d3d   substack_len ==
-00006110: 2063 635f 6c65 6e3a 0a20 2020 2020 2020   cc_len:.       
-00006120: 2020 2020 2023 2063 686f 6f73 6520 746f       # choose to
-00006130: 206b 6565 7020 616c 6c20 6666 7420 6461   keep all fft da
-00006140: 7461 2066 6f72 2061 2064 6179 0a20 2020  ta for a day.   
-00006150: 2020 2020 2020 2020 2073 5f63 6f72 7220           s_corr 
-00006160: 3d20 6e70 2e7a 6572 6f73 2873 6861 7065  = np.zeros(shape
-00006170: 3d28 6e77 696e 2c20 4e66 6674 292c 2064  =(nwin, Nfft), d
-00006180: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
-00006190: 2020 2320 7374 6163 6b65 6420 636f 7272    # stacked corr
-000061a0: 656c 6174 696f 6e0a 2020 2020 2020 2020  elation.        
-000061b0: 2020 2020 616d 706d 6178 203d 206e 702e      ampmax = np.
-000061c0: 7a65 726f 7328 6e77 696e 2c20 6474 7970  zeros(nwin, dtyp
-000061d0: 653d 6e70 2e66 6c6f 6174 3332 290a 2020  e=np.float32).  
-000061e0: 2020 2020 2020 2020 2020 6e5f 636f 7272            n_corr
-000061f0: 203d 206e 702e 7a65 726f 7328 6e77 696e   = np.zeros(nwin
-00006200: 2c20 6474 7970 653d 6e70 2e69 6e74 3136  , dtype=np.int16
-00006210: 2920 2023 206e 756d 6265 7220 6f66 2063  )  # number of c
-00006220: 6f72 7265 6c61 7469 6f6e 7320 666f 7220  orrelations for 
-00006230: 6561 6368 2073 7562 7374 6163 6b0a 2020  each substack.  
-00006240: 2020 2020 2020 2020 2020 745f 636f 7272            t_corr
-00006250: 203d 2064 6174 6153 5f74 2020 2320 7469   = dataS_t  # ti
-00006260: 6d65 7374 616d 700a 2020 2020 2020 2020  mestamp.        
-00006270: 2020 2020 6372 6170 203d 206e 702e 7a65      crap = np.ze
-00006280: 726f 7328 4e66 6674 2c20 6474 7970 653d  ros(Nfft, dtype=
-00006290: 6e70 2e63 6f6d 706c 6578 3634 290a 2020  np.complex64).  
-000062a0: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
-000062b0: 696e 2072 616e 6765 286e 7769 6e29 3a0a  in range(nwin):.
-000062c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062d0: 6e5f 636f 7272 5b69 5d20 3d20 310a 2020  n_corr[i] = 1.  
-000062e0: 2020 2020 2020 2020 2020 2020 2020 6372                cr
-000062f0: 6170 5b3a 4e66 6674 325d 203d 2063 6f72  ap[:Nfft2] = cor
-00006300: 725b 692c 203a 5d0a 2020 2020 2020 2020  r[i, :].        
-00006310: 2020 2020 2020 2020 6372 6170 5b3a 4e66          crap[:Nf
-00006320: 6674 325d 203d 2063 7261 705b 3a4e 6666  ft2] = crap[:Nff
-00006330: 7432 5d20 2d20 6e70 2e6d 6561 6e28 6372  t2] - np.mean(cr
-00006340: 6170 5b3a 4e66 6674 325d 2920 2023 2072  ap[:Nfft2])  # r
-00006350: 656d 6f76 6520 7468 6520 6d65 616e 2069  emove the mean i
-00006360: 6e20 6672 6571 2064 6f6d 6169 6e20 2873  n freq domain (s
-00006370: 7069 6b65 2061 7420 743d 3029 0a20 2020  pike at t=0).   
-00006380: 2020 2020 2020 2020 2020 2020 2063 7261               cra
-00006390: 705b 2d28 4e66 6674 3229 202b 2031 203a  p[-(Nfft2) + 1 :
-000063a0: 5d20 3d20 6e70 2e66 6c69 7028 6e70 2e63  ] = np.flip(np.c
-000063b0: 6f6e 6a28 6372 6170 5b31 3a28 4e66 6674  onj(crap[1:(Nfft
-000063c0: 3229 5d29 2c20 6178 6973 3d30 290a 2020  2)]), axis=0).  
-000063d0: 2020 2020 2020 2020 2020 2020 2020 6372                cr
-000063e0: 6170 5b30 5d20 3d20 636f 6d70 6c65 7828  ap[0] = complex(
-000063f0: 302c 2030 290a 2020 2020 2020 2020 2020  0, 0).          
-00006400: 2020 2020 2020 735f 636f 7272 5b69 2c20        s_corr[i, 
-00006410: 3a5d 203d 206e 702e 7265 616c 286e 702e  :] = np.real(np.
-00006420: 6666 742e 6966 6674 7368 6966 7428 7363  fft.ifftshift(sc
-00006430: 6970 792e 6666 7470 6163 6b2e 6966 6674  ipy.fftpack.ifft
-00006440: 2863 7261 702c 204e 6666 742c 2061 7869  (crap, Nfft, axi
-00006450: 733d 3029 2929 0a0a 2020 2020 2020 2020  s=0)))..        
-00006460: 2020 2020 2320 7265 6d6f 7665 2061 626e      # remove abn
-00006470: 6f72 6d61 6c20 6461 7461 0a20 2020 2020  ormal data.     
-00006480: 2020 2020 2020 2061 6d70 6d61 7820 3d20         ampmax = 
-00006490: 6e70 2e6d 6178 2873 5f63 6f72 722c 2061  np.max(s_corr, a
-000064a0: 7869 733d 3129 0a20 2020 2020 2020 2020  xis=1).         
-000064b0: 2020 2074 696e 6478 203d 206e 702e 7768     tindx = np.wh
-000064c0: 6572 6528 2861 6d70 6d61 7820 3c20 3230  ere((ampmax < 20
-000064d0: 202a 206e 702e 6d65 6469 616e 2861 6d70   * np.median(amp
-000064e0: 6d61 7829 2920 2620 2861 6d70 6d61 7820  max)) & (ampmax 
-000064f0: 3e20 3029 295b 305d 0a20 2020 2020 2020  > 0))[0].       
-00006500: 2020 2020 2073 5f63 6f72 7220 3d20 735f       s_corr = s_
-00006510: 636f 7272 5b74 696e 6478 2c20 3a5d 0a20  corr[tindx, :]. 
-00006520: 2020 2020 2020 2020 2020 2074 5f63 6f72             t_cor
-00006530: 7220 3d20 745f 636f 7272 5b74 696e 6478  r = t_corr[tindx
-00006540: 5d0a 2020 2020 2020 2020 2020 2020 6e5f  ].            n_
-00006550: 636f 7272 203d 206e 5f63 6f72 725b 7469  corr = n_corr[ti
-00006560: 6e64 785d 0a0a 2020 2020 2020 2020 656c  ndx]..        el
-00006570: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00006580: 2320 6765 7420 7469 6d65 2069 6e66 6f72  # get time infor
-00006590: 6d61 7469 6f6e 0a20 2020 2020 2020 2020  mation.         
-000065a0: 2020 2054 746f 7461 6c20 3d20 6461 7461     Ttotal = data
-000065b0: 535f 745b 2d31 5d20 2d20 6461 7461 535f  S_t[-1] - dataS_
-000065c0: 745b 305d 2020 2320 746f 7461 6c20 6475  t[0]  # total du
-000065d0: 7261 7469 6f6e 206f 6620 7768 6174 2077  ration of what w
-000065e0: 6520 6861 7665 206e 6f77 0a20 2020 2020  e have now.     
-000065f0: 2020 2020 2020 2074 7374 6172 7420 3d20         tstart = 
-00006600: 6461 7461 535f 745b 305d 0a0a 2020 2020  dataS_t[0]..    
-00006610: 2020 2020 2020 2020 6e73 7461 636b 203d          nstack =
-00006620: 2069 6e74 286e 702e 726f 756e 6428 5474   int(np.round(Tt
-00006630: 6f74 616c 202f 2073 7562 7374 6163 6b5f  otal / substack_
-00006640: 6c65 6e29 290a 2020 2020 2020 2020 2020  len)).          
-00006650: 2020 616d 706d 6178 203d 206e 702e 7a65    ampmax = np.ze
-00006660: 726f 7328 6e73 7461 636b 2c20 6474 7970  ros(nstack, dtyp
-00006670: 653d 6e70 2e66 6c6f 6174 3332 290a 2020  e=np.float32).  
-00006680: 2020 2020 2020 2020 2020 735f 636f 7272            s_corr
-00006690: 203d 206e 702e 7a65 726f 7328 7368 6170   = np.zeros(shap
-000066a0: 653d 286e 7374 6163 6b2c 204e 6666 7429  e=(nstack, Nfft)
-000066b0: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
-000066c0: 3332 290a 2020 2020 2020 2020 2020 2020  32).            
-000066d0: 6e5f 636f 7272 203d 206e 702e 7a65 726f  n_corr = np.zero
-000066e0: 7328 6e73 7461 636b 2c20 6474 7970 653d  s(nstack, dtype=
-000066f0: 6e70 2e69 6e74 3136 290a 2020 2020 2020  np.int16).      
-00006700: 2020 2020 2020 745f 636f 7272 203d 206e        t_corr = n
-00006710: 702e 7a65 726f 7328 6e73 7461 636b 2c20  p.zeros(nstack, 
-00006720: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
-00006730: 290a 2020 2020 2020 2020 2020 2020 6372  ).            cr
-00006740: 6170 203d 206e 702e 7a65 726f 7328 4e66  ap = np.zeros(Nf
-00006750: 6674 2c20 6474 7970 653d 6e70 2e63 6f6d  ft, dtype=np.com
-00006760: 706c 6578 3634 290a 0a20 2020 2020 2020  plex64)..       
-00006770: 2020 2020 2066 6f72 2069 7374 6163 6b20       for istack 
-00006780: 696e 2072 616e 6765 286e 7374 6163 6b29  in range(nstack)
-00006790: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000067a0: 2020 2320 6669 6e64 2074 6865 2069 6e64    # find the ind
-000067b0: 6578 6573 206f 6620 616c 6c20 6f66 2074  exes of all of t
-000067c0: 6865 2077 696e 646f 7773 2074 6861 7420  he windows that 
-000067d0: 7374 6172 7420 6f72 2065 6e64 2077 6974  start or end wit
-000067e0: 6869 6e0a 2020 2020 2020 2020 2020 2020  hin.            
-000067f0: 2020 2020 6974 696d 6520 3d20 6e70 2e77      itime = np.w
-00006800: 6865 7265 2828 6461 7461 535f 7420 3e3d  here((dataS_t >=
-00006810: 2074 7374 6172 7429 2026 2028 6461 7461   tstart) & (data
-00006820: 535f 7420 3c20 7473 7461 7274 202b 2073  S_t < tstart + s
-00006830: 7562 7374 6163 6b5f 6c65 6e29 295b 305d  ubstack_len))[0]
-00006840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006850: 2069 6620 6c65 6e28 6974 696d 6529 203d   if len(itime) =
-00006860: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-00006870: 2020 2020 2020 2020 2074 7374 6172 7420           tstart 
-00006880: 2b3d 2073 7562 7374 6163 6b5f 6c65 6e0a  += substack_len.
-00006890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068a0: 2020 2020 636f 6e74 696e 7565 0a0a 2020      continue..  
-000068b0: 2020 2020 2020 2020 2020 2020 2020 6372                cr
-000068c0: 6170 5b3a 4e66 6674 325d 203d 206e 702e  ap[:Nfft2] = np.
-000068d0: 6d65 616e 2863 6f72 725b 6974 696d 652c  mean(corr[itime,
-000068e0: 203a 5d2c 2061 7869 733d 3029 2020 2320   :], axis=0)  # 
-000068f0: 6c69 6e65 6172 2061 7665 7261 6765 206f  linear average o
-00006900: 6620 7468 6520 636f 7272 656c 6174 696f  f the correlatio
-00006910: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00006920: 2020 6372 6170 5b3a 4e66 6674 325d 203d    crap[:Nfft2] =
-00006930: 2063 7261 705b 3a4e 6666 7432 5d20 2d20   crap[:Nfft2] - 
-00006940: 6e70 2e6d 6561 6e28 6372 6170 5b3a 4e66  np.mean(crap[:Nf
-00006950: 6674 325d 2920 2023 2072 656d 6f76 6520  ft2])  # remove 
-00006960: 7468 6520 6d65 616e 2069 6e20 6672 6571  the mean in freq
-00006970: 2064 6f6d 6169 6e20 2873 7069 6b65 2061   domain (spike a
-00006980: 7420 743d 3029 0a20 2020 2020 2020 2020  t t=0).         
-00006990: 2020 2020 2020 2063 7261 705b 2d28 4e66         crap[-(Nf
-000069a0: 6674 3229 202b 2031 203a 5d20 3d20 6e70  ft2) + 1 :] = np
-000069b0: 2e66 6c69 7028 6e70 2e63 6f6e 6a28 6372  .flip(np.conj(cr
-000069c0: 6170 5b31 3a28 4e66 6674 3229 5d29 2c20  ap[1:(Nfft2)]), 
-000069d0: 6178 6973 3d30 290a 2020 2020 2020 2020  axis=0).        
-000069e0: 2020 2020 2020 2020 6372 6170 5b30 5d20          crap[0] 
-000069f0: 3d20 636f 6d70 6c65 7828 302c 2030 290a  = complex(0, 0).
-00006a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a10: 735f 636f 7272 5b69 7374 6163 6b2c 203a  s_corr[istack, :
-00006a20: 5d20 3d20 6e70 2e72 6561 6c28 6e70 2e66  ] = np.real(np.f
-00006a30: 6674 2e69 6666 7473 6869 6674 2873 6369  ft.ifftshift(sci
-00006a40: 7079 2e66 6674 7061 636b 2e69 6666 7428  py.fftpack.ifft(
-00006a50: 6372 6170 2c20 4e66 6674 2c20 6178 6973  crap, Nfft, axis
-00006a60: 3d30 2929 290a 2020 2020 2020 2020 2020  =0))).          
-00006a70: 2020 2020 2020 6e5f 636f 7272 5b69 7374        n_corr[ist
-00006a80: 6163 6b5d 203d 206c 656e 2869 7469 6d65  ack] = len(itime
-00006a90: 2920 2023 206e 756d 6265 7220 6f66 2077  )  # number of w
-00006aa0: 696e 646f 7773 2073 7461 636b 730a 2020  indows stacks.  
-00006ab0: 2020 2020 2020 2020 2020 2020 2020 745f                t_
-00006ac0: 636f 7272 5b69 7374 6163 6b5d 203d 2074  corr[istack] = t
-00006ad0: 7374 6172 7420 2023 2073 6176 6520 7468  start  # save th
-00006ae0: 6520 7469 6d65 2073 7461 6d70 730a 2020  e time stamps.  
-00006af0: 2020 2020 2020 2020 2020 2020 2020 7473                ts
-00006b00: 7461 7274 202b 3d20 7375 6273 7461 636b  tart += substack
-00006b10: 5f6c 656e 0a20 2020 2020 2020 2020 2020  _len.           
-00006b20: 2020 2020 2023 2070 7269 6e74 2827 636f       # print('co
-00006b30: 7272 656c 6174 696f 6e20 646f 6e65 2061  rrelation done a
-00006b40: 6e64 2073 7461 636b 6564 2061 7420 7469  nd stacked at ti
-00006b50: 6d65 2025 7327 2025 2073 7472 2874 5f63  me %s' % str(t_c
-00006b60: 6f72 725b 6973 7461 636b 5d29 290a 0a20  orr[istack])).. 
-00006b70: 2020 2020 2020 2020 2020 2023 2072 656d             # rem
-00006b80: 6f76 6520 6162 6e6f 726d 616c 2064 6174  ove abnormal dat
-00006b90: 610a 2020 2020 2020 2020 2020 2020 616d  a.            am
-00006ba0: 706d 6178 203d 206e 702e 6d61 7828 735f  pmax = np.max(s_
-00006bb0: 636f 7272 2c20 6178 6973 3d31 290a 2020  corr, axis=1).  
-00006bc0: 2020 2020 2020 2020 2020 7469 6e64 7820            tindx 
-00006bd0: 3d20 6e70 2e77 6865 7265 2828 616d 706d  = np.where((ampm
-00006be0: 6178 203c 2032 3020 2a20 6e70 2e6d 6564  ax < 20 * np.med
-00006bf0: 6961 6e28 616d 706d 6178 2929 2026 2028  ian(ampmax)) & (
-00006c00: 616d 706d 6178 203e 2030 2929 5b30 5d0a  ampmax > 0))[0].
-00006c10: 2020 2020 2020 2020 2020 2020 735f 636f              s_co
-00006c20: 7272 203d 2073 5f63 6f72 725b 7469 6e64  rr = s_corr[tind
-00006c30: 782c 203a 5d0a 2020 2020 2020 2020 2020  x, :].          
-00006c40: 2020 745f 636f 7272 203d 2074 5f63 6f72    t_corr = t_cor
-00006c50: 725b 7469 6e64 785d 0a20 2020 2020 2020  r[tindx].       
-00006c60: 2020 2020 206e 5f63 6f72 7220 3d20 6e5f       n_corr = n_
-00006c70: 636f 7272 5b74 696e 6478 5d0a 0a20 2020  corr[tindx]..   
-00006c80: 2065 6c73 653a 0a20 2020 2020 2020 2023   else:.        #
-00006c90: 2061 7665 7261 6765 2064 6169 6c79 2063   average daily c
-00006ca0: 726f 7373 2063 6f72 7265 6c61 7469 6f6e  ross correlation
-00006cb0: 2066 756e 6374 696f 6e73 0a20 2020 2020   functions.     
-00006cc0: 2020 2061 6d70 6d61 7820 3d20 6e70 2e6d     ampmax = np.m
-00006cd0: 6178 2863 6f72 722c 2061 7869 733d 3129  ax(corr, axis=1)
-00006ce0: 0a20 2020 2020 2020 2074 696e 6478 203d  .        tindx =
-00006cf0: 206e 702e 7768 6572 6528 2861 6d70 6d61   np.where((ampma
-00006d00: 7820 3c20 3230 202a 206e 702e 6d65 6469  x < 20 * np.medi
-00006d10: 616e 2861 6d70 6d61 7829 2920 2620 2861  an(ampmax)) & (a
-00006d20: 6d70 6d61 7820 3e20 3029 295b 305d 0a20  mpmax > 0))[0]. 
-00006d30: 2020 2020 2020 206e 5f63 6f72 7220 3d20         n_corr = 
-00006d40: 6e77 696e 0a20 2020 2020 2020 2073 5f63  nwin.        s_c
-00006d50: 6f72 7220 3d20 6e70 2e7a 6572 6f73 284e  orr = np.zeros(N
-00006d60: 6666 742c 2064 7479 7065 3d6e 702e 666c  fft, dtype=np.fl
-00006d70: 6f61 7433 3229 0a20 2020 2020 2020 2074  oat32).        t
-00006d80: 5f63 6f72 7220 3d20 6461 7461 535f 745b  _corr = dataS_t[
-00006d90: 305d 0a20 2020 2020 2020 2063 7261 7020  0].        crap 
-00006da0: 3d20 6e70 2e7a 6572 6f73 284e 6666 742c  = np.zeros(Nfft,
-00006db0: 2064 7479 7065 3d6e 702e 636f 6d70 6c65   dtype=np.comple
-00006dc0: 7836 3429 0a20 2020 2020 2020 2063 7261  x64).        cra
-00006dd0: 705b 3a4e 6666 7432 5d20 3d20 6e70 2e6d  p[:Nfft2] = np.m
-00006de0: 6561 6e28 636f 7272 5b74 696e 6478 5d2c  ean(corr[tindx],
-00006df0: 2061 7869 733d 3029 0a20 2020 2020 2020   axis=0).       
-00006e00: 2063 7261 705b 3a4e 6666 7432 5d20 3d20   crap[:Nfft2] = 
-00006e10: 6372 6170 5b3a 4e66 6674 325d 202d 206e  crap[:Nfft2] - n
-00006e20: 702e 6d65 616e 2863 7261 705b 3a4e 6666  p.mean(crap[:Nff
-00006e30: 7432 5d2c 2061 7869 733d 3029 0a20 2020  t2], axis=0).   
-00006e40: 2020 2020 2063 7261 705b 2d28 4e66 6674       crap[-(Nfft
-00006e50: 3229 202b 2031 203a 5d20 3d20 6e70 2e66  2) + 1 :] = np.f
-00006e60: 6c69 7028 6e70 2e63 6f6e 6a28 6372 6170  lip(np.conj(crap
-00006e70: 5b31 3a28 4e66 6674 3229 5d29 2c20 6178  [1:(Nfft2)]), ax
-00006e80: 6973 3d30 290a 2020 2020 2020 2020 735f  is=0).        s_
-00006e90: 636f 7272 203d 206e 702e 7265 616c 286e  corr = np.real(n
-00006ea0: 702e 6666 742e 6966 6674 7368 6966 7428  p.fft.ifftshift(
-00006eb0: 7363 6970 792e 6666 7470 6163 6b2e 6966  scipy.fftpack.if
-00006ec0: 6674 2863 7261 702c 204e 6666 742c 2061  ft(crap, Nfft, a
-00006ed0: 7869 733d 3029 2929 0a0a 2020 2020 2320  xis=0)))..    # 
-00006ee0: 7472 696d 2074 6865 2043 4346 7320 696e  trim the CCFs in
-00006ef0: 205b 2d6d 6178 6c61 6720 6d61 786c 6167   [-maxlag maxlag
-00006f00: 5d0a 2020 2020 7420 3d20 6e70 2e61 7261  ].    t = np.ara
-00006f10: 6e67 6528 2d4e 6666 7432 202b 2031 2c20  nge(-Nfft2 + 1, 
-00006f20: 4e66 6674 3229 202a 2064 740a 2020 2020  Nfft2) * dt.    
-00006f30: 696e 6420 3d20 6e70 2e77 6865 7265 286e  ind = np.where(n
-00006f40: 702e 6162 7328 7429 203c 3d20 6d61 786c  p.abs(t) <= maxl
-00006f50: 6167 295b 305d 0a20 2020 2069 6620 735f  ag)[0].    if s_
-00006f60: 636f 7272 2e6e 6469 6d20 3d3d 2031 3a0a  corr.ndim == 1:.
-00006f70: 2020 2020 2020 2020 735f 636f 7272 203d          s_corr =
-00006f80: 2073 5f63 6f72 725b 696e 645d 0a20 2020   s_corr[ind].   
-00006f90: 2065 6c69 6620 735f 636f 7272 2e6e 6469   elif s_corr.ndi
-00006fa0: 6d20 3d3d 2032 3a0a 2020 2020 2020 2020  m == 2:.        
-00006fb0: 735f 636f 7272 203d 2073 5f63 6f72 725b  s_corr = s_corr[
-00006fc0: 3a2c 2069 6e64 5d0a 2020 2020 7265 7475  :, ind].    retu
-00006fd0: 726e 2073 5f63 6f72 722c 2074 5f63 6f72  rn s_corr, t_cor
-00006fe0: 722c 206e 5f63 6f72 720a 0a0a 6465 6620  r, n_corr...def 
-00006ff0: 636f 7272 656c 6174 655f 6e6f 6e6c 696e  correlate_nonlin
-00007000: 6561 725f 7374 6163 6b28 6666 7431 5f73  ear_stack(fft1_s
-00007010: 6d6f 6f74 6865 645f 6162 732c 2066 6674  moothed_abs, fft
-00007020: 322c 2044 2c20 4e66 6674 2c20 6461 7461  2, D, Nfft, data
-00007030: 535f 7429 3a0a 2020 2020 2222 220a 2020  S_t):.    """.  
-00007040: 2020 7468 6973 2066 756e 6374 696f 6e20    this function 
-00007050: 646f 6573 2074 6865 2063 726f 7373 2d63  does the cross-c
-00007060: 6f72 7265 6c61 7469 6f6e 2069 6e20 6672  orrelation in fr
-00007070: 6571 2064 6f6d 6169 6e20 616e 6420 6861  eq domain and ha
-00007080: 7320 7468 6520 6f70 7469 6f6e 2074 6f20  s the option to 
-00007090: 6b65 6570 2073 7562 2d73 7461 636b 7320  keep sub-stacks 
-000070a0: 6f66 0a20 2020 2074 6865 2063 726f 7373  of.    the cross
-000070b0: 2d63 6f72 7265 6c61 7469 6f6e 2069 6620  -correlation if 
-000070c0: 6e65 6564 6564 2e20 6974 2074 616b 6573  needed. it takes
-000070d0: 2061 6476 616e 7461 6765 206f 6620 7468   advantage of th
-000070e0: 6520 6c69 6e65 6172 2072 656c 6174 696f  e linear relatio
-000070f0: 6e73 6869 7020 6f66 2069 6666 742c 2073  nship of ifft, s
-00007100: 6f20 7468 6174 0a20 2020 2073 7461 636b  o that.    stack
-00007110: 696e 6720 6973 2070 6572 666f 726d 6564  ing is performed
-00007120: 2069 6e20 7370 6563 7472 756d 2064 6f6d   in spectrum dom
-00007130: 6169 6e20 6669 7273 7420 746f 2072 6564  ain first to red
-00007140: 7563 6520 7468 6520 746f 7461 6c20 6e75  uce the total nu
-00007150: 6d62 6572 206f 6620 6966 6674 2e20 2875  mber of ifft. (u
-00007160: 7365 6420 696e 2053 3129 0a20 2020 2050  sed in S1).    P
-00007170: 4152 414d 4554 4552 533a 0a20 2020 202d  ARAMETERS:.    -
-00007180: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007190: 2d2d 2d2d 0a20 2020 2066 6674 315f 736d  ----.    fft1_sm
-000071a0: 6f6f 7468 6564 5f61 6273 3a20 736d 6f6f  oothed_abs: smoo
-000071b0: 7468 6564 2070 6f77 6572 2073 7065 6374  thed power spect
-000071c0: 7261 6c20 6465 6e73 6974 7920 6f66 2074  ral density of t
-000071d0: 6865 2046 4654 2066 6f72 2074 6865 2073  he FFT for the s
-000071e0: 6f75 7263 6520 7374 6174 696f 6e0a 2020  ource station.  
-000071f0: 2020 6666 7432 3a20 7261 7720 4646 5420    fft2: raw FFT 
-00007200: 7370 6563 7472 756d 206f 6620 7468 6520  spectrum of the 
-00007210: 7265 6365 6976 6572 2073 7461 7469 6f6e  receiver station
-00007220: 0a20 2020 2044 3a20 6469 6374 696f 6e61  .    D: dictiona
-00007230: 7279 2063 6f6e 7461 696e 696e 6720 666f  ry containing fo
-00007240: 6c6c 6f77 696e 6720 7061 7261 6d65 7465  llowing paramete
-00007250: 7273 3a0a 2020 2020 2020 2020 6d61 786c  rs:.        maxl
-00007260: 6167 3a20 206d 6178 696d 756d 206c 6167  ag:  maximum lag
-00007270: 7320 746f 206b 6565 7020 696e 2074 6865  s to keep in the
-00007280: 2063 726f 7373 2063 6f72 7265 6c61 7469   cross correlati
-00007290: 6f6e 0a20 2020 2020 2020 2064 743a 2020  on.        dt:  
-000072a0: 2020 2020 7361 6d70 6c69 6e67 2072 6174      sampling rat
-000072b0: 6520 2869 6e20 7329 0a20 2020 2020 2020  e (in s).       
-000072c0: 206e 7769 6e3a 2020 2020 6e75 6d62 6572   nwin:    number
-000072d0: 206f 6620 7365 676d 656e 7473 2069 6e20   of segments in 
-000072e0: 7468 6520 3244 206d 6174 7269 780a 2020  the 2D matrix.  
-000072f0: 2020 2020 2020 6d65 7468 6f64 3a20 2063        method:  c
-00007300: 726f 7373 2d63 6f72 7265 6c61 7469 6f6e  ross-correlation
-00007310: 206d 6574 686f 6473 2073 656c 6563 7465   methods selecte
-00007320: 6420 6279 2074 6865 2075 7365 720a 2020  d by the user.  
-00007330: 2020 2020 2020 6672 6571 6d69 6e3a 206d        freqmin: m
-00007340: 696e 696d 756d 2066 7265 7175 656e 6379  inimum frequency
-00007350: 2028 487a 290a 2020 2020 2020 2020 6672   (Hz).        fr
-00007360: 6571 6d61 783a 206d 6178 696d 756d 2066  eqmax: maximum f
-00007370: 7265 7175 656e 6379 2028 487a 290a 2020  requency (Hz).  
-00007380: 2020 4e66 6674 3a20 2020 206e 756d 6265    Nfft:    numbe
-00007390: 7220 6f66 2066 7265 7175 656e 6379 2070  r of frequency p
-000073a0: 6f69 6e74 7320 666f 7220 6966 6674 0a20  oints for ifft. 
-000073b0: 2020 2064 6174 6153 5f74 3a20 6d61 7472     dataS_t: matr
-000073c0: 6978 206f 6620 6461 7465 7469 6d65 206f  ix of datetime o
-000073d0: 626a 6563 742e 0a20 2020 2052 4554 5552  bject..    RETUR
-000073e0: 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  NS:.    --------
-000073f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-00007400: 2020 735f 636f 7272 3a20 3144 206f 7220    s_corr: 1D or 
-00007410: 3244 206d 6174 7269 7820 6f66 2074 6865  2D matrix of the
-00007420: 2061 7665 7261 6765 6420 6f72 2073 7562   averaged or sub
-00007430: 2d73 7461 636b 7320 6f66 2063 726f 7373  -stacks of cross
-00007440: 2d63 6f72 7265 6c61 7469 6f6e 2066 756e  -correlation fun
-00007450: 6374 696f 6e73 2069 6e20 7469 6d65 2064  ctions in time d
-00007460: 6f6d 6169 6e0a 2020 2020 745f 636f 7272  omain.    t_corr
-00007470: 3a20 7469 6d65 7374 616d 7020 666f 7220  : timestamp for 
-00007480: 6561 6368 2073 7562 2d73 7461 636b 206f  each sub-stack o
-00007490: 7220 6176 6572 6167 6564 2066 756e 6374  r averaged funct
-000074a0: 696f 6e0a 2020 2020 6e5f 636f 7272 3a20  ion.    n_corr: 
-000074b0: 6e75 6d62 6572 206f 6620 696e 636c 7564  number of includ
-000074c0: 6564 2073 6567 6d65 6e74 7320 666f 7220  ed segments for 
-000074d0: 6561 6368 2073 7562 2d73 7461 636b 206f  each sub-stack o
-000074e0: 7220 6176 6572 6167 6564 2066 756e 6374  r averaged funct
-000074f0: 696f 6e0a 2020 2020 2222 220a 2020 2020  ion.    """.    
-00007500: 2320 2d2d 2d2d 6c6f 6164 2070 6172 616d  # ----load param
-00007510: 7465 7273 2d2d 2d2d 0a20 2020 2064 7420  ters----.    dt 
-00007520: 3d20 445b 2264 7422 5d0a 2020 2020 6d61  = D["dt"].    ma
-00007530: 786c 6167 203d 2044 5b22 6d61 786c 6167  xlag = D["maxlag
-00007540: 225d 0a20 2020 206d 6574 686f 6420 3d20  "].    method = 
-00007550: 445b 2263 635f 6d65 7468 6f64 225d 0a20  D["cc_method"]. 
-00007560: 2020 2063 635f 6c65 6e20 3d20 445b 2263     cc_len = D["c
-00007570: 635f 6c65 6e22 5d0a 2020 2020 7375 6273  c_len"].    subs
-00007580: 7461 636b 203d 2044 5b22 7375 6273 7461  tack = D["substa
-00007590: 636b 225d 0a20 2020 2073 7461 636b 5f6d  ck"].    stack_m
-000075a0: 6574 686f 6420 3d20 445b 2273 7461 636b  ethod = D["stack
-000075b0: 5f6d 6574 686f 6422 5d0a 2020 2020 7375  _method"].    su
-000075c0: 6273 7461 636b 5f6c 656e 203d 2044 5b22  bstack_len = D["
-000075d0: 7375 6273 7461 636b 5f6c 656e 225d 0a20  substack_len"]. 
-000075e0: 2020 2073 6d6f 6f74 6873 7065 6374 5f4e     smoothspect_N
-000075f0: 203d 2044 5b22 736d 6f6f 7468 7370 6563   = D["smoothspec
-00007600: 745f 4e22 5d0a 0a20 2020 206e 7769 6e20  t_N"]..    nwin 
-00007610: 3d20 6666 7431 5f73 6d6f 6f74 6865 645f  = fft1_smoothed_
-00007620: 6162 732e 7368 6170 655b 305d 0a20 2020  abs.shape[0].   
-00007630: 204e 6666 7432 203d 2066 6674 315f 736d   Nfft2 = fft1_sm
-00007640: 6f6f 7468 6564 5f61 6273 2e73 6861 7065  oothed_abs.shape
-00007650: 5b31 5d0a 0a20 2020 2023 202d 2d2d 2d2d  [1]..    # -----
-00007660: 2d63 6f6e 7665 7274 2061 6c6c 2032 4420  -convert all 2D 
-00007670: 6172 7261 7973 2069 6e74 6f20 3144 2074  arrays into 1D t
-00007680: 6f20 7370 6565 6420 7570 2d2d 2d2d 2d2d  o speed up------
-00007690: 2d2d 0a20 2020 2063 6f72 7220 3d20 6e70  --.    corr = np
-000076a0: 2e7a 6572 6f73 286e 7769 6e20 2a20 4e66  .zeros(nwin * Nf
-000076b0: 6674 322c 2064 7479 7065 3d6e 702e 636f  ft2, dtype=np.co
-000076c0: 6d70 6c65 7836 3429 0a20 2020 2063 6f72  mplex64).    cor
-000076d0: 7220 3d20 6666 7431 5f73 6d6f 6f74 6865  r = fft1_smoothe
-000076e0: 645f 6162 732e 7265 7368 6170 6528 0a20  d_abs.reshape(. 
-000076f0: 2020 2020 2020 2066 6674 315f 736d 6f6f         fft1_smoo
-00007700: 7468 6564 5f61 6273 2e73 697a 652c 0a20  thed_abs.size,. 
-00007710: 2020 2029 202a 2066 6674 322e 7265 7368     ) * fft2.resh
-00007720: 6170 6528 0a20 2020 2020 2020 2066 6674  ape(.        fft
-00007730: 322e 7369 7a65 2c0a 2020 2020 290a 0a20  2.size,.    ).. 
-00007740: 2020 2023 206e 6f72 6d61 6c69 7a65 2062     # normalize b
-00007750: 7920 7265 6365 6976 6572 2073 7065 6374  y receiver spect
-00007760: 7261 6c20 666f 7220 636f 6865 7265 6e63  ral for coherenc
-00007770: 790a 2020 2020 6966 206d 6574 686f 6420  y.    if method 
-00007780: 3d3d 2022 636f 6865 7265 6e63 7922 3a0a  == "coherency":.
-00007790: 2020 2020 2020 2020 7465 6d70 203d 206d          temp = m
-000077a0: 6f76 696e 675f 6176 6528 0a20 2020 2020  oving_ave(.     
-000077b0: 2020 2020 2020 206e 702e 6162 7328 0a20         np.abs(. 
-000077c0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000077d0: 6674 322e 7265 7368 6170 6528 0a20 2020  ft2.reshape(.   
-000077e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077f0: 2066 6674 322e 7369 7a65 2c0a 2020 2020   fft2.size,.    
-00007800: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00007810: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-00007820: 2020 2020 2020 2020 2073 6d6f 6f74 6873           smooths
-00007830: 7065 6374 5f4e 2c0a 2020 2020 2020 2020  pect_N,.        
-00007840: 290a 2020 2020 2020 2020 636f 7272 202f  ).        corr /
-00007850: 3d20 7465 6d70 0a20 2020 2063 6f72 7220  = temp.    corr 
-00007860: 3d20 636f 7272 2e72 6573 6861 7065 286e  = corr.reshape(n
-00007870: 7769 6e2c 204e 6666 7432 290a 0a20 2020  win, Nfft2)..   
-00007880: 2023 2074 7261 6e73 666f 726d 2062 6163   # transform bac
-00007890: 6b20 746f 2074 696d 6520 646f 6d61 696e  k to time domain
-000078a0: 2077 6176 6566 6f72 6d73 0a20 2020 2073   waveforms.    s
-000078b0: 5f63 6f72 7220 3d20 6e70 2e7a 6572 6f73  _corr = np.zeros
-000078c0: 2873 6861 7065 3d28 6e77 696e 2c20 4e66  (shape=(nwin, Nf
-000078d0: 6674 292c 2064 7479 7065 3d6e 702e 666c  ft), dtype=np.fl
-000078e0: 6f61 7433 3229 2020 2320 7374 6163 6b65  oat32)  # stacke
-000078f0: 6420 636f 7272 656c 6174 696f 6e0a 2020  d correlation.  
-00007900: 2020 616d 706d 6178 203d 206e 702e 7a65    ampmax = np.ze
-00007910: 726f 7328 6e77 696e 2c20 6474 7970 653d  ros(nwin, dtype=
-00007920: 6e70 2e66 6c6f 6174 3332 290a 2020 2020  np.float32).    
-00007930: 6e5f 636f 7272 203d 206e 702e 7a65 726f  n_corr = np.zero
-00007940: 7328 6e77 696e 2c20 6474 7970 653d 6e70  s(nwin, dtype=np
-00007950: 2e69 6e74 3136 2920 2023 206e 756d 6265  .int16)  # numbe
-00007960: 7220 6f66 2063 6f72 7265 6c61 7469 6f6e  r of correlation
-00007970: 7320 666f 7220 6561 6368 2073 7562 7374  s for each subst
-00007980: 6163 6b0a 2020 2020 745f 636f 7272 203d  ack.    t_corr =
-00007990: 2064 6174 6153 5f74 2020 2320 7469 6d65   dataS_t  # time
-000079a0: 7374 616d 700a 2020 2020 6372 6170 203d  stamp.    crap =
-000079b0: 206e 702e 7a65 726f 7328 4e66 6674 2c20   np.zeros(Nfft, 
-000079c0: 6474 7970 653d 6e70 2e63 6f6d 706c 6578  dtype=np.complex
-000079d0: 3634 290a 2020 2020 666f 7220 6920 696e  64).    for i in
-000079e0: 2072 616e 6765 286e 7769 6e29 3a0a 2020   range(nwin):.  
-000079f0: 2020 2020 2020 6e5f 636f 7272 5b69 5d20        n_corr[i] 
-00007a00: 3d20 310a 2020 2020 2020 2020 6372 6170  = 1.        crap
-00007a10: 5b3a 4e66 6674 325d 203d 2063 6f72 725b  [:Nfft2] = corr[
-00007a20: 692c 203a 5d0a 2020 2020 2020 2020 6372  i, :].        cr
-00007a30: 6170 5b3a 4e66 6674 325d 203d 2063 7261  ap[:Nfft2] = cra
-00007a40: 705b 3a4e 6666 7432 5d20 2d20 6e70 2e6d  p[:Nfft2] - np.m
-00007a50: 6561 6e28 6372 6170 5b3a 4e66 6674 325d  ean(crap[:Nfft2]
-00007a60: 2920 2023 2072 656d 6f76 6520 7468 6520  )  # remove the 
-00007a70: 6d65 616e 2069 6e20 6672 6571 2064 6f6d  mean in freq dom
-00007a80: 6169 6e20 2873 7069 6b65 2061 7420 743d  ain (spike at t=
-00007a90: 3029 0a20 2020 2020 2020 2063 7261 705b  0).        crap[
-00007aa0: 2d28 4e66 6674 3229 202b 2031 203a 5d20  -(Nfft2) + 1 :] 
-00007ab0: 3d20 6e70 2e66 6c69 7028 6e70 2e63 6f6e  = np.flip(np.con
-00007ac0: 6a28 6372 6170 5b31 3a28 4e66 6674 3229  j(crap[1:(Nfft2)
-00007ad0: 5d29 2c20 6178 6973 3d30 290a 2020 2020  ]), axis=0).    
-00007ae0: 2020 2020 6372 6170 5b30 5d20 3d20 636f      crap[0] = co
-00007af0: 6d70 6c65 7828 302c 2030 290a 2020 2020  mplex(0, 0).    
-00007b00: 2020 2020 735f 636f 7272 5b69 2c20 3a5d      s_corr[i, :]
-00007b10: 203d 206e 702e 7265 616c 286e 702e 6666   = np.real(np.ff
-00007b20: 742e 6966 6674 7368 6966 7428 7363 6970  t.ifftshift(scip
-00007b30: 792e 6666 7470 6163 6b2e 6966 6674 2863  y.fftpack.ifft(c
-00007b40: 7261 702c 204e 6666 742c 2061 7869 733d  rap, Nfft, axis=
-00007b50: 3029 2929 0a0a 2020 2020 6e73 5f63 6f72  0)))..    ns_cor
-00007b60: 7220 3d20 735f 636f 7272 0a20 2020 2066  r = s_corr.    f
-00007b70: 6f72 2069 6969 2069 6e20 7261 6e67 6528  or iii in range(
-00007b80: 6e73 5f63 6f72 722e 7368 6170 655b 305d  ns_corr.shape[0]
-00007b90: 293a 0a20 2020 2020 2020 206e 735f 636f  ):.        ns_co
-00007ba0: 7272 5b69 6969 5d20 2f3d 206e 702e 6d61  rr[iii] /= np.ma
-00007bb0: 7828 6e70 2e61 6273 286e 735f 636f 7272  x(np.abs(ns_corr
-00007bc0: 5b69 6969 5d29 290a 0a20 2020 2069 6620  [iii]))..    if 
-00007bd0: 7375 6273 7461 636b 3a0a 2020 2020 2020  substack:.      
-00007be0: 2020 6966 2073 7562 7374 6163 6b5f 6c65    if substack_le
-00007bf0: 6e20 3d3d 2063 635f 6c65 6e3a 0a20 2020  n == cc_len:.   
-00007c00: 2020 2020 2020 2020 2023 2072 656d 6f76           # remov
-00007c10: 6520 6162 6e6f 726d 616c 2064 6174 610a  e abnormal data.
-00007c20: 2020 2020 2020 2020 2020 2020 616d 706d              ampm
-00007c30: 6178 203d 206e 702e 6d61 7828 735f 636f  ax = np.max(s_co
-00007c40: 7272 2c20 6178 6973 3d31 290a 2020 2020  rr, axis=1).    
-00007c50: 2020 2020 2020 2020 7469 6e64 7820 3d20          tindx = 
-00007c60: 6e70 2e77 6865 7265 2828 616d 706d 6178  np.where((ampmax
-00007c70: 203c 2032 3020 2a20 6e70 2e6d 6564 6961   < 20 * np.media
-00007c80: 6e28 616d 706d 6178 2929 2026 2028 616d  n(ampmax)) & (am
-00007c90: 706d 6178 203e 2030 2929 5b30 5d0a 2020  pmax > 0))[0].  
-00007ca0: 2020 2020 2020 2020 2020 735f 636f 7272            s_corr
-00007cb0: 203d 2073 5f63 6f72 725b 7469 6e64 782c   = s_corr[tindx,
-00007cc0: 203a 5d0a 2020 2020 2020 2020 2020 2020   :].            
-00007cd0: 745f 636f 7272 203d 2074 5f63 6f72 725b  t_corr = t_corr[
-00007ce0: 7469 6e64 785d 0a20 2020 2020 2020 2020  tindx].         
-00007cf0: 2020 206e 5f63 6f72 7220 3d20 6e5f 636f     n_corr = n_co
-00007d00: 7272 5b74 696e 6478 5d0a 0a20 2020 2020  rr[tindx]..     
-00007d10: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00007d20: 2020 2020 2023 2067 6574 2074 696d 6520       # get time 
-00007d30: 696e 666f 726d 6174 696f 6e0a 2020 2020  information.    
-00007d40: 2020 2020 2020 2020 5474 6f74 616c 203d          Ttotal =
-00007d50: 2064 6174 6153 5f74 5b2d 315d 202d 2064   dataS_t[-1] - d
-00007d60: 6174 6153 5f74 5b30 5d20 2023 2074 6f74  ataS_t[0]  # tot
-00007d70: 616c 2064 7572 6174 696f 6e20 6f66 2077  al duration of w
-00007d80: 6861 7420 7765 2068 6176 6520 6e6f 770a  hat we have now.
-00007d90: 2020 2020 2020 2020 2020 2020 7473 7461              tsta
-00007da0: 7274 203d 2064 6174 6153 5f74 5b30 5d0a  rt = dataS_t[0].
-00007db0: 0a20 2020 2020 2020 2020 2020 206e 7374  .            nst
-00007dc0: 6163 6b20 3d20 696e 7428 6e70 2e72 6f75  ack = int(np.rou
-00007dd0: 6e64 2854 746f 7461 6c20 2f20 7375 6273  nd(Ttotal / subs
-00007de0: 7461 636b 5f6c 656e 2929 0a20 2020 2020  tack_len)).     
-00007df0: 2020 2020 2020 2061 6d70 6d61 7820 3d20         ampmax = 
-00007e00: 6e70 2e7a 6572 6f73 286e 7374 6163 6b2c  np.zeros(nstack,
-00007e10: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
-00007e20: 3229 0a20 2020 2020 2020 2020 2020 2073  2).            s
-00007e30: 5f63 6f72 7220 3d20 6e70 2e7a 6572 6f73  _corr = np.zeros
-00007e40: 2873 6861 7065 3d28 6e73 7461 636b 2c20  (shape=(nstack, 
-00007e50: 4e66 6674 292c 2064 7479 7065 3d6e 702e  Nfft), dtype=np.
-00007e60: 666c 6f61 7433 3229 0a20 2020 2020 2020  float32).       
-00007e70: 2020 2020 206e 5f63 6f72 7220 3d20 6e70       n_corr = np
-00007e80: 2e7a 6572 6f73 286e 7374 6163 6b2c 2064  .zeros(nstack, d
-00007e90: 7479 7065 3d6e 702e 696e 7429 0a20 2020  type=np.int).   
-00007ea0: 2020 2020 2020 2020 2074 5f63 6f72 7220           t_corr 
-00007eb0: 3d20 6e70 2e7a 6572 6f73 286e 7374 6163  = np.zeros(nstac
-00007ec0: 6b2c 2064 7479 7065 3d6e 702e 666c 6f61  k, dtype=np.floa
-00007ed0: 7429 0a20 2020 2020 2020 2020 2020 2063  t).            c
-00007ee0: 7261 7020 3d20 6e70 2e7a 6572 6f73 284e  rap = np.zeros(N
-00007ef0: 6666 742c 2064 7479 7065 3d6e 702e 636f  fft, dtype=np.co
-00007f00: 6d70 6c65 7836 3429 0a0a 2020 2020 2020  mplex64)..      
-00007f10: 2020 2020 2020 666f 7220 6973 7461 636b        for istack
-00007f20: 2069 6e20 7261 6e67 6528 6e73 7461 636b   in range(nstack
-00007f30: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00007f40: 2020 2023 2066 696e 6420 7468 6520 696e     # find the in
-00007f50: 6465 7865 7320 6f66 2061 6c6c 206f 6620  dexes of all of 
-00007f60: 7468 6520 7769 6e64 6f77 7320 7468 6174  the windows that
-00007f70: 2073 7461 7274 206f 7220 656e 6420 7769   start or end wi
-00007f80: 7468 696e 0a20 2020 2020 2020 2020 2020  thin.           
-00007f90: 2020 2020 2069 7469 6d65 203d 206e 702e       itime = np.
-00007fa0: 7768 6572 6528 2864 6174 6153 5f74 203e  where((dataS_t >
-00007fb0: 3d20 7473 7461 7274 2920 2620 2864 6174  = tstart) & (dat
-00007fc0: 6153 5f74 203c 2074 7374 6172 7420 2b20  aS_t < tstart + 
-00007fd0: 7375 6273 7461 636b 5f6c 656e 2929 5b30  substack_len))[0
-00007fe0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00007ff0: 2020 6966 206c 656e 2869 7469 6d65 2920    if len(itime) 
-00008000: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
-00008010: 2020 2020 2020 2020 2020 7473 7461 7274            tstart
-00008020: 202b 3d20 7375 6273 7461 636b 5f6c 656e   += substack_len
-00008030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008040: 2020 2020 2063 6f6e 7469 6e75 650a 0a20       continue.. 
-00008050: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00008060: 7261 705b 3a4e 6666 7432 5d20 3d20 6e70  rap[:Nfft2] = np
-00008070: 2e6d 6561 6e28 636f 7272 5b69 7469 6d65  .mean(corr[itime
-00008080: 2c20 3a5d 2c20 6178 6973 3d30 2920 2023  , :], axis=0)  #
-00008090: 206c 696e 6561 7220 6176 6572 6167 6520   linear average 
-000080a0: 6f66 2074 6865 2063 6f72 7265 6c61 7469  of the correlati
-000080b0: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
-000080c0: 2020 2063 7261 705b 3a4e 6666 7432 5d20     crap[:Nfft2] 
-000080d0: 3d20 6372 6170 5b3a 4e66 6674 325d 202d  = crap[:Nfft2] -
-000080e0: 206e 702e 6d65 616e 2863 7261 705b 3a4e   np.mean(crap[:N
-000080f0: 6666 7432 5d29 2020 2320 7265 6d6f 7665  fft2])  # remove
-00008100: 2074 6865 206d 6561 6e20 696e 2066 7265   the mean in fre
-00008110: 7120 646f 6d61 696e 2028 7370 696b 6520  q domain (spike 
-00008120: 6174 2074 3d30 290a 2020 2020 2020 2020  at t=0).        
-00008130: 2020 2020 2020 2020 6372 6170 5b2d 284e          crap[-(N
-00008140: 6666 7432 2920 2b20 3120 3a5d 203d 206e  fft2) + 1 :] = n
-00008150: 702e 666c 6970 286e 702e 636f 6e6a 2863  p.flip(np.conj(c
-00008160: 7261 705b 313a 284e 6666 7432 295d 292c  rap[1:(Nfft2)]),
-00008170: 2061 7869 733d 3029 0a20 2020 2020 2020   axis=0).       
-00008180: 2020 2020 2020 2020 2063 7261 705b 305d           crap[0]
-00008190: 203d 2063 6f6d 706c 6578 2830 2c20 3029   = complex(0, 0)
-000081a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000081b0: 2073 5f63 6f72 725b 6973 7461 636b 2c20   s_corr[istack, 
-000081c0: 3a5d 203d 206e 702e 7265 616c 286e 702e  :] = np.real(np.
-000081d0: 6666 742e 6966 6674 7368 6966 7428 7363  fft.ifftshift(sc
-000081e0: 6970 792e 6666 7470 6163 6b2e 6966 6674  ipy.fftpack.ifft
-000081f0: 2863 7261 702c 204e 6666 742c 2061 7869  (crap, Nfft, axi
-00008200: 733d 3029 2929 0a20 2020 2020 2020 2020  s=0))).         
-00008210: 2020 2020 2020 206e 5f63 6f72 725b 6973         n_corr[is
-00008220: 7461 636b 5d20 3d20 6c65 6e28 6974 696d  tack] = len(itim
-00008230: 6529 2020 2320 6e75 6d62 6572 206f 6620  e)  # number of 
-00008240: 7769 6e64 6f77 7320 7374 6163 6b73 0a20  windows stacks. 
-00008250: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00008260: 5f63 6f72 725b 6973 7461 636b 5d20 3d20  _corr[istack] = 
-00008270: 7473 7461 7274 2020 2320 7361 7665 2074  tstart  # save t
-00008280: 6865 2074 696d 6520 7374 616d 7073 0a20  he time stamps. 
-00008290: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000082a0: 7374 6172 7420 2b3d 2073 7562 7374 6163  start += substac
-000082b0: 6b5f 6c65 6e0a 2020 2020 2020 2020 2020  k_len.          
-000082c0: 2020 2020 2020 2320 7072 696e 7428 2763        # print('c
-000082d0: 6f72 7265 6c61 7469 6f6e 2064 6f6e 6520  orrelation done 
-000082e0: 616e 6420 7374 6163 6b65 6420 6174 2074  and stacked at t
-000082f0: 696d 6520 2573 2720 2520 7374 7228 745f  ime %s' % str(t_
-00008300: 636f 7272 5b69 7374 6163 6b5d 2929 0a0a  corr[istack]))..
-00008310: 2020 2020 2020 2020 2020 2020 2320 7265              # re
-00008320: 6d6f 7665 2061 626e 6f72 6d61 6c20 6461  move abnormal da
-00008330: 7461 0a20 2020 2020 2020 2020 2020 2061  ta.            a
-00008340: 6d70 6d61 7820 3d20 6e70 2e6d 6178 2873  mpmax = np.max(s
-00008350: 5f63 6f72 722c 2061 7869 733d 3129 0a20  _corr, axis=1). 
-00008360: 2020 2020 2020 2020 2020 2074 696e 6478             tindx
-00008370: 203d 206e 702e 7768 6572 6528 2861 6d70   = np.where((amp
-00008380: 6d61 7820 3c20 3230 202a 206e 702e 6d65  max < 20 * np.me
-00008390: 6469 616e 2861 6d70 6d61 7829 2920 2620  dian(ampmax)) & 
-000083a0: 2861 6d70 6d61 7820 3e20 3029 295b 305d  (ampmax > 0))[0]
-000083b0: 0a20 2020 2020 2020 2020 2020 2073 5f63  .            s_c
-000083c0: 6f72 7220 3d20 735f 636f 7272 5b74 696e  orr = s_corr[tin
-000083d0: 6478 2c20 3a5d 0a20 2020 2020 2020 2020  dx, :].         
-000083e0: 2020 2074 5f63 6f72 7220 3d20 745f 636f     t_corr = t_co
-000083f0: 7272 5b74 696e 6478 5d0a 2020 2020 2020  rr[tindx].      
-00008400: 2020 2020 2020 6e5f 636f 7272 203d 206e        n_corr = n
-00008410: 5f63 6f72 725b 7469 6e64 785d 0a0a 2020  _corr[tindx]..  
-00008420: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00008430: 2320 6176 6572 6167 6520 6461 696c 7920  # average daily 
-00008440: 6372 6f73 7320 636f 7272 656c 6174 696f  cross correlatio
-00008450: 6e20 6675 6e63 7469 6f6e 730a 2020 2020  n functions.    
-00008460: 2020 2020 6966 2073 7461 636b 5f6d 6574      if stack_met
-00008470: 686f 6420 3d3d 2053 7461 636b 4d65 7468  hod == StackMeth
-00008480: 6f64 2e4c 494e 4541 523a 0a20 2020 2020  od.LINEAR:.     
-00008490: 2020 2020 2020 2061 6d70 6d61 7820 3d20         ampmax = 
-000084a0: 6e70 2e6d 6178 2873 5f63 6f72 722c 2061  np.max(s_corr, a
-000084b0: 7869 733d 3129 0a20 2020 2020 2020 2020  xis=1).         
-000084c0: 2020 2074 696e 6478 203d 206e 702e 7768     tindx = np.wh
-000084d0: 6572 6528 2861 6d70 6d61 7820 3c20 3230  ere((ampmax < 20
-000084e0: 202a 206e 702e 6d65 6469 616e 2861 6d70   * np.median(amp
-000084f0: 6d61 7829 2920 2620 2861 6d70 6d61 7820  max)) & (ampmax 
-00008500: 3e20 3029 295b 305d 0a20 2020 2020 2020  > 0))[0].       
-00008510: 2020 2020 2073 5f63 6f72 7220 3d20 6e70       s_corr = np
-00008520: 2e6d 6561 6e28 735f 636f 7272 5b74 696e  .mean(s_corr[tin
-00008530: 6478 5d2c 2061 7869 733d 3029 0a20 2020  dx], axis=0).   
-00008540: 2020 2020 2020 2020 2074 5f63 6f72 7220           t_corr 
-00008550: 3d20 6461 7461 535f 745b 305d 0a20 2020  = dataS_t[0].   
-00008560: 2020 2020 2020 2020 206e 5f63 6f72 7220           n_corr 
-00008570: 3d20 6c65 6e28 7469 6e64 7829 0a20 2020  = len(tindx).   
-00008580: 2020 2020 2065 6c69 6620 7374 6163 6b5f       elif stack_
-00008590: 6d65 7468 6f64 203d 3d20 5374 6163 6b4d  method == StackM
-000085a0: 6574 686f 642e 524f 4255 5354 3a0a 2020  ethod.ROBUST:.  
-000085b0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-000085c0: 2e69 6e66 6f28 2264 6f20 726f 6275 7374  .info("do robust
-000085d0: 2073 7562 7374 6163 6b69 6e67 2229 0a20   substacking"). 
-000085e0: 2020 2020 2020 2020 2020 2073 5f63 6f72             s_cor
-000085f0: 7220 3d20 726f 6275 7374 5f73 7461 636b  r = robust_stack
-00008600: 2873 5f63 6f72 722c 2030 2e30 3031 290a  (s_corr, 0.001).
-00008610: 2020 2020 2020 2020 2020 2020 745f 636f              t_co
-00008620: 7272 203d 2064 6174 6153 5f74 5b30 5d0a  rr = dataS_t[0].
-00008630: 2020 2020 2020 2020 2020 2020 6e5f 636f              n_co
-00008640: 7272 203d 206e 7769 6e0a 2020 2020 2320  rr = nwin.    # 
-00008650: 2065 6c69 6620 7374 6163 6b5f 6d65 7468   elif stack_meth
-00008660: 6f64 203d 3d20 2773 656c 6563 7469 7665  od == 'selective
-00008670: 273a 0a20 2020 2023 2020 2020 2020 7072  ':.    #      pr
-00008680: 696e 7428 2764 6f20 7365 6c65 6374 6976  int('do selectiv
-00008690: 6520 7375 6273 7461 636b 696e 6727 290a  e substacking').
-000086a0: 2020 2020 2320 2020 2020 2073 5f63 6f72      #      s_cor
-000086b0: 7220 3d20 7365 6c65 6374 6976 655f 7374  r = selective_st
-000086c0: 6163 6b28 735f 636f 7272 2c30 2e30 3031  ack(s_corr,0.001
-000086d0: 290a 2020 2020 2320 2020 2020 2074 5f63  ).    #      t_c
-000086e0: 6f72 7220 3d20 6461 7461 535f 745b 305d  orr = dataS_t[0]
-000086f0: 0a20 2020 2023 2020 2020 2020 6e5f 636f  .    #      n_co
-00008700: 7272 203d 206e 7769 6e0a 0a20 2020 2023  rr = nwin..    #
-00008710: 2074 7269 6d20 7468 6520 4343 4673 2069   trim the CCFs i
-00008720: 6e20 5b2d 6d61 786c 6167 206d 6178 6c61  n [-maxlag maxla
-00008730: 675d 0a20 2020 2074 203d 206e 702e 6172  g].    t = np.ar
-00008740: 616e 6765 282d 4e66 6674 3220 2b20 312c  ange(-Nfft2 + 1,
-00008750: 204e 6666 7432 2920 2a20 6474 0a20 2020   Nfft2) * dt.   
-00008760: 2069 6e64 203d 206e 702e 7768 6572 6528   ind = np.where(
-00008770: 6e70 2e61 6273 2874 2920 3c3d 206d 6178  np.abs(t) <= max
-00008780: 6c61 6729 5b30 5d0a 2020 2020 6966 2073  lag)[0].    if s
-00008790: 5f63 6f72 722e 6e64 696d 203d 3d20 313a  _corr.ndim == 1:
-000087a0: 0a20 2020 2020 2020 2073 5f63 6f72 7220  .        s_corr 
-000087b0: 3d20 735f 636f 7272 5b69 6e64 5d0a 2020  = s_corr[ind].  
-000087c0: 2020 656c 6966 2073 5f63 6f72 722e 6e64    elif s_corr.nd
-000087d0: 696d 203d 3d20 323a 0a20 2020 2020 2020  im == 2:.       
-000087e0: 2073 5f63 6f72 7220 3d20 735f 636f 7272   s_corr = s_corr
-000087f0: 5b3a 2c20 696e 645d 0a20 2020 2072 6574  [:, ind].    ret
-00008800: 7572 6e20 735f 636f 7272 2c20 745f 636f  urn s_corr, t_co
-00008810: 7272 2c20 6e5f 636f 7272 2c20 6e73 5f63  rr, n_corr, ns_c
-00008820: 6f72 725b 3a2c 2069 6e64 5d0a 0a0a 6465  orr[:, ind]...de
-00008830: 6620 6363 5f70 6172 616d 6574 6572 7328  f cc_parameters(
-00008840: 6363 5f70 6172 612c 2063 6f6f 722c 2074  cc_para, coor, t
-00008850: 636f 7272 2c20 6e63 6f72 722c 2063 6f6d  corr, ncorr, com
-00008860: 7029 3a0a 2020 2020 2222 220a 2020 2020  p):.    """.    
-00008870: 7468 6973 2066 756e 6374 696f 6e20 6173  this function as
-00008880: 7365 6d62 6c65 7320 7468 6520 7061 7261  sembles the para
-00008890: 6d65 7465 7273 2066 6f72 2074 6865 2063  meters for the c
-000088a0: 6320 6675 6e63 7469 6f6e 2c20 7768 6963  c function, whic
-000088b0: 6820 6973 2075 7365 640a 2020 2020 7768  h is used.    wh
-000088c0: 656e 2077 7269 7469 6e67 2074 6865 6d20  en writing them 
-000088d0: 696e 746f 2041 5344 4620 6669 6c65 730a  into ASDF files.
-000088e0: 2020 2020 5041 5241 4d45 5445 5253 3a0a      PARAMETERS:.
-000088f0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
-00008900: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6363  ---------.    cc
-00008910: 5f70 6172 613a 2064 6963 7420 636f 6e74  _para: dict cont
-00008920: 6169 6e69 6e67 2070 6172 616d 6574 6572  aining parameter
-00008930: 7320 7573 6564 2069 6e20 7468 6520 6666  s used in the ff
-00008940: 745f 6363 2073 7465 700a 2020 2020 636f  t_cc step.    co
-00008950: 6f72 3a20 2020 2064 6963 7420 636f 6e74  or:    dict cont
-00008960: 6169 6e69 6e67 2063 6f6f 7264 696e 6174  aining coordinat
-00008970: 6573 2069 6e66 6f20 6f66 2074 6865 2073  es info of the s
-00008980: 6f75 7263 6520 616e 6420 7265 6365 6976  ource and receiv
-00008990: 6572 2073 7461 7469 6f6e 730a 2020 2020  er stations.    
-000089a0: 7463 6f72 723a 2020 2074 696d 6573 7461  tcorr:   timesta
-000089b0: 6d70 206d 6174 7269 780a 2020 2020 6e63  mp matrix.    nc
-000089c0: 6f72 723a 2020 206d 6174 7269 7820 6f66  orr:   matrix of
-000089d0: 206e 756d 6265 7220 6f66 2067 6f6f 6420   number of good 
-000089e0: 7365 676d 656e 7473 2066 6f72 2065 6163  segments for eac
-000089f0: 6820 7375 622d 7374 6163 6b2f 6669 6e61  h sub-stack/fina
-00008a00: 6c20 7374 6163 6b0a 2020 2020 636f 6d70  l stack.    comp
-00008a10: 3a20 2020 2032 2063 6861 7261 6374 6572  :    2 character
-00008a20: 2073 7472 696e 6773 2066 6f72 2074 6865   strings for the
-00008a30: 2063 726f 7373 2063 6f72 7265 6c61 7469   cross correlati
-00008a40: 6f6e 2063 6f6d 706f 6e65 6e74 0a20 2020  on component.   
-00008a50: 2052 4554 5552 4e53 3a0a 2020 2020 2d2d   RETURNS:.    --
-00008a60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008a70: 0a20 2020 2070 6172 616d 6574 6572 733a  .    parameters:
-00008a80: 2064 6963 7420 636f 6e74 6169 6e69 6e67   dict containing
-00008a90: 2061 626f 7665 2069 6e66 6f20 7573 6564   above info used
-00008aa0: 2066 6f72 206c 6174 6572 2073 7461 636b   for later stack
-00008ab0: 696e 672f 706c 6f74 7469 6e67 0a20 2020  ing/plotting.   
-00008ac0: 2022 2222 0a20 2020 206c 6174 5320 3d20   """.    latS = 
-00008ad0: 636f 6f72 5b22 6c61 7453 225d 0a20 2020  coor["latS"].   
-00008ae0: 206c 6f6e 5320 3d20 636f 6f72 5b22 6c6f   lonS = coor["lo
-00008af0: 6e53 225d 0a20 2020 206c 6174 5220 3d20  nS"].    latR = 
-00008b00: 636f 6f72 5b22 6c61 7452 225d 0a20 2020  coor["latR"].   
-00008b10: 206c 6f6e 5220 3d20 636f 6f72 5b22 6c6f   lonR = coor["lo
-00008b20: 6e52 225d 0a20 2020 2064 7420 3d20 6363  nR"].    dt = cc
-00008b30: 5f70 6172 615b 2264 7422 5d0a 2020 2020  _para["dt"].    
-00008b40: 6d61 786c 6167 203d 2063 635f 7061 7261  maxlag = cc_para
-00008b50: 5b22 6d61 786c 6167 225d 0a20 2020 2073  ["maxlag"].    s
-00008b60: 7562 7374 6163 6b20 3d20 6363 5f70 6172  ubstack = cc_par
-00008b70: 615b 2273 7562 7374 6163 6b22 5d0a 2020  a["substack"].  
-00008b80: 2020 6363 5f6d 6574 686f 6420 3d20 6363    cc_method = cc
-00008b90: 5f70 6172 615b 2263 635f 6d65 7468 6f64  _para["cc_method
-00008ba0: 225d 0a0a 2020 2020 6469 7374 2c20 617a  "]..    dist, az
-00008bb0: 692c 2062 617a 203d 206f 6273 7079 2e67  i, baz = obspy.g
-00008bc0: 656f 6465 7469 6373 2e62 6173 652e 6770  eodetics.base.gp
-00008bd0: 7332 6469 7374 5f61 7a69 6d75 7468 286c  s2dist_azimuth(l
-00008be0: 6174 532c 206c 6f6e 532c 206c 6174 522c  atS, lonS, latR,
-00008bf0: 206c 6f6e 5229 0a20 2020 2070 6172 616d   lonR).    param
-00008c00: 6574 6572 7320 3d20 7b0a 2020 2020 2020  eters = {.      
-00008c10: 2020 2264 7422 3a20 6474 2c0a 2020 2020    "dt": dt,.    
-00008c20: 2020 2020 226d 6178 6c61 6722 3a20 696e      "maxlag": in
-00008c30: 7428 6d61 786c 6167 292c 0a20 2020 2020  t(maxlag),.     
-00008c40: 2020 2022 6469 7374 223a 206e 702e 666c     "dist": np.fl
-00008c50: 6f61 7433 3228 6469 7374 202f 2031 3030  oat32(dist / 100
-00008c60: 3029 2c0a 2020 2020 2020 2020 2261 7a69  0),.        "azi
-00008c70: 223a 206e 702e 666c 6f61 7433 3228 617a  ": np.float32(az
-00008c80: 6929 2c0a 2020 2020 2020 2020 2262 617a  i),.        "baz
-00008c90: 223a 206e 702e 666c 6f61 7433 3228 6261  ": np.float32(ba
-00008ca0: 7a29 2c0a 2020 2020 2020 2020 226c 6f6e  z),.        "lon
-00008cb0: 5322 3a20 6e70 2e66 6c6f 6174 3332 286c  S": np.float32(l
-00008cc0: 6f6e 5329 2c0a 2020 2020 2020 2020 226c  onS),.        "l
-00008cd0: 6174 5322 3a20 6e70 2e66 6c6f 6174 3332  atS": np.float32
-00008ce0: 286c 6174 5329 2c0a 2020 2020 2020 2020  (latS),.        
-00008cf0: 226c 6f6e 5222 3a20 6e70 2e66 6c6f 6174  "lonR": np.float
-00008d00: 3332 286c 6f6e 5229 2c0a 2020 2020 2020  32(lonR),.      
-00008d10: 2020 226c 6174 5222 3a20 6e70 2e66 6c6f    "latR": np.flo
-00008d20: 6174 3332 286c 6174 5229 2c0a 2020 2020  at32(latR),.    
-00008d30: 2020 2020 226e 676f 6f64 223a 206e 636f      "ngood": nco
-00008d40: 7272 2c0a 2020 2020 2020 2020 2263 635f  rr,.        "cc_
-00008d50: 6d65 7468 6f64 223a 2063 635f 6d65 7468  method": cc_meth
-00008d60: 6f64 2c0a 2020 2020 2020 2020 2274 696d  od,.        "tim
-00008d70: 6522 3a20 7463 6f72 722c 0a20 2020 2020  e": tcorr,.     
-00008d80: 2020 2022 7375 6273 7461 636b 223a 2073     "substack": s
-00008d90: 7562 7374 6163 6b2c 0a20 2020 2020 2020  ubstack,.       
-00008da0: 2022 636f 6d70 223a 2063 6f6d 702c 0a20   "comp": comp,. 
-00008db0: 2020 207d 0a20 2020 2072 6574 7572 6e20     }.    return 
-00008dc0: 7061 7261 6d65 7465 7273 0a0a 0a64 6566  parameters...def
-00008dd0: 2073 7461 636b 696e 6728 6363 5f61 7272   stacking(cc_arr
-00008de0: 6179 2c20 6363 5f74 696d 652c 2063 635f  ay, cc_time, cc_
-00008df0: 6e67 6f6f 642c 2073 7461 636b 5f70 6172  ngood, stack_par
-00008e00: 6129 3a0a 2020 2020 2222 220a 2020 2020  a):.    """.    
-00008e10: 7468 6973 2066 756e 6374 696f 6e20 7374  this function st
-00008e20: 6163 6b73 2074 6865 2063 726f 7373 2063  acks the cross c
-00008e30: 6f72 7265 6c61 7469 6f6e 2064 6174 6120  orrelation data 
-00008e40: 6163 636f 7264 696e 6720 746f 2074 6865  according to the
-00008e50: 2075 7365 722d 6465 6669 6e65 6420 7375   user-defined su
-00008e60: 6273 7461 636b 5f6c 656e 2070 6172 616d  bstack_len param
-00008e70: 6574 6572 0a0a 2020 2020 5041 5241 4d45  eter..    PARAME
-00008e80: 5445 5253 3a0a 2020 2020 2d2d 2d2d 2d2d  TERS:.    ------
-00008e90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008ea0: 0a20 2020 2063 635f 6172 7261 793a 2032  .    cc_array: 2
-00008eb0: 4420 6e75 6d70 7920 666c 6f61 7433 3220  D numpy float32 
-00008ec0: 6d61 7472 6978 2063 6f6e 7461 696e 696e  matrix containin
-00008ed0: 6720 616c 6c20 7365 676d 656e 7465 6420  g all segmented 
-00008ee0: 6372 6f73 732d 636f 7272 656c 6174 696f  cross-correlatio
-00008ef0: 6e20 6461 7461 0a20 2020 2063 635f 7469  n data.    cc_ti
-00008f00: 6d65 3a20 2031 4420 6e75 6d70 7920 6172  me:  1D numpy ar
-00008f10: 7261 7920 6f66 2074 696d 6573 7461 6d70  ray of timestamp
-00008f20: 7320 666f 7220 6561 6368 2073 6567 6d65  s for each segme
-00008f30: 6e74 206f 6620 6363 5f61 7272 6179 0a20  nt of cc_array. 
-00008f40: 2020 2063 635f 6e67 6f6f 643a 2031 4420     cc_ngood: 1D 
-00008f50: 6e75 6d70 7920 696e 7431 3620 6d61 7472  numpy int16 matr
-00008f60: 6978 2073 686f 7769 6e67 2074 6865 206e  ix showing the n
-00008f70: 756d 6265 7220 6f66 2073 6567 6d65 6e74  umber of segment
-00008f80: 7320 666f 7220 6561 6368 2073 7562 2d73  s for each sub-s
-00008f90: 7461 636b 2061 6e64 2f6f 7220 6675 6c6c  tack and/or full
-00008fa0: 2073 7461 636b 0a20 2020 2073 7461 636b   stack.    stack
-00008fb0: 5f70 6172 613a 2061 2064 6963 7420 636f  _para: a dict co
-00008fc0: 6e74 6169 6e69 6e67 2061 6c6c 2073 7461  ntaining all sta
-00008fd0: 636b 696e 6720 7061 7261 6d65 7465 7273  cking parameters
-00008fe0: 0a0a 2020 2020 5245 5455 524e 533a 0a20  ..    RETURNS:. 
-00008ff0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
-00009000: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6363  ---------.    cc
-00009010: 5f61 7272 6179 2c20 6363 5f6e 676f 6f64  _array, cc_ngood
-00009020: 2c20 6363 5f74 696d 653a 2073 616d 6520  , cc_time: same 
-00009030: 746f 2074 6865 2069 6e70 7574 2070 6172  to the input par
-00009040: 616d 6574 6572 7320 6275 7420 7769 7468  ameters but with
-00009050: 2061 626e 6f72 6d61 6c20 6372 6f73 732d   abnormal cross-
-00009060: 636f 7272 6561 6c74 696f 6e73 2072 656d  correaltions rem
-00009070: 6f76 6564 0a20 2020 2061 6c6c 7374 6163  oved.    allstac
-00009080: 6b73 313a 2031 4420 6d61 7472 6978 206f  ks1: 1D matrix o
-00009090: 6620 7374 6163 6b65 6420 6372 6f73 732d  f stacked cross-
-000090a0: 636f 7272 656c 6174 696f 6e20 6675 6e63  correlation func
-000090b0: 7469 6f6e 7320 6f76 6572 2061 6c6c 2074  tions over all t
-000090c0: 6865 2073 6567 6d65 6e74 730a 2020 2020  he segments.    
-000090d0: 6e73 7461 636b 733a 2020 2020 6e75 6d62  nstacks:    numb
-000090e0: 6572 206f 6620 6f76 6572 616c 6c20 7365  er of overall se
-000090f0: 676d 656e 7473 2066 6f72 2074 6865 2066  gments for the f
-00009100: 696e 616c 2073 7461 636b 730a 2020 2020  inal stacks.    
-00009110: 2222 220a 2020 2020 2320 6c6f 6164 2075  """.    # load u
-00009120: 7365 6675 6c20 7061 7261 6d65 7465 7273  seful parameters
-00009130: 2066 726f 6d20 6469 6374 0a20 2020 2073   from dict.    s
-00009140: 616d 705f 6672 6571 203d 2073 7461 636b  amp_freq = stack
-00009150: 5f70 6172 615b 2273 616d 705f 6672 6571  _para["samp_freq
-00009160: 225d 0a20 2020 2073 6d65 7468 6f64 203d  "].    smethod =
-00009170: 2073 7461 636b 5f70 6172 615b 2273 7461   stack_para["sta
-00009180: 636b 5f6d 6574 686f 6422 5d0a 2020 2020  ck_method"].    
-00009190: 6e70 7473 203d 2063 635f 6172 7261 792e  npts = cc_array.
-000091a0: 7368 6170 655b 315d 0a0a 2020 2020 2320  shape[1]..    # 
-000091b0: 7265 6d6f 7665 2061 626e 6f72 6d61 6c20  remove abnormal 
-000091c0: 6461 7461 0a20 2020 2061 6d70 6d61 7820  data.    ampmax 
-000091d0: 3d20 6e70 2e6d 6178 2863 635f 6172 7261  = np.max(cc_arra
-000091e0: 792c 2061 7869 733d 3129 0a20 2020 2074  y, axis=1).    t
-000091f0: 696e 6478 203d 206e 702e 7768 6572 6528  indx = np.where(
-00009200: 2861 6d70 6d61 7820 3c20 3230 202a 206e  (ampmax < 20 * n
-00009210: 702e 6d65 6469 616e 2861 6d70 6d61 7829  p.median(ampmax)
-00009220: 2920 2620 2861 6d70 6d61 7820 3e20 3029  ) & (ampmax > 0)
-00009230: 295b 305d 0a20 2020 2069 6620 6e6f 7420  )[0].    if not 
-00009240: 6c65 6e28 7469 6e64 7829 3a0a 2020 2020  len(tindx):.    
-00009250: 2020 2020 616c 6c73 7461 636b 7331 203d      allstacks1 =
-00009260: 205b 5d0a 2020 2020 2020 2020 616c 6c73   [].        alls
-00009270: 7461 636b 7332 203d 205b 5d0a 2020 2020  tacks2 = [].    
-00009280: 2020 2020 616c 6c73 7461 636b 7333 203d      allstacks3 =
-00009290: 205b 5d0a 2020 2020 2020 2020 6e73 7461   [].        nsta
-000092a0: 636b 7320 3d20 300a 2020 2020 2020 2020  cks = 0.        
-000092b0: 6363 5f61 7272 6179 203d 205b 5d0a 2020  cc_array = [].  
-000092c0: 2020 2020 2020 6363 5f6e 676f 6f64 203d        cc_ngood =
-000092d0: 205b 5d0a 2020 2020 2020 2020 6363 5f74   [].        cc_t
-000092e0: 696d 6520 3d20 5b5d 0a20 2020 2020 2020  ime = [].       
-000092f0: 2072 6574 7572 6e20 6363 5f61 7272 6179   return cc_array
-00009300: 2c20 6363 5f6e 676f 6f64 2c20 6363 5f74  , cc_ngood, cc_t
-00009310: 696d 652c 2061 6c6c 7374 6163 6b73 312c  ime, allstacks1,
-00009320: 2061 6c6c 7374 6163 6b73 322c 2061 6c6c   allstacks2, all
-00009330: 7374 6163 6b73 332c 206e 7374 6163 6b73  stacks3, nstacks
-00009340: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-00009350: 2020 2023 2072 656d 6f76 6520 6f6e 6573     # remove ones
-00009360: 2077 6974 6820 6261 6420 616d 706c 6974   with bad amplit
-00009370: 7564 650a 2020 2020 2020 2020 6363 5f61  ude.        cc_a
-00009380: 7272 6179 203d 2063 635f 6172 7261 795b  rray = cc_array[
-00009390: 7469 6e64 782c 203a 5d0a 2020 2020 2020  tindx, :].      
-000093a0: 2020 6363 5f74 696d 6520 3d20 6363 5f74    cc_time = cc_t
-000093b0: 696d 655b 7469 6e64 785d 0a20 2020 2020  ime[tindx].     
-000093c0: 2020 2063 635f 6e67 6f6f 6420 3d20 6363     cc_ngood = cc
-000093d0: 5f6e 676f 6f64 5b74 696e 6478 5d0a 0a20  _ngood[tindx].. 
-000093e0: 2020 2020 2020 2023 2064 6f20 7374 6163         # do stac
-000093f0: 6b69 6e67 0a20 2020 2020 2020 2061 6c6c  king.        all
-00009400: 7374 6163 6b73 3120 3d20 6e70 2e7a 6572  stacks1 = np.zer
-00009410: 6f73 286e 7074 732c 2064 7479 7065 3d6e  os(npts, dtype=n
-00009420: 702e 666c 6f61 7433 3229 0a20 2020 2020  p.float32).     
-00009430: 2020 2061 6c6c 7374 6163 6b73 3220 3d20     allstacks2 = 
-00009440: 6e70 2e7a 6572 6f73 286e 7074 732c 2064  np.zeros(npts, d
-00009450: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
-00009460: 0a20 2020 2020 2020 2061 6c6c 7374 6163  .        allstac
-00009470: 6b73 3320 3d20 6e70 2e7a 6572 6f73 286e  ks3 = np.zeros(n
-00009480: 7074 732c 2064 7479 7065 3d6e 702e 666c  pts, dtype=np.fl
-00009490: 6f61 7433 3229 0a0a 2020 2020 2020 2020  oat32)..        
-000094a0: 6966 2073 6d65 7468 6f64 203d 3d20 5374  if smethod == St
-000094b0: 6163 6b4d 6574 686f 642e 4c49 4e45 4152  ackMethod.LINEAR
-000094c0: 3a0a 2020 2020 2020 2020 2020 2020 616c  :.            al
-000094d0: 6c73 7461 636b 7331 203d 206e 702e 6d65  lstacks1 = np.me
-000094e0: 616e 2863 635f 6172 7261 792c 2061 7869  an(cc_array, axi
-000094f0: 733d 3029 0a20 2020 2020 2020 2065 6c69  s=0).        eli
-00009500: 6620 736d 6574 686f 6420 3d3d 2053 7461  f smethod == Sta
-00009510: 636b 4d65 7468 6f64 2e50 5753 3a0a 2020  ckMethod.PWS:.  
-00009520: 2020 2020 2020 2020 2020 616c 6c73 7461            allsta
-00009530: 636b 7331 203d 2070 7773 2863 635f 6172  cks1 = pws(cc_ar
-00009540: 7261 792c 2073 616d 705f 6672 6571 290a  ray, samp_freq).
-00009550: 2020 2020 2020 2020 656c 6966 2073 6d65          elif sme
-00009560: 7468 6f64 203d 3d20 5374 6163 6b4d 6574  thod == StackMet
-00009570: 686f 642e 524f 4255 5354 3a0a 2020 2020  hod.ROBUST:.    
-00009580: 2020 2020 2020 2020 616c 6c73 7461 636b          allstack
-00009590: 7331 2c20 772c 206e 7374 6570 203d 2072  s1, w, nstep = r
-000095a0: 6f62 7573 745f 7374 6163 6b28 6363 5f61  obust_stack(cc_a
-000095b0: 7272 6179 2c20 302e 3030 3129 0a20 2020  rray, 0.001).   
-000095c0: 2020 2020 2065 6c69 6620 736d 6574 686f       elif smetho
-000095d0: 6420 3d3d 2053 7461 636b 4d65 7468 6f64  d == StackMethod
-000095e0: 2e41 5554 4f5f 434f 5641 5249 414e 4345  .AUTO_COVARIANCE
-000095f0: 3a0a 2020 2020 2020 2020 2020 2020 616c  :.            al
-00009600: 6c73 7461 636b 7331 203d 2061 6461 7074  lstacks1 = adapt
-00009610: 6976 655f 6669 6c74 6572 2863 635f 6172  ive_filter(cc_ar
-00009620: 7261 792c 2031 290a 2020 2020 2020 2020  ray, 1).        
-00009630: 656c 6966 2073 6d65 7468 6f64 203d 3d20  elif smethod == 
-00009640: 5374 6163 6b4d 6574 686f 642e 4e52 4f4f  StackMethod.NROO
-00009650: 543a 0a20 2020 2020 2020 2020 2020 2061  T:.            a
-00009660: 6c6c 7374 6163 6b73 3120 3d20 6e72 6f6f  llstacks1 = nroo
-00009670: 745f 7374 6163 6b28 6363 5f61 7272 6179  t_stack(cc_array
-00009680: 2c20 3229 0a20 2020 2020 2020 2065 6c69  , 2).        eli
-00009690: 6620 736d 6574 686f 6420 3d3d 2053 7461  f smethod == Sta
-000096a0: 636b 4d65 7468 6f64 2e41 4c4c 3a0a 2020  ckMethod.ALL:.  
-000096b0: 2020 2020 2020 2020 2020 616c 6c73 7461            allsta
-000096c0: 636b 7331 203d 206e 702e 6d65 616e 2863  cks1 = np.mean(c
-000096d0: 635f 6172 7261 792c 2061 7869 733d 3029  c_array, axis=0)
-000096e0: 0a20 2020 2020 2020 2020 2020 2061 6c6c  .            all
-000096f0: 7374 6163 6b73 3220 3d20 7077 7328 6363  stacks2 = pws(cc
-00009700: 5f61 7272 6179 2c20 7361 6d70 5f66 7265  _array, samp_fre
-00009710: 7129 0a20 2020 2020 2020 2020 2020 2061  q).            a
-00009720: 6c6c 7374 6163 6b73 332c 2077 2c20 6e73  llstacks3, w, ns
-00009730: 7465 7020 3d20 726f 6275 7374 5f73 7461  tep = robust_sta
-00009740: 636b 2863 635f 6172 7261 792c 2030 2e30  ck(cc_array, 0.0
-00009750: 3031 290a 2020 2020 2020 2020 6e73 7461  01).        nsta
-00009760: 636b 7320 3d20 6e70 2e73 756d 2863 635f  cks = np.sum(cc_
-00009770: 6e67 6f6f 6429 0a0a 2020 2020 2320 676f  ngood)..    # go
-00009780: 6f64 2074 6f20 7265 7475 726e 0a20 2020  od to return.   
-00009790: 2072 6574 7572 6e20 6363 5f61 7272 6179   return cc_array
-000097a0: 2c20 6363 5f6e 676f 6f64 2c20 6363 5f74  , cc_ngood, cc_t
-000097b0: 696d 652c 2061 6c6c 7374 6163 6b73 312c  ime, allstacks1,
-000097c0: 2061 6c6c 7374 6163 6b73 322c 2061 6c6c   allstacks2, all
-000097d0: 7374 6163 6b73 332c 206e 7374 6163 6b73  stacks3, nstacks
-000097e0: 0a0a 0a64 6566 2073 7461 636b 696e 675f  ...def stacking_
-000097f0: 726d 6128 6363 5f61 7272 6179 2c20 6363  rma(cc_array, cc
-00009800: 5f74 696d 652c 2063 635f 6e67 6f6f 642c  _time, cc_ngood,
-00009810: 2073 7461 636b 5f70 6172 6129 3a0a 2020   stack_para):.  
-00009820: 2020 2222 220a 2020 2020 7468 6973 2066    """.    this f
-00009830: 756e 6374 696f 6e20 7374 6163 6b73 2074  unction stacks t
-00009840: 6865 2063 726f 7373 2063 6f72 7265 6c61  he cross correla
-00009850: 7469 6f6e 2064 6174 6120 6163 636f 7264  tion data accord
-00009860: 696e 6720 746f 2074 6865 2075 7365 722d  ing to the user-
-00009870: 6465 6669 6e65 6420 7375 6273 7461 636b  defined substack
-00009880: 5f6c 656e 2070 6172 616d 6574 6572 0a20  _len parameter. 
-00009890: 2020 2050 4152 414d 4554 4552 533a 0a20     PARAMETERS:. 
-000098a0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
-000098b0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6363  ---------.    cc
-000098c0: 5f61 7272 6179 3a20 3244 206e 756d 7079  _array: 2D numpy
-000098d0: 2066 6c6f 6174 3332 206d 6174 7269 7820   float32 matrix 
-000098e0: 636f 6e74 6169 6e69 6e67 2061 6c6c 2073  containing all s
-000098f0: 6567 6d65 6e74 6564 2063 726f 7373 2d63  egmented cross-c
-00009900: 6f72 7265 6c61 7469 6f6e 2064 6174 610a  orrelation data.
-00009910: 2020 2020 6363 5f74 696d 653a 2020 3144      cc_time:  1D
-00009920: 206e 756d 7079 2061 7272 6179 206f 6620   numpy array of 
-00009930: 7469 6d65 7374 616d 7073 2066 6f72 2065  timestamps for e
-00009940: 6163 6820 7365 676d 656e 7420 6f66 2063  ach segment of c
-00009950: 635f 6172 7261 790a 2020 2020 6363 5f6e  c_array.    cc_n
-00009960: 676f 6f64 3a20 3144 206e 756d 7079 2069  good: 1D numpy i
-00009970: 6e74 3136 206d 6174 7269 7820 7368 6f77  nt16 matrix show
-00009980: 696e 6720 7468 6520 6e75 6d62 6572 206f  ing the number o
-00009990: 6620 7365 676d 656e 7473 2066 6f72 2065  f segments for e
-000099a0: 6163 6820 7375 622d 7374 6163 6b20 616e  ach sub-stack an
-000099b0: 642f 6f72 2066 756c 6c20 7374 6163 6b0a  d/or full stack.
-000099c0: 2020 2020 7374 6163 6b5f 7061 7261 3a20      stack_para: 
-000099d0: 6120 6469 6374 2063 6f6e 7461 696e 696e  a dict containin
-000099e0: 6720 616c 6c20 7374 6163 6b69 6e67 2070  g all stacking p
-000099f0: 6172 616d 6574 6572 730a 2020 2020 5245  arameters.    RE
-00009a00: 5455 524e 533a 0a20 2020 202d 2d2d 2d2d  TURNS:.    -----
-00009a10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009a20: 2d0a 2020 2020 6363 5f61 7272 6179 2c20  -.    cc_array, 
-00009a30: 6363 5f6e 676f 6f64 2c20 6363 5f74 696d  cc_ngood, cc_tim
-00009a40: 653a 2073 616d 6520 746f 2074 6865 2069  e: same to the i
-00009a50: 6e70 7574 2070 6172 616d 6574 6572 7320  nput parameters 
-00009a60: 6275 7420 7769 7468 2061 626e 6f72 6d61  but with abnorma
-00009a70: 6c20 6372 6f73 732d 636f 7272 6561 6c74  l cross-correalt
-00009a80: 696f 6e73 2072 656d 6f76 6564 0a20 2020  ions removed.   
-00009a90: 2061 6c6c 7374 6163 6b73 313a 2031 4420   allstacks1: 1D 
-00009aa0: 6d61 7472 6978 206f 6620 7374 6163 6b65  matrix of stacke
-00009ab0: 6420 6372 6f73 732d 636f 7272 656c 6174  d cross-correlat
-00009ac0: 696f 6e20 6675 6e63 7469 6f6e 7320 6f76  ion functions ov
-00009ad0: 6572 2061 6c6c 2074 6865 2073 6567 6d65  er all the segme
-00009ae0: 6e74 730a 2020 2020 6e73 7461 636b 733a  nts.    nstacks:
-00009af0: 2020 2020 6e75 6d62 6572 206f 6620 6f76      number of ov
-00009b00: 6572 616c 6c20 7365 676d 656e 7473 2066  erall segments f
-00009b10: 6f72 2074 6865 2066 696e 616c 2073 7461  or the final sta
-00009b20: 636b 730a 2020 2020 2222 220a 2020 2020  cks.    """.    
-00009b30: 2320 6c6f 6164 2075 7365 6675 6c20 7061  # load useful pa
-00009b40: 7261 6d65 7465 7273 2066 726f 6d20 6469  rameters from di
-00009b50: 6374 0a20 2020 2073 616d 705f 6672 6571  ct.    samp_freq
-00009b60: 203d 2073 7461 636b 5f70 6172 615b 2273   = stack_para["s
-00009b70: 616d 705f 6672 6571 225d 0a20 2020 2073  amp_freq"].    s
-00009b80: 6d65 7468 6f64 203d 2073 7461 636b 5f70  method = stack_p
-00009b90: 6172 615b 2273 7461 636b 5f6d 6574 686f  ara["stack_metho
-00009ba0: 6422 5d0a 2020 2020 726d 615f 7375 6273  d"].    rma_subs
-00009bb0: 7461 636b 203d 2073 7461 636b 5f70 6172  tack = stack_par
-00009bc0: 615b 2272 6d61 5f73 7562 7374 6163 6b22  a["rma_substack"
-00009bd0: 5d0a 2020 2020 726d 615f 7374 6570 203d  ].    rma_step =
-00009be0: 2073 7461 636b 5f70 6172 615b 2272 6d61   stack_para["rma
-00009bf0: 5f73 7465 7022 5d0a 2020 2020 7374 6172  _step"].    star
-00009c00: 745f 6461 7465 203d 2073 7461 636b 5f70  t_date = stack_p
-00009c10: 6172 615b 2273 7461 7274 5f64 6174 6522  ara["start_date"
-00009c20: 5d0a 2020 2020 656e 645f 6461 7465 203d  ].    end_date =
-00009c30: 2073 7461 636b 5f70 6172 615b 2265 6e64   stack_para["end
-00009c40: 5f64 6174 6522 5d0a 2020 2020 6e70 7473  _date"].    npts
-00009c50: 203d 2063 635f 6172 7261 792e 7368 6170   = cc_array.shap
-00009c60: 655b 315d 0a0a 2020 2020 2320 7265 6d6f  e[1]..    # remo
-00009c70: 7665 2061 626e 6f72 6d61 6c20 6461 7461  ve abnormal data
-00009c80: 0a20 2020 2061 6d70 6d61 7820 3d20 6e70  .    ampmax = np
-00009c90: 2e6d 6178 2863 635f 6172 7261 792c 2061  .max(cc_array, a
-00009ca0: 7869 733d 3129 0a20 2020 2074 696e 6478  xis=1).    tindx
-00009cb0: 203d 206e 702e 7768 6572 6528 2861 6d70   = np.where((amp
-00009cc0: 6d61 7820 3c20 3230 202a 206e 702e 6d65  max < 20 * np.me
-00009cd0: 6469 616e 2861 6d70 6d61 7829 2920 2620  dian(ampmax)) & 
-00009ce0: 2861 6d70 6d61 7820 3e20 3029 295b 305d  (ampmax > 0))[0]
-00009cf0: 0a20 2020 2069 6620 6e6f 7420 6c65 6e28  .    if not len(
-00009d00: 7469 6e64 7829 3a0a 2020 2020 2020 2020  tindx):.        
-00009d10: 616c 6c73 7461 636b 7331 203d 205b 5d0a  allstacks1 = [].
-00009d20: 2020 2020 2020 2020 616c 6c73 7461 636b          allstack
-00009d30: 7332 203d 205b 5d0a 2020 2020 2020 2020  s2 = [].        
-00009d40: 6e73 7461 636b 7320 3d20 300a 2020 2020  nstacks = 0.    
-00009d50: 2020 2020 6363 5f61 7272 6179 203d 205b      cc_array = [
-00009d60: 5d0a 2020 2020 2020 2020 6363 5f6e 676f  ].        cc_ngo
-00009d70: 6f64 203d 205b 5d0a 2020 2020 2020 2020  od = [].        
-00009d80: 6363 5f74 696d 6520 3d20 5b5d 0a20 2020  cc_time = [].   
-00009d90: 2020 2020 2072 6574 7572 6e20 6363 5f61       return cc_a
-00009da0: 7272 6179 2c20 6363 5f6e 676f 6f64 2c20  rray, cc_ngood, 
-00009db0: 6363 5f74 696d 652c 2061 6c6c 7374 6163  cc_time, allstac
-00009dc0: 6b73 312c 2061 6c6c 7374 6163 6b73 322c  ks1, allstacks2,
-00009dd0: 206e 7374 6163 6b73 0a20 2020 2065 6c73   nstacks.    els
-00009de0: 653a 0a20 2020 2020 2020 2023 2072 656d  e:.        # rem
-00009df0: 6f76 6520 6f6e 6573 2077 6974 6820 6261  ove ones with ba
-00009e00: 6420 616d 706c 6974 7564 650a 2020 2020  d amplitude.    
-00009e10: 2020 2020 6363 5f61 7272 6179 203d 2063      cc_array = c
-00009e20: 635f 6172 7261 795b 7469 6e64 782c 203a  c_array[tindx, :
-00009e30: 5d0a 2020 2020 2020 2020 6363 5f74 696d  ].        cc_tim
-00009e40: 6520 3d20 6363 5f74 696d 655b 7469 6e64  e = cc_time[tind
-00009e50: 785d 0a20 2020 2020 2020 2063 635f 6e67  x].        cc_ng
-00009e60: 6f6f 6420 3d20 6363 5f6e 676f 6f64 5b74  ood = cc_ngood[t
-00009e70: 696e 6478 5d0a 0a20 2020 2020 2020 2023  indx]..        #
-00009e80: 2064 6f20 7375 6273 7461 636b 730a 2020   do substacks.  
-00009e90: 2020 2020 2020 6966 2072 6d61 5f73 7562        if rma_sub
-00009ea0: 7374 6163 6b3a 0a20 2020 2020 2020 2020  stack:.         
-00009eb0: 2020 2074 7374 6172 7420 3d20 6f62 7370     tstart = obsp
-00009ec0: 792e 5554 4344 6174 6554 696d 6528 7374  y.UTCDateTime(st
-00009ed0: 6172 745f 6461 7465 2920 2d20 6f62 7370  art_date) - obsp
-00009ee0: 792e 5554 4344 6174 6554 696d 6528 3139  y.UTCDateTime(19
-00009ef0: 3730 2c20 312c 2031 290a 2020 2020 2020  70, 1, 1).      
-00009f00: 2020 2020 2020 7465 6e64 203d 206f 6273        tend = obs
-00009f10: 7079 2e55 5443 4461 7465 5469 6d65 2865  py.UTCDateTime(e
-00009f20: 6e64 5f64 6174 6529 202d 206f 6273 7079  nd_date) - obspy
-00009f30: 2e55 5443 4461 7465 5469 6d65 2831 3937  .UTCDateTime(197
-00009f40: 302c 2031 2c20 3129 0a20 2020 2020 2020  0, 1, 1).       
-00009f50: 2020 2020 2074 7469 6d65 203d 2074 7374       ttime = tst
-00009f60: 6172 740a 2020 2020 2020 2020 2020 2020  art.            
-00009f70: 6e73 7461 636b 203d 2069 6e74 286e 702e  nstack = int(np.
-00009f80: 726f 756e 6428 2874 656e 6420 2d20 7473  round((tend - ts
-00009f90: 7461 7274 2920 2f20 2872 6d61 5f73 7465  tart) / (rma_ste
-00009fa0: 7020 2a20 3336 3030 2929 290a 2020 2020  p * 3600))).    
-00009fb0: 2020 2020 2020 2020 6e63 635f 6172 7261          ncc_arra
-00009fc0: 7920 3d20 6e70 2e7a 6572 6f73 2873 6861  y = np.zeros(sha
-00009fd0: 7065 3d28 6e73 7461 636b 2c20 6e70 7473  pe=(nstack, npts
-00009fe0: 292c 2064 7479 7065 3d6e 702e 666c 6f61  ), dtype=np.floa
-00009ff0: 7433 3229 0a20 2020 2020 2020 2020 2020  t32).           
-0000a000: 206e 6363 5f74 696d 6520 3d20 6e70 2e7a   ncc_time = np.z
-0000a010: 6572 6f73 286e 7374 6163 6b2c 2064 7479  eros(nstack, dty
-0000a020: 7065 3d6e 702e 666c 6f61 7429 0a20 2020  pe=np.float).   
-0000a030: 2020 2020 2020 2020 206e 6363 5f6e 676f           ncc_ngo
-0000a040: 6f64 203d 206e 702e 7a65 726f 7328 6e73  od = np.zeros(ns
-0000a050: 7461 636b 2c20 6474 7970 653d 6e70 2e69  tack, dtype=np.i
-0000a060: 6e74 290a 0a20 2020 2020 2020 2020 2020  nt)..           
-0000a070: 2023 206c 6f6f 7020 7468 726f 7567 6820   # loop through 
-0000a080: 6561 6368 2074 696d 650a 2020 2020 2020  each time.      
-0000a090: 2020 2020 2020 666f 7220 6969 2069 6e20        for ii in 
-0000a0a0: 7261 6e67 6528 6e73 7461 636b 293a 0a20  range(nstack):. 
-0000a0b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000a0c0: 696e 6478 203d 206e 702e 7768 6572 6528  indx = np.where(
-0000a0d0: 2863 635f 7469 6d65 203e 3d20 7474 696d  (cc_time >= ttim
-0000a0e0: 6529 2026 2028 6363 5f74 696d 6520 3c20  e) & (cc_time < 
-0000a0f0: 7474 696d 6520 2b20 726d 615f 7375 6273  ttime + rma_subs
-0000a100: 7461 636b 202a 2033 3630 3029 295b 305d  tack * 3600))[0]
-0000a110: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000a120: 2020 2320 7768 656e 2074 6865 7265 2061    # when there a
-0000a130: 7265 2064 6174 6120 696e 2074 6865 2074  re data in the t
-0000a140: 696d 6520 7769 6e64 6f77 0a20 2020 2020  ime window.     
-0000a150: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-0000a160: 6e28 7369 6e64 7829 3a0a 2020 2020 2020  n(sindx):.      
-0000a170: 2020 2020 2020 2020 2020 2020 2020 6e63                nc
-0000a180: 635f 6172 7261 795b 6969 5d20 3d20 6e70  c_array[ii] = np
-0000a190: 2e6d 6561 6e28 6363 5f61 7272 6179 5b73  .mean(cc_array[s
-0000a1a0: 696e 6478 5d2c 2061 7869 733d 3029 0a20  indx], axis=0). 
-0000a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1c0: 2020 206e 6363 5f74 696d 655b 6969 5d20     ncc_time[ii] 
-0000a1d0: 3d20 7474 696d 650a 2020 2020 2020 2020  = ttime.        
-0000a1e0: 2020 2020 2020 2020 2020 2020 6e63 635f              ncc_
-0000a1f0: 6e67 6f6f 645b 6969 5d20 3d20 6e70 2e73  ngood[ii] = np.s
-0000a200: 756d 2863 635f 6e67 6f6f 645b 7369 6e64  um(cc_ngood[sind
-0000a210: 785d 2c20 6178 6973 3d30 290a 2020 2020  x], axis=0).    
-0000a220: 2020 2020 2020 2020 2020 2020 7474 696d              ttim
-0000a230: 6520 2b3d 2072 6d61 5f73 7465 7020 2a20  e += rma_step * 
-0000a240: 3336 3030 0a0a 2020 2020 2020 2020 2020  3600..          
-0000a250: 2020 2320 7265 6d6f 7665 2062 6164 206f    # remove bad o
-0000a260: 6e65 730a 2020 2020 2020 2020 2020 2020  nes.            
-0000a270: 7469 6e64 7820 3d20 6e70 2e77 6865 7265  tindx = np.where
-0000a280: 286e 6363 5f6e 676f 6f64 203e 2030 295b  (ncc_ngood > 0)[
-0000a290: 305d 0a20 2020 2020 2020 2020 2020 206e  0].            n
-0000a2a0: 6363 5f61 7272 6179 203d 206e 6363 5f61  cc_array = ncc_a
-0000a2b0: 7272 6179 5b74 696e 6478 5d0a 2020 2020  rray[tindx].    
-0000a2c0: 2020 2020 2020 2020 6e63 635f 7469 6d65          ncc_time
-0000a2d0: 203d 206e 6363 5f74 696d 655b 7469 6e64   = ncc_time[tind
-0000a2e0: 785d 0a20 2020 2020 2020 2020 2020 206e  x].            n
-0000a2f0: 6363 5f6e 676f 6f64 203d 206e 6363 5f6e  cc_ngood = ncc_n
-0000a300: 676f 6f64 5b74 696e 6478 5d0a 0a20 2020  good[tindx]..   
-0000a310: 2020 2020 2023 2064 6f20 7374 6163 6b69       # do stacki
-0000a320: 6e67 0a20 2020 2020 2020 2061 6c6c 7374  ng.        allst
-0000a330: 6163 6b73 3120 3d20 6e70 2e7a 6572 6f73  acks1 = np.zeros
-0000a340: 286e 7074 732c 2064 7479 7065 3d6e 702e  (npts, dtype=np.
-0000a350: 666c 6f61 7433 3229 0a20 2020 2020 2020  float32).       
-0000a360: 2061 6c6c 7374 6163 6b73 3220 3d20 6e70   allstacks2 = np
-0000a370: 2e7a 6572 6f73 286e 7074 732c 2064 7479  .zeros(npts, dty
-0000a380: 7065 3d6e 702e 666c 6f61 7433 3229 0a20  pe=np.float32). 
-0000a390: 2020 2020 2020 2061 6c6c 7374 6163 6b73         allstacks
-0000a3a0: 3320 3d20 6e70 2e7a 6572 6f73 286e 7074  3 = np.zeros(npt
-0000a3b0: 732c 2064 7479 7065 3d6e 702e 666c 6f61  s, dtype=np.floa
-0000a3c0: 7433 3229 0a20 2020 2020 2020 2061 6c6c  t32).        all
-0000a3d0: 7374 6163 6b73 3420 3d20 6e70 2e7a 6572  stacks4 = np.zer
-0000a3e0: 6f73 286e 7074 732c 2064 7479 7065 3d6e  os(npts, dtype=n
-0000a3f0: 702e 666c 6f61 7433 3229 0a0a 2020 2020  p.float32)..    
-0000a400: 2020 2020 6966 2073 6d65 7468 6f64 203d      if smethod =
-0000a410: 3d20 5374 6163 6b4d 6574 686f 642e 4c49  = StackMethod.LI
-0000a420: 4e45 4152 3a0a 2020 2020 2020 2020 2020  NEAR:.          
-0000a430: 2020 616c 6c73 7461 636b 7331 203d 206e    allstacks1 = n
-0000a440: 702e 6d65 616e 2863 635f 6172 7261 792c  p.mean(cc_array,
-0000a450: 2061 7869 733d 3029 0a20 2020 2020 2020   axis=0).       
-0000a460: 2065 6c69 6620 736d 6574 686f 6420 3d3d   elif smethod ==
-0000a470: 2053 7461 636b 4d65 7468 6f64 2e50 5753   StackMethod.PWS
-0000a480: 3a0a 2020 2020 2020 2020 2020 2020 616c  :.            al
-0000a490: 6c73 7461 636b 7331 203d 2070 7773 2863  lstacks1 = pws(c
-0000a4a0: 635f 6172 7261 792c 2073 616d 705f 6672  c_array, samp_fr
-0000a4b0: 6571 290a 2020 2020 2020 2020 656c 6966  eq).        elif
-0000a4c0: 2073 6d65 7468 6f64 203d 3d20 5374 6163   smethod == Stac
-0000a4d0: 6b4d 6574 686f 642e 524f 4255 5354 3a0a  kMethod.ROBUST:.
-0000a4e0: 2020 2020 2020 2020 2020 2020 280a 2020              (.  
-0000a4f0: 2020 2020 2020 2020 2020 2020 2020 616c                al
-0000a500: 6c73 7461 636b 7331 2c0a 2020 2020 2020  lstacks1,.      
-0000a510: 2020 2020 2020 2020 2020 772c 0a20 2020            w,.   
-0000a520: 2020 2020 2020 2020 2029 203d 2072 6f62           ) = rob
-0000a530: 7573 745f 7374 6163 6b28 6363 5f61 7272  ust_stack(cc_arr
-0000a540: 6179 2c20 302e 3030 3129 0a20 2020 2020  ay, 0.001).     
-0000a550: 2020 2065 6c69 6620 736d 6574 686f 6420     elif smethod 
-0000a560: 3d3d 2053 7461 636b 4d65 7468 6f64 2e53  == StackMethod.S
-0000a570: 454c 4543 5449 5645 3a0a 2020 2020 2020  ELECTIVE:.      
-0000a580: 2020 2020 2020 616c 6c73 7461 636b 7331        allstacks1
-0000a590: 203d 2073 656c 6563 7469 7665 5f73 7461   = selective_sta
-0000a5a0: 636b 2863 635f 6172 7261 792c 2030 2e30  ck(cc_array, 0.0
-0000a5b0: 3031 290a 2020 2020 2020 2020 656c 6966  01).        elif
-0000a5c0: 2073 6d65 7468 6f64 203d 3d20 5374 6163   smethod == Stac
-0000a5d0: 6b4d 6574 686f 642e 414c 4c3a 0a20 2020  kMethod.ALL:.   
-0000a5e0: 2020 2020 2020 2020 2061 6c6c 7374 6163           allstac
-0000a5f0: 6b73 3120 3d20 6e70 2e6d 6561 6e28 6363  ks1 = np.mean(cc
-0000a600: 5f61 7272 6179 2c20 6178 6973 3d30 290a  _array, axis=0).
-0000a610: 2020 2020 2020 2020 2020 2020 616c 6c73              alls
-0000a620: 7461 636b 7332 203d 2070 7773 2863 635f  tacks2 = pws(cc_
-0000a630: 6172 7261 792c 2073 616d 705f 6672 6571  array, samp_freq
-0000a640: 290a 2020 2020 2020 2020 2020 2020 616c  ).            al
-0000a650: 6c73 7461 636b 7333 203d 2072 6f62 7573  lstacks3 = robus
-0000a660: 745f 7374 6163 6b28 6363 5f61 7272 6179  t_stack(cc_array
-0000a670: 2c20 302e 3030 3129 0a20 2020 2020 2020  , 0.001).       
-0000a680: 2020 2020 2061 6c6c 7374 6163 6b73 3420       allstacks4 
-0000a690: 3d20 7365 6c65 6374 6976 655f 7374 6163  = selective_stac
-0000a6a0: 6b28 6363 5f61 7272 6179 2c20 302e 3030  k(cc_array, 0.00
-0000a6b0: 3129 0a20 2020 2020 2020 206e 7374 6163  1).        nstac
-0000a6c0: 6b73 203d 206e 702e 7375 6d28 6363 5f6e  ks = np.sum(cc_n
-0000a6d0: 676f 6f64 290a 0a20 2020 2023 2072 6570  good)..    # rep
-0000a6e0: 6c61 6365 2074 6865 2061 7272 6179 2066  lace the array f
-0000a6f0: 6f72 2073 7562 7374 6163 6b73 0a20 2020  or substacks.   
-0000a700: 2069 6620 726d 615f 7375 6273 7461 636b   if rma_substack
-0000a710: 3a0a 2020 2020 2020 2020 6363 5f61 7272  :.        cc_arr
-0000a720: 6179 203d 206e 6363 5f61 7272 6179 0a20  ay = ncc_array. 
-0000a730: 2020 2020 2020 2063 635f 7469 6d65 203d         cc_time =
-0000a740: 206e 6363 5f74 696d 650a 2020 2020 2020   ncc_time.      
-0000a750: 2020 6363 5f6e 676f 6f64 203d 206e 6363    cc_ngood = ncc
-0000a760: 5f6e 676f 6f64 0a0a 2020 2020 2320 676f  _ngood..    # go
-0000a770: 6f64 2074 6f20 7265 7475 726e 0a20 2020  od to return.   
-0000a780: 2072 6574 7572 6e20 280a 2020 2020 2020   return (.      
-0000a790: 2020 6363 5f61 7272 6179 2c0a 2020 2020    cc_array,.    
-0000a7a0: 2020 2020 6363 5f6e 676f 6f64 2c0a 2020      cc_ngood,.  
-0000a7b0: 2020 2020 2020 6363 5f74 696d 652c 0a20        cc_time,. 
-0000a7c0: 2020 2020 2020 2061 6c6c 7374 6163 6b73         allstacks
-0000a7d0: 312c 0a20 2020 2020 2020 2061 6c6c 7374  1,.        allst
-0000a7e0: 6163 6b73 322c 0a20 2020 2020 2020 2061  acks2,.        a
-0000a7f0: 6c6c 7374 6163 6b73 332c 0a20 2020 2020  llstacks3,.     
-0000a800: 2020 2061 6c6c 7374 6163 6b73 342c 0a20     allstacks4,. 
-0000a810: 2020 2020 2020 206e 7374 6163 6b73 2c0a         nstacks,.
-0000a820: 2020 2020 290a 0a0a 6465 6620 726f 7461      )...def rota
-0000a830: 7469 6f6e 2862 6967 7374 6163 6b2c 2070  tion(bigstack, p
-0000a840: 6172 616d 6574 6572 732c 206c 6f63 7329  arameters, locs)
-0000a850: 3a0a 2020 2020 2222 220a 2020 2020 7468  :.    """.    th
-0000a860: 6973 2066 756e 6374 696f 6e20 7472 616e  is function tran
-0000a870: 7366 6572 7320 7468 6520 4772 6565 6e27  sfers the Green'
-0000a880: 7320 7465 6e73 6f72 2066 726f 6d20 6120  s tensor from a 
-0000a890: 452d 4e2d 5a20 7379 7374 656d 2069 6e74  E-N-Z system int
-0000a8a0: 6f20 6120 522d 542d 5a20 6f6e 650a 0a20  o a R-T-Z one.. 
-0000a8b0: 2020 2050 4152 414d 4554 4552 533a 0a20     PARAMETERS:. 
-0000a8c0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
-0000a8d0: 2d2d 2d2d 2d2d 0a20 2020 2062 6967 7374  ------.    bigst
-0000a8e0: 6163 6b3a 2020 2039 2063 6f6d 706f 6e65  ack:   9 compone
-0000a8f0: 6e74 2047 7265 656e 2773 2074 656e 736f  nt Green's tenso
-0000a900: 7220 696e 2045 2d4e 2d5a 2073 7973 7465  r in E-N-Z syste
-0000a910: 6d0a 2020 2020 7061 7261 6d65 7465 7273  m.    parameters
-0000a920: 3a20 6469 6374 2063 6f6e 7461 696e 696e  : dict containin
-0000a930: 6720 616c 6c20 7061 7261 6d65 7465 7273  g all parameters
-0000a940: 2073 6176 6564 2069 6e20 4153 4446 2066   saved in ASDF f
-0000a950: 696c 650a 2020 2020 6c6f 6373 3a20 2020  ile.    locs:   
-0000a960: 2020 2020 6469 6374 2063 6f6e 7461 696e      dict contain
-0000a970: 696e 6720 7374 6174 696f 6e20 616e 676c  ing station angl
-0000a980: 6520 696e 666f 2066 6f72 2063 6f72 7265  e info for corre
-0000a990: 6374 696f 6e20 7075 7270 6f73 650a 2020  ction purpose.  
-0000a9a0: 2020 5245 5455 524e 533a 0a20 2020 202d    RETURNS:.    -
-0000a9b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000a9c0: 2d2d 0a20 2020 2074 636f 7272 3a20 3920  --.    tcorr: 9 
-0000a9d0: 636f 6d70 6f6e 656e 7420 4772 6565 6e27  component Green'
-0000a9e0: 7320 7465 6e73 6f72 2069 6e20 522d 542d  s tensor in R-T-
-0000a9f0: 5a20 7379 7374 656d 0a20 2020 2022 2222  Z system.    """
-0000aa00: 0a20 2020 2023 206c 6f61 6420 7061 7261  .    # load para
-0000aa10: 6d65 7465 7220 6469 630a 2020 2020 7069  meter dic.    pi
-0000aa20: 203d 206e 702e 7069 0a20 2020 2061 7a69   = np.pi.    azi
-0000aa30: 203d 2070 6172 616d 6574 6572 735b 2261   = parameters["a
-0000aa40: 7a69 225d 0a20 2020 2062 617a 203d 2070  zi"].    baz = p
-0000aa50: 6172 616d 6574 6572 735b 2262 617a 225d  arameters["baz"]
-0000aa60: 0a20 2020 206e 636f 6d70 2c20 6e70 7473  .    ncomp, npts
-0000aa70: 203d 2062 6967 7374 6163 6b2e 7368 6170   = bigstack.shap
-0000aa80: 650a 2020 2020 6966 206e 636f 6d70 203c  e.    if ncomp <
-0000aa90: 2039 3a0a 2020 2020 2020 2020 6c6f 6767   9:.        logg
-0000aaa0: 6572 2e64 6562 7567 2822 6372 6170 2064  er.debug("crap d
-0000aab0: 6964 206e 6f74 2067 6574 2065 6e6f 7567  id not get enoug
-0000aac0: 6820 636f 6d70 6f6e 656e 7473 2229 0a20  h components"). 
-0000aad0: 2020 2020 2020 2074 636f 7272 203d 205b         tcorr = [
-0000aae0: 5d0a 2020 2020 2020 2020 7265 7475 726e  ].        return
-0000aaf0: 2074 636f 7272 0a20 2020 2073 7461 5320   tcorr.    staS 
-0000ab00: 3d20 7061 7261 6d65 7465 7273 5b22 7374  = parameters["st
-0000ab10: 6174 696f 6e5f 736f 7572 6365 225d 0a20  ation_source"]. 
-0000ab20: 2020 2073 7461 5220 3d20 7061 7261 6d65     staR = parame
-0000ab30: 7465 7273 5b22 7374 6174 696f 6e5f 7265  ters["station_re
-0000ab40: 6365 6976 6572 225d 0a0a 2020 2020 6966  ceiver"]..    if
-0000ab50: 206c 656e 286c 6f63 7329 3a0a 2020 2020   len(locs):.    
-0000ab60: 2020 2020 7374 615f 6c69 7374 203d 206c      sta_list = l
-0000ab70: 6973 7428 6c6f 6373 5b22 7374 6174 696f  ist(locs["statio
-0000ab80: 6e22 5d29 0a20 2020 2020 2020 2061 6e67  n"]).        ang
-0000ab90: 6c65 7320 3d20 6c69 7374 286c 6f63 735b  les = list(locs[
-0000aba0: 2261 6e67 6c65 225d 290a 2020 2020 2020  "angle"]).      
-0000abb0: 2020 2320 6765 7420 7374 6174 696f 6e20    # get station 
-0000abc0: 696e 666f 2066 726f 6d20 7468 6520 6e61  info from the na
-0000abd0: 6d65 206f 6620 4153 4446 2066 696c 650a  me of ASDF file.
-0000abe0: 2020 2020 2020 2020 696e 6420 3d20 7374          ind = st
-0000abf0: 615f 6c69 7374 2e69 6e64 6578 2873 7461  a_list.index(sta
-0000ac00: 5329 0a20 2020 2020 2020 2061 636f 7272  S).        acorr
-0000ac10: 203d 2061 6e67 6c65 735b 696e 645d 0a20   = angles[ind]. 
-0000ac20: 2020 2020 2020 2069 6e64 203d 2073 7461         ind = sta
-0000ac30: 5f6c 6973 742e 696e 6465 7828 7374 6152  _list.index(staR
-0000ac40: 290a 2020 2020 2020 2020 6263 6f72 7220  ).        bcorr 
-0000ac50: 3d20 616e 676c 6573 5b69 6e64 5d0a 0a20  = angles[ind].. 
-0000ac60: 2020 2023 202d 2d2d 616e 676c 6573 2074     # ---angles t
-0000ac70: 6f20 6265 2063 6f72 7265 6374 6564 2d2d  o be corrected--
-0000ac80: 2d2d 0a20 2020 2069 6620 6c65 6e28 6c6f  --.    if len(lo
-0000ac90: 6373 293a 0a20 2020 2020 2020 2063 6f73  cs):.        cos
-0000aca0: 6120 3d20 6e70 2e63 6f73 2828 617a 6920  a = np.cos((azi 
-0000acb0: 2b20 6163 6f72 7229 202a 2070 6920 2f20  + acorr) * pi / 
-0000acc0: 3138 3029 0a20 2020 2020 2020 2073 696e  180).        sin
-0000acd0: 6120 3d20 6e70 2e73 696e 2828 617a 6920  a = np.sin((azi 
-0000ace0: 2b20 6163 6f72 7229 202a 2070 6920 2f20  + acorr) * pi / 
-0000acf0: 3138 3029 0a20 2020 2020 2020 2063 6f73  180).        cos
-0000ad00: 6220 3d20 6e70 2e63 6f73 2828 6261 7a20  b = np.cos((baz 
-0000ad10: 2b20 6263 6f72 7229 202a 2070 6920 2f20  + bcorr) * pi / 
-0000ad20: 3138 3029 0a20 2020 2020 2020 2073 696e  180).        sin
-0000ad30: 6220 3d20 6e70 2e73 696e 2828 6261 7a20  b = np.sin((baz 
-0000ad40: 2b20 6263 6f72 7229 202a 2070 6920 2f20  + bcorr) * pi / 
-0000ad50: 3138 3029 0a20 2020 2065 6c73 653a 0a20  180).    else:. 
-0000ad60: 2020 2020 2020 2063 6f73 6120 3d20 6e70         cosa = np
-0000ad70: 2e63 6f73 2861 7a69 202a 2070 6920 2f20  .cos(azi * pi / 
+00004dc0: 6e67 2866 6674 5f70 6172 613a 2043 6f6e  ng(fft_para: Con
+00004dd0: 6669 6750 6172 616d 6574 6572 732c 2064  figParameters, d
+00004de0: 6174 6153 293a 0a20 2020 2022 2222 0a20  ataS):.    """. 
+00004df0: 2020 2074 6869 7320 6675 6e63 7469 6f6e     this function
+00004e00: 2070 6572 666f 726d 7320 7469 6d65 2064   performs time d
+00004e10: 6f6d 6169 6e20 616e 6420 6672 6571 7565  omain and freque
+00004e20: 6e63 7920 646f 6d61 696e 206e 6f72 6d61  ncy domain norma
+00004e30: 6c69 7a61 7469 6f6e 2069 6620 6e65 6564  lization if need
+00004e40: 6564 2e20 696e 2072 6561 6c20 6361 7365  ed. in real case
+00004e50: 2c20 7765 2070 7265 6665 7220 7573 6520  , we prefer use 
+00004e60: 696e 636c 7564 650a 2020 2020 7468 6520  include.    the 
+00004e70: 6e6f 726d 616c 697a 6174 696f 6e20 696e  normalization in
+00004e80: 2074 6865 2063 726f 7373 2d63 6f72 7265   the cross-corre
+00004e90: 616c 7469 6f6e 2073 7465 7073 2062 7920  altion steps by 
+00004ea0: 7365 6c65 6374 696e 6720 636f 6865 7265  selecting cohere
+00004eb0: 6e63 7920 6f72 2064 6563 6f6e 0a20 2020  ncy or decon.   
+00004ec0: 2028 5072 6965 746f 2065 7420 616c 2c20   (Prieto et al, 
+00004ed0: 3230 3038 2c20 3230 3039 3b20 4465 6e6f  2008, 2009; Deno
+00004ee0: 6c6c 6520 6574 2061 6c2c 2032 3031 3329  lle et al, 2013)
+00004ef0: 0a20 2020 2050 4152 4d41 4554 4552 533a  .    PARMAETERS:
+00004f00: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
+00004f10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+00004f20: 2020 6666 745f 7061 7261 3a20 436f 6e66    fft_para: Conf
+00004f30: 6967 5061 7261 6d65 7465 7273 2063 6c61  igParameters cla
+00004f40: 7373 2063 6f6e 7461 696e 696e 6720 616c  ss containing al
+00004f50: 6c20 7573 6566 756c 2076 6172 6961 626c  l useful variabl
+00004f60: 6573 2075 7365 6420 666f 7220 6666 7420  es used for fft 
+00004f70: 616e 6420 6363 0a20 2020 2064 6174 6153  and cc.    dataS
+00004f80: 3a20 3244 206d 6174 7269 7820 6f66 2061  : 2D matrix of a
+00004f90: 6c6c 2073 6567 6d65 6e74 6564 206e 6f69  ll segmented noi
+00004fa0: 7365 2064 6174 610a 2020 2020 2320 4f55  se data.    # OU
+00004fb0: 5450 5554 2056 4152 4941 424c 4553 3a0a  TPUT VARIABLES:.
+00004fc0: 2020 2020 736f 7572 6365 5f77 6869 7465      source_white
+00004fd0: 3a20 3244 206d 6174 7269 7820 6f66 2064  : 2D matrix of d
+00004fe0: 6174 6120 7370 6563 7472 610a 2020 2020  ata spectra.    
+00004ff0: 2222 220a 2020 2020 2320 2d2d 2d2d 2d2d  """.    # ------
+00005000: 746f 206e 6f72 6d61 6c69 7a65 2069 6e20  to normalize in 
+00005010: 7469 6d65 206f 7220 6e6f 742d 2d2d 2d2d  time or not-----
+00005020: 2d0a 2020 2020 6966 2066 6674 5f70 6172  -.    if fft_par
+00005030: 612e 7469 6d65 5f6e 6f72 6d20 213d 2022  a.time_norm != "
+00005040: 6e6f 223a 0a20 2020 2020 2020 2069 6620  no":.        if 
+00005050: 6666 745f 7061 7261 2e74 696d 655f 6e6f  fft_para.time_no
+00005060: 726d 203d 3d20 226f 6e65 5f62 6974 223a  rm == "one_bit":
+00005070: 2020 2320 7369 676e 206e 6f72 6d61 6c69    # sign normali
+00005080: 7a61 7469 6f6e 0a20 2020 2020 2020 2020  zation.         
+00005090: 2020 2077 6869 7465 203d 206e 702e 7369     white = np.si
+000050a0: 676e 2864 6174 6153 290a 2020 2020 2020  gn(dataS).      
+000050b0: 2020 656c 6966 2066 6674 5f70 6172 612e    elif fft_para.
+000050c0: 7469 6d65 5f6e 6f72 6d20 3d3d 2022 726d  time_norm == "rm
+000050d0: 6122 3a20 2023 2072 756e 6e69 6e67 206d  a":  # running m
+000050e0: 6561 6e3a 206e 6f72 6d61 6c69 7a61 7469  ean: normalizati
+000050f0: 6f6e 206f 7665 7220 736d 6f6f 7468 6564  on over smoothed
+00005100: 2061 6273 6f6c 7574 6520 6176 6572 6167   absolute averag
+00005110: 650a 2020 2020 2020 2020 2020 2020 7768  e.            wh
+00005120: 6974 6520 3d20 6e70 2e7a 6572 6f73 2873  ite = np.zeros(s
+00005130: 6861 7065 3d64 6174 6153 2e73 6861 7065  hape=dataS.shape
+00005140: 2c20 6474 7970 653d 6461 7461 532e 6474  , dtype=dataS.dt
+00005150: 7970 6529 0a20 2020 2020 2020 2020 2020  ype).           
+00005160: 2066 6f72 206b 6b6b 2069 6e20 7261 6e67   for kkk in rang
+00005170: 6528 6461 7461 532e 7368 6170 655b 305d  e(dataS.shape[0]
+00005180: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00005190: 2020 2077 6869 7465 5b6b 6b6b 2c20 3a5d     white[kkk, :]
+000051a0: 203d 2064 6174 6153 5b6b 6b6b 2c20 3a5d   = dataS[kkk, :]
+000051b0: 202f 206d 6f76 696e 675f 6176 6528 6e70   / moving_ave(np
+000051c0: 2e61 6273 2864 6174 6153 5b6b 6b6b 2c20  .abs(dataS[kkk, 
+000051d0: 3a5d 292c 2066 6674 5f70 6172 612e 736d  :]), fft_para.sm
+000051e0: 6f6f 7468 5f4e 290a 0a20 2020 2065 6c73  ooth_N)..    els
+000051f0: 653a 2020 2320 646f 6e27 7420 6e6f 726d  e:  # don't norm
+00005200: 616c 697a 650a 2020 2020 2020 2020 7768  alize.        wh
+00005210: 6974 6520 3d20 6461 7461 530a 0a20 2020  ite = dataS..   
+00005220: 2023 202d 2d2d 2d2d 746f 2077 6869 7465   # -----to white
+00005230: 6e20 6f72 206e 6f74 2d2d 2d2d 2d2d 0a20  n or not------. 
+00005240: 2020 2069 6620 6666 745f 7061 7261 2e66     if fft_para.f
+00005250: 7265 715f 6e6f 726d 2021 3d20 226e 6f22  req_norm != "no"
+00005260: 3a0a 2020 2020 2020 2020 736f 7572 6365  :.        source
+00005270: 5f77 6869 7465 203d 2077 6869 7465 6e28  _white = whiten(
+00005280: 7768 6974 652c 2066 6674 5f70 6172 6129  white, fft_para)
+00005290: 2020 2320 7768 6974 656e 2061 6e64 2072    # whiten and r
+000052a0: 6574 7572 6e20 4646 540a 2020 2020 656c  eturn FFT.    el
+000052b0: 7365 3a0a 2020 2020 2020 2020 4e66 6674  se:.        Nfft
+000052c0: 203d 2069 6e74 286e 6578 745f 6661 7374   = int(next_fast
+000052d0: 5f6c 656e 2869 6e74 2864 6174 6153 2e73  _len(int(dataS.s
+000052e0: 6861 7065 5b31 5d29 2929 0a20 2020 2020  hape[1]))).     
+000052f0: 2020 2073 6f75 7263 655f 7768 6974 6520     source_white 
+00005300: 3d20 7363 6970 792e 6666 7470 6163 6b2e  = scipy.fftpack.
+00005310: 6666 7428 7768 6974 652c 204e 6666 742c  fft(white, Nfft,
+00005320: 2061 7869 733d 3129 2020 2320 7265 7475   axis=1)  # retu
+00005330: 726e 2046 4654 0a0a 2020 2020 7265 7475  rn FFT..    retu
+00005340: 726e 2073 6f75 7263 655f 7768 6974 650a  rn source_white.
+00005350: 0a0a 6465 6620 736d 6f6f 7468 5f73 6f75  ..def smooth_sou
+00005360: 7263 655f 7370 6563 7428 6363 5f70 6172  rce_spect(cc_par
+00005370: 612c 2066 6674 3129 3a0a 2020 2020 2222  a, fft1):.    ""
+00005380: 220a 2020 2020 7468 6973 2066 756e 6374  ".    this funct
+00005390: 696f 6e20 736d 6f6f 7468 6573 2061 6d70  ion smoothes amp
+000053a0: 6c69 7475 6465 2073 7065 6374 7275 6d20  litude spectrum 
+000053b0: 6f66 2074 6865 2032 4420 7370 6563 7472  of the 2D spectr
+000053c0: 616c 206d 6174 7269 782e 2028 7573 6564  al matrix. (used
+000053d0: 2069 6e20 5331 290a 2020 2020 5041 5241   in S1).    PARA
+000053e0: 4d45 5445 5253 3a0a 2020 2020 2d2d 2d2d  METERS:.    ----
+000053f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005400: 2d0a 2020 2020 6363 5f70 6172 613a 2064  -.    cc_para: d
+00005410: 6963 7469 6f6e 6172 7920 636f 6e74 6169  ictionary contai
+00005420: 6e69 6e67 2075 7365 6675 6c20 6363 2070  ning useful cc p
+00005430: 6172 616d 6574 6572 730a 2020 2020 6666  arameters.    ff
+00005440: 7431 3a20 2020 2073 6f75 7263 6520 7370  t1:    source sp
+00005450: 6563 7472 756d 206d 6174 7269 780a 0a20  ectrum matrix.. 
+00005460: 2020 2052 4554 5552 4e53 3a0a 2020 2020     RETURNS:.    
+00005470: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005480: 2d2d 2d2d 2d0a 2020 2020 7366 6674 313a  -----.    sfft1:
+00005490: 2063 6f6d 706c 6578 206e 756d 7079 2061   complex numpy a
+000054a0: 7272 6179 2077 6974 6820 6e6f 726d 616c  rray with normal
+000054b0: 697a 6564 2073 7065 6374 7275 6d0a 2020  ized spectrum.  
+000054c0: 2020 2222 220a 2020 2020 6363 5f6d 6574    """.    cc_met
+000054d0: 686f 6420 3d20 6363 5f70 6172 615b 2263  hod = cc_para["c
+000054e0: 635f 6d65 7468 6f64 225d 0a20 2020 2073  c_method"].    s
+000054f0: 6d6f 6f74 6873 7065 6374 5f4e 203d 2063  moothspect_N = c
+00005500: 635f 7061 7261 5b22 736d 6f6f 7468 7370  c_para["smoothsp
+00005510: 6563 745f 4e22 5d0a 0a20 2020 2069 6620  ect_N"]..    if 
+00005520: 6363 5f6d 6574 686f 6420 3d3d 2022 6465  cc_method == "de
+00005530: 636f 6e76 223a 0a20 2020 2020 2020 2023  conv":.        #
+00005540: 202d 2d2d 2d2d 6e6f 726d 616c 697a 6520   -----normalize 
+00005550: 7369 6e67 6c65 2d73 7461 7469 6f6e 2063  single-station c
+00005560: 6320 746f 207a 2063 6f6d 706f 6e65 6e74  c to z component
+00005570: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7465  -----.        te
+00005580: 6d70 203d 206d 6f76 696e 675f 6176 6528  mp = moving_ave(
+00005590: 6e70 2e61 6273 2866 6674 3129 2c20 736d  np.abs(fft1), sm
+000055a0: 6f6f 7468 7370 6563 745f 4e29 0a20 2020  oothspect_N).   
+000055b0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+000055c0: 2020 2020 2020 7366 6674 3120 3d20 6e70        sfft1 = np
+000055d0: 2e63 6f6e 6a28 6666 7431 2920 2f20 7465  .conj(fft1) / te
+000055e0: 6d70 2a2a 320a 2020 2020 2020 2020 6578  mp**2.        ex
+000055f0: 6365 7074 2045 7863 6570 7469 6f6e 3a0a  cept Exception:.
+00005600: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00005610: 6520 5661 6c75 6545 7272 6f72 2822 736d  e ValueError("sm
+00005620: 6f6f 7468 6564 2073 7065 6374 7275 6d20  oothed spectrum 
+00005630: 6861 7320 7a65 726f 2076 616c 7565 7322  has zero values"
+00005640: 290a 0a20 2020 2065 6c69 6620 6363 5f6d  )..    elif cc_m
+00005650: 6574 686f 6420 3d3d 2022 636f 6865 7265  ethod == "cohere
+00005660: 6e63 7922 3a0a 2020 2020 2020 2020 7465  ncy":.        te
+00005670: 6d70 203d 206d 6f76 696e 675f 6176 6528  mp = moving_ave(
+00005680: 6e70 2e61 6273 2866 6674 3129 2c20 736d  np.abs(fft1), sm
+00005690: 6f6f 7468 7370 6563 745f 4e29 0a20 2020  oothspect_N).   
+000056a0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+000056b0: 2020 2020 2020 7366 6674 3120 3d20 6e70        sfft1 = np
+000056c0: 2e63 6f6e 6a28 6666 7431 2920 2f20 7465  .conj(fft1) / te
+000056d0: 6d70 0a20 2020 2020 2020 2065 7863 6570  mp.        excep
+000056e0: 7420 4578 6365 7074 696f 6e3a 0a20 2020  t Exception:.   
+000056f0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+00005700: 616c 7565 4572 726f 7228 2273 6d6f 6f74  alueError("smoot
+00005710: 6865 6420 7370 6563 7472 756d 2068 6173  hed spectrum has
+00005720: 207a 6572 6f20 7661 6c75 6573 2229 0a0a   zero values")..
+00005730: 2020 2020 656c 6966 2063 635f 6d65 7468      elif cc_meth
+00005740: 6f64 203d 3d20 2278 636f 7272 223a 0a20  od == "xcorr":. 
+00005750: 2020 2020 2020 2073 6666 7431 203d 206e         sfft1 = n
+00005760: 702e 636f 6e6a 2866 6674 3129 0a0a 2020  p.conj(fft1)..  
+00005770: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00005780: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00005790: 2822 6e6f 2063 6f72 7265 6374 696f 6e20  ("no correction 
+000057a0: 636f 7272 656c 6174 696f 6e20 6d65 7468  correlation meth
+000057b0: 6f64 2069 7320 7365 6c65 6374 6564 2061  od is selected a
+000057c0: 7420 4c35 3922 290a 0a20 2020 2072 6574  t L59")..    ret
+000057d0: 7572 6e20 7366 6674 310a 0a0a 6465 6620  urn sfft1...def 
+000057e0: 636f 7272 656c 6174 6528 6666 7431 5f73  correlate(fft1_s
+000057f0: 6d6f 6f74 6865 645f 6162 732c 2066 6674  moothed_abs, fft
+00005800: 322c 2044 2c20 4e66 6674 2c20 6461 7461  2, D, Nfft, data
+00005810: 535f 7429 3a0a 2020 2020 2222 220a 2020  S_t):.    """.  
+00005820: 2020 7468 6973 2066 756e 6374 696f 6e20    this function 
+00005830: 646f 6573 2074 6865 2063 726f 7373 2d63  does the cross-c
+00005840: 6f72 7265 6c61 7469 6f6e 2069 6e20 6672  orrelation in fr
+00005850: 6571 2064 6f6d 6169 6e20 616e 6420 6861  eq domain and ha
+00005860: 7320 7468 6520 6f70 7469 6f6e 2074 6f20  s the option to 
+00005870: 6b65 6570 2073 7562 2d73 7461 636b 7320  keep sub-stacks 
+00005880: 6f66 0a20 2020 2074 6865 2063 726f 7373  of.    the cross
+00005890: 2d63 6f72 7265 6c61 7469 6f6e 2069 6620  -correlation if 
+000058a0: 6e65 6564 6564 2e20 6974 2074 616b 6573  needed. it takes
+000058b0: 2061 6476 616e 7461 6765 206f 6620 7468   advantage of th
+000058c0: 6520 6c69 6e65 6172 2072 656c 6174 696f  e linear relatio
+000058d0: 6e73 6869 7020 6f66 2069 6666 742c 2073  nship of ifft, s
+000058e0: 6f20 7468 6174 0a20 2020 2073 7461 636b  o that.    stack
+000058f0: 696e 6720 6973 2070 6572 666f 726d 6564  ing is performed
+00005900: 2069 6e20 7370 6563 7472 756d 2064 6f6d   in spectrum dom
+00005910: 6169 6e20 6669 7273 7420 746f 2072 6564  ain first to red
+00005920: 7563 6520 7468 6520 746f 7461 6c20 6e75  uce the total nu
+00005930: 6d62 6572 206f 6620 6966 6674 2e20 2875  mber of ifft. (u
+00005940: 7365 6420 696e 2053 3129 0a20 2020 2050  sed in S1).    P
+00005950: 4152 414d 4554 4552 533a 0a20 2020 202d  ARAMETERS:.    -
+00005960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005970: 2d2d 2d2d 0a20 2020 2066 6674 315f 736d  ----.    fft1_sm
+00005980: 6f6f 7468 6564 5f61 6273 3a20 736d 6f6f  oothed_abs: smoo
+00005990: 7468 6564 2070 6f77 6572 2073 7065 6374  thed power spect
+000059a0: 7261 6c20 6465 6e73 6974 7920 6f66 2074  ral density of t
+000059b0: 6865 2046 4654 2066 6f72 2074 6865 2073  he FFT for the s
+000059c0: 6f75 7263 6520 7374 6174 696f 6e0a 2020  ource station.  
+000059d0: 2020 6666 7432 3a20 7261 7720 4646 5420    fft2: raw FFT 
+000059e0: 7370 6563 7472 756d 206f 6620 7468 6520  spectrum of the 
+000059f0: 7265 6365 6976 6572 2073 7461 7469 6f6e  receiver station
+00005a00: 0a20 2020 2044 3a20 6469 6374 696f 6e61  .    D: dictiona
+00005a10: 7279 2063 6f6e 7461 696e 696e 6720 666f  ry containing fo
+00005a20: 6c6c 6f77 696e 6720 7061 7261 6d65 7465  llowing paramete
+00005a30: 7273 3a0a 2020 2020 2020 2020 6d61 786c  rs:.        maxl
+00005a40: 6167 3a20 206d 6178 696d 756d 206c 6167  ag:  maximum lag
+00005a50: 7320 746f 206b 6565 7020 696e 2074 6865  s to keep in the
+00005a60: 2063 726f 7373 2063 6f72 7265 6c61 7469   cross correlati
+00005a70: 6f6e 0a20 2020 2020 2020 2064 743a 2020  on.        dt:  
+00005a80: 2020 2020 7361 6d70 6c69 6e67 2072 6174      sampling rat
+00005a90: 6520 2869 6e20 7329 0a20 2020 2020 2020  e (in s).       
+00005aa0: 206e 7769 6e3a 2020 2020 6e75 6d62 6572   nwin:    number
+00005ab0: 206f 6620 7365 676d 656e 7473 2069 6e20   of segments in 
+00005ac0: 7468 6520 3244 206d 6174 7269 780a 2020  the 2D matrix.  
+00005ad0: 2020 2020 2020 6d65 7468 6f64 3a20 2063        method:  c
+00005ae0: 726f 7373 2d63 6f72 7265 6c61 7469 6f6e  ross-correlation
+00005af0: 206d 6574 686f 6473 2073 656c 6563 7465   methods selecte
+00005b00: 6420 6279 2074 6865 2075 7365 720a 2020  d by the user.  
+00005b10: 2020 2020 2020 6672 6571 6d69 6e3a 206d        freqmin: m
+00005b20: 696e 696d 756d 2066 7265 7175 656e 6379  inimum frequency
+00005b30: 2028 487a 290a 2020 2020 2020 2020 6672   (Hz).        fr
+00005b40: 6571 6d61 783a 206d 6178 696d 756d 2066  eqmax: maximum f
+00005b50: 7265 7175 656e 6379 2028 487a 290a 2020  requency (Hz).  
+00005b60: 2020 4e66 6674 3a20 2020 206e 756d 6265    Nfft:    numbe
+00005b70: 7220 6f66 2066 7265 7175 656e 6379 2070  r of frequency p
+00005b80: 6f69 6e74 7320 666f 7220 6966 6674 0a20  oints for ifft. 
+00005b90: 2020 2064 6174 6153 5f74 3a20 6d61 7472     dataS_t: matr
+00005ba0: 6978 206f 6620 6461 7465 7469 6d65 206f  ix of datetime o
+00005bb0: 626a 6563 742e 0a0a 2020 2020 5245 5455  bject...    RETU
+00005bc0: 524e 533a 0a20 2020 202d 2d2d 2d2d 2d2d  RNS:.    -------
+00005bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+00005be0: 2020 2073 5f63 6f72 723a 2031 4420 6f72     s_corr: 1D or
+00005bf0: 2032 4420 6d61 7472 6978 206f 6620 7468   2D matrix of th
+00005c00: 6520 6176 6572 6167 6564 206f 7220 7375  e averaged or su
+00005c10: 622d 7374 6163 6b73 206f 6620 6372 6f73  b-stacks of cros
+00005c20: 732d 636f 7272 656c 6174 696f 6e20 6675  s-correlation fu
+00005c30: 6e63 7469 6f6e 7320 696e 2074 696d 6520  nctions in time 
+00005c40: 646f 6d61 696e 0a20 2020 2074 5f63 6f72  domain.    t_cor
+00005c50: 723a 2074 696d 6573 7461 6d70 2066 6f72  r: timestamp for
+00005c60: 2065 6163 6820 7375 622d 7374 6163 6b20   each sub-stack 
+00005c70: 6f72 2061 7665 7261 6765 6420 6675 6e63  or averaged func
+00005c80: 7469 6f6e 0a20 2020 206e 5f63 6f72 723a  tion.    n_corr:
+00005c90: 206e 756d 6265 7220 6f66 2069 6e63 6c75   number of inclu
+00005ca0: 6465 6420 7365 676d 656e 7473 2066 6f72  ded segments for
+00005cb0: 2065 6163 6820 7375 622d 7374 6163 6b20   each sub-stack 
+00005cc0: 6f72 2061 7665 7261 6765 6420 6675 6e63  or averaged func
+00005cd0: 7469 6f6e 0a0a 2020 2020 4d4f 4449 4649  tion..    MODIFI
+00005ce0: 4341 5449 4f4e 533a 0a20 2020 202d 2d2d  CATIONS:.    ---
+00005cf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005d00: 2d2d 0a20 2020 206f 7574 7075 7420 7468  --.    output th
+00005d10: 6520 6c69 6e65 6172 2073 7461 636b 206f  e linear stack o
+00005d20: 6620 6561 6368 2074 696d 6520 6368 756e  f each time chun
+00005d30: 6b20 6576 656e 2077 6865 6e20 7375 6273  k even when subs
+00005d40: 7461 636b 2069 7320 7365 6c65 6374 6564  tack is selected
+00005d50: 2028 6279 2043 6865 6e67 7869 6e20 4041   (by Chengxin @A
+00005d60: 7567 3230 3230 290a 2020 2020 2222 220a  ug2020).    """.
+00005d70: 2020 2020 2320 2d2d 2d2d 6c6f 6164 2070      # ----load p
+00005d80: 6172 616d 7465 7273 2d2d 2d2d 0a20 2020  aramters----.   
+00005d90: 2064 7420 3d20 445b 2264 7422 5d0a 2020   dt = D["dt"].  
+00005da0: 2020 6d61 786c 6167 203d 2044 5b22 6d61    maxlag = D["ma
+00005db0: 786c 6167 225d 0a20 2020 206d 6574 686f  xlag"].    metho
+00005dc0: 6420 3d20 445b 2263 635f 6d65 7468 6f64  d = D["cc_method
+00005dd0: 225d 0a20 2020 2063 635f 6c65 6e20 3d20  "].    cc_len = 
+00005de0: 445b 2263 635f 6c65 6e22 5d0a 2020 2020  D["cc_len"].    
+00005df0: 7375 6273 7461 636b 203d 2044 5b22 7375  substack = D["su
+00005e00: 6273 7461 636b 225d 0a20 2020 2073 7562  bstack"].    sub
+00005e10: 7374 6163 6b5f 6c65 6e20 3d20 445b 2273  stack_len = D["s
+00005e20: 7562 7374 6163 6b5f 6c65 6e22 5d0a 2020  ubstack_len"].  
+00005e30: 2020 736d 6f6f 7468 7370 6563 745f 4e20    smoothspect_N 
+00005e40: 3d20 445b 2273 6d6f 6f74 6873 7065 6374  = D["smoothspect
+00005e50: 5f4e 225d 0a0a 2020 2020 6e77 696e 203d  _N"]..    nwin =
+00005e60: 2066 6674 315f 736d 6f6f 7468 6564 5f61   fft1_smoothed_a
+00005e70: 6273 2e73 6861 7065 5b30 5d0a 2020 2020  bs.shape[0].    
+00005e80: 4e66 6674 3220 3d20 6666 7431 5f73 6d6f  Nfft2 = fft1_smo
+00005e90: 6f74 6865 645f 6162 732e 7368 6170 655b  othed_abs.shape[
+00005ea0: 315d 0a0a 2020 2020 2320 2d2d 2d2d 2d2d  1]..    # ------
+00005eb0: 636f 6e76 6572 7420 616c 6c20 3244 2061  convert all 2D a
+00005ec0: 7272 6179 7320 696e 746f 2031 4420 746f  rrays into 1D to
+00005ed0: 2073 7065 6564 2075 702d 2d2d 2d2d 2d2d   speed up-------
+00005ee0: 2d0a 2020 2020 636f 7272 203d 206e 702e  -.    corr = np.
+00005ef0: 7a65 726f 7328 6e77 696e 202a 204e 6666  zeros(nwin * Nff
+00005f00: 7432 2c20 6474 7970 653d 6e70 2e63 6f6d  t2, dtype=np.com
+00005f10: 706c 6578 3634 290a 2020 2020 636f 7272  plex64).    corr
+00005f20: 203d 2066 6674 315f 736d 6f6f 7468 6564   = fft1_smoothed
+00005f30: 5f61 6273 2e72 6573 6861 7065 280a 2020  _abs.reshape(.  
+00005f40: 2020 2020 2020 6666 7431 5f73 6d6f 6f74        fft1_smoot
+00005f50: 6865 645f 6162 732e 7369 7a65 2c0a 2020  hed_abs.size,.  
+00005f60: 2020 2920 2a20 6666 7432 2e72 6573 6861    ) * fft2.resha
+00005f70: 7065 280a 2020 2020 2020 2020 6666 7432  pe(.        fft2
+00005f80: 2e73 697a 652c 0a20 2020 2029 0a0a 2020  .size,.    )..  
+00005f90: 2020 6966 206d 6574 686f 6420 3d3d 2022    if method == "
+00005fa0: 636f 6865 7265 6e63 7922 3a0a 2020 2020  coherency":.    
+00005fb0: 2020 2020 7465 6d70 203d 206d 6f76 696e      temp = movin
+00005fc0: 675f 6176 6528 0a20 2020 2020 2020 2020  g_ave(.         
+00005fd0: 2020 206e 702e 6162 7328 0a20 2020 2020     np.abs(.     
+00005fe0: 2020 2020 2020 2020 2020 2066 6674 322e             fft2.
+00005ff0: 7265 7368 6170 6528 0a20 2020 2020 2020  reshape(.       
+00006000: 2020 2020 2020 2020 2020 2020 2066 6674               fft
+00006010: 322e 7369 7a65 2c0a 2020 2020 2020 2020  2.size,.        
+00006020: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00006030: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+00006040: 2020 2020 2073 6d6f 6f74 6873 7065 6374       smoothspect
+00006050: 5f4e 2c0a 2020 2020 2020 2020 290a 2020  _N,.        ).  
+00006060: 2020 2020 2020 636f 7272 202f 3d20 7465        corr /= te
+00006070: 6d70 0a20 2020 2063 6f72 7220 3d20 636f  mp.    corr = co
+00006080: 7272 2e72 6573 6861 7065 286e 7769 6e2c  rr.reshape(nwin,
+00006090: 204e 6666 7432 290a 0a20 2020 2069 6620   Nfft2)..    if 
+000060a0: 7375 6273 7461 636b 3a0a 2020 2020 2020  substack:.      
+000060b0: 2020 6966 2073 7562 7374 6163 6b5f 6c65    if substack_le
+000060c0: 6e20 3d3d 2063 635f 6c65 6e3a 0a20 2020  n == cc_len:.   
+000060d0: 2020 2020 2020 2020 2023 2063 686f 6f73           # choos
+000060e0: 6520 746f 206b 6565 7020 616c 6c20 6666  e to keep all ff
+000060f0: 7420 6461 7461 2066 6f72 2061 2064 6179  t data for a day
+00006100: 0a20 2020 2020 2020 2020 2020 2073 5f63  .            s_c
+00006110: 6f72 7220 3d20 6e70 2e7a 6572 6f73 2873  orr = np.zeros(s
+00006120: 6861 7065 3d28 6e77 696e 2c20 4e66 6674  hape=(nwin, Nfft
+00006130: 292c 2064 7479 7065 3d6e 702e 666c 6f61  ), dtype=np.floa
+00006140: 7433 3229 2020 2320 7374 6163 6b65 6420  t32)  # stacked 
+00006150: 636f 7272 656c 6174 696f 6e0a 2020 2020  correlation.    
+00006160: 2020 2020 2020 2020 616d 706d 6178 203d          ampmax =
+00006170: 206e 702e 7a65 726f 7328 6e77 696e 2c20   np.zeros(nwin, 
+00006180: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+00006190: 290a 2020 2020 2020 2020 2020 2020 6e5f  ).            n_
+000061a0: 636f 7272 203d 206e 702e 7a65 726f 7328  corr = np.zeros(
+000061b0: 6e77 696e 2c20 6474 7970 653d 6e70 2e69  nwin, dtype=np.i
+000061c0: 6e74 3136 2920 2023 206e 756d 6265 7220  nt16)  # number 
+000061d0: 6f66 2063 6f72 7265 6c61 7469 6f6e 7320  of correlations 
+000061e0: 666f 7220 6561 6368 2073 7562 7374 6163  for each substac
+000061f0: 6b0a 2020 2020 2020 2020 2020 2020 745f  k.            t_
+00006200: 636f 7272 203d 2064 6174 6153 5f74 2020  corr = dataS_t  
+00006210: 2320 7469 6d65 7374 616d 700a 2020 2020  # timestamp.    
+00006220: 2020 2020 2020 2020 6372 6170 203d 206e          crap = n
+00006230: 702e 7a65 726f 7328 4e66 6674 2c20 6474  p.zeros(Nfft, dt
+00006240: 7970 653d 6e70 2e63 6f6d 706c 6578 3634  ype=np.complex64
+00006250: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
+00006260: 7220 6920 696e 2072 616e 6765 286e 7769  r i in range(nwi
+00006270: 6e29 3a0a 2020 2020 2020 2020 2020 2020  n):.            
+00006280: 2020 2020 6e5f 636f 7272 5b69 5d20 3d20      n_corr[i] = 
+00006290: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
+000062a0: 2020 6372 6170 5b3a 4e66 6674 325d 203d    crap[:Nfft2] =
+000062b0: 2063 6f72 725b 692c 203a 5d0a 2020 2020   corr[i, :].    
+000062c0: 2020 2020 2020 2020 2020 2020 6372 6170              crap
+000062d0: 5b3a 4e66 6674 325d 203d 2063 7261 705b  [:Nfft2] = crap[
+000062e0: 3a4e 6666 7432 5d20 2d20 6e70 2e6d 6561  :Nfft2] - np.mea
+000062f0: 6e28 6372 6170 5b3a 4e66 6674 325d 2920  n(crap[:Nfft2]) 
+00006300: 2023 2072 656d 6f76 6520 7468 6520 6d65   # remove the me
+00006310: 616e 2069 6e20 6672 6571 2064 6f6d 6169  an in freq domai
+00006320: 6e20 2873 7069 6b65 2061 7420 743d 3029  n (spike at t=0)
+00006330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006340: 2063 7261 705b 2d28 4e66 6674 3229 202b   crap[-(Nfft2) +
+00006350: 2031 203a 5d20 3d20 6e70 2e66 6c69 7028   1 :] = np.flip(
+00006360: 6e70 2e63 6f6e 6a28 6372 6170 5b31 3a28  np.conj(crap[1:(
+00006370: 4e66 6674 3229 5d29 2c20 6178 6973 3d30  Nfft2)]), axis=0
+00006380: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00006390: 2020 6372 6170 5b30 5d20 3d20 636f 6d70    crap[0] = comp
+000063a0: 6c65 7828 302c 2030 290a 2020 2020 2020  lex(0, 0).      
+000063b0: 2020 2020 2020 2020 2020 735f 636f 7272            s_corr
+000063c0: 5b69 2c20 3a5d 203d 206e 702e 7265 616c  [i, :] = np.real
+000063d0: 286e 702e 6666 742e 6966 6674 7368 6966  (np.fft.ifftshif
+000063e0: 7428 7363 6970 792e 6666 7470 6163 6b2e  t(scipy.fftpack.
+000063f0: 6966 6674 2863 7261 702c 204e 6666 742c  ifft(crap, Nfft,
+00006400: 2061 7869 733d 3029 2929 0a0a 2020 2020   axis=0)))..    
+00006410: 2020 2020 2020 2020 2320 7265 6d6f 7665          # remove
+00006420: 2061 626e 6f72 6d61 6c20 6461 7461 0a20   abnormal data. 
+00006430: 2020 2020 2020 2020 2020 2061 6d70 6d61             ampma
+00006440: 7820 3d20 6e70 2e6d 6178 2873 5f63 6f72  x = np.max(s_cor
+00006450: 722c 2061 7869 733d 3129 0a20 2020 2020  r, axis=1).     
+00006460: 2020 2020 2020 2074 696e 6478 203d 206e         tindx = n
+00006470: 702e 7768 6572 6528 2861 6d70 6d61 7820  p.where((ampmax 
+00006480: 3c20 3230 202a 206e 702e 6d65 6469 616e  < 20 * np.median
+00006490: 2861 6d70 6d61 7829 2920 2620 2861 6d70  (ampmax)) & (amp
+000064a0: 6d61 7820 3e20 3029 295b 305d 0a20 2020  max > 0))[0].   
+000064b0: 2020 2020 2020 2020 2073 5f63 6f72 7220           s_corr 
+000064c0: 3d20 735f 636f 7272 5b74 696e 6478 2c20  = s_corr[tindx, 
+000064d0: 3a5d 0a20 2020 2020 2020 2020 2020 2074  :].            t
+000064e0: 5f63 6f72 7220 3d20 745f 636f 7272 5b74  _corr = t_corr[t
+000064f0: 696e 6478 5d0a 2020 2020 2020 2020 2020  indx].          
+00006500: 2020 6e5f 636f 7272 203d 206e 5f63 6f72    n_corr = n_cor
+00006510: 725b 7469 6e64 785d 0a0a 2020 2020 2020  r[tindx]..      
+00006520: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00006530: 2020 2020 2320 6765 7420 7469 6d65 2069      # get time i
+00006540: 6e66 6f72 6d61 7469 6f6e 0a20 2020 2020  nformation.     
+00006550: 2020 2020 2020 2054 746f 7461 6c20 3d20         Ttotal = 
+00006560: 6461 7461 535f 745b 2d31 5d20 2d20 6461  dataS_t[-1] - da
+00006570: 7461 535f 745b 305d 2020 2320 746f 7461  taS_t[0]  # tota
+00006580: 6c20 6475 7261 7469 6f6e 206f 6620 7768  l duration of wh
+00006590: 6174 2077 6520 6861 7665 206e 6f77 0a20  at we have now. 
+000065a0: 2020 2020 2020 2020 2020 2074 7374 6172             tstar
+000065b0: 7420 3d20 6461 7461 535f 745b 305d 0a0a  t = dataS_t[0]..
+000065c0: 2020 2020 2020 2020 2020 2020 6e73 7461              nsta
+000065d0: 636b 203d 2069 6e74 286e 702e 726f 756e  ck = int(np.roun
+000065e0: 6428 5474 6f74 616c 202f 2073 7562 7374  d(Ttotal / subst
+000065f0: 6163 6b5f 6c65 6e29 290a 2020 2020 2020  ack_len)).      
+00006600: 2020 2020 2020 616d 706d 6178 203d 206e        ampmax = n
+00006610: 702e 7a65 726f 7328 6e73 7461 636b 2c20  p.zeros(nstack, 
+00006620: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+00006630: 290a 2020 2020 2020 2020 2020 2020 735f  ).            s_
+00006640: 636f 7272 203d 206e 702e 7a65 726f 7328  corr = np.zeros(
+00006650: 7368 6170 653d 286e 7374 6163 6b2c 204e  shape=(nstack, N
+00006660: 6666 7429 2c20 6474 7970 653d 6e70 2e66  fft), dtype=np.f
+00006670: 6c6f 6174 3332 290a 2020 2020 2020 2020  loat32).        
+00006680: 2020 2020 6e5f 636f 7272 203d 206e 702e      n_corr = np.
+00006690: 7a65 726f 7328 6e73 7461 636b 2c20 6474  zeros(nstack, dt
+000066a0: 7970 653d 6e70 2e69 6e74 3136 290a 2020  ype=np.int16).  
+000066b0: 2020 2020 2020 2020 2020 745f 636f 7272            t_corr
+000066c0: 203d 206e 702e 7a65 726f 7328 6e73 7461   = np.zeros(nsta
+000066d0: 636b 2c20 6474 7970 653d 6e70 2e66 6c6f  ck, dtype=np.flo
+000066e0: 6174 3332 290a 2020 2020 2020 2020 2020  at32).          
+000066f0: 2020 6372 6170 203d 206e 702e 7a65 726f    crap = np.zero
+00006700: 7328 4e66 6674 2c20 6474 7970 653d 6e70  s(Nfft, dtype=np
+00006710: 2e63 6f6d 706c 6578 3634 290a 0a20 2020  .complex64)..   
+00006720: 2020 2020 2020 2020 2066 6f72 2069 7374           for ist
+00006730: 6163 6b20 696e 2072 616e 6765 286e 7374  ack in range(nst
+00006740: 6163 6b29 3a0a 2020 2020 2020 2020 2020  ack):.          
+00006750: 2020 2020 2020 2320 6669 6e64 2074 6865        # find the
+00006760: 2069 6e64 6578 6573 206f 6620 616c 6c20   indexes of all 
+00006770: 6f66 2074 6865 2077 696e 646f 7773 2074  of the windows t
+00006780: 6861 7420 7374 6172 7420 6f72 2065 6e64  hat start or end
+00006790: 2077 6974 6869 6e0a 2020 2020 2020 2020   within.        
+000067a0: 2020 2020 2020 2020 6974 696d 6520 3d20          itime = 
+000067b0: 6e70 2e77 6865 7265 2828 6461 7461 535f  np.where((dataS_
+000067c0: 7420 3e3d 2074 7374 6172 7429 2026 2028  t >= tstart) & (
+000067d0: 6461 7461 535f 7420 3c20 7473 7461 7274  dataS_t < tstart
+000067e0: 202b 2073 7562 7374 6163 6b5f 6c65 6e29   + substack_len)
+000067f0: 295b 305d 0a20 2020 2020 2020 2020 2020  )[0].           
+00006800: 2020 2020 2069 6620 6c65 6e28 6974 696d       if len(itim
+00006810: 6529 203d 3d20 303a 0a20 2020 2020 2020  e) == 0:.       
+00006820: 2020 2020 2020 2020 2020 2020 2074 7374               tst
+00006830: 6172 7420 2b3d 2073 7562 7374 6163 6b5f  art += substack_
+00006840: 6c65 6e0a 2020 2020 2020 2020 2020 2020  len.            
+00006850: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+00006860: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006870: 2020 6372 6170 5b3a 4e66 6674 325d 203d    crap[:Nfft2] =
+00006880: 206e 702e 6d65 616e 2863 6f72 725b 6974   np.mean(corr[it
+00006890: 696d 652c 203a 5d2c 2061 7869 733d 3029  ime, :], axis=0)
+000068a0: 2020 2320 6c69 6e65 6172 2061 7665 7261    # linear avera
+000068b0: 6765 206f 6620 7468 6520 636f 7272 656c  ge of the correl
+000068c0: 6174 696f 6e0a 2020 2020 2020 2020 2020  ation.          
+000068d0: 2020 2020 2020 6372 6170 5b3a 4e66 6674        crap[:Nfft
+000068e0: 325d 203d 2063 7261 705b 3a4e 6666 7432  2] = crap[:Nfft2
+000068f0: 5d20 2d20 6e70 2e6d 6561 6e28 6372 6170  ] - np.mean(crap
+00006900: 5b3a 4e66 6674 325d 2920 2023 2072 656d  [:Nfft2])  # rem
+00006910: 6f76 6520 7468 6520 6d65 616e 2069 6e20  ove the mean in 
+00006920: 6672 6571 2064 6f6d 6169 6e20 2873 7069  freq domain (spi
+00006930: 6b65 2061 7420 743d 3029 0a20 2020 2020  ke at t=0).     
+00006940: 2020 2020 2020 2020 2020 2063 7261 705b             crap[
+00006950: 2d28 4e66 6674 3229 202b 2031 203a 5d20  -(Nfft2) + 1 :] 
+00006960: 3d20 6e70 2e66 6c69 7028 6e70 2e63 6f6e  = np.flip(np.con
+00006970: 6a28 6372 6170 5b31 3a28 4e66 6674 3229  j(crap[1:(Nfft2)
+00006980: 5d29 2c20 6178 6973 3d30 290a 2020 2020  ]), axis=0).    
+00006990: 2020 2020 2020 2020 2020 2020 6372 6170              crap
+000069a0: 5b30 5d20 3d20 636f 6d70 6c65 7828 302c  [0] = complex(0,
+000069b0: 2030 290a 2020 2020 2020 2020 2020 2020   0).            
+000069c0: 2020 2020 735f 636f 7272 5b69 7374 6163      s_corr[istac
+000069d0: 6b2c 203a 5d20 3d20 6e70 2e72 6561 6c28  k, :] = np.real(
+000069e0: 6e70 2e66 6674 2e69 6666 7473 6869 6674  np.fft.ifftshift
+000069f0: 2873 6369 7079 2e66 6674 7061 636b 2e69  (scipy.fftpack.i
+00006a00: 6666 7428 6372 6170 2c20 4e66 6674 2c20  fft(crap, Nfft, 
+00006a10: 6178 6973 3d30 2929 290a 2020 2020 2020  axis=0))).      
+00006a20: 2020 2020 2020 2020 2020 6e5f 636f 7272            n_corr
+00006a30: 5b69 7374 6163 6b5d 203d 206c 656e 2869  [istack] = len(i
+00006a40: 7469 6d65 2920 2023 206e 756d 6265 7220  time)  # number 
+00006a50: 6f66 2077 696e 646f 7773 2073 7461 636b  of windows stack
+00006a60: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00006a70: 2020 745f 636f 7272 5b69 7374 6163 6b5d    t_corr[istack]
+00006a80: 203d 2074 7374 6172 7420 2023 2073 6176   = tstart  # sav
+00006a90: 6520 7468 6520 7469 6d65 2073 7461 6d70  e the time stamp
+00006aa0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00006ab0: 2020 7473 7461 7274 202b 3d20 7375 6273    tstart += subs
+00006ac0: 7461 636b 5f6c 656e 0a20 2020 2020 2020  tack_len.       
+00006ad0: 2020 2020 2020 2020 2023 2070 7269 6e74           # print
+00006ae0: 2827 636f 7272 656c 6174 696f 6e20 646f  ('correlation do
+00006af0: 6e65 2061 6e64 2073 7461 636b 6564 2061  ne and stacked a
+00006b00: 7420 7469 6d65 2025 7327 2025 2073 7472  t time %s' % str
+00006b10: 2874 5f63 6f72 725b 6973 7461 636b 5d29  (t_corr[istack])
+00006b20: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
+00006b30: 2072 656d 6f76 6520 6162 6e6f 726d 616c   remove abnormal
+00006b40: 2064 6174 610a 2020 2020 2020 2020 2020   data.          
+00006b50: 2020 616d 706d 6178 203d 206e 702e 6d61    ampmax = np.ma
+00006b60: 7828 735f 636f 7272 2c20 6178 6973 3d31  x(s_corr, axis=1
+00006b70: 290a 2020 2020 2020 2020 2020 2020 7469  ).            ti
+00006b80: 6e64 7820 3d20 6e70 2e77 6865 7265 2828  ndx = np.where((
+00006b90: 616d 706d 6178 203c 2032 3020 2a20 6e70  ampmax < 20 * np
+00006ba0: 2e6d 6564 6961 6e28 616d 706d 6178 2929  .median(ampmax))
+00006bb0: 2026 2028 616d 706d 6178 203e 2030 2929   & (ampmax > 0))
+00006bc0: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+00006bd0: 735f 636f 7272 203d 2073 5f63 6f72 725b  s_corr = s_corr[
+00006be0: 7469 6e64 782c 203a 5d0a 2020 2020 2020  tindx, :].      
+00006bf0: 2020 2020 2020 745f 636f 7272 203d 2074        t_corr = t
+00006c00: 5f63 6f72 725b 7469 6e64 785d 0a20 2020  _corr[tindx].   
+00006c10: 2020 2020 2020 2020 206e 5f63 6f72 7220           n_corr 
+00006c20: 3d20 6e5f 636f 7272 5b74 696e 6478 5d0a  = n_corr[tindx].
+00006c30: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00006c40: 2020 2023 2061 7665 7261 6765 2064 6169     # average dai
+00006c50: 6c79 2063 726f 7373 2063 6f72 7265 6c61  ly cross correla
+00006c60: 7469 6f6e 2066 756e 6374 696f 6e73 0a20  tion functions. 
+00006c70: 2020 2020 2020 2061 6d70 6d61 7820 3d20         ampmax = 
+00006c80: 6e70 2e6d 6178 2863 6f72 722c 2061 7869  np.max(corr, axi
+00006c90: 733d 3129 0a20 2020 2020 2020 2074 696e  s=1).        tin
+00006ca0: 6478 203d 206e 702e 7768 6572 6528 2861  dx = np.where((a
+00006cb0: 6d70 6d61 7820 3c20 3230 202a 206e 702e  mpmax < 20 * np.
+00006cc0: 6d65 6469 616e 2861 6d70 6d61 7829 2920  median(ampmax)) 
+00006cd0: 2620 2861 6d70 6d61 7820 3e20 3029 295b  & (ampmax > 0))[
+00006ce0: 305d 0a20 2020 2020 2020 206e 5f63 6f72  0].        n_cor
+00006cf0: 7220 3d20 6e77 696e 0a20 2020 2020 2020  r = nwin.       
+00006d00: 2073 5f63 6f72 7220 3d20 6e70 2e7a 6572   s_corr = np.zer
+00006d10: 6f73 284e 6666 742c 2064 7479 7065 3d6e  os(Nfft, dtype=n
+00006d20: 702e 666c 6f61 7433 3229 0a20 2020 2020  p.float32).     
+00006d30: 2020 2074 5f63 6f72 7220 3d20 6461 7461     t_corr = data
+00006d40: 535f 745b 305d 0a20 2020 2020 2020 2063  S_t[0].        c
+00006d50: 7261 7020 3d20 6e70 2e7a 6572 6f73 284e  rap = np.zeros(N
+00006d60: 6666 742c 2064 7479 7065 3d6e 702e 636f  fft, dtype=np.co
+00006d70: 6d70 6c65 7836 3429 0a20 2020 2020 2020  mplex64).       
+00006d80: 2063 7261 705b 3a4e 6666 7432 5d20 3d20   crap[:Nfft2] = 
+00006d90: 6e70 2e6d 6561 6e28 636f 7272 5b74 696e  np.mean(corr[tin
+00006da0: 6478 5d2c 2061 7869 733d 3029 0a20 2020  dx], axis=0).   
+00006db0: 2020 2020 2063 7261 705b 3a4e 6666 7432       crap[:Nfft2
+00006dc0: 5d20 3d20 6372 6170 5b3a 4e66 6674 325d  ] = crap[:Nfft2]
+00006dd0: 202d 206e 702e 6d65 616e 2863 7261 705b   - np.mean(crap[
+00006de0: 3a4e 6666 7432 5d2c 2061 7869 733d 3029  :Nfft2], axis=0)
+00006df0: 0a20 2020 2020 2020 2063 7261 705b 2d28  .        crap[-(
+00006e00: 4e66 6674 3229 202b 2031 203a 5d20 3d20  Nfft2) + 1 :] = 
+00006e10: 6e70 2e66 6c69 7028 6e70 2e63 6f6e 6a28  np.flip(np.conj(
+00006e20: 6372 6170 5b31 3a28 4e66 6674 3229 5d29  crap[1:(Nfft2)])
+00006e30: 2c20 6178 6973 3d30 290a 2020 2020 2020  , axis=0).      
+00006e40: 2020 735f 636f 7272 203d 206e 702e 7265    s_corr = np.re
+00006e50: 616c 286e 702e 6666 742e 6966 6674 7368  al(np.fft.ifftsh
+00006e60: 6966 7428 7363 6970 792e 6666 7470 6163  ift(scipy.fftpac
+00006e70: 6b2e 6966 6674 2863 7261 702c 204e 6666  k.ifft(crap, Nff
+00006e80: 742c 2061 7869 733d 3029 2929 0a0a 2020  t, axis=0)))..  
+00006e90: 2020 2320 7472 696d 2074 6865 2043 4346    # trim the CCF
+00006ea0: 7320 696e 205b 2d6d 6178 6c61 6720 6d61  s in [-maxlag ma
+00006eb0: 786c 6167 5d0a 2020 2020 7420 3d20 6e70  xlag].    t = np
+00006ec0: 2e61 7261 6e67 6528 2d4e 6666 7432 202b  .arange(-Nfft2 +
+00006ed0: 2031 2c20 4e66 6674 3229 202a 2064 740a   1, Nfft2) * dt.
+00006ee0: 2020 2020 696e 6420 3d20 6e70 2e77 6865      ind = np.whe
+00006ef0: 7265 286e 702e 6162 7328 7429 203c 3d20  re(np.abs(t) <= 
+00006f00: 6d61 786c 6167 295b 305d 0a20 2020 2069  maxlag)[0].    i
+00006f10: 6620 735f 636f 7272 2e6e 6469 6d20 3d3d  f s_corr.ndim ==
+00006f20: 2031 3a0a 2020 2020 2020 2020 735f 636f   1:.        s_co
+00006f30: 7272 203d 2073 5f63 6f72 725b 696e 645d  rr = s_corr[ind]
+00006f40: 0a20 2020 2065 6c69 6620 735f 636f 7272  .    elif s_corr
+00006f50: 2e6e 6469 6d20 3d3d 2032 3a0a 2020 2020  .ndim == 2:.    
+00006f60: 2020 2020 735f 636f 7272 203d 2073 5f63      s_corr = s_c
+00006f70: 6f72 725b 3a2c 2069 6e64 5d0a 2020 2020  orr[:, ind].    
+00006f80: 7265 7475 726e 2073 5f63 6f72 722c 2074  return s_corr, t
+00006f90: 5f63 6f72 722c 206e 5f63 6f72 720a 0a0a  _corr, n_corr...
+00006fa0: 6465 6620 636f 7272 656c 6174 655f 6e6f  def correlate_no
+00006fb0: 6e6c 696e 6561 725f 7374 6163 6b28 6666  nlinear_stack(ff
+00006fc0: 7431 5f73 6d6f 6f74 6865 645f 6162 732c  t1_smoothed_abs,
+00006fd0: 2066 6674 322c 2044 2c20 4e66 6674 2c20   fft2, D, Nfft, 
+00006fe0: 6461 7461 535f 7429 3a0a 2020 2020 2222  dataS_t):.    ""
+00006ff0: 220a 2020 2020 7468 6973 2066 756e 6374  ".    this funct
+00007000: 696f 6e20 646f 6573 2074 6865 2063 726f  ion does the cro
+00007010: 7373 2d63 6f72 7265 6c61 7469 6f6e 2069  ss-correlation i
+00007020: 6e20 6672 6571 2064 6f6d 6169 6e20 616e  n freq domain an
+00007030: 6420 6861 7320 7468 6520 6f70 7469 6f6e  d has the option
+00007040: 2074 6f20 6b65 6570 2073 7562 2d73 7461   to keep sub-sta
+00007050: 636b 7320 6f66 0a20 2020 2074 6865 2063  cks of.    the c
+00007060: 726f 7373 2d63 6f72 7265 6c61 7469 6f6e  ross-correlation
+00007070: 2069 6620 6e65 6564 6564 2e20 6974 2074   if needed. it t
+00007080: 616b 6573 2061 6476 616e 7461 6765 206f  akes advantage o
+00007090: 6620 7468 6520 6c69 6e65 6172 2072 656c  f the linear rel
+000070a0: 6174 696f 6e73 6869 7020 6f66 2069 6666  ationship of iff
+000070b0: 742c 2073 6f20 7468 6174 0a20 2020 2073  t, so that.    s
+000070c0: 7461 636b 696e 6720 6973 2070 6572 666f  tacking is perfo
+000070d0: 726d 6564 2069 6e20 7370 6563 7472 756d  rmed in spectrum
+000070e0: 2064 6f6d 6169 6e20 6669 7273 7420 746f   domain first to
+000070f0: 2072 6564 7563 6520 7468 6520 746f 7461   reduce the tota
+00007100: 6c20 6e75 6d62 6572 206f 6620 6966 6674  l number of ifft
+00007110: 2e20 2875 7365 6420 696e 2053 3129 0a20  . (used in S1). 
+00007120: 2020 2050 4152 414d 4554 4552 533a 0a20     PARAMETERS:. 
+00007130: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+00007140: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2066 6674  --------.    fft
+00007150: 315f 736d 6f6f 7468 6564 5f61 6273 3a20  1_smoothed_abs: 
+00007160: 736d 6f6f 7468 6564 2070 6f77 6572 2073  smoothed power s
+00007170: 7065 6374 7261 6c20 6465 6e73 6974 7920  pectral density 
+00007180: 6f66 2074 6865 2046 4654 2066 6f72 2074  of the FFT for t
+00007190: 6865 2073 6f75 7263 6520 7374 6174 696f  he source statio
+000071a0: 6e0a 2020 2020 6666 7432 3a20 7261 7720  n.    fft2: raw 
+000071b0: 4646 5420 7370 6563 7472 756d 206f 6620  FFT spectrum of 
+000071c0: 7468 6520 7265 6365 6976 6572 2073 7461  the receiver sta
+000071d0: 7469 6f6e 0a20 2020 2044 3a20 6469 6374  tion.    D: dict
+000071e0: 696f 6e61 7279 2063 6f6e 7461 696e 696e  ionary containin
+000071f0: 6720 666f 6c6c 6f77 696e 6720 7061 7261  g following para
+00007200: 6d65 7465 7273 3a0a 2020 2020 2020 2020  meters:.        
+00007210: 6d61 786c 6167 3a20 206d 6178 696d 756d  maxlag:  maximum
+00007220: 206c 6167 7320 746f 206b 6565 7020 696e   lags to keep in
+00007230: 2074 6865 2063 726f 7373 2063 6f72 7265   the cross corre
+00007240: 6c61 7469 6f6e 0a20 2020 2020 2020 2064  lation.        d
+00007250: 743a 2020 2020 2020 7361 6d70 6c69 6e67  t:      sampling
+00007260: 2072 6174 6520 2869 6e20 7329 0a20 2020   rate (in s).   
+00007270: 2020 2020 206e 7769 6e3a 2020 2020 6e75       nwin:    nu
+00007280: 6d62 6572 206f 6620 7365 676d 656e 7473  mber of segments
+00007290: 2069 6e20 7468 6520 3244 206d 6174 7269   in the 2D matri
+000072a0: 780a 2020 2020 2020 2020 6d65 7468 6f64  x.        method
+000072b0: 3a20 2063 726f 7373 2d63 6f72 7265 6c61  :  cross-correla
+000072c0: 7469 6f6e 206d 6574 686f 6473 2073 656c  tion methods sel
+000072d0: 6563 7465 6420 6279 2074 6865 2075 7365  ected by the use
+000072e0: 720a 2020 2020 2020 2020 6672 6571 6d69  r.        freqmi
+000072f0: 6e3a 206d 696e 696d 756d 2066 7265 7175  n: minimum frequ
+00007300: 656e 6379 2028 487a 290a 2020 2020 2020  ency (Hz).      
+00007310: 2020 6672 6571 6d61 783a 206d 6178 696d    freqmax: maxim
+00007320: 756d 2066 7265 7175 656e 6379 2028 487a  um frequency (Hz
+00007330: 290a 2020 2020 4e66 6674 3a20 2020 206e  ).    Nfft:    n
+00007340: 756d 6265 7220 6f66 2066 7265 7175 656e  umber of frequen
+00007350: 6379 2070 6f69 6e74 7320 666f 7220 6966  cy points for if
+00007360: 6674 0a20 2020 2064 6174 6153 5f74 3a20  ft.    dataS_t: 
+00007370: 6d61 7472 6978 206f 6620 6461 7465 7469  matrix of dateti
+00007380: 6d65 206f 626a 6563 742e 0a20 2020 2052  me object..    R
+00007390: 4554 5552 4e53 3a0a 2020 2020 2d2d 2d2d  ETURNS:.    ----
+000073a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000073b0: 2d0a 2020 2020 735f 636f 7272 3a20 3144  -.    s_corr: 1D
+000073c0: 206f 7220 3244 206d 6174 7269 7820 6f66   or 2D matrix of
+000073d0: 2074 6865 2061 7665 7261 6765 6420 6f72   the averaged or
+000073e0: 2073 7562 2d73 7461 636b 7320 6f66 2063   sub-stacks of c
+000073f0: 726f 7373 2d63 6f72 7265 6c61 7469 6f6e  ross-correlation
+00007400: 2066 756e 6374 696f 6e73 2069 6e20 7469   functions in ti
+00007410: 6d65 2064 6f6d 6169 6e0a 2020 2020 745f  me domain.    t_
+00007420: 636f 7272 3a20 7469 6d65 7374 616d 7020  corr: timestamp 
+00007430: 666f 7220 6561 6368 2073 7562 2d73 7461  for each sub-sta
+00007440: 636b 206f 7220 6176 6572 6167 6564 2066  ck or averaged f
+00007450: 756e 6374 696f 6e0a 2020 2020 6e5f 636f  unction.    n_co
+00007460: 7272 3a20 6e75 6d62 6572 206f 6620 696e  rr: number of in
+00007470: 636c 7564 6564 2073 6567 6d65 6e74 7320  cluded segments 
+00007480: 666f 7220 6561 6368 2073 7562 2d73 7461  for each sub-sta
+00007490: 636b 206f 7220 6176 6572 6167 6564 2066  ck or averaged f
+000074a0: 756e 6374 696f 6e0a 2020 2020 2222 220a  unction.    """.
+000074b0: 2020 2020 2320 2d2d 2d2d 6c6f 6164 2070      # ----load p
+000074c0: 6172 616d 7465 7273 2d2d 2d2d 0a20 2020  aramters----.   
+000074d0: 2064 7420 3d20 445b 2264 7422 5d0a 2020   dt = D["dt"].  
+000074e0: 2020 6d61 786c 6167 203d 2044 5b22 6d61    maxlag = D["ma
+000074f0: 786c 6167 225d 0a20 2020 206d 6574 686f  xlag"].    metho
+00007500: 6420 3d20 445b 2263 635f 6d65 7468 6f64  d = D["cc_method
+00007510: 225d 0a20 2020 2063 635f 6c65 6e20 3d20  "].    cc_len = 
+00007520: 445b 2263 635f 6c65 6e22 5d0a 2020 2020  D["cc_len"].    
+00007530: 7375 6273 7461 636b 203d 2044 5b22 7375  substack = D["su
+00007540: 6273 7461 636b 225d 0a20 2020 2073 7461  bstack"].    sta
+00007550: 636b 5f6d 6574 686f 6420 3d20 445b 2273  ck_method = D["s
+00007560: 7461 636b 5f6d 6574 686f 6422 5d0a 2020  tack_method"].  
+00007570: 2020 7375 6273 7461 636b 5f6c 656e 203d    substack_len =
+00007580: 2044 5b22 7375 6273 7461 636b 5f6c 656e   D["substack_len
+00007590: 225d 0a20 2020 2073 6d6f 6f74 6873 7065  "].    smoothspe
+000075a0: 6374 5f4e 203d 2044 5b22 736d 6f6f 7468  ct_N = D["smooth
+000075b0: 7370 6563 745f 4e22 5d0a 0a20 2020 206e  spect_N"]..    n
+000075c0: 7769 6e20 3d20 6666 7431 5f73 6d6f 6f74  win = fft1_smoot
+000075d0: 6865 645f 6162 732e 7368 6170 655b 305d  hed_abs.shape[0]
+000075e0: 0a20 2020 204e 6666 7432 203d 2066 6674  .    Nfft2 = fft
+000075f0: 315f 736d 6f6f 7468 6564 5f61 6273 2e73  1_smoothed_abs.s
+00007600: 6861 7065 5b31 5d0a 0a20 2020 2023 202d  hape[1]..    # -
+00007610: 2d2d 2d2d 2d63 6f6e 7665 7274 2061 6c6c  -----convert all
+00007620: 2032 4420 6172 7261 7973 2069 6e74 6f20   2D arrays into 
+00007630: 3144 2074 6f20 7370 6565 6420 7570 2d2d  1D to speed up--
+00007640: 2d2d 2d2d 2d2d 0a20 2020 2063 6f72 7220  ------.    corr 
+00007650: 3d20 6e70 2e7a 6572 6f73 286e 7769 6e20  = np.zeros(nwin 
+00007660: 2a20 4e66 6674 322c 2064 7479 7065 3d6e  * Nfft2, dtype=n
+00007670: 702e 636f 6d70 6c65 7836 3429 0a20 2020  p.complex64).   
+00007680: 2063 6f72 7220 3d20 6666 7431 5f73 6d6f   corr = fft1_smo
+00007690: 6f74 6865 645f 6162 732e 7265 7368 6170  othed_abs.reshap
+000076a0: 6528 0a20 2020 2020 2020 2066 6674 315f  e(.        fft1_
+000076b0: 736d 6f6f 7468 6564 5f61 6273 2e73 697a  smoothed_abs.siz
+000076c0: 652c 0a20 2020 2029 202a 2066 6674 322e  e,.    ) * fft2.
+000076d0: 7265 7368 6170 6528 0a20 2020 2020 2020  reshape(.       
+000076e0: 2066 6674 322e 7369 7a65 2c0a 2020 2020   fft2.size,.    
+000076f0: 290a 0a20 2020 2023 206e 6f72 6d61 6c69  )..    # normali
+00007700: 7a65 2062 7920 7265 6365 6976 6572 2073  ze by receiver s
+00007710: 7065 6374 7261 6c20 666f 7220 636f 6865  pectral for cohe
+00007720: 7265 6e63 790a 2020 2020 6966 206d 6574  rency.    if met
+00007730: 686f 6420 3d3d 2022 636f 6865 7265 6e63  hod == "coherenc
+00007740: 7922 3a0a 2020 2020 2020 2020 7465 6d70  y":.        temp
+00007750: 203d 206d 6f76 696e 675f 6176 6528 0a20   = moving_ave(. 
+00007760: 2020 2020 2020 2020 2020 206e 702e 6162             np.ab
+00007770: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
+00007780: 2020 2066 6674 322e 7265 7368 6170 6528     fft2.reshape(
+00007790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000077a0: 2020 2020 2066 6674 322e 7369 7a65 2c0a       fft2.size,.
+000077b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077c0: 290a 2020 2020 2020 2020 2020 2020 292c  ).            ),
+000077d0: 0a20 2020 2020 2020 2020 2020 2073 6d6f  .            smo
+000077e0: 6f74 6873 7065 6374 5f4e 2c0a 2020 2020  othspect_N,.    
+000077f0: 2020 2020 290a 2020 2020 2020 2020 636f      ).        co
+00007800: 7272 202f 3d20 7465 6d70 0a20 2020 2063  rr /= temp.    c
+00007810: 6f72 7220 3d20 636f 7272 2e72 6573 6861  orr = corr.resha
+00007820: 7065 286e 7769 6e2c 204e 6666 7432 290a  pe(nwin, Nfft2).
+00007830: 0a20 2020 2023 2074 7261 6e73 666f 726d  .    # transform
+00007840: 2062 6163 6b20 746f 2074 696d 6520 646f   back to time do
+00007850: 6d61 696e 2077 6176 6566 6f72 6d73 0a20  main waveforms. 
+00007860: 2020 2073 5f63 6f72 7220 3d20 6e70 2e7a     s_corr = np.z
+00007870: 6572 6f73 2873 6861 7065 3d28 6e77 696e  eros(shape=(nwin
+00007880: 2c20 4e66 6674 292c 2064 7479 7065 3d6e  , Nfft), dtype=n
+00007890: 702e 666c 6f61 7433 3229 2020 2320 7374  p.float32)  # st
+000078a0: 6163 6b65 6420 636f 7272 656c 6174 696f  acked correlatio
+000078b0: 6e0a 2020 2020 616d 706d 6178 203d 206e  n.    ampmax = n
+000078c0: 702e 7a65 726f 7328 6e77 696e 2c20 6474  p.zeros(nwin, dt
+000078d0: 7970 653d 6e70 2e66 6c6f 6174 3332 290a  ype=np.float32).
+000078e0: 2020 2020 6e5f 636f 7272 203d 206e 702e      n_corr = np.
+000078f0: 7a65 726f 7328 6e77 696e 2c20 6474 7970  zeros(nwin, dtyp
+00007900: 653d 6e70 2e69 6e74 3136 2920 2023 206e  e=np.int16)  # n
+00007910: 756d 6265 7220 6f66 2063 6f72 7265 6c61  umber of correla
+00007920: 7469 6f6e 7320 666f 7220 6561 6368 2073  tions for each s
+00007930: 7562 7374 6163 6b0a 2020 2020 745f 636f  ubstack.    t_co
+00007940: 7272 203d 2064 6174 6153 5f74 2020 2320  rr = dataS_t  # 
+00007950: 7469 6d65 7374 616d 700a 2020 2020 6372  timestamp.    cr
+00007960: 6170 203d 206e 702e 7a65 726f 7328 4e66  ap = np.zeros(Nf
+00007970: 6674 2c20 6474 7970 653d 6e70 2e63 6f6d  ft, dtype=np.com
+00007980: 706c 6578 3634 290a 2020 2020 666f 7220  plex64).    for 
+00007990: 6920 696e 2072 616e 6765 286e 7769 6e29  i in range(nwin)
+000079a0: 3a0a 2020 2020 2020 2020 6e5f 636f 7272  :.        n_corr
+000079b0: 5b69 5d20 3d20 310a 2020 2020 2020 2020  [i] = 1.        
+000079c0: 6372 6170 5b3a 4e66 6674 325d 203d 2063  crap[:Nfft2] = c
+000079d0: 6f72 725b 692c 203a 5d0a 2020 2020 2020  orr[i, :].      
+000079e0: 2020 6372 6170 5b3a 4e66 6674 325d 203d    crap[:Nfft2] =
+000079f0: 2063 7261 705b 3a4e 6666 7432 5d20 2d20   crap[:Nfft2] - 
+00007a00: 6e70 2e6d 6561 6e28 6372 6170 5b3a 4e66  np.mean(crap[:Nf
+00007a10: 6674 325d 2920 2023 2072 656d 6f76 6520  ft2])  # remove 
+00007a20: 7468 6520 6d65 616e 2069 6e20 6672 6571  the mean in freq
+00007a30: 2064 6f6d 6169 6e20 2873 7069 6b65 2061   domain (spike a
+00007a40: 7420 743d 3029 0a20 2020 2020 2020 2063  t t=0).        c
+00007a50: 7261 705b 2d28 4e66 6674 3229 202b 2031  rap[-(Nfft2) + 1
+00007a60: 203a 5d20 3d20 6e70 2e66 6c69 7028 6e70   :] = np.flip(np
+00007a70: 2e63 6f6e 6a28 6372 6170 5b31 3a28 4e66  .conj(crap[1:(Nf
+00007a80: 6674 3229 5d29 2c20 6178 6973 3d30 290a  ft2)]), axis=0).
+00007a90: 2020 2020 2020 2020 6372 6170 5b30 5d20          crap[0] 
+00007aa0: 3d20 636f 6d70 6c65 7828 302c 2030 290a  = complex(0, 0).
+00007ab0: 2020 2020 2020 2020 735f 636f 7272 5b69          s_corr[i
+00007ac0: 2c20 3a5d 203d 206e 702e 7265 616c 286e  , :] = np.real(n
+00007ad0: 702e 6666 742e 6966 6674 7368 6966 7428  p.fft.ifftshift(
+00007ae0: 7363 6970 792e 6666 7470 6163 6b2e 6966  scipy.fftpack.if
+00007af0: 6674 2863 7261 702c 204e 6666 742c 2061  ft(crap, Nfft, a
+00007b00: 7869 733d 3029 2929 0a0a 2020 2020 6e73  xis=0)))..    ns
+00007b10: 5f63 6f72 7220 3d20 735f 636f 7272 0a20  _corr = s_corr. 
+00007b20: 2020 2066 6f72 2069 6969 2069 6e20 7261     for iii in ra
+00007b30: 6e67 6528 6e73 5f63 6f72 722e 7368 6170  nge(ns_corr.shap
+00007b40: 655b 305d 293a 0a20 2020 2020 2020 206e  e[0]):.        n
+00007b50: 735f 636f 7272 5b69 6969 5d20 2f3d 206e  s_corr[iii] /= n
+00007b60: 702e 6d61 7828 6e70 2e61 6273 286e 735f  p.max(np.abs(ns_
+00007b70: 636f 7272 5b69 6969 5d29 290a 0a20 2020  corr[iii]))..   
+00007b80: 2069 6620 7375 6273 7461 636b 3a0a 2020   if substack:.  
+00007b90: 2020 2020 2020 6966 2073 7562 7374 6163        if substac
+00007ba0: 6b5f 6c65 6e20 3d3d 2063 635f 6c65 6e3a  k_len == cc_len:
+00007bb0: 0a20 2020 2020 2020 2020 2020 2023 2072  .            # r
+00007bc0: 656d 6f76 6520 6162 6e6f 726d 616c 2064  emove abnormal d
+00007bd0: 6174 610a 2020 2020 2020 2020 2020 2020  ata.            
+00007be0: 616d 706d 6178 203d 206e 702e 6d61 7828  ampmax = np.max(
+00007bf0: 735f 636f 7272 2c20 6178 6973 3d31 290a  s_corr, axis=1).
+00007c00: 2020 2020 2020 2020 2020 2020 7469 6e64              tind
+00007c10: 7820 3d20 6e70 2e77 6865 7265 2828 616d  x = np.where((am
+00007c20: 706d 6178 203c 2032 3020 2a20 6e70 2e6d  pmax < 20 * np.m
+00007c30: 6564 6961 6e28 616d 706d 6178 2929 2026  edian(ampmax)) &
+00007c40: 2028 616d 706d 6178 203e 2030 2929 5b30   (ampmax > 0))[0
+00007c50: 5d0a 2020 2020 2020 2020 2020 2020 735f  ].            s_
+00007c60: 636f 7272 203d 2073 5f63 6f72 725b 7469  corr = s_corr[ti
+00007c70: 6e64 782c 203a 5d0a 2020 2020 2020 2020  ndx, :].        
+00007c80: 2020 2020 745f 636f 7272 203d 2074 5f63      t_corr = t_c
+00007c90: 6f72 725b 7469 6e64 785d 0a20 2020 2020  orr[tindx].     
+00007ca0: 2020 2020 2020 206e 5f63 6f72 7220 3d20         n_corr = 
+00007cb0: 6e5f 636f 7272 5b74 696e 6478 5d0a 0a20  n_corr[tindx].. 
+00007cc0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00007cd0: 2020 2020 2020 2020 2023 2067 6574 2074           # get t
+00007ce0: 696d 6520 696e 666f 726d 6174 696f 6e0a  ime information.
+00007cf0: 2020 2020 2020 2020 2020 2020 5474 6f74              Ttot
+00007d00: 616c 203d 2064 6174 6153 5f74 5b2d 315d  al = dataS_t[-1]
+00007d10: 202d 2064 6174 6153 5f74 5b30 5d20 2023   - dataS_t[0]  #
+00007d20: 2074 6f74 616c 2064 7572 6174 696f 6e20   total duration 
+00007d30: 6f66 2077 6861 7420 7765 2068 6176 6520  of what we have 
+00007d40: 6e6f 770a 2020 2020 2020 2020 2020 2020  now.            
+00007d50: 7473 7461 7274 203d 2064 6174 6153 5f74  tstart = dataS_t
+00007d60: 5b30 5d0a 0a20 2020 2020 2020 2020 2020  [0]..           
+00007d70: 206e 7374 6163 6b20 3d20 696e 7428 6e70   nstack = int(np
+00007d80: 2e72 6f75 6e64 2854 746f 7461 6c20 2f20  .round(Ttotal / 
+00007d90: 7375 6273 7461 636b 5f6c 656e 2929 0a20  substack_len)). 
+00007da0: 2020 2020 2020 2020 2020 2061 6d70 6d61             ampma
+00007db0: 7820 3d20 6e70 2e7a 6572 6f73 286e 7374  x = np.zeros(nst
+00007dc0: 6163 6b2c 2064 7479 7065 3d6e 702e 666c  ack, dtype=np.fl
+00007dd0: 6f61 7433 3229 0a20 2020 2020 2020 2020  oat32).         
+00007de0: 2020 2073 5f63 6f72 7220 3d20 6e70 2e7a     s_corr = np.z
+00007df0: 6572 6f73 2873 6861 7065 3d28 6e73 7461  eros(shape=(nsta
+00007e00: 636b 2c20 4e66 6674 292c 2064 7479 7065  ck, Nfft), dtype
+00007e10: 3d6e 702e 666c 6f61 7433 3229 0a20 2020  =np.float32).   
+00007e20: 2020 2020 2020 2020 206e 5f63 6f72 7220           n_corr 
+00007e30: 3d20 6e70 2e7a 6572 6f73 286e 7374 6163  = np.zeros(nstac
+00007e40: 6b2c 2064 7479 7065 3d6e 702e 696e 7429  k, dtype=np.int)
+00007e50: 0a20 2020 2020 2020 2020 2020 2074 5f63  .            t_c
+00007e60: 6f72 7220 3d20 6e70 2e7a 6572 6f73 286e  orr = np.zeros(n
+00007e70: 7374 6163 6b2c 2064 7479 7065 3d6e 702e  stack, dtype=np.
+00007e80: 666c 6f61 7429 0a20 2020 2020 2020 2020  float).         
+00007e90: 2020 2063 7261 7020 3d20 6e70 2e7a 6572     crap = np.zer
+00007ea0: 6f73 284e 6666 742c 2064 7479 7065 3d6e  os(Nfft, dtype=n
+00007eb0: 702e 636f 6d70 6c65 7836 3429 0a0a 2020  p.complex64)..  
+00007ec0: 2020 2020 2020 2020 2020 666f 7220 6973            for is
+00007ed0: 7461 636b 2069 6e20 7261 6e67 6528 6e73  tack in range(ns
+00007ee0: 7461 636b 293a 0a20 2020 2020 2020 2020  tack):.         
+00007ef0: 2020 2020 2020 2023 2066 696e 6420 7468         # find th
+00007f00: 6520 696e 6465 7865 7320 6f66 2061 6c6c  e indexes of all
+00007f10: 206f 6620 7468 6520 7769 6e64 6f77 7320   of the windows 
+00007f20: 7468 6174 2073 7461 7274 206f 7220 656e  that start or en
+00007f30: 6420 7769 7468 696e 0a20 2020 2020 2020  d within.       
+00007f40: 2020 2020 2020 2020 2069 7469 6d65 203d           itime =
+00007f50: 206e 702e 7768 6572 6528 2864 6174 6153   np.where((dataS
+00007f60: 5f74 203e 3d20 7473 7461 7274 2920 2620  _t >= tstart) & 
+00007f70: 2864 6174 6153 5f74 203c 2074 7374 6172  (dataS_t < tstar
+00007f80: 7420 2b20 7375 6273 7461 636b 5f6c 656e  t + substack_len
+00007f90: 2929 5b30 5d0a 2020 2020 2020 2020 2020  ))[0].          
+00007fa0: 2020 2020 2020 6966 206c 656e 2869 7469        if len(iti
+00007fb0: 6d65 2920 3d3d 2030 3a0a 2020 2020 2020  me) == 0:.      
+00007fc0: 2020 2020 2020 2020 2020 2020 2020 7473                ts
+00007fd0: 7461 7274 202b 3d20 7375 6273 7461 636b  tart += substack
+00007fe0: 5f6c 656e 0a20 2020 2020 2020 2020 2020  _len.           
+00007ff0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+00008000: 650a 0a20 2020 2020 2020 2020 2020 2020  e..             
+00008010: 2020 2063 7261 705b 3a4e 6666 7432 5d20     crap[:Nfft2] 
+00008020: 3d20 6e70 2e6d 6561 6e28 636f 7272 5b69  = np.mean(corr[i
+00008030: 7469 6d65 2c20 3a5d 2c20 6178 6973 3d30  time, :], axis=0
+00008040: 2920 2023 206c 696e 6561 7220 6176 6572  )  # linear aver
+00008050: 6167 6520 6f66 2074 6865 2063 6f72 7265  age of the corre
+00008060: 6c61 7469 6f6e 0a20 2020 2020 2020 2020  lation.         
+00008070: 2020 2020 2020 2063 7261 705b 3a4e 6666         crap[:Nff
+00008080: 7432 5d20 3d20 6372 6170 5b3a 4e66 6674  t2] = crap[:Nfft
+00008090: 325d 202d 206e 702e 6d65 616e 2863 7261  2] - np.mean(cra
+000080a0: 705b 3a4e 6666 7432 5d29 2020 2320 7265  p[:Nfft2])  # re
+000080b0: 6d6f 7665 2074 6865 206d 6561 6e20 696e  move the mean in
+000080c0: 2066 7265 7120 646f 6d61 696e 2028 7370   freq domain (sp
+000080d0: 696b 6520 6174 2074 3d30 290a 2020 2020  ike at t=0).    
+000080e0: 2020 2020 2020 2020 2020 2020 6372 6170              crap
+000080f0: 5b2d 284e 6666 7432 2920 2b20 3120 3a5d  [-(Nfft2) + 1 :]
+00008100: 203d 206e 702e 666c 6970 286e 702e 636f   = np.flip(np.co
+00008110: 6e6a 2863 7261 705b 313a 284e 6666 7432  nj(crap[1:(Nfft2
+00008120: 295d 292c 2061 7869 733d 3029 0a20 2020  )]), axis=0).   
+00008130: 2020 2020 2020 2020 2020 2020 2063 7261               cra
+00008140: 705b 305d 203d 2063 6f6d 706c 6578 2830  p[0] = complex(0
+00008150: 2c20 3029 0a20 2020 2020 2020 2020 2020  , 0).           
+00008160: 2020 2020 2073 5f63 6f72 725b 6973 7461       s_corr[ista
+00008170: 636b 2c20 3a5d 203d 206e 702e 7265 616c  ck, :] = np.real
+00008180: 286e 702e 6666 742e 6966 6674 7368 6966  (np.fft.ifftshif
+00008190: 7428 7363 6970 792e 6666 7470 6163 6b2e  t(scipy.fftpack.
+000081a0: 6966 6674 2863 7261 702c 204e 6666 742c  ifft(crap, Nfft,
+000081b0: 2061 7869 733d 3029 2929 0a20 2020 2020   axis=0))).     
+000081c0: 2020 2020 2020 2020 2020 206e 5f63 6f72             n_cor
+000081d0: 725b 6973 7461 636b 5d20 3d20 6c65 6e28  r[istack] = len(
+000081e0: 6974 696d 6529 2020 2320 6e75 6d62 6572  itime)  # number
+000081f0: 206f 6620 7769 6e64 6f77 7320 7374 6163   of windows stac
+00008200: 6b73 0a20 2020 2020 2020 2020 2020 2020  ks.             
+00008210: 2020 2074 5f63 6f72 725b 6973 7461 636b     t_corr[istack
+00008220: 5d20 3d20 7473 7461 7274 2020 2320 7361  ] = tstart  # sa
+00008230: 7665 2074 6865 2074 696d 6520 7374 616d  ve the time stam
+00008240: 7073 0a20 2020 2020 2020 2020 2020 2020  ps.             
+00008250: 2020 2074 7374 6172 7420 2b3d 2073 7562     tstart += sub
+00008260: 7374 6163 6b5f 6c65 6e0a 2020 2020 2020  stack_len.      
+00008270: 2020 2020 2020 2020 2020 2320 7072 696e            # prin
+00008280: 7428 2763 6f72 7265 6c61 7469 6f6e 2064  t('correlation d
+00008290: 6f6e 6520 616e 6420 7374 6163 6b65 6420  one and stacked 
+000082a0: 6174 2074 696d 6520 2573 2720 2520 7374  at time %s' % st
+000082b0: 7228 745f 636f 7272 5b69 7374 6163 6b5d  r(t_corr[istack]
+000082c0: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
+000082d0: 2320 7265 6d6f 7665 2061 626e 6f72 6d61  # remove abnorma
+000082e0: 6c20 6461 7461 0a20 2020 2020 2020 2020  l data.         
+000082f0: 2020 2061 6d70 6d61 7820 3d20 6e70 2e6d     ampmax = np.m
+00008300: 6178 2873 5f63 6f72 722c 2061 7869 733d  ax(s_corr, axis=
+00008310: 3129 0a20 2020 2020 2020 2020 2020 2074  1).            t
+00008320: 696e 6478 203d 206e 702e 7768 6572 6528  indx = np.where(
+00008330: 2861 6d70 6d61 7820 3c20 3230 202a 206e  (ampmax < 20 * n
+00008340: 702e 6d65 6469 616e 2861 6d70 6d61 7829  p.median(ampmax)
+00008350: 2920 2620 2861 6d70 6d61 7820 3e20 3029  ) & (ampmax > 0)
+00008360: 295b 305d 0a20 2020 2020 2020 2020 2020  )[0].           
+00008370: 2073 5f63 6f72 7220 3d20 735f 636f 7272   s_corr = s_corr
+00008380: 5b74 696e 6478 2c20 3a5d 0a20 2020 2020  [tindx, :].     
+00008390: 2020 2020 2020 2074 5f63 6f72 7220 3d20         t_corr = 
+000083a0: 745f 636f 7272 5b74 696e 6478 5d0a 2020  t_corr[tindx].  
+000083b0: 2020 2020 2020 2020 2020 6e5f 636f 7272            n_corr
+000083c0: 203d 206e 5f63 6f72 725b 7469 6e64 785d   = n_corr[tindx]
+000083d0: 0a0a 2020 2020 656c 7365 3a0a 2020 2020  ..    else:.    
+000083e0: 2020 2020 2320 6176 6572 6167 6520 6461      # average da
+000083f0: 696c 7920 6372 6f73 7320 636f 7272 656c  ily cross correl
+00008400: 6174 696f 6e20 6675 6e63 7469 6f6e 730a  ation functions.
+00008410: 2020 2020 2020 2020 6966 2073 7461 636b          if stack
+00008420: 5f6d 6574 686f 6420 3d3d 2053 7461 636b  _method == Stack
+00008430: 4d65 7468 6f64 2e4c 494e 4541 523a 0a20  Method.LINEAR:. 
+00008440: 2020 2020 2020 2020 2020 2061 6d70 6d61             ampma
+00008450: 7820 3d20 6e70 2e6d 6178 2873 5f63 6f72  x = np.max(s_cor
+00008460: 722c 2061 7869 733d 3129 0a20 2020 2020  r, axis=1).     
+00008470: 2020 2020 2020 2074 696e 6478 203d 206e         tindx = n
+00008480: 702e 7768 6572 6528 2861 6d70 6d61 7820  p.where((ampmax 
+00008490: 3c20 3230 202a 206e 702e 6d65 6469 616e  < 20 * np.median
+000084a0: 2861 6d70 6d61 7829 2920 2620 2861 6d70  (ampmax)) & (amp
+000084b0: 6d61 7820 3e20 3029 295b 305d 0a20 2020  max > 0))[0].   
+000084c0: 2020 2020 2020 2020 2073 5f63 6f72 7220           s_corr 
+000084d0: 3d20 6e70 2e6d 6561 6e28 735f 636f 7272  = np.mean(s_corr
+000084e0: 5b74 696e 6478 5d2c 2061 7869 733d 3029  [tindx], axis=0)
+000084f0: 0a20 2020 2020 2020 2020 2020 2074 5f63  .            t_c
+00008500: 6f72 7220 3d20 6461 7461 535f 745b 305d  orr = dataS_t[0]
+00008510: 0a20 2020 2020 2020 2020 2020 206e 5f63  .            n_c
+00008520: 6f72 7220 3d20 6c65 6e28 7469 6e64 7829  orr = len(tindx)
+00008530: 0a20 2020 2020 2020 2065 6c69 6620 7374  .        elif st
+00008540: 6163 6b5f 6d65 7468 6f64 203d 3d20 5374  ack_method == St
+00008550: 6163 6b4d 6574 686f 642e 524f 4255 5354  ackMethod.ROBUST
+00008560: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+00008570: 6767 6572 2e69 6e66 6f28 2264 6f20 726f  gger.info("do ro
+00008580: 6275 7374 2073 7562 7374 6163 6b69 6e67  bust substacking
+00008590: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
+000085a0: 5f63 6f72 7220 3d20 726f 6275 7374 5f73  _corr = robust_s
+000085b0: 7461 636b 2873 5f63 6f72 722c 2030 2e30  tack(s_corr, 0.0
+000085c0: 3031 290a 2020 2020 2020 2020 2020 2020  01).            
+000085d0: 745f 636f 7272 203d 2064 6174 6153 5f74  t_corr = dataS_t
+000085e0: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+000085f0: 6e5f 636f 7272 203d 206e 7769 6e0a 2020  n_corr = nwin.  
+00008600: 2020 2320 2065 6c69 6620 7374 6163 6b5f    #  elif stack_
+00008610: 6d65 7468 6f64 203d 3d20 2773 656c 6563  method == 'selec
+00008620: 7469 7665 273a 0a20 2020 2023 2020 2020  tive':.    #    
+00008630: 2020 7072 696e 7428 2764 6f20 7365 6c65    print('do sele
+00008640: 6374 6976 6520 7375 6273 7461 636b 696e  ctive substackin
+00008650: 6727 290a 2020 2020 2320 2020 2020 2073  g').    #      s
+00008660: 5f63 6f72 7220 3d20 7365 6c65 6374 6976  _corr = selectiv
+00008670: 655f 7374 6163 6b28 735f 636f 7272 2c30  e_stack(s_corr,0
+00008680: 2e30 3031 290a 2020 2020 2320 2020 2020  .001).    #     
+00008690: 2074 5f63 6f72 7220 3d20 6461 7461 535f   t_corr = dataS_
+000086a0: 745b 305d 0a20 2020 2023 2020 2020 2020  t[0].    #      
+000086b0: 6e5f 636f 7272 203d 206e 7769 6e0a 0a20  n_corr = nwin.. 
+000086c0: 2020 2023 2074 7269 6d20 7468 6520 4343     # trim the CC
+000086d0: 4673 2069 6e20 5b2d 6d61 786c 6167 206d  Fs in [-maxlag m
+000086e0: 6178 6c61 675d 0a20 2020 2074 203d 206e  axlag].    t = n
+000086f0: 702e 6172 616e 6765 282d 4e66 6674 3220  p.arange(-Nfft2 
+00008700: 2b20 312c 204e 6666 7432 2920 2a20 6474  + 1, Nfft2) * dt
+00008710: 0a20 2020 2069 6e64 203d 206e 702e 7768  .    ind = np.wh
+00008720: 6572 6528 6e70 2e61 6273 2874 2920 3c3d  ere(np.abs(t) <=
+00008730: 206d 6178 6c61 6729 5b30 5d0a 2020 2020   maxlag)[0].    
+00008740: 6966 2073 5f63 6f72 722e 6e64 696d 203d  if s_corr.ndim =
+00008750: 3d20 313a 0a20 2020 2020 2020 2073 5f63  = 1:.        s_c
+00008760: 6f72 7220 3d20 735f 636f 7272 5b69 6e64  orr = s_corr[ind
+00008770: 5d0a 2020 2020 656c 6966 2073 5f63 6f72  ].    elif s_cor
+00008780: 722e 6e64 696d 203d 3d20 323a 0a20 2020  r.ndim == 2:.   
+00008790: 2020 2020 2073 5f63 6f72 7220 3d20 735f       s_corr = s_
+000087a0: 636f 7272 5b3a 2c20 696e 645d 0a20 2020  corr[:, ind].   
+000087b0: 2072 6574 7572 6e20 735f 636f 7272 2c20   return s_corr, 
+000087c0: 745f 636f 7272 2c20 6e5f 636f 7272 2c20  t_corr, n_corr, 
+000087d0: 6e73 5f63 6f72 725b 3a2c 2069 6e64 5d0a  ns_corr[:, ind].
+000087e0: 0a0a 6465 6620 6363 5f70 6172 616d 6574  ..def cc_paramet
+000087f0: 6572 7328 6363 5f70 6172 612c 2063 6f6f  ers(cc_para, coo
+00008800: 722c 2074 636f 7272 2c20 6e63 6f72 722c  r, tcorr, ncorr,
+00008810: 2063 6f6d 7029 3a0a 2020 2020 2222 220a   comp):.    """.
+00008820: 2020 2020 7468 6973 2066 756e 6374 696f      this functio
+00008830: 6e20 6173 7365 6d62 6c65 7320 7468 6520  n assembles the 
+00008840: 7061 7261 6d65 7465 7273 2066 6f72 2074  parameters for t
+00008850: 6865 2063 6320 6675 6e63 7469 6f6e 2c20  he cc function, 
+00008860: 7768 6963 6820 6973 2075 7365 640a 2020  which is used.  
+00008870: 2020 7768 656e 2077 7269 7469 6e67 2074    when writing t
+00008880: 6865 6d20 696e 746f 2041 5344 4620 6669  hem into ASDF fi
+00008890: 6c65 730a 2020 2020 5041 5241 4d45 5445  les.    PARAMETE
+000088a0: 5253 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  RS:.    --------
+000088b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+000088c0: 2020 6363 5f70 6172 613a 2064 6963 7420    cc_para: dict 
+000088d0: 636f 6e74 6169 6e69 6e67 2070 6172 616d  containing param
+000088e0: 6574 6572 7320 7573 6564 2069 6e20 7468  eters used in th
+000088f0: 6520 6666 745f 6363 2073 7465 700a 2020  e fft_cc step.  
+00008900: 2020 636f 6f72 3a20 2020 2064 6963 7420    coor:    dict 
+00008910: 636f 6e74 6169 6e69 6e67 2063 6f6f 7264  containing coord
+00008920: 696e 6174 6573 2069 6e66 6f20 6f66 2074  inates info of t
+00008930: 6865 2073 6f75 7263 6520 616e 6420 7265  he source and re
+00008940: 6365 6976 6572 2073 7461 7469 6f6e 730a  ceiver stations.
+00008950: 2020 2020 7463 6f72 723a 2020 2074 696d      tcorr:   tim
+00008960: 6573 7461 6d70 206d 6174 7269 780a 2020  estamp matrix.  
+00008970: 2020 6e63 6f72 723a 2020 206d 6174 7269    ncorr:   matri
+00008980: 7820 6f66 206e 756d 6265 7220 6f66 2067  x of number of g
+00008990: 6f6f 6420 7365 676d 656e 7473 2066 6f72  ood segments for
+000089a0: 2065 6163 6820 7375 622d 7374 6163 6b2f   each sub-stack/
+000089b0: 6669 6e61 6c20 7374 6163 6b0a 2020 2020  final stack.    
+000089c0: 636f 6d70 3a20 2020 2032 2063 6861 7261  comp:    2 chara
+000089d0: 6374 6572 2073 7472 696e 6773 2066 6f72  cter strings for
+000089e0: 2074 6865 2063 726f 7373 2063 6f72 7265   the cross corre
+000089f0: 6c61 7469 6f6e 2063 6f6d 706f 6e65 6e74  lation component
+00008a00: 0a20 2020 2052 4554 5552 4e53 3a0a 2020  .    RETURNS:.  
+00008a10: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+00008a20: 2d2d 2d2d 0a20 2020 2070 6172 616d 6574  ----.    paramet
+00008a30: 6572 733a 2064 6963 7420 636f 6e74 6169  ers: dict contai
+00008a40: 6e69 6e67 2061 626f 7665 2069 6e66 6f20  ning above info 
+00008a50: 7573 6564 2066 6f72 206c 6174 6572 2073  used for later s
+00008a60: 7461 636b 696e 672f 706c 6f74 7469 6e67  tacking/plotting
+00008a70: 0a20 2020 2022 2222 0a20 2020 206c 6174  .    """.    lat
+00008a80: 5320 3d20 636f 6f72 5b22 6c61 7453 225d  S = coor["latS"]
+00008a90: 0a20 2020 206c 6f6e 5320 3d20 636f 6f72  .    lonS = coor
+00008aa0: 5b22 6c6f 6e53 225d 0a20 2020 206c 6174  ["lonS"].    lat
+00008ab0: 5220 3d20 636f 6f72 5b22 6c61 7452 225d  R = coor["latR"]
+00008ac0: 0a20 2020 206c 6f6e 5220 3d20 636f 6f72  .    lonR = coor
+00008ad0: 5b22 6c6f 6e52 225d 0a20 2020 2064 7420  ["lonR"].    dt 
+00008ae0: 3d20 6363 5f70 6172 615b 2264 7422 5d0a  = cc_para["dt"].
+00008af0: 2020 2020 6d61 786c 6167 203d 2063 635f      maxlag = cc_
+00008b00: 7061 7261 5b22 6d61 786c 6167 225d 0a20  para["maxlag"]. 
+00008b10: 2020 2073 7562 7374 6163 6b20 3d20 6363     substack = cc
+00008b20: 5f70 6172 615b 2273 7562 7374 6163 6b22  _para["substack"
+00008b30: 5d0a 2020 2020 6363 5f6d 6574 686f 6420  ].    cc_method 
+00008b40: 3d20 6363 5f70 6172 615b 2263 635f 6d65  = cc_para["cc_me
+00008b50: 7468 6f64 225d 0a0a 2020 2020 6469 7374  thod"]..    dist
+00008b60: 2c20 617a 692c 2062 617a 203d 206f 6273  , azi, baz = obs
+00008b70: 7079 2e67 656f 6465 7469 6373 2e62 6173  py.geodetics.bas
+00008b80: 652e 6770 7332 6469 7374 5f61 7a69 6d75  e.gps2dist_azimu
+00008b90: 7468 286c 6174 532c 206c 6f6e 532c 206c  th(latS, lonS, l
+00008ba0: 6174 522c 206c 6f6e 5229 0a20 2020 2070  atR, lonR).    p
+00008bb0: 6172 616d 6574 6572 7320 3d20 7b0a 2020  arameters = {.  
+00008bc0: 2020 2020 2020 2264 7422 3a20 6474 2c0a        "dt": dt,.
+00008bd0: 2020 2020 2020 2020 226d 6178 6c61 6722          "maxlag"
+00008be0: 3a20 696e 7428 6d61 786c 6167 292c 0a20  : int(maxlag),. 
+00008bf0: 2020 2020 2020 2022 6469 7374 223a 206e         "dist": n
+00008c00: 702e 666c 6f61 7433 3228 6469 7374 202f  p.float32(dist /
+00008c10: 2031 3030 3029 2c0a 2020 2020 2020 2020   1000),.        
+00008c20: 2261 7a69 223a 206e 702e 666c 6f61 7433  "azi": np.float3
+00008c30: 3228 617a 6929 2c0a 2020 2020 2020 2020  2(azi),.        
+00008c40: 2262 617a 223a 206e 702e 666c 6f61 7433  "baz": np.float3
+00008c50: 3228 6261 7a29 2c0a 2020 2020 2020 2020  2(baz),.        
+00008c60: 226c 6f6e 5322 3a20 6e70 2e66 6c6f 6174  "lonS": np.float
+00008c70: 3332 286c 6f6e 5329 2c0a 2020 2020 2020  32(lonS),.      
+00008c80: 2020 226c 6174 5322 3a20 6e70 2e66 6c6f    "latS": np.flo
+00008c90: 6174 3332 286c 6174 5329 2c0a 2020 2020  at32(latS),.    
+00008ca0: 2020 2020 226c 6f6e 5222 3a20 6e70 2e66      "lonR": np.f
+00008cb0: 6c6f 6174 3332 286c 6f6e 5229 2c0a 2020  loat32(lonR),.  
+00008cc0: 2020 2020 2020 226c 6174 5222 3a20 6e70        "latR": np
+00008cd0: 2e66 6c6f 6174 3332 286c 6174 5229 2c0a  .float32(latR),.
+00008ce0: 2020 2020 2020 2020 226e 676f 6f64 223a          "ngood":
+00008cf0: 206e 636f 7272 2c0a 2020 2020 2020 2020   ncorr,.        
+00008d00: 2263 635f 6d65 7468 6f64 223a 2063 635f  "cc_method": cc_
+00008d10: 6d65 7468 6f64 2c0a 2020 2020 2020 2020  method,.        
+00008d20: 2274 696d 6522 3a20 7463 6f72 722c 0a20  "time": tcorr,. 
+00008d30: 2020 2020 2020 2022 7375 6273 7461 636b         "substack
+00008d40: 223a 2073 7562 7374 6163 6b2c 0a20 2020  ": substack,.   
+00008d50: 2020 2020 2022 636f 6d70 223a 2063 6f6d       "comp": com
+00008d60: 702c 0a20 2020 207d 0a20 2020 2072 6574  p,.    }.    ret
+00008d70: 7572 6e20 7061 7261 6d65 7465 7273 0a0a  urn parameters..
+00008d80: 0a64 6566 2073 7461 636b 696e 6728 6363  .def stacking(cc
+00008d90: 5f61 7272 6179 2c20 6363 5f74 696d 652c  _array, cc_time,
+00008da0: 2063 635f 6e67 6f6f 642c 2073 7461 636b   cc_ngood, stack
+00008db0: 5f70 6172 6129 3a0a 2020 2020 2222 220a  _para):.    """.
+00008dc0: 2020 2020 7468 6973 2066 756e 6374 696f      this functio
+00008dd0: 6e20 7374 6163 6b73 2074 6865 2063 726f  n stacks the cro
+00008de0: 7373 2063 6f72 7265 6c61 7469 6f6e 2064  ss correlation d
+00008df0: 6174 6120 6163 636f 7264 696e 6720 746f  ata according to
+00008e00: 2074 6865 2075 7365 722d 6465 6669 6e65   the user-define
+00008e10: 6420 7375 6273 7461 636b 5f6c 656e 2070  d substack_len p
+00008e20: 6172 616d 6574 6572 0a0a 2020 2020 5041  arameter..    PA
+00008e30: 5241 4d45 5445 5253 3a0a 2020 2020 2d2d  RAMETERS:.    --
+00008e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008e50: 2d2d 2d2d 0a20 2020 2063 635f 6172 7261  ----.    cc_arra
+00008e60: 793a 2032 4420 6e75 6d70 7920 666c 6f61  y: 2D numpy floa
+00008e70: 7433 3220 6d61 7472 6978 2063 6f6e 7461  t32 matrix conta
+00008e80: 696e 696e 6720 616c 6c20 7365 676d 656e  ining all segmen
+00008e90: 7465 6420 6372 6f73 732d 636f 7272 656c  ted cross-correl
+00008ea0: 6174 696f 6e20 6461 7461 0a20 2020 2063  ation data.    c
+00008eb0: 635f 7469 6d65 3a20 2031 4420 6e75 6d70  c_time:  1D nump
+00008ec0: 7920 6172 7261 7920 6f66 2074 696d 6573  y array of times
+00008ed0: 7461 6d70 7320 666f 7220 6561 6368 2073  tamps for each s
+00008ee0: 6567 6d65 6e74 206f 6620 6363 5f61 7272  egment of cc_arr
+00008ef0: 6179 0a20 2020 2063 635f 6e67 6f6f 643a  ay.    cc_ngood:
+00008f00: 2031 4420 6e75 6d70 7920 696e 7431 3620   1D numpy int16 
+00008f10: 6d61 7472 6978 2073 686f 7769 6e67 2074  matrix showing t
+00008f20: 6865 206e 756d 6265 7220 6f66 2073 6567  he number of seg
+00008f30: 6d65 6e74 7320 666f 7220 6561 6368 2073  ments for each s
+00008f40: 7562 2d73 7461 636b 2061 6e64 2f6f 7220  ub-stack and/or 
+00008f50: 6675 6c6c 2073 7461 636b 0a20 2020 2073  full stack.    s
+00008f60: 7461 636b 5f70 6172 613a 2061 2064 6963  tack_para: a dic
+00008f70: 7420 636f 6e74 6169 6e69 6e67 2061 6c6c  t containing all
+00008f80: 2073 7461 636b 696e 6720 7061 7261 6d65   stacking parame
+00008f90: 7465 7273 0a0a 2020 2020 5245 5455 524e  ters..    RETURN
+00008fa0: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
+00008fb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+00008fc0: 2020 6363 5f61 7272 6179 2c20 6363 5f6e    cc_array, cc_n
+00008fd0: 676f 6f64 2c20 6363 5f74 696d 653a 2073  good, cc_time: s
+00008fe0: 616d 6520 746f 2074 6865 2069 6e70 7574  ame to the input
+00008ff0: 2070 6172 616d 6574 6572 7320 6275 7420   parameters but 
+00009000: 7769 7468 2061 626e 6f72 6d61 6c20 6372  with abnormal cr
+00009010: 6f73 732d 636f 7272 6561 6c74 696f 6e73  oss-correaltions
+00009020: 2072 656d 6f76 6564 0a20 2020 2061 6c6c   removed.    all
+00009030: 7374 6163 6b73 313a 2031 4420 6d61 7472  stacks1: 1D matr
+00009040: 6978 206f 6620 7374 6163 6b65 6420 6372  ix of stacked cr
+00009050: 6f73 732d 636f 7272 656c 6174 696f 6e20  oss-correlation 
+00009060: 6675 6e63 7469 6f6e 7320 6f76 6572 2061  functions over a
+00009070: 6c6c 2074 6865 2073 6567 6d65 6e74 730a  ll the segments.
+00009080: 2020 2020 6e73 7461 636b 733a 2020 2020      nstacks:    
+00009090: 6e75 6d62 6572 206f 6620 6f76 6572 616c  number of overal
+000090a0: 6c20 7365 676d 656e 7473 2066 6f72 2074  l segments for t
+000090b0: 6865 2066 696e 616c 2073 7461 636b 730a  he final stacks.
+000090c0: 2020 2020 2222 220a 2020 2020 2320 6c6f      """.    # lo
+000090d0: 6164 2075 7365 6675 6c20 7061 7261 6d65  ad useful parame
+000090e0: 7465 7273 2066 726f 6d20 6469 6374 0a20  ters from dict. 
+000090f0: 2020 2073 616d 705f 6672 6571 203d 2073     samp_freq = s
+00009100: 7461 636b 5f70 6172 615b 2273 616d 705f  tack_para["samp_
+00009110: 6672 6571 225d 0a20 2020 2073 6d65 7468  freq"].    smeth
+00009120: 6f64 203d 2073 7461 636b 5f70 6172 615b  od = stack_para[
+00009130: 2273 7461 636b 5f6d 6574 686f 6422 5d0a  "stack_method"].
+00009140: 2020 2020 6e70 7473 203d 2063 635f 6172      npts = cc_ar
+00009150: 7261 792e 7368 6170 655b 315d 0a0a 2020  ray.shape[1]..  
+00009160: 2020 2320 7265 6d6f 7665 2061 626e 6f72    # remove abnor
+00009170: 6d61 6c20 6461 7461 0a20 2020 2061 6d70  mal data.    amp
+00009180: 6d61 7820 3d20 6e70 2e6d 6178 2863 635f  max = np.max(cc_
+00009190: 6172 7261 792c 2061 7869 733d 3129 0a20  array, axis=1). 
+000091a0: 2020 2074 696e 6478 203d 206e 702e 7768     tindx = np.wh
+000091b0: 6572 6528 2861 6d70 6d61 7820 3c20 3230  ere((ampmax < 20
+000091c0: 202a 206e 702e 6d65 6469 616e 2861 6d70   * np.median(amp
+000091d0: 6d61 7829 2920 2620 2861 6d70 6d61 7820  max)) & (ampmax 
+000091e0: 3e20 3029 295b 305d 0a20 2020 2069 6620  > 0))[0].    if 
+000091f0: 6e6f 7420 6c65 6e28 7469 6e64 7829 3a0a  not len(tindx):.
+00009200: 2020 2020 2020 2020 616c 6c73 7461 636b          allstack
+00009210: 7331 203d 205b 5d0a 2020 2020 2020 2020  s1 = [].        
+00009220: 616c 6c73 7461 636b 7332 203d 205b 5d0a  allstacks2 = [].
+00009230: 2020 2020 2020 2020 616c 6c73 7461 636b          allstack
+00009240: 7333 203d 205b 5d0a 2020 2020 2020 2020  s3 = [].        
+00009250: 6e73 7461 636b 7320 3d20 300a 2020 2020  nstacks = 0.    
+00009260: 2020 2020 6363 5f61 7272 6179 203d 205b      cc_array = [
+00009270: 5d0a 2020 2020 2020 2020 6363 5f6e 676f  ].        cc_ngo
+00009280: 6f64 203d 205b 5d0a 2020 2020 2020 2020  od = [].        
+00009290: 6363 5f74 696d 6520 3d20 5b5d 0a20 2020  cc_time = [].   
+000092a0: 2020 2020 2072 6574 7572 6e20 6363 5f61       return cc_a
+000092b0: 7272 6179 2c20 6363 5f6e 676f 6f64 2c20  rray, cc_ngood, 
+000092c0: 6363 5f74 696d 652c 2061 6c6c 7374 6163  cc_time, allstac
+000092d0: 6b73 312c 2061 6c6c 7374 6163 6b73 322c  ks1, allstacks2,
+000092e0: 2061 6c6c 7374 6163 6b73 332c 206e 7374   allstacks3, nst
+000092f0: 6163 6b73 0a20 2020 2065 6c73 653a 0a20  acks.    else:. 
+00009300: 2020 2020 2020 2023 2072 656d 6f76 6520         # remove 
+00009310: 6f6e 6573 2077 6974 6820 6261 6420 616d  ones with bad am
+00009320: 706c 6974 7564 650a 2020 2020 2020 2020  plitude.        
+00009330: 6363 5f61 7272 6179 203d 2063 635f 6172  cc_array = cc_ar
+00009340: 7261 795b 7469 6e64 782c 203a 5d0a 2020  ray[tindx, :].  
+00009350: 2020 2020 2020 6363 5f74 696d 6520 3d20        cc_time = 
+00009360: 6363 5f74 696d 655b 7469 6e64 785d 0a20  cc_time[tindx]. 
+00009370: 2020 2020 2020 2063 635f 6e67 6f6f 6420         cc_ngood 
+00009380: 3d20 6363 5f6e 676f 6f64 5b74 696e 6478  = cc_ngood[tindx
+00009390: 5d0a 0a20 2020 2020 2020 2023 2064 6f20  ]..        # do 
+000093a0: 7374 6163 6b69 6e67 0a20 2020 2020 2020  stacking.       
+000093b0: 2061 6c6c 7374 6163 6b73 3120 3d20 6e70   allstacks1 = np
+000093c0: 2e7a 6572 6f73 286e 7074 732c 2064 7479  .zeros(npts, dty
+000093d0: 7065 3d6e 702e 666c 6f61 7433 3229 0a20  pe=np.float32). 
+000093e0: 2020 2020 2020 2061 6c6c 7374 6163 6b73         allstacks
+000093f0: 3220 3d20 6e70 2e7a 6572 6f73 286e 7074  2 = np.zeros(npt
+00009400: 732c 2064 7479 7065 3d6e 702e 666c 6f61  s, dtype=np.floa
+00009410: 7433 3229 0a20 2020 2020 2020 2061 6c6c  t32).        all
+00009420: 7374 6163 6b73 3320 3d20 6e70 2e7a 6572  stacks3 = np.zer
+00009430: 6f73 286e 7074 732c 2064 7479 7065 3d6e  os(npts, dtype=n
+00009440: 702e 666c 6f61 7433 3229 0a0a 2020 2020  p.float32)..    
+00009450: 2020 2020 6966 2073 6d65 7468 6f64 203d      if smethod =
+00009460: 3d20 5374 6163 6b4d 6574 686f 642e 4c49  = StackMethod.LI
+00009470: 4e45 4152 3a0a 2020 2020 2020 2020 2020  NEAR:.          
+00009480: 2020 616c 6c73 7461 636b 7331 203d 206e    allstacks1 = n
+00009490: 702e 6d65 616e 2863 635f 6172 7261 792c  p.mean(cc_array,
+000094a0: 2061 7869 733d 3029 0a20 2020 2020 2020   axis=0).       
+000094b0: 2065 6c69 6620 736d 6574 686f 6420 3d3d   elif smethod ==
+000094c0: 2053 7461 636b 4d65 7468 6f64 2e50 5753   StackMethod.PWS
+000094d0: 3a0a 2020 2020 2020 2020 2020 2020 616c  :.            al
+000094e0: 6c73 7461 636b 7331 203d 2070 7773 2863  lstacks1 = pws(c
+000094f0: 635f 6172 7261 792c 2073 616d 705f 6672  c_array, samp_fr
+00009500: 6571 290a 2020 2020 2020 2020 656c 6966  eq).        elif
+00009510: 2073 6d65 7468 6f64 203d 3d20 5374 6163   smethod == Stac
+00009520: 6b4d 6574 686f 642e 524f 4255 5354 3a0a  kMethod.ROBUST:.
+00009530: 2020 2020 2020 2020 2020 2020 616c 6c73              alls
+00009540: 7461 636b 7331 2c20 772c 206e 7374 6570  tacks1, w, nstep
+00009550: 203d 2072 6f62 7573 745f 7374 6163 6b28   = robust_stack(
+00009560: 6363 5f61 7272 6179 2c20 302e 3030 3129  cc_array, 0.001)
+00009570: 0a20 2020 2020 2020 2065 6c69 6620 736d  .        elif sm
+00009580: 6574 686f 6420 3d3d 2053 7461 636b 4d65  ethod == StackMe
+00009590: 7468 6f64 2e41 5554 4f5f 434f 5641 5249  thod.AUTO_COVARI
+000095a0: 414e 4345 3a0a 2020 2020 2020 2020 2020  ANCE:.          
+000095b0: 2020 616c 6c73 7461 636b 7331 203d 2061    allstacks1 = a
+000095c0: 6461 7074 6976 655f 6669 6c74 6572 2863  daptive_filter(c
+000095d0: 635f 6172 7261 792c 2031 290a 2020 2020  c_array, 1).    
+000095e0: 2020 2020 656c 6966 2073 6d65 7468 6f64      elif smethod
+000095f0: 203d 3d20 5374 6163 6b4d 6574 686f 642e   == StackMethod.
+00009600: 4e52 4f4f 543a 0a20 2020 2020 2020 2020  NROOT:.         
+00009610: 2020 2061 6c6c 7374 6163 6b73 3120 3d20     allstacks1 = 
+00009620: 6e72 6f6f 745f 7374 6163 6b28 6363 5f61  nroot_stack(cc_a
+00009630: 7272 6179 2c20 3229 0a20 2020 2020 2020  rray, 2).       
+00009640: 2065 6c69 6620 736d 6574 686f 6420 3d3d   elif smethod ==
+00009650: 2053 7461 636b 4d65 7468 6f64 2e41 4c4c   StackMethod.ALL
+00009660: 3a0a 2020 2020 2020 2020 2020 2020 616c  :.            al
+00009670: 6c73 7461 636b 7331 203d 206e 702e 6d65  lstacks1 = np.me
+00009680: 616e 2863 635f 6172 7261 792c 2061 7869  an(cc_array, axi
+00009690: 733d 3029 0a20 2020 2020 2020 2020 2020  s=0).           
+000096a0: 2061 6c6c 7374 6163 6b73 3220 3d20 7077   allstacks2 = pw
+000096b0: 7328 6363 5f61 7272 6179 2c20 7361 6d70  s(cc_array, samp
+000096c0: 5f66 7265 7129 0a20 2020 2020 2020 2020  _freq).         
+000096d0: 2020 2061 6c6c 7374 6163 6b73 332c 2077     allstacks3, w
+000096e0: 2c20 6e73 7465 7020 3d20 726f 6275 7374  , nstep = robust
+000096f0: 5f73 7461 636b 2863 635f 6172 7261 792c  _stack(cc_array,
+00009700: 2030 2e30 3031 290a 2020 2020 2020 2020   0.001).        
+00009710: 6e73 7461 636b 7320 3d20 6e70 2e73 756d  nstacks = np.sum
+00009720: 2863 635f 6e67 6f6f 6429 0a0a 2020 2020  (cc_ngood)..    
+00009730: 2320 676f 6f64 2074 6f20 7265 7475 726e  # good to return
+00009740: 0a20 2020 2072 6574 7572 6e20 6363 5f61  .    return cc_a
+00009750: 7272 6179 2c20 6363 5f6e 676f 6f64 2c20  rray, cc_ngood, 
+00009760: 6363 5f74 696d 652c 2061 6c6c 7374 6163  cc_time, allstac
+00009770: 6b73 312c 2061 6c6c 7374 6163 6b73 322c  ks1, allstacks2,
+00009780: 2061 6c6c 7374 6163 6b73 332c 206e 7374   allstacks3, nst
+00009790: 6163 6b73 0a0a 0a64 6566 2073 7461 636b  acks...def stack
+000097a0: 696e 675f 726d 6128 6363 5f61 7272 6179  ing_rma(cc_array
+000097b0: 2c20 6363 5f74 696d 652c 2063 635f 6e67  , cc_time, cc_ng
+000097c0: 6f6f 642c 2073 7461 636b 5f70 6172 6129  ood, stack_para)
+000097d0: 3a0a 2020 2020 2222 220a 2020 2020 7468  :.    """.    th
+000097e0: 6973 2066 756e 6374 696f 6e20 7374 6163  is function stac
+000097f0: 6b73 2074 6865 2063 726f 7373 2063 6f72  ks the cross cor
+00009800: 7265 6c61 7469 6f6e 2064 6174 6120 6163  relation data ac
+00009810: 636f 7264 696e 6720 746f 2074 6865 2075  cording to the u
+00009820: 7365 722d 6465 6669 6e65 6420 7375 6273  ser-defined subs
+00009830: 7461 636b 5f6c 656e 2070 6172 616d 6574  tack_len paramet
+00009840: 6572 0a20 2020 2050 4152 414d 4554 4552  er.    PARAMETER
+00009850: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
+00009860: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+00009870: 2020 6363 5f61 7272 6179 3a20 3244 206e    cc_array: 2D n
+00009880: 756d 7079 2066 6c6f 6174 3332 206d 6174  umpy float32 mat
+00009890: 7269 7820 636f 6e74 6169 6e69 6e67 2061  rix containing a
+000098a0: 6c6c 2073 6567 6d65 6e74 6564 2063 726f  ll segmented cro
+000098b0: 7373 2d63 6f72 7265 6c61 7469 6f6e 2064  ss-correlation d
+000098c0: 6174 610a 2020 2020 6363 5f74 696d 653a  ata.    cc_time:
+000098d0: 2020 3144 206e 756d 7079 2061 7272 6179    1D numpy array
+000098e0: 206f 6620 7469 6d65 7374 616d 7073 2066   of timestamps f
+000098f0: 6f72 2065 6163 6820 7365 676d 656e 7420  or each segment 
+00009900: 6f66 2063 635f 6172 7261 790a 2020 2020  of cc_array.    
+00009910: 6363 5f6e 676f 6f64 3a20 3144 206e 756d  cc_ngood: 1D num
+00009920: 7079 2069 6e74 3136 206d 6174 7269 7820  py int16 matrix 
+00009930: 7368 6f77 696e 6720 7468 6520 6e75 6d62  showing the numb
+00009940: 6572 206f 6620 7365 676d 656e 7473 2066  er of segments f
+00009950: 6f72 2065 6163 6820 7375 622d 7374 6163  or each sub-stac
+00009960: 6b20 616e 642f 6f72 2066 756c 6c20 7374  k and/or full st
+00009970: 6163 6b0a 2020 2020 7374 6163 6b5f 7061  ack.    stack_pa
+00009980: 7261 3a20 6120 6469 6374 2063 6f6e 7461  ra: a dict conta
+00009990: 696e 696e 6720 616c 6c20 7374 6163 6b69  ining all stacki
+000099a0: 6e67 2070 6172 616d 6574 6572 730a 2020  ng parameters.  
+000099b0: 2020 5245 5455 524e 533a 0a20 2020 202d    RETURNS:.    -
+000099c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000099d0: 2d2d 2d2d 2d0a 2020 2020 6363 5f61 7272  -----.    cc_arr
+000099e0: 6179 2c20 6363 5f6e 676f 6f64 2c20 6363  ay, cc_ngood, cc
+000099f0: 5f74 696d 653a 2073 616d 6520 746f 2074  _time: same to t
+00009a00: 6865 2069 6e70 7574 2070 6172 616d 6574  he input paramet
+00009a10: 6572 7320 6275 7420 7769 7468 2061 626e  ers but with abn
+00009a20: 6f72 6d61 6c20 6372 6f73 732d 636f 7272  ormal cross-corr
+00009a30: 6561 6c74 696f 6e73 2072 656d 6f76 6564  ealtions removed
+00009a40: 0a20 2020 2061 6c6c 7374 6163 6b73 313a  .    allstacks1:
+00009a50: 2031 4420 6d61 7472 6978 206f 6620 7374   1D matrix of st
+00009a60: 6163 6b65 6420 6372 6f73 732d 636f 7272  acked cross-corr
+00009a70: 656c 6174 696f 6e20 6675 6e63 7469 6f6e  elation function
+00009a80: 7320 6f76 6572 2061 6c6c 2074 6865 2073  s over all the s
+00009a90: 6567 6d65 6e74 730a 2020 2020 6e73 7461  egments.    nsta
+00009aa0: 636b 733a 2020 2020 6e75 6d62 6572 206f  cks:    number o
+00009ab0: 6620 6f76 6572 616c 6c20 7365 676d 656e  f overall segmen
+00009ac0: 7473 2066 6f72 2074 6865 2066 696e 616c  ts for the final
+00009ad0: 2073 7461 636b 730a 2020 2020 2222 220a   stacks.    """.
+00009ae0: 2020 2020 2320 6c6f 6164 2075 7365 6675      # load usefu
+00009af0: 6c20 7061 7261 6d65 7465 7273 2066 726f  l parameters fro
+00009b00: 6d20 6469 6374 0a20 2020 2073 616d 705f  m dict.    samp_
+00009b10: 6672 6571 203d 2073 7461 636b 5f70 6172  freq = stack_par
+00009b20: 615b 2273 616d 705f 6672 6571 225d 0a20  a["samp_freq"]. 
+00009b30: 2020 2073 6d65 7468 6f64 203d 2073 7461     smethod = sta
+00009b40: 636b 5f70 6172 615b 2273 7461 636b 5f6d  ck_para["stack_m
+00009b50: 6574 686f 6422 5d0a 2020 2020 726d 615f  ethod"].    rma_
+00009b60: 7375 6273 7461 636b 203d 2073 7461 636b  substack = stack
+00009b70: 5f70 6172 615b 2272 6d61 5f73 7562 7374  _para["rma_subst
+00009b80: 6163 6b22 5d0a 2020 2020 726d 615f 7374  ack"].    rma_st
+00009b90: 6570 203d 2073 7461 636b 5f70 6172 615b  ep = stack_para[
+00009ba0: 2272 6d61 5f73 7465 7022 5d0a 2020 2020  "rma_step"].    
+00009bb0: 7374 6172 745f 6461 7465 203d 2073 7461  start_date = sta
+00009bc0: 636b 5f70 6172 615b 2273 7461 7274 5f64  ck_para["start_d
+00009bd0: 6174 6522 5d0a 2020 2020 656e 645f 6461  ate"].    end_da
+00009be0: 7465 203d 2073 7461 636b 5f70 6172 615b  te = stack_para[
+00009bf0: 2265 6e64 5f64 6174 6522 5d0a 2020 2020  "end_date"].    
+00009c00: 6e70 7473 203d 2063 635f 6172 7261 792e  npts = cc_array.
+00009c10: 7368 6170 655b 315d 0a0a 2020 2020 2320  shape[1]..    # 
+00009c20: 7265 6d6f 7665 2061 626e 6f72 6d61 6c20  remove abnormal 
+00009c30: 6461 7461 0a20 2020 2061 6d70 6d61 7820  data.    ampmax 
+00009c40: 3d20 6e70 2e6d 6178 2863 635f 6172 7261  = np.max(cc_arra
+00009c50: 792c 2061 7869 733d 3129 0a20 2020 2074  y, axis=1).    t
+00009c60: 696e 6478 203d 206e 702e 7768 6572 6528  indx = np.where(
+00009c70: 2861 6d70 6d61 7820 3c20 3230 202a 206e  (ampmax < 20 * n
+00009c80: 702e 6d65 6469 616e 2861 6d70 6d61 7829  p.median(ampmax)
+00009c90: 2920 2620 2861 6d70 6d61 7820 3e20 3029  ) & (ampmax > 0)
+00009ca0: 295b 305d 0a20 2020 2069 6620 6e6f 7420  )[0].    if not 
+00009cb0: 6c65 6e28 7469 6e64 7829 3a0a 2020 2020  len(tindx):.    
+00009cc0: 2020 2020 616c 6c73 7461 636b 7331 203d      allstacks1 =
+00009cd0: 205b 5d0a 2020 2020 2020 2020 616c 6c73   [].        alls
+00009ce0: 7461 636b 7332 203d 205b 5d0a 2020 2020  tacks2 = [].    
+00009cf0: 2020 2020 6e73 7461 636b 7320 3d20 300a      nstacks = 0.
+00009d00: 2020 2020 2020 2020 6363 5f61 7272 6179          cc_array
+00009d10: 203d 205b 5d0a 2020 2020 2020 2020 6363   = [].        cc
+00009d20: 5f6e 676f 6f64 203d 205b 5d0a 2020 2020  _ngood = [].    
+00009d30: 2020 2020 6363 5f74 696d 6520 3d20 5b5d      cc_time = []
+00009d40: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00009d50: 6363 5f61 7272 6179 2c20 6363 5f6e 676f  cc_array, cc_ngo
+00009d60: 6f64 2c20 6363 5f74 696d 652c 2061 6c6c  od, cc_time, all
+00009d70: 7374 6163 6b73 312c 2061 6c6c 7374 6163  stacks1, allstac
+00009d80: 6b73 322c 206e 7374 6163 6b73 0a20 2020  ks2, nstacks.   
+00009d90: 2065 6c73 653a 0a20 2020 2020 2020 2023   else:.        #
+00009da0: 2072 656d 6f76 6520 6f6e 6573 2077 6974   remove ones wit
+00009db0: 6820 6261 6420 616d 706c 6974 7564 650a  h bad amplitude.
+00009dc0: 2020 2020 2020 2020 6363 5f61 7272 6179          cc_array
+00009dd0: 203d 2063 635f 6172 7261 795b 7469 6e64   = cc_array[tind
+00009de0: 782c 203a 5d0a 2020 2020 2020 2020 6363  x, :].        cc
+00009df0: 5f74 696d 6520 3d20 6363 5f74 696d 655b  _time = cc_time[
+00009e00: 7469 6e64 785d 0a20 2020 2020 2020 2063  tindx].        c
+00009e10: 635f 6e67 6f6f 6420 3d20 6363 5f6e 676f  c_ngood = cc_ngo
+00009e20: 6f64 5b74 696e 6478 5d0a 0a20 2020 2020  od[tindx]..     
+00009e30: 2020 2023 2064 6f20 7375 6273 7461 636b     # do substack
+00009e40: 730a 2020 2020 2020 2020 6966 2072 6d61  s.        if rma
+00009e50: 5f73 7562 7374 6163 6b3a 0a20 2020 2020  _substack:.     
+00009e60: 2020 2020 2020 2074 7374 6172 7420 3d20         tstart = 
+00009e70: 6f62 7370 792e 5554 4344 6174 6554 696d  obspy.UTCDateTim
+00009e80: 6528 7374 6172 745f 6461 7465 2920 2d20  e(start_date) - 
+00009e90: 6f62 7370 792e 5554 4344 6174 6554 696d  obspy.UTCDateTim
+00009ea0: 6528 3139 3730 2c20 312c 2031 290a 2020  e(1970, 1, 1).  
+00009eb0: 2020 2020 2020 2020 2020 7465 6e64 203d            tend =
+00009ec0: 206f 6273 7079 2e55 5443 4461 7465 5469   obspy.UTCDateTi
+00009ed0: 6d65 2865 6e64 5f64 6174 6529 202d 206f  me(end_date) - o
+00009ee0: 6273 7079 2e55 5443 4461 7465 5469 6d65  bspy.UTCDateTime
+00009ef0: 2831 3937 302c 2031 2c20 3129 0a20 2020  (1970, 1, 1).   
+00009f00: 2020 2020 2020 2020 2074 7469 6d65 203d           ttime =
+00009f10: 2074 7374 6172 740a 2020 2020 2020 2020   tstart.        
+00009f20: 2020 2020 6e73 7461 636b 203d 2069 6e74      nstack = int
+00009f30: 286e 702e 726f 756e 6428 2874 656e 6420  (np.round((tend 
+00009f40: 2d20 7473 7461 7274 2920 2f20 2872 6d61  - tstart) / (rma
+00009f50: 5f73 7465 7020 2a20 3336 3030 2929 290a  _step * 3600))).
+00009f60: 2020 2020 2020 2020 2020 2020 6e63 635f              ncc_
+00009f70: 6172 7261 7920 3d20 6e70 2e7a 6572 6f73  array = np.zeros
+00009f80: 2873 6861 7065 3d28 6e73 7461 636b 2c20  (shape=(nstack, 
+00009f90: 6e70 7473 292c 2064 7479 7065 3d6e 702e  npts), dtype=np.
+00009fa0: 666c 6f61 7433 3229 0a20 2020 2020 2020  float32).       
+00009fb0: 2020 2020 206e 6363 5f74 696d 6520 3d20       ncc_time = 
+00009fc0: 6e70 2e7a 6572 6f73 286e 7374 6163 6b2c  np.zeros(nstack,
+00009fd0: 2064 7479 7065 3d6e 702e 666c 6f61 7429   dtype=np.float)
+00009fe0: 0a20 2020 2020 2020 2020 2020 206e 6363  .            ncc
+00009ff0: 5f6e 676f 6f64 203d 206e 702e 7a65 726f  _ngood = np.zero
+0000a000: 7328 6e73 7461 636b 2c20 6474 7970 653d  s(nstack, dtype=
+0000a010: 6e70 2e69 6e74 290a 0a20 2020 2020 2020  np.int)..       
+0000a020: 2020 2020 2023 206c 6f6f 7020 7468 726f       # loop thro
+0000a030: 7567 6820 6561 6368 2074 696d 650a 2020  ugh each time.  
+0000a040: 2020 2020 2020 2020 2020 666f 7220 6969            for ii
+0000a050: 2069 6e20 7261 6e67 6528 6e73 7461 636b   in range(nstack
+0000a060: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000a070: 2020 2073 696e 6478 203d 206e 702e 7768     sindx = np.wh
+0000a080: 6572 6528 2863 635f 7469 6d65 203e 3d20  ere((cc_time >= 
+0000a090: 7474 696d 6529 2026 2028 6363 5f74 696d  ttime) & (cc_tim
+0000a0a0: 6520 3c20 7474 696d 6520 2b20 726d 615f  e < ttime + rma_
+0000a0b0: 7375 6273 7461 636b 202a 2033 3630 3029  substack * 3600)
+0000a0c0: 295b 305d 0a0a 2020 2020 2020 2020 2020  )[0]..          
+0000a0d0: 2020 2020 2020 2320 7768 656e 2074 6865        # when the
+0000a0e0: 7265 2061 7265 2064 6174 6120 696e 2074  re are data in t
+0000a0f0: 6865 2074 696d 6520 7769 6e64 6f77 0a20  he time window. 
+0000a100: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000a110: 6620 6c65 6e28 7369 6e64 7829 3a0a 2020  f len(sindx):.  
+0000a120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a130: 2020 6e63 635f 6172 7261 795b 6969 5d20    ncc_array[ii] 
+0000a140: 3d20 6e70 2e6d 6561 6e28 6363 5f61 7272  = np.mean(cc_arr
+0000a150: 6179 5b73 696e 6478 5d2c 2061 7869 733d  ay[sindx], axis=
+0000a160: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
+0000a170: 2020 2020 2020 206e 6363 5f74 696d 655b         ncc_time[
+0000a180: 6969 5d20 3d20 7474 696d 650a 2020 2020  ii] = ttime.    
+0000a190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1a0: 6e63 635f 6e67 6f6f 645b 6969 5d20 3d20  ncc_ngood[ii] = 
+0000a1b0: 6e70 2e73 756d 2863 635f 6e67 6f6f 645b  np.sum(cc_ngood[
+0000a1c0: 7369 6e64 785d 2c20 6178 6973 3d30 290a  sindx], axis=0).
+0000a1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1e0: 7474 696d 6520 2b3d 2072 6d61 5f73 7465  ttime += rma_ste
+0000a1f0: 7020 2a20 3336 3030 0a0a 2020 2020 2020  p * 3600..      
+0000a200: 2020 2020 2020 2320 7265 6d6f 7665 2062        # remove b
+0000a210: 6164 206f 6e65 730a 2020 2020 2020 2020  ad ones.        
+0000a220: 2020 2020 7469 6e64 7820 3d20 6e70 2e77      tindx = np.w
+0000a230: 6865 7265 286e 6363 5f6e 676f 6f64 203e  here(ncc_ngood >
+0000a240: 2030 295b 305d 0a20 2020 2020 2020 2020   0)[0].         
+0000a250: 2020 206e 6363 5f61 7272 6179 203d 206e     ncc_array = n
+0000a260: 6363 5f61 7272 6179 5b74 696e 6478 5d0a  cc_array[tindx].
+0000a270: 2020 2020 2020 2020 2020 2020 6e63 635f              ncc_
+0000a280: 7469 6d65 203d 206e 6363 5f74 696d 655b  time = ncc_time[
+0000a290: 7469 6e64 785d 0a20 2020 2020 2020 2020  tindx].         
+0000a2a0: 2020 206e 6363 5f6e 676f 6f64 203d 206e     ncc_ngood = n
+0000a2b0: 6363 5f6e 676f 6f64 5b74 696e 6478 5d0a  cc_ngood[tindx].
+0000a2c0: 0a20 2020 2020 2020 2023 2064 6f20 7374  .        # do st
+0000a2d0: 6163 6b69 6e67 0a20 2020 2020 2020 2061  acking.        a
+0000a2e0: 6c6c 7374 6163 6b73 3120 3d20 6e70 2e7a  llstacks1 = np.z
+0000a2f0: 6572 6f73 286e 7074 732c 2064 7479 7065  eros(npts, dtype
+0000a300: 3d6e 702e 666c 6f61 7433 3229 0a20 2020  =np.float32).   
+0000a310: 2020 2020 2061 6c6c 7374 6163 6b73 3220       allstacks2 
+0000a320: 3d20 6e70 2e7a 6572 6f73 286e 7074 732c  = np.zeros(npts,
+0000a330: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+0000a340: 3229 0a20 2020 2020 2020 2061 6c6c 7374  2).        allst
+0000a350: 6163 6b73 3320 3d20 6e70 2e7a 6572 6f73  acks3 = np.zeros
+0000a360: 286e 7074 732c 2064 7479 7065 3d6e 702e  (npts, dtype=np.
+0000a370: 666c 6f61 7433 3229 0a20 2020 2020 2020  float32).       
+0000a380: 2061 6c6c 7374 6163 6b73 3420 3d20 6e70   allstacks4 = np
+0000a390: 2e7a 6572 6f73 286e 7074 732c 2064 7479  .zeros(npts, dty
+0000a3a0: 7065 3d6e 702e 666c 6f61 7433 3229 0a0a  pe=np.float32)..
+0000a3b0: 2020 2020 2020 2020 6966 2073 6d65 7468          if smeth
+0000a3c0: 6f64 203d 3d20 5374 6163 6b4d 6574 686f  od == StackMetho
+0000a3d0: 642e 4c49 4e45 4152 3a0a 2020 2020 2020  d.LINEAR:.      
+0000a3e0: 2020 2020 2020 616c 6c73 7461 636b 7331        allstacks1
+0000a3f0: 203d 206e 702e 6d65 616e 2863 635f 6172   = np.mean(cc_ar
+0000a400: 7261 792c 2061 7869 733d 3029 0a20 2020  ray, axis=0).   
+0000a410: 2020 2020 2065 6c69 6620 736d 6574 686f       elif smetho
+0000a420: 6420 3d3d 2053 7461 636b 4d65 7468 6f64  d == StackMethod
+0000a430: 2e50 5753 3a0a 2020 2020 2020 2020 2020  .PWS:.          
+0000a440: 2020 616c 6c73 7461 636b 7331 203d 2070    allstacks1 = p
+0000a450: 7773 2863 635f 6172 7261 792c 2073 616d  ws(cc_array, sam
+0000a460: 705f 6672 6571 290a 2020 2020 2020 2020  p_freq).        
+0000a470: 656c 6966 2073 6d65 7468 6f64 203d 3d20  elif smethod == 
+0000a480: 5374 6163 6b4d 6574 686f 642e 524f 4255  StackMethod.ROBU
+0000a490: 5354 3a0a 2020 2020 2020 2020 2020 2020  ST:.            
+0000a4a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000a4b0: 2020 616c 6c73 7461 636b 7331 2c0a 2020    allstacks1,.  
+0000a4c0: 2020 2020 2020 2020 2020 2020 2020 772c                w,
+0000a4d0: 0a20 2020 2020 2020 2020 2020 2029 203d  .            ) =
+0000a4e0: 2072 6f62 7573 745f 7374 6163 6b28 6363   robust_stack(cc
+0000a4f0: 5f61 7272 6179 2c20 302e 3030 3129 0a20  _array, 0.001). 
+0000a500: 2020 2020 2020 2065 6c69 6620 736d 6574         elif smet
+0000a510: 686f 6420 3d3d 2053 7461 636b 4d65 7468  hod == StackMeth
+0000a520: 6f64 2e53 454c 4543 5449 5645 3a0a 2020  od.SELECTIVE:.  
+0000a530: 2020 2020 2020 2020 2020 616c 6c73 7461            allsta
+0000a540: 636b 7331 203d 2073 656c 6563 7469 7665  cks1 = selective
+0000a550: 5f73 7461 636b 2863 635f 6172 7261 792c  _stack(cc_array,
+0000a560: 2030 2e30 3031 290a 2020 2020 2020 2020   0.001).        
+0000a570: 656c 6966 2073 6d65 7468 6f64 203d 3d20  elif smethod == 
+0000a580: 5374 6163 6b4d 6574 686f 642e 414c 4c3a  StackMethod.ALL:
+0000a590: 0a20 2020 2020 2020 2020 2020 2061 6c6c  .            all
+0000a5a0: 7374 6163 6b73 3120 3d20 6e70 2e6d 6561  stacks1 = np.mea
+0000a5b0: 6e28 6363 5f61 7272 6179 2c20 6178 6973  n(cc_array, axis
+0000a5c0: 3d30 290a 2020 2020 2020 2020 2020 2020  =0).            
+0000a5d0: 616c 6c73 7461 636b 7332 203d 2070 7773  allstacks2 = pws
+0000a5e0: 2863 635f 6172 7261 792c 2073 616d 705f  (cc_array, samp_
+0000a5f0: 6672 6571 290a 2020 2020 2020 2020 2020  freq).          
+0000a600: 2020 616c 6c73 7461 636b 7333 203d 2072    allstacks3 = r
+0000a610: 6f62 7573 745f 7374 6163 6b28 6363 5f61  obust_stack(cc_a
+0000a620: 7272 6179 2c20 302e 3030 3129 0a20 2020  rray, 0.001).   
+0000a630: 2020 2020 2020 2020 2061 6c6c 7374 6163           allstac
+0000a640: 6b73 3420 3d20 7365 6c65 6374 6976 655f  ks4 = selective_
+0000a650: 7374 6163 6b28 6363 5f61 7272 6179 2c20  stack(cc_array, 
+0000a660: 302e 3030 3129 0a20 2020 2020 2020 206e  0.001).        n
+0000a670: 7374 6163 6b73 203d 206e 702e 7375 6d28  stacks = np.sum(
+0000a680: 6363 5f6e 676f 6f64 290a 0a20 2020 2023  cc_ngood)..    #
+0000a690: 2072 6570 6c61 6365 2074 6865 2061 7272   replace the arr
+0000a6a0: 6179 2066 6f72 2073 7562 7374 6163 6b73  ay for substacks
+0000a6b0: 0a20 2020 2069 6620 726d 615f 7375 6273  .    if rma_subs
+0000a6c0: 7461 636b 3a0a 2020 2020 2020 2020 6363  tack:.        cc
+0000a6d0: 5f61 7272 6179 203d 206e 6363 5f61 7272  _array = ncc_arr
+0000a6e0: 6179 0a20 2020 2020 2020 2063 635f 7469  ay.        cc_ti
+0000a6f0: 6d65 203d 206e 6363 5f74 696d 650a 2020  me = ncc_time.  
+0000a700: 2020 2020 2020 6363 5f6e 676f 6f64 203d        cc_ngood =
+0000a710: 206e 6363 5f6e 676f 6f64 0a0a 2020 2020   ncc_ngood..    
+0000a720: 2320 676f 6f64 2074 6f20 7265 7475 726e  # good to return
+0000a730: 0a20 2020 2072 6574 7572 6e20 280a 2020  .    return (.  
+0000a740: 2020 2020 2020 6363 5f61 7272 6179 2c0a        cc_array,.
+0000a750: 2020 2020 2020 2020 6363 5f6e 676f 6f64          cc_ngood
+0000a760: 2c0a 2020 2020 2020 2020 6363 5f74 696d  ,.        cc_tim
+0000a770: 652c 0a20 2020 2020 2020 2061 6c6c 7374  e,.        allst
+0000a780: 6163 6b73 312c 0a20 2020 2020 2020 2061  acks1,.        a
+0000a790: 6c6c 7374 6163 6b73 322c 0a20 2020 2020  llstacks2,.     
+0000a7a0: 2020 2061 6c6c 7374 6163 6b73 332c 0a20     allstacks3,. 
+0000a7b0: 2020 2020 2020 2061 6c6c 7374 6163 6b73         allstacks
+0000a7c0: 342c 0a20 2020 2020 2020 206e 7374 6163  4,.        nstac
+0000a7d0: 6b73 2c0a 2020 2020 290a 0a0a 6465 6620  ks,.    )...def 
+0000a7e0: 726f 7461 7469 6f6e 2862 6967 7374 6163  rotation(bigstac
+0000a7f0: 6b2c 2070 6172 616d 6574 6572 732c 206c  k, parameters, l
+0000a800: 6f63 7329 3a0a 2020 2020 2222 220a 2020  ocs):.    """.  
+0000a810: 2020 7468 6973 2066 756e 6374 696f 6e20    this function 
+0000a820: 7472 616e 7366 6572 7320 7468 6520 4772  transfers the Gr
+0000a830: 6565 6e27 7320 7465 6e73 6f72 2066 726f  een's tensor fro
+0000a840: 6d20 6120 452d 4e2d 5a20 7379 7374 656d  m a E-N-Z system
+0000a850: 2069 6e74 6f20 6120 522d 542d 5a20 6f6e   into a R-T-Z on
+0000a860: 650a 0a20 2020 2050 4152 414d 4554 4552  e..    PARAMETER
+0000a870: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
+0000a880: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2062  ----------.    b
+0000a890: 6967 7374 6163 6b3a 2020 2039 2063 6f6d  igstack:   9 com
+0000a8a0: 706f 6e65 6e74 2047 7265 656e 2773 2074  ponent Green's t
+0000a8b0: 656e 736f 7220 696e 2045 2d4e 2d5a 2073  ensor in E-N-Z s
+0000a8c0: 7973 7465 6d0a 2020 2020 7061 7261 6d65  ystem.    parame
+0000a8d0: 7465 7273 3a20 6469 6374 2063 6f6e 7461  ters: dict conta
+0000a8e0: 696e 696e 6720 616c 6c20 7061 7261 6d65  ining all parame
+0000a8f0: 7465 7273 2073 6176 6564 2069 6e20 4153  ters saved in AS
+0000a900: 4446 2066 696c 650a 2020 2020 6c6f 6373  DF file.    locs
+0000a910: 3a20 2020 2020 2020 6469 6374 2063 6f6e  :       dict con
+0000a920: 7461 696e 696e 6720 7374 6174 696f 6e20  taining station 
+0000a930: 616e 676c 6520 696e 666f 2066 6f72 2063  angle info for c
+0000a940: 6f72 7265 6374 696f 6e20 7075 7270 6f73  orrection purpos
+0000a950: 650a 2020 2020 5245 5455 524e 533a 0a20  e.    RETURNS:. 
+0000a960: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+0000a970: 2d2d 2d2d 2d2d 0a20 2020 2074 636f 7272  ------.    tcorr
+0000a980: 3a20 3920 636f 6d70 6f6e 656e 7420 4772  : 9 component Gr
+0000a990: 6565 6e27 7320 7465 6e73 6f72 2069 6e20  een's tensor in 
+0000a9a0: 522d 542d 5a20 7379 7374 656d 0a20 2020  R-T-Z system.   
+0000a9b0: 2022 2222 0a20 2020 2023 206c 6f61 6420   """.    # load 
+0000a9c0: 7061 7261 6d65 7465 7220 6469 630a 2020  parameter dic.  
+0000a9d0: 2020 7069 203d 206e 702e 7069 0a20 2020    pi = np.pi.   
+0000a9e0: 2061 7a69 203d 2070 6172 616d 6574 6572   azi = parameter
+0000a9f0: 735b 2261 7a69 225d 0a20 2020 2062 617a  s["azi"].    baz
+0000aa00: 203d 2070 6172 616d 6574 6572 735b 2262   = parameters["b
+0000aa10: 617a 225d 0a20 2020 206e 636f 6d70 2c20  az"].    ncomp, 
+0000aa20: 6e70 7473 203d 2062 6967 7374 6163 6b2e  npts = bigstack.
+0000aa30: 7368 6170 650a 2020 2020 6966 206e 636f  shape.    if nco
+0000aa40: 6d70 203c 2039 3a0a 2020 2020 2020 2020  mp < 9:.        
+0000aa50: 6c6f 6767 6572 2e64 6562 7567 2822 6372  logger.debug("cr
+0000aa60: 6170 2064 6964 206e 6f74 2067 6574 2065  ap did not get e
+0000aa70: 6e6f 7567 6820 636f 6d70 6f6e 656e 7473  nough components
+0000aa80: 2229 0a20 2020 2020 2020 2074 636f 7272  ").        tcorr
+0000aa90: 203d 205b 5d0a 2020 2020 2020 2020 7265   = [].        re
+0000aaa0: 7475 726e 2074 636f 7272 0a20 2020 2073  turn tcorr.    s
+0000aab0: 7461 5320 3d20 7061 7261 6d65 7465 7273  taS = parameters
+0000aac0: 5b22 7374 6174 696f 6e5f 736f 7572 6365  ["station_source
+0000aad0: 225d 0a20 2020 2073 7461 5220 3d20 7061  "].    staR = pa
+0000aae0: 7261 6d65 7465 7273 5b22 7374 6174 696f  rameters["statio
+0000aaf0: 6e5f 7265 6365 6976 6572 225d 0a0a 2020  n_receiver"]..  
+0000ab00: 2020 6966 206c 656e 286c 6f63 7329 3a0a    if len(locs):.
+0000ab10: 2020 2020 2020 2020 7374 615f 6c69 7374          sta_list
+0000ab20: 203d 206c 6973 7428 6c6f 6373 5b22 7374   = list(locs["st
+0000ab30: 6174 696f 6e22 5d29 0a20 2020 2020 2020  ation"]).       
+0000ab40: 2061 6e67 6c65 7320 3d20 6c69 7374 286c   angles = list(l
+0000ab50: 6f63 735b 2261 6e67 6c65 225d 290a 2020  ocs["angle"]).  
+0000ab60: 2020 2020 2020 2320 6765 7420 7374 6174        # get stat
+0000ab70: 696f 6e20 696e 666f 2066 726f 6d20 7468  ion info from th
+0000ab80: 6520 6e61 6d65 206f 6620 4153 4446 2066  e name of ASDF f
+0000ab90: 696c 650a 2020 2020 2020 2020 696e 6420  ile.        ind 
+0000aba0: 3d20 7374 615f 6c69 7374 2e69 6e64 6578  = sta_list.index
+0000abb0: 2873 7461 5329 0a20 2020 2020 2020 2061  (staS).        a
+0000abc0: 636f 7272 203d 2061 6e67 6c65 735b 696e  corr = angles[in
+0000abd0: 645d 0a20 2020 2020 2020 2069 6e64 203d  d].        ind =
+0000abe0: 2073 7461 5f6c 6973 742e 696e 6465 7828   sta_list.index(
+0000abf0: 7374 6152 290a 2020 2020 2020 2020 6263  staR).        bc
+0000ac00: 6f72 7220 3d20 616e 676c 6573 5b69 6e64  orr = angles[ind
+0000ac10: 5d0a 0a20 2020 2023 202d 2d2d 616e 676c  ]..    # ---angl
+0000ac20: 6573 2074 6f20 6265 2063 6f72 7265 6374  es to be correct
+0000ac30: 6564 2d2d 2d2d 0a20 2020 2069 6620 6c65  ed----.    if le
+0000ac40: 6e28 6c6f 6373 293a 0a20 2020 2020 2020  n(locs):.       
+0000ac50: 2063 6f73 6120 3d20 6e70 2e63 6f73 2828   cosa = np.cos((
+0000ac60: 617a 6920 2b20 6163 6f72 7229 202a 2070  azi + acorr) * p
+0000ac70: 6920 2f20 3138 3029 0a20 2020 2020 2020  i / 180).       
+0000ac80: 2073 696e 6120 3d20 6e70 2e73 696e 2828   sina = np.sin((
+0000ac90: 617a 6920 2b20 6163 6f72 7229 202a 2070  azi + acorr) * p
+0000aca0: 6920 2f20 3138 3029 0a20 2020 2020 2020  i / 180).       
+0000acb0: 2063 6f73 6220 3d20 6e70 2e63 6f73 2828   cosb = np.cos((
+0000acc0: 6261 7a20 2b20 6263 6f72 7229 202a 2070  baz + bcorr) * p
+0000acd0: 6920 2f20 3138 3029 0a20 2020 2020 2020  i / 180).       
+0000ace0: 2073 696e 6220 3d20 6e70 2e73 696e 2828   sinb = np.sin((
+0000acf0: 6261 7a20 2b20 6263 6f72 7229 202a 2070  baz + bcorr) * p
+0000ad00: 6920 2f20 3138 3029 0a20 2020 2065 6c73  i / 180).    els
+0000ad10: 653a 0a20 2020 2020 2020 2063 6f73 6120  e:.        cosa 
+0000ad20: 3d20 6e70 2e63 6f73 2861 7a69 202a 2070  = np.cos(azi * p
+0000ad30: 6920 2f20 3138 3029 0a20 2020 2020 2020  i / 180).       
+0000ad40: 2073 696e 6120 3d20 6e70 2e73 696e 2861   sina = np.sin(a
+0000ad50: 7a69 202a 2070 6920 2f20 3138 3029 0a20  zi * pi / 180). 
+0000ad60: 2020 2020 2020 2063 6f73 6220 3d20 6e70         cosb = np
+0000ad70: 2e63 6f73 2862 617a 202a 2070 6920 2f20  .cos(baz * pi / 
 0000ad80: 3138 3029 0a20 2020 2020 2020 2073 696e  180).        sin
-0000ad90: 6120 3d20 6e70 2e73 696e 2861 7a69 202a  a = np.sin(azi *
-0000ada0: 2070 6920 2f20 3138 3029 0a20 2020 2020   pi / 180).     
-0000adb0: 2020 2063 6f73 6220 3d20 6e70 2e63 6f73     cosb = np.cos
-0000adc0: 2862 617a 202a 2070 6920 2f20 3138 3029  (baz * pi / 180)
-0000add0: 0a20 2020 2020 2020 2073 696e 6220 3d20  .        sinb = 
-0000ade0: 6e70 2e73 696e 2862 617a 202a 2070 6920  np.sin(baz * pi 
-0000adf0: 2f20 3138 3029 0a0a 2020 2020 2320 7274  / 180)..    # rt
-0000ae00: 7a5f 636f 6d70 6f6e 656e 7473 203d 205b  z_components = [
-0000ae10: 275a 5227 2c27 5a54 272c 275a 5a27 2c27  'ZR','ZT','ZZ','
-0000ae20: 5252 272c 2752 5427 2c27 525a 272c 2754  RR','RT','RZ','T
-0000ae30: 5227 2c27 5454 272c 2754 5a27 5d0a 2020  R','TT','TZ'].  
-0000ae40: 2020 7463 6f72 7220 3d20 6e70 2e7a 6572    tcorr = np.zer
-0000ae50: 6f73 2873 6861 7065 3d28 392c 206e 7074  os(shape=(9, npt
-0000ae60: 7329 2c20 6474 7970 653d 6e70 2e66 6c6f  s), dtype=np.flo
-0000ae70: 6174 3332 290a 2020 2020 7463 6f72 725b  at32).    tcorr[
-0000ae80: 305d 203d 202d 636f 7362 202a 2062 6967  0] = -cosb * big
-0000ae90: 7374 6163 6b5b 375d 202d 2073 696e 6220  stack[7] - sinb 
-0000aea0: 2a20 6269 6773 7461 636b 5b36 5d0a 2020  * bigstack[6].  
-0000aeb0: 2020 7463 6f72 725b 315d 203d 2073 696e    tcorr[1] = sin
-0000aec0: 6220 2a20 6269 6773 7461 636b 5b37 5d20  b * bigstack[7] 
-0000aed0: 2d20 636f 7362 202a 2062 6967 7374 6163  - cosb * bigstac
-0000aee0: 6b5b 365d 0a20 2020 2074 636f 7272 5b32  k[6].    tcorr[2
-0000aef0: 5d20 3d20 6269 6773 7461 636b 5b38 5d0a  ] = bigstack[8].
-0000af00: 2020 2020 7463 6f72 725b 335d 203d 2028      tcorr[3] = (
-0000af10: 0a20 2020 2020 2020 202d 636f 7361 202a  .        -cosa *
-0000af20: 2063 6f73 6220 2a20 6269 6773 7461 636b   cosb * bigstack
-0000af30: 5b34 5d20 2d20 636f 7361 202a 2073 696e  [4] - cosa * sin
-0000af40: 6220 2a20 6269 6773 7461 636b 5b33 5d20  b * bigstack[3] 
-0000af50: 2d20 7369 6e61 202a 2063 6f73 6220 2a20  - sina * cosb * 
-0000af60: 6269 6773 7461 636b 5b31 5d20 2d20 7369  bigstack[1] - si
-0000af70: 6e61 202a 2073 696e 6220 2a20 6269 6773  na * sinb * bigs
-0000af80: 7461 636b 5b30 5d0a 2020 2020 290a 2020  tack[0].    ).  
-0000af90: 2020 7463 6f72 725b 345d 203d 2028 0a20    tcorr[4] = (. 
-0000afa0: 2020 2020 2020 2063 6f73 6120 2a20 7369         cosa * si
-0000afb0: 6e62 202a 2062 6967 7374 6163 6b5b 345d  nb * bigstack[4]
-0000afc0: 202d 2063 6f73 6120 2a20 636f 7362 202a   - cosa * cosb *
-0000afd0: 2062 6967 7374 6163 6b5b 335d 202b 2073   bigstack[3] + s
-0000afe0: 696e 6120 2a20 7369 6e62 202a 2062 6967  ina * sinb * big
-0000aff0: 7374 6163 6b5b 315d 202d 2073 696e 6120  stack[1] - sina 
-0000b000: 2a20 636f 7362 202a 2062 6967 7374 6163  * cosb * bigstac
-0000b010: 6b5b 305d 0a20 2020 2029 0a20 2020 2074  k[0].    ).    t
-0000b020: 636f 7272 5b35 5d20 3d20 636f 7361 202a  corr[5] = cosa *
-0000b030: 2062 6967 7374 6163 6b5b 355d 202b 2073   bigstack[5] + s
-0000b040: 696e 6120 2a20 6269 6773 7461 636b 5b32  ina * bigstack[2
-0000b050: 5d0a 2020 2020 7463 6f72 725b 365d 203d  ].    tcorr[6] =
-0000b060: 2028 0a20 2020 2020 2020 2073 696e 6120   (.        sina 
-0000b070: 2a20 636f 7362 202a 2062 6967 7374 6163  * cosb * bigstac
-0000b080: 6b5b 345d 202b 2073 696e 6120 2a20 7369  k[4] + sina * si
-0000b090: 6e62 202a 2062 6967 7374 6163 6b5b 335d  nb * bigstack[3]
-0000b0a0: 202d 2063 6f73 6120 2a20 636f 7362 202a   - cosa * cosb *
-0000b0b0: 2062 6967 7374 6163 6b5b 315d 202d 2063   bigstack[1] - c
-0000b0c0: 6f73 6120 2a20 7369 6e62 202a 2062 6967  osa * sinb * big
-0000b0d0: 7374 6163 6b5b 305d 0a20 2020 2029 0a20  stack[0].    ). 
-0000b0e0: 2020 2074 636f 7272 5b37 5d20 3d20 280a     tcorr[7] = (.
-0000b0f0: 2020 2020 2020 2020 2d73 696e 6120 2a20          -sina * 
-0000b100: 7369 6e62 202a 2062 6967 7374 6163 6b5b  sinb * bigstack[
-0000b110: 345d 202b 2073 696e 6120 2a20 636f 7362  4] + sina * cosb
-0000b120: 202a 2062 6967 7374 6163 6b5b 335d 202b   * bigstack[3] +
-0000b130: 2063 6f73 6120 2a20 7369 6e62 202a 2062   cosa * sinb * b
-0000b140: 6967 7374 6163 6b5b 315d 202d 2063 6f73  igstack[1] - cos
-0000b150: 6120 2a20 636f 7362 202a 2062 6967 7374  a * cosb * bigst
-0000b160: 6163 6b5b 305d 0a20 2020 2029 0a20 2020  ack[0].    ).   
-0000b170: 2074 636f 7272 5b38 5d20 3d20 2d73 696e   tcorr[8] = -sin
-0000b180: 6120 2a20 6269 6773 7461 636b 5b35 5d20  a * bigstack[5] 
-0000b190: 2b20 636f 7361 202a 2062 6967 7374 6163  + cosa * bigstac
-0000b1a0: 6b5b 325d 0a0a 2020 2020 7265 7475 726e  k[2]..    return
-0000b1b0: 2074 636f 7272 0a0a 0a23 2323 2323 2323   tcorr...#######
-0000b1c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000b1d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000b1e0: 2323 2323 2323 2323 2323 2323 230a 2323  #############.##
-0000b1f0: 2323 2323 2323 2323 2323 2323 2055 5449  ############ UTI
-0000b200: 4c49 5459 2046 554e 4354 494f 4e53 2023  LITY FUNCTIONS #
-0000b210: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000b220: 2323 0a23 2323 2323 2323 2323 2323 2323  ##.#############
-0000b230: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000b240: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000b250: 2323 2323 2323 230a 0a0a 6465 6620 6368  #######...def ch
-0000b260: 6563 6b5f 7361 6d70 6c65 5f67 6170 7328  eck_sample_gaps(
-0000b270: 7374 7265 616d 3a20 6f62 7370 792e 5374  stream: obspy.St
-0000b280: 7265 616d 2c20 7374 6172 7474 696d 653a  ream, starttime:
-0000b290: 206f 6273 7079 2e55 5443 4461 7465 5469   obspy.UTCDateTi
-0000b2a0: 6d65 2c20 656e 6474 696d 653a 206f 6273  me, endtime: obs
-0000b2b0: 7079 2e55 5443 4461 7465 5469 6d65 293a  py.UTCDateTime):
-0000b2c0: 0a20 2020 2022 2222 0a20 2020 2074 6869  .    """.    thi
-0000b2d0: 7320 6675 6e63 7469 6f6e 2063 6865 636b  s function check
-0000b2e0: 7320 7361 6d70 6c69 6e67 2072 6174 6520  s sampling rate 
-0000b2f0: 616e 6420 6669 6e64 2067 6170 7320 6f66  and find gaps of
-0000b300: 2061 6c6c 2074 7261 6365 7320 696e 2073   all traces in s
-0000b310: 7472 6561 6d2e 0a20 2020 2050 4152 414d  tream..    PARAM
-0000b320: 4554 4552 533a 0a20 2020 202d 2d2d 2d2d  ETERS:.    -----
-0000b330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
-0000b340: 2073 7472 6561 6d3a 206f 6273 7079 2073   stream: obspy s
-0000b350: 7472 6561 6d20 6f62 6a65 6374 2e0a 2020  tream object..  
-0000b360: 2020 6461 7465 5f69 6e66 6f3a 2064 6963    date_info: dic
-0000b370: 7420 6f66 2073 7461 7274 696e 6720 616e  t of starting an
-0000b380: 6420 656e 6469 6e67 2074 696d 6520 6f66  d ending time of
-0000b390: 2074 6865 2073 7472 6561 6d0a 0a20 2020   the stream..   
-0000b3a0: 2052 4554 5552 454e 533a 0a20 2020 202d   RETURENS:.    -
-0000b3b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000b3c0: 0a20 2020 2073 7472 6561 6d3a 204c 6973  .    stream: Lis
-0000b3d0: 7420 6f66 2067 6f6f 6420 7472 6163 6573  t of good traces
-0000b3e0: 2069 6e20 7468 6520 7374 7265 616d 0a20   in the stream. 
-0000b3f0: 2020 2022 2222 0a20 2020 2023 2072 656d     """.    # rem
-0000b400: 6f76 6520 656d 7074 792f 6269 6720 7472  ove empty/big tr
-0000b410: 6163 6573 0a20 2020 2069 6620 6c65 6e28  aces.    if len(
-0000b420: 7374 7265 616d 2920 3d3d 2030 206f 7220  stream) == 0 or 
-0000b430: 6c65 6e28 7374 7265 616d 2920 3e20 3130  len(stream) > 10
-0000b440: 303a 0a20 2020 2020 2020 2073 7472 6561  0:.        strea
-0000b450: 6d20 3d20 5b5d 0a20 2020 2020 2020 2072  m = [].        r
-0000b460: 6574 7572 6e20 7374 7265 616d 0a0a 2020  eturn stream..  
-0000b470: 2020 2320 7265 6d6f 7665 2074 7261 6365    # remove trace
-0000b480: 7320 7769 7468 2062 6967 2067 6170 730a  s with big gaps.
-0000b490: 2020 2020 6966 2070 6f72 7469 6f6e 5f67      if portion_g
-0000b4a0: 6170 7328 7374 7265 616d 2c20 7374 6172  aps(stream, star
-0000b4b0: 7474 696d 652c 2065 6e64 7469 6d65 2920  ttime, endtime) 
-0000b4c0: 3e20 302e 333a 0a20 2020 2020 2020 2073  > 0.3:.        s
-0000b4d0: 7472 6561 6d20 3d20 5b5d 0a20 2020 2020  tream = [].     
-0000b4e0: 2020 2072 6574 7572 6e20 7374 7265 616d     return stream
-0000b4f0: 0a0a 2020 2020 6672 6571 7320 3d20 5b5d  ..    freqs = []
-0000b500: 0a20 2020 2066 6f72 2074 7220 696e 2073  .    for tr in s
-0000b510: 7472 6561 6d3a 0a20 2020 2020 2020 2066  tream:.        f
-0000b520: 7265 7173 2e61 7070 656e 6428 696e 7428  reqs.append(int(
-0000b530: 7472 2e73 7461 7473 2e73 616d 706c 696e  tr.stats.samplin
-0000b540: 675f 7261 7465 2929 0a20 2020 2066 7265  g_rate)).    fre
-0000b550: 7120 3d20 6d61 7828 6672 6571 7329 0a20  q = max(freqs). 
-0000b560: 2020 2066 6f72 2074 7220 696e 2073 7472     for tr in str
-0000b570: 6561 6d3a 0a20 2020 2020 2020 2069 6620  eam:.        if 
-0000b580: 696e 7428 7472 2e73 7461 7473 2e73 616d  int(tr.stats.sam
-0000b590: 706c 696e 675f 7261 7465 2920 213d 2066  pling_rate) != f
-0000b5a0: 7265 713a 0a20 2020 2020 2020 2020 2020  req:.           
-0000b5b0: 2073 7472 6561 6d2e 7265 6d6f 7665 2874   stream.remove(t
-0000b5c0: 7229 0a20 2020 2020 2020 2069 6620 7472  r).        if tr
-0000b5d0: 2e73 7461 7473 2e6e 7074 7320 3c20 3130  .stats.npts < 10
-0000b5e0: 3a0a 2020 2020 2020 2020 2020 2020 7374  :.            st
-0000b5f0: 7265 616d 2e72 656d 6f76 6528 7472 290a  ream.remove(tr).
-0000b600: 0a20 2020 2072 6574 7572 6e20 7374 7265  .    return stre
-0000b610: 616d 0a0a 0a64 6566 2070 6f72 7469 6f6e  am...def portion
-0000b620: 5f67 6170 7328 7374 7265 616d 2c20 7374  _gaps(stream, st
-0000b630: 6172 7474 696d 653a 206f 6273 7079 2e55  arttime: obspy.U
-0000b640: 5443 4461 7465 5469 6d65 2c20 656e 6474  TCDateTime, endt
-0000b650: 696d 653a 206f 6273 7079 2e55 5443 4461  ime: obspy.UTCDa
-0000b660: 7465 5469 6d65 293a 0a20 2020 2022 2222  teTime):.    """
-0000b670: 0a20 2020 2074 6869 7320 6675 6e63 7469  .    this functi
-0000b680: 6f6e 2074 7261 636b 7320 7468 6520 6761  on tracks the ga
-0000b690: 7073 2028 6e70 7473 2920 6672 6f6d 2074  ps (npts) from t
-0000b6a0: 6865 2061 6363 756d 756c 6174 6564 2064  he accumulated d
-0000b6b0: 6966 6665 7265 6e63 6520 6265 7477 6565  ifference betwee
-0000b6c0: 6e20 7374 6172 7474 696d 6520 616e 6420  n starttime and 
-0000b6d0: 656e 6474 696d 650a 2020 2020 6f66 2065  endtime.    of e
-0000b6e0: 6163 6820 7374 7265 616d 2074 7261 6365  ach stream trace
-0000b6f0: 2e20 6974 2072 656d 6f76 6573 2074 7261  . it removes tra
-0000b700: 6365 2077 6974 6820 6761 7020 6c65 6e67  ce with gap leng
-0000b710: 7468 203e 2033 3025 206f 6620 7472 6163  th > 30% of trac
-0000b720: 6520 7369 7a65 2e0a 2020 2020 5041 5241  e size..    PARA
-0000b730: 4d45 5445 5253 3a0a 2020 2020 2d2d 2d2d  METERS:.    ----
-0000b740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-0000b750: 2020 2020 7374 7265 616d 3a20 6f62 7370      stream: obsp
-0000b760: 7920 7374 7265 616d 206f 626a 6563 740a  y stream object.
-0000b770: 2020 2020 6461 7465 5f69 6e66 6f3a 2064      date_info: d
-0000b780: 6963 7420 6f66 2073 7461 7274 696e 6720  ict of starting 
-0000b790: 616e 6420 656e 6469 6e67 2074 696d 6520  and ending time 
-0000b7a0: 6f66 2074 6865 2073 7472 6561 6d0a 0a20  of the stream.. 
-0000b7b0: 2020 2052 4554 5552 4e53 3a0a 2020 2020     RETURNS:.    
-0000b7c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000b7d0: 2d0a 2020 2020 7067 6170 733a 2070 726f  -.    pgaps: pro
-0000b7e0: 706f 7274 696f 6e20 6f66 2067 6170 732f  portion of gaps/
-0000b7f0: 616c 6c5f 7074 7320 696e 2073 7472 6561  all_pts in strea
-0000b800: 6d0a 2020 2020 2222 220a 2020 2020 2320  m.    """.    # 
-0000b810: 6964 6561 6c20 6475 7261 7469 6f6e 206f  ideal duration o
-0000b820: 6620 6461 7461 0a20 2020 206e 7074 7320  f data.    npts 
-0000b830: 3d20 2865 6e64 7469 6d65 202d 2073 7461  = (endtime - sta
-0000b840: 7274 7469 6d65 2920 2a20 7374 7265 616d  rttime) * stream
-0000b850: 5b30 5d2e 7374 6174 732e 7361 6d70 6c69  [0].stats.sampli
-0000b860: 6e67 5f72 6174 650a 0a20 2020 2070 6761  ng_rate..    pga
-0000b870: 7073 203d 2030 0a20 2020 2023 206c 6f6f  ps = 0.    # loo
-0000b880: 7020 7468 726f 7567 6820 616c 6c20 7472  p through all tr
-0000b890: 6163 6520 746f 2061 6363 756d 756c 6174  ace to accumulat
-0000b8a0: 6520 6761 7073 0a20 2020 2066 6f72 2069  e gaps.    for i
-0000b8b0: 6920 696e 2072 616e 6765 286c 656e 2873  i in range(len(s
-0000b8c0: 7472 6561 6d29 202d 2031 293a 0a20 2020  tream) - 1):.   
-0000b8d0: 2020 2020 2070 6761 7073 202b 3d20 2873       pgaps += (s
-0000b8e0: 7472 6561 6d5b 6969 202b 2031 5d2e 7374  tream[ii + 1].st
-0000b8f0: 6174 732e 7374 6172 7474 696d 6520 2d20  ats.starttime - 
-0000b900: 7374 7265 616d 5b69 695d 2e73 7461 7473  stream[ii].stats
-0000b910: 2e65 6e64 7469 6d65 2920 2a20 7374 7265  .endtime) * stre
-0000b920: 616d 5b69 695d 2e73 7461 7473 2e73 616d  am[ii].stats.sam
-0000b930: 706c 696e 675f 7261 7465 0a20 2020 2069  pling_rate.    i
-0000b940: 6620 6e70 7473 2021 3d20 303a 0a20 2020  f npts != 0:.   
-0000b950: 2020 2020 2070 6761 7073 203d 2070 6761       pgaps = pga
-0000b960: 7073 202f 206e 7074 730a 2020 2020 6966  ps / npts.    if
-0000b970: 206e 7074 7320 3d3d 2030 3a0a 2020 2020   npts == 0:.    
-0000b980: 2020 2020 7067 6170 7320 3d20 310a 2020      pgaps = 1.  
-0000b990: 2020 7265 7475 726e 2070 6761 7073 0a0a    return pgaps..
-0000b9a0: 0a40 6a69 7428 2266 6c6f 6174 3332 5b3a  .@jit("float32[:
-0000b9b0: 5d28 666c 6f61 7433 325b 3a5d 2c66 6c6f  ](float32[:],flo
-0000b9c0: 6174 3332 2922 290a 6465 6620 7365 676d  at32)").def segm
-0000b9d0: 656e 745f 696e 7465 7270 6f6c 6174 6528  ent_interpolate(
-0000b9e0: 7369 6731 2c20 6e66 7269 6329 3a0a 2020  sig1, nfric):.  
-0000b9f0: 2020 2222 220a 2020 2020 7468 6973 2066    """.    this f
-0000ba00: 756e 6374 696f 6e20 696e 7465 7270 6f6c  unction interpol
-0000ba10: 6174 6573 2074 6865 2064 6174 6120 746f  ates the data to
-0000ba20: 2065 6e73 7572 6520 616c 6c20 706f 696e   ensure all poin
-0000ba30: 7473 206c 6f63 6174 6564 206f 6e20 696e  ts located on in
-0000ba40: 7465 7267 6572 2074 696d 6573 206f 6620  terger times of 
-0000ba50: 7468 650a 2020 2020 7361 6d70 6c69 6e67  the.    sampling
-0000ba60: 2072 6174 6520 2865 2e67 2e2c 2073 7461   rate (e.g., sta
-0000ba70: 7274 7469 6d65 203d 2030 303a 3030 3a30  rttime = 00:00:0
-0000ba80: 302e 3031 352c 2064 656c 7461 203d 2030  0.015, delta = 0
-0000ba90: 2e30 352e 290a 2020 2020 5041 5241 4d45  .05.).    PARAME
-0000baa0: 5445 5253 3a0a 2020 2020 2d2d 2d2d 2d2d  TERS:.    ------
-0000bab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000bac0: 0a20 2020 2073 6967 313a 2020 7365 6973  .    sig1:  seis
-0000bad0: 6d69 6320 7265 636f 7264 696e 6773 2069  mic recordings i
-0000bae0: 6e20 6120 3144 2061 7272 6179 0a20 2020  n a 1D array.   
-0000baf0: 206e 6672 6963 3a20 7468 6520 616d 6f75   nfric: the amou
-0000bb00: 6e74 206f 6620 7469 6d65 2064 6966 6665  nt of time diffe
-0000bb10: 7265 6e63 6520 6265 7477 6565 6e20 7468  rence between th
-0000bb20: 6520 706f 696e 7420 616e 6420 7468 6520  e point and the 
-0000bb30: 6164 6a61 6365 6e74 2061 7373 756d 6564  adjacent assumed
-0000bb40: 2073 616d 706c 6573 0a20 2020 2052 4554   samples.    RET
-0000bb50: 5552 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d  URNS:.    ------
-0000bb60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000bb70: 0a20 2020 2073 6967 323a 2020 696e 7465  .    sig2:  inte
-0000bb80: 7270 6f6c 6174 6564 2073 6569 736d 6963  rpolated seismic
-0000bb90: 2072 6563 6f72 6469 6e67 7320 6f6e 2074   recordings on t
-0000bba0: 6865 2073 616d 706c 696e 6720 706f 696e  he sampling poin
-0000bbb0: 7473 0a20 2020 2022 2222 0a20 2020 206e  ts.    """.    n
-0000bbc0: 7074 7320 3d20 6c65 6e28 7369 6731 290a  pts = len(sig1).
-0000bbd0: 2020 2020 7369 6732 203d 206e 702e 7a65      sig2 = np.ze
-0000bbe0: 726f 7328 6e70 7473 2c20 6474 7970 653d  ros(npts, dtype=
-0000bbf0: 6e70 2e66 6c6f 6174 3332 290a 0a20 2020  np.float32)..   
-0000bc00: 2023 202d 2d2d 2d69 6e73 7465 6164 206f   # ----instead o
-0000bc10: 6620 7368 6966 7469 6e67 2c20 646f 2061  f shifting, do a
-0000bc20: 2069 6e74 6572 706f 6c61 7469 6f6e 2d2d   interpolation--
-0000bc30: 2d2d 2d2d 0a20 2020 2066 6f72 2069 6920  ----.    for ii 
-0000bc40: 696e 2072 616e 6765 286e 7074 7329 3a0a  in range(npts):.
-0000bc50: 2020 2020 2020 2020 2320 2d2d 2d2d 6465          # ----de
-0000bc60: 616c 2077 6974 6820 6564 6765 732d 2d2d  al with edges---
-0000bc70: 2d2d 0a20 2020 2020 2020 2069 6620 6969  --.        if ii
-0000bc80: 203d 3d20 3020 6f72 2069 6920 3d3d 206e   == 0 or ii == n
-0000bc90: 7074 7320 2d20 313a 0a20 2020 2020 2020  pts - 1:.       
-0000bca0: 2020 2020 2073 6967 325b 6969 5d20 3d20       sig2[ii] = 
-0000bcb0: 7369 6731 5b69 695d 0a20 2020 2020 2020  sig1[ii].       
-0000bcc0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000bcd0: 2020 2023 202d 2d2d 2d2d 2d69 6e74 6572     # ------inter
-0000bce0: 706f 6c61 7465 2075 7369 6e67 2061 2068  polate using a h
-0000bcf0: 6174 2066 756e 6374 696f 6e2d 2d2d 2d2d  at function-----
-0000bd00: 2d0a 2020 2020 2020 2020 2020 2020 7369  -.            si
-0000bd10: 6732 5b69 695d 203d 2028 3120 2d20 6e66  g2[ii] = (1 - nf
-0000bd20: 7269 6329 202a 2073 6967 315b 6969 202b  ric) * sig1[ii +
-0000bd30: 2031 5d20 2b20 6e66 7269 6320 2a20 7369   1] + nfric * si
-0000bd40: 6731 5b69 695d 0a0a 2020 2020 7265 7475  g1[ii]..    retu
-0000bd50: 726e 2073 6967 320a 0a0a 6465 6620 7265  rn sig2...def re
-0000bd60: 7370 5f73 7065 6374 7275 6d28 736f 7572  sp_spectrum(sour
-0000bd70: 6365 2c20 7265 7370 5f66 696c 652c 2064  ce, resp_file, d
-0000bd80: 6f77 6e73 616d 705f 6672 6571 2c20 7072  ownsamp_freq, pr
-0000bd90: 655f 6669 6c74 3d4e 6f6e 6529 3a0a 2020  e_filt=None):.  
-0000bda0: 2020 2222 220a 2020 2020 7468 6973 2066    """.    this f
-0000bdb0: 756e 6374 696f 6e20 7265 6d6f 7665 7320  unction removes 
-0000bdc0: 7468 6520 696e 7374 7275 6d65 6e74 2072  the instrument r
-0000bdd0: 6573 706f 6e73 6520 7573 696e 6720 7265  esponse using re
-0000bde0: 7370 6f6e 7365 2073 7065 6374 7275 6d20  sponse spectrum 
-0000bdf0: 6672 6f6d 2065 7661 6c72 6573 702e 0a20  from evalresp.. 
-0000be00: 2020 2074 6865 2072 6573 706f 6e73 6520     the response 
-0000be10: 7370 6563 7472 756d 2069 7320 6576 616c  spectrum is eval
-0000be20: 7561 7465 6420 6261 7365 6420 6f6e 2052  uated based on R
-0000be30: 4553 502f 505a 2066 696c 6573 2062 6566  ESP/PZ files bef
-0000be40: 6f72 6520 696e 7665 7274 6564 2075 7369  ore inverted usi
-0000be50: 6e67 2074 6865 206f 6273 7079 0a20 2020  ng the obspy.   
-0000be60: 2066 756e 6374 696f 6e20 6f66 2069 6e76   function of inv
-0000be70: 6572 745f 7370 6563 7472 756d 2e20 6120  ert_spectrum. a 
-0000be80: 6d6f 6475 6c65 206f 6620 6372 6561 7465  module of create
-0000be90: 5f72 6573 702e 7079 2069 7320 7072 6f76  _resp.py is prov
-0000bea0: 6964 6564 2069 6e20 6469 7265 6374 6f72  ided in director
-0000beb0: 7920 6f66 2027 6164 6469 7469 6f6e 616c  y of 'additional
-0000bec0: 5f6d 6f64 756c 6573 270a 2020 2020 746f  _modules'.    to
-0000bed0: 2063 7265 6174 6520 7468 6520 7265 7370   create the resp
-0000bee0: 6f6e 7365 2073 7065 6374 7275 6d0a 2020  onse spectrum.  
-0000bef0: 2020 5041 5241 4d45 5445 5253 3a0a 2020    PARAMETERS:.  
-0000bf00: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
-0000bf10: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2073 6f75  --------.    sou
-0000bf20: 7263 653a 206f 6273 7079 2073 7472 6561  rce: obspy strea
-0000bf30: 6d20 6f62 6a65 6374 206f 6620 7461 7267  m object of targ
-0000bf40: 6574 6564 206e 6f69 7365 2064 6174 610a  eted noise data.
-0000bf50: 2020 2020 7265 7370 5f66 696c 653a 206e      resp_file: n
-0000bf60: 756d 7079 2064 6174 6120 6669 6c65 206f  umpy data file o
-0000bf70: 6620 7265 7370 6f6e 7365 2073 7065 6374  f response spect
-0000bf80: 7275 6d0a 2020 2020 646f 776e 7361 6d70  rum.    downsamp
-0000bf90: 5f66 7265 713a 2073 616d 706c 696e 6720  _freq: sampling 
-0000bfa0: 7261 7465 206f 6620 7468 6520 736f 7572  rate of the sour
-0000bfb0: 6365 2064 6174 610a 2020 2020 7072 655f  ce data.    pre_
-0000bfc0: 6669 6c74 3a20 7072 652d 6465 6669 6e65  filt: pre-define
-0000bfd0: 6420 6669 6c74 6572 2070 6172 616d 6574  d filter paramet
-0000bfe0: 6572 730a 2020 2020 5245 5455 524e 533a  ers.    RETURNS:
-0000bff0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
-0000c000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
-0000c010: 736f 7572 6365 3a20 6f62 7370 7920 7374  source: obspy st
-0000c020: 7265 616d 206f 626a 6563 7420 6f66 206e  ream object of n
-0000c030: 6f69 7365 2064 6174 6120 7769 7468 2069  oise data with i
-0000c040: 6e73 7472 756d 656e 7420 7265 7370 6f6e  nstrument respon
-0000c050: 7365 2072 656d 6f76 6564 0a20 2020 2022  se removed.    "
-0000c060: 2222 0a20 2020 2023 202d 2d2d 2d2d 2d2d  "".    # -------
-0000c070: 2d72 6573 705f 6669 6c65 2069 7320 7468  -resp_file is th
-0000c080: 6520 696e 7665 7274 6564 2073 7065 6374  e inverted spect
-0000c090: 7275 6d20 7265 7370 6f6e 7365 2d2d 2d2d  rum response----
-0000c0a0: 2d2d 2d2d 2d0a 2020 2020 7265 7370 7a20  -----.    respz 
-0000c0b0: 3d20 6e70 2e6c 6f61 6428 7265 7370 5f66  = np.load(resp_f
-0000c0c0: 696c 6529 0a20 2020 206e 7265 7370 7a20  ile).    nrespz 
-0000c0d0: 3d20 7265 7370 7a5b 315d 5b3a 5d0a 2020  = respz[1][:].  
-0000c0e0: 2020 7370 6563 5f66 7265 7120 3d20 6d61    spec_freq = ma
-0000c0f0: 7828 7265 7370 7a5b 305d 290a 0a20 2020  x(respz[0])..   
-0000c100: 2023 202d 2d2d 2d2d 2d2d 6f6e 2063 7572   # -------on cur
-0000c110: 7265 6e74 2074 7261 6365 2d2d 2d2d 2d2d  rent trace------
-0000c120: 2d2d 2d2d 0a20 2020 206e 6666 7420 3d20  ----.    nfft = 
-0000c130: 5f6e 7074 7332 6e66 6674 2873 6f75 7263  _npts2nfft(sourc
-0000c140: 655b 305d 2e73 7461 7473 2e6e 7074 7329  e[0].stats.npts)
-0000c150: 0a20 2020 2073 7073 203d 2069 6e74 2873  .    sps = int(s
-0000c160: 6f75 7263 655b 305d 2e73 7461 7473 2e73  ource[0].stats.s
-0000c170: 616d 706c 696e 675f 7261 7465 290a 0a20  ampling_rate).. 
-0000c180: 2020 2023 202d 2d2d 2d2d 2d2d 2d2d 646f     # ---------do
-0000c190: 2074 6865 2069 6e74 6572 706f 6c61 7469   the interpolati
-0000c1a0: 6f6e 2069 6620 6e65 6564 6564 2d2d 2d2d  on if needed----
-0000c1b0: 2d2d 2d2d 0a20 2020 2069 6620 7370 6563  ----.    if spec
-0000c1c0: 5f66 7265 7120 3c20 302e 3520 2a20 7370  _freq < 0.5 * sp
-0000c1d0: 733a 0a20 2020 2020 2020 2072 6169 7365  s:.        raise
-0000c1e0: 2056 616c 7565 4572 726f 7228 2273 7065   ValueError("spe
-0000c1f0: 6374 7275 6d20 6669 6c65 2068 6173 2070  ctrum file has p
-0000c200: 6561 6b20 6672 6571 2073 6d61 6c6c 6572  eak freq smaller
-0000c210: 2074 6861 6e20 7468 6520 6461 7461 2c20   than the data, 
-0000c220: 6162 6f72 7421 2229 0a20 2020 2065 6c73  abort!").    els
-0000c230: 653a 0a20 2020 2020 2020 2069 6e64 7820  e:.        indx 
-0000c240: 3d20 6e70 2e77 6865 7265 2872 6573 707a  = np.where(respz
-0000c250: 5b30 5d20 3c3d 2030 2e35 202a 2073 7073  [0] <= 0.5 * sps
-0000c260: 290a 2020 2020 2020 2020 6e66 7265 7120  ).        nfreq 
-0000c270: 3d20 6e70 2e6c 696e 7370 6163 6528 302c  = np.linspace(0,
-0000c280: 2030 2e35 202a 2073 7073 2c20 6e66 6674   0.5 * sps, nfft
-0000c290: 202f 2f20 3220 2b20 3129 0a20 2020 2020   // 2 + 1).     
-0000c2a0: 2020 206e 7265 7370 7a20 3d20 6e70 2e69     nrespz = np.i
-0000c2b0: 6e74 6572 7028 6e66 7265 712c 206e 702e  nterp(nfreq, np.
-0000c2c0: 7265 616c 2872 6573 707a 5b30 5d5b 696e  real(respz[0][in
-0000c2d0: 6478 5d29 2c20 7265 7370 7a5b 315d 5b69  dx]), respz[1][i
-0000c2e0: 6e64 785d 290a 0a20 2020 2023 202d 2d2d  ndx])..    # ---
-0000c2f0: 2d64 6f20 696e 7465 7270 6f6c 6174 696f  -do interpolatio
-0000c300: 6e20 6966 206e 6563 6573 7361 7279 2d2d  n if necessary--
-0000c310: 2d2d 2d0a 2020 2020 736f 7572 6365 5f73  ---.    source_s
-0000c320: 7065 6374 203d 206e 702e 6666 742e 7266  pect = np.fft.rf
-0000c330: 6674 2873 6f75 7263 655b 305d 2e64 6174  ft(source[0].dat
-0000c340: 612c 206e 3d6e 6666 7429 0a0a 2020 2020  a, n=nfft)..    
-0000c350: 2320 2d2d 2d2d 2d6e 7265 7370 7a20 6973  # -----nrespz is
-0000c360: 2069 6e76 6572 7365 6420 2877 6174 6572   inversed (water
-0000c370: 2d6c 6576 656c 6564 2920 7370 6563 7472  -leveled) spectr
-0000c380: 756d 2d2d 2d2d 2d0a 2020 2020 736f 7572  um-----.    sour
-0000c390: 6365 5f73 7065 6374 202a 3d20 6e72 6573  ce_spect *= nres
-0000c3a0: 707a 0a20 2020 2073 6f75 7263 655b 305d  pz.    source[0]
-0000c3b0: 2e64 6174 6120 3d20 6e70 2e66 6674 2e69  .data = np.fft.i
-0000c3c0: 7266 6674 2873 6f75 7263 655f 7370 6563  rfft(source_spec
-0000c3d0: 7429 5b30 203a 2073 6f75 7263 655b 305d  t)[0 : source[0]
-0000c3e0: 2e73 7461 7473 2e6e 7074 735d 0a0a 2020  .stats.npts]..  
-0000c3f0: 2020 6966 2070 7265 5f66 696c 7420 6973    if pre_filt is
-0000c400: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000c410: 2020 2073 6f75 7263 655b 305d 2e64 6174     source[0].dat
-0000c420: 6120 3d20 6e70 2e66 6c6f 6174 3332 280a  a = np.float32(.
-0000c430: 2020 2020 2020 2020 2020 2020 6261 6e64              band
-0000c440: 7061 7373 280a 2020 2020 2020 2020 2020  pass(.          
-0000c450: 2020 2020 2020 736f 7572 6365 5b30 5d2e        source[0].
-0000c460: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
-0000c470: 2020 2020 2020 7072 655f 6669 6c74 5b30        pre_filt[0
-0000c480: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-0000c490: 2020 2070 7265 5f66 696c 745b 2d31 5d2c     pre_filt[-1],
-0000c4a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c4b0: 2064 663d 7370 732c 0a20 2020 2020 2020   df=sps,.       
-0000c4c0: 2020 2020 2020 2020 2063 6f72 6e65 7273           corners
-0000c4d0: 3d34 2c0a 2020 2020 2020 2020 2020 2020  =4,.            
-0000c4e0: 2020 2020 7a65 726f 7068 6173 653d 5472      zerophase=Tr
-0000c4f0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-0000c500: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
-0000c510: 2072 6574 7572 6e20 736f 7572 6365 0a0a   return source..
-0000c520: 0a64 6566 206d 6164 2861 7272 293a 0a20  .def mad(arr):. 
-0000c530: 2020 2022 2222 0a20 2020 204d 6564 6961     """.    Media
-0000c540: 6e20 4162 736f 6c75 7465 2044 6576 6961  n Absolute Devia
-0000c550: 7469 6f6e 3a20 4d41 4420 3d20 6d65 6469  tion: MAD = medi
-0000c560: 616e 287c 5869 2d20 6d65 6469 616e 2858  an(|Xi- median(X
-0000c570: 297c 290a 2020 2020 5041 5241 4d45 5445  )|).    PARAMETE
-0000c580: 5253 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  RS:.    --------
-0000c590: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
-0000c5a0: 6172 723a 206e 756d 7079 2e6e 6461 7272  arr: numpy.ndarr
-0000c5b0: 6179 2c20 7365 6973 6d69 6320 7472 6163  ay, seismic trac
-0000c5c0: 6520 6461 7461 2061 7272 6179 0a20 2020  e data array.   
-0000c5d0: 2052 4554 5552 4e53 3a0a 2020 2020 6461   RETURNS:.    da
-0000c5e0: 7461 3a20 4d65 6469 616e 2041 6273 6f6c  ta: Median Absol
-0000c5f0: 7574 6520 4465 7669 6174 696f 6e20 6f66  ute Deviation of
-0000c600: 2064 6174 610a 2020 2020 2222 220a 2020   data.    """.  
-0000c610: 2020 6966 206e 6f74 206e 702e 6d61 2e69    if not np.ma.i
-0000c620: 735f 6d61 736b 6564 2861 7272 293a 0a20  s_masked(arr):. 
-0000c630: 2020 2020 2020 206d 6564 203d 206e 702e         med = np.
-0000c640: 6d65 6469 616e 2861 7272 290a 2020 2020  median(arr).    
-0000c650: 2020 2020 6461 7461 203d 206e 702e 6d65      data = np.me
-0000c660: 6469 616e 286e 702e 6162 7328 6172 7220  dian(np.abs(arr 
-0000c670: 2d20 6d65 6429 290a 2020 2020 656c 7365  - med)).    else
-0000c680: 3a0a 2020 2020 2020 2020 6d65 6420 3d20  :.        med = 
-0000c690: 6e70 2e6d 612e 6d65 6469 616e 2861 7272  np.ma.median(arr
-0000c6a0: 290a 2020 2020 2020 2020 6461 7461 203d  ).        data =
-0000c6b0: 206e 702e 6d61 2e6d 6564 6961 6e28 6e70   np.ma.median(np
-0000c6c0: 2e6d 612e 6162 7328 6172 7220 2d20 6d65  .ma.abs(arr - me
-0000c6d0: 6429 290a 2020 2020 7265 7475 726e 2064  d)).    return d
-0000c6e0: 6174 610a 0a0a 6465 6620 6465 7472 656e  ata...def detren
-0000c6f0: 6428 6461 7461 293a 0a20 2020 2022 2222  d(data):.    """
-0000c700: 0a20 2020 2074 6869 7320 6675 6e63 7469  .    this functi
-0000c710: 6f6e 2072 656d 6f76 6573 2074 6865 2073  on removes the s
-0000c720: 6967 6e61 6c20 7472 656e 6420 6261 7365  ignal trend base
-0000c730: 6420 6f6e 2051 5220 6465 636f 6d70 6f73  d on QR decompos
-0000c740: 696f 6e0a 2020 2020 4e4f 5445 3a20 5152  ion.    NOTE: QR
-0000c750: 2069 7320 6120 6c6f 7420 6661 7374 6572   is a lot faster
-0000c760: 2074 6861 6e20 7468 6520 6c65 6173 7420   than the least 
-0000c770: 7371 7561 7265 2069 6e76 6572 7369 6f6e  square inversion
-0000c780: 2075 7365 6420 6279 0a20 2020 2073 6369   used by.    sci
-0000c790: 7079 2028 616c 736f 2069 6e20 6f62 7370  py (also in obsp
-0000c7a0: 7929 2e0a 2020 2020 5041 5241 4d45 5445  y)..    PARAMETE
-0000c7b0: 5253 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  RS:.    --------
-0000c7c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-0000c7d0: 2020 6461 7461 3a20 696e 7075 7420 6461    data: input da
-0000c7e0: 7461 206d 6174 7269 780a 2020 2020 5245  ta matrix.    RE
-0000c7f0: 5455 524e 533a 0a20 2020 202d 2d2d 2d2d  TURNS:.    -----
-0000c800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000c810: 0a20 2020 2064 6174 613a 2064 6174 6120  .    data: data 
-0000c820: 6d61 7472 6978 2077 6974 6820 7472 656e  matrix with tren
-0000c830: 6420 7265 6d6f 7665 640a 2020 2020 2222  d removed.    ""
-0000c840: 220a 2020 2020 2320 6e64 6174 6120 3d20  ".    # ndata = 
-0000c850: 6e70 2e7a 6572 6f73 2873 6861 7065 3d64  np.zeros(shape=d
-0000c860: 6174 612e 7368 6170 652c 6474 7970 653d  ata.shape,dtype=
-0000c870: 6461 7461 2e64 7479 7065 290a 2020 2020  data.dtype).    
-0000c880: 6966 2064 6174 612e 6e64 696d 203d 3d20  if data.ndim == 
-0000c890: 313a 0a20 2020 2020 2020 206e 7074 7320  1:.        npts 
-0000c8a0: 3d20 6461 7461 2e73 6861 7065 5b30 5d0a  = data.shape[0].
-0000c8b0: 2020 2020 2020 2020 5820 3d20 6e70 2e6f          X = np.o
-0000c8c0: 6e65 7328 286e 7074 732c 2032 2929 0a20  nes((npts, 2)). 
-0000c8d0: 2020 2020 2020 2058 5b3a 2c20 305d 203d         X[:, 0] =
-0000c8e0: 206e 702e 6172 616e 6765 2830 2c20 6e70   np.arange(0, np
-0000c8f0: 7473 2920 2f20 6e70 7473 0a20 2020 2020  ts) / npts.     
-0000c900: 2020 2051 2c20 5220 3d20 6e70 2e6c 696e     Q, R = np.lin
-0000c910: 616c 672e 7172 2858 290a 2020 2020 2020  alg.qr(X).      
-0000c920: 2020 7271 203d 206e 702e 646f 7428 6e70    rq = np.dot(np
-0000c930: 2e6c 696e 616c 672e 696e 7628 5229 2c20  .linalg.inv(R), 
-0000c940: 512e 7472 616e 7370 6f73 6528 2929 0a20  Q.transpose()). 
-0000c950: 2020 2020 2020 2063 6f65 6666 203d 206e         coeff = n
-0000c960: 702e 646f 7428 7271 2c20 6461 7461 290a  p.dot(rq, data).
-0000c970: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-0000c980: 6174 6120 2d20 6e70 2e64 6f74 2858 2c20  ata - np.dot(X, 
-0000c990: 636f 6566 6629 0a20 2020 2065 6c69 6620  coeff).    elif 
-0000c9a0: 6461 7461 2e6e 6469 6d20 3d3d 2032 3a0a  data.ndim == 2:.
-0000c9b0: 2020 2020 2020 2020 6e70 7473 203d 2064          npts = d
-0000c9c0: 6174 612e 7368 6170 655b 315d 0a20 2020  ata.shape[1].   
-0000c9d0: 2020 2020 2058 203d 206e 702e 6f6e 6573       X = np.ones
-0000c9e0: 2828 6e70 7473 2c20 3229 290a 2020 2020  ((npts, 2)).    
-0000c9f0: 2020 2020 585b 3a2c 2030 5d20 3d20 6e70      X[:, 0] = np
-0000ca00: 2e61 7261 6e67 6528 302c 206e 7074 7329  .arange(0, npts)
-0000ca10: 202f 206e 7074 730a 2020 2020 2020 2020   / npts.        
-0000ca20: 512c 2052 203d 206e 702e 6c69 6e61 6c67  Q, R = np.linalg
-0000ca30: 2e71 7228 5829 0a20 2020 2020 2020 2072  .qr(X).        r
-0000ca40: 7120 3d20 6e70 2e64 6f74 286e 702e 6c69  q = np.dot(np.li
-0000ca50: 6e61 6c67 2e69 6e76 2852 292c 2051 2e74  nalg.inv(R), Q.t
-0000ca60: 7261 6e73 706f 7365 2829 290a 2020 2020  ranspose()).    
-0000ca70: 2020 2020 666f 7220 6969 2069 6e20 7261      for ii in ra
-0000ca80: 6e67 6528 6461 7461 2e73 6861 7065 5b30  nge(data.shape[0
-0000ca90: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
-0000caa0: 636f 6566 6620 3d20 6e70 2e64 6f74 2872  coeff = np.dot(r
-0000cab0: 712c 2064 6174 615b 6969 5d29 0a20 2020  q, data[ii]).   
-0000cac0: 2020 2020 2020 2020 2064 6174 615b 6969           data[ii
-0000cad0: 5d20 3d20 6461 7461 5b69 695d 202d 206e  ] = data[ii] - n
-0000cae0: 702e 646f 7428 582c 2063 6f65 6666 290a  p.dot(X, coeff).
-0000caf0: 2020 2020 7265 7475 726e 2064 6174 610a      return data.
-0000cb00: 0a0a 6465 6620 6465 6d65 616e 2864 6174  ..def demean(dat
-0000cb10: 6129 3a0a 2020 2020 2222 220a 2020 2020  a):.    """.    
-0000cb20: 7468 6973 2066 756e 6374 696f 6e20 7265  this function re
-0000cb30: 6d6f 7665 2074 6865 206d 6561 6e20 6f66  move the mean of
-0000cb40: 2074 6865 2073 6967 6e61 6c0a 2020 2020   the signal.    
-0000cb50: 5041 5241 4d45 5445 5253 3a0a 2020 2020  PARAMETERS:.    
-0000cb60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000cb70: 2d2d 2d2d 2d0a 2020 2020 6461 7461 3a20  -----.    data: 
-0000cb80: 696e 7075 7420 6461 7461 206d 6174 7269  input data matri
-0000cb90: 780a 2020 2020 5245 5455 524e 533a 0a20  x.    RETURNS:. 
-0000cba0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
-0000cbb0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 6174  --------.    dat
-0000cbc0: 613a 2064 6174 6120 6d61 7472 6978 2077  a: data matrix w
-0000cbd0: 6974 6820 6d65 616e 2072 656d 6f76 6564  ith mean removed
-0000cbe0: 0a20 2020 2022 2222 0a20 2020 2023 206e  .    """.    # n
-0000cbf0: 6461 7461 203d 206e 702e 7a65 726f 7328  data = np.zeros(
-0000cc00: 7368 6170 653d 6461 7461 2e73 6861 7065  shape=data.shape
-0000cc10: 2c64 7479 7065 3d64 6174 612e 6474 7970  ,dtype=data.dtyp
-0000cc20: 6529 0a20 2020 2069 6620 6461 7461 2e6e  e).    if data.n
-0000cc30: 6469 6d20 3d3d 2031 3a0a 2020 2020 2020  dim == 1:.      
-0000cc40: 2020 6461 7461 203d 2064 6174 6120 2d20    data = data - 
-0000cc50: 6e70 2e6d 6561 6e28 6461 7461 290a 2020  np.mean(data).  
-0000cc60: 2020 656c 6966 2064 6174 612e 6e64 696d    elif data.ndim
-0000cc70: 203d 3d20 323a 0a20 2020 2020 2020 2066   == 2:.        f
-0000cc80: 6f72 2069 6920 696e 2072 616e 6765 2864  or ii in range(d
-0000cc90: 6174 612e 7368 6170 655b 305d 293a 0a20  ata.shape[0]):. 
-0000cca0: 2020 2020 2020 2020 2020 2064 6174 615b             data[
-0000ccb0: 6969 5d20 3d20 6461 7461 5b69 695d 202d  ii] = data[ii] -
-0000ccc0: 206e 702e 6d65 616e 2864 6174 615b 6969   np.mean(data[ii
-0000ccd0: 5d29 0a20 2020 2072 6574 7572 6e20 6461  ]).    return da
-0000cce0: 7461 0a0a 0a64 6566 2074 6170 6572 2864  ta...def taper(d
-0000ccf0: 6174 6129 3a0a 2020 2020 2222 220a 2020  ata):.    """.  
-0000cd00: 2020 7468 6973 2066 756e 6374 696f 6e20    this function 
-0000cd10: 6170 706c 6965 7320 6120 636f 7369 6e65  applies a cosine
-0000cd20: 2074 6170 6572 2075 7369 6e67 206f 6273   taper using obs
-0000cd30: 7079 2066 756e 6374 696f 6e73 0a20 2020  py functions.   
-0000cd40: 2050 4152 414d 4554 4552 533a 0a20 2020   PARAMETERS:.   
-0000cd50: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-0000cd60: 2d2d 2d2d 2d2d 0a20 2020 2064 6174 613a  ------.    data:
-0000cd70: 2069 6e70 7574 2064 6174 6120 6d61 7472   input data matr
-0000cd80: 6978 0a20 2020 2052 4554 5552 4e53 3a0a  ix.    RETURNS:.
-0000cd90: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
-0000cda0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6461  ---------.    da
-0000cdb0: 7461 3a20 6461 7461 206d 6174 7269 7820  ta: data matrix 
-0000cdc0: 7769 7468 2074 6170 6572 2061 7070 6c69  with taper appli
-0000cdd0: 6564 0a20 2020 2022 2222 0a20 2020 2023  ed.    """.    #
-0000cde0: 206e 6461 7461 203d 206e 702e 7a65 726f   ndata = np.zero
-0000cdf0: 7328 7368 6170 653d 6461 7461 2e73 6861  s(shape=data.sha
-0000ce00: 7065 2c64 7479 7065 3d64 6174 612e 6474  pe,dtype=data.dt
-0000ce10: 7970 6529 0a20 2020 2069 6620 6461 7461  ype).    if data
-0000ce20: 2e6e 6469 6d20 3d3d 2031 3a0a 2020 2020  .ndim == 1:.    
-0000ce30: 2020 2020 6e70 7473 203d 2064 6174 612e      npts = data.
-0000ce40: 7368 6170 655b 305d 0a20 2020 2020 2020  shape[0].       
-0000ce50: 2023 2077 696e 646f 7720 6c65 6e67 7468   # window length
-0000ce60: 0a20 2020 2020 2020 2069 6620 6e70 7473  .        if npts
-0000ce70: 202a 2030 2e30 3520 3e20 3230 3a0a 2020   * 0.05 > 20:.  
-0000ce80: 2020 2020 2020 2020 2020 776c 656e 203d            wlen =
-0000ce90: 2032 300a 2020 2020 2020 2020 656c 7365   20.        else
-0000cea0: 3a0a 2020 2020 2020 2020 2020 2020 776c  :.            wl
-0000ceb0: 656e 203d 206e 7074 7320 2a20 302e 3035  en = npts * 0.05
-0000cec0: 0a20 2020 2020 2020 2023 2074 6170 6572  .        # taper
-0000ced0: 2076 616c 7565 730a 2020 2020 2020 2020   values.        
-0000cee0: 6675 6e63 203d 205f 6765 745f 6675 6e63  func = _get_func
-0000cef0: 7469 6f6e 5f66 726f 6d5f 656e 7472 795f  tion_from_entry_
-0000cf00: 706f 696e 7428 2274 6170 6572 222c 2022  point("taper", "
-0000cf10: 6861 6e6e 2229 0a20 2020 2020 2020 2069  hann").        i
-0000cf20: 6620 3220 2a20 776c 656e 203d 3d20 6e70  f 2 * wlen == np
-0000cf30: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
-0000cf40: 7461 7065 725f 7369 6465 7320 3d20 6675  taper_sides = fu
-0000cf50: 6e63 2832 202a 2077 6c65 6e29 0a20 2020  nc(2 * wlen).   
-0000cf60: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000cf70: 2020 2020 2020 2074 6170 6572 5f73 6964         taper_sid
-0000cf80: 6573 203d 2066 756e 6328 3220 2a20 776c  es = func(2 * wl
-0000cf90: 656e 202b 2031 290a 2020 2020 2020 2020  en + 1).        
-0000cfa0: 2320 7461 7065 7220 7769 6e64 6f77 0a20  # taper window. 
-0000cfb0: 2020 2020 2020 2077 696e 203d 206e 702e         win = np.
-0000cfc0: 6873 7461 636b 280a 2020 2020 2020 2020  hstack(.        
-0000cfd0: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
-0000cfe0: 2020 2020 2020 7461 7065 725f 7369 6465        taper_side
-0000cff0: 735b 3a77 6c65 6e5d 2c0a 2020 2020 2020  s[:wlen],.      
-0000d000: 2020 2020 2020 2020 2020 6e70 2e6f 6e65            np.one
-0000d010: 7328 6e70 7473 202d 2032 202a 2077 6c65  s(npts - 2 * wle
-0000d020: 6e29 2c0a 2020 2020 2020 2020 2020 2020  n),.            
-0000d030: 2020 2020 7461 7065 725f 7369 6465 735b      taper_sides[
-0000d040: 6c65 6e28 7461 7065 725f 7369 6465 7329  len(taper_sides)
-0000d050: 202d 2077 6c65 6e20 3a5d 2c0a 2020 2020   - wlen :],.    
-0000d060: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000d070: 2020 290a 2020 2020 2020 2020 6461 7461    ).        data
-0000d080: 202a 3d20 7769 6e0a 2020 2020 656c 6966   *= win.    elif
-0000d090: 2064 6174 612e 6e64 696d 203d 3d20 323a   data.ndim == 2:
-0000d0a0: 0a20 2020 2020 2020 206e 7074 7320 3d20  .        npts = 
-0000d0b0: 6461 7461 2e73 6861 7065 5b31 5d0a 2020  data.shape[1].  
-0000d0c0: 2020 2020 2020 2320 7769 6e64 6f77 206c        # window l
-0000d0d0: 656e 6774 680a 2020 2020 2020 2020 6966  ength.        if
-0000d0e0: 206e 7074 7320 2a20 302e 3035 203e 2032   npts * 0.05 > 2
-0000d0f0: 303a 0a20 2020 2020 2020 2020 2020 2077  0:.            w
-0000d100: 6c65 6e20 3d20 3230 0a20 2020 2020 2020  len = 20.       
-0000d110: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000d120: 2020 2077 6c65 6e20 3d20 6e70 7473 202a     wlen = npts *
-0000d130: 2030 2e30 350a 2020 2020 2020 2020 2320   0.05.        # 
-0000d140: 7461 7065 7220 7661 6c75 6573 0a20 2020  taper values.   
-0000d150: 2020 2020 2066 756e 6320 3d20 5f67 6574       func = _get
-0000d160: 5f66 756e 6374 696f 6e5f 6672 6f6d 5f65  _function_from_e
-0000d170: 6e74 7279 5f70 6f69 6e74 2822 7461 7065  ntry_point("tape
-0000d180: 7222 2c20 2268 616e 6e22 290a 2020 2020  r", "hann").    
-0000d190: 2020 2020 6966 2032 202a 2077 6c65 6e20      if 2 * wlen 
-0000d1a0: 3d3d 206e 7074 733a 0a20 2020 2020 2020  == npts:.       
-0000d1b0: 2020 2020 2074 6170 6572 5f73 6964 6573       taper_sides
-0000d1c0: 203d 2066 756e 6328 3220 2a20 776c 656e   = func(2 * wlen
-0000d1d0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-0000d1e0: 2020 2020 2020 2020 2020 2020 7461 7065              tape
-0000d1f0: 725f 7369 6465 7320 3d20 6675 6e63 2832  r_sides = func(2
-0000d200: 202a 2077 6c65 6e20 2b20 3129 0a20 2020   * wlen + 1).   
-0000d210: 2020 2020 2023 2074 6170 6572 2077 696e       # taper win
-0000d220: 646f 770a 2020 2020 2020 2020 7769 6e20  dow.        win 
-0000d230: 3d20 6e70 2e68 7374 6163 6b28 0a20 2020  = np.hstack(.   
-0000d240: 2020 2020 2020 2020 2028 0a20 2020 2020           (.     
-0000d250: 2020 2020 2020 2020 2020 2074 6170 6572             taper
-0000d260: 5f73 6964 6573 5b3a 776c 656e 5d2c 0a20  _sides[:wlen],. 
-0000d270: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000d280: 702e 6f6e 6573 286e 7074 7320 2d20 3220  p.ones(npts - 2 
-0000d290: 2a20 776c 656e 292c 0a20 2020 2020 2020  * wlen),.       
-0000d2a0: 2020 2020 2020 2020 2074 6170 6572 5f73           taper_s
-0000d2b0: 6964 6573 5b6c 656e 2874 6170 6572 5f73  ides[len(taper_s
-0000d2c0: 6964 6573 2920 2d20 776c 656e 203a 5d2c  ides) - wlen :],
-0000d2d0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0000d2e0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000d2f0: 2066 6f72 2069 6920 696e 2072 616e 6765   for ii in range
-0000d300: 2864 6174 612e 7368 6170 655b 305d 293a  (data.shape[0]):
-0000d310: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-0000d320: 615b 6969 5d20 2a3d 2077 696e 0a20 2020  a[ii] *= win.   
-0000d330: 2072 6574 7572 6e20 6461 7461 0a0a 0a23   return data...#
-0000d340: 2040 6a69 7428 6e6f 7079 7468 6f6e 203d   @jit(nopython =
-0000d350: 2054 7275 6529 0a0a 0a23 2063 6861 6e67   True)...# chang
-0000d360: 6520 7468 6520 6d6f 7669 6e67 2061 7665  e the moving ave
-0000d370: 7261 6765 2063 616c 6375 6c61 7469 6f6e  rage calculation
-0000d380: 2074 6f20 7461 6b65 2061 7320 696e 7075   to take as inpu
-0000d390: 7420 4e20 7468 6520 6675 6c6c 2077 696e  t N the full win
-0000d3a0: 646f 7720 6c65 6e67 7468 2074 6f20 736d  dow length to sm
-0000d3b0: 6f6f 7468 0a64 6566 206d 6f76 696e 675f  ooth.def moving_
-0000d3c0: 6176 6528 412c 204e 293a 0a20 2020 2022  ave(A, N):.    "
-0000d3d0: 2222 0a20 2020 2041 6c74 6572 6e61 7469  "".    Alternati
-0000d3e0: 7665 2066 756e 6374 696f 6e20 666f 7220  ve function for 
-0000d3f0: 6d6f 7669 6e67 2061 7665 7261 6765 2066  moving average f
-0000d400: 6f72 2061 6e20 6172 7261 792e 0a20 2020  or an array..   
-0000d410: 2050 4152 414d 4554 4552 533a 0a20 2020   PARAMETERS:.   
-0000d420: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-0000d430: 2d2d 2d2d 2d2d 0a20 2020 2041 3a20 312d  ------.    A: 1-
-0000d440: 4420 6172 7261 7920 6f66 2064 6174 6120  D array of data 
-0000d450: 746f 2062 6520 736d 6f6f 7468 6564 0a20  to be smoothed. 
-0000d460: 2020 204e 3a20 696e 7465 6765 722c 2069     N: integer, i
-0000d470: 7420 6465 6669 6e65 7320 7468 6520 6675  t defines the fu
-0000d480: 6c6c 2121 2077 696e 646f 7720 6c65 6e67  ll!! window leng
-0000d490: 7468 2074 6f20 736d 6f6f 7468 0a20 2020  th to smooth.   
-0000d4a0: 2052 4554 5552 4e53 3a0a 2020 2020 2d2d   RETURNS:.    --
-0000d4b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000d4c0: 2d2d 2d0a 2020 2020 423a 2031 2d44 2061  ---.    B: 1-D a
-0000d4d0: 7272 6179 2077 6974 6820 736d 6f6f 7468  rray with smooth
-0000d4e0: 6564 2064 6174 610a 2020 2020 2222 220a  ed data.    """.
-0000d4f0: 2020 2020 2320 6465 6669 6e65 7320 616e      # defines an
-0000d500: 2061 7272 6179 2077 6974 6820 4e20 6578   array with N ex
-0000d510: 7472 6120 7361 6d70 6c65 7320 6174 2065  tra samples at e
-0000d520: 6974 6865 7220 7369 6465 0a20 2020 2074  ither side.    t
-0000d530: 656d 7020 3d20 6e70 2e7a 6572 6f73 286c  emp = np.zeros(l
-0000d540: 656e 2841 2920 2b20 3220 2a20 4e29 0a20  en(A) + 2 * N). 
-0000d550: 2020 2023 2073 6574 2074 6865 2063 656e     # set the cen
-0000d560: 7472 616c 2070 6f72 7469 6f6e 206f 6620  tral portion of 
-0000d570: 7468 6520 6172 7261 7920 746f 2041 0a20  the array to A. 
-0000d580: 2020 2074 656d 705b 4e3a 2d4e 5d20 3d20     temp[N:-N] = 
-0000d590: 410a 2020 2020 2320 6c65 6164 696e 6720  A.    # leading 
-0000d5a0: 7361 6d70 6c65 733a 2065 7175 616c 2074  samples: equal t
-0000d5b0: 6f20 6669 7273 7420 7361 6d70 6c65 206f  o first sample o
-0000d5c0: 6620 6163 7475 616c 2061 7272 6179 0a20  f actual array. 
-0000d5d0: 2020 2074 656d 705b 303a 4e5d 203d 2074     temp[0:N] = t
-0000d5e0: 656d 705b 4e5d 0a20 2020 2023 2074 7261  emp[N].    # tra
-0000d5f0: 696c 696e 6720 7361 6d70 6c65 733a 2045  iling samples: E
-0000d600: 7175 616c 2074 6f20 6c61 7374 2073 616d  qual to last sam
-0000d610: 706c 6520 6f66 2061 6374 7561 6c20 6172  ple of actual ar
-0000d620: 7261 790a 2020 2020 7465 6d70 5b2d 4e3a  ray.    temp[-N:
-0000d630: 5d20 3d20 7465 6d70 5b2d 4e20 2d20 315d  ] = temp[-N - 1]
-0000d640: 0a20 2020 2023 2063 6f6e 766f 6c76 6520  .    # convolve 
-0000d650: 7769 7468 2061 2062 6f78 6361 7220 616e  with a boxcar an
-0000d660: 6420 6e6f 726d 616c 697a 652c 2061 6e64  d normalize, and
-0000d670: 2075 7365 206f 6e6c 7920 6365 6e74 7261   use only centra
-0000d680: 6c20 706f 7274 696f 6e20 6f66 2074 6865  l portion of the
-0000d690: 2072 6573 756c 740a 2020 2020 2320 7769   result.    # wi
-0000d6a0: 7468 206c 656e 6774 6820 6571 7561 6c20  th length equal 
-0000d6b0: 746f 2074 6865 206f 7269 6769 6e61 6c20  to the original 
-0000d6c0: 6172 7261 792c 2064 6973 6361 7264 696e  array, discardin
-0000d6d0: 6720 7468 6520 6164 6465 6420 6c65 6164  g the added lead
-0000d6e0: 696e 6720 616e 6420 7472 6169 6c69 6e67  ing and trailing
-0000d6f0: 2073 616d 706c 6573 0a20 2020 2042 203d   samples.    B =
-0000d700: 206e 702e 636f 6e76 6f6c 7665 2874 656d   np.convolve(tem
-0000d710: 702c 206e 702e 6f6e 6573 284e 2920 2f20  p, np.ones(N) / 
-0000d720: 4e2c 206d 6f64 653d 2273 616d 6522 295b  N, mode="same")[
-0000d730: 4e3a 2d4e 5d0a 2020 2020 7265 7475 726e  N:-N].    return
-0000d740: 2042 0a0a 0a23 2063 6861 6e67 6520 7468   B...# change th
-0000d750: 6520 6d6f 7669 6e67 2061 7665 7261 6765  e moving average
-0000d760: 2063 616c 6375 6c61 7469 6f6e 2074 6f20   calculation to 
-0000d770: 7461 6b65 2061 7320 696e 7075 7420 4e20  take as input N 
-0000d780: 7468 6520 6675 6c6c 2077 696e 646f 7720  the full window 
-0000d790: 6c65 6e67 7468 2074 6f20 736d 6f6f 7468  length to smooth
-0000d7a0: 0a64 6566 206d 6f76 696e 675f 6176 655f  .def moving_ave_
-0000d7b0: 3244 2841 2c20 4e29 3a0a 2020 2020 2222  2D(A, N):.    ""
-0000d7c0: 220a 2020 2020 416c 7465 726e 6174 6976  ".    Alternativ
-0000d7d0: 6520 6675 6e63 7469 6f6e 2066 6f72 206d  e function for m
-0000d7e0: 6f76 696e 6720 6176 6572 6167 6520 666f  oving average fo
-0000d7f0: 7220 616e 2061 7272 6179 2e0a 2020 2020  r an array..    
-0000d800: 5041 5241 4d45 5445 5253 3a0a 2020 2020  PARAMETERS:.    
-0000d810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000d820: 2d2d 2d2d 2d0a 2020 2020 413a 2032 2d44  -----.    A: 2-D
-0000d830: 2061 7272 6179 206f 6620 6461 7461 2074   array of data t
-0000d840: 6f20 6265 2073 6d6f 6f74 6865 640a 2020  o be smoothed.  
-0000d850: 2020 4e3a 2069 6e74 6567 6572 2c20 6974    N: integer, it
-0000d860: 2064 6566 696e 6573 2074 6865 2066 756c   defines the ful
-0000d870: 6c21 2120 7769 6e64 6f77 206c 656e 6774  l!! window lengt
-0000d880: 6820 746f 2073 6d6f 6f74 680a 2020 2020  h to smooth.    
-0000d890: 5245 5455 524e 533a 0a20 2020 202d 2d2d  RETURNS:.    ---
-0000d8a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000d8b0: 2d2d 0a20 2020 2042 3a20 322d 4420 6172  --.    B: 2-D ar
-0000d8c0: 7261 7920 7769 7468 2073 6d6f 6f74 6865  ray with smoothe
-0000d8d0: 6420 6461 7461 0a20 2020 2022 2222 0a20  d data.    """. 
-0000d8e0: 2020 206e 7463 2c20 6e73 7074 203d 2041     ntc, nspt = A
-0000d8f0: 2e73 6861 7065 0a20 2020 2023 2064 6566  .shape.    # def
-0000d900: 696e 6573 2061 6e20 6172 7261 7920 7769  ines an array wi
-0000d910: 7468 204e 2065 7874 7261 2073 616d 706c  th N extra sampl
-0000d920: 6573 2061 7420 6569 7468 6572 2073 6964  es at either sid
-0000d930: 650a 2020 2020 7465 6d70 203d 206e 702e  e.    temp = np.
-0000d940: 7a65 726f 7328 5b6e 7463 2c20 6e73 7074  zeros([ntc, nspt
-0000d950: 202b 2032 202a 204e 5d29 0a20 2020 2023   + 2 * N]).    #
-0000d960: 2073 6574 2074 6865 2063 656e 7472 616c   set the central
-0000d970: 2070 6f72 7469 6f6e 206f 6620 7468 6520   portion of the 
-0000d980: 6172 7261 7920 746f 2041 0a20 2020 2074  array to A.    t
-0000d990: 656d 705b 3a2c 204e 3a2d 4e5d 203d 2041  emp[:, N:-N] = A
-0000d9a0: 0a20 2020 2023 206c 6561 6469 6e67 2073  .    # leading s
-0000d9b0: 616d 706c 6573 3a20 6571 7561 6c20 746f  amples: equal to
-0000d9c0: 2066 6972 7374 2073 616d 706c 6520 6f66   first sample of
-0000d9d0: 2061 6374 7561 6c20 6172 7261 790a 2020   actual array.  
-0000d9e0: 2020 7465 6d70 5b3a 2c20 303a 4e5d 203d    temp[:, 0:N] =
-0000d9f0: 206e 702e 7265 7065 6174 286e 702e 6578   np.repeat(np.ex
-0000da00: 7061 6e64 5f64 696d 7328 7465 6d70 5b3a  pand_dims(temp[:
-0000da10: 2c20 4e5d 2c20 6178 6973 3d2d 3129 2c20  , N], axis=-1), 
-0000da20: 4e2c 2061 7869 733d 2d31 290a 2020 2020  N, axis=-1).    
-0000da30: 2320 7472 6169 6c69 6e67 2073 616d 706c  # trailing sampl
-0000da40: 6573 3a20 4571 7561 6c20 746f 206c 6173  es: Equal to las
-0000da50: 7420 7361 6d70 6c65 206f 6620 6163 7475  t sample of actu
-0000da60: 616c 2061 7272 6179 0a20 2020 2074 656d  al array.    tem
-0000da70: 705b 3a2c 202d 4e3a 5d20 3d20 6e70 2e72  p[:, -N:] = np.r
-0000da80: 6570 6561 7428 6e70 2e65 7870 616e 645f  epeat(np.expand_
-0000da90: 6469 6d73 2874 656d 705b 3a2c 202d 4e20  dims(temp[:, -N 
-0000daa0: 2d20 315d 2c20 6178 6973 3d2d 3129 2c20  - 1], axis=-1), 
-0000dab0: 4e2c 2061 7869 733d 2d31 290a 2020 2020  N, axis=-1).    
-0000dac0: 2320 636f 6e76 6f6c 7665 2077 6974 6820  # convolve with 
-0000dad0: 6120 626f 7863 6172 2061 6e64 206e 6f72  a boxcar and nor
-0000dae0: 6d61 6c69 7a65 2c20 616e 6420 7573 6520  malize, and use 
-0000daf0: 6f6e 6c79 2063 656e 7472 616c 2070 6f72  only central por
-0000db00: 7469 6f6e 206f 6620 7468 6520 7265 7375  tion of the resu
-0000db10: 6c74 0a20 2020 2023 2077 6974 6820 6c65  lt.    # with le
-0000db20: 6e67 7468 2065 7175 616c 2074 6f20 7468  ngth equal to th
-0000db30: 6520 6f72 6967 696e 616c 2061 7272 6179  e original array
-0000db40: 2c20 6469 7363 6172 6469 6e67 2074 6865  , discarding the
-0000db50: 2061 6464 6564 206c 6561 6469 6e67 2061   added leading a
-0000db60: 6e64 2074 7261 696c 696e 6720 7361 6d70  nd trailing samp
-0000db70: 6c65 730a 2020 2020 4220 3d20 7363 6970  les.    B = scip
-0000db80: 792e 7369 676e 616c 2e63 6f6e 766f 6c76  y.signal.convolv
-0000db90: 6532 6428 7465 6d70 2c20 6e70 2e65 7870  e2d(temp, np.exp
-0000dba0: 616e 645f 6469 6d73 286e 702e 6f6e 6573  and_dims(np.ones
-0000dbb0: 284e 2920 2f20 4e2c 2061 7869 733d 3029  (N) / N, axis=0)
-0000dbc0: 2c20 6d6f 6465 3d22 7361 6d65 2229 5b3a  , mode="same")[:
-0000dbd0: 2c20 4e3a 2d4e 5d0a 2020 2020 7265 7475  , N:-N].    retu
-0000dbe0: 726e 2042 0a0a 0a64 6566 2072 6f62 7573  rn B...def robus
-0000dbf0: 745f 7374 6163 6b28 6363 5f61 7272 6179  t_stack(cc_array
-0000dc00: 2c20 6570 7369 6c6f 6e29 3a0a 2020 2020  , epsilon):.    
-0000dc10: 2222 220a 2020 2020 7468 6973 2069 7320  """.    this is 
-0000dc20: 6120 726f 6275 7374 2073 7461 636b 696e  a robust stackin
-0000dc30: 6720 616c 676f 7269 7468 6d20 6465 7363  g algorithm desc
-0000dc40: 7269 6265 6420 696e 2050 616c 7669 7320  ribed in Palvis 
-0000dc50: 616e 6420 5665 726e 6f6e 2032 3031 300a  and Vernon 2010.
-0000dc60: 0a20 2020 2050 4152 414d 4554 4552 533a  .    PARAMETERS:
-0000dc70: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
-0000dc80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
-0000dc90: 6363 5f61 7272 6179 3a20 6e75 6d70 792e  cc_array: numpy.
-0000dca0: 6e64 6172 7261 7920 636f 6e74 6169 6e73  ndarray contains
-0000dcb0: 2074 6865 2032 4420 6372 6f73 7320 636f   the 2D cross co
-0000dcc0: 7272 656c 6174 696f 6e20 6d61 7472 6978  rrelation matrix
-0000dcd0: 0a20 2020 2065 7073 696c 6f6e 3a20 7265  .    epsilon: re
-0000dce0: 7369 6475 616c 2074 6872 6568 6f6c 6420  sidual threhold 
-0000dcf0: 746f 2071 7569 7420 7468 6520 6974 6572  to quit the iter
-0000dd00: 6174 696f 6e0a 2020 2020 5245 5455 524e  ation.    RETURN
-0000dd10: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
-0000dd20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-0000dd30: 2020 6e65 7773 7461 636b 3a20 6e75 6d70    newstack: nump
-0000dd40: 7920 7665 6374 6f72 2063 6f6e 7461 696e  y vector contain
-0000dd50: 7320 7468 6520 7374 6163 6b65 6420 6372  s the stacked cr
-0000dd60: 6f73 7320 636f 7272 656c 6174 696f 6e0a  oss correlation.
-0000dd70: 0a20 2020 2057 7269 7474 656e 2062 7920  .    Written by 
-0000dd80: 4d61 7269 6e65 2044 656e 6f6c 6c65 0a20  Marine Denolle. 
-0000dd90: 2020 2022 2222 0a20 2020 2072 6573 203d     """.    res =
-0000dda0: 2039 6539 2020 2320 7265 7369 6475 616c   9e9  # residual
-0000ddb0: 730a 2020 2020 7720 3d20 6e70 2e6f 6e65  s.    w = np.one
-0000ddc0: 7328 6363 5f61 7272 6179 2e73 6861 7065  s(cc_array.shape
-0000ddd0: 5b30 5d29 0a20 2020 206e 7374 6570 203d  [0]).    nstep =
-0000dde0: 2030 0a20 2020 206e 6577 7374 6163 6b20   0.    newstack 
-0000ddf0: 3d20 6e70 2e6d 6564 6961 6e28 6363 5f61  = np.median(cc_a
-0000de00: 7272 6179 2c20 6178 6973 3d30 290a 2020  rray, axis=0).  
-0000de10: 2020 7768 696c 6520 7265 7320 3e20 6570    while res > ep
-0000de20: 7369 6c6f 6e3a 0a20 2020 2020 2020 2073  silon:.        s
-0000de30: 7461 636b 203d 206e 6577 7374 6163 6b0a  tack = newstack.
-0000de40: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-0000de50: 2072 616e 6765 2863 635f 6172 7261 792e   range(cc_array.
-0000de60: 7368 6170 655b 305d 293a 0a20 2020 2020  shape[0]):.     
-0000de70: 2020 2020 2020 2063 7261 7020 3d20 6e70         crap = np
-0000de80: 2e6d 756c 7469 706c 7928 7374 6163 6b2c  .multiply(stack,
-0000de90: 2063 635f 6172 7261 795b 692c 203a 5d2e   cc_array[i, :].
-0000dea0: 5429 0a20 2020 2020 2020 2020 2020 2063  T).            c
-0000deb0: 7261 705f 646f 7420 3d20 6e70 2e73 756d  rap_dot = np.sum
-0000dec0: 2863 7261 7029 0a20 2020 2020 2020 2020  (crap).         
-0000ded0: 2020 2064 695f 6e6f 726d 203d 206e 702e     di_norm = np.
-0000dee0: 6c69 6e61 6c67 2e6e 6f72 6d28 6363 5f61  linalg.norm(cc_a
-0000def0: 7272 6179 5b69 2c20 3a5d 290a 2020 2020  rray[i, :]).    
-0000df00: 2020 2020 2020 2020 7269 203d 2063 635f          ri = cc_
-0000df10: 6172 7261 795b 692c 203a 5d20 2d20 6372  array[i, :] - cr
-0000df20: 6170 5f64 6f74 202a 2073 7461 636b 0a20  ap_dot * stack. 
-0000df30: 2020 2020 2020 2020 2020 2072 695f 6e6f             ri_no
-0000df40: 726d 203d 206e 702e 6c69 6e61 6c67 2e6e  rm = np.linalg.n
-0000df50: 6f72 6d28 7269 290a 2020 2020 2020 2020  orm(ri).        
-0000df60: 2020 2020 775b 695d 203d 206e 702e 6162      w[i] = np.ab
-0000df70: 7328 6372 6170 5f64 6f74 2920 2f20 6469  s(crap_dot) / di
-0000df80: 5f6e 6f72 6d20 2f20 7269 5f6e 6f72 6d20  _norm / ri_norm 
-0000df90: 2023 202f 6c65 6e28 6363 5f61 7272 6179   # /len(cc_array
-0000dfa0: 5b3a 2c31 5d29 0a20 2020 2020 2020 2023  [:,1]).        #
-0000dfb0: 2070 7269 6e74 2877 290a 2020 2020 2020   print(w).      
-0000dfc0: 2020 7720 3d20 7720 2f20 6e70 2e73 756d    w = w / np.sum
-0000dfd0: 2877 290a 2020 2020 2020 2020 6e65 7773  (w).        news
-0000dfe0: 7461 636b 203d 206e 702e 7375 6d28 2877  tack = np.sum((w
-0000dff0: 202a 2063 635f 6172 7261 792e 5429 2e54   * cc_array.T).T
-0000e000: 2c20 6178 6973 3d30 2920 2023 202f 6c65  , axis=0)  # /le
-0000e010: 6e28 6363 5f61 7272 6179 5b3a 2c31 5d29  n(cc_array[:,1])
-0000e020: 0a20 2020 2020 2020 2072 6573 203d 206e  .        res = n
-0000e030: 702e 6c69 6e61 6c67 2e6e 6f72 6d28 6e65  p.linalg.norm(ne
-0000e040: 7773 7461 636b 202d 2073 7461 636b 2c20  wstack - stack, 
-0000e050: 6f72 643d 3129 202f 206e 702e 6c69 6e61  ord=1) / np.lina
-0000e060: 6c67 2e6e 6f72 6d28 6e65 7773 7461 636b  lg.norm(newstack
-0000e070: 2920 2f20 6c65 6e28 6363 5f61 7272 6179  ) / len(cc_array
-0000e080: 5b3a 2c20 315d 290a 2020 2020 2020 2020  [:, 1]).        
-0000e090: 6e73 7465 7020 2b3d 2031 0a20 2020 2020  nstep += 1.     
-0000e0a0: 2020 2069 6620 6e73 7465 7020 3e20 3130     if nstep > 10
-0000e0b0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000e0c0: 7475 726e 206e 6577 7374 6163 6b2c 2077  turn newstack, w
-0000e0d0: 2c20 6e73 7465 700a 2020 2020 7265 7475  , nstep.    retu
-0000e0e0: 726e 206e 6577 7374 6163 6b2c 2077 2c20  rn newstack, w, 
-0000e0f0: 6e73 7465 700a 0a0a 6465 6620 7365 6c65  nstep...def sele
-0000e100: 6374 6976 655f 7374 6163 6b28 6363 5f61  ctive_stack(cc_a
-0000e110: 7272 6179 2c20 6570 7369 6c6f 6e29 3a0a  rray, epsilon):.
-0000e120: 2020 2020 2222 220a 2020 2020 7468 6973      """.    this
-0000e130: 2069 7320 6120 7365 6c65 6374 6976 6520   is a selective 
-0000e140: 7374 6163 6b69 6e67 2061 6c67 6f72 6974  stacking algorit
-0000e150: 686d 2064 6576 656c 6f70 6564 2062 7920  hm developed by 
-0000e160: 4a61 7265 6420 4272 7961 6e2e 0a0a 2020  Jared Bryan...  
-0000e170: 2020 5041 5241 4d45 5445 5253 3a0a 2020    PARAMETERS:.  
-0000e180: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
-0000e190: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2063 635f  --------.    cc_
-0000e1a0: 6172 7261 793a 206e 756d 7079 2e6e 6461  array: numpy.nda
-0000e1b0: 7272 6179 2063 6f6e 7461 696e 7320 7468  rray contains th
-0000e1c0: 6520 3244 2063 726f 7373 2063 6f72 7265  e 2D cross corre
-0000e1d0: 6c61 7469 6f6e 206d 6174 7269 780a 2020  lation matrix.  
-0000e1e0: 2020 6570 7369 6c6f 6e3a 2072 6573 6964    epsilon: resid
-0000e1f0: 7561 6c20 7468 7265 686f 6c64 2074 6f20  ual threhold to 
-0000e200: 7175 6974 2074 6865 2069 7465 7261 7469  quit the iterati
-0000e210: 6f6e 0a20 2020 2052 4554 5552 4e53 3a0a  on.    RETURNS:.
-0000e220: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
-0000e230: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 206e  ----------.    n
-0000e240: 6577 7374 6163 6b3a 206e 756d 7079 2076  ewstack: numpy v
-0000e250: 6563 746f 7220 636f 6e74 6169 6e73 2074  ector contains t
-0000e260: 6865 2073 7461 636b 6564 2063 726f 7373  he stacked cross
-0000e270: 2063 6f72 7265 6c61 7469 6f6e 0a0a 2020   correlation..  
-0000e280: 2020 5772 6974 7465 6e20 6279 204d 6172    Written by Mar
-0000e290: 696e 6520 4465 6e6f 6c6c 650a 2020 2020  ine Denolle.    
-0000e2a0: 2222 220a 2020 2020 6363 203d 206e 702e  """.    cc = np.
-0000e2b0: 6f6e 6573 2863 635f 6172 7261 792e 7368  ones(cc_array.sh
-0000e2c0: 6170 655b 305d 290a 2020 2020 6e65 7773  ape[0]).    news
-0000e2d0: 7461 636b 203d 206e 702e 6d65 616e 2863  tack = np.mean(c
-0000e2e0: 635f 6172 7261 792c 2061 7869 733d 3029  c_array, axis=0)
-0000e2f0: 0a20 2020 2066 6f72 2069 2069 6e20 7261  .    for i in ra
-0000e300: 6e67 6528 6363 5f61 7272 6179 2e73 6861  nge(cc_array.sha
-0000e310: 7065 5b30 5d29 3a0a 2020 2020 2020 2020  pe[0]):.        
-0000e320: 6363 5b69 5d20 3d20 6e70 2e73 756d 286e  cc[i] = np.sum(n
-0000e330: 702e 6d75 6c74 6970 6c79 286e 6577 7374  p.multiply(newst
-0000e340: 6163 6b2c 2063 635f 6172 7261 795b 692c  ack, cc_array[i,
-0000e350: 203a 5d2e 5429 290a 2020 2020 696b 203d   :].T)).    ik =
-0000e360: 206e 702e 7768 6572 6528 6363 203e 3d20   np.where(cc >= 
-0000e370: 6570 7369 6c6f 6e29 5b30 5d0a 2020 2020  epsilon)[0].    
-0000e380: 6e65 7773 7461 636b 203d 206e 702e 6d65  newstack = np.me
-0000e390: 616e 2863 635f 6172 7261 795b 696b 2c20  an(cc_array[ik, 
-0000e3a0: 3a5d 2c20 6178 6973 3d30 290a 0a20 2020  :], axis=0)..   
-0000e3b0: 2072 6574 7572 6e20 6e65 7773 7461 636b   return newstack
-0000e3c0: 2c20 6363 0a0a 0a64 6566 2077 6869 7465  , cc...def white
-0000e3d0: 6e5f 3144 2874 696d 6573 6572 6965 732c  n_1D(timeseries,
-0000e3e0: 2066 6674 5f70 6172 612c 206e 5f74 6170   fft_para, n_tap
-0000e3f0: 6572 293a 0a20 2020 2022 2222 0a20 2020  er):.    """.   
-0000e400: 2054 6869 7320 6675 6e63 7469 6f6e 2074   This function t
-0000e410: 616b 6573 2061 2031 2d64 696d 656e 7369  akes a 1-dimensi
-0000e420: 6f6e 616c 2074 696d 6573 6572 6965 7320  onal timeseries 
-0000e430: 6172 7261 792c 2074 7261 6e73 666f 726d  array, transform
-0000e440: 7320 746f 2066 7265 7175 656e 6379 2064  s to frequency d
-0000e450: 6f6d 6169 6e20 7573 696e 6720 6666 742c  omain using fft,
-0000e460: 0a20 2020 2077 6869 7465 6e73 2074 6865  .    whitens the
-0000e470: 2061 6d70 6c69 7475 6465 206f 6620 7468   amplitude of th
-0000e480: 6520 7370 6563 7472 756d 2069 6e20 6672  e spectrum in fr
-0000e490: 6571 7565 6e63 7920 646f 6d61 696e 2062  equency domain b
-0000e4a0: 6574 7765 656e 202a 6672 6571 6d69 6e2a  etween *freqmin*
-0000e4b0: 2061 6e64 202a 6672 6571 6d61 782a 0a20   and *freqmax*. 
-0000e4c0: 2020 2061 6e64 2072 6574 7572 6e73 2074     and returns t
-0000e4d0: 6865 2077 6869 7465 6e65 6420 6666 742e  he whitened fft.
-0000e4e0: 0a20 2020 2050 4152 414d 4554 4552 533a  .    PARAMETERS:
-0000e4f0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
-0000e500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
-0000e510: 6461 7461 3a20 6e75 6d70 792e 6e64 6172  data: numpy.ndar
-0000e520: 7261 7920 636f 6e74 6169 6e73 2074 6865  ray contains the
-0000e530: 2031 4420 7469 6d65 2073 6572 6965 7320   1D time series 
-0000e540: 746f 2077 6869 7465 6e0a 2020 2020 6666  to whiten.    ff
-0000e550: 745f 7061 7261 3a20 6469 6374 2063 6f6e  t_para: dict con
-0000e560: 7461 696e 696e 6720 616c 6c20 6666 745f  taining all fft_
-0000e570: 6363 2070 6172 616d 6574 6572 7320 7375  cc parameters su
-0000e580: 6368 2061 730a 2020 2020 2020 2020 6474  ch as.        dt
-0000e590: 3a20 5468 6520 7361 6d70 6c69 6e67 2073  : The sampling s
-0000e5a0: 7061 6365 206f 6620 7468 6520 6064 6174  pace of the `dat
-0000e5b0: 6160 0a20 2020 2020 2020 2066 7265 716d  a`.        freqm
-0000e5c0: 696e 3a20 5468 6520 6c6f 7765 7220 6672  in: The lower fr
-0000e5d0: 6571 7565 6e63 7920 626f 756e 640a 2020  equency bound.  
-0000e5e0: 2020 2020 2020 6672 6571 6d61 783a 2054        freqmax: T
-0000e5f0: 6865 2075 7070 6572 2066 7265 7175 656e  he upper frequen
-0000e600: 6379 2062 6f75 6e64 0a20 2020 2020 2020  cy bound.       
-0000e610: 2073 6d6f 6f74 685f 4e3a 2069 6e74 6567   smooth_N: integ
-0000e620: 6572 2c20 6974 2064 6566 696e 6573 2074  er, it defines t
-0000e630: 6865 2068 616c 6620 7769 6e64 6f77 206c  he half window l
-0000e640: 656e 6774 6820 746f 2073 6d6f 6f74 680a  ength to smooth.
-0000e650: 2020 2020 2020 2020 6e5f 7461 7065 722c          n_taper,
-0000e660: 206f 7074 696f 6e61 6c3a 2069 6e74 6567   optional: integ
-0000e670: 6572 2c20 6465 6669 6e65 2074 6865 2077  er, define the w
-0000e680: 6964 7468 206f 6620 7468 6520 7461 7065  idth of the tape
-0000e690: 7220 696e 2073 616d 706c 6573 0a20 2020  r in samples.   
-0000e6a0: 2052 4554 5552 4e53 3a0a 2020 2020 2d2d   RETURNS:.    --
-0000e6b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000e6c0: 2d2d 2d2d 0a20 2020 2046 4654 5261 7753  ----.    FFTRawS
-0000e6d0: 6967 6e3a 206e 756d 7079 2e6e 6461 7272  ign: numpy.ndarr
-0000e6e0: 6179 2063 6f6e 7461 696e 7320 7468 6520  ay contains the 
-0000e6f0: 4646 5420 6f66 2074 6865 2077 6869 7465  FFT of the white
-0000e700: 6e65 6420 696e 7075 7420 7472 6163 6520  ned input trace 
-0000e710: 6265 7477 6565 6e20 7468 6520 6672 6571  between the freq
-0000e720: 7565 6e63 7920 626f 756e 6473 0a20 2020  uency bounds.   
-0000e730: 2022 2222 0a20 2020 2023 206c 6f61 6420   """.    # load 
-0000e740: 7061 7261 6d65 7465 7273 0a20 2020 2064  parameters.    d
-0000e750: 656c 7461 203d 2066 6674 5f70 6172 615b  elta = fft_para[
-0000e760: 2264 7422 5d0a 2020 2020 6672 6571 6d69  "dt"].    freqmi
-0000e770: 6e20 3d20 6666 745f 7061 7261 5b22 6672  n = fft_para["fr
-0000e780: 6571 6d69 6e22 5d0a 2020 2020 6672 6571  eqmin"].    freq
-0000e790: 6d61 7820 3d20 6666 745f 7061 7261 5b22  max = fft_para["
-0000e7a0: 6672 6571 6d61 7822 5d0a 2020 2020 736d  freqmax"].    sm
-0000e7b0: 6f6f 7468 5f4e 203d 2066 6674 5f70 6172  ooth_N = fft_par
-0000e7c0: 615b 2273 6d6f 6f74 685f 4e22 5d0a 0a20  a["smooth_N"].. 
-0000e7d0: 2020 206e 6666 7420 3d20 6e65 7874 5f66     nfft = next_f
-0000e7e0: 6173 745f 6c65 6e28 6c65 6e28 7469 6d65  ast_len(len(time
-0000e7f0: 7365 7269 6573 2929 0a20 2020 2073 7065  series)).    spe
-0000e800: 6320 3d20 6e70 2e66 6674 2e66 6674 2874  c = np.fft.fft(t
-0000e810: 696d 6573 6572 6965 732c 206e 6666 7429  imeseries, nfft)
-0000e820: 0a20 2020 2066 7265 7120 3d20 6e70 2e66  .    freq = np.f
-0000e830: 6674 2e66 6674 6672 6571 286e 6666 742c  ft.fftfreq(nfft,
-0000e840: 2064 3d64 656c 7461 290a 0a20 2020 2069   d=delta)..    i
-0000e850: 7830 203d 206e 702e 6172 676d 696e 286e  x0 = np.argmin(n
-0000e860: 702e 6162 7328 6672 6571 202d 2066 7265  p.abs(freq - fre
-0000e870: 716d 696e 2929 0a20 2020 2069 7831 203d  qmin)).    ix1 =
-0000e880: 206e 702e 6172 676d 696e 286e 702e 6162   np.argmin(np.ab
-0000e890: 7328 6672 6571 202d 2066 7265 716d 6178  s(freq - freqmax
-0000e8a0: 2929 0a0a 2020 2020 6966 2069 7831 202b  ))..    if ix1 +
-0000e8b0: 206e 5f74 6170 6572 203e 206e 6666 743a   n_taper > nfft:
-0000e8c0: 0a20 2020 2020 2020 2069 7831 3120 3d20  .        ix11 = 
-0000e8d0: 6e66 6674 0a20 2020 2065 6c73 653a 0a20  nfft.    else:. 
-0000e8e0: 2020 2020 2020 2069 7831 3120 3d20 6978         ix11 = ix
-0000e8f0: 3120 2b20 6e5f 7461 7065 720a 0a20 2020  1 + n_taper..   
-0000e900: 2069 6620 6978 3020 2d20 6e5f 7461 7065   if ix0 - n_tape
-0000e910: 7220 3c20 303a 0a20 2020 2020 2020 2069  r < 0:.        i
-0000e920: 7830 3020 3d20 300a 2020 2020 656c 7365  x00 = 0.    else
-0000e930: 3a0a 2020 2020 2020 2020 6978 3030 203d  :.        ix00 =
-0000e940: 2069 7830 202d 206e 5f74 6170 6572 0a0a   ix0 - n_taper..
-0000e950: 2020 2020 7370 6563 5f6f 7574 203d 2073      spec_out = s
-0000e960: 7065 632e 636f 7079 2829 0a20 2020 2073  pec.copy().    s
-0000e970: 7065 635f 6f75 745b 303a 6978 3030 5d20  pec_out[0:ix00] 
-0000e980: 3d20 302e 3020 2b20 302e 306a 0a20 2020  = 0.0 + 0.0j.   
-0000e990: 2073 7065 635f 6f75 745b 6978 3131 3a5d   spec_out[ix11:]
-0000e9a0: 203d 2030 2e30 202b 2030 2e30 6a0a 0a20   = 0.0 + 0.0j.. 
-0000e9b0: 2020 2069 6620 736d 6f6f 7468 5f4e 203c     if smooth_N <
-0000e9c0: 3d20 313a 0a20 2020 2020 2020 2073 7065  = 1:.        spe
-0000e9d0: 635f 6f75 745b 6978 3030 3a69 7831 315d  c_out[ix00:ix11]
-0000e9e0: 203d 206e 702e 6578 7028 312e 306a 202a   = np.exp(1.0j *
-0000e9f0: 206e 702e 616e 676c 6528 7370 6563 5f6f   np.angle(spec_o
-0000ea00: 7574 5b69 7830 303a 6978 3131 5d29 290a  ut[ix00:ix11])).
-0000ea10: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000ea20: 2020 7370 6563 5f6f 7574 5b69 7830 303a    spec_out[ix00:
-0000ea30: 6978 3131 5d20 2f3d 206d 6f76 696e 675f  ix11] /= moving_
-0000ea40: 6176 6528 6e70 2e61 6273 2873 7065 635f  ave(np.abs(spec_
-0000ea50: 6f75 745b 6978 3030 3a69 7831 315d 292c  out[ix00:ix11]),
-0000ea60: 2073 6d6f 6f74 685f 4e29 0a0a 2020 2020   smooth_N)..    
-0000ea70: 7820 3d20 6e70 2e6c 696e 7370 6163 6528  x = np.linspace(
-0000ea80: 6e70 2e70 6920 2f20 322e 302c 206e 702e  np.pi / 2.0, np.
-0000ea90: 7069 2c20 6978 3020 2d20 6978 3030 290a  pi, ix0 - ix00).
-0000eaa0: 2020 2020 7370 6563 5f6f 7574 5b69 7830      spec_out[ix0
-0000eab0: 303a 6978 305d 202a 3d20 6e70 2e63 6f73  0:ix0] *= np.cos
-0000eac0: 2878 2920 2a2a 2032 0a0a 2020 2020 7820  (x) ** 2..    x 
-0000ead0: 3d20 6e70 2e6c 696e 7370 6163 6528 302e  = np.linspace(0.
-0000eae0: 302c 206e 702e 7069 202f 2032 2e30 2c20  0, np.pi / 2.0, 
-0000eaf0: 6978 3131 202d 2069 7831 290a 2020 2020  ix11 - ix1).    
-0000eb00: 7370 6563 5f6f 7574 5b69 7831 3a69 7831  spec_out[ix1:ix1
-0000eb10: 315d 202a 3d20 6e70 2e63 6f73 2878 2920  1] *= np.cos(x) 
-0000eb20: 2a2a 2032 0a0a 2020 2020 7265 7475 726e  ** 2..    return
-0000eb30: 2073 7065 635f 6f75 740a 0a0a 6465 6620   spec_out...def 
-0000eb40: 7768 6974 656e 5f32 4428 7469 6d65 7365  whiten_2D(timese
-0000eb50: 7269 6573 2c20 6666 745f 7061 7261 2c20  ries, fft_para, 
-0000eb60: 6e5f 7461 7065 7229 3a0a 2020 2020 2222  n_taper):.    ""
-0000eb70: 220a 2020 2020 5468 6973 2066 756e 6374  ".    This funct
-0000eb80: 696f 6e20 7461 6b65 7320 6120 322d 6469  ion takes a 2-di
-0000eb90: 6d65 6e73 696f 6e61 6c20 7469 6d65 7365  mensional timese
-0000eba0: 7269 6573 2061 7272 6179 2c20 7472 616e  ries array, tran
-0000ebb0: 7366 6f72 6d73 2074 6f20 6672 6571 7565  sforms to freque
-0000ebc0: 6e63 7920 646f 6d61 696e 2075 7369 6e67  ncy domain using
-0000ebd0: 2066 6674 2c0a 2020 2020 7768 6974 656e   fft,.    whiten
-0000ebe0: 7320 7468 6520 616d 706c 6974 7564 6520  s the amplitude 
-0000ebf0: 6f66 2074 6865 2073 7065 6374 7275 6d20  of the spectrum 
-0000ec00: 696e 2066 7265 7175 656e 6379 2064 6f6d  in frequency dom
-0000ec10: 6169 6e20 6265 7477 6565 6e20 2a66 7265  ain between *fre
-0000ec20: 716d 696e 2a20 616e 6420 2a66 7265 716d  qmin* and *freqm
-0000ec30: 6178 2a0a 2020 2020 616e 6420 7265 7475  ax*.    and retu
-0000ec40: 726e 7320 7468 6520 7768 6974 656e 6564  rns the whitened
-0000ec50: 2066 6674 2e0a 2020 2020 5041 5241 4d45   fft..    PARAME
-0000ec60: 5445 5253 3a0a 2020 2020 2d2d 2d2d 2d2d  TERS:.    ------
-0000ec70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000ec80: 0a20 2020 2064 6174 613a 206e 756d 7079  .    data: numpy
-0000ec90: 2e6e 6461 7272 6179 2063 6f6e 7461 696e  .ndarray contain
-0000eca0: 7320 7468 6520 3144 2074 696d 6520 7365  s the 1D time se
-0000ecb0: 7269 6573 2074 6f20 7768 6974 656e 0a20  ries to whiten. 
-0000ecc0: 2020 2066 6674 5f70 6172 613a 2064 6963     fft_para: dic
-0000ecd0: 7420 636f 6e74 6169 6e69 6e67 2061 6c6c  t containing all
-0000ece0: 2066 6674 5f63 6320 7061 7261 6d65 7465   fft_cc paramete
-0000ecf0: 7273 2073 7563 6820 6173 0a20 2020 2020  rs such as.     
-0000ed00: 2020 2064 743a 2054 6865 2073 616d 706c     dt: The sampl
-0000ed10: 696e 6720 7370 6163 6520 6f66 2074 6865  ing space of the
-0000ed20: 2060 6461 7461 600a 2020 2020 2020 2020   `data`.        
-0000ed30: 6672 6571 6d69 6e3a 2054 6865 206c 6f77  freqmin: The low
-0000ed40: 6572 2066 7265 7175 656e 6379 2062 6f75  er frequency bou
-0000ed50: 6e64 0a20 2020 2020 2020 2066 7265 716d  nd.        freqm
-0000ed60: 6178 3a20 5468 6520 7570 7065 7220 6672  ax: The upper fr
-0000ed70: 6571 7565 6e63 7920 626f 756e 640a 2020  equency bound.  
-0000ed80: 2020 2020 2020 736d 6f6f 7468 5f4e 3a20        smooth_N: 
-0000ed90: 696e 7465 6765 722c 2069 7420 6465 6669  integer, it defi
-0000eda0: 6e65 7320 7468 6520 6861 6c66 2077 696e  nes the half win
-0000edb0: 646f 7720 6c65 6e67 7468 2074 6f20 736d  dow length to sm
-0000edc0: 6f6f 7468 0a20 2020 2020 2020 206e 5f74  ooth.        n_t
-0000edd0: 6170 6572 2c20 6f70 7469 6f6e 616c 3a20  aper, optional: 
-0000ede0: 696e 7465 6765 722c 2064 6566 696e 6520  integer, define 
-0000edf0: 7468 6520 7769 6474 6820 6f66 2074 6865  the width of the
-0000ee00: 2074 6170 6572 2069 6e20 7361 6d70 6c65   taper in sample
-0000ee10: 730a 2020 2020 5245 5455 524e 533a 0a20  s.    RETURNS:. 
-0000ee20: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
-0000ee30: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 4646  ---------.    FF
-0000ee40: 5452 6177 5369 676e 3a20 6e75 6d70 792e  TRawSign: numpy.
-0000ee50: 6e64 6172 7261 7920 636f 6e74 6169 6e73  ndarray contains
-0000ee60: 2074 6865 2046 4654 206f 6620 7468 6520   the FFT of the 
-0000ee70: 7768 6974 656e 6564 2069 6e70 7574 2074  whitened input t
-0000ee80: 7261 6365 2062 6574 7765 656e 2074 6865  race between the
-0000ee90: 2066 7265 7175 656e 6379 2062 6f75 6e64   frequency bound
-0000eea0: 730a 2020 2020 2222 220a 2020 2020 2320  s.    """.    # 
-0000eeb0: 6c6f 6164 2070 6172 616d 6574 6572 730a  load parameters.
-0000eec0: 2020 2020 6465 6c74 6120 3d20 6666 745f      delta = fft_
-0000eed0: 7061 7261 5b22 6474 225d 0a20 2020 2066  para["dt"].    f
-0000eee0: 7265 716d 696e 203d 2066 6674 5f70 6172  reqmin = fft_par
-0000eef0: 615b 2266 7265 716d 696e 225d 0a20 2020  a["freqmin"].   
-0000ef00: 2066 7265 716d 6178 203d 2066 6674 5f70   freqmax = fft_p
-0000ef10: 6172 615b 2266 7265 716d 6178 225d 0a20  ara["freqmax"]. 
-0000ef20: 2020 2073 6d6f 6f74 685f 4e20 3d20 6666     smooth_N = ff
-0000ef30: 745f 7061 7261 5b22 736d 6f6f 7468 5f4e  t_para["smooth_N
-0000ef40: 225d 0a0a 2020 2020 6e66 6674 203d 206e  "]..    nfft = n
-0000ef50: 6578 745f 6661 7374 5f6c 656e 2874 696d  ext_fast_len(tim
-0000ef60: 6573 6572 6965 732e 7368 6170 655b 315d  eseries.shape[1]
-0000ef70: 290a 2020 2020 7370 6563 203d 206e 702e  ).    spec = np.
-0000ef80: 6666 742e 6666 746e 2874 696d 6573 6572  fft.fftn(timeser
-0000ef90: 6965 732c 2073 3d5b 6e66 6674 5d29 0a20  ies, s=[nfft]). 
-0000efa0: 2020 2066 7265 7120 3d20 6e70 2e66 6674     freq = np.fft
-0000efb0: 2e66 6674 6672 6571 286e 6666 742c 2064  .fftfreq(nfft, d
-0000efc0: 3d64 656c 7461 290a 0a20 2020 2069 7830  =delta)..    ix0
-0000efd0: 203d 206e 702e 6172 676d 696e 286e 702e   = np.argmin(np.
-0000efe0: 6162 7328 6672 6571 202d 2066 7265 716d  abs(freq - freqm
-0000eff0: 696e 2929 0a20 2020 2069 7831 203d 206e  in)).    ix1 = n
-0000f000: 702e 6172 676d 696e 286e 702e 6162 7328  p.argmin(np.abs(
-0000f010: 6672 6571 202d 2066 7265 716d 6178 2929  freq - freqmax))
-0000f020: 0a0a 2020 2020 6966 2069 7831 202b 206e  ..    if ix1 + n
-0000f030: 5f74 6170 6572 203e 206e 6666 743a 0a20  _taper > nfft:. 
-0000f040: 2020 2020 2020 2069 7831 3120 3d20 6e66         ix11 = nf
-0000f050: 6674 0a20 2020 2065 6c73 653a 0a20 2020  ft.    else:.   
-0000f060: 2020 2020 2069 7831 3120 3d20 6978 3120       ix11 = ix1 
-0000f070: 2b20 6e5f 7461 7065 720a 0a20 2020 2069  + n_taper..    i
-0000f080: 6620 6978 3020 2d20 6e5f 7461 7065 7220  f ix0 - n_taper 
-0000f090: 3c20 303a 0a20 2020 2020 2020 2069 7830  < 0:.        ix0
-0000f0a0: 3020 3d20 300a 2020 2020 656c 7365 3a0a  0 = 0.    else:.
-0000f0b0: 2020 2020 2020 2020 6978 3030 203d 2069          ix00 = i
-0000f0c0: 7830 202d 206e 5f74 6170 6572 0a0a 2020  x0 - n_taper..  
-0000f0d0: 2020 7370 6563 5f6f 7574 203d 2073 7065    spec_out = spe
-0000f0e0: 632e 636f 7079 2829 2020 2320 6d61 7920  c.copy()  # may 
-0000f0f0: 6265 2069 6e63 6f6e 7665 6e69 656e 7420  be inconvenient 
-0000f100: 6475 6520 746f 2068 6967 6865 7220 6d65  due to higher me
-0000f110: 6d6f 7279 2075 7361 6765 0a20 2020 2073  mory usage.    s
-0000f120: 7065 635f 6f75 745b 3a2c 2030 3a69 7830  pec_out[:, 0:ix0
-0000f130: 305d 203d 2030 2e30 202b 2030 2e30 6a0a  0] = 0.0 + 0.0j.
-0000f140: 2020 2020 7370 6563 5f6f 7574 5b3a 2c20      spec_out[:, 
-0000f150: 6978 3131 3a5d 203d 2030 2e30 202b 2030  ix11:] = 0.0 + 0
-0000f160: 2e30 6a0a 0a20 2020 2069 6620 736d 6f6f  .0j..    if smoo
-0000f170: 7468 5f4e 203c 3d20 313a 0a20 2020 2020  th_N <= 1:.     
-0000f180: 2020 2073 7065 635f 6f75 745b 3a2c 2069     spec_out[:, i
-0000f190: 7830 303a 6978 3131 5d20 3d20 6e70 2e65  x00:ix11] = np.e
-0000f1a0: 7870 2831 2e30 6a20 2a20 6e70 2e61 6e67  xp(1.0j * np.ang
-0000f1b0: 6c65 2873 7065 635f 6f75 745b 3a2c 2069  le(spec_out[:, i
-0000f1c0: 7830 303a 6978 3131 5d29 290a 2020 2020  x00:ix11])).    
-0000f1d0: 656c 7365 3a0a 2020 2020 2020 2020 7370  else:.        sp
-0000f1e0: 6563 5f6f 7574 5b3a 2c20 6978 3030 3a69  ec_out[:, ix00:i
-0000f1f0: 7831 315d 202f 3d20 6d6f 7669 6e67 5f61  x11] /= moving_a
-0000f200: 7665 5f32 4428 6e70 2e61 6273 2873 7065  ve_2D(np.abs(spe
-0000f210: 635f 6f75 745b 3a2c 2069 7830 303a 6978  c_out[:, ix00:ix
-0000f220: 3131 5d29 2c20 736d 6f6f 7468 5f4e 290a  11]), smooth_N).
-0000f230: 0a20 2020 2078 203d 206e 702e 6c69 6e73  .    x = np.lins
-0000f240: 7061 6365 286e 702e 7069 202f 2032 2e30  pace(np.pi / 2.0
-0000f250: 2c20 6e70 2e70 692c 2069 7830 202d 2069  , np.pi, ix0 - i
-0000f260: 7830 3029 0a20 2020 2073 7065 635f 6f75  x00).    spec_ou
-0000f270: 745b 3a2c 2069 7830 303a 6978 305d 202a  t[:, ix00:ix0] *
-0000f280: 3d20 6e70 2e63 6f73 2878 2920 2a2a 2032  = np.cos(x) ** 2
-0000f290: 0a0a 2020 2020 7820 3d20 6e70 2e6c 696e  ..    x = np.lin
-0000f2a0: 7370 6163 6528 302e 302c 206e 702e 7069  space(0.0, np.pi
-0000f2b0: 202f 2032 2e30 2c20 6978 3131 202d 2069   / 2.0, ix11 - i
-0000f2c0: 7831 290a 2020 2020 7370 6563 5f6f 7574  x1).    spec_out
-0000f2d0: 5b3a 2c20 6978 313a 6978 3131 5d20 2a3d  [:, ix1:ix11] *=
-0000f2e0: 206e 702e 636f 7328 7829 202a 2a20 320a   np.cos(x) ** 2.
-0000f2f0: 0a20 2020 2072 6574 7572 6e20 7370 6563  .    return spec
-0000f300: 5f6f 7574 0a0a 0a64 6566 2077 6869 7465  _out...def white
-0000f310: 6e28 6461 7461 2c20 6666 745f 7061 7261  n(data, fft_para
-0000f320: 2c20 6e5f 7461 7065 723d 3130 3029 3a0a  , n_taper=100):.
-0000f330: 2020 2020 2222 220a 2020 2020 5468 6973      """.    This
-0000f340: 2066 756e 6374 696f 6e20 7461 6b65 7320   function takes 
-0000f350: 6120 7469 6d65 7365 7269 6573 2061 7272  a timeseries arr
-0000f360: 6179 2c20 7472 616e 7366 6f72 6d73 2074  ay, transforms t
-0000f370: 6f20 6672 6571 7565 6e63 7920 646f 6d61  o frequency doma
-0000f380: 696e 2075 7369 6e67 2066 6674 2c0a 2020  in using fft,.  
-0000f390: 2020 7768 6974 656e 7320 7468 6520 616d    whitens the am
-0000f3a0: 706c 6974 7564 6520 6f66 2074 6865 2073  plitude of the s
-0000f3b0: 7065 6374 7275 6d20 696e 2066 7265 7175  pectrum in frequ
-0000f3c0: 656e 6379 2064 6f6d 6169 6e20 6265 7477  ency domain betw
-0000f3d0: 6565 6e20 2a66 7265 716d 696e 2a20 616e  een *freqmin* an
-0000f3e0: 6420 2a66 7265 716d 6178 2a0a 2020 2020  d *freqmax*.    
-0000f3f0: 616e 6420 7265 7475 726e 7320 7468 6520  and returns the 
-0000f400: 7768 6974 656e 6564 2066 6674 2e0a 2020  whitened fft..  
-0000f410: 2020 5041 5241 4d45 5445 5253 3a0a 2020    PARAMETERS:.  
-0000f420: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
-0000f430: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 6174  --------.    dat
-0000f440: 613a 206e 756d 7079 2e6e 6461 7272 6179  a: numpy.ndarray
-0000f450: 2063 6f6e 7461 696e 7320 7468 6520 3144   contains the 1D
-0000f460: 2074 696d 6520 7365 7269 6573 2074 6f20   time series to 
-0000f470: 7768 6974 656e 0a20 2020 2066 6674 5f70  whiten.    fft_p
-0000f480: 6172 613a 2064 6963 7420 636f 6e74 6169  ara: dict contai
-0000f490: 6e69 6e67 2061 6c6c 2066 6674 5f63 6320  ning all fft_cc 
-0000f4a0: 7061 7261 6d65 7465 7273 2073 7563 6820  parameters such 
-0000f4b0: 6173 0a20 2020 2020 2020 2064 743a 2054  as.        dt: T
-0000f4c0: 6865 2073 616d 706c 696e 6720 7370 6163  he sampling spac
-0000f4d0: 6520 6f66 2074 6865 2060 6461 7461 600a  e of the `data`.
-0000f4e0: 2020 2020 2020 2020 6672 6571 6d69 6e3a          freqmin:
-0000f4f0: 2054 6865 206c 6f77 6572 2066 7265 7175   The lower frequ
-0000f500: 656e 6379 2062 6f75 6e64 0a20 2020 2020  ency bound.     
-0000f510: 2020 2066 7265 716d 6178 3a20 5468 6520     freqmax: The 
-0000f520: 7570 7065 7220 6672 6571 7565 6e63 7920  upper frequency 
-0000f530: 626f 756e 640a 2020 2020 2020 2020 736d  bound.        sm
-0000f540: 6f6f 7468 5f4e 3a20 696e 7465 6765 722c  ooth_N: integer,
-0000f550: 2069 7420 6465 6669 6e65 7320 7468 6520   it defines the 
-0000f560: 6861 6c66 2077 696e 646f 7720 6c65 6e67  half window leng
-0000f570: 7468 2074 6f20 736d 6f6f 7468 0a20 2020  th to smooth.   
-0000f580: 2020 2020 2066 7265 715f 6e6f 726d 3a20       freq_norm: 
-0000f590: 7768 6974 656e 696e 6720 6d65 7468 6f64  whitening method
-0000f5a0: 2062 6574 7765 656e 2027 6f6e 652d 6269   between 'one-bi
-0000f5b0: 7427 2061 6e64 2027 524d 4127 0a20 2020  t' and 'RMA'.   
-0000f5c0: 2052 4554 5552 4e53 3a0a 2020 2020 2d2d   RETURNS:.    --
-0000f5d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000f5e0: 2d2d 2d2d 0a20 2020 2046 4654 5261 7753  ----.    FFTRawS
-0000f5f0: 6967 6e3a 206e 756d 7079 2e6e 6461 7272  ign: numpy.ndarr
-0000f600: 6179 2063 6f6e 7461 696e 7320 7468 6520  ay contains the 
-0000f610: 4646 5420 6f66 2074 6865 2077 6869 7465  FFT of the white
-0000f620: 6e65 6420 696e 7075 7420 7472 6163 6520  ned input trace 
-0000f630: 6265 7477 6565 6e20 7468 6520 6672 6571  between the freq
-0000f640: 7565 6e63 7920 626f 756e 6473 0a20 2020  uency bounds.   
-0000f650: 2022 2222 0a0a 2020 2020 2320 5370 6565   """..    # Spee
-0000f660: 6420 7570 2046 4654 2062 7920 7061 6464  d up FFT by padd
-0000f670: 696e 6720 746f 206f 7074 696d 616c 2073  ing to optimal s
-0000f680: 697a 6520 666f 7220 4646 5450 4143 4b0a  ize for FFTPACK.
-0000f690: 2020 2020 6966 2064 6174 612e 6e64 696d      if data.ndim
-0000f6a0: 203d 3d20 313a 0a20 2020 2020 2020 2046   == 1:.        F
-0000f6b0: 4654 5261 7753 6967 6e20 3d20 7768 6974  FTRawSign = whit
-0000f6c0: 656e 5f31 4428 6461 7461 2c20 6666 745f  en_1D(data, fft_
-0000f6d0: 7061 7261 2c20 6e5f 7461 7065 7229 0a20  para, n_taper). 
-0000f6e0: 2020 2020 2020 2023 2041 5252 5f4f 5554         # ARR_OUT
-0000f6f0: 3a20 4f6e 6c79 2066 6f72 2063 6f6e 7369  : Only for consi
-0000f700: 7374 656e 6379 2077 6974 6820 6e6f 6973  stency with nois
-0000f710: 6570 7920 6170 7072 6f61 6368 206f 6620  epy approach of 
-0000f720: 686f 6c64 696e 6720 7468 6520 6675 6c6c  holding the full
-0000f730: 0a20 2020 2020 2020 2023 2073 7065 6374  .        # spect
-0000f740: 7275 6d20 286e 6f74 206a 7573 7420 3020  rum (not just 0 
-0000f750: 616e 6420 706f 7369 7469 7665 2066 7265  and positive fre
-0000f760: 712e 2070 6172 7429 0a20 2020 2020 2020  q. part).       
-0000f770: 2061 7272 5f6f 7574 203d 206e 702e 7a65   arr_out = np.ze
-0000f780: 726f 7328 2846 4654 5261 7753 6967 6e2e  ros((FFTRawSign.
-0000f790: 7368 6170 655b 305d 202d 2031 2920 2a20  shape[0] - 1) * 
-0000f7a0: 3220 2b20 312c 2064 7479 7065 3d63 6f6d  2 + 1, dtype=com
-0000f7b0: 706c 6578 290a 2020 2020 2020 2020 6172  plex).        ar
-0000f7c0: 725f 6f75 745b 3020 3a20 4646 5452 6177  r_out[0 : FFTRaw
-0000f7d0: 5369 676e 2e73 6861 7065 5b30 5d5d 203d  Sign.shape[0]] =
-0000f7e0: 2046 4654 5261 7753 6967 6e0a 2020 2020   FFTRawSign.    
-0000f7f0: 2020 2020 6172 725f 6f75 745b 4646 5452      arr_out[FFTR
-0000f800: 6177 5369 676e 2e73 6861 7065 5b30 5d20  awSign.shape[0] 
-0000f810: 3a5d 203d 2046 4654 5261 7753 6967 6e5b  :] = FFTRawSign[
-0000f820: 313a 5d2e 636f 6e6a 7567 6174 6528 295b  1:].conjugate()[
-0000f830: 3a3a 2d31 5d0a 0a20 2020 2065 6c69 6620  ::-1]..    elif 
-0000f840: 6461 7461 2e6e 6469 6d20 3d3d 2032 3a0a  data.ndim == 2:.
-0000f850: 2020 2020 2020 2020 4646 5452 6177 5369          FFTRawSi
-0000f860: 676e 203d 2077 6869 7465 6e5f 3244 2864  gn = whiten_2D(d
-0000f870: 6174 612c 2066 6674 5f70 6172 612c 206e  ata, fft_para, n
-0000f880: 5f74 6170 6572 290a 2020 2020 2020 2020  _taper).        
-0000f890: 6172 725f 6f75 7420 3d20 6e70 2e7a 6572  arr_out = np.zer
-0000f8a0: 6f73 2828 4646 5452 6177 5369 676e 2e73  os((FFTRawSign.s
-0000f8b0: 6861 7065 5b30 5d2c 2028 4646 5452 6177  hape[0], (FFTRaw
-0000f8c0: 5369 676e 2e73 6861 7065 5b31 5d20 2d20  Sign.shape[1] - 
-0000f8d0: 3129 202a 2032 202b 2031 292c 2064 7479  1) * 2 + 1), dty
-0000f8e0: 7065 3d63 6f6d 706c 6578 290a 2020 2020  pe=complex).    
-0000f8f0: 2020 2020 6172 725f 6f75 745b 3a2c 2046      arr_out[:, F
-0000f900: 4654 5261 7753 6967 6e2e 7368 6170 655b  FTRawSign.shape[
-0000f910: 315d 203a 5d20 3d20 4646 5452 6177 5369  1] :] = FFTRawSi
-0000f920: 676e 5b3a 2c20 313a 5d2e 636f 6e6a 7567  gn[:, 1:].conjug
-0000f930: 6174 6528 295b 3a3a 2d31 5d0a 2020 2020  ate()[::-1].    
-0000f940: 7265 7475 726e 2046 4654 5261 7753 6967  return FFTRawSig
-0000f950: 6e0a 0a0a 6465 6620 6164 6170 7469 7665  n...def adaptive
-0000f960: 5f66 696c 7465 7228 6172 722c 2067 293a  _filter(arr, g):
-0000f970: 0a20 2020 2022 2222 0a20 2020 2074 6865  .    """.    the
-0000f980: 2061 6461 7074 6976 6520 636f 7661 7269   adaptive covari
-0000f990: 616e 6365 2066 696c 7465 7220 746f 2065  ance filter to e
-0000f9a0: 6e68 616e 6365 2063 6f68 6572 656e 7420  nhance coherent 
-0000f9b0: 7369 676e 616c 732e 2046 656c 6c6f 7773  signals. Fellows
-0000f9c0: 2074 6865 206d 6574 686f 6420 6f66 0a20   the method of. 
-0000f9d0: 2020 204e 616b 6174 6120 6574 2061 6c2e     Nakata et al.
-0000f9e0: 2c20 3230 3135 2028 4170 7065 6e64 6978  , 2015 (Appendix
-0000f9f0: 2042 290a 0a20 2020 2074 6865 2066 696c   B)..    the fil
-0000fa00: 7465 7265 6420 7369 676e 616c 205b 7831  tered signal [x1
-0000fa10: 5d20 6973 2067 6976 656e 2062 7920 7831  ] is given by x1
-0000fa20: 203d 2069 6666 7428 502a 7831 2877 2929   = ifft(P*x1(w))
-0000fa30: 2077 6865 7265 2078 3120 6973 2074 6865   where x1 is the
-0000fa40: 2066 6674 6564 2073 7065 6374 7261 0a20   ffted spectra. 
-0000fa50: 2020 2061 6e64 2050 2069 7320 7468 6520     and P is the 
-0000fa60: 6669 6c74 6572 2e20 5020 6973 2063 6f6e  filter. P is con
-0000fa70: 7374 7275 6374 6564 2062 7920 7573 696e  structed by usin
-0000fa80: 6720 7468 6520 7465 6d70 6f72 616c 2063  g the temporal c
-0000fa90: 6f76 6172 6961 6e63 6520 6d61 7472 6978  ovariance matrix
-0000faa0: 2e0a 0a20 2020 2050 4152 414d 4554 4552  ...    PARAMETER
-0000fab0: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
-0000fac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-0000fad0: 2020 6172 723a 206e 756d 7079 2e6e 6461    arr: numpy.nda
-0000fae0: 7272 6179 2063 6f6e 7461 696e 7320 7468  rray contains th
-0000faf0: 6520 3244 2074 7261 6365 7320 6f66 2064  e 2D traces of d
-0000fb00: 6169 6c79 2f68 6f75 726c 7920 6372 6f73  aily/hourly cros
-0000fb10: 732d 636f 7272 656c 6174 696f 6e20 6675  s-correlation fu
-0000fb20: 6e63 7469 6f6e 730a 2020 2020 673a 2061  nctions.    g: a
-0000fb30: 2070 6f73 6974 6976 6520 6e75 6d62 6572   positive number
-0000fb40: 2074 6f20 6164 6a75 7374 2074 6865 2066   to adjust the f
-0000fb50: 696c 7465 7220 6861 7273 686e 6573 730a  ilter harshness.
-0000fb60: 2020 2020 5245 5455 524e 533a 0a20 2020      RETURNS:.   
-0000fb70: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-0000fb80: 2d2d 2d2d 2d2d 2d0a 2020 2020 6e61 7272  -------.    narr
-0000fb90: 3a20 6e75 6d70 7920 7665 6374 6f72 2063  : numpy vector c
-0000fba0: 6f6e 7461 696e 7320 7468 6520 7374 6163  ontains the stac
-0000fbb0: 6b65 6420 6372 6f73 7320 636f 7272 656c  ked cross correl
-0000fbc0: 6174 696f 6e20 6675 6e63 7469 6f6e 0a20  ation function. 
-0000fbd0: 2020 2022 2222 0a20 2020 2069 6620 6172     """.    if ar
-0000fbe0: 722e 6e64 696d 203d 3d20 313a 0a20 2020  r.ndim == 1:.   
-0000fbf0: 2020 2020 2072 6574 7572 6e20 6172 720a       return arr.
-0000fc00: 2020 2020 4e2c 204d 203d 2061 7272 2e73      N, M = arr.s
-0000fc10: 6861 7065 0a20 2020 204e 6666 7420 3d20  hape.    Nfft = 
-0000fc20: 6e65 7874 5f66 6173 745f 6c65 6e28 4d29  next_fast_len(M)
-0000fc30: 0a0a 2020 2020 2320 6666 7420 7468 6520  ..    # fft the 
-0000fc40: 3244 2061 7272 6179 0a20 2020 2073 7065  2D array.    spe
-0000fc50: 6320 3d20 7363 6970 792e 6666 7470 6163  c = scipy.fftpac
-0000fc60: 6b2e 6666 7428 6172 722c 2061 7869 733d  k.fft(arr, axis=
-0000fc70: 312c 206e 3d4e 6666 7429 5b3a 2c20 3a4d  1, n=Nfft)[:, :M
-0000fc80: 5d0a 0a20 2020 2023 206d 616b 6520 6372  ]..    # make cr
-0000fc90: 6f73 732d 7370 6563 7472 6d20 6d61 7472  oss-spectrm matr
-0000fca0: 6978 0a20 2020 2063 7370 6563 203d 206e  ix.    cspec = n
-0000fcb0: 702e 7a65 726f 7328 7368 6170 653d 284e  p.zeros(shape=(N
-0000fcc0: 202a 204e 2c20 4d29 2c20 6474 7970 653d   * N, M), dtype=
-0000fcd0: 6e70 2e63 6f6d 706c 6578 3634 290a 2020  np.complex64).  
-0000fce0: 2020 666f 7220 6969 2069 6e20 7261 6e67    for ii in rang
-0000fcf0: 6528 4e29 3a0a 2020 2020 2020 2020 666f  e(N):.        fo
-0000fd00: 7220 6a6a 2069 6e20 7261 6e67 6528 4e29  r jj in range(N)
-0000fd10: 3a0a 2020 2020 2020 2020 2020 2020 6b6b  :.            kk
-0000fd20: 203d 2069 6920 2a20 4e20 2b20 6a6a 0a20   = ii * N + jj. 
-0000fd30: 2020 2020 2020 2020 2020 2063 7370 6563             cspec
-0000fd40: 5b6b 6b5d 203d 2073 7065 635b 6969 5d20  [kk] = spec[ii] 
-0000fd50: 2a20 6e70 2e63 6f6e 6a75 6761 7465 2873  * np.conjugate(s
-0000fd60: 7065 635b 6a6a 5d29 0a0a 2020 2020 5331  pec[jj])..    S1
-0000fd70: 203d 206e 702e 7a65 726f 7328 4d2c 2064   = np.zeros(M, d
-0000fd80: 7479 7065 3d6e 702e 636f 6d70 6c65 7836  type=np.complex6
-0000fd90: 3429 0a20 2020 2053 3220 3d20 6e70 2e7a  4).    S2 = np.z
-0000fda0: 6572 6f73 284d 2c20 6474 7970 653d 6e70  eros(M, dtype=np
-0000fdb0: 2e63 6f6d 706c 6578 3634 290a 2020 2020  .complex64).    
-0000fdc0: 2320 636f 6e73 7472 7563 7420 7468 6520  # construct the 
-0000fdd0: 6669 6c74 6572 2050 0a20 2020 2066 6f72  filter P.    for
-0000fde0: 2069 6920 696e 2072 616e 6765 284e 293a   ii in range(N):
-0000fdf0: 0a20 2020 2020 2020 206d 6d20 3d20 6969  .        mm = ii
-0000fe00: 202a 204e 202b 2069 690a 2020 2020 2020   * N + ii.      
-0000fe10: 2020 5332 202b 3d20 6373 7065 635b 6d6d    S2 += cspec[mm
-0000fe20: 5d0a 2020 2020 2020 2020 666f 7220 6a6a  ].        for jj
-0000fe30: 2069 6e20 7261 6e67 6528 4e29 3a0a 2020   in range(N):.  
-0000fe40: 2020 2020 2020 2020 2020 6b6b 203d 2069            kk = i
-0000fe50: 6920 2a20 4e20 2b20 6a6a 0a20 2020 2020  i * N + jj.     
-0000fe60: 2020 2020 2020 2053 3120 2b3d 2063 7370         S1 += csp
-0000fe70: 6563 5b6b 6b5d 0a0a 2020 2020 7020 3d20  ec[kk]..    p = 
-0000fe80: 6e70 2e70 6f77 6572 2828 5331 202d 2053  np.power((S1 - S
-0000fe90: 3229 202f 2028 5332 202a 2028 4e20 2d20  2) / (S2 * (N - 
-0000fea0: 3129 292c 2067 290a 0a20 2020 2023 206d  1)), g)..    # m
-0000feb0: 616b 6520 6966 6674 0a20 2020 206e 6172  ake ifft.    nar
-0000fec0: 7220 3d20 6e70 2e72 6561 6c28 7363 6970  r = np.real(scip
-0000fed0: 792e 6666 7470 6163 6b2e 6966 6674 286e  y.fftpack.ifft(n
-0000fee0: 702e 6d75 6c74 6970 6c79 2870 2c20 7370  p.multiply(p, sp
-0000fef0: 6563 292c 204e 6666 742c 2061 7869 733d  ec), Nfft, axis=
-0000ff00: 3129 5b3a 2c20 3a4d 5d29 0a20 2020 2072  1)[:, :M]).    r
-0000ff10: 6574 7572 6e20 6e70 2e6d 6561 6e28 6e61  eturn np.mean(na
-0000ff20: 7272 2c20 6178 6973 3d30 290a 0a0a 6465  rr, axis=0)...de
-0000ff30: 6620 7077 7328 6172 722c 2073 616d 706c  f pws(arr, sampl
-0000ff40: 696e 675f 7261 7465 2c20 706f 7765 723d  ing_rate, power=
-0000ff50: 322c 2070 7773 5f74 696d 6567 6174 653d  2, pws_timegate=
-0000ff60: 352e 3029 3a0a 2020 2020 2222 220a 2020  5.0):.    """.  
-0000ff70: 2020 5065 7266 6f72 6d73 2070 6861 7365    Performs phase
-0000ff80: 2d77 6569 6768 7465 6420 7374 6163 6b20  -weighted stack 
-0000ff90: 6f6e 2061 7272 6179 206f 6620 7469 6d65  on array of time
-0000ffa0: 2073 6572 6965 732e 204d 6f64 6966 6965   series. Modifie
-0000ffb0: 6420 6f6e 2074 6865 206e 6f69 7365 2066  d on the noise f
-0000ffc0: 756e 6374 696f 6e20 6279 2054 696d 2043  unction by Tim C
-0000ffd0: 6c69 6d65 6e74 732e 0a20 2020 2046 6f6c  liments..    Fol
-0000ffe0: 6c6f 7773 206d 6574 686f 6473 206f 6620  lows methods of 
-0000fff0: 5363 6869 6d6d 656c 2061 6e64 2050 6175  Schimmel and Pau
-00010000: 6c73 7365 6e2c 2031 3939 372e 0a20 2020  lssen, 1997..   
-00010010: 2049 6620 7328 7429 2069 7320 7469 6d65   If s(t) is time
-00010020: 2073 6572 6965 7320 6461 7461 2028 7365   series data (se
-00010030: 6973 6d6f 6772 616d 2c20 6f72 2063 726f  ismogram, or cro
-00010040: 7373 2d63 6f72 7265 6c61 7469 6f6e 292c  ss-correlation),
-00010050: 0a20 2020 2053 2874 2920 3d20 7328 7429  .    S(t) = s(t)
-00010060: 202b 2069 2a48 2873 2874 2929 2c20 7768   + i*H(s(t)), wh
-00010070: 6572 6520 4828 7328 7429 2920 6973 2048  ere H(s(t)) is H
-00010080: 696c 6265 7274 2074 7261 6e73 666f 726d  ilbert transform
-00010090: 206f 6620 7328 7429 0a20 2020 2053 2874   of s(t).    S(t
-000100a0: 2920 3d20 7328 7429 202b 2069 2a48 2873  ) = s(t) + i*H(s
-000100b0: 2874 2929 203d 2041 2874 292a 6578 7028  (t)) = A(t)*exp(
-000100c0: 692a 7068 6928 7429 292c 2077 6865 7265  i*phi(t)), where
-000100d0: 0a20 2020 2041 2874 2920 6973 2065 6e76  .    A(t) is env
-000100e0: 656c 6f70 6520 6f66 2073 2874 2920 616e  elope of s(t) an
-000100f0: 6420 7068 6928 7429 2069 7320 7068 6173  d phi(t) is phas
-00010100: 6520 6f66 2073 2874 290a 2020 2020 5068  e of s(t).    Ph
-00010110: 6173 652d 7765 6967 6874 6564 2073 7461  ase-weighted sta
-00010120: 636b 2c20 6728 7429 2c20 6973 2074 6865  ck, g(t), is the
-00010130: 6e3a 0a20 2020 2067 2874 2920 3d20 312f  n:.    g(t) = 1/
-00010140: 4e20 7375 6d20 6a20 3d20 313a 4e20 735f  N sum j = 1:N s_
-00010150: 6a28 7429 202a 207c 2031 2f4e 2073 756d  j(t) * | 1/N sum
-00010160: 206b 203d 2031 3a4e 2065 7870 5b69 202a   k = 1:N exp[i *
-00010170: 2070 6869 5f6b 2874 295d 7c5e 760a 2020   phi_k(t)]|^v.  
-00010180: 2020 7768 6572 6520 4e20 6973 206e 756d    where N is num
-00010190: 6265 7220 6f66 2074 7261 6365 7320 7573  ber of traces us
-000101a0: 6564 2c20 7620 6973 2073 6861 7270 6e65  ed, v is sharpne
-000101b0: 7373 206f 6620 7068 6173 652d 7765 6967  ss of phase-weig
-000101c0: 6874 6564 2073 7461 636b 0a0a 2020 2020  hted stack..    
-000101d0: 5041 5241 4d45 5445 5253 3a0a 2020 2020  PARAMETERS:.    
-000101e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000101f0: 2d2d 2d2d 2d0a 2020 2020 6172 723a 204e  -----.    arr: N
-00010200: 206c 656e 6774 6820 6172 7261 7920 6f66   length array of
-00010210: 2074 696d 6520 7365 7269 6573 2064 6174   time series dat
-00010220: 6120 286e 756d 7079 2e6e 6461 7272 6179  a (numpy.ndarray
-00010230: 290a 2020 2020 7361 6d70 6c69 6e67 5f72  ).    sampling_r
-00010240: 6174 653a 2073 616d 706c 696e 6720 7261  ate: sampling ra
-00010250: 7465 206f 6620 7469 6d65 2073 6572 6965  te of time serie
-00010260: 7320 6172 7220 2869 6e74 290a 2020 2020  s arr (int).    
-00010270: 706f 7765 723a 2065 7870 6f6e 656e 7420  power: exponent 
-00010280: 666f 7220 7068 6173 6520 7374 6163 6b20  for phase stack 
-00010290: 2869 6e74 290a 2020 2020 7077 735f 7469  (int).    pws_ti
-000102a0: 6d65 6761 7465 3a20 6e75 6d62 6572 206f  megate: number o
-000102b0: 6620 7365 636f 6e64 7320 746f 2073 6d6f  f seconds to smo
-000102c0: 6f74 6820 7068 6173 6520 7374 6163 6b20  oth phase stack 
-000102d0: 2866 6c6f 6174 290a 0a20 2020 2052 4554  (float)..    RET
-000102e0: 5552 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d  URNS:.    ------
-000102f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-00010300: 2020 2020 7765 6967 6874 6564 3a20 5068      weighted: Ph
-00010310: 6173 6520 7765 6967 6874 6564 2073 7461  ase weighted sta
-00010320: 636b 206f 6620 7469 6d65 2073 6572 6965  ck of time serie
-00010330: 7320 6461 7461 2028 6e75 6d70 792e 6e64  s data (numpy.nd
-00010340: 6172 7261 7929 0a20 2020 2022 2222 0a0a  array).    """..
-00010350: 2020 2020 6966 2061 7272 2e6e 6469 6d20      if arr.ndim 
-00010360: 3d3d 2031 3a0a 2020 2020 2020 2020 7265  == 1:.        re
-00010370: 7475 726e 2061 7272 0a20 2020 204e 2c20  turn arr.    N, 
-00010380: 4d20 3d20 6172 722e 7368 6170 650a 2020  M = arr.shape.  
-00010390: 2020 616e 616c 7974 6963 203d 2068 696c    analytic = hil
-000103a0: 6265 7274 2861 7272 2c20 6178 6973 3d31  bert(arr, axis=1
-000103b0: 2c20 4e3d 6e65 7874 5f66 6173 745f 6c65  , N=next_fast_le
-000103c0: 6e28 4d29 295b 3a2c 203a 4d5d 0a20 2020  n(M))[:, :M].   
-000103d0: 2070 6861 7365 203d 206e 702e 616e 676c   phase = np.angl
-000103e0: 6528 616e 616c 7974 6963 290a 2020 2020  e(analytic).    
-000103f0: 7068 6173 655f 7374 6163 6b20 3d20 6e70  phase_stack = np
-00010400: 2e6d 6561 6e28 6e70 2e65 7870 2831 6a20  .mean(np.exp(1j 
-00010410: 2a20 7068 6173 6529 2c20 6178 6973 3d30  * phase), axis=0
-00010420: 290a 2020 2020 7068 6173 655f 7374 6163  ).    phase_stac
-00010430: 6b20 3d20 6e70 2e61 6273 2870 6861 7365  k = np.abs(phase
-00010440: 5f73 7461 636b 2920 2a2a 2028 706f 7765  _stack) ** (powe
-00010450: 7229 0a0a 2020 2020 2320 736d 6f6f 7468  r)..    # smooth
-00010460: 696e 670a 2020 2020 2320 7469 6d65 6761  ing.    # timega
-00010470: 7465 5f73 616d 706c 6573 203d 2069 6e74  te_samples = int
-00010480: 2870 7773 5f74 696d 6567 6174 6520 2a20  (pws_timegate * 
-00010490: 7361 6d70 6c69 6e67 5f72 6174 6529 0a20  sampling_rate). 
-000104a0: 2020 2023 2070 6861 7365 5f73 7461 636b     # phase_stack
-000104b0: 203d 206d 6f76 696e 675f 6176 6528 7068   = moving_ave(ph
-000104c0: 6173 655f 7374 6163 6b2c 7469 6d65 6761  ase_stack,timega
-000104d0: 7465 5f73 616d 706c 6573 290a 2020 2020  te_samples).    
-000104e0: 7765 6967 6874 6564 203d 206e 702e 6d75  weighted = np.mu
-000104f0: 6c74 6970 6c79 2861 7272 2c20 7068 6173  ltiply(arr, phas
-00010500: 655f 7374 6163 6b29 0a20 2020 2072 6574  e_stack).    ret
-00010510: 7572 6e20 6e70 2e6d 6561 6e28 7765 6967  urn np.mean(weig
-00010520: 6874 6564 2c20 6178 6973 3d30 290a 0a0a  hted, axis=0)...
-00010530: 6465 6620 6e72 6f6f 745f 7374 6163 6b28  def nroot_stack(
-00010540: 6363 5f61 7272 6179 2c20 706f 7765 7229  cc_array, power)
-00010550: 3a0a 2020 2020 2222 220a 2020 2020 7468  :.    """.    th
-00010560: 6973 2069 7320 6e74 682d 726f 6f74 2073  is is nth-root s
-00010570: 7461 636b 696e 6720 616c 676f 7269 7468  tacking algorith
-00010580: 6d20 7472 616e 736c 6174 6564 2062 6173  m translated bas
-00010590: 6564 206f 6e20 7468 6520 6d61 746c 6162  ed on the matlab
-000105a0: 2066 756e 6374 696f 6e0a 2020 2020 6672   function.    fr
-000105b0: 6f6d 2068 7474 7073 3a2f 2f67 6974 6875  om https://githu
-000105c0: 622e 636f 6d2f 7874 7961 6e67 7073 702f  b.com/xtyangpsp/
-000105d0: 5365 6973 5374 6163 6b20 2862 7920 5869  SeisStack (by Xi
-000105e0: 616f 7461 6f20 5961 6e67 3b20 666f 6c6c  aotao Yang; foll
-000105f0: 6f77 7320 7468 650a 2020 2020 7265 6665  ows the.    refe
-00010600: 7265 6e63 6520 6f66 204d 696c 6c65 742c  rence of Millet,
-00010610: 2046 2065 7420 616c 2e2c 2032 3031 3920   F et al., 2019 
-00010620: 4a47 5229 0a0a 2020 2020 5061 7261 6d65  JGR)..    Parame
-00010630: 7465 7273 3a0a 2020 2020 2d2d 2d2d 2d2d  ters:.    ------
-00010640: 2d2d 2d2d 2d2d 0a20 2020 2063 635f 6172  ------.    cc_ar
-00010650: 7261 793a 206e 756d 7079 2e6e 6461 7272  ray: numpy.ndarr
-00010660: 6179 2063 6f6e 7461 696e 7320 7468 6520  ay contains the 
-00010670: 3244 2063 726f 7373 2063 6f72 7265 6c61  2D cross correla
-00010680: 7469 6f6e 206d 6174 7269 780a 2020 2020  tion matrix.    
-00010690: 706f 7765 723a 206e 702e 696e 742c 206e  power: np.int, n
-000106a0: 7468 2072 6f6f 7420 666f 7220 7468 6520  th root for the 
-000106b0: 7374 6163 6b69 6e67 0a0a 2020 2020 5265  stacking..    Re
-000106c0: 7475 726e 733a 0a20 2020 202d 2d2d 2d2d  turns:.    -----
-000106d0: 2d2d 2d2d 2d2d 2d0a 2020 2020 6e73 7461  -------.    nsta
-000106e0: 636b 3a20 6e70 2e6e 6461 7272 6179 2c20  ck: np.ndarray, 
-000106f0: 6669 6e61 6c20 7374 6163 6b65 6420 7761  final stacked wa
-00010700: 7665 666f 726d 730a 0a20 2020 2057 7269  veforms..    Wri
-00010710: 7474 656e 2062 7920 4368 656e 6778 696e  tten by Chengxin
-00010720: 204a 6961 6e67 2040 414e 5520 284d 6179   Jiang @ANU (May
-00010730: 3230 3230 290a 2020 2020 2222 220a 2020  2020).    """.  
-00010740: 2020 6966 2063 635f 6172 7261 792e 6e64    if cc_array.nd
-00010750: 696d 203d 3d20 313a 0a20 2020 2020 2020  im == 1:.       
-00010760: 206c 6f67 6765 722e 6465 6275 6728 2232   logger.debug("2
-00010770: 4420 6d61 7472 6978 2069 7320 6e65 6564  D matrix is need
-00010780: 6564 2066 6f72 206e 726f 6f74 5f73 7461  ed for nroot_sta
-00010790: 636b 2229 0a20 2020 2020 2020 2072 6574  ck").        ret
-000107a0: 7572 6e20 6363 5f61 7272 6179 0a20 2020  urn cc_array.   
-000107b0: 204e 2c20 4d20 3d20 6363 5f61 7272 6179   N, M = cc_array
-000107c0: 2e73 6861 7065 0a20 2020 2064 6f75 7420  .shape.    dout 
-000107d0: 3d20 6e70 2e7a 6572 6f73 284d 2c20 6474  = np.zeros(M, dt
-000107e0: 7970 653d 6e70 2e66 6c6f 6174 3332 290a  ype=np.float32).
-000107f0: 0a20 2020 2023 2063 6f6e 7374 7275 6374  .    # construct
-00010800: 2079 0a20 2020 2066 6f72 2069 6920 696e   y.    for ii in
-00010810: 2072 616e 6765 284e 293a 0a20 2020 2020   range(N):.     
-00010820: 2020 2064 6174 203d 2063 635f 6172 7261     dat = cc_arra
-00010830: 795b 6969 2c20 3a5d 0a20 2020 2020 2020  y[ii, :].       
-00010840: 2064 6f75 7420 2b3d 206e 702e 7369 676e   dout += np.sign
-00010850: 2864 6174 2920 2a20 6e70 2e61 6273 2864  (dat) * np.abs(d
-00010860: 6174 2920 2a2a 2028 3120 2f20 706f 7765  at) ** (1 / powe
-00010870: 7229 0a20 2020 2064 6f75 7420 2f3d 204e  r).    dout /= N
-00010880: 0a0a 2020 2020 2320 7468 6520 6669 6e61  ..    # the fina
-00010890: 6c20 7374 6163 6b65 6420 7761 7665 666f  l stacked wavefo
-000108a0: 726d 0a20 2020 206e 7374 6163 6b20 3d20  rm.    nstack = 
-000108b0: 646f 7574 202a 206e 702e 6162 7328 646f  dout * np.abs(do
-000108c0: 7574 2920 2a2a 2028 706f 7765 7220 2d20  ut) ** (power - 
-000108d0: 3129 0a0a 2020 2020 7265 7475 726e 206e  1)..    return n
-000108e0: 7374 6163 6b0a 0a0a 6465 6620 7365 6c65  stack...def sele
-000108f0: 6374 6976 655f 7374 6163 6b28 6363 5f61  ctive_stack(cc_a
-00010900: 7272 6179 2c20 6570 7369 6c6f 6e2c 2063  rray, epsilon, c
-00010910: 635f 7468 293a 2020 2320 6e6f 7161 3a20  c_th):  # noqa: 
-00010920: 4638 3131 0a20 2020 2022 2222 0a20 2020  F811.    """.   
-00010930: 2074 6869 7320 6973 2061 2073 656c 6563   this is a selec
-00010940: 7469 7665 2073 7461 636b 696e 6720 616c  tive stacking al
-00010950: 676f 7269 7468 6d20 6465 7665 6c6f 7065  gorithm develope
-00010960: 6420 6279 204a 6172 6564 2042 7279 616e  d by Jared Bryan
-00010970: 2f4b 7572 616d 6120 4f6b 7562 6f2e 0a0a  /Kurama Okubo...
-00010980: 2020 2020 5041 5241 4d45 5445 5253 3a0a      PARAMETERS:.
-00010990: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
-000109a0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2063  ----------.    c
-000109b0: 635f 6172 7261 793a 206e 756d 7079 2e6e  c_array: numpy.n
-000109c0: 6461 7272 6179 2063 6f6e 7461 696e 7320  darray contains 
-000109d0: 7468 6520 3244 2063 726f 7373 2063 6f72  the 2D cross cor
-000109e0: 7265 6c61 7469 6f6e 206d 6174 7269 780a  relation matrix.
-000109f0: 2020 2020 6570 7369 6c6f 6e3a 2072 6573      epsilon: res
-00010a00: 6964 7561 6c20 7468 7265 686f 6c64 2074  idual threhold t
-00010a10: 6f20 7175 6974 2074 6865 2069 7465 7261  o quit the itera
-00010a20: 7469 6f6e 0a20 2020 2063 635f 7468 3a20  tion.    cc_th: 
-00010a30: 6e75 6d70 792e 666c 6f61 742c 2074 6872  numpy.float, thr
-00010a40: 6573 686f 6c64 206f 6620 636f 7272 656c  eshold of correl
-00010a50: 6174 696f 6e20 636f 6566 6669 6369 656e  ation coefficien
-00010a60: 7420 746f 2062 6520 7365 6c65 6374 6564  t to be selected
-00010a70: 0a0a 2020 2020 5245 5455 524e 533a 0a20  ..    RETURNS:. 
-00010a80: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
-00010a90: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6e65  ---------.    ne
-00010aa0: 7773 7461 636b 3a20 6e75 6d70 7920 7665  wstack: numpy ve
-00010ab0: 6374 6f72 2063 6f6e 7461 696e 7320 7468  ctor contains th
-00010ac0: 6520 7374 6163 6b65 6420 6372 6f73 7320  e stacked cross 
-00010ad0: 636f 7272 656c 6174 696f 6e0a 2020 2020  correlation.    
-00010ae0: 6e73 7465 703a 206e 702e 696e 742c 2074  nstep: np.int, t
-00010af0: 6f74 616c 206e 756d 6265 7220 6f66 2069  otal number of i
-00010b00: 7465 7261 7469 6f6e 7320 666f 7220 7468  terations for th
-00010b10: 6520 7374 6163 6b69 6e67 0a0a 2020 2020  e stacking..    
-00010b20: 4f72 6967 696e 616c 6c79 2072 6974 7465  Originally ritte
-00010b30: 6e20 6279 204d 6172 696e 6520 4465 6e6f  n by Marine Deno
-00010b40: 6c6c 650a 2020 2020 4d6f 6469 6669 6564  lle.    Modified
-00010b50: 2062 7920 4368 656e 6778 696e 204a 6961   by Chengxin Jia
-00010b60: 6e67 2040 4861 7276 6172 6420 284f 6374  ng @Harvard (Oct
-00010b70: 3230 3230 290a 2020 2020 2222 220a 2020  2020).    """.  
-00010b80: 2020 6966 2063 635f 6172 7261 792e 6e64    if cc_array.nd
-00010b90: 696d 203d 3d20 313a 0a20 2020 2020 2020  im == 1:.       
-00010ba0: 206c 6f67 6765 722e 6465 6275 6728 2232   logger.debug("2
-00010bb0: 4420 6d61 7472 6978 2069 7320 6e65 6564  D matrix is need
-00010bc0: 6564 2066 6f72 206e 726f 6f74 5f73 7461  ed for nroot_sta
-00010bd0: 636b 2229 0a20 2020 2020 2020 2072 6574  ck").        ret
-00010be0: 7572 6e20 6363 5f61 7272 6179 0a20 2020  urn cc_array.   
-00010bf0: 204e 2c20 4d20 3d20 6363 5f61 7272 6179   N, M = cc_array
-00010c00: 2e73 6861 7065 0a0a 2020 2020 7265 7320  .shape..    res 
-00010c10: 3d20 3965 3920 2023 2072 6573 6964 7561  = 9e9  # residua
-00010c20: 6c73 0a20 2020 2063 6f66 203d 206e 702e  ls.    cof = np.
-00010c30: 7a65 726f 7328 4e2c 2064 7479 7065 3d6e  zeros(N, dtype=n
-00010c40: 702e 666c 6f61 7433 3229 0a20 2020 206e  p.float32).    n
-00010c50: 6577 7374 6163 6b20 3d20 6e70 2e6d 6561  ewstack = np.mea
-00010c60: 6e28 6363 5f61 7272 6179 2c20 6178 6973  n(cc_array, axis
-00010c70: 3d30 290a 0a20 2020 206e 7374 6570 203d  =0)..    nstep =
-00010c80: 2030 0a20 2020 2023 2073 7461 7274 2069   0.    # start i
-00010c90: 7465 7261 7469 6f6e 0a20 2020 2077 6869  teration.    whi
-00010ca0: 6c65 2072 6573 203e 2065 7073 696c 6f6e  le res > epsilon
-00010cb0: 3a0a 2020 2020 2020 2020 666f 7220 6969  :.        for ii
-00010cc0: 2069 6e20 7261 6e67 6528 4e29 3a0a 2020   in range(N):.  
-00010cd0: 2020 2020 2020 2020 2020 636f 665b 6969            cof[ii
-00010ce0: 5d20 3d20 6e70 2e63 6f72 7263 6f65 6628  ] = np.corrcoef(
-00010cf0: 6e65 7773 7461 636b 2c20 6363 5f61 7272  newstack, cc_arr
-00010d00: 6179 5b69 692c 203a 5d29 5b30 2c20 315d  ay[ii, :])[0, 1]
-00010d10: 0a0a 2020 2020 2020 2020 2320 6669 6e64  ..        # find
-00010d20: 2067 6f6f 6420 7761 7665 666f 726d 730a   good waveforms.
-00010d30: 2020 2020 2020 2020 696e 6478 203d 206e          indx = n
-00010d40: 702e 7768 6572 6528 636f 6620 3e3d 2063  p.where(cof >= c
-00010d50: 635f 7468 295b 305d 0a20 2020 2020 2020  c_th)[0].       
-00010d60: 2069 6620 6e6f 7420 6c65 6e28 696e 6478   if not len(indx
-00010d70: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-00010d80: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00010d90: 2263 616e 6e6f 7420 6669 6e64 2067 6f6f  "cannot find goo
-00010da0: 6420 7761 7665 666f 726d 7320 696e 7369  d waveforms insi
-00010db0: 6465 2073 656c 6563 7469 7665 2073 7461  de selective sta
-00010dc0: 636b 696e 6722 290a 2020 2020 2020 2020  cking").        
-00010dd0: 6f6c 6473 7461 636b 203d 206e 6577 7374  oldstack = newst
-00010de0: 6163 6b0a 2020 2020 2020 2020 6e65 7773  ack.        news
-00010df0: 7461 636b 203d 206e 702e 6d65 616e 2863  tack = np.mean(c
-00010e00: 635f 6172 7261 795b 696e 6478 5d2c 2061  c_array[indx], a
-00010e10: 7869 733d 3029 0a20 2020 2020 2020 2072  xis=0).        r
-00010e20: 6573 203d 206e 702e 6c69 6e61 6c67 2e6e  es = np.linalg.n
-00010e30: 6f72 6d28 6e65 7773 7461 636b 202d 206f  orm(newstack - o
-00010e40: 6c64 7374 6163 6b29 202f 2028 6e70 2e6c  ldstack) / (np.l
-00010e50: 696e 616c 672e 6e6f 726d 286e 6577 7374  inalg.norm(newst
-00010e60: 6163 6b29 202a 204d 290a 2020 2020 2020  ack) * M).      
-00010e70: 2020 6e73 7465 7020 2b3d 2031 0a0a 2020    nstep += 1..  
-00010e80: 2020 7265 7475 726e 206e 6577 7374 6163    return newstac
-00010e90: 6b2c 206e 7374 6570 0a0a 0a64 6566 2067  k, nstep...def g
-00010ea0: 6574 5f63 6328 7331 2c20 735f 7265 6629  et_cc(s1, s_ref)
-00010eb0: 3a0a 2020 2020 2320 7265 7475 726e 7320  :.    # returns 
-00010ec0: 7468 6520 636f 7272 656c 6174 696f 6e20  the correlation 
-00010ed0: 636f 6566 6669 6369 656e 7420 6265 7477  coefficient betw
-00010ee0: 6565 6e20 7761 7665 666f 726d 7320 696e  een waveforms in
-00010ef0: 2073 3120 6167 6169 6e73 7420 7265 6665   s1 against refe
-00010f00: 7265 6e63 650a 2020 2020 2320 7761 7665  rence.    # wave
-00010f10: 666f 726d 2073 5f72 6566 2e0a 2020 2020  form s_ref..    
-00010f20: 230a 2020 2020 6363 203d 206e 702e 7a65  #.    cc = np.ze
-00010f30: 726f 7328 7331 2e73 6861 7065 5b30 5d29  ros(s1.shape[0])
-00010f40: 0a20 2020 2073 5f72 6566 5f6e 6f72 6d20  .    s_ref_norm 
-00010f50: 3d20 6e70 2e6c 696e 616c 672e 6e6f 726d  = np.linalg.norm
-00010f60: 2873 5f72 6566 290a 2020 2020 666f 7220  (s_ref).    for 
-00010f70: 6920 696e 2072 616e 6765 2873 312e 7368  i in range(s1.sh
-00010f80: 6170 655b 305d 293a 0a20 2020 2020 2020  ape[0]):.       
-00010f90: 2063 635b 695d 203d 206e 702e 7375 6d28   cc[i] = np.sum(
-00010fa0: 6e70 2e6d 756c 7469 706c 7928 7331 5b69  np.multiply(s1[i
-00010fb0: 2c20 3a5d 2c20 735f 7265 6629 2920 2f20  , :], s_ref)) / 
-00010fc0: 6e70 2e6c 696e 616c 672e 6e6f 726d 2873  np.linalg.norm(s
-00010fd0: 315b 692c 203a 5d29 202f 2073 5f72 6566  1[i, :]) / s_ref
-00010fe0: 5f6e 6f72 6d0a 2020 2020 7265 7475 726e  _norm.    return
-00010ff0: 2063 630a 0a0a 2323 2323 2323 2323 2323   cc...##########
-00011000: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00011010: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00011020: 2323 2323 2323 2323 2323 2323 2323 0a23  ##############.#
-00011030: 2323 2323 2323 2323 2323 2323 2323 2320  ############### 
-00011040: 4d4f 4e49 544f 5249 4e47 2046 554e 4354  MONITORING FUNCT
-00011050: 494f 4e53 2023 2323 2323 2323 2323 2323  IONS ###########
-00011060: 2323 2323 2323 230a 2323 2323 2323 2323  #######.########
-00011070: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00011080: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00011090: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000110a0: 0a0a 2222 220a 6120 636f 6d70 696c 6174  ..""".a compilat
-000110b0: 696f 6e20 6f66 2061 6c6c 2061 7661 696c  ion of all avail
-000110c0: 6162 6c65 2063 6f72 6520 6675 6e63 7469  able core functi
-000110d0: 6f6e 7320 666f 7220 636f 6d70 7574 696e  ons for computin
-000110e0: 6720 7068 6173 6520 6465 6c61 7973 2062  g phase delays b
-000110f0: 6173 6564 206f 6e20 616d 6269 656e 7420  ased on ambient 
-00011100: 6e6f 6973 6520 696e 7465 7266 6572 6f6d  noise interferom
-00011110: 6574 7279 0a0a 7175 6963 6b20 696e 6465  etry..quick inde
-00011120: 7820 6f66 2064 762f 7620 6d65 7468 6f64  x of dv/v method
-00011130: 733a 0a31 2920 7374 7265 7463 6869 6e67  s:.1) stretching
-00011140: 2028 7469 6d65 2073 7472 6574 6368 696e   (time stretchin
-00011150: 673b 2057 6561 7665 7220 6574 2061 6c20  g; Weaver et al 
-00011160: 2832 3031 3129 290a 3229 2064 7477 5f64  (2011)).2) dtw_d
-00011170: 7676 2028 4479 6e61 6d69 6320 5469 6d65  vv (Dynamic Time
-00011180: 2057 6172 7069 6e67 3b20 4d69 6b65 7365   Warping; Mikese
-00011190: 6c6c 2065 7420 616c 2e20 3230 3135 290a  ll et al. 2015).
-000111a0: 3329 206d 7763 735f 6476 7620 284d 6f76  3) mwcs_dvv (Mov
-000111b0: 696e 6720 5769 6e64 6f77 2043 726f 7373  ing Window Cross
-000111c0: 2053 7065 6374 7275 6d3b 2043 6c61 726b   Spectrum; Clark
-000111d0: 2065 7420 616c 2e2c 2032 3031 3129 0a34   et al., 2011).4
-000111e0: 2920 6d77 6363 5f64 7676 2028 4d6f 7669  ) mwcc_dvv (Movi
-000111f0: 6e67 2057 696e 646f 7720 4372 6f73 7320  ng Window Cross 
-00011200: 436f 7272 656c 6174 696f 6e3b 2053 6e69  Correlation; Sni
-00011210: 6564 6572 2065 7420 616c 2e2c 2032 3031  eder et al., 201
-00011220: 3229 0a35 2920 7774 735f 6476 7620 2857  2).5) wts_dvv (W
-00011230: 6176 656c 6574 2053 7472 6563 6869 6e67  avelet Streching
-00011240: 3b20 5975 616e 2065 7420 616c 2e2c 2069  ; Yuan et al., i
-00011250: 6e20 7072 6570 290a 3629 2077 7873 5f64  n prep).6) wxs_d
-00011260: 7676 2028 5761 7665 6c65 7420 5872 6f73  vv (Wavelet Xros
-00011270: 7320 5370 6563 7472 756d 3b20 4d61 6f20  s Spectrum; Mao 
-00011280: 6574 2061 6c2e 2c20 3230 3139 290a 3729  et al., 2019).7)
-00011290: 2077 6477 5f64 7676 2028 5761 7665 6c65   wdw_dvv (Wavele
-000112a0: 7420 4479 6e61 6d69 6320 5761 7270 696e  t Dynamic Warpin
-000112b0: 673b 2059 7561 6e20 6574 2061 6c2e 2c20  g; Yuan et al., 
-000112c0: 696e 2070 7265 7029 0a22 2222 0a0a 0a64  in prep)."""...d
-000112d0: 6566 2073 7472 6574 6368 696e 6728 7265  ef stretching(re
-000112e0: 662c 2063 7572 2c20 6476 5f72 616e 6765  f, cur, dv_range
-000112f0: 2c20 6e62 7472 6961 6c2c 2070 6172 6129  , nbtrial, para)
-00011300: 3a0a 2020 2020 2222 220a 2020 2020 5468  :.    """.    Th
-00011310: 6973 2066 756e 6374 696f 6e20 636f 6d70  is function comp
-00011320: 6172 6573 2074 6865 2052 6566 6572 656e  ares the Referen
-00011330: 6365 2077 6176 6566 6f72 6d20 746f 2073  ce waveform to s
-00011340: 7472 6574 6368 6564 2f63 6f6d 7072 6573  tretched/compres
-00011350: 7365 6420 6375 7272 656e 7420 7761 7665  sed current wave
-00011360: 666f 726d 7320 746f 2067 6574 2074 6865  forms to get the
-00011370: 0a20 2020 2072 656c 6174 6976 6520 7365  .    relative se
-00011380: 6973 6d69 6320 7665 6c6f 6369 7479 2076  ismic velocity v
-00011390: 6172 6961 7469 6f6e 2028 616e 6420 6173  ariation (and as
-000113a0: 736f 6369 6174 6564 2065 7272 6f72 292e  sociated error).
-000113b0: 0a20 2020 2049 7420 616c 736f 2063 6f6d  .    It also com
-000113c0: 7075 7465 7320 7468 6520 636f 7272 656c  putes the correl
-000113d0: 6174 696f 6e20 636f 6566 6669 6369 656e  ation coefficien
-000113e0: 7420 6265 7477 6565 6e20 7468 6520 5265  t between the Re
-000113f0: 6665 7265 6e63 6520 7761 7665 666f 726d  ference waveform
-00011400: 2061 6e64 2074 6865 2063 7572 7265 6e74   and the current
-00011410: 2077 6176 6566 6f72 6d2e 0a0a 2020 2020   waveform...    
-00011420: 5041 5241 4d45 5445 5253 3a0a 2020 2020  PARAMETERS:.    
-00011430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011440: 0a20 2020 2072 6566 3a20 5265 6665 7265  .    ref: Refere
-00011450: 6e63 6520 7761 7665 666f 726d 2028 6e70  nce waveform (np
-00011460: 2e6e 6461 7272 6179 2c20 7369 7a65 204e  .ndarray, size N
-00011470: 290a 2020 2020 6375 723a 2043 7572 7265  ).    cur: Curre
-00011480: 6e74 2077 6176 6566 6f72 6d20 286e 702e  nt waveform (np.
-00011490: 6e64 6172 7261 792c 2073 697a 6520 4e29  ndarray, size N)
-000114a0: 0a20 2020 2064 765f 7261 6e67 653a 2061  .    dv_range: a
-000114b0: 6273 6f6c 7574 6520 626f 756e 6420 666f  bsolute bound fo
-000114c0: 7220 7468 6520 7665 6c6f 6369 7479 2076  r the velocity v
-000114d0: 6172 6961 7469 6f6e 3b20 6578 616d 706c  ariation; exampl
-000114e0: 653a 2064 763d 302e 3033 2066 6f72 205b  e: dv=0.03 for [
-000114f0: 2d33 2c33 5d25 0a20 2020 206f 6620 7265  -3,3]%.    of re
-00011500: 6c61 7469 7665 2076 656c 6f63 6974 7920  lative velocity 
-00011510: 6368 616e 6765 2028 2766 6c6f 6174 2729  change ('float')
-00011520: 0a20 2020 206e 6274 7269 616c 3a20 6e75  .    nbtrial: nu
-00011530: 6d62 6572 206f 6620 7374 7265 7463 6869  mber of stretchi
-00011540: 6e67 2063 6f65 6666 6963 6965 6e74 2062  ng coefficient b
-00011550: 6574 7765 656e 2064 766d 696e 2061 6e64  etween dvmin and
-00011560: 2064 766d 6178 2c20 6e6f 206e 6565 6420   dvmax, no need 
-00011570: 746f 2062 6520 6869 6768 6572 2074 6861  to be higher tha
-00011580: 6e20 3130 3020 2028 2766 6c6f 6174 2729  n 100  ('float')
-00011590: 0a20 2020 2070 6172 613a 2076 6563 746f  .    para: vecto
-000115a0: 7220 6f66 2074 6865 2069 6e64 6963 6573  r of the indices
-000115b0: 206f 6620 7468 6520 6375 7220 616e 6420   of the cur and 
-000115c0: 7265 6620 7769 6e64 6f77 7320 6f6e 2077  ref windows on w
-000115d0: 6963 6820 796f 7520 7761 6e74 2074 6f20  ich you want to 
-000115e0: 646f 2074 6865 206d 6561 7375 7265 6d65  do the measureme
-000115f0: 6e74 730a 2020 2020 286e 702e 6e64 6172  nts.    (np.ndar
-00011600: 7261 792c 2073 697a 6520 746d 696e 2a64  ray, size tmin*d
-00011610: 656c 7461 3a74 6d61 782a 6465 6c74 6129  elta:tmax*delta)
-00011620: 0a20 2020 2046 6f72 2065 7272 6f72 2063  .    For error c
-00011630: 6f6d 7075 7461 7469 6f6e 2c20 7765 206e  omputation, we n
-00011640: 6565 6420 7061 7261 6d65 7465 7273 3a0a  eed parameters:.
-00011650: 2020 2020 2020 2020 666d 696e 3a20 6d69          fmin: mi
-00011660: 6e69 6d75 6d20 6672 6571 7565 6e63 7920  nimum frequency 
-00011670: 6f66 2074 6865 2064 6174 610a 2020 2020  of the data.    
-00011680: 2020 2020 666d 6178 3a20 6d61 7869 6d75      fmax: maximu
-00011690: 6d20 6672 6571 7565 6e63 7920 6f66 2074  m frequency of t
-000116a0: 6865 2064 6174 610a 2020 2020 2020 2020  he data.        
-000116b0: 746d 696e 3a20 6d69 6e69 6d75 6d20 7469  tmin: minimum ti
-000116c0: 6d65 2077 696e 646f 7720 7768 6572 6520  me window where 
-000116d0: 7468 6520 6476 2f76 2069 7320 636f 6d70  the dv/v is comp
-000116e0: 7574 6564 0a20 2020 2020 2020 2074 6d61  uted.        tma
-000116f0: 783a 206d 6178 696d 756d 2074 696d 6520  x: maximum time 
-00011700: 7769 6e64 6f77 2077 6865 7265 2074 6865  window where the
-00011710: 2064 762f 7620 6973 2063 6f6d 7075 7465   dv/v is compute
-00011720: 640a 2020 2020 5245 5455 524e 533a 0a20  d.    RETURNS:. 
-00011730: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
-00011740: 2d2d 2d0a 2020 2020 6476 3a20 5265 6c61  ---.    dv: Rela
-00011750: 7469 7665 2076 656c 6f63 6974 7920 6368  tive velocity ch
-00011760: 616e 6765 2064 762f 7620 2869 6e20 2529  ange dv/v (in %)
-00011770: 0a20 2020 2063 633a 2063 6f72 7265 6c61  .    cc: correla
-00011780: 7469 6f6e 2063 6f65 6666 6963 6965 6e74  tion coefficient
-00011790: 2062 6574 7765 656e 2074 6865 2072 6566   between the ref
-000117a0: 6572 656e 6365 2077 6176 6566 6f72 6d20  erence waveform 
-000117b0: 616e 6420 7468 6520 6265 7374 2073 7472  and the best str
-000117c0: 6574 6368 6564 2f63 6f6d 7072 6573 7365  etched/compresse
-000117d0: 6420 6375 7272 656e 7420 7761 7665 666f  d current wavefo
-000117e0: 726d 0a20 2020 2063 6470 3a20 636f 7272  rm.    cdp: corr
-000117f0: 656c 6174 696f 6e20 636f 6566 6669 6369  elation coeffici
-00011800: 656e 7420 6265 7477 6565 6e20 7468 6520  ent between the 
-00011810: 7265 6665 7265 6e63 6520 7761 7665 666f  reference wavefo
-00011820: 726d 2061 6e64 2074 6865 2069 6e69 7469  rm and the initi
-00011830: 616c 2063 7572 7265 6e74 2077 6176 6566  al current wavef
-00011840: 6f72 6d0a 2020 2020 6572 726f 723a 2045  orm.    error: E
-00011850: 7272 6f72 7320 696e 2074 6865 2064 762f  rrors in the dv/
-00011860: 7620 6d65 6173 7572 656d 656e 7473 2062  v measurements b
-00011870: 6173 6564 206f 6e20 5765 6176 6572 2065  ased on Weaver e
-00011880: 7420 616c 2028 3230 3131 292c 0a20 2020  t al (2011),.   
-00011890: 204f 6e20 7468 6520 7072 6563 6973 696f   On the precisio
-000118a0: 6e20 6f66 206e 6f69 7365 2d63 6f72 7265  n of noise-corre
-000118b0: 6c61 7469 6f6e 2069 6e74 6572 6665 726f  lation interfero
-000118c0: 6d65 7472 792c 2047 656f 7068 7973 2e20  metry, Geophys. 
-000118d0: 4a2e 2049 6e74 2e2c 2031 3835 2833 290a  J. Int., 185(3).
-000118e0: 0a20 2020 204e 6f74 653a 2054 6865 2063  .    Note: The c
-000118f0: 6f64 6520 6669 7273 7420 6669 6e64 7320  ode first finds 
-00011900: 7468 6520 6265 7374 2063 6f72 7265 6c61  the best correla
-00011910: 7469 6f6e 2063 6f65 6666 6963 6965 6e74  tion coefficient
-00011920: 2062 6574 7765 656e 2074 6865 2052 6566   between the Ref
-00011930: 6572 656e 6365 2077 6176 6566 6f72 6d20  erence waveform 
-00011940: 616e 640a 2020 2020 7468 6520 7374 7265  and.    the stre
-00011950: 7463 6865 642f 636f 6d70 7265 7373 6564  tched/compressed
-00011960: 2063 7572 7265 6e74 2077 6176 6566 6f72   current wavefor
-00011970: 6d20 616d 6f6e 6720 7468 6520 226e 6274  m among the "nbt
-00011980: 7269 616c 2220 7661 6c75 6573 2e0a 2020  rial" values..  
-00011990: 2020 4120 7265 6669 6e65 6420 616e 616c    A refined anal
-000119a0: 7973 6973 2069 7320 7468 656e 2070 6572  ysis is then per
-000119b0: 666f 726d 6564 2061 726f 756e 6420 7468  formed around th
-000119c0: 6973 2076 616c 7565 2074 6f20 6f62 7461  is value to obta
-000119d0: 696e 2061 206d 6f72 6520 7072 6563 6973  in a more precis
-000119e0: 6520 6476 2f76 206d 6561 7375 7265 6d65  e dv/v measureme
-000119f0: 6e74 202e 0a0a 2020 2020 4f72 6967 696e  nt ...    Origin
-00011a00: 616c 6c79 2062 7920 4c2e 2056 6965 6e73  ally by L. Viens
-00011a10: 2030 342f 3236 2f32 3031 3820 2856 6965   04/26/2018 (Vie
-00011a20: 6e73 2065 7420 616c 2e2c 2032 3031 3820  ns et al., 2018 
-00011a30: 4a47 5229 0a20 2020 206d 6f64 6966 6965  JGR).    modifie
-00011a40: 6420 6279 2043 6865 6e67 7869 6e20 4a69  d by Chengxin Ji
-00011a50: 616e 670a 2020 2020 2222 220a 2020 2020  ang.    """.    
-00011a60: 2320 6c6f 6164 2063 6f6d 6d6f 6e20 7661  # load common va
-00011a70: 7269 6162 6c65 7320 6672 6f6d 2064 6963  riables from dic
-00011a80: 7469 6f6e 6172 790a 2020 2020 7477 696e  tionary.    twin
-00011a90: 203d 2070 6172 615b 2274 7769 6e22 5d0a   = para["twin"].
-00011aa0: 2020 2020 6672 6571 203d 2070 6172 615b      freq = para[
-00011ab0: 2266 7265 7122 5d0a 2020 2020 6474 203d  "freq"].    dt =
-00011ac0: 2070 6172 615b 2264 7422 5d0a 2020 2020   para["dt"].    
-00011ad0: 746d 696e 203d 206e 702e 6d69 6e28 7477  tmin = np.min(tw
-00011ae0: 696e 290a 2020 2020 746d 6178 203d 206e  in).    tmax = n
-00011af0: 702e 6d61 7828 7477 696e 290a 2020 2020  p.max(twin).    
-00011b00: 666d 696e 203d 206e 702e 6d69 6e28 6672  fmin = np.min(fr
-00011b10: 6571 290a 2020 2020 666d 6178 203d 206e  eq).    fmax = n
-00011b20: 702e 6d61 7828 6672 6571 290a 2020 2020  p.max(freq).    
-00011b30: 7476 6563 203d 206e 702e 6172 616e 6765  tvec = np.arange
-00011b40: 2874 6d69 6e2c 2074 6d61 782c 2064 7429  (tmin, tmax, dt)
-00011b50: 0a0a 2020 2020 2320 6d61 6b65 2075 7365  ..    # make use
-00011b60: 6675 6c20 6f6e 6520 666f 7220 6d65 6173  ful one for meas
-00011b70: 7572 656d 656e 7473 0a20 2020 2064 766d  urements.    dvm
-00011b80: 696e 203d 202d 6e70 2e61 6273 2864 765f  in = -np.abs(dv_
-00011b90: 7261 6e67 6529 0a20 2020 2064 766d 6178  range).    dvmax
-00011ba0: 203d 206e 702e 6162 7328 6476 5f72 616e   = np.abs(dv_ran
-00011bb0: 6765 290a 2020 2020 4570 7320 3d20 3120  ge).    Eps = 1 
-00011bc0: 2b20 286e 702e 6c69 6e73 7061 6365 2864  + (np.linspace(d
-00011bd0: 766d 696e 2c20 6476 6d61 782c 206e 6274  vmin, dvmax, nbt
-00011be0: 7269 616c 2929 0a20 2020 2063 6f66 203d  rial)).    cof =
-00011bf0: 206e 702e 7a65 726f 7328 4570 732e 7368   np.zeros(Eps.sh
-00011c00: 6170 652c 2064 7479 7065 3d6e 702e 666c  ape, dtype=np.fl
-00011c10: 6f61 7433 3229 0a0a 2020 2020 2320 5365  oat32)..    # Se
-00011c20: 7420 6f66 2073 7472 6574 6368 6564 2f63  t of stretched/c
-00011c30: 6f6d 7072 6573 7365 6420 6375 7272 656e  ompressed curren
-00011c40: 7420 7761 7665 666f 726d 730a 2020 2020  t waveforms.    
-00011c50: 666f 7220 6969 2069 6e20 7261 6e67 6528  for ii in range(
-00011c60: 6c65 6e28 4570 7329 293a 0a20 2020 2020  len(Eps)):.     
-00011c70: 2020 206e 7420 3d20 7476 6563 202a 2045     nt = tvec * E
-00011c80: 7073 5b69 695d 0a20 2020 2020 2020 2073  ps[ii].        s
-00011c90: 203d 206e 702e 696e 7465 7270 2878 3d74   = np.interp(x=t
-00011ca0: 7665 632c 2078 703d 6e74 2c20 6670 3d63  vec, xp=nt, fp=c
-00011cb0: 7572 290a 2020 2020 2020 2020 7761 7665  ur).        wave
-00011cc0: 666f 726d 5f72 6566 203d 2072 6566 0a20  form_ref = ref. 
-00011cd0: 2020 2020 2020 2077 6176 6566 6f72 6d5f         waveform_
-00011ce0: 6375 7220 3d20 730a 2020 2020 2020 2020  cur = s.        
-00011cf0: 636f 665b 6969 5d20 3d20 6e70 2e63 6f72  cof[ii] = np.cor
-00011d00: 7263 6f65 6628 7761 7665 666f 726d 5f72  rcoef(waveform_r
-00011d10: 6566 2c20 7761 7665 666f 726d 5f63 7572  ef, waveform_cur
-00011d20: 295b 302c 2031 5d0a 0a20 2020 2063 6470  )[0, 1]..    cdp
-00011d30: 203d 206e 702e 636f 7272 636f 6566 2863   = np.corrcoef(c
-00011d40: 7572 2c20 7265 6629 5b30 2c20 315d 2020  ur, ref)[0, 1]  
-00011d50: 2320 636f 7272 656c 6174 696f 6e20 636f  # correlation co
-00011d60: 6566 6669 6369 656e 7420 6265 7477 6565  efficient betwee
-00011d70: 6e20 7468 6520 7265 6665 7265 6e63 6520  n the reference 
-00011d80: 616e 6420 696e 6974 6961 6c20 6375 7272  and initial curr
-00011d90: 656e 7420 7761 7665 666f 726d 730a 0a20  ent waveforms.. 
-00011da0: 2020 2023 2066 696e 6420 7468 6520 6d61     # find the ma
-00011db0: 7869 6d75 6d20 636f 7272 656c 6174 696f  ximum correlatio
-00011dc0: 6e20 636f 6566 6669 6369 656e 740a 2020  n coefficient.  
-00011dd0: 2020 696d 6178 203d 206e 702e 6e61 6e61    imax = np.nana
-00011de0: 7267 6d61 7828 636f 6629 0a20 2020 2069  rgmax(cof).    i
-00011df0: 6620 696d 6178 203e 3d20 6c65 6e28 4570  f imax >= len(Ep
-00011e00: 7329 202d 2032 3a0a 2020 2020 2020 2020  s) - 2:.        
-00011e10: 696d 6178 203d 2069 6d61 7820 2d20 320a  imax = imax - 2.
-00011e20: 2020 2020 6966 2069 6d61 7820 3c3d 2032      if imax <= 2
-00011e30: 3a0a 2020 2020 2020 2020 696d 6178 203d  :.        imax =
-00011e40: 2069 6d61 7820 2b20 320a 0a20 2020 2023   imax + 2..    #
-00011e50: 2050 726f 6365 6564 2074 6f20 7468 6520   Proceed to the 
-00011e60: 7365 636f 6e64 2073 7465 7020 746f 2067  second step to g
-00011e70: 6574 2061 206d 6f72 6520 7072 6563 6973  et a more precis
-00011e80: 6520 6476 2f76 206d 6561 7375 7265 6d65  e dv/v measureme
-00011e90: 6e74 0a20 2020 2064 7466 696e 6572 203d  nt.    dtfiner =
-00011ea0: 206e 702e 6c69 6e73 7061 6365 2845 7073   np.linspace(Eps
-00011eb0: 5b69 6d61 7820 2d20 325d 2c20 4570 735b  [imax - 2], Eps[
-00011ec0: 696d 6178 202b 2032 5d2c 2031 3030 290a  imax + 2], 100).
-00011ed0: 2020 2020 6e63 6f66 203d 206e 702e 7a65      ncof = np.ze
-00011ee0: 726f 7328 6474 6669 6e65 722e 7368 6170  ros(dtfiner.shap
-00011ef0: 652c 2064 7479 7065 3d6e 702e 666c 6f61  e, dtype=np.floa
-00011f00: 7433 3229 0a20 2020 2066 6f72 2069 6920  t32).    for ii 
-00011f10: 696e 2072 616e 6765 286c 656e 2864 7466  in range(len(dtf
-00011f20: 696e 6572 2929 3a0a 2020 2020 2020 2020  iner)):.        
-00011f30: 6e74 203d 2074 7665 6320 2a20 6474 6669  nt = tvec * dtfi
-00011f40: 6e65 725b 6969 5d0a 2020 2020 2020 2020  ner[ii].        
-00011f50: 7320 3d20 6e70 2e69 6e74 6572 7028 783d  s = np.interp(x=
-00011f60: 7476 6563 2c20 7870 3d6e 742c 2066 703d  tvec, xp=nt, fp=
-00011f70: 6375 7229 0a20 2020 2020 2020 2077 6176  cur).        wav
-00011f80: 6566 6f72 6d5f 7265 6620 3d20 7265 660a  eform_ref = ref.
-00011f90: 2020 2020 2020 2020 7761 7665 666f 726d          waveform
-00011fa0: 5f63 7572 203d 2073 0a20 2020 2020 2020  _cur = s.       
-00011fb0: 206e 636f 665b 6969 5d20 3d20 6e70 2e63   ncof[ii] = np.c
-00011fc0: 6f72 7263 6f65 6628 7761 7665 666f 726d  orrcoef(waveform
-00011fd0: 5f72 6566 2c20 7761 7665 666f 726d 5f63  _ref, waveform_c
-00011fe0: 7572 295b 302c 2031 5d0a 0a20 2020 2063  ur)[0, 1]..    c
-00011ff0: 6320 3d20 6e70 2e6d 6178 286e 636f 6629  c = np.max(ncof)
-00012000: 2020 2320 4669 6e64 206d 6178 696d 756d    # Find maximum
-00012010: 2063 6f72 7265 6c61 7469 6f6e 2063 6f65   correlation coe
-00012020: 6666 6963 6965 6e74 206f 6620 7468 6520  fficient of the 
-00012030: 7265 6669 6e65 6420 2061 6e61 6c79 7369  refined  analysi
-00012040: 730a 2020 2020 6476 203d 2031 3030 2e30  s.    dv = 100.0
-00012050: 202a 2064 7466 696e 6572 5b6e 702e 6172   * dtfiner[np.ar
-00012060: 676d 6178 286e 636f 6629 5d20 2d20 3130  gmax(ncof)] - 10
-00012070: 3020 2023 204d 756c 7469 706c 7920 6279  0  # Multiply by
-00012080: 2031 3030 2074 6f20 636f 6e76 6572 7420   100 to convert 
-00012090: 746f 2070 6572 6365 6e74 6167 6520 2845  to percentage (E
-000120a0: 7073 696c 6f6e 203d 202d 6474 2f74 203d  psilon = -dt/t =
-000120b0: 2064 762f 7629 0a0a 2020 2020 2320 4572   dv/v)..    # Er
-000120c0: 726f 7220 636f 6d70 7574 6174 696f 6e20  ror computation 
-000120d0: 6261 7365 6420 6f6e 2057 6561 7665 7220  based on Weaver 
-000120e0: 6574 2061 6c20 2832 3031 3129 2c20 4f6e  et al (2011), On
-000120f0: 2074 6865 2070 7265 6369 7369 6f6e 206f   the precision o
-00012100: 6620 6e6f 6973 652d 636f 7272 656c 6174  f noise-correlat
-00012110: 696f 6e0a 2020 2020 2320 696e 7465 7266  ion.    # interf
-00012120: 6572 6f6d 6574 7279 2c20 4765 6f70 6879  erometry, Geophy
-00012130: 732e 204a 2e20 496e 742e 2c20 3138 3528  s. J. Int., 185(
-00012140: 3329 0a20 2020 2054 203d 2031 202f 2028  3).    T = 1 / (
-00012150: 666d 6178 202d 2066 6d69 6e29 0a20 2020  fmax - fmin).   
-00012160: 2058 203d 2063 630a 2020 2020 7763 203d   X = cc.    wc =
-00012170: 206e 702e 7069 202a 2028 666d 696e 202b   np.pi * (fmin +
-00012180: 2066 6d61 7829 0a20 2020 2074 3120 3d20   fmax).    t1 = 
-00012190: 6e70 2e6d 696e 285b 746d 696e 2c20 746d  np.min([tmin, tm
-000121a0: 6178 5d29 0a20 2020 2074 3220 3d20 6e70  ax]).    t2 = np
-000121b0: 2e6d 6178 285b 746d 696e 2c20 746d 6178  .max([tmin, tmax
-000121c0: 5d29 0a20 2020 2065 7272 6f72 203d 2031  ]).    error = 1
-000121d0: 3030 202a 2028 0a20 2020 2020 2020 206e  00 * (.        n
-000121e0: 702e 7371 7274 2831 202d 2058 2a2a 3229  p.sqrt(1 - X**2)
-000121f0: 202f 2028 3220 2a20 5829 202a 206e 702e   / (2 * X) * np.
-00012200: 7371 7274 2828 3620 2a20 6e70 2e73 7172  sqrt((6 * np.sqr
-00012210: 7428 6e70 2e70 6920 2f20 3229 202a 2054  t(np.pi / 2) * T
-00012220: 2920 2f20 2877 632a 2a32 202a 2028 7432  ) / (wc**2 * (t2
-00012230: 2a2a 3320 2d20 7431 2a2a 3329 2929 0a20  **3 - t1**3))). 
-00012240: 2020 2029 0a0a 2020 2020 7265 7475 726e     )..    return
-00012250: 2064 762c 2065 7272 6f72 2c20 6363 2c20   dv, error, cc, 
-00012260: 6364 700a 0a0a 6465 6620 7374 7265 7463  cdp...def stretc
-00012270: 6869 6e67 5f76 6563 7428 7265 662c 2063  hing_vect(ref, c
-00012280: 7572 2c20 6476 5f72 616e 6765 2c20 6e62  ur, dv_range, nb
-00012290: 7472 6961 6c2c 2070 6172 6129 3a0a 2020  trial, para):.  
-000122a0: 2020 2222 220a 2020 2020 5468 6973 2066    """.    This f
-000122b0: 756e 6374 696f 6e20 636f 6d70 6172 6573  unction compares
-000122c0: 2074 6865 2052 6566 6572 656e 6365 2077   the Reference w
-000122d0: 6176 6566 6f72 6d20 746f 2073 7472 6574  aveform to stret
-000122e0: 6368 6564 2f63 6f6d 7072 6573 7365 6420  ched/compressed 
-000122f0: 6375 7272 656e 7420 7761 7665 666f 726d  current waveform
-00012300: 730a 2020 2020 746f 2067 6574 2074 6865  s.    to get the
-00012310: 2072 656c 6174 6976 6520 7365 6973 6d69   relative seismi
-00012320: 6320 7665 6c6f 6369 7479 2076 6172 6961  c velocity varia
-00012330: 7469 6f6e 2028 616e 6420 6173 736f 6369  tion (and associ
-00012340: 6174 6564 2065 7272 6f72 292e 0a20 2020  ated error)..   
-00012350: 2049 7420 616c 736f 2063 6f6d 7075 7465   It also compute
-00012360: 7320 7468 6520 636f 7272 656c 6174 696f  s the correlatio
-00012370: 6e20 636f 6566 6669 6369 656e 7420 6265  n coefficient be
-00012380: 7477 6565 6e20 7468 6520 5265 6665 7265  tween the Refere
-00012390: 6e63 6520 7761 7665 666f 726d 2061 6e64  nce waveform and
-000123a0: 2074 6865 2063 7572 7265 6e74 2077 6176   the current wav
-000123b0: 6566 6f72 6d2e 0a0a 2020 2020 5041 5241  eform...    PARA
-000123c0: 4d45 5445 5253 3a0a 2020 2020 2d2d 2d2d  METERS:.    ----
-000123d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
-000123e0: 2072 6566 3a20 5265 6665 7265 6e63 6520   ref: Reference 
-000123f0: 7761 7665 666f 726d 2028 6e70 2e6e 6461  waveform (np.nda
-00012400: 7272 6179 2c20 7369 7a65 204e 290a 2020  rray, size N).  
-00012410: 2020 6375 723a 2043 7572 7265 6e74 2077    cur: Current w
-00012420: 6176 6566 6f72 6d20 286e 702e 6e64 6172  aveform (np.ndar
-00012430: 7261 792c 2073 697a 6520 4e29 0a20 2020  ray, size N).   
-00012440: 2064 765f 7261 6e67 653a 2061 6273 6f6c   dv_range: absol
-00012450: 7574 6520 626f 756e 6420 666f 7220 7468  ute bound for th
-00012460: 6520 7665 6c6f 6369 7479 2076 6172 6961  e velocity varia
-00012470: 7469 6f6e 3b20 6578 616d 706c 653a 2064  tion; example: d
-00012480: 763d 302e 3033 2066 6f72 205b 2d33 2c33  v=0.03 for [-3,3
-00012490: 5d25 0a20 2020 206f 6620 7265 6c61 7469  ]%.    of relati
-000124a0: 7665 2076 656c 6f63 6974 7920 6368 616e  ve velocity chan
-000124b0: 6765 2028 2766 6c6f 6174 2729 0a20 2020  ge ('float').   
-000124c0: 206e 6274 7269 616c 3a20 6e75 6d62 6572   nbtrial: number
-000124d0: 206f 6620 7374 7265 7463 6869 6e67 2063   of stretching c
-000124e0: 6f65 6666 6963 6965 6e74 2062 6574 7765  oefficient betwe
-000124f0: 656e 2064 766d 696e 2061 6e64 2064 766d  en dvmin and dvm
-00012500: 6178 2c20 6e6f 206e 6565 6420 746f 2062  ax, no need to b
-00012510: 6520 6869 6768 6572 2074 6861 6e20 3130  e higher than 10
-00012520: 3020 2028 2766 6c6f 6174 2729 0a20 2020  0  ('float').   
-00012530: 2070 6172 613a 2076 6563 746f 7220 6f66   para: vector of
-00012540: 2074 6865 2069 6e64 6963 6573 206f 6620   the indices of 
-00012550: 7468 6520 6375 7220 616e 6420 7265 6620  the cur and ref 
-00012560: 7769 6e64 6f77 7320 6f6e 2077 6963 6820  windows on wich 
-00012570: 796f 7520 7761 6e74 2074 6f20 646f 2074  you want to do t
-00012580: 6865 0a20 2020 206d 6561 7375 7265 6d65  he.    measureme
-00012590: 6e74 7320 286e 702e 6e64 6172 7261 792c  nts (np.ndarray,
-000125a0: 2073 697a 6520 746d 696e 2a64 656c 7461   size tmin*delta
-000125b0: 3a74 6d61 782a 6465 6c74 6129 0a20 2020  :tmax*delta).   
-000125c0: 2046 6f72 2065 7272 6f72 2063 6f6d 7075   For error compu
-000125d0: 7461 7469 6f6e 2c20 7765 206e 6565 6420  tation, we need 
-000125e0: 7061 7261 6d65 7465 7273 3a0a 2020 2020  parameters:.    
-000125f0: 2020 2020 666d 696e 3a20 6d69 6e69 6d75      fmin: minimu
-00012600: 6d20 6672 6571 7565 6e63 7920 6f66 2074  m frequency of t
-00012610: 6865 2064 6174 610a 2020 2020 2020 2020  he data.        
-00012620: 666d 6178 3a20 6d61 7869 6d75 6d20 6672  fmax: maximum fr
-00012630: 6571 7565 6e63 7920 6f66 2074 6865 2064  equency of the d
-00012640: 6174 610a 2020 2020 2020 2020 746d 696e  ata.        tmin
-00012650: 3a20 6d69 6e69 6d75 6d20 7469 6d65 2077  : minimum time w
-00012660: 696e 646f 7720 7768 6572 6520 7468 6520  indow where the 
-00012670: 6476 2f76 2069 7320 636f 6d70 7574 6564  dv/v is computed
-00012680: 0a20 2020 2020 2020 2074 6d61 783a 206d  .        tmax: m
-00012690: 6178 696d 756d 2074 696d 6520 7769 6e64  aximum time wind
-000126a0: 6f77 2077 6865 7265 2074 6865 2064 762f  ow where the dv/
-000126b0: 7620 6973 2063 6f6d 7075 7465 640a 2020  v is computed.  
-000126c0: 2020 5245 5455 524e 533a 0a20 2020 202d    RETURNS:.    -
-000126d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-000126e0: 2020 2020 6476 3a20 5265 6c61 7469 7665      dv: Relative
-000126f0: 2076 656c 6f63 6974 7920 6368 616e 6765   velocity change
-00012700: 2064 762f 7620 2869 6e20 2529 0a20 2020   dv/v (in %).   
-00012710: 2063 633a 2063 6f72 7265 6c61 7469 6f6e   cc: correlation
-00012720: 2063 6f65 6666 6963 6965 6e74 2062 6574   coefficient bet
-00012730: 7765 656e 2074 6865 2072 6566 6572 656e  ween the referen
-00012740: 6365 2077 6176 6566 6f72 6d20 616e 6420  ce waveform and 
-00012750: 7468 6520 6265 7374 2073 7472 6574 6368  the best stretch
-00012760: 6564 2f63 6f6d 7072 6573 7365 6420 6375  ed/compressed cu
-00012770: 7272 656e 7420 7761 7665 666f 726d 0a20  rrent waveform. 
-00012780: 2020 2063 6470 3a20 636f 7272 656c 6174     cdp: correlat
-00012790: 696f 6e20 636f 6566 6669 6369 656e 7420  ion coefficient 
-000127a0: 6265 7477 6565 6e20 7468 6520 7265 6665  between the refe
-000127b0: 7265 6e63 6520 7761 7665 666f 726d 2061  rence waveform a
-000127c0: 6e64 2074 6865 2069 6e69 7469 616c 2063  nd the initial c
-000127d0: 7572 7265 6e74 2077 6176 6566 6f72 6d0a  urrent waveform.
-000127e0: 2020 2020 6572 726f 723a 2045 7272 6f72      error: Error
-000127f0: 7320 696e 2074 6865 2064 762f 7620 6d65  s in the dv/v me
-00012800: 6173 7572 656d 656e 7473 2062 6173 6564  asurements based
-00012810: 206f 6e20 5765 6176 6572 2065 7420 616c   on Weaver et al
-00012820: 2028 3230 3131 292c 204f 6e20 7468 6520   (2011), On the 
-00012830: 7072 6563 6973 696f 6e0a 2020 2020 6f66  precision.    of
-00012840: 206e 6f69 7365 2d63 6f72 7265 6c61 7469   noise-correlati
-00012850: 6f6e 2069 6e74 6572 6665 726f 6d65 7472  on interferometr
-00012860: 792c 2047 656f 7068 7973 2e20 4a2e 2049  y, Geophys. J. I
-00012870: 6e74 2e2c 2031 3835 2833 290a 0a20 2020  nt., 185(3)..   
-00012880: 204e 6f74 653a 2054 6865 2063 6f64 6520   Note: The code 
-00012890: 6669 7273 7420 6669 6e64 7320 7468 6520  first finds the 
-000128a0: 6265 7374 2063 6f72 7265 6c61 7469 6f6e  best correlation
-000128b0: 2063 6f65 6666 6963 6965 6e74 2062 6574   coefficient bet
-000128c0: 7765 656e 2074 6865 2052 6566 6572 656e  ween the Referen
-000128d0: 6365 2077 6176 6566 6f72 6d20 616e 640a  ce waveform and.
-000128e0: 2020 2020 7468 6520 7374 7265 7463 6865      the stretche
-000128f0: 642f 636f 6d70 7265 7373 6564 2063 7572  d/compressed cur
-00012900: 7265 6e74 2077 6176 6566 6f72 6d20 616d  rent waveform am
-00012910: 6f6e 6720 7468 6520 226e 6274 7269 616c  ong the "nbtrial
-00012920: 2220 7661 6c75 6573 2e0a 2020 2020 4120  " values..    A 
-00012930: 7265 6669 6e65 6420 616e 616c 7973 6973  refined analysis
-00012940: 2069 7320 7468 656e 2070 6572 666f 726d   is then perform
-00012950: 6564 2061 726f 756e 6420 7468 6973 2076  ed around this v
-00012960: 616c 7565 2074 6f20 6f62 7461 696e 2061  alue to obtain a
-00012970: 206d 6f72 6520 7072 6563 6973 6520 6476   more precise dv
-00012980: 2f76 206d 6561 7375 7265 6d65 6e74 202e  /v measurement .
-00012990: 0a0a 2020 2020 4f72 6967 696e 616c 6c79  ..    Originally
-000129a0: 2062 7920 4c2e 2056 6965 6e73 2030 342f   by L. Viens 04/
-000129b0: 3236 2f32 3031 3820 2856 6965 6e73 2065  26/2018 (Viens e
-000129c0: 7420 616c 2e2c 2032 3031 3820 4a47 5229  t al., 2018 JGR)
-000129d0: 0a20 2020 206d 6f64 6966 6965 6420 6279  .    modified by
-000129e0: 2043 6865 6e67 7869 6e20 4a69 616e 670a   Chengxin Jiang.
-000129f0: 2020 2020 6d6f 6469 6669 6564 2062 7920      modified by 
-00012a00: 4c61 7572 6120 4572 6d65 7274 3a20 7665  Laura Ermert: ve
-00012a10: 6374 6f72 697a 6564 2076 6572 7369 6f6e  ctorized version
-00012a20: 0a20 2020 2022 2222 0a20 2020 2023 206c  .    """.    # l
-00012a30: 6f61 6420 636f 6d6d 6f6e 2076 6172 6961  oad common varia
-00012a40: 626c 6573 2066 726f 6d20 6469 6374 696f  bles from dictio
-00012a50: 6e61 7279 0a20 2020 2074 7769 6e20 3d20  nary.    twin = 
-00012a60: 7061 7261 5b22 7477 696e 225d 0a20 2020  para["twin"].   
-00012a70: 2066 7265 7120 3d20 7061 7261 5b22 6672   freq = para["fr
-00012a80: 6571 225d 0a20 2020 2064 7420 3d20 7061  eq"].    dt = pa
-00012a90: 7261 5b22 6474 225d 0a20 2020 2074 6d69  ra["dt"].    tmi
-00012aa0: 6e20 3d20 6e70 2e6d 696e 2874 7769 6e29  n = np.min(twin)
-00012ab0: 0a20 2020 2074 6d61 7820 3d20 6e70 2e6d  .    tmax = np.m
-00012ac0: 6178 2874 7769 6e29 0a20 2020 2066 6d69  ax(twin).    fmi
-00012ad0: 6e20 3d20 6e70 2e6d 696e 2866 7265 7129  n = np.min(freq)
-00012ae0: 0a20 2020 2066 6d61 7820 3d20 6e70 2e6d  .    fmax = np.m
-00012af0: 6178 2866 7265 7129 0a20 2020 2074 7665  ax(freq).    tve
-00012b00: 6320 3d20 6e70 2e61 7261 6e67 6528 746d  c = np.arange(tm
-00012b10: 696e 2c20 746d 6178 2c20 6474 290a 0a20  in, tmax, dt).. 
-00012b20: 2020 2023 206d 616b 6520 7573 6566 756c     # make useful
-00012b30: 206f 6e65 2066 6f72 206d 6561 7375 7265   one for measure
-00012b40: 6d65 6e74 730a 2020 2020 6476 6d69 6e20  ments.    dvmin 
-00012b50: 3d20 2d6e 702e 6162 7328 6476 5f72 616e  = -np.abs(dv_ran
-00012b60: 6765 290a 2020 2020 6476 6d61 7820 3d20  ge).    dvmax = 
-00012b70: 6e70 2e61 6273 2864 765f 7261 6e67 6529  np.abs(dv_range)
-00012b80: 0a20 2020 2045 7073 203d 2031 202b 2028  .    Eps = 1 + (
-00012b90: 6e70 2e6c 696e 7370 6163 6528 6476 6d69  np.linspace(dvmi
-00012ba0: 6e2c 2064 766d 6178 2c20 6e62 7472 6961  n, dvmax, nbtria
-00012bb0: 6c29 290a 2020 2020 6364 7020 3d20 6e70  l)).    cdp = np
-00012bc0: 2e63 6f72 7263 6f65 6628 6375 722c 2072  .corrcoef(cur, r
-00012bd0: 6566 295b 302c 2031 5d20 2023 2063 6f72  ef)[0, 1]  # cor
-00012be0: 7265 6c61 7469 6f6e 2063 6f65 6666 6963  relation coeffic
-00012bf0: 6965 6e74 2062 6574 7765 656e 2074 6865  ient between the
-00012c00: 2072 6566 6572 656e 6365 2061 6e64 2069   reference and i
-00012c10: 6e69 7469 616c 2063 7572 7265 6e74 2077  nitial current w
-00012c20: 6176 6566 6f72 6d73 0a20 2020 2077 6176  aveforms.    wav
-00012c30: 6566 6f72 6d73 203d 206e 702e 7a65 726f  eforms = np.zero
-00012c40: 7328 286e 6274 7269 616c 202b 2031 2c20  s((nbtrial + 1, 
-00012c50: 6c65 6e28 7265 6629 2929 0a20 2020 2077  len(ref))).    w
-00012c60: 6176 6566 6f72 6d73 5b30 2c20 3a5d 203d  aveforms[0, :] =
-00012c70: 2072 6566 0a0a 2020 2020 2320 5365 7420   ref..    # Set 
-00012c80: 6f66 2073 7472 6574 6368 6564 2f63 6f6d  of stretched/com
-00012c90: 7072 6573 7365 6420 6375 7272 656e 7420  pressed current 
-00012ca0: 7761 7665 666f 726d 730a 2020 2020 666f  waveforms.    fo
-00012cb0: 7220 6969 2069 6e20 7261 6e67 6528 6e62  r ii in range(nb
-00012cc0: 7472 6961 6c29 3a0a 2020 2020 2020 2020  trial):.        
-00012cd0: 6e74 203d 2074 7665 6320 2a20 4570 735b  nt = tvec * Eps[
-00012ce0: 6969 5d0a 2020 2020 2020 2020 7320 3d20  ii].        s = 
-00012cf0: 6e70 2e69 6e74 6572 7028 783d 7476 6563  np.interp(x=tvec
-00012d00: 2c20 7870 3d6e 742c 2066 703d 6375 7229  , xp=nt, fp=cur)
-00012d10: 0a20 2020 2020 2020 2077 6176 6566 6f72  .        wavefor
-00012d20: 6d73 5b69 6920 2b20 312c 203a 5d20 3d20  ms[ii + 1, :] = 
-00012d30: 730a 2020 2020 636f 6620 3d20 6e70 2e63  s.    cof = np.c
-00012d40: 6f72 7263 6f65 6628 7761 7665 666f 726d  orrcoef(waveform
-00012d50: 7329 5b30 5d5b 313a 5d0a 0a20 2020 2023  s)[0][1:]..    #
-00012d60: 2066 696e 6420 7468 6520 6d61 7869 6d75   find the maximu
-00012d70: 6d20 636f 7272 656c 6174 696f 6e20 636f  m correlation co
-00012d80: 6566 6669 6369 656e 740a 2020 2020 696d  efficient.    im
-00012d90: 6178 203d 206e 702e 6e61 6e61 7267 6d61  ax = np.nanargma
-00012da0: 7828 636f 6629 0a20 2020 2069 6620 696d  x(cof).    if im
-00012db0: 6178 203e 3d20 6c65 6e28 4570 7329 202d  ax >= len(Eps) -
-00012dc0: 2032 3a0a 2020 2020 2020 2020 696d 6178   2:.        imax
-00012dd0: 203d 2069 6d61 7820 2d20 320a 2020 2020   = imax - 2.    
-00012de0: 6966 2069 6d61 7820 3c20 323a 0a20 2020  if imax < 2:.   
-00012df0: 2020 2020 2069 6d61 7820 3d20 696d 6178       imax = imax
-00012e00: 202b 2032 0a0a 2020 2020 2320 5072 6f63   + 2..    # Proc
-00012e10: 6565 6420 746f 2074 6865 2073 6563 6f6e  eed to the secon
-00012e20: 6420 7374 6570 2074 6f20 6765 7420 6120  d step to get a 
-00012e30: 6d6f 7265 2070 7265 6369 7365 2064 762f  more precise dv/
-00012e40: 7620 6d65 6173 7572 656d 656e 740a 2020  v measurement.  
-00012e50: 2020 6474 6669 6e65 7220 3d20 6e70 2e6c    dtfiner = np.l
-00012e60: 696e 7370 6163 6528 4570 735b 696d 6178  inspace(Eps[imax
-00012e70: 202d 2032 5d2c 2045 7073 5b69 6d61 7820   - 2], Eps[imax 
-00012e80: 2b20 325d 2c20 6e62 7472 6961 6c29 0a20  + 2], nbtrial). 
-00012e90: 2020 2023 206e 636f 6620 2020 203d 206e     # ncof    = n
-00012ea0: 702e 7a65 726f 7328 6474 6669 6e65 722e  p.zeros(dtfiner.
-00012eb0: 7368 6170 652c 6474 7970 653d 6e70 2e66  shape,dtype=np.f
-00012ec0: 6c6f 6174 3332 290a 2020 2020 7761 7665  loat32).    wave
-00012ed0: 666f 726d 7320 3d20 6e70 2e7a 6572 6f73  forms = np.zeros
-00012ee0: 2828 6e62 7472 6961 6c20 2b20 312c 206c  ((nbtrial + 1, l
-00012ef0: 656e 2872 6566 2929 290a 2020 2020 7761  en(ref))).    wa
-00012f00: 7665 666f 726d 735b 302c 203a 5d20 3d20  veforms[0, :] = 
-00012f10: 7265 660a 2020 2020 666f 7220 6969 2069  ref.    for ii i
-00012f20: 6e20 7261 6e67 6528 6c65 6e28 6474 6669  n range(len(dtfi
-00012f30: 6e65 7229 293a 0a20 2020 2020 2020 206e  ner)):.        n
-00012f40: 7420 3d20 7476 6563 202a 2064 7466 696e  t = tvec * dtfin
-00012f50: 6572 5b69 695d 0a20 2020 2020 2020 2073  er[ii].        s
-00012f60: 203d 206e 702e 696e 7465 7270 2878 3d74   = np.interp(x=t
-00012f70: 7665 632c 2078 703d 6e74 2c20 6670 3d63  vec, xp=nt, fp=c
-00012f80: 7572 290a 2020 2020 2020 2020 7761 7665  ur).        wave
-00012f90: 666f 726d 735b 6969 202b 2031 2c20 3a5d  forms[ii + 1, :]
-00012fa0: 203d 2073 0a20 2020 206e 636f 6620 3d20   = s.    ncof = 
-00012fb0: 6e70 2e63 6f72 7263 6f65 6628 7761 7665  np.corrcoef(wave
-00012fc0: 666f 726d 7329 5b30 5d5b 313a 5d0a 2020  forms)[0][1:].  
-00012fd0: 2020 6363 203d 206e 702e 6d61 7828 6e63    cc = np.max(nc
-00012fe0: 6f66 2920 2023 2046 696e 6420 6d61 7869  of)  # Find maxi
-00012ff0: 6d75 6d20 636f 7272 656c 6174 696f 6e20  mum correlation 
-00013000: 636f 6566 6669 6369 656e 7420 6f66 2074  coefficient of t
-00013010: 6865 2072 6566 696e 6564 2020 616e 616c  he refined  anal
-00013020: 7973 6973 0a20 2020 2064 7620 3d20 3130  ysis.    dv = 10
-00013030: 302e 3020 2a20 6474 6669 6e65 725b 6e70  0.0 * dtfiner[np
-00013040: 2e61 7267 6d61 7828 6e63 6f66 295d 202d  .argmax(ncof)] -
-00013050: 2031 3030 2020 2320 4d75 6c74 6970 6c79   100  # Multiply
-00013060: 2062 7920 3130 3020 746f 2063 6f6e 7665   by 100 to conve
-00013070: 7274 2074 6f20 7065 7263 656e 7461 6765  rt to percentage
-00013080: 2028 4570 7369 6c6f 6e20 3d20 2d64 742f   (Epsilon = -dt/
-00013090: 7420 3d20 6476 2f76 290a 0a20 2020 2023  t = dv/v)..    #
-000130a0: 2045 7272 6f72 2063 6f6d 7075 7461 7469   Error computati
-000130b0: 6f6e 2062 6173 6564 206f 6e20 5765 6176  on based on Weav
-000130c0: 6572 2065 7420 616c 2028 3230 3131 292c  er et al (2011),
-000130d0: 204f 6e20 7468 6520 7072 6563 6973 696f   On the precisio
-000130e0: 6e20 6f66 206e 6f69 7365 2d63 6f72 7265  n of noise-corre
-000130f0: 6c61 7469 6f6e 2069 6e74 6572 6665 726f  lation interfero
-00013100: 6d65 7472 792c 0a20 2020 2023 2047 656f  metry,.    # Geo
-00013110: 7068 7973 2e20 4a2e 2049 6e74 2e2c 2031  phys. J. Int., 1
-00013120: 3835 2833 290a 2020 2020 5420 3d20 3120  85(3).    T = 1 
-00013130: 2f20 2866 6d61 7820 2d20 666d 696e 290a  / (fmax - fmin).
-00013140: 2020 2020 5820 3d20 6363 0a20 2020 2077      X = cc.    w
-00013150: 6320 3d20 6e70 2e70 6920 2a20 2866 6d69  c = np.pi * (fmi
-00013160: 6e20 2b20 666d 6178 290a 2020 2020 7431  n + fmax).    t1
-00013170: 203d 206e 702e 6d69 6e28 5b74 6d69 6e2c   = np.min([tmin,
-00013180: 2074 6d61 785d 290a 2020 2020 7432 203d   tmax]).    t2 =
-00013190: 206e 702e 6d61 7828 5b74 6d69 6e2c 2074   np.max([tmin, t
-000131a0: 6d61 785d 290a 2020 2020 6572 726f 7220  max]).    error 
-000131b0: 3d20 3130 3020 2a20 280a 2020 2020 2020  = 100 * (.      
-000131c0: 2020 6e70 2e73 7172 7428 3120 2d20 582a    np.sqrt(1 - X*
-000131d0: 2a32 2920 2f20 2832 202a 2058 2920 2a20  *2) / (2 * X) * 
-000131e0: 6e70 2e73 7172 7428 2836 202a 206e 702e  np.sqrt((6 * np.
-000131f0: 7371 7274 286e 702e 7069 202f 2032 2920  sqrt(np.pi / 2) 
-00013200: 2a20 5429 202f 2028 7763 2a2a 3220 2a20  * T) / (wc**2 * 
-00013210: 2874 322a 2a33 202d 2074 312a 2a33 2929  (t2**3 - t1**3))
-00013220: 290a 2020 2020 290a 0a20 2020 2072 6574  ).    )..    ret
-00013230: 7572 6e20 6476 2c20 6572 726f 722c 2063  urn dv, error, c
-00013240: 632c 2063 6470 0a0a 0a64 6566 2064 7477  c, cdp...def dtw
-00013250: 5f64 7676 2872 6566 2c20 6375 722c 2070  _dvv(ref, cur, p
-00013260: 6172 612c 206d 6178 4c61 672c 2062 2c20  ara, maxLag, b, 
-00013270: 6469 7265 6374 696f 6e29 3a0a 2020 2020  direction):.    
-00013280: 2222 220a 2020 2020 4479 6e61 6d69 6320  """.    Dynamic 
-00013290: 7469 6d65 2077 6172 7069 6e67 2066 6f72  time warping for
-000132a0: 2064 762f 7620 6573 7469 6d61 7469 6f6e   dv/v estimation
-000132b0: 2e0a 0a20 2020 2050 4152 414d 4554 4552  ...    PARAMETER
-000132c0: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
-000132d0: 2d2d 2d2d 2d2d 2d0a 2020 2020 7265 6620  -------.    ref 
-000132e0: 3a20 7265 6665 7265 6e63 6520 7369 676e  : reference sign
-000132f0: 616c 2028 6e70 2e61 7272 6179 2c20 7369  al (np.array, si
-00013300: 7a65 204e 290a 2020 2020 6375 7220 3a20  ze N).    cur : 
-00013310: 6375 7272 656e 7420 7369 676e 616c 2028  current signal (
-00013320: 6e70 2e61 7272 6179 2c20 7369 7a65 204e  np.array, size N
-00013330: 290a 2020 2020 7061 7261 3a20 6469 6374  ).    para: dict
-00013340: 2063 6f6e 7461 696e 696e 6720 7573 6566   containing usef
-00013350: 756c 2070 6172 616d 6574 6572 7320 6162  ul parameters ab
-00013360: 6f75 7420 7468 6520 6461 7461 2077 696e  out the data win
-00013370: 646f 7720 616e 6420 7461 7267 6574 6564  dow and targeted
-00013380: 2066 7265 7175 656e 6379 0a20 2020 206d   frequency.    m
-00013390: 6178 4c61 6720 3a20 6d61 7820 6e75 6d62  axLag : max numb
-000133a0: 6572 206f 6620 706f 696e 7473 2074 6f20  er of points to 
-000133b0: 7365 6172 6368 2066 6f72 7761 7264 2061  search forward a
-000133c0: 6e64 2062 6163 6b77 6172 642e 0a20 2020  nd backward..   
-000133d0: 2020 2020 2020 2020 2053 7567 6765 7374           Suggest
-000133e0: 2073 6574 7469 6e67 2069 7420 6c61 7267   setting it larg
-000133f0: 6572 2069 6620 7769 6e64 6f77 2069 7320  er if window is 
-00013400: 7365 7420 6c61 7267 6572 2e0a 2020 2020  set larger..    
-00013410: 6220 3a20 622d 7661 6c75 6520 746f 206c  b : b-value to l
-00013420: 696d 6974 2073 7472 6169 6e2c 2077 6869  imit strain, whi
-00013430: 6368 2069 7320 746f 206c 696d 6974 2074  ch is to limit t
-00013440: 6865 206d 6178 696d 756d 2076 656c 6f63  he maximum veloc
-00013450: 6974 7920 7065 7274 7572 6261 7469 6f6e  ity perturbation
-00013460: 2e0a 2020 2020 2020 2020 2020 2020 5365  ..            Se
-00013470: 6520 6571 7561 7469 6f6e 2031 3120 696e  e equation 11 in
-00013480: 2028 4d69 6b65 7365 6c6c 2065 7420 616c   (Mikesell et al
-00013490: 2e20 3230 3135 290a 2020 2020 6469 7265  . 2015).    dire
-000134a0: 6374 696f 6e3a 2064 6972 6563 7469 6f6e  ction: direction
-000134b0: 2074 6f20 6163 6375 6d75 6c61 7465 2065   to accumulate e
-000134c0: 7272 6f72 7320 2831 3d66 6f72 7761 7264  rrors (1=forward
-000134d0: 2c20 2d31 3d62 6163 6b77 6172 6429 0a20  , -1=backward). 
-000134e0: 2020 2052 4554 5552 4e53 3a0a 2020 2020     RETURNS:.    
-000134f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00013500: 2d2d 0a20 2020 202d 6d30 203a 2065 7374  --.    -m0 : est
-00013510: 696d 6174 6564 2064 762f 760a 2020 2020  imated dv/v.    
-00013520: 656d 3020 3a20 6572 726f 7220 6f66 2064  em0 : error of d
-00013530: 762f 7620 6573 7469 6d61 7469 6f6e 0a0a  v/v estimation..
-00013540: 2020 2020 4f72 6967 696e 616c 2062 7920      Original by 
-00013550: 4469 2059 616e 670a 2020 2020 4c61 7374  Di Yang.    Last
-00013560: 206d 6f64 6966 6965 6420 6279 2044 796c   modified by Dyl
-00013570: 616e 204d 696b 6573 656c 6c20 2832 3520  an Mikesell (25 
-00013580: 4665 622e 2032 3031 3529 0a20 2020 2054  Feb. 2015).    T
-00013590: 7261 6e73 6c61 7465 6420 746f 2070 7974  ranslated to pyt
-000135a0: 686f 6e20 6279 2054 696d 2043 6c65 6d65  hon by Tim Cleme
-000135b0: 6e74 7320 2831 3720 4175 672e 2032 3031  nts (17 Aug. 201
-000135c0: 3829 0a20 2020 2022 2222 0a20 2020 2074  8).    """.    t
-000135d0: 7769 6e20 3d20 7061 7261 5b22 7477 696e  win = para["twin
-000135e0: 225d 0a20 2020 2064 7420 3d20 7061 7261  "].    dt = para
-000135f0: 5b22 6474 225d 0a20 2020 2074 6d69 6e20  ["dt"].    tmin 
-00013600: 3d20 6e70 2e6d 696e 2874 7769 6e29 0a20  = np.min(twin). 
-00013610: 2020 2074 6d61 7820 3d20 6e70 2e6d 6178     tmax = np.max
-00013620: 2874 7769 6e29 0a20 2020 2074 7665 6374  (twin).    tvect
-00013630: 203d 206e 702e 6172 616e 6765 2874 6d69   = np.arange(tmi
-00013640: 6e2c 2074 6d61 782c 2064 7429 0a0a 2020  n, tmax, dt)..  
-00013650: 2020 2320 7365 7475 7020 6f74 6865 7220    # setup other 
-00013660: 7061 7261 6d65 7465 7273 0a20 2020 206e  parameters.    n
-00013670: 7074 7320 3d20 6c65 6e28 7265 6629 2020  pts = len(ref)  
-00013680: 2320 6e75 6d62 6572 206f 6620 7469 6d65  # number of time
-00013690: 2073 616d 706c 6573 0a0a 2020 2020 2320   samples..    # 
-000136a0: 636f 6d70 7574 6520 6572 726f 7220 6675  compute error fu
-000136b0: 6e63 7469 6f6e 206f 7665 7220 6c61 6773  nction over lags
-000136c0: 2c20 7768 6963 6820 6973 2069 6e64 6570  , which is indep
-000136d0: 656e 6465 6e74 206f 6620 7374 7261 696e  endent of strain
-000136e0: 206c 696d 6974 2027 6227 2e0a 2020 2020   limit 'b'..    
-000136f0: 6572 7220 3d20 636f 6d70 7574 6545 7272  err = computeErr
-00013700: 6f72 4675 6e63 7469 6f6e 2863 7572 2c20  orFunction(cur, 
-00013710: 7265 662c 206e 7074 732c 206d 6178 4c61  ref, npts, maxLa
-00013720: 6729 0a0a 2020 2020 2320 6469 7265 6374  g)..    # direct
-00013730: 696f 6e20 746f 2061 6363 756d 756c 6174  ion to accumulat
-00013740: 6520 6572 726f 7273 2028 313d 666f 7277  e errors (1=forw
-00013750: 6172 642c 202d 313d 6261 636b 7761 7264  ard, -1=backward
-00013760: 290a 2020 2020 6469 7374 203d 2061 6363  ).    dist = acc
-00013770: 756d 756c 6174 6545 7272 6f72 4675 6e63  umulateErrorFunc
-00013780: 7469 6f6e 2864 6972 6563 7469 6f6e 2c20  tion(direction, 
-00013790: 6572 722c 206e 7074 732c 206d 6178 4c61  err, npts, maxLa
-000137a0: 672c 2062 290a 2020 2020 7374 6261 7220  g, b).    stbar 
-000137b0: 3d20 6261 636b 7472 6163 6b44 6973 7461  = backtrackDista
-000137c0: 6e63 6546 756e 6374 696f 6e28 2d31 202a  nceFunction(-1 *
-000137d0: 2064 6972 6563 7469 6f6e 2c20 6469 7374   direction, dist
-000137e0: 2c20 6572 722c 202d 6d61 784c 6167 2c20  , err, -maxLag, 
-000137f0: 6229 0a20 2020 2073 7462 6172 5469 6d65  b).    stbarTime
-00013800: 203d 2073 7462 6172 202a 2064 7420 2023   = stbar * dt  #
-00013810: 2063 6f6e 7665 7274 2066 726f 6d20 7361   convert from sa
-00013820: 6d70 6c65 7320 746f 2074 696d 650a 0a20  mples to time.. 
-00013830: 2020 2023 2063 7574 2074 6865 2066 6972     # cut the fir
-00013840: 7374 2061 6e64 206c 6173 7420 3525 2066  st and last 5% f
-00013850: 6f72 2062 6574 7465 7220 7265 6772 6573  or better regres
-00013860: 7369 6f6e 0a20 2020 2069 6e64 7820 3d20  sion.    indx = 
-00013870: 6e70 2e77 6865 7265 2828 7476 6563 7420  np.where((tvect 
-00013880: 3e3d 2030 2e30 3520 2a20 6e70 7473 202a  >= 0.05 * npts *
-00013890: 2064 7429 2026 2028 7476 6563 7420 3c3d   dt) & (tvect <=
-000138a0: 2030 2e39 3520 2a20 6e70 7473 202a 2064   0.95 * npts * d
-000138b0: 7429 295b 305d 0a0a 2020 2020 2320 6c69  t))[0]..    # li
-000138c0: 6e65 6172 2072 6567 7265 7373 696f 6e20  near regression 
-000138d0: 746f 2067 6574 2064 762f 760a 2020 2020  to get dv/v.    
-000138e0: 6966 206e 7074 7320 3e20 323a 0a20 2020  if npts > 2:.   
-000138f0: 2020 2020 2023 2077 6569 6768 7473 0a20       # weights. 
-00013900: 2020 2020 2020 2077 203d 206e 702e 6f6e         w = np.on
-00013910: 6573 286e 7074 7329 0a20 2020 2020 2020  es(npts).       
-00013920: 2023 206d 2c20 612c 2065 6d2c 2065 6120   # m, a, em, ea 
-00013930: 3d20 6c69 6e65 6172 5f72 6567 7265 7373  = linear_regress
-00013940: 696f 6e28 7469 6d65 5f61 7869 735b 696e  ion(time_axis[in
-00013950: 6478 5d2c 2064 656c 7461 5f74 5b69 6e64  dx], delta_t[ind
-00013960: 785d 2c20 772c 2069 6e74 6572 6365 7074  x], w, intercept
-00013970: 5f6f 7269 6769 6e3d 4661 6c73 6529 0a20  _origin=False). 
-00013980: 2020 2020 2020 206d 302c 2065 6d30 203d         m0, em0 =
-00013990: 206c 696e 6561 725f 7265 6772 6573 7369   linear_regressi
-000139a0: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
-000139b0: 7476 6563 742e 666c 6174 7465 6e28 295b  tvect.flatten()[
-000139c0: 696e 6478 5d2c 0a20 2020 2020 2020 2020  indx],.         
-000139d0: 2020 2073 7462 6172 5469 6d65 2e66 6c61     stbarTime.fla
-000139e0: 7474 656e 2829 5b69 6e64 785d 2c0a 2020  tten()[indx],.  
-000139f0: 2020 2020 2020 2020 2020 772e 666c 6174            w.flat
-00013a00: 7465 6e28 295b 696e 6478 5d2c 0a20 2020  ten()[indx],.   
-00013a10: 2020 2020 2020 2020 2069 6e74 6572 6365           interce
-00013a20: 7074 5f6f 7269 6769 6e3d 5472 7565 2c0a  pt_origin=True,.
-00013a30: 2020 2020 2020 2020 290a 0a20 2020 2065          )..    e
-00013a40: 6c73 653a 0a20 2020 2020 2020 206c 6f67  lse:.        log
-00013a50: 6765 722e 6465 6275 6728 226e 6f74 2065  ger.debug("not e
-00013a60: 6e6f 7567 6820 706f 696e 7473 2074 6f20  nough points to 
-00013a70: 6573 7469 6d61 7465 2064 762f 7620 666f  estimate dv/v fo
-00013a80: 7220 6474 7722 290a 2020 2020 2020 2020  r dtw").        
-00013a90: 6d30 203d 2030 0a20 2020 2020 2020 2065  m0 = 0.        e
-00013aa0: 6d30 203d 2030 0a0a 2020 2020 7265 7475  m0 = 0..    retu
-00013ab0: 726e 206d 3020 2a20 3130 302c 2065 6d30  rn m0 * 100, em0
-00013ac0: 202a 2031 3030 2c20 6469 7374 0a0a 0a64   * 100, dist...d
-00013ad0: 6566 206d 7763 735f 6476 7628 7265 662c  ef mwcs_dvv(ref,
-00013ae0: 2063 7572 2c20 6d6f 7669 6e67 5f77 696e   cur, moving_win
-00013af0: 646f 775f 6c65 6e67 7468 2c20 736c 6964  dow_length, slid
-00013b00: 655f 7374 6570 2c20 7061 7261 2c20 736d  e_step, para, sm
-00013b10: 6f6f 7468 696e 675f 6861 6c66 5f77 696e  oothing_half_win
-00013b20: 3d35 293a 0a20 2020 2022 2222 0a20 2020  =5):.    """.   
-00013b30: 204d 6f76 696e 6720 5769 6e64 6f77 2043   Moving Window C
-00013b40: 726f 7373 2053 7065 6374 7275 6d20 6d65  ross Spectrum me
-00013b50: 7468 6f64 2074 6f20 6d65 6173 7572 6520  thod to measure 
-00013b60: 6476 2f76 2028 7265 6c79 696e 6720 6f6e  dv/v (relying on
-00013b70: 2070 6869 3d32 2a70 692a 662a 7420 696e   phi=2*pi*f*t in
-00013b80: 2066 7265 7120 646f 6d61 696e 290a 0a20   freq domain).. 
-00013b90: 2020 2050 4152 414d 4554 4552 533a 0a20     PARAMETERS:. 
-00013ba0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
-00013bb0: 2d2d 2d0a 2020 2020 7265 663a 2052 6566  ---.    ref: Ref
-00013bc0: 6572 656e 6365 2077 6176 6566 6f72 6d20  erence waveform 
-00013bd0: 286e 702e 6e64 6172 7261 792c 2073 697a  (np.ndarray, siz
-00013be0: 6520 4e29 0a20 2020 2063 7572 3a20 4375  e N).    cur: Cu
-00013bf0: 7272 656e 7420 7761 7665 666f 726d 2028  rrent waveform (
-00013c00: 6e70 2e6e 6461 7272 6179 2c20 7369 7a65  np.ndarray, size
-00013c10: 204e 290a 2020 2020 6d6f 7669 6e67 5f77   N).    moving_w
-00013c20: 696e 646f 775f 6c65 6e67 7468 3a20 6d6f  indow_length: mo
-00013c30: 7669 6e67 2077 696e 646f 7720 6c65 6e67  ving window leng
-00013c40: 7468 2074 6f20 6361 6c63 756c 6174 6520  th to calculate 
-00013c50: 6372 6f73 732d 7370 6563 7472 756d 2028  cross-spectrum (
-00013c60: 6e70 2e66 6c6f 6174 2c20 696e 2073 6563  np.float, in sec
-00013c70: 290a 2020 2020 736c 6964 655f 7374 6570  ).    slide_step
-00013c80: 3a20 7374 6570 7320 696e 2074 696d 6520  : steps in time 
-00013c90: 746f 2073 6869 6674 2074 6865 206d 6f76  to shift the mov
-00013ca0: 696e 6720 7769 6e64 6f77 2028 6e70 2e66  ing window (np.f
-00013cb0: 6c6f 6174 2c20 696e 2073 6563 6f6e 6473  loat, in seconds
-00013cc0: 290a 2020 2020 7061 7261 3a20 6120 6469  ).    para: a di
-00013cd0: 6374 2063 6f6e 7461 696e 696e 6720 7061  ct containing pa
-00013ce0: 7261 6d65 7465 7273 2061 626f 7574 2069  rameters about i
-00013cf0: 6e70 7574 2064 6174 6120 7769 6e64 6f77  nput data window
-00013d00: 2061 6e64 2066 7265 7175 656e 6379 2069   and frequency i
-00013d10: 6e66 6f2c 2069 6e63 6c75 6469 6e67 0a20  nfo, including. 
-00013d20: 2020 2020 2020 2064 656c 7461 2d3e 5468         delta->Th
-00013d30: 6520 7361 6d70 6c69 6e67 2072 6174 6520  e sampling rate 
-00013d40: 6f66 2074 6865 2069 6e70 7574 2074 696d  of the input tim
-00013d50: 6573 6572 6965 7320 2869 6e20 487a 290a  eseries (in Hz).
-00013d60: 2020 2020 2020 2020 7769 6e64 6f77 2d3e          window->
-00013d70: 2054 6865 2074 6172 6765 7420 7769 6e64   The target wind
-00013d80: 6f77 2066 6f72 206d 6561 7375 7269 6e67  ow for measuring
-00013d90: 2064 742f 740a 2020 2020 2020 2020 6672   dt/t.        fr
-00013da0: 6571 2d3e 2054 6865 2066 7265 7175 656e  eq-> The frequen
-00013db0: 6379 2062 6f75 6e64 2074 6f20 636f 6d70  cy bound to comp
-00013dc0: 7574 6520 7468 6520 6465 7068 6173 696e  ute the dephasin
-00013dd0: 6720 2869 6e20 487a 290a 2020 2020 2020  g (in Hz).      
-00013de0: 2020 746d 696e 3a20 5468 6520 6c65 6674    tmin: The left
-00013df0: 6d6f 7374 2074 696d 6520 6c61 6720 2875  most time lag (u
-00013e00: 7365 6420 746f 2063 6f6d 7075 7465 2074  sed to compute t
-00013e10: 6865 2022 7469 6d65 206c 6167 7320 6172  he "time lags ar
-00013e20: 7261 7922 290a 2020 2020 736d 6f6f 7468  ray").    smooth
-00013e30: 696e 675f 6861 6c66 5f77 696e 3a20 4966  ing_half_win: If
-00013e40: 2064 6966 6665 7265 6e74 2066 726f 6d20   different from 
-00013e50: 302c 2064 6566 696e 6573 2074 6865 2068  0, defines the h
-00013e60: 616c 6620 6c65 6e67 7468 206f 6620 7468  alf length of th
-00013e70: 6520 736d 6f6f 7468 696e 6720 6861 6e6e  e smoothing hann
-00013e80: 696e 6720 7769 6e64 6f77 2e0a 0a20 2020  ing window...   
-00013e90: 2052 4554 5552 4e53 3a0a 2020 2020 2d2d   RETURNS:.    --
-00013ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00013eb0: 0a20 2020 2074 696d 655f 6178 6973 3a20  .    time_axis: 
-00013ec0: 7468 6520 6365 6e74 7261 6c20 7469 6d65  the central time
-00013ed0: 7320 6f66 2074 6865 2077 696e 646f 7773  s of the windows
-00013ee0: 2e0a 2020 2020 6465 6c74 615f 743a 2064  ..    delta_t: d
-00013ef0: 740a 2020 2020 6465 6c74 615f 6572 723a  t.    delta_err:
-00013f00: 6572 726f 720a 2020 2020 6465 6c74 615f  error.    delta_
-00013f10: 6d63 6f68 3a20 6d65 616e 2063 6f68 6572  mcoh: mean coher
-00013f20: 656e 6365 0a0a 2020 2020 436f 7069 6564  ence..    Copied
-00013f30: 2066 726f 6d20 4d53 4e6f 6973 6520 2868   from MSNoise (h
-00013f40: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00013f50: 6d2f 524f 4265 6c67 6975 6d2f 4d53 4e6f  m/ROBelgium/MSNo
-00013f60: 6973 652f 7472 6565 2f6d 6173 7465 722f  ise/tree/master/
-00013f70: 6d73 6e6f 6973 6529 0a20 2020 204d 6f64  msnoise).    Mod
-00013f80: 6966 6965 6420 6279 2043 6865 6e67 7869  ified by Chengxi
-00013f90: 6e20 4a69 616e 670a 2020 2020 2222 220a  n Jiang.    """.
-00013fa0: 2020 2020 2320 636f 6d6d 6f6e 2076 6172      # common var
-00013fb0: 6961 626c 6573 0a20 2020 2074 7769 6e20  iables.    twin 
-00013fc0: 3d20 7061 7261 5b22 7477 696e 225d 0a20  = para["twin"]. 
-00013fd0: 2020 2066 7265 7120 3d20 7061 7261 5b22     freq = para["
-00013fe0: 6672 6571 225d 0a20 2020 2064 7420 3d20  freq"].    dt = 
-00013ff0: 7061 7261 5b22 6474 225d 0a20 2020 2074  para["dt"].    t
-00014000: 6d69 6e20 3d20 6e70 2e6d 696e 2874 7769  min = np.min(twi
-00014010: 6e29 0a20 2020 2066 6d69 6e20 3d20 6e70  n).    fmin = np
-00014020: 2e6d 696e 2866 7265 7129 0a20 2020 2066  .min(freq).    f
-00014030: 6d61 7820 3d20 6e70 2e6d 6178 2866 7265  max = np.max(fre
-00014040: 7129 0a0a 2020 2020 2320 7061 7261 6d65  q)..    # parame
-00014050: 7465 7220 696e 6974 6961 6c69 7a65 0a20  ter initialize. 
-00014060: 2020 2064 656c 7461 5f74 203d 205b 5d0a     delta_t = [].
-00014070: 2020 2020 6465 6c74 615f 6572 7220 3d20      delta_err = 
-00014080: 5b5d 0a20 2020 2064 656c 7461 5f6d 636f  [].    delta_mco
-00014090: 6820 3d20 5b5d 0a20 2020 2074 696d 655f  h = [].    time_
-000140a0: 6178 6973 203d 205b 5d0a 0a20 2020 2023  axis = []..    #
-000140b0: 2069 6e66 6f20 6f6e 2074 6865 206d 6f76   info on the mov
-000140c0: 696e 6720 7769 6e64 6f77 0a20 2020 2077  ing window.    w
-000140d0: 696e 646f 775f 6c65 6e67 7468 5f73 616d  indow_length_sam
-000140e0: 706c 6573 203d 206e 702e 696e 7428 6d6f  ples = np.int(mo
-000140f0: 7669 6e67 5f77 696e 646f 775f 6c65 6e67  ving_window_leng
-00014100: 7468 202f 2064 7429 0a20 2020 2070 6164  th / dt).    pad
-00014110: 6420 3d20 696e 7428 3220 2a2a 2028 6e65  d = int(2 ** (ne
-00014120: 7874 706f 7732 2877 696e 646f 775f 6c65  xtpow2(window_le
-00014130: 6e67 7468 5f73 616d 706c 6573 2920 2b20  ngth_samples) + 
-00014140: 3229 290a 2020 2020 636f 756e 7420 3d20  2)).    count = 
-00014150: 300a 2020 2020 7470 203d 2063 6f73 696e  0.    tp = cosin
-00014160: 655f 7461 7065 7228 7769 6e64 6f77 5f6c  e_taper(window_l
-00014170: 656e 6774 685f 7361 6d70 6c65 732c 2030  ength_samples, 0
-00014180: 2e31 3529 0a0a 2020 2020 6d69 6e69 6e64  .15)..    minind
-00014190: 203d 2030 0a20 2020 206d 6178 696e 6420   = 0.    maxind 
-000141a0: 3d20 7769 6e64 6f77 5f6c 656e 6774 685f  = window_length_
-000141b0: 7361 6d70 6c65 730a 0a20 2020 2023 206c  samples..    # l
-000141c0: 6f6f 7020 7468 726f 7567 6820 616c 6c20  oop through all 
-000141d0: 7375 622d 7769 6e64 6f77 730a 2020 2020  sub-windows.    
-000141e0: 7768 696c 6520 6d61 7869 6e64 203c 3d20  while maxind <= 
-000141f0: 6c65 6e28 7265 6629 3a0a 2020 2020 2020  len(ref):.      
-00014200: 2020 6363 6920 3d20 6375 725b 6d69 6e69    cci = cur[mini
-00014210: 6e64 3a6d 6178 696e 645d 0a20 2020 2020  nd:maxind].     
-00014220: 2020 2063 6369 203d 2073 6369 7079 2e73     cci = scipy.s
-00014230: 6967 6e61 6c2e 6465 7472 656e 6428 6363  ignal.detrend(cc
-00014240: 692c 2074 7970 653d 226c 696e 6561 7222  i, type="linear"
-00014250: 290a 2020 2020 2020 2020 6363 6920 2a3d  ).        cci *=
-00014260: 2074 700a 0a20 2020 2020 2020 2063 7269   tp..        cri
-00014270: 203d 2072 6566 5b6d 696e 696e 643a 6d61   = ref[minind:ma
-00014280: 7869 6e64 5d0a 2020 2020 2020 2020 6372  xind].        cr
-00014290: 6920 3d20 7363 6970 792e 7369 676e 616c  i = scipy.signal
-000142a0: 2e64 6574 7265 6e64 2863 7269 2c20 7479  .detrend(cri, ty
-000142b0: 7065 3d22 6c69 6e65 6172 2229 0a20 2020  pe="linear").   
-000142c0: 2020 2020 2063 7269 202a 3d20 7470 0a0a       cri *= tp..
-000142d0: 2020 2020 2020 2020 6d69 6e69 6e64 202b          minind +
-000142e0: 3d20 696e 7428 736c 6964 655f 7374 6570  = int(slide_step
-000142f0: 202f 2064 7429 0a20 2020 2020 2020 206d   / dt).        m
-00014300: 6178 696e 6420 2b3d 2069 6e74 2873 6c69  axind += int(sli
-00014310: 6465 5f73 7465 7020 2f20 6474 290a 0a20  de_step / dt).. 
-00014320: 2020 2020 2020 2023 2064 6f20 6666 740a         # do fft.
-00014330: 2020 2020 2020 2020 6663 7572 203d 2073          fcur = s
-00014340: 6369 7079 2e66 6674 7061 636b 2e66 6674  cipy.fftpack.fft
-00014350: 2863 6369 2c20 6e3d 7061 6464 295b 3a20  (cci, n=padd)[: 
-00014360: 7061 6464 202f 2f20 325d 0a20 2020 2020  padd // 2].     
-00014370: 2020 2066 7265 6620 3d20 7363 6970 792e     fref = scipy.
-00014380: 6666 7470 6163 6b2e 6666 7428 6372 692c  fftpack.fft(cri,
-00014390: 206e 3d70 6164 6429 5b3a 2070 6164 6420   n=padd)[: padd 
-000143a0: 2f2f 2032 5d0a 0a20 2020 2020 2020 2066  // 2]..        f
-000143b0: 6375 7232 203d 206e 702e 7265 616c 2866  cur2 = np.real(f
-000143c0: 6375 7229 202a 2a20 3220 2b20 6e70 2e69  cur) ** 2 + np.i
-000143d0: 6d61 6728 6663 7572 2920 2a2a 2032 0a20  mag(fcur) ** 2. 
-000143e0: 2020 2020 2020 2066 7265 6632 203d 206e         fref2 = n
-000143f0: 702e 7265 616c 2866 7265 6629 202a 2a20  p.real(fref) ** 
-00014400: 3220 2b20 6e70 2e69 6d61 6728 6672 6566  2 + np.imag(fref
-00014410: 2920 2a2a 2032 0a0a 2020 2020 2020 2020  ) ** 2..        
-00014420: 2320 6765 7420 6372 6f73 732d 7370 6563  # get cross-spec
-00014430: 7472 756d 2026 2064 6f20 6669 6c74 6572  trum & do filter
-00014440: 696e 670a 2020 2020 2020 2020 5820 3d20  ing.        X = 
-00014450: 6672 6566 202a 2028 6663 7572 2e63 6f6e  fref * (fcur.con
-00014460: 6a28 2929 0a20 2020 2020 2020 2069 6620  j()).        if 
-00014470: 736d 6f6f 7468 696e 675f 6861 6c66 5f77  smoothing_half_w
-00014480: 696e 2021 3d20 303a 0a20 2020 2020 2020  in != 0:.       
-00014490: 2020 2020 2064 6375 7220 3d20 6e70 2e73       dcur = np.s
-000144a0: 7172 7428 736d 6f6f 7468 2866 6375 7232  qrt(smooth(fcur2
-000144b0: 2c20 7769 6e64 6f77 3d22 6861 6e6e 696e  , window="hannin
-000144c0: 6722 2c20 6861 6c66 5f77 696e 3d73 6d6f  g", half_win=smo
-000144d0: 6f74 6869 6e67 5f68 616c 665f 7769 6e29  othing_half_win)
-000144e0: 290a 2020 2020 2020 2020 2020 2020 6472  ).            dr
-000144f0: 6566 203d 206e 702e 7371 7274 2873 6d6f  ef = np.sqrt(smo
-00014500: 6f74 6828 6672 6566 322c 2077 696e 646f  oth(fref2, windo
-00014510: 773d 2268 616e 6e69 6e67 222c 2068 616c  w="hanning", hal
-00014520: 665f 7769 6e3d 736d 6f6f 7468 696e 675f  f_win=smoothing_
-00014530: 6861 6c66 5f77 696e 2929 0a20 2020 2020  half_win)).     
-00014540: 2020 2020 2020 2058 203d 2073 6d6f 6f74         X = smoot
-00014550: 6828 582c 2077 696e 646f 773d 2268 616e  h(X, window="han
-00014560: 6e69 6e67 222c 2068 616c 665f 7769 6e3d  ning", half_win=
-00014570: 736d 6f6f 7468 696e 675f 6861 6c66 5f77  smoothing_half_w
-00014580: 696e 290a 2020 2020 2020 2020 656c 7365  in).        else
-00014590: 3a0a 2020 2020 2020 2020 2020 2020 6463  :.            dc
-000145a0: 7572 203d 206e 702e 7371 7274 2866 6375  ur = np.sqrt(fcu
-000145b0: 7232 290a 2020 2020 2020 2020 2020 2020  r2).            
-000145c0: 6472 6566 203d 206e 702e 7371 7274 2866  dref = np.sqrt(f
-000145d0: 7265 6632 290a 0a20 2020 2020 2020 2064  ref2)..        d
-000145e0: 6373 203d 206e 702e 6162 7328 5829 0a0a  cs = np.abs(X)..
-000145f0: 2020 2020 2020 2020 2320 4669 6e64 2074          # Find t
-00014600: 6865 2076 616c 7565 7320 7468 6520 6672  he values the fr
-00014610: 6571 7565 6e63 7920 7261 6e67 6520 6f66  equency range of
-00014620: 2069 6e74 6572 6573 740a 2020 2020 2020   interest.      
-00014630: 2020 6672 6571 5f76 6563 203d 2073 6369    freq_vec = sci
-00014640: 7079 2e66 6674 7061 636b 2e66 6674 6672  py.fftpack.fftfr
-00014650: 6571 286c 656e 2858 2920 2a20 322c 2064  eq(len(X) * 2, d
-00014660: 7429 5b3a 2070 6164 6420 2f2f 2032 5d0a  t)[: padd // 2].
-00014670: 2020 2020 2020 2020 696e 6465 785f 7261          index_ra
-00014680: 6e67 6520 3d20 6e70 2e61 7267 7768 6572  nge = np.argwher
-00014690: 6528 6e70 2e6c 6f67 6963 616c 5f61 6e64  e(np.logical_and
-000146a0: 2866 7265 715f 7665 6320 3e3d 2066 6d69  (freq_vec >= fmi
-000146b0: 6e2c 2066 7265 715f 7665 6320 3c3d 2066  n, freq_vec <= f
-000146c0: 6d61 7829 290a 0a20 2020 2020 2020 2023  max))..        #
-000146d0: 2047 6574 2043 6f68 6572 656e 6365 2061   Get Coherence a
-000146e0: 6e64 2069 7473 206d 6561 6e20 7661 6c75  nd its mean valu
-000146f0: 650a 2020 2020 2020 2020 636f 6820 3d20  e.        coh = 
-00014700: 6765 7443 6f68 6572 656e 6365 2864 6373  getCoherence(dcs
-00014710: 2c20 6472 6566 2c20 6463 7572 290a 2020  , dref, dcur).  
-00014720: 2020 2020 2020 6d63 6f68 203d 206e 702e        mcoh = np.
-00014730: 6d65 616e 2863 6f68 5b69 6e64 6578 5f72  mean(coh[index_r
-00014740: 616e 6765 5d29 0a0a 2020 2020 2020 2020  ange])..        
-00014750: 2320 4765 7420 5765 6967 6874 730a 2020  # Get Weights.  
-00014760: 2020 2020 2020 7720 3d20 312e 3020 2f20        w = 1.0 / 
-00014770: 2831 2e30 202f 2028 636f 685b 696e 6465  (1.0 / (coh[inde
-00014780: 785f 7261 6e67 655d 202a 2a20 3229 202d  x_range] ** 2) -
-00014790: 2031 2e30 290a 2020 2020 2020 2020 775b   1.0).        w[
-000147a0: 636f 685b 696e 6465 785f 7261 6e67 655d  coh[index_range]
-000147b0: 203e 3d20 302e 3939 5d20 3d20 312e 3020   >= 0.99] = 1.0 
-000147c0: 2f20 2831 2e30 202f 2030 2e39 3830 3120  / (1.0 / 0.9801 
-000147d0: 2d20 312e 3029 0a20 2020 2020 2020 2077  - 1.0).        w
-000147e0: 203d 206e 702e 7371 7274 2877 202a 206e   = np.sqrt(w * n
-000147f0: 702e 7371 7274 2864 6373 5b69 6e64 6578  p.sqrt(dcs[index
-00014800: 5f72 616e 6765 5d29 290a 2020 2020 2020  _range])).      
-00014810: 2020 7720 3d20 6e70 2e72 6561 6c28 7729    w = np.real(w)
-00014820: 0a0a 2020 2020 2020 2020 2320 4672 6571  ..        # Freq
-00014830: 7565 6e63 7920 6172 7261 793a 0a20 2020  uency array:.   
-00014840: 2020 2020 2076 203d 206e 702e 7265 616c       v = np.real
-00014850: 2866 7265 715f 7665 635b 696e 6465 785f  (freq_vec[index_
-00014860: 7261 6e67 655d 2920 2a20 3220 2a20 6e70  range]) * 2 * np
-00014870: 2e70 690a 0a20 2020 2020 2020 2023 2050  .pi..        # P
-00014880: 6861 7365 3a0a 2020 2020 2020 2020 7068  hase:.        ph
-00014890: 6920 3d20 6e70 2e61 6e67 6c65 2858 290a  i = np.angle(X).
-000148a0: 2020 2020 2020 2020 7068 695b 305d 203d          phi[0] =
-000148b0: 2030 2e30 0a20 2020 2020 2020 2070 6869   0.0.        phi
-000148c0: 203d 206e 702e 756e 7772 6170 2870 6869   = np.unwrap(phi
-000148d0: 290a 2020 2020 2020 2020 7068 6920 3d20  ).        phi = 
-000148e0: 7068 695b 696e 6465 785f 7261 6e67 655d  phi[index_range]
-000148f0: 0a0a 2020 2020 2020 2020 2320 4361 6c63  ..        # Calc
-00014900: 756c 6174 6520 7468 6520 736c 6f70 6520  ulate the slope 
-00014910: 7769 7468 2061 2077 6569 6768 7465 6420  with a weighted 
-00014920: 6c65 6173 7420 7371 7561 7265 206c 696e  least square lin
-00014930: 6561 7220 7265 6772 6573 7369 6f6e 0a20  ear regression. 
-00014940: 2020 2020 2020 2023 2066 6f72 6365 6420         # forced 
-00014950: 7468 726f 7567 6820 7468 6520 6f72 6967  through the orig
-00014960: 696e 3b20 7765 6967 6874 7320 666f 7220  in; weights for 
-00014970: 7468 6520 574c 5320 6d75 7374 2062 6520  the WLS must be 
-00014980: 7468 6520 7661 7269 616e 6365 2021 0a20  the variance !. 
-00014990: 2020 2020 2020 206d 2c20 656d 203d 206c         m, em = l
-000149a0: 696e 6561 725f 7265 6772 6573 7369 6f6e  inear_regression
-000149b0: 2876 2e66 6c61 7474 656e 2829 2c20 7068  (v.flatten(), ph
-000149c0: 692e 666c 6174 7465 6e28 292c 2077 2e66  i.flatten(), w.f
-000149d0: 6c61 7474 656e 2829 290a 2020 2020 2020  latten()).      
-000149e0: 2020 6465 6c74 615f 742e 6170 7065 6e64    delta_t.append
-000149f0: 286d 290a 0a20 2020 2020 2020 2023 2070  (m)..        # p
-00014a00: 7269 6e74 2070 6869 2e73 6861 7065 2c20  rint phi.shape, 
-00014a10: 762e 7368 6170 652c 2077 2e73 6861 7065  v.shape, w.shape
-00014a20: 0a20 2020 2020 2020 2065 203d 206e 702e  .        e = np.
-00014a30: 7375 6d28 2870 6869 202d 206d 202a 2076  sum((phi - m * v
-00014a40: 2920 2a2a 2032 2920 2f20 286e 702e 7369  ) ** 2) / (np.si
-00014a50: 7a65 2876 2920 2d20 3129 0a20 2020 2020  ze(v) - 1).     
-00014a60: 2020 2073 3278 3220 3d20 6e70 2e73 756d     s2x2 = np.sum
-00014a70: 2876 2a2a 3220 2a20 772a 2a32 290a 2020  (v**2 * w**2).  
-00014a80: 2020 2020 2020 7378 3220 3d20 6e70 2e73        sx2 = np.s
-00014a90: 756d 2877 202a 2076 2a2a 3229 0a20 2020  um(w * v**2).   
-00014aa0: 2020 2020 2065 203d 206e 702e 7371 7274       e = np.sqrt
-00014ab0: 2865 202a 2073 3278 3220 2f20 7378 322a  (e * s2x2 / sx2*
-00014ac0: 2a32 290a 0a20 2020 2020 2020 2064 656c  *2)..        del
-00014ad0: 7461 5f65 7272 2e61 7070 656e 6428 6529  ta_err.append(e)
-00014ae0: 0a20 2020 2020 2020 2064 656c 7461 5f6d  .        delta_m
-00014af0: 636f 682e 6170 7065 6e64 286e 702e 7265  coh.append(np.re
-00014b00: 616c 286d 636f 6829 290a 2020 2020 2020  al(mcoh)).      
-00014b10: 2020 7469 6d65 5f61 7869 732e 6170 7065    time_axis.appe
-00014b20: 6e64 2874 6d69 6e20 2b20 6d6f 7669 6e67  nd(tmin + moving
-00014b30: 5f77 696e 646f 775f 6c65 6e67 7468 202f  _window_length /
-00014b40: 2032 2e30 202b 2063 6f75 6e74 202a 2073   2.0 + count * s
-00014b50: 6c69 6465 5f73 7465 7029 0a20 2020 2020  lide_step).     
-00014b60: 2020 2063 6f75 6e74 202b 3d20 310a 0a20     count += 1.. 
-00014b70: 2020 2020 2020 2064 656c 2066 6375 722c         del fcur,
-00014b80: 2066 7265 660a 2020 2020 2020 2020 6465   fref.        de
-00014b90: 6c20 580a 2020 2020 2020 2020 6465 6c20  l X.        del 
-00014ba0: 6672 6571 5f76 6563 0a20 2020 2020 2020  freq_vec.       
-00014bb0: 2064 656c 2069 6e64 6578 5f72 616e 6765   del index_range
-00014bc0: 0a20 2020 2020 2020 2064 656c 2077 2c20  .        del w, 
-00014bd0: 762c 2065 2c20 7332 7832 2c20 7378 322c  v, e, s2x2, sx2,
-00014be0: 206d 2c20 656d 0a0a 2020 2020 6966 206d   m, em..    if m
-00014bf0: 6178 696e 6420 3e20 6c65 6e28 6375 7229  axind > len(cur)
-00014c00: 202b 2069 6e74 2873 6c69 6465 5f73 7465   + int(slide_ste
-00014c10: 7020 2f20 6474 293a 0a20 2020 2020 2020  p / dt):.       
-00014c20: 206c 6f67 6765 722e 6465 6275 6728 2254   logger.debug("T
-00014c30: 6865 206c 6173 7420 7769 6e64 6f77 2077  he last window w
-00014c40: 6173 2074 6f6f 2073 6d61 6c6c 2c20 6275  as too small, bu
-00014c50: 7420 7761 7320 636f 6d70 7574 6564 2229  t was computed")
-00014c60: 0a0a 2020 2020 2320 656e 7375 7265 2061  ..    # ensure a
-00014c70: 6c6c 206d 6174 7269 7820 6172 6520 6e70  ll matrix are np
-00014c80: 2061 7272 6179 0a20 2020 2064 656c 7461   array.    delta
-00014c90: 5f74 203d 206e 702e 6172 7261 7928 6465  _t = np.array(de
-00014ca0: 6c74 615f 7429 0a20 2020 2064 656c 7461  lta_t).    delta
-00014cb0: 5f65 7272 203d 206e 702e 6172 7261 7928  _err = np.array(
-00014cc0: 6465 6c74 615f 6572 7229 0a20 2020 2064  delta_err).    d
-00014cd0: 656c 7461 5f6d 636f 6820 3d20 6e70 2e61  elta_mcoh = np.a
-00014ce0: 7272 6179 2864 656c 7461 5f6d 636f 6829  rray(delta_mcoh)
-00014cf0: 0a20 2020 2074 696d 655f 6178 6973 203d  .    time_axis =
-00014d00: 206e 702e 6172 7261 7928 7469 6d65 5f61   np.array(time_a
-00014d10: 7869 7329 0a0a 2020 2020 2320 7265 6164  xis)..    # read
-00014d20: 7920 666f 7220 6c69 6e65 6172 2072 6567  y for linear reg
-00014d30: 7265 7373 696f 6e0a 2020 2020 6465 6c74  ression.    delt
-00014d40: 615f 6d69 6e63 686f 203d 2030 2e36 350a  a_mincho = 0.65.
-00014d50: 2020 2020 6465 6c74 615f 6d61 7865 7272      delta_maxerr
-00014d60: 203d 2030 2e31 0a20 2020 2064 656c 7461   = 0.1.    delta
-00014d70: 5f6d 6178 6474 203d 2030 2e31 0a20 2020  _maxdt = 0.1.   
-00014d80: 2069 6e64 7831 203d 206e 702e 7768 6572   indx1 = np.wher
-00014d90: 6528 6465 6c74 615f 6d63 6f68 203e 2064  e(delta_mcoh > d
-00014da0: 656c 7461 5f6d 696e 6368 6f29 0a20 2020  elta_mincho).   
-00014db0: 2069 6e64 7832 203d 206e 702e 7768 6572   indx2 = np.wher
-00014dc0: 6528 6465 6c74 615f 6572 7220 3c20 6465  e(delta_err < de
-00014dd0: 6c74 615f 6d61 7865 7272 290a 2020 2020  lta_maxerr).    
-00014de0: 696e 6478 3320 3d20 6e70 2e77 6865 7265  indx3 = np.where
-00014df0: 2864 656c 7461 5f74 203c 2064 656c 7461  (delta_t < delta
-00014e00: 5f6d 6178 6474 290a 0a20 2020 2023 202d  _maxdt)..    # -
-00014e10: 2d2d 2d2d 6669 6e64 2067 6f6f 6420 6474  ----find good dt
-00014e20: 206d 6561 7375 7265 6d65 6e74 732d 2d2d   measurements---
-00014e30: 2d2d 0a20 2020 2069 6e64 7820 3d20 6e70  --.    indx = np
-00014e40: 2e69 6e74 6572 7365 6374 3164 2869 6e64  .intersect1d(ind
-00014e50: 7831 2c20 696e 6478 3229 0a20 2020 2069  x1, indx2).    i
-00014e60: 6e64 7820 3d20 6e70 2e69 6e74 6572 7365  ndx = np.interse
-00014e70: 6374 3164 2869 6e64 782c 2069 6e64 7833  ct1d(indx, indx3
-00014e80: 290a 0a20 2020 2069 6620 6c65 6e28 696e  )..    if len(in
-00014e90: 6478 2920 3e20 323a 0a20 2020 2020 2020  dx) > 2:.       
-00014ea0: 2023 202d 2d2d 2d65 7374 696d 6174 6520   # ----estimate 
-00014eb0: 7765 6967 6874 2066 6f72 2072 6567 7265  weight for regre
-00014ec0: 7373 696f 6e2d 2d2d 2d0a 2020 2020 2020  ssion----.      
-00014ed0: 2020 7720 3d20 3120 2f20 6465 6c74 615f    w = 1 / delta_
-00014ee0: 6572 725b 696e 6478 5d0a 2020 2020 2020  err[indx].      
-00014ef0: 2020 775b 7e6e 702e 6973 6669 6e69 7465    w[~np.isfinite
-00014f00: 2877 295d 203d 2031 2e30 0a0a 2020 2020  (w)] = 1.0..    
-00014f10: 2020 2020 2320 2d2d 2d2d 2d2d 2d2d 2d64      # ---------d
-00014f20: 6f20 6c69 6e65 6172 2072 6567 7265 7373  o linear regress
-00014f30: 696f 6e2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  ion-----------. 
-00014f40: 2020 2020 2020 2023 206d 2c20 612c 2065         # m, a, e
-00014f50: 6d2c 2065 6120 3d20 6c69 6e65 6172 5f72  m, ea = linear_r
-00014f60: 6567 7265 7373 696f 6e28 7469 6d65 5f61  egression(time_a
-00014f70: 7869 735b 696e 6478 5d2c 2064 656c 7461  xis[indx], delta
-00014f80: 5f74 5b69 6e64 785d 2c20 772c 2069 6e74  _t[indx], w, int
-00014f90: 6572 6365 7074 5f6f 7269 6769 6e3d 4661  ercept_origin=Fa
-00014fa0: 6c73 6529 0a20 2020 2020 2020 206d 302c  lse).        m0,
-00014fb0: 2065 6d30 203d 206c 696e 6561 725f 7265   em0 = linear_re
-00014fc0: 6772 6573 7369 6f6e 2874 696d 655f 6178  gression(time_ax
-00014fd0: 6973 5b69 6e64 785d 2c20 6465 6c74 615f  is[indx], delta_
-00014fe0: 745b 696e 6478 5d2c 2077 2c20 696e 7465  t[indx], w, inte
-00014ff0: 7263 6570 745f 6f72 6967 696e 3d54 7275  rcept_origin=Tru
-00015000: 6529 0a0a 2020 2020 656c 7365 3a0a 2020  e)..    else:.  
-00015010: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-00015020: 7567 2822 6e6f 7420 656e 6f75 6768 2070  ug("not enough p
-00015030: 6f69 6e74 7320 746f 2065 7374 696d 6174  oints to estimat
-00015040: 6520 6476 2f76 2066 6f72 206d 7763 7322  e dv/v for mwcs"
-00015050: 290a 2020 2020 2020 2020 6d30 203d 2030  ).        m0 = 0
-00015060: 0a20 2020 2020 2020 2065 6d30 203d 2030  .        em0 = 0
-00015070: 0a0a 2020 2020 7265 7475 726e 202d 6d30  ..    return -m0
-00015080: 202a 2031 3030 2c20 656d 3020 2a20 3130   * 100, em0 * 10
-00015090: 300a 0a0a 6465 6620 5743 435f 6476 7628  0...def WCC_dvv(
-000150a0: 7265 662c 2063 7572 2c20 6d6f 7669 6e67  ref, cur, moving
-000150b0: 5f77 696e 646f 775f 6c65 6e67 7468 2c20  _window_length, 
-000150c0: 736c 6964 655f 7374 6570 2c20 7061 7261  slide_step, para
-000150d0: 293a 0a20 2020 2022 2222 0a20 2020 2057  ):.    """.    W
-000150e0: 696e 646f 7765 6420 6372 6f73 7320 636f  indowed cross co
-000150f0: 7272 656c 6174 696f 6e20 2857 4343 2920  rrelation (WCC) 
-00015100: 666f 7220 6474 206f 7220 6476 2f76 206d  for dt or dv/v m
-00015110: 6573 7572 656d 656e 7420 2853 6e69 6564  esurement (Snied
-00015120: 6572 2065 7420 616c 2e20 3230 3132 290a  er et al. 2012).
-00015130: 0a20 2020 2050 6172 616d 6574 6572 733a  .    Parameters:
-00015140: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
-00015150: 0a20 2020 2072 6566 3a20 5468 6520 2252  .    ref: The "R
-00015160: 6566 6572 656e 6365 2220 7469 6d65 7365  eference" timese
-00015170: 7269 6573 0a20 2020 2063 7572 3a20 5468  ries.    cur: Th
-00015180: 6520 2243 7572 7265 6e74 2220 7469 6d65  e "Current" time
-00015190: 7365 7269 6573 0a20 2020 206d 6f76 696e  series.    movin
-000151a0: 675f 7769 6e64 6f77 5f6c 656e 6774 683a  g_window_length:
-000151b0: 2054 6865 206d 6f76 696e 6720 7769 6e64   The moving wind
-000151c0: 6f77 206c 656e 6774 6820 2869 6e20 7365  ow length (in se
-000151d0: 636f 6e64 7329 0a20 2020 2073 6c69 6465  conds).    slide
-000151e0: 5f73 7465 703a 2054 6865 2073 7465 7020  _step: The step 
-000151f0: 746f 206a 756d 7020 666f 7220 7468 6520  to jump for the 
-00015200: 6d6f 7669 6e67 2077 696e 646f 7720 2869  moving window (i
-00015210: 6e20 7365 636f 6e64 7329 0a20 2020 2070  n seconds).    p
-00015220: 6172 613a 2061 2064 6963 7420 636f 6e74  ara: a dict cont
-00015230: 6169 6e69 6e67 2066 7265 712f 7469 6d65  aining freq/time
-00015240: 2069 6e66 6f20 6f66 2074 6865 2064 6174   info of the dat
-00015250: 6120 6d61 7472 6978 0a0a 2020 2020 5265  a matrix..    Re
-00015260: 7475 726e 733a 0a20 2020 202d 2d2d 2d2d  turns:.    -----
-00015270: 2d2d 2d2d 2d2d 2d0a 2020 2020 7469 6d65  -------.    time
-00015280: 5f61 7869 733a 2063 656e 7472 616c 2074  _axis: central t
-00015290: 696d 6573 206f 6620 7468 6520 6d6f 7669  imes of the movi
-000152a0: 6e67 2077 696e 646f 770a 2020 2020 6465  ng window.    de
-000152b0: 6c74 615f 743a 2064 740a 2020 2020 6465  lta_t: dt.    de
-000152c0: 6c74 615f 6572 723a 2065 7272 6f72 0a20  lta_err: error. 
-000152d0: 2020 2064 656c 7461 5f6d 636f 683a 206d     delta_mcoh: m
-000152e0: 6561 6e20 636f 6865 7265 6e63 6520 666f  ean coherence fo
-000152f0: 7220 6561 6368 2077 696e 646f 770a 0a20  r each window.. 
-00015300: 2020 2057 7269 7474 656e 2062 7920 436f     Written by Co
-00015310: 6e67 636f 6e67 2059 7561 6e20 2831 204a  ngcong Yuan (1 J
-00015320: 756c 792c 2032 3031 3929 0a20 2020 2022  uly, 2019).    "
-00015330: 2222 0a20 2020 2023 2063 6f6d 6d6f 6e20  "".    # common 
-00015340: 7661 7269 6162 6c65 730a 2020 2020 7477  variables.    tw
-00015350: 696e 203d 2070 6172 615b 2274 7769 6e22  in = para["twin"
-00015360: 5d0a 2020 2020 6474 203d 2070 6172 615b  ].    dt = para[
-00015370: 2264 7422 5d0a 2020 2020 746d 696e 203d  "dt"].    tmin =
-00015380: 206e 702e 6d69 6e28 7477 696e 290a 0a20   np.min(twin).. 
-00015390: 2020 2023 2070 6172 616d 6574 6572 2069     # parameter i
-000153a0: 6e69 7469 616c 697a 650a 2020 2020 6465  nitialize.    de
-000153b0: 6c74 615f 7420 3d20 5b5d 0a20 2020 2064  lta_t = [].    d
-000153c0: 656c 7461 5f74 5f63 6f65 6620 3d20 5b5d  elta_t_coef = []
-000153d0: 0a20 2020 2074 696d 655f 6178 6973 203d  .    time_axis =
-000153e0: 205b 5d0a 0a20 2020 2023 2069 6e66 6f20   []..    # info 
-000153f0: 6f6e 2074 6865 206d 6f76 696e 6720 7769  on the moving wi
-00015400: 6e64 6f77 0a20 2020 2077 696e 646f 775f  ndow.    window_
-00015410: 6c65 6e67 7468 5f73 616d 706c 6573 203d  length_samples =
-00015420: 206e 702e 696e 7428 6d6f 7669 6e67 5f77   np.int(moving_w
-00015430: 696e 646f 775f 6c65 6e67 7468 202f 2064  indow_length / d
-00015440: 7429 0a20 2020 2063 6f75 6e74 203d 2030  t).    count = 0
-00015450: 0a20 2020 2074 7020 3d20 636f 7369 6e65  .    tp = cosine
-00015460: 5f74 6170 6572 2877 696e 646f 775f 6c65  _taper(window_le
-00015470: 6e67 7468 5f73 616d 706c 6573 2c20 302e  ngth_samples, 0.
-00015480: 3135 290a 0a20 2020 206d 696e 696e 6420  15)..    minind 
-00015490: 3d20 300a 2020 2020 6d61 7869 6e64 203d  = 0.    maxind =
-000154a0: 2077 696e 646f 775f 6c65 6e67 7468 5f73   window_length_s
-000154b0: 616d 706c 6573 0a0a 2020 2020 2320 6c6f  amples..    # lo
-000154c0: 6f70 2074 6872 6f75 6768 2061 6c6c 2073  op through all s
-000154d0: 7562 2d77 696e 646f 7773 0a20 2020 2077  ub-windows.    w
-000154e0: 6869 6c65 206d 6178 696e 6420 3c3d 206c  hile maxind <= l
-000154f0: 656e 2872 6566 293a 0a20 2020 2020 2020  en(ref):.       
-00015500: 2063 6369 203d 2063 7572 5b6d 696e 696e   cci = cur[minin
-00015510: 643a 6d61 7869 6e64 5d0a 2020 2020 2020  d:maxind].      
-00015520: 2020 6363 6920 3d20 7363 6970 792e 7369    cci = scipy.si
-00015530: 676e 616c 2e64 6574 7265 6e64 2863 6369  gnal.detrend(cci
-00015540: 2c20 7479 7065 3d22 6c69 6e65 6172 2229  , type="linear")
-00015550: 0a20 2020 2020 2020 2063 6369 202a 3d20  .        cci *= 
-00015560: 7470 0a0a 2020 2020 2020 2020 6372 6920  tp..        cri 
-00015570: 3d20 7265 665b 6d69 6e69 6e64 3a6d 6178  = ref[minind:max
-00015580: 696e 645d 0a20 2020 2020 2020 2063 7269  ind].        cri
-00015590: 203d 2073 6369 7079 2e73 6967 6e61 6c2e   = scipy.signal.
-000155a0: 6465 7472 656e 6428 6372 692c 2074 7970  detrend(cri, typ
-000155b0: 653d 226c 696e 6561 7222 290a 2020 2020  e="linear").    
-000155c0: 2020 2020 6372 6920 2a3d 2074 700a 0a20      cri *= tp.. 
-000155d0: 2020 2020 2020 206d 696e 696e 6420 2b3d         minind +=
-000155e0: 2069 6e74 2873 6c69 6465 5f73 7465 7020   int(slide_step 
-000155f0: 2f20 6474 290a 2020 2020 2020 2020 6d61  / dt).        ma
-00015600: 7869 6e64 202b 3d20 696e 7428 736c 6964  xind += int(slid
-00015610: 655f 7374 6570 202f 2064 7429 0a0a 2020  e_step / dt)..  
-00015620: 2020 2020 2020 2320 6e6f 726d 616c 697a        # normaliz
-00015630: 6520 7369 676e 616c 7320 6265 666f 7265  e signals before
-00015640: 2063 726f 7373 2063 6f72 7265 6c61 7469   cross correlati
-00015650: 6f6e 0a20 2020 2020 2020 2063 6369 203d  on.        cci =
-00015660: 2028 6363 6920 2d20 6363 692e 6d65 616e   (cci - cci.mean
-00015670: 2829 2920 2f20 6363 692e 7374 6428 290a  ()) / cci.std().
-00015680: 2020 2020 2020 2020 6372 6920 3d20 2863          cri = (c
-00015690: 7269 202d 2063 7269 2e6d 6561 6e28 2929  ri - cri.mean())
-000156a0: 202f 2063 7269 2e73 7464 2829 0a0a 2020   / cri.std()..  
-000156b0: 2020 2020 2020 2320 6765 7420 6d61 7869        # get maxi
-000156c0: 6d75 6d20 636f 7272 656c 6174 696f 6e20  mum correlation 
-000156d0: 636f 6566 6669 6369 656e 7420 616e 6420  coefficient and 
-000156e0: 6974 7320 696e 6465 780a 2020 2020 2020  its index.      
-000156f0: 2020 6363 3220 3d20 6e70 2e63 6f72 7265    cc2 = np.corre
-00015700: 6c61 7465 2863 6369 2c20 6372 692c 206d  late(cci, cri, m
-00015710: 6f64 653d 2273 616d 6522 290a 2020 2020  ode="same").    
-00015720: 2020 2020 6363 3220 3d20 6363 3220 2f20      cc2 = cc2 / 
-00015730: 6e70 2e73 7172 7428 2863 6369 2a2a 3229  np.sqrt((cci**2)
-00015740: 2e73 756d 2829 202a 2028 6372 692a 2a32  .sum() * (cri**2
-00015750: 292e 7375 6d28 2929 0a0a 2020 2020 2020  ).sum())..      
-00015760: 2020 696d 6178 6363 3220 3d20 6e70 2e77    imaxcc2 = np.w
-00015770: 6865 7265 2863 6332 203d 3d20 6e70 2e6d  here(cc2 == np.m
-00015780: 6178 2863 6332 2929 5b30 5d0a 2020 2020  ax(cc2))[0].    
-00015790: 2020 2020 6d61 7863 6332 203d 206e 702e      maxcc2 = np.
-000157a0: 6d61 7828 6363 3229 0a0a 2020 2020 2020  max(cc2)..      
-000157b0: 2020 2320 6765 7420 7468 6520 7469 6d65    # get the time
-000157c0: 2073 6869 6674 0a20 2020 2020 2020 206d   shift.        m
-000157d0: 203d 2028 696d 6178 6363 3220 2d20 2828   = (imaxcc2 - ((
-000157e0: 6d61 7869 6e64 202d 206d 696e 696e 6429  maxind - minind)
-000157f0: 202f 2f20 3229 2920 2a20 6474 0a20 2020   // 2)) * dt.   
-00015800: 2020 2020 2064 656c 7461 5f74 2e61 7070       delta_t.app
-00015810: 656e 6428 6d29 0a20 2020 2020 2020 2064  end(m).        d
-00015820: 656c 7461 5f74 5f63 6f65 662e 6170 7065  elta_t_coef.appe
-00015830: 6e64 286d 6178 6363 3229 0a0a 2020 2020  nd(maxcc2)..    
-00015840: 2020 2020 7469 6d65 5f61 7869 732e 6170      time_axis.ap
-00015850: 7065 6e64 2874 6d69 6e20 2b20 6d6f 7669  pend(tmin + movi
-00015860: 6e67 5f77 696e 646f 775f 6c65 6e67 7468  ng_window_length
-00015870: 202f 2032 2e30 202b 2063 6f75 6e74 202a   / 2.0 + count *
-00015880: 2073 6c69 6465 5f73 7465 7029 0a20 2020   slide_step).   
-00015890: 2020 2020 2063 6f75 6e74 202b 3d20 310a       count += 1.
-000158a0: 0a20 2020 2064 656c 2063 6369 2c20 6372  .    del cci, cr
-000158b0: 692c 2063 6332 2c20 696d 6178 6363 322c  i, cc2, imaxcc2,
-000158c0: 206d 6178 6363 320a 2020 2020 6465 6c20   maxcc2.    del 
-000158d0: 6d0a 0a20 2020 2069 6620 6d61 7869 6e64  m..    if maxind
-000158e0: 203e 206c 656e 2863 7572 2920 2b20 696e   > len(cur) + in
-000158f0: 7428 736c 6964 655f 7374 6570 202f 2064  t(slide_step / d
-00015900: 7429 3a0a 2020 2020 2020 2020 6c6f 6767  t):.        logg
-00015910: 6572 2e64 6562 7567 2822 5468 6520 6c61  er.debug("The la
-00015920: 7374 2077 696e 646f 7720 7761 7320 746f  st window was to
-00015930: 6f20 736d 616c 6c2c 2062 7574 2077 6173  o small, but was
-00015940: 2063 6f6d 7075 7465 6422 290a 0a20 2020   computed")..   
-00015950: 2064 656c 7461 5f74 203d 206e 702e 6172   delta_t = np.ar
-00015960: 7261 7928 6465 6c74 615f 7429 0a20 2020  ray(delta_t).   
-00015970: 2064 656c 7461 5f74 5f63 6f65 6620 3d20   delta_t_coef = 
-00015980: 6e70 2e61 7272 6179 2864 656c 7461 5f74  np.array(delta_t
-00015990: 5f63 6f65 6629 0a20 2020 2074 696d 655f  _coef).    time_
-000159a0: 6178 6973 203d 206e 702e 6172 7261 7928  axis = np.array(
-000159b0: 7469 6d65 5f61 7869 7329 0a0a 2020 2020  time_axis)..    
-000159c0: 2320 6c69 6e65 6172 2072 6567 7265 7373  # linear regress
-000159d0: 696f 6e20 746f 2067 6574 2064 762f 760a  ion to get dv/v.
-000159e0: 2020 2020 6966 2063 6f75 6e74 203e 2032      if count > 2
-000159f0: 3a0a 2020 2020 2020 2020 2320 7369 6d70  :.        # simp
-00015a00: 6c65 2077 6569 6768 740a 2020 2020 2020  le weight.      
-00015a10: 2020 7720 3d20 6e70 2e6f 6e65 7328 636f    w = np.ones(co
-00015a20: 756e 7429 0a20 2020 2020 2020 2023 206d  unt).        # m
-00015a30: 2c20 612c 2065 6d2c 2065 6120 3d20 6c69  , a, em, ea = li
-00015a40: 6e65 6172 5f72 6567 7265 7373 696f 6e28  near_regression(
-00015a50: 7469 6d65 5f61 7869 735b 696e 6478 5d2c  time_axis[indx],
-00015a60: 2064 656c 7461 5f74 5b69 6e64 785d 2c20   delta_t[indx], 
-00015a70: 772c 2069 6e74 6572 6365 7074 5f6f 7269  w, intercept_ori
-00015a80: 6769 6e3d 4661 6c73 6529 0a20 2020 2020  gin=False).     
-00015a90: 2020 206d 302c 2065 6d30 203d 206c 696e     m0, em0 = lin
-00015aa0: 6561 725f 7265 6772 6573 7369 6f6e 2874  ear_regression(t
-00015ab0: 696d 655f 6178 6973 2e66 6c61 7474 656e  ime_axis.flatten
-00015ac0: 2829 2c20 6465 6c74 615f 742e 666c 6174  (), delta_t.flat
-00015ad0: 7465 6e28 292c 2077 2e66 6c61 7474 656e  ten(), w.flatten
-00015ae0: 2829 2c20 696e 7465 7263 6570 745f 6f72  (), intercept_or
-00015af0: 6967 696e 3d54 7275 6529 0a0a 2020 2020  igin=True)..    
-00015b00: 656c 7365 3a0a 2020 2020 2020 2020 6c6f  else:.        lo
-00015b10: 6767 6572 2e64 6562 7567 2822 6e6f 7420  gger.debug("not 
-00015b20: 656e 6f75 6768 2070 6f69 6e74 7320 746f  enough points to
-00015b30: 2065 7374 696d 6174 6520 6476 2f76 2066   estimate dv/v f
-00015b40: 6f72 2077 6363 2229 0a20 2020 2020 2020  or wcc").       
-00015b50: 206d 3020 3d20 300a 2020 2020 2020 2020   m0 = 0.        
-00015b60: 656d 3020 3d20 300a 0a20 2020 2072 6574  em0 = 0..    ret
-00015b70: 7572 6e20 2d6d 3020 2a20 3130 302c 2065  urn -m0 * 100, e
-00015b80: 6d30 202a 2031 3030 0a0a 0a64 6566 2077  m0 * 100...def w
-00015b90: 7873 5f64 7676 280a 2020 2020 7265 662c  xs_dvv(.    ref,
-00015ba0: 0a20 2020 2063 7572 2c0a 2020 2020 616c  .    cur,.    al
-00015bb0: 6c66 7265 712c 0a20 2020 2070 6172 612c  lfreq,.    para,
-00015bc0: 0a20 2020 2064 6a3d 3120 2f20 3132 2c0a  .    dj=1 / 12,.
-00015bd0: 2020 2020 7330 3d2d 312c 0a20 2020 204a      s0=-1,.    J
-00015be0: 3d2d 312c 0a20 2020 2073 6967 3d46 616c  =-1,.    sig=Fal
-00015bf0: 7365 2c0a 2020 2020 7776 6e3d 226d 6f72  se,.    wvn="mor
-00015c00: 6c65 7422 2c0a 2020 2020 756e 7772 6170  let",.    unwrap
-00015c10: 666c 6167 3d46 616c 7365 2c0a 293a 0a20  flag=False,.):. 
-00015c20: 2020 2022 2222 0a20 2020 2043 6f6d 7075     """.    Compu
-00015c30: 7465 2064 7420 6f72 2064 762f 7620 696e  te dt or dv/v in
-00015c40: 2074 696d 6520 616e 6420 6672 6571 7565   time and freque
-00015c50: 6e63 7920 646f 6d61 696e 2066 726f 6d20  ncy domain from 
-00015c60: 7761 7665 6c65 7420 6372 6f73 7320 7370  wavelet cross sp
-00015c70: 6563 7472 756d 2028 7778 7329 2e0a 2020  ectrum (wxs)..  
-00015c80: 2020 666f 7220 616c 6c20 6672 6571 7565    for all freque
-00015c90: 6369 6573 2069 6e20 616e 2069 6e74 6572  cies in an inter
-00015ca0: 6573 7420 7261 6e67 650a 0a20 2020 2050  est range..    P
-00015cb0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-00015cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
-00015cd0: 2072 6566 3a20 5468 6520 2252 6566 6572   ref: The "Refer
-00015ce0: 656e 6365 2220 7469 6d65 7365 7269 6573  ence" timeseries
-00015cf0: 2028 6e75 6d70 792e 6e64 6172 7261 7929   (numpy.ndarray)
-00015d00: 0a20 2020 2063 7572 3a20 5468 6520 2243  .    cur: The "C
-00015d10: 7572 7265 6e74 2220 7469 6d65 7365 7269  urrent" timeseri
-00015d20: 6573 2028 6e75 6d70 792e 6e64 6172 7261  es (numpy.ndarra
-00015d30: 7929 0a20 2020 2061 6c6c 6672 6571 3a20  y).    allfreq: 
-00015d40: 6120 626f 6f6c 656e 2076 6172 6961 626c  a boolen variabl
-00015d50: 6520 746f 206d 616b 6520 6d65 6173 7572  e to make measur
-00015d60: 656d 656e 7473 206f 6e20 616c 6c20 6672  ements on all fr
-00015d70: 6571 7565 6e63 7920 7261 6e67 6520 6f72  equency range or
-00015d80: 206e 6f74 0a20 2020 2070 6172 613a 2061   not.    para: a
-00015d90: 2064 6963 7420 636f 6e74 6169 6e69 6e67   dict containing
-00015da0: 2066 7265 712f 7469 6d65 2069 6e66 6f20   freq/time info 
-00015db0: 6f66 2074 6865 2064 6174 6120 6d61 7472  of the data matr
-00015dc0: 6978 0a20 2020 2064 6a2c 2073 302c 204a  ix.    dj, s0, J
-00015dd0: 2c20 7369 672c 2077 766e 3a20 636f 6d6d  , sig, wvn: comm
-00015de0: 6f6e 2070 6172 616d 6574 6572 7320 7573  on parameters us
-00015df0: 6564 2069 6e20 2777 6176 656c 6574 2e77  ed in 'wavelet.w
-00015e00: 6374 270a 2020 2020 756e 7772 6170 666c  ct'.    unwrapfl
-00015e10: 6167 3a20 5472 7565 202d 2075 6e77 7261  ag: True - unwra
-00015e20: 7020 7068 6173 6520 6465 6c61 7973 2e20  p phase delays. 
-00015e30: 4465 6661 756c 7420 6973 2046 616c 7365  Default is False
-00015e40: 0a0a 2020 2020 5245 5455 524e 533a 0a20  ..    RETURNS:. 
-00015e50: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
-00015e60: 2d2d 2d2d 2d0a 2020 2020 6476 762a 3130  -----.    dvv*10
-00015e70: 3020 3a20 6573 7469 6d61 7465 6420 6476  0 : estimated dv
-00015e80: 2f76 2069 6e20 250a 2020 2020 6572 722a  /v in %.    err*
-00015e90: 3130 3020 3a20 6572 726f 7220 6f66 2064  100 : error of d
-00015ea0: 762f 7620 6573 7469 6d61 7469 6f6e 2069  v/v estimation i
-00015eb0: 6e20 250a 0a20 2020 204f 7269 6769 6e61  n %..    Origina
-00015ec0: 6c6c 7920 7772 6974 7465 6e20 6279 2054  lly written by T
-00015ed0: 696d 2043 6c65 6d65 6e74 7320 2831 204d  im Clements (1 M
-00015ee0: 6172 6368 2c20 3230 3139 290a 2020 2020  arch, 2019).    
-00015ef0: 4d6f 6469 6669 6564 2062 7920 436f 6e67  Modified by Cong
-00015f00: 636f 6e67 2059 7561 6e20 2833 3020 4a75  cong Yuan (30 Ju
-00015f10: 6e65 2c20 3230 3139 2920 6261 7365 6420  ne, 2019) based 
-00015f20: 6f6e 2028 4d61 6f20 6574 2061 6c2e 2032  on (Mao et al. 2
-00015f30: 3031 3929 2e0a 2020 2020 5570 6461 7465  019)..    Update
-00015f40: 6420 6279 2043 6865 6e67 7869 6e20 4a69  d by Chengxin Ji
-00015f50: 616e 6720 2831 3020 4f63 742c 2032 3031  ang (10 Oct, 201
-00015f60: 3929 2074 6f20 6d65 7267 6520 7468 6520  9) to merge the 
-00015f70: 6675 6e63 7469 6f6e 616c 6974 7920 666f  functionality fo
-00015f80: 7220 6d65 7375 7265 6d65 6e74 730a 2020  r mesurements.  
-00015f90: 2020 6163 726f 7373 2061 6c6c 2066 7265    across all fre
-00015fa0: 7175 656e 6379 2061 6e64 206f 6e65 2066  quency and one f
-00015fb0: 7265 7120 7261 6e67 650a 2020 2020 2222  req range.    ""
-00015fc0: 220a 2020 2020 2320 636f 6d6d 6f6e 2076  ".    # common v
-00015fd0: 6172 6961 626c 6573 0a20 2020 2074 7769  ariables.    twi
-00015fe0: 6e20 3d20 7061 7261 5b22 7477 696e 225d  n = para["twin"]
-00015ff0: 0a20 2020 2066 7265 7120 3d20 7061 7261  .    freq = para
-00016000: 5b22 6672 6571 225d 0a20 2020 2064 7420  ["freq"].    dt 
-00016010: 3d20 7061 7261 5b22 6474 225d 0a20 2020  = para["dt"].   
-00016020: 2074 6d69 6e20 3d20 6e70 2e6d 696e 2874   tmin = np.min(t
-00016030: 7769 6e29 0a20 2020 2074 6d61 7820 3d20  win).    tmax = 
-00016040: 6e70 2e6d 6178 2874 7769 6e29 0a20 2020  np.max(twin).   
-00016050: 2066 6d69 6e20 3d20 6e70 2e6d 696e 2866   fmin = np.min(f
-00016060: 7265 7129 0a20 2020 2066 6d61 7820 3d20  req).    fmax = 
-00016070: 6e70 2e6d 6178 2866 7265 7129 0a20 2020  np.max(freq).   
-00016080: 2074 7665 6320 3d20 6e70 2e61 7261 6e67   tvec = np.arang
-00016090: 6528 746d 696e 2c20 746d 6178 2c20 6474  e(tmin, tmax, dt
-000160a0: 290a 2020 2020 6e70 7473 203d 206c 656e  ).    npts = len
-000160b0: 2874 7665 6329 0a0a 2020 2020 2320 7065  (tvec)..    # pe
-000160c0: 7266 6f72 6d20 6372 6f73 7320 636f 6865  rform cross cohe
-000160d0: 7265 6e74 2061 6e61 6c79 7369 732c 206d  rent analysis, m
-000160e0: 6f64 6966 6965 6420 6672 6f6d 2066 756e  odified from fun
-000160f0: 6374 696f 6e20 2777 6176 656c 6574 2e63  ction 'wavelet.c
-00016100: 7774 270a 2020 2020 5743 542c 2061 5743  wt'.    WCT, aWC
-00016110: 542c 2063 6f69 2c20 6672 6571 2c20 7369  T, coi, freq, si
-00016120: 6720 3d20 7763 745f 6d6f 6469 6669 6564  g = wct_modified
-00016130: 2872 6566 2c20 6375 722c 2064 742c 2064  (ref, cur, dt, d
-00016140: 6a3d 646a 2c20 7330 3d73 302c 204a 3d4a  j=dj, s0=s0, J=J
-00016150: 2c20 7369 673d 7369 672c 2077 6176 656c  , sig=sig, wavel
-00016160: 6574 3d77 766e 2c20 6e6f 726d 616c 697a  et=wvn, normaliz
-00016170: 653d 5472 7565 290a 0a20 2020 2069 6620  e=True)..    if 
-00016180: 756e 7772 6170 666c 6167 3a0a 2020 2020  unwrapflag:.    
-00016190: 2020 2020 7068 6173 6520 3d20 6e70 2e75      phase = np.u
-000161a0: 6e77 7261 7028 6157 4354 2c20 6178 6973  nwrap(aWCT, axis
-000161b0: 3d2d 3129 2020 2320 6178 6973 3d30 2c20  =-1)  # axis=0, 
-000161c0: 7570 7772 6170 2061 6c6f 6e67 2074 696d  upwrap along tim
-000161d0: 653b 2061 7869 733d 2d31 2c20 756e 7772  e; axis=-1, unwr
-000161e0: 6170 2061 6c6f 6e67 2066 7265 7175 656e  ap along frequen
-000161f0: 6379 0a20 2020 2065 6c73 653a 0a20 2020  cy.    else:.   
-00016200: 2020 2020 2070 6861 7365 203d 2061 5743       phase = aWC
-00016210: 540a 0a20 2020 2023 207a 6572 6f20 6f75  T..    # zero ou
-00016220: 7420 6461 7461 206f 7574 7369 6465 2066  t data outside f
-00016230: 7265 7175 656e 6379 2062 616e 640a 2020  requency band.  
-00016240: 2020 6966 2028 666d 6178 203e 206e 702e    if (fmax > np.
-00016250: 6d61 7828 6672 6571 2929 207c 2028 666d  max(freq)) | (fm
-00016260: 6178 203c 3d20 666d 696e 293a 0a20 2020  ax <= fmin):.   
-00016270: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00016280: 4572 726f 7228 2241 626f 7274 3a20 696e  Error("Abort: in
-00016290: 7075 7420 6672 6571 7565 6e63 7920 6f75  put frequency ou
-000162a0: 7420 6f66 206c 696d 6974 7321 2229 0a20  t of limits!"). 
-000162b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000162c0: 2066 7265 715f 696e 6469 6e20 3d20 6e70   freq_indin = np
-000162d0: 2e77 6865 7265 2828 6672 6571 203e 3d20  .where((freq >= 
-000162e0: 666d 696e 2920 2620 2866 7265 7120 3c3d  fmin) & (freq <=
-000162f0: 2066 6d61 7829 295b 305d 0a0a 2020 2020   fmax))[0]..    
-00016300: 2320 666f 6c6c 6f77 204d 5743 5320 746f  # follow MWCS to
-00016310: 2064 6f20 7477 6f20 7374 6570 7320 6f66   do two steps of
-00016320: 206c 696e 6561 7220 7265 6772 6573 7369   linear regressi
-00016330: 6f6e 0a20 2020 2069 6620 6e6f 7420 616c  on.    if not al
-00016340: 6c66 7265 713a 0a20 2020 2020 2020 2064  lfreq:.        d
-00016350: 656c 7461 5f74 5f6d 2c20 6465 6c74 615f  elta_t_m, delta_
-00016360: 745f 756e 6320 3d20 6e70 2e7a 6572 6f73  t_unc = np.zeros
-00016370: 286e 7074 732c 2064 7479 7065 3d6e 702e  (npts, dtype=np.
-00016380: 666c 6f61 7433 3229 2c20 6e70 2e7a 6572  float32), np.zer
-00016390: 6f73 286e 7074 732c 2064 7479 7065 3d6e  os(npts, dtype=n
-000163a0: 702e 666c 6f61 7433 3229 0a20 2020 2020  p.float32).     
-000163b0: 2020 2023 2061 7373 756d 6520 7468 6520     # assume the 
-000163c0: 7476 6563 2069 7320 7468 6520 7469 6d65  tvec is the time
-000163d0: 2077 696e 646f 7720 746f 206d 6561 7375   window to measu
-000163e0: 7265 2064 740a 2020 2020 2020 2020 666f  re dt.        fo
-000163f0: 7220 6974 2069 6e20 7261 6e67 6528 6e70  r it in range(np
-00016400: 7473 293a 0a20 2020 2020 2020 2020 2020  ts):.           
-00016410: 2077 203d 2031 202f 2057 4354 5b66 7265   w = 1 / WCT[fre
-00016420: 715f 696e 6469 6e2c 2069 745d 0a20 2020  q_indin, it].   
-00016430: 2020 2020 2020 2020 2077 5b7e 6e70 2e69           w[~np.i
-00016440: 7366 696e 6974 6528 7729 5d20 3d20 312e  sfinite(w)] = 1.
-00016450: 300a 2020 2020 2020 2020 2020 2020 6465  0.            de
-00016460: 6c74 615f 745f 6d5b 6974 5d2c 2064 656c  lta_t_m[it], del
-00016470: 7461 5f74 5f75 6e63 5b69 745d 203d 206c  ta_t_unc[it] = l
-00016480: 696e 6561 725f 7265 6772 6573 7369 6f6e  inear_regression
-00016490: 2866 7265 715b 6672 6571 5f69 6e64 696e  (freq[freq_indin
-000164a0: 5d20 2a20 3220 2a20 6e70 2e70 692c 2070  ] * 2 * np.pi, p
-000164b0: 6861 7365 5b66 7265 715f 696e 6469 6e2c  hase[freq_indin,
-000164c0: 2069 745d 2c20 7729 0a0a 2020 2020 2020   it], w)..      
-000164d0: 2020 2320 6e65 7720 7765 6967 6874 7320    # new weights 
-000164e0: 666f 7220 7265 6772 6573 7369 6f6e 0a20  for regression. 
-000164f0: 2020 2020 2020 2077 3220 3d20 3120 2f20         w2 = 1 / 
-00016500: 6e70 2e6d 6561 6e28 5743 545b 6672 6571  np.mean(WCT[freq
-00016510: 5f69 6e64 696e 2c20 3a5d 2c20 6178 6973  _indin, :], axis
-00016520: 3d30 290a 2020 2020 2020 2020 7732 5b7e  =0).        w2[~
-00016530: 6e70 2e69 7366 696e 6974 6528 7732 295d  np.isfinite(w2)]
-00016540: 203d 2031 2e30 0a0a 2020 2020 2020 2020   = 1.0..        
-00016550: 2320 6e6f 7720 7573 6520 6474 2061 6e64  # now use dt and
-00016560: 2074 2074 6f20 6765 7420 6476 2f76 0a20   t to get dv/v. 
-00016570: 2020 2020 2020 2069 6620 6c65 6e28 7732         if len(w2
-00016580: 2920 3e20 323a 0a20 2020 2020 2020 2020  ) > 2:.         
-00016590: 2020 2069 6620 6e6f 7420 6e70 2e61 6e79     if not np.any
-000165a0: 2864 656c 7461 5f74 5f6d 293a 0a20 2020  (delta_t_m):.   
-000165b0: 2020 2020 2020 2020 2020 2020 2064 7676               dvv
-000165c0: 2c20 6572 7220 3d20 6e70 2e6e 616e 2c20  , err = np.nan, 
-000165d0: 6e70 2e6e 616e 0a20 2020 2020 2020 2020  np.nan.         
-000165e0: 2020 206d 2c20 656d 203d 206c 696e 6561     m, em = linea
-000165f0: 725f 7265 6772 6573 7369 6f6e 2874 7665  r_regression(tve
-00016600: 632c 2064 656c 7461 5f74 5f6d 2c20 7732  c, delta_t_m, w2
-00016610: 2c20 696e 7465 7263 6570 745f 6f72 6967  , intercept_orig
-00016620: 696e 3d54 7275 6529 0a20 2020 2020 2020  in=True).       
-00016630: 2020 2020 2064 7676 2c20 6572 7220 3d20       dvv, err = 
-00016640: 2d6d 2c20 656d 0a20 2020 2020 2020 2065  -m, em.        e
-00016650: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00016660: 206c 6f67 6765 722e 6465 6275 6728 226e   logger.debug("n
-00016670: 6f74 2065 6e6f 7567 6820 706f 696e 7473  ot enough points
-00016680: 2074 6f20 6573 7469 6d61 7465 2064 762f   to estimate dv/
-00016690: 7620 666f 7220 7774 7322 290a 2020 2020  v for wts").    
-000166a0: 2020 2020 2020 2020 6476 762c 2065 7272          dvv, err
-000166b0: 203d 206e 702e 6e61 6e2c 206e 702e 6e61   = np.nan, np.na
-000166c0: 6e0a 0a20 2020 2020 2020 2072 6574 7572  n..        retur
-000166d0: 6e20 6476 7620 2a20 3130 302c 2065 7272  n dvv * 100, err
-000166e0: 202a 2031 3030 0a0a 2020 2020 2320 636f   * 100..    # co
-000166f0: 6e76 6572 7420 7068 6173 6520 6469 7265  nvert phase dire
-00016700: 6374 6c79 2074 6f20 6465 6c74 615f 7420  ctly to delta_t 
-00016710: 666f 7220 616c 6c20 6672 6571 7565 6e63  for all frequenc
-00016720: 6965 730a 2020 2020 656c 7365 3a0a 2020  ies.    else:.  
-00016730: 2020 2020 2020 2320 636f 6e76 6572 7420        # convert 
-00016740: 7068 6173 6520 6465 6c61 7920 746f 2074  phase delay to t
-00016750: 696d 6520 6465 6c61 790a 2020 2020 2020  ime delay.      
-00016760: 2020 6465 6c74 615f 7420 3d20 7068 6173    delta_t = phas
-00016770: 6520 2f20 2832 202a 206e 702e 7069 202a  e / (2 * np.pi *
-00016780: 2066 7265 715b 3a2c 204e 6f6e 655d 2920   freq[:, None]) 
-00016790: 2023 206e 6f72 6d61 6c69 7a65 2070 6861   # normalize pha
-000167a0: 7365 2062 7920 2832 2a70 692a 6672 6571  se by (2*pi*freq
-000167b0: 7565 6e63 7929 0a20 2020 2020 2020 2064  uency).        d
-000167c0: 7676 2c20 6572 7220 3d20 6e70 2e7a 6572  vv, err = np.zer
-000167d0: 6f73 2866 7265 715f 696e 6469 6e2e 7368  os(freq_indin.sh
-000167e0: 6170 6529 2c20 6e70 2e7a 6572 6f73 2866  ape), np.zeros(f
-000167f0: 7265 715f 696e 6469 6e2e 7368 6170 6529  req_indin.shape)
-00016800: 0a0a 2020 2020 2020 2020 2320 6c6f 6f70  ..        # loop
-00016810: 2074 6872 6f75 6768 2066 7265 7120 666f   through freq fo
-00016820: 7220 6c69 6e65 6172 2072 6567 7265 7373  r linear regress
-00016830: 696f 6e0a 2020 2020 2020 2020 666f 7220  ion.        for 
-00016840: 6969 2c20 6966 7265 7120 696e 2065 6e75  ii, ifreq in enu
-00016850: 6d65 7261 7465 2866 7265 715f 696e 6469  merate(freq_indi
-00016860: 6e29 3a0a 2020 2020 2020 2020 2020 2020  n):.            
-00016870: 6966 206c 656e 2874 7665 6329 203e 2032  if len(tvec) > 2
-00016880: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00016890: 2020 6966 206e 6f74 206e 702e 616e 7928    if not np.any(
-000168a0: 6465 6c74 615f 745b 6966 7265 715d 293a  delta_t[ifreq]):
-000168b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000168c0: 2020 2020 2063 6f6e 7469 6e75 650a 0a20       continue.. 
-000168d0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000168e0: 2068 6f77 2074 6f20 6265 7474 6572 2061   how to better a
-000168f0: 7070 726f 6163 6820 7468 6520 756e 6365  pproach the unce
-00016900: 7274 6169 6e74 7920 6f66 2064 656c 7461  rtainty of delta
-00016910: 5f74 0a20 2020 2020 2020 2020 2020 2020  _t.             
-00016920: 2020 2077 203d 2031 202f 2057 4354 5b69     w = 1 / WCT[i
-00016930: 6672 6571 5d0a 2020 2020 2020 2020 2020  freq].          
-00016940: 2020 2020 2020 775b 7e6e 702e 6973 6669        w[~np.isfi
-00016950: 6e69 7465 2877 295d 203d 2031 2e30 0a0a  nite(w)] = 1.0..
-00016960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016970: 2320 6d2c 2061 2c20 656d 2c20 6561 203d  # m, a, em, ea =
-00016980: 206c 696e 6561 725f 7265 6772 6573 7369   linear_regressi
-00016990: 6f6e 2874 696d 655f 6178 6973 5b69 6e64  on(time_axis[ind
-000169a0: 785d 2c20 6465 6c74 615f 745b 696e 6478  x], delta_t[indx
-000169b0: 5d2c 2077 2c20 696e 7465 7263 6570 745f  ], w, intercept_
-000169c0: 6f72 6967 696e 3d46 616c 7365 290a 2020  origin=False).  
-000169d0: 2020 2020 2020 2020 2020 2020 2020 6d2c                m,
-000169e0: 2065 6d20 3d20 6c69 6e65 6172 5f72 6567   em = linear_reg
-000169f0: 7265 7373 696f 6e28 7476 6563 2c20 6465  ression(tvec, de
-00016a00: 6c74 615f 745b 6966 7265 715d 2c20 772c  lta_t[ifreq], w,
-00016a10: 2069 6e74 6572 6365 7074 5f6f 7269 6769   intercept_origi
-00016a20: 6e3d 5472 7565 290a 2020 2020 2020 2020  n=True).        
-00016a30: 2020 2020 2020 2020 6476 765b 6969 5d2c          dvv[ii],
-00016a40: 2065 7272 5b69 695d 203d 202d 6d2c 2065   err[ii] = -m, e
-00016a50: 6d0a 2020 2020 2020 2020 2020 2020 656c  m.            el
-00016a60: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00016a70: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-00016a80: 2822 6e6f 7420 656e 6f75 6768 2070 6f69  ("not enough poi
-00016a90: 6e74 7320 746f 2065 7374 696d 6174 6520  nts to estimate 
-00016aa0: 6476 2f76 2066 6f72 2077 7473 2229 0a20  dv/v for wts"). 
-00016ab0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00016ac0: 7676 5b69 695d 2c20 6572 725b 6969 5d20  vv[ii], err[ii] 
-00016ad0: 3d20 6e70 2e6e 616e 2c20 6e70 2e6e 616e  = np.nan, np.nan
-00016ae0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00016af0: 2066 7265 715b 6672 6571 5f69 6e64 696e   freq[freq_indin
-00016b00: 5d2c 2064 7676 202a 2031 3030 2c20 6572  ], dvv * 100, er
-00016b10: 7220 2a20 3130 300a 0a0a 6465 6620 7774  r * 100...def wt
-00016b20: 735f 6476 7628 0a20 2020 2072 6566 2c0a  s_dvv(.    ref,.
-00016b30: 2020 2020 6375 722c 0a20 2020 2061 6c6c      cur,.    all
-00016b40: 6672 6571 2c0a 2020 2020 7061 7261 2c0a  freq,.    para,.
-00016b50: 2020 2020 6476 5f72 616e 6765 2c0a 2020      dv_range,.  
-00016b60: 2020 6e62 7472 6961 6c2c 0a20 2020 2064    nbtrial,.    d
-00016b70: 6a3d 3120 2f20 3132 2c0a 2020 2020 7330  j=1 / 12,.    s0
-00016b80: 3d2d 312c 0a20 2020 204a 3d2d 312c 0a20  =-1,.    J=-1,. 
-00016b90: 2020 2077 766e 3d22 6d6f 726c 6574 222c     wvn="morlet",
-00016ba0: 0a20 2020 206e 6f72 6d61 6c69 7a65 3d54  .    normalize=T
-00016bb0: 7275 652c 0a29 3a0a 2020 2020 2222 220a  rue,.):.    """.
-00016bc0: 2020 2020 4170 706c 7920 7374 7265 7463      Apply stretc
-00016bd0: 6869 6e67 206d 6574 686f 6420 746f 2063  hing method to c
-00016be0: 6f6e 7469 6e75 6f75 7320 7761 7665 6c65  ontinuous wavele
-00016bf0: 7420 7472 616e 7366 6f72 6d61 7469 6f6e  t transformation
-00016c00: 2028 4357 5429 206f 6620 7369 676e 616c   (CWT) of signal
-00016c10: 730a 2020 2020 666f 7220 616c 6c20 6672  s.    for all fr
-00016c20: 6571 7565 6369 6573 2069 6e20 616e 2069  equecies in an i
-00016c30: 6e74 6572 6573 7420 7261 6e67 650a 0a20  nterest range.. 
-00016c40: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00016c50: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
-00016c60: 0a20 2020 2072 6566 3a20 5468 6520 2252  .    ref: The "R
-00016c70: 6566 6572 656e 6365 2220 7469 6d65 7365  eference" timese
-00016c80: 7269 6573 2028 6e75 6d70 792e 6e64 6172  ries (numpy.ndar
-00016c90: 7261 7929 0a20 2020 2063 7572 3a20 5468  ray).    cur: Th
-00016ca0: 6520 2243 7572 7265 6e74 2220 7469 6d65  e "Current" time
-00016cb0: 7365 7269 6573 2028 6e75 6d70 792e 6e64  series (numpy.nd
-00016cc0: 6172 7261 7929 0a20 2020 2061 6c6c 6672  array).    allfr
-00016cd0: 6571 3a20 6120 626f 6f6c 656e 2076 6172  eq: a boolen var
-00016ce0: 6961 626c 6520 746f 206d 616b 6520 6d65  iable to make me
-00016cf0: 6173 7572 656d 656e 7473 206f 6e20 616c  asurements on al
-00016d00: 6c20 6672 6571 7565 6e63 7920 7261 6e67  l frequency rang
-00016d10: 6520 6f72 206e 6f74 0a20 2020 2070 6172  e or not.    par
-00016d20: 613a 2061 2064 6963 7420 636f 6e74 6169  a: a dict contai
-00016d30: 6e69 6e67 2066 7265 712f 7469 6d65 2069  ning freq/time i
-00016d40: 6e66 6f20 6f66 2074 6865 2064 6174 6120  nfo of the data 
-00016d50: 6d61 7472 6978 0a20 2020 2064 765f 7261  matrix.    dv_ra
-00016d60: 6e67 653a 2061 6273 6f6c 7574 6520 626f  nge: absolute bo
-00016d70: 756e 6420 666f 7220 7468 6520 7665 6c6f  und for the velo
-00016d80: 6369 7479 2076 6172 6961 7469 6f6e 3b20  city variation; 
-00016d90: 6578 616d 706c 653a 2064 763d 302e 3033  example: dv=0.03
-00016da0: 2066 6f72 205b 2d33 2c33 5d25 0a20 2020   for [-3,3]%.   
-00016db0: 206f 6620 7265 6c61 7469 7665 2076 656c   of relative vel
-00016dc0: 6f63 6974 7920 6368 616e 6765 2028 666c  ocity change (fl
-00016dd0: 6f61 7429 0a20 2020 206e 6274 7269 616c  oat).    nbtrial
-00016de0: 3a20 6e75 6d62 6572 206f 6620 7374 7265  : number of stre
-00016df0: 7463 6869 6e67 2063 6f65 6666 6963 6965  tching coefficie
-00016e00: 6e74 2062 6574 7765 656e 2064 766d 696e  nt between dvmin
-00016e10: 2061 6e64 2064 766d 6178 2c20 6e6f 206e   and dvmax, no n
-00016e20: 6565 6420 746f 2062 6520 6869 6768 6572  eed to be higher
-00016e30: 2074 6861 6e20 3130 3020 2028 666c 6f61   than 100  (floa
-00016e40: 7429 0a20 2020 2064 6a2c 2073 302c 204a  t).    dj, s0, J
-00016e50: 2c20 7369 672c 2077 766e 3a20 636f 6d6d  , sig, wvn: comm
-00016e60: 6f6e 2070 6172 616d 6574 6572 7320 7573  on parameters us
-00016e70: 6564 2069 6e20 2777 6176 656c 6574 2e77  ed in 'wavelet.w
-00016e80: 6374 270a 2020 2020 6e6f 726d 616c 697a  ct'.    normaliz
-00016e90: 653a 206e 6f72 6d61 6c69 7a65 2074 6865  e: normalize the
-00016ea0: 2077 6176 656c 6574 2073 7065 6374 7275   wavelet spectru
-00016eb0: 6d20 6f72 206e 6f74 2e20 4465 6661 756c  m or not. Defaul
-00016ec0: 7420 6973 2054 7275 650a 0a20 2020 2052  t is True..    R
-00016ed0: 4554 5552 4e53 3a0a 2020 2020 2d2d 2d2d  ETURNS:.    ----
-00016ee0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
-00016ef0: 2020 2064 7676 3a20 6573 7469 6d61 7465     dvv: estimate
-00016f00: 6420 6476 2f76 0a20 2020 2065 7272 3a20  d dv/v.    err: 
-00016f10: 6572 726f 7220 6f66 2064 762f 7620 6573  error of dv/v es
-00016f20: 7469 6d61 7469 6f6e 0a0a 2020 2020 5772  timation..    Wr
-00016f30: 6974 7465 6e20 6279 2043 6f6e 6763 6f6e  itten by Congcon
-00016f40: 6720 5975 616e 2028 3330 204a 756e 2c20  g Yuan (30 Jun, 
-00016f50: 3230 3139 290a 2020 2020 2222 220a 2020  2019).    """.  
-00016f60: 2020 2320 636f 6d6d 6f6e 2076 6172 6961    # common varia
-00016f70: 626c 6573 0a20 2020 2066 7265 7120 3d20  bles.    freq = 
-00016f80: 7061 7261 5b22 6672 6571 225d 0a20 2020  para["freq"].   
-00016f90: 2064 7420 3d20 7061 7261 5b22 6474 225d   dt = para["dt"]
-00016fa0: 0a20 2020 2066 6d69 6e20 3d20 6e70 2e6d  .    fmin = np.m
-00016fb0: 696e 2866 7265 7129 0a20 2020 2066 6d61  in(freq).    fma
-00016fc0: 7820 3d20 6e70 2e6d 6178 2866 7265 7129  x = np.max(freq)
-00016fd0: 0a0a 2020 2020 2320 6170 706c 7920 6377  ..    # apply cw
-00016fe0: 7420 6f6e 2074 776f 2074 7261 6365 730a  t on two traces.
-00016ff0: 2020 2020 6377 7431 2c20 736a 2c20 6672      cwt1, sj, fr
-00017000: 6571 2c20 636f 692c 205f 2c20 5f20 3d20  eq, coi, _, _ = 
-00017010: 7079 6377 742e 6377 7428 6375 722c 2064  pycwt.cwt(cur, d
-00017020: 742c 2064 6a2c 2073 302c 204a 2c20 7776  t, dj, s0, J, wv
-00017030: 6e29 0a20 2020 2063 7774 322c 2073 6a2c  n).    cwt2, sj,
-00017040: 2066 7265 712c 2063 6f69 2c20 5f2c 205f   freq, coi, _, _
-00017050: 203d 2070 7963 7774 2e63 7774 2872 6566   = pycwt.cwt(ref
-00017060: 2c20 6474 2c20 646a 2c20 7330 2c20 4a2c  , dt, dj, s0, J,
-00017070: 2077 766e 290a 0a20 2020 2023 2065 7874   wvn)..    # ext
-00017080: 7261 6374 2072 6561 6c20 7661 6c75 6573  ract real values
-00017090: 206f 6620 6377 740a 2020 2020 7263 7774   of cwt.    rcwt
-000170a0: 312c 2072 6377 7432 203d 206e 702e 7265  1, rcwt2 = np.re
-000170b0: 616c 2863 7774 3129 2c20 6e70 2e72 6561  al(cwt1), np.rea
-000170c0: 6c28 6377 7432 290a 0a20 2020 2023 207a  l(cwt2)..    # z
-000170d0: 6572 6f20 6f75 7420 6461 7461 206f 7574  ero out data out
-000170e0: 7369 6465 2066 7265 7175 656e 6379 2062  side frequency b
-000170f0: 616e 640a 2020 2020 6966 2028 666d 6178  and.    if (fmax
-00017100: 203e 206e 702e 6d61 7828 6672 6571 2929   > np.max(freq))
-00017110: 207c 2028 666d 6178 203c 3d20 666d 696e   | (fmax <= fmin
-00017120: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
-00017130: 2056 616c 7565 4572 726f 7228 2241 626f   ValueError("Abo
-00017140: 7274 3a20 696e 7075 7420 6672 6571 7565  rt: input freque
-00017150: 6e63 7920 6f75 7420 6f66 206c 696d 6974  ncy out of limit
-00017160: 7321 2229 0a20 2020 2065 6c73 653a 0a20  s!").    else:. 
-00017170: 2020 2020 2020 2066 7265 715f 696e 6469         freq_indi
-00017180: 6e20 3d20 6e70 2e77 6865 7265 2828 6672  n = np.where((fr
-00017190: 6571 203e 3d20 666d 696e 2920 2620 2866  eq >= fmin) & (f
-000171a0: 7265 7120 3c3d 2066 6d61 7829 295b 305d  req <= fmax))[0]
-000171b0: 0a0a 2020 2020 2320 636f 6e76 6572 7420  ..    # convert 
-000171c0: 7761 7665 6c65 7420 646f 6d61 696e 2062  wavelet domain b
-000171d0: 6163 6b20 746f 2074 696d 6520 646f 6d61  ack to time doma
-000171e0: 696e 2028 7e66 696c 7465 7269 6e67 290a  in (~filtering).
-000171f0: 2020 2020 6966 206e 6f74 2061 6c6c 6672      if not allfr
-00017200: 6571 3a0a 2020 2020 2020 2020 2320 696e  eq:.        # in
-00017210: 7665 7273 6520 6377 7420 746f 2074 696d  verse cwt to tim
-00017220: 6520 646f 6d61 696e 0a20 2020 2020 2020  e domain.       
-00017230: 2069 6377 7431 203d 2070 7963 7774 2e69   icwt1 = pycwt.i
-00017240: 6377 7428 6377 7431 5b66 7265 715f 696e  cwt(cwt1[freq_in
-00017250: 6469 6e5d 2c20 736a 5b66 7265 715f 696e  din], sj[freq_in
-00017260: 6469 6e5d 2c20 6474 2c20 646a 2c20 7776  din], dt, dj, wv
-00017270: 6e29 0a20 2020 2020 2020 2069 6377 7432  n).        icwt2
-00017280: 203d 2070 7963 7774 2e69 6377 7428 6377   = pycwt.icwt(cw
-00017290: 7432 5b66 7265 715f 696e 6469 6e5d 2c20  t2[freq_indin], 
-000172a0: 736a 5b66 7265 715f 696e 6469 6e5d 2c20  sj[freq_indin], 
-000172b0: 6474 2c20 646a 2c20 7776 6e29 0a0a 2020  dt, dj, wvn)..  
-000172c0: 2020 2020 2020 2320 6173 7375 6d65 2061        # assume a
-000172d0: 6c6c 2074 696d 6520 7769 6e64 6f77 2069  ll time window i
-000172e0: 7320 7573 6564 0a20 2020 2020 2020 2077  s used.        w
-000172f0: 6377 7431 2c20 7763 7774 3220 3d20 6e70  cwt1, wcwt2 = np
-00017300: 2e72 6561 6c28 6963 7774 3129 2c20 6e70  .real(icwt1), np
-00017310: 2e72 6561 6c28 6963 7774 3229 0a0a 2020  .real(icwt2)..  
-00017320: 2020 2020 2020 2320 4e6f 726d 616c 697a        # Normaliz
-00017330: 6573 2062 6f74 6820 7369 676e 616c 732c  es both signals,
-00017340: 2069 6620 6170 7072 6f70 7269 6174 652e   if appropriate.
-00017350: 0a20 2020 2020 2020 2069 6620 6e6f 726d  .        if norm
-00017360: 616c 697a 653a 0a20 2020 2020 2020 2020  alize:.         
-00017370: 2020 206e 6377 7431 203d 2028 7763 7774     ncwt1 = (wcwt
-00017380: 3120 2d20 7763 7774 312e 6d65 616e 2829  1 - wcwt1.mean()
-00017390: 2920 2f20 7763 7774 312e 7374 6428 290a  ) / wcwt1.std().
-000173a0: 2020 2020 2020 2020 2020 2020 6e63 7774              ncwt
-000173b0: 3220 3d20 2877 6377 7432 202d 2077 6377  2 = (wcwt2 - wcw
-000173c0: 7432 2e6d 6561 6e28 2929 202f 2077 6377  t2.mean()) / wcw
-000173d0: 7432 2e73 7464 2829 0a20 2020 2020 2020  t2.std().       
-000173e0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000173f0: 2020 206e 6377 7431 203d 2077 6377 7431     ncwt1 = wcwt1
-00017400: 0a20 2020 2020 2020 2020 2020 206e 6377  .            ncw
-00017410: 7432 203d 2077 6377 7432 0a0a 2020 2020  t2 = wcwt2..    
-00017420: 2020 2020 2320 7275 6e20 7374 7265 7463      # run stretc
-00017430: 6869 6e67 0a20 2020 2020 2020 2064 7676  hing.        dvv
-00017440: 2c20 6572 722c 2063 632c 2063 6470 203d  , err, cc, cdp =
-00017450: 2073 7472 6574 6368 696e 6728 6e63 7774   stretching(ncwt
-00017460: 322c 206e 6377 7431 2c20 6476 5f72 616e  2, ncwt1, dv_ran
-00017470: 6765 2c20 6e62 7472 6961 6c2c 2070 6172  ge, nbtrial, par
-00017480: 6129 0a20 2020 2020 2020 2072 6574 7572  a).        retur
-00017490: 6e20 6476 762c 2065 7272 0a0a 2020 2020  n dvv, err..    
-000174a0: 2320 6469 7265 6374 6c79 2074 616b 6520  # directly take 
-000174b0: 6164 7661 6e74 6167 6520 6f66 2074 6865  advantage of the
-000174c0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-000174d0: 2020 2023 2069 6e69 7469 616c 697a 6520     # initialize 
-000174e0: 7661 7269 6162 6c65 0a20 2020 2020 2020  variable.       
-000174f0: 206e 6672 6571 203d 206c 656e 2866 7265   nfreq = len(fre
-00017500: 715f 696e 6469 6e29 0a20 2020 2020 2020  q_indin).       
-00017510: 2064 7676 2c20 6363 2c20 6364 702c 2065   dvv, cc, cdp, e
-00017520: 7272 203d 2028 0a20 2020 2020 2020 2020  rr = (.         
-00017530: 2020 206e 702e 7a65 726f 7328 6e66 7265     np.zeros(nfre
-00017540: 712c 2064 7479 7065 3d6e 702e 666c 6f61  q, dtype=np.floa
-00017550: 7433 3229 2c0a 2020 2020 2020 2020 2020  t32),.          
-00017560: 2020 6e70 2e7a 6572 6f73 286e 6672 6571    np.zeros(nfreq
-00017570: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
-00017580: 3332 292c 0a20 2020 2020 2020 2020 2020  32),.           
-00017590: 206e 702e 7a65 726f 7328 6e66 7265 712c   np.zeros(nfreq,
-000175a0: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
-000175b0: 3229 2c0a 2020 2020 2020 2020 2020 2020  2),.            
-000175c0: 6e70 2e7a 6572 6f73 286e 6672 6571 2c20  np.zeros(nfreq, 
-000175d0: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
-000175e0: 292c 0a20 2020 2020 2020 2029 0a0a 2020  ),.        )..  
-000175f0: 2020 2020 2020 2320 6c6f 6f70 2074 6872        # loop thr
-00017600: 6f75 6768 2065 6163 6820 6672 6571 0a20  ough each freq. 
-00017610: 2020 2020 2020 2066 6f72 2069 692c 2069         for ii, i
-00017620: 6672 6571 2069 6e20 656e 756d 6572 6174  freq in enumerat
-00017630: 6528 6672 6571 5f69 6e64 696e 293a 0a20  e(freq_indin):. 
-00017640: 2020 2020 2020 2020 2020 2023 2070 7265             # pre
-00017650: 7061 7265 2077 696e 646f 7765 6420 6461  pare windowed da
-00017660: 7461 0a20 2020 2020 2020 2020 2020 2077  ta.            w
-00017670: 6377 7431 2c20 7763 7774 3220 3d20 7263  cwt1, wcwt2 = rc
-00017680: 7774 315b 6966 7265 715d 2c20 7263 7774  wt1[ifreq], rcwt
-00017690: 325b 6966 7265 715d 0a0a 2020 2020 2020  2[ifreq]..      
-000176a0: 2020 2020 2020 2320 4e6f 726d 616c 697a        # Normaliz
-000176b0: 6573 2062 6f74 6820 7369 676e 616c 732c  es both signals,
-000176c0: 2069 6620 6170 7072 6f70 7269 6174 652e   if appropriate.
-000176d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000176e0: 6e6f 726d 616c 697a 653a 0a20 2020 2020  normalize:.     
-000176f0: 2020 2020 2020 2020 2020 206e 6377 7431             ncwt1
-00017700: 203d 2028 7763 7774 3120 2d20 7763 7774   = (wcwt1 - wcwt
-00017710: 312e 6d65 616e 2829 2920 2f20 7763 7774  1.mean()) / wcwt
-00017720: 312e 7374 6428 290a 2020 2020 2020 2020  1.std().        
-00017730: 2020 2020 2020 2020 6e63 7774 3220 3d20          ncwt2 = 
-00017740: 2877 6377 7432 202d 2077 6377 7432 2e6d  (wcwt2 - wcwt2.m
-00017750: 6561 6e28 2929 202f 2077 6377 7432 2e73  ean()) / wcwt2.s
-00017760: 7464 2829 0a20 2020 2020 2020 2020 2020  td().           
-00017770: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00017780: 2020 2020 2020 206e 6377 7431 203d 2077         ncwt1 = w
-00017790: 6377 7431 0a20 2020 2020 2020 2020 2020  cwt1.           
-000177a0: 2020 2020 206e 6377 7432 203d 2077 6377       ncwt2 = wcw
-000177b0: 7432 0a0a 2020 2020 2020 2020 2020 2020  t2..            
-000177c0: 2320 7275 6e20 7374 7265 7463 6869 6e67  # run stretching
-000177d0: 0a20 2020 2020 2020 2020 2020 2064 762c  .            dv,
-000177e0: 2065 7272 6f72 2c20 6331 2c20 6332 203d   error, c1, c2 =
-000177f0: 2073 7472 6574 6368 696e 6728 6e63 7774   stretching(ncwt
-00017800: 322c 206e 6377 7431 2c20 6476 5f72 616e  2, ncwt1, dv_ran
-00017810: 6765 2c20 6e62 7472 6961 6c2c 2070 6172  ge, nbtrial, par
-00017820: 6129 0a20 2020 2020 2020 2020 2020 2064  a).            d
-00017830: 7676 5b69 695d 2c20 6363 5b69 695d 2c20  vv[ii], cc[ii], 
-00017840: 6364 705b 6969 5d2c 2065 7272 5b69 695d  cdp[ii], err[ii]
-00017850: 203d 2064 762c 2063 312c 2063 322c 2065   = dv, c1, c2, e
-00017860: 7272 6f72 0a0a 2020 2020 2020 2020 7265  rror..        re
-00017870: 7475 726e 2066 7265 715b 6672 6571 5f69  turn freq[freq_i
-00017880: 6e64 696e 5d2c 2064 7676 2c20 6572 720a  ndin], dvv, err.
-00017890: 0a0a 6465 6620 7774 6474 775f 616c 6c66  ..def wtdtw_allf
-000178a0: 7265 7128 0a20 2020 2072 6566 2c0a 2020  req(.    ref,.  
-000178b0: 2020 6375 722c 0a20 2020 2061 6c6c 6672    cur,.    allfr
-000178c0: 6571 2c0a 2020 2020 7061 7261 2c0a 2020  eq,.    para,.  
-000178d0: 2020 6d61 784c 6167 2c0a 2020 2020 622c    maxLag,.    b,
-000178e0: 0a20 2020 2064 6972 6563 7469 6f6e 2c0a  .    direction,.
-000178f0: 2020 2020 646a 3d31 202f 2031 322c 0a20      dj=1 / 12,. 
-00017900: 2020 2073 303d 2d31 2c0a 2020 2020 4a3d     s0=-1,.    J=
-00017910: 2d31 2c0a 2020 2020 7776 6e3d 226d 6f72  -1,.    wvn="mor
-00017920: 6c65 7422 2c0a 2020 2020 6e6f 726d 616c  let",.    normal
-00017930: 697a 653d 5472 7565 2c0a 293a 0a20 2020  ize=True,.):.   
-00017940: 2022 2222 0a20 2020 2041 7070 6c79 2064   """.    Apply d
-00017950: 796e 616d 6963 2074 696d 6520 7761 7270  ynamic time warp
-00017960: 696e 6720 6d65 7468 6f64 2074 6f20 636f  ing method to co
-00017970: 6e74 696e 756f 7573 2077 6176 656c 6574  ntinuous wavelet
-00017980: 2074 7261 6e73 666f 726d 6174 696f 6e20   transformation 
-00017990: 2843 5754 2920 6f66 2073 6967 6e61 6c73  (CWT) of signals
-000179a0: 0a20 2020 2066 6f72 2061 6c6c 2066 7265  .    for all fre
-000179b0: 7175 6563 6965 7320 696e 2061 6e20 696e  quecies in an in
-000179c0: 7465 7265 7374 2072 616e 6765 0a0a 2020  terest range..  
-000179d0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-000179e0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a   --------------.
-000179f0: 2020 2020 7265 663a 2054 6865 2022 5265      ref: The "Re
-00017a00: 6665 7265 6e63 6522 2074 696d 6573 6572  ference" timeser
-00017a10: 6965 7320 286e 756d 7079 2e6e 6461 7272  ies (numpy.ndarr
-00017a20: 6179 290a 2020 2020 6375 723a 2054 6865  ay).    cur: The
-00017a30: 2022 4375 7272 656e 7422 2074 696d 6573   "Current" times
-00017a40: 6572 6965 7320 286e 756d 7079 2e6e 6461  eries (numpy.nda
-00017a50: 7272 6179 290a 2020 2020 616c 6c66 7265  rray).    allfre
-00017a60: 713a 2061 2062 6f6f 6c65 6e20 7661 7269  q: a boolen vari
-00017a70: 6162 6c65 2074 6f20 6d61 6b65 206d 6561  able to make mea
-00017a80: 7375 7265 6d65 6e74 7320 6f6e 2061 6c6c  surements on all
-00017a90: 2066 7265 7175 656e 6379 2072 616e 6765   frequency range
-00017aa0: 206f 7220 6e6f 740a 2020 2020 6d61 784c   or not.    maxL
-00017ab0: 6167 3a20 6d61 7820 6e75 6d62 6572 206f  ag: max number o
-00017ac0: 6620 706f 696e 7473 2074 6f20 7365 6172  f points to sear
-00017ad0: 6368 2066 6f72 7761 7264 2061 6e64 2062  ch forward and b
-00017ae0: 6163 6b77 6172 642e 0a20 2020 2062 3a20  ackward..    b: 
-00017af0: 622d 7661 6c75 6520 746f 206c 696d 6974  b-value to limit
-00017b00: 2073 7472 6169 6e2c 2077 6869 6368 2069   strain, which i
-00017b10: 7320 746f 206c 696d 6974 2074 6865 206d  s to limit the m
-00017b20: 6178 696d 756d 2076 656c 6f63 6974 7920  aximum velocity 
-00017b30: 7065 7274 7572 6261 7469 6f6e 2e0a 2020  perturbation..  
-00017b40: 2020 5365 6520 6571 7561 7469 6f6e 2031    See equation 1
-00017b50: 3120 696e 2028 4d69 6b65 7365 6c6c 2065  1 in (Mikesell e
-00017b60: 7420 616c 2e20 3230 3135 290a 2020 2020  t al. 2015).    
-00017b70: 6469 7265 6374 696f 6e3a 2064 6972 6563  direction: direc
-00017b80: 7469 6f6e 2074 6f20 6163 6375 6d75 6c61  tion to accumula
-00017b90: 7465 2065 7272 6f72 7320 2831 3d66 6f72  te errors (1=for
-00017ba0: 7761 7264 2c20 2d31 3d62 6163 6b77 6172  ward, -1=backwar
-00017bb0: 6429 0a20 2020 2064 6a2c 2073 302c 204a  d).    dj, s0, J
-00017bc0: 2c20 7369 672c 2077 766e 3a20 636f 6d6d  , sig, wvn: comm
-00017bd0: 6f6e 2070 6172 616d 6574 6572 7320 7573  on parameters us
-00017be0: 6564 2069 6e20 2777 6176 656c 6574 2e77  ed in 'wavelet.w
-00017bf0: 6374 270a 2020 2020 6e6f 726d 616c 697a  ct'.    normaliz
-00017c00: 653a 206e 6f72 6d61 6c69 7a65 2074 6865  e: normalize the
-00017c10: 2077 6176 656c 6574 2073 7065 6374 7275   wavelet spectru
-00017c20: 6d20 6f72 206e 6f74 2e20 4465 6661 756c  m or not. Defaul
-00017c30: 7420 6973 2054 7275 650a 0a20 2020 2052  t is True..    R
-00017c40: 4554 5552 4e53 3a0a 2020 2020 2d2d 2d2d  ETURNS:.    ----
-00017c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
-00017c60: 2020 2064 7676 3a20 6573 7469 6d61 7465     dvv: estimate
-00017c70: 6420 6476 2f76 0a20 2020 2065 7272 3a20  d dv/v.    err: 
-00017c80: 6572 726f 7220 6f66 2064 762f 7620 6573  error of dv/v es
-00017c90: 7469 6d61 7469 6f6e 0a0a 2020 2020 5772  timation..    Wr
-00017ca0: 6974 7465 6e20 6279 2043 6f6e 6763 6f6e  itten by Congcon
-00017cb0: 6720 5975 616e 2028 3330 204a 756e 2c20  g Yuan (30 Jun, 
-00017cc0: 3230 3139 290a 2020 2020 2222 220a 2020  2019).    """.  
-00017cd0: 2020 2320 636f 6d6d 6f6e 2076 6172 6961    # common varia
-00017ce0: 626c 6573 0a20 2020 2066 7265 7120 3d20  bles.    freq = 
-00017cf0: 7061 7261 5b22 6672 6571 225d 0a20 2020  para["freq"].   
-00017d00: 2064 7420 3d20 7061 7261 5b22 6474 225d   dt = para["dt"]
-00017d10: 0a20 2020 2066 6d69 6e20 3d20 6e70 2e6d  .    fmin = np.m
-00017d20: 696e 2866 7265 7129 0a20 2020 2066 6d61  in(freq).    fma
-00017d30: 7820 3d20 6e70 2e6d 6178 2866 7265 7129  x = np.max(freq)
-00017d40: 0a0a 2020 2020 2320 6170 706c 7920 6377  ..    # apply cw
-00017d50: 7420 6f6e 2074 776f 2074 7261 6365 730a  t on two traces.
-00017d60: 2020 2020 6377 7431 2c20 736a 2c20 6672      cwt1, sj, fr
-00017d70: 6571 2c20 636f 692c 205f 2c20 5f20 3d20  eq, coi, _, _ = 
-00017d80: 7079 6377 742e 6377 7428 6375 722c 2064  pycwt.cwt(cur, d
-00017d90: 742c 2064 6a2c 2073 302c 204a 2c20 7776  t, dj, s0, J, wv
-00017da0: 6e29 0a20 2020 2063 7774 322c 2073 6a2c  n).    cwt2, sj,
-00017db0: 2066 7265 712c 2063 6f69 2c20 5f2c 205f   freq, coi, _, _
-00017dc0: 203d 2070 7963 7774 2e63 7774 2872 6566   = pycwt.cwt(ref
-00017dd0: 2c20 6474 2c20 646a 2c20 7330 2c20 4a2c  , dt, dj, s0, J,
-00017de0: 2077 766e 290a 0a20 2020 2023 2065 7874   wvn)..    # ext
-00017df0: 7261 6374 2072 6561 6c20 7661 6c75 6573  ract real values
-00017e00: 206f 6620 6377 740a 2020 2020 7263 7774   of cwt.    rcwt
-00017e10: 312c 2072 6377 7432 203d 206e 702e 7265  1, rcwt2 = np.re
-00017e20: 616c 2863 7774 3129 2c20 6e70 2e72 6561  al(cwt1), np.rea
-00017e30: 6c28 6377 7432 290a 0a20 2020 2023 207a  l(cwt2)..    # z
-00017e40: 6572 6f20 6f75 7420 636f 6e65 206f 6620  ero out cone of 
-00017e50: 696e 666c 7565 6e63 6520 616e 6420 6461  influence and da
-00017e60: 7461 206f 7574 7369 6465 2066 7265 7175  ta outside frequ
-00017e70: 656e 6379 2062 616e 640a 2020 2020 6966  ency band.    if
-00017e80: 2028 666d 6178 203e 206e 702e 6d61 7828   (fmax > np.max(
-00017e90: 6672 6571 2929 207c 2028 666d 6178 203c  freq)) | (fmax <
-00017ea0: 3d20 666d 696e 293a 0a20 2020 2020 2020  = fmin):.       
-00017eb0: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00017ec0: 7228 2241 626f 7274 3a20 696e 7075 7420  r("Abort: input 
-00017ed0: 6672 6571 7565 6e63 7920 6f75 7420 6f66  frequency out of
-00017ee0: 206c 696d 6974 7321 2229 0a20 2020 2065   limits!").    e
-00017ef0: 6c73 653a 0a20 2020 2020 2020 2066 7265  lse:.        fre
-00017f00: 715f 696e 6469 6e20 3d20 6e70 2e77 6865  q_indin = np.whe
-00017f10: 7265 2828 6672 6571 203e 3d20 666d 696e  re((freq >= fmin
-00017f20: 2920 2620 2866 7265 7120 3c3d 2066 6d61  ) & (freq <= fma
-00017f30: 7829 295b 305d 0a0a 2020 2020 2020 2020  x))[0]..        
-00017f40: 2320 5573 6520 4454 5720 6d65 7468 6f64  # Use DTW method
-00017f50: 2074 6f20 6578 7472 6163 7420 6476 760a   to extract dvv.
-00017f60: 2020 2020 2020 2020 6e66 7265 7120 3d20          nfreq = 
-00017f70: 6c65 6e28 6672 6571 5f69 6e64 696e 290a  len(freq_indin).
-00017f80: 2020 2020 2020 2020 6476 762c 2065 7272          dvv, err
-00017f90: 203d 206e 702e 7a65 726f 7328 6e66 7265   = np.zeros(nfre
-00017fa0: 712c 2064 7479 7065 3d6e 702e 666c 6f61  q, dtype=np.floa
-00017fb0: 7433 3229 2c20 6e70 2e7a 6572 6f73 286e  t32), np.zeros(n
-00017fc0: 6672 6571 2c20 6474 7970 653d 6e70 2e66  freq, dtype=np.f
-00017fd0: 6c6f 6174 3332 290a 0a20 2020 2020 2020  loat32)..       
-00017fe0: 2066 6f72 2069 692c 2069 6672 6571 2069   for ii, ifreq i
-00017ff0: 6e20 656e 756d 6572 6174 6528 6672 6571  n enumerate(freq
-00018000: 5f69 6e64 696e 293a 0a20 2020 2020 2020  _indin):.       
-00018010: 2020 2020 2023 2070 7265 7061 7265 2077       # prepare w
-00018020: 696e 646f 7765 6420 6461 7461 0a20 2020  indowed data.   
-00018030: 2020 2020 2020 2020 2077 6377 7431 2c20           wcwt1, 
-00018040: 7763 7774 3220 3d20 7263 7774 315b 6966  wcwt2 = rcwt1[if
-00018050: 7265 715d 2c20 7263 7774 325b 6966 7265  req], rcwt2[ifre
-00018060: 715d 0a20 2020 2020 2020 2020 2020 2023  q].            #
-00018070: 204e 6f72 6d61 6c69 7a65 7320 626f 7468   Normalizes both
-00018080: 2073 6967 6e61 6c73 2c20 6966 2061 7070   signals, if app
-00018090: 726f 7072 6961 7465 2e0a 2020 2020 2020  ropriate..      
-000180a0: 2020 2020 2020 6966 206e 6f72 6d61 6c69        if normali
-000180b0: 7a65 3a0a 2020 2020 2020 2020 2020 2020  ze:.            
-000180c0: 2020 2020 6e63 7774 3120 3d20 2877 6377      ncwt1 = (wcw
-000180d0: 7431 202d 2077 6377 7431 2e6d 6561 6e28  t1 - wcwt1.mean(
-000180e0: 2929 202f 2077 6377 7431 2e73 7464 2829  )) / wcwt1.std()
-000180f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018100: 206e 6377 7432 203d 2028 7763 7774 3220   ncwt2 = (wcwt2 
-00018110: 2d20 7763 7774 322e 6d65 616e 2829 2920  - wcwt2.mean()) 
-00018120: 2f20 7763 7774 322e 7374 6428 290a 2020  / wcwt2.std().  
-00018130: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00018140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018150: 6e63 7774 3120 3d20 7763 7774 310a 2020  ncwt1 = wcwt1.  
-00018160: 2020 2020 2020 2020 2020 2020 2020 6e63                nc
-00018170: 7774 3220 3d20 7763 7774 320a 0a20 2020  wt2 = wcwt2..   
-00018180: 2020 2020 2020 2020 2023 2072 756e 2064           # run d
-00018190: 7477 0a20 2020 2020 2020 2020 2020 2064  tw.            d
-000181a0: 762c 2065 7272 6f72 2c20 6469 7374 203d  v, error, dist =
-000181b0: 2064 7477 5f64 7676 286e 6377 7432 2c20   dtw_dvv(ncwt2, 
-000181c0: 6e63 7774 312c 2070 6172 612c 206d 6178  ncwt1, para, max
-000181d0: 4c61 672c 2062 2c20 6469 7265 6374 696f  Lag, b, directio
-000181e0: 6e29 0a20 2020 2020 2020 2020 2020 2064  n).            d
-000181f0: 7676 5b69 695d 2c20 6572 725b 6969 5d20  vv[ii], err[ii] 
-00018200: 3d20 6476 2c20 6572 726f 720a 0a20 2020  = dv, error..   
-00018210: 2064 656c 2063 7774 312c 2063 7774 322c   del cwt1, cwt2,
-00018220: 2072 6377 7431 2c20 7263 7774 322c 206e   rcwt1, rcwt2, n
-00018230: 6377 7431 2c20 6e63 7774 322c 2077 6377  cwt1, ncwt2, wcw
-00018240: 7431 2c20 7763 7774 322c 2063 6f69 2c20  t1, wcwt2, coi, 
-00018250: 736a 2c20 6469 7374 0a0a 2020 2020 6966  sj, dist..    if
-00018260: 206e 6f74 2061 6c6c 6672 6571 3a0a 2020   not allfreq:.  
-00018270: 2020 2020 2020 7265 7475 726e 206e 702e        return np.
-00018280: 6d65 616e 2864 7676 292c 206e 702e 6d65  mean(dvv), np.me
-00018290: 616e 2865 7272 290a 2020 2020 656c 7365  an(err).    else
-000182a0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-000182b0: 2066 7265 715b 6672 6571 5f69 6e64 696e   freq[freq_indin
-000182c0: 5d2c 2064 7676 2c20 6572 720a 0a0a 2323  ], dvv, err...##
-000182d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000182e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000182f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00018300: 2323 2323 2323 2323 2323 230a 2323 2323  ###########.####
-00018310: 2323 2323 2323 2323 2323 2323 204d 4f4e  ############ MON
-00018320: 4954 4f52 494e 4720 5554 494c 4954 5920  ITORING UTILITY 
-00018330: 4655 4e43 5449 4f4e 5320 2323 2323 2323  FUNCTIONS ######
-00018340: 2323 2323 2323 2323 230a 2323 2323 2323  #########.######
-00018350: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00018360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00018370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00018380: 2323 2323 2323 230a 0a22 2222 0a62 656c  #######..""".bel
-00018390: 6f77 2061 7265 2061 7373 656d 626c 7920  ow are assembly 
-000183a0: 6f66 2074 6865 206d 6f6e 6974 6f72 696e  of the monitorin
-000183b0: 6720 7574 696c 6974 7920 6675 6e63 7469  g utility functi
-000183c0: 6f6e 7320 6361 6c6c 6564 2062 7920 6d6f  ons called by mo
-000183d0: 6e69 746f 7269 6e67 2066 756e 6374 696f  nitoring functio
-000183e0: 6e73 0a22 2222 0a0a 0a64 6566 2073 6d6f  ns."""...def smo
-000183f0: 6f74 6828 782c 2077 696e 646f 773d 2262  oth(x, window="b
-00018400: 6f78 6361 7222 2c20 6861 6c66 5f77 696e  oxcar", half_win
-00018410: 3d33 293a 0a20 2020 2022 2222 0a20 2020  =3):.    """.   
-00018420: 2070 6572 666f 726d 7320 736d 6f6f 7468   performs smooth
-00018430: 696e 6720 696e 2069 6e74 6572 6573 7465  ing in intereste
-00018440: 6420 7469 6d65 2077 696e 646f 770a 0a20  d time window.. 
-00018450: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00018460: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
-00018470: 0a20 2020 2078 3a20 7469 6d65 7365 7269  .    x: timeseri
-00018480: 7320 6461 7461 0a20 2020 2077 696e 646f  s data.    windo
-00018490: 773a 2074 7970 6573 206f 6620 7769 6e64  w: types of wind
-000184a0: 6f77 2074 6f20 646f 2073 6d6f 6f74 6869  ow to do smoothi
-000184b0: 6e67 0a20 2020 2068 616c 665f 7769 6e3a  ng.    half_win:
-000184c0: 2068 616c 6620 7769 6e64 6f77 206c 656e   half window len
-000184d0: 6774 680a 0a20 2020 2052 4554 5552 4e53  gth..    RETURNS
-000184e0: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  :.    ----------
-000184f0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2079 3a20  --------.    y: 
-00018500: 736d 6f6f 7468 6564 2074 696d 6520 7769  smoothed time wi
-00018510: 6e64 6f77 0a20 2020 2022 2222 0a20 2020  ndow.    """.   
-00018520: 2023 2054 4f44 4f3a 2064 6f63 7374 696e   # TODO: docstin
-00018530: 670a 2020 2020 7769 6e64 6f77 5f6c 656e  g.    window_len
-00018540: 203d 2032 202a 2068 616c 665f 7769 6e20   = 2 * half_win 
-00018550: 2b20 310a 2020 2020 2320 6578 7465 6e64  + 1.    # extend
-00018560: 696e 6720 7468 6520 6461 7461 2061 7420  ing the data at 
-00018570: 6265 6769 6e6e 696e 6720 616e 6420 6174  beginning and at
-00018580: 2074 6865 2065 6e64 0a20 2020 2023 2074   the end.    # t
-00018590: 6f20 6170 706c 7920 7468 6520 7769 6e64  o apply the wind
-000185a0: 6f77 2061 7420 7468 6520 626f 7264 6572  ow at the border
-000185b0: 730a 2020 2020 7320 3d20 6e70 2e72 5f5b  s.    s = np.r_[
-000185c0: 785b 7769 6e64 6f77 5f6c 656e 202d 2031  x[window_len - 1
-000185d0: 203a 2030 203a 202d 315d 2c20 782c 2078   : 0 : -1], x, x
-000185e0: 5b2d 313a 2d77 696e 646f 775f 6c65 6e3a  [-1:-window_len:
-000185f0: 2d31 5d5d 0a20 2020 2069 6620 7769 6e64  -1]].    if wind
-00018600: 6f77 203d 3d20 2262 6f78 6361 7222 3a0a  ow == "boxcar":.
-00018610: 2020 2020 2020 2020 7720 3d20 7363 6970          w = scip
-00018620: 792e 7369 676e 616c 2e62 6f78 6361 7228  y.signal.boxcar(
-00018630: 7769 6e64 6f77 5f6c 656e 292e 6173 7479  window_len).asty
-00018640: 7065 2822 636f 6d70 6c65 7822 290a 2020  pe("complex").  
-00018650: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00018660: 7720 3d20 7363 6970 792e 7369 676e 616c  w = scipy.signal
-00018670: 2e68 616e 6e69 6e67 2877 696e 646f 775f  .hanning(window_
-00018680: 6c65 6e29 2e61 7374 7970 6528 2263 6f6d  len).astype("com
-00018690: 706c 6578 2229 0a20 2020 2079 203d 206e  plex").    y = n
-000186a0: 702e 636f 6e76 6f6c 7665 2877 202f 2077  p.convolve(w / w
-000186b0: 2e73 756d 2829 2c20 732c 206d 6f64 653d  .sum(), s, mode=
-000186c0: 2276 616c 6964 2229 0a20 2020 2072 6574  "valid").    ret
-000186d0: 7572 6e20 795b 6861 6c66 5f77 696e 203a  urn y[half_win :
-000186e0: 206c 656e 2879 2920 2d20 6861 6c66 5f77   len(y) - half_w
-000186f0: 696e 5d0a 0a0a 6465 6620 6e65 7874 706f  in]...def nextpo
-00018700: 7732 2878 293a 0a20 2020 2022 2222 0a20  w2(x):.    """. 
-00018710: 2020 2052 6574 7572 6e73 2074 6865 206e     Returns the n
-00018720: 6578 7420 706f 7765 7220 6f66 2032 206f  ext power of 2 o
-00018730: 6620 782e 0a20 2020 2022 2222 0a20 2020  f x..    """.   
-00018740: 2072 6574 7572 6e20 696e 7428 6e70 2e63   return int(np.c
-00018750: 6569 6c28 6e70 2e6c 6f67 3228 6e70 2e61  eil(np.log2(np.a
-00018760: 6273 2878 2929 2929 0a0a 0a64 6566 2067  bs(x))))...def g
-00018770: 6574 436f 6865 7265 6e63 6528 6463 732c  etCoherence(dcs,
-00018780: 2064 7331 2c20 6473 3229 3a0a 2020 2020   ds1, ds2):.    
-00018790: 2222 220a 2020 2020 6765 7420 6372 6f73  """.    get cros
-000187a0: 7320 636f 6865 7265 6e63 6520 6265 7477  s coherence betw
-000187b0: 6565 6e20 7265 6665 7265 6e63 6520 616e  een reference an
-000187c0: 6420 6375 7272 656e 7420 7761 7665 666f  d current wavefo
-000187d0: 726d 7320 666f 6c6c 6f77 696e 6720 6571  rms following eq
-000187e0: 7561 7469 6f6e 206f 6620 4133 2069 6e20  uation of A3 in 
-000187f0: 436c 6172 6b20 6574 2061 6c2e 2c20 3230  Clark et al., 20
-00018800: 3131 0a0a 2020 2020 5061 7261 6d65 7465  11..    Paramete
-00018810: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-00018820: 2d2d 2d2d 2d0a 2020 2020 6463 733a 2061  -----.    dcs: a
-00018830: 6d70 6c69 7475 6465 206f 6620 7468 6520  mplitude of the 
-00018840: 6372 6f73 7320 7370 6563 7472 756d 0a20  cross spectrum. 
-00018850: 2020 2064 7331 3a20 616d 706c 6974 7564     ds1: amplitud
-00018860: 6520 6f66 2074 6865 2073 7065 6374 7275  e of the spectru
-00018870: 6d20 6f66 2063 7572 7265 6e74 2077 6176  m of current wav
-00018880: 6566 6f72 6d0a 2020 2020 6473 323a 2061  eform.    ds2: a
-00018890: 6d70 6c69 7475 6465 206f 6620 7468 6520  mplitude of the 
-000188a0: 7370 6563 7472 756d 206f 6620 7265 6665  spectrum of refe
-000188b0: 7265 6e63 6520 7761 7665 666f 726d 0a0a  rence waveform..
-000188c0: 2020 2020 5245 5455 524e 533a 0a20 2020      RETURNS:.   
-000188d0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-000188e0: 2d2d 2d0a 2020 2020 636f 683a 2063 6f68  ---.    coh: coh
-000188f0: 7265 7265 6e63 7920 6d61 7472 6978 2075  rerency matrix u
-00018900: 7365 6420 666f 7220 6573 7469 6d61 7465  sed for estimate
-00018910: 2074 6865 2072 6f62 7573 746e 6573 7320   the robustness 
-00018920: 6f66 2074 6865 2063 726f 7373 2073 7065  of the cross spe
-00018930: 6374 7275 6d0a 2020 2020 2222 220a 2020  ctrum.    """.  
-00018940: 2020 6e20 3d20 6c65 6e28 6463 7329 0a20    n = len(dcs). 
-00018950: 2020 2063 6f68 203d 206e 702e 7a65 726f     coh = np.zero
-00018960: 7328 6e29 2e61 7374 7970 6528 2263 6f6d  s(n).astype("com
-00018970: 706c 6578 2229 0a20 2020 2076 616c 6964  plex").    valid
-00018980: 7320 3d20 6e70 2e61 7267 7768 6572 6528  s = np.argwhere(
-00018990: 6e70 2e6c 6f67 6963 616c 5f61 6e64 286e  np.logical_and(n
-000189a0: 702e 6162 7328 6473 3129 203e 2030 2c20  p.abs(ds1) > 0, 
-000189b0: 6e70 2e61 6273 2864 7332 2920 3e20 3029  np.abs(ds2) > 0)
-000189c0: 290a 2020 2020 636f 685b 7661 6c69 6473  ).    coh[valids
-000189d0: 5d20 3d20 6463 735b 7661 6c69 6473 5d20  ] = dcs[valids] 
-000189e0: 2f20 2864 7331 5b76 616c 6964 735d 202a  / (ds1[valids] *
-000189f0: 2064 7332 5b76 616c 6964 735d 290a 2020   ds2[valids]).  
-00018a00: 2020 636f 685b 636f 6820 3e20 2831 2e30    coh[coh > (1.0
-00018a10: 202b 2030 6a29 5d20 3d20 312e 3020 2b20   + 0j)] = 1.0 + 
-00018a20: 306a 0a20 2020 2072 6574 7572 6e20 636f  0j.    return co
-00018a30: 680a 0a0a 6465 6620 636f 6d70 7574 6545  h...def computeE
-00018a40: 7272 6f72 4675 6e63 7469 6f6e 2875 312c  rrorFunction(u1,
-00018a50: 2075 302c 206e 5361 6d70 6c65 2c20 6c61   u0, nSample, la
-00018a60: 672c 206e 6f72 6d3d 224c 3222 293a 0a20  g, norm="L2"):. 
-00018a70: 2020 2022 2222 0a20 2020 2063 6f6d 7075     """.    compu
-00018a80: 7465 2045 7272 6f72 2046 756e 6374 696f  te Error Functio
-00018a90: 6e20 7573 6564 2069 6e20 4454 572e 2054  n used in DTW. T
-00018aa0: 6865 2065 7272 6f72 2066 756e 6374 696f  he error functio
-00018ab0: 6e20 6973 2065 7175 6174 696f 6e20 3120  n is equation 1 
-00018ac0: 696e 2048 616c 652c 2032 3031 332e 2059  in Hale, 2013. Y
-00018ad0: 6f75 2063 6f75 6c64 2075 6e63 6f6d 6d65  ou could uncomme
-00018ae0: 6e74 2074 6865 0a20 2020 204c 3120 6e6f  nt the.    L1 no
-00018af0: 726d 2061 6e64 2063 6f6d 6d65 6e74 2074  rm and comment t
-00018b00: 6865 204c 3220 6e6f 726d 2069 6620 796f  he L2 norm if yo
-00018b10: 7520 7761 6e74 206f 6e20 4c69 6e65 2032  u want on Line 2
-00018b20: 390a 0a20 2020 2050 6172 616d 6574 6572  9..    Parameter
-00018b30: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-00018b40: 2d2d 2d2d 0a20 2020 2075 313a 2020 7472  ----.    u1:  tr
-00018b50: 6163 6520 7468 6174 2077 6520 7761 6e74  ace that we want
-00018b60: 2074 6f20 7761 7270 3b20 7369 7a65 203d   to warp; size =
-00018b70: 2028 6e73 616d 702c 3129 0a20 2020 2075   (nsamp,1).    u
-00018b80: 303a 2020 7265 6665 7265 6e63 6520 7472  0:  reference tr
-00018b90: 6163 6520 746f 2063 6f6d 7061 7265 2077  ace to compare w
-00018ba0: 6974 683a 2073 697a 6520 3d20 286e 7361  ith: size = (nsa
-00018bb0: 6d70 2c31 290a 2020 2020 6e53 616d 706c  mp,1).    nSampl
-00018bc0: 653a 206e 756d 6572 206f 6620 706f 696e  e: numer of poin
-00018bd0: 7473 2074 6f20 636f 6d70 6172 6520 696e  ts to compare in
-00018be0: 2074 6865 2074 7261 6365 730a 2020 2020   the traces.    
-00018bf0: 6c61 673a 206d 6178 696d 756d 206c 6167  lag: maximum lag
-00018c00: 2069 6e20 7361 6d70 6c65 206e 756d 6265   in sample numbe
-00018c10: 7220 746f 2073 6561 7263 680a 2020 2020  r to search.    
-00018c20: 6e6f 726d 3a20 274c 3227 206f 7220 274c  norm: 'L2' or 'L
-00018c30: 3127 2028 6465 6661 756c 7420 6973 2027  1' (default is '
-00018c40: 4c32 2729 0a0a 2020 2020 5245 5455 524e  L2')..    RETURN
-00018c50: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
-00018c60: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6572  ---------.    er
-00018c70: 723a 2074 6865 2032 4420 6572 726f 7220  r: the 2D error 
-00018c80: 6675 6e63 7469 6f6e 3b20 7369 7a65 203d  function; size =
-00018c90: 2028 6e73 616d 702c 322a 6c61 672b 3129   (nsamp,2*lag+1)
-00018ca0: 0a0a 2020 2020 4f72 6967 696e 616c 2062  ..    Original b
-00018cb0: 7920 4469 2059 616e 670a 2020 2020 4c61  y Di Yang.    La
-00018cc0: 7374 206d 6f64 6966 6965 6420 6279 2044  st modified by D
-00018cd0: 796c 616e 204d 696b 6573 656c 6c20 2832  ylan Mikesell (2
-00018ce0: 3520 4665 622e 2032 3031 3529 0a20 2020  5 Feb. 2015).   
-00018cf0: 2054 7261 6e73 6c61 7465 6420 746f 2070   Translated to p
-00018d00: 7974 686f 6e20 6279 2054 696d 2043 6c65  ython by Tim Cle
-00018d10: 6d65 6e74 7320 2831 3720 4175 672e 2032  ments (17 Aug. 2
-00018d20: 3031 3829 0a0a 2020 2020 2222 220a 0a20  018)..    """.. 
-00018d30: 2020 2069 6620 6c61 6720 3e3d 206e 5361     if lag >= nSa
-00018d40: 6d70 6c65 3a0a 2020 2020 2020 2020 7261  mple:.        ra
-00018d50: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
-00018d60: 636f 6d70 7574 6545 7272 6f72 4675 6e63  computeErrorFunc
-00018d70: 7469 6f6e 3a6c 6167 5072 6f62 6c65 6d22  tion:lagProblem"
-00018d80: 2c20 226c 6167 206d 7573 7420 6265 2073  , "lag must be s
-00018d90: 6d61 6c6c 6572 2074 6861 6e20 6e53 616d  maller than nSam
-00018da0: 706c 6522 290a 0a20 2020 2023 2041 6c6c  ple")..    # All
-00018db0: 6f63 6174 6520 6572 726f 7220 6675 6e63  ocate error func
-00018dc0: 7469 6f6e 2076 6172 6961 626c 650a 2020  tion variable.  
-00018dd0: 2020 6572 7220 3d20 6e70 2e7a 6572 6f73    err = np.zeros
-00018de0: 285b 6e53 616d 706c 652c 2032 202a 206c  ([nSample, 2 * l
-00018df0: 6167 202b 2031 5d29 0a0a 2020 2020 2320  ag + 1])..    # 
-00018e00: 696e 6974 6961 6c20 6572 726f 7220 6361  initial error ca
-00018e10: 6c63 756c 6174 696f 6e0a 2020 2020 2320  lculation.    # 
-00018e20: 6c6f 6f70 206f 7665 7220 6c61 6773 0a20  loop over lags. 
-00018e30: 2020 2066 6f72 206c 6c20 696e 206e 702e     for ll in np.
-00018e40: 6172 616e 6765 282d 6c61 672c 206c 6167  arange(-lag, lag
-00018e50: 202b 2031 293a 0a20 2020 2020 2020 2074   + 1):.        t
-00018e60: 6869 734c 6167 203d 206c 6c20 2b20 6c61  hisLag = ll + la
-00018e70: 670a 0a20 2020 2020 2020 2023 206c 6f6f  g..        # loo
-00018e80: 7020 6f76 6572 2073 616d 706c 6573 0a20  p over samples. 
-00018e90: 2020 2020 2020 2066 6f72 2069 6920 696e         for ii in
-00018ea0: 2072 616e 6765 286e 5361 6d70 6c65 293a   range(nSample):
-00018eb0: 0a20 2020 2020 2020 2020 2020 2023 2073  .            # s
-00018ec0: 6b69 7020 636f 726e 6572 7320 666f 7220  kip corners for 
-00018ed0: 6e6f 772c 2077 6520 7769 6c6c 2063 6f6d  now, we will com
-00018ee0: 6520 6261 636b 2074 6f20 7468 6573 650a  e back to these.
-00018ef0: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00018f00: 6969 202b 206c 6c20 3e3d 2030 2920 2620  ii + ll >= 0) & 
-00018f10: 2869 6920 2b20 6c6c 203c 206e 5361 6d70  (ii + ll < nSamp
-00018f20: 6c65 293a 0a20 2020 2020 2020 2020 2020  le):.           
-00018f30: 2020 2020 2065 7272 5b69 692c 2074 6869       err[ii, thi
-00018f40: 734c 6167 5d20 3d20 7531 5b69 695d 202d  sLag] = u1[ii] -
-00018f50: 2075 305b 6969 202b 206c 6c5d 0a0a 2020   u0[ii + ll]..  
-00018f60: 2020 6966 206e 6f72 6d20 3d3d 2022 4c32    if norm == "L2
-00018f70: 223a 0a20 2020 2020 2020 2065 7272 203d  ":.        err =
-00018f80: 2065 7272 2a2a 320a 2020 2020 656c 6966   err**2.    elif
-00018f90: 206e 6f72 6d20 3d3d 2022 4c31 223a 0a20   norm == "L1":. 
-00018fa0: 2020 2020 2020 2065 7272 203d 206e 702e         err = np.
-00018fb0: 6162 7328 6572 7229 0a0a 2020 2020 2320  abs(err)..    # 
-00018fc0: 4e6f 7720 6669 7820 636f 726e 6572 7320  Now fix corners 
-00018fd0: 7769 7468 2063 6f6e 7374 616e 7420 6578  with constant ex
-00018fe0: 7472 6170 6f6c 6174 696f 6e0a 2020 2020  trapolation.    
-00018ff0: 666f 7220 6c6c 2069 6e20 6e70 2e61 7261  for ll in np.ara
-00019000: 6e67 6528 2d6c 6167 2c20 6c61 6720 2b20  nge(-lag, lag + 
-00019010: 3129 3a0a 2020 2020 2020 2020 7468 6973  1):.        this
-00019020: 4c61 6720 3d20 6c6c 202b 206c 6167 0a0a  Lag = ll + lag..
-00019030: 2020 2020 2020 2020 666f 7220 6969 2069          for ii i
-00019040: 6e20 7261 6e67 6528 6e53 616d 706c 6529  n range(nSample)
-00019050: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00019060: 2069 6920 2b20 6c6c 203c 2030 3a0a 2020   ii + ll < 0:.  
-00019070: 2020 2020 2020 2020 2020 2020 2020 6572                er
-00019080: 725b 6969 2c20 7468 6973 4c61 675d 203d  r[ii, thisLag] =
-00019090: 2065 7272 5b2d 6c6c 2c20 7468 6973 4c61   err[-ll, thisLa
-000190a0: 675d 0a0a 2020 2020 2020 2020 2020 2020  g]..            
-000190b0: 656c 6966 2069 6920 2b20 6c6c 203e 206e  elif ii + ll > n
-000190c0: 5361 6d70 6c65 202d 2031 3a0a 2020 2020  Sample - 1:.    
-000190d0: 2020 2020 2020 2020 2020 2020 6572 725b              err[
-000190e0: 6969 2c20 7468 6973 4c61 675d 203d 2065  ii, thisLag] = e
-000190f0: 7272 5b6e 5361 6d70 6c65 202d 206c 6c20  rr[nSample - ll 
-00019100: 2d20 312c 2074 6869 734c 6167 5d0a 0a20  - 1, thisLag].. 
-00019110: 2020 2072 6574 7572 6e20 6572 720a 0a0a     return err...
-00019120: 6465 6620 6163 6375 6d75 6c61 7465 4572  def accumulateEr
-00019130: 726f 7246 756e 6374 696f 6e28 6469 722c  rorFunction(dir,
-00019140: 2065 7272 2c20 6e53 616d 706c 652c 206c   err, nSample, l
-00019150: 6167 2c20 6229 3a0a 2020 2020 2222 220a  ag, b):.    """.
-00019160: 2020 2020 6163 6375 6d75 6c61 7469 6f6e      accumulation
-00019170: 206f 6620 7468 6520 6572 726f 722c 2077   of the error, w
-00019180: 6869 6368 2066 6f6c 6c6f 7773 2074 6865  hich follows the
-00019190: 2065 7175 6174 696f 6e20 3620 696e 2048   equation 6 in H
-000191a0: 616c 652c 2032 3031 332e 0a0a 2020 2020  ale, 2013...    
-000191b0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-000191c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-000191d0: 2020 6469 723a 2061 6363 756d 756c 6174    dir: accumulat
-000191e0: 696f 6e20 6469 7265 6374 696f 6e20 2820  ion direction ( 
-000191f0: 6469 7220 3e20 3020 3d20 666f 7277 6172  dir > 0 = forwar
-00019200: 6420 696e 2074 696d 652c 2064 6972 203c  d in time, dir <
-00019210: 3d20 3020 3d20 6261 636b 7761 7264 2069  = 0 = backward i
-00019220: 6e20 7469 6d65 290a 2020 2020 6572 723a  n time).    err:
-00019230: 2074 6865 2032 4420 6572 726f 7220 6675   the 2D error fu
-00019240: 6e63 7469 6f6e 3b20 7369 7a65 203d 2028  nction; size = (
-00019250: 6e73 616d 702c 322a 6c61 672b 3129 0a20  nsamp,2*lag+1). 
-00019260: 2020 206e 5361 6d70 6c65 3a20 6e75 6d65     nSample: nume
-00019270: 7220 6f66 2070 6f69 6e74 7320 746f 2063  r of points to c
-00019280: 6f6d 7061 7265 2069 6e20 7468 6520 7472  ompare in the tr
-00019290: 6163 6573 0a20 2020 206c 6167 3a20 6d61  aces.    lag: ma
-000192a0: 7869 6d75 6d20 6c61 6720 696e 2073 616d  ximum lag in sam
-000192b0: 706c 6520 6e75 6d62 6572 2074 6f20 7365  ple number to se
-000192c0: 6172 6368 0a20 2020 2062 3a20 7374 7261  arch.    b: stra
-000192d0: 696e 206c 696d 6974 2028 696e 7465 6765  in limit (intege
-000192e0: 7220 7661 6c75 6520 3e3d 2031 290a 0a20  r value >= 1).. 
-000192f0: 2020 2052 4554 5552 4e53 3a0a 2020 2020     RETURNS:.    
-00019300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00019310: 2d2d 0a20 2020 2064 3a20 7468 6520 3244  --.    d: the 2D
-00019320: 2064 6973 7461 6e63 6520 6675 6e63 7469   distance functi
-00019330: 6f6e 3b20 7369 7a65 203d 2028 6e73 616d  on; size = (nsam
-00019340: 702c 322a 6c61 672b 3129 0a0a 2020 2020  p,2*lag+1)..    
-00019350: 4f72 6967 696e 616c 2062 7920 4469 2059  Original by Di Y
-00019360: 616e 670a 2020 2020 4c61 7374 206d 6f64  ang.    Last mod
-00019370: 6966 6965 6420 6279 2044 796c 616e 204d  ified by Dylan M
-00019380: 696b 6573 656c 6c20 2832 3520 4665 622e  ikesell (25 Feb.
-00019390: 2032 3031 3529 0a20 2020 2054 7261 6e73   2015).    Trans
-000193a0: 6c61 7465 6420 746f 2070 7974 686f 6e20  lated to python 
-000193b0: 6279 2054 696d 2043 6c65 6d65 6e74 7320  by Tim Clements 
-000193c0: 2831 3720 4175 672e 2032 3031 3829 0a0a  (17 Aug. 2018)..
-000193d0: 2020 2020 2222 220a 0a20 2020 2023 206e      """..    # n
-000193e0: 756d 6265 7220 6f66 206c 6167 7320 6672  umber of lags fr
-000193f0: 6f6d 205b 202d 6c61 6720 3a20 2b6c 6167  om [ -lag : +lag
-00019400: 205d 0a20 2020 206e 4c61 6720 3d20 2832   ].    nLag = (2
-00019410: 202a 206c 6167 2920 2b20 310a 0a20 2020   * lag) + 1..   
-00019420: 2023 2061 6c6c 6f63 6174 6520 6469 7374   # allocate dist
-00019430: 616e 6365 206d 6174 7269 780a 2020 2020  ance matrix.    
-00019440: 6420 3d20 6e70 2e7a 6572 6f73 285b 6e53  d = np.zeros([nS
-00019450: 616d 706c 652c 206e 4c61 675d 290a 0a20  ample, nLag]).. 
-00019460: 2020 2023 2053 6574 7570 2069 6e64 6963     # Setup indic
-00019470: 6573 2062 6173 6564 206f 6e20 666f 7277  es based on forw
-00019480: 6172 6420 6f72 2062 6163 6b77 6172 6420  ard or backward 
-00019490: 6163 6375 6d75 6c61 7469 6f6e 2064 6972  accumulation dir
-000194a0: 6563 7469 6f6e 0a20 2020 2069 6620 6469  ection.    if di
-000194b0: 7220 3e20 303a 2020 2320 464f 5257 4152  r > 0:  # FORWAR
-000194c0: 440a 2020 2020 2020 2020 6942 6567 696e  D.        iBegin
-000194d0: 2c20 6945 6e64 2c20 6949 6e63 203d 2030  , iEnd, iInc = 0
-000194e0: 2c20 6e53 616d 706c 6520 2d20 312c 2031  , nSample - 1, 1
-000194f0: 0a20 2020 2065 6c73 653a 2020 2320 4241  .    else:  # BA
-00019500: 434b 5741 5244 0a20 2020 2020 2020 2069  CKWARD.        i
-00019510: 4265 6769 6e2c 2069 456e 642c 2069 496e  Begin, iEnd, iIn
-00019520: 6320 3d20 6e53 616d 706c 6520 2d20 312c  c = nSample - 1,
-00019530: 2030 2c20 2d31 0a0a 2020 2020 2320 4c6f   0, -1..    # Lo
-00019540: 6f70 2074 6872 6f75 6768 2061 6c6c 2074  op through all t
-00019550: 696d 6573 2069 6920 696e 2066 6f72 7761  imes ii in forwa
-00019560: 7264 206f 7220 6261 636b 7761 7264 2064  rd or backward d
-00019570: 6972 6563 7469 6f6e 0a20 2020 2066 6f72  irection.    for
-00019580: 2069 6920 696e 2072 616e 6765 2869 4265   ii in range(iBe
-00019590: 6769 6e2c 2069 456e 6420 2b20 6949 6e63  gin, iEnd + iInc
-000195a0: 2c20 6949 6e63 293a 0a20 2020 2020 2020  , iInc):.       
-000195b0: 2023 206d 696e 2f6d 6178 2074 6f20 6163   # min/max to ac
-000195c0: 636f 756e 7420 666f 7220 7468 6520 6564  count for the ed
-000195d0: 6765 732f 626f 756e 6461 7269 6573 0a20  ges/boundaries. 
-000195e0: 2020 2020 2020 206a 6920 3d20 6d61 7828         ji = max(
-000195f0: 5b30 2c20 6d69 6e28 5b6e 5361 6d70 6c65  [0, min([nSample
-00019600: 202d 2031 2c20 6969 202d 2069 496e 635d   - 1, ii - iInc]
-00019610: 295d 290a 2020 2020 2020 2020 6a62 203d  )]).        jb =
-00019620: 206d 6178 285b 302c 206d 696e 285b 6e53   max([0, min([nS
-00019630: 616d 706c 6520 2d20 312c 2069 6920 2d20  ample - 1, ii - 
-00019640: 6949 6e63 202a 2062 5d29 5d29 0a0a 2020  iInc * b])])..  
-00019650: 2020 2020 2020 2320 6c6f 6f70 2074 6872        # loop thr
-00019660: 6f75 6768 2061 6c6c 206c 6167 0a20 2020  ough all lag.   
-00019670: 2020 2020 2066 6f72 206c 6c20 696e 2072       for ll in r
-00019680: 616e 6765 286e 4c61 6729 3a0a 2020 2020  ange(nLag):.    
-00019690: 2020 2020 2020 2020 2320 6368 6563 6b20          # check 
-000196a0: 6c69 6d69 7473 206f 6e20 6c61 6720 696e  limits on lag in
-000196b0: 6469 6365 730a 2020 2020 2020 2020 2020  dices.          
-000196c0: 2020 6c4d 696e 7573 3120 3d20 6c6c 202d    lMinus1 = ll -
-000196d0: 2031 0a0a 2020 2020 2020 2020 2020 2020   1..            
-000196e0: 2320 6368 6563 6b20 6c61 6720 696e 6465  # check lag inde
-000196f0: 7820 6973 2067 7265 6174 6572 2074 6861  x is greater tha
-00019700: 6e20 300a 2020 2020 2020 2020 2020 2020  n 0.            
-00019710: 6966 206c 4d69 6e75 7331 203c 2030 3a0a  if lMinus1 < 0:.
-00019720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019730: 6c4d 696e 7573 3120 3d20 3020 2023 206d  lMinus1 = 0  # m
-00019740: 616b 6520 6c61 6720 3d20 6669 7273 7420  ake lag = first 
-00019750: 6c61 670a 0a20 2020 2020 2020 2020 2020  lag..           
-00019760: 206c 506c 7573 3120 3d20 6c6c 202b 2031   lPlus1 = ll + 1
-00019770: 2020 2320 6c61 6720 6174 206c 2b31 0a0a    # lag at l+1..
-00019780: 2020 2020 2020 2020 2020 2020 2320 6368              # ch
-00019790: 6563 6b20 6c61 6720 696e 6465 7820 6c65  eck lag index le
-000197a0: 7373 2074 6861 6e20 6d61 7820 6c61 670a  ss than max lag.
-000197b0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-000197c0: 506c 7573 3120 3e20 6e4c 6167 202d 2031  Plus1 > nLag - 1
-000197d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000197e0: 2020 6c50 6c75 7331 203d 206e 4c61 6720    lPlus1 = nLag 
-000197f0: 2d20 310a 0a20 2020 2020 2020 2020 2020  - 1..           
-00019800: 2023 2067 6574 2064 6973 7461 6e63 6520   # get distance 
-00019810: 6174 206c 6167 7320 286c 6c2d 312c 206c  at lags (ll-1, l
-00019820: 6c2c 206c 6c2b 3129 0a20 2020 2020 2020  l, ll+1).       
-00019830: 2020 2020 2064 6973 744c 6d69 6e75 7331       distLminus1
-00019840: 203d 2064 5b6a 622c 206c 4d69 6e75 7331   = d[jb, lMinus1
-00019850: 5d20 2023 206d 696e 7573 3a20 2064 5b69  ]  # minus:  d[i
-00019860: 2d62 2c20 6a2d 315d 0a20 2020 2020 2020  -b, j-1].       
-00019870: 2020 2020 2064 6973 744c 203d 2064 5b6a       distL = d[j
-00019880: 692c 206c 6c5d 2020 2320 6163 7475 616c  i, ll]  # actual
-00019890: 2064 5b69 2d31 2c20 6a5d 0a20 2020 2020   d[i-1, j].     
-000198a0: 2020 2020 2020 2064 6973 744c 706c 7573         distLplus
-000198b0: 3120 3d20 645b 6a62 2c20 6c50 6c75 7331  1 = d[jb, lPlus1
-000198c0: 5d20 2023 2070 6c75 7320 645b 692d 622c  ]  # plus d[i-b,
-000198d0: 206a 2b31 5d0a 0a20 2020 2020 2020 2020   j+1]..         
-000198e0: 2020 2069 6620 6a69 2021 3d20 6a62 3a20     if ji != jb: 
-000198f0: 2023 2065 7175 6174 696f 6e20 3130 2069   # equation 10 i
-00019900: 6e20 4861 6c65 2c20 3230 3133 0a20 2020  n Hale, 2013.   
-00019910: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00019920: 206b 6220 696e 2072 616e 6765 286a 692c   kb in range(ji,
-00019930: 206a 6220 2b20 6949 6e63 202d 2031 2c20   jb + iInc - 1, 
-00019940: 2d69 496e 6329 3a0a 2020 2020 2020 2020  -iInc):.        
-00019950: 2020 2020 2020 2020 2020 2020 6469 7374              dist
-00019960: 4c6d 696e 7573 3120 3d20 6469 7374 4c6d  Lminus1 = distLm
-00019970: 696e 7573 3120 2b20 6572 725b 6b62 2c20  inus1 + err[kb, 
-00019980: 6c4d 696e 7573 315d 0a20 2020 2020 2020  lMinus1].       
-00019990: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-000199a0: 744c 706c 7573 3120 3d20 6469 7374 4c70  tLplus1 = distLp
-000199b0: 6c75 7331 202b 2065 7272 5b6b 622c 206c  lus1 + err[kb, l
-000199c0: 506c 7573 315d 0a0a 2020 2020 2020 2020  Plus1]..        
-000199d0: 2020 2020 2320 6571 7561 7469 6f6e 2036      # equation 6
-000199e0: 2028 6966 2062 3d31 2920 6f72 2031 3020   (if b=1) or 10 
-000199f0: 2869 6620 623e 3129 2069 6e20 4861 6c65  (if b>1) in Hale
-00019a00: 2028 3230 3133 2920 6166 7465 7220 7472   (2013) after tr
-00019a10: 6561 7469 6e67 2062 6f75 6e64 6172 6965  eating boundarie
-00019a20: 730a 2020 2020 2020 2020 2020 2020 645b  s.            d[
-00019a30: 6969 2c20 6c6c 5d20 3d20 6572 725b 6969  ii, ll] = err[ii
-00019a40: 2c20 6c6c 5d20 2b20 6d69 6e28 5b64 6973  , ll] + min([dis
-00019a50: 744c 6d69 6e75 7331 2c20 6469 7374 4c2c  tLminus1, distL,
-00019a60: 2064 6973 744c 706c 7573 315d 290a 0a20   distLplus1]).. 
-00019a70: 2020 2072 6574 7572 6e20 640a 0a0a 6465     return d...de
-00019a80: 6620 6261 636b 7472 6163 6b44 6973 7461  f backtrackDista
-00019a90: 6e63 6546 756e 6374 696f 6e28 6469 722c  nceFunction(dir,
-00019aa0: 2064 2c20 6572 722c 206c 6d69 6e2c 2062   d, err, lmin, b
-00019ab0: 293a 0a20 2020 2022 2222 0a20 2020 2054  ):.    """.    T
-00019ac0: 6865 2066 756e 6374 696f 6e20 6973 2065  he function is e
-00019ad0: 7175 6174 696f 6e20 3220 696e 2048 616c  quation 2 in Hal
-00019ae0: 652c 2032 3031 332e 0a0a 2020 2020 5061  e, 2013...    Pa
-00019af0: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-00019b00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
-00019b10: 6469 723a 2073 6964 6520 746f 2073 7461  dir: side to sta
-00019b20: 7274 206d 696e 696d 697a 6174 696f 6e20  rt minimization 
-00019b30: 2820 6469 7220 3e20 3020 3d20 6672 6f6e  ( dir > 0 = fron
-00019b40: 742c 2064 6972 203c 3d20 3020 3d20 2062  t, dir <= 0 =  b
-00019b50: 6163 6b29 0a20 2020 2064 203a 2074 6865  ack).    d : the
-00019b60: 2032 4420 6469 7374 616e 6365 2066 756e   2D distance fun
-00019b70: 6374 696f 6e3b 2073 697a 6520 3d20 286e  ction; size = (n
-00019b80: 7361 6d70 2c32 2a6c 6167 2b31 290a 2020  samp,2*lag+1).  
-00019b90: 2020 6572 723a 2074 6865 2032 4420 6572    err: the 2D er
-00019ba0: 726f 7220 6675 6e63 7469 6f6e 3b20 7369  ror function; si
-00019bb0: 7a65 203d 2028 6e73 616d 702c 322a 6c61  ze = (nsamp,2*la
-00019bc0: 672b 3129 0a20 2020 206c 6d69 6e3a 206d  g+1).    lmin: m
-00019bd0: 696e 696d 756d 206c 6167 2074 6f20 7365  inimum lag to se
-00019be0: 6172 6368 206f 7665 720a 2020 2020 6220  arch over.    b 
-00019bf0: 3a20 7374 7261 696e 206c 696d 6974 2028  : strain limit (
-00019c00: 696e 7465 6765 7220 7661 6c75 6520 3e3d  integer value >=
-00019c10: 2031 290a 0a20 2020 2052 4554 5552 4e53   1)..    RETURNS
-00019c20: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  :.    ----------
-00019c30: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2073 7462  --------.    stb
-00019c40: 6172 3a20 7665 6374 6f72 206f 6620 696e  ar: vector of in
-00019c50: 7465 6765 7220 7368 6966 7473 2073 7562  teger shifts sub
-00019c60: 6a65 6374 2074 6f20 7c75 2869 292d 7528  ject to |u(i)-u(
-00019c70: 692d 3129 7c20 3c3d 2031 2f62 0a0a 2020  i-1)| <= 1/b..  
-00019c80: 2020 4f72 6967 696e 616c 2062 7920 4469    Original by Di
-00019c90: 2059 616e 670a 2020 2020 4c61 7374 206d   Yang.    Last m
-00019ca0: 6f64 6966 6965 6420 6279 2044 796c 616e  odified by Dylan
-00019cb0: 204d 696b 6573 656c 6c20 2831 3920 4465   Mikesell (19 De
-00019cc0: 632e 2032 3031 3429 0a0a 2020 2020 5472  c. 2014)..    Tr
-00019cd0: 616e 736c 6174 6564 2074 6f20 7079 7468  anslated to pyth
-00019ce0: 6f6e 2062 7920 5469 6d20 436c 656d 656e  on by Tim Clemen
-00019cf0: 7473 2028 3137 2041 7567 2e20 3230 3138  ts (17 Aug. 2018
-00019d00: 290a 0a20 2020 2022 2222 0a0a 2020 2020  )..    """..    
-00019d10: 6e53 616d 706c 652c 206e 4c61 6720 3d20  nSample, nLag = 
-00019d20: 642e 7368 6170 650a 2020 2020 7374 6261  d.shape.    stba
-00019d30: 7220 3d20 6e70 2e7a 6572 6f73 286e 5361  r = np.zeros(nSa
-00019d40: 6d70 6c65 290a 0a20 2020 2023 2053 6574  mple)..    # Set
-00019d50: 7570 2069 6e64 6963 6573 2062 6173 6564  up indices based
-00019d60: 206f 6e20 666f 7277 6172 6420 6f72 2062   on forward or b
-00019d70: 6163 6b77 6172 6420 6163 6375 6d75 6c61  ackward accumula
-00019d80: 7469 6f6e 2064 6972 6563 7469 6f6e 0a20  tion direction. 
-00019d90: 2020 2069 6620 6469 7220 3e20 303a 2020     if dir > 0:  
-00019da0: 2320 464f 5257 4152 440a 2020 2020 2020  # FORWARD.      
-00019db0: 2020 6942 6567 696e 2c20 6945 6e64 2c20    iBegin, iEnd, 
-00019dc0: 6949 6e63 203d 2030 2c20 6e53 616d 706c  iInc = 0, nSampl
-00019dd0: 6520 2d20 312c 2031 0a20 2020 2065 6c73  e - 1, 1.    els
-00019de0: 653a 2020 2320 4241 434b 5741 5244 0a20  e:  # BACKWARD. 
-00019df0: 2020 2020 2020 2069 4265 6769 6e2c 2069         iBegin, i
-00019e00: 456e 642c 2069 496e 6320 3d20 6e53 616d  End, iInc = nSam
-00019e10: 706c 6520 2d20 312c 2030 2c20 2d31 0a0a  ple - 1, 0, -1..
-00019e20: 2020 2020 2320 7374 6172 7420 6672 6f6d      # start from
-00019e30: 2074 6865 2065 6e64 2028 6672 6f6e 7420   the end (front 
-00019e40: 6f72 2062 6163 6b29 0a20 2020 206c 6c20  or back).    ll 
-00019e50: 3d20 6e70 2e61 7267 6d69 6e28 645b 6942  = np.argmin(d[iB
-00019e60: 6567 696e 2c20 3a5d 2920 2023 2066 696e  egin, :])  # fin
-00019e70: 6420 6d69 6e69 6d75 6d20 6163 6375 6d75  d minimum accumu
-00019e80: 6c61 7465 6420 6469 7374 616e 6365 2061  lated distance a
-00019e90: 7420 6672 6f6e 7420 6f72 2062 6163 6b20  t front or back 
-00019ea0: 6465 7065 6e64 696e 6720 6f6e 2027 6469  depending on 'di
-00019eb0: 7227 0a20 2020 2073 7462 6172 5b69 4265  r'.    stbar[iBe
-00019ec0: 6769 6e5d 203d 206c 6c20 2b20 6c6d 696e  gin] = ll + lmin
-00019ed0: 2020 2320 6162 736f 6c75 7465 2076 616c    # absolute val
-00019ee0: 7565 206f 6620 696e 7465 6765 7220 7368  ue of integer sh
-00019ef0: 6966 740a 0a20 2020 2023 206d 6f76 6520  ift..    # move 
-00019f00: 7468 726f 7567 6820 616c 6c20 7469 6d65  through all time
-00019f10: 2073 616d 706c 6573 2069 6e20 666f 7277   samples in forw
-00019f20: 6172 6420 6f72 2062 6163 6b77 6172 6420  ard or backward 
-00019f30: 6469 7265 6374 696f 6e0a 2020 2020 6969  direction.    ii
-00019f40: 203d 2069 4265 6769 6e0a 0a20 2020 2077   = iBegin..    w
-00019f50: 6869 6c65 2069 6920 213d 2069 456e 643a  hile ii != iEnd:
-00019f60: 0a20 2020 2020 2020 2023 206d 696e 2f6d  .        # min/m
-00019f70: 6178 2066 6f72 2065 6467 6573 2f62 6f75  ax for edges/bou
-00019f80: 6e64 6172 6965 730a 2020 2020 2020 2020  ndaries.        
-00019f90: 6a69 203d 206e 702e 6d61 7828 5b30 2c20  ji = np.max([0, 
-00019fa0: 6e70 2e6d 696e 285b 6e53 616d 706c 6520  np.min([nSample 
-00019fb0: 2d20 312c 2069 6920 2b20 6949 6e63 5d29  - 1, ii + iInc])
-00019fc0: 5d29 0a20 2020 2020 2020 206a 6220 3d20  ]).        jb = 
-00019fd0: 6e70 2e6d 6178 285b 302c 206e 702e 6d69  np.max([0, np.mi
-00019fe0: 6e28 5b6e 5361 6d70 6c65 202d 2031 2c20  n([nSample - 1, 
-00019ff0: 6969 202b 2069 496e 6320 2a20 625d 295d  ii + iInc * b])]
-0001a000: 290a 0a20 2020 2020 2020 2023 2063 6865  )..        # che
-0001a010: 636b 206c 696d 6974 7320 6f6e 206c 6167  ck limits on lag
-0001a020: 2069 6e64 6963 6573 0a20 2020 2020 2020   indices.       
-0001a030: 206c 4d69 6e75 7331 203d 206c 6c20 2d20   lMinus1 = ll - 
-0001a040: 310a 0a20 2020 2020 2020 2069 6620 6c4d  1..        if lM
-0001a050: 696e 7573 3120 3c20 303a 2020 2320 6368  inus1 < 0:  # ch
-0001a060: 6563 6b20 6c61 6720 696e 6465 7820 6973  eck lag index is
-0001a070: 2067 7265 6174 6572 2074 6861 6e20 310a   greater than 1.
-0001a080: 2020 2020 2020 2020 2020 2020 6c4d 696e              lMin
-0001a090: 7573 3120 3d20 3020 2023 206d 616b 6520  us1 = 0  # make 
-0001a0a0: 6c61 6720 3d20 6669 7273 7420 6c61 670a  lag = first lag.
-0001a0b0: 0a20 2020 2020 2020 206c 506c 7573 3120  .        lPlus1 
-0001a0c0: 3d20 6c6c 202b 2031 0a0a 2020 2020 2020  = ll + 1..      
-0001a0d0: 2020 6966 206c 506c 7573 3120 3e20 6e4c    if lPlus1 > nL
-0001a0e0: 6167 202d 2031 3a20 2023 2063 6865 636b  ag - 1:  # check
-0001a0f0: 206c 6167 2069 6e64 6578 206c 6573 7320   lag index less 
-0001a100: 7468 616e 206d 6178 206c 6167 0a20 2020  than max lag.   
-0001a110: 2020 2020 2020 2020 206c 506c 7573 3120           lPlus1 
-0001a120: 3d20 6e4c 6167 202d 2031 0a0a 2020 2020  = nLag - 1..    
-0001a130: 2020 2020 2320 6765 7420 6469 7374 616e      # get distan
-0001a140: 6365 2061 7420 6c61 6773 2028 6c6c 2d31  ce at lags (ll-1
-0001a150: 2c20 6c6c 2c20 6c6c 2b31 290a 2020 2020  , ll, ll+1).    
-0001a160: 2020 2020 6469 7374 4c6d 696e 7573 3120      distLminus1 
-0001a170: 3d20 645b 6a62 2c20 6c4d 696e 7573 315d  = d[jb, lMinus1]
-0001a180: 2020 2320 6d69 6e75 733a 2020 645b 692d    # minus:  d[i-
-0001a190: 622c 206a 2d31 5d0a 2020 2020 2020 2020  b, j-1].        
-0001a1a0: 6469 7374 4c20 3d20 645b 6a69 2c20 6c6c  distL = d[ji, ll
-0001a1b0: 5d20 2023 2061 6374 7561 6c20 645b 692d  ]  # actual d[i-
-0001a1c0: 312c 206a 5d0a 2020 2020 2020 2020 6469  1, j].        di
-0001a1d0: 7374 4c70 6c75 7331 203d 2064 5b6a 622c  stLplus1 = d[jb,
-0001a1e0: 206c 506c 7573 315d 2020 2320 706c 7573   lPlus1]  # plus
-0001a1f0: 2064 5b69 2d62 2c20 6a2b 315d 0a0a 2020   d[i-b, j+1]..  
-0001a200: 2020 2020 2020 2320 6571 7561 7469 6f6e        # equation
-0001a210: 2031 3020 696e 2048 616c 6520 2832 3031   10 in Hale (201
-0001a220: 3329 0a20 2020 2020 2020 2023 2073 756d  3).        # sum
-0001a230: 2065 7272 6f72 7320 6f76 6572 2069 2d31   errors over i-1
-0001a240: 3a69 2d62 2b31 0a20 2020 2020 2020 2069  :i-b+1.        i
-0001a250: 6620 6a69 2021 3d20 6a62 3a0a 2020 2020  f ji != jb:.    
-0001a260: 2020 2020 2020 2020 666f 7220 6b62 2069          for kb i
-0001a270: 6e20 7261 6e67 6528 6a69 2c20 6a62 202d  n range(ji, jb -
-0001a280: 2069 496e 6320 2d20 312c 2069 496e 6329   iInc - 1, iInc)
-0001a290: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001a2a0: 2020 6469 7374 4c6d 696e 7573 3120 3d20    distLminus1 = 
-0001a2b0: 6469 7374 4c6d 696e 7573 3120 2b20 6572  distLminus1 + er
-0001a2c0: 725b 6b62 2c20 6c4d 696e 7573 315d 0a20  r[kb, lMinus1]. 
-0001a2d0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0001a2e0: 6973 744c 706c 7573 3120 3d20 6469 7374  istLplus1 = dist
-0001a2f0: 4c70 6c75 7331 202b 2065 7272 5b6b 622c  Lplus1 + err[kb,
-0001a300: 206c 506c 7573 315d 0a0a 2020 2020 2020   lPlus1]..      
-0001a310: 2020 2320 7570 6461 7465 206d 696e 696d    # update minim
-0001a320: 756d 2064 6973 7461 6e63 6520 746f 2070  um distance to p
-0001a330: 7265 7669 6f75 7320 7361 6d70 6c65 0a20  revious sample. 
-0001a340: 2020 2020 2020 2064 6c20 3d20 6e70 2e6d         dl = np.m
-0001a350: 696e 285b 6469 7374 4c6d 696e 7573 312c  in([distLminus1,
-0001a360: 2064 6973 744c 2c20 6469 7374 4c70 6c75   distL, distLplu
-0001a370: 7331 5d29 0a0a 2020 2020 2020 2020 6966  s1])..        if
-0001a380: 2064 6c20 213d 2064 6973 744c 3a20 2023   dl != distL:  #
-0001a390: 2074 6865 6e20 6c6c 207e 3d20 6c6c 2061   then ll ~= ll a
-0001a3a0: 6e64 2077 6520 6368 6563 6b20 666f 7277  nd we check forw
-0001a3b0: 6172 6420 616e 6420 6261 636b 7761 7264  ard and backward
-0001a3c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0001a3d0: 646c 203d 3d20 6469 7374 4c6d 696e 7573  dl == distLminus
-0001a3e0: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
-0001a3f0: 2020 206c 6c20 3d20 6c4d 696e 7573 310a     ll = lMinus1.
-0001a400: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0001a410: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001a420: 2020 6c6c 203d 206c 506c 7573 310a 0a20    ll = lPlus1.. 
-0001a430: 2020 2020 2020 2023 2061 7373 756d 6520         # assume 
-0001a440: 6969 203d 2069 6920 2d20 310a 2020 2020  ii = ii - 1.    
-0001a450: 2020 2020 6969 202b 3d20 6949 6e63 0a0a      ii += iInc..
-0001a460: 2020 2020 2020 2020 2320 6162 736f 6c75          # absolu
-0001a470: 7465 2069 6e74 6567 6572 206f 6620 6c61  te integer of la
-0001a480: 670a 2020 2020 2020 2020 7374 6261 725b  g.        stbar[
-0001a490: 6969 5d20 3d20 6c6c 202b 206c 6d69 6e0a  ii] = ll + lmin.
-0001a4a0: 0a20 2020 2020 2020 2023 206e 6f77 206d  .        # now m
-0001a4b0: 6f76 6520 746f 2063 6f72 7265 6374 2074  ove to correct t
-0001a4c0: 696d 6520 696e 6465 782c 2069 6620 736d  ime index, if sm
-0001a4d0: 6f6f 7468 696e 6720 6469 6666 6572 656e  oothing differen
-0001a4e0: 6365 206f 7665 7220 6d61 6e79 0a20 2020  ce over many.   
-0001a4f0: 2020 2020 2023 2074 696d 6520 7361 6d70       # time samp
-0001a500: 6c65 7320 7573 696e 6720 2762 270a 2020  les using 'b'.  
-0001a510: 2020 2020 2020 6966 2028 6c6c 203d 3d20        if (ll == 
-0001a520: 6c4d 696e 7573 3129 207c 2028 6c6c 203d  lMinus1) | (ll =
-0001a530: 3d20 6c50 6c75 7331 293a 2020 2320 6368  = lPlus1):  # ch
-0001a540: 6563 6b20 6564 6765 7320 746f 2073 6565  eck edges to see
-0001a550: 2061 626f 7574 2062 2076 616c 7565 730a   about b values.
-0001a560: 2020 2020 2020 2020 2020 2020 6966 206a              if j
-0001a570: 6920 213d 206a 623a 2020 2320 6966 2062  i != jb:  # if b
-0001a580: 3e31 2074 6865 6e20 6e65 6564 2074 6f20  >1 then need to 
-0001a590: 6d6f 7665 206d 6f72 6520 7374 6570 730a  move more steps.
-0001a5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a5b0: 666f 7220 6b62 2069 6e20 7261 6e67 6528  for kb in range(
-0001a5c0: 6a69 2c20 6a62 202d 2069 496e 6320 2d20  ji, jb - iInc - 
-0001a5d0: 312c 2069 496e 6329 3a0a 2020 2020 2020  1, iInc):.      
-0001a5e0: 2020 2020 2020 2020 2020 2020 2020 6969                ii
-0001a5f0: 203d 2069 6920 2b20 6949 6e63 2020 2320   = ii + iInc  # 
-0001a600: 6d6f 7665 2066 726f 6d20 692d 313a 692d  move from i-1:i-
-0001a610: 622d 310a 2020 2020 2020 2020 2020 2020  b-1.            
-0001a620: 2020 2020 2020 2020 7374 6261 725b 6969          stbar[ii
-0001a630: 5d20 3d20 6c6c 202b 206c 6d69 6e20 2023  ] = ll + lmin  #
-0001a640: 2063 6f6e 7374 616e 7420 6c61 6720 6f76   constant lag ov
-0001a650: 6572 2074 6861 7420 7469 6d65 0a0a 2020  er that time..  
-0001a660: 2020 7265 7475 726e 2073 7462 6172 0a0a    return stbar..
-0001a670: 0a64 6566 2077 6374 5f6d 6f64 6966 6965  .def wct_modifie
-0001a680: 6428 0a20 2020 2079 312c 2079 322c 2064  d(.    y1, y2, d
-0001a690: 742c 2064 6a3d 3120 2f20 3132 2c20 7330  t, dj=1 / 12, s0
-0001a6a0: 3d2d 312c 204a 3d2d 312c 2073 6967 3d54  =-1, J=-1, sig=T
-0001a6b0: 7275 652c 2073 6967 6e69 6669 6361 6e63  rue, significanc
-0001a6c0: 655f 6c65 7665 6c3d 302e 3935 2c20 7761  e_level=0.95, wa
-0001a6d0: 7665 6c65 743d 226d 6f72 6c65 7422 2c20  velet="morlet", 
-0001a6e0: 6e6f 726d 616c 697a 653d 5472 7565 2c20  normalize=True, 
-0001a6f0: 2a2a 6b77 6172 6773 0a29 3a0a 2020 2020  **kwargs.):.    
-0001a700: 2222 220a 2020 2020 2020 2020 5761 7665  """.        Wave
-0001a710: 6c65 7420 636f 6865 7265 6e63 6520 7472  let coherence tr
-0001a720: 616e 7366 6f72 6d20 2857 4354 292e 0a20  ansform (WCT).. 
-0001a730: 2020 20e2 808b 0a20 2020 2020 2020 2054     ....        T
-0001a740: 6865 2057 4354 2066 696e 6473 2072 6567  he WCT finds reg
-0001a750: 696f 6e73 2069 6e20 7469 6d65 2066 7265  ions in time fre
-0001a760: 7175 656e 6379 2073 7061 6365 2077 6865  quency space whe
-0001a770: 7265 2074 6865 2074 776f 2074 696d 650a  re the two time.
-0001a780: 2020 2020 2020 2020 7365 7269 6573 2063          series c
-0001a790: 6f2d 7661 7279 2c20 6275 7420 646f 206e  o-vary, but do n
-0001a7a0: 6f74 206e 6563 6573 7361 7269 6c79 2068  ot necessarily h
-0001a7b0: 6176 6520 6869 6768 2070 6f77 6572 2e0a  ave high power..
-0001a7c0: 2020 2020 e280 8b0a 2020 2020 2020 2020      ....        
-0001a7d0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-0001a7e0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-0001a7f0: 2020 2020 2020 7931 2c20 7932 203a 206e        y1, y2 : n
-0001a800: 756d 7079 2e6e 6461 7272 6179 2c20 6c69  umpy.ndarray, li
-0001a810: 7374 0a20 2020 2020 2020 2020 2020 2049  st.            I
-0001a820: 6e70 7574 2073 6967 6e61 6c73 2e0a 2020  nput signals..  
-0001a830: 2020 2020 2020 6474 203a 2066 6c6f 6174        dt : float
-0001a840: 0a20 2020 2020 2020 2020 2020 2053 616d  .            Sam
-0001a850: 706c 6520 7370 6163 696e 672e 0a20 2020  ple spacing..   
-0001a860: 2020 2020 2064 6a20 3a20 666c 6f61 742c       dj : float,
-0001a870: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-0001a880: 2020 2020 2020 5370 6163 696e 6720 6265        Spacing be
-0001a890: 7477 6565 6e20 6469 7363 7265 7465 2073  tween discrete s
-0001a8a0: 6361 6c65 732e 2044 6566 6175 6c74 2076  cales. Default v
-0001a8b0: 616c 7565 2069 7320 312f 3132 2e0a 2020  alue is 1/12..  
-0001a8c0: 2020 2020 2020 2020 2020 536d 616c 6c65            Smalle
-0001a8d0: 7220 7661 6c75 6573 2077 696c 6c20 7265  r values will re
-0001a8e0: 7375 6c74 2069 6e20 6265 7474 6572 2073  sult in better s
-0001a8f0: 6361 6c65 2072 6573 6f6c 7574 696f 6e2c  cale resolution,
-0001a900: 2062 7574 0a20 2020 2020 2020 2020 2020   but.           
-0001a910: 2073 6c6f 7765 7220 6361 6c63 756c 6174   slower calculat
-0001a920: 696f 6e20 616e 6420 706c 6f74 2e0a 2020  ion and plot..  
-0001a930: 2020 2020 2020 7330 203a 2066 6c6f 6174        s0 : float
-0001a940: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-0001a950: 2020 2020 2020 2053 6d61 6c6c 6573 7420         Smallest 
-0001a960: 7363 616c 6520 6f66 2074 6865 2077 6176  scale of the wav
-0001a970: 656c 6574 2e20 4465 6661 756c 7420 7661  elet. Default va
-0001a980: 6c75 6520 6973 2032 2a64 742e 0a20 2020  lue is 2*dt..   
-0001a990: 2020 2020 204a 203a 2066 6c6f 6174 2c20       J : float, 
-0001a9a0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-0001a9b0: 2020 2020 204e 756d 6265 7220 6f66 2073       Number of s
-0001a9c0: 6361 6c65 7320 6c65 7373 206f 6e65 2e20  cales less one. 
-0001a9d0: 5363 616c 6573 2072 616e 6765 2066 726f  Scales range fro
-0001a9e0: 6d20 7330 2075 7020 746f 0a20 2020 2020  m s0 up to.     
-0001a9f0: 2020 2020 2020 2073 3020 2a20 322a 2a28         s0 * 2**(
-0001aa00: 4a20 2a20 646a 292c 2077 6869 6368 2067  J * dj), which g
-0001aa10: 6976 6573 2061 2074 6f74 616c 206f 6620  ives a total of 
-0001aa20: 284a 202b 2031 2920 7363 616c 6573 2e0a  (J + 1) scales..
-0001aa30: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
-0001aa40: 756c 7420 6973 204a 203d 2028 6c6f 6732  ult is J = (log2
-0001aa50: 284e 2a64 742f 736f 2929 2f64 6a2e 0a20  (N*dt/so))/dj.. 
-0001aa60: 2020 2020 2020 2073 6967 6e69 6669 6361         significa
-0001aa70: 6e63 655f 6c65 7665 6c20 2866 6c6f 6174  nce_level (float
-0001aa80: 2c20 6f70 7469 6f6e 616c 2920 3a0a 2020  , optional) :.  
-0001aa90: 2020 2020 2020 2020 2020 5369 676e 6966            Signif
-0001aaa0: 6963 616e 6365 206c 6576 656c 2074 6f20  icance level to 
-0001aab0: 7573 652e 2044 6566 6175 6c74 2069 7320  use. Default is 
-0001aac0: 302e 3935 2e0a 2020 2020 2020 2020 6e6f  0.95..        no
-0001aad0: 726d 616c 697a 6520 2862 6f6f 6c65 616e  rmalize (boolean
-0001aae0: 2c20 6f70 7469 6f6e 616c 2920 3a0a 2020  , optional) :.  
-0001aaf0: 2020 2020 2020 2020 2020 4966 2073 6574            If set
-0001ab00: 2074 6f20 7472 7565 2c20 6e6f 726d 616c   to true, normal
-0001ab10: 697a 6573 2043 5754 2062 7920 7468 6520  izes CWT by the 
-0001ab20: 7374 616e 6461 7264 2064 6576 6961 7469  standard deviati
-0001ab30: 6f6e 206f 660a 2020 2020 2020 2020 2020  on of.          
-0001ab40: 2020 7468 6520 7369 676e 616c 732e 0a20    the signals.. 
-0001ab50: 2020 20e2 808b 0a20 2020 2020 2020 2052     ....        R
-0001ab60: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
-0001ab70: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2054  ------.        T
-0001ab80: 4f44 4f3a 2053 6f6d 6574 6869 6e67 2054  ODO: Something T
-0001ab90: 4241 2061 6e64 2054 4243 0a20 2020 20e2  BA and TBC.    .
-0001aba0: 808b 0a20 2020 2020 2020 2053 6565 2061  ...        See a
-0001abb0: 6c73 6f0a 2020 2020 2020 2020 2d2d 2d2d  lso.        ----
-0001abc0: 2d2d 2d2d 0a20 2020 2020 2020 2063 7774  ----.        cwt
-0001abd0: 2c20 7877 740a 2020 2020 e280 8b0a 2020  , xwt.    ....  
-0001abe0: 2020 2222 220a 0a20 2020 2077 6176 656c    """..    wavel
-0001abf0: 6574 203d 2070 7963 7774 2e77 6176 656c  et = pycwt.wavel
-0001ac00: 6574 2e5f 6368 6563 6b5f 7061 7261 6d65  et._check_parame
-0001ac10: 7465 725f 7761 7665 6c65 7428 7761 7665  ter_wavelet(wave
-0001ac20: 6c65 7429 0a20 2020 2023 2043 6865 636b  let).    # Check
-0001ac30: 696e 6720 736f 6d65 2069 6e70 7574 2070  ing some input p
-0001ac40: 6172 616d 6574 6572 730a 2020 2020 6966  arameters.    if
-0001ac50: 2073 3020 3d3d 202d 313a 0a20 2020 2020   s0 == -1:.     
-0001ac60: 2020 2023 204e 756d 6265 7220 6f66 2073     # Number of s
-0001ac70: 6361 6c65 730a 2020 2020 2020 2020 7330  cales.        s0
-0001ac80: 203d 2032 202a 2064 7420 2f20 7761 7665   = 2 * dt / wave
-0001ac90: 6c65 742e 666c 616d 6264 6128 290a 2020  let.flambda().  
-0001aca0: 2020 6966 204a 203d 3d20 2d31 3a0a 2020    if J == -1:.  
-0001acb0: 2020 2020 2020 2320 4e75 6d62 6572 206f        # Number o
-0001acc0: 6620 7363 616c 6573 0a20 2020 2020 2020  f scales.       
-0001acd0: 204a 203d 206e 702e 696e 7428 6e70 2e72   J = np.int(np.r
-0001ace0: 6f75 6e64 286e 702e 6c6f 6732 2879 312e  ound(np.log2(y1.
-0001acf0: 7369 7a65 202a 2064 7420 2f20 7330 2920  size * dt / s0) 
-0001ad00: 2f20 646a 2929 0a0a 2020 2020 2320 4d61  / dj))..    # Ma
-0001ad10: 6b65 7320 7375 7265 2069 6e70 7574 2073  kes sure input s
-0001ad20: 6967 6e61 6c73 2061 7265 206e 756d 7079  ignals are numpy
-0001ad30: 2061 7272 6179 732e 0a20 2020 2079 3120   arrays..    y1 
-0001ad40: 3d20 6e70 2e61 7361 7272 6179 2879 3129  = np.asarray(y1)
-0001ad50: 0a20 2020 2079 3220 3d20 6e70 2e61 7361  .    y2 = np.asa
-0001ad60: 7272 6179 2879 3229 0a20 2020 2023 2043  rray(y2).    # C
-0001ad70: 616c 6375 6c61 7465 7320 7468 6520 7374  alculates the st
-0001ad80: 616e 6461 7264 2064 6576 6961 7469 6f6e  andard deviation
-0001ad90: 206f 6620 626f 7468 2069 6e70 7574 2073   of both input s
-0001ada0: 6967 6e61 6c73 2e0a 2020 2020 7374 6431  ignals..    std1
-0001adb0: 203d 2079 312e 7374 6428 290a 2020 2020   = y1.std().    
-0001adc0: 7374 6432 203d 2079 322e 7374 6428 290a  std2 = y2.std().
-0001add0: 2020 2020 2320 4e6f 726d 616c 697a 6573      # Normalizes
-0001ade0: 2062 6f74 6820 7369 676e 616c 732c 2069   both signals, i
-0001adf0: 6620 6170 7072 6f70 7269 6174 652e 0a20  f appropriate.. 
-0001ae00: 2020 2069 6620 6e6f 726d 616c 697a 653a     if normalize:
-0001ae10: 0a20 2020 2020 2020 2079 315f 6e6f 726d  .        y1_norm
-0001ae20: 616c 203d 2028 7931 202d 2079 312e 6d65  al = (y1 - y1.me
-0001ae30: 616e 2829 2920 2f20 7374 6431 0a20 2020  an()) / std1.   
-0001ae40: 2020 2020 2079 325f 6e6f 726d 616c 203d       y2_normal =
-0001ae50: 2028 7932 202d 2079 322e 6d65 616e 2829   (y2 - y2.mean()
-0001ae60: 2920 2f20 7374 6432 0a20 2020 2065 6c73  ) / std2.    els
-0001ae70: 653a 0a20 2020 2020 2020 2079 315f 6e6f  e:.        y1_no
-0001ae80: 726d 616c 203d 2079 310a 2020 2020 2020  rmal = y1.      
-0001ae90: 2020 7932 5f6e 6f72 6d61 6c20 3d20 7932    y2_normal = y2
-0001aea0: 0a0a 2020 2020 2320 4361 6c63 756c 6174  ..    # Calculat
-0001aeb0: 6573 2074 6865 2043 5754 206f 6620 7468  es the CWT of th
-0001aec0: 6520 7469 6d65 2d73 6572 6965 7320 6d61  e time-series ma
-0001aed0: 6b69 6e67 2073 7572 6520 7468 6520 7361  king sure the sa
-0001aee0: 6d65 2070 6172 616d 6574 6572 730a 2020  me parameters.  
-0001aef0: 2020 2320 6172 6520 7573 6564 2069 6e20    # are used in 
-0001af00: 626f 7468 2063 616c 6375 6c61 7469 6f6e  both calculation
-0001af10: 732e 0a20 2020 205f 6b77 6172 6773 203d  s..    _kwargs =
-0001af20: 2064 6963 7428 646a 3d64 6a2c 2073 303d   dict(dj=dj, s0=
-0001af30: 7330 2c20 4a3d 4a2c 2077 6176 656c 6574  s0, J=J, wavelet
-0001af40: 3d77 6176 656c 6574 290a 2020 2020 5731  =wavelet).    W1
-0001af50: 2c20 736a 2c20 6672 6571 2c20 636f 692c  , sj, freq, coi,
-0001af60: 205f 2c20 5f20 3d20 7079 6377 742e 6377   _, _ = pycwt.cw
-0001af70: 7428 7931 5f6e 6f72 6d61 6c2c 2064 742c  t(y1_normal, dt,
-0001af80: 202a 2a5f 6b77 6172 6773 290a 2020 2020   **_kwargs).    
-0001af90: 5732 2c20 736a 2c20 6672 6571 2c20 636f  W2, sj, freq, co
-0001afa0: 692c 205f 2c20 5f20 3d20 7079 6377 742e  i, _, _ = pycwt.
-0001afb0: 6377 7428 7932 5f6e 6f72 6d61 6c2c 2064  cwt(y2_normal, d
-0001afc0: 742c 202a 2a5f 6b77 6172 6773 290a 0a20  t, **_kwargs).. 
-0001afd0: 2020 2073 6361 6c65 7331 203d 206e 702e     scales1 = np.
-0001afe0: 6f6e 6573 285b 312c 2079 312e 7369 7a65  ones([1, y1.size
-0001aff0: 5d29 202a 2073 6a5b 3a2c 204e 6f6e 655d  ]) * sj[:, None]
-0001b000: 0a20 2020 2073 6361 6c65 7332 203d 206e  .    scales2 = n
-0001b010: 702e 6f6e 6573 285b 312c 2079 322e 7369  p.ones([1, y2.si
-0001b020: 7a65 5d29 202a 2073 6a5b 3a2c 204e 6f6e  ze]) * sj[:, Non
-0001b030: 655d 0a0a 2020 2020 2320 536d 6f6f 7468  e]..    # Smooth
-0001b040: 2074 6865 2077 6176 656c 6574 2073 7065   the wavelet spe
-0001b050: 6374 7261 2062 6566 6f72 6520 7472 756e  ctra before trun
-0001b060: 6361 7469 6e67 2e0a 2020 2020 5331 203d  cating..    S1 =
-0001b070: 2077 6176 656c 6574 2e73 6d6f 6f74 6828   wavelet.smooth(
-0001b080: 6e70 2e61 6273 2857 3129 202a 2a20 3220  np.abs(W1) ** 2 
-0001b090: 2f20 7363 616c 6573 312c 2064 742c 2064  / scales1, dt, d
-0001b0a0: 6a2c 2073 6a29 0a20 2020 2053 3220 3d20  j, sj).    S2 = 
-0001b0b0: 7761 7665 6c65 742e 736d 6f6f 7468 286e  wavelet.smooth(n
-0001b0c0: 702e 6162 7328 5732 2920 2a2a 2032 202f  p.abs(W2) ** 2 /
-0001b0d0: 2073 6361 6c65 7332 2c20 6474 2c20 646a   scales2, dt, dj
-0001b0e0: 2c20 736a 290a 0a20 2020 2023 204e 6f77  , sj)..    # Now
-0001b0f0: 2074 6865 2077 6176 656c 6574 2074 7261   the wavelet tra
-0001b100: 6e73 666f 726d 2063 6f68 6572 656e 6365  nsform coherence
-0001b110: 0a20 2020 2057 3132 203d 2057 3120 2a20  .    W12 = W1 * 
-0001b120: 5732 2e63 6f6e 6a28 290a 2020 2020 7363  W2.conj().    sc
-0001b130: 616c 6573 203d 206e 702e 6f6e 6573 285b  ales = np.ones([
-0001b140: 312c 2079 312e 7369 7a65 5d29 202a 2073  1, y1.size]) * s
-0001b150: 6a5b 3a2c 204e 6f6e 655d 0a20 2020 2053  j[:, None].    S
-0001b160: 3132 203d 2077 6176 656c 6574 2e73 6d6f  12 = wavelet.smo
-0001b170: 6f74 6828 5731 3220 2f20 7363 616c 6573  oth(W12 / scales
-0001b180: 2c20 6474 2c20 646a 2c20 736a 290a 2020  , dt, dj, sj).  
-0001b190: 2020 5743 5420 3d20 6e70 2e61 6273 2853    WCT = np.abs(S
-0001b1a0: 3132 2920 2a2a 2032 202f 2028 5331 202a  12) ** 2 / (S1 *
-0001b1b0: 2053 3229 0a20 2020 2061 5743 5420 3d20   S2).    aWCT = 
-0001b1c0: 6e70 2e61 6e67 6c65 2857 3132 290a 0a20  np.angle(W12).. 
-0001b1d0: 2020 2023 2043 616c 6375 6c61 7465 7320     # Calculates 
-0001b1e0: 7468 6520 7369 676e 6966 6963 616e 6365  the significance
-0001b1f0: 2075 7369 6e67 204d 6f6e 7465 2043 6172   using Monte Car
-0001b200: 6c6f 2073 696d 756c 6174 696f 6e73 2077  lo simulations w
-0001b210: 6974 6820 3935 250a 2020 2020 2320 636f  ith 95%.    # co
-0001b220: 6e66 6964 656e 6365 2061 7320 6120 6675  nfidence as a fu
-0001b230: 6e63 7469 6f6e 206f 6620 7363 616c 652e  nction of scale.
-0001b240: 0a0a 2020 2020 6966 2073 6967 3a0a 2020  ..    if sig:.  
-0001b250: 2020 2020 2020 6131 2c20 6231 2c20 6331        a1, b1, c1
-0001b260: 203d 2070 7963 7774 2e61 7231 2879 3129   = pycwt.ar1(y1)
-0001b270: 0a20 2020 2020 2020 2061 322c 2062 322c  .        a2, b2,
-0001b280: 2063 3220 3d20 7079 6377 742e 6172 3128   c2 = pycwt.ar1(
-0001b290: 7932 290a 2020 2020 2020 2020 7369 6720  y2).        sig 
-0001b2a0: 3d20 7079 6377 742e 7763 745f 7369 676e  = pycwt.wct_sign
-0001b2b0: 6966 6963 616e 6365 280a 2020 2020 2020  ificance(.      
-0001b2c0: 2020 2020 2020 6131 2c20 6132 2c20 6474        a1, a2, dt
-0001b2d0: 3d64 742c 2064 6a3d 646a 2c20 7330 3d73  =dt, dj=dj, s0=s
-0001b2e0: 302c 204a 3d4a 2c20 7369 676e 6966 6963  0, J=J, signific
-0001b2f0: 616e 6365 5f6c 6576 656c 3d73 6967 6e69  ance_level=signi
-0001b300: 6669 6361 6e63 655f 6c65 7665 6c2c 2077  ficance_level, w
-0001b310: 6176 656c 6574 3d77 6176 656c 6574 2c20  avelet=wavelet, 
-0001b320: 2a2a 6b77 6172 6773 0a20 2020 2020 2020  **kwargs.       
-0001b330: 2029 0a20 2020 2065 6c73 653a 0a20 2020   ).    else:.   
-0001b340: 2020 2020 2073 6967 203d 206e 702e 6173       sig = np.as
-0001b350: 6172 7261 7928 5b30 5d29 0a0a 2020 2020  array([0])..    
-0001b360: 7265 7475 726e 2057 4354 2c20 6157 4354  return WCT, aWCT
-0001b370: 2c20 636f 692c 2066 7265 712c 2073 6967  , coi, freq, sig
-0001b380: 0a0a 0a23 2323 2323 2323 2323 2323 2323  ...#############
-0001b390: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001b3a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001b3b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001b3c0: 2323 230a 2323 2323 2323 2323 2323 2323  ###.############
-0001b3d0: 2323 2323 2044 4953 5045 5253 494f 4e20  #### DISPERSION 
-0001b3e0: 4558 5452 4143 5449 4f4e 2046 554e 4354  EXTRACTION FUNCT
-0001b3f0: 494f 4e53 2023 2323 2323 2323 2323 2323  IONS ###########
-0001b400: 2323 2323 0a23 2323 2323 2323 2323 2323  ####.###########
-0001b410: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001b420: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001b430: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001b440: 2323 2323 230a 0a0a 2320 6675 6e63 7469  #####...# functi
-0001b450: 6f6e 2074 6f20 6578 7472 6163 7420 7468  on to extract th
-0001b460: 6520 6469 7370 6572 7369 6f6e 2066 726f  e dispersion fro
-0001b470: 6d20 7468 6520 696d 6167 650a 6465 6620  m the image.def 
-0001b480: 6578 7472 6163 745f 6469 7370 6572 7369  extract_dispersi
-0001b490: 6f6e 2861 6d70 2c20 7065 722c 2076 656c  on(amp, per, vel
-0001b4a0: 293a 0a20 2020 2022 2222 0a20 2020 2074  ):.    """.    t
-0001b4b0: 6869 7320 6675 6e63 7469 6f6e 2074 616b  his function tak
-0001b4c0: 6573 2074 6865 2064 6973 7065 7273 696f  es the dispersio
-0001b4d0: 6e20 696d 6167 6520 6672 6f6d 2043 5754  n image from CWT
-0001b4e0: 2061 7320 696e 7075 742c 2074 7261 636b   as input, track
-0001b4f0: 7320 7468 6520 676c 6f62 616c 206d 6178  s the global max
-0001b500: 696e 756d 206f 6e0a 2020 2020 7468 6520  inum on.    the 
-0001b510: 7761 7665 6c65 7420 7370 6563 7472 756d  wavelet spectrum
-0001b520: 2061 6d70 6c69 7475 6465 2061 6e64 2065   amplitude and e
-0001b530: 7874 7261 6374 2074 6865 2073 6563 7469  xtract the secti
-0001b540: 6f6e 7320 7769 7468 2063 6f6e 7469 6e6f  ons with contino
-0001b550: 7573 2061 6e64 2068 6967 6820 7175 616c  us and high qual
-0001b560: 6974 7920 6461 7461 0a0a 2020 2020 5041  ity data..    PA
-0001b570: 5241 4d45 5445 5253 3a0a 2020 2020 2d2d  RAMETERS:.    --
-0001b580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
-0001b590: 2020 2061 6d70 3a20 3244 2061 6d70 6c69     amp: 2D ampli
-0001b5a0: 7475 6465 206d 6174 7269 7820 6f66 2074  tude matrix of t
-0001b5b0: 6865 2077 6176 656c 6574 2073 7065 6374  he wavelet spect
-0001b5c0: 7275 6d0a 2020 2020 7068 6173 653a 2032  rum.    phase: 2
-0001b5d0: 4420 7068 6173 6520 6d61 7472 6978 206f  D phase matrix o
-0001b5e0: 6620 7468 6520 7761 7665 6c65 7420 7370  f the wavelet sp
-0001b5f0: 6563 7472 756d 0a20 2020 2070 6572 3a20  ectrum.    per: 
-0001b600: 2070 6572 696f 6420 7665 6374 6f72 2066   period vector f
-0001b610: 6f72 2074 6865 2032 4420 6d61 7472 6978  or the 2D matrix
-0001b620: 0a20 2020 2076 656c 3a20 2076 656c 2076  .    vel:  vel v
-0001b630: 6563 746f 7220 6f66 2074 6865 2032 4420  ector of the 2D 
-0001b640: 6d61 7472 6978 0a20 2020 2052 4554 5552  matrix.    RETUR
-0001b650: 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  NS:.    --------
-0001b660: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2070 6572  --------.    per
-0001b670: 3a20 2063 656e 7472 616c 2066 7265 7175  :  central frequ
-0001b680: 656e 6379 206f 6620 6561 6368 2077 6176  ency of each wav
-0001b690: 656c 6574 2073 6361 6c65 2077 6974 6820  elet scale with 
-0001b6a0: 676f 6f64 2064 6174 610a 2020 2020 6776  good data.    gv
-0001b6b0: 3a20 2020 6772 6f75 7020 7665 6c6f 6369  :   group veloci
-0001b6c0: 7479 2076 6563 746f 7220 6174 2065 6163  ty vector at eac
-0001b6d0: 6820 6672 6571 7565 6e63 790a 2020 2020  h frequency.    
-0001b6e0: 2222 220a 2020 2020 6d61 7867 6170 203d  """.    maxgap =
-0001b6f0: 2035 0a20 2020 206e 7065 7220 3d20 616d   5.    nper = am
-0001b700: 702e 7368 6170 655b 305d 0a20 2020 2067  p.shape[0].    g
-0001b710: 7620 3d20 6e70 2e7a 6572 6f73 286e 7065  v = np.zeros(npe
-0001b720: 722c 2064 7479 7065 3d6e 702e 666c 6f61  r, dtype=np.floa
-0001b730: 7433 3229 0a20 2020 2064 7665 6c20 3d20  t32).    dvel = 
-0001b740: 7665 6c5b 315d 202d 2076 656c 5b30 5d0a  vel[1] - vel[0].
-0001b750: 0a20 2020 2023 2066 696e 6420 676c 6f62  .    # find glob
-0001b760: 616c 206d 6178 696d 756d 0a20 2020 2066  al maximum.    f
-0001b770: 6f72 2069 6920 696e 2072 616e 6765 286e  or ii in range(n
-0001b780: 7065 7229 3a0a 2020 2020 2020 2020 6d61  per):.        ma
-0001b790: 7876 616c 7565 203d 206e 702e 6d61 7828  xvalue = np.max(
-0001b7a0: 616d 705b 6969 5d2c 2061 7869 733d 3029  amp[ii], axis=0)
-0001b7b0: 0a20 2020 2020 2020 2069 6e64 7820 3d20  .        indx = 
-0001b7c0: 6c69 7374 2861 6d70 5b69 695d 292e 696e  list(amp[ii]).in
-0001b7d0: 6465 7828 6d61 7876 616c 7565 290a 2020  dex(maxvalue).  
-0001b7e0: 2020 2020 2020 6776 5b69 695d 203d 2076        gv[ii] = v
-0001b7f0: 656c 5b69 6e64 785d 0a0a 2020 2020 2320  el[indx]..    # 
-0001b800: 6368 6563 6b20 7468 6520 636f 6e74 696e  check the contin
-0001b810: 756f 7573 206f 6620 7468 6520 6469 7370  uous of the disp
-0001b820: 6572 7369 6f6e 0a20 2020 2066 6f72 2069  ersion.    for i
-0001b830: 6920 696e 2072 616e 6765 2831 2c20 6e70  i in range(1, np
-0001b840: 6572 202d 2031 3529 3a0a 2020 2020 2020  er - 15):.      
-0001b850: 2020 2320 3135 2069 7320 7468 6520 6d69    # 15 is the mi
-0001b860: 6e75 6d75 6d20 6c65 6e67 7468 206e 6565  numum length nee
-0001b870: 6465 6420 666f 7220 6f75 7470 7574 0a20  ded for output. 
-0001b880: 2020 2020 2020 2066 6f72 206a 6a20 696e         for jj in
-0001b890: 2072 616e 6765 2831 3529 3a0a 2020 2020   range(15):.    
-0001b8a0: 2020 2020 2020 2020 6966 206e 702e 6162          if np.ab
-0001b8b0: 7328 6776 5b69 6920 2b20 6a6a 5d20 2d20  s(gv[ii + jj] - 
-0001b8c0: 6776 5b69 6920 2b20 3120 2b20 6a6a 5d29  gv[ii + 1 + jj])
-0001b8d0: 203e 206d 6178 6761 7020 2a20 6476 656c   > maxgap * dvel
-0001b8e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001b8f0: 2020 6776 5b69 695d 203d 2030 0a20 2020    gv[ii] = 0.   
-0001b900: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-0001b910: 616b 0a0a 2020 2020 2320 7265 6d6f 7665  ak..    # remove
-0001b920: 2074 6865 2062 6164 206f 6e65 730a 2020   the bad ones.  
-0001b930: 2020 696e 6478 203d 206e 702e 7768 6572    indx = np.wher
-0001b940: 6528 6776 203e 2030 295b 305d 0a0a 2020  e(gv > 0)[0]..  
-0001b950: 2020 7265 7475 726e 2070 6572 5b69 6e64    return per[ind
-0001b960: 785d 2c20 6776 5b69 6e64 785d 0a         x], gv[indx].
+0000ad90: 6220 3d20 6e70 2e73 696e 2862 617a 202a  b = np.sin(baz *
+0000ada0: 2070 6920 2f20 3138 3029 0a0a 2020 2020   pi / 180)..    
+0000adb0: 2320 7274 7a5f 636f 6d70 6f6e 656e 7473  # rtz_components
+0000adc0: 203d 205b 275a 5227 2c27 5a54 272c 275a   = ['ZR','ZT','Z
+0000add0: 5a27 2c27 5252 272c 2752 5427 2c27 525a  Z','RR','RT','RZ
+0000ade0: 272c 2754 5227 2c27 5454 272c 2754 5a27  ','TR','TT','TZ'
+0000adf0: 5d0a 2020 2020 7463 6f72 7220 3d20 6e70  ].    tcorr = np
+0000ae00: 2e7a 6572 6f73 2873 6861 7065 3d28 392c  .zeros(shape=(9,
+0000ae10: 206e 7074 7329 2c20 6474 7970 653d 6e70   npts), dtype=np
+0000ae20: 2e66 6c6f 6174 3332 290a 2020 2020 7463  .float32).    tc
+0000ae30: 6f72 725b 305d 203d 202d 636f 7362 202a  orr[0] = -cosb *
+0000ae40: 2062 6967 7374 6163 6b5b 375d 202d 2073   bigstack[7] - s
+0000ae50: 696e 6220 2a20 6269 6773 7461 636b 5b36  inb * bigstack[6
+0000ae60: 5d0a 2020 2020 7463 6f72 725b 315d 203d  ].    tcorr[1] =
+0000ae70: 2073 696e 6220 2a20 6269 6773 7461 636b   sinb * bigstack
+0000ae80: 5b37 5d20 2d20 636f 7362 202a 2062 6967  [7] - cosb * big
+0000ae90: 7374 6163 6b5b 365d 0a20 2020 2074 636f  stack[6].    tco
+0000aea0: 7272 5b32 5d20 3d20 6269 6773 7461 636b  rr[2] = bigstack
+0000aeb0: 5b38 5d0a 2020 2020 7463 6f72 725b 335d  [8].    tcorr[3]
+0000aec0: 203d 2028 0a20 2020 2020 2020 202d 636f   = (.        -co
+0000aed0: 7361 202a 2063 6f73 6220 2a20 6269 6773  sa * cosb * bigs
+0000aee0: 7461 636b 5b34 5d20 2d20 636f 7361 202a  tack[4] - cosa *
+0000aef0: 2073 696e 6220 2a20 6269 6773 7461 636b   sinb * bigstack
+0000af00: 5b33 5d20 2d20 7369 6e61 202a 2063 6f73  [3] - sina * cos
+0000af10: 6220 2a20 6269 6773 7461 636b 5b31 5d20  b * bigstack[1] 
+0000af20: 2d20 7369 6e61 202a 2073 696e 6220 2a20  - sina * sinb * 
+0000af30: 6269 6773 7461 636b 5b30 5d0a 2020 2020  bigstack[0].    
+0000af40: 290a 2020 2020 7463 6f72 725b 345d 203d  ).    tcorr[4] =
+0000af50: 2028 0a20 2020 2020 2020 2063 6f73 6120   (.        cosa 
+0000af60: 2a20 7369 6e62 202a 2062 6967 7374 6163  * sinb * bigstac
+0000af70: 6b5b 345d 202d 2063 6f73 6120 2a20 636f  k[4] - cosa * co
+0000af80: 7362 202a 2062 6967 7374 6163 6b5b 335d  sb * bigstack[3]
+0000af90: 202b 2073 696e 6120 2a20 7369 6e62 202a   + sina * sinb *
+0000afa0: 2062 6967 7374 6163 6b5b 315d 202d 2073   bigstack[1] - s
+0000afb0: 696e 6120 2a20 636f 7362 202a 2062 6967  ina * cosb * big
+0000afc0: 7374 6163 6b5b 305d 0a20 2020 2029 0a20  stack[0].    ). 
+0000afd0: 2020 2074 636f 7272 5b35 5d20 3d20 636f     tcorr[5] = co
+0000afe0: 7361 202a 2062 6967 7374 6163 6b5b 355d  sa * bigstack[5]
+0000aff0: 202b 2073 696e 6120 2a20 6269 6773 7461   + sina * bigsta
+0000b000: 636b 5b32 5d0a 2020 2020 7463 6f72 725b  ck[2].    tcorr[
+0000b010: 365d 203d 2028 0a20 2020 2020 2020 2073  6] = (.        s
+0000b020: 696e 6120 2a20 636f 7362 202a 2062 6967  ina * cosb * big
+0000b030: 7374 6163 6b5b 345d 202b 2073 696e 6120  stack[4] + sina 
+0000b040: 2a20 7369 6e62 202a 2062 6967 7374 6163  * sinb * bigstac
+0000b050: 6b5b 335d 202d 2063 6f73 6120 2a20 636f  k[3] - cosa * co
+0000b060: 7362 202a 2062 6967 7374 6163 6b5b 315d  sb * bigstack[1]
+0000b070: 202d 2063 6f73 6120 2a20 7369 6e62 202a   - cosa * sinb *
+0000b080: 2062 6967 7374 6163 6b5b 305d 0a20 2020   bigstack[0].   
+0000b090: 2029 0a20 2020 2074 636f 7272 5b37 5d20   ).    tcorr[7] 
+0000b0a0: 3d20 280a 2020 2020 2020 2020 2d73 696e  = (.        -sin
+0000b0b0: 6120 2a20 7369 6e62 202a 2062 6967 7374  a * sinb * bigst
+0000b0c0: 6163 6b5b 345d 202b 2073 696e 6120 2a20  ack[4] + sina * 
+0000b0d0: 636f 7362 202a 2062 6967 7374 6163 6b5b  cosb * bigstack[
+0000b0e0: 335d 202b 2063 6f73 6120 2a20 7369 6e62  3] + cosa * sinb
+0000b0f0: 202a 2062 6967 7374 6163 6b5b 315d 202d   * bigstack[1] -
+0000b100: 2063 6f73 6120 2a20 636f 7362 202a 2062   cosa * cosb * b
+0000b110: 6967 7374 6163 6b5b 305d 0a20 2020 2029  igstack[0].    )
+0000b120: 0a20 2020 2074 636f 7272 5b38 5d20 3d20  .    tcorr[8] = 
+0000b130: 2d73 696e 6120 2a20 6269 6773 7461 636b  -sina * bigstack
+0000b140: 5b35 5d20 2b20 636f 7361 202a 2062 6967  [5] + cosa * big
+0000b150: 7374 6163 6b5b 325d 0a0a 2020 2020 7265  stack[2]..    re
+0000b160: 7475 726e 2074 636f 7272 0a0a 0a23 2323  turn tcorr...###
+0000b170: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000b180: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000b190: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000b1a0: 230a 2323 2323 2323 2323 2323 2323 2323  #.##############
+0000b1b0: 2055 5449 4c49 5459 2046 554e 4354 494f   UTILITY FUNCTIO
+0000b1c0: 4e53 2023 2323 2323 2323 2323 2323 2323  NS #############
+0000b1d0: 2323 2323 2323 0a23 2323 2323 2323 2323  ######.#########
+0000b1e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000b1f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000b200: 2323 2323 2323 2323 2323 230a 0a0a 6465  ###########...de
+0000b210: 6620 6368 6563 6b5f 7361 6d70 6c65 5f67  f check_sample_g
+0000b220: 6170 7328 7374 7265 616d 3a20 6f62 7370  aps(stream: obsp
+0000b230: 792e 5374 7265 616d 2c20 7374 6172 7474  y.Stream, startt
+0000b240: 696d 653a 206f 6273 7079 2e55 5443 4461  ime: obspy.UTCDa
+0000b250: 7465 5469 6d65 2c20 656e 6474 696d 653a  teTime, endtime:
+0000b260: 206f 6273 7079 2e55 5443 4461 7465 5469   obspy.UTCDateTi
+0000b270: 6d65 293a 0a20 2020 2022 2222 0a20 2020  me):.    """.   
+0000b280: 2074 6869 7320 6675 6e63 7469 6f6e 2063   this function c
+0000b290: 6865 636b 7320 7361 6d70 6c69 6e67 2072  hecks sampling r
+0000b2a0: 6174 6520 616e 6420 6669 6e64 2067 6170  ate and find gap
+0000b2b0: 7320 6f66 2061 6c6c 2074 7261 6365 7320  s of all traces 
+0000b2c0: 696e 2073 7472 6561 6d2e 0a20 2020 2050  in stream..    P
+0000b2d0: 4152 414d 4554 4552 533a 0a20 2020 202d  ARAMETERS:.    -
+0000b2e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b2f0: 0a20 2020 2073 7472 6561 6d3a 206f 6273  .    stream: obs
+0000b300: 7079 2073 7472 6561 6d20 6f62 6a65 6374  py stream object
+0000b310: 2e0a 2020 2020 6461 7465 5f69 6e66 6f3a  ..    date_info:
+0000b320: 2064 6963 7420 6f66 2073 7461 7274 696e   dict of startin
+0000b330: 6720 616e 6420 656e 6469 6e67 2074 696d  g and ending tim
+0000b340: 6520 6f66 2074 6865 2073 7472 6561 6d0a  e of the stream.
+0000b350: 0a20 2020 2052 4554 5552 454e 533a 0a20  .    RETURENS:. 
+0000b360: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+0000b370: 2d2d 2d2d 0a20 2020 2073 7472 6561 6d3a  ----.    stream:
+0000b380: 204c 6973 7420 6f66 2067 6f6f 6420 7472   List of good tr
+0000b390: 6163 6573 2069 6e20 7468 6520 7374 7265  aces in the stre
+0000b3a0: 616d 0a20 2020 2022 2222 0a20 2020 2023  am.    """.    #
+0000b3b0: 2072 656d 6f76 6520 656d 7074 792f 6269   remove empty/bi
+0000b3c0: 6720 7472 6163 6573 0a20 2020 2069 6620  g traces.    if 
+0000b3d0: 6c65 6e28 7374 7265 616d 2920 3d3d 2030  len(stream) == 0
+0000b3e0: 206f 7220 6c65 6e28 7374 7265 616d 2920   or len(stream) 
+0000b3f0: 3e20 3130 303a 0a20 2020 2020 2020 2073  > 100:.        s
+0000b400: 7472 6561 6d20 3d20 5b5d 0a20 2020 2020  tream = [].     
+0000b410: 2020 2072 6574 7572 6e20 7374 7265 616d     return stream
+0000b420: 0a0a 2020 2020 2320 7265 6d6f 7665 2074  ..    # remove t
+0000b430: 7261 6365 7320 7769 7468 2062 6967 2067  races with big g
+0000b440: 6170 730a 2020 2020 6966 2070 6f72 7469  aps.    if porti
+0000b450: 6f6e 5f67 6170 7328 7374 7265 616d 2c20  on_gaps(stream, 
+0000b460: 7374 6172 7474 696d 652c 2065 6e64 7469  starttime, endti
+0000b470: 6d65 2920 3e20 302e 333a 0a20 2020 2020  me) > 0.3:.     
+0000b480: 2020 2073 7472 6561 6d20 3d20 5b5d 0a20     stream = []. 
+0000b490: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
+0000b4a0: 7265 616d 0a0a 2020 2020 6672 6571 7320  ream..    freqs 
+0000b4b0: 3d20 5b5d 0a20 2020 2066 6f72 2074 7220  = [].    for tr 
+0000b4c0: 696e 2073 7472 6561 6d3a 0a20 2020 2020  in stream:.     
+0000b4d0: 2020 2066 7265 7173 2e61 7070 656e 6428     freqs.append(
+0000b4e0: 696e 7428 7472 2e73 7461 7473 2e73 616d  int(tr.stats.sam
+0000b4f0: 706c 696e 675f 7261 7465 2929 0a20 2020  pling_rate)).   
+0000b500: 2066 7265 7120 3d20 6d61 7828 6672 6571   freq = max(freq
+0000b510: 7329 0a20 2020 2066 6f72 2074 7220 696e  s).    for tr in
+0000b520: 2073 7472 6561 6d3a 0a20 2020 2020 2020   stream:.       
+0000b530: 2069 6620 696e 7428 7472 2e73 7461 7473   if int(tr.stats
+0000b540: 2e73 616d 706c 696e 675f 7261 7465 2920  .sampling_rate) 
+0000b550: 213d 2066 7265 713a 0a20 2020 2020 2020  != freq:.       
+0000b560: 2020 2020 2073 7472 6561 6d2e 7265 6d6f       stream.remo
+0000b570: 7665 2874 7229 0a20 2020 2020 2020 2069  ve(tr).        i
+0000b580: 6620 7472 2e73 7461 7473 2e6e 7074 7320  f tr.stats.npts 
+0000b590: 3c20 3130 3a0a 2020 2020 2020 2020 2020  < 10:.          
+0000b5a0: 2020 7374 7265 616d 2e72 656d 6f76 6528    stream.remove(
+0000b5b0: 7472 290a 0a20 2020 2072 6574 7572 6e20  tr)..    return 
+0000b5c0: 7374 7265 616d 0a0a 0a64 6566 2070 6f72  stream...def por
+0000b5d0: 7469 6f6e 5f67 6170 7328 7374 7265 616d  tion_gaps(stream
+0000b5e0: 2c20 7374 6172 7474 696d 653a 206f 6273  , starttime: obs
+0000b5f0: 7079 2e55 5443 4461 7465 5469 6d65 2c20  py.UTCDateTime, 
+0000b600: 656e 6474 696d 653a 206f 6273 7079 2e55  endtime: obspy.U
+0000b610: 5443 4461 7465 5469 6d65 293a 0a20 2020  TCDateTime):.   
+0000b620: 2022 2222 0a20 2020 2074 6869 7320 6675   """.    this fu
+0000b630: 6e63 7469 6f6e 2074 7261 636b 7320 7468  nction tracks th
+0000b640: 6520 6761 7073 2028 6e70 7473 2920 6672  e gaps (npts) fr
+0000b650: 6f6d 2074 6865 2061 6363 756d 756c 6174  om the accumulat
+0000b660: 6564 2064 6966 6665 7265 6e63 6520 6265  ed difference be
+0000b670: 7477 6565 6e20 7374 6172 7474 696d 6520  tween starttime 
+0000b680: 616e 6420 656e 6474 696d 650a 2020 2020  and endtime.    
+0000b690: 6f66 2065 6163 6820 7374 7265 616d 2074  of each stream t
+0000b6a0: 7261 6365 2e20 6974 2072 656d 6f76 6573  race. it removes
+0000b6b0: 2074 7261 6365 2077 6974 6820 6761 7020   trace with gap 
+0000b6c0: 6c65 6e67 7468 203e 2033 3025 206f 6620  length > 30% of 
+0000b6d0: 7472 6163 6520 7369 7a65 2e0a 2020 2020  trace size..    
+0000b6e0: 5041 5241 4d45 5445 5253 3a0a 2020 2020  PARAMETERS:.    
+0000b6f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b700: 2d2d 2d0a 2020 2020 7374 7265 616d 3a20  ---.    stream: 
+0000b710: 6f62 7370 7920 7374 7265 616d 206f 626a  obspy stream obj
+0000b720: 6563 740a 2020 2020 6461 7465 5f69 6e66  ect.    date_inf
+0000b730: 6f3a 2064 6963 7420 6f66 2073 7461 7274  o: dict of start
+0000b740: 696e 6720 616e 6420 656e 6469 6e67 2074  ing and ending t
+0000b750: 696d 6520 6f66 2074 6865 2073 7472 6561  ime of the strea
+0000b760: 6d0a 0a20 2020 2052 4554 5552 4e53 3a0a  m..    RETURNS:.
+0000b770: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+0000b780: 2d2d 2d2d 2d0a 2020 2020 7067 6170 733a  -----.    pgaps:
+0000b790: 2070 726f 706f 7274 696f 6e20 6f66 2067   proportion of g
+0000b7a0: 6170 732f 616c 6c5f 7074 7320 696e 2073  aps/all_pts in s
+0000b7b0: 7472 6561 6d0a 2020 2020 2222 220a 2020  tream.    """.  
+0000b7c0: 2020 2320 6964 6561 6c20 6475 7261 7469    # ideal durati
+0000b7d0: 6f6e 206f 6620 6461 7461 0a20 2020 206e  on of data.    n
+0000b7e0: 7074 7320 3d20 2865 6e64 7469 6d65 202d  pts = (endtime -
+0000b7f0: 2073 7461 7274 7469 6d65 2920 2a20 7374   starttime) * st
+0000b800: 7265 616d 5b30 5d2e 7374 6174 732e 7361  ream[0].stats.sa
+0000b810: 6d70 6c69 6e67 5f72 6174 650a 0a20 2020  mpling_rate..   
+0000b820: 2070 6761 7073 203d 2030 0a20 2020 2023   pgaps = 0.    #
+0000b830: 206c 6f6f 7020 7468 726f 7567 6820 616c   loop through al
+0000b840: 6c20 7472 6163 6520 746f 2061 6363 756d  l trace to accum
+0000b850: 756c 6174 6520 6761 7073 0a20 2020 2066  ulate gaps.    f
+0000b860: 6f72 2069 6920 696e 2072 616e 6765 286c  or ii in range(l
+0000b870: 656e 2873 7472 6561 6d29 202d 2031 293a  en(stream) - 1):
+0000b880: 0a20 2020 2020 2020 2070 6761 7073 202b  .        pgaps +
+0000b890: 3d20 2873 7472 6561 6d5b 6969 202b 2031  = (stream[ii + 1
+0000b8a0: 5d2e 7374 6174 732e 7374 6172 7474 696d  ].stats.starttim
+0000b8b0: 6520 2d20 7374 7265 616d 5b69 695d 2e73  e - stream[ii].s
+0000b8c0: 7461 7473 2e65 6e64 7469 6d65 2920 2a20  tats.endtime) * 
+0000b8d0: 7374 7265 616d 5b69 695d 2e73 7461 7473  stream[ii].stats
+0000b8e0: 2e73 616d 706c 696e 675f 7261 7465 0a20  .sampling_rate. 
+0000b8f0: 2020 2069 6620 6e70 7473 2021 3d20 303a     if npts != 0:
+0000b900: 0a20 2020 2020 2020 2070 6761 7073 203d  .        pgaps =
+0000b910: 2070 6761 7073 202f 206e 7074 730a 2020   pgaps / npts.  
+0000b920: 2020 6966 206e 7074 7320 3d3d 2030 3a0a    if npts == 0:.
+0000b930: 2020 2020 2020 2020 7067 6170 7320 3d20          pgaps = 
+0000b940: 310a 2020 2020 7265 7475 726e 2070 6761  1.    return pga
+0000b950: 7073 0a0a 0a40 6a69 7428 2266 6c6f 6174  ps...@jit("float
+0000b960: 3332 5b3a 5d28 666c 6f61 7433 325b 3a5d  32[:](float32[:]
+0000b970: 2c66 6c6f 6174 3332 2922 290a 6465 6620  ,float32)").def 
+0000b980: 7365 676d 656e 745f 696e 7465 7270 6f6c  segment_interpol
+0000b990: 6174 6528 7369 6731 2c20 6e66 7269 6329  ate(sig1, nfric)
+0000b9a0: 3a0a 2020 2020 2222 220a 2020 2020 7468  :.    """.    th
+0000b9b0: 6973 2066 756e 6374 696f 6e20 696e 7465  is function inte
+0000b9c0: 7270 6f6c 6174 6573 2074 6865 2064 6174  rpolates the dat
+0000b9d0: 6120 746f 2065 6e73 7572 6520 616c 6c20  a to ensure all 
+0000b9e0: 706f 696e 7473 206c 6f63 6174 6564 206f  points located o
+0000b9f0: 6e20 696e 7465 7267 6572 2074 696d 6573  n interger times
+0000ba00: 206f 6620 7468 650a 2020 2020 7361 6d70   of the.    samp
+0000ba10: 6c69 6e67 2072 6174 6520 2865 2e67 2e2c  ling rate (e.g.,
+0000ba20: 2073 7461 7274 7469 6d65 203d 2030 303a   starttime = 00:
+0000ba30: 3030 3a30 302e 3031 352c 2064 656c 7461  00:00.015, delta
+0000ba40: 203d 2030 2e30 352e 290a 2020 2020 5041   = 0.05.).    PA
+0000ba50: 5241 4d45 5445 5253 3a0a 2020 2020 2d2d  RAMETERS:.    --
+0000ba60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000ba70: 2d2d 2d2d 0a20 2020 2073 6967 313a 2020  ----.    sig1:  
+0000ba80: 7365 6973 6d69 6320 7265 636f 7264 696e  seismic recordin
+0000ba90: 6773 2069 6e20 6120 3144 2061 7272 6179  gs in a 1D array
+0000baa0: 0a20 2020 206e 6672 6963 3a20 7468 6520  .    nfric: the 
+0000bab0: 616d 6f75 6e74 206f 6620 7469 6d65 2064  amount of time d
+0000bac0: 6966 6665 7265 6e63 6520 6265 7477 6565  ifference betwee
+0000bad0: 6e20 7468 6520 706f 696e 7420 616e 6420  n the point and 
+0000bae0: 7468 6520 6164 6a61 6365 6e74 2061 7373  the adjacent ass
+0000baf0: 756d 6564 2073 616d 706c 6573 0a20 2020  umed samples.   
+0000bb00: 2052 4554 5552 4e53 3a0a 2020 2020 2d2d   RETURNS:.    --
+0000bb10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000bb20: 2d2d 2d2d 0a20 2020 2073 6967 323a 2020  ----.    sig2:  
+0000bb30: 696e 7465 7270 6f6c 6174 6564 2073 6569  interpolated sei
+0000bb40: 736d 6963 2072 6563 6f72 6469 6e67 7320  smic recordings 
+0000bb50: 6f6e 2074 6865 2073 616d 706c 696e 6720  on the sampling 
+0000bb60: 706f 696e 7473 0a20 2020 2022 2222 0a20  points.    """. 
+0000bb70: 2020 206e 7074 7320 3d20 6c65 6e28 7369     npts = len(si
+0000bb80: 6731 290a 2020 2020 7369 6732 203d 206e  g1).    sig2 = n
+0000bb90: 702e 7a65 726f 7328 6e70 7473 2c20 6474  p.zeros(npts, dt
+0000bba0: 7970 653d 6e70 2e66 6c6f 6174 3332 290a  ype=np.float32).
+0000bbb0: 0a20 2020 2023 202d 2d2d 2d69 6e73 7465  .    # ----inste
+0000bbc0: 6164 206f 6620 7368 6966 7469 6e67 2c20  ad of shifting, 
+0000bbd0: 646f 2061 2069 6e74 6572 706f 6c61 7469  do a interpolati
+0000bbe0: 6f6e 2d2d 2d2d 2d2d 0a20 2020 2066 6f72  on------.    for
+0000bbf0: 2069 6920 696e 2072 616e 6765 286e 7074   ii in range(npt
+0000bc00: 7329 3a0a 2020 2020 2020 2020 2320 2d2d  s):.        # --
+0000bc10: 2d2d 6465 616c 2077 6974 6820 6564 6765  --deal with edge
+0000bc20: 732d 2d2d 2d2d 0a20 2020 2020 2020 2069  s-----.        i
+0000bc30: 6620 6969 203d 3d20 3020 6f72 2069 6920  f ii == 0 or ii 
+0000bc40: 3d3d 206e 7074 7320 2d20 313a 0a20 2020  == npts - 1:.   
+0000bc50: 2020 2020 2020 2020 2073 6967 325b 6969           sig2[ii
+0000bc60: 5d20 3d20 7369 6731 5b69 695d 0a20 2020  ] = sig1[ii].   
+0000bc70: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000bc80: 2020 2020 2020 2023 202d 2d2d 2d2d 2d69         # ------i
+0000bc90: 6e74 6572 706f 6c61 7465 2075 7369 6e67  nterpolate using
+0000bca0: 2061 2068 6174 2066 756e 6374 696f 6e2d   a hat function-
+0000bcb0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 2020  -----.          
+0000bcc0: 2020 7369 6732 5b69 695d 203d 2028 3120    sig2[ii] = (1 
+0000bcd0: 2d20 6e66 7269 6329 202a 2073 6967 315b  - nfric) * sig1[
+0000bce0: 6969 202b 2031 5d20 2b20 6e66 7269 6320  ii + 1] + nfric 
+0000bcf0: 2a20 7369 6731 5b69 695d 0a0a 2020 2020  * sig1[ii]..    
+0000bd00: 7265 7475 726e 2073 6967 320a 0a0a 6465  return sig2...de
+0000bd10: 6620 7265 7370 5f73 7065 6374 7275 6d28  f resp_spectrum(
+0000bd20: 736f 7572 6365 2c20 7265 7370 5f66 696c  source, resp_fil
+0000bd30: 652c 2064 6f77 6e73 616d 705f 6672 6571  e, downsamp_freq
+0000bd40: 2c20 7072 655f 6669 6c74 3d4e 6f6e 6529  , pre_filt=None)
+0000bd50: 3a0a 2020 2020 2222 220a 2020 2020 7468  :.    """.    th
+0000bd60: 6973 2066 756e 6374 696f 6e20 7265 6d6f  is function remo
+0000bd70: 7665 7320 7468 6520 696e 7374 7275 6d65  ves the instrume
+0000bd80: 6e74 2072 6573 706f 6e73 6520 7573 696e  nt response usin
+0000bd90: 6720 7265 7370 6f6e 7365 2073 7065 6374  g response spect
+0000bda0: 7275 6d20 6672 6f6d 2065 7661 6c72 6573  rum from evalres
+0000bdb0: 702e 0a20 2020 2074 6865 2072 6573 706f  p..    the respo
+0000bdc0: 6e73 6520 7370 6563 7472 756d 2069 7320  nse spectrum is 
+0000bdd0: 6576 616c 7561 7465 6420 6261 7365 6420  evaluated based 
+0000bde0: 6f6e 2052 4553 502f 505a 2066 696c 6573  on RESP/PZ files
+0000bdf0: 2062 6566 6f72 6520 696e 7665 7274 6564   before inverted
+0000be00: 2075 7369 6e67 2074 6865 206f 6273 7079   using the obspy
+0000be10: 0a20 2020 2066 756e 6374 696f 6e20 6f66  .    function of
+0000be20: 2069 6e76 6572 745f 7370 6563 7472 756d   invert_spectrum
+0000be30: 2e20 6120 6d6f 6475 6c65 206f 6620 6372  . a module of cr
+0000be40: 6561 7465 5f72 6573 702e 7079 2069 7320  eate_resp.py is 
+0000be50: 7072 6f76 6964 6564 2069 6e20 6469 7265  provided in dire
+0000be60: 6374 6f72 7920 6f66 2027 6164 6469 7469  ctory of 'additi
+0000be70: 6f6e 616c 5f6d 6f64 756c 6573 270a 2020  onal_modules'.  
+0000be80: 2020 746f 2063 7265 6174 6520 7468 6520    to create the 
+0000be90: 7265 7370 6f6e 7365 2073 7065 6374 7275  response spectru
+0000bea0: 6d0a 2020 2020 5041 5241 4d45 5445 5253  m.    PARAMETERS
+0000beb0: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  :.    ----------
+0000bec0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+0000bed0: 2073 6f75 7263 653a 206f 6273 7079 2073   source: obspy s
+0000bee0: 7472 6561 6d20 6f62 6a65 6374 206f 6620  tream object of 
+0000bef0: 7461 7267 6574 6564 206e 6f69 7365 2064  targeted noise d
+0000bf00: 6174 610a 2020 2020 7265 7370 5f66 696c  ata.    resp_fil
+0000bf10: 653a 206e 756d 7079 2064 6174 6120 6669  e: numpy data fi
+0000bf20: 6c65 206f 6620 7265 7370 6f6e 7365 2073  le of response s
+0000bf30: 7065 6374 7275 6d0a 2020 2020 646f 776e  pectrum.    down
+0000bf40: 7361 6d70 5f66 7265 713a 2073 616d 706c  samp_freq: sampl
+0000bf50: 696e 6720 7261 7465 206f 6620 7468 6520  ing rate of the 
+0000bf60: 736f 7572 6365 2064 6174 610a 2020 2020  source data.    
+0000bf70: 7072 655f 6669 6c74 3a20 7072 652d 6465  pre_filt: pre-de
+0000bf80: 6669 6e65 6420 6669 6c74 6572 2070 6172  fined filter par
+0000bf90: 616d 6574 6572 730a 2020 2020 5245 5455  ameters.    RETU
+0000bfa0: 524e 533a 0a20 2020 202d 2d2d 2d2d 2d2d  RNS:.    -------
+0000bfb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+0000bfc0: 2020 2020 736f 7572 6365 3a20 6f62 7370      source: obsp
+0000bfd0: 7920 7374 7265 616d 206f 626a 6563 7420  y stream object 
+0000bfe0: 6f66 206e 6f69 7365 2064 6174 6120 7769  of noise data wi
+0000bff0: 7468 2069 6e73 7472 756d 656e 7420 7265  th instrument re
+0000c000: 7370 6f6e 7365 2072 656d 6f76 6564 0a20  sponse removed. 
+0000c010: 2020 2022 2222 0a20 2020 2023 202d 2d2d     """.    # ---
+0000c020: 2d2d 2d2d 2d72 6573 705f 6669 6c65 2069  -----resp_file i
+0000c030: 7320 7468 6520 696e 7665 7274 6564 2073  s the inverted s
+0000c040: 7065 6374 7275 6d20 7265 7370 6f6e 7365  pectrum response
+0000c050: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7265  ---------.    re
+0000c060: 7370 7a20 3d20 6e70 2e6c 6f61 6428 7265  spz = np.load(re
+0000c070: 7370 5f66 696c 6529 0a20 2020 206e 7265  sp_file).    nre
+0000c080: 7370 7a20 3d20 7265 7370 7a5b 315d 5b3a  spz = respz[1][:
+0000c090: 5d0a 2020 2020 7370 6563 5f66 7265 7120  ].    spec_freq 
+0000c0a0: 3d20 6d61 7828 7265 7370 7a5b 305d 290a  = max(respz[0]).
+0000c0b0: 0a20 2020 2023 202d 2d2d 2d2d 2d2d 6f6e  .    # -------on
+0000c0c0: 2063 7572 7265 6e74 2074 7261 6365 2d2d   current trace--
+0000c0d0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 206e 6666  --------.    nff
+0000c0e0: 7420 3d20 5f6e 7074 7332 6e66 6674 2873  t = _npts2nfft(s
+0000c0f0: 6f75 7263 655b 305d 2e73 7461 7473 2e6e  ource[0].stats.n
+0000c100: 7074 7329 0a20 2020 2073 7073 203d 2069  pts).    sps = i
+0000c110: 6e74 2873 6f75 7263 655b 305d 2e73 7461  nt(source[0].sta
+0000c120: 7473 2e73 616d 706c 696e 675f 7261 7465  ts.sampling_rate
+0000c130: 290a 0a20 2020 2023 202d 2d2d 2d2d 2d2d  )..    # -------
+0000c140: 2d2d 646f 2074 6865 2069 6e74 6572 706f  --do the interpo
+0000c150: 6c61 7469 6f6e 2069 6620 6e65 6564 6564  lation if needed
+0000c160: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2069 6620  --------.    if 
+0000c170: 7370 6563 5f66 7265 7120 3c20 302e 3520  spec_freq < 0.5 
+0000c180: 2a20 7370 733a 0a20 2020 2020 2020 2072  * sps:.        r
+0000c190: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+0000c1a0: 2273 7065 6374 7275 6d20 6669 6c65 2068  "spectrum file h
+0000c1b0: 6173 2070 6561 6b20 6672 6571 2073 6d61  as peak freq sma
+0000c1c0: 6c6c 6572 2074 6861 6e20 7468 6520 6461  ller than the da
+0000c1d0: 7461 2c20 6162 6f72 7421 2229 0a20 2020  ta, abort!").   
+0000c1e0: 2065 6c73 653a 0a20 2020 2020 2020 2069   else:.        i
+0000c1f0: 6e64 7820 3d20 6e70 2e77 6865 7265 2872  ndx = np.where(r
+0000c200: 6573 707a 5b30 5d20 3c3d 2030 2e35 202a  espz[0] <= 0.5 *
+0000c210: 2073 7073 290a 2020 2020 2020 2020 6e66   sps).        nf
+0000c220: 7265 7120 3d20 6e70 2e6c 696e 7370 6163  req = np.linspac
+0000c230: 6528 302c 2030 2e35 202a 2073 7073 2c20  e(0, 0.5 * sps, 
+0000c240: 6e66 6674 202f 2f20 3220 2b20 3129 0a20  nfft // 2 + 1). 
+0000c250: 2020 2020 2020 206e 7265 7370 7a20 3d20         nrespz = 
+0000c260: 6e70 2e69 6e74 6572 7028 6e66 7265 712c  np.interp(nfreq,
+0000c270: 206e 702e 7265 616c 2872 6573 707a 5b30   np.real(respz[0
+0000c280: 5d5b 696e 6478 5d29 2c20 7265 7370 7a5b  ][indx]), respz[
+0000c290: 315d 5b69 6e64 785d 290a 0a20 2020 2023  1][indx])..    #
+0000c2a0: 202d 2d2d 2d64 6f20 696e 7465 7270 6f6c   ----do interpol
+0000c2b0: 6174 696f 6e20 6966 206e 6563 6573 7361  ation if necessa
+0000c2c0: 7279 2d2d 2d2d 2d0a 2020 2020 736f 7572  ry-----.    sour
+0000c2d0: 6365 5f73 7065 6374 203d 206e 702e 6666  ce_spect = np.ff
+0000c2e0: 742e 7266 6674 2873 6f75 7263 655b 305d  t.rfft(source[0]
+0000c2f0: 2e64 6174 612c 206e 3d6e 6666 7429 0a0a  .data, n=nfft)..
+0000c300: 2020 2020 2320 2d2d 2d2d 2d6e 7265 7370      # -----nresp
+0000c310: 7a20 6973 2069 6e76 6572 7365 6420 2877  z is inversed (w
+0000c320: 6174 6572 2d6c 6576 656c 6564 2920 7370  ater-leveled) sp
+0000c330: 6563 7472 756d 2d2d 2d2d 2d0a 2020 2020  ectrum-----.    
+0000c340: 736f 7572 6365 5f73 7065 6374 202a 3d20  source_spect *= 
+0000c350: 6e72 6573 707a 0a20 2020 2073 6f75 7263  nrespz.    sourc
+0000c360: 655b 305d 2e64 6174 6120 3d20 6e70 2e66  e[0].data = np.f
+0000c370: 6674 2e69 7266 6674 2873 6f75 7263 655f  ft.irfft(source_
+0000c380: 7370 6563 7429 5b30 203a 2073 6f75 7263  spect)[0 : sourc
+0000c390: 655b 305d 2e73 7461 7473 2e6e 7074 735d  e[0].stats.npts]
+0000c3a0: 0a0a 2020 2020 6966 2070 7265 5f66 696c  ..    if pre_fil
+0000c3b0: 7420 6973 206e 6f74 204e 6f6e 653a 0a20  t is not None:. 
+0000c3c0: 2020 2020 2020 2073 6f75 7263 655b 305d         source[0]
+0000c3d0: 2e64 6174 6120 3d20 6e70 2e66 6c6f 6174  .data = np.float
+0000c3e0: 3332 280a 2020 2020 2020 2020 2020 2020  32(.            
+0000c3f0: 6261 6e64 7061 7373 280a 2020 2020 2020  bandpass(.      
+0000c400: 2020 2020 2020 2020 2020 736f 7572 6365            source
+0000c410: 5b30 5d2e 6461 7461 2c0a 2020 2020 2020  [0].data,.      
+0000c420: 2020 2020 2020 2020 2020 7072 655f 6669            pre_fi
+0000c430: 6c74 5b30 5d2c 0a20 2020 2020 2020 2020  lt[0],.         
+0000c440: 2020 2020 2020 2070 7265 5f66 696c 745b         pre_filt[
+0000c450: 2d31 5d2c 0a20 2020 2020 2020 2020 2020  -1],.           
+0000c460: 2020 2020 2064 663d 7370 732c 0a20 2020       df=sps,.   
+0000c470: 2020 2020 2020 2020 2020 2020 2063 6f72               cor
+0000c480: 6e65 7273 3d34 2c0a 2020 2020 2020 2020  ners=4,.        
+0000c490: 2020 2020 2020 2020 7a65 726f 7068 6173          zerophas
+0000c4a0: 653d 5472 7565 2c0a 2020 2020 2020 2020  e=True,.        
+0000c4b0: 2020 2020 290a 2020 2020 2020 2020 290a      ).        ).
+0000c4c0: 0a20 2020 2072 6574 7572 6e20 736f 7572  .    return sour
+0000c4d0: 6365 0a0a 0a64 6566 206d 6164 2861 7272  ce...def mad(arr
+0000c4e0: 293a 0a20 2020 2022 2222 0a20 2020 204d  ):.    """.    M
+0000c4f0: 6564 6961 6e20 4162 736f 6c75 7465 2044  edian Absolute D
+0000c500: 6576 6961 7469 6f6e 3a20 4d41 4420 3d20  eviation: MAD = 
+0000c510: 6d65 6469 616e 287c 5869 2d20 6d65 6469  median(|Xi- medi
+0000c520: 616e 2858 297c 290a 2020 2020 5041 5241  an(X)|).    PARA
+0000c530: 4d45 5445 5253 3a0a 2020 2020 2d2d 2d2d  METERS:.    ----
+0000c540: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+0000c550: 2020 2020 6172 723a 206e 756d 7079 2e6e      arr: numpy.n
+0000c560: 6461 7272 6179 2c20 7365 6973 6d69 6320  darray, seismic 
+0000c570: 7472 6163 6520 6461 7461 2061 7272 6179  trace data array
+0000c580: 0a20 2020 2052 4554 5552 4e53 3a0a 2020  .    RETURNS:.  
+0000c590: 2020 6461 7461 3a20 4d65 6469 616e 2041    data: Median A
+0000c5a0: 6273 6f6c 7574 6520 4465 7669 6174 696f  bsolute Deviatio
+0000c5b0: 6e20 6f66 2064 6174 610a 2020 2020 2222  n of data.    ""
+0000c5c0: 220a 2020 2020 6966 206e 6f74 206e 702e  ".    if not np.
+0000c5d0: 6d61 2e69 735f 6d61 736b 6564 2861 7272  ma.is_masked(arr
+0000c5e0: 293a 0a20 2020 2020 2020 206d 6564 203d  ):.        med =
+0000c5f0: 206e 702e 6d65 6469 616e 2861 7272 290a   np.median(arr).
+0000c600: 2020 2020 2020 2020 6461 7461 203d 206e          data = n
+0000c610: 702e 6d65 6469 616e 286e 702e 6162 7328  p.median(np.abs(
+0000c620: 6172 7220 2d20 6d65 6429 290a 2020 2020  arr - med)).    
+0000c630: 656c 7365 3a0a 2020 2020 2020 2020 6d65  else:.        me
+0000c640: 6420 3d20 6e70 2e6d 612e 6d65 6469 616e  d = np.ma.median
+0000c650: 2861 7272 290a 2020 2020 2020 2020 6461  (arr).        da
+0000c660: 7461 203d 206e 702e 6d61 2e6d 6564 6961  ta = np.ma.media
+0000c670: 6e28 6e70 2e6d 612e 6162 7328 6172 7220  n(np.ma.abs(arr 
+0000c680: 2d20 6d65 6429 290a 2020 2020 7265 7475  - med)).    retu
+0000c690: 726e 2064 6174 610a 0a0a 6465 6620 6465  rn data...def de
+0000c6a0: 7472 656e 6428 6461 7461 293a 0a20 2020  trend(data):.   
+0000c6b0: 2022 2222 0a20 2020 2074 6869 7320 6675   """.    this fu
+0000c6c0: 6e63 7469 6f6e 2072 656d 6f76 6573 2074  nction removes t
+0000c6d0: 6865 2073 6967 6e61 6c20 7472 656e 6420  he signal trend 
+0000c6e0: 6261 7365 6420 6f6e 2051 5220 6465 636f  based on QR deco
+0000c6f0: 6d70 6f73 696f 6e0a 2020 2020 4e4f 5445  mposion.    NOTE
+0000c700: 3a20 5152 2069 7320 6120 6c6f 7420 6661  : QR is a lot fa
+0000c710: 7374 6572 2074 6861 6e20 7468 6520 6c65  ster than the le
+0000c720: 6173 7420 7371 7561 7265 2069 6e76 6572  ast square inver
+0000c730: 7369 6f6e 2075 7365 6420 6279 0a20 2020  sion used by.   
+0000c740: 2073 6369 7079 2028 616c 736f 2069 6e20   scipy (also in 
+0000c750: 6f62 7370 7929 2e0a 2020 2020 5041 5241  obspy)..    PARA
+0000c760: 4d45 5445 5253 3a0a 2020 2020 2d2d 2d2d  METERS:.    ----
+0000c770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000c780: 2d0a 2020 2020 6461 7461 3a20 696e 7075  -.    data: inpu
+0000c790: 7420 6461 7461 206d 6174 7269 780a 2020  t data matrix.  
+0000c7a0: 2020 5245 5455 524e 533a 0a20 2020 202d    RETURNS:.    -
+0000c7b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000c7c0: 2d2d 2d2d 0a20 2020 2064 6174 613a 2064  ----.    data: d
+0000c7d0: 6174 6120 6d61 7472 6978 2077 6974 6820  ata matrix with 
+0000c7e0: 7472 656e 6420 7265 6d6f 7665 640a 2020  trend removed.  
+0000c7f0: 2020 2222 220a 2020 2020 2320 6e64 6174    """.    # ndat
+0000c800: 6120 3d20 6e70 2e7a 6572 6f73 2873 6861  a = np.zeros(sha
+0000c810: 7065 3d64 6174 612e 7368 6170 652c 6474  pe=data.shape,dt
+0000c820: 7970 653d 6461 7461 2e64 7479 7065 290a  ype=data.dtype).
+0000c830: 2020 2020 6966 2064 6174 612e 6e64 696d      if data.ndim
+0000c840: 203d 3d20 313a 0a20 2020 2020 2020 206e   == 1:.        n
+0000c850: 7074 7320 3d20 6461 7461 2e73 6861 7065  pts = data.shape
+0000c860: 5b30 5d0a 2020 2020 2020 2020 5820 3d20  [0].        X = 
+0000c870: 6e70 2e6f 6e65 7328 286e 7074 732c 2032  np.ones((npts, 2
+0000c880: 2929 0a20 2020 2020 2020 2058 5b3a 2c20  )).        X[:, 
+0000c890: 305d 203d 206e 702e 6172 616e 6765 2830  0] = np.arange(0
+0000c8a0: 2c20 6e70 7473 2920 2f20 6e70 7473 0a20  , npts) / npts. 
+0000c8b0: 2020 2020 2020 2051 2c20 5220 3d20 6e70         Q, R = np
+0000c8c0: 2e6c 696e 616c 672e 7172 2858 290a 2020  .linalg.qr(X).  
+0000c8d0: 2020 2020 2020 7271 203d 206e 702e 646f        rq = np.do
+0000c8e0: 7428 6e70 2e6c 696e 616c 672e 696e 7628  t(np.linalg.inv(
+0000c8f0: 5229 2c20 512e 7472 616e 7370 6f73 6528  R), Q.transpose(
+0000c900: 2929 0a20 2020 2020 2020 2063 6f65 6666  )).        coeff
+0000c910: 203d 206e 702e 646f 7428 7271 2c20 6461   = np.dot(rq, da
+0000c920: 7461 290a 2020 2020 2020 2020 6461 7461  ta).        data
+0000c930: 203d 2064 6174 6120 2d20 6e70 2e64 6f74   = data - np.dot
+0000c940: 2858 2c20 636f 6566 6629 0a20 2020 2065  (X, coeff).    e
+0000c950: 6c69 6620 6461 7461 2e6e 6469 6d20 3d3d  lif data.ndim ==
+0000c960: 2032 3a0a 2020 2020 2020 2020 6e70 7473   2:.        npts
+0000c970: 203d 2064 6174 612e 7368 6170 655b 315d   = data.shape[1]
+0000c980: 0a20 2020 2020 2020 2058 203d 206e 702e  .        X = np.
+0000c990: 6f6e 6573 2828 6e70 7473 2c20 3229 290a  ones((npts, 2)).
+0000c9a0: 2020 2020 2020 2020 585b 3a2c 2030 5d20          X[:, 0] 
+0000c9b0: 3d20 6e70 2e61 7261 6e67 6528 302c 206e  = np.arange(0, n
+0000c9c0: 7074 7329 202f 206e 7074 730a 2020 2020  pts) / npts.    
+0000c9d0: 2020 2020 512c 2052 203d 206e 702e 6c69      Q, R = np.li
+0000c9e0: 6e61 6c67 2e71 7228 5829 0a20 2020 2020  nalg.qr(X).     
+0000c9f0: 2020 2072 7120 3d20 6e70 2e64 6f74 286e     rq = np.dot(n
+0000ca00: 702e 6c69 6e61 6c67 2e69 6e76 2852 292c  p.linalg.inv(R),
+0000ca10: 2051 2e74 7261 6e73 706f 7365 2829 290a   Q.transpose()).
+0000ca20: 2020 2020 2020 2020 666f 7220 6969 2069          for ii i
+0000ca30: 6e20 7261 6e67 6528 6461 7461 2e73 6861  n range(data.sha
+0000ca40: 7065 5b30 5d29 3a0a 2020 2020 2020 2020  pe[0]):.        
+0000ca50: 2020 2020 636f 6566 6620 3d20 6e70 2e64      coeff = np.d
+0000ca60: 6f74 2872 712c 2064 6174 615b 6969 5d29  ot(rq, data[ii])
+0000ca70: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+0000ca80: 615b 6969 5d20 3d20 6461 7461 5b69 695d  a[ii] = data[ii]
+0000ca90: 202d 206e 702e 646f 7428 582c 2063 6f65   - np.dot(X, coe
+0000caa0: 6666 290a 2020 2020 7265 7475 726e 2064  ff).    return d
+0000cab0: 6174 610a 0a0a 6465 6620 6465 6d65 616e  ata...def demean
+0000cac0: 2864 6174 6129 3a0a 2020 2020 2222 220a  (data):.    """.
+0000cad0: 2020 2020 7468 6973 2066 756e 6374 696f      this functio
+0000cae0: 6e20 7265 6d6f 7665 2074 6865 206d 6561  n remove the mea
+0000caf0: 6e20 6f66 2074 6865 2073 6967 6e61 6c0a  n of the signal.
+0000cb00: 2020 2020 5041 5241 4d45 5445 5253 3a0a      PARAMETERS:.
+0000cb10: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+0000cb20: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6461  ---------.    da
+0000cb30: 7461 3a20 696e 7075 7420 6461 7461 206d  ta: input data m
+0000cb40: 6174 7269 780a 2020 2020 5245 5455 524e  atrix.    RETURN
+0000cb50: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
+0000cb60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+0000cb70: 2064 6174 613a 2064 6174 6120 6d61 7472   data: data matr
+0000cb80: 6978 2077 6974 6820 6d65 616e 2072 656d  ix with mean rem
+0000cb90: 6f76 6564 0a20 2020 2022 2222 0a20 2020  oved.    """.   
+0000cba0: 2023 206e 6461 7461 203d 206e 702e 7a65   # ndata = np.ze
+0000cbb0: 726f 7328 7368 6170 653d 6461 7461 2e73  ros(shape=data.s
+0000cbc0: 6861 7065 2c64 7479 7065 3d64 6174 612e  hape,dtype=data.
+0000cbd0: 6474 7970 6529 0a20 2020 2069 6620 6461  dtype).    if da
+0000cbe0: 7461 2e6e 6469 6d20 3d3d 2031 3a0a 2020  ta.ndim == 1:.  
+0000cbf0: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+0000cc00: 6120 2d20 6e70 2e6d 6561 6e28 6461 7461  a - np.mean(data
+0000cc10: 290a 2020 2020 656c 6966 2064 6174 612e  ).    elif data.
+0000cc20: 6e64 696d 203d 3d20 323a 0a20 2020 2020  ndim == 2:.     
+0000cc30: 2020 2066 6f72 2069 6920 696e 2072 616e     for ii in ran
+0000cc40: 6765 2864 6174 612e 7368 6170 655b 305d  ge(data.shape[0]
+0000cc50: 293a 0a20 2020 2020 2020 2020 2020 2064  ):.            d
+0000cc60: 6174 615b 6969 5d20 3d20 6461 7461 5b69  ata[ii] = data[i
+0000cc70: 695d 202d 206e 702e 6d65 616e 2864 6174  i] - np.mean(dat
+0000cc80: 615b 6969 5d29 0a20 2020 2072 6574 7572  a[ii]).    retur
+0000cc90: 6e20 6461 7461 0a0a 0a64 6566 2074 6170  n data...def tap
+0000cca0: 6572 2864 6174 6129 3a0a 2020 2020 2222  er(data):.    ""
+0000ccb0: 220a 2020 2020 7468 6973 2066 756e 6374  ".    this funct
+0000ccc0: 696f 6e20 6170 706c 6965 7320 6120 636f  ion applies a co
+0000ccd0: 7369 6e65 2074 6170 6572 2075 7369 6e67  sine taper using
+0000cce0: 206f 6273 7079 2066 756e 6374 696f 6e73   obspy functions
+0000ccf0: 0a20 2020 2050 4152 414d 4554 4552 533a  .    PARAMETERS:
+0000cd00: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
+0000cd10: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064  ----------.    d
+0000cd20: 6174 613a 2069 6e70 7574 2064 6174 6120  ata: input data 
+0000cd30: 6d61 7472 6978 0a20 2020 2052 4554 5552  matrix.    RETUR
+0000cd40: 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  NS:.    --------
+0000cd50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+0000cd60: 2020 6461 7461 3a20 6461 7461 206d 6174    data: data mat
+0000cd70: 7269 7820 7769 7468 2074 6170 6572 2061  rix with taper a
+0000cd80: 7070 6c69 6564 0a20 2020 2022 2222 0a20  pplied.    """. 
+0000cd90: 2020 2023 206e 6461 7461 203d 206e 702e     # ndata = np.
+0000cda0: 7a65 726f 7328 7368 6170 653d 6461 7461  zeros(shape=data
+0000cdb0: 2e73 6861 7065 2c64 7479 7065 3d64 6174  .shape,dtype=dat
+0000cdc0: 612e 6474 7970 6529 0a20 2020 2069 6620  a.dtype).    if 
+0000cdd0: 6461 7461 2e6e 6469 6d20 3d3d 2031 3a0a  data.ndim == 1:.
+0000cde0: 2020 2020 2020 2020 6e70 7473 203d 2064          npts = d
+0000cdf0: 6174 612e 7368 6170 655b 305d 0a20 2020  ata.shape[0].   
+0000ce00: 2020 2020 2023 2077 696e 646f 7720 6c65       # window le
+0000ce10: 6e67 7468 0a20 2020 2020 2020 2069 6620  ngth.        if 
+0000ce20: 6e70 7473 202a 2030 2e30 3520 3e20 3230  npts * 0.05 > 20
+0000ce30: 3a0a 2020 2020 2020 2020 2020 2020 776c  :.            wl
+0000ce40: 656e 203d 2032 300a 2020 2020 2020 2020  en = 20.        
+0000ce50: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000ce60: 2020 776c 656e 203d 206e 7074 7320 2a20    wlen = npts * 
+0000ce70: 302e 3035 0a20 2020 2020 2020 2023 2074  0.05.        # t
+0000ce80: 6170 6572 2076 616c 7565 730a 2020 2020  aper values.    
+0000ce90: 2020 2020 6675 6e63 203d 205f 6765 745f      func = _get_
+0000cea0: 6675 6e63 7469 6f6e 5f66 726f 6d5f 656e  function_from_en
+0000ceb0: 7472 795f 706f 696e 7428 2274 6170 6572  try_point("taper
+0000cec0: 222c 2022 6861 6e6e 2229 0a20 2020 2020  ", "hann").     
+0000ced0: 2020 2069 6620 3220 2a20 776c 656e 203d     if 2 * wlen =
+0000cee0: 3d20 6e70 7473 3a0a 2020 2020 2020 2020  = npts:.        
+0000cef0: 2020 2020 7461 7065 725f 7369 6465 7320      taper_sides 
+0000cf00: 3d20 6675 6e63 2832 202a 2077 6c65 6e29  = func(2 * wlen)
+0000cf10: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0000cf20: 2020 2020 2020 2020 2020 2074 6170 6572             taper
+0000cf30: 5f73 6964 6573 203d 2066 756e 6328 3220  _sides = func(2 
+0000cf40: 2a20 776c 656e 202b 2031 290a 2020 2020  * wlen + 1).    
+0000cf50: 2020 2020 2320 7461 7065 7220 7769 6e64      # taper wind
+0000cf60: 6f77 0a20 2020 2020 2020 2077 696e 203d  ow.        win =
+0000cf70: 206e 702e 6873 7461 636b 280a 2020 2020   np.hstack(.    
+0000cf80: 2020 2020 2020 2020 280a 2020 2020 2020          (.      
+0000cf90: 2020 2020 2020 2020 2020 7461 7065 725f            taper_
+0000cfa0: 7369 6465 735b 3a77 6c65 6e5d 2c0a 2020  sides[:wlen],.  
+0000cfb0: 2020 2020 2020 2020 2020 2020 2020 6e70                np
+0000cfc0: 2e6f 6e65 7328 6e70 7473 202d 2032 202a  .ones(npts - 2 *
+0000cfd0: 2077 6c65 6e29 2c0a 2020 2020 2020 2020   wlen),.        
+0000cfe0: 2020 2020 2020 2020 7461 7065 725f 7369          taper_si
+0000cff0: 6465 735b 6c65 6e28 7461 7065 725f 7369  des[len(taper_si
+0000d000: 6465 7329 202d 2077 6c65 6e20 3a5d 2c0a  des) - wlen :],.
+0000d010: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000d020: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000d030: 6461 7461 202a 3d20 7769 6e0a 2020 2020  data *= win.    
+0000d040: 656c 6966 2064 6174 612e 6e64 696d 203d  elif data.ndim =
+0000d050: 3d20 323a 0a20 2020 2020 2020 206e 7074  = 2:.        npt
+0000d060: 7320 3d20 6461 7461 2e73 6861 7065 5b31  s = data.shape[1
+0000d070: 5d0a 2020 2020 2020 2020 2320 7769 6e64  ].        # wind
+0000d080: 6f77 206c 656e 6774 680a 2020 2020 2020  ow length.      
+0000d090: 2020 6966 206e 7074 7320 2a20 302e 3035    if npts * 0.05
+0000d0a0: 203e 2032 303a 0a20 2020 2020 2020 2020   > 20:.         
+0000d0b0: 2020 2077 6c65 6e20 3d20 3230 0a20 2020     wlen = 20.   
+0000d0c0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000d0d0: 2020 2020 2020 2077 6c65 6e20 3d20 6e70         wlen = np
+0000d0e0: 7473 202a 2030 2e30 350a 2020 2020 2020  ts * 0.05.      
+0000d0f0: 2020 2320 7461 7065 7220 7661 6c75 6573    # taper values
+0000d100: 0a20 2020 2020 2020 2066 756e 6320 3d20  .        func = 
+0000d110: 5f67 6574 5f66 756e 6374 696f 6e5f 6672  _get_function_fr
+0000d120: 6f6d 5f65 6e74 7279 5f70 6f69 6e74 2822  om_entry_point("
+0000d130: 7461 7065 7222 2c20 2268 616e 6e22 290a  taper", "hann").
+0000d140: 2020 2020 2020 2020 6966 2032 202a 2077          if 2 * w
+0000d150: 6c65 6e20 3d3d 206e 7074 733a 0a20 2020  len == npts:.   
+0000d160: 2020 2020 2020 2020 2074 6170 6572 5f73           taper_s
+0000d170: 6964 6573 203d 2066 756e 6328 3220 2a20  ides = func(2 * 
+0000d180: 776c 656e 290a 2020 2020 2020 2020 656c  wlen).        el
+0000d190: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000d1a0: 7461 7065 725f 7369 6465 7320 3d20 6675  taper_sides = fu
+0000d1b0: 6e63 2832 202a 2077 6c65 6e20 2b20 3129  nc(2 * wlen + 1)
+0000d1c0: 0a20 2020 2020 2020 2023 2074 6170 6572  .        # taper
+0000d1d0: 2077 696e 646f 770a 2020 2020 2020 2020   window.        
+0000d1e0: 7769 6e20 3d20 6e70 2e68 7374 6163 6b28  win = np.hstack(
+0000d1f0: 0a20 2020 2020 2020 2020 2020 2028 0a20  .            (. 
+0000d200: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000d210: 6170 6572 5f73 6964 6573 5b3a 776c 656e  aper_sides[:wlen
+0000d220: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+0000d230: 2020 206e 702e 6f6e 6573 286e 7074 7320     np.ones(npts 
+0000d240: 2d20 3220 2a20 776c 656e 292c 0a20 2020  - 2 * wlen),.   
+0000d250: 2020 2020 2020 2020 2020 2020 2074 6170               tap
+0000d260: 6572 5f73 6964 6573 5b6c 656e 2874 6170  er_sides[len(tap
+0000d270: 6572 5f73 6964 6573 2920 2d20 776c 656e  er_sides) - wlen
+0000d280: 203a 5d2c 0a20 2020 2020 2020 2020 2020   :],.           
+0000d290: 2029 0a20 2020 2020 2020 2029 0a20 2020   ).        ).   
+0000d2a0: 2020 2020 2066 6f72 2069 6920 696e 2072       for ii in r
+0000d2b0: 616e 6765 2864 6174 612e 7368 6170 655b  ange(data.shape[
+0000d2c0: 305d 293a 0a20 2020 2020 2020 2020 2020  0]):.           
+0000d2d0: 2064 6174 615b 6969 5d20 2a3d 2077 696e   data[ii] *= win
+0000d2e0: 0a20 2020 2072 6574 7572 6e20 6461 7461  .    return data
+0000d2f0: 0a0a 0a23 2040 6a69 7428 6e6f 7079 7468  ...# @jit(nopyth
+0000d300: 6f6e 203d 2054 7275 6529 0a0a 0a23 2063  on = True)...# c
+0000d310: 6861 6e67 6520 7468 6520 6d6f 7669 6e67  hange the moving
+0000d320: 2061 7665 7261 6765 2063 616c 6375 6c61   average calcula
+0000d330: 7469 6f6e 2074 6f20 7461 6b65 2061 7320  tion to take as 
+0000d340: 696e 7075 7420 4e20 7468 6520 6675 6c6c  input N the full
+0000d350: 2077 696e 646f 7720 6c65 6e67 7468 2074   window length t
+0000d360: 6f20 736d 6f6f 7468 0a64 6566 206d 6f76  o smooth.def mov
+0000d370: 696e 675f 6176 6528 412c 204e 293a 0a20  ing_ave(A, N):. 
+0000d380: 2020 2022 2222 0a20 2020 2041 6c74 6572     """.    Alter
+0000d390: 6e61 7469 7665 2066 756e 6374 696f 6e20  native function 
+0000d3a0: 666f 7220 6d6f 7669 6e67 2061 7665 7261  for moving avera
+0000d3b0: 6765 2066 6f72 2061 6e20 6172 7261 792e  ge for an array.
+0000d3c0: 0a20 2020 2050 4152 414d 4554 4552 533a  .    PARAMETERS:
+0000d3d0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
+0000d3e0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2041  ----------.    A
+0000d3f0: 3a20 312d 4420 6172 7261 7920 6f66 2064  : 1-D array of d
+0000d400: 6174 6120 746f 2062 6520 736d 6f6f 7468  ata to be smooth
+0000d410: 6564 0a20 2020 204e 3a20 696e 7465 6765  ed.    N: intege
+0000d420: 722c 2069 7420 6465 6669 6e65 7320 7468  r, it defines th
+0000d430: 6520 6675 6c6c 2121 2077 696e 646f 7720  e full!! window 
+0000d440: 6c65 6e67 7468 2074 6f20 736d 6f6f 7468  length to smooth
+0000d450: 0a20 2020 2052 4554 5552 4e53 3a0a 2020  .    RETURNS:.  
+0000d460: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+0000d470: 2d2d 2d2d 2d2d 2d0a 2020 2020 423a 2031  -------.    B: 1
+0000d480: 2d44 2061 7272 6179 2077 6974 6820 736d  -D array with sm
+0000d490: 6f6f 7468 6564 2064 6174 610a 2020 2020  oothed data.    
+0000d4a0: 2222 220a 2020 2020 2320 6465 6669 6e65  """.    # define
+0000d4b0: 7320 616e 2061 7272 6179 2077 6974 6820  s an array with 
+0000d4c0: 4e20 6578 7472 6120 7361 6d70 6c65 7320  N extra samples 
+0000d4d0: 6174 2065 6974 6865 7220 7369 6465 0a20  at either side. 
+0000d4e0: 2020 2074 656d 7020 3d20 6e70 2e7a 6572     temp = np.zer
+0000d4f0: 6f73 286c 656e 2841 2920 2b20 3220 2a20  os(len(A) + 2 * 
+0000d500: 4e29 0a20 2020 2023 2073 6574 2074 6865  N).    # set the
+0000d510: 2063 656e 7472 616c 2070 6f72 7469 6f6e   central portion
+0000d520: 206f 6620 7468 6520 6172 7261 7920 746f   of the array to
+0000d530: 2041 0a20 2020 2074 656d 705b 4e3a 2d4e   A.    temp[N:-N
+0000d540: 5d20 3d20 410a 2020 2020 2320 6c65 6164  ] = A.    # lead
+0000d550: 696e 6720 7361 6d70 6c65 733a 2065 7175  ing samples: equ
+0000d560: 616c 2074 6f20 6669 7273 7420 7361 6d70  al to first samp
+0000d570: 6c65 206f 6620 6163 7475 616c 2061 7272  le of actual arr
+0000d580: 6179 0a20 2020 2074 656d 705b 303a 4e5d  ay.    temp[0:N]
+0000d590: 203d 2074 656d 705b 4e5d 0a20 2020 2023   = temp[N].    #
+0000d5a0: 2074 7261 696c 696e 6720 7361 6d70 6c65   trailing sample
+0000d5b0: 733a 2045 7175 616c 2074 6f20 6c61 7374  s: Equal to last
+0000d5c0: 2073 616d 706c 6520 6f66 2061 6374 7561   sample of actua
+0000d5d0: 6c20 6172 7261 790a 2020 2020 7465 6d70  l array.    temp
+0000d5e0: 5b2d 4e3a 5d20 3d20 7465 6d70 5b2d 4e20  [-N:] = temp[-N 
+0000d5f0: 2d20 315d 0a20 2020 2023 2063 6f6e 766f  - 1].    # convo
+0000d600: 6c76 6520 7769 7468 2061 2062 6f78 6361  lve with a boxca
+0000d610: 7220 616e 6420 6e6f 726d 616c 697a 652c  r and normalize,
+0000d620: 2061 6e64 2075 7365 206f 6e6c 7920 6365   and use only ce
+0000d630: 6e74 7261 6c20 706f 7274 696f 6e20 6f66  ntral portion of
+0000d640: 2074 6865 2072 6573 756c 740a 2020 2020   the result.    
+0000d650: 2320 7769 7468 206c 656e 6774 6820 6571  # with length eq
+0000d660: 7561 6c20 746f 2074 6865 206f 7269 6769  ual to the origi
+0000d670: 6e61 6c20 6172 7261 792c 2064 6973 6361  nal array, disca
+0000d680: 7264 696e 6720 7468 6520 6164 6465 6420  rding the added 
+0000d690: 6c65 6164 696e 6720 616e 6420 7472 6169  leading and trai
+0000d6a0: 6c69 6e67 2073 616d 706c 6573 0a20 2020  ling samples.   
+0000d6b0: 2042 203d 206e 702e 636f 6e76 6f6c 7665   B = np.convolve
+0000d6c0: 2874 656d 702c 206e 702e 6f6e 6573 284e  (temp, np.ones(N
+0000d6d0: 2920 2f20 4e2c 206d 6f64 653d 2273 616d  ) / N, mode="sam
+0000d6e0: 6522 295b 4e3a 2d4e 5d0a 2020 2020 7265  e")[N:-N].    re
+0000d6f0: 7475 726e 2042 0a0a 0a23 2063 6861 6e67  turn B...# chang
+0000d700: 6520 7468 6520 6d6f 7669 6e67 2061 7665  e the moving ave
+0000d710: 7261 6765 2063 616c 6375 6c61 7469 6f6e  rage calculation
+0000d720: 2074 6f20 7461 6b65 2061 7320 696e 7075   to take as inpu
+0000d730: 7420 4e20 7468 6520 6675 6c6c 2077 696e  t N the full win
+0000d740: 646f 7720 6c65 6e67 7468 2074 6f20 736d  dow length to sm
+0000d750: 6f6f 7468 0a64 6566 206d 6f76 696e 675f  ooth.def moving_
+0000d760: 6176 655f 3244 2841 2c20 4e29 3a0a 2020  ave_2D(A, N):.  
+0000d770: 2020 2222 220a 2020 2020 416c 7465 726e    """.    Altern
+0000d780: 6174 6976 6520 6675 6e63 7469 6f6e 2066  ative function f
+0000d790: 6f72 206d 6f76 696e 6720 6176 6572 6167  or moving averag
+0000d7a0: 6520 666f 7220 616e 2061 7272 6179 2e0a  e for an array..
+0000d7b0: 2020 2020 5041 5241 4d45 5445 5253 3a0a      PARAMETERS:.
+0000d7c0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+0000d7d0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 413a  ---------.    A:
+0000d7e0: 2032 2d44 2061 7272 6179 206f 6620 6461   2-D array of da
+0000d7f0: 7461 2074 6f20 6265 2073 6d6f 6f74 6865  ta to be smoothe
+0000d800: 640a 2020 2020 4e3a 2069 6e74 6567 6572  d.    N: integer
+0000d810: 2c20 6974 2064 6566 696e 6573 2074 6865  , it defines the
+0000d820: 2066 756c 6c21 2120 7769 6e64 6f77 206c   full!! window l
+0000d830: 656e 6774 6820 746f 2073 6d6f 6f74 680a  ength to smooth.
+0000d840: 2020 2020 5245 5455 524e 533a 0a20 2020      RETURNS:.   
+0000d850: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+0000d860: 2d2d 2d2d 2d2d 0a20 2020 2042 3a20 322d  ------.    B: 2-
+0000d870: 4420 6172 7261 7920 7769 7468 2073 6d6f  D array with smo
+0000d880: 6f74 6865 6420 6461 7461 0a20 2020 2022  othed data.    "
+0000d890: 2222 0a20 2020 206e 7463 2c20 6e73 7074  "".    ntc, nspt
+0000d8a0: 203d 2041 2e73 6861 7065 0a20 2020 2023   = A.shape.    #
+0000d8b0: 2064 6566 696e 6573 2061 6e20 6172 7261   defines an arra
+0000d8c0: 7920 7769 7468 204e 2065 7874 7261 2073  y with N extra s
+0000d8d0: 616d 706c 6573 2061 7420 6569 7468 6572  amples at either
+0000d8e0: 2073 6964 650a 2020 2020 7465 6d70 203d   side.    temp =
+0000d8f0: 206e 702e 7a65 726f 7328 5b6e 7463 2c20   np.zeros([ntc, 
+0000d900: 6e73 7074 202b 2032 202a 204e 5d29 0a20  nspt + 2 * N]). 
+0000d910: 2020 2023 2073 6574 2074 6865 2063 656e     # set the cen
+0000d920: 7472 616c 2070 6f72 7469 6f6e 206f 6620  tral portion of 
+0000d930: 7468 6520 6172 7261 7920 746f 2041 0a20  the array to A. 
+0000d940: 2020 2074 656d 705b 3a2c 204e 3a2d 4e5d     temp[:, N:-N]
+0000d950: 203d 2041 0a20 2020 2023 206c 6561 6469   = A.    # leadi
+0000d960: 6e67 2073 616d 706c 6573 3a20 6571 7561  ng samples: equa
+0000d970: 6c20 746f 2066 6972 7374 2073 616d 706c  l to first sampl
+0000d980: 6520 6f66 2061 6374 7561 6c20 6172 7261  e of actual arra
+0000d990: 790a 2020 2020 7465 6d70 5b3a 2c20 303a  y.    temp[:, 0:
+0000d9a0: 4e5d 203d 206e 702e 7265 7065 6174 286e  N] = np.repeat(n
+0000d9b0: 702e 6578 7061 6e64 5f64 696d 7328 7465  p.expand_dims(te
+0000d9c0: 6d70 5b3a 2c20 4e5d 2c20 6178 6973 3d2d  mp[:, N], axis=-
+0000d9d0: 3129 2c20 4e2c 2061 7869 733d 2d31 290a  1), N, axis=-1).
+0000d9e0: 2020 2020 2320 7472 6169 6c69 6e67 2073      # trailing s
+0000d9f0: 616d 706c 6573 3a20 4571 7561 6c20 746f  amples: Equal to
+0000da00: 206c 6173 7420 7361 6d70 6c65 206f 6620   last sample of 
+0000da10: 6163 7475 616c 2061 7272 6179 0a20 2020  actual array.   
+0000da20: 2074 656d 705b 3a2c 202d 4e3a 5d20 3d20   temp[:, -N:] = 
+0000da30: 6e70 2e72 6570 6561 7428 6e70 2e65 7870  np.repeat(np.exp
+0000da40: 616e 645f 6469 6d73 2874 656d 705b 3a2c  and_dims(temp[:,
+0000da50: 202d 4e20 2d20 315d 2c20 6178 6973 3d2d   -N - 1], axis=-
+0000da60: 3129 2c20 4e2c 2061 7869 733d 2d31 290a  1), N, axis=-1).
+0000da70: 2020 2020 2320 636f 6e76 6f6c 7665 2077      # convolve w
+0000da80: 6974 6820 6120 626f 7863 6172 2061 6e64  ith a boxcar and
+0000da90: 206e 6f72 6d61 6c69 7a65 2c20 616e 6420   normalize, and 
+0000daa0: 7573 6520 6f6e 6c79 2063 656e 7472 616c  use only central
+0000dab0: 2070 6f72 7469 6f6e 206f 6620 7468 6520   portion of the 
+0000dac0: 7265 7375 6c74 0a20 2020 2023 2077 6974  result.    # wit
+0000dad0: 6820 6c65 6e67 7468 2065 7175 616c 2074  h length equal t
+0000dae0: 6f20 7468 6520 6f72 6967 696e 616c 2061  o the original a
+0000daf0: 7272 6179 2c20 6469 7363 6172 6469 6e67  rray, discarding
+0000db00: 2074 6865 2061 6464 6564 206c 6561 6469   the added leadi
+0000db10: 6e67 2061 6e64 2074 7261 696c 696e 6720  ng and trailing 
+0000db20: 7361 6d70 6c65 730a 2020 2020 4220 3d20  samples.    B = 
+0000db30: 7363 6970 792e 7369 676e 616c 2e63 6f6e  scipy.signal.con
+0000db40: 766f 6c76 6532 6428 7465 6d70 2c20 6e70  volve2d(temp, np
+0000db50: 2e65 7870 616e 645f 6469 6d73 286e 702e  .expand_dims(np.
+0000db60: 6f6e 6573 284e 2920 2f20 4e2c 2061 7869  ones(N) / N, axi
+0000db70: 733d 3029 2c20 6d6f 6465 3d22 7361 6d65  s=0), mode="same
+0000db80: 2229 5b3a 2c20 4e3a 2d4e 5d0a 2020 2020  ")[:, N:-N].    
+0000db90: 7265 7475 726e 2042 0a0a 0a64 6566 2072  return B...def r
+0000dba0: 6f62 7573 745f 7374 6163 6b28 6363 5f61  obust_stack(cc_a
+0000dbb0: 7272 6179 2c20 6570 7369 6c6f 6e29 3a0a  rray, epsilon):.
+0000dbc0: 2020 2020 2222 220a 2020 2020 7468 6973      """.    this
+0000dbd0: 2069 7320 6120 726f 6275 7374 2073 7461   is a robust sta
+0000dbe0: 636b 696e 6720 616c 676f 7269 7468 6d20  cking algorithm 
+0000dbf0: 6465 7363 7269 6265 6420 696e 2050 616c  described in Pal
+0000dc00: 7669 7320 616e 6420 5665 726e 6f6e 2032  vis and Vernon 2
+0000dc10: 3031 300a 0a20 2020 2050 4152 414d 4554  010..    PARAMET
+0000dc20: 4552 533a 0a20 2020 202d 2d2d 2d2d 2d2d  ERS:.    -------
+0000dc30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+0000dc40: 2020 2020 6363 5f61 7272 6179 3a20 6e75      cc_array: nu
+0000dc50: 6d70 792e 6e64 6172 7261 7920 636f 6e74  mpy.ndarray cont
+0000dc60: 6169 6e73 2074 6865 2032 4420 6372 6f73  ains the 2D cros
+0000dc70: 7320 636f 7272 656c 6174 696f 6e20 6d61  s correlation ma
+0000dc80: 7472 6978 0a20 2020 2065 7073 696c 6f6e  trix.    epsilon
+0000dc90: 3a20 7265 7369 6475 616c 2074 6872 6568  : residual threh
+0000dca0: 6f6c 6420 746f 2071 7569 7420 7468 6520  old to quit the 
+0000dcb0: 6974 6572 6174 696f 6e0a 2020 2020 5245  iteration.    RE
+0000dcc0: 5455 524e 533a 0a20 2020 202d 2d2d 2d2d  TURNS:.    -----
+0000dcd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000dce0: 2d0a 2020 2020 6e65 7773 7461 636b 3a20  -.    newstack: 
+0000dcf0: 6e75 6d70 7920 7665 6374 6f72 2063 6f6e  numpy vector con
+0000dd00: 7461 696e 7320 7468 6520 7374 6163 6b65  tains the stacke
+0000dd10: 6420 6372 6f73 7320 636f 7272 656c 6174  d cross correlat
+0000dd20: 696f 6e0a 0a20 2020 2057 7269 7474 656e  ion..    Written
+0000dd30: 2062 7920 4d61 7269 6e65 2044 656e 6f6c   by Marine Denol
+0000dd40: 6c65 0a20 2020 2022 2222 0a20 2020 2072  le.    """.    r
+0000dd50: 6573 203d 2039 6539 2020 2320 7265 7369  es = 9e9  # resi
+0000dd60: 6475 616c 730a 2020 2020 7720 3d20 6e70  duals.    w = np
+0000dd70: 2e6f 6e65 7328 6363 5f61 7272 6179 2e73  .ones(cc_array.s
+0000dd80: 6861 7065 5b30 5d29 0a20 2020 206e 7374  hape[0]).    nst
+0000dd90: 6570 203d 2030 0a20 2020 206e 6577 7374  ep = 0.    newst
+0000dda0: 6163 6b20 3d20 6e70 2e6d 6564 6961 6e28  ack = np.median(
+0000ddb0: 6363 5f61 7272 6179 2c20 6178 6973 3d30  cc_array, axis=0
+0000ddc0: 290a 2020 2020 7768 696c 6520 7265 7320  ).    while res 
+0000ddd0: 3e20 6570 7369 6c6f 6e3a 0a20 2020 2020  > epsilon:.     
+0000dde0: 2020 2073 7461 636b 203d 206e 6577 7374     stack = newst
+0000ddf0: 6163 6b0a 2020 2020 2020 2020 666f 7220  ack.        for 
+0000de00: 6920 696e 2072 616e 6765 2863 635f 6172  i in range(cc_ar
+0000de10: 7261 792e 7368 6170 655b 305d 293a 0a20  ray.shape[0]):. 
+0000de20: 2020 2020 2020 2020 2020 2063 7261 7020             crap 
+0000de30: 3d20 6e70 2e6d 756c 7469 706c 7928 7374  = np.multiply(st
+0000de40: 6163 6b2c 2063 635f 6172 7261 795b 692c  ack, cc_array[i,
+0000de50: 203a 5d2e 5429 0a20 2020 2020 2020 2020   :].T).         
+0000de60: 2020 2063 7261 705f 646f 7420 3d20 6e70     crap_dot = np
+0000de70: 2e73 756d 2863 7261 7029 0a20 2020 2020  .sum(crap).     
+0000de80: 2020 2020 2020 2064 695f 6e6f 726d 203d         di_norm =
+0000de90: 206e 702e 6c69 6e61 6c67 2e6e 6f72 6d28   np.linalg.norm(
+0000dea0: 6363 5f61 7272 6179 5b69 2c20 3a5d 290a  cc_array[i, :]).
+0000deb0: 2020 2020 2020 2020 2020 2020 7269 203d              ri =
+0000dec0: 2063 635f 6172 7261 795b 692c 203a 5d20   cc_array[i, :] 
+0000ded0: 2d20 6372 6170 5f64 6f74 202a 2073 7461  - crap_dot * sta
+0000dee0: 636b 0a20 2020 2020 2020 2020 2020 2072  ck.            r
+0000def0: 695f 6e6f 726d 203d 206e 702e 6c69 6e61  i_norm = np.lina
+0000df00: 6c67 2e6e 6f72 6d28 7269 290a 2020 2020  lg.norm(ri).    
+0000df10: 2020 2020 2020 2020 775b 695d 203d 206e          w[i] = n
+0000df20: 702e 6162 7328 6372 6170 5f64 6f74 2920  p.abs(crap_dot) 
+0000df30: 2f20 6469 5f6e 6f72 6d20 2f20 7269 5f6e  / di_norm / ri_n
+0000df40: 6f72 6d20 2023 202f 6c65 6e28 6363 5f61  orm  # /len(cc_a
+0000df50: 7272 6179 5b3a 2c31 5d29 0a20 2020 2020  rray[:,1]).     
+0000df60: 2020 2023 2070 7269 6e74 2877 290a 2020     # print(w).  
+0000df70: 2020 2020 2020 7720 3d20 7720 2f20 6e70        w = w / np
+0000df80: 2e73 756d 2877 290a 2020 2020 2020 2020  .sum(w).        
+0000df90: 6e65 7773 7461 636b 203d 206e 702e 7375  newstack = np.su
+0000dfa0: 6d28 2877 202a 2063 635f 6172 7261 792e  m((w * cc_array.
+0000dfb0: 5429 2e54 2c20 6178 6973 3d30 2920 2023  T).T, axis=0)  #
+0000dfc0: 202f 6c65 6e28 6363 5f61 7272 6179 5b3a   /len(cc_array[:
+0000dfd0: 2c31 5d29 0a20 2020 2020 2020 2072 6573  ,1]).        res
+0000dfe0: 203d 206e 702e 6c69 6e61 6c67 2e6e 6f72   = np.linalg.nor
+0000dff0: 6d28 6e65 7773 7461 636b 202d 2073 7461  m(newstack - sta
+0000e000: 636b 2c20 6f72 643d 3129 202f 206e 702e  ck, ord=1) / np.
+0000e010: 6c69 6e61 6c67 2e6e 6f72 6d28 6e65 7773  linalg.norm(news
+0000e020: 7461 636b 2920 2f20 6c65 6e28 6363 5f61  tack) / len(cc_a
+0000e030: 7272 6179 5b3a 2c20 315d 290a 2020 2020  rray[:, 1]).    
+0000e040: 2020 2020 6e73 7465 7020 2b3d 2031 0a20      nstep += 1. 
+0000e050: 2020 2020 2020 2069 6620 6e73 7465 7020         if nstep 
+0000e060: 3e20 3130 3a0a 2020 2020 2020 2020 2020  > 10:.          
+0000e070: 2020 7265 7475 726e 206e 6577 7374 6163    return newstac
+0000e080: 6b2c 2077 2c20 6e73 7465 700a 2020 2020  k, w, nstep.    
+0000e090: 7265 7475 726e 206e 6577 7374 6163 6b2c  return newstack,
+0000e0a0: 2077 2c20 6e73 7465 700a 0a0a 6465 6620   w, nstep...def 
+0000e0b0: 7365 6c65 6374 6976 655f 7374 6163 6b28  selective_stack(
+0000e0c0: 6363 5f61 7272 6179 2c20 6570 7369 6c6f  cc_array, epsilo
+0000e0d0: 6e29 3a0a 2020 2020 2222 220a 2020 2020  n):.    """.    
+0000e0e0: 7468 6973 2069 7320 6120 7365 6c65 6374  this is a select
+0000e0f0: 6976 6520 7374 6163 6b69 6e67 2061 6c67  ive stacking alg
+0000e100: 6f72 6974 686d 2064 6576 656c 6f70 6564  orithm developed
+0000e110: 2062 7920 4a61 7265 6420 4272 7961 6e2e   by Jared Bryan.
+0000e120: 0a0a 2020 2020 5041 5241 4d45 5445 5253  ..    PARAMETERS
+0000e130: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  :.    ----------
+0000e140: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+0000e150: 2063 635f 6172 7261 793a 206e 756d 7079   cc_array: numpy
+0000e160: 2e6e 6461 7272 6179 2063 6f6e 7461 696e  .ndarray contain
+0000e170: 7320 7468 6520 3244 2063 726f 7373 2063  s the 2D cross c
+0000e180: 6f72 7265 6c61 7469 6f6e 206d 6174 7269  orrelation matri
+0000e190: 780a 2020 2020 6570 7369 6c6f 6e3a 2072  x.    epsilon: r
+0000e1a0: 6573 6964 7561 6c20 7468 7265 686f 6c64  esidual threhold
+0000e1b0: 2074 6f20 7175 6974 2074 6865 2069 7465   to quit the ite
+0000e1c0: 7261 7469 6f6e 0a20 2020 2052 4554 5552  ration.    RETUR
+0000e1d0: 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  NS:.    --------
+0000e1e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+0000e1f0: 2020 206e 6577 7374 6163 6b3a 206e 756d     newstack: num
+0000e200: 7079 2076 6563 746f 7220 636f 6e74 6169  py vector contai
+0000e210: 6e73 2074 6865 2073 7461 636b 6564 2063  ns the stacked c
+0000e220: 726f 7373 2063 6f72 7265 6c61 7469 6f6e  ross correlation
+0000e230: 0a0a 2020 2020 5772 6974 7465 6e20 6279  ..    Written by
+0000e240: 204d 6172 696e 6520 4465 6e6f 6c6c 650a   Marine Denolle.
+0000e250: 2020 2020 2222 220a 2020 2020 6363 203d      """.    cc =
+0000e260: 206e 702e 6f6e 6573 2863 635f 6172 7261   np.ones(cc_arra
+0000e270: 792e 7368 6170 655b 305d 290a 2020 2020  y.shape[0]).    
+0000e280: 6e65 7773 7461 636b 203d 206e 702e 6d65  newstack = np.me
+0000e290: 616e 2863 635f 6172 7261 792c 2061 7869  an(cc_array, axi
+0000e2a0: 733d 3029 0a20 2020 2066 6f72 2069 2069  s=0).    for i i
+0000e2b0: 6e20 7261 6e67 6528 6363 5f61 7272 6179  n range(cc_array
+0000e2c0: 2e73 6861 7065 5b30 5d29 3a0a 2020 2020  .shape[0]):.    
+0000e2d0: 2020 2020 6363 5b69 5d20 3d20 6e70 2e73      cc[i] = np.s
+0000e2e0: 756d 286e 702e 6d75 6c74 6970 6c79 286e  um(np.multiply(n
+0000e2f0: 6577 7374 6163 6b2c 2063 635f 6172 7261  ewstack, cc_arra
+0000e300: 795b 692c 203a 5d2e 5429 290a 2020 2020  y[i, :].T)).    
+0000e310: 696b 203d 206e 702e 7768 6572 6528 6363  ik = np.where(cc
+0000e320: 203e 3d20 6570 7369 6c6f 6e29 5b30 5d0a   >= epsilon)[0].
+0000e330: 2020 2020 6e65 7773 7461 636b 203d 206e      newstack = n
+0000e340: 702e 6d65 616e 2863 635f 6172 7261 795b  p.mean(cc_array[
+0000e350: 696b 2c20 3a5d 2c20 6178 6973 3d30 290a  ik, :], axis=0).
+0000e360: 0a20 2020 2072 6574 7572 6e20 6e65 7773  .    return news
+0000e370: 7461 636b 2c20 6363 0a0a 0a64 6566 2077  tack, cc...def w
+0000e380: 6869 7465 6e5f 3144 2874 696d 6573 6572  hiten_1D(timeser
+0000e390: 6965 732c 2066 6674 5f70 6172 613a 2043  ies, fft_para: C
+0000e3a0: 6f6e 6669 6750 6172 616d 6574 6572 732c  onfigParameters,
+0000e3b0: 206e 5f74 6170 6572 293a 0a20 2020 2022   n_taper):.    "
+0000e3c0: 2222 0a20 2020 2054 6869 7320 6675 6e63  "".    This func
+0000e3d0: 7469 6f6e 2074 616b 6573 2061 2031 2d64  tion takes a 1-d
+0000e3e0: 696d 656e 7369 6f6e 616c 2074 696d 6573  imensional times
+0000e3f0: 6572 6965 7320 6172 7261 792c 2074 7261  eries array, tra
+0000e400: 6e73 666f 726d 7320 746f 2066 7265 7175  nsforms to frequ
+0000e410: 656e 6379 2064 6f6d 6169 6e20 7573 696e  ency domain usin
+0000e420: 6720 6666 742c 0a20 2020 2077 6869 7465  g fft,.    white
+0000e430: 6e73 2074 6865 2061 6d70 6c69 7475 6465  ns the amplitude
+0000e440: 206f 6620 7468 6520 7370 6563 7472 756d   of the spectrum
+0000e450: 2069 6e20 6672 6571 7565 6e63 7920 646f   in frequency do
+0000e460: 6d61 696e 2062 6574 7765 656e 202a 6672  main between *fr
+0000e470: 6571 6d69 6e2a 2061 6e64 202a 6672 6571  eqmin* and *freq
+0000e480: 6d61 782a 0a20 2020 2061 6e64 2072 6574  max*.    and ret
+0000e490: 7572 6e73 2074 6865 2077 6869 7465 6e65  urns the whitene
+0000e4a0: 6420 6666 742e 0a20 2020 2050 4152 414d  d fft..    PARAM
+0000e4b0: 4554 4552 533a 0a20 2020 202d 2d2d 2d2d  ETERS:.    -----
+0000e4c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000e4d0: 2d0a 2020 2020 6461 7461 3a20 6e75 6d70  -.    data: nump
+0000e4e0: 792e 6e64 6172 7261 7920 636f 6e74 6169  y.ndarray contai
+0000e4f0: 6e73 2074 6865 2031 4420 7469 6d65 2073  ns the 1D time s
+0000e500: 6572 6965 7320 746f 2077 6869 7465 6e0a  eries to whiten.
+0000e510: 2020 2020 6666 745f 7061 7261 3a20 436f      fft_para: Co
+0000e520: 6e66 6967 5061 7261 6d65 7465 7273 2063  nfigParameters c
+0000e530: 6c61 7373 2063 6f6e 7461 696e 696e 6720  lass containing 
+0000e540: 616c 6c20 6666 745f 6363 2070 6172 616d  all fft_cc param
+0000e550: 6574 6572 7320 7375 6368 2061 730a 2020  eters such as.  
+0000e560: 2020 2020 2020 6474 3a20 5468 6520 7361        dt: The sa
+0000e570: 6d70 6c69 6e67 2073 7061 6365 206f 6620  mpling space of 
+0000e580: 7468 6520 6064 6174 6160 0a20 2020 2020  the `data`.     
+0000e590: 2020 2066 7265 716d 696e 3a20 5468 6520     freqmin: The 
+0000e5a0: 6c6f 7765 7220 6672 6571 7565 6e63 7920  lower frequency 
+0000e5b0: 626f 756e 640a 2020 2020 2020 2020 6672  bound.        fr
+0000e5c0: 6571 6d61 783a 2054 6865 2075 7070 6572  eqmax: The upper
+0000e5d0: 2066 7265 7175 656e 6379 2062 6f75 6e64   frequency bound
+0000e5e0: 0a20 2020 2020 2020 2073 6d6f 6f74 685f  .        smooth_
+0000e5f0: 4e3a 2069 6e74 6567 6572 2c20 6974 2064  N: integer, it d
+0000e600: 6566 696e 6573 2074 6865 2068 616c 6620  efines the half 
+0000e610: 7769 6e64 6f77 206c 656e 6774 6820 746f  window length to
+0000e620: 2073 6d6f 6f74 680a 2020 2020 2020 2020   smooth.        
+0000e630: 6e5f 7461 7065 722c 206f 7074 696f 6e61  n_taper, optiona
+0000e640: 6c3a 2069 6e74 6567 6572 2c20 6465 6669  l: integer, defi
+0000e650: 6e65 2074 6865 2077 6964 7468 206f 6620  ne the width of 
+0000e660: 7468 6520 7461 7065 7220 696e 2073 616d  the taper in sam
+0000e670: 706c 6573 0a20 2020 2052 4554 5552 4e53  ples.    RETURNS
+0000e680: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  :.    ----------
+0000e690: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+0000e6a0: 2046 4654 5261 7753 6967 6e3a 206e 756d   FFTRawSign: num
+0000e6b0: 7079 2e6e 6461 7272 6179 2063 6f6e 7461  py.ndarray conta
+0000e6c0: 696e 7320 7468 6520 4646 5420 6f66 2074  ins the FFT of t
+0000e6d0: 6865 2077 6869 7465 6e65 6420 696e 7075  he whitened inpu
+0000e6e0: 7420 7472 6163 6520 6265 7477 6565 6e20  t trace between 
+0000e6f0: 7468 6520 6672 6571 7565 6e63 7920 626f  the frequency bo
+0000e700: 756e 6473 0a20 2020 2022 2222 0a20 2020  unds.    """.   
+0000e710: 206e 6666 7420 3d20 6e65 7874 5f66 6173   nfft = next_fas
+0000e720: 745f 6c65 6e28 6c65 6e28 7469 6d65 7365  t_len(len(timese
+0000e730: 7269 6573 2929 0a20 2020 2073 7065 6320  ries)).    spec 
+0000e740: 3d20 6e70 2e66 6674 2e66 6674 2874 696d  = np.fft.fft(tim
+0000e750: 6573 6572 6965 732c 206e 6666 7429 0a20  eseries, nfft). 
+0000e760: 2020 2066 7265 7120 3d20 6e70 2e66 6674     freq = np.fft
+0000e770: 2e66 6674 6672 6571 286e 6666 742c 2064  .fftfreq(nfft, d
+0000e780: 3d66 6674 5f70 6172 612e 6474 290a 0a20  =fft_para.dt).. 
+0000e790: 2020 2069 7830 203d 206e 702e 6172 676d     ix0 = np.argm
+0000e7a0: 696e 286e 702e 6162 7328 6672 6571 202d  in(np.abs(freq -
+0000e7b0: 2066 6674 5f70 6172 612e 6672 6571 6d69   fft_para.freqmi
+0000e7c0: 6e29 290a 2020 2020 6978 3120 3d20 6e70  n)).    ix1 = np
+0000e7d0: 2e61 7267 6d69 6e28 6e70 2e61 6273 2866  .argmin(np.abs(f
+0000e7e0: 7265 7120 2d20 6666 745f 7061 7261 2e66  req - fft_para.f
+0000e7f0: 7265 716d 6178 2929 0a0a 2020 2020 6966  reqmax))..    if
+0000e800: 2069 7831 202b 206e 5f74 6170 6572 203e   ix1 + n_taper >
+0000e810: 206e 6666 743a 0a20 2020 2020 2020 2069   nfft:.        i
+0000e820: 7831 3120 3d20 6e66 6674 0a20 2020 2065  x11 = nfft.    e
+0000e830: 6c73 653a 0a20 2020 2020 2020 2069 7831  lse:.        ix1
+0000e840: 3120 3d20 6978 3120 2b20 6e5f 7461 7065  1 = ix1 + n_tape
+0000e850: 720a 0a20 2020 2069 6620 6978 3020 2d20  r..    if ix0 - 
+0000e860: 6e5f 7461 7065 7220 3c20 303a 0a20 2020  n_taper < 0:.   
+0000e870: 2020 2020 2069 7830 3020 3d20 300a 2020       ix00 = 0.  
+0000e880: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000e890: 6978 3030 203d 2069 7830 202d 206e 5f74  ix00 = ix0 - n_t
+0000e8a0: 6170 6572 0a0a 2020 2020 7370 6563 5f6f  aper..    spec_o
+0000e8b0: 7574 203d 2073 7065 632e 636f 7079 2829  ut = spec.copy()
+0000e8c0: 0a20 2020 2073 7065 635f 6f75 745b 303a  .    spec_out[0:
+0000e8d0: 6978 3030 5d20 3d20 302e 3020 2b20 302e  ix00] = 0.0 + 0.
+0000e8e0: 306a 0a20 2020 2073 7065 635f 6f75 745b  0j.    spec_out[
+0000e8f0: 6978 3131 3a5d 203d 2030 2e30 202b 2030  ix11:] = 0.0 + 0
+0000e900: 2e30 6a0a 0a20 2020 2069 6620 6666 745f  .0j..    if fft_
+0000e910: 7061 7261 2e73 6d6f 6f74 685f 4e20 3c3d  para.smooth_N <=
+0000e920: 2031 3a0a 2020 2020 2020 2020 7370 6563   1:.        spec
+0000e930: 5f6f 7574 5b69 7830 303a 6978 3131 5d20  _out[ix00:ix11] 
+0000e940: 3d20 6e70 2e65 7870 2831 2e30 6a20 2a20  = np.exp(1.0j * 
+0000e950: 6e70 2e61 6e67 6c65 2873 7065 635f 6f75  np.angle(spec_ou
+0000e960: 745b 6978 3030 3a69 7831 315d 2929 0a20  t[ix00:ix11])). 
+0000e970: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000e980: 2073 7065 635f 6f75 745b 6978 3030 3a69   spec_out[ix00:i
+0000e990: 7831 315d 202f 3d20 6d6f 7669 6e67 5f61  x11] /= moving_a
+0000e9a0: 7665 286e 702e 6162 7328 7370 6563 5f6f  ve(np.abs(spec_o
+0000e9b0: 7574 5b69 7830 303a 6978 3131 5d29 2c20  ut[ix00:ix11]), 
+0000e9c0: 6666 745f 7061 7261 2e73 6d6f 6f74 685f  fft_para.smooth_
+0000e9d0: 4e29 0a0a 2020 2020 7820 3d20 6e70 2e6c  N)..    x = np.l
+0000e9e0: 696e 7370 6163 6528 6e70 2e70 6920 2f20  inspace(np.pi / 
+0000e9f0: 322e 302c 206e 702e 7069 2c20 6978 3020  2.0, np.pi, ix0 
+0000ea00: 2d20 6978 3030 290a 2020 2020 7370 6563  - ix00).    spec
+0000ea10: 5f6f 7574 5b69 7830 303a 6978 305d 202a  _out[ix00:ix0] *
+0000ea20: 3d20 6e70 2e63 6f73 2878 2920 2a2a 2032  = np.cos(x) ** 2
+0000ea30: 0a0a 2020 2020 7820 3d20 6e70 2e6c 696e  ..    x = np.lin
+0000ea40: 7370 6163 6528 302e 302c 206e 702e 7069  space(0.0, np.pi
+0000ea50: 202f 2032 2e30 2c20 6978 3131 202d 2069   / 2.0, ix11 - i
+0000ea60: 7831 290a 2020 2020 7370 6563 5f6f 7574  x1).    spec_out
+0000ea70: 5b69 7831 3a69 7831 315d 202a 3d20 6e70  [ix1:ix11] *= np
+0000ea80: 2e63 6f73 2878 2920 2a2a 2032 0a0a 2020  .cos(x) ** 2..  
+0000ea90: 2020 7265 7475 726e 2073 7065 635f 6f75    return spec_ou
+0000eaa0: 740a 0a0a 6465 6620 7768 6974 656e 5f32  t...def whiten_2
+0000eab0: 4428 7469 6d65 7365 7269 6573 2c20 6666  D(timeseries, ff
+0000eac0: 745f 7061 7261 3a20 436f 6e66 6967 5061  t_para: ConfigPa
+0000ead0: 7261 6d65 7465 7273 2c20 6e5f 7461 7065  rameters, n_tape
+0000eae0: 7229 3a0a 2020 2020 2222 220a 2020 2020  r):.    """.    
+0000eaf0: 5468 6973 2066 756e 6374 696f 6e20 7461  This function ta
+0000eb00: 6b65 7320 6120 322d 6469 6d65 6e73 696f  kes a 2-dimensio
+0000eb10: 6e61 6c20 7469 6d65 7365 7269 6573 2061  nal timeseries a
+0000eb20: 7272 6179 2c20 7472 616e 7366 6f72 6d73  rray, transforms
+0000eb30: 2074 6f20 6672 6571 7565 6e63 7920 646f   to frequency do
+0000eb40: 6d61 696e 2075 7369 6e67 2066 6674 2c0a  main using fft,.
+0000eb50: 2020 2020 7768 6974 656e 7320 7468 6520      whitens the 
+0000eb60: 616d 706c 6974 7564 6520 6f66 2074 6865  amplitude of the
+0000eb70: 2073 7065 6374 7275 6d20 696e 2066 7265   spectrum in fre
+0000eb80: 7175 656e 6379 2064 6f6d 6169 6e20 6265  quency domain be
+0000eb90: 7477 6565 6e20 2a66 7265 716d 696e 2a20  tween *freqmin* 
+0000eba0: 616e 6420 2a66 7265 716d 6178 2a0a 2020  and *freqmax*.  
+0000ebb0: 2020 616e 6420 7265 7475 726e 7320 7468    and returns th
+0000ebc0: 6520 7768 6974 656e 6564 2066 6674 2e0a  e whitened fft..
+0000ebd0: 2020 2020 5041 5241 4d45 5445 5253 3a0a      PARAMETERS:.
+0000ebe0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+0000ebf0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064  ----------.    d
+0000ec00: 6174 613a 206e 756d 7079 2e6e 6461 7272  ata: numpy.ndarr
+0000ec10: 6179 2063 6f6e 7461 696e 7320 7468 6520  ay contains the 
+0000ec20: 3144 2074 696d 6520 7365 7269 6573 2074  1D time series t
+0000ec30: 6f20 7768 6974 656e 0a20 2020 2066 6674  o whiten.    fft
+0000ec40: 5f70 6172 613a 2043 6f6e 6669 6750 6172  _para: ConfigPar
+0000ec50: 616d 6574 6572 7320 636c 6173 7320 636f  ameters class co
+0000ec60: 6e74 6169 6e69 6e67 2061 6c6c 2066 6674  ntaining all fft
+0000ec70: 5f63 6320 7061 7261 6d65 7465 7273 2073  _cc parameters s
+0000ec80: 7563 6820 6173 0a20 2020 2020 2020 2064  uch as.        d
+0000ec90: 743a 2054 6865 2073 616d 706c 696e 6720  t: The sampling 
+0000eca0: 7370 6163 6520 6f66 2074 6865 2060 6461  space of the `da
+0000ecb0: 7461 600a 2020 2020 2020 2020 6672 6571  ta`.        freq
+0000ecc0: 6d69 6e3a 2054 6865 206c 6f77 6572 2066  min: The lower f
+0000ecd0: 7265 7175 656e 6379 2062 6f75 6e64 0a20  requency bound. 
+0000ece0: 2020 2020 2020 2066 7265 716d 6178 3a20         freqmax: 
+0000ecf0: 5468 6520 7570 7065 7220 6672 6571 7565  The upper freque
+0000ed00: 6e63 7920 626f 756e 640a 2020 2020 2020  ncy bound.      
+0000ed10: 2020 736d 6f6f 7468 5f4e 3a20 696e 7465    smooth_N: inte
+0000ed20: 6765 722c 2069 7420 6465 6669 6e65 7320  ger, it defines 
+0000ed30: 7468 6520 6861 6c66 2077 696e 646f 7720  the half window 
+0000ed40: 6c65 6e67 7468 2074 6f20 736d 6f6f 7468  length to smooth
+0000ed50: 0a20 2020 2020 2020 206e 5f74 6170 6572  .        n_taper
+0000ed60: 2c20 6f70 7469 6f6e 616c 3a20 696e 7465  , optional: inte
+0000ed70: 6765 722c 2064 6566 696e 6520 7468 6520  ger, define the 
+0000ed80: 7769 6474 6820 6f66 2074 6865 2074 6170  width of the tap
+0000ed90: 6572 2069 6e20 7361 6d70 6c65 730a 2020  er in samples.  
+0000eda0: 2020 5245 5455 524e 533a 0a20 2020 202d    RETURNS:.    -
+0000edb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000edc0: 2d2d 2d2d 2d0a 2020 2020 4646 5452 6177  -----.    FFTRaw
+0000edd0: 5369 676e 3a20 6e75 6d70 792e 6e64 6172  Sign: numpy.ndar
+0000ede0: 7261 7920 636f 6e74 6169 6e73 2074 6865  ray contains the
+0000edf0: 2046 4654 206f 6620 7468 6520 7768 6974   FFT of the whit
+0000ee00: 656e 6564 2069 6e70 7574 2074 7261 6365  ened input trace
+0000ee10: 2062 6574 7765 656e 2074 6865 2066 7265   between the fre
+0000ee20: 7175 656e 6379 2062 6f75 6e64 730a 2020  quency bounds.  
+0000ee30: 2020 2222 220a 2020 2020 6e66 6674 203d    """.    nfft =
+0000ee40: 206e 6578 745f 6661 7374 5f6c 656e 2874   next_fast_len(t
+0000ee50: 696d 6573 6572 6965 732e 7368 6170 655b  imeseries.shape[
+0000ee60: 315d 290a 2020 2020 7370 6563 203d 206e  1]).    spec = n
+0000ee70: 702e 6666 742e 6666 746e 2874 696d 6573  p.fft.fftn(times
+0000ee80: 6572 6965 732c 2073 3d5b 6e66 6674 5d29  eries, s=[nfft])
+0000ee90: 0a20 2020 2066 7265 7120 3d20 6e70 2e66  .    freq = np.f
+0000eea0: 6674 2e66 6674 6672 6571 286e 6666 742c  ft.fftfreq(nfft,
+0000eeb0: 2064 3d66 6674 5f70 6172 612e 6474 290a   d=fft_para.dt).
+0000eec0: 0a20 2020 2069 7830 203d 206e 702e 6172  .    ix0 = np.ar
+0000eed0: 676d 696e 286e 702e 6162 7328 6672 6571  gmin(np.abs(freq
+0000eee0: 202d 2066 6674 5f70 6172 612e 6672 6571   - fft_para.freq
+0000eef0: 6d69 6e29 290a 2020 2020 6978 3120 3d20  min)).    ix1 = 
+0000ef00: 6e70 2e61 7267 6d69 6e28 6e70 2e61 6273  np.argmin(np.abs
+0000ef10: 2866 7265 7120 2d20 6666 745f 7061 7261  (freq - fft_para
+0000ef20: 2e66 7265 716d 6178 2929 0a0a 2020 2020  .freqmax))..    
+0000ef30: 6966 2069 7831 202b 206e 5f74 6170 6572  if ix1 + n_taper
+0000ef40: 203e 206e 6666 743a 0a20 2020 2020 2020   > nfft:.       
+0000ef50: 2069 7831 3120 3d20 6e66 6674 0a20 2020   ix11 = nfft.   
+0000ef60: 2065 6c73 653a 0a20 2020 2020 2020 2069   else:.        i
+0000ef70: 7831 3120 3d20 6978 3120 2b20 6e5f 7461  x11 = ix1 + n_ta
+0000ef80: 7065 720a 0a20 2020 2069 6620 6978 3020  per..    if ix0 
+0000ef90: 2d20 6e5f 7461 7065 7220 3c20 303a 0a20  - n_taper < 0:. 
+0000efa0: 2020 2020 2020 2069 7830 3020 3d20 300a         ix00 = 0.
+0000efb0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000efc0: 2020 6978 3030 203d 2069 7830 202d 206e    ix00 = ix0 - n
+0000efd0: 5f74 6170 6572 0a0a 2020 2020 7370 6563  _taper..    spec
+0000efe0: 5f6f 7574 203d 2073 7065 632e 636f 7079  _out = spec.copy
+0000eff0: 2829 2020 2320 6d61 7920 6265 2069 6e63  ()  # may be inc
+0000f000: 6f6e 7665 6e69 656e 7420 6475 6520 746f  onvenient due to
+0000f010: 2068 6967 6865 7220 6d65 6d6f 7279 2075   higher memory u
+0000f020: 7361 6765 0a20 2020 2073 7065 635f 6f75  sage.    spec_ou
+0000f030: 745b 3a2c 2030 3a69 7830 305d 203d 2030  t[:, 0:ix00] = 0
+0000f040: 2e30 202b 2030 2e30 6a0a 2020 2020 7370  .0 + 0.0j.    sp
+0000f050: 6563 5f6f 7574 5b3a 2c20 6978 3131 3a5d  ec_out[:, ix11:]
+0000f060: 203d 2030 2e30 202b 2030 2e30 6a0a 0a20   = 0.0 + 0.0j.. 
+0000f070: 2020 2069 6620 6666 745f 7061 7261 2e73     if fft_para.s
+0000f080: 6d6f 6f74 685f 4e20 3c3d 2031 3a0a 2020  mooth_N <= 1:.  
+0000f090: 2020 2020 2020 7370 6563 5f6f 7574 5b3a        spec_out[:
+0000f0a0: 2c20 6978 3030 3a69 7831 315d 203d 206e  , ix00:ix11] = n
+0000f0b0: 702e 6578 7028 312e 306a 202a 206e 702e  p.exp(1.0j * np.
+0000f0c0: 616e 676c 6528 7370 6563 5f6f 7574 5b3a  angle(spec_out[:
+0000f0d0: 2c20 6978 3030 3a69 7831 315d 2929 0a20  , ix00:ix11])). 
+0000f0e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000f0f0: 2073 7065 635f 6f75 745b 3a2c 2069 7830   spec_out[:, ix0
+0000f100: 303a 6978 3131 5d20 2f3d 206d 6f76 696e  0:ix11] /= movin
+0000f110: 675f 6176 655f 3244 286e 702e 6162 7328  g_ave_2D(np.abs(
+0000f120: 7370 6563 5f6f 7574 5b3a 2c20 6978 3030  spec_out[:, ix00
+0000f130: 3a69 7831 315d 292c 2066 6674 5f70 6172  :ix11]), fft_par
+0000f140: 612e 736d 6f6f 7468 5f4e 290a 0a20 2020  a.smooth_N)..   
+0000f150: 2078 203d 206e 702e 6c69 6e73 7061 6365   x = np.linspace
+0000f160: 286e 702e 7069 202f 2032 2e30 2c20 6e70  (np.pi / 2.0, np
+0000f170: 2e70 692c 2069 7830 202d 2069 7830 3029  .pi, ix0 - ix00)
+0000f180: 0a20 2020 2073 7065 635f 6f75 745b 3a2c  .    spec_out[:,
+0000f190: 2069 7830 303a 6978 305d 202a 3d20 6e70   ix00:ix0] *= np
+0000f1a0: 2e63 6f73 2878 2920 2a2a 2032 0a0a 2020  .cos(x) ** 2..  
+0000f1b0: 2020 7820 3d20 6e70 2e6c 696e 7370 6163    x = np.linspac
+0000f1c0: 6528 302e 302c 206e 702e 7069 202f 2032  e(0.0, np.pi / 2
+0000f1d0: 2e30 2c20 6978 3131 202d 2069 7831 290a  .0, ix11 - ix1).
+0000f1e0: 2020 2020 7370 6563 5f6f 7574 5b3a 2c20      spec_out[:, 
+0000f1f0: 6978 313a 6978 3131 5d20 2a3d 206e 702e  ix1:ix11] *= np.
+0000f200: 636f 7328 7829 202a 2a20 320a 0a20 2020  cos(x) ** 2..   
+0000f210: 2072 6574 7572 6e20 7370 6563 5f6f 7574   return spec_out
+0000f220: 0a0a 0a64 6566 2077 6869 7465 6e28 6461  ...def whiten(da
+0000f230: 7461 2c20 6666 745f 7061 7261 3a20 436f  ta, fft_para: Co
+0000f240: 6e66 6967 5061 7261 6d65 7465 7273 2c20  nfigParameters, 
+0000f250: 6e5f 7461 7065 723d 3130 3029 3a0a 2020  n_taper=100):.  
+0000f260: 2020 2222 220a 2020 2020 5468 6973 2066    """.    This f
+0000f270: 756e 6374 696f 6e20 7461 6b65 7320 6120  unction takes a 
+0000f280: 7469 6d65 7365 7269 6573 2061 7272 6179  timeseries array
+0000f290: 2c20 7472 616e 7366 6f72 6d73 2074 6f20  , transforms to 
+0000f2a0: 6672 6571 7565 6e63 7920 646f 6d61 696e  frequency domain
+0000f2b0: 2075 7369 6e67 2066 6674 2c0a 2020 2020   using fft,.    
+0000f2c0: 7768 6974 656e 7320 7468 6520 616d 706c  whitens the ampl
+0000f2d0: 6974 7564 6520 6f66 2074 6865 2073 7065  itude of the spe
+0000f2e0: 6374 7275 6d20 696e 2066 7265 7175 656e  ctrum in frequen
+0000f2f0: 6379 2064 6f6d 6169 6e20 6265 7477 6565  cy domain betwee
+0000f300: 6e20 2a66 7265 716d 696e 2a20 616e 6420  n *freqmin* and 
+0000f310: 2a66 7265 716d 6178 2a0a 2020 2020 616e  *freqmax*.    an
+0000f320: 6420 7265 7475 726e 7320 7468 6520 7768  d returns the wh
+0000f330: 6974 656e 6564 2066 6674 2e0a 2020 2020  itened fft..    
+0000f340: 5041 5241 4d45 5445 5253 3a0a 2020 2020  PARAMETERS:.    
+0000f350: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000f360: 2d2d 2d2d 2d2d 0a20 2020 2064 6174 613a  ------.    data:
+0000f370: 206e 756d 7079 2e6e 6461 7272 6179 2063   numpy.ndarray c
+0000f380: 6f6e 7461 696e 7320 7468 6520 3144 2074  ontains the 1D t
+0000f390: 696d 6520 7365 7269 6573 2074 6f20 7768  ime series to wh
+0000f3a0: 6974 656e 0a20 2020 2066 6674 5f70 6172  iten.    fft_par
+0000f3b0: 613a 2043 6f6e 6669 6750 6172 616d 6574  a: ConfigParamet
+0000f3c0: 6572 7320 636c 6173 7320 636f 6e74 6169  ers class contai
+0000f3d0: 6e69 6e67 2061 6c6c 2066 6674 5f63 6320  ning all fft_cc 
+0000f3e0: 7061 7261 6d65 7465 7273 2073 7563 6820  parameters such 
+0000f3f0: 6173 0a20 2020 2020 2020 2064 743a 2054  as.        dt: T
+0000f400: 6865 2073 616d 706c 696e 6720 7370 6163  he sampling spac
+0000f410: 6520 6f66 2074 6865 2060 6461 7461 600a  e of the `data`.
+0000f420: 2020 2020 2020 2020 6672 6571 6d69 6e3a          freqmin:
+0000f430: 2054 6865 206c 6f77 6572 2066 7265 7175   The lower frequ
+0000f440: 656e 6379 2062 6f75 6e64 0a20 2020 2020  ency bound.     
+0000f450: 2020 2066 7265 716d 6178 3a20 5468 6520     freqmax: The 
+0000f460: 7570 7065 7220 6672 6571 7565 6e63 7920  upper frequency 
+0000f470: 626f 756e 640a 2020 2020 2020 2020 736d  bound.        sm
+0000f480: 6f6f 7468 5f4e 3a20 696e 7465 6765 722c  ooth_N: integer,
+0000f490: 2069 7420 6465 6669 6e65 7320 7468 6520   it defines the 
+0000f4a0: 6861 6c66 2077 696e 646f 7720 6c65 6e67  half window leng
+0000f4b0: 7468 2074 6f20 736d 6f6f 7468 0a20 2020  th to smooth.   
+0000f4c0: 2020 2020 2066 7265 715f 6e6f 726d 3a20       freq_norm: 
+0000f4d0: 7768 6974 656e 696e 6720 6d65 7468 6f64  whitening method
+0000f4e0: 2062 6574 7765 656e 2027 6f6e 652d 6269   between 'one-bi
+0000f4f0: 7427 2061 6e64 2027 524d 4127 0a20 2020  t' and 'RMA'.   
+0000f500: 2052 4554 5552 4e53 3a0a 2020 2020 2d2d   RETURNS:.    --
+0000f510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000f520: 2d2d 2d2d 0a20 2020 2046 4654 5261 7753  ----.    FFTRawS
+0000f530: 6967 6e3a 206e 756d 7079 2e6e 6461 7272  ign: numpy.ndarr
+0000f540: 6179 2063 6f6e 7461 696e 7320 7468 6520  ay contains the 
+0000f550: 4646 5420 6f66 2074 6865 2077 6869 7465  FFT of the white
+0000f560: 6e65 6420 696e 7075 7420 7472 6163 6520  ned input trace 
+0000f570: 6265 7477 6565 6e20 7468 6520 6672 6571  between the freq
+0000f580: 7565 6e63 7920 626f 756e 6473 0a20 2020  uency bounds.   
+0000f590: 2022 2222 0a0a 2020 2020 2320 5370 6565   """..    # Spee
+0000f5a0: 6420 7570 2046 4654 2062 7920 7061 6464  d up FFT by padd
+0000f5b0: 696e 6720 746f 206f 7074 696d 616c 2073  ing to optimal s
+0000f5c0: 697a 6520 666f 7220 4646 5450 4143 4b0a  ize for FFTPACK.
+0000f5d0: 2020 2020 6966 2064 6174 612e 6e64 696d      if data.ndim
+0000f5e0: 203d 3d20 313a 0a20 2020 2020 2020 2046   == 1:.        F
+0000f5f0: 4654 5261 7753 6967 6e20 3d20 7768 6974  FTRawSign = whit
+0000f600: 656e 5f31 4428 6461 7461 2c20 6666 745f  en_1D(data, fft_
+0000f610: 7061 7261 2c20 6e5f 7461 7065 7229 0a20  para, n_taper). 
+0000f620: 2020 2020 2020 2023 2041 5252 5f4f 5554         # ARR_OUT
+0000f630: 3a20 4f6e 6c79 2066 6f72 2063 6f6e 7369  : Only for consi
+0000f640: 7374 656e 6379 2077 6974 6820 6e6f 6973  stency with nois
+0000f650: 6570 7920 6170 7072 6f61 6368 206f 6620  epy approach of 
+0000f660: 686f 6c64 696e 6720 7468 6520 6675 6c6c  holding the full
+0000f670: 0a20 2020 2020 2020 2023 2073 7065 6374  .        # spect
+0000f680: 7275 6d20 286e 6f74 206a 7573 7420 3020  rum (not just 0 
+0000f690: 616e 6420 706f 7369 7469 7665 2066 7265  and positive fre
+0000f6a0: 712e 2070 6172 7429 0a20 2020 2020 2020  q. part).       
+0000f6b0: 2061 7272 5f6f 7574 203d 206e 702e 7a65   arr_out = np.ze
+0000f6c0: 726f 7328 2846 4654 5261 7753 6967 6e2e  ros((FFTRawSign.
+0000f6d0: 7368 6170 655b 305d 202d 2031 2920 2a20  shape[0] - 1) * 
+0000f6e0: 3220 2b20 312c 2064 7479 7065 3d63 6f6d  2 + 1, dtype=com
+0000f6f0: 706c 6578 290a 2020 2020 2020 2020 6172  plex).        ar
+0000f700: 725f 6f75 745b 3020 3a20 4646 5452 6177  r_out[0 : FFTRaw
+0000f710: 5369 676e 2e73 6861 7065 5b30 5d5d 203d  Sign.shape[0]] =
+0000f720: 2046 4654 5261 7753 6967 6e0a 2020 2020   FFTRawSign.    
+0000f730: 2020 2020 6172 725f 6f75 745b 4646 5452      arr_out[FFTR
+0000f740: 6177 5369 676e 2e73 6861 7065 5b30 5d20  awSign.shape[0] 
+0000f750: 3a5d 203d 2046 4654 5261 7753 6967 6e5b  :] = FFTRawSign[
+0000f760: 313a 5d2e 636f 6e6a 7567 6174 6528 295b  1:].conjugate()[
+0000f770: 3a3a 2d31 5d0a 0a20 2020 2065 6c69 6620  ::-1]..    elif 
+0000f780: 6461 7461 2e6e 6469 6d20 3d3d 2032 3a0a  data.ndim == 2:.
+0000f790: 2020 2020 2020 2020 4646 5452 6177 5369          FFTRawSi
+0000f7a0: 676e 203d 2077 6869 7465 6e5f 3244 2864  gn = whiten_2D(d
+0000f7b0: 6174 612c 2066 6674 5f70 6172 612c 206e  ata, fft_para, n
+0000f7c0: 5f74 6170 6572 290a 2020 2020 2020 2020  _taper).        
+0000f7d0: 6172 725f 6f75 7420 3d20 6e70 2e7a 6572  arr_out = np.zer
+0000f7e0: 6f73 2828 4646 5452 6177 5369 676e 2e73  os((FFTRawSign.s
+0000f7f0: 6861 7065 5b30 5d2c 2028 4646 5452 6177  hape[0], (FFTRaw
+0000f800: 5369 676e 2e73 6861 7065 5b31 5d20 2d20  Sign.shape[1] - 
+0000f810: 3129 202a 2032 202b 2031 292c 2064 7479  1) * 2 + 1), dty
+0000f820: 7065 3d63 6f6d 706c 6578 290a 2020 2020  pe=complex).    
+0000f830: 2020 2020 6172 725f 6f75 745b 3a2c 2046      arr_out[:, F
+0000f840: 4654 5261 7753 6967 6e2e 7368 6170 655b  FTRawSign.shape[
+0000f850: 315d 203a 5d20 3d20 4646 5452 6177 5369  1] :] = FFTRawSi
+0000f860: 676e 5b3a 2c20 313a 5d2e 636f 6e6a 7567  gn[:, 1:].conjug
+0000f870: 6174 6528 295b 3a3a 2d31 5d0a 2020 2020  ate()[::-1].    
+0000f880: 7265 7475 726e 2046 4654 5261 7753 6967  return FFTRawSig
+0000f890: 6e0a 0a0a 6465 6620 6164 6170 7469 7665  n...def adaptive
+0000f8a0: 5f66 696c 7465 7228 6172 722c 2067 293a  _filter(arr, g):
+0000f8b0: 0a20 2020 2022 2222 0a20 2020 2074 6865  .    """.    the
+0000f8c0: 2061 6461 7074 6976 6520 636f 7661 7269   adaptive covari
+0000f8d0: 616e 6365 2066 696c 7465 7220 746f 2065  ance filter to e
+0000f8e0: 6e68 616e 6365 2063 6f68 6572 656e 7420  nhance coherent 
+0000f8f0: 7369 676e 616c 732e 2046 656c 6c6f 7773  signals. Fellows
+0000f900: 2074 6865 206d 6574 686f 6420 6f66 0a20   the method of. 
+0000f910: 2020 204e 616b 6174 6120 6574 2061 6c2e     Nakata et al.
+0000f920: 2c20 3230 3135 2028 4170 7065 6e64 6978  , 2015 (Appendix
+0000f930: 2042 290a 0a20 2020 2074 6865 2066 696c   B)..    the fil
+0000f940: 7465 7265 6420 7369 676e 616c 205b 7831  tered signal [x1
+0000f950: 5d20 6973 2067 6976 656e 2062 7920 7831  ] is given by x1
+0000f960: 203d 2069 6666 7428 502a 7831 2877 2929   = ifft(P*x1(w))
+0000f970: 2077 6865 7265 2078 3120 6973 2074 6865   where x1 is the
+0000f980: 2066 6674 6564 2073 7065 6374 7261 0a20   ffted spectra. 
+0000f990: 2020 2061 6e64 2050 2069 7320 7468 6520     and P is the 
+0000f9a0: 6669 6c74 6572 2e20 5020 6973 2063 6f6e  filter. P is con
+0000f9b0: 7374 7275 6374 6564 2062 7920 7573 696e  structed by usin
+0000f9c0: 6720 7468 6520 7465 6d70 6f72 616c 2063  g the temporal c
+0000f9d0: 6f76 6172 6961 6e63 6520 6d61 7472 6978  ovariance matrix
+0000f9e0: 2e0a 0a20 2020 2050 4152 414d 4554 4552  ...    PARAMETER
+0000f9f0: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
+0000fa00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+0000fa10: 2020 6172 723a 206e 756d 7079 2e6e 6461    arr: numpy.nda
+0000fa20: 7272 6179 2063 6f6e 7461 696e 7320 7468  rray contains th
+0000fa30: 6520 3244 2074 7261 6365 7320 6f66 2064  e 2D traces of d
+0000fa40: 6169 6c79 2f68 6f75 726c 7920 6372 6f73  aily/hourly cros
+0000fa50: 732d 636f 7272 656c 6174 696f 6e20 6675  s-correlation fu
+0000fa60: 6e63 7469 6f6e 730a 2020 2020 673a 2061  nctions.    g: a
+0000fa70: 2070 6f73 6974 6976 6520 6e75 6d62 6572   positive number
+0000fa80: 2074 6f20 6164 6a75 7374 2074 6865 2066   to adjust the f
+0000fa90: 696c 7465 7220 6861 7273 686e 6573 730a  ilter harshness.
+0000faa0: 2020 2020 5245 5455 524e 533a 0a20 2020      RETURNS:.   
+0000fab0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+0000fac0: 2d2d 2d2d 2d2d 2d0a 2020 2020 6e61 7272  -------.    narr
+0000fad0: 3a20 6e75 6d70 7920 7665 6374 6f72 2063  : numpy vector c
+0000fae0: 6f6e 7461 696e 7320 7468 6520 7374 6163  ontains the stac
+0000faf0: 6b65 6420 6372 6f73 7320 636f 7272 656c  ked cross correl
+0000fb00: 6174 696f 6e20 6675 6e63 7469 6f6e 0a20  ation function. 
+0000fb10: 2020 2022 2222 0a20 2020 2069 6620 6172     """.    if ar
+0000fb20: 722e 6e64 696d 203d 3d20 313a 0a20 2020  r.ndim == 1:.   
+0000fb30: 2020 2020 2072 6574 7572 6e20 6172 720a       return arr.
+0000fb40: 2020 2020 4e2c 204d 203d 2061 7272 2e73      N, M = arr.s
+0000fb50: 6861 7065 0a20 2020 204e 6666 7420 3d20  hape.    Nfft = 
+0000fb60: 6e65 7874 5f66 6173 745f 6c65 6e28 4d29  next_fast_len(M)
+0000fb70: 0a0a 2020 2020 2320 6666 7420 7468 6520  ..    # fft the 
+0000fb80: 3244 2061 7272 6179 0a20 2020 2073 7065  2D array.    spe
+0000fb90: 6320 3d20 7363 6970 792e 6666 7470 6163  c = scipy.fftpac
+0000fba0: 6b2e 6666 7428 6172 722c 2061 7869 733d  k.fft(arr, axis=
+0000fbb0: 312c 206e 3d4e 6666 7429 5b3a 2c20 3a4d  1, n=Nfft)[:, :M
+0000fbc0: 5d0a 0a20 2020 2023 206d 616b 6520 6372  ]..    # make cr
+0000fbd0: 6f73 732d 7370 6563 7472 6d20 6d61 7472  oss-spectrm matr
+0000fbe0: 6978 0a20 2020 2063 7370 6563 203d 206e  ix.    cspec = n
+0000fbf0: 702e 7a65 726f 7328 7368 6170 653d 284e  p.zeros(shape=(N
+0000fc00: 202a 204e 2c20 4d29 2c20 6474 7970 653d   * N, M), dtype=
+0000fc10: 6e70 2e63 6f6d 706c 6578 3634 290a 2020  np.complex64).  
+0000fc20: 2020 666f 7220 6969 2069 6e20 7261 6e67    for ii in rang
+0000fc30: 6528 4e29 3a0a 2020 2020 2020 2020 666f  e(N):.        fo
+0000fc40: 7220 6a6a 2069 6e20 7261 6e67 6528 4e29  r jj in range(N)
+0000fc50: 3a0a 2020 2020 2020 2020 2020 2020 6b6b  :.            kk
+0000fc60: 203d 2069 6920 2a20 4e20 2b20 6a6a 0a20   = ii * N + jj. 
+0000fc70: 2020 2020 2020 2020 2020 2063 7370 6563             cspec
+0000fc80: 5b6b 6b5d 203d 2073 7065 635b 6969 5d20  [kk] = spec[ii] 
+0000fc90: 2a20 6e70 2e63 6f6e 6a75 6761 7465 2873  * np.conjugate(s
+0000fca0: 7065 635b 6a6a 5d29 0a0a 2020 2020 5331  pec[jj])..    S1
+0000fcb0: 203d 206e 702e 7a65 726f 7328 4d2c 2064   = np.zeros(M, d
+0000fcc0: 7479 7065 3d6e 702e 636f 6d70 6c65 7836  type=np.complex6
+0000fcd0: 3429 0a20 2020 2053 3220 3d20 6e70 2e7a  4).    S2 = np.z
+0000fce0: 6572 6f73 284d 2c20 6474 7970 653d 6e70  eros(M, dtype=np
+0000fcf0: 2e63 6f6d 706c 6578 3634 290a 2020 2020  .complex64).    
+0000fd00: 2320 636f 6e73 7472 7563 7420 7468 6520  # construct the 
+0000fd10: 6669 6c74 6572 2050 0a20 2020 2066 6f72  filter P.    for
+0000fd20: 2069 6920 696e 2072 616e 6765 284e 293a   ii in range(N):
+0000fd30: 0a20 2020 2020 2020 206d 6d20 3d20 6969  .        mm = ii
+0000fd40: 202a 204e 202b 2069 690a 2020 2020 2020   * N + ii.      
+0000fd50: 2020 5332 202b 3d20 6373 7065 635b 6d6d    S2 += cspec[mm
+0000fd60: 5d0a 2020 2020 2020 2020 666f 7220 6a6a  ].        for jj
+0000fd70: 2069 6e20 7261 6e67 6528 4e29 3a0a 2020   in range(N):.  
+0000fd80: 2020 2020 2020 2020 2020 6b6b 203d 2069            kk = i
+0000fd90: 6920 2a20 4e20 2b20 6a6a 0a20 2020 2020  i * N + jj.     
+0000fda0: 2020 2020 2020 2053 3120 2b3d 2063 7370         S1 += csp
+0000fdb0: 6563 5b6b 6b5d 0a0a 2020 2020 7020 3d20  ec[kk]..    p = 
+0000fdc0: 6e70 2e70 6f77 6572 2828 5331 202d 2053  np.power((S1 - S
+0000fdd0: 3229 202f 2028 5332 202a 2028 4e20 2d20  2) / (S2 * (N - 
+0000fde0: 3129 292c 2067 290a 0a20 2020 2023 206d  1)), g)..    # m
+0000fdf0: 616b 6520 6966 6674 0a20 2020 206e 6172  ake ifft.    nar
+0000fe00: 7220 3d20 6e70 2e72 6561 6c28 7363 6970  r = np.real(scip
+0000fe10: 792e 6666 7470 6163 6b2e 6966 6674 286e  y.fftpack.ifft(n
+0000fe20: 702e 6d75 6c74 6970 6c79 2870 2c20 7370  p.multiply(p, sp
+0000fe30: 6563 292c 204e 6666 742c 2061 7869 733d  ec), Nfft, axis=
+0000fe40: 3129 5b3a 2c20 3a4d 5d29 0a20 2020 2072  1)[:, :M]).    r
+0000fe50: 6574 7572 6e20 6e70 2e6d 6561 6e28 6e61  eturn np.mean(na
+0000fe60: 7272 2c20 6178 6973 3d30 290a 0a0a 6465  rr, axis=0)...de
+0000fe70: 6620 7077 7328 6172 722c 2073 616d 706c  f pws(arr, sampl
+0000fe80: 696e 675f 7261 7465 2c20 706f 7765 723d  ing_rate, power=
+0000fe90: 322c 2070 7773 5f74 696d 6567 6174 653d  2, pws_timegate=
+0000fea0: 352e 3029 3a0a 2020 2020 2222 220a 2020  5.0):.    """.  
+0000feb0: 2020 5065 7266 6f72 6d73 2070 6861 7365    Performs phase
+0000fec0: 2d77 6569 6768 7465 6420 7374 6163 6b20  -weighted stack 
+0000fed0: 6f6e 2061 7272 6179 206f 6620 7469 6d65  on array of time
+0000fee0: 2073 6572 6965 732e 204d 6f64 6966 6965   series. Modifie
+0000fef0: 6420 6f6e 2074 6865 206e 6f69 7365 2066  d on the noise f
+0000ff00: 756e 6374 696f 6e20 6279 2054 696d 2043  unction by Tim C
+0000ff10: 6c69 6d65 6e74 732e 0a20 2020 2046 6f6c  liments..    Fol
+0000ff20: 6c6f 7773 206d 6574 686f 6473 206f 6620  lows methods of 
+0000ff30: 5363 6869 6d6d 656c 2061 6e64 2050 6175  Schimmel and Pau
+0000ff40: 6c73 7365 6e2c 2031 3939 372e 0a20 2020  lssen, 1997..   
+0000ff50: 2049 6620 7328 7429 2069 7320 7469 6d65   If s(t) is time
+0000ff60: 2073 6572 6965 7320 6461 7461 2028 7365   series data (se
+0000ff70: 6973 6d6f 6772 616d 2c20 6f72 2063 726f  ismogram, or cro
+0000ff80: 7373 2d63 6f72 7265 6c61 7469 6f6e 292c  ss-correlation),
+0000ff90: 0a20 2020 2053 2874 2920 3d20 7328 7429  .    S(t) = s(t)
+0000ffa0: 202b 2069 2a48 2873 2874 2929 2c20 7768   + i*H(s(t)), wh
+0000ffb0: 6572 6520 4828 7328 7429 2920 6973 2048  ere H(s(t)) is H
+0000ffc0: 696c 6265 7274 2074 7261 6e73 666f 726d  ilbert transform
+0000ffd0: 206f 6620 7328 7429 0a20 2020 2053 2874   of s(t).    S(t
+0000ffe0: 2920 3d20 7328 7429 202b 2069 2a48 2873  ) = s(t) + i*H(s
+0000fff0: 2874 2929 203d 2041 2874 292a 6578 7028  (t)) = A(t)*exp(
+00010000: 692a 7068 6928 7429 292c 2077 6865 7265  i*phi(t)), where
+00010010: 0a20 2020 2041 2874 2920 6973 2065 6e76  .    A(t) is env
+00010020: 656c 6f70 6520 6f66 2073 2874 2920 616e  elope of s(t) an
+00010030: 6420 7068 6928 7429 2069 7320 7068 6173  d phi(t) is phas
+00010040: 6520 6f66 2073 2874 290a 2020 2020 5068  e of s(t).    Ph
+00010050: 6173 652d 7765 6967 6874 6564 2073 7461  ase-weighted sta
+00010060: 636b 2c20 6728 7429 2c20 6973 2074 6865  ck, g(t), is the
+00010070: 6e3a 0a20 2020 2067 2874 2920 3d20 312f  n:.    g(t) = 1/
+00010080: 4e20 7375 6d20 6a20 3d20 313a 4e20 735f  N sum j = 1:N s_
+00010090: 6a28 7429 202a 207c 2031 2f4e 2073 756d  j(t) * | 1/N sum
+000100a0: 206b 203d 2031 3a4e 2065 7870 5b69 202a   k = 1:N exp[i *
+000100b0: 2070 6869 5f6b 2874 295d 7c5e 760a 2020   phi_k(t)]|^v.  
+000100c0: 2020 7768 6572 6520 4e20 6973 206e 756d    where N is num
+000100d0: 6265 7220 6f66 2074 7261 6365 7320 7573  ber of traces us
+000100e0: 6564 2c20 7620 6973 2073 6861 7270 6e65  ed, v is sharpne
+000100f0: 7373 206f 6620 7068 6173 652d 7765 6967  ss of phase-weig
+00010100: 6874 6564 2073 7461 636b 0a0a 2020 2020  hted stack..    
+00010110: 5041 5241 4d45 5445 5253 3a0a 2020 2020  PARAMETERS:.    
+00010120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00010130: 2d2d 2d2d 2d0a 2020 2020 6172 723a 204e  -----.    arr: N
+00010140: 206c 656e 6774 6820 6172 7261 7920 6f66   length array of
+00010150: 2074 696d 6520 7365 7269 6573 2064 6174   time series dat
+00010160: 6120 286e 756d 7079 2e6e 6461 7272 6179  a (numpy.ndarray
+00010170: 290a 2020 2020 7361 6d70 6c69 6e67 5f72  ).    sampling_r
+00010180: 6174 653a 2073 616d 706c 696e 6720 7261  ate: sampling ra
+00010190: 7465 206f 6620 7469 6d65 2073 6572 6965  te of time serie
+000101a0: 7320 6172 7220 2869 6e74 290a 2020 2020  s arr (int).    
+000101b0: 706f 7765 723a 2065 7870 6f6e 656e 7420  power: exponent 
+000101c0: 666f 7220 7068 6173 6520 7374 6163 6b20  for phase stack 
+000101d0: 2869 6e74 290a 2020 2020 7077 735f 7469  (int).    pws_ti
+000101e0: 6d65 6761 7465 3a20 6e75 6d62 6572 206f  megate: number o
+000101f0: 6620 7365 636f 6e64 7320 746f 2073 6d6f  f seconds to smo
+00010200: 6f74 6820 7068 6173 6520 7374 6163 6b20  oth phase stack 
+00010210: 2866 6c6f 6174 290a 0a20 2020 2052 4554  (float)..    RET
+00010220: 5552 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d  URNS:.    ------
+00010230: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+00010240: 2020 2020 7765 6967 6874 6564 3a20 5068      weighted: Ph
+00010250: 6173 6520 7765 6967 6874 6564 2073 7461  ase weighted sta
+00010260: 636b 206f 6620 7469 6d65 2073 6572 6965  ck of time serie
+00010270: 7320 6461 7461 2028 6e75 6d70 792e 6e64  s data (numpy.nd
+00010280: 6172 7261 7929 0a20 2020 2022 2222 0a0a  array).    """..
+00010290: 2020 2020 6966 2061 7272 2e6e 6469 6d20      if arr.ndim 
+000102a0: 3d3d 2031 3a0a 2020 2020 2020 2020 7265  == 1:.        re
+000102b0: 7475 726e 2061 7272 0a20 2020 204e 2c20  turn arr.    N, 
+000102c0: 4d20 3d20 6172 722e 7368 6170 650a 2020  M = arr.shape.  
+000102d0: 2020 616e 616c 7974 6963 203d 2068 696c    analytic = hil
+000102e0: 6265 7274 2861 7272 2c20 6178 6973 3d31  bert(arr, axis=1
+000102f0: 2c20 4e3d 6e65 7874 5f66 6173 745f 6c65  , N=next_fast_le
+00010300: 6e28 4d29 295b 3a2c 203a 4d5d 0a20 2020  n(M))[:, :M].   
+00010310: 2070 6861 7365 203d 206e 702e 616e 676c   phase = np.angl
+00010320: 6528 616e 616c 7974 6963 290a 2020 2020  e(analytic).    
+00010330: 7068 6173 655f 7374 6163 6b20 3d20 6e70  phase_stack = np
+00010340: 2e6d 6561 6e28 6e70 2e65 7870 2831 6a20  .mean(np.exp(1j 
+00010350: 2a20 7068 6173 6529 2c20 6178 6973 3d30  * phase), axis=0
+00010360: 290a 2020 2020 7068 6173 655f 7374 6163  ).    phase_stac
+00010370: 6b20 3d20 6e70 2e61 6273 2870 6861 7365  k = np.abs(phase
+00010380: 5f73 7461 636b 2920 2a2a 2028 706f 7765  _stack) ** (powe
+00010390: 7229 0a0a 2020 2020 2320 736d 6f6f 7468  r)..    # smooth
+000103a0: 696e 670a 2020 2020 2320 7469 6d65 6761  ing.    # timega
+000103b0: 7465 5f73 616d 706c 6573 203d 2069 6e74  te_samples = int
+000103c0: 2870 7773 5f74 696d 6567 6174 6520 2a20  (pws_timegate * 
+000103d0: 7361 6d70 6c69 6e67 5f72 6174 6529 0a20  sampling_rate). 
+000103e0: 2020 2023 2070 6861 7365 5f73 7461 636b     # phase_stack
+000103f0: 203d 206d 6f76 696e 675f 6176 6528 7068   = moving_ave(ph
+00010400: 6173 655f 7374 6163 6b2c 7469 6d65 6761  ase_stack,timega
+00010410: 7465 5f73 616d 706c 6573 290a 2020 2020  te_samples).    
+00010420: 7765 6967 6874 6564 203d 206e 702e 6d75  weighted = np.mu
+00010430: 6c74 6970 6c79 2861 7272 2c20 7068 6173  ltiply(arr, phas
+00010440: 655f 7374 6163 6b29 0a20 2020 2072 6574  e_stack).    ret
+00010450: 7572 6e20 6e70 2e6d 6561 6e28 7765 6967  urn np.mean(weig
+00010460: 6874 6564 2c20 6178 6973 3d30 290a 0a0a  hted, axis=0)...
+00010470: 6465 6620 6e72 6f6f 745f 7374 6163 6b28  def nroot_stack(
+00010480: 6363 5f61 7272 6179 2c20 706f 7765 7229  cc_array, power)
+00010490: 3a0a 2020 2020 2222 220a 2020 2020 7468  :.    """.    th
+000104a0: 6973 2069 7320 6e74 682d 726f 6f74 2073  is is nth-root s
+000104b0: 7461 636b 696e 6720 616c 676f 7269 7468  tacking algorith
+000104c0: 6d20 7472 616e 736c 6174 6564 2062 6173  m translated bas
+000104d0: 6564 206f 6e20 7468 6520 6d61 746c 6162  ed on the matlab
+000104e0: 2066 756e 6374 696f 6e0a 2020 2020 6672   function.    fr
+000104f0: 6f6d 2068 7474 7073 3a2f 2f67 6974 6875  om https://githu
+00010500: 622e 636f 6d2f 7874 7961 6e67 7073 702f  b.com/xtyangpsp/
+00010510: 5365 6973 5374 6163 6b20 2862 7920 5869  SeisStack (by Xi
+00010520: 616f 7461 6f20 5961 6e67 3b20 666f 6c6c  aotao Yang; foll
+00010530: 6f77 7320 7468 650a 2020 2020 7265 6665  ows the.    refe
+00010540: 7265 6e63 6520 6f66 204d 696c 6c65 742c  rence of Millet,
+00010550: 2046 2065 7420 616c 2e2c 2032 3031 3920   F et al., 2019 
+00010560: 4a47 5229 0a0a 2020 2020 5061 7261 6d65  JGR)..    Parame
+00010570: 7465 7273 3a0a 2020 2020 2d2d 2d2d 2d2d  ters:.    ------
+00010580: 2d2d 2d2d 2d2d 0a20 2020 2063 635f 6172  ------.    cc_ar
+00010590: 7261 793a 206e 756d 7079 2e6e 6461 7272  ray: numpy.ndarr
+000105a0: 6179 2063 6f6e 7461 696e 7320 7468 6520  ay contains the 
+000105b0: 3244 2063 726f 7373 2063 6f72 7265 6c61  2D cross correla
+000105c0: 7469 6f6e 206d 6174 7269 780a 2020 2020  tion matrix.    
+000105d0: 706f 7765 723a 206e 702e 696e 742c 206e  power: np.int, n
+000105e0: 7468 2072 6f6f 7420 666f 7220 7468 6520  th root for the 
+000105f0: 7374 6163 6b69 6e67 0a0a 2020 2020 5265  stacking..    Re
+00010600: 7475 726e 733a 0a20 2020 202d 2d2d 2d2d  turns:.    -----
+00010610: 2d2d 2d2d 2d2d 2d0a 2020 2020 6e73 7461  -------.    nsta
+00010620: 636b 3a20 6e70 2e6e 6461 7272 6179 2c20  ck: np.ndarray, 
+00010630: 6669 6e61 6c20 7374 6163 6b65 6420 7761  final stacked wa
+00010640: 7665 666f 726d 730a 0a20 2020 2057 7269  veforms..    Wri
+00010650: 7474 656e 2062 7920 4368 656e 6778 696e  tten by Chengxin
+00010660: 204a 6961 6e67 2040 414e 5520 284d 6179   Jiang @ANU (May
+00010670: 3230 3230 290a 2020 2020 2222 220a 2020  2020).    """.  
+00010680: 2020 6966 2063 635f 6172 7261 792e 6e64    if cc_array.nd
+00010690: 696d 203d 3d20 313a 0a20 2020 2020 2020  im == 1:.       
+000106a0: 206c 6f67 6765 722e 6465 6275 6728 2232   logger.debug("2
+000106b0: 4420 6d61 7472 6978 2069 7320 6e65 6564  D matrix is need
+000106c0: 6564 2066 6f72 206e 726f 6f74 5f73 7461  ed for nroot_sta
+000106d0: 636b 2229 0a20 2020 2020 2020 2072 6574  ck").        ret
+000106e0: 7572 6e20 6363 5f61 7272 6179 0a20 2020  urn cc_array.   
+000106f0: 204e 2c20 4d20 3d20 6363 5f61 7272 6179   N, M = cc_array
+00010700: 2e73 6861 7065 0a20 2020 2064 6f75 7420  .shape.    dout 
+00010710: 3d20 6e70 2e7a 6572 6f73 284d 2c20 6474  = np.zeros(M, dt
+00010720: 7970 653d 6e70 2e66 6c6f 6174 3332 290a  ype=np.float32).
+00010730: 0a20 2020 2023 2063 6f6e 7374 7275 6374  .    # construct
+00010740: 2079 0a20 2020 2066 6f72 2069 6920 696e   y.    for ii in
+00010750: 2072 616e 6765 284e 293a 0a20 2020 2020   range(N):.     
+00010760: 2020 2064 6174 203d 2063 635f 6172 7261     dat = cc_arra
+00010770: 795b 6969 2c20 3a5d 0a20 2020 2020 2020  y[ii, :].       
+00010780: 2064 6f75 7420 2b3d 206e 702e 7369 676e   dout += np.sign
+00010790: 2864 6174 2920 2a20 6e70 2e61 6273 2864  (dat) * np.abs(d
+000107a0: 6174 2920 2a2a 2028 3120 2f20 706f 7765  at) ** (1 / powe
+000107b0: 7229 0a20 2020 2064 6f75 7420 2f3d 204e  r).    dout /= N
+000107c0: 0a0a 2020 2020 2320 7468 6520 6669 6e61  ..    # the fina
+000107d0: 6c20 7374 6163 6b65 6420 7761 7665 666f  l stacked wavefo
+000107e0: 726d 0a20 2020 206e 7374 6163 6b20 3d20  rm.    nstack = 
+000107f0: 646f 7574 202a 206e 702e 6162 7328 646f  dout * np.abs(do
+00010800: 7574 2920 2a2a 2028 706f 7765 7220 2d20  ut) ** (power - 
+00010810: 3129 0a0a 2020 2020 7265 7475 726e 206e  1)..    return n
+00010820: 7374 6163 6b0a 0a0a 6465 6620 7365 6c65  stack...def sele
+00010830: 6374 6976 655f 7374 6163 6b28 6363 5f61  ctive_stack(cc_a
+00010840: 7272 6179 2c20 6570 7369 6c6f 6e2c 2063  rray, epsilon, c
+00010850: 635f 7468 293a 2020 2320 6e6f 7161 3a20  c_th):  # noqa: 
+00010860: 4638 3131 0a20 2020 2022 2222 0a20 2020  F811.    """.   
+00010870: 2074 6869 7320 6973 2061 2073 656c 6563   this is a selec
+00010880: 7469 7665 2073 7461 636b 696e 6720 616c  tive stacking al
+00010890: 676f 7269 7468 6d20 6465 7665 6c6f 7065  gorithm develope
+000108a0: 6420 6279 204a 6172 6564 2042 7279 616e  d by Jared Bryan
+000108b0: 2f4b 7572 616d 6120 4f6b 7562 6f2e 0a0a  /Kurama Okubo...
+000108c0: 2020 2020 5041 5241 4d45 5445 5253 3a0a      PARAMETERS:.
+000108d0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+000108e0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2063  ----------.    c
+000108f0: 635f 6172 7261 793a 206e 756d 7079 2e6e  c_array: numpy.n
+00010900: 6461 7272 6179 2063 6f6e 7461 696e 7320  darray contains 
+00010910: 7468 6520 3244 2063 726f 7373 2063 6f72  the 2D cross cor
+00010920: 7265 6c61 7469 6f6e 206d 6174 7269 780a  relation matrix.
+00010930: 2020 2020 6570 7369 6c6f 6e3a 2072 6573      epsilon: res
+00010940: 6964 7561 6c20 7468 7265 686f 6c64 2074  idual threhold t
+00010950: 6f20 7175 6974 2074 6865 2069 7465 7261  o quit the itera
+00010960: 7469 6f6e 0a20 2020 2063 635f 7468 3a20  tion.    cc_th: 
+00010970: 6e75 6d70 792e 666c 6f61 742c 2074 6872  numpy.float, thr
+00010980: 6573 686f 6c64 206f 6620 636f 7272 656c  eshold of correl
+00010990: 6174 696f 6e20 636f 6566 6669 6369 656e  ation coefficien
+000109a0: 7420 746f 2062 6520 7365 6c65 6374 6564  t to be selected
+000109b0: 0a0a 2020 2020 5245 5455 524e 533a 0a20  ..    RETURNS:. 
+000109c0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+000109d0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6e65  ---------.    ne
+000109e0: 7773 7461 636b 3a20 6e75 6d70 7920 7665  wstack: numpy ve
+000109f0: 6374 6f72 2063 6f6e 7461 696e 7320 7468  ctor contains th
+00010a00: 6520 7374 6163 6b65 6420 6372 6f73 7320  e stacked cross 
+00010a10: 636f 7272 656c 6174 696f 6e0a 2020 2020  correlation.    
+00010a20: 6e73 7465 703a 206e 702e 696e 742c 2074  nstep: np.int, t
+00010a30: 6f74 616c 206e 756d 6265 7220 6f66 2069  otal number of i
+00010a40: 7465 7261 7469 6f6e 7320 666f 7220 7468  terations for th
+00010a50: 6520 7374 6163 6b69 6e67 0a0a 2020 2020  e stacking..    
+00010a60: 4f72 6967 696e 616c 6c79 2072 6974 7465  Originally ritte
+00010a70: 6e20 6279 204d 6172 696e 6520 4465 6e6f  n by Marine Deno
+00010a80: 6c6c 650a 2020 2020 4d6f 6469 6669 6564  lle.    Modified
+00010a90: 2062 7920 4368 656e 6778 696e 204a 6961   by Chengxin Jia
+00010aa0: 6e67 2040 4861 7276 6172 6420 284f 6374  ng @Harvard (Oct
+00010ab0: 3230 3230 290a 2020 2020 2222 220a 2020  2020).    """.  
+00010ac0: 2020 6966 2063 635f 6172 7261 792e 6e64    if cc_array.nd
+00010ad0: 696d 203d 3d20 313a 0a20 2020 2020 2020  im == 1:.       
+00010ae0: 206c 6f67 6765 722e 6465 6275 6728 2232   logger.debug("2
+00010af0: 4420 6d61 7472 6978 2069 7320 6e65 6564  D matrix is need
+00010b00: 6564 2066 6f72 206e 726f 6f74 5f73 7461  ed for nroot_sta
+00010b10: 636b 2229 0a20 2020 2020 2020 2072 6574  ck").        ret
+00010b20: 7572 6e20 6363 5f61 7272 6179 0a20 2020  urn cc_array.   
+00010b30: 204e 2c20 4d20 3d20 6363 5f61 7272 6179   N, M = cc_array
+00010b40: 2e73 6861 7065 0a0a 2020 2020 7265 7320  .shape..    res 
+00010b50: 3d20 3965 3920 2023 2072 6573 6964 7561  = 9e9  # residua
+00010b60: 6c73 0a20 2020 2063 6f66 203d 206e 702e  ls.    cof = np.
+00010b70: 7a65 726f 7328 4e2c 2064 7479 7065 3d6e  zeros(N, dtype=n
+00010b80: 702e 666c 6f61 7433 3229 0a20 2020 206e  p.float32).    n
+00010b90: 6577 7374 6163 6b20 3d20 6e70 2e6d 6561  ewstack = np.mea
+00010ba0: 6e28 6363 5f61 7272 6179 2c20 6178 6973  n(cc_array, axis
+00010bb0: 3d30 290a 0a20 2020 206e 7374 6570 203d  =0)..    nstep =
+00010bc0: 2030 0a20 2020 2023 2073 7461 7274 2069   0.    # start i
+00010bd0: 7465 7261 7469 6f6e 0a20 2020 2077 6869  teration.    whi
+00010be0: 6c65 2072 6573 203e 2065 7073 696c 6f6e  le res > epsilon
+00010bf0: 3a0a 2020 2020 2020 2020 666f 7220 6969  :.        for ii
+00010c00: 2069 6e20 7261 6e67 6528 4e29 3a0a 2020   in range(N):.  
+00010c10: 2020 2020 2020 2020 2020 636f 665b 6969            cof[ii
+00010c20: 5d20 3d20 6e70 2e63 6f72 7263 6f65 6628  ] = np.corrcoef(
+00010c30: 6e65 7773 7461 636b 2c20 6363 5f61 7272  newstack, cc_arr
+00010c40: 6179 5b69 692c 203a 5d29 5b30 2c20 315d  ay[ii, :])[0, 1]
+00010c50: 0a0a 2020 2020 2020 2020 2320 6669 6e64  ..        # find
+00010c60: 2067 6f6f 6420 7761 7665 666f 726d 730a   good waveforms.
+00010c70: 2020 2020 2020 2020 696e 6478 203d 206e          indx = n
+00010c80: 702e 7768 6572 6528 636f 6620 3e3d 2063  p.where(cof >= c
+00010c90: 635f 7468 295b 305d 0a20 2020 2020 2020  c_th)[0].       
+00010ca0: 2069 6620 6e6f 7420 6c65 6e28 696e 6478   if not len(indx
+00010cb0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00010cc0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00010cd0: 2263 616e 6e6f 7420 6669 6e64 2067 6f6f  "cannot find goo
+00010ce0: 6420 7761 7665 666f 726d 7320 696e 7369  d waveforms insi
+00010cf0: 6465 2073 656c 6563 7469 7665 2073 7461  de selective sta
+00010d00: 636b 696e 6722 290a 2020 2020 2020 2020  cking").        
+00010d10: 6f6c 6473 7461 636b 203d 206e 6577 7374  oldstack = newst
+00010d20: 6163 6b0a 2020 2020 2020 2020 6e65 7773  ack.        news
+00010d30: 7461 636b 203d 206e 702e 6d65 616e 2863  tack = np.mean(c
+00010d40: 635f 6172 7261 795b 696e 6478 5d2c 2061  c_array[indx], a
+00010d50: 7869 733d 3029 0a20 2020 2020 2020 2072  xis=0).        r
+00010d60: 6573 203d 206e 702e 6c69 6e61 6c67 2e6e  es = np.linalg.n
+00010d70: 6f72 6d28 6e65 7773 7461 636b 202d 206f  orm(newstack - o
+00010d80: 6c64 7374 6163 6b29 202f 2028 6e70 2e6c  ldstack) / (np.l
+00010d90: 696e 616c 672e 6e6f 726d 286e 6577 7374  inalg.norm(newst
+00010da0: 6163 6b29 202a 204d 290a 2020 2020 2020  ack) * M).      
+00010db0: 2020 6e73 7465 7020 2b3d 2031 0a0a 2020    nstep += 1..  
+00010dc0: 2020 7265 7475 726e 206e 6577 7374 6163    return newstac
+00010dd0: 6b2c 206e 7374 6570 0a0a 0a64 6566 2067  k, nstep...def g
+00010de0: 6574 5f63 6328 7331 2c20 735f 7265 6629  et_cc(s1, s_ref)
+00010df0: 3a0a 2020 2020 2320 7265 7475 726e 7320  :.    # returns 
+00010e00: 7468 6520 636f 7272 656c 6174 696f 6e20  the correlation 
+00010e10: 636f 6566 6669 6369 656e 7420 6265 7477  coefficient betw
+00010e20: 6565 6e20 7761 7665 666f 726d 7320 696e  een waveforms in
+00010e30: 2073 3120 6167 6169 6e73 7420 7265 6665   s1 against refe
+00010e40: 7265 6e63 650a 2020 2020 2320 7761 7665  rence.    # wave
+00010e50: 666f 726d 2073 5f72 6566 2e0a 2020 2020  form s_ref..    
+00010e60: 230a 2020 2020 6363 203d 206e 702e 7a65  #.    cc = np.ze
+00010e70: 726f 7328 7331 2e73 6861 7065 5b30 5d29  ros(s1.shape[0])
+00010e80: 0a20 2020 2073 5f72 6566 5f6e 6f72 6d20  .    s_ref_norm 
+00010e90: 3d20 6e70 2e6c 696e 616c 672e 6e6f 726d  = np.linalg.norm
+00010ea0: 2873 5f72 6566 290a 2020 2020 666f 7220  (s_ref).    for 
+00010eb0: 6920 696e 2072 616e 6765 2873 312e 7368  i in range(s1.sh
+00010ec0: 6170 655b 305d 293a 0a20 2020 2020 2020  ape[0]):.       
+00010ed0: 2063 635b 695d 203d 206e 702e 7375 6d28   cc[i] = np.sum(
+00010ee0: 6e70 2e6d 756c 7469 706c 7928 7331 5b69  np.multiply(s1[i
+00010ef0: 2c20 3a5d 2c20 735f 7265 6629 2920 2f20  , :], s_ref)) / 
+00010f00: 6e70 2e6c 696e 616c 672e 6e6f 726d 2873  np.linalg.norm(s
+00010f10: 315b 692c 203a 5d29 202f 2073 5f72 6566  1[i, :]) / s_ref
+00010f20: 5f6e 6f72 6d0a 2020 2020 7265 7475 726e  _norm.    return
+00010f30: 2063 630a 0a0a 2323 2323 2323 2323 2323   cc...##########
+00010f40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010f50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010f60: 2323 2323 2323 2323 2323 2323 2323 0a23  ##############.#
+00010f70: 2323 2323 2323 2323 2323 2323 2323 2320  ############### 
+00010f80: 4d4f 4e49 544f 5249 4e47 2046 554e 4354  MONITORING FUNCT
+00010f90: 494f 4e53 2023 2323 2323 2323 2323 2323  IONS ###########
+00010fa0: 2323 2323 2323 230a 2323 2323 2323 2323  #######.########
+00010fb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010fc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010fd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010fe0: 0a0a 2222 220a 6120 636f 6d70 696c 6174  ..""".a compilat
+00010ff0: 696f 6e20 6f66 2061 6c6c 2061 7661 696c  ion of all avail
+00011000: 6162 6c65 2063 6f72 6520 6675 6e63 7469  able core functi
+00011010: 6f6e 7320 666f 7220 636f 6d70 7574 696e  ons for computin
+00011020: 6720 7068 6173 6520 6465 6c61 7973 2062  g phase delays b
+00011030: 6173 6564 206f 6e20 616d 6269 656e 7420  ased on ambient 
+00011040: 6e6f 6973 6520 696e 7465 7266 6572 6f6d  noise interferom
+00011050: 6574 7279 0a0a 7175 6963 6b20 696e 6465  etry..quick inde
+00011060: 7820 6f66 2064 762f 7620 6d65 7468 6f64  x of dv/v method
+00011070: 733a 0a31 2920 7374 7265 7463 6869 6e67  s:.1) stretching
+00011080: 2028 7469 6d65 2073 7472 6574 6368 696e   (time stretchin
+00011090: 673b 2057 6561 7665 7220 6574 2061 6c20  g; Weaver et al 
+000110a0: 2832 3031 3129 290a 3229 2064 7477 5f64  (2011)).2) dtw_d
+000110b0: 7676 2028 4479 6e61 6d69 6320 5469 6d65  vv (Dynamic Time
+000110c0: 2057 6172 7069 6e67 3b20 4d69 6b65 7365   Warping; Mikese
+000110d0: 6c6c 2065 7420 616c 2e20 3230 3135 290a  ll et al. 2015).
+000110e0: 3329 206d 7763 735f 6476 7620 284d 6f76  3) mwcs_dvv (Mov
+000110f0: 696e 6720 5769 6e64 6f77 2043 726f 7373  ing Window Cross
+00011100: 2053 7065 6374 7275 6d3b 2043 6c61 726b   Spectrum; Clark
+00011110: 2065 7420 616c 2e2c 2032 3031 3129 0a34   et al., 2011).4
+00011120: 2920 6d77 6363 5f64 7676 2028 4d6f 7669  ) mwcc_dvv (Movi
+00011130: 6e67 2057 696e 646f 7720 4372 6f73 7320  ng Window Cross 
+00011140: 436f 7272 656c 6174 696f 6e3b 2053 6e69  Correlation; Sni
+00011150: 6564 6572 2065 7420 616c 2e2c 2032 3031  eder et al., 201
+00011160: 3229 0a35 2920 7774 735f 6476 7620 2857  2).5) wts_dvv (W
+00011170: 6176 656c 6574 2053 7472 6563 6869 6e67  avelet Streching
+00011180: 3b20 5975 616e 2065 7420 616c 2e2c 2069  ; Yuan et al., i
+00011190: 6e20 7072 6570 290a 3629 2077 7873 5f64  n prep).6) wxs_d
+000111a0: 7676 2028 5761 7665 6c65 7420 5872 6f73  vv (Wavelet Xros
+000111b0: 7320 5370 6563 7472 756d 3b20 4d61 6f20  s Spectrum; Mao 
+000111c0: 6574 2061 6c2e 2c20 3230 3139 290a 3729  et al., 2019).7)
+000111d0: 2077 6477 5f64 7676 2028 5761 7665 6c65   wdw_dvv (Wavele
+000111e0: 7420 4479 6e61 6d69 6320 5761 7270 696e  t Dynamic Warpin
+000111f0: 673b 2059 7561 6e20 6574 2061 6c2e 2c20  g; Yuan et al., 
+00011200: 696e 2070 7265 7029 0a22 2222 0a0a 0a64  in prep)."""...d
+00011210: 6566 2073 7472 6574 6368 696e 6728 7265  ef stretching(re
+00011220: 662c 2063 7572 2c20 6476 5f72 616e 6765  f, cur, dv_range
+00011230: 2c20 6e62 7472 6961 6c2c 2070 6172 6129  , nbtrial, para)
+00011240: 3a0a 2020 2020 2222 220a 2020 2020 5468  :.    """.    Th
+00011250: 6973 2066 756e 6374 696f 6e20 636f 6d70  is function comp
+00011260: 6172 6573 2074 6865 2052 6566 6572 656e  ares the Referen
+00011270: 6365 2077 6176 6566 6f72 6d20 746f 2073  ce waveform to s
+00011280: 7472 6574 6368 6564 2f63 6f6d 7072 6573  tretched/compres
+00011290: 7365 6420 6375 7272 656e 7420 7761 7665  sed current wave
+000112a0: 666f 726d 7320 746f 2067 6574 2074 6865  forms to get the
+000112b0: 0a20 2020 2072 656c 6174 6976 6520 7365  .    relative se
+000112c0: 6973 6d69 6320 7665 6c6f 6369 7479 2076  ismic velocity v
+000112d0: 6172 6961 7469 6f6e 2028 616e 6420 6173  ariation (and as
+000112e0: 736f 6369 6174 6564 2065 7272 6f72 292e  sociated error).
+000112f0: 0a20 2020 2049 7420 616c 736f 2063 6f6d  .    It also com
+00011300: 7075 7465 7320 7468 6520 636f 7272 656c  putes the correl
+00011310: 6174 696f 6e20 636f 6566 6669 6369 656e  ation coefficien
+00011320: 7420 6265 7477 6565 6e20 7468 6520 5265  t between the Re
+00011330: 6665 7265 6e63 6520 7761 7665 666f 726d  ference waveform
+00011340: 2061 6e64 2074 6865 2063 7572 7265 6e74   and the current
+00011350: 2077 6176 6566 6f72 6d2e 0a0a 2020 2020   waveform...    
+00011360: 5041 5241 4d45 5445 5253 3a0a 2020 2020  PARAMETERS:.    
+00011370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011380: 0a20 2020 2072 6566 3a20 5265 6665 7265  .    ref: Refere
+00011390: 6e63 6520 7761 7665 666f 726d 2028 6e70  nce waveform (np
+000113a0: 2e6e 6461 7272 6179 2c20 7369 7a65 204e  .ndarray, size N
+000113b0: 290a 2020 2020 6375 723a 2043 7572 7265  ).    cur: Curre
+000113c0: 6e74 2077 6176 6566 6f72 6d20 286e 702e  nt waveform (np.
+000113d0: 6e64 6172 7261 792c 2073 697a 6520 4e29  ndarray, size N)
+000113e0: 0a20 2020 2064 765f 7261 6e67 653a 2061  .    dv_range: a
+000113f0: 6273 6f6c 7574 6520 626f 756e 6420 666f  bsolute bound fo
+00011400: 7220 7468 6520 7665 6c6f 6369 7479 2076  r the velocity v
+00011410: 6172 6961 7469 6f6e 3b20 6578 616d 706c  ariation; exampl
+00011420: 653a 2064 763d 302e 3033 2066 6f72 205b  e: dv=0.03 for [
+00011430: 2d33 2c33 5d25 0a20 2020 206f 6620 7265  -3,3]%.    of re
+00011440: 6c61 7469 7665 2076 656c 6f63 6974 7920  lative velocity 
+00011450: 6368 616e 6765 2028 2766 6c6f 6174 2729  change ('float')
+00011460: 0a20 2020 206e 6274 7269 616c 3a20 6e75  .    nbtrial: nu
+00011470: 6d62 6572 206f 6620 7374 7265 7463 6869  mber of stretchi
+00011480: 6e67 2063 6f65 6666 6963 6965 6e74 2062  ng coefficient b
+00011490: 6574 7765 656e 2064 766d 696e 2061 6e64  etween dvmin and
+000114a0: 2064 766d 6178 2c20 6e6f 206e 6565 6420   dvmax, no need 
+000114b0: 746f 2062 6520 6869 6768 6572 2074 6861  to be higher tha
+000114c0: 6e20 3130 3020 2028 2766 6c6f 6174 2729  n 100  ('float')
+000114d0: 0a20 2020 2070 6172 613a 2076 6563 746f  .    para: vecto
+000114e0: 7220 6f66 2074 6865 2069 6e64 6963 6573  r of the indices
+000114f0: 206f 6620 7468 6520 6375 7220 616e 6420   of the cur and 
+00011500: 7265 6620 7769 6e64 6f77 7320 6f6e 2077  ref windows on w
+00011510: 6963 6820 796f 7520 7761 6e74 2074 6f20  ich you want to 
+00011520: 646f 2074 6865 206d 6561 7375 7265 6d65  do the measureme
+00011530: 6e74 730a 2020 2020 286e 702e 6e64 6172  nts.    (np.ndar
+00011540: 7261 792c 2073 697a 6520 746d 696e 2a64  ray, size tmin*d
+00011550: 656c 7461 3a74 6d61 782a 6465 6c74 6129  elta:tmax*delta)
+00011560: 0a20 2020 2046 6f72 2065 7272 6f72 2063  .    For error c
+00011570: 6f6d 7075 7461 7469 6f6e 2c20 7765 206e  omputation, we n
+00011580: 6565 6420 7061 7261 6d65 7465 7273 3a0a  eed parameters:.
+00011590: 2020 2020 2020 2020 666d 696e 3a20 6d69          fmin: mi
+000115a0: 6e69 6d75 6d20 6672 6571 7565 6e63 7920  nimum frequency 
+000115b0: 6f66 2074 6865 2064 6174 610a 2020 2020  of the data.    
+000115c0: 2020 2020 666d 6178 3a20 6d61 7869 6d75      fmax: maximu
+000115d0: 6d20 6672 6571 7565 6e63 7920 6f66 2074  m frequency of t
+000115e0: 6865 2064 6174 610a 2020 2020 2020 2020  he data.        
+000115f0: 746d 696e 3a20 6d69 6e69 6d75 6d20 7469  tmin: minimum ti
+00011600: 6d65 2077 696e 646f 7720 7768 6572 6520  me window where 
+00011610: 7468 6520 6476 2f76 2069 7320 636f 6d70  the dv/v is comp
+00011620: 7574 6564 0a20 2020 2020 2020 2074 6d61  uted.        tma
+00011630: 783a 206d 6178 696d 756d 2074 696d 6520  x: maximum time 
+00011640: 7769 6e64 6f77 2077 6865 7265 2074 6865  window where the
+00011650: 2064 762f 7620 6973 2063 6f6d 7075 7465   dv/v is compute
+00011660: 640a 2020 2020 5245 5455 524e 533a 0a20  d.    RETURNS:. 
+00011670: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+00011680: 2d2d 2d0a 2020 2020 6476 3a20 5265 6c61  ---.    dv: Rela
+00011690: 7469 7665 2076 656c 6f63 6974 7920 6368  tive velocity ch
+000116a0: 616e 6765 2064 762f 7620 2869 6e20 2529  ange dv/v (in %)
+000116b0: 0a20 2020 2063 633a 2063 6f72 7265 6c61  .    cc: correla
+000116c0: 7469 6f6e 2063 6f65 6666 6963 6965 6e74  tion coefficient
+000116d0: 2062 6574 7765 656e 2074 6865 2072 6566   between the ref
+000116e0: 6572 656e 6365 2077 6176 6566 6f72 6d20  erence waveform 
+000116f0: 616e 6420 7468 6520 6265 7374 2073 7472  and the best str
+00011700: 6574 6368 6564 2f63 6f6d 7072 6573 7365  etched/compresse
+00011710: 6420 6375 7272 656e 7420 7761 7665 666f  d current wavefo
+00011720: 726d 0a20 2020 2063 6470 3a20 636f 7272  rm.    cdp: corr
+00011730: 656c 6174 696f 6e20 636f 6566 6669 6369  elation coeffici
+00011740: 656e 7420 6265 7477 6565 6e20 7468 6520  ent between the 
+00011750: 7265 6665 7265 6e63 6520 7761 7665 666f  reference wavefo
+00011760: 726d 2061 6e64 2074 6865 2069 6e69 7469  rm and the initi
+00011770: 616c 2063 7572 7265 6e74 2077 6176 6566  al current wavef
+00011780: 6f72 6d0a 2020 2020 6572 726f 723a 2045  orm.    error: E
+00011790: 7272 6f72 7320 696e 2074 6865 2064 762f  rrors in the dv/
+000117a0: 7620 6d65 6173 7572 656d 656e 7473 2062  v measurements b
+000117b0: 6173 6564 206f 6e20 5765 6176 6572 2065  ased on Weaver e
+000117c0: 7420 616c 2028 3230 3131 292c 0a20 2020  t al (2011),.   
+000117d0: 204f 6e20 7468 6520 7072 6563 6973 696f   On the precisio
+000117e0: 6e20 6f66 206e 6f69 7365 2d63 6f72 7265  n of noise-corre
+000117f0: 6c61 7469 6f6e 2069 6e74 6572 6665 726f  lation interfero
+00011800: 6d65 7472 792c 2047 656f 7068 7973 2e20  metry, Geophys. 
+00011810: 4a2e 2049 6e74 2e2c 2031 3835 2833 290a  J. Int., 185(3).
+00011820: 0a20 2020 204e 6f74 653a 2054 6865 2063  .    Note: The c
+00011830: 6f64 6520 6669 7273 7420 6669 6e64 7320  ode first finds 
+00011840: 7468 6520 6265 7374 2063 6f72 7265 6c61  the best correla
+00011850: 7469 6f6e 2063 6f65 6666 6963 6965 6e74  tion coefficient
+00011860: 2062 6574 7765 656e 2074 6865 2052 6566   between the Ref
+00011870: 6572 656e 6365 2077 6176 6566 6f72 6d20  erence waveform 
+00011880: 616e 640a 2020 2020 7468 6520 7374 7265  and.    the stre
+00011890: 7463 6865 642f 636f 6d70 7265 7373 6564  tched/compressed
+000118a0: 2063 7572 7265 6e74 2077 6176 6566 6f72   current wavefor
+000118b0: 6d20 616d 6f6e 6720 7468 6520 226e 6274  m among the "nbt
+000118c0: 7269 616c 2220 7661 6c75 6573 2e0a 2020  rial" values..  
+000118d0: 2020 4120 7265 6669 6e65 6420 616e 616c    A refined anal
+000118e0: 7973 6973 2069 7320 7468 656e 2070 6572  ysis is then per
+000118f0: 666f 726d 6564 2061 726f 756e 6420 7468  formed around th
+00011900: 6973 2076 616c 7565 2074 6f20 6f62 7461  is value to obta
+00011910: 696e 2061 206d 6f72 6520 7072 6563 6973  in a more precis
+00011920: 6520 6476 2f76 206d 6561 7375 7265 6d65  e dv/v measureme
+00011930: 6e74 202e 0a0a 2020 2020 4f72 6967 696e  nt ...    Origin
+00011940: 616c 6c79 2062 7920 4c2e 2056 6965 6e73  ally by L. Viens
+00011950: 2030 342f 3236 2f32 3031 3820 2856 6965   04/26/2018 (Vie
+00011960: 6e73 2065 7420 616c 2e2c 2032 3031 3820  ns et al., 2018 
+00011970: 4a47 5229 0a20 2020 206d 6f64 6966 6965  JGR).    modifie
+00011980: 6420 6279 2043 6865 6e67 7869 6e20 4a69  d by Chengxin Ji
+00011990: 616e 670a 2020 2020 2222 220a 2020 2020  ang.    """.    
+000119a0: 2320 6c6f 6164 2063 6f6d 6d6f 6e20 7661  # load common va
+000119b0: 7269 6162 6c65 7320 6672 6f6d 2064 6963  riables from dic
+000119c0: 7469 6f6e 6172 790a 2020 2020 7477 696e  tionary.    twin
+000119d0: 203d 2070 6172 615b 2274 7769 6e22 5d0a   = para["twin"].
+000119e0: 2020 2020 6672 6571 203d 2070 6172 615b      freq = para[
+000119f0: 2266 7265 7122 5d0a 2020 2020 6474 203d  "freq"].    dt =
+00011a00: 2070 6172 615b 2264 7422 5d0a 2020 2020   para["dt"].    
+00011a10: 746d 696e 203d 206e 702e 6d69 6e28 7477  tmin = np.min(tw
+00011a20: 696e 290a 2020 2020 746d 6178 203d 206e  in).    tmax = n
+00011a30: 702e 6d61 7828 7477 696e 290a 2020 2020  p.max(twin).    
+00011a40: 666d 696e 203d 206e 702e 6d69 6e28 6672  fmin = np.min(fr
+00011a50: 6571 290a 2020 2020 666d 6178 203d 206e  eq).    fmax = n
+00011a60: 702e 6d61 7828 6672 6571 290a 2020 2020  p.max(freq).    
+00011a70: 7476 6563 203d 206e 702e 6172 616e 6765  tvec = np.arange
+00011a80: 2874 6d69 6e2c 2074 6d61 782c 2064 7429  (tmin, tmax, dt)
+00011a90: 0a0a 2020 2020 2320 6d61 6b65 2075 7365  ..    # make use
+00011aa0: 6675 6c20 6f6e 6520 666f 7220 6d65 6173  ful one for meas
+00011ab0: 7572 656d 656e 7473 0a20 2020 2064 766d  urements.    dvm
+00011ac0: 696e 203d 202d 6e70 2e61 6273 2864 765f  in = -np.abs(dv_
+00011ad0: 7261 6e67 6529 0a20 2020 2064 766d 6178  range).    dvmax
+00011ae0: 203d 206e 702e 6162 7328 6476 5f72 616e   = np.abs(dv_ran
+00011af0: 6765 290a 2020 2020 4570 7320 3d20 3120  ge).    Eps = 1 
+00011b00: 2b20 286e 702e 6c69 6e73 7061 6365 2864  + (np.linspace(d
+00011b10: 766d 696e 2c20 6476 6d61 782c 206e 6274  vmin, dvmax, nbt
+00011b20: 7269 616c 2929 0a20 2020 2063 6f66 203d  rial)).    cof =
+00011b30: 206e 702e 7a65 726f 7328 4570 732e 7368   np.zeros(Eps.sh
+00011b40: 6170 652c 2064 7479 7065 3d6e 702e 666c  ape, dtype=np.fl
+00011b50: 6f61 7433 3229 0a0a 2020 2020 2320 5365  oat32)..    # Se
+00011b60: 7420 6f66 2073 7472 6574 6368 6564 2f63  t of stretched/c
+00011b70: 6f6d 7072 6573 7365 6420 6375 7272 656e  ompressed curren
+00011b80: 7420 7761 7665 666f 726d 730a 2020 2020  t waveforms.    
+00011b90: 666f 7220 6969 2069 6e20 7261 6e67 6528  for ii in range(
+00011ba0: 6c65 6e28 4570 7329 293a 0a20 2020 2020  len(Eps)):.     
+00011bb0: 2020 206e 7420 3d20 7476 6563 202a 2045     nt = tvec * E
+00011bc0: 7073 5b69 695d 0a20 2020 2020 2020 2073  ps[ii].        s
+00011bd0: 203d 206e 702e 696e 7465 7270 2878 3d74   = np.interp(x=t
+00011be0: 7665 632c 2078 703d 6e74 2c20 6670 3d63  vec, xp=nt, fp=c
+00011bf0: 7572 290a 2020 2020 2020 2020 7761 7665  ur).        wave
+00011c00: 666f 726d 5f72 6566 203d 2072 6566 0a20  form_ref = ref. 
+00011c10: 2020 2020 2020 2077 6176 6566 6f72 6d5f         waveform_
+00011c20: 6375 7220 3d20 730a 2020 2020 2020 2020  cur = s.        
+00011c30: 636f 665b 6969 5d20 3d20 6e70 2e63 6f72  cof[ii] = np.cor
+00011c40: 7263 6f65 6628 7761 7665 666f 726d 5f72  rcoef(waveform_r
+00011c50: 6566 2c20 7761 7665 666f 726d 5f63 7572  ef, waveform_cur
+00011c60: 295b 302c 2031 5d0a 0a20 2020 2063 6470  )[0, 1]..    cdp
+00011c70: 203d 206e 702e 636f 7272 636f 6566 2863   = np.corrcoef(c
+00011c80: 7572 2c20 7265 6629 5b30 2c20 315d 2020  ur, ref)[0, 1]  
+00011c90: 2320 636f 7272 656c 6174 696f 6e20 636f  # correlation co
+00011ca0: 6566 6669 6369 656e 7420 6265 7477 6565  efficient betwee
+00011cb0: 6e20 7468 6520 7265 6665 7265 6e63 6520  n the reference 
+00011cc0: 616e 6420 696e 6974 6961 6c20 6375 7272  and initial curr
+00011cd0: 656e 7420 7761 7665 666f 726d 730a 0a20  ent waveforms.. 
+00011ce0: 2020 2023 2066 696e 6420 7468 6520 6d61     # find the ma
+00011cf0: 7869 6d75 6d20 636f 7272 656c 6174 696f  ximum correlatio
+00011d00: 6e20 636f 6566 6669 6369 656e 740a 2020  n coefficient.  
+00011d10: 2020 696d 6178 203d 206e 702e 6e61 6e61    imax = np.nana
+00011d20: 7267 6d61 7828 636f 6629 0a20 2020 2069  rgmax(cof).    i
+00011d30: 6620 696d 6178 203e 3d20 6c65 6e28 4570  f imax >= len(Ep
+00011d40: 7329 202d 2032 3a0a 2020 2020 2020 2020  s) - 2:.        
+00011d50: 696d 6178 203d 2069 6d61 7820 2d20 320a  imax = imax - 2.
+00011d60: 2020 2020 6966 2069 6d61 7820 3c3d 2032      if imax <= 2
+00011d70: 3a0a 2020 2020 2020 2020 696d 6178 203d  :.        imax =
+00011d80: 2069 6d61 7820 2b20 320a 0a20 2020 2023   imax + 2..    #
+00011d90: 2050 726f 6365 6564 2074 6f20 7468 6520   Proceed to the 
+00011da0: 7365 636f 6e64 2073 7465 7020 746f 2067  second step to g
+00011db0: 6574 2061 206d 6f72 6520 7072 6563 6973  et a more precis
+00011dc0: 6520 6476 2f76 206d 6561 7375 7265 6d65  e dv/v measureme
+00011dd0: 6e74 0a20 2020 2064 7466 696e 6572 203d  nt.    dtfiner =
+00011de0: 206e 702e 6c69 6e73 7061 6365 2845 7073   np.linspace(Eps
+00011df0: 5b69 6d61 7820 2d20 325d 2c20 4570 735b  [imax - 2], Eps[
+00011e00: 696d 6178 202b 2032 5d2c 2031 3030 290a  imax + 2], 100).
+00011e10: 2020 2020 6e63 6f66 203d 206e 702e 7a65      ncof = np.ze
+00011e20: 726f 7328 6474 6669 6e65 722e 7368 6170  ros(dtfiner.shap
+00011e30: 652c 2064 7479 7065 3d6e 702e 666c 6f61  e, dtype=np.floa
+00011e40: 7433 3229 0a20 2020 2066 6f72 2069 6920  t32).    for ii 
+00011e50: 696e 2072 616e 6765 286c 656e 2864 7466  in range(len(dtf
+00011e60: 696e 6572 2929 3a0a 2020 2020 2020 2020  iner)):.        
+00011e70: 6e74 203d 2074 7665 6320 2a20 6474 6669  nt = tvec * dtfi
+00011e80: 6e65 725b 6969 5d0a 2020 2020 2020 2020  ner[ii].        
+00011e90: 7320 3d20 6e70 2e69 6e74 6572 7028 783d  s = np.interp(x=
+00011ea0: 7476 6563 2c20 7870 3d6e 742c 2066 703d  tvec, xp=nt, fp=
+00011eb0: 6375 7229 0a20 2020 2020 2020 2077 6176  cur).        wav
+00011ec0: 6566 6f72 6d5f 7265 6620 3d20 7265 660a  eform_ref = ref.
+00011ed0: 2020 2020 2020 2020 7761 7665 666f 726d          waveform
+00011ee0: 5f63 7572 203d 2073 0a20 2020 2020 2020  _cur = s.       
+00011ef0: 206e 636f 665b 6969 5d20 3d20 6e70 2e63   ncof[ii] = np.c
+00011f00: 6f72 7263 6f65 6628 7761 7665 666f 726d  orrcoef(waveform
+00011f10: 5f72 6566 2c20 7761 7665 666f 726d 5f63  _ref, waveform_c
+00011f20: 7572 295b 302c 2031 5d0a 0a20 2020 2063  ur)[0, 1]..    c
+00011f30: 6320 3d20 6e70 2e6d 6178 286e 636f 6629  c = np.max(ncof)
+00011f40: 2020 2320 4669 6e64 206d 6178 696d 756d    # Find maximum
+00011f50: 2063 6f72 7265 6c61 7469 6f6e 2063 6f65   correlation coe
+00011f60: 6666 6963 6965 6e74 206f 6620 7468 6520  fficient of the 
+00011f70: 7265 6669 6e65 6420 2061 6e61 6c79 7369  refined  analysi
+00011f80: 730a 2020 2020 6476 203d 2031 3030 2e30  s.    dv = 100.0
+00011f90: 202a 2064 7466 696e 6572 5b6e 702e 6172   * dtfiner[np.ar
+00011fa0: 676d 6178 286e 636f 6629 5d20 2d20 3130  gmax(ncof)] - 10
+00011fb0: 3020 2023 204d 756c 7469 706c 7920 6279  0  # Multiply by
+00011fc0: 2031 3030 2074 6f20 636f 6e76 6572 7420   100 to convert 
+00011fd0: 746f 2070 6572 6365 6e74 6167 6520 2845  to percentage (E
+00011fe0: 7073 696c 6f6e 203d 202d 6474 2f74 203d  psilon = -dt/t =
+00011ff0: 2064 762f 7629 0a0a 2020 2020 2320 4572   dv/v)..    # Er
+00012000: 726f 7220 636f 6d70 7574 6174 696f 6e20  ror computation 
+00012010: 6261 7365 6420 6f6e 2057 6561 7665 7220  based on Weaver 
+00012020: 6574 2061 6c20 2832 3031 3129 2c20 4f6e  et al (2011), On
+00012030: 2074 6865 2070 7265 6369 7369 6f6e 206f   the precision o
+00012040: 6620 6e6f 6973 652d 636f 7272 656c 6174  f noise-correlat
+00012050: 696f 6e0a 2020 2020 2320 696e 7465 7266  ion.    # interf
+00012060: 6572 6f6d 6574 7279 2c20 4765 6f70 6879  erometry, Geophy
+00012070: 732e 204a 2e20 496e 742e 2c20 3138 3528  s. J. Int., 185(
+00012080: 3329 0a20 2020 2054 203d 2031 202f 2028  3).    T = 1 / (
+00012090: 666d 6178 202d 2066 6d69 6e29 0a20 2020  fmax - fmin).   
+000120a0: 2058 203d 2063 630a 2020 2020 7763 203d   X = cc.    wc =
+000120b0: 206e 702e 7069 202a 2028 666d 696e 202b   np.pi * (fmin +
+000120c0: 2066 6d61 7829 0a20 2020 2074 3120 3d20   fmax).    t1 = 
+000120d0: 6e70 2e6d 696e 285b 746d 696e 2c20 746d  np.min([tmin, tm
+000120e0: 6178 5d29 0a20 2020 2074 3220 3d20 6e70  ax]).    t2 = np
+000120f0: 2e6d 6178 285b 746d 696e 2c20 746d 6178  .max([tmin, tmax
+00012100: 5d29 0a20 2020 2065 7272 6f72 203d 2031  ]).    error = 1
+00012110: 3030 202a 2028 0a20 2020 2020 2020 206e  00 * (.        n
+00012120: 702e 7371 7274 2831 202d 2058 2a2a 3229  p.sqrt(1 - X**2)
+00012130: 202f 2028 3220 2a20 5829 202a 206e 702e   / (2 * X) * np.
+00012140: 7371 7274 2828 3620 2a20 6e70 2e73 7172  sqrt((6 * np.sqr
+00012150: 7428 6e70 2e70 6920 2f20 3229 202a 2054  t(np.pi / 2) * T
+00012160: 2920 2f20 2877 632a 2a32 202a 2028 7432  ) / (wc**2 * (t2
+00012170: 2a2a 3320 2d20 7431 2a2a 3329 2929 0a20  **3 - t1**3))). 
+00012180: 2020 2029 0a0a 2020 2020 7265 7475 726e     )..    return
+00012190: 2064 762c 2065 7272 6f72 2c20 6363 2c20   dv, error, cc, 
+000121a0: 6364 700a 0a0a 6465 6620 7374 7265 7463  cdp...def stretc
+000121b0: 6869 6e67 5f76 6563 7428 7265 662c 2063  hing_vect(ref, c
+000121c0: 7572 2c20 6476 5f72 616e 6765 2c20 6e62  ur, dv_range, nb
+000121d0: 7472 6961 6c2c 2070 6172 6129 3a0a 2020  trial, para):.  
+000121e0: 2020 2222 220a 2020 2020 5468 6973 2066    """.    This f
+000121f0: 756e 6374 696f 6e20 636f 6d70 6172 6573  unction compares
+00012200: 2074 6865 2052 6566 6572 656e 6365 2077   the Reference w
+00012210: 6176 6566 6f72 6d20 746f 2073 7472 6574  aveform to stret
+00012220: 6368 6564 2f63 6f6d 7072 6573 7365 6420  ched/compressed 
+00012230: 6375 7272 656e 7420 7761 7665 666f 726d  current waveform
+00012240: 730a 2020 2020 746f 2067 6574 2074 6865  s.    to get the
+00012250: 2072 656c 6174 6976 6520 7365 6973 6d69   relative seismi
+00012260: 6320 7665 6c6f 6369 7479 2076 6172 6961  c velocity varia
+00012270: 7469 6f6e 2028 616e 6420 6173 736f 6369  tion (and associ
+00012280: 6174 6564 2065 7272 6f72 292e 0a20 2020  ated error)..   
+00012290: 2049 7420 616c 736f 2063 6f6d 7075 7465   It also compute
+000122a0: 7320 7468 6520 636f 7272 656c 6174 696f  s the correlatio
+000122b0: 6e20 636f 6566 6669 6369 656e 7420 6265  n coefficient be
+000122c0: 7477 6565 6e20 7468 6520 5265 6665 7265  tween the Refere
+000122d0: 6e63 6520 7761 7665 666f 726d 2061 6e64  nce waveform and
+000122e0: 2074 6865 2063 7572 7265 6e74 2077 6176   the current wav
+000122f0: 6566 6f72 6d2e 0a0a 2020 2020 5041 5241  eform...    PARA
+00012300: 4d45 5445 5253 3a0a 2020 2020 2d2d 2d2d  METERS:.    ----
+00012310: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+00012320: 2072 6566 3a20 5265 6665 7265 6e63 6520   ref: Reference 
+00012330: 7761 7665 666f 726d 2028 6e70 2e6e 6461  waveform (np.nda
+00012340: 7272 6179 2c20 7369 7a65 204e 290a 2020  rray, size N).  
+00012350: 2020 6375 723a 2043 7572 7265 6e74 2077    cur: Current w
+00012360: 6176 6566 6f72 6d20 286e 702e 6e64 6172  aveform (np.ndar
+00012370: 7261 792c 2073 697a 6520 4e29 0a20 2020  ray, size N).   
+00012380: 2064 765f 7261 6e67 653a 2061 6273 6f6c   dv_range: absol
+00012390: 7574 6520 626f 756e 6420 666f 7220 7468  ute bound for th
+000123a0: 6520 7665 6c6f 6369 7479 2076 6172 6961  e velocity varia
+000123b0: 7469 6f6e 3b20 6578 616d 706c 653a 2064  tion; example: d
+000123c0: 763d 302e 3033 2066 6f72 205b 2d33 2c33  v=0.03 for [-3,3
+000123d0: 5d25 0a20 2020 206f 6620 7265 6c61 7469  ]%.    of relati
+000123e0: 7665 2076 656c 6f63 6974 7920 6368 616e  ve velocity chan
+000123f0: 6765 2028 2766 6c6f 6174 2729 0a20 2020  ge ('float').   
+00012400: 206e 6274 7269 616c 3a20 6e75 6d62 6572   nbtrial: number
+00012410: 206f 6620 7374 7265 7463 6869 6e67 2063   of stretching c
+00012420: 6f65 6666 6963 6965 6e74 2062 6574 7765  oefficient betwe
+00012430: 656e 2064 766d 696e 2061 6e64 2064 766d  en dvmin and dvm
+00012440: 6178 2c20 6e6f 206e 6565 6420 746f 2062  ax, no need to b
+00012450: 6520 6869 6768 6572 2074 6861 6e20 3130  e higher than 10
+00012460: 3020 2028 2766 6c6f 6174 2729 0a20 2020  0  ('float').   
+00012470: 2070 6172 613a 2076 6563 746f 7220 6f66   para: vector of
+00012480: 2074 6865 2069 6e64 6963 6573 206f 6620   the indices of 
+00012490: 7468 6520 6375 7220 616e 6420 7265 6620  the cur and ref 
+000124a0: 7769 6e64 6f77 7320 6f6e 2077 6963 6820  windows on wich 
+000124b0: 796f 7520 7761 6e74 2074 6f20 646f 2074  you want to do t
+000124c0: 6865 0a20 2020 206d 6561 7375 7265 6d65  he.    measureme
+000124d0: 6e74 7320 286e 702e 6e64 6172 7261 792c  nts (np.ndarray,
+000124e0: 2073 697a 6520 746d 696e 2a64 656c 7461   size tmin*delta
+000124f0: 3a74 6d61 782a 6465 6c74 6129 0a20 2020  :tmax*delta).   
+00012500: 2046 6f72 2065 7272 6f72 2063 6f6d 7075   For error compu
+00012510: 7461 7469 6f6e 2c20 7765 206e 6565 6420  tation, we need 
+00012520: 7061 7261 6d65 7465 7273 3a0a 2020 2020  parameters:.    
+00012530: 2020 2020 666d 696e 3a20 6d69 6e69 6d75      fmin: minimu
+00012540: 6d20 6672 6571 7565 6e63 7920 6f66 2074  m frequency of t
+00012550: 6865 2064 6174 610a 2020 2020 2020 2020  he data.        
+00012560: 666d 6178 3a20 6d61 7869 6d75 6d20 6672  fmax: maximum fr
+00012570: 6571 7565 6e63 7920 6f66 2074 6865 2064  equency of the d
+00012580: 6174 610a 2020 2020 2020 2020 746d 696e  ata.        tmin
+00012590: 3a20 6d69 6e69 6d75 6d20 7469 6d65 2077  : minimum time w
+000125a0: 696e 646f 7720 7768 6572 6520 7468 6520  indow where the 
+000125b0: 6476 2f76 2069 7320 636f 6d70 7574 6564  dv/v is computed
+000125c0: 0a20 2020 2020 2020 2074 6d61 783a 206d  .        tmax: m
+000125d0: 6178 696d 756d 2074 696d 6520 7769 6e64  aximum time wind
+000125e0: 6f77 2077 6865 7265 2074 6865 2064 762f  ow where the dv/
+000125f0: 7620 6973 2063 6f6d 7075 7465 640a 2020  v is computed.  
+00012600: 2020 5245 5455 524e 533a 0a20 2020 202d    RETURNS:.    -
+00012610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+00012620: 2020 2020 6476 3a20 5265 6c61 7469 7665      dv: Relative
+00012630: 2076 656c 6f63 6974 7920 6368 616e 6765   velocity change
+00012640: 2064 762f 7620 2869 6e20 2529 0a20 2020   dv/v (in %).   
+00012650: 2063 633a 2063 6f72 7265 6c61 7469 6f6e   cc: correlation
+00012660: 2063 6f65 6666 6963 6965 6e74 2062 6574   coefficient bet
+00012670: 7765 656e 2074 6865 2072 6566 6572 656e  ween the referen
+00012680: 6365 2077 6176 6566 6f72 6d20 616e 6420  ce waveform and 
+00012690: 7468 6520 6265 7374 2073 7472 6574 6368  the best stretch
+000126a0: 6564 2f63 6f6d 7072 6573 7365 6420 6375  ed/compressed cu
+000126b0: 7272 656e 7420 7761 7665 666f 726d 0a20  rrent waveform. 
+000126c0: 2020 2063 6470 3a20 636f 7272 656c 6174     cdp: correlat
+000126d0: 696f 6e20 636f 6566 6669 6369 656e 7420  ion coefficient 
+000126e0: 6265 7477 6565 6e20 7468 6520 7265 6665  between the refe
+000126f0: 7265 6e63 6520 7761 7665 666f 726d 2061  rence waveform a
+00012700: 6e64 2074 6865 2069 6e69 7469 616c 2063  nd the initial c
+00012710: 7572 7265 6e74 2077 6176 6566 6f72 6d0a  urrent waveform.
+00012720: 2020 2020 6572 726f 723a 2045 7272 6f72      error: Error
+00012730: 7320 696e 2074 6865 2064 762f 7620 6d65  s in the dv/v me
+00012740: 6173 7572 656d 656e 7473 2062 6173 6564  asurements based
+00012750: 206f 6e20 5765 6176 6572 2065 7420 616c   on Weaver et al
+00012760: 2028 3230 3131 292c 204f 6e20 7468 6520   (2011), On the 
+00012770: 7072 6563 6973 696f 6e0a 2020 2020 6f66  precision.    of
+00012780: 206e 6f69 7365 2d63 6f72 7265 6c61 7469   noise-correlati
+00012790: 6f6e 2069 6e74 6572 6665 726f 6d65 7472  on interferometr
+000127a0: 792c 2047 656f 7068 7973 2e20 4a2e 2049  y, Geophys. J. I
+000127b0: 6e74 2e2c 2031 3835 2833 290a 0a20 2020  nt., 185(3)..   
+000127c0: 204e 6f74 653a 2054 6865 2063 6f64 6520   Note: The code 
+000127d0: 6669 7273 7420 6669 6e64 7320 7468 6520  first finds the 
+000127e0: 6265 7374 2063 6f72 7265 6c61 7469 6f6e  best correlation
+000127f0: 2063 6f65 6666 6963 6965 6e74 2062 6574   coefficient bet
+00012800: 7765 656e 2074 6865 2052 6566 6572 656e  ween the Referen
+00012810: 6365 2077 6176 6566 6f72 6d20 616e 640a  ce waveform and.
+00012820: 2020 2020 7468 6520 7374 7265 7463 6865      the stretche
+00012830: 642f 636f 6d70 7265 7373 6564 2063 7572  d/compressed cur
+00012840: 7265 6e74 2077 6176 6566 6f72 6d20 616d  rent waveform am
+00012850: 6f6e 6720 7468 6520 226e 6274 7269 616c  ong the "nbtrial
+00012860: 2220 7661 6c75 6573 2e0a 2020 2020 4120  " values..    A 
+00012870: 7265 6669 6e65 6420 616e 616c 7973 6973  refined analysis
+00012880: 2069 7320 7468 656e 2070 6572 666f 726d   is then perform
+00012890: 6564 2061 726f 756e 6420 7468 6973 2076  ed around this v
+000128a0: 616c 7565 2074 6f20 6f62 7461 696e 2061  alue to obtain a
+000128b0: 206d 6f72 6520 7072 6563 6973 6520 6476   more precise dv
+000128c0: 2f76 206d 6561 7375 7265 6d65 6e74 202e  /v measurement .
+000128d0: 0a0a 2020 2020 4f72 6967 696e 616c 6c79  ..    Originally
+000128e0: 2062 7920 4c2e 2056 6965 6e73 2030 342f   by L. Viens 04/
+000128f0: 3236 2f32 3031 3820 2856 6965 6e73 2065  26/2018 (Viens e
+00012900: 7420 616c 2e2c 2032 3031 3820 4a47 5229  t al., 2018 JGR)
+00012910: 0a20 2020 206d 6f64 6966 6965 6420 6279  .    modified by
+00012920: 2043 6865 6e67 7869 6e20 4a69 616e 670a   Chengxin Jiang.
+00012930: 2020 2020 6d6f 6469 6669 6564 2062 7920      modified by 
+00012940: 4c61 7572 6120 4572 6d65 7274 3a20 7665  Laura Ermert: ve
+00012950: 6374 6f72 697a 6564 2076 6572 7369 6f6e  ctorized version
+00012960: 0a20 2020 2022 2222 0a20 2020 2023 206c  .    """.    # l
+00012970: 6f61 6420 636f 6d6d 6f6e 2076 6172 6961  oad common varia
+00012980: 626c 6573 2066 726f 6d20 6469 6374 696f  bles from dictio
+00012990: 6e61 7279 0a20 2020 2074 7769 6e20 3d20  nary.    twin = 
+000129a0: 7061 7261 5b22 7477 696e 225d 0a20 2020  para["twin"].   
+000129b0: 2066 7265 7120 3d20 7061 7261 5b22 6672   freq = para["fr
+000129c0: 6571 225d 0a20 2020 2064 7420 3d20 7061  eq"].    dt = pa
+000129d0: 7261 5b22 6474 225d 0a20 2020 2074 6d69  ra["dt"].    tmi
+000129e0: 6e20 3d20 6e70 2e6d 696e 2874 7769 6e29  n = np.min(twin)
+000129f0: 0a20 2020 2074 6d61 7820 3d20 6e70 2e6d  .    tmax = np.m
+00012a00: 6178 2874 7769 6e29 0a20 2020 2066 6d69  ax(twin).    fmi
+00012a10: 6e20 3d20 6e70 2e6d 696e 2866 7265 7129  n = np.min(freq)
+00012a20: 0a20 2020 2066 6d61 7820 3d20 6e70 2e6d  .    fmax = np.m
+00012a30: 6178 2866 7265 7129 0a20 2020 2074 7665  ax(freq).    tve
+00012a40: 6320 3d20 6e70 2e61 7261 6e67 6528 746d  c = np.arange(tm
+00012a50: 696e 2c20 746d 6178 2c20 6474 290a 0a20  in, tmax, dt).. 
+00012a60: 2020 2023 206d 616b 6520 7573 6566 756c     # make useful
+00012a70: 206f 6e65 2066 6f72 206d 6561 7375 7265   one for measure
+00012a80: 6d65 6e74 730a 2020 2020 6476 6d69 6e20  ments.    dvmin 
+00012a90: 3d20 2d6e 702e 6162 7328 6476 5f72 616e  = -np.abs(dv_ran
+00012aa0: 6765 290a 2020 2020 6476 6d61 7820 3d20  ge).    dvmax = 
+00012ab0: 6e70 2e61 6273 2864 765f 7261 6e67 6529  np.abs(dv_range)
+00012ac0: 0a20 2020 2045 7073 203d 2031 202b 2028  .    Eps = 1 + (
+00012ad0: 6e70 2e6c 696e 7370 6163 6528 6476 6d69  np.linspace(dvmi
+00012ae0: 6e2c 2064 766d 6178 2c20 6e62 7472 6961  n, dvmax, nbtria
+00012af0: 6c29 290a 2020 2020 6364 7020 3d20 6e70  l)).    cdp = np
+00012b00: 2e63 6f72 7263 6f65 6628 6375 722c 2072  .corrcoef(cur, r
+00012b10: 6566 295b 302c 2031 5d20 2023 2063 6f72  ef)[0, 1]  # cor
+00012b20: 7265 6c61 7469 6f6e 2063 6f65 6666 6963  relation coeffic
+00012b30: 6965 6e74 2062 6574 7765 656e 2074 6865  ient between the
+00012b40: 2072 6566 6572 656e 6365 2061 6e64 2069   reference and i
+00012b50: 6e69 7469 616c 2063 7572 7265 6e74 2077  nitial current w
+00012b60: 6176 6566 6f72 6d73 0a20 2020 2077 6176  aveforms.    wav
+00012b70: 6566 6f72 6d73 203d 206e 702e 7a65 726f  eforms = np.zero
+00012b80: 7328 286e 6274 7269 616c 202b 2031 2c20  s((nbtrial + 1, 
+00012b90: 6c65 6e28 7265 6629 2929 0a20 2020 2077  len(ref))).    w
+00012ba0: 6176 6566 6f72 6d73 5b30 2c20 3a5d 203d  aveforms[0, :] =
+00012bb0: 2072 6566 0a0a 2020 2020 2320 5365 7420   ref..    # Set 
+00012bc0: 6f66 2073 7472 6574 6368 6564 2f63 6f6d  of stretched/com
+00012bd0: 7072 6573 7365 6420 6375 7272 656e 7420  pressed current 
+00012be0: 7761 7665 666f 726d 730a 2020 2020 666f  waveforms.    fo
+00012bf0: 7220 6969 2069 6e20 7261 6e67 6528 6e62  r ii in range(nb
+00012c00: 7472 6961 6c29 3a0a 2020 2020 2020 2020  trial):.        
+00012c10: 6e74 203d 2074 7665 6320 2a20 4570 735b  nt = tvec * Eps[
+00012c20: 6969 5d0a 2020 2020 2020 2020 7320 3d20  ii].        s = 
+00012c30: 6e70 2e69 6e74 6572 7028 783d 7476 6563  np.interp(x=tvec
+00012c40: 2c20 7870 3d6e 742c 2066 703d 6375 7229  , xp=nt, fp=cur)
+00012c50: 0a20 2020 2020 2020 2077 6176 6566 6f72  .        wavefor
+00012c60: 6d73 5b69 6920 2b20 312c 203a 5d20 3d20  ms[ii + 1, :] = 
+00012c70: 730a 2020 2020 636f 6620 3d20 6e70 2e63  s.    cof = np.c
+00012c80: 6f72 7263 6f65 6628 7761 7665 666f 726d  orrcoef(waveform
+00012c90: 7329 5b30 5d5b 313a 5d0a 0a20 2020 2023  s)[0][1:]..    #
+00012ca0: 2066 696e 6420 7468 6520 6d61 7869 6d75   find the maximu
+00012cb0: 6d20 636f 7272 656c 6174 696f 6e20 636f  m correlation co
+00012cc0: 6566 6669 6369 656e 740a 2020 2020 696d  efficient.    im
+00012cd0: 6178 203d 206e 702e 6e61 6e61 7267 6d61  ax = np.nanargma
+00012ce0: 7828 636f 6629 0a20 2020 2069 6620 696d  x(cof).    if im
+00012cf0: 6178 203e 3d20 6c65 6e28 4570 7329 202d  ax >= len(Eps) -
+00012d00: 2032 3a0a 2020 2020 2020 2020 696d 6178   2:.        imax
+00012d10: 203d 2069 6d61 7820 2d20 320a 2020 2020   = imax - 2.    
+00012d20: 6966 2069 6d61 7820 3c20 323a 0a20 2020  if imax < 2:.   
+00012d30: 2020 2020 2069 6d61 7820 3d20 696d 6178       imax = imax
+00012d40: 202b 2032 0a0a 2020 2020 2320 5072 6f63   + 2..    # Proc
+00012d50: 6565 6420 746f 2074 6865 2073 6563 6f6e  eed to the secon
+00012d60: 6420 7374 6570 2074 6f20 6765 7420 6120  d step to get a 
+00012d70: 6d6f 7265 2070 7265 6369 7365 2064 762f  more precise dv/
+00012d80: 7620 6d65 6173 7572 656d 656e 740a 2020  v measurement.  
+00012d90: 2020 6474 6669 6e65 7220 3d20 6e70 2e6c    dtfiner = np.l
+00012da0: 696e 7370 6163 6528 4570 735b 696d 6178  inspace(Eps[imax
+00012db0: 202d 2032 5d2c 2045 7073 5b69 6d61 7820   - 2], Eps[imax 
+00012dc0: 2b20 325d 2c20 6e62 7472 6961 6c29 0a20  + 2], nbtrial). 
+00012dd0: 2020 2023 206e 636f 6620 2020 203d 206e     # ncof    = n
+00012de0: 702e 7a65 726f 7328 6474 6669 6e65 722e  p.zeros(dtfiner.
+00012df0: 7368 6170 652c 6474 7970 653d 6e70 2e66  shape,dtype=np.f
+00012e00: 6c6f 6174 3332 290a 2020 2020 7761 7665  loat32).    wave
+00012e10: 666f 726d 7320 3d20 6e70 2e7a 6572 6f73  forms = np.zeros
+00012e20: 2828 6e62 7472 6961 6c20 2b20 312c 206c  ((nbtrial + 1, l
+00012e30: 656e 2872 6566 2929 290a 2020 2020 7761  en(ref))).    wa
+00012e40: 7665 666f 726d 735b 302c 203a 5d20 3d20  veforms[0, :] = 
+00012e50: 7265 660a 2020 2020 666f 7220 6969 2069  ref.    for ii i
+00012e60: 6e20 7261 6e67 6528 6c65 6e28 6474 6669  n range(len(dtfi
+00012e70: 6e65 7229 293a 0a20 2020 2020 2020 206e  ner)):.        n
+00012e80: 7420 3d20 7476 6563 202a 2064 7466 696e  t = tvec * dtfin
+00012e90: 6572 5b69 695d 0a20 2020 2020 2020 2073  er[ii].        s
+00012ea0: 203d 206e 702e 696e 7465 7270 2878 3d74   = np.interp(x=t
+00012eb0: 7665 632c 2078 703d 6e74 2c20 6670 3d63  vec, xp=nt, fp=c
+00012ec0: 7572 290a 2020 2020 2020 2020 7761 7665  ur).        wave
+00012ed0: 666f 726d 735b 6969 202b 2031 2c20 3a5d  forms[ii + 1, :]
+00012ee0: 203d 2073 0a20 2020 206e 636f 6620 3d20   = s.    ncof = 
+00012ef0: 6e70 2e63 6f72 7263 6f65 6628 7761 7665  np.corrcoef(wave
+00012f00: 666f 726d 7329 5b30 5d5b 313a 5d0a 2020  forms)[0][1:].  
+00012f10: 2020 6363 203d 206e 702e 6d61 7828 6e63    cc = np.max(nc
+00012f20: 6f66 2920 2023 2046 696e 6420 6d61 7869  of)  # Find maxi
+00012f30: 6d75 6d20 636f 7272 656c 6174 696f 6e20  mum correlation 
+00012f40: 636f 6566 6669 6369 656e 7420 6f66 2074  coefficient of t
+00012f50: 6865 2072 6566 696e 6564 2020 616e 616c  he refined  anal
+00012f60: 7973 6973 0a20 2020 2064 7620 3d20 3130  ysis.    dv = 10
+00012f70: 302e 3020 2a20 6474 6669 6e65 725b 6e70  0.0 * dtfiner[np
+00012f80: 2e61 7267 6d61 7828 6e63 6f66 295d 202d  .argmax(ncof)] -
+00012f90: 2031 3030 2020 2320 4d75 6c74 6970 6c79   100  # Multiply
+00012fa0: 2062 7920 3130 3020 746f 2063 6f6e 7665   by 100 to conve
+00012fb0: 7274 2074 6f20 7065 7263 656e 7461 6765  rt to percentage
+00012fc0: 2028 4570 7369 6c6f 6e20 3d20 2d64 742f   (Epsilon = -dt/
+00012fd0: 7420 3d20 6476 2f76 290a 0a20 2020 2023  t = dv/v)..    #
+00012fe0: 2045 7272 6f72 2063 6f6d 7075 7461 7469   Error computati
+00012ff0: 6f6e 2062 6173 6564 206f 6e20 5765 6176  on based on Weav
+00013000: 6572 2065 7420 616c 2028 3230 3131 292c  er et al (2011),
+00013010: 204f 6e20 7468 6520 7072 6563 6973 696f   On the precisio
+00013020: 6e20 6f66 206e 6f69 7365 2d63 6f72 7265  n of noise-corre
+00013030: 6c61 7469 6f6e 2069 6e74 6572 6665 726f  lation interfero
+00013040: 6d65 7472 792c 0a20 2020 2023 2047 656f  metry,.    # Geo
+00013050: 7068 7973 2e20 4a2e 2049 6e74 2e2c 2031  phys. J. Int., 1
+00013060: 3835 2833 290a 2020 2020 5420 3d20 3120  85(3).    T = 1 
+00013070: 2f20 2866 6d61 7820 2d20 666d 696e 290a  / (fmax - fmin).
+00013080: 2020 2020 5820 3d20 6363 0a20 2020 2077      X = cc.    w
+00013090: 6320 3d20 6e70 2e70 6920 2a20 2866 6d69  c = np.pi * (fmi
+000130a0: 6e20 2b20 666d 6178 290a 2020 2020 7431  n + fmax).    t1
+000130b0: 203d 206e 702e 6d69 6e28 5b74 6d69 6e2c   = np.min([tmin,
+000130c0: 2074 6d61 785d 290a 2020 2020 7432 203d   tmax]).    t2 =
+000130d0: 206e 702e 6d61 7828 5b74 6d69 6e2c 2074   np.max([tmin, t
+000130e0: 6d61 785d 290a 2020 2020 6572 726f 7220  max]).    error 
+000130f0: 3d20 3130 3020 2a20 280a 2020 2020 2020  = 100 * (.      
+00013100: 2020 6e70 2e73 7172 7428 3120 2d20 582a    np.sqrt(1 - X*
+00013110: 2a32 2920 2f20 2832 202a 2058 2920 2a20  *2) / (2 * X) * 
+00013120: 6e70 2e73 7172 7428 2836 202a 206e 702e  np.sqrt((6 * np.
+00013130: 7371 7274 286e 702e 7069 202f 2032 2920  sqrt(np.pi / 2) 
+00013140: 2a20 5429 202f 2028 7763 2a2a 3220 2a20  * T) / (wc**2 * 
+00013150: 2874 322a 2a33 202d 2074 312a 2a33 2929  (t2**3 - t1**3))
+00013160: 290a 2020 2020 290a 0a20 2020 2072 6574  ).    )..    ret
+00013170: 7572 6e20 6476 2c20 6572 726f 722c 2063  urn dv, error, c
+00013180: 632c 2063 6470 0a0a 0a64 6566 2064 7477  c, cdp...def dtw
+00013190: 5f64 7676 2872 6566 2c20 6375 722c 2070  _dvv(ref, cur, p
+000131a0: 6172 612c 206d 6178 4c61 672c 2062 2c20  ara, maxLag, b, 
+000131b0: 6469 7265 6374 696f 6e29 3a0a 2020 2020  direction):.    
+000131c0: 2222 220a 2020 2020 4479 6e61 6d69 6320  """.    Dynamic 
+000131d0: 7469 6d65 2077 6172 7069 6e67 2066 6f72  time warping for
+000131e0: 2064 762f 7620 6573 7469 6d61 7469 6f6e   dv/v estimation
+000131f0: 2e0a 0a20 2020 2050 4152 414d 4554 4552  ...    PARAMETER
+00013200: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
+00013210: 2d2d 2d2d 2d2d 2d0a 2020 2020 7265 6620  -------.    ref 
+00013220: 3a20 7265 6665 7265 6e63 6520 7369 676e  : reference sign
+00013230: 616c 2028 6e70 2e61 7272 6179 2c20 7369  al (np.array, si
+00013240: 7a65 204e 290a 2020 2020 6375 7220 3a20  ze N).    cur : 
+00013250: 6375 7272 656e 7420 7369 676e 616c 2028  current signal (
+00013260: 6e70 2e61 7272 6179 2c20 7369 7a65 204e  np.array, size N
+00013270: 290a 2020 2020 7061 7261 3a20 6469 6374  ).    para: dict
+00013280: 2063 6f6e 7461 696e 696e 6720 7573 6566   containing usef
+00013290: 756c 2070 6172 616d 6574 6572 7320 6162  ul parameters ab
+000132a0: 6f75 7420 7468 6520 6461 7461 2077 696e  out the data win
+000132b0: 646f 7720 616e 6420 7461 7267 6574 6564  dow and targeted
+000132c0: 2066 7265 7175 656e 6379 0a20 2020 206d   frequency.    m
+000132d0: 6178 4c61 6720 3a20 6d61 7820 6e75 6d62  axLag : max numb
+000132e0: 6572 206f 6620 706f 696e 7473 2074 6f20  er of points to 
+000132f0: 7365 6172 6368 2066 6f72 7761 7264 2061  search forward a
+00013300: 6e64 2062 6163 6b77 6172 642e 0a20 2020  nd backward..   
+00013310: 2020 2020 2020 2020 2053 7567 6765 7374           Suggest
+00013320: 2073 6574 7469 6e67 2069 7420 6c61 7267   setting it larg
+00013330: 6572 2069 6620 7769 6e64 6f77 2069 7320  er if window is 
+00013340: 7365 7420 6c61 7267 6572 2e0a 2020 2020  set larger..    
+00013350: 6220 3a20 622d 7661 6c75 6520 746f 206c  b : b-value to l
+00013360: 696d 6974 2073 7472 6169 6e2c 2077 6869  imit strain, whi
+00013370: 6368 2069 7320 746f 206c 696d 6974 2074  ch is to limit t
+00013380: 6865 206d 6178 696d 756d 2076 656c 6f63  he maximum veloc
+00013390: 6974 7920 7065 7274 7572 6261 7469 6f6e  ity perturbation
+000133a0: 2e0a 2020 2020 2020 2020 2020 2020 5365  ..            Se
+000133b0: 6520 6571 7561 7469 6f6e 2031 3120 696e  e equation 11 in
+000133c0: 2028 4d69 6b65 7365 6c6c 2065 7420 616c   (Mikesell et al
+000133d0: 2e20 3230 3135 290a 2020 2020 6469 7265  . 2015).    dire
+000133e0: 6374 696f 6e3a 2064 6972 6563 7469 6f6e  ction: direction
+000133f0: 2074 6f20 6163 6375 6d75 6c61 7465 2065   to accumulate e
+00013400: 7272 6f72 7320 2831 3d66 6f72 7761 7264  rrors (1=forward
+00013410: 2c20 2d31 3d62 6163 6b77 6172 6429 0a20  , -1=backward). 
+00013420: 2020 2052 4554 5552 4e53 3a0a 2020 2020     RETURNS:.    
+00013430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00013440: 2d2d 0a20 2020 202d 6d30 203a 2065 7374  --.    -m0 : est
+00013450: 696d 6174 6564 2064 762f 760a 2020 2020  imated dv/v.    
+00013460: 656d 3020 3a20 6572 726f 7220 6f66 2064  em0 : error of d
+00013470: 762f 7620 6573 7469 6d61 7469 6f6e 0a0a  v/v estimation..
+00013480: 2020 2020 4f72 6967 696e 616c 2062 7920      Original by 
+00013490: 4469 2059 616e 670a 2020 2020 4c61 7374  Di Yang.    Last
+000134a0: 206d 6f64 6966 6965 6420 6279 2044 796c   modified by Dyl
+000134b0: 616e 204d 696b 6573 656c 6c20 2832 3520  an Mikesell (25 
+000134c0: 4665 622e 2032 3031 3529 0a20 2020 2054  Feb. 2015).    T
+000134d0: 7261 6e73 6c61 7465 6420 746f 2070 7974  ranslated to pyt
+000134e0: 686f 6e20 6279 2054 696d 2043 6c65 6d65  hon by Tim Cleme
+000134f0: 6e74 7320 2831 3720 4175 672e 2032 3031  nts (17 Aug. 201
+00013500: 3829 0a20 2020 2022 2222 0a20 2020 2074  8).    """.    t
+00013510: 7769 6e20 3d20 7061 7261 5b22 7477 696e  win = para["twin
+00013520: 225d 0a20 2020 2064 7420 3d20 7061 7261  "].    dt = para
+00013530: 5b22 6474 225d 0a20 2020 2074 6d69 6e20  ["dt"].    tmin 
+00013540: 3d20 6e70 2e6d 696e 2874 7769 6e29 0a20  = np.min(twin). 
+00013550: 2020 2074 6d61 7820 3d20 6e70 2e6d 6178     tmax = np.max
+00013560: 2874 7769 6e29 0a20 2020 2074 7665 6374  (twin).    tvect
+00013570: 203d 206e 702e 6172 616e 6765 2874 6d69   = np.arange(tmi
+00013580: 6e2c 2074 6d61 782c 2064 7429 0a0a 2020  n, tmax, dt)..  
+00013590: 2020 2320 7365 7475 7020 6f74 6865 7220    # setup other 
+000135a0: 7061 7261 6d65 7465 7273 0a20 2020 206e  parameters.    n
+000135b0: 7074 7320 3d20 6c65 6e28 7265 6629 2020  pts = len(ref)  
+000135c0: 2320 6e75 6d62 6572 206f 6620 7469 6d65  # number of time
+000135d0: 2073 616d 706c 6573 0a0a 2020 2020 2320   samples..    # 
+000135e0: 636f 6d70 7574 6520 6572 726f 7220 6675  compute error fu
+000135f0: 6e63 7469 6f6e 206f 7665 7220 6c61 6773  nction over lags
+00013600: 2c20 7768 6963 6820 6973 2069 6e64 6570  , which is indep
+00013610: 656e 6465 6e74 206f 6620 7374 7261 696e  endent of strain
+00013620: 206c 696d 6974 2027 6227 2e0a 2020 2020   limit 'b'..    
+00013630: 6572 7220 3d20 636f 6d70 7574 6545 7272  err = computeErr
+00013640: 6f72 4675 6e63 7469 6f6e 2863 7572 2c20  orFunction(cur, 
+00013650: 7265 662c 206e 7074 732c 206d 6178 4c61  ref, npts, maxLa
+00013660: 6729 0a0a 2020 2020 2320 6469 7265 6374  g)..    # direct
+00013670: 696f 6e20 746f 2061 6363 756d 756c 6174  ion to accumulat
+00013680: 6520 6572 726f 7273 2028 313d 666f 7277  e errors (1=forw
+00013690: 6172 642c 202d 313d 6261 636b 7761 7264  ard, -1=backward
+000136a0: 290a 2020 2020 6469 7374 203d 2061 6363  ).    dist = acc
+000136b0: 756d 756c 6174 6545 7272 6f72 4675 6e63  umulateErrorFunc
+000136c0: 7469 6f6e 2864 6972 6563 7469 6f6e 2c20  tion(direction, 
+000136d0: 6572 722c 206e 7074 732c 206d 6178 4c61  err, npts, maxLa
+000136e0: 672c 2062 290a 2020 2020 7374 6261 7220  g, b).    stbar 
+000136f0: 3d20 6261 636b 7472 6163 6b44 6973 7461  = backtrackDista
+00013700: 6e63 6546 756e 6374 696f 6e28 2d31 202a  nceFunction(-1 *
+00013710: 2064 6972 6563 7469 6f6e 2c20 6469 7374   direction, dist
+00013720: 2c20 6572 722c 202d 6d61 784c 6167 2c20  , err, -maxLag, 
+00013730: 6229 0a20 2020 2073 7462 6172 5469 6d65  b).    stbarTime
+00013740: 203d 2073 7462 6172 202a 2064 7420 2023   = stbar * dt  #
+00013750: 2063 6f6e 7665 7274 2066 726f 6d20 7361   convert from sa
+00013760: 6d70 6c65 7320 746f 2074 696d 650a 0a20  mples to time.. 
+00013770: 2020 2023 2063 7574 2074 6865 2066 6972     # cut the fir
+00013780: 7374 2061 6e64 206c 6173 7420 3525 2066  st and last 5% f
+00013790: 6f72 2062 6574 7465 7220 7265 6772 6573  or better regres
+000137a0: 7369 6f6e 0a20 2020 2069 6e64 7820 3d20  sion.    indx = 
+000137b0: 6e70 2e77 6865 7265 2828 7476 6563 7420  np.where((tvect 
+000137c0: 3e3d 2030 2e30 3520 2a20 6e70 7473 202a  >= 0.05 * npts *
+000137d0: 2064 7429 2026 2028 7476 6563 7420 3c3d   dt) & (tvect <=
+000137e0: 2030 2e39 3520 2a20 6e70 7473 202a 2064   0.95 * npts * d
+000137f0: 7429 295b 305d 0a0a 2020 2020 2320 6c69  t))[0]..    # li
+00013800: 6e65 6172 2072 6567 7265 7373 696f 6e20  near regression 
+00013810: 746f 2067 6574 2064 762f 760a 2020 2020  to get dv/v.    
+00013820: 6966 206e 7074 7320 3e20 323a 0a20 2020  if npts > 2:.   
+00013830: 2020 2020 2023 2077 6569 6768 7473 0a20       # weights. 
+00013840: 2020 2020 2020 2077 203d 206e 702e 6f6e         w = np.on
+00013850: 6573 286e 7074 7329 0a20 2020 2020 2020  es(npts).       
+00013860: 2023 206d 2c20 612c 2065 6d2c 2065 6120   # m, a, em, ea 
+00013870: 3d20 6c69 6e65 6172 5f72 6567 7265 7373  = linear_regress
+00013880: 696f 6e28 7469 6d65 5f61 7869 735b 696e  ion(time_axis[in
+00013890: 6478 5d2c 2064 656c 7461 5f74 5b69 6e64  dx], delta_t[ind
+000138a0: 785d 2c20 772c 2069 6e74 6572 6365 7074  x], w, intercept
+000138b0: 5f6f 7269 6769 6e3d 4661 6c73 6529 0a20  _origin=False). 
+000138c0: 2020 2020 2020 206d 302c 2065 6d30 203d         m0, em0 =
+000138d0: 206c 696e 6561 725f 7265 6772 6573 7369   linear_regressi
+000138e0: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+000138f0: 7476 6563 742e 666c 6174 7465 6e28 295b  tvect.flatten()[
+00013900: 696e 6478 5d2c 0a20 2020 2020 2020 2020  indx],.         
+00013910: 2020 2073 7462 6172 5469 6d65 2e66 6c61     stbarTime.fla
+00013920: 7474 656e 2829 5b69 6e64 785d 2c0a 2020  tten()[indx],.  
+00013930: 2020 2020 2020 2020 2020 772e 666c 6174            w.flat
+00013940: 7465 6e28 295b 696e 6478 5d2c 0a20 2020  ten()[indx],.   
+00013950: 2020 2020 2020 2020 2069 6e74 6572 6365           interce
+00013960: 7074 5f6f 7269 6769 6e3d 5472 7565 2c0a  pt_origin=True,.
+00013970: 2020 2020 2020 2020 290a 0a20 2020 2065          )..    e
+00013980: 6c73 653a 0a20 2020 2020 2020 206c 6f67  lse:.        log
+00013990: 6765 722e 6465 6275 6728 226e 6f74 2065  ger.debug("not e
+000139a0: 6e6f 7567 6820 706f 696e 7473 2074 6f20  nough points to 
+000139b0: 6573 7469 6d61 7465 2064 762f 7620 666f  estimate dv/v fo
+000139c0: 7220 6474 7722 290a 2020 2020 2020 2020  r dtw").        
+000139d0: 6d30 203d 2030 0a20 2020 2020 2020 2065  m0 = 0.        e
+000139e0: 6d30 203d 2030 0a0a 2020 2020 7265 7475  m0 = 0..    retu
+000139f0: 726e 206d 3020 2a20 3130 302c 2065 6d30  rn m0 * 100, em0
+00013a00: 202a 2031 3030 2c20 6469 7374 0a0a 0a64   * 100, dist...d
+00013a10: 6566 206d 7763 735f 6476 7628 7265 662c  ef mwcs_dvv(ref,
+00013a20: 2063 7572 2c20 6d6f 7669 6e67 5f77 696e   cur, moving_win
+00013a30: 646f 775f 6c65 6e67 7468 2c20 736c 6964  dow_length, slid
+00013a40: 655f 7374 6570 2c20 7061 7261 2c20 736d  e_step, para, sm
+00013a50: 6f6f 7468 696e 675f 6861 6c66 5f77 696e  oothing_half_win
+00013a60: 3d35 293a 0a20 2020 2022 2222 0a20 2020  =5):.    """.   
+00013a70: 204d 6f76 696e 6720 5769 6e64 6f77 2043   Moving Window C
+00013a80: 726f 7373 2053 7065 6374 7275 6d20 6d65  ross Spectrum me
+00013a90: 7468 6f64 2074 6f20 6d65 6173 7572 6520  thod to measure 
+00013aa0: 6476 2f76 2028 7265 6c79 696e 6720 6f6e  dv/v (relying on
+00013ab0: 2070 6869 3d32 2a70 692a 662a 7420 696e   phi=2*pi*f*t in
+00013ac0: 2066 7265 7120 646f 6d61 696e 290a 0a20   freq domain).. 
+00013ad0: 2020 2050 4152 414d 4554 4552 533a 0a20     PARAMETERS:. 
+00013ae0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+00013af0: 2d2d 2d0a 2020 2020 7265 663a 2052 6566  ---.    ref: Ref
+00013b00: 6572 656e 6365 2077 6176 6566 6f72 6d20  erence waveform 
+00013b10: 286e 702e 6e64 6172 7261 792c 2073 697a  (np.ndarray, siz
+00013b20: 6520 4e29 0a20 2020 2063 7572 3a20 4375  e N).    cur: Cu
+00013b30: 7272 656e 7420 7761 7665 666f 726d 2028  rrent waveform (
+00013b40: 6e70 2e6e 6461 7272 6179 2c20 7369 7a65  np.ndarray, size
+00013b50: 204e 290a 2020 2020 6d6f 7669 6e67 5f77   N).    moving_w
+00013b60: 696e 646f 775f 6c65 6e67 7468 3a20 6d6f  indow_length: mo
+00013b70: 7669 6e67 2077 696e 646f 7720 6c65 6e67  ving window leng
+00013b80: 7468 2074 6f20 6361 6c63 756c 6174 6520  th to calculate 
+00013b90: 6372 6f73 732d 7370 6563 7472 756d 2028  cross-spectrum (
+00013ba0: 6e70 2e66 6c6f 6174 2c20 696e 2073 6563  np.float, in sec
+00013bb0: 290a 2020 2020 736c 6964 655f 7374 6570  ).    slide_step
+00013bc0: 3a20 7374 6570 7320 696e 2074 696d 6520  : steps in time 
+00013bd0: 746f 2073 6869 6674 2074 6865 206d 6f76  to shift the mov
+00013be0: 696e 6720 7769 6e64 6f77 2028 6e70 2e66  ing window (np.f
+00013bf0: 6c6f 6174 2c20 696e 2073 6563 6f6e 6473  loat, in seconds
+00013c00: 290a 2020 2020 7061 7261 3a20 6120 6469  ).    para: a di
+00013c10: 6374 2063 6f6e 7461 696e 696e 6720 7061  ct containing pa
+00013c20: 7261 6d65 7465 7273 2061 626f 7574 2069  rameters about i
+00013c30: 6e70 7574 2064 6174 6120 7769 6e64 6f77  nput data window
+00013c40: 2061 6e64 2066 7265 7175 656e 6379 2069   and frequency i
+00013c50: 6e66 6f2c 2069 6e63 6c75 6469 6e67 0a20  nfo, including. 
+00013c60: 2020 2020 2020 2064 656c 7461 2d3e 5468         delta->Th
+00013c70: 6520 7361 6d70 6c69 6e67 2072 6174 6520  e sampling rate 
+00013c80: 6f66 2074 6865 2069 6e70 7574 2074 696d  of the input tim
+00013c90: 6573 6572 6965 7320 2869 6e20 487a 290a  eseries (in Hz).
+00013ca0: 2020 2020 2020 2020 7769 6e64 6f77 2d3e          window->
+00013cb0: 2054 6865 2074 6172 6765 7420 7769 6e64   The target wind
+00013cc0: 6f77 2066 6f72 206d 6561 7375 7269 6e67  ow for measuring
+00013cd0: 2064 742f 740a 2020 2020 2020 2020 6672   dt/t.        fr
+00013ce0: 6571 2d3e 2054 6865 2066 7265 7175 656e  eq-> The frequen
+00013cf0: 6379 2062 6f75 6e64 2074 6f20 636f 6d70  cy bound to comp
+00013d00: 7574 6520 7468 6520 6465 7068 6173 696e  ute the dephasin
+00013d10: 6720 2869 6e20 487a 290a 2020 2020 2020  g (in Hz).      
+00013d20: 2020 746d 696e 3a20 5468 6520 6c65 6674    tmin: The left
+00013d30: 6d6f 7374 2074 696d 6520 6c61 6720 2875  most time lag (u
+00013d40: 7365 6420 746f 2063 6f6d 7075 7465 2074  sed to compute t
+00013d50: 6865 2022 7469 6d65 206c 6167 7320 6172  he "time lags ar
+00013d60: 7261 7922 290a 2020 2020 736d 6f6f 7468  ray").    smooth
+00013d70: 696e 675f 6861 6c66 5f77 696e 3a20 4966  ing_half_win: If
+00013d80: 2064 6966 6665 7265 6e74 2066 726f 6d20   different from 
+00013d90: 302c 2064 6566 696e 6573 2074 6865 2068  0, defines the h
+00013da0: 616c 6620 6c65 6e67 7468 206f 6620 7468  alf length of th
+00013db0: 6520 736d 6f6f 7468 696e 6720 6861 6e6e  e smoothing hann
+00013dc0: 696e 6720 7769 6e64 6f77 2e0a 0a20 2020  ing window...   
+00013dd0: 2052 4554 5552 4e53 3a0a 2020 2020 2d2d   RETURNS:.    --
+00013de0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00013df0: 0a20 2020 2074 696d 655f 6178 6973 3a20  .    time_axis: 
+00013e00: 7468 6520 6365 6e74 7261 6c20 7469 6d65  the central time
+00013e10: 7320 6f66 2074 6865 2077 696e 646f 7773  s of the windows
+00013e20: 2e0a 2020 2020 6465 6c74 615f 743a 2064  ..    delta_t: d
+00013e30: 740a 2020 2020 6465 6c74 615f 6572 723a  t.    delta_err:
+00013e40: 6572 726f 720a 2020 2020 6465 6c74 615f  error.    delta_
+00013e50: 6d63 6f68 3a20 6d65 616e 2063 6f68 6572  mcoh: mean coher
+00013e60: 656e 6365 0a0a 2020 2020 436f 7069 6564  ence..    Copied
+00013e70: 2066 726f 6d20 4d53 4e6f 6973 6520 2868   from MSNoise (h
+00013e80: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00013e90: 6d2f 524f 4265 6c67 6975 6d2f 4d53 4e6f  m/ROBelgium/MSNo
+00013ea0: 6973 652f 7472 6565 2f6d 6173 7465 722f  ise/tree/master/
+00013eb0: 6d73 6e6f 6973 6529 0a20 2020 204d 6f64  msnoise).    Mod
+00013ec0: 6966 6965 6420 6279 2043 6865 6e67 7869  ified by Chengxi
+00013ed0: 6e20 4a69 616e 670a 2020 2020 2222 220a  n Jiang.    """.
+00013ee0: 2020 2020 2320 636f 6d6d 6f6e 2076 6172      # common var
+00013ef0: 6961 626c 6573 0a20 2020 2074 7769 6e20  iables.    twin 
+00013f00: 3d20 7061 7261 5b22 7477 696e 225d 0a20  = para["twin"]. 
+00013f10: 2020 2066 7265 7120 3d20 7061 7261 5b22     freq = para["
+00013f20: 6672 6571 225d 0a20 2020 2064 7420 3d20  freq"].    dt = 
+00013f30: 7061 7261 5b22 6474 225d 0a20 2020 2074  para["dt"].    t
+00013f40: 6d69 6e20 3d20 6e70 2e6d 696e 2874 7769  min = np.min(twi
+00013f50: 6e29 0a20 2020 2066 6d69 6e20 3d20 6e70  n).    fmin = np
+00013f60: 2e6d 696e 2866 7265 7129 0a20 2020 2066  .min(freq).    f
+00013f70: 6d61 7820 3d20 6e70 2e6d 6178 2866 7265  max = np.max(fre
+00013f80: 7129 0a0a 2020 2020 2320 7061 7261 6d65  q)..    # parame
+00013f90: 7465 7220 696e 6974 6961 6c69 7a65 0a20  ter initialize. 
+00013fa0: 2020 2064 656c 7461 5f74 203d 205b 5d0a     delta_t = [].
+00013fb0: 2020 2020 6465 6c74 615f 6572 7220 3d20      delta_err = 
+00013fc0: 5b5d 0a20 2020 2064 656c 7461 5f6d 636f  [].    delta_mco
+00013fd0: 6820 3d20 5b5d 0a20 2020 2074 696d 655f  h = [].    time_
+00013fe0: 6178 6973 203d 205b 5d0a 0a20 2020 2023  axis = []..    #
+00013ff0: 2069 6e66 6f20 6f6e 2074 6865 206d 6f76   info on the mov
+00014000: 696e 6720 7769 6e64 6f77 0a20 2020 2077  ing window.    w
+00014010: 696e 646f 775f 6c65 6e67 7468 5f73 616d  indow_length_sam
+00014020: 706c 6573 203d 206e 702e 696e 7428 6d6f  ples = np.int(mo
+00014030: 7669 6e67 5f77 696e 646f 775f 6c65 6e67  ving_window_leng
+00014040: 7468 202f 2064 7429 0a20 2020 2070 6164  th / dt).    pad
+00014050: 6420 3d20 696e 7428 3220 2a2a 2028 6e65  d = int(2 ** (ne
+00014060: 7874 706f 7732 2877 696e 646f 775f 6c65  xtpow2(window_le
+00014070: 6e67 7468 5f73 616d 706c 6573 2920 2b20  ngth_samples) + 
+00014080: 3229 290a 2020 2020 636f 756e 7420 3d20  2)).    count = 
+00014090: 300a 2020 2020 7470 203d 2063 6f73 696e  0.    tp = cosin
+000140a0: 655f 7461 7065 7228 7769 6e64 6f77 5f6c  e_taper(window_l
+000140b0: 656e 6774 685f 7361 6d70 6c65 732c 2030  ength_samples, 0
+000140c0: 2e31 3529 0a0a 2020 2020 6d69 6e69 6e64  .15)..    minind
+000140d0: 203d 2030 0a20 2020 206d 6178 696e 6420   = 0.    maxind 
+000140e0: 3d20 7769 6e64 6f77 5f6c 656e 6774 685f  = window_length_
+000140f0: 7361 6d70 6c65 730a 0a20 2020 2023 206c  samples..    # l
+00014100: 6f6f 7020 7468 726f 7567 6820 616c 6c20  oop through all 
+00014110: 7375 622d 7769 6e64 6f77 730a 2020 2020  sub-windows.    
+00014120: 7768 696c 6520 6d61 7869 6e64 203c 3d20  while maxind <= 
+00014130: 6c65 6e28 7265 6629 3a0a 2020 2020 2020  len(ref):.      
+00014140: 2020 6363 6920 3d20 6375 725b 6d69 6e69    cci = cur[mini
+00014150: 6e64 3a6d 6178 696e 645d 0a20 2020 2020  nd:maxind].     
+00014160: 2020 2063 6369 203d 2073 6369 7079 2e73     cci = scipy.s
+00014170: 6967 6e61 6c2e 6465 7472 656e 6428 6363  ignal.detrend(cc
+00014180: 692c 2074 7970 653d 226c 696e 6561 7222  i, type="linear"
+00014190: 290a 2020 2020 2020 2020 6363 6920 2a3d  ).        cci *=
+000141a0: 2074 700a 0a20 2020 2020 2020 2063 7269   tp..        cri
+000141b0: 203d 2072 6566 5b6d 696e 696e 643a 6d61   = ref[minind:ma
+000141c0: 7869 6e64 5d0a 2020 2020 2020 2020 6372  xind].        cr
+000141d0: 6920 3d20 7363 6970 792e 7369 676e 616c  i = scipy.signal
+000141e0: 2e64 6574 7265 6e64 2863 7269 2c20 7479  .detrend(cri, ty
+000141f0: 7065 3d22 6c69 6e65 6172 2229 0a20 2020  pe="linear").   
+00014200: 2020 2020 2063 7269 202a 3d20 7470 0a0a       cri *= tp..
+00014210: 2020 2020 2020 2020 6d69 6e69 6e64 202b          minind +
+00014220: 3d20 696e 7428 736c 6964 655f 7374 6570  = int(slide_step
+00014230: 202f 2064 7429 0a20 2020 2020 2020 206d   / dt).        m
+00014240: 6178 696e 6420 2b3d 2069 6e74 2873 6c69  axind += int(sli
+00014250: 6465 5f73 7465 7020 2f20 6474 290a 0a20  de_step / dt).. 
+00014260: 2020 2020 2020 2023 2064 6f20 6666 740a         # do fft.
+00014270: 2020 2020 2020 2020 6663 7572 203d 2073          fcur = s
+00014280: 6369 7079 2e66 6674 7061 636b 2e66 6674  cipy.fftpack.fft
+00014290: 2863 6369 2c20 6e3d 7061 6464 295b 3a20  (cci, n=padd)[: 
+000142a0: 7061 6464 202f 2f20 325d 0a20 2020 2020  padd // 2].     
+000142b0: 2020 2066 7265 6620 3d20 7363 6970 792e     fref = scipy.
+000142c0: 6666 7470 6163 6b2e 6666 7428 6372 692c  fftpack.fft(cri,
+000142d0: 206e 3d70 6164 6429 5b3a 2070 6164 6420   n=padd)[: padd 
+000142e0: 2f2f 2032 5d0a 0a20 2020 2020 2020 2066  // 2]..        f
+000142f0: 6375 7232 203d 206e 702e 7265 616c 2866  cur2 = np.real(f
+00014300: 6375 7229 202a 2a20 3220 2b20 6e70 2e69  cur) ** 2 + np.i
+00014310: 6d61 6728 6663 7572 2920 2a2a 2032 0a20  mag(fcur) ** 2. 
+00014320: 2020 2020 2020 2066 7265 6632 203d 206e         fref2 = n
+00014330: 702e 7265 616c 2866 7265 6629 202a 2a20  p.real(fref) ** 
+00014340: 3220 2b20 6e70 2e69 6d61 6728 6672 6566  2 + np.imag(fref
+00014350: 2920 2a2a 2032 0a0a 2020 2020 2020 2020  ) ** 2..        
+00014360: 2320 6765 7420 6372 6f73 732d 7370 6563  # get cross-spec
+00014370: 7472 756d 2026 2064 6f20 6669 6c74 6572  trum & do filter
+00014380: 696e 670a 2020 2020 2020 2020 5820 3d20  ing.        X = 
+00014390: 6672 6566 202a 2028 6663 7572 2e63 6f6e  fref * (fcur.con
+000143a0: 6a28 2929 0a20 2020 2020 2020 2069 6620  j()).        if 
+000143b0: 736d 6f6f 7468 696e 675f 6861 6c66 5f77  smoothing_half_w
+000143c0: 696e 2021 3d20 303a 0a20 2020 2020 2020  in != 0:.       
+000143d0: 2020 2020 2064 6375 7220 3d20 6e70 2e73       dcur = np.s
+000143e0: 7172 7428 736d 6f6f 7468 2866 6375 7232  qrt(smooth(fcur2
+000143f0: 2c20 7769 6e64 6f77 3d22 6861 6e6e 696e  , window="hannin
+00014400: 6722 2c20 6861 6c66 5f77 696e 3d73 6d6f  g", half_win=smo
+00014410: 6f74 6869 6e67 5f68 616c 665f 7769 6e29  othing_half_win)
+00014420: 290a 2020 2020 2020 2020 2020 2020 6472  ).            dr
+00014430: 6566 203d 206e 702e 7371 7274 2873 6d6f  ef = np.sqrt(smo
+00014440: 6f74 6828 6672 6566 322c 2077 696e 646f  oth(fref2, windo
+00014450: 773d 2268 616e 6e69 6e67 222c 2068 616c  w="hanning", hal
+00014460: 665f 7769 6e3d 736d 6f6f 7468 696e 675f  f_win=smoothing_
+00014470: 6861 6c66 5f77 696e 2929 0a20 2020 2020  half_win)).     
+00014480: 2020 2020 2020 2058 203d 2073 6d6f 6f74         X = smoot
+00014490: 6828 582c 2077 696e 646f 773d 2268 616e  h(X, window="han
+000144a0: 6e69 6e67 222c 2068 616c 665f 7769 6e3d  ning", half_win=
+000144b0: 736d 6f6f 7468 696e 675f 6861 6c66 5f77  smoothing_half_w
+000144c0: 696e 290a 2020 2020 2020 2020 656c 7365  in).        else
+000144d0: 3a0a 2020 2020 2020 2020 2020 2020 6463  :.            dc
+000144e0: 7572 203d 206e 702e 7371 7274 2866 6375  ur = np.sqrt(fcu
+000144f0: 7232 290a 2020 2020 2020 2020 2020 2020  r2).            
+00014500: 6472 6566 203d 206e 702e 7371 7274 2866  dref = np.sqrt(f
+00014510: 7265 6632 290a 0a20 2020 2020 2020 2064  ref2)..        d
+00014520: 6373 203d 206e 702e 6162 7328 5829 0a0a  cs = np.abs(X)..
+00014530: 2020 2020 2020 2020 2320 4669 6e64 2074          # Find t
+00014540: 6865 2076 616c 7565 7320 7468 6520 6672  he values the fr
+00014550: 6571 7565 6e63 7920 7261 6e67 6520 6f66  equency range of
+00014560: 2069 6e74 6572 6573 740a 2020 2020 2020   interest.      
+00014570: 2020 6672 6571 5f76 6563 203d 2073 6369    freq_vec = sci
+00014580: 7079 2e66 6674 7061 636b 2e66 6674 6672  py.fftpack.fftfr
+00014590: 6571 286c 656e 2858 2920 2a20 322c 2064  eq(len(X) * 2, d
+000145a0: 7429 5b3a 2070 6164 6420 2f2f 2032 5d0a  t)[: padd // 2].
+000145b0: 2020 2020 2020 2020 696e 6465 785f 7261          index_ra
+000145c0: 6e67 6520 3d20 6e70 2e61 7267 7768 6572  nge = np.argwher
+000145d0: 6528 6e70 2e6c 6f67 6963 616c 5f61 6e64  e(np.logical_and
+000145e0: 2866 7265 715f 7665 6320 3e3d 2066 6d69  (freq_vec >= fmi
+000145f0: 6e2c 2066 7265 715f 7665 6320 3c3d 2066  n, freq_vec <= f
+00014600: 6d61 7829 290a 0a20 2020 2020 2020 2023  max))..        #
+00014610: 2047 6574 2043 6f68 6572 656e 6365 2061   Get Coherence a
+00014620: 6e64 2069 7473 206d 6561 6e20 7661 6c75  nd its mean valu
+00014630: 650a 2020 2020 2020 2020 636f 6820 3d20  e.        coh = 
+00014640: 6765 7443 6f68 6572 656e 6365 2864 6373  getCoherence(dcs
+00014650: 2c20 6472 6566 2c20 6463 7572 290a 2020  , dref, dcur).  
+00014660: 2020 2020 2020 6d63 6f68 203d 206e 702e        mcoh = np.
+00014670: 6d65 616e 2863 6f68 5b69 6e64 6578 5f72  mean(coh[index_r
+00014680: 616e 6765 5d29 0a0a 2020 2020 2020 2020  ange])..        
+00014690: 2320 4765 7420 5765 6967 6874 730a 2020  # Get Weights.  
+000146a0: 2020 2020 2020 7720 3d20 312e 3020 2f20        w = 1.0 / 
+000146b0: 2831 2e30 202f 2028 636f 685b 696e 6465  (1.0 / (coh[inde
+000146c0: 785f 7261 6e67 655d 202a 2a20 3229 202d  x_range] ** 2) -
+000146d0: 2031 2e30 290a 2020 2020 2020 2020 775b   1.0).        w[
+000146e0: 636f 685b 696e 6465 785f 7261 6e67 655d  coh[index_range]
+000146f0: 203e 3d20 302e 3939 5d20 3d20 312e 3020   >= 0.99] = 1.0 
+00014700: 2f20 2831 2e30 202f 2030 2e39 3830 3120  / (1.0 / 0.9801 
+00014710: 2d20 312e 3029 0a20 2020 2020 2020 2077  - 1.0).        w
+00014720: 203d 206e 702e 7371 7274 2877 202a 206e   = np.sqrt(w * n
+00014730: 702e 7371 7274 2864 6373 5b69 6e64 6578  p.sqrt(dcs[index
+00014740: 5f72 616e 6765 5d29 290a 2020 2020 2020  _range])).      
+00014750: 2020 7720 3d20 6e70 2e72 6561 6c28 7729    w = np.real(w)
+00014760: 0a0a 2020 2020 2020 2020 2320 4672 6571  ..        # Freq
+00014770: 7565 6e63 7920 6172 7261 793a 0a20 2020  uency array:.   
+00014780: 2020 2020 2076 203d 206e 702e 7265 616c       v = np.real
+00014790: 2866 7265 715f 7665 635b 696e 6465 785f  (freq_vec[index_
+000147a0: 7261 6e67 655d 2920 2a20 3220 2a20 6e70  range]) * 2 * np
+000147b0: 2e70 690a 0a20 2020 2020 2020 2023 2050  .pi..        # P
+000147c0: 6861 7365 3a0a 2020 2020 2020 2020 7068  hase:.        ph
+000147d0: 6920 3d20 6e70 2e61 6e67 6c65 2858 290a  i = np.angle(X).
+000147e0: 2020 2020 2020 2020 7068 695b 305d 203d          phi[0] =
+000147f0: 2030 2e30 0a20 2020 2020 2020 2070 6869   0.0.        phi
+00014800: 203d 206e 702e 756e 7772 6170 2870 6869   = np.unwrap(phi
+00014810: 290a 2020 2020 2020 2020 7068 6920 3d20  ).        phi = 
+00014820: 7068 695b 696e 6465 785f 7261 6e67 655d  phi[index_range]
+00014830: 0a0a 2020 2020 2020 2020 2320 4361 6c63  ..        # Calc
+00014840: 756c 6174 6520 7468 6520 736c 6f70 6520  ulate the slope 
+00014850: 7769 7468 2061 2077 6569 6768 7465 6420  with a weighted 
+00014860: 6c65 6173 7420 7371 7561 7265 206c 696e  least square lin
+00014870: 6561 7220 7265 6772 6573 7369 6f6e 0a20  ear regression. 
+00014880: 2020 2020 2020 2023 2066 6f72 6365 6420         # forced 
+00014890: 7468 726f 7567 6820 7468 6520 6f72 6967  through the orig
+000148a0: 696e 3b20 7765 6967 6874 7320 666f 7220  in; weights for 
+000148b0: 7468 6520 574c 5320 6d75 7374 2062 6520  the WLS must be 
+000148c0: 7468 6520 7661 7269 616e 6365 2021 0a20  the variance !. 
+000148d0: 2020 2020 2020 206d 2c20 656d 203d 206c         m, em = l
+000148e0: 696e 6561 725f 7265 6772 6573 7369 6f6e  inear_regression
+000148f0: 2876 2e66 6c61 7474 656e 2829 2c20 7068  (v.flatten(), ph
+00014900: 692e 666c 6174 7465 6e28 292c 2077 2e66  i.flatten(), w.f
+00014910: 6c61 7474 656e 2829 290a 2020 2020 2020  latten()).      
+00014920: 2020 6465 6c74 615f 742e 6170 7065 6e64    delta_t.append
+00014930: 286d 290a 0a20 2020 2020 2020 2023 2070  (m)..        # p
+00014940: 7269 6e74 2070 6869 2e73 6861 7065 2c20  rint phi.shape, 
+00014950: 762e 7368 6170 652c 2077 2e73 6861 7065  v.shape, w.shape
+00014960: 0a20 2020 2020 2020 2065 203d 206e 702e  .        e = np.
+00014970: 7375 6d28 2870 6869 202d 206d 202a 2076  sum((phi - m * v
+00014980: 2920 2a2a 2032 2920 2f20 286e 702e 7369  ) ** 2) / (np.si
+00014990: 7a65 2876 2920 2d20 3129 0a20 2020 2020  ze(v) - 1).     
+000149a0: 2020 2073 3278 3220 3d20 6e70 2e73 756d     s2x2 = np.sum
+000149b0: 2876 2a2a 3220 2a20 772a 2a32 290a 2020  (v**2 * w**2).  
+000149c0: 2020 2020 2020 7378 3220 3d20 6e70 2e73        sx2 = np.s
+000149d0: 756d 2877 202a 2076 2a2a 3229 0a20 2020  um(w * v**2).   
+000149e0: 2020 2020 2065 203d 206e 702e 7371 7274       e = np.sqrt
+000149f0: 2865 202a 2073 3278 3220 2f20 7378 322a  (e * s2x2 / sx2*
+00014a00: 2a32 290a 0a20 2020 2020 2020 2064 656c  *2)..        del
+00014a10: 7461 5f65 7272 2e61 7070 656e 6428 6529  ta_err.append(e)
+00014a20: 0a20 2020 2020 2020 2064 656c 7461 5f6d  .        delta_m
+00014a30: 636f 682e 6170 7065 6e64 286e 702e 7265  coh.append(np.re
+00014a40: 616c 286d 636f 6829 290a 2020 2020 2020  al(mcoh)).      
+00014a50: 2020 7469 6d65 5f61 7869 732e 6170 7065    time_axis.appe
+00014a60: 6e64 2874 6d69 6e20 2b20 6d6f 7669 6e67  nd(tmin + moving
+00014a70: 5f77 696e 646f 775f 6c65 6e67 7468 202f  _window_length /
+00014a80: 2032 2e30 202b 2063 6f75 6e74 202a 2073   2.0 + count * s
+00014a90: 6c69 6465 5f73 7465 7029 0a20 2020 2020  lide_step).     
+00014aa0: 2020 2063 6f75 6e74 202b 3d20 310a 0a20     count += 1.. 
+00014ab0: 2020 2020 2020 2064 656c 2066 6375 722c         del fcur,
+00014ac0: 2066 7265 660a 2020 2020 2020 2020 6465   fref.        de
+00014ad0: 6c20 580a 2020 2020 2020 2020 6465 6c20  l X.        del 
+00014ae0: 6672 6571 5f76 6563 0a20 2020 2020 2020  freq_vec.       
+00014af0: 2064 656c 2069 6e64 6578 5f72 616e 6765   del index_range
+00014b00: 0a20 2020 2020 2020 2064 656c 2077 2c20  .        del w, 
+00014b10: 762c 2065 2c20 7332 7832 2c20 7378 322c  v, e, s2x2, sx2,
+00014b20: 206d 2c20 656d 0a0a 2020 2020 6966 206d   m, em..    if m
+00014b30: 6178 696e 6420 3e20 6c65 6e28 6375 7229  axind > len(cur)
+00014b40: 202b 2069 6e74 2873 6c69 6465 5f73 7465   + int(slide_ste
+00014b50: 7020 2f20 6474 293a 0a20 2020 2020 2020  p / dt):.       
+00014b60: 206c 6f67 6765 722e 6465 6275 6728 2254   logger.debug("T
+00014b70: 6865 206c 6173 7420 7769 6e64 6f77 2077  he last window w
+00014b80: 6173 2074 6f6f 2073 6d61 6c6c 2c20 6275  as too small, bu
+00014b90: 7420 7761 7320 636f 6d70 7574 6564 2229  t was computed")
+00014ba0: 0a0a 2020 2020 2320 656e 7375 7265 2061  ..    # ensure a
+00014bb0: 6c6c 206d 6174 7269 7820 6172 6520 6e70  ll matrix are np
+00014bc0: 2061 7272 6179 0a20 2020 2064 656c 7461   array.    delta
+00014bd0: 5f74 203d 206e 702e 6172 7261 7928 6465  _t = np.array(de
+00014be0: 6c74 615f 7429 0a20 2020 2064 656c 7461  lta_t).    delta
+00014bf0: 5f65 7272 203d 206e 702e 6172 7261 7928  _err = np.array(
+00014c00: 6465 6c74 615f 6572 7229 0a20 2020 2064  delta_err).    d
+00014c10: 656c 7461 5f6d 636f 6820 3d20 6e70 2e61  elta_mcoh = np.a
+00014c20: 7272 6179 2864 656c 7461 5f6d 636f 6829  rray(delta_mcoh)
+00014c30: 0a20 2020 2074 696d 655f 6178 6973 203d  .    time_axis =
+00014c40: 206e 702e 6172 7261 7928 7469 6d65 5f61   np.array(time_a
+00014c50: 7869 7329 0a0a 2020 2020 2320 7265 6164  xis)..    # read
+00014c60: 7920 666f 7220 6c69 6e65 6172 2072 6567  y for linear reg
+00014c70: 7265 7373 696f 6e0a 2020 2020 6465 6c74  ression.    delt
+00014c80: 615f 6d69 6e63 686f 203d 2030 2e36 350a  a_mincho = 0.65.
+00014c90: 2020 2020 6465 6c74 615f 6d61 7865 7272      delta_maxerr
+00014ca0: 203d 2030 2e31 0a20 2020 2064 656c 7461   = 0.1.    delta
+00014cb0: 5f6d 6178 6474 203d 2030 2e31 0a20 2020  _maxdt = 0.1.   
+00014cc0: 2069 6e64 7831 203d 206e 702e 7768 6572   indx1 = np.wher
+00014cd0: 6528 6465 6c74 615f 6d63 6f68 203e 2064  e(delta_mcoh > d
+00014ce0: 656c 7461 5f6d 696e 6368 6f29 0a20 2020  elta_mincho).   
+00014cf0: 2069 6e64 7832 203d 206e 702e 7768 6572   indx2 = np.wher
+00014d00: 6528 6465 6c74 615f 6572 7220 3c20 6465  e(delta_err < de
+00014d10: 6c74 615f 6d61 7865 7272 290a 2020 2020  lta_maxerr).    
+00014d20: 696e 6478 3320 3d20 6e70 2e77 6865 7265  indx3 = np.where
+00014d30: 2864 656c 7461 5f74 203c 2064 656c 7461  (delta_t < delta
+00014d40: 5f6d 6178 6474 290a 0a20 2020 2023 202d  _maxdt)..    # -
+00014d50: 2d2d 2d2d 6669 6e64 2067 6f6f 6420 6474  ----find good dt
+00014d60: 206d 6561 7375 7265 6d65 6e74 732d 2d2d   measurements---
+00014d70: 2d2d 0a20 2020 2069 6e64 7820 3d20 6e70  --.    indx = np
+00014d80: 2e69 6e74 6572 7365 6374 3164 2869 6e64  .intersect1d(ind
+00014d90: 7831 2c20 696e 6478 3229 0a20 2020 2069  x1, indx2).    i
+00014da0: 6e64 7820 3d20 6e70 2e69 6e74 6572 7365  ndx = np.interse
+00014db0: 6374 3164 2869 6e64 782c 2069 6e64 7833  ct1d(indx, indx3
+00014dc0: 290a 0a20 2020 2069 6620 6c65 6e28 696e  )..    if len(in
+00014dd0: 6478 2920 3e20 323a 0a20 2020 2020 2020  dx) > 2:.       
+00014de0: 2023 202d 2d2d 2d65 7374 696d 6174 6520   # ----estimate 
+00014df0: 7765 6967 6874 2066 6f72 2072 6567 7265  weight for regre
+00014e00: 7373 696f 6e2d 2d2d 2d0a 2020 2020 2020  ssion----.      
+00014e10: 2020 7720 3d20 3120 2f20 6465 6c74 615f    w = 1 / delta_
+00014e20: 6572 725b 696e 6478 5d0a 2020 2020 2020  err[indx].      
+00014e30: 2020 775b 7e6e 702e 6973 6669 6e69 7465    w[~np.isfinite
+00014e40: 2877 295d 203d 2031 2e30 0a0a 2020 2020  (w)] = 1.0..    
+00014e50: 2020 2020 2320 2d2d 2d2d 2d2d 2d2d 2d64      # ---------d
+00014e60: 6f20 6c69 6e65 6172 2072 6567 7265 7373  o linear regress
+00014e70: 696f 6e2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  ion-----------. 
+00014e80: 2020 2020 2020 2023 206d 2c20 612c 2065         # m, a, e
+00014e90: 6d2c 2065 6120 3d20 6c69 6e65 6172 5f72  m, ea = linear_r
+00014ea0: 6567 7265 7373 696f 6e28 7469 6d65 5f61  egression(time_a
+00014eb0: 7869 735b 696e 6478 5d2c 2064 656c 7461  xis[indx], delta
+00014ec0: 5f74 5b69 6e64 785d 2c20 772c 2069 6e74  _t[indx], w, int
+00014ed0: 6572 6365 7074 5f6f 7269 6769 6e3d 4661  ercept_origin=Fa
+00014ee0: 6c73 6529 0a20 2020 2020 2020 206d 302c  lse).        m0,
+00014ef0: 2065 6d30 203d 206c 696e 6561 725f 7265   em0 = linear_re
+00014f00: 6772 6573 7369 6f6e 2874 696d 655f 6178  gression(time_ax
+00014f10: 6973 5b69 6e64 785d 2c20 6465 6c74 615f  is[indx], delta_
+00014f20: 745b 696e 6478 5d2c 2077 2c20 696e 7465  t[indx], w, inte
+00014f30: 7263 6570 745f 6f72 6967 696e 3d54 7275  rcept_origin=Tru
+00014f40: 6529 0a0a 2020 2020 656c 7365 3a0a 2020  e)..    else:.  
+00014f50: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+00014f60: 7567 2822 6e6f 7420 656e 6f75 6768 2070  ug("not enough p
+00014f70: 6f69 6e74 7320 746f 2065 7374 696d 6174  oints to estimat
+00014f80: 6520 6476 2f76 2066 6f72 206d 7763 7322  e dv/v for mwcs"
+00014f90: 290a 2020 2020 2020 2020 6d30 203d 2030  ).        m0 = 0
+00014fa0: 0a20 2020 2020 2020 2065 6d30 203d 2030  .        em0 = 0
+00014fb0: 0a0a 2020 2020 7265 7475 726e 202d 6d30  ..    return -m0
+00014fc0: 202a 2031 3030 2c20 656d 3020 2a20 3130   * 100, em0 * 10
+00014fd0: 300a 0a0a 6465 6620 5743 435f 6476 7628  0...def WCC_dvv(
+00014fe0: 7265 662c 2063 7572 2c20 6d6f 7669 6e67  ref, cur, moving
+00014ff0: 5f77 696e 646f 775f 6c65 6e67 7468 2c20  _window_length, 
+00015000: 736c 6964 655f 7374 6570 2c20 7061 7261  slide_step, para
+00015010: 293a 0a20 2020 2022 2222 0a20 2020 2057  ):.    """.    W
+00015020: 696e 646f 7765 6420 6372 6f73 7320 636f  indowed cross co
+00015030: 7272 656c 6174 696f 6e20 2857 4343 2920  rrelation (WCC) 
+00015040: 666f 7220 6474 206f 7220 6476 2f76 206d  for dt or dv/v m
+00015050: 6573 7572 656d 656e 7420 2853 6e69 6564  esurement (Snied
+00015060: 6572 2065 7420 616c 2e20 3230 3132 290a  er et al. 2012).
+00015070: 0a20 2020 2050 6172 616d 6574 6572 733a  .    Parameters:
+00015080: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
+00015090: 0a20 2020 2072 6566 3a20 5468 6520 2252  .    ref: The "R
+000150a0: 6566 6572 656e 6365 2220 7469 6d65 7365  eference" timese
+000150b0: 7269 6573 0a20 2020 2063 7572 3a20 5468  ries.    cur: Th
+000150c0: 6520 2243 7572 7265 6e74 2220 7469 6d65  e "Current" time
+000150d0: 7365 7269 6573 0a20 2020 206d 6f76 696e  series.    movin
+000150e0: 675f 7769 6e64 6f77 5f6c 656e 6774 683a  g_window_length:
+000150f0: 2054 6865 206d 6f76 696e 6720 7769 6e64   The moving wind
+00015100: 6f77 206c 656e 6774 6820 2869 6e20 7365  ow length (in se
+00015110: 636f 6e64 7329 0a20 2020 2073 6c69 6465  conds).    slide
+00015120: 5f73 7465 703a 2054 6865 2073 7465 7020  _step: The step 
+00015130: 746f 206a 756d 7020 666f 7220 7468 6520  to jump for the 
+00015140: 6d6f 7669 6e67 2077 696e 646f 7720 2869  moving window (i
+00015150: 6e20 7365 636f 6e64 7329 0a20 2020 2070  n seconds).    p
+00015160: 6172 613a 2061 2064 6963 7420 636f 6e74  ara: a dict cont
+00015170: 6169 6e69 6e67 2066 7265 712f 7469 6d65  aining freq/time
+00015180: 2069 6e66 6f20 6f66 2074 6865 2064 6174   info of the dat
+00015190: 6120 6d61 7472 6978 0a0a 2020 2020 5265  a matrix..    Re
+000151a0: 7475 726e 733a 0a20 2020 202d 2d2d 2d2d  turns:.    -----
+000151b0: 2d2d 2d2d 2d2d 2d0a 2020 2020 7469 6d65  -------.    time
+000151c0: 5f61 7869 733a 2063 656e 7472 616c 2074  _axis: central t
+000151d0: 696d 6573 206f 6620 7468 6520 6d6f 7669  imes of the movi
+000151e0: 6e67 2077 696e 646f 770a 2020 2020 6465  ng window.    de
+000151f0: 6c74 615f 743a 2064 740a 2020 2020 6465  lta_t: dt.    de
+00015200: 6c74 615f 6572 723a 2065 7272 6f72 0a20  lta_err: error. 
+00015210: 2020 2064 656c 7461 5f6d 636f 683a 206d     delta_mcoh: m
+00015220: 6561 6e20 636f 6865 7265 6e63 6520 666f  ean coherence fo
+00015230: 7220 6561 6368 2077 696e 646f 770a 0a20  r each window.. 
+00015240: 2020 2057 7269 7474 656e 2062 7920 436f     Written by Co
+00015250: 6e67 636f 6e67 2059 7561 6e20 2831 204a  ngcong Yuan (1 J
+00015260: 756c 792c 2032 3031 3929 0a20 2020 2022  uly, 2019).    "
+00015270: 2222 0a20 2020 2023 2063 6f6d 6d6f 6e20  "".    # common 
+00015280: 7661 7269 6162 6c65 730a 2020 2020 7477  variables.    tw
+00015290: 696e 203d 2070 6172 615b 2274 7769 6e22  in = para["twin"
+000152a0: 5d0a 2020 2020 6474 203d 2070 6172 615b  ].    dt = para[
+000152b0: 2264 7422 5d0a 2020 2020 746d 696e 203d  "dt"].    tmin =
+000152c0: 206e 702e 6d69 6e28 7477 696e 290a 0a20   np.min(twin).. 
+000152d0: 2020 2023 2070 6172 616d 6574 6572 2069     # parameter i
+000152e0: 6e69 7469 616c 697a 650a 2020 2020 6465  nitialize.    de
+000152f0: 6c74 615f 7420 3d20 5b5d 0a20 2020 2064  lta_t = [].    d
+00015300: 656c 7461 5f74 5f63 6f65 6620 3d20 5b5d  elta_t_coef = []
+00015310: 0a20 2020 2074 696d 655f 6178 6973 203d  .    time_axis =
+00015320: 205b 5d0a 0a20 2020 2023 2069 6e66 6f20   []..    # info 
+00015330: 6f6e 2074 6865 206d 6f76 696e 6720 7769  on the moving wi
+00015340: 6e64 6f77 0a20 2020 2077 696e 646f 775f  ndow.    window_
+00015350: 6c65 6e67 7468 5f73 616d 706c 6573 203d  length_samples =
+00015360: 206e 702e 696e 7428 6d6f 7669 6e67 5f77   np.int(moving_w
+00015370: 696e 646f 775f 6c65 6e67 7468 202f 2064  indow_length / d
+00015380: 7429 0a20 2020 2063 6f75 6e74 203d 2030  t).    count = 0
+00015390: 0a20 2020 2074 7020 3d20 636f 7369 6e65  .    tp = cosine
+000153a0: 5f74 6170 6572 2877 696e 646f 775f 6c65  _taper(window_le
+000153b0: 6e67 7468 5f73 616d 706c 6573 2c20 302e  ngth_samples, 0.
+000153c0: 3135 290a 0a20 2020 206d 696e 696e 6420  15)..    minind 
+000153d0: 3d20 300a 2020 2020 6d61 7869 6e64 203d  = 0.    maxind =
+000153e0: 2077 696e 646f 775f 6c65 6e67 7468 5f73   window_length_s
+000153f0: 616d 706c 6573 0a0a 2020 2020 2320 6c6f  amples..    # lo
+00015400: 6f70 2074 6872 6f75 6768 2061 6c6c 2073  op through all s
+00015410: 7562 2d77 696e 646f 7773 0a20 2020 2077  ub-windows.    w
+00015420: 6869 6c65 206d 6178 696e 6420 3c3d 206c  hile maxind <= l
+00015430: 656e 2872 6566 293a 0a20 2020 2020 2020  en(ref):.       
+00015440: 2063 6369 203d 2063 7572 5b6d 696e 696e   cci = cur[minin
+00015450: 643a 6d61 7869 6e64 5d0a 2020 2020 2020  d:maxind].      
+00015460: 2020 6363 6920 3d20 7363 6970 792e 7369    cci = scipy.si
+00015470: 676e 616c 2e64 6574 7265 6e64 2863 6369  gnal.detrend(cci
+00015480: 2c20 7479 7065 3d22 6c69 6e65 6172 2229  , type="linear")
+00015490: 0a20 2020 2020 2020 2063 6369 202a 3d20  .        cci *= 
+000154a0: 7470 0a0a 2020 2020 2020 2020 6372 6920  tp..        cri 
+000154b0: 3d20 7265 665b 6d69 6e69 6e64 3a6d 6178  = ref[minind:max
+000154c0: 696e 645d 0a20 2020 2020 2020 2063 7269  ind].        cri
+000154d0: 203d 2073 6369 7079 2e73 6967 6e61 6c2e   = scipy.signal.
+000154e0: 6465 7472 656e 6428 6372 692c 2074 7970  detrend(cri, typ
+000154f0: 653d 226c 696e 6561 7222 290a 2020 2020  e="linear").    
+00015500: 2020 2020 6372 6920 2a3d 2074 700a 0a20      cri *= tp.. 
+00015510: 2020 2020 2020 206d 696e 696e 6420 2b3d         minind +=
+00015520: 2069 6e74 2873 6c69 6465 5f73 7465 7020   int(slide_step 
+00015530: 2f20 6474 290a 2020 2020 2020 2020 6d61  / dt).        ma
+00015540: 7869 6e64 202b 3d20 696e 7428 736c 6964  xind += int(slid
+00015550: 655f 7374 6570 202f 2064 7429 0a0a 2020  e_step / dt)..  
+00015560: 2020 2020 2020 2320 6e6f 726d 616c 697a        # normaliz
+00015570: 6520 7369 676e 616c 7320 6265 666f 7265  e signals before
+00015580: 2063 726f 7373 2063 6f72 7265 6c61 7469   cross correlati
+00015590: 6f6e 0a20 2020 2020 2020 2063 6369 203d  on.        cci =
+000155a0: 2028 6363 6920 2d20 6363 692e 6d65 616e   (cci - cci.mean
+000155b0: 2829 2920 2f20 6363 692e 7374 6428 290a  ()) / cci.std().
+000155c0: 2020 2020 2020 2020 6372 6920 3d20 2863          cri = (c
+000155d0: 7269 202d 2063 7269 2e6d 6561 6e28 2929  ri - cri.mean())
+000155e0: 202f 2063 7269 2e73 7464 2829 0a0a 2020   / cri.std()..  
+000155f0: 2020 2020 2020 2320 6765 7420 6d61 7869        # get maxi
+00015600: 6d75 6d20 636f 7272 656c 6174 696f 6e20  mum correlation 
+00015610: 636f 6566 6669 6369 656e 7420 616e 6420  coefficient and 
+00015620: 6974 7320 696e 6465 780a 2020 2020 2020  its index.      
+00015630: 2020 6363 3220 3d20 6e70 2e63 6f72 7265    cc2 = np.corre
+00015640: 6c61 7465 2863 6369 2c20 6372 692c 206d  late(cci, cri, m
+00015650: 6f64 653d 2273 616d 6522 290a 2020 2020  ode="same").    
+00015660: 2020 2020 6363 3220 3d20 6363 3220 2f20      cc2 = cc2 / 
+00015670: 6e70 2e73 7172 7428 2863 6369 2a2a 3229  np.sqrt((cci**2)
+00015680: 2e73 756d 2829 202a 2028 6372 692a 2a32  .sum() * (cri**2
+00015690: 292e 7375 6d28 2929 0a0a 2020 2020 2020  ).sum())..      
+000156a0: 2020 696d 6178 6363 3220 3d20 6e70 2e77    imaxcc2 = np.w
+000156b0: 6865 7265 2863 6332 203d 3d20 6e70 2e6d  here(cc2 == np.m
+000156c0: 6178 2863 6332 2929 5b30 5d0a 2020 2020  ax(cc2))[0].    
+000156d0: 2020 2020 6d61 7863 6332 203d 206e 702e      maxcc2 = np.
+000156e0: 6d61 7828 6363 3229 0a0a 2020 2020 2020  max(cc2)..      
+000156f0: 2020 2320 6765 7420 7468 6520 7469 6d65    # get the time
+00015700: 2073 6869 6674 0a20 2020 2020 2020 206d   shift.        m
+00015710: 203d 2028 696d 6178 6363 3220 2d20 2828   = (imaxcc2 - ((
+00015720: 6d61 7869 6e64 202d 206d 696e 696e 6429  maxind - minind)
+00015730: 202f 2f20 3229 2920 2a20 6474 0a20 2020   // 2)) * dt.   
+00015740: 2020 2020 2064 656c 7461 5f74 2e61 7070       delta_t.app
+00015750: 656e 6428 6d29 0a20 2020 2020 2020 2064  end(m).        d
+00015760: 656c 7461 5f74 5f63 6f65 662e 6170 7065  elta_t_coef.appe
+00015770: 6e64 286d 6178 6363 3229 0a0a 2020 2020  nd(maxcc2)..    
+00015780: 2020 2020 7469 6d65 5f61 7869 732e 6170      time_axis.ap
+00015790: 7065 6e64 2874 6d69 6e20 2b20 6d6f 7669  pend(tmin + movi
+000157a0: 6e67 5f77 696e 646f 775f 6c65 6e67 7468  ng_window_length
+000157b0: 202f 2032 2e30 202b 2063 6f75 6e74 202a   / 2.0 + count *
+000157c0: 2073 6c69 6465 5f73 7465 7029 0a20 2020   slide_step).   
+000157d0: 2020 2020 2063 6f75 6e74 202b 3d20 310a       count += 1.
+000157e0: 0a20 2020 2064 656c 2063 6369 2c20 6372  .    del cci, cr
+000157f0: 692c 2063 6332 2c20 696d 6178 6363 322c  i, cc2, imaxcc2,
+00015800: 206d 6178 6363 320a 2020 2020 6465 6c20   maxcc2.    del 
+00015810: 6d0a 0a20 2020 2069 6620 6d61 7869 6e64  m..    if maxind
+00015820: 203e 206c 656e 2863 7572 2920 2b20 696e   > len(cur) + in
+00015830: 7428 736c 6964 655f 7374 6570 202f 2064  t(slide_step / d
+00015840: 7429 3a0a 2020 2020 2020 2020 6c6f 6767  t):.        logg
+00015850: 6572 2e64 6562 7567 2822 5468 6520 6c61  er.debug("The la
+00015860: 7374 2077 696e 646f 7720 7761 7320 746f  st window was to
+00015870: 6f20 736d 616c 6c2c 2062 7574 2077 6173  o small, but was
+00015880: 2063 6f6d 7075 7465 6422 290a 0a20 2020   computed")..   
+00015890: 2064 656c 7461 5f74 203d 206e 702e 6172   delta_t = np.ar
+000158a0: 7261 7928 6465 6c74 615f 7429 0a20 2020  ray(delta_t).   
+000158b0: 2064 656c 7461 5f74 5f63 6f65 6620 3d20   delta_t_coef = 
+000158c0: 6e70 2e61 7272 6179 2864 656c 7461 5f74  np.array(delta_t
+000158d0: 5f63 6f65 6629 0a20 2020 2074 696d 655f  _coef).    time_
+000158e0: 6178 6973 203d 206e 702e 6172 7261 7928  axis = np.array(
+000158f0: 7469 6d65 5f61 7869 7329 0a0a 2020 2020  time_axis)..    
+00015900: 2320 6c69 6e65 6172 2072 6567 7265 7373  # linear regress
+00015910: 696f 6e20 746f 2067 6574 2064 762f 760a  ion to get dv/v.
+00015920: 2020 2020 6966 2063 6f75 6e74 203e 2032      if count > 2
+00015930: 3a0a 2020 2020 2020 2020 2320 7369 6d70  :.        # simp
+00015940: 6c65 2077 6569 6768 740a 2020 2020 2020  le weight.      
+00015950: 2020 7720 3d20 6e70 2e6f 6e65 7328 636f    w = np.ones(co
+00015960: 756e 7429 0a20 2020 2020 2020 2023 206d  unt).        # m
+00015970: 2c20 612c 2065 6d2c 2065 6120 3d20 6c69  , a, em, ea = li
+00015980: 6e65 6172 5f72 6567 7265 7373 696f 6e28  near_regression(
+00015990: 7469 6d65 5f61 7869 735b 696e 6478 5d2c  time_axis[indx],
+000159a0: 2064 656c 7461 5f74 5b69 6e64 785d 2c20   delta_t[indx], 
+000159b0: 772c 2069 6e74 6572 6365 7074 5f6f 7269  w, intercept_ori
+000159c0: 6769 6e3d 4661 6c73 6529 0a20 2020 2020  gin=False).     
+000159d0: 2020 206d 302c 2065 6d30 203d 206c 696e     m0, em0 = lin
+000159e0: 6561 725f 7265 6772 6573 7369 6f6e 2874  ear_regression(t
+000159f0: 696d 655f 6178 6973 2e66 6c61 7474 656e  ime_axis.flatten
+00015a00: 2829 2c20 6465 6c74 615f 742e 666c 6174  (), delta_t.flat
+00015a10: 7465 6e28 292c 2077 2e66 6c61 7474 656e  ten(), w.flatten
+00015a20: 2829 2c20 696e 7465 7263 6570 745f 6f72  (), intercept_or
+00015a30: 6967 696e 3d54 7275 6529 0a0a 2020 2020  igin=True)..    
+00015a40: 656c 7365 3a0a 2020 2020 2020 2020 6c6f  else:.        lo
+00015a50: 6767 6572 2e64 6562 7567 2822 6e6f 7420  gger.debug("not 
+00015a60: 656e 6f75 6768 2070 6f69 6e74 7320 746f  enough points to
+00015a70: 2065 7374 696d 6174 6520 6476 2f76 2066   estimate dv/v f
+00015a80: 6f72 2077 6363 2229 0a20 2020 2020 2020  or wcc").       
+00015a90: 206d 3020 3d20 300a 2020 2020 2020 2020   m0 = 0.        
+00015aa0: 656d 3020 3d20 300a 0a20 2020 2072 6574  em0 = 0..    ret
+00015ab0: 7572 6e20 2d6d 3020 2a20 3130 302c 2065  urn -m0 * 100, e
+00015ac0: 6d30 202a 2031 3030 0a0a 0a64 6566 2077  m0 * 100...def w
+00015ad0: 7873 5f64 7676 280a 2020 2020 7265 662c  xs_dvv(.    ref,
+00015ae0: 0a20 2020 2063 7572 2c0a 2020 2020 616c  .    cur,.    al
+00015af0: 6c66 7265 712c 0a20 2020 2070 6172 612c  lfreq,.    para,
+00015b00: 0a20 2020 2064 6a3d 3120 2f20 3132 2c0a  .    dj=1 / 12,.
+00015b10: 2020 2020 7330 3d2d 312c 0a20 2020 204a      s0=-1,.    J
+00015b20: 3d2d 312c 0a20 2020 2073 6967 3d46 616c  =-1,.    sig=Fal
+00015b30: 7365 2c0a 2020 2020 7776 6e3d 226d 6f72  se,.    wvn="mor
+00015b40: 6c65 7422 2c0a 2020 2020 756e 7772 6170  let",.    unwrap
+00015b50: 666c 6167 3d46 616c 7365 2c0a 293a 0a20  flag=False,.):. 
+00015b60: 2020 2022 2222 0a20 2020 2043 6f6d 7075     """.    Compu
+00015b70: 7465 2064 7420 6f72 2064 762f 7620 696e  te dt or dv/v in
+00015b80: 2074 696d 6520 616e 6420 6672 6571 7565   time and freque
+00015b90: 6e63 7920 646f 6d61 696e 2066 726f 6d20  ncy domain from 
+00015ba0: 7761 7665 6c65 7420 6372 6f73 7320 7370  wavelet cross sp
+00015bb0: 6563 7472 756d 2028 7778 7329 2e0a 2020  ectrum (wxs)..  
+00015bc0: 2020 666f 7220 616c 6c20 6672 6571 7565    for all freque
+00015bd0: 6369 6573 2069 6e20 616e 2069 6e74 6572  cies in an inter
+00015be0: 6573 7420 7261 6e67 650a 0a20 2020 2050  est range..    P
+00015bf0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+00015c00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+00015c10: 2072 6566 3a20 5468 6520 2252 6566 6572   ref: The "Refer
+00015c20: 656e 6365 2220 7469 6d65 7365 7269 6573  ence" timeseries
+00015c30: 2028 6e75 6d70 792e 6e64 6172 7261 7929   (numpy.ndarray)
+00015c40: 0a20 2020 2063 7572 3a20 5468 6520 2243  .    cur: The "C
+00015c50: 7572 7265 6e74 2220 7469 6d65 7365 7269  urrent" timeseri
+00015c60: 6573 2028 6e75 6d70 792e 6e64 6172 7261  es (numpy.ndarra
+00015c70: 7929 0a20 2020 2061 6c6c 6672 6571 3a20  y).    allfreq: 
+00015c80: 6120 626f 6f6c 656e 2076 6172 6961 626c  a boolen variabl
+00015c90: 6520 746f 206d 616b 6520 6d65 6173 7572  e to make measur
+00015ca0: 656d 656e 7473 206f 6e20 616c 6c20 6672  ements on all fr
+00015cb0: 6571 7565 6e63 7920 7261 6e67 6520 6f72  equency range or
+00015cc0: 206e 6f74 0a20 2020 2070 6172 613a 2061   not.    para: a
+00015cd0: 2064 6963 7420 636f 6e74 6169 6e69 6e67   dict containing
+00015ce0: 2066 7265 712f 7469 6d65 2069 6e66 6f20   freq/time info 
+00015cf0: 6f66 2074 6865 2064 6174 6120 6d61 7472  of the data matr
+00015d00: 6978 0a20 2020 2064 6a2c 2073 302c 204a  ix.    dj, s0, J
+00015d10: 2c20 7369 672c 2077 766e 3a20 636f 6d6d  , sig, wvn: comm
+00015d20: 6f6e 2070 6172 616d 6574 6572 7320 7573  on parameters us
+00015d30: 6564 2069 6e20 2777 6176 656c 6574 2e77  ed in 'wavelet.w
+00015d40: 6374 270a 2020 2020 756e 7772 6170 666c  ct'.    unwrapfl
+00015d50: 6167 3a20 5472 7565 202d 2075 6e77 7261  ag: True - unwra
+00015d60: 7020 7068 6173 6520 6465 6c61 7973 2e20  p phase delays. 
+00015d70: 4465 6661 756c 7420 6973 2046 616c 7365  Default is False
+00015d80: 0a0a 2020 2020 5245 5455 524e 533a 0a20  ..    RETURNS:. 
+00015d90: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+00015da0: 2d2d 2d2d 2d0a 2020 2020 6476 762a 3130  -----.    dvv*10
+00015db0: 3020 3a20 6573 7469 6d61 7465 6420 6476  0 : estimated dv
+00015dc0: 2f76 2069 6e20 250a 2020 2020 6572 722a  /v in %.    err*
+00015dd0: 3130 3020 3a20 6572 726f 7220 6f66 2064  100 : error of d
+00015de0: 762f 7620 6573 7469 6d61 7469 6f6e 2069  v/v estimation i
+00015df0: 6e20 250a 0a20 2020 204f 7269 6769 6e61  n %..    Origina
+00015e00: 6c6c 7920 7772 6974 7465 6e20 6279 2054  lly written by T
+00015e10: 696d 2043 6c65 6d65 6e74 7320 2831 204d  im Clements (1 M
+00015e20: 6172 6368 2c20 3230 3139 290a 2020 2020  arch, 2019).    
+00015e30: 4d6f 6469 6669 6564 2062 7920 436f 6e67  Modified by Cong
+00015e40: 636f 6e67 2059 7561 6e20 2833 3020 4a75  cong Yuan (30 Ju
+00015e50: 6e65 2c20 3230 3139 2920 6261 7365 6420  ne, 2019) based 
+00015e60: 6f6e 2028 4d61 6f20 6574 2061 6c2e 2032  on (Mao et al. 2
+00015e70: 3031 3929 2e0a 2020 2020 5570 6461 7465  019)..    Update
+00015e80: 6420 6279 2043 6865 6e67 7869 6e20 4a69  d by Chengxin Ji
+00015e90: 616e 6720 2831 3020 4f63 742c 2032 3031  ang (10 Oct, 201
+00015ea0: 3929 2074 6f20 6d65 7267 6520 7468 6520  9) to merge the 
+00015eb0: 6675 6e63 7469 6f6e 616c 6974 7920 666f  functionality fo
+00015ec0: 7220 6d65 7375 7265 6d65 6e74 730a 2020  r mesurements.  
+00015ed0: 2020 6163 726f 7373 2061 6c6c 2066 7265    across all fre
+00015ee0: 7175 656e 6379 2061 6e64 206f 6e65 2066  quency and one f
+00015ef0: 7265 7120 7261 6e67 650a 2020 2020 2222  req range.    ""
+00015f00: 220a 2020 2020 2320 636f 6d6d 6f6e 2076  ".    # common v
+00015f10: 6172 6961 626c 6573 0a20 2020 2074 7769  ariables.    twi
+00015f20: 6e20 3d20 7061 7261 5b22 7477 696e 225d  n = para["twin"]
+00015f30: 0a20 2020 2066 7265 7120 3d20 7061 7261  .    freq = para
+00015f40: 5b22 6672 6571 225d 0a20 2020 2064 7420  ["freq"].    dt 
+00015f50: 3d20 7061 7261 5b22 6474 225d 0a20 2020  = para["dt"].   
+00015f60: 2074 6d69 6e20 3d20 6e70 2e6d 696e 2874   tmin = np.min(t
+00015f70: 7769 6e29 0a20 2020 2074 6d61 7820 3d20  win).    tmax = 
+00015f80: 6e70 2e6d 6178 2874 7769 6e29 0a20 2020  np.max(twin).   
+00015f90: 2066 6d69 6e20 3d20 6e70 2e6d 696e 2866   fmin = np.min(f
+00015fa0: 7265 7129 0a20 2020 2066 6d61 7820 3d20  req).    fmax = 
+00015fb0: 6e70 2e6d 6178 2866 7265 7129 0a20 2020  np.max(freq).   
+00015fc0: 2074 7665 6320 3d20 6e70 2e61 7261 6e67   tvec = np.arang
+00015fd0: 6528 746d 696e 2c20 746d 6178 2c20 6474  e(tmin, tmax, dt
+00015fe0: 290a 2020 2020 6e70 7473 203d 206c 656e  ).    npts = len
+00015ff0: 2874 7665 6329 0a0a 2020 2020 2320 7065  (tvec)..    # pe
+00016000: 7266 6f72 6d20 6372 6f73 7320 636f 6865  rform cross cohe
+00016010: 7265 6e74 2061 6e61 6c79 7369 732c 206d  rent analysis, m
+00016020: 6f64 6966 6965 6420 6672 6f6d 2066 756e  odified from fun
+00016030: 6374 696f 6e20 2777 6176 656c 6574 2e63  ction 'wavelet.c
+00016040: 7774 270a 2020 2020 5743 542c 2061 5743  wt'.    WCT, aWC
+00016050: 542c 2063 6f69 2c20 6672 6571 2c20 7369  T, coi, freq, si
+00016060: 6720 3d20 7763 745f 6d6f 6469 6669 6564  g = wct_modified
+00016070: 2872 6566 2c20 6375 722c 2064 742c 2064  (ref, cur, dt, d
+00016080: 6a3d 646a 2c20 7330 3d73 302c 204a 3d4a  j=dj, s0=s0, J=J
+00016090: 2c20 7369 673d 7369 672c 2077 6176 656c  , sig=sig, wavel
+000160a0: 6574 3d77 766e 2c20 6e6f 726d 616c 697a  et=wvn, normaliz
+000160b0: 653d 5472 7565 290a 0a20 2020 2069 6620  e=True)..    if 
+000160c0: 756e 7772 6170 666c 6167 3a0a 2020 2020  unwrapflag:.    
+000160d0: 2020 2020 7068 6173 6520 3d20 6e70 2e75      phase = np.u
+000160e0: 6e77 7261 7028 6157 4354 2c20 6178 6973  nwrap(aWCT, axis
+000160f0: 3d2d 3129 2020 2320 6178 6973 3d30 2c20  =-1)  # axis=0, 
+00016100: 7570 7772 6170 2061 6c6f 6e67 2074 696d  upwrap along tim
+00016110: 653b 2061 7869 733d 2d31 2c20 756e 7772  e; axis=-1, unwr
+00016120: 6170 2061 6c6f 6e67 2066 7265 7175 656e  ap along frequen
+00016130: 6379 0a20 2020 2065 6c73 653a 0a20 2020  cy.    else:.   
+00016140: 2020 2020 2070 6861 7365 203d 2061 5743       phase = aWC
+00016150: 540a 0a20 2020 2023 207a 6572 6f20 6f75  T..    # zero ou
+00016160: 7420 6461 7461 206f 7574 7369 6465 2066  t data outside f
+00016170: 7265 7175 656e 6379 2062 616e 640a 2020  requency band.  
+00016180: 2020 6966 2028 666d 6178 203e 206e 702e    if (fmax > np.
+00016190: 6d61 7828 6672 6571 2929 207c 2028 666d  max(freq)) | (fm
+000161a0: 6178 203c 3d20 666d 696e 293a 0a20 2020  ax <= fmin):.   
+000161b0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+000161c0: 4572 726f 7228 2241 626f 7274 3a20 696e  Error("Abort: in
+000161d0: 7075 7420 6672 6571 7565 6e63 7920 6f75  put frequency ou
+000161e0: 7420 6f66 206c 696d 6974 7321 2229 0a20  t of limits!"). 
+000161f0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00016200: 2066 7265 715f 696e 6469 6e20 3d20 6e70   freq_indin = np
+00016210: 2e77 6865 7265 2828 6672 6571 203e 3d20  .where((freq >= 
+00016220: 666d 696e 2920 2620 2866 7265 7120 3c3d  fmin) & (freq <=
+00016230: 2066 6d61 7829 295b 305d 0a0a 2020 2020   fmax))[0]..    
+00016240: 2320 666f 6c6c 6f77 204d 5743 5320 746f  # follow MWCS to
+00016250: 2064 6f20 7477 6f20 7374 6570 7320 6f66   do two steps of
+00016260: 206c 696e 6561 7220 7265 6772 6573 7369   linear regressi
+00016270: 6f6e 0a20 2020 2069 6620 6e6f 7420 616c  on.    if not al
+00016280: 6c66 7265 713a 0a20 2020 2020 2020 2064  lfreq:.        d
+00016290: 656c 7461 5f74 5f6d 2c20 6465 6c74 615f  elta_t_m, delta_
+000162a0: 745f 756e 6320 3d20 6e70 2e7a 6572 6f73  t_unc = np.zeros
+000162b0: 286e 7074 732c 2064 7479 7065 3d6e 702e  (npts, dtype=np.
+000162c0: 666c 6f61 7433 3229 2c20 6e70 2e7a 6572  float32), np.zer
+000162d0: 6f73 286e 7074 732c 2064 7479 7065 3d6e  os(npts, dtype=n
+000162e0: 702e 666c 6f61 7433 3229 0a20 2020 2020  p.float32).     
+000162f0: 2020 2023 2061 7373 756d 6520 7468 6520     # assume the 
+00016300: 7476 6563 2069 7320 7468 6520 7469 6d65  tvec is the time
+00016310: 2077 696e 646f 7720 746f 206d 6561 7375   window to measu
+00016320: 7265 2064 740a 2020 2020 2020 2020 666f  re dt.        fo
+00016330: 7220 6974 2069 6e20 7261 6e67 6528 6e70  r it in range(np
+00016340: 7473 293a 0a20 2020 2020 2020 2020 2020  ts):.           
+00016350: 2077 203d 2031 202f 2057 4354 5b66 7265   w = 1 / WCT[fre
+00016360: 715f 696e 6469 6e2c 2069 745d 0a20 2020  q_indin, it].   
+00016370: 2020 2020 2020 2020 2077 5b7e 6e70 2e69           w[~np.i
+00016380: 7366 696e 6974 6528 7729 5d20 3d20 312e  sfinite(w)] = 1.
+00016390: 300a 2020 2020 2020 2020 2020 2020 6465  0.            de
+000163a0: 6c74 615f 745f 6d5b 6974 5d2c 2064 656c  lta_t_m[it], del
+000163b0: 7461 5f74 5f75 6e63 5b69 745d 203d 206c  ta_t_unc[it] = l
+000163c0: 696e 6561 725f 7265 6772 6573 7369 6f6e  inear_regression
+000163d0: 2866 7265 715b 6672 6571 5f69 6e64 696e  (freq[freq_indin
+000163e0: 5d20 2a20 3220 2a20 6e70 2e70 692c 2070  ] * 2 * np.pi, p
+000163f0: 6861 7365 5b66 7265 715f 696e 6469 6e2c  hase[freq_indin,
+00016400: 2069 745d 2c20 7729 0a0a 2020 2020 2020   it], w)..      
+00016410: 2020 2320 6e65 7720 7765 6967 6874 7320    # new weights 
+00016420: 666f 7220 7265 6772 6573 7369 6f6e 0a20  for regression. 
+00016430: 2020 2020 2020 2077 3220 3d20 3120 2f20         w2 = 1 / 
+00016440: 6e70 2e6d 6561 6e28 5743 545b 6672 6571  np.mean(WCT[freq
+00016450: 5f69 6e64 696e 2c20 3a5d 2c20 6178 6973  _indin, :], axis
+00016460: 3d30 290a 2020 2020 2020 2020 7732 5b7e  =0).        w2[~
+00016470: 6e70 2e69 7366 696e 6974 6528 7732 295d  np.isfinite(w2)]
+00016480: 203d 2031 2e30 0a0a 2020 2020 2020 2020   = 1.0..        
+00016490: 2320 6e6f 7720 7573 6520 6474 2061 6e64  # now use dt and
+000164a0: 2074 2074 6f20 6765 7420 6476 2f76 0a20   t to get dv/v. 
+000164b0: 2020 2020 2020 2069 6620 6c65 6e28 7732         if len(w2
+000164c0: 2920 3e20 323a 0a20 2020 2020 2020 2020  ) > 2:.         
+000164d0: 2020 2069 6620 6e6f 7420 6e70 2e61 6e79     if not np.any
+000164e0: 2864 656c 7461 5f74 5f6d 293a 0a20 2020  (delta_t_m):.   
+000164f0: 2020 2020 2020 2020 2020 2020 2064 7676               dvv
+00016500: 2c20 6572 7220 3d20 6e70 2e6e 616e 2c20  , err = np.nan, 
+00016510: 6e70 2e6e 616e 0a20 2020 2020 2020 2020  np.nan.         
+00016520: 2020 206d 2c20 656d 203d 206c 696e 6561     m, em = linea
+00016530: 725f 7265 6772 6573 7369 6f6e 2874 7665  r_regression(tve
+00016540: 632c 2064 656c 7461 5f74 5f6d 2c20 7732  c, delta_t_m, w2
+00016550: 2c20 696e 7465 7263 6570 745f 6f72 6967  , intercept_orig
+00016560: 696e 3d54 7275 6529 0a20 2020 2020 2020  in=True).       
+00016570: 2020 2020 2064 7676 2c20 6572 7220 3d20       dvv, err = 
+00016580: 2d6d 2c20 656d 0a20 2020 2020 2020 2065  -m, em.        e
+00016590: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000165a0: 206c 6f67 6765 722e 6465 6275 6728 226e   logger.debug("n
+000165b0: 6f74 2065 6e6f 7567 6820 706f 696e 7473  ot enough points
+000165c0: 2074 6f20 6573 7469 6d61 7465 2064 762f   to estimate dv/
+000165d0: 7620 666f 7220 7774 7322 290a 2020 2020  v for wts").    
+000165e0: 2020 2020 2020 2020 6476 762c 2065 7272          dvv, err
+000165f0: 203d 206e 702e 6e61 6e2c 206e 702e 6e61   = np.nan, np.na
+00016600: 6e0a 0a20 2020 2020 2020 2072 6574 7572  n..        retur
+00016610: 6e20 6476 7620 2a20 3130 302c 2065 7272  n dvv * 100, err
+00016620: 202a 2031 3030 0a0a 2020 2020 2320 636f   * 100..    # co
+00016630: 6e76 6572 7420 7068 6173 6520 6469 7265  nvert phase dire
+00016640: 6374 6c79 2074 6f20 6465 6c74 615f 7420  ctly to delta_t 
+00016650: 666f 7220 616c 6c20 6672 6571 7565 6e63  for all frequenc
+00016660: 6965 730a 2020 2020 656c 7365 3a0a 2020  ies.    else:.  
+00016670: 2020 2020 2020 2320 636f 6e76 6572 7420        # convert 
+00016680: 7068 6173 6520 6465 6c61 7920 746f 2074  phase delay to t
+00016690: 696d 6520 6465 6c61 790a 2020 2020 2020  ime delay.      
+000166a0: 2020 6465 6c74 615f 7420 3d20 7068 6173    delta_t = phas
+000166b0: 6520 2f20 2832 202a 206e 702e 7069 202a  e / (2 * np.pi *
+000166c0: 2066 7265 715b 3a2c 204e 6f6e 655d 2920   freq[:, None]) 
+000166d0: 2023 206e 6f72 6d61 6c69 7a65 2070 6861   # normalize pha
+000166e0: 7365 2062 7920 2832 2a70 692a 6672 6571  se by (2*pi*freq
+000166f0: 7565 6e63 7929 0a20 2020 2020 2020 2064  uency).        d
+00016700: 7676 2c20 6572 7220 3d20 6e70 2e7a 6572  vv, err = np.zer
+00016710: 6f73 2866 7265 715f 696e 6469 6e2e 7368  os(freq_indin.sh
+00016720: 6170 6529 2c20 6e70 2e7a 6572 6f73 2866  ape), np.zeros(f
+00016730: 7265 715f 696e 6469 6e2e 7368 6170 6529  req_indin.shape)
+00016740: 0a0a 2020 2020 2020 2020 2320 6c6f 6f70  ..        # loop
+00016750: 2074 6872 6f75 6768 2066 7265 7120 666f   through freq fo
+00016760: 7220 6c69 6e65 6172 2072 6567 7265 7373  r linear regress
+00016770: 696f 6e0a 2020 2020 2020 2020 666f 7220  ion.        for 
+00016780: 6969 2c20 6966 7265 7120 696e 2065 6e75  ii, ifreq in enu
+00016790: 6d65 7261 7465 2866 7265 715f 696e 6469  merate(freq_indi
+000167a0: 6e29 3a0a 2020 2020 2020 2020 2020 2020  n):.            
+000167b0: 6966 206c 656e 2874 7665 6329 203e 2032  if len(tvec) > 2
+000167c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000167d0: 2020 6966 206e 6f74 206e 702e 616e 7928    if not np.any(
+000167e0: 6465 6c74 615f 745b 6966 7265 715d 293a  delta_t[ifreq]):
+000167f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016800: 2020 2020 2063 6f6e 7469 6e75 650a 0a20       continue.. 
+00016810: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00016820: 2068 6f77 2074 6f20 6265 7474 6572 2061   how to better a
+00016830: 7070 726f 6163 6820 7468 6520 756e 6365  pproach the unce
+00016840: 7274 6169 6e74 7920 6f66 2064 656c 7461  rtainty of delta
+00016850: 5f74 0a20 2020 2020 2020 2020 2020 2020  _t.             
+00016860: 2020 2077 203d 2031 202f 2057 4354 5b69     w = 1 / WCT[i
+00016870: 6672 6571 5d0a 2020 2020 2020 2020 2020  freq].          
+00016880: 2020 2020 2020 775b 7e6e 702e 6973 6669        w[~np.isfi
+00016890: 6e69 7465 2877 295d 203d 2031 2e30 0a0a  nite(w)] = 1.0..
+000168a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168b0: 2320 6d2c 2061 2c20 656d 2c20 6561 203d  # m, a, em, ea =
+000168c0: 206c 696e 6561 725f 7265 6772 6573 7369   linear_regressi
+000168d0: 6f6e 2874 696d 655f 6178 6973 5b69 6e64  on(time_axis[ind
+000168e0: 785d 2c20 6465 6c74 615f 745b 696e 6478  x], delta_t[indx
+000168f0: 5d2c 2077 2c20 696e 7465 7263 6570 745f  ], w, intercept_
+00016900: 6f72 6967 696e 3d46 616c 7365 290a 2020  origin=False).  
+00016910: 2020 2020 2020 2020 2020 2020 2020 6d2c                m,
+00016920: 2065 6d20 3d20 6c69 6e65 6172 5f72 6567   em = linear_reg
+00016930: 7265 7373 696f 6e28 7476 6563 2c20 6465  ression(tvec, de
+00016940: 6c74 615f 745b 6966 7265 715d 2c20 772c  lta_t[ifreq], w,
+00016950: 2069 6e74 6572 6365 7074 5f6f 7269 6769   intercept_origi
+00016960: 6e3d 5472 7565 290a 2020 2020 2020 2020  n=True).        
+00016970: 2020 2020 2020 2020 6476 765b 6969 5d2c          dvv[ii],
+00016980: 2065 7272 5b69 695d 203d 202d 6d2c 2065   err[ii] = -m, e
+00016990: 6d0a 2020 2020 2020 2020 2020 2020 656c  m.            el
+000169a0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000169b0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+000169c0: 2822 6e6f 7420 656e 6f75 6768 2070 6f69  ("not enough poi
+000169d0: 6e74 7320 746f 2065 7374 696d 6174 6520  nts to estimate 
+000169e0: 6476 2f76 2066 6f72 2077 7473 2229 0a20  dv/v for wts"). 
+000169f0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00016a00: 7676 5b69 695d 2c20 6572 725b 6969 5d20  vv[ii], err[ii] 
+00016a10: 3d20 6e70 2e6e 616e 2c20 6e70 2e6e 616e  = np.nan, np.nan
+00016a20: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00016a30: 2066 7265 715b 6672 6571 5f69 6e64 696e   freq[freq_indin
+00016a40: 5d2c 2064 7676 202a 2031 3030 2c20 6572  ], dvv * 100, er
+00016a50: 7220 2a20 3130 300a 0a0a 6465 6620 7774  r * 100...def wt
+00016a60: 735f 6476 7628 0a20 2020 2072 6566 2c0a  s_dvv(.    ref,.
+00016a70: 2020 2020 6375 722c 0a20 2020 2061 6c6c      cur,.    all
+00016a80: 6672 6571 2c0a 2020 2020 7061 7261 2c0a  freq,.    para,.
+00016a90: 2020 2020 6476 5f72 616e 6765 2c0a 2020      dv_range,.  
+00016aa0: 2020 6e62 7472 6961 6c2c 0a20 2020 2064    nbtrial,.    d
+00016ab0: 6a3d 3120 2f20 3132 2c0a 2020 2020 7330  j=1 / 12,.    s0
+00016ac0: 3d2d 312c 0a20 2020 204a 3d2d 312c 0a20  =-1,.    J=-1,. 
+00016ad0: 2020 2077 766e 3d22 6d6f 726c 6574 222c     wvn="morlet",
+00016ae0: 0a20 2020 206e 6f72 6d61 6c69 7a65 3d54  .    normalize=T
+00016af0: 7275 652c 0a29 3a0a 2020 2020 2222 220a  rue,.):.    """.
+00016b00: 2020 2020 4170 706c 7920 7374 7265 7463      Apply stretc
+00016b10: 6869 6e67 206d 6574 686f 6420 746f 2063  hing method to c
+00016b20: 6f6e 7469 6e75 6f75 7320 7761 7665 6c65  ontinuous wavele
+00016b30: 7420 7472 616e 7366 6f72 6d61 7469 6f6e  t transformation
+00016b40: 2028 4357 5429 206f 6620 7369 676e 616c   (CWT) of signal
+00016b50: 730a 2020 2020 666f 7220 616c 6c20 6672  s.    for all fr
+00016b60: 6571 7565 6369 6573 2069 6e20 616e 2069  equecies in an i
+00016b70: 6e74 6572 6573 7420 7261 6e67 650a 0a20  nterest range.. 
+00016b80: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00016b90: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+00016ba0: 0a20 2020 2072 6566 3a20 5468 6520 2252  .    ref: The "R
+00016bb0: 6566 6572 656e 6365 2220 7469 6d65 7365  eference" timese
+00016bc0: 7269 6573 2028 6e75 6d70 792e 6e64 6172  ries (numpy.ndar
+00016bd0: 7261 7929 0a20 2020 2063 7572 3a20 5468  ray).    cur: Th
+00016be0: 6520 2243 7572 7265 6e74 2220 7469 6d65  e "Current" time
+00016bf0: 7365 7269 6573 2028 6e75 6d70 792e 6e64  series (numpy.nd
+00016c00: 6172 7261 7929 0a20 2020 2061 6c6c 6672  array).    allfr
+00016c10: 6571 3a20 6120 626f 6f6c 656e 2076 6172  eq: a boolen var
+00016c20: 6961 626c 6520 746f 206d 616b 6520 6d65  iable to make me
+00016c30: 6173 7572 656d 656e 7473 206f 6e20 616c  asurements on al
+00016c40: 6c20 6672 6571 7565 6e63 7920 7261 6e67  l frequency rang
+00016c50: 6520 6f72 206e 6f74 0a20 2020 2070 6172  e or not.    par
+00016c60: 613a 2061 2064 6963 7420 636f 6e74 6169  a: a dict contai
+00016c70: 6e69 6e67 2066 7265 712f 7469 6d65 2069  ning freq/time i
+00016c80: 6e66 6f20 6f66 2074 6865 2064 6174 6120  nfo of the data 
+00016c90: 6d61 7472 6978 0a20 2020 2064 765f 7261  matrix.    dv_ra
+00016ca0: 6e67 653a 2061 6273 6f6c 7574 6520 626f  nge: absolute bo
+00016cb0: 756e 6420 666f 7220 7468 6520 7665 6c6f  und for the velo
+00016cc0: 6369 7479 2076 6172 6961 7469 6f6e 3b20  city variation; 
+00016cd0: 6578 616d 706c 653a 2064 763d 302e 3033  example: dv=0.03
+00016ce0: 2066 6f72 205b 2d33 2c33 5d25 0a20 2020   for [-3,3]%.   
+00016cf0: 206f 6620 7265 6c61 7469 7665 2076 656c   of relative vel
+00016d00: 6f63 6974 7920 6368 616e 6765 2028 666c  ocity change (fl
+00016d10: 6f61 7429 0a20 2020 206e 6274 7269 616c  oat).    nbtrial
+00016d20: 3a20 6e75 6d62 6572 206f 6620 7374 7265  : number of stre
+00016d30: 7463 6869 6e67 2063 6f65 6666 6963 6965  tching coefficie
+00016d40: 6e74 2062 6574 7765 656e 2064 766d 696e  nt between dvmin
+00016d50: 2061 6e64 2064 766d 6178 2c20 6e6f 206e   and dvmax, no n
+00016d60: 6565 6420 746f 2062 6520 6869 6768 6572  eed to be higher
+00016d70: 2074 6861 6e20 3130 3020 2028 666c 6f61   than 100  (floa
+00016d80: 7429 0a20 2020 2064 6a2c 2073 302c 204a  t).    dj, s0, J
+00016d90: 2c20 7369 672c 2077 766e 3a20 636f 6d6d  , sig, wvn: comm
+00016da0: 6f6e 2070 6172 616d 6574 6572 7320 7573  on parameters us
+00016db0: 6564 2069 6e20 2777 6176 656c 6574 2e77  ed in 'wavelet.w
+00016dc0: 6374 270a 2020 2020 6e6f 726d 616c 697a  ct'.    normaliz
+00016dd0: 653a 206e 6f72 6d61 6c69 7a65 2074 6865  e: normalize the
+00016de0: 2077 6176 656c 6574 2073 7065 6374 7275   wavelet spectru
+00016df0: 6d20 6f72 206e 6f74 2e20 4465 6661 756c  m or not. Defaul
+00016e00: 7420 6973 2054 7275 650a 0a20 2020 2052  t is True..    R
+00016e10: 4554 5552 4e53 3a0a 2020 2020 2d2d 2d2d  ETURNS:.    ----
+00016e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+00016e30: 2020 2064 7676 3a20 6573 7469 6d61 7465     dvv: estimate
+00016e40: 6420 6476 2f76 0a20 2020 2065 7272 3a20  d dv/v.    err: 
+00016e50: 6572 726f 7220 6f66 2064 762f 7620 6573  error of dv/v es
+00016e60: 7469 6d61 7469 6f6e 0a0a 2020 2020 5772  timation..    Wr
+00016e70: 6974 7465 6e20 6279 2043 6f6e 6763 6f6e  itten by Congcon
+00016e80: 6720 5975 616e 2028 3330 204a 756e 2c20  g Yuan (30 Jun, 
+00016e90: 3230 3139 290a 2020 2020 2222 220a 2020  2019).    """.  
+00016ea0: 2020 2320 636f 6d6d 6f6e 2076 6172 6961    # common varia
+00016eb0: 626c 6573 0a20 2020 2066 7265 7120 3d20  bles.    freq = 
+00016ec0: 7061 7261 5b22 6672 6571 225d 0a20 2020  para["freq"].   
+00016ed0: 2064 7420 3d20 7061 7261 5b22 6474 225d   dt = para["dt"]
+00016ee0: 0a20 2020 2066 6d69 6e20 3d20 6e70 2e6d  .    fmin = np.m
+00016ef0: 696e 2866 7265 7129 0a20 2020 2066 6d61  in(freq).    fma
+00016f00: 7820 3d20 6e70 2e6d 6178 2866 7265 7129  x = np.max(freq)
+00016f10: 0a0a 2020 2020 2320 6170 706c 7920 6377  ..    # apply cw
+00016f20: 7420 6f6e 2074 776f 2074 7261 6365 730a  t on two traces.
+00016f30: 2020 2020 6377 7431 2c20 736a 2c20 6672      cwt1, sj, fr
+00016f40: 6571 2c20 636f 692c 205f 2c20 5f20 3d20  eq, coi, _, _ = 
+00016f50: 7079 6377 742e 6377 7428 6375 722c 2064  pycwt.cwt(cur, d
+00016f60: 742c 2064 6a2c 2073 302c 204a 2c20 7776  t, dj, s0, J, wv
+00016f70: 6e29 0a20 2020 2063 7774 322c 2073 6a2c  n).    cwt2, sj,
+00016f80: 2066 7265 712c 2063 6f69 2c20 5f2c 205f   freq, coi, _, _
+00016f90: 203d 2070 7963 7774 2e63 7774 2872 6566   = pycwt.cwt(ref
+00016fa0: 2c20 6474 2c20 646a 2c20 7330 2c20 4a2c  , dt, dj, s0, J,
+00016fb0: 2077 766e 290a 0a20 2020 2023 2065 7874   wvn)..    # ext
+00016fc0: 7261 6374 2072 6561 6c20 7661 6c75 6573  ract real values
+00016fd0: 206f 6620 6377 740a 2020 2020 7263 7774   of cwt.    rcwt
+00016fe0: 312c 2072 6377 7432 203d 206e 702e 7265  1, rcwt2 = np.re
+00016ff0: 616c 2863 7774 3129 2c20 6e70 2e72 6561  al(cwt1), np.rea
+00017000: 6c28 6377 7432 290a 0a20 2020 2023 207a  l(cwt2)..    # z
+00017010: 6572 6f20 6f75 7420 6461 7461 206f 7574  ero out data out
+00017020: 7369 6465 2066 7265 7175 656e 6379 2062  side frequency b
+00017030: 616e 640a 2020 2020 6966 2028 666d 6178  and.    if (fmax
+00017040: 203e 206e 702e 6d61 7828 6672 6571 2929   > np.max(freq))
+00017050: 207c 2028 666d 6178 203c 3d20 666d 696e   | (fmax <= fmin
+00017060: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
+00017070: 2056 616c 7565 4572 726f 7228 2241 626f   ValueError("Abo
+00017080: 7274 3a20 696e 7075 7420 6672 6571 7565  rt: input freque
+00017090: 6e63 7920 6f75 7420 6f66 206c 696d 6974  ncy out of limit
+000170a0: 7321 2229 0a20 2020 2065 6c73 653a 0a20  s!").    else:. 
+000170b0: 2020 2020 2020 2066 7265 715f 696e 6469         freq_indi
+000170c0: 6e20 3d20 6e70 2e77 6865 7265 2828 6672  n = np.where((fr
+000170d0: 6571 203e 3d20 666d 696e 2920 2620 2866  eq >= fmin) & (f
+000170e0: 7265 7120 3c3d 2066 6d61 7829 295b 305d  req <= fmax))[0]
+000170f0: 0a0a 2020 2020 2320 636f 6e76 6572 7420  ..    # convert 
+00017100: 7761 7665 6c65 7420 646f 6d61 696e 2062  wavelet domain b
+00017110: 6163 6b20 746f 2074 696d 6520 646f 6d61  ack to time doma
+00017120: 696e 2028 7e66 696c 7465 7269 6e67 290a  in (~filtering).
+00017130: 2020 2020 6966 206e 6f74 2061 6c6c 6672      if not allfr
+00017140: 6571 3a0a 2020 2020 2020 2020 2320 696e  eq:.        # in
+00017150: 7665 7273 6520 6377 7420 746f 2074 696d  verse cwt to tim
+00017160: 6520 646f 6d61 696e 0a20 2020 2020 2020  e domain.       
+00017170: 2069 6377 7431 203d 2070 7963 7774 2e69   icwt1 = pycwt.i
+00017180: 6377 7428 6377 7431 5b66 7265 715f 696e  cwt(cwt1[freq_in
+00017190: 6469 6e5d 2c20 736a 5b66 7265 715f 696e  din], sj[freq_in
+000171a0: 6469 6e5d 2c20 6474 2c20 646a 2c20 7776  din], dt, dj, wv
+000171b0: 6e29 0a20 2020 2020 2020 2069 6377 7432  n).        icwt2
+000171c0: 203d 2070 7963 7774 2e69 6377 7428 6377   = pycwt.icwt(cw
+000171d0: 7432 5b66 7265 715f 696e 6469 6e5d 2c20  t2[freq_indin], 
+000171e0: 736a 5b66 7265 715f 696e 6469 6e5d 2c20  sj[freq_indin], 
+000171f0: 6474 2c20 646a 2c20 7776 6e29 0a0a 2020  dt, dj, wvn)..  
+00017200: 2020 2020 2020 2320 6173 7375 6d65 2061        # assume a
+00017210: 6c6c 2074 696d 6520 7769 6e64 6f77 2069  ll time window i
+00017220: 7320 7573 6564 0a20 2020 2020 2020 2077  s used.        w
+00017230: 6377 7431 2c20 7763 7774 3220 3d20 6e70  cwt1, wcwt2 = np
+00017240: 2e72 6561 6c28 6963 7774 3129 2c20 6e70  .real(icwt1), np
+00017250: 2e72 6561 6c28 6963 7774 3229 0a0a 2020  .real(icwt2)..  
+00017260: 2020 2020 2020 2320 4e6f 726d 616c 697a        # Normaliz
+00017270: 6573 2062 6f74 6820 7369 676e 616c 732c  es both signals,
+00017280: 2069 6620 6170 7072 6f70 7269 6174 652e   if appropriate.
+00017290: 0a20 2020 2020 2020 2069 6620 6e6f 726d  .        if norm
+000172a0: 616c 697a 653a 0a20 2020 2020 2020 2020  alize:.         
+000172b0: 2020 206e 6377 7431 203d 2028 7763 7774     ncwt1 = (wcwt
+000172c0: 3120 2d20 7763 7774 312e 6d65 616e 2829  1 - wcwt1.mean()
+000172d0: 2920 2f20 7763 7774 312e 7374 6428 290a  ) / wcwt1.std().
+000172e0: 2020 2020 2020 2020 2020 2020 6e63 7774              ncwt
+000172f0: 3220 3d20 2877 6377 7432 202d 2077 6377  2 = (wcwt2 - wcw
+00017300: 7432 2e6d 6561 6e28 2929 202f 2077 6377  t2.mean()) / wcw
+00017310: 7432 2e73 7464 2829 0a20 2020 2020 2020  t2.std().       
+00017320: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00017330: 2020 206e 6377 7431 203d 2077 6377 7431     ncwt1 = wcwt1
+00017340: 0a20 2020 2020 2020 2020 2020 206e 6377  .            ncw
+00017350: 7432 203d 2077 6377 7432 0a0a 2020 2020  t2 = wcwt2..    
+00017360: 2020 2020 2320 7275 6e20 7374 7265 7463      # run stretc
+00017370: 6869 6e67 0a20 2020 2020 2020 2064 7676  hing.        dvv
+00017380: 2c20 6572 722c 2063 632c 2063 6470 203d  , err, cc, cdp =
+00017390: 2073 7472 6574 6368 696e 6728 6e63 7774   stretching(ncwt
+000173a0: 322c 206e 6377 7431 2c20 6476 5f72 616e  2, ncwt1, dv_ran
+000173b0: 6765 2c20 6e62 7472 6961 6c2c 2070 6172  ge, nbtrial, par
+000173c0: 6129 0a20 2020 2020 2020 2072 6574 7572  a).        retur
+000173d0: 6e20 6476 762c 2065 7272 0a0a 2020 2020  n dvv, err..    
+000173e0: 2320 6469 7265 6374 6c79 2074 616b 6520  # directly take 
+000173f0: 6164 7661 6e74 6167 6520 6f66 2074 6865  advantage of the
+00017400: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00017410: 2020 2023 2069 6e69 7469 616c 697a 6520     # initialize 
+00017420: 7661 7269 6162 6c65 0a20 2020 2020 2020  variable.       
+00017430: 206e 6672 6571 203d 206c 656e 2866 7265   nfreq = len(fre
+00017440: 715f 696e 6469 6e29 0a20 2020 2020 2020  q_indin).       
+00017450: 2064 7676 2c20 6363 2c20 6364 702c 2065   dvv, cc, cdp, e
+00017460: 7272 203d 2028 0a20 2020 2020 2020 2020  rr = (.         
+00017470: 2020 206e 702e 7a65 726f 7328 6e66 7265     np.zeros(nfre
+00017480: 712c 2064 7479 7065 3d6e 702e 666c 6f61  q, dtype=np.floa
+00017490: 7433 3229 2c0a 2020 2020 2020 2020 2020  t32),.          
+000174a0: 2020 6e70 2e7a 6572 6f73 286e 6672 6571    np.zeros(nfreq
+000174b0: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
+000174c0: 3332 292c 0a20 2020 2020 2020 2020 2020  32),.           
+000174d0: 206e 702e 7a65 726f 7328 6e66 7265 712c   np.zeros(nfreq,
+000174e0: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+000174f0: 3229 2c0a 2020 2020 2020 2020 2020 2020  2),.            
+00017500: 6e70 2e7a 6572 6f73 286e 6672 6571 2c20  np.zeros(nfreq, 
+00017510: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+00017520: 292c 0a20 2020 2020 2020 2029 0a0a 2020  ),.        )..  
+00017530: 2020 2020 2020 2320 6c6f 6f70 2074 6872        # loop thr
+00017540: 6f75 6768 2065 6163 6820 6672 6571 0a20  ough each freq. 
+00017550: 2020 2020 2020 2066 6f72 2069 692c 2069         for ii, i
+00017560: 6672 6571 2069 6e20 656e 756d 6572 6174  freq in enumerat
+00017570: 6528 6672 6571 5f69 6e64 696e 293a 0a20  e(freq_indin):. 
+00017580: 2020 2020 2020 2020 2020 2023 2070 7265             # pre
+00017590: 7061 7265 2077 696e 646f 7765 6420 6461  pare windowed da
+000175a0: 7461 0a20 2020 2020 2020 2020 2020 2077  ta.            w
+000175b0: 6377 7431 2c20 7763 7774 3220 3d20 7263  cwt1, wcwt2 = rc
+000175c0: 7774 315b 6966 7265 715d 2c20 7263 7774  wt1[ifreq], rcwt
+000175d0: 325b 6966 7265 715d 0a0a 2020 2020 2020  2[ifreq]..      
+000175e0: 2020 2020 2020 2320 4e6f 726d 616c 697a        # Normaliz
+000175f0: 6573 2062 6f74 6820 7369 676e 616c 732c  es both signals,
+00017600: 2069 6620 6170 7072 6f70 7269 6174 652e   if appropriate.
+00017610: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00017620: 6e6f 726d 616c 697a 653a 0a20 2020 2020  normalize:.     
+00017630: 2020 2020 2020 2020 2020 206e 6377 7431             ncwt1
+00017640: 203d 2028 7763 7774 3120 2d20 7763 7774   = (wcwt1 - wcwt
+00017650: 312e 6d65 616e 2829 2920 2f20 7763 7774  1.mean()) / wcwt
+00017660: 312e 7374 6428 290a 2020 2020 2020 2020  1.std().        
+00017670: 2020 2020 2020 2020 6e63 7774 3220 3d20          ncwt2 = 
+00017680: 2877 6377 7432 202d 2077 6377 7432 2e6d  (wcwt2 - wcwt2.m
+00017690: 6561 6e28 2929 202f 2077 6377 7432 2e73  ean()) / wcwt2.s
+000176a0: 7464 2829 0a20 2020 2020 2020 2020 2020  td().           
+000176b0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000176c0: 2020 2020 2020 206e 6377 7431 203d 2077         ncwt1 = w
+000176d0: 6377 7431 0a20 2020 2020 2020 2020 2020  cwt1.           
+000176e0: 2020 2020 206e 6377 7432 203d 2077 6377       ncwt2 = wcw
+000176f0: 7432 0a0a 2020 2020 2020 2020 2020 2020  t2..            
+00017700: 2320 7275 6e20 7374 7265 7463 6869 6e67  # run stretching
+00017710: 0a20 2020 2020 2020 2020 2020 2064 762c  .            dv,
+00017720: 2065 7272 6f72 2c20 6331 2c20 6332 203d   error, c1, c2 =
+00017730: 2073 7472 6574 6368 696e 6728 6e63 7774   stretching(ncwt
+00017740: 322c 206e 6377 7431 2c20 6476 5f72 616e  2, ncwt1, dv_ran
+00017750: 6765 2c20 6e62 7472 6961 6c2c 2070 6172  ge, nbtrial, par
+00017760: 6129 0a20 2020 2020 2020 2020 2020 2064  a).            d
+00017770: 7676 5b69 695d 2c20 6363 5b69 695d 2c20  vv[ii], cc[ii], 
+00017780: 6364 705b 6969 5d2c 2065 7272 5b69 695d  cdp[ii], err[ii]
+00017790: 203d 2064 762c 2063 312c 2063 322c 2065   = dv, c1, c2, e
+000177a0: 7272 6f72 0a0a 2020 2020 2020 2020 7265  rror..        re
+000177b0: 7475 726e 2066 7265 715b 6672 6571 5f69  turn freq[freq_i
+000177c0: 6e64 696e 5d2c 2064 7676 2c20 6572 720a  ndin], dvv, err.
+000177d0: 0a0a 6465 6620 7774 6474 775f 616c 6c66  ..def wtdtw_allf
+000177e0: 7265 7128 0a20 2020 2072 6566 2c0a 2020  req(.    ref,.  
+000177f0: 2020 6375 722c 0a20 2020 2061 6c6c 6672    cur,.    allfr
+00017800: 6571 2c0a 2020 2020 7061 7261 2c0a 2020  eq,.    para,.  
+00017810: 2020 6d61 784c 6167 2c0a 2020 2020 622c    maxLag,.    b,
+00017820: 0a20 2020 2064 6972 6563 7469 6f6e 2c0a  .    direction,.
+00017830: 2020 2020 646a 3d31 202f 2031 322c 0a20      dj=1 / 12,. 
+00017840: 2020 2073 303d 2d31 2c0a 2020 2020 4a3d     s0=-1,.    J=
+00017850: 2d31 2c0a 2020 2020 7776 6e3d 226d 6f72  -1,.    wvn="mor
+00017860: 6c65 7422 2c0a 2020 2020 6e6f 726d 616c  let",.    normal
+00017870: 697a 653d 5472 7565 2c0a 293a 0a20 2020  ize=True,.):.   
+00017880: 2022 2222 0a20 2020 2041 7070 6c79 2064   """.    Apply d
+00017890: 796e 616d 6963 2074 696d 6520 7761 7270  ynamic time warp
+000178a0: 696e 6720 6d65 7468 6f64 2074 6f20 636f  ing method to co
+000178b0: 6e74 696e 756f 7573 2077 6176 656c 6574  ntinuous wavelet
+000178c0: 2074 7261 6e73 666f 726d 6174 696f 6e20   transformation 
+000178d0: 2843 5754 2920 6f66 2073 6967 6e61 6c73  (CWT) of signals
+000178e0: 0a20 2020 2066 6f72 2061 6c6c 2066 7265  .    for all fre
+000178f0: 7175 6563 6965 7320 696e 2061 6e20 696e  quecies in an in
+00017900: 7465 7265 7374 2072 616e 6765 0a0a 2020  terest range..  
+00017910: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00017920: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a   --------------.
+00017930: 2020 2020 7265 663a 2054 6865 2022 5265      ref: The "Re
+00017940: 6665 7265 6e63 6522 2074 696d 6573 6572  ference" timeser
+00017950: 6965 7320 286e 756d 7079 2e6e 6461 7272  ies (numpy.ndarr
+00017960: 6179 290a 2020 2020 6375 723a 2054 6865  ay).    cur: The
+00017970: 2022 4375 7272 656e 7422 2074 696d 6573   "Current" times
+00017980: 6572 6965 7320 286e 756d 7079 2e6e 6461  eries (numpy.nda
+00017990: 7272 6179 290a 2020 2020 616c 6c66 7265  rray).    allfre
+000179a0: 713a 2061 2062 6f6f 6c65 6e20 7661 7269  q: a boolen vari
+000179b0: 6162 6c65 2074 6f20 6d61 6b65 206d 6561  able to make mea
+000179c0: 7375 7265 6d65 6e74 7320 6f6e 2061 6c6c  surements on all
+000179d0: 2066 7265 7175 656e 6379 2072 616e 6765   frequency range
+000179e0: 206f 7220 6e6f 740a 2020 2020 6d61 784c   or not.    maxL
+000179f0: 6167 3a20 6d61 7820 6e75 6d62 6572 206f  ag: max number o
+00017a00: 6620 706f 696e 7473 2074 6f20 7365 6172  f points to sear
+00017a10: 6368 2066 6f72 7761 7264 2061 6e64 2062  ch forward and b
+00017a20: 6163 6b77 6172 642e 0a20 2020 2062 3a20  ackward..    b: 
+00017a30: 622d 7661 6c75 6520 746f 206c 696d 6974  b-value to limit
+00017a40: 2073 7472 6169 6e2c 2077 6869 6368 2069   strain, which i
+00017a50: 7320 746f 206c 696d 6974 2074 6865 206d  s to limit the m
+00017a60: 6178 696d 756d 2076 656c 6f63 6974 7920  aximum velocity 
+00017a70: 7065 7274 7572 6261 7469 6f6e 2e0a 2020  perturbation..  
+00017a80: 2020 5365 6520 6571 7561 7469 6f6e 2031    See equation 1
+00017a90: 3120 696e 2028 4d69 6b65 7365 6c6c 2065  1 in (Mikesell e
+00017aa0: 7420 616c 2e20 3230 3135 290a 2020 2020  t al. 2015).    
+00017ab0: 6469 7265 6374 696f 6e3a 2064 6972 6563  direction: direc
+00017ac0: 7469 6f6e 2074 6f20 6163 6375 6d75 6c61  tion to accumula
+00017ad0: 7465 2065 7272 6f72 7320 2831 3d66 6f72  te errors (1=for
+00017ae0: 7761 7264 2c20 2d31 3d62 6163 6b77 6172  ward, -1=backwar
+00017af0: 6429 0a20 2020 2064 6a2c 2073 302c 204a  d).    dj, s0, J
+00017b00: 2c20 7369 672c 2077 766e 3a20 636f 6d6d  , sig, wvn: comm
+00017b10: 6f6e 2070 6172 616d 6574 6572 7320 7573  on parameters us
+00017b20: 6564 2069 6e20 2777 6176 656c 6574 2e77  ed in 'wavelet.w
+00017b30: 6374 270a 2020 2020 6e6f 726d 616c 697a  ct'.    normaliz
+00017b40: 653a 206e 6f72 6d61 6c69 7a65 2074 6865  e: normalize the
+00017b50: 2077 6176 656c 6574 2073 7065 6374 7275   wavelet spectru
+00017b60: 6d20 6f72 206e 6f74 2e20 4465 6661 756c  m or not. Defaul
+00017b70: 7420 6973 2054 7275 650a 0a20 2020 2052  t is True..    R
+00017b80: 4554 5552 4e53 3a0a 2020 2020 2d2d 2d2d  ETURNS:.    ----
+00017b90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+00017ba0: 2020 2064 7676 3a20 6573 7469 6d61 7465     dvv: estimate
+00017bb0: 6420 6476 2f76 0a20 2020 2065 7272 3a20  d dv/v.    err: 
+00017bc0: 6572 726f 7220 6f66 2064 762f 7620 6573  error of dv/v es
+00017bd0: 7469 6d61 7469 6f6e 0a0a 2020 2020 5772  timation..    Wr
+00017be0: 6974 7465 6e20 6279 2043 6f6e 6763 6f6e  itten by Congcon
+00017bf0: 6720 5975 616e 2028 3330 204a 756e 2c20  g Yuan (30 Jun, 
+00017c00: 3230 3139 290a 2020 2020 2222 220a 2020  2019).    """.  
+00017c10: 2020 2320 636f 6d6d 6f6e 2076 6172 6961    # common varia
+00017c20: 626c 6573 0a20 2020 2066 7265 7120 3d20  bles.    freq = 
+00017c30: 7061 7261 5b22 6672 6571 225d 0a20 2020  para["freq"].   
+00017c40: 2064 7420 3d20 7061 7261 5b22 6474 225d   dt = para["dt"]
+00017c50: 0a20 2020 2066 6d69 6e20 3d20 6e70 2e6d  .    fmin = np.m
+00017c60: 696e 2866 7265 7129 0a20 2020 2066 6d61  in(freq).    fma
+00017c70: 7820 3d20 6e70 2e6d 6178 2866 7265 7129  x = np.max(freq)
+00017c80: 0a0a 2020 2020 2320 6170 706c 7920 6377  ..    # apply cw
+00017c90: 7420 6f6e 2074 776f 2074 7261 6365 730a  t on two traces.
+00017ca0: 2020 2020 6377 7431 2c20 736a 2c20 6672      cwt1, sj, fr
+00017cb0: 6571 2c20 636f 692c 205f 2c20 5f20 3d20  eq, coi, _, _ = 
+00017cc0: 7079 6377 742e 6377 7428 6375 722c 2064  pycwt.cwt(cur, d
+00017cd0: 742c 2064 6a2c 2073 302c 204a 2c20 7776  t, dj, s0, J, wv
+00017ce0: 6e29 0a20 2020 2063 7774 322c 2073 6a2c  n).    cwt2, sj,
+00017cf0: 2066 7265 712c 2063 6f69 2c20 5f2c 205f   freq, coi, _, _
+00017d00: 203d 2070 7963 7774 2e63 7774 2872 6566   = pycwt.cwt(ref
+00017d10: 2c20 6474 2c20 646a 2c20 7330 2c20 4a2c  , dt, dj, s0, J,
+00017d20: 2077 766e 290a 0a20 2020 2023 2065 7874   wvn)..    # ext
+00017d30: 7261 6374 2072 6561 6c20 7661 6c75 6573  ract real values
+00017d40: 206f 6620 6377 740a 2020 2020 7263 7774   of cwt.    rcwt
+00017d50: 312c 2072 6377 7432 203d 206e 702e 7265  1, rcwt2 = np.re
+00017d60: 616c 2863 7774 3129 2c20 6e70 2e72 6561  al(cwt1), np.rea
+00017d70: 6c28 6377 7432 290a 0a20 2020 2023 207a  l(cwt2)..    # z
+00017d80: 6572 6f20 6f75 7420 636f 6e65 206f 6620  ero out cone of 
+00017d90: 696e 666c 7565 6e63 6520 616e 6420 6461  influence and da
+00017da0: 7461 206f 7574 7369 6465 2066 7265 7175  ta outside frequ
+00017db0: 656e 6379 2062 616e 640a 2020 2020 6966  ency band.    if
+00017dc0: 2028 666d 6178 203e 206e 702e 6d61 7828   (fmax > np.max(
+00017dd0: 6672 6571 2929 207c 2028 666d 6178 203c  freq)) | (fmax <
+00017de0: 3d20 666d 696e 293a 0a20 2020 2020 2020  = fmin):.       
+00017df0: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00017e00: 7228 2241 626f 7274 3a20 696e 7075 7420  r("Abort: input 
+00017e10: 6672 6571 7565 6e63 7920 6f75 7420 6f66  frequency out of
+00017e20: 206c 696d 6974 7321 2229 0a20 2020 2065   limits!").    e
+00017e30: 6c73 653a 0a20 2020 2020 2020 2066 7265  lse:.        fre
+00017e40: 715f 696e 6469 6e20 3d20 6e70 2e77 6865  q_indin = np.whe
+00017e50: 7265 2828 6672 6571 203e 3d20 666d 696e  re((freq >= fmin
+00017e60: 2920 2620 2866 7265 7120 3c3d 2066 6d61  ) & (freq <= fma
+00017e70: 7829 295b 305d 0a0a 2020 2020 2020 2020  x))[0]..        
+00017e80: 2320 5573 6520 4454 5720 6d65 7468 6f64  # Use DTW method
+00017e90: 2074 6f20 6578 7472 6163 7420 6476 760a   to extract dvv.
+00017ea0: 2020 2020 2020 2020 6e66 7265 7120 3d20          nfreq = 
+00017eb0: 6c65 6e28 6672 6571 5f69 6e64 696e 290a  len(freq_indin).
+00017ec0: 2020 2020 2020 2020 6476 762c 2065 7272          dvv, err
+00017ed0: 203d 206e 702e 7a65 726f 7328 6e66 7265   = np.zeros(nfre
+00017ee0: 712c 2064 7479 7065 3d6e 702e 666c 6f61  q, dtype=np.floa
+00017ef0: 7433 3229 2c20 6e70 2e7a 6572 6f73 286e  t32), np.zeros(n
+00017f00: 6672 6571 2c20 6474 7970 653d 6e70 2e66  freq, dtype=np.f
+00017f10: 6c6f 6174 3332 290a 0a20 2020 2020 2020  loat32)..       
+00017f20: 2066 6f72 2069 692c 2069 6672 6571 2069   for ii, ifreq i
+00017f30: 6e20 656e 756d 6572 6174 6528 6672 6571  n enumerate(freq
+00017f40: 5f69 6e64 696e 293a 0a20 2020 2020 2020  _indin):.       
+00017f50: 2020 2020 2023 2070 7265 7061 7265 2077       # prepare w
+00017f60: 696e 646f 7765 6420 6461 7461 0a20 2020  indowed data.   
+00017f70: 2020 2020 2020 2020 2077 6377 7431 2c20           wcwt1, 
+00017f80: 7763 7774 3220 3d20 7263 7774 315b 6966  wcwt2 = rcwt1[if
+00017f90: 7265 715d 2c20 7263 7774 325b 6966 7265  req], rcwt2[ifre
+00017fa0: 715d 0a20 2020 2020 2020 2020 2020 2023  q].            #
+00017fb0: 204e 6f72 6d61 6c69 7a65 7320 626f 7468   Normalizes both
+00017fc0: 2073 6967 6e61 6c73 2c20 6966 2061 7070   signals, if app
+00017fd0: 726f 7072 6961 7465 2e0a 2020 2020 2020  ropriate..      
+00017fe0: 2020 2020 2020 6966 206e 6f72 6d61 6c69        if normali
+00017ff0: 7a65 3a0a 2020 2020 2020 2020 2020 2020  ze:.            
+00018000: 2020 2020 6e63 7774 3120 3d20 2877 6377      ncwt1 = (wcw
+00018010: 7431 202d 2077 6377 7431 2e6d 6561 6e28  t1 - wcwt1.mean(
+00018020: 2929 202f 2077 6377 7431 2e73 7464 2829  )) / wcwt1.std()
+00018030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018040: 206e 6377 7432 203d 2028 7763 7774 3220   ncwt2 = (wcwt2 
+00018050: 2d20 7763 7774 322e 6d65 616e 2829 2920  - wcwt2.mean()) 
+00018060: 2f20 7763 7774 322e 7374 6428 290a 2020  / wcwt2.std().  
+00018070: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00018080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018090: 6e63 7774 3120 3d20 7763 7774 310a 2020  ncwt1 = wcwt1.  
+000180a0: 2020 2020 2020 2020 2020 2020 2020 6e63                nc
+000180b0: 7774 3220 3d20 7763 7774 320a 0a20 2020  wt2 = wcwt2..   
+000180c0: 2020 2020 2020 2020 2023 2072 756e 2064           # run d
+000180d0: 7477 0a20 2020 2020 2020 2020 2020 2064  tw.            d
+000180e0: 762c 2065 7272 6f72 2c20 6469 7374 203d  v, error, dist =
+000180f0: 2064 7477 5f64 7676 286e 6377 7432 2c20   dtw_dvv(ncwt2, 
+00018100: 6e63 7774 312c 2070 6172 612c 206d 6178  ncwt1, para, max
+00018110: 4c61 672c 2062 2c20 6469 7265 6374 696f  Lag, b, directio
+00018120: 6e29 0a20 2020 2020 2020 2020 2020 2064  n).            d
+00018130: 7676 5b69 695d 2c20 6572 725b 6969 5d20  vv[ii], err[ii] 
+00018140: 3d20 6476 2c20 6572 726f 720a 0a20 2020  = dv, error..   
+00018150: 2064 656c 2063 7774 312c 2063 7774 322c   del cwt1, cwt2,
+00018160: 2072 6377 7431 2c20 7263 7774 322c 206e   rcwt1, rcwt2, n
+00018170: 6377 7431 2c20 6e63 7774 322c 2077 6377  cwt1, ncwt2, wcw
+00018180: 7431 2c20 7763 7774 322c 2063 6f69 2c20  t1, wcwt2, coi, 
+00018190: 736a 2c20 6469 7374 0a0a 2020 2020 6966  sj, dist..    if
+000181a0: 206e 6f74 2061 6c6c 6672 6571 3a0a 2020   not allfreq:.  
+000181b0: 2020 2020 2020 7265 7475 726e 206e 702e        return np.
+000181c0: 6d65 616e 2864 7676 292c 206e 702e 6d65  mean(dvv), np.me
+000181d0: 616e 2865 7272 290a 2020 2020 656c 7365  an(err).    else
+000181e0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+000181f0: 2066 7265 715b 6672 6571 5f69 6e64 696e   freq[freq_indin
+00018200: 5d2c 2064 7676 2c20 6572 720a 0a0a 2323  ], dvv, err...##
+00018210: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018220: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018230: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018240: 2323 2323 2323 2323 2323 230a 2323 2323  ###########.####
+00018250: 2323 2323 2323 2323 2323 2323 204d 4f4e  ############ MON
+00018260: 4954 4f52 494e 4720 5554 494c 4954 5920  ITORING UTILITY 
+00018270: 4655 4e43 5449 4f4e 5320 2323 2323 2323  FUNCTIONS ######
+00018280: 2323 2323 2323 2323 230a 2323 2323 2323  #########.######
+00018290: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000182a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000182b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000182c0: 2323 2323 2323 230a 0a22 2222 0a62 656c  #######..""".bel
+000182d0: 6f77 2061 7265 2061 7373 656d 626c 7920  ow are assembly 
+000182e0: 6f66 2074 6865 206d 6f6e 6974 6f72 696e  of the monitorin
+000182f0: 6720 7574 696c 6974 7920 6675 6e63 7469  g utility functi
+00018300: 6f6e 7320 6361 6c6c 6564 2062 7920 6d6f  ons called by mo
+00018310: 6e69 746f 7269 6e67 2066 756e 6374 696f  nitoring functio
+00018320: 6e73 0a22 2222 0a0a 0a64 6566 2073 6d6f  ns."""...def smo
+00018330: 6f74 6828 782c 2077 696e 646f 773d 2262  oth(x, window="b
+00018340: 6f78 6361 7222 2c20 6861 6c66 5f77 696e  oxcar", half_win
+00018350: 3d33 293a 0a20 2020 2022 2222 0a20 2020  =3):.    """.   
+00018360: 2070 6572 666f 726d 7320 736d 6f6f 7468   performs smooth
+00018370: 696e 6720 696e 2069 6e74 6572 6573 7465  ing in intereste
+00018380: 6420 7469 6d65 2077 696e 646f 770a 0a20  d time window.. 
+00018390: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+000183a0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+000183b0: 0a20 2020 2078 3a20 7469 6d65 7365 7269  .    x: timeseri
+000183c0: 7320 6461 7461 0a20 2020 2077 696e 646f  s data.    windo
+000183d0: 773a 2074 7970 6573 206f 6620 7769 6e64  w: types of wind
+000183e0: 6f77 2074 6f20 646f 2073 6d6f 6f74 6869  ow to do smoothi
+000183f0: 6e67 0a20 2020 2068 616c 665f 7769 6e3a  ng.    half_win:
+00018400: 2068 616c 6620 7769 6e64 6f77 206c 656e   half window len
+00018410: 6774 680a 0a20 2020 2052 4554 5552 4e53  gth..    RETURNS
+00018420: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  :.    ----------
+00018430: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2079 3a20  --------.    y: 
+00018440: 736d 6f6f 7468 6564 2074 696d 6520 7769  smoothed time wi
+00018450: 6e64 6f77 0a20 2020 2022 2222 0a20 2020  ndow.    """.   
+00018460: 2023 2054 4f44 4f3a 2064 6f63 7374 696e   # TODO: docstin
+00018470: 670a 2020 2020 7769 6e64 6f77 5f6c 656e  g.    window_len
+00018480: 203d 2032 202a 2068 616c 665f 7769 6e20   = 2 * half_win 
+00018490: 2b20 310a 2020 2020 2320 6578 7465 6e64  + 1.    # extend
+000184a0: 696e 6720 7468 6520 6461 7461 2061 7420  ing the data at 
+000184b0: 6265 6769 6e6e 696e 6720 616e 6420 6174  beginning and at
+000184c0: 2074 6865 2065 6e64 0a20 2020 2023 2074   the end.    # t
+000184d0: 6f20 6170 706c 7920 7468 6520 7769 6e64  o apply the wind
+000184e0: 6f77 2061 7420 7468 6520 626f 7264 6572  ow at the border
+000184f0: 730a 2020 2020 7320 3d20 6e70 2e72 5f5b  s.    s = np.r_[
+00018500: 785b 7769 6e64 6f77 5f6c 656e 202d 2031  x[window_len - 1
+00018510: 203a 2030 203a 202d 315d 2c20 782c 2078   : 0 : -1], x, x
+00018520: 5b2d 313a 2d77 696e 646f 775f 6c65 6e3a  [-1:-window_len:
+00018530: 2d31 5d5d 0a20 2020 2069 6620 7769 6e64  -1]].    if wind
+00018540: 6f77 203d 3d20 2262 6f78 6361 7222 3a0a  ow == "boxcar":.
+00018550: 2020 2020 2020 2020 7720 3d20 7363 6970          w = scip
+00018560: 792e 7369 676e 616c 2e62 6f78 6361 7228  y.signal.boxcar(
+00018570: 7769 6e64 6f77 5f6c 656e 292e 6173 7479  window_len).asty
+00018580: 7065 2822 636f 6d70 6c65 7822 290a 2020  pe("complex").  
+00018590: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000185a0: 7720 3d20 7363 6970 792e 7369 676e 616c  w = scipy.signal
+000185b0: 2e68 616e 6e69 6e67 2877 696e 646f 775f  .hanning(window_
+000185c0: 6c65 6e29 2e61 7374 7970 6528 2263 6f6d  len).astype("com
+000185d0: 706c 6578 2229 0a20 2020 2079 203d 206e  plex").    y = n
+000185e0: 702e 636f 6e76 6f6c 7665 2877 202f 2077  p.convolve(w / w
+000185f0: 2e73 756d 2829 2c20 732c 206d 6f64 653d  .sum(), s, mode=
+00018600: 2276 616c 6964 2229 0a20 2020 2072 6574  "valid").    ret
+00018610: 7572 6e20 795b 6861 6c66 5f77 696e 203a  urn y[half_win :
+00018620: 206c 656e 2879 2920 2d20 6861 6c66 5f77   len(y) - half_w
+00018630: 696e 5d0a 0a0a 6465 6620 6e65 7874 706f  in]...def nextpo
+00018640: 7732 2878 293a 0a20 2020 2022 2222 0a20  w2(x):.    """. 
+00018650: 2020 2052 6574 7572 6e73 2074 6865 206e     Returns the n
+00018660: 6578 7420 706f 7765 7220 6f66 2032 206f  ext power of 2 o
+00018670: 6620 782e 0a20 2020 2022 2222 0a20 2020  f x..    """.   
+00018680: 2072 6574 7572 6e20 696e 7428 6e70 2e63   return int(np.c
+00018690: 6569 6c28 6e70 2e6c 6f67 3228 6e70 2e61  eil(np.log2(np.a
+000186a0: 6273 2878 2929 2929 0a0a 0a64 6566 2067  bs(x))))...def g
+000186b0: 6574 436f 6865 7265 6e63 6528 6463 732c  etCoherence(dcs,
+000186c0: 2064 7331 2c20 6473 3229 3a0a 2020 2020   ds1, ds2):.    
+000186d0: 2222 220a 2020 2020 6765 7420 6372 6f73  """.    get cros
+000186e0: 7320 636f 6865 7265 6e63 6520 6265 7477  s coherence betw
+000186f0: 6565 6e20 7265 6665 7265 6e63 6520 616e  een reference an
+00018700: 6420 6375 7272 656e 7420 7761 7665 666f  d current wavefo
+00018710: 726d 7320 666f 6c6c 6f77 696e 6720 6571  rms following eq
+00018720: 7561 7469 6f6e 206f 6620 4133 2069 6e20  uation of A3 in 
+00018730: 436c 6172 6b20 6574 2061 6c2e 2c20 3230  Clark et al., 20
+00018740: 3131 0a0a 2020 2020 5061 7261 6d65 7465  11..    Paramete
+00018750: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+00018760: 2d2d 2d2d 2d0a 2020 2020 6463 733a 2061  -----.    dcs: a
+00018770: 6d70 6c69 7475 6465 206f 6620 7468 6520  mplitude of the 
+00018780: 6372 6f73 7320 7370 6563 7472 756d 0a20  cross spectrum. 
+00018790: 2020 2064 7331 3a20 616d 706c 6974 7564     ds1: amplitud
+000187a0: 6520 6f66 2074 6865 2073 7065 6374 7275  e of the spectru
+000187b0: 6d20 6f66 2063 7572 7265 6e74 2077 6176  m of current wav
+000187c0: 6566 6f72 6d0a 2020 2020 6473 323a 2061  eform.    ds2: a
+000187d0: 6d70 6c69 7475 6465 206f 6620 7468 6520  mplitude of the 
+000187e0: 7370 6563 7472 756d 206f 6620 7265 6665  spectrum of refe
+000187f0: 7265 6e63 6520 7761 7665 666f 726d 0a0a  rence waveform..
+00018800: 2020 2020 5245 5455 524e 533a 0a20 2020      RETURNS:.   
+00018810: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00018820: 2d2d 2d0a 2020 2020 636f 683a 2063 6f68  ---.    coh: coh
+00018830: 7265 7265 6e63 7920 6d61 7472 6978 2075  rerency matrix u
+00018840: 7365 6420 666f 7220 6573 7469 6d61 7465  sed for estimate
+00018850: 2074 6865 2072 6f62 7573 746e 6573 7320   the robustness 
+00018860: 6f66 2074 6865 2063 726f 7373 2073 7065  of the cross spe
+00018870: 6374 7275 6d0a 2020 2020 2222 220a 2020  ctrum.    """.  
+00018880: 2020 6e20 3d20 6c65 6e28 6463 7329 0a20    n = len(dcs). 
+00018890: 2020 2063 6f68 203d 206e 702e 7a65 726f     coh = np.zero
+000188a0: 7328 6e29 2e61 7374 7970 6528 2263 6f6d  s(n).astype("com
+000188b0: 706c 6578 2229 0a20 2020 2076 616c 6964  plex").    valid
+000188c0: 7320 3d20 6e70 2e61 7267 7768 6572 6528  s = np.argwhere(
+000188d0: 6e70 2e6c 6f67 6963 616c 5f61 6e64 286e  np.logical_and(n
+000188e0: 702e 6162 7328 6473 3129 203e 2030 2c20  p.abs(ds1) > 0, 
+000188f0: 6e70 2e61 6273 2864 7332 2920 3e20 3029  np.abs(ds2) > 0)
+00018900: 290a 2020 2020 636f 685b 7661 6c69 6473  ).    coh[valids
+00018910: 5d20 3d20 6463 735b 7661 6c69 6473 5d20  ] = dcs[valids] 
+00018920: 2f20 2864 7331 5b76 616c 6964 735d 202a  / (ds1[valids] *
+00018930: 2064 7332 5b76 616c 6964 735d 290a 2020   ds2[valids]).  
+00018940: 2020 636f 685b 636f 6820 3e20 2831 2e30    coh[coh > (1.0
+00018950: 202b 2030 6a29 5d20 3d20 312e 3020 2b20   + 0j)] = 1.0 + 
+00018960: 306a 0a20 2020 2072 6574 7572 6e20 636f  0j.    return co
+00018970: 680a 0a0a 6465 6620 636f 6d70 7574 6545  h...def computeE
+00018980: 7272 6f72 4675 6e63 7469 6f6e 2875 312c  rrorFunction(u1,
+00018990: 2075 302c 206e 5361 6d70 6c65 2c20 6c61   u0, nSample, la
+000189a0: 672c 206e 6f72 6d3d 224c 3222 293a 0a20  g, norm="L2"):. 
+000189b0: 2020 2022 2222 0a20 2020 2063 6f6d 7075     """.    compu
+000189c0: 7465 2045 7272 6f72 2046 756e 6374 696f  te Error Functio
+000189d0: 6e20 7573 6564 2069 6e20 4454 572e 2054  n used in DTW. T
+000189e0: 6865 2065 7272 6f72 2066 756e 6374 696f  he error functio
+000189f0: 6e20 6973 2065 7175 6174 696f 6e20 3120  n is equation 1 
+00018a00: 696e 2048 616c 652c 2032 3031 332e 2059  in Hale, 2013. Y
+00018a10: 6f75 2063 6f75 6c64 2075 6e63 6f6d 6d65  ou could uncomme
+00018a20: 6e74 2074 6865 0a20 2020 204c 3120 6e6f  nt the.    L1 no
+00018a30: 726d 2061 6e64 2063 6f6d 6d65 6e74 2074  rm and comment t
+00018a40: 6865 204c 3220 6e6f 726d 2069 6620 796f  he L2 norm if yo
+00018a50: 7520 7761 6e74 206f 6e20 4c69 6e65 2032  u want on Line 2
+00018a60: 390a 0a20 2020 2050 6172 616d 6574 6572  9..    Parameter
+00018a70: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+00018a80: 2d2d 2d2d 0a20 2020 2075 313a 2020 7472  ----.    u1:  tr
+00018a90: 6163 6520 7468 6174 2077 6520 7761 6e74  ace that we want
+00018aa0: 2074 6f20 7761 7270 3b20 7369 7a65 203d   to warp; size =
+00018ab0: 2028 6e73 616d 702c 3129 0a20 2020 2075   (nsamp,1).    u
+00018ac0: 303a 2020 7265 6665 7265 6e63 6520 7472  0:  reference tr
+00018ad0: 6163 6520 746f 2063 6f6d 7061 7265 2077  ace to compare w
+00018ae0: 6974 683a 2073 697a 6520 3d20 286e 7361  ith: size = (nsa
+00018af0: 6d70 2c31 290a 2020 2020 6e53 616d 706c  mp,1).    nSampl
+00018b00: 653a 206e 756d 6572 206f 6620 706f 696e  e: numer of poin
+00018b10: 7473 2074 6f20 636f 6d70 6172 6520 696e  ts to compare in
+00018b20: 2074 6865 2074 7261 6365 730a 2020 2020   the traces.    
+00018b30: 6c61 673a 206d 6178 696d 756d 206c 6167  lag: maximum lag
+00018b40: 2069 6e20 7361 6d70 6c65 206e 756d 6265   in sample numbe
+00018b50: 7220 746f 2073 6561 7263 680a 2020 2020  r to search.    
+00018b60: 6e6f 726d 3a20 274c 3227 206f 7220 274c  norm: 'L2' or 'L
+00018b70: 3127 2028 6465 6661 756c 7420 6973 2027  1' (default is '
+00018b80: 4c32 2729 0a0a 2020 2020 5245 5455 524e  L2')..    RETURN
+00018b90: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
+00018ba0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6572  ---------.    er
+00018bb0: 723a 2074 6865 2032 4420 6572 726f 7220  r: the 2D error 
+00018bc0: 6675 6e63 7469 6f6e 3b20 7369 7a65 203d  function; size =
+00018bd0: 2028 6e73 616d 702c 322a 6c61 672b 3129   (nsamp,2*lag+1)
+00018be0: 0a0a 2020 2020 4f72 6967 696e 616c 2062  ..    Original b
+00018bf0: 7920 4469 2059 616e 670a 2020 2020 4c61  y Di Yang.    La
+00018c00: 7374 206d 6f64 6966 6965 6420 6279 2044  st modified by D
+00018c10: 796c 616e 204d 696b 6573 656c 6c20 2832  ylan Mikesell (2
+00018c20: 3520 4665 622e 2032 3031 3529 0a20 2020  5 Feb. 2015).   
+00018c30: 2054 7261 6e73 6c61 7465 6420 746f 2070   Translated to p
+00018c40: 7974 686f 6e20 6279 2054 696d 2043 6c65  ython by Tim Cle
+00018c50: 6d65 6e74 7320 2831 3720 4175 672e 2032  ments (17 Aug. 2
+00018c60: 3031 3829 0a0a 2020 2020 2222 220a 0a20  018)..    """.. 
+00018c70: 2020 2069 6620 6c61 6720 3e3d 206e 5361     if lag >= nSa
+00018c80: 6d70 6c65 3a0a 2020 2020 2020 2020 7261  mple:.        ra
+00018c90: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+00018ca0: 636f 6d70 7574 6545 7272 6f72 4675 6e63  computeErrorFunc
+00018cb0: 7469 6f6e 3a6c 6167 5072 6f62 6c65 6d22  tion:lagProblem"
+00018cc0: 2c20 226c 6167 206d 7573 7420 6265 2073  , "lag must be s
+00018cd0: 6d61 6c6c 6572 2074 6861 6e20 6e53 616d  maller than nSam
+00018ce0: 706c 6522 290a 0a20 2020 2023 2041 6c6c  ple")..    # All
+00018cf0: 6f63 6174 6520 6572 726f 7220 6675 6e63  ocate error func
+00018d00: 7469 6f6e 2076 6172 6961 626c 650a 2020  tion variable.  
+00018d10: 2020 6572 7220 3d20 6e70 2e7a 6572 6f73    err = np.zeros
+00018d20: 285b 6e53 616d 706c 652c 2032 202a 206c  ([nSample, 2 * l
+00018d30: 6167 202b 2031 5d29 0a0a 2020 2020 2320  ag + 1])..    # 
+00018d40: 696e 6974 6961 6c20 6572 726f 7220 6361  initial error ca
+00018d50: 6c63 756c 6174 696f 6e0a 2020 2020 2320  lculation.    # 
+00018d60: 6c6f 6f70 206f 7665 7220 6c61 6773 0a20  loop over lags. 
+00018d70: 2020 2066 6f72 206c 6c20 696e 206e 702e     for ll in np.
+00018d80: 6172 616e 6765 282d 6c61 672c 206c 6167  arange(-lag, lag
+00018d90: 202b 2031 293a 0a20 2020 2020 2020 2074   + 1):.        t
+00018da0: 6869 734c 6167 203d 206c 6c20 2b20 6c61  hisLag = ll + la
+00018db0: 670a 0a20 2020 2020 2020 2023 206c 6f6f  g..        # loo
+00018dc0: 7020 6f76 6572 2073 616d 706c 6573 0a20  p over samples. 
+00018dd0: 2020 2020 2020 2066 6f72 2069 6920 696e         for ii in
+00018de0: 2072 616e 6765 286e 5361 6d70 6c65 293a   range(nSample):
+00018df0: 0a20 2020 2020 2020 2020 2020 2023 2073  .            # s
+00018e00: 6b69 7020 636f 726e 6572 7320 666f 7220  kip corners for 
+00018e10: 6e6f 772c 2077 6520 7769 6c6c 2063 6f6d  now, we will com
+00018e20: 6520 6261 636b 2074 6f20 7468 6573 650a  e back to these.
+00018e30: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+00018e40: 6969 202b 206c 6c20 3e3d 2030 2920 2620  ii + ll >= 0) & 
+00018e50: 2869 6920 2b20 6c6c 203c 206e 5361 6d70  (ii + ll < nSamp
+00018e60: 6c65 293a 0a20 2020 2020 2020 2020 2020  le):.           
+00018e70: 2020 2020 2065 7272 5b69 692c 2074 6869       err[ii, thi
+00018e80: 734c 6167 5d20 3d20 7531 5b69 695d 202d  sLag] = u1[ii] -
+00018e90: 2075 305b 6969 202b 206c 6c5d 0a0a 2020   u0[ii + ll]..  
+00018ea0: 2020 6966 206e 6f72 6d20 3d3d 2022 4c32    if norm == "L2
+00018eb0: 223a 0a20 2020 2020 2020 2065 7272 203d  ":.        err =
+00018ec0: 2065 7272 2a2a 320a 2020 2020 656c 6966   err**2.    elif
+00018ed0: 206e 6f72 6d20 3d3d 2022 4c31 223a 0a20   norm == "L1":. 
+00018ee0: 2020 2020 2020 2065 7272 203d 206e 702e         err = np.
+00018ef0: 6162 7328 6572 7229 0a0a 2020 2020 2320  abs(err)..    # 
+00018f00: 4e6f 7720 6669 7820 636f 726e 6572 7320  Now fix corners 
+00018f10: 7769 7468 2063 6f6e 7374 616e 7420 6578  with constant ex
+00018f20: 7472 6170 6f6c 6174 696f 6e0a 2020 2020  trapolation.    
+00018f30: 666f 7220 6c6c 2069 6e20 6e70 2e61 7261  for ll in np.ara
+00018f40: 6e67 6528 2d6c 6167 2c20 6c61 6720 2b20  nge(-lag, lag + 
+00018f50: 3129 3a0a 2020 2020 2020 2020 7468 6973  1):.        this
+00018f60: 4c61 6720 3d20 6c6c 202b 206c 6167 0a0a  Lag = ll + lag..
+00018f70: 2020 2020 2020 2020 666f 7220 6969 2069          for ii i
+00018f80: 6e20 7261 6e67 6528 6e53 616d 706c 6529  n range(nSample)
+00018f90: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00018fa0: 2069 6920 2b20 6c6c 203c 2030 3a0a 2020   ii + ll < 0:.  
+00018fb0: 2020 2020 2020 2020 2020 2020 2020 6572                er
+00018fc0: 725b 6969 2c20 7468 6973 4c61 675d 203d  r[ii, thisLag] =
+00018fd0: 2065 7272 5b2d 6c6c 2c20 7468 6973 4c61   err[-ll, thisLa
+00018fe0: 675d 0a0a 2020 2020 2020 2020 2020 2020  g]..            
+00018ff0: 656c 6966 2069 6920 2b20 6c6c 203e 206e  elif ii + ll > n
+00019000: 5361 6d70 6c65 202d 2031 3a0a 2020 2020  Sample - 1:.    
+00019010: 2020 2020 2020 2020 2020 2020 6572 725b              err[
+00019020: 6969 2c20 7468 6973 4c61 675d 203d 2065  ii, thisLag] = e
+00019030: 7272 5b6e 5361 6d70 6c65 202d 206c 6c20  rr[nSample - ll 
+00019040: 2d20 312c 2074 6869 734c 6167 5d0a 0a20  - 1, thisLag].. 
+00019050: 2020 2072 6574 7572 6e20 6572 720a 0a0a     return err...
+00019060: 6465 6620 6163 6375 6d75 6c61 7465 4572  def accumulateEr
+00019070: 726f 7246 756e 6374 696f 6e28 6469 722c  rorFunction(dir,
+00019080: 2065 7272 2c20 6e53 616d 706c 652c 206c   err, nSample, l
+00019090: 6167 2c20 6229 3a0a 2020 2020 2222 220a  ag, b):.    """.
+000190a0: 2020 2020 6163 6375 6d75 6c61 7469 6f6e      accumulation
+000190b0: 206f 6620 7468 6520 6572 726f 722c 2077   of the error, w
+000190c0: 6869 6368 2066 6f6c 6c6f 7773 2074 6865  hich follows the
+000190d0: 2065 7175 6174 696f 6e20 3620 696e 2048   equation 6 in H
+000190e0: 616c 652c 2032 3031 332e 0a0a 2020 2020  ale, 2013...    
+000190f0: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+00019100: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+00019110: 2020 6469 723a 2061 6363 756d 756c 6174    dir: accumulat
+00019120: 696f 6e20 6469 7265 6374 696f 6e20 2820  ion direction ( 
+00019130: 6469 7220 3e20 3020 3d20 666f 7277 6172  dir > 0 = forwar
+00019140: 6420 696e 2074 696d 652c 2064 6972 203c  d in time, dir <
+00019150: 3d20 3020 3d20 6261 636b 7761 7264 2069  = 0 = backward i
+00019160: 6e20 7469 6d65 290a 2020 2020 6572 723a  n time).    err:
+00019170: 2074 6865 2032 4420 6572 726f 7220 6675   the 2D error fu
+00019180: 6e63 7469 6f6e 3b20 7369 7a65 203d 2028  nction; size = (
+00019190: 6e73 616d 702c 322a 6c61 672b 3129 0a20  nsamp,2*lag+1). 
+000191a0: 2020 206e 5361 6d70 6c65 3a20 6e75 6d65     nSample: nume
+000191b0: 7220 6f66 2070 6f69 6e74 7320 746f 2063  r of points to c
+000191c0: 6f6d 7061 7265 2069 6e20 7468 6520 7472  ompare in the tr
+000191d0: 6163 6573 0a20 2020 206c 6167 3a20 6d61  aces.    lag: ma
+000191e0: 7869 6d75 6d20 6c61 6720 696e 2073 616d  ximum lag in sam
+000191f0: 706c 6520 6e75 6d62 6572 2074 6f20 7365  ple number to se
+00019200: 6172 6368 0a20 2020 2062 3a20 7374 7261  arch.    b: stra
+00019210: 696e 206c 696d 6974 2028 696e 7465 6765  in limit (intege
+00019220: 7220 7661 6c75 6520 3e3d 2031 290a 0a20  r value >= 1).. 
+00019230: 2020 2052 4554 5552 4e53 3a0a 2020 2020     RETURNS:.    
+00019240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00019250: 2d2d 0a20 2020 2064 3a20 7468 6520 3244  --.    d: the 2D
+00019260: 2064 6973 7461 6e63 6520 6675 6e63 7469   distance functi
+00019270: 6f6e 3b20 7369 7a65 203d 2028 6e73 616d  on; size = (nsam
+00019280: 702c 322a 6c61 672b 3129 0a0a 2020 2020  p,2*lag+1)..    
+00019290: 4f72 6967 696e 616c 2062 7920 4469 2059  Original by Di Y
+000192a0: 616e 670a 2020 2020 4c61 7374 206d 6f64  ang.    Last mod
+000192b0: 6966 6965 6420 6279 2044 796c 616e 204d  ified by Dylan M
+000192c0: 696b 6573 656c 6c20 2832 3520 4665 622e  ikesell (25 Feb.
+000192d0: 2032 3031 3529 0a20 2020 2054 7261 6e73   2015).    Trans
+000192e0: 6c61 7465 6420 746f 2070 7974 686f 6e20  lated to python 
+000192f0: 6279 2054 696d 2043 6c65 6d65 6e74 7320  by Tim Clements 
+00019300: 2831 3720 4175 672e 2032 3031 3829 0a0a  (17 Aug. 2018)..
+00019310: 2020 2020 2222 220a 0a20 2020 2023 206e      """..    # n
+00019320: 756d 6265 7220 6f66 206c 6167 7320 6672  umber of lags fr
+00019330: 6f6d 205b 202d 6c61 6720 3a20 2b6c 6167  om [ -lag : +lag
+00019340: 205d 0a20 2020 206e 4c61 6720 3d20 2832   ].    nLag = (2
+00019350: 202a 206c 6167 2920 2b20 310a 0a20 2020   * lag) + 1..   
+00019360: 2023 2061 6c6c 6f63 6174 6520 6469 7374   # allocate dist
+00019370: 616e 6365 206d 6174 7269 780a 2020 2020  ance matrix.    
+00019380: 6420 3d20 6e70 2e7a 6572 6f73 285b 6e53  d = np.zeros([nS
+00019390: 616d 706c 652c 206e 4c61 675d 290a 0a20  ample, nLag]).. 
+000193a0: 2020 2023 2053 6574 7570 2069 6e64 6963     # Setup indic
+000193b0: 6573 2062 6173 6564 206f 6e20 666f 7277  es based on forw
+000193c0: 6172 6420 6f72 2062 6163 6b77 6172 6420  ard or backward 
+000193d0: 6163 6375 6d75 6c61 7469 6f6e 2064 6972  accumulation dir
+000193e0: 6563 7469 6f6e 0a20 2020 2069 6620 6469  ection.    if di
+000193f0: 7220 3e20 303a 2020 2320 464f 5257 4152  r > 0:  # FORWAR
+00019400: 440a 2020 2020 2020 2020 6942 6567 696e  D.        iBegin
+00019410: 2c20 6945 6e64 2c20 6949 6e63 203d 2030  , iEnd, iInc = 0
+00019420: 2c20 6e53 616d 706c 6520 2d20 312c 2031  , nSample - 1, 1
+00019430: 0a20 2020 2065 6c73 653a 2020 2320 4241  .    else:  # BA
+00019440: 434b 5741 5244 0a20 2020 2020 2020 2069  CKWARD.        i
+00019450: 4265 6769 6e2c 2069 456e 642c 2069 496e  Begin, iEnd, iIn
+00019460: 6320 3d20 6e53 616d 706c 6520 2d20 312c  c = nSample - 1,
+00019470: 2030 2c20 2d31 0a0a 2020 2020 2320 4c6f   0, -1..    # Lo
+00019480: 6f70 2074 6872 6f75 6768 2061 6c6c 2074  op through all t
+00019490: 696d 6573 2069 6920 696e 2066 6f72 7761  imes ii in forwa
+000194a0: 7264 206f 7220 6261 636b 7761 7264 2064  rd or backward d
+000194b0: 6972 6563 7469 6f6e 0a20 2020 2066 6f72  irection.    for
+000194c0: 2069 6920 696e 2072 616e 6765 2869 4265   ii in range(iBe
+000194d0: 6769 6e2c 2069 456e 6420 2b20 6949 6e63  gin, iEnd + iInc
+000194e0: 2c20 6949 6e63 293a 0a20 2020 2020 2020  , iInc):.       
+000194f0: 2023 206d 696e 2f6d 6178 2074 6f20 6163   # min/max to ac
+00019500: 636f 756e 7420 666f 7220 7468 6520 6564  count for the ed
+00019510: 6765 732f 626f 756e 6461 7269 6573 0a20  ges/boundaries. 
+00019520: 2020 2020 2020 206a 6920 3d20 6d61 7828         ji = max(
+00019530: 5b30 2c20 6d69 6e28 5b6e 5361 6d70 6c65  [0, min([nSample
+00019540: 202d 2031 2c20 6969 202d 2069 496e 635d   - 1, ii - iInc]
+00019550: 295d 290a 2020 2020 2020 2020 6a62 203d  )]).        jb =
+00019560: 206d 6178 285b 302c 206d 696e 285b 6e53   max([0, min([nS
+00019570: 616d 706c 6520 2d20 312c 2069 6920 2d20  ample - 1, ii - 
+00019580: 6949 6e63 202a 2062 5d29 5d29 0a0a 2020  iInc * b])])..  
+00019590: 2020 2020 2020 2320 6c6f 6f70 2074 6872        # loop thr
+000195a0: 6f75 6768 2061 6c6c 206c 6167 0a20 2020  ough all lag.   
+000195b0: 2020 2020 2066 6f72 206c 6c20 696e 2072       for ll in r
+000195c0: 616e 6765 286e 4c61 6729 3a0a 2020 2020  ange(nLag):.    
+000195d0: 2020 2020 2020 2020 2320 6368 6563 6b20          # check 
+000195e0: 6c69 6d69 7473 206f 6e20 6c61 6720 696e  limits on lag in
+000195f0: 6469 6365 730a 2020 2020 2020 2020 2020  dices.          
+00019600: 2020 6c4d 696e 7573 3120 3d20 6c6c 202d    lMinus1 = ll -
+00019610: 2031 0a0a 2020 2020 2020 2020 2020 2020   1..            
+00019620: 2320 6368 6563 6b20 6c61 6720 696e 6465  # check lag inde
+00019630: 7820 6973 2067 7265 6174 6572 2074 6861  x is greater tha
+00019640: 6e20 300a 2020 2020 2020 2020 2020 2020  n 0.            
+00019650: 6966 206c 4d69 6e75 7331 203c 2030 3a0a  if lMinus1 < 0:.
+00019660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019670: 6c4d 696e 7573 3120 3d20 3020 2023 206d  lMinus1 = 0  # m
+00019680: 616b 6520 6c61 6720 3d20 6669 7273 7420  ake lag = first 
+00019690: 6c61 670a 0a20 2020 2020 2020 2020 2020  lag..           
+000196a0: 206c 506c 7573 3120 3d20 6c6c 202b 2031   lPlus1 = ll + 1
+000196b0: 2020 2320 6c61 6720 6174 206c 2b31 0a0a    # lag at l+1..
+000196c0: 2020 2020 2020 2020 2020 2020 2320 6368              # ch
+000196d0: 6563 6b20 6c61 6720 696e 6465 7820 6c65  eck lag index le
+000196e0: 7373 2074 6861 6e20 6d61 7820 6c61 670a  ss than max lag.
+000196f0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00019700: 506c 7573 3120 3e20 6e4c 6167 202d 2031  Plus1 > nLag - 1
+00019710: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00019720: 2020 6c50 6c75 7331 203d 206e 4c61 6720    lPlus1 = nLag 
+00019730: 2d20 310a 0a20 2020 2020 2020 2020 2020  - 1..           
+00019740: 2023 2067 6574 2064 6973 7461 6e63 6520   # get distance 
+00019750: 6174 206c 6167 7320 286c 6c2d 312c 206c  at lags (ll-1, l
+00019760: 6c2c 206c 6c2b 3129 0a20 2020 2020 2020  l, ll+1).       
+00019770: 2020 2020 2064 6973 744c 6d69 6e75 7331       distLminus1
+00019780: 203d 2064 5b6a 622c 206c 4d69 6e75 7331   = d[jb, lMinus1
+00019790: 5d20 2023 206d 696e 7573 3a20 2064 5b69  ]  # minus:  d[i
+000197a0: 2d62 2c20 6a2d 315d 0a20 2020 2020 2020  -b, j-1].       
+000197b0: 2020 2020 2064 6973 744c 203d 2064 5b6a       distL = d[j
+000197c0: 692c 206c 6c5d 2020 2320 6163 7475 616c  i, ll]  # actual
+000197d0: 2064 5b69 2d31 2c20 6a5d 0a20 2020 2020   d[i-1, j].     
+000197e0: 2020 2020 2020 2064 6973 744c 706c 7573         distLplus
+000197f0: 3120 3d20 645b 6a62 2c20 6c50 6c75 7331  1 = d[jb, lPlus1
+00019800: 5d20 2023 2070 6c75 7320 645b 692d 622c  ]  # plus d[i-b,
+00019810: 206a 2b31 5d0a 0a20 2020 2020 2020 2020   j+1]..         
+00019820: 2020 2069 6620 6a69 2021 3d20 6a62 3a20     if ji != jb: 
+00019830: 2023 2065 7175 6174 696f 6e20 3130 2069   # equation 10 i
+00019840: 6e20 4861 6c65 2c20 3230 3133 0a20 2020  n Hale, 2013.   
+00019850: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00019860: 206b 6220 696e 2072 616e 6765 286a 692c   kb in range(ji,
+00019870: 206a 6220 2b20 6949 6e63 202d 2031 2c20   jb + iInc - 1, 
+00019880: 2d69 496e 6329 3a0a 2020 2020 2020 2020  -iInc):.        
+00019890: 2020 2020 2020 2020 2020 2020 6469 7374              dist
+000198a0: 4c6d 696e 7573 3120 3d20 6469 7374 4c6d  Lminus1 = distLm
+000198b0: 696e 7573 3120 2b20 6572 725b 6b62 2c20  inus1 + err[kb, 
+000198c0: 6c4d 696e 7573 315d 0a20 2020 2020 2020  lMinus1].       
+000198d0: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+000198e0: 744c 706c 7573 3120 3d20 6469 7374 4c70  tLplus1 = distLp
+000198f0: 6c75 7331 202b 2065 7272 5b6b 622c 206c  lus1 + err[kb, l
+00019900: 506c 7573 315d 0a0a 2020 2020 2020 2020  Plus1]..        
+00019910: 2020 2020 2320 6571 7561 7469 6f6e 2036      # equation 6
+00019920: 2028 6966 2062 3d31 2920 6f72 2031 3020   (if b=1) or 10 
+00019930: 2869 6620 623e 3129 2069 6e20 4861 6c65  (if b>1) in Hale
+00019940: 2028 3230 3133 2920 6166 7465 7220 7472   (2013) after tr
+00019950: 6561 7469 6e67 2062 6f75 6e64 6172 6965  eating boundarie
+00019960: 730a 2020 2020 2020 2020 2020 2020 645b  s.            d[
+00019970: 6969 2c20 6c6c 5d20 3d20 6572 725b 6969  ii, ll] = err[ii
+00019980: 2c20 6c6c 5d20 2b20 6d69 6e28 5b64 6973  , ll] + min([dis
+00019990: 744c 6d69 6e75 7331 2c20 6469 7374 4c2c  tLminus1, distL,
+000199a0: 2064 6973 744c 706c 7573 315d 290a 0a20   distLplus1]).. 
+000199b0: 2020 2072 6574 7572 6e20 640a 0a0a 6465     return d...de
+000199c0: 6620 6261 636b 7472 6163 6b44 6973 7461  f backtrackDista
+000199d0: 6e63 6546 756e 6374 696f 6e28 6469 722c  nceFunction(dir,
+000199e0: 2064 2c20 6572 722c 206c 6d69 6e2c 2062   d, err, lmin, b
+000199f0: 293a 0a20 2020 2022 2222 0a20 2020 2054  ):.    """.    T
+00019a00: 6865 2066 756e 6374 696f 6e20 6973 2065  he function is e
+00019a10: 7175 6174 696f 6e20 3220 696e 2048 616c  quation 2 in Hal
+00019a20: 652c 2032 3031 332e 0a0a 2020 2020 5061  e, 2013...    Pa
+00019a30: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
+00019a40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+00019a50: 6469 723a 2073 6964 6520 746f 2073 7461  dir: side to sta
+00019a60: 7274 206d 696e 696d 697a 6174 696f 6e20  rt minimization 
+00019a70: 2820 6469 7220 3e20 3020 3d20 6672 6f6e  ( dir > 0 = fron
+00019a80: 742c 2064 6972 203c 3d20 3020 3d20 2062  t, dir <= 0 =  b
+00019a90: 6163 6b29 0a20 2020 2064 203a 2074 6865  ack).    d : the
+00019aa0: 2032 4420 6469 7374 616e 6365 2066 756e   2D distance fun
+00019ab0: 6374 696f 6e3b 2073 697a 6520 3d20 286e  ction; size = (n
+00019ac0: 7361 6d70 2c32 2a6c 6167 2b31 290a 2020  samp,2*lag+1).  
+00019ad0: 2020 6572 723a 2074 6865 2032 4420 6572    err: the 2D er
+00019ae0: 726f 7220 6675 6e63 7469 6f6e 3b20 7369  ror function; si
+00019af0: 7a65 203d 2028 6e73 616d 702c 322a 6c61  ze = (nsamp,2*la
+00019b00: 672b 3129 0a20 2020 206c 6d69 6e3a 206d  g+1).    lmin: m
+00019b10: 696e 696d 756d 206c 6167 2074 6f20 7365  inimum lag to se
+00019b20: 6172 6368 206f 7665 720a 2020 2020 6220  arch over.    b 
+00019b30: 3a20 7374 7261 696e 206c 696d 6974 2028  : strain limit (
+00019b40: 696e 7465 6765 7220 7661 6c75 6520 3e3d  integer value >=
+00019b50: 2031 290a 0a20 2020 2052 4554 5552 4e53   1)..    RETURNS
+00019b60: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  :.    ----------
+00019b70: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2073 7462  --------.    stb
+00019b80: 6172 3a20 7665 6374 6f72 206f 6620 696e  ar: vector of in
+00019b90: 7465 6765 7220 7368 6966 7473 2073 7562  teger shifts sub
+00019ba0: 6a65 6374 2074 6f20 7c75 2869 292d 7528  ject to |u(i)-u(
+00019bb0: 692d 3129 7c20 3c3d 2031 2f62 0a0a 2020  i-1)| <= 1/b..  
+00019bc0: 2020 4f72 6967 696e 616c 2062 7920 4469    Original by Di
+00019bd0: 2059 616e 670a 2020 2020 4c61 7374 206d   Yang.    Last m
+00019be0: 6f64 6966 6965 6420 6279 2044 796c 616e  odified by Dylan
+00019bf0: 204d 696b 6573 656c 6c20 2831 3920 4465   Mikesell (19 De
+00019c00: 632e 2032 3031 3429 0a0a 2020 2020 5472  c. 2014)..    Tr
+00019c10: 616e 736c 6174 6564 2074 6f20 7079 7468  anslated to pyth
+00019c20: 6f6e 2062 7920 5469 6d20 436c 656d 656e  on by Tim Clemen
+00019c30: 7473 2028 3137 2041 7567 2e20 3230 3138  ts (17 Aug. 2018
+00019c40: 290a 0a20 2020 2022 2222 0a0a 2020 2020  )..    """..    
+00019c50: 6e53 616d 706c 652c 206e 4c61 6720 3d20  nSample, nLag = 
+00019c60: 642e 7368 6170 650a 2020 2020 7374 6261  d.shape.    stba
+00019c70: 7220 3d20 6e70 2e7a 6572 6f73 286e 5361  r = np.zeros(nSa
+00019c80: 6d70 6c65 290a 0a20 2020 2023 2053 6574  mple)..    # Set
+00019c90: 7570 2069 6e64 6963 6573 2062 6173 6564  up indices based
+00019ca0: 206f 6e20 666f 7277 6172 6420 6f72 2062   on forward or b
+00019cb0: 6163 6b77 6172 6420 6163 6375 6d75 6c61  ackward accumula
+00019cc0: 7469 6f6e 2064 6972 6563 7469 6f6e 0a20  tion direction. 
+00019cd0: 2020 2069 6620 6469 7220 3e20 303a 2020     if dir > 0:  
+00019ce0: 2320 464f 5257 4152 440a 2020 2020 2020  # FORWARD.      
+00019cf0: 2020 6942 6567 696e 2c20 6945 6e64 2c20    iBegin, iEnd, 
+00019d00: 6949 6e63 203d 2030 2c20 6e53 616d 706c  iInc = 0, nSampl
+00019d10: 6520 2d20 312c 2031 0a20 2020 2065 6c73  e - 1, 1.    els
+00019d20: 653a 2020 2320 4241 434b 5741 5244 0a20  e:  # BACKWARD. 
+00019d30: 2020 2020 2020 2069 4265 6769 6e2c 2069         iBegin, i
+00019d40: 456e 642c 2069 496e 6320 3d20 6e53 616d  End, iInc = nSam
+00019d50: 706c 6520 2d20 312c 2030 2c20 2d31 0a0a  ple - 1, 0, -1..
+00019d60: 2020 2020 2320 7374 6172 7420 6672 6f6d      # start from
+00019d70: 2074 6865 2065 6e64 2028 6672 6f6e 7420   the end (front 
+00019d80: 6f72 2062 6163 6b29 0a20 2020 206c 6c20  or back).    ll 
+00019d90: 3d20 6e70 2e61 7267 6d69 6e28 645b 6942  = np.argmin(d[iB
+00019da0: 6567 696e 2c20 3a5d 2920 2023 2066 696e  egin, :])  # fin
+00019db0: 6420 6d69 6e69 6d75 6d20 6163 6375 6d75  d minimum accumu
+00019dc0: 6c61 7465 6420 6469 7374 616e 6365 2061  lated distance a
+00019dd0: 7420 6672 6f6e 7420 6f72 2062 6163 6b20  t front or back 
+00019de0: 6465 7065 6e64 696e 6720 6f6e 2027 6469  depending on 'di
+00019df0: 7227 0a20 2020 2073 7462 6172 5b69 4265  r'.    stbar[iBe
+00019e00: 6769 6e5d 203d 206c 6c20 2b20 6c6d 696e  gin] = ll + lmin
+00019e10: 2020 2320 6162 736f 6c75 7465 2076 616c    # absolute val
+00019e20: 7565 206f 6620 696e 7465 6765 7220 7368  ue of integer sh
+00019e30: 6966 740a 0a20 2020 2023 206d 6f76 6520  ift..    # move 
+00019e40: 7468 726f 7567 6820 616c 6c20 7469 6d65  through all time
+00019e50: 2073 616d 706c 6573 2069 6e20 666f 7277   samples in forw
+00019e60: 6172 6420 6f72 2062 6163 6b77 6172 6420  ard or backward 
+00019e70: 6469 7265 6374 696f 6e0a 2020 2020 6969  direction.    ii
+00019e80: 203d 2069 4265 6769 6e0a 0a20 2020 2077   = iBegin..    w
+00019e90: 6869 6c65 2069 6920 213d 2069 456e 643a  hile ii != iEnd:
+00019ea0: 0a20 2020 2020 2020 2023 206d 696e 2f6d  .        # min/m
+00019eb0: 6178 2066 6f72 2065 6467 6573 2f62 6f75  ax for edges/bou
+00019ec0: 6e64 6172 6965 730a 2020 2020 2020 2020  ndaries.        
+00019ed0: 6a69 203d 206e 702e 6d61 7828 5b30 2c20  ji = np.max([0, 
+00019ee0: 6e70 2e6d 696e 285b 6e53 616d 706c 6520  np.min([nSample 
+00019ef0: 2d20 312c 2069 6920 2b20 6949 6e63 5d29  - 1, ii + iInc])
+00019f00: 5d29 0a20 2020 2020 2020 206a 6220 3d20  ]).        jb = 
+00019f10: 6e70 2e6d 6178 285b 302c 206e 702e 6d69  np.max([0, np.mi
+00019f20: 6e28 5b6e 5361 6d70 6c65 202d 2031 2c20  n([nSample - 1, 
+00019f30: 6969 202b 2069 496e 6320 2a20 625d 295d  ii + iInc * b])]
+00019f40: 290a 0a20 2020 2020 2020 2023 2063 6865  )..        # che
+00019f50: 636b 206c 696d 6974 7320 6f6e 206c 6167  ck limits on lag
+00019f60: 2069 6e64 6963 6573 0a20 2020 2020 2020   indices.       
+00019f70: 206c 4d69 6e75 7331 203d 206c 6c20 2d20   lMinus1 = ll - 
+00019f80: 310a 0a20 2020 2020 2020 2069 6620 6c4d  1..        if lM
+00019f90: 696e 7573 3120 3c20 303a 2020 2320 6368  inus1 < 0:  # ch
+00019fa0: 6563 6b20 6c61 6720 696e 6465 7820 6973  eck lag index is
+00019fb0: 2067 7265 6174 6572 2074 6861 6e20 310a   greater than 1.
+00019fc0: 2020 2020 2020 2020 2020 2020 6c4d 696e              lMin
+00019fd0: 7573 3120 3d20 3020 2023 206d 616b 6520  us1 = 0  # make 
+00019fe0: 6c61 6720 3d20 6669 7273 7420 6c61 670a  lag = first lag.
+00019ff0: 0a20 2020 2020 2020 206c 506c 7573 3120  .        lPlus1 
+0001a000: 3d20 6c6c 202b 2031 0a0a 2020 2020 2020  = ll + 1..      
+0001a010: 2020 6966 206c 506c 7573 3120 3e20 6e4c    if lPlus1 > nL
+0001a020: 6167 202d 2031 3a20 2023 2063 6865 636b  ag - 1:  # check
+0001a030: 206c 6167 2069 6e64 6578 206c 6573 7320   lag index less 
+0001a040: 7468 616e 206d 6178 206c 6167 0a20 2020  than max lag.   
+0001a050: 2020 2020 2020 2020 206c 506c 7573 3120           lPlus1 
+0001a060: 3d20 6e4c 6167 202d 2031 0a0a 2020 2020  = nLag - 1..    
+0001a070: 2020 2020 2320 6765 7420 6469 7374 616e      # get distan
+0001a080: 6365 2061 7420 6c61 6773 2028 6c6c 2d31  ce at lags (ll-1
+0001a090: 2c20 6c6c 2c20 6c6c 2b31 290a 2020 2020  , ll, ll+1).    
+0001a0a0: 2020 2020 6469 7374 4c6d 696e 7573 3120      distLminus1 
+0001a0b0: 3d20 645b 6a62 2c20 6c4d 696e 7573 315d  = d[jb, lMinus1]
+0001a0c0: 2020 2320 6d69 6e75 733a 2020 645b 692d    # minus:  d[i-
+0001a0d0: 622c 206a 2d31 5d0a 2020 2020 2020 2020  b, j-1].        
+0001a0e0: 6469 7374 4c20 3d20 645b 6a69 2c20 6c6c  distL = d[ji, ll
+0001a0f0: 5d20 2023 2061 6374 7561 6c20 645b 692d  ]  # actual d[i-
+0001a100: 312c 206a 5d0a 2020 2020 2020 2020 6469  1, j].        di
+0001a110: 7374 4c70 6c75 7331 203d 2064 5b6a 622c  stLplus1 = d[jb,
+0001a120: 206c 506c 7573 315d 2020 2320 706c 7573   lPlus1]  # plus
+0001a130: 2064 5b69 2d62 2c20 6a2b 315d 0a0a 2020   d[i-b, j+1]..  
+0001a140: 2020 2020 2020 2320 6571 7561 7469 6f6e        # equation
+0001a150: 2031 3020 696e 2048 616c 6520 2832 3031   10 in Hale (201
+0001a160: 3329 0a20 2020 2020 2020 2023 2073 756d  3).        # sum
+0001a170: 2065 7272 6f72 7320 6f76 6572 2069 2d31   errors over i-1
+0001a180: 3a69 2d62 2b31 0a20 2020 2020 2020 2069  :i-b+1.        i
+0001a190: 6620 6a69 2021 3d20 6a62 3a0a 2020 2020  f ji != jb:.    
+0001a1a0: 2020 2020 2020 2020 666f 7220 6b62 2069          for kb i
+0001a1b0: 6e20 7261 6e67 6528 6a69 2c20 6a62 202d  n range(ji, jb -
+0001a1c0: 2069 496e 6320 2d20 312c 2069 496e 6329   iInc - 1, iInc)
+0001a1d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001a1e0: 2020 6469 7374 4c6d 696e 7573 3120 3d20    distLminus1 = 
+0001a1f0: 6469 7374 4c6d 696e 7573 3120 2b20 6572  distLminus1 + er
+0001a200: 725b 6b62 2c20 6c4d 696e 7573 315d 0a20  r[kb, lMinus1]. 
+0001a210: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0001a220: 6973 744c 706c 7573 3120 3d20 6469 7374  istLplus1 = dist
+0001a230: 4c70 6c75 7331 202b 2065 7272 5b6b 622c  Lplus1 + err[kb,
+0001a240: 206c 506c 7573 315d 0a0a 2020 2020 2020   lPlus1]..      
+0001a250: 2020 2320 7570 6461 7465 206d 696e 696d    # update minim
+0001a260: 756d 2064 6973 7461 6e63 6520 746f 2070  um distance to p
+0001a270: 7265 7669 6f75 7320 7361 6d70 6c65 0a20  revious sample. 
+0001a280: 2020 2020 2020 2064 6c20 3d20 6e70 2e6d         dl = np.m
+0001a290: 696e 285b 6469 7374 4c6d 696e 7573 312c  in([distLminus1,
+0001a2a0: 2064 6973 744c 2c20 6469 7374 4c70 6c75   distL, distLplu
+0001a2b0: 7331 5d29 0a0a 2020 2020 2020 2020 6966  s1])..        if
+0001a2c0: 2064 6c20 213d 2064 6973 744c 3a20 2023   dl != distL:  #
+0001a2d0: 2074 6865 6e20 6c6c 207e 3d20 6c6c 2061   then ll ~= ll a
+0001a2e0: 6e64 2077 6520 6368 6563 6b20 666f 7277  nd we check forw
+0001a2f0: 6172 6420 616e 6420 6261 636b 7761 7264  ard and backward
+0001a300: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001a310: 646c 203d 3d20 6469 7374 4c6d 696e 7573  dl == distLminus
+0001a320: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
+0001a330: 2020 206c 6c20 3d20 6c4d 696e 7573 310a     ll = lMinus1.
+0001a340: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0001a350: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001a360: 2020 6c6c 203d 206c 506c 7573 310a 0a20    ll = lPlus1.. 
+0001a370: 2020 2020 2020 2023 2061 7373 756d 6520         # assume 
+0001a380: 6969 203d 2069 6920 2d20 310a 2020 2020  ii = ii - 1.    
+0001a390: 2020 2020 6969 202b 3d20 6949 6e63 0a0a      ii += iInc..
+0001a3a0: 2020 2020 2020 2020 2320 6162 736f 6c75          # absolu
+0001a3b0: 7465 2069 6e74 6567 6572 206f 6620 6c61  te integer of la
+0001a3c0: 670a 2020 2020 2020 2020 7374 6261 725b  g.        stbar[
+0001a3d0: 6969 5d20 3d20 6c6c 202b 206c 6d69 6e0a  ii] = ll + lmin.
+0001a3e0: 0a20 2020 2020 2020 2023 206e 6f77 206d  .        # now m
+0001a3f0: 6f76 6520 746f 2063 6f72 7265 6374 2074  ove to correct t
+0001a400: 696d 6520 696e 6465 782c 2069 6620 736d  ime index, if sm
+0001a410: 6f6f 7468 696e 6720 6469 6666 6572 656e  oothing differen
+0001a420: 6365 206f 7665 7220 6d61 6e79 0a20 2020  ce over many.   
+0001a430: 2020 2020 2023 2074 696d 6520 7361 6d70       # time samp
+0001a440: 6c65 7320 7573 696e 6720 2762 270a 2020  les using 'b'.  
+0001a450: 2020 2020 2020 6966 2028 6c6c 203d 3d20        if (ll == 
+0001a460: 6c4d 696e 7573 3129 207c 2028 6c6c 203d  lMinus1) | (ll =
+0001a470: 3d20 6c50 6c75 7331 293a 2020 2320 6368  = lPlus1):  # ch
+0001a480: 6563 6b20 6564 6765 7320 746f 2073 6565  eck edges to see
+0001a490: 2061 626f 7574 2062 2076 616c 7565 730a   about b values.
+0001a4a0: 2020 2020 2020 2020 2020 2020 6966 206a              if j
+0001a4b0: 6920 213d 206a 623a 2020 2320 6966 2062  i != jb:  # if b
+0001a4c0: 3e31 2074 6865 6e20 6e65 6564 2074 6f20  >1 then need to 
+0001a4d0: 6d6f 7665 206d 6f72 6520 7374 6570 730a  move more steps.
+0001a4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a4f0: 666f 7220 6b62 2069 6e20 7261 6e67 6528  for kb in range(
+0001a500: 6a69 2c20 6a62 202d 2069 496e 6320 2d20  ji, jb - iInc - 
+0001a510: 312c 2069 496e 6329 3a0a 2020 2020 2020  1, iInc):.      
+0001a520: 2020 2020 2020 2020 2020 2020 2020 6969                ii
+0001a530: 203d 2069 6920 2b20 6949 6e63 2020 2320   = ii + iInc  # 
+0001a540: 6d6f 7665 2066 726f 6d20 692d 313a 692d  move from i-1:i-
+0001a550: 622d 310a 2020 2020 2020 2020 2020 2020  b-1.            
+0001a560: 2020 2020 2020 2020 7374 6261 725b 6969          stbar[ii
+0001a570: 5d20 3d20 6c6c 202b 206c 6d69 6e20 2023  ] = ll + lmin  #
+0001a580: 2063 6f6e 7374 616e 7420 6c61 6720 6f76   constant lag ov
+0001a590: 6572 2074 6861 7420 7469 6d65 0a0a 2020  er that time..  
+0001a5a0: 2020 7265 7475 726e 2073 7462 6172 0a0a    return stbar..
+0001a5b0: 0a64 6566 2077 6374 5f6d 6f64 6966 6965  .def wct_modifie
+0001a5c0: 6428 0a20 2020 2079 312c 2079 322c 2064  d(.    y1, y2, d
+0001a5d0: 742c 2064 6a3d 3120 2f20 3132 2c20 7330  t, dj=1 / 12, s0
+0001a5e0: 3d2d 312c 204a 3d2d 312c 2073 6967 3d54  =-1, J=-1, sig=T
+0001a5f0: 7275 652c 2073 6967 6e69 6669 6361 6e63  rue, significanc
+0001a600: 655f 6c65 7665 6c3d 302e 3935 2c20 7761  e_level=0.95, wa
+0001a610: 7665 6c65 743d 226d 6f72 6c65 7422 2c20  velet="morlet", 
+0001a620: 6e6f 726d 616c 697a 653d 5472 7565 2c20  normalize=True, 
+0001a630: 2a2a 6b77 6172 6773 0a29 3a0a 2020 2020  **kwargs.):.    
+0001a640: 2222 220a 2020 2020 2020 2020 5761 7665  """.        Wave
+0001a650: 6c65 7420 636f 6865 7265 6e63 6520 7472  let coherence tr
+0001a660: 616e 7366 6f72 6d20 2857 4354 292e 0a20  ansform (WCT).. 
+0001a670: 2020 20e2 808b 0a20 2020 2020 2020 2054     ....        T
+0001a680: 6865 2057 4354 2066 696e 6473 2072 6567  he WCT finds reg
+0001a690: 696f 6e73 2069 6e20 7469 6d65 2066 7265  ions in time fre
+0001a6a0: 7175 656e 6379 2073 7061 6365 2077 6865  quency space whe
+0001a6b0: 7265 2074 6865 2074 776f 2074 696d 650a  re the two time.
+0001a6c0: 2020 2020 2020 2020 7365 7269 6573 2063          series c
+0001a6d0: 6f2d 7661 7279 2c20 6275 7420 646f 206e  o-vary, but do n
+0001a6e0: 6f74 206e 6563 6573 7361 7269 6c79 2068  ot necessarily h
+0001a6f0: 6176 6520 6869 6768 2070 6f77 6572 2e0a  ave high power..
+0001a700: 2020 2020 e280 8b0a 2020 2020 2020 2020      ....        
+0001a710: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+0001a720: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+0001a730: 2020 2020 2020 7931 2c20 7932 203a 206e        y1, y2 : n
+0001a740: 756d 7079 2e6e 6461 7272 6179 2c20 6c69  umpy.ndarray, li
+0001a750: 7374 0a20 2020 2020 2020 2020 2020 2049  st.            I
+0001a760: 6e70 7574 2073 6967 6e61 6c73 2e0a 2020  nput signals..  
+0001a770: 2020 2020 2020 6474 203a 2066 6c6f 6174        dt : float
+0001a780: 0a20 2020 2020 2020 2020 2020 2053 616d  .            Sam
+0001a790: 706c 6520 7370 6163 696e 672e 0a20 2020  ple spacing..   
+0001a7a0: 2020 2020 2064 6a20 3a20 666c 6f61 742c       dj : float,
+0001a7b0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+0001a7c0: 2020 2020 2020 5370 6163 696e 6720 6265        Spacing be
+0001a7d0: 7477 6565 6e20 6469 7363 7265 7465 2073  tween discrete s
+0001a7e0: 6361 6c65 732e 2044 6566 6175 6c74 2076  cales. Default v
+0001a7f0: 616c 7565 2069 7320 312f 3132 2e0a 2020  alue is 1/12..  
+0001a800: 2020 2020 2020 2020 2020 536d 616c 6c65            Smalle
+0001a810: 7220 7661 6c75 6573 2077 696c 6c20 7265  r values will re
+0001a820: 7375 6c74 2069 6e20 6265 7474 6572 2073  sult in better s
+0001a830: 6361 6c65 2072 6573 6f6c 7574 696f 6e2c  cale resolution,
+0001a840: 2062 7574 0a20 2020 2020 2020 2020 2020   but.           
+0001a850: 2073 6c6f 7765 7220 6361 6c63 756c 6174   slower calculat
+0001a860: 696f 6e20 616e 6420 706c 6f74 2e0a 2020  ion and plot..  
+0001a870: 2020 2020 2020 7330 203a 2066 6c6f 6174        s0 : float
+0001a880: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+0001a890: 2020 2020 2020 2053 6d61 6c6c 6573 7420         Smallest 
+0001a8a0: 7363 616c 6520 6f66 2074 6865 2077 6176  scale of the wav
+0001a8b0: 656c 6574 2e20 4465 6661 756c 7420 7661  elet. Default va
+0001a8c0: 6c75 6520 6973 2032 2a64 742e 0a20 2020  lue is 2*dt..   
+0001a8d0: 2020 2020 204a 203a 2066 6c6f 6174 2c20       J : float, 
+0001a8e0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+0001a8f0: 2020 2020 204e 756d 6265 7220 6f66 2073       Number of s
+0001a900: 6361 6c65 7320 6c65 7373 206f 6e65 2e20  cales less one. 
+0001a910: 5363 616c 6573 2072 616e 6765 2066 726f  Scales range fro
+0001a920: 6d20 7330 2075 7020 746f 0a20 2020 2020  m s0 up to.     
+0001a930: 2020 2020 2020 2073 3020 2a20 322a 2a28         s0 * 2**(
+0001a940: 4a20 2a20 646a 292c 2077 6869 6368 2067  J * dj), which g
+0001a950: 6976 6573 2061 2074 6f74 616c 206f 6620  ives a total of 
+0001a960: 284a 202b 2031 2920 7363 616c 6573 2e0a  (J + 1) scales..
+0001a970: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
+0001a980: 756c 7420 6973 204a 203d 2028 6c6f 6732  ult is J = (log2
+0001a990: 284e 2a64 742f 736f 2929 2f64 6a2e 0a20  (N*dt/so))/dj.. 
+0001a9a0: 2020 2020 2020 2073 6967 6e69 6669 6361         significa
+0001a9b0: 6e63 655f 6c65 7665 6c20 2866 6c6f 6174  nce_level (float
+0001a9c0: 2c20 6f70 7469 6f6e 616c 2920 3a0a 2020  , optional) :.  
+0001a9d0: 2020 2020 2020 2020 2020 5369 676e 6966            Signif
+0001a9e0: 6963 616e 6365 206c 6576 656c 2074 6f20  icance level to 
+0001a9f0: 7573 652e 2044 6566 6175 6c74 2069 7320  use. Default is 
+0001aa00: 302e 3935 2e0a 2020 2020 2020 2020 6e6f  0.95..        no
+0001aa10: 726d 616c 697a 6520 2862 6f6f 6c65 616e  rmalize (boolean
+0001aa20: 2c20 6f70 7469 6f6e 616c 2920 3a0a 2020  , optional) :.  
+0001aa30: 2020 2020 2020 2020 2020 4966 2073 6574            If set
+0001aa40: 2074 6f20 7472 7565 2c20 6e6f 726d 616c   to true, normal
+0001aa50: 697a 6573 2043 5754 2062 7920 7468 6520  izes CWT by the 
+0001aa60: 7374 616e 6461 7264 2064 6576 6961 7469  standard deviati
+0001aa70: 6f6e 206f 660a 2020 2020 2020 2020 2020  on of.          
+0001aa80: 2020 7468 6520 7369 676e 616c 732e 0a20    the signals.. 
+0001aa90: 2020 20e2 808b 0a20 2020 2020 2020 2052     ....        R
+0001aaa0: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+0001aab0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2054  ------.        T
+0001aac0: 4f44 4f3a 2053 6f6d 6574 6869 6e67 2054  ODO: Something T
+0001aad0: 4241 2061 6e64 2054 4243 0a20 2020 20e2  BA and TBC.    .
+0001aae0: 808b 0a20 2020 2020 2020 2053 6565 2061  ...        See a
+0001aaf0: 6c73 6f0a 2020 2020 2020 2020 2d2d 2d2d  lso.        ----
+0001ab00: 2d2d 2d2d 0a20 2020 2020 2020 2063 7774  ----.        cwt
+0001ab10: 2c20 7877 740a 2020 2020 e280 8b0a 2020  , xwt.    ....  
+0001ab20: 2020 2222 220a 0a20 2020 2077 6176 656c    """..    wavel
+0001ab30: 6574 203d 2070 7963 7774 2e77 6176 656c  et = pycwt.wavel
+0001ab40: 6574 2e5f 6368 6563 6b5f 7061 7261 6d65  et._check_parame
+0001ab50: 7465 725f 7761 7665 6c65 7428 7761 7665  ter_wavelet(wave
+0001ab60: 6c65 7429 0a20 2020 2023 2043 6865 636b  let).    # Check
+0001ab70: 696e 6720 736f 6d65 2069 6e70 7574 2070  ing some input p
+0001ab80: 6172 616d 6574 6572 730a 2020 2020 6966  arameters.    if
+0001ab90: 2073 3020 3d3d 202d 313a 0a20 2020 2020   s0 == -1:.     
+0001aba0: 2020 2023 204e 756d 6265 7220 6f66 2073     # Number of s
+0001abb0: 6361 6c65 730a 2020 2020 2020 2020 7330  cales.        s0
+0001abc0: 203d 2032 202a 2064 7420 2f20 7761 7665   = 2 * dt / wave
+0001abd0: 6c65 742e 666c 616d 6264 6128 290a 2020  let.flambda().  
+0001abe0: 2020 6966 204a 203d 3d20 2d31 3a0a 2020    if J == -1:.  
+0001abf0: 2020 2020 2020 2320 4e75 6d62 6572 206f        # Number o
+0001ac00: 6620 7363 616c 6573 0a20 2020 2020 2020  f scales.       
+0001ac10: 204a 203d 206e 702e 696e 7428 6e70 2e72   J = np.int(np.r
+0001ac20: 6f75 6e64 286e 702e 6c6f 6732 2879 312e  ound(np.log2(y1.
+0001ac30: 7369 7a65 202a 2064 7420 2f20 7330 2920  size * dt / s0) 
+0001ac40: 2f20 646a 2929 0a0a 2020 2020 2320 4d61  / dj))..    # Ma
+0001ac50: 6b65 7320 7375 7265 2069 6e70 7574 2073  kes sure input s
+0001ac60: 6967 6e61 6c73 2061 7265 206e 756d 7079  ignals are numpy
+0001ac70: 2061 7272 6179 732e 0a20 2020 2079 3120   arrays..    y1 
+0001ac80: 3d20 6e70 2e61 7361 7272 6179 2879 3129  = np.asarray(y1)
+0001ac90: 0a20 2020 2079 3220 3d20 6e70 2e61 7361  .    y2 = np.asa
+0001aca0: 7272 6179 2879 3229 0a20 2020 2023 2043  rray(y2).    # C
+0001acb0: 616c 6375 6c61 7465 7320 7468 6520 7374  alculates the st
+0001acc0: 616e 6461 7264 2064 6576 6961 7469 6f6e  andard deviation
+0001acd0: 206f 6620 626f 7468 2069 6e70 7574 2073   of both input s
+0001ace0: 6967 6e61 6c73 2e0a 2020 2020 7374 6431  ignals..    std1
+0001acf0: 203d 2079 312e 7374 6428 290a 2020 2020   = y1.std().    
+0001ad00: 7374 6432 203d 2079 322e 7374 6428 290a  std2 = y2.std().
+0001ad10: 2020 2020 2320 4e6f 726d 616c 697a 6573      # Normalizes
+0001ad20: 2062 6f74 6820 7369 676e 616c 732c 2069   both signals, i
+0001ad30: 6620 6170 7072 6f70 7269 6174 652e 0a20  f appropriate.. 
+0001ad40: 2020 2069 6620 6e6f 726d 616c 697a 653a     if normalize:
+0001ad50: 0a20 2020 2020 2020 2079 315f 6e6f 726d  .        y1_norm
+0001ad60: 616c 203d 2028 7931 202d 2079 312e 6d65  al = (y1 - y1.me
+0001ad70: 616e 2829 2920 2f20 7374 6431 0a20 2020  an()) / std1.   
+0001ad80: 2020 2020 2079 325f 6e6f 726d 616c 203d       y2_normal =
+0001ad90: 2028 7932 202d 2079 322e 6d65 616e 2829   (y2 - y2.mean()
+0001ada0: 2920 2f20 7374 6432 0a20 2020 2065 6c73  ) / std2.    els
+0001adb0: 653a 0a20 2020 2020 2020 2079 315f 6e6f  e:.        y1_no
+0001adc0: 726d 616c 203d 2079 310a 2020 2020 2020  rmal = y1.      
+0001add0: 2020 7932 5f6e 6f72 6d61 6c20 3d20 7932    y2_normal = y2
+0001ade0: 0a0a 2020 2020 2320 4361 6c63 756c 6174  ..    # Calculat
+0001adf0: 6573 2074 6865 2043 5754 206f 6620 7468  es the CWT of th
+0001ae00: 6520 7469 6d65 2d73 6572 6965 7320 6d61  e time-series ma
+0001ae10: 6b69 6e67 2073 7572 6520 7468 6520 7361  king sure the sa
+0001ae20: 6d65 2070 6172 616d 6574 6572 730a 2020  me parameters.  
+0001ae30: 2020 2320 6172 6520 7573 6564 2069 6e20    # are used in 
+0001ae40: 626f 7468 2063 616c 6375 6c61 7469 6f6e  both calculation
+0001ae50: 732e 0a20 2020 205f 6b77 6172 6773 203d  s..    _kwargs =
+0001ae60: 2064 6963 7428 646a 3d64 6a2c 2073 303d   dict(dj=dj, s0=
+0001ae70: 7330 2c20 4a3d 4a2c 2077 6176 656c 6574  s0, J=J, wavelet
+0001ae80: 3d77 6176 656c 6574 290a 2020 2020 5731  =wavelet).    W1
+0001ae90: 2c20 736a 2c20 6672 6571 2c20 636f 692c  , sj, freq, coi,
+0001aea0: 205f 2c20 5f20 3d20 7079 6377 742e 6377   _, _ = pycwt.cw
+0001aeb0: 7428 7931 5f6e 6f72 6d61 6c2c 2064 742c  t(y1_normal, dt,
+0001aec0: 202a 2a5f 6b77 6172 6773 290a 2020 2020   **_kwargs).    
+0001aed0: 5732 2c20 736a 2c20 6672 6571 2c20 636f  W2, sj, freq, co
+0001aee0: 692c 205f 2c20 5f20 3d20 7079 6377 742e  i, _, _ = pycwt.
+0001aef0: 6377 7428 7932 5f6e 6f72 6d61 6c2c 2064  cwt(y2_normal, d
+0001af00: 742c 202a 2a5f 6b77 6172 6773 290a 0a20  t, **_kwargs).. 
+0001af10: 2020 2073 6361 6c65 7331 203d 206e 702e     scales1 = np.
+0001af20: 6f6e 6573 285b 312c 2079 312e 7369 7a65  ones([1, y1.size
+0001af30: 5d29 202a 2073 6a5b 3a2c 204e 6f6e 655d  ]) * sj[:, None]
+0001af40: 0a20 2020 2073 6361 6c65 7332 203d 206e  .    scales2 = n
+0001af50: 702e 6f6e 6573 285b 312c 2079 322e 7369  p.ones([1, y2.si
+0001af60: 7a65 5d29 202a 2073 6a5b 3a2c 204e 6f6e  ze]) * sj[:, Non
+0001af70: 655d 0a0a 2020 2020 2320 536d 6f6f 7468  e]..    # Smooth
+0001af80: 2074 6865 2077 6176 656c 6574 2073 7065   the wavelet spe
+0001af90: 6374 7261 2062 6566 6f72 6520 7472 756e  ctra before trun
+0001afa0: 6361 7469 6e67 2e0a 2020 2020 5331 203d  cating..    S1 =
+0001afb0: 2077 6176 656c 6574 2e73 6d6f 6f74 6828   wavelet.smooth(
+0001afc0: 6e70 2e61 6273 2857 3129 202a 2a20 3220  np.abs(W1) ** 2 
+0001afd0: 2f20 7363 616c 6573 312c 2064 742c 2064  / scales1, dt, d
+0001afe0: 6a2c 2073 6a29 0a20 2020 2053 3220 3d20  j, sj).    S2 = 
+0001aff0: 7761 7665 6c65 742e 736d 6f6f 7468 286e  wavelet.smooth(n
+0001b000: 702e 6162 7328 5732 2920 2a2a 2032 202f  p.abs(W2) ** 2 /
+0001b010: 2073 6361 6c65 7332 2c20 6474 2c20 646a   scales2, dt, dj
+0001b020: 2c20 736a 290a 0a20 2020 2023 204e 6f77  , sj)..    # Now
+0001b030: 2074 6865 2077 6176 656c 6574 2074 7261   the wavelet tra
+0001b040: 6e73 666f 726d 2063 6f68 6572 656e 6365  nsform coherence
+0001b050: 0a20 2020 2057 3132 203d 2057 3120 2a20  .    W12 = W1 * 
+0001b060: 5732 2e63 6f6e 6a28 290a 2020 2020 7363  W2.conj().    sc
+0001b070: 616c 6573 203d 206e 702e 6f6e 6573 285b  ales = np.ones([
+0001b080: 312c 2079 312e 7369 7a65 5d29 202a 2073  1, y1.size]) * s
+0001b090: 6a5b 3a2c 204e 6f6e 655d 0a20 2020 2053  j[:, None].    S
+0001b0a0: 3132 203d 2077 6176 656c 6574 2e73 6d6f  12 = wavelet.smo
+0001b0b0: 6f74 6828 5731 3220 2f20 7363 616c 6573  oth(W12 / scales
+0001b0c0: 2c20 6474 2c20 646a 2c20 736a 290a 2020  , dt, dj, sj).  
+0001b0d0: 2020 5743 5420 3d20 6e70 2e61 6273 2853    WCT = np.abs(S
+0001b0e0: 3132 2920 2a2a 2032 202f 2028 5331 202a  12) ** 2 / (S1 *
+0001b0f0: 2053 3229 0a20 2020 2061 5743 5420 3d20   S2).    aWCT = 
+0001b100: 6e70 2e61 6e67 6c65 2857 3132 290a 0a20  np.angle(W12).. 
+0001b110: 2020 2023 2043 616c 6375 6c61 7465 7320     # Calculates 
+0001b120: 7468 6520 7369 676e 6966 6963 616e 6365  the significance
+0001b130: 2075 7369 6e67 204d 6f6e 7465 2043 6172   using Monte Car
+0001b140: 6c6f 2073 696d 756c 6174 696f 6e73 2077  lo simulations w
+0001b150: 6974 6820 3935 250a 2020 2020 2320 636f  ith 95%.    # co
+0001b160: 6e66 6964 656e 6365 2061 7320 6120 6675  nfidence as a fu
+0001b170: 6e63 7469 6f6e 206f 6620 7363 616c 652e  nction of scale.
+0001b180: 0a0a 2020 2020 6966 2073 6967 3a0a 2020  ..    if sig:.  
+0001b190: 2020 2020 2020 6131 2c20 6231 2c20 6331        a1, b1, c1
+0001b1a0: 203d 2070 7963 7774 2e61 7231 2879 3129   = pycwt.ar1(y1)
+0001b1b0: 0a20 2020 2020 2020 2061 322c 2062 322c  .        a2, b2,
+0001b1c0: 2063 3220 3d20 7079 6377 742e 6172 3128   c2 = pycwt.ar1(
+0001b1d0: 7932 290a 2020 2020 2020 2020 7369 6720  y2).        sig 
+0001b1e0: 3d20 7079 6377 742e 7763 745f 7369 676e  = pycwt.wct_sign
+0001b1f0: 6966 6963 616e 6365 280a 2020 2020 2020  ificance(.      
+0001b200: 2020 2020 2020 6131 2c20 6132 2c20 6474        a1, a2, dt
+0001b210: 3d64 742c 2064 6a3d 646a 2c20 7330 3d73  =dt, dj=dj, s0=s
+0001b220: 302c 204a 3d4a 2c20 7369 676e 6966 6963  0, J=J, signific
+0001b230: 616e 6365 5f6c 6576 656c 3d73 6967 6e69  ance_level=signi
+0001b240: 6669 6361 6e63 655f 6c65 7665 6c2c 2077  ficance_level, w
+0001b250: 6176 656c 6574 3d77 6176 656c 6574 2c20  avelet=wavelet, 
+0001b260: 2a2a 6b77 6172 6773 0a20 2020 2020 2020  **kwargs.       
+0001b270: 2029 0a20 2020 2065 6c73 653a 0a20 2020   ).    else:.   
+0001b280: 2020 2020 2073 6967 203d 206e 702e 6173       sig = np.as
+0001b290: 6172 7261 7928 5b30 5d29 0a0a 2020 2020  array([0])..    
+0001b2a0: 7265 7475 726e 2057 4354 2c20 6157 4354  return WCT, aWCT
+0001b2b0: 2c20 636f 692c 2066 7265 712c 2073 6967  , coi, freq, sig
+0001b2c0: 0a0a 0a23 2323 2323 2323 2323 2323 2323  ...#############
+0001b2d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b2e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b2f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b300: 2323 230a 2323 2323 2323 2323 2323 2323  ###.############
+0001b310: 2323 2323 2044 4953 5045 5253 494f 4e20  #### DISPERSION 
+0001b320: 4558 5452 4143 5449 4f4e 2046 554e 4354  EXTRACTION FUNCT
+0001b330: 494f 4e53 2023 2323 2323 2323 2323 2323  IONS ###########
+0001b340: 2323 2323 0a23 2323 2323 2323 2323 2323  ####.###########
+0001b350: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b380: 2323 2323 230a 0a0a 2320 6675 6e63 7469  #####...# functi
+0001b390: 6f6e 2074 6f20 6578 7472 6163 7420 7468  on to extract th
+0001b3a0: 6520 6469 7370 6572 7369 6f6e 2066 726f  e dispersion fro
+0001b3b0: 6d20 7468 6520 696d 6167 650a 6465 6620  m the image.def 
+0001b3c0: 6578 7472 6163 745f 6469 7370 6572 7369  extract_dispersi
+0001b3d0: 6f6e 2861 6d70 2c20 7065 722c 2076 656c  on(amp, per, vel
+0001b3e0: 293a 0a20 2020 2022 2222 0a20 2020 2074  ):.    """.    t
+0001b3f0: 6869 7320 6675 6e63 7469 6f6e 2074 616b  his function tak
+0001b400: 6573 2074 6865 2064 6973 7065 7273 696f  es the dispersio
+0001b410: 6e20 696d 6167 6520 6672 6f6d 2043 5754  n image from CWT
+0001b420: 2061 7320 696e 7075 742c 2074 7261 636b   as input, track
+0001b430: 7320 7468 6520 676c 6f62 616c 206d 6178  s the global max
+0001b440: 696e 756d 206f 6e0a 2020 2020 7468 6520  inum on.    the 
+0001b450: 7761 7665 6c65 7420 7370 6563 7472 756d  wavelet spectrum
+0001b460: 2061 6d70 6c69 7475 6465 2061 6e64 2065   amplitude and e
+0001b470: 7874 7261 6374 2074 6865 2073 6563 7469  xtract the secti
+0001b480: 6f6e 7320 7769 7468 2063 6f6e 7469 6e6f  ons with contino
+0001b490: 7573 2061 6e64 2068 6967 6820 7175 616c  us and high qual
+0001b4a0: 6974 7920 6461 7461 0a0a 2020 2020 5041  ity data..    PA
+0001b4b0: 5241 4d45 5445 5253 3a0a 2020 2020 2d2d  RAMETERS:.    --
+0001b4c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+0001b4d0: 2020 2061 6d70 3a20 3244 2061 6d70 6c69     amp: 2D ampli
+0001b4e0: 7475 6465 206d 6174 7269 7820 6f66 2074  tude matrix of t
+0001b4f0: 6865 2077 6176 656c 6574 2073 7065 6374  he wavelet spect
+0001b500: 7275 6d0a 2020 2020 7068 6173 653a 2032  rum.    phase: 2
+0001b510: 4420 7068 6173 6520 6d61 7472 6978 206f  D phase matrix o
+0001b520: 6620 7468 6520 7761 7665 6c65 7420 7370  f the wavelet sp
+0001b530: 6563 7472 756d 0a20 2020 2070 6572 3a20  ectrum.    per: 
+0001b540: 2070 6572 696f 6420 7665 6374 6f72 2066   period vector f
+0001b550: 6f72 2074 6865 2032 4420 6d61 7472 6978  or the 2D matrix
+0001b560: 0a20 2020 2076 656c 3a20 2076 656c 2076  .    vel:  vel v
+0001b570: 6563 746f 7220 6f66 2074 6865 2032 4420  ector of the 2D 
+0001b580: 6d61 7472 6978 0a20 2020 2052 4554 5552  matrix.    RETUR
+0001b590: 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  NS:.    --------
+0001b5a0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2070 6572  --------.    per
+0001b5b0: 3a20 2063 656e 7472 616c 2066 7265 7175  :  central frequ
+0001b5c0: 656e 6379 206f 6620 6561 6368 2077 6176  ency of each wav
+0001b5d0: 656c 6574 2073 6361 6c65 2077 6974 6820  elet scale with 
+0001b5e0: 676f 6f64 2064 6174 610a 2020 2020 6776  good data.    gv
+0001b5f0: 3a20 2020 6772 6f75 7020 7665 6c6f 6369  :   group veloci
+0001b600: 7479 2076 6563 746f 7220 6174 2065 6163  ty vector at eac
+0001b610: 6820 6672 6571 7565 6e63 790a 2020 2020  h frequency.    
+0001b620: 2222 220a 2020 2020 6d61 7867 6170 203d  """.    maxgap =
+0001b630: 2035 0a20 2020 206e 7065 7220 3d20 616d   5.    nper = am
+0001b640: 702e 7368 6170 655b 305d 0a20 2020 2067  p.shape[0].    g
+0001b650: 7620 3d20 6e70 2e7a 6572 6f73 286e 7065  v = np.zeros(npe
+0001b660: 722c 2064 7479 7065 3d6e 702e 666c 6f61  r, dtype=np.floa
+0001b670: 7433 3229 0a20 2020 2064 7665 6c20 3d20  t32).    dvel = 
+0001b680: 7665 6c5b 315d 202d 2076 656c 5b30 5d0a  vel[1] - vel[0].
+0001b690: 0a20 2020 2023 2066 696e 6420 676c 6f62  .    # find glob
+0001b6a0: 616c 206d 6178 696d 756d 0a20 2020 2066  al maximum.    f
+0001b6b0: 6f72 2069 6920 696e 2072 616e 6765 286e  or ii in range(n
+0001b6c0: 7065 7229 3a0a 2020 2020 2020 2020 6d61  per):.        ma
+0001b6d0: 7876 616c 7565 203d 206e 702e 6d61 7828  xvalue = np.max(
+0001b6e0: 616d 705b 6969 5d2c 2061 7869 733d 3029  amp[ii], axis=0)
+0001b6f0: 0a20 2020 2020 2020 2069 6e64 7820 3d20  .        indx = 
+0001b700: 6c69 7374 2861 6d70 5b69 695d 292e 696e  list(amp[ii]).in
+0001b710: 6465 7828 6d61 7876 616c 7565 290a 2020  dex(maxvalue).  
+0001b720: 2020 2020 2020 6776 5b69 695d 203d 2076        gv[ii] = v
+0001b730: 656c 5b69 6e64 785d 0a0a 2020 2020 2320  el[indx]..    # 
+0001b740: 6368 6563 6b20 7468 6520 636f 6e74 696e  check the contin
+0001b750: 756f 7573 206f 6620 7468 6520 6469 7370  uous of the disp
+0001b760: 6572 7369 6f6e 0a20 2020 2066 6f72 2069  ersion.    for i
+0001b770: 6920 696e 2072 616e 6765 2831 2c20 6e70  i in range(1, np
+0001b780: 6572 202d 2031 3529 3a0a 2020 2020 2020  er - 15):.      
+0001b790: 2020 2320 3135 2069 7320 7468 6520 6d69    # 15 is the mi
+0001b7a0: 6e75 6d75 6d20 6c65 6e67 7468 206e 6565  numum length nee
+0001b7b0: 6465 6420 666f 7220 6f75 7470 7574 0a20  ded for output. 
+0001b7c0: 2020 2020 2020 2066 6f72 206a 6a20 696e         for jj in
+0001b7d0: 2072 616e 6765 2831 3529 3a0a 2020 2020   range(15):.    
+0001b7e0: 2020 2020 2020 2020 6966 206e 702e 6162          if np.ab
+0001b7f0: 7328 6776 5b69 6920 2b20 6a6a 5d20 2d20  s(gv[ii + jj] - 
+0001b800: 6776 5b69 6920 2b20 3120 2b20 6a6a 5d29  gv[ii + 1 + jj])
+0001b810: 203e 206d 6178 6761 7020 2a20 6476 656c   > maxgap * dvel
+0001b820: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001b830: 2020 6776 5b69 695d 203d 2030 0a20 2020    gv[ii] = 0.   
+0001b840: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+0001b850: 616b 0a0a 2020 2020 2320 7265 6d6f 7665  ak..    # remove
+0001b860: 2074 6865 2062 6164 206f 6e65 730a 2020   the bad ones.  
+0001b870: 2020 696e 6478 203d 206e 702e 7768 6572    indx = np.wher
+0001b880: 6528 6776 203e 2030 295b 305d 0a0a 2020  e(gv > 0)[0]..  
+0001b890: 2020 7265 7475 726e 2070 6572 5b69 6e64    return per[ind
+0001b8a0: 785d 2c20 6776 5b69 6e64 785d 0a         x], gv[indx].
```

### Comparing `noisepy_seis-0.9.6/src/noisepy/seis/plotting_modules.py` & `noisepy_seis-0.9.61/src/noisepy/seis/plotting_modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -668,14 +668,15 @@
         logger.error("No data available for plotting")
         return
 
     # Read some common arguments from the first available data set:
     params, dtmp = store.read(sta_pairs[0][0], sta_pairs[0][1], ccomp, stack_name)
     if len(params) == 0 or dtmp.size == 0:
         logger.error(f"No data available for plotting {stack_name}/{ccomp}")
+        return
 
     dt, maxlag = (params[p] for p in ["dt", "maxlag"])
     stack_method = stack_name.split("0")[-1]
 
     # lags for display
     if not disp_lag:
         disp_lag = maxlag
@@ -690,14 +691,17 @@
     data = np.zeros(shape=(nwin, indx2 - indx1), dtype=np.float32)
     dist = np.zeros(nwin, dtype=np.float32)
     ngood = np.zeros(nwin, dtype=np.int16)
 
     # load cc and parameter matrix
     for ii, (src, rec) in enumerate(sta_pairs):
         params, all_data = store.read(src, rec, ccomp, stack_name)
+        if len(params) == 0 or all_data.size == 0:
+            logger.warning(f"No data available for {src}_{rec}/{stack_name}/{ccomp}")
+            continue
         dist[ii] = params["dist"]
         ngood[ii] = params["ngood"]
 
         data[ii] = bandpass(all_data[indx1:indx2], freqmin, freqmax, int(1 / dt), corners=4, zerophase=True)
 
     # average cc
     ntrace = int(np.round(np.max(dist) + 0.51) / dist_inc)
```

### Comparing `noisepy_seis-0.9.6/src/noisepy/seis/pnwstore.py` & `noisepy_seis-0.9.61/src/noisepy/seis/pnwstore.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     def _load_channels(self, full_path: str, ch_filter: Callable[[Channel], bool]):
         # The path should look like: .../UW/2020/125/
         parts = full_path.split(os.path.sep)
         assert len(parts) >= 4
         net, year, doy = parts[-4:-1]
 
         rst = self._dbquery(
-            f"SELECT network, station, channel, location, filename "
+            f"SELECT DISTINCT network, station, channel, location, filename "
             f"FROM tsindex WHERE filename LIKE '%%/{net}/{year}/{doy}/%%'"
         )
         timespans = []
         for i in rst:
             timespan = PNWDataStore._parse_timespan(os.path.basename(i[4]))
             self.paths[timespan.start_datetime] = full_path
             channel = PNWDataStore._parse_channel(i)
@@ -97,33 +97,41 @@
         doy = str(timespan.start_datetime.timetuple().tm_yday).zfill(3)
 
         rst = self._dbquery(
             f"SELECT byteoffset, bytes "
             f"FROM tsindex WHERE network='{chan.station.network}' AND station='{chan.station.name}' "
             f"AND channel='{chan.type.name}' and location='{chan.station.location}' "
             f"AND filename LIKE '%%/{chan.station.network}/{year}/{doy}/%%'"
+            "ORDER BY byteoffset ASC"
         )
 
         if len(rst) == 0:
             logger.warning(f"Could not find file {timespan}/{chan} in the database")
             return ChannelData.empty()
-        byteoffset, bytes = rst[0]
+        elif len(rst) > 10:
+            # skip if stream has more than 10 gaps
+            logger.warning(f"Too many gaps (>10) from {timespan}/{chan}")
+            return ChannelData.empty()
 
         # reconstruct the file name from the channel parameters
         chan_str = f"{chan.station.name}.{chan.station.network}.{timespan.start_datetime.strftime('%Y.%j')}"
         filename = fs_join(self.paths[timespan.start_datetime].replace("__", chan.station.network), f"{chan_str}")
         if not self.fs.exists(filename):
             logger.warning(f"Could not find file {filename}")
             return ChannelData.empty()
 
+        stream = obspy.Stream()
         with self.fs.open(filename, "rb") as f:
-            f.seek(byteoffset)
-            buff = io.BytesIO(f.read(bytes))
-            stream = obspy.read(buff)
-        return ChannelData(stream)
+            for byteoffset, bytes in rst:
+                f.seek(byteoffset)
+                buff = io.BytesIO(f.read(bytes))
+                stream += obspy.read(buff)
+        # taper each segment
+        stream = stream.taper(max_percentage=0.03)
+        return ChannelData(stream.merge(fill_value=0))
 
     def get_inventory(self, timespan: DateTimeRange, station: Station) -> obspy.Inventory:
         return self.channel_catalog.get_inventory(timespan, station)
 
     def _parse_timespan(filename: str) -> DateTimeRange:
         # The PNWStore repository stores files in the form: STA.NET.YYYY.DOY
         # YA2.UW.2020.366
```

### Comparing `noisepy_seis-0.9.6/src/noisepy/seis/scedc_s3store.py` & `noisepy_seis-0.9.61/src/noisepy/seis/scedc_s3store.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     # for checking the filename has the form: CIGMR__LHN___2022002.ms
     file_re = re.compile(r".*[0-9]{7}\.ms$", re.IGNORECASE)
 
     def __init__(
         self,
         path: str,
         chan_catalog: ChannelCatalog,
-        ch_filter: Callable[[Channel], bool] = None,
+        ch_filter: Callable[[Channel], bool] = lambda s: True,  # noqa: E731
         date_range: DateTimeRange = None,
     ):
         """
         Parameters:
             path: path to look for ms files. Can be a local file directory or an s3://... url path
             chan_catalog: ChannelCatalog to retrieve inventory information for the channels
             channel_filter: Function to decide whether a channel should be used or not,
@@ -57,16 +57,14 @@
         super().__init__()
         self.fs = get_filesystem(path)
         self.channel_catalog = chan_catalog
         self.path = path
         self.paths = {}
         # to store a dict of {timerange: list of channels}
         self.channels = {}
-        if ch_filter is None:
-            ch_filter = lambda s: True  # noqa: E731
 
         if date_range is None:
             self._load_channels(self.path, ch_filter)
         else:
             dt = date_range.end_datetime - date_range.start_datetime
             for d in range(0, dt.days):
                 date = date_range.start_datetime + timedelta(days=d)
```

### Comparing `noisepy_seis-0.9.6/src/noisepy/seis/scheduler.py` & `noisepy_seis-0.9.61/src/noisepy/seis/scheduler.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.6/src/noisepy/seis/stores.py` & `noisepy_seis-0.9.61/src/noisepy/seis/stores.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.6/src/noisepy/seis/utils.py` & `noisepy_seis-0.9.61/src/noisepy/seis/utils.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.6/src/noisepy/seis/zarrstore.py` & `noisepy_seis-0.9.61/src/noisepy/seis/zarrstore.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.6/src/noisepy/seis/application_modules/comp_stacking.py` & `noisepy_seis-0.9.61/src/noisepy/seis/application_modules/comp_stacking.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.6/src/noisepy/seis/application_modules/dispersion_analysis.py` & `noisepy_seis-0.9.61/src/noisepy/seis/application_modules/dispersion_analysis.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.6/src/noisepy/seis/application_modules/measure_dvv.py` & `noisepy_seis-0.9.61/src/noisepy/seis/application_modules/measure_dvv.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.6/src/noisepy/seis/application_modules/write_sac.py` & `noisepy_seis-0.9.61/src/noisepy/seis/application_modules/write_sac.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.6/.gitignore` & `noisepy_seis-0.9.61/.gitignore`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.6/LICENSE` & `noisepy_seis-0.9.61/LICENSE`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.6/README.md` & `noisepy_seis-0.9.61/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [![Documentation Status](https://readthedocs.org/projects/noisepy/badge/?version=latest)](https://noisepy.readthedocs.io/en/latest/?badge=latest)
 [![Build Status](https://travis-ci.com/chengxinjiang/NoisePy.svg?branch=master)](https://travis-ci.com/github/chengxinjiang/NoisePy)
 [![Codecov](https://codecov.io/gh/chengxinjiang/NoisePy/branch/master/graph/badge.svg)](https://codecov.io/gh/chengxinjiang/NoisePy)
 
 <img src="https://raw.githubusercontent.com/mdenolle/NoisePy/master/docs/figures/logo.png" width="800" height="400">
 
 ## Major updates coming
-NoisePy is going through a major refactoring to make this package easier to develop and deploy. Submit an issue, fork the repository and create pull requests to contribute.
+NoisePy is going through a major refactoring to make this package easier to develop and deploy. Submit an issue, fork the repository and create pull requests to [contribute](CONTRIBUTING.md).
 
 # Installation
 The nature of NoisePy being composed of python scripts allows flexible package installation, which is essentially to build dependent libraries the scripts and related functions live upon. We recommend using [conda](https://docs.conda.io/en/latest/) or [pip](https://pypi.org/project/pip/) to install.
 
 ### Note the order of the command lines below matters ###
 
 ## With Conda and pip:
@@ -101,14 +101,21 @@
 * ``smooth_N`` number of points for smoothing the  time or frequency domain discrete arrays.
 * ``maxlag`` maximum length in seconds saved in files in each side of the correlation (save on storage)
 * ``substack,substack_len`` boolean, window length over which to substack the correlation (to save storage or do monitoring), it has to be a multiple of ``cc_len``.
 * ``time_chunk, nchunk`` refers to the time unit that defined a single job. for instace, ``cc_len`` is the correlation length (e.g., 1 hour, 30 min), the overall duration of the experiment is the total length (1 month, 1 year, ...). The time chunk could be 1 day: the code would loop through each cc_len window in a for loop. But each day will be sent as a thread.
 
 
 # Acknowledgements
+
+## Contributing
+
+Thanks to our contributors so far!
+
+[![Contributors](https://contrib.rocks/image?repo=mdenolle/NoisePy)](https://github.com/mdenolle/NoisePy/graphs/contributors)
+
 ## Use this reference when publishing on your work with noisepy
 
 Main code:
 * Jiang, C. and Denolle, M. [NoisePy: a new high-performance python tool for seismic ambient noise seismology.](https://doi.org/10.1785/0220190364) _Seismological Research Letter_ 91, no. 3 (2020): 1853–1866. https://doi.org/10.1785/0220190364
 
 Algorithms used:
 * (data pre-processing) Seats, K. J., Jesse F. L., and German A. P. [Improved ambient noise correlation functions using Welch′ s method.](https://doi.org/10.1111/j.1365-246X.2011.05263.x) _Geophysical Journal International_ 188, no. 2 (2012): 513-523. https://doi.org/10.1111/j.1365-246X.2011.05263.x
```

### Comparing `noisepy_seis-0.9.6/pyproject.toml` & `noisepy_seis-0.9.61/pyproject.toml`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.6/PKG-INFO` & `noisepy_seis-0.9.61/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noisepy-seis
-Version: 0.9.6
+Version: 0.9.61
 Summary: A High-performance Computing Python Package for Ambient Noise Analysis
 Project-URL: Homepage, https://github.com/mdenolle/NoisePy
 Author-email: Marine Denolle <mdenolle@uw.edu>, Chengxin Jiang <chengxin_jiang@fas.harvard.edu>
 License: MIT License
         
         Copyright (c) 2019 Marine Denolle & Chengxin Jiang
         
@@ -67,15 +67,15 @@
 [![Documentation Status](https://readthedocs.org/projects/noisepy/badge/?version=latest)](https://noisepy.readthedocs.io/en/latest/?badge=latest)
 [![Build Status](https://travis-ci.com/chengxinjiang/NoisePy.svg?branch=master)](https://travis-ci.com/github/chengxinjiang/NoisePy)
 [![Codecov](https://codecov.io/gh/chengxinjiang/NoisePy/branch/master/graph/badge.svg)](https://codecov.io/gh/chengxinjiang/NoisePy)
 
 <img src="https://raw.githubusercontent.com/mdenolle/NoisePy/master/docs/figures/logo.png" width="800" height="400">
 
 ## Major updates coming
-NoisePy is going through a major refactoring to make this package easier to develop and deploy. Submit an issue, fork the repository and create pull requests to contribute.
+NoisePy is going through a major refactoring to make this package easier to develop and deploy. Submit an issue, fork the repository and create pull requests to [contribute](CONTRIBUTING.md).
 
 # Installation
 The nature of NoisePy being composed of python scripts allows flexible package installation, which is essentially to build dependent libraries the scripts and related functions live upon. We recommend using [conda](https://docs.conda.io/en/latest/) or [pip](https://pypi.org/project/pip/) to install.
 
 ### Note the order of the command lines below matters ###
 
 ## With Conda and pip:
@@ -160,14 +160,21 @@
 * ``smooth_N`` number of points for smoothing the  time or frequency domain discrete arrays.
 * ``maxlag`` maximum length in seconds saved in files in each side of the correlation (save on storage)
 * ``substack,substack_len`` boolean, window length over which to substack the correlation (to save storage or do monitoring), it has to be a multiple of ``cc_len``.
 * ``time_chunk, nchunk`` refers to the time unit that defined a single job. for instace, ``cc_len`` is the correlation length (e.g., 1 hour, 30 min), the overall duration of the experiment is the total length (1 month, 1 year, ...). The time chunk could be 1 day: the code would loop through each cc_len window in a for loop. But each day will be sent as a thread.
 
 
 # Acknowledgements
+
+## Contributing
+
+Thanks to our contributors so far!
+
+[![Contributors](https://contrib.rocks/image?repo=mdenolle/NoisePy)](https://github.com/mdenolle/NoisePy/graphs/contributors)
+
 ## Use this reference when publishing on your work with noisepy
 
 Main code:
 * Jiang, C. and Denolle, M. [NoisePy: a new high-performance python tool for seismic ambient noise seismology.](https://doi.org/10.1785/0220190364) _Seismological Research Letter_ 91, no. 3 (2020): 1853–1866. https://doi.org/10.1785/0220190364
 
 Algorithms used:
 * (data pre-processing) Seats, K. J., Jesse F. L., and German A. P. [Improved ambient noise correlation functions using Welch′ s method.](https://doi.org/10.1111/j.1365-246X.2011.05263.x) _Geophysical Journal International_ 188, no. 2 (2012): 513-523. https://doi.org/10.1111/j.1365-246X.2011.05263.x
```

