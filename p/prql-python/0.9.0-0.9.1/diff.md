# Comparing `tmp/prql_python-0.9.0.tar.gz` & `tmp/prql_python-0.9.1.tar.gz`

## Comparing `prql_python-0.9.0.tar` & `prql_python-0.9.1.tar`

### file list

```diff
@@ -1,180 +1,183 @@
--rw-r--r--   0        0        0      469 1970-01-01 00:00:00.000000 prql_python-0.9.0/local_dependencies/prql_ast/Cargo.toml
--rw-r--r--   0     1001      123     1452 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql_ast/src/expr/generic.rs
--rw-r--r--   0     1001      123     4890 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql_ast/src/expr/ident.rs
--rw-r--r--   0     1001      123      654 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql_ast/src/expr/literal.rs
--rw-r--r--   0     1001      123     1214 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql_ast/src/expr/ops.rs
--rw-r--r--   0     1001      123     3390 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql_ast/src/expr.rs
--rw-r--r--   0     1001      123       59 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql_ast/src/lib.rs
--rw-r--r--   0     1001      123     2571 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql_ast/src/span.rs
--rw-r--r--   0     1001      123     1552 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql_ast/src/stmt.rs
--rw-r--r--   0        0        0     2401 1970-01-01 00:00:00.000000 prql_python-0.9.0/local_dependencies/prql-compiler/Cargo.toml
--rw-r--r--   0     1001      123      869 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/README.md
--rw-r--r--   0     1001      123     1223 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/benches/bench.rs
--rw-r--r--   0     1001      123     2729 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/codegen/literal.rs
--rw-r--r--   0     1001      123    23108 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/codegen.rs
--rw-r--r--   0     1001      123    12249 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/error.rs
--rw-r--r--   0     1001      123     1114 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/generic.rs
--rw-r--r--   0     1001      123      143 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/mod.rs
--rw-r--r--   0     1001      123     4957 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/pl/expr.rs
--rw-r--r--   0     1001      123     3661 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/pl/extra/expr.rs
--rw-r--r--   0     1001      123       28 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/pl/extra/mod.rs
--rw-r--r--   0     1001      123     2359 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/pl/extra/stmt.rs
--rw-r--r--   0     1001      123    10962 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/pl/fold.rs
--rw-r--r--   0     1001      123     5356 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/pl/from_ast.rs
--rw-r--r--   0     1001      123     2632 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/pl/lineage.rs
--rw-r--r--   0     1001      123     3854 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/pl/mod.rs
--rw-r--r--   0     1001      123     1386 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/pl/stmt.rs
--rw-r--r--   0     1001      123     6016 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/pl/types.rs
--rw-r--r--   0     1001      123      418 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/pl/utils.rs
--rw-r--r--   0     1001      123     1508 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/rq/expr.rs
--rw-r--r--   0     1001      123     8954 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/rq/fold.rs
--rw-r--r--   0     1001      123      874 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/rq/ids.rs
--rw-r--r--   0     1001      123     2371 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/rq/mod.rs
--rw-r--r--   0     1001      123     1530 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/rq/transform.rs
--rw-r--r--   0     1001      123      683 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/rq/utils.rs
--rw-r--r--   0     1001      123    12862 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/lib.rs
--rw-r--r--   0     1001      123     8464 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/parser.rs
--rw-r--r--   0     1001      123     6043 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/context.rs
--rw-r--r--   0     1001      123    17218 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/eval/mod.rs
--rw-r--r--   0     1001      123    36027 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/lowering.rs
--rw-r--r--   0     1001      123     9199 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/mod.rs
--rw-r--r--   0     1001      123    15641 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/module.rs
--rw-r--r--   0     1001      123     7466 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/reporting.rs
--rw-r--r--   0     1001      123    12328 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/context_impl.rs
--rw-r--r--   0     1001      123     5455 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/flatten.rs
--rw-r--r--   0     1001      123    41194 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/mod.rs
--rw-r--r--   0     1001      123      467 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names-2.snap
--rw-r--r--   0     1001      123      795 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names-3.snap
--rw-r--r--   0     1001      123      683 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names.snap
--rw-r--r--   0     1001      123     1956 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_1.snap
--rw-r--r--   0     1001      123     2976 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_nested.snap
--rw-r--r--   0     1001      123     2356 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_pipeline-2.snap
--rw-r--r--   0     1001      123      654 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_pipeline.snap
--rw-r--r--   0     1001      123     2672 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__named_args.snap
--rw-r--r--   0     1001      123     3639 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__variables_1.snap
--rw-r--r--   0     1001      123     5351 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__transforms__tests__aggregate_positional_arg-2.snap
--rw-r--r--   0     1001      123    35936 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/transforms.rs
--rw-r--r--   0     1001      123    11917 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/type_resolver.rs
--rw-r--r--   0     1001      123     4165 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/static_analysis.rs
--rw-r--r--   0     1001      123     6140 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/std.prql
--rw-r--r--   0     1001      123    10042 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/dialect.rs
--rw-r--r--   0     1001      123    35825 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/gen_expr.rs
--rw-r--r--   0     1001      123     7284 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/gen_projection.rs
--rw-r--r--   0     1001      123    21640 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/gen_query.rs
--rw-r--r--   0     1001      123     3127 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/keywords.rs
--rw-r--r--   0     1001      123     4566 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/mod.rs
--rw-r--r--   0     1001      123     5176 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/operators.rs
--rw-r--r--   0     1001      123    20817 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/srq/anchor.rs
--rw-r--r--   0     1001      123     7166 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/srq/ast.rs
--rw-r--r--   0     1001      123    10595 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/srq/context.rs
--rw-r--r--   0     1001      123     9660 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/srq/gen_query.rs
--rw-r--r--   0     1001      123     2188 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/srq/mod.rs
--rw-r--r--   0     1001      123     7101 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/srq/postprocess.rs
--rw-r--r--   0     1001      123    20042 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/srq/preprocess.rs
--rw-r--r--   0     1001      123     5461 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/std.sql.prql
--rw-r--r--   0     1001      123       88 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/tests/mod.rs
--rw-r--r--   0     1001      123    75737 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/tests/test.rs
--rw-r--r--   0     1001      123     4090 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/tests/test_bad_error_messages.rs
--rw-r--r--   0     1001      123     6630 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/tests/test_error_messages.rs
--rw-r--r--   0     1001      123     1912 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/utils/id_gen.rs
--rw-r--r--   0     1001      123     3180 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/utils/mod.rs
--rw-r--r--   0     1001      123     3892 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/src/utils/toposort.rs
--rw-r--r--   0     1001      123     1612 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/README.md
--rw-r--r--   0     1001      123    10021 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/connection.rs
--rw-r--r--   0     1001      123    10818 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/data/chinook/albums.csv
--rw-r--r--   0     1001      123     7017 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/data/chinook/artists.csv
--rw-r--r--   0     1001      123     6743 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/data/chinook/customers.csv
--rw-r--r--   0     1001      123     1690 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/data/chinook/employees.csv
--rw-r--r--   0     1001      123      329 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/data/chinook/genres.csv
--rw-r--r--   0     1001      123    44678 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/data/chinook/invoice_items.csv
--rw-r--r--   0     1001      123    35719 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/data/chinook/invoices.csv
--rw-r--r--   0     1001      123      138 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/data/chinook/media_types.csv
--rw-r--r--   0     1001      123    58709 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/data/chinook/playlist_track.csv
--rw-r--r--   0     1001      123      299 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/data/chinook/playlists.csv
--rw-r--r--   0     1001      123     2193 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/data/chinook/schema.sql
--rw-r--r--   0     1001      123   241743 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/data/chinook/tracks.csv
--rw-r--r--   0     1001      123     2076 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/docker-compose.yml
--rw-r--r--   0     1001      123    14665 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/main.rs
--rw-r--r--   0     1001      123      188 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/queries/aggregation.prql
--rw-r--r--   0     1001      123      813 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/queries/arithmetic.prql
--rw-r--r--   0     1001      123      106 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/queries/cast.prql
--rw-r--r--   0     1001      123       66 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/queries/constants_only.prql
--rw-r--r--   0     1001      123       91 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/queries/distinct.prql
--rw-r--r--   0     1001      123      160 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/queries/distinct_on.prql
--rw-r--r--   0     1001      123      231 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/queries/genre_counts.prql
--rw-r--r--   0     1001      123      148 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/queries/group_all.prql
--rw-r--r--   0     1001      123      151 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/queries/group_sort.prql
--rw-r--r--   0     1001      123      718 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/queries/invoice_totals.prql
--rw-r--r--   0     1001      123      143 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/queries/loop.prql
--rw-r--r--   0     1001      123      298 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/queries/pipelines.prql
--rw-r--r--   0     1001      123      246 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/queries/set_ops_remove.prql
--rw-r--r--   0     1001      123      272 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/queries/sort.prql
--rw-r--r--   0     1001      123      179 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/queries/switch.prql
--rw-r--r--   0     1001      123      481 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/queries/window.prql
--rw-r--r--   0     1001      123      450 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@aggregation.prql.snap
--rw-r--r--   0     1001      123     1806 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@arithmetic.prql.snap
--rw-r--r--   0     1001      123      317 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@cast.prql.snap
--rw-r--r--   0     1001      123      282 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@constants_only.prql.snap
--rw-r--r--   0     1001      123      298 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@distinct.prql.snap
--rw-r--r--   0     1001      123      457 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@distinct_on.prql.snap
--rw-r--r--   0     1001      123      493 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@genre_counts.prql.snap
--rw-r--r--   0     1001      123      428 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@group_all.prql.snap
--rw-r--r--   0     1001      123      403 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@group_sort.prql.snap
--rw-r--r--   0     1001      123     1518 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@invoice_totals.prql.snap
--rw-r--r--   0     1001      123      426 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@loop.prql.snap
--rw-r--r--   0     1001      123      654 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@pipelines.prql.snap
--rw-r--r--   0     1001      123      642 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@set_ops_remove.prql.snap
--rw-r--r--   0     1001      123      609 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@sort.prql.snap
--rw-r--r--   0     1001      123      471 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@switch.prql.snap
--rw-r--r--   0     1001      123      895 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@window.prql.snap
--rw-r--r--   0     1001      123      301 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@aggregation.prql.snap
--rw-r--r--   0     1001      123     1185 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@arithmetic.prql.snap
--rw-r--r--   0     1001      123      775 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@cast.prql.snap
--rw-r--r--   0     1001      123      245 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@constants_only.prql.snap
--rw-r--r--   0     1001      123     2389 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@distinct.prql.snap
--rw-r--r--   0     1001      123      640 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@distinct_on.prql.snap
--rw-r--r--   0     1001      123      261 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@genre_counts.prql.snap
--rw-r--r--   0     1001      123      632 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@group_all.prql.snap
--rw-r--r--   0     1001      123      347 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@group_sort.prql.snap
--rw-r--r--   0     1001      123     1721 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@invoice_totals.prql.snap
--rw-r--r--   0     1001      123      366 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@loop.prql.snap
--rw-r--r--   0     1001      123     1177 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@pipelines.prql.snap
--rw-r--r--   0     1001      123      389 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@set_ops_remove.prql.snap
--rw-r--r--   0     1001      123      571 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@sort.prql.snap
--rw-r--r--   0     1001      123      438 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@switch.prql.snap
--rw-r--r--   0     1001      123     1020 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@window.prql.snap
--rw-r--r--   0     1001      123      525 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@aggregation.prql.snap
--rw-r--r--   0     1001      123     2369 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@arithmetic.prql.snap
--rw-r--r--   0     1001      123      440 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@cast.prql.snap
--rw-r--r--   0     1001      123      417 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@constants_only.prql.snap
--rw-r--r--   0     1001      123      380 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@distinct.prql.snap
--rw-r--r--   0     1001      123      715 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@distinct_on.prql.snap
--rw-r--r--   0     1001      123      503 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@genre_counts.prql.snap
--rw-r--r--   0     1001      123      615 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@group_all.prql.snap
--rw-r--r--   0     1001      123      616 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@group_sort.prql.snap
--rw-r--r--   0     1001      123     1741 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@invoice_totals.prql.snap
--rw-r--r--   0     1001      123      582 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@loop.prql.snap
--rw-r--r--   0     1001      123      872 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@pipelines.prql.snap
--rw-r--r--   0     1001      123      752 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@set_ops_remove.prql.snap
--rw-r--r--   0     1001      123      755 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@sort.prql.snap
--rw-r--r--   0     1001      123      622 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@switch.prql.snap
--rw-r--r--   0     1001      123     1314 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@window.prql.snap
--rw-r--r--   0        0        0      834 1970-01-01 00:00:00.000000 prql_python-0.9.0/local_dependencies/prql_parser/Cargo.toml
--rw-r--r--   0     1001      123    13388 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql_parser/src/expr.rs
--rw-r--r--   0     1001      123     1916 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql_parser/src/interpolation.rs
--rw-r--r--   0     1001      123    11984 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql_parser/src/lexer.rs
--rw-r--r--   0     1001      123    63208 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql_parser/src/lib.rs
--rw-r--r--   0     1001      123     5385 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql_parser/src/snapshots/prql_parser__test__pipeline_parse_tree.snap
--rw-r--r--   0     1001      123     1110 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql_parser/src/span.rs
--rw-r--r--   0     1001      123     5310 2023-07-25 06:00:03.000000 prql_python-0.9.0/local_dependencies/prql_parser/src/stmt.rs
--rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 prql_python-0.9.0/Cargo.toml
--rw-r--r--   0     1001      123      647 2023-07-25 06:00:03.000000 prql_python-0.9.0/.gitignore
--rw-r--r--   0     1001      123      889 2023-07-25 06:00:03.000000 prql_python-0.9.0/README.md
--rw-r--r--   0     1001      123      257 2023-07-25 06:00:03.000000 prql_python-0.9.0/build.rs
--rw-r--r--   0     1001      123      974 2023-07-25 06:00:03.000000 prql_python-0.9.0/noxfile.py
--rw-r--r--   0     1001      123      482 2023-07-25 06:00:03.000000 prql_python-0.9.0/prql_python.pyi
--rw-r--r--   0     1001      123     1007 2023-07-25 06:00:03.000000 prql_python-0.9.0/pyproject.toml
--rw-r--r--   0     1001      123     2019 2023-07-25 06:00:03.000000 prql_python-0.9.0/python/tests/test_all.py
--rw-r--r--   0     1001      123       56 2023-07-25 06:00:03.000000 prql_python-0.9.0/requirements.txt
--rw-r--r--   0     1001      123     4104 2023-07-25 06:00:03.000000 prql_python-0.9.0/src/lib.rs
--rw-r--r--   0        0        0     1294 1970-01-01 00:00:00.000000 prql_python-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2401 1970-01-01 00:00:00.000000 prql_python-0.9.1/local_dependencies/prql-compiler/Cargo.toml
+-rw-r--r--   0     1001      123     2691 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/ARCHITECTURE.md
+-rw-r--r--   0     1001      123      869 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/README.md
+-rw-r--r--   0     1001      123     1223 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/benches/bench.rs
+-rw-r--r--   0     1001      123    15010 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/codegen/ast.rs
+-rw-r--r--   0     1001      123     2729 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/codegen/literal.rs
+-rw-r--r--   0     1001      123     4411 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/codegen/mod.rs
+-rw-r--r--   0     1001      123     3017 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/codegen/pl.rs
+-rw-r--r--   0     1001      123    12249 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/error.rs
+-rw-r--r--   0     1001      123     1114 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/generic.rs
+-rw-r--r--   0     1001      123      143 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/mod.rs
+-rw-r--r--   0     1001      123     4957 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/expr.rs
+-rw-r--r--   0     1001      123     3897 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/extra/expr.rs
+-rw-r--r--   0     1001      123       28 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/extra/mod.rs
+-rw-r--r--   0     1001      123      568 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/extra/stmt.rs
+-rw-r--r--   0     1001      123    10962 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/fold.rs
+-rw-r--r--   0     1001      123     2632 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/lineage.rs
+-rw-r--r--   0     1001      123     3840 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/mod.rs
+-rw-r--r--   0     1001      123     1386 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/stmt.rs
+-rw-r--r--   0     1001      123     6176 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/types.rs
+-rw-r--r--   0     1001      123      418 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/utils.rs
+-rw-r--r--   0     1001      123     1508 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/rq/expr.rs
+-rw-r--r--   0     1001      123     8954 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/rq/fold.rs
+-rw-r--r--   0     1001      123      874 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/rq/ids.rs
+-rw-r--r--   0     1001      123     2371 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/rq/mod.rs
+-rw-r--r--   0     1001      123     1530 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/rq/transform.rs
+-rw-r--r--   0     1001      123      683 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/rq/utils.rs
+-rw-r--r--   0     1001      123    12931 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/lib.rs
+-rw-r--r--   0     1001      123     8442 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/parser.rs
+-rw-r--r--   0     1001      123    10998 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/ast_expand.rs
+-rw-r--r--   0     1001      123     6064 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/context.rs
+-rw-r--r--   0     1001      123    17337 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/eval/mod.rs
+-rw-r--r--   0     1001      123    36124 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/lowering.rs
+-rw-r--r--   0     1001      123     9621 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/mod.rs
+-rw-r--r--   0     1001      123    15641 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/module.rs
+-rw-r--r--   0     1001      123     7472 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/reporting.rs
+-rw-r--r--   0     1001      123    12386 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/context_impl.rs
+-rw-r--r--   0     1001      123     5455 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/flatten.rs
+-rw-r--r--   0     1001      123    40705 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/mod.rs
+-rw-r--r--   0     1001      123      478 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names-2.snap
+-rw-r--r--   0     1001      123      806 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names-3.snap
+-rw-r--r--   0     1001      123      694 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names.snap
+-rw-r--r--   0     1001      123     1956 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_1.snap
+-rw-r--r--   0     1001      123     2976 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_nested.snap
+-rw-r--r--   0     1001      123     2356 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_pipeline-2.snap
+-rw-r--r--   0     1001      123      654 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_pipeline.snap
+-rw-r--r--   0     1001      123     2672 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__named_args.snap
+-rw-r--r--   0     1001      123     3639 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__variables_1.snap
+-rw-r--r--   0     1001      123     5367 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__transforms__tests__aggregate_positional_arg-2.snap
+-rw-r--r--   0     1001      123    36088 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/transforms.rs
+-rw-r--r--   0     1001      123    12039 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/type_resolver.rs
+-rw-r--r--   0     1001      123     4165 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/static_analysis.rs
+-rw-r--r--   0     1001      123     6208 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/std.prql
+-rw-r--r--   0     1001      123    10042 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/dialect.rs
+-rw-r--r--   0     1001      123    35825 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/gen_expr.rs
+-rw-r--r--   0     1001      123     7284 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/gen_projection.rs
+-rw-r--r--   0     1001      123    21640 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/gen_query.rs
+-rw-r--r--   0     1001      123     3127 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/keywords.rs
+-rw-r--r--   0     1001      123     4566 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/mod.rs
+-rw-r--r--   0     1001      123     5176 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/operators.rs
+-rw-r--r--   0     1001      123    20817 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/anchor.rs
+-rw-r--r--   0     1001      123     7166 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/ast.rs
+-rw-r--r--   0     1001      123    10595 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/context.rs
+-rw-r--r--   0     1001      123     9660 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/gen_query.rs
+-rw-r--r--   0     1001      123     2188 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/mod.rs
+-rw-r--r--   0     1001      123     7101 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/postprocess.rs
+-rw-r--r--   0     1001      123    20042 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/preprocess.rs
+-rw-r--r--   0     1001      123     5461 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/std.sql.prql
+-rw-r--r--   0     1001      123       88 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/tests/mod.rs
+-rw-r--r--   0     1001      123    75720 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/tests/test.rs
+-rw-r--r--   0     1001      123     4090 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/tests/test_bad_error_messages.rs
+-rw-r--r--   0     1001      123     6630 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/tests/test_error_messages.rs
+-rw-r--r--   0     1001      123     1912 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/utils/id_gen.rs
+-rw-r--r--   0     1001      123     3180 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/utils/mod.rs
+-rw-r--r--   0     1001      123     3892 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/src/utils/toposort.rs
+-rw-r--r--   0     1001      123     1612 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/README.md
+-rw-r--r--   0     1001      123    10021 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/connection.rs
+-rw-r--r--   0     1001      123    10818 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/albums.csv
+-rw-r--r--   0     1001      123     7017 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/artists.csv
+-rw-r--r--   0     1001      123     6743 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/customers.csv
+-rw-r--r--   0     1001      123     1690 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/employees.csv
+-rw-r--r--   0     1001      123      329 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/genres.csv
+-rw-r--r--   0     1001      123    44678 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/invoice_items.csv
+-rw-r--r--   0     1001      123    35719 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/invoices.csv
+-rw-r--r--   0     1001      123      138 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/media_types.csv
+-rw-r--r--   0     1001      123    58709 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/playlist_track.csv
+-rw-r--r--   0     1001      123      299 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/playlists.csv
+-rw-r--r--   0     1001      123     2193 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/schema.sql
+-rw-r--r--   0     1001      123   241743 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/tracks.csv
+-rw-r--r--   0     1001      123     2076 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/docker-compose.yml
+-rw-r--r--   0     1001      123    14665 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/main.rs
+-rw-r--r--   0     1001      123      188 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/aggregation.prql
+-rw-r--r--   0     1001      123      813 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/arithmetic.prql
+-rw-r--r--   0     1001      123      106 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/cast.prql
+-rw-r--r--   0     1001      123       66 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/constants_only.prql
+-rw-r--r--   0     1001      123       91 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/distinct.prql
+-rw-r--r--   0     1001      123      160 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/distinct_on.prql
+-rw-r--r--   0     1001      123      231 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/genre_counts.prql
+-rw-r--r--   0     1001      123      148 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/group_all.prql
+-rw-r--r--   0     1001      123      151 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/group_sort.prql
+-rw-r--r--   0     1001      123      718 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/invoice_totals.prql
+-rw-r--r--   0     1001      123      143 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/loop.prql
+-rw-r--r--   0     1001      123      298 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/pipelines.prql
+-rw-r--r--   0     1001      123      246 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/set_ops_remove.prql
+-rw-r--r--   0     1001      123      272 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/sort.prql
+-rw-r--r--   0     1001      123      179 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/switch.prql
+-rw-r--r--   0     1001      123      481 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/window.prql
+-rw-r--r--   0     1001      123      450 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@aggregation.prql.snap
+-rw-r--r--   0     1001      123     1806 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@arithmetic.prql.snap
+-rw-r--r--   0     1001      123      317 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@cast.prql.snap
+-rw-r--r--   0     1001      123      282 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@constants_only.prql.snap
+-rw-r--r--   0     1001      123      298 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@distinct.prql.snap
+-rw-r--r--   0     1001      123      457 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@distinct_on.prql.snap
+-rw-r--r--   0     1001      123      493 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@genre_counts.prql.snap
+-rw-r--r--   0     1001      123      428 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@group_all.prql.snap
+-rw-r--r--   0     1001      123      403 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@group_sort.prql.snap
+-rw-r--r--   0     1001      123     1518 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@invoice_totals.prql.snap
+-rw-r--r--   0     1001      123      426 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@loop.prql.snap
+-rw-r--r--   0     1001      123      654 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@pipelines.prql.snap
+-rw-r--r--   0     1001      123      660 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@set_ops_remove.prql.snap
+-rw-r--r--   0     1001      123      609 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@sort.prql.snap
+-rw-r--r--   0     1001      123      471 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@switch.prql.snap
+-rw-r--r--   0     1001      123      895 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@window.prql.snap
+-rw-r--r--   0     1001      123      301 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@aggregation.prql.snap
+-rw-r--r--   0     1001      123     1185 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@arithmetic.prql.snap
+-rw-r--r--   0     1001      123      775 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@cast.prql.snap
+-rw-r--r--   0     1001      123      245 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@constants_only.prql.snap
+-rw-r--r--   0     1001      123     2389 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@distinct.prql.snap
+-rw-r--r--   0     1001      123      640 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@distinct_on.prql.snap
+-rw-r--r--   0     1001      123      261 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@genre_counts.prql.snap
+-rw-r--r--   0     1001      123      632 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@group_all.prql.snap
+-rw-r--r--   0     1001      123      347 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@group_sort.prql.snap
+-rw-r--r--   0     1001      123     1721 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@invoice_totals.prql.snap
+-rw-r--r--   0     1001      123      366 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@loop.prql.snap
+-rw-r--r--   0     1001      123     1177 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@pipelines.prql.snap
+-rw-r--r--   0     1001      123      389 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@set_ops_remove.prql.snap
+-rw-r--r--   0     1001      123      571 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@sort.prql.snap
+-rw-r--r--   0     1001      123      438 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@switch.prql.snap
+-rw-r--r--   0     1001      123     1020 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@window.prql.snap
+-rw-r--r--   0     1001      123      525 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@aggregation.prql.snap
+-rw-r--r--   0     1001      123     2369 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@arithmetic.prql.snap
+-rw-r--r--   0     1001      123      440 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@cast.prql.snap
+-rw-r--r--   0     1001      123      417 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@constants_only.prql.snap
+-rw-r--r--   0     1001      123      380 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@distinct.prql.snap
+-rw-r--r--   0     1001      123      715 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@distinct_on.prql.snap
+-rw-r--r--   0     1001      123      503 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@genre_counts.prql.snap
+-rw-r--r--   0     1001      123      615 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@group_all.prql.snap
+-rw-r--r--   0     1001      123      616 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@group_sort.prql.snap
+-rw-r--r--   0     1001      123     1741 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@invoice_totals.prql.snap
+-rw-r--r--   0     1001      123      582 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@loop.prql.snap
+-rw-r--r--   0     1001      123      872 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@pipelines.prql.snap
+-rw-r--r--   0     1001      123      752 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@set_ops_remove.prql.snap
+-rw-r--r--   0     1001      123      755 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@sort.prql.snap
+-rw-r--r--   0     1001      123      622 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@switch.prql.snap
+-rw-r--r--   0     1001      123     1314 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@window.prql.snap
+-rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 prql_python-0.9.1/local_dependencies/prql_parser/Cargo.toml
+-rw-r--r--   0     1001      123    13388 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_parser/src/expr.rs
+-rw-r--r--   0     1001      123     1916 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_parser/src/interpolation.rs
+-rw-r--r--   0     1001      123    11984 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_parser/src/lexer.rs
+-rw-r--r--   0     1001      123    63208 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_parser/src/lib.rs
+-rw-r--r--   0     1001      123     5385 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_parser/src/snapshots/prql_parser__test__pipeline_parse_tree.snap
+-rw-r--r--   0     1001      123     1110 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_parser/src/span.rs
+-rw-r--r--   0     1001      123     5411 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_parser/src/stmt.rs
+-rw-r--r--   0        0        0      354 1970-01-01 00:00:00.000000 prql_python-0.9.1/local_dependencies/prql_ast/Cargo.toml
+-rw-r--r--   0     1001      123     1452 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_ast/src/expr/generic.rs
+-rw-r--r--   0     1001      123     4890 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_ast/src/expr/ident.rs
+-rw-r--r--   0     1001      123      654 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_ast/src/expr/literal.rs
+-rw-r--r--   0     1001      123     1214 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_ast/src/expr/ops.rs
+-rw-r--r--   0     1001      123     3390 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_ast/src/expr.rs
+-rw-r--r--   0     1001      123       59 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_ast/src/lib.rs
+-rw-r--r--   0     1001      123     2571 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_ast/src/span.rs
+-rw-r--r--   0     1001      123     1552 2023-07-25 18:01:49.000000 prql_python-0.9.1/local_dependencies/prql_ast/src/stmt.rs
+-rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 prql_python-0.9.1/Cargo.toml
+-rw-r--r--   0     1001      123      647 2023-07-25 18:01:49.000000 prql_python-0.9.1/.gitignore
+-rw-r--r--   0     1001      123      889 2023-07-25 18:01:49.000000 prql_python-0.9.1/README.md
+-rw-r--r--   0     1001      123      257 2023-07-25 18:01:49.000000 prql_python-0.9.1/build.rs
+-rw-r--r--   0     1001      123      974 2023-07-25 18:01:49.000000 prql_python-0.9.1/noxfile.py
+-rw-r--r--   0     1001      123      482 2023-07-25 18:01:49.000000 prql_python-0.9.1/prql_python.pyi
+-rw-r--r--   0     1001      123     1007 2023-07-25 18:01:49.000000 prql_python-0.9.1/pyproject.toml
+-rw-r--r--   0     1001      123     2019 2023-07-25 18:01:49.000000 prql_python-0.9.1/python/tests/test_all.py
+-rw-r--r--   0     1001      123       56 2023-07-25 18:01:49.000000 prql_python-0.9.1/requirements.txt
+-rw-r--r--   0     1001      123     4104 2023-07-25 18:01:49.000000 prql_python-0.9.1/src/lib.rs
+-rw-r--r--   0        0        0     1294 1970-01-01 00:00:00.000000 prql_python-0.9.1/PKG-INFO
```

### Comparing `prql_python-0.9.0/local_dependencies/prql_ast/src/expr/generic.rs` & `prql_python-0.9.1/local_dependencies/prql_ast/src/expr/generic.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql_ast/src/expr/ident.rs` & `prql_python-0.9.1/local_dependencies/prql_ast/src/expr/ident.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql_ast/src/expr/literal.rs` & `prql_python-0.9.1/local_dependencies/prql_ast/src/expr/literal.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql_ast/src/expr/ops.rs` & `prql_python-0.9.1/local_dependencies/prql_ast/src/expr/ops.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql_ast/src/expr.rs` & `prql_python-0.9.1/local_dependencies/prql_ast/src/expr.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql_ast/src/span.rs` & `prql_python-0.9.1/local_dependencies/prql_ast/src/span.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql_ast/src/stmt.rs` & `prql_python-0.9.1/local_dependencies/prql_ast/src/stmt.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/Cargo.toml` & `prql_python-0.9.1/local_dependencies/prql-compiler/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 description = "PRQL is a modern language for transforming data — a simple, powerful, pipelined SQL replacement."
 name = "prql-compiler"
 
 edition= "2021"
 license= "Apache-2.0"
 repository= "https://github.com/PRQL/prql"
 rust-version= "1.65.0"
-version= "0.9.0"
+version= "0.9.1"
 
 metadata.msrv = "1.65.0"
 
 [features]
 default = []
 # Technically tokio could be limited to external tests, but its types are in
 # signatures which would require lots of conditional compilation.
```

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/README.md` & `prql_python-0.9.1/local_dependencies/prql-compiler/README.md`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/benches/bench.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/benches/bench.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/codegen/literal.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/codegen/literal.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/error.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/error.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/generic.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/generic.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/pl/expr.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/expr.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/pl/extra/expr.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/extra/expr.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 use enum_as_inner::EnumAsInner;
-use prql_ast::expr::Literal;
+use prql_ast::expr::{Ident, Literal};
 use serde::{Deserialize, Serialize};
 
 use crate::generic::WindowKind;
 use crate::ir::pl::{Expr, ExprKind, Func, FuncCall, Range, Ty};
 
 impl FuncCall {
     pub fn new_simple(name: Expr, args: Vec<Expr>) -> Self {
@@ -132,10 +132,22 @@
             flatten: false,
         }
     }
 }
 
 impl From<Literal> for ExprKind {
     fn from(value: Literal) -> Self {
-        Self::Literal(value)
+        ExprKind::Literal(value)
+    }
+}
+
+impl From<Ident> for ExprKind {
+    fn from(value: Ident) -> Self {
+        ExprKind::Ident(value)
+    }
+}
+
+impl From<Func> for ExprKind {
+    fn from(value: Func) -> Self {
+        ExprKind::Func(Box::new(value))
     }
 }
```

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/pl/fold.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/fold.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/pl/lineage.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/lineage.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/pl/mod.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 //! The central struct here is [Expr] and its [ExprKind].
 //!
 //! Top-level construct is a list of statements [`Vec<Stmt>`].
 
 mod expr;
 mod extra;
 mod fold;
-mod from_ast;
 mod lineage;
 mod stmt;
 mod types;
 mod utils;
 
 use crate::generic::{SortDirection, WindowKind};
 use crate::ir::rq::TableRef;
```

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/pl/stmt.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/stmt.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/pl/types.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/pl/types.rs`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     Array(Box<Ty>),
 
     /// Type of sets
     /// Used for expressions that can be converted to TypeExpr.
     Set,
 
     /// Type of functions with defined params and return types.
-    Function(TyFunc),
+    Function(Option<TyFunc>),
 }
 
 #[derive(Debug, Clone, PartialEq, Serialize, Deserialize, EnumAsInner)]
 pub enum TupleField {
     /// Named tuple element.
     Single(Option<String>, Option<Ty>),
 
@@ -142,15 +142,17 @@
                 .iter()
                 .all(|(_, each)| one.is_super_type_of(&each.kind)),
 
             (TyKind::Union(many), one) => {
                 many.iter().any(|(_, any)| any.kind.is_super_type_of(one))
             }
 
-            (TyKind::Function(sup), TyKind::Function(sub)) => {
+            (TyKind::Function(None), TyKind::Function(_)) => true,
+            (TyKind::Function(Some(_)), TyKind::Function(None)) => true,
+            (TyKind::Function(Some(sup)), TyKind::Function(Some(sub))) => {
                 if is_not_super_type_of(sup.return_ty.as_ref(), sub.return_ty.as_ref()) {
                     return false;
                 }
                 if sup.args.len() != sub.args.len() {
                     return false;
                 }
                 for (sup_arg, sub_arg) in zip(&sup.args, &sub.args) {
```

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/rq/expr.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/rq/expr.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/rq/fold.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/rq/fold.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/rq/ids.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/rq/ids.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/rq/mod.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/rq/mod.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/rq/transform.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/rq/transform.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/ir/rq/utils.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/ir/rq/utils.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/lib.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -256,65 +256,67 @@
 }
 
 #[doc = include_str!("../README.md")]
 #[cfg(doctest)]
 pub struct ReadmeDoctests;
 
 /// Parse PRQL into a PL AST
-pub fn prql_to_pl(prql: &str) -> Result<Vec<ir::pl::Stmt>, ErrorMessages> {
+pub fn prql_to_pl(prql: &str) -> Result<Vec<prql_ast::stmt::Stmt>, ErrorMessages> {
     let sources = SourceTree::from(prql);
 
     parser::parse(&sources)
         .map(|x| x.sources.into_values().next().unwrap())
         .map_err(error::downcast)
         .map_err(|e| e.composed(&prql.into()))
 }
 
 /// Parse PRQL into a PL AST
-pub fn prql_to_pl_tree(prql: &SourceTree) -> Result<SourceTree<Vec<ir::pl::Stmt>>, ErrorMessages> {
+pub fn prql_to_pl_tree(
+    prql: &SourceTree,
+) -> Result<SourceTree<Vec<prql_ast::stmt::Stmt>>, ErrorMessages> {
     parser::parse(prql)
         .map_err(error::downcast)
         .map_err(|e| e.composed(prql))
 }
 
 /// Perform semantic analysis and convert PL to RQ.
-pub fn pl_to_rq(pl: Vec<ir::pl::Stmt>) -> Result<ir::rq::Query, ErrorMessages> {
+pub fn pl_to_rq(pl: Vec<prql_ast::stmt::Stmt>) -> Result<ir::rq::Query, ErrorMessages> {
     let source_tree = SourceTree::single(PathBuf::new(), pl);
     semantic::resolve_and_lower(source_tree, &[]).map_err(error::downcast)
 }
 
 /// Perform semantic analysis and convert PL to RQ.
 pub fn pl_to_rq_tree(
-    pl: SourceTree<Vec<ir::pl::Stmt>>,
+    pl: SourceTree<Vec<prql_ast::stmt::Stmt>>,
     main_path: &[String],
 ) -> Result<ir::rq::Query, ErrorMessages> {
     semantic::resolve_and_lower(pl, main_path).map_err(error::downcast)
 }
 
 /// Generate SQL from RQ.
 pub fn rq_to_sql(rq: ir::rq::Query, options: &Options) -> Result<String, ErrorMessages> {
     sql::compile(rq, options).map_err(error::downcast)
 }
 
 /// Generate PRQL code from PL AST
-pub fn pl_to_prql(pl: Vec<ir::pl::Stmt>) -> Result<String, ErrorMessages> {
-    Ok(codegen::write(&pl))
+pub fn pl_to_prql(pl: Vec<prql_ast::stmt::Stmt>) -> Result<String, ErrorMessages> {
+    Ok(codegen::write_stmts(&pl))
 }
 
 /// JSON serialization and deserialization functions
 pub mod json {
     use super::*;
 
     /// JSON serialization
-    pub fn from_pl(pl: Vec<ir::pl::Stmt>) -> Result<String, ErrorMessages> {
+    pub fn from_pl(pl: Vec<prql_ast::stmt::Stmt>) -> Result<String, ErrorMessages> {
         serde_json::to_string(&pl).map_err(|e| anyhow::anyhow!(e).into())
     }
 
     /// JSON deserialization
-    pub fn to_pl(json: &str) -> Result<Vec<ir::pl::Stmt>, ErrorMessages> {
+    pub fn to_pl(json: &str) -> Result<Vec<prql_ast::stmt::Stmt>, ErrorMessages> {
         serde_json::from_str(json).map_err(|e| anyhow::anyhow!(e).into())
     }
 
     /// JSON serialization
     pub fn from_rq(rq: ir::rq::Query) -> Result<String, ErrorMessages> {
         serde_json::to_string(&rq).map_err(|e| anyhow::anyhow!(e).into())
     }
```

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/parser.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/parser.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 use std::collections::HashMap;
 
 use anyhow::Result;
 use chumsky::{error::SimpleReason, Span as ChumskySpan};
-use prql_ast::Span;
+use prql_ast::{stmt::Stmt, Span};
 use prql_parser::chumsky;
 
-use crate::{
-    codegen,
-    error::{Error, Errors, Reason, WithErrorInfo},
-    ir::pl::Stmt,
-    utils::IdGenerator,
-    SourceTree,
-};
+use crate::error::{Error, Errors, Reason, WithErrorInfo};
+use crate::utils::IdGenerator;
+use crate::{codegen, SourceTree};
 use prql_parser::lexer::Token;
 
 pub fn parse(file_tree: &SourceTree<String>) -> Result<SourceTree<Vec<Stmt>>> {
     let mut res = SourceTree::default();
 
     let ids: HashMap<_, _> = file_tree.source_ids.iter().map(|(a, b)| (b, a)).collect();
     let mut id_gen = IdGenerator::<usize>::new();
@@ -29,28 +25,28 @@
 
         res.sources.insert(path.clone(), stmts);
         res.source_ids.insert(id, path.clone());
     }
     Ok(res)
 }
 
-fn parse_source(source: &str, source_id: u16) -> Result<Vec<Stmt>> {
+fn parse_source(source: &str, source_id: u16) -> Result<Vec<prql_ast::stmt::Stmt>> {
     let stmts = prql_parser::parse_source(source, source_id).map_err(|errors| {
         Errors(
             errors
                 .into_iter()
                 .map(|err| match err {
                     prql_parser::Error::Lexer(err) => convert_lexer_error(source, err, source_id),
                     prql_parser::Error::Parser(err) => convert_parser_error(err),
                 })
                 .collect(),
         )
     })?;
 
-    Ok(stmts.into_iter().map(Stmt::from).collect())
+    Ok(stmts)
 }
 
 fn convert_lexer_error(source: &str, e: chumsky::error::Cheap<char>, source_id: u16) -> Error {
     // TODO: is there a neater way of taking a span? We want to take it based on
     // the chars, not the bytes, so can't just index into the str.
     let found = source
         .chars()
@@ -186,15 +182,15 @@
     }
 }
 
 #[cfg(test)]
 mod tests {
     use insta::assert_debug_snapshot;
 
-    use crate::ir::pl::Stmt;
+    use prql_ast::stmt::Stmt;
 
     /// Helper that does not track source_ids
     #[cfg(test)]
     pub fn parse_single(source: &str) -> anyhow::Result<Vec<Stmt>> {
         super::parse_source(source, 0)
     }
```

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/context.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/context.rs`

 * *Files 2% similar despite different names*

```diff
@@ -194,15 +194,15 @@
                     "TableDecl: {} {expr:?}",
                     ty.as_ref().map(|t| t.to_string()).unwrap_or_default()
                 )
             }
             Self::InstanceOf(arg0) => write!(f, "InstanceOf: {arg0}"),
             Self::Column(arg0) => write!(f, "Column (target {arg0})"),
             Self::Infer(arg0) => write!(f, "Infer (default: {arg0})"),
-            Self::Expr(arg0) => write!(f, "Expr: {arg0}"),
+            Self::Expr(arg0) => write!(f, "Expr: {}", write_pl(*arg0.clone())),
             Self::QueryDef(_) => write!(f, "QueryDef"),
         }
     }
 }
 
 fn is_zero(x: &usize) -> bool {
     *x == 0
```

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/eval/mod.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/eval/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 
 use anyhow::Result;
 use itertools::Itertools;
 
 use crate::error::{Error, Span, WithErrorInfo};
 use crate::ir::pl::{Expr, ExprKind, Func, FuncCall, FuncParam, Ident, Literal, PlFold};
 
+use super::ast_expand;
 use super::resolver::{binary_to_func_call, unary_to_func_call};
 
-pub fn eval(expr: Expr) -> Result<Expr> {
+pub fn eval(expr: prql_ast::expr::Expr) -> Result<Expr> {
+    let expr = ast_expand::expand_expr(expr);
+
     Evaluator::new().fold_expr(expr)
 }
 
 /// Converts an expression to a value
 ///
 /// Serves as a working draft of PRQL semantics definition.
 struct Evaluator {
@@ -470,23 +473,25 @@
 
 #[cfg(test)]
 mod test {
 
     use insta::assert_display_snapshot;
     use itertools::Itertools;
 
+    use crate::semantic::write_pl;
+
     use super::*;
 
     fn eval(source: &str) -> Result<String> {
         let stmts = crate::prql_to_pl(source)?.into_iter().exactly_one()?;
-        let expr = stmts.kind.into_var_def()?.value;
+        let expr = stmts.kind.into_main().unwrap();
 
         let value = super::eval(*expr)?;
 
-        Ok(value.to_string())
+        Ok(write_pl(value))
     }
 
     #[test]
     fn basic() {
         assert_display_snapshot!(eval(r"
             [std.floor (3.5 + 2.9) + 3, 3]
         ").unwrap(),
```

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/lowering.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/lowering.rs`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 use crate::ir::generic::{InterpolateItem, Range, SwitchCase};
 use crate::ir::pl::{
     self, BinaryExpr, Ident, Lineage, LineageColumn, PlFold, QueryDef, TupleField, UnaryExpr,
 };
 use crate::ir::rq::{self, CId, Query, RelationColumn, RelationLiteral, TId, TableDecl, Transform};
 use crate::semantic::context::TableExpr;
 use crate::semantic::module::Module;
+use crate::semantic::write_pl;
 use crate::utils::{toposort, IdGenerator};
 use crate::COMPILER_VERSION;
 
 use super::context::{self, Context, DeclKind};
 use super::NS_DEFAULT_DB;
 
 /// Convert AST into IR and make sure that:
@@ -357,15 +358,15 @@
                 self.create_a_table_instance(id, None, tid)
             }
 
             _ => {
                 return Err(Error::new(Reason::Expected {
                     who: None,
                     expected: "a pipeline that resolves to a table".to_string(),
-                    found: format!("`{expr}`"),
+                    found: format!("`{}`", write_pl(expr.clone())),
                 })
                 .push_hint("are you missing `from` statement?")
                 .with_span(expr.span)
                 .into())
             }
         })
     }
@@ -719,41 +720,41 @@
         };
         self.node_mapping.insert(id, LoweredTarget::Compute(cid));
 
         self.pipeline.push(Transform::Compute(compute));
         Ok(cid)
     }
 
-    fn lower_expr(&mut self, ast: pl::Expr) -> Result<rq::Expr> {
-        if ast.needs_window {
-            let span = ast.span;
-            let cid = self.declare_as_column(ast, false)?;
+    fn lower_expr(&mut self, expr: pl::Expr) -> Result<rq::Expr> {
+        if expr.needs_window {
+            let span = expr.span;
+            let cid = self.declare_as_column(expr, false)?;
 
             let kind = rq::ExprKind::ColumnRef(cid);
             return Ok(rq::Expr { kind, span });
         }
 
-        let kind = match ast.kind {
+        let kind = match expr.kind {
             pl::ExprKind::Ident(ident) => {
-                log::debug!("lowering ident {ident} (target {:?})", ast.target_id);
+                log::debug!("lowering ident {ident} (target {:?})", expr.target_id);
 
-                if let Some(id) = ast.target_id {
+                if let Some(id) = expr.target_id {
                     let cid = self.lookup_cid(id, Some(&ident.name))?;
 
                     rq::ExprKind::ColumnRef(cid)
                 } else {
                     // This is an unresolved ident.
                     // Let's hope that the database engine can resolve it.
                     rq::ExprKind::SString(vec![InterpolateItem::String(ident.name)])
                 }
             }
             pl::ExprKind::All { except, .. } => {
                 let mut targets = Vec::new();
 
-                for target_id in &ast.target_ids {
+                for target_id in &expr.target_ids {
                     match self.node_mapping.get(target_id) {
                         Some(LoweredTarget::Compute(cid)) => targets.push(*cid),
                         Some(LoweredTarget::Input(input_columns)) => {
                             targets.extend(input_columns.values().map(|(c, _)| c))
                         }
                         _ => {}
                     }
@@ -772,15 +773,15 @@
                 targets.retain(|t| !except.contains(t));
 
                 if targets.len() == 1 {
                     rq::ExprKind::ColumnRef(targets[0])
                 } else {
                     return Err(
                         Error::new_simple("This wildcard usage is not yet supported.")
-                            .with_span(ast.span)
+                            .with_span(expr.span)
                             .into(),
                     );
                 }
             }
             pl::ExprKind::Literal(literal) => rq::ExprKind::Literal(literal),
 
             pl::ExprKind::SString(items) => {
@@ -821,33 +822,33 @@
             | pl::ExprKind::Range(_)
             | pl::ExprKind::Tuple(_)
             | pl::ExprKind::Array(_)
             | pl::ExprKind::Func(_)
             | pl::ExprKind::Pipeline(_)
             | pl::ExprKind::Type(_)
             | pl::ExprKind::TransformCall(_) => {
-                log::debug!("cannot lower {ast:?}");
+                log::debug!("cannot lower {expr:?}");
                 return Err(Error::new(Reason::Unexpected {
-                    found: format!("`{ast}`"),
+                    found: format!("`{}`", write_pl(expr.clone())),
                 })
                 .push_hint("this is probably a 'bad type' error (we are working on that)")
-                .with_span(ast.span)
+                .with_span(expr.span)
                 .into());
             }
 
             pl::ExprKind::Unary(UnaryExpr { .. })
             | pl::ExprKind::Binary(BinaryExpr { .. })
             | pl::ExprKind::Internal(_) => {
-                panic!("Unresolved lowering: {ast}")
+                panic!("Unresolved lowering: {}", write_pl(expr))
             }
         };
 
         Ok(rq::Expr {
             kind,
-            span: ast.span,
+            span: expr.span,
         })
     }
 
     fn lower_interpolations(
         &mut self,
         items: Vec<InterpolateItem<pl::Expr>>,
     ) -> Result<Vec<InterpolateItem<rq::Expr>>> {
```

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/mod.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/mod.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 //! Semantic resolver (name resolution, type checking and lowering to RQ)
 
+mod ast_expand;
 mod context;
 mod eval;
 mod lowering;
 mod module;
 pub mod reporting;
 mod resolver;
 mod static_analysis;
@@ -21,23 +22,29 @@
 
 use crate::error::WithErrorInfo;
 use crate::ir::pl::{self, Lineage, LineageColumn, ModuleDef, Stmt, StmtKind, TypeDef, VarDef};
 use crate::ir::rq::Query;
 use crate::{Error, Reason, SourceTree};
 
 /// Runs semantic analysis on the query and lowers PL to RQ.
-pub fn resolve_and_lower(file_tree: SourceTree<Vec<Stmt>>, main_path: &[String]) -> Result<Query> {
+pub fn resolve_and_lower(
+    file_tree: SourceTree<Vec<prql_ast::stmt::Stmt>>,
+    main_path: &[String],
+) -> Result<Query> {
     let context = resolve(file_tree, Default::default())?;
 
     let (query, _) = lowering::lower_to_ir(context, main_path)?;
     Ok(query)
 }
 
 /// Runs semantic analysis on the query.
-pub fn resolve(mut file_tree: SourceTree<Vec<Stmt>>, options: ResolverOptions) -> Result<Context> {
+pub fn resolve(
+    mut file_tree: SourceTree<Vec<prql_ast::stmt::Stmt>>,
+    options: ResolverOptions,
+) -> Result<Context> {
     // inject std module if it does not exist
     if !file_tree.sources.contains_key(&PathBuf::from("std.prql")) {
         let mut source_tree = SourceTree {
             sources: Default::default(),
             source_ids: file_tree.source_ids.clone(),
         };
         load_std_lib(&mut source_tree);
@@ -52,14 +59,16 @@
         ..Context::default()
     };
     let mut resolver = Resolver::new(context, options);
 
     // resolve sources one by one
     // TODO: recursive references
     for (path, stmts) in normalize(file_tree)? {
+        let stmts = ast_expand::expand_stmts(stmts);
+
         resolver.current_module_path = path;
         resolver.fold_statements(stmts)?;
     }
 
     Ok(resolver.context)
 }
 
@@ -82,15 +91,17 @@
                 .to_str()
                 .ok_or_else(|| anyhow::anyhow!("Invalid file path: {path:?}"))
                 .map(str::to_string)
         })
         .try_collect()
 }
 
-fn normalize(mut tree: SourceTree<Vec<Stmt>>) -> Result<Vec<(Vec<String>, Vec<Stmt>)>> {
+fn normalize(
+    mut tree: SourceTree<Vec<prql_ast::stmt::Stmt>>,
+) -> Result<Vec<(Vec<String>, Vec<prql_ast::stmt::Stmt>)>> {
     // find root
     let root_path = PathBuf::from("");
 
     if tree.sources.get(&root_path).is_none() {
         if tree.sources.len() == 1 {
             // if there is only one file, use that as the root
             let (_, only) = tree.sources.drain().exactly_one().unwrap();
@@ -175,21 +186,29 @@
     where
         F: FnOnce(pl::ExprKind) -> Result<T, pl::ExprKind>,
     {
         f(self.kind).map_err(|i| {
             Error::new(Reason::Expected {
                 who: who.map(|s| s.to_string()),
                 expected: expected.to_string(),
-                found: format!("`{}`", pl::Expr::new(i)),
+                found: format!("`{}`", write_pl(pl::Expr::new(i))),
             })
             .with_span(self.span)
         })
     }
 }
 
+/// Write a PL IR to string.
+///
+/// Because PL needs to be restricted back to AST, ownerships of expr is required.
+pub fn write_pl(expr: pl::Expr) -> String {
+    let expr = ast_expand::restrict_expr(expr);
+
+    crate::codegen::write_expr(&expr)
+}
 #[cfg(test)]
 pub mod test {
     use anyhow::Result;
     use insta::assert_yaml_snapshot;
 
     use crate::ir::rq::Query;
     use crate::parser::parse;
```

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/module.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/module.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/reporting.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/reporting.rs`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                         .and_then(|id| self.get_span_lines(id))
                         .unwrap_or_default();
 
                     let decl = match &decl.kind {
                         DeclKind::TableDecl(TableDecl { ty, .. }) => {
                             format!(
                                 "table {}",
-                                ty.as_ref().map(|t| t.to_string()).unwrap_or_default()
+                                ty.as_ref().and_then(|t| t.name.clone()).unwrap_or_default()
                             )
                         }
                         _ => decl.to_string(),
                     };
 
                     (format!("{decl}{location}"), color)
                 } else if let Some(decl_id) = node.target_id {
```

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/context_impl.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/context_impl.rs`

 * *Files 1% similar despite different names*

```diff
@@ -66,17 +66,18 @@
             // to select a `download_2020_01_01` column later in the query. But
             // sometimes we want to query for `*.parquet` files, and give them an
             // alias. So we don't raise an error here, but if there's a way of
             // differentiating the cases, we can implement that.
             // if ident.name != "*" {
             //     return Err("Unsupported feature: advanced wildcard column matching".to_string());
             // }
-            return self
-                .resolve_ident_wildcard(ident)
-                .map_err(Error::new_simple);
+            return self.resolve_ident_wildcard(ident).map_err(|e| {
+                log::debug!("{:#?}", self.root_mod);
+                Error::new_simple(e)
+            });
         }
 
         // base case: direct lookup
         let decls = self.root_mod.lookup(ident);
         match decls.len() {
             // no match: try match *
             0 => {}
```

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/flatten.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/flatten.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/mod.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 use crate::semantic::context::TableDecl;
 use crate::semantic::{static_analysis, NS_PARAM};
 use crate::utils::IdGenerator;
 
 use super::context::{Context, Decl, DeclKind, TableExpr};
 use super::module::Module;
 use super::reporting::debug_call_tree;
-use super::{NS_DEFAULT_DB, NS_INFER, NS_STD, NS_THAT, NS_THIS};
+use super::{write_pl, NS_DEFAULT_DB, NS_INFER, NS_STD, NS_THAT, NS_THIS};
 use flatten::Flattener;
 use transforms::coerce_into_tuple_and_flatten;
 use type_resolver::infer_type;
 
 mod context_impl;
 mod flatten;
 mod transforms;
@@ -363,23 +363,23 @@
                 let name = self.fold_expr(*name)?;
                 self.in_func_call_name = old;
 
                 let func = *name.try_cast(|n| n.into_func(), None, "a function")?;
 
                 // fold function
                 let func = self.apply_args_to_closure(func, args, named_args)?;
-                self.fold_function(func, node.span)?
+                self.fold_function(func, span)?
             }
 
             ExprKind::Pipeline(pipeline) => {
                 self.default_namespace = None;
                 self.resolve_pipeline(pipeline)?
             }
 
-            ExprKind::Func(closure) => self.fold_function(*closure, node.span)?,
+            ExprKind::Func(closure) => self.fold_function(*closure, span)?,
 
             ExprKind::Unary(UnaryExpr {
                 op: UnOp::EqSelf,
                 expr,
             }) => {
                 let kind = self.resolve_eq_self(*expr, span)?;
                 Expr { kind, ..node }
@@ -625,17 +625,16 @@
 
         // log::debug!(
         //     "cannot resolve `{ident}`: `{e}`, context={:#?}",
         //     self.context
         // );
     }
 
-    fn fold_function(&mut self, closure: Func, span: Option<Span>) -> Result<Expr, anyhow::Error> {
+    fn fold_function(&mut self, closure: Func, span: Option<Span>) -> Result<Expr> {
         let closure = self.fold_function_types(closure)?;
-        let args_len = closure.args.len();
 
         log::debug!(
             "func {} {}/{} params",
             closure.as_debug_name(),
             closure.args.len(),
             closure.params.len()
         );
@@ -646,134 +645,109 @@
                 closure.as_debug_name()
             ))
             .with_span(span)
             .into());
         }
 
         let enough_args = closure.args.len() == closure.params.len();
+        if !enough_args {
+            // not enough arguments: don't fold
+            log::debug!("returning as closure");
+            return Ok(expr_of_func(closure));
+        }
 
-        let mut r = if enough_args {
-            // make sure named args are pushed into params
-            let closure = if !closure.named_params.is_empty() {
-                self.apply_args_to_closure(closure, [].into(), [].into())?
-            } else {
-                closure
-            };
-
-            // push the env
-            let closure_env = Module::from_exprs(closure.env);
-            self.context.root_mod.stack_push(NS_PARAM, closure_env);
-            let closure = Func {
-                env: HashMap::new(),
-                ..closure
-            };
-
-            if log::log_enabled!(log::Level::Debug) {
-                let name = closure
-                    .name_hint
-                    .clone()
-                    .unwrap_or_else(|| Ident::from_name("<unnamed>"));
-                log::debug!("resolving args of function {}", name);
-            }
-            let closure = self.resolve_function_args(closure)?;
-
-            let needs_window = (closure.params.last())
-                .and_then(|p| p.ty.as_ref())
-                .map(|t| t.as_ty().unwrap().is_sub_type_of_array())
-                .unwrap_or_default();
-
-            // evaluate
-            let res = if let ExprKind::Internal(operator_name) = &closure.body.kind {
-                // special case: functions that have internal body
-
-                if operator_name.starts_with("std.") {
-                    Expr {
-                        ty: closure.return_ty.map(|t| t.into_ty().unwrap()),
-                        needs_window,
-                        ..Expr::new(ExprKind::RqOperator {
-                            name: operator_name.clone(),
-                            args: closure.args,
-                        })
-                    }
-                } else {
-                    let expr = transforms::cast_transform(self, closure)?;
-                    self.fold_expr(expr)?
-                }
-            } else {
-                // base case: materialize
-                log::debug!("stack_push for {}", closure.as_debug_name());
+        // make sure named args are pushed into params
+        let closure = if !closure.named_params.is_empty() {
+            self.apply_args_to_closure(closure, [].into(), [].into())?
+        } else {
+            closure
+        };
 
-                let (func_env, body) = env_of_closure(closure);
+        // push the env
+        let closure_env = Module::from_exprs(closure.env);
+        self.context.root_mod.stack_push(NS_PARAM, closure_env);
+        let closure = Func {
+            env: HashMap::new(),
+            ..closure
+        };
 
-                self.context.root_mod.stack_push(NS_PARAM, func_env);
+        if log::log_enabled!(log::Level::Debug) {
+            let name = closure
+                .name_hint
+                .clone()
+                .unwrap_or_else(|| Ident::from_name("<unnamed>"));
+            log::debug!("resolving args of function {}", name);
+        }
+        let closure = self.resolve_function_args(closure)?;
+
+        let needs_window = (closure.params.last())
+            .and_then(|p| p.ty.as_ref())
+            .map(|t| t.as_ty().unwrap().is_sub_type_of_array())
+            .unwrap_or_default();
+
+        // evaluate
+        let res = if let ExprKind::Internal(operator_name) = &closure.body.kind {
+            // special case: functions that have internal body
 
-                // fold again, to resolve inner variables & functions
-                let body = self.fold_expr(body)?;
-
-                // remove param decls
-                log::debug!("stack_pop: {:?}", body.id);
-                let func_env = self.context.root_mod.stack_pop(NS_PARAM).unwrap();
-
-                if let ExprKind::Func(mut inner_closure) = body.kind {
-                    // body couldn't been resolved - construct a closure to be evaluated later
-
-                    inner_closure.env = func_env.into_exprs();
-
-                    let (got, missing) = inner_closure.params.split_at(inner_closure.args.len());
-                    let missing = missing.to_vec();
-                    inner_closure.params = got.to_vec();
-
-                    Expr::new(ExprKind::Func(Box::new(Func {
-                        name_hint: None,
-                        args: vec![],
-                        params: missing,
-                        named_params: vec![],
-                        body: Box::new(Expr::new(ExprKind::Func(inner_closure))),
-                        return_ty: None,
-                        env: HashMap::new(),
-                    })))
-                } else {
-                    // resolved, return result
-                    body
+            if operator_name.starts_with("std.") {
+                Expr {
+                    ty: closure.return_ty.map(|t| t.into_ty().unwrap()),
+                    needs_window,
+                    ..Expr::new(ExprKind::RqOperator {
+                        name: operator_name.clone(),
+                        args: closure.args,
+                    })
                 }
-            };
-
-            // pop the env
-            self.context.root_mod.stack_pop(NS_PARAM).unwrap();
-
-            res
+            } else {
+                let expr = transforms::cast_transform(self, closure)?;
+                self.fold_expr(expr)?
+            }
         } else {
-            // not enough arguments: don't fold
-            log::debug!("returning as closure");
+            // base case: materialize
+            log::debug!("stack_push for {}", closure.as_debug_name());
 
-            let ty = TyFunc {
-                args: closure
-                    .params
-                    .iter()
-                    .skip(args_len)
-                    .map(|a| a.ty.as_ref().map(|x| x.as_ty().cloned().unwrap()))
-                    .collect(),
-                return_ty: Box::new(
-                    closure
-                        .return_ty
-                        .as_ref()
-                        .map(|x| x.as_ty().cloned().unwrap()),
-                ),
-            };
+            let (func_env, body) = env_of_closure(closure);
 
-            let mut node = Expr::new(ExprKind::Func(Box::new(closure)));
-            node.ty = Some(Ty {
-                kind: TyKind::Function(ty),
-                name: None,
-            });
+            self.context.root_mod.stack_push(NS_PARAM, func_env);
 
-            node
+            // fold again, to resolve inner variables & functions
+            let body = self.fold_expr(body)?;
+
+            // remove param decls
+            log::debug!("stack_pop: {:?}", body.id);
+            let func_env = self.context.root_mod.stack_pop(NS_PARAM).unwrap();
+
+            if let ExprKind::Func(mut inner_closure) = body.kind {
+                // body couldn't been resolved - construct a closure to be evaluated later
+
+                inner_closure.env = func_env.into_exprs();
+
+                let (got, missing) = inner_closure.params.split_at(inner_closure.args.len());
+                let missing = missing.to_vec();
+                inner_closure.params = got.to_vec();
+
+                Expr::new(ExprKind::Func(Box::new(Func {
+                    name_hint: None,
+                    args: vec![],
+                    params: missing,
+                    named_params: vec![],
+                    body: Box::new(Expr::new(ExprKind::Func(inner_closure))),
+                    return_ty: None,
+                    env: HashMap::new(),
+                })))
+            } else {
+                // resolved, return result
+                body
+            }
         };
-        r.span = span;
-        Ok(r)
+
+        // pop the env
+        self.context.root_mod.stack_pop(NS_PARAM).unwrap();
+
+        Ok(res)
     }
 
     fn fold_function_types(&mut self, mut closure: Func) -> Result<Func> {
         closure.params = closure
             .params
             .into_iter()
             .map(|p| -> Result<_> {
@@ -964,25 +938,25 @@
             name: "std.eq".to_string(),
             args: vec![left, right],
         };
         let kind = fold_expr_kind(self, kind)?;
         Ok(kind)
     }
 
-    fn resolve_column_exclusion(&mut self, expr: Expr) -> Result<Expr, anyhow::Error> {
+    fn resolve_column_exclusion(&mut self, expr: Expr) -> Result<Expr> {
         let expr = self.fold_expr(expr)?;
         let tuple = coerce_into_tuple_and_flatten(expr)?;
         let except: Vec<Expr> = tuple
             .into_iter()
             .map(|e| match e.kind {
                 ExprKind::Ident(_) | ExprKind::All { .. } => Ok(e),
                 _ => Err(Error::new(Reason::Expected {
                     who: Some("exclusion".to_string()),
                     expected: "column name".to_string(),
-                    found: format!("`{e}`"),
+                    found: format!("`{}`", write_pl(e)),
                 })),
             })
             .try_collect()?;
 
         self.fold_expr(Expr::new(ExprKind::All {
             within: Ident::from_name(NS_THIS),
             except,
@@ -1013,14 +987,34 @@
                 Some(TyOrExpr::Ty(self.fold_type_expr(Some(ty_expr))?.unwrap()))
             }
             _ => ty_or_expr,
         })
     }
 }
 
+fn expr_of_func(func: Func) -> Expr {
+    let ty = TyFunc {
+        args: func
+            .params
+            .iter()
+            .skip(func.args.len())
+            .map(|a| a.ty.as_ref().map(|x| x.as_ty().cloned().unwrap()))
+            .collect(),
+        return_ty: Box::new(func.return_ty.as_ref().map(|x| x.as_ty().cloned().unwrap())),
+    };
+
+    Expr {
+        ty: Some(Ty {
+            kind: TyKind::Function(Some(ty)),
+            name: None,
+        }),
+        ..Expr::new(ExprKind::Func(Box::new(func)))
+    }
+}
+
 fn ty_of_lineage(lineage: &Lineage) -> Ty {
     Ty::relation(
         lineage
             .columns
             .iter()
             .map(|col| match col {
                 LineageColumn::All { .. } => TupleField::Wildcard(None),
@@ -1057,14 +1051,20 @@
         "int" => PrimitiveSet::Int,
         "float" => PrimitiveSet::Float,
         "bool" => PrimitiveSet::Bool,
         "text" => PrimitiveSet::Text,
         "date" => PrimitiveSet::Date,
         "time" => PrimitiveSet::Time,
         "timestamp" => PrimitiveSet::Timestamp,
+        "func" => {
+            return Some(ExprKind::Type(Ty {
+                kind: TyKind::Function(None),
+                name: None,
+            }))
+        }
         _ => return None,
     };
     Some(ExprKind::Type(Ty {
         kind: TyKind::Primitive(set),
         name: None,
     }))
 }
@@ -1100,18 +1100,15 @@
 
     fn resolve_lineage(query: &str) -> Result<Lineage> {
         Ok(parse_and_resolve(query)?.lineage.unwrap())
     }
 
     fn resolve_derive(query: &str) -> Result<Vec<Expr>> {
         let expr = parse_and_resolve(query)?;
-        let derive = expr
-            .kind
-            .into_transform_call()
-            .unwrap_or_else(|e| panic!("Failed to convert `{}`", Expr::new(e)));
+        let derive = expr.kind.into_transform_call().unwrap();
         let exprs = derive
             .kind
             .into_derive()
             .unwrap_or_else(|e| panic!("Failed to convert `{e:?}`"));
 
         let exprs = IdEraser {}.fold_exprs(exprs).unwrap();
         Ok(exprs)
```

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names-3.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__frames_and_names-3.snap`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 ---
-source: prql-compiler/src/semantic/resolver.rs
+source: crates/prql_compiler/src/semantic/resolver/mod.rs
 expression: "resolve_lineage(r#\"\n            from e = employees\n            join salaries (==emp_no)\n            group {e.emp_no, e.gender} (\n                aggregate {\n                    emp_salary = average salaries.salary\n                }\n            )\n            \"#).unwrap()"
 ---
 columns:
   - Single:
       name:
         - e
         - emp_no
-      target_id: 219
+      target_id: 221
       target_name: ~
   - Single:
       name:
         - e
         - gender
-      target_id: 220
+      target_id: 222
       target_name: ~
   - Single:
       name:
         - emp_salary
-      target_id: 245
+      target_id: 247
       target_name: ~
 inputs:
-  - id: 180
+  - id: 182
     name: e
     table:
       - default_db
       - employees
-  - id: 214
+  - id: 216
     name: salaries
     table:
       - default_db
       - salaries
```

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_1.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_1.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_nested.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_nested.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_pipeline-2.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_pipeline-2.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_pipeline.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__functions_pipeline.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__named_args.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__named_args.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__variables_1.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__test__variables_1.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__transforms__tests__aggregate_positional_arg-2.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/snapshots/prql_compiler__semantic__resolver__transforms__tests__aggregate_positional_arg-2.snap`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ---
-source: prql-compiler/src/semantic/transforms.rs
+source: crates/prql_compiler/src/semantic/resolver/transforms.rs
 expression: expr
 ---
 TransformCall:
   input:
     Ident:
       - default_db
       - c_invoice
@@ -17,15 +17,15 @@
       name: ~
     lineage:
       columns:
         - All:
             input_name: c_invoice
             except: []
       inputs:
-        - id: 180
+        - id: 182
           name: c_invoice
           table:
             - default_db
             - c_invoice
   kind:
     Aggregate:
       assigns:
@@ -181,20 +181,20 @@
   name: relation
 lineage:
   columns:
     - Single:
         name:
           - c_invoice
           - issued_at
-        target_id: 203
+        target_id: 205
         target_name: ~
     - Single:
         name: ~
-        target_id: 227
+        target_id: 229
         target_name: ~
   inputs:
-    - id: 180
+    - id: 182
       name: c_invoice
       table:
         - default_db
         - c_invoice
```

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/transforms.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/transforms.rs`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 use std::iter::zip;
 
 use crate::error::{Error, Reason, WithErrorInfo};
 use crate::generic::{SortDirection, WindowKind};
 use crate::ir::pl::BinaryExpr;
 use crate::ir::pl::PlFold;
 use crate::ir::pl::*;
+use crate::semantic::write_pl;
 
 use super::super::context::{Decl, DeclKind};
 use super::super::module::Module;
 use super::Resolver;
 use super::{Context, Lineage};
 use super::{NS_PARAM, NS_THIS};
 
@@ -77,15 +78,15 @@
             let range = match expr.kind {
                 ExprKind::Literal(Literal::Integer(n)) => range_from_ints(None, Some(n)),
                 ExprKind::Range(range) => range,
                 _ => {
                     return Err(Error::new(Reason::Expected {
                         who: Some("`take`".to_string()),
                         expected: "int or range".to_string(),
-                        found: expr.to_string(),
+                        found: write_pl(expr.clone()),
                     })
                     // Possibly this should refer to the item after the `take` where
                     // one exists?
                     .with_span(expr.span)
                     .into());
                 }
             };
@@ -134,28 +135,28 @@
             let expanding = {
                 let as_bool = expanding.kind.as_literal().and_then(|l| l.as_boolean());
 
                 *as_bool.ok_or_else(|| {
                     Error::new(Reason::Expected {
                         who: Some("parameter `expanding`".to_string()),
                         expected: "a boolean".to_string(),
-                        found: format!("{expanding}"),
+                        found: write_pl(expanding.clone()),
                     })
                     .with_span(expanding.span)
                 })?
             };
 
             let rolling = {
                 let as_int = rolling.kind.as_literal().and_then(|x| x.as_integer());
 
                 *as_int.ok_or_else(|| {
                     Error::new(Reason::Expected {
                         who: Some("parameter `rolling`".to_string()),
                         expected: "a number".to_string(),
-                        found: format!("{rolling}"),
+                        found: write_pl(rolling.clone()),
                     })
                     .with_span(rolling.span)
                 })?
             };
 
             let rows = rows.try_cast(|r| r.into_range(), Some("parameter `rows`"), "a range")?;
 
@@ -233,15 +234,15 @@
                     //   even expressions that evaluate to a tuple.
                 }
                 _ => {}
             }
             return Err(Error::new(Reason::Expected {
                 who: Some("std.in".to_string()),
                 expected: "a pattern".to_string(),
-                found: pattern.to_string(),
+                found: write_pl(pattern.clone()),
             })
             .with_span(pattern.span)
             .into());
         }
 
         "tuple_every" => {
             // yes, this is not a transform, but this is the most appropriate place for it
@@ -313,15 +314,15 @@
 
             let text = match text_expr.kind {
                 ExprKind::Literal(Literal::String(text)) => text,
                 _ => {
                     return Err(Error::new(Reason::Expected {
                         who: Some("std.from_text".to_string()),
                         expected: "a string literal".to_string(),
-                        found: format!("`{text_expr}`"),
+                        found: format!("`{}`", write_pl(text_expr.clone())),
                     })
                     .with_span(text_expr.span)
                     .into());
                 }
             };
 
             let res = {
@@ -535,15 +536,18 @@
             }
             Group { pipeline, by, .. } => {
                 // pipeline's body is resolved, just use its type
                 let Func { body, .. } = pipeline.kind.as_func().unwrap().as_ref();
 
                 let mut frame = body.lineage.clone().unwrap();
 
-                log::debug!("inferring type of group with pipeline: {body}");
+                log::debug!(
+                    "inferring type of group with pipeline: {}",
+                    write_pl(*body.clone())
+                );
 
                 // prepend aggregate with `by` columns
                 if let ExprKind::TransformCall(TransformCall { kind, .. }) = &body.as_ref().kind {
                     if let TransformKind::Aggregate { .. } = kind.as_ref() {
                         let aggregate_columns = frame.columns;
                         frame.columns = Vec::new();
```

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/resolver/type_resolver.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/resolver/type_resolver.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 use anyhow::Result;
 use itertools::Itertools;
 
 use crate::error::{Error, Reason, WithErrorInfo};
 use crate::ir::pl::*;
+use crate::semantic::write_pl;
 
 use super::Resolver;
 
 /// Takes a resolved [Expr] and evaluates it a type expression that can be used to construct a type.
 pub fn coerce_to_type(resolver: &mut Resolver, expr: Expr) -> Result<Ty> {
     coerce_kind_to_set(resolver, expr.kind)
 }
@@ -102,28 +103,30 @@
                 kind: TyKind::Union(options),
             }
         }
 
         // functions
         ExprKind::Func(func) => Ty {
             name: None,
-            kind: TyKind::Function(TyFunc {
+            kind: TyKind::Function(Some(TyFunc {
                 args: func
                     .params
                     .into_iter()
                     .map(|p| p.ty.map(|t| t.into_ty().unwrap()))
                     .collect_vec(),
                 return_ty: Box::new(resolver.fold_type_expr(Some(func.body))?),
-            }),
+            })),
         },
 
         _ => {
-            return Err(
-                Error::new_simple(format!("not a type expression: {}", Expr::new(expr))).into(),
-            )
+            return Err(Error::new_simple(format!(
+                "not a type expression: {}",
+                write_pl(Expr::new(expr))
+            ))
+            .into())
         }
     })
 }
 
 pub fn infer_type(node: &Expr) -> Result<Option<Ty>> {
     if let Some(ty) = &node.ty {
         return Ok(Some(ty.clone()));
@@ -322,22 +325,24 @@
         Ok(found.next().is_none())
     }
 }
 
 #[allow(dead_code)]
 fn too_many_arguments(call: &FuncCall, expected_len: usize, passed_len: usize) -> Error {
     let err = Error::new(Reason::Expected {
-        who: Some(format!("{}", call.name)),
+        who: Some(write_pl(*call.name.clone())),
         expected: format!("{} arguments", expected_len),
         found: format!("{}", passed_len),
     });
     if passed_len >= 2 {
         err.push_hint(format!(
             "if you are calling a function, you may want to add parentheses `{} [{:?} {:?}]`",
-            call.name, call.args[0], call.args[1]
+            write_pl(*call.name.clone()),
+            call.args[0],
+            call.args[1]
         ))
     } else {
         err
     }
 }
 
 fn find_potential_tuple_fields(expected: &Ty) -> Option<&Vec<TupleField>> {
```

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/static_analysis.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/static_analysis.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/semantic/std.prql` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/semantic/std.prql`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 type int
 type float
 type bool
 type text
 type date
 type time
 type timestamp
+type `func`
 
 ## Generic array
 # TODO: an array of anything, not just nulls
 type array = [null]
 
 ## Scalar
 type scalar = int || float || bool || text || date || time || timestamp || null
@@ -129,15 +130,18 @@
 )
 let remove = `default_db.bottom`<relation> top<relation> -> <relation> (
   noop t = top
   join side:left (noop b = bottom) (tuple_every (tuple_map _eq (tuple_zip t.* b.*)))
   filter (tuple_every (tuple_map _is_null b.*))
   select t.*
 )
-let loop = pipeline top<relation> -> <relation> internal loop
+let loop = func
+  pipeline <transform>
+  top <relation>
+  -> <relation> internal loop
 
 ## Aggregate functions
 # These return either a scalar when used within `aggregate`, or a column when used anywhere else.
 
 let min = column <array> -> <int || float || null> internal std.min
 
 let max = column <array> -> <int || float || null> internal std.max
@@ -173,19 +177,19 @@
 
 ## Misc functions
 let round = n_digits column -> <scalar> internal std.round
 let as = `noresolve.type` column -> <scalar> internal std.as
 let in = pattern value -> <bool> internal in
 
 ## Tuple functions
-let tuple_every = list -> <bool> internal tuple_every
-let tuple_map = fn list -> internal tuple_map
-let tuple_zip = a b -> internal tuple_zip
-let _eq = a -> internal _eq
-let _is_null = a -> _param.a == null
+let tuple_every = func list -> <bool> internal tuple_every
+let tuple_map = func fn <func> list -> internal tuple_map
+let tuple_zip = func a b -> internal tuple_zip
+let _eq = func a -> internal _eq
+let _is_null = func a -> _param.a == null
 
 ## Misc
 let from_text = input<text> `noresolve.format`:csv -> <relation> internal from_text
 
 ## String functions
 let lower = column -> <text> internal std.lower
 let upper = column -> <text> internal std.upper
```

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/dialect.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/dialect.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/gen_expr.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/gen_expr.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/gen_projection.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/gen_projection.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/gen_query.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/gen_query.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/keywords.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/keywords.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/mod.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/mod.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/operators.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/operators.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/srq/anchor.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/anchor.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/srq/ast.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/ast.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/srq/context.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/context.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/srq/gen_query.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/gen_query.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/srq/mod.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/mod.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/srq/postprocess.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/postprocess.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/srq/preprocess.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/srq/preprocess.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/sql/std.sql.prql` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/sql/std.sql.prql`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/tests/test.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/tests/test.rs`

 * *Files 0% similar despite different names*

```diff
@@ -175,38 +175,36 @@
       *
     FROM
       managers
     "###);
 
     assert_display_snapshot!(compile(r###"
     from employees
-    derive {name, cost = salary}
+    select {name, cost = salary}
     take 3
     append (
         from employees
-        derive {name, cost = salary + bonuses}
+        select {name, cost = salary + bonuses}
         take 10
     )
     "###).unwrap(), @r###"
     WITH table_0 AS (
       SELECT
-        *,
         name,
         salary + bonuses AS cost
       FROM
         employees
       LIMIT
         10
     )
     SELECT
       *
     FROM
       (
         SELECT
-          *,
           name,
           salary AS cost
         FROM
           employees
         LIMIT
           3
       ) AS table_1
@@ -3038,15 +3036,15 @@
 }
 
 #[test]
 fn test_closures_and_pipelines() {
     assert_display_snapshot!(compile(
         r###"
     let addthree = a b c -> s"{a} || {b} || {c}"
-    let arg = myarg myfunc -> ( myfunc myarg )
+    let arg = myarg myfunc <func> -> ( myfunc myarg )
 
     from y
     select x = (
         addthree "apples"
         arg "bananas"
         arg "citrus"
     )
```

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/tests/test_bad_error_messages.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/tests/test_bad_error_messages.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/tests/test_error_messages.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/tests/test_error_messages.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/utils/id_gen.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/utils/id_gen.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/utils/mod.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/src/utils/toposort.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/src/utils/toposort.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/README.md` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/README.md`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/connection.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/connection.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/data/chinook/albums.csv` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/albums.csv`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/data/chinook/artists.csv` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/artists.csv`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/data/chinook/customers.csv` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/customers.csv`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/data/chinook/employees.csv` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/employees.csv`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/data/chinook/invoice_items.csv` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/invoice_items.csv`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/data/chinook/invoices.csv` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/invoices.csv`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/data/chinook/playlist_track.csv` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/playlist_track.csv`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/data/chinook/schema.sql` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/schema.sql`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/data/chinook/tracks.csv` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/data/chinook/tracks.csv`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/docker-compose.yml` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/main.rs` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/main.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/queries/arithmetic.prql` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/arithmetic.prql`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/queries/invoice_totals.prql` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/queries/invoice_totals.prql`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@arithmetic.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@arithmetic.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@invoice_totals.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@invoice_totals.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@pipelines.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@pipelines.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@set_ops_remove.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@set_ops_remove.prql.snap`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 ---
-source: prql-compiler/tests/integration/main.rs
+source: crates/prql_compiler/tests/integration/main.rs
 expression: "# mssql:test\nlet distinct = rel -> (from t = _param.rel | group {t.*} (take 1))\n\nfrom_text format:json '{ \"columns\": [\"a\"], \"data\": [[1], [2], [2], [3]] }'\ndistinct\nremove (from_text format:json '{ \"columns\": [\"a\"], \"data\": [[1], [2]] }')\nsort a\n"
-input_file: prql-compiler/tests/integration/queries/set_ops_remove.prql
+input_file: crates/prql_compiler/tests/integration/queries/set_ops_remove.prql
 ---
-let distinct = rel -> (from t = _param.rel | group {t.*} (take 1))
+let distinct = rel -> (
+  from t = _param.rel
+  group {t.*} (take 1)
+)
 
 from_text format:json '{ "columns": ["a"], "data": [[1], [2], [2], [3]] }'
 distinct
 remove (from_text format:json '{ "columns": ["a"], "data": [[1], [2]] }')
 sort a
```

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@sort.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@sort.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@window.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__fmt@window.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@arithmetic.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@arithmetic.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@cast.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@cast.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@distinct.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@distinct.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@distinct_on.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@distinct_on.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@group_all.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@group_all.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@invoice_totals.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@invoice_totals.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@pipelines.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@pipelines.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@sort.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@sort.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@window.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__results@window.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@aggregation.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@aggregation.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@arithmetic.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@arithmetic.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@distinct_on.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@distinct_on.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@group_all.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@group_all.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@group_sort.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@group_sort.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@invoice_totals.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@invoice_totals.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@loop.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@loop.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@pipelines.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@pipelines.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@set_ops_remove.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@set_ops_remove.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@sort.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@sort.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@switch.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@switch.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@window.prql.snap` & `prql_python-0.9.1/local_dependencies/prql-compiler/tests/integration/snapshots/integration__sql@window.prql.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql_parser/src/expr.rs` & `prql_python-0.9.1/local_dependencies/prql_parser/src/expr.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql_parser/src/interpolation.rs` & `prql_python-0.9.1/local_dependencies/prql_parser/src/interpolation.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql_parser/src/lexer.rs` & `prql_python-0.9.1/local_dependencies/prql_parser/src/lexer.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql_parser/src/lib.rs` & `prql_python-0.9.1/local_dependencies/prql_parser/src/lib.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql_parser/src/snapshots/prql_parser__test__pipeline_parse_tree.snap` & `prql_python-0.9.1/local_dependencies/prql_parser/src/snapshots/prql_parser__test__pipeline_parse_tree.snap`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql_parser/src/span.rs` & `prql_python-0.9.1/local_dependencies/prql_parser/src/span.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/local_dependencies/prql_parser/src/stmt.rs` & `prql_python-0.9.1/local_dependencies/prql_parser/src/stmt.rs`

 * *Files 2% similar despite different names*

```diff
@@ -142,13 +142,15 @@
 }
 
 pub fn type_expr() -> impl Parser<Token, Expr, Error = PError> {
     let literal = select! { Token::Literal(lit) => ExprKind::Literal(lit) };
 
     let ident = ident().map(ExprKind::Ident);
 
-    let term = literal.or(ident).map_with_span(into_expr);
+    let func = keyword("func").to(ExprKind::Ident(Ident::from_path(vec!["std", "func"])));
+
+    let term = literal.or(ident).or(func).map_with_span(into_expr);
 
     binary_op_parser(term, operator_or())
         .delimited_by(ctrl('<'), ctrl('>'))
         .labelled("type expression")
 }
```

### Comparing `prql_python-0.9.0/Cargo.toml` & `prql_python-0.9.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 name = "prql-python"
 publish = false
 
 edition= "2021"
 license= "Apache-2.0"
 repository= "https://github.com/PRQL/prql"
 rust-version= "1.65.0"
-version= "0.9.0"
+version= "0.9.1"
 
 [lib]
 crate-type = ["cdylib"]
 name = "prql_python"
 
 [target.'cfg(not(target_family="wasm"))'.dependencies]
 pyo3 = {version = "0.19.0", features = ["abi3-py37"]}
```

### Comparing `prql_python-0.9.0/.gitignore` & `prql_python-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/README.md` & `prql_python-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/noxfile.py` & `prql_python-0.9.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/pyproject.toml` & `prql_python-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/python/tests/test_all.py` & `prql_python-0.9.1/python/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/src/lib.rs` & `prql_python-0.9.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `prql_python-0.9.0/PKG-INFO` & `prql_python-0.9.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prql-python
-Version: 0.9.0
+Version: 0.9.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/PRQL/prql
```

