# Comparing `tmp/prql_python-0.9.1.tar.gz` & `tmp/prql_python-0.9.2.tar.gz`

## Comparing `prql_python-0.9.1.tar` & `prql_python-0.9.2.tar`

### file list

```diff
@@ -1,183 +1,183 @@
--rw-r--r--   0        0        0     2401 1970-01-01 00:00:00.000000 prql_python-0.9.1/local_dependencies/prql-compiler/Cargo.toml
--rw-r--r--   0     1001      123     2691 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/ARCHITECTURE.md
--rw-r--r--   0     1001      123      869 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/README.md
--rw-r--r--   0     1001      123     1223 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/benches/bench.rs
--rw-r--r--   0     1001      123    15010 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/codegen/ast.rs
--rw-r--r--   0     1001      123     2729 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/codegen/literal.rs
--rw-r--r--   0     1001      123     4411 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/codegen/mod.rs
--rw-r--r--   0     1001      123     3017 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/codegen/pl.rs
--rw-r--r--   0     1001      123    12249 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/error.rs
--rw-r--r--   0     1001      123     1114 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/generic.rs
--rw-r--r--   0     1001      123      143 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/mod.rs
--rw-r--r--   0     1001      123     4957 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/expr.rs
--rw-r--r--   0     1001      123     3897 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/extra/expr.rs
--rw-r--r--   0     1001      123       28 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/extra/mod.rs
--rw-r--r--   0     1001      123      568 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/extra/stmt.rs
--rw-r--r--   0     1001      123    10962 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/fold.rs
--rw-r--r--   0     1001      123     2632 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/lineage.rs
--rw-r--r--   0     1001      123     3840 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/mod.rs
--rw-r--r--   0     1001      123     1386 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/stmt.rs
--rw-r--r--   0     1001      123     6176 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/types.rs
--rw-r--r--   0     1001      123      418 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/utils.rs
--rw-r--r--   0     1001      123     1508 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/rq/expr.rs
--rw-r--r--   0     1001      123     8954 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/rq/fold.rs
--rw-r--r--   0     1001      123      874 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/rq/ids.rs
--rw-r--r--   0     1001      123     2371 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/rq/mod.rs
--rw-r--r--   0     1001      123     1530 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/rq/transform.rs
--rw-r--r--   0     1001      123      683 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/rq/utils.rs
--rw-r--r--   0     1001      123    12931 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/lib.rs
--rw-r--r--   0     1001      123     8442 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/parser.rs
--rw-r--r--   0     1001      123    10998 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/ast_expand.rs
--rw-r--r--   0     1001      123     6064 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/context.rs
--rw-r--r--   0     1001      123    17337 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/eval/mod.rs
--rw-r--r--   0     1001      123    36124 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/lowering.rs
--rw-r--r--   0     1001      123     9621 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/mod.rs
--rw-r--r--   0     1001      123    15641 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/module.rs
--rw-r--r--   0     1001      123     7472 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/reporting.rs
--rw-r--r--   0     1001      123    12386 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/context_impl.rs
--rw-r--r--   0     1001      123     5455 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/flatten.rs
--rw-r--r--   0     1001      123    40705 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/mod.rs
--rw-r--r--   0     1001      123      478 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names-2.snap
--rw-r--r--   0     1001      123      806 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names-3.snap
--rw-r--r--   0     1001      123      694 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names.snap
--rw-r--r--   0     1001      123     1956 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_1.snap
--rw-r--r--   0     1001      123     2976 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_nested.snap
--rw-r--r--   0     1001      123     2356 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_pipeline-2.snap
--rw-r--r--   0     1001      123      654 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_pipeline.snap
--rw-r--r--   0     1001      123     2672 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__named_args.snap
--rw-r--r--   0     1001      123     3639 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__variables_1.snap
--rw-r--r--   0     1001      123     5367 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__transforms__tests__aggregate_positional_arg-2.snap
--rw-r--r--   0     1001      123    36088 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/transforms.rs
--rw-r--r--   0     1001      123    12039 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/type_resolver.rs
--rw-r--r--   0     1001      123     4165 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/static_analysis.rs
--rw-r--r--   0     1001      123     6208 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/std.prql
--rw-r--r--   0     1001      123    10042 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/dialect.rs
--rw-r--r--   0     1001      123    35825 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/gen_expr.rs
--rw-r--r--   0     1001      123     7284 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/gen_projection.rs
--rw-r--r--   0     1001      123    21640 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/gen_query.rs
--rw-r--r--   0     1001      123     3127 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/keywords.rs
--rw-r--r--   0     1001      123     4566 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/mod.rs
--rw-r--r--   0     1001      123     5176 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/operators.rs
--rw-r--r--   0     1001      123    20817 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/anchor.rs
--rw-r--r--   0     1001      123     7166 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/ast.rs
--rw-r--r--   0     1001      123    10595 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/context.rs
--rw-r--r--   0     1001      123     9660 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/gen_query.rs
--rw-r--r--   0     1001      123     2188 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/mod.rs
--rw-r--r--   0     1001      123     7101 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/postprocess.rs
--rw-r--r--   0     1001      123    20042 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/preprocess.rs
--rw-r--r--   0     1001      123     5461 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/std.sql.prql
--rw-r--r--   0     1001      123       88 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/tests/mod.rs
--rw-r--r--   0     1001      123    75720 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/tests/test.rs
--rw-r--r--   0     1001      123     4090 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/tests/test_bad_error_messages.rs
--rw-r--r--   0     1001      123     6630 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/tests/test_error_messages.rs
--rw-r--r--   0     1001      123     1912 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/utils/id_gen.rs
--rw-r--r--   0     1001      123     3180 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/utils/mod.rs
--rw-r--r--   0     1001      123     3892 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/utils/toposort.rs
--rw-r--r--   0     1001      123     1612 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/README.md
--rw-r--r--   0     1001      123    10021 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/connection.rs
--rw-r--r--   0     1001      123    10818 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/albums.csv
--rw-r--r--   0     1001      123     7017 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/artists.csv
--rw-r--r--   0     1001      123     6743 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/customers.csv
--rw-r--r--   0     1001      123     1690 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/employees.csv
--rw-r--r--   0     1001      123      329 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/genres.csv
--rw-r--r--   0     1001      123    44678 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/invoice_items.csv
--rw-r--r--   0     1001      123    35719 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/invoices.csv
--rw-r--r--   0     1001      123      138 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/media_types.csv
--rw-r--r--   0     1001      123    58709 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/playlist_track.csv
--rw-r--r--   0     1001      123      299 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/playlists.csv
--rw-r--r--   0     1001      123     2193 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/schema.sql
--rw-r--r--   0     1001      123   241743 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/tracks.csv
--rw-r--r--   0     1001      123     2076 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/docker-compose.yml
--rw-r--r--   0     1001      123    14665 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/main.rs
--rw-r--r--   0     1001      123      188 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/aggregation.prql
--rw-r--r--   0     1001      123      813 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/arithmetic.prql
--rw-r--r--   0     1001      123      106 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/cast.prql
--rw-r--r--   0     1001      123       66 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/constants_only.prql
--rw-r--r--   0     1001      123       91 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/distinct.prql
--rw-r--r--   0     1001      123      160 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/distinct_on.prql
--rw-r--r--   0     1001      123      231 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/genre_counts.prql
--rw-r--r--   0     1001      123      148 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/group_all.prql
--rw-r--r--   0     1001      123      151 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/group_sort.prql
--rw-r--r--   0     1001      123      718 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/invoice_totals.prql
--rw-r--r--   0     1001      123      143 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/loop.prql
--rw-r--r--   0     1001      123      298 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/pipelines.prql
--rw-r--r--   0     1001      123      246 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/set_ops_remove.prql
--rw-r--r--   0     1001      123      272 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/sort.prql
--rw-r--r--   0     1001      123      179 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/switch.prql
--rw-r--r--   0     1001      123      481 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/window.prql
--rw-r--r--   0     1001      123      450 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@aggregation.prql.snap
--rw-r--r--   0     1001      123     1806 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@arithmetic.prql.snap
--rw-r--r--   0     1001      123      317 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@cast.prql.snap
--rw-r--r--   0     1001      123      282 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@constants_only.prql.snap
--rw-r--r--   0     1001      123      298 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@distinct.prql.snap
--rw-r--r--   0     1001      123      457 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@distinct_on.prql.snap
--rw-r--r--   0     1001      123      493 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@genre_counts.prql.snap
--rw-r--r--   0     1001      123      428 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@group_all.prql.snap
--rw-r--r--   0     1001      123      403 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@group_sort.prql.snap
--rw-r--r--   0     1001      123     1518 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@invoice_totals.prql.snap
--rw-r--r--   0     1001      123      426 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@loop.prql.snap
--rw-r--r--   0     1001      123      654 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@pipelines.prql.snap
--rw-r--r--   0     1001      123      660 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@set_ops_remove.prql.snap
--rw-r--r--   0     1001      123      609 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@sort.prql.snap
--rw-r--r--   0     1001      123      471 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@switch.prql.snap
--rw-r--r--   0     1001      123      895 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@window.prql.snap
--rw-r--r--   0     1001      123      301 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@aggregation.prql.snap
--rw-r--r--   0     1001      123     1185 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@arithmetic.prql.snap
--rw-r--r--   0     1001      123      775 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@cast.prql.snap
--rw-r--r--   0     1001      123      245 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@constants_only.prql.snap
--rw-r--r--   0     1001      123     2389 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@distinct.prql.snap
--rw-r--r--   0     1001      123      640 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@distinct_on.prql.snap
--rw-r--r--   0     1001      123      261 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@genre_counts.prql.snap
--rw-r--r--   0     1001      123      632 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@group_all.prql.snap
--rw-r--r--   0     1001      123      347 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@group_sort.prql.snap
--rw-r--r--   0     1001      123     1721 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@invoice_totals.prql.snap
--rw-r--r--   0     1001      123      366 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@loop.prql.snap
--rw-r--r--   0     1001      123     1177 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@pipelines.prql.snap
--rw-r--r--   0     1001      123      389 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@set_ops_remove.prql.snap
--rw-r--r--   0     1001      123      571 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@sort.prql.snap
--rw-r--r--   0     1001      123      438 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@switch.prql.snap
--rw-r--r--   0     1001      123     1020 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@window.prql.snap
--rw-r--r--   0     1001      123      525 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@aggregation.prql.snap
--rw-r--r--   0     1001      123     2369 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@arithmetic.prql.snap
--rw-r--r--   0     1001      123      440 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@cast.prql.snap
--rw-r--r--   0     1001      123      417 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@constants_only.prql.snap
--rw-r--r--   0     1001      123      380 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@distinct.prql.snap
--rw-r--r--   0     1001      123      715 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@distinct_on.prql.snap
--rw-r--r--   0     1001      123      503 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@genre_counts.prql.snap
--rw-r--r--   0     1001      123      615 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@group_all.prql.snap
--rw-r--r--   0     1001      123      616 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@group_sort.prql.snap
--rw-r--r--   0     1001      123     1741 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@invoice_totals.prql.snap
--rw-r--r--   0     1001      123      582 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@loop.prql.snap
--rw-r--r--   0     1001      123      872 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@pipelines.prql.snap
--rw-r--r--   0     1001      123      752 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@set_ops_remove.prql.snap
--rw-r--r--   0     1001      123      755 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@sort.prql.snap
--rw-r--r--   0     1001      123      622 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@switch.prql.snap
--rw-r--r--   0     1001      123     1314 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@window.prql.snap
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 prql_python-0.9.1/local_dependencies/prql_parser/Cargo.toml
--rw-r--r--   0     1001      123    13388 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_parser/src/expr.rs
--rw-r--r--   0     1001      123     1916 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_parser/src/interpolation.rs
--rw-r--r--   0     1001      123    11984 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_parser/src/lexer.rs
--rw-r--r--   0     1001      123    63208 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_parser/src/lib.rs
--rw-r--r--   0     1001      123     5385 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_parser/src/snapshots/prql_parser__test__pipeline_parse_tree.snap
--rw-r--r--   0     1001      123     1110 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_parser/src/span.rs
--rw-r--r--   0     1001      123     5411 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_parser/src/stmt.rs
--rw-r--r--   0        0        0      354 1970-01-01 00:00:00.000000 prql_python-0.9.1/local_dependencies/prql_ast/Cargo.toml
--rw-r--r--   0     1001      123     1452 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_ast/src/expr/generic.rs
--rw-r--r--   0     1001      123     4890 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_ast/src/expr/ident.rs
--rw-r--r--   0     1001      123      654 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_ast/src/expr/literal.rs
--rw-r--r--   0     1001      123     1214 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_ast/src/expr/ops.rs
--rw-r--r--   0     1001      123     3390 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_ast/src/expr.rs
--rw-r--r--   0     1001      123       59 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_ast/src/lib.rs
--rw-r--r--   0     1001      123     2571 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_ast/src/span.rs
--rw-r--r--   0     1001      123     1552 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_ast/src/stmt.rs
--rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 prql_python-0.9.1/Cargo.toml
--rw-r--r--   0     1001      123      647 2023-07-25 18:01:49.000000 prql_python-0.9.1/.gitignore
--rw-r--r--   0     1001      123      889 2023-07-25 18:01:49.000000 prql_python-0.9.1/README.md
--rw-r--r--   0     1001      123      257 2023-07-25 18:01:49.000000 prql_python-0.9.1/build.rs
--rw-r--r--   0     1001      123      974 2023-07-25 18:01:49.000000 prql_python-0.9.1/noxfile.py
--rw-r--r--   0     1001      123      482 2023-07-25 18:01:49.000000 prql_python-0.9.1/prql_python.pyi
--rw-r--r--   0     1001      123     1007 2023-07-25 18:01:49.000000 prql_python-0.9.1/pyproject.toml
--rw-r--r--   0     1001      123     2019 2023-07-25 18:01:49.000000 prql_python-0.9.1/python/tests/test_all.py
--rw-r--r--   0     1001      123       56 2023-07-25 18:01:49.000000 prql_python-0.9.1/requirements.txt
--rw-r--r--   0     1001      123     4104 2023-07-25 18:01:49.000000 prql_python-0.9.1/src/lib.rs
--rw-r--r--   0        0        0     1294 1970-01-01 00:00:00.000000 prql_python-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 prql_python-0.9.2/local_dependencies/prql-ast/Cargo.toml
+-rw-r--r--   0     1001      123     1452 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-ast/src/expr/generic.rs
+-rw-r--r--   0     1001      123     4890 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-ast/src/expr/ident.rs
+-rw-r--r--   0     1001      123      654 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-ast/src/expr/literal.rs
+-rw-r--r--   0     1001      123     1214 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-ast/src/expr/ops.rs
+-rw-r--r--   0     1001      123     3390 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-ast/src/expr.rs
+-rw-r--r--   0     1001      123       59 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-ast/src/lib.rs
+-rw-r--r--   0     1001      123     2571 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-ast/src/span.rs
+-rw-r--r--   0     1001      123     1552 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-ast/src/stmt.rs
+-rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 prql_python-0.9.2/local_dependencies/prql-parser/Cargo.toml
+-rw-r--r--   0     1001      123    13388 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-parser/src/expr.rs
+-rw-r--r--   0     1001      123     1916 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-parser/src/interpolation.rs
+-rw-r--r--   0     1001      123    11984 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-parser/src/lexer.rs
+-rw-r--r--   0     1001      123    63208 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-parser/src/lib.rs
+-rw-r--r--   0     1001      123     5385 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-parser/src/snapshots/prql_parser__test__pipeline_parse_tree.snap
+-rw-r--r--   0     1001      123     1110 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-parser/src/span.rs
+-rw-r--r--   0     1001      123     5411 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-parser/src/stmt.rs
+-rw-r--r--   0        0        0     2439 1970-01-01 00:00:00.000000 prql_python-0.9.2/local_dependencies/prql-compiler/Cargo.toml
+-rw-r--r--   0     1001      123     2691 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/ARCHITECTURE.md
+-rw-r--r--   0     1001      123      869 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/README.md
+-rw-r--r--   0     1001      123     1223 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/benches/bench.rs
+-rw-r--r--   0     1001      123    15010 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/codegen/ast.rs
+-rw-r--r--   0     1001      123     2729 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/codegen/literal.rs
+-rw-r--r--   0     1001      123     4411 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/codegen/mod.rs
+-rw-r--r--   0     1001      123     3017 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/codegen/pl.rs
+-rw-r--r--   0     1001      123    12249 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/error.rs
+-rw-r--r--   0     1001      123     1114 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/generic.rs
+-rw-r--r--   0     1001      123      143 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/mod.rs
+-rw-r--r--   0     1001      123     4957 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/expr.rs
+-rw-r--r--   0     1001      123     3897 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/extra/expr.rs
+-rw-r--r--   0     1001      123       28 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/extra/mod.rs
+-rw-r--r--   0     1001      123      568 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/extra/stmt.rs
+-rw-r--r--   0     1001      123    10962 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/fold.rs
+-rw-r--r--   0     1001      123     2632 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/lineage.rs
+-rw-r--r--   0     1001      123     3840 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/mod.rs
+-rw-r--r--   0     1001      123     1386 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/stmt.rs
+-rw-r--r--   0     1001      123     6176 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/types.rs
+-rw-r--r--   0     1001      123      418 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/utils.rs
+-rw-r--r--   0     1001      123     1508 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/rq/expr.rs
+-rw-r--r--   0     1001      123     8954 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/rq/fold.rs
+-rw-r--r--   0     1001      123      874 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/rq/ids.rs
+-rw-r--r--   0     1001      123     2371 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/rq/mod.rs
+-rw-r--r--   0     1001      123     1530 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/rq/transform.rs
+-rw-r--r--   0     1001      123      683 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/rq/utils.rs
+-rw-r--r--   0     1001      123    12931 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/lib.rs
+-rw-r--r--   0     1001      123     8442 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/parser.rs
+-rw-r--r--   0     1001      123    10998 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/ast_expand.rs
+-rw-r--r--   0     1001      123     6064 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/context.rs
+-rw-r--r--   0     1001      123    17337 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/eval/mod.rs
+-rw-r--r--   0     1001      123    36124 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/lowering.rs
+-rw-r--r--   0     1001      123     9621 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/mod.rs
+-rw-r--r--   0     1001      123    15641 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/module.rs
+-rw-r--r--   0     1001      123     7472 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/reporting.rs
+-rw-r--r--   0     1001      123    12386 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/context_impl.rs
+-rw-r--r--   0     1001      123     5455 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/flatten.rs
+-rw-r--r--   0     1001      123    40705 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/mod.rs
+-rw-r--r--   0     1001      123      478 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names-2.snap
+-rw-r--r--   0     1001      123      806 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names-3.snap
+-rw-r--r--   0     1001      123      694 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names.snap
+-rw-r--r--   0     1001      123     1956 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_1.snap
+-rw-r--r--   0     1001      123     2976 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_nested.snap
+-rw-r--r--   0     1001      123     2356 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_pipeline-2.snap
+-rw-r--r--   0     1001      123      654 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_pipeline.snap
+-rw-r--r--   0     1001      123     2672 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__named_args.snap
+-rw-r--r--   0     1001      123     3639 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__variables_1.snap
+-rw-r--r--   0     1001      123     5367 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__transforms__tests__aggregate_positional_arg-2.snap
+-rw-r--r--   0     1001      123    36088 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/transforms.rs
+-rw-r--r--   0     1001      123    12039 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/type_resolver.rs
+-rw-r--r--   0     1001      123     4165 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/static_analysis.rs
+-rw-r--r--   0     1001      123     6208 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/std.prql
+-rw-r--r--   0     1001      123    10042 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/dialect.rs
+-rw-r--r--   0     1001      123    35825 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/gen_expr.rs
+-rw-r--r--   0     1001      123     7284 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/gen_projection.rs
+-rw-r--r--   0     1001      123    21640 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/gen_query.rs
+-rw-r--r--   0     1001      123     3127 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/keywords.rs
+-rw-r--r--   0     1001      123     4566 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/mod.rs
+-rw-r--r--   0     1001      123     5176 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/operators.rs
+-rw-r--r--   0     1001      123    20817 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/anchor.rs
+-rw-r--r--   0     1001      123     7166 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/ast.rs
+-rw-r--r--   0     1001      123    10595 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/context.rs
+-rw-r--r--   0     1001      123     9660 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/gen_query.rs
+-rw-r--r--   0     1001      123     2188 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/mod.rs
+-rw-r--r--   0     1001      123     7101 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/postprocess.rs
+-rw-r--r--   0     1001      123    20042 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/preprocess.rs
+-rw-r--r--   0     1001      123     5461 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/std.sql.prql
+-rw-r--r--   0     1001      123       88 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/tests/mod.rs
+-rw-r--r--   0     1001      123    75720 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/tests/test.rs
+-rw-r--r--   0     1001      123     4090 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/tests/test_bad_error_messages.rs
+-rw-r--r--   0     1001      123     6630 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/tests/test_error_messages.rs
+-rw-r--r--   0     1001      123     1912 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/utils/id_gen.rs
+-rw-r--r--   0     1001      123     3180 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/utils/mod.rs
+-rw-r--r--   0     1001      123     3892 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/src/utils/toposort.rs
+-rw-r--r--   0     1001      123     1612 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/README.md
+-rw-r--r--   0     1001      123    10021 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/connection.rs
+-rw-r--r--   0     1001      123    10818 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/albums.csv
+-rw-r--r--   0     1001      123     7017 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/artists.csv
+-rw-r--r--   0     1001      123     6743 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/customers.csv
+-rw-r--r--   0     1001      123     1690 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/employees.csv
+-rw-r--r--   0     1001      123      329 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/genres.csv
+-rw-r--r--   0     1001      123    44678 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/invoice_items.csv
+-rw-r--r--   0     1001      123    35719 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/invoices.csv
+-rw-r--r--   0     1001      123      138 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/media_types.csv
+-rw-r--r--   0     1001      123    58709 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/playlist_track.csv
+-rw-r--r--   0     1001      123      299 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/playlists.csv
+-rw-r--r--   0     1001      123     2193 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/schema.sql
+-rw-r--r--   0     1001      123   241743 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/tracks.csv
+-rw-r--r--   0     1001      123     2076 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/docker-compose.yml
+-rw-r--r--   0     1001      123    14665 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/main.rs
+-rw-r--r--   0     1001      123      188 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/aggregation.prql
+-rw-r--r--   0     1001      123      813 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/arithmetic.prql
+-rw-r--r--   0     1001      123      106 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/cast.prql
+-rw-r--r--   0     1001      123       66 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/constants_only.prql
+-rw-r--r--   0     1001      123       91 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/distinct.prql
+-rw-r--r--   0     1001      123      160 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/distinct_on.prql
+-rw-r--r--   0     1001      123      231 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/genre_counts.prql
+-rw-r--r--   0     1001      123      148 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/group_all.prql
+-rw-r--r--   0     1001      123      151 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/group_sort.prql
+-rw-r--r--   0     1001      123      718 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/invoice_totals.prql
+-rw-r--r--   0     1001      123      143 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/loop.prql
+-rw-r--r--   0     1001      123      298 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/pipelines.prql
+-rw-r--r--   0     1001      123      246 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/set_ops_remove.prql
+-rw-r--r--   0     1001      123      272 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/sort.prql
+-rw-r--r--   0     1001      123      179 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/switch.prql
+-rw-r--r--   0     1001      123      481 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/window.prql
+-rw-r--r--   0     1001      123      450 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@aggregation.prql.snap
+-rw-r--r--   0     1001      123     1806 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@arithmetic.prql.snap
+-rw-r--r--   0     1001      123      317 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@cast.prql.snap
+-rw-r--r--   0     1001      123      282 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@constants_only.prql.snap
+-rw-r--r--   0     1001      123      298 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@distinct.prql.snap
+-rw-r--r--   0     1001      123      457 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@distinct_on.prql.snap
+-rw-r--r--   0     1001      123      493 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@genre_counts.prql.snap
+-rw-r--r--   0     1001      123      428 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@group_all.prql.snap
+-rw-r--r--   0     1001      123      403 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@group_sort.prql.snap
+-rw-r--r--   0     1001      123     1518 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@invoice_totals.prql.snap
+-rw-r--r--   0     1001      123      426 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@loop.prql.snap
+-rw-r--r--   0     1001      123      654 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@pipelines.prql.snap
+-rw-r--r--   0     1001      123      660 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@set_ops_remove.prql.snap
+-rw-r--r--   0     1001      123      609 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@sort.prql.snap
+-rw-r--r--   0     1001      123      471 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@switch.prql.snap
+-rw-r--r--   0     1001      123      895 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@window.prql.snap
+-rw-r--r--   0     1001      123      301 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@aggregation.prql.snap
+-rw-r--r--   0     1001      123     1185 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@arithmetic.prql.snap
+-rw-r--r--   0     1001      123      775 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@cast.prql.snap
+-rw-r--r--   0     1001      123      245 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@constants_only.prql.snap
+-rw-r--r--   0     1001      123     2389 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@distinct.prql.snap
+-rw-r--r--   0     1001      123      640 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@distinct_on.prql.snap
+-rw-r--r--   0     1001      123      261 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@genre_counts.prql.snap
+-rw-r--r--   0     1001      123      632 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@group_all.prql.snap
+-rw-r--r--   0     1001      123      347 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@group_sort.prql.snap
+-rw-r--r--   0     1001      123     1721 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@invoice_totals.prql.snap
+-rw-r--r--   0     1001      123      366 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@loop.prql.snap
+-rw-r--r--   0     1001      123     1177 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@pipelines.prql.snap
+-rw-r--r--   0     1001      123      389 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@set_ops_remove.prql.snap
+-rw-r--r--   0     1001      123      571 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@sort.prql.snap
+-rw-r--r--   0     1001      123      438 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@switch.prql.snap
+-rw-r--r--   0     1001      123     1020 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@window.prql.snap
+-rw-r--r--   0     1001      123      525 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@aggregation.prql.snap
+-rw-r--r--   0     1001      123     2369 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@arithmetic.prql.snap
+-rw-r--r--   0     1001      123      440 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@cast.prql.snap
+-rw-r--r--   0     1001      123      417 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@constants_only.prql.snap
+-rw-r--r--   0     1001      123      380 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@distinct.prql.snap
+-rw-r--r--   0     1001      123      715 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@distinct_on.prql.snap
+-rw-r--r--   0     1001      123      503 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@genre_counts.prql.snap
+-rw-r--r--   0     1001      123      615 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@group_all.prql.snap
+-rw-r--r--   0     1001      123      616 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@group_sort.prql.snap
+-rw-r--r--   0     1001      123     1741 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@invoice_totals.prql.snap
+-rw-r--r--   0     1001      123      582 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@loop.prql.snap
+-rw-r--r--   0     1001      123      872 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@pipelines.prql.snap
+-rw-r--r--   0     1001      123      752 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@set_ops_remove.prql.snap
+-rw-r--r--   0     1001      123      755 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@sort.prql.snap
+-rw-r--r--   0     1001      123      622 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@switch.prql.snap
+-rw-r--r--   0     1001      123     1314 2023-07-25 21:04:44.000000 prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@window.prql.snap
+-rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 prql_python-0.9.2/Cargo.toml
+-rw-r--r--   0     1001      123      647 2023-07-25 21:04:44.000000 prql_python-0.9.2/.gitignore
+-rw-r--r--   0     1001      123      889 2023-07-25 21:04:44.000000 prql_python-0.9.2/README.md
+-rw-r--r--   0     1001      123      257 2023-07-25 21:04:44.000000 prql_python-0.9.2/build.rs
+-rw-r--r--   0     1001      123      974 2023-07-25 21:04:44.000000 prql_python-0.9.2/noxfile.py
+-rw-r--r--   0     1001      123      482 2023-07-25 21:04:44.000000 prql_python-0.9.2/prql_python.pyi
+-rw-r--r--   0     1001      123     1007 2023-07-25 21:04:44.000000 prql_python-0.9.2/pyproject.toml
+-rw-r--r--   0     1001      123     2019 2023-07-25 21:04:44.000000 prql_python-0.9.2/python/tests/test_all.py
+-rw-r--r--   0     1001      123       56 2023-07-25 21:04:44.000000 prql_python-0.9.2/requirements.txt
+-rw-r--r--   0     1001      123     4104 2023-07-25 21:04:44.000000 prql_python-0.9.2/src/lib.rs
+-rw-r--r--   0        0        0     1294 1970-01-01 00:00:00.000000 prql_python-0.9.2/PKG-INFO
```

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/Cargo.toml` & `prql_python-0.9.2/local_dependencies/prql-compiler/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 description = "PRQL is a modern language for transforming data — a simple, powerful, pipelined SQL replacement."
 name = "prql-compiler"
 
 edition= "2021"
 license= "Apache-2.0"
 repository= "https://github.com/PRQL/prql"
 rust-version= "1.65.0"
-version= "0.9.1"
+version= "0.9.2"
 
 metadata.msrv = "1.65.0"
 
 [features]
 default = []
 # Technically tokio could be limited to external tests, but its types are in
 # signatures which would require lots of conditional compilation.
 test-dbs = ["duckdb", "rusqlite", "tokio"]
 test-dbs-external = ["chrono", "duckdb", "mysql", "pg_bigdecimal", "postgres", "rusqlite", "tiberius", "tokio", "tokio-util"]
 
 [dependencies]
-prql_ast = {path = "../prql_ast" }
-prql_parser = {path = "../prql_parser" }
+prql-ast = {path = "../prql-ast", version = "0.9.2" }
+prql-parser = {path = "../prql-parser", version = "0.9.2" }
 
 anstream = {version = "0.3.2", features = ["auto"]}
 anyhow = {version = "1.0.57", features = ["backtrace"]}
 ariadne = "0.3.0"
 csv = "1.2.0"
 enum-as-inner = "0.6.0"
 itertools = "0.11.0"
```

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/ARCHITECTURE.md` & `prql_python-0.9.2/local_dependencies/prql-compiler/ARCHITECTURE.md`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/README.md` & `prql_python-0.9.2/local_dependencies/prql-compiler/README.md`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/benches/bench.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/benches/bench.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/codegen/ast.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/codegen/ast.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/codegen/literal.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/codegen/literal.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/codegen/mod.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/codegen/mod.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/codegen/pl.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/codegen/pl.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/error.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/error.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/generic.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/generic.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/expr.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/expr.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/extra/expr.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/extra/expr.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/extra/stmt.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/extra/stmt.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/fold.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/fold.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/lineage.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/lineage.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/mod.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/mod.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/stmt.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/stmt.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/types.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/pl/types.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/rq/expr.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/rq/expr.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/rq/fold.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/rq/fold.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/rq/ids.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/rq/ids.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/rq/mod.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/rq/mod.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/rq/transform.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/rq/transform.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/rq/utils.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/ir/rq/utils.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/lib.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/lib.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/parser.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/parser.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/ast_expand.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/ast_expand.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/context.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/context.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/eval/mod.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/eval/mod.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/lowering.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/lowering.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/mod.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/mod.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/module.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/module.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/reporting.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/reporting.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/context_impl.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/context_impl.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/flatten.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/flatten.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/mod.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/mod.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names-3.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names-3.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_1.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_1.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_nested.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_nested.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_pipeline-2.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_pipeline-2.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_pipeline.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_pipeline.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__named_args.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__named_args.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__variables_1.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__variables_1.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__transforms__tests__aggregate_positional_arg-2.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__transforms__tests__aggregate_positional_arg-2.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/transforms.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/transforms.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/type_resolver.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/resolver/type_resolver.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/static_analysis.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/static_analysis.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/std.prql` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/semantic/std.prql`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/dialect.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/dialect.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/gen_expr.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/gen_expr.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/gen_projection.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/gen_projection.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/gen_query.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/gen_query.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/keywords.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/keywords.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/mod.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/mod.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/operators.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/operators.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/anchor.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/anchor.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/ast.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/ast.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/context.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/context.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/gen_query.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/gen_query.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/mod.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/mod.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/postprocess.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/postprocess.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/preprocess.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/srq/preprocess.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/std.sql.prql` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/sql/std.sql.prql`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/tests/test.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/tests/test.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/tests/test_bad_error_messages.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/tests/test_bad_error_messages.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/tests/test_error_messages.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/tests/test_error_messages.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/utils/id_gen.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/utils/id_gen.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/utils/mod.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/src/utils/toposort.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/src/utils/toposort.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/README.md` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/README.md`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/connection.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/connection.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/albums.csv` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/albums.csv`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/artists.csv` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/artists.csv`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/customers.csv` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/customers.csv`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/employees.csv` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/employees.csv`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/invoice_items.csv` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/invoice_items.csv`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/invoices.csv` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/invoices.csv`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/playlist_track.csv` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/playlist_track.csv`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/schema.sql` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/schema.sql`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/tracks.csv` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/data/chinook/tracks.csv`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/docker-compose.yml` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/main.rs` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/main.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/arithmetic.prql` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/arithmetic.prql`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/invoice_totals.prql` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/queries/invoice_totals.prql`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@arithmetic.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@arithmetic.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@invoice_totals.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@invoice_totals.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@pipelines.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@pipelines.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@set_ops_remove.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@set_ops_remove.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@sort.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@sort.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@window.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@window.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@arithmetic.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@arithmetic.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@cast.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@cast.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@distinct.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@distinct.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@distinct_on.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@distinct_on.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@group_all.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@group_all.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@invoice_totals.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@invoice_totals.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@pipelines.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@pipelines.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@sort.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@sort.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@window.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@window.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@aggregation.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@aggregation.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@arithmetic.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@arithmetic.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@distinct_on.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@distinct_on.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@group_all.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@group_all.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@group_sort.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@group_sort.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@invoice_totals.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@invoice_totals.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@loop.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@loop.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@pipelines.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@pipelines.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@set_ops_remove.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@set_ops_remove.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@sort.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@sort.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@switch.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@switch.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@window.prql.snap` & `prql_python-0.9.2/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@window.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql_parser/src/expr.rs` & `prql_python-0.9.2/local_dependencies/prql-parser/src/expr.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql_parser/src/interpolation.rs` & `prql_python-0.9.2/local_dependencies/prql-parser/src/interpolation.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql_parser/src/lexer.rs` & `prql_python-0.9.2/local_dependencies/prql-parser/src/lexer.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql_parser/src/lib.rs` & `prql_python-0.9.2/local_dependencies/prql-parser/src/lib.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql_parser/src/snapshots/prql_parser__test__pipeline_parse_tree.snap` & `prql_python-0.9.2/local_dependencies/prql-parser/src/snapshots/prql_parser__test__pipeline_parse_tree.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql_parser/src/span.rs` & `prql_python-0.9.2/local_dependencies/prql-parser/src/span.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql_parser/src/stmt.rs` & `prql_python-0.9.2/local_dependencies/prql-parser/src/stmt.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql_ast/src/expr/generic.rs` & `prql_python-0.9.2/local_dependencies/prql-ast/src/expr/generic.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql_ast/src/expr/ident.rs` & `prql_python-0.9.2/local_dependencies/prql-ast/src/expr/ident.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql_ast/src/expr/literal.rs` & `prql_python-0.9.2/local_dependencies/prql-ast/src/expr/literal.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql_ast/src/expr/ops.rs` & `prql_python-0.9.2/local_dependencies/prql-ast/src/expr/ops.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql_ast/src/expr.rs` & `prql_python-0.9.2/local_dependencies/prql-ast/src/expr.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql_ast/src/span.rs` & `prql_python-0.9.2/local_dependencies/prql-ast/src/span.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/local_dependencies/prql_ast/src/stmt.rs` & `prql_python-0.9.2/local_dependencies/prql-ast/src/stmt.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/Cargo.toml` & `prql_python-0.9.2/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 name = "prql-python"
 publish = false
 
 edition= "2021"
 license= "Apache-2.0"
 repository= "https://github.com/PRQL/prql"
 rust-version= "1.65.0"
-version= "0.9.1"
+version= "0.9.2"
 
 [lib]
 crate-type = ["cdylib"]
 name = "prql_python"
 
 [target.'cfg(not(target_family="wasm"))'.dependencies]
 pyo3 = {version = "0.19.0", features = ["abi3-py37"]}
```

### Comparing `prql_python-0.9.1/.gitignore` & `prql_python-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/README.md` & `prql_python-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/noxfile.py` & `prql_python-0.9.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/pyproject.toml` & `prql_python-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/python/tests/test_all.py` & `prql_python-0.9.2/python/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/src/lib.rs` & `prql_python-0.9.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.1/PKG-INFO` & `prql_python-0.9.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prql-python
-Version: 0.9.1
+Version: 0.9.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/PRQL/prql
```

