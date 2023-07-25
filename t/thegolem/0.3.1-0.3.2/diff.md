# Comparing `tmp/thegolem-0.3.1.tar.gz` & `tmp/thegolem-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thegolem-0.3.1.tar", last modified: Tue May 23 10:19:29 2023, max compression
+gzip compressed data, was "thegolem-0.3.2.tar", last modified: Tue Jul 25 11:25:12 2023, max compression
```

## Comparing `thegolem-0.3.1.tar` & `thegolem-0.3.2.tar`

### file list

```diff
@@ -1,197 +1,241 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.212335 thegolem-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-23 10:19:21.000000 thegolem-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-05-23 10:19:29.212335 thegolem-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17967 2023-05-23 10:19:21.000000 thegolem-0.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.180334 thegolem-0.3.1/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:21.000000 thegolem-0.3.1/docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.180334 thegolem-0.3.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:21.000000 thegolem-0.3.1/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-23 10:19:21.000000 thegolem-0.3.1/examples/graph_model_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-23 10:19:21.000000 thegolem-0.3.1/examples/profiler_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.180334 thegolem-0.3.1/examples/structural_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:21.000000 thegolem-0.3.1/examples/structural_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-05-23 10:19:21.000000 thegolem-0.3.1/examples/structural_analysis/opt_graph_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.180334 thegolem-0.3.1/examples/synthetic_graph_evolution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:21.000000 thegolem-0.3.1/examples/synthetic_graph_evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-23 10:19:21.000000 thegolem-0.3.1/examples/synthetic_graph_evolution/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-23 10:19:21.000000 thegolem-0.3.1/examples/synthetic_graph_evolution/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-23 10:19:21.000000 thegolem-0.3.1/examples/synthetic_graph_evolution/graph_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-23 10:19:21.000000 thegolem-0.3.1/examples/synthetic_graph_evolution/simple_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-23 10:19:21.000000 thegolem-0.3.1/examples/synthetic_graph_evolution/tree_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-05-23 10:19:21.000000 thegolem-0.3.1/examples/synthetic_graph_evolution/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-23 10:19:21.000000 thegolem-0.3.1/examples/viz_with_labels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.180334 thegolem-0.3.1/golem/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.180334 thegolem-0.3.1/golem/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.184334 thegolem-0.3.1/golem/core/adapter/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/adapter/adapt_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/adapter/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/adapter/nx_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.184334 thegolem-0.3.1/golem/core/dag/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/dag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/dag/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/dag/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/dag/graph_delegate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/dag/graph_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/dag/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/dag/graph_verifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/dag/linked_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/dag/linked_graph_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/dag/verification_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.188334 thegolem-0.3.1/golem/core/optimisers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/advisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.188334 thegolem-0.3.1/golem/core/optimisers/archive/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/archive/generation_keeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/archive/individuals_containers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.188334 thegolem-0.3.1/golem/core/optimisers/fitness/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/fitness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/fitness/fitness.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/fitness/multi_objective_fitness.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.188334 thegolem-0.3.1/golem/core/optimisers/genetic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/genetic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/genetic/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/genetic/gp_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/genetic/gp_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/genetic/gp_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.192335 thegolem-0.3.1/golem/core/optimisers/genetic/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/genetic/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14366 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/genetic/operators/base_mutations.py
--rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/genetic/operators/crossover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/genetic/operators/elitism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/genetic/operators/inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/genetic/operators/mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/genetic/operators/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/genetic/operators/regularization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9331 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/genetic/operators/selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.192335 thegolem-0.3.1/golem/core/optimisers/genetic/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/genetic/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/genetic/parameters/graph_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/genetic/parameters/mutation_prob.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/genetic/parameters/operators_prob.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/genetic/parameters/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/genetic/parameters/population_size.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/graph_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/initial_graphs_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.192335 thegolem-0.3.1/golem/core/optimisers/objective/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/objective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/objective/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/objective/objective_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/opt_graph_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.196335 thegolem-0.3.1/golem/core/optimisers/opt_history_objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/opt_history_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/opt_history_objects/generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/opt_history_objects/individual.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/opt_history_objects/opt_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/opt_history_objects/parent_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/opt_node_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/optimization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/populational_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.196335 thegolem-0.3.1/golem/core/optimisers/random/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/random/random_mutation_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/random/random_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/random_graph_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/optimisers/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.196335 thegolem-0.3.1/golem/core/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/tuning/search_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/tuning/sequential.py
--rw-r--r--   0 runner    (1001) docker     (123)     8793 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/tuning/simultaneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/tuning/tuner_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.196335 thegolem-0.3.1/golem/core/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/utilities/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/utilities/grouped_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/utilities/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/utilities/sequence_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/utilities/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/core/utilities/singleton_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.200335 thegolem-0.3.1/golem/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/metrics/edit_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/metrics/graph_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/metrics/graph_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/metrics/mmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.200335 thegolem-0.3.1/golem/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/serializers/any_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.200335 thegolem-0.3.1/golem/serializers/coders/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/serializers/coders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/serializers/coders/enum_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/serializers/coders/graph_node_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/serializers/coders/graph_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/serializers/coders/opt_history_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/serializers/coders/parent_operator_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/serializers/coders/uuid_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/serializers/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.200335 thegolem-0.3.1/golem/structural_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/structural_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/structural_analysis/base_sa_approaches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.204335 thegolem-0.3.1/golem/structural_analysis/graph_sa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/structural_analysis/graph_sa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14396 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/structural_analysis/graph_sa/edge_sa_approaches.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/structural_analysis/graph_sa/edges_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.204335 thegolem-0.3.1/golem/structural_analysis/graph_sa/entities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/structural_analysis/graph_sa/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/structural_analysis/graph_sa/entities/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/structural_analysis/graph_sa/graph_structural_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    13975 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/structural_analysis/graph_sa/node_sa_approaches.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/structural_analysis/graph_sa/nodes_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/structural_analysis/graph_sa/postproc_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.204335 thegolem-0.3.1/golem/structural_analysis/graph_sa/results/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/structural_analysis/graph_sa/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/structural_analysis/graph_sa/results/base_sa_approach_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/structural_analysis/graph_sa/results/deletion_sa_approach_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/structural_analysis/graph_sa/results/object_sa_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/structural_analysis/graph_sa/results/replace_sa_approach_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/structural_analysis/graph_sa/results/sa_analysis_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/structural_analysis/graph_sa/results/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/structural_analysis/graph_sa/sa_approaches_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/structural_analysis/graph_sa/sa_requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.204335 thegolem-0.3.1/golem/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/utilities/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.204335 thegolem-0.3.1/golem/utilities/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/utilities/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/utilities/profiler/memory_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/utilities/profiler/time_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/utilities/requirements_notificator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.208335 thegolem-0.3.1/golem/visualisation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20647 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/visualisation/graph_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.208335 thegolem-0.3.1/golem/visualisation/opt_history/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/visualisation/opt_history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/visualisation/opt_history/arg_constraint_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/visualisation/opt_history/fitness_box.py
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/visualisation/opt_history/fitness_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/visualisation/opt_history/graphs_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/visualisation/opt_history/history_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/visualisation/opt_history/operations_animated_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/visualisation/opt_history/operations_kde.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/visualisation/opt_history/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/visualisation/opt_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-05-23 10:19:21.000000 thegolem-0.3.1/golem/visualisation/opt_viz_extra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.208335 thegolem-0.3.1/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:21.000000 thegolem-0.3.1/libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.208335 thegolem-0.3.1/libs/netcomp/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-23 10:19:21.000000 thegolem-0.3.1/libs/netcomp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-23 10:19:21.000000 thegolem-0.3.1/libs/netcomp/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-23 10:19:21.000000 thegolem-0.3.1/libs/netcomp/eigenstuff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-23 10:19:21.000000 thegolem-0.3.1/libs/netcomp/matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 10:19:29.212335 thegolem-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-23 10:19:21.000000 thegolem-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:19:29.212335 thegolem-0.3.1/thegolem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-05-23 10:19:29.000000 thegolem-0.3.1/thegolem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-05-23 10:19:29.000000 thegolem-0.3.1/thegolem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 10:19:29.000000 thegolem-0.3.1/thegolem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-23 10:19:29.000000 thegolem-0.3.1/thegolem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-23 10:19:29.000000 thegolem-0.3.1/thegolem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.831920 thegolem-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-25 11:25:05.000000 thegolem-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-07-25 11:25:12.831920 thegolem-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18221 2023-07-25 11:25:05.000000 thegolem-0.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.803919 thegolem-0.3.2/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.803919 thegolem-0.3.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.807919 thegolem-0.3.2/examples/adaptive_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/adaptive_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/adaptive_optimizer/context_mab_experiment_different_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/adaptive_optimizer/experiment_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/adaptive_optimizer/mab_experiment_different_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/adaptive_optimizer/neural_mab_experiment_different_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/adaptive_optimizer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/graph_model_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.807919 thegolem-0.3.2/examples/molecule_search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/molecule_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/molecule_search/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/molecule_search/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/molecule_search/guacamol_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/molecule_search/mol_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/molecule_search/mol_advisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/molecule_search/mol_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/molecule_search/mol_graph_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/molecule_search/mol_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/molecule_search/mol_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/molecule_search/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/profiler_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.807919 thegolem-0.3.2/examples/structural_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/structural_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/structural_analysis/opt_graph_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.807919 thegolem-0.3.2/examples/synthetic_graph_evolution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/synthetic_graph_evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/synthetic_graph_evolution/experiment_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/synthetic_graph_evolution/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/synthetic_graph_evolution/graph_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/synthetic_graph_evolution/simple_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/synthetic_graph_evolution/tree_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/synthetic_graph_evolution/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-25 11:25:05.000000 thegolem-0.3.2/examples/viz_with_labels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.807919 thegolem-0.3.2/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.807919 thegolem-0.3.2/experiments/mab/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/experiments/mab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-07-25 11:25:05.000000 thegolem-0.3.2/experiments/mab/mab_synthetic_experiment_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.807919 thegolem-0.3.2/golem/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.807919 thegolem-0.3.2/golem/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.811919 thegolem-0.3.2/golem/core/adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/adapter/adapt_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/adapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/adapter/nx_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.811919 thegolem-0.3.2/golem/core/dag/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/dag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/dag/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/dag/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/dag/graph_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/dag/graph_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/dag/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/dag/graph_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/dag/linked_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/dag/linked_graph_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/dag/verification_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.811919 thegolem-0.3.2/golem/core/optimisers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.811919 thegolem-0.3.2/golem/core/optimisers/adaptive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/adaptive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/adaptive/context_agents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.815919 thegolem-0.3.2/golem/core/optimisers/adaptive/mab_agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/adaptive/mab_agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/adaptive/mab_agents/contextual_mab_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/adaptive/mab_agents/mab_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/adaptive/mab_agents/neural_contextual_mab_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/adaptive/neural_mab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/adaptive/operator_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/advisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.815919 thegolem-0.3.2/golem/core/optimisers/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/archive/generation_keeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/archive/individuals_containers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.815919 thegolem-0.3.2/golem/core/optimisers/fitness/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/fitness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/fitness/fitness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/fitness/multi_objective_fitness.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.815919 thegolem-0.3.2/golem/core/optimisers/genetic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/genetic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/genetic/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/genetic/gp_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/genetic/gp_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/genetic/gp_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.815919 thegolem-0.3.2/golem/core/optimisers/genetic/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/genetic/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14938 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/genetic/operators/base_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/genetic/operators/crossover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/genetic/operators/elitism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/genetic/operators/inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/genetic/operators/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/genetic/operators/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/genetic/operators/regularization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/genetic/operators/reproduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9523 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/genetic/operators/selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.815919 thegolem-0.3.2/golem/core/optimisers/genetic/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/genetic/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/genetic/parameters/graph_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/genetic/parameters/mutation_prob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/genetic/parameters/operators_prob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/genetic/parameters/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/genetic/parameters/population_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/graph_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/initial_graphs_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.819919 thegolem-0.3.2/golem/core/optimisers/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/meta/surrogate_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/meta/surrogate_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/meta/surrogate_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.819919 thegolem-0.3.2/golem/core/optimisers/objective/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/objective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/objective/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/objective/objective_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/opt_graph_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.819919 thegolem-0.3.2/golem/core/optimisers/opt_history_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/opt_history_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/opt_history_objects/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/opt_history_objects/individual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10213 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/opt_history_objects/opt_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/opt_history_objects/parent_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/opt_node_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/optimization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/populational_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.819919 thegolem-0.3.2/golem/core/optimisers/random/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/random/random_mutation_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/random/random_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/random_graph_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/optimisers/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.819919 thegolem-0.3.2/golem/core/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/tuning/hyperopt_tuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/tuning/iopt_tuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/tuning/optuna_tuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/tuning/search_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/tuning/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/tuning/simultaneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/tuning/tuner_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.819919 thegolem-0.3.2/golem/core/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/utilities/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/utilities/grouped_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/utilities/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/utilities/sequence_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/utilities/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/core/utilities/singleton_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.823919 thegolem-0.3.2/golem/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/metrics/edit_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/metrics/graph_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/metrics/graph_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/metrics/mmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.823919 thegolem-0.3.2/golem/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/serializers/any_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.823919 thegolem-0.3.2/golem/serializers/coders/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/serializers/coders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/serializers/coders/enum_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/serializers/coders/graph_node_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/serializers/coders/graph_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/serializers/coders/opt_history_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/serializers/coders/parent_operator_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/serializers/coders/uuid_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16048 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/serializers/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.823919 thegolem-0.3.2/golem/structural_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/structural_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/structural_analysis/base_sa_approaches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.823919 thegolem-0.3.2/golem/structural_analysis/graph_sa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/structural_analysis/graph_sa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14312 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/structural_analysis/graph_sa/edge_sa_approaches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/structural_analysis/graph_sa/edges_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.823919 thegolem-0.3.2/golem/structural_analysis/graph_sa/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/structural_analysis/graph_sa/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/structural_analysis/graph_sa/entities/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/structural_analysis/graph_sa/graph_structural_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13975 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/structural_analysis/graph_sa/node_sa_approaches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/structural_analysis/graph_sa/nodes_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/structural_analysis/graph_sa/postproc_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.823919 thegolem-0.3.2/golem/structural_analysis/graph_sa/results/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/structural_analysis/graph_sa/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/structural_analysis/graph_sa/results/base_sa_approach_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/structural_analysis/graph_sa/results/deletion_sa_approach_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/structural_analysis/graph_sa/results/object_sa_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/structural_analysis/graph_sa/results/replace_sa_approach_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/structural_analysis/graph_sa/results/sa_analysis_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/structural_analysis/graph_sa/results/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/structural_analysis/graph_sa/sa_approaches_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/structural_analysis/graph_sa/sa_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.827919 thegolem-0.3.2/golem/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/utilities/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.827919 thegolem-0.3.2/golem/utilities/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/utilities/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/utilities/profiler/memory_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/utilities/profiler/time_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/utilities/requirements_notificator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.827919 thegolem-0.3.2/golem/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/visualisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20622 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/visualisation/graph_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.827919 thegolem-0.3.2/golem/visualisation/opt_history/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/visualisation/opt_history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/visualisation/opt_history/arg_constraint_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/visualisation/opt_history/diversity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/visualisation/opt_history/fitness_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14945 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/visualisation/opt_history/fitness_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/visualisation/opt_history/graphs_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/visualisation/opt_history/history_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/visualisation/opt_history/operations_animated_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/visualisation/opt_history/operations_kde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/visualisation/opt_history/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/visualisation/opt_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-07-25 11:25:05.000000 thegolem-0.3.2/golem/visualisation/opt_viz_extra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.827919 thegolem-0.3.2/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:05.000000 thegolem-0.3.2/libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.827919 thegolem-0.3.2/libs/netcomp/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-25 11:25:05.000000 thegolem-0.3.2/libs/netcomp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-25 11:25:05.000000 thegolem-0.3.2/libs/netcomp/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-25 11:25:05.000000 thegolem-0.3.2/libs/netcomp/eigenstuff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-25 11:25:05.000000 thegolem-0.3.2/libs/netcomp/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 11:25:12.831920 thegolem-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-25 11:25:05.000000 thegolem-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:12.827919 thegolem-0.3.2/thegolem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-07-25 11:25:12.000000 thegolem-0.3.2/thegolem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-07-25 11:25:12.000000 thegolem-0.3.2/thegolem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 11:25:12.000000 thegolem-0.3.2/thegolem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-25 11:25:12.000000 thegolem-0.3.2/thegolem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-25 11:25:12.000000 thegolem-0.3.2/thegolem.egg-info/top_level.txt
```

### Comparing `thegolem-0.3.1/LICENSE` & `thegolem-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/PKG-INFO` & `thegolem-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: thegolem
-Version: 0.3.1
+Version: 0.3.2
 Summary: Framework for Graph Optimization and Learning by Evolutionary Methods
 Home-page: https://github.com/aimclub/GOLEM
 Author: NSS Lab
 Author-email: itmo.nss.team@gmail.com
 License: BSD 3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: profilers
+Provides-Extra: molecules
+Provides-Extra: adaptive
 License-File: LICENSE
 
 .. image:: /docs/source/img/golem_logo-02.png
    :alt: Logo of GOLEM framework
    :align: center
    :width: 500
 
 .. class:: center
 
     |sai| |itmo|
 
-    |python| |pypi| |build| |docs| |license| |tg| |rus| |mirror|
+    |python| |pypi| |build| |integration| |docs| |license| |tg| |rus| |mirror|
 
 
 Graph Optimization and Learning by Evolutionary Methods
 -------------------------------------------------------
 
 GOLEM is an open-source AI framework for optimization and learning of structured graph-based models with meta-heuristic
 methods. It is centered around 2 ideas:
@@ -205,14 +207,18 @@
     :target: https://thegolem.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. |build| image:: https://github.com/aimclub/GOLEM/actions/workflows/unit-build.yml/badge.svg?branch=main
    :alt: Build Status
    :target: https://github.com/aimclub/GOLEM/actions/workflows/unit-build.yml
 
+.. |integration| image:: https://github.com/aimclub/GOLEM/actions/workflows/integration-build.yml/badge.svg?branch=main
+   :alt: Integration Build Status
+   :target: https://github.com/aimclub/GOLEM/actions/workflows/integration-build.yml
+
 .. |coverage| image:: https://codecov.io/gh/aimclub/GOLEM/branch/main/graph/badge.svg
    :alt: Coverage Status
    :target: https://codecov.io/gh/aimclub/GOLEM
 
 .. |pypi| image:: https://img.shields.io/pypi/v/thegolem.svg
    :alt: PyPI Package Version
    :target: https://img.shields.io/pypi/v/thegolem
```

### Comparing `thegolem-0.3.1/README.rst` & `thegolem-0.3.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
    :align: center
    :width: 500
 
 .. class:: center
 
     |sai| |itmo|
 
-    |python| |pypi| |build| |docs| |license| |tg| |eng| |mirror|
+    |python| |pypi| |build| |integration| |docs| |license| |tg| |eng| |mirror|
 
 
 Оптимизация и обучение графовых моделей эволюционными методами
 --------------------------------------------------------------
 
 GOLEM - это фреймворк искусственного интеллекта с открытым исходным кодом для оптимизации и обучения структурированных
 моделей на основе графов с помощью метаэвристических методов. Он основан на двух идеях:
@@ -188,14 +188,18 @@
     :target: https://thegolem.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. |build| image:: https://github.com/aimclub/GOLEM/actions/workflows/unit-build.yml/badge.svg?branch=main
    :alt: Build Status
    :target: https://github.com/aimclub/GOLEM/actions/workflows/unit-build.yml
 
+.. |integration| image:: https://github.com/aimclub/GOLEM/actions/workflows/integration-build.yml/badge.svg?branch=main
+   :alt: Integration Build Status
+   :target: https://github.com/aimclub/GOLEM/actions/workflows/integration-build.yml
+
 .. |coverage| image:: https://codecov.io/gh/aimclub/GOLEM/branch/main/graph/badge.svg
    :alt: Coverage Status
    :target: https://codecov.io/gh/aimclub/GOLEM
 
 .. |pypi| image:: https://img.shields.io/pypi/v/thegolem.svg
    :alt: PyPI Package Version
    :target: https://img.shields.io/pypi/v/thegolem
```

### Comparing `thegolem-0.3.1/examples/graph_model_optimization.py` & `thegolem-0.3.2/examples/graph_model_optimization.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/examples/profiler_example.py` & `thegolem-0.3.2/examples/profiler_example.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/examples/structural_analysis/opt_graph_optimization.py` & `thegolem-0.3.2/examples/structural_analysis/opt_graph_optimization.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/examples/synthetic_graph_evolution/experiment.py` & `thegolem-0.3.2/examples/synthetic_graph_evolution/experiment_setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from datetime import datetime, timedelta
 from functools import partial
 from io import StringIO
 from itertools import product
 from pathlib import Path
-from typing import Sequence, Type, Callable, Optional
+from typing import Sequence, Type, Callable, Optional, List
+
+import networkx as nx
+import numpy as np
 
 from examples.synthetic_graph_evolution.generators import generate_labeled_graph, graph_kinds
 from examples.synthetic_graph_evolution.utils import draw_graphs_subplots
 from golem.core.adapter.nx_adapter import BaseNetworkxAdapter
 from golem.core.optimisers.genetic.gp_optimizer import EvoGraphOptimizer
 from golem.core.optimisers.optimizer import GraphOptimizer
 from golem.metrics.edit_distance import get_edit_dist_metric, matrix_edit_dist
-from golem.metrics.graph_metrics import *
+from golem.metrics.graph_metrics import \
+    spectral_dist, size_diff, degree_distance_kernel, degree_distance, nxgraph_stats
 
 
 def get_all_quality_metrics(target_graph):
     quality_metrics = {
         'edit_distance': get_edit_dist_metric(target_graph),
         'matrix_edit_dist': partial(matrix_edit_dist, target_graph),
         'sp_adj': partial(spectral_dist, target_graph, kind='adjacency'),
@@ -66,15 +70,18 @@
 
             duration = datetime.now() - start_time
             print(f'Trial #{i} finished, spent time: {duration}', file=log)
             print('target graph stats: ', nxgraph_stats(target_graph), file=log)
             print('found graph stats: ', nxgraph_stats(found_nx_graph), file=log)
             if visualize:
                 draw_graphs_subplots(target_graph, found_nx_graph,
-                                     titles=['Target Graph', 'Found Graph'])
+                                     titles=['Target Graph', 'Found Graph'], show=False)
+                diversity_filename = (f'./results/diversity_hist_{graph_name}_n{num_nodes}.gif')
+                history.show.diversity_population(save_path=diversity_filename)
+                history.show.diversity_line(show=False)
                 history.show.fitness_line()
             history.save(f'./results/hist_{graph_name}_n{num_nodes}_trial{i}.json')
 
         # Compute mean & std for metrics of trials
         ff = objective.format_fitness
         trial_metrics = np.array([ind.fitness.values for ind in trial_results])
         trial_metrics_mean = trial_metrics.mean(axis=0)
@@ -87,16 +94,18 @@
     return log.getvalue()
 
 
 def run_trial(target_graph: nx.DiGraph,
               optimizer_setup: Callable,
               optimizer_cls: Type[GraphOptimizer] = EvoGraphOptimizer,
               timeout: Optional[timedelta] = None,
-              num_iterations: Optional[int] = None):
+              num_iterations: Optional[int] = None,
+              node_types: Optional[List[str]] = None):
     optimizer, objective = optimizer_setup(target_graph,
                                            optimizer_cls=optimizer_cls,
                                            timeout=timeout,
+                                           node_types=node_types,
                                            num_iterations=num_iterations)
     found_graphs = optimizer.optimise(objective)
     found_graph = found_graphs[0] if isinstance(found_graphs, Sequence) else found_graphs
     history = optimizer.history
     return found_graph, history
```

### Comparing `thegolem-0.3.1/examples/synthetic_graph_evolution/generators.py` & `thegolem-0.3.2/examples/synthetic_graph_evolution/generators.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,17 +86,19 @@
 
 def generate_labeled_graph(kind: str,
                            size: int,
                            node_labels: Optional[Sequence[str]] = ('x',),
                            connected: bool = True,
                            directed: bool = True):
     """Generate randomly labeled graph of the specified kind and size,
-    optionally enforce connectedness and direction."""
-    graph = graph_generators[kind](size)
-    return postprocess_nx_graph(graph, node_labels, connected, directed)
+    optionally enforce connectedness and direction. Important! With small specified size
+    some methods can generate smaller graphs due to removal of unconnected components."""
+    nx_graph = graph_generators[kind](size)
+    graph = postprocess_nx_graph(nx_graph, node_labels, connected, directed)
+    return graph
 
 
 def _draw_sample_graphs(kind: str = 'gnp', sizes=tuple(range(5, 50, 5))):
     graphs = [generate_labeled_graph(kind, n) for n in sizes]
     draw_graphs_subplots(*graphs)
```

### Comparing `thegolem-0.3.1/examples/synthetic_graph_evolution/graph_search.py` & `thegolem-0.3.2/examples/synthetic_graph_evolution/graph_search.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,104 @@
 from datetime import timedelta
 from functools import partial
-from typing import Type, Optional
+from typing import Type, Optional, Sequence, List
 
-from examples.synthetic_graph_evolution.experiment import run_experiments
-from examples.synthetic_graph_evolution.generators import generate_labeled_graph
+import networkx as nx
+from examples.synthetic_graph_evolution.experiment_setup import run_experiments
 from golem.core.adapter.nx_adapter import BaseNetworkxAdapter
-from golem.core.dag.verification_rules import has_no_self_cycled_nodes
+from golem.core.dag.graph import Graph
+from golem.core.dag.verification_rules import DEFAULT_DAG_RULES
+from golem.core.optimisers.adaptive.operator_agent import MutationAgentTypeEnum
 from golem.core.optimisers.genetic.gp_optimizer import EvoGraphOptimizer
 from golem.core.optimisers.genetic.gp_params import GPAlgorithmParameters
 from golem.core.optimisers.genetic.operators.base_mutations import MutationTypesEnum
 from golem.core.optimisers.genetic.operators.crossover import CrossoverTypesEnum
 from golem.core.optimisers.genetic.operators.inheritance import GeneticSchemeTypesEnum
 from golem.core.optimisers.objective import Objective
 from golem.core.optimisers.optimization_parameters import GraphRequirements
-from golem.core.optimisers.optimizer import GraphGenerationParams, GraphOptimizer
-from golem.metrics.graph_metrics import *
+from golem.core.optimisers.optimizer import GraphGenerationParams, GraphOptimizer, AlgorithmParameters
+from golem.metrics.graph_metrics import spectral_dist, size_diff, degree_distance
 
 
-def graph_search_setup(target_graph: nx.DiGraph,
+def graph_search_setup(target_graph: Optional[nx.DiGraph] = None,
+                       objective: Optional[Objective] = None,
                        optimizer_cls: Type[GraphOptimizer] = EvoGraphOptimizer,
-                       node_types: Sequence[str] = ('X',),
+                       algorithm_parameters: Optional[AlgorithmParameters] = None,
+                       node_types: Sequence[str] = ('x',),
                        timeout: Optional[timedelta] = None,
-                       num_iterations: Optional[int] = None):
+                       num_iterations: Optional[int] = None,
+                       initial_graph_sizes: Optional[List[int]] = None,
+                       initial_graphs: List[Graph] = None,
+                       pop_size: int = None):
+    if target_graph is not None and objective is not None:
+        raise ValueError('Please provide either target or objective, not both')
+    elif target_graph is not None:
+        # Setup objective that measures some graph-theoretic similarity measure
+        objective = Objective(
+            quality_metrics={
+                'sp_adj': partial(spectral_dist, target_graph, kind='adjacency'),
+                'sp_lapl': partial(spectral_dist, target_graph, kind='laplacian'),
+            },
+            complexity_metrics={
+                'graph_size': partial(size_diff, target_graph),
+                'degree': partial(degree_distance, target_graph),
+            },
+            is_multi_objective=True
+        )
+        max_graph_size = target_graph.number_of_nodes()
+    elif objective is not None:
+        max_graph_size = 1000
+    else:
+        raise ValueError()
+
     # Setup parameters
-    num_nodes = target_graph.number_of_nodes()
     requirements = GraphRequirements(
-        max_arity=num_nodes,
-        max_depth=num_nodes,
-        early_stopping_timeout=5,
-        early_stopping_iterations=1000,
+        max_arity=max_graph_size,
+        max_depth=max_graph_size,
+        early_stopping_timeout=10,
+        early_stopping_iterations=num_iterations // 3 if num_iterations else None,
         keep_n_best=4,
         timeout=timeout,
         num_of_generations=num_iterations,
         n_jobs=-1,
         history_dir=None,
     )
-    gp_params = GPAlgorithmParameters(
-        multi_objective=True,
-        genetic_scheme_type=GeneticSchemeTypesEnum.parameter_free,
+    default_gp_params = GPAlgorithmParameters(
+        adaptive_mutation_type=MutationAgentTypeEnum.random,
+        pop_size=pop_size or 21,
+        multi_objective=objective.is_multi_objective,
+        genetic_scheme_type=GeneticSchemeTypesEnum.generational,
         mutation_types=[
             MutationTypesEnum.single_add,
-            MutationTypesEnum.single_drop,
             MutationTypesEnum.single_edge,
+            MutationTypesEnum.single_drop
         ],
+        crossover_types=[CrossoverTypesEnum.none]
     )
+    gp_params = algorithm_parameters or default_gp_params
     graph_gen_params = GraphGenerationParams(
         adapter=BaseNetworkxAdapter(),
-        rules_for_constraint=[has_no_self_cycled_nodes],
+        rules_for_constraint=DEFAULT_DAG_RULES,
         available_node_types=node_types,
     )
 
-    # Setup objective that measures some graph-theoretic similarity measure
-    objective = Objective(
-        quality_metrics={
-            'sp_adj': partial(spectral_dist, target_graph, kind='adjacency'),
-            'sp_lapl': partial(spectral_dist, target_graph, kind='laplacian'),
-        },
-        complexity_metrics={
-            'degree': partial(degree_distance, target_graph),
-            'graph_size': partial(size_diff, target_graph),
-        },
-        is_multi_objective=True
-    )
-
     # Generate simple initial population with line graphs
-    initial_graphs = [generate_labeled_graph('line', k+3, node_types)
-                      for k in range(gp_params.pop_size)]
+    if not initial_graphs:
+        if not initial_graph_sizes:
+            initial_graph_sizes = [7] * gp_params.pop_size
+        initial_graphs = [nx.random_tree(initial_graph_sizes[i], create_using=nx.DiGraph)
+                          for i in range(gp_params.pop_size)]
     # Build the optimizer
     optimiser = optimizer_cls(objective, initial_graphs, requirements, graph_gen_params, gp_params)
     return optimiser, objective
 
 
 if __name__ == '__main__':
     results_log = run_experiments(optimizer_setup=graph_search_setup,
                                   optimizer_cls=EvoGraphOptimizer,
-                                  graph_names=['2ring', 'gnp'],
-                                  graph_sizes=[30, 100],
+                                  graph_names=['gnp'],
+                                  graph_sizes=[50],
                                   num_trials=1,
-                                  trial_timeout=5,
-                                  trial_iterations=2000,
+                                  trial_timeout=15,
+                                  trial_iterations=1000,
                                   visualize=True)
     print(results_log)
```

### Comparing `thegolem-0.3.1/examples/synthetic_graph_evolution/simple_run.py` & `thegolem-0.3.2/examples/synthetic_graph_evolution/simple_run.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/examples/synthetic_graph_evolution/tree_search.py` & `thegolem-0.3.2/examples/synthetic_graph_evolution/tree_search.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,94 @@
 from datetime import timedelta
 from functools import partial
 from typing import Type, Optional, Sequence
 
 import networkx as nx
 
-from examples.synthetic_graph_evolution.experiment import run_experiments
+from examples.synthetic_graph_evolution.experiment_setup import run_experiments
 from examples.synthetic_graph_evolution.generators import generate_labeled_graph
 from golem.core.adapter.nx_adapter import BaseNetworkxAdapter
 from golem.core.dag.verification_rules import DEFAULT_DAG_RULES
 from golem.core.optimisers.genetic.gp_optimizer import EvoGraphOptimizer
 from golem.core.optimisers.genetic.gp_params import GPAlgorithmParameters
 from golem.core.optimisers.genetic.operators.base_mutations import MutationTypesEnum
 from golem.core.optimisers.genetic.operators.crossover import CrossoverTypesEnum
 from golem.core.optimisers.objective import Objective
 from golem.core.optimisers.optimization_parameters import GraphRequirements
-from golem.core.optimisers.optimizer import GraphGenerationParams, GraphOptimizer
+from golem.core.optimisers.optimizer import GraphGenerationParams, GraphOptimizer, AlgorithmParameters
 from golem.metrics.edit_distance import tree_edit_dist
 from golem.metrics.graph_metrics import degree_distance
 
 
-def tree_search_setup(target_graph: nx.DiGraph,
+def tree_search_setup(target_graph: Optional[nx.DiGraph] = None,
+                      objective: Optional[Objective] = None,
                       optimizer_cls: Type[GraphOptimizer] = EvoGraphOptimizer,
+                      algorithm_parameters: Optional[AlgorithmParameters] = None,
                       node_types: Sequence[str] = ('x',),
                       timeout: Optional[timedelta] = None,
                       num_iterations: Optional[int] = None):
+    if target_graph is not None and objective is not None:
+        raise ValueError('Please provide either target or objective, not both')
+    elif target_graph is not None:
+        # Setup objective:
+        # - primary metric is edit distance between 2 trees
+        # - secondary metric is difference in node degree distribution
+        objective = Objective(
+            quality_metrics={'edit_dist': partial(tree_edit_dist, target_graph)},
+            complexity_metrics={'degree': partial(degree_distance, target_graph)},
+            is_multi_objective=False,
+        )
+        max_graph_size = target_graph.number_of_nodes()
+    elif objective is not None:
+        max_graph_size = 1000
+    else:
+        raise ValueError()
+
     # Setup parameters
-    num_nodes = target_graph.number_of_nodes()
     requirements = GraphRequirements(
-        max_arity=num_nodes,
-        max_depth=num_nodes,
+        max_arity=max_graph_size,
+        max_depth=max_graph_size,
         early_stopping_timeout=10,
-        early_stopping_iterations=500,
+        early_stopping_iterations=num_iterations // 3 if num_iterations else None,
         keep_n_best=4,
         max_graph_fit_time=timedelta(seconds=10),
         timeout=timeout,
         num_of_generations=num_iterations,
         n_jobs=-1,
         history_dir=None,
     )
-    gp_params = GPAlgorithmParameters(
-        multi_objective=False,
+    default_gp_params = GPAlgorithmParameters(
+        multi_objective=objective.is_multi_objective,
         mutation_types=[
             MutationTypesEnum.single_add,
             MutationTypesEnum.single_drop,
         ],
-        crossover_types=[CrossoverTypesEnum.subtree]
+        crossover_types=[CrossoverTypesEnum.none]
     )
+    gp_params = algorithm_parameters or default_gp_params
     graph_gen_params = GraphGenerationParams(
         adapter=BaseNetworkxAdapter(),
         rules_for_constraint=DEFAULT_DAG_RULES,
         available_node_types=node_types,
     )
 
-    # Setup objective:
-    # - primary metric is edit distance between 2 trees
-    # - secondary metric is difference in node degree distribution
-    objective = Objective(
-        quality_metrics={'edit_dist': partial(tree_edit_dist, target_graph)},
-        complexity_metrics={'degree': partial(degree_distance, target_graph)},
-        is_multi_objective=gp_params.multi_objective
-    )
-
     # Generate simple initial population with small tree graphs
     initial_graphs = [generate_labeled_graph('tree', 5, node_types)
                       for _ in range(gp_params.pop_size)]
     # Build the optimizer
     optimiser = optimizer_cls(objective, initial_graphs, requirements, graph_gen_params, gp_params)
     return optimiser, objective
 
 
 if __name__ == '__main__':
     """
-    In this experiment Optimizer is expected to find the target graph 
+    In this experiment Optimizer is expected to find the target graph
     (exact or almost exact, depending on available time and graph complexity)
     using Tree Edit Distance metric and a random tree (nx.random_tree) as target.
-    
+
     This convergence can be seen from achieved metrics and visually from graph plots.
     """
     results_log = run_experiments(optimizer_setup=tree_search_setup,
                                   optimizer_cls=EvoGraphOptimizer,
                                   graph_names=['tree'],
                                   graph_sizes=[16],
                                   num_trials=1,
```

### Comparing `thegolem-0.3.1/examples/synthetic_graph_evolution/utils.py` & `thegolem-0.3.2/examples/synthetic_graph_evolution/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from datetime import datetime
-from itertools import chain, product
-from typing import Tuple, Optional, Sequence, Iterable
+from itertools import chain
+from typing import Tuple, Optional, Sequence
 
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
 import networkx as nx
 import numpy as np
 from matplotlib import cm
 
@@ -68,53 +67,74 @@
         ax.fill_between(xs, mean - std, mean + std, alpha=0.25)
 
     return fig, ax
 
 
 def plot_nx_graph(g: nx.DiGraph, ax: plt.Axes = None):
     adapter = BaseNetworkxAdapter()
-    GraphVisualizer.draw_nx_dag(adapter.adapt(g), ax,
-                                node_size_scale=0.2, font_size_scale=0.25,
-                                edge_curvature_scale=0.5)
+    GraphVisualizer(adapter.adapt(g)).draw_nx_dag(ax,
+                                                  node_size_scale=0.2,
+                                                  font_size_scale=0.25,
+                                                  edge_curvature_scale=0.5)
 
 
 def draw_graphs_subplots(*graphs: nx.Graph,
                          titles: Optional[Sequence[str]] = None,
-                         draw_fn=nx.draw_kamada_kawai,
-                         size=10):
+                         color_degrees: bool = False,
+                         with_labels: bool = False,
+                         draw_fn=nx.draw,
+                         size: int = 10,
+                         show: bool = True):
+    """Draw 1 or several NetworkX graphs
+    with coloring of roots, sources and node degrees.
+
+    Args:
+        graphs: 1 or many instances of nx.Graph
+        titles: optional sequence of titles for graph subplots
+        color_degrees: flag specifying if graph nodes must be colored relative to their degree
+        with_labels: flag specifying if graph nodes must be drawn with labels
+        draw_fn: nx.draw_* primitive for drawing graph subplots
+        size: figure size, passed to plt.subplots(figsize=...)
+        show: if plt.show() is necessary
+    """
+
     graphs = ensure_wrapped_in_sequence(graphs)
-    titles = [f'Graph #{i+1}' for i in range(len(graphs))] if not titles else titles
+    titles = [f'Graph #{i + 1}' for i in range(len(graphs))] if not titles else titles
     # Setup subplots
     ncols = int(np.ceil(np.sqrt(len(graphs))))
     nrows = len(graphs) // ncols
     aspect = nrows / ncols
     figsize = (size, int(size * aspect))
     fig, axs = plt.subplots(nrows, ncols, figsize=figsize)
     axs = np.atleast_2d(axs)
     # Draw graphs
     for title, ax, graph in zip(titles, chain(*axs), graphs):
-        colors, labeldict, legend_handles = _get_node_colors_and_labels(graph)
+        colors, labeldict, legend_handles = _get_node_colors_and_labels(graph, color_degrees)
         draw_fn(graph, ax=ax, arrows=True,
-                node_color=colors, with_labels=True, labels=labeldict)
+                node_color=colors, with_labels=with_labels, labels=labeldict)
         ax.set_title(title)
     fig.legend(handles=legend_handles)
-    plt.show()
+    if show:
+        plt.show()
 
 
-def _get_node_colors_and_labels(graph: nx.Graph, cmap_name='viridis'):
+def _get_node_colors_and_labels(graph: nx.Graph,
+                                color_degrees: bool = True,
+                                cmap_name='viridis'):
     degrees = dict(graph.degree())
     if isinstance(graph, nx.DiGraph):
         roots = {n for n, d in graph.out_degree() if d == 0}
         sources = {n for n, d in graph.in_degree() if d == 0}
     else:
         roots = {max(*graph.nodes(), key=lambda n: graph.degree[n])}
         sources = {min(*graph.nodes(), key=lambda n: graph.degree[n])}
 
-    max_degree = max(degrees.values())
+    max_degree = max(2, max(degrees.values()))
     root_cm = max_degree
+    node_cm = max_degree // 2
     src_cm = 0
     colormap = cm.get_cmap(cmap_name, max_degree + 1)
     colors = []
     labels = {}
 
     for node, data in graph.nodes(data=True):
         # Determine color of the node:
@@ -122,21 +142,23 @@
         # if node is source -- use special 'max' color
         # else use node color according to colormap and node degree
         if node in roots:
             color = colormap(root_cm)
         elif node in sources:
             color = colormap(src_cm)
         else:
-            color = colormap(graph.degree(node))
+            clr_id = graph.degree(node) if color_degrees else node_cm
+            color = colormap(clr_id)
         colors.append(color)
 
         # Get node label
         label = data.get('name') or str(node)
         labels[node] = label
 
     # Construct legend handles
     root_legend = mpatches.Patch(color=colormap(root_cm), label='Root')
-    degree_legend = mpatches.Patch(color=colormap(max_degree // 2 + 1), label='Node Degree')
+    default_legend = mpatches.Patch(color=colormap(node_cm),
+                                    label='Node Degree' if color_degrees else 'Intermediate')
     source_legend = mpatches.Patch(color=colormap(src_cm), label='Source')
-    handles = [root_legend, degree_legend, source_legend]
+    handles = [root_legend, default_legend, source_legend]
 
     return colors, labels, handles
```

### Comparing `thegolem-0.3.1/examples/viz_with_labels.py` & `thegolem-0.3.2/examples/viz_with_labels.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/adapter/adapt_registry.py` & `thegolem-0.3.2/golem/core/adapter/adapt_registry.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/adapter/adapter.py` & `thegolem-0.3.2/golem/core/adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/adapter/nx_adapter.py` & `thegolem-0.3.2/golem/core/adapter/nx_adapter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from copy import deepcopy
 from typing import Optional, Dict, Any, Iterable
 
 import networkx as nx
-import numpy as np
 
 from golem.core.adapter import BaseOptimizationAdapter
 from golem.core.dag.graph_node import GraphNode
 from golem.core.optimisers.graph import OptGraph, OptNode
 
 
 class BaseNetworkxAdapter(BaseOptimizationAdapter[nx.DiGraph]):
@@ -40,14 +39,15 @@
             for pred_id in adaptee.predecessors(node_id):
                 yield mapped_nodes[pred_id]
 
         # map nodes
         for node_id, node_data in adaptee.nodes.items():
             # transform node
             node = self._node_adapt(node_data)
+            node.uid = str(node_id)
             mapped_nodes[node_id] = node
 
         # map parent nodes
         for node_id, node in mapped_nodes.items():
             # append its parent edges
             node.nodes_from = map_predecessors(node_id)
 
@@ -81,7 +81,32 @@
     `OptNode` as an attribute of NetworkX graph node."""
 
     def _node_restore(self, node: GraphNode) -> Dict:
         return {_NX_NODE_KEY: node}
 
     def _node_adapt(self, data: Dict) -> OptNode:
         return data[_NX_NODE_KEY]
+
+
+class BanditNetworkxAdapter(BaseNetworkxAdapter):
+    """ Classic networkx adapter with nodes indexes in names instead of uids.
+    It is needed since some frameworks (e.g. karateclub) have asserts in which node
+    names should consist only of its indexes.
+    """
+    def _restore(self, opt_graph: OptGraph, metadata: Optional[Dict[str, Any]] = None) -> nx.DiGraph:
+        nx_graph = nx.DiGraph()
+        nx_node_data = {}
+
+        # add nodes
+        for node in opt_graph.nodes:
+            nx_node_data[node.uid] = self._node_restore(node)
+            nx_graph.add_node(opt_graph.nodes.index(node))
+
+        # add edges
+        for node in opt_graph.nodes:
+            for parent in node.nodes_from:
+                nx_graph.add_edge(opt_graph.nodes.index(parent), opt_graph.nodes.index(node))
+
+        # add nodes ad labels
+        nx.set_node_attributes(nx_graph, nx_node_data)
+
+        return nx_graph
```

### Comparing `thegolem-0.3.1/golem/core/dag/convert.py` & `thegolem-0.3.2/golem/core/dag/convert.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/dag/graph.py` & `thegolem-0.3.2/golem/core/dag/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,15 +242,18 @@
     @property
     def descriptive_id(self) -> str:
         """Returns human-readable identifier of the graph.
 
         Returns:
             str: text description of the content in the node and its parameters
         """
-        return self.root_node.descriptive_id
+        if self.root_nodes:
+            return self.root_node.descriptive_id
+        else:
+            return sorted(self.nodes, key=lambda x: x.uid)[0].descriptive_id
 
     def __str__(self):
         return str(self.graph_description)
 
     def __repr__(self):
         return self.__str__()
```

### Comparing `thegolem-0.3.1/golem/core/dag/graph_delegate.py` & `thegolem-0.3.2/golem/core/dag/graph_delegate.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/dag/graph_node.py` & `thegolem-0.3.2/golem/core/dag/graph_node.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/dag/graph_verifier.py` & `thegolem-0.3.2/golem/core/dag/graph_verifier.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/dag/linked_graph.py` & `thegolem-0.3.2/golem/core/dag/linked_graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from copy import deepcopy
 from typing import Any, Dict, List, Optional, Tuple, Union, Callable, Sequence
 
 from networkx import graph_edit_distance, set_node_attributes
 
+from golem.core.dag.convert import graph_structure_as_nx_graph
 from golem.core.dag.graph import Graph, ReconnectType
 from golem.core.dag.graph_node import GraphNode
-from golem.core.dag.graph_utils import ordered_subnodes_hierarchy, node_depth
-from golem.core.dag.convert import graph_structure_as_nx_graph
-from golem.core.utilities.data_structures import ensure_wrapped_in_sequence, Copyable, remove_items
+from golem.core.dag.graph_utils import ordered_subnodes_hierarchy, node_depth, graph_has_cycle
 from golem.core.paths import copy_doc
+from golem.core.utilities.data_structures import ensure_wrapped_in_sequence, Copyable, remove_items
 
 NodePostprocessCallable = Callable[[Graph, Sequence[GraphNode]], Any]
 
 
 class LinkedGraph(Graph, Copyable):
     """Graph implementation based on linked graph node
     that directly stores its parent nodes.
@@ -65,15 +65,15 @@
             subtree.nodes_from = remove_items(subtree.nodes_from, subtree_nodes)
 
     @copy_doc(Graph.update_node)
     def update_node(self, old_node: GraphNode, new_node: GraphNode):
         self.actualise_old_node_children(old_node, new_node)
         new_node.nodes_from.extend(old_node.nodes_from)
         self._nodes.remove(old_node)
-        self._nodes.append(new_node)
+        self.add_node(new_node)
         self.sort_nodes()
         self._postprocess_nodes(self, self._nodes)
 
     @copy_doc(Graph.update_subtree)
     def update_subtree(self, old_subtree: GraphNode, new_subtree: GraphNode):
         new_subtree = deepcopy(new_subtree)
         self.actualise_old_node_children(old_subtree, new_subtree)
@@ -97,15 +97,15 @@
         old_node_offspring = self.node_children(old_node)
         for old_node_child in old_node_offspring:
             updated_index = old_node_child.nodes_from.index(old_node)
             old_node_child.nodes_from[updated_index] = new_node
 
     def sort_nodes(self):
         """ Layer by layer sorting """
-        if not isinstance(self.root_node, Sequence):
+        if not isinstance(self.root_node, Sequence) and not graph_has_cycle(self):
             self._nodes = ordered_subnodes_hierarchy(self.root_node)
 
     @copy_doc(Graph.node_children)
     def node_children(self, node: GraphNode) -> List[Optional[GraphNode]]:
         """ Returns list of children of specified node. """
         return [other_node for other_node in self._nodes
                 if other_node.nodes_from and
@@ -158,20 +158,31 @@
         return \
             set(rn.descriptive_id for rn in self.root_nodes()) == \
             set(rn.descriptive_id for rn in other_graph.root_nodes())
 
     @copy_doc(Graph.descriptive_id)
     @property
     def descriptive_id(self) -> str:
-        return ''.join([r.descriptive_id for r in self.root_nodes()])
+        if self.length == 0:
+            return 'EMPTY'
+        elif self.root_nodes():
+            return ''.join([r.descriptive_id for r in self.root_nodes()])
+        else:
+            return sorted(self.nodes, key=lambda x: x.uid)[0].descriptive_id
 
     @copy_doc(Graph.depth)
     @property
     def depth(self) -> int:
-        return 0 if not self._nodes else max(map(node_depth, self.root_nodes()))
+        if not self._nodes:
+            return 0
+        elif not self.root_nodes() or graph_has_cycle(self):
+            return -1
+        else:
+            depths = node_depth(self.root_nodes())
+            return max(ensure_wrapped_in_sequence(depths))
 
     @copy_doc(Graph.get_edges)
     def get_edges(self) -> Sequence[Tuple[GraphNode, GraphNode]]:
         edges = []
         for node in self._nodes:
             if node.nodes_from:
                 for parent_node in node.nodes_from:
```

### Comparing `thegolem-0.3.1/golem/core/dag/linked_graph_node.py` & `thegolem-0.3.2/golem/core/dag/linked_graph_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from typing import Union, Optional, Iterable, List, Hashable
-from uuid import uuid4
-
+from typing import Union, Optional, Iterable, List
 from golem.core.dag.graph_node import GraphNode
 from golem.core.utilities.data_structures import UniqueList
 
 
 class LinkedGraphNode(GraphNode):
     """Class for node definition in the directed graph structure
     that directly stores its parent nodes.
```

### Comparing `thegolem-0.3.1/golem/core/dag/verification_rules.py` & `thegolem-0.3.2/golem/core/dag/verification_rules.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import networkx as nx
-from networkx import isolates, simple_cycles
+from networkx import isolates
 
 from golem.core.adapter import register_native
 from golem.core.dag.convert import graph_structure_as_nx_graph
 from golem.core.dag.graph import Graph
 from golem.core.dag.graph_node import GraphNode
+from golem.core.dag.graph_utils import graph_has_cycle
 
 ERROR_PREFIX = 'Invalid graph configuration:'
 
 
 @register_native
 def has_root(graph: Graph):
     if graph.root_node:
@@ -19,17 +20,15 @@
 def has_one_root(graph: Graph):
     if isinstance(graph.root_node, GraphNode):
         return True
 
 
 @register_native
 def has_no_cycle(graph: Graph):
-    nx_graph, _ = graph_structure_as_nx_graph(graph)
-    cycled = list(simple_cycles(nx_graph))
-    if len(cycled) > 0:
+    if graph_has_cycle(graph):
         raise ValueError(f'{ERROR_PREFIX} Graph has cycles')
 
     return True
 
 
 @register_native
 def has_no_isolated_nodes(graph: Graph):
```

### Comparing `thegolem-0.3.1/golem/core/log.py` & `thegolem-0.3.2/golem/core/log.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/optimisers/advisor.py` & `thegolem-0.3.2/golem/core/optimisers/advisor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,32 @@
-from typing import List, Any
+from typing import List, Any, TypeVar, Generic
 
-from golem.core.optimisers.graph import OptNode
 from golem.core.utilities.data_structures import ComparableEnum as Enum
 
+NodeType = TypeVar('NodeType')
+
 
 class RemoveType(Enum):
     """Defines allowed kinds of removals in Graph. Used by mutations."""
     forbidden = 'forbidden'
     node_only = 'node_only'
     node_rewire = 'node_rewire'
     with_direct_children = 'with_direct_children'
     with_parents = 'with_parents'
 
 
-class DefaultChangeAdvisor:
+class DefaultChangeAdvisor(Generic[NodeType]):
     """
     Class for advising of graph changes during evolution
     """
 
     def __init__(self, task=None):
         self.task = task
 
-    def propose_change(self, node: OptNode, possible_operations: List[Any]) -> List[Any]:
+    def propose_change(self, node: NodeType, possible_operations: List[Any]) -> List[Any]:
         return possible_operations
 
-    def can_be_removed(self, node: OptNode) -> RemoveType:
+    def can_be_removed(self, node: NodeType) -> RemoveType:
         return RemoveType.node_rewire
 
-    def propose_parent(self, node: OptNode, possible_operations: List[Any]) -> List[Any]:
+    def propose_parent(self, node: NodeType, possible_operations: List[Any]) -> List[Any]:
         return possible_operations
```

### Comparing `thegolem-0.3.1/golem/core/optimisers/archive/generation_keeper.py` & `thegolem-0.3.2/golem/core/optimisers/archive/generation_keeper.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/optimisers/archive/individuals_containers.py` & `thegolem-0.3.2/golem/core/optimisers/archive/individuals_containers.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/optimisers/fitness/fitness.py` & `thegolem-0.3.2/golem/core/optimisers/fitness/fitness.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/optimisers/fitness/multi_objective_fitness.py` & `thegolem-0.3.2/golem/core/optimisers/fitness/multi_objective_fitness.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/optimisers/genetic/evaluation.py` & `thegolem-0.3.2/golem/core/optimisers/genetic/evaluation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import gc
 import logging
 import pathlib
 import timeit
 from abc import ABC, abstractmethod
 from datetime import datetime
 from functools import partial
-from random import choice
-from typing import Dict, List, Optional, Sequence, Tuple, TypeVar
+from typing import List, Optional, Sequence, Tuple, TypeVar, Dict
 
 from joblib import Parallel, cpu_count, delayed
 
 from golem.core.adapter import BaseOptimizationAdapter
 from golem.core.dag.graph import Graph
 from golem.core.log import default_log, Log
 from golem.core.optimisers.fitness import Fitness
@@ -29,14 +28,15 @@
 OptionalEvalResult = Optional[GraphEvalResult]
 EvalResultsList = List[OptionalEvalResult]
 G = TypeVar('G', bound=Serializable)
 
 
 class DelegateEvaluator:
     """Interface for delegate evaluator of graphs."""
+
     @property
     @abstractmethod
     def is_enabled(self) -> bool:
         return False
 
     @abstractmethod
     def compute_graphs(self, graphs: Sequence[G]) -> Sequence[G]:
@@ -123,14 +123,15 @@
         self._post_eval_callback = None
         self._delegate_evaluator = delegate_evaluator
 
         self.timer = None
         self.logger = default_log(self)
         self._n_jobs = n_jobs
         self.evaluation_cache = None
+        self._reset_eval_cache()
 
     def dispatch(self, objective: ObjectiveFunction, timer: Optional[Timer] = None) -> EvaluationOperator:
         """Return handler to this object that hides all details
         and allows only to evaluate population with provided objective."""
         self._objective_eval = objective
         self.timer = timer or get_forever_timer()
         return self.evaluate_population
@@ -138,29 +139,33 @@
     def set_graph_evaluation_callback(self, callback: Optional[GraphFunction]):
         self._post_eval_callback = callback
 
     def population_evaluation_info(self, pop_size: int, evaluated_pop_size: int):
         """ Shows the amount of successfully evaluated individuals and total number of individuals in population.
          If there are more that 50% of successful evaluations than it's more likely
          there is no problem in optimization process. """
-        if evaluated_pop_size / pop_size > STAGNATION_EVALUATION_PERCENTAGE:
-            self.logger.message(f"{evaluated_pop_size} individuals out of {pop_size} in previous population "
-                                f"were evaluated successfully.")
-        else:
+        if pop_size == 0 or evaluated_pop_size / pop_size <= STAGNATION_EVALUATION_PERCENTAGE:
+            success_rate = evaluated_pop_size / pop_size if pop_size != 0 else 0
             self.logger.warning(f"{evaluated_pop_size} individuals out of {pop_size} in previous population "
-                                f"were evaluated successfully. {evaluated_pop_size / pop_size}% "
+                                f"were evaluated successfully. {success_rate}% "
                                 f"is a fairly small percentage of successful evaluation.")
+        else:
+            self.logger.message(f"{evaluated_pop_size} individuals out of {pop_size} in previous population "
+                                f"were evaluated successfully.")
 
     @abstractmethod
     def evaluate_population(self, individuals: PopulationT) -> Optional[PopulationT]:
         raise NotImplementedError()
 
-    def evaluate_single(self, graph: OptGraph, uid_of_individual: str, with_time_limit: bool = True, cache_key: Optional[str] = None,
+    def evaluate_single(self, graph: OptGraph, uid_of_individual: str, with_time_limit: bool = True,
+                        cache_key: Optional[str] = None,
                         logs_initializer: Optional[Tuple[int, pathlib.Path]] = None) -> OptionalEvalResult:
 
+        graph = self.evaluation_cache.get(cache_key, graph)
+
         if with_time_limit and self.timer.is_time_limit_reached():
             return None
         if logs_initializer is not None:
             # in case of multiprocessing run
             Log.setup_in_mp(*logs_initializer)
 
         adapted_evaluate = self._adapter.adapt_func(self._evaluate_graph)
@@ -184,14 +189,32 @@
             self._post_eval_callback(domain_graph)
         if self._cleanup:
             self._cleanup(domain_graph)
         gc.collect()
 
         return fitness, domain_graph
 
+    def evaluate_with_cache(self, population: PopulationT) -> Optional[PopulationT]:
+        reversed_population = list(reversed(population))
+        self._remote_compute_cache(reversed_population)
+        evaluated_population = self.evaluate_population(reversed_population)
+        self._reset_eval_cache()
+        return evaluated_population
+
+    def _reset_eval_cache(self):
+        self.evaluation_cache: Dict[str, Graph] = {}
+
+    def _remote_compute_cache(self, population: PopulationT):
+        self._reset_eval_cache()
+        if self._delegate_evaluator and self._delegate_evaluator.is_enabled:
+            self.logger.info('Remote fit used')
+            restored_graphs = self._adapter.restore(population)
+            computed_graphs = self._delegate_evaluator.compute_graphs(restored_graphs)
+            self.evaluation_cache = {ind.uid: graph for ind, graph in zip(population, computed_graphs)}
+
 
 class MultiprocessingDispatcher(BaseGraphEvaluationDispatcher):
     """Evaluates objective function on population using multiprocessing pool
     and optionally model evaluation cache with RemoteEvaluator.
 
     Usage: call `dispatch(objective_function)` to get evaluation function.
 
@@ -206,29 +229,20 @@
                  adapter: BaseOptimizationAdapter,
                  n_jobs: int = 1,
                  graph_cleanup_fn: Optional[GraphFunction] = None,
                  delegate_evaluator: Optional[DelegateEvaluator] = None):
 
         super().__init__(adapter, n_jobs, graph_cleanup_fn, delegate_evaluator)
 
-        self._reset_eval_cache()
-
     def dispatch(self, objective: ObjectiveFunction, timer: Optional[Timer] = None) -> EvaluationOperator:
         """Return handler to this object that hides all details
         and allows only to evaluate population with provided objective."""
         super().dispatch(objective, timer)
         return self.evaluate_with_cache
 
-    def evaluate_with_cache(self, population: PopulationT) -> Optional[PopulationT]:
-        reversed_population = list(reversed(population))
-        self._remote_compute_cache(reversed_population)
-        evaluated_population = self.evaluate_population(reversed_population)
-        self._reset_eval_cache()
-        return evaluated_population
-
     def evaluate_population(self, individuals: PopulationT) -> Optional[PopulationT]:
         individuals_to_evaluate, individuals_to_skip = self.split_individuals_to_evaluate(individuals)
         # Evaluate individuals without valid fitness in parallel.
         n_jobs = determine_n_jobs(self._n_jobs, self.logger)
 
         parallel = Parallel(n_jobs=n_jobs, verbose=0, pre_dispatch="2*n_jobs")
         eval_func = partial(self.evaluate_single, logs_initializer=Log().get_parameters())
@@ -246,33 +260,14 @@
                 if successful_evals:
                     break
         MemoryAnalytics.log(self.logger,
                             additional_info='parallel evaluation of population',
                             logging_level=logging.INFO)
         return successful_evals
 
-    def evaluate_single(self, graph: OptGraph, uid_of_individual: str, with_time_limit: bool = True,
-                        cache_key: Optional[str] = None,
-                        logs_initializer: Optional[Tuple[int, pathlib.Path]] = None) -> OptionalEvalResult:
-
-        graph = self.evaluation_cache.get(cache_key, graph)
-        eval_res = super().evaluate_single(graph, uid_of_individual, with_time_limit, cache_key, logs_initializer)
-        return eval_res
-
-    def _reset_eval_cache(self):
-        self.evaluation_cache: Dict[str, Graph] = {}
-
-    def _remote_compute_cache(self, population: PopulationT):
-        self._reset_eval_cache()
-        if self._delegate_evaluator and self._delegate_evaluator.is_enabled:
-            self.logger.info('Remote fit used')
-            restored_graphs = self._adapter.restore(population)
-            computed_graphs = self._delegate_evaluator.compute_graphs(restored_graphs)
-            self.evaluation_cache = {ind.uid: graph for ind, graph in zip(population, computed_graphs)}
-
 
 class SequentialDispatcher(BaseGraphEvaluationDispatcher):
     """Evaluates objective function on population in sequential way.
 
         Usage: call `dispatch(objective_function)` to get evaluation function.
     """
```

### Comparing `thegolem-0.3.1/golem/core/optimisers/genetic/gp_operators.py` & `thegolem-0.3.2/golem/core/optimisers/genetic/gp_operators.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/optimisers/genetic/gp_optimizer.py` & `thegolem-0.3.2/golem/core/optimisers/genetic/gp_optimizer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 from copy import deepcopy
 from random import choice
-from typing import Sequence, Callable, Union, Any
+from typing import Sequence, Union, Any
 
 from golem.core.constants import MAX_GRAPH_GEN_ATTEMPTS
 from golem.core.dag.graph import Graph
 from golem.core.optimisers.genetic.gp_params import GPAlgorithmParameters
 from golem.core.optimisers.genetic.operators.crossover import Crossover
 from golem.core.optimisers.genetic.operators.elitism import Elitism
 from golem.core.optimisers.genetic.operators.inheritance import Inheritance
 from golem.core.optimisers.genetic.operators.mutation import Mutation
 from golem.core.optimisers.genetic.operators.operator import PopulationT, EvaluationOperator
 from golem.core.optimisers.genetic.operators.regularization import Regularization
+from golem.core.optimisers.genetic.operators.reproduction import ReproductionController
 from golem.core.optimisers.genetic.operators.selection import Selection
 from golem.core.optimisers.genetic.parameters.graph_depth import AdaptiveGraphDepth
 from golem.core.optimisers.genetic.parameters.operators_prob import init_adaptive_operators_prob
 from golem.core.optimisers.genetic.parameters.population_size import init_adaptive_pop_size, PopulationSize
-from golem.core.optimisers.optimization_parameters import GraphRequirements
 from golem.core.optimisers.objective.objective import Objective
 from golem.core.optimisers.opt_history_objects.individual import Individual
+from golem.core.optimisers.optimization_parameters import GraphRequirements
 from golem.core.optimisers.optimizer import GraphGenerationParams
-from golem.core.optimisers.populational_optimizer import PopulationalOptimizer, EvaluationAttemptsError
-
-
-EVALUATION_ATTEMPTS_NUMBER = 5
+from golem.core.optimisers.populational_optimizer import PopulationalOptimizer
 
 
 class EvoGraphOptimizer(PopulationalOptimizer):
     """
     Multi-objective evolutionary graph optimizer named GPComp
     """
 
@@ -42,14 +40,15 @@
         self.selection = Selection(graph_optimizer_params)
         self.crossover = Crossover(graph_optimizer_params, requirements, graph_generation_params)
         self.mutation = Mutation(graph_optimizer_params, requirements, graph_generation_params)
         self.inheritance = Inheritance(graph_optimizer_params, self.selection)
         self.elitism = Elitism(graph_optimizer_params)
         self.operators = [self.regularization, self.selection, self.crossover,
                           self.mutation, self.inheritance, self.elitism]
+        self.reproducer = ReproductionController(graph_optimizer_params, self.selection, self.mutation, self.crossover)
 
         # Define adaptive parameters
         self._pop_size: PopulationSize = init_adaptive_pop_size(graph_optimizer_params, self.generations)
         self._operators_prob = init_adaptive_operators_prob(graph_optimizer_params)
         self._graph_depth = AdaptiveGraphDepth(self.generations,
                                                start_depth=requirements.start_depth,
                                                max_depth=requirements.max_depth,
@@ -62,50 +61,67 @@
         self.initial_individuals = [Individual(graph, metadata=requirements.static_individual_metadata)
                                     for graph in self.initial_graphs]
 
     def _initial_population(self, evaluator: EvaluationOperator):
         """ Initializes the initial population """
         # Adding of initial assumptions to history as zero generation
         self._update_population(evaluator(self.initial_individuals), 'initial_assumptions')
+        pop_size = self.graph_optimizer_params.pop_size
 
-        if len(self.initial_individuals) < self.graph_optimizer_params.pop_size:
-            self.initial_individuals = self._extend_population(self.initial_individuals)
+        if len(self.initial_individuals) < pop_size:
+            self.initial_individuals = self._extend_population(self.initial_individuals, pop_size)
             # Adding of extended population to history
             self._update_population(evaluator(self.initial_individuals), 'extended_initial_assumptions')
 
-    def _extend_population(self, initial_individuals: PopulationT) -> PopulationT:
-        initial_individuals = list(initial_individuals)
-        initial_graphs = [ind.graph for ind in initial_individuals]
+    def _extend_population(self, pop: PopulationT, target_pop_size: int) -> PopulationT:
+        verifier = self.graph_generation_params.verifier
+        extended_pop = list(pop)
+        pop_graphs = [ind.graph for ind in extended_pop]
+
+        # Set mutation probabilities to 1.0
         initial_req = deepcopy(self.requirements)
-        initial_req.mutation_prob = 1
+        initial_req.mutation_prob = 1.0
         self.mutation.update_requirements(requirements=initial_req)
 
         for iter_num in range(MAX_GRAPH_GEN_ATTEMPTS):
-            if len(initial_individuals) == self.graph_optimizer_params.pop_size:
+            if len(extended_pop) == target_pop_size:
                 break
-            new_ind = self.mutation(choice(self.initial_individuals))
-            new_graph = new_ind.graph
-            if new_graph not in initial_graphs and self.graph_generation_params.verifier(new_graph):
-                initial_individuals.append(new_ind)
-                initial_graphs.append(new_graph)
+            new_ind = self.mutation(choice(pop))
+            if new_ind:
+                new_graph = new_ind.graph
+                if new_graph not in pop_graphs and verifier(new_graph):
+                    extended_pop.append(new_ind)
+                    pop_graphs.append(new_graph)
         else:
             self.log.warning(f'Exceeded max number of attempts for extending initial graphs, stopping.'
-                             f'Current size {len(self.initial_individuals)} '
-                             f'instead of {self.graph_optimizer_params.pop_size} graphs.')
+                             f'Current size {len(pop)}, required {target_pop_size} graphs.')
 
+        # Reset mutation probabilities to default
         self.mutation.update_requirements(requirements=self.requirements)
-        return initial_individuals
+        return extended_pop
 
     def _evolve_population(self, evaluator: EvaluationOperator) -> PopulationT:
         """ Method realizing full evolution cycle """
+
+        # Defines adaptive changes to algorithm parameters
+        #  like pop_size and operator probabilities
         self._update_requirements()
 
+        # Regularize previous population
         individuals_to_select = self.regularization(self.population, evaluator)
-        selected_individuals = self.selection(individuals_to_select)
-        new_population = self._spawn_evaluated_population(selected_individuals, evaluator)
+        # Reproduce from previous pop to get next population
+        new_population = self.reproducer.reproduce(individuals_to_select, evaluator)
+
+        # Adaptive agent experience collection & learning
+        # Must be called after reproduction (that collects the new experience)
+        experience = self.mutation.agent_experience
+        experience.collect_results(new_population)
+        self.mutation.agent.partial_fit(experience)
+
+        # Use some part of previous pop in the next pop
         new_population = self.inheritance(self.population, new_population)
         new_population = self.elitism(self.generations.best_individuals, new_population)
 
         return new_population
 
     def _update_requirements(self):
         if not self.generations.is_any_improved:
@@ -116,21 +132,7 @@
         self.log.info(
             f'Next population size: {self.graph_optimizer_params.pop_size}; '
             f'max graph depth: {self.requirements.max_depth}')
 
         # update requirements in operators
         for operator in self.operators:
             operator.update_requirements(self.graph_optimizer_params, self.requirements)
-
-    def _spawn_evaluated_population(self, selected_individuals: PopulationT, evaluator: Callable) -> PopulationT:
-        """ Reproduce and evaluate new population. If at least one of received individuals can not be evaluated then
-        mutate and evaluate selected individuals until a new population is obtained
-        or the number of attempts is exceeded """
-        for i in range(EVALUATION_ATTEMPTS_NUMBER):
-            new_population = self.crossover(selected_individuals)
-            new_population = self.mutation(new_population)
-            new_population = evaluator(new_population)
-            if new_population:
-                return new_population
-        else:
-            # Could not generate valid population; raise an error
-            raise EvaluationAttemptsError()
```

### Comparing `thegolem-0.3.1/golem/core/optimisers/genetic/operators/base_mutations.py` & `thegolem-0.3.2/golem/core/optimisers/genetic/operators/base_mutations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from copy import deepcopy
 from functools import partial
 from random import choice, randint, random, sample
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
 from golem.core.adapter import register_native
 from golem.core.dag.graph import ReconnectType
 from golem.core.dag.graph_node import GraphNode
-from golem.core.dag.graph_utils import distance_to_root_level, ordered_subnodes_hierarchy, distance_to_primary_level
+from golem.core.dag.graph_utils import distance_to_root_level, distance_to_primary_level, graph_has_cycle
 from golem.core.optimisers.advisor import RemoveType
 from golem.core.optimisers.graph import OptGraph, OptNode
 from golem.core.optimisers.opt_node_factory import OptNodeFactory
 from golem.core.optimisers.optimization_parameters import GraphRequirements
 from golem.core.optimisers.optimizer import GraphGenerationParams, AlgorithmParameters
 from golem.core.utilities.data_structures import ComparableEnum as Enum
 
@@ -26,44 +25,46 @@
 
 class MutationTypesEnum(Enum):
     simple = 'simple'
     growth = 'growth'
     local_growth = 'local_growth'
     tree_growth = 'tree_growth'
     reduce = 'reduce'
-    single_add = 'single_add',
-    single_change = 'single_change',
-    single_drop = 'single_drop',
+    single_add = 'single_add'
+    single_change = 'single_change'
+    single_drop = 'single_drop'
     single_edge = 'single_edge'
 
     none = 'none'
 
 
-def get_mutation_prob(mut_id: MutationStrengthEnum, node: GraphNode,
+def get_mutation_prob(mut_id: MutationStrengthEnum, node: Optional[GraphNode],
                       default_mutation_prob: float = 0.7) -> float:
     """ Function returns mutation probability for certain node in the graph
 
     :param mut_id: MutationStrengthEnum mean weak or strong mutation
     :param node: root node of the graph
-    :param default_mutation_prob: mutation probability used when mutation_id is invalid
+    :param default_mutation_prob: mutation probability used when mutation_id is invalid or graph has cycles
     :return mutation_prob: mutation probability
     """
-    if mut_id in list(MutationStrengthEnum):
+    mutation_prob = default_mutation_prob
+    graph_cycled = node is None
+    if node:
+        graph_cycled = distance_to_primary_level(node) < 0
+    if mut_id in list(MutationStrengthEnum) and not graph_cycled:
         mutation_strength = mut_id.value
         mutation_prob = mutation_strength / (distance_to_primary_level(node) + 1)
-    else:
-        mutation_prob = default_mutation_prob
     return mutation_prob
 
 
 @register_native
 def simple_mutation(graph: OptGraph,
                     requirements: GraphRequirements,
                     graph_gen_params: GraphGenerationParams,
-                    parameters: 'GPAlgorithmParameters',
+                    parameters: 'GPAlgorithmParameters'
                     ) -> OptGraph:
     """
     This type of mutation is passed over all nodes of the tree started from the root node and changes
     nodes’ operations with probability - 'node mutation probability'
     which is initialised inside the function
 
     :param graph: graph to mutate
@@ -80,49 +81,62 @@
             # removed node must not be visited because it's outdated
             visited_nodes.add(node)
             # new node must not mutated if encountered further during traverse
             visited_nodes.add(new_node)
             for parent in node.nodes_from:
                 replace_node_to_random_recursive(parent)
 
+    root_nodes = graph.root_nodes()
+    root_node = choice(root_nodes) if root_nodes else None
     node_mutation_probability = get_mutation_prob(mut_id=parameters.mutation_strength,
-                                                  node=graph.root_node)
+                                                  node=root_node)
 
-    replace_node_to_random_recursive(graph.root_node)
+    root_node = root_node or choice(graph.nodes)
+    replace_node_to_random_recursive(root_node)
 
     return graph
 
 
 @register_native
 def single_edge_mutation(graph: OptGraph,
                          requirements: GraphRequirements,
                          graph_gen_params: GraphGenerationParams,
-                         parameters: 'GPAlgorithmParameters',
+                         parameters: 'GPAlgorithmParameters'
                          ) -> OptGraph:
     """
     This mutation adds new edge between two random nodes in graph.
 
     :param graph: graph to mutate
     """
-    old_graph = deepcopy(graph)
+
+    def nodes_not_cycling(source_node: OptNode, target_node: OptNode):
+        parents = source_node.nodes_from
+        while parents:
+            if target_node not in parents:
+                grandparents = []
+                for parent in parents:
+                    grandparents.extend(parent.nodes_from)
+                parents = grandparents
+            else:
+                return False
+        return True
 
     for _ in range(parameters.max_num_of_operator_attempts):
         if len(graph.nodes) < 2 or graph.depth > requirements.max_depth:
             return graph
 
         source_node, target_node = sample(graph.nodes, 2)
-
-        nodes_not_cycling = (target_node.descriptive_id not in
-                             [n.descriptive_id for n in ordered_subnodes_hierarchy(source_node)])
-        if nodes_not_cycling and (source_node not in target_node.nodes_from):
-            graph.connect_nodes(source_node, target_node)
-            break
-
-    if graph.depth > requirements.max_depth:
-        return old_graph
+        if source_node not in target_node.nodes_from:
+            if graph_has_cycle(graph):
+                graph.connect_nodes(source_node, target_node)
+                break
+            else:
+                if nodes_not_cycling(source_node, target_node):
+                    graph.connect_nodes(source_node, target_node)
+                    break
     return graph
 
 
 @register_native
 def add_intermediate_node(graph: OptGraph,
                           node_to_mutate: OptNode,
                           node_factory: OptNodeFactory) -> OptGraph:
@@ -178,15 +192,15 @@
     return graph
 
 
 @register_native
 def single_add_mutation(graph: OptGraph,
                         requirements: GraphRequirements,
                         graph_gen_params: GraphGenerationParams,
-                        parameters: AlgorithmParameters,
+                        parameters: AlgorithmParameters
                         ) -> OptGraph:
     """
     Add new node between two sequential existing modes
 
     :param graph: graph to mutate
     """
 
@@ -205,15 +219,15 @@
     return result
 
 
 @register_native
 def single_change_mutation(graph: OptGraph,
                            requirements: GraphRequirements,
                            graph_gen_params: GraphGenerationParams,
-                           parameters: AlgorithmParameters,
+                           parameters: AlgorithmParameters
                            ) -> OptGraph:
     """
     Change node between two sequential existing modes.
 
     :param graph: graph to mutate
     """
     node = choice(graph.nodes)
@@ -224,15 +238,15 @@
     return graph
 
 
 @register_native
 def single_drop_mutation(graph: OptGraph,
                          requirements: GraphRequirements,
                          graph_gen_params: GraphGenerationParams,
-                         parameters: AlgorithmParameters,
+                         parameters: AlgorithmParameters
                          ) -> OptGraph:
     """
     Drop single node from graph.
 
     :param graph: graph to mutate
     """
     if len(graph.nodes) < 2:
@@ -241,16 +255,15 @@
     node_name = node_to_del.name
     removal_type = graph_gen_params.advisor.can_be_removed(node_to_del)
     if removal_type == RemoveType.with_direct_children:
         # TODO refactor workaround with data_source
         graph.delete_node(node_to_del)
         nodes_to_delete = \
             [n for n in graph.nodes
-             if n.descriptive_id.count('data_source') == 1
-             and node_name in n.descriptive_id]
+             if n.descriptive_id.count('data_source') == 1 and node_name in n.descriptive_id]
         for child_node in nodes_to_delete:
             graph.delete_node(child_node, reconnect=ReconnectType.all)
     elif removal_type == RemoveType.with_parents:
         graph.delete_subtree(node_to_del)
     elif removal_type == RemoveType.node_rewire:
         graph.delete_node(node_to_del, reconnect=ReconnectType.all)
     elif removal_type == RemoveType.node_only:
@@ -364,26 +377,24 @@
     MutationTypesEnum.reduce: reduce_mutation,
     MutationTypesEnum.single_add: single_add_mutation,
     MutationTypesEnum.single_edge: single_edge_mutation,
     MutationTypesEnum.single_drop: single_drop_mutation,
     MutationTypesEnum.single_change: single_change_mutation,
 }
 
-
 simple_mutation_set = (
     MutationTypesEnum.tree_growth,
     MutationTypesEnum.single_add,
     MutationTypesEnum.single_change,
     MutationTypesEnum.single_drop,
     MutationTypesEnum.single_edge,
     # join nodes
     # flip edge
     # cycle edge
 )
 
-
 rich_mutation_set = (
     MutationTypesEnum.simple,
     MutationTypesEnum.reduce,
     MutationTypesEnum.growth,
     MutationTypesEnum.local_growth
 )
```

### Comparing `thegolem-0.3.1/golem/core/optimisers/genetic/operators/crossover.py` & `thegolem-0.3.2/golem/core/optimisers/genetic/operators/crossover.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from copy import deepcopy
-from random import choice, random, sample
-from math import ceil
 from itertools import chain
+from math import ceil
+from random import choice, random, sample
 from typing import Callable, Union, Iterable, Tuple, TYPE_CHECKING
 
 from golem.core.adapter import register_native
-from golem.core.dag.graph_node import GraphNode
 from golem.core.dag.graph_utils import nodes_from_layer, node_depth
 from golem.core.optimisers.genetic.gp_operators import equivalent_subtree, replace_subtrees
 from golem.core.optimisers.genetic.operators.operator import PopulationT, Operator
-from golem.core.optimisers.optimization_parameters import GraphRequirements
-from golem.core.optimisers.graph import OptGraph
+from golem.core.optimisers.graph import OptGraph, OptNode
 from golem.core.optimisers.opt_history_objects.individual import Individual
 from golem.core.optimisers.opt_history_objects.parent_operator import ParentOperator
+from golem.core.optimisers.optimization_parameters import GraphRequirements
 from golem.core.optimisers.optimizer import GraphGenerationParams
 from golem.core.utilities.data_structures import ComparableEnum as Enum
 
 if TYPE_CHECKING:
     from golem.core.optimisers.genetic.gp_params import GPAlgorithmParameters
 
 
@@ -157,21 +156,21 @@
     def find_edges_in_other_graph(edges, graph: OptGraph):
         new_edges = []
         for parent, child in edges:
             parent_new = graph.get_nodes_by_name(str(parent))
             if parent_new:
                 parent_new = parent_new[0]
             else:
-                parent_new = GraphNode(str(parent))
+                parent_new = OptNode(str(parent))
                 graph.add_node(parent_new)
             child_new = graph.get_nodes_by_name(str(child))
             if child_new:
                 child_new = child_new[0]
             else:
-                child_new = GraphNode(str(child))
+                child_new = OptNode(str(child))
                 graph.add_node(child_new)
             new_edges.append((parent_new, child_new))
         return new_edges
 
     edges_1 = graph_first.get_edges()
     edges_2 = graph_second.get_edges()
     count = ceil(min(len(edges_1), len(edges_2)) / 2)
@@ -208,15 +207,15 @@
     def find_nodes_in_other_graph(nodes, graph: OptGraph):
         new_nodes = []
         for node in nodes:
             new_node = graph.get_nodes_by_name(str(node))
             if new_node:
                 new_node = new_node[0]
             else:
-                new_node = GraphNode(str(node))
+                new_node = OptNode(str(node))
                 graph.add_node(new_node)
             new_nodes.append(new_node)
         return new_nodes
 
     edges = graph_second.get_edges()
     nodes_with_parent_or_child = list(set(chain(*edges)))
     if nodes_with_parent_or_child:
@@ -250,15 +249,15 @@
     def find_nodes_in_other_graph(nodes, graph: OptGraph):
         new_nodes = []
         for node in nodes:
             new_node = graph.get_nodes_by_name(str(node))
             if new_node:
                 new_node = new_node[0]
             else:
-                new_node = GraphNode(str(node))
+                new_node = OptNode(str(node))
                 graph.add_node(new_node)
             new_nodes.append(new_node)
         return new_nodes
 
     edges = graph_second.get_edges()
     nodes_with_parent_or_child = list(set(chain(*edges)))
     if nodes_with_parent_or_child:
```

### Comparing `thegolem-0.3.1/golem/core/optimisers/genetic/operators/elitism.py` & `thegolem-0.3.2/golem/core/optimisers/genetic/operators/elitism.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from random import shuffle
-from typing import TYPE_CHECKING
 
 from golem.core.optimisers.genetic.operators.operator import PopulationT, Operator
 from golem.core.utilities.data_structures import ComparableEnum as Enum
 
 
 class ElitismTypesEnum(Enum):
     keep_n_best = 'keep_n_best'
@@ -13,28 +12,35 @@
 
 class Elitism(Operator):
     def __call__(self, best_individuals: PopulationT, new_population: PopulationT) -> PopulationT:
         elitism_type = self.parameters.elitism_type
         if elitism_type is ElitismTypesEnum.none or not self._is_elitism_applicable():
             return new_population
         elif elitism_type is ElitismTypesEnum.keep_n_best:
-            return self._keep_n_best_elitism(best_individuals, new_population)
+            return self.keep_n_best_elitism(best_individuals, new_population)
         elif elitism_type is ElitismTypesEnum.replace_worst:
-            return self._replace_worst_elitism(best_individuals, new_population)
+            return self.replace_worst_elitism(best_individuals, new_population)
         else:
             raise ValueError(f'Required elitism type not found: {elitism_type}')
 
     def _is_elitism_applicable(self) -> bool:
         if self.parameters.multi_objective:
             return False
         return self.parameters.pop_size >= self.parameters.min_pop_size_with_elitism
 
-    def _keep_n_best_elitism(self, best_individuals: PopulationT, new_population: PopulationT) -> PopulationT:
-        shuffle(new_population)
-        new_population[:len(best_individuals)] = best_individuals
-        return new_population
+    @staticmethod
+    def keep_n_best_elitism(best_individuals: PopulationT, new_population: PopulationT) -> PopulationT:
+        final_population = []
+        final_population += best_individuals
+        new_unique_inds = [ind for ind in new_population if ind not in best_individuals]
+        if new_unique_inds:
+            shuffle(new_unique_inds)
+            remain_n = len(new_population) - len(best_individuals)
+            final_population += new_unique_inds[:remain_n]
+        return final_population
 
-    def _replace_worst_elitism(self, best_individuals: PopulationT, new_population: PopulationT) -> PopulationT:
+    @staticmethod
+    def replace_worst_elitism(best_individuals: PopulationT, new_population: PopulationT) -> PopulationT:
         population = best_individuals + new_population
         # sort in descending order (Fitness(10) > Fitness(11))
         sorted_ascending_population = sorted(population, key=lambda individual: individual.fitness, reverse=True)
         return sorted_ascending_population[:len(new_population)]
```

### Comparing `thegolem-0.3.1/golem/core/optimisers/genetic/operators/inheritance.py` & `thegolem-0.3.2/golem/core/optimisers/genetic/operators/inheritance.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from functools import partial
-from typing import (Callable, TYPE_CHECKING)
+from typing import TYPE_CHECKING
 
 from golem.core.optimisers.genetic.operators.operator import PopulationT, Operator
 from golem.core.optimisers.genetic.operators.selection import Selection
 from golem.core.utilities.data_structures import ComparableEnum as Enum
 
 if TYPE_CHECKING:
     from golem.core.optimisers.genetic.gp_params import GPAlgorithmParameters
@@ -12,36 +11,38 @@
 class GeneticSchemeTypesEnum(Enum):
     steady_state = 'steady_state'
     generational = 'generational'
     parameter_free = 'parameter_free'
 
 
 class Inheritance(Operator):
-    def __init__(self, parameters: 'GPAlgorithmParameters',
-                 selection: Selection):
+    def __init__(self, parameters: 'GPAlgorithmParameters', selection: Selection):
         super().__init__(parameters=parameters)
         self.selection = selection
 
     def __call__(self, previous_population: PopulationT, new_population: PopulationT) -> PopulationT:
-        return self._inheritance_type_by_genetic_scheme(previous_population, new_population)()
+        gp_scheme = self.parameters.genetic_scheme_type
+        if gp_scheme == GeneticSchemeTypesEnum.generational:
+            # Previous population is completely substituted
+            next_population = self.direct_inheritance(new_population)
+        elif gp_scheme == GeneticSchemeTypesEnum.steady_state:
+            # Previous population is mixed with new one
+            next_population = self.steady_state_inheritance(previous_population, new_population)
+        elif gp_scheme == GeneticSchemeTypesEnum.parameter_free:
+            # Same as steady-state
+            next_population = self.steady_state_inheritance(previous_population, new_population)
+        else:
+            raise ValueError(f'Unknown genetic scheme {gp_scheme}!')
+        return next_population
+
+    def steady_state_inheritance(self,
+                                 prev_population: PopulationT,
+                                 new_population: PopulationT
+                                 ) -> PopulationT:
+        # use individuals with non-repetitive uid
+        not_repetitive_inds = [ind for ind in prev_population if ind not in new_population]
+        full_population = new_population + not_repetitive_inds
+        return self.selection(full_population,
+                              pop_size=self.parameters.pop_size)
 
-    def _inheritance_type_by_genetic_scheme(self, previous_population: PopulationT,
-                                            new_population: PopulationT) -> Callable:
-        steady_state_scheme = partial(steady_state_inheritance, previous_population,
-                                      new_population, self.selection)
-        generational_scheme = partial(direct_inheritance, new_population, self.parameters.pop_size)
-        inheritance_type_by_genetic_scheme = {
-            GeneticSchemeTypesEnum.generational: generational_scheme,
-            GeneticSchemeTypesEnum.steady_state: steady_state_scheme,
-            GeneticSchemeTypesEnum.parameter_free: steady_state_scheme
-        }
-        return inheritance_type_by_genetic_scheme[self.parameters.genetic_scheme_type]
-
-
-def steady_state_inheritance(prev_population: PopulationT, new_population: PopulationT, selection: Selection) \
-        -> PopulationT:
-    selected_individuals = selection.individuals_selection(individuals=prev_population + new_population)
-    return selected_individuals
-
-
-def direct_inheritance(new_population: PopulationT, pop_size: int) -> PopulationT:
-    return new_population[:pop_size]
+    def direct_inheritance(self, new_population: PopulationT) -> PopulationT:
+        return new_population[:self.parameters.pop_size]
```

### Comparing `thegolem-0.3.1/golem/core/optimisers/genetic/operators/operator.py` & `thegolem-0.3.2/golem/core/optimisers/genetic/operators/operator.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/optimisers/genetic/operators/regularization.py` & `thegolem-0.3.2/golem/core/optimisers/genetic/operators/regularization.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,25 +41,25 @@
             prev_nodes_ids.add(ind.graph.descriptive_id)
             parent_operator = ParentOperator(type_='regularization',
                                              operators='decremental_regularization',
                                              parent_individuals=ind)
             subtree_inds = [Individual(OptGraph(deepcopy(ordered_subnodes_hierarchy(node))), parent_operator,
                                        metadata=self.requirements.static_individual_metadata)
                             for node in ind.graph.nodes
-                            if Regularization._is_fitted_subtree(self.graph_generation_params.adapter.restore(node))
-                            and node.descriptive_id not in prev_nodes_ids]
+                            if Regularization._is_fitted_subtree(self.graph_generation_params.adapter.restore(node)) and
+                            node.descriptive_id not in prev_nodes_ids]
 
             additional_inds.extend(subtree_inds)
             prev_nodes_ids.update(subtree.graph.root_node.descriptive_id for subtree in subtree_inds)
 
         additional_inds = [ind for ind in additional_inds if self.graph_generation_params.verifier(ind.graph)]
         evaluator(additional_inds)
         additional_inds.extend(population)
         if len(additional_inds) > size:
-            additional_inds = sorted(additional_inds, key=lambda ind: ind.fitness)[:size]
+            additional_inds = sorted(additional_inds, key=lambda ind: ind.fitness, reverse=True)[:size]
 
         return additional_inds
 
     # TODO: remove this hack (e.g. provide smth like FitGraph with fit/unfit interface)
     @staticmethod
     def _is_fitted_subtree(node: OptNode) -> bool:
         return node.nodes_from and hasattr(node, 'fitted_operation') and node.fitted_operation
```

### Comparing `thegolem-0.3.1/golem/core/optimisers/genetic/operators/selection.py` & `thegolem-0.3.2/golem/core/optimisers/genetic/operators/selection.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,36 +10,36 @@
 
 class SelectionTypesEnum(Enum):
     tournament = 'tournament'
     spea2 = 'spea2'
 
 
 class Selection(Operator):
-    def __call__(self, population: PopulationT) -> PopulationT:
+    def __call__(self, population: PopulationT, pop_size: Optional[int] = None) -> PopulationT:
         """
         Selection of individuals based on specified type of selection
         :param population: A list of individuals to select from.
+        :param pop_size: Optional custom population_size.
+        Taken from algorithm parameters if not specified.
         """
+        pop_size = pop_size or self.parameters.pop_size
         selection_type = choice(self.parameters.selection_types)
-        return self._selection_by_type(selection_type)(population, self.parameters.pop_size)
+        return self._selection_by_type(selection_type)(population, pop_size)
 
     @staticmethod
     def _selection_by_type(selection_type: SelectionTypesEnum) -> Callable[[PopulationT, int], PopulationT]:
         selections = {
             SelectionTypesEnum.tournament: tournament_selection,
             SelectionTypesEnum.spea2: spea2_selection
         }
         if selection_type in selections:
             return selections[selection_type]
         else:
             raise ValueError(f'Required selection not found: {selection_type}')
 
-    def individuals_selection(self, individuals: PopulationT) -> PopulationT:
-        return self.__call__(individuals)
-
 
 def default_selection_behaviour(selection_func: Optional[Callable] = None, *, ensure_unique: bool = True,
                                 populate_by_single: bool = True):
     def func_wrapper(func: Callable):
         @functools.wraps(func)
         def wrapper(individuals: PopulationT, pop_size: int, *args, **kwargs):
             if ensure_unique:
@@ -59,14 +59,16 @@
     if selection_func:
         return func_wrapper(selection_func)  # Allows to decorate without args.
     return func_wrapper  # Allows to decorate with args but no selection_func specified.
 
 
 @default_selection_behaviour
 def tournament_selection(individuals: PopulationT, pop_size: int, fraction: float = 0.1) -> PopulationT:
+    """ Having the size of *individuals* equals to *n* will have no effect other
+    than lax ordering of *individuals*. """
     individuals = list(individuals)  # don't modify original
     group_size = math.ceil(len(individuals) * fraction)
     min_group_size = min(2, len(individuals))
     group_size = max(group_size, min_group_size)
     chosen = []
     iterations_limit = pop_size * 10
     for _ in range(iterations_limit):
```

### Comparing `thegolem-0.3.1/golem/core/optimisers/genetic/parameters/graph_depth.py` & `thegolem-0.3.2/golem/core/optimisers/genetic/parameters/graph_depth.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/optimisers/genetic/parameters/mutation_prob.py` & `thegolem-0.3.2/golem/core/optimisers/genetic/parameters/mutation_prob.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/optimisers/genetic/parameters/operators_prob.py` & `thegolem-0.3.2/golem/core/optimisers/genetic/parameters/operators_prob.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/optimisers/genetic/parameters/parameter.py` & `thegolem-0.3.2/golem/core/optimisers/genetic/parameters/parameter.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/optimisers/genetic/parameters/population_size.py` & `thegolem-0.3.2/golem/core/optimisers/genetic/parameters/population_size.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import math
 from typing import Optional
 
-from .parameter import AdaptiveParameter
-from golem.core.utilities.data_structures import BidirectionalIterator
-from golem.core.utilities.sequence_iterator import fibonacci_sequence, SequenceIterator
-from ..gp_params import GPAlgorithmParameters
+from golem.core.constants import MIN_POP_SIZE
 from golem.core.optimisers.archive.generation_keeper import ImprovementWatcher
+from golem.core.optimisers.genetic.gp_params import GPAlgorithmParameters
 from golem.core.optimisers.genetic.operators.inheritance import GeneticSchemeTypesEnum
 from golem.core.optimisers.genetic.operators.operator import PopulationT
+from golem.core.optimisers.genetic.parameters.parameter import AdaptiveParameter
+from golem.core.utilities.data_structures import BidirectionalIterator
+from golem.core.utilities.sequence_iterator import fibonacci_sequence, SequenceIterator
 
 PopulationSize = AdaptiveParameter[int]
 
-# min pop size to avoid getting stuck in local maximum during optimization
-MIN_POP_SIZE = 5
-
 
 class ConstRatePopulationSize(PopulationSize):
     def __init__(self, pop_size: int, offspring_rate: float, max_pop_size: Optional[int] = None):
         self._offspring_rate = offspring_rate
         self._initial = pop_size
         self._max_pop_size = max_pop_size
 
@@ -52,15 +50,15 @@
     def next(self, population: PopulationT) -> int:
         fitness_improved = self._improvements.is_quality_improved
         complexity_decreased = self._improvements.is_complexity_improved
         progress_in_both_goals = fitness_improved and complexity_decreased
         no_progress = not fitness_improved and not complexity_decreased
         pop_size = len(population)
         too_many_fitness_eval_errors = \
-            pop_size/self._iterator.current() < 0.5
+            pop_size / self._iterator.current() < 0.5
 
         if too_many_fitness_eval_errors or no_progress:
             if self._iterator.has_next():
                 pop_size = self._iterator.next()
         elif progress_in_both_goals and pop_size > 0:
             if self._iterator.has_prev():
                 pop_size = self._iterator.prev()
```

### Comparing `thegolem-0.3.1/golem/core/optimisers/graph_builder.py` & `thegolem-0.3.2/golem/core/optimisers/graph_builder.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/optimisers/initial_graphs_generator.py` & `thegolem-0.3.2/golem/core/optimisers/initial_graphs_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,24 +40,23 @@
                 self.initial_graphs = self.initial_graphs[:pop_size]
             return adapter.adapt(self.initial_graphs)
 
         if not self.generation_function:
             self.generation_function = partial(self.graph_generation_params.random_graph_factory, self.requirements)
 
         population = []
-        n_iter = 0
-        while len(population) < pop_size:
+        for iter_num in range(MAX_GRAPH_GEN_ATTEMPTS):
+            if len(population) == pop_size:
+                break
             new_graph = self.generation_function()
             if new_graph not in population and self.graph_generation_params.verifier(new_graph):
                 population.append(new_graph)
-            n_iter += 1
-            if n_iter >= MAX_GRAPH_GEN_ATTEMPTS:
-                self.log.warning(f'Exceeded max number of attempts for generating initial graphs, stopping.'
-                                 f'Generated {len(population)} instead of {pop_size} graphs.')
-                break
+        else:
+            self.log.warning(f'Exceeded max number of attempts for generating initial graphs, stopping.'
+                             f'Generated {len(population)} instead of {pop_size} graphs.')
         return population
 
     def with_initial_graphs(self, initial_graphs: Union[Graph, Sequence[Graph]]):
         """Use initial graphs as initial population."""
         if isinstance(initial_graphs, Graph):
             self.initial_graphs = [initial_graphs]
         elif isinstance(initial_graphs, Iterable):
```

### Comparing `thegolem-0.3.1/golem/core/optimisers/objective/objective.py` & `thegolem-0.3.2/golem/core/optimisers/objective/objective.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/optimisers/objective/objective_eval.py` & `thegolem-0.3.2/golem/core/optimisers/objective/objective_eval.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/optimisers/opt_graph_builder.py` & `thegolem-0.3.2/golem/core/optimisers/opt_graph_builder.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/optimisers/opt_history_objects/generation.py` & `thegolem-0.3.2/golem/core/optimisers/opt_history_objects/generation.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/optimisers/opt_history_objects/individual.py` & `thegolem-0.3.2/golem/core/optimisers/opt_history_objects/individual.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/optimisers/opt_history_objects/opt_history.py` & `thegolem-0.3.2/golem/core/optimisers/opt_history_objects/opt_history.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,18 +31,17 @@
         default_save_dir: default directory used for saving history when not explicit path is provided.
     """
 
     def __init__(self,
                  objective: Optional[ObjectiveInfo] = None,
                  default_save_dir: Optional[os.PathLike] = None):
         self._objective = objective or ObjectiveInfo()
-        self.individuals: List[Generation] = []
+        self._generations: List[Generation] = []
         self.archive_history: List[List[Individual]] = []
         self._tuning_result: Optional[Graph] = None
-        self._log = default_log(self)
 
         # init default save directory
         if default_save_dir:
             default_save_dir = Path(default_save_dir)
             if not default_save_dir.is_absolute():
                 # if path is not absolute, treat it as relative to data dir
                 default_save_dir = Path(default_data_dir()) / default_save_dir
@@ -51,20 +50,20 @@
         self._default_save_dir = str(default_save_dir)
 
     @property
     def objective(self):
         return self._objective
 
     def is_empty(self) -> bool:
-        return not self.individuals
+        return not self.generations
 
     def add_to_history(self, individuals: Sequence[Individual], generation_label: Optional[str] = None,
                        generation_metadata: Optional[Dict[str, Any]] = None):
         generation = Generation(individuals, self.generations_count, generation_label, generation_metadata)
-        self.individuals.append(generation)
+        self.generations.append(generation)
 
     def add_to_archive_history(self, individuals: Sequence[Individual]):
         self.archive_history.append(list(individuals))
 
     def to_csv(self, save_dir: Optional[os.PathLike] = None, file: os.PathLike = 'history.csv'):
         save_dir = save_dir or self._default_save_dir
         if not os.path.isdir(save_dir):
@@ -78,30 +77,30 @@
             if self.objective.is_multi_objective:
                 metric_str += 's'
             header_row = ['index', 'generation', metric_str, 'quantity_of_operations', 'depth', 'metadata']
             writer.writerow(header_row)
 
             # Write history rows
             idx = 0
-            for gen_num, gen_inds in enumerate(self.individuals):
+            for gen_num, gen_inds in enumerate(self.generations):
                 for ind_num, ind in enumerate(gen_inds):
                     row = [idx, gen_num, ind.fitness.values, ind.graph.length, ind.graph.depth, ind.metadata]
                     writer.writerow(row)
                     idx += 1
 
     def save_current_results(self, save_dir: Optional[os.PathLike] = None):
         # Create folder if it's not exists
         save_dir = save_dir or self._default_save_dir
         if not os.path.isdir(save_dir):
             os.makedirs(save_dir)
             self._log.info(f"Created directory for saving optimization history: {save_dir}")
 
         try:
             last_gen_id = self.generations_count - 1
-            last_gen = self.individuals[last_gen_id]
+            last_gen = self.generations[last_gen_id]
             for individual in last_gen:
                 ind_path = Path(save_dir, str(last_gen_id), str(individual.uid))
                 if not os.path.isdir(ind_path):
                     os.makedirs(ind_path)
                 individual.save(json_file_path=Path(ind_path, f'{str(individual.uid)}.json'))
         except Exception as ex:
             self._log.exception(ex)
@@ -121,23 +120,23 @@
             os.mkdir(dir_path)
 
     @property
     def historical_fitness(self) -> Sequence[Sequence[Union[float, Sequence[float]]]]:
         """Return sequence of histories of generations per each metric"""
         if self.objective.is_multi_objective:
             historical_fitness = []
-            num_metrics = len(self.individuals[0][0].fitness.values)
+            num_metrics = len(self.generations[0][0].fitness.values)
             for objective_num in range(num_metrics):
                 # history of specific objective for each generation
                 objective_history = [[ind.fitness.values[objective_num] for ind in generation]
-                                     for generation in self.individuals]
+                                     for generation in self.generations]
                 historical_fitness.append(objective_history)
         else:
             historical_fitness = [[ind.fitness.value for ind in pop]
-                                  for pop in self.individuals]
+                                  for pop in self.generations]
         return historical_fitness
 
     @property
     def all_historical_fitness(self) -> List[float]:
         historical_fitness = self.historical_fitness
         if self.objective.is_multi_objective:
             all_historical_fitness = []
@@ -172,15 +171,15 @@
         """
         Prints ordered description of the best solutions in history
         :param top_n: number of solutions to print
         """
         # Take only the first graph's appearance in history
         individuals_with_positions \
             = list({ind.graph.descriptive_id: (ind, gen_num, ind_num)
-                    for gen_num, gen in enumerate(self.individuals)
+                    for gen_num, gen in enumerate(self.generations)
                     for ind_num, ind in reversed(list(enumerate(gen)))}.values())
 
         top_individuals = sorted(individuals_with_positions,
                                  key=lambda pos_ind: pos_ind[0].fitness, reverse=True)[:top_n]
 
         output = io.StringIO()
         separator = ' | '
@@ -191,46 +190,69 @@
             positional_id = f'g{gen_num}-i{ind_num}'
             print(separator.join([f'{ind_num:>3}, '
                                   f'{str(individual.fitness):>8}, '
                                   f'{positional_id:>8}, '
                                   f'{individual.graph.descriptive_id}']), file=output)
 
         # add info about initial assumptions (stored as zero generation)
-        for i, individual in enumerate(self.individuals[0]):
+        for i, individual in enumerate(self.generations[0]):
             ind = f'I{i}'
             positional_id = '-'
             print(separator.join([f'{ind:>3}'
                                   f'{str(individual.fitness):>8}',
                                   f'{positional_id}',
                                   f'{individual.graph.descriptive_id}']), file=output)
         return output.getvalue()
 
     @property
     def initial_assumptions(self) -> Optional[Generation]:
-        if not self.individuals:
+        if not self.generations:
             return None
-        for gen in self.individuals:
+        for gen in self.generations:
             if gen.label == 'initial_assumptions':
                 return gen
 
     @property
     def final_choices(self) -> Optional[Generation]:
-        if not self.individuals:
+        if not self.generations:
             return None
-        for gen in reversed(self.individuals):
+        for gen in reversed(self.generations):
             if gen.label == 'final_choices':
                 return gen
 
     @property
     def generations_count(self) -> int:
-        return len(self.individuals)
+        return len(self.generations)
 
     @property
     def tuning_result(self):
         if hasattr(self, '_tuning_result'):
             return self._tuning_result
         else:
             return None
 
     @tuning_result.setter
     def tuning_result(self, val):
         self._tuning_result = val
+
+    @property
+    def generations(self):
+        return self._generations
+
+    @generations.setter
+    def generations(self, value):
+        self._generations = value
+
+    @property
+    def individuals(self):
+        self._log.warning(
+            '"OptHistory.individuals" is deprecated and will be removed later. '
+            'Please, use "OptHistory.generations" to access generations.')
+        return self.generations
+
+    @individuals.setter
+    def individuals(self, value):
+        self.generations = value
+
+    @property
+    def _log(self):
+        return default_log(self)
```

### Comparing `thegolem-0.3.1/golem/core/optimisers/opt_history_objects/parent_operator.py` & `thegolem-0.3.2/golem/core/optimisers/opt_history_objects/parent_operator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import Iterable, Tuple, Union
+from typing import Hashable, Sequence
 from uuid import uuid4
 
 from golem.core.optimisers.opt_history_objects.individual import Individual
 from golem.core.utilities.data_structures import ensure_wrapped_in_sequence
 
 
 @dataclass(frozen=True)
 class ParentOperator:
     type_: str
-    operators: Union[Tuple[str, ...], str]
-    parent_individuals: Union[Iterable[Individual], Individual] = field()
+    operators: Sequence[Hashable]
+    parent_individuals: Sequence[Individual] = field()
     uid: str = field(default_factory=lambda: str(uuid4()), init=False)
 
     def __post_init__(self):
-        if isinstance(self.operators, str):
-            object.__setattr__(self, 'operators', (self.operators,))
+        operators = ensure_wrapped_in_sequence(self.operators)
+        object.__setattr__(self, 'operators', tuple(operators))
         parent_individuals = ensure_wrapped_in_sequence(self.parent_individuals)
         object.__setattr__(self, 'parent_individuals', tuple(parent_individuals))
 
     def __repr__(self):
         return (f'<ParentOperator {self.uid} | type: {self.type_} | operators: {self.operators} '
                 f'| parent_individuals({len(self.parent_individuals)}): {self.parent_individuals}>')
```

### Comparing `thegolem-0.3.1/golem/core/optimisers/opt_node_factory.py` & `thegolem-0.3.2/golem/core/optimisers/opt_node_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,21 +40,21 @@
     one node from the provided lists of available nodes
     or returns a node with a random numeric node name
     in the range from 0 to `num_node_types`."""
 
     def __init__(self,
                  available_node_types: Optional[Iterable[str]] = None,
                  num_node_types: Optional[int] = None):
-        self._available_nodes = tuple(available_node_types) if available_node_types else None
+        self.available_nodes = tuple(available_node_types) if available_node_types else None
         self._num_node_types = num_node_types or 1000
 
     def exchange_node(self, node: OptNode) -> OptNode:
         return self.get_node()
 
     def get_parent_node(self, node: OptNode, **kwargs) -> OptNode:
         return self.get_node(**kwargs)
 
     def get_node(self, **kwargs) -> OptNode:
-        chosen_node_type = choice(self._available_nodes) \
-            if self._available_nodes \
+        chosen_node_type = choice(self.available_nodes) \
+            if self.available_nodes \
             else random.randint(0, self._num_node_types)
         return OptNode(content={'name': chosen_node_type})
```

### Comparing `thegolem-0.3.1/golem/core/optimisers/optimization_parameters.py` & `thegolem-0.3.2/golem/core/optimisers/optimization_parameters.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/optimisers/optimizer.py` & `thegolem-0.3.2/golem/core/optimisers/optimizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 from golem.core.adapter import BaseOptimizationAdapter, IdentityAdapter
 from golem.core.dag.graph import Graph
 from golem.core.dag.graph_verifier import GraphVerifier, VerifierRuleType
 from golem.core.dag.verification_rules import DEFAULT_DAG_RULES
 from golem.core.log import default_log
 from golem.core.optimisers.advisor import DefaultChangeAdvisor
-from golem.core.optimisers.archive import GenerationKeeper
 from golem.core.optimisers.optimization_parameters import OptimizationParameters
 from golem.core.optimisers.genetic.evaluation import DelegateEvaluator
 from golem.core.optimisers.genetic.operators.operator import PopulationT
 from golem.core.optimisers.graph import OptGraph
 from golem.core.optimisers.objective import GraphFunction, Objective, ObjectiveFunction
 from golem.core.optimisers.opt_history_objects.opt_history import OptHistory
 from golem.core.optimisers.opt_node_factory import DefaultOptNodeFactory, OptNodeFactory
 from golem.core.optimisers.random_graph_factory import RandomGraphFactory, RandomGrowthGraphFactory
 
-OptimisationCallback = Callable[[PopulationT, GenerationKeeper], Any]
+
+STRUCTURAL_DIVERSITY_FREQUENCY_CHECK = 5
 
 
 def do_nothing_callback(*args, **kwargs):
     pass
 
 
 @dataclass
@@ -40,14 +40,15 @@
 
     multi_objective: bool = False
     offspring_rate: float = 0.5
     pop_size: int = 20
     max_pop_size: Optional[int] = 55
     adaptive_depth: bool = False
     adaptive_depth_max_stagnation: int = 3
+    structural_diversity_frequency_check: int = STRUCTURAL_DIVERSITY_FREQUENCY_CHECK
 
 
 @dataclass
 class GraphGenerationParams:
     """
     This dataclass is for defining the parameters using in graph generation process
 
@@ -110,15 +111,15 @@
                  graph_optimizer_params: Optional[AlgorithmParameters] = None):
         self.log = default_log(self)
         self._objective = objective
         self.initial_graphs = graph_generation_params.adapter.adapt(initial_graphs) if initial_graphs else None
         self.requirements = requirements or OptimizationParameters()
         self.graph_generation_params = graph_generation_params or GraphGenerationParams()
         self.graph_optimizer_params = graph_optimizer_params or AlgorithmParameters()
-        self._optimisation_callback: OptimisationCallback = do_nothing_callback
+        self._iteration_callback: IterationCallback = do_nothing_callback
         self._history = OptHistory(objective.get_info(), requirements.history_dir) \
             if requirements and requirements.keep_history else None
 
     @property
     def objective(self) -> Objective:
         """Returns Objective of this optimizer with information about metrics used."""
         return self._objective
@@ -133,16 +134,20 @@
         """
         Method for running of optimization using specified algorithm.
         :param objective: objective function that specifies optimization target
         :return: sequence of the best graphs
         """
         pass
 
-    def set_optimisation_callback(self, callback: Optional[OptimisationCallback]):
-        """Set optimisation callback that must run on each iteration.
-        Reset the callback if None is passed."""
-        self._optimisation_callback = callback or do_nothing_callback
+    def set_iteration_callback(self, callback: Optional[Callable]):
+        """Set optimisation callback that is called at the end of
+        each iteration, with the next generation passed as argument.
+        Resets the callback if None is passed."""
+        self._iteration_callback = callback or do_nothing_callback
 
     def set_evaluation_callback(self, callback: Optional[GraphFunction]):
         """Set or reset (with None) post-evaluation callback
         that's called on each graph after its evaluation."""
         pass
+
+
+IterationCallback = Callable[[PopulationT, GraphOptimizer], Any]
```

### Comparing `thegolem-0.3.1/golem/core/optimisers/populational_optimizer.py` & `thegolem-0.3.2/golem/core/optimisers/populational_optimizer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from abc import abstractmethod
+from random import choice
 from typing import Any, Optional, Sequence, Dict
 
 from tqdm import tqdm
 
+from golem.core.constants import MIN_POP_SIZE
 from golem.core.dag.graph import Graph
 from golem.core.optimisers.archive import GenerationKeeper
 from golem.core.optimisers.genetic.evaluation import MultiprocessingDispatcher, SequentialDispatcher
 from golem.core.optimisers.genetic.operators.operator import PopulationT, EvaluationOperator
-from golem.core.optimisers.optimization_parameters import GraphRequirements
 from golem.core.optimisers.objective import GraphFunction, ObjectiveFunction
 from golem.core.optimisers.objective.objective import Objective
+from golem.core.optimisers.opt_history_objects.individual import Individual
+from golem.core.optimisers.optimization_parameters import GraphRequirements
 from golem.core.optimisers.optimizer import GraphGenerationParams, GraphOptimizer, AlgorithmParameters
 from golem.core.optimisers.timer import OptimisationTimer
 from golem.core.utilities.grouped_condition import GroupedCondition
 
 
 class PopulationalOptimizer(GraphOptimizer):
     """
@@ -59,20 +62,23 @@
                 lambda: self.timer.is_time_limit_reached(self.current_generation_num),
                 'Optimisation stopped: Time limit is reached'
             ).add_condition(
                 lambda: (requirements.num_of_generations is not None and
                          self.current_generation_num >= requirements.num_of_generations + 1),
                 'Optimisation stopped: Max number of generations reached'
             ).add_condition(
-                lambda: self.generations.stagnation_iter_count >= max_stagnation_length,
+                lambda: (max_stagnation_length is not None and
+                         self.generations.stagnation_iter_count >= max_stagnation_length),
                 'Optimisation finished: Early stopping iterations criteria was satisfied'
             ).add_condition(
                 lambda: self.generations.stagnation_time_duration >= max_stagnation_time,
                 'Optimisation finished: Early stopping timeout criteria was satisfied'
             )
+        # in how many generations structural diversity check should be performed
+        self.gen_structural_diversity_check = self.graph_optimizer_params.structural_diversity_frequency_check
 
     @property
     def current_generation_num(self) -> int:
         return self.generations.generation_num
 
     def set_evaluation_callback(self, callback: Optional[GraphFunction]):
         # Redirect callback to evaluation dispatcher
@@ -86,14 +92,18 @@
         with self.timer, self._progressbar:
 
             self._initial_population(evaluator)
 
             while not self.stop_optimization():
                 try:
                     new_population = self._evolve_population(evaluator)
+                    if self.gen_structural_diversity_check != -1 \
+                            and self.generations.generation_num % self.gen_structural_diversity_check == 0 \
+                            and self.generations.generation_num != 0:
+                        new_population = self.get_structure_unique_population(new_population, evaluator)
                 except EvaluationAttemptsError as ex:
                     self.log.warning(f'Composition process was stopped due to: {ex}')
                     return [ind.graph for ind in self.best_individuals]
                 # Adding of new population to history
                 self._update_population(new_population)
         self._update_population(self.best_individuals, 'final_choices')
         return [ind.graph for ind in self.best_individuals]
@@ -108,33 +118,51 @@
         raise NotImplementedError()
 
     @abstractmethod
     def _evolve_population(self, evaluator: EvaluationOperator) -> PopulationT:
         """ Method realizing full evolution cycle """
         raise NotImplementedError()
 
+    def _extend_population(self, pop: PopulationT, target_pop_size: int) -> PopulationT:
+        """ Extends population to specified `target_pop_size`. """
+        n = target_pop_size - len(pop)
+        extended_population = list(pop)
+        extended_population.extend([Individual(graph=choice(pop).graph) for _ in range(n)])
+        return extended_population
+
     def _update_population(self, next_population: PopulationT, label: Optional[str] = None,
                            metadata: Optional[Dict[str, Any]] = None):
         self.generations.append(next_population)
-        self._optimisation_callback(next_population, self.generations)
         self._log_to_history(next_population, label, metadata)
+        self._iteration_callback(next_population, self)
         self.population = next_population
 
         self.log.info(f'Generation num: {self.current_generation_num} size: {len(next_population)}')
         self.log.info(f'Best individuals: {str(self.generations)}')
         if self.generations.stagnation_iter_count > 0:
             self.log.info(f'no improvements for {self.generations.stagnation_iter_count} iterations')
             self.log.info(f'spent time: {round(self.timer.minutes_from_start, 1)} min')
 
     def _log_to_history(self, population: PopulationT, label: Optional[str] = None,
                         metadata: Optional[Dict[str, Any]] = None):
         self.history.add_to_history(population, label, metadata)
         self.history.add_to_archive_history(self.generations.best_individuals)
         if self.requirements.history_dir:
-            self.history.save_current_results()
+            self.history.save_current_results(self.requirements.history_dir)
+
+    def get_structure_unique_population(self, population: PopulationT, evaluator: EvaluationOperator) -> PopulationT:
+        """ Increases structurally uniqueness of population to prevent stagnation in optimization process.
+        Returned population may be not entirely unique, if the size of unique population is lower than MIN_POP_SIZE. """
+        unique_population_with_ids = {ind.graph.descriptive_id: ind for ind in population}
+        unique_population = list(unique_population_with_ids.values())
+
+        # if size of unique population is too small, then extend it to MIN_POP_SIZE by repeating individuals
+        if len(unique_population) < MIN_POP_SIZE:
+            unique_population = self._extend_population(pop=unique_population, target_pop_size=MIN_POP_SIZE)
+        return evaluator(unique_population)
 
     @property
     def _progressbar(self):
         if self.requirements.show_progress:
             bar = tqdm(total=self.requirements.num_of_generations,
                        desc='Generations', unit='gen', initial=1)
         else:
```

### Comparing `thegolem-0.3.1/golem/core/optimisers/random/random_mutation_optimizer.py` & `thegolem-0.3.2/golem/core/optimisers/random/random_mutation_optimizer.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/optimisers/random/random_search.py` & `thegolem-0.3.2/golem/core/optimisers/random/random_search.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/optimisers/random_graph_factory.py` & `thegolem-0.3.2/golem/core/optimisers/random_graph_factory.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/optimisers/timer.py` & `thegolem-0.3.2/golem/core/optimisers/timer.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/paths.py` & `thegolem-0.3.2/golem/core/paths.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/tuning/sequential.py` & `thegolem-0.3.2/golem/core/tuning/sequential.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,34 +2,43 @@
 from functools import partial
 from typing import Callable, Optional
 
 from hyperopt import tpe, fmin, space_eval
 
 from golem.core.adapter import BaseOptimizationAdapter
 from golem.core.optimisers.graph import OptGraph
-from golem.core.optimisers.objective import ObjectiveEvaluate
-from golem.core.tuning.search_space import SearchSpace, convert_params
-from golem.core.tuning.tuner_interface import HyperoptTuner, DomainGraphForTune
+from golem.core.optimisers.objective import ObjectiveFunction
+from golem.core.tuning.hyperopt_tuner import HyperoptTuner, get_node_parameters_for_hyperopt
+from golem.core.tuning.search_space import SearchSpace
+from golem.core.tuning.tuner_interface import DomainGraphForTune
 
 
 class SequentialTuner(HyperoptTuner):
     """
     Class for hyperparameters optimization for all nodes sequentially
     """
 
-    def __init__(self, objective_evaluate: ObjectiveEvaluate,
+    def __init__(self, objective_evaluate: ObjectiveFunction,
                  search_space: SearchSpace,
                  adapter: Optional[BaseOptimizationAdapter] = None,
-                 iterations=100, early_stopping_rounds=None,
+                 iterations: int = 100,
+                 early_stopping_rounds: Optional[int] = None,
                  timeout: timedelta = timedelta(minutes=5),
-                 inverse_node_order=False,
+                 n_jobs: int = -1,
+                 deviation: float = 0.05,
                  algo: Callable = tpe.suggest,
-                 n_jobs: int = -1):
-        super().__init__(objective_evaluate, search_space, adapter, iterations, early_stopping_rounds,
-                         timeout, algo, n_jobs)
+                 inverse_node_order: bool = False):
+        super().__init__(objective_evaluate,
+                         search_space,
+                         adapter,
+                         iterations,
+                         early_stopping_rounds, timeout,
+                         n_jobs,
+                         deviation,
+                         algo)
 
         self.inverse_node_order = inverse_node_order
 
     def tune(self, graph: DomainGraphForTune) -> DomainGraphForTune:
         """ Method for hyperparameters tuning on the entire graph
 
         Args:
@@ -57,33 +66,33 @@
         # Tuning performed sequentially for every node - so get ids of nodes
         nodes_ids = self.get_nodes_order(nodes_number=nodes_amount)
         for node_id in nodes_ids:
             node = graph.nodes[node_id]
             operation_name = node.name
 
             # Get node's parameters to optimize
-            node_params = self.search_space.get_node_params(node_id=node_id,
-                                                            operation_name=operation_name)
+            node_params = get_node_parameters_for_hyperopt(self.search_space, node_id, operation_name)
 
-            if node_params is None:
+            if not node_params:
                 self.log.info(f'"{operation_name}" operation has no parameters to optimize')
             else:
                 # Apply tuning for current node
                 self._optimize_node(node_id=node_id,
                                     graph=graph,
                                     node_params=node_params,
                                     iterations_per_node=iterations_per_node,
                                     seconds_per_node=seconds_per_node)
 
-        # Validation is the optimization do well
+        # Validate if optimisation did well
         final_graph = self.final_check(graph)
 
         self.was_tuned = True
+        final_graph = self.adapter.restore(final_graph)
 
-        return self.adapter.restore(final_graph)
+        return final_graph
 
     def get_nodes_order(self, nodes_number: int) -> range:
         """ Method returns list with indices of nodes in the graph
 
         Args:
             nodes_number: number of nodes to get
         """
@@ -111,18 +120,19 @@
 
         self.init_check(graph)
 
         node = graph.nodes[node_index]
         operation_name = node.name
 
         # Get node's parameters to optimize
-        node_params = self.search_space.get_node_params(node_id=node_index,
-                                                        operation_name=operation_name)
+        node_params = get_node_parameters_for_hyperopt(self.search_space,
+                                                       node_id=node_index,
+                                                       operation_name=operation_name)
 
-        if node_params is None:
+        if not node_params:
             self._stop_tuning_with_message(f'"{operation_name}" operation has no parameters to optimize')
         else:
             # Apply tuning for current node
             self._optimize_node(graph=graph,
                                 node_id=node_index,
                                 node_params=node_params,
                                 iterations_per_node=self.iterations,
@@ -131,46 +141,43 @@
             self.was_tuned = True
 
         # Validation is the optimization do well
         final_graph = self.final_check(graph)
         final_graph = self.adapter.restore(final_graph)
         return final_graph
 
-    def _optimize_node(self, graph: OptGraph, node_id: int, node_params: dict, iterations_per_node: int,
+    def _optimize_node(self, graph: OptGraph,
+                       node_id: int,
+                       node_params: dict,
+                       iterations_per_node: int,
                        seconds_per_node: int) -> OptGraph:
         """
         Method for node optimization
 
         Args:
             graph: Graph which node is optimized
             node_id: id of the current node in the graph
             node_params: dictionary with parameters for node
             iterations_per_node: amount of iterations to produce
             seconds_per_node: amount of seconds to produce
 
         Returns:
             updated graph with tuned parameters in particular node
         """
-        best_parameters = fmin(partial(self._objective,
-                                       graph=graph,
-                                       node_id=node_id
-                                       ),
+        best_parameters = fmin(partial(self._objective, graph=graph, node_id=node_id),
                                node_params,
                                algo=self.algo,
                                max_evals=iterations_per_node,
                                early_stop_fn=self.early_stop_fn,
                                timeout=seconds_per_node)
 
-        best_parameters = space_eval(space=node_params,
-                                     hp_assignment=best_parameters)
+        best_parameters = space_eval(space=node_params, hp_assignment=best_parameters)
 
         # Set best params for this node in the graph
-        graph = self.set_arg_node(graph=graph,
-                                  node_id=node_id,
-                                  node_params=best_parameters)
+        graph = self.set_arg_node(graph=graph, node_id=node_id, node_params=best_parameters)
         return graph
 
     def _objective(self, node_params: dict, graph: OptGraph, node_id: int) -> float:
         """ Objective function for minimization problem
 
         Args:
             node_params: dictionary with parameters for node
@@ -178,33 +185,11 @@
             node_id: id of the node to which parameters should be assigned
 
         Returns:
             value of objective function
         """
 
         # Set hyperparameters for node
-        graph = self.set_arg_node(graph=graph, node_id=node_id,
-                                  node_params=node_params)
+        graph = self.set_arg_node(graph=graph, node_id=node_id, node_params=node_params)
 
         metric_value = self.get_metric_value(graph=graph)
         return metric_value
-
-    @staticmethod
-    def set_arg_node(graph: OptGraph, node_id: int, node_params: dict) -> OptGraph:
-        """ Method for parameters setting to a graph
-
-        Args:
-            graph: graph which contains the node
-            node_id: id of the node to which parameters should be assigned
-            node_params: dictionary with labeled parameters to set
-
-        Returns:
-            graph with new hyperparameters in each node
-        """
-
-        # Remove label prefixes
-        node_params = convert_params(node_params)
-
-        # Update parameters in nodes
-        graph.nodes[node_id].parameters = node_params
-
-        return graph
```

### Comparing `thegolem-0.3.1/golem/core/tuning/simultaneous.py` & `thegolem-0.3.2/golem/core/tuning/simultaneous.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 from typing import Tuple, Optional
 
 from hyperopt import Trials, fmin, space_eval
 
 from golem.core.constants import MIN_TIME_FOR_TUNING_IN_SEC
 from golem.core.optimisers.graph import OptGraph
 from golem.core.optimisers.timer import Timer
-from golem.core.tuning.search_space import get_node_operation_parameter_label, convert_params
-from golem.core.tuning.tuner_interface import HyperoptTuner, DomainGraphForTune
+from golem.core.tuning.hyperopt_tuner import HyperoptTuner, get_node_parameters_for_hyperopt
+from golem.core.tuning.search_space import get_node_operation_parameter_label
+from golem.core.tuning.tuner_interface import DomainGraphForTune
 
 
 class SimultaneousTuner(HyperoptTuner):
     """
         Class for hyperparameters optimization for all nodes simultaneously
     """
+
     def tune(self, graph: DomainGraphForTune, show_progress: bool = True) -> DomainGraphForTune:
         """ Function for hyperparameters tuning on the entire graph
 
         Args:
             graph: graph which hyperparameters will be tuned
             show_progress: shows progress of tuning if True
 
@@ -26,69 +28,72 @@
         """
 
         graph = self.adapter.adapt(graph)
         parameters_dict, init_parameters = self._get_parameters_for_tune(graph)
 
         with Timer() as global_tuner_timer:
             self.init_check(graph)
-
             self._update_remaining_time(global_tuner_timer)
 
-            if self.max_seconds <= MIN_TIME_FOR_TUNING_IN_SEC:
-                self._stop_tuning_with_message('Tunner stopped after initial assumption due to the lack of time')
-
-            elif not parameters_dict:
+            if not parameters_dict:
                 self._stop_tuning_with_message(f'Graph "{graph.graph_description}" has no parameters to optimize')
+                final_graph = graph
 
-            else:
+            elif self.max_seconds <= MIN_TIME_FOR_TUNING_IN_SEC:
+                self._stop_tuning_with_message('Tunner stopped after initial assumption due to the lack of time')
+                final_graph = graph
 
+            else:
                 trials = Trials()
 
                 try:
                     # try searching using initial parameters
                     # (uses original search space with fixed initial parameters)
-                    trials, init_trials_num = self._search_near_initial_parameters(graph, parameters_dict,
+                    trials, init_trials_num = self._search_near_initial_parameters(graph,
+                                                                                   parameters_dict,
                                                                                    init_parameters,
-                                                                                   trials, show_progress)
+                                                                                   trials,
+                                                                                   show_progress)
                     self._update_remaining_time(global_tuner_timer)
                     if self.max_seconds > MIN_TIME_FOR_TUNING_IN_SEC:
-                        best = fmin(partial(self._objective, graph=graph),
-                                    parameters_dict,
-                                    trials=trials,
-                                    algo=self.algo,
-                                    max_evals=self.iterations,
-                                    show_progressbar=show_progress,
-                                    early_stop_fn=self.early_stop_fn,
-                                    timeout=self.max_seconds)
+                        fmin(partial(self._objective, graph=graph),
+                             parameters_dict,
+                             trials=trials,
+                             algo=self.algo,
+                             max_evals=self.iterations,
+                             show_progressbar=show_progress,
+                             early_stop_fn=self.early_stop_fn,
+                             timeout=self.max_seconds)
                     else:
                         self.log.message('Tunner stopped after initial search due to the lack of time')
 
-                    best = space_eval(space=parameters_dict, hp_assignment=best)
+                    best = space_eval(space=parameters_dict, hp_assignment=trials.argmin)
                     # check if best point was obtained using search space with fixed initial parameters
                     is_best_trial_with_init_params = trials.best_trial.get('tid') in range(init_trials_num)
                     if is_best_trial_with_init_params:
                         best = {**best, **init_parameters}
 
-                    tuned_graph = self.set_arg_graph(graph=graph,
-                                                     parameters=best)
-
-                    # Validation is the optimization do well
-                    graph = self.final_check(tuned_graph)
+                    final_graph = self.set_arg_graph(graph=graph, parameters=best)
 
                     self.was_tuned = True
 
                 except Exception as ex:
                     self.log.warning(f'Exception {ex} occurred during tuning')
+                    final_graph = graph
 
+        # Validate if optimisation did well
+        graph = self.final_check(final_graph)
         final_graph = self.adapter.restore(graph)
-
         return final_graph
 
-    def _search_near_initial_parameters(self, graph: OptGraph, search_space: dict, initial_parameters: dict,
-                                        trials: Trials, show_progress: bool = True) -> Tuple[Trials, int]:
+    def _search_near_initial_parameters(self, graph: OptGraph,
+                                        search_space: dict,
+                                        initial_parameters: dict,
+                                        trials: Trials,
+                                        show_progress: bool = True) -> Tuple[Trials, int]:
         """ Method to search using the search space where parameters initially set for the graph are fixed.
         This allows not to lose results obtained while composition process
 
         Args:
             graph: graph to be tuned
             search_space: dict with parameters to be optimized and their search spaces
             initial_parameters: dict with initial parameters of the graph
@@ -135,24 +140,22 @@
         parameters_dict = {}
         initial_parameters = {}
         for node_id, node in enumerate(graph.nodes):
             operation_name = node.name
 
             # Assign unique prefix for each model hyperparameter
             # label - number of node in the graph
-            node_params = self.search_space.get_node_params(node_id=node_id,
-                                                            operation_name=operation_name)
+            node_params = get_node_parameters_for_hyperopt(self.search_space, node_id=node_id,
+                                                           operation_name=operation_name)
+            parameters_dict.update(node_params)
 
-            if node_params is not None:
-                parameters_dict.update(node_params)
-
-            tunable_node_params = self.search_space.get_operation_parameter_range(operation_name)
+            tunable_node_params = self.search_space.get_parameters_for_operation(operation_name)
             if tunable_node_params:
                 tunable_initial_params = {get_node_operation_parameter_label(node_id, operation_name, p):
-                                              node.parameters[p] for p in node.parameters if p in tunable_node_params}
+                                          node.parameters[p] for p in node.parameters if p in tunable_node_params}
                 if tunable_initial_params:
                     initial_parameters.update(tunable_initial_params)
 
         return parameters_dict, initial_parameters
 
     def _objective(self, parameters_dict: dict, graph: OptGraph, unchangeable_parameters: Optional[dict] = None) \
             -> float:
@@ -174,32 +177,7 @@
 
         # Set hyperparameters for every node
         graph = self.set_arg_graph(graph, parameters_dict)
 
         metric_value = self.get_metric_value(graph=graph)
 
         return metric_value
-
-    @staticmethod
-    def set_arg_graph(graph: OptGraph, parameters: dict) -> OptGraph:
-        """ Method for parameters setting to a graph
-
-        Args:
-            graph: graph to which parameters should be assigned
-            parameters: dictionary with parameters to set
-
-        Returns:
-            graph: graph with new hyperparameters in each node
-        """
-        # Set hyperparameters for every node
-        for node_id, node in enumerate(graph.nodes):
-            node_params = {key: value for key, value in parameters.items()
-                           if key.startswith(f'{str(node_id)} || {node.name}')}
-
-            if node_params is not None:
-                # Delete all prefix strings to get appropriate parameters names
-                new_params = convert_params(node_params)
-
-                # Update parameters in nodes
-                graph.nodes[node_id].parameters = new_params
-
-        return graph
```

### Comparing `thegolem-0.3.1/golem/core/tuning/tuner_interface.py` & `thegolem-0.3.2/golem/core/tuning/tuner_interface.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,134 +1,128 @@
 from abc import abstractmethod
 from copy import deepcopy
 from datetime import timedelta
-from typing import Callable, TypeVar, Generic
+from typing import TypeVar, Generic, Optional, Union, Sequence
 
 import numpy as np
-from hyperopt.early_stop import no_progress_loss
 
 from golem.core.adapter import BaseOptimizationAdapter
 from golem.core.adapter.adapter import IdentityAdapter
 from golem.core.constants import MAX_TUNING_METRIC_VALUE
 from golem.core.dag.graph_utils import graph_structure
 from golem.core.log import default_log
+from golem.core.optimisers.fitness import SingleObjFitness, MultiObjFitness
 from golem.core.optimisers.graph import OptGraph
-from golem.core.optimisers.objective import ObjectiveEvaluate
-from golem.core.optimisers.timer import Timer
-from golem.core.tuning.search_space import SearchSpace
+from golem.core.optimisers.objective import ObjectiveEvaluate, ObjectiveFunction
+from golem.core.tuning.search_space import SearchSpace, convert_parameters
+from golem.core.utilities.data_structures import ensure_wrapped_in_sequence
 
 DomainGraphForTune = TypeVar('DomainGraphForTune')
 
 
-class HyperoptTuner(Generic[DomainGraphForTune]):
+class BaseTuner(Generic[DomainGraphForTune]):
     """
-    Base class for hyperparameters optimization based on hyperopt library
-    
+    Base class for hyperparameters optimization
+
     Args:
       objective_evaluate: objective to optimize
       adapter: the function for processing of external object that should be optimized
+      search_space: SearchSpace instance
       iterations: max number of iterations
+      early_stopping_rounds: Optional max number of stagnating iterations for early stopping.
       timeout: max time for tuning
-      search_space: SearchSpace instance
-      algo: algorithm for hyperparameters optimization with signature similar to :obj:`hyperopt.tse.suggest`
       n_jobs: num of ``n_jobs`` for parallelization (``-1`` for use all cpu's)
       deviation: required improvement (in percent) of a metric to return tuned graph.
         By default, ``deviation=0.05``, which means that tuned graph will be returned
         if it's metric will be at least 0.05% better than the initial.
     """
 
-    def __init__(self, objective_evaluate: ObjectiveEvaluate,
+    def __init__(self, objective_evaluate: ObjectiveFunction,
                  search_space: SearchSpace,
-                 adapter: BaseOptimizationAdapter = None,
-                 iterations=100, early_stopping_rounds=None,
+                 adapter: Optional[BaseOptimizationAdapter] = None,
+                 iterations: int = 100,
+                 early_stopping_rounds: Optional[int] = None,
                  timeout: timedelta = timedelta(minutes=5),
-                 algo: Callable = None,
                  n_jobs: int = -1,
                  deviation: float = 0.05):
         self.iterations = iterations
         self.adapter = adapter or IdentityAdapter()
-        iteration_stop_count = early_stopping_rounds or max(100, int(np.sqrt(iterations) * 10))
-        self.early_stop_fn = no_progress_loss(iteration_stop_count=iteration_stop_count)
-        self.max_seconds = int(timeout.seconds) if timeout is not None else None
-        self.init_graph = None
-        self.init_metric = None
-        self.obtained_metric = None
-        self.n_jobs = n_jobs
-        objective_evaluate.eval_n_jobs = self.n_jobs
-        self.objective_evaluate = self.adapter.adapt_func(objective_evaluate.evaluate)
-        self._default_metric_value = MAX_TUNING_METRIC_VALUE
         self.search_space = search_space
-        self.algo = algo
+        self.n_jobs = n_jobs
+        if isinstance(objective_evaluate, ObjectiveEvaluate):
+            objective_evaluate.eval_n_jobs = self.n_jobs
+        self.objective_evaluate = self.adapter.adapt_func(objective_evaluate)
         self.deviation = deviation
+
+        self.timeout = timeout
+        self.early_stopping_rounds = early_stopping_rounds
+
+        self._default_metric_value = MAX_TUNING_METRIC_VALUE
         self.was_tuned = False
+        self.init_graph = None
+        self.init_metric = None
+        self.obtained_metric = None
         self.log = default_log(self)
 
     @abstractmethod
-    def tune(self, graph: DomainGraphForTune) -> DomainGraphForTune:
+    def tune(self, graph: DomainGraphForTune) -> Union[DomainGraphForTune, Sequence[DomainGraphForTune]]:
         """
         Function for hyperparameters tuning on the graph
 
         Args:
           graph: domain graph for which hyperparameters tuning is needed
 
         Returns:
           Graph with optimized hyperparameters
+          or pareto front of optimized graphs in case of multi-objective optimization
         """
         raise NotImplementedError()
 
-    def get_metric_value(self, graph: OptGraph) -> float:
-        """
-        Method calculates metric for algorithm validation
-        
-        Args:
-          graph: Graph to evaluate
-
-        Returns:
-          value of loss function
-        """
-        graph_fitness = self.objective_evaluate(graph)
-        metric_value = graph_fitness.value
-        if not graph_fitness.valid:
-            return self._default_metric_value
-        return metric_value
-
     def init_check(self, graph: OptGraph) -> None:
         """
         Method get metric on validation set before start optimization
 
         Args:
           graph: graph to calculate objective
         """
         self.log.info('Hyperparameters optimization start: estimation of metric for initial graph')
 
         # Train graph
         self.init_graph = deepcopy(graph)
 
         self.init_metric = self.get_metric_value(graph=self.init_graph)
         self.log.message(f'Initial graph: {graph_structure(self.init_graph)} \n'
-                         f'Initial metric: {abs(self.init_metric):.3f}')
+                         f'Initial metric: '
+                         f'{list(map(lambda x: round(abs(x), 3), ensure_wrapped_in_sequence(self.init_metric)))}')
 
-    def final_check(self, tuned_graph: OptGraph) -> OptGraph:
+    def final_check(self, tuned_graphs: Union[OptGraph, Sequence[OptGraph]], multi_obj: bool = False) \
+            -> Union[OptGraph, Sequence[OptGraph]]:
         """
         Method propose final quality check after optimization process
 
         Args:
-          tuned_graph: Tuned graph to calculate objective
+          tuned_graphs: Tuned graph to calculate objective
+          multi_obj: If optimization was multi objective.
         """
+        self.log.info('Hyperparameters optimization finished')
 
-        self.obtained_metric = self.get_metric_value(graph=tuned_graph)
-
-        if self.obtained_metric == self._default_metric_value:
-            self.obtained_metric = None
+        if multi_obj:
+            return self._multi_obj_final_check(tuned_graphs)
+        else:
+            return self._single_obj_final_check(tuned_graphs)
 
-        self.log.info('Hyperparameters optimization finished')
+    def _single_obj_final_check(self, tuned_graph: OptGraph):
+        self.obtained_metric = self.get_metric_value(graph=tuned_graph)
 
         prefix_tuned_phrase = 'Return tuned graph due to the fact that obtained metric'
         prefix_init_phrase = 'Return init graph due to the fact that obtained metric'
 
+        if np.isclose(self.obtained_metric, self._default_metric_value):
+            self.obtained_metric = None
+
         # 0.05% deviation is acceptable
         deviation_value = (self.init_metric / 100.0) * self.deviation
         init_metric = self.init_metric + deviation_value * (-np.sign(self.init_metric))
         if self.obtained_metric is None:
             self.log.info(f'{prefix_init_phrase} is None. Initial metric is {abs(init_metric):.3f}')
             final_graph = self.init_graph
             final_metric = self.init_metric
@@ -142,16 +136,101 @@
                           f'worse than initial (+ {self.deviation}% deviation) {abs(init_metric):.3f}')
             final_graph = self.init_graph
             final_metric = self.init_metric
         self.log.message(f'Final graph: {graph_structure(final_graph)}')
         if final_metric is not None:
             self.log.message(f'Final metric: {abs(final_metric):.3f}')
         else:
-            self.log.message(f'Final metric is None')
+            self.log.message('Final metric is None')
         return final_graph
 
-    def _update_remaining_time(self, tuner_timer: Timer):
-        self.max_seconds = self.max_seconds - tuner_timer.minutes_from_start * 60
+    def _multi_obj_final_check(self, tuned_graphs: Sequence[OptGraph]) -> Sequence[OptGraph]:
+        self.obtained_metric = []
+        final_graphs = []
+        for tuned_graph in tuned_graphs:
+            obtained_metric = self.get_metric_value(graph=tuned_graph)
+            for e, value in enumerate(obtained_metric):
+                if np.isclose(value, self._default_metric_value):
+                    obtained_metric[e] = None
+            if not MultiObjFitness(self.init_metric).dominates(MultiObjFitness(obtained_metric)):
+                self.obtained_metric.append(obtained_metric)
+                final_graphs.append(tuned_graph)
+        if final_graphs:
+            metrics_formatted = [str([round(x, 3) for x in metrics]) for metrics in self.obtained_metric]
+            metrics_formatted = '\n'.join(metrics_formatted)
+            self.log.message('Return tuned graphs with obtained metrics \n'
+                             f'{metrics_formatted}')
+        else:
+            self.log.message('Initial metric dominates all found solutions. Return initial graph.')
+            final_graphs = self.init_graph
+        return final_graphs
+
+    def get_metric_value(self, graph: OptGraph) -> Union[float, Sequence[float]]:
+        """
+        Method calculates metric for algorithm validation
+
+        Args:
+          graph: Graph to evaluate
+
+        Returns:
+          value of loss function
+        """
+        graph_fitness = self.objective_evaluate(graph)
+
+        if isinstance(graph_fitness, SingleObjFitness):
+            metric_value = graph_fitness.value
+            if not graph_fitness.valid:
+                return self._default_metric_value
+            return metric_value
+
+        elif isinstance(graph_fitness, MultiObjFitness):
+            metric_values = graph_fitness.values
+            for e, value in enumerate(metric_values):
+                if value is None:
+                    metric_values[e] = self._default_metric_value
+            return metric_values
+
+    @staticmethod
+    def set_arg_graph(graph: OptGraph, parameters: dict) -> OptGraph:
+        """ Method for parameters setting to a graph
+
+        Args:
+            graph: graph to which parameters should be assigned
+            parameters: dictionary with parameters to set
+
+        Returns:
+            graph: graph with new hyperparameters in each node
+        """
+        # Set hyperparameters for every node
+        for node_id, node in enumerate(graph.nodes):
+            node_params = {key: value for key, value in parameters.items()
+                           if key.startswith(f'{str(node_id)} || {node.name}')}
+
+            if node_params is not None:
+                BaseTuner.set_arg_node(graph, node_id, node_params)
+
+        return graph
+
+    @staticmethod
+    def set_arg_node(graph: OptGraph, node_id: int, node_params: dict) -> OptGraph:
+        """ Method for parameters setting to a graph
+
+        Args:
+            graph: graph which contains the node
+            node_id: id of the node to which parameters should be assigned
+            node_params: dictionary with labeled parameters to set
+
+        Returns:
+            graph with new hyperparameters in each node
+        """
+
+        # Remove label prefixes
+        node_params = convert_parameters(node_params)
+
+        # Update parameters in nodes
+        graph.nodes[node_id].parameters = node_params
+
+        return graph
 
     def _stop_tuning_with_message(self, message: str):
         self.log.message(message)
         self.obtained_metric = self.init_metric
```

### Comparing `thegolem-0.3.1/golem/core/utilities/data_structures.py` & `thegolem-0.3.2/golem/core/utilities/data_structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import collections.abc
 
 from abc import ABC, abstractmethod
 from copy import deepcopy
 from enum import Enum
-from typing import Callable, Container, Generic, Iterable, Iterator, List, Optional, Sequence, Sized, TypeVar, Union
+from typing import Callable, Container, Generic, Iterable, Iterator, List, Optional, Sequence, Sized, TypeVar, Union, \
+    Tuple
 
 T = TypeVar('T')
 
 
 class UniqueList(list, Generic[T]):
     """
     Simple list that maintains uniqueness of elements.
@@ -299,7 +300,11 @@
     def __iter__(self):
         """
         Returns this iterator
 
         :return: this iterator
         """
         return self
+
+
+def unzip(tuples: Iterable[Tuple]) -> Tuple[Sequence, Sequence]:
+    return tuple(zip(*tuples))
```

### Comparing `thegolem-0.3.1/golem/core/utilities/grouped_condition.py` & `thegolem-0.3.2/golem/core/utilities/grouped_condition.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/utilities/random.py` & `thegolem-0.3.2/golem/core/utilities/random.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/utilities/sequence_iterator.py` & `thegolem-0.3.2/golem/core/utilities/sequence_iterator.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/utilities/serializable.py` & `thegolem-0.3.2/golem/core/utilities/serializable.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/core/utilities/singleton_meta.py` & `thegolem-0.3.2/golem/core/utilities/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/metrics/edit_distance.py` & `thegolem-0.3.2/golem/metrics/edit_distance.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 from datetime import timedelta, datetime
 from itertools import zip_longest
 from typing import Optional, Callable, Dict, Sequence
 
 import networkx as nx
 import numpy as np
 import zss
-from networkx import graph_edit_distance
+from networkx import graph_edit_distance, is_tree
 
 from examples.synthetic_graph_evolution.generators import generate_labeled_graph
 from golem.core.optimisers.optimization_parameters import GraphRequirements
 from golem.metrics.graph_metrics import min_max
 from libs.netcomp import edit_distance
 
 
 def _label_dist(label1: str, label2: str) -> int:
     return int(label1 != label2)
 
 
 def tree_edit_dist(target_graph: nx.DiGraph, graph: nx.DiGraph) -> float:
+    """Compares nodes by their `name` (if present) or `uid` attribute.
+    Nodes with the same name/id are considered the same."""
+    if not (is_tree(target_graph) and is_tree(graph)):
+        raise ValueError('Both target graphs must be trees')
     target_tree_root = _nx_to_zss_tree(target_graph)
     cmp_tree_root = _nx_to_zss_tree(graph)
     dist = zss.simple_distance(target_tree_root, cmp_tree_root, label_dist=_label_dist)
     return dist
 
 
+def graph_size(target_graph: nx.DiGraph, graph: nx.DiGraph) -> int:
+    return abs(target_graph.number_of_nodes() - graph.number_of_nodes())
+
+
 def _nx_to_zss_tree(graph: nx.DiGraph) -> zss.Node:
     # Root is the node without successors
     root = _get_root_node(graph)
     # that's why we first reverse the tree to get proper DFS traverse
     tree = graph.reverse()
     # Add nodes with appropriate labels for comparison
     nodes_dict = {}
@@ -59,15 +67,15 @@
         timeout = timeout or requirements.max_graph_fit_time
 
     def metric(graph: nx.DiGraph) -> float:
         ged = graph_edit_distance(target_graph, graph,
                                   node_match=node_match,
                                   upper_bound=upper_bound,
                                   timeout=timeout.total_seconds() if timeout else None,
-                                 )
+                                  )
         return float(ged) or upper_bound
 
     return metric
 
 
 def matrix_edit_dist(target_graph: nx.DiGraph, graph: nx.DiGraph) -> float:
     target_adj = nx.adjacency_matrix(target_graph)
@@ -103,9 +111,7 @@
         if print_trees:
             print(nx.forest_str(g1))
             print(nx.forest_str(g2))
 
 
 if __name__ == "__main__":
     try_tree_edit_distance(print_trees=False, node_types=list('XYZWQ'))
-
-
```

### Comparing `thegolem-0.3.1/golem/metrics/graph_features.py` & `thegolem-0.3.2/golem/metrics/graph_features.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/metrics/graph_metrics.py` & `thegolem-0.3.2/golem/metrics/graph_metrics.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/metrics/mmd.py` & `thegolem-0.3.2/golem/metrics/mmd.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/serializers/any_serialization.py` & `thegolem-0.3.2/golem/serializers/any_serialization.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/serializers/coders/graph_node_serialization.py` & `thegolem-0.3.2/golem/serializers/coders/graph_node_serialization.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/serializers/coders/opt_history_serialization.py` & `thegolem-0.3.2/golem/serializers/coders/opt_history_serialization.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 
 def _archive_to_uids(generations_list: List[List[Individual]]) -> List[List[str]]:
     return [[individual.uid for individual in generation] for generation in generations_list]
 
 
 def opt_history_to_json(obj: OptHistory) -> Dict[str, Any]:
     serialized = any_to_json(obj)
-    serialized['individuals_pool'] = _flatten_generations_list(serialized['individuals'])
-    serialized['individuals'] = _generations_list_to_uids(serialized['individuals'])
+    serialized['individuals_pool'] = _flatten_generations_list(serialized['_generations'])
+    serialized['_generations'] = _generations_list_to_uids(serialized['_generations'])
     serialized['archive_history'] = _archive_to_uids(serialized['archive_history'])
     return serialized
 
 
 def _uids_to_individuals(uid_sequence: Sequence[Union[str, Individual]],
                          uid_to_individual_map: Dict[str, Individual]) -> List[Individual]:
     def get_missing_individual(uid: str) -> Individual:
@@ -95,23 +95,27 @@
 
 def opt_history_from_json(cls: Type[OptHistory], json_obj: Dict[str, Any]) -> OptHistory:
     # backward compatibility with history._is_multi_objective field
     if '_is_multi_objective' in json_obj:
         json_obj['_objective'] = ObjectiveInfo(json_obj['_is_multi_objective'])
         del json_obj['_is_multi_objective']
 
+    # OptHistory.individuals are now OptHistory._generations
+    if 'individuals' in json_obj:
+        json_obj['_generations'] = json_obj.pop('individuals')
+
     history = any_from_json(cls, json_obj)
     # Read all individuals from history.
     individuals_pool = history.individuals_pool
     uid_to_individual_map = {ind.uid: ind for ind in individuals_pool}
     # The attributes `individuals` and `archive_history` at the moment contain uid strings that must be converted
     # to `Individual` instances.
-    _deserialize_generations_list(history.individuals, uid_to_individual_map)
+    _deserialize_generations_list(history.generations, uid_to_individual_map)
     _deserialize_generations_list(history.archive_history, uid_to_individual_map)
     # Process older histories to wrap generations into the new class.
-    if isinstance(history.individuals[0], list):
-        history.individuals = [Generation(gen, gen_num) for gen_num, gen in enumerate(history.individuals)]
+    if isinstance(history.generations[0], list):
+        history.generations = [Generation(gen, gen_num) for gen_num, gen in enumerate(history.generations)]
     # Deserialize parents for all generations.
-    _deserialize_parent_individuals(list(chain(*history.individuals)), uid_to_individual_map)
+    _deserialize_parent_individuals(list(chain(*history.generations)), uid_to_individual_map)
     # The attribute is used only for serialization.
     del history.individuals_pool
     return history
```

### Comparing `thegolem-0.3.1/golem/serializers/coders/parent_operator_serialization.py` & `thegolem-0.3.2/golem/serializers/coders/parent_operator_serialization.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/serializers/serializer.py` & `thegolem-0.3.2/golem/serializers/serializer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import json
 import os
 from importlib import import_module
 from inspect import isclass, isfunction, ismethod, signature
 from json import JSONDecoder, JSONEncoder
 from typing import Any, Callable, Dict, Optional, Type, TypeVar, Union
 
+from golem.core.dag.linked_graph import LinkedGraph
+from golem.core.dag.linked_graph_node import LinkedGraphNode
+from golem.core.log import default_log
+
 # NB: at the end of module init happens registration of default class coders
 
 INSTANCE_OR_CALLABLE = TypeVar('INSTANCE_OR_CALLABLE', object, Callable)
 EncodeCallable = Callable[[INSTANCE_OR_CALLABLE], Dict[str, Any]]
 DecodeCallable = Callable[[Type[INSTANCE_OR_CALLABLE], Dict[str, Any]], INSTANCE_OR_CALLABLE]
 
-
 MODULE_X_NAME_DELIMITER = '/'
 CLASS_PATH_KEY = '_class_path'
 
 # Mapping between class paths for backward compatibility for renamed/moved classes
 LEGACY_CLASS_PATHS = {
     'fedot.core.optimisers.gp_comp.individual/Individual':
         'golem.core.optimisers.opt_history_objects.individual/Individual',
@@ -52,15 +55,14 @@
     'fedot.core.adapter': 'golem.core.adapter',
     'fedot.core.dag': 'golem.core.dag',
     'fedot.core.utilities': 'golem.core.utilities',
 }
 
 
 class Serializer(JSONEncoder, JSONDecoder):
-
     _to_json = 'to_json'
     _from_json = 'from_json'
 
     CODERS_BY_TYPE = {}
 
     __default_coders_initialized = False
 
@@ -218,27 +220,41 @@
             if CLASS_PATH_KEY not in encoded:
                 encoded.update(Serializer.dump_path_to_obj(obj))
             return encoded
 
         return JSONEncoder.default(self, obj)
 
     @staticmethod
-    def _get_class(class_path: str) -> Type[INSTANCE_OR_CALLABLE]:
+    def _get_class(json_obj: dict) -> Optional[Type[INSTANCE_OR_CALLABLE]]:
         """
         Gets the object type from the class_path
 
         :param class_path: full path (module + name) of the class
 
         :return: class, function or method type
         """
+        class_path = json_obj[CLASS_PATH_KEY]
         class_path = LEGACY_CLASS_PATHS.get(class_path, class_path)
         module_name, class_name = class_path.split(MODULE_X_NAME_DELIMITER)
         module_name = Serializer._legacy_module_map(module_name)
 
-        obj_cls = import_module(module_name)
+        try:
+            obj_cls = import_module(module_name)
+        except ImportError as ex:
+            obj_cls = Serializer._import_as_base_class(json_obj)
+            if not obj_cls:
+                default_log('Serializer').info(
+                    f'Object was not decoded and will be stored as a dict '
+                    f'because of an ImportError: {ex}.')
+            else:
+                default_log('Serializer').info(
+                    f'Object was decoded as {obj_cls} and not as an original class '
+                    f'because of an ImportError: {ex}.')
+            return obj_cls
+
         for sub in class_name.split('.'):
             obj_cls = getattr(obj_cls, sub)
         return obj_cls
 
     @staticmethod
     def _legacy_module_map(module_path: str) -> str:
         for legacy_prefix, new_prefix in LEGACY_MODULE_PATHS.items():
@@ -247,51 +263,65 @@
         return module_path
 
     @staticmethod
     def _is_bound_method(method: Callable) -> bool:
         return hasattr(method, '__self__')
 
     @staticmethod
+    def _import_as_base_class(json_obj: dict) \
+            -> Optional[Union[Type[LinkedGraph], Type[LinkedGraphNode]]]:
+        linked_graph_keys = {'_nodes', '_postprocess_nodes'}
+        linked_node_keys = {'content', '_nodes_from', 'uid'}
+        if linked_graph_keys.issubset(json_obj.keys()):
+            return LinkedGraph
+        elif linked_node_keys.issubset(json_obj.keys()):
+            return LinkedGraphNode
+        else:
+            return None
+
+    @staticmethod
     def object_hook(json_obj: Dict[str, Any]) -> Union[INSTANCE_OR_CALLABLE, dict]:
         """
         Decodes every JSON-object to python class/func object or just returns dict
 
         :param json_obj: dict[str, Any] to be decoded into Python class, function or
             method object only if it has some special fields
 
         :return: Python class, function or method object OR input if it's just a regular dict
         """
         if CLASS_PATH_KEY in json_obj:
-            obj_cls = Serializer._get_class(json_obj[CLASS_PATH_KEY])
+            obj_cls = Serializer._get_class(json_obj)
             del json_obj[CLASS_PATH_KEY]
             base_type = Serializer._get_base_type(obj_cls)
             if isclass(obj_cls) and base_type is not None:
                 coder = Serializer._get_coder_by_type(base_type, Serializer._from_json)
                 # call with a right num of arguments
                 if Serializer._is_bound_method(coder):
                     return coder(json_obj)
                 else:
                     return coder(obj_cls, json_obj)
             elif isfunction(obj_cls) or ismethod(obj_cls):
                 return obj_cls
-            raise TypeError(f'Parsed obj_cls={obj_cls} is not serializable, but should be')
+            else:
+                return json_obj
         return json_obj
 
 
 def default_save(obj: Any, json_file_path: Optional[Union[str, os.PathLike]] = None) -> Optional[str]:
     """ Default save to json using Serializer """
     if json_file_path is None:
         return json.dumps(obj, indent=4, cls=Serializer)
     with open(json_file_path, mode='w') as json_file:
         json.dump(obj, json_file, indent=4, cls=Serializer)
         return None
 
 
 def default_load(json_str_or_file_path: Union[str, os.PathLike]) -> Any:
     """ Default load from json using Serializer """
+
     def load_as_file_path():
         with open(json_str_or_file_path, mode='r') as json_file:
             return json.load(json_file, cls=Serializer)
 
     def load_as_json_str():
         return json.loads(json_str_or_file_path, cls=Serializer)
```

### Comparing `thegolem-0.3.1/golem/structural_analysis/base_sa_approaches.py` & `thegolem-0.3.2/golem/structural_analysis/base_sa_approaches.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/structural_analysis/graph_sa/edge_sa_approaches.py` & `thegolem-0.3.2/golem/structural_analysis/graph_sa/edge_sa_approaches.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,16 +300,14 @@
 
         available_edges_idx = list()
 
         for parent_node in cur_graph.nodes[1:]:
             for child_node in cur_graph.nodes:
                 if parent_node == child_node:
                     continue
-                if parent_node == cur_graph.root_node:
-                    continue
                 if [parent_node, child_node] in edges_in_graph or [child_node, parent_node] in edges_in_graph:
                     continue
                 if cur_graph.nodes.index(parent_node) == child_node_index and \
                         cur_graph.nodes.index(child_node) == parent_node_index:
                     continue
                 available_edges_idx.append({'parent_node_idx': cur_graph.nodes.index(parent_node),
                                             'child_node_idx': cur_graph.nodes.index(child_node)})
```

### Comparing `thegolem-0.3.1/golem/structural_analysis/graph_sa/edges_analysis.py` & `thegolem-0.3.2/golem/structural_analysis/graph_sa/edges_analysis.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/structural_analysis/graph_sa/entities/edge.py` & `thegolem-0.3.2/golem/structural_analysis/graph_sa/entities/edge.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/structural_analysis/graph_sa/graph_structural_analysis.py` & `thegolem-0.3.2/golem/structural_analysis/graph_sa/graph_structural_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 from copy import deepcopy
-from typing import List, Optional, Tuple
+from pathlib import Path
+from typing import List, Optional, Tuple, Dict
 import multiprocessing
 
 from golem.core.log import default_log
 from golem.core.dag.graph import Graph, GraphNode
 from golem.core.optimisers.objective import Objective
 from golem.core.optimisers.opt_node_factory import OptNodeFactory
 from golem.core.optimisers.timer import OptimisationTimer
@@ -222,15 +223,15 @@
         :param node_size_scale: use to make node size bigger or lesser. Supported only for the engine 'matplotlib'.
         :param font_size_scale: use to make font size bigger or lesser. Supported only for the engine 'matplotlib'.
         :param edge_curvature_scale: use to make edges more or less curved. Supported only for the engine 'matplotlib'.
         :param dpi: DPI of the output image. Not supported for the engine 'pyvis'.
         """
 
         def get_nodes_and_edges_labels(analysis_result: SAAnalysisResults, iter: int) \
-                -> tuple[dict[int, str], dict[int, str]]:
+                -> Tuple[Dict[int, str], Dict[int, str]]:
             """ Get nodes and edges labels in dictionary form. """
 
             def get_str_labels(result: ObjectSAResult) -> str:
                 """ Get string results. """
                 approaches = result.result_approaches
                 cur_label = ''
                 for approach in approaches:
@@ -258,18 +259,24 @@
             iters = [0]
         else:
             iters = range(num_of_iter)
 
         for i in iters:
             nodes_labels, edges_labels = get_nodes_and_edges_labels(analysis_result=analysis_result, iter=i)
             if not (mode == 'final' and i != iters[-1]):
+                if not Path.is_file(Path(save_path)):
+                    j = 0
+                    while f'pipeline_after_sa_{j}.png' in os.listdir(save_path):
+                        j += 1
+                    cur_path = os.path.join(save_path, f'pipeline_after_sa_{j}.png')
                 graph.show(node_color=node_color, dpi=dpi, node_size_scale=node_size_scale,
                            nodes_labels=nodes_labels, font_size_scale=font_size_scale,
                            edge_curvature_scale=edge_curvature_scale,
-                           edges_labels=edges_labels, save_path=save_path)
+                           edges_labels=edges_labels, save_path=cur_path)
+                default_log("SA_visualization").info(f"SA visualization was saved to: {cur_path}")
             if mode == 'by_iteration':
                 graph = GraphStructuralAnalysis.apply_results(graph=graph, analysis_result=analysis_result,
                                                               metric_idx_to_optimize_by=metric_idx_to_optimize_by,
                                                               iter=i)
 
     @staticmethod
     def graph_preprocessing(graph: Graph) -> Graph:
```

### Comparing `thegolem-0.3.1/golem/structural_analysis/graph_sa/node_sa_approaches.py` & `thegolem-0.3.2/golem/structural_analysis/graph_sa/node_sa_approaches.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/structural_analysis/graph_sa/nodes_analysis.py` & `thegolem-0.3.2/golem/structural_analysis/graph_sa/nodes_analysis.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/structural_analysis/graph_sa/postproc_methods.py` & `thegolem-0.3.2/golem/structural_analysis/graph_sa/postproc_methods.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/structural_analysis/graph_sa/results/base_sa_approach_result.py` & `thegolem-0.3.2/golem/structural_analysis/graph_sa/results/base_sa_approach_result.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/structural_analysis/graph_sa/results/deletion_sa_approach_result.py` & `thegolem-0.3.2/golem/structural_analysis/graph_sa/results/deletion_sa_approach_result.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/structural_analysis/graph_sa/results/object_sa_result.py` & `thegolem-0.3.2/golem/structural_analysis/graph_sa/results/object_sa_result.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/structural_analysis/graph_sa/results/replace_sa_approach_result.py` & `thegolem-0.3.2/golem/structural_analysis/graph_sa/results/replace_sa_approach_result.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/structural_analysis/graph_sa/results/sa_analysis_results.py` & `thegolem-0.3.2/golem/structural_analysis/graph_sa/results/sa_analysis_results.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/structural_analysis/graph_sa/results/utils.py` & `thegolem-0.3.2/golem/structural_analysis/graph_sa/results/utils.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/structural_analysis/graph_sa/sa_approaches_repository.py` & `thegolem-0.3.2/golem/structural_analysis/graph_sa/sa_approaches_repository.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/structural_analysis/graph_sa/sa_requirements.py` & `thegolem-0.3.2/golem/structural_analysis/graph_sa/sa_requirements.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/utilities/memory.py` & `thegolem-0.3.2/golem/utilities/memory.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/utilities/profiler/memory_profiler.py` & `thegolem-0.3.2/golem/utilities/profiler/memory_profiler.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/utilities/profiler/time_profiler.py` & `thegolem-0.3.2/golem/utilities/profiler/time_profiler.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/utilities/requirements_notificator.py` & `thegolem-0.3.2/golem/utilities/requirements_notificator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from golem.core.log import default_log
 
 
-def warn_requirement(name: str, default_install_path: str = '.[extra]', *, should_raise: bool = False):
+def warn_requirement(name: str, default_install_path: str, *, should_raise: bool = False):
     """
     :param name: module name failed to load
+    :default_install_path: path to requirements than need to be installed
     :param should_raise: bool indicating if ImportError should be raised
     """
     msg = f'"{name}" is not installed, use "pip install {default_install_path}" to fulfil requirement'
     if should_raise:
         raise ImportError(msg)
     else:
         default_log(prefix='Requirements').debug(f'{msg} or ignore this warning')
```

### Comparing `thegolem-0.3.1/golem/visualisation/graph_viz.py` & `thegolem-0.3.2/golem/visualisation/graph_viz.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,23 +176,23 @@
         edge_curvature_scale = (edge_curvature_scale if edge_curvature_scale is not None
                                 else self.get_predefined_value('edge_curvature_scale'))
         graph_to_nx_convert_func = graph_to_nx_convert_func or self.get_predefined_value('graph_to_nx_convert_func')
 
         fig, ax = plt.subplots(figsize=(7, 7))
         fig.set_dpi(dpi)
 
-        self.draw_nx_dag(self.graph, ax, node_color, node_size_scale, font_size_scale, edge_curvature_scale,
+        self.draw_nx_dag(ax, node_color, node_size_scale, font_size_scale, edge_curvature_scale,
                          graph_to_nx_convert_func, nodes_labels, edges_labels)
         if not save_path:
             plt.show()
         else:
             plt.savefig(save_path, dpi=dpi)
             plt.close()
 
-    def draw_nx_dag(self, graph: GraphType, ax: Optional[plt.Axes] = None,
+    def draw_nx_dag(self, ax: Optional[plt.Axes] = None,
                     node_color: Optional[NodeColorType] = None,
                     node_size_scale: float = 1, font_size_scale: float = 1, edge_curvature_scale: float = 1,
                     graph_to_nx_convert_func: Callable = graph_structure_as_nx_graph,
                     nodes_labels: Dict[int, str] = None, edges_labels: Dict[int, str] = None):
 
         def draw_nx_labels(pos, node_labels, ax, max_sequence_length, font_size_scale=1.0):
             def get_scaled_font_size(nodes_amount):
@@ -215,15 +215,15 @@
             max_size = 5000
             size = min_size + int((max_size - min_size) / np.log2(max(nodes_amount, 2)))
             return size
 
         if ax is None:
             ax = plt.gca()
 
-        nx_graph, nodes = graph_to_nx_convert_func(graph)
+        nx_graph, nodes = graph_to_nx_convert_func(self.graph)
         # Define colors
         if callable(node_color):
             node_color = node_color([str(node) for node in nodes.values()])
         if isinstance(node_color, dict):
             node_color = [node_color.get(str(node), node_color.get(None)) for node in nodes.values()]
         # Define hierarchy_level
         for node_id, node_data in nx_graph.nodes(data=True):
```

### Comparing `thegolem-0.3.1/golem/visualisation/opt_history/arg_constraint_wrapper.py` & `thegolem-0.3.2/golem/visualisation/opt_history/arg_constraint_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     from golem.visualisation.opt_history.history_visualization import HistoryVisualization
 
 ArgConstraintChecker = Callable[..., Dict[str, Any]]
 
 
 def per_time(visualization: HistoryVisualization, **kwargs) -> Dict[str, Any]:
     value = kwargs.get('per_time')
-    if value and visualization.history.individuals[0][0].metadata.get('evaluation_time_iso') is None:
+    if value and visualization.history.generations[0][0].metadata.get('evaluation_time_iso') is None:
         visualization.log.warning('Evaluation time not found in optimization history. '
                                   'Showing fitness line per generations...')
         kwargs['per_time'] = False
     return kwargs
 
 
 def best_fraction(visualization: HistoryVisualization, **kwargs) -> Dict[str, Any]:
```

### Comparing `thegolem-0.3.1/golem/visualisation/opt_history/fitness_box.py` & `thegolem-0.3.2/golem/visualisation/opt_history/fitness_box.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         sns.boxplot(data=df_history, x='generation', y='fitness', palette=fitness.map(colormap), ax=ax)
         fig.set_dpi(dpi)
         fig.set_facecolor('w')
 
         ax.set_title('Fitness by generations')
         ax.set_xlabel('Generation')
         # Set ticks for every 5 generation if there's more than 10 generations.
-        if len(self.history.individuals) > 10:
+        if len(self.history.generations) > 10:
             ax.xaxis.set_major_locator(ticker.MultipleLocator(5))
             ax.xaxis.set_major_formatter(ticker.ScalarFormatter())
             ax.xaxis.grid(True)
         str_fraction_of_graphs = 'all' if best_fraction is None else f'top {best_fraction * 100}% of'
         ax.set_ylabel(f'Fitness of {str_fraction_of_graphs} generation graphs')
         ax.yaxis.grid(True)
```

### Comparing `thegolem-0.3.1/golem/visualisation/opt_history/graphs_interactive.py` & `thegolem-0.3.2/golem/visualisation/opt_history/graphs_interactive.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/visualisation/opt_history/history_visualization.py` & `thegolem-0.3.2/golem/visualisation/opt_history/history_visualization.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/visualisation/opt_history/operations_animated_bar.py` & `thegolem-0.3.2/golem/visualisation/opt_history/operations_animated_bar.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/golem/visualisation/opt_history/operations_kde.py` & `thegolem-0.3.2/golem/visualisation/opt_history/operations_kde.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,13 +66,13 @@
             palette=palette
         )
 
         fig = plot.figure
         fig.set_dpi(dpi)
         fig.set_facecolor('w')
         ax = plt.gca()
-        ax.set_xticks(range(len(self.history.individuals)))
+        ax.set_xticks(range(len(self.history.generations)))
         ax.locator_params(nbins=10)
         str_fraction_of_graphs = 'all' if best_fraction is None else f'top {best_fraction * 100}% of'
         ax.set_ylabel(f'Fraction in {str_fraction_of_graphs} generation graphs')
 
         show_or_save_figure(fig, save_path, dpi)
```

### Comparing `thegolem-0.3.1/golem/visualisation/opt_history/utils.py` & `thegolem-0.3.2/golem/visualisation/opt_history/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         history_data['tag'] = []
         new_map = {}
         for tag, operations in tags_map.items():
             new_map.update({operation: tag for operation in operations})
         tags_map = new_map
 
     uid_counts = {}  # Resolving individuals with the same uid
-    for gen_num, gen in enumerate(history.individuals):
+    for gen_num, gen in enumerate(history.generations):
         for ind in gen:
             uid_counts[ind.uid] = uid_counts.get(ind.uid, -1) + 1
             for node in ind.graph.nodes:
                 history_data['generation'].append(gen_num)
                 history_data['individual'].append('_'.join([ind.uid, str(uid_counts[ind.uid])]))
                 fitness = abs(ind.fitness.value)
                 history_data['fitness'].append(fitness)
```

### Comparing `thegolem-0.3.1/golem/visualisation/opt_viz.py` & `thegolem-0.3.2/golem/visualisation/opt_viz.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 from golem.core.log import default_log
+from golem.visualisation.opt_history.diversity import DiversityLine, DiversityPopulation
 from golem.visualisation.opt_history.fitness_box import FitnessBox
 from golem.visualisation.opt_history.fitness_line import FitnessLine, FitnessLineInteractive
 from golem.visualisation.opt_history.operations_animated_bar import OperationsAnimatedBar
 from golem.visualisation.opt_history.operations_kde import OperationsKDE
 
 if TYPE_CHECKING:
     from golem.core.optimisers.opt_history_objects.opt_history import OptHistory
@@ -15,14 +16,16 @@
 
 class PlotTypesEnum(Enum):
     fitness_box = FitnessBox
     fitness_line = FitnessLine
     fitness_line_interactive = FitnessLineInteractive
     operations_kde = OperationsKDE
     operations_animated_bar = OperationsAnimatedBar
+    diversity_line = DiversityLine
+    diversity_population = DiversityPopulation
 
     @classmethod
     def member_names(cls):
         return cls._member_names_
 
 
 class OptHistoryVisualizer:
@@ -51,14 +54,16 @@
         self.history = history
 
         self.fitness_box = FitnessBox(history, self.visuals_params).visualize
         self.fitness_line = FitnessLine(history, self.visuals_params).visualize
         self.fitness_line_interactive = FitnessLineInteractive(history, self.visuals_params).visualize
         self.operations_kde = OperationsKDE(history, self.visuals_params).visualize
         self.operations_animated_bar = OperationsAnimatedBar(history, self.visuals_params).visualize
+        self.diversity_line = DiversityLine(history, self.visuals_params).visualize
+        self.diversity_population = DiversityPopulation(history, self.visuals_params).visualize
 
         self.log = default_log(self)
 
     def __call__(self, plot_type: Union[PlotTypesEnum, str] = PlotTypesEnum.fitness_line, **kwargs):
         """ Visualizes the OptHistory with one of the supported methods.
 
         :param plot_type: visualization to show. Expected values are listed in
@@ -82,8 +87,7 @@
             except KeyError:
                 raise NotImplementedError(
                     f'Visualization "{plot_type}" is not supported. Expected values: '
                     f'{", ".join(PlotTypesEnum.member_names())}.')
         else:
             visualize_function = vars(self)[plot_type.name]
         visualize_function(**kwargs)
-
```

### Comparing `thegolem-0.3.1/golem/visualisation/opt_viz_extra.py` & `thegolem-0.3.2/golem/visualisation/opt_viz_extra.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,62 @@
 import itertools
 import os
 from copy import deepcopy
 from datetime import datetime
 from glob import glob
 from os import remove
-from typing import Any, List, Sequence, Tuple
+from typing import Any, List, Sequence, Tuple, Optional
 
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from matplotlib import pyplot as plt
 
 from golem.core.dag.graph import Graph
 from golem.core.log import default_log
 from golem.core.optimisers.opt_history_objects.individual import Individual
 from golem.core.optimisers.opt_history_objects.opt_history import OptHistory
 from golem.core.paths import default_data_dir
 from golem.visualisation.graph_viz import GraphVisualizer
-from golem.utilities.requirements_notificator import warn_requirement
-
-try:
-    import PIL
-    from PIL import Image
-except ModuleNotFoundError:
-    warn_requirement('Pillow')
-    PIL = None
+from PIL import Image
+from imageio import get_writer, v2
 
 
 class OptHistoryExtraVisualizer:
-    """ Implements legacy history visualizations that are not available via `history.show()` """
+    """ Implements legacy history visualizations that are not available via `history.show()`
+    Args:
+        history: history of optimisation
+        folder: path to folder to save results of visualization
+    """
 
-    def __init__(self):
-        data_dir = default_data_dir()
+    def __init__(self, history: OptHistory, folder: Optional[str] = None):
+        data_dir = folder or default_data_dir()
 
-        self.temp_path = os.path.join(data_dir, 'composing_history')
+        self.save_path = os.path.join(data_dir, 'composing_history')
         if 'composing_history' not in os.listdir(data_dir):
-            os.mkdir(self.temp_path)
+            os.mkdir(self.save_path)
+        self.history = history
         self.log = default_log(self)
         self.graphs_imgs = []
         self.convergence_imgs = []
         self.best_graphs_imgs = []
         self.merged_imgs = []
-        self.graph_visualizer = GraphVisualizer()
+        self.graph_visualizer = GraphVisualizer
 
-    def pareto_gif_create(self, pareto_fronts: List[List[Any]], individuals: List[List[Any]] = None,
-                          objectives_numbers: Tuple[int] = (1, 0),
-                          objectives_names: Tuple[str] = ('Complexity', 'ROC-AUC')):
+    def pareto_gif_create(self,
+                          objectives_numbers: Tuple[int, int] = (0, 1),
+                          objectives_names: Tuple[str] = ('ROC-AUC', 'Complexity')):
         files = []
+        pareto_fronts = self.history.archive_history
+        individuals = self.history.generations
         array_for_analysis = individuals if individuals else pareto_fronts
         all_objectives = extract_objectives(array_for_analysis, objectives_numbers)
         min_x, max_x = min(all_objectives[0]) - 0.01, max(all_objectives[0]) + 0.01
         min_y, max_y = min(all_objectives[1]) - 0.01, max(all_objectives[1]) + 0.01
-        folder = f'{self.temp_path}'
+        folder = f'{self.save_path}'
         for i, front in enumerate(pareto_fronts):
             file_name = f'pareto{i}.png'
             visualise_pareto(front, file_name=file_name, save=True, show=False,
                              folder=folder, generation_num=i, individuals=individuals[i],
                              minmax_x=[min_x, max_x], minmax_y=[min_y, max_y],
                              objectives_numbers=objectives_numbers,
                              objectives_names=objectives_names)
@@ -67,26 +68,26 @@
 
     def _visualise_graphs(self, graphs: List[Graph], fitnesses: List[float]):
         fitnesses = deepcopy(fitnesses)
         last_best_graph = graphs[0]
         prev_fit = fitnesses[0]
         fig = plt.figure(figsize=(10, 10))
         for ch_id, graph in enumerate(graphs):
-            self.graph_visualizer.draw_nx_dag(graph)
+            self.graph_visualizer(graph).draw_nx_dag()
             fig.canvas.draw()
             img = figure_to_array(fig)
             self.graphs_imgs.append(img)
             plt.clf()
             if fitnesses[ch_id] > prev_fit:
                 fitnesses[ch_id] = prev_fit
             else:
                 last_best_graph = graph
             prev_fit = fitnesses[ch_id]
             plt.clf()
-            self.graph_visualizer.draw_nx_dag(last_best_graph)
+            self.graph_visualizer(last_best_graph).draw_nx_dag()
             fig.canvas.draw()
             img = figure_to_array(fig)
             self.best_graphs_imgs.append(img)
             plt.clf()
         plt.close('all')
 
     def _visualise_convergence(self, fitness_history):
@@ -111,80 +112,77 @@
             plt.legend(loc='upper left')
             fig.canvas.draw()
             img = figure_to_array(fig)
             self.convergence_imgs.append(img)
             plt.clf()
         plt.close('all')
 
-    def visualise_history(self, history: OptHistory, metric_index: int = 0):
+    def visualise_history(self, metric_index: int = 0):
         try:
             self._clean(with_gif=True)
-            all_historical_fitness = history.all_historical_quality(metric_index)
+            all_historical_fitness = self.history.all_historical_quality(metric_index)
             historical_graphs = [ind.graph
-                                 for ind in list(itertools.chain(*history.individuals))]
+                                 for ind in list(itertools.chain(*self.history.generations))]
             self._visualise_graphs(historical_graphs, all_historical_fitness)
             self._visualise_convergence(all_historical_fitness)
             self._merge_images()
             self._combine_gifs()
             self._clean()
         except Exception as ex:
             self.log.error(f'Visualisation failed with {ex}')
 
     def _merge_images(self):
-        from PIL import Image
-
         for i in range(1, len(self.graphs_imgs)):
             im1 = self.graphs_imgs[i]
             im2 = self.best_graphs_imgs[i]
             im3 = self.convergence_imgs[i]
             imgs = (im1, im2, im3)
             merged = np.concatenate(imgs, axis=1)
             self.merged_imgs.append(Image.fromarray(np.uint8(merged)))
 
     def _combine_gifs(self):
-        date_time = datetime.now().strftime('%B-%d-%Y,%H-%M-%S,%p')
-        save_path = f'{self.temp_path}\\final_{date_time}.gif'
+        date_time = datetime.now().strftime('%B-%d-%Y_%H-%M-%S_%p')
+        save_path = os.path.join(self.save_path, f'history_visualisation_{date_time}.gif')
         imgs = self.merged_imgs[1:]
         self.merged_imgs[0].save(save_path, save_all=True, append_images=imgs,
                                  optimize=False, duration=0.5, loop=0)
         self.log.info(f"Visualizations were saved to {save_path}")
 
     def _clean(self, with_gif=False):
-        files = glob(f'{self.temp_path}*.png')
+        files = glob(f'{self.save_path}*.png')
         if with_gif:
-            files += glob(f'{self.temp_path}*.gif')
+            files += glob(f'{self.save_path}*.gif')
         for file in files:
             remove(file)
 
     def _create_boxplot(self, individuals: List[Any], generation_num: int = None,
                         objectives_names: Tuple[str] = ('ROC-AUC', 'Complexity'), file_name: str = 'obj_boxplots.png',
                         folder: str = None, y_limits: Tuple[float] = None):
-        folder = f'{self.temp_path}/boxplots' if folder is None else folder
+        folder = f'{self.save_path}/boxplots' if folder is None else folder
         fig, ax = plt.subplots()
         ax.set_title(f'Generation: {generation_num}', fontsize=15)
         objectives = objectives_lists(individuals)
         df_objectives = pd.DataFrame({objectives_names[i]: objectives[i] for i in range(len(objectives))})
         sns.boxplot(data=df_objectives, palette="Blues")
         if y_limits:
             plt.ylim(y_limits[0], y_limits[1])
         if not os.path.isdir('../../tmp'):
             os.mkdir('../../tmp')
         if not os.path.isdir(f'{folder}'):
             os.mkdir(f'{folder}')
         path = f'{folder}/{file_name}'
         plt.savefig(path, bbox_inches='tight')
 
-    def boxplots_gif_create(self, individuals: List[List[Any]],
-                            objectives_names: Tuple[str] = ('ROC-AUC', 'Complexity'),
-                            folder: str = None):
+    def boxplots_gif_create(self, objectives_names: Tuple[str] = ('ROC-AUC', 'Complexity')):
+        individuals = self.history.generations
         objectives = extract_objectives(individuals)
         objectives = list(itertools.chain(*objectives))
         min_y, max_y = min(objectives), max(objectives)
         files = []
-        folder = f'{self.temp_path}' if folder is None else folder
+        folder = f'{self.save_path}'
         for generation_num, individuals_in_genaration in enumerate(individuals):
             file_name = f'{generation_num}.png'
             self._create_boxplot(individuals_in_genaration, generation_num, objectives_names,
                                  file_name=file_name, folder=folder, y_limits=(min_y, max_y))
             files.append(f'{folder}/{file_name}')
         create_gif_using_images(gif_path=f'{folder}/boxplots_history.gif', files=files)
         for file in files:
@@ -194,15 +192,15 @@
         plt.close('all')
 
 
 def visualise_pareto(front: Sequence[Individual],
                      objectives_numbers: Tuple[int, int] = (0, 1),
                      objectives_names: Sequence[str] = ('ROC-AUC', 'Complexity'),
                      file_name: str = 'result_pareto.png', show: bool = False, save: bool = True,
-                     folder: str = f'../../tmp/pareto',
+                     folder: str = '../../tmp/pareto',
                      generation_num: int = None,
                      individuals: Sequence[Individual] = None,
                      minmax_x: List[float] = None,
                      minmax_y: List[float] = None):
     pareto_obj_first, pareto_obj_second = [], []
     for ind in front:
         fit_first = ind.fitness.values[objectives_numbers[0]]
@@ -250,23 +248,21 @@
 
     plt.cla()
     plt.clf()
     plt.close('all')
 
 
 def create_gif_using_images(gif_path: str, files: List[str]):
-    from imageio import get_writer, imread
-
     with get_writer(gif_path, mode='I', duration=0.5) as writer:
         for filename in files:
-            image = imread(filename)
+            image = v2.imread(filename)
             writer.append_data(image)
 
 
-def extract_objectives(individuals: List[List[Any]], objectives_numbers: Tuple[int] = None,
+def extract_objectives(individuals: List[List[Any]], objectives_numbers: Tuple[int, ...] = None,
                        transform_from_minimization=True):
     if not objectives_numbers:
         objectives_numbers = [i for i in range(len(individuals[0][0].fitness.values))]
     all_inds = list(itertools.chain(*individuals))
     all_objectives = [[ind.fitness.values[i] for ind in all_inds] for i in objectives_numbers]
     if transform_from_minimization:
         transformed_objectives = []
```

### Comparing `thegolem-0.3.1/libs/netcomp/eigenstuff.py` & `thegolem-0.3.2/libs/netcomp/eigenstuff.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/libs/netcomp/matrices.py` & `thegolem-0.3.2/libs/netcomp/matrices.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.3.1/setup.py` & `thegolem-0.3.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 # The directory containing this file
 HERE = Path(__file__).parent.resolve()
 
 # The text of the README file
 NAME = 'thegolem'
-VERSION = '0.3.1'
+VERSION = '0.3.2'
 AUTHOR = 'NSS Lab'
 SHORT_DESCRIPTION = 'Framework for Graph Optimization and Learning by Evolutionary Methods'
 
 README = Path(HERE, 'README_en.rst').read_text(encoding='utf-8')
 URL = 'https://github.com/aimclub/GOLEM'
 REQUIRES_PYTHON = '>=3.8'
 LICENSE = 'BSD 3-Clause'
@@ -45,15 +45,15 @@
     python_requires=REQUIRES_PYTHON,
     license=LICENSE,
     packages=setuptools.find_packages(exclude=['test*']),
     include_package_data=True,
     install_requires=_get_requirements('requirements.txt'),
     extras_require={
         key: _get_requirements(Path('other_requirements', f'{key}.txt'))
-        for key in ('docs', 'profilers')
+        for key in ('docs', 'profilers', 'molecules', 'adaptive')
     },
     classifiers=[
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10'
     ],
```

### Comparing `thegolem-0.3.1/thegolem.egg-info/PKG-INFO` & `thegolem-0.3.2/thegolem.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: thegolem
-Version: 0.3.1
+Version: 0.3.2
 Summary: Framework for Graph Optimization and Learning by Evolutionary Methods
 Home-page: https://github.com/aimclub/GOLEM
 Author: NSS Lab
 Author-email: itmo.nss.team@gmail.com
 License: BSD 3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: profilers
+Provides-Extra: molecules
+Provides-Extra: adaptive
 License-File: LICENSE
 
 .. image:: /docs/source/img/golem_logo-02.png
    :alt: Logo of GOLEM framework
    :align: center
    :width: 500
 
 .. class:: center
 
     |sai| |itmo|
 
-    |python| |pypi| |build| |docs| |license| |tg| |rus| |mirror|
+    |python| |pypi| |build| |integration| |docs| |license| |tg| |rus| |mirror|
 
 
 Graph Optimization and Learning by Evolutionary Methods
 -------------------------------------------------------
 
 GOLEM is an open-source AI framework for optimization and learning of structured graph-based models with meta-heuristic
 methods. It is centered around 2 ideas:
@@ -205,14 +207,18 @@
     :target: https://thegolem.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. |build| image:: https://github.com/aimclub/GOLEM/actions/workflows/unit-build.yml/badge.svg?branch=main
    :alt: Build Status
    :target: https://github.com/aimclub/GOLEM/actions/workflows/unit-build.yml
 
+.. |integration| image:: https://github.com/aimclub/GOLEM/actions/workflows/integration-build.yml/badge.svg?branch=main
+   :alt: Integration Build Status
+   :target: https://github.com/aimclub/GOLEM/actions/workflows/integration-build.yml
+
 .. |coverage| image:: https://codecov.io/gh/aimclub/GOLEM/branch/main/graph/badge.svg
    :alt: Coverage Status
    :target: https://codecov.io/gh/aimclub/GOLEM
 
 .. |pypi| image:: https://img.shields.io/pypi/v/thegolem.svg
    :alt: PyPI Package Version
    :target: https://img.shields.io/pypi/v/thegolem
```

### Comparing `thegolem-0.3.1/thegolem.egg-info/SOURCES.txt` & `thegolem-0.3.2/thegolem.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,23 +2,43 @@
 README.rst
 setup.py
 docs/__init__.py
 examples/__init__.py
 examples/graph_model_optimization.py
 examples/profiler_example.py
 examples/viz_with_labels.py
+examples/adaptive_optimizer/__init__.py
+examples/adaptive_optimizer/context_mab_experiment_different_targets.py
+examples/adaptive_optimizer/experiment_setup.py
+examples/adaptive_optimizer/mab_experiment_different_targets.py
+examples/adaptive_optimizer/neural_mab_experiment_different_targets.py
+examples/adaptive_optimizer/utils.py
+examples/molecule_search/__init__.py
+examples/molecule_search/constants.py
+examples/molecule_search/experiment.py
+examples/molecule_search/guacamol_benchmark.py
+examples/molecule_search/mol_adapter.py
+examples/molecule_search/mol_advisor.py
+examples/molecule_search/mol_graph.py
+examples/molecule_search/mol_graph_parameters.py
+examples/molecule_search/mol_metrics.py
+examples/molecule_search/mol_mutations.py
+examples/molecule_search/utils.py
 examples/structural_analysis/__init__.py
 examples/structural_analysis/opt_graph_optimization.py
 examples/synthetic_graph_evolution/__init__.py
-examples/synthetic_graph_evolution/experiment.py
+examples/synthetic_graph_evolution/experiment_setup.py
 examples/synthetic_graph_evolution/generators.py
 examples/synthetic_graph_evolution/graph_search.py
 examples/synthetic_graph_evolution/simple_run.py
 examples/synthetic_graph_evolution/tree_search.py
 examples/synthetic_graph_evolution/utils.py
+experiments/__init__.py
+experiments/mab/__init__.py
+experiments/mab/mab_synthetic_experiment_helper.py
 golem/__init__.py
 golem/core/__init__.py
 golem/core/constants.py
 golem/core/log.py
 golem/core/paths.py
 golem/core/adapter/__init__.py
 golem/core/adapter/adapt_registry.py
@@ -42,14 +62,22 @@
 golem/core/optimisers/opt_graph_builder.py
 golem/core/optimisers/opt_node_factory.py
 golem/core/optimisers/optimization_parameters.py
 golem/core/optimisers/optimizer.py
 golem/core/optimisers/populational_optimizer.py
 golem/core/optimisers/random_graph_factory.py
 golem/core/optimisers/timer.py
+golem/core/optimisers/adaptive/__init__.py
+golem/core/optimisers/adaptive/context_agents.py
+golem/core/optimisers/adaptive/neural_mab.py
+golem/core/optimisers/adaptive/operator_agent.py
+golem/core/optimisers/adaptive/mab_agents/__init__.py
+golem/core/optimisers/adaptive/mab_agents/contextual_mab_agent.py
+golem/core/optimisers/adaptive/mab_agents/mab_agent.py
+golem/core/optimisers/adaptive/mab_agents/neural_contextual_mab_agent.py
 golem/core/optimisers/archive/__init__.py
 golem/core/optimisers/archive/generation_keeper.py
 golem/core/optimisers/archive/individuals_containers.py
 golem/core/optimisers/fitness/__init__.py
 golem/core/optimisers/fitness/fitness.py
 golem/core/optimisers/fitness/multi_objective_fitness.py
 golem/core/optimisers/genetic/__init__.py
@@ -61,33 +89,41 @@
 golem/core/optimisers/genetic/operators/base_mutations.py
 golem/core/optimisers/genetic/operators/crossover.py
 golem/core/optimisers/genetic/operators/elitism.py
 golem/core/optimisers/genetic/operators/inheritance.py
 golem/core/optimisers/genetic/operators/mutation.py
 golem/core/optimisers/genetic/operators/operator.py
 golem/core/optimisers/genetic/operators/regularization.py
+golem/core/optimisers/genetic/operators/reproduction.py
 golem/core/optimisers/genetic/operators/selection.py
 golem/core/optimisers/genetic/parameters/__init__.py
 golem/core/optimisers/genetic/parameters/graph_depth.py
 golem/core/optimisers/genetic/parameters/mutation_prob.py
 golem/core/optimisers/genetic/parameters/operators_prob.py
 golem/core/optimisers/genetic/parameters/parameter.py
 golem/core/optimisers/genetic/parameters/population_size.py
+golem/core/optimisers/meta/__init__.py
+golem/core/optimisers/meta/surrogate_evaluator.py
+golem/core/optimisers/meta/surrogate_model.py
+golem/core/optimisers/meta/surrogate_optimizer.py
 golem/core/optimisers/objective/__init__.py
 golem/core/optimisers/objective/objective.py
 golem/core/optimisers/objective/objective_eval.py
 golem/core/optimisers/opt_history_objects/__init__.py
 golem/core/optimisers/opt_history_objects/generation.py
 golem/core/optimisers/opt_history_objects/individual.py
 golem/core/optimisers/opt_history_objects/opt_history.py
 golem/core/optimisers/opt_history_objects/parent_operator.py
 golem/core/optimisers/random/__init__.py
 golem/core/optimisers/random/random_mutation_optimizer.py
 golem/core/optimisers/random/random_search.py
 golem/core/tuning/__init__.py
+golem/core/tuning/hyperopt_tuner.py
+golem/core/tuning/iopt_tuner.py
+golem/core/tuning/optuna_tuner.py
 golem/core/tuning/search_space.py
 golem/core/tuning/sequential.py
 golem/core/tuning/simultaneous.py
 golem/core/tuning/tuner_interface.py
 golem/core/utilities/__init__.py
 golem/core/utilities/data_structures.py
 golem/core/utilities/grouped_condition.py
@@ -138,14 +174,15 @@
 golem/utilities/profiler/time_profiler.py
 golem/visualisation/__init__.py
 golem/visualisation/graph_viz.py
 golem/visualisation/opt_viz.py
 golem/visualisation/opt_viz_extra.py
 golem/visualisation/opt_history/__init__.py
 golem/visualisation/opt_history/arg_constraint_wrapper.py
+golem/visualisation/opt_history/diversity.py
 golem/visualisation/opt_history/fitness_box.py
 golem/visualisation/opt_history/fitness_line.py
 golem/visualisation/opt_history/graphs_interactive.py
 golem/visualisation/opt_history/history_visualization.py
 golem/visualisation/opt_history/operations_animated_bar.py
 golem/visualisation/opt_history/operations_kde.py
 golem/visualisation/opt_history/utils.py
```

