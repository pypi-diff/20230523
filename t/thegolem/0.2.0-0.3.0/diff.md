# Comparing `tmp/thegolem-0.2.0.tar.gz` & `tmp/thegolem-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/thegolem-0.2.0.tar", last modified: Fri Feb 17 05:49:44 2023, max compression
+gzip compressed data, was "thegolem-0.3.0.tar", last modified: Tue May 23 09:52:29 2023, max compression
```

## Comparing `thegolem-0.2.0.tar` & `thegolem-0.3.0.tar`

### file list

```diff
@@ -1,163 +1,197 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-02-17 05:49:40.000000 thegolem-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-02-17 05:49:44.000000 thegolem-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-02-17 05:49:40.000000 thegolem-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:40.000000 thegolem-0.2.0/docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:40.000000 thegolem-0.2.0/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-02-17 05:49:40.000000 thegolem-0.2.0/examples/graph_model_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-02-17 05:49:40.000000 thegolem-0.2.0/examples/profiler_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/examples/synthetic_graph_evolution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:40.000000 thegolem-0.2.0/examples/synthetic_graph_evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-02-17 05:49:40.000000 thegolem-0.2.0/examples/synthetic_graph_evolution/abstract_graph_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-02-17 05:49:40.000000 thegolem-0.2.0/examples/synthetic_graph_evolution/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/golem/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/golem/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/golem/core/adapter/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/adapter/adapt_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/adapter/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/adapter/nx_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/golem/core/dag/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/dag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/dag/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/dag/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/dag/graph_delegate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/dag/graph_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/dag/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/dag/graph_verifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/dag/linked_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/dag/linked_graph_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/dag/verification_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/golem/core/optimisers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/advisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/golem/core/optimisers/archive/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/archive/generation_keeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/archive/individuals_containers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/golem/core/optimisers/fitness/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/fitness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/fitness/fitness.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/fitness/multi_objective_fitness.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/golem/core/optimisers/genetic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/genetic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/genetic/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/genetic/gp_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/genetic/gp_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/genetic/gp_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/golem/core/optimisers/genetic/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/genetic/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/genetic/operators/crossover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/genetic/operators/elitism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/genetic/operators/inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)    17207 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/genetic/operators/mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/genetic/operators/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/genetic/operators/regularization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9331 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/genetic/operators/selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/golem/core/optimisers/genetic/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/genetic/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/genetic/parameters/graph_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/genetic/parameters/mutation_prob.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/genetic/parameters/operators_prob.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/genetic/parameters/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/genetic/parameters/population_size.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/graph_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/initial_graphs_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/golem/core/optimisers/objective/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/objective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/objective/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/objective/objective_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/opt_graph_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/golem/core/optimisers/opt_history_objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/opt_history_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/opt_history_objects/generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/opt_history_objects/individual.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/opt_history_objects/opt_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/opt_history_objects/parent_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/opt_node_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/optimization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/populational_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/golem/core/optimisers/random/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/random/random_mutation_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/random/random_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/random_graph_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/optimisers/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/golem/core/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/tuning/search_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/tuning/sequential.py
--rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/tuning/simultaneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/tuning/tuner_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/golem/core/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/utilities/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/utilities/grouped_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/utilities/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/utilities/sequence_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/utilities/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/core/utilities/singleton_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/golem/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/metrics/graph_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/metrics/graph_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/metrics/mmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/golem/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/serializers/any_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/golem/serializers/coders/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/serializers/coders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/serializers/coders/enum_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/serializers/coders/graph_node_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/serializers/coders/graph_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/serializers/coders/opt_history_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/serializers/coders/parent_operator_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/serializers/coders/uuid_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/serializers/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/golem/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/utilities/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/golem/utilities/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/utilities/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/utilities/profiler/memory_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/utilities/profiler/time_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/utilities/requirements_notificator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/golem/visualisation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16021 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/visualisation/graph_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/golem/visualisation/opt_history/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/visualisation/opt_history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/visualisation/opt_history/arg_constraint_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/visualisation/opt_history/fitness_box.py
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/visualisation/opt_history/fitness_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/visualisation/opt_history/graphs_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/visualisation/opt_history/history_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/visualisation/opt_history/operations_animated_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/visualisation/opt_history/operations_kde.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/visualisation/opt_history/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/visualisation/opt_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-02-17 05:49:40.000000 thegolem-0.2.0/golem/visualisation/opt_viz_extra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:40.000000 thegolem-0.2.0/libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/libs/netcomp/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-17 05:49:40.000000 thegolem-0.2.0/libs/netcomp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-02-17 05:49:40.000000 thegolem-0.2.0/libs/netcomp/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-02-17 05:49:40.000000 thegolem-0.2.0/libs/netcomp/eigenstuff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-02-17 05:49:40.000000 thegolem-0.2.0/libs/netcomp/matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 05:49:44.000000 thegolem-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-02-17 05:49:40.000000 thegolem-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 05:49:44.000000 thegolem-0.2.0/thegolem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-02-17 05:49:44.000000 thegolem-0.2.0/thegolem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-02-17 05:49:44.000000 thegolem-0.2.0/thegolem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 05:49:44.000000 thegolem-0.2.0/thegolem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-02-17 05:49:44.000000 thegolem-0.2.0/thegolem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-17 05:49:44.000000 thegolem-0.2.0/thegolem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.541627 thegolem-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-23 09:52:22.000000 thegolem-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-05-23 09:52:29.541627 thegolem-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17967 2023-05-23 09:52:22.000000 thegolem-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.505627 thegolem-0.3.0/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:22.000000 thegolem-0.3.0/docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.505627 thegolem-0.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:22.000000 thegolem-0.3.0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-23 09:52:22.000000 thegolem-0.3.0/examples/graph_model_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-23 09:52:22.000000 thegolem-0.3.0/examples/profiler_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.505627 thegolem-0.3.0/examples/structural_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:22.000000 thegolem-0.3.0/examples/structural_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-05-23 09:52:22.000000 thegolem-0.3.0/examples/structural_analysis/opt_graph_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.509627 thegolem-0.3.0/examples/synthetic_graph_evolution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:22.000000 thegolem-0.3.0/examples/synthetic_graph_evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-23 09:52:22.000000 thegolem-0.3.0/examples/synthetic_graph_evolution/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-23 09:52:22.000000 thegolem-0.3.0/examples/synthetic_graph_evolution/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-23 09:52:22.000000 thegolem-0.3.0/examples/synthetic_graph_evolution/graph_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-23 09:52:22.000000 thegolem-0.3.0/examples/synthetic_graph_evolution/simple_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-23 09:52:22.000000 thegolem-0.3.0/examples/synthetic_graph_evolution/tree_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-05-23 09:52:22.000000 thegolem-0.3.0/examples/synthetic_graph_evolution/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-23 09:52:22.000000 thegolem-0.3.0/examples/viz_with_labels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.509627 thegolem-0.3.0/golem/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.509627 thegolem-0.3.0/golem/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.509627 thegolem-0.3.0/golem/core/adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/adapter/adapt_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/adapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/adapter/nx_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.513627 thegolem-0.3.0/golem/core/dag/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/dag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/dag/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/dag/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/dag/graph_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/dag/graph_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/dag/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/dag/graph_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/dag/linked_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/dag/linked_graph_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/dag/verification_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.513627 thegolem-0.3.0/golem/core/optimisers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/advisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.513627 thegolem-0.3.0/golem/core/optimisers/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/archive/generation_keeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/archive/individuals_containers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.513627 thegolem-0.3.0/golem/core/optimisers/fitness/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/fitness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/fitness/fitness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/fitness/multi_objective_fitness.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.517627 thegolem-0.3.0/golem/core/optimisers/genetic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/genetic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/genetic/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/genetic/gp_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/genetic/gp_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/genetic/gp_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.517627 thegolem-0.3.0/golem/core/optimisers/genetic/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/genetic/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14366 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/genetic/operators/base_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/genetic/operators/crossover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/genetic/operators/elitism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/genetic/operators/inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/genetic/operators/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/genetic/operators/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/genetic/operators/regularization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9331 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/genetic/operators/selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.517627 thegolem-0.3.0/golem/core/optimisers/genetic/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/genetic/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/genetic/parameters/graph_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/genetic/parameters/mutation_prob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/genetic/parameters/operators_prob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/genetic/parameters/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/genetic/parameters/population_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/graph_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/initial_graphs_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.521627 thegolem-0.3.0/golem/core/optimisers/objective/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/objective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/objective/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/objective/objective_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/opt_graph_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.521627 thegolem-0.3.0/golem/core/optimisers/opt_history_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/opt_history_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/opt_history_objects/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/opt_history_objects/individual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/opt_history_objects/opt_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/opt_history_objects/parent_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/opt_node_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/optimization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/populational_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.521627 thegolem-0.3.0/golem/core/optimisers/random/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/random/random_mutation_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/random/random_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/random_graph_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/optimisers/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.521627 thegolem-0.3.0/golem/core/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/tuning/search_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/tuning/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8793 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/tuning/simultaneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/tuning/tuner_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.525627 thegolem-0.3.0/golem/core/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/utilities/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/utilities/grouped_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/utilities/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/utilities/sequence_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/utilities/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/core/utilities/singleton_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.525627 thegolem-0.3.0/golem/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/metrics/edit_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/metrics/graph_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/metrics/graph_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/metrics/mmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.525627 thegolem-0.3.0/golem/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/serializers/any_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.529627 thegolem-0.3.0/golem/serializers/coders/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/serializers/coders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/serializers/coders/enum_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/serializers/coders/graph_node_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/serializers/coders/graph_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/serializers/coders/opt_history_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/serializers/coders/parent_operator_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/serializers/coders/uuid_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/serializers/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.529627 thegolem-0.3.0/golem/structural_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/structural_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/structural_analysis/base_sa_approaches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.529627 thegolem-0.3.0/golem/structural_analysis/graph_sa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/structural_analysis/graph_sa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14396 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/structural_analysis/graph_sa/edge_sa_approaches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/structural_analysis/graph_sa/edges_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.529627 thegolem-0.3.0/golem/structural_analysis/graph_sa/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/structural_analysis/graph_sa/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/structural_analysis/graph_sa/entities/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/structural_analysis/graph_sa/graph_structural_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13975 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/structural_analysis/graph_sa/node_sa_approaches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/structural_analysis/graph_sa/nodes_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/structural_analysis/graph_sa/postproc_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.533627 thegolem-0.3.0/golem/structural_analysis/graph_sa/results/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/structural_analysis/graph_sa/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/structural_analysis/graph_sa/results/base_sa_approach_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/structural_analysis/graph_sa/results/deletion_sa_approach_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/structural_analysis/graph_sa/results/object_sa_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/structural_analysis/graph_sa/results/replace_sa_approach_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/structural_analysis/graph_sa/results/sa_analysis_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/structural_analysis/graph_sa/results/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/structural_analysis/graph_sa/sa_approaches_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/structural_analysis/graph_sa/sa_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.533627 thegolem-0.3.0/golem/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/utilities/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.533627 thegolem-0.3.0/golem/utilities/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/utilities/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/utilities/profiler/memory_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/utilities/profiler/time_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/utilities/requirements_notificator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.533627 thegolem-0.3.0/golem/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/visualisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20647 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/visualisation/graph_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.537627 thegolem-0.3.0/golem/visualisation/opt_history/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/visualisation/opt_history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/visualisation/opt_history/arg_constraint_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/visualisation/opt_history/fitness_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/visualisation/opt_history/fitness_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/visualisation/opt_history/graphs_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/visualisation/opt_history/history_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/visualisation/opt_history/operations_animated_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/visualisation/opt_history/operations_kde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/visualisation/opt_history/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/visualisation/opt_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-05-23 09:52:22.000000 thegolem-0.3.0/golem/visualisation/opt_viz_extra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.537627 thegolem-0.3.0/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:22.000000 thegolem-0.3.0/libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.537627 thegolem-0.3.0/libs/netcomp/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-23 09:52:22.000000 thegolem-0.3.0/libs/netcomp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-23 09:52:22.000000 thegolem-0.3.0/libs/netcomp/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-23 09:52:22.000000 thegolem-0.3.0/libs/netcomp/eigenstuff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-23 09:52:22.000000 thegolem-0.3.0/libs/netcomp/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 09:52:29.541627 thegolem-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-23 09:52:22.000000 thegolem-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:52:29.537627 thegolem-0.3.0/thegolem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-05-23 09:52:29.000000 thegolem-0.3.0/thegolem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-05-23 09:52:29.000000 thegolem-0.3.0/thegolem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:52:29.000000 thegolem-0.3.0/thegolem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-23 09:52:29.000000 thegolem-0.3.0/thegolem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-23 09:52:29.000000 thegolem-0.3.0/thegolem.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `thegolem-0.2.0/LICENSE` & `thegolem-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/README.rst` & `thegolem-0.3.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 .. image:: /docs/source/img/golem_logo-02.png
    :alt: Logo of GOLEM framework
    :align: center
    :width: 500
 
 .. class:: center
 
-    |python| |pypi| |build| |docs| |license| |tg| |eng|
+    |sai| |itmo|
+
+    |python| |pypi| |build| |docs| |license| |tg| |eng| |mirror|
 
 
 Оптимизация и обучение графовых моделей эволюционными методами
 --------------------------------------------------------------
 
 GOLEM - это фреймворк искусственного интеллекта с открытым исходным кодом для оптимизации и обучения структурированных
 моделей на основе графов с помощью метаэвристических методов. Он основан на двух идеях:
@@ -57,28 +59,58 @@
 - Автоматическое машинное обучение (AutoML) для поиска оптимальных пайплайнов машинного обучения в `фреймворке FEDOT <https://github.com/aimclub/FEDOT>`_
 - Поиск структуры при помощи байесовской сети в `фреймворке BAMT <https://github.com/ITMO-NSS-team/BAMT>`_
 - Поиск дифференциальных уравнений для физических моделей в рамках `фреймворка EPDE <https://github.com/ITMO-NSS-team/EPDE>`_
 - Геометрический дизайн физических объектов в рамках `фреймворка GEFEST <https://github.com/aimclub/GEFEST>`_
 - `Поиск архитектуры нейронных сетей <https://github.com/ITMO-NSS-team/nas-fedot>`_
 
 Поскольку GOLEM - это фреймворк общего назначения, легко представить его потенциальное применение, например,
-поиск конечных автоматов для управления в робототехнике или изучение молекулярных графов для разработки лекарств и
+поиск конечных автоматов для алгоритмов контроля в робототехнике или оптимизация молекулярных графов для разработки лекарств и
 многое другое.
 
 
 Установка
 =========
 
 GOLEM можно установить с помощью ``pip``:
 
 .. code-block::
 
   $ pip install thegolem
 
 
+Быстрый старт
+=============
+
+Следующий пример показывает поиск графа по графу-эталону с помощью метрики расстояния редактирования (Edit Distance). Оптимизатор настраивается с минимальным набором параметров и простыми одноточечными мутациями. Более подробные примеры можно найти в файлах `simple_run.py <https://github.com/aimclub/GOLEM/blob/main/examples/synthetic_graph_evolution/simple_run.py>`_, `graph_search.py <https://github.com/aimclub/GOLEM/blob/main/examples/synthetic_graph_evolution/graph_search.py>`_ и `tree_search.py <https://github.com/aimclub/GOLEM/blob/main/examples/synthetic_graph_evolution/tree_search.py>`_ в директории `examples/synthetic_graph_evolution <https://github.com/aimclub/GOLEM/tree/main/examples/synthetic_graph_evolution>`_.
+
+.. code-block::
+
+    def run_graph_search(size=16, timeout=8):
+        # Генерируем целевой граф и целевую функцию в виде edit distance
+        node_types = ('a', 'b')  # Available node types that can appear in graphs
+        target_graph = generate_labeled_graph('tree', size, node_types)
+        objective = Objective(partial(tree_edit_dist, target_graph))
+        initial_population = [generate_labeled_graph('tree', 5, node_types) for _ in range(10)]
+
+        # Укажем параметры оптимизации
+        requirements = GraphRequirements(timeout=timedelta(minutes=timeout))
+        gen_params = GraphGenerationParams(adapter=BaseNetworkxAdapter(), available_node_types=node_types)
+        algo_params = GPAlgorithmParameters(pop_size=30)
+
+        # Инициализируем оптимизатор и запустим оптимизацию
+        optimiser = EvoGraphOptimizer(objective, initial_population, requirements, gen_params, algo_params)
+        found_graphs = optimiser.optimise(objective)
+
+        # Визуализируем итоговый граф и график сходимости
+        found_graph = gen_params.adapter.restore(found_graphs[0])  # Transform back to NetworkX graph
+        draw_graphs_subplots(target_graph, found_graph, titles=['Target Graph', 'Found Graph'])
+        optimiser.history.show.fitness_line()
+        return found_graph
+
+
 Структура проекта
 =================
 
 Репозиторий включает в себя следующие пакеты и папки:
 
 - Пакет ``core`` содержит основные классы и скрипты.
 - Пакет ``core.adapter`` отвечает за преобразование между графами из предметной области и внутренним представлением, используемым оптимизаторами.
@@ -105,29 +137,27 @@
 
 Благодарности
 =============
 
 Мы благодарны контрибьютерам за их важный вклад, а участникам многочисленных конференций и семинаров -
 за их ценные советы и предложения.
 
-Разработка ведётся при поддержке
-================================
-
-.. image:: /docs/source/img/AIM-Strong_Sign_Norm-01_Colors.svg
-    :width: 400px
-    :align: center
-    :alt: Strong AI in industry logo
+Поддержка
+=========
 
-Разработка поддерживается исследовательским центром `Сильный искусственный интеллект в промышленности <https://sai.itmo.ru/>`__ `Университета ИТМО <https://itmo.ru/>`__.
+Исследование проводится при поддержке `Исследовательского центра сильного искусственного интеллекта в промышленности <https://sai.itmo.ru/>`_
+`Университета ИТМО <https://itmo.ru/>`_ в рамках мероприятия программы центра: Разработка и испытания 
+экспериментального образца библиотеки алгоритмов сильного ИИ в части базовых алгоритмов автоматического МО 
+для структурного обучения композитных моделей ИИ, включая автоматизацию отбора признаков
 
 Контакты
 ========
 - `Telegram канал <https://t.me/FEDOT_helpdesk>`_ для решения проблем и ответов на вопросы, связанные с FEDOT
-- `Команда Лаборатории моделирования естественных систем <https://itmo-nss-team.github.io/>`_
-- `Анна Калюжная <https://scholar.google.com/citations?user=bjiILqcAAAAJ&hl=ru>`_, тимлид (anna.kalyuzhnaya@itmo.ru)
+- `Команда Лаборатории моделирования природных систем <https://itmo-nss-team.github.io/>`_
+- `Николай Никитин <https://scholar.google.com/citations?user=eQBTGccAAAAJ&hl=ru>`_, руководитель направления AutoML (nnikitin@itmo.ru)
 - `Новости <https://t.me/NSS_group>`_
 - `Youtube канал <https://www.youtube.com/channel/UC4K9QWaEUpT_p3R4FeDp5jA>`_
 
 Цитирование
 ===========
 
 Если вы используете наш проект в своей работе или исследовании, мы будем признательны за цитирование.
@@ -136,24 +166,27 @@
   title = {Automated evolutionary approach for the design of composite machine learning pipelines},
   author = {Nikolay O. Nikitin and Pavel Vychuzhanin and Mikhail Sarafanov and Iana S. Polonskaia and Ilia Revin and Irina V. Barabanova and Gleb Maximov and Anna V. Kalyuzhnaya and Alexander Boukhanovsky},
   journal = {Future Generation Computer Systems},
   year = {2021},
   issn = {0167-739X},
   doi = {https://doi.org/10.1016/j.future.2021.08.022}}
 
-@inproceedings{polonskaia2021multi,
-  title={Multi-Objective Evolutionary Design of Composite Data-Driven Models},
-  author={Polonskaia, Iana S. and Nikitin, Nikolay O. and Revin, Ilia and Vychuzhanin, Pavel and Kalyuzhnaya, Anna V.},
-  booktitle={2021 IEEE Congress on Evolutionary Computation (CEC)},
-  year={2021},
-  pages={926-933},
-  doi={10.1109/CEC45853.2021.9504773}}
+Публикации, описывающие применение GOLEM для прикладных задач:
+==============================================================
+
+В данных публикациях описывается применение алгоритмов GOLEM и основанных на нем решений
+для различных прикладных задач.
 
+- Алгоритмы поиска оптимального пайплайна машинного обучения для прогнозирования временных рядов: Sarafanov M., Pokrovskii V., Nikitin N. O. Evolutionary Automated Machine Learning for Multi-Scale Decomposition and Forecasting of Sensor Time Series //2022 IEEE Congress on Evolutionary Computation (CEC). – IEEE, 2022. – С. 01-08.
 
-Другие статьи можно найти на `ResearchGate <https://www.researchgate.net/project/Evolutionary-multi-modal-AutoML-with-FEDOT-framework>`_.
+- Алгоритмы идентификации структуры уравнения для акустических данных: Hvatov A. Data-Driven Approach for the Floquet Propagator Inverse Problem Solution //ICASSP 2022-2022 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP). – IEEE, 2022. – С. 3813-3817.
+
+- Алгоритмы идентификации структуры дифференциальных уравнений в частных производных: Maslyaev M., Hvatov A. Solver-Based Fitness Function for the Data-Driven Evolutionary Discovery of Partial Differential Equations //2022 IEEE Congress on Evolutionary Computation (CEC). – IEEE, 2022. – С. 1-8.
+
+- Алгоритмы структурного обучения сетей: Deeva I., Kalyuzhnaya A. V., Alexander V. Boukhanovsky Adaptive Learning Algorithm for Bayesian Networks Based on Kernel Mixtures Distributions//International Journal of Artificial Intelligence. – 2023. - Т.21. - №. 1. - С. 90.
 
 .. |docs| image:: https://readthedocs.org/projects/thegolem/badge/?version=latest
     :target: https://thegolem.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. |build| image:: https://github.com/aimclub/GOLEM/actions/workflows/unit-build.yml/badge.svg?branch=main
    :alt: Build Status
@@ -183,8 +216,20 @@
    :target: https://t.me/FEDOT_helpdesk
 
 .. |by-golem| image:: http://img.shields.io/badge/powered%20by-GOLEM-orange.svg?style=flat
    :target: http://github.com/aimclub/GOLEM
    :alt: Powered by GOLEM
 
 .. |eng| image:: https://img.shields.io/badge/lang-en-red.svg
-            :target: /README_en.rst
+            :target: /README_en.rst
+
+.. |ITMO| image:: https://github.com/ITMO-NSS-team/open-source-ops/blob/add_badge/badges/ITMO_badge_rus.svg
+   :alt: Acknowledgement to ITMO
+   :target: https://itmo.ru
+
+.. |SAI| image:: https://github.com/ITMO-NSS-team/open-source-ops/blob/add_badge/badges/SAI_badge.svg
+   :alt: Acknowledgement to SAI
+   :target: https://sai.itmo.ru/
+
+.. |mirror| image:: https://camo.githubusercontent.com/9bd7b8c5b418f1364e72110a83629772729b29e8f3393b6c86bff237a6b784f6/68747470733a2f2f62616467656e2e6e65742f62616467652f6769746c61622f6d6972726f722f6f72616e67653f69636f6e3d6769746c6162
+   :alt: GitLab mirror for this repository
+   :target: https://gitlab.actcognitive.org/itmo-nss-team/GOLEM
```

### Comparing `thegolem-0.2.0/examples/graph_model_optimization.py` & `thegolem-0.3.0/examples/graph_model_optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         nodes = data.columns.to_list()
         _, labels = graph_structure_as_nx_graph(self)
         return len(nodes)
 
 
 class CustomGraphNode(OptNode):
     def __str__(self):
-        return f'Node_{self.content["name"]}'
+        return f'Node_{self.name}'
 
 
 def custom_metric(graph: CustomGraphModel, data: pd.DataFrame, visualisation: bool = False):
     if visualisation:
         graph.show()
     existing_variables_num = -graph.depth - graph.evaluate(data)
```

### Comparing `thegolem-0.2.0/examples/profiler_example.py` & `thegolem-0.3.0/examples/profiler_example.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/adapter/adapt_registry.py` & `thegolem-0.3.0/golem/core/adapter/adapt_registry.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/adapter/adapter.py` & `thegolem-0.3.0/golem/core/adapter/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self._log = default_log(self)
         self.domain_graph_class = base_graph_class
         self.opt_graph_class = OptGraph
 
     def restore_func(self, fun: Callable) -> Callable:
         """Wraps native function so that it could accept domain graphs as arguments.
 
-        Behavior: ``restore( f(OptGraph)->OptGraph ) => f'(DomainGraph)->DomainGraph``
+        Behavior: ``restore( f(Graph)->Graph ) => f'(DomainGraph)->DomainGraph``
 
         Implementation details.
         The method wraps callable into a function that transforms its args & return value.
         Arguments are transformed by ``adapt`` (that maps domain graphs to internal graphs).
         Return value is transformed by ``restore`` (that maps internal graphs to domain graphs).
 
         Args:
@@ -41,15 +41,15 @@
         return _transform(fun, f_args=self.adapt, f_ret=self.restore)
 
     def adapt_func(self, fun: Callable) -> Callable:
         """Wraps domain function so that it could accept native optimization graphs
         as arguments. If the function was registered as native, it is returned as-is.
         ``AdaptRegistry`` is responsible for function registration.
 
-        Behavior: ``adapt( f(DomainGraph)->DomainGraph ) => f'(OptGraph)->OptGraph``
+        Behavior: ``adapt( f(DomainGraph)->DomainGraph ) => f'(Graph)->Graph``
 
         Implementation details.
         The method wraps callable into a function that transforms its args & return value.
         Arguments are transformed by ``restore`` (that maps internal graphs to domain graphs).
         Return value is transformed by ``adapt`` (that maps domain graphs to internal graphs).
 
         Args:
@@ -60,94 +60,93 @@
             and be used inside Optimizer
         """
         if AdaptRegistry.is_native(fun):
             return fun
         return _transform(fun, f_args=self.restore, f_ret=self.adapt)
 
     def adapt(self, item: Union[DomainStructureType, Sequence[DomainStructureType]]) \
-            -> Union[OptGraph, Sequence[OptGraph]]:
+            -> Union[Graph, Sequence[Graph]]:
         """Maps domain graphs to internal graph representation used by optimizer.
         Performs mapping only if argument has a type of domain graph.
 
         Args:
             item: a domain graph or sequence of them
 
         Returns:
-            OptGraph | Sequence: mapped internal graph or sequence of them
+            Graph | Sequence: mapped internal graph or sequence of them
         """
         if type(item) is self.domain_graph_class:
             return self._adapt(item)
         elif isinstance(item, Sequence) and type(item[0]) is self.domain_graph_class:
             return [self._adapt(graph) for graph in item]
         else:
             return item
 
-    def restore(self, item: Union[OptGraph, Individual, PopulationT]) \
+    def restore(self, item: Union[Graph, Individual, PopulationT]) \
             -> Union[DomainStructureType, Sequence[DomainStructureType]]:
         """Maps graphs from internal representation to domain graphs.
         Performs mapping only if argument has a type of internal representation.
 
         Args:
             item: an internal graph representation or sequence of them
 
         Returns:
-            OptGraph | Sequence: mapped domain graph or sequence of them
+            Graph | Sequence: mapped domain graph or sequence of them
         """
         if type(item) is self.opt_graph_class:
             return self._restore(item)
         elif isinstance(item, Individual):
             return self._restore(item.graph, item.metadata)
         elif isinstance(item, Sequence) and isinstance(item[0], Individual):
             return [self._restore(ind.graph, ind.metadata) for ind in item]
         else:
             return item
 
     @abstractmethod
-    def _adapt(self, adaptee: DomainStructureType) -> OptGraph:
+    def _adapt(self, adaptee: DomainStructureType) -> Graph:
         """Implementation of ``adapt`` for single graph."""
         raise NotImplementedError()
 
     @abstractmethod
-    def _restore(self, opt_graph: OptGraph, metadata: Optional[Dict[str, Any]] = None) -> DomainStructureType:
+    def _restore(self, opt_graph: Graph, metadata: Optional[Dict[str, Any]] = None) -> DomainStructureType:
         """Implementation of ``restore`` for single graph."""
         raise NotImplementedError()
 
 
 class IdentityAdapter(BaseOptimizationAdapter[DomainStructureType]):
     """Identity adapter that performs no transformation, returning same graphs."""
 
-    def _adapt(self, adaptee: DomainStructureType) -> OptGraph:
+    def _adapt(self, adaptee: DomainStructureType) -> Graph:
         return adaptee
 
-    def _restore(self, opt_graph: OptGraph, metadata: Optional[Dict[str, Any]] = None) -> DomainStructureType:
+    def _restore(self, opt_graph: Graph, metadata: Optional[Dict[str, Any]] = None) -> DomainStructureType:
         return opt_graph
 
 
 class DirectAdapter(BaseOptimizationAdapter[DomainStructureType]):
     """Naive optimization adapter for arbitrary class that just overwrites __class__."""
 
     def __init__(self,
                  base_graph_class: Type[DomainStructureType] = OptGraph,
                  base_node_class: Type = OptNode):
         super().__init__(base_graph_class)
-        self._base_node_class = base_node_class
+        self.domain_node_class = base_node_class
 
-    def _adapt(self, adaptee: DomainStructureType) -> OptGraph:
+    def _adapt(self, adaptee: DomainStructureType) -> Graph:
         opt_graph = deepcopy(adaptee)
-        opt_graph.__class__ = OptGraph
-
+        opt_graph.__class__ = self.opt_graph_class
         for node in opt_graph.nodes:
             node.__class__ = OptNode
         return opt_graph
 
-    def _restore(self, opt_graph: OptGraph, metadata: Optional[Dict[str, Any]] = None) -> DomainStructureType:
+    def _restore(self, opt_graph: Graph, metadata: Optional[Dict[str, Any]] = None) -> DomainStructureType:
         obj = deepcopy(opt_graph)
         obj.__class__ = self.domain_graph_class
         for node in obj.nodes:
-            node.__class__ = self._base_node_class
+            node.__class__ = self.domain_node_class
         return obj
 
 
 def _transform(fun: Callable, f_args: Callable, f_ret: Callable) -> Callable:
     """Wraps function by transforming its arguments and return value:
      ``f_args`` is called on each of the function arguments,
      ``f_ret`` is called on the return value of original function.
```

### Comparing `thegolem-0.2.0/golem/core/adapter/nx_adapter.py` & `thegolem-0.3.0/golem/core/adapter/nx_adapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -81,30 +81,7 @@
     `OptNode` as an attribute of NetworkX graph node."""
 
     def _node_restore(self, node: GraphNode) -> Dict:
         return {_NX_NODE_KEY: node}
 
     def _node_adapt(self, data: Dict) -> OptNode:
         return data[_NX_NODE_KEY]
-
-
-def nx_to_directed(graph: nx.Graph) -> nx.DiGraph:
-    """Randomly chooses a direction for each edge."""
-    dedges = set()
-    digraph = nx.DiGraph()
-
-    for node, data in graph.nodes(data=True):
-        digraph.add_node(node, **data)
-
-    for u, v, data in graph.edges.data():
-        edge = (u, v)
-        inv_edge = (v, u)
-        if edge in dedges or inv_edge in dedges:
-            continue
-
-        if np.random.default_rng().random() > 0.5:
-            digraph.add_edge(*edge, **data)
-            dedges.add(edge)
-        else:
-            digraph.add_edge(*inv_edge, **data)
-            dedges.add(inv_edge)
-    return digraph
```

### Comparing `thegolem-0.2.0/golem/core/dag/convert.py` & `thegolem-0.3.0/golem/core/dag/convert.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/dag/graph.py` & `thegolem-0.3.0/golem/core/dag/graph.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 from abc import ABC, abstractmethod
+from enum import Enum
 from os import PathLike
 from typing import Dict, List, Optional, Sequence, Union, Tuple, TypeVar
 
 from golem.core.dag.graph_node import GraphNode
 from golem.visualisation.graph_viz import GraphVisualizer, NodeColorType
 
 NodeType = TypeVar('NodeType', bound=GraphNode, covariant=False, contravariant=False)
 
 
+class ReconnectType(Enum):
+    """Defines allowed kinds of removals in Graph. Used by mutations."""
+    none = 'none'  # do not reconnect predecessors
+    single = 'single'  # reconnect a predecessor only if it's single
+    all = 'all'  # reconnect all predecessors to all successors
+
+
 class Graph(ABC):
     """Defines abstract graph interface that's required by graph optimisation process.
     """
 
     @abstractmethod
     def add_node(self, node: GraphNode):
         """Adds new node to the graph together with its parent nodes.
@@ -37,20 +45,21 @@
         Args:
             old_subtree: node and its subtree to be removed
             new_subtree: node and its subtree to be placed instead
         """
         raise NotImplementedError()
 
     @abstractmethod
-    def delete_node(self, node: GraphNode):
+    def delete_node(self, node: GraphNode, reconnect: ReconnectType = ReconnectType.single):
         """Removes ``node`` from the graph.
         If ``node`` has only one child, then connects all of the ``node`` parents to it.
 
         Args:
             node: node of the graph to be deleted
+            reconnect: defines how to treat left edges between parents and children
         """
         raise NotImplementedError()
 
     @abstractmethod
     def delete_subtree(self, subtree: GraphNode):
         """Deletes given node with all its parents.
         Deletes all edges from removed nodes to remaining graph nodes
@@ -80,15 +89,15 @@
             node_parent: acts like parent in graph connection relations
             node_child:  acts like child in graph connection relations
         """
         raise NotImplementedError()
 
     @abstractmethod
     def disconnect_nodes(self, node_parent: GraphNode, node_child: GraphNode,
-                         clean_up_leftovers: bool = True):
+                         clean_up_leftovers: bool = False):
         """Removes an edge between two nodes
 
         Args:
             node_parent: where the removing edge comes out
             node_child: where the removing edge enters
             clean_up_leftovers: whether to remove the remaining invalid vertices with edges or not
         """
@@ -192,28 +201,34 @@
         """
 
         return len(self.nodes)
 
     def show(self, save_path: Optional[Union[PathLike, str]] = None, engine: Optional[str] = None,
              node_color: Optional[NodeColorType] = None, dpi: Optional[int] = None,
              node_size_scale: Optional[float] = None, font_size_scale: Optional[float] = None,
-             edge_curvature_scale: Optional[float] = None):
+             edge_curvature_scale: Optional[float] = None,
+             nodes_labels: Dict[int, str] = None, edges_labels: Dict[int, str] = None):
         """Visualizes graph or saves its picture to the specified ``path``
 
         Args:
             save_path: optional, save location of the graph visualization image.
             engine: engine to visualize the graph. Possible values: 'matplotlib', 'pyvis', 'graphviz'.
             node_color: color of nodes to use.
             node_size_scale: use to make node size bigger or lesser. Supported only for the engine 'matplotlib'.
             font_size_scale: use to make font size bigger or lesser. Supported only for the engine 'matplotlib'.
             edge_curvature_scale: use to make edges more or less curved. Supported only for the engine 'matplotlib'.
             dpi: DPI of the output image. Not supported for the engine 'pyvis'.
+            nodes_labels: labels to display near nodes
+            edges_labels: labels to display near edges
         """
-        GraphVisualizer(self).visualise(save_path, engine, node_color, dpi, node_size_scale, font_size_scale,
-                                        edge_curvature_scale)
+        GraphVisualizer(graph=self)\
+            .visualise(save_path=save_path, engine=engine, node_color=node_color, dpi=dpi,
+                       node_size_scale=node_size_scale, font_size_scale=font_size_scale,
+                       edge_curvature_scale=edge_curvature_scale,
+                       nodes_labels=nodes_labels, edges_labels=edges_labels)
 
     @property
     def graph_description(self) -> Dict:
         """Return summary characteristics of the graph
 
         Returns:
             dict: containing information about the graph
```

### Comparing `thegolem-0.2.0/golem/core/dag/graph_delegate.py` & `thegolem-0.3.0/golem/core/dag/graph_delegate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Union, Sequence, List, Optional, Tuple, Type
 
-from golem.core.dag.graph import Graph
+from golem.core.dag.graph import Graph, ReconnectType
 from golem.core.dag.graph_node import GraphNode
 from golem.core.dag.linked_graph import LinkedGraph
 
 
 class GraphDelegate(Graph):
     """
     Graph that delegates calls to another Graph implementation.
@@ -22,28 +22,28 @@
 
     def update_node(self, old_node: GraphNode, new_node: GraphNode):
         self.operator.update_node(old_node, new_node)
 
     def update_subtree(self, old_subtree: GraphNode, new_subtree: GraphNode):
         self.operator.update_subtree(old_subtree, new_subtree)
 
-    def delete_node(self, node: GraphNode):
-        self.operator.delete_node(node)
+    def delete_node(self, node: GraphNode, reconnect: ReconnectType = ReconnectType.single):
+        self.operator.delete_node(node, reconnect)
 
     def delete_subtree(self, subtree: GraphNode):
         self.operator.delete_subtree(subtree)
 
     def node_children(self, node: GraphNode) -> Sequence[Optional[GraphNode]]:
         return self.operator.node_children(node=node)
 
     def connect_nodes(self, node_parent: GraphNode, node_child: GraphNode):
         self.operator.connect_nodes(node_parent, node_child)
 
     def disconnect_nodes(self, node_parent: GraphNode, node_child: GraphNode,
-                         clean_up_leftovers: bool = True):
+                         clean_up_leftovers: bool = False):
         self.operator.disconnect_nodes(node_parent, node_child, clean_up_leftovers)
 
     def get_edges(self) -> Sequence[Tuple[GraphNode, GraphNode]]:
         return self.operator.get_edges()
 
     def __eq__(self, other) -> bool:
         return self.operator.__eq__(other)
```

### Comparing `thegolem-0.2.0/golem/core/dag/graph_node.py` & `thegolem-0.3.0/golem/core/dag/graph_node.py`

 * *Files 22% similar despite different names*

```diff
@@ -73,14 +73,15 @@
         Returns:
             str: text description of the content in the node and its parameters
         """
         return descriptive_id_recursive(self)
 
 
 def descriptive_id_recursive(current_node: GraphNode, visited_nodes=None) -> str:
+    """ Returns descriptive id with nodes names. """
     if visited_nodes is None:
         visited_nodes = []
 
     node_label = current_node.description()
 
     full_path_items = []
     if current_node in visited_nodes:
@@ -93,7 +94,25 @@
         previous_items.sort()
         previous_items_str = ';'.join(previous_items)
 
         full_path_items.append(f'({previous_items_str})')
     full_path_items.append(f'/{node_label}')
     full_path = ''.join(full_path_items)
     return full_path
+
+
+def descriptive_id_recursive_nodes(current_node: GraphNode, visited_nodes=None) -> List[GraphNode]:
+    """ Returns descriptive id with nodes, not with its names. """
+    if visited_nodes is None:
+        visited_nodes = []
+
+    full_path_items = []
+    if current_node in visited_nodes:
+        return []
+    visited_nodes.append(current_node)
+    if current_node.nodes_from:
+        previous_items = []
+        for parent_node in current_node.nodes_from:
+            previous_items.extend(descriptive_id_recursive_nodes(parent_node, copy(visited_nodes)))
+        full_path_items.extend(previous_items)
+    full_path_items.append(current_node)
+    return full_path_items
```

### Comparing `thegolem-0.2.0/golem/core/dag/graph_utils.py` & `thegolem-0.3.0/golem/core/dag/graph_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,31 +38,31 @@
         graph: graph with nodes
         layer_number: max height of diving
 
     Returns:
         all nodes from the surface to the ``layer_number`` layer
     """
 
-    def get_nodes(node: Union['GraphNode', List['GraphNode']], current_height: int):
-        """Gets all the parent nodes of ``node``
+    def get_nodes(roots: Sequence['GraphNode'], current_height: int) -> Sequence['GraphNode']:
+        """Gets all the parent nodes of ``roots``
 
-        :param node: node to get all subnodes from
+        :param roots: nodes to get all subnodes from
         :param current_height: current diving step depth
 
-        :return: all parent nodes of ``node``
+        :return: all parent nodes of ``roots`` in one sequence:69
         """
         nodes = []
         if current_height == layer_number:
-            nodes.append(node)
+            nodes.extend(roots)
         else:
-            for parent in node.nodes_from:
-                nodes.extend(get_nodes(parent, current_height + 1))
+            for root in roots:
+                nodes.extend(get_nodes(root.nodes_from, current_height + 1))
         return nodes
 
-    nodes = get_nodes(graph.root_node, current_height=0)
+    nodes = get_nodes(graph.root_nodes(), current_height=0)
     return nodes
 
 
 def ordered_subnodes_hierarchy(node: 'GraphNode') -> List['GraphNode']:
     """Gets hierarchical subnodes representation of the graph starting from the bounded node
 
     Returns:
```

### Comparing `thegolem-0.2.0/golem/core/dag/graph_verifier.py` & `thegolem-0.3.0/golem/core/dag/graph_verifier.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/dag/linked_graph.py` & `thegolem-0.3.0/golem/core/dag/linked_graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from copy import deepcopy
 from typing import Any, Dict, List, Optional, Tuple, Union, Callable, Sequence
 
 from networkx import graph_edit_distance, set_node_attributes
 
-from golem.core.dag.graph import Graph
+from golem.core.dag.graph import Graph, ReconnectType
 from golem.core.dag.graph_node import GraphNode
 from golem.core.dag.graph_utils import ordered_subnodes_hierarchy, node_depth
 from golem.core.dag.convert import graph_structure_as_nx_graph
 from golem.core.utilities.data_structures import ensure_wrapped_in_sequence, Copyable, remove_items
 from golem.core.paths import copy_doc
 
 NodePostprocessCallable = Callable[[Graph, Sequence[GraphNode]], Any]
@@ -30,26 +30,34 @@
         self._postprocess_nodes = postprocess_nodes or self._empty_postprocess
 
     @staticmethod
     def _empty_postprocess(*args):
         pass
 
     @copy_doc(Graph.delete_node)
-    def delete_node(self, node: GraphNode):
+    def delete_node(self, node: GraphNode, reconnect: ReconnectType = ReconnectType.single) -> object:
         node_children_cached = self.node_children(node)
-        self_root_node_cached = self.root_node
 
-        for node_child in self.node_children(node):
+        self._nodes.remove(node)
+        for node_child in node_children_cached:
             node_child.nodes_from.remove(node)
 
-        if node.nodes_from and len(node_children_cached) == 1:
-            for node_from in node.nodes_from:
-                node_children_cached[0].nodes_from.append(node_from)
-        self._nodes.clear()
-        self.add_node(self_root_node_cached)
+        if reconnect == ReconnectType.single:
+            # if removed node had a single child
+            # then reconnect it to preceding parent nodes.
+            if node.nodes_from and len(node_children_cached) == 1:
+                child = node_children_cached[0]
+                child.nodes_from.extend(node.nodes_from)
+        elif reconnect == ReconnectType.all:
+            if node.nodes_from:
+                for child in node_children_cached:
+                    child.nodes_from.extend(node.nodes_from)
+        elif reconnect == ReconnectType.none:
+            pass
+
         self._postprocess_nodes(self, self._nodes)
 
     @copy_doc(Graph.delete_subtree)
     def delete_subtree(self, subtree: GraphNode):
         subtree_nodes = ordered_subnodes_hierarchy(subtree)
         self._nodes = remove_items(self._nodes, subtree_nodes)
         # prune all edges coming from the removed subtree
@@ -94,14 +102,15 @@
     def sort_nodes(self):
         """ Layer by layer sorting """
         if not isinstance(self.root_node, Sequence):
             self._nodes = ordered_subnodes_hierarchy(self.root_node)
 
     @copy_doc(Graph.node_children)
     def node_children(self, node: GraphNode) -> List[Optional[GraphNode]]:
+        """ Returns list of children of specified node. """
         return [other_node for other_node in self._nodes
                 if other_node.nodes_from and
                 node in other_node.nodes_from]
 
     @copy_doc(Graph.connect_nodes)
     def connect_nodes(self, node_parent: GraphNode, node_child: GraphNode):
         if node_child in self.node_children(node_parent):
@@ -119,15 +128,15 @@
         if not self.node_children(node):
             self._nodes.remove(node)
             for node in node.nodes_from:
                 self._clean_up_leftovers(node)
 
     @copy_doc(Graph.disconnect_nodes)
     def disconnect_nodes(self, node_parent: GraphNode, node_child: GraphNode,
-                         clean_up_leftovers: bool = True):
+                         clean_up_leftovers: bool = False):
         if node_parent not in node_child.nodes_from:
             return
         if node_parent not in self._nodes or node_child not in self._nodes:
             return
         node_child.nodes_from.remove(node_parent)
         if clean_up_leftovers:
             self._clean_up_leftovers(node_parent)
```

### Comparing `thegolem-0.2.0/golem/core/dag/linked_graph_node.py` & `thegolem-0.3.0/golem/core/dag/linked_graph_node.py`

 * *Files 20% similar despite different names*

```diff
@@ -37,15 +37,16 @@
 
     @nodes_from.setter
     def nodes_from(self, nodes: Optional[Iterable['LinkedGraphNode']]):
         self._nodes_from = UniqueList(nodes)
 
     @property
     def name(self) -> str:
-        return str(self.content.get('name'))
+        name = self.content.get('name')
+        return str(name) if name is not None else ''
 
     @property
     def parameters(self) -> dict:
         return self.content.get('params', {})
 
     @parameters.setter
     def parameters(self, new_parameters):
@@ -60,20 +61,18 @@
     def __str__(self) -> str:
         return str(self.content.get('name', self.uid))
 
     def __repr__(self) -> str:
         return self.__str__()
 
     def description(self) -> str:
-        node_operation = self.content.get('name')
-        if node_operation is None:
-            raise ValueError('Unknown content in the node: expected content[`name`], got None')
+        label = self.name or self.uid
         # TODO: possibly unify with __repr__ & don't duplicate Operation.description
         if not self.parameters:
-            node_label = f'n_{node_operation}'
-        elif isinstance(node_operation, str):
+            node_label = f'n_{label}'
+        elif isinstance(label, str):
             # If there is a string: name of operation (as in json repository)
-            node_label = f'n_{node_operation}_{self.parameters}'
+            node_label = f'n_{label}_{self.parameters}'
         else:
             # If instance of Operation is placed in 'name'
-            node_label = node_operation.description(self.parameters)
+            node_label = label.description(self.parameters)
         return node_label
```

### Comparing `thegolem-0.2.0/golem/core/dag/verification_rules.py` & `thegolem-0.3.0/golem/core/dag/verification_rules.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 import networkx as nx
 from networkx import isolates, simple_cycles
 
 from golem.core.adapter import register_native
 from golem.core.dag.convert import graph_structure_as_nx_graph
 from golem.core.dag.graph import Graph
+from golem.core.dag.graph_node import GraphNode
 
 ERROR_PREFIX = 'Invalid graph configuration:'
 
 
 @register_native
-def has_one_root(graph: Graph):
+def has_root(graph: Graph):
     if graph.root_node:
         return True
 
 
 @register_native
+def has_one_root(graph: Graph):
+    if isinstance(graph.root_node, GraphNode):
+        return True
+
+
+@register_native
 def has_no_cycle(graph: Graph):
     nx_graph, _ = graph_structure_as_nx_graph(graph)
     cycled = list(simple_cycles(nx_graph))
     if len(cycled) > 0:
         raise ValueError(f'{ERROR_PREFIX} Graph has cycles')
 
     return True
@@ -42,14 +49,16 @@
 
 @register_native
 def has_no_isolated_components(graph: Graph):
     nx_graph, _ = graph_structure_as_nx_graph(graph)
     ud_nx_graph = nx.Graph()
     ud_nx_graph.add_nodes_from(nx_graph)
     ud_nx_graph.add_edges_from(nx_graph.edges)
+    if ud_nx_graph.number_of_nodes() == 0:
+        raise ValueError(f'{ERROR_PREFIX} Graph is null, connectivity not defined')
     if not nx.is_connected(ud_nx_graph):
         raise ValueError(f'{ERROR_PREFIX} Graph has isolated components')
     return True
 
 
-DEFAULT_DAG_RULES = [has_one_root, has_no_cycle, has_no_isolated_components,
+DEFAULT_DAG_RULES = [has_root, has_no_cycle, has_no_isolated_components,
                      has_no_self_cycled_nodes, has_no_isolated_nodes]
```

### Comparing `thegolem-0.2.0/golem/core/log.py` & `thegolem-0.3.0/golem/core/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,16 @@
     def reset_logging_level(self, logging_level: int):
         """ Resets logging level for logger and its handlers """
         # Resets logging level is needed because before initialization with API params Singleton
         # can be initialized somewhere else with default ones
         self.logger.setLevel(logging_level)
         for handler in self.handlers:
             handler.setLevel(logging_level)
+        for adapter in self.__log_adapters.values():
+            adapter.logging_level = logging_level
 
     def get_adapter(self, prefix: str) -> 'LoggerAdapter':
         """ Get adapter to pass contextual information to log messages
 
         Args:
             prefix: prefix to log messages with this adapter. Usually, the prefix is the name of the class
                 where the log came from
```

### Comparing `thegolem-0.2.0/golem/core/optimisers/advisor.py` & `thegolem-0.3.0/golem/core/optimisers/advisor.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 
 from golem.core.optimisers.graph import OptNode
 from golem.core.utilities.data_structures import ComparableEnum as Enum
 
 
 class RemoveType(Enum):
     """Defines allowed kinds of removals in Graph. Used by mutations."""
+    forbidden = 'forbidden'
     node_only = 'node_only'
+    node_rewire = 'node_rewire'
     with_direct_children = 'with_direct_children'
     with_parents = 'with_parents'
-    forbidden = 'forbidden'
 
 
 class DefaultChangeAdvisor:
     """
     Class for advising of graph changes during evolution
     """
 
     def __init__(self, task=None):
         self.task = task
 
     def propose_change(self, node: OptNode, possible_operations: List[Any]) -> List[Any]:
         return possible_operations
 
     def can_be_removed(self, node: OptNode) -> RemoveType:
-        return RemoveType.node_only
+        return RemoveType.node_rewire
 
     def propose_parent(self, node: OptNode, possible_operations: List[Any]) -> List[Any]:
         return possible_operations
```

### Comparing `thegolem-0.2.0/golem/core/optimisers/archive/generation_keeper.py` & `thegolem-0.3.0/golem/core/optimisers/archive/generation_keeper.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/archive/individuals_containers.py` & `thegolem-0.3.0/golem/core/optimisers/archive/individuals_containers.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/fitness/fitness.py` & `thegolem-0.3.0/golem/core/optimisers/fitness/fitness.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/fitness/multi_objective_fitness.py` & `thegolem-0.3.0/golem/core/optimisers/fitness/multi_objective_fitness.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/genetic/evaluation.py` & `thegolem-0.3.0/golem/core/optimisers/genetic/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,17 +236,19 @@
         individuals_evaluated = self.apply_evaluation_results(individuals_to_evaluate, evaluation_results)
         # If there were no successful evals then try once again getting at least one,
         # even if time limit was reached
         successful_evals = individuals_evaluated + individuals_to_skip
         self.population_evaluation_info(evaluated_pop_size=len(successful_evals),
                                         pop_size=len(individuals))
         if not successful_evals:
-            single_ind = choice(individuals)
-            evaluation_result = eval_func(single_ind.graph, single_ind.uid, with_time_limit=False)
-            successful_evals = self.apply_evaluation_results([single_ind], [evaluation_result]) or None
+            for single_ind in individuals:
+                evaluation_result = eval_func(single_ind.graph, single_ind.uid, with_time_limit=False)
+                successful_evals = self.apply_evaluation_results([single_ind], [evaluation_result]) or None
+                if successful_evals:
+                    break
         MemoryAnalytics.log(self.logger,
                             additional_info='parallel evaluation of population',
                             logging_level=logging.INFO)
         return successful_evals
 
     def evaluate_single(self, graph: OptGraph, uid_of_individual: str, with_time_limit: bool = True,
                         cache_key: Optional[str] = None,
```

### Comparing `thegolem-0.2.0/golem/core/optimisers/genetic/gp_optimizer.py` & `thegolem-0.3.0/golem/core/optimisers/genetic/gp_optimizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from copy import deepcopy
 from random import choice
-from typing import Sequence, Callable
+from typing import Sequence, Callable, Union, Any
 
 from golem.core.constants import MAX_GRAPH_GEN_ATTEMPTS
 from golem.core.dag.graph import Graph
 from golem.core.optimisers.genetic.gp_params import GPAlgorithmParameters
 from golem.core.optimisers.genetic.operators.crossover import Crossover
 from golem.core.optimisers.genetic.operators.elitism import Elitism
 from golem.core.optimisers.genetic.operators.inheritance import Inheritance
@@ -12,15 +12,14 @@
 from golem.core.optimisers.genetic.operators.operator import PopulationT, EvaluationOperator
 from golem.core.optimisers.genetic.operators.regularization import Regularization
 from golem.core.optimisers.genetic.operators.selection import Selection
 from golem.core.optimisers.genetic.parameters.graph_depth import AdaptiveGraphDepth
 from golem.core.optimisers.genetic.parameters.operators_prob import init_adaptive_operators_prob
 from golem.core.optimisers.genetic.parameters.population_size import init_adaptive_pop_size, PopulationSize
 from golem.core.optimisers.optimization_parameters import GraphRequirements
-from golem.core.optimisers.graph import OptGraph
 from golem.core.optimisers.objective.objective import Objective
 from golem.core.optimisers.opt_history_objects.individual import Individual
 from golem.core.optimisers.optimizer import GraphGenerationParams
 from golem.core.optimisers.populational_optimizer import PopulationalOptimizer, EvaluationAttemptsError
 
 
 EVALUATION_ATTEMPTS_NUMBER = 5
@@ -29,15 +28,15 @@
 class EvoGraphOptimizer(PopulationalOptimizer):
     """
     Multi-objective evolutionary graph optimizer named GPComp
     """
 
     def __init__(self,
                  objective: Objective,
-                 initial_graphs: Sequence[OptGraph],
+                 initial_graphs: Sequence[Union[Graph, Any]],
                  requirements: GraphRequirements,
                  graph_generation_params: GraphGenerationParams,
                  graph_optimizer_params: GPAlgorithmParameters):
         super().__init__(objective, initial_graphs, requirements, graph_generation_params, graph_optimizer_params)
         # Define genetic operators
         self.regularization = Regularization(graph_optimizer_params, graph_generation_params)
         self.selection = Selection(graph_optimizer_params)
@@ -57,56 +56,56 @@
                                                max_stagnation_gens=graph_optimizer_params.adaptive_depth_max_stagnation,
                                                adaptive=graph_optimizer_params.adaptive_depth)
 
         # Define initial parameters
         self.requirements.max_depth = self._graph_depth.initial
         self.graph_optimizer_params.pop_size = self._pop_size.initial
         self.initial_individuals = [Individual(graph, metadata=requirements.static_individual_metadata)
-                                    for graph in initial_graphs]
+                                    for graph in self.initial_graphs]
 
     def _initial_population(self, evaluator: EvaluationOperator):
         """ Initializes the initial population """
         # Adding of initial assumptions to history as zero generation
         self._update_population(evaluator(self.initial_individuals), 'initial_assumptions')
 
         if len(self.initial_individuals) < self.graph_optimizer_params.pop_size:
             self.initial_individuals = self._extend_population(self.initial_individuals)
             # Adding of extended population to history
             self._update_population(evaluator(self.initial_individuals), 'extended_initial_assumptions')
 
     def _extend_population(self, initial_individuals: PopulationT) -> PopulationT:
-        iter_num = 0
         initial_individuals = list(initial_individuals)
         initial_graphs = [ind.graph for ind in initial_individuals]
         initial_req = deepcopy(self.requirements)
         initial_req.mutation_prob = 1
         self.mutation.update_requirements(requirements=initial_req)
-        while len(initial_individuals) < self.graph_optimizer_params.pop_size:
+
+        for iter_num in range(MAX_GRAPH_GEN_ATTEMPTS):
+            if len(initial_individuals) == self.graph_optimizer_params.pop_size:
+                break
             new_ind = self.mutation(choice(self.initial_individuals))
             new_graph = new_ind.graph
-            iter_num += 1
             if new_graph not in initial_graphs and self.graph_generation_params.verifier(new_graph):
                 initial_individuals.append(new_ind)
                 initial_graphs.append(new_graph)
-            if iter_num > MAX_GRAPH_GEN_ATTEMPTS:
-                self.log.warning(f'Exceeded max number of attempts for extending initial graphs, stopping.'
-                                 f'Current size {len(self.initial_individuals)} '
-                                 f'instead of {self.graph_optimizer_params.pop_size} graphs.')
-                break
+        else:
+            self.log.warning(f'Exceeded max number of attempts for extending initial graphs, stopping.'
+                             f'Current size {len(self.initial_individuals)} '
+                             f'instead of {self.graph_optimizer_params.pop_size} graphs.')
+
         self.mutation.update_requirements(requirements=self.requirements)
         return initial_individuals
 
     def _evolve_population(self, evaluator: EvaluationOperator) -> PopulationT:
         """ Method realizing full evolution cycle """
         self._update_requirements()
 
         individuals_to_select = self.regularization(self.population, evaluator)
         selected_individuals = self.selection(individuals_to_select)
-        new_population = self._spawn_evaluated_population(selected_individuals=selected_individuals,
-                                                          evaluator=evaluator)
+        new_population = self._spawn_evaluated_population(selected_individuals, evaluator)
         new_population = self.inheritance(self.population, new_population)
         new_population = self.elitism(self.generations.best_individuals, new_population)
 
         return new_population
 
     def _update_requirements(self):
         if not self.generations.is_any_improved:
@@ -122,23 +121,16 @@
         for operator in self.operators:
             operator.update_requirements(self.graph_optimizer_params, self.requirements)
 
     def _spawn_evaluated_population(self, selected_individuals: PopulationT, evaluator: Callable) -> PopulationT:
         """ Reproduce and evaluate new population. If at least one of received individuals can not be evaluated then
         mutate and evaluate selected individuals until a new population is obtained
         or the number of attempts is exceeded """
-
-        iter_num = 0
-        new_population = None
-        while not new_population:
+        for i in range(EVALUATION_ATTEMPTS_NUMBER):
             new_population = self.crossover(selected_individuals)
             new_population = self.mutation(new_population)
             new_population = evaluator(new_population)
-
-            if iter_num > EVALUATION_ATTEMPTS_NUMBER:
-                break
-            iter_num += 1
-
-        if not new_population:
+            if new_population:
+                return new_population
+        else:
+            # Could not generate valid population; raise an error
             raise EvaluationAttemptsError()
-
-        return new_population
```

### Comparing `thegolem-0.2.0/golem/core/optimisers/genetic/operators/elitism.py` & `thegolem-0.3.0/golem/core/optimisers/genetic/operators/elitism.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/genetic/operators/inheritance.py` & `thegolem-0.3.0/golem/core/optimisers/genetic/operators/inheritance.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/genetic/operators/operator.py` & `thegolem-0.3.0/golem/core/optimisers/genetic/operators/operator.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/genetic/operators/regularization.py` & `thegolem-0.3.0/golem/core/optimisers/genetic/operators/regularization.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/genetic/operators/selection.py` & `thegolem-0.3.0/golem/core/optimisers/genetic/operators/selection.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/genetic/parameters/graph_depth.py` & `thegolem-0.3.0/golem/core/optimisers/genetic/parameters/graph_depth.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/genetic/parameters/mutation_prob.py` & `thegolem-0.3.0/golem/core/optimisers/genetic/parameters/mutation_prob.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/genetic/parameters/operators_prob.py` & `thegolem-0.3.0/golem/core/optimisers/genetic/parameters/operators_prob.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/genetic/parameters/parameter.py` & `thegolem-0.3.0/golem/core/optimisers/genetic/parameters/parameter.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/genetic/parameters/population_size.py` & `thegolem-0.3.0/golem/core/optimisers/genetic/parameters/population_size.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/graph_builder.py` & `thegolem-0.3.0/golem/core/optimisers/graph_builder.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/initial_graphs_generator.py` & `thegolem-0.3.0/golem/core/optimisers/initial_graphs_generator.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/objective/objective.py` & `thegolem-0.3.0/golem/core/optimisers/objective/objective.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import itertools
 from dataclasses import dataclass
 from numbers import Real
-from typing import Any, Optional, Iterable, Callable, Sequence, TypeVar, Dict, Tuple, Union
+from typing import Any, Optional, Callable, Sequence, TypeVar, Dict, Tuple, Union
 
 from golem.core.dag.graph import Graph
 from golem.core.log import default_log
-from golem.core.optimisers.fitness import *
+from golem.core.optimisers.fitness import Fitness, SingleObjFitness, null_fitness, MultiObjFitness
 
 G = TypeVar('G', bound=Graph, covariant=True)
 R = TypeVar('R', contravariant=True)
 GraphFunction = Callable[[G], R]
 ObjectiveFunction = GraphFunction[G, Fitness]
 
 
@@ -20,28 +20,32 @@
     metric_names: Sequence[str] = ()
 
     def format_fitness(self, fitness: Union[Fitness, Sequence[float]]) -> str:
         """Returns formatted fitness string.
         Example for 3 metrics: `<roc_auc=0.542 f1=0.72 complexity=0.8>`"""
         values = fitness.values if isinstance(fitness, Fitness) else fitness
         fitness_info_str = [f'{name}={value:.3f}'
+                            if value is not None
+                            else f'{name}=None'
                             for name, value in zip(self.metric_names, values)]
         return f"<{' '.join(fitness_info_str)}>"
 
 
 class Objective(ObjectiveInfo, ObjectiveFunction):
     """Represents objective function for computing metric values
     on Graphs and keeps information about metrics used."""
 
     def __init__(self,
-                 quality_metrics: Dict[Any, Callable],
+                 quality_metrics: Union[Callable, Dict[Any, Callable]],
                  complexity_metrics: Optional[Dict[Any, Callable]] = None,
                  is_multi_objective: bool = False,
                  ):
         self._log = default_log(self)
+        if isinstance(quality_metrics, Callable):
+            quality_metrics = {'metric': quality_metrics}
         self.quality_metrics = quality_metrics
         self.complexity_metrics = complexity_metrics or {}
         metric_names = [str(metric_id) for metric_id, _ in self.metrics]
         ObjectiveInfo.__init__(self, is_multi_objective, metric_names)
 
     def __call__(self, graph: Graph, **metrics_kwargs: Any) -> Fitness:
         evaluated_metrics = []
```

### Comparing `thegolem-0.2.0/golem/core/optimisers/objective/objective_eval.py` & `thegolem-0.3.0/golem/core/optimisers/objective/objective_eval.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/opt_graph_builder.py` & `thegolem-0.3.0/golem/core/optimisers/opt_graph_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,16 +125,16 @@
         if second_node not in first_node.nodes_from and first_node not in second_node.nodes_from:
             second_node.nodes_from.append(first_node)
 
         return self
 
     def _get_node_from_branch_with_idx(self, branch_idx: int, node_idx_in_branch: int):
         head_node = self.heads[branch_idx]
-        branch_pipeline = OptGraph(head_node)
-        return branch_pipeline.nodes[node_idx_in_branch]
+        branch_graph = OptGraph(head_node)
+        return branch_graph.nodes[node_idx_in_branch]
 
     def join_branches(self, operation_type: Optional[str], params: Optional[Dict] = None):
         """ Joins all current branches with provided operation as ensemble node.
 
         If there are no branches => does nothing.
         If there is single branch => adds single node using it as input.
         If there are several branches => adds single node using all heads as inputs.
@@ -195,15 +195,15 @@
     i.e. one final node to many initial nodes and many final nodes to one initial node.
     Merging is undefined for the case of many-to-many nodes and None is returned.
     Merging of the builder with itself is well-defined and leads to duplication of the graph.
 
     If one of the builders is empty -- the other one is returned, no merging is performed.
     State of the passed builders is preserved as they were, after merging new builder is returned.
 
-    :return: PipelineBuilder if merging is well-defined, None otherwise.
+    :return: GraphBuilder if merging is well-defined, None otherwise.
     """
 
     if not following.heads:
         return previous
     elif not previous.heads:
         return following
```

### Comparing `thegolem-0.2.0/golem/core/optimisers/opt_history_objects/generation.py` & `thegolem-0.3.0/golem/core/optimisers/opt_history_objects/generation.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/opt_history_objects/individual.py` & `thegolem-0.3.0/golem/core/optimisers/opt_history_objects/individual.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/opt_history_objects/opt_history.py` & `thegolem-0.3.0/golem/core/optimisers/opt_history_objects/opt_history.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/opt_history_objects/parent_operator.py` & `thegolem-0.3.0/golem/core/optimisers/opt_history_objects/parent_operator.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/opt_node_factory.py` & `thegolem-0.3.0/golem/core/optimisers/opt_node_factory.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/optimization_parameters.py` & `thegolem-0.3.0/golem/core/optimisers/optimization_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         If the path is relative, then save relative to `default_data_dir`.
         If absolute -- then save directly by specified path.
         If None -- do not save the history to disk and keep it only in-memory.
     """
 
     num_of_generations: Optional[int] = None
     timeout: Optional[datetime.timedelta] = datetime.timedelta(minutes=5)
-    early_stopping_iterations: Optional[int] = 10
+    early_stopping_iterations: Optional[int] = 50
     early_stopping_timeout: Optional[float] = 5
 
     keep_n_best: int = 1
     max_graph_fit_time: Optional[datetime.timedelta] = None
     n_jobs: int = 1
     show_progress: bool = True
     collect_intermediate_metric: bool = False
@@ -75,17 +75,17 @@
     :param start_depth: start value of adaptive tree depth
     :param max_depth: max depth of the resulting graph
     :param min_arity: min number of parents for node
     :param max_arity: max number of parents for node
     """
 
     start_depth: int = 3
-    max_depth: int = 3
+    max_depth: int = 10
     min_arity: int = 2
-    max_arity: int = 2
+    max_arity: int = 4
 
     def __post_init__(self):
         excluded_fields = ['n_jobs']
         for field_name, field_value in dataclasses.asdict(self).items():
             if field_name in excluded_fields:
                 continue
             if isinstance(field_value, Number) and field_value < 0:
```

### Comparing `thegolem-0.2.0/golem/core/optimisers/optimizer.py` & `thegolem-0.3.0/golem/core/optimisers/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import abstractmethod
 from dataclasses import dataclass
-from typing import Any, Callable, Optional, Sequence
+from typing import Any, Callable, Optional, Sequence, Union
 
 from golem.core.adapter import BaseOptimizationAdapter, IdentityAdapter
 from golem.core.dag.graph import Graph
 from golem.core.dag.graph_verifier import GraphVerifier, VerifierRuleType
 from golem.core.dag.verification_rules import DEFAULT_DAG_RULES
 from golem.core.log import default_log
 from golem.core.optimisers.advisor import DefaultChangeAdvisor
@@ -99,21 +99,22 @@
     :param requirements: implementation-independent requirements for graph optimizer
     :param graph_generation_params: parameters for new graph generation
     :param graph_optimizer_params: parameters for specific implementation of graph optimizer
     """
 
     def __init__(self,
                  objective: Objective,
-                 initial_graphs: Optional[Sequence[Graph]] = None,
+                 initial_graphs: Optional[Sequence[Union[Graph, Any]]] = None,
+                 # TODO: rename params to avoid confusion
                  requirements: Optional[OptimizationParameters] = None,
                  graph_generation_params: Optional[GraphGenerationParams] = None,
                  graph_optimizer_params: Optional[AlgorithmParameters] = None):
         self.log = default_log(self)
-        self.initial_graphs = initial_graphs
         self._objective = objective
+        self.initial_graphs = graph_generation_params.adapter.adapt(initial_graphs) if initial_graphs else None
         self.requirements = requirements or OptimizationParameters()
         self.graph_generation_params = graph_generation_params or GraphGenerationParams()
         self.graph_optimizer_params = graph_optimizer_params or AlgorithmParameters()
         self._optimisation_callback: OptimisationCallback = do_nothing_callback
         self._history = OptHistory(objective.get_info(), requirements.history_dir) \
             if requirements and requirements.keep_history else None
```

### Comparing `thegolem-0.2.0/golem/core/optimisers/populational_optimizer.py` & `thegolem-0.3.0/golem/core/optimisers/populational_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from tqdm import tqdm
 
 from golem.core.dag.graph import Graph
 from golem.core.optimisers.archive import GenerationKeeper
 from golem.core.optimisers.genetic.evaluation import MultiprocessingDispatcher, SequentialDispatcher
 from golem.core.optimisers.genetic.operators.operator import PopulationT, EvaluationOperator
 from golem.core.optimisers.optimization_parameters import GraphRequirements
-from golem.core.optimisers.graph import OptGraph
 from golem.core.optimisers.objective import GraphFunction, ObjectiveFunction
 from golem.core.optimisers.objective.objective import Objective
 from golem.core.optimisers.optimizer import GraphGenerationParams, GraphOptimizer, AlgorithmParameters
 from golem.core.optimisers.timer import OptimisationTimer
 from golem.core.utilities.grouped_condition import GroupedCondition
 
 
@@ -56,16 +55,16 @@
         max_stagnation_length = requirements.early_stopping_iterations or requirements.num_of_generations
         max_stagnation_time = requirements.early_stopping_timeout or self.timer.timeout
         self.stop_optimization = \
             GroupedCondition(results_as_message=True).add_condition(
                 lambda: self.timer.is_time_limit_reached(self.current_generation_num),
                 'Optimisation stopped: Time limit is reached'
             ).add_condition(
-                lambda: requirements.num_of_generations is not None and
-                        self.current_generation_num >= requirements.num_of_generations + 1,
+                lambda: (requirements.num_of_generations is not None and
+                         self.current_generation_num >= requirements.num_of_generations + 1),
                 'Optimisation stopped: Max number of generations reached'
             ).add_condition(
                 lambda: self.generations.stagnation_iter_count >= max_stagnation_length,
                 'Optimisation finished: Early stopping iterations criteria was satisfied'
             ).add_condition(
                 lambda: self.generations.stagnation_time_duration >= max_stagnation_time,
                 'Optimisation finished: Early stopping timeout criteria was satisfied'
@@ -75,15 +74,15 @@
     def current_generation_num(self) -> int:
         return self.generations.generation_num
 
     def set_evaluation_callback(self, callback: Optional[GraphFunction]):
         # Redirect callback to evaluation dispatcher
         self.eval_dispatcher.set_graph_evaluation_callback(callback)
 
-    def optimise(self, objective: ObjectiveFunction) -> Sequence[OptGraph]:
+    def optimise(self, objective: ObjectiveFunction) -> Sequence[Graph]:
 
         # eval_dispatcher defines how to evaluate objective on the whole population
         evaluator = self.eval_dispatcher.dispatch(objective, self.timer)
 
         with self.timer, self._progressbar:
 
             self._initial_population(evaluator)
```

### Comparing `thegolem-0.2.0/golem/core/optimisers/random/random_mutation_optimizer.py` & `thegolem-0.3.0/golem/core/optimisers/random/random_mutation_optimizer.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/random/random_search.py` & `thegolem-0.3.0/golem/core/optimisers/random/random_search.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/random_graph_factory.py` & `thegolem-0.3.0/golem/core/optimisers/random_graph_factory.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/optimisers/timer.py` & `thegolem-0.3.0/golem/core/optimisers/timer.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/paths.py` & `thegolem-0.3.0/golem/core/paths.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/tuning/search_space.py` & `thegolem-0.3.0/golem/core/tuning/search_space.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/tuning/sequential.py` & `thegolem-0.3.0/golem/core/tuning/sequential.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,14 +73,16 @@
                                     node_params=node_params,
                                     iterations_per_node=iterations_per_node,
                                     seconds_per_node=seconds_per_node)
 
         # Validation is the optimization do well
         final_graph = self.final_check(graph)
 
+        self.was_tuned = True
+
         return self.adapter.restore(final_graph)
 
     def get_nodes_order(self, nodes_number: int) -> range:
         """ Method returns list with indices of nodes in the graph
 
         Args:
             nodes_number: number of nodes to get
@@ -122,14 +124,15 @@
             # Apply tuning for current node
             self._optimize_node(graph=graph,
                                 node_id=node_index,
                                 node_params=node_params,
                                 iterations_per_node=self.iterations,
                                 seconds_per_node=self.max_seconds,
                                 )
+            self.was_tuned = True
 
         # Validation is the optimization do well
         final_graph = self.final_check(graph)
         final_graph = self.adapter.restore(final_graph)
         return final_graph
 
     def _optimize_node(self, graph: OptGraph, node_id: int, node_params: dict, iterations_per_node: int,
```

### Comparing `thegolem-0.2.0/golem/core/tuning/simultaneous.py` & `thegolem-0.3.0/golem/core/tuning/simultaneous.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,25 +70,27 @@
 
                     tuned_graph = self.set_arg_graph(graph=graph,
                                                      parameters=best)
 
                     # Validation is the optimization do well
                     graph = self.final_check(tuned_graph)
 
+                    self.was_tuned = True
+
                 except Exception as ex:
                     self.log.warning(f'Exception {ex} occurred during tuning')
 
         final_graph = self.adapter.restore(graph)
 
         return final_graph
 
     def _search_near_initial_parameters(self, graph: OptGraph, search_space: dict, initial_parameters: dict,
                                         trials: Trials, show_progress: bool = True) -> Tuple[Trials, int]:
-        """ Method to search using the search space where initially parameters set for the graph are fixed.
-        This allows not to lose results obtained while composition process (e.g. ``parameter_change_mutation``)
+        """ Method to search using the search space where parameters initially set for the graph are fixed.
+        This allows not to lose results obtained while composition process
 
         Args:
             graph: graph to be tuned
             search_space: dict with parameters to be optimized and their search spaces
             initial_parameters: dict with initial parameters of the graph
             trials: Trials object to store all the search iterations
             show_progress: shows progress of tuning if True
@@ -151,15 +153,15 @@
                     initial_parameters.update(tunable_initial_params)
 
         return parameters_dict, initial_parameters
 
     def _objective(self, parameters_dict: dict, graph: OptGraph, unchangeable_parameters: Optional[dict] = None) \
             -> float:
         """
-        Objective function for minimization / maximization problem
+        Objective function for minimization problem
 
         Args:
             parameters_dict: dict which contains new graph hyperparameters
             graph: graph to optimize
             unchangeable_parameters: dict with parameters that should not be changed
 
         Returns:
```

### Comparing `thegolem-0.2.0/golem/core/tuning/tuner_interface.py` & `thegolem-0.3.0/golem/core/tuning/tuner_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     def init_check(self, graph: OptGraph) -> None:
         """
         Method get metric on validation set before start optimization
 
         Args:
           graph: graph to calculate objective
         """
-        self.log.info('Hyperparameters optimization start: estimation of metric for initial pipeline')
+        self.log.info('Hyperparameters optimization start: estimation of metric for initial graph')
 
         # Train graph
         self.init_graph = deepcopy(graph)
 
         self.init_metric = self.get_metric_value(graph=self.init_graph)
         self.log.message(f'Initial graph: {graph_structure(self.init_graph)} \n'
                          f'Initial metric: {abs(self.init_metric):.3f}')
```

### Comparing `thegolem-0.2.0/golem/core/utilities/data_structures.py` & `thegolem-0.3.0/golem/core/utilities/data_structures.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/utilities/grouped_condition.py` & `thegolem-0.3.0/golem/core/utilities/grouped_condition.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/utilities/random.py` & `thegolem-0.3.0/golem/core/utilities/random.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/utilities/sequence_iterator.py` & `thegolem-0.3.0/golem/core/utilities/sequence_iterator.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/utilities/serializable.py` & `thegolem-0.3.0/golem/core/utilities/serializable.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/core/utilities/singleton_meta.py` & `thegolem-0.3.0/golem/core/utilities/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/metrics/graph_features.py` & `thegolem-0.3.0/golem/metrics/graph_features.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/metrics/mmd.py` & `thegolem-0.3.0/golem/metrics/mmd.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import itertools
 import numpy as np
 from scipy.linalg import toeplitz
-import pyemd
+from scipy.stats import wasserstein_distance
 
 
 def emd(x, y, distance_scaling=1.0):
+    """Earth's mover distance (or Wasserstein metric)
+     between 2 probability distributions."""
     support_size = max(len(x), len(y))
     d_mat = toeplitz(range(support_size)).astype(np.float64)
     distance_mat = d_mat / distance_scaling
 
     # convert histogram values x and y to float, and make them equal len
     x = x.astype(np.float64)
     y = y.astype(np.float64)
     if len(x) < len(y):
         x = np.hstack((x, [0.0] * (support_size - len(x))))
     elif len(y) < len(x):
         y = np.hstack((y, [0.0] * (support_size - len(y))))
 
-    emd_value = pyemd.emd(x, y, distance_mat)
+    emd_value = wasserstein_distance(x, y, distance_mat)
     return emd_value
 
 
 def l2(x, y):
     dist = np.linalg.norm(x - y, 2)
     return dist
```

### Comparing `thegolem-0.2.0/golem/serializers/any_serialization.py` & `thegolem-0.3.0/golem/serializers/any_serialization.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/serializers/coders/graph_node_serialization.py` & `thegolem-0.3.0/golem/serializers/coders/graph_node_serialization.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Uses regular serialization but excludes "_operator" field to rid of circular references
     """
     encoded = {
         k: v
         for k, v in any_to_json(obj).items()
         if k not in ['_operator', '_fitted_operation', '_node_data', '_parameters']
     }
-    encoded['content']['name'] = str(encoded['content']['name'])
+    if 'name' in encoded['content']:
+        encoded['content']['name'] = str(encoded['content']['name'])
     if encoded['_nodes_from']:
         encoded['_nodes_from'] = [
             node.uid
             for node in encoded['_nodes_from']
         ]
     return encoded
```

### Comparing `thegolem-0.2.0/golem/serializers/coders/graph_serialization.py` & `thegolem-0.3.0/golem/serializers/coders/graph_serialization.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/serializers/coders/opt_history_serialization.py` & `thegolem-0.3.0/golem/serializers/coders/opt_history_serialization.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/serializers/coders/parent_operator_serialization.py` & `thegolem-0.3.0/golem/serializers/coders/parent_operator_serialization.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/serializers/serializer.py` & `thegolem-0.3.0/golem/serializers/serializer.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/utilities/memory.py` & `thegolem-0.3.0/golem/utilities/memory.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/utilities/profiler/memory_profiler.py` & `thegolem-0.3.0/golem/utilities/profiler/memory_profiler.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/utilities/profiler/time_profiler.py` & `thegolem-0.3.0/golem/utilities/profiler/time_profiler.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/utilities/requirements_notificator.py` & `thegolem-0.3.0/golem/utilities/requirements_notificator.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/visualisation/graph_viz.py` & `thegolem-0.3.0/golem/visualisation/graph_viz.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import datetime
 import os
+from copy import deepcopy
 from pathlib import Path
 from textwrap import wrap
-from typing import TYPE_CHECKING, Any, Callable, Dict, Iterable, Optional, Sequence, Tuple, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, Iterable, Optional, Sequence, Tuple, Union, List
 from uuid import uuid4
 
 import networkx as nx
 import numpy as np
 from matplotlib import pyplot as plt
 from matplotlib.colors import to_hex
 from matplotlib.patches import ArrowStyle
@@ -31,15 +32,15 @@
 MatplotlibColorType = Union[str, Sequence[float]]
 LabelsColorMapType = Dict[str, MatplotlibColorType]
 NodeColorFunctionType = Callable[[Iterable[str]], LabelsColorMapType]
 NodeColorType = Union[MatplotlibColorType, LabelsColorMapType, NodeColorFunctionType]
 
 
 class GraphVisualizer:
-    def __init__(self, graph: GraphType, visuals_params: Optional[Dict[str, Any]] = None):
+    def __init__(self, graph: GraphType, visuals_params: Optional[Dict[str, Any]] = None, ):
         visuals_params = visuals_params or {}
         default_visuals_params = dict(
             engine='matplotlib',
             dpi=100,
             node_color=self.__get_colors_by_labels,
             node_size_scale=1.0,
             font_size_scale=1.0,
@@ -51,23 +52,26 @@
         self.graph = graph
 
         self.log = default_log(self)
 
     def visualise(self, save_path: Optional[PathType] = None, engine: Optional[str] = None,
                   node_color: Optional[NodeColorType] = None, dpi: Optional[int] = None,
                   node_size_scale: Optional[float] = None,
-                  font_size_scale: Optional[float] = None, edge_curvature_scale: Optional[float] = None):
+                  font_size_scale: Optional[float] = None, edge_curvature_scale: Optional[float] = None,
+                  nodes_labels: Dict[int, str] = None, edges_labels: Dict[int, str] = None):
         engine = engine or self.get_predefined_value('engine')
 
         if not self.graph.nodes:
             raise ValueError('Empty graph can not be visualized.')
 
         if engine == 'matplotlib':
-            self.__draw_with_networkx(save_path, node_color, dpi, node_size_scale, font_size_scale,
-                                      edge_curvature_scale)
+            self.__draw_with_networkx(save_path=save_path, node_color=node_color, dpi=dpi,
+                                      node_size_scale=node_size_scale, font_size_scale=font_size_scale,
+                                      edge_curvature_scale=edge_curvature_scale,
+                                      nodes_labels=nodes_labels, edges_labels=edges_labels)
         elif engine == 'pyvis':
             self.__draw_with_pyvis(save_path, node_color)
         elif engine == 'graphviz':
             self.__draw_with_graphviz(save_path, node_color, dpi)
         else:
             raise NotImplementedError(f'Unexpected visualization engine: {engine}. '
                                       'Possible values: matplotlib, pyvis, graphviz.')
@@ -158,42 +162,41 @@
         net.show(str(save_path))
         remove_old_files_from_dir(save_path.parent)
 
     def __draw_with_networkx(self, save_path: Optional[PathType] = None,
                              node_color: Optional[NodeColorType] = None,
                              dpi: Optional[int] = None, node_size_scale: Optional[float] = None,
                              font_size_scale: Optional[float] = None, edge_curvature_scale: Optional[float] = None,
-                             graph_to_nx_convert_func: Optional[Callable] = None):
+                             graph_to_nx_convert_func: Optional[Callable] = None,
+                             nodes_labels: Dict[int, str] = None, edges_labels: Dict[int, str] = None):
         save_path = save_path or self.get_predefined_value('save_path')
         node_color = node_color or self.get_predefined_value('node_color')
         dpi = dpi or self.get_predefined_value('dpi')
         node_size_scale = node_size_scale or self.get_predefined_value('node_size_scale')
         font_size_scale = font_size_scale or self.get_predefined_value('font_size_scale')
         edge_curvature_scale = (edge_curvature_scale if edge_curvature_scale is not None
                                 else self.get_predefined_value('edge_curvature_scale'))
         graph_to_nx_convert_func = graph_to_nx_convert_func or self.get_predefined_value('graph_to_nx_convert_func')
 
         fig, ax = plt.subplots(figsize=(7, 7))
         fig.set_dpi(dpi)
 
-        # nx_graph = BaseNetworkxAdapter().restore(self.graph)
-        # nx.draw_kamada_kawai(nx_graph, arrows=True, ax=ax)
         self.draw_nx_dag(self.graph, ax, node_color, node_size_scale, font_size_scale, edge_curvature_scale,
-                         graph_to_nx_convert_func)
+                         graph_to_nx_convert_func, nodes_labels, edges_labels)
         if not save_path:
             plt.show()
         else:
             plt.savefig(save_path, dpi=dpi)
             plt.close()
 
-    @staticmethod
-    def draw_nx_dag(graph: GraphType, ax: Optional[plt.Axes] = None,
+    def draw_nx_dag(self, graph: GraphType, ax: Optional[plt.Axes] = None,
                     node_color: Optional[NodeColorType] = None,
                     node_size_scale: float = 1, font_size_scale: float = 1, edge_curvature_scale: float = 1,
-                    graph_to_nx_convert_func: Callable = graph_structure_as_nx_graph):
+                    graph_to_nx_convert_func: Callable = graph_structure_as_nx_graph,
+                    nodes_labels: Dict[int, str] = None, edges_labels: Dict[int, str] = None):
 
         def draw_nx_labels(pos, node_labels, ax, max_sequence_length, font_size_scale=1.0):
             def get_scaled_font_size(nodes_amount):
                 min_size = 2
                 max_size = 20
 
                 size = min_size + int((max_size - min_size) / np.log2(max(nodes_amount, 2)))
@@ -252,17 +255,17 @@
             min_distance_found = node_distance_gap * 2  # It just must be bigger than the gap.
             closest_node_id = None
             for node_id in nx_graph.nodes:
                 if node_id in (u, v):
                     continue  # The node is adjacent to the edge.
                 p_3 = np.array(pos[node_id])
                 distance_to_node = abs(np.cross(p_1_2, p_3 - p_1)) / p_1_2_length
-                if (distance_to_node > min(node_distance_gap, min_distance_found)  # The node is too far.
-                        or ((p_3 - p_1) @ p_1_2) < 0  # There's no perpendicular from the node to the edge.
-                        or ((p_3 - p_2) @ -p_1_2) < 0):
+                if (distance_to_node > min(node_distance_gap, min_distance_found) or  # The node is too far.
+                        ((p_3 - p_1) @ p_1_2) < 0 or  # There's no perpendicular from the node to the edge.
+                        ((p_3 - p_2) @ -p_1_2) < 0):
                     continue
                 min_distance_found = distance_to_node
                 closest_node_id = node_id
 
             if closest_node_id is None:
                 continue  # There's no node to bend around.
             # Finally, define the edge's curvature based on the closest node position.
@@ -280,28 +283,122 @@
             edge_curvature = curvature_direction * curvature_strength
             e['connectionstyle'] = connection_style_curved_template.format(edge_curvature)
         # Draw the graph's edges.
         arrow_style = ArrowStyle('Simple', head_length=1.5, head_width=0.8)
         for u, v, e in nx_graph.edges(data=True):
             nx.draw_networkx_edges(nx_graph, pos, edgelist=[(u, v)], node_size=node_size, ax=ax, arrowsize=10,
                                    arrowstyle=arrow_style, connectionstyle=e['connectionstyle'])
+        if nodes_labels or edges_labels:
+            self._set_labels(ax, pos, nx_graph,
+                             longest_sequence, longest_sequence, font_size_scale,
+                             nodes_labels, edges_labels)
         # Rescale the figure for all nodes to fit in.
         x_1, x_2 = ax.get_xlim()
         y_1, y_2 = ax.get_ylim()
         offset = 0.2
         x_offset = x_2 * offset
         y_offset = y_2 * offset
         ax.set_xlim(x_1 - x_offset, x_2 + x_offset)
         ax.set_ylim(y_1 - y_offset, y_2 + y_offset)
         ax.axis('off')
         plt.tight_layout()
 
     def get_predefined_value(self, param: str):
         return self.visuals_params.get(param)
 
+    def _set_labels(self, ax: plt.Axes, pos: Any, nx_graph: nx.DiGraph,
+                    longest_sequence: int, longest_y_sequence: int, font_size_scale: float,
+                    nodes_labels: Dict[int, str], edges_labels: Dict[int, str]):
+        """ Set labels with scores to nodes and edges. """
+
+        def calculate_labels_bias(ax: plt.Axes, longest_y_sequence: int):
+            y_1, y_2 = ax.get_ylim()
+            y_size = y_2 - y_1
+            if longest_y_sequence == 1:
+                bias_scale = 0.25  # Fits between the central line and the upper bound.
+            else:
+                bias_scale = 1 / longest_y_sequence / 3 * 0.9  # Fits between the narrowest horizontal rows.
+            bias = y_size * bias_scale
+            return bias
+
+        def _get_scaled_font_size(nodes_amount: int, size_scale: float) -> float:
+            min_size = 11
+            max_size = 25
+            size = max(max_size * (1 - np.log10(nodes_amount)), min_size)
+            return size * size_scale
+
+        def match_labels_with_nx_nodes(nx_graph: nx.DiGraph, labels: Dict[int, str]) -> Dict[str, str]:
+            """ Matches index of node in GOLEM graph with networkx node name. """
+            nx_nodes = list(nx_graph.nodes.keys())
+            nx_labels = {}
+            for index in labels:
+                nx_labels[nx_nodes[index]] = labels[index]
+            return nx_labels
+
+        def match_labels_with_nx_edges(nx_graph: nx.DiGraph, labels: Dict[int, str]) \
+                -> Dict[Tuple[str, str], List[str]]:
+            """ Matches index of edge in GOLEM graph with tuple of networkx nodes names. """
+            nx_nodes = list(nx_graph.nodes.keys())
+            edges = self.graph.get_edges()
+            nx_labels = {}
+            for index in labels:
+                edge = edges[index]
+                parent_node_nx = nx_nodes[self.graph.nodes.index(edge[0])]
+                child_node_nx = nx_nodes[self.graph.nodes.index(edge[1])]
+                nx_labels[(parent_node_nx, child_node_nx)] = labels[index]
+            return nx_labels
+
+        if not edges_labels and not nodes_labels:
+            return
+
+        bias = calculate_labels_bias(ax, longest_y_sequence)
+        if nodes_labels:
+            # Set labels for nodes
+            labels_pos = deepcopy(pos)
+            font_size = _get_scaled_font_size(longest_sequence, font_size_scale * 0.7)
+            bbox = dict(alpha=0.9, color='w')
+            for value in labels_pos.values():
+                value[1] += bias
+
+            nodes_nx_labels = match_labels_with_nx_nodes(nx_graph=nx_graph, labels=nodes_labels)
+            nx.draw_networkx_labels(
+                nx_graph, labels_pos,
+                labels=nodes_nx_labels,
+                font_color='black',
+                font_size=font_size,
+                bbox=bbox
+            )
+
+        if not edges_labels:
+            return
+        labels_pos_edges = deepcopy(pos)
+        label_bias_y = 2 / 3 * bias
+        if len(set([coord[1] for coord in pos.values()])) == 1 and len(list(pos.values())) > 2:
+            for value in labels_pos_edges.values():
+                value[1] += label_bias_y
+
+        edges_nx_labels = match_labels_with_nx_edges(nx_graph=nx_graph, labels=edges_labels)
+        # Set labels for edges
+        for u, v, e in nx_graph.edges(data=True):
+            if (u, v) not in edges_nx_labels:
+                continue
+            current_pos = labels_pos_edges
+            if 'edge_center_position' in e:
+                x, y = e['edge_center_position']
+                plt.text(x, y, edges_nx_labels[(u, v)], bbox=bbox, fontsize=font_size)
+            else:
+                nx.draw_networkx_edge_labels(
+                    nx_graph, current_pos, {(u, v): edges_nx_labels[(u, v)]},
+                    label_pos=0.5, ax=ax,
+                    font_color='black',
+                    font_size=font_size,
+                    rotate=False,
+                    bbox=bbox
+                )
+
 
 def get_hierarchy_pos(graph: nx.DiGraph, max_line_length: int = 6) -> Tuple[Dict[Any, Tuple[float, float]], int]:
     """By default, returns 'networkx.multipartite_layout' positions based on 'hierarchy_level` from node data - the
      property must be set beforehand.
     If line of nodes reaches 'max_line_length', the result is the combination of 'networkx.multipartite_layout' and
     'networkx.spring_layout'.
     :param graph: the graph.
```

### Comparing `thegolem-0.2.0/golem/visualisation/opt_history/arg_constraint_wrapper.py` & `thegolem-0.3.0/golem/visualisation/opt_history/arg_constraint_wrapper.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/visualisation/opt_history/fitness_box.py` & `thegolem-0.3.0/golem/visualisation/opt_history/fitness_box.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/visualisation/opt_history/fitness_line.py` & `thegolem-0.3.0/golem/visualisation/opt_history/fitness_line.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/visualisation/opt_history/graphs_interactive.py` & `thegolem-0.3.0/golem/visualisation/opt_history/graphs_interactive.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/visualisation/opt_history/history_visualization.py` & `thegolem-0.3.0/golem/visualisation/opt_history/history_visualization.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/visualisation/opt_history/operations_animated_bar.py` & `thegolem-0.3.0/golem/visualisation/opt_history/operations_animated_bar.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/visualisation/opt_history/operations_kde.py` & `thegolem-0.3.0/golem/visualisation/opt_history/operations_kde.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/visualisation/opt_history/utils.py` & `thegolem-0.3.0/golem/visualisation/opt_history/utils.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/visualisation/opt_viz.py` & `thegolem-0.3.0/golem/visualisation/opt_viz.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/golem/visualisation/opt_viz_extra.py` & `thegolem-0.3.0/golem/visualisation/opt_viz_extra.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/libs/netcomp/eigenstuff.py` & `thegolem-0.3.0/libs/netcomp/eigenstuff.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/libs/netcomp/matrices.py` & `thegolem-0.3.0/libs/netcomp/matrices.py`

 * *Files identical despite different names*

### Comparing `thegolem-0.2.0/setup.py` & `thegolem-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 import setuptools
 
 # The directory containing this file
 HERE = Path(__file__).parent.resolve()
 
 # The text of the README file
 NAME = 'thegolem'
-VERSION = '0.2.0'
+VERSION = '0.3.0'
 AUTHOR = 'NSS Lab'
 SHORT_DESCRIPTION = 'Framework for Graph Optimization and Learning by Evolutionary Methods'
 
 README = Path(HERE, 'README_en.rst').read_text(encoding='utf-8')
 URL = 'https://github.com/aimclub/GOLEM'
-REQUIRES_PYTHON = '>=3.7'
+REQUIRES_PYTHON = '>=3.8'
 LICENSE = 'BSD 3-Clause'
 
 
 def _readlines(*names: str, **kwargs) -> List[str]:
     encoding = kwargs.get('encoding', 'utf-8')
     lines = Path(__file__).parent.joinpath(*names).read_text(encoding=encoding).splitlines()
     return list(map(str.strip, lines))
@@ -49,12 +49,12 @@
     install_requires=_get_requirements('requirements.txt'),
     extras_require={
         key: _get_requirements(Path('other_requirements', f'{key}.txt'))
         for key in ('docs', 'profilers')
     },
     classifiers=[
         'License :: OSI Approved :: BSD License',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9'
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10'
     ],
 )
```

### Comparing `thegolem-0.2.0/thegolem.egg-info/SOURCES.txt` & `thegolem-0.3.0/thegolem.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 LICENSE
 README.rst
 setup.py
 docs/__init__.py
 examples/__init__.py
 examples/graph_model_optimization.py
 examples/profiler_example.py
+examples/viz_with_labels.py
+examples/structural_analysis/__init__.py
+examples/structural_analysis/opt_graph_optimization.py
 examples/synthetic_graph_evolution/__init__.py
-examples/synthetic_graph_evolution/abstract_graph_search.py
+examples/synthetic_graph_evolution/experiment.py
+examples/synthetic_graph_evolution/generators.py
+examples/synthetic_graph_evolution/graph_search.py
+examples/synthetic_graph_evolution/simple_run.py
+examples/synthetic_graph_evolution/tree_search.py
 examples/synthetic_graph_evolution/utils.py
 golem/__init__.py
 golem/core/__init__.py
 golem/core/constants.py
 golem/core/log.py
 golem/core/paths.py
 golem/core/adapter/__init__.py
@@ -47,14 +54,15 @@
 golem/core/optimisers/fitness/multi_objective_fitness.py
 golem/core/optimisers/genetic/__init__.py
 golem/core/optimisers/genetic/evaluation.py
 golem/core/optimisers/genetic/gp_operators.py
 golem/core/optimisers/genetic/gp_optimizer.py
 golem/core/optimisers/genetic/gp_params.py
 golem/core/optimisers/genetic/operators/__init__.py
+golem/core/optimisers/genetic/operators/base_mutations.py
 golem/core/optimisers/genetic/operators/crossover.py
 golem/core/optimisers/genetic/operators/elitism.py
 golem/core/optimisers/genetic/operators/inheritance.py
 golem/core/optimisers/genetic/operators/mutation.py
 golem/core/optimisers/genetic/operators/operator.py
 golem/core/optimisers/genetic/operators/regularization.py
 golem/core/optimisers/genetic/operators/selection.py
@@ -84,27 +92,48 @@
 golem/core/utilities/data_structures.py
 golem/core/utilities/grouped_condition.py
 golem/core/utilities/random.py
 golem/core/utilities/sequence_iterator.py
 golem/core/utilities/serializable.py
 golem/core/utilities/singleton_meta.py
 golem/metrics/__init__.py
+golem/metrics/edit_distance.py
 golem/metrics/graph_features.py
 golem/metrics/graph_metrics.py
 golem/metrics/mmd.py
 golem/serializers/__init__.py
 golem/serializers/any_serialization.py
 golem/serializers/serializer.py
 golem/serializers/coders/__init__.py
 golem/serializers/coders/enum_serialization.py
 golem/serializers/coders/graph_node_serialization.py
 golem/serializers/coders/graph_serialization.py
 golem/serializers/coders/opt_history_serialization.py
 golem/serializers/coders/parent_operator_serialization.py
 golem/serializers/coders/uuid_serialization.py
+golem/structural_analysis/__init__.py
+golem/structural_analysis/base_sa_approaches.py
+golem/structural_analysis/graph_sa/__init__.py
+golem/structural_analysis/graph_sa/edge_sa_approaches.py
+golem/structural_analysis/graph_sa/edges_analysis.py
+golem/structural_analysis/graph_sa/graph_structural_analysis.py
+golem/structural_analysis/graph_sa/node_sa_approaches.py
+golem/structural_analysis/graph_sa/nodes_analysis.py
+golem/structural_analysis/graph_sa/postproc_methods.py
+golem/structural_analysis/graph_sa/sa_approaches_repository.py
+golem/structural_analysis/graph_sa/sa_requirements.py
+golem/structural_analysis/graph_sa/entities/__init__.py
+golem/structural_analysis/graph_sa/entities/edge.py
+golem/structural_analysis/graph_sa/results/__init__.py
+golem/structural_analysis/graph_sa/results/base_sa_approach_result.py
+golem/structural_analysis/graph_sa/results/deletion_sa_approach_result.py
+golem/structural_analysis/graph_sa/results/object_sa_result.py
+golem/structural_analysis/graph_sa/results/replace_sa_approach_result.py
+golem/structural_analysis/graph_sa/results/sa_analysis_results.py
+golem/structural_analysis/graph_sa/results/utils.py
 golem/utilities/__init__.py
 golem/utilities/memory.py
 golem/utilities/requirements_notificator.py
 golem/utilities/profiler/__init__.py
 golem/utilities/profiler/memory_profiler.py
 golem/utilities/profiler/time_profiler.py
 golem/visualisation/__init__.py
```

