# Comparing `tmp/getdaft-0.1.8.tar.gz` & `tmp/getdaft-0.1.9.tar.gz`

## Comparing `getdaft-0.1.8.tar` & `getdaft-0.1.9.tar`

### file list

```diff
@@ -1,499 +1,525 @@
--rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 getdaft-0.1.8/local_dependencies/daft-table/Cargo.toml
--rw-r--r--   0      501       20     2853 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/ffi.rs
--rw-r--r--   0      501       20    20730 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/lib.rs
--rw-r--r--   0      501       20     2168 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/ops/agg.rs
--rw-r--r--   0      501       20     3748 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/ops/explode.rs
--rw-r--r--   0      501       20     4415 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/ops/groups.rs
--rw-r--r--   0      501       20     2898 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/ops/hash.rs
--rw-r--r--   0      501       20     2499 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/ops/joins/hash_join.rs
--rw-r--r--   0      501       20     3727 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/ops/joins/mod.rs
--rw-r--r--   0      501       20       99 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/ops/mod.rs
--rw-r--r--   0      501       20     3478 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/ops/partition.rs
--rw-r--r--   0      501       20     1808 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/ops/search_sorted.rs
--rw-r--r--   0      501       20      998 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/ops/sort.rs
--rw-r--r--   0      501       20    11179 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-table/src/python.rs
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 getdaft-0.1.8/local_dependencies/common-error/Cargo.toml
--rw-r--r--   0      501       20     2849 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/common-error/src/error.rs
--rw-r--r--   0      501       20       64 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/common-error/src/lib.rs
--rw-r--r--   0        0        0     1165 1970-01-01 00:00:00.000000 getdaft-0.1.8/local_dependencies/daft-io/Cargo.toml
--rw-r--r--   0      501       20     1087 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-io/src/config.rs
--rw-r--r--   0      501       20     4730 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-io/src/http.rs
--rw-r--r--   0      501       20     8332 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-io/src/lib.rs
--rw-r--r--   0      501       20     6205 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-io/src/local.rs
--rw-r--r--   0      501       20     1652 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-io/src/object_io.rs
--rw-r--r--   0      501       20     1966 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-io/src/python.rs
--rw-r--r--   0      501       20    13490 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-io/src/s3_like.rs
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 getdaft-0.1.8/local_dependencies/daft-dsl/Cargo.toml
--rw-r--r--   0      501       20      273 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/README.md
--rw-r--r--   0      501       20     1454 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/arithmetic.rs
--rw-r--r--   0      501       20    19598 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/expr.rs
--rw-r--r--   0      501       20     1456 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/float/is_nan.rs
--rw-r--r--   0      501       20      582 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/float/mod.rs
--rw-r--r--   0      501       20     1353 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/image/decode.rs
--rw-r--r--   0      501       20     1790 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/image/encode.rs
--rw-r--r--   0      501       20     1292 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/image/mod.rs
--rw-r--r--   0      501       20     2524 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/image/resize.rs
--rw-r--r--   0      501       20     1130 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/list/explode.rs
--rw-r--r--   0      501       20     2329 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/list/join.rs
--rw-r--r--   0      501       20      873 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/list/mod.rs
--rw-r--r--   0      501       20     2085 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/mod.rs
--rw-r--r--   0      501       20     1197 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/numeric/abs.rs
--rw-r--r--   0      501       20      575 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/numeric/mod.rs
--rw-r--r--   0      501       20      684 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/python/mod.rs
--rw-r--r--   0      501       20     2050 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/python/partial_udf.rs
--rw-r--r--   0      501       20     2793 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/python/udf.rs
--rw-r--r--   0      501       20     1344 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/temporal/day.rs
--rw-r--r--   0      501       20     1373 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/temporal/day_of_week.rs
--rw-r--r--   0      501       20     1415 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/temporal/mod.rs
--rw-r--r--   0      501       20     1355 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/temporal/month.rs
--rw-r--r--   0      501       20     1349 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/temporal/year.rs
--rw-r--r--   0      501       20     2295 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/uri/download.rs
--rw-r--r--   0      501       20     1073 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/uri/mod.rs
--rw-r--r--   0      501       20     1652 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/utf8/contains.rs
--rw-r--r--   0      501       20     1651 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/utf8/endswith.rs
--rw-r--r--   0      501       20     1370 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/utf8/length.rs
--rw-r--r--   0      501       20     1519 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/utf8/mod.rs
--rw-r--r--   0      501       20     1661 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/utf8/startswith.rs
--rw-r--r--   0      501       20      707 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/lib.rs
--rw-r--r--   0      501       20     4967 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/lit.rs
--rw-r--r--   0      501       20     5298 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/optimization.rs
--rw-r--r--   0      501       20     1982 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/pyobject.rs
--rw-r--r--   0      501       20    11937 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-dsl/src/python.rs
--rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 getdaft-0.1.8/local_dependencies/daft-core/Cargo.toml
--rw-r--r--   0      501       20     5844 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/from.rs
--rw-r--r--   0      501       20      734 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/iterator.rs
--rw-r--r--   0      501       20     3012 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/mod.rs
--rw-r--r--   0      501       20      269 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/abs.rs
--rw-r--r--   0      501       20      738 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/apply.rs
--rw-r--r--   0      501       20      849 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arange.rs
--rw-r--r--   0      501       20     6972 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arithmetic.rs
--rw-r--r--   0      501       20     3055 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arrow2/comparison.rs
--rw-r--r--   0      501       20       34 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arrow2/mod.rs
--rw-r--r--   0      501       20       19 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arrow2/sort/mod.rs
--rw-r--r--   0      501       20     3482 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/common.rs
--rw-r--r--   0      501       20      723 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/indices.rs
--rw-r--r--   0      501       20       47 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/mod.rs
--rw-r--r--   0      501       20     8075 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/sort.rs
--rw-r--r--   0      501       20     2409 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/as_arrow.rs
--rw-r--r--   0      501       20    11395 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/broadcast.rs
--rw-r--r--   0      501       20    40353 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/cast.rs
--rw-r--r--   0      501       20    11029 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/compare_agg.rs
--rw-r--r--   0      501       20    47241 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/comparison.rs
--rw-r--r--   0      501       20     1630 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/concat.rs
--rw-r--r--   0      501       20     5991 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/concat_agg.rs
--rw-r--r--   0      501       20     1444 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/count.rs
--rw-r--r--   0      501       20     1548 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/date.rs
--rw-r--r--   0      501       20     2430 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/filter.rs
--rw-r--r--   0      501       20     1271 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/float.rs
--rw-r--r--   0      501       20     1936 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/full.rs
--rw-r--r--   0      501       20     4823 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/get.rs
--rw-r--r--   0      501       20     4119 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/groups.rs
--rw-r--r--   0      501       20     1523 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/hash.rs
--rw-r--r--   0      501       20    12222 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/if_else.rs
--rw-r--r--   0      501       20    29241 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/image.rs
--rw-r--r--   0      501       20     1069 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/len.rs
--rw-r--r--   0      501       20     6625 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/list.rs
--rw-r--r--   0      501       20     3367 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/list_agg.rs
--rw-r--r--   0      501       20     1634 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/mean.rs
--rw-r--r--   0      501       20     2629 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/mod.rs
--rw-r--r--   0      501       20     1325 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/null.rs
--rw-r--r--   0      501       20     3826 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/pairwise.rs
--rw-r--r--   0      501       20     9877 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/repr.rs
--rw-r--r--   0      501       20      491 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/search_sorted.rs
--rw-r--r--   0      501       20    19867 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/sort.rs
--rw-r--r--   0      501       20     2396 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/sum.rs
--rw-r--r--   0      501       20     4604 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/take.rs
--rw-r--r--   0      501       20     5279 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/utf8.rs
--rw-r--r--   0      501       20      995 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/pseudo_arrow/compute.rs
--rw-r--r--   0      501       20    13611 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/pseudo_arrow/mod.rs
--rw-r--r--   0      501       20     2502 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/array/pseudo_arrow/python.rs
--rw-r--r--   0      501       20     8228 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/binary_ops.rs
--rw-r--r--   0      501       20    15026 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/dtype.rs
--rw-r--r--   0      501       20     2021 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/field.rs
--rw-r--r--   0      501       20     3187 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/image_format.rs
--rw-r--r--   0      501       20     6382 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/image_mode.rs
--rw-r--r--   0      501       20     3589 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/logical.rs
--rw-r--r--   0      501       20     9200 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/matching.rs
--rw-r--r--   0      501       20     6905 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/mod.rs
--rw-r--r--   0      501       20     1100 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/time_unit.rs
--rw-r--r--   0      501       20     5128 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/ffi.rs
--rw-r--r--   0      501       20     6022 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/kernels/hashing.rs
--rw-r--r--   0      501       20       54 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/kernels/mod.rs
--rw-r--r--   0      501       20    12159 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/kernels/search_sorted.rs
--rw-r--r--   0      501       20     3917 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/kernels/utf8.rs
--rw-r--r--   0      501       20      553 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/lib.rs
--rw-r--r--   0      501       20     8528 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/python/datatype.rs
--rw-r--r--   0      501       20     1661 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/python/field.rs
--rw-r--r--   0      501       20      610 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/python/mod.rs
--rw-r--r--   0      501       20     2843 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/python/schema.rs
--rw-r--r--   0      501       20    12308 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/python/series.rs
--rw-r--r--   0      501       20     3729 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/schema.rs
--rw-r--r--   0      501       20     7500 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/array_impl/binary_ops.rs
--rw-r--r--   0      501       20    11522 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/array_impl/data_array.rs
--rw-r--r--   0      501       20     6504 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/array_impl/logical_array.rs
--rw-r--r--   0      501       20      181 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/array_impl/mod.rs
--rw-r--r--   0      501       20     2106 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/from.rs
--rw-r--r--   0      501       20     2309 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/mod.rs
--rw-r--r--   0      501       20      910 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/abs.rs
--rw-r--r--   0      501       20     5199 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/agg.rs
--rw-r--r--   0      501       20     3419 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/arithmetic.rs
--rw-r--r--   0      501       20     1924 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/broadcast.rs
--rw-r--r--   0      501       20      205 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/cast.rs
--rw-r--r--   0      501       20     2616 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/comparison.rs
--rw-r--r--   0      501       20     1565 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/concat.rs
--rw-r--r--   0      501       20     1820 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/date.rs
--rw-r--r--   0      501       20     3621 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/downcast.rs
--rw-r--r--   0      501       20      693 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/filter.rs
--rw-r--r--   0      501       20      411 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/float.rs
--rw-r--r--   0      501       20      439 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/groups.rs
--rw-r--r--   0      501       20      416 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/hash.rs
--rw-r--r--   0      501       20      324 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/if_else.rs
--rw-r--r--   0      501       20     2468 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/image.rs
--rw-r--r--   0      501       20      297 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/len.rs
--rw-r--r--   0      501       20     2351 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/list.rs
--rw-r--r--   0      501       20     2541 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/mod.rs
--rw-r--r--   0      501       20      475 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/not.rs
--rw-r--r--   0      501       20      160 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/null.rs
--rw-r--r--   0      501       20      645 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/search_sorted.rs
--rw-r--r--   0      501       20     1504 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/sort.rs
--rw-r--r--   0      501       20      662 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/take.rs
--rw-r--r--   0      501       20     1526 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/utf8.rs
--rw-r--r--   0      501       20     1718 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/series/series_like.rs
--rw-r--r--   0      501       20     5401 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/utils/arrow.rs
--rw-r--r--   0      501       20      347 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/utils/mod.rs
--rw-r--r--   0      501       20    10066 2023-07-05 18:53:54.000000 getdaft-0.1.8/local_dependencies/daft-core/src/utils/supertype.rs
--rw-r--r--   0        0        0     2202 1970-01-01 00:00:00.000000 getdaft-0.1.8/Cargo.toml
--rw-r--r--   0      501       20      834 2023-07-05 18:53:54.000000 getdaft-0.1.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0      501       20      595 2023-07-05 18:53:54.000000 getdaft-0.1.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0      501       20      431 2023-07-05 18:53:54.000000 getdaft-0.1.8/.github/dependabot.yml
--rw-r--r--   0      501       20     1063 2023-07-05 18:53:54.000000 getdaft-0.1.8/.github/release-drafter.yml
--rw-r--r--   0      501       20     1333 2023-07-05 18:53:54.000000 getdaft-0.1.8/.github/workflows/broken-link-checker.yml
--rw-r--r--   0      501       20     3395 2023-07-05 18:53:54.000000 getdaft-0.1.8/.github/workflows/daft-profiling.yml
--rw-r--r--   0      501       20     1627 2023-07-05 18:53:54.000000 getdaft-0.1.8/.github/workflows/notebook-checker.yml
--rw-r--r--   0      501       20     2211 2023-07-05 18:53:54.000000 getdaft-0.1.8/.github/workflows/property-based-tests.yml
--rw-r--r--   0      501       20    16055 2023-07-05 18:53:54.000000 getdaft-0.1.8/.github/workflows/python-package.yml
--rw-r--r--   0      501       20     6165 2023-07-05 18:53:54.000000 getdaft-0.1.8/.github/workflows/python-publish.yml
--rw-r--r--   0      501       20     2655 2023-07-05 18:53:54.000000 getdaft-0.1.8/.github/workflows/ray-compatibility.yml
--rw-r--r--   0      501       20     2696 2023-07-05 18:53:54.000000 getdaft-0.1.8/.github/workflows/release-drafter.yml
--rw-r--r--   0      501       20      306 2023-07-05 18:53:54.000000 getdaft-0.1.8/.gitignore
--rw-r--r--   0      501       20     2226 2023-07-05 18:53:54.000000 getdaft-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0      501       20      205 2023-07-05 18:53:54.000000 getdaft-0.1.8/.readthedocs.yaml
--rw-r--r--   0      501       20     1550 2023-07-05 18:53:54.000000 getdaft-0.1.8/CONTRIBUTING.md
--rw-r--r--   0      501       20    11357 2023-07-05 18:53:54.000000 getdaft-0.1.8/LICENSE
--rw-r--r--   0      501       20     1295 2023-07-05 18:53:54.000000 getdaft-0.1.8/Makefile
--rw-r--r--   0      501       20     8834 2023-07-05 18:53:54.000000 getdaft-0.1.8/README.rst
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/benchmarking/__init__.py
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/benchmarking/tpch/__init__.py
--rw-r--r--   0      501       20     9495 2023-07-05 18:53:54.000000 getdaft-0.1.8/benchmarking/tpch/__main__.py
--rw-r--r--   0      501       20    12428 2023-07-05 18:53:54.000000 getdaft-0.1.8/benchmarking/tpch/answers.py
--rw-r--r--   0      501       20    12336 2023-07-05 18:53:54.000000 getdaft-0.1.8/benchmarking/tpch/data_generation.py
--rw-r--r--   0      501       20     4573 2023-07-05 18:53:54.000000 getdaft-0.1.8/benchmarking/tpch/pipelined_data_generation.py
--rw-r--r--   0      501       20     2654 2023-07-05 18:53:54.000000 getdaft-0.1.8/benchmarking/tpch/subprefix_s3_files.py
--rw-r--r--   0      501       20     1436 2023-07-05 18:53:54.000000 getdaft-0.1.8/ci/upload_wheels.sh
--rw-r--r--   0      501       20      446 2023-07-05 18:53:54.000000 getdaft-0.1.8/codecov.yml
--rw-r--r--   0      501       20     2199 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/__init__.py
--rw-r--r--   0      501       20     6724 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/analytics.py
--rw-r--r--   0      501       20     3935 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/api_annotations.py
--rw-r--r--   0      501       20    10591 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/arrow_utils.py
--rw-r--r--   0      501       20     5511 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/context.py
--rw-r--r--   0      501       20     3412 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/convert.py
--rw-r--r--   0      501       20     1298 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/daft.pyi
--rw-r--r--   0      501       20       94 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/dataframe/__init__.py
--rw-r--r--   0      501       20    54827 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/dataframe/dataframe.py
--rw-r--r--   0      501       20      306 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/dataframe/preview.py
--rw-r--r--   0      501       20     1404 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/dataframe/to_torch.py
--rw-r--r--   0      501       20      850 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/datasources.py
--rw-r--r--   0      501       20    17515 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/datatype.py
--rw-r--r--   0      501       20       84 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/errors.py
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/execution/__init__.py
--rw-r--r--   0      501       20    28993 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/execution/execution_step.py
--rw-r--r--   0      501       20    28946 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/execution/physical_plan.py
--rw-r--r--   0      501       20     6350 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/execution/physical_plan_factory.py
--rw-r--r--   0      501       20      170 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/expressions/__init__.py
--rw-r--r--   0      501       20    28908 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/expressions/expressions.py
--rw-r--r--   0      501       20      572 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/expressions/testing.py
--rw-r--r--   0      501       20    12728 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/filesystem.py
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/internal/__init__.py
--rw-r--r--   0      501       20      509 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/internal/gpu.py
--rw-r--r--   0      501       20     1804 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/internal/rule.py
--rw-r--r--   0      501       20     2030 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/internal/rule_runner.py
--rw-r--r--   0      501       20     3490 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/internal/treenode.py
--rw-r--r--   0      501       20      377 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/io/__init__.py
--rw-r--r--   0      501       20     2456 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/io/_csv.py
--rw-r--r--   0      501       20     1642 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/io/_json.py
--rw-r--r--   0      501       20     2317 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/io/common.py
--rw-r--r--   0      501       20     2036 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/io/file_path.py
--rw-r--r--   0      501       20     1665 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/io/parquet.py
--rw-r--r--   0      501       20      264 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/logging.py
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/logical/__init__.py
--rw-r--r--   0      501       20     8601 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/logical/aggregation_plan_builder.py
--rw-r--r--   0      501       20    38976 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/logical/logical_plan.py
--rw-r--r--   0      501       20     1492 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/logical/map_partition_ops.py
--rw-r--r--   0      501       20    19757 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/logical/optimizer.py
--rw-r--r--   0      501       20     3868 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/logical/schema.py
--rw-r--r--   0      501       20       99 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/pickle/__init__.py
--rw-r--r--   0      501       20    34760 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/pickle/cloudpickle.py
--rw-r--r--   0      501       20    34262 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/pickle/cloudpickle_fast.py
--rw-r--r--   0      501       20      639 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/pickle/compat.py
--rw-r--r--   0      501       20      312 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/pickle/pickle.py
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/py.typed
--rw-r--r--   0      501       20     2036 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/resource_request.py
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/runners/__init__.py
--rw-r--r--   0      501       20     4676 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/runners/partitioning.py
--rw-r--r--   0      501       20     1488 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/runners/profiler.py
--rw-r--r--   0      501       20    13802 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/runners/pyrunner.py
--rw-r--r--   0      501       20    28094 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/runners/ray_runner.py
--rw-r--r--   0      501       20     1428 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/runners/runner.py
--rw-r--r--   0      501       20     3344 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/runners/runner_io.py
--rw-r--r--   0      501       20    22246 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/series.py
--rw-r--r--   0      501       20       82 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/table/__init__.py
--rw-r--r--   0      501       20     2960 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/table/schema_inference.py
--rw-r--r--   0      501       20    14029 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/table/table.py
--rw-r--r--   0      501       20     9916 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/table/table_io.py
--rw-r--r--   0      501       20     7370 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/udf.py
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/udf_library/__init__.py
--rw-r--r--   0      501       20     3486 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/udf_library/url_udfs.py
--rw-r--r--   0      501       20     2796 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/utils.py
--rw-r--r--   0      501       20      183 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/viz/__init__.py
--rw-r--r--   0      501       20     1929 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/viz/dataframe_display.py
--rw-r--r--   0      501       20     1522 2023-07-05 18:53:54.000000 getdaft-0.1.8/daft/viz/html_viz_hooks.py
--rw-r--r--   0      501       20      148 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/CONTRIBUTING.md
--rw-r--r--   0      501       20      638 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/Makefile
--rw-r--r--   0      501       20    73229 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/10-min.ipynb
--rw-r--r--   0      501       20      389 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/custom-function-signatures.css
--rw-r--r--   0      501       20      565 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/daft-favicon.png
--rw-r--r--   0      501       20     7804 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/daft-logo.png
--rw-r--r--   0      501       20    42148 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/daft_illustration.png
--rw-r--r--   0      501       20      583 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/dataframe-comp-table.csv
--rw-r--r--   0      501       20    25200 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/execution_model.png
--rw-r--r--   0      501       20     1901 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/header.css
--rw-r--r--   0      501       20    32864 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/high_level_architecture.png
--rw-r--r--   0      501       20      343 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/icon-menu-close.svg
--rw-r--r--   0      501       20      333 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/icon-menu-dots.svg
--rw-r--r--   0      501       20    18177 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/in_memory_data_representation.png
--rw-r--r--   0      501       20      786 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/mobile-menu.js
--rw-r--r--   0      501       20     9142 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/tpch-1000sf.html
--rw-r--r--   0      501       20     9647 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/tpch-100sf.html
--rw-r--r--   0      501       20     8757 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_static/tpch-nodes-count-daft-1000-sf.html
--rw-r--r--   0      501       20      856 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_templates/layout.html
--rw-r--r--   0      501       20     1179 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_templates/sections/header.html
--rw-r--r--   0      501       20     1129 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/_templates/sections/mobile-menu.html
--rw-r--r--   0      501       20      333 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/context.rst
--rw-r--r--   0      501       20     2759 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/dataframe.rst
--rw-r--r--   0      501       20     2293 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/datatype.rst
--rw-r--r--   0      501       20      139 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/datatype_image_mode/daft.ImageMode.from_mode_string.rst
--rw-r--r--   0      501       20      430 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/datatype_image_mode/daft.ImageMode.rst
--rw-r--r--   0      501       20      151 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/datetype_image_format/daft.ImageFormat.from_format_string.rst
--rw-r--r--   0      501       20      333 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/datetype_image_format/daft.ImageFormat.rst
--rw-r--r--   0      501       20     4727 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/expressions.rst
--rw-r--r--   0      501       20      816 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/groupby.rst
--rw-r--r--   0      501       20      146 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/index.rst
--rw-r--r--   0      501       20     1537 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/input_output.rst
--rw-r--r--   0      501       20      273 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/series/daft.Series.rst
--rw-r--r--   0      501       20      492 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/series.rst
--rw-r--r--   0      501       20       88 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/api_docs/udf.rst
--rw-r--r--   0      501       20    14528 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/benchmarks/index.rst
--rw-r--r--   0      501       20     4200 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/conf.py
--rw-r--r--   0      501       20     5114 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/dataframe_comparison.rst
--rw-r--r--   0      501       20     1723 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/index.rst
--rw-r--r--   0      501       20     1356 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/install.rst
--rw-r--r--   0      501       20      896 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/index.rst
--rw-r--r--   0      501       20     7830 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/key_concepts.rst
--rw-r--r--   0      501       20     1783 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/tutorials.rst
--rw-r--r--   0      501       20     1388 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/user_guides/aggregations.rst
--rw-r--r--   0      501       20     7009 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/user_guides/dataframe-operations.rst
--rw-r--r--   0      501       20     5166 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/user_guides/datatypes.rst
--rw-r--r--   0      501       20     9481 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/user_guides/expressions.rst
--rw-r--r--   0      501       20     8241 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/user_guides/intro-dataframes.rst
--rw-r--r--   0      501       20      206 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/user_guides/partitioning.rst
--rw-r--r--   0      501       20     3251 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/user_guides/read-write.rst
--rw-r--r--   0      501       20     1257 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/user_guides/scaling-up.rst
--rw-r--r--   0      501       20     8853 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/user_guides/udf.rst
--rw-r--r--   0      501       20     1577 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/learn/user_guides.rst
--rw-r--r--   0      501       20     6628 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/technical_architecture.rst
--rw-r--r--   0      501       20     1316 2023-07-05 18:53:54.000000 getdaft-0.1.8/docs/source/telemetry.rst
--rw-r--r--   0      501       20     1871 2023-07-05 18:53:54.000000 getdaft-0.1.8/pyproject.toml
--rw-r--r--   0      501       20     1137 2023-07-05 18:53:54.000000 getdaft-0.1.8/requirements-dev.txt
--rw-r--r--   0      501       20       98 2023-07-05 18:53:54.000000 getdaft-0.1.8/rust-toolchain.toml
--rw-r--r--   0      501       20      687 2023-07-05 18:53:54.000000 getdaft-0.1.8/src/lib.rs
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/__init__.py
--rw-r--r--   0      501       20      299 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/assets/__init__.py
--rw-r--r--   0      501       20      544 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/assets/tpch-sqlite-queries/1.sql
--rw-r--r--   0      501       20      542 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/assets/tpch-sqlite-queries/10.sql
--rw-r--r--   0      501       20      703 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/assets/tpch-sqlite-queries/2.sql
--rw-r--r--   0      501       20      444 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/assets/tpch-sqlite-queries/3.sql
--rw-r--r--   0      501       20      371 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/assets/tpch-sqlite-queries/4.sql
--rw-r--r--   0      501       20      504 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/assets/tpch-sqlite-queries/5.sql
--rw-r--r--   0      501       20      259 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/assets/tpch-sqlite-queries/6.sql
--rw-r--r--   0      501       20      834 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/assets/tpch-sqlite-queries/7.sql
--rw-r--r--   0      501       20      815 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/assets/tpch-sqlite-queries/8.sql
--rw-r--r--   0      501       20      627 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/assets/tpch-sqlite-queries/9.sql
--rw-r--r--   0      501       20       48 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/assets/tpch-sqlite-queries/README.md
--rw-r--r--   0      501       20      604 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/benchmarks/conftest.py
--rw-r--r--   0      501       20     1227 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/benchmarks/test_df_arithmetic.py
--rw-r--r--   0      501       20     2706 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/benchmarks/test_file_read.py
--rw-r--r--   0      501       20     5604 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/benchmarks/test_groups_and_aggs.py
--rw-r--r--   0      501       20     7292 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/benchmarks/test_join.py
--rw-r--r--   0      501       20     2603 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/benchmarks/test_repartition.py
--rw-r--r--   0      501       20     4005 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/benchmarks/test_sort.py
--rw-r--r--   0      501       20     2911 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/conftest.py
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/__init__.py
--rw-r--r--   0      501       20    13229 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/assets/311-service-requests.24.csv
--rw-r--r--   0      501       20      255 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/assets/__init__.py
--rw-r--r--   0      501       20      924 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/assets/images/0000.jpg
--rw-r--r--   0      501       20      941 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/assets/images/0007.jpg
--rw-r--r--   0      501       20     2740 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/assets/images/0018.png
--rw-r--r--   0      501       20     7462 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/assets/images/0025.tiff
--rw-r--r--   0      501       20      882 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/conftest.py
--rw-r--r--   0      501       20     9268 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/test_aggregations.py
--rw-r--r--   0      501       20     2979 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/test_computations.py
--rw-r--r--   0      501       20     1798 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/test_count_rows.py
--rw-r--r--   0      501       20     7099 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/test_dataloading.py
--rw-r--r--   0      501       20      800 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/test_distinct.py
--rw-r--r--   0      501       20     6049 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/test_filter.py
--rw-r--r--   0      501       20     2930 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/test_image.py
--rw-r--r--   0      501       20     3810 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/test_joins.py
--rw-r--r--   0      501       20     2878 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/test_literals.py
--rw-r--r--   0      501       20    10311 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/test_pandas_cookbook.py
--rw-r--r--   0      501       20     4148 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/test_sorting.py
--rw-r--r--   0      501       20     1497 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/cookbook/test_write.py
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/__init__.py
--rw-r--r--   0      501       20      751 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/conftest.py
--rw-r--r--   0      501       20      805 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_accessors.py
--rw-r--r--   0      501       20    10308 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_aggregations.py
--rw-r--r--   0      501       20      472 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_concat.py
--rw-r--r--   0      501       20    26635 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_creation.py
--rw-r--r--   0      501       20     1824 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_distinct.py
--rw-r--r--   0      501       20     1428 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_explode.py
--rw-r--r--   0      501       20     1097 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_filter.py
--rw-r--r--   0      501       20     2435 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_getitem.py
--rw-r--r--   0      501       20     3205 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_iter.py
--rw-r--r--   0      501       20     4091 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_joins.py
--rw-r--r--   0      501       20     2253 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_logical_type.py
--rw-r--r--   0      501       20      223 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_repartition.py
--rw-r--r--   0      501       20     8608 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_repr.py
--rw-r--r--   0      501       20      815 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_select.py
--rw-r--r--   0      501       20      656 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_show.py
--rw-r--r--   0      501       20     6364 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_sort.py
--rw-r--r--   0      501       20     7542 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_temporals.py
--rw-r--r--   0      501       20     2385 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_to_integrations.py
--rw-r--r--   0      501       20      850 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/dataframe/test_with_column.py
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/__init__.py
--rw-r--r--   0      501       20     1417 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/test_apply.py
--rw-r--r--   0      501       20     3533 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/test_expressions.py
--rw-r--r--   0      501       20     4259 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/test_expressions_projection.py
--rw-r--r--   0      501       20     5019 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/test_udf.py
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/typing/__init__.py
--rw-r--r--   0      501       20     6290 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/typing/conftest.py
--rw-r--r--   0      501       20     1363 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/typing/test_aggs.py
--rw-r--r--   0      501       20     2335 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/typing/test_arithmetic.py
--rw-r--r--   0      501       20      853 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/typing/test_compare.py
--rw-r--r--   0      501       20      792 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/typing/test_dt.py
--rw-r--r--   0      501       20      531 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/typing/test_float.py
--rw-r--r--   0      501       20      684 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/typing/test_if_else.py
--rw-r--r--   0      501       20      422 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/typing/test_is_null.py
--rw-r--r--   0      501       20     1176 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/typing/test_logical.py
--rw-r--r--   0      501       20     1544 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/expressions/typing/test_str.py
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/integration/__init__.py
--rw-r--r--   0      501       20       91 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/integration/docker-compose/Dockerfile.nginx
--rw-r--r--   0      501       20      699 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/integration/docker-compose/docker-compose.yml
--rw-r--r--   0      501       20     1007 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/integration/docker-compose/nginx-serve-static-files.conf
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/integration/io/__init__.py
--rw-r--r--   0      501       20     2902 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/integration/io/conftest.py
--rw-r--r--   0      501       20     2242 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/integration/io/test_url_download_http.py
--rw-r--r--   0      501       20     1829 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/integration/io/test_url_download_local.py
--rw-r--r--   0      501       20     1780 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/integration/io/test_url_download_public_aws_s3.py
--rw-r--r--   0      501       20     1062 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/integration/io/test_url_download_s3_minio.py
--rw-r--r--   0      501       20     4343 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/integration/test_tpch.py
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/optimizer/__init__.py
--rw-r--r--   0      501       20     1116 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/optimizer/conftest.py
--rw-r--r--   0      501       20     1666 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/optimizer/test_drop_projections.py
--rw-r--r--   0      501       20     1847 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/optimizer/test_drop_repartition.py
--rw-r--r--   0      501       20     2463 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/optimizer/test_fold_projections.py
--rw-r--r--   0      501       20     8050 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/optimizer/test_prune_columns.py
--rw-r--r--   0      501       20     3597 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/optimizer/test_pushdown_clauses_into_scan.py
--rw-r--r--   0      501       20     1170 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/optimizer/test_pushdown_limit.py
--rw-r--r--   0      501       20     8981 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/optimizer/test_pushdown_predicates.py
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/property_based_testing/__init__.py
--rw-r--r--   0      501       20     4575 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/property_based_testing/strategies.py
--rw-r--r--   0      501       20     8895 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/property_based_testing/test_sort.py
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/ray/__init__.py
--rw-r--r--   0      501       20     5375 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/ray/test_dask.py
--rw-r--r--   0      501       20     8864 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/ray/test_datasets.py
--rw-r--r--   0      501       20      278 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/__init__.py
--rw-r--r--   0      501       20     9299 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_arithmetic.py
--rw-r--r--   0      501       20    15034 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_cast.py
--rw-r--r--   0      501       20    17207 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_comparisons.py
--rw-r--r--   0      501       20     7188 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_concat.py
--rw-r--r--   0      501       20      896 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_embedding.py
--rw-r--r--   0      501       20     6151 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_filter.py
--rw-r--r--   0      501       20      874 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_float.py
--rw-r--r--   0      501       20     3344 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_hash.py
--rw-r--r--   0      501       20    21522 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_if_else.py
--rw-r--r--   0      501       20    22626 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_image.py
--rw-r--r--   0      501       20      889 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_numeric_ops.py
--rw-r--r--   0      501       20     3418 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_series.py
--rw-r--r--   0      501       20     9173 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_size_bytes.py
--rw-r--r--   0      501       20     2188 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_slice.py
--rw-r--r--   0      501       20     5495 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_sort.py
--rw-r--r--   0      501       20     6111 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_take.py
--rw-r--r--   0      501       20     1934 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_temporal_ops.py
--rw-r--r--   0      501       20     4413 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/series/test_utf8_ops.py
--rw-r--r--   0      501       20      694 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/__init__.py
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/list/__init__.py
--rw-r--r--   0      501       20     1156 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/list/test_list_join.py
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/table_io/__init__.py
--rw-r--r--   0      501       20     6289 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/table_io/test_csv.py
--rw-r--r--   0      501       20     4355 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/table_io/test_json.py
--rw-r--r--   0      501       20     4778 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/table_io/test_parquet.py
--rw-r--r--   0      501       20     2100 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/table_io/test_read_time_cast.py
--rw-r--r--   0      501       20     1070 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_blackbox_kernels.py
--rw-r--r--   0      501       20      426 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_broadcasts.py
--rw-r--r--   0      501       20     2123 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_concat.py
--rw-r--r--   0      501       20     4900 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_eval.py
--rw-r--r--   0      501       20     3930 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_explodes.py
--rw-r--r--   0      501       20     7413 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_filter.py
--rw-r--r--   0      501       20    23530 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_from_py.py
--rw-r--r--   0      501       20      842 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_head.py
--rw-r--r--   0      501       20    10974 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_joins.py
--rw-r--r--   0      501       20     7811 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_partitioning.py
--rw-r--r--   0      501       20      654 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_size_bytes.py
--rw-r--r--   0      501       20    10955 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_sorting.py
--rw-r--r--   0      501       20    20923 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_table_aggs.py
--rw-r--r--   0      501       20     5061 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/test_take.py
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/utf8/__init__.py
--rw-r--r--   0      501       20     1165 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/utf8/test_compares.py
--rw-r--r--   0      501       20      321 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/table/utf8/test_length.py
--rw-r--r--   0      501       20     3533 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/test_analytics.py
--rw-r--r--   0      501       20      703 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/test_datatypes.py
--rw-r--r--   0      501       20     3653 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/test_schema.py
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/udf_library/__init__.py
--rw-r--r--   0      501       20     4508 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/udf_library/test_url_udfs.py
--rw-r--r--   0      501       20      338 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests/utils.py
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests_legacy/__init__.py
--rw-r--r--   0      501       20     6988 2023-07-05 18:53:54.000000 getdaft-0.1.8/tests_legacy/test_resource_requests.py
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/__init__.py
--rw-r--r--   0      501       20     1633 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/patch_package_version.py
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/__init__.py
--rw-r--r--   0      501       20        0 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/_vendor/__init__.py
--rw-r--r--   0      501       20     1125 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/_vendor/wheel/LICENSE.txt
--rw-r--r--   0      501       20       59 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/_vendor/wheel/__init__.py
--rw-r--r--   0      501       20     2499 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/_vendor/wheel/cli/__init__.py
--rw-r--r--   0      501       20     9514 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/_vendor/wheel/cli/convert.py
--rw-r--r--   0      501       20     3113 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/_vendor/wheel/cli/pack.py
--rw-r--r--   0      501       20      662 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/_vendor/wheel/cli/unpack.py
--rw-r--r--   0      501       20     1246 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/_vendor/wheel/pkginfo.py
--rw-r--r--   0      501       20      974 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/_vendor/wheel/util.py
--rw-r--r--   0      501       20     7125 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/_vendor/wheel/wheelfile.py
--rw-r--r--   0      501       20      878 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/fix-and-copy-wheel.py
--rw-r--r--   0      501       20     2981 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/tmpdirs.py
--rw-r--r--   0      501       20     4469 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/tools.py
--rw-r--r--   0      501       20     9484 2023-07-05 18:53:54.000000 getdaft-0.1.8/tools/wheels/wheeltools.py
--rw-r--r--   0      501       20       19 2023-07-05 18:53:54.000000 getdaft-0.1.8/tutorials/.gitignore
--rw-r--r--   0      501       20    19755 2023-07-05 18:53:54.000000 getdaft-0.1.8/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb
--rw-r--r--   0      501       20    12692 2023-07-05 18:53:54.000000 getdaft-0.1.8/tutorials/image_querying/top_n_red_color.ipynb
--rw-r--r--   0      501       20    98730 2023-07-05 18:53:54.000000 getdaft-0.1.8/tutorials/mnist.ipynb
--rw-r--r--   0      501       20    11690 2023-07-05 18:53:54.000000 getdaft-0.1.8/tutorials/text_to_image/text_to_image_generation.ipynb
--rw-r--r--   0      501       20     9134 2023-07-05 18:53:54.000000 getdaft-0.1.8/tutorials/text_to_image/using_cloud_with_ray.ipynb
--rw-r--r--   0      501       20    74387 2023-07-05 18:54:55.000000 getdaft-0.1.8/Cargo.lock
--rw-r--r--   0        0        0    10000 1970-01-01 00:00:00.000000 getdaft-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1205 1970-01-01 00:00:00.000000 getdaft-0.1.9/local_dependencies/daft-io/Cargo.toml
+-rw-r--r--   0      501       20     1087 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-io/src/config.rs
+-rw-r--r--   0      501       20     6412 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-io/src/http.rs
+-rw-r--r--   0      501       20    10822 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-io/src/lib.rs
+-rw-r--r--   0      501       20     7068 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-io/src/local.rs
+-rw-r--r--   0      501       20     1686 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-io/src/object_io.rs
+-rw-r--r--   0      501       20     1966 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-io/src/python.rs
+-rw-r--r--   0      501       20    17140 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-io/src/s3_like.rs
+-rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 getdaft-0.1.9/local_dependencies/daft-parquet/Cargo.toml
+-rw-r--r--   0      501       20     1851 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-parquet/src/lib.rs
+-rw-r--r--   0      501       20     3543 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-parquet/src/metadata.rs
+-rw-r--r--   0      501       20      943 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-parquet/src/python.rs
+-rw-r--r--   0      501       20     9163 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-parquet/src/read.rs
+-rw-r--r--   0      501       20     9494 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-parquet/src/read_planner.rs
+-rw-r--r--   0        0        0     1564 1970-01-01 00:00:00.000000 getdaft-0.1.9/local_dependencies/daft-core/Cargo.toml
+-rw-r--r--   0      501       20     5844 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/from.rs
+-rw-r--r--   0      501       20      734 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/iterator.rs
+-rw-r--r--   0      501       20     3012 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/mod.rs
+-rw-r--r--   0      501       20      269 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/abs.rs
+-rw-r--r--   0      501       20      738 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/apply.rs
+-rw-r--r--   0      501       20      849 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/arange.rs
+-rw-r--r--   0      501       20     7136 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/arithmetic.rs
+-rw-r--r--   0      501       20     3055 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/arrow2/comparison.rs
+-rw-r--r--   0      501       20       34 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/arrow2/mod.rs
+-rw-r--r--   0      501       20       19 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/arrow2/sort/mod.rs
+-rw-r--r--   0      501       20     3482 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/common.rs
+-rw-r--r--   0      501       20      723 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/indices.rs
+-rw-r--r--   0      501       20       47 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/mod.rs
+-rw-r--r--   0      501       20     8075 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/sort.rs
+-rw-r--r--   0      501       20     2675 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/as_arrow.rs
+-rw-r--r--   0      501       20    11395 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/broadcast.rs
+-rw-r--r--   0      501       20    68047 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/cast.rs
+-rw-r--r--   0      501       20    11029 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/compare_agg.rs
+-rw-r--r--   0      501       20    47241 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/comparison.rs
+-rw-r--r--   0      501       20     1630 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/concat.rs
+-rw-r--r--   0      501       20     5991 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/concat_agg.rs
+-rw-r--r--   0      501       20     1444 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/count.rs
+-rw-r--r--   0      501       20     1548 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/date.rs
+-rw-r--r--   0      501       20     2430 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/filter.rs
+-rw-r--r--   0      501       20     1271 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/float.rs
+-rw-r--r--   0      501       20     1936 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/full.rs
+-rw-r--r--   0      501       20     4880 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/get.rs
+-rw-r--r--   0      501       20     4119 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/groups.rs
+-rw-r--r--   0      501       20     1523 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/hash.rs
+-rw-r--r--   0      501       20    12416 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/if_else.rs
+-rw-r--r--   0      501       20    34040 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/image.rs
+-rw-r--r--   0      501       20     1069 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/len.rs
+-rw-r--r--   0      501       20     6625 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/list.rs
+-rw-r--r--   0      501       20     3367 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/list_agg.rs
+-rw-r--r--   0      501       20     1634 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/mean.rs
+-rw-r--r--   0      501       20     2652 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/mod.rs
+-rw-r--r--   0      501       20     1325 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/null.rs
+-rw-r--r--   0      501       20     3826 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/pairwise.rs
+-rw-r--r--   0      501       20    10520 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/repr.rs
+-rw-r--r--   0      501       20      491 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/search_sorted.rs
+-rw-r--r--   0      501       20    20398 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/sort.rs
+-rw-r--r--   0      501       20     2396 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/sum.rs
+-rw-r--r--   0      501       20     7346 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/take.rs
+-rw-r--r--   0      501       20      621 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/tensor.rs
+-rw-r--r--   0      501       20     5279 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/utf8.rs
+-rw-r--r--   0      501       20      995 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/pseudo_arrow/compute.rs
+-rw-r--r--   0      501       20    13611 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/pseudo_arrow/mod.rs
+-rw-r--r--   0      501       20     2502 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/array/pseudo_arrow/python.rs
+-rw-r--r--   0      501       20    10734 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/datatypes/binary_ops.rs
+-rw-r--r--   0      501       20    17055 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/datatypes/dtype.rs
+-rw-r--r--   0      501       20     2021 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/datatypes/field.rs
+-rw-r--r--   0      501       20     3187 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/datatypes/image_format.rs
+-rw-r--r--   0      501       20     6382 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/datatypes/image_mode.rs
+-rw-r--r--   0      501       20     3818 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/datatypes/logical.rs
+-rw-r--r--   0      501       20     9918 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/datatypes/matching.rs
+-rw-r--r--   0      501       20     7334 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/datatypes/mod.rs
+-rw-r--r--   0      501       20     1100 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/datatypes/time_unit.rs
+-rw-r--r--   0      501       20     5601 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/ffi.rs
+-rw-r--r--   0      501       20     6022 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/kernels/hashing.rs
+-rw-r--r--   0      501       20       54 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/kernels/mod.rs
+-rw-r--r--   0      501       20    12159 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/kernels/search_sorted.rs
+-rw-r--r--   0      501       20     3917 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/kernels/utf8.rs
+-rw-r--r--   0      501       20      578 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/lib.rs
+-rw-r--r--   0      501       20    12073 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/python/datatype.rs
+-rw-r--r--   0      501       20     1661 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/python/field.rs
+-rw-r--r--   0      501       20      610 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/python/mod.rs
+-rw-r--r--   0      501       20     2843 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/python/schema.rs
+-rw-r--r--   0      501       20    14573 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/python/series.rs
+-rw-r--r--   0      501       20     4055 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/schema.rs
+-rw-r--r--   0      501       20    10305 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/array_impl/binary_ops.rs
+-rw-r--r--   0      501       20    12778 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/array_impl/data_array.rs
+-rw-r--r--   0      501       20     9031 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/array_impl/logical_array.rs
+-rw-r--r--   0      501       20      181 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/array_impl/mod.rs
+-rw-r--r--   0      501       20     3030 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/from.rs
+-rw-r--r--   0      501       20     2309 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/mod.rs
+-rw-r--r--   0      501       20      910 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/abs.rs
+-rw-r--r--   0      501       20     5199 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/agg.rs
+-rw-r--r--   0      501       20     3419 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/arithmetic.rs
+-rw-r--r--   0      501       20     1924 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/broadcast.rs
+-rw-r--r--   0      501       20      205 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/cast.rs
+-rw-r--r--   0      501       20      682 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/comparison.rs
+-rw-r--r--   0      501       20     1565 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/concat.rs
+-rw-r--r--   0      501       20     1820 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/date.rs
+-rw-r--r--   0      501       20     3862 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/downcast.rs
+-rw-r--r--   0      501       20      693 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/filter.rs
+-rw-r--r--   0      501       20      411 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/float.rs
+-rw-r--r--   0      501       20      439 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/groups.rs
+-rw-r--r--   0      501       20      416 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/hash.rs
+-rw-r--r--   0      501       20      324 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/if_else.rs
+-rw-r--r--   0      501       20     3202 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/image.rs
+-rw-r--r--   0      501       20      297 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/len.rs
+-rw-r--r--   0      501       20     2353 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/list.rs
+-rw-r--r--   0      501       20     2541 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/mod.rs
+-rw-r--r--   0      501       20      475 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/not.rs
+-rw-r--r--   0      501       20      160 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/null.rs
+-rw-r--r--   0      501       20      645 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/search_sorted.rs
+-rw-r--r--   0      501       20     1504 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/sort.rs
+-rw-r--r--   0      501       20      662 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/take.rs
+-rw-r--r--   0      501       20     1526 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/utf8.rs
+-rw-r--r--   0      501       20     2315 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/series/series_like.rs
+-rw-r--r--   0      501       20     5401 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/utils/arrow.rs
+-rw-r--r--   0      501       20      347 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/utils/mod.rs
+-rw-r--r--   0      501       20    10066 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-core/src/utils/supertype.rs
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 getdaft-0.1.9/local_dependencies/daft-dsl/Cargo.toml
+-rw-r--r--   0      501       20      273 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/README.md
+-rw-r--r--   0      501       20     1454 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/arithmetic.rs
+-rw-r--r--   0      501       20    17967 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/expr.rs
+-rw-r--r--   0      501       20     1456 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/float/is_nan.rs
+-rw-r--r--   0      501       20      582 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/float/mod.rs
+-rw-r--r--   0      501       20     2719 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/image/crop.rs
+-rw-r--r--   0      501       20     1353 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/image/decode.rs
+-rw-r--r--   0      501       20     1790 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/image/encode.rs
+-rw-r--r--   0      501       20     1576 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/image/mod.rs
+-rw-r--r--   0      501       20     2524 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/image/resize.rs
+-rw-r--r--   0      501       20     1130 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/list/explode.rs
+-rw-r--r--   0      501       20     2329 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/list/join.rs
+-rw-r--r--   0      501       20     1493 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/list/lengths.rs
+-rw-r--r--   0      501       20     1141 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/list/mod.rs
+-rw-r--r--   0      501       20     2085 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/mod.rs
+-rw-r--r--   0      501       20     1197 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/numeric/abs.rs
+-rw-r--r--   0      501       20      575 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/numeric/mod.rs
+-rw-r--r--   0      501       20      684 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/python/mod.rs
+-rw-r--r--   0      501       20     2050 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/python/partial_udf.rs
+-rw-r--r--   0      501       20     2793 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/python/udf.rs
+-rw-r--r--   0      501       20     1344 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/temporal/day.rs
+-rw-r--r--   0      501       20     1373 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/temporal/day_of_week.rs
+-rw-r--r--   0      501       20     1415 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/temporal/mod.rs
+-rw-r--r--   0      501       20     1355 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/temporal/month.rs
+-rw-r--r--   0      501       20     1349 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/temporal/year.rs
+-rw-r--r--   0      501       20     2295 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/uri/download.rs
+-rw-r--r--   0      501       20     1073 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/uri/mod.rs
+-rw-r--r--   0      501       20     1652 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/utf8/contains.rs
+-rw-r--r--   0      501       20     1651 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/utf8/endswith.rs
+-rw-r--r--   0      501       20     1370 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/utf8/length.rs
+-rw-r--r--   0      501       20     1519 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/utf8/mod.rs
+-rw-r--r--   0      501       20     1661 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/utf8/startswith.rs
+-rw-r--r--   0      501       20      707 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/lib.rs
+-rw-r--r--   0      501       20     4967 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/lit.rs
+-rw-r--r--   0      501       20     5298 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/optimization.rs
+-rw-r--r--   0      501       20     1982 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/pyobject.rs
+-rw-r--r--   0      501       20    12239 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-dsl/src/python.rs
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 getdaft-0.1.9/local_dependencies/daft-table/Cargo.toml
+-rw-r--r--   0      501       20     2853 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-table/src/ffi.rs
+-rw-r--r--   0      501       20    20730 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-table/src/lib.rs
+-rw-r--r--   0      501       20     2168 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-table/src/ops/agg.rs
+-rw-r--r--   0      501       20     3750 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-table/src/ops/explode.rs
+-rw-r--r--   0      501       20     4415 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-table/src/ops/groups.rs
+-rw-r--r--   0      501       20     2898 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-table/src/ops/hash.rs
+-rw-r--r--   0      501       20     2499 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-table/src/ops/joins/hash_join.rs
+-rw-r--r--   0      501       20     3727 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-table/src/ops/joins/mod.rs
+-rw-r--r--   0      501       20       99 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-table/src/ops/mod.rs
+-rw-r--r--   0      501       20     3478 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-table/src/ops/partition.rs
+-rw-r--r--   0      501       20     1808 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-table/src/ops/search_sorted.rs
+-rw-r--r--   0      501       20      998 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-table/src/ops/sort.rs
+-rw-r--r--   0      501       20    11179 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/daft-table/src/python.rs
+-rw-r--r--   0        0        0      414 1970-01-01 00:00:00.000000 getdaft-0.1.9/local_dependencies/common-error/Cargo.toml
+-rw-r--r--   0      501       20     2849 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/common-error/src/error.rs
+-rw-r--r--   0      501       20       64 2023-07-25 04:16:55.000000 getdaft-0.1.9/local_dependencies/common-error/src/lib.rs
+-rw-r--r--   0        0        0     2300 1970-01-01 00:00:00.000000 getdaft-0.1.9/Cargo.toml
+-rw-r--r--   0      501       20      834 2023-07-25 04:16:55.000000 getdaft-0.1.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0      501       20      595 2023-07-25 04:16:55.000000 getdaft-0.1.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0      501       20      431 2023-07-25 04:16:55.000000 getdaft-0.1.9/.github/dependabot.yml
+-rw-r--r--   0      501       20     1063 2023-07-25 04:16:55.000000 getdaft-0.1.9/.github/release-drafter.yml
+-rw-r--r--   0      501       20     1333 2023-07-25 04:16:55.000000 getdaft-0.1.9/.github/workflows/broken-link-checker.yml
+-rw-r--r--   0      501       20     3136 2023-07-25 04:16:55.000000 getdaft-0.1.9/.github/workflows/daft-profiling.yml
+-rw-r--r--   0      501       20     1627 2023-07-25 04:16:55.000000 getdaft-0.1.9/.github/workflows/notebook-checker.yml
+-rw-r--r--   0      501       20     1958 2023-07-25 04:16:55.000000 getdaft-0.1.9/.github/workflows/property-based-tests.yml
+-rw-r--r--   0      501       20    14717 2023-07-25 04:16:55.000000 getdaft-0.1.9/.github/workflows/python-package.yml
+-rw-r--r--   0      501       20     6129 2023-07-25 04:16:55.000000 getdaft-0.1.9/.github/workflows/python-publish.yml
+-rw-r--r--   0      501       20     2416 2023-07-25 04:16:55.000000 getdaft-0.1.9/.github/workflows/ray-compatibility.yml
+-rw-r--r--   0      501       20     2696 2023-07-25 04:16:55.000000 getdaft-0.1.9/.github/workflows/release-drafter.yml
+-rw-r--r--   0      501       20      306 2023-07-25 04:16:55.000000 getdaft-0.1.9/.gitignore
+-rw-r--r--   0      501       20     2835 2023-07-25 04:16:55.000000 getdaft-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0      501       20      205 2023-07-25 04:16:55.000000 getdaft-0.1.9/.readthedocs.yaml
+-rw-r--r--   0      501       20     1550 2023-07-25 04:16:55.000000 getdaft-0.1.9/CONTRIBUTING.md
+-rw-r--r--   0      501       20    11357 2023-07-25 04:16:55.000000 getdaft-0.1.9/LICENSE
+-rw-r--r--   0      501       20     1295 2023-07-25 04:16:55.000000 getdaft-0.1.9/Makefile
+-rw-r--r--   0      501       20     8826 2023-07-25 04:16:55.000000 getdaft-0.1.9/README.rst
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/benchmarking/__init__.py
+-rw-r--r--   0      501       20      925 2023-07-25 04:16:55.000000 getdaft-0.1.9/benchmarking/parquet/README.md
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/benchmarking/parquet/__init__.py
+-rw-r--r--   0      501       20       89 2023-07-25 04:16:55.000000 getdaft-0.1.9/benchmarking/parquet/benchmark-requirements.txt
+-rw-r--r--   0      501       20     1764 2023-07-25 04:16:55.000000 getdaft-0.1.9/benchmarking/parquet/conftest.py
+-rw-r--r--   0      501       20     2019 2023-07-25 04:16:55.000000 getdaft-0.1.9/benchmarking/parquet/test_num_rowgroups.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/benchmarking/tpch/__init__.py
+-rw-r--r--   0      501       20     9495 2023-07-25 04:16:55.000000 getdaft-0.1.9/benchmarking/tpch/__main__.py
+-rw-r--r--   0      501       20    12428 2023-07-25 04:16:55.000000 getdaft-0.1.9/benchmarking/tpch/answers.py
+-rw-r--r--   0      501       20    12336 2023-07-25 04:16:55.000000 getdaft-0.1.9/benchmarking/tpch/data_generation.py
+-rw-r--r--   0      501       20     4573 2023-07-25 04:16:55.000000 getdaft-0.1.9/benchmarking/tpch/pipelined_data_generation.py
+-rw-r--r--   0      501       20     2654 2023-07-25 04:16:55.000000 getdaft-0.1.9/benchmarking/tpch/subprefix_s3_files.py
+-rw-r--r--   0      501       20     1436 2023-07-25 04:16:55.000000 getdaft-0.1.9/ci/upload_wheels.sh
+-rw-r--r--   0      501       20      446 2023-07-25 04:16:55.000000 getdaft-0.1.9/codecov.yml
+-rw-r--r--   0      501       20     2199 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/__init__.py
+-rw-r--r--   0      501       20     6724 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/analytics.py
+-rw-r--r--   0      501       20     3935 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/api_annotations.py
+-rw-r--r--   0      501       20    10591 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/arrow_utils.py
+-rw-r--r--   0      501       20     5511 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/context.py
+-rw-r--r--   0      501       20     3412 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/convert.py
+-rw-r--r--   0      501       20     1298 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/daft.pyi
+-rw-r--r--   0      501       20       94 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/dataframe/__init__.py
+-rw-r--r--   0      501       20    55044 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/dataframe/dataframe.py
+-rw-r--r--   0      501       20      306 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/dataframe/preview.py
+-rw-r--r--   0      501       20     1404 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/dataframe/to_torch.py
+-rw-r--r--   0      501       20      850 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/datasources.py
+-rw-r--r--   0      501       20    20147 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/datatype.py
+-rw-r--r--   0      501       20       84 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/errors.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/execution/__init__.py
+-rw-r--r--   0      501       20    28993 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/execution/execution_step.py
+-rw-r--r--   0      501       20    28946 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/execution/physical_plan.py
+-rw-r--r--   0      501       20     6350 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/execution/physical_plan_factory.py
+-rw-r--r--   0      501       20      170 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/expressions/__init__.py
+-rw-r--r--   0      501       20    30203 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/expressions/expressions.py
+-rw-r--r--   0      501       20      572 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/expressions/testing.py
+-rw-r--r--   0      501       20    12728 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/filesystem.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/internal/__init__.py
+-rw-r--r--   0      501       20      509 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/internal/gpu.py
+-rw-r--r--   0      501       20     1804 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/internal/rule.py
+-rw-r--r--   0      501       20     2030 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/internal/rule_runner.py
+-rw-r--r--   0      501       20     3490 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/internal/treenode.py
+-rw-r--r--   0      501       20      377 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/io/__init__.py
+-rw-r--r--   0      501       20     2456 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/io/_csv.py
+-rw-r--r--   0      501       20     1642 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/io/_json.py
+-rw-r--r--   0      501       20     2317 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/io/common.py
+-rw-r--r--   0      501       20     2036 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/io/file_path.py
+-rw-r--r--   0      501       20     1665 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/io/parquet.py
+-rw-r--r--   0      501       20      264 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/logging.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/logical/__init__.py
+-rw-r--r--   0      501       20     8601 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/logical/aggregation_plan_builder.py
+-rw-r--r--   0      501       20    38976 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/logical/logical_plan.py
+-rw-r--r--   0      501       20     1492 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/logical/map_partition_ops.py
+-rw-r--r--   0      501       20    19757 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/logical/optimizer.py
+-rw-r--r--   0      501       20     3868 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/logical/schema.py
+-rw-r--r--   0      501       20       99 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/pickle/__init__.py
+-rw-r--r--   0      501       20    34760 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/pickle/cloudpickle.py
+-rw-r--r--   0      501       20    34262 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/pickle/cloudpickle_fast.py
+-rw-r--r--   0      501       20      639 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/pickle/compat.py
+-rw-r--r--   0      501       20      312 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/pickle/pickle.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/py.typed
+-rw-r--r--   0      501       20     2036 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/resource_request.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/runners/__init__.py
+-rw-r--r--   0      501       20     4893 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/runners/partitioning.py
+-rw-r--r--   0      501       20     1488 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/runners/profiler.py
+-rw-r--r--   0      501       20    13802 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/runners/pyrunner.py
+-rw-r--r--   0      501       20    28389 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/runners/ray_runner.py
+-rw-r--r--   0      501       20     1428 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/runners/runner.py
+-rw-r--r--   0      501       20     3344 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/runners/runner_io.py
+-rw-r--r--   0      501       20    25378 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/series.py
+-rw-r--r--   0      501       20       82 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/table/__init__.py
+-rw-r--r--   0      501       20     2960 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/table/schema_inference.py
+-rw-r--r--   0      501       20    14609 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/table/table.py
+-rw-r--r--   0      501       20     9916 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/table/table_io.py
+-rw-r--r--   0      501       20     7367 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/udf.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/udf_library/__init__.py
+-rw-r--r--   0      501       20     3486 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/udf_library/url_udfs.py
+-rw-r--r--   0      501       20     3194 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/utils.py
+-rw-r--r--   0      501       20      183 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/viz/__init__.py
+-rw-r--r--   0      501       20     1929 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/viz/dataframe_display.py
+-rw-r--r--   0      501       20     1522 2023-07-25 04:16:55.000000 getdaft-0.1.9/daft/viz/html_viz_hooks.py
+-rw-r--r--   0      501       20      148 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/CONTRIBUTING.md
+-rw-r--r--   0      501       20      638 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/Makefile
+-rw-r--r--   0      501       20    73229 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/10-min.ipynb
+-rw-r--r--   0      501       20      389 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/_static/custom-function-signatures.css
+-rw-r--r--   0      501       20      565 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/_static/daft-favicon.png
+-rw-r--r--   0      501       20     7804 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/_static/daft-logo.png
+-rw-r--r--   0      501       20    42148 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/_static/daft_illustration.png
+-rw-r--r--   0      501       20      583 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/_static/dataframe-comp-table.csv
+-rw-r--r--   0      501       20    25200 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/_static/execution_model.png
+-rw-r--r--   0      501       20     1901 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/_static/header.css
+-rw-r--r--   0      501       20    32864 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/_static/high_level_architecture.png
+-rw-r--r--   0      501       20      343 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/_static/icon-menu-close.svg
+-rw-r--r--   0      501       20      333 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/_static/icon-menu-dots.svg
+-rw-r--r--   0      501       20    18177 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/_static/in_memory_data_representation.png
+-rw-r--r--   0      501       20      786 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/_static/mobile-menu.js
+-rw-r--r--   0      501       20     9142 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/_static/tpch-1000sf.html
+-rw-r--r--   0      501       20     9647 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/_static/tpch-100sf.html
+-rw-r--r--   0      501       20     8757 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/_static/tpch-nodes-count-daft-1000-sf.html
+-rw-r--r--   0      501       20      856 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/_templates/layout.html
+-rw-r--r--   0      501       20     1179 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/_templates/sections/header.html
+-rw-r--r--   0      501       20     1129 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/_templates/sections/mobile-menu.html
+-rw-r--r--   0      501       20      333 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/api_docs/context.rst
+-rw-r--r--   0      501       20     2759 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/api_docs/dataframe.rst
+-rw-r--r--   0      501       20     2318 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/api_docs/datatype.rst
+-rw-r--r--   0      501       20      139 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/api_docs/datatype_image_mode/daft.ImageMode.from_mode_string.rst
+-rw-r--r--   0      501       20      430 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/api_docs/datatype_image_mode/daft.ImageMode.rst
+-rw-r--r--   0      501       20      151 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/api_docs/datetype_image_format/daft.ImageFormat.from_format_string.rst
+-rw-r--r--   0      501       20      333 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/api_docs/datetype_image_format/daft.ImageFormat.rst
+-rw-r--r--   0      501       20     4791 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/api_docs/expressions.rst
+-rw-r--r--   0      501       20      816 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/api_docs/groupby.rst
+-rw-r--r--   0      501       20      146 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/api_docs/index.rst
+-rw-r--r--   0      501       20     1537 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/api_docs/input_output.rst
+-rw-r--r--   0      501       20      273 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/api_docs/series/daft.Series.rst
+-rw-r--r--   0      501       20      492 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/api_docs/series.rst
+-rw-r--r--   0      501       20       88 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/api_docs/udf.rst
+-rw-r--r--   0      501       20    14528 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/benchmarks/index.rst
+-rw-r--r--   0      501       20     4200 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/conf.py
+-rw-r--r--   0      501       20     5098 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/dataframe_comparison.rst
+-rw-r--r--   0      501       20     1723 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/index.rst
+-rw-r--r--   0      501       20     1356 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/install.rst
+-rw-r--r--   0      501       20      896 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/learn/index.rst
+-rw-r--r--   0      501       20     7830 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/learn/key_concepts.rst
+-rw-r--r--   0      501       20     1783 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/learn/tutorials.rst
+-rw-r--r--   0      501       20     1388 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/learn/user_guides/aggregations.rst
+-rw-r--r--   0      501       20     7009 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/learn/user_guides/dataframe-operations.rst
+-rw-r--r--   0      501       20     5281 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/learn/user_guides/datatypes.rst
+-rw-r--r--   0      501       20     9481 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/learn/user_guides/expressions.rst
+-rw-r--r--   0      501       20     8241 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/learn/user_guides/intro-dataframes.rst
+-rw-r--r--   0      501       20      206 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/learn/user_guides/partitioning.rst
+-rw-r--r--   0      501       20     3251 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/learn/user_guides/read-write.rst
+-rw-r--r--   0      501       20     1257 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/learn/user_guides/scaling-up.rst
+-rw-r--r--   0      501       20     8853 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/learn/user_guides/udf.rst
+-rw-r--r--   0      501       20     1577 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/learn/user_guides.rst
+-rw-r--r--   0      501       20     6628 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/technical_architecture.rst
+-rw-r--r--   0      501       20     1316 2023-07-25 04:16:55.000000 getdaft-0.1.9/docs/source/telemetry.rst
+-rw-r--r--   0      501       20     1871 2023-07-25 04:16:55.000000 getdaft-0.1.9/pyproject.toml
+-rw-r--r--   0      501       20     1137 2023-07-25 04:16:55.000000 getdaft-0.1.9/requirements-dev.txt
+-rw-r--r--   0      501       20       98 2023-07-25 04:16:55.000000 getdaft-0.1.9/rust-toolchain.toml
+-rw-r--r--   0      501       20      736 2023-07-25 04:16:55.000000 getdaft-0.1.9/src/lib.rs
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/__init__.py
+-rw-r--r--   0      501       20      299 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/assets/__init__.py
+-rw-r--r--   0      501       20      544 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/assets/tpch-sqlite-queries/1.sql
+-rw-r--r--   0      501       20      542 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/assets/tpch-sqlite-queries/10.sql
+-rw-r--r--   0      501       20      703 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/assets/tpch-sqlite-queries/2.sql
+-rw-r--r--   0      501       20      444 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/assets/tpch-sqlite-queries/3.sql
+-rw-r--r--   0      501       20      371 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/assets/tpch-sqlite-queries/4.sql
+-rw-r--r--   0      501       20      504 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/assets/tpch-sqlite-queries/5.sql
+-rw-r--r--   0      501       20      259 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/assets/tpch-sqlite-queries/6.sql
+-rw-r--r--   0      501       20      834 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/assets/tpch-sqlite-queries/7.sql
+-rw-r--r--   0      501       20      815 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/assets/tpch-sqlite-queries/8.sql
+-rw-r--r--   0      501       20      627 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/assets/tpch-sqlite-queries/9.sql
+-rw-r--r--   0      501       20       48 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/assets/tpch-sqlite-queries/README.md
+-rw-r--r--   0      501       20      604 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/benchmarks/conftest.py
+-rw-r--r--   0      501       20     1227 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/benchmarks/test_df_arithmetic.py
+-rw-r--r--   0      501       20     2706 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/benchmarks/test_file_read.py
+-rw-r--r--   0      501       20     5604 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/benchmarks/test_groups_and_aggs.py
+-rw-r--r--   0      501       20     7292 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/benchmarks/test_join.py
+-rw-r--r--   0      501       20     2603 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/benchmarks/test_repartition.py
+-rw-r--r--   0      501       20     4005 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/benchmarks/test_sort.py
+-rw-r--r--   0      501       20     2911 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/conftest.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/cookbook/__init__.py
+-rw-r--r--   0      501       20    13229 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/cookbook/assets/311-service-requests.24.csv
+-rw-r--r--   0      501       20      255 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/cookbook/assets/__init__.py
+-rw-r--r--   0      501       20      924 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/cookbook/assets/images/0000.jpg
+-rw-r--r--   0      501       20      941 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/cookbook/assets/images/0007.jpg
+-rw-r--r--   0      501       20     2740 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/cookbook/assets/images/0018.png
+-rw-r--r--   0      501       20     7462 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/cookbook/assets/images/0025.tiff
+-rw-r--r--   0      501       20      882 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/cookbook/conftest.py
+-rw-r--r--   0      501       20     9268 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/cookbook/test_aggregations.py
+-rw-r--r--   0      501       20     2979 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/cookbook/test_computations.py
+-rw-r--r--   0      501       20     1798 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/cookbook/test_count_rows.py
+-rw-r--r--   0      501       20     7099 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/cookbook/test_dataloading.py
+-rw-r--r--   0      501       20      800 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/cookbook/test_distinct.py
+-rw-r--r--   0      501       20     6049 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/cookbook/test_filter.py
+-rw-r--r--   0      501       20     2930 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/cookbook/test_image.py
+-rw-r--r--   0      501       20     3810 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/cookbook/test_joins.py
+-rw-r--r--   0      501       20     2878 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/cookbook/test_literals.py
+-rw-r--r--   0      501       20    10311 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/cookbook/test_pandas_cookbook.py
+-rw-r--r--   0      501       20     4148 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/cookbook/test_sorting.py
+-rw-r--r--   0      501       20     1497 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/cookbook/test_write.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/dataframe/__init__.py
+-rw-r--r--   0      501       20      751 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/dataframe/conftest.py
+-rw-r--r--   0      501       20      805 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/dataframe/test_accessors.py
+-rw-r--r--   0      501       20    10308 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/dataframe/test_aggregations.py
+-rw-r--r--   0      501       20      472 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/dataframe/test_concat.py
+-rw-r--r--   0      501       20    26819 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/dataframe/test_creation.py
+-rw-r--r--   0      501       20     1456 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/dataframe/test_decimals.py
+-rw-r--r--   0      501       20     1824 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/dataframe/test_distinct.py
+-rw-r--r--   0      501       20     1428 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/dataframe/test_explode.py
+-rw-r--r--   0      501       20     1097 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/dataframe/test_filter.py
+-rw-r--r--   0      501       20     2435 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/dataframe/test_getitem.py
+-rw-r--r--   0      501       20     3205 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/dataframe/test_iter.py
+-rw-r--r--   0      501       20     4091 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/dataframe/test_joins.py
+-rw-r--r--   0      501       20     3651 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/dataframe/test_logical_type.py
+-rw-r--r--   0      501       20      223 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/dataframe/test_repartition.py
+-rw-r--r--   0      501       20     8608 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/dataframe/test_repr.py
+-rw-r--r--   0      501       20      815 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/dataframe/test_select.py
+-rw-r--r--   0      501       20      656 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/dataframe/test_show.py
+-rw-r--r--   0      501       20     6364 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/dataframe/test_sort.py
+-rw-r--r--   0      501       20     7492 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/dataframe/test_temporals.py
+-rw-r--r--   0      501       20     2385 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/dataframe/test_to_integrations.py
+-rw-r--r--   0      501       20      850 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/dataframe/test_with_column.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/expressions/__init__.py
+-rw-r--r--   0      501       20     1417 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/expressions/test_apply.py
+-rw-r--r--   0      501       20     3533 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/expressions/test_expressions.py
+-rw-r--r--   0      501       20     4259 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/expressions/test_expressions_projection.py
+-rw-r--r--   0      501       20     5042 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/expressions/test_udf.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/expressions/typing/__init__.py
+-rw-r--r--   0      501       20     6290 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/expressions/typing/conftest.py
+-rw-r--r--   0      501       20     1363 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/expressions/typing/test_aggs.py
+-rw-r--r--   0      501       20     2335 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/expressions/typing/test_arithmetic.py
+-rw-r--r--   0      501       20      853 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/expressions/typing/test_compare.py
+-rw-r--r--   0      501       20      792 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/expressions/typing/test_dt.py
+-rw-r--r--   0      501       20      531 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/expressions/typing/test_float.py
+-rw-r--r--   0      501       20      684 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/expressions/typing/test_if_else.py
+-rw-r--r--   0      501       20      422 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/expressions/typing/test_is_null.py
+-rw-r--r--   0      501       20     1176 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/expressions/typing/test_logical.py
+-rw-r--r--   0      501       20     1544 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/expressions/typing/test_str.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/integration/__init__.py
+-rw-r--r--   0      501       20       91 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/integration/docker-compose/Dockerfile.nginx
+-rw-r--r--   0      501       20      699 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/integration/docker-compose/docker-compose.yml
+-rw-r--r--   0      501       20     1007 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/integration/docker-compose/nginx-serve-static-files.conf
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/integration/io/__init__.py
+-rw-r--r--   0      501       20     4300 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/integration/io/conftest.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/integration/io/parquet/__init__.py
+-rw-r--r--   0      501       20     8046 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/integration/io/parquet/test_remote_reads.py
+-rw-r--r--   0      501       20     2242 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/integration/io/test_url_download_http.py
+-rw-r--r--   0      501       20     1829 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/integration/io/test_url_download_local.py
+-rw-r--r--   0      501       20     1780 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/integration/io/test_url_download_public_aws_s3.py
+-rw-r--r--   0      501       20     1066 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/integration/io/test_url_download_s3_minio.py
+-rw-r--r--   0      501       20     4343 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/integration/test_tpch.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/optimizer/__init__.py
+-rw-r--r--   0      501       20     1116 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/optimizer/conftest.py
+-rw-r--r--   0      501       20     1666 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/optimizer/test_drop_projections.py
+-rw-r--r--   0      501       20     1847 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/optimizer/test_drop_repartition.py
+-rw-r--r--   0      501       20     2463 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/optimizer/test_fold_projections.py
+-rw-r--r--   0      501       20     8050 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/optimizer/test_prune_columns.py
+-rw-r--r--   0      501       20     3597 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/optimizer/test_pushdown_clauses_into_scan.py
+-rw-r--r--   0      501       20     1170 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/optimizer/test_pushdown_limit.py
+-rw-r--r--   0      501       20     8981 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/optimizer/test_pushdown_predicates.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/property_based_testing/__init__.py
+-rw-r--r--   0      501       20     4575 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/property_based_testing/strategies.py
+-rw-r--r--   0      501       20     8895 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/property_based_testing/test_sort.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/ray/__init__.py
+-rw-r--r--   0      501       20     5375 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/ray/test_dask.py
+-rw-r--r--   0      501       20     9391 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/ray/test_datasets.py
+-rw-r--r--   0      501       20      278 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/series/__init__.py
+-rw-r--r--   0      501       20     9299 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/series/test_arithmetic.py
+-rw-r--r--   0      501       20    22126 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/series/test_cast.py
+-rw-r--r--   0      501       20    17003 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/series/test_comparisons.py
+-rw-r--r--   0      501       20     7109 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/series/test_concat.py
+-rw-r--r--   0      501       20      896 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/series/test_embedding.py
+-rw-r--r--   0      501       20     6157 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/series/test_filter.py
+-rw-r--r--   0      501       20      874 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/series/test_float.py
+-rw-r--r--   0      501       20     3344 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/series/test_hash.py
+-rw-r--r--   0      501       20    21412 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/series/test_if_else.py
+-rw-r--r--   0      501       20    22626 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/series/test_image.py
+-rw-r--r--   0      501       20      889 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/series/test_numeric_ops.py
+-rw-r--r--   0      501       20     3418 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/series/test_series.py
+-rw-r--r--   0      501       20     9049 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/series/test_size_bytes.py
+-rw-r--r--   0      501       20     2188 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/series/test_slice.py
+-rw-r--r--   0      501       20     5495 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/series/test_sort.py
+-rw-r--r--   0      501       20     6020 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/series/test_take.py
+-rw-r--r--   0      501       20     1934 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/series/test_temporal_ops.py
+-rw-r--r--   0      501       20     3686 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/series/test_tensor.py
+-rw-r--r--   0      501       20     4413 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/series/test_utf8_ops.py
+-rw-r--r--   0      501       20      694 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/__init__.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/image/__init__.py
+-rw-r--r--   0      501       20     4802 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/image/test_crop.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/list/__init__.py
+-rw-r--r--   0      501       20     1156 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/list/test_list_join.py
+-rw-r--r--   0      501       20      370 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/list/test_list_lengths.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/table_io/__init__.py
+-rw-r--r--   0      501       20     6289 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/table_io/test_csv.py
+-rw-r--r--   0      501       20     4355 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/table_io/test_json.py
+-rw-r--r--   0      501       20     4778 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/table_io/test_parquet.py
+-rw-r--r--   0      501       20     2100 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/table_io/test_read_time_cast.py
+-rw-r--r--   0      501       20     1070 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/test_blackbox_kernels.py
+-rw-r--r--   0      501       20      426 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/test_broadcasts.py
+-rw-r--r--   0      501       20     2123 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/test_concat.py
+-rw-r--r--   0      501       20     4900 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/test_eval.py
+-rw-r--r--   0      501       20     3930 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/test_explodes.py
+-rw-r--r--   0      501       20     7413 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/test_filter.py
+-rw-r--r--   0      501       20    24082 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/test_from_py.py
+-rw-r--r--   0      501       20      842 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/test_head.py
+-rw-r--r--   0      501       20    10974 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/test_joins.py
+-rw-r--r--   0      501       20     7811 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/test_partitioning.py
+-rw-r--r--   0      501       20      654 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/test_size_bytes.py
+-rw-r--r--   0      501       20    10955 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/test_sorting.py
+-rw-r--r--   0      501       20    20923 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/test_table_aggs.py
+-rw-r--r--   0      501       20     5061 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/test_take.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/utf8/__init__.py
+-rw-r--r--   0      501       20     1165 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/utf8/test_compares.py
+-rw-r--r--   0      501       20      321 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/table/utf8/test_length.py
+-rw-r--r--   0      501       20     3533 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/test_analytics.py
+-rw-r--r--   0      501       20      703 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/test_datatypes.py
+-rw-r--r--   0      501       20     3653 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/test_schema.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/udf_library/__init__.py
+-rw-r--r--   0      501       20     5096 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/udf_library/test_url_udfs.py
+-rw-r--r--   0      501       20      338 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests/utils.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests_legacy/__init__.py
+-rw-r--r--   0      501       20     6988 2023-07-25 04:16:55.000000 getdaft-0.1.9/tests_legacy/test_resource_requests.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/tools/__init__.py
+-rw-r--r--   0      501       20     1633 2023-07-25 04:16:55.000000 getdaft-0.1.9/tools/patch_package_version.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/tools/wheels/__init__.py
+-rw-r--r--   0      501       20        0 2023-07-25 04:16:55.000000 getdaft-0.1.9/tools/wheels/_vendor/__init__.py
+-rw-r--r--   0      501       20     1125 2023-07-25 04:16:55.000000 getdaft-0.1.9/tools/wheels/_vendor/wheel/LICENSE.txt
+-rw-r--r--   0      501       20       59 2023-07-25 04:16:55.000000 getdaft-0.1.9/tools/wheels/_vendor/wheel/__init__.py
+-rw-r--r--   0      501       20     2499 2023-07-25 04:16:55.000000 getdaft-0.1.9/tools/wheels/_vendor/wheel/cli/__init__.py
+-rw-r--r--   0      501       20     9514 2023-07-25 04:16:55.000000 getdaft-0.1.9/tools/wheels/_vendor/wheel/cli/convert.py
+-rw-r--r--   0      501       20     3113 2023-07-25 04:16:55.000000 getdaft-0.1.9/tools/wheels/_vendor/wheel/cli/pack.py
+-rw-r--r--   0      501       20      662 2023-07-25 04:16:55.000000 getdaft-0.1.9/tools/wheels/_vendor/wheel/cli/unpack.py
+-rw-r--r--   0      501       20     1246 2023-07-25 04:16:55.000000 getdaft-0.1.9/tools/wheels/_vendor/wheel/pkginfo.py
+-rw-r--r--   0      501       20      974 2023-07-25 04:16:55.000000 getdaft-0.1.9/tools/wheels/_vendor/wheel/util.py
+-rw-r--r--   0      501       20     7125 2023-07-25 04:16:55.000000 getdaft-0.1.9/tools/wheels/_vendor/wheel/wheelfile.py
+-rw-r--r--   0      501       20      878 2023-07-25 04:16:55.000000 getdaft-0.1.9/tools/wheels/fix-and-copy-wheel.py
+-rw-r--r--   0      501       20     2981 2023-07-25 04:16:55.000000 getdaft-0.1.9/tools/wheels/tmpdirs.py
+-rw-r--r--   0      501       20     4469 2023-07-25 04:16:55.000000 getdaft-0.1.9/tools/wheels/tools.py
+-rw-r--r--   0      501       20     9484 2023-07-25 04:16:55.000000 getdaft-0.1.9/tools/wheels/wheeltools.py
+-rw-r--r--   0      501       20       19 2023-07-25 04:16:55.000000 getdaft-0.1.9/tutorials/.gitignore
+-rw-r--r--   0      501       20    19755 2023-07-25 04:16:55.000000 getdaft-0.1.9/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb
+-rw-r--r--   0      501       20        5 2023-07-25 04:16:55.000000 getdaft-0.1.9/tutorials/flyte/.dockerignore
+-rw-r--r--   0      501       20       98 2023-07-25 04:16:55.000000 getdaft-0.1.9/tutorials/flyte/Dockerfile
+-rw-r--r--   0      501       20      604 2023-07-25 04:16:55.000000 getdaft-0.1.9/tutorials/flyte/README.md
+-rw-r--r--   0      501       20     2309 2023-07-25 04:16:55.000000 getdaft-0.1.9/tutorials/flyte/app.py
+-rw-r--r--   0      501       20     2874 2023-07-25 04:16:55.000000 getdaft-0.1.9/tutorials/flyte/notebook.ipynb
+-rw-r--r--   0      501       20    12692 2023-07-25 04:16:55.000000 getdaft-0.1.9/tutorials/image_querying/top_n_red_color.ipynb
+-rw-r--r--   0      501       20    98730 2023-07-25 04:16:55.000000 getdaft-0.1.9/tutorials/mnist.ipynb
+-rw-r--r--   0      501       20    11690 2023-07-25 04:16:55.000000 getdaft-0.1.9/tutorials/text_to_image/text_to_image_generation.ipynb
+-rw-r--r--   0      501       20     9134 2023-07-25 04:16:55.000000 getdaft-0.1.9/tutorials/text_to_image/using_cloud_with_ray.ipynb
+-rw-r--r--   0      501       20    79826 2023-07-25 04:16:55.000000 getdaft-0.1.9/Cargo.lock
+-rw-r--r--   0        0        0     9992 1970-01-01 00:00:00.000000 getdaft-0.1.9/PKG-INFO
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-table/Cargo.toml` & `getdaft-0.1.9/local_dependencies/daft-io/Cargo.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,52 @@
 [dependencies]
+async-recursion = "1.0.4"
+async-trait = "0.1.71"
+aws-config = {version = "0.55.3"}
+aws-credential-types = {version = "0.55.3", features = ["hardcoded-credentials"]}
+aws-sdk-s3 = "0.28.0"
+aws-sig-auth = "0.55.3"
+aws-sigv4 = "0.55.3"
+bytes = "1.4.0"
 common-error = {path = "../common-error", default-features = false}
 daft-core = {path = "../daft-core", default-features = false}
-daft-dsl = {path = "../daft-dsl", default-features = false}
-html-escape = "0.2.13"
-num-traits = "0.2"
-prettytable-rs = "0.10"
-rand = "^0.8"
+futures = "0.3.28"
+snafu = "0.7.4"
+url = "2.4.0"
+
+[dependencies.reqwest]
+default-features = false
+features = ["stream", "rustls-tls"]
+version = "0.11.18"
 
 [features]
 default = ["python"]
-python = ["dep:pyo3", "common-error/python", "daft-core/python", "daft-dsl/python"]
+python = ["dep:pyo3", "dep:pyo3-log", "common-error/python", "daft-core/python"]
 
 [package]
 edition = "2021"
-name = "daft-table"
+name = "daft-io"
 version = "0.1.0"
 
-[dependencies.arrow2 ]
-branch = "clark/expand-casting-support"
-features = [ "chrono-tz", "compute_take", "compute_cast", "compute_aggregate", "compute_if_then_else", "compute_sort", "compute_filter", "compute_temporal", "compute_comparison", "compute_arithmetics", "compute_concatenate", "io_ipc",]
-git = "https://github.com/Eventual-Inc/arrow2"
-package = "arrow2"
-version = "0.17.1"
+[dependencies.tokio ]
+version = "1.29.1"
+features = [ "net", "time", "bytes", "process", "signal", "macros", "rt", "rt-multi-thread",]
+
+[dependencies.lazy_static ]
+version = "1.4.0"
+
+[dependencies.log ]
+features = [ "std",]
+version = "0.4.19"
 
 [dependencies.pyo3 ]
 features = [ "extension-module", "abi3-py37",]
-version = "0.19.0"
+version = "0.19.1"
 optional = true
 
 [dependencies.pyo3-log ]
 version = "0.8.2"
+optional = true
+
+[dependencies.serde ]
+features = [ "derive", "rc",]
+version = "1.0.164"
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-table/src/ffi.rs` & `getdaft-0.1.9/local_dependencies/daft-table/src/ffi.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-table/src/lib.rs` & `getdaft-0.1.9/local_dependencies/daft-table/src/lib.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-table/src/ops/agg.rs` & `getdaft-0.1.9/local_dependencies/daft-table/src/ops/agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-table/src/ops/explode.rs` & `getdaft-0.1.9/local_dependencies/daft-table/src/ops/explode.rs`

 * *Files 1% similar despite different names*

```diff
@@ -56,19 +56,19 @@
                 _ => {
                     return Err(DaftError::ValueError(
                         "Can only explode a ListExpr::Explode function expression".to_string(),
                     ))
                 }
             }
         }
-        let first_len = evaluated_columns.first().unwrap().arr_lengths()?;
+        let first_len = evaluated_columns.first().unwrap().list_lengths()?;
         if evaluated_columns
             .iter()
             .skip(1)
-            .any(|c| c.arr_lengths().unwrap().ne(&first_len))
+            .any(|c| c.list_lengths().unwrap().ne(&first_len))
         {
             return Err(DaftError::ValueError(
                 "In multicolumn explode, list length did not match".to_string(),
             ));
         }
         let mut exploded_columns = evaluated_columns
             .iter()
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-table/src/ops/groups.rs` & `getdaft-0.1.9/local_dependencies/daft-table/src/ops/groups.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-table/src/ops/hash.rs` & `getdaft-0.1.9/local_dependencies/daft-table/src/ops/hash.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-table/src/ops/joins/hash_join.rs` & `getdaft-0.1.9/local_dependencies/daft-table/src/ops/joins/hash_join.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-table/src/ops/joins/mod.rs` & `getdaft-0.1.9/local_dependencies/daft-table/src/ops/joins/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-table/src/ops/partition.rs` & `getdaft-0.1.9/local_dependencies/daft-table/src/ops/partition.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-table/src/ops/search_sorted.rs` & `getdaft-0.1.9/local_dependencies/daft-table/src/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-table/src/ops/sort.rs` & `getdaft-0.1.9/local_dependencies/daft-table/src/ops/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-table/src/python.rs` & `getdaft-0.1.9/local_dependencies/daft-table/src/python.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/common-error/src/error.rs` & `getdaft-0.1.9/local_dependencies/common-error/src/error.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-io/Cargo.toml` & `getdaft-0.1.9/local_dependencies/daft-core/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,69 @@
 [dependencies]
-async-trait = "0.1.68"
-aws-config = {version = "0.55.3"}
-aws-credential-types = {version = "0.55.3", features = ["hardcoded-credentials"]}
-aws-sdk-s3 = "0.28.0"
-aws-sig-auth = "0.55.3"
-aws-sigv4 = "0.55.3"
-bytes = "1.4.0"
+base64 = "0.21.2"
+chrono = "0.4.26"
+chrono-tz = "0.8.3"
 common-error = {path = "../common-error", default-features = false}
-daft-core = {path = "../daft-core", default-features = false}
-futures = "0.3.28"
-snafu = "0.7.4"
-tokio = {version = "1.28.2", features = ["net", "time", "bytes", "process", "signal", "macros", "rt", "rt-multi-thread"]}
-url = "2.4.0"
+dyn-clone = "1.0.11"
+fnv = "1.0.7"
+html-escape = "0.2.13"
+ndarray = "0.15.6"
+num-derive = "0.3.3"
+num-traits = "0.2"
+prettytable-rs = "0.10"
+rand = "^0.8"
+serde_json = "1.0.100"
 
-[dependencies.reqwest]
+[dependencies.image]
 default-features = false
-features = ["stream", "rustls-tls"]
-version = "0.11.18"
+features = ["gif", "jpeg", "ico", "png", "tiff", "webp", "bmp", "hdr"]
+version = "0.24.6"
+
+[dependencies.indexmap]
+features = ["serde"]
+version = "1.9.2"
+
+[dependencies.numpy]
+optional = true
+version = "0.19"
+
+[dependencies.xxhash-rust]
+features = ["xxh3", "const_xxh3"]
+version = "0.8.5"
 
 [features]
 default = ["python"]
-python = ["dep:pyo3", "dep:pyo3-log", "common-error/python", "daft-core/python"]
+python = ["dep:pyo3", "dep:numpy", "common-error/python"]
 
 [package]
 edition = "2021"
-name = "daft-io"
+name = "daft-core"
 version = "0.1.0"
 
+[dependencies.arrow2 ]
+branch = "clark/expand-casting-support"
+git = "https://github.com/Eventual-Inc/arrow2"
+package = "arrow2"
+version = "0.17.1"
+features = ["chrono-tz", "compute_take", "compute_cast", "compute_aggregate", "compute_if_then_else", "compute_sort", "compute_filter", "compute_temporal", "compute_comparison", "compute_arithmetics", "compute_concatenate", "io_ipc"]
+
+[dependencies.bincode ]
+version = "1.3.3"
+
 [dependencies.lazy_static ]
 version = "1.4.0"
 
 [dependencies.log ]
 features = [ "std",]
 version = "0.4.19"
 
 [dependencies.pyo3 ]
 features = [ "extension-module", "abi3-py37",]
-version = "0.19.0"
+version = "0.19.1"
 optional = true
 
 [dependencies.pyo3-log ]
 version = "0.8.2"
-optional = true
 
 [dependencies.serde ]
 features = [ "derive", "rc",]
 version = "1.0.164"
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-io/src/config.rs` & `getdaft-0.1.9/local_dependencies/daft-io/src/config.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-io/src/http.rs` & `getdaft-0.1.9/local_dependencies/daft-io/src/http.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-use std::{ops::Range, sync::Arc};
+use std::{num::ParseIntError, ops::Range, string::FromUtf8Error, sync::Arc};
 
 use async_trait::async_trait;
 use futures::{StreamExt, TryStreamExt};
-use lazy_static::lazy_static;
-use reqwest::header::RANGE;
+
+use reqwest::header::{CONTENT_LENGTH, RANGE};
 use snafu::{IntoError, ResultExt, Snafu};
 
 use super::object_io::{GetResult, ObjectSource};
 
 #[derive(Debug, Snafu)]
 enum Error {
     #[snafu(display("Unable to connect to {}: {}", path, source))]
@@ -18,25 +18,41 @@
 
     #[snafu(display("Unable to open {}: {}", path, source))]
     UnableToOpenFile {
         path: String,
         source: reqwest::Error,
     },
 
+    #[snafu(display("Unable to determine size of {}", path))]
+    UnableToDetermineSize { path: String },
+
     #[snafu(display("Unable to read data from {}: {}", path, source))]
     UnableToReadBytes {
         path: String,
         source: reqwest::Error,
     },
 
+    #[snafu(display("Unable to create Http Client {}", source))]
+    UnableToCreateClient { source: reqwest::Error },
+
     #[snafu(display("Unable to parse URL: \"{}\"", path))]
     InvalidUrl {
         path: String,
         source: url::ParseError,
     },
+
+    #[snafu(display(
+        "Unable to parse data as Utf8 while reading header for file: {path}. {source}"
+    ))]
+    UnableToParseUtf8 { path: String, source: FromUtf8Error },
+
+    #[snafu(display(
+        "Unable to parse data as Integer while reading header for file: {path}. {source}"
+    ))]
+    UnableToParseInteger { path: String, source: ParseIntError },
 }
 
 pub(crate) struct HttpSource {
     client: reqwest::Client,
 }
 
 impl From<Error> for super::Error {
@@ -57,24 +73,22 @@
                 store: super::SourceType::Http,
                 source: error.into(),
             },
         }
     }
 }
 
-lazy_static! {
-    static ref HTTP_CLIENT: Arc<HttpSource> = HttpSource {
-        client: reqwest::ClientBuilder::default().build().unwrap(),
-    }
-    .into();
-}
-
 impl HttpSource {
     pub async fn get_client() -> super::Result<Arc<Self>> {
-        Ok(HTTP_CLIENT.clone())
+        Ok(HttpSource {
+            client: reqwest::ClientBuilder::default()
+                .build()
+                .context(UnableToCreateClientSnafu)?,
+        }
+        .into())
     }
 }
 
 #[async_trait]
 impl ObjectSource for HttpSource {
     async fn get(&self, uri: &str, range: Option<Range<usize>>) -> super::Result<GetResult> {
         let request = self.client.get(uri);
@@ -101,22 +115,46 @@
                 path: owned_string.clone(),
             }
             .into_error(e)
             .into()
         });
         Ok(GetResult::Stream(stream.boxed(), size_bytes))
     }
+
+    async fn get_size(&self, uri: &str) -> super::Result<usize> {
+        let request = self.client.head(uri);
+        let response = request
+            .send()
+            .await
+            .context(UnableToConnectSnafu::<String> { path: uri.into() })?;
+        let response = response
+            .error_for_status()
+            .context(UnableToOpenFileSnafu::<String> { path: uri.into() })?;
+
+        let headers = response.headers();
+        match headers.get(CONTENT_LENGTH) {
+            Some(v) => {
+                let size_bytes = String::from_utf8(v.as_bytes().to_vec())
+                    .with_context(|_| UnableToParseUtf8Snafu::<String> { path: uri.into() })?;
+
+                Ok(size_bytes
+                    .parse()
+                    .with_context(|_| UnableToParseIntegerSnafu::<String> { path: uri.into() })?)
+            }
+            None => Err(Error::UnableToDetermineSize { path: uri.into() }.into()),
+        }
+    }
 }
+
 #[cfg(test)]
 mod tests {
 
     use crate::object_io::ObjectSource;
     use crate::HttpSource;
     use crate::Result;
-    use tokio;
 
     #[tokio::test]
     async fn test_full_get_from_http() -> Result<()> {
         let parquet_file_path = "https://daft-public-data.s3.us-west-2.amazonaws.com/test_fixtures/parquet_small/0dad4c3f-da0d-49db-90d8-98684571391b-0.parquet";
         let parquet_expected_md5 = "929674747af64a98aceaa6d895863bd3";
 
         let client = HttpSource::get_client().await?;
@@ -149,10 +187,12 @@
             )
             .await?
             .bytes()
             .await?;
         assert_eq!(last_bytes.len(), 10);
         assert_eq!(last_bytes.as_ref(), &all_bytes[(all_bytes.len() - 10)..]);
 
+        let size_from_get_size = client.get_size(parquet_file_path).await?;
+        assert_eq!(size_from_get_size, all_bytes.len());
         Ok(())
     }
 }
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-io/src/lib.rs` & `getdaft-0.1.9/local_dependencies/daft-io/src/lib.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #![feature(async_closure)]
 
 pub mod config;
 mod http;
 mod local;
 mod object_io;
 mod s3_like;
-
+use lazy_static::lazy_static;
 #[cfg(feature = "python")]
 pub mod python;
 
 use config::IOConfig;
+pub use object_io::GetResult;
 #[cfg(feature = "python")]
 pub use python::register_modules;
 
-use std::{borrow::Cow, hash::Hash, ops::Range, sync::Arc};
+use std::{borrow::Cow, collections::HashMap, hash::Hash, ops::Range, sync::Arc};
 
 use futures::{StreamExt, TryStreamExt};
 
 use snafu::Snafu;
 use url::ParseError;
 
 use snafu::prelude::*;
@@ -27,22 +28,18 @@
     datatypes::{BinaryArray, Utf8Array},
     DataType, IntoSeries, Series,
 };
 
 use common_error::{DaftError, DaftResult};
 use s3_like::S3LikeSource;
 
-use self::{
-    http::HttpSource,
-    local::LocalSource,
-    object_io::{GetResult, ObjectSource},
-};
+use self::{http::HttpSource, local::LocalSource, object_io::ObjectSource};
 
 #[derive(Debug, Snafu)]
-pub(crate) enum Error {
+pub enum Error {
     #[snafu(display("Generic {} error: {:?}", store, source))]
     Generic { store: SourceType, source: DynError },
 
     #[snafu(display("Object at location {} not found: {:?}", path, source))]
     NotFound { path: String, source: DynError },
 
     #[snafu(display("Invalid Argument: {:?}", msg))]
@@ -87,24 +84,106 @@
             _ => DaftError::External(err.into()),
         }
     }
 }
 
 type Result<T, E = Error> = std::result::Result<T, E>;
 
-async fn get_source(source_type: SourceType, config: &IOConfig) -> Result<Arc<dyn ObjectSource>> {
-    Ok(match source_type {
-        SourceType::File => LocalSource::get_client().await? as Arc<dyn ObjectSource>,
-        SourceType::Http => HttpSource::get_client().await? as Arc<dyn ObjectSource>,
-        SourceType::S3 => S3LikeSource::get_client(&config.s3).await? as Arc<dyn ObjectSource>,
-    })
+#[derive(Default)]
+pub struct IOClient {
+    source_type_to_store: tokio::sync::RwLock<HashMap<SourceType, Arc<dyn ObjectSource>>>,
+    config: Arc<IOConfig>,
+}
+
+impl IOClient {
+    pub fn new(config: Arc<IOConfig>) -> Result<Self> {
+        Ok(IOClient {
+            source_type_to_store: tokio::sync::RwLock::new(HashMap::new()),
+            config,
+        })
+    }
+
+    async fn get_source(&self, source_type: &SourceType) -> Result<Arc<dyn ObjectSource>> {
+        {
+            if let Some(client) = self.source_type_to_store.read().await.get(source_type) {
+                return Ok(client.clone());
+            }
+        }
+        let mut w_handle = self.source_type_to_store.write().await;
+
+        if let Some(client) = w_handle.get(source_type) {
+            return Ok(client.clone());
+        }
+
+        let new_source = match source_type {
+            SourceType::File => LocalSource::get_client().await? as Arc<dyn ObjectSource>,
+            SourceType::Http => HttpSource::get_client().await? as Arc<dyn ObjectSource>,
+            SourceType::S3 => {
+                S3LikeSource::get_client(&self.config.s3).await? as Arc<dyn ObjectSource>
+            }
+        };
+
+        if w_handle.get(source_type).is_none() {
+            w_handle.insert(*source_type, new_source.clone());
+        }
+        Ok(new_source)
+    }
+
+    pub async fn single_url_get(
+        &self,
+        input: String,
+        range: Option<Range<usize>>,
+    ) -> Result<GetResult> {
+        let (scheme, path) = parse_url(&input)?;
+        let source = self.get_source(&scheme).await?;
+        source.get(path.as_ref(), range).await
+    }
+
+    pub async fn single_url_get_size(&self, input: String) -> Result<usize> {
+        let (scheme, path) = parse_url(&input)?;
+        let source = self.get_source(&scheme).await?;
+        source.get_size(path.as_ref()).await
+    }
+
+    async fn single_url_download(
+        &self,
+        index: usize,
+        input: Option<String>,
+        raise_error_on_failure: bool,
+    ) -> Result<Option<bytes::Bytes>> {
+        let value = if let Some(input) = input {
+            let response = self.single_url_get(input, None).await;
+            let res = match response {
+                Ok(res) => res.bytes().await,
+                Err(err) => Err(err),
+            };
+            Some(res)
+        } else {
+            None
+        };
+
+        match value {
+            Some(Ok(bytes)) => Ok(Some(bytes)),
+            Some(Err(err)) => match raise_error_on_failure {
+                true => Err(err),
+                false => {
+                    log::warn!(
+                        "Error occurred during url_download at index: {index} {} (falling back to Null)",
+                        err
+                    );
+                    Ok(None)
+                }
+            },
+            None => Ok(None),
+        }
+    }
 }
 
 #[derive(Debug, Hash, PartialEq, std::cmp::Eq, Clone, Copy)]
-pub(crate) enum SourceType {
+pub enum SourceType {
     File,
     Http,
     S3,
 }
 
 impl std::fmt::Display for SourceType {
     fn fmt(&self, f: &mut std::fmt::Formatter) -> std::fmt::Result {
@@ -134,54 +213,51 @@
         "file" => Ok((SourceType::File, fixed_input)),
         "http" | "https" => Ok((SourceType::Http, fixed_input)),
         "s3" => Ok((SourceType::S3, fixed_input)),
         _ => Err(Error::NotImplementedSource { store: scheme }),
     }
 }
 
-async fn single_url_get(
-    input: String,
-    range: Option<Range<usize>>,
-    config: &IOConfig,
-) -> Result<GetResult> {
-    let (scheme, path) = parse_url(&input)?;
-    let source = get_source(scheme, config).await?;
-    source.get(path.as_ref(), range).await
+lazy_static! {
+    static ref THREADED_RUNTIME: Arc<tokio::runtime::Runtime> = Arc::new(
+        tokio::runtime::Builder::new_multi_thread()
+            .enable_all()
+            .build()
+            .unwrap()
+    );
+    static ref CLIENT_CACHE: tokio::sync::RwLock<HashMap<IOConfig, Arc<IOClient>>> =
+        tokio::sync::RwLock::new(HashMap::new());
 }
 
-async fn single_url_download(
-    index: usize,
-    input: Option<String>,
-    raise_error_on_failure: bool,
-    config: Arc<IOConfig>,
-) -> Result<Option<bytes::Bytes>> {
-    let value = if let Some(input) = input {
-        let response = single_url_get(input, None, config.as_ref()).await;
-        let res = match response {
-            Ok(res) => res.bytes().await,
-            Err(err) => Err(err),
-        };
-        Some(res)
+pub fn get_io_client(config: Arc<IOConfig>) -> DaftResult<Arc<IOClient>> {
+    let read_handle = CLIENT_CACHE.blocking_read();
+    if let Some(client) = read_handle.get(&config) {
+        Ok(client.clone())
     } else {
-        None
-    };
+        drop(read_handle);
 
-    match value {
-        Some(Ok(bytes)) => Ok(Some(bytes)),
-        Some(Err(err)) => match raise_error_on_failure {
-            true => Err(err),
-            false => {
-                log::warn!(
-                    "Error occurred during url_download at index: {index} {} (falling back to Null)",
-                    err
-                );
-                Ok(None)
-            }
-        },
-        None => Ok(None),
+        let mut w_handle = CLIENT_CACHE.blocking_write();
+        if let Some(client) = w_handle.get(&config) {
+            Ok(client.clone())
+        } else {
+            let client = Arc::new(IOClient::new(config.clone())?);
+            w_handle.insert(config.as_ref().clone(), client.clone());
+            Ok(client)
+        }
+    }
+}
+
+pub fn get_runtime(multi_thread: bool) -> DaftResult<Arc<tokio::runtime::Runtime>> {
+    match multi_thread {
+        false => Ok(Arc::new(
+            tokio::runtime::Builder::new_current_thread()
+                .enable_all()
+                .build()?,
+        )),
+        true => Ok(THREADED_RUNTIME.clone()),
     }
 }
 
 pub fn _url_download(
     array: &Utf8Array,
     max_connections: usize,
     raise_error_on_failure: bool,
@@ -192,47 +268,44 @@
     let name = array.name();
     ensure!(
         max_connections > 0,
         InvalidArgumentSnafu {
             msg: "max_connections for url_download must be non-zero".to_owned()
         }
     );
-    let rt = match multi_thread {
-        false => tokio::runtime::Builder::new_current_thread()
-            .enable_all()
-            .build(),
-        true => tokio::runtime::Builder::new_multi_thread()
-            .enable_all()
-            .build(),
-    }?;
 
+    let runtime_handle = get_runtime(multi_thread)?;
+    let _rt_guard = runtime_handle.enter();
     let max_connections = match multi_thread {
         false => max_connections,
         true => max_connections * usize::from(std::thread::available_parallelism()?),
     };
-    // let thread_max_connections =
+    let io_client = get_io_client(config)?;
+
     let fetches = futures::stream::iter(urls.enumerate().map(|(i, url)| {
         let owned_url = url.map(|s| s.to_string());
-        let owned_config = config.clone();
+        let owned_client = io_client.clone();
         tokio::spawn(async move {
             (
                 i,
-                single_url_download(i, owned_url, raise_error_on_failure, owned_config).await,
+                owned_client
+                    .single_url_download(i, owned_url, raise_error_on_failure)
+                    .await,
             )
         })
     }))
     .buffer_unordered(max_connections)
     .then(async move |r| match r {
         Ok((i, Ok(v))) => Ok((i, v)),
         Ok((_i, Err(error))) => Err(error),
         Err(error) => Err(Error::JoinError { source: error }),
     });
 
     let collect_future = fetches.try_collect::<Vec<_>>();
-    let mut results = rt.block_on(collect_future)?;
+    let mut results = runtime_handle.block_on(collect_future)?;
 
     results.sort_by_key(|k| k.0);
     let mut offsets: Vec<i64> = Vec::with_capacity(results.len() + 1);
     offsets.push(0);
     let mut valid = Vec::with_capacity(results.len());
     valid.reserve(results.len());
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-io/src/local.rs` & `getdaft-0.1.9/local_dependencies/daft-io/src/local.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-use std::io::{Seek, SeekFrom};
+use std::io::SeekFrom;
 use std::ops::Range;
 use std::path::PathBuf;
 
 use super::object_io::{GetResult, ObjectSource};
 use super::Result;
 use async_trait::async_trait;
 use bytes::Bytes;
 use snafu::{ResultExt, Snafu};
 use std::sync::Arc;
-use tokio::io::{AsyncReadExt, AsyncSeek, AsyncSeekExt};
+use tokio::io::{AsyncReadExt, AsyncSeekExt};
 use url::ParseError;
 pub(crate) struct LocalSource {}
 
 #[derive(Debug, Snafu)]
 enum Error {
     #[snafu(display("Unable to open file {}: {}", path, source))]
     UnableToOpenFile {
@@ -92,14 +92,35 @@
         } else {
             return Err(Error::InvalidFilePath {
                 path: uri.to_string(),
             }
             .into());
         }
     }
+
+    async fn get_size(&self, uri: &str) -> super::Result<usize> {
+        const TO_STRIP: &str = "file://";
+        if let Some(p) = uri.strip_prefix(TO_STRIP) {
+            let path = std::path::Path::new(p);
+            let file = tokio::fs::File::open(path)
+                .await
+                .context(UnableToOpenFileSnafu {
+                    path: path.to_string_lossy(),
+                })?;
+            let metadata = file.metadata().await.context(UnableToOpenFileSnafu {
+                path: path.to_string_lossy(),
+            })?;
+            return Ok(metadata.len() as usize);
+        } else {
+            return Err(Error::InvalidFilePath {
+                path: uri.to_string(),
+            }
+            .into());
+        }
+    }
 }
 
 pub(crate) async fn collect_file(local_file: LocalFile) -> Result<Bytes> {
     let path = &local_file.path;
     let mut file = tokio::fs::File::open(path)
         .await
         .context(UnableToOpenFileSnafu {
@@ -141,15 +162,15 @@
 mod tests {
 
     use std::io::Write;
 
     use crate::object_io::ObjectSource;
     use crate::Result;
     use crate::{HttpSource, LocalSource};
-    use tokio;
+
     #[tokio::test]
     async fn test_full_get_from_local() -> Result<()> {
         let mut file1 = tempfile::NamedTempFile::new().unwrap();
         let parquet_file_path = "https://daft-public-data.s3.us-west-2.amazonaws.com/test_fixtures/parquet_small/0dad4c3f-da0d-49db-90d8-98684571391b-0.parquet";
         let parquet_expected_md5 = "929674747af64a98aceaa6d895863bd3";
 
         let client = HttpSource::get_client().await?;
@@ -191,10 +212,13 @@
             )
             .await?
             .bytes()
             .await?;
         assert_eq!(last_bytes.len(), 10);
         assert_eq!(last_bytes.as_ref(), &all_bytes[(all_bytes.len() - 10)..]);
 
+        let size_from_get_size = client.get_size(parquet_file_path.as_str()).await?;
+        assert_eq!(size_from_get_size, all_bytes.len());
+
         Ok(())
     }
 }
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-io/src/object_io.rs` & `getdaft-0.1.9/local_dependencies/daft-io/src/object_io.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 use std::ops::Range;
-use std::path::PathBuf;
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use futures::stream::{BoxStream, Stream};
 use futures::StreamExt;
 
 use crate::local::{collect_file, LocalFile};
 
-pub(crate) enum GetResult {
+pub enum GetResult {
     File(LocalFile),
     Stream(BoxStream<'static, super::Result<Bytes>>, Option<usize>),
 }
 
 async fn collect_bytes<S>(mut stream: S, size_hint: Option<usize>) -> super::Result<Bytes>
 where
     S: Stream<Item = super::Result<Bytes>> + Send + Unpin,
@@ -48,8 +47,9 @@
 
 #[async_trait]
 pub(crate) trait ObjectSource: Sync + Send {
     async fn get(&self, uri: &str, range: Option<Range<usize>>) -> super::Result<GetResult>;
     async fn get_range(&self, uri: &str, range: Range<usize>) -> super::Result<GetResult> {
         self.get(uri, Some(range)).await
     }
+    async fn get_size(&self, uri: &str) -> super::Result<usize>;
 }
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-io/src/python.rs` & `getdaft-0.1.9/local_dependencies/daft-io/src/python.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-io/src/s3_like.rs` & `getdaft-0.1.9/local_dependencies/daft-io/src/s3_like.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 use async_trait::async_trait;
+use reqwest::StatusCode;
+use s3::operation::head_object::HeadObjectError;
 
 use crate::config::S3Config;
 use crate::SourceType;
 use aws_config::SdkConfig;
 use aws_credential_types::cache::ProvideCachedCredentials;
 use aws_credential_types::provider::error::CredentialsError;
 use aws_sig_auth::signer::SigningRequirements;
 use futures::{StreamExt, TryStreamExt};
 use s3::client::customize::Response;
 use s3::config::{Credentials, Region};
-use s3::error::{ProvideErrorMetadata, SdkError};
+use s3::error::SdkError;
 use s3::operation::get_object::GetObjectError;
 use snafu::{IntoError, ResultExt, Snafu};
 use url::ParseError;
 
 use super::object_io::{GetResult, ObjectSource};
+use async_recursion::async_recursion;
 use aws_sdk_s3 as s3;
 use aws_sdk_s3::primitives::ByteStreamError;
-use lazy_static::lazy_static;
+
 use std::collections::HashMap;
 use std::ops::Range;
 use std::string::FromUtf8Error;
-use std::sync::{Arc, RwLock};
-
-#[derive(Clone)]
+use std::sync::Arc;
 pub(crate) struct S3LikeSource {
-    s3_client: s3::Client,
+    region_to_client_map: tokio::sync::RwLock<HashMap<Region, Arc<s3::Client>>>,
+    default_region: Region,
     s3_config: S3Config,
-    http_client: reqwest::Client,
     anonymous: bool,
 }
 
 #[derive(Debug, Snafu)]
 enum Error {
     #[snafu(display("Unable to open {}: {}", path, s3::error::DisplayErrorContext(source)))]
     UnableToOpenFile {
         path: String,
         source: SdkError<GetObjectError, Response>,
     },
 
+    #[snafu(display("Unable to head {}: {}", path, s3::error::DisplayErrorContext(source)))]
+    UnableToHeadFile {
+        path: String,
+        source: SdkError<HeadObjectError, Response>,
+    },
+
     #[snafu(display("Unable to query the region for {}: {}", path, source))]
     UnableToQueryRegion {
         path: String,
         source: reqwest::Error,
     },
 
     #[snafu(display("Unable missing header: {header} when performing request for: {path}"))]
@@ -106,15 +113,15 @@
                 store: SourceType::S3,
                 source: err.into(),
             },
         }
     }
 }
 
-async fn build_client(config: &S3Config) -> super::Result<S3LikeSource> {
+async fn build_s3_client(config: &S3Config) -> super::Result<(bool, s3::Client)> {
     const DEFAULT_REGION: Region = Region::from_static("us-east-1");
 
     let mut anonymous = config.anonymous;
 
     let conf: SdkConfig = if anonymous {
         aws_config::SdkConfig::builder().build()
     } else {
@@ -161,63 +168,83 @@
                 anonymous = true;
                 Ok(())
             },
             Err(err) => Err(err),
         }.with_context(|_| UnableToLoadCredentialsSnafu {})?;
     };
 
-    let client = s3::Client::from_conf(s3_conf);
+    Ok((anonymous, s3::Client::from_conf(s3_conf)))
+}
 
+async fn build_client(config: &S3Config) -> super::Result<S3LikeSource> {
+    let (anonymous, client) = build_s3_client(config).await?;
+    let mut client_map = HashMap::new();
+    let default_region = client.conf().region().unwrap().clone();
+    client_map.insert(default_region.clone(), client.into());
     Ok(S3LikeSource {
-        s3_client: client,
+        region_to_client_map: tokio::sync::RwLock::new(client_map),
         s3_config: config.clone(),
-        http_client: reqwest::Client::builder()
-            .build()
-            .with_context(|_| UnableToCreateClientSnafu {})?,
-        anonymous: anonymous,
+        default_region,
+        anonymous,
     })
 }
-
-lazy_static! {
-    static ref S3_CLIENT_MAP: RwLock<HashMap<S3Config, Arc<S3LikeSource>>> =
-        RwLock::new(HashMap::new());
-}
+const REGION_HEADER: &str = "x-amz-bucket-region";
 
 impl S3LikeSource {
     pub async fn get_client(config: &S3Config) -> super::Result<Arc<S3LikeSource>> {
+        Ok(build_client(config).await?.into())
+    }
+
+    async fn get_s3_client(&self, region: &Region) -> super::Result<Arc<s3::Client>> {
         {
-            if let Some(client) = S3_CLIENT_MAP.read().unwrap().get(config) {
+            if let Some(client) = self.region_to_client_map.read().await.get(region) {
                 return Ok(client.clone());
             }
         }
 
-        let new_client = Arc::new(build_client(config).await?);
+        let mut w_handle = self.region_to_client_map.write().await;
 
-        let mut w_handle = S3_CLIENT_MAP.write().unwrap();
-        if w_handle.get(config).is_none() {
-            w_handle.insert(config.clone(), new_client.clone());
+        if let Some(client) = w_handle.get(region) {
+            return Ok(client.clone());
         }
-        Ok(w_handle.get(config).unwrap().clone())
+
+        let mut new_config = self.s3_config.clone();
+        new_config.region_name = Some(region.to_string());
+        let (_, new_client) = build_s3_client(&new_config).await?;
+
+        if w_handle.get(region).is_none() {
+            w_handle.insert(region.clone(), new_client.into());
+        }
+        Ok(w_handle.get(region).unwrap().clone())
     }
-}
 
-#[async_trait]
-impl ObjectSource for S3LikeSource {
-    async fn get(&self, uri: &str, range: Option<Range<usize>>) -> super::Result<GetResult> {
+    #[async_recursion]
+    async fn _get_impl(
+        &self,
+        uri: &str,
+        range: Option<Range<usize>>,
+        region: &Region,
+    ) -> super::Result<GetResult> {
         let parsed = url::Url::parse(uri).with_context(|_| InvalidUrlSnafu { path: uri })?;
         let bucket = match parsed.host_str() {
             Some(s) => Ok(s),
             None => Err(Error::InvalidUrl {
                 path: uri.into(),
                 source: ParseError::EmptyHost,
             }),
         }?;
         let key = parsed.path();
         if let Some(key) = key.strip_prefix('/') {
-            let request = self.s3_client.get_object().bucket(bucket).key(key);
+            let request = self
+                .get_s3_client(region)
+                .await?
+                .get_object()
+                .bucket(bucket)
+                .key(key);
+
             let request = match &range {
                 None => request,
                 Some(range) => request.range(format!(
                     "bytes={}-{}",
                     range.start,
                     range.end.saturating_sub(1)
                 )),
@@ -257,76 +284,152 @@
                             }
                             .into_error(e)
                             .into()
                         })
                         .boxed();
                     Ok(GetResult::Stream(stream, Some(v.content_length as usize)))
                 }
-                Err(SdkError::ServiceError(err)) => match err.err() {
-                    GetObjectError::Unhandled(unhandled) => match unhandled.meta().code() {
-                        Some("PermanentRedirect") if self.s3_config.endpoint_url.is_none() => {
-                            log::warn!("S3 Region of {uri} doesn't match that of the client: {:?}, Attempting to Resolve.", self.s3_client.conf().region().map_or("", |v| v.as_ref()));
-                            let head = self
-                                .http_client
-                                .head(format! {"https://{bucket}.s3.amazonaws.com"})
-                                .send()
-                                .await
-                                .with_context(|_| UnableToQueryRegionSnafu::<String> {
-                                    path: uri.into(),
-                                })?;
-                            const REGION_HEADER: &str = "x-amz-bucket-region";
-                            let headers = head.headers();
+
+                Err(SdkError::ServiceError(err)) => {
+                    let bad_response = err.raw().http();
+                    match bad_response.status() {
+                        StatusCode::MOVED_PERMANENTLY => {
+                            let headers = bad_response.headers();
                             let new_region =
                                 headers.get(REGION_HEADER).ok_or(Error::MissingHeader {
                                     path: uri.into(),
                                     header: REGION_HEADER.into(),
                                 })?;
 
-                            let mut new_config = self.s3_config.clone();
-                            new_config.region_name = Some(
-                                String::from_utf8(new_region.as_bytes().to_vec()).with_context(
-                                    |_| UnableToParseUtf8Snafu::<String> { path: uri.into() },
-                                )?,
-                            );
-
-                            let new_client = S3LikeSource::get_client(&new_config).await?;
-                            log::warn!("Correct S3 Region of {uri} found: {:?}. Attempting GET in that region with new client", new_client.s3_client.conf().region().map_or("", |v| v.as_ref()));
-                            return new_client.get(uri, range).await;
+                            let region_name = String::from_utf8(new_region.as_bytes().to_vec())
+                                .with_context(|_| UnableToParseUtf8Snafu::<String> {
+                                    path: uri.into(),
+                                })?;
+
+                            let new_region = Region::new(region_name);
+                            log::warn!("S3 Region of {uri} different than client {:?} vs {:?} Attempting GET in that region with new client", new_region, region);
+                            self._get_impl(uri, range, &new_region).await
                         }
                         _ => Err(UnableToOpenFileSnafu { path: uri }
                             .into_error(SdkError::ServiceError(err))
                             .into()),
-                    },
-                    &_ => Err(UnableToOpenFileSnafu { path: uri }
-                        .into_error(SdkError::ServiceError(err))
-                        .into()),
-                },
+                    }
+                }
                 Err(err) => Err(UnableToOpenFileSnafu { path: uri }.into_error(err).into()),
             }
         } else {
-            return Err(Error::NotAFile { path: uri.into() }.into());
+            Err(Error::NotAFile { path: uri.into() }.into())
+        }
+    }
+
+    #[async_recursion]
+    async fn _head_impl(&self, uri: &str, region: &Region) -> super::Result<usize> {
+        let parsed = url::Url::parse(uri).with_context(|_| InvalidUrlSnafu { path: uri })?;
+
+        let bucket = match parsed.host_str() {
+            Some(s) => Ok(s),
+            None => Err(Error::InvalidUrl {
+                path: uri.into(),
+                source: ParseError::EmptyHost,
+            }),
+        }?;
+        let key = parsed.path();
+        if let Some(key) = key.strip_prefix('/') {
+            let request = self
+                .get_s3_client(region)
+                .await?
+                .head_object()
+                .bucket(bucket)
+                .key(key);
+
+            let response = if self.anonymous {
+                request
+                    .customize_middleware()
+                    .await
+                    .unwrap()
+                    .map_operation::<Error>(|mut o| {
+                        {
+                            let mut properties = o.properties_mut();
+                            let mut config = properties
+                                .get_mut::<::aws_sig_auth::signer::OperationSigningConfig>()
+                                .expect("signing config added by make_operation()");
+
+                            config.signing_requirements = SigningRequirements::Disabled;
+                        }
+                        Ok(o)
+                    })
+                    .unwrap()
+                    .send()
+                    .await
+            } else {
+                request.send().await
+            };
+
+            match response {
+                Ok(v) => Ok(v.content_length() as usize),
+                Err(SdkError::ServiceError(err)) => {
+                    let bad_response = err.raw().http();
+                    match bad_response.status() {
+                        StatusCode::MOVED_PERMANENTLY => {
+                            let headers = bad_response.headers();
+                            let new_region =
+                                headers.get(REGION_HEADER).ok_or(Error::MissingHeader {
+                                    path: uri.into(),
+                                    header: REGION_HEADER.into(),
+                                })?;
+
+                            let region_name = String::from_utf8(new_region.as_bytes().to_vec())
+                                .with_context(|_| UnableToParseUtf8Snafu::<String> {
+                                    path: uri.into(),
+                                })?;
+
+                            let new_region = Region::new(region_name);
+                            log::warn!("S3 Region of {uri} different than client {:?} vs {:?} Attempting HEAD in that region with new client", new_region, region);
+                            self._head_impl(uri, &new_region).await
+                        }
+                        _ => Err(UnableToHeadFileSnafu { path: uri }
+                            .into_error(SdkError::ServiceError(err))
+                            .into()),
+                    }
+                }
+                Err(err) => Err(UnableToHeadFileSnafu { path: uri }.into_error(err).into()),
+            }
+        } else {
+            Err(Error::NotAFile { path: uri.into() }.into())
         }
     }
 }
 
+#[async_trait]
+impl ObjectSource for S3LikeSource {
+    async fn get(&self, uri: &str, range: Option<Range<usize>>) -> super::Result<GetResult> {
+        self._get_impl(uri, range, &self.default_region).await
+    }
+
+    async fn get_size(&self, uri: &str) -> super::Result<usize> {
+        self._head_impl(uri, &self.default_region).await
+    }
+}
+
 #[cfg(test)]
 mod tests {
 
     use crate::object_io::ObjectSource;
     use crate::S3LikeSource;
     use crate::{config::S3Config, Result};
-    use tokio;
 
     #[tokio::test]
     async fn test_full_get_from_s3() -> Result<()> {
         let parquet_file_path = "s3://daft-public-data/test_fixtures/parquet_small/0dad4c3f-da0d-49db-90d8-98684571391b-0.parquet";
         let parquet_expected_md5 = "929674747af64a98aceaa6d895863bd3";
 
-        let mut config = S3Config::default();
-        config.anonymous = true;
+        let config = S3Config {
+            anonymous: true,
+            ..Default::default()
+        };
         let client = S3LikeSource::get_client(&config).await?;
         let parquet_file = client.get(parquet_file_path, None).await?;
         let bytes = parquet_file.bytes().await?;
         let all_bytes = bytes.as_ref();
         let checksum = format!("{:x}", md5::compute(all_bytes));
         assert_eq!(checksum, parquet_expected_md5);
 
@@ -353,10 +456,13 @@
             )
             .await?
             .bytes()
             .await?;
         assert_eq!(last_bytes.len(), 10);
         assert_eq!(last_bytes.as_ref(), &all_bytes[(all_bytes.len() - 10)..]);
 
+        let size_from_get_size = client.get_size(parquet_file_path).await?;
+        assert_eq!(size_from_get_size, all_bytes.len());
+
         Ok(())
     }
 }
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/Cargo.toml` & `getdaft-0.1.9/local_dependencies/daft-dsl/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 version = "0.1.0"
 
 [dependencies.bincode ]
 version = "1.3.3"
 
 [dependencies.pyo3 ]
 features = [ "extension-module", "abi3-py37",]
-version = "0.19.0"
+version = "0.19.1"
 optional = true
 
 [dependencies.pyo3-log ]
 version = "0.8.2"
 optional = true
 
 [dependencies.serde ]
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/arithmetic.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/expr.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/expr.rs`

 * *Files 4% similar despite different names*

```diff
@@ -252,54 +252,31 @@
             BinaryOp { op, left, right } => {
                 let left_field = left.to_field(schema)?;
                 let right_field = right.to_field(schema)?;
 
                 match op {
                     // Logical operations
                     Operator::And | Operator::Or | Operator::Xor => {
-                        match try_get_supertype(&left_field.dtype, &right_field.dtype) {
-                            Ok(DataType::Boolean) => Ok(Field::new(
-                                left_field.name.as_str(),
-                                DataType::Boolean,
-                            )),
-                            #[cfg(feature = "python")]
-                            Ok(DataType::Python) => Ok(Field::new(
-                                left_field.name.as_str(),
-                                DataType::Boolean,
-                            )),
-                            Ok(other_stype) => Err(DaftError::TypeError(format!(
-                                "Expected boolean supertype arguments for {op} but received {left_field} {op} {right_field} with supertype {other_stype}",
-                            ))),
-                            Err(_) => Err(DaftError::TypeError(format!("Expected left and right arguments to be castable to the same supertype for comparison {op}, but received {left_field} and {right_field}"))),
-                        }
+                        let result_type = left_field.dtype.logical_op(&right_field.dtype)?;
+                        Ok(Field::new(left_field.name.as_str(), result_type))
                     }
 
                     // Comparison operations
                     Operator::Lt
                     | Operator::Gt
                     | Operator::Eq
                     | Operator::NotEq
                     | Operator::LtEq
                     | Operator::GtEq => {
-                        // TODO: [ISSUE-688] Make Binary type comparable
-                        if left_field.dtype == DataType::Binary
-                            || right_field.dtype == DataType::Binary
-                        {
-                            return Err(DaftError::TypeError(format!(
-                                "Binary types cannot be compared: {left_field} {op} {right_field}",
-                            )));
-                        }
-                        match try_get_supertype(&left_field.dtype, &right_field.dtype) {
-                            Ok(_) => Ok(Field::new(
-                                left.to_field(schema)?.name.as_str(),
-                                DataType::Boolean,
-                            )),
-                            Err(_) => Err(DaftError::TypeError(format!("Expected left and right arguments to be castable to the same supertype for comparison {op}, but received {left_field} and {right_field}"))),
-                        }
+                        let (result_type, _comp_type) =
+                            left_field.dtype.comparison_op(&right_field.dtype)?;
+                        Ok(Field::new(left_field.name.as_str(), result_type))
                     }
+
+                    // Arithmetic operations
                     Operator::Plus => {
                         let result_type = (&left_field.dtype + &right_field.dtype)?;
                         Ok(Field::new(left_field.name.as_str(), result_type))
                     }
                     Operator::Minus => {
                         let result_type = (&left_field.dtype - &right_field.dtype)?;
                         Ok(Field::new(left_field.name.as_str(), result_type))
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/float/is_nan.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/float/is_nan.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/float/mod.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/float/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/image/decode.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/image/decode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/image/encode.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/image/encode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/image/mod.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/image/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+mod crop;
 mod decode;
 mod encode;
 mod resize;
 
+use crop::CropEvaluator;
 use decode::DecodeEvaluator;
 use encode::EncodeEvaluator;
 use resize::ResizeEvaluator;
 use serde::{Deserialize, Serialize};
 
 use daft_core::datatypes::ImageFormat;
 
@@ -14,25 +16,27 @@
 use super::FunctionEvaluator;
 
 #[derive(Debug, Clone, Serialize, Deserialize, PartialEq)]
 pub enum ImageExpr {
     Decode(),
     Encode { image_format: ImageFormat },
     Resize { w: u32, h: u32 },
+    Crop(),
 }
 
 impl ImageExpr {
     #[inline]
     pub fn get_evaluator(&self) -> &dyn FunctionEvaluator {
         use ImageExpr::*;
 
         match self {
             Decode() => &DecodeEvaluator {},
             Encode { .. } => &EncodeEvaluator {},
             Resize { .. } => &ResizeEvaluator {},
+            Crop { .. } => &CropEvaluator {},
         }
     }
 }
 
 pub fn decode(input: &Expr) -> Expr {
     Expr::Function {
         func: super::FunctionExpr::Image(ImageExpr::Decode()),
@@ -49,7 +53,14 @@
 
 pub fn resize(input: &Expr, w: u32, h: u32) -> Expr {
     Expr::Function {
         func: super::FunctionExpr::Image(ImageExpr::Resize { w, h }),
         inputs: vec![input.clone()],
     }
 }
+
+pub fn crop(input: &Expr, bbox: &Expr) -> Expr {
+    Expr::Function {
+        func: super::FunctionExpr::Image(ImageExpr::Crop()),
+        inputs: vec![input.clone(), bbox.clone()],
+    }
+}
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/image/resize.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/image/resize.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/list/explode.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/list/explode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/list/join.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/list/join.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/list/mod.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/list/mod.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 mod explode;
 mod join;
+mod lengths;
 
 use explode::ExplodeEvaluator;
 use join::JoinEvaluator;
+use lengths::LengthsEvaluator;
 use serde::{Deserialize, Serialize};
 
 use crate::Expr;
 
 use super::FunctionEvaluator;
 
 #[derive(Debug, Clone, Serialize, Deserialize, PartialEq)]
 pub enum ListExpr {
     Explode,
     Join,
+    Lengths,
 }
 
 impl ListExpr {
     #[inline]
     pub fn get_evaluator(&self) -> &dyn FunctionEvaluator {
         use ListExpr::*;
         match self {
             Explode => &ExplodeEvaluator {},
             Join => &JoinEvaluator {},
+            Lengths => &LengthsEvaluator {},
         }
     }
 }
 
 pub fn explode(input: &Expr) -> Expr {
     Expr::Function {
         func: super::FunctionExpr::List(ListExpr::Explode),
@@ -35,7 +39,14 @@
 
 pub fn join(input: &Expr, delimiter: &Expr) -> Expr {
     Expr::Function {
         func: super::FunctionExpr::List(ListExpr::Join),
         inputs: vec![input.clone(), delimiter.clone()],
     }
 }
+
+pub fn lengths(input: &Expr) -> Expr {
+    Expr::Function {
+        func: super::FunctionExpr::List(ListExpr::Lengths),
+        inputs: vec![input.clone()],
+    }
+}
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/mod.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/numeric/abs.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/numeric/abs.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/numeric/mod.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/numeric/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/python/mod.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/python/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/python/partial_udf.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/python/partial_udf.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/python/udf.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/python/udf.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/temporal/day.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/temporal/day.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/temporal/day_of_week.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/temporal/day_of_week.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/temporal/mod.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/temporal/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/temporal/month.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/temporal/month.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/temporal/year.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/temporal/year.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/uri/download.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/uri/download.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/uri/mod.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/uri/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/utf8/contains.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/utf8/contains.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/utf8/endswith.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/utf8/endswith.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/utf8/length.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/utf8/length.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/utf8/mod.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/utf8/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/functions/utf8/startswith.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/functions/utf8/startswith.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/lib.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/lib.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/lit.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/lit.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/optimization.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/optimization.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/pyobject.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/pyobject.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-dsl/src/python.rs` & `getdaft-0.1.9/local_dependencies/daft-dsl/src/python.rs`

 * *Files 1% similar despite different names*

```diff
@@ -334,19 +334,29 @@
                 "height can not be negative: {h}"
             )));
         }
         use crate::functions::image::resize;
         Ok(resize(&self.expr, w as u32, h as u32).into())
     }
 
+    pub fn image_crop(&self, bbox: &Self) -> PyResult<Self> {
+        use crate::functions::image::crop;
+        Ok(crop(&self.expr, &bbox.expr).into())
+    }
+
     pub fn list_join(&self, delimiter: &Self) -> PyResult<Self> {
         use crate::functions::list::join;
         Ok(join(&self.expr, &delimiter.expr).into())
     }
 
+    pub fn list_lengths(&self) -> PyResult<Self> {
+        use crate::functions::list::lengths;
+        Ok(lengths(&self.expr).into())
+    }
+
     pub fn url_download(
         &self,
         max_connections: i64,
         raise_error_on_failure: bool,
         multi_thread: bool,
         config: Option<PyIOConfig>,
     ) -> PyResult<Self> {
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/from.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/from.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/iterator.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/iterator.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/mod.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/apply.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/apply.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arange.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/arange.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arithmetic.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/arithmetic.rs`

 * *Files 12% similar despite different names*

```diff
@@ -73,14 +73,15 @@
         ))),
     }
 }
 
 impl<T> Add for &DataArray<T>
 where
     T: DaftNumericType,
+    T::Native: basic::NativeArithmetics,
 {
     type Output = DaftResult<DataArray<T>>;
     fn add(self, rhs: Self) -> Self::Output {
         arithmetic_helper(self, rhs, basic::add, |l, r| l + r)
     }
 }
 
@@ -90,24 +91,26 @@
         let result = Box::new(add_utf8_arrays(self.as_arrow(), rhs.as_arrow())?);
         Ok(Utf8Array::from((self.name(), result)))
     }
 }
 impl<T> Sub for &DataArray<T>
 where
     T: DaftNumericType,
+    T::Native: basic::NativeArithmetics,
 {
     type Output = DaftResult<DataArray<T>>;
     fn sub(self, rhs: Self) -> Self::Output {
         arithmetic_helper(self, rhs, basic::sub, |l, r| l - r)
     }
 }
 
 impl<T> Mul for &DataArray<T>
 where
     T: DaftNumericType,
+    T::Native: basic::NativeArithmetics,
 {
     type Output = DaftResult<DataArray<T>>;
     fn mul(self, rhs: Self) -> Self::Output {
         arithmetic_helper(self, rhs, basic::mul, |l, r| l * r)
     }
 }
 
@@ -144,14 +147,15 @@
 {
     binary_with_nulls(lhs, rhs, |a, b| a % b)
 }
 
 impl<T> Rem for &DataArray<T>
 where
     T: DaftNumericType,
+    T::Native: basic::NativeArithmetics,
 {
     type Output = DaftResult<DataArray<T>>;
     fn rem(self, rhs: Self) -> Self::Output {
         if rhs.data().null_count() == 0 {
             arithmetic_helper(self, rhs, basic::rem, |l, r| l % r)
         } else {
             match (self.len(), rhs.len()) {
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arrow2/comparison.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/arrow2/comparison.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/common.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/common.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/indices.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/indices.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/sort.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/arrow2/sort/primitive/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/as_arrow.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/as_arrow.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 use arrow2;
 use arrow2::array;
 
 use crate::{
     array::DataArray,
     datatypes::{
         logical::{
-            DateArray, DurationArray, EmbeddingArray, FixedShapeImageArray, ImageArray,
-            TimestampArray,
+            DateArray, Decimal128Array, DurationArray, EmbeddingArray, FixedShapeImageArray,
+            FixedShapeTensorArray, ImageArray, TensorArray, TimestampArray,
         },
         BinaryArray, BooleanArray, DaftNumericType, FixedSizeListArray, ListArray, StructArray,
         Utf8Array,
     },
 };
 
 #[cfg(feature = "python")]
@@ -65,13 +65,16 @@
 impl_asarrow_dataarray!(ListArray, array::ListArray<i64>);
 impl_asarrow_dataarray!(FixedSizeListArray, array::FixedSizeListArray);
 impl_asarrow_dataarray!(StructArray, array::StructArray);
 
 #[cfg(feature = "python")]
 impl_asarrow_dataarray!(PythonArray, PseudoArrowArray<pyo3::PyObject>);
 
+impl_asarrow_logicalarray!(Decimal128Array, array::PrimitiveArray<i128>);
 impl_asarrow_logicalarray!(DateArray, array::PrimitiveArray<i32>);
 impl_asarrow_logicalarray!(DurationArray, array::PrimitiveArray<i64>);
 impl_asarrow_logicalarray!(TimestampArray, array::PrimitiveArray<i64>);
 impl_asarrow_logicalarray!(EmbeddingArray, array::FixedSizeListArray);
 impl_asarrow_logicalarray!(ImageArray, array::StructArray);
 impl_asarrow_logicalarray!(FixedShapeImageArray, array::FixedSizeListArray);
+impl_asarrow_logicalarray!(TensorArray, array::StructArray);
+impl_asarrow_logicalarray!(FixedShapeTensorArray, array::FixedSizeListArray);
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/broadcast.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/broadcast.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/compare_agg.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/compare_agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/comparison.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/comparison.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/concat.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/concat.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/concat_agg.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/concat_agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/count.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/count.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/date.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/date.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/filter.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/filter.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/float.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/float.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/full.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/full.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/get.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/get.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use crate::{
     array::DataArray,
     datatypes::{
         logical::{
-            DateArray, DurationArray, EmbeddingArray, FixedShapeImageArray, ImageArray,
-            TimestampArray,
+            DateArray, Decimal128Array, DurationArray, EmbeddingArray, FixedShapeImageArray,
+            ImageArray, TimestampArray,
         },
         BinaryArray, BooleanArray, DaftNumericType, ExtensionArray, FixedSizeListArray, ListArray,
         NullArray, StructArray, Utf8Array,
     },
 };
 
 use super::as_arrow::AsArrow;
@@ -57,14 +57,15 @@
 }
 
 impl_array_get!(Utf8Array, &str);
 impl_array_get!(BooleanArray, bool);
 impl_array_get!(BinaryArray, &[u8]);
 impl_array_get!(ListArray, Box<dyn arrow2::array::Array>);
 impl_array_get!(FixedSizeListArray, Box<dyn arrow2::array::Array>);
+impl_array_get!(Decimal128Array, i128);
 impl_array_get!(DateArray, i32);
 impl_array_get!(DurationArray, i64);
 impl_array_get!(TimestampArray, i64);
 impl_array_get!(EmbeddingArray, Box<dyn arrow2::array::Array>);
 impl_array_get!(FixedShapeImageArray, Box<dyn arrow2::array::Array>);
 
 impl NullArray {
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/groups.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/groups.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/hash.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/hash.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/if_else.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/if_else.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use crate::array::DataArray;
 use crate::datatypes::logical::{
-    DateArray, DurationArray, EmbeddingArray, FixedShapeImageArray, ImageArray, TimestampArray,
+    DateArray, Decimal128Array, DurationArray, EmbeddingArray, FixedShapeImageArray,
+    FixedShapeTensorArray, ImageArray, TensorArray, TimestampArray,
 };
 use crate::datatypes::{
     BinaryArray, BooleanArray, DaftArrowBackedType, DaftNumericType, ExtensionArray, Field,
     FixedSizeListArray, ListArray, NullArray, StructArray, Utf8Array,
 };
 use crate::utils::arrow::arrow_bitmap_and_helper;
 use common_error::{DaftError, DaftResult};
@@ -330,13 +331,16 @@
                 let new_array = self.physical.if_else(&other.physical, predicate)?;
                 Ok(Self::new(self.field.clone(), new_array))
             }
         }
     };
 }
 
+impl_logicalarray_if_else!(Decimal128Array);
 impl_logicalarray_if_else!(DateArray);
 impl_logicalarray_if_else!(DurationArray);
 impl_logicalarray_if_else!(TimestampArray);
 impl_logicalarray_if_else!(EmbeddingArray);
 impl_logicalarray_if_else!(ImageArray);
 impl_logicalarray_if_else!(FixedShapeImageArray);
+impl_logicalarray_if_else!(TensorArray);
+impl_logicalarray_if_else!(FixedShapeTensorArray);
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/image.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/image.rs`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,34 @@
 use image::{Luma, LumaA, Rgb, Rgba};
 
 use super::as_arrow::AsArrow;
 use num_traits::FromPrimitive;
 
 use std::ops::Deref;
 
+#[derive(Clone)]
+pub struct BBox(u32, u32, u32, u32);
+
+impl BBox {
+    pub fn from_u32_arrow_array(arr: Box<dyn arrow2::array::Array>) -> Self {
+        assert!(arr.len() == 4);
+        let mut iter = arr
+            .as_any()
+            .downcast_ref::<arrow2::array::UInt32Array>()
+            .unwrap()
+            .iter();
+        BBox(
+            *iter.next().unwrap().unwrap(),
+            *iter.next().unwrap().unwrap(),
+            *iter.next().unwrap().unwrap(),
+            *iter.next().unwrap().unwrap(),
+        )
+    }
+}
+
 #[allow(clippy::upper_case_acronyms, dead_code)]
 #[derive(Debug)]
 pub enum DaftImageBuffer<'a> {
     L(ImageBuffer<Luma<u8>, Cow<'a, [u8]>>),
     LA(ImageBuffer<LumaA<u8>, Cow<'a, [u8]>>),
     RGB(ImageBuffer<Rgb<u8>, Cow<'a, [u8]>>),
     RGBA(ImageBuffer<Rgba<u8>, Cow<'a, [u8]>>),
@@ -199,14 +219,44 @@
                 let result =
                     image::imageops::resize(imgbuf, w, h, image::imageops::FilterType::Triangle);
                 DaftImageBuffer::RGBA(image_buffer_vec_to_cow(result))
             }
             _ => unimplemented!("Mode {self:?} not implemented"),
         }
     }
+
+    pub fn crop(&self, bbox: &BBox) -> Self {
+        // HACK(jay): The `.to_image()` method on SubImage takes in `'static` references for some reason
+        // This hack will ensure that `&self` adheres to that overly prescriptive bound
+        let inner =
+            unsafe { std::mem::transmute::<&DaftImageBuffer<'a>, &DaftImageBuffer<'static>>(self) };
+        match inner {
+            DaftImageBuffer::L(imgbuf) => {
+                let result =
+                    image::imageops::crop_imm(imgbuf, bbox.0, bbox.1, bbox.2, bbox.3).to_image();
+                DaftImageBuffer::L(image_buffer_vec_to_cow(result))
+            }
+            DaftImageBuffer::LA(imgbuf) => {
+                let result =
+                    image::imageops::crop_imm(imgbuf, bbox.0, bbox.1, bbox.2, bbox.3).to_image();
+                DaftImageBuffer::LA(image_buffer_vec_to_cow(result))
+            }
+            DaftImageBuffer::RGB(imgbuf) => {
+                let result =
+                    image::imageops::crop_imm(imgbuf, bbox.0, bbox.1, bbox.2, bbox.3).to_image();
+                DaftImageBuffer::RGB(image_buffer_vec_to_cow(result))
+            }
+            DaftImageBuffer::RGBA(imgbuf) => {
+                let result =
+                    image::imageops::crop_imm(imgbuf, bbox.0, bbox.1, bbox.2, bbox.3).to_image();
+                DaftImageBuffer::RGBA(image_buffer_vec_to_cow(result))
+            }
+            _ => unimplemented!("Mode {self:?} not implemented"),
+        }
+    }
 }
 
 fn image_buffer_vec_to_cow<'a, P, T>(input: ImageBuffer<P, Vec<T>>) -> ImageBuffer<P, Cow<'a, [T]>>
 where
     P: image::Pixel<Subpixel = T>,
     Vec<T>: Deref<Target = [P::Subpixel]>,
     T: ToOwned + std::clone::Clone,
@@ -252,21 +302,19 @@
                 DaftImageBuffer::<'a>::RGBA32F(image_buffer_vec_to_cow(img_buf))
             }
             _ => unimplemented!("{dyn_img:?} not implemented"),
         }
     }
 }
 
-pub struct ImageArrayVecs<T> {
-    pub data: Vec<T>,
+pub struct ImageArraySidecarData {
     pub channels: Vec<u16>,
     pub heights: Vec<u32>,
     pub widths: Vec<u32>,
     pub modes: Vec<u8>,
-    pub offsets: Vec<i64>,
     pub validity: Option<arrow2::bitmap::Bitmap>,
 }
 
 pub trait AsImageObj {
     fn as_image_obj(&self, idx: usize) -> Option<DaftImageBuffer<'_>>;
 }
 
@@ -350,70 +398,83 @@
         let array = p.values().get(IMAGE_MODE_IDX).unwrap();
         array.as_ref().as_any().downcast_ref().unwrap()
     }
 
     pub fn from_vecs<T: arrow2::types::NativeType>(
         name: &str,
         data_type: DataType,
-        vecs: ImageArrayVecs<T>,
+        data: Vec<T>,
+        offsets: Vec<i64>,
+        sidecar_data: ImageArraySidecarData,
     ) -> DaftResult<Self> {
-        if vecs.data.is_empty() {
+        if data.is_empty() {
             // Create an all-null array if the data array is empty.
             let physical_type = data_type.to_physical();
-            let null_struct_array =
-                arrow2::array::new_null_array(physical_type.to_arrow()?, vecs.channels.len());
+            let null_struct_array = arrow2::array::new_null_array(
+                physical_type.to_arrow()?,
+                sidecar_data.channels.len(),
+            );
             let daft_struct_array =
                 StructArray::new(Field::new(name, physical_type).into(), null_struct_array)?;
             return Ok(ImageArray::new(
                 Field::new(name, data_type),
                 daft_struct_array,
             ));
         }
-        let offsets = arrow2::offset::OffsetsBuffer::try_from(vecs.offsets)?;
+        let offsets = arrow2::offset::OffsetsBuffer::try_from(offsets)?;
         let arrow_dtype: arrow2::datatypes::DataType = T::PRIMITIVE.into();
         if let DataType::Image(Some(mode)) = &data_type {
             if mode.get_dtype().to_arrow()? != arrow_dtype {
                 panic!("Inner value dtype of provided dtype {data_type:?} is inconsistent with inferred value dtype {arrow_dtype:?}");
             }
         }
 
         let list_datatype = arrow2::datatypes::DataType::LargeList(Box::new(
             arrow2::datatypes::Field::new("data", arrow_dtype, true),
         ));
         let data_array = Box::new(arrow2::array::ListArray::<i64>::new(
             list_datatype,
             offsets,
-            Box::new(arrow2::array::PrimitiveArray::from_vec(vecs.data)),
-            vecs.validity.clone(),
+            Box::new(arrow2::array::PrimitiveArray::from_vec(data)),
+            sidecar_data.validity.clone(),
         ));
 
+        Self::from_list_array(name, data_type, data_array, sidecar_data)
+    }
+
+    pub fn from_list_array(
+        name: &str,
+        data_type: DataType,
+        data_array: Box<arrow2::array::ListArray<i64>>,
+        sidecar_data: ImageArraySidecarData,
+    ) -> DaftResult<Self> {
         let values: Vec<Box<dyn arrow2::array::Array>> = vec![
             data_array,
             Box::new(
-                arrow2::array::UInt16Array::from_vec(vecs.channels)
-                    .with_validity(vecs.validity.clone()),
+                arrow2::array::UInt16Array::from_vec(sidecar_data.channels)
+                    .with_validity(sidecar_data.validity.clone()),
             ),
             Box::new(
-                arrow2::array::UInt32Array::from_vec(vecs.heights)
-                    .with_validity(vecs.validity.clone()),
+                arrow2::array::UInt32Array::from_vec(sidecar_data.heights)
+                    .with_validity(sidecar_data.validity.clone()),
             ),
             Box::new(
-                arrow2::array::UInt32Array::from_vec(vecs.widths)
-                    .with_validity(vecs.validity.clone()),
+                arrow2::array::UInt32Array::from_vec(sidecar_data.widths)
+                    .with_validity(sidecar_data.validity.clone()),
             ),
             Box::new(
-                arrow2::array::UInt8Array::from_vec(vecs.modes)
-                    .with_validity(vecs.validity.clone()),
+                arrow2::array::UInt8Array::from_vec(sidecar_data.modes)
+                    .with_validity(sidecar_data.validity.clone()),
             ),
         ];
         let physical_type = data_type.to_physical();
         let struct_array = Box::new(arrow2::array::StructArray::new(
             physical_type.to_arrow()?,
             values,
-            vecs.validity,
+            sidecar_data.validity,
         ));
 
         let daft_struct_array = crate::datatypes::StructArray::new(
             Field::new(name, physical_type).into(),
             struct_array,
         )?;
         Ok(ImageArray::new(
@@ -427,14 +488,34 @@
     }
 
     pub fn resize(&self, w: u32, h: u32) -> DaftResult<Self> {
         let result = resize_images(self, w, h);
         Self::from_daft_image_buffers(self.name(), result.as_slice(), self.image_mode())
     }
 
+    pub fn crop(&self, bboxes: &FixedSizeListArray) -> DaftResult<ImageArray> {
+        let mut bboxes_iterator: Box<dyn Iterator<Item = Option<BBox>>> = if bboxes.len() == 1 {
+            Box::new(std::iter::repeat(
+                bboxes
+                    .as_arrow()
+                    .get(0)
+                    .map(|bbox| BBox::from_u32_arrow_array(bbox)),
+            ))
+        } else {
+            Box::new(
+                bboxes
+                    .as_arrow()
+                    .iter()
+                    .map(|bbox| bbox.map(|bbox| BBox::from_u32_arrow_array(bbox))),
+            )
+        };
+        let result = crop_images(self, &mut bboxes_iterator);
+        Self::from_daft_image_buffers(self.name(), result.as_slice(), self.image_mode())
+    }
+
     pub fn resize_to_fixed_shape_image_array(
         &self,
         w: u32,
         h: u32,
         mode: &ImageMode,
     ) -> DaftResult<FixedShapeImageArray> {
         let result = resize_images(self, w, h);
@@ -480,21 +561,21 @@
         let validity: Option<arrow2::bitmap::Bitmap> = match validity.unset_bits() {
             0 => None,
             _ => Some(validity.into()),
         };
         Self::from_vecs(
             name,
             DataType::Image(*image_mode),
-            ImageArrayVecs {
-                data,
+            data,
+            offsets,
+            ImageArraySidecarData {
                 channels,
                 heights,
                 widths,
                 modes,
-                offsets,
                 validity,
             },
         )
     }
 }
 
 impl AsImageObj for ImageArray {
@@ -547,14 +628,21 @@
         assert_eq!(result.height(), h);
         assert_eq!(result.width(), w);
         Some(result)
     }
 }
 
 impl FixedShapeImageArray {
+    fn mode(&self) -> ImageMode {
+        match &self.field.dtype {
+            DataType::FixedShapeImage(mode, _, _) => *mode,
+            _ => panic!("FixedShapeImageArray does not have the correct FixedShapeImage dtype"),
+        }
+    }
+
     pub fn from_daft_image_buffers(
         name: &str,
         inputs: &[Option<DaftImageBuffer<'_>>],
         image_mode: &ImageMode,
         height: u32,
         width: u32,
     ) -> DaftResult<Self> {
@@ -612,14 +700,34 @@
     pub fn resize(&self, w: u32, h: u32) -> DaftResult<Self> {
         let result = resize_images(self, w, h);
         match self.logical_type() {
             DataType::FixedShapeImage(mode, _, _) => Self::from_daft_image_buffers(self.name(), result.as_slice(), mode, h, w),
             dt => panic!("FixedShapeImageArray should always have DataType::FixedShapeImage() as it's dtype, but got {}", dt),
         }
     }
+
+    pub fn crop(&self, bboxes: &FixedSizeListArray) -> DaftResult<ImageArray> {
+        let mut bboxes_iterator: Box<dyn Iterator<Item = Option<BBox>>> = if bboxes.len() == 1 {
+            Box::new(std::iter::repeat(
+                bboxes
+                    .as_arrow()
+                    .get(0)
+                    .map(|bbox| BBox::from_u32_arrow_array(bbox)),
+            ))
+        } else {
+            Box::new(
+                bboxes
+                    .as_arrow()
+                    .iter()
+                    .map(|bbox| bbox.map(|bbox| BBox::from_u32_arrow_array(bbox))),
+            )
+        };
+        let result = crop_images(self, &mut bboxes_iterator);
+        ImageArray::from_daft_image_buffers(self.name(), result.as_slice(), &Some(self.mode()))
+    }
 }
 
 impl AsImageObj for FixedShapeImageArray {
     fn as_image_obj<'a>(&'a self, idx: usize) -> Option<DaftImageBuffer<'a>> {
         assert!(idx < self.len());
         if !self.physical.is_valid(idx) {
             return None;
@@ -811,7 +919,27 @@
         IntoIterator<Item = Option<DaftImageBuffer<'a>>, IntoIter = ImageBufferIter<'a, T>>,
 {
     images
         .into_iter()
         .map(|img| img.map(|img| img.resize(w, h)))
         .collect::<Vec<_>>()
 }
+
+fn crop_images<'a, T>(
+    images: &'a LogicalArray<T>,
+    bboxes: &mut dyn Iterator<Item = Option<BBox>>,
+) -> Vec<Option<DaftImageBuffer<'a>>>
+where
+    T: DaftImageryType,
+    LogicalArray<T>: AsImageObj,
+    &'a LogicalArray<T>:
+        IntoIterator<Item = Option<DaftImageBuffer<'a>>, IntoIter = ImageBufferIter<'a, T>>,
+{
+    images
+        .into_iter()
+        .zip(bboxes)
+        .map(|(img, bbox)| match (img, bbox) {
+            (None, _) | (_, None) => None,
+            (Some(img), Some(bbox)) => Some(img.crop(&bbox)),
+        })
+        .collect::<Vec<_>>()
+}
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/len.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/len.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/list.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/list.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/list_agg.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/list_agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/mean.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/mean.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/mod.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 mod null;
 mod pairwise;
 mod repr;
 mod search_sorted;
 mod sort;
 mod sum;
 mod take;
+pub(crate) mod tensor;
 mod utf8;
 
 pub use sort::{build_multi_array_bicompare, build_multi_array_compare};
 
 use common_error::DaftResult;
 
 pub trait DaftCompare<Rhs> {
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/null.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/null.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/pairwise.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/pairwise.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/repr.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/repr.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use base64::Engine;
 
 use crate::{
     array::DataArray,
     datatypes::{
         logical::{
-            DateArray, DurationArray, EmbeddingArray, FixedShapeImageArray, ImageArray,
-            TimestampArray,
+            DateArray, Decimal128Array, DurationArray, EmbeddingArray, FixedShapeImageArray,
+            ImageArray, TimestampArray,
         },
         BinaryArray, BooleanArray, DaftNumericType, ExtensionArray, FixedSizeListArray,
         ImageFormat, ListArray, NullArray, StructArray, Utf8Array,
     },
 };
 use common_error::DaftResult;
 
@@ -184,14 +184,29 @@
                 )
             }
         );
         Ok(res)
     }
 }
 
+impl Decimal128Array {
+    pub fn str_value(&self, idx: usize) -> DaftResult<String> {
+        let res = self.get(idx).map_or_else(
+            || "None".to_string(),
+            |val| -> String {
+                use crate::array::ops::cast::decimal128_to_str;
+                use crate::datatypes::DataType::Decimal128;
+                let Decimal128(precision, scale) = &self.field.dtype else { panic!("Wrong dtype for Decimal128Array: {}", self.field.dtype) };
+                decimal128_to_str(val, *precision as u8, *scale as i8)
+            }
+        );
+        Ok(res)
+    }
+}
+
 // Default implementation of html_value: html escape the str_value.
 macro_rules! impl_array_html_value {
     ($ArrayT:ty) => {
         impl $ArrayT {
             pub fn html_value(&self, idx: usize) -> String {
                 let str_value = self.str_value(idx).unwrap();
                 html_escape::encode_text(&str_value)
@@ -206,14 +221,15 @@
 impl_array_html_value!(BooleanArray);
 impl_array_html_value!(NullArray);
 impl_array_html_value!(BinaryArray);
 impl_array_html_value!(ListArray);
 impl_array_html_value!(FixedSizeListArray);
 impl_array_html_value!(StructArray);
 impl_array_html_value!(ExtensionArray);
+impl_array_html_value!(Decimal128Array);
 impl_array_html_value!(DateArray);
 impl_array_html_value!(DurationArray);
 impl_array_html_value!(TimestampArray);
 impl_array_html_value!(EmbeddingArray);
 
 #[cfg(feature = "python")]
 impl crate::datatypes::PythonArray {
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/sort.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/sort.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use crate::{
     array::DataArray,
     datatypes::{
         logical::{
-            DateArray, DurationArray, EmbeddingArray, FixedShapeImageArray, ImageArray,
-            TimestampArray,
+            DateArray, Decimal128Array, DurationArray, EmbeddingArray, FixedShapeImageArray,
+            FixedShapeTensorArray, ImageArray, TensorArray, TimestampArray,
         },
         BinaryArray, BooleanArray, DaftIntegerType, DaftNumericType, ExtensionArray,
         FixedSizeListArray, Float32Array, Float64Array, ListArray, NullArray, StructArray,
         Utf8Array,
     },
     kernels::search_sorted::{build_compare_with_nulls, cmp_float},
     series::Series,
@@ -59,15 +59,15 @@
     });
     Ok(combined_comparator)
 }
 
 impl<T> DataArray<T>
 where
     T: DaftIntegerType,
-    <T as DaftNumericType>::Native: arrow2::types::Index,
+    <T as DaftNumericType>::Native: Ord,
 {
     pub fn argsort<I>(&self, descending: bool) -> DaftResult<DataArray<I>>
     where
         I: DaftIntegerType,
         <I as DaftNumericType>::Native: arrow2::types::Index,
     {
         let arrow_array = self.as_arrow();
@@ -590,14 +590,21 @@
 #[cfg(feature = "python")]
 impl PythonArray {
     pub fn sort(&self, _descending: bool) -> DaftResult<Self> {
         todo!("impl sort for python array")
     }
 }
 
+impl Decimal128Array {
+    pub fn sort(&self, descending: bool) -> DaftResult<Self> {
+        let new_array = self.physical.sort(descending)?;
+        Ok(Self::new(self.field.clone(), new_array))
+    }
+}
+
 impl DateArray {
     pub fn sort(&self, descending: bool) -> DaftResult<Self> {
         let new_array = self.physical.sort(descending)?;
         Ok(Self::new(self.field.clone(), new_array))
     }
 }
 
@@ -628,7 +635,19 @@
 }
 
 impl FixedShapeImageArray {
     pub fn sort(&self, _descending: bool) -> DaftResult<Self> {
         todo!("impl sort for FixedShapeImageArray")
     }
 }
+
+impl TensorArray {
+    pub fn sort(&self, _descending: bool) -> DaftResult<Self> {
+        todo!("impl sort for TensorArray")
+    }
+}
+
+impl FixedShapeTensorArray {
+    pub fn sort(&self, _descending: bool) -> DaftResult<Self> {
+        todo!("impl sort for FixedShapeTensorArray")
+    }
+}
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/sum.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/sum.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/ops/utf8.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/ops/utf8.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/pseudo_arrow/compute.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/pseudo_arrow/compute.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/pseudo_arrow/mod.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/pseudo_arrow/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/array/pseudo_arrow/python.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/array/pseudo_arrow/python.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/binary_ops.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/utils/supertype.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,220 +1,234 @@
-use std::ops::{Add, Div, Mul, Rem, Sub};
-
-use common_error::{DaftError, DaftResult};
-
-use crate::impl_binary_trait_by_reference;
-
-use super::DataType;
-
-impl Add for &DataType {
-    type Output = DaftResult<DataType>;
-
-    fn add(self, other: Self) -> Self::Output {
-        use DataType::*;
-        try_numeric_supertype(self, other).or(
-            match (self, other) {
-                #[cfg(feature = "python")]
-                (Python, _) | (_, Python) => Ok(Python),
-                (Timestamp(t_unit, tz), Duration(d_unit))
-                | (Duration(d_unit), Timestamp(t_unit, tz))
-                    if t_unit == d_unit => Ok(Timestamp(*t_unit, tz.clone())),
-                (ts @ Timestamp(..), du @ Duration(..))
-                | (du @ Duration(..), ts @ Timestamp(..)) => Err(DaftError::TypeError(
-                    format!("Cannot add due to differing precision: {}, {}. Please explicitly cast to the precision you wish to add in.", ts, du)
-                )),
-                (Null, other) | (other, Null) => {
-                    match other {
-                        // Condition is for backwards compatibility. TODO: remove
-                        Binary | Date => Err(DaftError::TypeError(
-                            format!("Cannot add types: {}, {}", self, other)
-                        )),
-                        other if other.is_physical() => Ok(other.clone()),
-                        _ => Err(DaftError::TypeError(
-                            format!("Cannot add types: {}, {}", self, other)
-                        )),
-                    }
-                }
-                (Utf8, other) | (other, Utf8) => {
-                    match other {
-                        // Date condition is for backwards compatibility. TODO: remove
-                        Binary | Date => Err(DaftError::TypeError(
-                            format!("Cannot add types: {}, {}", self, other)
-                        )),
-                        other if other.is_physical() => Ok(Utf8),
-                        _ => Err(DaftError::TypeError(
-                            format!("Cannot add types: {}, {}", self, other)
-                        )),
-                    }
-                }
-                (Boolean, other) | (other, Boolean)
-                    if other.is_numeric() => Ok(other.clone()),
-                _ => Err(DaftError::TypeError(
-                    format!("Cannot add types: {}, {}", self, other)
-                ))
-            }
-        )
+use crate::datatypes::DataType;
+use crate::datatypes::Field;
+use crate::datatypes::TimeUnit;
+use common_error::DaftError;
+use common_error::DaftResult;
+
+/// Largely influenced by polars supertype logic which is based on numpy / python type propagation
+// Copyright (c) 2020 Ritchie Vink
+// Permission is hereby granted, free of charge, to any person obtaining a copy
+// of this software and associated documentation files (the "Software"), to deal
+// in the Software without restriction, including without limitation the rights
+// to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+// copies of the Software, and to permit persons to whom the Software is
+// furnished to do so, subject to the following conditions:
+
+// The above copyright notice and this permission notice shall be included in all
+// copies or substantial portions of the Software.
+
+// THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+// IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+// FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+// AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+// LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+// OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+// SOFTWARE.
+
+fn get_time_units(tu_l: &TimeUnit, tu_r: &TimeUnit) -> TimeUnit {
+    use TimeUnit::*;
+    match (tu_l, tu_r) {
+        (Nanoseconds, Microseconds) => Microseconds,
+        (_, Milliseconds) => Milliseconds,
+        _ => *tu_l,
     }
 }
 
-impl Sub for &DataType {
-    type Output = DaftResult<DataType>;
-
-    fn sub(self, other: Self) -> Self::Output {
-        use DataType::*;
-        try_numeric_supertype(self, other).or(
-            match (self, other) {
-                #[cfg(feature = "python")]
-                (Python, _) | (_, Python) => Ok(Python),
-                (Timestamp(t_unit, tz), Duration(d_unit))
-                    if t_unit == d_unit => Ok(Timestamp(*t_unit, tz.clone())),
-                (ts @ Timestamp(..), du @ Duration(..)) => Err(DaftError::TypeError(
-                    format!("Cannot subtract due to differing precision: {}, {}. Please explicitly cast to the precision you wish to add in.", ts, du)
-                )),
-                _ => Err(DaftError::TypeError(
-                    format!("Cannot subtract types: {}, {}", self, other)
-                ))
-            }
-        )
+pub fn try_get_supertype(l: &DataType, r: &DataType) -> DaftResult<DataType> {
+    match get_supertype(l, r) {
+        Some(dt) => Ok(dt),
+        None => Err(DaftError::TypeError(format!(
+            "could not determine supertype of {l:?} and {r:?}"
+        ))),
     }
 }
 
-impl Div for &DataType {
-    type Output = DaftResult<DataType>;
-
-    fn div(self, other: Self) -> Self::Output {
-        use DataType::*;
-        match (self, other) {
-            #[cfg(feature = "python")]
-            (Python, _) | (_, Python) => Ok(Python),
-            (s, o) if s.is_numeric() && o.is_numeric() => Ok(Float64),
-            _ => Err(DaftError::TypeError(format!(
-                "Cannot divide types: {}, {}",
-                self, other
-            ))),
-        }
-    }
-}
-
-impl Mul for &DataType {
-    type Output = DaftResult<DataType>;
-
-    fn mul(self, other: Self) -> Self::Output {
+pub fn get_supertype(l: &DataType, r: &DataType) -> Option<DataType> {
+    fn inner(l: &DataType, r: &DataType) -> Option<DataType> {
         use DataType::*;
-        try_numeric_supertype(self, other).or(match (self, other) {
-            #[cfg(feature = "python")]
-            (Python, _) | (_, Python) => Ok(Python),
-            _ => Err(DaftError::TypeError(format!(
-                "Cannot multiply types: {}, {}",
-                self, other
-            ))),
-        })
-    }
-}
 
-impl Rem for &DataType {
-    type Output = DaftResult<DataType>;
+        if l == r {
+            return Some(l.clone());
+        }
 
-    fn rem(self, other: Self) -> Self::Output {
-        use DataType::*;
-        try_numeric_supertype(self, other).or(match (self, other) {
+        match (l, r) {
             #[cfg(feature = "python")]
-            (Python, _) | (_, Python) => Ok(Python),
-            _ => Err(DaftError::TypeError(format!(
-                "Cannot multiply types: {}, {}",
-                self, other
-            ))),
-        })
-    }
-}
+            // The supertype of anything and Python is Python.
+            (_, Python) => Some(Python),
 
-impl_binary_trait_by_reference!(DataType, Add, add);
-impl_binary_trait_by_reference!(DataType, Sub, sub);
-impl_binary_trait_by_reference!(DataType, Mul, mul);
-impl_binary_trait_by_reference!(DataType, Div, div);
-impl_binary_trait_by_reference!(DataType, Rem, rem);
-
-pub fn try_numeric_supertype(l: &DataType, r: &DataType) -> DaftResult<DataType> {
-    // If given two numeric data types,
-    // get the numeric type that they should both be casted to
-    // for the purpose of performing numeric operations.
-
-    fn inner(l: &DataType, r: &DataType) -> Option<DataType> {
-        use DataType::*;
-
-        match (l, r) {
-            (Int8, Int8) => Some(Int8),
+            (Int8, Boolean) => Some(Int8),
             (Int8, Int16) => Some(Int16),
             (Int8, Int32) => Some(Int32),
             (Int8, Int64) => Some(Int64),
             (Int8, UInt8) => Some(Int16),
             (Int8, UInt16) => Some(Int32),
             (Int8, UInt32) => Some(Int64),
             (Int8, UInt64) => Some(Float64), // Follow numpy
             (Int8, Float32) => Some(Float32),
             (Int8, Float64) => Some(Float64),
 
-            (Int16, Int16) => Some(Int16),
+            (Int16, Boolean) => Some(Int16),
+            (Int16, Int8) => Some(Int16),
             (Int16, Int32) => Some(Int32),
             (Int16, Int64) => Some(Int64),
             (Int16, UInt8) => Some(Int16),
             (Int16, UInt16) => Some(Int32),
             (Int16, UInt32) => Some(Int64),
             (Int16, UInt64) => Some(Float64), // Follow numpy
             (Int16, Float32) => Some(Float32),
             (Int16, Float64) => Some(Float64),
 
-            (Int32, Int32) => Some(Int32),
+            (Int32, Boolean) => Some(Int32),
+            (Int32, Int8) => Some(Int32),
+            (Int32, Int16) => Some(Int32),
             (Int32, Int64) => Some(Int64),
             (Int32, UInt8) => Some(Int32),
             (Int32, UInt16) => Some(Int32),
             (Int32, UInt32) => Some(Int64),
             (Int32, UInt64) => Some(Float64),  // Follow numpy
             (Int32, Float32) => Some(Float64), // Follow numpy
             (Int32, Float64) => Some(Float64),
 
-            (Int64, Int64) => Some(Int64),
+            (Int64, Boolean) => Some(Int64),
+            (Int64, Int8) => Some(Int64),
+            (Int64, Int16) => Some(Int64),
+            (Int64, Int32) => Some(Int64),
             (Int64, UInt8) => Some(Int64),
             (Int64, UInt16) => Some(Int64),
             (Int64, UInt32) => Some(Int64),
             (Int64, UInt64) => Some(Float64),  // Follow numpy
             (Int64, Float32) => Some(Float64), // Follow numpy
             (Int64, Float64) => Some(Float64),
 
-            (UInt8, UInt8) => Some(UInt8),
-            (UInt8, UInt16) => Some(UInt16),
-            (UInt8, UInt32) => Some(UInt32),
-            (UInt8, UInt64) => Some(UInt64),
-            (UInt8, Float32) => Some(Float32),
-            (UInt8, Float64) => Some(Float64),
-
-            (UInt16, UInt16) => Some(UInt16),
+            (UInt16, UInt8) => Some(UInt16),
             (UInt16, UInt32) => Some(UInt32),
             (UInt16, UInt64) => Some(UInt64),
-            (UInt16, Float32) => Some(Float32),
-            (UInt16, Float64) => Some(Float64),
 
-            (UInt32, UInt32) => Some(UInt32),
+            (UInt8, UInt32) => Some(UInt32),
+            (UInt8, UInt64) => Some(UInt64),
             (UInt32, UInt64) => Some(UInt64),
-            (UInt32, Float32) => Some(Float64),
-            (UInt32, Float64) => Some(Float64),
 
-            (UInt64, UInt64) => Some(UInt64),
-            (UInt64, Float32) => Some(Float64),
-            (UInt64, Float64) => Some(Float64),
+            (Boolean, UInt8) => Some(UInt8),
+            (Boolean, UInt16) => Some(UInt16),
+            (Boolean, UInt32) => Some(UInt32),
+            (Boolean, UInt64) => Some(UInt64),
+
+            (Float32, UInt8) => Some(Float32),
+            (Float32, UInt16) => Some(Float32),
+            (Float32, UInt32) => Some(Float64),
+            (Float32, UInt64) => Some(Float64),
+
+            (Float64, UInt8) => Some(Float64),
+            (Float64, UInt16) => Some(Float64),
+            (Float64, UInt32) => Some(Float64),
+            (Float64, UInt64) => Some(Float64),
+
+            (Float64, Float32) => Some(Float64),
+
+            (Date, UInt8) => Some(Int64),
+            (Date, UInt16) => Some(Int64),
+            (Date, UInt32) => Some(Int64),
+            (Date, UInt64) => Some(Int64),
+            (Date, Int8) => Some(Int32),
+            (Date, Int16) => Some(Int32),
+            (Date, Int32) => Some(Int32),
+            (Date, Int64) => Some(Int64),
+            (Date, Float32) => Some(Float32),
+            (Date, Float64) => Some(Float64),
+            (Date, Timestamp(tu, tz)) => Some(Timestamp(*tu, tz.clone())),
+
+            (Timestamp(_, _), UInt32) => Some(Int64),
+            (Timestamp(_, _), UInt64) => Some(Int64),
+            (Timestamp(_, _), Int32) => Some(Int64),
+            (Timestamp(_, _), Int64) => Some(Int64),
+            (Timestamp(_, _), Float32) => Some(Float64),
+            (Timestamp(_, _), Float64) => Some(Float64),
+            (Timestamp(tu, tz), Date) => Some(Timestamp(*tu, tz.clone())),
+
+            (Duration(_), UInt32) => Some(Int64),
+            (Duration(_), UInt64) => Some(Int64),
+            (Duration(_), Int32) => Some(Int64),
+            (Duration(_), Int64) => Some(Int64),
+            (Duration(_), Float32) => Some(Float64),
+            (Duration(_), Float64) => Some(Float64),
+
+            (Time(_), Int32) => Some(Int64),
+            (Time(_), Int64) => Some(Int64),
+            (Time(_), Float32) => Some(Float64),
+            (Time(_), Float64) => Some(Float64),
+
+            (Duration(lu), Timestamp(ru, Some(tz))) | (Timestamp(lu, Some(tz)), Duration(ru)) => {
+                if tz.is_empty() {
+                    Some(Timestamp(get_time_units(lu, ru), None))
+                } else {
+                    Some(Timestamp(get_time_units(lu, ru), Some(tz.clone())))
+                }
+            }
+            (Duration(lu), Timestamp(ru, None)) | (Timestamp(lu, None), Duration(ru)) => {
+                Some(Timestamp(get_time_units(lu, ru), None))
+            }
+            (Duration(_), Date) | (Date, Duration(_)) => Some(Date),
+            (Duration(lu), Duration(ru)) => Some(Duration(get_time_units(lu, ru))),
+
+            // None and Some("") timezones
+            // we cast from more precision to higher precision as that always fits with occasional loss of precision
+            (Timestamp(tu_l, tz_l), Timestamp(tu_r, tz_r))
+                if (tz_l.is_none() || tz_l.as_deref() == Some(""))
+                    && (tz_r.is_none() || tz_r.as_deref() == Some("")) =>
+            {
+                let tu = get_time_units(tu_l, tu_r);
+                Some(Timestamp(tu, None))
+            }
+            // None and Some("<tz>") timezones
+            // we cast from more precision to higher precision as that always fits with occasional loss of precision
+            (Timestamp(tu_l, tz_l), Timestamp(tu_r, tz_r)) if
+                // both are none
+                tz_l.is_none() && tz_r.is_some()
+                // both have the same time zone
+                || (tz_l.is_some() && (tz_l == tz_r)) => {
+                let tu = get_time_units(tu_l, tu_r);
+                Some(Timestamp(tu, tz_r.clone()))
+            }
 
-            (Float32, Float32) => Some(Float32),
-            (Float32, Float64) => Some(Float64),
+            //TODO(sammy): add time, struct related dtypes
+            (Boolean, Float32) => Some(Float32),
+            (Boolean, Float64) => Some(Float64),
+            (List(inner_left_field), List(inner_right_field)) => {
+                let inner_st = get_supertype(&inner_left_field.dtype, &inner_right_field.dtype)?;
+                Some(DataType::List(Box::new(Field::new(inner_left_field.name.clone(), inner_st))))
+            }
+            // TODO(Clark): Add support for getting supertype for two fixed size lists once Arrow2 supports such a cast.
+            // (FixedSizeList(inner_left_field, inner_left_size), FixedSizeList(inner_right_field, inner_right_size)) if inner_left_size == inner_right_size => {
+            //     let inner_st = inner(&inner_left_field.dtype, &inner_right_field.dtype)?;
+            //     Some(DataType::FixedSizeList(Box::new(Field::new(inner_left_field.name.clone(), inner_st)), *inner_left_size))
+            // }
+            // TODO(Clark): Add support for getting supertype for a fixed size list and a list once Arrow2 supports such a cast.
+            // (FixedSizeList(inner_left_field, _inner_left_size), List(inner_right_field)) => {
+            //     let inner_st = get_supertype(&inner_left_field.dtype, &inner_right_field.dtype)?;
+            //     Some(DataType::List(Box::new(Field::new(inner_left_field.name.clone(), inner_st))))
+            // }
+
+            // every known type can be casted to a string except binary
+            (dt, Utf8) if dt.ne(&Binary) => Some(Utf8),
+            (dt, Null) => Some(dt.clone()), // Drop Null Type
 
-            (Float64, Float64) => Some(Float64),
 
             _ => None,
         }
     }
+    match inner(l, r) {
+        Some(dt) => Some(dt),
+        None => inner(r, l),
+    }
+}
+
+#[cfg(test)]
+mod tests {
+    use super::*;
 
-    inner(l, r)
-        .or(inner(r, l))
-        .ok_or(DaftError::TypeError(format!(
-            "Invalid arguments to numeric supertype: {}, {}",
-            l, r
-        )))
+    #[test]
+    fn check_bad_arrow_type() -> DaftResult<()> {
+        let result = get_supertype(&DataType::Utf8, &DataType::Binary);
+        assert_eq!(result, None);
+        Ok(())
+    }
 }
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/dtype.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/datatypes/dtype.rs`

 * *Files 7% similar despite different names*

```diff
@@ -21,28 +21,33 @@
     Int8,
     /// An [`i16`]
     Int16,
     /// An [`i32`]
     Int32,
     /// An [`i64`]
     Int64,
+    /// An [`i128`]
+    Int128,
     /// An [`u8`]
     UInt8,
     /// An [`u16`]
     UInt16,
     /// An [`u32`]
     UInt32,
     /// An [`u64`]
     UInt64,
     /// An 16-bit float
     Float16,
     /// A [`f32`]
     Float32,
     /// A [`f64`]
     Float64,
+    /// Fixed-precision decimal type.
+    /// TODO: allow negative scale once Arrow2 allows it: https://github.com/jorgecarleitao/arrow2/issues/1518
+    Decimal128(usize, usize),
     /// A [`i64`] representing a timestamp measured in [`TimeUnit`] with an optional timezone.
     ///
     /// Time is measured as a Unix epoch, counting the seconds from
     /// 00:00:00.000 on 1 January 1970, excluding leap seconds,
     /// as a 64-bit signed integer.
     ///
     /// The time zone is a string indicating the name of a time zone, one of:
@@ -76,14 +81,18 @@
     // Stop ArrowTypes
     /// A logical type for embeddings.
     Embedding(Box<Field>, usize),
     /// A logical type for images with variable shapes.
     Image(Option<ImageMode>),
     /// A logical type for images with the same size (height x width).
     FixedShapeImage(ImageMode, u32, u32),
+    /// A logical type for tensors with variable shapes.
+    Tensor(Box<DataType>),
+    /// A logical type for tensors with the same shape.
+    FixedShapeTensor(Box<DataType>, Vec<u64>),
     Python,
     Unknown,
 }
 
 #[derive(Serialize, Deserialize)]
 struct DataTypePayload {
     datatype: DataType,
@@ -111,21 +120,23 @@
         match self {
             DataType::Null => Ok(ArrowType::Null),
             DataType::Boolean => Ok(ArrowType::Boolean),
             DataType::Int8 => Ok(ArrowType::Int8),
             DataType::Int16 => Ok(ArrowType::Int16),
             DataType::Int32 => Ok(ArrowType::Int32),
             DataType::Int64 => Ok(ArrowType::Int64),
+            DataType::Int128 => Ok(ArrowType::Decimal(38, 0)),
             DataType::UInt8 => Ok(ArrowType::UInt8),
             DataType::UInt16 => Ok(ArrowType::UInt16),
             DataType::UInt32 => Ok(ArrowType::UInt32),
             DataType::UInt64 => Ok(ArrowType::UInt64),
             DataType::Float16 => Ok(ArrowType::Float16),
             DataType::Float32 => Ok(ArrowType::Float32),
             DataType::Float64 => Ok(ArrowType::Float64),
+            DataType::Decimal128(precision, scale) => Ok(ArrowType::Decimal(*precision, *scale)),
             DataType::Timestamp(unit, timezone) => {
                 Ok(ArrowType::Timestamp(unit.to_arrow()?, timezone.clone()))
             }
             DataType::Date => Ok(ArrowType::Date32),
             DataType::Time(unit) => Ok(ArrowType::Time64(unit.to_arrow()?)),
             DataType::Duration(unit) => Ok(ArrowType::Duration(unit.to_arrow()?)),
             DataType::Binary => Ok(ArrowType::LargeBinary),
@@ -142,32 +153,37 @@
                 ArrowType::Struct(fields)
             }),
             DataType::Extension(name, dtype, metadata) => Ok(ArrowType::Extension(
                 name.clone(),
                 Box::new(dtype.to_arrow()?),
                 metadata.clone(),
             )),
-            DataType::Embedding(..) | DataType::Image(..) | DataType::FixedShapeImage(..) => {
+            DataType::Embedding(..)
+            | DataType::Image(..)
+            | DataType::FixedShapeImage(..)
+            | DataType::Tensor(..)
+            | DataType::FixedShapeTensor(..) => {
                 let physical = Box::new(self.to_physical());
-                let embedding_extension = DataType::Extension(
+                let logical_extension = DataType::Extension(
                     DAFT_SUPER_EXTENSION_NAME.into(),
                     physical,
                     Some(self.to_json()?),
                 );
-                embedding_extension.to_arrow()
+                logical_extension.to_arrow()
             }
             _ => Err(DaftError::TypeError(format!(
                 "Can not convert {self:?} into arrow type"
             ))),
         }
     }
 
     pub fn to_physical(&self) -> DataType {
         use DataType::*;
         match self {
+            Decimal128(..) => Int128,
             Date => Int32,
             Duration(_) | Timestamp(..) | Time(_) => Int64,
             List(field) => List(Box::new(
                 Field::new(field.name.clone(), field.dtype.to_physical())
                     .with_metadata(field.metadata.clone()),
             )),
             FixedSizeList(field, size) => FixedSizeList(
@@ -194,15 +210,29 @@
                 Field::new("width", UInt32),
                 Field::new("mode", UInt8),
             ]),
             FixedShapeImage(mode, height, width) => FixedSizeList(
                 Box::new(Field::new("data", mode.get_dtype())),
                 usize::try_from(mode.num_channels() as u32 * height * width).unwrap(),
             ),
-            _ => self.clone(),
+            Tensor(dtype) => Struct(vec![
+                Field::new("data", List(Box::new(Field::new("data", *dtype.clone())))),
+                Field::new(
+                    "shape",
+                    List(Box::new(Field::new("shape", DataType::UInt64))),
+                ),
+            ]),
+            FixedShapeTensor(dtype, shape) => FixedSizeList(
+                Box::new(Field::new("data", *dtype.clone())),
+                usize::try_from(shape.iter().product::<u64>()).unwrap(),
+            ),
+            _ => {
+                assert!(self.is_physical());
+                self.clone()
+            }
         }
     }
 
     #[inline]
     pub fn is_arrow(&self) -> bool {
         self.to_arrow().is_ok()
     }
@@ -210,14 +240,15 @@
     #[inline]
     pub fn is_numeric(&self) -> bool {
         match self {
              DataType::Int8
              | DataType::Int16
              | DataType::Int32
              | DataType::Int64
+             | DataType::Int128
              | DataType::UInt8
              | DataType::UInt16
              | DataType::UInt32
              | DataType::UInt64
              // DataType::Float16
              | DataType::Float32
              | DataType::Float64 => true,
@@ -230,14 +261,15 @@
     pub fn is_integer(&self) -> bool {
         matches!(
             self,
             DataType::Int8
                 | DataType::Int16
                 | DataType::Int32
                 | DataType::Int64
+                | DataType::Int128
                 | DataType::UInt8
                 | DataType::UInt16
                 | DataType::UInt32
                 | DataType::UInt64
         )
     }
 
@@ -255,14 +287,34 @@
             DataType::Date | DataType::Timestamp(..) => true,
             DataType::Extension(_, inner, _) => inner.is_temporal(),
             _ => false,
         }
     }
 
     #[inline]
+    pub fn is_tensor(&self) -> bool {
+        matches!(self, DataType::Tensor(..))
+    }
+
+    #[inline]
+    pub fn is_fixed_shape_tensor(&self) -> bool {
+        matches!(self, DataType::FixedShapeTensor(..))
+    }
+
+    #[inline]
+    pub fn is_image(&self) -> bool {
+        matches!(self, DataType::Image(..))
+    }
+
+    #[inline]
+    pub fn is_fixed_shape_image(&self) -> bool {
+        matches!(self, DataType::FixedShapeImage(..))
+    }
+
+    #[inline]
     pub fn is_null(&self) -> bool {
         match self {
             DataType::Null => true,
             DataType::Extension(_, inner, _) => inner.is_null(),
             _ => false,
         }
     }
@@ -281,20 +333,23 @@
         }
     }
 
     #[inline]
     pub fn is_logical(&self) -> bool {
         matches!(
             self,
-            DataType::Date
+            DataType::Decimal128(..)
+                | DataType::Date
                 | DataType::Timestamp(..)
                 | DataType::Duration(..)
                 | DataType::Embedding(..)
                 | DataType::Image(..)
                 | DataType::FixedShapeImage(..)
+                | DataType::Tensor(..)
+                | DataType::FixedShapeTensor(..)
         )
     }
 
     #[inline]
     pub fn is_physical(&self) -> bool {
         !self.is_logical()
     }
@@ -354,14 +409,15 @@
             ArrowType::Date64 => DataType::Timestamp(TimeUnit::Milliseconds, None),
             ArrowType::Time32(timeunit) | ArrowType::Time64(timeunit) => {
                 DataType::Time(timeunit.into())
             }
             ArrowType::Duration(timeunit) => DataType::Duration(timeunit.into()),
             ArrowType::Binary | ArrowType::LargeBinary => DataType::Binary,
             ArrowType::Utf8 | ArrowType::LargeUtf8 => DataType::Utf8,
+            ArrowType::Decimal(precision, scale) => DataType::Decimal128(*precision, *scale),
             ArrowType::List(field) | ArrowType::LargeList(field) => {
                 DataType::List(Box::new(field.as_ref().into()))
             }
             ArrowType::FixedSizeList(field, size) => {
                 DataType::FixedSizeList(Box::new(field.as_ref().into()), *size)
             }
             ArrowType::Struct(fields) => {
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/field.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/datatypes/field.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/image_format.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/datatypes/image_format.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/image_mode.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/datatypes/image_mode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/logical.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/datatypes/logical.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 use std::{marker::PhantomData, sync::Arc};
 
 use crate::datatypes::{BooleanArray, DaftLogicalType, DateType, Field};
 use common_error::DaftResult;
 
 use super::{
-    DataArray, DataType, DurationType, EmbeddingType, FixedShapeImageType, ImageType, TimestampType,
+    DataArray, DataType, Decimal128Type, DurationType, EmbeddingType, FixedShapeImageType,
+    FixedShapeTensorType, ImageType, TensorType, TimestampType,
 };
 pub struct LogicalArray<L: DaftLogicalType> {
     pub field: Arc<Field>,
     pub physical: DataArray<L::PhysicalType>,
     marker_: PhantomData<L>,
 }
 
@@ -102,18 +103,21 @@
 
     pub fn filter(&self, mask: &BooleanArray) -> DaftResult<Self> {
         let new_array = self.physical.filter(mask)?;
         Ok(Self::new(self.field.clone(), new_array))
     }
 }
 
+pub type Decimal128Array = LogicalArray<Decimal128Type>;
 pub type DateArray = LogicalArray<DateType>;
 pub type DurationArray = LogicalArray<DurationType>;
 pub type EmbeddingArray = LogicalArray<EmbeddingType>;
 pub type ImageArray = LogicalArray<ImageType>;
 pub type FixedShapeImageArray = LogicalArray<FixedShapeImageType>;
 pub type TimestampArray = LogicalArray<TimestampType>;
+pub type TensorArray = LogicalArray<TensorType>;
+pub type FixedShapeTensorArray = LogicalArray<FixedShapeTensorType>;
 
 pub trait DaftImageryType: DaftLogicalType {}
 
 impl DaftImageryType for ImageType {}
 impl DaftImageryType for FixedShapeImageType {}
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/matching.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/datatypes/matching.rs`

 * *Files 20% similar despite different names*

```diff
@@ -226,16 +226,34 @@
 ) => ({
     macro_rules! __with_ty__ {( $_ $T:ident ) => ( $($body)* )}
     use $crate::datatypes::DataType::*;
     #[allow(unused_imports)]
     use $crate::datatypes::*;
 
     match $key_type {
+        Decimal128(..) => __with_ty__! { Decimal128Type },
         Date => __with_ty__! { DateType },
         Duration(..) => __with_ty__! { DurationType },
         Timestamp(..) => __with_ty__! { TimestampType },
         Embedding(..) => __with_ty__! { EmbeddingType },
         Image(..) => __with_ty__! { ImageType },
         FixedShapeImage(..) => __with_ty__! { FixedShapeImageType },
+        Tensor(..) => __with_ty__! { TensorType },
+        FixedShapeTensor(..) => __with_ty__! { FixedShapeTensorType },
         _ => panic!("{:?} not implemented for with_match_daft_logical_types", $key_type)
     }
 })}
+
+#[macro_export]
+macro_rules! with_match_daft_logical_primitive_types {(
+    $key_type:expr, | $_:tt $T:ident | $($body:tt)*
+) => ({
+    macro_rules! __with_ty__ {( $_ $T:ident ) => ( $($body)* )}
+    use $crate::datatypes::DataType::*;
+    match $key_type {
+        Decimal128(..) => __with_ty__! { i128 },
+        Duration(..) => __with_ty__! { i64 },
+        Date => __with_ty__! { i32 },
+        Timestamp(..) => __with_ty__! { i64 },
+        _ => panic!("no logical -> primitive conversion available for {:?}", $key_type)
+    }
+})}
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/mod.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/datatypes/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 mod matching;
 mod time_unit;
 
 use std::ops::{Add, Div, Mul, Rem, Sub};
 
 pub use crate::array::DataArray;
 use arrow2::{
-    compute::{arithmetics::basic::NativeArithmetics, comparison::Simd8},
+    compute::comparison::Simd8,
     types::{simd::Simd, NativeType},
 };
+pub use binary_ops::try_physical_supertype;
 pub use dtype::DataType;
 pub use field::Field;
 pub use image_format::ImageFormat;
 pub use image_mode::ImageMode;
 use num_traits::{Bounded, Float, FromPrimitive, Num, NumCast, ToPrimitive, Zero};
 pub use time_unit::TimeUnit;
 pub mod logical;
@@ -86,14 +87,15 @@
 
 impl_daft_arrow_datatype!(NullType, Null);
 impl_daft_arrow_datatype!(BooleanType, Boolean);
 impl_daft_arrow_datatype!(Int8Type, Int8);
 impl_daft_arrow_datatype!(Int16Type, Int16);
 impl_daft_arrow_datatype!(Int32Type, Int32);
 impl_daft_arrow_datatype!(Int64Type, Int64);
+impl_daft_arrow_datatype!(Int128Type, Int128);
 impl_daft_arrow_datatype!(UInt8Type, UInt8);
 impl_daft_arrow_datatype!(UInt16Type, UInt16);
 impl_daft_arrow_datatype!(UInt32Type, UInt32);
 impl_daft_arrow_datatype!(UInt64Type, UInt64);
 impl_daft_arrow_datatype!(Float16Type, Float16);
 impl_daft_arrow_datatype!(Float32Type, Float32);
 impl_daft_arrow_datatype!(Float64Type, Float64);
@@ -103,21 +105,24 @@
 impl_daft_arrow_datatype!(ListType, Unknown);
 impl_daft_arrow_datatype!(StructType, Unknown);
 impl_daft_arrow_datatype!(ExtensionType, Unknown);
 
 #[cfg(feature = "python")]
 impl_daft_non_arrow_datatype!(PythonType, Python);
 
+impl_daft_logical_datatype!(Decimal128Type, Unknown, Int128Type);
 impl_daft_logical_datatype!(TimestampType, Unknown, Int64Type);
 impl_daft_logical_datatype!(DateType, Date, Int32Type);
 impl_daft_logical_datatype!(TimeType, Unknown, Int64Type);
 impl_daft_logical_datatype!(DurationType, Unknown, Int64Type);
 impl_daft_logical_datatype!(EmbeddingType, Unknown, FixedSizeListType);
 impl_daft_logical_datatype!(ImageType, Unknown, StructType);
 impl_daft_logical_datatype!(FixedShapeImageType, Unknown, FixedSizeListType);
+impl_daft_logical_datatype!(TensorType, Unknown, StructType);
+impl_daft_logical_datatype!(FixedShapeTensorType, Unknown, FixedSizeListType);
 
 pub trait NumericNative:
     PartialOrd
     + NativeType
     + Num
     + NumCast
     + Zero
@@ -128,15 +133,14 @@
     + Sub<Output = Self>
     + Mul<Output = Self>
     + Div<Output = Self>
     + Rem<Output = Self>
     + Bounded
     + FromPrimitive
     + ToPrimitive
-    + NativeArithmetics
 {
     type DAFTTYPE: DaftNumericType;
 }
 
 /// Trait to express types that are native and can be vectorized
 pub trait DaftNumericType: Send + Sync + DaftArrowBackedType + 'static {
     type Native: NumericNative;
@@ -150,14 +154,17 @@
 }
 impl NumericNative for i32 {
     type DAFTTYPE = Int32Type;
 }
 impl NumericNative for i64 {
     type DAFTTYPE = Int64Type;
 }
+impl NumericNative for i128 {
+    type DAFTTYPE = Int128Type;
+}
 impl NumericNative for u8 {
     type DAFTTYPE = UInt8Type;
 }
 impl NumericNative for u16 {
     type DAFTTYPE = UInt16Type;
 }
 impl NumericNative for u32 {
@@ -194,35 +201,39 @@
 }
 impl DaftNumericType for Int32Type {
     type Native = i32;
 }
 impl DaftNumericType for Int64Type {
     type Native = i64;
 }
+impl DaftNumericType for Int128Type {
+    type Native = i128;
+}
 impl DaftNumericType for Float32Type {
     type Native = f32;
 }
 impl DaftNumericType for Float64Type {
     type Native = f64;
 }
 
 pub trait DaftIntegerType: DaftNumericType
 where
-    Self::Native: arrow2::types::Index,
+    Self::Native: Ord,
 {
 }
 
 impl DaftIntegerType for UInt8Type {}
 impl DaftIntegerType for UInt16Type {}
 impl DaftIntegerType for UInt32Type {}
 impl DaftIntegerType for UInt64Type {}
 impl DaftIntegerType for Int8Type {}
 impl DaftIntegerType for Int16Type {}
 impl DaftIntegerType for Int32Type {}
 impl DaftIntegerType for Int64Type {}
+impl DaftIntegerType for Int128Type {}
 
 pub trait DaftFloatType: DaftNumericType
 where
     Self::Native: Float,
 {
 }
 
@@ -236,14 +247,15 @@
 
 pub type NullArray = DataArray<NullType>;
 pub type BooleanArray = DataArray<BooleanType>;
 pub type Int8Array = DataArray<Int8Type>;
 pub type Int16Array = DataArray<Int16Type>;
 pub type Int32Array = DataArray<Int32Type>;
 pub type Int64Array = DataArray<Int64Type>;
+pub type Int128Array = DataArray<Int128Type>;
 pub type UInt8Array = DataArray<UInt8Type>;
 pub type UInt16Array = DataArray<UInt16Type>;
 pub type UInt32Array = DataArray<UInt32Type>;
 pub type UInt64Array = DataArray<UInt64Type>;
 pub type Float16Array = DataArray<Float16Type>;
 pub type Float32Array = DataArray<Float32Type>;
 pub type Float64Array = DataArray<Float64Type>;
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/datatypes/time_unit.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/datatypes/time_unit.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/ffi.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/ffi.rs`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,30 @@
         pyo3::intern!(py, "_import_from_c"),
         (array_ptr as Py_uintptr_t, schema_ptr as Py_uintptr_t),
     )?;
 
     Ok(array.to_object(py))
 }
 
+pub fn to_py_schema(
+    dtype: &arrow2::datatypes::DataType,
+    py: Python,
+    pyarrow: &PyModule,
+) -> PyResult<PyObject> {
+    let schema = Box::new(ffi::export_field_to_c(&Field::new("", dtype.clone(), true)));
+    let schema_ptr: *const ffi::ArrowSchema = &*schema;
+
+    let field = pyarrow.getattr(pyo3::intern!(py, "Field"))?.call_method1(
+        pyo3::intern!(py, "_import_from_c"),
+        (schema_ptr as Py_uintptr_t,),
+    )?;
+
+    Ok(field.to_object(py))
+}
+
 fn fix_child_array_slice_offsets(array: ArrayRef) -> ArrayRef {
     /* Zero-copy slices of arrow2 struct/fixed-size list arrays are currently not correctly
     converted to pyarrow struct/fixed-size list arrays when going over the FFI boundary;
     this helper function ensures that such arrays' slice representation is changed to work
     around this bug.
 
     -- The Problem --
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/kernels/hashing.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/kernels/hashing.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/kernels/search_sorted.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/kernels/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/kernels/utf8.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/kernels/utf8.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/lib.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/lib.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#![feature(let_chains)]
+
 pub mod array;
 pub mod datatypes;
 #[cfg(feature = "python")]
 pub mod ffi;
 pub mod kernels;
 #[cfg(feature = "python")]
 pub mod python;
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/python/datatype.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/python/datatype.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-use crate::datatypes::{DataType, Field, ImageMode, TimeUnit};
+use crate::{
+    datatypes::{DataType, Field, ImageMode, TimeUnit},
+    ffi,
+};
 use pyo3::{
     class::basic::CompareOp,
     exceptions::PyValueError,
     prelude::*,
     types::{PyBytes, PyDict, PyString, PyTuple},
 };
 
@@ -154,14 +157,19 @@
 
     #[staticmethod]
     pub fn string() -> PyResult<Self> {
         Ok(DataType::Utf8.into())
     }
 
     #[staticmethod]
+    pub fn decimal128(precision: usize, scale: usize) -> PyResult<Self> {
+        Ok(DataType::Decimal128(precision, scale).into())
+    }
+
+    #[staticmethod]
     pub fn date() -> PyResult<Self> {
         Ok(DataType::Date.into())
     }
 
     #[staticmethod]
     pub fn timestamp(timeunit: PyTimeUnit, timezone: Option<String>) -> PyResult<Self> {
         Ok(DataType::Timestamp(timeunit.timeunit, timezone).into())
@@ -259,31 +267,113 @@
             }
             (None, None) => Ok(DataType::Image(mode).into()),
             (_, _) => Err(PyValueError::new_err(format!("Height and width for image type must both be specified or both not specified, but got: height={:?}, width={:?}", height, width))),
         }
     }
 
     #[staticmethod]
+    pub fn tensor(dtype: Self, shape: Option<Vec<u64>>) -> PyResult<Self> {
+        // TODO(Clark): Add support for non-numeric (e.g. string) tensor columns.
+        if !dtype.dtype.is_numeric() {
+            return Err(PyValueError::new_err(format!(
+                "The data type for a tensor column must be numeric, but got: {}",
+                dtype.dtype
+            )));
+        }
+        let dtype = Box::new(dtype.dtype);
+        match shape {
+            Some(shape) => Ok(DataType::FixedShapeTensor(dtype, shape).into()),
+            None => Ok(DataType::Tensor(dtype).into()),
+        }
+    }
+
+    #[staticmethod]
     pub fn python() -> PyResult<Self> {
         Ok(DataType::Python.into())
     }
 
+    pub fn to_arrow(&self, cast_tensor_type_for_ray: Option<bool>) -> PyResult<PyObject> {
+        Python::with_gil(|py| {
+            let pyarrow = py.import(pyo3::intern!(py, "pyarrow"))?;
+            let cast_tensor_to_ray_type = cast_tensor_type_for_ray.unwrap_or(false);
+            match (&self.dtype, cast_tensor_to_ray_type) {
+                (DataType::FixedShapeTensor(dtype, shape), false) => Ok(
+                    if py
+                        .import(pyo3::intern!(py, "daft.utils"))?
+                        .getattr(pyo3::intern!(py, "pyarrow_supports_fixed_shape_tensor"))?
+                        .call0()?
+                        .extract()?
+                    {
+                        pyarrow
+                            .getattr(pyo3::intern!(py, "fixed_shape_tensor"))?
+                            .call1((
+                                Self {
+                                    dtype: *dtype.clone(),
+                                }
+                                .to_arrow(None)?,
+                                pyo3::types::PyTuple::new(py, shape.clone()),
+                            ))?
+                            .to_object(py)
+                    } else {
+                        // Fall back to default Daft super extension representation if installed pyarrow doesn't have the
+                        // canonical tensor extension type.
+                        ffi::to_py_schema(&self.dtype.to_arrow()?, py, pyarrow)?
+                    },
+                ),
+                (DataType::FixedShapeTensor(dtype, shape), true) => Ok(py
+                    .import(pyo3::intern!(py, "ray.data.extensions"))?
+                    .getattr(pyo3::intern!(py, "ArrowTensorType"))?
+                    .call1((
+                        pyo3::types::PyTuple::new(py, shape.clone()),
+                        Self {
+                            dtype: *dtype.clone(),
+                        }
+                        .to_arrow(None)?,
+                    ))?
+                    .to_object(py)),
+                (_, _) => ffi::to_py_schema(&self.dtype.to_arrow()?, py, pyarrow)?
+                    .getattr(py, pyo3::intern!(py, "type")),
+            }
+        })
+    }
+
+    pub fn is_image(&self) -> PyResult<bool> {
+        Ok(self.dtype.is_image())
+    }
+
+    pub fn is_fixed_shape_image(&self) -> PyResult<bool> {
+        Ok(self.dtype.is_fixed_shape_image())
+    }
+
+    pub fn is_tensor(&self) -> PyResult<bool> {
+        Ok(self.dtype.is_tensor())
+    }
+
+    pub fn is_fixed_shape_tensor(&self) -> PyResult<bool> {
+        Ok(self.dtype.is_fixed_shape_tensor())
+    }
+
     pub fn is_logical(&self) -> PyResult<bool> {
         Ok(self.dtype.is_logical())
     }
 
     pub fn is_equal(&self, other: &PyAny) -> PyResult<bool> {
         if other.is_instance_of::<PyDataType>() {
             let other = other.extract::<PyDataType>()?;
             Ok(self.dtype == other.dtype)
         } else {
             Ok(false)
         }
     }
 
+    #[staticmethod]
+    pub fn from_json(serialized: &str) -> PyResult<Self> {
+        Ok(DataType::from_json(serialized)?.into())
+    }
+
     pub fn __setstate__(&mut self, py: Python, state: PyObject) -> PyResult<()> {
         match state.extract::<&PyBytes>(py) {
             Ok(s) => {
                 self.dtype = bincode::deserialize(s.as_bytes()).unwrap();
                 Ok(())
             }
             Err(e) => Err(e),
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/python/field.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/python/field.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/python/mod.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/python/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/python/schema.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/python/schema.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/python/series.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/python/series.rs`

 * *Files 12% similar despite different names*

```diff
@@ -30,18 +30,17 @@
     }
 
     // This ingests a Python list[object] directly into a Rust PythonArray.
     #[staticmethod]
     pub fn from_pylist(name: &str, pylist: &PyAny, pyobj: &str) -> PyResult<Self> {
         let vec_pyobj: Vec<PyObject> = pylist.extract()?;
         let py = pylist.py();
-
         let dtype = match pyobj {
             "force" => DataType::Python,
-            "allow" => infer_daft_dtype_for_sequence(&vec_pyobj, py)?.unwrap_or(DataType::Python),
+            "allow" => infer_daft_dtype_for_sequence(&vec_pyobj, py, name)?.unwrap_or(DataType::Python),
             "disallow" => panic!("Cannot create a Series from a pylist and being strict about only using Arrow types by setting pyobj=disallow"),
             _ => panic!("Unsupported pyobj behavior when creating Series from pylist: {}", pyobj)
         };
         let arrow_array: Box<dyn arrow2::array::Array> =
             Box::new(PseudoArrowArray::<PyObject>::from_pyobj_vec(vec_pyobj));
         let field = Field::new(name, DataType::Python);
 
@@ -267,16 +266,16 @@
         Ok(self.series.dt_year()?.into())
     }
 
     pub fn dt_day_of_week(&self) -> PyResult<Self> {
         Ok(self.series.dt_day_of_week()?.into())
     }
 
-    pub fn arr_lengths(&self) -> PyResult<Self> {
-        Ok(self.series.arr_lengths()?.into_series().into())
+    pub fn list_lengths(&self) -> PyResult<Self> {
+        Ok(self.series.list_lengths()?.into_series().into())
     }
 
     pub fn image_decode(&self) -> PyResult<Self> {
         Ok(self.series.image_decode()?.into())
     }
 
     pub fn image_encode(&self, image_format: ImageFormat) -> PyResult<Self> {
@@ -321,46 +320,84 @@
         item.series
     }
 }
 
 fn infer_daft_dtype_for_sequence(
     vec_pyobj: &[PyObject],
     py: pyo3::Python,
+    name: &str,
 ) -> PyResult<Option<DataType>> {
     let py_pil_image_type = py
         .import(pyo3::intern!(py, "PIL.Image"))
         .and_then(|m| m.getattr(pyo3::intern!(py, "Image")));
+    let np_ndarray_type = py
+        .import(pyo3::intern!(py, "numpy"))
+        .and_then(|m| m.getattr(pyo3::intern!(py, "ndarray")));
+    let np_generic_type = py
+        .import(pyo3::intern!(py, "numpy"))
+        .and_then(|m| m.getattr(pyo3::intern!(py, "generic")));
+    let from_numpy_dtype = {
+        py.import(pyo3::intern!(py, "daft.datatype"))?
+            .getattr(pyo3::intern!(py, "DataType"))?
+            .getattr(pyo3::intern!(py, "from_numpy_dtype"))?
+    };
     let mut dtype: Option<DataType> = None;
     for obj in vec_pyobj.iter() {
         let obj = obj.as_ref(py);
-        if let Ok(pil_image_type) = py_pil_image_type {
-            if obj.is_instance(pil_image_type)? {
-                let mode_str = obj
-                    .getattr(pyo3::intern!(py, "mode"))?
-                    .extract::<String>()?;
-                let mode = ImageMode::from_pil_mode_str(&mode_str)?;
-                match dtype {
-                    Some(DataType::Image(Some(existing_mode))) => {
-                        if existing_mode != mode {
-                            // Mixed-mode case, set mode to None.
-                            dtype = Some(DataType::Image(None));
-                        }
-                    }
-                    None => {
-                        // Set to (currently) uniform mode image dtype.
-                        dtype = Some(DataType::Image(Some(mode)));
-                    }
-                    // No-op, since dtype is already for mixed-mode images.
-                    Some(DataType::Image(None)) => {}
-                    _ => {
-                        // Images mixed with non-images; short-circuit since union dtypes are not (yet) supported.
-                        dtype = None;
-                        break;
+        if let Ok(pil_image_type) = py_pil_image_type && obj.is_instance(pil_image_type)? {
+            let mode_str = obj
+                .getattr(pyo3::intern!(py, "mode"))?
+                .extract::<String>()?;
+            let mode = ImageMode::from_pil_mode_str(&mode_str)?;
+            match &dtype {
+                Some(DataType::Image(Some(existing_mode))) => {
+                    if *existing_mode != mode {
+                        // Mixed-mode case, set mode to None.
+                        dtype = Some(DataType::Image(None));
                     }
                 }
+                None => {
+                    // Set to (currently) uniform mode image dtype.
+                    dtype = Some(DataType::Image(Some(mode)));
+                }
+                // No-op, since dtype is already for mixed-mode images.
+                Some(DataType::Image(None)) => {}
+                _ => {
+                    // Images mixed with non-images; short-circuit since union dtypes are not (yet) supported.
+                    dtype = None;
+                    break;
+                }
+            }
+        } else if let Ok(np_ndarray_type) = np_ndarray_type && let Ok(np_generic_type) = np_generic_type && (obj.is_instance(np_ndarray_type)? || obj.is_instance(np_generic_type)?) {
+            let np_dtype = obj.getattr(pyo3::intern!(py, "dtype"))?;
+            let inferred_inner_dtype = from_numpy_dtype.call1((np_dtype,)).map(|dt| dt.getattr(pyo3::intern!(py, "_dtype")).unwrap().extract::<PyDataType>().unwrap().dtype);
+            let shape: Vec<u64> = obj.getattr(pyo3::intern!(py, "shape"))?.extract()?;
+            let inferred_dtype = match inferred_inner_dtype {
+                Ok(inferred_inner_dtype) if shape.len() == 1 => Some(DataType::List(Box::new(Field::new(name, inferred_inner_dtype)))),
+                Ok(inferred_inner_dtype) if shape.len() > 1 => Some(DataType::Tensor(Box::new(inferred_inner_dtype))),
+                _ => None,
+            };
+            match (&dtype, &inferred_dtype) {
+                // Tensors with mixed inner dtypes is not supported, short-circuit.
+                (Some(existing_dtype), Some(inferred_dtype)) if existing_dtype != inferred_dtype => {
+                    // TODO(Clark): Do some basic type promotion here, e.g. (u32, u64) --> u64.
+                    dtype = None;
+                    break;
+                }
+                // Existing and inferred dtypes must be the same here, so this is a no-op.
+                (Some(_), Some(_)) => {}
+                // No existing dtype and inferred is non-None, so set cached dtype to inferred.
+                (None, Some(inferred_dtype)) => {
+                    dtype = Some(inferred_dtype.clone());
+                }
+                // Inferred inner dtype isn't representable with Arrow, so we'll need to use a plain Python representation.
+                (_, None) => {
+                    dtype = None;
+                    break;
+                }
             }
         } else if !obj.is_none() {
             // Non-image types; short-circuit since only image types are supported and union dtypes are not (yet)
             // supported.
             dtype = None;
             break;
         }
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/schema.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/schema.rs`

 * *Files 7% similar despite different names*

```diff
@@ -120,7 +120,16 @@
             .iter()
             .map(|(name, field)| format!("{}\n{:?}", name, field.dtype))
             .collect();
         table.add_row(header);
         write!(f, "{table}")
     }
 }
+
+impl TryFrom<&arrow2::datatypes::Schema> for Schema {
+    type Error = DaftError;
+    fn try_from(arrow_schema: &arrow2::datatypes::Schema) -> DaftResult<Self> {
+        let fields = &arrow_schema.fields;
+        let daft_fields: Vec<Field> = fields.iter().map(|f| f.into()).collect();
+        Self::new(daft_fields)
+    }
+}
```

#### html2text {}

```diff
@@ -26,8 +26,12 @@
 { fields }) } _ => Err(DaftError::ValueError( "Cannot union two schemas with
 overlapping keys".to_string(), )), } } pub fn repr_html(&self) -> String { /
 / Produces a
 "); res } } impl Display for Schema { // `f` is a buffer, and this method must
 write the formatted string into it fn fmt(&self, f: &mut Formatter) -> Result
 { let mut table = prettytable::Table::new(); let header = self .fields .iter()
 .map(|(name, field)| format!("{}\n{:?}", name, field.dtype)) .collect();
-table.add_row(header); write!(f, "{table}") } }
+table.add_row(header); write!(f, "{table}") } } impl TryFrom<&arrow2::
+datatypes::Schema> for Schema { type Error = DaftError; fn try_from
+(arrow_schema: &arrow2::datatypes::Schema) -> DaftResult { let fields =
+&arrow_schema.fields; let daft_fields: Vec = fields.iter().map(|f| f.into
+()).collect(); Self::new(daft_fields) } }
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/series/array_impl/binary_ops.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/series/array_impl/binary_ops.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,172 +1,236 @@
 use std::ops::{Add, Div, Mul, Rem, Sub};
 
 use common_error::DaftResult;
 
 use crate::{
-    datatypes::{Float64Type, Utf8Type},
+    array::ops::{DaftCompare, DaftLogical},
+    datatypes::{logical::Decimal128Array, BooleanType, Float64Type, Int128Array, Utf8Type},
     series::series_like::SeriesLike,
-    with_match_numeric_daft_types, DataType,
+    with_match_comparable_daft_types, with_match_numeric_daft_types, DataType,
 };
 
+use crate::datatypes::logical::{
+    DateArray, DurationArray, EmbeddingArray, FixedShapeImageArray, FixedShapeTensorArray,
+    ImageArray, TensorArray, TimestampArray,
+};
 use crate::datatypes::{
     BinaryArray, BooleanArray, ExtensionArray, FixedSizeListArray, Float32Array, Float64Array,
     Int16Array, Int32Array, Int64Array, Int8Array, ListArray, NullArray, StructArray, UInt16Array,
     UInt32Array, UInt64Array, UInt8Array, Utf8Array,
 };
 
-use crate::datatypes::logical::{
-    DateArray, DurationArray, EmbeddingArray, FixedShapeImageArray, ImageArray, TimestampArray,
-};
-
 use super::{ArrayWrapper, IntoSeries, Series};
 
 #[cfg(feature = "python")]
 use crate::{datatypes::PythonArray, series::ops::py_binary_op_utilfn};
 
-macro_rules! binary_op_default_impl {
-    ($self:expr, $rhs:expr, $op:ident, $default_op:ident) => {{
-        let output_type = ($self.data_type().$op($rhs.data_type()))?;
-        let lhs = $self.into_series();
-        $default_op(&lhs, $rhs, &output_type)
+#[cfg(feature = "python")]
+macro_rules! py_binary_op {
+    ($lhs:expr, $rhs:expr, $pyoperator:expr) => {
+        py_binary_op_utilfn!($lhs, $rhs, $pyoperator, "map_operator_arrow_semantics")
+    };
+}
+#[cfg(feature = "python")]
+macro_rules! py_binary_op_bool {
+    ($lhs:expr, $rhs:expr, $pyoperator:expr) => {
+        py_binary_op_utilfn!($lhs, $rhs, $pyoperator, "map_operator_arrow_semantics_bool")
+    };
+}
+
+macro_rules! cast_downcast_op {
+    ($lhs:expr, $rhs:expr, $ty_expr:expr, $ty_type:ty, $op:ident) => {{
+        let lhs = $lhs.cast($ty_expr)?;
+        let rhs = $rhs.cast($ty_expr)?;
+        let lhs = lhs.downcast::<$ty_type>()?;
+        let rhs = rhs.downcast::<$ty_type>()?;
+        lhs.$op(rhs)
     }};
 }
 
-pub(crate) trait SeriesBinaryOps: SeriesLike {
-    fn add(&self, rhs: &Series) -> DaftResult<Series> {
-        binary_op_default_impl!(self, rhs, add, physical_add)
-    }
-    fn sub(&self, rhs: &Series) -> DaftResult<Series> {
-        binary_op_default_impl!(self, rhs, sub, physical_sub)
-    }
-    fn mul(&self, rhs: &Series) -> DaftResult<Series> {
-        binary_op_default_impl!(self, rhs, mul, physical_mul)
-    }
-    fn div(&self, rhs: &Series) -> DaftResult<Series> {
-        binary_op_default_impl!(self, rhs, div, physical_div)
-    }
-    fn rem(&self, rhs: &Series) -> DaftResult<Series> {
-        binary_op_default_impl!(self, rhs, rem, physical_rem)
-    }
+macro_rules! cast_downcast_op_into_series {
+    ($lhs:expr, $rhs:expr, $ty_expr:expr, $ty_type:ty, $op:ident) => {{
+        Ok(cast_downcast_op!($lhs, $rhs, $ty_expr, $ty_type, $op)?
+            .into_series()
+            .rename($lhs.name()))
+    }};
 }
 
-#[cfg(feature = "python")]
-macro_rules! py_binary_op {
-    ($lhs:expr, $rhs:expr, $pyoperator:expr) => {
-        py_binary_op_utilfn!($lhs, $rhs, $pyoperator, "map_operator_arrow_semantics")
+macro_rules! binary_op_unimplemented {
+    ($lhs:expr, $op:expr, $rhs:expr, $output_ty:expr) => {
+        unimplemented!(
+            "No implementation for {} {} {} -> {}",
+            $lhs.data_type(),
+            $op,
+            $rhs.data_type(),
+            $output_ty,
+        )
     };
 }
 
 macro_rules! py_numeric_binary_op {
-    ($op:ident, $pyop:expr, $lhs:expr, $rhs:expr, $output_ty:expr) => {{
+    ($self:expr, $rhs:expr, $op:ident, $pyop:expr) => {{
+        let output_type = ($self.data_type().$op($rhs.data_type()))?;
+        let lhs = $self.into_series();
         use DataType::*;
-        match $output_ty {
+        match &output_type {
             #[cfg(feature = "python")]
-            Python => Ok(py_binary_op!($lhs, $rhs, $pyop)),
+            Python => Ok(py_binary_op!(lhs, $rhs, $pyop)),
             output_type if output_type.is_numeric() => {
-                let lhs = $lhs.cast(&output_type)?;
-                let rhs = $rhs.cast(&output_type)?;
                 with_match_numeric_daft_types!(output_type, |$T| {
-                    let lhs = lhs.downcast::<$T>()?;
-                    let rhs = rhs.downcast::<$T>()?;
-                    Ok(lhs.$op(rhs)?.into_series().rename(lhs.name()))
+                    cast_downcast_op_into_series!(lhs, $rhs, output_type, $T, $op)
                 })
             }
-            _ => panic!(
-                "No implementation for {} {} {} -> {}",
-                $lhs.data_type(),
-                $pyop,
-                $rhs.data_type(),
-                $output_ty,
-            ),
+            _ => binary_op_unimplemented!(lhs, $pyop, $rhs, output_type),
         }
     }};
 }
 
-fn physical_add(lhs: &Series, rhs: &Series, output_type: &DataType) -> DaftResult<Series> {
-    use DataType::*;
-    match output_type {
-        Utf8 => {
-            let lhs = lhs.cast(&Utf8)?;
-            let rhs = rhs.cast(&Utf8)?;
-            let lhs = lhs.downcast::<Utf8Type>()?;
-            let rhs = rhs.downcast::<Utf8Type>()?;
-            Ok(lhs.add(rhs)?.into_series().rename(lhs.name()))
+macro_rules! physical_logic_op {
+    ($self:expr, $rhs:expr, $op:ident, $pyop:expr) => {{
+        let output_type = ($self.data_type().logical_op($rhs.data_type()))?;
+        let lhs = $self.into_series();
+        use DataType::*;
+        if let Boolean = output_type {
+            match (&lhs.data_type(), &$rhs.data_type()) {
+                #[cfg(feature = "python")]
+                (Python, _) | (_, Python) => py_binary_op_bool!(lhs, $rhs, $pyop)
+                    .downcast::<BooleanType>()
+                    .cloned(),
+                _ => cast_downcast_op!(lhs, $rhs, &Boolean, BooleanType, $op),
+            }
+        } else {
+            unreachable!()
         }
-        _ => py_numeric_binary_op!(add, "add", lhs, rhs, output_type),
-    }
-}
-
-fn physical_sub(lhs: &Series, rhs: &Series, output_type: &DataType) -> DaftResult<Series> {
-    py_numeric_binary_op!(sub, "sub", lhs, rhs, output_type)
+    }};
 }
 
-fn physical_mul(lhs: &Series, rhs: &Series, output_type: &DataType) -> DaftResult<Series> {
-    py_numeric_binary_op!(mul, "mul", lhs, rhs, output_type)
+macro_rules! physical_compare_op {
+    ($self:expr, $rhs:expr, $op:ident, $pyop:expr) => {{
+        let (output_type, comp_type) = ($self.data_type().comparison_op($rhs.data_type()))?;
+        let lhs = $self.into_series();
+        use DataType::*;
+        if let Boolean = output_type {
+            match comp_type {
+                #[cfg(feature = "python")]
+                Python => py_binary_op_bool!(lhs, $rhs, $pyop)
+                    .downcast::<BooleanType>()
+                    .cloned(),
+                _ => with_match_comparable_daft_types!(comp_type, |$T| {
+                    cast_downcast_op!(lhs, $rhs, &comp_type, $T, $op)
+                }),
+            }
+        } else {
+            unreachable!()
+        }
+    }};
 }
 
-fn physical_div(lhs: &Series, rhs: &Series, output_type: &DataType) -> DaftResult<Series> {
-    use DataType::*;
-    match output_type {
-        #[cfg(feature = "python")]
-        Python => Ok(py_binary_op!(lhs, rhs, "truediv")),
-        Float64 => {
-            let lhs = lhs.cast(&Float64)?;
-            let rhs = rhs.cast(&Float64)?;
-            let lhs = lhs.downcast::<Float64Type>()?;
-            let rhs = rhs.downcast::<Float64Type>()?;
-            Ok(lhs.div(rhs)?.into_series().rename(lhs.name()))
+pub(crate) trait SeriesBinaryOps: SeriesLike {
+    fn add(&self, rhs: &Series) -> DaftResult<Series> {
+        let output_type = (self.data_type().add(rhs.data_type()))?;
+        let lhs = self.into_series();
+        use DataType::*;
+        match &output_type {
+            #[cfg(feature = "python")]
+            Python => Ok(py_binary_op!(lhs, rhs, "add")),
+            Utf8 => cast_downcast_op_into_series!(lhs, rhs, &Utf8, Utf8Type, add),
+            output_type if output_type.is_numeric() => {
+                with_match_numeric_daft_types!(output_type, |$T| {
+                    cast_downcast_op_into_series!(lhs, rhs, output_type, $T, add)
+                })
+            }
+            _ => binary_op_unimplemented!(lhs, "+", rhs, output_type),
         }
-        _ => panic!(
-            "No implementation for {} / {} -> {}",
-            lhs.data_type(),
-            rhs.data_type(),
-            output_type,
-        ),
     }
-}
-
-fn physical_rem(lhs: &Series, rhs: &Series, output_type: &DataType) -> DaftResult<Series> {
-    py_numeric_binary_op!(rem, "mod", lhs, rhs, output_type)
+    fn sub(&self, rhs: &Series) -> DaftResult<Series> {
+        py_numeric_binary_op!(self, rhs, sub, "sub")
+    }
+    fn mul(&self, rhs: &Series) -> DaftResult<Series> {
+        py_numeric_binary_op!(self, rhs, mul, "mul")
+    }
+    fn div(&self, rhs: &Series) -> DaftResult<Series> {
+        let output_type = (self.data_type().div(rhs.data_type()))?;
+        let lhs = self.into_series();
+        use DataType::*;
+        match &output_type {
+            #[cfg(feature = "python")]
+            Python => Ok(py_binary_op!(lhs, rhs, "truediv")),
+            Float64 => cast_downcast_op_into_series!(lhs, rhs, &Float64, Float64Type, div),
+            _ => binary_op_unimplemented!(lhs, "/", rhs, output_type),
+        }
+    }
+    fn rem(&self, rhs: &Series) -> DaftResult<Series> {
+        py_numeric_binary_op!(self, rhs, rem, "mod")
+    }
+    fn and(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+        physical_logic_op!(self, rhs, and, "and_")
+    }
+    fn or(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+        physical_logic_op!(self, rhs, or, "or_")
+    }
+    fn xor(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+        physical_logic_op!(self, rhs, xor, "xor")
+    }
+    fn equal(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+        physical_compare_op!(self, rhs, equal, "eq")
+    }
+    fn not_equal(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+        physical_compare_op!(self, rhs, not_equal, "ne")
+    }
+    fn lt(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+        physical_compare_op!(self, rhs, lt, "lt")
+    }
+    fn lte(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+        physical_compare_op!(self, rhs, lte, "le")
+    }
+    fn gt(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+        physical_compare_op!(self, rhs, gt, "gt")
+    }
+    fn gte(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+        physical_compare_op!(self, rhs, gte, "ge")
+    }
 }
 
 #[cfg(feature = "python")]
 impl SeriesBinaryOps for ArrayWrapper<PythonArray> {}
 impl SeriesBinaryOps for ArrayWrapper<NullArray> {}
 impl SeriesBinaryOps for ArrayWrapper<BooleanArray> {}
 impl SeriesBinaryOps for ArrayWrapper<BinaryArray> {}
 impl SeriesBinaryOps for ArrayWrapper<Int8Array> {}
 impl SeriesBinaryOps for ArrayWrapper<Int16Array> {}
 impl SeriesBinaryOps for ArrayWrapper<Int32Array> {}
 impl SeriesBinaryOps for ArrayWrapper<Int64Array> {}
+impl SeriesBinaryOps for ArrayWrapper<Int128Array> {}
 impl SeriesBinaryOps for ArrayWrapper<UInt8Array> {}
 impl SeriesBinaryOps for ArrayWrapper<UInt16Array> {}
 impl SeriesBinaryOps for ArrayWrapper<UInt32Array> {}
 impl SeriesBinaryOps for ArrayWrapper<UInt64Array> {}
 impl SeriesBinaryOps for ArrayWrapper<Float32Array> {}
 impl SeriesBinaryOps for ArrayWrapper<Float64Array> {}
 impl SeriesBinaryOps for ArrayWrapper<Utf8Array> {}
 impl SeriesBinaryOps for ArrayWrapper<FixedSizeListArray> {}
 impl SeriesBinaryOps for ArrayWrapper<ListArray> {}
 impl SeriesBinaryOps for ArrayWrapper<StructArray> {}
 impl SeriesBinaryOps for ArrayWrapper<ExtensionArray> {}
+impl SeriesBinaryOps for ArrayWrapper<Decimal128Array> {}
 impl SeriesBinaryOps for ArrayWrapper<DateArray> {}
 impl SeriesBinaryOps for ArrayWrapper<DurationArray> {
     fn add(&self, rhs: &Series) -> DaftResult<Series> {
         use DataType::*;
         let output_type = (self.data_type() + rhs.data_type())?;
         let lhs = self.0.clone().into_series();
         match rhs.data_type() {
             Timestamp(..) => {
                 let lhs = lhs.as_physical()?;
                 let rhs = rhs.as_physical()?;
                 let physical_result = lhs.add(rhs)?;
                 physical_result.cast(&output_type)
             }
-            _ => physical_add(&lhs, rhs, &output_type),
+            _ => binary_op_unimplemented!(lhs, "+", rhs, output_type),
         }
     }
 }
 impl SeriesBinaryOps for ArrayWrapper<TimestampArray> {
     fn add(&self, rhs: &Series) -> DaftResult<Series> {
         use DataType::*;
         let output_type = (self.data_type() + rhs.data_type())?;
@@ -174,28 +238,30 @@
         match rhs.data_type() {
             Duration(..) => {
                 let lhs = lhs.as_physical()?;
                 let rhs = rhs.as_physical()?;
                 let physical_result = lhs.add(rhs)?;
                 physical_result.cast(&output_type)
             }
-            _ => physical_add(&lhs, rhs, &output_type),
+            _ => binary_op_unimplemented!(lhs, "+", rhs, output_type),
         }
     }
     fn sub(&self, rhs: &Series) -> DaftResult<Series> {
         use DataType::*;
         let output_type = (self.data_type() - rhs.data_type())?;
         let lhs = self.0.clone().into_series();
         match rhs.data_type() {
             Duration(..) => {
                 let lhs = lhs.as_physical()?;
                 let rhs = rhs.as_physical()?;
                 let physical_result = lhs.sub(rhs)?;
                 physical_result.cast(&output_type)
             }
-            _ => physical_sub(&lhs, rhs, &output_type),
+            _ => binary_op_unimplemented!(lhs, "-", rhs, output_type),
         }
     }
 }
 impl SeriesBinaryOps for ArrayWrapper<EmbeddingArray> {}
 impl SeriesBinaryOps for ArrayWrapper<ImageArray> {}
 impl SeriesBinaryOps for ArrayWrapper<FixedShapeImageArray> {}
+impl SeriesBinaryOps for ArrayWrapper<TensorArray> {}
+impl SeriesBinaryOps for ArrayWrapper<FixedShapeTensorArray> {}
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/series/array_impl/data_array.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/series/array_impl/data_array.rs`

 * *Files 8% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 #[cfg(feature = "python")]
 use crate::datatypes::PythonArray;
 use crate::series::array_impl::binary_ops::SeriesBinaryOps;
 use crate::series::Field;
 use crate::{
     datatypes::{
         BinaryArray, BooleanArray, ExtensionArray, FixedSizeListArray, Float32Array, Float64Array,
-        Int16Array, Int32Array, Int64Array, Int8Array, ListArray, NullArray, StructArray,
-        UInt16Array, UInt32Array, UInt64Array, UInt8Array, Utf8Array,
+        Int128Array, Int16Array, Int32Array, Int64Array, Int8Array, ListArray, NullArray,
+        StructArray, UInt16Array, UInt32Array, UInt64Array, UInt8Array, Utf8Array,
     },
     series::series_like::SeriesLike,
     with_match_integer_daft_types,
 };
 use common_error::DaftResult;
 
 use crate::datatypes::DataType;
@@ -271,41 +271,67 @@
                     None => Ok(self.0.list()?.into_series()),
                 }
             }
 
             fn add(&self, rhs: &Series) -> DaftResult<Series> {
                 SeriesBinaryOps::add(self, rhs)
             }
-
             fn sub(&self, rhs: &Series) -> DaftResult<Series> {
                 SeriesBinaryOps::sub(self, rhs)
             }
-
             fn mul(&self, rhs: &Series) -> DaftResult<Series> {
                 SeriesBinaryOps::mul(self, rhs)
             }
-
             fn div(&self, rhs: &Series) -> DaftResult<Series> {
                 SeriesBinaryOps::div(self, rhs)
             }
-
             fn rem(&self, rhs: &Series) -> DaftResult<Series> {
                 SeriesBinaryOps::rem(self, rhs)
             }
+
+            fn and(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+                SeriesBinaryOps::and(self, rhs)
+            }
+            fn or(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+                SeriesBinaryOps::or(self, rhs)
+            }
+            fn xor(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+                SeriesBinaryOps::xor(self, rhs)
+            }
+
+            fn equal(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+                SeriesBinaryOps::equal(self, rhs)
+            }
+            fn not_equal(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+                SeriesBinaryOps::not_equal(self, rhs)
+            }
+            fn lt(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+                SeriesBinaryOps::lt(self, rhs)
+            }
+            fn lte(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+                SeriesBinaryOps::lte(self, rhs)
+            }
+            fn gt(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+                SeriesBinaryOps::gt(self, rhs)
+            }
+            fn gte(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+                SeriesBinaryOps::gte(self, rhs)
+            }
         }
     };
 }
 
 impl_series_like_for_data_array!(NullArray);
 impl_series_like_for_data_array!(BooleanArray);
 impl_series_like_for_data_array!(BinaryArray);
 impl_series_like_for_data_array!(Int8Array);
 impl_series_like_for_data_array!(Int16Array);
 impl_series_like_for_data_array!(Int32Array);
 impl_series_like_for_data_array!(Int64Array);
+impl_series_like_for_data_array!(Int128Array);
 impl_series_like_for_data_array!(UInt8Array);
 impl_series_like_for_data_array!(UInt16Array);
 impl_series_like_for_data_array!(UInt32Array);
 impl_series_like_for_data_array!(UInt64Array);
 impl_series_like_for_data_array!(Float32Array);
 impl_series_like_for_data_array!(Float64Array);
 impl_series_like_for_data_array!(Utf8Array);
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/series/array_impl/logical_array.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/series/array_impl/logical_array.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 use crate::datatypes::logical::{
-    DateArray, DurationArray, EmbeddingArray, FixedShapeImageArray, ImageArray, TimestampArray,
+    DateArray, Decimal128Array, DurationArray, EmbeddingArray, FixedShapeImageArray,
+    FixedShapeTensorArray, ImageArray, TensorArray, TimestampArray,
 };
+use crate::datatypes::BooleanArray;
 
 use super::{ArrayWrapper, IntoSeries, Series};
 use crate::array::ops::GroupIndices;
 use crate::series::array_impl::binary_ops::SeriesBinaryOps;
 use crate::series::DaftResult;
 use crate::series::SeriesLike;
+use crate::with_match_daft_logical_primitive_types;
 use crate::with_match_integer_daft_types;
 use std::sync::Arc;
 
 macro_rules! impl_series_like_for_logical_array {
     ($da:ident) => {
         impl IntoSeries for $da {
             fn into_series(self) -> Series {
@@ -21,25 +24,43 @@
         }
 
         impl SeriesLike for ArrayWrapper<$da> {
             fn into_series(&self) -> Series {
                 self.0.clone().into_series()
             }
             fn to_arrow(&self) -> Box<dyn arrow2::array::Array> {
-                let arrow_logical_type = self.0.logical_type().to_arrow().unwrap();
+                let daft_type = self.0.logical_type();
+                let arrow_logical_type = daft_type.to_arrow().unwrap();
                 let physical_arrow_array = self.0.physical.data();
-                arrow2::compute::cast::cast(
-                    physical_arrow_array,
-                    &arrow_logical_type,
-                    arrow2::compute::cast::CastOptions {
-                        wrapped: true,
-                        partial: false,
-                    },
-                )
-                .unwrap()
+                use crate::datatypes::DataType::*;
+                match daft_type {
+                    // For wrapped primitive types, switch the datatype label on the arrow2 Array.
+                    Decimal128(..) | Date | Timestamp(..) | Duration(..) => {
+                        with_match_daft_logical_primitive_types!(daft_type, |$P| {
+                            use arrow2::array::Array;
+                            physical_arrow_array
+                                .as_any()
+                                .downcast_ref::<arrow2::array::PrimitiveArray<$P>>()
+                                .unwrap()
+                                .clone()
+                                .to(arrow_logical_type)
+                                .to_boxed()
+                        })
+                    }
+                    // Otherwise, use arrow cast to make sure the result arrow2 array is of the correct type.
+                    _ => arrow2::compute::cast::cast(
+                        physical_arrow_array,
+                        &arrow_logical_type,
+                        arrow2::compute::cast::CastOptions {
+                            wrapped: true,
+                            partial: false,
+                        },
+                    )
+                    .unwrap(),
+                }
             }
 
             fn as_any(&self) -> &dyn std::any::Any {
                 self
             }
 
             fn broadcast(&self, num: usize) -> DaftResult<Series> {
@@ -161,17 +182,47 @@
             fn div(&self, rhs: &Series) -> DaftResult<Series> {
                 SeriesBinaryOps::div(self, rhs)
             }
 
             fn rem(&self, rhs: &Series) -> DaftResult<Series> {
                 SeriesBinaryOps::rem(self, rhs)
             }
+            fn and(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+                SeriesBinaryOps::and(self, rhs)
+            }
+            fn or(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+                SeriesBinaryOps::or(self, rhs)
+            }
+            fn xor(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+                SeriesBinaryOps::xor(self, rhs)
+            }
+            fn equal(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+                SeriesBinaryOps::equal(self, rhs)
+            }
+            fn not_equal(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+                SeriesBinaryOps::not_equal(self, rhs)
+            }
+            fn lt(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+                SeriesBinaryOps::lt(self, rhs)
+            }
+            fn lte(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+                SeriesBinaryOps::lte(self, rhs)
+            }
+            fn gt(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+                SeriesBinaryOps::gt(self, rhs)
+            }
+            fn gte(&self, rhs: &Series) -> DaftResult<BooleanArray> {
+                SeriesBinaryOps::gte(self, rhs)
+            }
         }
     };
 }
 
+impl_series_like_for_logical_array!(Decimal128Array);
 impl_series_like_for_logical_array!(DateArray);
 impl_series_like_for_logical_array!(DurationArray);
 impl_series_like_for_logical_array!(EmbeddingArray);
 impl_series_like_for_logical_array!(ImageArray);
 impl_series_like_for_logical_array!(FixedShapeImageArray);
 impl_series_like_for_logical_array!(TimestampArray);
+impl_series_like_for_logical_array!(TensorArray);
+impl_series_like_for_logical_array!(FixedShapeTensorArray);
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/series/mod.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/abs.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/abs.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/agg.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/arithmetic.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/broadcast.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/broadcast.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/concat.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/concat.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/date.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/date.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/downcast.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/downcast.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use crate::datatypes::*;
 
-use crate::datatypes::logical::LogicalArray;
+use crate::datatypes::logical::{FixedShapeImageArray, ImageArray, LogicalArray};
 use crate::series::array_impl::ArrayWrapper;
 use crate::series::Series;
 use common_error::DaftResult;
 
 impl Series {
     pub fn downcast<T>(&self) -> DaftResult<&DataArray<T>>
     where
@@ -123,12 +123,20 @@
         self.downcast()
     }
 
     pub fn struct_(&self) -> DaftResult<&StructArray> {
         self.downcast()
     }
 
+    pub fn image(&self) -> DaftResult<&ImageArray> {
+        self.downcast_logical()
+    }
+
+    pub fn fixed_size_image(&self) -> DaftResult<&FixedShapeImageArray> {
+        self.downcast_logical()
+    }
+
     #[cfg(feature = "python")]
     pub fn python(&self) -> DaftResult<&PythonArray> {
         self.downcast()
     }
 }
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/filter.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/filter.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/image.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/image.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use crate::datatypes::{DataType, FixedShapeImageType, ImageFormat, ImageType};
+use crate::datatypes::{DataType, Field, FixedShapeImageType, ImageFormat, ImageType};
 
 use crate::series::{IntoSeries, Series};
 use common_error::{DaftError, DaftResult};
 
 impl Series {
     pub fn image_decode(&self) -> DaftResult<Series> {
         match self.data_type() {
@@ -51,8 +51,26 @@
             _ => Err(DaftError::ValueError(format!(
                 "datatype: {} does not support Image Resize. Occurred while resizing Series: {}",
                 self.data_type(),
                 self.name()
             ))),
         }
     }
+
+    pub fn image_crop(&self, bbox: &Series) -> DaftResult<Series> {
+        let bbox_type = DataType::FixedSizeList(Box::new(Field::new("bbox", DataType::UInt32)), 4);
+        let bbox = bbox.cast(&bbox_type)?;
+        let bbox = bbox.fixed_size_list()?;
+
+        match &self.data_type() {
+            DataType::Image(_) => self.image()?.crop(bbox).map(|arr| arr.into_series()),
+            DataType::FixedShapeImage(..) => self
+                .fixed_size_image()?
+                .crop(bbox)
+                .map(|arr| arr.into_series()),
+            dt => Err(DaftError::ValueError(format!(
+                "Expected input to crop to be an Image type, but received: {}",
+                dt
+            ))),
+        }
+    }
 }
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/list.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/list.rs`

 * *Files 6% similar despite different names*

```diff
@@ -14,21 +14,21 @@
             dt => Err(DaftError::TypeError(format!(
                 "explode not implemented for {}",
                 dt
             ))),
         }
     }
 
-    pub fn arr_lengths(&self) -> DaftResult<UInt64Array> {
+    pub fn list_lengths(&self) -> DaftResult<UInt64Array> {
         use DataType::*;
 
         match self.data_type() {
             List(_) => self.list()?.lengths(),
             FixedSizeList(..) => self.fixed_size_list()?.lengths(),
-            Embedding(..) | FixedShapeImage(..) => self.as_physical()?.arr_lengths(),
+            Embedding(..) | FixedShapeImage(..) => self.as_physical()?.list_lengths(),
             Image(..) => {
                 let struct_array = self.as_physical()?;
                 let data_array = struct_array.struct_()?.as_arrow().values()[0]
                     .as_any()
                     .downcast_ref::<arrow2::array::ListArray<i64>>()
                     .unwrap();
                 let offsets = data_array.offsets();
```

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/mod.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/search_sorted.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/sort.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/take.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/take.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/series/ops/utf8.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/series/ops/utf8.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/local_dependencies/daft-core/src/utils/arrow.rs` & `getdaft-0.1.9/local_dependencies/daft-core/src/utils/arrow.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/Cargo.toml` & `getdaft-0.1.9/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 [features]
 default = [ "python",]
-python = [ "dep:pyo3", "dep:pyo3-log", "daft-core/python", "daft-table/python", "daft-dsl/python", "daft-io/python",]
+python = [ "dep:pyo3", "dep:pyo3-log", "daft-core/python", "daft-table/python", "daft-dsl/python", "daft-io/python", "daft-parquet/python",]
 
 [lib]
 crate-type = [ "cdylib",]
 name = "daft"
 
 [package]
 edition = "2021"
 name = "daft"
 publish = false
-version = "0.1.8"
+version = "0.1.9"
 
 [workspace]
-members = ["local_dependencies/daft-core", "local_dependencies/daft-io", "local_dependencies/daft-dsl", "local_dependencies/daft-table"]
+members = ["local_dependencies/daft-core", "local_dependencies/daft-io", "local_dependencies/daft-parquet", "local_dependencies/daft-dsl", "local_dependencies/daft-table"]
 
 [dependencies.daft-core]
 path = "local_dependencies/daft-core"
 default-features = false
 
 [dependencies.daft-dsl]
 path = "local_dependencies/daft-dsl"
 default-features = false
 
 [dependencies.daft-io]
 path = "local_dependencies/daft-io"
 default-features = false
 
+[dependencies.daft-parquet]
+path = "local_dependencies/daft-parquet"
+default-features = false
+
 [dependencies.daft-table]
 path = "local_dependencies/daft-table"
 default-features = false
 
 [profile.dev]
 overflow-checks = false
 
@@ -46,28 +50,33 @@
 inherits = "release"
 lto = "fat"
 
 [profile.rust-analyzer]
 inherits = "dev"
 
 [workspace.dependencies]
+futures = "0.3.28"
 html-escape = "0.2.13"
 num-derive = "0.3.3"
 num-traits = "0.2"
 prettytable-rs = "0.10"
 rand = "^0.8"
-serde_json = "1.0.99"
+serde_json = "1.0.100"
+snafu = "0.7.4"
 
 [workspace.package]
 edition = "2021"
 version = "0.1.0"
 
+[workspace.dependencies.tokio]
+version = "1.29.1"
+features = [ "net", "time", "bytes", "process", "signal", "macros", "rt", "rt-multi-thread",]
+
 [workspace.dependencies.arrow2]
 branch = "clark/expand-casting-support"
-features = [ "chrono-tz", "compute_take", "compute_cast", "compute_aggregate", "compute_if_then_else", "compute_sort", "compute_filter", "compute_temporal", "compute_comparison", "compute_arithmetics", "compute_concatenate", "io_ipc",]
 git = "https://github.com/Eventual-Inc/arrow2"
 package = "arrow2"
 version = "0.17.1"
 
 [workspace.dependencies.bincode]
 version = "1.3.3"
 
@@ -76,19 +85,19 @@
 
 [workspace.dependencies.log]
 features = [ "std",]
 version = "0.4.19"
 
 [workspace.dependencies.pyo3]
 features = [ "extension-module", "abi3-py37",]
-version = "0.19.0"
+version = "0.19.1"
 
 [dependencies.pyo3]
 features = [ "extension-module", "abi3-py37",]
-version = "0.19.0"
+version = "0.19.1"
 optional = true
 
 [workspace.dependencies.pyo3-log]
 version = "0.8.2"
 
 [dependencies.pyo3-log]
 version = "0.8.2"
```

### Comparing `getdaft-0.1.8/.github/ISSUE_TEMPLATE/bug_report.md` & `getdaft-0.1.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/.github/ISSUE_TEMPLATE/feature_request.md` & `getdaft-0.1.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/.github/release-drafter.yml` & `getdaft-0.1.9/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/.github/workflows/broken-link-checker.yml` & `getdaft-0.1.9/.github/workflows/broken-link-checker.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/.github/workflows/daft-profiling.yml` & `getdaft-0.1.9/.github/workflows/daft-profiling.yml`

 * *Files 11% similar despite different names*

```diff
@@ -11,33 +11,26 @@
   TPCH_NUM_PARTS: '32'
   PYTHON_VERSION: '3.9'
 
 
 jobs:
   profile-daft:
     runs-on: ubuntu-latest
-    timeout-minutes: 20
+    timeout-minutes: 30
     strategy:
       fail-fast: false
     steps:
     - uses: actions/checkout@v3
     - uses: moonrepo/setup-rust@v0
-    - uses: actions/cache@v3
-      env:
-        cache-name: cache-cargo-profile
       with:
-        path: |
-          ~/.cargo/registry
-          ~/.cargo/git
-          target
-        key: ${{ runner.os }}-build-${{ env.cache-name }}-${{ hashFiles('**/Cargo.lock') }}
-        restore-keys: |
-          ${{ runner.os }}-build-${{ env.cache-name }}-
-          ${{ runner.os }}-build-
-          ${{ runner.os }}-
+        cache: false
+    - uses: Swatinem/rust-cache@v2
+      with:
+        key: ${{ runner.os }}-profile
+        cache-all-crates: 'true'
 
     - name: Set up Python ${{ env.PYTHON_VERSION }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ env.PYTHON_VERSION }}
 
     - name: Setup Virtual Env
```

### Comparing `getdaft-0.1.8/.github/workflows/notebook-checker.yml` & `getdaft-0.1.9/.github/workflows/notebook-checker.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/.github/workflows/property-based-tests.yml` & `getdaft-0.1.9/.github/workflows/property-based-tests.yml`

 * *Files 9% similar despite different names*

```diff
@@ -16,27 +16,20 @@
       fail-fast: false
       matrix:
         python-version: ['3.7']
         daft_runner: [py]
     steps:
     - uses: actions/checkout@v3
     - uses: moonrepo/setup-rust@v0
-    - uses: actions/cache@v3
-      env:
-        cache-name: cache-cargo
       with:
-        path: |
-          ~/.cargo/registry
-          ~/.cargo/git
-          target
-        key: ${{ runner.os }}-build-${{ env.cache-name }}-${{ hashFiles('**/Cargo.lock') }}
-        restore-keys: |
-          ${{ runner.os }}-build-${{ env.cache-name }}-
-          ${{ runner.os }}-build-
-          ${{ runner.os }}-
+        cache: false
+    - uses: Swatinem/rust-cache@v2
+      with:
+        key: ${{ runner.os }}-build
+        cache-all-crates: 'true'
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Setup Virtual Env
```

### Comparing `getdaft-0.1.8/.github/workflows/python-package.yml` & `getdaft-0.1.9/.github/workflows/python-package.yml`

 * *Files 14% similar despite different names*

```diff
@@ -28,29 +28,23 @@
         - daft-runner: py
           python-version: '3.10'
           pyarrow-version: 6.0.1
 
     steps:
     - uses: actions/checkout@v3
     - uses: moonrepo/setup-rust@v0
+      with:
+        cache: false
     - name: Install cargo-llvm-cov
       uses: taiki-e/install-action@cargo-llvm-cov
-    - uses: actions/cache@v3
-      env:
-        cache-name: cache-cargo
+    - uses: Swatinem/rust-cache@v2
       with:
-        path: |
-          ~/.cargo/registry
-          ~/.cargo/git
-          target
-        key: ${{ runner.os }}-build-${{ env.cache-name }}-${{ hashFiles('**/Cargo.lock') }}
-        restore-keys: |
-          ${{ runner.os }}-build-${{ env.cache-name }}-
-          ${{ runner.os }}-build-
-          ${{ runner.os }}-
+        key: ${{ runner.os }}-build
+        cache-all-crates: 'true'
+
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Setup Virtual Env
       run: |
@@ -122,29 +116,22 @@
         fetch-depth: 0
     - uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
         architecture: x64
     - run: pip install -U twine toml maturin
     - run: python tools/patch_package_version.py
-    - name: Install Rust toolchain
-      uses: moonrepo/setup-rust@v0
-    - uses: actions/cache@v3
-      env:
-        cache-name: cache-cargo
+    - uses: moonrepo/setup-rust@v0
+      with:
+        cache: false
+    - uses: Swatinem/rust-cache@v2
       with:
-        path: |
-          ~/.cargo/registry
-          ~/.cargo/git
-          target
-        key: ${{ runner.os }}-integration-build-${{ env.cache-name }}-${{ hashFiles('**/Cargo.lock') }}
-        restore-keys: |
-          ${{ runner.os }}-integration-build-${{ env.cache-name }}-
-          ${{ runner.os }}-integration-build-
-          ${{ runner.os }}-
+        key: ${{ runner.os }}-integration-build
+        cache-all-crates: 'true'
+
     # NOTE: we don't build with all the actual release optimizations to avoid hellish CI times
     - name: Build wheels
       run: maturin build --release --compatibility linux --out dist
     - name: Upload wheels
       uses: actions/upload-artifact@v3
       with:
         name: wheels
@@ -289,27 +276,21 @@
     runs-on: ubuntu-latest
     timeout-minutes: 15
     strategy:
       fail-fast: false
     steps:
     - uses: actions/checkout@v3
     - uses: moonrepo/setup-rust@v0
-    - uses: actions/cache@v3
-      env:
-        cache-name: cache-cargo
       with:
-        path: |
-          ~/.cargo/registry
-          ~/.cargo/git
-          target
-        key: ${{ runner.os }}-rust-package-${{ env.cache-name }}-${{ hashFiles('**/Cargo.lock') }}
-        restore-keys: |
-          ${{ runner.os }}-rust-package-${{ env.cache-name }}-
-          ${{ runner.os }}-rust-package-
-          ${{ runner.os }}-
+        cache: false
+    - uses: Swatinem/rust-cache@v2
+      with:
+        key: ${{ runner.os }}-rust-build
+        cache-all-crates: 'true'
+
     - name: Install cargo-llvm-cov
       uses: taiki-e/install-action@cargo-llvm-cov
     - name: Generate code coverage
       run: mkdir -p report-output && cargo llvm-cov --no-default-features --workspace --lcov --output-path ./report-output/lcov.info
     - name: Upload coverage report
       uses: actions/upload-artifact@v3
       with:
@@ -379,27 +360,20 @@
       fail-fast: false
       matrix:
         python-version: ['3.7']
 
     steps:
     - uses: actions/checkout@v3
     - uses: moonrepo/setup-rust@v0
-    - uses: actions/cache@v3
-      env:
-        cache-name: cache-cargo
       with:
-        path: |
-          ~/.cargo/registry
-          ~/.cargo/git
-          target
-        key: ${{ runner.os }}-build-${{ env.cache-name }}-${{ hashFiles('**/Cargo.lock') }}
-        restore-keys: |
-          ${{ runner.os }}-build-${{ env.cache-name }}-
-          ${{ runner.os }}-build-
-          ${{ runner.os }}-
+        cache: false
+    - uses: Swatinem/rust-cache@v2
+      with:
+        key: ${{ runner.os }}-build
+        cache-all-crates: 'true'
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Setup Virtual Env
@@ -455,29 +429,21 @@
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install pre-commit
       run: |
         pip install --upgrade pip
         pip install pre-commit
-
     - uses: moonrepo/setup-rust@v0
-    - uses: actions/cache@v3
-      env:
-        cache-name: cache-cargo
       with:
-        path: |
-          ~/.cargo/registry
-          ~/.cargo/git
-          target
-        key: ${{ runner.os }}-build-${{ env.cache-name }}-${{ hashFiles('**/Cargo.lock') }}
-        restore-keys: |
-          ${{ runner.os }}-build-${{ env.cache-name }}-
-          ${{ runner.os }}-build-
-          ${{ runner.os }}-
+        cache: false
+    - uses: Swatinem/rust-cache@v2
+      with:
+        key: ${{ runner.os }}-build
+        cache-all-crates: 'true'
 
     - uses: actions/cache@v3
       id: pre-commit-cache
       with:
         path: ~/.cache/pre-commit/
         key: ${{ runner.os }}-python-${{ steps.setup-python.outputs.python-version }}-pre-commit-${{ hashFiles('.pre-commit-config.yaml') }}
     - name: Python And Rust Style Check
```

### Comparing `getdaft-0.1.8/.github/workflows/python-publish.yml` & `getdaft-0.1.9/.github/workflows/python-publish.yml`

 * *Files 4% similar despite different names*

```diff
@@ -41,17 +41,15 @@
         fetch-depth: 0
     - uses: actions/setup-python@v4
       with:
         python-version: ${{ env.PYTHON_VERSION }}
         architecture: x64
     - run: pip install -U twine toml
     - run: python tools/patch_package_version.py
-    - name: Install Rust toolchain
-      uses: moonrepo/setup-rust@v0
-
+    - uses: moonrepo/setup-rust@v0
     - name: Build wheels - x86
       if: ${{ matrix.compile_arch == 'x86_64' }}
       uses: messense/maturin-action@v1
       with:
         target: x86_64
         manylinux: auto
         args: --profile release-lto --out dist --sdist
```

### Comparing `getdaft-0.1.8/.github/workflows/ray-compatibility.yml` & `getdaft-0.1.9/.github/workflows/ray-compatibility.yml`

 * *Files 10% similar despite different names*

```diff
@@ -14,32 +14,25 @@
   build:
     runs-on: ubuntu-latest
     timeout-minutes: 15
     strategy:
       fail-fast: false
       matrix:
         python-version: ['3.9']
-        ray-version: [2.3.0, 2.2.0, 2.1.0, 2.0.0]
+        ray-version: [2.5.1, 2.4.0, 2.3.0, 2.2.0, 2.1.0, 2.0.0]
 
     steps:
     - uses: actions/checkout@v3
     - uses: moonrepo/setup-rust@v0
-    - uses: actions/cache@v3
-      env:
-        cache-name: cache-cargo
       with:
-        path: |
-          ~/.cargo/registry
-          ~/.cargo/git
-          target
-        key: ${{ runner.os }}-build-${{ env.cache-name }}-${{ hashFiles('**/Cargo.lock') }}
-        restore-keys: |
-          ${{ runner.os }}-build-${{ env.cache-name }}-
-          ${{ runner.os }}-build-
-          ${{ runner.os }}-
+        cache: false
+    - uses: Swatinem/rust-cache@v2
+      with:
+        key: ${{ runner.os }}-build
+        cache-all-crates: 'true'
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Setup Virtual Env
```

### Comparing `getdaft-0.1.8/.github/workflows/release-drafter.yml` & `getdaft-0.1.9/.github/workflows/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/.pre-commit-config.yaml` & `getdaft-0.1.9/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -16,14 +16,19 @@
   - id: trailing-whitespace
     exclude: docs/source/api_docs/
   - id: end-of-file-fixer
     exclude: docs/source/api_docs/
   - id: check-yaml
     exclude: kubernetes-ops
   - id: pretty-format-json
+    exclude: |
+      (?x)^(
+          tutorials/.*\.ipynb|
+          docs/.*\.ipynb
+      )$
     args:
     - --autofix
     - --no-sort-keys
     - '--indent=  '
   - id: check-added-large-files
   - id: check-merge-conflict
   - id: check-docstring-first
@@ -65,23 +70,50 @@
     args: [--in-place, --remove-all-unused-imports, --remove-unused-variable, --ignore-init-module-imports]
 
 - repo: https://github.com/psf/black
   rev: 22.12.0
   hooks:
   - id: black
 
-- repo: https://github.com/doublify/pre-commit-rust
-  rev: v1.0
+- repo: local
   hooks:
   - id: fmt
+    name: fmt
+    description: Format files with cargo fmt.
+    entry: cargo fmt
+    language: system
+    types: [rust]
+    args: [--]
   - id: cargo-check
-    args: [--profile, rust-analyzer]
-  - id: cargo-check
-    name: cargo check --no-default-features
-    args: [--no-default-features, --profile, rust-analyzer]
+    name: cargo check
+    description: Check the package for errors.
+    entry: cargo check
+    language: system
+    types: [rust]
+    pass_filenames: false
+    args: [--workspace]
+
+  - id: cargo-check-no-default
+    name: cargo check
+    description: Check the package for errors without default features.
+    entry: cargo check
+    language: system
+    types: [rust]
+    pass_filenames: false
+    args: [--workspace, --no-default-features]
+
+
   - id: clippy
-    args: [--profile, rust-analyzer]
+    name: clippy
+    description: Lint rust sources
+    entry: cargo clippy
+    language: system
+    args: [--workspace, --, -D, warnings]
+    types: [rust]
+    pass_filenames: false
+
+
 
 - repo: https://github.com/abravalheri/validate-pyproject
   rev: v0.10.1
   hooks:
   - id: validate-pyproject
```

### Comparing `getdaft-0.1.8/CONTRIBUTING.md` & `getdaft-0.1.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/LICENSE` & `getdaft-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/Makefile` & `getdaft-0.1.9/Makefile`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/README.rst` & `getdaft-0.1.9/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
   Check out our `10-minute quickstart <https://www.getdaft.io/projects/docs/en/latest/learn/10-min.html>`_!
 
 In this example, we load images from an AWS S3 bucket's URLs and resize each image in the dataframe:
 
 .. code:: python
 
-    import daft as daft
+    import daft
 
     # Load a dataframe from filepaths in an S3 bucket
     df = daft.from_glob_path("s3://daft-public-data/laion-sample-images/*")
 
     # 1. Download column of image URLs as a column of bytes
     # 2. Decode the column of bytes into a column of images
     df = df.with_column("image", df["path"].url.download().image.decode())
```

### Comparing `getdaft-0.1.8/benchmarking/tpch/__main__.py` & `getdaft-0.1.9/benchmarking/tpch/__main__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/benchmarking/tpch/answers.py` & `getdaft-0.1.9/benchmarking/tpch/answers.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/benchmarking/tpch/data_generation.py` & `getdaft-0.1.9/benchmarking/tpch/data_generation.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/benchmarking/tpch/pipelined_data_generation.py` & `getdaft-0.1.9/benchmarking/tpch/pipelined_data_generation.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/benchmarking/tpch/subprefix_s3_files.py` & `getdaft-0.1.9/benchmarking/tpch/subprefix_s3_files.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/ci/upload_wheels.sh` & `getdaft-0.1.9/ci/upload_wheels.sh`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/__init__.py` & `getdaft-0.1.9/daft/__init__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/analytics.py` & `getdaft-0.1.9/daft/analytics.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/api_annotations.py` & `getdaft-0.1.9/daft/api_annotations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/arrow_utils.py` & `getdaft-0.1.9/daft/arrow_utils.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/context.py` & `getdaft-0.1.9/daft/context.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/convert.py` & `getdaft-0.1.9/daft/convert.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/daft.pyi` & `getdaft-0.1.9/daft/daft.pyi`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/dataframe/dataframe.py` & `getdaft-0.1.9/daft/dataframe/dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1063,47 +1063,49 @@
             "Cannot call len() on an unmaterialized dataframe:"
             " either materialize your dataframe with df.collect() first before calling len(),"
             " or use `df.count_rows()` instead which will calculate the total number of rows."
         )
         raise RuntimeError(message)
 
     @DataframePublicAPI
-    def to_pandas(self) -> "pd.DataFrame":
+    def to_pandas(self, cast_tensors_to_ray_tensor_dtype: bool = False) -> "pd.DataFrame":
         """Converts the current DataFrame to a pandas DataFrame.
         If results have not computed yet, collect will be called.
 
         Returns:
             pd.DataFrame: pandas DataFrame converted from a Daft DataFrame
 
             .. NOTE::
                 This call is **blocking** and will execute the DataFrame when called
         """
         self.collect()
         result = self._result
         assert result is not None
 
-        pd_df = result.to_pandas(schema=self._plan.schema())
+        pd_df = result.to_pandas(
+            schema=self._plan.schema(), cast_tensors_to_ray_tensor_dtype=cast_tensors_to_ray_tensor_dtype
+        )
         return pd_df
 
     @DataframePublicAPI
-    def to_arrow(self) -> "pa.Table":
+    def to_arrow(self, cast_tensors_to_ray_tensor_dtype: bool = False) -> "pa.Table":
         """Converts the current DataFrame to a pyarrow Table.
         If results have not computed yet, collect will be called.
 
         Returns:
             pyarrow.Table: pyarrow Table converted from a Daft DataFrame
 
             .. NOTE::
                 This call is **blocking** and will execute the DataFrame when called
         """
         self.collect()
         result = self._result
         assert result is not None
 
-        return result.to_arrow()
+        return result.to_arrow(cast_tensors_to_ray_tensor_dtype)
 
     @DataframePublicAPI
     def to_pydict(self) -> Dict[str, List[Any]]:
         """Converts the current DataFrame to a python dictionary. The dictionary contains Python lists of Python objects for each column.
 
         If results have not computed yet, collect will be called.
```

### Comparing `getdaft-0.1.8/daft/dataframe/to_torch.py` & `getdaft-0.1.9/daft/dataframe/to_torch.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/datasources.py` & `getdaft-0.1.9/daft/datasources.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/datatype.py` & `getdaft-0.1.9/daft/datatype.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from __future__ import annotations
 
 import builtins
+from typing import TYPE_CHECKING
 
 import pyarrow as pa
 
 from daft.context import get_context
 from daft.daft import ImageMode, PyDataType, PyTimeUnit
 
+if TYPE_CHECKING:
+    import numpy as np
+
 _RAY_DATA_EXTENSIONS_AVAILABLE = True
 _TENSOR_EXTENSION_TYPES = []
 try:
     import ray
 except ImportError:
     _RAY_DATA_EXTENSIONS_AVAILABLE = False
 else:
@@ -176,14 +180,19 @@
 
     @classmethod
     def null(cls) -> DataType:
         """Creates the Null DataType: Always the ``Null`` value"""
         return cls._from_pydatatype(PyDataType.null())
 
     @classmethod
+    def decimal128(cls, precision: int, scale: int) -> DataType:
+        """Fixed-precision decimal."""
+        return cls._from_pydatatype(PyDataType.decimal128(precision, scale))
+
+    @classmethod
     def date(cls) -> DataType:
         """Create a Date DataType: A date with a year, month and day"""
         return cls._from_pydatatype(PyDataType.date())
 
     @classmethod
     def timestamp(cls, timeunit: TimeUnit, timezone: str | None = None) -> DataType:
         """Timestamp DataType."""
@@ -280,14 +289,38 @@
         elif height is not None or width is not None:
             raise ValueError(
                 f"Image height and width must either both be specified, or both not be specified, but got height={height}, width={width}"
             )
         return cls._from_pydatatype(PyDataType.image(mode, height, width))
 
     @classmethod
+    def tensor(
+        cls,
+        dtype: DataType,
+        shape: tuple[int, ...] | None = None,
+    ) -> DataType:
+        """Create a tensor DataType: tensor arrays contain n-dimensional arrays of data of the provided ``dtype`` as elements, each of the provided
+        ``shape``.
+
+        If a ``shape`` is given, each ndarray in the column will have this shape.
+
+        If ``shape`` is not given, the ndarrays in the column can have different shapes. This is much more flexible,
+        but will result in a less compact representation and may be make some operations less efficient.
+
+        Args:
+            dtype: The type of the data contained within the tensor elements.
+            shape: The shape of each tensor in the column. This is ``None`` by default, which allows the shapes of
+                each tensor element to vary.
+        """
+        if shape is not None:
+            if not isinstance(shape, tuple) or not shape or any(not isinstance(n, int) for n in shape):
+                raise ValueError("Tensor shape must be a non-empty tuple of ints, but got: ", shape)
+        return cls._from_pydatatype(PyDataType.tensor(dtype._dtype, shape))
+
+    @classmethod
     def from_arrow_type(cls, arrow_type: pa.lib.DataType) -> DataType:
         """Maps a PyArrow DataType to a Daft DataType"""
         if pa.types.is_int8(arrow_type):
             return cls.int8()
         elif pa.types.is_int16(arrow_type):
             return cls.int16()
         elif pa.types.is_int32(arrow_type):
@@ -310,14 +343,16 @@
             return cls.string()
         elif pa.types.is_binary(arrow_type) or pa.types.is_large_binary(arrow_type):
             return cls.binary()
         elif pa.types.is_boolean(arrow_type):
             return cls.bool()
         elif pa.types.is_null(arrow_type):
             return cls.null()
+        elif pa.types.is_decimal128(arrow_type):
+            return cls.decimal128(arrow_type.precision, arrow_type.scale)
         elif pa.types.is_date32(arrow_type):
             return cls.date()
         elif pa.types.is_timestamp(arrow_type):
             timeunit = TimeUnit.from_str(arrow_type.unit)
             return cls.timestamp(timeunit=timeunit, timezone=arrow_type.tz)
         elif pa.types.is_duration(arrow_type):
             timeunit = TimeUnit.from_str(arrow_type.unit)
@@ -331,16 +366,20 @@
             field = arrow_type.value_field
             return cls.fixed_size_list(field.name, cls.from_arrow_type(field.type), arrow_type.list_size)
         elif pa.types.is_struct(arrow_type):
             assert isinstance(arrow_type, pa.StructType)
             fields = [arrow_type[i] for i in range(arrow_type.num_fields)]
             return cls.struct({field.name: cls.from_arrow_type(field.type) for field in fields})
         elif _RAY_DATA_EXTENSIONS_AVAILABLE and isinstance(arrow_type, tuple(_TENSOR_EXTENSION_TYPES)):
-            # TODO(Clark): Add a native cross-lang extension type representation for Ray's tensor extension types.
-            return cls.python()
+            scalar_dtype = cls.from_arrow_type(arrow_type.scalar_type)
+            shape = arrow_type.shape if isinstance(arrow_type, ArrowTensorType) else None
+            return cls.tensor(scalar_dtype, shape)
+        elif isinstance(arrow_type, getattr(pa, "FixedShapeTensorType", ())):
+            scalar_dtype = cls.from_arrow_type(arrow_type.value_type)
+            return cls.tensor(scalar_dtype, tuple(arrow_type.shape))
         elif isinstance(arrow_type, pa.PyExtensionType):
             # TODO(Clark): Add a native cross-lang extension type representation for PyExtensionTypes.
             raise ValueError(
                 "pyarrow extension types that subclass pa.PyExtensionType can't be used in Daft, since they can't be "
                 f"used in non-Python Arrow implementations and Daft uses the Rust Arrow2 implementation: {arrow_type}"
             )
         elif isinstance(arrow_type, pa.BaseExtensionType):
@@ -355,42 +394,62 @@
                     "For more details see this issue: "
                     "https://github.com/apache/arrow/issues/35599"
                 )
             try:
                 metadata = arrow_type.__arrow_ext_serialize__().decode()
             except AttributeError:
                 metadata = None
-            return cls.extension(
-                name,
-                cls.from_arrow_type(arrow_type.storage_type),
-                metadata,
-            )
+
+            if name == "daft.super_extension":
+                assert metadata is not None
+                return cls._from_pydatatype(PyDataType.from_json(metadata))
+            else:
+                return cls.extension(
+                    name,
+                    cls.from_arrow_type(arrow_type.storage_type),
+                    metadata,
+                )
         else:
             # Fall back to a Python object type.
             # TODO(Clark): Add native support for remaining Arrow types.
             return cls.python()
 
     @classmethod
-    def from_numpy_dtype(cls, np_type) -> DataType:
+    def from_numpy_dtype(cls, np_type: np.dtype) -> DataType:
         """Maps a Numpy datatype to a Daft DataType"""
         arrow_type = pa.from_numpy_dtype(np_type)
         return cls.from_arrow_type(arrow_type)
 
+    def to_arrow_dtype(self, cast_tensor_to_ray_type: builtins.bool = False) -> pa.DataType:
+        return self._dtype.to_arrow(cast_tensor_to_ray_type)
+
     @classmethod
     def python(cls) -> DataType:
         """Create a Python DataType: a type which refers to an arbitrary Python object"""
         return cls._from_pydatatype(PyDataType.python())
 
     def _is_python_type(self) -> builtins.bool:
         # NOTE: This is currently used in a few places still. We can get rid of it once these are refactored away. To be discussed.
         # 1. Visualizations - we can get rid of it if we do all our repr and repr_html logic in a Series instead of in Python
         # 2. Hypothesis test data generation - we can get rid of it if we allow for creation of Series from a Python list and DataType
 
         return self == DataType.python()
 
+    def _is_tensor_type(self) -> builtins.bool:
+        return self._dtype.is_tensor()
+
+    def _is_fixed_shape_tensor_type(self) -> builtins.bool:
+        return self._dtype.is_fixed_shape_tensor()
+
+    def _is_image_type(self) -> builtins.bool:
+        return self._dtype.is_image()
+
+    def _is_fixed_shape_image_type(self) -> builtins.bool:
+        return self._dtype.is_fixed_shape_image()
+
     def _is_logical_type(self) -> builtins.bool:
         return self._dtype.is_logical()
 
     def __repr__(self) -> str:
         return self._dtype.__repr__()
 
     def __eq__(self, other: object) -> builtins.bool:
```

### Comparing `getdaft-0.1.8/daft/execution/execution_step.py` & `getdaft-0.1.9/daft/execution/execution_step.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/execution/physical_plan.py` & `getdaft-0.1.9/daft/execution/physical_plan.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/execution/physical_plan_factory.py` & `getdaft-0.1.9/daft/execution/physical_plan_factory.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/expressions/expressions.py` & `getdaft-0.1.9/daft/expressions/expressions.py`

 * *Files 4% similar despite different names*

```diff
@@ -610,14 +610,22 @@
 
         Returns:
             Expression: a String expression which is every element of the list joined on the delimiter
         """
         delimiter_expr = Expression._to_expression(delimiter)
         return Expression._from_pyexpr(self._expr.list_join(delimiter_expr._expr))
 
+    def lengths(self) -> Expression:
+        """Gets the length of each list
+
+        Returns:
+            Expression: a UInt64 expression which is the length of each list
+        """
+        return Expression._from_pyexpr(self._expr.list_lengths())
+
 
 class ExpressionsProjection(Iterable[Expression]):
     """A collection of Expressions that can be projected onto a Table to produce another Table
 
     Invariants:
         1. All Expressions have names
         2. All Expressions have unique names
@@ -764,7 +772,28 @@
             Expression: An Image expression representing an image column of the resized images.
         """
         if not isinstance(w, int):
             raise TypeError(f"expected int for w but got {type(w)}")
         if not isinstance(h, int):
             raise TypeError(f"expected int for h but got {type(h)}")
         return Expression._from_pyexpr(self._expr.image_resize(w, h))
+
+    def crop(self, bbox: tuple[int, int, int, int] | Expression) -> Expression:
+        """
+        Crops images with the provided bounding box
+
+        Args:
+            bbox (tuple[float, float, float, float] | Expression): Either a tuple of (x, y, width, height)
+                parameters for cropping, or a List Expression where each element is a length 4 List
+                which represents the bounding box for the crop
+
+        Returns:
+            Expression: An Image expression representing the cropped image
+        """
+        if not isinstance(bbox, Expression):
+            if len(bbox) != 4 or not all([isinstance(x, int) for x in bbox]):
+                raise ValueError(
+                    f"Expected `bbox` to be either a tuple of 4 ints or an Expression but received: {bbox}"
+                )
+            bbox = Expression._to_expression(bbox).cast(DataType.fixed_size_list("", DataType.uint64(), 4))
+        assert isinstance(bbox, Expression)
+        return Expression._from_pyexpr(self._expr.image_crop(bbox._expr))
```

### Comparing `getdaft-0.1.8/daft/expressions/testing.py` & `getdaft-0.1.9/daft/expressions/testing.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/filesystem.py` & `getdaft-0.1.9/daft/filesystem.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/internal/rule.py` & `getdaft-0.1.9/daft/internal/rule.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/internal/rule_runner.py` & `getdaft-0.1.9/daft/internal/rule_runner.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/internal/treenode.py` & `getdaft-0.1.9/daft/internal/treenode.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/io/_csv.py` & `getdaft-0.1.9/daft/io/_csv.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/io/_json.py` & `getdaft-0.1.9/daft/io/_json.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/io/common.py` & `getdaft-0.1.9/daft/io/common.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/io/file_path.py` & `getdaft-0.1.9/daft/io/file_path.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/io/parquet.py` & `getdaft-0.1.9/daft/io/parquet.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/logical/aggregation_plan_builder.py` & `getdaft-0.1.9/daft/logical/aggregation_plan_builder.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/logical/logical_plan.py` & `getdaft-0.1.9/daft/logical/logical_plan.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/logical/map_partition_ops.py` & `getdaft-0.1.9/daft/logical/map_partition_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/logical/optimizer.py` & `getdaft-0.1.9/daft/logical/optimizer.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/logical/schema.py` & `getdaft-0.1.9/daft/logical/schema.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/pickle/cloudpickle.py` & `getdaft-0.1.9/daft/pickle/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/pickle/cloudpickle_fast.py` & `getdaft-0.1.9/daft/pickle/cloudpickle_fast.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/pickle/compat.py` & `getdaft-0.1.9/daft/pickle/compat.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/resource_request.py` & `getdaft-0.1.9/daft/resource_request.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/runners/partitioning.py` & `getdaft-0.1.9/daft/runners/partitioning.py`

 * *Files 12% similar despite different names*

```diff
@@ -70,21 +70,23 @@
         raise NotImplementedError()
 
     def to_pydict(self) -> dict[str, list[Any]]:
         """Retrieves all the data in a PartitionSet as a Python dictionary. Values are the raw data from each Block."""
         merged_partition = self._get_merged_vpartition()
         return merged_partition.to_pydict()
 
-    def to_pandas(self, schema: Schema | None = None) -> pd.DataFrame:
+    def to_pandas(self, schema: Schema | None = None, cast_tensors_to_ray_tensor_dtype: bool = False) -> pd.DataFrame:
         merged_partition = self._get_merged_vpartition()
-        return merged_partition.to_pandas(schema=schema)
+        return merged_partition.to_pandas(
+            schema=schema, cast_tensors_to_ray_tensor_dtype=cast_tensors_to_ray_tensor_dtype
+        )
 
-    def to_arrow(self) -> pa.Table:
+    def to_arrow(self, cast_tensors_to_ray_tensor_dtype: bool = False) -> pa.Table:
         merged_partition = self._get_merged_vpartition()
-        return merged_partition.to_arrow()
+        return merged_partition.to_arrow(cast_tensors_to_ray_tensor_dtype)
 
     def items(self) -> list[tuple[PartID, PartitionT]]:
         """
         Returns all (partition id, partition) in this PartitionSet,
         ordered by partition ID.
         """
         raise NotImplementedError()
```

### Comparing `getdaft-0.1.8/daft/runners/profiler.py` & `getdaft-0.1.9/daft/runners/profiler.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/runners/pyrunner.py` & `getdaft-0.1.9/daft/runners/pyrunner.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/runners/ray_runner.py` & `getdaft-0.1.9/daft/runners/ray_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
     return partition_refs
 
 
 @ray.remote
 def _make_ray_block_from_vpartition(partition: Table) -> RayDatasetBlock:
     try:
-        return partition.to_arrow()
+        return partition.to_arrow(cast_tensors_to_ray_tensor_dtype=True)
     except pa.ArrowInvalid:
         return partition.to_pylist()
 
 
 @ray.remote
 def _make_daft_partition_from_ray_dataset_blocks(ray_dataset_block: pa.Table, daft_schema: Schema) -> Table:
     return Table.from_arrow(ray_dataset_block)
@@ -281,14 +281,18 @@
                 lambda x: x,
                 batch_size=None,
                 batch_format="pyarrow",
                 **extra_kwargs,
             )
             arrow_schema = ds.schema(fetch_if_missing=True)
 
+            # Ray 2.5.0 broke the API by using its own `ray.data.dataset.Schema` instead of PyArrow schemas
+            if RAY_VERSION >= (2, 5, 0):
+                arrow_schema = pa.schema({name: t for name, t in zip(arrow_schema.names, arrow_schema.types)})
+
         daft_schema = Schema._from_field_name_and_types(
             [(arrow_field.name, DataType.from_arrow_type(arrow_field.type)) for arrow_field in arrow_schema]
         )
         block_refs = ds.get_internal_block_refs()
 
         # NOTE: This materializes the entire Ray Dataset - we could make this more intelligent by creating a new RayDatasetScan node
         # which can iterate on Ray Dataset blocks and materialize as-needed
@@ -463,25 +467,22 @@
             f"{datetime.replace(datetime.now(), second=0, microsecond=0).isoformat()[:-3]}.json"
         )
         with profiler(profile_filename):
             try:
                 next_step = next(phys_plan)
 
                 while True:  # Loop: Dispatch -> await.
-
                     while True:  # Loop: Dispatch (get tasks -> batch dispatch).
-
                         tasks_to_dispatch: list[PartitionTask] = []
 
                         dispatches_allowed = max_inflight_tasks - len(inflight_tasks)
                         dispatches_allowed = min(cores, dispatches_allowed)
 
                         # Loop: Get a batch of tasks.
                         while len(tasks_to_dispatch) < dispatches_allowed:
-
                             if next_step is None:
                                 # Blocked on already dispatched tasks; await some tasks.
                                 break
 
                             elif isinstance(next_step, ray.ObjectRef):
                                 # A final result.
                                 self.results_by_df[result_uuid].put(next_step)
```

### Comparing `getdaft-0.1.8/daft/runners/runner.py` & `getdaft-0.1.9/daft/runners/runner.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/runners/runner_io.py` & `getdaft-0.1.9/daft/runners/runner_io.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/series.py` & `getdaft-0.1.9/daft/series.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,27 +3,40 @@
 from typing import TypeVar
 
 import pyarrow as pa
 
 from daft.arrow_utils import ensure_array, ensure_chunked_array
 from daft.daft import ImageFormat, PySeries
 from daft.datatype import DataType
+from daft.utils import pyarrow_supports_fixed_shape_tensor
+
+_RAY_DATA_EXTENSIONS_AVAILABLE = True
+try:
+    from ray.data.extensions import (
+        ArrowTensorArray,
+        ArrowTensorType,
+        ArrowVariableShapedTensorType,
+    )
+except ImportError:
+    _RAY_DATA_EXTENSIONS_AVAILABLE = False
 
 _NUMPY_AVAILABLE = True
 try:
     import numpy as np
 except ImportError:
     _NUMPY_AVAILABLE = False
 
 _PANDAS_AVAILABLE = True
 try:
     import pandas as pd
 except ImportError:
     _PANDAS_AVAILABLE = False
 
+ARROW_VERSION = tuple(int(s) for s in pa.__version__.split(".") if s.isnumeric())
+
 
 class Series:
     """
     A Daft Series is an array of data of a single type, and is usually a column in a DataFrame.
     """
 
     _series: PySeries
@@ -47,27 +60,39 @@
             name: The name associated with the Series; this is usually the column name.
         """
         if DataType.from_arrow_type(array.type) == DataType.python():
             # If the Arrow type is not natively supported, go through the Python list path.
             return Series.from_pylist(array.to_pylist(), name=name, pyobj="force")
         elif isinstance(array, pa.Array):
             array = ensure_array(array)
-            pys = PySeries.from_arrow(name, array)
-            return Series._from_pyseries(pys)
+            if _RAY_DATA_EXTENSIONS_AVAILABLE and isinstance(array.type, ArrowTensorType):
+                storage_series = Series.from_arrow(array.storage, name=name)
+                series = storage_series.cast(
+                    DataType.fixed_size_list(
+                        "item", DataType.from_arrow_type(array.type.scalar_type), int(np.prod(array.type.shape))
+                    )
+                )
+                return series.cast(DataType.from_arrow_type(array.type))
+            elif _RAY_DATA_EXTENSIONS_AVAILABLE and isinstance(array.type, ArrowVariableShapedTensorType):
+                return Series.from_numpy(array.to_numpy(zero_copy_only=False), name=name)
+            elif isinstance(array.type, getattr(pa, "FixedShapeTensorType", ())):
+                series = Series.from_arrow(array.storage, name=name)
+                return series.cast(DataType.from_arrow_type(array.type))
+            else:
+                pys = PySeries.from_arrow(name, array)
+                return Series._from_pyseries(pys)
         elif isinstance(array, pa.ChunkedArray):
             array = ensure_chunked_array(array)
             arr_type = array.type
             if isinstance(arr_type, pa.BaseExtensionType):
                 combined_storage_array = array.cast(arr_type.storage_type).combine_chunks()
                 combined_array = arr_type.wrap_array(combined_storage_array)
             else:
                 combined_array = array.combine_chunks()
-
-            pys = PySeries.from_arrow(name, combined_array)
-            return Series._from_pyseries(pys)
+            return Series.from_arrow(combined_array)
         else:
             raise TypeError(f"expected either PyArrow Array or Chunked Array, got {type(array)}")
 
     @staticmethod
     def from_pylist(data: list, name: str = "list_series", pyobj: str = "allow") -> Series:
         """Construct a Series from a Python list.
 
@@ -124,15 +149,15 @@
             except pa.ArrowInvalid:
                 pass
             else:
                 return cls.from_arrow(arrow_array, name=name)
         # TODO(Clark): Represent the tensor series with an Arrow extension type in order
         # to keep the series data contiguous.
         list_ndarray = [np.asarray(item) for item in data]
-        return cls.from_pylist(list_ndarray, name=name, pyobj="force")
+        return cls.from_pylist(list_ndarray, name=name, pyobj="allow")
 
     @classmethod
     def from_pandas(cls, data: pd.Series, name: str = "pd_series") -> Series:
         """
         Construct a Series from a pandas Series.
 
         This will first try to convert the series into a pyarrow array, then will fall
@@ -212,19 +237,45 @@
 
     def rename(self, name: str) -> Series:
         return Series._from_pyseries(self._series.rename(name))
 
     def datatype(self) -> DataType:
         return DataType._from_pydatatype(self._series.data_type())
 
-    def to_arrow(self) -> pa.Array:
+    def to_arrow(self, cast_tensors_to_ray_tensor_dtype: bool = False) -> pa.Array:
         """
         Convert this Series to an pyarrow array.
         """
-        return self._series.to_arrow()
+        dtype = self.datatype()
+        if cast_tensors_to_ray_tensor_dtype and (dtype._is_tensor_type() or dtype._is_fixed_shape_tensor_type()):
+            if not _RAY_DATA_EXTENSIONS_AVAILABLE:
+                raise ValueError("Trying to convert tensors to Ray tensor dtypes, but Ray is not installed.")
+            pyarrow_dtype = dtype.to_arrow_dtype(cast_tensor_to_ray_type=True)
+            if isinstance(pyarrow_dtype, ArrowTensorType):
+                assert dtype._is_fixed_shape_tensor_type()
+                arrow_series = self._series.to_arrow()
+                storage = arrow_series.storage
+                list_size = storage.type.list_size
+                storage = pa.ListArray.from_arrays(
+                    pa.array(list(range(0, (len(arrow_series) + 1) * list_size, list_size)), pa.int32()),
+                    storage.values,
+                )
+                return pa.ExtensionArray.from_storage(pyarrow_dtype, storage)
+            else:
+                # Variable-shaped tensor columns can't be converted directly to Ray's variable-shaped tensor extension
+                # type since it expects all tensor elements to have the same number of dimensions, which Daft does not enforce.
+                # TODO(Clark): Convert directly to Ray's variable-shaped tensor extension type when all tensor
+                # elements have the same number of dimensions, without going through pylist roundtrip.
+                return ArrowTensorArray.from_numpy(self.to_pylist())
+        elif dtype._is_fixed_shape_tensor_type() and pyarrow_supports_fixed_shape_tensor():
+            pyarrow_dtype = dtype.to_arrow_dtype(cast_tensor_to_ray_type=False)
+            arrow_series = self._series.to_arrow()
+            return pa.ExtensionArray.from_storage(pyarrow_dtype, arrow_series.storage)
+        else:
+            return self._series.to_arrow()
 
     def to_pylist(self) -> list:
         """
         Convert this Series to a Python list.
         """
         if self.datatype()._is_python_type():
             return self._series.to_pylist()
@@ -425,16 +476,16 @@
         return SeriesStringNamespace.from_series(self)
 
     @property
     def dt(self) -> SeriesDateNamespace:
         return SeriesDateNamespace.from_series(self)
 
     @property
-    def arr(self) -> SeriesArrayNamespace:
-        return SeriesArrayNamespace.from_series(self)
+    def list(self) -> SeriesListNamespace:
+        return SeriesListNamespace.from_series(self)
 
     @property
     def image(self) -> SeriesImageNamespace:
         return SeriesImageNamespace.from_series(self)
 
     def __reduce__(self) -> tuple:
         if self.datatype()._is_python_type():
@@ -504,17 +555,17 @@
     def year(self) -> Series:
         return Series._from_pyseries(self._series.dt_year())
 
     def day_of_week(self) -> Series:
         return Series._from_pyseries(self._series.dt_day_of_week())
 
 
-class SeriesArrayNamespace(SeriesNamespace):
+class SeriesListNamespace(SeriesNamespace):
     def lengths(self) -> Series:
-        return Series._from_pyseries(self._series.arr_lengths())
+        return Series._from_pyseries(self._series.list_lengths())
 
 
 class SeriesImageNamespace(SeriesNamespace):
     def decode(self) -> Series:
         return Series._from_pyseries(self._series.image_decode())
 
     def encode(self, image_format: str | ImageFormat) -> Series:
```

### Comparing `getdaft-0.1.8/daft/table/schema_inference.py` & `getdaft-0.1.9/daft/table/schema_inference.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/table/table.py` & `getdaft-0.1.9/daft/table/table.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,25 +3,20 @@
 from typing import TYPE_CHECKING, Any
 
 import pyarrow as pa
 from loguru import logger
 
 from daft.arrow_utils import ensure_table
 from daft.daft import PyTable as _PyTable
+from daft.daft import read_parquet as _read_parquet
 from daft.datatype import DataType
 from daft.expressions import Expression, ExpressionsProjection
 from daft.logical.schema import Schema
 from daft.series import Series
 
-_RAY_DATA_EXTENSIONS_AVAILABLE = True
-try:
-    from ray.data.extensions import ArrowTensorArray
-except ImportError:
-    _RAY_DATA_EXTENSIONS_AVAILABLE = False
-
 _NUMPY_AVAILABLE = True
 try:
     import numpy as np
 except ImportError:
     _NUMPY_AVAILABLE = False
 
 _PANDAS_AVAILABLE = True
@@ -31,14 +26,16 @@
     _PANDAS_AVAILABLE = False
 
 if TYPE_CHECKING:
     import numpy as np
     import pandas as pd
     import pyarrow as pa
 
+    from daft.io import IOConfig
+
 
 class Table:
     _table: _PyTable
 
     def __init__(self) -> None:
         raise NotImplementedError("We do not support creating a Table via __init__ ")
 
@@ -81,21 +78,25 @@
 
     @staticmethod
     def from_arrow(arrow_table: pa.Table) -> Table:
         assert isinstance(arrow_table, pa.Table)
         schema = Schema._from_field_name_and_types(
             [(f.name, DataType.from_arrow_type(f.type)) for f in arrow_table.schema]
         )
-        python_fields = [field.name for field in schema if field.dtype == DataType.python()]
-        if python_fields:
+        non_native_fields = [
+            field.name
+            for field in schema
+            if field.dtype == DataType.python()
+            or field.dtype._is_tensor_type()
+            or field.dtype._is_fixed_shape_tensor_type()
+        ]
+        if non_native_fields:
             # If there are any contained Arrow types that are not natively supported, go through Table.from_pydict()
             # path.
-            logger.debug(
-                f"Unsupported Arrow types detected, falling back to Python object type for columns: {python_fields}"
-            )
+            logger.debug(f"Unsupported Arrow types detected for columns: {non_native_fields}")
             return Table.from_pydict(dict(zip(arrow_table.column_names, arrow_table.columns)))
         else:
             # Otherwise, go through record batch happy path.
             arrow_table = ensure_table(arrow_table)
             pyt = _PyTable.from_arrow_record_batches(arrow_table.to_batches(), schema._schema)
             return Table._from_pytable(pyt)
 
@@ -120,17 +121,15 @@
         for k, v in data.items():
             if isinstance(v, list):
                 series = Series.from_pylist(v, name=k)
             elif _NUMPY_AVAILABLE and isinstance(v, np.ndarray):
                 series = Series.from_numpy(v, name=k)
             elif isinstance(v, Series):
                 series = v
-            elif isinstance(v, pa.Array):
-                series = Series.from_arrow(v, name=k)
-            elif isinstance(v, pa.ChunkedArray):
+            elif isinstance(v, (pa.Array, pa.ChunkedArray)):
                 series = Series.from_arrow(v, name=k)
             elif _PANDAS_AVAILABLE and isinstance(v, pd.Series):
                 series = Series.from_pandas(v, name=k)
             else:
                 raise ValueError(f"Creating a Series from data of type {type(v)} not implemented")
             series_dict[k] = series._series
         return Table._from_pytable(_PyTable.from_pylist_series(series_dict))
@@ -151,30 +150,30 @@
             raise TypeError(f"expected int for end but got {type(end)}")
         return Table._from_pytable(self._table.slice(start, end))
 
     ###
     # Exporting methods
     ###
 
-    def to_arrow(self) -> pa.Table:
-        python_fields = {field.name for field in self.schema() if field.dtype == DataType.python()}
-        if python_fields:
+    def to_arrow(self, cast_tensors_to_ray_tensor_dtype: bool = False) -> pa.Table:
+        python_fields = set()
+        tensor_fields = set()
+        for field in self.schema():
+            if field.dtype._is_python_type():
+                python_fields.add(field.name)
+            elif field.dtype._is_tensor_type() or field.dtype._is_fixed_shape_tensor_type():
+                tensor_fields.add(field.name)
+        if python_fields or tensor_fields:
             table = {}
             for colname in self.column_names():
                 column_series = self.get_column(colname)
                 if colname in python_fields:
-                    # TODO(Clark): Get the column as a top-level ndarray to ensure it remains contiguous.
                     column = column_series.to_pylist()
-                    # TODO(Clark): Infer the tensor extension type even when the column is empty.
-                    # This will probably require encoding more information in the Daft type that we use to
-                    # represent tensors.
-                    if _RAY_DATA_EXTENSIONS_AVAILABLE and len(column) > 0 and isinstance(column[0], np.ndarray):
-                        column = ArrowTensorArray.from_numpy(column)
                 else:
-                    column = column_series.to_arrow()
+                    column = column_series.to_arrow(cast_tensors_to_ray_tensor_dtype)
                 table[colname] = column
 
             return pa.Table.from_pydict(table)
         else:
             return pa.Table.from_batches([self._table.to_arrow_record_batch()])
 
     def to_pydict(self) -> dict[str, list]:
@@ -183,33 +182,39 @@
     def to_pylist(self) -> list[dict[str, Any]]:
         # TODO(Clark): Avoid a double-materialization of the table once the Rust-side table supports
         # by-row selection or iteration.
         table = self.to_pydict()
         column_names = self.column_names()
         return [{colname: table[colname][i] for colname in column_names} for i in range(len(self))]
 
-    def to_pandas(self, schema: Schema | None = None) -> pd.DataFrame:
+    def to_pandas(self, schema: Schema | None = None, cast_tensors_to_ray_tensor_dtype: bool = False) -> pd.DataFrame:
         if not _PANDAS_AVAILABLE:
             raise ImportError("Unable to import Pandas - please ensure that it is installed.")
-        python_fields = {field.name for field in self.schema() if field.dtype == DataType.python()}
-        if python_fields:
+        python_fields = set()
+        tensor_fields = set()
+        for field in self.schema():
+            if field.dtype._is_python_type():
+                python_fields.add(field.name)
+            elif field.dtype._is_tensor_type() or field.dtype._is_fixed_shape_tensor_type():
+                tensor_fields.add(field.name)
+        if python_fields or tensor_fields:
             # Use Python list representation for Python typed columns.
             table = {}
             for colname in self.column_names():
                 column_series = self.get_column(colname)
-                if colname in python_fields:
+                if colname in python_fields or (colname in tensor_fields and not cast_tensors_to_ray_tensor_dtype):
                     column = column_series.to_pylist()
                 else:
                     # Arrow-native field, so provide column as Arrow array.
-                    column = column_series.to_arrow()
+                    column = column_series.to_arrow(cast_tensors_to_ray_tensor_dtype).to_pandas()
                 table[colname] = column
 
             return pd.DataFrame.from_dict(table)
         else:
-            return self.to_arrow().to_pandas()
+            return self.to_arrow(cast_tensors_to_ray_tensor_dtype).to_pandas()
 
     ###
     # Compute methods (Table -> Table)
     ###
 
     def cast_to_schema(self, schema: Schema) -> Table:
         """Casts a Table into the provided schema"""
@@ -333,7 +338,20 @@
         else:
             raise TypeError(f"Expected a bool, list[bool] or None for `descending` but got {type(descending)}")
         return Series._from_pyseries(self._table.argsort(pyexprs, descending))
 
     def __reduce__(self) -> tuple:
         names = self.column_names()
         return Table.from_pydict, ({name: self.get_column(name) for name in names},)
+
+    @classmethod
+    def read_parquet(
+        cls,
+        path: str,
+        columns: list[str] | None = None,
+        row_groups: list[int] | None = None,
+        file_size: None | int = None,
+        io_config: IOConfig | None = None,
+    ) -> Table:
+        return Table._from_pytable(
+            _read_parquet(uri=path, columns=columns, row_groups=row_groups, size=file_size, io_config=io_config)
+        )
```

### Comparing `getdaft-0.1.8/daft/table/table_io.py` & `getdaft-0.1.9/daft/table/table_io.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/udf.py` & `getdaft-0.1.9/daft/udf.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         # Post-processing of results into a Series of the appropriate dtype
         if isinstance(result, Series):
             return result.rename(name).cast(self.udf.return_dtype)._series
         elif isinstance(result, list):
             if self.udf.return_dtype == DataType.python():
                 return Series.from_pylist(result, name=name, pyobj="force")._series
             else:
-                return Series.from_pylist(result, name=name, pyobj="disallow").cast(self.udf.return_dtype)._series
+                return Series.from_pylist(result, name=name, pyobj="allow").cast(self.udf.return_dtype)._series
         elif _NUMPY_AVAILABLE and isinstance(result, np.ndarray):
             return Series.from_numpy(result, name=name).cast(self.udf.return_dtype)._series
         else:
             raise NotImplementedError(f"Return type not supported for UDF: {type(result)}")
 
 
 @dataclasses.dataclass
```

### Comparing `getdaft-0.1.8/daft/udf_library/url_udfs.py` & `getdaft-0.1.9/daft/udf_library/url_udfs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/utils.py` & `getdaft-0.1.9/daft/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from __future__ import annotations
 
 import pickle
 import random
 import statistics
 from typing import Any, Callable
 
+import pyarrow as pa
+
+ARROW_VERSION = tuple(int(s) for s in pa.__version__.split(".") if s.isnumeric())
+
 
 def pydict_to_rows(pydict: dict[str, list]) -> list[frozenset[tuple[str, Any]]]:
     """Converts a dataframe pydict to a list of rows representation.
 
     e.g.
     {
         "fruit": ["apple", "banana", "carrot"],
@@ -85,7 +89,14 @@
 
 def map_operator_arrow_semantics(
     operator: Callable[[Any, Any], Any],
     left_pylist: list,
     right_pylist: list,
 ) -> list:
     return [operator(l, r) if (l is not None and r is not None) else None for (l, r) in zip(left_pylist, right_pylist)]
+
+
+def pyarrow_supports_fixed_shape_tensor() -> bool:
+    """Whether pyarrow supports the fixed_shape_tensor canonical extension type."""
+    from daft.context import get_context
+
+    return hasattr(pa, "fixed_shape_tensor") and (not get_context().is_ray_runner or ARROW_VERSION >= (13, 0, 0))
```

### Comparing `getdaft-0.1.8/daft/viz/dataframe_display.py` & `getdaft-0.1.9/daft/viz/dataframe_display.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/daft/viz/html_viz_hooks.py` & `getdaft-0.1.9/daft/viz/html_viz_hooks.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/Makefile` & `getdaft-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/10-min.ipynb` & `getdaft-0.1.9/docs/source/10-min.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/_static/daft-favicon.png` & `getdaft-0.1.9/docs/source/_static/daft-favicon.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/_static/daft-logo.png` & `getdaft-0.1.9/docs/source/_static/daft-logo.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/_static/daft_illustration.png` & `getdaft-0.1.9/docs/source/_static/daft_illustration.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/_static/dataframe-comp-table.csv` & `getdaft-0.1.9/docs/source/_static/dataframe-comp-table.csv`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/_static/execution_model.png` & `getdaft-0.1.9/docs/source/_static/execution_model.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/_static/header.css` & `getdaft-0.1.9/docs/source/_static/header.css`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/_static/high_level_architecture.png` & `getdaft-0.1.9/docs/source/_static/high_level_architecture.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/_static/in_memory_data_representation.png` & `getdaft-0.1.9/docs/source/_static/in_memory_data_representation.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/_static/mobile-menu.js` & `getdaft-0.1.9/docs/source/_static/mobile-menu.js`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/_static/tpch-1000sf.html` & `getdaft-0.1.9/docs/source/_static/tpch-1000sf.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/_static/tpch-100sf.html` & `getdaft-0.1.9/docs/source/_static/tpch-100sf.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/_static/tpch-nodes-count-daft-1000-sf.html` & `getdaft-0.1.9/docs/source/_static/tpch-nodes-count-daft-1000-sf.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/_templates/layout.html` & `getdaft-0.1.9/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/_templates/sections/header.html` & `getdaft-0.1.9/docs/source/_templates/sections/header.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/_templates/sections/mobile-menu.html` & `getdaft-0.1.9/docs/source/_templates/sections/mobile-menu.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/api_docs/dataframe.rst` & `getdaft-0.1.9/docs/source/api_docs/dataframe.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/api_docs/datatype.rst` & `getdaft-0.1.9/docs/source/api_docs/datatype.rst`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,15 @@
 Machine Learning
 ^^^^^^^^^^^^^^^^
 
 .. autosummary::
     :nosignatures:
     :toctree: doc_gen/datatype_methods
 
+    daft.DataType.tensor
     daft.DataType.embedding
 
 Computer Vision
 ^^^^^^^^^^^^^^^
 
 .. autosummary::
     :nosignatures:
```

### Comparing `getdaft-0.1.8/docs/source/api_docs/expressions.rst` & `getdaft-0.1.9/docs/source/api_docs/expressions.rst`

 * *Files 2% similar despite different names*

```diff
@@ -162,20 +162,21 @@
 
 
 Nested
 ******
 
 Operations on nested types (such as List and FixedSizeList), accessible through the ``Expression.list`` method accessor.
 
-Example: ``e1.str.concat(e2)``
+Example: ``e1.list.join(e2)``
 
 .. autosummary::
     :toctree: doc_gen/expression_methods
 
     daft.expressions.expressions.ExpressionListNamespace.join
+    daft.expressions.expressions.ExpressionListNamespace.lengths
 
 
 Changing Column Names/Types
 ###########################
 
 .. autosummary::
     :nosignatures:
```

### Comparing `getdaft-0.1.8/docs/source/api_docs/groupby.rst` & `getdaft-0.1.9/docs/source/api_docs/groupby.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/api_docs/input_output.rst` & `getdaft-0.1.9/docs/source/api_docs/input_output.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/benchmarks/index.rst` & `getdaft-0.1.9/docs/source/benchmarks/index.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/conf.py` & `getdaft-0.1.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/dataframe_comparison.rst` & `getdaft-0.1.9/docs/source/dataframe_comparison.rst`

 * *Files 2% similar despite different names*

```diff
@@ -46,10 +46,10 @@
 * **Compatibility with downstream Machine Learning tasks:** Spark itself is not well suited for performing distributed ML training which is increasingly becoming the domain of frameworks such as Ray and Horovod. Integrating with such a solution is difficult and requires expert tuning of intermediate storage and data engineering solutions.
 
 Ray Datasets
 ------------
 
 Ray Datasets make it easy to feed data really efficiently into Ray's model training and inference ecosystem. Datasets also provide basic functionality for data preprocessing such as mapping a function over each data item, filtering data etc.
 
-However, Ray Datasets are not a fully-fledged Dataframe abstraction (and `it is explicit in not being an ETL framework for data science <https://docs.ray.io/en/latest/data/faq.html#what-should-i-not-use-ray-datasets-for>`_) which means that it lacks key features in data querying, visualization and aggregations.
+However, Ray Datasets are not a fully-fledged Dataframe abstraction (and `it is explicit in not being an ETL framework for data science <https://docs.ray.io/en/latest/data/overview.html#ray-data-overview>`_) which means that it lacks key features in data querying, visualization and aggregations.
 
 Instead, Ray Data is a perfect destination for processed data from DaFt Dataframes to be sent to with a simple :meth:`df.to_ray_dataset() <daft.DataFrame.to_ray_dataset>` call. This is useful as an entrypoint into your model training and inference ecosystem!
```

### Comparing `getdaft-0.1.8/docs/source/index.rst` & `getdaft-0.1.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/install.rst` & `getdaft-0.1.9/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/learn/index.rst` & `getdaft-0.1.9/docs/source/learn/index.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/learn/key_concepts.rst` & `getdaft-0.1.9/docs/source/learn/key_concepts.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/learn/tutorials.rst` & `getdaft-0.1.9/docs/source/learn/tutorials.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/learn/user_guides/aggregations.rst` & `getdaft-0.1.9/docs/source/learn/user_guides/aggregations.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/learn/user_guides/dataframe-operations.rst` & `getdaft-0.1.9/docs/source/learn/user_guides/dataframe-operations.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/learn/user_guides/datatypes.rst` & `getdaft-0.1.9/docs/source/learn/user_guides/datatypes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Datatypes
 =========
 
 All columns in a Daft DataFrame have a DataType \(also often abbreviated as ``dtype``\).
 
 All elements of a column are of the same dtype, or they can be the special Null value \(indicating a missing value\).
 
-Daft provides simple DataTypes that are ubiquituous in many DataFrames such as numbers, strings and dates - all the way up to more complex types like images and embeddings.
+Daft provides simple DataTypes that are ubiquituous in many DataFrames such as numbers, strings and dates - all the way up to more complex types like tensors and images.
 
 .. NOTE::
 
     For a full overview on all the DataTypes that Daft supports, see the :doc:`DataType API Reference <../../api_docs/datatype>`.
 
 Numeric DataTypes
 -----------------
@@ -107,14 +107,15 @@
     Please get in touch with the Daft team and we would love to work together on building your type into canonical Daft types.
 
 Complex Types
 -------------
 
 Daft supports many more interesting complex DataTypes, for example:
 
+* :meth::`DataType.tensor() <daft.DataType.tensor>`: Multi-dimensional (potentially uniformly-shaped) tensors of data
 * :meth:`DataType.embedding() <daft.DataType.embedding>`: Lower-dimensional vector representation of data (e.g. words)
 * :meth:`DataType.image() <daft.DataType.image>`: NHWC images
 
 Daft abstracts away the in-memory representation of your data and provides kernels for many common operations on top of these data types. For supported image operations see the :ref:`image expressions API reference <api-expressions-images>`.
 
 For more complex algorithms, you can also drop into a Python UDF to process this data using your custom Python libraries.
```

### Comparing `getdaft-0.1.8/docs/source/learn/user_guides/expressions.rst` & `getdaft-0.1.9/docs/source/learn/user_guides/expressions.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/learn/user_guides/intro-dataframes.rst` & `getdaft-0.1.9/docs/source/learn/user_guides/intro-dataframes.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/learn/user_guides/read-write.rst` & `getdaft-0.1.9/docs/source/learn/user_guides/read-write.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/learn/user_guides/scaling-up.rst` & `getdaft-0.1.9/docs/source/learn/user_guides/scaling-up.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/learn/user_guides/udf.rst` & `getdaft-0.1.9/docs/source/learn/user_guides/udf.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/learn/user_guides.rst` & `getdaft-0.1.9/docs/source/learn/user_guides.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/technical_architecture.rst` & `getdaft-0.1.9/docs/source/technical_architecture.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/docs/source/telemetry.rst` & `getdaft-0.1.9/docs/source/telemetry.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/pyproject.toml` & `getdaft-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/requirements-dev.txt` & `getdaft-0.1.9/requirements-dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Development/Build utilities (allow to be unpinned)
 ipdb
 maturin
 pre-commit
 docker
 
 # Tracing
-orjson==3.9.1  # orjson recommended for viztracer
+orjson==3.9.2  # orjson recommended for viztracer
 py-spy==0.3.14
 viztracer==0.15.6
 
 # Testing frameworks
 hypothesis==6.79.2
 pytest==7.4.0
 pytest-benchmark==4.0.0
@@ -19,21 +19,21 @@
 lxml==4.9.2
 dask==2022.2.0; python_version < '3.8'
 dask==2023.5.0; python_version == '3.8'
 dask==2023.6.0; python_version >= '3.9'
 numpy; python_version < '3.9'
 numpy==1.25.0; python_version >= '3.9'
 pandas==1.3.5; python_version < '3.8'
-pandas==2.0.2; python_version >= '3.8'
+pandas==2.0.3; python_version >= '3.8'
 xxhash>=3.0.0
 Pillow==9.5.0
-opencv-python==4.7.0.72
+opencv-python==4.8.0.74
 
 # Ray
-ray[data, default]==2.4.0
+ray[data, default]==2.5.1
 pydantic<2  # pin pydantic because Ray uses broken APIs
 
 # AWS
 s3fs==2023.1.0; python_version < '3.8'
 s3fs==2023.6.0; python_version >= '3.8'
 # on old versions of s3fs's pinned botocore, they neglected to pin urllib3<2 which leads to:
 # "ImportError: cannot import name 'DEFAULT_CIPHERS' from 'urllib3.util.ssl_'"
```

### Comparing `getdaft-0.1.8/src/lib.rs` & `getdaft-0.1.9/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -17,13 +17,14 @@
     fn daft(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
         pyo3_log::init();
 
         daft_core::python::register_modules(_py, m)?;
         daft_dsl::register_modules(_py, m)?;
         daft_table::register_modules(_py, m)?;
         daft_io::register_modules(_py, m)?;
+        daft_parquet::register_modules(_py, m)?;
 
         m.add_wrapped(wrap_pyfunction!(version))?;
         m.add_wrapped(wrap_pyfunction!(build_type))?;
         Ok(())
     }
 }
```

### Comparing `getdaft-0.1.8/tests/assets/tpch-sqlite-queries/1.sql` & `getdaft-0.1.9/tests/assets/tpch-sqlite-queries/1.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/assets/tpch-sqlite-queries/10.sql` & `getdaft-0.1.9/tests/assets/tpch-sqlite-queries/10.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/assets/tpch-sqlite-queries/2.sql` & `getdaft-0.1.9/tests/assets/tpch-sqlite-queries/2.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/assets/tpch-sqlite-queries/7.sql` & `getdaft-0.1.9/tests/assets/tpch-sqlite-queries/7.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/assets/tpch-sqlite-queries/8.sql` & `getdaft-0.1.9/tests/assets/tpch-sqlite-queries/8.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/assets/tpch-sqlite-queries/9.sql` & `getdaft-0.1.9/tests/assets/tpch-sqlite-queries/9.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/benchmarks/conftest.py` & `getdaft-0.1.9/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/benchmarks/test_df_arithmetic.py` & `getdaft-0.1.9/tests/benchmarks/test_df_arithmetic.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/benchmarks/test_file_read.py` & `getdaft-0.1.9/tests/benchmarks/test_file_read.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/benchmarks/test_groups_and_aggs.py` & `getdaft-0.1.9/tests/benchmarks/test_groups_and_aggs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/benchmarks/test_join.py` & `getdaft-0.1.9/tests/benchmarks/test_join.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/benchmarks/test_repartition.py` & `getdaft-0.1.9/tests/benchmarks/test_repartition.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/benchmarks/test_sort.py` & `getdaft-0.1.9/tests/benchmarks/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/conftest.py` & `getdaft-0.1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/cookbook/assets/311-service-requests.24.csv` & `getdaft-0.1.9/tests/cookbook/assets/311-service-requests.24.csv`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/cookbook/assets/images/0000.jpg` & `getdaft-0.1.9/tests/cookbook/assets/images/0000.jpg`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/cookbook/assets/images/0007.jpg` & `getdaft-0.1.9/tests/cookbook/assets/images/0007.jpg`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/cookbook/assets/images/0018.png` & `getdaft-0.1.9/tests/cookbook/assets/images/0018.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/cookbook/assets/images/0025.tiff` & `getdaft-0.1.9/tests/cookbook/assets/images/0025.tiff`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/cookbook/conftest.py` & `getdaft-0.1.9/tests/cookbook/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/cookbook/test_aggregations.py` & `getdaft-0.1.9/tests/cookbook/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/cookbook/test_computations.py` & `getdaft-0.1.9/tests/cookbook/test_computations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/cookbook/test_count_rows.py` & `getdaft-0.1.9/tests/cookbook/test_count_rows.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/cookbook/test_dataloading.py` & `getdaft-0.1.9/tests/cookbook/test_dataloading.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/cookbook/test_distinct.py` & `getdaft-0.1.9/tests/cookbook/test_distinct.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/cookbook/test_filter.py` & `getdaft-0.1.9/tests/cookbook/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/cookbook/test_image.py` & `getdaft-0.1.9/tests/cookbook/test_image.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/cookbook/test_joins.py` & `getdaft-0.1.9/tests/cookbook/test_joins.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/cookbook/test_literals.py` & `getdaft-0.1.9/tests/cookbook/test_literals.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/cookbook/test_pandas_cookbook.py` & `getdaft-0.1.9/tests/cookbook/test_pandas_cookbook.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/cookbook/test_sorting.py` & `getdaft-0.1.9/tests/cookbook/test_sorting.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/cookbook/test_write.py` & `getdaft-0.1.9/tests/cookbook/test_write.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/dataframe/conftest.py` & `getdaft-0.1.9/tests/dataframe/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/dataframe/test_accessors.py` & `getdaft-0.1.9/tests/dataframe/test_accessors.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/dataframe/test_aggregations.py` & `getdaft-0.1.9/tests/dataframe/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/dataframe/test_creation.py` & `getdaft-0.1.9/tests/dataframe/test_creation.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as papq
 import pytest
 from fsspec.implementations.local import LocalFileSystem
-from ray.data.extensions import ArrowTensorArray
+from ray.data.extensions import ArrowTensorArray, TensorArray
 
 import daft
 from daft.api_annotations import APITypeError
 from daft.context import get_context
 from daft.dataframe import DataFrame
 from daft.datatype import DataType
+from daft.utils import pyarrow_supports_fixed_shape_tensor
 from tests.conftest import UuidType
 
 ARROW_VERSION = tuple(int(s) for s in pa.__version__.split(".") if s.isnumeric())
 
 
 class MyObj:
     pass
@@ -164,47 +165,46 @@
     expected = t.cast(t.schema.set(t.schema.get_field_index("variety"), casted_field))
     # Check roundtrip.
     assert df.to_arrow() == expected
 
 
 def test_create_dataframe_arrow_tensor_ray(valid_data: list[dict[str, float]]) -> None:
     pydict = {k: [item[k] for item in valid_data] for k in valid_data[0].keys()}
-    ata = ArrowTensorArray.from_numpy(np.ones((len(valid_data), 2, 2)))
-    pydict["obj"] = ata
+    shape = (2, 2)
+    arr = np.ones((len(valid_data),) + shape)
+    ata = ArrowTensorArray.from_numpy(arr)
+    pydict["tensor"] = ata
     t = pa.Table.from_pydict(pydict)
     df = daft.from_arrow(t)
     assert set(df.column_names) == set(t.column_names)
-    # Type not natively supported, so should have Python object dtype.
-    assert df.schema()["obj"].dtype == DataType.python()
-    casted_field = t.schema.field("variety").with_type(pa.large_string())
-    expected = t.cast(t.schema.set(t.schema.get_field_index("variety"), casted_field))
+    # Tensor type should be inferred.
+    expected_tensor_dtype = DataType.tensor(DataType.float64(), shape)
+    assert df.schema()["tensor"].dtype == expected_tensor_dtype
+    casted_variety = t.schema.field("variety").with_type(pa.large_string())
+    schema = t.schema.set(t.schema.get_field_index("variety"), casted_variety)
+    expected = t.cast(schema)
     # Check roundtrip.
-    assert df.to_arrow() == expected
+    assert df.to_arrow(True) == expected
 
 
 @pytest.mark.skipif(
-    ARROW_VERSION < (12, 0, 0),
+    not pyarrow_supports_fixed_shape_tensor(),
     reason=f"Arrow version {ARROW_VERSION} doesn't support the canonical tensor extension type.",
 )
-@pytest.mark.skipif(
-    get_context().runner_config.name == "ray",
-    reason="Pickling canonical tensor extension type is not supported by pyarrow",
-)
 def test_create_dataframe_arrow_tensor_canonical(valid_data: list[dict[str, float]]) -> None:
     pydict = {k: [item[k] for item in valid_data] for k in valid_data[0].keys()}
-    dtype = pa.fixed_shape_tensor(pa.int64(), (2, 2))
+    shape = (2, 2)
+    dtype = pa.fixed_shape_tensor(pa.int64(), shape)
     storage = pa.array([list(range(4 * i, 4 * (i + 1))) for i in range(len(valid_data))], pa.list_(pa.int64(), 4))
-    ata = pa.ExtensionArray.from_storage(dtype, storage)
-    pydict["obj"] = ata
+    fst = pa.ExtensionArray.from_storage(dtype, storage)
+    pydict["tensor"] = fst
     t = pa.Table.from_pydict(pydict)
     df = daft.from_arrow(t)
     assert set(df.column_names) == set(t.column_names)
-    assert df.schema()["obj"].dtype == DataType.extension(
-        "arrow.fixed_shape_tensor", DataType.from_arrow_type(dtype.storage_type), '{"shape":[2,2]}'
-    )
+    assert df.schema()["tensor"].dtype == DataType.tensor(DataType.int64(), shape)
     casted_field = t.schema.field("variety").with_type(pa.large_string())
     expected = t.cast(t.schema.set(t.schema.get_field_index("variety"), casted_field))
     # Check roundtrip.
     assert df.to_arrow() == expected
 
 
 def test_create_dataframe_arrow_extension_type(valid_data: list[dict[str, float]], uuid_ext_type: UuidType) -> None:
@@ -240,15 +240,17 @@
     t = pa.Table.from_pydict(pydict)
     with pytest.raises(ValueError):
         daft.from_arrow(t)
 
 
 def test_create_dataframe_arrow_unsupported_dtype(valid_data: list[dict[str, float]]) -> None:
     pydict = {k: [item[k] for item in valid_data] for k in valid_data[0].keys()}
-    pydict["obj"] = [decimal.Decimal("1.1") for _ in range(len(valid_data))]
+    pydict["obj"] = [
+        decimal.Decimal("12456789012345678901234567890123456789012345678901234567890") for _ in range(len(valid_data))
+    ]
     t = pa.Table.from_pydict(pydict)
     df = daft.from_arrow(t)
     assert set(df.column_names) == set(t.column_names)
     # Type not natively supported, so should have Python object dtype.
     assert df.schema()["obj"].dtype == DataType.python()
     casted_field = t.schema.field("variety").with_type(pa.large_string())
     expected = t.cast(t.schema.set(t.schema.get_field_index("variety"), casted_field))
@@ -284,22 +286,22 @@
     assert set(df.column_names) == set(pd_df.columns)
     # Check roundtrip.
     pd.testing.assert_frame_equal(df.to_pandas(), pd_df)
 
 
 def test_create_dataframe_pandas_tensor(valid_data: list[dict[str, float]]) -> None:
     pydict = {k: [item[k] for item in valid_data] for k in valid_data[0].keys()}
-    pydict["obj"] = pd.Series([np.ones((2, 2)) for _ in range(len(valid_data))])
+    shape = (2, 2)
+    pydict["tensor"] = TensorArray(np.ones((len(valid_data),) + shape))
     pd_df = pd.DataFrame(pydict)
     df = daft.from_pandas(pd_df)
-    # Type not natively supported, so should have Python object dtype.
-    assert df.schema()["obj"].dtype == DataType.python()
+    assert df.schema()["tensor"].dtype == DataType.tensor(DataType.float64(), shape)
     assert set(df.column_names) == set(pd_df.columns)
     # Check roundtrip.
-    pd.testing.assert_frame_equal(df.to_pandas(), pd_df)
+    pd.testing.assert_frame_equal(df.to_pandas(cast_tensors_to_ray_tensor_dtype=True), pd_df)
 
 
 @pytest.mark.parametrize(
     ["data", "expected_dtype"],
     [
         pytest.param([None, 2, 3], DataType.int64(), id="arrow_int"),
         pytest.param([None, 1.0, 3.0], DataType.float64(), id="arrow_float"),
@@ -325,15 +327,16 @@
         ),
         pytest.param(pa.array([[1, 2, 3], [1, 2], [1]]), DataType.list("item", DataType.int64()), id="pa_nested"),
         pytest.param(
             pa.chunked_array([pa.array([[1, 2, 3], [1, 2], [1]])]),
             DataType.list("item", DataType.int64()),
             id="pa_nested_chunked",
         ),
-        pytest.param(np.ones((3, 3)), DataType.python(), id="np_nested"),
+        pytest.param(np.ones((3, 3)), DataType.list("item", DataType.float64()), id="np_nested_1d"),
+        pytest.param(np.ones((3, 3, 3)), DataType.tensor(DataType.float64()), id="np_nested_nd"),
     ],
 )
 def test_load_pydict_types(data, expected_dtype):
     data_dict = {"x": data}
     daft_df = daft.from_pydict(data_dict)
     daft_df.collect()
     collected_data = daft_df.to_pydict()
```

### Comparing `getdaft-0.1.8/tests/dataframe/test_distinct.py` & `getdaft-0.1.9/tests/dataframe/test_distinct.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/dataframe/test_explode.py` & `getdaft-0.1.9/tests/dataframe/test_explode.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/dataframe/test_filter.py` & `getdaft-0.1.9/tests/dataframe/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/dataframe/test_getitem.py` & `getdaft-0.1.9/tests/dataframe/test_getitem.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/dataframe/test_iter.py` & `getdaft-0.1.9/tests/dataframe/test_iter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/dataframe/test_joins.py` & `getdaft-0.1.9/tests/dataframe/test_joins.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/dataframe/test_logical_type.py` & `getdaft-0.1.9/tests/dataframe/test_logical_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from __future__ import annotations
 
 import numpy as np
 import pandas as pd
+import pyarrow as pa
 import pytest
 from PIL import Image
 
 import daft
 from daft import DataType, Series, col
 from daft.datatype import DaftExtension
+from daft.utils import pyarrow_supports_fixed_shape_tensor
+
+ARROW_VERSION = tuple(int(s) for s in pa.__version__.split(".") if s.isnumeric())
 
 
 def test_embedding_type_df() -> None:
     data = [[1, 2, 3], np.arange(3), ["1", "2", "3"], [1, "2", 3.0], pd.Series([1.1, 2, 3]), (1, 2, 3), None]
     df = daft.from_pydict({"index": np.arange(len(data)), "embeddings": Series.from_pylist(data, pyobj="force")})
 
     target = DataType.embedding("arr", DataType.float32(), 3)
@@ -45,18 +49,55 @@
     arrow_table = df.to_arrow()
     assert isinstance(arrow_table["image"].type, DaftExtension)
 
 
 def test_fixed_shape_image_type_df() -> None:
     height = 2
     width = 2
-    shape = (3, height, width)
+    shape = (height, width, 3)
     data = [np.arange(12, dtype=np.uint8).reshape(shape), np.arange(12, 24, dtype=np.uint8).reshape(shape), None]
     df = daft.from_pydict({"index": np.arange(len(data)), "image": Series.from_pylist(data, pyobj="force")})
 
     target = DataType.image("RGB", height, width)
     df = df.select(col("index"), col("image").cast(target))
     df = df.repartition(4, "index")
     df = df.sort("index")
     df = df.collect()
     arrow_table = df.to_arrow()
     assert isinstance(arrow_table["image"].type, DaftExtension)
+
+
+def test_tensor_type_df() -> None:
+    data = [
+        np.arange(12).reshape((3, 2, 2)),
+        np.arange(12, 39).reshape((3, 3, 3)),
+        None,
+    ]
+    df = daft.from_pydict({"index": np.arange(len(data)), "tensor": Series.from_pylist(data, pyobj="allow")})
+
+    df = df.select(col("index"), col("tensor"))
+    df = df.repartition(4, "index")
+    df = df.sort("index")
+    df = df.collect()
+    arrow_table = df.to_arrow()
+    assert isinstance(arrow_table["tensor"].type, DaftExtension)
+
+
+def test_fixed_shape_tensor_type_df() -> None:
+    shape = (3, 2, 2)
+    data = [
+        np.arange(12).reshape(shape),
+        np.arange(12, 24).reshape(shape),
+        None,
+    ]
+    df = daft.from_pydict({"index": np.arange(len(data)), "tensor": Series.from_pylist(data, pyobj="allow")})
+
+    target = DataType.tensor(DataType.int64(), shape)
+    df = df.select(col("index"), col("tensor").cast(target))
+    df = df.repartition(4, "index")
+    df = df.sort("index")
+    df = df.collect()
+    arrow_table = df.to_arrow()
+    if pyarrow_supports_fixed_shape_tensor():
+        assert arrow_table["tensor"].type == pa.fixed_shape_tensor(pa.int64(), shape)
+    else:
+        assert isinstance(arrow_table["tensor"].type, DaftExtension)
```

### Comparing `getdaft-0.1.8/tests/dataframe/test_repr.py` & `getdaft-0.1.9/tests/dataframe/test_repr.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/dataframe/test_select.py` & `getdaft-0.1.9/tests/dataframe/test_select.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/dataframe/test_show.py` & `getdaft-0.1.9/tests/dataframe/test_show.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/dataframe/test_sort.py` & `getdaft-0.1.9/tests/dataframe/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/dataframe/test_temporals.py` & `getdaft-0.1.9/tests/dataframe/test_temporals.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import pytest
 
 import daft
 
 PYARROW_GE_7_0_0 = tuple(int(s) for s in pa.__version__.split(".") if s.isnumeric()) >= (7, 0, 0)
 
 
-@pytest.mark.skip("Requires Daft duration type.")
 def test_temporal_arithmetic() -> None:
     now = datetime.now()
     now_tz = datetime.now(timezone.utc)
     df = daft.from_pydict(
         {
             "dt_us": [datetime.min, now],
             "dt_us_tz": [datetime.min.replace(tzinfo=timezone.utc), now_tz],
```

### Comparing `getdaft-0.1.8/tests/dataframe/test_to_integrations.py` & `getdaft-0.1.9/tests/dataframe/test_to_integrations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/dataframe/test_with_column.py` & `getdaft-0.1.9/tests/dataframe/test_with_column.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/expressions/test_apply.py` & `getdaft-0.1.9/tests/expressions/test_apply.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/expressions/test_expressions.py` & `getdaft-0.1.9/tests/expressions/test_expressions.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/expressions/test_expressions_projection.py` & `getdaft-0.1.9/tests/expressions/test_expressions_projection.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/expressions/test_udf.py` & `getdaft-0.1.9/tests/expressions/test_udf.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,25 +142,25 @@
     def udf1(x):
         pass
 
     assert expr_structurally_equal(udf1("x"), udf1("x"))
     assert not expr_structurally_equal(udf1("x"), udf1("y"))
 
 
-def test_udf_return_numpy():
-    @udf(return_dtype=DataType.python())
+def test_udf_return_tensor():
+    @udf(return_dtype=DataType.tensor(DataType.float64()))
     def np_udf(x):
-        return [np.ones((3,)) * i for i in x.to_pylist()]
+        return [np.ones((3, 3)) * i for i in x.to_pylist()]
 
     expr = np_udf(col("x"))
     table = Table.from_pydict({"x": [0, 1, 2]})
     result = table.eval_expression_list([expr])
     assert len(result.to_pydict()["x"]) == 3
     for i in range(3):
-        np.testing.assert_array_equal(result.to_pydict()["x"][i], np.ones((3,)) * i)
+        np.testing.assert_array_equal(result.to_pydict()["x"][i], np.ones((3, 3)) * i)
 
 
 @pytest.mark.skip(
     reason="[RUST-INT][UDF] repr is very naive at the moment py_udf(...exprs), we should fix to show all parameters and use the function name"
 )
 def test_udf_repr():
     @udf(return_dtype=DataType.int64(), expr_inputs=["x"])
```

### Comparing `getdaft-0.1.8/tests/expressions/typing/conftest.py` & `getdaft-0.1.9/tests/expressions/typing/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/expressions/typing/test_aggs.py` & `getdaft-0.1.9/tests/expressions/typing/test_aggs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/expressions/typing/test_arithmetic.py` & `getdaft-0.1.9/tests/expressions/typing/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/expressions/typing/test_compare.py` & `getdaft-0.1.9/tests/expressions/typing/test_compare.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/expressions/typing/test_dt.py` & `getdaft-0.1.9/tests/expressions/typing/test_dt.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/expressions/typing/test_float.py` & `getdaft-0.1.9/tests/expressions/typing/test_float.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/expressions/typing/test_if_else.py` & `getdaft-0.1.9/tests/expressions/typing/test_if_else.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/expressions/typing/test_logical.py` & `getdaft-0.1.9/tests/expressions/typing/test_logical.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/expressions/typing/test_str.py` & `getdaft-0.1.9/tests/expressions/typing/test_str.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/integration/docker-compose/docker-compose.yml` & `getdaft-0.1.9/tests/integration/docker-compose/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/integration/docker-compose/nginx-serve-static-files.conf` & `getdaft-0.1.9/tests/integration/docker-compose/nginx-serve-static-files.conf`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/integration/io/test_url_download_http.py` & `getdaft-0.1.9/tests/integration/io/test_url_download_http.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/integration/io/test_url_download_local.py` & `getdaft-0.1.9/tests/integration/io/test_url_download_local.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/integration/io/test_url_download_public_aws_s3.py` & `getdaft-0.1.9/tests/integration/io/test_url_download_public_aws_s3.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/integration/io/test_url_download_s3_minio.py` & `getdaft-0.1.9/tests/integration/io/test_url_download_s3_minio.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,12 +19,11 @@
     df = df.with_column("data", df["urls"].url.download(fs=fs))
 
     assert df.to_pydict() == {**data, "data": [image_data for _ in range(len(urls))]}
 
 
 @pytest.mark.integration()
 def test_url_download_minio_native_downloader(minio_io_config, minio_image_data_fixture, image_data):
-    urls = minio_image_data_fixture
-    data = {"urls": urls}
+    data = {"urls": minio_image_data_fixture}
     df = daft.from_pydict(data)
     df = df.with_column("data", df["urls"].url.download(io_config=minio_io_config, use_native_downloader=True))
-    assert df.to_pydict() == {**data, "data": [image_data for _ in range(len(urls))]}
+    assert df.to_pydict() == {**data, "data": [image_data for _ in range(len(minio_image_data_fixture))]}
```

### Comparing `getdaft-0.1.8/tests/integration/test_tpch.py` & `getdaft-0.1.9/tests/integration/test_tpch.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/optimizer/conftest.py` & `getdaft-0.1.9/tests/optimizer/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/optimizer/test_drop_projections.py` & `getdaft-0.1.9/tests/optimizer/test_drop_projections.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/optimizer/test_drop_repartition.py` & `getdaft-0.1.9/tests/optimizer/test_drop_repartition.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/optimizer/test_fold_projections.py` & `getdaft-0.1.9/tests/optimizer/test_fold_projections.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/optimizer/test_prune_columns.py` & `getdaft-0.1.9/tests/optimizer/test_prune_columns.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/optimizer/test_pushdown_clauses_into_scan.py` & `getdaft-0.1.9/tests/optimizer/test_pushdown_clauses_into_scan.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/optimizer/test_pushdown_limit.py` & `getdaft-0.1.9/tests/optimizer/test_pushdown_limit.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/optimizer/test_pushdown_predicates.py` & `getdaft-0.1.9/tests/optimizer/test_pushdown_predicates.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/property_based_testing/strategies.py` & `getdaft-0.1.9/tests/property_based_testing/strategies.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/property_based_testing/test_sort.py` & `getdaft-0.1.9/tests/property_based_testing/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/ray/test_dask.py` & `getdaft-0.1.9/tests/ray/test_dask.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/ray/test_datasets.py` & `getdaft-0.1.9/tests/ray/test_datasets.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,39 +26,48 @@
 
 DATA = {
     "intcol": [1, 2, 3],
     "strcol": ["a", "b", "c"],
 }
 
 
+def _row_to_pydict(row: ray.data.row.TableRow | dict) -> dict:
+    if isinstance(row, dict):
+        return row
+    return row.as_pydict()
+
+
 @pytest.mark.skipif(get_context().runner_config.name != "ray", reason="Needs to run on Ray runner")
 @pytest.mark.parametrize("n_partitions", [1, 2])
 def test_to_ray_dataset_all_arrow(n_partitions: int):
     df = daft.from_pydict(DATA).repartition(n_partitions)
     df = df.with_column("floatcol", df["intcol"].cast(DataType.float64()))
     ds = df.to_ray_dataset()
 
     if RAY_VERSION < (2, 4, 0):
         if RAY_VERSION >= (2, 2, 0):
             assert ds.dataset_format() == "arrow", "Ray Dataset format should be arrow"
         elif RAY_VERSION >= (2, 0, 0):
             assert ds._dataset_format() == "arrow", "Ray Dataset format should be arrow"
 
-    rows = sorted([row.as_pydict() for row in ds.iter_rows()], key=lambda r: r["intcol"])
+    rows = sorted([_row_to_pydict(row) for row in ds.iter_rows()], key=lambda r: r["intcol"])
     assert rows == sorted(
         [
             {"intcol": 1, "strcol": "a", "floatcol": 1.0},
             {"intcol": 2, "strcol": "b", "floatcol": 2.0},
             {"intcol": 3, "strcol": "c", "floatcol": 3.0},
         ],
         key=lambda r: r["intcol"],
     )
 
 
 @pytest.mark.skipif(get_context().runner_config.name != "ray", reason="Needs to run on Ray runner")
+@pytest.mark.skipif(
+    RAY_VERSION >= (2, 5, 0), reason="Ray Datasets versions >= 2.5.0 no longer support Python objects as rows"
+)
 @pytest.mark.parametrize("n_partitions", [1, 2])
 def test_to_ray_dataset_with_py(n_partitions: int):
     df = daft.from_pydict(DATA).repartition(n_partitions)
     df = df.with_column("pycol", df["intcol"].apply(lambda x: MyObj(x), DataType.python()))
     ds = df.to_ray_dataset()
 
     if RAY_VERSION < (2, 4, 0):
@@ -78,28 +87,29 @@
     )
 
 
 @pytest.mark.skipif(get_context().runner_config.name != "ray", reason="Needs to run on Ray runner")
 @pytest.mark.parametrize("n_partitions", [1, 2])
 def test_to_ray_dataset_with_numpy(n_partitions: int):
     df = daft.from_pydict(DATA).repartition(n_partitions)
-    df = df.with_column("npcol", df["intcol"].apply(lambda _: np.ones((3, 3)), DataType.python()))
+    shape = (3, 3)
+    df = df.with_column("npcol", df["intcol"].apply(lambda _: np.ones(shape), DataType.tensor(DataType.int64(), shape)))
     ds = df.to_ray_dataset()
 
     if RAY_VERSION < (2, 4, 0):
         if RAY_VERSION >= (2, 2, 0):
             assert (
                 ds.dataset_format() == "arrow"
             ), "Ray Dataset format should be arrow because it uses a Tensor extension type"
         elif RAY_VERSION >= (2, 0, 0):
             assert (
                 ds._dataset_format() == "arrow"
             ), "Ray Dataset format should be arrow because it uses a Tensor extension type"
 
-    rows = sorted([row.as_pydict() for row in ds.iter_rows()], key=lambda r: r["intcol"])
+    rows = sorted([_row_to_pydict(row) for row in ds.iter_rows()], key=lambda r: r["intcol"])
     np.testing.assert_equal(
         rows,
         sorted(
             [
                 {"intcol": 1, "strcol": "a", "npcol": np.ones((3, 3))},
                 {"intcol": 2, "strcol": "b", "npcol": np.ones((3, 3))},
                 {"intcol": 3, "strcol": "c", "npcol": np.ones((3, 3))},
@@ -110,28 +120,28 @@
 
 
 @pytest.mark.skipif(get_context().runner_config.name != "ray", reason="Needs to run on Ray runner")
 @pytest.mark.skipif(RAY_VERSION < (2, 2, 0), reason="Variable-shaped tensor columns not supported in Ray < 2.1.0")
 @pytest.mark.parametrize("n_partitions", [1, 2])
 def test_to_ray_dataset_with_numpy_variable_shaped(n_partitions: int):
     df = daft.from_pydict(DATA).repartition(n_partitions)
-    df = df.with_column("npcol", df["intcol"].apply(lambda x: np.ones((x, 3)), DataType.python()))
+    df = df.with_column("npcol", df["intcol"].apply(lambda x: np.ones((x, 3)), DataType.tensor(DataType.int64())))
     ds = df.to_ray_dataset()
 
     if RAY_VERSION < (2, 4, 0):
         if RAY_VERSION >= (2, 2, 0):
             assert (
                 ds.dataset_format() == "arrow"
             ), "Ray Dataset format should be arrow because it uses a Tensor extension type"
         elif RAY_VERSION >= (2, 0, 0):
             assert (
                 ds._dataset_format() == "simple"
             ), "In old versions of Ray, we drop down to `simple` format because ArrowTensorType is not compatible with ragged tensors"
 
-    rows = sorted([row.as_pydict() for row in ds.iter_rows()], key=lambda r: r["intcol"])
+    rows = sorted([_row_to_pydict(row) for row in ds.iter_rows()], key=lambda r: r["intcol"])
     np.testing.assert_equal(
         rows,
         sorted(
             [
                 {"intcol": 1, "strcol": "a", "npcol": np.ones((1, 3))},
                 {"intcol": 2, "strcol": "b", "npcol": np.ones((2, 3))},
                 {"intcol": 3, "strcol": "c", "npcol": np.ones((3, 3))},
@@ -176,23 +186,29 @@
 @pytest.mark.parametrize("n_partitions", [1, 2])
 def test_from_ray_dataset_simple(n_partitions: int):
     ds = ray.data.range(8, parallelism=n_partitions)
 
     df = daft.from_ray_dataset(ds)
     # Sort data since partition ordering in Datasets is not deterministic.
     out = df.to_pydict()
-    assert list(out.keys()) == ["value"]
-    assert sorted(out["value"]) == list(range(8))
+    key = "id" if RAY_VERSION >= (2, 5, 0) else "value"
+    assert list(out.keys()) == [key]
+    assert sorted(out[key]) == list(range(8))
 
 
 @pytest.mark.skipif(get_context().runner_config.name != "ray", reason="Needs to run on Ray runner")
 @pytest.mark.parametrize("n_partitions", [1, 2])
 def test_from_ray_dataset_tensor(n_partitions: int):
     ds = ray.data.range(8)
-    ds = ds.map(lambda i: {"int": i, "np": np.ones((3, 3))}).repartition(n_partitions)
+    ds = (
+        ds.map(lambda d: {"int": d["id"], "np": np.ones((3, 3))})
+        if RAY_VERSION >= (2, 5, 0)
+        else ds.map(lambda i: {"int": i, "np": np.ones((3, 3))})
+    )
+    ds = ds.repartition(n_partitions)
 
     df = daft.from_ray_dataset(ds)
     out = df.to_pydict()
     assert out.keys() == {"int", "np"}
     # Sort data since partition ordering in Datasets is not deterministic.
     out_sorted_rows = sorted(list(zip(out["int"], out["np"])), key=lambda row: row[0])
     int_col, np_col = zip(*out_sorted_rows)
```

### Comparing `getdaft-0.1.8/tests/series/test_arithmetic.py` & `getdaft-0.1.9/tests/series/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/series/test_cast.py` & `getdaft-0.1.9/tests/series/test_cast.py`

 * *Files 20% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     target_dtype = DataType.list("arr", DataType.from_arrow_type(dtype))
 
     t = s.cast(target_dtype)
 
     assert t.datatype() == target_dtype
     assert len(t) == len(data)
 
-    assert t.arr.lengths().to_pylist() == [3, 3, 3, 3, 2, 2, None]
+    assert t.list.lengths().to_pylist() == [3, 3, 3, 3, 2, 2, None]
 
     pydata = t.to_pylist()
     assert pydata[-1] is None
     assert list(map(int, itertools.chain.from_iterable(data[:-1]))) == list(
         map(int, itertools.chain.from_iterable(pydata[:-1]))
     )
 
@@ -156,15 +156,15 @@
     target_dtype = DataType.fixed_size_list("arr", DataType.from_arrow_type(dtype), 3)
 
     t = s.cast(target_dtype)
 
     assert t.datatype() == target_dtype
     assert len(t) == len(data)
 
-    assert t.arr.lengths().to_pylist() == [3, 3, 3, 3, 3, 3, None]
+    assert t.list.lengths().to_pylist() == [3, 3, 3, 3, 3, 3, None]
 
     pydata = t.to_pylist()
     assert pydata[-1] is None
     assert list(map(int, itertools.chain.from_iterable(data[:-1]))) == list(
         map(int, itertools.chain.from_iterable(pydata[:-1]))
     )
 
@@ -177,37 +177,37 @@
     target_dtype = DataType.embedding("arr", DataType.from_arrow_type(dtype), 3)
 
     t = s.cast(target_dtype)
 
     assert t.datatype() == target_dtype
     assert len(t) == len(data)
 
-    assert t.arr.lengths().to_pylist() == [3, 3, 3, 3, 3, 3, None]
+    assert t.list.lengths().to_pylist() == [3, 3, 3, 3, 3, 3, None]
 
     pydata = t.to_pylist()
     assert pydata[-1] is None
     np.testing.assert_equal([np.asarray(arr, dtype=dtype.to_pandas_dtype()) for arr in data[:-1]], pydata[:-1])
 
 
 def test_series_cast_numpy_to_image() -> None:
     data = [
-        np.arange(12, dtype=np.uint8).reshape((3, 2, 2)),
+        np.arange(12, dtype=np.uint8).reshape((2, 2, 3)),
         np.arange(12, 39, dtype=np.uint8).reshape((3, 3, 3)),
         None,
     ]
     s = Series.from_pylist(data, pyobj="force")
 
     target_dtype = DataType.image("RGB")
 
     t = s.cast(target_dtype)
 
     assert t.datatype() == target_dtype
     assert len(t) == len(data)
 
-    assert t.arr.lengths().to_pylist() == [12, 27, None]
+    assert t.list.lengths().to_pylist() == [12, 27, None]
 
     pydata = t.to_pylist()
     assert pydata[-1] is None
     np.testing.assert_equal(data[:-1], pydata[:-1])
 
 
 def test_series_cast_numpy_to_image_infer_mode() -> None:
@@ -217,46 +217,309 @@
     target_dtype = DataType.image()
 
     t = s.cast(target_dtype)
 
     assert t.datatype() == target_dtype
     assert len(t) == len(data)
 
-    assert t.arr.lengths().to_pylist() == [4, 27, None]
+    assert t.list.lengths().to_pylist() == [4, 27, None]
 
     pydata = t.to_arrow().to_pylist()
     assert pydata[0] == {"data": data[0].ravel().tolist(), "mode": ImageMode.L, "channel": 1, "height": 2, "width": 2}
     assert pydata[1] == {"data": data[1].ravel().tolist(), "mode": ImageMode.RGB, "channel": 3, "height": 3, "width": 3}
     assert pydata[2] is None
     pydata = t.to_pylist()
     assert pydata[-1] is None
     np.testing.assert_equal([np.expand_dims(data[0], -1), data[1]], pydata[:-1])
 
 
 def test_series_cast_python_to_fixed_shape_image() -> None:
     height = 2
     width = 2
     shape = (height, width, 3)
-    data = [np.arange(12).reshape(shape), np.arange(12, 24).reshape(shape), None]
+    data = [np.arange(12, dtype=np.uint8).reshape(shape), np.arange(12, 24, dtype=np.uint8).reshape(shape), None]
     s = Series.from_pylist(data, pyobj="force")
 
     target_dtype = DataType.image("RGB", height, width)
 
     t = s.cast(target_dtype)
 
     assert t.datatype() == target_dtype
     assert len(t) == len(data)
 
-    assert t.arr.lengths().to_pylist() == [12, 12, None]
+    assert t.list.lengths().to_pylist() == [12, 12, None]
 
     pydata = t.to_pylist()
     assert pydata[-1] is None
     np.testing.assert_equal(data[:-1], pydata[:-1])
 
 
+def test_series_cast_numpy_to_tensor() -> None:
+    data = [
+        np.arange(12, dtype=np.uint8).reshape((2, 2, 3)),
+        np.arange(12, 39, dtype=np.uint8).reshape((3, 3, 3)),
+        None,
+    ]
+    s = Series.from_pylist(data, pyobj="force")
+
+    target_dtype = DataType.tensor(DataType.uint8())
+
+    t = s.cast(target_dtype)
+
+    assert t.datatype() == target_dtype
+    assert len(t) == len(data)
+
+    pydata = t.to_pylist()
+    assert pydata[-1] is None
+    np.testing.assert_equal(data[:-1], pydata[:-1])
+
+
+def test_series_cast_numpy_to_fixed_shape_tensor() -> None:
+    shape = (2, 2)
+    data = [
+        np.arange(4, dtype=np.uint8).reshape(shape),
+        np.arange(4, 8, dtype=np.uint8).reshape(shape),
+        None,
+    ]
+    s = Series.from_pylist(data, pyobj="force")
+
+    target_dtype = DataType.tensor(DataType.uint8(), shape)
+
+    t = s.cast(target_dtype)
+
+    assert t.datatype() == target_dtype
+    assert len(t) == len(data)
+
+    pydata = t.to_pylist()
+    assert pydata[-1] is None
+    np.testing.assert_equal(data[:-1], pydata[:-1])
+
+
+def test_series_cast_image_to_fixed_shape_image() -> None:
+    height = 2
+    width = 2
+    shape = (height, width, 3)
+    data = [np.arange(12, dtype=np.uint8).reshape(shape), np.arange(12, 24, dtype=np.uint8).reshape(shape), None]
+    s = Series.from_pylist(data, pyobj="force")
+
+    target_dtype = DataType.image("RGB")
+
+    t = s.cast(target_dtype)
+
+    assert t.datatype() == target_dtype
+
+    target_dtype = DataType.image("RGB", height, width)
+    u = t.cast(target_dtype)
+
+    assert u.datatype() == target_dtype
+    assert len(u) == len(data)
+
+    pydata = u.to_pylist()
+    assert pydata[-1] is None
+    np.testing.assert_equal(pydata[:-1], data[:-1])
+
+
+def test_series_cast_image_to_tensor() -> None:
+    data = [
+        np.arange(12, dtype=np.uint8).reshape((2, 2, 3)),
+        np.arange(12, 39, dtype=np.uint8).reshape((3, 3, 3)),
+        None,
+    ]
+    s = Series.from_pylist(data, pyobj="force")
+
+    target_dtype = DataType.image("RGB")
+
+    t = s.cast(target_dtype)
+
+    assert t.datatype() == target_dtype
+
+    target_dtype = DataType.tensor(DataType.uint8())
+
+    u = t.cast(target_dtype)
+
+    assert u.datatype() == target_dtype
+    assert len(u) == len(data)
+
+    pydata = u.to_pylist()
+    assert pydata[-1] is None
+    np.testing.assert_equal(data[:-1], pydata[:-1])
+
+
+def test_series_cast_image_to_fixed_shape_tensor() -> None:
+    height = 2
+    width = 2
+    shape = (height, width, 3)
+    data = [np.arange(12, dtype=np.uint8).reshape(shape), np.arange(12, 24, dtype=np.uint8).reshape(shape), None]
+    s = Series.from_pylist(data, pyobj="force")
+
+    target_dtype = DataType.image("RGB")
+
+    t = s.cast(target_dtype)
+
+    assert t.datatype() == target_dtype
+
+    target_dtype = DataType.tensor(DataType.uint8(), shape)
+    u = t.cast(target_dtype)
+
+    assert u.datatype() == target_dtype
+    assert len(u) == len(data)
+
+    pydata = u.to_pylist()
+    assert pydata[-1] is None
+    np.testing.assert_equal(pydata[:-1], data[:-1])
+
+
+def test_series_cast_fixed_shape_image_to_image() -> None:
+    height = 2
+    width = 2
+    shape = (height, width, 3)
+    data = [np.arange(12, dtype=np.uint8).reshape(shape), np.arange(12, 24, dtype=np.uint8).reshape(shape), None]
+    s = Series.from_pylist(data, pyobj="force")
+
+    target_dtype = DataType.image("RGB", height, width)
+
+    t = s.cast(target_dtype)
+
+    assert t.datatype() == target_dtype
+
+    target_dtype = DataType.image("RGB")
+    u = t.cast(target_dtype)
+
+    assert u.datatype() == target_dtype
+    assert len(u) == len(data)
+
+    pydata = u.to_pylist()
+    assert pydata[-1] is None
+    np.testing.assert_equal(pydata[:-1], data[:-1])
+
+
+def test_series_cast_fixed_shape_image_to_fixed_shape_tensor() -> None:
+    height = 2
+    width = 2
+    shape = (height, width, 3)
+    data = [np.arange(12, dtype=np.uint8).reshape(shape), np.arange(12, 24, dtype=np.uint8).reshape(shape), None]
+    s = Series.from_pylist(data, pyobj="force")
+
+    target_dtype = DataType.image("RGB", height, width)
+
+    t = s.cast(target_dtype)
+
+    assert t.datatype() == target_dtype
+
+    target_dtype = DataType.tensor(DataType.uint8(), shape)
+    u = t.cast(target_dtype)
+
+    assert u.datatype() == target_dtype
+    assert len(u) == len(data)
+
+    pydata = u.to_pylist()
+    assert pydata[-1] is None
+    np.testing.assert_equal(pydata[:-1], data[:-1])
+
+
+def test_series_cast_fixed_shape_image_to_tensor() -> None:
+    height = 2
+    width = 2
+    shape = (height, width, 3)
+    data = [np.arange(12, dtype=np.uint8).reshape(shape), np.arange(12, 24, dtype=np.uint8).reshape(shape), None]
+    s = Series.from_pylist(data, pyobj="force")
+
+    target_dtype = DataType.image("RGB", height, width)
+
+    t = s.cast(target_dtype)
+
+    assert t.datatype() == target_dtype
+
+    target_dtype = DataType.tensor(DataType.uint8())
+    u = t.cast(target_dtype)
+
+    assert u.datatype() == target_dtype
+    assert len(u) == len(data)
+
+    pydata = u.to_pylist()
+    assert pydata[-1] is None
+    np.testing.assert_equal(pydata[:-1], data[:-1])
+
+
+def test_series_cast_fixed_shape_tensor_to_tensor() -> None:
+    shape = (2, 2, 3)
+    data = [np.arange(12, dtype=np.uint8).reshape(shape), np.arange(12, 24, dtype=np.uint8).reshape(shape), None]
+    s = Series.from_pylist(data, pyobj="force")
+
+    target_dtype = DataType.tensor(DataType.uint8(), shape)
+
+    t = s.cast(target_dtype)
+
+    assert t.datatype() == target_dtype
+
+    target_dtype = DataType.tensor(DataType.uint8())
+    u = t.cast(target_dtype)
+
+    assert u.datatype() == target_dtype
+    assert len(u) == len(data)
+
+    pydata = u.to_pylist()
+    assert pydata[-1] is None
+    np.testing.assert_equal(pydata[:-1], data[:-1])
+
+
+def test_series_cast_embedding_to_fixed_shape_tensor() -> None:
+    shape = (4,)
+    data = [
+        np.arange(4, dtype=np.uint8).reshape(shape),
+        np.arange(4, 8, dtype=np.uint8).reshape(shape),
+        None,
+    ]
+    s = Series.from_pylist(data, pyobj="force")
+
+    target_dtype = DataType.embedding("arr", DataType.uint8(), 4)
+
+    t = s.cast(target_dtype)
+
+    assert t.datatype() == target_dtype
+
+    target_dtype = DataType.tensor(DataType.uint8(), shape)
+
+    u = t.cast(target_dtype)
+
+    assert u.datatype() == target_dtype
+    assert len(u) == len(data)
+
+    pydata = u.to_pylist()
+    assert pydata[-1] is None
+    np.testing.assert_equal(data[:-1], pydata[:-1])
+
+
+def test_series_cast_embedding_to_tensor() -> None:
+    shape = (4,)
+    data = [
+        np.arange(4, dtype=np.uint8).reshape(shape),
+        np.arange(4, 8, dtype=np.uint8).reshape(shape),
+        None,
+    ]
+    s = Series.from_pylist(data, pyobj="force")
+
+    target_dtype = DataType.embedding("arr", DataType.uint8(), 4)
+
+    t = s.cast(target_dtype)
+
+    assert t.datatype() == target_dtype
+
+    target_dtype = DataType.tensor(DataType.uint8())
+
+    u = t.cast(target_dtype)
+
+    assert u.datatype() == target_dtype
+    assert len(u) == len(data)
+
+    pydata = u.to_pylist()
+    assert pydata[-1] is None
+    np.testing.assert_equal(data[:-1], pydata[:-1])
+
+
 @pytest.mark.parametrize(
     "timeunit",
     [
         TimeUnit.s(),
         TimeUnit.ms(),
         TimeUnit.us(),
         TimeUnit.ns(),
```

### Comparing `getdaft-0.1.8/tests/series/test_comparisons.py` & `getdaft-0.1.9/tests/series/test_comparisons.py`

 * *Files 1% similar despite different names*

```diff
@@ -442,30 +442,30 @@
 def test_logical_ops_with_non_boolean() -> None:
     l_arrow = pa.array([False, True, None, None])
     r_arrow = pa.array([1, 2, 3, 4])
 
     l = Series.from_arrow(l_arrow)
     r = Series.from_arrow(r_arrow)
 
-    with pytest.raises(ValueError, match="logical operations on boolean supertype"):
+    with pytest.raises(ValueError, match="logic"):
         l & r
 
-    with pytest.raises(ValueError, match="logical operations on boolean supertype"):
+    with pytest.raises(ValueError, match="logic"):
         l | r
 
-    with pytest.raises(ValueError, match="logical operations on boolean supertype"):
+    with pytest.raises(ValueError, match="logic"):
         l ^ r
 
-    with pytest.raises(ValueError, match="logical operations on boolean supertype"):
+    with pytest.raises(ValueError, match="logic"):
         r & l
 
-    with pytest.raises(ValueError, match="logical operations on boolean supertype"):
+    with pytest.raises(ValueError, match="logic"):
         r | l
 
-    with pytest.raises(ValueError, match="logical operations on boolean supertype"):
+    with pytest.raises(ValueError, match="logic"):
         r ^ l
 
 
 def test_comparisons_dates() -> None:
 
     from datetime import date
```

### Comparing `getdaft-0.1.8/tests/series/test_concat.py` & `getdaft-0.1.9/tests/series/test_concat.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import numpy as np
 import pyarrow as pa
 import pytest
 from ray.data.extensions import ArrowTensorArray
 
 from daft import DataType, Series
 from daft.context import get_context
+from daft.utils import pyarrow_supports_fixed_shape_tensor
 from tests.conftest import *
 from tests.series import ARROW_FLOAT_TYPES, ARROW_INT_TYPES, ARROW_STRING_TYPES
 
 ARROW_VERSION = tuple(int(s) for s in pa.__version__.split(".") if s.isnumeric())
 
 
 class MockObject:
@@ -103,27 +104,23 @@
         )
         for i in range(chunks)
     ]
     series = [Series.from_arrow(ArrowTensorArray.from_numpy(chunk)) for chunk in chunks]
 
     concated = Series.concat(series)
 
-    assert concated.datatype() == DataType.python()
+    assert concated.datatype() == DataType.tensor(DataType.int64(), element_shape)
     expected = [chunk[i] for chunk in chunks for i in range(len(chunk))]
     np.testing.assert_equal(concated.to_pylist(), expected)
 
 
 @pytest.mark.skipif(
-    ARROW_VERSION < (12, 0, 0),
+    not pyarrow_supports_fixed_shape_tensor(),
     reason=f"Arrow version {ARROW_VERSION} doesn't support the canonical tensor extension type.",
 )
-@pytest.mark.skipif(
-    get_context().runner_config.name == "ray",
-    reason="Pickling canonical tensor extension type is not supported by pyarrow",
-)
 @pytest.mark.parametrize("chunks", [1, 2, 3, 10])
 def test_series_concat_tensor_array_canonical(chunks) -> None:
     element_shape = (2, 2)
     num_elements_per_tensor = np.prod(element_shape)
     chunk_size = 3
     chunk_shape = (chunk_size,) + element_shape
     chunks = [
@@ -133,16 +130,16 @@
         for i in range(chunks)
     ]
     ext_arrays = [pa.FixedShapeTensorArray.from_numpy_ndarray(chunk) for chunk in chunks]
     series = [Series.from_arrow(ext_array) for ext_array in ext_arrays]
 
     concated = Series.concat(series)
 
-    assert concated.datatype() == DataType.extension(
-        "arrow.fixed_shape_tensor", DataType.from_arrow_type(ext_arrays[0].type.storage_type), '{"shape":[2,2]}'
+    assert concated.datatype() == DataType.tensor(
+        DataType.from_arrow_type(ext_arrays[0].type.storage_type.value_type), (2, 2)
     )
     expected = [chunk[i] for chunk in chunks for i in range(len(chunk))]
     concated_arrow = concated.to_arrow()
     assert isinstance(concated_arrow.type, pa.FixedShapeTensorType)
     np.testing.assert_equal(concated_arrow.to_numpy_ndarray(), expected)
```

### Comparing `getdaft-0.1.8/tests/series/test_embedding.py` & `getdaft-0.1.9/tests/series/test_embedding.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/series/test_filter.py` & `getdaft-0.1.9/tests/series/test_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import numpy as np
 import pyarrow as pa
 import pytest
 
 from daft.context import get_context
 from daft.datatype import DataType
 from daft.series import Series
+from daft.utils import pyarrow_supports_fixed_shape_tensor
 from tests.series import ARROW_FLOAT_TYPES, ARROW_INT_TYPES, ARROW_STRING_TYPES
 
 ARROW_VERSION = tuple(int(s) for s in pa.__version__.split(".") if s.isnumeric())
 
 
 @pytest.mark.parametrize("dtype", ARROW_INT_TYPES + ARROW_FLOAT_TYPES + ARROW_STRING_TYPES)
 def test_series_filter(dtype) -> None:
@@ -130,34 +131,31 @@
 
     assert s.datatype() == result.datatype()
     expected = [val for val, keep in zip(s.to_pylist(), pymask) if keep]
     assert result.to_pylist() == expected
 
 
 @pytest.mark.skipif(
-    ARROW_VERSION < (12, 0, 0),
+    not pyarrow_supports_fixed_shape_tensor(),
     reason=f"Arrow version {ARROW_VERSION} doesn't support the canonical tensor extension type.",
 )
-@pytest.mark.skipif(
-    get_context().runner_config.name == "ray",
-    reason="Pickling canonical tensor extension type is not supported by pyarrow",
-)
 def test_series_filter_on_canonical_tensor_extension_array() -> None:
     arr = np.arange(20).reshape((5, 2, 2))
     data = pa.FixedShapeTensorArray.from_numpy_ndarray(arr)
 
     s = Series.from_arrow(data)
+    assert s.datatype() == DataType.tensor(DataType.int64(), (2, 2))
     pymask = [False, True, True, None, False]
     mask = Series.from_pylist(pymask)
 
     result = s.filter(mask)
 
     assert s.datatype() == result.datatype()
     expected = [val for val, keep in zip(s.to_pylist(), pymask) if keep]
-    assert result.to_pylist() == expected
+    np.testing.assert_equal(result.to_pylist(), expected)
 
 
 @pytest.mark.parametrize("dtype", ARROW_INT_TYPES + ARROW_FLOAT_TYPES + ARROW_STRING_TYPES)
 def test_series_filter_broadcast(dtype) -> None:
     data = pa.array([1, 2, 3, None, 5, None])
 
     s = Series.from_arrow(data.cast(dtype))
```

### Comparing `getdaft-0.1.8/tests/series/test_float.py` & `getdaft-0.1.9/tests/series/test_float.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/series/test_hash.py` & `getdaft-0.1.9/tests/series/test_hash.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/series/test_if_else.py` & `getdaft-0.1.9/tests/series/test_if_else.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import numpy as np
 import pyarrow as pa
 import pytest
 
 from daft import Series
 from daft.context import get_context
 from daft.datatype import DataType
+from daft.utils import pyarrow_supports_fixed_shape_tensor
 
 ARROW_VERSION = tuple(int(s) for s in pa.__version__.split(".") if s.isnumeric())
 
 
 @pytest.mark.parametrize("if_true_value", [1, None])
 @pytest.mark.parametrize("if_false_value", [0, None])
 @pytest.mark.parametrize(
@@ -344,21 +345,17 @@
         uuid_ext_type.NAME, DataType.from_arrow_type(uuid_ext_type.storage_type), ""
     )
     result_arrow = result.to_arrow()
     assert result_arrow == expected_arrow
 
 
 @pytest.mark.skipif(
-    ARROW_VERSION < (12, 0, 0),
+    not pyarrow_supports_fixed_shape_tensor(),
     reason=f"Arrow version {ARROW_VERSION} doesn't support the canonical tensor extension type.",
 )
-@pytest.mark.skipif(
-    get_context().runner_config.name == "ray",
-    reason="Pickling canonical tensor extension type is not supported by pyarrow",
-)
 @pytest.mark.parametrize(
     ["if_true", "if_false", "expected"],
     [
         # Same length, same type
         (
             np.arange(16).reshape((4, 2, 2)),
             np.arange(16, 32).reshape((4, 2, 2)),
@@ -393,16 +390,16 @@
     if_false_arrow = pa.FixedShapeTensorArray.from_numpy_ndarray(if_false)
     if_true_series = Series.from_arrow(if_true_arrow)
     if_false_series = Series.from_arrow(if_false_arrow)
     predicate_series = Series.from_arrow(pa.array([True, False, None, True]))
 
     result = predicate_series.if_else(if_true_series, if_false_series)
 
-    assert result.datatype() == DataType.extension(
-        "arrow.fixed_shape_tensor", DataType.from_arrow_type(if_true_arrow.type.storage_type), '{"shape":[2,2]}'
+    assert result.datatype() == DataType.tensor(
+        DataType.from_arrow_type(if_true_arrow.type.storage_type.value_type), (2, 2)
     )
     result_arrow = result.to_arrow()
     np.testing.assert_equal(result_arrow.to_numpy_ndarray(), expected)
 
 
 @pytest.mark.parametrize(
     "if_true_length",
```

### Comparing `getdaft-0.1.8/tests/series/test_image.py` & `getdaft-0.1.9/tests/series/test_image.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/series/test_numeric_ops.py` & `getdaft-0.1.9/tests/series/test_numeric_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/series/test_series.py` & `getdaft-0.1.9/tests/series/test_series.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/series/test_size_bytes.py` & `getdaft-0.1.9/tests/series/test_size_bytes.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import numpy as np
 import pyarrow as pa
 import pytest
 
 from daft.context import get_context
 from daft.datatype import DataType
 from daft.series import Series
+from daft.utils import pyarrow_supports_fixed_shape_tensor
 from tests.series import ARROW_FLOAT_TYPES, ARROW_INT_TYPES
 
 ARROW_VERSION = tuple(int(s) for s in pa.__version__.split(".") if s.isnumeric())
 PYARROW_GE_7_0_0 = ARROW_VERSION >= (7, 0, 0)
 
 
 def get_total_buffer_size(arr: pa.Array) -> int:
@@ -205,21 +206,17 @@
         uuid_ext_type.NAME, DataType.from_arrow_type(uuid_ext_type.storage_type), ""
     )
     post_daft_cast_data = storage.cast(pa.large_binary())
     assert size_bytes == get_total_buffer_size(post_daft_cast_data)
 
 
 @pytest.mark.skipif(
-    ARROW_VERSION < (12, 0, 0),
+    not pyarrow_supports_fixed_shape_tensor(),
     reason=f"Arrow version {ARROW_VERSION} doesn't support the canonical tensor extension type.",
 )
-@pytest.mark.skipif(
-    get_context().runner_config.name == "ray",
-    reason="Pickling canonical tensor extension type is not supported by pyarrow",
-)
 @pytest.mark.parametrize("dtype, size", itertools.product(ARROW_INT_TYPES + ARROW_FLOAT_TYPES, [0, 1, 2, 8, 9, 16]))
 @pytest.mark.parametrize("with_nulls", [True, False])
 def test_series_canonical_tensor_extension_type_size_bytes(dtype, size, with_nulls) -> None:
     tensor_type = pa.fixed_shape_tensor(pa.int64(), (2, 2))
     if size == 0:
         storage = pa.array([], pa.list_(pa.int64(), 4))
         data = pa.FixedShapeTensorArray.from_storage(tensor_type, storage)
@@ -229,11 +226,9 @@
         data = pa.FixedShapeTensorArray.from_storage(tensor_type, storage)
     else:
         arr = np.arange(4 * size).reshape((size, 2, 2))
         data = pa.FixedShapeTensorArray.from_numpy_ndarray(arr)
 
     s = Series.from_arrow(data)
 
-    assert s.datatype() == DataType.extension(
-        "arrow.fixed_shape_tensor", DataType.from_arrow_type(data.type.storage_type), '{"shape":[2,2]}'
-    )
+    assert s.datatype() == DataType.tensor(DataType.from_arrow_type(data.type.storage_type.value_type), (2, 2))
     assert s.size_bytes() == get_total_buffer_size(data)
```

### Comparing `getdaft-0.1.8/tests/series/test_slice.py` & `getdaft-0.1.9/tests/series/test_slice.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/series/test_sort.py` & `getdaft-0.1.9/tests/series/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/series/test_take.py` & `getdaft-0.1.9/tests/series/test_take.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import numpy as np
 import pyarrow as pa
 import pytest
 
 from daft.context import get_context
 from daft.datatype import DataType
 from daft.series import Series
+from daft.utils import pyarrow_supports_fixed_shape_tensor
 from tests.series import ARROW_FLOAT_TYPES, ARROW_INT_TYPES, ARROW_STRING_TYPES
 
 ARROW_VERSION = tuple(int(s) for s in pa.__version__.split(".") if s.isnumeric())
 
 
 @pytest.mark.parametrize("dtype", ARROW_INT_TYPES + ARROW_FLOAT_TYPES + ARROW_STRING_TYPES)
 def test_series_take(dtype) -> None:
@@ -141,42 +142,37 @@
     assert len(result) == 4
 
     expected = [pydata[i] if i is not None else None for i in pyidx]
     assert result.to_pylist() == expected
 
 
 @pytest.mark.skipif(
-    ARROW_VERSION < (12, 0, 0),
+    not pyarrow_supports_fixed_shape_tensor(),
     reason=f"Arrow version {ARROW_VERSION} doesn't support the canonical tensor extension type.",
 )
-@pytest.mark.skipif(
-    get_context().runner_config.name == "ray",
-    reason="Pickling canonical tensor extension type is not supported by pyarrow",
-)
 def test_series_canonical_tensor_extension_type_take() -> None:
     pydata = np.arange(24).reshape((6, 4)).tolist()
     pydata[2] = None
     storage = pa.array(pydata, pa.list_(pa.int64(), 4))
-    tensor_type = pa.fixed_shape_tensor(pa.int64(), (2, 2))
+    shape = (2, 2)
+    tensor_type = pa.fixed_shape_tensor(pa.int64(), shape)
     data = pa.FixedShapeTensorArray.from_storage(tensor_type, storage)
 
     s = Series.from_arrow(data)
-    assert s.datatype() == DataType.extension(
-        "arrow.fixed_shape_tensor", DataType.from_arrow_type(tensor_type.storage_type), '{"shape":[2,2]}'
-    )
+    assert s.datatype() == DataType.tensor(DataType.from_arrow_type(tensor_type.storage_type.value_type), shape)
     pyidx = [2, 0, None, 5]
     idx = Series.from_pylist(pyidx)
 
     result = s.take(idx)
     assert result.datatype() == s.datatype()
     assert len(result) == 4
 
     original_data = s.to_pylist()
     expected = [original_data[i] if i is not None else None for i in pyidx]
-    assert result.to_pylist() == expected
+    np.testing.assert_equal(result.to_pylist(), expected)
 
 
 def test_series_deeply_nested_take() -> None:
     # Test take on a Series with a deeply nested type: struct of list of struct of list of strings.
     data = pa.array([{"a": [{"b": ["foo", "bar"]}]}, {"a": [{"b": ["baz", "quux"]}]}])
     dtype = pa.struct([("a", pa.large_list(pa.struct([("b", pa.large_list(pa.large_string()))])))])
```

### Comparing `getdaft-0.1.8/tests/series/test_temporal_ops.py` & `getdaft-0.1.9/tests/series/test_temporal_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/series/test_utf8_ops.py` & `getdaft-0.1.9/tests/series/test_utf8_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/table/__init__.py` & `getdaft-0.1.9/tests/table/__init__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/table/list/test_list_join.py` & `getdaft-0.1.9/tests/table/list/test_list_join.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/table/table_io/test_csv.py` & `getdaft-0.1.9/tests/table/table_io/test_csv.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/table/table_io/test_json.py` & `getdaft-0.1.9/tests/table/table_io/test_json.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/table/table_io/test_parquet.py` & `getdaft-0.1.9/tests/table/table_io/test_parquet.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/table/table_io/test_read_time_cast.py` & `getdaft-0.1.9/tests/table/table_io/test_read_time_cast.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/table/test_blackbox_kernels.py` & `getdaft-0.1.9/tests/table/test_blackbox_kernels.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/table/test_concat.py` & `getdaft-0.1.9/tests/table/test_concat.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/table/test_eval.py` & `getdaft-0.1.9/tests/table/test_eval.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/table/test_explodes.py` & `getdaft-0.1.9/tests/table/test_explodes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/table/test_filter.py` & `getdaft-0.1.9/tests/table/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/table/test_from_py.py` & `getdaft-0.1.9/tests/table/test_from_py.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,54 +4,52 @@
 import itertools
 
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import pyarrow.compute as pac
 import pytest
-from ray.data.extensions import ArrowTensorArray, ArrowTensorType
 
 from daft import DataType, TimeUnit
 from daft.context import get_context
 from daft.series import Series
 from daft.table import Table
+from daft.utils import pyarrow_supports_fixed_shape_tensor
 
 ARROW_VERSION = tuple(int(s) for s in pa.__version__.split(".") if s.isnumeric())
 
 PYTHON_TYPE_ARRAYS = {
     "int": [1, 2],
     "float": [1.0, 2.0],
     "bool": [True, False],
     "str": ["foo", "bar"],
     "binary": [b"foo", b"bar"],
     "date": [datetime.date.today(), datetime.date.today()],
     "list": [[1, 2], [3]],
     "struct": [{"a": 1, "b": 2.0}, {"b": 3.0}],
     "empty_struct": [{}, {}],
     "null": [None, None],
+    "tensor": [np.ones((2, 2), np.int64), np.ones((3, 3), np.int64)],
     # The following types are not natively supported and will be cast to Python object types.
-    "tensor": list(np.arange(8).reshape(2, 2, 2)),
     "timestamp": [datetime.datetime.now(), datetime.datetime.now()],
 }
 
-
 PYTHON_INFERRED_TYPES = {
     "int": DataType.int64(),
     "float": DataType.float64(),
     "bool": DataType.bool(),
     "str": DataType.string(),
     "binary": DataType.binary(),
     "date": DataType.date(),
     "list": DataType.list("item", DataType.int64()),
     "struct": DataType.struct({"a": DataType.int64(), "b": DataType.float64()}),
     "empty_struct": DataType.struct({"": DataType.null()}),
     "null": DataType.null(),
+    "tensor": DataType.tensor(DataType.int64()),
     # The following types are not natively supported and will be cast to Python object types.
-    # TODO(Clark): Change the tensor inferred type to be the canonical fixed-shape tensor extension type.
-    "tensor": DataType.python(),
     "timestamp": DataType.timestamp(TimeUnit.us()),
 }
 
 PANDAS_INFERRED_TYPES = {
     **PYTHON_INFERRED_TYPES,
     "timestamp": DataType.timestamp(TimeUnit.ns()),
 }
@@ -63,16 +61,16 @@
     "str": pa.large_string(),
     "binary": pa.large_binary(),
     "date": pa.date32(),
     "list": pa.large_list(pa.int64()),
     "struct": pa.struct({"a": pa.int64(), "b": pa.float64()}),
     "empty_struct": pa.struct({"": pa.null()}),
     "null": pa.null(),
+    "tensor": PYTHON_INFERRED_TYPES["tensor"].to_arrow_dtype(),
     # The following types are not natively supported and will be cast to Python object types.
-    "tensor": ArrowTensorType(shape=(2, 2), dtype=pa.int64()),
     "timestamp": pa.timestamp("us"),
 }
 
 
 ARROW_TYPE_ARRAYS = {
     "int8": pa.array(PYTHON_TYPE_ARRAYS["int"], pa.int8()),
     "int16": pa.array(PYTHON_TYPE_ARRAYS["int"], pa.int16()),
@@ -89,16 +87,30 @@
     "boolean": pa.array(PYTHON_TYPE_ARRAYS["bool"], pa.bool_()),
     "date32": pa.array(PYTHON_TYPE_ARRAYS["date"], pa.date32()),
     "list": pa.array(PYTHON_TYPE_ARRAYS["list"], pa.list_(pa.int64())),
     "fixed_size_list": pa.array([[1, 2], [3, 4]], pa.list_(pa.int64(), 2)),
     "struct": pa.array(PYTHON_TYPE_ARRAYS["struct"], pa.struct([("a", pa.int64()), ("b", pa.float64())])),
     "empty_struct": pa.array(PYTHON_TYPE_ARRAYS["empty_struct"], pa.struct({"": pa.null()})),
     "null": pa.array(PYTHON_TYPE_ARRAYS["null"], pa.null()),
+    "tensor": pa.ExtensionArray.from_storage(
+        ROUNDTRIP_TYPES["tensor"],
+        pa.array(
+            [
+                {"data": PYTHON_TYPE_ARRAYS["tensor"][0].ravel(), "shape": [2, 2]},
+                {"data": PYTHON_TYPE_ARRAYS["tensor"][1].ravel(), "shape": [3, 3]},
+            ],
+            pa.struct(
+                {
+                    "data": pa.large_list(pa.field("data", pa.int64())),
+                    "shape": pa.large_list(pa.field("shape", pa.uint64())),
+                }
+            ),
+        ),
+    ),
     # The following types are not natively supported and will be cast to Python object types.
-    "tensor": ArrowTensorArray.from_numpy(PYTHON_TYPE_ARRAYS["tensor"]),
     "timestamp": pa.array(PYTHON_TYPE_ARRAYS["timestamp"]),
 }
 
 
 ARROW_ROUNDTRIP_TYPES = {
     "int8": pa.int8(),
     "int16": pa.int16(),
@@ -115,24 +127,28 @@
     "boolean": pa.bool_(),
     "date32": pa.date32(),
     "list": pa.large_list(pa.int64()),
     "fixed_size_list": pa.list_(pa.int64(), 2),
     "struct": pa.struct([("a", pa.int64()), ("b", pa.float64())]),
     "empty_struct": pa.struct({"": pa.null()}),
     "null": pa.null(),
+    "tensor": PYTHON_INFERRED_TYPES["tensor"].to_arrow_dtype(),
     # The following types are not natively supported and will be cast to Python object types.
-    "tensor": ArrowTensorType(shape=(2, 2), dtype=pa.int64()),
     "timestamp": pa.timestamp("us"),
 }
 
-if ARROW_VERSION >= (12, 0, 0) and get_context().runner_config.name != "ray":
-    ARROW_ROUNDTRIP_TYPES["canonical_tensor"] = pa.fixed_shape_tensor(pa.int64(), (2, 2))
-    ARROW_TYPE_ARRAYS["canonical_tensor"] = pa.FixedShapeTensorArray.from_numpy_ndarray(
-        np.array(PYTHON_TYPE_ARRAYS["tensor"])
-    )
+if pyarrow_supports_fixed_shape_tensor():
+    arrow_tensor_dtype = pa.fixed_shape_tensor(pa.int64(), (2, 2))
+    # NOTE: We don't infer fixed-shape tensors when constructing a table from Python objects, since
+    # the shapes may be variable across partitions.
+    # PYTHON_TYPE_ARRAYS["canonical_tensor"] = list(np.arange(8).reshape(2, 2, 2))
+    # PYTHON_INFERRED_TYPES["canonical_tensor"] = DataType.tensor(DataType.int64(), (2, 2))
+    # ROUNDTRIP_TYPES["canonical_tensor"] = arrow_tensor_dtype
+    ARROW_ROUNDTRIP_TYPES["canonical_tensor"] = arrow_tensor_dtype
+    ARROW_TYPE_ARRAYS["canonical_tensor"] = pa.FixedShapeTensorArray.from_numpy_ndarray(np.arange(8).reshape(2, 2, 2))
 
 
 def _with_uuid_ext_type(uuid_ext_type) -> tuple[dict, dict]:
     if get_context().runner_config.name == "ray":
         # pyarrow extension types aren't supported in Ray clusters yet.
         return ARROW_ROUNDTRIP_TYPES, ARROW_TYPE_ARRAYS
     arrow_roundtrip_types = ARROW_ROUNDTRIP_TYPES.copy()
@@ -149,15 +165,15 @@
     assert set(table.column_names()) == set(PYTHON_TYPE_ARRAYS.keys())
     for field in table.schema():
         assert field.dtype == PYTHON_INFERRED_TYPES[field.name]
     schema = pa.schema(ROUNDTRIP_TYPES)
     arrs = {}
     for col_name, col in PYTHON_TYPE_ARRAYS.items():
         if col_name == "tensor":
-            arrs[col_name] = ArrowTensorArray.from_numpy(col)
+            arrs[col_name] = ARROW_TYPE_ARRAYS[col_name]
         else:
             arrs[col_name] = pa.array(col, type=schema.field(col_name).type)
     expected_table = pa.table(arrs, schema=schema)
     assert table.to_arrow() == expected_table
 
 
 def test_from_pydict_arrow_roundtrip(uuid_ext_type) -> None:
@@ -186,17 +202,14 @@
 def test_from_pandas_roundtrip() -> None:
     df = pd.DataFrame(PYTHON_TYPE_ARRAYS)
     table = Table.from_pandas(df)
     assert len(table) == 2
     assert set(table.column_names()) == set(PYTHON_TYPE_ARRAYS.keys())
     for field in table.schema():
         assert field.dtype == PANDAS_INFERRED_TYPES[field.name]
-    # pyarrow --> pandas doesn't preserve the datetime type for the "date" column, so we need to
-    # convert it before the comparison.
-    df["date"] = pd.to_datetime(df["date"]).astype("datetime64[s]")
     # pyarrow --> pandas will insert explicit Nones within the struct fields.
     df["struct"][1]["a"] = None
     df["empty_struct"][0][""] = None
     df["empty_struct"][1][""] = None
     pd.testing.assert_frame_equal(table.to_pandas(), df)
```

### Comparing `getdaft-0.1.8/tests/table/test_head.py` & `getdaft-0.1.9/tests/table/test_head.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/table/test_joins.py` & `getdaft-0.1.9/tests/table/test_joins.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/table/test_partitioning.py` & `getdaft-0.1.9/tests/table/test_partitioning.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/table/test_size_bytes.py` & `getdaft-0.1.9/tests/table/test_size_bytes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/table/test_sorting.py` & `getdaft-0.1.9/tests/table/test_sorting.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/table/test_table_aggs.py` & `getdaft-0.1.9/tests/table/test_table_aggs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/table/test_take.py` & `getdaft-0.1.9/tests/table/test_take.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/table/utf8/test_compares.py` & `getdaft-0.1.9/tests/table/utf8/test_compares.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/test_analytics.py` & `getdaft-0.1.9/tests/test_analytics.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/test_datatypes.py` & `getdaft-0.1.9/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/test_schema.py` & `getdaft-0.1.9/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tests/udf_library/test_url_udfs.py` & `getdaft-0.1.9/tests/udf_library/test_url_udfs.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,84 +28,100 @@
     for fp in filepaths:
         fp.write_bytes(fp.name.encode("utf-8"))
     return filepaths
 
 
 @pytest.mark.parametrize("use_native_downloader", [False, True])
 def test_download(files, use_native_downloader):
-    df = daft.from_pydict({"filenames": [str(f) for f in files]})
-    df = df.with_column("bytes", col("filenames").url.download(use_native_downloader=use_native_downloader))
-    pd_df = pd.DataFrame.from_dict({"filenames": [str(f) for f in files]})
-    pd_df["bytes"] = pd.Series([pathlib.Path(fn).read_bytes() for fn in files])
-    assert_df_equals(df.to_pandas(), pd_df, sort_key="filenames")
+    # Run it twice to ensure runtime works
+    for _ in range(2):
+        df = daft.from_pydict({"filenames": [str(f) for f in files]})
+        df = df.with_column("bytes", col("filenames").url.download(use_native_downloader=use_native_downloader))
+        pd_df = pd.DataFrame.from_dict({"filenames": [str(f) for f in files]})
+        pd_df["bytes"] = pd.Series([pathlib.Path(fn).read_bytes() for fn in files])
+        assert_df_equals(df.to_pandas(), pd_df, sort_key="filenames")
+        print(_)
 
 
 @pytest.mark.skipif(get_context().runner_config.name not in {"py"}, reason="requires PyRunner to be in use")
 def test_download_custom_ds(files):
     # Mark that this filesystem instance shouldn't be automatically reused by fsspec; without this,
     # fsspec would cache this instance and reuse it for Daft's default construction of filesystems,
     # which would make this test pass without the passed filesystem being used.
-    fs = LocalFileSystem(skip_instance_cache=True)
 
-    df = daft.from_pydict({"filenames": [str(f) for f in files]})
-
-    df = df.with_column("bytes", col("filenames").url.download(fs=fs))
-    out_df = df.to_pandas()
-
-    pd_df = pd.DataFrame.from_dict({"filenames": [str(f) for f in files]})
-    pd_df["bytes"] = pd.Series([pathlib.Path(fn).read_bytes() for fn in files])
-    assert_df_equals(out_df, pd_df, sort_key="filenames")
+    # Run it twice to ensure runtime works
+    for _ in range(2):
+        fs = LocalFileSystem(skip_instance_cache=True)
+
+        df = daft.from_pydict({"filenames": [str(f) for f in files]})
+
+        df = df.with_column("bytes", col("filenames").url.download(fs=fs))
+        out_df = df.to_pandas()
+
+        pd_df = pd.DataFrame.from_dict({"filenames": [str(f) for f in files]})
+        pd_df["bytes"] = pd.Series([pathlib.Path(fn).read_bytes() for fn in files])
+        assert_df_equals(out_df, pd_df, sort_key="filenames")
 
 
 @pytest.mark.parametrize("use_native_downloader", [False, True])
 def test_download_with_none(files, use_native_downloader):
     data = {"id": list(range(len(files) * 2)), "filenames": [str(f) for f in files] + [None for _ in range(len(files))]}
-    df = daft.from_pydict(data)
-    df = df.with_column("bytes", col("filenames").url.download(use_native_downloader=use_native_downloader))
-    pd_df = pd.DataFrame.from_dict(data)
-    pd_df["bytes"] = pd.Series([pathlib.Path(fn).read_bytes() if fn is not None else None for fn in files])
-    assert_df_equals(df.to_pandas(), pd_df, sort_key="id")
+    # Run it twice to ensure runtime works
+    for _ in range(2):
+        df = daft.from_pydict(data)
+        df = df.with_column("bytes", col("filenames").url.download(use_native_downloader=use_native_downloader))
+        pd_df = pd.DataFrame.from_dict(data)
+        pd_df["bytes"] = pd.Series([pathlib.Path(fn).read_bytes() if fn is not None else None for fn in files])
+        assert_df_equals(df.to_pandas(), pd_df, sort_key="id")
 
 
 @pytest.mark.parametrize("use_native_downloader", [False, True])
 def test_download_with_missing_urls(files, use_native_downloader):
     data = {
         "id": list(range(len(files) * 2)),
         "filenames": [str(f) for f in files] + [str(uuid.uuid4()) for _ in range(len(files))],
     }
-    df = daft.from_pydict(data)
-    df = df.with_column(
-        "bytes", col("filenames").url.download(on_error="null", use_native_downloader=use_native_downloader)
-    )
-    pd_df = pd.DataFrame.from_dict(data)
-    pd_df["bytes"] = pd.Series([pathlib.Path(fn).read_bytes() if pathlib.Path(fn).exists() else None for fn in files])
-    assert_df_equals(df.to_pandas(), pd_df, sort_key="id")
+    # Run it twice to ensure runtime works
+    for _ in range(2):
+        df = daft.from_pydict(data)
+        df = df.with_column(
+            "bytes", col("filenames").url.download(on_error="null", use_native_downloader=use_native_downloader)
+        )
+        pd_df = pd.DataFrame.from_dict(data)
+        pd_df["bytes"] = pd.Series(
+            [pathlib.Path(fn).read_bytes() if pathlib.Path(fn).exists() else None for fn in files]
+        )
+        assert_df_equals(df.to_pandas(), pd_df, sort_key="id")
 
 
 @pytest.mark.parametrize("use_native_downloader", [False, True])
 def test_download_with_missing_urls_reraise_errors(files, use_native_downloader):
     data = {
         "id": list(range(len(files) * 2)),
         "filenames": [str(f) for f in files] + [str(uuid.uuid4()) for _ in range(len(files))],
     }
-    df = daft.from_pydict(data)
-    df = df.with_column(
-        "bytes", col("filenames").url.download(on_error="raise", use_native_downloader=use_native_downloader)
-    )
-    # TODO: Change to a FileNotFound Error
-    with pytest.raises(FileNotFoundError):
-        df.collect()
+    # Run it twice to ensure runtime works
+    for _ in range(2):
+        df = daft.from_pydict(data)
+        df = df.with_column(
+            "bytes", col("filenames").url.download(on_error="raise", use_native_downloader=use_native_downloader)
+        )
+        # TODO: Change to a FileNotFound Error
+        with pytest.raises(FileNotFoundError):
+            df.collect()
 
 
 @pytest.mark.parametrize("use_native_downloader", [False, True])
 def test_download_with_duplicate_urls(files, use_native_downloader):
     data = {
         "id": list(range(len(files) * 2)),
         "filenames": [str(f) for f in files] * 2,
     }
-    df = daft.from_pydict(data)
-    df = df.with_column("bytes", col("filenames").url.download(use_native_downloader=use_native_downloader))
-    pd_df = pd.DataFrame.from_dict(data)
-    pd_df["bytes"] = pd.Series(
-        [pathlib.Path(fn).read_bytes() if pathlib.Path(fn).exists() else None for fn in files * 2]
-    )
-    assert_df_equals(df.to_pandas(), pd_df, sort_key="id")
+    # Run it twice to ensure runtime works
+    for _ in range(2):
+        df = daft.from_pydict(data)
+        df = df.with_column("bytes", col("filenames").url.download(use_native_downloader=use_native_downloader))
+        pd_df = pd.DataFrame.from_dict(data)
+        pd_df["bytes"] = pd.Series(
+            [pathlib.Path(fn).read_bytes() if pathlib.Path(fn).exists() else None for fn in files * 2]
+        )
+        assert_df_equals(df.to_pandas(), pd_df, sort_key="id")
```

### Comparing `getdaft-0.1.8/tests_legacy/test_resource_requests.py` & `getdaft-0.1.9/tests_legacy/test_resource_requests.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tools/patch_package_version.py` & `getdaft-0.1.9/tools/patch_package_version.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tools/wheels/_vendor/wheel/LICENSE.txt` & `getdaft-0.1.9/tools/wheels/_vendor/wheel/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tools/wheels/_vendor/wheel/cli/__init__.py` & `getdaft-0.1.9/tools/wheels/_vendor/wheel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tools/wheels/_vendor/wheel/cli/convert.py` & `getdaft-0.1.9/tools/wheels/_vendor/wheel/cli/convert.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tools/wheels/_vendor/wheel/cli/pack.py` & `getdaft-0.1.9/tools/wheels/_vendor/wheel/cli/pack.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tools/wheels/_vendor/wheel/cli/unpack.py` & `getdaft-0.1.9/tools/wheels/_vendor/wheel/cli/unpack.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tools/wheels/_vendor/wheel/pkginfo.py` & `getdaft-0.1.9/tools/wheels/_vendor/wheel/pkginfo.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tools/wheels/_vendor/wheel/util.py` & `getdaft-0.1.9/tools/wheels/_vendor/wheel/util.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tools/wheels/_vendor/wheel/wheelfile.py` & `getdaft-0.1.9/tools/wheels/_vendor/wheel/wheelfile.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tools/wheels/fix-and-copy-wheel.py` & `getdaft-0.1.9/tools/wheels/fix-and-copy-wheel.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tools/wheels/tmpdirs.py` & `getdaft-0.1.9/tools/wheels/tmpdirs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tools/wheels/tools.py` & `getdaft-0.1.9/tools/wheels/tools.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tools/wheels/wheeltools.py` & `getdaft-0.1.9/tools/wheels/wheeltools.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb` & `getdaft-0.1.9/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tutorials/image_querying/top_n_red_color.ipynb` & `getdaft-0.1.9/tutorials/image_querying/top_n_red_color.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tutorials/mnist.ipynb` & `getdaft-0.1.9/tutorials/mnist.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tutorials/text_to_image/text_to_image_generation.ipynb` & `getdaft-0.1.9/tutorials/text_to_image/text_to_image_generation.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/tutorials/text_to_image/using_cloud_with_ray.ipynb` & `getdaft-0.1.9/tutorials/text_to_image/using_cloud_with_ray.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.8/Cargo.lock` & `getdaft-0.1.9/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "addr2line"
+version = "0.20.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f4fa78e18c64fce05e902adecd7a5eed15a5e0a3439f7b0e169f0252214865e3"
+dependencies = [
+ "gimli",
+]
+
+[[package]]
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "ahash"
@@ -26,14 +35,29 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "alloc-no-stdlib"
+version = "2.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cc7bb162ec39d46ab1ca8c77bf72e890535becd1751bb45f64c597edb4c8c6b3"
+
+[[package]]
+name = "alloc-stdlib"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "94fb8275041c72129eb51b7d0322c29b8387a0386127718b096429201a5d6ece"
+dependencies = [
+ "alloc-no-stdlib",
+]
+
+[[package]]
 name = "android-tzdata"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
 
 [[package]]
 name = "android_system_properties"
@@ -65,45 +89,83 @@
  "planus",
  "serde",
 ]
 
 [[package]]
 name = "arrow2"
 version = "0.17.1"
-source = "git+https://github.com/Eventual-Inc/arrow2?branch=clark/expand-casting-support#2ace8097342d5634746915b094c5a3cdf53f75b9"
+source = "git+https://github.com/Eventual-Inc/arrow2?branch=clark/expand-casting-support#46bc134e386f597eed00a0396ea2de224d12943c"
 dependencies = [
  "ahash",
  "arrow-format",
+ "base64",
  "bytemuck",
  "chrono",
  "chrono-tz",
  "dyn-clone",
  "either",
  "ethnum",
+ "fallible-streaming-iterator",
  "foreign_vec",
+ "futures",
  "getrandom",
  "hash_hasher",
  "hashbrown 0.13.2",
  "lexical-core",
  "multiversion",
  "num-traits",
+ "parquet2",
  "rustc_version",
  "simdutf8",
+ "streaming-iterator",
  "strength_reduce",
 ]
 
 [[package]]
+name = "async-recursion"
+version = "1.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0e97ce7de6cf12de5d7226c73f5ba9811622f4db3a5b91b55c53e987e5f91cba"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.25",
+]
+
+[[package]]
+name = "async-stream"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cd56dd203fef61ac097dd65721a419ddccb106b2d2b70ba60a6b529f03961a51"
+dependencies = [
+ "async-stream-impl",
+ "futures-core",
+ "pin-project-lite",
+]
+
+[[package]]
+name = "async-stream-impl"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "16e62a023e7c117e27523144c5d2459f4397fcc3cab0085af8e2224f643a0193"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.25",
+]
+
+[[package]]
 name = "async-trait"
-version = "0.1.68"
+version = "0.1.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
+checksum = "a564d521dd56509c4c47480d00b80ee55f7e385ae48db5744c67ad50c92d2ebf"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
@@ -127,15 +189,15 @@
  "aws-types",
  "bytes",
  "fastrand",
  "hex",
  "http",
  "hyper",
  "ring",
- "time 0.3.22",
+ "time 0.3.23",
  "tokio",
  "tower",
  "tracing",
  "zeroize",
 ]
 
 [[package]]
@@ -297,15 +359,15 @@
  "hex",
  "hmac",
  "http",
  "once_cell",
  "percent-encoding",
  "regex",
  "sha2",
- "time 0.3.22",
+ "time 0.3.23",
  "tracing",
 ]
 
 [[package]]
 name = "aws-smithy-async"
 version = "0.55.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -437,15 +499,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "16a3d0bf4f324f4ef9793b86a1701d9700fbcdbd12a846da45eed104c634c6e8"
 dependencies = [
  "base64-simd",
  "itoa",
  "num-integer",
  "ryu",
- "time 0.3.22",
+ "time 0.3.23",
 ]
 
 [[package]]
 name = "aws-smithy-xml"
 version = "0.55.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1b9d12875731bd07e767be7baad95700c3137b56730ec9ddeedb52a5e5ca63b"
@@ -466,14 +528,29 @@
  "aws-smithy-types",
  "http",
  "rustc_version",
  "tracing",
 ]
 
 [[package]]
+name = "backtrace"
+version = "0.3.68"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4319208da049c43661739c5fade2ba182f09d1dc2299b32298d3a31692b17e12"
+dependencies = [
+ "addr2line",
+ "cc",
+ "cfg-if",
+ "libc",
+ "miniz_oxide",
+ "object",
+ "rustc-demangle",
+]
+
+[[package]]
 name = "base64"
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
 
 [[package]]
 name = "base64-simd"
@@ -497,23 +574,50 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "630be753d4e58660abd17930c71b647fe46c27ea6b63cc59e1e3851406972e42"
+
+[[package]]
 name = "block-buffer"
 version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
+name = "brotli"
+version = "3.3.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a1a0b1dbcc8ae29329621f8d4f0d835787c1c38bb1401979b49d13b0b305ff68"
+dependencies = [
+ "alloc-no-stdlib",
+ "alloc-stdlib",
+ "brotli-decompressor",
+]
+
+[[package]]
+name = "brotli-decompressor"
+version = "2.3.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4b6561fd3f895a11e8f72af2cb7d22e08366bebc2b6b57f7744c4bda27034744"
+dependencies = [
+ "alloc-no-stdlib",
+ "alloc-stdlib",
+]
+
+[[package]]
 name = "bumpalo"
 version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "bytemuck"
@@ -528,15 +632,15 @@
 name = "bytemuck_derive"
 version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fdde5c9cd29ebd706ce1b35600920a33550e402fc998a2e53ad3b42c3c47a192"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
@@ -558,14 +662,17 @@
 ]
 
 [[package]]
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
+dependencies = [
+ "jobserver",
+]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -582,28 +689,28 @@
  "time 0.1.45",
  "wasm-bindgen",
  "winapi",
 ]
 
 [[package]]
 name = "chrono-tz"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf9cc2b23599e6d7479755f3594285efb3f74a1bdca7a7374948bc831e23a552"
+checksum = "f1369bc6b9e9a7dfdae2055f6ec151fe9c554a9d23d357c0237cee2e25eaabb7"
 dependencies = [
  "chrono",
  "chrono-tz-build",
  "phf",
 ]
 
 [[package]]
 name = "chrono-tz-build"
-version = "0.1.0"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9998fb9f7e9b2111641485bf8beb32f92945f97f92a3d061f744cfef335f751"
+checksum = "e2f5ebdc942f57ed96d560a6d1a459bae5851102a25d5bf89dc04ae453e31ecf"
 dependencies = [
  "parse-zoneinfo",
  "phf",
  "phf_codegen",
 ]
 
 [[package]]
@@ -635,17 +742,17 @@
 name = "core-foundation-sys"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03e69e28e9f7f77debdedbaafa2866e1de9ba56df55a8bd7cfc724c25a09987c"
+checksum = "a17b76ff3a4162b0b27f354a0c87015ddad39d35f9c0c36607a3bdd175dde1f1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32c"
 version = "0.6.3"
@@ -693,19 +800,20 @@
 checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "daft"
-version = "0.1.8"
+version = "0.1.9"
 dependencies = [
  "daft-core",
  "daft-dsl",
  "daft-io",
+ "daft-parquet",
  "daft-table",
  "pyo3",
  "pyo3-log",
 ]
 
 [[package]]
 name = "daft-core"
@@ -750,14 +858,15 @@
  "serde",
 ]
 
 [[package]]
 name = "daft-io"
 version = "0.1.0"
 dependencies = [
+ "async-recursion",
  "async-trait",
  "aws-config",
  "aws-credential-types",
  "aws-sdk-s3",
  "aws-sig-auth",
  "aws-sigv4",
  "bytes",
@@ -774,14 +883,39 @@
  "snafu",
  "tempfile",
  "tokio",
  "url",
 ]
 
 [[package]]
+name = "daft-parquet"
+version = "0.1.0"
+dependencies = [
+ "arrow2",
+ "common-error",
+ "daft-core",
+ "daft-io",
+ "daft-table",
+ "futures",
+ "log",
+ "parquet2",
+ "pyo3",
+ "pyo3-log",
+ "snafu",
+ "tokio",
+]
+
+[[package]]
+name = "daft-plan"
+version = "0.1.0"
+dependencies = [
+ "pyo3",
+]
+
+[[package]]
 name = "daft-table"
 version = "0.1.0"
 dependencies = [
  "arrow2",
  "common-error",
  "daft-core",
  "daft-dsl",
@@ -862,15 +996,15 @@
 name = "errno"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "errno-dragonfly"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
@@ -882,14 +1016,20 @@
 [[package]]
 name = "ethnum"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0198b9d0078e0f30dedc7acbb21c974e838fc8fae3ee170128658a98cb2c1c04"
 
 [[package]]
+name = "fallible-streaming-iterator"
+version = "0.1.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7360491ce676a36bf9bb3c56c1aa791658183a54d2744120f27285738d90465a"
+
+[[package]]
 name = "fastrand"
 version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
 dependencies = [
  "instant",
 ]
@@ -986,15 +1126,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -1053,18 +1193,24 @@
 checksum = "80792593675e051cf94a4b111980da2ba60d4a83e43e0048c5693baab3977045"
 dependencies = [
  "color_quant",
  "weezl",
 ]
 
 [[package]]
+name = "gimli"
+version = "0.27.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6c80984affa11d98d1b88b66ac8853f143217b399d3c74116778ff8fdb4ed2e"
+
+[[package]]
 name = "h2"
-version = "0.3.19"
+version = "0.3.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d357c7ae988e7d2182f7d7871d0b963962420b0678b0997ce7de72001aeab782"
+checksum = "97ec8491ebaf99c8eaa73058b045fe58073cd6be7f596ac993ced0b0a0c01049"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
@@ -1097,26 +1243,17 @@
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
-version = "0.2.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
-
-[[package]]
-name = "hermit-abi"
-version = "0.3.1"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
+checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
 
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
@@ -1170,17 +1307,17 @@
 name = "httpdate"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c4a1e36c821dbe04574f602848a19f742f4fb3c98d40449f11bcad18d6b17421"
 
 [[package]]
 name = "hyper"
-version = "0.14.26"
+version = "0.14.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab302d72a6f11a3b910431ff93aae7e773078c769f0a3ef15fb9ec692ed147d4"
+checksum = "ffb1cfd654a8219eaef89881fdb3bb3b1cdc5fa75ded05d6933b2b382e395468"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "h2",
  "http",
@@ -1209,21 +1346,22 @@
  "rustls-native-certs",
  "tokio",
  "tokio-rustls 0.23.4",
 ]
 
 [[package]]
 name = "hyper-rustls"
-version = "0.24.0"
+version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0646026eb1b3eea4cd9ba47912ea5ce9cc07713d105b1a14698f4e6433d348b7"
+checksum = "8d78e1e73ec14cf7375674f74d7dde185c8206fd9dea6fb6295e8a98098aaa97"
 dependencies = [
+ "futures-util",
  "http",
  "hyper",
- "rustls 0.21.2",
+ "rustls 0.21.5",
  "tokio",
  "tokio-rustls 0.24.1",
 ]
 
 [[package]]
 name = "iana-time-zone"
 version = "0.1.57"
@@ -1302,42 +1440,50 @@
 
 [[package]]
 name = "io-lifetimes"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
- "hermit-abi 0.3.1",
+ "hermit-abi",
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "ipnet"
-version = "2.7.2"
+version = "2.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12b6ee2129af8d4fb011108c73d99a1b83a85977f23b82460c0ae2e25bb4b57f"
+checksum = "28b29a3cd74f0f4598934efe3aeba42bae0eb4680554128851ebbecb02af14e6"
 
 [[package]]
 name = "is-terminal"
-version = "0.4.7"
+version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
+checksum = "cb0889898416213fab133e1d33a0e5858a48177452750691bde3666d0fdbaf8b"
 dependencies = [
- "hermit-abi 0.3.1",
- "io-lifetimes",
- "rustix",
- "windows-sys 0.48.0",
+ "hermit-abi",
+ "rustix 0.38.3",
+ "windows-sys",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.6"
+version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+checksum = "62b02a5381cc465bd3041d84623d0fa3b66738b52b8e2fc3bab8ad63ab032f4a"
+
+[[package]]
+name = "jobserver"
+version = "0.1.26"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
+dependencies = [
+ "libc",
+]
 
 [[package]]
 name = "jpeg-decoder"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bc0000e42512c92e31c2252315bda326620a4e034105e900c98ec492fa077b3e"
 
@@ -1418,25 +1564,31 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.146"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "linux-raw-sys"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
+name = "linux-raw-sys"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "09fc20d2ca12cb9f044c93e3bd6d32d523e6e2ec3db4f7b2939cd99026ecd3f0"
+
+[[package]]
 name = "lock_api"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
@@ -1445,14 +1597,34 @@
 [[package]]
 name = "log"
 version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
+name = "lz4"
+version = "1.24.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7e9e2dd86df36ce760a60f6ff6ad526f7ba1f14ba0356f8254fb6905e6494df1"
+dependencies = [
+ "libc",
+ "lz4-sys",
+]
+
+[[package]]
+name = "lz4-sys"
+version = "1.9.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "57d27b317e207b10f69f5e75494119e391a96f48861ae870d1da6edac98ca900"
+dependencies = [
+ "cc",
+ "libc",
+]
+
+[[package]]
 name = "matrixmultiply"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "090126dc04f95dc0d1c1c91f61bdd474b3930ca064c1edc8a849da2c6cbe1e77"
 dependencies = [
  "autocfg",
  "rawpointer",
@@ -1508,15 +1680,15 @@
 name = "mio"
 version = "0.8.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
 dependencies = [
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "multiversion"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8cda45dade5144c2c929bf2ed6c24bebbba784e9198df049ec87d722b9462bd1"
@@ -1598,19 +1770,19 @@
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
- "hermit-abi 0.2.6",
+ "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "numpy"
 version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1622,14 +1794,23 @@
  "num-integer",
  "num-traits",
  "pyo3",
  "rustc-hash",
 ]
 
 [[package]]
+name = "object"
+version = "0.31.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8bda667d9f2b5051b8833f59f3bf748b28ef54f850f4fcb389a252aa383866d1"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "once_cell"
 version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "openssl-probe"
@@ -1663,14 +1844,43 @@
  "libc",
  "redox_syscall 0.3.5",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
+name = "parquet-format-safe"
+version = "0.2.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1131c54b167dd4e4799ce762e1ab01549ebb94d5bdd13e6ec1b467491c378e1f"
+dependencies = [
+ "async-trait",
+ "futures",
+]
+
+[[package]]
+name = "parquet2"
+version = "0.17.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "579fe5745f02cef3d5f236bfed216fd4693e49e4e920a13475c6132233283bce"
+dependencies = [
+ "async-stream",
+ "brotli",
+ "flate2",
+ "futures",
+ "lz4",
+ "parquet-format-safe",
+ "seq-macro",
+ "snap",
+ "streaming-decompression",
+ "xxhash-rust",
+ "zstd",
+]
+
+[[package]]
 name = "parse-zoneinfo"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c705f256449c60da65e11ff6626e0c16a0a0b96aaa348de61376b249bc340f41"
 dependencies = [
  "regex",
 ]
@@ -1679,98 +1889,104 @@
 name = "percent-encoding"
 version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
 name = "phf"
-version = "0.11.1"
+version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "928c6535de93548188ef63bb7c4036bd415cd8f36ad25af44b9789b2ee72a48c"
+checksum = "ade2d8b8f33c7333b51bcf0428d37e217e9f32192ae4772156f65063b8ce03dc"
 dependencies = [
  "phf_shared",
 ]
 
 [[package]]
 name = "phf_codegen"
-version = "0.11.1"
+version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a56ac890c5e3ca598bbdeaa99964edb5b0258a583a9eb6ef4e89fc85d9224770"
+checksum = "e8d39688d359e6b34654d328e262234662d16cc0f60ec8dcbe5e718709342a5a"
 dependencies = [
  "phf_generator",
  "phf_shared",
 ]
 
 [[package]]
 name = "phf_generator"
-version = "0.11.1"
+version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1181c94580fa345f50f19d738aaa39c0ed30a600d95cb2d3e23f94266f14fbf"
+checksum = "48e4cc64c2ad9ebe670cb8fd69dd50ae301650392e81c05f9bfcb2d5bdbc24b0"
 dependencies = [
  "phf_shared",
  "rand",
 ]
 
 [[package]]
 name = "phf_shared"
-version = "0.11.1"
+version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1fb5f6f826b772a8d4c0394209441e7d37cbbb967ae9c7e0e8134365c9ee676"
+checksum = "90fcb95eef784c2ac79119d1dd819e162b5da872ce6f3c3abe1e8ca1c082f72b"
 dependencies = [
  "siphasher",
 ]
 
 [[package]]
 name = "pin-project"
-version = "1.1.0"
+version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c95a7476719eab1e366eaf73d0260af3021184f18177925b07f54b30089ceead"
+checksum = "030ad2bc4db10a8944cb0d837f158bdfec4d4a4873ab701a95046770d11f8842"
 dependencies = [
  "pin-project-internal",
 ]
 
 [[package]]
 name = "pin-project-internal"
-version = "1.1.0"
+version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39407670928234ebc5e6e580247dd567ad73a3578460c5990f9503df207e8f07"
+checksum = "ec2e072ecce94ec471b13398d5402c188e76ac03cf74dd1a975161b23a3f6d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
+checksum = "4c40d25201921e5ff0c862a505c6557ea88568a4e3ace775ab55e93f2f4f9d57"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
+name = "pkg-config"
+version = "0.3.27"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
+
+[[package]]
 name = "planus"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fc1691dd09e82f428ce8d6310bd6d5da2557c82ff17694d2a32cad7242aea89f"
 dependencies = [
  "array-init-cursor",
 ]
 
 [[package]]
 name = "png"
 version = "0.17.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "59871cc5b6cce7eaccca5a802b4173377a1c2ba90654246789a8fa2334426d11"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "crc32fast",
  "fdeflate",
  "flate2",
  "miniz_oxide",
 ]
 
 [[package]]
@@ -1791,53 +2007,53 @@
  "lazy_static",
  "term",
  "unicode-width",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.60"
+version = "1.0.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
+checksum = "78803b62cbf1f46fde80d7c0e803111524b9877184cfe7c3033659490ac7a7da"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
+checksum = "ffb88ae05f306b4bfcde40ac4a51dc0b05936a9207a4b75b798c7729c4258a59"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
+checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
+checksum = "922ede8759e8600ad4da3195ae41259654b9c55da4f7eec84a0ccc7d067a70a4"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-log"
@@ -1848,40 +2064,40 @@
  "arc-swap",
  "log",
  "pyo3",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
+checksum = "8a5caec6a1dd355964a841fcbeeb1b89fe4146c87295573f94228911af3cc5a2"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
+checksum = "e0b78ccbb160db1556cdb6fd96c50334c5d4ec44dc5e0a968d0a1208fa0efa8b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.28"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
+checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1920,24 +2136,24 @@
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "redox_users"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b033d837a7cf162d7993aded9304e30a83213c648b6e389db233191f891e5c2b"
@@ -1945,28 +2161,40 @@
  "getrandom",
  "redox_syscall 0.2.16",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.4"
+version = "1.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
+checksum = "b2eae68fc220f7cf2532e4494aded17545fce192d59cd996e0fe7887f4ceb575"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-automata",
+ "regex-syntax",
+]
+
+[[package]]
+name = "regex-automata"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "83d3daa6976cffb758ec878f108ba0e062a45b2d6ca3a2cca965338855476caf"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.2"
+version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
+checksum = "2ab07dc67230e4a4718e70fd5c20055a4334b121f1f9db8fe63ef39ce9b8c846"
 
 [[package]]
 name = "reqwest"
 version = "0.11.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cde824a14b7c14f85caff81225f411faacc04a2013f41670f41443742b1c1c55"
 dependencies = [
@@ -1975,23 +2203,23 @@
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
  "http",
  "http-body",
  "hyper",
- "hyper-rustls 0.24.0",
+ "hyper-rustls 0.24.1",
  "ipnet",
  "js-sys",
  "log",
  "mime",
  "once_cell",
  "percent-encoding",
  "pin-project-lite",
- "rustls 0.21.2",
+ "rustls 0.21.5",
  "rustls-pemfile",
  "serde",
  "serde_json",
  "serde_urlencoded",
  "tokio",
  "tokio-rustls 0.24.1",
  "tokio-util",
@@ -2017,14 +2245,20 @@
  "spin",
  "untrusted",
  "web-sys",
  "winapi",
 ]
 
 [[package]]
+name = "rustc-demangle"
+version = "0.1.23"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+
+[[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustc_version"
@@ -2033,24 +2267,37 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.37.20"
+version = "0.37.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b96e891d04aa506a6d1f318d2771bcb1c7dfda84e126660ace067c9b474bb2c0"
+checksum = "4d69718bf81c6127a49dc64e44a742e8bb9213c0ff8869a22c308f84c1d4ab06"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "errno",
  "io-lifetimes",
  "libc",
- "linux-raw-sys",
- "windows-sys 0.48.0",
+ "linux-raw-sys 0.3.8",
+ "windows-sys",
+]
+
+[[package]]
+name = "rustix"
+version = "0.38.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ac5ffa1efe7548069688cd7028f32591853cd7b5b756d41bcffd2353e4fc75b4"
+dependencies = [
+ "bitflags 2.3.3",
+ "errno",
+ "libc",
+ "linux-raw-sys 0.4.3",
+ "windows-sys",
 ]
 
 [[package]]
 name = "rustls"
 version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fff78fc74d175294f4e83b28343315ffcfb114b156f0185e9741cb5570f50e2f"
@@ -2059,17 +2306,17 @@
  "ring",
  "sct",
  "webpki",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.21.2"
+version = "0.21.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e32ca28af694bc1bbf399c33a516dbdf1c90090b8ab23c2bc24f834aa2247f5f"
+checksum = "79ea77c539259495ce8ca47f53e66ae0330a8819f67e23ac96ca02f50e7b7d36"
 dependencies = [
  "log",
  "ring",
  "rustls-webpki",
  "sct",
 ]
 
@@ -2083,50 +2330,50 @@
  "rustls-pemfile",
  "schannel",
  "security-framework",
 ]
 
 [[package]]
 name = "rustls-pemfile"
-version = "1.0.2"
+version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d194b56d58803a43635bdc398cd17e383d6f71f9182b9a192c127ca42494a59b"
+checksum = "2d3987094b1d07b653b7dfdc3f70ce9a1da9c51ac18c1b06b662e4f9a0e9f4b2"
 dependencies = [
  "base64",
 ]
 
 [[package]]
 name = "rustls-webpki"
-version = "0.100.1"
+version = "0.101.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d6207cd5ed3d8dca7816f8f3725513a34609c0c765bf652b8c3cb4cfd87db46b"
+checksum = "15f36a6828982f422756984e47912a7a51dcbc2a197aa791158f8ca61cd8204e"
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.12"
+version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
+checksum = "dc31bd9b61a32c31f9650d18add92aa83a49ba979c143eefd27fe7177b05bd5f"
 
 [[package]]
 name = "ryu"
-version = "1.0.13"
+version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
+checksum = "fe232bdf6be8c8de797b22184ee71118d63780ea42ac85b61d1baa6d3b782ae9"
 
 [[package]]
 name = "schannel"
-version = "0.1.21"
+version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "713cfb06c7059f3588fb8044c0fad1d09e3c01d225e25b9220dbfdcf16dbb1b3"
+checksum = "0c3733bf4cf7ea0880754e19cb5a462007c4a8c1914bff372ccc95b464f1df88"
 dependencies = [
- "windows-sys 0.42.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
@@ -2143,15 +2390,15 @@
 
 [[package]]
 name = "security-framework"
 version = "2.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fc758eb7bffce5b308734e9b0c1468893cae9ff70ebf13e7090be8dcbcc83a8"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
@@ -2167,38 +2414,44 @@
 [[package]]
 name = "semver"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 
 [[package]]
+name = "seq-macro"
+version = "0.3.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "63134939175b3131fe4d2c131b103fd42f25ccca89423d43b5e4f267920ccf03"
+
+[[package]]
 name = "serde"
-version = "1.0.164"
+version = "1.0.171"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
+checksum = "30e27d1e4fd7659406c492fd6cfaf2066ba8773de45ca75e855590f856dc34a9"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.164"
+version = "1.0.171"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
+checksum = "389894603bd18c46fa56231694f8d827779c0951a667087194cf9de94ed24682"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.99"
+version = "1.0.100"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46266871c240a00b8f503b877622fe33430b3c7d963bdc0f2adc511e54a1eae3"
+checksum = "0f1e14e89be7aa4c4b78bdbdc9eb5bf8517829a600ae8eaa39a6e1d960b5185c"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -2269,41 +2522,47 @@
 checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "snafu"
-version = "0.7.4"
+version = "0.7.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb0656e7e3ffb70f6c39b3c2a86332bb74aa3c679da781642590f3c1118c5045"
+checksum = "e4de37ad025c587a29e8f3f5605c00f70b98715ef90b9061a815b9e59e9042d6"
 dependencies = [
  "doc-comment",
  "snafu-derive",
 ]
 
 [[package]]
 name = "snafu-derive"
-version = "0.7.4"
+version = "0.7.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "475b3bbe5245c26f2d8a6f62d67c1f30eb9fffeccee721c45d162c3ebbdf81b2"
+checksum = "990079665f075b699031e9c08fd3ab99be5029b96f3b78dc0709e8f77e4efebf"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "snap"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5e9f0ab6ef7eb7353d9119c170a436d1bf248eea575ac42d19d12f4e34130831"
+
+[[package]]
 name = "socket2"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "64a4a911eed85daf18834cfaa86a79b7d266ff93ff5ba14005426219480ed662"
 dependencies = [
  "libc",
  "winapi",
@@ -2318,14 +2577,29 @@
 [[package]]
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
+name = "streaming-decompression"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bf6cc3b19bfb128a8ad11026086e31d3ce9ad23f8ea37354b31383a187c44cf3"
+dependencies = [
+ "fallible-streaming-iterator",
+]
+
+[[package]]
+name = "streaming-iterator"
+version = "0.1.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2b2231b7c3057d5e4ad0156fb3dc807d900806020c5ffa3ee6ff2c8c76fb8520"
+
+[[package]]
 name = "strength_reduce"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe895eb47f22e2ddd4dabc02bce419d2e643c8e3b585c78158b349195bc24d82"
 
 [[package]]
 name = "subtle"
@@ -2342,17 +2616,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.18"
+version = "2.0.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
+checksum = "15e3fc8c0c74267e2df136e5e5fb656a464158aa57624053375eb9c8c6e25ae2"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -2373,16 +2647,16 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "31c0432476357e58790aaa47a8efb0c5138f137343f3b5f23bd36a27e3b0a6d6"
 dependencies = [
  "autocfg",
  "cfg-if",
  "fastrand",
  "redox_syscall 0.3.5",
- "rustix",
- "windows-sys 0.48.0",
+ "rustix 0.37.23",
+ "windows-sys",
 ]
 
 [[package]]
 name = "term"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c59df8ac95d96ff9bede18eb7300b0fda5e5d8d90960e76f8e14ae765eedbf1f"
@@ -2390,30 +2664,30 @@
  "dirs-next",
  "rustversion",
  "winapi",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.40"
+version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
+checksum = "a35fc5b8971143ca348fa6df4f024d4d55264f3468c71ad1c2f365b0a4d58c42"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.40"
+version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
+checksum = "463fe12d7993d3b327787537ce8dd4dfa058de32fc2b195ef3cde03dc4771e8f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "tiff"
 version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7449334f9ff2baf290d55d73983a7d6fa15e01198faef72af07e2a8db851e471"
@@ -2432,34 +2706,34 @@
  "libc",
  "wasi 0.10.0+wasi-snapshot-preview1",
  "winapi",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.22"
+version = "0.3.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea9e1b3cf1243ae005d9e74085d4d542f3125458f3a81af210d901dcd7411efd"
+checksum = "59e399c068f43a5d116fedaf73b203fa4f9c519f17e2b34f63221d3792f81446"
 dependencies = [
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
 
 [[package]]
 name = "time-macros"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
+checksum = "96ba15a897f3c86766b757e5ac7221554c6750054d74d5b28844fce5fb36a6c4"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
@@ -2473,39 +2747,40 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.28.2"
+version = "1.29.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94d7b1cfd2aa4011f2de74c2c4c63665e27a71006b0a192dcd2710272e73dfa2"
+checksum = "532826ff75199d5833b9d2c5fe410f29235e25704ee5f0ef599fb51c21f4a4da"
 dependencies = [
  "autocfg",
+ "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "pin-project-lite",
  "signal-hook-registry",
  "socket2",
  "tokio-macros",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "tokio-macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "tokio-rustls"
 version = "0.23.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c43ee83903113e03984cb9e5cebe6c04a5116269e900e3ddba8f068a62adda59"
@@ -2517,15 +2792,15 @@
 
 [[package]]
 name = "tokio-rustls"
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
 dependencies = [
- "rustls 0.21.2",
+ "rustls 0.21.5",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-stream"
 version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2595,15 +2870,15 @@
 name = "tracing-attributes"
 version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5f4f31f56159e98206da9efd823404b79b6ef3143b4a7ab76e67b1751b25a4ab"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.25",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
@@ -2627,17 +2902,17 @@
 name = "unicode-bidi"
 version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.9"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+checksum = "22049a19f4a68748a168c0fc439f9516686aa045927ff767eca0a85101fb6e73"
 
 [[package]]
 name = "unicode-normalization"
 version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
 dependencies = [
@@ -2735,15 +3010,15 @@
 checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.25",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2769,15 +3044,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.25",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.87"
@@ -2861,131 +3136,74 @@
 checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-sys"
-version = "0.42.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
-dependencies = [
- "windows_aarch64_gnullvm 0.42.2",
- "windows_aarch64_msvc 0.42.2",
- "windows_i686_gnu 0.42.2",
- "windows_i686_msvc 0.42.2",
- "windows_x86_64_gnu 0.42.2",
- "windows_x86_64_gnullvm 0.42.2",
- "windows_x86_64_msvc 0.42.2",
-]
-
-[[package]]
-name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.48.0"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
- "windows_aarch64_gnullvm 0.48.0",
- "windows_aarch64_msvc 0.48.0",
- "windows_i686_gnu 0.48.0",
- "windows_i686_msvc 0.48.0",
- "windows_x86_64_gnu 0.48.0",
- "windows_x86_64_gnullvm 0.48.0",
- "windows_x86_64_msvc 0.48.0",
+ "windows_aarch64_gnullvm",
+ "windows_aarch64_msvc",
+ "windows_i686_gnu",
+ "windows_i686_msvc",
+ "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
+ "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
-
-[[package]]
-name = "windows_aarch64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
-
-[[package]]
-name = "windows_aarch64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
-
-[[package]]
-name = "windows_i686_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
-
-[[package]]
-name = "windows_i686_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
-
-[[package]]
-name = "windows_x86_64_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
-
-[[package]]
-name = "windows_x86_64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
-
-[[package]]
-name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "winreg"
 version = "0.10.1"
@@ -3008,7 +3226,37 @@
 checksum = "735a71d46c4d68d71d4b24d03fdc2b98e38cea81730595801db779c04fe80d70"
 
 [[package]]
 name = "zeroize"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2a0956f1ba7c7909bfb66c2e9e4124ab6f6482560f6628b5aaeba39207c9aad9"
+
+[[package]]
+name = "zstd"
+version = "0.12.3+zstd.1.5.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "76eea132fb024e0e13fd9c2f5d5d595d8a967aa72382ac2f9d39fcc95afd0806"
+dependencies = [
+ "zstd-safe",
+]
+
+[[package]]
+name = "zstd-safe"
+version = "6.0.5+zstd.1.5.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d56d9e60b4b1758206c238a10165fbcae3ca37b01744e394c463463f6529d23b"
+dependencies = [
+ "libc",
+ "zstd-sys",
+]
+
+[[package]]
+name = "zstd-sys"
+version = "2.0.8+zstd.1.5.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5556e6ee25d32df2586c098bbfa278803692a20d0ab9565e049480d52707ec8c"
+dependencies = [
+ "cc",
+ "libc",
+ "pkg-config",
+]
```

### Comparing `getdaft-0.1.8/PKG-INFO` & `getdaft-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: getdaft
-Version: 0.1.8
+Version: 0.1.9
 Requires-Dist: pyarrow >= 6.0.1
 Requires-Dist: fsspec[http]
 Requires-Dist: loguru
 Requires-Dist: psutil
 Requires-Dist: typing-extensions >= 4.0.0; python_version < '3.8'
 Requires-Dist: pickle5 >= 0.0.12; python_version < '3.8'
-Requires-Dist: pydot; extra == 'viz'
-Requires-Dist: numpy; extra == 'numpy'
-Requires-Dist: pandas; extra == 'pandas'
 Requires-Dist: getdaft[aws, ray, pandas, numpy, viz]; extra == 'all'
+Requires-Dist: pandas; extra == 'pandas'
 Requires-Dist: ray[data, default]>=2.0.0; extra == 'ray'
 Requires-Dist: packaging; extra == 'ray'
 Requires-Dist: s3fs; extra == 'aws'
-Provides-Extra: viz
-Provides-Extra: numpy
-Provides-Extra: pandas
+Requires-Dist: numpy; extra == 'numpy'
+Requires-Dist: pydot; extra == 'viz'
 Provides-Extra: all
+Provides-Extra: pandas
 Provides-Extra: ray
 Provides-Extra: aws
+Provides-Extra: numpy
+Provides-Extra: viz
 License-File: LICENSE
 Summary: A Distributed DataFrame library for large scale complex data processing.
 Author-email: Eventual Inc <daft@eventualcomputing.com>
 Maintainer-email: Sammy Sidhu <sammy@eventualcomputing.com>, Jay Chia <jay@eventualcomputing.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
-Project-URL: homepage, https://www.getdaft.io
 Project-URL: repository, https://github.com/Eventual-Inc/Daft
+Project-URL: homepage, https://www.getdaft.io
 
 |Banner|
 
 |CI| |PyPI| |Latest Tag| |Coverage| |Slack|
 
 `Website <https://www.getdaft.io>`_ • `Docs <https://www.getdaft.io/projects/docs/>`_ • `Installation`_ • `10-minute tour of Daft <https://www.getdaft.io/projects/docs/en/latest/learn/10-min.html>`_ • `Community and Support <https://github.com/Eventual-Inc/Daft/discussions>`_
 
@@ -76,15 +76,15 @@
 
   Check out our `10-minute quickstart <https://www.getdaft.io/projects/docs/en/latest/learn/10-min.html>`_!
 
 In this example, we load images from an AWS S3 bucket's URLs and resize each image in the dataframe:
 
 .. code:: python
 
-    import daft as daft
+    import daft
 
     # Load a dataframe from filepaths in an S3 bucket
     df = daft.from_glob_path("s3://daft-public-data/laion-sample-images/*")
 
     # 1. Download column of image URLs as a column of bytes
     # 2. Decode the column of bytes into a column of images
     df = df.with_column("image", df["path"].url.download().image.decode())
```

