# Comparing `tmp/dlrover-0.1.0rc0.dev1-py3-none-any.whl.zip` & `tmp/dlrover-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,151 +1,193 @@
-Zip file size: 214203 bytes, number of entries: 149
--rw-r--r--  2.0 unx      411 b- defN 22-Nov-17 02:43 dlrover/Makefile
--rw-r--r--  2.0 unx      599 b- defN 22-Nov-07 08:41 dlrover/__init__.py
--rw-r--r--  2.0 unx       70 b- defN 22-Dec-09 03:19 dlrover/requirements.txt
--rw-r--r--  2.0 unx     4440 b- defN 22-Dec-16 11:20 dlrover/proto/brain.proto
--rw-r--r--  2.0 unx    23048 b- defN 22-Dec-15 10:19 dlrover/proto/brain_pb2.py
--rw-r--r--  2.0 unx     5867 b- defN 22-Dec-15 10:19 dlrover/proto/brain_pb2_grpc.py
--rw-r--r--  2.0 unx     7206 b- defN 22-Dec-16 11:20 dlrover/proto/elastic_training.proto
--rw-r--r--  2.0 unx    28522 b- defN 22-Dec-15 10:19 dlrover/proto/elastic_training_pb2.py
--rw-r--r--  2.0 unx    40617 b- defN 22-Dec-15 10:19 dlrover/proto/elastic_training_pb2_grpc.py
--rw-r--r--  2.0 unx      599 b- defN 22-Nov-07 08:41 dlrover/python/__init__.py
--rw-r--r--  2.0 unx      599 b- defN 22-Dec-09 03:19 dlrover/python/brain/__init__.py
--rw-r--r--  2.0 unx    10825 b- defN 23-Jan-04 02:24 dlrover/python/brain/client.py
--rw-r--r--  2.0 unx      599 b- defN 22-Nov-07 08:41 dlrover/python/common/__init__.py
--rw-r--r--  2.0 unx     4215 b- defN 23-Jan-13 13:40 dlrover/python/common/constants.py
--rw-r--r--  2.0 unx     4944 b- defN 22-Dec-21 01:25 dlrover/python/common/global_context.py
--rw-r--r--  2.0 unx     1598 b- defN 22-Dec-02 09:08 dlrover/python/common/grpc.py
--rw-r--r--  2.0 unx     1344 b- defN 22-Dec-02 09:08 dlrover/python/common/log.py
--rw-r--r--  2.0 unx     8093 b- defN 23-Jan-14 02:43 dlrover/python/common/node.py
--rw-r--r--  2.0 unx      923 b- defN 23-Jan-10 02:20 dlrover/python/common/serialize.py
--rw-r--r--  2.0 unx      905 b- defN 22-Dec-02 09:08 dlrover/python/common/singleton.py
--rw-r--r--  2.0 unx      599 b- defN 22-Dec-10 12:25 dlrover/python/elastic_agent/__init__.py
--rw-r--r--  2.0 unx    16066 b- defN 22-Dec-22 09:56 dlrover/python/elastic_agent/master_client.py
--rw-r--r--  2.0 unx      599 b- defN 22-Dec-02 09:08 dlrover/python/elastic_agent/monitor/__init__.py
--rw-r--r--  2.0 unx     3154 b- defN 22-Dec-16 11:20 dlrover/python/elastic_agent/monitor/resource.py
--rw-r--r--  2.0 unx     2483 b- defN 22-Dec-16 11:20 dlrover/python/elastic_agent/monitor/training.py
--rw-r--r--  2.0 unx      599 b- defN 22-Dec-02 09:08 dlrover/python/elastic_agent/sharding/__init__.py
--rw-r--r--  2.0 unx     6983 b- defN 22-Dec-16 13:47 dlrover/python/elastic_agent/sharding/client.py
--rw-r--r--  2.0 unx      599 b- defN 22-Dec-02 09:08 dlrover/python/elastic_agent/tensorflow/__init__.py
--rw-r--r--  2.0 unx     3397 b- defN 22-Dec-24 11:33 dlrover/python/elastic_agent/tensorflow/elastic_ps.py
--rw-r--r--  2.0 unx     3932 b- defN 22-Dec-16 13:47 dlrover/python/elastic_agent/tensorflow/hooks.py
--rw-r--r--  2.0 unx     4556 b- defN 22-Dec-02 09:08 dlrover/python/elastic_agent/tensorflow/profile_extractor.py
--rw-r--r--  2.0 unx      599 b- defN 22-Nov-07 08:41 dlrover/python/master/__init__.py
--rw-r--r--  2.0 unx     2879 b- defN 22-Dec-21 09:44 dlrover/python/master/args.py
--rw-r--r--  2.0 unx     1827 b- defN 22-Dec-21 01:25 dlrover/python/master/main.py
--rw-r--r--  2.0 unx     7564 b- defN 23-Jan-13 09:51 dlrover/python/master/master.py
--rw-r--r--  2.0 unx    16440 b- defN 23-Jan-11 09:48 dlrover/python/master/servicer.py
--rw-r--r--  2.0 unx      599 b- defN 22-Dec-09 03:19 dlrover/python/master/elastic_training/__init__.py
--rw-r--r--  2.0 unx     3414 b- defN 22-Dec-02 09:08 dlrover/python/master/elastic_training/elastic_ps.py
--rw-r--r--  2.0 unx      599 b- defN 22-Nov-15 06:22 dlrover/python/master/monitor/__init__.py
--rw-r--r--  2.0 unx     5779 b- defN 23-Jan-06 09:06 dlrover/python/master/monitor/speed_monitor.py
--rw-r--r--  2.0 unx      599 b- defN 22-Dec-09 03:19 dlrover/python/master/node/__init__.py
--rw-r--r--  2.0 unx     7190 b- defN 23-Jan-11 01:38 dlrover/python/master/node/event_callback.py
--rw-r--r--  2.0 unx    26929 b- defN 23-Jan-14 02:24 dlrover/python/master/node/node_manager.py
--rw-r--r--  2.0 unx    13412 b- defN 23-Jan-10 08:35 dlrover/python/master/node/ps.py
--rw-r--r--  2.0 unx     3663 b- defN 22-Nov-24 06:42 dlrover/python/master/node/status_flow.py
--rw-r--r--  2.0 unx     9557 b- defN 23-Jan-16 03:08 dlrover/python/master/node/training_node.py
--rw-r--r--  2.0 unx     8970 b- defN 23-Jan-06 06:05 dlrover/python/master/node/worker.py
--rw-r--r--  2.0 unx      599 b- defN 22-Nov-24 05:59 dlrover/python/master/resource/__init__.py
--rw-r--r--  2.0 unx     4153 b- defN 23-Jan-06 01:42 dlrover/python/master/resource/brain_optimizer.py
--rw-r--r--  2.0 unx    16950 b- defN 23-Jan-13 13:40 dlrover/python/master/resource/job.py
--rw-r--r--  2.0 unx    13010 b- defN 23-Jan-13 09:51 dlrover/python/master/resource/local_optimizer.py
--rw-r--r--  2.0 unx     5349 b- defN 22-Dec-21 01:25 dlrover/python/master/resource/optimizer.py
--rw-r--r--  2.0 unx      599 b- defN 22-Nov-09 09:03 dlrover/python/master/scaler/__init__.py
--rw-r--r--  2.0 unx     1994 b- defN 23-Jan-11 12:02 dlrover/python/master/scaler/base_scaler.py
--rw-r--r--  2.0 unx     5562 b- defN 22-Dec-21 01:25 dlrover/python/master/scaler/elasticjob_scaler.py
--rw-r--r--  2.0 unx     1149 b- defN 22-Dec-20 10:15 dlrover/python/master/scaler/factory.py
--rw-r--r--  2.0 unx    21985 b- defN 23-Jan-16 02:19 dlrover/python/master/scaler/pod_scaler.py
--rw-r--r--  2.0 unx      599 b- defN 22-Nov-24 06:42 dlrover/python/master/shard/__init__.py
--rw-r--r--  2.0 unx     4304 b- defN 22-Dec-16 13:47 dlrover/python/master/shard/base_dataset_manager.py
--rw-r--r--  2.0 unx     6345 b- defN 23-Jan-04 09:03 dlrover/python/master/shard/batch_dataset_manager.py
--rw-r--r--  2.0 unx    15618 b- defN 23-Jan-04 09:03 dlrover/python/master/shard/dataset_splitter.py
--rw-r--r--  2.0 unx     7064 b- defN 22-Dec-17 03:34 dlrover/python/master/shard/streaming_dataset_manager.py
--rw-r--r--  2.0 unx     9505 b- defN 23-Jan-11 07:59 dlrover/python/master/shard/task_manager.py
--rw-r--r--  2.0 unx      599 b- defN 22-Nov-24 06:42 dlrover/python/master/stats/__init__.py
--rw-r--r--  2.0 unx     6394 b- defN 23-Jan-11 09:48 dlrover/python/master/stats/job_collector.py
--rw-r--r--  2.0 unx     3484 b- defN 23-Jan-13 09:51 dlrover/python/master/stats/reporter.py
--rw-r--r--  2.0 unx     4344 b- defN 22-Dec-16 13:47 dlrover/python/master/stats/training_metrics.py
--rw-r--r--  2.0 unx      599 b- defN 22-Nov-24 06:42 dlrover/python/master/watcher/__init__.py
--rw-r--r--  2.0 unx     1241 b- defN 22-Nov-29 03:04 dlrover/python/master/watcher/base_watcher.py
--rw-r--r--  2.0 unx     1079 b- defN 22-Dec-09 03:19 dlrover/python/master/watcher/factory.py
--rw-r--r--  2.0 unx     5727 b- defN 23-Jan-10 02:20 dlrover/python/master/watcher/pod_watcher.py
--rw-r--r--  2.0 unx      599 b- defN 22-Nov-10 02:23 dlrover/python/scheduler/__init__.py
--rw-r--r--  2.0 unx     1393 b- defN 22-Dec-15 08:57 dlrover/python/scheduler/factory.py
--rw-r--r--  2.0 unx     3458 b- defN 22-Dec-16 11:20 dlrover/python/scheduler/job.py
--rw-r--r--  2.0 unx    12081 b- defN 23-Jan-13 13:40 dlrover/python/scheduler/kubernetes.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jan-16 04:20 dlrover/python/tests/__init__.py
--rw-r--r--  2.0 unx     1668 b- defN 22-Dec-16 11:20 dlrover/python/tests/test_agent_monitor.py
--rw-r--r--  2.0 unx     1049 b- defN 22-Dec-07 01:42 dlrover/python/tests/test_args.py
--rw-r--r--  2.0 unx     4595 b- defN 22-Dec-02 06:13 dlrover/python/tests/test_dataset_splitter.py
--rw-r--r--  2.0 unx     3008 b- defN 22-Dec-12 08:29 dlrover/python/tests/test_dataset_task_manager.py
--rw-r--r--  2.0 unx     2160 b- defN 23-Jan-13 13:40 dlrover/python/tests/test_job_params.py
--rw-r--r--  2.0 unx     1909 b- defN 23-Jan-13 13:40 dlrover/python/tests/test_k8s_scaler.py
--rw-r--r--  2.0 unx     6830 b- defN 22-Dec-15 05:49 dlrover/python/tests/test_local_optimizer.py
--rw-r--r--  2.0 unx     2751 b- defN 22-Dec-22 06:27 dlrover/python/tests/test_master.py
--rw-r--r--  2.0 unx    13885 b- defN 23-Jan-13 13:40 dlrover/python/tests/test_node_manager.py
--rw-r--r--  2.0 unx      599 b- defN 22-Nov-17 02:07 dlrover/python/tests/test_node_watcher.py
--rw-r--r--  2.0 unx     5491 b- defN 23-Jan-11 11:45 dlrover/python/tests/test_pod_scaler.py
--rw-r--r--  2.0 unx     3707 b- defN 22-Dec-16 13:47 dlrover/python/tests/test_pod_watcher.py
--rw-r--r--  2.0 unx     6234 b- defN 23-Jan-13 13:40 dlrover/python/tests/test_ps_manager.py
--rw-r--r--  2.0 unx     8459 b- defN 23-Jan-13 13:40 dlrover/python/tests/test_resource_optimizer.py
--rw-r--r--  2.0 unx     6434 b- defN 23-Jan-11 07:59 dlrover/python/tests/test_servicer.py
--rw-r--r--  2.0 unx     1932 b- defN 22-Dec-02 09:08 dlrover/python/tests/test_sharding_client.py
--rw-r--r--  2.0 unx     1482 b- defN 22-Dec-13 01:52 dlrover/python/tests/test_speed_monitor.py
--rw-r--r--  2.0 unx     2254 b- defN 22-Dec-15 05:49 dlrover/python/tests/test_stats_collector.py
--rw-r--r--  2.0 unx     4136 b- defN 22-Dec-12 08:29 dlrover/python/tests/test_task_manager.py
--rw-r--r--  2.0 unx     5866 b- defN 23-Jan-13 13:40 dlrover/python/tests/test_utils.py
--rw-r--r--  2.0 unx     4379 b- defN 23-Jan-13 13:40 dlrover/python/tests/test_worker_manager.py
--rw-r--r--  2.0 unx      599 b- defN 23-Jan-03 01:41 dlrover/trainer/__init__.py
--rw-r--r--  2.0 unx      778 b- defN 23-Jan-04 08:41 dlrover/trainer/__main__.py
--rw-r--r--  2.0 unx      599 b- defN 23-Jan-03 01:41 dlrover/trainer/constants/__init__.py
--rw-r--r--  2.0 unx     1090 b- defN 23-Jan-03 01:41 dlrover/trainer/constants/constants.py
--rw-r--r--  2.0 unx      956 b- defN 23-Jan-03 01:41 dlrover/trainer/constants/platform_constants.py
--rw-r--r--  2.0 unx     2703 b- defN 23-Jan-13 09:51 dlrover/trainer/constants/tf_constants.py
--rw-r--r--  2.0 unx      599 b- defN 23-Jan-03 01:41 dlrover/trainer/entry/__init__.py
--rw-r--r--  2.0 unx      967 b- defN 23-Jan-03 01:41 dlrover/trainer/entry/local_entry.py
--rw-r--r--  2.0 unx      599 b- defN 23-Jan-13 09:51 dlrover/trainer/examples/__init__.py
--rw-r--r--  2.0 unx     2364 b- defN 23-Jan-13 09:51 dlrover/trainer/examples/estimator_executor/MyEstimator.py
--rw-r--r--  2.0 unx      599 b- defN 23-Jan-13 09:51 dlrover/trainer/examples/estimator_executor/__init__.py
--rw-r--r--  2.0 unx     1649 b- defN 23-Jan-13 09:51 dlrover/trainer/examples/estimator_executor/conf.py
--rw-r--r--  2.0 unx      599 b- defN 23-Jan-03 01:41 dlrover/trainer/mock/__init__.py
--rw-r--r--  2.0 unx     4086 b- defN 23-Jan-04 08:41 dlrover/trainer/mock/base_process_scheduler.py
--rw-r--r--  2.0 unx     5686 b- defN 23-Jan-04 08:41 dlrover/trainer/mock/tf_process_scheduler.py
--rw-r--r--  2.0 unx      599 b- defN 23-Jan-03 01:41 dlrover/trainer/platform/__init__.py
--rw-r--r--  2.0 unx     2801 b- defN 23-Jan-04 08:41 dlrover/trainer/platform/starter.py
--rw-r--r--  2.0 unx      599 b- defN 23-Jan-04 08:41 dlrover/trainer/tensorflow/__init__.py
--rw-r--r--  2.0 unx      599 b- defN 23-Jan-04 08:41 dlrover/trainer/tensorflow/executor/__init__.py
--rw-r--r--  2.0 unx     6643 b- defN 23-Jan-13 09:51 dlrover/trainer/tensorflow/executor/base_executor.py
--rw-r--r--  2.0 unx     8560 b- defN 23-Jan-13 09:51 dlrover/trainer/tensorflow/executor/estimator_executor.py
--rw-r--r--  2.0 unx      599 b- defN 23-Jan-13 09:51 dlrover/trainer/tensorflow/failover/__init__.py
--rw-r--r--  2.0 unx     4455 b- defN 23-Jan-13 09:51 dlrover/trainer/tensorflow/failover/failover_client.py
--rw-r--r--  2.0 unx     6596 b- defN 23-Jan-13 09:51 dlrover/trainer/tensorflow/failover/tensorflow_failover.py
--rw-r--r--  2.0 unx      599 b- defN 23-Jan-04 08:41 dlrover/trainer/tensorflow/hooks/__init__.py
--rw-r--r--  2.0 unx     1151 b- defN 23-Jan-04 08:41 dlrover/trainer/tensorflow/hooks/elastic_data_shard_report_hook.py
--rw-r--r--  2.0 unx     1611 b- defN 23-Jan-04 08:41 dlrover/trainer/tensorflow/hooks/global_step_hook.py
--rw-r--r--  2.0 unx      599 b- defN 23-Jan-04 08:41 dlrover/trainer/tensorflow/reader/__init__.py
--rw-r--r--  2.0 unx     2625 b- defN 23-Jan-13 09:51 dlrover/trainer/tensorflow/reader/fake_reader.py
--rw-r--r--  2.0 unx     2918 b- defN 23-Jan-10 06:24 dlrover/trainer/tensorflow/reader/file_reader.py
--rw-r--r--  2.0 unx      599 b- defN 23-Jan-04 08:41 dlrover/trainer/tensorflow/util/__init__.py
--rw-r--r--  2.0 unx     1805 b- defN 23-Jan-10 06:24 dlrover/trainer/tensorflow/util/column_info.py
--rw-r--r--  2.0 unx     3666 b- defN 23-Jan-04 08:41 dlrover/trainer/tensorflow/util/common_util.py
--rw-r--r--  2.0 unx     1061 b- defN 23-Jan-09 03:26 dlrover/trainer/tensorflow/util/data_mapping_util.py
--rw-r--r--  2.0 unx     5251 b- defN 23-Jan-10 06:24 dlrover/trainer/tensorflow/util/dataset_util.py
--rw-r--r--  2.0 unx     2572 b- defN 23-Jan-04 08:41 dlrover/trainer/tensorflow/util/estimator_util.py
--rw-r--r--  2.0 unx     1122 b- defN 23-Jan-10 06:24 dlrover/trainer/tensorflow/util/path_util.py
--rw-r--r--  2.0 unx    13869 b- defN 23-Jan-13 09:51 dlrover/trainer/tensorflow/util/tf_patch_util.py
--rw-r--r--  2.0 unx     1104 b- defN 23-Jan-04 08:41 dlrover/trainer/tensorflow/util/tf_version_util.py
--rw-r--r--  2.0 unx      599 b- defN 23-Jan-03 01:41 dlrover/trainer/util/__init__.py
--rw-r--r--  2.0 unx     1849 b- defN 23-Jan-13 09:51 dlrover/trainer/util/args_util.py
--rw-r--r--  2.0 unx     6362 b- defN 23-Jan-03 01:41 dlrover/trainer/util/conf_util.py
--rw-r--r--  2.0 unx     2863 b- defN 23-Jan-09 03:26 dlrover/trainer/util/log_util.py
--rw-r--r--  2.0 unx      736 b- defN 23-Jan-03 01:41 dlrover/trainer/util/net_util.py
--rw-r--r--  2.0 unx     3860 b- defN 23-Jan-03 01:41 dlrover/trainer/util/reflect_util.py
--rw-r--r--  2.0 unx      599 b- defN 23-Jan-03 01:41 dlrover/trainer/worker/__init__.py
--rw-r--r--  2.0 unx     2186 b- defN 23-Jan-13 09:51 dlrover/trainer/worker/tf_kubernetes_worker.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jan-16 05:58 dlrover-0.1.0rc0.dev1.dist-info/LICENSE
--rw-r--r--  2.0 unx      743 b- defN 23-Jan-16 05:58 dlrover-0.1.0rc0.dev1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-16 05:58 dlrover-0.1.0rc0.dev1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jan-16 05:58 dlrover-0.1.0rc0.dev1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    14491 b- defN 23-Jan-16 05:58 dlrover-0.1.0rc0.dev1.dist-info/RECORD
-149 files, 684643 bytes uncompressed, 190681 bytes compressed:  72.1%
+Zip file size: 298868 bytes, number of entries: 191
+-rw-r--r--  2.0 unx      411 b- defN 23-Mar-07 11:16 dlrover/Makefile
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/__init__.py
+-rw-r--r--  2.0 unx     4439 b- defN 23-May-08 02:53 dlrover/proto/brain.proto
+-rw-r--r--  2.0 unx    92639 b- defN 23-Jul-25 09:08 dlrover/proto/brain_pb2.py
+-rw-r--r--  2.0 unx     5867 b- defN 23-Jul-25 09:08 dlrover/proto/brain_pb2_grpc.py
+-rw-r--r--  2.0 unx     7729 b- defN 23-Jul-25 09:06 dlrover/proto/elastic_training.proto
+-rw-r--r--  2.0 unx   105858 b- defN 23-Jul-25 09:08 dlrover/proto/elastic_training_pb2.py
+-rw-r--r--  2.0 unx    57297 b- defN 23-Jul-25 09:08 dlrover/proto/elastic_training_pb2_grpc.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/__init__.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/brain/__init__.py
+-rw-r--r--  2.0 unx    11185 b- defN 23-May-15 05:59 dlrover/python/brain/client.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/common/__init__.py
+-rw-r--r--  2.0 unx     5625 b- defN 23-Jul-25 09:06 dlrover/python/common/constants.py
+-rw-r--r--  2.0 unx     5873 b- defN 23-Jul-19 09:19 dlrover/python/common/global_context.py
+-rw-r--r--  2.0 unx     2182 b- defN 23-Jul-07 03:22 dlrover/python/common/grpc.py
+-rw-r--r--  2.0 unx     1344 b- defN 23-Mar-07 11:16 dlrover/python/common/log.py
+-rw-r--r--  2.0 unx     9732 b- defN 23-Jul-25 09:06 dlrover/python/common/node.py
+-rw-r--r--  2.0 unx      923 b- defN 23-Mar-07 11:16 dlrover/python/common/serialize.py
+-rw-r--r--  2.0 unx      905 b- defN 23-Mar-07 11:16 dlrover/python/common/singleton.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/elastic_agent/__init__.py
+-rw-r--r--  2.0 unx    20421 b- defN 23-Jul-25 09:06 dlrover/python/elastic_agent/master_client.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/elastic_agent/monitor/__init__.py
+-rw-r--r--  2.0 unx     3264 b- defN 23-Jul-07 03:22 dlrover/python/elastic_agent/monitor/resource.py
+-rw-r--r--  2.0 unx     2489 b- defN 23-May-08 02:53 dlrover/python/elastic_agent/monitor/training.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/elastic_agent/sharding/__init__.py
+-rw-r--r--  2.0 unx    12227 b- defN 23-Jul-07 03:22 dlrover/python/elastic_agent/sharding/client.py
+-rw-r--r--  2.0 unx      599 b- defN 23-May-08 02:53 dlrover/python/elastic_agent/sychronization/__init__.py
+-rw-r--r--  2.0 unx     2699 b- defN 23-May-08 02:53 dlrover/python/elastic_agent/sychronization/sync_client.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/elastic_agent/tensorflow/__init__.py
+-rw-r--r--  2.0 unx     3397 b- defN 23-Mar-07 11:16 dlrover/python/elastic_agent/tensorflow/elastic_ps.py
+-rw-r--r--  2.0 unx     3930 b- defN 23-Mar-07 11:16 dlrover/python/elastic_agent/tensorflow/hooks.py
+-rw-r--r--  2.0 unx     4556 b- defN 23-Mar-07 11:16 dlrover/python/elastic_agent/tensorflow/profile_extractor.py
+-rw-r--r--  2.0 unx      599 b- defN 23-May-08 02:53 dlrover/python/elastic_agent/torch/__init__.py
+-rw-r--r--  2.0 unx     4599 b- defN 23-Jun-29 10:15 dlrover/python/elastic_agent/torch/master_kv_store.py
+-rw-r--r--  2.0 unx    26917 b- defN 23-Jul-25 09:06 dlrover/python/elastic_agent/torch/training.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/__init__.py
+-rw-r--r--  2.0 unx     3114 b- defN 23-Jul-07 03:22 dlrover/python/master/args.py
+-rw-r--r--  2.0 unx     1960 b- defN 23-Jul-11 11:37 dlrover/python/master/main.py
+-rw-r--r--  2.0 unx     8650 b- defN 23-Jul-25 09:06 dlrover/python/master/master.py
+-rw-r--r--  2.0 unx    18494 b- defN 23-Jul-25 09:06 dlrover/python/master/servicer.py
+-rw-r--r--  2.0 unx      599 b- defN 23-May-08 02:53 dlrover/python/master/cluster/__init__.py
+-rw-r--r--  2.0 unx     1124 b- defN 23-Jul-25 09:06 dlrover/python/master/cluster/quota.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/elastic_training/__init__.py
+-rw-r--r--  2.0 unx     3494 b- defN 23-Mar-07 11:16 dlrover/python/master/elastic_training/elastic_ps.py
+-rw-r--r--  2.0 unx     1017 b- defN 23-Jun-30 02:26 dlrover/python/master/elastic_training/kv_store_service.py
+-rw-r--r--  2.0 unx    14853 b- defN 23-Jul-25 09:06 dlrover/python/master/elastic_training/rdzv_manager.py
+-rw-r--r--  2.0 unx     4944 b- defN 23-May-08 02:53 dlrover/python/master/elastic_training/sync_service.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/monitor/__init__.py
+-rw-r--r--  2.0 unx     1864 b- defN 23-Jul-25 09:06 dlrover/python/master/monitor/error_monitor.py
+-rw-r--r--  2.0 unx     7002 b- defN 23-Jun-16 02:37 dlrover/python/master/monitor/speed_monitor.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/node/__init__.py
+-rw-r--r--  2.0 unx    11103 b- defN 23-Jul-25 09:06 dlrover/python/master/node/event_callback.py
+-rw-r--r--  2.0 unx    11844 b- defN 23-Jul-25 09:06 dlrover/python/master/node/job_auto_scaler.py
+-rw-r--r--  2.0 unx    26844 b- defN 23-Jul-25 09:06 dlrover/python/master/node/job_manager.py
+-rw-r--r--  2.0 unx    14460 b- defN 23-May-10 07:56 dlrover/python/master/node/ps.py
+-rw-r--r--  2.0 unx     4046 b- defN 23-Jul-25 09:06 dlrover/python/master/node/status_flow.py
+-rw-r--r--  2.0 unx    11531 b- defN 23-Jul-25 09:06 dlrover/python/master/node/training_node.py
+-rw-r--r--  2.0 unx    10616 b- defN 23-Jul-25 09:06 dlrover/python/master/node/worker.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/resource/__init__.py
+-rw-r--r--  2.0 unx     4187 b- defN 23-May-08 02:53 dlrover/python/master/resource/brain_optimizer.py
+-rw-r--r--  2.0 unx    20985 b- defN 23-Jul-25 09:06 dlrover/python/master/resource/job.py
+-rw-r--r--  2.0 unx    15717 b- defN 23-Jul-25 09:06 dlrover/python/master/resource/local_optimizer.py
+-rw-r--r--  2.0 unx     6065 b- defN 23-May-08 02:53 dlrover/python/master/resource/optimizer.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/scaler/__init__.py
+-rw-r--r--  2.0 unx     2062 b- defN 23-May-08 02:53 dlrover/python/master/scaler/base_scaler.py
+-rw-r--r--  2.0 unx     8519 b- defN 23-May-08 02:53 dlrover/python/master/scaler/elasticjob_scaler.py
+-rw-r--r--  2.0 unx     1300 b- defN 23-Mar-07 11:16 dlrover/python/master/scaler/factory.py
+-rw-r--r--  2.0 unx    23329 b- defN 23-Jul-24 09:28 dlrover/python/master/scaler/pod_scaler.py
+-rw-r--r--  2.0 unx     4670 b- defN 23-May-08 02:53 dlrover/python/master/scaler/ray_scaler.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/shard/__init__.py
+-rw-r--r--  2.0 unx     4574 b- defN 23-Jul-20 05:59 dlrover/python/master/shard/base_dataset_manager.py
+-rw-r--r--  2.0 unx     6964 b- defN 23-May-08 02:53 dlrover/python/master/shard/batch_dataset_manager.py
+-rw-r--r--  2.0 unx    15928 b- defN 23-May-08 02:53 dlrover/python/master/shard/dataset_splitter.py
+-rw-r--r--  2.0 unx     7064 b- defN 23-Mar-07 11:16 dlrover/python/master/shard/streaming_dataset_manager.py
+-rw-r--r--  2.0 unx    10773 b- defN 23-Jul-25 09:06 dlrover/python/master/shard/task_manager.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/stats/__init__.py
+-rw-r--r--  2.0 unx     6557 b- defN 23-May-08 02:53 dlrover/python/master/stats/job_collector.py
+-rw-r--r--  2.0 unx     8730 b- defN 23-May-08 02:53 dlrover/python/master/stats/reporter.py
+-rw-r--r--  2.0 unx     1567 b- defN 23-Mar-07 11:16 dlrover/python/master/stats/stats_backend.py
+-rw-r--r--  2.0 unx     4416 b- defN 23-May-08 02:53 dlrover/python/master/stats/training_metrics.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/master/watcher/__init__.py
+-rw-r--r--  2.0 unx     1241 b- defN 23-Mar-07 11:16 dlrover/python/master/watcher/base_watcher.py
+-rw-r--r--  2.0 unx     1740 b- defN 23-Mar-07 11:16 dlrover/python/master/watcher/factory.py
+-rw-r--r--  2.0 unx    10539 b- defN 23-Jul-25 09:06 dlrover/python/master/watcher/k8s_watcher.py
+-rw-r--r--  2.0 unx     3247 b- defN 23-Mar-07 11:16 dlrover/python/master/watcher/ray_watcher.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/scheduler/__init__.py
+-rw-r--r--  2.0 unx     1649 b- defN 23-Mar-07 11:16 dlrover/python/scheduler/factory.py
+-rw-r--r--  2.0 unx     3439 b- defN 23-May-08 02:53 dlrover/python/scheduler/job.py
+-rw-r--r--  2.0 unx    12928 b- defN 23-Jul-07 03:22 dlrover/python/scheduler/kubernetes.py
+-rw-r--r--  2.0 unx     7317 b- defN 23-May-08 02:53 dlrover/python/scheduler/ray.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/tests/__init__.py
+-rw-r--r--  2.0 unx     1668 b- defN 23-Jun-19 03:52 dlrover/python/tests/test_agent_monitor.py
+-rw-r--r--  2.0 unx     1049 b- defN 23-Mar-07 11:16 dlrover/python/tests/test_args.py
+-rw-r--r--  2.0 unx     4582 b- defN 23-May-08 02:53 dlrover/python/tests/test_dataset_splitter.py
+-rw-r--r--  2.0 unx     4904 b- defN 23-May-08 02:53 dlrover/python/tests/test_dataset_task_manager.py
+-rw-r--r--  2.0 unx     4648 b- defN 23-Jul-25 09:06 dlrover/python/tests/test_elastic_training_agent.py
+-rw-r--r--  2.0 unx     3359 b- defN 23-May-08 02:53 dlrover/python/tests/test_elasticjob_scaler.py
+-rw-r--r--  2.0 unx      978 b- defN 23-Jul-07 03:22 dlrover/python/tests/test_grpc_utils.py
+-rw-r--r--  2.0 unx     3617 b- defN 23-Jul-25 09:06 dlrover/python/tests/test_job_auto_scaler.py
+-rw-r--r--  2.0 unx    14675 b- defN 23-Jul-25 09:06 dlrover/python/tests/test_job_manager.py
+-rw-r--r--  2.0 unx     2134 b- defN 23-May-08 02:53 dlrover/python/tests/test_job_params.py
+-rw-r--r--  2.0 unx     5302 b- defN 23-Mar-07 11:16 dlrover/python/tests/test_k8s_watcher.py
+-rw-r--r--  2.0 unx     9139 b- defN 23-Jul-25 09:06 dlrover/python/tests/test_local_optimizer.py
+-rw-r--r--  2.0 unx     2792 b- defN 23-May-09 06:52 dlrover/python/tests/test_master.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/tests/test_node_watcher.py
+-rw-r--r--  2.0 unx     7346 b- defN 23-Jul-07 03:22 dlrover/python/tests/test_pod_scaler.py
+-rw-r--r--  2.0 unx     7402 b- defN 23-May-08 02:53 dlrover/python/tests/test_ps_manager.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/tests/test_ray_client.py
+-rw-r--r--  2.0 unx     1837 b- defN 23-May-08 02:53 dlrover/python/tests/test_ray_job_args.py
+-rw-r--r--  2.0 unx      970 b- defN 23-Mar-07 11:16 dlrover/python/tests/test_ray_scaler.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/tests/test_ray_watcher.py
+-rw-r--r--  2.0 unx     7095 b- defN 23-Jul-25 09:06 dlrover/python/tests/test_rdzv_manager.py
+-rw-r--r--  2.0 unx    10021 b- defN 23-Jul-25 09:06 dlrover/python/tests/test_resource_optimizer.py
+-rw-r--r--  2.0 unx     9209 b- defN 23-Jul-25 09:06 dlrover/python/tests/test_servicer.py
+-rw-r--r--  2.0 unx     2552 b- defN 23-Jun-16 02:37 dlrover/python/tests/test_sharding_client.py
+-rw-r--r--  2.0 unx     1782 b- defN 23-Jun-16 02:37 dlrover/python/tests/test_speed_monitor.py
+-rw-r--r--  2.0 unx     1344 b- defN 23-Mar-07 11:16 dlrover/python/tests/test_state_backend.py
+-rw-r--r--  2.0 unx     3268 b- defN 23-May-08 02:53 dlrover/python/tests/test_stats_collector.py
+-rw-r--r--  2.0 unx     2455 b- defN 23-May-08 02:53 dlrover/python/tests/test_sync_service.py
+-rw-r--r--  2.0 unx     4416 b- defN 23-May-08 02:53 dlrover/python/tests/test_task_manager.py
+-rw-r--r--  2.0 unx     7667 b- defN 23-Jul-25 09:06 dlrover/python/tests/test_utils.py
+-rw-r--r--  2.0 unx     6132 b- defN 23-Jul-25 09:06 dlrover/python/tests/test_worker_manager.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/util/__init__.py
+-rw-r--r--  2.0 unx     3856 b- defN 23-Mar-07 11:16 dlrover/python/util/reflect_util.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/util/actor_util/__init__.py
+-rw-r--r--  2.0 unx     1552 b- defN 23-Mar-07 11:16 dlrover/python/util/actor_util/parse_actor.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/util/queue/__init__.py
+-rw-r--r--  2.0 unx     2834 b- defN 23-Mar-07 11:16 dlrover/python/util/queue/queue.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/python/util/state/__init__.py
+-rw-r--r--  2.0 unx     2322 b- defN 23-Mar-07 11:16 dlrover/python/util/state/memory_store.py
+-rw-r--r--  2.0 unx     1593 b- defN 23-Mar-07 11:16 dlrover/python/util/state/stats_backend.py
+-rw-r--r--  2.0 unx     2654 b- defN 23-Mar-07 11:16 dlrover/python/util/state/store_mananger.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/trainer/__init__.py
+-rw-r--r--  2.0 unx      778 b- defN 23-Mar-07 11:16 dlrover/trainer/__main__.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/trainer/constants/__init__.py
+-rw-r--r--  2.0 unx     1090 b- defN 23-Mar-07 11:16 dlrover/trainer/constants/constants.py
+-rw-r--r--  2.0 unx      989 b- defN 23-Mar-07 11:16 dlrover/trainer/constants/platform_constants.py
+-rw-r--r--  2.0 unx     3350 b- defN 23-Jun-16 02:37 dlrover/trainer/constants/tf_constants.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/trainer/entry/__init__.py
+-rw-r--r--  2.0 unx      967 b- defN 23-Mar-07 11:16 dlrover/trainer/entry/local_entry.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/trainer/mock/__init__.py
+-rw-r--r--  2.0 unx     4086 b- defN 23-Mar-07 11:16 dlrover/trainer/mock/base_process_scheduler.py
+-rw-r--r--  2.0 unx     6917 b- defN 23-May-08 02:53 dlrover/trainer/mock/tf_process_scheduler.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/trainer/platform/__init__.py
+-rw-r--r--  2.0 unx     3422 b- defN 23-May-08 02:53 dlrover/trainer/platform/starter.py
+-rw-r--r--  2.0 unx      666 b- defN 23-May-08 02:53 dlrover/trainer/tensorflow/__init__.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/trainer/tensorflow/executor/__init__.py
+-rw-r--r--  2.0 unx     7127 b- defN 23-May-08 02:53 dlrover/trainer/tensorflow/executor/base_executor.py
+-rw-r--r--  2.0 unx    10386 b- defN 23-Jun-16 02:37 dlrover/trainer/tensorflow/executor/estimator_executor.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/trainer/tensorflow/failover/__init__.py
+-rw-r--r--  2.0 unx     4312 b- defN 23-Jun-16 02:37 dlrover/trainer/tensorflow/failover/failover_client.py
+-rw-r--r--  2.0 unx     6111 b- defN 23-Jun-16 02:37 dlrover/trainer/tensorflow/failover/tensorflow_failover.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/trainer/tensorflow/hooks/__init__.py
+-rw-r--r--  2.0 unx     1151 b- defN 23-Mar-07 11:16 dlrover/trainer/tensorflow/hooks/elastic_data_shard_report_hook.py
+-rw-r--r--  2.0 unx     1611 b- defN 23-Mar-07 11:16 dlrover/trainer/tensorflow/hooks/global_step_hook.py
+-rw-r--r--  2.0 unx      691 b- defN 23-May-08 02:53 dlrover/trainer/tensorflow/reader/__init__.py
+-rw-r--r--  2.0 unx     3109 b- defN 23-May-08 02:53 dlrover/trainer/tensorflow/reader/base_reader.py
+-rw-r--r--  2.0 unx     1592 b- defN 23-Jun-16 02:37 dlrover/trainer/tensorflow/reader/file_reader.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/trainer/tensorflow/util/__init__.py
+-rw-r--r--  2.0 unx     1805 b- defN 23-Mar-07 11:16 dlrover/trainer/tensorflow/util/column_info.py
+-rw-r--r--  2.0 unx     3666 b- defN 23-Mar-07 11:16 dlrover/trainer/tensorflow/util/common_util.py
+-rw-r--r--  2.0 unx     1061 b- defN 23-Mar-07 11:16 dlrover/trainer/tensorflow/util/data_mapping_util.py
+-rw-r--r--  2.0 unx     5429 b- defN 23-May-08 02:53 dlrover/trainer/tensorflow/util/dataset_util.py
+-rw-r--r--  2.0 unx     8506 b- defN 23-Jun-16 02:37 dlrover/trainer/tensorflow/util/estimator_util.py
+-rw-r--r--  2.0 unx     1122 b- defN 23-Mar-07 11:16 dlrover/trainer/tensorflow/util/path_util.py
+-rw-r--r--  2.0 unx     1598 b- defN 23-May-08 02:53 dlrover/trainer/tensorflow/util/tf_env_util.py
+-rw-r--r--  2.0 unx    15226 b- defN 23-Jun-16 02:37 dlrover/trainer/tensorflow/util/tf_patch_util.py
+-rw-r--r--  2.0 unx     1104 b- defN 23-Mar-07 11:16 dlrover/trainer/tensorflow/util/tf_version_util.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Jun-30 07:14 dlrover/trainer/torch/__init__.py
+-rw-r--r--  2.0 unx     9587 b- defN 23-Jul-07 03:22 dlrover/trainer/torch/elastic.py
+-rw-r--r--  2.0 unx     3815 b- defN 23-Jun-30 07:14 dlrover/trainer/torch/elastic_dataset.py
+-rw-r--r--  2.0 unx     3705 b- defN 23-Jul-25 09:06 dlrover/trainer/torch/elastic_run.py
+-rw-r--r--  2.0 unx     4197 b- defN 23-Jun-30 07:14 dlrover/trainer/torch/elastic_sampler.py
+-rw-r--r--  2.0 unx      690 b- defN 23-Jul-07 03:22 dlrover/trainer/torch/main.py
+-rw-r--r--  2.0 unx     1700 b- defN 23-Jul-25 09:06 dlrover/trainer/torch/run_network_check.py
+-rw-r--r--  2.0 unx      741 b- defN 23-Jun-30 07:14 dlrover/trainer/torch/utils.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/trainer/util/__init__.py
+-rw-r--r--  2.0 unx     2031 b- defN 23-Mar-07 11:16 dlrover/trainer/util/args_util.py
+-rw-r--r--  2.0 unx     6436 b- defN 23-Mar-07 11:16 dlrover/trainer/util/conf_util.py
+-rw-r--r--  2.0 unx     2863 b- defN 23-Mar-07 11:16 dlrover/trainer/util/log_util.py
+-rw-r--r--  2.0 unx      736 b- defN 23-Mar-07 11:16 dlrover/trainer/util/net_util.py
+-rw-r--r--  2.0 unx     3860 b- defN 23-Mar-07 11:16 dlrover/trainer/util/reflect_util.py
+-rw-r--r--  2.0 unx      599 b- defN 23-Mar-07 11:16 dlrover/trainer/worker/__init__.py
+-rw-r--r--  2.0 unx     3540 b- defN 23-Jun-16 02:37 dlrover/trainer/worker/tf_kubernetes_worker.py
+-rw-r--r--  2.0 unx     6932 b- defN 23-Mar-07 11:16 dlrover/trainer/worker/tf_ray_worker.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-25 09:09 dlrover-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      956 b- defN 23-Jul-25 09:09 dlrover-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 09:09 dlrover-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       64 b- defN 23-Jul-25 09:09 dlrover-0.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-25 09:09 dlrover-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    18594 b- defN 23-Jul-25 09:09 dlrover-0.2.0.dist-info/RECORD
+191 files, 1100464 bytes uncompressed, 268740 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -1,16 +1,13 @@
 Filename: dlrover/Makefile
 Comment: 
 
 Filename: dlrover/__init__.py
 Comment: 
 
-Filename: dlrover/requirements.txt
-Comment: 
-
 Filename: dlrover/proto/brain.proto
 Comment: 
 
 Filename: dlrover/proto/brain_pb2.py
 Comment: 
 
 Filename: dlrover/proto/brain_pb2_grpc.py
@@ -75,26 +72,41 @@
 
 Filename: dlrover/python/elastic_agent/sharding/__init__.py
 Comment: 
 
 Filename: dlrover/python/elastic_agent/sharding/client.py
 Comment: 
 
+Filename: dlrover/python/elastic_agent/sychronization/__init__.py
+Comment: 
+
+Filename: dlrover/python/elastic_agent/sychronization/sync_client.py
+Comment: 
+
 Filename: dlrover/python/elastic_agent/tensorflow/__init__.py
 Comment: 
 
 Filename: dlrover/python/elastic_agent/tensorflow/elastic_ps.py
 Comment: 
 
 Filename: dlrover/python/elastic_agent/tensorflow/hooks.py
 Comment: 
 
 Filename: dlrover/python/elastic_agent/tensorflow/profile_extractor.py
 Comment: 
 
+Filename: dlrover/python/elastic_agent/torch/__init__.py
+Comment: 
+
+Filename: dlrover/python/elastic_agent/torch/master_kv_store.py
+Comment: 
+
+Filename: dlrover/python/elastic_agent/torch/training.py
+Comment: 
+
 Filename: dlrover/python/master/__init__.py
 Comment: 
 
 Filename: dlrover/python/master/args.py
 Comment: 
 
 Filename: dlrover/python/master/main.py
@@ -102,33 +114,54 @@
 
 Filename: dlrover/python/master/master.py
 Comment: 
 
 Filename: dlrover/python/master/servicer.py
 Comment: 
 
+Filename: dlrover/python/master/cluster/__init__.py
+Comment: 
+
+Filename: dlrover/python/master/cluster/quota.py
+Comment: 
+
 Filename: dlrover/python/master/elastic_training/__init__.py
 Comment: 
 
 Filename: dlrover/python/master/elastic_training/elastic_ps.py
 Comment: 
 
+Filename: dlrover/python/master/elastic_training/kv_store_service.py
+Comment: 
+
+Filename: dlrover/python/master/elastic_training/rdzv_manager.py
+Comment: 
+
+Filename: dlrover/python/master/elastic_training/sync_service.py
+Comment: 
+
 Filename: dlrover/python/master/monitor/__init__.py
 Comment: 
 
+Filename: dlrover/python/master/monitor/error_monitor.py
+Comment: 
+
 Filename: dlrover/python/master/monitor/speed_monitor.py
 Comment: 
 
 Filename: dlrover/python/master/node/__init__.py
 Comment: 
 
 Filename: dlrover/python/master/node/event_callback.py
 Comment: 
 
-Filename: dlrover/python/master/node/node_manager.py
+Filename: dlrover/python/master/node/job_auto_scaler.py
+Comment: 
+
+Filename: dlrover/python/master/node/job_manager.py
 Comment: 
 
 Filename: dlrover/python/master/node/ps.py
 Comment: 
 
 Filename: dlrover/python/master/node/status_flow.py
 Comment: 
@@ -165,14 +198,17 @@
 
 Filename: dlrover/python/master/scaler/factory.py
 Comment: 
 
 Filename: dlrover/python/master/scaler/pod_scaler.py
 Comment: 
 
+Filename: dlrover/python/master/scaler/ray_scaler.py
+Comment: 
+
 Filename: dlrover/python/master/shard/__init__.py
 Comment: 
 
 Filename: dlrover/python/master/shard/base_dataset_manager.py
 Comment: 
 
 Filename: dlrover/python/master/shard/batch_dataset_manager.py
@@ -192,41 +228,50 @@
 
 Filename: dlrover/python/master/stats/job_collector.py
 Comment: 
 
 Filename: dlrover/python/master/stats/reporter.py
 Comment: 
 
+Filename: dlrover/python/master/stats/stats_backend.py
+Comment: 
+
 Filename: dlrover/python/master/stats/training_metrics.py
 Comment: 
 
 Filename: dlrover/python/master/watcher/__init__.py
 Comment: 
 
 Filename: dlrover/python/master/watcher/base_watcher.py
 Comment: 
 
 Filename: dlrover/python/master/watcher/factory.py
 Comment: 
 
-Filename: dlrover/python/master/watcher/pod_watcher.py
+Filename: dlrover/python/master/watcher/k8s_watcher.py
+Comment: 
+
+Filename: dlrover/python/master/watcher/ray_watcher.py
 Comment: 
 
 Filename: dlrover/python/scheduler/__init__.py
 Comment: 
 
 Filename: dlrover/python/scheduler/factory.py
 Comment: 
 
 Filename: dlrover/python/scheduler/job.py
 Comment: 
 
 Filename: dlrover/python/scheduler/kubernetes.py
 Comment: 
 
+Filename: dlrover/python/scheduler/ray.py
+Comment: 
+
 Filename: dlrover/python/tests/__init__.py
 Comment: 
 
 Filename: dlrover/python/tests/test_agent_monitor.py
 Comment: 
 
 Filename: dlrover/python/tests/test_args.py
@@ -234,99 +279,147 @@
 
 Filename: dlrover/python/tests/test_dataset_splitter.py
 Comment: 
 
 Filename: dlrover/python/tests/test_dataset_task_manager.py
 Comment: 
 
+Filename: dlrover/python/tests/test_elastic_training_agent.py
+Comment: 
+
+Filename: dlrover/python/tests/test_elasticjob_scaler.py
+Comment: 
+
+Filename: dlrover/python/tests/test_grpc_utils.py
+Comment: 
+
+Filename: dlrover/python/tests/test_job_auto_scaler.py
+Comment: 
+
+Filename: dlrover/python/tests/test_job_manager.py
+Comment: 
+
 Filename: dlrover/python/tests/test_job_params.py
 Comment: 
 
-Filename: dlrover/python/tests/test_k8s_scaler.py
+Filename: dlrover/python/tests/test_k8s_watcher.py
 Comment: 
 
 Filename: dlrover/python/tests/test_local_optimizer.py
 Comment: 
 
 Filename: dlrover/python/tests/test_master.py
 Comment: 
 
-Filename: dlrover/python/tests/test_node_manager.py
-Comment: 
-
 Filename: dlrover/python/tests/test_node_watcher.py
 Comment: 
 
 Filename: dlrover/python/tests/test_pod_scaler.py
 Comment: 
 
-Filename: dlrover/python/tests/test_pod_watcher.py
+Filename: dlrover/python/tests/test_ps_manager.py
 Comment: 
 
-Filename: dlrover/python/tests/test_ps_manager.py
+Filename: dlrover/python/tests/test_ray_client.py
+Comment: 
+
+Filename: dlrover/python/tests/test_ray_job_args.py
+Comment: 
+
+Filename: dlrover/python/tests/test_ray_scaler.py
+Comment: 
+
+Filename: dlrover/python/tests/test_ray_watcher.py
+Comment: 
+
+Filename: dlrover/python/tests/test_rdzv_manager.py
 Comment: 
 
 Filename: dlrover/python/tests/test_resource_optimizer.py
 Comment: 
 
 Filename: dlrover/python/tests/test_servicer.py
 Comment: 
 
 Filename: dlrover/python/tests/test_sharding_client.py
 Comment: 
 
 Filename: dlrover/python/tests/test_speed_monitor.py
 Comment: 
 
+Filename: dlrover/python/tests/test_state_backend.py
+Comment: 
+
 Filename: dlrover/python/tests/test_stats_collector.py
 Comment: 
 
+Filename: dlrover/python/tests/test_sync_service.py
+Comment: 
+
 Filename: dlrover/python/tests/test_task_manager.py
 Comment: 
 
 Filename: dlrover/python/tests/test_utils.py
 Comment: 
 
 Filename: dlrover/python/tests/test_worker_manager.py
 Comment: 
 
-Filename: dlrover/trainer/__init__.py
+Filename: dlrover/python/util/__init__.py
 Comment: 
 
-Filename: dlrover/trainer/__main__.py
+Filename: dlrover/python/util/reflect_util.py
 Comment: 
 
-Filename: dlrover/trainer/constants/__init__.py
+Filename: dlrover/python/util/actor_util/__init__.py
 Comment: 
 
-Filename: dlrover/trainer/constants/constants.py
+Filename: dlrover/python/util/actor_util/parse_actor.py
 Comment: 
 
-Filename: dlrover/trainer/constants/platform_constants.py
+Filename: dlrover/python/util/queue/__init__.py
 Comment: 
 
-Filename: dlrover/trainer/constants/tf_constants.py
+Filename: dlrover/python/util/queue/queue.py
 Comment: 
 
-Filename: dlrover/trainer/entry/__init__.py
+Filename: dlrover/python/util/state/__init__.py
 Comment: 
 
-Filename: dlrover/trainer/entry/local_entry.py
+Filename: dlrover/python/util/state/memory_store.py
+Comment: 
+
+Filename: dlrover/python/util/state/stats_backend.py
+Comment: 
+
+Filename: dlrover/python/util/state/store_mananger.py
+Comment: 
+
+Filename: dlrover/trainer/__init__.py
+Comment: 
+
+Filename: dlrover/trainer/__main__.py
 Comment: 
 
-Filename: dlrover/trainer/examples/__init__.py
+Filename: dlrover/trainer/constants/__init__.py
 Comment: 
 
-Filename: dlrover/trainer/examples/estimator_executor/MyEstimator.py
+Filename: dlrover/trainer/constants/constants.py
 Comment: 
 
-Filename: dlrover/trainer/examples/estimator_executor/__init__.py
+Filename: dlrover/trainer/constants/platform_constants.py
 Comment: 
 
-Filename: dlrover/trainer/examples/estimator_executor/conf.py
+Filename: dlrover/trainer/constants/tf_constants.py
+Comment: 
+
+Filename: dlrover/trainer/entry/__init__.py
+Comment: 
+
+Filename: dlrover/trainer/entry/local_entry.py
 Comment: 
 
 Filename: dlrover/trainer/mock/__init__.py
 Comment: 
 
 Filename: dlrover/trainer/mock/base_process_scheduler.py
 Comment: 
@@ -369,15 +462,15 @@
 
 Filename: dlrover/trainer/tensorflow/hooks/global_step_hook.py
 Comment: 
 
 Filename: dlrover/trainer/tensorflow/reader/__init__.py
 Comment: 
 
-Filename: dlrover/trainer/tensorflow/reader/fake_reader.py
+Filename: dlrover/trainer/tensorflow/reader/base_reader.py
 Comment: 
 
 Filename: dlrover/trainer/tensorflow/reader/file_reader.py
 Comment: 
 
 Filename: dlrover/trainer/tensorflow/util/__init__.py
 Comment: 
@@ -396,20 +489,47 @@
 
 Filename: dlrover/trainer/tensorflow/util/estimator_util.py
 Comment: 
 
 Filename: dlrover/trainer/tensorflow/util/path_util.py
 Comment: 
 
+Filename: dlrover/trainer/tensorflow/util/tf_env_util.py
+Comment: 
+
 Filename: dlrover/trainer/tensorflow/util/tf_patch_util.py
 Comment: 
 
 Filename: dlrover/trainer/tensorflow/util/tf_version_util.py
 Comment: 
 
+Filename: dlrover/trainer/torch/__init__.py
+Comment: 
+
+Filename: dlrover/trainer/torch/elastic.py
+Comment: 
+
+Filename: dlrover/trainer/torch/elastic_dataset.py
+Comment: 
+
+Filename: dlrover/trainer/torch/elastic_run.py
+Comment: 
+
+Filename: dlrover/trainer/torch/elastic_sampler.py
+Comment: 
+
+Filename: dlrover/trainer/torch/main.py
+Comment: 
+
+Filename: dlrover/trainer/torch/run_network_check.py
+Comment: 
+
+Filename: dlrover/trainer/torch/utils.py
+Comment: 
+
 Filename: dlrover/trainer/util/__init__.py
 Comment: 
 
 Filename: dlrover/trainer/util/args_util.py
 Comment: 
 
 Filename: dlrover/trainer/util/conf_util.py
@@ -426,23 +546,29 @@
 
 Filename: dlrover/trainer/worker/__init__.py
 Comment: 
 
 Filename: dlrover/trainer/worker/tf_kubernetes_worker.py
 Comment: 
 
-Filename: dlrover-0.1.0rc0.dev1.dist-info/LICENSE
+Filename: dlrover/trainer/worker/tf_ray_worker.py
+Comment: 
+
+Filename: dlrover-0.2.0.dist-info/LICENSE
+Comment: 
+
+Filename: dlrover-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: dlrover-0.1.0rc0.dev1.dist-info/METADATA
+Filename: dlrover-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: dlrover-0.1.0rc0.dev1.dist-info/WHEEL
+Filename: dlrover-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: dlrover-0.1.0rc0.dev1.dist-info/top_level.txt
+Filename: dlrover-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dlrover-0.1.0rc0.dev1.dist-info/RECORD
+Filename: dlrover-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dlrover/proto/brain.proto

```diff
@@ -86,15 +86,15 @@
   Type = 7;
   Resource = 8;
   Customized_Data = 9;
   Optimization = 10;
 }
 
 message JobMetrics {
-  string data_store = 1; // data_store_elasticdl
+  string data_store = 1;
   JobMeta job_meta = 2;
   MetricsType metrics_type = 3;
   oneof metrics {
     TrainingHyperParams training_hyper_params = 4;
     WorkflowFeature workflow_feature = 5;
     TrainingSetFeature training_set_feature = 6;
     ModelFeature model_feature = 7;
@@ -146,14 +146,15 @@
 }
 
 message PodResource {
   int64 memory = 1; // unit MB
   float cpu = 2;    // The number of cores
   float gpu = 3;
   string gpu_type = 4;
+  string priority = 5;
 }
 
 message TaskGroupResource {
   int64 count = 1;
   PodResource resource = 2;
 }
```

## dlrover/proto/brain_pb2.py

```diff
@@ -1,71 +1,1786 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: dlrover/proto/brain.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19\x64lrover/proto/brain.proto\x12\x05\x62rain\x1a\x1bgoogle/protobuf/empty.proto\"K\n\x13TrainingHyperParams\x12\x12\n\nbatch_size\x18\x01 \x01(\x03\x12\r\n\x05\x65poch\x18\x02 \x01(\x03\x12\x11\n\tmax_steps\x18\x03 \x01(\x03\"\x97\x01\n\x0fWorkflowFeature\x12\x10\n\x08job_name\x18\x01 \x01(\t\x12\x0f\n\x07user_id\x18\x02 \x01(\t\x12\x14\n\x0c\x63ode_address\x18\x03 \x01(\t\x12\x13\n\x0bworkflow_id\x18\x04 \x01(\t\x12\x0f\n\x07node_id\x18\x05 \x01(\t\x12\x14\n\x0codps_project\x18\x06 \x01(\t\x12\x0f\n\x07is_prod\x18\x07 \x01(\x08\"\xfe\x01\n\x12TrainingSetFeature\x12\x14\n\x0c\x64\x61taset_size\x18\x01 \x01(\x03\x12\x14\n\x0c\x64\x61taset_name\x18\x02 \x01(\t\x12\x19\n\x11sparse_item_count\x18\x03 \x01(\x03\x12\x17\n\x0fsparse_features\x18\x04 \x01(\t\x12\x1d\n\x15sparse_feature_groups\x18\x05 \x01(\t\x12\x1d\n\x15sparse_feature_shapes\x18\x06 \x01(\t\x12\x16\n\x0e\x64\x65nse_features\x18\x07 \x01(\t\x12\x1c\n\x14\x64\x65nse_feature_shapes\x18\x08 \x01(\t\x12\x14\n\x0cstorage_size\x18\t \x01(\x03\"\x97\x03\n\x0cModelFeature\x12\x16\n\x0evariable_count\x18\x01 \x01(\x03\x12\x10\n\x08op_count\x18\x02 \x01(\x03\x12\x1b\n\x13\x65mbedding_dimension\x18\x03 \x01(\x03\x12\x1b\n\x13total_variable_size\x18\x04 \x01(\x03\x12\x19\n\x11max_variable_size\x18\x05 \x01(\x03\x12\x17\n\x0fupdate_op_count\x18\x06 \x01(\x03\x12\x15\n\rread_op_count\x18\x07 \x01(\x03\x12\x17\n\x0finput_fetch_dur\x18\x08 \x01(\x03\x12\r\n\x05\x66lops\x18\t \x01(\x03\x12\x15\n\rrecv_op_count\x18\n \x01(\x03\x12\x19\n\x11kv_embedding_dims\x18\x0b \x03(\x03\x12\x45\n\x12tensor_alloc_bytes\x18\x0c \x03(\x0b\x32).brain.ModelFeature.TensorAllocBytesEntry\x1a\x37\n\x15TensorAllocBytesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x03:\x02\x38\x01\"k\n\x0bRuntimeInfo\x12\x13\n\x0bglobal_step\x18\x01 \x01(\x03\x12$\n\x0crunning_pods\x18\x02 \x03(\x0b\x32\x0e.brain.PodMeta\x12\x12\n\ntime_stamp\x18\x03 \x01(\x03\x12\r\n\x05speed\x18\x04 \x01(\x02\"\x9a\x01\n\x07PodMeta\x12\x10\n\x08pod_name\x18\x01 \x01(\t\x12\x0e\n\x06pod_ip\x18\x02 \x01(\t\x12\x0f\n\x07node_ip\x18\x03 \x01(\t\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x11\n\tnamespace\x18\x05 \x01(\t\x12\x10\n\x08is_mixed\x18\x06 \x01(\x08\x12\x11\n\tmem_usage\x18\x07 \x01(\x01\x12\x11\n\tcpu_usage\x18\x08 \x01(\x01\"W\n\x07JobMeta\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04user\x18\x03 \x01(\t\x12\x0f\n\x07\x63luster\x18\x04 \x01(\t\x12\x11\n\tnamespace\x18\x05 \x01(\t\"\xa1\x04\n\nJobMetrics\x12\x12\n\ndata_store\x18\x01 \x01(\t\x12 \n\x08job_meta\x18\x02 \x01(\x0b\x32\x0e.brain.JobMeta\x12(\n\x0cmetrics_type\x18\x03 \x01(\x0e\x32\x12.brain.MetricsType\x12;\n\x15training_hyper_params\x18\x04 \x01(\x0b\x32\x1a.brain.TrainingHyperParamsH\x00\x12\x32\n\x10workflow_feature\x18\x05 \x01(\x0b\x32\x16.brain.WorkflowFeatureH\x00\x12\x39\n\x14training_set_feature\x18\x06 \x01(\x0b\x32\x19.brain.TrainingSetFeatureH\x00\x12,\n\rmodel_feature\x18\x07 \x01(\x0b\x32\x13.brain.ModelFeatureH\x00\x12*\n\x0cruntime_info\x18\x08 \x01(\x0b\x32\x12.brain.RuntimeInfoH\x00\x12\x19\n\x0fjob_exit_reason\x18\t \x01(\tH\x00\x12\x14\n\nextra_info\x18\n \x01(\tH\x00\x12\x0e\n\x04type\x18\x0b \x01(\tH\x00\x12\x12\n\x08resource\x18\x0c \x01(\tH\x00\x12\x19\n\x0f\x63ustomized_data\x18\r \x01(\tH\x00\x12\x32\n\x10job_optimization\x18\x0e \x01(\x0b\x32\x16.brain.JobOptimizationH\x00\x42\t\n\x07metrics\"\xe2\x01\n\x0eOptimizeConfig\x12\"\n\x1aoptimizer_config_retriever\x18\x01 \x01(\t\x12\x12\n\ndata_store\x18\x02 \x01(\t\x12\x17\n\x0f\x62rain_processor\x18\x03 \x01(\t\x12\x46\n\x11\x63ustomized_config\x18\x04 \x03(\x0b\x32+.brain.OptimizeConfig.CustomizedConfigEntry\x1a\x37\n\x15\x43ustomizedConfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x89\x02\n\x08PodState\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03uid\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0e\n\x06is_oom\x18\x04 \x01(\x08\x12$\n\x08resource\x18\x05 \x01(\x0b\x32\x12.brain.PodResource\x12)\n\rused_resource\x18\x06 \x01(\x0b\x32\x12.brain.PodResource\x12<\n\x0f\x63ustomized_data\x18\x07 \x03(\x0b\x32#.brain.PodState.CustomizedDataEntry\x1a\x35\n\x13\x43ustomizedDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x88\x02\n\x08JobState\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\'\n\x04pods\x18\x02 \x03(\x0b\x32\x19.brain.JobState.PodsEntry\x12\r\n\x05speed\x18\x03 \x01(\x02\x12<\n\x0f\x63ustomized_data\x18\x04 \x03(\x0b\x32#.brain.JobState.CustomizedDataEntry\x1a<\n\tPodsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.brain.PodState:\x02\x38\x01\x1a\x35\n\x13\x43ustomizedDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"b\n\x0fOptimizeJobMeta\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12\x0f\n\x07\x63luster\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x1e\n\x05state\x18\x04 \x01(\x0b\x32\x0f.brain.JobState\"l\n\x0fOptimizeRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12%\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x15.brain.OptimizeConfig\x12$\n\x04jobs\x18\x03 \x03(\x0b\x32\x16.brain.OptimizeJobMeta\"I\n\x0bPodResource\x12\x0e\n\x06memory\x18\x01 \x01(\x03\x12\x0b\n\x03\x63pu\x18\x02 \x01(\x02\x12\x0b\n\x03gpu\x18\x03 \x01(\x02\x12\x10\n\x08gpu_type\x18\x04 \x01(\t\"H\n\x11TaskGroupResource\x12\r\n\x05\x63ount\x18\x01 \x01(\x03\x12$\n\x08resource\x18\x02 \x01(\x0b\x32\x12.brain.PodResource\"\xb2\x02\n\x0bJobResource\x12H\n\x14task_group_resources\x18\x01 \x03(\x0b\x32*.brain.JobResource.TaskGroupResourcesEntry\x12;\n\rpod_resources\x18\x02 \x03(\x0b\x32$.brain.JobResource.PodResourcesEntry\x1aS\n\x17TaskGroupResourcesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x18.brain.TaskGroupResource:\x02\x38\x01\x1aG\n\x11PodResourcesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.brain.PodResource:\x02\x38\x01\"o\n\x0fJobOptimizePlan\x12\x11\n\ttimestamp\x18\x01 \x01(\x04\x12$\n\x08resource\x18\x02 \x01(\x0b\x32\x12.brain.JobResource\x12#\n\x03job\x18\x03 \x01(\x0b\x32\x16.brain.OptimizeJobMeta\"\x96\x01\n\x0fJobOptimization\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12%\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x15.brain.OptimizeConfig\x12$\n\x04plan\x18\x03 \x01(\x0b\x32\x16.brain.JobOptimizePlan\x12#\n\njob_states\x18\x04 \x03(\x0b\x32\x0f.brain.JobState\"+\n\x08Response\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x0e\n\x06reason\x18\x02 \x01(\t\"i\n\x10OptimizeResponse\x12!\n\x08response\x18\x01 \x01(\x0b\x32\x0f.brain.Response\x12\x32\n\x12job_optimize_plans\x18\x02 \x03(\x0b\x32\x16.brain.JobOptimizePlan\"%\n\x11JobMetricsRequest\x12\x10\n\x08job_uuid\x18\x01 \x01(\t\"L\n\x12JobMetricsResponse\x12!\n\x08response\x18\x01 \x01(\x0b\x32\x0f.brain.Response\x12\x13\n\x0bjob_metrics\x18\x02 \x01(\t*\xea\x01\n\x0bMetricsType\x12\x19\n\x15Training_Hyper_Params\x10\x00\x12\x14\n\x10Workflow_Feature\x10\x01\x12\x18\n\x14Training_Set_Feature\x10\x02\x12\x11\n\rModel_Feature\x10\x03\x12\x10\n\x0cRuntime_Info\x10\x04\x12\x13\n\x0fJob_Exit_Reason\x10\x05\x12\x17\n\x13Optimization_Result\x10\x06\x12\x08\n\x04Type\x10\x07\x12\x0c\n\x08Resource\x10\x08\x12\x13\n\x0f\x43ustomized_Data\x10\t\x12\x10\n\x0cOptimization\x10\n2\xca\x01\n\x05\x42rain\x12<\n\x0fpersist_metrics\x12\x11.brain.JobMetrics\x1a\x16.google.protobuf.Empty\x12;\n\x08optimize\x12\x16.brain.OptimizeRequest\x1a\x17.brain.OptimizeResponse\x12\x46\n\x0fget_job_metrics\x12\x18.brain.JobMetricsRequest\x1a\x19.brain.JobMetricsResponseB\x1cZ\x1a\x64lrover/go/brain/pkg/protob\x06proto3')
+DESCRIPTOR = _descriptor.FileDescriptor(
+  name='dlrover/proto/brain.proto',
+  package='brain',
+  syntax='proto3',
+  serialized_options=b'Z\032dlrover/go/brain/pkg/proto',
+  create_key=_descriptor._internal_create_key,
+  serialized_pb=b'\n\x19\x64lrover/proto/brain.proto\x12\x05\x62rain\x1a\x1bgoogle/protobuf/empty.proto\"K\n\x13TrainingHyperParams\x12\x12\n\nbatch_size\x18\x01 \x01(\x03\x12\r\n\x05\x65poch\x18\x02 \x01(\x03\x12\x11\n\tmax_steps\x18\x03 \x01(\x03\"\x97\x01\n\x0fWorkflowFeature\x12\x10\n\x08job_name\x18\x01 \x01(\t\x12\x0f\n\x07user_id\x18\x02 \x01(\t\x12\x14\n\x0c\x63ode_address\x18\x03 \x01(\t\x12\x13\n\x0bworkflow_id\x18\x04 \x01(\t\x12\x0f\n\x07node_id\x18\x05 \x01(\t\x12\x14\n\x0codps_project\x18\x06 \x01(\t\x12\x0f\n\x07is_prod\x18\x07 \x01(\x08\"\xfe\x01\n\x12TrainingSetFeature\x12\x14\n\x0c\x64\x61taset_size\x18\x01 \x01(\x03\x12\x14\n\x0c\x64\x61taset_name\x18\x02 \x01(\t\x12\x19\n\x11sparse_item_count\x18\x03 \x01(\x03\x12\x17\n\x0fsparse_features\x18\x04 \x01(\t\x12\x1d\n\x15sparse_feature_groups\x18\x05 \x01(\t\x12\x1d\n\x15sparse_feature_shapes\x18\x06 \x01(\t\x12\x16\n\x0e\x64\x65nse_features\x18\x07 \x01(\t\x12\x1c\n\x14\x64\x65nse_feature_shapes\x18\x08 \x01(\t\x12\x14\n\x0cstorage_size\x18\t \x01(\x03\"\x97\x03\n\x0cModelFeature\x12\x16\n\x0evariable_count\x18\x01 \x01(\x03\x12\x10\n\x08op_count\x18\x02 \x01(\x03\x12\x1b\n\x13\x65mbedding_dimension\x18\x03 \x01(\x03\x12\x1b\n\x13total_variable_size\x18\x04 \x01(\x03\x12\x19\n\x11max_variable_size\x18\x05 \x01(\x03\x12\x17\n\x0fupdate_op_count\x18\x06 \x01(\x03\x12\x15\n\rread_op_count\x18\x07 \x01(\x03\x12\x17\n\x0finput_fetch_dur\x18\x08 \x01(\x03\x12\r\n\x05\x66lops\x18\t \x01(\x03\x12\x15\n\rrecv_op_count\x18\n \x01(\x03\x12\x19\n\x11kv_embedding_dims\x18\x0b \x03(\x03\x12\x45\n\x12tensor_alloc_bytes\x18\x0c \x03(\x0b\x32).brain.ModelFeature.TensorAllocBytesEntry\x1a\x37\n\x15TensorAllocBytesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x03:\x02\x38\x01\"k\n\x0bRuntimeInfo\x12\x13\n\x0bglobal_step\x18\x01 \x01(\x03\x12$\n\x0crunning_pods\x18\x02 \x03(\x0b\x32\x0e.brain.PodMeta\x12\x12\n\ntime_stamp\x18\x03 \x01(\x03\x12\r\n\x05speed\x18\x04 \x01(\x02\"\x9a\x01\n\x07PodMeta\x12\x10\n\x08pod_name\x18\x01 \x01(\t\x12\x0e\n\x06pod_ip\x18\x02 \x01(\t\x12\x0f\n\x07node_ip\x18\x03 \x01(\t\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x11\n\tnamespace\x18\x05 \x01(\t\x12\x10\n\x08is_mixed\x18\x06 \x01(\x08\x12\x11\n\tmem_usage\x18\x07 \x01(\x01\x12\x11\n\tcpu_usage\x18\x08 \x01(\x01\"W\n\x07JobMeta\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04user\x18\x03 \x01(\t\x12\x0f\n\x07\x63luster\x18\x04 \x01(\t\x12\x11\n\tnamespace\x18\x05 \x01(\t\"\xa1\x04\n\nJobMetrics\x12\x12\n\ndata_store\x18\x01 \x01(\t\x12 \n\x08job_meta\x18\x02 \x01(\x0b\x32\x0e.brain.JobMeta\x12(\n\x0cmetrics_type\x18\x03 \x01(\x0e\x32\x12.brain.MetricsType\x12;\n\x15training_hyper_params\x18\x04 \x01(\x0b\x32\x1a.brain.TrainingHyperParamsH\x00\x12\x32\n\x10workflow_feature\x18\x05 \x01(\x0b\x32\x16.brain.WorkflowFeatureH\x00\x12\x39\n\x14training_set_feature\x18\x06 \x01(\x0b\x32\x19.brain.TrainingSetFeatureH\x00\x12,\n\rmodel_feature\x18\x07 \x01(\x0b\x32\x13.brain.ModelFeatureH\x00\x12*\n\x0cruntime_info\x18\x08 \x01(\x0b\x32\x12.brain.RuntimeInfoH\x00\x12\x19\n\x0fjob_exit_reason\x18\t \x01(\tH\x00\x12\x14\n\nextra_info\x18\n \x01(\tH\x00\x12\x0e\n\x04type\x18\x0b \x01(\tH\x00\x12\x12\n\x08resource\x18\x0c \x01(\tH\x00\x12\x19\n\x0f\x63ustomized_data\x18\r \x01(\tH\x00\x12\x32\n\x10job_optimization\x18\x0e \x01(\x0b\x32\x16.brain.JobOptimizationH\x00\x42\t\n\x07metrics\"\xe2\x01\n\x0eOptimizeConfig\x12\"\n\x1aoptimizer_config_retriever\x18\x01 \x01(\t\x12\x12\n\ndata_store\x18\x02 \x01(\t\x12\x17\n\x0f\x62rain_processor\x18\x03 \x01(\t\x12\x46\n\x11\x63ustomized_config\x18\x04 \x03(\x0b\x32+.brain.OptimizeConfig.CustomizedConfigEntry\x1a\x37\n\x15\x43ustomizedConfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x89\x02\n\x08PodState\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03uid\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0e\n\x06is_oom\x18\x04 \x01(\x08\x12$\n\x08resource\x18\x05 \x01(\x0b\x32\x12.brain.PodResource\x12)\n\rused_resource\x18\x06 \x01(\x0b\x32\x12.brain.PodResource\x12<\n\x0f\x63ustomized_data\x18\x07 \x03(\x0b\x32#.brain.PodState.CustomizedDataEntry\x1a\x35\n\x13\x43ustomizedDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x88\x02\n\x08JobState\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\'\n\x04pods\x18\x02 \x03(\x0b\x32\x19.brain.JobState.PodsEntry\x12\r\n\x05speed\x18\x03 \x01(\x02\x12<\n\x0f\x63ustomized_data\x18\x04 \x03(\x0b\x32#.brain.JobState.CustomizedDataEntry\x1a<\n\tPodsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.brain.PodState:\x02\x38\x01\x1a\x35\n\x13\x43ustomizedDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"b\n\x0fOptimizeJobMeta\x12\x0b\n\x03uid\x18\x01 \x01(\t\x12\x0f\n\x07\x63luster\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x1e\n\x05state\x18\x04 \x01(\x0b\x32\x0f.brain.JobState\"l\n\x0fOptimizeRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12%\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x15.brain.OptimizeConfig\x12$\n\x04jobs\x18\x03 \x03(\x0b\x32\x16.brain.OptimizeJobMeta\"[\n\x0bPodResource\x12\x0e\n\x06memory\x18\x01 \x01(\x03\x12\x0b\n\x03\x63pu\x18\x02 \x01(\x02\x12\x0b\n\x03gpu\x18\x03 \x01(\x02\x12\x10\n\x08gpu_type\x18\x04 \x01(\t\x12\x10\n\x08priority\x18\x05 \x01(\t\"H\n\x11TaskGroupResource\x12\r\n\x05\x63ount\x18\x01 \x01(\x03\x12$\n\x08resource\x18\x02 \x01(\x0b\x32\x12.brain.PodResource\"\xb2\x02\n\x0bJobResource\x12H\n\x14task_group_resources\x18\x01 \x03(\x0b\x32*.brain.JobResource.TaskGroupResourcesEntry\x12;\n\rpod_resources\x18\x02 \x03(\x0b\x32$.brain.JobResource.PodResourcesEntry\x1aS\n\x17TaskGroupResourcesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x18.brain.TaskGroupResource:\x02\x38\x01\x1aG\n\x11PodResourcesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.brain.PodResource:\x02\x38\x01\"o\n\x0fJobOptimizePlan\x12\x11\n\ttimestamp\x18\x01 \x01(\x04\x12$\n\x08resource\x18\x02 \x01(\x0b\x32\x12.brain.JobResource\x12#\n\x03job\x18\x03 \x01(\x0b\x32\x16.brain.OptimizeJobMeta\"\x96\x01\n\x0fJobOptimization\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12%\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x15.brain.OptimizeConfig\x12$\n\x04plan\x18\x03 \x01(\x0b\x32\x16.brain.JobOptimizePlan\x12#\n\njob_states\x18\x04 \x03(\x0b\x32\x0f.brain.JobState\"+\n\x08Response\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x0e\n\x06reason\x18\x02 \x01(\t\"i\n\x10OptimizeResponse\x12!\n\x08response\x18\x01 \x01(\x0b\x32\x0f.brain.Response\x12\x32\n\x12job_optimize_plans\x18\x02 \x03(\x0b\x32\x16.brain.JobOptimizePlan\"%\n\x11JobMetricsRequest\x12\x10\n\x08job_uuid\x18\x01 \x01(\t\"L\n\x12JobMetricsResponse\x12!\n\x08response\x18\x01 \x01(\x0b\x32\x0f.brain.Response\x12\x13\n\x0bjob_metrics\x18\x02 \x01(\t*\xea\x01\n\x0bMetricsType\x12\x19\n\x15Training_Hyper_Params\x10\x00\x12\x14\n\x10Workflow_Feature\x10\x01\x12\x18\n\x14Training_Set_Feature\x10\x02\x12\x11\n\rModel_Feature\x10\x03\x12\x10\n\x0cRuntime_Info\x10\x04\x12\x13\n\x0fJob_Exit_Reason\x10\x05\x12\x17\n\x13Optimization_Result\x10\x06\x12\x08\n\x04Type\x10\x07\x12\x0c\n\x08Resource\x10\x08\x12\x13\n\x0f\x43ustomized_Data\x10\t\x12\x10\n\x0cOptimization\x10\n2\xca\x01\n\x05\x42rain\x12<\n\x0fpersist_metrics\x12\x11.brain.JobMetrics\x1a\x16.google.protobuf.Empty\x12;\n\x08optimize\x12\x16.brain.OptimizeRequest\x1a\x17.brain.OptimizeResponse\x12\x46\n\x0fget_job_metrics\x12\x18.brain.JobMetricsRequest\x1a\x19.brain.JobMetricsResponseB\x1cZ\x1a\x64lrover/go/brain/pkg/protob\x06proto3'
+  ,
+  dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,])
+
+_METRICSTYPE = _descriptor.EnumDescriptor(
+  name='MetricsType',
+  full_name='brain.MetricsType',
+  filename=None,
+  file=DESCRIPTOR,
+  create_key=_descriptor._internal_create_key,
+  values=[
+    _descriptor.EnumValueDescriptor(
+      name='Training_Hyper_Params', index=0, number=0,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='Workflow_Feature', index=1, number=1,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='Training_Set_Feature', index=2, number=2,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='Model_Feature', index=3, number=3,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='Runtime_Info', index=4, number=4,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='Job_Exit_Reason', index=5, number=5,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='Optimization_Result', index=6, number=6,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='Type', index=7, number=7,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='Resource', index=8, number=8,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='Customized_Data', index=9, number=9,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='Optimization', index=10, number=10,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+  ],
+  containing_type=None,
+  serialized_options=None,
+  serialized_start=3852,
+  serialized_end=4086,
+)
+_sym_db.RegisterEnumDescriptor(_METRICSTYPE)
 
-_METRICSTYPE = DESCRIPTOR.enum_types_by_name['MetricsType']
 MetricsType = enum_type_wrapper.EnumTypeWrapper(_METRICSTYPE)
 Training_Hyper_Params = 0
 Workflow_Feature = 1
 Training_Set_Feature = 2
 Model_Feature = 3
 Runtime_Info = 4
 Job_Exit_Reason = 5
 Optimization_Result = 6
 Type = 7
 Resource = 8
 Customized_Data = 9
 Optimization = 10
 
 
-_TRAININGHYPERPARAMS = DESCRIPTOR.message_types_by_name['TrainingHyperParams']
-_WORKFLOWFEATURE = DESCRIPTOR.message_types_by_name['WorkflowFeature']
-_TRAININGSETFEATURE = DESCRIPTOR.message_types_by_name['TrainingSetFeature']
-_MODELFEATURE = DESCRIPTOR.message_types_by_name['ModelFeature']
-_MODELFEATURE_TENSORALLOCBYTESENTRY = _MODELFEATURE.nested_types_by_name['TensorAllocBytesEntry']
-_RUNTIMEINFO = DESCRIPTOR.message_types_by_name['RuntimeInfo']
-_PODMETA = DESCRIPTOR.message_types_by_name['PodMeta']
-_JOBMETA = DESCRIPTOR.message_types_by_name['JobMeta']
-_JOBMETRICS = DESCRIPTOR.message_types_by_name['JobMetrics']
-_OPTIMIZECONFIG = DESCRIPTOR.message_types_by_name['OptimizeConfig']
-_OPTIMIZECONFIG_CUSTOMIZEDCONFIGENTRY = _OPTIMIZECONFIG.nested_types_by_name['CustomizedConfigEntry']
-_PODSTATE = DESCRIPTOR.message_types_by_name['PodState']
-_PODSTATE_CUSTOMIZEDDATAENTRY = _PODSTATE.nested_types_by_name['CustomizedDataEntry']
-_JOBSTATE = DESCRIPTOR.message_types_by_name['JobState']
-_JOBSTATE_PODSENTRY = _JOBSTATE.nested_types_by_name['PodsEntry']
-_JOBSTATE_CUSTOMIZEDDATAENTRY = _JOBSTATE.nested_types_by_name['CustomizedDataEntry']
-_OPTIMIZEJOBMETA = DESCRIPTOR.message_types_by_name['OptimizeJobMeta']
-_OPTIMIZEREQUEST = DESCRIPTOR.message_types_by_name['OptimizeRequest']
-_PODRESOURCE = DESCRIPTOR.message_types_by_name['PodResource']
-_TASKGROUPRESOURCE = DESCRIPTOR.message_types_by_name['TaskGroupResource']
-_JOBRESOURCE = DESCRIPTOR.message_types_by_name['JobResource']
-_JOBRESOURCE_TASKGROUPRESOURCESENTRY = _JOBRESOURCE.nested_types_by_name['TaskGroupResourcesEntry']
-_JOBRESOURCE_PODRESOURCESENTRY = _JOBRESOURCE.nested_types_by_name['PodResourcesEntry']
-_JOBOPTIMIZEPLAN = DESCRIPTOR.message_types_by_name['JobOptimizePlan']
-_JOBOPTIMIZATION = DESCRIPTOR.message_types_by_name['JobOptimization']
-_RESPONSE = DESCRIPTOR.message_types_by_name['Response']
-_OPTIMIZERESPONSE = DESCRIPTOR.message_types_by_name['OptimizeResponse']
-_JOBMETRICSREQUEST = DESCRIPTOR.message_types_by_name['JobMetricsRequest']
-_JOBMETRICSRESPONSE = DESCRIPTOR.message_types_by_name['JobMetricsResponse']
+
+_TRAININGHYPERPARAMS = _descriptor.Descriptor(
+  name='TrainingHyperParams',
+  full_name='brain.TrainingHyperParams',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='batch_size', full_name='brain.TrainingHyperParams.batch_size', index=0,
+      number=1, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='epoch', full_name='brain.TrainingHyperParams.epoch', index=1,
+      number=2, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='max_steps', full_name='brain.TrainingHyperParams.max_steps', index=2,
+      number=3, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=65,
+  serialized_end=140,
+)
+
+
+_WORKFLOWFEATURE = _descriptor.Descriptor(
+  name='WorkflowFeature',
+  full_name='brain.WorkflowFeature',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='job_name', full_name='brain.WorkflowFeature.job_name', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='user_id', full_name='brain.WorkflowFeature.user_id', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='code_address', full_name='brain.WorkflowFeature.code_address', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='workflow_id', full_name='brain.WorkflowFeature.workflow_id', index=3,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='node_id', full_name='brain.WorkflowFeature.node_id', index=4,
+      number=5, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='odps_project', full_name='brain.WorkflowFeature.odps_project', index=5,
+      number=6, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='is_prod', full_name='brain.WorkflowFeature.is_prod', index=6,
+      number=7, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=143,
+  serialized_end=294,
+)
+
+
+_TRAININGSETFEATURE = _descriptor.Descriptor(
+  name='TrainingSetFeature',
+  full_name='brain.TrainingSetFeature',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='dataset_size', full_name='brain.TrainingSetFeature.dataset_size', index=0,
+      number=1, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='dataset_name', full_name='brain.TrainingSetFeature.dataset_name', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='sparse_item_count', full_name='brain.TrainingSetFeature.sparse_item_count', index=2,
+      number=3, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='sparse_features', full_name='brain.TrainingSetFeature.sparse_features', index=3,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='sparse_feature_groups', full_name='brain.TrainingSetFeature.sparse_feature_groups', index=4,
+      number=5, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='sparse_feature_shapes', full_name='brain.TrainingSetFeature.sparse_feature_shapes', index=5,
+      number=6, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='dense_features', full_name='brain.TrainingSetFeature.dense_features', index=6,
+      number=7, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='dense_feature_shapes', full_name='brain.TrainingSetFeature.dense_feature_shapes', index=7,
+      number=8, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='storage_size', full_name='brain.TrainingSetFeature.storage_size', index=8,
+      number=9, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=297,
+  serialized_end=551,
+)
+
+
+_MODELFEATURE_TENSORALLOCBYTESENTRY = _descriptor.Descriptor(
+  name='TensorAllocBytesEntry',
+  full_name='brain.ModelFeature.TensorAllocBytesEntry',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='key', full_name='brain.ModelFeature.TensorAllocBytesEntry.key', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='value', full_name='brain.ModelFeature.TensorAllocBytesEntry.value', index=1,
+      number=2, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=b'8\001',
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=906,
+  serialized_end=961,
+)
+
+_MODELFEATURE = _descriptor.Descriptor(
+  name='ModelFeature',
+  full_name='brain.ModelFeature',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='variable_count', full_name='brain.ModelFeature.variable_count', index=0,
+      number=1, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='op_count', full_name='brain.ModelFeature.op_count', index=1,
+      number=2, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='embedding_dimension', full_name='brain.ModelFeature.embedding_dimension', index=2,
+      number=3, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='total_variable_size', full_name='brain.ModelFeature.total_variable_size', index=3,
+      number=4, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='max_variable_size', full_name='brain.ModelFeature.max_variable_size', index=4,
+      number=5, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='update_op_count', full_name='brain.ModelFeature.update_op_count', index=5,
+      number=6, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='read_op_count', full_name='brain.ModelFeature.read_op_count', index=6,
+      number=7, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='input_fetch_dur', full_name='brain.ModelFeature.input_fetch_dur', index=7,
+      number=8, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='flops', full_name='brain.ModelFeature.flops', index=8,
+      number=9, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='recv_op_count', full_name='brain.ModelFeature.recv_op_count', index=9,
+      number=10, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='kv_embedding_dims', full_name='brain.ModelFeature.kv_embedding_dims', index=10,
+      number=11, type=3, cpp_type=2, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='tensor_alloc_bytes', full_name='brain.ModelFeature.tensor_alloc_bytes', index=11,
+      number=12, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[_MODELFEATURE_TENSORALLOCBYTESENTRY, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=554,
+  serialized_end=961,
+)
+
+
+_RUNTIMEINFO = _descriptor.Descriptor(
+  name='RuntimeInfo',
+  full_name='brain.RuntimeInfo',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='global_step', full_name='brain.RuntimeInfo.global_step', index=0,
+      number=1, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='running_pods', full_name='brain.RuntimeInfo.running_pods', index=1,
+      number=2, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='time_stamp', full_name='brain.RuntimeInfo.time_stamp', index=2,
+      number=3, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='speed', full_name='brain.RuntimeInfo.speed', index=3,
+      number=4, type=2, cpp_type=6, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=963,
+  serialized_end=1070,
+)
+
+
+_PODMETA = _descriptor.Descriptor(
+  name='PodMeta',
+  full_name='brain.PodMeta',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='pod_name', full_name='brain.PodMeta.pod_name', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='pod_ip', full_name='brain.PodMeta.pod_ip', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='node_ip', full_name='brain.PodMeta.node_ip', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='host_name', full_name='brain.PodMeta.host_name', index=3,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='namespace', full_name='brain.PodMeta.namespace', index=4,
+      number=5, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='is_mixed', full_name='brain.PodMeta.is_mixed', index=5,
+      number=6, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='mem_usage', full_name='brain.PodMeta.mem_usage', index=6,
+      number=7, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='cpu_usage', full_name='brain.PodMeta.cpu_usage', index=7,
+      number=8, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1073,
+  serialized_end=1227,
+)
+
+
+_JOBMETA = _descriptor.Descriptor(
+  name='JobMeta',
+  full_name='brain.JobMeta',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='uuid', full_name='brain.JobMeta.uuid', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='name', full_name='brain.JobMeta.name', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='user', full_name='brain.JobMeta.user', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='cluster', full_name='brain.JobMeta.cluster', index=3,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='namespace', full_name='brain.JobMeta.namespace', index=4,
+      number=5, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1229,
+  serialized_end=1316,
+)
+
+
+_JOBMETRICS = _descriptor.Descriptor(
+  name='JobMetrics',
+  full_name='brain.JobMetrics',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='data_store', full_name='brain.JobMetrics.data_store', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='job_meta', full_name='brain.JobMetrics.job_meta', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='metrics_type', full_name='brain.JobMetrics.metrics_type', index=2,
+      number=3, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='training_hyper_params', full_name='brain.JobMetrics.training_hyper_params', index=3,
+      number=4, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='workflow_feature', full_name='brain.JobMetrics.workflow_feature', index=4,
+      number=5, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='training_set_feature', full_name='brain.JobMetrics.training_set_feature', index=5,
+      number=6, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='model_feature', full_name='brain.JobMetrics.model_feature', index=6,
+      number=7, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='runtime_info', full_name='brain.JobMetrics.runtime_info', index=7,
+      number=8, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='job_exit_reason', full_name='brain.JobMetrics.job_exit_reason', index=8,
+      number=9, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='extra_info', full_name='brain.JobMetrics.extra_info', index=9,
+      number=10, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='type', full_name='brain.JobMetrics.type', index=10,
+      number=11, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='resource', full_name='brain.JobMetrics.resource', index=11,
+      number=12, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='customized_data', full_name='brain.JobMetrics.customized_data', index=12,
+      number=13, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='job_optimization', full_name='brain.JobMetrics.job_optimization', index=13,
+      number=14, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+    _descriptor.OneofDescriptor(
+      name='metrics', full_name='brain.JobMetrics.metrics',
+      index=0, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
+  ],
+  serialized_start=1319,
+  serialized_end=1864,
+)
+
+
+_OPTIMIZECONFIG_CUSTOMIZEDCONFIGENTRY = _descriptor.Descriptor(
+  name='CustomizedConfigEntry',
+  full_name='brain.OptimizeConfig.CustomizedConfigEntry',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='key', full_name='brain.OptimizeConfig.CustomizedConfigEntry.key', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='value', full_name='brain.OptimizeConfig.CustomizedConfigEntry.value', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=b'8\001',
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2038,
+  serialized_end=2093,
+)
+
+_OPTIMIZECONFIG = _descriptor.Descriptor(
+  name='OptimizeConfig',
+  full_name='brain.OptimizeConfig',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='optimizer_config_retriever', full_name='brain.OptimizeConfig.optimizer_config_retriever', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='data_store', full_name='brain.OptimizeConfig.data_store', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='brain_processor', full_name='brain.OptimizeConfig.brain_processor', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='customized_config', full_name='brain.OptimizeConfig.customized_config', index=3,
+      number=4, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[_OPTIMIZECONFIG_CUSTOMIZEDCONFIGENTRY, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1867,
+  serialized_end=2093,
+)
+
+
+_PODSTATE_CUSTOMIZEDDATAENTRY = _descriptor.Descriptor(
+  name='CustomizedDataEntry',
+  full_name='brain.PodState.CustomizedDataEntry',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='key', full_name='brain.PodState.CustomizedDataEntry.key', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='value', full_name='brain.PodState.CustomizedDataEntry.value', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=b'8\001',
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2308,
+  serialized_end=2361,
+)
+
+_PODSTATE = _descriptor.Descriptor(
+  name='PodState',
+  full_name='brain.PodState',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='name', full_name='brain.PodState.name', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='uid', full_name='brain.PodState.uid', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='type', full_name='brain.PodState.type', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='is_oom', full_name='brain.PodState.is_oom', index=3,
+      number=4, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='resource', full_name='brain.PodState.resource', index=4,
+      number=5, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='used_resource', full_name='brain.PodState.used_resource', index=5,
+      number=6, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='customized_data', full_name='brain.PodState.customized_data', index=6,
+      number=7, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[_PODSTATE_CUSTOMIZEDDATAENTRY, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2096,
+  serialized_end=2361,
+)
+
+
+_JOBSTATE_PODSENTRY = _descriptor.Descriptor(
+  name='PodsEntry',
+  full_name='brain.JobState.PodsEntry',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='key', full_name='brain.JobState.PodsEntry.key', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='value', full_name='brain.JobState.PodsEntry.value', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=b'8\001',
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2513,
+  serialized_end=2573,
+)
+
+_JOBSTATE_CUSTOMIZEDDATAENTRY = _descriptor.Descriptor(
+  name='CustomizedDataEntry',
+  full_name='brain.JobState.CustomizedDataEntry',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='key', full_name='brain.JobState.CustomizedDataEntry.key', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='value', full_name='brain.JobState.CustomizedDataEntry.value', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=b'8\001',
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2308,
+  serialized_end=2361,
+)
+
+_JOBSTATE = _descriptor.Descriptor(
+  name='JobState',
+  full_name='brain.JobState',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='timestamp', full_name='brain.JobState.timestamp', index=0,
+      number=1, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='pods', full_name='brain.JobState.pods', index=1,
+      number=2, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='speed', full_name='brain.JobState.speed', index=2,
+      number=3, type=2, cpp_type=6, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='customized_data', full_name='brain.JobState.customized_data', index=3,
+      number=4, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[_JOBSTATE_PODSENTRY, _JOBSTATE_CUSTOMIZEDDATAENTRY, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2364,
+  serialized_end=2628,
+)
+
+
+_OPTIMIZEJOBMETA = _descriptor.Descriptor(
+  name='OptimizeJobMeta',
+  full_name='brain.OptimizeJobMeta',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='uid', full_name='brain.OptimizeJobMeta.uid', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='cluster', full_name='brain.OptimizeJobMeta.cluster', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='namespace', full_name='brain.OptimizeJobMeta.namespace', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='state', full_name='brain.OptimizeJobMeta.state', index=3,
+      number=4, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2630,
+  serialized_end=2728,
+)
+
+
+_OPTIMIZEREQUEST = _descriptor.Descriptor(
+  name='OptimizeRequest',
+  full_name='brain.OptimizeRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='brain.OptimizeRequest.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='config', full_name='brain.OptimizeRequest.config', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='jobs', full_name='brain.OptimizeRequest.jobs', index=2,
+      number=3, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2730,
+  serialized_end=2838,
+)
+
+
+_PODRESOURCE = _descriptor.Descriptor(
+  name='PodResource',
+  full_name='brain.PodResource',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='memory', full_name='brain.PodResource.memory', index=0,
+      number=1, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='cpu', full_name='brain.PodResource.cpu', index=1,
+      number=2, type=2, cpp_type=6, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='gpu', full_name='brain.PodResource.gpu', index=2,
+      number=3, type=2, cpp_type=6, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='gpu_type', full_name='brain.PodResource.gpu_type', index=3,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='priority', full_name='brain.PodResource.priority', index=4,
+      number=5, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2840,
+  serialized_end=2931,
+)
+
+
+_TASKGROUPRESOURCE = _descriptor.Descriptor(
+  name='TaskGroupResource',
+  full_name='brain.TaskGroupResource',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='count', full_name='brain.TaskGroupResource.count', index=0,
+      number=1, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='resource', full_name='brain.TaskGroupResource.resource', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2933,
+  serialized_end=3005,
+)
+
+
+_JOBRESOURCE_TASKGROUPRESOURCESENTRY = _descriptor.Descriptor(
+  name='TaskGroupResourcesEntry',
+  full_name='brain.JobResource.TaskGroupResourcesEntry',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='key', full_name='brain.JobResource.TaskGroupResourcesEntry.key', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='value', full_name='brain.JobResource.TaskGroupResourcesEntry.value', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=b'8\001',
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3158,
+  serialized_end=3241,
+)
+
+_JOBRESOURCE_PODRESOURCESENTRY = _descriptor.Descriptor(
+  name='PodResourcesEntry',
+  full_name='brain.JobResource.PodResourcesEntry',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='key', full_name='brain.JobResource.PodResourcesEntry.key', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='value', full_name='brain.JobResource.PodResourcesEntry.value', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=b'8\001',
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3243,
+  serialized_end=3314,
+)
+
+_JOBRESOURCE = _descriptor.Descriptor(
+  name='JobResource',
+  full_name='brain.JobResource',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='task_group_resources', full_name='brain.JobResource.task_group_resources', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='pod_resources', full_name='brain.JobResource.pod_resources', index=1,
+      number=2, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[_JOBRESOURCE_TASKGROUPRESOURCESENTRY, _JOBRESOURCE_PODRESOURCESENTRY, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3008,
+  serialized_end=3314,
+)
+
+
+_JOBOPTIMIZEPLAN = _descriptor.Descriptor(
+  name='JobOptimizePlan',
+  full_name='brain.JobOptimizePlan',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='timestamp', full_name='brain.JobOptimizePlan.timestamp', index=0,
+      number=1, type=4, cpp_type=4, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='resource', full_name='brain.JobOptimizePlan.resource', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='job', full_name='brain.JobOptimizePlan.job', index=2,
+      number=3, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3316,
+  serialized_end=3427,
+)
+
+
+_JOBOPTIMIZATION = _descriptor.Descriptor(
+  name='JobOptimization',
+  full_name='brain.JobOptimization',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='timestamp', full_name='brain.JobOptimization.timestamp', index=0,
+      number=1, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='config', full_name='brain.JobOptimization.config', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='plan', full_name='brain.JobOptimization.plan', index=2,
+      number=3, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='job_states', full_name='brain.JobOptimization.job_states', index=3,
+      number=4, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3430,
+  serialized_end=3580,
+)
+
+
+_RESPONSE = _descriptor.Descriptor(
+  name='Response',
+  full_name='brain.Response',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='success', full_name='brain.Response.success', index=0,
+      number=1, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='reason', full_name='brain.Response.reason', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3582,
+  serialized_end=3625,
+)
+
+
+_OPTIMIZERESPONSE = _descriptor.Descriptor(
+  name='OptimizeResponse',
+  full_name='brain.OptimizeResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='response', full_name='brain.OptimizeResponse.response', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='job_optimize_plans', full_name='brain.OptimizeResponse.job_optimize_plans', index=1,
+      number=2, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3627,
+  serialized_end=3732,
+)
+
+
+_JOBMETRICSREQUEST = _descriptor.Descriptor(
+  name='JobMetricsRequest',
+  full_name='brain.JobMetricsRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='job_uuid', full_name='brain.JobMetricsRequest.job_uuid', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3734,
+  serialized_end=3771,
+)
+
+
+_JOBMETRICSRESPONSE = _descriptor.Descriptor(
+  name='JobMetricsResponse',
+  full_name='brain.JobMetricsResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='response', full_name='brain.JobMetricsResponse.response', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='job_metrics', full_name='brain.JobMetricsResponse.job_metrics', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3773,
+  serialized_end=3849,
+)
+
+_MODELFEATURE_TENSORALLOCBYTESENTRY.containing_type = _MODELFEATURE
+_MODELFEATURE.fields_by_name['tensor_alloc_bytes'].message_type = _MODELFEATURE_TENSORALLOCBYTESENTRY
+_RUNTIMEINFO.fields_by_name['running_pods'].message_type = _PODMETA
+_JOBMETRICS.fields_by_name['job_meta'].message_type = _JOBMETA
+_JOBMETRICS.fields_by_name['metrics_type'].enum_type = _METRICSTYPE
+_JOBMETRICS.fields_by_name['training_hyper_params'].message_type = _TRAININGHYPERPARAMS
+_JOBMETRICS.fields_by_name['workflow_feature'].message_type = _WORKFLOWFEATURE
+_JOBMETRICS.fields_by_name['training_set_feature'].message_type = _TRAININGSETFEATURE
+_JOBMETRICS.fields_by_name['model_feature'].message_type = _MODELFEATURE
+_JOBMETRICS.fields_by_name['runtime_info'].message_type = _RUNTIMEINFO
+_JOBMETRICS.fields_by_name['job_optimization'].message_type = _JOBOPTIMIZATION
+_JOBMETRICS.oneofs_by_name['metrics'].fields.append(
+  _JOBMETRICS.fields_by_name['training_hyper_params'])
+_JOBMETRICS.fields_by_name['training_hyper_params'].containing_oneof = _JOBMETRICS.oneofs_by_name['metrics']
+_JOBMETRICS.oneofs_by_name['metrics'].fields.append(
+  _JOBMETRICS.fields_by_name['workflow_feature'])
+_JOBMETRICS.fields_by_name['workflow_feature'].containing_oneof = _JOBMETRICS.oneofs_by_name['metrics']
+_JOBMETRICS.oneofs_by_name['metrics'].fields.append(
+  _JOBMETRICS.fields_by_name['training_set_feature'])
+_JOBMETRICS.fields_by_name['training_set_feature'].containing_oneof = _JOBMETRICS.oneofs_by_name['metrics']
+_JOBMETRICS.oneofs_by_name['metrics'].fields.append(
+  _JOBMETRICS.fields_by_name['model_feature'])
+_JOBMETRICS.fields_by_name['model_feature'].containing_oneof = _JOBMETRICS.oneofs_by_name['metrics']
+_JOBMETRICS.oneofs_by_name['metrics'].fields.append(
+  _JOBMETRICS.fields_by_name['runtime_info'])
+_JOBMETRICS.fields_by_name['runtime_info'].containing_oneof = _JOBMETRICS.oneofs_by_name['metrics']
+_JOBMETRICS.oneofs_by_name['metrics'].fields.append(
+  _JOBMETRICS.fields_by_name['job_exit_reason'])
+_JOBMETRICS.fields_by_name['job_exit_reason'].containing_oneof = _JOBMETRICS.oneofs_by_name['metrics']
+_JOBMETRICS.oneofs_by_name['metrics'].fields.append(
+  _JOBMETRICS.fields_by_name['extra_info'])
+_JOBMETRICS.fields_by_name['extra_info'].containing_oneof = _JOBMETRICS.oneofs_by_name['metrics']
+_JOBMETRICS.oneofs_by_name['metrics'].fields.append(
+  _JOBMETRICS.fields_by_name['type'])
+_JOBMETRICS.fields_by_name['type'].containing_oneof = _JOBMETRICS.oneofs_by_name['metrics']
+_JOBMETRICS.oneofs_by_name['metrics'].fields.append(
+  _JOBMETRICS.fields_by_name['resource'])
+_JOBMETRICS.fields_by_name['resource'].containing_oneof = _JOBMETRICS.oneofs_by_name['metrics']
+_JOBMETRICS.oneofs_by_name['metrics'].fields.append(
+  _JOBMETRICS.fields_by_name['customized_data'])
+_JOBMETRICS.fields_by_name['customized_data'].containing_oneof = _JOBMETRICS.oneofs_by_name['metrics']
+_JOBMETRICS.oneofs_by_name['metrics'].fields.append(
+  _JOBMETRICS.fields_by_name['job_optimization'])
+_JOBMETRICS.fields_by_name['job_optimization'].containing_oneof = _JOBMETRICS.oneofs_by_name['metrics']
+_OPTIMIZECONFIG_CUSTOMIZEDCONFIGENTRY.containing_type = _OPTIMIZECONFIG
+_OPTIMIZECONFIG.fields_by_name['customized_config'].message_type = _OPTIMIZECONFIG_CUSTOMIZEDCONFIGENTRY
+_PODSTATE_CUSTOMIZEDDATAENTRY.containing_type = _PODSTATE
+_PODSTATE.fields_by_name['resource'].message_type = _PODRESOURCE
+_PODSTATE.fields_by_name['used_resource'].message_type = _PODRESOURCE
+_PODSTATE.fields_by_name['customized_data'].message_type = _PODSTATE_CUSTOMIZEDDATAENTRY
+_JOBSTATE_PODSENTRY.fields_by_name['value'].message_type = _PODSTATE
+_JOBSTATE_PODSENTRY.containing_type = _JOBSTATE
+_JOBSTATE_CUSTOMIZEDDATAENTRY.containing_type = _JOBSTATE
+_JOBSTATE.fields_by_name['pods'].message_type = _JOBSTATE_PODSENTRY
+_JOBSTATE.fields_by_name['customized_data'].message_type = _JOBSTATE_CUSTOMIZEDDATAENTRY
+_OPTIMIZEJOBMETA.fields_by_name['state'].message_type = _JOBSTATE
+_OPTIMIZEREQUEST.fields_by_name['config'].message_type = _OPTIMIZECONFIG
+_OPTIMIZEREQUEST.fields_by_name['jobs'].message_type = _OPTIMIZEJOBMETA
+_TASKGROUPRESOURCE.fields_by_name['resource'].message_type = _PODRESOURCE
+_JOBRESOURCE_TASKGROUPRESOURCESENTRY.fields_by_name['value'].message_type = _TASKGROUPRESOURCE
+_JOBRESOURCE_TASKGROUPRESOURCESENTRY.containing_type = _JOBRESOURCE
+_JOBRESOURCE_PODRESOURCESENTRY.fields_by_name['value'].message_type = _PODRESOURCE
+_JOBRESOURCE_PODRESOURCESENTRY.containing_type = _JOBRESOURCE
+_JOBRESOURCE.fields_by_name['task_group_resources'].message_type = _JOBRESOURCE_TASKGROUPRESOURCESENTRY
+_JOBRESOURCE.fields_by_name['pod_resources'].message_type = _JOBRESOURCE_PODRESOURCESENTRY
+_JOBOPTIMIZEPLAN.fields_by_name['resource'].message_type = _JOBRESOURCE
+_JOBOPTIMIZEPLAN.fields_by_name['job'].message_type = _OPTIMIZEJOBMETA
+_JOBOPTIMIZATION.fields_by_name['config'].message_type = _OPTIMIZECONFIG
+_JOBOPTIMIZATION.fields_by_name['plan'].message_type = _JOBOPTIMIZEPLAN
+_JOBOPTIMIZATION.fields_by_name['job_states'].message_type = _JOBSTATE
+_OPTIMIZERESPONSE.fields_by_name['response'].message_type = _RESPONSE
+_OPTIMIZERESPONSE.fields_by_name['job_optimize_plans'].message_type = _JOBOPTIMIZEPLAN
+_JOBMETRICSRESPONSE.fields_by_name['response'].message_type = _RESPONSE
+DESCRIPTOR.message_types_by_name['TrainingHyperParams'] = _TRAININGHYPERPARAMS
+DESCRIPTOR.message_types_by_name['WorkflowFeature'] = _WORKFLOWFEATURE
+DESCRIPTOR.message_types_by_name['TrainingSetFeature'] = _TRAININGSETFEATURE
+DESCRIPTOR.message_types_by_name['ModelFeature'] = _MODELFEATURE
+DESCRIPTOR.message_types_by_name['RuntimeInfo'] = _RUNTIMEINFO
+DESCRIPTOR.message_types_by_name['PodMeta'] = _PODMETA
+DESCRIPTOR.message_types_by_name['JobMeta'] = _JOBMETA
+DESCRIPTOR.message_types_by_name['JobMetrics'] = _JOBMETRICS
+DESCRIPTOR.message_types_by_name['OptimizeConfig'] = _OPTIMIZECONFIG
+DESCRIPTOR.message_types_by_name['PodState'] = _PODSTATE
+DESCRIPTOR.message_types_by_name['JobState'] = _JOBSTATE
+DESCRIPTOR.message_types_by_name['OptimizeJobMeta'] = _OPTIMIZEJOBMETA
+DESCRIPTOR.message_types_by_name['OptimizeRequest'] = _OPTIMIZEREQUEST
+DESCRIPTOR.message_types_by_name['PodResource'] = _PODRESOURCE
+DESCRIPTOR.message_types_by_name['TaskGroupResource'] = _TASKGROUPRESOURCE
+DESCRIPTOR.message_types_by_name['JobResource'] = _JOBRESOURCE
+DESCRIPTOR.message_types_by_name['JobOptimizePlan'] = _JOBOPTIMIZEPLAN
+DESCRIPTOR.message_types_by_name['JobOptimization'] = _JOBOPTIMIZATION
+DESCRIPTOR.message_types_by_name['Response'] = _RESPONSE
+DESCRIPTOR.message_types_by_name['OptimizeResponse'] = _OPTIMIZERESPONSE
+DESCRIPTOR.message_types_by_name['JobMetricsRequest'] = _JOBMETRICSREQUEST
+DESCRIPTOR.message_types_by_name['JobMetricsResponse'] = _JOBMETRICSRESPONSE
+DESCRIPTOR.enum_types_by_name['MetricsType'] = _METRICSTYPE
+_sym_db.RegisterFileDescriptor(DESCRIPTOR)
+
 TrainingHyperParams = _reflection.GeneratedProtocolMessageType('TrainingHyperParams', (_message.Message,), {
   'DESCRIPTOR' : _TRAININGHYPERPARAMS,
   '__module__' : 'dlrover.proto.brain_pb2'
   # @@protoc_insertion_point(class_scope:brain.TrainingHyperParams)
   })
 _sym_db.RegisterMessage(TrainingHyperParams)
 
@@ -268,89 +1983,63 @@
 JobMetricsResponse = _reflection.GeneratedProtocolMessageType('JobMetricsResponse', (_message.Message,), {
   'DESCRIPTOR' : _JOBMETRICSRESPONSE,
   '__module__' : 'dlrover.proto.brain_pb2'
   # @@protoc_insertion_point(class_scope:brain.JobMetricsResponse)
   })
 _sym_db.RegisterMessage(JobMetricsResponse)
 
-_BRAIN = DESCRIPTOR.services_by_name['Brain']
-if _descriptor._USE_C_DESCRIPTORS == False:
 
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z\032dlrover/go/brain/pkg/proto'
-  _MODELFEATURE_TENSORALLOCBYTESENTRY._options = None
-  _MODELFEATURE_TENSORALLOCBYTESENTRY._serialized_options = b'8\001'
-  _OPTIMIZECONFIG_CUSTOMIZEDCONFIGENTRY._options = None
-  _OPTIMIZECONFIG_CUSTOMIZEDCONFIGENTRY._serialized_options = b'8\001'
-  _PODSTATE_CUSTOMIZEDDATAENTRY._options = None
-  _PODSTATE_CUSTOMIZEDDATAENTRY._serialized_options = b'8\001'
-  _JOBSTATE_PODSENTRY._options = None
-  _JOBSTATE_PODSENTRY._serialized_options = b'8\001'
-  _JOBSTATE_CUSTOMIZEDDATAENTRY._options = None
-  _JOBSTATE_CUSTOMIZEDDATAENTRY._serialized_options = b'8\001'
-  _JOBRESOURCE_TASKGROUPRESOURCESENTRY._options = None
-  _JOBRESOURCE_TASKGROUPRESOURCESENTRY._serialized_options = b'8\001'
-  _JOBRESOURCE_PODRESOURCESENTRY._options = None
-  _JOBRESOURCE_PODRESOURCESENTRY._serialized_options = b'8\001'
-  _METRICSTYPE._serialized_start=3834
-  _METRICSTYPE._serialized_end=4068
-  _TRAININGHYPERPARAMS._serialized_start=65
-  _TRAININGHYPERPARAMS._serialized_end=140
-  _WORKFLOWFEATURE._serialized_start=143
-  _WORKFLOWFEATURE._serialized_end=294
-  _TRAININGSETFEATURE._serialized_start=297
-  _TRAININGSETFEATURE._serialized_end=551
-  _MODELFEATURE._serialized_start=554
-  _MODELFEATURE._serialized_end=961
-  _MODELFEATURE_TENSORALLOCBYTESENTRY._serialized_start=906
-  _MODELFEATURE_TENSORALLOCBYTESENTRY._serialized_end=961
-  _RUNTIMEINFO._serialized_start=963
-  _RUNTIMEINFO._serialized_end=1070
-  _PODMETA._serialized_start=1073
-  _PODMETA._serialized_end=1227
-  _JOBMETA._serialized_start=1229
-  _JOBMETA._serialized_end=1316
-  _JOBMETRICS._serialized_start=1319
-  _JOBMETRICS._serialized_end=1864
-  _OPTIMIZECONFIG._serialized_start=1867
-  _OPTIMIZECONFIG._serialized_end=2093
-  _OPTIMIZECONFIG_CUSTOMIZEDCONFIGENTRY._serialized_start=2038
-  _OPTIMIZECONFIG_CUSTOMIZEDCONFIGENTRY._serialized_end=2093
-  _PODSTATE._serialized_start=2096
-  _PODSTATE._serialized_end=2361
-  _PODSTATE_CUSTOMIZEDDATAENTRY._serialized_start=2308
-  _PODSTATE_CUSTOMIZEDDATAENTRY._serialized_end=2361
-  _JOBSTATE._serialized_start=2364
-  _JOBSTATE._serialized_end=2628
-  _JOBSTATE_PODSENTRY._serialized_start=2513
-  _JOBSTATE_PODSENTRY._serialized_end=2573
-  _JOBSTATE_CUSTOMIZEDDATAENTRY._serialized_start=2308
-  _JOBSTATE_CUSTOMIZEDDATAENTRY._serialized_end=2361
-  _OPTIMIZEJOBMETA._serialized_start=2630
-  _OPTIMIZEJOBMETA._serialized_end=2728
-  _OPTIMIZEREQUEST._serialized_start=2730
-  _OPTIMIZEREQUEST._serialized_end=2838
-  _PODRESOURCE._serialized_start=2840
-  _PODRESOURCE._serialized_end=2913
-  _TASKGROUPRESOURCE._serialized_start=2915
-  _TASKGROUPRESOURCE._serialized_end=2987
-  _JOBRESOURCE._serialized_start=2990
-  _JOBRESOURCE._serialized_end=3296
-  _JOBRESOURCE_TASKGROUPRESOURCESENTRY._serialized_start=3140
-  _JOBRESOURCE_TASKGROUPRESOURCESENTRY._serialized_end=3223
-  _JOBRESOURCE_PODRESOURCESENTRY._serialized_start=3225
-  _JOBRESOURCE_PODRESOURCESENTRY._serialized_end=3296
-  _JOBOPTIMIZEPLAN._serialized_start=3298
-  _JOBOPTIMIZEPLAN._serialized_end=3409
-  _JOBOPTIMIZATION._serialized_start=3412
-  _JOBOPTIMIZATION._serialized_end=3562
-  _RESPONSE._serialized_start=3564
-  _RESPONSE._serialized_end=3607
-  _OPTIMIZERESPONSE._serialized_start=3609
-  _OPTIMIZERESPONSE._serialized_end=3714
-  _JOBMETRICSREQUEST._serialized_start=3716
-  _JOBMETRICSREQUEST._serialized_end=3753
-  _JOBMETRICSRESPONSE._serialized_start=3755
-  _JOBMETRICSRESPONSE._serialized_end=3831
-  _BRAIN._serialized_start=4071
-  _BRAIN._serialized_end=4273
+DESCRIPTOR._options = None
+_MODELFEATURE_TENSORALLOCBYTESENTRY._options = None
+_OPTIMIZECONFIG_CUSTOMIZEDCONFIGENTRY._options = None
+_PODSTATE_CUSTOMIZEDDATAENTRY._options = None
+_JOBSTATE_PODSENTRY._options = None
+_JOBSTATE_CUSTOMIZEDDATAENTRY._options = None
+_JOBRESOURCE_TASKGROUPRESOURCESENTRY._options = None
+_JOBRESOURCE_PODRESOURCESENTRY._options = None
+
+_BRAIN = _descriptor.ServiceDescriptor(
+  name='Brain',
+  full_name='brain.Brain',
+  file=DESCRIPTOR,
+  index=0,
+  serialized_options=None,
+  create_key=_descriptor._internal_create_key,
+  serialized_start=4089,
+  serialized_end=4291,
+  methods=[
+  _descriptor.MethodDescriptor(
+    name='persist_metrics',
+    full_name='brain.Brain.persist_metrics',
+    index=0,
+    containing_service=None,
+    input_type=_JOBMETRICS,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='optimize',
+    full_name='brain.Brain.optimize',
+    index=1,
+    containing_service=None,
+    input_type=_OPTIMIZEREQUEST,
+    output_type=_OPTIMIZERESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='get_job_metrics',
+    full_name='brain.Brain.get_job_metrics',
+    index=2,
+    containing_service=None,
+    input_type=_JOBMETRICSREQUEST,
+    output_type=_JOBMETRICSRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+])
+_sym_db.RegisterServiceDescriptor(_BRAIN)
+
+DESCRIPTOR.services_by_name['Brain'] = _BRAIN
+
 # @@protoc_insertion_point(module_scope)
```

## dlrover/proto/elastic_training.proto

```diff
@@ -21,15 +21,15 @@
 
   // Starting and ending (non-inclusive) record number.
   int64 start = 2;
   int64 end = 3;
   repeated int64 indices = 4;
 }
 
-// A task is a unit of work for ElasticDL training workers, assigned by master.
+// A task is a unit of work for DLRover training workers, assigned by master.
 // Worker divides a task into multiple minibatches and compute a gradient for
 // each minibatch. For now, only RecordIO file format is supported.
 message Task {
   // Unique id assigned by master.
   // TODO: int32 -> int64
   int32 task_id = 1;
 
@@ -76,63 +76,23 @@
   bool shuffle = 4;
   int32 num_minibatches_per_shard = 5;
   string dataset_name = 6;
   TaskType task_type = 7;
   string storage_type = 8;
 }
 
-message DatasetMeta { string dataset_name = 1; }
-
-message GetDatasetEpochResponse { int32 epoch = 1; }
-
-message DdpResetSyncRequest {
-  string worker_host = 1;
-  int32 worker_local_process_id = 2;
-  int32 rendezvous_id = 3;
-}
-
-message DdpResetSyncResponse { bool reset = 1; }
-
-message DdpInitSyncRequest {
-  string worker_host = 1;
-  int32 worker_local_process_id = 2;
-  int32 rendezvous_id = 3;
-}
-
-message DdpInitSyncResponse { bool reset = 1; }
-
-message GetCommRankRequest {
-  string worker_host = 1;
-  int32 worker_local_process_id = 2;
-}
-
-message GetCommRankResponse {
-  int32 rank_id = 1;
-  int32 world_size = 2;
-  int32 rendezvous_id = 3;
-  int32 rendezvous_port = 4;
-  int32 local_rank = 5;
-  int32 local_size = 6;
-  int32 cross_rank = 7;
-  int32 cross_size = 8;
-  int32 master_port = 9;
-  string master_addr = 10;
+message DatasetMeta {
+  string dataset_name = 1;
+  int32 shard_num = 2;
 }
 
-message ReportTrainingLoopStatusRequest {
-  string worker_host = 1;
-  int32 status = 2;
-  int32 worker_local_process_id = 3;
-  int32 ddp_server_port = 4;
-}
+message GetDatasetEpochResponse { int32 epoch = 1; }
 
 message ShardCheckpoint { string content = 1; }
 
-message ReportShardCheckpointResponse { bool success = 1; }
-
 message ReportUsedResourceRequest {
   // Used memory with Byte
   int64 memory = 1;
   float cpu = 2;
   int32 node_id = 3;
   string node_type = 4;
 }
@@ -194,80 +154,145 @@
   int64 timestamp = 1;
   int64 global_step = 2;
 }
 
 message QueryPsNodesResponse {
   repeated NodeMeta ps_nodes = 1;
   bool new_ps_ready = 2;
+  bool ps_failure = 3;
 }
 
 message NodeMeta {
   string type = 1;
   string addr = 2;
   int32 memory = 3;
-  int32 cpu = 4;
+  float cpu = 4;
   int32 gpu = 5;
   string gpu_type = 6;
+  int32 id = 7;
+  int32 rank = 8;
+  string status = 9;
+}
+
+message NodeEvent {
+  string event_type = 1;
+  NodeMeta node = 2;
+  string message = 3;
 }
 
 message RunningNodes { repeated NodeMeta nodes = 1; }
 
 message QueryTrainingStatusResponse { int32 status = 1; }
 
 message ResourceConfig {
   int32 num = 1;
   int32 cpu = 2;
   int32 memory = 3; // Mi
 }
 
 message ReportPreStopRequest { string worker_host = 1; }
 
-service Master {
-  rpc reset_sync(DdpResetSyncRequest) returns (DdpResetSyncResponse);
-  rpc barrier_sync(DdpInitSyncRequest) returns (DdpInitSyncResponse);
-  rpc get_comm_rank(GetCommRankRequest) returns (GetCommRankResponse);
-  rpc report_training_loop_status(ReportTrainingLoopStatusRequest)
-      returns (google.protobuf.Empty);
+message SyncRequest {
+  string sync_name = 1;
+  int32 worker_id = 2;
+  string worker_type = 3;
+}
 
-  // TODO : Unify the above 3 PRCs with new ones.
+message BarrierRequest {
+  string barrier_name = 1;
+  bool notify = 3;
+}
+
+message RendezvousState {
+  map<int32, int32> world = 1;
+  int32 waiting_num = 2;
+  int32 round = 3;
+  int32 group = 4;
+}
+
+message RendezvousRequest {
+  int32 node_id = 1;
+  int32 local_world_size = 2;
+  string rdzv_name = 4;
+}
+
+message RendezvousParams {
+  int32 min_nodes = 1;
+  int32 max_nodes = 2;
+  int32 waiting_timeout = 3;
+  int32 node_unit = 4;
+}
+
+message KeyValuePair {
+  string key = 1;
+  bytes value = 2;
+}
+
+message Response {
+  bool success = 1;
+  string reason = 2;
+}
+
+message NodeFailure {
+  int32 node_id = 1;
+  string node_type = 2;
+  string error_data = 3;
+  int32 restart_count = 4;
+}
+
+service Master {
   rpc get_task(GetTaskRequest) returns (Task);
   rpc report_task_result(ReportTaskResultRequest)
       returns (google.protobuf.Empty);
   rpc report_dataset_shard_params(ReportDatasetShardParamsRequest)
       returns (google.protobuf.Empty);
-
   rpc get_dataset_epoch(DatasetMeta) returns (GetDatasetEpochResponse);
-
-  // rpcs for supporting PS adjustment
-  rpc ready_for_ps_relaunch(google.protobuf.Empty)
-      returns (google.protobuf.Empty);
+  rpc get_dataset_shard_num(DatasetMeta) returns (DatasetMeta);
 
   // rpcs for saving and restoring data shard checkpoints
   rpc get_shard_checkpoint(DatasetMeta) returns (ShardCheckpoint);
-  rpc report_shard_checkpoint(ShardCheckpoint)
-      returns (ReportShardCheckpointResponse);
+  rpc report_shard_checkpoint(ShardCheckpoint) returns (Response);
 
+  // rpcs to report training metrics
   rpc report_used_resource(ReportUsedResourceRequest)
       returns (google.protobuf.Empty);
-
   rpc report_model_metric(ModelMetric) returns (google.protobuf.Empty);
   rpc report_global_step(GlobalStepRecord) returns (google.protobuf.Empty);
-  rpc query_running_nodes(google.protobuf.Empty) returns (RunningNodes);
+
+  // rpcs for worker sync
+  rpc join_sync(SyncRequest) returns (Response);
+  rpc sync_finished(SyncRequest) returns (Response);
+  rpc barrier(BarrierRequest) returns (Response);
 
   // rpc for elastic PS
   rpc get_cluster_version(GetClusterVersionRequest)
       returns (GetClusterVersionResponse);
   rpc update_cluster_version(UpdateClusterVersionRequest)
       returns (google.protobuf.Empty);
   rpc query_ps_nodes(google.protobuf.Empty) returns (QueryPsNodesResponse);
   rpc query_training_status(google.protobuf.Empty)
       returns (QueryTrainingStatusResponse);
+  rpc query_running_nodes(google.protobuf.Empty) returns (RunningNodes);
+  rpc ready_for_ps_relaunch(google.protobuf.Empty)
+      returns (google.protobuf.Empty);
 
   // rpc for remote lock
   rpc init_remote_lock(InitRemoteLockRequest) returns (google.protobuf.Empty);
   rpc acquire_remote_lock(AcquireRemoteLockRequest)
       returns (AcquireRemoteLockResponse);
   rpc release_remote_lock(ReleaseRemoteLockRequest)
       returns (google.protobuf.Empty);
 
+  // rpc for torch elastic
+  rpc get_comm_world(RendezvousRequest) returns (RendezvousState);
+  rpc join_rendezvous(RendezvousRequest) returns (RendezvousState);
+  rpc num_nodes_waiting(RendezvousRequest) returns (RendezvousState);
+  rpc report_rdzv_params(RendezvousParams) returns (Response);
+  rpc kv_store_set(KeyValuePair) returns (Response);
+  rpc kv_store_get(KeyValuePair) returns (KeyValuePair);
+  rpc report_failure(NodeFailure) returns (Response);
+  rpc network_check_success(RendezvousRequest) returns (Response);
+
   rpc report_prestop(ReportPreStopRequest) returns (google.protobuf.Empty);
+  rpc update_node_status(NodeMeta) returns (Response);
+  rpc update_node_event(NodeEvent) returns (google.protobuf.Empty);
 }
```

## dlrover/proto/elastic_training_pb2.py

```diff
@@ -1,74 +1,1925 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: dlrover/proto/elastic_training.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$dlrover/proto/elastic_training.proto\x12\x07\x65lastic\x1a\x1bgoogle/protobuf/empty.proto\"B\n\x05Shard\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05start\x18\x02 \x01(\x03\x12\x0b\n\x03\x65nd\x18\x03 \x01(\x03\x12\x0f\n\x07indices\x18\x04 \x03(\x03\"\xe1\x01\n\x04Task\x12\x0f\n\x07task_id\x18\x01 \x01(\x05\x12\x1d\n\x05shard\x18\x02 \x01(\x0b\x32\x0e.elastic.Shard\x12\x15\n\rmodel_version\x18\x03 \x01(\x05\x12\x1f\n\x04type\x18\x04 \x01(\x0e\x32\x11.elastic.TaskType\x12:\n\x0f\x65xtended_config\x18\x05 \x03(\x0b\x32!.elastic.Task.ExtendedConfigEntry\x1a\x35\n\x13\x45xtendedConfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"N\n\x0eGetTaskRequest\x12\x13\n\x0bworker_type\x18\x01 \x01(\t\x12\x11\n\tworker_id\x18\x02 \x01(\x05\x12\x14\n\x0c\x64\x61taset_name\x18\x03 \x01(\t\"\xd5\x01\n\x17ReportTaskResultRequest\x12\x14\n\x0c\x64\x61taset_name\x18\x01 \x01(\t\x12\x0f\n\x07task_id\x18\x02 \x01(\x03\x12\x13\n\x0b\x65rr_message\x18\x03 \x01(\t\x12I\n\rexec_counters\x18\x04 \x03(\x0b\x32\x32.elastic.ReportTaskResultRequest.ExecCountersEntry\x1a\x33\n\x11\x45xecCountersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"\xe5\x01\n\x1fReportDatasetShardParamsRequest\x12\x12\n\nbatch_size\x18\x01 \x01(\x05\x12\x12\n\nnum_epochs\x18\x02 \x01(\x05\x12\x14\n\x0c\x64\x61taset_size\x18\x03 \x01(\x03\x12\x0f\n\x07shuffle\x18\x04 \x01(\x08\x12!\n\x19num_minibatches_per_shard\x18\x05 \x01(\x05\x12\x14\n\x0c\x64\x61taset_name\x18\x06 \x01(\t\x12$\n\ttask_type\x18\x07 \x01(\x0e\x32\x11.elastic.TaskType\x12\x14\n\x0cstorage_type\x18\x08 \x01(\t\"#\n\x0b\x44\x61tasetMeta\x12\x14\n\x0c\x64\x61taset_name\x18\x01 \x01(\t\"(\n\x17GetDatasetEpochResponse\x12\r\n\x05\x65poch\x18\x01 \x01(\x05\"b\n\x13\x44\x64pResetSyncRequest\x12\x13\n\x0bworker_host\x18\x01 \x01(\t\x12\x1f\n\x17worker_local_process_id\x18\x02 \x01(\x05\x12\x15\n\rrendezvous_id\x18\x03 \x01(\x05\"%\n\x14\x44\x64pResetSyncResponse\x12\r\n\x05reset\x18\x01 \x01(\x08\"a\n\x12\x44\x64pInitSyncRequest\x12\x13\n\x0bworker_host\x18\x01 \x01(\t\x12\x1f\n\x17worker_local_process_id\x18\x02 \x01(\x05\x12\x15\n\rrendezvous_id\x18\x03 \x01(\x05\"$\n\x13\x44\x64pInitSyncResponse\x12\r\n\x05reset\x18\x01 \x01(\x08\"J\n\x12GetCommRankRequest\x12\x13\n\x0bworker_host\x18\x01 \x01(\t\x12\x1f\n\x17worker_local_process_id\x18\x02 \x01(\x05\"\xe4\x01\n\x13GetCommRankResponse\x12\x0f\n\x07rank_id\x18\x01 \x01(\x05\x12\x12\n\nworld_size\x18\x02 \x01(\x05\x12\x15\n\rrendezvous_id\x18\x03 \x01(\x05\x12\x17\n\x0frendezvous_port\x18\x04 \x01(\x05\x12\x12\n\nlocal_rank\x18\x05 \x01(\x05\x12\x12\n\nlocal_size\x18\x06 \x01(\x05\x12\x12\n\ncross_rank\x18\x07 \x01(\x05\x12\x12\n\ncross_size\x18\x08 \x01(\x05\x12\x13\n\x0bmaster_port\x18\t \x01(\x05\x12\x13\n\x0bmaster_addr\x18\n \x01(\t\"\x80\x01\n\x1fReportTrainingLoopStatusRequest\x12\x13\n\x0bworker_host\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\x05\x12\x1f\n\x17worker_local_process_id\x18\x03 \x01(\x05\x12\x17\n\x0f\x64\x64p_server_port\x18\x04 \x01(\x05\"\"\n\x0fShardCheckpoint\x12\x0f\n\x07\x63ontent\x18\x01 \x01(\t\"0\n\x1dReportShardCheckpointResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"\\\n\x19ReportUsedResourceRequest\x12\x0e\n\x06memory\x18\x01 \x01(\x03\x12\x0b\n\x03\x63pu\x18\x02 \x01(\x02\x12\x0f\n\x07node_id\x18\x03 \x01(\x05\x12\x11\n\tnode_type\x18\x04 \x01(\t\"\xf9\x01\n\x0bTensorStats\x12\x16\n\x0evariable_count\x18\x01 \x01(\x03\x12\x1b\n\x13total_variable_size\x18\x02 \x01(\x03\x12\x19\n\x11max_variable_size\x18\x03 \x01(\x03\x12\x19\n\x11kv_embedding_dims\x18\x04 \x03(\x03\x12\x46\n\x12tensor_alloc_bytes\x18\x05 \x03(\x0b\x32*.elastic.TensorStats.TensorAllocBytesEntry\x1a\x37\n\x15TensorAllocBytesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x03:\x02\x38\x01\"\x91\x01\n\x0eOperationStats\x12\x10\n\x08op_count\x18\x01 \x01(\x03\x12\x17\n\x0fupdate_op_count\x18\x02 \x01(\x03\x12\x15\n\rread_op_count\x18\x03 \x01(\x03\x12\x17\n\x0finput_fetch_dur\x18\x04 \x01(\x03\x12\r\n\x05\x66lops\x18\x05 \x01(\x03\x12\x15\n\rrecv_op_count\x18\x06 \x01(\x03\"d\n\x0bModelMetric\x12*\n\x0ctensor_stats\x18\x01 \x01(\x0b\x32\x14.elastic.TensorStats\x12)\n\x08op_stats\x18\x02 \x01(\x0b\x32\x17.elastic.OperationStats\"T\n\x18GetClusterVersionRequest\x12\x0f\n\x07task_id\x18\x01 \x01(\x05\x12\x14\n\x0cversion_type\x18\x02 \x01(\t\x12\x11\n\ttask_type\x18\x03 \x01(\t\",\n\x19GetClusterVersionResponse\x12\x0f\n\x07version\x18\x01 \x01(\x05\"h\n\x1bUpdateClusterVersionRequest\x12\x0f\n\x07task_id\x18\x01 \x01(\x05\x12\x0f\n\x07version\x18\x02 \x01(\x05\x12\x14\n\x0cversion_type\x18\x03 \x01(\t\x12\x11\n\ttask_type\x18\x04 \x01(\t\"I\n\x15InitRemoteLockRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07timeout\x18\x02 \x01(\x05\x12\x11\n\tworker_id\x18\x03 \x01(\x05\"L\n\x18\x41\x63quireRemoteLockRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07timeout\x18\x02 \x01(\x05\x12\x11\n\tworker_id\x18\x03 \x01(\x05\",\n\x19\x41\x63quireRemoteLockResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"(\n\x18ReleaseRemoteLockRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\":\n\x10GlobalStepRecord\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x13\n\x0bglobal_step\x18\x02 \x01(\x03\"Q\n\x14QueryPsNodesResponse\x12#\n\x08ps_nodes\x18\x01 \x03(\x0b\x32\x11.elastic.NodeMeta\x12\x14\n\x0cnew_ps_ready\x18\x02 \x01(\x08\"b\n\x08NodeMeta\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0c\n\x04\x61\x64\x64r\x18\x02 \x01(\t\x12\x0e\n\x06memory\x18\x03 \x01(\x05\x12\x0b\n\x03\x63pu\x18\x04 \x01(\x05\x12\x0b\n\x03gpu\x18\x05 \x01(\x05\x12\x10\n\x08gpu_type\x18\x06 \x01(\t\"0\n\x0cRunningNodes\x12 \n\x05nodes\x18\x01 \x03(\x0b\x32\x11.elastic.NodeMeta\"-\n\x1bQueryTrainingStatusResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\":\n\x0eResourceConfig\x12\x0b\n\x03num\x18\x01 \x01(\x05\x12\x0b\n\x03\x63pu\x18\x02 \x01(\x05\x12\x0e\n\x06memory\x18\x03 \x01(\x05\"+\n\x14ReportPreStopRequest\x12\x13\n\x0bworker_host\x18\x01 \x01(\t*d\n\x08TaskType\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08TRAINING\x10\x01\x12\x0e\n\nEVALUATION\x10\x02\x12\x0e\n\nPREDICTION\x10\x03\x12\x08\n\x04WAIT\x10\x04\x12\x16\n\x12TRAIN_END_CALLBACK\x10\x05\x32\xae\x0e\n\x06Master\x12I\n\nreset_sync\x12\x1c.elastic.DdpResetSyncRequest\x1a\x1d.elastic.DdpResetSyncResponse\x12I\n\x0c\x62\x61rrier_sync\x12\x1b.elastic.DdpInitSyncRequest\x1a\x1c.elastic.DdpInitSyncResponse\x12J\n\rget_comm_rank\x12\x1b.elastic.GetCommRankRequest\x1a\x1c.elastic.GetCommRankResponse\x12_\n\x1breport_training_loop_status\x12(.elastic.ReportTrainingLoopStatusRequest\x1a\x16.google.protobuf.Empty\x12\x32\n\x08get_task\x12\x17.elastic.GetTaskRequest\x1a\r.elastic.Task\x12N\n\x12report_task_result\x12 .elastic.ReportTaskResultRequest\x1a\x16.google.protobuf.Empty\x12_\n\x1breport_dataset_shard_params\x12(.elastic.ReportDatasetShardParamsRequest\x1a\x16.google.protobuf.Empty\x12K\n\x11get_dataset_epoch\x12\x14.elastic.DatasetMeta\x1a .elastic.GetDatasetEpochResponse\x12G\n\x15ready_for_ps_relaunch\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\x12\x46\n\x14get_shard_checkpoint\x12\x14.elastic.DatasetMeta\x1a\x18.elastic.ShardCheckpoint\x12[\n\x17report_shard_checkpoint\x12\x18.elastic.ShardCheckpoint\x1a&.elastic.ReportShardCheckpointResponse\x12R\n\x14report_used_resource\x12\".elastic.ReportUsedResourceRequest\x1a\x16.google.protobuf.Empty\x12\x43\n\x13report_model_metric\x12\x14.elastic.ModelMetric\x1a\x16.google.protobuf.Empty\x12G\n\x12report_global_step\x12\x19.elastic.GlobalStepRecord\x1a\x16.google.protobuf.Empty\x12\x44\n\x13query_running_nodes\x12\x16.google.protobuf.Empty\x1a\x15.elastic.RunningNodes\x12\\\n\x13get_cluster_version\x12!.elastic.GetClusterVersionRequest\x1a\".elastic.GetClusterVersionResponse\x12V\n\x16update_cluster_version\x12$.elastic.UpdateClusterVersionRequest\x1a\x16.google.protobuf.Empty\x12G\n\x0equery_ps_nodes\x12\x16.google.protobuf.Empty\x1a\x1d.elastic.QueryPsNodesResponse\x12U\n\x15query_training_status\x12\x16.google.protobuf.Empty\x1a$.elastic.QueryTrainingStatusResponse\x12J\n\x10init_remote_lock\x12\x1e.elastic.InitRemoteLockRequest\x1a\x16.google.protobuf.Empty\x12\\\n\x13\x61\x63quire_remote_lock\x12!.elastic.AcquireRemoteLockRequest\x1a\".elastic.AcquireRemoteLockResponse\x12P\n\x13release_remote_lock\x12!.elastic.ReleaseRemoteLockRequest\x1a\x16.google.protobuf.Empty\x12G\n\x0ereport_prestop\x12\x1d.elastic.ReportPreStopRequest\x1a\x16.google.protobuf.Emptyb\x06proto3')
+DESCRIPTOR = _descriptor.FileDescriptor(
+  name='dlrover/proto/elastic_training.proto',
+  package='elastic',
+  syntax='proto3',
+  serialized_options=None,
+  create_key=_descriptor._internal_create_key,
+  serialized_pb=b'\n$dlrover/proto/elastic_training.proto\x12\x07\x65lastic\x1a\x1bgoogle/protobuf/empty.proto\"B\n\x05Shard\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05start\x18\x02 \x01(\x03\x12\x0b\n\x03\x65nd\x18\x03 \x01(\x03\x12\x0f\n\x07indices\x18\x04 \x03(\x03\"\xe1\x01\n\x04Task\x12\x0f\n\x07task_id\x18\x01 \x01(\x05\x12\x1d\n\x05shard\x18\x02 \x01(\x0b\x32\x0e.elastic.Shard\x12\x15\n\rmodel_version\x18\x03 \x01(\x05\x12\x1f\n\x04type\x18\x04 \x01(\x0e\x32\x11.elastic.TaskType\x12:\n\x0f\x65xtended_config\x18\x05 \x03(\x0b\x32!.elastic.Task.ExtendedConfigEntry\x1a\x35\n\x13\x45xtendedConfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"N\n\x0eGetTaskRequest\x12\x13\n\x0bworker_type\x18\x01 \x01(\t\x12\x11\n\tworker_id\x18\x02 \x01(\x05\x12\x14\n\x0c\x64\x61taset_name\x18\x03 \x01(\t\"\xd5\x01\n\x17ReportTaskResultRequest\x12\x14\n\x0c\x64\x61taset_name\x18\x01 \x01(\t\x12\x0f\n\x07task_id\x18\x02 \x01(\x03\x12\x13\n\x0b\x65rr_message\x18\x03 \x01(\t\x12I\n\rexec_counters\x18\x04 \x03(\x0b\x32\x32.elastic.ReportTaskResultRequest.ExecCountersEntry\x1a\x33\n\x11\x45xecCountersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"\xe5\x01\n\x1fReportDatasetShardParamsRequest\x12\x12\n\nbatch_size\x18\x01 \x01(\x05\x12\x12\n\nnum_epochs\x18\x02 \x01(\x05\x12\x14\n\x0c\x64\x61taset_size\x18\x03 \x01(\x03\x12\x0f\n\x07shuffle\x18\x04 \x01(\x08\x12!\n\x19num_minibatches_per_shard\x18\x05 \x01(\x05\x12\x14\n\x0c\x64\x61taset_name\x18\x06 \x01(\t\x12$\n\ttask_type\x18\x07 \x01(\x0e\x32\x11.elastic.TaskType\x12\x14\n\x0cstorage_type\x18\x08 \x01(\t\"6\n\x0b\x44\x61tasetMeta\x12\x14\n\x0c\x64\x61taset_name\x18\x01 \x01(\t\x12\x11\n\tshard_num\x18\x02 \x01(\x05\"(\n\x17GetDatasetEpochResponse\x12\r\n\x05\x65poch\x18\x01 \x01(\x05\"\"\n\x0fShardCheckpoint\x12\x0f\n\x07\x63ontent\x18\x01 \x01(\t\"\\\n\x19ReportUsedResourceRequest\x12\x0e\n\x06memory\x18\x01 \x01(\x03\x12\x0b\n\x03\x63pu\x18\x02 \x01(\x02\x12\x0f\n\x07node_id\x18\x03 \x01(\x05\x12\x11\n\tnode_type\x18\x04 \x01(\t\"\xf9\x01\n\x0bTensorStats\x12\x16\n\x0evariable_count\x18\x01 \x01(\x03\x12\x1b\n\x13total_variable_size\x18\x02 \x01(\x03\x12\x19\n\x11max_variable_size\x18\x03 \x01(\x03\x12\x19\n\x11kv_embedding_dims\x18\x04 \x03(\x03\x12\x46\n\x12tensor_alloc_bytes\x18\x05 \x03(\x0b\x32*.elastic.TensorStats.TensorAllocBytesEntry\x1a\x37\n\x15TensorAllocBytesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x03:\x02\x38\x01\"\x91\x01\n\x0eOperationStats\x12\x10\n\x08op_count\x18\x01 \x01(\x03\x12\x17\n\x0fupdate_op_count\x18\x02 \x01(\x03\x12\x15\n\rread_op_count\x18\x03 \x01(\x03\x12\x17\n\x0finput_fetch_dur\x18\x04 \x01(\x03\x12\r\n\x05\x66lops\x18\x05 \x01(\x03\x12\x15\n\rrecv_op_count\x18\x06 \x01(\x03\"d\n\x0bModelMetric\x12*\n\x0ctensor_stats\x18\x01 \x01(\x0b\x32\x14.elastic.TensorStats\x12)\n\x08op_stats\x18\x02 \x01(\x0b\x32\x17.elastic.OperationStats\"T\n\x18GetClusterVersionRequest\x12\x0f\n\x07task_id\x18\x01 \x01(\x05\x12\x14\n\x0cversion_type\x18\x02 \x01(\t\x12\x11\n\ttask_type\x18\x03 \x01(\t\",\n\x19GetClusterVersionResponse\x12\x0f\n\x07version\x18\x01 \x01(\x05\"h\n\x1bUpdateClusterVersionRequest\x12\x0f\n\x07task_id\x18\x01 \x01(\x05\x12\x0f\n\x07version\x18\x02 \x01(\x05\x12\x14\n\x0cversion_type\x18\x03 \x01(\t\x12\x11\n\ttask_type\x18\x04 \x01(\t\"I\n\x15InitRemoteLockRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07timeout\x18\x02 \x01(\x05\x12\x11\n\tworker_id\x18\x03 \x01(\x05\"L\n\x18\x41\x63quireRemoteLockRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07timeout\x18\x02 \x01(\x05\x12\x11\n\tworker_id\x18\x03 \x01(\x05\",\n\x19\x41\x63quireRemoteLockResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"(\n\x18ReleaseRemoteLockRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\":\n\x10GlobalStepRecord\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x13\n\x0bglobal_step\x18\x02 \x01(\x03\"e\n\x14QueryPsNodesResponse\x12#\n\x08ps_nodes\x18\x01 \x03(\x0b\x32\x11.elastic.NodeMeta\x12\x14\n\x0cnew_ps_ready\x18\x02 \x01(\x08\x12\x12\n\nps_failure\x18\x03 \x01(\x08\"\x8c\x01\n\x08NodeMeta\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0c\n\x04\x61\x64\x64r\x18\x02 \x01(\t\x12\x0e\n\x06memory\x18\x03 \x01(\x05\x12\x0b\n\x03\x63pu\x18\x04 \x01(\x02\x12\x0b\n\x03gpu\x18\x05 \x01(\x05\x12\x10\n\x08gpu_type\x18\x06 \x01(\t\x12\n\n\x02id\x18\x07 \x01(\x05\x12\x0c\n\x04rank\x18\x08 \x01(\x05\x12\x0e\n\x06status\x18\t \x01(\t\"Q\n\tNodeEvent\x12\x12\n\nevent_type\x18\x01 \x01(\t\x12\x1f\n\x04node\x18\x02 \x01(\x0b\x32\x11.elastic.NodeMeta\x12\x0f\n\x07message\x18\x03 \x01(\t\"0\n\x0cRunningNodes\x12 \n\x05nodes\x18\x01 \x03(\x0b\x32\x11.elastic.NodeMeta\"-\n\x1bQueryTrainingStatusResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\":\n\x0eResourceConfig\x12\x0b\n\x03num\x18\x01 \x01(\x05\x12\x0b\n\x03\x63pu\x18\x02 \x01(\x05\x12\x0e\n\x06memory\x18\x03 \x01(\x05\"+\n\x14ReportPreStopRequest\x12\x13\n\x0bworker_host\x18\x01 \x01(\t\"H\n\x0bSyncRequest\x12\x11\n\tsync_name\x18\x01 \x01(\t\x12\x11\n\tworker_id\x18\x02 \x01(\x05\x12\x13\n\x0bworker_type\x18\x03 \x01(\t\"6\n\x0e\x42\x61rrierRequest\x12\x14\n\x0c\x62\x61rrier_name\x18\x01 \x01(\t\x12\x0e\n\x06notify\x18\x03 \x01(\x08\"\xa6\x01\n\x0fRendezvousState\x12\x32\n\x05world\x18\x01 \x03(\x0b\x32#.elastic.RendezvousState.WorldEntry\x12\x13\n\x0bwaiting_num\x18\x02 \x01(\x05\x12\r\n\x05round\x18\x03 \x01(\x05\x12\r\n\x05group\x18\x04 \x01(\x05\x1a,\n\nWorldEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"Q\n\x11RendezvousRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\x05\x12\x18\n\x10local_world_size\x18\x02 \x01(\x05\x12\x11\n\trdzv_name\x18\x04 \x01(\t\"d\n\x10RendezvousParams\x12\x11\n\tmin_nodes\x18\x01 \x01(\x05\x12\x11\n\tmax_nodes\x18\x02 \x01(\x05\x12\x17\n\x0fwaiting_timeout\x18\x03 \x01(\x05\x12\x11\n\tnode_unit\x18\x04 \x01(\x05\"*\n\x0cKeyValuePair\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c\"+\n\x08Response\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x0e\n\x06reason\x18\x02 \x01(\t\"\\\n\x0bNodeFailure\x12\x0f\n\x07node_id\x18\x01 \x01(\x05\x12\x11\n\tnode_type\x18\x02 \x01(\t\x12\x12\n\nerror_data\x18\x03 \x01(\t\x12\x15\n\rrestart_count\x18\x04 \x01(\x05*d\n\x08TaskType\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08TRAINING\x10\x01\x12\x0e\n\nEVALUATION\x10\x02\x12\x0e\n\nPREDICTION\x10\x03\x12\x08\n\x04WAIT\x10\x04\x12\x16\n\x12TRAIN_END_CALLBACK\x10\x05\x32\xda\x12\n\x06Master\x12\x32\n\x08get_task\x12\x17.elastic.GetTaskRequest\x1a\r.elastic.Task\x12N\n\x12report_task_result\x12 .elastic.ReportTaskResultRequest\x1a\x16.google.protobuf.Empty\x12_\n\x1breport_dataset_shard_params\x12(.elastic.ReportDatasetShardParamsRequest\x1a\x16.google.protobuf.Empty\x12K\n\x11get_dataset_epoch\x12\x14.elastic.DatasetMeta\x1a .elastic.GetDatasetEpochResponse\x12\x43\n\x15get_dataset_shard_num\x12\x14.elastic.DatasetMeta\x1a\x14.elastic.DatasetMeta\x12\x46\n\x14get_shard_checkpoint\x12\x14.elastic.DatasetMeta\x1a\x18.elastic.ShardCheckpoint\x12\x46\n\x17report_shard_checkpoint\x12\x18.elastic.ShardCheckpoint\x1a\x11.elastic.Response\x12R\n\x14report_used_resource\x12\".elastic.ReportUsedResourceRequest\x1a\x16.google.protobuf.Empty\x12\x43\n\x13report_model_metric\x12\x14.elastic.ModelMetric\x1a\x16.google.protobuf.Empty\x12G\n\x12report_global_step\x12\x19.elastic.GlobalStepRecord\x1a\x16.google.protobuf.Empty\x12\x34\n\tjoin_sync\x12\x14.elastic.SyncRequest\x1a\x11.elastic.Response\x12\x38\n\rsync_finished\x12\x14.elastic.SyncRequest\x1a\x11.elastic.Response\x12\x35\n\x07\x62\x61rrier\x12\x17.elastic.BarrierRequest\x1a\x11.elastic.Response\x12\\\n\x13get_cluster_version\x12!.elastic.GetClusterVersionRequest\x1a\".elastic.GetClusterVersionResponse\x12V\n\x16update_cluster_version\x12$.elastic.UpdateClusterVersionRequest\x1a\x16.google.protobuf.Empty\x12G\n\x0equery_ps_nodes\x12\x16.google.protobuf.Empty\x1a\x1d.elastic.QueryPsNodesResponse\x12U\n\x15query_training_status\x12\x16.google.protobuf.Empty\x1a$.elastic.QueryTrainingStatusResponse\x12\x44\n\x13query_running_nodes\x12\x16.google.protobuf.Empty\x1a\x15.elastic.RunningNodes\x12G\n\x15ready_for_ps_relaunch\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\x12J\n\x10init_remote_lock\x12\x1e.elastic.InitRemoteLockRequest\x1a\x16.google.protobuf.Empty\x12\\\n\x13\x61\x63quire_remote_lock\x12!.elastic.AcquireRemoteLockRequest\x1a\".elastic.AcquireRemoteLockResponse\x12P\n\x13release_remote_lock\x12!.elastic.ReleaseRemoteLockRequest\x1a\x16.google.protobuf.Empty\x12\x46\n\x0eget_comm_world\x12\x1a.elastic.RendezvousRequest\x1a\x18.elastic.RendezvousState\x12G\n\x0fjoin_rendezvous\x12\x1a.elastic.RendezvousRequest\x1a\x18.elastic.RendezvousState\x12I\n\x11num_nodes_waiting\x12\x1a.elastic.RendezvousRequest\x1a\x18.elastic.RendezvousState\x12\x42\n\x12report_rdzv_params\x12\x19.elastic.RendezvousParams\x1a\x11.elastic.Response\x12\x38\n\x0ckv_store_set\x12\x15.elastic.KeyValuePair\x1a\x11.elastic.Response\x12<\n\x0ckv_store_get\x12\x15.elastic.KeyValuePair\x1a\x15.elastic.KeyValuePair\x12\x39\n\x0ereport_failure\x12\x14.elastic.NodeFailure\x1a\x11.elastic.Response\x12\x46\n\x15network_check_success\x12\x1a.elastic.RendezvousRequest\x1a\x11.elastic.Response\x12G\n\x0ereport_prestop\x12\x1d.elastic.ReportPreStopRequest\x1a\x16.google.protobuf.Empty\x12:\n\x12update_node_status\x12\x11.elastic.NodeMeta\x1a\x11.elastic.Response\x12?\n\x11update_node_event\x12\x12.elastic.NodeEvent\x1a\x16.google.protobuf.Emptyb\x06proto3'
+  ,
+  dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,])
+
+_TASKTYPE = _descriptor.EnumDescriptor(
+  name='TaskType',
+  full_name='elastic.TaskType',
+  filename=None,
+  file=DESCRIPTOR,
+  create_key=_descriptor._internal_create_key,
+  values=[
+    _descriptor.EnumValueDescriptor(
+      name='NONE', index=0, number=0,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='TRAINING', index=1, number=1,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='EVALUATION', index=2, number=2,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='PREDICTION', index=3, number=3,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='WAIT', index=4, number=4,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='TRAIN_END_CALLBACK', index=5, number=5,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+  ],
+  containing_type=None,
+  serialized_options=None,
+  serialized_start=3369,
+  serialized_end=3469,
+)
+_sym_db.RegisterEnumDescriptor(_TASKTYPE)
 
-_TASKTYPE = DESCRIPTOR.enum_types_by_name['TaskType']
 TaskType = enum_type_wrapper.EnumTypeWrapper(_TASKTYPE)
 NONE = 0
 TRAINING = 1
 EVALUATION = 2
 PREDICTION = 3
 WAIT = 4
 TRAIN_END_CALLBACK = 5
 
 
-_SHARD = DESCRIPTOR.message_types_by_name['Shard']
-_TASK = DESCRIPTOR.message_types_by_name['Task']
-_TASK_EXTENDEDCONFIGENTRY = _TASK.nested_types_by_name['ExtendedConfigEntry']
-_GETTASKREQUEST = DESCRIPTOR.message_types_by_name['GetTaskRequest']
-_REPORTTASKRESULTREQUEST = DESCRIPTOR.message_types_by_name['ReportTaskResultRequest']
-_REPORTTASKRESULTREQUEST_EXECCOUNTERSENTRY = _REPORTTASKRESULTREQUEST.nested_types_by_name['ExecCountersEntry']
-_REPORTDATASETSHARDPARAMSREQUEST = DESCRIPTOR.message_types_by_name['ReportDatasetShardParamsRequest']
-_DATASETMETA = DESCRIPTOR.message_types_by_name['DatasetMeta']
-_GETDATASETEPOCHRESPONSE = DESCRIPTOR.message_types_by_name['GetDatasetEpochResponse']
-_DDPRESETSYNCREQUEST = DESCRIPTOR.message_types_by_name['DdpResetSyncRequest']
-_DDPRESETSYNCRESPONSE = DESCRIPTOR.message_types_by_name['DdpResetSyncResponse']
-_DDPINITSYNCREQUEST = DESCRIPTOR.message_types_by_name['DdpInitSyncRequest']
-_DDPINITSYNCRESPONSE = DESCRIPTOR.message_types_by_name['DdpInitSyncResponse']
-_GETCOMMRANKREQUEST = DESCRIPTOR.message_types_by_name['GetCommRankRequest']
-_GETCOMMRANKRESPONSE = DESCRIPTOR.message_types_by_name['GetCommRankResponse']
-_REPORTTRAININGLOOPSTATUSREQUEST = DESCRIPTOR.message_types_by_name['ReportTrainingLoopStatusRequest']
-_SHARDCHECKPOINT = DESCRIPTOR.message_types_by_name['ShardCheckpoint']
-_REPORTSHARDCHECKPOINTRESPONSE = DESCRIPTOR.message_types_by_name['ReportShardCheckpointResponse']
-_REPORTUSEDRESOURCEREQUEST = DESCRIPTOR.message_types_by_name['ReportUsedResourceRequest']
-_TENSORSTATS = DESCRIPTOR.message_types_by_name['TensorStats']
-_TENSORSTATS_TENSORALLOCBYTESENTRY = _TENSORSTATS.nested_types_by_name['TensorAllocBytesEntry']
-_OPERATIONSTATS = DESCRIPTOR.message_types_by_name['OperationStats']
-_MODELMETRIC = DESCRIPTOR.message_types_by_name['ModelMetric']
-_GETCLUSTERVERSIONREQUEST = DESCRIPTOR.message_types_by_name['GetClusterVersionRequest']
-_GETCLUSTERVERSIONRESPONSE = DESCRIPTOR.message_types_by_name['GetClusterVersionResponse']
-_UPDATECLUSTERVERSIONREQUEST = DESCRIPTOR.message_types_by_name['UpdateClusterVersionRequest']
-_INITREMOTELOCKREQUEST = DESCRIPTOR.message_types_by_name['InitRemoteLockRequest']
-_ACQUIREREMOTELOCKREQUEST = DESCRIPTOR.message_types_by_name['AcquireRemoteLockRequest']
-_ACQUIREREMOTELOCKRESPONSE = DESCRIPTOR.message_types_by_name['AcquireRemoteLockResponse']
-_RELEASEREMOTELOCKREQUEST = DESCRIPTOR.message_types_by_name['ReleaseRemoteLockRequest']
-_GLOBALSTEPRECORD = DESCRIPTOR.message_types_by_name['GlobalStepRecord']
-_QUERYPSNODESRESPONSE = DESCRIPTOR.message_types_by_name['QueryPsNodesResponse']
-_NODEMETA = DESCRIPTOR.message_types_by_name['NodeMeta']
-_RUNNINGNODES = DESCRIPTOR.message_types_by_name['RunningNodes']
-_QUERYTRAININGSTATUSRESPONSE = DESCRIPTOR.message_types_by_name['QueryTrainingStatusResponse']
-_RESOURCECONFIG = DESCRIPTOR.message_types_by_name['ResourceConfig']
-_REPORTPRESTOPREQUEST = DESCRIPTOR.message_types_by_name['ReportPreStopRequest']
+
+_SHARD = _descriptor.Descriptor(
+  name='Shard',
+  full_name='elastic.Shard',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='name', full_name='elastic.Shard.name', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='start', full_name='elastic.Shard.start', index=1,
+      number=2, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='end', full_name='elastic.Shard.end', index=2,
+      number=3, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='indices', full_name='elastic.Shard.indices', index=3,
+      number=4, type=3, cpp_type=2, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=78,
+  serialized_end=144,
+)
+
+
+_TASK_EXTENDEDCONFIGENTRY = _descriptor.Descriptor(
+  name='ExtendedConfigEntry',
+  full_name='elastic.Task.ExtendedConfigEntry',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='key', full_name='elastic.Task.ExtendedConfigEntry.key', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='value', full_name='elastic.Task.ExtendedConfigEntry.value', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=b'8\001',
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=319,
+  serialized_end=372,
+)
+
+_TASK = _descriptor.Descriptor(
+  name='Task',
+  full_name='elastic.Task',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='task_id', full_name='elastic.Task.task_id', index=0,
+      number=1, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='shard', full_name='elastic.Task.shard', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='model_version', full_name='elastic.Task.model_version', index=2,
+      number=3, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='type', full_name='elastic.Task.type', index=3,
+      number=4, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='extended_config', full_name='elastic.Task.extended_config', index=4,
+      number=5, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[_TASK_EXTENDEDCONFIGENTRY, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=147,
+  serialized_end=372,
+)
+
+
+_GETTASKREQUEST = _descriptor.Descriptor(
+  name='GetTaskRequest',
+  full_name='elastic.GetTaskRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='worker_type', full_name='elastic.GetTaskRequest.worker_type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='worker_id', full_name='elastic.GetTaskRequest.worker_id', index=1,
+      number=2, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='dataset_name', full_name='elastic.GetTaskRequest.dataset_name', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=374,
+  serialized_end=452,
+)
+
+
+_REPORTTASKRESULTREQUEST_EXECCOUNTERSENTRY = _descriptor.Descriptor(
+  name='ExecCountersEntry',
+  full_name='elastic.ReportTaskResultRequest.ExecCountersEntry',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='key', full_name='elastic.ReportTaskResultRequest.ExecCountersEntry.key', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='value', full_name='elastic.ReportTaskResultRequest.ExecCountersEntry.value', index=1,
+      number=2, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=b'8\001',
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=617,
+  serialized_end=668,
+)
+
+_REPORTTASKRESULTREQUEST = _descriptor.Descriptor(
+  name='ReportTaskResultRequest',
+  full_name='elastic.ReportTaskResultRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='dataset_name', full_name='elastic.ReportTaskResultRequest.dataset_name', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='task_id', full_name='elastic.ReportTaskResultRequest.task_id', index=1,
+      number=2, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='err_message', full_name='elastic.ReportTaskResultRequest.err_message', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='exec_counters', full_name='elastic.ReportTaskResultRequest.exec_counters', index=3,
+      number=4, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[_REPORTTASKRESULTREQUEST_EXECCOUNTERSENTRY, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=455,
+  serialized_end=668,
+)
+
+
+_REPORTDATASETSHARDPARAMSREQUEST = _descriptor.Descriptor(
+  name='ReportDatasetShardParamsRequest',
+  full_name='elastic.ReportDatasetShardParamsRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='batch_size', full_name='elastic.ReportDatasetShardParamsRequest.batch_size', index=0,
+      number=1, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='num_epochs', full_name='elastic.ReportDatasetShardParamsRequest.num_epochs', index=1,
+      number=2, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='dataset_size', full_name='elastic.ReportDatasetShardParamsRequest.dataset_size', index=2,
+      number=3, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='shuffle', full_name='elastic.ReportDatasetShardParamsRequest.shuffle', index=3,
+      number=4, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='num_minibatches_per_shard', full_name='elastic.ReportDatasetShardParamsRequest.num_minibatches_per_shard', index=4,
+      number=5, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='dataset_name', full_name='elastic.ReportDatasetShardParamsRequest.dataset_name', index=5,
+      number=6, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='task_type', full_name='elastic.ReportDatasetShardParamsRequest.task_type', index=6,
+      number=7, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='storage_type', full_name='elastic.ReportDatasetShardParamsRequest.storage_type', index=7,
+      number=8, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=671,
+  serialized_end=900,
+)
+
+
+_DATASETMETA = _descriptor.Descriptor(
+  name='DatasetMeta',
+  full_name='elastic.DatasetMeta',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='dataset_name', full_name='elastic.DatasetMeta.dataset_name', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='shard_num', full_name='elastic.DatasetMeta.shard_num', index=1,
+      number=2, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=902,
+  serialized_end=956,
+)
+
+
+_GETDATASETEPOCHRESPONSE = _descriptor.Descriptor(
+  name='GetDatasetEpochResponse',
+  full_name='elastic.GetDatasetEpochResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='epoch', full_name='elastic.GetDatasetEpochResponse.epoch', index=0,
+      number=1, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=958,
+  serialized_end=998,
+)
+
+
+_SHARDCHECKPOINT = _descriptor.Descriptor(
+  name='ShardCheckpoint',
+  full_name='elastic.ShardCheckpoint',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='content', full_name='elastic.ShardCheckpoint.content', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1000,
+  serialized_end=1034,
+)
+
+
+_REPORTUSEDRESOURCEREQUEST = _descriptor.Descriptor(
+  name='ReportUsedResourceRequest',
+  full_name='elastic.ReportUsedResourceRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='memory', full_name='elastic.ReportUsedResourceRequest.memory', index=0,
+      number=1, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='cpu', full_name='elastic.ReportUsedResourceRequest.cpu', index=1,
+      number=2, type=2, cpp_type=6, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='node_id', full_name='elastic.ReportUsedResourceRequest.node_id', index=2,
+      number=3, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='node_type', full_name='elastic.ReportUsedResourceRequest.node_type', index=3,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1036,
+  serialized_end=1128,
+)
+
+
+_TENSORSTATS_TENSORALLOCBYTESENTRY = _descriptor.Descriptor(
+  name='TensorAllocBytesEntry',
+  full_name='elastic.TensorStats.TensorAllocBytesEntry',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='key', full_name='elastic.TensorStats.TensorAllocBytesEntry.key', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='value', full_name='elastic.TensorStats.TensorAllocBytesEntry.value', index=1,
+      number=2, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=b'8\001',
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1325,
+  serialized_end=1380,
+)
+
+_TENSORSTATS = _descriptor.Descriptor(
+  name='TensorStats',
+  full_name='elastic.TensorStats',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='variable_count', full_name='elastic.TensorStats.variable_count', index=0,
+      number=1, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='total_variable_size', full_name='elastic.TensorStats.total_variable_size', index=1,
+      number=2, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='max_variable_size', full_name='elastic.TensorStats.max_variable_size', index=2,
+      number=3, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='kv_embedding_dims', full_name='elastic.TensorStats.kv_embedding_dims', index=3,
+      number=4, type=3, cpp_type=2, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='tensor_alloc_bytes', full_name='elastic.TensorStats.tensor_alloc_bytes', index=4,
+      number=5, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[_TENSORSTATS_TENSORALLOCBYTESENTRY, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1131,
+  serialized_end=1380,
+)
+
+
+_OPERATIONSTATS = _descriptor.Descriptor(
+  name='OperationStats',
+  full_name='elastic.OperationStats',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='op_count', full_name='elastic.OperationStats.op_count', index=0,
+      number=1, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='update_op_count', full_name='elastic.OperationStats.update_op_count', index=1,
+      number=2, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='read_op_count', full_name='elastic.OperationStats.read_op_count', index=2,
+      number=3, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='input_fetch_dur', full_name='elastic.OperationStats.input_fetch_dur', index=3,
+      number=4, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='flops', full_name='elastic.OperationStats.flops', index=4,
+      number=5, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='recv_op_count', full_name='elastic.OperationStats.recv_op_count', index=5,
+      number=6, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1383,
+  serialized_end=1528,
+)
+
+
+_MODELMETRIC = _descriptor.Descriptor(
+  name='ModelMetric',
+  full_name='elastic.ModelMetric',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='tensor_stats', full_name='elastic.ModelMetric.tensor_stats', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='op_stats', full_name='elastic.ModelMetric.op_stats', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1530,
+  serialized_end=1630,
+)
+
+
+_GETCLUSTERVERSIONREQUEST = _descriptor.Descriptor(
+  name='GetClusterVersionRequest',
+  full_name='elastic.GetClusterVersionRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='task_id', full_name='elastic.GetClusterVersionRequest.task_id', index=0,
+      number=1, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='version_type', full_name='elastic.GetClusterVersionRequest.version_type', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='task_type', full_name='elastic.GetClusterVersionRequest.task_type', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1632,
+  serialized_end=1716,
+)
+
+
+_GETCLUSTERVERSIONRESPONSE = _descriptor.Descriptor(
+  name='GetClusterVersionResponse',
+  full_name='elastic.GetClusterVersionResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='version', full_name='elastic.GetClusterVersionResponse.version', index=0,
+      number=1, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1718,
+  serialized_end=1762,
+)
+
+
+_UPDATECLUSTERVERSIONREQUEST = _descriptor.Descriptor(
+  name='UpdateClusterVersionRequest',
+  full_name='elastic.UpdateClusterVersionRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='task_id', full_name='elastic.UpdateClusterVersionRequest.task_id', index=0,
+      number=1, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='version', full_name='elastic.UpdateClusterVersionRequest.version', index=1,
+      number=2, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='version_type', full_name='elastic.UpdateClusterVersionRequest.version_type', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='task_type', full_name='elastic.UpdateClusterVersionRequest.task_type', index=3,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1764,
+  serialized_end=1868,
+)
+
+
+_INITREMOTELOCKREQUEST = _descriptor.Descriptor(
+  name='InitRemoteLockRequest',
+  full_name='elastic.InitRemoteLockRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='name', full_name='elastic.InitRemoteLockRequest.name', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='timeout', full_name='elastic.InitRemoteLockRequest.timeout', index=1,
+      number=2, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='worker_id', full_name='elastic.InitRemoteLockRequest.worker_id', index=2,
+      number=3, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1870,
+  serialized_end=1943,
+)
+
+
+_ACQUIREREMOTELOCKREQUEST = _descriptor.Descriptor(
+  name='AcquireRemoteLockRequest',
+  full_name='elastic.AcquireRemoteLockRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='name', full_name='elastic.AcquireRemoteLockRequest.name', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='timeout', full_name='elastic.AcquireRemoteLockRequest.timeout', index=1,
+      number=2, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='worker_id', full_name='elastic.AcquireRemoteLockRequest.worker_id', index=2,
+      number=3, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1945,
+  serialized_end=2021,
+)
+
+
+_ACQUIREREMOTELOCKRESPONSE = _descriptor.Descriptor(
+  name='AcquireRemoteLockResponse',
+  full_name='elastic.AcquireRemoteLockResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='success', full_name='elastic.AcquireRemoteLockResponse.success', index=0,
+      number=1, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2023,
+  serialized_end=2067,
+)
+
+
+_RELEASEREMOTELOCKREQUEST = _descriptor.Descriptor(
+  name='ReleaseRemoteLockRequest',
+  full_name='elastic.ReleaseRemoteLockRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='name', full_name='elastic.ReleaseRemoteLockRequest.name', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2069,
+  serialized_end=2109,
+)
+
+
+_GLOBALSTEPRECORD = _descriptor.Descriptor(
+  name='GlobalStepRecord',
+  full_name='elastic.GlobalStepRecord',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='timestamp', full_name='elastic.GlobalStepRecord.timestamp', index=0,
+      number=1, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='global_step', full_name='elastic.GlobalStepRecord.global_step', index=1,
+      number=2, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2111,
+  serialized_end=2169,
+)
+
+
+_QUERYPSNODESRESPONSE = _descriptor.Descriptor(
+  name='QueryPsNodesResponse',
+  full_name='elastic.QueryPsNodesResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='ps_nodes', full_name='elastic.QueryPsNodesResponse.ps_nodes', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='new_ps_ready', full_name='elastic.QueryPsNodesResponse.new_ps_ready', index=1,
+      number=2, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='ps_failure', full_name='elastic.QueryPsNodesResponse.ps_failure', index=2,
+      number=3, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2171,
+  serialized_end=2272,
+)
+
+
+_NODEMETA = _descriptor.Descriptor(
+  name='NodeMeta',
+  full_name='elastic.NodeMeta',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='elastic.NodeMeta.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='addr', full_name='elastic.NodeMeta.addr', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='memory', full_name='elastic.NodeMeta.memory', index=2,
+      number=3, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='cpu', full_name='elastic.NodeMeta.cpu', index=3,
+      number=4, type=2, cpp_type=6, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='gpu', full_name='elastic.NodeMeta.gpu', index=4,
+      number=5, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='gpu_type', full_name='elastic.NodeMeta.gpu_type', index=5,
+      number=6, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='id', full_name='elastic.NodeMeta.id', index=6,
+      number=7, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='rank', full_name='elastic.NodeMeta.rank', index=7,
+      number=8, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='status', full_name='elastic.NodeMeta.status', index=8,
+      number=9, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2275,
+  serialized_end=2415,
+)
+
+
+_NODEEVENT = _descriptor.Descriptor(
+  name='NodeEvent',
+  full_name='elastic.NodeEvent',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='event_type', full_name='elastic.NodeEvent.event_type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='node', full_name='elastic.NodeEvent.node', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='message', full_name='elastic.NodeEvent.message', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2417,
+  serialized_end=2498,
+)
+
+
+_RUNNINGNODES = _descriptor.Descriptor(
+  name='RunningNodes',
+  full_name='elastic.RunningNodes',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='nodes', full_name='elastic.RunningNodes.nodes', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2500,
+  serialized_end=2548,
+)
+
+
+_QUERYTRAININGSTATUSRESPONSE = _descriptor.Descriptor(
+  name='QueryTrainingStatusResponse',
+  full_name='elastic.QueryTrainingStatusResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='status', full_name='elastic.QueryTrainingStatusResponse.status', index=0,
+      number=1, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2550,
+  serialized_end=2595,
+)
+
+
+_RESOURCECONFIG = _descriptor.Descriptor(
+  name='ResourceConfig',
+  full_name='elastic.ResourceConfig',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='num', full_name='elastic.ResourceConfig.num', index=0,
+      number=1, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='cpu', full_name='elastic.ResourceConfig.cpu', index=1,
+      number=2, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='memory', full_name='elastic.ResourceConfig.memory', index=2,
+      number=3, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2597,
+  serialized_end=2655,
+)
+
+
+_REPORTPRESTOPREQUEST = _descriptor.Descriptor(
+  name='ReportPreStopRequest',
+  full_name='elastic.ReportPreStopRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='worker_host', full_name='elastic.ReportPreStopRequest.worker_host', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2657,
+  serialized_end=2700,
+)
+
+
+_SYNCREQUEST = _descriptor.Descriptor(
+  name='SyncRequest',
+  full_name='elastic.SyncRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='sync_name', full_name='elastic.SyncRequest.sync_name', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='worker_id', full_name='elastic.SyncRequest.worker_id', index=1,
+      number=2, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='worker_type', full_name='elastic.SyncRequest.worker_type', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2702,
+  serialized_end=2774,
+)
+
+
+_BARRIERREQUEST = _descriptor.Descriptor(
+  name='BarrierRequest',
+  full_name='elastic.BarrierRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='barrier_name', full_name='elastic.BarrierRequest.barrier_name', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='notify', full_name='elastic.BarrierRequest.notify', index=1,
+      number=3, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2776,
+  serialized_end=2830,
+)
+
+
+_RENDEZVOUSSTATE_WORLDENTRY = _descriptor.Descriptor(
+  name='WorldEntry',
+  full_name='elastic.RendezvousState.WorldEntry',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='key', full_name='elastic.RendezvousState.WorldEntry.key', index=0,
+      number=1, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='value', full_name='elastic.RendezvousState.WorldEntry.value', index=1,
+      number=2, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=b'8\001',
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2955,
+  serialized_end=2999,
+)
+
+_RENDEZVOUSSTATE = _descriptor.Descriptor(
+  name='RendezvousState',
+  full_name='elastic.RendezvousState',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='world', full_name='elastic.RendezvousState.world', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='waiting_num', full_name='elastic.RendezvousState.waiting_num', index=1,
+      number=2, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='round', full_name='elastic.RendezvousState.round', index=2,
+      number=3, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='group', full_name='elastic.RendezvousState.group', index=3,
+      number=4, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[_RENDEZVOUSSTATE_WORLDENTRY, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2833,
+  serialized_end=2999,
+)
+
+
+_RENDEZVOUSREQUEST = _descriptor.Descriptor(
+  name='RendezvousRequest',
+  full_name='elastic.RendezvousRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='node_id', full_name='elastic.RendezvousRequest.node_id', index=0,
+      number=1, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='local_world_size', full_name='elastic.RendezvousRequest.local_world_size', index=1,
+      number=2, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='rdzv_name', full_name='elastic.RendezvousRequest.rdzv_name', index=2,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3001,
+  serialized_end=3082,
+)
+
+
+_RENDEZVOUSPARAMS = _descriptor.Descriptor(
+  name='RendezvousParams',
+  full_name='elastic.RendezvousParams',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='min_nodes', full_name='elastic.RendezvousParams.min_nodes', index=0,
+      number=1, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='max_nodes', full_name='elastic.RendezvousParams.max_nodes', index=1,
+      number=2, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='waiting_timeout', full_name='elastic.RendezvousParams.waiting_timeout', index=2,
+      number=3, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='node_unit', full_name='elastic.RendezvousParams.node_unit', index=3,
+      number=4, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3084,
+  serialized_end=3184,
+)
+
+
+_KEYVALUEPAIR = _descriptor.Descriptor(
+  name='KeyValuePair',
+  full_name='elastic.KeyValuePair',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='key', full_name='elastic.KeyValuePair.key', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='value', full_name='elastic.KeyValuePair.value', index=1,
+      number=2, type=12, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"",
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3186,
+  serialized_end=3228,
+)
+
+
+_RESPONSE = _descriptor.Descriptor(
+  name='Response',
+  full_name='elastic.Response',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='success', full_name='elastic.Response.success', index=0,
+      number=1, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='reason', full_name='elastic.Response.reason', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3230,
+  serialized_end=3273,
+)
+
+
+_NODEFAILURE = _descriptor.Descriptor(
+  name='NodeFailure',
+  full_name='elastic.NodeFailure',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='node_id', full_name='elastic.NodeFailure.node_id', index=0,
+      number=1, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='node_type', full_name='elastic.NodeFailure.node_type', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='error_data', full_name='elastic.NodeFailure.error_data', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='restart_count', full_name='elastic.NodeFailure.restart_count', index=3,
+      number=4, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3275,
+  serialized_end=3367,
+)
+
+_TASK_EXTENDEDCONFIGENTRY.containing_type = _TASK
+_TASK.fields_by_name['shard'].message_type = _SHARD
+_TASK.fields_by_name['type'].enum_type = _TASKTYPE
+_TASK.fields_by_name['extended_config'].message_type = _TASK_EXTENDEDCONFIGENTRY
+_REPORTTASKRESULTREQUEST_EXECCOUNTERSENTRY.containing_type = _REPORTTASKRESULTREQUEST
+_REPORTTASKRESULTREQUEST.fields_by_name['exec_counters'].message_type = _REPORTTASKRESULTREQUEST_EXECCOUNTERSENTRY
+_REPORTDATASETSHARDPARAMSREQUEST.fields_by_name['task_type'].enum_type = _TASKTYPE
+_TENSORSTATS_TENSORALLOCBYTESENTRY.containing_type = _TENSORSTATS
+_TENSORSTATS.fields_by_name['tensor_alloc_bytes'].message_type = _TENSORSTATS_TENSORALLOCBYTESENTRY
+_MODELMETRIC.fields_by_name['tensor_stats'].message_type = _TENSORSTATS
+_MODELMETRIC.fields_by_name['op_stats'].message_type = _OPERATIONSTATS
+_QUERYPSNODESRESPONSE.fields_by_name['ps_nodes'].message_type = _NODEMETA
+_NODEEVENT.fields_by_name['node'].message_type = _NODEMETA
+_RUNNINGNODES.fields_by_name['nodes'].message_type = _NODEMETA
+_RENDEZVOUSSTATE_WORLDENTRY.containing_type = _RENDEZVOUSSTATE
+_RENDEZVOUSSTATE.fields_by_name['world'].message_type = _RENDEZVOUSSTATE_WORLDENTRY
+DESCRIPTOR.message_types_by_name['Shard'] = _SHARD
+DESCRIPTOR.message_types_by_name['Task'] = _TASK
+DESCRIPTOR.message_types_by_name['GetTaskRequest'] = _GETTASKREQUEST
+DESCRIPTOR.message_types_by_name['ReportTaskResultRequest'] = _REPORTTASKRESULTREQUEST
+DESCRIPTOR.message_types_by_name['ReportDatasetShardParamsRequest'] = _REPORTDATASETSHARDPARAMSREQUEST
+DESCRIPTOR.message_types_by_name['DatasetMeta'] = _DATASETMETA
+DESCRIPTOR.message_types_by_name['GetDatasetEpochResponse'] = _GETDATASETEPOCHRESPONSE
+DESCRIPTOR.message_types_by_name['ShardCheckpoint'] = _SHARDCHECKPOINT
+DESCRIPTOR.message_types_by_name['ReportUsedResourceRequest'] = _REPORTUSEDRESOURCEREQUEST
+DESCRIPTOR.message_types_by_name['TensorStats'] = _TENSORSTATS
+DESCRIPTOR.message_types_by_name['OperationStats'] = _OPERATIONSTATS
+DESCRIPTOR.message_types_by_name['ModelMetric'] = _MODELMETRIC
+DESCRIPTOR.message_types_by_name['GetClusterVersionRequest'] = _GETCLUSTERVERSIONREQUEST
+DESCRIPTOR.message_types_by_name['GetClusterVersionResponse'] = _GETCLUSTERVERSIONRESPONSE
+DESCRIPTOR.message_types_by_name['UpdateClusterVersionRequest'] = _UPDATECLUSTERVERSIONREQUEST
+DESCRIPTOR.message_types_by_name['InitRemoteLockRequest'] = _INITREMOTELOCKREQUEST
+DESCRIPTOR.message_types_by_name['AcquireRemoteLockRequest'] = _ACQUIREREMOTELOCKREQUEST
+DESCRIPTOR.message_types_by_name['AcquireRemoteLockResponse'] = _ACQUIREREMOTELOCKRESPONSE
+DESCRIPTOR.message_types_by_name['ReleaseRemoteLockRequest'] = _RELEASEREMOTELOCKREQUEST
+DESCRIPTOR.message_types_by_name['GlobalStepRecord'] = _GLOBALSTEPRECORD
+DESCRIPTOR.message_types_by_name['QueryPsNodesResponse'] = _QUERYPSNODESRESPONSE
+DESCRIPTOR.message_types_by_name['NodeMeta'] = _NODEMETA
+DESCRIPTOR.message_types_by_name['NodeEvent'] = _NODEEVENT
+DESCRIPTOR.message_types_by_name['RunningNodes'] = _RUNNINGNODES
+DESCRIPTOR.message_types_by_name['QueryTrainingStatusResponse'] = _QUERYTRAININGSTATUSRESPONSE
+DESCRIPTOR.message_types_by_name['ResourceConfig'] = _RESOURCECONFIG
+DESCRIPTOR.message_types_by_name['ReportPreStopRequest'] = _REPORTPRESTOPREQUEST
+DESCRIPTOR.message_types_by_name['SyncRequest'] = _SYNCREQUEST
+DESCRIPTOR.message_types_by_name['BarrierRequest'] = _BARRIERREQUEST
+DESCRIPTOR.message_types_by_name['RendezvousState'] = _RENDEZVOUSSTATE
+DESCRIPTOR.message_types_by_name['RendezvousRequest'] = _RENDEZVOUSREQUEST
+DESCRIPTOR.message_types_by_name['RendezvousParams'] = _RENDEZVOUSPARAMS
+DESCRIPTOR.message_types_by_name['KeyValuePair'] = _KEYVALUEPAIR
+DESCRIPTOR.message_types_by_name['Response'] = _RESPONSE
+DESCRIPTOR.message_types_by_name['NodeFailure'] = _NODEFAILURE
+DESCRIPTOR.enum_types_by_name['TaskType'] = _TASKTYPE
+_sym_db.RegisterFileDescriptor(DESCRIPTOR)
+
 Shard = _reflection.GeneratedProtocolMessageType('Shard', (_message.Message,), {
   'DESCRIPTOR' : _SHARD,
   '__module__' : 'dlrover.proto.elastic_training_pb2'
   # @@protoc_insertion_point(class_scope:elastic.Shard)
   })
 _sym_db.RegisterMessage(Shard)
 
@@ -126,77 +1977,21 @@
 GetDatasetEpochResponse = _reflection.GeneratedProtocolMessageType('GetDatasetEpochResponse', (_message.Message,), {
   'DESCRIPTOR' : _GETDATASETEPOCHRESPONSE,
   '__module__' : 'dlrover.proto.elastic_training_pb2'
   # @@protoc_insertion_point(class_scope:elastic.GetDatasetEpochResponse)
   })
 _sym_db.RegisterMessage(GetDatasetEpochResponse)
 
-DdpResetSyncRequest = _reflection.GeneratedProtocolMessageType('DdpResetSyncRequest', (_message.Message,), {
-  'DESCRIPTOR' : _DDPRESETSYNCREQUEST,
-  '__module__' : 'dlrover.proto.elastic_training_pb2'
-  # @@protoc_insertion_point(class_scope:elastic.DdpResetSyncRequest)
-  })
-_sym_db.RegisterMessage(DdpResetSyncRequest)
-
-DdpResetSyncResponse = _reflection.GeneratedProtocolMessageType('DdpResetSyncResponse', (_message.Message,), {
-  'DESCRIPTOR' : _DDPRESETSYNCRESPONSE,
-  '__module__' : 'dlrover.proto.elastic_training_pb2'
-  # @@protoc_insertion_point(class_scope:elastic.DdpResetSyncResponse)
-  })
-_sym_db.RegisterMessage(DdpResetSyncResponse)
-
-DdpInitSyncRequest = _reflection.GeneratedProtocolMessageType('DdpInitSyncRequest', (_message.Message,), {
-  'DESCRIPTOR' : _DDPINITSYNCREQUEST,
-  '__module__' : 'dlrover.proto.elastic_training_pb2'
-  # @@protoc_insertion_point(class_scope:elastic.DdpInitSyncRequest)
-  })
-_sym_db.RegisterMessage(DdpInitSyncRequest)
-
-DdpInitSyncResponse = _reflection.GeneratedProtocolMessageType('DdpInitSyncResponse', (_message.Message,), {
-  'DESCRIPTOR' : _DDPINITSYNCRESPONSE,
-  '__module__' : 'dlrover.proto.elastic_training_pb2'
-  # @@protoc_insertion_point(class_scope:elastic.DdpInitSyncResponse)
-  })
-_sym_db.RegisterMessage(DdpInitSyncResponse)
-
-GetCommRankRequest = _reflection.GeneratedProtocolMessageType('GetCommRankRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETCOMMRANKREQUEST,
-  '__module__' : 'dlrover.proto.elastic_training_pb2'
-  # @@protoc_insertion_point(class_scope:elastic.GetCommRankRequest)
-  })
-_sym_db.RegisterMessage(GetCommRankRequest)
-
-GetCommRankResponse = _reflection.GeneratedProtocolMessageType('GetCommRankResponse', (_message.Message,), {
-  'DESCRIPTOR' : _GETCOMMRANKRESPONSE,
-  '__module__' : 'dlrover.proto.elastic_training_pb2'
-  # @@protoc_insertion_point(class_scope:elastic.GetCommRankResponse)
-  })
-_sym_db.RegisterMessage(GetCommRankResponse)
-
-ReportTrainingLoopStatusRequest = _reflection.GeneratedProtocolMessageType('ReportTrainingLoopStatusRequest', (_message.Message,), {
-  'DESCRIPTOR' : _REPORTTRAININGLOOPSTATUSREQUEST,
-  '__module__' : 'dlrover.proto.elastic_training_pb2'
-  # @@protoc_insertion_point(class_scope:elastic.ReportTrainingLoopStatusRequest)
-  })
-_sym_db.RegisterMessage(ReportTrainingLoopStatusRequest)
-
 ShardCheckpoint = _reflection.GeneratedProtocolMessageType('ShardCheckpoint', (_message.Message,), {
   'DESCRIPTOR' : _SHARDCHECKPOINT,
   '__module__' : 'dlrover.proto.elastic_training_pb2'
   # @@protoc_insertion_point(class_scope:elastic.ShardCheckpoint)
   })
 _sym_db.RegisterMessage(ShardCheckpoint)
 
-ReportShardCheckpointResponse = _reflection.GeneratedProtocolMessageType('ReportShardCheckpointResponse', (_message.Message,), {
-  'DESCRIPTOR' : _REPORTSHARDCHECKPOINTRESPONSE,
-  '__module__' : 'dlrover.proto.elastic_training_pb2'
-  # @@protoc_insertion_point(class_scope:elastic.ReportShardCheckpointResponse)
-  })
-_sym_db.RegisterMessage(ReportShardCheckpointResponse)
-
 ReportUsedResourceRequest = _reflection.GeneratedProtocolMessageType('ReportUsedResourceRequest', (_message.Message,), {
   'DESCRIPTOR' : _REPORTUSEDRESOURCEREQUEST,
   '__module__' : 'dlrover.proto.elastic_training_pb2'
   # @@protoc_insertion_point(class_scope:elastic.ReportUsedResourceRequest)
   })
 _sym_db.RegisterMessage(ReportUsedResourceRequest)
 
@@ -295,14 +2090,21 @@
 NodeMeta = _reflection.GeneratedProtocolMessageType('NodeMeta', (_message.Message,), {
   'DESCRIPTOR' : _NODEMETA,
   '__module__' : 'dlrover.proto.elastic_training_pb2'
   # @@protoc_insertion_point(class_scope:elastic.NodeMeta)
   })
 _sym_db.RegisterMessage(NodeMeta)
 
+NodeEvent = _reflection.GeneratedProtocolMessageType('NodeEvent', (_message.Message,), {
+  'DESCRIPTOR' : _NODEEVENT,
+  '__module__' : 'dlrover.proto.elastic_training_pb2'
+  # @@protoc_insertion_point(class_scope:elastic.NodeEvent)
+  })
+_sym_db.RegisterMessage(NodeEvent)
+
 RunningNodes = _reflection.GeneratedProtocolMessageType('RunningNodes', (_message.Message,), {
   'DESCRIPTOR' : _RUNNINGNODES,
   '__module__' : 'dlrover.proto.elastic_training_pb2'
   # @@protoc_insertion_point(class_scope:elastic.RunningNodes)
   })
 _sym_db.RegisterMessage(RunningNodes)
 
@@ -323,96 +2125,423 @@
 ReportPreStopRequest = _reflection.GeneratedProtocolMessageType('ReportPreStopRequest', (_message.Message,), {
   'DESCRIPTOR' : _REPORTPRESTOPREQUEST,
   '__module__' : 'dlrover.proto.elastic_training_pb2'
   # @@protoc_insertion_point(class_scope:elastic.ReportPreStopRequest)
   })
 _sym_db.RegisterMessage(ReportPreStopRequest)
 
-_MASTER = DESCRIPTOR.services_by_name['Master']
-if _descriptor._USE_C_DESCRIPTORS == False:
+SyncRequest = _reflection.GeneratedProtocolMessageType('SyncRequest', (_message.Message,), {
+  'DESCRIPTOR' : _SYNCREQUEST,
+  '__module__' : 'dlrover.proto.elastic_training_pb2'
+  # @@protoc_insertion_point(class_scope:elastic.SyncRequest)
+  })
+_sym_db.RegisterMessage(SyncRequest)
+
+BarrierRequest = _reflection.GeneratedProtocolMessageType('BarrierRequest', (_message.Message,), {
+  'DESCRIPTOR' : _BARRIERREQUEST,
+  '__module__' : 'dlrover.proto.elastic_training_pb2'
+  # @@protoc_insertion_point(class_scope:elastic.BarrierRequest)
+  })
+_sym_db.RegisterMessage(BarrierRequest)
+
+RendezvousState = _reflection.GeneratedProtocolMessageType('RendezvousState', (_message.Message,), {
+
+  'WorldEntry' : _reflection.GeneratedProtocolMessageType('WorldEntry', (_message.Message,), {
+    'DESCRIPTOR' : _RENDEZVOUSSTATE_WORLDENTRY,
+    '__module__' : 'dlrover.proto.elastic_training_pb2'
+    # @@protoc_insertion_point(class_scope:elastic.RendezvousState.WorldEntry)
+    })
+  ,
+  'DESCRIPTOR' : _RENDEZVOUSSTATE,
+  '__module__' : 'dlrover.proto.elastic_training_pb2'
+  # @@protoc_insertion_point(class_scope:elastic.RendezvousState)
+  })
+_sym_db.RegisterMessage(RendezvousState)
+_sym_db.RegisterMessage(RendezvousState.WorldEntry)
+
+RendezvousRequest = _reflection.GeneratedProtocolMessageType('RendezvousRequest', (_message.Message,), {
+  'DESCRIPTOR' : _RENDEZVOUSREQUEST,
+  '__module__' : 'dlrover.proto.elastic_training_pb2'
+  # @@protoc_insertion_point(class_scope:elastic.RendezvousRequest)
+  })
+_sym_db.RegisterMessage(RendezvousRequest)
+
+RendezvousParams = _reflection.GeneratedProtocolMessageType('RendezvousParams', (_message.Message,), {
+  'DESCRIPTOR' : _RENDEZVOUSPARAMS,
+  '__module__' : 'dlrover.proto.elastic_training_pb2'
+  # @@protoc_insertion_point(class_scope:elastic.RendezvousParams)
+  })
+_sym_db.RegisterMessage(RendezvousParams)
+
+KeyValuePair = _reflection.GeneratedProtocolMessageType('KeyValuePair', (_message.Message,), {
+  'DESCRIPTOR' : _KEYVALUEPAIR,
+  '__module__' : 'dlrover.proto.elastic_training_pb2'
+  # @@protoc_insertion_point(class_scope:elastic.KeyValuePair)
+  })
+_sym_db.RegisterMessage(KeyValuePair)
+
+Response = _reflection.GeneratedProtocolMessageType('Response', (_message.Message,), {
+  'DESCRIPTOR' : _RESPONSE,
+  '__module__' : 'dlrover.proto.elastic_training_pb2'
+  # @@protoc_insertion_point(class_scope:elastic.Response)
+  })
+_sym_db.RegisterMessage(Response)
+
+NodeFailure = _reflection.GeneratedProtocolMessageType('NodeFailure', (_message.Message,), {
+  'DESCRIPTOR' : _NODEFAILURE,
+  '__module__' : 'dlrover.proto.elastic_training_pb2'
+  # @@protoc_insertion_point(class_scope:elastic.NodeFailure)
+  })
+_sym_db.RegisterMessage(NodeFailure)
+
+
+_TASK_EXTENDEDCONFIGENTRY._options = None
+_REPORTTASKRESULTREQUEST_EXECCOUNTERSENTRY._options = None
+_TENSORSTATS_TENSORALLOCBYTESENTRY._options = None
+_RENDEZVOUSSTATE_WORLDENTRY._options = None
+
+_MASTER = _descriptor.ServiceDescriptor(
+  name='Master',
+  full_name='elastic.Master',
+  file=DESCRIPTOR,
+  index=0,
+  serialized_options=None,
+  create_key=_descriptor._internal_create_key,
+  serialized_start=3472,
+  serialized_end=5866,
+  methods=[
+  _descriptor.MethodDescriptor(
+    name='get_task',
+    full_name='elastic.Master.get_task',
+    index=0,
+    containing_service=None,
+    input_type=_GETTASKREQUEST,
+    output_type=_TASK,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='report_task_result',
+    full_name='elastic.Master.report_task_result',
+    index=1,
+    containing_service=None,
+    input_type=_REPORTTASKRESULTREQUEST,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='report_dataset_shard_params',
+    full_name='elastic.Master.report_dataset_shard_params',
+    index=2,
+    containing_service=None,
+    input_type=_REPORTDATASETSHARDPARAMSREQUEST,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='get_dataset_epoch',
+    full_name='elastic.Master.get_dataset_epoch',
+    index=3,
+    containing_service=None,
+    input_type=_DATASETMETA,
+    output_type=_GETDATASETEPOCHRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='get_dataset_shard_num',
+    full_name='elastic.Master.get_dataset_shard_num',
+    index=4,
+    containing_service=None,
+    input_type=_DATASETMETA,
+    output_type=_DATASETMETA,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='get_shard_checkpoint',
+    full_name='elastic.Master.get_shard_checkpoint',
+    index=5,
+    containing_service=None,
+    input_type=_DATASETMETA,
+    output_type=_SHARDCHECKPOINT,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='report_shard_checkpoint',
+    full_name='elastic.Master.report_shard_checkpoint',
+    index=6,
+    containing_service=None,
+    input_type=_SHARDCHECKPOINT,
+    output_type=_RESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='report_used_resource',
+    full_name='elastic.Master.report_used_resource',
+    index=7,
+    containing_service=None,
+    input_type=_REPORTUSEDRESOURCEREQUEST,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='report_model_metric',
+    full_name='elastic.Master.report_model_metric',
+    index=8,
+    containing_service=None,
+    input_type=_MODELMETRIC,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='report_global_step',
+    full_name='elastic.Master.report_global_step',
+    index=9,
+    containing_service=None,
+    input_type=_GLOBALSTEPRECORD,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='join_sync',
+    full_name='elastic.Master.join_sync',
+    index=10,
+    containing_service=None,
+    input_type=_SYNCREQUEST,
+    output_type=_RESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='sync_finished',
+    full_name='elastic.Master.sync_finished',
+    index=11,
+    containing_service=None,
+    input_type=_SYNCREQUEST,
+    output_type=_RESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='barrier',
+    full_name='elastic.Master.barrier',
+    index=12,
+    containing_service=None,
+    input_type=_BARRIERREQUEST,
+    output_type=_RESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='get_cluster_version',
+    full_name='elastic.Master.get_cluster_version',
+    index=13,
+    containing_service=None,
+    input_type=_GETCLUSTERVERSIONREQUEST,
+    output_type=_GETCLUSTERVERSIONRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='update_cluster_version',
+    full_name='elastic.Master.update_cluster_version',
+    index=14,
+    containing_service=None,
+    input_type=_UPDATECLUSTERVERSIONREQUEST,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='query_ps_nodes',
+    full_name='elastic.Master.query_ps_nodes',
+    index=15,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=_QUERYPSNODESRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='query_training_status',
+    full_name='elastic.Master.query_training_status',
+    index=16,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=_QUERYTRAININGSTATUSRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='query_running_nodes',
+    full_name='elastic.Master.query_running_nodes',
+    index=17,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=_RUNNINGNODES,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='ready_for_ps_relaunch',
+    full_name='elastic.Master.ready_for_ps_relaunch',
+    index=18,
+    containing_service=None,
+    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='init_remote_lock',
+    full_name='elastic.Master.init_remote_lock',
+    index=19,
+    containing_service=None,
+    input_type=_INITREMOTELOCKREQUEST,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='acquire_remote_lock',
+    full_name='elastic.Master.acquire_remote_lock',
+    index=20,
+    containing_service=None,
+    input_type=_ACQUIREREMOTELOCKREQUEST,
+    output_type=_ACQUIREREMOTELOCKRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='release_remote_lock',
+    full_name='elastic.Master.release_remote_lock',
+    index=21,
+    containing_service=None,
+    input_type=_RELEASEREMOTELOCKREQUEST,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='get_comm_world',
+    full_name='elastic.Master.get_comm_world',
+    index=22,
+    containing_service=None,
+    input_type=_RENDEZVOUSREQUEST,
+    output_type=_RENDEZVOUSSTATE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='join_rendezvous',
+    full_name='elastic.Master.join_rendezvous',
+    index=23,
+    containing_service=None,
+    input_type=_RENDEZVOUSREQUEST,
+    output_type=_RENDEZVOUSSTATE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='num_nodes_waiting',
+    full_name='elastic.Master.num_nodes_waiting',
+    index=24,
+    containing_service=None,
+    input_type=_RENDEZVOUSREQUEST,
+    output_type=_RENDEZVOUSSTATE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='report_rdzv_params',
+    full_name='elastic.Master.report_rdzv_params',
+    index=25,
+    containing_service=None,
+    input_type=_RENDEZVOUSPARAMS,
+    output_type=_RESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='kv_store_set',
+    full_name='elastic.Master.kv_store_set',
+    index=26,
+    containing_service=None,
+    input_type=_KEYVALUEPAIR,
+    output_type=_RESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='kv_store_get',
+    full_name='elastic.Master.kv_store_get',
+    index=27,
+    containing_service=None,
+    input_type=_KEYVALUEPAIR,
+    output_type=_KEYVALUEPAIR,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='report_failure',
+    full_name='elastic.Master.report_failure',
+    index=28,
+    containing_service=None,
+    input_type=_NODEFAILURE,
+    output_type=_RESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='network_check_success',
+    full_name='elastic.Master.network_check_success',
+    index=29,
+    containing_service=None,
+    input_type=_RENDEZVOUSREQUEST,
+    output_type=_RESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='report_prestop',
+    full_name='elastic.Master.report_prestop',
+    index=30,
+    containing_service=None,
+    input_type=_REPORTPRESTOPREQUEST,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='update_node_status',
+    full_name='elastic.Master.update_node_status',
+    index=31,
+    containing_service=None,
+    input_type=_NODEMETA,
+    output_type=_RESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='update_node_event',
+    full_name='elastic.Master.update_node_event',
+    index=32,
+    containing_service=None,
+    input_type=_NODEEVENT,
+    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+])
+_sym_db.RegisterServiceDescriptor(_MASTER)
+
+DESCRIPTOR.services_by_name['Master'] = _MASTER
 
-  DESCRIPTOR._options = None
-  _TASK_EXTENDEDCONFIGENTRY._options = None
-  _TASK_EXTENDEDCONFIGENTRY._serialized_options = b'8\001'
-  _REPORTTASKRESULTREQUEST_EXECCOUNTERSENTRY._options = None
-  _REPORTTASKRESULTREQUEST_EXECCOUNTERSENTRY._serialized_options = b'8\001'
-  _TENSORSTATS_TENSORALLOCBYTESENTRY._options = None
-  _TENSORSTATS_TENSORALLOCBYTESENTRY._serialized_options = b'8\001'
-  _TASKTYPE._serialized_start=3301
-  _TASKTYPE._serialized_end=3401
-  _SHARD._serialized_start=78
-  _SHARD._serialized_end=144
-  _TASK._serialized_start=147
-  _TASK._serialized_end=372
-  _TASK_EXTENDEDCONFIGENTRY._serialized_start=319
-  _TASK_EXTENDEDCONFIGENTRY._serialized_end=372
-  _GETTASKREQUEST._serialized_start=374
-  _GETTASKREQUEST._serialized_end=452
-  _REPORTTASKRESULTREQUEST._serialized_start=455
-  _REPORTTASKRESULTREQUEST._serialized_end=668
-  _REPORTTASKRESULTREQUEST_EXECCOUNTERSENTRY._serialized_start=617
-  _REPORTTASKRESULTREQUEST_EXECCOUNTERSENTRY._serialized_end=668
-  _REPORTDATASETSHARDPARAMSREQUEST._serialized_start=671
-  _REPORTDATASETSHARDPARAMSREQUEST._serialized_end=900
-  _DATASETMETA._serialized_start=902
-  _DATASETMETA._serialized_end=937
-  _GETDATASETEPOCHRESPONSE._serialized_start=939
-  _GETDATASETEPOCHRESPONSE._serialized_end=979
-  _DDPRESETSYNCREQUEST._serialized_start=981
-  _DDPRESETSYNCREQUEST._serialized_end=1079
-  _DDPRESETSYNCRESPONSE._serialized_start=1081
-  _DDPRESETSYNCRESPONSE._serialized_end=1118
-  _DDPINITSYNCREQUEST._serialized_start=1120
-  _DDPINITSYNCREQUEST._serialized_end=1217
-  _DDPINITSYNCRESPONSE._serialized_start=1219
-  _DDPINITSYNCRESPONSE._serialized_end=1255
-  _GETCOMMRANKREQUEST._serialized_start=1257
-  _GETCOMMRANKREQUEST._serialized_end=1331
-  _GETCOMMRANKRESPONSE._serialized_start=1334
-  _GETCOMMRANKRESPONSE._serialized_end=1562
-  _REPORTTRAININGLOOPSTATUSREQUEST._serialized_start=1565
-  _REPORTTRAININGLOOPSTATUSREQUEST._serialized_end=1693
-  _SHARDCHECKPOINT._serialized_start=1695
-  _SHARDCHECKPOINT._serialized_end=1729
-  _REPORTSHARDCHECKPOINTRESPONSE._serialized_start=1731
-  _REPORTSHARDCHECKPOINTRESPONSE._serialized_end=1779
-  _REPORTUSEDRESOURCEREQUEST._serialized_start=1781
-  _REPORTUSEDRESOURCEREQUEST._serialized_end=1873
-  _TENSORSTATS._serialized_start=1876
-  _TENSORSTATS._serialized_end=2125
-  _TENSORSTATS_TENSORALLOCBYTESENTRY._serialized_start=2070
-  _TENSORSTATS_TENSORALLOCBYTESENTRY._serialized_end=2125
-  _OPERATIONSTATS._serialized_start=2128
-  _OPERATIONSTATS._serialized_end=2273
-  _MODELMETRIC._serialized_start=2275
-  _MODELMETRIC._serialized_end=2375
-  _GETCLUSTERVERSIONREQUEST._serialized_start=2377
-  _GETCLUSTERVERSIONREQUEST._serialized_end=2461
-  _GETCLUSTERVERSIONRESPONSE._serialized_start=2463
-  _GETCLUSTERVERSIONRESPONSE._serialized_end=2507
-  _UPDATECLUSTERVERSIONREQUEST._serialized_start=2509
-  _UPDATECLUSTERVERSIONREQUEST._serialized_end=2613
-  _INITREMOTELOCKREQUEST._serialized_start=2615
-  _INITREMOTELOCKREQUEST._serialized_end=2688
-  _ACQUIREREMOTELOCKREQUEST._serialized_start=2690
-  _ACQUIREREMOTELOCKREQUEST._serialized_end=2766
-  _ACQUIREREMOTELOCKRESPONSE._serialized_start=2768
-  _ACQUIREREMOTELOCKRESPONSE._serialized_end=2812
-  _RELEASEREMOTELOCKREQUEST._serialized_start=2814
-  _RELEASEREMOTELOCKREQUEST._serialized_end=2854
-  _GLOBALSTEPRECORD._serialized_start=2856
-  _GLOBALSTEPRECORD._serialized_end=2914
-  _QUERYPSNODESRESPONSE._serialized_start=2916
-  _QUERYPSNODESRESPONSE._serialized_end=2997
-  _NODEMETA._serialized_start=2999
-  _NODEMETA._serialized_end=3097
-  _RUNNINGNODES._serialized_start=3099
-  _RUNNINGNODES._serialized_end=3147
-  _QUERYTRAININGSTATUSRESPONSE._serialized_start=3149
-  _QUERYTRAININGSTATUSRESPONSE._serialized_end=3194
-  _RESOURCECONFIG._serialized_start=3196
-  _RESOURCECONFIG._serialized_end=3254
-  _REPORTPRESTOPREQUEST._serialized_start=3256
-  _REPORTPRESTOPREQUEST._serialized_end=3299
-  _MASTER._serialized_start=3404
-  _MASTER._serialized_end=5242
 # @@protoc_insertion_point(module_scope)
```

## dlrover/proto/elastic_training_pb2_grpc.py

```diff
@@ -11,34 +11,14 @@
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.reset_sync = channel.unary_unary(
-                '/elastic.Master/reset_sync',
-                request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.DdpResetSyncRequest.SerializeToString,
-                response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.DdpResetSyncResponse.FromString,
-                )
-        self.barrier_sync = channel.unary_unary(
-                '/elastic.Master/barrier_sync',
-                request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.DdpInitSyncRequest.SerializeToString,
-                response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.DdpInitSyncResponse.FromString,
-                )
-        self.get_comm_rank = channel.unary_unary(
-                '/elastic.Master/get_comm_rank',
-                request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.GetCommRankRequest.SerializeToString,
-                response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.GetCommRankResponse.FromString,
-                )
-        self.report_training_loop_status = channel.unary_unary(
-                '/elastic.Master/report_training_loop_status',
-                request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.ReportTrainingLoopStatusRequest.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                )
         self.get_task = channel.unary_unary(
                 '/elastic.Master/get_task',
                 request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.GetTaskRequest.SerializeToString,
                 response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.Task.FromString,
                 )
         self.report_task_result = channel.unary_unary(
                 '/elastic.Master/report_task_result',
@@ -51,28 +31,28 @@
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
         self.get_dataset_epoch = channel.unary_unary(
                 '/elastic.Master/get_dataset_epoch',
                 request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.DatasetMeta.SerializeToString,
                 response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.GetDatasetEpochResponse.FromString,
                 )
-        self.ready_for_ps_relaunch = channel.unary_unary(
-                '/elastic.Master/ready_for_ps_relaunch',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+        self.get_dataset_shard_num = channel.unary_unary(
+                '/elastic.Master/get_dataset_shard_num',
+                request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.DatasetMeta.SerializeToString,
+                response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.DatasetMeta.FromString,
                 )
         self.get_shard_checkpoint = channel.unary_unary(
                 '/elastic.Master/get_shard_checkpoint',
                 request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.DatasetMeta.SerializeToString,
                 response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.ShardCheckpoint.FromString,
                 )
         self.report_shard_checkpoint = channel.unary_unary(
                 '/elastic.Master/report_shard_checkpoint',
                 request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.ShardCheckpoint.SerializeToString,
-                response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.ReportShardCheckpointResponse.FromString,
+                response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.Response.FromString,
                 )
         self.report_used_resource = channel.unary_unary(
                 '/elastic.Master/report_used_resource',
                 request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.ReportUsedResourceRequest.SerializeToString,
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
         self.report_model_metric = channel.unary_unary(
@@ -81,18 +61,28 @@
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
         self.report_global_step = channel.unary_unary(
                 '/elastic.Master/report_global_step',
                 request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.GlobalStepRecord.SerializeToString,
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
-        self.query_running_nodes = channel.unary_unary(
-                '/elastic.Master/query_running_nodes',
-                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.RunningNodes.FromString,
+        self.join_sync = channel.unary_unary(
+                '/elastic.Master/join_sync',
+                request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.SyncRequest.SerializeToString,
+                response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.Response.FromString,
+                )
+        self.sync_finished = channel.unary_unary(
+                '/elastic.Master/sync_finished',
+                request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.SyncRequest.SerializeToString,
+                response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.Response.FromString,
+                )
+        self.barrier = channel.unary_unary(
+                '/elastic.Master/barrier',
+                request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.BarrierRequest.SerializeToString,
+                response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.Response.FromString,
                 )
         self.get_cluster_version = channel.unary_unary(
                 '/elastic.Master/get_cluster_version',
                 request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.GetClusterVersionRequest.SerializeToString,
                 response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.GetClusterVersionResponse.FromString,
                 )
         self.update_cluster_version = channel.unary_unary(
@@ -106,14 +96,24 @@
                 response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.QueryPsNodesResponse.FromString,
                 )
         self.query_training_status = channel.unary_unary(
                 '/elastic.Master/query_training_status',
                 request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
                 response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.QueryTrainingStatusResponse.FromString,
                 )
+        self.query_running_nodes = channel.unary_unary(
+                '/elastic.Master/query_running_nodes',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.RunningNodes.FromString,
+                )
+        self.ready_for_ps_relaunch = channel.unary_unary(
+                '/elastic.Master/ready_for_ps_relaunch',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
         self.init_remote_lock = channel.unary_unary(
                 '/elastic.Master/init_remote_lock',
                 request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.InitRemoteLockRequest.SerializeToString,
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
         self.acquire_remote_lock = channel.unary_unary(
                 '/elastic.Master/acquire_remote_lock',
@@ -121,190 +121,281 @@
                 response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.AcquireRemoteLockResponse.FromString,
                 )
         self.release_remote_lock = channel.unary_unary(
                 '/elastic.Master/release_remote_lock',
                 request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.ReleaseRemoteLockRequest.SerializeToString,
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
+        self.get_comm_world = channel.unary_unary(
+                '/elastic.Master/get_comm_world',
+                request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.RendezvousRequest.SerializeToString,
+                response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.RendezvousState.FromString,
+                )
+        self.join_rendezvous = channel.unary_unary(
+                '/elastic.Master/join_rendezvous',
+                request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.RendezvousRequest.SerializeToString,
+                response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.RendezvousState.FromString,
+                )
+        self.num_nodes_waiting = channel.unary_unary(
+                '/elastic.Master/num_nodes_waiting',
+                request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.RendezvousRequest.SerializeToString,
+                response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.RendezvousState.FromString,
+                )
+        self.report_rdzv_params = channel.unary_unary(
+                '/elastic.Master/report_rdzv_params',
+                request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.RendezvousParams.SerializeToString,
+                response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.Response.FromString,
+                )
+        self.kv_store_set = channel.unary_unary(
+                '/elastic.Master/kv_store_set',
+                request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.KeyValuePair.SerializeToString,
+                response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.Response.FromString,
+                )
+        self.kv_store_get = channel.unary_unary(
+                '/elastic.Master/kv_store_get',
+                request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.KeyValuePair.SerializeToString,
+                response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.KeyValuePair.FromString,
+                )
+        self.report_failure = channel.unary_unary(
+                '/elastic.Master/report_failure',
+                request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.NodeFailure.SerializeToString,
+                response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.Response.FromString,
+                )
+        self.network_check_success = channel.unary_unary(
+                '/elastic.Master/network_check_success',
+                request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.RendezvousRequest.SerializeToString,
+                response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.Response.FromString,
+                )
         self.report_prestop = channel.unary_unary(
                 '/elastic.Master/report_prestop',
                 request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.ReportPreStopRequest.SerializeToString,
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
+        self.update_node_status = channel.unary_unary(
+                '/elastic.Master/update_node_status',
+                request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.NodeMeta.SerializeToString,
+                response_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.Response.FromString,
+                )
+        self.update_node_event = channel.unary_unary(
+                '/elastic.Master/update_node_event',
+                request_serializer=dlrover_dot_proto_dot_elastic__training__pb2.NodeEvent.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
 
 
 class MasterServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def reset_sync(self, request, context):
+    def get_task(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def barrier_sync(self, request, context):
+    def report_task_result(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def get_comm_rank(self, request, context):
+    def report_dataset_shard_params(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def report_training_loop_status(self, request, context):
+    def get_dataset_epoch(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def get_task(self, request, context):
-        """TODO : Unify the above 3 PRCs with new ones.
+    def get_dataset_shard_num(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def get_shard_checkpoint(self, request, context):
+        """rpcs for saving and restoring data shard checkpoints
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def report_task_result(self, request, context):
+    def report_shard_checkpoint(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def report_dataset_shard_params(self, request, context):
+    def report_used_resource(self, request, context):
+        """rpcs to report training metrics
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def report_model_metric(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def get_dataset_epoch(self, request, context):
+    def report_global_step(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ready_for_ps_relaunch(self, request, context):
-        """rpcs for supporting PS adjustment
+    def join_sync(self, request, context):
+        """rpcs for worker sync
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def get_shard_checkpoint(self, request, context):
-        """rpcs for saving and restoring data shard checkpoints
-        """
+    def sync_finished(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def report_shard_checkpoint(self, request, context):
+    def barrier(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def report_used_resource(self, request, context):
+    def get_cluster_version(self, request, context):
+        """rpc for elastic PS
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def update_cluster_version(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def report_model_metric(self, request, context):
+    def query_ps_nodes(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def report_global_step(self, request, context):
+    def query_training_status(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def query_running_nodes(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def get_cluster_version(self, request, context):
-        """rpc for elastic PS
+    def ready_for_ps_relaunch(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def init_remote_lock(self, request, context):
+        """rpc for remote lock
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def update_cluster_version(self, request, context):
+    def acquire_remote_lock(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def query_ps_nodes(self, request, context):
+    def release_remote_lock(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def query_training_status(self, request, context):
+    def get_comm_world(self, request, context):
+        """rpc for torch elastic
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def join_rendezvous(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def init_remote_lock(self, request, context):
-        """rpc for remote lock
-        """
+    def num_nodes_waiting(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def acquire_remote_lock(self, request, context):
+    def report_rdzv_params(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def release_remote_lock(self, request, context):
+    def kv_store_set(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def kv_store_get(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def report_failure(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def network_check_success(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def report_prestop(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def update_node_status(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def update_node_event(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_MasterServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'reset_sync': grpc.unary_unary_rpc_method_handler(
-                    servicer.reset_sync,
-                    request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.DdpResetSyncRequest.FromString,
-                    response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.DdpResetSyncResponse.SerializeToString,
-            ),
-            'barrier_sync': grpc.unary_unary_rpc_method_handler(
-                    servicer.barrier_sync,
-                    request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.DdpInitSyncRequest.FromString,
-                    response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.DdpInitSyncResponse.SerializeToString,
-            ),
-            'get_comm_rank': grpc.unary_unary_rpc_method_handler(
-                    servicer.get_comm_rank,
-                    request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.GetCommRankRequest.FromString,
-                    response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.GetCommRankResponse.SerializeToString,
-            ),
-            'report_training_loop_status': grpc.unary_unary_rpc_method_handler(
-                    servicer.report_training_loop_status,
-                    request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.ReportTrainingLoopStatusRequest.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            ),
             'get_task': grpc.unary_unary_rpc_method_handler(
                     servicer.get_task,
                     request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.GetTaskRequest.FromString,
                     response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.Task.SerializeToString,
             ),
             'report_task_result': grpc.unary_unary_rpc_method_handler(
                     servicer.report_task_result,
@@ -317,28 +408,28 @@
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
             'get_dataset_epoch': grpc.unary_unary_rpc_method_handler(
                     servicer.get_dataset_epoch,
                     request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.DatasetMeta.FromString,
                     response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.GetDatasetEpochResponse.SerializeToString,
             ),
-            'ready_for_ps_relaunch': grpc.unary_unary_rpc_method_handler(
-                    servicer.ready_for_ps_relaunch,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            'get_dataset_shard_num': grpc.unary_unary_rpc_method_handler(
+                    servicer.get_dataset_shard_num,
+                    request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.DatasetMeta.FromString,
+                    response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.DatasetMeta.SerializeToString,
             ),
             'get_shard_checkpoint': grpc.unary_unary_rpc_method_handler(
                     servicer.get_shard_checkpoint,
                     request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.DatasetMeta.FromString,
                     response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.ShardCheckpoint.SerializeToString,
             ),
             'report_shard_checkpoint': grpc.unary_unary_rpc_method_handler(
                     servicer.report_shard_checkpoint,
                     request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.ShardCheckpoint.FromString,
-                    response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.ReportShardCheckpointResponse.SerializeToString,
+                    response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.Response.SerializeToString,
             ),
             'report_used_resource': grpc.unary_unary_rpc_method_handler(
                     servicer.report_used_resource,
                     request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.ReportUsedResourceRequest.FromString,
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
             'report_model_metric': grpc.unary_unary_rpc_method_handler(
@@ -347,18 +438,28 @@
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
             'report_global_step': grpc.unary_unary_rpc_method_handler(
                     servicer.report_global_step,
                     request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.GlobalStepRecord.FromString,
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
-            'query_running_nodes': grpc.unary_unary_rpc_method_handler(
-                    servicer.query_running_nodes,
-                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                    response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.RunningNodes.SerializeToString,
+            'join_sync': grpc.unary_unary_rpc_method_handler(
+                    servicer.join_sync,
+                    request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.SyncRequest.FromString,
+                    response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.Response.SerializeToString,
+            ),
+            'sync_finished': grpc.unary_unary_rpc_method_handler(
+                    servicer.sync_finished,
+                    request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.SyncRequest.FromString,
+                    response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.Response.SerializeToString,
+            ),
+            'barrier': grpc.unary_unary_rpc_method_handler(
+                    servicer.barrier,
+                    request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.BarrierRequest.FromString,
+                    response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.Response.SerializeToString,
             ),
             'get_cluster_version': grpc.unary_unary_rpc_method_handler(
                     servicer.get_cluster_version,
                     request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.GetClusterVersionRequest.FromString,
                     response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.GetClusterVersionResponse.SerializeToString,
             ),
             'update_cluster_version': grpc.unary_unary_rpc_method_handler(
@@ -372,14 +473,24 @@
                     response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.QueryPsNodesResponse.SerializeToString,
             ),
             'query_training_status': grpc.unary_unary_rpc_method_handler(
                     servicer.query_training_status,
                     request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                     response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.QueryTrainingStatusResponse.SerializeToString,
             ),
+            'query_running_nodes': grpc.unary_unary_rpc_method_handler(
+                    servicer.query_running_nodes,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.RunningNodes.SerializeToString,
+            ),
+            'ready_for_ps_relaunch': grpc.unary_unary_rpc_method_handler(
+                    servicer.ready_for_ps_relaunch,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
             'init_remote_lock': grpc.unary_unary_rpc_method_handler(
                     servicer.init_remote_lock,
                     request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.InitRemoteLockRequest.FromString,
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
             'acquire_remote_lock': grpc.unary_unary_rpc_method_handler(
                     servicer.acquire_remote_lock,
@@ -387,349 +498,399 @@
                     response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.AcquireRemoteLockResponse.SerializeToString,
             ),
             'release_remote_lock': grpc.unary_unary_rpc_method_handler(
                     servicer.release_remote_lock,
                     request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.ReleaseRemoteLockRequest.FromString,
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
+            'get_comm_world': grpc.unary_unary_rpc_method_handler(
+                    servicer.get_comm_world,
+                    request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.RendezvousRequest.FromString,
+                    response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.RendezvousState.SerializeToString,
+            ),
+            'join_rendezvous': grpc.unary_unary_rpc_method_handler(
+                    servicer.join_rendezvous,
+                    request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.RendezvousRequest.FromString,
+                    response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.RendezvousState.SerializeToString,
+            ),
+            'num_nodes_waiting': grpc.unary_unary_rpc_method_handler(
+                    servicer.num_nodes_waiting,
+                    request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.RendezvousRequest.FromString,
+                    response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.RendezvousState.SerializeToString,
+            ),
+            'report_rdzv_params': grpc.unary_unary_rpc_method_handler(
+                    servicer.report_rdzv_params,
+                    request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.RendezvousParams.FromString,
+                    response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.Response.SerializeToString,
+            ),
+            'kv_store_set': grpc.unary_unary_rpc_method_handler(
+                    servicer.kv_store_set,
+                    request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.KeyValuePair.FromString,
+                    response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.Response.SerializeToString,
+            ),
+            'kv_store_get': grpc.unary_unary_rpc_method_handler(
+                    servicer.kv_store_get,
+                    request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.KeyValuePair.FromString,
+                    response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.KeyValuePair.SerializeToString,
+            ),
+            'report_failure': grpc.unary_unary_rpc_method_handler(
+                    servicer.report_failure,
+                    request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.NodeFailure.FromString,
+                    response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.Response.SerializeToString,
+            ),
+            'network_check_success': grpc.unary_unary_rpc_method_handler(
+                    servicer.network_check_success,
+                    request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.RendezvousRequest.FromString,
+                    response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.Response.SerializeToString,
+            ),
             'report_prestop': grpc.unary_unary_rpc_method_handler(
                     servicer.report_prestop,
                     request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.ReportPreStopRequest.FromString,
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
+            'update_node_status': grpc.unary_unary_rpc_method_handler(
+                    servicer.update_node_status,
+                    request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.NodeMeta.FromString,
+                    response_serializer=dlrover_dot_proto_dot_elastic__training__pb2.Response.SerializeToString,
+            ),
+            'update_node_event': grpc.unary_unary_rpc_method_handler(
+                    servicer.update_node_event,
+                    request_deserializer=dlrover_dot_proto_dot_elastic__training__pb2.NodeEvent.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'elastic.Master', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class Master(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def reset_sync(request,
+    def get_task(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/elastic.Master/reset_sync',
-            dlrover_dot_proto_dot_elastic__training__pb2.DdpResetSyncRequest.SerializeToString,
-            dlrover_dot_proto_dot_elastic__training__pb2.DdpResetSyncResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/get_task',
+            dlrover_dot_proto_dot_elastic__training__pb2.GetTaskRequest.SerializeToString,
+            dlrover_dot_proto_dot_elastic__training__pb2.Task.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def barrier_sync(request,
+    def report_task_result(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/elastic.Master/barrier_sync',
-            dlrover_dot_proto_dot_elastic__training__pb2.DdpInitSyncRequest.SerializeToString,
-            dlrover_dot_proto_dot_elastic__training__pb2.DdpInitSyncResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/report_task_result',
+            dlrover_dot_proto_dot_elastic__training__pb2.ReportTaskResultRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def get_comm_rank(request,
+    def report_dataset_shard_params(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/elastic.Master/get_comm_rank',
-            dlrover_dot_proto_dot_elastic__training__pb2.GetCommRankRequest.SerializeToString,
-            dlrover_dot_proto_dot_elastic__training__pb2.GetCommRankResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/report_dataset_shard_params',
+            dlrover_dot_proto_dot_elastic__training__pb2.ReportDatasetShardParamsRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def report_training_loop_status(request,
+    def get_dataset_epoch(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/elastic.Master/report_training_loop_status',
-            dlrover_dot_proto_dot_elastic__training__pb2.ReportTrainingLoopStatusRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/get_dataset_epoch',
+            dlrover_dot_proto_dot_elastic__training__pb2.DatasetMeta.SerializeToString,
+            dlrover_dot_proto_dot_elastic__training__pb2.GetDatasetEpochResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def get_task(request,
+    def get_dataset_shard_num(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/elastic.Master/get_task',
-            dlrover_dot_proto_dot_elastic__training__pb2.GetTaskRequest.SerializeToString,
-            dlrover_dot_proto_dot_elastic__training__pb2.Task.FromString,
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/get_dataset_shard_num',
+            dlrover_dot_proto_dot_elastic__training__pb2.DatasetMeta.SerializeToString,
+            dlrover_dot_proto_dot_elastic__training__pb2.DatasetMeta.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def report_task_result(request,
+    def get_shard_checkpoint(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/elastic.Master/report_task_result',
-            dlrover_dot_proto_dot_elastic__training__pb2.ReportTaskResultRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/get_shard_checkpoint',
+            dlrover_dot_proto_dot_elastic__training__pb2.DatasetMeta.SerializeToString,
+            dlrover_dot_proto_dot_elastic__training__pb2.ShardCheckpoint.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def report_dataset_shard_params(request,
+    def report_shard_checkpoint(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/elastic.Master/report_dataset_shard_params',
-            dlrover_dot_proto_dot_elastic__training__pb2.ReportDatasetShardParamsRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/report_shard_checkpoint',
+            dlrover_dot_proto_dot_elastic__training__pb2.ShardCheckpoint.SerializeToString,
+            dlrover_dot_proto_dot_elastic__training__pb2.Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def get_dataset_epoch(request,
+    def report_used_resource(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/elastic.Master/get_dataset_epoch',
-            dlrover_dot_proto_dot_elastic__training__pb2.DatasetMeta.SerializeToString,
-            dlrover_dot_proto_dot_elastic__training__pb2.GetDatasetEpochResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/report_used_resource',
+            dlrover_dot_proto_dot_elastic__training__pb2.ReportUsedResourceRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ready_for_ps_relaunch(request,
+    def report_model_metric(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/elastic.Master/ready_for_ps_relaunch',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/report_model_metric',
+            dlrover_dot_proto_dot_elastic__training__pb2.ModelMetric.SerializeToString,
             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def get_shard_checkpoint(request,
+    def report_global_step(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/elastic.Master/get_shard_checkpoint',
-            dlrover_dot_proto_dot_elastic__training__pb2.DatasetMeta.SerializeToString,
-            dlrover_dot_proto_dot_elastic__training__pb2.ShardCheckpoint.FromString,
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/report_global_step',
+            dlrover_dot_proto_dot_elastic__training__pb2.GlobalStepRecord.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def report_shard_checkpoint(request,
+    def join_sync(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/elastic.Master/report_shard_checkpoint',
-            dlrover_dot_proto_dot_elastic__training__pb2.ShardCheckpoint.SerializeToString,
-            dlrover_dot_proto_dot_elastic__training__pb2.ReportShardCheckpointResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/join_sync',
+            dlrover_dot_proto_dot_elastic__training__pb2.SyncRequest.SerializeToString,
+            dlrover_dot_proto_dot_elastic__training__pb2.Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def report_used_resource(request,
+    def sync_finished(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/elastic.Master/report_used_resource',
-            dlrover_dot_proto_dot_elastic__training__pb2.ReportUsedResourceRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/sync_finished',
+            dlrover_dot_proto_dot_elastic__training__pb2.SyncRequest.SerializeToString,
+            dlrover_dot_proto_dot_elastic__training__pb2.Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def report_model_metric(request,
+    def barrier(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/elastic.Master/report_model_metric',
-            dlrover_dot_proto_dot_elastic__training__pb2.ModelMetric.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/barrier',
+            dlrover_dot_proto_dot_elastic__training__pb2.BarrierRequest.SerializeToString,
+            dlrover_dot_proto_dot_elastic__training__pb2.Response.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def report_global_step(request,
+    def get_cluster_version(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/elastic.Master/report_global_step',
-            dlrover_dot_proto_dot_elastic__training__pb2.GlobalStepRecord.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/get_cluster_version',
+            dlrover_dot_proto_dot_elastic__training__pb2.GetClusterVersionRequest.SerializeToString,
+            dlrover_dot_proto_dot_elastic__training__pb2.GetClusterVersionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def query_running_nodes(request,
+    def update_cluster_version(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/elastic.Master/query_running_nodes',
-            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            dlrover_dot_proto_dot_elastic__training__pb2.RunningNodes.FromString,
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/update_cluster_version',
+            dlrover_dot_proto_dot_elastic__training__pb2.UpdateClusterVersionRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def get_cluster_version(request,
+    def query_ps_nodes(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/elastic.Master/get_cluster_version',
-            dlrover_dot_proto_dot_elastic__training__pb2.GetClusterVersionRequest.SerializeToString,
-            dlrover_dot_proto_dot_elastic__training__pb2.GetClusterVersionResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/query_ps_nodes',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            dlrover_dot_proto_dot_elastic__training__pb2.QueryPsNodesResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def update_cluster_version(request,
+    def query_training_status(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/elastic.Master/update_cluster_version',
-            dlrover_dot_proto_dot_elastic__training__pb2.UpdateClusterVersionRequest.SerializeToString,
-            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/query_training_status',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            dlrover_dot_proto_dot_elastic__training__pb2.QueryTrainingStatusResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def query_ps_nodes(request,
+    def query_running_nodes(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/elastic.Master/query_ps_nodes',
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/query_running_nodes',
             google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            dlrover_dot_proto_dot_elastic__training__pb2.QueryPsNodesResponse.FromString,
+            dlrover_dot_proto_dot_elastic__training__pb2.RunningNodes.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def query_training_status(request,
+    def ready_for_ps_relaunch(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/elastic.Master/query_training_status',
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/ready_for_ps_relaunch',
             google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-            dlrover_dot_proto_dot_elastic__training__pb2.QueryTrainingStatusResponse.FromString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def init_remote_lock(request,
             target,
             options=(),
@@ -777,14 +938,150 @@
         return grpc.experimental.unary_unary(request, target, '/elastic.Master/release_remote_lock',
             dlrover_dot_proto_dot_elastic__training__pb2.ReleaseRemoteLockRequest.SerializeToString,
             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def get_comm_world(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/get_comm_world',
+            dlrover_dot_proto_dot_elastic__training__pb2.RendezvousRequest.SerializeToString,
+            dlrover_dot_proto_dot_elastic__training__pb2.RendezvousState.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def join_rendezvous(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/join_rendezvous',
+            dlrover_dot_proto_dot_elastic__training__pb2.RendezvousRequest.SerializeToString,
+            dlrover_dot_proto_dot_elastic__training__pb2.RendezvousState.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def num_nodes_waiting(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/num_nodes_waiting',
+            dlrover_dot_proto_dot_elastic__training__pb2.RendezvousRequest.SerializeToString,
+            dlrover_dot_proto_dot_elastic__training__pb2.RendezvousState.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def report_rdzv_params(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/report_rdzv_params',
+            dlrover_dot_proto_dot_elastic__training__pb2.RendezvousParams.SerializeToString,
+            dlrover_dot_proto_dot_elastic__training__pb2.Response.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def kv_store_set(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/kv_store_set',
+            dlrover_dot_proto_dot_elastic__training__pb2.KeyValuePair.SerializeToString,
+            dlrover_dot_proto_dot_elastic__training__pb2.Response.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def kv_store_get(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/kv_store_get',
+            dlrover_dot_proto_dot_elastic__training__pb2.KeyValuePair.SerializeToString,
+            dlrover_dot_proto_dot_elastic__training__pb2.KeyValuePair.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def report_failure(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/report_failure',
+            dlrover_dot_proto_dot_elastic__training__pb2.NodeFailure.SerializeToString,
+            dlrover_dot_proto_dot_elastic__training__pb2.Response.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def network_check_success(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/network_check_success',
+            dlrover_dot_proto_dot_elastic__training__pb2.RendezvousRequest.SerializeToString,
+            dlrover_dot_proto_dot_elastic__training__pb2.Response.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def report_prestop(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -792,7 +1089,41 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/elastic.Master/report_prestop',
             dlrover_dot_proto_dot_elastic__training__pb2.ReportPreStopRequest.SerializeToString,
             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def update_node_status(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/update_node_status',
+            dlrover_dot_proto_dot_elastic__training__pb2.NodeMeta.SerializeToString,
+            dlrover_dot_proto_dot_elastic__training__pb2.Response.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def update_node_event(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/elastic.Master/update_node_event',
+            dlrover_dot_proto_dot_elastic__training__pb2.NodeEvent.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

## dlrover/python/brain/client.py

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 The ElasticDL Authors. All rights reserved.
+# Copyright 2020 The DLRover Authors. All rights reserved.
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
@@ -10,22 +10,23 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
 from dlrover.proto import brain_pb2, brain_pb2_grpc
-from dlrover.python.common.grpc import build_channel
+from dlrover.python.common.grpc import build_channel, grpc_server_ready
 from dlrover.python.common.log import default_logger as logger
 
-DATA_STORE = "data_store_elasticdl"
-OPTIMIZE_PROCESSOR = "running_training_job_optimize_processor"
+DATA_STORE = "base_datastore"
+OPTIMIZE_PROCESSOR = "running_training_job_optimize_request_processor"
 BASE_OPTIMIZE_PROCESSOR = "base_optimize_processor"
 
-_ENV_BRAIN_ADDR_KEY = "EASYDL_BRAIN_SERVICE_ADDR"
+_ENV_BRAIN_ADDR_KEY = "DLROVER_BRAIN_SERVICE_ADDR"
+_DEFAULT_BRAIN_ADDR = "dlrover-brain.dlrover.svc.cluster.local:50001"
 
 
 def catch_exception(func):
     def wrapper(self, *args, **kwargs):
         try:
             return func(self, *args, **kwargs)
         except Exception as e:
@@ -75,32 +76,36 @@
         """Initialize an EasyDL client.
         Args:
             channel: grpc.Channel
             the gRPC channel object connects to master gRPC server.
 
             job_name: string
             the unique and ordered worker ID assigned
-            by elasticdl command-line.
+            by dlrover command-line.
         """
         if brain_channel:
             self._brain_stub = brain_pb2_grpc.BrainStub(brain_channel)
         else:
             logger.warning("Cannot initialize brain channel")
+            self._brain_stub = None
+
+    def available(self):
+        return self._brain_stub is not None
 
     def report_metrics(self, job_metrics):
         """Report job metrics to administer service"""
         return self._brain_stub.persist_metrics(job_metrics)
 
     def get_job_metrics(self, job_uuid):
         """Get the job metrics by the job uuid.
         Examples:
             ```
             import json
 
-            client = build_easydl_client()
+            client = build_brain_client()
             metrics_res = client.get_job_metrics("xxxx")
             metrics = json.loads(metrics_res.job_metrics)
             ```
         """
         request = brain_pb2.JobMetricsRequest()
         request.job_uuid = job_uuid
         return self._brain_stub.get_job_metrics(request)
@@ -216,29 +221,29 @@
         for key, value in config.items():
             request.config.customized_config[key] = value
         request.jobs.add()
         request.jobs[0].uid = job_uuid
         return self.request_optimization(request)
 
     def get_oom_resource_plan(
-        self, oom_pods, job_uuid, stage, opt_retriever, config={}
+        self, nodes, job_uuid, stage, opt_retriever, config={}
     ):
         request = brain_pb2.OptimizeRequest()
         request.type = stage
         request.config.optimizer_config_retriever = opt_retriever
         request.config.data_store = DATA_STORE
         request.config.brain_processor = OPTIMIZE_PROCESSOR
         for key, value in config.items():
             request.config.customized_config[key] = value
         request.jobs.add()
         job = request.jobs[0]
         job.uid = job_uuid
-        for pod_name in oom_pods:
-            job.state.pods[pod_name].is_oom = True
-            job.state.pods[pod_name].name = pod_name
+        for node in nodes:
+            job.state.pods[node.name].is_oom = True
+            job.state.pods[node.name].name = node.name
         return self.request_optimization(request)
 
     def report_job_exit_reason(self, job_meta, reason):
         job_metrics = init_job_metrics_message(job_meta)
         job_metrics.metrics_type = brain_pb2.MetricsType.Job_Exit_Reason
         job_metrics.job_exit_reason = reason
         return self.report_metrics(job_metrics)
@@ -249,24 +254,28 @@
         request.config_key = key
         response = self._brain_stub.get_config(request)
         if response.response.success:
             return response.config_value
         return None
 
 
-def build_easydl_client():
+def build_brain_client():
     """Build a client of the EasyDL server.
 
     Example:
         ```
         import os
         os.environ["EASYDL_BRAIN_SERVICE_ADDR"] = "xxx"
-        client = build_easydl_client()
+        client = build_brain_client()
         ```
     """
-    brain_addr = os.getenv(_ENV_BRAIN_ADDR_KEY, None)
+    brain_addr = os.getenv(_ENV_BRAIN_ADDR_KEY, _DEFAULT_BRAIN_ADDR)
     channel = build_channel(brain_addr)
-    return BrainClient(channel)
+    if channel and grpc_server_ready(channel):
+        return BrainClient(channel)
+    else:
+        logger.warning("The GRPC service of brain is not available.")
+        return BrainClient(None)
 
 
-class GlobalEasydlClient(object):
-    EASYDL_CLIENT = build_easydl_client()
+class GlobalBrainClient(object):
+    BRAIN_CLIENT = build_brain_client()
```

## dlrover/python/common/constants.py

```diff
@@ -15,17 +15,27 @@
 class PriorityClass(object):
     LOW = "low"
     HIGH = "high"
 
 
 class PlatformType(object):
     KUBERNETES = "k8s"
+    RAY = "ray"
     PY_KUBERNETES = "pyk8s"
 
 
+class ElasticJobApi(object):
+    GROUP = "elastic.iml.github.io"
+    VERION = "v1alpha1"
+    SCALEPLAN_KIND = "ScalePlan"
+    SCALEPLAN_PLURAL = "scaleplans"
+    ELASTICJOB_KIND = "elasticjob"
+    ELASTICJOB_PLURAL = "elasticjobs"
+
+
 class UserEnv(object):
     USER_ID = "USER_ID"
 
 
 class TaskType(object):
     TRAINING = "training"
     EVALUATION = "evaluation"
@@ -39,40 +49,49 @@
     EVALUATOR = "evaluator"
     CHIEF = "chief"
     DLROVER_MASTER = "dlrover-master"
 
 
 class ElasticJobLabel(object):
     APP_NAME = "dlrover"
-    JOB_KEY = "elasticjob-name"
-    REPLICA_TYPE_KEY = "replica-type"
-    REPLICA_INDEX_KEY = "replica-index"
-    RANK_INDEX_KEY = "rank-index"
+    JOB_KEY = "elasticjob.dlrover/name"
+    REPLICA_TYPE_KEY = "elasticjob.dlrover/replica-type"
+    REPLICA_INDEX_KEY = "elasticjob.dlrover/replica-index"
+    RANK_INDEX_KEY = "elasticjob.dlrover/rank-index"
+
+
+class ScalePlanLabel(object):
+    SCALE_TYPE_KEY = "scale-type"
+    MANUAL_SCALE = "manual"
+    AUTO_SCALE = "auto"
 
 
 class NodeStatus(object):
     SUCCEEDED = "Succeeded"
     FAILED = "Failed"
     RUNNING = "Running"
     FINISHED = "Finished"
     PENDING = "Pending"
     INITIAL = "Initial"
     DELETED = "Deleted"
+    UNKNOWN = "Unknown"
+    BREAKDOWN = "Breakdown"
 
 
 class NodeEventType(object):
     MODIFIED = "MODIFIED"
     DELETED = "DELETED"
 
 
 class NodeExitReason(object):
     KILLED = "Deleted"
     OOM = "OOMKilled"
     FATAL_ERROR = "Error"
     UNKNOWN_ERROR = "UnknownError"
+    HARDWARE_ERROR = "HardwareError"
 
 
 class JobExitReason(object):
     SUCCEEDED = "Completed"
     CODE_ERROR = "CodeError"
     WORKER_OOM = "WorkerOOM"
     WORKER_ERROR = "WorkerError"
@@ -84,14 +103,18 @@
 
 
 class ExitCode(object):
     FATAL_ERROR_CODE = 1
     KILLED_CODE = 137
     TERMED_CODE = 143
     CORE_DUMP_ERROR_CODE = 134
+    OOM_CODE = 247
+    GPU_DRIVER_ERROR = 201
+    GPU_POD_RESIDUE = 202
+    GPU_INFOROM_CORRUPTED = 14
 
 
 class NodeResourceLimit(object):
     MAX_CPU_CORES = 32
     MIN_CPU_CORES = 4
     MIN_MEMORY = 6144  # 6Gi
     MAX_MEMORY = 65536  # 65536Mi, 64Gi
@@ -102,23 +125,24 @@
     HUGE_CPU_THRESHOLD = 100
     WAIT_CHIEF_TIMEOUT_SECS = 1800  # 30min
     WAIT_DATA_SHARD_SERVICE_CREATION_SECS = 600  # 10min
     PS_CPU_GROWTH_RATE = 1.2
     PS_CPU_DECREASED_RATE = 0.5
     MIN_VALID_MEMORY = 1024  # 1GB
     MIN_VALID_CPU = 2
+    MAX_HANG_TIMEOUT_SECS = 10800  # unit: seconds
 
 
 class DefaultNodeResource(object):
-    PS_NUM = 3
-    PS_MEMORY = 16384  # 16GB
-    PS_CPU = 12
-    WORKER_NUM = 5
-    WORKER_CPU = 16
-    WORKER_MEMORY = 16384  # 16GB
+    PS_NUM = 1
+    PS_MEMORY = 8000  # MB
+    PS_CPU = 1
+    WORKER_NUM = 2
+    WORKER_CPU = 1
+    WORKER_MEMORY = 8000  # MB
 
 
 class ResourceOptimizerName(object):
     BRAIN = "brain"
     LOCAL = "local"
 
 
@@ -133,15 +157,15 @@
     SAMPLE = "sample"
     INITIAL = "initial"
     STABLE = "stable"
 
 
 class DistributionStrategy(object):
     LOCAL = "Local"
-    PARAMETER_SERVER = "ParameterServerStrategy"
+    PS = "ParameterServerStrategy"
     ALLREDUCE = "AllreduceStrategy"
     CUSTOM = "CustomStrategy"
 
 
 class PSClusterVersionType(object):
     GLOBAL = "GLOBAL"
     LOCAL = "LOCAL"
@@ -159,23 +183,60 @@
     START = 1
     END = 2
     PENDING = 3
 
 
 class NodeEnv(object):
     RELAUNCHED_POD = "RELAUNCHED_POD"
-    ELASTICDL_ENABLED = "ELASTICDL_ENABLED"
-    MASTER_ADDR = "DLROVER_MASTER_ADDR"
+    DLROVER_MASTER_ADDR = "DLROVER_MASTER_ADDR"
     WORKER_TYPE = "WORKER_TYPE"
     WORKER_ID = "WORKER_ID"
     WORKER_NUM = "WORKER_NUM"
+    WORKER_RANK = "WORKER_RANK"
+    RDZV_ENDPOINT = "RDZV_ENDPOINT"
+    GRPC_ENABLE_FORK = "GRPC_ENABLE_FORK_SUPPORT"
+    POD_NAME = "POD_NAME"
+    AUTO_MONITOR_WORKLOAD = "AUTO_MONITOR_WORKLOAD"
 
 
 class DatasetType(object):
     TEXT = "text"
     MAXCOMPUTE_TABLE = "maxcompute_table"
 
 
 class DefaultResourceLimits(object):
     CPU_LIMIT = 100
     MEMORY_LIMIT = "102400Mi"  # 100Gi
     GPU_LIMIT = 4
+
+
+class OptimizeMode(object):
+    MANNUAL = "manunal"
+    SINGLE_JOB = "single-job"
+    CLUSTER = "cluster"
+
+
+class ReporterType(object):
+    LOCAL = "local"
+    DLROVER_BRAIN = "brain"
+
+
+class MemoryUnit(object):
+    MB = 1024 * 1024
+
+
+class k8sAPIExceptionReason(object):
+    NOT_FOUND = "Not Found"
+
+
+class RendezvousName(object):
+    ELASTIC_TRAINING = "elastic-training"
+    NETWORK_CHECK = "network-check"
+
+
+class NodeErrorMessage(object):
+    NETWORKER_ERROR = "Network is breakdown"
+
+
+class NetworkFailureReason(object):
+    NODE_FAILURE = "Node Failure"
+    WAITING_NODE = "Waiting node"
```

## dlrover/python/common/global_context.py

```diff
@@ -11,99 +11,118 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import threading
 
 from dlrover.python.common.constants import UserEnv
+from dlrover.python.common.grpc import find_free_port_in_range
 from dlrover.python.common.log import default_logger as logger
 
 
-# TODO: Get configuration parameters from DLRover Brain
-def get_param_value_from_easydl(key_name, default_value, dtype=int):
-    value = default_value
-    return dtype(value)
-
-
 class ConfigKeys(object):
     TRAIN_SPEED_RECORD_NUM = "train_speed_record_num"
     SECONDS_TO_START_AUTOSCALE_WORKER = "seconds_to_start_autoscale_worker"
     STEP_TO_ADJUST_WORKER = "step_to_adjust_worker"
     OPTIMIZE_WORKER_CPU_THRESHOLD = "optimize_worker_cpu_threshold"
     SECONDS_FOR_STABLE_WORKER_COUNT = "seconds_for_stable_worker_count"
     SECONDS_INTERVAL_TO_OPTIMIZE = "seconds_interval_to_optimize"
     FACTOR_TO_CUT_PENDING_CPU = "factor_to_cut_pending_cpu"
     SECONDS_TO_WAIT_PENDING_POD = "seconds_to_wait_pending_pod"
     SECONDS_HUGE_TRAINING_THRESHOLD = "seconds_huge_training_threshold"
     GLOBAL_STEP_COUNT_TO_AUTO_WORKER = "global_step_count_to_auto_worker"
+    SECONDS_TO_CHANGE_PS = "seconds_to_change_ps"
+    SECONDS_TO_WAIT_FAILED_PS = "seconds_to_wait_failed_ps"
 
 
 class DefaultConfigValues(object):
     DEFAULT_TRAIN_SPEED_RECORD_NUM = 50
     DEFAULT_SECENDS_TO_START_AUTOSCALE_WORKER = 90
     DEFAULT_STEP_TO_ADJUST_WORKER = 200
     DEFAULT_OPTIMIZED_WORKER_CPU_THRESHOLD = 20
     DEFAULT_SECONDS_FOR_STABLE_WORKER_COUNT = 60
     DEFAULT_SECONDS_INTERVAL_TO_OPTIMIZE = 300
     DEFAULT_FACTOR_TO_CUT_PENDING_CPU = 2
     DEFAULT_SECONDS_TO_WAIT_PENDING_POD = 900  # 15min
     DEFAULT_SECONDS_HUGE_TRAINING_THRESHOLD = 1800  # 30min
     DEFALUT_GLOBAL_STEP_COUNT_TO_AUTO_WORKER = 5
+    DEFAULT_SECONDS_TO_CHANGE_PS = 3600  # 1h
+    DEFAULT_SECONDS_TO_WAIT_FAILED_PS = 600  # 10min
 
 
 class Context(object):
     _instance_lock = threading.Lock()
 
     def __init__(self):
-        self.train_speed_record_num = get_param_value_from_easydl(
+        self.train_speed_record_num = self.get_param_value_from_brain(
             ConfigKeys.TRAIN_SPEED_RECORD_NUM,
             DefaultConfigValues.DEFAULT_TRAIN_SPEED_RECORD_NUM,
         )
-        self.seconds_to_autoscale_worker = get_param_value_from_easydl(
+        self.seconds_to_autoscale_worker = self.get_param_value_from_brain(
             ConfigKeys.SECONDS_TO_START_AUTOSCALE_WORKER,
             DefaultConfigValues.DEFAULT_SECENDS_TO_START_AUTOSCALE_WORKER,
         )
-        self.step_to_adjust_worker = get_param_value_from_easydl(
+        self.step_to_adjust_worker = self.get_param_value_from_brain(
             ConfigKeys.STEP_TO_ADJUST_WORKER,
             DefaultConfigValues.DEFAULT_STEP_TO_ADJUST_WORKER,
         )
-        self.optimize_worker_cpu_threshold = get_param_value_from_easydl(
+        self.optimize_worker_cpu_threshold = self.get_param_value_from_brain(
             ConfigKeys.OPTIMIZE_WORKER_CPU_THRESHOLD,
             DefaultConfigValues.DEFAULT_OPTIMIZED_WORKER_CPU_THRESHOLD,
         )
-        self.seconds_for_stable_worker_count = get_param_value_from_easydl(
+        self.seconds_for_stable_worker_count = self.get_param_value_from_brain(
             ConfigKeys.SECONDS_FOR_STABLE_WORKER_COUNT,
             DefaultConfigValues.DEFAULT_SECONDS_FOR_STABLE_WORKER_COUNT,
         )
-        self.seconds_interval_to_optimize = get_param_value_from_easydl(
+        self.seconds_interval_to_optimize = self.get_param_value_from_brain(
             ConfigKeys.SECONDS_INTERVAL_TO_OPTIMIZE,
             DefaultConfigValues.DEFAULT_SECONDS_INTERVAL_TO_OPTIMIZE,
         )
-        self.factor_to_cut_pending_cpu = get_param_value_from_easydl(
+        self.factor_to_cut_pending_cpu = self.get_param_value_from_brain(
             ConfigKeys.FACTOR_TO_CUT_PENDING_CPU,
             DefaultConfigValues.DEFAULT_FACTOR_TO_CUT_PENDING_CPU,
         )
-        self.seconds_to_wait_pending_pod = get_param_value_from_easydl(
+        self.seconds_to_wait_pending_pod = self.get_param_value_from_brain(
             ConfigKeys.SECONDS_TO_WAIT_PENDING_POD,
             DefaultConfigValues.DEFAULT_SECONDS_TO_WAIT_PENDING_POD,
         )
-        self.seconds_huge_training_threshold = get_param_value_from_easydl(
+        self.seconds_huge_training_threshold = self.get_param_value_from_brain(
             ConfigKeys.SECONDS_HUGE_TRAINING_THRESHOLD,
             DefaultConfigValues.DEFAULT_SECONDS_HUGE_TRAINING_THRESHOLD,
         )
-        self.sample_count_to_adjust_worker = get_param_value_from_easydl(
+        self.sample_count_to_adjust_worker = self.get_param_value_from_brain(
             ConfigKeys.GLOBAL_STEP_COUNT_TO_AUTO_WORKER,
             DefaultConfigValues.DEFALUT_GLOBAL_STEP_COUNT_TO_AUTO_WORKER,
         )
+        self.seconds_interval_to_change_ps = self.get_param_value_from_brain(
+            ConfigKeys.SECONDS_TO_CHANGE_PS,
+            DefaultConfigValues.DEFAULT_SECONDS_TO_CHANGE_PS,
+        )
+        self.seconds_to_wait_failed_ps = self.get_param_value_from_brain(
+            ConfigKeys.SECONDS_TO_WAIT_FAILED_PS,
+            DefaultConfigValues.DEFAULT_SECONDS_TO_WAIT_FAILED_PS,
+        )
         self.auto_worker_enabled = False
         self.auto_ps_enabled = False
         self.is_tfv1_ps = False
-        self.launch_worker_after_ps_running = False
+        self.master_port = 0
+        self.relaunch_error = False
         self.print_config()
 
+    def config_master_port(self, port=0):
+        if port > 0:
+            self.master_port = port
+        else:
+            self.master_port = find_free_port_in_range(50001, 65535)
+
+    def get_param_value_from_brain(self, key_name, default_value, dtype=int):
+        """TODO: Get the configured value from Brain service."""
+        value = default_value
+        return dtype(value)
+
     def print_config(self):
         logger.info("DLRover global context = {}".format(self.__dict__))
 
     @property
     def user_id(self):
         return os.getenv(UserEnv.USER_ID, "")
```

## dlrover/python/common/grpc.py

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 The ElasticDL Authors. All rights reserved.
+# Copyright 2020 The DLRover Authors. All rights reserved.
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
@@ -13,14 +13,17 @@
 
 import socket
 from contextlib import closing
 
 import grpc
 
 from dlrover.python.common.constants import GRPC
+from dlrover.python.common.log import default_logger as logger
+
+TIMEOUT_SEC = 5
 
 
 def build_channel(addr):
     if not addr:
         return None
     channel = grpc.insecure_channel(
         addr,
@@ -39,12 +42,29 @@
 "retryableStatusCodes": [ "UNAVAILABLE" ] } }""",
             ),
         ],
     )
     return channel
 
 
-def find_free_port():
+def find_free_port(port=0):
     with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as s:
-        s.bind(("", 0))
+        s.bind(("", port))
         s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         return s.getsockname()[1]
+
+
+def find_free_port_in_range(start, end):
+    for i in range(start, end):
+        try:
+            return find_free_port(i)
+        except OSError as e:
+            logger.info("Socket creation attempt failed.", exc_info=e)
+    return RuntimeError(f"Fail to find a free port in [{start}, {end})")
+
+
+def grpc_server_ready(channel) -> bool:
+    try:
+        grpc.channel_ready_future(channel).result(timeout=TIMEOUT_SEC)
+        return True
+    except grpc.FutureTimeoutError:
+        return False
```

## dlrover/python/common/node.py

```diff
@@ -8,14 +8,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
+import time
+
+from kubernetes.utils.quantity import parse_quantity
 
 from dlrover.python.common.constants import (
     NodeExitReason,
     NodeResourceLimit,
     NodeStatus,
     PriorityClass,
 )
@@ -28,30 +31,30 @@
     try:
         float(str_number)
         return True
     except ValueError:
         return False
 
 
-class NodeResource(object):
+class NodeResource(JsonSerializable):
     """NodeResource records a resource of a Node.
     Attributes:
         cpu: float, CPU cores.
         memory: float, memory MB.
         gpu_type: str, the type of GPU.
         gpu_num: int,
         image: the image name of the node.
         priority: the priority classs of the node.
     """
 
     def __init__(
         self,
         cpu,
         memory,
-        gpu_type=None,
+        gpu_type="",
         gpu_num=0,
         priority="",
         **kwargs,
     ):
         self.cpu = cpu
         self.memory = memory
         self.gpu_type = gpu_type
@@ -86,21 +89,23 @@
             if "nvidia.com" in key:
                 gpu_type = key
                 gpu_num = int(resource[key])
         return NodeResource(cpu, memory, gpu_type, gpu_num)
 
     @classmethod
     def convert_memory_to_mb(cls, memory: str):
-        unit = memory[-2:]
-        value = int(memory[0:-2])
-        if unit == "Gi":
-            value = value * 1024
-        elif unit == "Ki":
-            value = int(value / 1024)
-        return value
+        return int(parse_quantity(memory) / 1024 / 1024)
+
+    @classmethod
+    def convert_memory_to_byte(cls, memory: str):
+        return parse_quantity(memory)
+
+    @classmethod
+    def convert_cpu_to_decimal(cls, cpu: str):
+        return round(float(parse_quantity(cpu)), 1)
 
 
 class NodeGroupResource(JsonSerializable):
     """The node group resource contains the number of the task
     and resource (cpu, memory) of each task.
     Args:
         count: int, the number of task.
@@ -133,33 +138,38 @@
         status: the status of a node.
         start_time: int, the start timestamp of a node.
         rank_index: int, the rank index of a node in a training cluster.
         relaunch_count: int, the relaunched number of the training node.
         critical: bool, if true, the job will fail if the node fails.
         max_relaunch_count: int, the maximum to relaunch a node.
         relaunchable: bool, whether to relaunch a node if it fails.
-        is_released: bool, whether to released the node.
+        is_released: bool, ture if the master deletes the node.
         exit_reason: str, the exited reason of a node.
         used_resource: the resource usage of the node.
+        init_time: the timestamp to initialize the node object.
+        host_name: the name of the host where the node is placed.
+        host_ip: the ip of host node.
     """
 
     def __init__(
         self,
         node_type,
         node_id,
-        config_resource: NodeResource,
+        config_resource: NodeResource = NodeResource(0, 0),
         name=None,
         status=NodeStatus.INITIAL,
         start_time=None,
         rank_index=None,
         relaunch_count=0,
         critical=False,
         max_relaunch_count=0,
         relaunchable=True,
         service_addr=None,
+        host_name=None,
+        host_ip=None,
     ):
         self.type = node_type
         self.id = node_id
         self.name = name
         self.status = status
         self.start_time = start_time
         self.rank_index = rank_index if rank_index is not None else node_id
@@ -171,54 +181,77 @@
         self.create_time = None
         self.finish_time = None
         self.is_recovered_oom = False
         self.is_released = False
         self.exit_reason = None
         self.config_resource = config_resource
         self.used_resource = NodeResource(0.0, 0.0)
+        self.start_hang_time = 0
+        self.init_time = time.time()
+        self.eval_time = 0
+        self.host_name = host_name
+        self.host_ip = host_ip
 
     def inc_relaunch_count(self):
         self.relaunch_count += 1
 
     def update_info(
         self,
         name=None,
         start_time=None,
         create_time=None,
+        host_name=None,
+        host_ip=None,
     ):
         if name is not None:
             self.name = name
         if start_time is not None:
             self.start_time = start_time
         if create_time is not None:
             self.create_time = create_time
+        if host_name:
+            self.host_name = host_name
+        if host_ip:
+            self.host_ip = host_ip
 
     def update_status(self, status=None):
         if status is not None:
             self.status = status
 
     def update_resource_usage(self, cpu, memory):
         self.used_resource.cpu = round(cpu, 2)
         self.used_resource.memory = memory
+        if cpu < 0.1:
+            self.start_hang_time = time.time()
+        else:
+            self.start_hang_time = 0
+
+    def update_service_address(self, service_addr):
+        self.service_addr = service_addr
 
     def get_relaunch_node_info(self, new_id):
         new_node = copy.deepcopy(self)
         new_node.id = new_id
         new_node.name = None
         new_node.status = NodeStatus.INITIAL
         new_node.start_time = None
         new_node.is_released = False
         new_node.relaunchable = True
+        new_node.init_time = time.time()
         return new_node
 
     def is_unrecoverable_failure(self):
+        cpu_memory_overload = (
+            self.config_resource.gpu_num == 0
+            and self.config_resource.memory >= NodeResourceLimit.MAX_MEMORY
+        )
         if (
             self.relaunch_count >= self.max_relaunch_count
             or self.exit_reason == NodeExitReason.FATAL_ERROR
-            or self.config_resource.memory >= NodeResourceLimit.MAX_MEMORY
+            or cpu_memory_overload
         ):
             return True
         return False
 
     def set_exit_reason(self, reason):
         self.exit_reason = reason
 
@@ -244,7 +277,26 @@
             else:
                 self.config_resource.priority = PriorityClass.LOW
         elif priority not in [None, "", PriorityClass.HIGH, PriorityClass.LOW]:
             raise ValueError(
                 "Not support priority = {}, please set priority = "
                 "high/low/a fraction value.".format(priority)
             )
+
+    def timeout(self, timeout):
+        now = time.time()
+        if (
+            now - self.init_time > timeout
+            and self.status == NodeStatus.INITIAL
+        ):
+            return True
+
+    def __repr__(self):
+        return (
+            f"name:{self.name};"
+            f"rank_index:{self.rank_index};"
+            f"type:{self.type};"
+            f"status:{self.status};"
+            f"addr:{self.service_addr};"
+            f"is_released:{self.is_released};"
+            f"priroity:{self.config_resource.priority}"
+        )
```

## dlrover/python/elastic_agent/master_client.py

```diff
@@ -17,15 +17,15 @@
 import time
 from contextlib import closing
 from typing import Dict
 
 from google.protobuf import empty_pb2
 
 from dlrover.proto import elastic_training_pb2, elastic_training_pb2_grpc
-from dlrover.python.common.constants import NodeEnv
+from dlrover.python.common.constants import NetworkFailureReason, NodeEnv
 from dlrover.python.common.grpc import build_channel
 from dlrover.python.common.log import default_logger as logger
 
 
 def retry_grpc_request(func):
     def wrapper(self, *args, **kwargs):
         retry = kwargs.get("retry", 10)
@@ -37,16 +37,17 @@
                 logger.warning(
                     "Retry %s to %s.%s with failure",
                     i,
                     self.__class__.__name__,
                     func.__name__,
                 )
                 execption = e
-                time.sleep(15)
+                time.sleep(5)
         if execption:
+            logger.error(execption)
             raise execption
 
     return wrapper
 
 
 class MasterClient(object):
     """MasterClient provides some APIs connect with the master
@@ -64,24 +65,26 @@
     def __init__(self, master_addr, node_id, node_type):
         """Initialize a master client.
         Args:
             master_addr: the master address
 
             worker_id: int
             the unique and ordered worker ID assigned
-            by elasticdl command-line.
+            by dlrover command-line.
         """
         self._master_addr = master_addr
         self._channel = build_channel(master_addr)
+        logger.info("dlrover master addr is %s" % self._master_addr)
         self._stub = elastic_training_pb2_grpc.MasterStub(self._channel)
         self._node_id = node_id
         self._node_type = node_type
         self._host = os.getenv("MY_POD_IP", "localhost")
         self._worker_local_process_id = int(os.getenv("LOCAL_RANK", 0))
         self._ddp_server_port = self.find_free_port()
+        self._host_name = os.getenv("POD_NAME", "")
 
     def __del__(self):
         self._channel.close()
 
     def close_channel(self):
         self._channel.close()
 
@@ -99,41 +102,44 @@
             return port
 
     def get_task(self, dataset_name):
         """Get a task from master.
 
         Args:
             dataset_name: string
-            the training phase, c.f. /elasticdl/proto/elasticdl.proto
+            the training phase, c.f. /dlrover/proto/dlrover.proto
 
         Returns:
             the task unit assigned by master,
-            c.f. /elasticdl/proto/elasticdl.proto
+            c.f. /dlrover/proto/dlrover.proto
         """
 
         req = elastic_training_pb2.GetTaskRequest()
         req.worker_type = self._node_type
         req.worker_id = self._node_id
         req.dataset_name = dataset_name
 
         success = False
         res = None
+        exception = None
         for _ in range(10):
             try:
                 res = self._stub.get_task(req)
                 success = True
                 break
             except Exception as e:
-                logger.warning(e)
+                exception = e
                 time.sleep(15)
+        if not success:
+            logger.warning(exception)
         if not res:
             res = elastic_training_pb2.Task()
         return success, res
 
-    # @retry_grpc_request
+    @retry_grpc_request
     def report_task_result(self, dataset_name, task_id, err_msg):
         """Report task result to master.
 
         Args:
           task_id: int
           the task ID assigned by master
 
@@ -143,46 +149,14 @@
         request = elastic_training_pb2.ReportTaskResultRequest()
         request.dataset_name = dataset_name
         request.task_id = task_id
         request.err_message = err_msg
         return self._stub.report_task_result(request)
 
     @retry_grpc_request
-    def reset_sync(self, rendezvous_id):
-        req = elastic_training_pb2.DdpResetSyncRequest()
-        req.rendezvous_id = rendezvous_id
-        req.worker_host = self._host
-        req.worker_local_process_id = self._worker_local_process_id
-        return self._stub.reset_sync(req)
-
-    @retry_grpc_request
-    def barrier_sync(self, rendezvous_id):
-        req = elastic_training_pb2.DdpInitSyncRequest()
-        req.rendezvous_id = rendezvous_id
-        req.worker_host = self._host
-        req.worker_local_process_id = self._worker_local_process_id
-        return self._stub.barrier_sync(req)
-
-    @retry_grpc_request
-    def get_comm_rank(self):
-        req = elastic_training_pb2.GetCommRankRequest()
-        req.worker_host = self._host
-        req.worker_local_process_id = self._worker_local_process_id
-        return self._stub.get_comm_rank(req)
-
-    @retry_grpc_request
-    def report_training_loop_status(self, status):
-        req = elastic_training_pb2.ReportTrainingLoopStatusRequest()
-        req.worker_host = self._host
-        req.worker_local_process_id = self._worker_local_process_id
-        req.status = status
-        req.ddp_server_port = self._ddp_server_port
-        return self._stub.report_training_loop_status(req)
-
-    @retry_grpc_request
     def report_dataset_shard_params(
         self,
         batch_size,
         num_epochs=None,
         dataset_size=None,
         shuffle=False,
         num_minibatches_per_shard=0,
@@ -227,15 +201,15 @@
         request.cpu = cpu
         request.node_id = self._node_id
         request.node_type = self._node_type
         return self._stub.report_used_resource(request)
 
     @retry_grpc_request
     def get_dataset_epoch(self, dataset_name):
-        request = elastic_training_pb2.GetDatasetEpochRequest()
+        request = elastic_training_pb2.DatasetMeta()
         request.dataset_name = dataset_name if dataset_name else ""
         return self._stub.get_dataset_epoch(request)
 
     @retry_grpc_request
     def report_model_metric(self, tensor_stats, op_stats):
         metric_msg = elastic_training_pb2.ModelMetric()
         tensor_msg = metric_msg.tensor_stats
@@ -247,15 +221,14 @@
 
         op_msg = metric_msg.op_stats
         op_msg.op_count = op_stats.op_count
         op_msg.update_op_count = op_stats.update_op_count
         op_msg.read_op_count = op_stats.read_op_count
         op_msg.input_fetch_dur = op_stats.input_fetch_dur
         op_msg.flops = op_stats.flops
-        op_msg.runtime_flops = int(op_stats.runtime_flops)
         op_msg.recv_op_count = op_stats.recv_op_count
         return self._stub.report_model_metric(metric_msg)
 
     @retry_grpc_request
     def report_global_step(self, global_step, timestamp):
         record = elastic_training_pb2.GlobalStepRecord()
         record.global_step = global_step
@@ -266,48 +239,181 @@
     def get_cluster_version(self, version_type, task_type, task_id):
         request = elastic_training_pb2.GetClusterVersionRequest()
         request.task_id = task_id
         request.version_type = version_type
         request.task_type = task_type
         return self._stub.get_cluster_version(request)
 
+    def update_node_addr(self, task_type, task_id, node_addr):
+        request = elastic_training_pb2.NodeMeta()
+        request.id = task_id
+        request.type = task_type
+        request.addr = node_addr
+        request.rank = -1
+        res = self._stub.update_node_status(request)
+        return res
+
+    @retry_grpc_request
+    def update_node_event(self, task_type, task_id, event):
+        request = elastic_training_pb2.NodeEvent()
+        request.node.id = task_id
+        request.node.type = task_type
+        request.message = "train_success"
+        request.event_type = "1"
+        return self._stub.update_node_event(request)
+
     @retry_grpc_request
     def update_cluster_version(
         self, version_type, version, task_type, task_id
     ):
         request = elastic_training_pb2.UpdateClusterVersionRequest()
         request.task_id = task_id
         request.version_type = version_type
         request.version = version
         request.task_type = task_type
         self._stub.update_cluster_version(request)
 
-    @retry_grpc_request
     def query_ps_nodes(self):
         request = empty_pb2.Empty()
         response = self._stub.query_ps_nodes(request)
-        return response.ps_nodes, response.new_ps_ready
+        return response.ps_nodes, response.ps_failure
 
     @retry_grpc_request
     def query_training_status(self):
         request = empty_pb2.Empty()
         response = self._stub.query_training_status(request)
         return response.status
 
+    @retry_grpc_request
+    def get_dataset_shard_num(self, dataset_name):
+        request = elastic_training_pb2.DatasetMeta()
+        request.dataset_name = dataset_name
+        response = self._stub.get_dataset_shard_num(request)
+        return response.shard_num
+
+    @retry_grpc_request
+    def join_sync(self, sync_name):
+        request = elastic_training_pb2.SyncRequest()
+        request.sync_name = sync_name
+        request.worker_id = self._node_id
+        request.worker_type = self._node_type
+        logger.info(
+            " {}:{} join sync {}".format(
+                self._node_id, self._node_type, sync_name
+            )
+        )
+        return self._stub.join_sync(request)
+
+    @retry_grpc_request
+    def sync_finished(self, sync_name):
+        request = elastic_training_pb2.SyncRequest()
+        request.sync_name = sync_name
+        return self._stub.sync_finished(request)
+
+    @retry_grpc_request
+    def barrier(self, barrier_name, notify=False):
+        request = elastic_training_pb2.BarrierRequest()
+        request.barrier_name = barrier_name
+        request.notify = notify
+        return self._stub.barrier(request)
+
     def report_prestop(self):
         req = elastic_training_pb2.ReportPreStopRequest()
         req.worker_host = self._host
         logger.info("Worker {} report prestop hook".format(self._host))
         return self._stub.report_prestop(req)
 
     def get_running_nodes(self):
         request = empty_pb2.Empty()
         response = self._stub.query_running_nodes(request)
         return response.nodes
 
+    @retry_grpc_request
+    def num_nodes_waiting(self, rdzv_name):
+        request = elastic_training_pb2.RendezvousRequest()
+        request.rdzv_name = rdzv_name
+        response = self._stub.num_nodes_waiting(request)
+        return response.waiting_num
+
+    @retry_grpc_request
+    def join_rendezvous(self, rank_id, local_world_size, rdzv_name=""):
+        request = elastic_training_pb2.RendezvousRequest()
+        request.node_id = rank_id
+        request.local_world_size = local_world_size
+        request.rdzv_name = rdzv_name
+        response = self._stub.join_rendezvous(request)
+        return response.round
+
+    @retry_grpc_request
+    def get_comm_world(self, rdzv_name, rank_id):
+        request = elastic_training_pb2.RendezvousRequest()
+        request.node_id = rank_id
+        request.rdzv_name = rdzv_name
+        response = self._stub.get_comm_world(request)
+        return response.group, response.world
+
+    @retry_grpc_request
+    def network_check_success(self, timeout=300):
+        request = elastic_training_pb2.RendezvousRequest()
+        start = time.time()
+        while True:
+            response = self._stub.network_check_success(request)
+            if (
+                response.reason == NetworkFailureReason.WAITING_NODE
+                and time.time() - start < timeout
+            ):
+                time.sleep(5)
+                continue
+            break
+        return response.success
+
+    @retry_grpc_request
+    def report_rdzv_params(
+        self, min_nodes, max_nodes, waiting_timeout, node_unit
+    ):
+        request = elastic_training_pb2.RendezvousParams()
+        request.min_nodes = min_nodes
+        request.max_nodes = max_nodes
+        request.waiting_timeout = waiting_timeout
+        request.node_unit = node_unit
+        response = self._stub.report_rdzv_params(request)
+        return response.success
+
+    @retry_grpc_request
+    def kv_store_set(self, key, value):
+        request = elastic_training_pb2.KeyValuePair()
+        request.key = key
+        request.value = value
+        response = self._stub.kv_store_set(request)
+        return response.success
+
+    @retry_grpc_request
+    def kv_store_get(self, key):
+        request = elastic_training_pb2.KeyValuePair()
+        request.key = key
+        response = self._stub.kv_store_get(request)
+        return response.value
+
+    @retry_grpc_request
+    def report_node_status(self, rank_id, status):
+        request = elastic_training_pb2.NodeMeta()
+        request.id = rank_id
+        request.type = self._node_type
+        request.status = status
+        self._stub.update_node_status(request)
+
+    @retry_grpc_request
+    def report_failures(self, error_data, restart_count=-1):
+        request = elastic_training_pb2.NodeFailure()
+        request.node_id = self._node_id
+        request.node_type = self._node_type
+        request.error_data = error_data
+        request.restart_count = restart_count
+        self._stub.report_failure(request)
+
 
 class LocalDataset(object):
     def __init__(
         self,
         batch_size,
         num_epochs,
         dataset_size,
@@ -325,15 +431,15 @@
         self._task_type = task_type
 
     def create_tasks(self):
         start = 0
         if self._records_per_shard <= 0:
             raise ValueError(
                 "records_per_shard {} can not be less than 1".format(
-                    self._record_per_shard
+                    self._records_per_shard
                 )
             )
         while start < self._dataset_size:
             end = min(start + self._records_per_shard, self._dataset_size)
             self._todo.append((start, end))
             start = end
         if self._shuffle:
@@ -363,20 +469,22 @@
     """
 
     def __init__(self, node_id):
         """Initialize a master client.
         Args:
             worker_id: int
             the unique and ordered worker ID assigned
-            by elasticdl command-line.
+            by dlrover command-line.
         """
         self._node_id = node_id
         self._num_minibatches_per_shard = 0
         self._datasets: Dict[str, LocalDataset] = {}
         self._task_type = None
+        self._kv_store: Dict[str, str] = {}
+        self._rdzv_nodes: Dict[int, int] = {}
 
     def reset_dataset(self, dataset_name):
         """Reset a dataset
 
         Args:
             dataset_name: name of the dataset, must not be None.
         """
@@ -384,19 +492,19 @@
         dataset.reset()
 
     def get_task(self, dataset_name):
         """Get a task from master.
 
         Args:
             dataset_name: string
-            the training phase, c.f. /elasticdl/proto/elasticdl.proto
+            the training phase, c.f. /dlrover/proto/dlrover.proto
 
         Returns:
             the task unit assigned by master,
-            c.f. /elasticdl/proto/elasticdl.proto
+            c.f. /dlrover/proto/dlrover.proto
         """
 
         shard = elastic_training_pb2.Shard()
         res = elastic_training_pb2.Task(shard=shard)
         dataset = self._datasets.get(dataset_name, None)
         if dataset:
             start, end = dataset.get_task()
@@ -417,27 +525,15 @@
           the error message on training.
 
           exec_counters: dict
           statistics of the task being executed.
         """
         return empty_pb2.Empty()
 
-    def get_comm_rank(self):
-        res = elastic_training_pb2.GetCommRankResponse()
-        res.rank_id = 0
-        res.world_size = 1
-        res.rendezvous_id = 0
-        res.rendezvous_port = 12345
-        res.local_rank = 0
-        res.local_size = 1
-        res.cross_rank = 0
-        res.cross_size = 1
-        return res
-
-    def report_training_loop_status(self, status):
+    def update_node_event(self, task_type, task_id, enent):
         return True
 
     def report_dataset_shard_params(
         self,
         batch_size,
         num_epochs=None,
         dataset_size=None,
@@ -467,22 +563,57 @@
 
     def report_model_metric(self, *args):
         return empty_pb2.Empty()
 
     def report_used_resource(self, memory, cpu):
         return empty_pb2.Empty()
 
+    def num_nodes_waiting(self, rdzv_name=""):
+        return 0
+
+    def join_rendezvous(
+        self, node_id, local_world_size, rdzv_name="", round=0
+    ):
+        self._rdzv_nodes[node_id] = local_world_size
+        return 0
+
+    def get_comm_world(self, *args, **kwarg):
+        return 0, self._rdzv_nodes
+
+    def network_check_success(self, node_id):
+        return True
+
+    def report_node_status(self, normal):
+        return True
+
+    def report_rdzv_params(
+        self, min_nodes, max_nodes, waiting_timeout, node_unit
+    ):
+        return True
+
+    def kv_store_set(self, key, value):
+        self._kv_store[key] = value
+        logger.info(self._kv_store)
+        return True
+
+    def kv_store_get(self, key):
+        return self._kv_store.get(key, "".encode())
+
+    def report_failures(self, error_data, restart_count=-1):
+        return True
+
 
 def build_master_client(master_addr=None):
     if master_addr is None:
-        master_addr = os.getenv(NodeEnv.MASTER_ADDR, "")
+        master_addr = os.getenv(NodeEnv.DLROVER_MASTER_ADDR, "")
     worker_id = int(os.getenv(NodeEnv.WORKER_ID, 0))
     worker_type = os.getenv(NodeEnv.WORKER_TYPE, "worker")
 
     if master_addr:
+        logger.info("Build master client to connect with the DLRover master.")
         master_client = MasterClient(master_addr, worker_id, worker_type)
     else:
         master_client = LocalMasterClient(worker_id)
     return master_client
 
 
 class GlobalMasterClient(object):
```

## dlrover/python/elastic_agent/monitor/resource.py

```diff
@@ -13,14 +13,15 @@
 
 import os
 import threading
 import time
 
 import psutil
 
+from dlrover.python.common.constants import NodeEnv
 from dlrover.python.common.log import default_logger as logger
 from dlrover.python.common.singleton import singleton
 from dlrover.python.elastic_agent.master_client import GlobalMasterClient
 
 
 def get_process_cpu_percent():
     """Get the cpu percent of the current process."""
@@ -45,27 +46,29 @@
         cpu_percent = 0.0
     return cpu_percent / 100.0
 
 
 def get_used_memory():
     """ "Get the used memory of the container"""
     mem = psutil.virtual_memory()
-    used_mem = mem.total - mem.available
-    return int(used_mem / 1024 / 1024)
+    return int(mem.used / 1024 / 1024)
 
 
 @singleton
 class ResourceMonitor(object):
     def __init__(self):
         """
         The monitor samples the used memory and cpu percent
-        reports the used memory and cpu percent to the ElasticDL master.
+        reports the used memory and cpu percent to the DLRover master.
         """
         self._total_cpu = psutil.cpu_count(logical=True)
-        if os.getenv("DLROVER_MASTER_ADDR", ""):
+        if (
+            os.getenv(NodeEnv.DLROVER_MASTER_ADDR, "")
+            and os.getenv(NodeEnv.AUTO_MONITOR_WORKLOAD, "") == "true"
+        ):
             threading.Thread(
                 target=self._monitor_resource,
                 name="monitor_resource",
                 daemon=True,
             ).start()
 
     def start_monitor_cpu(self):
```

## dlrover/python/elastic_agent/monitor/training.py

```diff
@@ -46,24 +46,24 @@
     def set_start_time(self):
         if self._start_time == 0:
             timestamp = int(time.time())
             self._last_timestamp = timestamp
             self._start_time = timestamp
             self._resource_monitor.start_monitor_cpu()
             logger.info(
-                "Start training process reporter in TF hooks : %s",
+                "Start training process reporter in training hooks : %s",
                 self.called_in_tf_hook,
             )
 
     def report_resource_with_step(self, step):
         if not self._is_tf_chief:
             return
         try:
             timestamp = int(time.time())
-            if step > 0 and timestamp - self._last_timestamp > 15:
+            if step > 0 and timestamp - self._last_timestamp > 30:
                 self._resource_monitor.report_resource()
                 logger.info("Report global step = {}".format(step))
                 self._last_timestamp = timestamp
                 GlobalMasterClient.MASTER_CLIENT.report_global_step(
                     step, self._last_timestamp
                 )
         except Exception as e:
```

## dlrover/python/elastic_agent/sharding/client.py

```diff
@@ -1,64 +1,98 @@
-# Copyright 2020 The ElasticDL Authors. All rights reserved.
+# Copyright 2020 The DLRover Authors. All rights reserved.
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import os
+import sys
 import threading
 import time
 from collections import OrderedDict
+from multiprocessing import SimpleQueue
 
 from dlrover.proto import elastic_training_pb2
+from dlrover.python.common.log import default_logger as logger
 from dlrover.python.elastic_agent.master_client import GlobalMasterClient
 from dlrover.python.elastic_agent.monitor.training import (
     TrainingProcessReporter,
 )
 
 training_reporter = TrainingProcessReporter()
 
+_DEFAULT_MINI_BATCH_NUM_PER_SHARD = 10
+
 
 class ShardingClient(object):
+    """ShardingClient queries data shards from the DLRover master.
+    Args:
+        dataset_name: the name of dataset.
+        batch_size: the size of batch data.
+        num_epochs: the number of epochs.
+        dataset_size: the size of dataset.
+        shuffle: whether to shuffle shards.
+        task_type: Task type is the computation type like
+            elastic_training_pb2.TRAINING, elastic_training_pb2.EVALUATION.
+        num_minibatches_per_shard: the number of batch in each shard.
+        storage_type: the storage type of dataset. It is "text" if the
+            dataset is stored in a text file. It is "table" if the
+            dataset is stored in a table like MaxCompute and Hive.
+    Example:
+        batch_size = 64
+        client = ShardingClient(
+            datset_name="test",
+            batch_size=batch_size,
+            num_epochs=1,
+            dataset_size=10000,
+        )
+        while True:
+            shard = client.fetch_shard()
+            if not shard:
+                break
+            for i in range(shard.start, shard.end):
+                print(i)
+                if i % batch_size == 0:
+                    client.report_batch_done()
+    """
+
     def __init__(
         self,
         dataset_name,
         batch_size,
-        num_epochs=None,
-        dataset_size=None,
+        num_epochs,
+        dataset_size,
         shuffle=False,
         task_type=elastic_training_pb2.TRAINING,
-        num_minibatches_per_shard=0,
-        master_client=None,
+        num_minibatches_per_shard=_DEFAULT_MINI_BATCH_NUM_PER_SHARD,
         storage_type="",
     ):
-        self._mc = (
-            master_client
-            if master_client
-            else GlobalMasterClient.MASTER_CLIENT
-        )
+        self._mc = GlobalMasterClient.MASTER_CLIENT
         self._batch_size = batch_size
         self._num_epochs = num_epochs
         self._dataset_size = dataset_size
         self._shuffle = shuffle
         self._task_type = task_type
         self._storage_type = storage_type
         self._num_minibatches_per_shard = num_minibatches_per_shard
         self._lock = threading.Lock()
         self._reported_record_count = {}
         self._current_task = None
         self._pending_tasks = OrderedDict()
         self._dataset_name = dataset_name
         self._batch_count = 0
+        self._max_shard_count = sys.maxsize
+        self._shard_count = 0
         self._report_sharding_params()
 
     def _report_sharding_params(self):
         if self._num_epochs and self._dataset_size:
             self._mc.report_dataset_shard_params(
                 batch_size=self._batch_size,
                 num_epochs=self._num_epochs,
@@ -76,26 +110,29 @@
     def reset_dataset(self):
         # Only dataset with a name will be reset.
         self._mc.reset_dataset(self._dataset_name)
 
     def get_current_task(self):
         return self._current_task
 
-    def get_task(self):
+    def get_task(self) -> elastic_training_pb2.Task:
         training_reporter.set_start_time()
+        if self._shard_count >= self._max_shard_count:
+            return None
         for _ in range(5):
             success, task = self._mc.get_task(self._dataset_name)
             if success:
                 break
             time.sleep(5)
         if task.shard.end - task.shard.start > 0:
             with self._lock:
                 self._pending_tasks[task.task_id] = task
                 if len(self._pending_tasks) == 1:
                     self._current_task = task
+            self._shard_count += 1
             return task
         return None
 
     def _report_task(self, task, err_msg=""):
         self._mc.report_task_result(
             self._dataset_name,
             task.task_id,
@@ -185,8 +222,115 @@
 
     def restore_shard_from_checkpoint(self, shard_checkpoint):
         res = self._mc.report_shard_checkpoint(shard_checkpoint)
         return res.success
 
     def get_current_epoch(self):
         res = self._mc.get_dataset_epoch(self._dataset_name)
-        return res.epoch
+        return res.epoch - 1
+
+    def get_total_sample_num(self):
+        return self._dataset_size * self._num_epochs
+
+    def set_max_shard_count(self):
+        world_size = int(os.getenv("WORLD_SIZE", 0))
+        if world_size:
+            total_shard_count = self._mc.get_dataset_shard_num(
+                self._dataset_name
+            )
+            if total_shard_count == 0:
+                return
+            self._max_shard_count = total_shard_count // world_size
+            logger.info(
+                "The max number of shards is %s", self._max_shard_count
+            )
+
+
+class IndexShardingClient(ShardingClient):
+    """ShardingClient queries data shards from the DLRover master
+    and generates the index of sample from the shard.
+    Users can read data from the disk by the sample index.
+    Args:
+        dataset_name: the name of dataset.
+        batch_size: the size of batch data.
+        num_epochs: the number of epochs.
+        dataset_size: the size of dataset.
+        shuffle: whether to shuffle shards.
+        task_type: Task type is the computation type like
+            elastic_training_pb2.TRAINING, elastic_training_pb2.EVALUATION.
+        num_minibatches_per_shard: the number of batch in each shard.
+        storage_type: the storage type of dataset. It is "text" if the
+            dataset is stored in a text file. It is "table" if the
+            dataset is stored in a table like MaxCompute and Hive.
+        num_workers: the number of worker processes to share the client
+            to get the sample index.
+    """
+
+    def __init__(
+        self,
+        dataset_name,
+        batch_size,
+        num_epochs,
+        dataset_size,
+        shuffle=False,
+        task_type=elastic_training_pb2.TRAINING,
+        num_minibatches_per_shard=_DEFAULT_MINI_BATCH_NUM_PER_SHARD,
+        storage_type="",
+        num_workers=1,
+    ):
+        super(IndexShardingClient, self).__init__(
+            dataset_name,
+            batch_size,
+            num_epochs,
+            dataset_size,
+            shuffle,
+            task_type,
+            num_minibatches_per_shard,
+            storage_type,
+        )
+        self._num_workers = num_workers
+        self._sample_queue = SimpleQueue()
+        self._report_sharding_params()
+
+        threading.Thread(
+            target=self._prefetch_sample_indices,
+            name="fetch_sample_indices",
+            daemon=True,
+        ).start()
+
+    def _prefetch_sample_indices(self):
+        while True:
+            if self._sample_queue.empty():
+                task = self.get_task()
+                if not task or not task.shard:
+                    for _ in range(128):
+                        self._sample_queue.put(None)
+                    break
+                ids = (
+                    task.shard.indices
+                    if task.shard.indices
+                    else list(range(task.shard.start, task.shard.end))
+                )
+                for i in ids:
+                    self._sample_queue.put(i)
+            else:
+                time.sleep(0.001)
+
+    def fetch_sample_index(self):
+        """Fetch an index of the sample. The function get an index
+        from a queue because there may be multiple sub-process to call
+        the function.
+        """
+        index = self._sample_queue.get()
+        if index is None:
+            logger.info("No more data.")
+            raise StopIteration()
+        return index
+
+    def clear_shard_queue(self):
+        self._sample_queue = SimpleQueue()
+
+    def restore_shard_from_checkpoint(self, shard_checkpoint):
+        # To avoid duplicate shards, drop all shards in the _shard_queue
+        # before restoring shard from checkpoint
+        # self.clear_shard_queue()
+        super().restore_shard_from_checkpoint(shard_checkpoint)
```

## dlrover/python/elastic_agent/tensorflow/hooks.py

```diff
@@ -57,15 +57,15 @@
     tensor_stats.update_varible_stats(tf.global_variables())
     return tensor_stats, op_stats
 
 
 class ReportModelMetricHook(SessionRunHook):
     def __init__(self):
         """Report variables and operators in a model to
-        the ElasticDL master.
+        the DLRover master.
         """
         self._is_chief = False
         training_reporter.called_in_tf_hook = True
         self._global_step = 0
         self._op_stats = None
         self._tensor_stats = None
         super(ReportModelMetricHook, self).__init__()
```

## dlrover/python/master/args.py

```diff
@@ -27,14 +27,22 @@
     )
     parser.add_argument(
         "--platform",
         default="pyk8s",
         type=str,
         help="The name of platform",
     )
+    parser.add_argument(
+        "--relaunch_error",  # should be in "--foo" format
+        nargs="?",
+        const=not False,
+        default=False,
+        type=lambda x: x.lower() in ["true", "yes", "t", "y"],
+        help=help,
+    )
 
 
 def print_args(args, exclude_args=[], groups=None):
     """
     Args:
         args: parsing results returned from `parser.parse_args`
         exclude_args: the arguments which won't be printed.
@@ -72,15 +80,15 @@
     return res
 
 
 def _build_master_args_parser():
     parser = argparse.ArgumentParser(description="Training Master")
     parser.add_argument(
         "--port",
-        default=50001,
+        default=0,
         type=pos_int,
         help="The listening port of master",
     )
     add_params(parser)
     return parser
```

## dlrover/python/master/main.py

```diff
@@ -33,16 +33,18 @@
     _dlrover_context.print_config()
 
 
 def run(args):
     job_args = new_job_args(args.platform, args.job_name, args.namespace)
     job_args.initilize()
     logger.info("Job args : %s", job_args.toJSON())
+    _dlrover_context.config_master_port(port=args.port)
+    _dlrover_context.relaunch_error = args.relaunch_error
     update_context(job_args)
-    master = Master(args.port, job_args)
+    master = Master(_dlrover_context.master_port, job_args)
     master.prepare()
     return master.run()
 
 
 def main():
     args = parse_master_args()
     exit_code = run(args)
```

## dlrover/python/master/master.py

```diff
@@ -7,187 +7,207 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
 import time
+from typing import Dict
 
 from dlrover.python.common.constants import (
     DistributionStrategy,
     JobExitReason,
     NodeType,
+    OptimizeMode,
+    RendezvousName,
+    ReporterType,
 )
 from dlrover.python.common.log import default_logger as logger
 from dlrover.python.master.elastic_training.elastic_ps import ElasticPsService
+from dlrover.python.master.elastic_training.rdzv_manager import (
+    ElasticTrainingRendezvousManager,
+    NetworkCheckRendezvousManager,
+    RendezvousManager,
+)
+from dlrover.python.master.elastic_training.sync_service import SyncService
 from dlrover.python.master.monitor.speed_monitor import SpeedMonitor
 from dlrover.python.master.node.event_callback import (
+    AllReduceNodeHandlingCallback,
     TaskRescheduleCallback,
     TFPSNodeHandlingCallback,
 )
-from dlrover.python.master.node.node_manager import create_node_manager
+from dlrover.python.master.node.job_manager import create_job_manager
 from dlrover.python.master.servicer import create_master_service
 from dlrover.python.master.shard.task_manager import TaskManager
 from dlrover.python.master.stats.job_collector import JobMetricCollector
 from dlrover.python.scheduler.job import JobArgs
 
 
-def _create_rendezvous_server_if_needed(params: JobArgs):
-    master_ip = os.getenv("MY_POD_IP", "localhost")
-    if params.use_ddp:
-        logger.info("call DDPRendezvousServer, master_ip:{}".format(master_ip))
-        return None
-    elif params.distribution_strategy != DistributionStrategy.ALLREDUCE:
-        return None
-    else:
-        logger.info(
-            "call HorovodRendezvousServer, master_ip:{}".format(master_ip)
-        )
-        return None
-
-
 def _create_elastic_ps_service_if_needed(params: JobArgs):
-    if params.distribution_strategy == DistributionStrategy.PARAMETER_SERVER:
+    if params.distribution_strategy == DistributionStrategy.PS:
         return ElasticPsService()
     return None
 
 
 class Master(object):
     def __init__(self, port, args: JobArgs):
         self.speed_monitor = SpeedMonitor()
-        self.node_manager = (
-            create_node_manager(args, self.speed_monitor)
+        self.job_manager = (
+            create_job_manager(args, self.speed_monitor)
             if args.enable_elastic_scheduling
             else None
         )
         self.task_manager = (
             TaskManager(
                 args.node_args[NodeType.WORKER].restart_timeout,
                 self.speed_monitor,
             )
             if args.enable_dynamic_sharding
             else None
         )
-        self.rendezvous_server = _create_rendezvous_server_if_needed(args)
+        elastic_training = RendezvousName.ELASTIC_TRAINING
+        self.rdzv_managers: Dict[str, RendezvousManager] = {
+            elastic_training: ElasticTrainingRendezvousManager(),
+            RendezvousName.NETWORK_CHECK: NetworkCheckRendezvousManager(),
+        }
         self.job_metric_collector = self._create_metric_collector_if_needed(
             args
         )
         self.elastic_ps_service = _create_elastic_ps_service_if_needed(args)
+        self.sync_service = SyncService(self.job_manager)
         self._master_server = self._create_master_grpc_service(port, args)
         self._job_args = args
         self._stop_requested = False
         self._exit_code = 0
         self._exit_reason = None
 
     def _create_master_grpc_service(self, port, params: JobArgs):
         return create_master_service(
             port,
             self.task_manager,
-            self.node_manager,
+            self.job_manager,
             self.speed_monitor,
-            self.rendezvous_server,
+            self.rdzv_managers,
             self.job_metric_collector,
             self.elastic_ps_service,
+            self.sync_service,
         )
 
     def _create_metric_collector_if_needed(self, params: JobArgs):
         if not params.enable_dynamic_sharding:
             return None
         job_uuid = params.job_uuid
+        reporter = ReporterType.LOCAL
+        if params.optimize_mode == OptimizeMode.CLUSTER:
+            reporter = ReporterType.DLROVER_BRAIN
         collector = JobMetricCollector(
-            job_uuid, params.namespace, params.cluster, params.user
+            job_uuid, params.namespace, params.cluster, params.user, reporter
         )
         collector.collect_job_type(params.distribution_strategy)
         return collector
 
     def prepare(self):
+        # Start the master GRPC server
+        logger.info("Starting master RPC server")
+        self._master_server.start()
+        logger.info("Master RPC server started")
+
         # Composite the components
-        if self.task_manager and self.node_manager:
+        if self.task_manager and self.job_manager:
             self.task_manager.set_task_timeout_callback(
-                self.node_manager.remove_worker
+                self.job_manager.remove_worker
             )
-        if self.node_manager:
+        if self.job_manager:
             self._add_node_event_callback()
 
         # Start the components one by one
         if self.task_manager:
             self.task_manager.start()
-        if self.rendezvous_server:
-            self.rendezvous_server.start()
-        if self.node_manager:
-            self.node_manager.start()
-
-        # Start the master GRPC server
-        logger.info("Starting master RPC server")
-        self._master_server.start()
-        logger.info("Master RPC server started")
+        if self.job_manager:
+            self.job_manager.start()
 
     def _add_node_event_callback(self):
         """Add NodeEventCallbacks for the listeners of Pod events."""
         if self.task_manager:
-            self.node_manager.add_node_event_callback(
+            self.job_manager.add_node_event_callback(
                 TaskRescheduleCallback(self.task_manager)
             )
-        if (
-            self._job_args.distribution_strategy
-            == DistributionStrategy.PARAMETER_SERVER
-        ):
-            self.node_manager.add_node_event_callback(
+        strategy = self._job_args.distribution_strategy
+        if strategy == DistributionStrategy.PS:
+            self.job_manager.add_node_event_callback(
                 TFPSNodeHandlingCallback(self)
             )
+        elif strategy == DistributionStrategy.ALLREDUCE:
+            self.job_manager.add_node_event_callback(
+                AllReduceNodeHandlingCallback(self)
+            )
 
     def run(self):
         """
         The main loop of master.
         Dispatch the tasks to the workers until all the tasks are completed.
         """
         try:
             while True:
                 if self._stop_requested:
                     break
-                if (
-                    self.node_manager
-                    and self.node_manager.all_workers_exited()
-                ):
-                    if self.node_manager.all_workers_failed():
+                if self.job_manager and self.job_manager.all_workers_exited():
+                    if self.job_manager.pend_without_workers():
+                        time.sleep(30)
+                        continue
+                    if self.job_manager.all_workers_failed():
                         logger.error("All workers failed")
                         self._exit_code = 1
                         self._exit_reason = JobExitReason.UNKNOWN_ERROR
-                        break
-
-                    if self.task_manager and not self.task_manager.finished():
+                    elif (
+                        self.task_manager and not self.task_manager.finished()
+                    ):
                         logger.warning(
                             "All workers exited but there also are "
                             "unfinished tasks",
                         )
                     break
 
                 if (
+                    self.job_manager.all_running_node_hanged()
+                    and self.task_manager.task_hanged()
+                ):
+                    logger.error("All nodes hangeds")
+                    self._exit_code = 1
+                    self._exit_reason = JobExitReason.UNKNOWN_ERROR
+
+                if (
                     self.task_manager
                     and self.task_manager.finished()
                     and (
-                        not self.node_manager
-                        or self.node_manager.all_critical_node_completed()
+                        not self.job_manager
+                        or self.job_manager.all_critical_node_completed()
                     )
                 ):
                     logger.info("All task completed")
                     break
 
                 time.sleep(30)
         except KeyboardInterrupt:
             logger.warning("Server stopping")
         finally:
-            if self.node_manager:
-                self.node_manager.stop()
+            if self.job_manager:
+                self.job_manager.stop()
             self.stop()
 
         return self._exit_code
 
+    def _remove_not_participated_workers(self):
+        """Remove workers who do not participate training."""
+        for manager in self.rdzv_managers.values():
+            ranks = manager.not_joined_rdzv_nodes()
+            if ranks:
+                self.job_manager.remove_not_joined_rdzv_workers(ranks)
+
     def stop(self):
         """
         Stop all the components.
         Make sure that the created services and components are shut down.
         """
         if self._exit_code == 0 and not self._exit_reason:
             self._exit_reason = JobExitReason.SUCCEEDED
```

## dlrover/python/master/servicer.py

```diff
@@ -10,55 +10,73 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import threading
 import time
 from concurrent import futures
-from typing import List
+from typing import Dict, List
 
 import grpc
 from google.protobuf import empty_pb2
 
 from dlrover.proto import elastic_training_pb2, elastic_training_pb2_grpc
-from dlrover.python.common.constants import GRPC, NodeType, TrainingLoopStatus
+from dlrover.python.common.constants import (
+    GRPC,
+    NodeStatus,
+    NodeType,
+    RendezvousName,
+    TrainingLoopStatus,
+)
 from dlrover.python.common.global_context import Context
 from dlrover.python.common.log import default_logger as logger
 from dlrover.python.master.elastic_training.elastic_ps import ElasticPsService
+from dlrover.python.master.elastic_training.kv_store_service import (
+    KVStoreService,
+)
+from dlrover.python.master.elastic_training.rdzv_manager import (
+    RendezvousManager,
+)
+from dlrover.python.master.elastic_training.sync_service import SyncService
 from dlrover.python.master.monitor.speed_monitor import SpeedMonitor
-from dlrover.python.master.node.node_manager import NodeManager
+from dlrover.python.master.node.job_manager import JobManager
 from dlrover.python.master.shard.dataset_splitter import new_dataset_splitter
 from dlrover.python.master.shard.task_manager import TaskManager
 from dlrover.python.master.stats.job_collector import JobMetricCollector
 from dlrover.python.master.stats.training_metrics import OpStats, TensorStats
-from dlrover.python.master.watcher.base_watcher import Node
+from dlrover.python.master.watcher.base_watcher import Node, NodeEvent
+from dlrover.python.util.queue.queue import RayEventQueue
 
 _dlrover_context = Context.singleton_instance()
 _DEFAULT_NUM_MINIBATCHES_PER_SHARD = 100
+ray_event_queue = RayEventQueue.singleton_instance()
 
 
 class MasterServicer(elastic_training_pb2_grpc.MasterServicer):
     """Master service implementation"""
 
     def __init__(
         self,
         task_manager: TaskManager,
-        node_manager: NodeManager,
+        job_manager: JobManager,
         speed_monitor: SpeedMonitor,
-        rendezvous_server=None,
+        rdzv_managers: Dict[str, RendezvousManager],
         job_metric_collector=None,
         elastic_ps_service=None,
+        sync_service=None,
     ):
         # TODO: group params together into a single object.
         self._task_manager = task_manager
-        self._node_manager = node_manager
+        self._job_manager = job_manager
         self._speed_monitor = speed_monitor
-        self._rendezvous_server = rendezvous_server
+        self._rdzv_managers = rdzv_managers
+        self._kv_store = KVStoreService()
         self._job_metric_collector: JobMetricCollector = job_metric_collector
         self._elastic_ps_service: ElasticPsService = elastic_ps_service
+        self._sync_service: SyncService = sync_service
         self._lock = threading.Lock()
         self._version = 0
         self._start_training_time = None
         self._start_autoscale = False
 
     def get_model_version(self):
         return self._version
@@ -67,25 +85,26 @@
         success = True
         if request.err_message:
             logger.warning("Worker reported error: " + request.err_message)
             success = False
         task, _ = self._task_manager.report_dataset_task(request, success)
         if (
             not self._start_autoscale
-            and self._node_manager
+            and self._job_manager
             and self._speed_monitor.completed_global_step == 0
             and int(time.time()) - self._start_training_time
             > _dlrover_context.seconds_to_autoscale_worker
         ):
             logger.info("Start autoscale for non-training jobs")
-            self._node_manager.start_auto_scale()
+            self._job_manager.start_auto_scaling()
             self._start_autoscale = True
 
         if (
             self._job_metric_collector
+            and task
             and task.task_type == elastic_training_pb2.PREDICTION
         ):
             self._collect_runtime_stats()
             self._check_start_auto_scale_worker()
         return empty_pb2.Empty()
 
     def get_task(self, request, _):
@@ -106,26 +125,15 @@
             res.task_id = task.task_id
             res.type = task.task_type
             res.shard.name = task.shard.name
             res.shard.start = task.shard.start
             res.shard.end = task.shard.end
             res.shard.indices.extend(task.shard.record_indices)
         elif not dataset.completed():
-            # If the todo and doing tasks are not empty,
-            # Otherwise if the callback list is not empty,
-            # we are trying to pop and invoke the callback.
-            # Then the master tells the worker to wait
-            # in case of new tasks later.
-            if self._rendezvous_server:
-                # If there is no more task, master only send wait task to
-                # the last worker and other workers exit.
-                if len(self._node_manager.get_running_workers()) == 1:
-                    res.type = elastic_training_pb2.WAIT
-            else:
-                res.type = elastic_training_pb2.WAIT
+            res.type = elastic_training_pb2.WAIT
         with self._lock:
             self._task_manager.reset_worker_start_task_time(request.worker_id)
         return res
 
     def report_dataset_shard_params(self, request, _):
         num_minibatches_per_task = (
             request.num_minibatches_per_shard
@@ -155,117 +163,42 @@
             )
             if request.task_type == elastic_training_pb2.TRAINING:
                 self._job_metric_collector.collect_training_hyper_params(
                     request.num_epochs, request.batch_size
                 )
         return empty_pb2.Empty()
 
-    def reset_sync(self, request, _):
-        rendezvous_id = request.rendezvous_id
-        worker_host = request.worker_host
-        worker_local_process_id = request.worker_local_process_id
-        res = elastic_training_pb2.DdpResetSyncResponse()
-        res.reset = self._rendezvous_server.reset_sync(
-            worker_host,
-            worker_local_process_id,
-            rendezvous_id,
-        )
-        return res
-
-    def barrier_sync(self, request, _):
-        rendezvous_id = request.rendezvous_id
-        worker_host = request.worker_host
-        worker_local_process_id = request.worker_local_process_id
-        res = elastic_training_pb2.DdpInitSyncResponse()
-        res.reset = self._rendezvous_server.barrier_sync(
-            worker_host,
-            worker_local_process_id,
-            rendezvous_id,
-        )
-        return res
-
-    def get_comm_rank(self, request, _):
-        worker_host = request.worker_host
-        worker_local_process_id = request.worker_local_process_id
-
-        res = elastic_training_pb2.GetCommRankResponse()
-        host_rank_info = self._rendezvous_server.get_worker_host_rank(
-            worker_host, worker_local_process_id
-        )
-        if host_rank_info[0] == "horovod":
-            res.rank_id = host_rank_info[1]
-            res.local_rank = host_rank_info[2]
-            res.local_size = host_rank_info[3]
-            res.cross_rank = host_rank_info[4]
-            res.cross_size = host_rank_info[5]
-            res.rendezvous_port = self._rendezvous_server.get_rendezvous_port()
-        elif host_rank_info[0] == "DDP":
-            res.rank_id = host_rank_info[1]
-            res.local_rank = host_rank_info[2]
-            res.local_size = host_rank_info[3]
-            res.master_addr = str(host_rank_info[4])
-            res.master_port = host_rank_info[5]
-        res.world_size = self._rendezvous_server.get_size()
-        res.rendezvous_id = self._rendezvous_server.get_rendezvous_id()
-        return res
-
-    def report_training_loop_status(self, request, _):
-        training_loop_status = request.status
-        worker_local_process_id = request.worker_local_process_id
-        worker_host = request.worker_host
-        ddp_server_port = request.ddp_server_port
-
-        if not self._rendezvous_server:
-            logger.warning("The rendezvous server does not exit")
-            return empty_pb2.Empty()
-
-        logger.info(
-            "Servicer get ddp_server_port:{} "
-            "from host:{} id:{}".format(
-                ddp_server_port, worker_host, worker_local_process_id
-            )
-        )
-        if training_loop_status == TrainingLoopStatus.START:
-            self._rendezvous_server.add_process(
-                worker_host, worker_local_process_id, ddp_server_port
-            )
-        if training_loop_status == TrainingLoopStatus.END:
-            self._rendezvous_server.remove_process(
-                worker_host, worker_local_process_id
-            )
-        return empty_pb2.Empty()
-
     def ready_for_ps_relaunch(self, request, _):
-        self._node_manager.post_ps_ready()
+        self._job_manager.post_ps_ready()
         return empty_pb2.Empty()
 
     def get_shard_checkpoint(self, request, _):
         res = elastic_training_pb2.ShardCheckpoint()
         dataset = self._task_manager.get_dataset(request.dataset_name)
         checkpoint = dataset.checkpoint()
         if checkpoint:
             res.content = checkpoint.to_json()
         else:
             res.content = ""
         return res
 
     def report_shard_checkpoint(self, request, _):
-        res = elastic_training_pb2.ReportShardCheckpointResponse()
+        res = elastic_training_pb2.Response()
         success = self._task_manager.restore_dataset_from_checkpoint(
             request.content
         )
         res.success = success
         return res
 
     def report_used_resource(self, request, _):
         cpu = request.cpu
-        memory = int(request.memory / 1024)  # Mi
+        memory = request.memory
         pod_id = request.node_id
         pod_type = request.node_type
-        self._node_manager.update_node_resource_usage(
+        self._job_manager.update_node_resource_usage(
             pod_type, pod_id, cpu, memory
         )
         return empty_pb2.Empty()
 
     def get_dataset_epoch(self, request, _):
         res = elastic_training_pb2.GetDatasetEpochResponse()
         dataset_name = request.dataset_name
@@ -278,14 +211,15 @@
                 variable_count=request.tensor_stats.variable_count,
                 total_variable_size=request.tensor_stats.total_variable_size,
                 max_variable_size=request.tensor_stats.max_variable_size,
             )
             op_stats = OpStats(
                 op_count=request.op_stats.op_count,
                 update_op_count=request.op_stats.update_op_count,
+                read_op_count=request.op_stats.read_op_count,
                 input_fetch_dur=request.op_stats.input_fetch_dur,
                 flops=request.op_stats.flops,
             )
             self._job_metric_collector.collect_model_metric(
                 tensor_stats,
                 op_stats,
             )
@@ -297,30 +231,30 @@
         )
         self._collect_runtime_stats()
         self._check_start_auto_scale_worker()
         return empty_pb2.Empty()
 
     def _collect_runtime_stats(self):
         if self._job_metric_collector:
-            nodes = self._node_manager.get_running_nodes()
+            nodes = self._job_manager.get_running_nodes()
             self._job_metric_collector.collect_runtime_stats(
                 self._speed_monitor, nodes
             )
 
     def _check_start_auto_scale_worker(self):
         sample_count = self._speed_monitor.get_sample_count()
         if (
             not self._start_autoscale
             and sample_count >= _dlrover_context.sample_count_to_adjust_worker
         ):
             logger.info(
                 "Start autoscale with %s stats samples",
                 sample_count,
             )
-            self._node_manager.start_auto_scale()
+            self._job_manager.start_auto_scaling()
             self._start_autoscale = True
 
     def get_cluster_version(self, request, _):
         response = elastic_training_pb2.GetClusterVersionResponse()
         if not self._elastic_ps_service:
             return response
 
@@ -344,64 +278,207 @@
             )
         elif request.task_type == NodeType.PS:
             self._elastic_ps_service.update_ps_version(
                 request.task_id, request.version_type, request.version
             )
         return empty_pb2.Empty()
 
+    def update_node_status(self, request, _):
+        node_type = request.type
+        node_id = request.id
+        server_addr = request.addr
+
+        if server_addr:
+            self._job_manager.update_node_service_addr(
+                node_type, node_id, server_addr
+            )
+        node_status = request.status
+        if node_status:
+            net_rdzv_manager = self._rdzv_managers.get(
+                RendezvousName.NETWORK_CHECK, None
+            )
+            if net_rdzv_manager:
+                succeed = request.status == NodeStatus.SUCCEEDED
+                net_rdzv_manager.report_network_check_result(node_id, succeed)
+
+        response = elastic_training_pb2.Response()
+        response.success = True
+        return response
+
+    def update_node_event(self, request, _):
+
+        event_type = request.event_type
+        message = request.message
+        event = {
+            "event_type": event_type,
+            "message": message,
+            "id": request.node.id,
+            "type": request.node.type,
+        }
+        node = Node(request.node.type, request.node.id)
+        event = NodeEvent("exit", node)
+        ray_event_queue.put(event)
+        return empty_pb2.Empty()
+
     def query_ps_nodes(self, request, _):
-        training_ps: List[Node] = self._node_manager.get_next_cluster_ps()
-        ready = self._node_manager.ready_for_new_ps_cluster()
+        training_ps: List[Node] = self._job_manager.get_next_cluster_ps()
+        ready = self._job_manager.ready_for_new_ps_cluster()
+        ps_failure = self._job_manager.has_ps_failure()
         res = elastic_training_pb2.QueryPsNodesResponse()
         for ps in training_ps:
             ps_meta = res.ps_nodes.add()
             ps_meta.type = NodeType.PS
             ps_meta.addr = ps.service_addr
             ps_meta.cpu = ps.config_resource.cpu
-            ps_meta.memory = ps.config_resource.memory
+            ps_meta.memory = int(ps.config_resource.memory)
+        logger.info("PS nodes : %s", res)
         res.new_ps_ready = ready
+        res.ps_failure = ps_failure
         return res
 
     def query_running_nodes(self, request, _):
-        nodes: List[Node] = self._node_manager.get_all_running_nodes()
+        nodes: List[Node] = self._job_manager.get_running_nodes()
         res = elastic_training_pb2.RunningNodes()
         for node in nodes:
             meta = elastic_training_pb2.NodeMeta()
             meta.type = node.type
             meta.addr = node.service_addr
             meta.cpu = node.config_resource.cpu
             meta.memory = node.config_resource.memory
             if node.config_resource.gpu_type:
                 meta.gpu_type = node.config_resource.gpu_type
-                meta.gpu_num = node.config_resource.gpu_num
+                meta.gpu = node.config_resource.gpu_num
             res.nodes.append(meta)
         return res
 
     def query_training_status(self, request, _):
         res = elastic_training_pb2.QueryTrainingStatusResponse()
         if self._task_manager.training_started():
             res.status = TrainingLoopStatus.START
         else:
             res.status = TrainingLoopStatus.PENDING
         return res
 
+    def get_dataset_shard_num(self, request, _):
+        res = elastic_training_pb2.DatasetMeta()
+        dataset = self._task_manager.get_dataset(request.dataset_name)
+        res.dataset_name = request.dataset_name
+        res.shard_num = dataset.get_task_count()
+        return res
+
     def report_prestop(self, request, _):
-        worker_host = request.worker_host
-        self._rendezvous_server.report_prestop(worker_host)
         return empty_pb2.Empty()
 
+    def join_sync(self, request, _):
+        res = elastic_training_pb2.Response()
+        res.success = self._sync_service.join_sync(
+            request.sync_name, request.worker_type, request.worker_id
+        )
+        return res
+
+    def sync_finished(self, request, _):
+        res = elastic_training_pb2.Response()
+        res.success = self._sync_service.sync_finished(request.sync_name)
+        return res
+
+    def barrier(self, request, _):
+        res = elastic_training_pb2.Response()
+        if request.notify:
+            res.success = self._sync_service.notify_barrier(
+                request.barrier_name
+            )
+        else:
+            res.success = self._sync_service.barrier(request.barrier_name)
+        return res
+
+    def get_comm_world(self, request, _):
+        rdzv_manager = self._rdzv_managers[request.rdzv_name]
+        group, nodes = rdzv_manager.get_comm_world(request.node_id)
+        res = elastic_training_pb2.RendezvousState()
+        res.group = group
+        for rank_id, worker_num in nodes.items():
+            res.world[rank_id] = worker_num
+        return res
+
+    def join_rendezvous(self, request, _):
+        rdzv_manager = self._rdzv_managers[request.rdzv_name]
+        round = rdzv_manager.join_rendezvous(
+            request.node_id, request.local_world_size
+        )
+        res = elastic_training_pb2.RendezvousState()
+        res.round = round
+        return res
+
+    def num_nodes_waiting(self, request, _):
+        waiting_num = 0
+        for rdzv_manager in self._rdzv_managers.values():
+            num = rdzv_manager.num_nodes_waiting()
+            waiting_num = max(num, waiting_num)
+        res = elastic_training_pb2.RendezvousState()
+        res.waiting_num = waiting_num
+        return res
+
+    def report_rdzv_params(self, request, _):
+        # Enable auto-scaling workers if elasticity is enabled.
+        _dlrover_context.auto_worker_enabled = (
+            request.max_nodes > request.min_nodes
+        )
+        for manager in self._rdzv_managers.values():
+            manager.update_rdzv_params(
+                min_nodes=request.min_nodes,
+                max_ndoes=request.max_nodes,
+                waiting_timeout=request.waiting_timeout,
+                node_unit=request.node_unit,
+            )
+        self._job_manager.update_allreduce_node_unit(request.node_unit)
+        res = elastic_training_pb2.Response()
+        res.success = True
+        return res
+
+    def kv_store_set(self, request, _):
+        self._kv_store.set(request.key, request.value)
+        res = elastic_training_pb2.Response()
+        res.success = True
+        return res
+
+    def kv_store_get(self, request, _):
+        res = elastic_training_pb2.KeyValuePair()
+        res.key = request.key
+        res.value = self._kv_store.get(request.key)
+        return res
+
+    def report_failure(self, request, _):
+        self._job_manager.handle_training_failure(
+            request.node_type,
+            request.node_id,
+            request.restart_count,
+            request.error_data,
+        )
+        res = elastic_training_pb2.Response()
+        res.success = True
+        return res
+
+    def network_check_success(self, request, _):
+        res = elastic_training_pb2.Response()
+        net_rdzv_manager = self._rdzv_managers[RendezvousName.NETWORK_CHECK]
+        success, reason = net_rdzv_manager.network_check_success()
+        res.success = success
+        res.reason = reason
+        return res
+
 
 def create_master_service(
     port,
     task_manager,
-    node_manager,
+    job_manager,
     speed_monitor,
-    rendezvous_server,
+    rdzv_managers,
     job_metric_collector,
     elastic_ps_service,
+    sync_service,
 ) -> MasterServicer:
     """Create GRPC server"""
     logger.info("Creating master service")
     server = grpc.server(
         futures.ThreadPoolExecutor(max_workers=64),
         options=[
             ("grpc.max_send_message_length", GRPC.MAX_SEND_MESSAGE_LENGTH),
@@ -409,20 +486,22 @@
                 "grpc.max_receive_message_length",
                 GRPC.MAX_RECEIVE_MESSAGE_LENGTH,
             ),
         ],
     )
     master_servicer = MasterServicer(
         task_manager=task_manager,
-        node_manager=node_manager,
+        job_manager=job_manager,
         speed_monitor=speed_monitor,
-        rendezvous_server=rendezvous_server,
+        rdzv_managers=rdzv_managers,
         job_metric_collector=job_metric_collector,
         elastic_ps_service=elastic_ps_service,
+        sync_service=sync_service,
     )
 
     elastic_training_pb2_grpc.add_MasterServicer_to_server(
         master_servicer, server
     )
     server.add_insecure_port("[::]:{}".format(port))
     logger.info("The port of the master server is: %d", port)
+
     return server
```

## dlrover/python/master/elastic_training/elastic_ps.py

```diff
@@ -19,14 +19,15 @@
     def __init__(self):
         self._global_version = 0
         self._ps_local_version = {}
         self._worker_local_version = {}
         self._worker_restored_version = {}
 
     def inc_global_cluster_version(self):
+        logger.info("Increment the global version to %s", self._global_version)
         self._global_version += 1
 
     def get_ps_version(self, version_type, ps_id):
         if version_type == PSClusterVersionType.GLOBAL:
             return self._global_version
         elif version_type == PSClusterVersionType.LOCAL:
             return self._ps_local_version.get(ps_id, 0)
```

## dlrover/python/master/monitor/speed_monitor.py

```diff
@@ -8,15 +8,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import time
-from typing import List, Set, Tuple
+from typing import Dict, List, Set, Tuple
 
 from dlrover.python.common.global_context import Context
 from dlrover.python.common.log import default_logger as logger
 
 _dlrover_context = Context.singleton_instance()
 
 
@@ -30,26 +30,33 @@
 
     def __init__(self, global_step, timestamp, worker_num):
         self.global_step = global_step
         self.timestamp = timestamp
         self.worker_num = worker_num
 
 
+class EvaluationTime(object):
+    def __init__(self):
+        self.start_eval = 0
+        self.eval_time = 0
+
+
 class SpeedMonitor(object):
     """Monitor the training speed by the number of batch per second"""
 
     def __init__(self):
         self._global_step_records: List[GlobalStepRecord] = []
         self._workers: Set[Tuple[str, int]] = set()
         self._max_record_count = _dlrover_context.train_speed_record_num
         self._global_step = 0
         self._target_worker_num = 0
         self._init_time = time.time()
         self._start_training_time = None
         self._sample_count = 0
+        self._worker_eval_times: Dict[int, EvaluationTime] = {}
 
     def set_target_worker_num(self, worker_num):
         """Set the target number of workers"""
         self._target_worker_num = worker_num
         logger.info(
             "The target number of worker : %s", self._target_worker_num
         )
@@ -135,16 +142,41 @@
         return self._global_step
 
     @property
     def running_workers(self):
         return self._workers
 
     def reset_running_speed_monitor(self):
-        """Reest the speed monitor"""
+        """Reset the speed monitor by clearing the record of global records
+        and running workers."""
         self._global_step_records = []
+        self._workers = set()
+
+    def set_worker_start_eval_time(self, worker_id):
+        self._worker_eval_times.setdefault(worker_id, EvaluationTime())
+        self._worker_eval_times[worker_id].start_eval = time.time()
+
+    def update_worker_eval_time(self, worker_id):
+        if worker_id in self._worker_eval_times:
+            eval_time = self._worker_eval_times[worker_id]
+            if eval_time.start_eval > 0:
+                eval_time.eval_time += time.time() - eval_time.start_eval
+                eval_time.start_eval = 0
+
+    def get_worker_eval_time(self, worker_id):
+        if worker_id in self._worker_eval_times:
+            eval = self._worker_eval_times[worker_id]
+            if eval.start_eval > 0:
+                eval.eval_time += time.time() - eval.start_eval
+                eval.start_eval = 0
+            return eval.eval_time
+        return 0
+
+    def all_worker_joined(self):
+        return len(self._workers) == self._target_worker_num
 
     def worker_adjustment_finished(self):
         """Check the number of workers is equal to the target
         in the enough time, such 5min"""
         if not self._global_step_records:
             return False
         worker_num = self._global_step_records[-1].worker_num
```

## dlrover/python/master/node/event_callback.py

```diff
@@ -9,27 +9,32 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import abc
 from datetime import datetime
+from typing import Dict
 
 from dlrover.python.common.constants import (
     JobExitReason,
     NodeExitReason,
     NodeType,
 )
 from dlrover.python.common.log import default_logger as logger
+from dlrover.python.master.elastic_training.rdzv_manager import (
+    RendezvousManager,
+)
+from dlrover.python.master.monitor.speed_monitor import SpeedMonitor
 from dlrover.python.master.watcher.base_watcher import Node
 
 
 class ClusterContext(object):
-    def __init__(self, node_manager):
-        self.node_manager = node_manager
+    def __init__(self, job_manager):
+        self.job_manager = job_manager
 
 
 class NodeEventCallback(metaclass=abc.ABCMeta):
     """
     The interface for the observers that are interested in the node event.
     The subclass observers can override the following methods to handle
     various events.
@@ -148,42 +153,126 @@
     @NodeEventCallback.log_callback_exception
     def on_node_started(self, node: Node, cluster_context):
         pass
 
     @NodeEventCallback.log_callback_exception
     def on_node_succeeded(self, node: Node, cluster_context: ClusterContext):
         node.finish_time = datetime.now()  # type: ignore
-        node_manager = cluster_context.node_manager
+        job_manager = cluster_context.job_manager
         if node.critical:
-            completed = node_manager.all_critical_node_completed()
+            completed = job_manager.all_critical_node_completed()
             if completed:
                 self._master.request_stop(
                     success=True,
                     reason=JobExitReason.SUCCEEDED,
                     msg="All critical nodes completed",
                 )
         self._master.speed_monitor.remove_running_worker(node.type, node.id)
+        self._master.sync_service.remove_exited_worker_sync(node.type, node.id)
 
     @NodeEventCallback.log_callback_exception
     def on_node_failed(self, node: Node, cluster_context):
         node.finish_time = datetime.now()  # type: ignore
         self._stop_job_if_needed(node)
+        if node.type == NodeType.PS:
+            self._master.elastic_ps_service.inc_global_cluster_version()
         if node.is_unrecoverable_failure():
             self._master.speed_monitor.reduce_target_worker_num(
                 [(node.type, node.id)]
             )
         self._master.speed_monitor.remove_running_worker(node.type, node.id)
+        self._master.sync_service.remove_exited_worker_sync(node.type, node.id)
 
     @NodeEventCallback.log_callback_exception
     def on_node_deleted(self, node, cluster_context):
         node.finish_time = datetime.now()  # type: ignore
-        self._stop_job_if_needed(
-            node,
-        )
+        self._stop_job_if_needed(node)
+        if node.type == NodeType.PS:
+            self._master.elastic_ps_service.inc_global_cluster_version()
         self._master.speed_monitor.remove_running_worker(node.type, node.id)
+        self._master.sync_service.remove_exited_worker_sync(node.type, node.id)
+
+    def _stop_job_if_needed(self, node: Node):
+        if node.critical and node.is_unrecoverable_failure():
+            job_exit_reason = self.get_job_exit_reason(node)
+            self._master.request_stop(
+                success=False,
+                reason=job_exit_reason,
+                msg=(
+                    "Critical node (type={}, id={}) is failed "
+                    "and {} relaunches have been exhausted.".format(
+                        node.type, node.id, node.max_relaunch_count
+                    )
+                ),
+            )
+
+
+class AllReduceNodeHandlingCallback(NodeEventCallback):
+    def __init__(self, master):
+        super(AllReduceNodeHandlingCallback, self).__init__()
+        self._master = master
+        self._speed_monitor: SpeedMonitor = self._master.speed_monitor
+        self._rdzv_managers: Dict[
+            str, RendezvousManager
+        ] = self._master.rdzv_managers
+
+    def get_job_exit_reason(self, node: Node):
+        if self._master.task_manager.training_started():
+            if node.type == NodeType.WORKER:
+                if node.exit_reason == NodeExitReason.OOM:
+                    return JobExitReason.WORKER_OOM
+                else:
+                    return JobExitReason.WORKER_ERROR
+            else:
+                return JobExitReason.UNKNOWN_ERROR
+        else:
+            return JobExitReason.CODE_ERROR
+
+    @NodeEventCallback.log_callback_exception
+    def on_node_started(self, node: Node, cluster_context):
+        if node.type == NodeType.WORKER and node.id == 0:
+            self._master.job_manager.start_auto_scaling()
+        for manager in self._rdzv_managers.values():
+            manager.add_alive_node(node)
+
+    @NodeEventCallback.log_callback_exception
+    def on_node_succeeded(self, node: Node, cluster_context: ClusterContext):
+        node.finish_time = datetime.now()  # type: ignore
+        job_manager = cluster_context.job_manager
+        if node.critical:
+            completed = job_manager.all_critical_node_completed()
+            if completed:
+                self._master.request_stop(
+                    success=True,
+                    reason=JobExitReason.SUCCEEDED,
+                    msg="All critical nodes completed",
+                )
+        self._speed_monitor.remove_running_worker(node.type, node.id)
+
+    @NodeEventCallback.log_callback_exception
+    def on_node_failed(self, node: Node, cluster_context):
+        node.finish_time = datetime.now()  # type: ignore
+        self._stop_job_if_needed(node)
+        if node.is_unrecoverable_failure():
+            self._master.speed_monitor.reduce_target_worker_num(
+                [(node.type, node.id)]
+            )
+        if node.exit_reason == NodeExitReason.HARDWARE_ERROR:
+            self._master.job_manager.handle_training_failure(
+                node.type, node.id, error_data=NodeExitReason.HARDWARE_ERROR
+            )
+        for manager in self._rdzv_managers.values():
+            manager.remove_alive_node(node)
+
+    @NodeEventCallback.log_callback_exception
+    def on_node_deleted(self, node, cluster_context):
+        node.finish_time = datetime.now()  # type: ignore
+        self._stop_job_if_needed(node)
+        for manager in self._rdzv_managers.values():
+            manager.remove_alive_node(node)
 
     def _stop_job_if_needed(self, node: Node):
         if node.critical and node.is_unrecoverable_failure():
             job_exit_reason = self.get_job_exit_reason(node)
             self._master.request_stop(
                 success=False,
                 reason=job_exit_reason,
```

## dlrover/python/master/node/ps.py

```diff
@@ -13,25 +13,24 @@
 
 import collections
 import copy
 import itertools
 import threading
 from typing import Dict, List
 
-from dlrover.python.common.constants import (
-    NodeResourceLimit,
-    NodeStatus,
-    NodeType,
-)
+from dlrover.python.common.constants import NodeStatus, NodeType
+from dlrover.python.common.global_context import Context
 from dlrover.python.common.log import default_logger as logger
 from dlrover.python.common.node import Node, NodeGroupResource, NodeResource
 from dlrover.python.master.node.training_node import TrainingNodeManager
 from dlrover.python.master.resource.job import JobResource
 from dlrover.python.master.scaler.base_scaler import ScalePlan
 
+_dlrover_ctx = Context.singleton_instance()
+
 
 class ParameterServerManager(TrainingNodeManager):
     def __init__(
         self,
         ps_nodes: Dict[int, Node],
         job_resource: JobResource,
         max_relaunch_num,
@@ -53,154 +52,188 @@
             ps_nodes, new_node_name_fn
         )
         self._max_relaunch_num = max_relaunch_num
         self._job_resource = job_resource
         self._new_service_fn = new_service_fn
         self._pre_dropped_ps: List[Node] = []
         self._lock = threading.Lock()
-        self._ready_for_new_ps_cluster = False
+        self._ps_cluster_changed = True
         self._migrated_ps_nodes: Dict[int, Node] = {}
         self._next_training_ps_cluster: List[Node] = []
         self._training_ps_cluster: List[Node] = []
         self._node_id_iter = itertools.count(self._job_resource.ps_num)
         self._init_training_ps_cluster()
 
     def _init_training_ps_cluster(self):
         for node in self._nodes.values():
+            alive = node.status in [
+                NodeStatus.INITIAL,
+                NodeStatus.PENDING,
+                NodeStatus.RUNNING,
+            ]
+            logger.info("PS : %s", node)
             if (
                 node.id not in self._migrated_ps_nodes
                 and not node.is_released
-                and node.status
-                in [NodeStatus.INITIAL, NodeStatus.PENDING, NodeStatus.RUNNING]
+                and alive
             ):
                 self._training_ps_cluster.append(node)
                 self._next_training_ps_cluster.append(node)
 
     def relaunch_node(self, node: Node):
         plan = ScalePlan()
         with self._lock:
             node.is_released = True
             new_id = next(self._node_id_iter)
             self._nodes[new_id] = node.get_relaunch_node_info(new_id)
+            self._nodes.pop(node.id)
             if node in self._training_ps_cluster:
                 i = self._training_ps_cluster.index(node)
                 self._training_ps_cluster[i] = self._nodes[new_id]
         logger.info("Relaunch node %s to %s", node.name, new_id)
         plan.launch_nodes.append(
             Node(
                 node.type,
                 new_id,
                 copy.deepcopy(node.config_resource),
                 rank_index=node.rank_index,
                 name=self._new_node_name_fn(node.type, new_id),
                 service_addr=node.service_addr,
+                relaunch_count=node.relaunch_count,
             )
         )
+        self._ps_cluster_changed = True
         return plan
 
     def adjust_ps(self, ps_resource: NodeGroupResource):
         logger.info(
             "Adjust ps resource to num = %s, cpu = %s, memory = %sMi",
             ps_resource.count,
             ps_resource.node_resource.cpu,
             ps_resource.node_resource.memory,
         )
+        plan = ScalePlan()
         alive_num = len(self.get_training_ps_cluster())
+        logger.info("The current number of alive PS is %s", alive_num)
         if ps_resource.count > alive_num:
-            self._scale_up_ps(ps_resource.count - alive_num)
+            new_ps = self._scale_up_ps(ps_resource.count - alive_num)
+            plan.launch_nodes.extend(new_ps)
         elif ps_resource.count < alive_num:
             self._scale_down_ps(alive_num - ps_resource.count)
+        return plan
 
     def _scale_up_ps(self, up_num):
         logger.info("Scale up ps with the number %s", up_num)
+        new_ps = []
         with self._lock:
-            self._ready_for_new_ps_cluster = False
-            task_id_iter = itertools.count(self._job_resource.ps_num)
+            self._ps_cluster_changed = True
+            alive_num = len(self.get_training_ps_cluster())
+            task_id_iter = itertools.count(alive_num)
             for _ in range(up_num):
                 ps_id = next(self._node_id_iter)
                 task_id = next(task_id_iter)
                 service_addr = self._new_service_fn(NodeType.PS, ps_id)
                 ps_resource = self._job_resource.get_node_group_resource(
                     NodeType.PS
                 ).node_resource
-                self._nodes[ps_id] = Node(
+                ps = Node(
                     NodeType.PS,
                     node_id=ps_id,
                     rank_index=task_id,
                     name=self._new_node_name_fn(NodeType.PS, ps_id),
                     max_relaunch_count=self._max_relaunch_num,
                     config_resource=copy.deepcopy(ps_resource),
                     critical=True,
                     service_addr=service_addr,
                 )
+                self._nodes[ps_id] = ps
+                new_ps.append(ps)
+                logger.info("Create PS %s", ps)
+        return new_ps
 
     def _scale_down_ps(self, down_num):
         with self._lock:
             self._pre_dropped_ps = []
-            self._ready_for_new_ps_cluster = False
+            self._ps_cluster_changed = True
             new_ps_num = self._job_resource.ps_num - down_num
             self._job_resource.update_node_group_resource(
                 NodeType.PS, new_ps_num, 0, 0
             )
             running_ps = self._get_alive_ps()
-            for pod in reversed(running_ps):
+            for node in reversed(running_ps):
                 if down_num <= 0:
                     break
-                self._pre_dropped_ps.append(pod)
+                self._pre_dropped_ps.append(node)
                 down_num -= 1
         dropped_ps = [ps.name for ps in self._pre_dropped_ps]
         logger.info("Scale down PS %s", dropped_ps)
 
     def process_after_ps_cluster_ready(self):
-        self._ready_for_new_ps_cluster = True
+        self._ps_cluster_changed = False
         self._training_ps_cluster = []
+        logger.info("Process PS nodes after ps training is ready")
         self._training_ps_cluster.extend(self._next_training_ps_cluster)
+        logger.info(
+            "Update training PS cluster = %s", self._training_ps_cluster
+        )
         plan = ScalePlan()
         with self._lock:
             while self._pre_dropped_ps:
                 node = self._pre_dropped_ps.pop()
                 node.critical = False
                 node.relaunchable = False
                 node.is_released = True
                 if node.id in self._migrated_ps_nodes:
                     self._migrated_ps_nodes.pop(node.id)
-                plan.remove_nodes.append(node.name)
+                plan.remove_nodes.append(node)
         return plan
 
     def _get_alive_ps(self) -> List[Node]:
         """Get all running PS pods"""
         alive_ps = []
-        for pod_info in self._nodes.values():
-            if (
-                pod_info.status == NodeStatus.RUNNING
-                and not pod_info.is_released
-            ):
-                alive_ps.append(pod_info)
+        for node in self._nodes.values():
+            if node.status == NodeStatus.RUNNING and not node.is_released:
+                alive_ps.append(node)
         return alive_ps
 
     def get_next_training_ps_cluster(self):
         """Get the next training PS cluster.
         After rescaling PS, it should return the new PS set until
         all new PS are running. Otherwise, it returns the old PS set.
         """
-        if self._ready_for_new_ps_cluster:
+        if not self._ps_cluster_changed:
             return self._next_training_ps_cluster
 
         all_new_ps_ready = True
         for node in self._nodes.values():
-            if not node.is_released and node.status in [
-                NodeStatus.INITIAL,
-                NodeStatus.PENDING,
-            ]:
+            if self._wait_ps_node(node):
                 all_new_ps_ready = False
                 break
         if all_new_ps_ready:
             self._next_training_ps_cluster = self._get_all_non_migrated_ps()
         return self._next_training_ps_cluster
 
+    def _wait_ps_node(self, node: Node):
+        """Whether to wait the PS node is running"""
+        return (
+            not node.is_released
+            and not node.timeout(_dlrover_ctx.seconds_to_wait_failed_ps)
+            and node.status in [NodeStatus.INITIAL, NodeStatus.PENDING]
+        )
+
+    def has_ps_failure(self):
+        """
+        Check whether there is PS failure and the master does not relaunch
+        the failed PS node.
+        """
+        for node in self._nodes.values():
+            if node.timeout(_dlrover_ctx.seconds_to_wait_failed_ps):
+                return True
+        return False
+
     def _get_all_non_migrated_ps(self):
         """Get all running PS pods without migrated PS nodes for training"""
         training_ps = {}
         with self._lock:
             alive_ps = self._get_alive_ps()
             self._pre_drop_migrated_ps(alive_ps)
             for ps in alive_ps:
@@ -217,15 +250,16 @@
             if node.status != NodeStatus.RUNNING:
                 return
         for node in alive_ps:
             if (
                 node.id in self._migrated_ps_nodes
                 and node.status == NodeStatus.RUNNING
             ):
-                self._pre_dropped_ps.append(node)
+                if node not in self._pre_dropped_ps:
+                    self._pre_dropped_ps.append(node)
 
     def get_total_request_cpu(self):
         total_cpu = 0
         for node in self._get_alive_ps():
             total_cpu += node.config_resource.cpu
         return total_cpu
 
@@ -233,28 +267,30 @@
         """Get the ps nodes who are training."""
         if not self._training_ps_cluster:
             self._init_training_ps_cluster()
         training_ps: List[Node] = []
         for ps in self._training_ps_cluster:
             if not ps.is_released and ps.status != NodeStatus.FAILED:
                 training_ps.append(ps)
+        logger.info("training_ps_cluster is {}".format(training_ps))
         return training_ps
 
     def get_ready_for_new_ps_cluster(self):
-        return self._ready_for_new_ps_cluster
+        return not self._ps_cluster_changed
 
     def get_ps_addrs(self):
         """Get the address list of ps services"""
         ps_addrs = {}
         for ps in list(self._nodes.values()):
             if (
                 ps.id not in self._migrated_ps_nodes
                 and not ps.is_released
                 and ps.status
                 in [NodeStatus.INITIAL, NodeStatus.PENDING, NodeStatus.RUNNING]
+                and not ps.timeout(_dlrover_ctx.seconds_to_wait_failed_ps)
             ):
                 ps_addrs[ps.rank_index] = ps.service_addr
         ps_addrs = collections.OrderedDict(sorted(ps_addrs.items()))
         return list(ps_addrs.values())
 
     def delete_running_ps(self):
         """Delete all running ps pods"""
@@ -269,15 +305,15 @@
                 logger.info(
                     "Remove the pod {} after the worker-0 completed".format(
                         node.name
                     )
                 )
                 node.is_released = True
                 node.status = NodeStatus.DELETED
-                plan.remove_nodes.append(node.name)
+                plan.remove_nodes.append(node)
         return plan
 
     def migrate_parameter_servers(self, ps_nodes: Dict[str, NodeResource]):
         plan = ScalePlan()
         for name, resource in ps_nodes.items():
             node = self._migrate_parameter_server(
                 name, resource.cpu, resource.memory
@@ -295,28 +331,19 @@
             or original_pod.is_released
             or original_pod.status
             not in [NodeStatus.PENDING, NodeStatus.RUNNING]
         ):
             return
 
         resource = copy.deepcopy(original_pod.config_resource)
-        rate = NodeResourceLimit.PS_CPU_GROWTH_RATE
-        if cpu <= resource.cpu * rate and memory <= resource.memory:
-            logger.info(
-                "Skip the PS %s with CPU=%s, memory=%s",
-                original_pod.name,
-                cpu,
-                memory,
-            )
-            return None
         with self._lock:
-            self._ready_for_new_ps_cluster = False
+            self._ps_cluster_changed = True
             new_ps_id = next(self._node_id_iter)
-            resource.cpu = cpu if cpu > resource.cpu * rate else resource.cpu
-            resource.memory = memory if memory > 0 else resource.memory
+            resource.cpu = cpu
+            resource.memory = memory
             logger.info(
                 "resource memory = %s, cpu = %s", resource.memory, resource.cpu
             )
 
             service_addr = self._new_service_fn(NodeType.PS, new_ps_id)
             new_node = Node(
                 NodeType.PS,
```

## dlrover/python/master/node/status_flow.py

```diff
@@ -18,15 +18,15 @@
 NodeStateFlow = namedtuple(
     "NodeStateFlow",
     ("from_status", "to_status", "event_type", "phase", "should_relaunch"),
 )
 
 """
 The DAG for the state machine is in the issue
-https://github.com/sql-machine-learning/elasticdl/issues/2395#issue-753964852
+https://github.com/sql-machine-learning/dlrover/issues/2395#issue-753964852
 """
 NODE_STATE_FLOWS = [
     NodeStateFlow(
         from_status=NodeStatus.INITIAL,
         to_status=NodeStatus.PENDING,
         event_type=["ADDED", "MODIFIED"],
         phase="Pending",
@@ -36,14 +36,28 @@
         from_status=NodeStatus.INITIAL,
         to_status=NodeStatus.RUNNING,
         event_type=["ADDED", "MODIFIED"],
         phase="Running",
         should_relaunch=False,
     ),
     NodeStateFlow(
+        from_status=NodeStatus.INITIAL,
+        to_status=NodeStatus.FAILED,
+        event_type=["ADDED", "MODIFIED"],
+        phase="Failed",
+        should_relaunch=True,
+    ),
+    NodeStateFlow(
+        from_status=NodeStatus.INITIAL,
+        to_status=NodeStatus.DELETED,
+        event_type=["DELETED"],
+        phase=None,
+        should_relaunch=True,
+    ),
+    NodeStateFlow(
         from_status=NodeStatus.PENDING,
         to_status=NodeStatus.RUNNING,
         event_type=["ADDED", "MODIFIED"],
         phase="Running",
         should_relaunch=False,
     ),
     NodeStateFlow(
```

## dlrover/python/master/node/training_node.py

```diff
@@ -13,21 +13,22 @@
 
 import copy
 import itertools
 import math
 import threading
 import time
 from collections import Counter
-from typing import Dict
+from typing import Dict, List
 
 from dlrover.python.common.constants import (
     DistributionStrategy,
     NodeResourceLimit,
     NodeStatus,
     NodeType,
+    PriorityClass,
 )
 from dlrover.python.common.global_context import Context
 from dlrover.python.common.log import default_logger as logger
 from dlrover.python.common.node import Node
 from dlrover.python.master.scaler.base_scaler import ScalePlan
 from dlrover.python.scheduler.job import JobArgs
 
@@ -84,18 +85,15 @@
             workers and the value is the relaunchable count of the worker.
     """
     critical_worker_index = {}
     worker_params = params.node_args[NodeType.WORKER]
 
     if worker_params.critical_nodes == "":
         # for default, worker0 is critical if PS strategy with custom training
-        if (
-            params.distribution_strategy
-            == DistributionStrategy.PARAMETER_SERVER
-        ):
+        if params.distribution_strategy == DistributionStrategy.PS:
             critical_worker_index[0] = worker_params.restart_count
     elif worker_params.critical_nodes == "all":
         for i in range(worker_params.group_resource.count):
             critical_worker_index[i] = worker_params.restart_count
     elif worker_params.critical_nodes != "none":
         for pod_relaunch_conf in worker_params.critical_nodes.split(","):
             # The conf is "pod_index:relaunch_times"
@@ -149,31 +147,33 @@
             max_relaunch_num: The maximum relaunch number of PS.
             command: The command of worker pods.
         """
         self._nodes = nodes
         self._new_node_name_fn = new_node_name_fn
         self._lock = threading.Lock()
         self._node_id_iter = itertools.count(len(self._nodes))
+        self._rank_id_iter = itertools.count(len(self._nodes))
 
     def update_nodes(self, nodes):
         self._nodes = nodes
         self._node_id_iter = itertools.count(len(self._nodes))
+        self._rank_id_iter = itertools.count(len(self._nodes))
 
     def remove_node(self, node_id):
         plan = ScalePlan()
         if node_id not in self._nodes:
             logger.info("Delete non-existed worker %s", node_id)
             return plan
         worker = self._nodes[node_id]
         with self._lock:
             if worker.status in [NodeStatus.DELETED, NodeStatus.INITIAL]:
                 logger.error("Unknown deletable worker id: %s" % node_id)
                 return
         worker.is_released = True
-        plan.remove_nodes.append(worker.name)
+        plan.remove_nodes.append(worker)
         return plan
 
     def relaunch_node(self, node: Node):
         plan = ScalePlan()
         with self._lock:
             node.is_released = True
             new_id = next(self._node_id_iter)
@@ -184,17 +184,17 @@
             Node(
                 node.type,
                 new_id,
                 copy.deepcopy(relaunch_node.config_resource),
                 rank_index=node.rank_index,
                 name=self._new_node_name_fn(node.type, new_id),
                 service_addr=node.service_addr,
+                relaunch_count=relaunch_node.relaunch_count,
             )
         )
-        plan.remove_nodes.append(node.name)
         return plan
 
     def cut_pending_node_cpu(self):
         """Cut down CPU cores of pendding PS Pods"""
         plan = ScalePlan()
         nodes = copy.deepcopy(self._nodes)
         for node in nodes.values():
@@ -212,27 +212,56 @@
         with self._lock:
             for node in self._nodes.values():
                 if node.status == NodeStatus.RUNNING:
                     nodes.append(node)
         return nodes
 
     def all_nodes_exited(self):
+        if len(self._nodes) == 0:
+            return True
         counter = self._get_node_counter()
 
         # At start, there may be no launched worker.
         if len(counter) == 1 and NodeStatus.INITIAL in counter:
             return False
 
-        all_exited = True
         with self._lock:
-            for node in self._nodes.values():
-                if not node.is_released and (node.status in ALIVE_STATUS):
-                    all_exited = False
-                    break
-        return all_exited
+            high_worker_num = 0
+            running_workers = []
+            pending_high_workers = []
+            pending_low_workers = []
+            for worker_id, worker in self._nodes.items():
+                if worker.is_released:
+                    continue
+                if worker.config_resource.priority == PriorityClass.LOW:
+                    if worker.status == NodeStatus.RUNNING:
+                        running_workers.append(worker_id)
+                    elif worker.status in [
+                        NodeStatus.INITIAL,
+                        NodeStatus.PENDING,
+                    ]:
+                        pending_low_workers.append(worker_id)
+                else:
+                    high_worker_num += 1
+                    if worker.status == NodeStatus.RUNNING:
+                        running_workers.append(worker_id)
+                    elif worker.status in [
+                        NodeStatus.INITIAL,
+                        NodeStatus.PENDING,
+                    ]:
+                        pending_high_workers.append(worker_id)
+
+            if (
+                running_workers
+                or pending_high_workers
+                or (not high_worker_num and pending_low_workers)
+            ):
+                return False
+            else:
+                return True
 
     def all_nodes_deleted(self):
         counter = self._get_node_counter()
         all_deleted = all([status == NodeStatus.DELETED for status in counter])
         return all_deleted
 
     def all_nodes_failed(self):
@@ -245,14 +274,31 @@
                 status
                 in [NodeStatus.FAILED, NodeStatus.DELETED, NodeStatus.INITIAL]
                 for status in counter
             ]
         )
         return all_failed
 
+    def running_nodes_hanged(self) -> List[bool]:
+        cur_time = time.time()
+        node_hang = []
+        for _, node in self._nodes.items():
+            if node.status == NodeStatus.RUNNING:
+                hang = (
+                    node.start_hang_time > 0
+                    and cur_time - node.start_hang_time
+                    > NodeResourceLimit.MAX_HANG_TIMEOUT_SECS
+                )
+                if hang:
+                    time_array = time.localtime(node.start_hang_time)
+                    date_time = time.strftime("%Y-%m-%d %H:%M:%S", time_array)
+                    logger.warning("Node %s hangs at %s", node.name, date_time)
+                node_hang.append(hang)
+        return node_hang
+
     def _get_node_counter(self):
         with self._lock:
             return Counter([node.status for node in self._nodes.values()])
 
     def update_critical_node(self, critical_node_restarts):
         """Update critical node by a dict.
         Args:
```

## dlrover/python/master/node/worker.py

```diff
@@ -8,18 +8,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
-import itertools
 from typing import Dict, List
 
-from dlrover.python.common.constants import NodeStatus, NodeType
+from dlrover.python.common.constants import (
+    NodeExitReason,
+    NodeStatus,
+    NodeType,
+)
 from dlrover.python.common.log import default_logger as logger
 from dlrover.python.common.node import Node, NodeGroupResource, NodeResource
 from dlrover.python.master.node.training_node import (
     ALIVE_STATUS,
     TrainingNodeManager,
 )
 from dlrover.python.master.resource.job import JobResource
@@ -100,15 +103,14 @@
     def __init__(
         self,
         worker_nodes: Dict[int, Node],
         job_resource: JobResource,
         max_relaunch_num,
         new_service_fn,
         new_node_name_fn,
-        use_ddp=False,
     ):
         """
         Args:
             worker_nodes: A dictionary where the key is the index of worker
                 and the value is a Node instance.
             job_resource: the resource configuration of a job.
             max_relaunch_num: The maximum relaunch number of worker.
@@ -118,66 +120,78 @@
                 worker.
             use_ddp: bool, whether workers use DDP to train a model.
         """
         super(WorkerManager, self).__init__(worker_nodes, new_node_name_fn)
         self._job_resource = job_resource
         self._max_relaunch_num = max_relaunch_num
         self._new_service_fn = new_service_fn
-        self._use_ddp = use_ddp
-        worker = job_resource.get_node_group_resource(NodeType.WORKER)
-        self._task_id_iter = itertools.count(worker.count)
 
     def adjust_worker(self, worker_resource: NodeGroupResource):
+        plan = ScalePlan()
         num = worker_resource.count
         logger.info(
             "Adjust worker resource to {}, {}, {}".format(
                 num,
                 worker_resource.node_resource.cpu,
                 worker_resource.node_resource.memory,
             )
         )
         alive_workers = []
+        completed_worker_num = 0
         for worker in self._nodes.values():
             if worker.status in ALIVE_STATUS:
                 alive_workers.append(worker)
+            elif worker.status in [NodeStatus.SUCCEEDED, NodeStatus.FINISHED]:
+                completed_worker_num += 1
         alive_num = len(alive_workers)
         with self._lock:
-            if num > alive_num:
-                self._scale_up_workers(num - alive_num)
+            if num > alive_num + completed_worker_num:
+                plan = self._scale_up_workers(
+                    num - alive_num - completed_worker_num
+                )
             elif num < alive_num:
-                self._scale_down_workers(alive_num - num, alive_workers)
+                plan = self._scale_down_workers(alive_num - num, alive_workers)
+        return plan
 
     def _scale_up_workers(self, up_num):
         """Launch up_num workers."""
+        plan = ScalePlan()
         for _ in range(up_num):
             worker_id = next(self._node_id_iter)
-            task_id = next(self._task_id_iter)
+            task_id = next(self._rank_id_iter)
             worker_resource = self._job_resource.get_node_group_resource(
                 NodeType.WORKER
             ).node_resource
             service_addr = self._new_service_fn(NodeType.WORKER, task_id)
-            self._nodes[worker_id] = Node(
+            new_node = Node(
                 NodeType.WORKER,
                 node_id=worker_id,
                 rank_index=task_id,
                 name=self._new_node_name_fn(NodeType.WORKER, worker_id),
                 max_relaunch_count=self._max_relaunch_num,
                 config_resource=copy.deepcopy(worker_resource),
                 service_addr=service_addr,
             )
+            self._nodes[worker_id] = new_node
+            logger.info("Create worker %s", self._nodes[worker_id])
+            plan.launch_nodes.append(new_node)
+        return plan
 
     def _scale_down_workers(self, down_num, running_workers: List[Node]):
         """Remove down_num running workers"""
+        plan = ScalePlan()
         for worker in reversed(running_workers):
             if down_num <= 0:
                 break
             if not worker.critical:
                 worker.relaunchable = False
                 worker.is_released = True
                 down_num -= 1
+                plan.remove_nodes.append(worker)
+        return plan
 
     def delete_exited_workers(self):
         """Delete failed, succeed, finished workers."""
         plan = ScalePlan()
         with self._lock:
             for worker in self._nodes.values():
                 if (
@@ -186,15 +200,15 @@
                         NodeStatus.FAILED,
                         NodeStatus.SUCCEEDED,
                         NodeStatus.FINISHED,
                     ]
                     and not worker.is_released
                 ):
                     worker.is_released = True
-                    plan.remove_nodes.append(worker.name)
+                    plan.remove_nodes.append(worker)
         return plan
 
     def delete_running_workers(self):
         plan = ScalePlan()
         for worker in self._nodes.values():
             if not worker.critical and worker.status in [
                 NodeStatus.RUNNING,
@@ -203,34 +217,67 @@
             ]:
                 worker.relaunchable = False
                 logger.info(
                     "Remove the worker %s after the worker-0 completed",
                     worker.name,
                 )
                 worker.is_released = True
-                plan.remove_nodes.append(worker.name)
+                plan.remove_nodes.append(worker)
         return plan
 
     def remove_noncritical_worker(self, worker_id):
         if self._nodes[worker_id].critical:
             logger.info("Skip the critical worker %s", worker_id)
         else:
             return self.remove_node(worker_id)
 
     def migrate_workers(self, workers: Dict[str, NodeResource]):
         """Migrate workers with the new resource"""
         plan = ScalePlan()
         for name, resource in workers.items():
             old_node_id = int(name.split("-")[-1])
+            old_node = self._nodes[old_node_id]
             node_id = next(self._node_id_iter)
-            task_id = self._nodes[old_node_id].rank_index
-            self._nodes[node_id] = Node(
+            task_id = old_node.rank_index
+            new_node = Node(
                 NodeType.WORKER,
                 node_id,
                 config_resource=resource,
                 status=NodeStatus.INITIAL,
                 rank_index=task_id,
                 name=self._new_node_name_fn(NodeType.WORKER, node_id),
             )
-            plan.launch_nodes.append(self._nodes[node_id])
-            plan.remove_nodes.append(name)
+            self._nodes[node_id] = new_node
+            plan.launch_nodes.append(new_node)
+            plan.remove_nodes.append(old_node)
         return plan
+
+    def remove_not_joined_rdzv_workers(self, worker_ranks: List[int]):
+        """Remove workers which do not participate in the training.
+        Args:
+            worker_ranks: The rank of worker which does not join rendezvous.
+        """
+        plan = ScalePlan()
+        for node_id, node in self._nodes.items():
+            if node.rank_index in worker_ranks:
+                p = self.remove_node(node.id)
+                self._nodes[node_id].relaunchable = False
+                if p:
+                    plan.merge(p)
+        return plan
+
+    def has_failed_worker(self):
+        """Check whether there is failed worker except evicted workers."""
+        for worker in self._nodes.values():
+            if worker.exit_reason == NodeExitReason.FATAL_ERROR:
+                return True
+        return False
+
+    def wait_worker_restart(self):
+        """Check whether there are workers tha have remaining retries."""
+        for worker in self._nodes.values():
+            if (
+                worker.exit_reason == NodeExitReason.KILLED
+                and worker.relaunch_count < worker.max_relaunch_count
+            ):
+                return True
+        return False
```

## dlrover/python/master/resource/brain_optimizer.py

```diff
@@ -9,32 +9,34 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import math
 
-from dlrover.python.brain.client import GlobalEasydlClient
+import grpc
+
+from dlrover.python.brain.client import GlobalBrainClient
+from dlrover.python.common.constants import MemoryUnit
 from dlrover.python.common.log import default_logger as logger
 from dlrover.python.common.node import NodeGroupResource, NodeResource
 from dlrover.python.master.resource.optimizer import (
     ResourceOptimizer,
     ResourcePlan,
 )
 
 _BASE_CONFIG_RETRIEVER = "base_config_retriever"
-_MEMORY_MB = 1024 * 1024
 
 
 def catch_brain_optimization_exception(func):
     def wrapper(self, *args, **kwargs):
         try:
             return func(self, *args, **kwargs)
-        except Exception as e:
-            logger.debug("Fail to execute %s by %s", func.__name__, e)
+        except grpc.RpcError as e:
+            logger.warning("Fail to execute %s by %s", func.__name__, e)
             return ResourcePlan()
 
     return wrapper
 
 
 def convert_plan_msg(plan_msg):
     """Convert a GRPC plan message to a ResourcePlan.
@@ -42,35 +44,33 @@
         plan_msg: brain_pb2.JobOptimizePlan instance.
     """
     plan = ResourcePlan()
     if not plan_msg:
         return plan
     for type, group in plan_msg.resource.task_group_resources.items():
         count = group.count
-        memory = int(group.resource.memory / _MEMORY_MB)  # MiB
+        memory = int(group.resource.memory / MemoryUnit.MB)  # MiB
         cpu = math.ceil(group.resource.cpu)
         plan.node_group_resources[type] = NodeGroupResource(
             count, NodeResource(cpu, memory)
         )
 
     for name, resource in plan_msg.resource.pod_resources.items():
         cpu = int(resource.cpu)
-        memory = int(resource.memory / _MEMORY_MB)
+        memory = int(resource.memory / MemoryUnit.MB)
         plan.node_resources[name] = NodeResource(cpu, memory)
     return plan
 
 
 class BrainResoureOptimizer(ResourceOptimizer):
     """Query resource plan from the brain service."""
 
-    name = "brain"
-
     def __init__(self, job_uuid, resource_limits):
         super(BrainResoureOptimizer, self).__init__(job_uuid, resource_limits)
-        self._brain_client = GlobalEasydlClient.EASYDL_CLIENT
+        self._brain_client = GlobalBrainClient.BRAIN_CLIENT
 
     @catch_brain_optimization_exception
     def generate_opt_plan(self, stage, config={}) -> ResourcePlan:
         res = self._brain_client.get_optimization_plan(
             self._job_uuid,
             stage,
             _BASE_CONFIG_RETRIEVER,
@@ -87,17 +87,17 @@
             config,
             plan_msg,
         )
         plan = convert_plan_msg(plan_msg)
         return plan
 
     @catch_brain_optimization_exception
-    def generate_oom_recovery_plan(self, oom_pods, stage, config={}):
+    def generate_oom_recovery_plan(self, oom_nodes, stage, config={}):
         res = self._brain_client.get_oom_resource_plan(
-            oom_pods,
+            oom_nodes,
             self._job_uuid,
             stage,
             _BASE_CONFIG_RETRIEVER,
             config,
         )
         if not res.job_optimize_plans:
             logger.info("No any optimization plan for PS")
```

## dlrover/python/master/resource/job.py

```diff
@@ -9,48 +9,67 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
 import threading
+import time
+from abc import ABCMeta, abstractmethod
 from typing import Dict
 
+from dlrover.python.brain.client import GlobalBrainClient
 from dlrover.python.common.constants import (
     JobOptStage,
     NodeResourceLimit,
     NodeType,
+    OptimizeMode,
     OptimizeWorkerPhase,
 )
 from dlrover.python.common.global_context import Context
 from dlrover.python.common.log import default_logger as logger
 from dlrover.python.common.node import Node, NodeGroupResource, NodeResource
 from dlrover.python.common.serialize import JsonSerializable
 from dlrover.python.master.resource.brain_optimizer import (
     BrainResoureOptimizer,
 )
-from dlrover.python.master.resource.local_optimizer import LocalOptimizer
-from dlrover.python.master.resource.optimizer import ResourcePlan
+from dlrover.python.master.resource.local_optimizer import PSLocalOptimizer
+from dlrover.python.master.resource.optimizer import (
+    ResourcePlan,
+    SimpleOptimizer,
+)
 from dlrover.python.scheduler.job import ResourceLimits
 
 _WORKER_OPTIMIZE_PHASE = "optimizer.worker.optimize-phase"
 
 _dlrover_context = Context.singleton_instance()
 
 
-def new_resource_optimizer(
-    optimizer: str, job_uuid, resoure_limits: ResourceLimits
+def new_ps_resource_optimizer(
+    optimize_mode: str, job_uuid, resoure_limits: ResourceLimits
 ):
-    logger.info("New  %s resource optimizer for job %s", optimizer, job_uuid)
-    if optimizer == BrainResoureOptimizer.name:
-        return BrainResoureOptimizer(job_uuid, resoure_limits)
-    elif optimizer == LocalOptimizer.name:
-        return LocalOptimizer(job_uuid, resoure_limits)
+    logger.info(
+        "New  %s resource optimizer for job %s", optimize_mode, job_uuid
+    )
+    if optimize_mode == OptimizeMode.CLUSTER:
+        if GlobalBrainClient.BRAIN_CLIENT.available():
+            return BrainResoureOptimizer(job_uuid, resoure_limits)
+        else:
+            logger.warning(
+                "Brain service is not available, use a local optimizer"
+            )
+            return PSLocalOptimizer(job_uuid, resoure_limits)
+    elif optimize_mode == OptimizeMode.SINGLE_JOB:
+        return PSLocalOptimizer(job_uuid, resoure_limits)
     else:
-        logger.error("Not support %s optimizer", optimizer)
+        logger.warning(
+            "Not support optiimzem mode %s, use a simple optimizer",
+            optimize_mode,
+        )
+        return SimpleOptimizer(job_uuid, resoure_limits)
 
 
 class JobResource(JsonSerializable):
     def __init__(self):
         self.node_group_resources: Dict[str, NodeGroupResource] = {}
 
     def get_node_group_resource(self, node_type):
@@ -96,36 +115,39 @@
     def init_job_node_meta(
         self,
         relaunch_on_worker_failure,
         service_create_fn,
         new_node_name_fn,
     ):
         """
-        job_resource: resource configuration of a job.
         relaunch_on_worker_failure: int, the number of relaunches.
-        service_create_fn: a callable function to get the service address
-            of a node.
+        service_create_fn: a callable function to create the name for a sevice.
+        new_node_name_fn: a callable function to create the name for a node.
         return: a dict with pod_type as key, and another dict as value.
                 The other dict uses pod id as key, and PodInfo as value.
         """
         job_nodes: Dict[str, Dict[int, Node]] = {}
         for node_type in self.get_node_types():
             group_resource = self.get_node_group_resource(node_type)
             config_resource = group_resource.node_resource
             group_nodes: Dict[int, Node] = {}
             for i in range(group_resource.count):
                 group_nodes[i] = Node(
                     node_type=node_type,
                     node_id=i,
+                    rank_index=i,
                     name=new_node_name_fn(node_type, i),
                     config_resource=copy.deepcopy(config_resource),
                     max_relaunch_count=relaunch_on_worker_failure,
                     service_addr=service_create_fn(node_type, i),
                 )
             job_nodes[node_type] = group_nodes
+        logger.info(
+            "after initiating job node meta job_nodes are %s" % job_nodes
+        )
         return job_nodes
 
     def adjust_worker_for_estimator(self):
         if (
             NodeType.CHIEF in self.node_group_resources
             and self.node_group_resources[NodeType.CHIEF].count > 0
         ) or (NodeType.WORKER not in self.node_group_resources):
@@ -142,36 +164,70 @@
         chief.node_resource.cpu = worker.node_resource.cpu
         chief.node_resource.memory = worker.node_resource.memory
         self.node_group_resources[NodeType.CHIEF] = chief
         worker.count -= 1
         logger.info("self = %s", self.toJSON())
 
 
-class JobResourceOptimizer(object):
-    """It generates resource configuration for a job."""
+class JobResourceOptimizer(metaclass=ABCMeta):
+    @abstractmethod
+    def update_job_uuid(self, job_uuid):
+        pass
+
+    @abstractmethod
+    def init_job_resource(self, job_resource: JobResource):
+        """Initialize resource configuration for a job."""
+        pass
+
+    @abstractmethod
+    def get_job_resource_plan(self) -> ResourcePlan:
+        """Get resource plan for a job."""
+        pass
+
+    @abstractmethod
+    def adjust_oom_resource(self, node: Node):
+        """Adjust the resource configuration for OOM nodes"""
+        pass
+
+    @abstractmethod
+    def get_config_resource(self) -> JobResource:
+        pass
+
+
+class PSJobResourceOptimizer(JobResourceOptimizer):
+    """It generates resource configuration for a PS job."""
 
     def __init__(
         self,
         worker_resource: NodeGroupResource,
         ps_resource: NodeGroupResource,
-        optimizer: str,
+        optimize_mode: str,
         job_uuid="",
         resource_limits=ResourceLimits(),
     ):
         self._worker_resource = worker_resource
         self._ps_resource = ps_resource
         self._original_worker_resource = copy.deepcopy(self._worker_resource)
         self._original_ps_resource = copy.deepcopy(self._ps_resource)
-        self._resource_optimizer = new_resource_optimizer(
-            optimizer, job_uuid, resource_limits
+        self._resource_optimizer = new_ps_resource_optimizer(
+            optimize_mode, job_uuid, resource_limits
         )
         self._lock = threading.Lock()
         self.optimized_ps_mem = False
         self.optimize_worker_sampled = False
         self._job_stage = JobOptStage.CREATE
+        self._last_ps_change_time = 0.0
+
+    def get_config_resource(self):
+        job_config = JobResource()
+        worker_config = self._original_worker_resource
+        job_config.node_group_resources[NodeType.WORKER] = worker_config
+        ps_config = self._original_worker_resource
+        job_config.node_group_resources[NodeType.PS] = ps_config
+        return job_config
 
     def update_job_uuid(self, job_uuid):
         self._resource_optimizer.update_job_uuid(job_uuid)
 
     def _init_job_resource_by_optimizer(self):
         plan = self._resource_optimizer.generate_opt_plan(self._job_stage)
         if not plan or plan.empty():
@@ -200,35 +256,14 @@
             )
             self._ps_resource.update(
                 ps_resource.count,
                 ps_resource.node_resource.cpu,
                 ps_resource.node_resource.memory,
             )
 
-    def optimize_worker_resource(self):
-        plan = self._get_worker_resource_at_init_phase()
-        if NodeType.WORKER in plan.node_group_resources:
-            worker_resource = self._check_ignore_original_worker_resource(
-                plan.node_group_resources[NodeType.WORKER]
-            )
-            self._worker_resource.update(
-                worker_resource.count,
-                worker_resource.node_resource.cpu,
-                worker_resource.node_resource.memory,
-            )
-        else:
-            logger.info("Use the default original worker resource.")
-            plan.node_group_resources[NodeType.WORKER] = copy.deepcopy(
-                self._worker_resource
-            )
-        return plan
-
-    def get_worker_resource(self):
-        return self._worker_resource
-
     def init_job_resource(self, job_resource: JobResource):
         """Adjust the initial resource of typed pods by EasyDL.
         Args:
             job_resource: node resource configuration of a job.
         """
         self._init_job_resource_by_optimizer()
         job_resource.update_node_group_resource(
@@ -255,55 +290,70 @@
             min_memory = NodeResourceLimit.MIN_VALID_MEMORY
             if resource.memory < min_memory:
                 resource.memory = self._worker_resource.node_resource.memory
 
         logger.info("Job resource = %s", job_resource.toJSON())
         return job_resource
 
-    def adjust_oom_worker_resource(self, node: Node):
+    def adjust_oom_resource(self, node):
+        if node.type == NodeType.PS:
+            self._adjust_oom_ps_resource(node)
+        else:
+            self._adjust_oom_worker_resource(node)
+
+    def _adjust_oom_worker_resource(self, node: Node):
         """Increment the memory to launch worker. The new memory
         is max(1.5 * memory, the memory set by users).
 
         Args:
             node: Node object.
         """
         cur_mem = node.config_resource.memory
         if (
             _dlrover_context.auto_worker_enabled
             and self._job_stage == JobOptStage.WORKER_INITIAL
         ):
             plan = self._resource_optimizer.generate_oom_recovery_plan(
-                [node.name], JobOptStage.CREATE
+                [node], JobOptStage.CREATE
             )
             if plan and not plan.empty():
                 new_resource = plan.node_group_resources[NodeType.WORKER]
                 self._worker_resource.node_resource.memory = max(
                     self._worker_resource.node_resource.memory,
                     new_resource.node_resource.memory,
                 )
         else:
-            self.optimize_worker_resource()
+            plan = self._get_worker_resource_at_init_phase()
+            if NodeType.WORKER in plan.node_group_resources:
+                new_resource = self._check_ignore_original_worker_resource(
+                    plan.node_group_resources[NodeType.WORKER]
+                )
+                self._worker_resource.node_resource.memory = max(
+                    self._worker_resource.node_resource.memory,
+                    new_resource.node_resource.memory,
+                )
         cur_mem *= NodeResourceLimit.INCREMENTAL_MEMORY_FACTOR
+        cur_mem = min(cur_mem, NodeResourceLimit.MAX_MEMORY)
         node.config_resource.memory = int(
             max(
                 self._worker_resource.node_resource.memory,
                 cur_mem,
                 self._original_worker_resource.node_resource.memory,
             )
         )
         logger.info(
             "Increment the memory of %s to %s",
             node.name,
             node.config_resource.memory,
         )
 
-    def adjust_oom_ps_resource(self, node: Node):
+    def _adjust_oom_ps_resource(self, node: Node):
         """Adjust PS resource if there is a OOM PS"""
         plan = self._resource_optimizer.generate_oom_recovery_plan(
-            [node.name], JobOptStage.PS_INITIAL
+            [node], JobOptStage.PS_INITIAL
         )
         if plan and not plan.empty():
             ps = plan.node_group_resources[NodeType.PS]
             self._ps_resource.node_resource.memory = max(
                 self._ps_resource.node_resource.memory,
                 ps.node_resource.memory,
             )
@@ -317,14 +367,15 @@
             )
         )
         logger.info(
             "Increment the memory of %s to %s",
             node.name,
             node.config_resource.memory,
         )
+        self._last_ps_change_time = time.time()
 
     def get_job_resource_plan(self):
         plan = None
         if self._job_stage == JobOptStage.WORKER_INITIAL:
             plan = self._get_worker_resource_at_init_phase()
             self._job_stage = JobOptStage.PS_INITIAL
         elif self._job_stage == JobOptStage.PS_INITIAL:
@@ -350,49 +401,56 @@
         if not self.optimize_worker_sampled:
             plan = self._get_worker_resource_at_sample_phase()
             self.optimize_worker_sampled = True
         else:
             plan = self._get_worker_resource_at_stable_phase()
         return plan
 
-    def _get_worker_resource_at_init_phase(self):
-        optimizer_config = {}
+    def _get_worker_resource_at_init_phase(self, optimizer_config={}):
         optimizer_config[_WORKER_OPTIMIZE_PHASE] = OptimizeWorkerPhase.INITIAL
         plan = self._resource_optimizer.generate_opt_plan(
             JobOptStage.WORKER_INITIAL, optimizer_config
         )
         if plan.empty():
             logger.info("No any plan to initialize the number of worker")
         return plan
 
-    def _get_worker_resource_at_sample_phase(self):
-        optimizer_config = {}
+    def _get_worker_resource_at_sample_phase(self, optimizer_config={}):
         optimizer_config[_WORKER_OPTIMIZE_PHASE] = OptimizeWorkerPhase.SAMPLE
         plan = self._resource_optimizer.generate_opt_plan(
             JobOptStage.WORKER_INITIAL, optimizer_config
         )
         if not plan or plan.empty():
             return
         return plan
 
-    def _get_worker_resource_at_stable_phase(self):
-        optimizer_config = {}
+    def _get_worker_resource_at_stable_phase(self, optimizer_config={}):
         optimizer_config[_WORKER_OPTIMIZE_PHASE] = OptimizeWorkerPhase.STABLE
         plan = self._resource_optimizer.generate_opt_plan(
             JobOptStage.WORKER_INITIAL, optimizer_config
         )
         if not plan:
             return
         return plan
 
-    def _get_ps_resource_plan(self):
-        optimizer_config = {}
-        plan = self._resource_optimizer.generate_opt_plan(
-            self._job_stage, optimizer_config
-        )
+    def _get_ps_resource_plan(self, optimizer_config={}):
+        # The interval of changing PS should be long enough.
+        interval = _dlrover_context.seconds_interval_to_change_ps
+        if time.time() - self._last_ps_change_time > interval:
+            plan = self._resource_optimizer.generate_opt_plan(
+                self._job_stage, optimizer_config
+            )
+        else:
+            logger.info(
+                "Skip optimizing PS, because the interval"
+                "to change ps is too short."
+            )
+            return ResourcePlan()
+        if not plan.empty():
+            self._last_ps_change_time = time.time()
         return plan
 
     def _verify_optimized_group_resource(self, plan: ResourcePlan, node_type):
         group = plan.node_group_resources[node_type]
         if node_type == NodeType.WORKER:
             group = self._check_ignore_original_worker_resource(group)
             node_resource = group.node_resource
@@ -430,7 +488,62 @@
         if self._original_ps_resource.count > 0:
             resource.count = self._original_ps_resource.count
         if original_resource.memory >= NodeResourceLimit.MIN_VALID_MEMORY:
             resource.node_resource.memory = original_resource.memory
         if original_resource.cpu >= NodeResourceLimit.MIN_VALID_CPU:
             resource.node_resource.cpu = original_resource.cpu
         return resource
+
+
+class AllreduceJobResourceOptimizer(JobResourceOptimizer):
+    """It generates resource configuration for a job."""
+
+    def __init__(
+        self,
+        worker_resource: NodeGroupResource,
+        job_uuid="",
+    ):
+        self._worker_resource = worker_resource
+        self._original_worker_resource = copy.deepcopy(self._worker_resource)
+        self._job_uuid = job_uuid
+        self._lock = threading.Lock()
+        self._node_unit = 1
+        self._alive_node_num = 0
+
+    def update_job_uuid(self, job_uuid):
+        pass
+
+    def init_job_resource(self, job_resource: JobResource):
+        pass
+
+    def get_job_resource_plan(self) -> ResourcePlan:
+        """Check wether there are free nodes in the cluster."""
+        plan = ResourcePlan()
+        worker_config = copy.deepcopy(self._original_worker_resource)
+        max_node_num = self._original_worker_resource.count
+        request_num = max_node_num - self._alive_node_num
+        free_num = self._get_free_gpu_node()
+        free_num = (free_num // self._node_unit) * self._node_unit
+        new_num = min(free_num, request_num)
+        worker_config.count = self._alive_node_num + new_num
+        plan.node_group_resources[NodeType.WORKER] = worker_config
+        return plan
+
+    # TODO: implement the function to query the number free GPU nodes.
+    def _get_free_gpu_node(self):
+        return 0
+
+    def adjust_oom_resource(self, node: Node):
+        """Adjust the resource configuration for OOM nodes"""
+        node.config_resource.memory *= 2
+
+    def get_config_resource(self):
+        job_config = JobResource()
+        worker_config = self._original_worker_resource
+        job_config.node_group_resources[NodeType.WORKER] = worker_config
+        return job_config
+
+    def set_node_unit(self, node_unit):
+        self._node_unit = node_unit
+
+    def set_alive_node_num(self, node_num):
+        self._alive_node_num = node_num
```

## dlrover/python/master/resource/local_optimizer.py

```diff
@@ -10,54 +10,67 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import math
 from typing import Dict, List
 
-from dlrover.python.common.constants import JobOptStage, NodeType
+from dlrover.python.common.constants import JobOptStage, MemoryUnit, NodeType
 from dlrover.python.common.log import default_logger as logger
 from dlrover.python.common.node import Node, NodeGroupResource, NodeResource
 from dlrover.python.common.serialize import JsonSerializable
 from dlrover.python.master.resource.optimizer import (
     ResourceOptimizer,
     ResourcePlan,
 )
 from dlrover.python.master.stats.reporter import JobMeta, LocalStatsReporter
 from dlrover.python.master.stats.training_metrics import RuntimeMetric
 from dlrover.python.scheduler.job import ResourceLimits
 
 _LATEST_SAMPLE_COUNT = 5
-_INITIAL_NODE_CPU = 16
-_INITIAL_NODE_MEMORY = 16 * 1024  # 16Gi
-_MINIKUBE_INITIAL_NODE_CPU = 1
-_MINIKUBE_INITIAL_NODE_MEMORY = 512  # 512Mi
+_MAX_INITIAL_NODE_CPU = 16
+_MAX_INITIAL_NODE_MEMORY = 8 * 1024  # 8Gi
 _MIN_NODE_CPU = 1
 _MIN_NODE_MEMORY = 1024
+_MIN_NODE_NUM = 5
+
+
+def convert_memory_to_mb(plan: ResourcePlan):
+    for _, group in plan.node_group_resources.items():
+        group.node_resource.memory = int(
+            group.node_resource.memory / MemoryUnit.MB
+        )
+    for _, node in plan.node_resources.items():
+        node.memory = int(node.memory / MemoryUnit.MB)
+    return plan
 
 
 class OptimizerParams(object):
     def __init__(self):
         self.ps_cpu_overload_threshold = 0.9
         self.ps_cpu_hot_threshold = 0.9
         self.ps_memory_margin_percent = 0.2
         self.worker_memory_margin_percent = 0.5
         self.oom_memory_up_factor = 2
         self.node_max_cpu = 32
+        self.min_worker_speed_ratio = 0.2
+        self.max_ps_cpu_util = 0.95
 
 
 class ProcessResourceRequirement(JsonSerializable):
     def __init__(self, worker_cpu, ps_cpu, worker_memory) -> None:
         self.worker_cpu = worker_cpu
         self.ps_cpu = ps_cpu
         self.worker_memory = worker_memory
 
 
-class LocalOptimizer(ResourceOptimizer):
-    name = "local"
+class PSLocalOptimizer(ResourceOptimizer):
+    """PS Local optimizer stores runtime statistics locally and optimize
+    the resource of a training job without cluster information.
+    """
 
     def __init__(self, job_uuid, resource_limits: ResourceLimits):
         self._job_uuid = job_uuid
         self._stats_collector = LocalStatsReporter(JobMeta(job_uuid))
         self._opt_params = OptimizerParams()
         self._resource_limits = resource_limits
 
@@ -67,58 +80,57 @@
             plan = self._generate_job_create_resource()
         if stage == JobOptStage.WORKER_INITIAL:
             plan = self._generate_worker_resoruce()
         if stage == JobOptStage.PS_INITIAL:
             plan = self._generate_ps_initial_resource()
         if stage == JobOptStage.RUNNING:
             plan = self._generate_job_running_resource()
+        plan = convert_memory_to_mb(plan)
         if plan.empty():
-            logger.info("Not support job stage %s", stage)
+            logger.info("No any resource plan for %s", stage)
         else:
             logger.info("plan of stage %s is %s", stage, plan.toJSON(indent=4))
         return plan
 
     def generate_oom_recovery_plan(
         self, oom_nodes: List[Node], stage, config={}
     ):
         plan = ResourcePlan()
         for node in oom_nodes:
             factor = self._opt_params.oom_memory_up_factor
             opt_memory = factor * node.config_resource.memory
-            plan.node_resources[node.name] = NodeResource(0, opt_memory)
+            plan.node_resources[node.name] = NodeResource(
+                node.config_resource.cpu, opt_memory
+            )
         return plan
 
     def generate_resource_plan_with_optimizer(self, config={}) -> ResourcePlan:
         """Generate a resource plan by an optimizer"""
         pass
 
     def _generate_job_create_resource(self):
         plan = ResourcePlan()
-        node_cpu = _INITIAL_NODE_CPU
-        node_memory = _INITIAL_NODE_MEMORY
-        if (
-            self._resource_limits.cpu < 16
-            and self._resource_limits.memory < 32 * 1024
-        ):
-            # Set a little resource to test an elastic job on minikube.
-            node_cpu = _MINIKUBE_INITIAL_NODE_CPU
-            node_memory = _MINIKUBE_INITIAL_NODE_MEMORY
+        node_cpu = math.ceil(self._resource_limits.cpu / _MIN_NODE_NUM)
+        node_cpu = min(node_cpu, _MAX_INITIAL_NODE_CPU)
+        node_memory = math.ceil(self._resource_limits.memory / _MIN_NODE_NUM)
+        node_memory = min(node_memory, _MAX_INITIAL_NODE_MEMORY)
 
         ps = NodeGroupResource(1, NodeResource(node_cpu, node_memory))
         worker = NodeGroupResource(1, NodeResource(node_cpu, node_memory))
         plan.node_group_resources[NodeType.WORKER] = worker
         plan.node_group_resources[NodeType.PS] = ps
         return plan
 
     def _generate_ps_initial_resource(self):
         node_samples = self._extract_node_resource()
         max_ps_memory = 0
         ps_cpu_requested = 0
         plan = ResourcePlan()
         if len(node_samples[NodeType.PS]) == 0:
+            logger.info("No any workload metrics for PS.")
             return plan
         for node in node_samples[NodeType.PS][0]:
             max_ps_memory = max(max_ps_memory, node.used_resource.memory)
             ps_cpu_requested = max(node.config_resource.cpu, ps_cpu_requested)
 
         resource = self._estimate_process_require_resource()
 
@@ -176,14 +188,23 @@
         plan = ResourcePlan()
         node_samples = self._extract_node_resource()
         max_ps_cpu_util = 0.0
         for nodes in node_samples[NodeType.PS]:
             for node in nodes:
                 cpu_util = node.used_resource.cpu / node.config_resource.cpu
                 max_ps_cpu_util = max(cpu_util, max_ps_cpu_util)
+        logger.info("max ps cpu util = %s", max_ps_cpu_util)
+
+        if max_ps_cpu_util > self._opt_params.max_ps_cpu_util:
+            return plan
+
+        worker_speed_ratio = self._compute_worker_speed_ratio()
+        logger.info("The speed ratio of worker = %s", max_ps_cpu_util)
+        if worker_speed_ratio < self._opt_params.min_worker_speed_ratio:
+            return plan
 
         sample_count = len(node_samples[NodeType.WORKER])
         if max_ps_cpu_util == 0 or sample_count == 0:
             logger.warning("No CPU utilization of PS")
             return plan
         opt_worker_num = len(node_samples[NodeType.WORKER][0])
         factor = self._opt_params.ps_cpu_overload_threshold / max_ps_cpu_util
@@ -218,14 +239,65 @@
         )
         opt_worker_num = int(min(max_worker_num, opt_worker_num))
         plan.node_group_resources[NodeType.WORKER] = NodeGroupResource(
             opt_worker_num, NodeResource(opt_cpu, opt_memory)
         )
         return plan
 
+    def _compute_worker_speed_ratio(self):
+        stats = self._stats_collector.get_runtime_stats()
+        post_start_index = 0
+        for i in reversed(range(len(stats))):
+            if len(stats[i].running_nodes) != len(stats[-1].running_nodes):
+                break
+            post_start_index = i
+        post_worker_num, post_speed = self._compute_worker_speed(
+            stats, post_start_index, len(stats)
+        )
+        if post_start_index == 0:
+            return 1
+
+        pre_start_index = 0
+        pre_latest_stat = stats[post_start_index - 1]
+        for i in reversed(range(post_start_index)):
+            if len(stats[i].running_nodes) != len(
+                pre_latest_stat.running_nodes
+            ):
+                break
+            pre_start_index = i
+        pre_worker_num, pre_speed = self._compute_worker_speed(
+            stats, pre_start_index, post_start_index
+        )
+        if (
+            pre_worker_num == 0
+            or pre_speed == 0
+            or pre_worker_num == post_worker_num
+        ):
+            return 1
+
+        speed_diff = post_speed - pre_speed
+        worker_diff = post_worker_num - pre_worker_num
+        new_worker_avg_speed = speed_diff / worker_diff
+        old_worker_avg_speed = pre_speed / pre_worker_num
+        speed_ratio = new_worker_avg_speed / old_worker_avg_speed
+        return speed_ratio
+
+    def _compute_worker_speed(self, stats: List[RuntimeMetric], start, end):
+        if end == start:
+            return 0, 0
+        sum_speed = 0
+        for i in range(start, end):
+            sum_speed += stats[i].speed
+        avg_speed = sum_speed / (end - start)
+        worker_num = 0
+        for node in stats[start].running_nodes:
+            if node.type == NodeType.WORKER:
+                worker_num += 1
+        return worker_num, avg_speed
+
     def _optimize_hot_ps_cpu(self):
         node_samples = self._extract_node_resource()
         ps_used_cpus: Dict[int, List[float]] = {}
         ps_config_cpu: Dict[int, float] = {}
         for nodes in node_samples[NodeType.PS]:
             for node in nodes:
                 ps_used_cpus.setdefault(node.id, [])
@@ -289,29 +361,28 @@
                     cur_ps_samples.append(node)
                     cur_ps.add(node.id)
             if cur_ps == latest_ps:
                 node_used_resources[NodeType.PS].append(cur_ps_samples)
             if latest_worker_num == cur_worker_num:
                 node_used_resources[NodeType.WORKER].append(cur_worker_samples)
 
-        for ps_samples in node_used_resources[NodeType.PS]:
-            ps_resource = []
-            for ps in ps_samples:
-                ps_resource.append(
-                    (ps.used_resource.cpu, ps.used_resource.memory)
-                )
-            logger.info("PS resource samples = %s", ps_resource)
-
-        for ps_samples in node_used_resources[NodeType.WORKER]:
-            ps_resource = []
-            for ps in ps_samples:
-                ps_resource.append(
-                    (ps.used_resource.cpu, ps.used_resource.memory)
+        for node_type, resource_samples in node_used_resources.items():
+            for node_samples in resource_samples:
+                node_resource = []
+                for node in node_samples:
+                    node_resource.append(
+                        (
+                            node.id,
+                            node.used_resource.cpu,
+                            node.used_resource.memory,
+                        )
+                    )
+                logger.info(
+                    "%s resource samples = %s", node_type, node_resource
                 )
-            logger.info("worker resource samples = %s", ps_resource)
         return node_used_resources
 
     def _compute_total_requested_resource(self, type):
         stats: List[RuntimeMetric] = self._stats_collector.get_runtime_stats()
         cpu = 0
         memory = 0
         for node in stats[-1].running_nodes:
```

## dlrover/python/master/resource/optimizer.py

```diff
@@ -146,7 +146,29 @@
         """Generate a recovery plan for OOM nodes"""
         pass
 
     @abstractmethod
     def generate_resource_plan_with_optimizer(self, config={}) -> ResourcePlan:
         """Generate a resource plan by an optimizer"""
         pass
+
+
+class SimpleOptimizer(ResourceOptimizer):
+    def __init__(self, job_uuid, resource_limits: ResourceLimits):
+        self._job_uuid = job_uuid
+        self._resource_limits = resource_limits
+
+    def update_job_uuid(self, job_uuid):
+        self._job_uuid = job_uuid
+
+    def generate_opt_plan(self, stage, config={}) -> ResourcePlan:
+        """Generate a resource configuration plan"""
+        return ResourcePlan()
+
+    def generate_oom_recovery_plan(
+        self, oom_nodes, stage, config={}
+    ) -> ResourcePlan:
+        """Generate a recovery plan for OOM nodes"""
+        return ResourcePlan()
+
+    def generate_resource_plan_with_optimizer(self, config={}) -> ResourcePlan:
+        return ResourcePlan()
```

## dlrover/python/master/scaler/base_scaler.py

```diff
@@ -26,19 +26,23 @@
         remove_nodes: a scaler to remove nodes.
         ps_addrs: all add addresses of PS nodes.
     """
 
     def __init__(self):
         self.node_group_resources: Dict[str, NodeGroupResource] = {}
         self.launch_nodes: List[Node] = []
-        self.remove_nodes: List[str] = []
+        self.remove_nodes: List[Node] = []
         self.ps_addrs: List[str] = []
 
     def empty(self):
-        return len(self.node_group_resources) + len(self.node_resources) == 0
+        return (
+            not self.node_group_resources
+            and not self.launch_nodes
+            and not self.remove_nodes
+        )
 
     def merge(self, plan):
         self.node_group_resources.update(plan.node_group_resources)
         self.launch_nodes.extend(plan.launch_nodes)
         self.remove_nodes.extend(plan.remove_nodes)
```

## dlrover/python/master/scaler/elasticjob_scaler.py

```diff
@@ -7,33 +7,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import time
 from abc import ABCMeta, abstractmethod
-from typing import Dict
+from typing import Dict, List
 
+from dlrover.python.common.constants import ElasticJobApi, ScalePlanLabel
 from dlrover.python.master.scaler.base_scaler import ScalePlan, Scaler
-from dlrover.python.scheduler.kubernetes import get_pod_name, k8sClient
+from dlrover.python.scheduler.kubernetes import k8sClient
 
-SCALER_GROUP = "elastic.iml.github.io"
-SCALER_VERION = "v1alpha1"
-SCALER_KIND = "Scaler"
 
-
-class BaseScalerSpec(metaclass=ABCMeta):
+class BaseScaleSpec(metaclass=ABCMeta):
     @abstractmethod
     def to_dict(self):
         """Serialize the object to a dictionary"""
         pass
 
 
-class ScalerResourceSpec(BaseScalerSpec):
+class ContainerResourceSpec(BaseScaleSpec):
     """The resource specification of a node.
     Attributes:
         cpu: CPU cores of a node.
         memory: The memory of of a node with unit of MB.
         gpu: GPU cores of a node.
     """
 
@@ -44,66 +42,109 @@
         self.gpu_num = gpu_num
 
     def to_dict(self):
         spec = {}
         spec["cpu"] = str(self.cpu)
         spec["memory"] = "{}Mi".format(self.memory)
         if self.gpu_type:
-            spec["gpu_type"] = self.gpu_type
-            spec["gpu_num"] = str(self.gpu_num)
+            spec[self.gpu_type] = str(self.gpu_num)
         return spec
 
 
-class ScalerReplicaResourceSpec(BaseScalerSpec):
-    def __init__(self, replicas, resource_spec) -> None:
+class ReplicaResourceSpec(BaseScaleSpec):
+    def __init__(self, replicas, resource_spec: ContainerResourceSpec) -> None:
         self.replicas = replicas
         self.resource = resource_spec
 
     def to_dict(self):
         spec = {}
         spec["replicas"] = self.replicas
         spec["resource"] = self.resource.to_dict()
         return spec
 
 
-class ScalerSpec(BaseScalerSpec):
+class PodMeta(BaseScaleSpec):
+    def __init__(
+        self,
+        name,
+        id,
+        type,
+        rank_index,
+        service,
+        resource: ContainerResourceSpec,
+    ):
+        self.name = name
+        self.id = id
+        self.type = type
+        self.rank_index = rank_index
+        self.service = service
+        self.resource = resource
+
+    def to_dict(self):
+        spec = {}
+        spec["name"] = self.name
+        spec["type"] = self.type
+        spec["id"] = self.id
+        spec["rankIndex"] = self.rank_index
+        spec["service"] = self.service
+        spec["resource"] = self.resource.to_dict()
+        return spec
+
+
+class ScaleSpec(BaseScaleSpec):
     def __init__(self, owner_job: str) -> None:
         self.owner_job = owner_job
-        self.replica_resource_specs: Dict[str, ScalerReplicaResourceSpec] = {}
-        self.node_resource_specs: Dict[str, ScalerResourceSpec] = {}
+        self.replica_resource_specs: Dict[str, ReplicaResourceSpec] = {}
+        self.create_pods: List[PodMeta] = []
+        self.remove_pods: List[PodMeta] = []
+        self.ps_hosts: List[str] = []
+        self.manual_scaling = False
 
     def to_dict(self):
         spec = {}
         spec["ownerJob"] = self.owner_job
-        spec["replicaResourceSpec"] = dict()
+        spec["replicaResourceSpecs"] = dict()
         for name, resource_spec in self.replica_resource_specs.items():
-            spec["replicaResourceSpec"][name] = resource_spec.to_dict()
-        spec["nodeResourceSpec"] = dict()
-        for name, resource_spec in self.node_resource_specs.items():
-            spec["nodeResourceSpec"] = resource_spec.to_dict()
+            spec["replicaResourceSpecs"][name] = resource_spec.to_dict()
+        spec["createPods"] = []
+        for pod in self.create_pods:
+            spec["createPods"].append(pod.to_dict())
+        spec["removePods"] = []
+        for pod in self.remove_pods:
+            spec["removePods"].append(pod.to_dict())
+        spec["psHosts"] = self.ps_hosts
         return spec
 
 
-class ScalerKind(BaseScalerSpec):
+class ScalePlanCrd(BaseScaleSpec):
     """ScalerKind is a dictionary of a Scaler CRD for an ElasticJob
     to scale up/down Pods of a job on a k8s cluster.
     """
 
     def __init__(
         self,
         api_version: str,
         kind: str,
-        metadata: Dict[str, str],
-        spec: ScalerSpec,
+        metadata,
+        spec: ScaleSpec,
     ):
         self.api_version = api_version
         self.kind = kind
         self.metadata = metadata
         self.spec = spec
 
+    def set_owner_reference(self, api_version, name, uid):
+        ref_dict = {}
+        ref_dict["apiVersion"] = api_version
+        ref_dict["blockOwnerDeletion"] = True
+        ref_dict["kind"] = ElasticJobApi.ELASTICJOB_KIND
+        ref_dict["name"] = name
+        ref_dict["uid"] = uid
+        self.metadata["ownerReferences"] = [ref_dict]
+
     def to_dict(self):
         spec = {}
         spec["apiVersion"] = self.api_version
         spec["kind"] = self.kind
         spec["metadata"] = self.metadata
         spec["spec"] = self.spec.to_dict()
         return spec
@@ -111,50 +152,102 @@
 
 class ElasticJobScaler(Scaler):
     """ElasticJobScaler creates a elastic.iml.github.io/v1alpha1/Scaler
     CRD to notify ElasticJob controller to scale Pods of a job."""
 
     def __init__(self, job_name, namespace):
         super(ElasticJobScaler, self).__init__(job_name)
-        self._client = k8sClient.singleton_instance(namespace, job_name)
+        self._client = k8sClient.singleton_instance(namespace)
         self._namespace = namespace
+        self._scaleplan_name = self._job_name + "-scaleplan"
+        self._scaleplan_index = 0
+        self._job = self._retry_to_get_job()
+        self._job_uid = self._job["metadata"]["uid"]
+
+    def _retry_to_get_job(self):
+        for _ in range(3):
+            job = self._client.get_custom_resource(
+                name=self._job_name,
+                group=ElasticJobApi.GROUP,
+                version=ElasticJobApi.VERION,
+                plural=ElasticJobApi.ELASTICJOB_PLURAL,
+            )
+            if job:
+                return job
+            else:
+                time.sleep(5)
+        raise ValueError("Cannot get the training job %s", self._job_name)
 
     def scale(self, plan: ScalePlan):
-        scaler_crd = self._generate_scaler_crd_by_plan(plan)
+        scale_plan_crd = self._generate_scale_plan_crd(plan)
         self._client.create_custom_resource(
-            group=SCALER_GROUP,
-            version=SCALER_VERION,
-            plural="scalers",
-            body=scaler_crd.to_dict(),
+            group=ElasticJobApi.GROUP,
+            version=ElasticJobApi.VERION,
+            plural=ElasticJobApi.SCALEPLAN_PLURAL,
+            body=scale_plan_crd.to_dict(),
         )
+        self._scaleplan_index += 1
 
-    def _generate_scaler_crd_by_plan(self, plan: ScalePlan) -> ScalerKind:
-        api_version = SCALER_GROUP + "/" + SCALER_VERION
-        scaler_crd = ScalerKind(
+    def _generate_scale_plan_crd(self, plan: ScalePlan) -> ScalePlanCrd:
+        api_version = ElasticJobApi.GROUP + "/" + ElasticJobApi.VERION
+        name = self._scaleplan_name + "-" + str(self._scaleplan_index)
+        scale_crd = ScalePlanCrd(
             api_version=api_version,
-            kind=SCALER_KIND,
-            metadata={"name": "{}-scaler".format(self._job_name)},
-            spec=ScalerSpec(self._job_name),
+            kind=ElasticJobApi.SCALEPLAN_KIND,
+            metadata={"name": name},
+            spec=ScaleSpec(self._job_name),
+        )
+        scale_crd.set_owner_reference(
+            api_version, self._job_name, self._job_uid
         )
+
         for name, group_resource in plan.node_group_resources.items():
-            resource_spec = ScalerResourceSpec(
+            resource_spec = ContainerResourceSpec(
                 cpu=group_resource.node_resource.cpu,
                 memory=group_resource.node_resource.memory,
                 gpu_type=group_resource.node_resource.gpu_type,
                 gpu_num=group_resource.node_resource.gpu_num,
             )
-            replica_spec = ScalerReplicaResourceSpec(
+            replica_spec = ReplicaResourceSpec(
                 replicas=group_resource.count,
                 resource_spec=resource_spec,
             )
-            scaler_crd.spec.replica_resource_specs[name] = replica_spec
+            scale_crd.spec.replica_resource_specs[name] = replica_spec
 
         for node in plan.launch_nodes:
-            resource_spec = ScalerResourceSpec(
+            resource_spec = ContainerResourceSpec(
                 cpu=node.config_resource.cpu,
                 memory=node.config_resource.memory,
                 gpu_type=node.config_resource.gpu_type,
                 gpu_num=node.config_resource.gpu_num,
             )
-            name = get_pod_name(self._job_name, node.type, node.id)
-            scaler_crd.spec.node_resource_specs[name] = resource_spec
-        return scaler_crd
+            pod_meta = PodMeta(
+                node.name,
+                node.id,
+                node.type,
+                node.rank_index,
+                node.service_addr,
+                resource_spec,
+            )
+            scale_crd.spec.create_pods.append(pod_meta)
+
+        for node in plan.remove_nodes:
+            resource_spec = ContainerResourceSpec(
+                cpu=node.config_resource.cpu,
+                memory=node.config_resource.memory,
+                gpu_type=node.config_resource.gpu_type,
+                gpu_num=node.config_resource.gpu_num,
+            )
+            pod_meta = PodMeta(
+                node.name,
+                node.id,
+                node.type,
+                node.rank_index,
+                node.service_addr,
+                resource_spec,
+            )
+            scale_crd.spec.remove_pods.append(pod_meta)
+        scale_crd.spec.ps_hosts = plan.ps_addrs
+        scale_crd.metadata["labels"] = {
+            ScalePlanLabel.SCALE_TYPE_KEY: ScalePlanLabel.AUTO_SCALE
+        }
+        return scale_crd
```

## dlrover/python/master/scaler/factory.py

```diff
@@ -11,15 +11,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from dlrover.python.common.constants import PlatformType
 from dlrover.python.common.log import default_logger as logger
 from dlrover.python.master.scaler.elasticjob_scaler import ElasticJobScaler
 from dlrover.python.master.scaler.pod_scaler import PodScaler
+from dlrover.python.master.scaler.ray_scaler import ActorScaler
 
 
 def new_job_scaler(platform, job_name, namespace):
     logger.info("New %s JobScaler", platform)
     if platform == PlatformType.KUBERNETES:
         return ElasticJobScaler(job_name, namespace)
     elif platform == PlatformType.PY_KUBERNETES:
         return PodScaler(job_name, namespace)
+    elif platform == PlatformType.RAY:
+        return ActorScaler(job_name, namespace)
```

## dlrover/python/master/scaler/pod_scaler.py

```diff
@@ -23,23 +23,31 @@
 from dlrover.python.common.constants import (
     DistributionStrategy,
     ElasticJobLabel,
     NodeEnv,
     NodeStatus,
     NodeType,
 )
+from dlrover.python.common.global_context import Context
 from dlrover.python.common.log import default_logger as logger
 from dlrover.python.common.node import Node, NodeResource
 from dlrover.python.master.scaler.base_scaler import ScalePlan, Scaler
 from dlrover.python.scheduler.kubernetes import (
     NODE_SERVICE_PORTS,
     get_pod_name,
     k8sClient,
 )
 
+_dlrover_context = Context.singleton_instance()
+
+
+class FakeKubeResponse:
+    def __init__(self, obj):
+        self.data = json.dumps(obj)
+
 
 def append_pod_ip_to_env(env):
     pod_ip_var = V1EnvVar(
         name="MY_POD_IP",
         value_from=V1EnvVarSource(
             field_ref=V1ObjectFieldSelector(field_path="status.podIP")
         ),
@@ -54,54 +62,55 @@
         env.append(pod_ip_var)
         env.append(node_ip_var)
     else:
         env = [pod_ip_var, node_ip_var]
     return env
 
 
-class PodTemplate(object):
-    """PodTemplate is the template of replica in a job"""
-
-    def __init__(self, template):
-        self.spec = template["spec"]
-        self.restart_policy = self.spec["restartPolicy"]
-        self.main_container = self.spec["containers"][0]
-        self.name = self.main_container["name"]
-        self.image = self.main_container["image"]
-        self.command = self.main_container["command"]
-        self.args = self.main_container.get("args", [])
-        self.image_pull_policy = self.main_container.get(
-            "imagePullPolicy", "Always"
-        )
-        self.volumes = self.spec.get("volumes", [])
-
-
 class PodScaler(Scaler):
-    """PodScaler launches or removes Pods using Kubernetes Python APIs."""
+    """PodScaler launches or removes Pods using Kubernetes Python APIs
+    by a ScalePlan. After PodScaler receives a ScalePlan, it will
+    list all alive Pods of the job and push new `Node`s to a queue.
+    The thread of creating Pods will create Pods if there is `Node`
+    in a queue.
+    """
 
     def __init__(self, job_name, namespace):
         super(PodScaler, self).__init__(job_name)
-        self._k8s_client = k8sClient.singleton_instance(namespace, job_name)
+        self._k8s_client = k8sClient.singleton_instance(namespace)
         self._namespace = namespace
-        self._replica_template: Dict[str, PodTemplate] = {}
-        self._job = self._retry_to_get_job()
-        self._distribution_strategy = self._job["spec"].get(
-            "distributionStrategy", None
-        )
-        if "replicaSpecs" in self._job["spec"]:
-            for replica, spec in self._job["spec"]["replicaSpecs"].items():
-                self._replica_template[replica] = PodTemplate(spec["template"])
-
-        self._initial_nodes: List[Node] = []
+        self._replica_template: Dict[str, client.V1Pod] = {}
+        self._create_node_queue: List[Node] = []
         self._lock = threading.Lock()
         self._plan = ScalePlan()
         self._pod_stats: Dict[str, int] = {}
+        self._init_pod_config_by_job()
         threading.Thread(
             target=self._periodic_create_pod, name="pod-creater", daemon=True
         ).start()
+        self.api_client = client.ApiClient()
+        self._k8s_client.api_instance
+
+    def _init_pod_config_by_job(self):
+        self._job = self._retry_to_get_job()
+        self._distribution_strategy = self._job["spec"].get(
+            "distributionStrategy", None
+        )
+        worker_spec = self._job["spec"]["replicaSpecs"][NodeType.WORKER]
+        self._config_worker_num = worker_spec.get("replicas", 0)
+        if "replicaSpecs" in self._job["spec"]:
+            for replica, spec in self._job["spec"]["replicaSpecs"].items():
+                if replica == NodeType.DLROVER_MASTER:
+                    continue
+                pod = spec["template"]
+                pod["apiVesion"] = "v1"
+                pod["kind"] = "Pod"
+                res = FakeKubeResponse(pod)
+                v1pod = self._k8s_client.api_client.deserialize(res, "V1Pod")
+                self._replica_template[replica] = v1pod
 
     def _retry_to_get_job(self):
         for _ in range(3):
             job = self._k8s_client.get_custom_resource(
                 name=self._job_name,
                 group="elastic.iml.github.io",
                 version="v1alpha1",
@@ -110,65 +119,76 @@
             if job:
                 return job
             else:
                 time.sleep(5)
         raise ValueError("Cannot get the training job %s", self._job_name)
 
     def scale(self, plan: ScalePlan):
+        """Scale in/out Pods by a ScalePlan."""
         self._plan = plan
-        job_pods = self._stats_alive_pods()
+        job_pods = self._list_job_pods()
         logger.info("Scale the job by plan %s", plan.toJSON())
 
         with self._lock:
             for type, group_resource in plan.node_group_resources.items():
-                cur_pods = job_pods.get(type, []) + self._get_initial_pods(
-                    type
-                )
+                type_pods = job_pods.get(type, [])
+                max_pod_id = self._get_max_pod_id(type_pods)
+                normal_pods = []
+                for node in type_pods:
+                    if node.status in [
+                        NodeStatus.PENDING,
+                        NodeStatus.RUNNING,
+                        NodeStatus.SUCCEEDED,
+                    ]:
+                        normal_pods.append(node)
+                cur_pods = normal_pods + self._get_type_pod_in_queue(type)
                 if group_resource.count > len(cur_pods):
-                    self._scale_up_pods(type, plan, cur_pods)
+                    self._scale_up_pods(type, plan, cur_pods, max_pod_id)
                 elif group_resource.count < len(cur_pods):
                     self._scale_down_pods(type, plan, cur_pods)
             for node in plan.launch_nodes:
-                self._initial_nodes.append(node)
-            for pod_name in plan.remove_nodes:
-                removed = self._remove_not_create_pod(pod_name)
+                self._create_node_queue.append(node)
+            for node in plan.remove_nodes:
+                removed = self._remove_not_create_pod(node.name)
                 if not removed:
-                    self._k8s_client.delete_pod(pod_name)
+                    self._k8s_client.delete_pod(node.name)
             self._update_job_pods(job_pods)
 
     def _update_job_pods(self, job_pods: Dict[str, List[Node]]):
         for type in [
             NodeType.CHIEF,
             NodeType.MASTER,
             NodeType.PS,
             NodeType.WORKER,
             NodeType.EVALUATOR,
         ]:
-            cur_pods = job_pods.get(type, []) + self._get_initial_pods(type)
+            cur_pods = job_pods.get(type, []) + self._get_type_pod_in_queue(
+                type
+            )
             self._pod_stats[type] = len(cur_pods)
 
-    def _get_initial_pods(self, type):
-        initial_pods = []
-        for pod in self._initial_nodes:
+    def _get_type_pod_in_queue(self, type):
+        pods = []
+        for pod in self._create_node_queue:
             if pod.type == type:
-                initial_pods.append(pod)
-        return initial_pods
+                pods.append(pod)
+        return pods
 
     def _remove_not_create_pod(self, pod_name):
         not_created_pod = None
-        for pod in self._initial_nodes:
+        for pod in self._create_node_queue:
             if pod_name == get_pod_name(self._job_name, pod.type, pod.id):
                 not_created_pod = pod
                 break
         if not_created_pod:
-            self._initial_nodes.remove(not_created_pod)
+            self._create_node_queue.remove(not_created_pod)
             return True
         return False
 
-    def _stats_alive_pods(self):
+    def _list_job_pods(self):
         job_selector = ElasticJobLabel.JOB_KEY + "=" + self._job_name
         pod_list = self._k8s_client.list_namespaced_pod(job_selector)
         job_pods: Dict[str, List[Node]] = {}
         for pod in pod_list.items:
             pod_type = pod.metadata.labels[ElasticJobLabel.REPLICA_TYPE_KEY]
             if pod_type == NodeType.DLROVER_MASTER:
                 continue
@@ -182,77 +202,79 @@
                 node_type=pod_type,
                 node_id=pod_id,
                 name=pod.metadata.name,
                 rank_index=task_id,
                 status=pod.status.phase,
                 config_resource=pod_resource,
             )
-            if node.status in [
-                NodeStatus.PENDING,
-                NodeStatus.RUNNING,
-                NodeStatus.SUCCEEDED,
-            ]:
-                job_pods[pod_type].append(node)
+            job_pods[pod_type].append(node)
         return job_pods
 
     def _get_pod_resource(self, pod):
         resources = pod.spec.containers[0].resources
-        cpu = float(resources.requests.get("cpu", 0))
+        cpu = NodeResource.convert_cpu_to_decimal(
+            resources.requests.get("cpu", "0")
+        )
         if "memory" in resources.requests:
             memory = NodeResource.convert_memory_to_mb(
                 resources.requests["memory"]
             )
         else:
             memory = 0
         return NodeResource(cpu, memory)
 
     def _scale_up_pods(
         self,
         type,
         plan: ScalePlan,
         cur_pods: List[Node],
+        max_pod_id,
     ):
+        """The method will create a Node instances and push it into a queue.
+        The thread to create Pods will periodicall create Pods by
+        the Node instance in the queue."""
         cur_num = len(cur_pods)
         group_resource = plan.node_group_resources[type]
         up_num = group_resource.count - cur_num
-        max_id = self._get_max_pod_id(cur_pods)
         for i in range(up_num):
-            node_id = max_id + 1 + i
+            node_id = max_pod_id + 1 + i
             task_id = cur_num + i
             node = Node(
                 type,
                 node_id,
                 copy.deepcopy(group_resource.node_resource),
                 rank_index=task_id,
                 name=get_pod_name(self._job_name, type, node_id),
+                service_addr=self.get_node_service_addr(type, task_id),
             )
-            self._initial_nodes.append(node)
+            self._create_node_queue.append(node)
 
     def _get_max_pod_id(self, pods: List[Node]):
         max_id = -1
         for pod in pods:
             max_id = max(pod.id, max_id)
         return max_id
 
     def _scale_down_pods(
         self,
         type,
         plan: ScalePlan,
         cur_pods: List[Node],
     ):
+        """Delete Pods to scale down Pods."""
         group_resource = plan.node_group_resources[type]
         down_num = len(cur_pods) - group_resource.count
 
         not_created_pods = []
-        for pending_pod in self._initial_nodes:
+        for pending_pod in self._create_node_queue:
             if pending_pod.type == type:
                 not_created_pods.append(pending_pod)
         while down_num > 0 and not_created_pods:
             pod = not_created_pods.pop()
-            self._initial_nodes.remove(pod)
+            self._create_node_queue.remove(pod)
             down_num -= 1
         cur_pods.sort(key=lambda x: x.id, reverse=True)
         for pod in cur_pods:
             if down_num <= 0:
                 break
             self._k8s_client.delete_pod(pod.name)
             down_num -= 1
@@ -277,57 +299,96 @@
     def get_typed_pod(self, pod_type, id):
         pod_name = get_pod_name(self._job_name, pod_type, id)
         return self._k8s_client.get_pod(pod_name)
 
     def _periodic_create_pod(self):
         while True:
             with self._lock:
-                while self._initial_nodes:
-                    node = self._initial_nodes.pop(0)
+                while self._create_node_queue:
+                    node = self._create_node_queue.pop(0)
                     succeed = False
                     if self._check_cluster_ready_for_pod(node):
                         pod = self._create_pod(
                             node,
                             self._pod_stats,
                             self._plan.ps_addrs,
                         )
                         succeed = self._k8s_client.create_pod(pod)
                     if not succeed:
-                        self._initial_nodes.insert(0, node)
+                        self._create_node_queue.insert(0, node)
                         break
                     service_ready = self._create_service_for_pod(node)
                     if not service_ready:
-                        self._initial_nodes.insert(0, node)
+                        self._create_node_queue.insert(0, node)
                         break
             time.sleep(3)
 
     def _check_cluster_ready_for_pod(self, node: Node):
         """Check whether the resource of a cluster is enough to
         create a node"""
         return True
 
     def _create_pod(self, node: Node, pod_stats: Dict[str, int], ps_addrs):
         # Find that master pod that will be used as the owner reference
         # for the ps or worker pod.
-        node.update_priority(pod_stats[node.type])
+        node.update_priority(pod_stats.get(node.type, 0))
         pod_name = get_pod_name(self._job_name, node.type, node.id)
         logger.info(
             "Create Pod %s with resource %s",
             pod_name,
             node.config_resource.to_resource_dict(),
         )
         env: List[V1EnvVar] = []
         env = append_pod_ip_to_env(env)
 
         env.append(V1EnvVar(name=NodeEnv.WORKER_TYPE, value=node.type))
         env.append(V1EnvVar(name=NodeEnv.WORKER_ID, value=str(node.id)))
-        master_service = "elasticjob-{}-dlrover-master:50001".format(
-            self._job_name
+
+        # A deadlock can happen when pthread_atfork handler is running.
+        # For detail https://chromium.googlesource.com/external/github.com/grpc/grpc/+/refs/tags/v1.19.0-pre1/doc/fork_support.md  # noqa: E501
+        env.append(V1EnvVar(name=NodeEnv.GRPC_ENABLE_FORK, value="False"))
+
+        worker_num = self._config_worker_num
+        if worker_num == 0:
+            worker_num = pod_stats[node.type]
+        env.append(V1EnvVar(name=NodeEnv.WORKER_NUM, value=str(worker_num)))
+        env.append(
+            V1EnvVar(name=NodeEnv.WORKER_RANK, value=str(node.rank_index))
+        )
+        master_service = "elasticjob-{}-dlrover-master:{}".format(
+            self._job_name, _dlrover_context.master_port
+        )
+        env.append(
+            V1EnvVar(name=NodeEnv.DLROVER_MASTER_ADDR, value=master_service)
+        )
+        if self._distribution_strategy == DistributionStrategy.ALLREDUCE:
+            torch_master_ip = self.get_first_worker_host()
+            if torch_master_ip:
+                env.append(
+                    V1EnvVar(name=NodeEnv.RDZV_ENDPOINT, value=torch_master_ip)
+                )
+            else:
+                node_ip_var = V1EnvVar(
+                    name=NodeEnv.RDZV_ENDPOINT,
+                    value_from=V1EnvVarSource(
+                        field_ref=V1ObjectFieldSelector(
+                            field_path="status.podIP"
+                        )
+                    ),
+                )
+                env.append(node_ip_var)
+
+        env.append(
+            V1EnvVar(
+                name=NodeEnv.POD_NAME,
+                value_from=V1EnvVarSource(
+                    field_ref=V1ObjectFieldSelector(field_path="metadata.name")
+                ),
+            )
         )
-        env.append(V1EnvVar(name=NodeEnv.MASTER_ADDR, value=master_service))
 
         node_type = node.type
         if node.type not in self._replica_template:
             if node.type in [NodeType.CHIEF, NodeType.EVALUATOR]:
                 node_type = NodeType.WORKER
         if node_type not in self._replica_template:
             raise ValueError(
@@ -339,34 +400,42 @@
         labels = self._get_common_labels()
         pod = self._create_pod_obj(
             name=pod_name,
             pod_template=pod_template,
             resource_requests=node.config_resource.to_resource_dict(),
             resource_limits=node.config_resource.to_resource_dict(),
             priority=node.config_resource.priority,
-            owner=self._job,
             env=env,
             lifecycle=None,
             labels=labels,
         )
         # Add replica type and index
         pod.metadata.labels[ElasticJobLabel.REPLICA_TYPE_KEY] = node.type
         pod.metadata.labels[ElasticJobLabel.REPLICA_INDEX_KEY] = str(node.id)
         pod.metadata.labels[ElasticJobLabel.RANK_INDEX_KEY] = str(
             node.rank_index
         )
         self._patch_tf_config_into_env(pod, node, pod_stats, ps_addrs)
+        if (
+            _dlrover_context.auto_ps_enabled
+            or _dlrover_context.auto_worker_enabled
+        ):
+            pod.spec.containers[0].env.append(
+                V1EnvVar(name=NodeEnv.AUTO_MONITOR_WORKLOAD, value="true")
+            )
         return pod
 
+    def get_first_worker_host(self):
+        pod = self.get_typed_pod(NodeType.WORKER, 0)
+        if pod:
+            return pod.status.pod_ip
+        return ""
+
     def _patch_tf_config_into_env(self, pod, node: Node, pod_stats, ps_addrs):
-        if (
-            self._distribution_strategy
-            == DistributionStrategy.PARAMETER_SERVER
-            and ps_addrs
-        ):
+        if self._distribution_strategy == DistributionStrategy.PS and ps_addrs:
             tf_config = new_tf_config(
                 pod_stats,
                 self.get_node_service_addr,
                 node.type,
                 node.rank_index,
                 ps_addrs,
             )
@@ -386,57 +455,56 @@
             service_name = node.service_addr.split(".")[0]
         else:
             service_name = get_pod_name(
                 self._job_name, node.type, node.rank_index
             )
         if not self._k8s_client.get_service(service_name):
             succeed = self._create_service_with_retry(
-                node.type, node.id, service_name
+                node.type, node.rank_index, service_name
             )
             service_ready = service_ready and succeed
         else:
             succeed = self._patch_service_with_retry(
-                node.type, node.id, service_name
+                node.type, node.rank_index, service_name
             )
             service_ready = service_ready and succeed
         if not service_ready:
             logger.error(
                 "Fail to create service %s for the %s pod %s",
                 service_name,
                 node.type,
                 node.id,
             )
             self._delete_typed_pod(node.type, node.id)
             service_ready = False
         return service_ready
 
     def _create_service_with_retry(
-        self, pod_type, pod_id, service_name, retry_num=5
+        self, pod_type, rank_id, service_name, retry_num=5
     ):
         for _ in range(retry_num):
-            succeed = self._create_service(pod_type, pod_id, service_name)
+            succeed = self._create_service(pod_type, rank_id, service_name)
             if succeed:
                 return succeed
             else:
                 time.sleep(5)
         return False
 
-    def _create_service(self, pod_type, pod_id, service_name):
+    def _create_service(self, pod_type, rank_id, service_name):
         # Use master pod as service owner so the service will not be
         #  deleted if the corresponding pod is deleted.
         service = self._create_service_obj(
             name=service_name,
             port=NODE_SERVICE_PORTS[pod_type],
             target_port=NODE_SERVICE_PORTS[pod_type],
             replica_type=pod_type,
-            replica_index=pod_id,
-            owner=self._job,
+            rank_index=rank_id,
         )
-        self._k8s_client.create_service(service)
-        return service
+
+        return self._k8s_client.create_service(service)
 
     def _patch_service_with_retry(
         self, pod_type, new_id, service_name, retry_num=5
     ):
         for _ in range(retry_num):
             succeed = self._patch_service(pod_type, new_id, service_name)
             if succeed:
@@ -447,146 +515,92 @@
 
     def _create_service_obj(
         self,
         name,
         port,
         target_port,
         replica_type,
-        replica_index,
-        owner=None,
+        rank_index,
     ):
         labels = self._get_common_labels()
 
         metadata = client.V1ObjectMeta(
             name=name,
             labels=labels,
             # Note: We have to add at least one annotation here.
             # Otherwise annotation is `None` and cannot be modified
             # using `with_service()` for cluster specific information.
             annotations=labels,
-            owner_references=self._create_owner_reference(owner)
-            if owner
-            else None,
+            owner_references=[self._create_job_owner_reference()],
             namespace=self._namespace,
         )
         selector = {
             ElasticJobLabel.JOB_KEY: self._job_name,
             ElasticJobLabel.REPLICA_TYPE_KEY: replica_type,
-            ElasticJobLabel.REPLICA_INDEX_KEY: str(replica_index),
+            ElasticJobLabel.RANK_INDEX_KEY: str(rank_index),
         }
         spec = client.V1ServiceSpec(
             ports=[client.V1ServicePort(port=port, target_port=target_port)],
             selector=selector,
             type=None,
         )
         service = client.V1Service(
             api_version="v1", kind="Service", metadata=metadata, spec=spec
         )
         return service
 
-    def _patch_service(self, pod_type, id, service_name):
+    def _patch_service(self, pod_type, rank_id, service_name):
         service = self._create_service_obj(
             name=service_name,
             port=NODE_SERVICE_PORTS[pod_type],
             target_port=NODE_SERVICE_PORTS[pod_type],
             replica_type=pod_type,
-            replica_index=id,
-            owner=self._job,
+            rank_index=rank_id,
         )
         return self._k8s_client.patch_service(service_name, service)
 
     def _create_pod_obj(
         self,
         name,
-        pod_template: PodTemplate,
+        pod_template: client.V1Pod,
         resource_requests: Dict[str, float],
         resource_limits: Dict[str, float],
-        owner,
         lifecycle,
         env,
         priority,
         labels,
         termination_period=None,
     ):
+        pod = copy.deepcopy(pod_template)
+        main_container: client.V1Container = pod.spec.containers[0]
         resource_limits = (
             resource_limits if len(resource_limits) > 0 else resource_requests
         )
-
-        volume_mounts = []
-        mounts_conf = pod_template.main_container.get("volumeMounts", [])
-        for mounts in mounts_conf:
-            volume_mounts.append(
-                client.V1VolumeMount(
-                    name=mounts["name"],
-                    mount_path=mounts["mountPath"],
-                    sub_path=mounts.get("sub_path", None),
-                )
-            )
-        container = client.V1Container(
-            name="main",
-            image=pod_template.image,
-            command=pod_template.command,
-            args=pod_template.args,
-            resources=client.V1ResourceRequirements(
-                requests=resource_requests,
-                limits=resource_limits,
-            ),
-            image_pull_policy=pod_template.image_pull_policy,
-            env=env,
-            lifecycle=lifecycle,
-            volume_mounts=volume_mounts,
-        )
-
-        volumes = []
-        for volume in pod_template.volumes:
-            pvc_volume_source = client.V1PersistentVolumeClaimVolumeSource(
-                claim_name=volume["persistentVolumeClaim"]["claimName"],
-                read_only=False,
-            )
-            volume = client.V1Volume(
-                name=volume["name"], persistent_volume_claim=pvc_volume_source
-            )
-            volumes.append(volume)
-
-        # Pod
-        spec = client.V1PodSpec(
-            containers=[container],
-            restart_policy=pod_template.restart_policy,
-            priority_class_name=priority,
-            termination_grace_period_seconds=termination_period,
-            volumes=volumes,
-        )
-
-        pod = client.V1Pod(
-            api_version="v1",
-            kind="Pod",
-            spec=spec,
-            metadata=client.V1ObjectMeta(
-                name=name,
-                labels=labels,
-                owner_references=self._create_owner_reference(owner),
-                namespace=self._namespace,
-            ),
+        main_container.resources = client.V1ResourceRequirements(
+            requests=resource_requests,
+            limits=resource_limits,
+        )
+        main_container.env = env
+        main_container.lifecycle = lifecycle
+        pod.spec.priority_class_name = priority
+        pod.spec.termination_grace_period_seconds = termination_period
+        pod.metadata = client.V1ObjectMeta(
+            name=name,
+            labels=labels,
+            owner_references=[self._create_job_owner_reference()],
+            namespace=self._namespace,
         )
         return pod
 
-    @staticmethod
-    def _create_owner_reference(job):
-        owner_ref = (
-            [
-                client.V1OwnerReference(
-                    api_version="elastic.iml.github.io/v1alpha1",
-                    block_owner_deletion=True,
-                    kind="ElasticJob",
-                    name=job["metadata"]["name"],
-                    uid=job["metadata"]["uid"],
-                )
-            ]
-            if job
-            else None
+    def _create_job_owner_reference(self):
+        owner_ref = k8sClient.create_owner_reference(
+            api_version="elastic.iml.github.io/v1alpha1",
+            kind="ElasticJob",
+            name=self._job["metadata"]["name"],
+            uid=self._job["metadata"]["uid"],
         )
         return owner_ref
 
 
 def new_tf_config(
     pod_stats: Dict[str, int],
     new_service_fn,
```

## dlrover/python/master/shard/base_dataset_manager.py

```diff
@@ -102,14 +102,22 @@
     ):
         self.todo: List[Task] = []
         self.doing: Dict[int, DoingTask] = {}
 
         self._task_type = task_type
         self._batch_size = batch_size
         self._dataset_splitter = dataset_splitter
+        self._latest_task_end_time = 0
+
+    def get_latest_task_end_time(self):
+        return self._latest_task_end_time
+
+    def get_task_count(self):
+        epoch_task_count = self._dataset_splitter.get_shard_count()
+        return len(self.todo) + epoch_task_count
 
     @abstractmethod
     def get_epoch(self):
         """Get the training epoch"""
         pass
 
     @abstractmethod
```

## dlrover/python/master/shard/batch_dataset_manager.py

```diff
@@ -96,15 +96,15 @@
             "todo.extend: %d tasks created for dataset = %s.",
             len(tasks),
             self._dataset_splitter.dataset_name,
         )
         self.todo.extend(tasks)
 
     def report_task_status(self, task_id, success):
-        doing_task = self.doing.pop(task_id)
+        doing_task = self.doing.pop(task_id, None)
         if not doing_task:
             logger.warning(
                 "Unknown task_id: %d of dataset %s"
                 % (task_id, self._dataset_splitter.dataset_name)
             )
             success = False
         elif not success:
@@ -112,28 +112,31 @@
                 "Task %d of %s failed "
                 % (task_id, self._dataset_splitter.dataset_name)
             )
             self.recover_task(doing_task.task)
         else:
             self._update_completed_step(doing_task.task)
             logger.info(
-                "Task:%d completed, %d remaining tasks for Dataset %s",
+                "Task:%d completed, %d doing tasks and %d todo "
+                "tasks of dataset %s",
                 task_id,
-                len(self.todo) + len(self.doing),
+                len(self.doing),
+                len(self.todo),
                 self._dataset_splitter.dataset_name,
             )
             task_completed_time = time.time() - doing_task.start_time
             if task_completed_time > self._max_task_completed_time:
                 self._max_task_completed_time = task_completed_time
         return success, doing_task
 
     def _update_completed_step(self, task: Task):
         record_count = task.shard.end - task.shard.start
         batch_count = math.ceil(record_count / self._batch_size)
         self._completed_step += batch_count
+        self._latest_task_end_time = int(time.time())
 
     def get_completed_step(self):
         return self._completed_step
 
     def recover_task(self, task):
         if not self._check_exceed_max_task_retries(task):
             self.todo.append(task)
@@ -150,38 +153,51 @@
 
     def get_doing_tasks(self):
         return self.doing
 
     def checkpoint(self):
         todo_shards = []
         for task in self.todo:
-            todo_shards.append([task.shard.start, task.shard.end])
+            shard = [task.shard.start, task.shard.end]
+            if task.shard.record_indices:
+                shard.append(task.shard.record_indices)
+            todo_shards.append(shard)
 
         doing_shards = []
         for task_id in self.doing:
             task = self.doing[task_id].task
-            doing_shards.append([task.shard.start, task.shard.end])
+            shard = [task.shard.start, task.shard.end]
+            if task.shard.record_indices:
+                shard.append(task.shard.record_indices)
+            doing_shards.append(shard)
 
         return DatasetShardCheckpoint(
             dataset_name=self._dataset_splitter.dataset_name,
             todo=todo_shards,
             doing=doing_shards,
             epoch=self._dataset_splitter.epoch,
         )
 
     def restore_checkpoint(self, checkpoint: DatasetShardCheckpoint):
         """Restore the task manager from a checkpoint"""
         self._dataset_splitter.epoch = checkpoint.epoch
         self.todo = []
+        self.doing = {}
         for shard_indices in checkpoint.doing + checkpoint.todo:
+            record_indices = None
+            if len(shard_indices) > 2:
+                record_indices = shard_indices[2]
             shard = Shard(
                 name=self._dataset_splitter.dataset_name,
                 start=shard_indices[0],
                 end=shard_indices[1],
+                record_indices=record_indices,
             )
             self.todo.append(
                 Task(
-                    self._dataset_splitter.dataset_name,
+                    self._task_id,
                     self._task_type,
                     shard,
                 )
             )
+            self._task_id += 1
+        logger.info("Restore %s todo tasks", len(self.todo))
```

## dlrover/python/master/shard/dataset_splitter.py

```diff
@@ -121,14 +121,19 @@
         """Get all shards of the dataset"""
         pass
 
     def epoch_finished(self) -> bool:
         """Check wether to finish the configured epochs"""
         return self.epoch >= self._num_epochs
 
+    def get_shard_count(self) -> int:
+        remain_epoch = self._num_epochs - self.epoch
+        shard_count_per_epoch = self._dataset_size // self._shard_size
+        return shard_count_per_epoch * remain_epoch
+
 
 class TableDatasetSplitter(DatasetSplitter):
     """TableDatasetSplitter split a dataset stored in a table like Hive or
     MaxCompute (ODPS) table. We can read data by record indices in the table.
     The shard contains index ranges [start, end) of batch records.
     Attributes:
         dataset_name: the name of the table.
@@ -286,17 +291,20 @@
         if self._shuffle:
             random.shuffle(record_indices)
         for shard_start_idx in range(start_idx, end_idx, self._shard_size):
             shard_end_idx = min(
                 shard_start_idx + self._shard_size,
                 end_idx,
             )
-            size = shard_end_idx - shard_start_idx
-            shard_indices = record_indices[0:size]
-            record_indices = record_indices[size:]
+            if self._shuffle:
+                size = shard_end_idx - shard_start_idx
+                shard_indices = record_indices[0:size]
+                record_indices = record_indices[size:]
+            else:
+                shard_indices = []
             shards.append(
                 Shard(
                     name=self._dataset_name,
                     start=shard_start_idx,
                     end=shard_end_idx,
                     record_indices=shard_indices,
                 )
```

## dlrover/python/master/shard/task_manager.py

```diff
@@ -23,15 +23,14 @@
 from dlrover.python.master.monitor.speed_monitor import SpeedMonitor
 from dlrover.python.master.shard.base_dataset_manager import (
     DatasetManger,
     DatasetShardCheckpoint,
 )
 from dlrover.python.master.shard.batch_dataset_manager import (
     BatchDatasetManager,
-    DoingTask,
 )
 from dlrover.python.master.shard.dataset_splitter import DatasetSplitter
 
 _TASK_TIMEOUT_THRESHOLD_SECS = 1800
 
 
 class TaskManager(object):
@@ -59,18 +58,16 @@
         batch_size,
         dataset_size,
         dataset_name,
         dataset_splitter: DatasetSplitter,
         task_type=elastic_training_pb2.NONE,
     ):
         logger.info(
-            "New %s dataset with batch size = %s, dataset size = %s",
-            dataset_name,
-            batch_size,
-            dataset_size,
+            f"New {task_type} dataset {dataset_name} with, "
+            f"batch size = {batch_size} dataset size = {dataset_size}"
         )
 
         with self._lock:
             if dataset_name in self._datasets:
                 logger.info(
                     "The shards for dataset %s have already been initialized. "
                     "Ignore these shard parameters.",
@@ -99,17 +96,22 @@
                 task = dataset.get_task(node_type, node_id)
                 if (
                     task.task_type == elastic_training_pb2.EVALUATION
                     and node_type == NodeType.WORKER
                 ):
                     # All workers will stop training to evaluate the model
                     # at parallel validation
+                    logger.info(
+                        "Reset speed monitor if the worker starts evaluation"
+                    )
                     self._speed_monitor.reset_running_speed_monitor()
+                    self._speed_monitor.set_worker_start_eval_time(node_id)
                 if task.task_type == elastic_training_pb2.TRAINING:
                     self._speed_monitor.add_running_worker(node_type, node_id)
+                    self._speed_monitor.update_worker_eval_time(node_id)
                 self._worker_start_task_time[node_id] = time.time()
                 return task
             else:
                 return None
 
     def get_dataset(self, dataset_name):
         return self._datasets.get(dataset_name, None)
@@ -124,40 +126,67 @@
             if not dataset:
                 raise ValueError(
                     "There is no dataset shard for the dataset {}".format(
                         dataset_name
                     )
                 )
             success, doing_task = dataset.report_task_status(task_id, success)
-            self._worker_start_task_time[doing_task.node_id] = time.time()
-            return doing_task.task, doing_task.node_id
+            if success:
+                self._worker_start_task_time[doing_task.node_id] = time.time()
+                return doing_task.task, doing_task.node_id
+            return None, None
+
+    def task_hanged(self):
+        dataset_hang = []
+        for _, ds in self._datasets.items():
+            end_time = ds.get_latest_task_end_time()
+            hang = (
+                end_time > 0
+                and time.time() - end_time > _TASK_TIMEOUT_THRESHOLD_SECS
+            )
+            dataset_hang.append(hang)
+        if dataset_hang:
+            return all(dataset_hang)
+        return False
 
     def finished(self):
         """Return if all tasks are done"""
         if not self._datasets:
             return False
         finished = all([ds.completed() for ds in self._datasets.values()])
         return finished
 
     def recover_tasks(self, node_type, node_id):
         """Recover doing tasks for a dead worker if needed"""
         for name, dataset in self._datasets.items():
-            doing_tasks: Dict[int, DoingTask] = dataset.get_doing_tasks()
+            doing_tasks = dataset.doing
+            if not doing_tasks:
+                continue
             ids = [
                 task_id
                 for task_id, doing_task in doing_tasks.items()
                 if doing_task.node_id == node_id
                 and doing_task.node_type == node_type
             ]
+            if not ids:
+                continue
             request = elastic_training_pb2.ReportTaskResultRequest()
+            recover_tasks = []
             for id in ids:
                 request.task_id = id
                 request.dataset_name = name
+                recover_tasks.append(id)
                 self.report_dataset_task(request, False)
-            logger.info("Recover tasks assigned to %s-%d", node_type, node_id)
+            logger.info(
+                "Recover tasks %s of dataset %s assigned to %s-%d",
+                recover_tasks,
+                name,
+                node_type,
+                node_id,
+            )
 
     def start(self):
         if self._worker_restart_timeout > 0:
             threading.Thread(
                 target=self._check_and_reassign_timeout_tasks,
                 name="check_timeout_tasks",
                 daemon=True,
@@ -171,17 +200,19 @@
 
     def _invoke_task_timeout_callback(self, worker_id):
         for callback_fn in self._task_timeout_callbacks:
             callback_fn(worker_id)
 
     def _check_and_reassign_timeout_tasks(self):
         """Check whether there are timeout tasks periodically."""
-        logger.info("Start the thread to monitor timeout tasks")
+        logger.info("Start the thread to monitor timeout tasks.")
         while True:
             for _, dataset in self._datasets.items():
+                # Copy doing task list because the doing list will pop items
+                # in the following loop.
                 doing_tasks = dataset.doing.copy()
                 cur = time.time()
                 for task_id, doing_task in doing_tasks.items():
                     start = self._worker_start_task_time.get(
                         doing_task.node_id, cur
                     )
                     if (
@@ -194,14 +225,15 @@
                         )
                     ):
                         logger.info(
                             "worker %d timeout with task %d, relaunch it",
                             doing_task.node_id,
                             task_id,
                         )
+                        dataset.report_task_status(task_id, success=False)
                         self._invoke_task_timeout_callback(doing_task.node_id)
                         break
             time.sleep(30)
 
     def get_dataset_checkpoint(self, dataset_name):
         """Get the data shard checkpoint by dataset name.
 
@@ -215,29 +247,29 @@
             if dataset_name in self._datasets:
                 dataset = self._datasets[dataset_name]
                 return dataset.checkpoint()
             else:
                 return None
 
     def restore_dataset_from_checkpoint(self, checkpoint):
-        # try:
-        dataset_checkpoint = DatasetShardCheckpoint.from_json(checkpoint)
-        dataset = self._datasets.get(dataset_checkpoint.dataset_name, None)
-        if not dataset:
-            logger.error("No dataset for checkpoint %s", checkpoint)
+        try:
+            dataset_checkpoint = DatasetShardCheckpoint.from_json(checkpoint)
+            dataset = self._datasets.get(dataset_checkpoint.dataset_name, None)
+            if not dataset:
+                logger.error("No dataset for checkpoint %s", checkpoint)
 
-        dataset.restore_checkpoint(dataset_checkpoint)
-        logger.info(
-            "Restore %s dataset shards from checkpoint %s",
-            dataset_checkpoint.dataset_name,
-            checkpoint,
-        )
-        return True
-        # except Exception as e:
-        #     logger.error("Fail to restore shards from the checkpoint %s", e)
+            dataset.restore_checkpoint(dataset_checkpoint)
+            logger.info(
+                "Restore %s dataset with %s shards from checkpoint",
+                dataset_checkpoint.dataset_name,
+                len(dataset.todo) + len(dataset.doing),
+            )
+            return True
+        except Exception as e:
+            logger.error("Fail to restore shards from the checkpoint %s", e)
 
         return False
 
     def get_dataset_epoch(self, dataset_name):
         if dataset_name in self._datasets:
             return self._datasets[dataset_name].get_epoch()
         else:
```

## dlrover/python/master/stats/job_collector.py

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 The ElasticDL Authors. All rights reserved.
+# Copyright 2021 The DLRover Authors. All rights reserved.
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
@@ -13,14 +13,15 @@
 
 import copy
 import threading
 import time
 from abc import ABCMeta, abstractmethod
 from typing import Dict, List
 
+from dlrover.python.common.constants import MemoryUnit
 from dlrover.python.common.log import default_logger as logger
 from dlrover.python.master.monitor.speed_monitor import SpeedMonitor
 from dlrover.python.master.stats.reporter import JobMeta, StatsReporter
 from dlrover.python.master.stats.training_metrics import (
     CustomMetricKey,
     DatasetMetric,
     DatasetType,
@@ -30,18 +31,18 @@
     TensorStats,
     TrainingHyperParams,
 )
 from dlrover.python.master.watcher.base_watcher import Node
 
 
 class BaseMetricCollector(metaclass=ABCMeta):
-    def __init__(self, job_meta: JobMeta, reporter_type=None):
+    def __init__(self, job_meta: JobMeta, reporter=None):
         self._job_meta = job_meta
         self._stats_reporter = StatsReporter.new_stats_reporter(
-            job_meta, reporter_type
+            job_meta, reporter
         )
 
     @classmethod
     def catch_exception(cls, func):
         def wrapper(self, *args, **kwargs):
             try:
                 return func(self, *args, **kwargs)
@@ -76,17 +77,17 @@
 
 class JobMetricCollector(BaseMetricCollector):
     """The collector receives model parameters message from workers
     and processes the message. Then, it will report model parameters
     to EasyDL server.
     """
 
-    def __init__(self, job_uuid, namespace, cluster, user):
+    def __init__(self, job_uuid, namespace, cluster, user, reporter=None):
         job_meta = JobMeta(job_uuid, namespace, cluster, user)
-        super(JobMetricCollector, self).__init__(job_meta)
+        super(JobMetricCollector, self).__init__(job_meta, reporter=reporter)
         self._runtime_metric = RuntimeMetric([])
         self.dataset_metric = None
         self._flops = 0
         self._batch_size = 0
         self._report_runtime_thread = threading.Thread(
             target=self.report_runtime_stats_periodically, daemon=True
         )
@@ -133,15 +134,18 @@
     def collect_custom_data(self):
         self._stats_reporter.report_customized_data(self._custom_metric)
 
     def collect_runtime_stats(
         self, speed_monitor: SpeedMonitor, running_nodes: List[Node]
     ):
         """Set runtime info by global step"""
-        if speed_monitor.running_speed == 0:
+        if (
+            speed_monitor.running_speed == 0
+            or not speed_monitor.all_worker_joined()
+        ):
             return
         self._runtime_metric.clear()
         self._runtime_metric.global_step = speed_monitor.completed_global_step
         self._runtime_metric.timestamp = int(time.time())
         self._runtime_metric.speed = speed_monitor.running_speed
 
         if (
@@ -151,15 +155,15 @@
         ):
             self._custom_metric[
                 CustomMetricKey.INIT_TRAINING_TIME
             ] = speed_monitor.init_training_time
             self.collect_custom_data()
         for node in running_nodes:
             node_sample = copy.deepcopy(node)
-            node_sample.used_resource.memory *= 1024
+            node_sample.used_resource.memory *= MemoryUnit.MB
             if (node.type, node.id) in speed_monitor.running_workers:
                 self._runtime_metric.running_nodes.append(node_sample)
             else:
                 self._runtime_metric.running_nodes.append(node_sample)
         if not self._report_runtime_thread.is_alive():
             self._report_runtime_thread.start()
```

## dlrover/python/master/stats/reporter.py

```diff
@@ -8,39 +8,52 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
+import json
 from abc import ABCMeta, abstractmethod
 from typing import List
 
+from dlrover.proto import brain_pb2
+from dlrover.python.brain.client import GlobalBrainClient
+from dlrover.python.common.constants import ReporterType
 from dlrover.python.common.log import default_logger as logger
 from dlrover.python.common.singleton import singleton
 from dlrover.python.master.stats.training_metrics import (
     DatasetMetric,
     ModelMetric,
     RuntimeMetric,
     TrainingHyperParams,
 )
 
+DATA_STORE = "base_datastore"
+_MAX_SAMPLE_NUM_PER_STAT = 5
+
 
 class JobMeta(object):
     def __init__(self, uuid, name="", namespace="", cluster="", user=""):
         self.uuid = uuid
         self.name = name
         self.namespace = namespace
         self.cluster = cluster
         self.user = user
 
 
-class ReporterType(object):
-    LOCAL = "local"
-    DLROVER_BRAIN = "brain"
+def init_job_metrics_message(job_meta: JobMeta):
+    job_metrics = brain_pb2.JobMetrics()
+    job_metrics.data_store = DATA_STORE
+    job_metrics.job_meta.uuid = job_meta.uuid
+    job_metrics.job_meta.name = job_meta.name
+    job_metrics.job_meta.user = job_meta.user
+    job_metrics.job_meta.cluster = job_meta.cluster
+    job_metrics.job_meta.namespace = job_meta.namespace
+    return job_metrics
 
 
 class StatsReporter(metaclass=ABCMeta):
     def __init__(self, job_meta: JobMeta):
         self._job_meta = job_meta
 
     @abstractmethod
@@ -68,20 +81,23 @@
         pass
 
     @abstractmethod
     def report_customized_data(self, data):
         pass
 
     @classmethod
-    def new_stats_reporter(cls, job_meta, reporter_type=None):
-        if not reporter_type or reporter_type == ReporterType.LOCAL:
-            logger.info("New local stats reporter")
+    def new_stats_reporter(cls, job_meta, reporter=None):
+        if not reporter or reporter == ReporterType.LOCAL:
+            logger.info("New local stats reporter.")
             return LocalStatsReporter(job_meta)
+        elif reporter == ReporterType.DLROVER_BRAIN:
+            logger.info("New brain stats reporter.")
+            return BrainReporter(job_meta)
         else:
-            logger.warning("Not support stats collector %s", reporter_type)
+            logger.warning("Not support stats collector %s.", reporter)
 
 
 @singleton
 class LocalStatsReporter(StatsReporter):
     def __init__(self, job_meta):
         self._job_meta = job_meta
         self._runtime_stats: List[RuntimeMetric] = []
@@ -99,19 +115,121 @@
         self._training_hype_params = params
 
     def report_model_metrics(self, metric: ModelMetric):
         self._model_metric = metric
 
     def report_runtime_stats(self, stats: RuntimeMetric):
         self._runtime_stats.append(copy.deepcopy(stats))
+        latest_stat = self._runtime_stats[-1]
+        index = 0
+        for i, stat in enumerate(self._runtime_stats):
+            if len(stat.running_nodes) == len(latest_stat.running_nodes):
+                index = i
+                break
+        if len(self._runtime_stats) - index > _MAX_SAMPLE_NUM_PER_STAT:
+            new_stats = self._runtime_stats[0:index]
+            start_index = len(self._runtime_stats) - _MAX_SAMPLE_NUM_PER_STAT
+            new_stats.extend(self._runtime_stats[start_index:])
+            self._runtime_stats = new_stats
 
     def report_job_type(self, job_type: str):
         self._job_type = job_type
 
     def report_job_exit_reason(self, reason: str):
         self._exit_reason = reason
 
     def report_customized_data(self, data):
         self._custom_data = data
 
     def get_runtime_stats(self) -> List[RuntimeMetric]:
         return self._runtime_stats
+
+
+@singleton
+class BrainReporter(StatsReporter):
+    def __init__(self, job_meta: JobMeta) -> None:
+        self._job_meta = job_meta
+        self._brain_client = GlobalBrainClient.BRAIN_CLIENT
+
+    def report_dataset_metric(self, dataset: DatasetMetric):
+        self._brain_client.report_training_set_metric(self._job_meta, dataset)
+
+    def report_training_hyper_params(self, params: TrainingHyperParams):
+        self._brain_client.report_training_hyper_params(self._job_meta, params)
+
+    def report_model_metrics(self, metric: ModelMetric):
+        """Report the model meta to EasyDL DB.
+        Args:
+            job_uuid: str, the unique id of the job which is usually
+                the uuid in the job yaml of k8s.
+            model size: int, the size of the NN model.
+            variable_count: int, the total count of variables in the model.
+            ops_count: int, the total count of ops in the model.
+        """
+        job_metrics = init_job_metrics_message(self._job_meta)
+        job_metrics.metrics_type = brain_pb2.MetricsType.Model_Feature
+        metrics = job_metrics.model_feature
+        metrics.total_variable_size = metric.tensor_stats.total_variable_size
+        metrics.variable_count = metric.tensor_stats.variable_count
+        metrics.op_count = metric.op_stats.op_count
+        self._brain_client.report_metrics(job_metrics)
+
+    def report_runtime_stats(self, stats: RuntimeMetric):
+        self._brain_client.report_node_runtime_stats(
+            self._job_meta, self._job_meta.namespace, stats
+        )
+
+    def report_job_type(self, job_type: str):
+        """Report the job type to EasyDL DB.
+        Args:
+            job_uuid: str, the unique id of the job which is usually
+                the uuid in the job yaml of k8s.
+            job_type: str, the type of training job like "alps", "atorch",
+                "penrose" and so on.
+        """
+        job_metrics = init_job_metrics_message(self._job_meta)
+        job_metrics.metrics_type = brain_pb2.MetricsType.Type
+        job_metrics.type = job_type
+        logger.info("Report job_type = %s", job_type)
+        self._brain_client.report_metrics(job_metrics)
+
+    def report_job_exit_reason(self, reason: str):
+        self._brain_client.report_job_exit_reason(self._job_meta, reason)
+
+    def report_customized_data(self, data):
+        """Report the job resource to EasyDL DB.
+        Args:
+            job_uuid: str, the unique id of the job which is usually
+                the uuid in the job yaml of k8s.
+            cutomized_data: A dictionary.
+        """
+        job_metrics = init_job_metrics_message(self._job_meta)
+        job_metrics.metrics_type = brain_pb2.MetricsType.Customized_Data
+        job_metrics.customized_data = json.dumps(data)
+        self._brain_client.report_metrics(job_metrics)
+
+    def report_job_meta(self):
+        """Report the job meta to EasyDL DB.
+        Args:
+            job_uuid: str, the unique id of the job which is usually
+                the uuid in the job yaml of k8s.
+            job_name: str, the name of training job.
+            user_id: the user id.
+        """
+        job_metrics = init_job_metrics_message(self._job_meta)
+        job_metrics.metrics_type = brain_pb2.MetricsType.Workflow_Feature
+        metrics = job_metrics.workflow_feature
+        metrics.job_name = self._job_meta.name
+        metrics.user_id = self._job_meta.user
+        self._brain_client.report_metrics(job_metrics)
+
+    def report_job_resource(self, job_resource):
+        """Report the job resource to EasyDL DB.
+        Args:
+            job_uuid: str, the unique id of the job which is usually
+                the uuid in the job yaml of k8s.
+            job_resource: dlrover.python.master.resource.JobResource instance.
+        """
+        job_metrics = init_job_metrics_message(self._job_meta)
+        job_metrics.metrics_type = brain_pb2.MetricsType.Resource
+        job_metrics.resource = job_resource.toJSON()
+        self._brain_client.report_metrics(job_metrics)
```

## dlrover/python/master/stats/training_metrics.py

```diff
@@ -116,17 +116,20 @@
         self.total_variable_size = total_variable_size
         self.max_variable_size = max_variable_size
 
 
 class OpStats(object):
     """TensorStats contains OP statistics of a deep learning model"""
 
-    def __init__(self, op_count, update_op_count, input_fetch_dur, flops):
+    def __init__(
+        self, op_count, update_op_count, read_op_count, input_fetch_dur, flops
+    ):
         self.op_count = op_count
         self.update_op_count = update_op_count
+        self.read_op_count = read_op_count
         self.input_fetch_dur = input_fetch_dur
         self.flops = flops
 
 
 class ModelMetric(object):
     """ModelMetric contains profiling data of a model."""
```

## dlrover/python/master/watcher/factory.py

```diff
@@ -9,16 +9,35 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from dlrover.python.common.constants import PlatformType
 from dlrover.python.common.log import default_logger as logger
-from dlrover.python.master.watcher.pod_watcher import PodWatcher
+from dlrover.python.master.watcher.k8s_watcher import (
+    K8sScalePlanWatcher,
+    PodWatcher,
+)
+from dlrover.python.master.watcher.ray_watcher import (
+    ActorWatcher,
+    RayScalePlanWatcher,
+)
 
 
 def new_node_watcher(platform, job_name, namespace):
     logger.info("New %s NodeWatcher", platform)
     if platform in (PlatformType.KUBERNETES, PlatformType.PY_KUBERNETES):
         return PodWatcher(job_name, namespace)
+    elif platform in (PlatformType.RAY):
+        return ActorWatcher(job_name, namespace)
+    else:
+        raise ValueError("Not support engine %s", platform)
+
+
+def new_scale_plan_watcher(platform, job_name, namespace, job_uuid):
+    logger.info("New %s NodeWatcher", platform)
+    if platform in (PlatformType.KUBERNETES, PlatformType.PY_KUBERNETES):
+        return K8sScalePlanWatcher(job_name, namespace, job_uuid)
+    elif platform in (PlatformType.RAY):
+        return RayScalePlanWatcher(job_name, namespace, job_uuid)
     else:
         raise ValueError("Not support engine %s", platform)
```

## dlrover/python/scheduler/factory.py

```diff
@@ -10,23 +10,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from dlrover.python.common.constants import PlatformType
 from dlrover.python.common.log import default_logger as logger
 from dlrover.python.scheduler.kubernetes import K8sElasticJob, K8sJobArgs
+from dlrover.python.scheduler.ray import RayElasticJob, RayJobArgs
 
 
 def new_elastic_job(platform, job_name, namespace):
     logger.info("New %s ElasticJob", platform)
     if platform in (PlatformType.KUBERNETES, PlatformType.PY_KUBERNETES):
         return K8sElasticJob(job_name, namespace)
+    elif platform in (PlatformType.RAY):
+        return RayElasticJob(job_name, namespace)
     else:
         raise ValueError("Not support engine %s", platform)
 
 
 def new_job_args(platform, job_name, namespace):
     logger.info("New %s JobParameters", platform)
     if platform in (PlatformType.KUBERNETES, PlatformType.PY_KUBERNETES):
         return K8sJobArgs(platform, namespace, job_name)
+    elif platform in (PlatformType.RAY):
+        return RayJobArgs(platform, namespace, job_name)
     else:
         raise ValueError("Not support platform %s", platform)
```

## dlrover/python/scheduler/job.py

```diff
@@ -22,18 +22,18 @@
 class ElasticJob(metaclass=ABCMeta):
     def __init__(self, namespace, job_name):
         """
         ElasticJob manages Pods by K8s Python APIs. The example of an elastic
         job is in dlrover/go/elasticjob_operator/config/samples/
         elastic_v1alpha1_elasticjob.yaml
         Args:
-            image_name: Docker image path for ElasticDL pod.
-            namespace: The name of the Kubernetes namespace where ElasticDL
+            image_name: Docker image path for DLRover pod.
+            namespace: The name of the Kubernetes namespace where DLRover
                 pods will be created.
-            job_name: ElasticDL job name, should be unique in the namespace.
+            job_name: DLRover job name, should be unique in the namespace.
                 Used as pod name prefix and value for "elastic" label.
         """
         self._namespace = namespace
         self._job_name = job_name
 
     @abstractmethod
     def get_node_service_addr(self, type, id):
@@ -83,18 +83,18 @@
     def __init__(self, platform, namespace, job_name):
         self.platform = platform
         self.namespace = namespace
         self.job_name = job_name
         self.node_args: Dict[str, NodeArgs] = {}
         self.enable_dynamic_sharding = True
         self.enable_elastic_scheduling = True
-        self.distribution_strategy = DistributionStrategy.PARAMETER_SERVER
+        self.distribution_strategy = DistributionStrategy.PS
         self.job_uuid = ""
         self.user = ""
         self.cluster = ""
-        self.scaling_optimizer = "local"
+        self.optimize_mode = "single-job"
         self.use_ddp = False
         self.resource_limits = ResourceLimits()
 
     @abstractmethod
     def initilize(self):
         pass
```

## dlrover/python/scheduler/kubernetes.py

```diff
@@ -13,15 +13,20 @@
 
 import os
 import threading
 import time
 
 from kubernetes import client, config
 
-from dlrover.python.common.constants import DefaultResourceLimits, NodeType
+from dlrover.python.common.constants import (
+    DefaultResourceLimits,
+    NodeType,
+    OptimizeMode,
+    k8sAPIExceptionReason,
+)
 from dlrover.python.common.log import default_logger as logger
 from dlrover.python.common.node import NodeGroupResource, NodeResource
 from dlrover.python.scheduler.job import ElasticJob, JobArgs, NodeArgs
 
 NODE_SERVICE_PORTS = {
     NodeType.WORKER: 3333,
     NodeType.EVALUATOR: 3333,
@@ -37,27 +42,47 @@
     return s.lower() in ["true", "yes", "t", "y"]
 
 
 def get_pod_name(job_name, pod_type, node_id):
     return "%s-%s" % (job_name + JOB_SUFFIX + pod_type, str(node_id))
 
 
+def retry_k8s_request(func):
+    def wrapper(self, *args, **kwargs):
+        retry = kwargs.get("retry", 5)
+        execption = None
+        for _ in range(retry):
+            try:
+                return func(self, *args, **kwargs)
+            except client.rest.ApiException as e:
+                if e.reason == k8sAPIExceptionReason.NOT_FOUND:
+                    return None
+                execption = e
+                time.sleep(3)
+            except Exception as e:
+                execption = e
+                time.sleep(3)
+        if execption:
+            logger.error("Fail to execute %s: %s", func.__name__, execption)
+            return None
+
+    return wrapper
+
+
 class k8sClient(object):
     _instance_lock = threading.Lock()
 
-    def __init__(self, namespace, job_name):
+    def __init__(self, namespace):
         """
-        ElasticDL k8s client.
+        DLRover k8s client.
 
         Args:
-            image_name: Docker image path for ElasticDL pod.
-            namespace: The name of the Kubernetes namespace where ElasticDL
+            image_name: Docker image path for DLRover pod.
+            namespace: The name of the Kubernetes namespace where DLRover
                 pods will be created.
-            job_name: ElasticDL job name, should be unique in the namespace.
-                Used as pod name prefix and value for "elastic" label.
             event_callback: If not None, an event watcher will be created and
                 events passed to the callback.
             periodic_call_func: If not None, call this method periodically.
         """
         try:
             if os.getenv("KUBERNETES_SERVICE_HOST"):
                 # We are running inside a k8s cluster
@@ -70,119 +95,120 @@
         except Exception as ex:
             logger.error(
                 "Failed to load configuration for Kubernetes:\n%s", ex
             )
 
         self.client = client.CoreV1Api()
         self.api_instance = client.CustomObjectsApi()
+        self.api_client = client.ApiClient()
         self._namespace = namespace
-        self._job_name = job_name
 
+    @retry_k8s_request
     def list_namespaced_pod(self, label_selector):
-        try:
-            pod_list = self.client.list_namespaced_pod(
-                self._namespace,
-                label_selector=label_selector,
-            )
-            return pod_list
-        except Exception as e:
-            logger.warning(e)
-        return None
+        pod_list = self.client.list_namespaced_pod(
+            self._namespace,
+            label_selector=label_selector,
+        )
+        return pod_list
 
+    @retry_k8s_request
     def create_custom_resource(self, group, version, plural, body):
-        try:
-            self.api_instance.create_namespaced_custom_object(
-                group,
-                version,
-                "default",
-                plural,
-                body,
-            )
-        except client.rest.ApiException as e:
-            logger.error(
-                "Exception when calling CustomObjectsApi->",
-                "create_namespaced_custom_object: %s" % e,
-            )
+        self.api_instance.create_namespaced_custom_object(
+            group=group,
+            version=version,
+            namespace=self._namespace,
+            plural=plural,
+            body=body,
+        )
 
-    def get_custom_resource(self, name, group, version, plural):
+    @retry_k8s_request
+    def patch_custom_resource(self, group, version, plural, name, body):
+        self.api_instance.patch_namespaced_custom_object(
+            group=group,
+            version=version,
+            namespace=self._namespace,
+            plural=plural,
+            name=name,
+            body=body,
+        )
+
+    def delete_custom_resource(self, group, version, plural, name):
         try:
-            crd_object = self.api_instance.get_namespaced_custom_object(
-                namespace=self._namespace,
-                name=name,
+            self.api_instance.delete_namespaced_custom_object(
                 group=group,
                 version=version,
+                namespace=self._namespace,
                 plural=plural,
+                name=name,
             )
-            return crd_object
-        except client.ApiException as e:
-            logger.warning("Exception when getting custom object: %s\n" % e)
-            return None
+        except client.rest.ApiException as e:
+            if e.reason != k8sAPIExceptionReason.NOT_FOUND:
+                logger.error("Fail to delete %s", name)
+
+    @retry_k8s_request
+    def get_custom_resource(self, name, group, version, plural):
+        crd_object = self.api_instance.get_namespaced_custom_object(
+            namespace=self._namespace,
+            name=name,
+            group=group,
+            version=version,
+            plural=plural,
+        )
+        return crd_object
 
+    @retry_k8s_request
     def get_configmap(self, name):
-        try:
-            configmap = self.client.read_namespaced_config_map(
-                namespace=self._namespace, name=name
-            )
-            return configmap
-        except client.ApiException as e:
-            logger.warning("Exception when getting configmap: %s\n" % e)
-            return None
+        configmap = self.client.read_namespaced_config_map(
+            namespace=self._namespace, name=name
+        )
+        return configmap
 
     def create_pod(self, pod):
         try:
             self.client.create_namespaced_pod(self._namespace, pod)
             return True
         except client.rest.ApiException as e:
             logger.warning(
                 "Failed to create %s pod: %s\n", pod.metadata.name, e
             )
             return False
 
+    @retry_k8s_request
     def get_pod(self, name):
-        try:
-            return self.client.read_namespaced_pod(
-                namespace=self._namespace, name=name
-            )
-        except client.ApiException as e:
-            logger.warning("Exception when reading pod %s: %s\n" % (name, e))
-            return None
+        return self.client.read_namespaced_pod(
+            namespace=self._namespace, name=name
+        )
 
     def delete_pod(self, name):
         try:
             self.client.delete_namespaced_pod(
                 name,
                 self._namespace,
                 body=client.V1DeleteOptions(),
             )
             return True
-        except Exception as e:
-            logger.warning(e)
+        except client.ApiException as e:
+            if e.reason == k8sAPIExceptionReason.NOT_FOUND:
+                return True
+            logger.warning("Exception when removing pod %s: %s\n" % (name, e))
             return False
 
+    @retry_k8s_request
     def patch_labels_to_pod(self, name, labels_dict):
         body = {"metadata": {"labels": labels_dict}}
-        try:
-            return self.client.patch_namespaced_pod(
-                name=name, namespace=self._namespace, body=body
-            )
-        except client.ApiException as e:
-            logger.warning("Exception when patching labels to pod: %s\n" % e)
-            return None
+        return self.client.patch_namespaced_pod(
+            name=name, namespace=self._namespace, body=body
+        )
 
+    @retry_k8s_request
     def patch_annotations_to_pod(self, name, annotations):
         body = {"metadata": {"annotations": annotations}}
-        try:
-            return self.client.patch_namespaced_pod(
-                name=name, namespace=self._namespace, body=body
-            )
-        except client.ApiException as e:
-            logger.warning(
-                "Exception when patching annotations to pod: %s\n" % e
-            )
-            return None
+        return self.client.patch_namespaced_pod(
+            name=name, namespace=self._namespace, body=body
+        )
 
     def create_service(self, service):
         try:
             self.client.create_namespaced_service(self._namespace, service)
             return True
         except client.rest.ApiException as e:
             logger.warning(
@@ -199,23 +225,20 @@
             return True
         except client.rest.ApiException as e:
             logger.warning(
                 "Failed to patch %s service: %s\n" % (service_name, e)
             )
             return False
 
+    @retry_k8s_request
     def get_service(self, name):
-        try:
-            return self.client.read_namespaced_service(
-                # worker service has the same name as pod name
-                name=name,
-                namespace=self._namespace,
-            )
-        except client.ApiException:
-            return None
+        return self.client.read_namespaced_service(
+            name=name,
+            namespace=self._namespace,
+        )
 
     def create_pvc(self, pvc):
         try:
             self.client.create_namespaced_persistent_volume_claim(
                 self._namespace, pvc
             )
             return True
@@ -230,29 +253,40 @@
     def singleton_instance(cls, *args, **kwargs):
         if not hasattr(k8sClient, "_instance"):
             with k8sClient._instance_lock:
                 if not hasattr(k8sClient, "_instance"):
                     k8sClient._instance = k8sClient(*args, **kwargs)
         return k8sClient._instance
 
+    @classmethod
+    def create_owner_reference(cls, api_version, kind, name, uid):
+        owner_ref = client.V1OwnerReference(
+            api_version=api_version,
+            block_owner_deletion=True,
+            kind=kind,
+            name=name,
+            uid=uid,
+        )
+        return owner_ref
+
 
 class K8sElasticJob(ElasticJob):
     def __init__(self, job_name, namespace):
         """
         ElasticJob manages Pods by K8s Python APIs. The example of an elastic
         job is in dlrover/go/elasticjob_operator/config/samples/
         elastic_v1alpha1_elasticjob.yaml
         Args:
-            image_name: Docker image path for ElasticDL pod.
-            namespace: The name of the Kubernetes namespace where ElasticDL
+            image_name: Docker image path for DLRover pod.
+            namespace: The name of the Kubernetes namespace where DLRover
                 pods will be created.
-            job_name: ElasticDL job name, should be unique in the namespace.
+            job_name: DLRover job name, should be unique in the namespace.
                 Used as pod name prefix and value for "elastic" label.
         """
-        self._k8s_client = k8sClient.singleton_instance(namespace, job_name)
+        self._k8s_client = k8sClient.singleton_instance(namespace)
         self._namespace = namespace
         self._job_name = job_name
 
     def get_node_name(self, type, id):
         return get_pod_name(self._job_name, type, id)
 
     def get_node_service_addr(self, type, id):
@@ -266,39 +300,40 @@
 
 class K8sJobArgs(JobArgs):
     def __init__(self, platform, namespace, job_name):
         super(K8sJobArgs, self).__init__(platform, namespace, job_name)
 
     def initilize(self):
         self.user = os.getenv("USER", "")
-        k8s_client = k8sClient.singleton_instance(
-            self.namespace, self.job_name
-        )
+        k8s_client = k8sClient.singleton_instance(self.namespace)
         job = self._retry_to_get_job(k8s_client)
         self.job_uuid = self._get_job_uuid(job)
         if "distributionStrategy" in job["spec"]:
             self.distribution_strategy = job["spec"]["distributionStrategy"]
         limit_config = job["spec"].get("resourceLimits", {})
-        self.resource_limits.cpu = float(
+        self.resource_limits.cpu = NodeResource.convert_cpu_to_decimal(
             limit_config.get("cpu", DefaultResourceLimits.CPU_LIMIT)
         )
-        self.resource_limits.memory = NodeResource.convert_memory_to_mb(
+        self.resource_limits.memory = NodeResource.convert_memory_to_byte(
             limit_config.get("memory", DefaultResourceLimits.MEMORY_LIMIT)
         )
         self.resource_limits.gpu_num = int(
             limit_config.get("gpu", DefaultResourceLimits.GPU_LIMIT)
         )
+        self.optimize_mode = job["spec"].get(
+            "optimizeMode", OptimizeMode.SINGLE_JOB
+        )
 
         for replica, spec in job["spec"]["replicaSpecs"].items():
             priority = spec.get("priority", "")
             num = int(spec.get("replicas", 0))
             container = spec["template"]["spec"]["containers"][0]
             resources = container.get("resources", {})
             requests = resources.get("requests", {})
-            cpu = float(requests.get("cpu", 0))
+            cpu = NodeResource.convert_cpu_to_decimal(requests.get("cpu", 0))
             if "memory" in requests:
                 memory = NodeResource.convert_memory_to_mb(requests["memory"])
             else:
                 memory = 0
             gpu_type = None
             gpu_num = 0
             for k, v in requests.items():
@@ -306,24 +341,25 @@
                     gpu_type = k
                     gpu_num = int(v)
             group_resource = NodeGroupResource(
                 num,
                 NodeResource(cpu, memory, gpu_type, gpu_num, priority),
             )
             restart_count = int(spec.get("restartCount", 3))
-            auto_scale = parse_bool(spec.get("autoScale", "True"))
+            auto_scale = parse_bool(str(spec.get("autoScale", "true")))
             restart_timeout = int(spec.get("restartTimeout", 0))
             critical_nodes = spec.get("criticalNodes", "")
             self.node_args[replica] = NodeArgs(
                 group_resource,
                 auto_scale,
                 restart_count,
                 restart_timeout,
                 critical_nodes,
             )
+        logger.info("Job args = %s", self.__dict__)
 
     def _retry_to_get_job(self, k8s_client: k8sClient):
         for _ in range(3):
             job = k8s_client.get_custom_resource(
                 name=self.job_name,
                 group="elastic.iml.github.io",
                 version="v1alpha1",
```

## dlrover/python/tests/__init__.py

```diff
@@ -0,0 +1,38 @@
+00000000: 2320 436f 7079 7269 6768 7420 3230 3233  # Copyright 2023
+00000010: 2054 6865 2044 4c52 6f76 6572 2041 7574   The DLRover Aut
+00000020: 686f 7273 2e20 416c 6c20 7269 6768 7473  hors. All rights
+00000030: 2072 6573 6572 7665 642e 0a23 204c 6963   reserved..# Lic
+00000040: 656e 7365 6420 756e 6465 7220 7468 6520  ensed under the 
+00000050: 4170 6163 6865 204c 6963 656e 7365 2c20  Apache License, 
+00000060: 5665 7273 696f 6e20 322e 3020 2874 6865  Version 2.0 (the
+00000070: 2022 4c69 6365 6e73 6522 293b 0a23 2079   "License");.# y
+00000080: 6f75 206d 6179 206e 6f74 2075 7365 2074  ou may not use t
+00000090: 6869 7320 6669 6c65 2065 7863 6570 7420  his file except 
+000000a0: 696e 2063 6f6d 706c 6961 6e63 6520 7769  in compliance wi
+000000b0: 7468 2074 6865 204c 6963 656e 7365 2e0a  th the License..
+000000c0: 2320 596f 7520 6d61 7920 6f62 7461 696e  # You may obtain
+000000d0: 2061 2063 6f70 7920 6f66 2074 6865 204c   a copy of the L
+000000e0: 6963 656e 7365 2061 740a 230a 2320 6874  icense at.#.# ht
+000000f0: 7470 3a2f 2f77 7777 2e61 7061 6368 652e  tp://www.apache.
+00000100: 6f72 672f 6c69 6365 6e73 6573 2f4c 4943  org/licenses/LIC
+00000110: 454e 5345 2d32 2e30 0a23 0a23 2055 6e6c  ENSE-2.0.#.# Unl
+00000120: 6573 7320 7265 7175 6972 6564 2062 7920  ess required by 
+00000130: 6170 706c 6963 6162 6c65 206c 6177 206f  applicable law o
+00000140: 7220 6167 7265 6564 2074 6f20 696e 2077  r agreed to in w
+00000150: 7269 7469 6e67 2c20 736f 6674 7761 7265  riting, software
+00000160: 0a23 2064 6973 7472 6962 7574 6564 2075  .# distributed u
+00000170: 6e64 6572 2074 6865 204c 6963 656e 7365  nder the License
+00000180: 2069 7320 6469 7374 7269 6275 7465 6420   is distributed 
+00000190: 6f6e 2061 6e20 2241 5320 4953 2220 4241  on an "AS IS" BA
+000001a0: 5349 532c 0a23 2057 4954 484f 5554 2057  SIS,.# WITHOUT W
+000001b0: 4152 5241 4e54 4945 5320 4f52 2043 4f4e  ARRANTIES OR CON
+000001c0: 4449 5449 4f4e 5320 4f46 2041 4e59 204b  DITIONS OF ANY K
+000001d0: 494e 442c 2065 6974 6865 7220 6578 7072  IND, either expr
+000001e0: 6573 7320 6f72 2069 6d70 6c69 6564 2e0a  ess or implied..
+000001f0: 2320 5365 6520 7468 6520 4c69 6365 6e73  # See the Licens
+00000200: 6520 666f 7220 7468 6520 7370 6563 6966  e for the specif
+00000210: 6963 206c 616e 6775 6167 6520 676f 7665  ic language gove
+00000220: 726e 696e 6720 7065 726d 6973 7369 6f6e  rning permission
+00000230: 7320 616e 640a 2320 6c69 6d69 7461 7469  s and.# limitati
+00000240: 6f6e 7320 756e 6465 7220 7468 6520 4c69  ons under the Li
+00000250: 6365 6e73 652e 0a                        cense..
```

## dlrover/python/tests/test_dataset_splitter.py

```diff
@@ -102,15 +102,15 @@
             shuffle=False,
         )
         splitter.create_shards()
         shards = splitter.get_shards()
         self.assertEqual(len(shards), 100)
         self.assertEqual(shards[0].start, 0)
         self.assertEqual(shards[0].end, 10)
-        self.assertListEqual(shards[0].record_indices, list(range(10)))
+        self.assertListEqual(shards[0].record_indices, [])
         self.assertEqual(shards[0].name, "test")
         self.assertEqual(splitter.epoch, 1)
 
     def test_create_shards_with_shuffle(self):
         splitter = TextDatasetSplitter(
             dataset_name="test",
             dataset_size=1000,
```

## dlrover/python/tests/test_dataset_task_manager.py

```diff
@@ -17,14 +17,15 @@
 from dlrover.python.master.shard.batch_dataset_manager import (
     BatchDatasetManager,
 )
 from dlrover.python.master.shard.dataset_splitter import (
     PartitionOffsets,
     StreamingDatasetSplitter,
     TableDatasetSplitter,
+    TextDatasetSplitter,
 )
 from dlrover.python.master.shard.streaming_dataset_manager import (
     StreamingDatasetManager,
 )
 
 
 class BatchDatasetTaskMangerTest(unittest.TestCase):
@@ -50,14 +51,57 @@
             task = task_manager.get_task(NodeType.WORKER, worker_id)
             if task.task_id < 0:
                 break
             task_manager.report_task_status(task.task_id, True)
         self.assertTrue(task_manager.completed())
         self.assertEqual(task_manager.get_completed_step(), 1000)
 
+    def test_shard_checkpoint_without_shuffle(self):
+        splitter = TextDatasetSplitter(
+            dataset_name="test",
+            dataset_size=10000,
+            shard_size=100,
+            num_epochs=1,
+        )
+        ds_manager = BatchDatasetManager(TaskType.TRAINING, 10, splitter)
+        worker_id = 0
+        task = ds_manager.get_task(NodeType.WORKER, worker_id)
+        self.assertEqual(task.task_id, 0)
+        self.assertEqual(len(ds_manager.todo), 99)
+        self.assertEqual(len(ds_manager.doing), 1)
+        self.assertFalse(ds_manager.completed())
+        checkpoint = ds_manager.checkpoint()
+        self.assertListEqual(checkpoint.todo[0], [100, 200])
+        ds_manager.restore_checkpoint(checkpoint)
+        self.assertEqual(ds_manager.todo[0].shard.start, 0)
+        self.assertEqual(ds_manager.todo[0].shard.end, 100)
+        self.assertEqual(ds_manager.todo[0].shard.record_indices, None)
+
+    def test_shard_checkpoint_with_shuffle(self):
+        splitter = TextDatasetSplitter(
+            dataset_name="test",
+            dataset_size=10000,
+            shard_size=100,
+            num_epochs=1,
+            shuffle=True,
+        )
+        ds_manager = BatchDatasetManager(TaskType.TRAINING, 10, splitter)
+        worker_id = 0
+        task = ds_manager.get_task(NodeType.WORKER, worker_id)
+        self.assertEqual(task.task_id, 0)
+        self.assertEqual(len(ds_manager.todo), 99)
+        self.assertEqual(len(ds_manager.doing), 1)
+        self.assertFalse(ds_manager.completed())
+        checkpoint = ds_manager.checkpoint()
+        self.assertEqual(len(checkpoint.todo[0][-1]), 100)
+        ds_manager.restore_checkpoint(checkpoint)
+        self.assertEqual(ds_manager.todo[0].shard.start, 0)
+        self.assertEqual(ds_manager.todo[0].shard.end, 100)
+        self.assertEqual(len(ds_manager.todo[0].shard.record_indices), 100)
+
 
 class StreamingDatasetTaskMangerTest(unittest.TestCase):
     def test_create_shards(self):
         partition_offset = PartitionOffsets({0: 1, 1: 0})
         splitter = StreamingDatasetSplitter(
             dataset_name="logstore_test",
             dataset_size=1000,
```

## dlrover/python/tests/test_job_params.py

```diff
@@ -26,16 +26,15 @@
     def test_initialize_params(self):
         mock_k8s_client()
         params = K8sJobArgs(PlatformType.KUBERNETES, "default", "test")
         params.initilize()
         self.assertTrue(NodeType.WORKER in params.node_args)
         self.assertTrue(NodeType.PS in params.node_args)
         self.assertTrue(
-            params.distribution_strategy
-            == DistributionStrategy.PARAMETER_SERVER
+            params.distribution_strategy == DistributionStrategy.PS
         )
         worker_params = params.node_args[NodeType.WORKER]
         self.assertEqual(worker_params.restart_count, 3)
         self.assertEqual(worker_params.restart_timeout, 0)
         self.assertEqual(worker_params.group_resource.count, 0)
         self.assertEqual(worker_params.group_resource.node_resource.cpu, 0)
         self.assertEqual(worker_params.group_resource.node_resource.memory, 0)
```

## dlrover/python/tests/test_local_optimizer.py

```diff
@@ -11,23 +11,23 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 
 from dlrover.python.common.constants import JobOptStage, NodeType
 from dlrover.python.common.node import Node, NodeResource
-from dlrover.python.master.resource.local_optimizer import LocalOptimizer
+from dlrover.python.master.resource.local_optimizer import PSLocalOptimizer
 from dlrover.python.master.stats.training_metrics import RuntimeMetric
 from dlrover.python.scheduler.job import ResourceLimits
 
 
 class LocalOptimizerTest(unittest.TestCase):
     def setUp(self) -> None:
         limits = ResourceLimits(10, 8192)
-        self._optimizer = LocalOptimizer("1111", limits)
+        self._optimizer = PSLocalOptimizer("1111", limits)
         for i in range(10):
             nodes = []
             ps = Node(
                 NodeType.PS,
                 0,
                 config_resource=NodeResource(4, 4096),
                 name="ps-0",
@@ -63,20 +63,20 @@
         )
         self.assertEqual(plan.node_resources[node.name].memory, 8192)
 
     def test_generate_job_create_resource(self):
         plan = self._optimizer._generate_job_create_resource()
         worker = plan.node_group_resources[NodeType.WORKER]
         self.assertEqual(worker.count, 1)
-        self.assertEqual(worker.node_resource.cpu, 1)
-        self.assertEqual(worker.node_resource.memory, 512)
+        self.assertEqual(worker.node_resource.cpu, 2)
+        self.assertEqual(worker.node_resource.memory, 1639)
         ps = plan.node_group_resources[NodeType.PS]
         self.assertEqual(ps.count, 1)
-        self.assertEqual(ps.node_resource.cpu, 1)
-        self.assertEqual(ps.node_resource.memory, 512)
+        self.assertEqual(ps.node_resource.cpu, 2)
+        self.assertEqual(ps.node_resource.memory, 1639)
 
     def test_extract_node_resource(self):
         node_samples = self._optimizer._extract_node_resource()
         self.assertEqual(len(node_samples[NodeType.WORKER]), 5)
         latest_workers = node_samples[NodeType.WORKER][0]
         self.assertEqual(len(latest_workers), 3)
         latest_ps = node_samples[NodeType.PS][0]
@@ -167,7 +167,75 @@
         self._optimizer._resource_limits.cpu = 100
         self._optimizer._resource_limits.memory = 102400
         plan = self._optimizer._generate_worker_resoruce()
         worker_resource = plan.node_group_resources[NodeType.WORKER]
         self.assertEqual(worker_resource.count, 10)
         self.assertEqual(worker_resource.node_resource.cpu, 1.0)
         self.assertEqual(worker_resource.node_resource.memory, 2048 * 1.5)
+
+    def test_compute_worker_speed_ratio(self):
+        for i in range(10, 15):
+            nodes = []
+            ps = Node(
+                NodeType.PS,
+                0,
+                config_resource=NodeResource(4, 4096),
+                name="ps-0",
+            )
+            ps.used_resource = NodeResource(1.0, 2048)
+            nodes.append(ps)
+
+            ps = Node(
+                NodeType.PS,
+                1,
+                config_resource=NodeResource(4, 4096),
+                name="ps-1",
+            )
+            ps.used_resource = NodeResource(0.3, 2048)
+            nodes.append(ps)
+
+            for i in range(3):
+                worker = Node(
+                    NodeType.WORKER, i, config_resource=NodeResource(6, 4096)
+                )
+                worker.used_resource = NodeResource(1, 2048)
+                nodes.append(worker)
+            step = i * 100 + 1
+            ts = i * 1000 + 1
+            m = RuntimeMetric(nodes, global_step=step, speed=12, timestamp=ts)
+            self._optimizer._stats_collector.report_runtime_stats(m)
+        ratio = self._optimizer._compute_worker_speed_ratio()
+        self.assertEqual(ratio, 1)
+
+        for i in range(15, 20):
+            nodes = []
+            ps = Node(
+                NodeType.PS,
+                0,
+                config_resource=NodeResource(4, 4096),
+                name="ps-0",
+            )
+            ps.used_resource = NodeResource(1.0, 2048)
+            nodes.append(ps)
+
+            ps = Node(
+                NodeType.PS,
+                1,
+                config_resource=NodeResource(4, 4096),
+                name="ps-1",
+            )
+            ps.used_resource = NodeResource(0.3, 2048)
+            nodes.append(ps)
+
+            for i in range(4):
+                worker = Node(
+                    NodeType.WORKER, i, config_resource=NodeResource(6, 4096)
+                )
+                worker.used_resource = NodeResource(1, 2048)
+                nodes.append(worker)
+            step = i * 100 + 1
+            ts = i * 1000 + 1
+            m = RuntimeMetric(nodes, global_step=step, speed=15, timestamp=ts)
+            self._optimizer._stats_collector.report_runtime_stats(m)
+
+        ratio = self._optimizer._compute_worker_speed_ratio()
+        self.assertEqual(ratio, 0.75)
```

## dlrover/python/tests/test_master.py

```diff
@@ -12,39 +12,40 @@
 # limitations under the License.
 
 import unittest
 
 from dlrover.python.common.constants import JobExitReason, NodeStatus, NodeType
 from dlrover.python.master.master import Master
 from dlrover.python.master.shard.dataset_splitter import new_dataset_splitter
-from dlrover.python.tests.test_utils import MockJobArgs
+from dlrover.python.tests.test_utils import MockK8sPSJobArgs, mock_k8s_client
 
 
 class MasterTest(unittest.TestCase):
     def setUp(self) -> None:
-        params = MockJobArgs()
+        mock_k8s_client()
+        params = MockK8sPSJobArgs()
         params.initilize()
         self.master = Master(2222, params)
 
     def test_exit_by_workers(self):
-        self.master.node_manager._init_job_nodes()
-        job_nodes = self.master.node_manager._job_nodes
+        self.master.job_manager._init_nodes()
+        job_nodes = self.master.job_manager._job_nodes
         for node in job_nodes[NodeType.WORKER].values():
             node.status = NodeStatus.FINISHED
         for node in job_nodes[NodeType.EVALUATOR].values():
             node.status = NodeStatus.FINISHED
         for node in job_nodes[NodeType.CHIEF].values():
             node.status = NodeStatus.FINISHED
         self.master.run()
         self.assertEqual(self.master._exit_code, 0)
         self.assertEqual(self.master._exit_reason, JobExitReason.SUCCEEDED)
 
     def test_exit_by_tasks(self):
-        self.master.node_manager._init_job_nodes()
-        job_nodes = self.master.node_manager._job_nodes
+        self.master.job_manager._init_nodes()
+        job_nodes = self.master.job_manager._job_nodes
         for node in job_nodes[NodeType.PS].values():
             node.status = NodeStatus.FINISHED
         for node in job_nodes[NodeType.EVALUATOR].values():
             node.status = NodeStatus.FINISHED
         for node in job_nodes[NodeType.CHIEF].values():
             node.status = NodeStatus.FINISHED
```

## dlrover/python/tests/test_pod_scaler.py

```diff
@@ -9,73 +9,85 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 
-from dlrover.python.common.constants import DistributionStrategy, NodeType
+from dlrover.python.common.constants import (
+    DistributionStrategy,
+    ElasticJobLabel,
+    NodeType,
+)
 from dlrover.python.common.node import Node, NodeGroupResource, NodeResource
 from dlrover.python.master.scaler.base_scaler import ScalePlan
-from dlrover.python.master.scaler.pod_scaler import PodScaler
+from dlrover.python.master.scaler.pod_scaler import PodScaler, new_tf_config
 from dlrover.python.tests.test_utils import mock_k8s_client
 
 
+def new_service_fn(node_type, node_id):
+    return str(node_type) + "_" + str(node_id)
+
+
 class PodScalerTest(unittest.TestCase):
     def setUp(self) -> None:
         mock_k8s_client()
 
     def test_init_pod_template(self):
         scaler = PodScaler("elasticjob-sample", "default")
         self.assertEqual(
             scaler._distribution_strategy,
-            DistributionStrategy.PARAMETER_SERVER,
+            DistributionStrategy.PS,
         )
-        worker_template = scaler._replica_template[NodeType.WORKER]
+        worker_pod = scaler._replica_template[NodeType.WORKER]
+        main_container = worker_pod.spec.containers[0]
         self.assertEqual(
-            worker_template.image, "dlrover/elasticjob:iris_estimator"
+            main_container.image, "dlrover/elasticjob:iris_estimator"
         )
-        self.assertEqual(worker_template.restart_policy, "Never")
+        self.assertEqual(worker_pod.spec.restart_policy, "Never")
         self.assertListEqual(
-            worker_template.command,
+            main_container.command,
             [
                 "python",
                 "-m",
                 "model_zoo.iris.dnn_estimator",
                 "--batch_size=32",
                 "--training_steps=1000",
             ],
         )
 
     def test_create_pod(self):
         scaler = PodScaler("elasticjob-sample", "default")
-        scaler._distribution_strategy = DistributionStrategy.PARAMETER_SERVER
+        scaler._distribution_strategy = DistributionStrategy.PS
         resource = NodeResource(4, 8192)
         node = Node(NodeType.WORKER, 0, resource, rank_index=0)
         pod_stats = {
             NodeType.WORKER: 3,
             NodeType.CHIEF: 1,
             NodeType.PS: 2,
         }
         ps_addrs = [
             "elasticjob-sample-edljob-ps-0",
             "elasticjob-sample-edljob-ps-1",
         ]
+        scaler._config_worker_num = 2
         pod = scaler._create_pod(node, pod_stats, ps_addrs)
         self.assertEqual(
             pod.metadata.name, "elasticjob-sample-edljob-worker-0"
         )
         main_container = pod.spec.containers[0]
         self.assertEqual(main_container.resources.limits["cpu"], 4)
         self.assertEqual(main_container.resources.limits["memory"], "8192Mi")
         self.assertEqual(main_container.env[-1].name, "TF_CONFIG")
         self.assertTrue(
             """{"type": "worker", "index": 0}"""
             in main_container.env[-1].value
         )
+        self.assertEqual(main_container.env[5].name, "WORKER_NUM")
+        self.assertEqual(main_container.env[5].value, "2")
         node = Node(NodeType.CHIEF, 0, resource, rank_index=0)
         pod = scaler._create_pod(node, pod_stats, ps_addrs)
         main_container = pod.spec.containers[0]
         self.assertTrue(
             """{"type": "chief", "index": 0}""" in main_container.env[-1].value
         )
 
@@ -91,36 +103,45 @@
         main_container = pod.spec.containers[0]
         self.assertEqual(len(pod.spec.volumes), 1)
         self.assertEqual(pod.spec.volumes[0].name, "pvc-nas")
         self.assertEqual(len(main_container.volume_mounts), 1)
 
     def test_create_service(self):
         scaler = PodScaler("elasticjob-sample", "default")
-        service = scaler._create_service(
-            NodeType.WORKER, 0, "elasticjob-sample-edljob-worker-0"
+        service = scaler._create_service_obj(
+            name="elasticjob-sample-edljob-worker-0",
+            port="2222",
+            target_port="2222",
+            replica_type=NodeType.WORKER,
+            rank_index=0,
+        )
+        self.assertEqual(
+            service.spec.selector[ElasticJobLabel.RANK_INDEX_KEY], "0"
+        )
+        self.assertEqual(
+            service.spec.selector[ElasticJobLabel.REPLICA_TYPE_KEY], "worker"
         )
-        self.assertEqual(service.spec.selector["replica-index"], "0")
-        self.assertEqual(service.spec.selector["replica-type"], "worker")
 
     def test_scale(self):
         scaler = PodScaler("elasticjob-sample", "default")
-        scaler._distribution_strategy = DistributionStrategy.PARAMETER_SERVER
+        scaler._distribution_strategy = DistributionStrategy.PS
         resource = NodeResource(4, 8192)
         scale_plan = ScalePlan()
+        self.assertTrue(scale_plan.empty())
         scale_plan.node_group_resources = {
             NodeType.WORKER: NodeGroupResource(5, resource),
             NodeType.CHIEF: NodeGroupResource(1, resource),
             NodeType.PS: NodeGroupResource(2, resource),
         }
         scaler.scale(scale_plan)
-        self.assertEqual(len(scaler._initial_nodes), 3)
+        self.assertEqual(len(scaler._create_node_queue), 3)
 
         worker_ids = []
         chief_ids = []
-        for node in scaler._initial_nodes:
+        for node in scaler._create_node_queue:
             if node.type == NodeType.WORKER:
                 worker_ids.append(node.id)
             elif node.type == NodeType.CHIEF:
                 chief_ids.append(node.id)
         self.assertListEqual(chief_ids, [0])
         self.assertListEqual(worker_ids, [3, 4])
 
@@ -129,8 +150,42 @@
             NodeType.CHIEF: NodeGroupResource(1, resource),
             NodeType.PS: NodeGroupResource(2, resource),
         }
         scale_plan.launch_nodes.append(
             Node(NodeType.WORKER, 1, NodeResource(0, 0))
         )
         scaler.scale(scale_plan)
-        self.assertEqual(len(scaler._initial_nodes), 2)
+        self.assertFalse(scale_plan.empty())
+        self.assertEqual(len(scaler._create_node_queue), 2)
+
+    def test_new_tf_config(self):
+        pod_stats = {NodeType.WORKER: 1}
+
+        tf_config = new_tf_config(
+            pod_stats, new_service_fn, NodeType.WORKER, 0, []
+        )
+        self.assertDictEqual(
+            tf_config,
+            {
+                "cluster": {"ps": [], "worker": ["worker_0"]},
+                "task": {"type": "worker", "index": 0},
+            },
+        )
+
+    def test_scale_up_pods(self):
+        scaler = PodScaler("elasticjob-sample", "default")
+        scaler._distribution_strategy = DistributionStrategy.PS
+        resource = NodeResource(4, 8192)
+        scale_plan = ScalePlan()
+        self.assertTrue(scale_plan.empty())
+        scale_plan.node_group_resources = {
+            NodeType.WORKER: NodeGroupResource(5, resource),
+            NodeType.CHIEF: NodeGroupResource(1, resource),
+            NodeType.PS: NodeGroupResource(2, resource),
+        }
+        cur_nodes = [Node(NodeType.WORKER, 1, rank_index=0)]
+        scaler._scale_up_pods(NodeType.WORKER, scale_plan, cur_nodes, 1)
+        self.assertEqual(len(scaler._create_node_queue), 4)
+        self.assertEqual(
+            scaler._create_node_queue[0].service_addr,
+            "elasticjob-sample-edljob-worker-1.default.svc:3333",
+        )
```

## dlrover/python/tests/test_ps_manager.py

```diff
@@ -93,15 +93,15 @@
         for node in ps_manager._nodes.values():
             node.status = NodeStatus.RUNNING
         ps_manager._scale_down_ps(1)
         self.assertEqual(len(ps_manager._pre_dropped_ps), 1)
         self.assertEqual(ps_manager._pre_dropped_ps[0].id, 1)
 
         plan = ps_manager.process_after_ps_cluster_ready()
-        self.assertListEqual(plan.remove_nodes, ["test-edljob-ps-1"])
+        self.assertEqual(plan.remove_nodes[0].name, "test-edljob-ps-1")
 
     def test_delete_running_ps(self):
         job_nodes = self._job_resource.init_job_node_meta(
             1,
             self._elastic_job.get_node_service_addr,
             self._elastic_job.get_node_name,
         )
@@ -150,7 +150,38 @@
         self.assertEqual(len(ps_manager._pre_dropped_ps), 1)
 
         training_ps = ps_manager.get_next_training_ps_cluster()
         self.assertEqual(len(training_ps), 2)
         self.assertEqual(
             training_ps[0].service_addr, "test-edljob-ps-2.default.svc:2222"
         )
+
+    def test_parameter_server_failure(self):
+        job_nodes = self._job_resource.init_job_node_meta(
+            1,
+            self._elastic_job.get_node_service_addr,
+            self._elastic_job.get_node_name,
+        )
+        ps_manager = ParameterServerManager(
+            job_nodes[NodeType.PS],
+            self._job_resource,
+            3,
+            self._elastic_job.get_node_service_addr,
+            self._elastic_job.get_node_name,
+        )
+        for node in ps_manager._nodes.values():
+            node.status = NodeStatus.RUNNING
+        ps_failure = ps_manager.has_ps_failure()
+        self.assertFalse(ps_failure)
+        latest_ps_index = len(ps_manager._nodes) - 1
+        ps = ps_manager._nodes[latest_ps_index]
+        ps_manager._ps_cluster_changed = True
+        ps.status = NodeStatus.INITIAL
+        ps.init_time -= 600
+        ps_failure = ps_manager.has_ps_failure()
+        self.assertTrue(ps_failure)
+        cluster = ps_manager.get_next_training_ps_cluster()
+        self.assertEqual(len(cluster), 1)
+        self.assertEqual(
+            cluster[0].service_addr,
+            "test-edljob-ps-0.default.svc:2222",
+        )
```

## dlrover/python/tests/test_resource_optimizer.py

```diff
@@ -8,26 +8,33 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
+from unittest import mock
 
 from dlrover.proto import brain_pb2
-from dlrover.python.brain.client import build_easydl_client
-from dlrover.python.common.constants import NodeResourceLimit, NodeType
+from dlrover.python.brain.client import build_brain_client
+from dlrover.python.common.constants import (
+    MemoryUnit,
+    NodeResourceLimit,
+    NodeType,
+    OptimizeMode,
+)
 from dlrover.python.common.global_context import Context
 from dlrover.python.common.node import Node, NodeGroupResource, NodeResource
 from dlrover.python.master.resource.brain_optimizer import (
     BrainResoureOptimizer,
 )
 from dlrover.python.master.resource.job import (
+    AllreduceJobResourceOptimizer,
     JobResource,
-    JobResourceOptimizer,
+    PSJobResourceOptimizer,
     ResourceLimits,
 )
 from dlrover.python.master.resource.optimizer import ResourcePlan
 
 _dlrover_context = Context.singleton_instance()
 _MEMORY = 8192
 
@@ -37,28 +44,28 @@
         res = brain_pb2.OptimizeResponse()
         res.job_optimize_plans.add()
         group_resources = res.job_optimize_plans[
             0
         ].resource.task_group_resources
         group_resources[NodeType.WORKER].count = 5
         group_resources[NodeType.WORKER].resource.memory = (
-            _MEMORY * 1024 * 1024
+            _MEMORY * MemoryUnit.MB
         )
         group_resources[NodeType.WORKER].resource.cpu = 16
 
         group_resources[NodeType.PS].count = 2
-        group_resources[NodeType.PS].resource.memory = _MEMORY * 1024 * 1024
+        group_resources[NodeType.PS].resource.memory = _MEMORY * MemoryUnit.MB
         group_resources[NodeType.PS].resource.cpu = 16
         return res
 
 
 class ResourceOptimizerTest(unittest.TestCase):
     def test_brain_optimizer(self):
         optimizer = BrainResoureOptimizer("1111", ResourceLimits(100, 102400))
-        optimizer._brain_client = build_easydl_client()
+        optimizer._brain_client = build_brain_client()
         optimizer._brain_client._brain_stub = MockStub()
         plan: ResourcePlan = optimizer.generate_opt_plan("", {})
         worker = plan.node_group_resources[NodeType.WORKER]
         self.assertEqual(worker.count, 5)
         self.assertEqual(worker.node_resource.cpu, 16)
         self.assertEqual(worker.node_resource.memory, _MEMORY)
 
@@ -89,28 +96,31 @@
 
         ps = plan.node_group_resources[NodeType.PS]
         self.assertEqual(ps.count, 1)
         self.assertEqual(ps.node_resource.cpu, NodeResourceLimit.MAX_CPU_CORES)
         self.assertEqual(ps.node_resource.memory, NodeResourceLimit.MAX_MEMORY)
 
 
-class JobResourceOptimizerTest(unittest.TestCase):
+class PSJobResourceOptimizerTest(unittest.TestCase):
     def setUp(self):
-        self._client = build_easydl_client()
+        self._client = build_brain_client()
         self._client._brain_stub = MockStub()
         worker_resource = NodeGroupResource(
             0,
             NodeResource(0, 0),
         )
         ps_resource = NodeGroupResource(
             0,
             NodeResource(0, 0),
         )
-        self._job_optimizer = JobResourceOptimizer(
-            worker_resource, ps_resource, "brain", "aa0_uuid"
+        self._job_optimizer = PSJobResourceOptimizer(
+            worker_resource, ps_resource, OptimizeMode.CLUSTER, "aa0_uuid"
+        )
+        self._job_optimizer._resource_optimizer = BrainResoureOptimizer(
+            "1111", ResourceLimits(100, 102400)
         )
         resource_optimizer = self._job_optimizer._resource_optimizer
         resource_optimizer._brain_client = self._client
         _dlrover_context.auto_ps_enabled = True
         _dlrover_context.auto_worker_enabled = True
 
     def test_fixed_resource(self):
@@ -118,16 +128,19 @@
             1,
             NodeResource(0, 1024),
         )
         ps_resource = NodeGroupResource(
             1,
             NodeResource(4, 1024),
         )
-        self._job_optimizer = JobResourceOptimizer(
-            worker_resource, ps_resource, "brain", "aa0_uuid"
+        self._job_optimizer = PSJobResourceOptimizer(
+            worker_resource, ps_resource, OptimizeMode.CLUSTER, "aa0_uuid"
+        )
+        self._job_optimizer._resource_optimizer = BrainResoureOptimizer(
+            "1111", ResourceLimits(100, 102400)
         )
         resource_optimizer = self._job_optimizer._resource_optimizer
         resource_optimizer._brain_client = self._client
         self._job_optimizer._init_job_resource_by_optimizer()
         worker = self._job_optimizer._worker_resource
         self.assertEqual(
             worker.node_resource.memory,
@@ -150,19 +163,14 @@
         self.assertEqual(worker.node_resource.cpu, 16)
         self.assertEqual(worker.count, 5)
         ps = self._job_optimizer._ps_resource
         self.assertEqual(ps.node_resource.memory, _MEMORY)
         self.assertEqual(ps.node_resource.cpu, 16)
         self.assertEqual(ps.count, 2)
 
-    def test_optimize_worker_resource(self):
-        self._job_optimizer.optimize_worker_resource()
-        worker = self._job_optimizer._worker_resource
-        self.assertEqual(worker.node_resource.memory, _MEMORY)
-
     def test_init_job_resource(self):
         job = JobResource()
         job.node_group_resources[NodeType.PS] = NodeGroupResource(
             3, NodeResource(1, 256, priority="high")
         )
         job.node_group_resources[NodeType.WORKER] = NodeGroupResource(
             0, NodeResource(1, 256, priority="high")
@@ -181,34 +189,64 @@
         self.assertEqual(evaluator.node_resource.memory, _MEMORY)
         self.assertEqual(evaluator.node_resource.cpu, 16)
 
         ps = job.get_node_group_resource(NodeType.PS)
         self.assertEqual(ps.node_resource.memory, _MEMORY)
         self.assertEqual(ps.node_resource.cpu, 16)
 
-    def test_update_worker_resource_from_easydl(self):
+    def test_update_worker_resource_from_brain(self):
         worker_resource = NodeGroupResource(5, NodeResource(0, 0))
         ps_resource = NodeGroupResource(0, NodeResource(0, 0))
-        job_optimizer = JobResourceOptimizer(
-            worker_resource, ps_resource, "brain", "aa0_uuid"
+        job_optimizer = PSJobResourceOptimizer(
+            worker_resource, ps_resource, OptimizeMode.CLUSTER, "aa0_uuid"
+        )
+        job_optimizer._resource_optimizer = BrainResoureOptimizer(
+            "1111", ResourceLimits(100, 102400)
         )
         job_optimizer._resource_optimizer._brain_client = self._client
         job_optimizer._init_job_resource_by_optimizer()
         worker = job_optimizer._worker_resource
         self.assertEqual(worker.count, 5)
         self.assertEqual(worker.node_resource.memory, _MEMORY)
         self.assertEqual(worker.node_resource.cpu, 16)
 
     def test_adjust_oom_ps_resource(self):
         worker_resource = NodeGroupResource(10, NodeResource(1, 256))
         ps_resource = NodeGroupResource(3, NodeResource(2, 1024))
-        job_optimizer = JobResourceOptimizer(
-            worker_resource, ps_resource, "brain", "aa0_uuid"
+        job_optimizer = PSJobResourceOptimizer(
+            worker_resource, ps_resource, OptimizeMode.CLUSTER, "aa0_uuid"
+        )
+        job_optimizer._resource_optimizer = BrainResoureOptimizer(
+            "1111", ResourceLimits(100, 102400)
         )
 
         job_optimizer._resource_optimizer._brain_client = self._client
         oom_ps = Node(
             "ps", 0, name="ps-0", config_resource=NodeResource(2, 1024)
         )
 
-        job_optimizer.adjust_oom_ps_resource(oom_ps)
+        job_optimizer._adjust_oom_ps_resource(oom_ps)
         self.assertEqual(oom_ps.config_resource.memory, 8192)
+
+
+class AllreduceResourceOptimizerTest(unittest.TestCase):
+    def test_free_node_plan(self):
+        worker_resource = NodeGroupResource(8, NodeResource(1, 256))
+        self._optimizer = AllreduceJobResourceOptimizer(
+            worker_resource, "test-job"
+        )
+        self._optimizer.set_alive_node_num(4)
+        self._optimizer.set_node_unit(4)
+        self._optimizer._get_free_gpu_node = mock.MagicMock(return_value=4)
+        plan: ResourcePlan = self._optimizer.get_job_resource_plan()
+        worker_plan = plan.node_group_resources[NodeType.WORKER]
+        self.assertEqual(worker_plan.count, 8)
+
+        self._optimizer._get_free_gpu_node = mock.MagicMock(return_value=3)
+        plan: ResourcePlan = self._optimizer.get_job_resource_plan()
+        worker_plan = plan.node_group_resources[NodeType.WORKER]
+        self.assertEqual(worker_plan.count, 4)
+
+        self._optimizer.set_node_unit(1)
+        plan: ResourcePlan = self._optimizer.get_job_resource_plan()
+        worker_plan = plan.node_group_resources[NodeType.WORKER]
+        self.assertEqual(worker_plan.count, 7)
```

## dlrover/python/tests/test_servicer.py

```diff
@@ -16,41 +16,60 @@
 
 from google.protobuf import empty_pb2
 
 from dlrover.proto import elastic_training_pb2
 from dlrover.python.common.constants import NodeStatus, NodeType
 from dlrover.python.master.elastic_training.elastic_ps import ElasticPsService
 from dlrover.python.master.monitor.speed_monitor import SpeedMonitor
-from dlrover.python.master.node.node_manager import create_node_manager
+from dlrover.python.master.node.job_manager import create_job_manager
 from dlrover.python.master.servicer import MasterServicer
 from dlrover.python.master.shard.task_manager import TaskManager
 from dlrover.python.master.stats.job_collector import JobMetricCollector
-from dlrover.python.tests.test_utils import MockJobArgs
+from dlrover.python.tests.test_utils import (
+    MockK8sPSJobArgs,
+    MockRayJobArgs,
+    mock_k8s_client,
+)
+from dlrover.python.util.queue.queue import RayEventQueue
+
+ray_event_queue = RayEventQueue.singleton_instance()
 
 
 class MasterServicerTest(unittest.TestCase):
     def setUp(self) -> None:
-        params = MockJobArgs()
+        mock_k8s_client()
+        params = MockK8sPSJobArgs()
         params.initilize()
+        worker_resource = params.node_args[NodeType.WORKER].group_resource
+        worker_resource.node_resource.gpu_num = 1
+        worker_resource.node_resource.gpu_type = "a100"
         speed_monitor = SpeedMonitor()
         self.task_manager = TaskManager(False, speed_monitor)
-        self.node_manager = create_node_manager(params, speed_monitor)
+        self.job_manager = create_job_manager(params, speed_monitor)
+        self.job_manager._init_nodes()
         self.job_metric_collector = JobMetricCollector(
             "1", "default", "local", "dlrover"
         )
         self.elastic_ps_service = ElasticPsService()
         self.servicer = MasterServicer(
             task_manager=self.task_manager,
-            node_manager=self.node_manager,
+            job_manager=self.job_manager,
             speed_monitor=speed_monitor,
-            rendezvous_server=None,
+            rdzv_managers={},
             job_metric_collector=self.job_metric_collector,
             elastic_ps_service=self.elastic_ps_service,
         )
 
+    def test_query_running_nodes(self):
+        req = empty_pb2.Empty()
+        workers = self.job_manager._job_nodes[NodeType.WORKER]
+        workers[0].status = NodeStatus.RUNNING
+        res = self.servicer.query_running_nodes(req, None)
+        self.assertEqual(len(res.nodes), 1)
+
     def test_dataset_service(self):
         request = elastic_training_pb2.ReportDatasetShardParamsRequest()
         request.batch_size = 10
         request.num_epochs = 1
         request.dataset_size = 1000
         request.shuffle = False
         request.num_minibatches_per_shard = 10
@@ -83,15 +102,16 @@
         self.assertLessEqual(10, len(checkpoint.content))
         self.servicer.report_shard_checkpoint(checkpoint, None)
 
         res = self.servicer.get_dataset_epoch(request, None)
         self.assertEqual(res.epoch, 1)
 
     def test_metric_service(self):
-        self.node_manager._init_job_nodes()
+        self.job_manager._init_nodes()
+        self.job_manager._init_job_auto_scaler()
         request = elastic_training_pb2.ReportUsedResourceRequest()
         request.memory = 4096
         request.cpu = 2
         request.node_id = 0
         request.node_type = NodeType.WORKER
         self.servicer.report_used_resource(request, None)
         request.node_type = NodeType.PS
@@ -104,31 +124,32 @@
         request.op_stats.op_count = 100
         request.op_stats.flops = 10000
         self.servicer.report_model_metric(request, None)
         reporter = self.job_metric_collector._stats_reporter
         reporter._runtime_stats = []
         self.assertEqual(reporter._model_metric.op_stats.flops, 10000)
 
-        worker0 = self.node_manager._job_nodes[NodeType.WORKER][0]
+        worker0 = self.job_manager._job_nodes[NodeType.WORKER][0]
         worker0.status = NodeStatus.RUNNING
-        ps0 = self.node_manager._job_nodes[NodeType.PS][0]
+        ps0 = self.job_manager._job_nodes[NodeType.PS][0]
         ps0.status = NodeStatus.RUNNING
         request = elastic_training_pb2.GlobalStepRecord()
         self.task_manager._speed_monitor.add_running_worker(NodeType.WORKER, 0)
+        self.task_manager._speed_monitor.set_target_worker_num(1)
         ts = int(time.time())
         request.timestamp = ts
         request.global_step = 100
         self.servicer.report_global_step(request, None)
         request.timestamp = ts + 10
         request.global_step = 1100
         self.servicer.report_global_step(request, None)
         self.job_metric_collector._report_runtime_stats()
         self.assertEqual(len(reporter._runtime_stats), 2)
         self.assertEqual(reporter._runtime_stats[0].global_step, 1100)
-        self.assertEqual(len(reporter._runtime_stats[0].running_nodes), 4)
+        self.assertEqual(len(reporter._runtime_stats[0].running_nodes), 2)
 
         request.timestamp = ts + 20
         request.global_step = 2100
         self.servicer.report_global_step(request, None)
 
         request.timestamp = ts + 30
         request.global_step = 3100
@@ -141,15 +162,67 @@
         request.timestamp = ts + 50
         request.global_step = 5100
         self.servicer.report_global_step(request, None)
         self.assertTrue(self.servicer._start_autoscale)
 
     def test_query_ps_nodes(self):
         request = empty_pb2.Empty()
-        self.node_manager._init_job_nodes()
-        for node in self.node_manager._job_nodes[NodeType.PS].values():
+        self.job_manager._init_nodes()
+        for node in self.job_manager._job_nodes[NodeType.PS].values():
             node.status = NodeStatus.RUNNING
         res = self.servicer.query_ps_nodes(request, None)
         self.assertEqual(len(res.ps_nodes), 3)
         self.assertEqual(
             res.ps_nodes[0].addr, "test-edljob-ps-0.default.svc:2222"
         )
+
+
+class MasterServicerForRayTest(unittest.TestCase):
+    def setUp(self) -> None:
+        params = MockRayJobArgs()
+        params.initilize()
+        speed_monitor = SpeedMonitor()
+        self.task_manager = TaskManager(False, speed_monitor)
+        self.job_manager = create_job_manager(params, speed_monitor)
+        self.job_metric_collector = JobMetricCollector(
+            "1", "default", "local", "dlrover"
+        )
+        self.elastic_ps_service = ElasticPsService()
+        self.servicer = MasterServicer(
+            task_manager=self.task_manager,
+            job_manager=self.job_manager,
+            speed_monitor=speed_monitor,
+            rdzv_managers={},
+            job_metric_collector=self.job_metric_collector,
+            elastic_ps_service=self.elastic_ps_service,
+        )
+
+    def test_update_node_addr(self):
+        request = elastic_training_pb2.NodeMeta()
+        task_id = 1
+        task_type = NodeType.PS
+        addr = "localhost:5001"
+        request.type = task_type
+        request.id = task_id
+        request.addr = "localhost:5001"
+        self.job_manager._init_nodes()
+        self.servicer.update_node_status(request, None)
+        self.assertEqual(
+            self.job_manager._job_nodes[task_type][task_id].service_addr, addr
+        )
+        for node in self.job_manager._job_nodes[NodeType.PS].values():
+            node.status = NodeStatus.RUNNING
+        res = self.servicer.query_ps_nodes(request, None)
+        self.assertEqual(addr, res.ps_nodes[task_id].addr)
+        self.assertEqual("", res.ps_nodes[0].addr)
+
+    def test_update_node_event(self):
+        request = elastic_training_pb2.NodeEvent()
+        task_id = 1
+        task_type = NodeType.PS
+        request.node.type = task_type
+        request.node.id = task_id
+        request.event_type = "Deleted"
+        request.message = "OOM"
+        self.servicer.update_node_event(request, None)
+        event = ray_event_queue.get()
+        event.event_type = "OOM"
```

## dlrover/python/tests/test_sharding_client.py

```diff
@@ -10,18 +10,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 
 from dlrover.python.elastic_agent.master_client import LocalDataset
-from dlrover.python.elastic_agent.sharding.client import ShardingClient
+from dlrover.python.elastic_agent.sharding.client import (
+    IndexShardingClient,
+    ShardingClient,
+)
 
 
-class DataShardServiceTest(unittest.TestCase):
+class DataShardClientTest(unittest.TestCase):
     def test_local_dataset(self):
         dataset = LocalDataset(
             batch_size=16,
             num_epochs=2,
             dataset_size=100,
             shuffle=False,
             num_minibatches_per_shard=2,
@@ -39,19 +42,39 @@
             dataset_size=100,
             num_minibatches_per_shard=2,
             dataset_name="test",
         )
         shard = data_shard_service.fetch_shard()
         self.assertEqual(shard.start, 0)
         self.assertEqual(shard.end, 32)
-        self.assertEqual(data_shard_service.get_current_epoch(), 1)
+        self.assertEqual(data_shard_service.get_current_epoch(), 0)
         shard_count = 1
         while True:
             shard = data_shard_service.fetch_shard()
             if not shard:
                 break
             shard_count += 1
         self.assertEqual(shard_count, 8)
 
 
+class IndexShardingClientTest(unittest.TestCase):
+    def test_sharding_client(self):
+        client = IndexShardingClient(
+            batch_size=16,
+            num_epochs=2,
+            dataset_size=100,
+            num_minibatches_per_shard=2,
+            dataset_name="test",
+        )
+        index = client.fetch_sample_index()
+        self.assertEqual(index, 0)
+        sample_count = 1
+        while True:
+            index = client.fetch_sample_index()
+            if not index:
+                break
+            sample_count += 1
+        self.assertEqual(sample_count, 100)
+
+
 if __name__ == "__main__":
     unittest.main()
```

## dlrover/python/tests/test_speed_monitor.py

```diff
@@ -7,28 +7,37 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import time
 import unittest
 
 from dlrover.python.common.constants import NodeType
 from dlrover.python.master.monitor.speed_monitor import SpeedMonitor
 
 
 class SpeedMonitorTest(unittest.TestCase):
-    def test_speed_monitor(self):
+    def test_monitor_running_workers(self):
         monitor = SpeedMonitor()
         monitor.set_target_worker_num(2)
         monitor.add_running_worker(NodeType.WORKER, 0)
         monitor.add_running_worker(NodeType.WORKER, 1)
         monitor.collect_global_step(1, 1)
         monitor.collect_global_step(301, 11),
         monitor.collect_global_step(9001, 301),
         self.assertEqual(monitor.completed_global_step, 9001)
         self.assertTrue(monitor.worker_adjustment_finished())
         self.assertEqual(monitor.running_speed, 30)
         monitor.remove_running_worker(NodeType.WORKER, 1)
         monitor.collect_global_step(18001, 601)
         self.assertFalse(monitor.worker_adjustment_finished())
+
+    def test_monitor_eval_time(self):
+        monitor = SpeedMonitor()
+        monitor.set_worker_start_eval_time(0)
+        time.sleep(0.1)
+        monitor.update_worker_eval_time(0)
+        eval_time = monitor.get_worker_eval_time(0)
+        self.assertTrue(eval_time > 0.1)
```

## dlrover/python/tests/test_stats_collector.py

```diff
@@ -11,38 +11,67 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import time
 import unittest
 
 from dlrover.python.common.constants import NodeType
+from dlrover.python.common.node import Node, NodeResource
 from dlrover.python.master.monitor.speed_monitor import SpeedMonitor
 from dlrover.python.master.stats.job_collector import JobMetricCollector
 from dlrover.python.master.stats.reporter import JobMeta, LocalStatsReporter
 from dlrover.python.master.stats.training_metrics import RuntimeMetric
-from dlrover.python.master.watcher.base_watcher import Node
 
 
 class LocalStatsCollectorTest(unittest.TestCase):
     def test_report_resource_usage(self):
         job_meta = JobMeta("1111")
         reporter = LocalStatsReporter(job_meta)
         reporter._runtime_stats = []
-        reporter.report_runtime_stats(RuntimeMetric([]))
-        reporter.report_runtime_stats(RuntimeMetric([]))
-        self.assertEqual(len(reporter._runtime_stats), 2)
+        ps = Node(
+            NodeType.PS,
+            0,
+            config_resource=NodeResource(4, 4096),
+            name="ps-0",
+        )
+        worker = Node(
+            NodeType.WORKER, 0, config_resource=NodeResource(6, 4096)
+        )
+        worker.used_resource = NodeResource(1, 2048)
+        ps.used_resource = NodeResource(1.0, 2048)
+        for i in range(3):
+            nodes = [ps]
+            for i in range(3):
+                nodes.append(worker)
+            step = i * 100 + 1
+            ts = i * 1000 + 1
+            m = RuntimeMetric(nodes, global_step=step, speed=12, timestamp=ts)
+            reporter.report_runtime_stats(m)
+        self.assertEqual(len(reporter._runtime_stats), 3)
+
+        for i in range(10):
+            nodes = [ps]
+            for i in range(4):
+                worker.used_resource = NodeResource(1, 2048)
+                nodes.append(worker)
+            step = i * 100 + 1
+            ts = i * 1000 + 1
+            m = RuntimeMetric(nodes, global_step=step, speed=12, timestamp=ts)
+            reporter.report_runtime_stats(m)
+        self.assertEqual(len(reporter._runtime_stats), 8)
 
 
 class StatsCollectorTest(unittest.TestCase):
     def test_job_metric_collector(self):
         collector = JobMetricCollector("1111", "default", "local", "dlrover")
         collector.collect_dataset_metric("test", 1000)
 
         speed_monitor = SpeedMonitor()
         t = int(time.time())
+        speed_monitor.set_target_worker_num(1)
         speed_monitor.collect_global_step(100, t)
         speed_monitor.collect_global_step(1100, t + 10)
         speed_monitor.add_running_worker(NodeType.WORKER, 0)
         worker = Node(NodeType.WORKER, 0, None)
         collector._stats_reporter._runtime_stats = []
         collector.collect_runtime_stats(speed_monitor, [worker])
         self.assertEqual(len(collector._runtime_metric.running_nodes), 1)
```

## dlrover/python/tests/test_task_manager.py

```diff
@@ -93,7 +93,15 @@
 
         dataset = task_manager.get_dataset(dataset_name)
         task_manager.get_dataset_task(NodeType.WORKER, 0, dataset_name)
         self.assertEqual(len(dataset.todo), 7)
         task_manager.restore_dataset_from_checkpoint(checkpoint_str)
         self.assertEqual(dataset.todo[1].shard.start, 100)
         self.assertEqual(len(dataset.todo), 10)
+
+    def test_task_hang(self):
+        task_manager = create_task_manager()
+        dataset_name = "test"
+        dataset = task_manager.get_dataset(dataset_name)
+        dataset._latest_task_end_time = 3600
+        hang = task_manager.task_hanged()
+        self.assertTrue(hang)
```

## dlrover/python/tests/test_utils.py

```diff
@@ -15,27 +15,35 @@
 from unittest import mock
 
 import yaml
 from kubernetes import client
 
 from dlrover.proto import elastic_training_pb2
 from dlrover.python.common.constants import (
+    DistributionStrategy,
     ElasticJobLabel,
     NodeStatus,
     NodeType,
     PlatformType,
 )
 from dlrover.python.common.node import NodeGroupResource, NodeResource
 from dlrover.python.master.monitor.speed_monitor import SpeedMonitor
 from dlrover.python.master.shard.dataset_splitter import new_dataset_splitter
 from dlrover.python.master.shard.task_manager import TaskManager
 from dlrover.python.scheduler.job import JobArgs, NodeArgs
 from dlrover.python.scheduler.kubernetes import k8sClient
 
 
+def get_test_scale_plan(*args, **kwargs):
+    with open("dlrover/python/tests/data/scaleplan_sample.yaml", "r") as f:
+        job_content = f.read()
+    job = yaml.safe_load(job_content)
+    return job
+
+
 def _get_training_job(*args, **kwargs):
     with open("dlrover/python/tests/data/elasticjob_sample.yaml", "r") as f:
         job_content = f.read()
     job = yaml.safe_load(job_content)
     return job
 
 
@@ -50,17 +58,17 @@
             namespace="default",
             uid="111",
         ),
     )
     return pod
 
 
-class MockJobArgs(JobArgs):
+class MockK8sPSJobArgs(JobArgs):
     def __init__(self):
-        super(MockJobArgs, self).__init__(
+        super(MockK8sPSJobArgs, self).__init__(
             PlatformType.KUBERNETES, "default", "test"
         )
 
     def initilize(self):
         worker_resource = NodeGroupResource(3, NodeResource(1, 4096))
         self.node_args[NodeType.WORKER] = NodeArgs(
             worker_resource, True, 3, 0, ""
@@ -75,14 +83,59 @@
         )
 
         chief_resource = NodeGroupResource(1, NodeResource(1, 4096))
         self.node_args[NodeType.CHIEF] = NodeArgs(
             chief_resource, True, 1, 0, ""
         )
         self.job_uuid = "11111"
+        self.distribution_strategy = DistributionStrategy.PS
+
+
+class MockK8sAllreduceJobArgs(JobArgs):
+    def __init__(self):
+        super(MockK8sAllreduceJobArgs, self).__init__(
+            PlatformType.KUBERNETES, "default", "test"
+        )
+
+    def initilize(self):
+        worker_resource = NodeGroupResource(
+            16, NodeResource(1, 4096, "a100", 8)
+        )
+        self.node_args[NodeType.WORKER] = NodeArgs(
+            worker_resource, True, 3, 0, ""
+        )
+        self.job_uuid = "11111"
+        self.distribution_strategy = DistributionStrategy.ALLREDUCE
+
+
+class MockRayJobArgs(JobArgs):
+    def __init__(self):
+        super(MockRayJobArgs, self).__init__(
+            PlatformType.RAY, "default", "test"
+        )
+
+    def initilize(self):
+        worker_resource = NodeGroupResource(3, NodeResource(1, 4096))
+        self.node_args[NodeType.WORKER] = NodeArgs(
+            worker_resource, True, 3, 0, ""
+        )
+
+        ps_resource = NodeGroupResource(3, NodeResource(1, 4096))
+        self.node_args[NodeType.PS] = NodeArgs(ps_resource, True, 1, 0, "all")
+
+        evaluator_resource = NodeGroupResource(1, NodeResource(1, 4096))
+        self.node_args[NodeType.EVALUATOR] = NodeArgs(
+            evaluator_resource, False, 1, 0, ""
+        )
+
+        chief_resource = NodeGroupResource(1, NodeResource(1, 4096))
+        self.node_args[NodeType.CHIEF] = NodeArgs(
+            chief_resource, True, 1, 0, ""
+        )
+        self.job_uuid = "11111"
 
 
 def create_pod(labels):
     status = client.V1PodStatus(
         container_statuses=[
             client.V1ContainerStatus(
                 image="test",
@@ -156,17 +209,16 @@
         pod = create_pod(labels)
         pods.append(pod)
     return client.V1PodList(
         items=pods, metadata=client.V1ListMeta(resource_version="12345678")
     )
 
 
-def create_task_manager():
+def create_task_manager(dataset_name="test"):
     task_manager = TaskManager(False, SpeedMonitor())
-    dataset_name = "test"
     splitter = new_dataset_splitter(
         False,
         100,
         1000,
         1,
         dataset_name,
         "table",
@@ -178,18 +230,21 @@
         dataset_splitter=splitter,
         task_type=elastic_training_pb2.TRAINING,
     )
     return task_manager
 
 
 def mock_k8s_client():
-    k8s_client = k8sClient.singleton_instance("default", "elasticjob-sample")
+    k8s_client = k8sClient.singleton_instance("default")
     k8s_client.get_custom_resource = _get_training_job  # type: ignore
     k8s_client.get_pod = _get_pod  # type: ignore
     k8s_client.list_namespaced_pod = mock_list_namespaced_pod  # type: ignore
     k8s_client.create_custom_resource = mock.MagicMock(  # type: ignore
         return_value=True
     )
+    k8s_client.delete_custom_resource = mock.MagicMock(  # type: ignore
+        return_value=True
+    )
     k8s_client.create_pod = mock.MagicMock(return_value=True)  # type: ignore
     k8s_client.create_service = mock.MagicMock(  # type: ignore
         return_value=True
     )
```

## dlrover/python/tests/test_worker_manager.py

```diff
@@ -10,17 +10,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 from datetime import datetime, timedelta
 
-from dlrover.python.common.constants import NodeStatus, NodeType, PlatformType
-from dlrover.python.common.node import NodeGroupResource, NodeResource
-from dlrover.python.master.node.worker import WorkerManager
+from dlrover.python.common.constants import (
+    NodeExitReason,
+    NodeStatus,
+    NodeType,
+    PlatformType,
+)
+from dlrover.python.common.node import Node, NodeGroupResource, NodeResource
+from dlrover.python.master.node.worker import ChiefManager, WorkerManager
 from dlrover.python.master.resource.job import JobResource
 from dlrover.python.scheduler.factory import new_elastic_job
 from dlrover.python.tests.test_utils import mock_k8s_client
 
 
 class WorkerManagerTest(unittest.TestCase):
     def setUp(self) -> None:
@@ -61,25 +66,27 @@
         self.assertEqual(len(released_workers), 2)
 
     def test_delete_exited_workers(self):
         self._worker_manager._nodes[3].status = NodeStatus.FINISHED
         self._worker_manager._nodes[4].status = NodeStatus.FAILED
 
         plan = self._worker_manager.delete_exited_workers()
+        node_names = [node.name for node in plan.remove_nodes]
         self.assertListEqual(
-            plan.remove_nodes,
+            node_names,
             ["test-edljob-worker-3", "test-edljob-worker-4"],
         )
 
     def test_delete_running_workers(self):
         for node in self._worker_manager._nodes.values():
             node.status = NodeStatus.RUNNING
         plan = self._worker_manager.delete_running_workers()
+        node_names = [node.name for node in plan.remove_nodes]
         self.assertListEqual(
-            plan.remove_nodes,
+            node_names,
             [
                 "test-edljob-worker-0",
                 "test-edljob-worker-1",
                 "test-edljob-worker-2",
                 "test-edljob-worker-3",
                 "test-edljob-worker-4",
             ],
@@ -95,20 +102,64 @@
         )
         plan = worker_manager.relaunch_node(
             self._job_nodes[NodeType.WORKER][4]
         )
         self.assertEqual(plan.launch_nodes[0].config_resource.cpu, 16)
         self.assertEqual(worker_manager._nodes[5].id, 5)
 
+    def test_relaunch_chief_node(self):
+        tf_master_node = Node(
+            NodeType.MASTER,
+            node_id=0,
+            config_resource=NodeResource(cpu=16, memory=10240),
+        )
+        manager = ChiefManager(
+            {0: tf_master_node},
+            self._job_resource,
+            3,
+            self._elastic_job.get_node_service_addr,
+            self._elastic_job.get_node_name,
+        )
+        plan = manager.relaunch_node(tf_master_node)
+        self.assertEqual(plan.launch_nodes[0].config_resource.cpu, 16)
+        self.assertEqual(manager._nodes[1].id, 1)
+
     def test_cut_pending_node_cpu(self):
         worker_manager = WorkerManager(
             self._job_nodes[NodeType.WORKER],
             self._job_resource,
             3,
             self._elastic_job.get_node_service_addr,
             self._elastic_job.get_node_name,
         )
         for node in worker_manager._nodes.values():
             node.status = NodeStatus.PENDING
             node.create_time = datetime.now() + timedelta(days=-1)
         plan = worker_manager.cut_pending_node_cpu()
         self.assertEqual(len(plan.launch_nodes), 5)
+
+    def test_pending_without_workers(self):
+        worker_manager = WorkerManager(
+            self._job_nodes[NodeType.WORKER],
+            self._job_resource,
+            3,
+            self._elastic_job.get_node_service_addr,
+            self._elastic_job.get_node_name,
+        )
+        for node in worker_manager._nodes.values():
+            node.status = NodeStatus.FAILED
+            node.exit_reason = NodeExitReason.FATAL_ERROR
+        failed = worker_manager.has_failed_worker()
+        self.assertTrue(failed)
+
+        for node in worker_manager._nodes.values():
+            node.exit_reason = NodeExitReason.KILLED
+        failed = worker_manager.has_failed_worker()
+        self.assertFalse(failed)
+
+        wait = worker_manager.wait_worker_restart()
+        self.assertTrue(wait)
+        for node in worker_manager._nodes.values():
+            node.relaunch_count = node.max_relaunch_count
+
+        wait = worker_manager.wait_worker_restart()
+        self.assertFalse(wait)
```

## dlrover/trainer/constants/platform_constants.py

```diff
@@ -17,8 +17,9 @@
 class PlatformConstants(object):
     """Platform related constants"""
 
     PlatformName = Constant("Platform")
     ExecutePlaform = Constant("ExecutePlaform")
     Local = Constant("LOCAL", "LOCAL")
     Kubernetes = Constant("KUBERNETES", "KUBERNETES")
+    Ray = Constant("RAY", "RAY")
     WorkerActionRun = Constant("run", "run")
```

## dlrover/trainer/constants/tf_constants.py

```diff
@@ -60,7 +60,20 @@
     ANY_NODE_FO_LEVEL = Constant(1)
     EstimatorTrainingChiefHooks = Constant("training_chief_hooks")
     EstimatorTrainingHooks = Constant("training_hooks")
     EstimatorPredictionHooks = Constant("prediction_hooks")
     EstimatorEvaluationHooks = Constant("evaluation_hooks")
     EnableAutoScaling = Constant("enable_auto_scaling")
     EnableDynamicSharding = Constant("enable_dynamic_sharding", True)
+    EnableIncrSavedModel = Constant("enable_incr_saved_model", False)
+    RelaunchForPs = Constant("relaunch_for_ps", False)
+    RelaunchForFailure = Constant("relaunch_for_failure", False)
+    SaveCheckpoint = Constant("save_checkpoint_for_ps", False)
+    CheckpointIncrementalSaveSecs = Constant(
+        "checkpoint_incremental_save_secs", None
+    )
+    KeepCheckpointMax = Constant("keep_checkpoint_max", 5)
+    DataShardClient = Constant("data_shard_client", None)
+    ExitRecoverableSession = Constant("exit_recoverable_session", None)
+    DataShardCheckpoint = Constant(
+        "data_shard_checkpoint", "data_shard_checkpoint.json"
+    )
```

## dlrover/trainer/mock/tf_process_scheduler.py

```diff
@@ -19,15 +19,49 @@
 import sys
 
 from dlrover.trainer.mock.base_process_scheduler import BaseProcessScheduler
 from dlrover.trainer.util.log_util import default_logger as logger
 from dlrover.trainer.util.net_util import get_available_port
 
 
-def start_subprocess(tf_config):
+def mock_ray_platform_subprocess(tf_config):
+    """
+    start process using subprocess
+    """
+    argv = sys.argv
+    task_type = tf_config["task"]["type"]
+    task_id = tf_config["task"]["index"]
+    worker_argv = [sys.executable, "-m", "dlrover.trainer.entry.local_entry"]
+
+    worker_argv.extend(argv[1:])
+    worker_argv.extend(["--platform", "ray"])
+    worker_argv.extend(["--mock", "True"])
+    worker_argv.extend(["--task_type", task_type])
+    worker_argv.extend(["--task_id", str(task_id)])
+
+    logger.info(worker_argv)
+    env = dict(os.environ)
+    fild_path = os.path.dirname(__file__)
+    fild_path = fild_path.split("/")
+    python_path = "/".join(fild_path[: len(fild_path) - 3])
+    logger.info(python_path)
+    env.update(
+        {
+            "PYTHONPATH": python_path,
+        }
+    )
+
+    logger.info(json.dumps(tf_config))
+    env["WORKFLOW_ID"] = os.getenv("WORKFLOW_ID", default="test_id")
+    env["USERNUMBER"] = os.getenv("USERNUMBER", default="test_user")
+    process = subprocess.Popen(worker_argv, shell=False, env=env)
+    return process
+
+
+def mock_k8s_platform_subprocess(tf_config):
     """
     start process using subprocess
     """
     argv = sys.argv
     worker_argv = [sys.executable, "-m", "dlrover.trainer.entry.local_entry"]
     worker_argv.extend(argv[1:])
     worker_argv.extend(["--platform", "kubernetes"])
@@ -62,14 +96,18 @@
         super(TFProcessScheduler, self).__init__()
         assert worker_num >= 1, "worker number should be as least 1"
         assert evaluator_num <= 1, "evaluator number should be as most 1"
         self.ps_num = ps_num
         self.chief_num = 1
         self.worker_num = worker_num - 1
         self.evaluator_num = evaluator_num
+        self.start_subprocess = None
+
+    def set_start_subprocess(self, start_subprocess):
+        self.start_subprocess = start_subprocess
 
     def prepare_cluster(self):
         """
         get available ports for ps/worker/evaluator
         """
         ps_ports = [get_available_port() for i in range(self.ps_num)]
         worker_ports = [get_available_port() for i in range(self.worker_num)]
@@ -87,15 +125,15 @@
         if self.evaluator_num == 1:
             cluster_info.update({"evaluator": evaluator_ports})
         self.tf_cluster_spec = {"cluster": cluster_info}
 
     def update_spec_and_start_process(self, task_spec):
         tf_cluster_spec = copy.deepcopy(self.tf_cluster_spec)
         tf_cluster_spec.update(task_spec)
-        p = start_subprocess(tf_cluster_spec)
+        p = self.start_subprocess(tf_cluster_spec)
         return p
 
     def start_chief_process(self):
         chief_task_spec = {
             "task": {
                 "type": "chief",
                 "index": 0,
@@ -143,19 +181,18 @@
             }
             p = self.update_spec_and_start_process(evaluator_task_spec)
             evaluator_process.append(p)
         return evaluator_process
 
     def run_process(self):
         self.prepare_cluster()
-        chief_process = self.start_chief_process()
         ps_process = self.start_ps_process()
+        chief_process = self.start_chief_process()
         evaluator_process = self.start_evaluator_process()
         worker_process = self.start_worker_process()
-
         self.all_processes = {
             "chief_process": chief_process,
             "ps_process": ps_process,
             "worker_process": worker_process,
             "evaluator_process": evaluator_process,
         }
         all_process = list(itertools.chain(*self.all_processes.values()))
```

## dlrover/trainer/platform/starter.py

```diff
@@ -8,21 +8,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
+import traceback
 
 from dlrover import trainer
 from dlrover.trainer.constants.platform_constants import PlatformConstants
-from dlrover.trainer.mock.tf_process_scheduler import TFProcessScheduler
+from dlrover.trainer.mock.tf_process_scheduler import (
+    TFProcessScheduler,
+    mock_k8s_platform_subprocess,
+    mock_ray_platform_subprocess,
+)
 from dlrover.trainer.util.args_util import get_parsed_args
 from dlrover.trainer.util.log_util import default_logger as logger
 from dlrover.trainer.worker.tf_kubernetes_worker import TFKubernetesWorker
+from dlrover.trainer.worker.tf_ray_worker import TFRayWorker
 
 
 def print_info(append_detail=False):
     """Print dlrover_trainer information"""
     dlrover_trainer = os.path.dirname(trainer.__file__)
     file_path = os.path.join(dlrover_trainer, "COMMIT_INFO")
     if not os.path.exists(file_path):
@@ -44,24 +50,35 @@
 
 
 def execute(args):
     """run routine"""
     platform = args.platform.upper()
     if platform == PlatformConstants.Kubernetes():
         worker = TFKubernetesWorker(args)
-    elif platform in [PlatformConstants.Local()]:
+    if platform == PlatformConstants.Ray():
+        worker = TFRayWorker(args)
+    elif PlatformConstants.Local() in platform:
         # local mode, actually we use a scheduler
         logger.info("create ProcessScheduler with run_type = ProcessScheduler")
         worker = TFProcessScheduler(
             ps_num=args.ps_num,
             worker_num=args.worker_num,
             evaluator_num=args.evaluator_num,
             conf=args.conf,
             parsed_args=args,
         )
+        # to do use constants
+
+        if PlatformConstants.Ray() in platform:
+            worker.set_start_subprocess(mock_ray_platform_subprocess)
+        elif PlatformConstants.Kubernetes() in platform:
+            worker.set_start_subprocess(mock_k8s_platform_subprocess)
+        else:
+            detail_trace_back = traceback.format_exc()
+            logger.error(detail_trace_back)
 
     logger.info(
         "Running platform: %s, worker action: %s",
         args.platform,
         args.worker_action,
     )
     if args.worker_action == PlatformConstants.WorkerActionRun():
```

## dlrover/trainer/tensorflow/__init__.py

```diff
@@ -6,7 +6,8 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from dlrover.trainer.tensorflow.reader import *  # noqa: F401,F403
```

## dlrover/trainer/tensorflow/executor/base_executor.py

```diff
@@ -9,20 +9,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import os
+import socket
 
 import tensorflow.compat.v1 as tf
 from tensorflow.core.protobuf import cluster_pb2
 from tensorflow.python.training import server_lib
 
 from dlrover.trainer.constants.tf_constants import TFConstants
+from dlrover.trainer.tensorflow.util.tf_env_util import (
+    get_tf_config,
+    get_tf_config_task_type_and_index,
+)
 from dlrover.trainer.util.log_util import default_logger as logger
 
 tf.disable_v2_behavior()
 
 
 class BaseExecutor:
     """BaseExecutor is a wrapper for tensorflow model.
@@ -31,41 +36,34 @@
     """
 
     def __init__(self):
         self.cluster_spec = None
         self.mini_cluster_spec = None
         self.task_id = None
         self.task_type = None
-        self.address = None
-        self.role = None
+        self.address: str = ""
+        self.role: str = ""
 
     def get_tf_config_from_env(self):
-        tf_config = json.loads(os.environ.get("TF_CONFIG") or "{}")
-        if not tf_config:
-            logger.error(
-                "TF_CONFIG should not be empty in distributed environment."
-            )
-            raise Exception(
-                "TF_CONFIG should not be empty in distributed environment."
-            )
-        return tf_config
+        return get_tf_config()
+
+    def get_cluster_info_by_master(self):
+        pass
 
     def get_cluster_info_by_tf_config(self):
         """
         get cluster info by TF_CONFIG
         {"cluster": {
                         "ps": ["web04-pod2.default.svc:5002"],
                         "chief": ["web04-pod1.default.svc:5000"]
                     },
          "task": {"type": "ps", "index": 0}}'
         """
-
         tf_config = self.get_tf_config_from_env()
-        task_type = tf_config["task"]["type"]
-        task_id = tf_config["task"]["index"]
+        task_type, task_id = get_tf_config_task_type_and_index()
         self.task_type = task_type
         self.task_id = task_id
         self.role = task_type + ":" + str(task_id)
         self.cluster_spec = tf_config["cluster"]
         self.address = tf_config["cluster"][task_type][task_id]
         logger.info(
             "cluster spec is {} \
@@ -114,22 +112,35 @@
             mini_cluster_spec["chief"] = worker_hosts
         else:
             mini_cluster_spec["worker"] = worker_hosts
         self.mini_cluster_spec = mini_cluster_spec
         logger.info("cluster def is:\n %s", cluster_def)
         return cluster_def
 
+    def address_initiated(self):
+        return self.address != ""
+
     def start_server(self):
         """start tensorflow server not using cluster spec."""
         if self.task_type != TFConstants.Evaluator():
-            logger.info("starting server")
-            self.server = server_lib.Server(
-                {"localhost": [self.address]}, protocol="grpc"
-            )
-            self.server.start()
+            logger.info("starting server {}".format(self.address))
+            logger.info(self.address_initiated())
+            if self.address_initiated():
+                self.server = server_lib.Server(
+                    {"localhost": [self.address]}, protocol="grpc"
+                )
+                self.server.start()
+            else:
+                self.server = server_lib.Server.create_local_server()
+                # grpc address 'grpc://localhost:37229'
+                grpc_address = self.server.target
+                hostname = socket.gethostname()
+                ip = socket.gethostbyname(hostname)
+                # ip + ":" + port,  "172.17.0.3" + ":" + "37229"
+                self.address = ip + ":" + grpc_address.split(":")[-1]
 
     def get_config(self, cluster_spec):
         """build session config and estimator.RunConfig"""
         config = tf.estimator.RunConfig()
         tf_config = os.environ["TF_CONFIG"]
         tf_config = json.loads(tf_config)
         # we set the tf_config["environment"] = "google" and _is_google_env() is True,   # noqa: E501
@@ -155,15 +166,15 @@
         logger.info("mini cluster spec is {}".format(self.mini_cluster_spec))
         config._cluster_spec = server_lib.ClusterSpec(self.mini_cluster_spec)
         config._task_id = self.task_id
         if self.task_type == TFConstants.Worker():
             config._task_id = self.task_id + 1
         config._task_type = self.task_type
         if self.task_type == TFConstants.Chief():
-            config._task_type = "chief"
+            config._task_type = TFConstants.Chief()
         config._num_ps_replicas = len(
             self.mini_cluster_spec.get(TFConstants.PS(), {})
         )
         config._num_worker_replicas = 1
         config._master = "grpc://" + self.address
         config._protocol = "grpc"
         config._log_step_count_steps = 10
```

## dlrover/trainer/tensorflow/executor/estimator_executor.py

```diff
@@ -7,34 +7,41 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import json
 import os
+import time
 
 import tensorflow as tf
 from tensorflow.python.estimator.exporter import BestExporter
 from tensorflow.python.ops import array_ops
 from tensorflow.python.training.basic_session_run_hooks import (
     CheckpointSaverHook,
 )
+from tensorflow_estimator.python.estimator.estimator import Estimator
 
 from dlrover.trainer.constants.tf_constants import TFConstants
 from dlrover.trainer.tensorflow.executor.base_executor import BaseExecutor
 from dlrover.trainer.tensorflow.hooks.elastic_data_shard_report_hook import (
     ElasticDataShardReportHook,
 )
 from dlrover.trainer.tensorflow.hooks.global_step_hook import GlobalStepHook
+from dlrover.trainer.tensorflow.util import common_util
 from dlrover.trainer.tensorflow.util.data_mapping_util import data_mapping
 from dlrover.trainer.tensorflow.util.dataset_util import DatasetUtil
 from dlrover.trainer.tensorflow.util.estimator_util import (
+    ck_after_run,
     hook_estimator_call_model_fn,
 )
+from dlrover.trainer.tensorflow.util.tf_patch_util import export_saved_model
+from dlrover.trainer.tensorflow.util.tf_version_util import is_tf_115
 from dlrover.trainer.util.log_util import default_logger as logger
 from dlrover.trainer.util.reflect_util import get_class
 
 try:
     from dlrover.python.elastic_agent.tensorflow.hooks import (
         ReportModelMetricHook,
     )
@@ -53,26 +60,42 @@
         """
         Args:
             context_from_storage: We saved the `context` value in storage and
                                 passed the storage-key as the `context`
         """
 
         super(EstimatorExecutor, self).__init__()
-        self.get_cluster_info_by_tf_config()
         self._task_conf = context
+
+    def wait_for_tf_config(self):
+        while os.environ.get("TF_CONFIG", None) is None:
+            time.sleep(1)
+
+    def set_tf_config(self, tf_config):
+        if not isinstance(tf_config, str):
+            tf_config = json.dumps(tf_config)
+        os.environ["TF_CONFIG"] = tf_config
+        self.prepare()
+
+    def prepare(self):
+
+        self.get_cluster_info_by_tf_config()
         self._initialize_estimator_related()
         self._prepare_env()
-        # prepare estimator class from user
-        self.gen_model_dir()
+
         self._prepare_estimator_class()
         self._prepare_estimator()
+        self._prepare_incr_saved_model_checkpoint()
 
     def gen_model_dir(self):
         self._model_dir = self._task_conf.get(TFConstants.ModelDir.name)
-        if not os.path.exists(self._model_dir):
+        if (
+            not os.path.exists(self._model_dir)
+            and self.task_type == TFConstants.Chief()
+        ):
             os.makedirs(self._model_dir)
 
     def _initialize_estimator_related(self):
         pass
 
     def _prepare_env(self):
         pass
@@ -126,48 +149,70 @@
         self._tf_estimator = self._classifier_class(
             self._model_dir, config, params
         )
 
     def _prepare_estimator_config_and_params(self):
         """prepare estimator.RunConfig and set default estimator hooks"""
         config = self.get_config(self.cluster_spec)
+        self.gen_model_dir()
         config._model_dir = self._model_dir
+        config._keep_checkpoint_max = self._task_conf.get(
+            TFConstants.KeepCheckpointMax.name, TFConstants.KeepCheckpointMax()
+        )
         params = {}
         training_hooks = [GlobalStepHook()]
         data_shard_client = self.train_dataset.reader.data_shard_client
+
         if data_shard_client is not None:
+            global_dict = common_util.GlobalDict()
+            global_dict[TFConstants.DataShardClient.name] = data_shard_client
             logger.info("appending ElasticDataShardReportHook")
             shard_report_hook = ElasticDataShardReportHook(data_shard_client)
             model_metric_report_hook = ReportModelMetricHook()
             training_hooks.append(shard_report_hook)
             training_hooks.append(model_metric_report_hook)
+
         params[TFConstants.EstimatorTrainingHooks.name] = training_hooks
 
         save_steps = self._task_conf.get(
             TFConstants.SaveSteps.name, TFConstants.SaveSteps()
         )
         save_secs = self._task_conf.get(
             TFConstants.SaveSecs.name, TFConstants.SaveSecs()
         )
         logger.info("checkpoint hook %s", self._model_dir)
-        params[TFConstants.EstimatorTrainingChiefHooks.name] = [
-            CheckpointSaverHook(
-                self._model_dir, save_steps=save_steps, save_secs=save_secs
+        checkpoint_save_hook = CheckpointSaverHook(
+            self._model_dir, save_steps=save_steps, save_secs=save_secs
+        )
+        checkpoint_incremental_save_secs = self._task_conf.get(
+            TFConstants.CheckpointIncrementalSaveSecs.name, None
+        )
+        if is_tf_115() and checkpoint_incremental_save_secs:
+            CheckpointSaverHook.after_run = ck_after_run
+            checkpoint_save_hook = CheckpointSaverHook(
+                self._model_dir,
+                save_steps=save_steps,
+                save_secs=save_secs,
+                incremental_save_secs=checkpoint_incremental_save_secs,
             )
+
+        params[TFConstants.EstimatorTrainingChiefHooks.name] = [
+            checkpoint_save_hook
         ]
         train_set = self._task_conf.get(TFConstants.TrainSet.name)
         params["columns"] = train_set.columns
         hook_estimator_call_model_fn(params)
         user_params = {}
         logger.info("config is {}".format(config))
         return config, user_params
 
     def _prepare_train_dataset(self):
         """prepare_train_dataset"""
         train_set = self._task_conf.get(TFConstants.TrainSet.name)
+        logger.info("Prepare training dataset with {}".format(train_set))
         self.train_dataset = DatasetUtil.create(train_set)
 
     def _prepare_eval_dataset(self):
         """prepare_eval_datasets"""
         eval_set = self._task_conf.get(TFConstants.EvalSet.name)
         self.eval_dataset = DatasetUtil.create(eval_set)
 
@@ -217,14 +262,19 @@
             input_fn=self._eval_input_fn,
             steps=eval_steps,
             throttle_secs=10,
             start_delay_secs=5,
             exporters=[exporter],
         )
 
+    def _prepare_incr_saved_model_checkpoint(self):
+        # check whether tf is deeprec
+        if is_tf_115():
+            Estimator.export_saved_model = export_saved_model
+
     def train_and_evaluate(self):
         logger.info("starting train and evaluate")
         try:
             tf.estimator.train_and_evaluate(
                 self._tf_estimator, self._train_spec, self._eval_spec
             )
         except tf.errors.OutOfRangeError:
```

## dlrover/trainer/tensorflow/failover/failover_client.py

```diff
@@ -62,19 +62,16 @@
         logger.info("successfully set ps global version: %s.", version)
 
     def set_local_version(self, version=0):
         self._client.update_local_cluster_version(version)
         logger.info("successfully set local version: %s.", version)
 
     def get_training_ps_addr(self):
-        logger.info("get training ps addresses")
-        ps_nodes, new_ps_ready = self._client.get_all_ps_nodes()
-        logger.info("ps_nodes is %s", ps_nodes)
-        logger.info("new_ps_ready is %s", new_ps_ready)
-        return [n.addr for n in ps_nodes]
+        ps_nodes, ps_failure = self._client.get_all_ps_nodes()
+        return [n.addr for n in ps_nodes], ps_failure
 
     def init_version(self, version=0):
         logger.info("initiating local and global version")
         local_version = self.get_local_version()
         global_version = self.get_global_version()
         if local_version == 0 and self.task_type == TFConstants.PS():
             version = local_version + 1
```

## dlrover/trainer/tensorflow/failover/tensorflow_failover.py

```diff
@@ -15,151 +15,143 @@
 
 # coding: utf-8
 
 import json
 import os
 import threading
 import time
-from typing import List
 
 from dlrover.trainer.constants.tf_constants import TFConstants
 from dlrover.trainer.tensorflow.failover.failover_client import FailoverClient
 from dlrover.trainer.tensorflow.util import common_util
-from dlrover.trainer.tensorflow.util.tf_patch_util import hotpatch_for_dynet
+from dlrover.trainer.tensorflow.util.tf_env_util import (
+    get_tf_config,
+    get_tf_config_task_type_and_index,
+)
 from dlrover.trainer.util.log_util import default_logger as logger
 
 
 class TensorflowFailover:
-    def __init__(self, role=None, failover_level=1):
+    def __init__(self, failover_client=FailoverClient, failover_level=1):
         """
         Args:
             role: "ps:0", "worker:1"
             uuid_key: unique key that marks this cluster
             failover_level: switch for dynet
         """
-        self._role = role
         logger.info(
             "initiating tensorflow_failover and failover level is {}".format(
                 failover_level
             )
         )
         self._failover_level = failover_level
-        hotpatch_for_dynet(failover_level)
         if common_util.should_failover(self._failover_level):
-            self.init_for_dynet_from_tf_config()
-        logger.info(
-            "TensorflowFailover: role: %s, failover_level: %s,  ",
-            role,
-            failover_level,
-        )
-
-    def init_for_dynet_from_tf_config(self):
-
-        tf_config = json.loads(os.environ.get("TF_CONFIG") or "{}")
-        if not tf_config:
-            logger.error(
-                "TF_CONFIG should not be empty in distributed environment."
-            )
-            raise Exception(
-                "TF_CONFIG should not be empty in distributed environment."
-            )
-        task_type = tf_config["task"]["type"]
-        task_id = tf_config["task"]["index"]
+            self.init_for_dynet()
+            self._failover_client = failover_client(role=self._role)
+            self._failover_client.init_version()
+
+    def init_for_dynet(self):
+        TF_CONFIG = get_tf_config()
+        logger.info("TF_CONFIG is {}".format(TF_CONFIG))
+        task_type, task_id = get_tf_config_task_type_and_index()
         self._role = task_type + ":" + str(task_id)
-        self._address = tf_config["cluster"][task_type][task_id]
+        if len(TF_CONFIG["cluster"][task_type]) > 1:
+            self._address = TF_CONFIG["cluster"][task_type][task_id]
+        else:
+            self._address = TF_CONFIG["cluster"][task_type][0]
+        if self._role is None:
+            return
         self.task_type, self.task_id = self._role.split(":")
         self.task_id = int(self.task_id)
-        self._failover_client = FailoverClient(role=self._role)
-        self._is_chief = (
-            self.task_type == TFConstants.Chief.name and self.task_id == 0
-        )
-        self.prev_address = tf_config["cluster"]["ps"]
-        self._failover_client.init_version()
+        self._is_chief = self.task_type == "chief" and self.task_id == 0
+        self.curr_ps_address = TF_CONFIG["cluster"]["ps"]
+        logger.info("Initial ps address is %s" % self.curr_ps_address)
 
     def start_failover_monitor(self):
-        if self._role and TFConstants.Evaluator.name not in self._role:
-            self._start_for_ps_migration()
-
-    def _start_for_ps_migration(self):
-        """
-        Listening for ps address in the training cluster.
-        If ps address changes, it means that dlrover master is
-        going to migrate ps. When found ps address changes, it
-        doesn't neede to restart worker and reconstuct graph.
-        Only cluster info in session config and estimator.RunConfig
-        needs to be refreshed. By building session with new config
-        instead of restarting worker,
-        """
+        if self._role and self.task_type not in ["evaluator", "ps"]:
+            self._start_failover_monitor()
 
+    def _start_failover_monitor(self):
         def monitor_fun():
-            logger.info("Successfully to start monitor ps address!")
+            logger.info("Successfully to start failover monitor!")
             while True:
-                logger.info("Checking whether ps address changes")
-                curr_address = self._failover_client.get_training_ps_addr()
-                refresh_session = False
-                logger.info(
-                    "prev address is {} and current address is {}".format(
-                        self.prev_address, curr_address
-                    )
-                )
-                if "".join(curr_address) != "".join(self.prev_address):
-                    self.prev_address = curr_address
-                    refresh_session = True
-                    logger.info("PS address changes, refresh session config")
-                if refresh_session:
-                    self.refresh_config(curr_address)
+                ps_address_changed, change_type = self.ps_addresses_changed()
+                if ps_address_changed:
+                    self.refresh_env()
+                    if change_type == "ps_failure":
+                        self.exit_from_recoverable_session()
+                    else:
+                        self.info_cheif_do_checkpoints()
+                    break
                 time.sleep(10)
 
         self.runner = threading.Thread(target=monitor_fun)
+        self.runner.setDaemon(True)
         self.runner.start()
 
-    def refresh_config(self, cluster_spec: List[str]):
-        """Refresh session_creator._config
-        Refresh the cluster information and rebuild a session
-        linked to the new PS.
-
-        Args:
-         cluster_spec: list of `String`, which is the ps addresses
+    def ps_addresses_changed(self):
         """
-        assert (
-            len(cluster_spec) > 0
-        ), "there should be as least one ps address in the training cluster"
-        logger.info("ps cluster is {}".format(cluster_spec))
-        global_dict = common_util.GlobalDict()
-        session_creator = global_dict["session_creator"]
-        config = session_creator._config
-        if (
-            config is not None
-            and getattr(config, "cluster_def", None) is not None
-        ):
-            logger.info("before updating, session config is {}".format(config))
-            # Get worker's index and address from previous session config
-            # instead of TF_CONFIG
-            for i in config.cluster_def.job:
-                if i.name in [TFConstants.Worker, TFConstants.Chief]:
-                    task = i.tasks[0]
-                    if isinstance(task, dict):
-                        ind, address = list(task.items())[0]
-                    else:
-                        ind = 0
-                        address = task
-            logger.info(
-                "worker ind is {} and address is {}".format(ind, address)
-            )
-            len_job = len(config.cluster_def.job)
-            for i in range(len_job):
-                # pop ps and worker/chief info
-                config.cluster_def.job.pop()
-            worker_job = config.cluster_def.job.add()
-            worker_job.name = self.task_type
-            worker_job.tasks[ind] = address
-            ps_job = config.cluster_def.job.add()
-            ps_job.name = TFConstants.PS()
-            for i, j in enumerate(cluster_spec):
-                ps_job.tasks[i] = j
+        Check whether ps addresses changed.
+        There are at least two kinds: 1) the num of ps
+        addresses changed, 2) single ps address varies.
+        """
+        changed = False
+        changed_type = None
+        curr_address, ps_failure = self._failover_client.get_training_ps_addr()
+        if "".join(curr_address) != "".join(self.curr_ps_address):
+            if len(curr_address) != len(self.curr_ps_address):
+                changed_type = "scaling"
+            else:
+                changed_type = "migrating"
             logger.info(
-                "after updating, session config is %s.", str(vars(config))
+                "ps address changed from {} to {}.".format(
+                    self.curr_ps_address, curr_address
+                )
             )
+            if ps_failure is True:
+                changed_type = "ps_failure"
+                logger.warning(
+                    "ps failure happens, worker pod is going to exit"
+                )
+            self.curr_ps_address = curr_address
+            changed = True
+        return changed, changed_type
+
+    def refresh_env(self):
+        """Refresh tf env
+        update TF_CONFIG, when the training thread restarts
+        estimator will use the new TF_CONFIG
+        """
+        global_dict = common_util.GlobalDict()
+        global_dict["failover"] = self
+        tf_config = get_tf_config()
+        tf_config["cluster"]["ps"] = self.curr_ps_address
+        os.environ["TF_CONFIG"] = json.dumps(tf_config)
+        logger.info(
+            "successfully refresh TF_CONFIFG %s" % os.environ["TF_CONFIG"]
+        )
+
+    def exit_from_recoverable_session(self):
+        logger.info("exit_from_recoverable_session")
+        # TODO: when encountering ps failure, session will be hanged.
+        # we need to add grpc timeout
+        os._exit(2)
 
-            # TODO: before relaunch ps, there should a sync between all workers
-            if self.task_type == "chief":
-                self._failover_client.ready_for_ps_relaunch()
+    def set_training_thread(self, training_thread):
+        global_dict = common_util.GlobalDict()
+        global_dict[TFConstants.RelaunchForFailure.name] = True
+        self.training_thread = training_thread
+
+    def info_cheif_do_checkpoints(self):
+        global_dict = common_util.GlobalDict()
+        if self._is_chief:
+            # chief needs to do checkpoint and then
+            # set global_dict[TFConstants.SaveCheckpoint.name] = True
+            # In the checkpoint save hook,
+            # chief set global_dict[TFConstants.RelaunchForPs.name] = True
+            global_dict[TFConstants.SaveCheckpoint.name] = True
+        else:
+            # worker needs set
+            # global_dict[TFConstants.RelaunchForPs.name] = True
+            # and wait chief do checkpoints.
+            global_dict[TFConstants.RelaunchForPs.name] = True
+        logger.info("global dict is %s" % global_dict)
```

## dlrover/trainer/tensorflow/reader/__init__.py

```diff
@@ -6,7 +6,10 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from dlrover.trainer.tensorflow.reader.file_reader import (  # noqa: F401
+    FileReader,
+)
```

## dlrover/trainer/tensorflow/reader/file_reader.py

```diff
@@ -6,85 +6,40 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from dlrover.trainer.tensorflow.reader.base_reader import (  # noqa: F401
+    ElasticReader,
+)
 
-from dlrover.python.elastic_agent.sharding.client import ShardingClient
-from dlrover.trainer.util.log_util import default_logger as logger
 
-
-def build_data_shard_service(
-    batch_size=1,
-    num_epochs=1,
-    dataset_size=1,
-    num_minibatches_per_shard=1,
-    dataset_name="iris_training_data",
-):
-    sharding_client = ShardingClient(
-        dataset_name=dataset_name,
-        batch_size=batch_size,
-        num_epochs=num_epochs,
-        dataset_size=dataset_size,
-        num_minibatches_per_shard=num_minibatches_per_shard,
-    )
-    return sharding_client
-
-
-class FileReader:
-    def __init__(
-        self,
-        file_name,
-        num_epochs=1,
-        batch_size=64,
-        enable_dynamic_sharding=True,
-        skip_header=True,
-    ):
-
-        self._num_epochs = num_epochs
-        self._batch_size = batch_size
+class FileReader(ElasticReader):
+    def __init__(self, path=None, skip_header=True):
         self._skip_header = skip_header
-        self.enable_dynamic_sharding = enable_dynamic_sharding
-        self.data_shard_service = None
-        self._file_handler = open(file_name, "r")
-
-        self.count_data()
-        self.data_shard_client = None
-        self._consumed_data = 0
-        self.build_data_shard_client()
-
-    def build_data_shard_client(self):
-        if self.enable_dynamic_sharding is True:
-            self.data_shard_client = build_data_shard_service(
-                batch_size=self._batch_size,
-                num_epochs=1,
-                dataset_size=self._data_nums,
-                num_minibatches_per_shard=1,
-                dataset_name="iris_training_data",
-            )
-
-    def count_data(self):
+        self._file_handler = open(path, "r")
         self.data = self._file_handler.readlines()
-        if self._skip_header:
-            self._data_nums = len(self.data) - 1
-            self.data = self.data[1:]
-        else:
-            self._data_nums = len(self.data)
+        self._file_name = path
+        super().__init__(
+            path=path,
+        )
+        self._data_nums = None
 
-    def iterator(self):
-        while True:
-            shard = self.data_shard_client.fetch_shard()
-            if not shard:
-                break
-            for i in range(shard.start, shard.end):
-                logger.info("shard is {}".format(shard))
-                d = self.data[i]
-                d = d.strip()
-                dd = d.split(",")
-                assert len(dd) == 40
-                yield d
+    def count_data(self):
+        if self._data_nums is None:
+            if self._skip_header:
+                self._data_nums = len(self.data) - 1
+                self.data = self.data[1:]
+            else:
+                self._data_nums = len(self.data)
+
+    def read_data_by_index_range(self, start_index, end_index):
+        for i in range(start_index, end_index):
+            d = self.data[i]
+            d = d.strip()
+            yield d
 
     def __del__(self):
         if self._file_handler is not None:
             self._file_handler.close()
```

## dlrover/trainer/tensorflow/util/dataset_util.py

```diff
@@ -13,49 +13,45 @@
 
 from typing import Any, List
 
 import numpy as np
 import tensorflow as tf
 from tensorflow.python.ops import parsing_ops
 
-from dlrover.trainer.constants.tf_constants import TFConstants
-from dlrover.trainer.tensorflow.reader.fake_reader import FakeReader
-from dlrover.trainer.tensorflow.reader.file_reader import FileReader
-from dlrover.trainer.tensorflow.util import path_util
+from dlrover.trainer.tensorflow.reader.base_reader import ElasticReader
 from dlrover.trainer.tensorflow.util.column_info import Column
 from dlrover.trainer.util.log_util import default_logger as logger
 
 
 class DatasetUtil(object):
     """Prepare dataset from generator and parse them"""
 
     def __init__(
         self,
-        path=None,
+        reader=None,
         columns: List[Column] = [],
         reader_fn: Any = None,
         schema=None,
         batch_size=64,
         epoch=10,
+        field_delim=",",
     ):
 
         self.columns = columns
         self._batch_size = batch_size
         self._epoch = epoch
-        scheme, path = path_util.parse_uri(path)
-        self.path = path
-        if scheme == TFConstants.FILE_SCHEME():
-            self.reader = FileReader(
-                self.path, batch_size=self._batch_size, num_epochs=self._epoch
-            )
-        elif scheme == TFConstants.FAKE_SCHEME():
-            self.reader = FakeReader()  # type: ignore
-
-        if reader_fn is not None:
-            self.reader = reader_fn
+        self.reader = reader
+        self.field_delim = field_delim
+        self.set_reader()
+
+    def set_reader(self):
+        if isinstance(self.reader, ElasticReader):
+            self.reader.set_batch_size(self._batch_size)
+            self.reader.set_num_epochs(self._epoch)
+            self.reader.build_sharding_client()
 
     def make_dataset(self):
         def reader_fn():
             for data in self.reader.iterator():
                 yield data
 
         self._reader_fn = reader_fn
@@ -89,15 +85,17 @@
             elif dtype in all_types:
                 default_val = np.dtype(dtype).type(0)
             default_columns_types.append(default_val)
             default_columns_names.append(i.name)
 
         def parse_csv(value):
             columns = parsing_ops.decode_csv(
-                value, record_defaults=default_columns_types, field_delim=","
+                value,
+                record_defaults=default_columns_types,
+                field_delim=self.field_delim,
             )
             features = dict(zip(default_columns_names, columns))
             labels = features.pop(self._label_column_name)
             return features, labels
 
         return dataset.map(parse_csv, num_parallel_calls=10)
 
@@ -138,16 +136,26 @@
             job_name: ps/worker/chief/master
             slice_id: used for sharding
             slice_count: used for sharding
             project_dir: estimator project directory
             options: other keyword arguments
         """
 
-        path = data_set.get("path")
+        path = data_set.get("reader")
         columns = data_set.get("columns")
         reader_fn = data_set.get("reader_fn")
+        field_delim = data_set.get("field_delim", ",")
         dataset_util_kwargs = {
-            "path": path,
+            "reader": path,
             "columns": columns,
             "reader_fn": reader_fn,
+            "field_delim": field_delim,
         }
+
+        batch_size = data_set.get("batch_size", None)
+        epoch = data_set.get("epoch", None)
+        if batch_size is not None:
+            dataset_util_kwargs.update({"batch_size": batch_size})
+        if epoch is not None:
+            dataset_util_kwargs.update({"epoch": epoch})
+
         return DatasetUtil(**dataset_util_kwargs)
```

## dlrover/trainer/tensorflow/util/estimator_util.py

```diff
@@ -7,20 +7,156 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import json
+
 from tensorflow.python.estimator.estimator import Estimator
+from tensorflow.python.training import basic_session_run_hooks
 
+from dlrover.python.elastic_agent.sychronization.sync_client import SyncClient
 from dlrover.trainer.constants.tf_constants import TFConstants
+from dlrover.trainer.tensorflow.util import common_util
+from dlrover.trainer.tensorflow.util.tf_env_util import (
+    get_tf_config_task_type_and_index,
+)
 from dlrover.trainer.util.log_util import default_logger as logger
 
 
+def after_run(self, run_context, run_values):
+    task_type, _ = get_tf_config_task_type_and_index()
+    global_dict = common_util.GlobalDict()
+    relaunch_for_ps = global_dict.get(
+        TFConstants.RelaunchForPs.name, TFConstants.RelaunchForPs()
+    )
+    if relaunch_for_ps:
+        logger.info(
+            "The training thread should stop for due to ps migration/scaling"
+        )
+    if relaunch_for_ps:
+        # Only worker need to wait for cheif to do somethin before exit
+        # Chief doesn't need to wait.
+        if task_type == TFConstants.Worker.name:
+            SyncClient().join_sync("relauch_for_ps")
+            logger.info(
+                "Before stopping training thread,  \
+                worker should wait for cheif to save checkpoint"
+            )
+        run_context.request_stop()
+        if task_type == TFConstants.Worker.name:
+            # Workers need to wait for cheif to do somethin before exit
+            SyncClient().barrier("relauch_for_ps")
+            logger.info(
+                "Training thread stopped because chief had saved checkpoint"
+            )
+        else:
+            # Chief need to nofity workers
+            SyncClient().notify_barrier("relauch_for_ps")
+            logger.info(
+                "Checkpointed saved, cheif notify \
+                workers that they can stop training thread."
+            )
+            fail_over = global_dict["failover"]
+            fail_over._failover_client.ready_for_ps_relaunch()
+
+
+basic_session_run_hooks.StopAtStepHook.after_run = after_run
+
+
+def ck_after_run(self, run_context, run_values):
+    logger.info("save checkpoint session hook runs")
+
+    stale_global_step = run_values.results
+    global_dict = common_util.GlobalDict()
+    print(global_dict)
+    should_save_checkpoint = global_dict.get(
+        TFConstants.SaveCheckpoint.name, TFConstants.SaveCheckpoint()
+    )
+    data_shard_client = global_dict.get(
+        TFConstants.DataShardClient.name, TFConstants.DataShardClient()
+    )
+    data_shard_checkpoint = None
+    if should_save_checkpoint:
+        logger.info(
+            "Before saving checkpoint, cheif should wait for \
+                worker to enter PreStopAtStep Hook."
+        )
+        # CheckpointSaveHook is a kind of chiefhook
+        # Only chief run the hook
+        SyncClient().join_sync("relauch_for_ps")
+        logger.info(
+            "All workers have entered PreStopAtStep Hook \
+                and wait for cheif to save checkpoints"
+        )
+        # chief can relaun ps
+        global_dict[TFConstants.RelaunchForPs.name] = True
+    if (
+        self._timer.should_trigger_for_step(
+            stale_global_step + self._steps_per_run
+        )
+        or should_save_checkpoint
+    ):
+        # get the real value after train op.
+        global_step = run_context.session.run(self._global_step_tensor)
+        if (
+            self._timer.should_trigger_for_step(global_step)
+            or should_save_checkpoint
+        ):
+            self._timer.update_last_triggered_step(global_step)
+            if self._save(run_context.session, global_step):
+                run_context.request_stop()
+            if data_shard_checkpoint is not None:
+                data_shard_checkpoint = (
+                    data_shard_client.get_shard_checkpoint()
+                )
+    elif self._incremental_save:
+        if (
+            self._incremental_timer.should_trigger_for_step(
+                stale_global_step + 1
+            )
+            or should_save_checkpoint
+        ):
+            global_step = run_context.session.run(self._global_step_tensor)
+            if (
+                self._incremental_timer.should_trigger_for_step(global_step)
+                or should_save_checkpoint
+            ):
+                self._incremental_timer.update_last_triggered_step(global_step)
+                logger.info(
+                    "Start Save incremental checkpoints for %d into %s.",
+                    global_step,
+                    self._incremental_save_path,
+                )
+                self._get_incr_saver().incremental_save(
+                    run_context.session,
+                    self._incremental_save_path,
+                    global_step=global_step,
+                )
+                logger.info(
+                    "Finish Save incremental checkpoints for %d into %s.",
+                    global_step,
+                    self._incremental_save_path,
+                )
+                if data_shard_checkpoint is not None:
+                    data_shard_checkpoint = (
+                        data_shard_client.get_shard_checkpoint()
+                    )
+    if data_shard_checkpoint is not None:
+        logger.info(
+            "data_shard_checkpoint for global step {} is {}".format(
+                global_step, data_shard_checkpoint
+            )
+        )
+        with open(TFConstants.DataShardCheckpoint(), "w") as f:
+            json.dump(data_shard_checkpoint, f)
+
+
 def append_hooks(estimator_spec, key, params):
     old = getattr(estimator_spec, key) or []
     hooks = [hook for hook in params.get(key, [])]
     if hooks:
         hooks_names = [c.__class__.__name__ for c in hooks]
         hooks.extend(old)
         logger.info("Hooks before deduplication: %s = %s", key, hooks_names)
@@ -60,12 +196,29 @@
         if params:
             keys = [
                 TFConstants.EstimatorTrainingChiefHooks.name,
                 TFConstants.EstimatorTrainingHooks.name,
                 TFConstants.EstimatorEvaluationHooks.name,
                 TFConstants.EstimatorPredictionHooks.name,
             ]
+            stop_at_step_hook = basic_session_run_hooks.StopAtStepHook(
+                num_steps=10
+            )
+            training_hooks = params.get(
+                TFConstants.EstimatorTrainingHooks.name, []
+            )
+            training_hooks.append(stop_at_step_hook)
+            params[TFConstants.EstimatorTrainingHooks.name] = training_hooks
+
+            chief_training_hooks = params.get(
+                TFConstants.EstimatorTrainingChiefHooks.name, []
+            )
+            chief_training_hooks.append(stop_at_step_hook)
+            params[
+                TFConstants.EstimatorTrainingChiefHooks.name
+            ] = chief_training_hooks
+
             for key in keys:
                 model_fn_results = append_hooks(model_fn_results, key, params)
         return model_fn_results
 
     Estimator._call_model_fn = dlrover_call_model_fn
```

## dlrover/trainer/tensorflow/util/tf_patch_util.py

```diff
@@ -7,21 +7,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import json
 import time
 
 from tensorflow.python.client import session
 from tensorflow.python.framework import errors
 from tensorflow.python.training import monitored_session, session_manager
 from tensorflow.python.training.monitored_session import _WrappedSession
+from tensorflow_estimator.python.estimator.mode_keys import ModeKeys
 
+from dlrover.trainer.constants.tf_constants import TFConstants
 from dlrover.trainer.tensorflow.util import common_util
 from dlrover.trainer.tensorflow.util.tf_version_util import (
     is_tf_2,
     is_tf_113,
     is_tf_115,
 )
 from dlrover.trainer.util.log_util import default_logger as logger
@@ -299,14 +302,25 @@
         saver,
         checkpoint_dir=checkpoint_dir,
         checkpoint_filename_with_path=checkpoint_filename_with_path,
         wait_for_checkpoint=wait_for_checkpoint,
         max_wait_secs=max_wait_secs,
         config=config,
     )
+    global_dict = common_util.GlobalDict()
+    if is_loaded_from_checkpoint:
+        data_shard_client = global_dict.get(
+            TFConstants.DataShardClient.name, TFConstants.DataShardClient()
+        )
+        if data_shard_client is not None:
+            with open("data_shard_checkpoint.json", "r") as f:
+                data_shard_checkpoint = json.load(f)
+                data_shard_client.restore_shard_from_checkpoint(
+                    data_shard_checkpoint
+                )
     if not is_loaded_from_checkpoint:
         if init_op is None and not init_fn and self._local_init_op is None:
             raise RuntimeError(
                 "Model is not initialized and no init_op or "
                 "init_fn or local_init_op was given"
             )
         if init_op is not None:
@@ -335,23 +349,51 @@
             )
         )
     global_dict = common_util.GlobalDict()
     global_dict["sess"] = sess
     return sess
 
 
+def export_saved_model(
+    self,
+    export_dir_base,
+    serving_input_receiver_fn,
+    assets_extra=None,
+    as_text=False,
+    checkpoint_path=None,
+    experimental_mode=ModeKeys.PREDICT,
+    save_incr_model=True,
+):
+    # pylint: enable=line-too-long
+    if not serving_input_receiver_fn:
+        raise ValueError("An input_receiver_fn must be defined.")
+
+    input_receiver_fn_map = {experimental_mode: serving_input_receiver_fn}
+
+    return self._export_all_saved_models(
+        export_dir_base,
+        input_receiver_fn_map,
+        assets_extra=assets_extra,
+        as_text=as_text,
+        checkpoint_path=checkpoint_path,
+        strip_default_attrs=True,
+        save_incr_model=save_incr_model,
+    )
+
+
 def hotpatch_for_dynet(failover_level=1):
     """Patch for tensorflow in order to"""
 
     logger.info("Hot patch for dynet")
     if failover_level == 1:
         # Get the session after initialization
         monitored_session._RecoverableSession.__init__ = (
             init_and_get_session_creator
         )
         session_manager.SessionManager.wait_for_session = (
             wait_for_session_and_get_session
         )
     if is_tf_115():
         session_manager.SessionManager.prepare_session = prepare_session_115
+
     if is_tf_113() or is_tf_2():
         session_manager.SessionManager.prepare_session = prepare_session_113
```

## dlrover/trainer/util/args_util.py

```diff
@@ -37,14 +37,20 @@
         "--evaluator_num", help="evaluator number", type=int, default=1
     )
 
     parser.add_argument(
         "--conf", help="configuration for training", default=None
     )
 
+    parser.add_argument("--task_id", help="worker id", type=int)
+
+    parser.add_argument("--task_type", help="worker type", type=str)
+
+    parser.add_argument("--mock", type=bool)
+
     parser.add_argument(
         "--enable_auto_scaling",
         help="configuration for elastic training",
         type=bool,
         default=False,
     )
```

## dlrover/trainer/util/conf_util.py

```diff
@@ -8,14 +8,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import inspect
+import os
 
 from pyhocon import ConfigFactory, ConfigMissingException, ConfigTree
 
 from dlrover.trainer.util import reflect_util
 from dlrover.trainer.util.log_util import default_logger as logger
 
 config_tree_get_ori = ConfigTree.get
@@ -187,14 +188,15 @@
 
     pass
 
 
 def get_conf(py_conf=None):
     """Get `ConfigurationManager` from args"""
     logger.info(f"Entering get_conf, original py_conf is {py_conf}")
+    logger.info("current working director is %s" % os.getcwd())
     attribute_class = py_conf
     if py_conf:
         if isinstance(py_conf, str):
             attribute_class = reflect_util.get_class(py_conf)
     properties = dict()
     for i in dir(attribute_class):
         if not i.startswith("__"):
```

## dlrover/trainer/worker/tf_kubernetes_worker.py

```diff
@@ -6,14 +6,15 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import threading
 
 from dlrover.trainer.constants.tf_constants import TFConstants
 from dlrover.trainer.tensorflow.executor.estimator_executor import (
     EstimatorExecutor,
 )
 from dlrover.trainer.tensorflow.failover.tensorflow_failover import (
     TensorflowFailover,
@@ -30,29 +31,62 @@
         """
         Argument:
             args: result of parsed command line arguments
         """
         self._args = args
         task_conf = get_conf(py_conf=args.conf)
         self._task_conf = task_conf
+        self.estimator_server_started = False
         self.init_executor(task_conf)
 
     def init_executor(self, task_conf):
+        logger.info("init_executor")
         self.estimator = EstimatorExecutor(task_conf)
 
     def start_failover_monitor(self):
         if self._args.enable_auto_scaling:
             self._task_conf.put(TFConstants.EnableDynamicSharding.name, True)
             self.tensorflow_failover = TensorflowFailover()
             self.tensorflow_failover.start_failover_monitor()
 
+    def run_ps(self):
+        logger.info("ps server join")
+        self.estimator.server.join()
+
+    def run_worker(self):
+        self.estimator.train_and_evaluate()
+
     def run(self):
-        global_dict = common_util.GlobalDict()
-        global_dict["executor"] = self.estimator
-        self.start_failover_monitor()
         logger.info("KubernetesWorker is running!")
-        self.estimator.start_server()
-        if self.estimator.task_type == TFConstants.PS():
-            logger.info("ps server join")
-            self.estimator.server.join()
-        else:
-            self.estimator.train_and_evaluate()
+        while True:
+            global_dict = common_util.GlobalDict()
+            self.start_failover_monitor()
+            global_dict["executor"] = self.estimator
+            self.estimator.prepare()
+            if not self.estimator_server_started:
+                self.estimator.start_server()
+                self.estimator_server_started = True
+            if self.estimator.task_type == TFConstants.PS():
+                run_thread = threading.Thread(target=self.run_ps)
+            else:
+                run_thread = threading.Thread(target=self.run_worker)
+                if hasattr(self, "tensorflow_failover"):
+                    self.tensorflow_failover.set_training_thread(run_thread)
+            run_thread.start()
+            run_thread.join()
+            if not run_thread.is_alive():
+                if global_dict.get(
+                    TFConstants.RelaunchForPs.name, TFConstants.RelaunchForPs()
+                ):
+                    logger.info("ps is migrating or scaling")
+                elif global_dict.get(
+                    TFConstants.RelaunchForFailure.name,
+                    TFConstants.RelaunchForFailure(),
+                ):
+                    logger.info(
+                        "worker encounters ps failure and restart thread"
+                    )
+                else:
+                    break
+                global_dict.clear()
+                self.init_executor(self._task_conf)
+                continue
```

## Comparing `dlrover/python/master/node/node_manager.py` & `dlrover/python/master/node/job_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,34 +8,44 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import copy
+import os
 import threading
 import time
+import traceback
 from typing import Dict, List
 
 from dlrover.python.common.constants import (
     DistributionStrategy,
     NodeEventType,
     NodeExitReason,
     NodeResourceLimit,
     NodeStatus,
     NodeType,
 )
 from dlrover.python.common.global_context import Context
 from dlrover.python.common.log import default_logger as logger
-from dlrover.python.common.node import Node, NodeResource
+from dlrover.python.common.node import Node, NodeGroupResource
+from dlrover.python.master.monitor.error_monitor import (
+    ErrorLogMonitor,
+    ErrorMonitor,
+)
 from dlrover.python.master.monitor.speed_monitor import SpeedMonitor
 from dlrover.python.master.node.event_callback import (
     ClusterContext,
     NodeEventCallback,
 )
+from dlrover.python.master.node.job_auto_scaler import (
+    JobAutoScaler,
+    new_job_auto_scaler,
+)
 from dlrover.python.master.node.ps import ParameterServerManager
 from dlrover.python.master.node.status_flow import (
     NodeStateFlow,
     get_node_state_flow,
 )
 from dlrover.python.master.node.training_node import (
     get_critical_worker_index,
@@ -44,109 +54,143 @@
 )
 from dlrover.python.master.node.worker import (
     ChiefManager,
     EvaluatorManager,
     WorkerManager,
 )
 from dlrover.python.master.resource.job import (
+    AllreduceJobResourceOptimizer,
     JobResource,
     JobResourceOptimizer,
+    PSJobResourceOptimizer,
 )
-from dlrover.python.master.resource.optimizer import ResourcePlan
 from dlrover.python.master.scaler.base_scaler import ScalePlan, Scaler
 from dlrover.python.master.scaler.factory import new_job_scaler
 from dlrover.python.master.watcher.base_watcher import NodeEvent
-from dlrover.python.master.watcher.factory import new_node_watcher
+from dlrover.python.master.watcher.factory import (
+    new_node_watcher,
+    new_scale_plan_watcher,
+)
 from dlrover.python.scheduler.factory import new_elastic_job
 from dlrover.python.scheduler.job import ElasticJob, JobArgs
 
-_MAX_POD_RELAUNCH_COUNT = 5
 _dlrover_context = Context.singleton_instance()
 
+_MAX_POD_RELAUNCH_COUNT = 5
+
 
-class NodeManager(object):
+class JobManager(object):
     def __init__(
         self,
         job_args: JobArgs,
         critical_worker_index={},
         wait_pending_relaunch=False,
         speed_monitor=None,
         job=None,
         node_watcher=None,
         job_scaler=None,
+        error_monitor=None,
     ):
         self._job_resource = JobResource()
         node_restart_count: Dict[str, int] = {}
         for type, node_args in job_args.node_args.items():
             self._job_resource.node_group_resources[
                 type
             ] = node_args.group_resource
             node_restart_count[type] = node_args.restart_count
 
         self._job_args = job_args
         self._ps_is_critical = False
         if (
-            job_args.distribution_strategy
-            == DistributionStrategy.PARAMETER_SERVER
+            job_args.distribution_strategy == DistributionStrategy.PS
+            or job_args.distribution_strategy == DistributionStrategy.CUSTOM
         ):
             self._ps_is_critical = (
                 job_args.node_args[NodeType.PS].critical_nodes == "all"
             )
+            self._job_optimizer: JobResourceOptimizer = PSJobResourceOptimizer(
+                self._job_resource.node_group_resources[NodeType.WORKER],
+                self._job_resource.node_group_resources[NodeType.PS],
+                job_args.optimize_mode,
+                job_args.job_uuid,
+                job_args.resource_limits,
+            )
+        elif job_args.distribution_strategy == DistributionStrategy.ALLREDUCE:
+            self._job_optimizer: JobResourceOptimizer = (
+                AllreduceJobResourceOptimizer(
+                    self._job_resource.node_group_resources[NodeType.WORKER],
+                    job_args.job_uuid,
+                )
+            )
+        else:
+            raise ValueError(
+                f"Distribution strategy {job_args.distribution_strategy} "
+                "is not supported. You can specify it with "
+                "ParameterServerStrategy/AllreduceStrategy."
+            )
+        logger.info("New job optimizer : %s", self._job_optimizer.__class__)
 
         worker_restart_count = node_restart_count.get(NodeType.WORKER, 0)
         ps_restart_count = node_restart_count.get(NodeType.PS, 0)
 
         self._relaunch_on_worker_failure = min(
             worker_restart_count, _MAX_POD_RELAUNCH_COUNT
         )
         self._wait_pending_relaunch = wait_pending_relaunch
         self._start_launch_waiting_workers_time = time.time()
-        self._stop_launch_worker_for_ps = False
         self._critical_worker_index = critical_worker_index
         self._ps_relaunch_max_num = min(
             ps_restart_count, _MAX_POD_RELAUNCH_COUNT
         )
-        self._use_ddp = job_args.use_ddp
         self._node_event_callbacks: List[NodeEventCallback] = []
-        self._chief_started = False
         self._stop_monitor = False
         self._speed_monitor: SpeedMonitor = speed_monitor
+        self._error_monitor: ErrorMonitor = error_monitor
 
         # Protects followed variables, which are accessed from event_cb.
         self._lock = threading.Lock()
         self._job_nodes: Dict[str, Dict[int, Node]] = {}
 
         self._elastic_job: ElasticJob = job
         self._node_watcher = node_watcher
-        self._scaler: Scaler = job_scaler
-        self._job_optimizer = JobResourceOptimizer(
-            self._job_resource.node_group_resources[NodeType.WORKER],
-            self._job_resource.node_group_resources[NodeType.PS],
-            job_args.scaling_optimizer,
+
+        self._scaler_watcher = new_scale_plan_watcher(
+            job_args.platform,
+            job_args.job_name,
+            job_args.namespace,
             job_args.job_uuid,
-            job_args.resource_limits,
         )
+        self._scaler: Scaler = job_scaler
         self._init_training_node_manager()
 
     def start(self):
         self._job_optimizer.update_job_uuid(self._job_args.job_uuid)
         self._job_optimizer.init_job_resource(self._job_resource)
         self._adjust_worker_for_estimator()
-        self._init_job_nodes()
+        self._init_nodes()
+        self._init_job_auto_scaler()
         plan = self._create_initial_scale_plan()
         self._scaler.scale(plan)
+        worker_num = 0
+        if NodeType.WORKER in plan.node_group_resources:
+            worker_num = plan.node_group_resources[NodeType.WORKER].count
+        if NodeType.CHIEF in plan.node_group_resources:
+            worker_num += plan.node_group_resources[NodeType.CHIEF].count
+        self._speed_monitor.set_target_worker_num(worker_num)
         threading.Thread(
             target=self._monitor_nodes, name="node_monitor", daemon=True
         ).start()
+        threading.Thread(
+            target=self._monitor_scale_plan_crd,
+            name="scaleplan_monitor",
+            daemon=True,
+        ).start()
 
     def _adjust_worker_for_estimator(self):
-        if (
-            self._job_args.distribution_strategy
-            == DistributionStrategy.PARAMETER_SERVER
-        ):
+        if self._job_args.distribution_strategy == DistributionStrategy.PS:
             self._job_resource.adjust_worker_for_estimator()
 
     def _create_initial_scale_plan(self):
         scale_plan = ScalePlan()
         scale_plan.node_group_resources = copy.deepcopy(
             self._job_resource.node_group_resources
         )
@@ -157,40 +201,44 @@
         self._ps_manager = ParameterServerManager(
             self._job_nodes.get(NodeType.PS, {}),
             self._job_resource,
             self._ps_relaunch_max_num,
             self._elastic_job.get_node_service_addr,
             self._elastic_job.get_node_name,
         )
+
+        chief_nodes = self._job_nodes.get(NodeType.CHIEF, {})
+        if not chief_nodes:
+            chief_nodes = self._job_nodes.get(NodeType.MASTER, {})
         self._chief_manager = ChiefManager(
-            self._job_nodes.get(NodeType.CHIEF, {}),
+            chief_nodes,
             self._job_resource,
-            self._ps_relaunch_max_num,
+            self._relaunch_on_worker_failure,
             self._elastic_job.get_node_service_addr,
             self._elastic_job.get_node_name,
         )
         self._worker_manager = WorkerManager(
             self._job_nodes.get(NodeType.WORKER, {}),
             self._job_resource,
-            self._ps_relaunch_max_num,
+            self._relaunch_on_worker_failure,
             self._elastic_job.get_node_service_addr,
             self._elastic_job.get_node_name,
         )
         self._evaluator_manager = EvaluatorManager(
             self._job_nodes.get(NodeType.EVALUATOR, {}),
             self._job_resource,
-            self._ps_relaunch_max_num,
+            self._relaunch_on_worker_failure,
             self._elastic_job.get_node_service_addr,
             self._elastic_job.get_node_name,
         )
 
     def add_node_event_callback(self, node_event_callback):
         self._node_event_callbacks.append(node_event_callback)
 
-    def _init_job_nodes(self):
+    def _init_nodes(self):
         self._job_nodes = self._job_resource.init_job_node_meta(
             self._relaunch_on_worker_failure,
             self._elastic_job.get_node_service_addr,
             self._elastic_job.get_node_name,
         )
 
         # worker and eval ids for nodes that should be created
@@ -203,45 +251,88 @@
         set_critical_node(
             self._job_nodes,
             self._ps_is_critical,
             self._ps_relaunch_max_num,
             self._critical_worker_index,
         )
         update_nodes_priority(self._job_nodes)
+
         self._ps_manager.update_nodes(self._job_nodes.get(NodeType.PS, {}))
         self._chief_manager.update_nodes(
             self._job_nodes.get(NodeType.CHIEF, {})
         )
         self._worker_manager.update_nodes(
             self._job_nodes.get(NodeType.WORKER, {})
         )
         self._evaluator_manager.update_nodes(
             self._job_nodes.get(NodeType.EVALUATOR, {})
         )
 
+    def _init_job_auto_scaler(self):
+        self._job_autoscaler: JobAutoScaler = new_job_auto_scaler(
+            self._job_args.distribution_strategy,
+            self._job_resource,
+            self._job_nodes,
+            self._job_optimizer,
+            self._speed_monitor,
+            self._ps_manager,
+            self._worker_manager,
+            self._scaler,
+        )
+        logger.info(
+            "Create job autoscaler: %s", self._job_autoscaler.__class__
+        )
+
     def _monitor_nodes(self):
         logger.info("Start to monitor nodes")
         while True:
             nodes = self._node_watcher.list()
             self._process_list_nodes(nodes)
             try:
                 if self._stop_monitor:
                     logger.info("Stop processing node events")
                     break
                 for event in self._node_watcher.watch():
                     try:
                         self._process_event(event)
                     except Exception as e:
                         logger.warning(e)
+                        detail_trace_back = traceback.format_exc()
+                        logger.warning(detail_trace_back)
             except Exception as e:
                 logger.warning(e)
                 time.sleep(30)
 
+    def _monitor_scale_plan_crd(self):
+        """Monitor the Scaler CRD from users to adjust the job resource"""
+        logger.info("Start to monitor Scaler CRD")
+        while True:
+            try:
+                if self._stop_monitor:
+                    logger.info("Stop monitoring Scaler CRDs")
+                    break
+                for plan in self._scaler_watcher.watch():
+                    try:
+                        self._job_autoscaler.execute_job_optimization_plan(
+                            plan
+                        )
+                    except Exception as e:
+                        logger.warning(e)
+                        detail_trace_back = traceback.format_exc()
+                        logger.warning(detail_trace_back)
+            except Exception as e:
+                logger.warning(e)
+                detail_trace_back = traceback.format_exc()
+                logger.warning(detail_trace_back)
+                time.sleep(5)
+
     def _process_list_nodes(self, nodes: List[Node]):
         """Callback with node list by the list api of k8s."""
+        if not nodes:
+            return
         exist_nodes: Dict[str, List[int]] = {}
         for node_type in self._job_nodes.keys():
             exist_nodes[node_type] = []
         for node in nodes:
             exist_nodes[node.type].append(node.id)
             if node.status == NodeStatus.DELETED:
                 type = NodeEventType.DELETED
@@ -261,30 +352,45 @@
                     logger.info(
                         "Node %s %s is deleted without the event",
                         node_type,
                         node_id,
                     )
                     node.is_released = True
 
+    def close_job(self):
+        plan = ScalePlan()
+        ps_resource = NodeGroupResource.new_empty()
+        worker_reource = NodeGroupResource.new_empty()
+        plan.node_group_resources = {
+            "worker": worker_reource,
+            "ps": ps_resource,
+        }
+        self._scaler.scale(plan=plan)
+        os._exit(0)
+
     def _process_event(self, event: NodeEvent):
         node_type = event.node.type
         node_id = event.node.id
         if node_id not in self._job_nodes[node_type]:
             self._job_nodes[node_type][node_id] = event.node
             return
         else:
             cur_node = self._job_nodes[node_type][node_id]
             cur_node.update_info(
                 name=event.node.name,
                 start_time=event.node.start_time,
                 create_time=event.node.create_time,
+                host_name=event.node.host_name,
+                host_ip=event.node.host_ip,
             )
 
         # For the given node id, check whether it meets
         # the state change condition
+        if event.event_type == "exit":
+            self.close_job()
         new_status = event.node.status
         with self._lock:
             old_status = cur_node.status
             status_change_flow: NodeStateFlow = get_node_state_flow(
                 old_status, event.event_type, new_status
             )
             cur_node.update_status(new_status)
@@ -304,29 +410,29 @@
             should_relaunch = self._should_relaunch(
                 cur_node, status_change_flow
             )
             if should_relaunch and self._wait_pending_relaunch:
                 self._pending_relaunch_count += 1
 
         logger.info(
-            "%s status change: %s to %s, by evt_type %s, phase %s",
+            "%s status change: %s to %s, by evt_type %s reason %s",
             cur_node.name,
             old_status,
             new_status,
             event.event_type,
-            new_status,
+            cur_node.exit_reason,
         )
 
         if should_relaunch:
             self._relaunch_node(cur_node)
 
     def _process_node_events(
         self, status_change_flow: NodeStateFlow, node: Node
     ):
-        cluster_context = ClusterContext(node_manager=self)
+        cluster_context = ClusterContext(job_manager=self)
         if status_change_flow.to_status == NodeStatus.RUNNING:
             [
                 callback.on_node_started(node, cluster_context)
                 for callback in self._node_event_callbacks
             ]
         elif status_change_flow.to_status == NodeStatus.SUCCEEDED:
             [
@@ -351,19 +457,22 @@
     def _should_relaunch(self, node: Node, status_change_flow: NodeStateFlow):
         should_relaunch = (
             status_change_flow.should_relaunch
             and self._enable_relaunch_node
             and node.relaunchable
         )
         if should_relaunch:
-            if node.exit_reason == NodeExitReason.FATAL_ERROR:
+            if (
+                node.exit_reason == NodeExitReason.FATAL_ERROR
+                and not _dlrover_context.relaunch_error
+            ):
                 should_relaunch = False
             elif node.exit_reason == NodeExitReason.OOM:
                 mem = node.config_resource.memory
-                if mem > NodeResourceLimit.MAX_MEMORY:
+                if mem >= NodeResourceLimit.MAX_MEMORY:
                     should_relaunch = False
                     logger.warning(
                         "The memory of worker %s is beyond the limit %s MB.",
                         mem,
                         NodeResourceLimit.MAX_MEMORY,
                     )
                 elif node.relaunch_count >= node.max_relaunch_count:
@@ -371,39 +480,37 @@
                     logger.warning(
                         "The relaunched count %s is beyond the maximum %s.",
                         node.relaunch_count,
                         node.max_relaunch_count,
                     )
                 else:
                     node.is_recovered_oom = True
-                    if node.type == NodeType.PS:
-                        self._job_optimizer.adjust_oom_ps_resource(node)
-                    else:
-                        self._job_optimizer.adjust_oom_worker_resource(node)
+                    self._job_optimizer.adjust_oom_resource(node)
             elif node.exit_reason != NodeExitReason.KILLED:
                 if node.relaunch_count > node.max_relaunch_count:
                     logger.warning(
                         "The relaunch count for Error has been exhausted."
                     )
                     should_relaunch = False
         if should_relaunch:
             node.inc_relaunch_count()
 
         return should_relaunch
 
     def _relaunch_node(self, node: Node):
-        logger.info("Relaunch node: {}".format(node.name))
         if node.type == NodeType.WORKER:
             plan = self._worker_manager.relaunch_node(node)
         elif node.type == NodeType.PS:
             plan = self._ps_manager.relaunch_node(node)
         elif node.type == NodeType.EVALUATOR:
             plan = self._evaluator_manager.relaunch_node(node)
-        elif node.type == NodeType.CHIEF:
+        elif node.type == NodeType.CHIEF or node.type == NodeType.MASTER:
             plan = self._chief_manager.relaunch_node(node)
+        else:
+            logger.error("Not support node type %s", node.type)
         self._set_ps_addrs_in_plan(plan)
         self._scaler.scale(plan)
 
     def all_workers_exited(self):
         return (
             self._chief_manager.all_nodes_exited()
             and self._worker_manager.all_nodes_exited()
@@ -442,254 +549,164 @@
 
     def remove_worker(self, worker_id):
         if self._job_nodes[NodeType.WORKER][worker_id].critical:
             logger.info("Skip the critical worker %s", worker_id)
         else:
             logger.info("Delete worker %s", worker_id)
             plan = self._worker_manager.remove_node(worker_id)
-            logger.info("plan %s", plan)
+            logger.info("plan %s", plan.toJSON())
+            self._scaler.scale(plan)
 
     def get_running_nodes(self):
         nodes = self._chief_manager.get_running_nodes()
         nodes.extend(self._worker_manager.get_running_nodes())
         nodes.extend(self._evaluator_manager.get_running_nodes())
-        nodes.extend(self._ps_manager.get_training_ps_cluster())
+        nodes.extend(self._ps_manager.get_running_nodes())
         return nodes
 
     def get_running_workers(self):
-        return self._worker_manager.get_running_nodes()
+        workers = self._worker_manager.get_running_nodes()
+        chiefs = self._chief_manager.get_running_nodes()
+        workers.extend(chiefs)
+        return workers
 
     def post_ps_ready(self):
-        self._ps_manager.process_after_ps_cluster_ready()
+        plan = self._ps_manager.process_after_ps_cluster_ready()
+        if not plan.empty():
+            self._scaler.scale(plan)
+        else:
+            logger.info("Skip an empty scaleplan")
 
     def stop(self):
         self._enable_relaunch_node = False
         with self._lock:
             for node_type in self._job_nodes.keys():
                 for node in self._job_nodes[node_type].values():
                     node.critical = False
                     node.is_released = True
                     node.relaunchable = False
+            for node in self._job_nodes[NodeType.WORKER].values():
+                node.eval_time = self._speed_monitor.get_worker_eval_time(
+                    node.id
+                )
         self._stop_monitor = True
 
     def update_node_resource_usage(self, node_type, node_id, cpu, memory):
         node = self._job_nodes[node_type][node_id]
         node.update_resource_usage(cpu, memory)
 
+    def update_node_service_addr(self, node_type, node_id, service_addr):
+        node = self._job_nodes[node_type][node_id]
+        node.update_service_address(service_addr)
+        node.status = NodeStatus.RUNNING
+        node.is_released = False
+        self._job_nodes[node_type][node_id] = node
+
     def get_cur_cluster_ps(self):
         """Get PS nodes in the current training cluster."""
+        logger.info("job nodes are {}".format(self._job_nodes))
         return self._ps_manager.get_training_ps_cluster()
 
     def get_next_cluster_ps(self):
         """Get PS nodes in the next training cluster."""
         return self._ps_manager.get_next_training_ps_cluster()
 
     def ready_for_new_ps_cluster(self):
+        """Check whether ps cluster is used to training"""
         return self._ps_manager.get_ready_for_new_ps_cluster()
 
+    def has_ps_failure(self):
+        """Check whether ther is PS failure"""
+        return self._ps_manager.has_ps_failure()
+
     def remove_training_nodes(self):
         """Remove all PS and workers"""
+        self._job_autoscaler.stop_auto_scaling()
         plan = ScalePlan()
         training_nodes = list(
             self._job_nodes[NodeType.WORKER].values()
         ) + list(self._job_nodes[NodeType.PS].values())
         for node in training_nodes:
             if (
                 node.status in [NodeStatus.RUNNING, NodeStatus.PENDING]
                 and not node.is_released
             ):
                 node.critical = False
                 node.relaunchable = False
                 node.is_released = True
                 node.status = NodeStatus.DELETED
                 logger.info("Remove node %s", node.name)
-                plan.remove_nodes.append(node.name)
+                plan.remove_nodes.append(node)
         self._scaler.scale(plan)
 
-    def start_auto_scale(self):
+    def start_auto_scaling(self):
         """Start to auto-scale nodes to improve the training throughput."""
-        if not self._chief_started:
-            logger.info("Chief started!")
-            self._chief_started = True
-            if self._job_resource.worker_num > 1:
-                plan = self._job_optimizer.optimize_worker_resource()
-                self._execute_job_optimization_plan(plan)
-            if (
-                not _dlrover_context.auto_ps_enabled
-                and not _dlrover_context.auto_worker_enabled
-            ):
-                return
-            if self._speed_monitor:
-                self._speed_monitor.set_target_worker_num(
-                    self._job_resource.worker_num
-                    + self._job_resource.chief_num
-                )
-                threading.Thread(
-                    target=self._periodic_optimize_running_resource,
-                    name="resource-autoscaler",
-                    daemon=True,
-                ).start()
-
-    def _periodic_optimize_running_resource(self):
-        """Adjust job resource periodically and stop adjustment
-        if there is a failed worker with the fatal error.
-        """
-        logger.info("Start to auto scale ")
-        last_plan_time = 0
-        opt_interval = _dlrover_context.seconds_interval_to_optimize
-        while True:
-            if self._stop_launch_worker_for_ps:
-                logger.info("Stop to autoscale the number of worker.")
-                break
-            if (
-                self._speed_monitor.worker_adjustment_finished()
-                # Control the interval to query plans
-                and time.time() - last_plan_time > opt_interval
-                and not self._ps_manager.exist_migrated_ps_nodes()
-            ):
-                plan = self._job_optimizer.get_job_resource_plan()
-                if plan:
-                    last_plan_time = time.time()
-                plan = self._skip_ps_plan_if_needed(plan)
-                self._execute_job_optimization_plan(plan)
-            time.sleep(30)
-
-    def _execute_job_optimization_plan(self, plan: ResourcePlan):
-        """Execute the optimization plan of the training job.
-        The plan may adjust the number of PS and workers or
-        adjust the cpu and memory of nodes.
-        """
-        scale_plan = ScalePlan()
-        if not plan or plan.empty():
-            return scale_plan
-        for node_type, group in plan.node_group_resources.items():
-            if group.count > 0:
-                self._job_resource.update_node_group_resource(
-                    node_type,
-                    group.count,
-                    group.node_resource.cpu,
-                    group.node_resource.memory,
-                )
-                scale_plan.node_group_resources[node_type] = copy.deepcopy(
-                    self._job_resource.get_node_group_resource(node_type)
-                )
-                if node_type == NodeType.PS:
-                    self._ps_manager.adjust_ps(group)
-                    self._speed_monitor.reset_running_speed_monitor()
-                elif node_type == NodeType.WORKER:
-                    self._speed_monitor.set_target_worker_num(group.count)
-                    self._worker_manager.adjust_worker(group)
-        if len(plan.node_resources) > 0:
-            migration_plan = self._migrate_nodes(plan.node_resources)
-            scale_plan.merge(migration_plan)
-        self._set_ps_addrs_in_plan(scale_plan)
-        self._scaler.scale(scale_plan)
-        return scale_plan
-
-    def _skip_ps_plan_if_needed(self, plan: ResourcePlan):
-        """There is overhead to adjust the PS resource. So, the master
-        will skip adjusting PS if there is no remarkable change
-        of the PS resource.
-        """
-        if not plan or NodeType.PS not in plan.node_group_resources:
-            return plan
-        ps_resource = plan.node_group_resources[NodeType.PS]
-        ps_cpu = ps_resource.node_resource.cpu
-
-        if ps_resource.count > 0:
-            total_cpu = ps_resource.count * ps_cpu
-            cur_request_cpu = self._ps_manager.get_total_request_cpu()
-            threshold = _dlrover_context.seconds_huge_training_threshold
-            if self._speed_monitor.init_training_time > threshold:
-                logger.info(
-                    "Skip adjusting PS because the initial time %s"
-                    "of model is too long",
-                    self._speed_monitor.init_training_time,
-                )
-                del plan.node_group_resources[NodeType.PS]
-                return plan
-            elif (
-                total_cpu
-                < cur_request_cpu * NodeResourceLimit.PS_CPU_GROWTH_RATE
-                and total_cpu
-                > cur_request_cpu * NodeResourceLimit.PS_CPU_DECREASED_RATE
-            ):
-                logger.info(
-                    "Skip adjusting PS: the current CPU = %s,"
-                    "the target CPU = %s",
-                    cur_request_cpu,
-                    total_cpu,
-                )
-                del plan.node_group_resources[NodeType.PS]
-                return plan
-
-        ps_nodes = self._ps_manager.get_training_ps_cluster()
-        for ps in ps_nodes:
-            if ps_cpu > ps.config_resource.cpu:
-                plan.node_resources[ps.name].cpu = ps_cpu
-        return plan
-
-    def _migrate_nodes(self, node_resources):
-        workers: Dict[str, NodeResource] = {}
-        ps: Dict[str, NodeResource] = {}
-        for name, resource in node_resources.items():
-            type = name.split("-")[-2]
-            if type == NodeType.WORKER:
-                workers[name] = resource
-            elif type == NodeType.PS:
-                ps[name] = resource
-
-        scale_plan = ScalePlan()
-        if len(ps) > 0:
-            plan = self._ps_manager.migrate_parameter_servers(ps)
-            scale_plan.merge(plan)
-            self._speed_monitor.reset_running_speed_monitor()
-
-        if len(workers) > 0:
-            plan = self._worker_manager.migrate_workers(workers)
-            scale_plan.merge(plan)
-        logger.info("Migration plan = %s", scale_plan.toJSON())
-        return scale_plan
+        self._job_autoscaler.start_auto_scaling()
 
     def _set_ps_addrs_in_plan(self, plan: ScalePlan):
         ps_addrs = self._ps_manager.get_ps_addrs()
         plan.ps_addrs.extend(ps_addrs)
 
-    def cut_timeout_pending_node_cpu(self):
-        """Cut down CPU cores of pending pod at the job starts"""
-        if self._chief_started:
-            return
-        if _dlrover_context.auto_ps_enabled:
-            self._ps_manager.cut_pending_node_cpu()
-        if _dlrover_context.auto_worker_enabled:
-            self._worker_manager.cut_pending_node_cpu()
+    def all_running_node_hanged(self):
+        node_hang = self._worker_manager.running_nodes_hanged()
+        node_hang.extend(self._chief_manager.running_nodes_hanged())
+        node_hang.extend(self._evaluator_manager.running_nodes_hanged())
+        node_hang.extend(self._ps_manager.running_nodes_hanged())
+        if node_hang:
+            return all(node_hang)
+        return False
+
+    def remove_not_joined_rdzv_workers(self, worker_ranks):
+        plan = self._worker_manager.remove_not_joined_rdzv_workers(
+            worker_ranks
+        )
+        self._scaler.scale(plan)
 
+    def pend_without_workers(self):
+        """Check whether to wait for evicted workers."""
+        if self._worker_manager.has_failed_worker():
+            return False
+        elif self._worker_manager.wait_worker_restart():
+            return True
+        else:
+            return False
 
-def create_node_manager(args: JobArgs, speed_monitor) -> NodeManager:
-    # relaunch on worker failure for PS or custom strategy
-    if (
-        args.distribution_strategy != DistributionStrategy.PARAMETER_SERVER
-        and args.distribution_strategy != DistributionStrategy.CUSTOM
+    def handle_training_failure(
+        self, node_type, node_id, restart_count=-1, error_data=""
     ):
-        args.node_args[NodeType.WORKER].restart_count = 0
+        """Process the training failure reported by the node."""
+        node = self._job_nodes[node_type][node_id]
+        if restart_count >= 0:
+            self._error_monitor.handle_process_error(
+                node, restart_count, error_data
+            )
+        else:
+            self._error_monitor.handle_node_error(node, error_data)
+
+    def update_allreduce_node_unit(self, node_unit):
+        if isinstance(self._job_optimizer, AllreduceJobResourceOptimizer):
+            self._job_optimizer.set_node_unit(node_unit)
+
 
+def create_job_manager(args: JobArgs, speed_monitor) -> JobManager:
     critical_worker_index = get_critical_worker_index(args)
     # Custom distribution strategy does not exit if there are pending nodes
     wait_pending_relaunch = (
         args.distribution_strategy == DistributionStrategy.CUSTOM
     )
 
     elastic_job = new_elastic_job(args.platform, args.job_name, args.namespace)
     node_watcher = new_node_watcher(
         args.platform, args.job_name, args.namespace
     )
     job_scaler = new_job_scaler(args.platform, args.job_name, args.namespace)
 
-    return NodeManager(
+    return JobManager(
         job_args=args,
         critical_worker_index=critical_worker_index,
         wait_pending_relaunch=wait_pending_relaunch,
         speed_monitor=speed_monitor,
         job=elastic_job,
         node_watcher=node_watcher,
         job_scaler=job_scaler,
+        error_monitor=ErrorLogMonitor(),
     )
```

## Comparing `dlrover/python/tests/test_k8s_scaler.py` & `dlrover/python/tests/test_elasticjob_scaler.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,38 +13,80 @@
 
 import unittest
 
 from dlrover.python.common.constants import NodeType
 from dlrover.python.common.node import Node, NodeGroupResource, NodeResource
 from dlrover.python.master.scaler.base_scaler import ScalePlan
 from dlrover.python.master.scaler.elasticjob_scaler import ElasticJobScaler
+from dlrover.python.tests.test_utils import mock_k8s_client
 
 
-class k8sScalerTest(unittest.TestCase):
+class ElasticJobScalerTest(unittest.TestCase):
     def test_generate_scaler_crd_by_plan(self):
+        mock_k8s_client()
         plan = ScalePlan()
-        node_resource = NodeResource(10, 4096)
+        node_resource = NodeResource(
+            10, 4096, gpu_type="nvidia.com/gpu", gpu_num=1
+        )
         plan.launch_nodes.append(
             Node(
                 NodeType.WORKER,
                 0,
                 NodeResource(10, 4096, priority="low"),
                 rank_index=0,
+                name="test-worker-0",
+                service_addr="test-worker-0:2222",
+            )
+        )
+        plan.remove_nodes.append(
+            Node(
+                NodeType.WORKER,
+                1,
+                NodeResource(10, 4096, priority="low"),
+                rank_index=1,
+                name="test-worker-1",
+                service_addr="test-worker-1:2222",
             )
         )
+        plan.ps_addrs = ["test-ps-0:2222", "test-ps-1:2222"]
         group_resource = NodeGroupResource(1, node_resource)
         plan.node_group_resources["worker"] = group_resource
 
         scaler = ElasticJobScaler("test", "dlrover")
-        scaler_crd = scaler._generate_scaler_crd_by_plan(plan)
+        scaler_crd = scaler._generate_scale_plan_crd(plan)
 
         expected_dict = {
             "ownerJob": "test",
-            "replicaResourceSpec": {
+            "replicaResourceSpecs": {
                 "worker": {
                     "replicas": 1,
-                    "resource": {"cpu": "10", "memory": "4096Mi"},
+                    "resource": {
+                        "cpu": "10",
+                        "memory": "4096Mi",
+                        "nvidia.com/gpu": "1",
+                    },
                 }
             },
-            "nodeResourceSpec": {"cpu": "10", "memory": "4096Mi"},
+            "createPods": [
+                {
+                    "name": "test-worker-0",
+                    "type": "worker",
+                    "id": 0,
+                    "rankIndex": 0,
+                    "service": "test-worker-0:2222",
+                    "resource": {"cpu": "10", "memory": "4096Mi"},
+                }
+            ],
+            "removePods": [
+                {
+                    "name": "test-worker-1",
+                    "type": "worker",
+                    "id": 1,
+                    "rankIndex": 1,
+                    "service": "test-worker-1:2222",
+                    "resource": {"cpu": "10", "memory": "4096Mi"},
+                }
+            ],
+            "psHosts": ["test-ps-0:2222", "test-ps-1:2222"],
         }
+        print(scaler_crd.spec.to_dict())
         self.assertDictEqual(scaler_crd.spec.to_dict(), expected_dict)
```

## Comparing `dlrover/python/tests/test_node_manager.py` & `dlrover/python/tests/test_job_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,50 +7,53 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import time
 import unittest
 from unittest import mock
 
+from dlrover.proto import elastic_training_pb2
 from dlrover.python.common.constants import (
+    DistributionStrategy,
     JobExitReason,
     NodeEventType,
     NodeExitReason,
     NodeStatus,
     NodeType,
 )
 from dlrover.python.common.node import NodeGroupResource, NodeResource
 from dlrover.python.master.master import Master
 from dlrover.python.master.monitor.speed_monitor import SpeedMonitor
 from dlrover.python.master.node.event_callback import (
     ClusterContext,
     TaskRescheduleCallback,
     TFPSNodeHandlingCallback,
 )
-from dlrover.python.master.node.node_manager import create_node_manager
+from dlrover.python.master.node.job_manager import create_job_manager
 from dlrover.python.master.node.status_flow import (
     NODE_STATE_FLOWS,
     NodeStateFlow,
     get_node_state_flow,
 )
 from dlrover.python.master.node.training_node import (
     get_critical_worker_index,
     set_critical_node,
     update_nodes_priority,
 )
 from dlrover.python.master.resource.job import JobResource
-from dlrover.python.master.resource.optimizer import ResourcePlan
 from dlrover.python.master.watcher.base_watcher import Node, NodeEvent
 from dlrover.python.tests.test_utils import (
-    MockJobArgs,
+    MockK8sPSJobArgs,
     create_task_manager,
     mock_k8s_client,
+    new_dataset_splitter,
 )
 
 _MOCK_JOB_UUID = "11111"
 
 
 def get_service_fn(*args):
     return "test:2222"
@@ -61,35 +64,35 @@
 
 
 class NodeStatusFlowTest(unittest.TestCase):
     def test_get_node_state_flow(self):
         flow: NodeStateFlow = get_node_state_flow(
             NodeStatus.PENDING, NodeEventType.MODIFIED, NodeStatus.RUNNING
         )
-        self.assertEqual(flow, NODE_STATE_FLOWS[2])
+        self.assertEqual(flow, NODE_STATE_FLOWS[4])
 
         flow = get_node_state_flow(
             NodeStatus.RUNNING, NodeEventType.MODIFIED, NodeStatus.SUCCEEDED
         )
-        self.assertEqual(flow, NODE_STATE_FLOWS[5])
+        self.assertEqual(flow, NODE_STATE_FLOWS[7])
 
         flow = get_node_state_flow(
             NodeStatus.RUNNING, NodeEventType.DELETED, NodeStatus.DELETED
         )
-        self.assertEqual(flow, NODE_STATE_FLOWS[8])
+        self.assertEqual(flow, NODE_STATE_FLOWS[10])
         self.assertTrue(flow.should_relaunch)
 
         flow = get_node_state_flow(
             NodeStatus.SUCCEEDED, NodeEventType.DELETED, NodeStatus.DELETED
         )
         self.assertEqual(flow, NODE_STATE_FLOWS[-2])
         self.assertFalse(flow.should_relaunch)
 
 
-class JobConfigTest(unittest.TestCase):
+class JobManagerTest(unittest.TestCase):
     def setUp(self) -> None:
         mock_k8s_client()
 
     def test_job_resource(self):
         job = JobResource()
         job.node_group_resources[NodeType.PS] = NodeGroupResource(
             3, NodeResource(1, 4096)
@@ -161,29 +164,29 @@
         self.assertEqual(nodes[NodeType.PS][0].max_relaunch_count, 2)
         self.assertTrue(nodes[NodeType.WORKER][0].critical)
         self.assertEqual(nodes[NodeType.WORKER][0].max_relaunch_count, 3)
         self.assertTrue(nodes[NodeType.WORKER][0].critical)
         self.assertFalse(nodes[NodeType.WORKER][1].critical)
 
     def test_get_critical_worker_index(self):
-        params = MockJobArgs()
+        params = MockK8sPSJobArgs()
         params.initilize()
         critical_worker = get_critical_worker_index(params)
         self.assertDictEqual(critical_worker, {0: 3})
         params.node_args[NodeType.WORKER].critical_nodes = "0:1"
         critical_worker = get_critical_worker_index(params)
         self.assertDictEqual(critical_worker, {0: 1})
         params.node_args[NodeType.WORKER].critical_nodes = "all"
         critical_worker = get_critical_worker_index(params)
         self.assertDictEqual(critical_worker, {0: 3, 1: 3, 2: 3})
 
-    def test_create_node_manager(self):
-        params = MockJobArgs()
+    def test_create_job_manager(self):
+        params = MockK8sPSJobArgs()
         params.initilize()
-        manager = create_node_manager(params, SpeedMonitor())
+        manager = create_job_manager(params, SpeedMonitor())
         self.assertEqual(manager._ps_relaunch_max_num, 1)
         manager.start()
         self.assertEqual(manager._job_args.job_uuid, _MOCK_JOB_UUID)
         self.assertEqual(len(manager._job_nodes), 4)
         self.assertTrue(manager._job_nodes[NodeType.PS][0].critical)
 
         node = Node(
@@ -217,57 +220,93 @@
         should_relaunch = manager._should_relaunch(node, NODE_STATE_FLOWS[6])
         self.assertFalse(should_relaunch)
 
         node.exit_reason = NodeExitReason.FATAL_ERROR
         should_relaunch = manager._should_relaunch(node, NODE_STATE_FLOWS[6])
         self.assertFalse(should_relaunch)
 
+    def test_create_allreduce_job_manager(self):
+        params = MockK8sPSJobArgs()
+        params.initilize()
+        params.distribution_strategy = DistributionStrategy.ALLREDUCE
+        params.node_args.pop(NodeType.PS)
+        params.node_args.pop(NodeType.CHIEF)
+        params.node_args.pop(NodeType.EVALUATOR)
+        manager = create_job_manager(params, SpeedMonitor())
+        manager._job_optimizer.init_job_resource(manager._job_resource)
+        manager._adjust_worker_for_estimator()
+        manager._init_nodes()
+        manager._init_job_auto_scaler()
+        self.assertEqual(len(manager._job_nodes[NodeType.WORKER]), 3)
+        manager.start_auto_scaling()
+        self.assertEqual(len(manager._job_nodes[NodeType.WORKER]), 3)
+
     def test_recover_tasks_for_failed_workers(self):
-        dataset_name = "test"
-        task_manager = create_task_manager()
+        ds_name_0 = "test-0"
+        ds_name_1 = "test-1"
+        task_manager = create_task_manager(ds_name_0)
+        splitter = new_dataset_splitter(
+            False,
+            100,
+            1000,
+            1,
+            ds_name_1,
+            "table",
+        )
+        task_manager.new_dataset(
+            batch_size=10,
+            dataset_size=1000,
+            dataset_name=ds_name_1,
+            dataset_splitter=splitter,
+            task_type=elastic_training_pb2.EVALUATION,
+        )
+
         task_callback = TaskRescheduleCallback(task_manager)
-        params = MockJobArgs()
+        params = MockK8sPSJobArgs()
         params.initilize()
-        manager = create_node_manager(params, SpeedMonitor())
-        manager._init_job_nodes()
+        manager = create_job_manager(params, SpeedMonitor())
+        manager._init_nodes()
         manager.add_node_event_callback(task_callback)
 
-        dataset = task_manager.get_dataset(dataset_name)
-        task_manager.get_dataset_task(NodeType.WORKER, 0, dataset_name)
+        dataset_0 = task_manager.get_dataset(ds_name_0)
+        dataset_1 = task_manager.get_dataset(ds_name_1)
+        task_manager.get_dataset_task(NodeType.WORKER, 0, ds_name_0)
+        task_manager.get_dataset_task(NodeType.WORKER, 0, ds_name_1)
         node = Node(
             node_type=NodeType.WORKER,
             node_id=0,
             status=NodeStatus.RUNNING,
             config_resource=NodeResource(1, 4096),
         )
-        manager._process_node_events(NODE_STATE_FLOWS[7], node)
-        self.assertEqual(len(dataset.doing), 0)
+        manager._process_node_events(NODE_STATE_FLOWS[9], node)
+        self.assertEqual(len(dataset_0.doing), 0)
+        self.assertEqual(len(dataset_1.doing), 0)
 
     def test_create_initial_nodes(self):
-        params = MockJobArgs()
+        params = MockK8sPSJobArgs()
         params.initilize()
-        manager = create_node_manager(params, SpeedMonitor())
-        manager._init_job_nodes()
+        manager = create_job_manager(params, SpeedMonitor())
+        manager._init_nodes()
         plan = manager._create_initial_scale_plan()
         self.assertEqual(
             plan.ps_addrs,
             [
                 "test-edljob-ps-0.default.svc:2222",
                 "test-edljob-ps-1.default.svc:2222",
                 "test-edljob-ps-2.default.svc:2222",
             ],
         )
         self.assertEqual(plan.node_group_resources[NodeType.PS].count, 3)
         self.assertEqual(plan.node_group_resources[NodeType.WORKER].count, 3)
 
     def test_check_worker_status(self):
-        params = MockJobArgs()
+        params = MockK8sPSJobArgs()
         params.initilize()
-        manager = create_node_manager(params, SpeedMonitor())
-        manager._init_job_nodes()
+        manager = create_job_manager(params, SpeedMonitor())
+        manager._init_nodes()
         self.assertFalse(manager.all_workers_exited())
 
         for worker in manager._job_nodes[NodeType.WORKER].values():
             worker.status = NodeStatus.FINISHED
         for worker in manager._job_nodes[NodeType.CHIEF].values():
             worker.status = NodeStatus.FINISHED
         for worker in manager._job_nodes[NodeType.EVALUATOR].values():
@@ -286,59 +325,48 @@
             worker.status = NodeStatus.FINISHED
         manager._job_nodes[NodeType.WORKER][0].status = NodeStatus.RUNNING
         self.assertFalse(manager.all_critical_node_completed())
         manager._job_nodes[NodeType.WORKER][0].status = NodeStatus.FINISHED
         self.assertTrue(manager.all_critical_node_completed())
 
     def test_tf_ps_node_handling(self):
-        params = MockJobArgs()
+        params = MockK8sPSJobArgs()
         params.initilize()
         master = Master(2222, params)
-        master.node_manager._init_job_nodes()
-        master.node_manager._scaler.scale = mock.MagicMock(return_value=True)
+        master.job_manager._init_nodes()
+        master.job_manager._scaler.scale = mock.MagicMock(return_value=True)
         callback = TFPSNodeHandlingCallback(master)
 
         node = Node(NodeType.PS, 0, None)
+        node.config_resource = NodeResource(1, 10240)
         node.exit_reason = NodeExitReason.OOM
         reason = callback.get_job_exit_reason(node)
         self.assertEqual(reason, JobExitReason.PS_OOM_ERROR)
 
         node.type = NodeType.WORKER
         reason = callback.get_job_exit_reason(node)
         self.assertEqual(reason, JobExitReason.CODE_ERROR)
 
         master.speed_monitor.add_running_worker(NodeType.WORKER, 0)
         master.speed_monitor.add_running_worker(NodeType.WORKER, 1)
-        cluster_context = ClusterContext(master.node_manager)
+        cluster_context = ClusterContext(master.job_manager)
         master.speed_monitor.set_target_worker_num(2)
         node.exit_reason = NodeExitReason.FATAL_ERROR
         callback.on_node_failed(node, cluster_context)
         self.assertEqual(master.speed_monitor._target_worker_num, 1)
         self.assertEqual(len(master.speed_monitor.running_workers), 1)
 
-    def test_execute_job_optimization_plan(self):
-        params = MockJobArgs()
+    def test_all_running_node_hang(self):
+        params = MockK8sPSJobArgs()
         params.initilize()
-        manager = create_node_manager(params, SpeedMonitor())
-        manager._init_job_nodes()
+        manager = create_job_manager(params, SpeedMonitor())
+        manager._init_nodes()
 
-        manager._scaler.scale = mock.MagicMock(return_value=True)
-        plan = ResourcePlan()
-        plan.node_group_resources[NodeType.WORKER] = NodeGroupResource(
-            6, NodeResource(4, 4096)
-        )
-        plan.node_resources["test-edljob-worker-0"] = NodeResource(8, 8192)
-        plan.node_resources["test-edljob-ps-1"] = NodeResource(8, 8192)
-        manager._ps_manager._nodes[1].status = NodeStatus.RUNNING
-        scale_plan = manager._execute_job_optimization_plan(plan)
-        self.assertEqual(len(manager._ps_manager._nodes), 4)
-        self.assertEqual(len(manager._worker_manager._nodes), 7)
-        self.assertEqual(
-            scale_plan.node_group_resources[NodeType.WORKER].count, 6
-        )
-        self.assertEqual(len(scale_plan.remove_nodes), 1)
-        self.assertEqual(len(scale_plan.launch_nodes), 2)
+        hang = manager.all_running_node_hanged()
+        self.assertFalse(hang)
 
-        ps_addrs = []
-        for i in [0, 3, 2]:
-            ps_addrs.append("test-edljob-ps-{}.default.svc:2222".format(i))
-        self.assertListEqual(scale_plan.ps_addrs, ps_addrs)
+        for _, nodes in manager._job_nodes.items():
+            for _, node in nodes.items():
+                node.start_hang_time = time.time() - 3600 * 4
+                node.status = NodeStatus.RUNNING
+        hang = manager.all_running_node_hanged()
+        self.assertTrue(hang)
```

## Comparing `dlrover/trainer/examples/__init__.py` & `dlrover/python/elastic_agent/sychronization/__init__.py`

 * *Files identical despite different names*

## Comparing `dlrover/trainer/examples/estimator_executor/__init__.py` & `dlrover/python/elastic_agent/torch/__init__.py`

 * *Files identical despite different names*

## Comparing `dlrover/trainer/tensorflow/reader/fake_reader.py` & `dlrover/trainer/tensorflow/reader/base_reader.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,79 +6,90 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import numpy as np
+
+from abc import ABCMeta, abstractmethod
 
 from dlrover.python.elastic_agent.sharding.client import ShardingClient
+from dlrover.trainer.util.log_util import default_logger as logger
 
 
-def build_data_shard_service(
+def build_sharding_client(
     batch_size=1,
     num_epochs=1,
     dataset_size=1,
     num_minibatches_per_shard=1,
-    dataset_name="iris_training_data",
+    dataset_name="training_data",
 ):
     sharding_client = ShardingClient(
         dataset_name=dataset_name,
         batch_size=batch_size,
         num_epochs=num_epochs,
         dataset_size=dataset_size,
         num_minibatches_per_shard=num_minibatches_per_shard,
     )
     return sharding_client
 
 
-class FakeReader:
+class ElasticReader(metaclass=ABCMeta):
     def __init__(
-        self, num_epochs=1, batch_size=64, enable_dynamic_sharding=True
+        self,
+        path=None,
     ):
+        self._path = path
+        self.enable_dynamic_sharding = True
+        self.num_minibatches_per_shard = 10
+
+    def set_path(self, path):
+        self._path = path
 
+    def set_num_epochs(self, num_epochs):
         self._num_epochs = num_epochs
+
+    def set_batch_size(self, batch_size):
         self._batch_size = batch_size
-        self.enable_dynamic_sharding = enable_dynamic_sharding
-        self.data_shard_service = None
-        self.count_data()
-        self.data_shard_client = None
-        self._consumed_data = 0
-        self.build_data_shard_client()
 
-    def build_data_shard_client(self):
+    def set_enable_dynamic_sharding(self, enable_dynamic_sharding):
+        self._enable_dynamic_sharding = enable_dynamic_sharding
+
+    def set_num_minibatches_per_shard(self, num_minibatches_per_shard):
+        self._num_minibatches_per_shard = num_minibatches_per_shard
+
+    def build_sharding_client(self):
+        self.count_data()
         if self.enable_dynamic_sharding is True:
-            self.data_shard_client = build_data_shard_service(
+            logger.info(
+                "Build data shard client in file reader: \n \
+                            num_epochs {} \n\
+                            batch_size {} \n\
+                            data_nums {}".format(
+                    self._num_epochs, self._batch_size, self._data_nums
+                )
+            )
+            self.data_shard_client = build_sharding_client(
                 batch_size=self._batch_size,
-                num_epochs=1,
+                num_epochs=self._num_epochs,
                 dataset_size=self._data_nums,
-                num_minibatches_per_shard=1,
-                dataset_name="iris_training_data",
+                num_minibatches_per_shard=2,
+                dataset_name=self._path,
             )
 
-    def count_data(self):
-        self._data_nums = 10000
-
-    def get_default_shard(self):
-        return 1
+    @abstractmethod
+    def read_data_by_index_range(self, start_index, end_index):
+        pass
 
-    def _read_data(self):
-        shard = None
-        if self.data_shard_client is not None:
-            shard = self.data_shard_client.fetch_shard()
-        data = self.get_data_by_shard(shard)
-        if shard is None:
-            data = None
-        return data
-
-    def get_data_by_shard(self, shard):
-        x = np.random.randint(1, 1000)
-        y = 2 * x + np.random.randint(1, 5)
-        return "{},{}".format(x, y)
+    @abstractmethod
+    def count_data(self):
+        pass
 
     def iterator(self):
         while True:
-            data = self._read_data()
-            if data is None:
+            shard = self.data_shard_client.fetch_shard()
+            if not shard:
                 break
-            yield data
+            logger.info("shard is {}".format(shard))
+            for d in self.read_data_by_index_range(shard.start, shard.end):
+                yield d
```

## Comparing `dlrover-0.1.0rc0.dev1.dist-info/LICENSE` & `dlrover-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dlrover-0.1.0rc0.dev1.dist-info/RECORD` & `dlrover-0.2.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,149 +1,191 @@
 dlrover/Makefile,sha256=gWX_j-z6M1UP3-h331dG--ZiwVIfLORm69qwof9Ke84,411
 dlrover/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
-dlrover/requirements.txt,sha256=EsTcv0u7SyxFeGfNGIJfKIeGjxlFbNYp7czgaF1TgwM,70
-dlrover/proto/brain.proto,sha256=ygAoEnwxd0--gW8KIxy5MR2zTCQpzTKPxx3KkpIH0vA,4440
-dlrover/proto/brain_pb2.py,sha256=3iyZDWxE8kuNLd3QQld8Rbii8p04q4ep6-I2t3ieQrg,23048
+dlrover/proto/brain.proto,sha256=HGeQp7U1BzaosYfGKjqviFhUAXIqTx9_mWET-kpi1aQ,4439
+dlrover/proto/brain_pb2.py,sha256=de1Blgbno6aQmXTEw4VTP-3MfhsVPlxv2llghGDkgIc,92639
 dlrover/proto/brain_pb2_grpc.py,sha256=uuc2uMH2lIv4J2RTkTuPPHBUg0xBdm9knKcWLVV7JlI,5867
-dlrover/proto/elastic_training.proto,sha256=yRdbx_GdPOIuRxzsu5aQwmEfhf1vBE87JsOp0bCL9nU,7206
-dlrover/proto/elastic_training_pb2.py,sha256=bj6R2N31P3AZ4BcvSdJIAJU64MCL8TqZAz5tP4ikSps,28522
-dlrover/proto/elastic_training_pb2_grpc.py,sha256=JbtEb1UIdLJwSH1o9JOe2LJ9glSV-TvxRhNW1dNc0Uk,40617
+dlrover/proto/elastic_training.proto,sha256=DSeHAzriI2eqDGmgVZm8mqBfVxiCMKoCU4W91OjVTBw,7729
+dlrover/proto/elastic_training_pb2.py,sha256=4JISB0LmIJnonw68jzNfAwz15Ivy4GMlurAqDV6tVR0,105858
+dlrover/proto/elastic_training_pb2_grpc.py,sha256=PKcwlaMPFKcv9pHECQoTbggImTWc5oay3c6JUcQFlvI,57297
 dlrover/python/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/brain/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
-dlrover/python/brain/client.py,sha256=OtI8DwEPhdS8EqjrmSVLmVMQPgDPgaGqmXkpoFXS_xY,10825
+dlrover/python/brain/client.py,sha256=tSNrXo9OPoru0VdIv4E5-Fn8aNsMTQ9DBUQNOjn0wyM,11185
 dlrover/python/common/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
-dlrover/python/common/constants.py,sha256=yPaAPvH6f1W7rBpS1e-S7L_qSCiSblbc8oxIR6pRc_c,4215
-dlrover/python/common/global_context.py,sha256=03UxtTfk3L6_Stqq_cdSU5Pj3ypCU00Pj94bAn9c5w8,4944
-dlrover/python/common/grpc.py,sha256=topZ-EeZV_TBdbHD8skawd9R9I4ZhEgvYXCviqbz80Y,1598
+dlrover/python/common/constants.py,sha256=02wOadv2hZB5RMPPp0mVYKN5w7g2W2rfSrBoYH5GAsY,5625
+dlrover/python/common/global_context.py,sha256=jdQH5fySuSEvKeLfbJRzAQbh5F7tmmmsgHm83nT6WBA,5873
+dlrover/python/common/grpc.py,sha256=h8NSH_g0k8RxthhY1LTb4l9keNhhJ4Liq5VTdnMZeGo,2182
 dlrover/python/common/log.py,sha256=N1qzo8yLgeDc9e50RCVgRfZpkSB-cX__nIiGFS7rQ2Y,1344
-dlrover/python/common/node.py,sha256=VbFAk5B43-ScWNGp8lBYqLa0Doit5b8YZ8EFW_CRGsg,8093
+dlrover/python/common/node.py,sha256=8EVJ5a67JVst6NS5U5F8BOlEoNzqpufpD9OrJVjV5Uc,9732
 dlrover/python/common/serialize.py,sha256=-EJivQ_QRocjctm0s_95eDxLtOsZCt1Vp0EwSzhnxLc,923
 dlrover/python/common/singleton.py,sha256=EAVohnN6bci_uQKvapIpfFam8K5wihc5nuNsxH5Nm1I,905
 dlrover/python/elastic_agent/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
-dlrover/python/elastic_agent/master_client.py,sha256=7Nvm_ImU87fiSZhTKkhYlNpGN4Ty09DRHPIJ8a5ozI4,16066
+dlrover/python/elastic_agent/master_client.py,sha256=ALkDd3M7Y-pexm04m_iF0yAK4M_zh-jwV-n1E0KLkb4,20421
 dlrover/python/elastic_agent/monitor/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
-dlrover/python/elastic_agent/monitor/resource.py,sha256=EYgNIv8ItaFULuM3Hq7LwSzC-fTuuxb_u6q0x_RGees,3154
-dlrover/python/elastic_agent/monitor/training.py,sha256=EzXSlDTloTte6rYONvMqWr3slMGOLtxGIS9TIMxmgpc,2483
+dlrover/python/elastic_agent/monitor/resource.py,sha256=sZduHUOF6kymEhjkK0ZVA55_gBixXV5h5-I-Z0xJlcY,3264
+dlrover/python/elastic_agent/monitor/training.py,sha256=hw-PTEsqAnu8LKfrtLOXGRXpWeSr2Hb3nk0ryMO32po,2489
 dlrover/python/elastic_agent/sharding/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
-dlrover/python/elastic_agent/sharding/client.py,sha256=SPavUU4HQMH3tu_cLXoUG2JiWgKfMXFTkxsUFTxWBSU,6983
+dlrover/python/elastic_agent/sharding/client.py,sha256=zCVgMdpg6fbvg3cuR2K5qd2T4m150gDBDeXyvXjBFJ4,12227
+dlrover/python/elastic_agent/sychronization/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
+dlrover/python/elastic_agent/sychronization/sync_client.py,sha256=HwqYpcto-3tImI_K9YcpLpdgrLPV0Dt_FXY9wUOBUuk,2699
 dlrover/python/elastic_agent/tensorflow/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/elastic_agent/tensorflow/elastic_ps.py,sha256=y2Qaeej-BLajBHw-baUqrotGpTrvLnQkshy7XxgrgIM,3397
-dlrover/python/elastic_agent/tensorflow/hooks.py,sha256=T9vIxr6yEXWLP9UocvQdA_AnRC-YH9qzBMeVkmbzQlE,3932
+dlrover/python/elastic_agent/tensorflow/hooks.py,sha256=279J7GhyZkOeeOquUFYRPXNNDtOZISJTRzn-zWuiwPA,3930
 dlrover/python/elastic_agent/tensorflow/profile_extractor.py,sha256=N7MsELFbfraXR9SY70XsE7v1T58CQUXbdCebRvyp6UQ,4556
+dlrover/python/elastic_agent/torch/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
+dlrover/python/elastic_agent/torch/master_kv_store.py,sha256=MQ84y98gsuuS-8CdAKFgRNKtEiC9UJhiL2hKdNDq2S0,4599
+dlrover/python/elastic_agent/torch/training.py,sha256=lUDLQc8mwfAQA_vK0lCRmfu7p7xV_AYLOY5dwRgweWc,26917
 dlrover/python/master/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
-dlrover/python/master/args.py,sha256=7ooN7Av48yj8kd5BRfrNFT-xYaps4PdWrBaJSsKIASs,2879
-dlrover/python/master/main.py,sha256=2xQbO0QsWg_rxKSkkKle7ZEy7x0XZiXr0wtNZY7UR5A,1827
-dlrover/python/master/master.py,sha256=D8oXGOkitTKBmaSS6LmNp_Dg6sqvwBg4hsDiE2gJL7A,7564
-dlrover/python/master/servicer.py,sha256=9nD5HMAYBAQfLBKCyqHq75uBGpTTUeYa0XzO0bJR21Y,16440
+dlrover/python/master/args.py,sha256=9khqeDu_doOGtky_F3Q7lsCI9cMZBkQAprG2y4RCpEE,3114
+dlrover/python/master/main.py,sha256=VGAq_KQEtxRBQe0GcGNrwWBWr1j2Nq94XRKUFErV1ng,1960
+dlrover/python/master/master.py,sha256=QQvNCME3GF__1oS8igy4RyC7Kw1NcgfY1-UqN83NOLc,8650
+dlrover/python/master/servicer.py,sha256=zMlY77lRczRyl-uSShT-u37k_SGQ4tISTTMO7kBlv8Q,18494
+dlrover/python/master/cluster/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
+dlrover/python/master/cluster/quota.py,sha256=Kfzb8B1gV7xZXkwsGaiIjISDH9Q0mh1DqNLSBZzTWnw,1124
 dlrover/python/master/elastic_training/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
-dlrover/python/master/elastic_training/elastic_ps.py,sha256=K3Jv6QfDkOM_qMZ0AsJZJwO0J8wnwDY9E1fCthrencE,3414
+dlrover/python/master/elastic_training/elastic_ps.py,sha256=rhplRZ7sfT6hUDD1mPvI8Gpqy8M2RgaFqCI874pQ56Y,3494
+dlrover/python/master/elastic_training/kv_store_service.py,sha256=TTSz8pCc2wifmG_ecUREPDYFwcBgBm97H0G4n8Ta4xA,1017
+dlrover/python/master/elastic_training/rdzv_manager.py,sha256=nLfqWz7rEbMNnjDiXPX8LjtgbEE8ElIpq2qwT-hmvxU,14853
+dlrover/python/master/elastic_training/sync_service.py,sha256=rlY-4VL4SlPo5TXP_SnuO-9GfvWz9fQ7_FIusp1nT_g,4944
 dlrover/python/master/monitor/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
-dlrover/python/master/monitor/speed_monitor.py,sha256=2kTzycgWjO3vczybeXJaPqs7HwpROu2IgliqMoNIhfI,5779
+dlrover/python/master/monitor/error_monitor.py,sha256=HrOzWA1V_HCgezn0ijQhvUeYlu_epA9jRQBggdd2YqI,1864
+dlrover/python/master/monitor/speed_monitor.py,sha256=0COdFCfEEc87vNFY-hWXP_NPNKVsHQSf3LMNo1AetXg,7002
 dlrover/python/master/node/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
-dlrover/python/master/node/event_callback.py,sha256=cNn6dQnfANz9mtX65ETVlnvEgNGkJC1Pt-112Gfcq1Q,7190
-dlrover/python/master/node/node_manager.py,sha256=3WArZ78216pL-QvAk2oatIAp6YnyRMbolA6srDnoNZ0,26929
-dlrover/python/master/node/ps.py,sha256=dPopLYWi8TZsxElBHThRwBvlkUCcWp0SCP3COijVLUQ,13412
-dlrover/python/master/node/status_flow.py,sha256=kBm_Nb4eo4TfS6bkkEoy-KtfVEmOHdTp3-BSkphNkbc,3663
-dlrover/python/master/node/training_node.py,sha256=p95JaR-6TXEwuEJ8S50FkOmdrP3ztG96OwUAnvMp4XQ,9557
-dlrover/python/master/node/worker.py,sha256=ikVxwWQ648tpCjuNs4QbWjgRMi0AZOqkWZuZ48DLPrY,8970
+dlrover/python/master/node/event_callback.py,sha256=frp-GXUfGrHS35Uvik8P2WXJ-dF07ObwfR7PzNY8zYs,11103
+dlrover/python/master/node/job_auto_scaler.py,sha256=gG0UaeoxCrJIi2O9tBkZi_f7Jsy4eo_-I50rLrN3DkU,11844
+dlrover/python/master/node/job_manager.py,sha256=_TEurcQ6N4lw_rU1BU3plvb4huylbxSm4R1UqCkPFxQ,26844
+dlrover/python/master/node/ps.py,sha256=GScdKk8uIuj2LDzPcXg_vkVNc1H3GF7y0bIAPgPPD50,14460
+dlrover/python/master/node/status_flow.py,sha256=kDMCbErbvTdh9lw-wp6ImHUp2eD7OTDilGI_zs7wYKg,4046
+dlrover/python/master/node/training_node.py,sha256=FuNRlOmO9sCq1iosX5VSIToo-GfBz9L0MkKeQO47KMk,11531
+dlrover/python/master/node/worker.py,sha256=t8qwUngv51PGuah1gAMtO05_zkKrGG3zuBIGx_-TM6I,10616
 dlrover/python/master/resource/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
-dlrover/python/master/resource/brain_optimizer.py,sha256=dBSGftP1B-zbfWyUKOdSf02bjMgaKeICz0fMeCNWCoo,4153
-dlrover/python/master/resource/job.py,sha256=bBEkuqrmBgZnT18HN2E0w8hnbTvMUlCScyvlZGUUzwI,16950
-dlrover/python/master/resource/local_optimizer.py,sha256=LpuCz6JfjFAA7LVfPqBCzClouMNWDcGoTAT_jP4rkew,13010
-dlrover/python/master/resource/optimizer.py,sha256=bmUuhDw06qCQpsX4WikYXQ6BzpMAiSuQ34ABgGLdS1c,5349
+dlrover/python/master/resource/brain_optimizer.py,sha256=KPJICeSkW-aS7ci3o4Mv6pg2lnNBsBqqfi1jKuNuzg0,4187
+dlrover/python/master/resource/job.py,sha256=jWgyjwhbmXIPk7IjvG5eTW6rPezsQap2QjAYXwjgli8,20985
+dlrover/python/master/resource/local_optimizer.py,sha256=M6GM9nmf34EwMZMYhaJqjouZIGO1DPqXUlAEtgrva54,15717
+dlrover/python/master/resource/optimizer.py,sha256=LAjP6CXSyp3YkfGUDTcEG9cQRzWU4IEmvU6BU5xic1E,6065
 dlrover/python/master/scaler/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
-dlrover/python/master/scaler/base_scaler.py,sha256=PxHFX8klME0tA8dCVzsKNPnkEdJluIlwFNgOjXfi7aQ,1994
-dlrover/python/master/scaler/elasticjob_scaler.py,sha256=gu3KwYeX4FDTqQ9cXSeNug4LLoqHo8ps83ZlGXWVweQ,5562
-dlrover/python/master/scaler/factory.py,sha256=d6niz_ILHcQZ77i2vbi-ZuhHfRmAE1jdFRysHuMRG14,1149
-dlrover/python/master/scaler/pod_scaler.py,sha256=vwVFg7ZKw8GHitTesQZ9q_DM53PeuBbz2t-bpSf_mA0,21985
+dlrover/python/master/scaler/base_scaler.py,sha256=_KjPuz42oSTBZ_kjLA-BBrEtTq9t2zg9jpHn9bsWnyc,2062
+dlrover/python/master/scaler/elasticjob_scaler.py,sha256=rn5vLH1DKS9OqQE3pXUt-vaS_Oc52qroJPiA58PRgsY,8519
+dlrover/python/master/scaler/factory.py,sha256=gwwz1F7G_VwvcB2LKoF7QMMq9d31Hurr6VbPtmzVrEk,1300
+dlrover/python/master/scaler/pod_scaler.py,sha256=OjwP9unaiFJ8hCd01ApfYpNy2rnwrpQe2PeOXhOMGuc,23329
+dlrover/python/master/scaler/ray_scaler.py,sha256=sDElDKVj-kIXi1ewD4KEJhDvM6azY41Wg6DuwME4uF0,4670
 dlrover/python/master/shard/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
-dlrover/python/master/shard/base_dataset_manager.py,sha256=XNAFWPHiJfPquuy1lpWviKoFUnEq0Uu-WR8Y722Riak,4304
-dlrover/python/master/shard/batch_dataset_manager.py,sha256=j60eufoudt5s1ZBnuPQ9e1GNJVTiYV6WhsYjKn6iRP8,6345
-dlrover/python/master/shard/dataset_splitter.py,sha256=6iviIN04Zw4ane6ESW0l_TRqFj72ivHhycR_X_HLXVA,15618
+dlrover/python/master/shard/base_dataset_manager.py,sha256=3jQ-kWrffGsGiCUE6_iLh9aug4GXVja-iWjM4lWcZaQ,4574
+dlrover/python/master/shard/batch_dataset_manager.py,sha256=mD8TEi-yww-4G7cTwL-9irEul49twD2HdRk-Y-_4KEw,6964
+dlrover/python/master/shard/dataset_splitter.py,sha256=1l_CCvLrxGfQU0gQWPx1PVZKIFgMl0pGNE8EkWaES4U,15928
 dlrover/python/master/shard/streaming_dataset_manager.py,sha256=vr_-JNbzwR0BkK2g1WIAuIwZXWaJCU6EtYI6EDVm1ZM,7064
-dlrover/python/master/shard/task_manager.py,sha256=sXxliyejzYviOAZbf3qFjxfh3Seeoi3lFjHJTqDX6v0,9505
+dlrover/python/master/shard/task_manager.py,sha256=jJKZrhT4xr_8CM13uSBsH6xX3DC7TxAxG8ptu80UCLY,10773
 dlrover/python/master/stats/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
-dlrover/python/master/stats/job_collector.py,sha256=V-bvVIbz7jqnFuZf2pCERfdKA0gN-gxAWSz968Egy64,6394
-dlrover/python/master/stats/reporter.py,sha256=wUWvFfFt3tlpgDa5a2oB9EVHMhxa783KKM-6hvKTosA,3484
-dlrover/python/master/stats/training_metrics.py,sha256=z5-dXzp_VfBbNqoA5O29ILCMiKtduusqAkFGSs4r0KQ,4344
+dlrover/python/master/stats/job_collector.py,sha256=Ml_5p1Mlmr_YyOftTNeRuibGSUjjHsGr2_e8rKlbsAo,6557
+dlrover/python/master/stats/reporter.py,sha256=qsBDYM-bVTzy1ShqRD0d8L2JbCdBmjd0vM7sA4968Ro,8730
+dlrover/python/master/stats/stats_backend.py,sha256=iJGkngsGLkXEWdN_2jv9xSfELrzpA2ow4Nle93WE4cQ,1567
+dlrover/python/master/stats/training_metrics.py,sha256=-3PjCD419-D0XIWXidVFbqmX2uLYKmePkTo58L7whMo,4416
 dlrover/python/master/watcher/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/python/master/watcher/base_watcher.py,sha256=OZkgRItgEMNC53hv59ciNKNc8fSKzX016zRIrINF0vQ,1241
-dlrover/python/master/watcher/factory.py,sha256=O3mIpRrLwJ7dacVcqSDbT2jLe3gye5HcabXIUtVtNCo,1079
-dlrover/python/master/watcher/pod_watcher.py,sha256=awL3D--hE9lZj6AlmatVjQoThlKDCSMOTl1jxadt_no,5727
+dlrover/python/master/watcher/factory.py,sha256=2eMeOuf7RtLmezAHM8-U7QPRTIIzAo_JTWexp62ZF1s,1740
+dlrover/python/master/watcher/k8s_watcher.py,sha256=S207AnCm5RMa-IAmHI2sVJYvqvm9enciTchIFfkjPVY,10539
+dlrover/python/master/watcher/ray_watcher.py,sha256=GvQIuXBjiMBY1SeyjzKeFlvFCJ6tOC9pKRnTRzIT9lE,3247
 dlrover/python/scheduler/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
-dlrover/python/scheduler/factory.py,sha256=LmmdSQUtaTWOkBO6yt7lm1P-nZVKFHCSVswJ8hsEcPM,1393
-dlrover/python/scheduler/job.py,sha256=lHYUUFul_jo1AD6YT-hZ3CiHudgwS7U0MFxj0FPV5xM,3458
-dlrover/python/scheduler/kubernetes.py,sha256=hB3Il2qbB0qsEHX10Fy7Gt7Bf3ws-viSdq4SHpbaCkM,12081
-dlrover/python/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+dlrover/python/scheduler/factory.py,sha256=_vXe-ztsIaNMMchye1V07o8LZBWamYyKgLxtxQAjamI,1649
+dlrover/python/scheduler/job.py,sha256=MQ5C2xYPrqLaBrNG06P3QW5lNKSNWAxbL2yKhGFioxg,3439
+dlrover/python/scheduler/kubernetes.py,sha256=r8wgMgaicIvIj7Ngv7jXx3Nz1_iLDoRQQqISUppjIT8,12928
+dlrover/python/scheduler/ray.py,sha256=U6Am9Pt5GPy90HEqlRFptj02ShF-oixfR0x6XOqfA7g,7317
+dlrover/python/tests/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
 dlrover/python/tests/test_agent_monitor.py,sha256=LKJguGlABTVW84dsdZpl5U4X83vJPjwVucaTskyp7pQ,1668
 dlrover/python/tests/test_args.py,sha256=xq0ZkOq0wXdyvjuQppwj8GPR0XmjAUFFcb8GmPe2l4I,1049
-dlrover/python/tests/test_dataset_splitter.py,sha256=n3mxlxhp4_BrhufPfZZUwdqqiopXeUrapuWWQhHnkks,4595
-dlrover/python/tests/test_dataset_task_manager.py,sha256=MYDuKs8AOsE1A8edqnz-QHd318bjIUcNN7fbGwr7hV4,3008
-dlrover/python/tests/test_job_params.py,sha256=cqSoHFqpk6YQDgWP5J7PyupIA1qL4uoWS9zO_kenrpA,2160
-dlrover/python/tests/test_k8s_scaler.py,sha256=saokOI9KS74d0R9HKucbUMaJyi7_xwwEcLo6f9-sny8,1909
-dlrover/python/tests/test_local_optimizer.py,sha256=iMVvIu2Es9Nw5bqDA7Svr9zNZzd9z2wdYChcIItDwC4,6830
-dlrover/python/tests/test_master.py,sha256=5cE7lpPVzGZgG60iQ_p7IKQD3WNMVgT0ejcsABjIQjM,2751
-dlrover/python/tests/test_node_manager.py,sha256=D_XwaQpoYwN5DWR6esl-SogDS3kVi1thXS_Asq5imL0,13885
+dlrover/python/tests/test_dataset_splitter.py,sha256=CMgknANQ_cTLCrYljv1mK_QZZIzV10_dQx6_n81PYJg,4582
+dlrover/python/tests/test_dataset_task_manager.py,sha256=daafnt5eWt74min0XKIbbY_wUZHZe38jLZHbAeW3swA,4904
+dlrover/python/tests/test_elastic_training_agent.py,sha256=zGwO8xJF50ZHKpzFjH9gboLLLzuBUTvr1wHc-a4RbGc,4648
+dlrover/python/tests/test_elasticjob_scaler.py,sha256=PtaPEj98S6Uq8C24wyQVZWo7IPmW9RRcEFDT2MrwwDE,3359
+dlrover/python/tests/test_grpc_utils.py,sha256=E3mvhSY7ks2ZAyLu9Cpy-wM8MTqBryXOGNiDJ0MlSoM,978
+dlrover/python/tests/test_job_auto_scaler.py,sha256=PK2I_58x5duRoOHq3K0BDY_qie06VzN6XtKTNnTIIhI,3617
+dlrover/python/tests/test_job_manager.py,sha256=821dMsqAWM3FObDqEgM7hiiRl1lcYADX2We3H_aK3QI,14675
+dlrover/python/tests/test_job_params.py,sha256=ouzep9CuB-GbObbm6FYjncH7UtMCMHNOjP3treijyOs,2134
+dlrover/python/tests/test_k8s_watcher.py,sha256=w35cWdCfEnCCqarm9FROrCqNHw0DdgLI7WpCDmV2250,5302
+dlrover/python/tests/test_local_optimizer.py,sha256=zWxeVAVw8GRJ0NRMC44z2y6njlg_kk1mPfLSgNaRpWA,9139
+dlrover/python/tests/test_master.py,sha256=W6ZiCWxcSKEuNg5HICPVBq6W2t_aoCdtU-N_JC9f8S4,2792
 dlrover/python/tests/test_node_watcher.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
-dlrover/python/tests/test_pod_scaler.py,sha256=UQEX9oFBwPsCT4TfQX2yWT6nOnBdBcQKHW6KjKYtMVA,5491
-dlrover/python/tests/test_pod_watcher.py,sha256=iYsp-oVgdXA9kGNVpG227-oeVdmQ9HivtcTBkQJKgyA,3707
-dlrover/python/tests/test_ps_manager.py,sha256=sEh4SQ2Ri7nAdMT3p2Rc5_R6sRty7ZrUneijmXn3dfQ,6234
-dlrover/python/tests/test_resource_optimizer.py,sha256=Vhk_qTlbAuYo2X3Ea8cuTh8UkfO79THL0S_S4Yibl28,8459
-dlrover/python/tests/test_servicer.py,sha256=XGOIANA7ZUrbOuFYKEtUtnufwb0eWsDLtA-nLJ2PX6s,6434
-dlrover/python/tests/test_sharding_client.py,sha256=4rUbhPFvAiC-UZ9Up0tuGDY7C6y3p9502XJ-HzMTExY,1932
-dlrover/python/tests/test_speed_monitor.py,sha256=42X4TCyyvac-ZzZ9kTQmQ5pK2UOxFUoo3iZwYJojh5s,1482
-dlrover/python/tests/test_stats_collector.py,sha256=-G3wnNML9EyjgRxV9lHt5_Bw6WuWCIJKW_LvhuQ0B8o,2254
-dlrover/python/tests/test_task_manager.py,sha256=5Hr081xuG_6_jBJBwX20avGJLejg4fG_ELADDFjI7DQ,4136
-dlrover/python/tests/test_utils.py,sha256=OT36s2j0ZRM1r2dOs7m924VoKqZ2ZxdG3Y5xxGcj0PQ,5866
-dlrover/python/tests/test_worker_manager.py,sha256=6LskTcvrbfY37AW0OG5bLPRq4eWH_V6oX7lAn8daC68,4379
+dlrover/python/tests/test_pod_scaler.py,sha256=ubySogMP0SAm3s3Chi1Rpd-azP2lNXFppP80405BSB4,7346
+dlrover/python/tests/test_ps_manager.py,sha256=wZw2HzhZEoxwZq5C4OqFo-wJlg6KZOgH_12mc5b7rs8,7402
+dlrover/python/tests/test_ray_client.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
+dlrover/python/tests/test_ray_job_args.py,sha256=Eeaeive9sZv6iyaSI4ksoH0qpZEGfBnHL4iS_JuE0Qs,1837
+dlrover/python/tests/test_ray_scaler.py,sha256=DFdUZIeB2I1wOWUl0o6FY2pqeEryVPTza6rLmr41EU4,970
+dlrover/python/tests/test_ray_watcher.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
+dlrover/python/tests/test_rdzv_manager.py,sha256=BgpmZS239o9vUXnD5y0iKiHQi5XHsKHkPOz-O1ukhYk,7095
+dlrover/python/tests/test_resource_optimizer.py,sha256=7elD8qAX7Fvo5hBN8CskMzJk2PlElUO1-EWvTHUbcQ4,10021
+dlrover/python/tests/test_servicer.py,sha256=ygHWmA9gnZX6ktV7rTZqn6krEquFC5w4hCSWIpH4_oc,9209
+dlrover/python/tests/test_sharding_client.py,sha256=DOZ5DhEvgIMMr_MusTkVwkgb972N7fFoRscOcKjTrxs,2552
+dlrover/python/tests/test_speed_monitor.py,sha256=BiZ--uSvxVs_NwOoxFG2Owk7O1p5mn5ese9zkvVQHVQ,1782
+dlrover/python/tests/test_state_backend.py,sha256=uocRJZWt1RjcTshOYfseUUiT9Bl9x_7dSNI3cvExJPs,1344
+dlrover/python/tests/test_stats_collector.py,sha256=nsiaHHPKIcodwWtRUCoA3BBSqXVwM79z-E8_UT0Brig,3268
+dlrover/python/tests/test_sync_service.py,sha256=ytlqyxPHjflzJAIpHQimVfFu_nGXKG4mon9Y5kQWL2o,2455
+dlrover/python/tests/test_task_manager.py,sha256=3b5q77FwdpMGKHJAo2ojMD9xsb6I8qTZI1yYjLpSfF0,4416
+dlrover/python/tests/test_utils.py,sha256=M6VFUYjlnIA9wQ94vhQtWo1iDMXh7vjHWGmOy2t8D0A,7667
+dlrover/python/tests/test_worker_manager.py,sha256=7114x9hCKRVaKqd59QR1SQUJyjHjJx-YFq8ufbo05gU,6132
+dlrover/python/util/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
+dlrover/python/util/reflect_util.py,sha256=6d__Wupk46-s5gwg5ChlZSJF5um4GDLhrZN-bz_oTnY,3856
+dlrover/python/util/actor_util/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
+dlrover/python/util/actor_util/parse_actor.py,sha256=QWQiECvoj4FVX1MnL_BtmCaZ3JHvcCvI-FWc8MVC2nA,1552
+dlrover/python/util/queue/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
+dlrover/python/util/queue/queue.py,sha256=aVR_a5vk6y5n5BAtMxBMA7XUhV04NUZfpDq7A1TKi8k,2834
+dlrover/python/util/state/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
+dlrover/python/util/state/memory_store.py,sha256=G9YoCClRxMqW038eIXNXt5K2uQxptEiA5_ZUy28FSj0,2322
+dlrover/python/util/state/stats_backend.py,sha256=LYxJX7qO0orxue3b1xQi4xOzKft8x4gFdL2hDNyMSqc,1593
+dlrover/python/util/state/store_mananger.py,sha256=3JwmU1Dj3fiowTUJjPfMbXDYglssu52v7z0H03RLzy0,2654
 dlrover/trainer/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/trainer/__main__.py,sha256=MFQrJ_Oq1Ng_ssgE0_Hq8Za0bsJpYIZkTcoNKAPCw4w,778
 dlrover/trainer/constants/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/trainer/constants/constants.py,sha256=SaCXYT4it9SMtBIsepAopvgC482rYhZwRurpz_v-zHw,1090
-dlrover/trainer/constants/platform_constants.py,sha256=mkgj4_EvtDimcNEXn8TdOFVfohZL6H0I7JjX94SbCnM,956
-dlrover/trainer/constants/tf_constants.py,sha256=7Y5jz9gcBy4bGnoz5FPxkjJ3Jv5O_kKrBBOYMvtXhXc,2703
+dlrover/trainer/constants/platform_constants.py,sha256=FyH8mbhb4mdkhrr6KhcYDdUKv9s-uQfywrpAGgR2T3U,989
+dlrover/trainer/constants/tf_constants.py,sha256=J-PD6-_dk79AtBNd7NA4iSk4hnvh3hFSqibGZzuPd-M,3350
 dlrover/trainer/entry/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/trainer/entry/local_entry.py,sha256=34j6UW2jWNJ24zjkikmsJvUHhr05k1wADylMthceDDw,967
-dlrover/trainer/examples/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
-dlrover/trainer/examples/estimator_executor/MyEstimator.py,sha256=6qbtNR3UX1kOMnhMrmzZcKxA0_rF4fcGXHAwIhQX6hI,2364
-dlrover/trainer/examples/estimator_executor/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
-dlrover/trainer/examples/estimator_executor/conf.py,sha256=RVWJTnBmAtm5NvyBLmgyRdaZ4fdkSUGteky1TTwIivg,1649
 dlrover/trainer/mock/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
 dlrover/trainer/mock/base_process_scheduler.py,sha256=gSZyapIBwtiUelS0CEMHinyQgGahDvwYQdB_iZ8C3Sc,4086
-dlrover/trainer/mock/tf_process_scheduler.py,sha256=o4KEsjDHhXIK7a0LCtzhFidYTbnFm6Zxs4_Do1Gx4s0,5686
+dlrover/trainer/mock/tf_process_scheduler.py,sha256=5PUxO5AZVY2yAY-cbPFMkdmuEEzi-kh0Q-8_VuE_xhk,6917
 dlrover/trainer/platform/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
-dlrover/trainer/platform/starter.py,sha256=lVV5a-zM5g5BeuU3jCE2EGYVrlVIjm3rJAhoGkBjL6U,2801
-dlrover/trainer/tensorflow/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
+dlrover/trainer/platform/starter.py,sha256=8msLizR_bQJnfE29jojV4qG7BsN5xFeXeCe4G89YeDA,3422
+dlrover/trainer/tensorflow/__init__.py,sha256=ozjPCxham3izMMFBM-WUH4Fd3f-DVo3besyL5DQYEXo,666
 dlrover/trainer/tensorflow/executor/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
-dlrover/trainer/tensorflow/executor/base_executor.py,sha256=t9mxrWNO7lxcZN_Mno9wIUT8ARUbj3GRg89-uj1it64,6643
-dlrover/trainer/tensorflow/executor/estimator_executor.py,sha256=UZC6uKJw5Z4m1s4pGRJobX7QGqXp2ptZZtoURfHH4NY,8560
+dlrover/trainer/tensorflow/executor/base_executor.py,sha256=CJWIaA65RfHYbh-htWjEGhoHXUzqBROnqvys_ZuR-Xw,7127
+dlrover/trainer/tensorflow/executor/estimator_executor.py,sha256=pVV2nzbzgJAaRvPfVDMRSPLUEgYPkLUog9S1vxGsFGY,10386
 dlrover/trainer/tensorflow/failover/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
-dlrover/trainer/tensorflow/failover/failover_client.py,sha256=9Kt_eeGjft7vFb4OHOkHoz-gGg_t1MuPLXnY1vck9wM,4455
-dlrover/trainer/tensorflow/failover/tensorflow_failover.py,sha256=OtmfJFBnehDn91d6K4_A-h8rKKaq7Vys0064xJnyBmQ,6596
+dlrover/trainer/tensorflow/failover/failover_client.py,sha256=hupz-2WpuZLJwPLV4xe_CMnByTSSJAOhVFdCcuAkJeg,4312
+dlrover/trainer/tensorflow/failover/tensorflow_failover.py,sha256=_xA8DbFOTb9LQbuTLQLbA94Y8dpJTgkBjI6cvzm_lKY,6111
 dlrover/trainer/tensorflow/hooks/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
 dlrover/trainer/tensorflow/hooks/elastic_data_shard_report_hook.py,sha256=duqa9_4uz9mhprJBiQQydvlnczHsYeUFi23XHLF84eI,1151
 dlrover/trainer/tensorflow/hooks/global_step_hook.py,sha256=KvE30qbmeR0xQgo9i6NEL1h9QcnX_AJ72pPu3syCxg8,1611
-dlrover/trainer/tensorflow/reader/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
-dlrover/trainer/tensorflow/reader/fake_reader.py,sha256=rjoxH3w_ng-H4wcB3_J5uXei9KWErHAcnaMIXW53yU8,2625
-dlrover/trainer/tensorflow/reader/file_reader.py,sha256=GlWSAMthkFaUOJ7FAZFM4F8Kt5ljUpX1PZcie8HmZLs,2918
+dlrover/trainer/tensorflow/reader/__init__.py,sha256=0r2grVaQ-691ITv1PgM9e985EaA0hnELlaJv-5Y716g,691
+dlrover/trainer/tensorflow/reader/base_reader.py,sha256=eGkn7XhfUwPx8N5pvCPPo57a6BwVNsD-pFkeY1_KkOQ,3109
+dlrover/trainer/tensorflow/reader/file_reader.py,sha256=Hc6A6KblFBFLvOvkWrHT9Ug8ql7LHSbJTynTMdawl68,1592
 dlrover/trainer/tensorflow/util/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
 dlrover/trainer/tensorflow/util/column_info.py,sha256=8VXBlsZqdSnv5WhMpJN3L7dXUCku4ZBqahPTGrcAU44,1805
 dlrover/trainer/tensorflow/util/common_util.py,sha256=y1kQy7TqRld0dDFa8Qjdz0zGmFOU8kq3Mku4c3nvCSA,3666
 dlrover/trainer/tensorflow/util/data_mapping_util.py,sha256=qKlMnsxdMbdZ6WUEEqGg6hAdzxeEYDB-t6tNwjLduRU,1061
-dlrover/trainer/tensorflow/util/dataset_util.py,sha256=wVwgTTulR4RvUl3xqXNTzaxSDQ8JssLu1C8owwQtNPs,5251
-dlrover/trainer/tensorflow/util/estimator_util.py,sha256=pa51pFQtxJv6qEI6M99dttxq7yIQaoomeNJqL3kOnb8,2572
+dlrover/trainer/tensorflow/util/dataset_util.py,sha256=qjz-NlmqBBwp-ztZrhegfJcvDYntjW2pFFzBLFuuPoM,5429
+dlrover/trainer/tensorflow/util/estimator_util.py,sha256=-ULYmgVFALFCd4oLGSbjZc3OQBl0dI26HUC9Uy2tnQc,8506
 dlrover/trainer/tensorflow/util/path_util.py,sha256=LQCCluOm2zR492dVuwW_z_hVtArgXVTkc1mnEjidHms,1122
-dlrover/trainer/tensorflow/util/tf_patch_util.py,sha256=OCbugs8T2eCDXopEhZb2axav-3_ZxTw48ToqXZGa08M,13869
+dlrover/trainer/tensorflow/util/tf_env_util.py,sha256=Zi0GaRhfHYytKVKcYNbTfh9E89hpRuADYzC0EyE3bjk,1598
+dlrover/trainer/tensorflow/util/tf_patch_util.py,sha256=8LjI9NclFCNPnZ63GIon0qgV7x5XqVUdDMFLkqugy-s,15226
 dlrover/trainer/tensorflow/util/tf_version_util.py,sha256=4zoYq-yImVA_6ymQCBdxwMCNMi8cT7_EQbe78uqq140,1104
+dlrover/trainer/torch/__init__.py,sha256=PPDUSDBrUEdum00XKyizIVb160YdBoWrFqQLcwmiJ9g,599
+dlrover/trainer/torch/elastic.py,sha256=8m1QQZ7IFBLceznQTG71seLwyRt3K3QbjNEdirZfOwo,9587
+dlrover/trainer/torch/elastic_dataset.py,sha256=CBCP-Mopi_WIYVXzD9SDP1HQMi-GeS1iJxhGsmFuUo4,3815
+dlrover/trainer/torch/elastic_run.py,sha256=YcxuzgBuE5erRd9zDrwa6bA1Xtz3yVfSN6BfAXDWdPo,3705
+dlrover/trainer/torch/elastic_sampler.py,sha256=BLEXpCRBXZ7xLrR2f6yr3HwdbE-sIXhITo7hBW-6doM,4197
+dlrover/trainer/torch/main.py,sha256=2lZr2YcXAFjKxYn4M4okmbThfnqd88BHUnMHh9jgYQk,690
+dlrover/trainer/torch/run_network_check.py,sha256=n8ORvVCsEuXSr44l0iKy-_Jp1e1hMaPX2q6jBLu2dJ0,1700
+dlrover/trainer/torch/utils.py,sha256=uEkrS6t6Fdr63T1QyPW-qUTvlSLE2Y4n5qFt9LlPAJg,741
 dlrover/trainer/util/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
-dlrover/trainer/util/args_util.py,sha256=W3xValmVDFuOVi3k8uKqWcBICcebrxXemp5cfxbGA48,1849
-dlrover/trainer/util/conf_util.py,sha256=OHIqrigIT4GypC9BmmlN8WryCPMkfrDOQNGBba5uoSo,6362
+dlrover/trainer/util/args_util.py,sha256=cWIf8seZuB-CZDDj2451M93RhedlZOoiK7Wje_61RJ8,2031
+dlrover/trainer/util/conf_util.py,sha256=0Qzx2glA0nwYe335RRq8zV9Rx-i9tLVKz6Pzz5NO5fs,6436
 dlrover/trainer/util/log_util.py,sha256=v0sxOgR0IWQl6odSXFc1h-GTHyeeCb7-MlQuLjiTfrA,2863
 dlrover/trainer/util/net_util.py,sha256=RLWB5efGRUgaXMbJk0uzdLuyboNEcOVhbFJb-VXG2tI,736
 dlrover/trainer/util/reflect_util.py,sha256=6MSIuzdcKqODcrH35oWINzE-oQa-Y58XIxi3QPkJWGM,3860
 dlrover/trainer/worker/__init__.py,sha256=vpZVhqJNwDst1RQ-nODrcGkpDsrj9CwRLfYNGyL2D1E,599
-dlrover/trainer/worker/tf_kubernetes_worker.py,sha256=UKazopGSbwyNk4DscpyKZ1ELb0XYxtKP6Rlyaos6xvc,2186
-dlrover-0.1.0rc0.dev1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-dlrover-0.1.0rc0.dev1.dist-info/METADATA,sha256=VAxzmTLyp6L53OgXoROQkZjRx-nawhakqO8aP95upOg,743
-dlrover-0.1.0rc0.dev1.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-dlrover-0.1.0rc0.dev1.dist-info/top_level.txt,sha256=DBXgCrSsRqJf0F1cJOaCbBv9tmdt3d7C6qEOFPBhCgg,8
-dlrover-0.1.0rc0.dev1.dist-info/RECORD,,
+dlrover/trainer/worker/tf_kubernetes_worker.py,sha256=ItXRn7H6ts1XD12dIJD7me5L061dUXIBKHF5lpCAFqI,3540
+dlrover/trainer/worker/tf_ray_worker.py,sha256=fPXlAoZJpB98KrOgRRf5MqqmEpsE0G_Br_mQn63AWUE,6932
+dlrover-0.2.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+dlrover-0.2.0.dist-info/METADATA,sha256=wZ_0KJRIB_CNJnAdZyMh7cvx6Duu3mYdNiJzZzuN0m0,956
+dlrover-0.2.0.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+dlrover-0.2.0.dist-info/entry_points.txt,sha256=5XjupQBuFi6kQ4TDGFgc_4cU_TEQJkX4qqqqmAR_csc,64
+dlrover-0.2.0.dist-info/top_level.txt,sha256=DBXgCrSsRqJf0F1cJOaCbBv9tmdt3d7C6qEOFPBhCgg,8
+dlrover-0.2.0.dist-info/RECORD,,
```

