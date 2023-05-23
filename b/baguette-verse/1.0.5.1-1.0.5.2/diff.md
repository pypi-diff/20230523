# Comparing `tmp/baguette_verse-1.0.5.1.tar.gz` & `tmp/baguette_verse-1.0.5.2.tar.gz`

## Comparing `baguette_verse-1.0.5.1.tar` & `baguette_verse-1.0.5.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/__init__.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/baguette.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/logger.py
--rw-r--r--   0        0        0    24429 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/rack.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/__init__.py
--rw-r--r--   0        0        0    23863 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/bake.py
--rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/compiler.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/__init__.py
--rw-r--r--   0        0        0    13119 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/build.py
--rw-r--r--   0        0        0    17960 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/colors.py
--rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/config.py
--rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/event.py
--rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/filters.py
--rw-r--r--   0        0        0    34141 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/graph.py
--rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/record.py
--rw-r--r--   0        0        0     7635 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/utils.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/__init__.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/utils.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/data/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/data/__proc__.py
--rw-r--r--   0        0        0    13656 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/data/entities.py
--rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/data/integration.py
--rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/data/relations.py
--rw-r--r--   0        0        0     9533 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/data/utils.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/execution/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/execution/__proc__.py
--rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/execution/entities.py
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/execution/integration.py
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/execution/relations.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/execution/utils.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/filesystem/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/filesystem/__proc__.py
--rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/filesystem/entities.py
--rw-r--r--   0        0        0    13702 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/filesystem/integration.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/filesystem/relations.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/imports/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/imports/__proc__.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/imports/entities.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/imports/integration.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/imports/relations.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/network/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/network/__proc__.py
--rw-r--r--   0        0        0    10482 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/network/entities.py
--rw-r--r--   0        0        0     9931 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/network/integration.py
--rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/network/relations.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/registry/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/registry/__proc__.py
--rw-r--r--   0        0        0    11045 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/registry/entities.py
--rw-r--r--   0        0        0    16630 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/registry/integration.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/bakery/source/types/registry/relations.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/croutons/__init__.py
--rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/croutons/extractor.py
--rw-r--r--   0        0        0    20653 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/croutons/toast.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/croutons/metalib/__init__.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/croutons/metalib/interact.py
--rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/croutons/metalib/utils.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/croutons/source/__init__.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/croutons/source/evaluator.py
--rw-r--r--   0        0        0    35062 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/croutons/source/metagraph.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/croutons/source/utils.py
--rw-r--r--   0        0        0  9439185 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/tutorial/data.zip
--rw-r--r--   0        0        0    16130 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/tutorial/scripts.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/tutorial/state.txt
--rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/baguette/tutorial/utils.py
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/.gitignore
--rw-r--r--   0        0        0    35123 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/LICENSE
--rw-r--r--   0        0        0     8419 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/README.md
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/pyproject.toml
--rw-r--r--   0        0        0    48797 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/__init__.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/baguette.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/logger.py
+-rw-r--r--   0        0        0    24429 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/rack.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/__init__.py
+-rw-r--r--   0        0        0    23863 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/bake.py
+-rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/compiler.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/__init__.py
+-rw-r--r--   0        0        0    13119 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/build.py
+-rw-r--r--   0        0        0    17960 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/colors.py
+-rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/config.py
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/event.py
+-rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/filters.py
+-rw-r--r--   0        0        0    34141 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/graph.py
+-rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/record.py
+-rw-r--r--   0        0        0     7635 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/utils.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/__init__.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/utils.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/data/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/data/__proc__.py
+-rw-r--r--   0        0        0    13656 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/data/entities.py
+-rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/data/integration.py
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/data/relations.py
+-rw-r--r--   0        0        0     9533 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/data/utils.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/execution/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/execution/__proc__.py
+-rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/execution/entities.py
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/execution/integration.py
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/execution/relations.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/execution/utils.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/filesystem/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/filesystem/__proc__.py
+-rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/filesystem/entities.py
+-rw-r--r--   0        0        0    13702 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/filesystem/integration.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/filesystem/relations.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/imports/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/imports/__proc__.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/imports/entities.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/imports/integration.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/imports/relations.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/network/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/network/__proc__.py
+-rw-r--r--   0        0        0    10482 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/network/entities.py
+-rw-r--r--   0        0        0     9931 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/network/integration.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/network/relations.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/registry/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/registry/__proc__.py
+-rw-r--r--   0        0        0    11045 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/registry/entities.py
+-rw-r--r--   0        0        0    16630 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/registry/integration.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/registry/relations.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/croutons/__init__.py
+-rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/croutons/extractor.py
+-rw-r--r--   0        0        0    20653 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/croutons/toast.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/croutons/metalib/__init__.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/croutons/metalib/interact.py
+-rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/croutons/metalib/utils.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/croutons/source/__init__.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/croutons/source/evaluator.py
+-rw-r--r--   0        0        0    35062 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/croutons/source/metagraph.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/croutons/source/utils.py
+-rw-r--r--   0        0        0  9439185 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/tutorial/data.zip
+-rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/tutorial/scripts.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/tutorial/state.txt
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/tutorial/utils.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/.gitignore
+-rw-r--r--   0        0        0    35123 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/LICENSE
+-rw-r--r--   0        0        0     8419 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/README.md
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/pyproject.toml
+-rw-r--r--   0        0        0    48797 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/PKG-INFO
```

### Comparing `baguette_verse-1.0.5.1/baguette/baguette.py` & `baguette_verse-1.0.5.2/baguette/baguette.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/logger.py` & `baguette_verse-1.0.5.2/baguette/logger.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/rack.py` & `baguette_verse-1.0.5.2/baguette/rack.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/bake.py` & `baguette_verse-1.0.5.2/baguette/bakery/bake.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/compiler.py` & `baguette_verse-1.0.5.2/baguette/bakery/compiler.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/build.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/build.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/colors.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/colors.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/config.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/config.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/event.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/event.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/filters.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/filters.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/graph.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/graph.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/record.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/record.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/utils.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/types/__init__.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/types/__init__.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/types/utils.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/types/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from functools import cache
 from types import ModuleType
 from .. import types as type_package
 from ..graph import Edge, Vertex
 
-__all__ = ["types", "relations", "relation_types", "baguette_structure"]
+__all__ = ["types", "relations", "relation_types", "behavioral_packages", "baguette_structure"]
 
 
 
 
 
 @cache
 def types(mod : ModuleType = type_package) -> set[type[Vertex]]:
@@ -67,14 +67,36 @@
     
     return type_set
 
 
 
 
 
+def behavioral_packages() -> dict[str, ModuleType]:
+    """
+    Returns a dictionary holding all the avaiable behavioral packages in the form {name : package}.
+    Such packages can be used with types() and relations().
+    """
+    from .. import types as type_package
+
+    index = {}
+    package_name = type_package.__name__
+    for name in dir(type_package):
+        value = getattr(type_package, name)
+        if isinstance(value, ModuleType):
+            pname, _, mname = value.__name__.rpartition(".")
+            if name == package_name:
+                index[mname] = value
+
+    return index
+
+
+
+
+
 @cache
 def relation_types(edge_class : type[Edge]) -> tuple[type[Vertex], type[Vertex]]:
     """
     Given an Edge or Arrow subclass, gives the best type hints for the source and destination vertices.
     Defaults to (Vertex, Vertex) when no annotations exist.
     """
     from typing import get_type_hints
```

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/types/data/entities.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/types/data/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/types/data/integration.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/types/data/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/types/data/relations.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/types/data/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/types/data/utils.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/types/data/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/types/execution/entities.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/types/execution/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/types/execution/integration.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/types/execution/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/types/execution/relations.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/types/execution/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/types/execution/utils.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/types/execution/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/types/filesystem/entities.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/types/filesystem/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/types/filesystem/integration.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/types/filesystem/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/types/filesystem/relations.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/types/filesystem/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/types/imports/entities.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/types/imports/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/types/imports/integration.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/types/imports/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/types/imports/relations.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/types/imports/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/types/network/entities.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/types/network/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/types/network/integration.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/types/network/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/types/network/relations.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/types/network/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/types/registry/entities.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/types/registry/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/types/registry/integration.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/types/registry/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/bakery/source/types/registry/relations.py` & `baguette_verse-1.0.5.2/baguette/bakery/source/types/registry/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/croutons/extractor.py` & `baguette_verse-1.0.5.2/baguette/croutons/extractor.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/croutons/toast.py` & `baguette_verse-1.0.5.2/baguette/croutons/toast.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/croutons/metalib/__init__.py` & `baguette_verse-1.0.5.2/baguette/croutons/metalib/__init__.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/croutons/metalib/interact.py` & `baguette_verse-1.0.5.2/baguette/croutons/metalib/interact.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/croutons/metalib/utils.py` & `baguette_verse-1.0.5.2/baguette/croutons/metalib/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,27 +13,28 @@
 
 def import_env(d : dict):
 
     """
     Imports all the necessary classes for building MetaGraphs
     """
 
-    from ...bakery.source import types
+    from ...bakery.source import types as types_package
     from ...bakery.source.graph import Graph, Vertex, Edge, Arrow
     from ..source.metagraph import MetaGraph, MetaEdge, MetaArrow, MetaVertex
+    from ...bakery.source.types.utils import types, relations, relation_types, behavioral_packages, baguette_structure 
     from types import ModuleType
 
     l = locals().copy()
     if "l" in l:
         l.pop("l")
     l.pop("d")
-    l.pop("types")
+    l.pop("types_package")
 
-    for name in dir(types):
-        val = getattr(types, name)
+    for name in dir(types_package):
+        val = getattr(types_package, name)
         if isinstance(val, ModuleType):
             l[name] = val
 
     d.update(l)
```

### Comparing `baguette_verse-1.0.5.1/baguette/croutons/source/evaluator.py` & `baguette_verse-1.0.5.2/baguette/croutons/source/evaluator.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/croutons/source/metagraph.py` & `baguette_verse-1.0.5.2/baguette/croutons/source/metagraph.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/croutons/source/utils.py` & `baguette_verse-1.0.5.2/baguette/croutons/source/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/tutorial/data.zip` & `baguette_verse-1.0.5.2/baguette/tutorial/data.zip`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/baguette/tutorial/scripts.py` & `baguette_verse-1.0.5.2/baguette/tutorial/scripts.py`

 * *Files 7% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 - the index, which is a pickle of a baguette rack (look at 'help(baguette.rack)'), located in the 'index.pyt' file. It contains the metadata of the BAGUETTE.
 - the BAGUETTE itself, also a pickle (look at 'help(baguette.bakery.source.graph)'), located in the 'baguette.pyt' file,
 - the render of the BAGUETTE, saved using the GEXF format, located in the 'visual.gexf' file. It is made to be used with Gephi (https://gephi.org/) for visualizing the BAGUETTE.
 """)
 
             chosen_baguette = str(baguettes[0]).replace("\\", "/")
             clean_print(f"""
-You can now use Gephi to visualize the BAGUETTEs, or if you prefer you can dissect a BAGUETTE by hand in an interactive interpreter:
+You can now use Gephi to visualize the BAGUETTEs (if it looks a bit messy, have a look at the 'filters' parameter of the 'bake' command using 'bake -h'), or if you prefer you can dissect a BAGUETTE by hand in an interactive interpreter:
 To do that, you just have to launch Python, import pickle, and load a 'baguette.pyt' file:
 >>> from pickle import load
 >>> bag = load(open('{chosen_baguette}', 'rb'))
 >>> help(bag)
 
 Good luck! And use 'baguette.tutorial' to learn about toasting!""")
 
@@ -105,14 +105,24 @@
 Put simply, MetaGraphs are pattern graphs. Indeed, they are made of MetaVertices, MetaEdges and MetaArrows, which are just like normal Vertices, Edges and Arrows, except that they allow you to put constrains on types to match real vertices, edges or arrows.
 
 For example, 'MetaVertex[File]' would mean 'Match a vertex which type is \"File\"'.
 If you have two MetaVertices MV1 and MV2, then 'MetaArrow(MV1, MV2)[HasChildProcess]' would mean 'Match an arrow between the two vertices you already matched for MV1 and MV2, which type should be \"HasChildProcess\"'.
 
 With such a syntax, you can build MetaGraphs using the 'metalib'. It is a script that can be launched without parameters which will start a Python interactive prompt with the environment necessary to work on MetaGraphs. Use 'dir()' to list all the resources available in the environment and 'help(resource)' to learn more about any of those.
 
+In the metalib, we could declare a simple MetaGraph using a few commands:
+>>> MG = MetaGraph()
+>>> MG.File = MetaVertex[filesystem.File]
+>>> MG.Directory = MetaVertex[filesystem.Directory]
+>>> MG.Contains = MetaEdge(MG.Directory, MG.File)[filesystem.contains]
+>>> save(MG, "dile_in_directory")
+
+Note that in BAGUETTE, all the Vertex, Edge and Arrow subclasses are organized in behavioral packages, such as 'filesystem'. Others can be listed with 'behavioral_packages()'.
+Remember, all the information you want can be found using Python 'dir' function (to enumerate your environment) and 'help' to find information about the available resources.
+
 For this step of the tutorial, launch the metalib using the command 'metalib' and create a metagraph of your choice and save it under the name you want.""")
 
             next_state("baked")
 
         case "metalib":
 
             clean_print("You should now have created at least one MetaGraph. Checking...")
```

### Comparing `baguette_verse-1.0.5.1/baguette/tutorial/utils.py` & `baguette_verse-1.0.5.2/baguette/tutorial/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/.gitignore` & `baguette_verse-1.0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/LICENSE` & `baguette_verse-1.0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/README.md` & `baguette_verse-1.0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.1/pyproject.toml` & `baguette_verse-1.0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "baguette-verse"
-version = "1.0.5.1"
+version = "1.0.5.2"
 authors = [
   { name="Vincent Raulin", email="vincent.raulin@inria.fr" },
 ]
 description = "A malware behavioral analysis framework centered around BAGUETTE!"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
```

### Comparing `baguette_verse-1.0.5.1/PKG-INFO` & `baguette_verse-1.0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baguette-verse
-Version: 1.0.5.1
+Version: 1.0.5.2
 Summary: A malware behavioral analysis framework centered around BAGUETTE!
 Project-URL: Repository, https://gitlab.inria.fr/vraulin/baguette-verse
 Project-URL: Bug Tracker, https://gitlab.inria.fr/vraulin/baguette-verse/-/issues
 Author-email: Vincent Raulin <vincent.raulin@inria.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
```

