# Comparing `tmp/mfhpo_simulator-1.2.4-py3-none-any.whl.zip` & `tmp/mfhpo_simulator-1.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 29158 bytes, number of entries: 15
--rw-rw-r--  2.0 unx      560 b- defN 23-Jul-07 16:03 benchmark_simulator/__init__.py
--rw-rw-r--  2.0 unx     7711 b- defN 23-Jul-07 13:22 benchmark_simulator/_constants.py
--rw-rw-r--  2.0 unx    12110 b- defN 23-Jul-07 15:56 benchmark_simulator/_secure_proc.py
+Zip file size: 30249 bytes, number of entries: 15
+-rw-rw-r--  2.0 unx      560 b- defN 23-Jul-25 08:25 benchmark_simulator/__init__.py
+-rw-rw-r--  2.0 unx     7761 b- defN 23-Jul-19 11:36 benchmark_simulator/_constants.py
+-rw-rw-r--  2.0 unx    12622 b- defN 23-Jul-19 07:25 benchmark_simulator/_secure_proc.py
 -rw-rw-r--  2.0 unx     5116 b- defN 23-Jul-06 23:36 benchmark_simulator/_utils.py
--rw-rw-r--  2.0 unx    27095 b- defN 23-Jul-07 15:59 benchmark_simulator/simulator.py
+-rw-rw-r--  2.0 unx    28910 b- defN 23-Jul-19 11:36 benchmark_simulator/simulator.py
 -rw-rw-r--  2.0 unx     2582 b- defN 23-Jul-06 18:41 benchmark_simulator/_simulator/_base_wrapper.py
--rw-rw-r--  2.0 unx     2978 b- defN 23-Jul-04 16:11 benchmark_simulator/_simulator/_utils.py
--rw-rw-r--  2.0 unx    12902 b- defN 23-Jul-07 16:01 benchmark_simulator/_simulator/_worker.py
--rw-rw-r--  2.0 unx     3249 b- defN 23-Jul-07 13:10 benchmark_simulator/_simulator/_worker_manager.py
--rw-rw-r--  2.0 unx     8290 b- defN 23-Jul-04 16:13 benchmark_simulator/_simulator/_worker_manager_for_ask_and_tell.py
--rw-rw-r--  2.0 unx    10760 b- defN 23-Jul-07 16:19 mfhpo_simulator-1.2.4.dist-info/LICENSE
--rw-rw-r--  2.0 unx      307 b- defN 23-Jul-07 16:19 mfhpo_simulator-1.2.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-07 16:19 mfhpo_simulator-1.2.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       51 b- defN 23-Jul-07 16:19 mfhpo_simulator-1.2.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1401 b- defN 23-Jul-07 16:19 mfhpo_simulator-1.2.4.dist-info/RECORD
-15 files, 95204 bytes uncompressed, 26792 bytes compressed:  71.9%
+-rw-rw-r--  2.0 unx     3335 b- defN 23-Jul-19 11:36 benchmark_simulator/_simulator/_utils.py
+-rw-rw-r--  2.0 unx    13196 b- defN 23-Jul-19 11:36 benchmark_simulator/_simulator/_worker.py
+-rw-rw-r--  2.0 unx     3767 b- defN 23-Jul-18 21:06 benchmark_simulator/_simulator/_worker_manager.py
+-rw-rw-r--  2.0 unx     9134 b- defN 23-Jul-18 21:22 benchmark_simulator/_simulator/_worker_manager_for_ask_and_tell.py
+-rw-rw-r--  2.0 unx    10760 b- defN 23-Jul-25 08:25 mfhpo_simulator-1.2.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      307 b- defN 23-Jul-25 08:25 mfhpo_simulator-1.2.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 08:25 mfhpo_simulator-1.2.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       51 b- defN 23-Jul-25 08:25 mfhpo_simulator-1.2.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1401 b- defN 23-Jul-25 08:25 mfhpo_simulator-1.2.5.dist-info/RECORD
+15 files, 99594 bytes uncompressed, 27883 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: benchmark_simulator/_simulator/_worker_manager.py
 Comment: 
 
 Filename: benchmark_simulator/_simulator/_worker_manager_for_ask_and_tell.py
 Comment: 
 
-Filename: mfhpo_simulator-1.2.4.dist-info/LICENSE
+Filename: mfhpo_simulator-1.2.5.dist-info/LICENSE
 Comment: 
 
-Filename: mfhpo_simulator-1.2.4.dist-info/METADATA
+Filename: mfhpo_simulator-1.2.5.dist-info/METADATA
 Comment: 
 
-Filename: mfhpo_simulator-1.2.4.dist-info/WHEEL
+Filename: mfhpo_simulator-1.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: mfhpo_simulator-1.2.4.dist-info/top_level.txt
+Filename: mfhpo_simulator-1.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: mfhpo_simulator-1.2.4.dist-info/RECORD
+Filename: mfhpo_simulator-1.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## benchmark_simulator/__init__.py

```diff
@@ -1,12 +1,12 @@
 from benchmark_simulator._constants import AbstractAskTellOptimizer, ObjectiveFuncType
 from benchmark_simulator.simulator import ObjectiveFuncWrapper, get_multiple_wrappers
 
 
-__version__ = "1.2.4"
+__version__ = "1.2.5"
 __copyright__ = "Copyright (C) 2023 Shuhei Watanabe"
 __licence__ = "Apache-2.0 License"
 __author__ = "Shuhei Watanabe"
 __author_email__ = "shuhei.watanabe.utokyo@gmail.com"
 __url__ = "https://github.com/nabenabe0928/mfhpo-simulator"
```

## benchmark_simulator/_constants.py

```diff
@@ -10,15 +10,15 @@
 
 
 DIR_NAME: Final[str] = "mfhpo-simulator-info/"
 INF: Final[float] = float(1 << 30)
 
 
 @dataclass(frozen=True)
-class _TimeNowDictType:
+class _SampledTimeDictType:
     before_sample: float
     after_sample: float
 
 
 @dataclass(frozen=True)
 class _StateType:
     runtime: float = 0.0
@@ -30,15 +30,15 @@
 @dataclass(frozen=True)
 class _InfoPaths:
     proc_alloc: str
     result: str
     state_cache: str
     worker_cumtime: str
     timestamp: str
-    timenow: str
+    sampled_time: str
     config_tracker: str
 
     def __len__(self) -> int:
         return len(self.__dict__)
 
 
 @dataclass(frozen=True)
@@ -54,15 +54,15 @@
 
 class _SharedDataFileNames(Enum):
     proc_alloc: str = "proc_alloc.json"
     result: str = "results.json"
     state_cache: str = "state_cache.json"
     worker_cumtime: str = "simulated_cumtime.json"
     timestamp: str = "timestamp.json"
-    timenow: str = "timenow.json"
+    sampled_time: str = "sampled_time.json"
     config_tracker: str = "config_tracker.json"
 
 
 @dataclass(frozen=True)
 class _TimeValue:
     terminated: float = float(1 << 40)
     crashed: float = float(1 << 41)
@@ -71,14 +71,15 @@
 @dataclass(frozen=True)
 class _WrapperVars:
     save_dir_name: str
     n_workers: int
     obj_func: ObjectiveFuncType
     n_actual_evals_in_opt: int
     n_evals: int
+    max_total_eval_time: float
     obj_keys: list[str]
     runtime_key: str
     fidel_keys: list[str] | None
     seed: int | None
     continual_max_fidel: int | None
     max_waiting_time: float
     check_interval_time: float
```

## benchmark_simulator/_secure_proc.py

```diff
@@ -3,18 +3,18 @@
 import fcntl
 import os
 import time
 import warnings
 from typing import Any
 
 from benchmark_simulator._constants import (
+    _SampledTimeDictType,
     _SharedDataFileNames,
     _StateType,
     _TIME_VALUES,
-    _TimeNowDictType,
 )
 from benchmark_simulator._utils import _SecureLock
 
 import numpy as np
 
 import ujson as json  # type: ignore
 
@@ -35,37 +35,41 @@
                 f.seek(0)
                 f.truncate()
                 f.write("{}")
 
             fcntl.flock(f.fileno(), fcntl.LOCK_UN)
 
 
-def _allocate_proc_to_worker(path: str, pid: int, lock: _SecureLock) -> None:
+def _allocate_proc_to_worker(path: str, pid: int, time_ns: int, lock: _SecureLock) -> int:
     with lock.edit(path) as f:
-        cur_alloc = json.load(f)
-        cur_alloc[pid] = 0
-        f.seek(0)
-        json.dump(cur_alloc, f, indent=4)
+        pid_str = str(pid)
+        alloc = json.load(f)
+        if pid_str not in alloc:
+            alloc[pid_str] = time_ns
+            alloc = {k: idx for idx, (k, _) in enumerate(sorted(alloc.items(), key=lambda x: x[1]))}
+            f.seek(0)
+            json.dump(alloc, f, indent=4)
+
+    return alloc[pid_str]
 
 
 def _complete_proc_allocation(path: str, lock: _SecureLock) -> dict[int, int]:
     with lock.edit(path) as f:
         alloc = json.load(f)
-        sorted_pids = np.sort([int(pid) for pid in alloc.keys()])
-        alloc = {pid: idx for idx, pid in enumerate(sorted_pids)}
+        alloc = {int(k): idx for idx, (k, _) in enumerate(sorted(alloc.items(), key=lambda x: x[1]))}
         f.seek(0)
         json.dump(alloc, f, indent=4)
 
     return alloc
 
 
-def _record_timenow(path: str, timenow_data: _TimeNowDictType, lock: _SecureLock) -> None:
+def _record_sampled_time(path: str, sampled_time: _SampledTimeDictType, lock: _SecureLock) -> None:
     with lock.edit(path) as f:
         record = json.load(f)
-        for k, v in timenow_data.__dict__.items():
+        for k, v in sampled_time.__dict__.items():
             if k not in record:
                 record[k] = [v]
             else:
                 record[k].append(v)
 
         f.seek(0)
         json.dump(record, f, indent=4)
@@ -129,19 +133,23 @@
 def _fetch_cache_states(path: str, config_hash: int, lock: _SecureLock) -> list[_StateType]:
     with lock.read(path) as f:
         states = json.load(f).get(str(config_hash), [])
 
     return [_StateType(runtime=state[0], cumtime=state[1], fidel=state[2], seed=state[3]) for state in states]
 
 
-def _fetch_timenow(path: str, lock: _SecureLock) -> dict[str, np.ndarray]:
+def _fetch_sampled_time(path: str, lock: _SecureLock) -> dict[str, np.ndarray]:
     with lock.read(path) as f:
         data = {k: np.asarray(v) for k, v in json.load(f).items()}
 
-    return data
+    if len(data) == 0:
+        # It ensures nothing will change in the main proc.
+        return dict(before_sample=np.array([-np.inf]), after_sample=np.array([-np.inf]))
+    else:
+        return data
 
 
 def _fetch_cumtimes(path: str, lock: _SecureLock) -> dict[str, float]:
     with lock.read(path) as f:
         cumtimes = json.load(f)
 
     return cumtimes
@@ -179,19 +187,21 @@
             else:
                 record[key].append(val)
 
         f.seek(0)
         json.dump(record, f, indent=4)
 
 
-def _is_simulator_terminated(path: str, max_evals: int, lock: _SecureLock) -> bool:
+def _is_simulator_terminated(path: str, max_evals: int, max_total_eval_time: float, lock: _SecureLock) -> bool:
     with lock.read(path) as f:
-        result = len(json.load(f)["cumtime"]) >= max_evals
+        cumtimes = json.load(f)["cumtime"]
 
-    return result
+    cond1 = len(cumtimes) >= max_evals
+    cond2 = cumtimes[-1] > max_total_eval_time
+    return cond1 or cond2
 
 
 def _is_simulator_ready(path: str, n_workers: int, lock: _SecureLock) -> bool:
     with lock.read(path) as f:
         result = len(json.load(f)) == n_workers
 
     return result
@@ -250,28 +260,28 @@
         "(2) n_workers specified in your optimizer and that in the simulator might be different.",
         "(3) launch_multiple_wrappers_from_user_side is incorrectly set.",
     ]
     return "\n".join(msg)
 
 
 def _wait_proc_allocation(
-    path: str, n_workers: int, lock: _SecureLock, waiting_time: float = 1e-2, time_limit: float = 10.0
+    path: str, n_workers: int, lock: _SecureLock, waiting_time: float = 1e-4, time_limit: float = 10.0
 ) -> dict[int, int]:
     start = time.time()
     waiting_time *= 1 + np.random.random()
     while not _is_allocation_ready(path, n_workers=n_workers, lock=lock):
         time.sleep(waiting_time)
         if time.time() - start >= time_limit:
             raise TimeoutError(_get_timeout_message(cause="the allocation of procs", path=path))
 
     return _complete_proc_allocation(path, lock=lock)
 
 
 def _wait_all_workers(
-    path: str, n_workers: int, lock: _SecureLock, waiting_time: float = 1e-2, time_limit: float = 10.0
+    path: str, n_workers: int, lock: _SecureLock, waiting_time: float = 1e-4, time_limit: float = 10.0
 ) -> dict[str, int]:
     start = time.time()
     waiting_time *= 1 + np.random.random()
     while not _is_simulator_ready(path, n_workers=n_workers, lock=lock):
         time.sleep(waiting_time)
         if time.time() - start >= time_limit:
             raise TimeoutError(_get_timeout_message(cause="creating a simulator", path=path))
@@ -316,17 +326,18 @@
 ) -> None:
     start = time.time()
     waiting_time *= 1 + np.random.random()
     while not _is_min_cumtime(path, worker_id=worker_id, lock=lock):
         time.sleep(waiting_time)
         curtime = time.time()
         if int(curtime - start + 1) % warning_interval == 0:
-            warnings.warn(
+            msg = (
                 "Workers might be hanging. Please consider setting `max_waiting_time` (< np.inf).\n"
-                "Note that if samplers or the objective function need long time (> 10 seconds), or \n"
+                "Note that if samplers or the objective function need long time (> 10 seconds), or "
                 "n_workers is large, please ignore this warning."
             )
+            warnings.warn(msg)
 
         if curtime - start > max_waiting_time:
             _terminate_with_unexpected_timeout(
                 path=path, worker_id=worker_id, max_waiting_time=max_waiting_time, lock=lock
             )
```

## benchmark_simulator/simulator.py

```diff
@@ -61,22 +61,23 @@
 5. mfhpo-simulator-info/*/timestamp.json
     * worker1_id -- prev_timestamp1
     * worker2_id -- prev_timestamp2
     :
     * workerN_id -- prev_timestampN
 This file tells the last checkpoint timestamp of each worker (prev_timestamp).
 
-6. mfhpo-simulator-info/*/timenow.json
+6. mfhpo-simulator-info/*/sampled_time.json
     * before_sample -- [time1 before sample, time2 before sample, ...]
     * after_sample -- [time1 after sample, time2 after sample, ...]
 This file is used to consider the sampling time.
 after_sample is the latest cumtime immediately after the last sample and before_sample is before the last sample.
 """
 from __future__ import annotations
 
+import json
 import os
 from datetime import datetime
 from typing import Any
 
 from benchmark_simulator._constants import AbstractAskTellOptimizer, DIR_NAME, ObjectiveFuncType, _WrapperVars
 from benchmark_simulator._simulator._worker import _ObjectiveFuncWorker
 from benchmark_simulator._simulator._worker_manager import _CentralWorkerManager
@@ -97,14 +98,15 @@
     seed: int | None = None,
     continual_max_fidel: int | None = None,
     max_waiting_time: float = np.inf,
     check_interval_time: float = 1e-4,
     store_config: bool = False,
     allow_parallel_sampling: bool = False,
     config_tracking: bool = True,
+    max_total_eval_time: float = np.inf,
 ) -> list[ObjectiveFuncWrapper]:
     """Return multiple wrapper instances.
 
     Args:
         obj_func (ObjectiveFuncType):
             A callable object that serves as the objective function.
             Args:
@@ -165,14 +167,19 @@
             Whether sampling can happen in parallel.
             In many cases, sampler will not be run in parallel and then allow_parallel_sampling should be False.
             The default value is False.
         config_tracking (bool):
             Whether to validate config_id provided from the user side.
             It slows the simulation down when n_evals is large (> 3000),
             but it is recommended to avoid unexpected bugs that could happen.
+        max_total_eval_time (float):
+            The maximum total evaluation time for the optimization.
+            For example, if max_total_eval_time=3600, the simulation evaluates until the simulated cumulative time
+            reaches 3600 seconds.
+            It is useful to combine with a large n_evals and n_actual_evals_in_opt.
 
     Returns:
         wrappers (list[ObjectiveFuncWrapper]):
             A list of wrappers.
             It contains n_workers of worker wrappers.
     """
     curtime = datetime.now().strftime("%Y-%m-%d-%H:%M:%S.%f")
@@ -195,14 +202,15 @@
         seed=seed,
         continual_max_fidel=continual_max_fidel,
         max_waiting_time=max_waiting_time,
         check_interval_time=check_interval_time,
         store_config=store_config,
         allow_parallel_sampling=allow_parallel_sampling,
         config_tracking=config_tracking,
+        max_total_eval_time=max_total_eval_time,
         _async_instantiations=False,
     )
     return [ObjectiveFuncWrapper(**wrapper_kwargs, worker_index=i) for i in range(n_workers)]  # type: ignore[arg-type]
 
 
 class ObjectiveFuncWrapper:
     """Objective function wrapper API for users.
@@ -258,14 +266,16 @@
         continual_max_fidel: int | None = None,
         max_waiting_time: float = np.inf,
         check_interval_time: float = 1e-4,
         store_config: bool = False,
         allow_parallel_sampling: bool = False,
         config_tracking: bool = True,
         worker_index: int | None = None,
+        max_total_eval_time: float = np.inf,
+        careful_init: bool = False,
         _async_instantiations: bool = True,
     ):
         """The initialization of a wrapper class.
 
         Both ObjectiveFuncWorker and CentralWorkerManager have the same interface and the same set of control params.
 
         Args:
@@ -349,14 +359,23 @@
                 It specifies which worker index will be used for this wrapper.
                 It is typically useful when you run this wrapper from different processes in parallel.
                 If you did not specify this index, our wrapper automatically allocates worker indices,
                 but this may sometimes fail (in our environment with 0.01% of the probability for n_workers=8).
                 The failure rate might be higher especially when you use a large n_workers, so in that case,
                 probably users would like to use this option.
                 The worker indices must be unique across the parallel workers and must be in [0, n_workers - 1].
+            max_total_eval_time (float):
+                The maximum total evaluation time for the optimization.
+                For example, if max_total_eval_time=3600, the simulation evaluates until the simulated cumulative time
+                reaches 3600 seconds.
+                It is useful to combine with a large n_evals and n_actual_evals_in_opt.
+            careful_init (bool):
+                Whether doing initialization very carefully or not in the default setup (and only for the default).
+                If True, we try to match the initialization order using sleep.
+                It is not necessary for normal usage, but if users expect perfect reproducibility, users want to use it.
             _async_instantiations (bool):
                 Whether each worker is instantiated asynchrously.
                 In other words, whether to wait all workers' instantiations or not.
                 This argument must not be touched by users.
         """
         curtime = datetime.now().strftime("%Y-%m-%d-%H:%M:%S.%f")
         wrapper_vars = _WrapperVars(
@@ -371,14 +390,15 @@
             seed=seed,
             continual_max_fidel=continual_max_fidel,
             max_waiting_time=max_waiting_time,
             check_interval_time=check_interval_time,
             store_config=store_config,
             allow_parallel_sampling=allow_parallel_sampling,
             config_tracking=config_tracking,
+            max_total_eval_time=max_total_eval_time,
         )
 
         self._main_wrapper: _AskTellWorkerManager | _CentralWorkerManager | _ObjectiveFuncWorker
         self._validate(
             save_dir_name=save_dir_name,
             ask_and_tell=ask_and_tell,
             launch_multiple_wrappers_from_user_side=launch_multiple_wrappers_from_user_side,
@@ -388,25 +408,29 @@
         if ask_and_tell:
             self._main_wrapper = _AskTellWorkerManager(wrapper_vars)
         elif launch_multiple_wrappers_from_user_side:
             self._main_wrapper = _ObjectiveFuncWorker(
                 wrapper_vars, worker_index=worker_index, async_instantiations=_async_instantiations
             )
         else:
-            self._main_wrapper = _CentralWorkerManager(wrapper_vars)
+            self._main_wrapper = _CentralWorkerManager(wrapper_vars, careful_init=careful_init)
 
     @property
     def dir_name(self) -> str:
         return self._main_wrapper.dir_name
 
     @property
     def result_file_path(self) -> str:
         return self._main_wrapper._paths.result
 
     @property
+    def optimizer_overhead_file_path(self) -> str:
+        return self._main_wrapper._paths.sampled_time
+
+    @property
     def obj_keys(self) -> list[str]:
         return self._main_wrapper.obj_keys
 
     @property
     def runtime_key(self) -> str:
         return self._main_wrapper.runtime_key
 
@@ -418,14 +442,26 @@
     def n_actual_evals_in_opt(self) -> int:
         return self._main_wrapper._wrapper_vars.n_actual_evals_in_opt
 
     @property
     def n_workers(self) -> int:
         return self._main_wrapper._wrapper_vars.n_workers
 
+    def get_results(self) -> dict[str, list[int | float | str | bool]]:
+        with open(self.result_file_path, mode="r") as f:
+            results = json.load(f)
+
+        return results
+
+    def get_optimizer_overhead(self) -> dict[str, list[float]]:
+        with open(self.optimizer_overhead_file_path, mode="r") as f:
+            results = json.load(f)
+
+        return results
+
     def _validate(
         self,
         save_dir_name: str | None,
         ask_and_tell: bool,
         launch_multiple_wrappers_from_user_side: bool,
         n_workers: int,
         worker_index: int | None,
```

## benchmark_simulator/_simulator/_utils.py

```diff
@@ -1,12 +1,21 @@
 from __future__ import annotations
 
 from benchmark_simulator._constants import AbstractAskTellOptimizer
 
 
+def _raise_optimizer_init_error() -> None:
+    msg = [
+        "The initialization of the optimizer must be cheaper than one objective evuation.",
+        "In principle, n_workers is too large for the objective to simulate correctly."
+        "Please set a smaller n_workers or use a cheaper initialization.",
+    ]
+    raise TimeoutError("\n".join(msg))
+
+
 def _validate_opt_class(opt: AbstractAskTellOptimizer) -> None:
     if not hasattr(opt, "ask") or not hasattr(opt, "tell"):
         example_url = "https://github.com/nabenabe0928/mfhpo-simulator/blob/main/examples/ask_and_tell/"
         opt_cls = AbstractAskTellOptimizer
         error_lines = [
             "opt must have `ask` and `tell` methods.",
             f"Inherit `{opt_cls.__name__}` and encapsulate your optimizer instance in the child class.",
```

## benchmark_simulator/_simulator/_worker.py

```diff
@@ -2,37 +2,38 @@
 
 import os
 import time
 from typing import Any
 
 from benchmark_simulator._constants import (
     INF,
+    _SampledTimeDictType,
     _TIME_VALUES,
-    _TimeNowDictType,
     _WorkerVars,
     _WrapperVars,
 )
 from benchmark_simulator._secure_proc import (
     _fetch_cumtimes,
-    _fetch_timenow,
+    _fetch_sampled_time,
     _fetch_timestamps,
     _finish_worker_timer,
     _init_simulator,
     _is_simulator_terminated,
     _record_cumtime,
     _record_result,
-    _record_timenow,
+    _record_sampled_time,
     _record_timestamp,
     _start_timestamp,
     _start_worker_timer,
     _wait_all_workers,
     _wait_until_next,
 )
 from benchmark_simulator._simulator._base_wrapper import _BaseWrapperInterface
 from benchmark_simulator._simulator._utils import (
+    _raise_optimizer_init_error,
     _validate_fidel_args,
     _validate_fidels,
     _validate_fidels_continual,
     _validate_output,
 )
 from benchmark_simulator._trackers._config_tracker import _ConfigIDTracker
 from benchmark_simulator._trackers._state_tracker import _StateTracker
@@ -54,14 +55,22 @@
         self._temp_worker_index = worker_index
         self._async_inst = async_instantiations
         super().__init__(wrapper_vars=wrapper_vars)
 
     def __repr__(self) -> str:
         return f"Worker-{self._worker_vars.worker_id}"
 
+    def _init_timestamp(self) -> None:
+        _start_timestamp(
+            path=self._paths.timestamp,
+            worker_id=self._worker_vars.worker_id,
+            prev_timestamp=time.time(),
+            lock=self._lock,
+        )
+
     def _init_worker(self, worker_id: str) -> None:
         os.makedirs(self.dir_name, exist_ok=True)
         self._state_tracker = _StateTracker(
             path=self._paths.state_cache, lock=self._lock, continual_max_fidel=self._wrapper_vars.continual_max_fidel
         )
         self._config_tracker = _ConfigIDTracker(path=self._paths.config_tracker, lock=self._lock)
         _init_simulator(dir_name=self.dir_name, worker_index=self._temp_worker_index)
@@ -106,14 +115,15 @@
             continual_eval=continual_eval,
             worker_id=worker_id,
             worker_index=worker_index,
             rng=np.random.RandomState(self._wrapper_vars.seed),
             use_fidel=self._wrapper_vars.fidel_keys is not None,
             stored_obj_keys=list(set(self.obj_keys + [self.runtime_key])),
         )
+        self._init_timestamp()
 
         # These variables change over time and must be either loaded from file system or updated.
         self._cumtime = 0.0
         self._terminated = False
         self._crashed = False
         self._used_config: dict[str, Any] = {}
 
@@ -234,51 +244,53 @@
             **self._used_config,
         )
         # Record the results to the main database when the cumulative runtime is the smallest
         _record_result(
             self._paths.result, results=row, fixed=bool(not self._wrapper_vars.store_config), lock=self._lock
         )
         self._used_config = {}  # Make it empty
-        if _is_simulator_terminated(self._paths.result, max_evals=self._wrapper_vars.n_evals, lock=self._lock):
+        if _is_simulator_terminated(
+            self._paths.result,
+            max_evals=self._wrapper_vars.n_evals,
+            max_total_eval_time=self._wrapper_vars.max_total_eval_time,
+            lock=self._lock,
+        ):
             self._finish()
 
-    def _load_timestamps(self) -> float:
-        timestamp_dict = _fetch_timestamps(self._paths.timestamp, lock=self._lock)
+    def _load_timestamps(self) -> None:
         worker_id = self._worker_vars.worker_id
-        if worker_id not in timestamp_dict:  # Initialize the timestamp
-            timestamp = time.time()
-            _start_timestamp(
-                path=self._paths.timestamp,
-                worker_id=worker_id,
-                prev_timestamp=timestamp,
-                lock=self._lock,
-            )
-            return timestamp
-
-        timenow_data = _fetch_timenow(path=self._paths.timenow, lock=self._lock)
-        cumtime = _fetch_cumtimes(self._paths.worker_cumtime, lock=self._lock)[worker_id]
+        sampling_time = max(0.0, time.time() - _fetch_timestamps(self._paths.timestamp, lock=self._lock)[worker_id])
+        sampled_time = _fetch_sampled_time(path=self._paths.sampled_time, lock=self._lock)
+        cumtimes = _fetch_cumtimes(self._paths.worker_cumtime, lock=self._lock)
+        cumtime = cumtimes[worker_id]
+        is_init_sample = bool(cumtime < 1e-12)
         # Consider the sampling time overlap
         self._cumtime = (
-            max(cumtime, np.max(timenow_data["after_sample"][timenow_data["before_sample"] <= cumtime]))
-            if not self._wrapper_vars.allow_parallel_sampling
+            max(cumtime, np.max(sampled_time["after_sample"][sampled_time["before_sample"] <= cumtime]))
+            if not self._wrapper_vars.allow_parallel_sampling and not is_init_sample
             else cumtime
-        )
-        self._terminated = self._cumtime >= _TIME_VALUES.terminated - 1e-5
+        ) + sampling_time
+        if cumtime < 1e-12 and any(1e-12 < ct < self._cumtime for ct in cumtimes.values()):
+            _raise_optimizer_init_error()
+
+        new_sampled_time = _SampledTimeDictType(before_sample=self._cumtime - sampling_time, after_sample=self._cumtime)
+        _record_sampled_time(path=self._paths.sampled_time, sampled_time=new_sampled_time, lock=self._lock)
+
+        self._terminated = self._cumtime >= min(self._wrapper_vars.max_total_eval_time, _TIME_VALUES.terminated - 1e-5)
         self._crashed = self._cumtime >= _TIME_VALUES.crashed - 1e-5
-        return timestamp_dict[worker_id]
 
     def __call__(
         self,
         eval_config: dict[str, Any],
         *,
         fidels: dict[str, int | float] | None = None,
         config_id: int | None = None,
         **data_to_scatter: Any,
     ) -> dict[str, float]:
-        prev_timestamp = self._load_timestamps()
+        self._load_timestamps()
         self._validate()
         _validate_fidels(
             fidels=fidels,
             fidel_keys=self._fidel_keys,
             use_fidel=self._worker_vars.use_fidel,
             continual_eval=self._worker_vars.continual_eval,
         )
@@ -286,19 +298,14 @@
         if config_tracking:  # validate the config_id to ensure the user implementation is correct
             assert config_id is not None  # mypy redefinition
             self._config_tracker.validate(config=eval_config, config_id=config_id)
 
         if self._terminated:
             return {**{k: INF for k in self._obj_keys}, self.runtime_key: INF}
 
-        sampling_time = max(0.0, time.time() - prev_timestamp)
-        timenow_data = _TimeNowDictType(before_sample=self._cumtime, after_sample=self._cumtime + sampling_time)
-        _record_timenow(path=self._paths.timenow, timenow_data=timenow_data, lock=self._lock)
-
-        self._cumtime += sampling_time
         results = self._proc_output(eval_config=eval_config, fidels=fidels, config_id=config_id, **data_to_scatter)
         self._post_proc(results)
         return results
 
     def _finish(self) -> None:
         """The method to close the worker instance.
         This method must be called before we finish the optimization.
```

## benchmark_simulator/_simulator/_worker_manager.py

```diff
@@ -1,19 +1,16 @@
 from __future__ import annotations
 
 import os
 import threading
+import time
 from typing import Any
 
-from benchmark_simulator._secure_proc import (
-    _allocate_proc_to_worker,
-    _fetch_proc_alloc,
-    _is_allocation_ready,
-    _wait_proc_allocation,
-)
+from benchmark_simulator._constants import _WrapperVars
+from benchmark_simulator._secure_proc import _allocate_proc_to_worker, _fetch_proc_alloc, _is_allocation_ready
 from benchmark_simulator._simulator._base_wrapper import _BaseWrapperInterface
 from benchmark_simulator._simulator._worker import _ObjectiveFuncWorker
 
 
 class _CentralWorkerManager(_BaseWrapperInterface):
     """A central worker manager class.
     This class is supposed to be instantiated if the optimizer module uses multiprocessing.
@@ -21,17 +18,22 @@
     This class recognizes each worker by process ID.
     Therefore, process ID for each worker must be always unique and identical.
 
     Note:
         See benchmark_simulator/simulator.py to know variables shared across workers.
     """
 
+    def __init__(self, wrapper_vars: _WrapperVars, careful_init: bool):
+        self._careful_init = careful_init
+        super().__init__(wrapper_vars=wrapper_vars)
+
     def _init_wrapper(self) -> None:
         self._workers: list[_ObjectiveFuncWorker]
         self._main_pid = os.getpid()
+        self._n_workers = self._wrapper_vars.n_workers
         self._init_workers()
         self._pid_to_index: dict[int, int] = {}
 
     def _init_workers(self) -> None:
         if os.path.exists(self.dir_name):
             raise FileExistsError(f"The directory `{self.dir_name}` already exists. Remove it first.")
 
@@ -40,33 +42,35 @@
             _ObjectiveFuncWorker(wrapper_vars=self._wrapper_vars, worker_index=i, async_instantiations=False)
             for i in range(n_workers)
         ]
 
     def _init_alloc(self, pid: int) -> None:
         path = self._paths.proc_alloc
         if not _is_allocation_ready(path=path, n_workers=self._wrapper_vars.n_workers, lock=self._lock):
-            _allocate_proc_to_worker(path=path, pid=pid, lock=self._lock)
-            self._pid_to_index = _wait_proc_allocation(
-                path=path, n_workers=self._wrapper_vars.n_workers, lock=self._lock
-            )
+            # _allocate_proc_to_worker will not be called twice by each process due to wait_other_workers
+            worker_index = _allocate_proc_to_worker(path=path, pid=pid, time_ns=time.time_ns(), lock=self._lock)
+            # Important to match the init eval order. The longest latency has 2 * self._n_workers * waiting_time
+            waiting_time = 1e-4
+            time.sleep(self._careful_init * 2 * self._n_workers * waiting_time * worker_index)
+            self._pid_to_index = {pid: worker_index}
         else:
             # This line is actually covered, but it is not visible due to multiprocessing nature
             self._pid_to_index = _fetch_proc_alloc(path=path, lock=self._lock)  # pragma: no cover
 
     def __call__(
         self,
         eval_config: dict[str, Any],
         *,
         fidels: dict[str, int | float] | None = None,
         config_id: int | None = None,
         **data_to_scatter: Any,
     ) -> dict[str, float]:
         pid = os.getpid()
         pid = threading.get_ident() if pid == self._main_pid else pid
-        if len(self._pid_to_index) != self._wrapper_vars.n_workers:
+        if len(self._pid_to_index) != self._n_workers:
             self._init_alloc(pid)
 
         if pid not in self._pid_to_index:  # pragma: no cover
             raise ProcessLookupError(
                 f"An unknown process/thread with ID {pid} was specified.\n"
                 "It is likely that one of the workers crashed and a new worker was added or \n"
                 f"n_workers in ObjectiveFuncWrapper and your optimizer were incompatible.\n"
```

## benchmark_simulator/_simulator/_worker_manager_for_ask_and_tell.py

```diff
@@ -3,14 +3,15 @@
 import os
 import time
 from typing import Any
 
 from benchmark_simulator._constants import AbstractAskTellOptimizer, _ResultData, _StateType, _WorkerVars
 from benchmark_simulator._simulator._base_wrapper import _BaseWrapperInterface
 from benchmark_simulator._simulator._utils import (
+    _raise_optimizer_init_error,
     _validate_fidel_args,
     _validate_fidels,
     _validate_fidels_continual,
     _validate_opt_class,
     _validate_output,
 )
 from benchmark_simulator._trackers._config_tracker import _AskTellConfigIDTracker
@@ -38,14 +39,15 @@
         self._wrapper_vars.validate()
         _validate_fidel_args(continual_eval=self._worker_vars.continual_eval, fidel_keys=self._fidel_keys)
 
         self._timenow = 0.0
         self._cumtimes: np.ndarray = np.zeros(self._wrapper_vars.n_workers, dtype=np.float64)
         self._pending_results: list[_ResultData | None] = [None] * self._wrapper_vars.n_workers
         self._seen_config_keys: list[str] = []
+        self._sampled_time: dict[str, list[float]] = {"before_sample": [], "after_sample": []}
         self._results: dict[str, list[Any]] = {"worker_index": [], "cumtime": []}
         self._results.update({k: [] for k in self._obj_keys})
         if self._wrapper_vars.store_config:
             self._results.update({k: [] for k in self._fidel_keys + ["seed"]})
             if self._wrapper_vars.continual_max_fidel is not None:
                 self._results["prev_fidel"] = []
 
@@ -152,20 +154,29 @@
         eval_config, fidels, config_id = opt.ask()
         config_tracking = config_id is not None and self._wrapper_vars.config_tracking
         if config_tracking:  # validate the config_id to ensure the user implementation is correct
             assert config_id is not None  # mypy redefinition
             self._config_tracker.validate(config=eval_config, config_id=config_id)
 
         sampling_time = time.time() - start
+        is_first_sample = bool(self._cumtimes[worker_id] < 1e-12)
         if self._wrapper_vars.allow_parallel_sampling:
             self._cumtimes[worker_id] = self._cumtimes[worker_id] + sampling_time
         else:
             self._timenow = max(self._timenow, self._cumtimes[worker_id]) + sampling_time
             self._cumtimes[worker_id] = self._timenow
 
+        self._sampled_time["before_sample"].append(self._cumtimes[worker_id] - sampling_time)
+        self._sampled_time["after_sample"].append(self._cumtimes[worker_id])
+
+        if is_first_sample and not np.isclose(
+            self._cumtimes[worker_id], np.min(self._cumtimes[self._cumtimes > 1e-12])
+        ):
+            _raise_optimizer_init_error()
+
         return eval_config, fidels, config_id
 
     def _tell_pending_result(self, opt: AbstractAskTellOptimizer, worker_id: int) -> None:
         result_data = self._pending_results[worker_id]
         if result_data is None:
             return
 
@@ -178,17 +189,23 @@
         )
         self._pending_results[worker_id] = None
 
     def _save_results(self) -> None:
         with open(self._paths.result, mode="w") as f:
             json.dump({k: np.asarray(v).tolist() for k, v in self._results.items()}, f, indent=4)
 
+        with open(self._paths.sampled_time, mode="w") as f:
+            json.dump({k: np.asarray(v).tolist() for k, v in self._sampled_time.items()}, f, indent=4)
+
     def simulate(self, opt: AbstractAskTellOptimizer) -> None:
         _validate_opt_class(opt)
         worker_id = 0
         for _ in range(self._wrapper_vars.n_evals + self._wrapper_vars.n_workers - 1):
             eval_config, fidels, config_id = self._ask_with_timer(opt=opt, worker_id=worker_id)
             self._proc_obj_func(eval_config=eval_config, worker_id=worker_id, fidels=fidels, config_id=config_id)
             worker_id = np.argmin(self._cumtimes)
             self._tell_pending_result(opt=opt, worker_id=worker_id)
 
+            if self._cumtimes[worker_id] > self._wrapper_vars.max_total_eval_time:  # exceed time limit
+                break
+
         self._save_results()
```

## Comparing `mfhpo_simulator-1.2.4.dist-info/LICENSE` & `mfhpo_simulator-1.2.5.dist-info/LICENSE`

 * *Files identical despite different names*

