# Comparing `tmp/diffsims-0.5.1.tar.gz` & `tmp/diffsims-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffsims-0.5.1.tar", last modified: Thu Jan 26 17:39:31 2023, max compression
+gzip compressed data, was "diffsims-0.5.2.tar", last modified: Tue May 23 14:38:43 2023, max compression
```

## Comparing `diffsims-0.5.1.tar` & `diffsims-0.5.2.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:39:31.764624 diffsims-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-01-26 17:39:20.000000 diffsims-0.5.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-01-26 17:39:20.000000 diffsims-0.5.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-01-26 17:39:20.000000 diffsims-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-01-26 17:39:20.000000 diffsims-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-01-26 17:39:31.764624 diffsims-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-01-26 17:39:20.000000 diffsims-0.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:39:31.756624 diffsims-0.5.1/diffsims/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:39:31.756624 diffsims-0.5.1/diffsims/crystallography/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/crystallography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17118 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/crystallography/reciprocal_lattice_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    51836 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/crystallography/reciprocal_lattice_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:39:31.756624 diffsims-0.5.1/diffsims/generators/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20944 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/generators/diffraction_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10958 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/generators/library_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/generators/rotation_list_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    18108 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/generators/sphere_mesh_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/generators/zap_map_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:39:31.756624 diffsims-0.5.1/diffsims/libraries/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/libraries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/libraries/diffraction_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/libraries/structure_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/libraries/vector_library.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:39:31.756624 diffsims-0.5.1/diffsims/pattern/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/pattern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/pattern/detector_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/release_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:39:31.756624 diffsims-0.5.1/diffsims/sims/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/sims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18084 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/sims/diffraction_simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:39:31.756624 diffsims-0.5.1/diffsims/structure_factor/
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/structure_factor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/structure_factor/atomic_scattering_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/structure_factor/atomic_scattering_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/structure_factor/structure_factor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:39:31.756624 diffsims-0.5.1/diffsims/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:39:31.756624 diffsims-0.5.1/diffsims/tests/crystallography/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/crystallography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/crystallography/test_reciprocal_lattice_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    24750 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/crystallography/test_reciprocal_lattice_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:39:31.760624 diffsims-0.5.1/diffsims/tests/generators/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/generators/test_diffraction_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/generators/test_library_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/generators/test_rotation_list_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/generators/test_sphere_mesh_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/generators/test_zap_map_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:39:31.760624 diffsims-0.5.1/diffsims/tests/library/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/library/test_diffraction_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/library/test_structure_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/library/test_vector_library.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:39:31.760624 diffsims-0.5.1/diffsims/tests/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/patterns/test_detector_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:39:31.760624 diffsims-0.5.1/diffsims/tests/sims/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/sims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/sims/test_diffraction_simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:39:31.760624 diffsims-0.5.1/diffsims/tests/structure_factor/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/structure_factor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/structure_factor/test_atomic_scattering_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/structure_factor/test_atomic_scattering_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/structure_factor/test_structure_factor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:39:31.760624 diffsims-0.5.1/diffsims/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/utils/test_atomic_diffraction_generator_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/utils/test_discretise_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/utils/test_fourier_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/utils/test_generic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/utils/test_kinematic_simulation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/utils/test_mask_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/utils/test_probe_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/utils/test_ring_pattern_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10926 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/utils/test_sim_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/tests/utils/test_vector_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:39:31.764624 diffsims-0.5.1/diffsims/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/utils/atomic_diffraction_generator_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24489 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/utils/atomic_scattering_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    54550 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/utils/discretise_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24253 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/utils/fourier_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/utils/generic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/utils/kinematic_simulation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    38198 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/utils/lobato_scattering_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/utils/mask_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/utils/probe_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/utils/ring_pattern_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    43469 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/utils/scattering_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/utils/shape_factor_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    23768 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/utils/sim_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-01-26 17:39:20.000000 diffsims-0.5.1/diffsims/utils/vector_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:39:31.756624 diffsims-0.5.1/diffsims.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-01-26 17:39:31.000000 diffsims-0.5.1/diffsims.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-01-26 17:39:31.000000 diffsims-0.5.1/diffsims.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 17:39:31.000000 diffsims-0.5.1/diffsims.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-01-26 17:39:31.000000 diffsims-0.5.1/diffsims.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-26 17:39:31.000000 diffsims-0.5.1/diffsims.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 17:39:31.764624 diffsims-0.5.1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-01-26 17:39:20.000000 diffsims-0.5.1/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-26 17:39:20.000000 diffsims-0.5.1/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-01-26 17:39:20.000000 diffsims-0.5.1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-01-26 17:39:20.000000 diffsims-0.5.1/doc/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-01-26 17:39:20.000000 diffsims-0.5.1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-01-26 17:39:20.000000 diffsims-0.5.1/doc/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-01-26 17:39:20.000000 diffsims-0.5.1/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-01-26 17:39:20.000000 diffsims-0.5.1/doc/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-01-26 17:39:20.000000 diffsims-0.5.1/doc/related_projects.rst
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-26 17:39:20.000000 diffsims-0.5.1/doc/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-01-26 17:39:20.000000 diffsims-0.5.1/readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-01-26 17:39:31.764624 diffsims-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-01-26 17:39:20.000000 diffsims-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.351786 diffsims-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-23 14:38:32.000000 diffsims-0.5.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-23 14:38:32.000000 diffsims-0.5.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-23 14:38:32.000000 diffsims-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-23 14:38:32.000000 diffsims-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-23 14:38:43.351786 diffsims-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-23 14:38:32.000000 diffsims-0.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.343785 diffsims-0.5.2/diffsims/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.343785 diffsims-0.5.2/diffsims/crystallography/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/crystallography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17118 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/crystallography/reciprocal_lattice_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51836 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/crystallography/reciprocal_lattice_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.343785 diffsims-0.5.2/diffsims/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20944 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/generators/diffraction_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10958 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/generators/library_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/generators/rotation_list_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18108 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/generators/sphere_mesh_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/generators/zap_map_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.343785 diffsims-0.5.2/diffsims/libraries/
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/libraries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/libraries/diffraction_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/libraries/structure_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/libraries/vector_library.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.347785 diffsims-0.5.2/diffsims/pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/pattern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/pattern/detector_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/release_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.347785 diffsims-0.5.2/diffsims/sims/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/sims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18084 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/sims/diffraction_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.347785 diffsims-0.5.2/diffsims/structure_factor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/structure_factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/structure_factor/atomic_scattering_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/structure_factor/atomic_scattering_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/structure_factor/structure_factor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.347785 diffsims-0.5.2/diffsims/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.347785 diffsims-0.5.2/diffsims/tests/crystallography/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/crystallography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/crystallography/test_reciprocal_lattice_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24750 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/crystallography/test_reciprocal_lattice_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.347785 diffsims-0.5.2/diffsims/tests/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/generators/test_diffraction_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/generators/test_library_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/generators/test_rotation_list_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/generators/test_sphere_mesh_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/generators/test_zap_map_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.347785 diffsims-0.5.2/diffsims/tests/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/library/test_diffraction_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/library/test_structure_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/library/test_vector_library.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.347785 diffsims-0.5.2/diffsims/tests/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/patterns/test_detector_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.347785 diffsims-0.5.2/diffsims/tests/sims/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/sims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/sims/test_diffraction_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.347785 diffsims-0.5.2/diffsims/tests/structure_factor/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/structure_factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/structure_factor/test_atomic_scattering_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/structure_factor/test_atomic_scattering_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/structure_factor/test_structure_factor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.351786 diffsims-0.5.2/diffsims/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/utils/test_atomic_diffraction_generator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/utils/test_discretise_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/utils/test_fourier_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/utils/test_generic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/utils/test_kinematic_simulation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/utils/test_mask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/utils/test_probe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/utils/test_ring_pattern_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10926 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/utils/test_sim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/utils/test_vector_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.351786 diffsims-0.5.2/diffsims/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/atomic_diffraction_generator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24489 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/atomic_scattering_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54440 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/discretise_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24183 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/fourier_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/generic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/kinematic_simulation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38198 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/lobato_scattering_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/mask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/probe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/ring_pattern_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43469 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/scattering_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/shape_factor_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23768 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/sim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/vector_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.343785 diffsims-0.5.2/diffsims.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-23 14:38:43.000000 diffsims-0.5.2/diffsims.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-05-23 14:38:43.000000 diffsims-0.5.2/diffsims.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:38:43.000000 diffsims-0.5.2/diffsims.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-23 14:38:43.000000 diffsims-0.5.2/diffsims.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 14:38:43.000000 diffsims-0.5.2/diffsims.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.351786 diffsims-0.5.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-23 14:38:32.000000 diffsims-0.5.2/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-23 14:38:32.000000 diffsims-0.5.2/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-23 14:38:32.000000 diffsims-0.5.2/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-23 14:38:32.000000 diffsims-0.5.2/doc/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-23 14:38:32.000000 diffsims-0.5.2/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-23 14:38:32.000000 diffsims-0.5.2/doc/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-23 14:38:32.000000 diffsims-0.5.2/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-05-23 14:38:32.000000 diffsims-0.5.2/doc/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-23 14:38:32.000000 diffsims-0.5.2/doc/related_projects.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-23 14:38:32.000000 diffsims-0.5.2/doc/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-23 14:38:32.000000 diffsims-0.5.2/readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-23 14:38:43.355785 diffsims-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-23 14:38:32.000000 diffsims-0.5.2/setup.py
```

### Comparing `diffsims-0.5.1/CHANGELOG.rst` & `diffsims-0.5.2/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog <https://keepachangelog.com/en/1.0.0>`_,
 and this project adheres to `Semantic Versioning
 <https://semver.org/spec/v2.0.0.html>`_.
 
+2023-05-22 - version 0.5.2
+==========================
+
+Fixed
+-----
+- Always use no-python mode to silence Numba deprecation warnings.
+
 2023-01-25 - version 0.5.1
 ==========================
 
 Fixed
 -----
 - ``ReciprocalLatticeVector.allowed`` rounds indices (hkl) internally to ensure correct
   selection of which vectors are allowed or not given a lattice centering. Integer
```

### Comparing `diffsims-0.5.1/CONTRIBUTING.rst` & `diffsims-0.5.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/LICENSE` & `diffsims-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/PKG-INFO` & `diffsims-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffsims
-Version: 0.5.1
+Version: 0.5.2
 Summary: Diffraction Simulations in Python
 Home-page: https://github.com/pyxem/diffsims
 Author: Duncan Johnstone, Phillip Crout
 Author-email: pyxem.team@gmail.com
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `diffsims-0.5.1/README.rst` & `diffsims-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/__init__.py` & `diffsims-0.5.2/diffsims/__init__.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/conftest.py` & `diffsims-0.5.2/diffsims/conftest.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/crystallography/__init__.py` & `diffsims-0.5.2/diffsims/crystallography/__init__.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/crystallography/reciprocal_lattice_point.py` & `diffsims-0.5.2/diffsims/crystallography/reciprocal_lattice_point.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/crystallography/reciprocal_lattice_vector.py` & `diffsims-0.5.2/diffsims/crystallography/reciprocal_lattice_vector.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/generators/__init__.py` & `diffsims-0.5.2/diffsims/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/generators/diffraction_generator.py` & `diffsims-0.5.2/diffsims/generators/diffraction_generator.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/generators/library_generator.py` & `diffsims-0.5.2/diffsims/generators/library_generator.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/generators/rotation_list_generators.py` & `diffsims-0.5.2/diffsims/generators/rotation_list_generators.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/generators/sphere_mesh_generators.py` & `diffsims-0.5.2/diffsims/generators/sphere_mesh_generators.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/generators/zap_map_generator.py` & `diffsims-0.5.2/diffsims/generators/zap_map_generator.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/libraries/__init__.py` & `diffsims-0.5.2/diffsims/libraries/__init__.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/libraries/diffraction_library.py` & `diffsims-0.5.2/diffsims/libraries/diffraction_library.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/libraries/structure_library.py` & `diffsims-0.5.2/diffsims/libraries/structure_library.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/libraries/vector_library.py` & `diffsims-0.5.2/diffsims/libraries/vector_library.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/pattern/__init__.py` & `diffsims-0.5.2/diffsims/pattern/__init__.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/pattern/detector_functions.py` & `diffsims-0.5.2/diffsims/pattern/detector_functions.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/release_info.py` & `diffsims-0.5.2/diffsims/release_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 name = "diffsims"
-version = "0.5.1"
+version = "0.5.2"
 author = "Duncan Johnstone, Phillip Crout"
-copyright = "Copyright 2017-2022, The diffsims developers"
+copyright = "Copyright 2017-2023, The diffsims developers"
 # Initial committer first, then listed by line additions
 credits = [
     "Duncan Johnstone",
     "Phillip Crout",
     "Håkon Wiik Ånes",
     "Eric Prestat",
     "Rob Tovey",
```

### Comparing `diffsims-0.5.1/diffsims/sims/__init__.py` & `diffsims-0.5.2/diffsims/sims/__init__.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/sims/diffraction_simulation.py` & `diffsims-0.5.2/diffsims/sims/diffraction_simulation.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/structure_factor/__init__.py` & `diffsims-0.5.2/diffsims/structure_factor/__init__.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/structure_factor/atomic_scattering_factor.py` & `diffsims-0.5.2/diffsims/structure_factor/atomic_scattering_factor.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/structure_factor/atomic_scattering_parameters.py` & `diffsims-0.5.2/diffsims/structure_factor/atomic_scattering_parameters.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/structure_factor/structure_factor.py` & `diffsims-0.5.2/diffsims/structure_factor/structure_factor.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/__init__.py` & `diffsims-0.5.2/diffsims/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/crystallography/__init__.py` & `diffsims-0.5.2/diffsims/tests/crystallography/__init__.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/crystallography/test_reciprocal_lattice_point.py` & `diffsims-0.5.2/diffsims/tests/crystallography/test_reciprocal_lattice_point.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/crystallography/test_reciprocal_lattice_vector.py` & `diffsims-0.5.2/diffsims/tests/crystallography/test_reciprocal_lattice_vector.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/generators/__init__.py` & `diffsims-0.5.2/diffsims/tests/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/generators/test_diffraction_generator.py` & `diffsims-0.5.2/diffsims/tests/generators/test_diffraction_generator.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/generators/test_library_generator.py` & `diffsims-0.5.2/diffsims/tests/generators/test_library_generator.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/generators/test_rotation_list_generator.py` & `diffsims-0.5.2/diffsims/tests/generators/test_rotation_list_generator.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/generators/test_sphere_mesh_generators.py` & `diffsims-0.5.2/diffsims/tests/generators/test_sphere_mesh_generators.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/generators/test_zap_map_generator.py` & `diffsims-0.5.2/diffsims/tests/generators/test_zap_map_generator.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/library/__init__.py` & `diffsims-0.5.2/diffsims/tests/library/__init__.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/library/test_diffraction_library.py` & `diffsims-0.5.2/diffsims/tests/library/test_diffraction_library.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/library/test_structure_library.py` & `diffsims-0.5.2/diffsims/tests/library/test_structure_library.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/library/test_vector_library.py` & `diffsims-0.5.2/diffsims/tests/library/test_vector_library.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/patterns/__init__.py` & `diffsims-0.5.2/diffsims/tests/patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/patterns/test_detector_functions.py` & `diffsims-0.5.2/diffsims/tests/patterns/test_detector_functions.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/sims/__init__.py` & `diffsims-0.5.2/diffsims/tests/sims/__init__.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/sims/test_diffraction_simulation.py` & `diffsims-0.5.2/diffsims/tests/sims/test_diffraction_simulation.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/structure_factor/__init__.py` & `diffsims-0.5.2/diffsims/tests/structure_factor/__init__.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/structure_factor/test_atomic_scattering_factor.py` & `diffsims-0.5.2/diffsims/tests/structure_factor/test_atomic_scattering_factor.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/structure_factor/test_atomic_scattering_parameters.py` & `diffsims-0.5.2/diffsims/tests/structure_factor/test_atomic_scattering_parameters.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/structure_factor/test_structure_factor.py` & `diffsims-0.5.2/diffsims/tests/structure_factor/test_structure_factor.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/utils/__init__.py` & `diffsims-0.5.2/diffsims/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/utils/test_atomic_diffraction_generator_utils.py` & `diffsims-0.5.2/diffsims/tests/utils/test_atomic_diffraction_generator_utils.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/utils/test_discretise_utils.py` & `diffsims-0.5.2/diffsims/tests/utils/test_discretise_utils.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/utils/test_fourier_transform.py` & `diffsims-0.5.2/diffsims/tests/utils/test_fourier_transform.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/utils/test_generic_utils.py` & `diffsims-0.5.2/diffsims/tests/utils/test_generic_utils.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/utils/test_kinematic_simulation_utils.py` & `diffsims-0.5.2/diffsims/tests/utils/test_kinematic_simulation_utils.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/utils/test_mask_utils.py` & `diffsims-0.5.2/diffsims/tests/utils/test_mask_utils.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/utils/test_probe_utils.py` & `diffsims-0.5.2/diffsims/tests/utils/test_probe_utils.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/utils/test_ring_pattern_utils.py` & `diffsims-0.5.2/diffsims/tests/utils/test_ring_pattern_utils.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/utils/test_sim_utils.py` & `diffsims-0.5.2/diffsims/tests/utils/test_sim_utils.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/tests/utils/test_vector_utils.py` & `diffsims-0.5.2/diffsims/tests/utils/test_vector_utils.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/utils/__init__.py` & `diffsims-0.5.2/diffsims/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/utils/atomic_diffraction_generator_utils.py` & `diffsims-0.5.2/diffsims/utils/atomic_diffraction_generator_utils.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/utils/atomic_scattering_params.py` & `diffsims-0.5.2/diffsims/utils/atomic_scattering_params.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/utils/discretise_utils.py` & `diffsims-0.5.2/diffsims/utils/discretise_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,51 +134,51 @@
 
 ##########
 # Evaluate single atom intensities
 ##########
 
 
 # Coverage: Numba code does not register when code is run
-@numba.jit(fastmath=True, nopython=True)
+@numba.njit(fastmath=True)
 def __linear_interp(x, i, arr):  # pragma: no cover
     # First order Lagrange interpolation: x_0=0, x_1=1
     # L_0(x) = (x-x_1)/(x_0-x_1) = 1-x
     # L_1(x) = (x-x_0)/(x_1-x_0) = x
     return (1 - x) * arr[i] + x * arr[i + 1]
 
 
 # Coverage: Numba code does not register when code is run
-@numba.jit(fastmath=True, nopython=True)
+@numba.njit(fastmath=True)
 def __quadratic_interp(x, i, arr):  # pragma: no cover
     # Second order Lagrange interpolation: x_0=-1, x_1=0, x_2=1
     # L_0(x) = (x-x_1)*(x-x_2)/(x_0-x_1)/(x_0-x_2) = x*(x-1)/-1/-2 = x(x-1)/2
     # L_1(x) = (x-x_0)*(x-x_2)/(x_1-x_0)/(x_1-x_2) = (x+1)*(x-1)/1/-1= 1-x^2
     # L_2(x) = (x-x_0)*(x-x_1)/(x_2-x_0)/(x_2-x_1) = (x+1)*x/2/1 = x(x+1)/2
     x2 = x * x
     if i == 0:  # arr[1] = arr[-1]
         return x2 * arr[1] + (1 - x2) * arr[0]
     return 0.5 * ((x2 - x) * arr[i - 1] + (x2 + x) * arr[i + 1]) + (1 - x2) * arr[i]
 
 
 # Coverage: Numba code does not register when code is run
-@numba.jit(fastmath=True, nopython=True)
+@numba.njit(fastmath=True)
 def __atom_pw_cpu(x0, x1, x2, pc, h):  # pragma: no cover
     n = x0 * x0 + x1 * x1 + x2 * x2
     if n >= h[0]:
         return 0
     else:
         n = h[1] * c_sqrt(n)
         i = int(n)
         n -= i
         #         return __linear_interp(n, i, pc)
         return __quadratic_interp(n, i, pc)
 
 
 # Coverage: Numba code does not register when code is run
-@numba.jit(fastmath=True, nopython=True)
+@numba.njit(fastmath=True)
 def __atom_av_cpu(x0, x1, x2, pc, h):  # pragma: no cover
     x0, x1, x2 = c_abs(x0), c_abs(x1), c_abs(x2)
     if x0 > h[0, 0] or x1 > h[0, 1] or x2 > h[0, 2]:
         return 0
 
     x0, x1, x2 = h[1, 0] * x0, h[1, 1] * x1, h[1, 2] * x2
     i0, i1, i2 = int(x0), int(x1), int(x2)
@@ -241,30 +241,30 @@
         return s
 
 
 ##########
 # Binning list of atoms into a grid for efficiency
 ##########
 # Coverage: Numba code does not register when code is run
-@numba.jit(cache=True)
+@numba.njit(cache=True)
 def __countbins(x0, x1, x2, loc, r, s, Len, MAX):  # pragma: no cover
     for j0 in range(loc.shape[0]):
         bin0 = int((loc[j0, 0] - x0) / r[0])
         bin1 = int((loc[j0, 1] - x1) / r[1])
         bin2 = int((loc[j0, 2] - x2) / r[2])
         for i in range(max(0, bin0 - s), min(Len.shape[0], bin0 + s + 1)):
             for j in range(max(0, bin1 - s), min(Len.shape[1], bin1 + s + 1)):
                 for k in range(max(0, bin2 - s), min(Len.shape[2], bin2 + s + 1)):
                     Len[i, j, k] += 1
                     if Len[i, j, k] == MAX:
                         return
 
 
 # Coverage: Numba code does not register when code is run
-@numba.jit(cache=True)
+@numba.njit(cache=True)
 def __rebin(x0, x1, x2, loc, sublist, r, s, Len):  # pragma: no cover
     for j0 in range(loc.shape[0]):
         bin0 = int((loc[j0, 0] - x0) / r[0])
         bin1 = int((loc[j0, 1] - x1) / r[1])
         bin2 = int((loc[j0, 2] - x2) / r[2])
         for i in range(max(0, bin0 - s), min(Len.shape[0], bin0 + s + 1)):
             for j in range(max(0, bin1 - s), min(Len.shape[1], bin1 + s + 1)):
@@ -400,15 +400,15 @@
             return subList, r, mem
 
 
 ##########
 # Discretise whole crystal
 ##########
 # Coverage: Numba code does not register when code is run
-@numba.jit(parallel=True, fastmath=True, nopython=True)
+@numba.njit(parallel=True, fastmath=True)
 def __density3D_pw_cpu(
     x0, x1, x2, xmin, loc, sublist, r, a, d, B, precomp, h, out
 ):  # pragma: no cover
     X0 = x0
     bin0 = int(floor((X0 - xmin[0]) / r[0]))
     if bin0 >= sublist.shape[0]:
         return
@@ -432,15 +432,15 @@
                 Y1 = loc[j0, 1] - X1
                 Y2 = loc[j0, 2] - X2
                 Sum += __atom_pw_cpu(Y0, Y1, Y2, precomp, h)
             out[i1, i2] = Sum
 
 
 # Coverage: Numba code does not register when code is run
-@numba.jit(parallel=True, fastmath=True, nopython=True)
+@numba.njit(parallel=True, fastmath=True)
 def __density3D_av_cpu(
     x0, x1, x2, xmin, loc, sublist, r, a, d, B, precomp, h, out
 ):  # pragma: no cover
     X0 = x0
     bin0 = int(floor((X0 - xmin[0]) / r[0]))
     if bin0 >= sublist.shape[0]:
         return
@@ -464,15 +464,15 @@
                 Y1 = loc[j0, 1] - X1
                 Y2 = loc[j0, 2] - X2
                 Sum += __atom_av_cpu(Y0, Y1, Y2, precomp, h)
             out[i1, i2] = Sum
 
 
 # Coverage: Numba code does not register when code is run
-@numba.jit(parallel=True, fastmath=True, nopython=True)
+@numba.njit(parallel=True, fastmath=True)
 def __FT3D_pw_cpu(x0, x1, x2, loc, a, b, d, B, precomp, h, out):  # pragma: no cover
     X0 = x0
     for i1 in numba.prange(x1.size):
         X1 = x1[i1]
         for i2 in range(x2.size):
             X2 = x2[i2]
             scale = __atom_pw_cpu(X0, X1, X2, precomp, h)
@@ -482,15 +482,15 @@
                 IP = loc[j0, 0] * X0 + loc[j0, 1] * X1 + loc[j0, 2] * X2
                 Sum += complex(scale * c_cos(IP), -scale * c_sin(IP))
 
             out[i1, i2] = Sum
 
 
 # Coverage: Numba code does not register when code is run
-@numba.jit(parallel=True, fastmath=True, nopython=True)
+@numba.njit(parallel=True, fastmath=True)
 def __FT3D_av_cpu(x0, x1, x2, loc, a, b, d, B, precomp, h, out):  # pragma: no cover
     X0 = x0
     for i1 in numba.prange(x1.size):
         X1 = x1[i1]
         for i2 in range(x2.size):
             X2 = x2[i2]
             scale = __atom_av_cpu(X0, X1, X2, precomp, h)
```

### Comparing `diffsims-0.5.1/diffsims/utils/fourier_transform.py` & `diffsims-0.5.2/diffsims/utils/fourier_transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -348,32 +348,32 @@
         __fftshift_phase2(x)
     else:
         __fftshift_phase3(x)
     return x.reshape(sz)
 
 
 # Coverage: Numba code does not register when code is run
-@numba.jit(nopython=True, parallel=True, fastmath=True)
+@numba.njit(parallel=True, fastmath=True)
 def __fftshift_phase1(x):  # pragma: no cover
     sz = x.shape[0] // 2
     for i in numba.prange(sz):
         x[2 * i + 1] = -x[2 * i + 1]
 
 
 # Coverage: Numba code does not register when code is run
-@numba.jit(nopython=True, parallel=True, fastmath=True)
+@numba.njit(parallel=True, fastmath=True)
 def __fftshift_phase2(x):  # pragma: no cover
     for i in numba.prange(x.shape[0]):
         start = (i + 1) % 2
         for j in range(start, x.shape[1], 2):
             x[i, j] = -x[i, j]
 
 
 # Coverage: Numba code does not register when code is run
-@numba.jit(nopython=True, parallel=True, fastmath=True)
+@numba.njit(parallel=True, fastmath=True)
 def __fftshift_phase3(x):  # pragma: no cover
     for i in numba.prange(x.shape[0]):
         for j in range(x.shape[1]):
             start = (i + j + 1) % 2
             for k in range(start, x.shape[2], 2):
                 x[i, j, k] = -x[i, j, k]
 
@@ -397,15 +397,15 @@
     if y is None:
         y = empty(x.shape, dtype=abs(x[(slice(1),) * x.ndim]).dtype)
     __fast_abs(x.reshape(-1), y.reshape(-1))
     return y
 
 
 # Coverage: Numba code does not register when code is run
-@numba.jit(nopython=True, parallel=True, fastmath=True)
+@numba.njit(parallel=True, fastmath=True)
 def __fast_abs(x, y):  # pragma: no cover
     for i in numba.prange(x.size):
         y[i] = abs(x[i])
 
 
 def to_recip(x):
     """
@@ -556,15 +556,15 @@
         Y = to_recip(X)
 
     ndim = len(X)
     dx = [x.item(min(1, x.size - 1)) - x.item(0) for x in X]
     xmin = [x.item(0) for x in X]
 
     # Coverage: Numba code does not register when code is run
-    @numba.jit(nopython=True, parallel=True, fastmath=True)
+    @numba.njit(parallel=True, fastmath=True)
     def apply_phase_3D(x, f0, f1, f2):  # pragma: no cover
         for i0 in numba.prange(x.shape[0]):
             F0 = f0[i0]
             for i1 in range(x.shape[1]):
                 F01 = F0 * f1[i1]
                 for i2 in range(x.shape[2]):
                     x[i0, i1, i2] *= F01 * f2[i2]
```

### Comparing `diffsims-0.5.1/diffsims/utils/generic_utils.py` & `diffsims-0.5.2/diffsims/utils/generic_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,26 +80,26 @@
                 tpb[i] -= 1
             grid[i] = sz[i] // tpb[i]
 
     return grid, tpb
 
 
 # Coverage: Numba code does not register when code is run
-@numba.jit(parallel=True, fastmath=True, cache=False, nopython=True)
+@numba.njit(parallel=True, fastmath=True, cache=False)
 def __toMesh2d(x0, x1, dx0, dx1, out):  # pragma: no cover
     for i0 in numba.prange(x0.size):
         X00 = x0[i0] * dx0[0]
         X01 = x0[i0] * dx0[1]
         for i1 in range(x1.size):
             out[i0, i1, 0] = X00 + x1[i1] * dx1[0]
             out[i0, i1, 1] = X01 + x1[i1] * dx1[1]
 
 
 # Coverage: Numba code does not register when code is run
-@numba.jit(parallel=True, fastmath=True, cache=False, nopython=True)
+@numba.njit(parallel=True, fastmath=True, cache=False)
 def __toMesh3d(x0, x1, x2, dx0, dx1, dx2, out):  # pragma: no cover
     for i0 in numba.prange(x0.size):
         X00 = x0[i0] * dx0[0]
         X01 = x0[i0] * dx0[1]
         X02 = x0[i0] * dx0[2]
         for i1 in range(x1.size):
             X10 = x1[i1] * dx1[0]
```

### Comparing `diffsims-0.5.1/diffsims/utils/kinematic_simulation_utils.py` & `diffsims-0.5.2/diffsims/utils/kinematic_simulation_utils.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/utils/lobato_scattering_params.py` & `diffsims-0.5.2/diffsims/utils/lobato_scattering_params.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/utils/mask_utils.py` & `diffsims-0.5.2/diffsims/utils/mask_utils.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/utils/probe_utils.py` & `diffsims-0.5.2/diffsims/utils/probe_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,15 +246,15 @@
                     out = (2 * pi * r ** 2) * (abs(y * y).sum(-1) <= 1 / r ** 2)
                 else:
                     out[...] = (2 * pi * r ** 2) * (abs(y * y).sum(-1) <= 1 / r ** 2)
         return out
 
 
 # Coverage: Numba code does not register when code is run
-@numba.jit(nopython=True, parallel=True, fastmath=True)
+@numba.njit(parallel=True, fastmath=True)
 def _bess(X, R, H, J, scale, out):  # pragma: no cover
     if scale.size == 1:
         for i in numba.prange(X.shape[0]):
             rad = c_sqrt(X[i, 0] * X[i, 0] + X[i, 1] * X[i, 1]) * R
             ind = int(rad * H)
             if ind < J.size:
                 out[i] = J[ind]
@@ -267,15 +267,15 @@
             if ind < J.size:
                 out[i] = scale[i] * J[ind]
             else:
                 out[i] = 0
 
 
 # Coverage: Numba code does not register when code is run
-@numba.jit(nopython=True, parallel=True, fastmath=True)
+@numba.njit(parallel=True, fastmath=True)
 def _bessFT(X, R, s, eps, out):  # pragma: no cover
     for i in numba.prange(X.shape[0]):
         rad = X[i, 0] * X[i, 0] + X[i, 1] * X[i, 1]
         if rad > R or abs(X[i, 2]) > eps:
             out[i] = 0
         else:
             out[i] = s
```

### Comparing `diffsims-0.5.1/diffsims/utils/ring_pattern_utils.py` & `diffsims-0.5.2/diffsims/utils/ring_pattern_utils.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/utils/scattering_params.py` & `diffsims-0.5.2/diffsims/utils/scattering_params.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/utils/shape_factor_models.py` & `diffsims-0.5.2/diffsims/utils/shape_factor_models.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/utils/sim_utils.py` & `diffsims-0.5.2/diffsims/utils/sim_utils.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims/utils/vector_utils.py` & `diffsims-0.5.2/diffsims/utils/vector_utils.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/diffsims.egg-info/PKG-INFO` & `diffsims-0.5.2/diffsims.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffsims
-Version: 0.5.1
+Version: 0.5.2
 Summary: Diffraction Simulations in Python
 Home-page: https://github.com/pyxem/diffsims
 Author: Duncan Johnstone, Phillip Crout
 Author-email: pyxem.team@gmail.com
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `diffsims-0.5.1/diffsims.egg-info/SOURCES.txt` & `diffsims-0.5.2/diffsims.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/doc/Makefile` & `diffsims-0.5.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/doc/conf.py` & `diffsims-0.5.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/doc/installation.rst` & `diffsims-0.5.2/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/doc/make.bat` & `diffsims-0.5.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/doc/reference.rst` & `diffsims-0.5.2/doc/reference.rst`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/doc/related_projects.rst` & `diffsims-0.5.2/doc/related_projects.rst`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/readthedocs.yaml` & `diffsims-0.5.2/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.1/setup.py` & `diffsims-0.5.2/setup.py`

 * *Files identical despite different names*

