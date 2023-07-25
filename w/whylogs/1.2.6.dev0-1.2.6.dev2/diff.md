# Comparing `tmp/whylogs-1.2.6.dev0.tar.gz` & `tmp/whylogs-1.2.6.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylogs-1.2.6.dev0.tar", max compression
+gzip compressed data, was "whylogs-1.2.6.dev2.tar", max compression
```

## Comparing `whylogs-1.2.6.dev0.tar` & `whylogs-1.2.6.dev2.tar`

### file list

```diff
@@ -1,217 +1,217 @@
--rw-r--r--   0        0        0     3166 2023-06-10 02:08:52.892155 whylogs-1.2.6.dev0/DESCRIPTION.md
--rw-r--r--   0        0        0     5851 2023-07-20 23:20:51.419575 whylogs-1.2.6.dev0/pyproject.toml
--rw-r--r--   0        0        0     1801 2023-07-03 21:21:20.160644 whylogs-1.2.6.dev0/whylogs/__init__.py
--rw-r--r--   0        0        0      347 2023-01-27 17:07:09.472540 whylogs-1.2.6.dev0/whylogs/api/__init__.py
--rw-r--r--   0        0        0      590 2023-01-27 17:07:09.472617 whylogs-1.2.6.dev0/whylogs/api/annotations.py
--rw-r--r--   0        0        0      120 2023-07-20 23:17:29.873324 whylogs-1.2.6.dev0/whylogs/api/fugue/__init__.py
--rw-r--r--   0        0        0     4840 2023-01-27 17:07:09.472808 whylogs-1.2.6.dev0/whylogs/api/fugue/profiler.py
--rw-r--r--   0        0        0     1997 2023-04-26 19:16:03.802667 whylogs-1.2.6.dev0/whylogs/api/fugue/registry.py
--rw-r--r--   0        0        0     8157 2023-07-03 21:21:20.161158 whylogs-1.2.6.dev0/whylogs/api/logger/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 19:16:03.802843 whylogs-1.2.6.dev0/whylogs/api/logger/experimental/multi_dataset_logger/__init__.py
--rw-r--r--   0        0        0      468 2023-04-26 19:16:03.802937 whylogs-1.2.6.dev0/whylogs/api/logger/experimental/multi_dataset_logger/future_util.py
--rw-r--r--   0        0        0     2119 2023-04-26 19:16:03.803018 whylogs-1.2.6.dev0/whylogs/api/logger/experimental/multi_dataset_logger/message_processor.py
--rw-r--r--   0        0        0    15693 2023-07-20 23:17:29.874500 whylogs-1.2.6.dev0/whylogs/api/logger/experimental/multi_dataset_logger/multi_dataset_rolling_logger.py
--rw-r--r--   0        0        0     3964 2023-04-26 19:16:03.803232 whylogs-1.2.6.dev0/whylogs/api/logger/experimental/multi_dataset_logger/time_util.py
--rw-r--r--   0        0        0     4770 2023-06-10 02:08:52.902704 whylogs-1.2.6.dev0/whylogs/api/logger/logger.py
--rw-r--r--   0        0        0    19765 2023-07-20 16:06:32.109570 whylogs-1.2.6.dev0/whylogs/api/logger/result_set.py
--rw-r--r--   0        0        0     9549 2023-07-20 16:01:51.601343 whylogs-1.2.6.dev0/whylogs/api/logger/rolling.py
--rw-r--r--   0        0        0     2113 2023-04-26 19:16:03.804600 whylogs-1.2.6.dev0/whylogs/api/logger/segment_cache.py
--rw-r--r--   0        0        0     6333 2023-06-10 02:08:52.903287 whylogs-1.2.6.dev0/whylogs/api/logger/segment_processing.py
--rw-r--r--   0        0        0      687 2023-01-27 17:07:09.473466 whylogs-1.2.6.dev0/whylogs/api/logger/transient.py
--rw-r--r--   0        0        0      406 2023-02-08 17:50:31.435292 whylogs-1.2.6.dev0/whylogs/api/pyspark/experimental/__init__.py
--rw-r--r--   0        0        0     6168 2023-07-20 16:01:51.601513 whylogs-1.2.6.dev0/whylogs/api/pyspark/experimental/profiler.py
--rw-r--r--   0        0        0     7663 2023-07-03 21:21:20.161462 whylogs-1.2.6.dev0/whylogs/api/pyspark/experimental/segmented_profiler.py
--rw-r--r--   0        0        0      465 2023-01-27 17:07:09.473854 whylogs-1.2.6.dev0/whylogs/api/reader/__init__.py
--rw-r--r--   0        0        0      645 2023-01-27 17:07:09.473918 whylogs-1.2.6.dev0/whylogs/api/reader/local.py
--rw-r--r--   0        0        0      617 2023-01-27 17:07:09.473991 whylogs-1.2.6.dev0/whylogs/api/reader/reader.py
--rw-r--r--   0        0        0     2073 2023-01-27 17:07:09.474087 whylogs-1.2.6.dev0/whylogs/api/reader/s3.py
--rw-r--r--   0        0        0      237 2023-01-27 17:07:09.474216 whylogs-1.2.6.dev0/whylogs/api/store/__init__.py
--rw-r--r--   0        0        0     4566 2023-01-27 17:07:09.474312 whylogs-1.2.6.dev0/whylogs/api/store/local_store.py
--rw-r--r--   0        0        0     1208 2023-04-26 19:16:03.805014 whylogs-1.2.6.dev0/whylogs/api/store/profile_store.py
--rw-r--r--   0        0        0      672 2023-01-27 17:07:09.474460 whylogs-1.2.6.dev0/whylogs/api/store/query.py
--rw-r--r--   0        0        0     5350 2023-01-27 17:07:09.474545 whylogs-1.2.6.dev0/whylogs/api/store/sqlite_store.py
--rw-r--r--   0        0        0     6128 2023-07-03 21:21:20.162051 whylogs-1.2.6.dev0/whylogs/api/usage_stats/__init__.py
--rw-r--r--   0        0        0       79 2023-07-03 21:21:20.162188 whylogs-1.2.6.dev0/whylogs/api/whylabs/__init__.py
--rw-r--r--   0        0        0     7497 2023-07-03 21:21:20.162328 whylogs-1.2.6.dev0/whylogs/api/whylabs/session/config.py
--rw-r--r--   0        0        0      329 2023-07-03 21:21:20.162408 whylogs-1.2.6.dev0/whylogs/api/whylabs/session/notebook_check.py
--rw-r--r--   0        0        0     3813 2023-07-03 21:21:20.162491 whylogs-1.2.6.dev0/whylogs/api/whylabs/session/notebook_logger.py
--rw-r--r--   0        0        0    10646 2023-07-03 21:21:20.162594 whylogs-1.2.6.dev0/whylogs/api/whylabs/session/session_manager.py
--rw-r--r--   0        0        0      666 2023-07-20 23:17:29.875213 whylogs-1.2.6.dev0/whylogs/api/whylabs/session/session_types.py
--rw-r--r--   0        0        0      947 2023-01-27 17:07:09.474801 whylogs-1.2.6.dev0/whylogs/api/writer/__init__.py
--rw-r--r--   0        0        0     2726 2023-01-27 17:07:09.474892 whylogs-1.2.6.dev0/whylogs/api/writer/gcs.py
--rw-r--r--   0        0        0     1169 2023-01-27 17:07:09.474976 whylogs-1.2.6.dev0/whylogs/api/writer/local.py
--rw-r--r--   0        0        0     2084 2023-07-03 21:21:20.163318 whylogs-1.2.6.dev0/whylogs/api/writer/mlflow.py
--rw-r--r--   0        0        0     3408 2023-07-03 21:21:20.163457 whylogs-1.2.6.dev0/whylogs/api/writer/s3.py
--rw-r--r--   0        0        0    41758 2023-07-20 16:01:51.601983 whylogs-1.2.6.dev0/whylogs/api/writer/whylabs.py
--rw-r--r--   0        0        0     1217 2023-02-10 21:03:36.388032 whylogs-1.2.6.dev0/whylogs/api/writer/writer.py
--rw-r--r--   0        0        0     1090 2023-04-26 19:16:03.805479 whylogs-1.2.6.dev0/whylogs/core/__init__.py
--rw-r--r--   0        0        0     3391 2023-07-03 21:21:20.163851 whylogs-1.2.6.dev0/whylogs/core/column_profile.py
--rw-r--r--   0        0        0      208 2023-01-27 17:07:09.475617 whylogs-1.2.6.dev0/whylogs/core/common.py
--rw-r--r--   0        0        0     1589 2023-07-20 16:01:51.602121 whylogs-1.2.6.dev0/whylogs/core/configs.py
--rw-r--r--   0        0        0      455 2023-07-03 21:21:20.163980 whylogs-1.2.6.dev0/whylogs/core/constraints/__init__.py
--rw-r--r--   0        0        0     1798 2023-07-03 21:21:20.164309 whylogs-1.2.6.dev0/whylogs/core/constraints/factories/__init__.py
--rw-r--r--   0        0        0     1103 2023-01-27 17:07:09.476006 whylogs-1.2.6.dev0/whylogs/core/constraints/factories/cardinality_metrics.py
--rw-r--r--   0        0        0     2049 2023-06-10 02:08:52.904508 whylogs-1.2.6.dev0/whylogs/core/constraints/factories/condition_counts.py
--rw-r--r--   0        0        0     2601 2023-01-27 17:07:09.476163 whylogs-1.2.6.dev0/whylogs/core/constraints/factories/count_metrics.py
--rw-r--r--   0        0        0     7063 2023-04-26 19:16:03.806082 whylogs-1.2.6.dev0/whylogs/core/constraints/factories/distribution_metrics.py
--rw-r--r--   0        0        0     2083 2023-01-27 17:07:09.476339 whylogs-1.2.6.dev0/whylogs/core/constraints/factories/frequent_items.py
--rw-r--r--   0        0        0      737 2023-06-10 02:08:52.904742 whylogs-1.2.6.dev0/whylogs/core/constraints/factories/multi_metrics.py
--rw-r--r--   0        0        0     3199 2023-04-26 19:16:03.806280 whylogs-1.2.6.dev0/whylogs/core/constraints/factories/types_metrics.py
--rw-r--r--   0        0        0    30671 2023-07-20 23:17:29.875827 whylogs-1.2.6.dev0/whylogs/core/constraints/metric_constraints.py
--rw-r--r--   0        0        0    11486 2023-07-03 21:21:20.164600 whylogs-1.2.6.dev0/whylogs/core/dataset_profile.py
--rw-r--r--   0        0        0     4230 2023-07-20 16:01:51.602704 whylogs-1.2.6.dev0/whylogs/core/datatypes.py
--rw-r--r--   0        0        0      518 2023-01-27 17:07:09.476805 whylogs-1.2.6.dev0/whylogs/core/errors.py
--rw-r--r--   0        0        0     2560 2023-01-27 17:07:09.476877 whylogs-1.2.6.dev0/whylogs/core/feature_weights.py
--rw-r--r--   0        0        0      806 2023-01-27 17:07:09.476954 whylogs-1.2.6.dev0/whylogs/core/input_resolver.py
--rw-r--r--   0        0        0     1740 2023-04-26 19:16:03.806702 whylogs-1.2.6.dev0/whylogs/core/metric_getters.py
--rw-r--r--   0        0        0      984 2023-01-27 17:07:09.477163 whylogs-1.2.6.dev0/whylogs/core/metrics/__init__.py
--rw-r--r--   0        0        0     4085 2023-07-20 16:38:24.694622 whylogs-1.2.6.dev0/whylogs/core/metrics/aggregators.py
--rw-r--r--   0        0        0     5031 2023-04-26 19:16:03.807018 whylogs-1.2.6.dev0/whylogs/core/metrics/column_metrics.py
--rw-r--r--   0        0        0     6481 2023-01-27 17:07:09.477448 whylogs-1.2.6.dev0/whylogs/core/metrics/compound_metric.py
--rw-r--r--   0        0        0     7615 2023-06-10 02:08:52.905421 whylogs-1.2.6.dev0/whylogs/core/metrics/condition_count_metric.py
--rw-r--r--   0        0        0     1597 2023-01-27 17:07:09.477621 whylogs-1.2.6.dev0/whylogs/core/metrics/decorators.py
--rw-r--r--   0        0        0     4840 2023-04-26 19:16:03.807141 whylogs-1.2.6.dev0/whylogs/core/metrics/deserializers.py
--rw-r--r--   0        0        0     1361 2023-01-27 17:07:09.477783 whylogs-1.2.6.dev0/whylogs/core/metrics/maths.py
--rw-r--r--   0        0        0     6053 2023-01-27 17:07:09.477875 whylogs-1.2.6.dev0/whylogs/core/metrics/metric_components.py
--rw-r--r--   0        0        0    21749 2023-06-10 02:08:52.905635 whylogs-1.2.6.dev0/whylogs/core/metrics/metrics.py
--rw-r--r--   0        0        0     8016 2023-04-26 19:16:03.807445 whylogs-1.2.6.dev0/whylogs/core/metrics/multimetric.py
--rw-r--r--   0        0        0     4517 2023-04-26 19:16:03.807560 whylogs-1.2.6.dev0/whylogs/core/metrics/serializers.py
--rw-r--r--   0        0        0     5504 2023-01-27 17:07:09.478316 whylogs-1.2.6.dev0/whylogs/core/metrics/unicode_range.py
--rw-r--r--   0        0        0      107 2023-01-27 17:07:09.478674 whylogs-1.2.6.dev0/whylogs/core/model_performance_metrics/__init__.py
--rw-r--r--   0        0        0     9253 2023-07-20 21:39:25.439962 whylogs-1.2.6.dev0/whylogs/core/model_performance_metrics/confusion_matrix.py
--rw-r--r--   0        0        0     7445 2023-04-26 19:16:03.808000 whylogs-1.2.6.dev0/whylogs/core/model_performance_metrics/model_performance_metrics.py
--rw-r--r--   0        0        0     2837 2023-01-27 17:07:09.479060 whylogs-1.2.6.dev0/whylogs/core/model_performance_metrics/regression_metrics.py
--rw-r--r--   0        0        0     5499 2023-04-26 19:16:03.808148 whylogs-1.2.6.dev0/whylogs/core/predicate_parser.py
--rw-r--r--   0        0        0    14489 2023-06-10 02:08:52.905830 whylogs-1.2.6.dev0/whylogs/core/preprocessing.py
--rw-r--r--   0        0        0      335 2023-01-27 17:07:09.479379 whylogs-1.2.6.dev0/whylogs/core/projectors.py
--rw-r--r--   0        0        0      183 2023-01-27 17:07:09.479504 whylogs-1.2.6.dev0/whylogs/core/proto/__init__.py
--rw-r--r--   0        0        0      242 2023-01-27 17:07:09.479628 whylogs-1.2.6.dev0/whylogs/core/proto/v0/__init__.py
--rw-r--r--   0        0        0     7135 2023-07-20 23:21:29.487742 whylogs-1.2.6.dev0/whylogs/core/proto/v0/v0_constraints_pb2.py
--rw-r--r--   0        0        0    20212 2023-07-20 23:21:29.043484 whylogs-1.2.6.dev0/whylogs/core/proto/v0/v0_constraints_pb2.pyi
--rw-r--r--   0        0        0    10533 2023-07-20 23:21:29.043555 whylogs-1.2.6.dev0/whylogs/core/proto/v0/v0_messages_pb2.py
--rw-r--r--   0        0        0    29724 2023-07-20 23:21:29.043722 whylogs-1.2.6.dev0/whylogs/core/proto/v0/v0_messages_pb2.pyi
--rw-r--r--   0        0        0     8826 2023-07-20 23:21:29.518627 whylogs-1.2.6.dev0/whylogs/core/proto/v0/v0_summaries_pb2.py
--rw-r--r--   0        0        0    24739 2023-07-20 23:21:29.043933 whylogs-1.2.6.dev0/whylogs/core/proto/v0/v0_summaries_pb2.pyi
--rw-r--r--   0        0        0     8849 2023-07-20 23:21:28.936543 whylogs-1.2.6.dev0/whylogs/core/proto/whylogs_messages_pb2.py
--rw-r--r--   0        0        0    21840 2023-07-20 23:21:28.936690 whylogs-1.2.6.dev0/whylogs/core/proto/whylogs_messages_pb2.pyi
--rw-r--r--   0        0        0     7350 2023-04-26 19:16:03.808440 whylogs-1.2.6.dev0/whylogs/core/relations.py
--rw-r--r--   0        0        0    11357 2023-07-20 16:01:51.602889 whylogs-1.2.6.dev0/whylogs/core/resolvers.py
--rw-r--r--   0        0        0    10029 2023-07-20 16:01:51.603142 whylogs-1.2.6.dev0/whylogs/core/schema.py
--rw-r--r--   0        0        0      144 2023-01-27 17:07:09.479971 whylogs-1.2.6.dev0/whylogs/core/segment.py
--rw-r--r--   0        0        0     2343 2023-01-27 17:07:09.480060 whylogs-1.2.6.dev0/whylogs/core/segmentation_partition.py
--rw-r--r--   0        0        0      826 2023-04-26 19:16:03.808767 whylogs-1.2.6.dev0/whylogs/core/specialized_resolvers.py
--rw-r--r--   0        0        0     2087 2023-04-26 19:16:03.808869 whylogs-1.2.6.dev0/whylogs/core/stubs.py
--rw-r--r--   0        0        0      486 2023-04-26 19:16:03.808997 whylogs-1.2.6.dev0/whylogs/core/utils/__init__.py
--rw-r--r--   0        0        0     3603 2023-02-08 17:50:31.436291 whylogs-1.2.6.dev0/whylogs/core/utils/protobuf_utils.py
--rw-r--r--   0        0        0     2569 2023-06-10 02:08:52.906396 whylogs-1.2.6.dev0/whylogs/core/utils/stats_calculations.py
--rw-r--r--   0        0        0      130 2023-01-27 17:07:09.480474 whylogs-1.2.6.dev0/whylogs/core/utils/timestamp_calculations.py
--rw-r--r--   0        0        0     1602 2023-01-27 17:07:09.480548 whylogs-1.2.6.dev0/whylogs/core/utils/utils.py
--rw-r--r--   0        0        0      210 2023-07-03 21:21:20.164964 whylogs-1.2.6.dev0/whylogs/core/validators/__init__.py
--rw-r--r--   0        0        0     4760 2023-07-03 21:21:20.165074 whylogs-1.2.6.dev0/whylogs/core/validators/condition_validator.py
--rw-r--r--   0        0        0      508 2023-01-27 17:07:09.480781 whylogs-1.2.6.dev0/whylogs/core/validators/validator.py
--rw-r--r--   0        0        0      214 2023-01-27 17:07:09.480884 whylogs-1.2.6.dev0/whylogs/core/view/__init__.py
--rw-r--r--   0        0        0     6157 2023-06-10 02:08:52.906601 whylogs-1.2.6.dev0/whylogs/core/view/column_profile_view.py
--rw-r--r--   0        0        0    17663 2023-04-26 19:16:03.809655 whylogs-1.2.6.dev0/whylogs/core/view/dataset_profile_view.py
--rw-r--r--   0        0        0     8747 2023-07-20 16:38:20.684036 whylogs-1.2.6.dev0/whylogs/core/view/segmented_dataset_profile_view.py
--rw-r--r--   0        0        0      211 2023-04-26 19:16:03.809887 whylogs-1.2.6.dev0/whylogs/datasets/__init__.py
--rw-r--r--   0        0        0     5813 2023-01-27 17:07:09.481601 whylogs-1.2.6.dev0/whylogs/datasets/base.py
--rw-r--r--   0        0        0     6087 2023-04-26 19:16:03.809996 whylogs-1.2.6.dev0/whylogs/datasets/configs.py
--rw-r--r--   0        0        0        0 2023-01-27 17:07:09.481815 whylogs-1.2.6.dev0/whylogs/datasets/descr/__init__.py
--rw-r--r--   0        0        0     6397 2023-04-26 19:16:03.810134 whylogs-1.2.6.dev0/whylogs/datasets/descr/ecommerce.rst
--rw-r--r--   0        0        0     3506 2023-04-26 19:16:03.810209 whylogs-1.2.6.dev0/whylogs/datasets/descr/employee.rst
--rw-r--r--   0        0        0    11285 2023-01-27 17:07:09.482028 whylogs-1.2.6.dev0/whylogs/datasets/descr/weather.rst
--rw-r--r--   0        0        0    10688 2023-04-26 19:16:03.810340 whylogs-1.2.6.dev0/whylogs/datasets/ecommerce.py
--rw-r--r--   0        0        0    10981 2023-04-26 19:16:03.810448 whylogs-1.2.6.dev0/whylogs/datasets/employee.py
--rw-r--r--   0        0        0     2349 2023-01-27 17:07:09.482221 whylogs-1.2.6.dev0/whylogs/datasets/utils.py
--rw-r--r--   0        0        0    11476 2023-04-26 19:16:03.810553 whylogs-1.2.6.dev0/whylogs/datasets/weather.py
--rw-r--r--   0        0        0        0 2023-04-26 19:16:03.810596 whylogs-1.2.6.dev0/whylogs/experimental/__init__.py
--rw-r--r--   0        0        0     3530 2023-07-20 16:01:51.603439 whylogs-1.2.6.dev0/whylogs/experimental/api/logger/__init__.py
--rw-r--r--   0        0        0     3770 2023-04-26 19:16:03.810717 whylogs-1.2.6.dev0/whylogs/experimental/constraints_generation/__init__.py
--rw-r--r--   0        0        0     1105 2023-04-26 19:16:03.810785 whylogs-1.2.6.dev0/whylogs/experimental/constraints_generation/condition_counts.py
--rw-r--r--   0        0        0      846 2023-04-26 19:16:03.810850 whylogs-1.2.6.dev0/whylogs/experimental/constraints_generation/count_metrics.py
--rw-r--r--   0        0        0     1554 2023-04-26 19:16:03.810923 whylogs-1.2.6.dev0/whylogs/experimental/constraints_generation/distribution_metrics.py
--rw-r--r--   0        0        0     1011 2023-04-26 19:16:03.810997 whylogs-1.2.6.dev0/whylogs/experimental/constraints_generation/frequent_items.py
--rw-r--r--   0        0        0      685 2023-04-26 19:16:03.811071 whylogs-1.2.6.dev0/whylogs/experimental/constraints_generation/multi_metrics.py
--rw-r--r--   0        0        0      973 2023-04-26 19:16:03.811147 whylogs-1.2.6.dev0/whylogs/experimental/constraints_generation/types_metrics.py
--rw-r--r--   0        0        0    19692 2023-07-03 21:21:20.165360 whylogs-1.2.6.dev0/whylogs/experimental/core/metrics/udf_metric.py
--rw-r--r--   0        0        0    14261 2023-07-20 16:01:51.603649 whylogs-1.2.6.dev0/whylogs/experimental/core/udf_schema.py
--rw-r--r--   0        0        0     8861 2023-04-26 19:16:03.811409 whylogs-1.2.6.dev0/whylogs/experimental/extras/embedding_metric.py
--rw-r--r--   0        0        0      939 2023-04-26 19:16:03.812029 whylogs-1.2.6.dev0/whylogs/experimental/extras/matrix_component.py
--rwxr-xr-x   0        0        0    16737 2023-07-03 21:21:20.165648 whylogs-1.2.6.dev0/whylogs/experimental/extras/nlp_metric.py
--rw-r--r--   0        0        0        0 2023-04-26 19:16:03.812276 whylogs-1.2.6.dev0/whylogs/experimental/performance_estimation/__init__.py
--rw-r--r--   0        0        0     1554 2023-04-26 19:16:03.812379 whylogs-1.2.6.dev0/whylogs/experimental/performance_estimation/estimation_results.py
--rw-r--r--   0        0        0     8872 2023-04-26 19:16:03.812474 whylogs-1.2.6.dev0/whylogs/experimental/performance_estimation/estimators.py
--rw-r--r--   0        0        0     3777 2023-04-26 19:16:03.812618 whylogs-1.2.6.dev0/whylogs/experimental/preprocess/embeddings/selectors.py
--rw-r--r--   0        0        0    10031 2023-04-26 19:16:03.813192 whylogs-1.2.6.dev0/whylogs/extras/image_metric.py
--rw-r--r--   0        0        0       52 2023-01-27 17:07:09.482908 whylogs-1.2.6.dev0/whylogs/migration/__init__.py
--rw-r--r--   0        0        0    15367 2023-04-26 19:16:03.813404 whylogs-1.2.6.dev0/whylogs/migration/converters.py
--rw-r--r--   0        0        0     6959 2023-04-26 19:16:03.813667 whylogs-1.2.6.dev0/whylogs/migration/uncompound.py
--rw-r--r--   0        0        0      296 2023-01-27 17:07:09.483280 whylogs-1.2.6.dev0/whylogs/viz/__init__.py
--rw-r--r--   0        0        0      168 2023-01-27 17:07:09.483359 whylogs-1.2.6.dev0/whylogs/viz/configs.py
--rw-r--r--   0        0        0        0 2023-01-27 17:07:09.483443 whylogs-1.2.6.dev0/whylogs/viz/drift/__init__.py
--rw-r--r--   0        0        0    21751 2023-01-27 17:07:09.483581 whylogs-1.2.6.dev0/whylogs/viz/drift/column_drift_algorithms.py
--rw-r--r--   0        0        0     1366 2023-04-26 19:16:03.813799 whylogs-1.2.6.dev0/whylogs/viz/drift/configs.py
--rw-r--r--   0        0        0        0 2023-01-27 17:07:09.483741 whylogs-1.2.6.dev0/whylogs/viz/enums/__init__.py
--rw-r--r--   0        0        0      901 2023-01-27 17:07:09.483870 whylogs-1.2.6.dev0/whylogs/viz/enums/enums.py
--rw-r--r--   0        0        0        0 2023-01-27 17:07:09.483956 whylogs-1.2.6.dev0/whylogs/viz/extensions/__init__.py
--rw-r--r--   0        0        0      114 2023-01-27 17:07:09.484104 whylogs-1.2.6.dev0/whylogs/viz/extensions/reports/constraints.py
--rw-r--r--   0        0        0      272 2023-01-27 17:07:09.484184 whylogs-1.2.6.dev0/whylogs/viz/extensions/reports/histograms.py
--rw-r--r--   0        0        0     2502 2023-01-27 17:07:09.484275 whylogs-1.2.6.dev0/whylogs/viz/extensions/reports/html_report.py
--rw-r--r--   0        0        0      975 2023-01-27 17:07:09.484350 whylogs-1.2.6.dev0/whylogs/viz/extensions/reports/profile_summary.py
--rw-r--r--   0        0        0     3218 2023-01-27 17:07:09.484433 whylogs-1.2.6.dev0/whylogs/viz/extensions/reports/summary_drift.py
--rw-r--r--   0        0        0       38 2023-01-27 17:07:09.484541 whylogs-1.2.6.dev0/whylogs/viz/html/.prettierignore
--rw-r--r--   0        0        0      135 2023-01-27 17:07:09.484618 whylogs-1.2.6.dev0/whylogs/viz/html/.prettierrc.yaml
--rw-r--r--   0        0        0   155568 2023-01-27 17:07:09.484984 whylogs-1.2.6.dev0/whylogs/viz/html/css/bootstrap.min.css
--rw-r--r--   0        0        0    22747 2023-01-27 17:07:09.485128 whylogs-1.2.6.dev0/whylogs/viz/html/css/whylogs-styles.css
--rw-r--r--   0        0        0   160788 2023-01-27 17:07:09.485713 whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-Bold.ttf
--rw-r--r--   0        0        0    50888 2023-01-27 17:07:09.486054 whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-Bold.woff
--rw-r--r--   0        0        0    32180 2023-01-27 17:07:09.486154 whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-Bold.woff2
--rw-r--r--   0        0        0   172144 2023-01-27 17:07:09.486670 whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.ttf
--rw-r--r--   0        0        0    55560 2023-01-27 17:07:09.486934 whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.woff
--rw-r--r--   0        0        0    35476 2023-01-27 17:07:09.487006 whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.woff2
--rw-r--r--   0        0        0   172188 2023-01-27 17:07:09.487498 whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-Italic.ttf
--rw-r--r--   0        0        0    55728 2023-01-27 17:07:09.487744 whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-Italic.woff
--rw-r--r--   0        0        0    35144 2023-01-27 17:07:09.487874 whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-Italic.woff2
--rw-r--r--   0        0        0   161212 2023-01-27 17:07:09.488350 whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-Medium.ttf
--rw-r--r--   0        0        0    53244 2023-01-27 17:07:09.488597 whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-Medium.woff
--rw-r--r--   0        0        0    34516 2023-01-27 17:07:09.488721 whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-Medium.woff2
--rw-r--r--   0        0        0   172380 2023-01-27 17:07:09.489235 whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.ttf
--rw-r--r--   0        0        0    59012 2023-01-27 17:07:09.489480 whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.woff
--rw-r--r--   0        0        0    38404 2023-01-27 17:07:09.489600 whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.woff2
--rw-r--r--   0        0        0   161220 2023-01-27 17:07:09.490060 whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-Regular.ttf
--rw-r--r--   0        0        0    50936 2023-01-27 17:07:09.490321 whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-Regular.woff
--rw-r--r--   0        0        0    32192 2023-01-27 17:07:09.490390 whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-Regular.woff2
--rw-r--r--   0        0        0   161152 2023-01-27 17:07:09.490866 whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-SemiBold.ttf
--rw-r--r--   0        0        0    53296 2023-01-27 17:07:09.491109 whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-SemiBold.woff
--rw-r--r--   0        0        0    34744 2023-01-27 17:07:09.491228 whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-SemiBold.woff2
--rw-r--r--   0        0        0   172396 2023-01-27 17:07:09.491740 whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf
--rw-r--r--   0        0        0    58892 2023-01-27 17:07:09.491930 whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff
--rw-r--r--   0        0        0    38500 2023-01-27 17:07:09.492048 whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2
--rw-r--r--   0        0        0     3156 2023-01-27 17:07:09.492155 whylogs-1.2.6.dev0/whylogs/viz/html/images/placement-chart.png
--rw-r--r--   0        0        0     9649 2023-01-27 17:07:09.492251 whylogs-1.2.6.dev0/whylogs/viz/html/images/whylabs-favicon.png
--rw-r--r--   0        0        0   270687 2023-01-27 17:07:09.493137 whylogs-1.2.6.dev0/whylogs/viz/html/js/d3.min.js
--rw-r--r--   0        0        0    12606 2023-01-27 17:07:09.493241 whylogs-1.2.6.dev0/whylogs/viz/html/js/handlebars.js
--rw-r--r--   0        0        0    89501 2023-01-27 17:07:09.493571 whylogs-1.2.6.dev0/whylogs/viz/html/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0    55927 2023-01-27 17:07:09.493747 whylogs-1.2.6.dev0/whylogs/viz/html/js/whylogs-script.js
--rw-r--r--   0        0        0    52663 2023-01-27 17:07:09.493970 whylogs-1.2.6.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html
--rw-r--r--   0        0        0    14235 2023-01-27 17:07:09.494104 whylogs-1.2.6.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html
--rw-r--r--   0        0        0    26825 2023-01-27 17:07:09.494247 whylogs-1.2.6.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html
--rw-r--r--   0        0        0    14144 2023-01-27 17:07:09.494331 whylogs-1.2.6.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html
--rw-r--r--   0        0        0    15177 2023-04-26 19:16:03.814370 whylogs-1.2.6.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html
--rw-r--r--   0        0        0    18298 2023-01-27 17:07:09.494574 whylogs-1.2.6.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html
--rw-r--r--   0        0        0    41933 2023-01-27 17:07:09.494690 whylogs-1.2.6.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html
--rw-r--r--   0        0        0    98500 2023-01-27 17:07:09.496954 whylogs-1.2.6.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in.html
--rw-r--r--   0        0        0   752494 2023-01-27 17:07:09.497218 whylogs-1.2.6.dev0/whylogs/viz/html/templates/index-hbs-library-all-in.html
--rw-r--r--   0        0        0    25371 2023-01-27 17:07:09.497431 whylogs-1.2.6.dev0/whylogs/viz/html/templates/index-hbs.html
--rw-r--r--   0        0        0    26014 2023-01-27 17:07:09.497640 whylogs-1.2.6.dev0/whylogs/viz/html/templates/index.html
--rw-r--r--   0        0        0    21376 2023-04-26 19:16:03.814652 whylogs-1.2.6.dev0/whylogs/viz/notebook_profile_viz.py
--rw-r--r--   0        0        0      410 2023-01-27 17:07:09.498077 whylogs-1.2.6.dev0/whylogs/viz/utils/__init__.py
--rw-r--r--   0        0        0     2466 2023-01-27 17:07:09.498172 whylogs-1.2.6.dev0/whylogs/viz/utils/descriptive_stats.py
--rw-r--r--   0        0        0    12576 2023-01-27 17:07:09.498286 whylogs-1.2.6.dev0/whylogs/viz/utils/drift_calculations.py
--rw-r--r--   0        0        0     3561 2023-04-26 19:16:03.814826 whylogs-1.2.6.dev0/whylogs/viz/utils/frequent_items_calculations.py
--rw-r--r--   0        0        0     2747 2023-01-27 17:07:09.498439 whylogs-1.2.6.dev0/whylogs/viz/utils/histogram_calculations.py
--rw-r--r--   0        0        0     1060 2023-04-26 19:16:03.814946 whylogs-1.2.6.dev0/whylogs/viz/utils/html_template_utils.py
--rw-r--r--   0        0        0    14298 2023-01-27 17:07:09.498593 whylogs-1.2.6.dev0/whylogs/viz/utils/profile_viz_calculations.py
--rw-r--r--   0        0        0     3581 2023-01-27 17:07:09.498677 whylogs-1.2.6.dev0/whylogs/viz/utils/quantile_stats.py
--rw-r--r--   0        0        0     8086 1970-01-01 00:00:00.000000 whylogs-1.2.6.dev0/setup.py
--rw-r--r--   0        0        0     6483 1970-01-01 00:00:00.000000 whylogs-1.2.6.dev0/PKG-INFO
+-rw-r--r--   0        0        0     3166 2023-06-27 17:33:07.264805 whylogs-1.2.6.dev2/DESCRIPTION.md
+-rw-r--r--   0        0        0     5851 2023-07-19 21:05:04.552366 whylogs-1.2.6.dev2/pyproject.toml
+-rw-r--r--   0        0        0     1801 2023-07-03 16:02:37.106297 whylogs-1.2.6.dev2/whylogs/__init__.py
+-rw-r--r--   0        0        0      347 2023-05-11 20:19:32.742898 whylogs-1.2.6.dev2/whylogs/api/__init__.py
+-rw-r--r--   0        0        0      590 2023-06-08 01:23:07.097906 whylogs-1.2.6.dev2/whylogs/api/annotations.py
+-rw-r--r--   0        0        0      120 2023-07-03 16:02:37.106297 whylogs-1.2.6.dev2/whylogs/api/fugue/__init__.py
+-rw-r--r--   0        0        0     4840 2023-06-16 15:50:21.999413 whylogs-1.2.6.dev2/whylogs/api/fugue/profiler.py
+-rw-r--r--   0        0        0     1997 2023-02-22 16:52:30.792231 whylogs-1.2.6.dev2/whylogs/api/fugue/registry.py
+-rw-r--r--   0        0        0     8157 2023-07-03 16:02:37.106297 whylogs-1.2.6.dev2/whylogs/api/logger/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-03 16:21:20.616995 whylogs-1.2.6.dev2/whylogs/api/logger/experimental/multi_dataset_logger/__init__.py
+-rw-r--r--   0        0        0      468 2023-03-03 16:21:20.616995 whylogs-1.2.6.dev2/whylogs/api/logger/experimental/multi_dataset_logger/future_util.py
+-rw-r--r--   0        0        0     2119 2023-03-03 16:21:20.616995 whylogs-1.2.6.dev2/whylogs/api/logger/experimental/multi_dataset_logger/message_processor.py
+-rw-r--r--   0        0        0    15693 2023-04-11 19:13:37.824666 whylogs-1.2.6.dev2/whylogs/api/logger/experimental/multi_dataset_logger/multi_dataset_rolling_logger.py
+-rw-r--r--   0        0        0     3964 2023-04-11 19:13:37.824666 whylogs-1.2.6.dev2/whylogs/api/logger/experimental/multi_dataset_logger/time_util.py
+-rw-r--r--   0        0        0     4743 2023-07-19 19:51:44.822366 whylogs-1.2.6.dev2/whylogs/api/logger/logger.py
+-rw-r--r--   0        0        0    19765 2023-07-11 15:58:04.999567 whylogs-1.2.6.dev2/whylogs/api/logger/result_set.py
+-rw-r--r--   0        0        0     9549 2023-07-19 19:51:34.012366 whylogs-1.2.6.dev2/whylogs/api/logger/rolling.py
+-rw-r--r--   0        0        0     2113 2023-04-11 19:13:37.824666 whylogs-1.2.6.dev2/whylogs/api/logger/segment_cache.py
+-rw-r--r--   0        0        0     6333 2023-07-13 23:04:30.059567 whylogs-1.2.6.dev2/whylogs/api/logger/segment_processing.py
+-rw-r--r--   0        0        0      687 2023-05-31 17:44:36.663303 whylogs-1.2.6.dev2/whylogs/api/logger/transient.py
+-rw-r--r--   0        0        0      510 2023-07-19 20:47:53.972366 whylogs-1.2.6.dev2/whylogs/api/pyspark/experimental/__init__.py
+-rw-r--r--   0        0        0     2703 2023-07-19 20:58:57.812366 whylogs-1.2.6.dev2/whylogs/api/pyspark/experimental/profile_distributed_upload.py
+-rw-r--r--   0        0        0     6168 2023-07-19 19:51:34.012366 whylogs-1.2.6.dev2/whylogs/api/pyspark/experimental/profiler.py
+-rw-r--r--   0        0        0     7663 2023-07-03 16:02:37.106297 whylogs-1.2.6.dev2/whylogs/api/pyspark/experimental/segmented_profiler.py
+-rw-r--r--   0        0        0      465 2023-01-30 20:46:41.225482 whylogs-1.2.6.dev2/whylogs/api/reader/__init__.py
+-rw-r--r--   0        0        0      645 2023-01-30 20:46:41.225482 whylogs-1.2.6.dev2/whylogs/api/reader/local.py
+-rw-r--r--   0        0        0      617 2023-01-30 20:46:41.225482 whylogs-1.2.6.dev2/whylogs/api/reader/reader.py
+-rw-r--r--   0        0        0     2073 2023-01-30 20:46:41.225482 whylogs-1.2.6.dev2/whylogs/api/reader/s3.py
+-rw-r--r--   0        0        0      237 2023-01-30 20:46:41.225482 whylogs-1.2.6.dev2/whylogs/api/store/__init__.py
+-rw-r--r--   0        0        0     4566 2023-01-30 20:46:41.225482 whylogs-1.2.6.dev2/whylogs/api/store/local_store.py
+-rw-r--r--   0        0        0     1208 2023-03-03 16:21:20.616995 whylogs-1.2.6.dev2/whylogs/api/store/profile_store.py
+-rw-r--r--   0        0        0      672 2023-01-30 20:46:41.225482 whylogs-1.2.6.dev2/whylogs/api/store/query.py
+-rw-r--r--   0        0        0     5350 2023-01-30 20:46:41.225482 whylogs-1.2.6.dev2/whylogs/api/store/sqlite_store.py
+-rw-r--r--   0        0        0     6128 2023-07-03 16:02:37.106297 whylogs-1.2.6.dev2/whylogs/api/usage_stats/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-03 16:02:37.106297 whylogs-1.2.6.dev2/whylogs/api/whylabs/__init__.py
+-rw-r--r--   0        0        0     7497 2023-07-03 16:02:37.106297 whylogs-1.2.6.dev2/whylogs/api/whylabs/session/config.py
+-rw-r--r--   0        0        0      329 2023-07-03 16:02:37.106297 whylogs-1.2.6.dev2/whylogs/api/whylabs/session/notebook_check.py
+-rw-r--r--   0        0        0     3813 2023-07-03 16:02:37.106297 whylogs-1.2.6.dev2/whylogs/api/whylabs/session/notebook_logger.py
+-rw-r--r--   0        0        0    10646 2023-07-03 16:02:37.106297 whylogs-1.2.6.dev2/whylogs/api/whylabs/session/session_manager.py
+-rw-r--r--   0        0        0      666 2023-07-03 16:02:37.106297 whylogs-1.2.6.dev2/whylogs/api/whylabs/session/session_types.py
+-rw-r--r--   0        0        0      947 2023-01-30 20:46:41.225482 whylogs-1.2.6.dev2/whylogs/api/writer/__init__.py
+-rw-r--r--   0        0        0     2726 2023-06-16 15:50:22.009413 whylogs-1.2.6.dev2/whylogs/api/writer/gcs.py
+-rw-r--r--   0        0        0     1169 2023-06-16 15:50:22.009413 whylogs-1.2.6.dev2/whylogs/api/writer/local.py
+-rw-r--r--   0        0        0     2084 2023-07-03 16:02:37.106297 whylogs-1.2.6.dev2/whylogs/api/writer/mlflow.py
+-rw-r--r--   0        0        0     3408 2023-07-03 16:02:37.106297 whylogs-1.2.6.dev2/whylogs/api/writer/s3.py
+-rw-r--r--   0        0        0    41758 2023-07-19 19:51:34.012366 whylogs-1.2.6.dev2/whylogs/api/writer/whylabs.py
+-rw-r--r--   0        0        0     1217 2023-01-30 20:46:41.225482 whylogs-1.2.6.dev2/whylogs/api/writer/writer.py
+-rw-r--r--   0        0        0     1090 2023-06-27 17:33:07.354805 whylogs-1.2.6.dev2/whylogs/core/__init__.py
+-rw-r--r--   0        0        0     3391 2023-07-03 16:02:37.106297 whylogs-1.2.6.dev2/whylogs/core/column_profile.py
+-rw-r--r--   0        0        0      208 2023-01-30 20:46:41.235482 whylogs-1.2.6.dev2/whylogs/core/common.py
+-rw-r--r--   0        0        0     1589 2023-07-19 19:51:34.012366 whylogs-1.2.6.dev2/whylogs/core/configs.py
+-rw-r--r--   0        0        0      455 2023-07-03 16:02:37.106297 whylogs-1.2.6.dev2/whylogs/core/constraints/__init__.py
+-rw-r--r--   0        0        0     1798 2023-07-03 16:02:37.106297 whylogs-1.2.6.dev2/whylogs/core/constraints/factories/__init__.py
+-rw-r--r--   0        0        0     1103 2023-05-25 19:20:19.422537 whylogs-1.2.6.dev2/whylogs/core/constraints/factories/cardinality_metrics.py
+-rw-r--r--   0        0        0     2049 2023-06-27 17:33:07.364805 whylogs-1.2.6.dev2/whylogs/core/constraints/factories/condition_counts.py
+-rw-r--r--   0        0        0     2601 2023-05-25 19:20:19.422537 whylogs-1.2.6.dev2/whylogs/core/constraints/factories/count_metrics.py
+-rw-r--r--   0        0        0     7063 2023-05-25 19:20:19.422537 whylogs-1.2.6.dev2/whylogs/core/constraints/factories/distribution_metrics.py
+-rw-r--r--   0        0        0     2083 2023-01-30 20:46:41.235482 whylogs-1.2.6.dev2/whylogs/core/constraints/factories/frequent_items.py
+-rw-r--r--   0        0        0      737 2023-06-27 17:33:07.364805 whylogs-1.2.6.dev2/whylogs/core/constraints/factories/multi_metrics.py
+-rw-r--r--   0        0        0     3199 2023-06-27 17:33:07.364805 whylogs-1.2.6.dev2/whylogs/core/constraints/factories/types_metrics.py
+-rw-r--r--   0        0        0    30671 2023-07-03 16:02:37.106297 whylogs-1.2.6.dev2/whylogs/core/constraints/metric_constraints.py
+-rw-r--r--   0        0        0    11486 2023-07-03 16:02:37.106297 whylogs-1.2.6.dev2/whylogs/core/dataset_profile.py
+-rw-r--r--   0        0        0     4230 2023-07-19 19:51:34.012366 whylogs-1.2.6.dev2/whylogs/core/datatypes.py
+-rw-r--r--   0        0        0      518 2023-01-30 20:46:41.235482 whylogs-1.2.6.dev2/whylogs/core/errors.py
+-rw-r--r--   0        0        0     2560 2023-01-30 20:46:41.235482 whylogs-1.2.6.dev2/whylogs/core/feature_weights.py
+-rw-r--r--   0        0        0      806 2023-01-30 20:46:41.235482 whylogs-1.2.6.dev2/whylogs/core/input_resolver.py
+-rw-r--r--   0        0        0     1740 2023-02-24 20:07:49.042231 whylogs-1.2.6.dev2/whylogs/core/metric_getters.py
+-rw-r--r--   0        0        0      984 2023-01-30 20:46:41.235482 whylogs-1.2.6.dev2/whylogs/core/metrics/__init__.py
+-rw-r--r--   0        0        0     4085 2023-04-11 19:13:37.824666 whylogs-1.2.6.dev2/whylogs/core/metrics/aggregators.py
+-rw-r--r--   0        0        0     5031 2023-04-20 13:28:02.613992 whylogs-1.2.6.dev2/whylogs/core/metrics/column_metrics.py
+-rw-r--r--   0        0        0     6481 2023-01-30 20:46:41.235482 whylogs-1.2.6.dev2/whylogs/core/metrics/compound_metric.py
+-rw-r--r--   0        0        0     7615 2023-06-27 17:33:07.364805 whylogs-1.2.6.dev2/whylogs/core/metrics/condition_count_metric.py
+-rw-r--r--   0        0        0     1597 2023-01-30 20:46:41.235482 whylogs-1.2.6.dev2/whylogs/core/metrics/decorators.py
+-rw-r--r--   0        0        0     4840 2023-04-11 19:13:37.824666 whylogs-1.2.6.dev2/whylogs/core/metrics/deserializers.py
+-rw-r--r--   0        0        0     1361 2023-01-30 20:46:41.235482 whylogs-1.2.6.dev2/whylogs/core/metrics/maths.py
+-rw-r--r--   0        0        0     6053 2023-01-30 20:46:41.235482 whylogs-1.2.6.dev2/whylogs/core/metrics/metric_components.py
+-rw-r--r--   0        0        0    21749 2023-07-04 17:04:07.025540 whylogs-1.2.6.dev2/whylogs/core/metrics/metrics.py
+-rw-r--r--   0        0        0     8016 2023-06-06 15:22:27.487907 whylogs-1.2.6.dev2/whylogs/core/metrics/multimetric.py
+-rw-r--r--   0        0        0     4517 2023-04-11 19:13:37.824666 whylogs-1.2.6.dev2/whylogs/core/metrics/serializers.py
+-rw-r--r--   0        0        0     5504 2023-01-30 20:46:41.235482 whylogs-1.2.6.dev2/whylogs/core/metrics/unicode_range.py
+-rw-r--r--   0        0        0      107 2023-01-30 20:46:41.235482 whylogs-1.2.6.dev2/whylogs/core/model_performance_metrics/__init__.py
+-rw-r--r--   0        0        0     8976 2023-02-24 20:07:49.042231 whylogs-1.2.6.dev2/whylogs/core/model_performance_metrics/confusion_matrix.py
+-rw-r--r--   0        0        0     7445 2023-02-24 20:07:49.042231 whylogs-1.2.6.dev2/whylogs/core/model_performance_metrics/model_performance_metrics.py
+-rw-r--r--   0        0        0     2837 2023-01-30 20:46:41.235482 whylogs-1.2.6.dev2/whylogs/core/model_performance_metrics/regression_metrics.py
+-rw-r--r--   0        0        0     5499 2023-02-24 20:07:49.042231 whylogs-1.2.6.dev2/whylogs/core/predicate_parser.py
+-rw-r--r--   0        0        0    14489 2023-06-27 17:33:07.374805 whylogs-1.2.6.dev2/whylogs/core/preprocessing.py
+-rw-r--r--   0        0        0      335 2023-01-30 20:46:41.235482 whylogs-1.2.6.dev2/whylogs/core/projectors.py
+-rw-r--r--   0        0        0      183 2023-01-30 20:46:41.235482 whylogs-1.2.6.dev2/whylogs/core/proto/__init__.py
+-rw-r--r--   0        0        0      242 2023-01-30 20:46:41.235482 whylogs-1.2.6.dev2/whylogs/core/proto/v0/__init__.py
+-rw-r--r--   0        0        0    12534 2023-07-19 21:25:42.090943 whylogs-1.2.6.dev2/whylogs/core/proto/v0/v0_constraints_pb2.py
+-rw-r--r--   0        0        0    20212 2023-07-19 21:25:40.880943 whylogs-1.2.6.dev2/whylogs/core/proto/v0/v0_constraints_pb2.pyi
+-rw-r--r--   0        0        0    21343 2023-07-19 21:25:40.880943 whylogs-1.2.6.dev2/whylogs/core/proto/v0/v0_messages_pb2.py
+-rw-r--r--   0        0        0    29724 2023-07-19 21:25:40.880943 whylogs-1.2.6.dev2/whylogs/core/proto/v0/v0_messages_pb2.pyi
+-rw-r--r--   0        0        0    18521 2023-07-19 21:25:42.330943 whylogs-1.2.6.dev2/whylogs/core/proto/v0/v0_summaries_pb2.py
+-rw-r--r--   0        0        0    24739 2023-07-19 21:25:40.880943 whylogs-1.2.6.dev2/whylogs/core/proto/v0/v0_summaries_pb2.pyi
+-rw-r--r--   0        0        0    18571 2023-07-19 21:25:40.680943 whylogs-1.2.6.dev2/whylogs/core/proto/whylogs_messages_pb2.py
+-rw-r--r--   0        0        0    21840 2023-07-19 21:25:40.680943 whylogs-1.2.6.dev2/whylogs/core/proto/whylogs_messages_pb2.pyi
+-rw-r--r--   0        0        0     7350 2023-02-24 20:07:49.042231 whylogs-1.2.6.dev2/whylogs/core/relations.py
+-rw-r--r--   0        0        0    11357 2023-07-19 19:51:34.012366 whylogs-1.2.6.dev2/whylogs/core/resolvers.py
+-rw-r--r--   0        0        0    10029 2023-07-04 17:49:56.925540 whylogs-1.2.6.dev2/whylogs/core/schema.py
+-rw-r--r--   0        0        0      144 2023-01-30 20:46:41.235482 whylogs-1.2.6.dev2/whylogs/core/segment.py
+-rw-r--r--   0        0        0     2343 2023-03-22 21:08:17.851744 whylogs-1.2.6.dev2/whylogs/core/segmentation_partition.py
+-rw-r--r--   0        0        0      826 2023-04-20 13:28:02.623992 whylogs-1.2.6.dev2/whylogs/core/specialized_resolvers.py
+-rw-r--r--   0        0        0     2087 2023-06-27 17:33:07.374805 whylogs-1.2.6.dev2/whylogs/core/stubs.py
+-rw-r--r--   0        0        0      486 2023-06-27 17:33:07.374805 whylogs-1.2.6.dev2/whylogs/core/utils/__init__.py
+-rw-r--r--   0        0        0     3603 2023-06-23 19:18:55.967672 whylogs-1.2.6.dev2/whylogs/core/utils/protobuf_utils.py
+-rw-r--r--   0        0        0     2569 2023-06-27 17:33:07.374805 whylogs-1.2.6.dev2/whylogs/core/utils/stats_calculations.py
+-rw-r--r--   0        0        0      130 2023-01-30 20:46:41.235482 whylogs-1.2.6.dev2/whylogs/core/utils/timestamp_calculations.py
+-rw-r--r--   0        0        0     1602 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/core/utils/utils.py
+-rw-r--r--   0        0        0      210 2023-07-03 16:02:37.106297 whylogs-1.2.6.dev2/whylogs/core/validators/__init__.py
+-rw-r--r--   0        0        0     4760 2023-07-03 16:02:37.106297 whylogs-1.2.6.dev2/whylogs/core/validators/condition_validator.py
+-rw-r--r--   0        0        0      508 2023-03-14 16:58:24.770989 whylogs-1.2.6.dev2/whylogs/core/validators/validator.py
+-rw-r--r--   0        0        0      214 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/core/view/__init__.py
+-rw-r--r--   0        0        0     6157 2023-06-27 17:33:07.374805 whylogs-1.2.6.dev2/whylogs/core/view/column_profile_view.py
+-rw-r--r--   0        0        0    18036 2023-07-19 20:34:51.582366 whylogs-1.2.6.dev2/whylogs/core/view/dataset_profile_view.py
+-rw-r--r--   0        0        0     8747 2023-07-11 15:58:04.999567 whylogs-1.2.6.dev2/whylogs/core/view/segmented_dataset_profile_view.py
+-rw-r--r--   0        0        0      211 2023-02-22 16:52:30.792231 whylogs-1.2.6.dev2/whylogs/datasets/__init__.py
+-rw-r--r--   0        0        0     5813 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/datasets/base.py
+-rw-r--r--   0        0        0     6087 2023-02-22 16:52:30.792231 whylogs-1.2.6.dev2/whylogs/datasets/configs.py
+-rw-r--r--   0        0        0        0 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/datasets/descr/__init__.py
+-rw-r--r--   0        0        0     6397 2023-02-22 16:52:30.792231 whylogs-1.2.6.dev2/whylogs/datasets/descr/ecommerce.rst
+-rw-r--r--   0        0        0     3506 2023-02-22 16:52:30.792231 whylogs-1.2.6.dev2/whylogs/datasets/descr/employee.rst
+-rw-r--r--   0        0        0    11285 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/datasets/descr/weather.rst
+-rw-r--r--   0        0        0    10688 2023-03-24 22:58:37.321744 whylogs-1.2.6.dev2/whylogs/datasets/ecommerce.py
+-rw-r--r--   0        0        0    10981 2023-03-24 22:58:37.321744 whylogs-1.2.6.dev2/whylogs/datasets/employee.py
+-rw-r--r--   0        0        0     2349 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/datasets/utils.py
+-rw-r--r--   0        0        0    11476 2023-03-24 22:58:37.321744 whylogs-1.2.6.dev2/whylogs/datasets/weather.py
+-rw-r--r--   0        0        0        0 2023-03-03 16:19:17.576995 whylogs-1.2.6.dev2/whylogs/experimental/__init__.py
+-rw-r--r--   0        0        0     3530 2023-07-19 19:51:34.012366 whylogs-1.2.6.dev2/whylogs/experimental/api/logger/__init__.py
+-rw-r--r--   0        0        0     3770 2023-06-27 17:33:07.384805 whylogs-1.2.6.dev2/whylogs/experimental/constraints_generation/__init__.py
+-rw-r--r--   0        0        0     1105 2023-06-27 17:33:07.384805 whylogs-1.2.6.dev2/whylogs/experimental/constraints_generation/condition_counts.py
+-rw-r--r--   0        0        0      846 2023-03-28 21:40:50.417571 whylogs-1.2.6.dev2/whylogs/experimental/constraints_generation/count_metrics.py
+-rw-r--r--   0        0        0     1554 2023-06-27 17:33:07.384805 whylogs-1.2.6.dev2/whylogs/experimental/constraints_generation/distribution_metrics.py
+-rw-r--r--   0        0        0     1011 2023-06-27 17:33:07.384805 whylogs-1.2.6.dev2/whylogs/experimental/constraints_generation/frequent_items.py
+-rw-r--r--   0        0        0      685 2023-06-27 17:33:07.384805 whylogs-1.2.6.dev2/whylogs/experimental/constraints_generation/multi_metrics.py
+-rw-r--r--   0        0        0      973 2023-06-27 17:33:07.384805 whylogs-1.2.6.dev2/whylogs/experimental/constraints_generation/types_metrics.py
+-rw-r--r--   0        0        0    19692 2023-07-03 16:02:37.106297 whylogs-1.2.6.dev2/whylogs/experimental/core/metrics/udf_metric.py
+-rw-r--r--   0        0        0    14261 2023-07-19 19:51:34.012366 whylogs-1.2.6.dev2/whylogs/experimental/core/udf_schema.py
+-rw-r--r--   0        0        0     8861 2023-06-27 17:33:07.384805 whylogs-1.2.6.dev2/whylogs/experimental/extras/embedding_metric.py
+-rw-r--r--   0        0        0      939 2023-02-14 19:22:29.792231 whylogs-1.2.6.dev2/whylogs/experimental/extras/matrix_component.py
+-rwxr-xr-x   0        0        0    16737 2023-07-03 16:02:37.106297 whylogs-1.2.6.dev2/whylogs/experimental/extras/nlp_metric.py
+-rw-r--r--   0        0        0        0 2023-03-03 16:19:17.576995 whylogs-1.2.6.dev2/whylogs/experimental/performance_estimation/__init__.py
+-rw-r--r--   0        0        0     1554 2023-04-11 19:13:37.834666 whylogs-1.2.6.dev2/whylogs/experimental/performance_estimation/estimation_results.py
+-rw-r--r--   0        0        0     8872 2023-03-03 16:19:17.576995 whylogs-1.2.6.dev2/whylogs/experimental/performance_estimation/estimators.py
+-rw-r--r--   0        0        0     3777 2023-06-27 17:33:07.394805 whylogs-1.2.6.dev2/whylogs/experimental/preprocess/embeddings/selectors.py
+-rw-r--r--   0        0        0    10031 2023-05-17 03:09:27.542898 whylogs-1.2.6.dev2/whylogs/extras/image_metric.py
+-rw-r--r--   0        0        0       52 2023-02-27 17:39:54.122231 whylogs-1.2.6.dev2/whylogs/migration/__init__.py
+-rw-r--r--   0        0        0    15367 2023-06-12 01:38:17.812653 whylogs-1.2.6.dev2/whylogs/migration/converters.py
+-rw-r--r--   0        0        0     6959 2023-06-23 19:18:55.967672 whylogs-1.2.6.dev2/whylogs/migration/uncompound.py
+-rw-r--r--   0        0        0      296 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/__init__.py
+-rw-r--r--   0        0        0      168 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/configs.py
+-rw-r--r--   0        0        0        0 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/drift/__init__.py
+-rw-r--r--   0        0        0    21751 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/drift/column_drift_algorithms.py
+-rw-r--r--   0        0        0     1366 2023-03-24 22:58:37.321744 whylogs-1.2.6.dev2/whylogs/viz/drift/configs.py
+-rw-r--r--   0        0        0        0 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/enums/__init__.py
+-rw-r--r--   0        0        0      901 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/enums/enums.py
+-rw-r--r--   0        0        0        0 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/extensions/__init__.py
+-rw-r--r--   0        0        0      114 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/extensions/reports/constraints.py
+-rw-r--r--   0        0        0      272 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/extensions/reports/histograms.py
+-rw-r--r--   0        0        0     2502 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/extensions/reports/html_report.py
+-rw-r--r--   0        0        0      975 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/extensions/reports/profile_summary.py
+-rw-r--r--   0        0        0     3218 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/extensions/reports/summary_drift.py
+-rw-r--r--   0        0        0       38 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/.prettierignore
+-rw-r--r--   0        0        0      135 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/.prettierrc.yaml
+-rw-r--r--   0        0        0   155568 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/css/bootstrap.min.css
+-rw-r--r--   0        0        0    22747 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/css/whylogs-styles.css
+-rw-r--r--   0        0        0   160788 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-Bold.ttf
+-rw-r--r--   0        0        0    50888 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-Bold.woff
+-rw-r--r--   0        0        0    32180 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-Bold.woff2
+-rw-r--r--   0        0        0   172144 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-BoldItalic.ttf
+-rw-r--r--   0        0        0    55560 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-BoldItalic.woff
+-rw-r--r--   0        0        0    35476 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-BoldItalic.woff2
+-rw-r--r--   0        0        0   172188 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-Italic.ttf
+-rw-r--r--   0        0        0    55728 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-Italic.woff
+-rw-r--r--   0        0        0    35144 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-Italic.woff2
+-rw-r--r--   0        0        0   161212 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-Medium.ttf
+-rw-r--r--   0        0        0    53244 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-Medium.woff
+-rw-r--r--   0        0        0    34516 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-Medium.woff2
+-rw-r--r--   0        0        0   172380 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-MediumItalic.ttf
+-rw-r--r--   0        0        0    59012 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-MediumItalic.woff
+-rw-r--r--   0        0        0    38404 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-MediumItalic.woff2
+-rw-r--r--   0        0        0   161220 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-Regular.ttf
+-rw-r--r--   0        0        0    50936 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-Regular.woff
+-rw-r--r--   0        0        0    32192 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-Regular.woff2
+-rw-r--r--   0        0        0   161152 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-SemiBold.ttf
+-rw-r--r--   0        0        0    53296 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-SemiBold.woff
+-rw-r--r--   0        0        0    34744 2023-01-30 20:46:41.245482 whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-SemiBold.woff2
+-rw-r--r--   0        0        0   172396 2023-01-30 20:46:41.255482 whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf
+-rw-r--r--   0        0        0    58892 2023-01-30 20:46:41.255482 whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff
+-rw-r--r--   0        0        0    38500 2023-01-30 20:46:41.255482 whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2
+-rw-r--r--   0        0        0     3156 2023-01-30 20:46:41.255482 whylogs-1.2.6.dev2/whylogs/viz/html/images/placement-chart.png
+-rw-r--r--   0        0        0     9649 2023-01-30 20:46:41.255482 whylogs-1.2.6.dev2/whylogs/viz/html/images/whylabs-favicon.png
+-rw-r--r--   0        0        0   270687 2023-01-30 20:46:41.255482 whylogs-1.2.6.dev2/whylogs/viz/html/js/d3.min.js
+-rw-r--r--   0        0        0    12606 2023-01-30 20:46:41.255482 whylogs-1.2.6.dev2/whylogs/viz/html/js/handlebars.js
+-rw-r--r--   0        0        0    89501 2023-01-30 20:46:41.255482 whylogs-1.2.6.dev2/whylogs/viz/html/js/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0    55927 2023-01-30 20:46:41.255482 whylogs-1.2.6.dev2/whylogs/viz/html/js/whylogs-script.js
+-rw-r--r--   0        0        0    52663 2023-01-30 20:46:41.255482 whylogs-1.2.6.dev2/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html
+-rw-r--r--   0        0        0    14235 2023-01-30 20:46:41.255482 whylogs-1.2.6.dev2/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html
+-rw-r--r--   0        0        0    26825 2023-05-25 19:20:19.432537 whylogs-1.2.6.dev2/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html
+-rw-r--r--   0        0        0    14144 2023-01-30 20:46:41.255482 whylogs-1.2.6.dev2/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html
+-rw-r--r--   0        0        0    15177 2023-04-20 13:28:02.623992 whylogs-1.2.6.dev2/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html
+-rw-r--r--   0        0        0    18298 2023-01-30 20:46:41.255482 whylogs-1.2.6.dev2/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html
+-rw-r--r--   0        0        0    41933 2023-01-30 20:46:41.265482 whylogs-1.2.6.dev2/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html
+-rw-r--r--   0        0        0    98500 2023-01-30 20:46:41.265482 whylogs-1.2.6.dev2/whylogs/viz/html/templates/index-hbs-cdn-all-in.html
+-rw-r--r--   0        0        0   752494 2023-01-30 20:46:41.265482 whylogs-1.2.6.dev2/whylogs/viz/html/templates/index-hbs-library-all-in.html
+-rw-r--r--   0        0        0    25371 2023-01-30 20:46:41.265482 whylogs-1.2.6.dev2/whylogs/viz/html/templates/index-hbs.html
+-rw-r--r--   0        0        0    26014 2023-01-30 20:46:41.265482 whylogs-1.2.6.dev2/whylogs/viz/html/templates/index.html
+-rw-r--r--   0        0        0    21376 2023-04-11 19:13:37.834666 whylogs-1.2.6.dev2/whylogs/viz/notebook_profile_viz.py
+-rw-r--r--   0        0        0      410 2023-01-30 20:46:41.265482 whylogs-1.2.6.dev2/whylogs/viz/utils/__init__.py
+-rw-r--r--   0        0        0     2466 2023-01-30 20:46:41.265482 whylogs-1.2.6.dev2/whylogs/viz/utils/descriptive_stats.py
+-rw-r--r--   0        0        0    12576 2023-01-30 20:46:41.265482 whylogs-1.2.6.dev2/whylogs/viz/utils/drift_calculations.py
+-rw-r--r--   0        0        0     3561 2023-04-20 13:28:02.623992 whylogs-1.2.6.dev2/whylogs/viz/utils/frequent_items_calculations.py
+-rw-r--r--   0        0        0     2747 2023-01-30 20:46:41.265482 whylogs-1.2.6.dev2/whylogs/viz/utils/histogram_calculations.py
+-rw-r--r--   0        0        0     1060 2023-04-20 13:28:02.623992 whylogs-1.2.6.dev2/whylogs/viz/utils/html_template_utils.py
+-rw-r--r--   0        0        0    14298 2023-01-30 20:46:41.265482 whylogs-1.2.6.dev2/whylogs/viz/utils/profile_viz_calculations.py
+-rw-r--r--   0        0        0     3581 2023-01-30 20:46:41.265482 whylogs-1.2.6.dev2/whylogs/viz/utils/quantile_stats.py
+-rw-r--r--   0        0        0     6563 1970-01-01 00:00:00.000000 whylogs-1.2.6.dev2/PKG-INFO
```

### Comparing `whylogs-1.2.6.dev0/DESCRIPTION.md` & `whylogs-1.2.6.dev2/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/pyproject.toml` & `whylogs-1.2.6.dev2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whylogs"
-version = "1.2.6-dev0"
+version = "1.2.6-dev2"
 description = "Profile and monitor your ML data pipeline end-to-end"
 authors = ["WhyLabs.ai <support@whylabs.ai>"]
 license = "Apache-2.0"
 homepage = "https://docs.whylabs.ai"
 readme = "DESCRIPTION.md"
 include = ["whylogs/core/proto/v0/*.py*", "whylogs/core/proto/*.py*"]
```

### Comparing `whylogs-1.2.6.dev0/whylogs/__init__.py` & `whylogs-1.2.6.dev2/whylogs/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/annotations.py` & `whylogs-1.2.6.dev2/whylogs/api/annotations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/fugue/profiler.py` & `whylogs-1.2.6.dev2/whylogs/api/fugue/profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/fugue/registry.py` & `whylogs-1.2.6.dev2/whylogs/api/fugue/registry.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/logger/__init__.py` & `whylogs-1.2.6.dev2/whylogs/api/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/logger/experimental/multi_dataset_logger/message_processor.py` & `whylogs-1.2.6.dev2/whylogs/api/logger/experimental/multi_dataset_logger/message_processor.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/logger/experimental/multi_dataset_logger/multi_dataset_rolling_logger.py` & `whylogs-1.2.6.dev2/whylogs/api/logger/experimental/multi_dataset_logger/multi_dataset_rolling_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/logger/experimental/multi_dataset_logger/time_util.py` & `whylogs-1.2.6.dev2/whylogs/api/logger/experimental/multi_dataset_logger/time_util.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/logger/logger.py` & `whylogs-1.2.6.dev2/whylogs/api/logger/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,14 @@
         if active_schema and active_schema.segments:
             return segment_processing(active_schema, obj, pandas, row, self._segment_cache)
 
         profiles = self._get_matching_profiles(obj, pandas=pandas, row=row, schema=active_schema)
 
         for prof in profiles:
             prof.track(obj, pandas=pandas, row=row, execute_udfs=False)
-            prof._metadata
 
         first_profile = profiles[0]
         if name is not None:
             if first_profile._metadata is None:
                 first_profile._metadata = dict()
             first_profile._metadata["name"] = name
         return ProfileResultSet(first_profile)
```

### Comparing `whylogs-1.2.6.dev0/whylogs/api/logger/result_set.py` & `whylogs-1.2.6.dev2/whylogs/api/logger/result_set.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/logger/rolling.py` & `whylogs-1.2.6.dev2/whylogs/api/logger/rolling.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/logger/segment_cache.py` & `whylogs-1.2.6.dev2/whylogs/api/logger/segment_cache.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/logger/segment_processing.py` & `whylogs-1.2.6.dev2/whylogs/api/logger/segment_processing.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/logger/transient.py` & `whylogs-1.2.6.dev2/whylogs/api/logger/transient.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/pyspark/experimental/profiler.py` & `whylogs-1.2.6.dev2/whylogs/api/pyspark/experimental/profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/pyspark/experimental/segmented_profiler.py` & `whylogs-1.2.6.dev2/whylogs/api/pyspark/experimental/segmented_profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/reader/local.py` & `whylogs-1.2.6.dev2/whylogs/api/reader/local.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/reader/reader.py` & `whylogs-1.2.6.dev2/whylogs/api/reader/reader.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/reader/s3.py` & `whylogs-1.2.6.dev2/whylogs/api/reader/s3.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/store/local_store.py` & `whylogs-1.2.6.dev2/whylogs/api/store/local_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/store/profile_store.py` & `whylogs-1.2.6.dev2/whylogs/api/store/profile_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/store/query.py` & `whylogs-1.2.6.dev2/whylogs/api/store/query.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/store/sqlite_store.py` & `whylogs-1.2.6.dev2/whylogs/api/store/sqlite_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/usage_stats/__init__.py` & `whylogs-1.2.6.dev2/whylogs/api/usage_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/whylabs/session/config.py` & `whylogs-1.2.6.dev2/whylogs/api/whylabs/session/config.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/whylabs/session/notebook_logger.py` & `whylogs-1.2.6.dev2/whylogs/api/whylabs/session/notebook_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/whylabs/session/session_manager.py` & `whylogs-1.2.6.dev2/whylogs/api/whylabs/session/session_manager.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/whylabs/session/session_types.py` & `whylogs-1.2.6.dev2/whylogs/api/whylabs/session/session_types.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/writer/__init__.py` & `whylogs-1.2.6.dev2/whylogs/api/writer/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/writer/gcs.py` & `whylogs-1.2.6.dev2/whylogs/api/writer/gcs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/writer/local.py` & `whylogs-1.2.6.dev2/whylogs/api/writer/local.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/writer/mlflow.py` & `whylogs-1.2.6.dev2/whylogs/api/writer/mlflow.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/writer/s3.py` & `whylogs-1.2.6.dev2/whylogs/api/writer/s3.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/writer/whylabs.py` & `whylogs-1.2.6.dev2/whylogs/api/writer/whylabs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/api/writer/writer.py` & `whylogs-1.2.6.dev2/whylogs/api/writer/writer.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/__init__.py` & `whylogs-1.2.6.dev2/whylogs/core/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/column_profile.py` & `whylogs-1.2.6.dev2/whylogs/core/column_profile.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/configs.py` & `whylogs-1.2.6.dev2/whylogs/core/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/constraints/factories/__init__.py` & `whylogs-1.2.6.dev2/whylogs/core/constraints/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/constraints/factories/cardinality_metrics.py` & `whylogs-1.2.6.dev2/whylogs/core/constraints/factories/cardinality_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/constraints/factories/condition_counts.py` & `whylogs-1.2.6.dev2/whylogs/core/constraints/factories/condition_counts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/constraints/factories/count_metrics.py` & `whylogs-1.2.6.dev2/whylogs/core/constraints/factories/count_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/constraints/factories/distribution_metrics.py` & `whylogs-1.2.6.dev2/whylogs/core/constraints/factories/distribution_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/constraints/factories/frequent_items.py` & `whylogs-1.2.6.dev2/whylogs/core/constraints/factories/frequent_items.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/constraints/factories/multi_metrics.py` & `whylogs-1.2.6.dev2/whylogs/core/constraints/factories/multi_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/constraints/factories/types_metrics.py` & `whylogs-1.2.6.dev2/whylogs/core/constraints/factories/types_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/constraints/metric_constraints.py` & `whylogs-1.2.6.dev2/whylogs/core/constraints/metric_constraints.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/dataset_profile.py` & `whylogs-1.2.6.dev2/whylogs/core/dataset_profile.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/datatypes.py` & `whylogs-1.2.6.dev2/whylogs/core/datatypes.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/errors.py` & `whylogs-1.2.6.dev2/whylogs/core/errors.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/feature_weights.py` & `whylogs-1.2.6.dev2/whylogs/core/feature_weights.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/input_resolver.py` & `whylogs-1.2.6.dev2/whylogs/core/input_resolver.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/metric_getters.py` & `whylogs-1.2.6.dev2/whylogs/core/metric_getters.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/metrics/__init__.py` & `whylogs-1.2.6.dev2/whylogs/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/metrics/aggregators.py` & `whylogs-1.2.6.dev2/whylogs/core/metrics/aggregators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/metrics/column_metrics.py` & `whylogs-1.2.6.dev2/whylogs/core/metrics/column_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/metrics/compound_metric.py` & `whylogs-1.2.6.dev2/whylogs/core/metrics/compound_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/metrics/condition_count_metric.py` & `whylogs-1.2.6.dev2/whylogs/core/metrics/condition_count_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/metrics/decorators.py` & `whylogs-1.2.6.dev2/whylogs/core/metrics/decorators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/metrics/deserializers.py` & `whylogs-1.2.6.dev2/whylogs/core/metrics/deserializers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/metrics/maths.py` & `whylogs-1.2.6.dev2/whylogs/core/metrics/maths.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/metrics/metric_components.py` & `whylogs-1.2.6.dev2/whylogs/core/metrics/metric_components.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/metrics/metrics.py` & `whylogs-1.2.6.dev2/whylogs/core/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/metrics/multimetric.py` & `whylogs-1.2.6.dev2/whylogs/core/metrics/multimetric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/metrics/serializers.py` & `whylogs-1.2.6.dev2/whylogs/core/metrics/serializers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/metrics/unicode_range.py` & `whylogs-1.2.6.dev2/whylogs/core/metrics/unicode_range.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/model_performance_metrics/confusion_matrix.py` & `whylogs-1.2.6.dev2/whylogs/core/model_performance_metrics/confusion_matrix.py`

 * *Files 6% similar despite different names*

```diff
@@ -157,20 +157,15 @@
             compact_theta=EMPTY_THETA,
             variance=variance_message,
             doubles=DoublesMessage(count=dist.n),
         )
 
     @staticmethod
     def _numbers_to_dist(numbers: NumbersMessageV0) -> DistributionMetric:
-        try:
-            doubles_sk = ds.kll_doubles_sketch.deserialize(numbers.histogram)
-        except ValueError:
-            # Fall back to KLL float for backward compatibility and convert it to doubles sketch
-            sk = ds.kll_floats_sketch.deserialize(numbers.histogram)
-            doubles_sk = ds.kll_floats_sketch.float_to_doubles(sk)
+        doubles_sk = ds.kll_doubles_sketch.deserialize(numbers.histogram)
         return DistributionMetric(
             kll=KllComponent(doubles_sk),
             mean=FractionalComponent(numbers.variance.mean),
             m2=FractionalComponent(numbers.variance.sum),
         )
 
     def to_protobuf(
```

### Comparing `whylogs-1.2.6.dev0/whylogs/core/model_performance_metrics/model_performance_metrics.py` & `whylogs-1.2.6.dev2/whylogs/core/model_performance_metrics/model_performance_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/model_performance_metrics/regression_metrics.py` & `whylogs-1.2.6.dev2/whylogs/core/model_performance_metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/predicate_parser.py` & `whylogs-1.2.6.dev2/whylogs/core/predicate_parser.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/preprocessing.py` & `whylogs-1.2.6.dev2/whylogs/core/preprocessing.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/proto/v0/v0_constraints_pb2.pyi` & `whylogs-1.2.6.dev2/whylogs/core/proto/v0/v0_constraints_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/proto/v0/v0_messages_pb2.pyi` & `whylogs-1.2.6.dev2/whylogs/core/proto/v0/v0_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/proto/v0/v0_summaries_pb2.pyi` & `whylogs-1.2.6.dev2/whylogs/core/proto/v0/v0_summaries_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/proto/whylogs_messages_pb2.pyi` & `whylogs-1.2.6.dev2/whylogs/core/proto/whylogs_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/relations.py` & `whylogs-1.2.6.dev2/whylogs/core/relations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/resolvers.py` & `whylogs-1.2.6.dev2/whylogs/core/resolvers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/schema.py` & `whylogs-1.2.6.dev2/whylogs/core/schema.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/segmentation_partition.py` & `whylogs-1.2.6.dev2/whylogs/core/segmentation_partition.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/specialized_resolvers.py` & `whylogs-1.2.6.dev2/whylogs/core/specialized_resolvers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/stubs.py` & `whylogs-1.2.6.dev2/whylogs/core/stubs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/utils/protobuf_utils.py` & `whylogs-1.2.6.dev2/whylogs/core/utils/protobuf_utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/utils/stats_calculations.py` & `whylogs-1.2.6.dev2/whylogs/core/utils/stats_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/utils/utils.py` & `whylogs-1.2.6.dev2/whylogs/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/validators/condition_validator.py` & `whylogs-1.2.6.dev2/whylogs/core/validators/condition_validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/view/column_profile_view.py` & `whylogs-1.2.6.dev2/whylogs/core/view/column_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/core/view/dataset_profile_view.py` & `whylogs-1.2.6.dev2/whylogs/core/view/dataset_profile_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,15 +252,15 @@
         metric_index_to_name: Dict[int, str] = {}
         for i in range(0, len(metric_name_list)):
             metric_name_indices[metric_name_list[i]] = i
             metric_index_to_name[i] = metric_name_list[i]
         column_chunk_offsets: Dict[str, ChunkOffsets] = {}
         with tempfile.TemporaryFile("w+b") as f:
             for col_name in sorted(self._columns.keys()):
-                column_chunk_offsets[col_name] = ChunkOffsets(offsets=[f.tell()])
+                column_chunk_offsets[str(col_name)] = ChunkOffsets(offsets=[f.tell()])
 
                 col = self._columns[col_name]
 
                 # for a given column, turn it into a ChunkMessage.
                 indexed_component_messages: Dict[int, MetricComponentMessage] = {}
                 metric_components = col.to_protobuf().metric_components
                 for m_name, m_component in metric_components.items():
@@ -280,20 +280,27 @@
 
             properties = DatasetProperties(
                 dataset_timestamp=to_utc_milliseconds(self._dataset_timestamp),
                 creation_timestamp=to_utc_milliseconds(self._creation_timestamp),
                 tags=tags,
                 metadata=metadata,
             )
-            dataset_header = DatasetProfileHeader(
-                column_offsets=column_chunk_offsets,
-                properties=properties,
-                length=total_len,
-                indexed_metric_paths=metric_index_to_name,
-            )
+            try:
+                dataset_header = DatasetProfileHeader(
+                    column_offsets=column_chunk_offsets,
+                    properties=properties,
+                    length=total_len,
+                    indexed_metric_paths=metric_index_to_name,
+                )
+            except Exception as e:
+                raise DeserializationError(
+                    f"DatasetProfileHeader(column_offsets={column_chunk_offsets}, "
+                    f"properties={properties}, length={total_len}, "
+                    f"indexed_metric_paths={metric_index_to_name}): -> {e}",
+                )
 
             # single file segments
             dataset_segment_header = DatasetSegmentHeader(
                 has_segments=False,
             )
 
             out_f.write(WHYLOGS_MAGIC_HEADER_BYTES)
```

### Comparing `whylogs-1.2.6.dev0/whylogs/core/view/segmented_dataset_profile_view.py` & `whylogs-1.2.6.dev2/whylogs/core/view/segmented_dataset_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/datasets/base.py` & `whylogs-1.2.6.dev2/whylogs/datasets/base.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/datasets/configs.py` & `whylogs-1.2.6.dev2/whylogs/datasets/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/datasets/descr/ecommerce.rst` & `whylogs-1.2.6.dev2/whylogs/datasets/descr/ecommerce.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/datasets/descr/employee.rst` & `whylogs-1.2.6.dev2/whylogs/datasets/descr/employee.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/datasets/descr/weather.rst` & `whylogs-1.2.6.dev2/whylogs/datasets/descr/weather.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/datasets/ecommerce.py` & `whylogs-1.2.6.dev2/whylogs/datasets/ecommerce.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/datasets/employee.py` & `whylogs-1.2.6.dev2/whylogs/datasets/employee.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/datasets/utils.py` & `whylogs-1.2.6.dev2/whylogs/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/datasets/weather.py` & `whylogs-1.2.6.dev2/whylogs/datasets/weather.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/experimental/api/logger/__init__.py` & `whylogs-1.2.6.dev2/whylogs/experimental/api/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/experimental/constraints_generation/__init__.py` & `whylogs-1.2.6.dev2/whylogs/experimental/constraints_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/experimental/constraints_generation/condition_counts.py` & `whylogs-1.2.6.dev2/whylogs/experimental/constraints_generation/condition_counts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/experimental/constraints_generation/count_metrics.py` & `whylogs-1.2.6.dev2/whylogs/experimental/constraints_generation/count_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/experimental/constraints_generation/distribution_metrics.py` & `whylogs-1.2.6.dev2/whylogs/experimental/constraints_generation/distribution_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/experimental/constraints_generation/frequent_items.py` & `whylogs-1.2.6.dev2/whylogs/experimental/constraints_generation/frequent_items.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/experimental/constraints_generation/multi_metrics.py` & `whylogs-1.2.6.dev2/whylogs/experimental/constraints_generation/multi_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/experimental/constraints_generation/types_metrics.py` & `whylogs-1.2.6.dev2/whylogs/experimental/constraints_generation/types_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/experimental/core/metrics/udf_metric.py` & `whylogs-1.2.6.dev2/whylogs/experimental/core/metrics/udf_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/experimental/core/udf_schema.py` & `whylogs-1.2.6.dev2/whylogs/experimental/core/udf_schema.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/experimental/extras/embedding_metric.py` & `whylogs-1.2.6.dev2/whylogs/experimental/extras/embedding_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/experimental/extras/matrix_component.py` & `whylogs-1.2.6.dev2/whylogs/experimental/extras/matrix_component.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/experimental/extras/nlp_metric.py` & `whylogs-1.2.6.dev2/whylogs/experimental/extras/nlp_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/experimental/performance_estimation/estimation_results.py` & `whylogs-1.2.6.dev2/whylogs/experimental/performance_estimation/estimation_results.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/experimental/performance_estimation/estimators.py` & `whylogs-1.2.6.dev2/whylogs/experimental/performance_estimation/estimators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/experimental/preprocess/embeddings/selectors.py` & `whylogs-1.2.6.dev2/whylogs/experimental/preprocess/embeddings/selectors.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/extras/image_metric.py` & `whylogs-1.2.6.dev2/whylogs/extras/image_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/migration/converters.py` & `whylogs-1.2.6.dev2/whylogs/migration/converters.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/migration/uncompound.py` & `whylogs-1.2.6.dev2/whylogs/migration/uncompound.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/drift/column_drift_algorithms.py` & `whylogs-1.2.6.dev2/whylogs/viz/drift/column_drift_algorithms.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/drift/configs.py` & `whylogs-1.2.6.dev2/whylogs/viz/drift/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/enums/enums.py` & `whylogs-1.2.6.dev2/whylogs/viz/enums/enums.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/extensions/reports/html_report.py` & `whylogs-1.2.6.dev2/whylogs/viz/extensions/reports/html_report.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/extensions/reports/profile_summary.py` & `whylogs-1.2.6.dev2/whylogs/viz/extensions/reports/profile_summary.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/extensions/reports/summary_drift.py` & `whylogs-1.2.6.dev2/whylogs/viz/extensions/reports/summary_drift.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/css/bootstrap.min.css` & `whylogs-1.2.6.dev2/whylogs/viz/html/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/css/whylogs-styles.css` & `whylogs-1.2.6.dev2/whylogs/viz/html/css/whylogs-styles.css`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-Bold.ttf` & `whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-Bold.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-Bold.woff` & `whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-Bold.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-Bold.woff2` & `whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-Bold.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.ttf` & `whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.woff` & `whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.woff2` & `whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-Italic.ttf` & `whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-Italic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-Italic.woff` & `whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-Italic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-Italic.woff2` & `whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-Italic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-Medium.ttf` & `whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-Medium.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-Medium.woff` & `whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-Medium.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-Medium.woff2` & `whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-Medium.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.ttf` & `whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.woff` & `whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-MediumItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.woff2` & `whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-MediumItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-Regular.ttf` & `whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-Regular.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-Regular.woff` & `whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-Regular.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-Regular.woff2` & `whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-Regular.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-SemiBold.ttf` & `whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-SemiBold.woff` & `whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-SemiBold.woff2` & `whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf` & `whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff` & `whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2` & `whylogs-1.2.6.dev2/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/images/placement-chart.png` & `whylogs-1.2.6.dev2/whylogs/viz/html/images/placement-chart.png`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/images/whylabs-favicon.png` & `whylogs-1.2.6.dev2/whylogs/viz/html/images/whylabs-favicon.png`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/js/d3.min.js` & `whylogs-1.2.6.dev2/whylogs/viz/html/js/d3.min.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/js/handlebars.js` & `whylogs-1.2.6.dev2/whylogs/viz/html/js/handlebars.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/js/jquery-3.6.0.min.js` & `whylogs-1.2.6.dev2/whylogs/viz/html/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/js/whylogs-script.js` & `whylogs-1.2.6.dev2/whylogs/viz/html/js/whylogs-script.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html` & `whylogs-1.2.6.dev2/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html` & `whylogs-1.2.6.dev2/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html` & `whylogs-1.2.6.dev2/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html` & `whylogs-1.2.6.dev2/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html` & `whylogs-1.2.6.dev2/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html` & `whylogs-1.2.6.dev2/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html` & `whylogs-1.2.6.dev2/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in.html` & `whylogs-1.2.6.dev2/whylogs/viz/html/templates/index-hbs-cdn-all-in.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/templates/index-hbs-library-all-in.html` & `whylogs-1.2.6.dev2/whylogs/viz/html/templates/index-hbs-library-all-in.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/templates/index-hbs.html` & `whylogs-1.2.6.dev2/whylogs/viz/html/templates/index-hbs.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/html/templates/index.html` & `whylogs-1.2.6.dev2/whylogs/viz/html/templates/index.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/notebook_profile_viz.py` & `whylogs-1.2.6.dev2/whylogs/viz/notebook_profile_viz.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/utils/descriptive_stats.py` & `whylogs-1.2.6.dev2/whylogs/viz/utils/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/utils/drift_calculations.py` & `whylogs-1.2.6.dev2/whylogs/viz/utils/drift_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/utils/frequent_items_calculations.py` & `whylogs-1.2.6.dev2/whylogs/viz/utils/frequent_items_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/utils/histogram_calculations.py` & `whylogs-1.2.6.dev2/whylogs/viz/utils/histogram_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/utils/html_template_utils.py` & `whylogs-1.2.6.dev2/whylogs/viz/utils/html_template_utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/utils/profile_viz_calculations.py` & `whylogs-1.2.6.dev2/whylogs/viz/utils/profile_viz_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/whylogs/viz/utils/quantile_stats.py` & `whylogs-1.2.6.dev2/whylogs/viz/utils/quantile_stats.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.6.dev0/PKG-INFO` & `whylogs-1.2.6.dev2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 Metadata-Version: 2.1
 Name: whylogs
-Version: 1.2.6.dev0
+Version: 1.2.6.dev2
 Summary: Profile and monitor your ML data pipeline end-to-end
 Home-page: https://docs.whylabs.ai
 License: Apache-2.0
 Author: WhyLabs.ai
 Author-email: support@whylabs.ai
 Requires-Python: >=3.7.1,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: datasets
 Provides-Extra: docs
 Provides-Extra: embeddings
 Provides-Extra: fugue
 Provides-Extra: gcs
 Provides-Extra: image
 Provides-Extra: mlflow
 Provides-Extra: s3
 Provides-Extra: spark
 Provides-Extra: viz
-Requires-Dist: Pillow (>=9.2.0,<10.0.0); extra == "viz" or extra == "image" or extra == "all"
-Requires-Dist: boto3 (>=1.22.13,<2.0.0); extra == "s3" or extra == "all"
-Requires-Dist: fugue (>=0.8.1,<0.9.0); extra == "fugue" or extra == "all"
-Requires-Dist: furo (>=2022.3.4,<2023.0.0); extra == "docs"
-Requires-Dist: google-cloud-storage (>=2.5.0,<3.0.0); extra == "gcs" or extra == "all"
-Requires-Dist: importlib-metadata (<4.3); python_version < "3.8"
-Requires-Dist: ipython; extra == "viz" or extra == "all"
-Requires-Dist: ipython_genutils (>=0.2.0,<0.3.0); extra == "docs"
-Requires-Dist: mlflow-skinny (>=1.26.1,<2.0.0); extra == "mlflow" or extra == "all"
-Requires-Dist: myst-parser[sphinx] (>=0.17.2,<0.18.0); extra == "docs"
-Requires-Dist: nbconvert (>=7.0.0,<8.0.0); extra == "docs"
-Requires-Dist: nbsphinx (>=0.8.9,<0.9.0); extra == "docs"
-Requires-Dist: numpy (>=1.23.2); (python_version >= "3.11") and (extra == "viz" or extra == "embeddings" or extra == "all")
-Requires-Dist: numpy; (python_version < "3.11") and (extra == "viz" or extra == "embeddings" or extra == "all")
-Requires-Dist: pandas; extra == "datasets" or extra == "all"
+Requires-Dist: Pillow (>=9.2.0,<10.0.0) ; extra == "viz" or extra == "image" or extra == "all"
+Requires-Dist: boto3 (>=1.22.13,<2.0.0) ; extra == "s3" or extra == "all"
+Requires-Dist: fugue (>=0.8.1,<0.9.0) ; extra == "fugue" or extra == "all"
+Requires-Dist: furo (>=2022.3.4,<2023.0.0) ; extra == "docs"
+Requires-Dist: google-cloud-storage (>=2.5.0,<3.0.0) ; extra == "gcs" or extra == "all"
+Requires-Dist: importlib-metadata (<4.3) ; python_version < "3.8"
+Requires-Dist: ipython ; extra == "viz" or extra == "all"
+Requires-Dist: ipython_genutils (>=0.2.0,<0.3.0) ; extra == "docs"
+Requires-Dist: mlflow-skinny (>=1.26.1,<2.0.0) ; extra == "mlflow" or extra == "all"
+Requires-Dist: myst-parser[sphinx] (>=0.17.2,<0.18.0) ; extra == "docs"
+Requires-Dist: nbconvert (>=7.0.0,<8.0.0) ; extra == "docs"
+Requires-Dist: nbsphinx (>=0.8.9,<0.9.0) ; extra == "docs"
+Requires-Dist: numpy (>=1.23.2) ; (python_version >= "3.11") and (extra == "viz" or extra == "embeddings" or extra == "all")
+Requires-Dist: numpy ; (python_version < "3.11") and (extra == "viz" or extra == "embeddings" or extra == "all")
+Requires-Dist: pandas ; extra == "datasets" or extra == "all"
 Requires-Dist: platformdirs (>=3.5.0,<4.0.0)
 Requires-Dist: protobuf (>=3.19.4)
-Requires-Dist: pyarrow (>=8.0.0,<13); extra == "spark" or extra == "all"
-Requires-Dist: pybars3 (>=0.9,<0.10); extra == "viz" or extra == "all"
-Requires-Dist: pyspark (>=3.0.0,<4.0.0); extra == "spark" or extra == "all"
+Requires-Dist: pyarrow (>=8.0.0,<13) ; extra == "spark" or extra == "all"
+Requires-Dist: pybars3 (>=0.9,<0.10) ; extra == "viz" or extra == "all"
+Requires-Dist: pyspark (>=3.0.0,<4.0.0) ; extra == "spark" or extra == "all"
 Requires-Dist: requests (>=2.27,<3.0)
-Requires-Dist: scikit-learn (>=1.0.2,<2.0.0); (python_version < "3.11") and (extra == "embeddings" or extra == "all")
-Requires-Dist: scikit-learn (>=1.1.2,<2); (python_version >= "3.11") and (extra == "embeddings" or extra == "all")
-Requires-Dist: scipy (>=1.5); (python_version < "3.11") and (extra == "viz" or extra == "all")
-Requires-Dist: scipy (>=1.9.2); (python_version >= "3.11") and (extra == "viz" or extra == "all")
-Requires-Dist: sphinx-autoapi; extra == "docs"
-Requires-Dist: sphinx-autobuild (>=2021.3.14,<2022.0.0); extra == "docs"
-Requires-Dist: sphinx-copybutton (>=0.5.0,<0.6.0); extra == "docs"
-Requires-Dist: sphinx-inline-tabs; (python_version >= "3.8" and python_version < "4") and (extra == "docs")
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: sphinxext-opengraph (>=0.6.3,<0.7.0); extra == "docs"
+Requires-Dist: scikit-learn (>=1.0.2,<2.0.0) ; (python_version < "3.11") and (extra == "embeddings" or extra == "all")
+Requires-Dist: scikit-learn (>=1.1.2,<2) ; (python_version >= "3.11") and (extra == "embeddings" or extra == "all")
+Requires-Dist: scipy (>=1.5) ; (python_version < "3.11") and (extra == "viz" or extra == "all")
+Requires-Dist: scipy (>=1.9.2) ; (python_version >= "3.11") and (extra == "viz" or extra == "all")
+Requires-Dist: sphinx ; extra == "docs"
+Requires-Dist: sphinx-autoapi ; extra == "docs"
+Requires-Dist: sphinx-autobuild (>=2021.3.14,<2022.0.0) ; extra == "docs"
+Requires-Dist: sphinx-copybutton (>=0.5.0,<0.6.0) ; extra == "docs"
+Requires-Dist: sphinx-inline-tabs ; (python_version >= "3.8" and python_version < "4") and (extra == "docs")
+Requires-Dist: sphinxext-opengraph (>=0.6.3,<0.7.0) ; extra == "docs"
 Requires-Dist: types-requests (>=2.30.0.0,<3.0.0.0)
-Requires-Dist: typing-extensions (>=3.10); python_version < "4"
+Requires-Dist: typing-extensions (>=3.10) ; python_version < "4"
 Requires-Dist: whylabs-client (>=0.5.1,<1)
 Requires-Dist: whylogs-sketching (>=3.4.1.dev3)
 Description-Content-Type: text/markdown
 
 <img src="https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82" /><p align="center">
 <img src="https://i.imgur.com/nv33goV.png" width="35%"/>
 </br>
```

#### html2text {}

```diff
@@ -1,52 +1,54 @@
-Metadata-Version: 2.1 Name: whylogs Version: 1.2.6.dev0 Summary: Profile and
+Metadata-Version: 2.1 Name: whylogs Version: 1.2.6.dev2 Summary: Profile and
 monitor your ML data pipeline end-to-end Home-page: https://docs.whylabs.ai
 License: Apache-2.0 Author: WhyLabs.ai Author-email: support@whylabs.ai
 Requires-Python: >=3.7.1,<4 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Provides-
-Extra: all Provides-Extra: datasets Provides-Extra: docs Provides-Extra:
-embeddings Provides-Extra: fugue Provides-Extra: gcs Provides-Extra: image
-Provides-Extra: mlflow Provides-Extra: s3 Provides-Extra: spark Provides-Extra:
-viz Requires-Dist: Pillow (>=9.2.0,<10.0.0); extra == "viz" or extra == "image"
-or extra == "all" Requires-Dist: boto3 (>=1.22.13,<2.0.0); extra == "s3" or
-extra == "all" Requires-Dist: fugue (>=0.8.1,<0.9.0); extra == "fugue" or extra
-== "all" Requires-Dist: furo (>=2022.3.4,<2023.0.0); extra == "docs" Requires-
-Dist: google-cloud-storage (>=2.5.0,<3.0.0); extra == "gcs" or extra == "all"
-Requires-Dist: importlib-metadata (<4.3); python_version < "3.8" Requires-Dist:
-ipython; extra == "viz" or extra == "all" Requires-Dist: ipython_genutils
-(>=0.2.0,<0.3.0); extra == "docs" Requires-Dist: mlflow-skinny
-(>=1.26.1,<2.0.0); extra == "mlflow" or extra == "all" Requires-Dist: myst-
-parser[sphinx] (>=0.17.2,<0.18.0); extra == "docs" Requires-Dist: nbconvert
-(>=7.0.0,<8.0.0); extra == "docs" Requires-Dist: nbsphinx (>=0.8.9,<0.9.0);
-extra == "docs" Requires-Dist: numpy (>=1.23.2); (python_version >= "3.11") and
-(extra == "viz" or extra == "embeddings" or extra == "all") Requires-Dist:
-numpy; (python_version < "3.11") and (extra == "viz" or extra == "embeddings"
-or extra == "all") Requires-Dist: pandas; extra == "datasets" or extra == "all"
-Requires-Dist: platformdirs (>=3.5.0,<4.0.0) Requires-Dist: protobuf (>=3.19.4)
-Requires-Dist: pyarrow (>=8.0.0,<13); extra == "spark" or extra == "all"
-Requires-Dist: pybars3 (>=0.9,<0.10); extra == "viz" or extra == "all"
-Requires-Dist: pyspark (>=3.0.0,<4.0.0); extra == "spark" or extra == "all"
-Requires-Dist: requests (>=2.27,<3.0) Requires-Dist: scikit-learn
-(>=1.0.2,<2.0.0); (python_version < "3.11") and (extra == "embeddings" or extra
-== "all") Requires-Dist: scikit-learn (>=1.1.2,<2); (python_version >= "3.11")
-and (extra == "embeddings" or extra == "all") Requires-Dist: scipy (>=1.5);
-(python_version < "3.11") and (extra == "viz" or extra == "all") Requires-Dist:
-scipy (>=1.9.2); (python_version >= "3.11") and (extra == "viz" or extra ==
-"all") Requires-Dist: sphinx-autoapi; extra == "docs" Requires-Dist: sphinx-
-autobuild (>=2021.3.14,<2022.0.0); extra == "docs" Requires-Dist: sphinx-
-copybutton (>=0.5.0,<0.6.0); extra == "docs" Requires-Dist: sphinx-inline-tabs;
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Provides-Extra: all Provides-Extra:
+datasets Provides-Extra: docs Provides-Extra: embeddings Provides-Extra: fugue
+Provides-Extra: gcs Provides-Extra: image Provides-Extra: mlflow Provides-
+Extra: s3 Provides-Extra: spark Provides-Extra: viz Requires-Dist: Pillow
+(>=9.2.0,<10.0.0) ; extra == "viz" or extra == "image" or extra == "all"
+Requires-Dist: boto3 (>=1.22.13,<2.0.0) ; extra == "s3" or extra == "all"
+Requires-Dist: fugue (>=0.8.1,<0.9.0) ; extra == "fugue" or extra == "all"
+Requires-Dist: furo (>=2022.3.4,<2023.0.0) ; extra == "docs" Requires-Dist:
+google-cloud-storage (>=2.5.0,<3.0.0) ; extra == "gcs" or extra == "all"
+Requires-Dist: importlib-metadata (<4.3) ; python_version < "3.8" Requires-
+Dist: ipython ; extra == "viz" or extra == "all" Requires-Dist:
+ipython_genutils (>=0.2.0,<0.3.0) ; extra == "docs" Requires-Dist: mlflow-
+skinny (>=1.26.1,<2.0.0) ; extra == "mlflow" or extra == "all" Requires-Dist:
+myst-parser[sphinx] (>=0.17.2,<0.18.0) ; extra == "docs" Requires-Dist:
+nbconvert (>=7.0.0,<8.0.0) ; extra == "docs" Requires-Dist: nbsphinx
+(>=0.8.9,<0.9.0) ; extra == "docs" Requires-Dist: numpy (>=1.23.2) ;
+(python_version >= "3.11") and (extra == "viz" or extra == "embeddings" or
+extra == "all") Requires-Dist: numpy ; (python_version < "3.11") and (extra ==
+"viz" or extra == "embeddings" or extra == "all") Requires-Dist: pandas ; extra
+== "datasets" or extra == "all" Requires-Dist: platformdirs (>=3.5.0,<4.0.0)
+Requires-Dist: protobuf (>=3.19.4) Requires-Dist: pyarrow (>=8.0.0,<13) ; extra
+== "spark" or extra == "all" Requires-Dist: pybars3 (>=0.9,<0.10) ; extra ==
+"viz" or extra == "all" Requires-Dist: pyspark (>=3.0.0,<4.0.0) ; extra ==
+"spark" or extra == "all" Requires-Dist: requests (>=2.27,<3.0) Requires-Dist:
+scikit-learn (>=1.0.2,<2.0.0) ; (python_version < "3.11") and (extra ==
+"embeddings" or extra == "all") Requires-Dist: scikit-learn (>=1.1.2,<2) ;
+(python_version >= "3.11") and (extra == "embeddings" or extra == "all")
+Requires-Dist: scipy (>=1.5) ; (python_version < "3.11") and (extra == "viz" or
+extra == "all") Requires-Dist: scipy (>=1.9.2) ; (python_version >= "3.11") and
+(extra == "viz" or extra == "all") Requires-Dist: sphinx ; extra == "docs"
+Requires-Dist: sphinx-autoapi ; extra == "docs" Requires-Dist: sphinx-autobuild
+(>=2021.3.14,<2022.0.0) ; extra == "docs" Requires-Dist: sphinx-copybutton
+(>=0.5.0,<0.6.0) ; extra == "docs" Requires-Dist: sphinx-inline-tabs ;
 (python_version >= "3.8" and python_version < "4") and (extra == "docs")
-Requires-Dist: sphinx; extra == "docs" Requires-Dist: sphinxext-opengraph
-(>=0.6.3,<0.7.0); extra == "docs" Requires-Dist: types-requests
-(>=2.30.0.0,<3.0.0.0) Requires-Dist: typing-extensions (>=3.10); python_version
-< "4" Requires-Dist: whylabs-client (>=0.5.1,<1) Requires-Dist: whylogs-
-sketching (>=3.4.1.dev3) Description-Content-Type: text/markdown [https://
-static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82]
+Requires-Dist: sphinxext-opengraph (>=0.6.3,<0.7.0) ; extra == "docs" Requires-
+Dist: types-requests (>=2.30.0.0,<3.0.0.0) Requires-Dist: typing-extensions
+(>=3.10) ; python_version < "4" Requires-Dist: whylabs-client (>=0.5.1,<1)
+Requires-Dist: whylogs-sketching (>=3.4.1.dev3) Description-Content-Type: text/
+markdown [https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-
+f711c4d35b82]
                       [https://i.imgur.com/nv33goV.png]
                ****** The open standard for data logging ******
  **** Documentation • Slack_Community • Python_Quickstart • WhyLabs_Quickstart
                                      ****
       [License] [PyPi_Version] [Code_style:_black] [PyPi_Downloads] [CI]
                                [Maintainability]
 ## What is whylogs whylogs is an open source library for logging any kind of
```

