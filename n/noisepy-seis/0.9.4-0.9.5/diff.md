# Comparing `tmp/noisepy_seis-0.9.4.tar.gz` & `tmp/noisepy_seis-0.9.5.tar.gz`

## Comparing `noisepy_seis-0.9.4.tar` & `noisepy_seis-0.9.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11683 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/S0A_download_ASDF_MPI.py
--rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/S0B_to_ASDF.py
--rw-r--r--   0        0        0    12197 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/S1_fft_cc_MPI.py
--rw-r--r--   0        0        0    11706 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/S2_stacking.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/_version.py
--rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/asdfstore.py
--rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/channelcatalog.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/constants.py
--rw-r--r--   0        0        0     9190 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/datatypes.py
--rw-r--r--   0        0        0     7676 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/main.py
--rw-r--r--   0        0        0   113005 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/noise_module.py
--rw-r--r--   0        0        0    35007 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/plotting_modules.py
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/pnwstore.py
--rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/scedc_s3store.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/scheduler.py
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/stores.py
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/utils.py
--rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/zarrstore.py
--rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/application_modules/comp_stacking.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/application_modules/dispersion_analysis.py
--rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/application_modules/measure_dvv.py
--rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/src/noisepy/seis/application_modules/write_sac.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/LICENSE
--rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/README.md
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/pyproject.toml
--rw-r--r--   0        0        0    10601 2020-02-02 00:00:00.000000 noisepy_seis-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0    11683 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/S0A_download_ASDF_MPI.py
+-rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/S0B_to_ASDF.py
+-rw-r--r--   0        0        0    12878 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/S1_fft_cc_MPI.py
+-rw-r--r--   0        0        0    11898 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/S2_stacking.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/_version.py
+-rw-r--r--   0        0        0    10254 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/asdfstore.py
+-rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/channelcatalog.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/constants.py
+-rw-r--r--   0        0        0     9190 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/datatypes.py
+-rw-r--r--   0        0        0     8461 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/main.py
+-rw-r--r--   0        0        0   113005 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/noise_module.py
+-rw-r--r--   0        0        0    34841 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/plotting_modules.py
+-rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/pnwstore.py
+-rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/scedc_s3store.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/scheduler.py
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/stores.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/utils.py
+-rw-r--r--   0        0        0     7463 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/zarrstore.py
+-rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/application_modules/comp_stacking.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/application_modules/dispersion_analysis.py
+-rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/application_modules/measure_dvv.py
+-rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/application_modules/write_sac.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/LICENSE
+-rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/README.md
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0    10729 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/PKG-INFO
```

### Comparing `noisepy_seis-0.9.4/src/noisepy/seis/S0A_download_ASDF_MPI.py` & `noisepy_seis-0.9.5/src/noisepy/seis/S0A_download_ASDF_MPI.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.4/src/noisepy/seis/S0B_to_ASDF.py` & `noisepy_seis-0.9.5/src/noisepy/seis/S0B_to_ASDF.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.4/src/noisepy/seis/S1_fft_cc_MPI.py` & `noisepy_seis-0.9.5/src/noisepy/seis/S1_fft_cc_MPI.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import gc
 import logging
 import sys
+import time
 from collections import OrderedDict
 from concurrent.futures import Executor, Future, ThreadPoolExecutor, as_completed
 from typing import Dict, Iterable, List, Tuple
 
 import numpy as np
 import obspy
 from datetimerange import DateTimeRange
@@ -73,14 +74,15 @@
         return [timespans]
 
     [timespans] = scheduler.initialize(init, 1)
 
     for its in scheduler.get_indices(timespans):
         ts = timespans[its]
         if cc_store.is_done(ts):
+            logger.info(f"{ts} already processed, skipped")
             continue
 
         """
         LOADING NOISE DATA AND DO FFT
         """
         nnfft = int(next_fast_len(int(fft_params.cc_len * fft_params.samp_freq)))  # samp_freq should be sampling_rate
 
@@ -138,19 +140,23 @@
                     if src_chan.station != rec_chan.station:
                         continue
                 if iiR not in ffts:
                     continue
                 t = executor.submit(cross_correlation, fft_params, iiS, iiR, channels, ffts, Nfft)
                 tasks.append(t)
 
+        t_append = 0
         for t in as_completed(tasks):
             # Use as_completed so we can start saving results to the store
             # while other computations are still running
             src_chan, rec_chan, parameters, corr = t.result()
+            t_start = time.time()
             cc_store.append(ts, src_chan, rec_chan, parameters, corr)
+            t_append += time.time() - t_start
+        tlog.log_raw("Append to store", t_append)
 
         ffts.clear()
         gc.collect()
 
         tlog.log(f"Process the chunk of {ts}", t_chunk)
         cc_store.mark_done(ts)
 
@@ -192,16 +198,26 @@
     ch_data: List[Tuple[Channel, ChannelData]],
     raw_store: RawDataStore,
     fft_params: ConfigParameters,
     ts: DateTimeRange,
 ) -> List[Tuple[Channel, ChannelData]]:
     stream_refs = [executor.submit(preprocess, raw_store, t[0], t[1], fft_params, ts) for t in ch_data]
     new_streams = _get_results(stream_refs)
+    # Log if any streams were removed during pre-processing
+    for ch, st in zip(ch_data, new_streams):
+        if len(st) == 0:
+            logging.warning(
+                f"Empty stream for {ts}/{ch[0]} after pre-processing. "
+                f"Before pre-processing data.shape: {ch[1].data.shape}, len(stream): {len(ch[1].stream)}"
+            )
+
+    # Filter to only non-empty streams
     channels = list(zip(*ch_data))[0]
-    return list(zip(channels, [ChannelData(st) for st in new_streams]))
+    non_empty = filter(lambda tup: len(tup[1]) > 0, zip(channels, new_streams))
+    return [(ch, ChannelData(st)) for ch, st in non_empty]
 
 
 def cross_corr(
     fft_params: ConfigParameters,
     src_chan: Channel,
     rec_chan: Channel,
     sfft1: np.ndarray,
```

### Comparing `noisepy_seis-0.9.4/src/noisepy/seis/S2_stacking.py` & `noisepy_seis-0.9.5/src/noisepy/seis/S2_stacking.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import sys
+import time
 from typing import Any, Dict, List, Tuple
 
 import numpy as np
 import pandas as pd
 from datetimerange import DateTimeRange
 
 from noisepy.seis.datatypes import ConfigParameters, StackMethod
@@ -44,15 +45,15 @@
 
 def stack(
     cc_store: CrossCorrelationDataStore,
     stack_store: StackStore,
     fft_params: ConfigParameters,
     scheduler: Scheduler = SingleNodeScheduler(),
 ):
-    tlog = TimeLogger(logger=logger)
+    tlog = TimeLogger(logger=logger, level=logging.INFO)
     t_tot = tlog.reset()
     if fft_params.rotation and fft_params.correction:
         if not fft_params.correction_csv:
             logger.warning("Missing correction_csv parameter but rotation=True and correction=True")
         else:
             locs = pd.read_csv(fft_params.correction_csv)
     else:
@@ -60,15 +61,16 @@
 
     # cross component info
     if fft_params.ncomp == 1:
         enz_system = ["ZZ"]
     else:
         enz_system = ["EE", "EN", "EZ", "NE", "NN", "NZ", "ZE", "ZN", "ZZ"]
 
-    rtz_components = ["ZR", "ZT", "ZZ", "RR", "RT", "RZ", "TR", "TT", "TZ"]
+    # ZZ_R component used to avoid a collision with ZZ component above
+    rtz_components = ["ZR", "ZT", "ZZ_R", "RR", "RT", "RZ", "TR", "TT", "TZ"]
 
     #######################################
     # #########PROCESSING SECTION##########
     #######################################
     def initializer():
         timespans = cc_store.get_timespans()
         pairs_all = cc_store.get_station_pairs()
@@ -83,14 +85,15 @@
     nccomp = fft_params.ncomp * fft_params.ncomp
     num_chunk = len(timespans) * nccomp
     num_segmts = 1
 
     # loop through each pair assigned to this process by the scheduler
     for ipair in scheduler.get_indices(pairs_all):
         tlog.reset()
+        t_append = 0.0
 
         logger.debug("%dth path for station-pair %s" % (ipair, pairs_all[ipair]))
         sta_pair = pairs_all[ipair]
         src_sta = sta_pair[0]
         rec_sta = sta_pair[1]
 
         # check if it is auto-correlation
@@ -157,16 +160,19 @@
         if fft_params.rotation:
             bigstack = np.zeros(shape=(9, npts_segmt), dtype=np.float32)
         if fft_params.stack_method == "all":
             bigstack1 = np.zeros(shape=(9, npts_segmt), dtype=np.float32)
             bigstack2 = np.zeros(shape=(9, npts_segmt), dtype=np.float32)
 
         def write_stacks(comp: str, tparameters: Dict[str, Any], stacks: List[Tuple[StackMethod, np.ndarray]]):
+            nonlocal t_append
+            t_start = time.time()
             for method, data in stacks:
                 stack_store.append(src_sta, rec_sta, comp, f"Allstack_{method.value}", tparameters, data)
+            t_append += time.time() - t_start
 
         # loop through cross-component for stacking
         iflag = 1
         for icomp in range(nccomp):
             tlog.reset()
             comp = enz_system[icomp]
             indx = np.where(cc_comp.lower() == comp.lower())[0]
@@ -212,16 +218,14 @@
             if fft_params.keep_substack:
                 for ii in range(cc_final.shape[0]):
                     tparameters["time"] = stamps_final[ii]
                     tparameters["ngood"] = ngood_final[ii]
                     stack_name = "T" + str(int(stamps_final[ii]))
                     write_stacks(comp, tparameters, [(stack_name, cc_final[ii])])
 
-            tlog.log(f"stack one component with {fft_params.stack_method} stacking method")
-
         # do rotation if needed
         if fft_params.rotation and iflag:
             if np.all(bigstack == 0):
                 continue
             tparameters["station_source"] = src_sta.name
             tparameters["station_receiver"] = rec_sta.name
             if fft_params.stack_method != "all":
@@ -246,14 +250,15 @@
                     stacks = [
                         (StackMethod.LINEAR, bigstack_rotated[icomp]),
                         (StackMethod.PWS, bigstack_rotated1[icomp]),
                         (StackMethod.ROBUST, bigstack_rotated2[icomp]),
                     ]
                     write_stacks(comp, tparameters, stacks)
         tlog.log(f"stack/rotate all station pairs {pairs_all[ipair]}", t_load)
+        tlog.log_raw("store.append", t_append)
 
         stack_store.mark_done(src_sta, rec_sta)
 
     tlog.log("step 2 in total", t_tot)
     scheduler.synchronize()
```

### Comparing `noisepy_seis-0.9.4/src/noisepy/seis/__init__.py` & `noisepy_seis-0.9.5/src/noisepy/seis/__init__.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.4/src/noisepy/seis/asdfstore.py` & `noisepy_seis-0.9.5/src/noisepy/seis/asdfstore.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     def __getitem__(self, key: T) -> pyasdf.ASDFDataSet:
         file_name = self.get_filename(key)
         file_path = os.path.join(self.directory, file_name)
         return _get_dataset(file_path, self.mode)
 
     def get_keys(self) -> List[T]:
-        h5files = sorted(glob.glob(os.path.join(self.directory, "*.h5")))
+        h5files = sorted(glob.glob(os.path.join(self.directory, "**/*.h5"), recursive=True))
         return list(map(self.parse_filename, h5files))
 
     def mark_done(self, key: T):
         self.add_aux_data(key, {}, PROGRESS_DATATYPE, DONE_PATH, np.zeros(0))
 
     def is_done(self, key: T):
         done = self.contains(key, PROGRESS_DATATYPE, DONE_PATH)
@@ -179,37 +179,61 @@
 
     def read(
         self, timespan: DateTimeRange, src_sta: Station, rec_sta: Station, src_ch: ChannelType, rec_ch: ChannelType
     ) -> Tuple[Dict, np.ndarray]:
         dtype = self._get_station_pair(src_sta, rec_sta)
         path = self._get_channel_pair(src_ch, rec_ch)
         with self.datasets[timespan] as ds:
+            if dtype not in ds.auxiliary_data or path not in ds.auxiliary_data[dtype]:
+                return ({}, np.empty((0, 0)))
             stream = ds.auxiliary_data[dtype][path]
             return (stream.parameters, stream.data[:])
 
 
 class ASDFStackStore(StackStore):
     def __init__(self, directory: str, mode: str = "a"):
         super().__init__()
-        self.datasets = ASDFDirectory(directory, mode, _filename_from_stations, parse_station_pair)
+        self.datasets = ASDFDirectory(directory, mode, _filename_from_stations, _parse_station_pair_h5file)
 
     def mark_done(self, src: Station, rec: Station):
         self.datasets.mark_done((src, rec))
 
     def is_done(self, src: Station, rec: Station):
         return self.datasets.is_done((src, rec))
 
     def append(
         self, src: Station, rec: Station, components: str, name: str, stack_params: Dict[str, Any], data: np.ndarray
     ):
         self.datasets.add_aux_data((src, rec), stack_params, name, components, data)
 
+    def get_station_pairs(self) -> List[Tuple[Station, Station]]:
+        return self.datasets.get_keys()
+
+    def get_stack_names(self, src: Station, rec: Station) -> List[str]:
+        with self.datasets[(src, rec)] as ds:
+            return [name for name in ds.auxiliary_data.list() if name != PROGRESS_DATATYPE]
+
+    def get_components(self, src: Station, rec: Station, name: str) -> List[str]:
+        with self.datasets[(src, rec)] as ds:
+            if name not in ds.auxiliary_data:
+                logger.warning(f"Not data available for {src}_{rec}/{name}")
+                return []
+            return ds.auxiliary_data[name].list()
+
+    def read(self, src: Station, rec: Station, component: str, name: str) -> Tuple[Dict[str, Any], np.ndarray]:
+        with self.datasets[(src, rec)] as ds:
+            if name not in ds.auxiliary_data or component not in ds.auxiliary_data[name]:
+                logger.warning(f"Not data available for {src}_{rec}/{name}/{component}")
+                return ({}, np.empty(0))
+            stream = ds.auxiliary_data[name][component]
+            return (stream.parameters, stream.data[:])
+
 
 def _get_dataset(filename: str, mode: str) -> pyasdf.ASDFDataSet:
-    logger.debug(f"ASDFCCStore - Opening {filename}")
+    logger.debug(f"Opening {filename}")
     if os.path.exists(filename):
         return pyasdf.ASDFDataSet(filename, mode=mode, mpi=False, compression=None)
     elif mode == "r":
         return None
     else:  # create new file
         Path(filename).parent.mkdir(exist_ok=True, parents=True)
         return pyasdf.ASDFDataSet(filename, mode=mode, mpi=False, compression=None)
@@ -217,7 +241,12 @@
 
 def _filename_from_stations(pair: Tuple[Station, Station]) -> str:
     return f"{pair[0]}/{pair[0]}_{pair[1]}.h5"
 
 
 def _filename_from_timespan(timespan: DateTimeRange) -> str:
     return f"{timespan_str(timespan)}.h5"
+
+
+def _parse_station_pair_h5file(path: str) -> Tuple[Station, Station]:
+    pair = Path(path).stem
+    return parse_station_pair(pair)
```

### Comparing `noisepy_seis-0.9.4/src/noisepy/seis/channelcatalog.py` & `noisepy_seis-0.9.5/src/noisepy/seis/channelcatalog.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.4/src/noisepy/seis/datatypes.py` & `noisepy_seis-0.9.5/src/noisepy/seis/datatypes.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.4/src/noisepy/seis/main.py` & `noisepy_seis-0.9.5/src/noisepy/seis/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,28 +19,34 @@
 from .datatypes import Channel, ConfigParameters
 from .S0A_download_ASDF_MPI import download
 from .S1_fft_cc_MPI import cross_correlate
 from .S2_stacking import stack
 from .scedc_s3store import SCEDCS3DataStore
 from .scheduler import MPIScheduler, SingleNodeScheduler
 from .utils import fs_join, get_filesystem
+from .zarrstore import ZarrCCStore, ZarrStackStore
 
 logger = logging.getLogger(__name__)
 # Utility running the different steps from the command line. Defines the arguments for each step
 
 default_data_path = "Documents/SCAL"
 
 
 class Command(Enum):
     DOWNLOAD = 1
     CROSS_CORRELATE = 2
     STACK = 3
     ALL = 4
 
 
+class DataFormat(Enum):
+    ZARR = "zarr"
+    ASDF = "asdf"
+
+
 def valid_date(d: str) -> str:
     _ = obspy.UTCDateTime(d)
     return d
 
 
 def list_str(values: str) -> List[str]:
     return values.split(",")
@@ -97,15 +103,15 @@
         config_path = fs_join(data_dir, CONFIG_FILE)
     if config_path is not None and os.path.isfile(config_path):
         logger.info(f"Loading parameters from {config_path}")
         params = ConfigParameters.load_yaml(config_path)
     else:
         logger.warning(f"Config file {config_path if config_path else ''} not found. Using default parameters.")
         params = ConfigParameters()
-    cpy = params.copy(update={k: v for (k, v) in vars(args).items() if k in params.__fields__})
+    cpy = params.model_copy(update={k: v for (k, v) in vars(args).items() if k in params.__fields__})
     return cpy
 
 
 def get_channel_filter(sta_list: List[str]) -> Callable[[Channel], bool]:
     if len(sta_list) == 1 and sta_list[0] == "*":
         return lambda ch: True
     else:
@@ -148,26 +154,40 @@
     logger.setLevel(args.loglevel.upper())
 
     def run_download():
         params = initialize_params(args, None)
         download(args.raw_data_path, params)
         params.save_yaml(fs_join(args.raw_data_path, CONFIG_FILE))
 
+    def get_cc_store(args, mode="a"):
+        return (
+            ZarrCCStore(args.ccf_path, mode=mode)
+            if args.format == DataFormat.ZARR.value
+            else ASDFCCStore(args.ccf_path, mode=mode)
+        )
+
+    def get_stack_store(args):
+        return (
+            ZarrStackStore(args.stack_path, mode="a")
+            if args.format == DataFormat.ZARR.value
+            else ASDFStackStore(args.stack_path, "w")
+        )
+
     def run_cross_correlation():
         ccf_dir = args.ccf_path
-        cc_store = ASDFCCStore(ccf_dir)
+        cc_store = get_cc_store(args)
         params = initialize_params(args, args.raw_data_path)
         raw_store = create_raw_store(args, params)
         scheduler = MPIScheduler(0) if args.mpi else SingleNodeScheduler()
         cross_correlate(raw_store, params, cc_store, scheduler)
         params.save_yaml(fs_join(ccf_dir, CONFIG_FILE))
 
     def run_stack():
-        cc_store = ASDFCCStore(args.ccf_path, "r")
-        stack_store = ASDFStackStore(args.stack_path)
+        cc_store = get_cc_store(args, mode="r")
+        stack_store = get_stack_store(args)
         params = initialize_params(args, args.ccf_path)
         scheduler = MPIScheduler(0) if args.mpi else SingleNodeScheduler()
         stack(cc_store, stack_store, params, scheduler)
         params.save_yaml(fs_join(args.stack_path, CONFIG_FILE))
 
     if args.cmd == Command.DOWNLOAD:
         run_download()
@@ -208,14 +228,22 @@
         default="info",
         choices=["notset", "debug", "info", "warning", "error", "critical"],
     )
     parser.add_argument(
         "-c", "--config", type=lambda f: _valid_config_file(parser, f), required=False, help="Configuration YAML file"
     )
     add_model(parser, ConfigParameters())
+
+    if cmd != Command.DOWNLOAD:
+        parser.add_argument(
+            "--format",
+            default=DataFormat.ZARR.value,
+            choices=[f.value for f in DataFormat],
+            help="Format of the raw data files",
+        )
     return parser
 
 
 def add_mpi(parser: Any):
     parser.add_argument("-m", "--mpi", action="store_true")
```

### Comparing `noisepy_seis-0.9.4/src/noisepy/seis/noise_module.py` & `noisepy_seis-0.9.5/src/noisepy/seis/noise_module.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.4/src/noisepy/seis/plotting_modules.py` & `noisepy_seis-0.9.5/src/noisepy/seis/plotting_modules.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 import os
 
 import matplotlib.pyplot as plt
 import numpy as np
 import obspy
 import pyasdf
 import scipy
+from datetimerange import DateTimeRange
 from obspy.signal.filter import bandpass
 from scipy.fftpack import next_fast_len
 
-from noisepy.seis.constants import PROGRESS_DATATYPE
+from noisepy.seis.stores import CrossCorrelationDataStore, StackStore
 
 logging.getLogger("matplotlib.font_manager").disabled = True
+logger = logging.getLogger(__name__)
 
 """
 Ensembles of plotting functions to display intermediate/final waveforms from the NoisePy package.
 by Chengxin Jiang @Harvard (May.04.2019)
 
 Specifically, this plotting module includes functions of:
     1) plot_waveform     -> display the downloaded waveform for specific station
@@ -115,81 +117,87 @@
 
 
 #############################################################################
 # #############PLOTTING FUNCTIONS FOR FILES FROM S1##########################
 #############################################################################
 
 
-def plot_substack_cc(sfile, freqmin, freqmax, disp_lag=None, savefig=True, sdir="./"):
+def plot_substack_cc(
+    cc_store: CrossCorrelationDataStore,
+    ts: DateTimeRange,
+    freqmin,
+    freqmax,
+    disp_lag=None,
+    savefig=True,
+    sdir="./",
+):
     """
     display the 2D matrix of the cross-correlation functions for a certain time-chunck.
 
     PARAMETERS:
     --------------------------
-    sfile: cross-correlation functions outputed by S1
+    cc_store: Store to read CC data from
+    ts: Timespan to ploe
     freqmin: min frequency to be filtered
     freqmax: max frequency to be filtered
     disp_lag: time ranges for display
-
-    USAGE:
-    --------------------------
-    plot_substack_cc('temp.h5',0.1,1,100,True,'./')
+    savefg: Whether to save the figures as a PDF on disk
+    sdir: Save directory
 
     Note: IMPORTANT!!!! this script only works for cross-correlation with sub-stacks being set to True in S1.
     """
     # open data for read
     if savefig:
         if sdir is None:
-            print("no path selected! save figures in the default path")
+            raise ValueError("sdir argument must be provided if savefig=True")
 
-    try:
-        ds = pyasdf.ASDFDataSet(sfile, mode="r")
-        # extract common variables
-        spairs = ds.auxiliary_data.list()
-        spairs = list(filter(lambda x: x != PROGRESS_DATATYPE, spairs))
-        path_lists = ds.auxiliary_data[spairs[0]].list()
-        flag = ds.auxiliary_data[spairs[0]][path_lists[0]].parameters["substack"]
-        dt = ds.auxiliary_data[spairs[0]][path_lists[0]].parameters["dt"]
-        maxlag = ds.auxiliary_data[spairs[0]][path_lists[0]].parameters["maxlag"]
-    except Exception:
-        raise Exception("exit! cannot open %s to read" % sfile)
+    sta_pairs = cc_store.get_station_pairs()
+    if len(sta_pairs) == 0:
+        logger.error("No data available for plotting")
+        return
+
+    ch_pairs = cc_store.get_channeltype_pairs(ts, sta_pairs[0][0], sta_pairs[0][1])
+    if len(ch_pairs) == 0:
+        logger.error(f"No data available for plotting in {ts}/{sta_pairs[0]}")
+        return
+
+    # Read some common arguments from the first available data set:
+    params, _ = cc_store.read(ts, sta_pairs[0][0], sta_pairs[0][1], ch_pairs[0][0], ch_pairs[0][1])
+    substack_flag, dt, maxlag = (params[p] for p in ["substack", "dt", "maxlag"])
 
     # only works for cross-correlation with substacks generated
-    if not flag:
+    if not substack_flag:
         raise ValueError("seems no substacks have been done! not suitable for this plotting function")
 
     # lags for display
     if not disp_lag:
         disp_lag = maxlag
     if disp_lag > maxlag:
         raise ValueError("lag excceds maxlag!")
 
     # t is the time labels for plotting
     t = np.arange(-int(disp_lag), int(disp_lag) + dt, step=int(2 * int(disp_lag) / 4))
     # windowing the data
     indx1 = int((maxlag - disp_lag) / dt)
     indx2 = indx1 + 2 * int(disp_lag / dt) + 1
 
-    for spair in spairs:
-        ttr = spair.split("_")
-        net1, sta1 = ttr[0].split(".")
-        net2, sta2 = ttr[1].split(".")
-        for ipath in path_lists:
-            chan1, chan2 = ipath.split("_")
+    # for spair in spairs:
+    for src_sta, rec_sta in sta_pairs:
+        ch_pairs = cc_store.get_channeltype_pairs(ts, src_sta, rec_sta)
+        for src_cha, rec_cha in ch_pairs:
             try:
-                dist = ds.auxiliary_data[spair][ipath].parameters["dist"]
-                ngood = ds.auxiliary_data[spair][ipath].parameters["ngood"]
-                ttime = ds.auxiliary_data[spair][ipath].parameters["time"]
-                timestamp = np.empty(ttime.size, dtype="datetime64[s]")
-            except Exception:
-                print("continue! something wrong with %s %s" % (spair, ipath))
+                params, all_data = cc_store.read(ts, src_sta, rec_sta, src_cha, rec_cha)
+                dist, ngood, ttime = (params[p] for p in ["dist", "ngood", "time"])
+                timestamp = np.empty(len(ttime), dtype="datetime64[s]")
+            except Exception as e:
+                logger.warning(f"continue! something wrong with {src_sta}_{rec_sta}/{src_cha}_{rec_cha}: {e}")
                 continue
 
             # cc matrix
-            data = ds.auxiliary_data[spair][ipath].data[:, indx1:indx2]
+            data = all_data[:, indx1:indx2]
             nwin = data.shape[0]
             amax = np.zeros(nwin, dtype=np.float32)
             if nwin == 0 or len(ngood) == 1:
                 print("continue! no enough substacks!")
                 continue
 
             tmarks = []
@@ -212,15 +220,15 @@
             ) = plt.subplots(2, 1, gridspec_kw={"height_ratios": [1, 3]}, figsize=(10, 6))
             ax1.matshow(
                 data,
                 cmap="seismic",
                 extent=[-disp_lag, disp_lag, nwin, 0],
                 aspect="auto",
             )
-            ax1.set_title("%s.%s.%s  %s.%s.%s  dist:%5.2fkm" % (net1, sta1, chan1, net2, sta2, chan2, dist))
+            ax1.set_title(f"{src_sta}.{src_cha} {rec_sta}.{rec_cha}  dist:{dist:5.2f}km")
             ax1.set_xlabel("time [s]")
             ax1.set_xticks(t)
             ax1.set_yticks(np.arange(0, nwin, step=tick_inc))
             ax1.set_yticklabels(timestamp[0::tick_inc])
             ax1.xaxis.set_ticks_position("bottom")
             ax2.set_title("stacked and filtered at %4.2f-%4.2f Hz" % (freqmin, freqmax))
             ax2.plot(
@@ -230,21 +238,17 @@
                 linewidth=1,
             )
             ax2.set_xticks(t)
             fig.tight_layout()
 
             # save figure or just show
             if savefig:
-                if sdir is None:
-                    sdir = sfile.split(".")[0]
                 if not os.path.isdir(sdir):
                     os.mkdir(sdir)
-                outfname = sdir + "/{0:s}.{1:s}.{2:s}_{3:s}.{4:s}.{5:s}.pdf".format(
-                    net1, sta1, chan1, net2, sta2, chan2
-                )
+                outfname = os.path.join(sdir, f"{src_sta}.{src_cha}_{rec_sta}.{rec_cha}.pdf")
                 fig.savefig(outfname, format="pdf", dpi=400)
                 plt.close()
             else:
                 plt.show()
 
 
 def plot_substack_cc_spect(sfile, freqmin, freqmax, disp_lag=None, savefig=True, sdir="./"):
@@ -621,31 +625,31 @@
         fig.savefig(outfname, format="pdf", dpi=400)
         plt.close()
     else:
         plt.show()
 
 
 def plot_all_moveout(
-    sfiles,
-    dtype,
+    store: StackStore,
+    stack_name,
     freqmin,
     freqmax,
     ccomp,
     dist_inc,
     disp_lag=None,
     savefig=False,
     sdir=None,
 ):
     """
     display the moveout (2D matrix) of the cross-correlation functions stacked for all time chuncks.
 
     PARAMETERS:
     ---------------------
-    sfile: cross-correlation functions outputed by S2
-    dtype: datatype either 'Allstack0pws' or 'Allstack0linear'
+    store: StackStore to read stacked data
+    stack_name: datatype either 'Allstack0pws' or 'Allstack0linear'
     freqmin: min frequency to be filtered
     freqmax: max frequency to be filtered
     ccomp:   cross component
     dist_inc: distance bins to stack over
     disp_lag: lag times for displaying
     savefig: set True to save the figures (in pdf format)
     sdir: diresied directory to save the figure (if not provided, save to default dir)
@@ -653,57 +657,51 @@
     USAGE:
     ----------------------
     plot_substack_moveout('temp.h5','Allstack_pws',0.1,0.2,1,'ZZ',200,True,'./temp')
     """
     # open data for read
     if savefig:
         if sdir is None:
-            print("no path selected! save figures in the default path")
+            raise ValueError("sdir argument must be provided if savefig=True")
 
-    path = ccomp
+    sta_pairs = store.get_station_pairs()
+    if len(sta_pairs) == 0:
+        logger.error("No data available for plotting")
+        return
+
+    # Read some common arguments from the first available data set:
+    params, dtmp = store.read(sta_pairs[0][0], sta_pairs[0][1], ccomp, stack_name)
+    if len(params) == 0 or dtmp.size == 0:
+        logger.error(f"No data available for plotting {stack_name}/{ccomp}")
 
-    # extract common variables
-    try:
-        ds = pyasdf.ASDFDataSet(sfiles[0], mode="r")
-        dt = ds.auxiliary_data[dtype][path].parameters["dt"]
-        maxlag = ds.auxiliary_data[dtype][path].parameters["maxlag"]
-        stack_method = dtype.split("0")[-1]
-    except Exception:
-        raise Exception("exit! cannot open %s to read" % sfiles[0])
+    dt, maxlag = (params[p] for p in ["dt", "maxlag"])
+    stack_method = stack_name.split("0")[-1]
 
     # lags for display
     if not disp_lag:
         disp_lag = maxlag
     if disp_lag > maxlag:
         raise ValueError("lag excceds maxlag!")
     t = np.arange(-int(disp_lag), int(disp_lag) + dt, step=(int(2 * int(disp_lag) / 4)))
     indx1 = int((maxlag - disp_lag) / dt)
     indx2 = indx1 + 2 * int(disp_lag / dt) + 1
 
     # cc matrix
-    nwin = len(sfiles)
+    nwin = len(sta_pairs)
     data = np.zeros(shape=(nwin, indx2 - indx1), dtype=np.float32)
     dist = np.zeros(nwin, dtype=np.float32)
     ngood = np.zeros(nwin, dtype=np.int16)
 
     # load cc and parameter matrix
-    for ii in range(len(sfiles)):
-        sfile = sfiles[ii]
-
-        ds = pyasdf.ASDFDataSet(sfile, mode="r")
-        try:
-            # load data to variables
-            dist[ii] = ds.auxiliary_data[dtype][path].parameters["dist"]
-            ngood[ii] = ds.auxiliary_data[dtype][path].parameters["ngood"]
-            tdata = ds.auxiliary_data[dtype][path].data[indx1:indx2]
-        except Exception as e:
-            print(f"continue! cannot read {sfile}: {e}")
-            continue
+    for ii, (src, rec) in enumerate(sta_pairs):
+        params, all_data = store.read(src, rec, ccomp, stack_name)
+        dist[ii] = params["dist"]
+        ngood[ii] = params["ngood"]
 
-        data[ii] = bandpass(tdata, freqmin, freqmax, int(1 / dt), corners=4, zerophase=True)
+        data[ii] = bandpass(all_data[indx1:indx2], freqmin, freqmax, int(1 / dt), corners=4, zerophase=True)
 
     # average cc
     ntrace = int(np.round(np.max(dist) + 0.51) / dist_inc)
     ndata = np.zeros(shape=(ntrace, indx2 - indx1), dtype=np.float32)
     ndist = np.zeros(ntrace, dtype=np.float32)
     for td in range(0, ntrace - 1):
         tindx = np.where((dist >= td * dist_inc) & (dist < (td + 1) * dist_inc))[0]
```

### Comparing `noisepy_seis-0.9.4/src/noisepy/seis/pnwstore.py` & `noisepy_seis-0.9.5/src/noisepy/seis/pnwstore.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         if len(rst) == 0:
             logger.warning(f"Could not find file {timespan}/{chan} in the database")
             return ChannelData.empty()
         byteoffset, bytes = rst[0]
 
         # reconstruct the file name from the channel parameters
         chan_str = f"{chan.station.name}.{chan.station.network}.{timespan.start_datetime.strftime('%Y.%j')}"
-        filename = fs_join(self.paths[timespan.start_datetime], f"{chan_str}")
+        filename = fs_join(self.paths[timespan.start_datetime].replace("__", chan.station.network), f"{chan_str}")
         if not self.fs.exists(filename):
             logger.warning(f"Could not find file {filename}")
             return ChannelData.empty()
 
         with self.fs.open(filename, "rb") as f:
             f.seek(byteoffset)
             buff = io.BytesIO(f.read(bytes))
```

### Comparing `noisepy_seis-0.9.4/src/noisepy/seis/scedc_s3store.py` & `noisepy_seis-0.9.5/src/noisepy/seis/scedc_s3store.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 
 from .datatypes import Channel, ChannelData, ChannelType, Station
 from .utils import fs_join, get_filesystem
 
 logger = logging.getLogger(__name__)
 
 
-def channel_filter(stations: List[str], ch_prefix: str) -> Callable[[Channel], bool]:
+def channel_filter(stations: List[str], ch_prefixes: str) -> Callable[[Channel], bool]:
     """
     Helper function for creating a channel filter to be used in the constructor of the store.
     This filter uses a list of allowed station name along with a channel filter prefix.
     """
     sta_set = set(stations)
 
     def filter(ch: Channel) -> bool:
-        return ch.station.name in sta_set and ch.type.name.lower().startswith(ch_prefix.lower())
+        return ch.station.name in sta_set and ch.type.name.lower().startswith(tuple(ch_prefixes.lower().split(",")))
 
     return filter
 
 
 class SCEDCS3DataStore(RawDataStore):
     """
     A data store implementation to read from a directory of miniSEED (.ms) files from the SCEDC S3 bucket.
```

### Comparing `noisepy_seis-0.9.4/src/noisepy/seis/scheduler.py` & `noisepy_seis-0.9.5/src/noisepy/seis/scheduler.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.4/src/noisepy/seis/stores.py` & `noisepy_seis-0.9.5/src/noisepy/seis/stores.py`

 * *Files 7% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
     def _get_channel_pair(self, src_chan: ChannelType, rec_chan: ChannelType) -> str:
         return f"{src_chan.name}_{rec_chan.name}"
 
 
 class StackStore:
     """
-    A class for writing stack data
+    A class for reading and writing stack data
     """
 
     @abstractmethod
     def mark_done(self, src: Station, rec: Station):
         pass
 
     @abstractmethod
@@ -110,21 +110,37 @@
 
     @abstractmethod
     def append(
         self, src: Station, rec: Station, components: str, name: str, stack_params: Dict[str, Any], data: np.ndarray
     ):
         pass
 
+    @abstractmethod
+    def get_station_pairs(self) -> List[Tuple[Station, Station]]:
+        pass
+
+    @abstractmethod
+    def get_stack_names(self, src: Station, rec: Station) -> List[str]:
+        pass
+
+    @abstractmethod
+    def get_components(self, src: Station, rec: Station, name: str) -> List[str]:
+        pass
+
+    @abstractmethod
+    def read(self, src: Station, rec: Station, component: str, name: str) -> Tuple[Dict[str, Any], np.ndarray]:
+        pass
+
 
 def timespan_str(timespan: DateTimeRange) -> str:
     return f"{timespan.start_datetime.strftime(DATE_FORMAT)}T{timespan.end_datetime.strftime(DATE_FORMAT)}"
 
 
 def parse_station_pair(pair: str) -> Tuple[Station, Station]:
-    # Parse from:'CI.ARV_CI.BAK
+    # Parse from: CI.ARV_CI.BAK
     def station(sta: str) -> Station:
         net, name = sta.split(".")
         return Station(net, name)
 
     return tuple(map(station, pair.split("_")))
```

### Comparing `noisepy_seis-0.9.4/src/noisepy/seis/utils.py` & `noisepy_seis-0.9.5/src/noisepy/seis/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,14 +66,18 @@
         self.time = time.time()
         return self.time
 
     def log(self, message: str = None, start: float = -1.0) -> float:
         stop = time.time()
         dt = stop - self.time if start <= 0 else stop - start
         self.reset()
+        self.log_raw(message, dt)
+        return self.time
+
+    def log_raw(self, message: str, dt: float):
         if self.enabled:
             self.logger.log(self.level, f"TIMING: {dt:6.4f} for {message}")
         return self.time
 
 
 def error_if(condition: bool, msg: str, error_type: type = RuntimeError):
     """
```

### Comparing `noisepy_seis-0.9.4/src/noisepy/seis/application_modules/comp_stacking.py` & `noisepy_seis-0.9.5/src/noisepy/seis/application_modules/comp_stacking.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.4/src/noisepy/seis/application_modules/dispersion_analysis.py` & `noisepy_seis-0.9.5/src/noisepy/seis/application_modules/dispersion_analysis.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.4/src/noisepy/seis/application_modules/measure_dvv.py` & `noisepy_seis-0.9.5/src/noisepy/seis/application_modules/measure_dvv.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.4/src/noisepy/seis/application_modules/write_sac.py` & `noisepy_seis-0.9.5/src/noisepy/seis/application_modules/write_sac.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.4/.gitignore` & `noisepy_seis-0.9.5/.gitignore`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.4/LICENSE` & `noisepy_seis-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.4/README.md` & `noisepy_seis-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.4/PKG-INFO` & `noisepy_seis-0.9.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noisepy-seis
-Version: 0.9.4
+Version: 0.9.5
 Summary: A High-performance Computing Python Package for Ambient Noise Analysis
 Project-URL: Homepage, https://github.com/mdenolle/NoisePy
 Author-email: Marine Denolle <mdenolle@uw.edu>, Chengxin Jiang <chengxin_jiang@fas.harvard.edu>
 License: MIT License
         
         Copyright (c) 2019 Marine Denolle & Chengxin Jiang
         
@@ -29,34 +29,34 @@
 Keywords: ambient,change,cross-correlation,dispersion,monitoring,noise,seismic,surface,velocity,wave
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: <3.11,>=3.8
-Requires-Dist: datetimerange==2.0.0
-Requires-Dist: diskcache>=5.5
-Requires-Dist: fsspec>=2023.4.0
-Requires-Dist: h5py>=3.8.0
-Requires-Dist: numba>=0.57.0
-Requires-Dist: numpy>=1.22.0
-Requires-Dist: pandas>=1.5.3
-Requires-Dist: pyasdf>=0.7.5
-Requires-Dist: pycwt>=0.3.0a22
-Requires-Dist: pydantic-yaml>=1.0
-Requires-Dist: pydantic>=2.0.0
-Requires-Dist: pyyaml>=6.0
-Requires-Dist: s3fs>=2023.4.0
-Requires-Dist: zarr>=2.14.2
+Requires-Dist: datetimerange<3.0.0,==2.0.0
+Requires-Dist: diskcache<6.0,>=5.5
+Requires-Dist: fsspec<2024.0.0,>=2023.4.0
+Requires-Dist: h5py<4.0.0,>=3.8.0
+Requires-Dist: numba<1.0.0,>=0.57.0
+Requires-Dist: numpy<2.0.0,>=1.22.0
+Requires-Dist: pandas<2.0.0,>=1.5.3
+Requires-Dist: pyasdf<1.0.0,>=0.7.5
+Requires-Dist: pycwt<1.0.0,>=0.3.0a22
+Requires-Dist: pydantic-yaml<2.0,>=1.0
+Requires-Dist: pydantic<3.0.0,>=2.0.0
+Requires-Dist: pyyaml<7.0,>=6.0
+Requires-Dist: s3fs<2024.0.0,>=2023.4.0
+Requires-Dist: zarr<3.0.0,>=2.14.2
 Provides-Extra: dev
-Requires-Dist: memory-profiler>=0.61; extra == 'dev'
-Requires-Dist: pre-commit>=3.2; extra == 'dev'
-Requires-Dist: pytest>=7.2.2; extra == 'dev'
+Requires-Dist: memory-profiler<1.0.0,>=0.61; extra == 'dev'
+Requires-Dist: pre-commit<4.0.0,>=3.3.3; extra == 'dev'
+Requires-Dist: pytest<8.0.0,>=7.2.2; extra == 'dev'
 Provides-Extra: mpi
-Requires-Dist: mpi4py>=3.1.4; extra == 'mpi'
+Requires-Dist: mpi4py<4.0.0,>=3.1.4; extra == 'mpi'
 Provides-Extra: sql
 Requires-Dist: sqlite3-0611; extra == 'sql'
 Description-Content-Type: text/markdown
 
 # About NoisePy
 NoisePy is a Python package designed for fast and easy computation of ambient noise cross-correlation functions. It provides additional functionality for noise monitoring and surface wave dispersion analysis.
```

