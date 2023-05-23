# Comparing `tmp/geoh5py-0.8.0a1.tar.gz` & `tmp/geoh5py-0.8.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoh5py-0.8.0a1.tar", max compression
+gzip compressed data, was "geoh5py-0.8.0a2.tar", max compression
```

## Comparing `geoh5py-0.8.0a1.tar` & `geoh5py-0.8.0a2.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0      841 2023-04-27 16:38:56.715801 geoh5py-0.8.0a1/geoh5py/__init__.py
--rw-r--r--   0        0        0     1486 2023-01-27 16:07:08.404026 geoh5py-0.8.0a1/geoh5py/data/__init__.py
--rw-r--r--   0        0        0     1311 2023-01-27 16:07:08.405036 geoh5py-0.8.0a1/geoh5py/data/blob_data.py
--rw-r--r--   0        0        0     3948 2023-03-27 18:34:50.646957 geoh5py-0.8.0a1/geoh5py/data/color_map.py
--rw-r--r--   0        0        0     8158 2023-04-04 17:51:20.060566 geoh5py-0.8.0a1/geoh5py/data/data.py
--rw-r--r--   0        0        0     1138 2023-01-27 16:07:08.407026 geoh5py-0.8.0a1/geoh5py/data/data_association_enum.py
--rw-r--r--   0        0        0     9612 2023-03-16 20:09:06.192137 geoh5py-0.8.0a1/geoh5py/data/data_type.py
--rw-r--r--   0        0        0     1138 2023-01-27 16:07:08.408028 geoh5py-0.8.0a1/geoh5py/data/data_unit.py
--rw-r--r--   0        0        0     1340 2023-02-09 14:27:13.492642 geoh5py-0.8.0a1/geoh5py/data/datetime_data.py
--rw-r--r--   0        0        0     3698 2023-03-16 20:09:06.192137 geoh5py-0.8.0a1/geoh5py/data/filename_data.py
--rw-r--r--   0        0        0     1218 2023-01-27 16:07:08.410027 geoh5py-0.8.0a1/geoh5py/data/float_data.py
--rw-r--r--   0        0        0     1625 2023-01-27 16:07:08.411061 geoh5py-0.8.0a1/geoh5py/data/geometric_data_constants.py
--rw-r--r--   0        0        0     2415 2023-01-27 16:07:08.412062 geoh5py-0.8.0a1/geoh5py/data/integer_data.py
--rw-r--r--   0        0        0     3473 2023-04-27 16:38:56.716801 geoh5py-0.8.0a1/geoh5py/data/numeric_data.py
--rw-r--r--   0        0        0     1103 2023-01-27 16:07:08.413026 geoh5py-0.8.0a1/geoh5py/data/primitive_type_enum.py
--rw-r--r--   0        0        0     1649 2023-01-27 16:07:08.413026 geoh5py-0.8.0a1/geoh5py/data/reference_value_map.py
--rw-r--r--   0        0        0     1531 2023-01-27 16:07:08.414026 geoh5py-0.8.0a1/geoh5py/data/referenced_data.py
--rw-r--r--   0        0        0     4445 2023-03-16 20:09:06.193137 geoh5py-0.8.0a1/geoh5py/data/text_data.py
--rw-r--r--   0        0        0     1571 2023-01-27 16:07:08.415027 geoh5py-0.8.0a1/geoh5py/data/unknown_data.py
--rw-r--r--   0        0        0     1587 2023-01-27 16:07:08.416026 geoh5py-0.8.0a1/geoh5py/groups/__init__.py
--rw-r--r--   0        0        0     1495 2023-01-27 16:07:08.416026 geoh5py-0.8.0a1/geoh5py/groups/container_group.py
--rw-r--r--   0        0        0     1449 2023-01-27 16:07:08.416026 geoh5py-0.8.0a1/geoh5py/groups/custom_group.py
--rw-r--r--   0        0        0     1851 2023-03-16 20:09:06.194139 geoh5py-0.8.0a1/geoh5py/groups/drillhole_group.py
--rw-r--r--   0        0        0     1498 2023-01-27 16:07:08.417027 geoh5py-0.8.0a1/geoh5py/groups/giftools_group.py
--rw-r--r--   0        0        0     6311 2023-03-27 18:34:50.648948 geoh5py-0.8.0a1/geoh5py/groups/group.py
--rw-r--r--   0        0        0     3698 2023-01-27 16:07:08.418027 geoh5py-0.8.0a1/geoh5py/groups/group_type.py
--rw-r--r--   0        0        0     7324 2023-01-27 16:07:08.419027 geoh5py-0.8.0a1/geoh5py/groups/integrator_group.py
--rw-r--r--   0        0        0     1311 2023-01-27 16:07:08.420026 geoh5py-0.8.0a1/geoh5py/groups/maps_group.py
--rw-r--r--   0        0        0     1468 2023-01-27 16:07:08.420026 geoh5py-0.8.0a1/geoh5py/groups/notype_group.py
--rw-r--r--   0        0        0     4449 2023-03-16 20:09:06.195138 geoh5py-0.8.0a1/geoh5py/groups/property_group.py
--rw-r--r--   0        0        0     1593 2023-01-27 16:07:08.421026 geoh5py-0.8.0a1/geoh5py/groups/root_group.py
--rw-r--r--   0        0        0     2107 2023-04-27 16:38:56.717802 geoh5py-0.8.0a1/geoh5py/groups/simpeg_group.py
--rw-r--r--   0        0        0     1338 2023-01-27 16:07:08.422027 geoh5py-0.8.0a1/geoh5py/groups/survey_group.py
--rw-r--r--   0        0        0      866 2023-01-27 16:07:08.429046 geoh5py-0.8.0a1/geoh5py/io/__init__.py
--rw-r--r--   0        0        0    17088 2023-03-16 20:09:06.195138 geoh5py-0.8.0a1/geoh5py/io/h5_reader.py
--rw-r--r--   0        0        0    32435 2023-04-27 16:38:56.717802 geoh5py-0.8.0a1/geoh5py/io/h5_writer.py
--rw-r--r--   0        0        0     2223 2023-04-27 16:38:56.718801 geoh5py-0.8.0a1/geoh5py/objects/__init__.py
--rw-r--r--   0        0        0     9496 2023-03-16 20:09:06.197153 geoh5py-0.8.0a1/geoh5py/objects/block_model.py
--rw-r--r--   0        0        0     7803 2023-03-27 18:34:50.649448 geoh5py-0.8.0a1/geoh5py/objects/cell_object.py
--rw-r--r--   0        0        0     6283 2023-03-16 20:09:06.198164 geoh5py-0.8.0a1/geoh5py/objects/curve.py
--rw-r--r--   0        0        0     5129 2023-03-16 20:09:06.198164 geoh5py-0.8.0a1/geoh5py/objects/drape_model.py
--rw-r--r--   0        0        0    25527 2023-03-27 18:34:50.650448 geoh5py-0.8.0a1/geoh5py/objects/drillhole.py
--rw-r--r--   0        0        0    16653 2023-03-27 18:34:50.650948 geoh5py-0.8.0a1/geoh5py/objects/geo_image.py
--rw-r--r--   0        0        0    13506 2023-03-27 18:34:50.651448 geoh5py-0.8.0a1/geoh5py/objects/grid2d.py
--rw-r--r--   0        0        0     4775 2023-03-27 18:34:50.651948 geoh5py-0.8.0a1/geoh5py/objects/grid_object.py
--rw-r--r--   0        0        0     1919 2023-03-16 20:09:06.201539 geoh5py-0.8.0a1/geoh5py/objects/integrator.py
--rw-r--r--   0        0        0     2977 2023-03-27 18:34:50.652448 geoh5py-0.8.0a1/geoh5py/objects/label.py
--rw-r--r--   0        0        0     2890 2023-03-27 18:34:50.652948 geoh5py-0.8.0a1/geoh5py/objects/notype_object.py
--rw-r--r--   0        0        0    17763 2023-03-27 18:34:50.653448 geoh5py-0.8.0a1/geoh5py/objects/object_base.py
--rw-r--r--   0        0        0     2748 2023-01-27 16:07:08.438024 geoh5py-0.8.0a1/geoh5py/objects/object_type.py
--rw-r--r--   0        0        0    13349 2023-03-16 20:09:06.203794 geoh5py-0.8.0a1/geoh5py/objects/octree.py
--rw-r--r--   0        0        0     5410 2023-03-27 18:34:50.653948 geoh5py-0.8.0a1/geoh5py/objects/points.py
--rw-r--r--   0        0        0     2588 2023-03-16 20:09:06.204796 geoh5py-0.8.0a1/geoh5py/objects/surface.py
--rw-r--r--   0        0        0      747 2023-01-27 16:07:08.440024 geoh5py-0.8.0a1/geoh5py/objects/surveys/__init__.py
--rw-r--r--   0        0        0    14570 2023-03-16 20:09:06.205794 geoh5py-0.8.0a1/geoh5py/objects/surveys/direct_current.py
--rw-r--r--   0        0        0      747 2023-01-27 16:07:08.441024 geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/__init__.py
--rw-r--r--   0        0        0     3660 2023-04-27 16:38:56.718801 geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/airborne_fem.py
--rw-r--r--   0        0        0     3629 2023-04-27 16:38:56.719810 geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/airborne_tem.py
--rw-r--r--   0        0        0    35608 2023-04-27 16:38:56.719810 geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/base.py
--rw-r--r--   0        0        0     6925 2023-04-27 16:38:56.720802 geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/ground_fem.py
--rw-r--r--   0        0        0     7019 2023-04-27 16:38:56.720802 geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/ground_tem.py
--rw-r--r--   0        0        0     2615 2023-04-27 16:38:56.721800 geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py
--rw-r--r--   0        0        0     6636 2023-04-27 16:38:56.722800 geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/tipper.py
--rw-r--r--   0        0        0     1247 2023-01-27 16:07:08.443024 geoh5py-0.8.0a1/geoh5py/objects/surveys/magnetics.py
--rw-r--r--   0        0        0        0 2023-03-27 18:34:50.654950 geoh5py-0.8.0a1/geoh5py/py.typed
--rw-r--r--   0        0        0     1015 2023-01-27 16:07:08.444702 geoh5py-0.8.0a1/geoh5py/shared/__init__.py
--rw-r--r--   0        0        0    37812 2023-03-27 18:34:50.655448 geoh5py-0.8.0a1/geoh5py/shared/concatenation.py
--rw-r--r--   0        0        0      937 2023-01-27 16:07:08.446085 geoh5py-0.8.0a1/geoh5py/shared/conversion/__init__.py
--rw-r--r--   0        0        0     4287 2023-01-27 16:07:08.446085 geoh5py-0.8.0a1/geoh5py/shared/conversion/base.py
--rw-r--r--   0        0        0     7599 2023-01-27 16:07:08.446085 geoh5py-0.8.0a1/geoh5py/shared/conversion/geo_image.py
--rw-r--r--   0        0        0     8083 2023-03-16 20:09:06.209634 geoh5py-0.8.0a1/geoh5py/shared/conversion/grid2d.py
--rw-r--r--   0        0        0    16876 2023-03-27 18:34:50.656448 geoh5py-0.8.0a1/geoh5py/shared/entity.py
--rw-r--r--   0        0        0     4275 2023-03-16 20:09:06.210634 geoh5py-0.8.0a1/geoh5py/shared/entity_type.py
--rw-r--r--   0        0        0     5732 2023-03-16 20:09:06.211635 geoh5py-0.8.0a1/geoh5py/shared/exceptions.py
--rw-r--r--   0        0        0    15205 2023-04-27 16:38:56.722800 geoh5py-0.8.0a1/geoh5py/shared/utils.py
--rw-r--r--   0        0        0     8969 2023-04-27 16:38:56.723802 geoh5py-0.8.0a1/geoh5py/shared/validators.py
--rw-r--r--   0        0        0     2647 2023-01-27 16:07:08.451084 geoh5py-0.8.0a1/geoh5py/shared/weakref_utils.py
--rw-r--r--   0        0        0      921 2023-01-27 16:07:08.452070 geoh5py-0.8.0a1/geoh5py/ui_json/__init__.py
--rw-r--r--   0        0        0     2936 2023-01-27 16:07:08.452070 geoh5py-0.8.0a1/geoh5py/ui_json/constants.py
--rw-r--r--   0        0        0    18349 2023-04-27 16:38:56.723802 geoh5py-0.8.0a1/geoh5py/ui_json/input_file.py
--rw-r--r--   0        0        0    11946 2023-04-27 16:38:56.724800 geoh5py-0.8.0a1/geoh5py/ui_json/templates.py
--rw-r--r--   0        0        0    10990 2023-04-27 16:38:56.724800 geoh5py-0.8.0a1/geoh5py/ui_json/utils.py
--rw-r--r--   0        0        0    10777 2023-04-27 16:38:56.725800 geoh5py-0.8.0a1/geoh5py/ui_json/validation.py
--rw-r--r--   0        0        0      852 2023-01-27 16:07:08.455078 geoh5py-0.8.0a1/geoh5py/workspace/__init__.py
--rw-r--r--   0        0        0    42630 2023-04-27 16:38:56.726801 geoh5py-0.8.0a1/geoh5py/workspace/workspace.py
--rw-r--r--   0        0        0     2111 2023-01-27 16:07:08.456070 geoh5py-0.8.0a1/package.rst
--rw-r--r--   0        0        0     2500 2023-04-27 16:51:35.348107 geoh5py-0.8.0a1/pyproject.toml
--rw-r--r--   0        0        0     3419 1970-01-01 00:00:00.000000 geoh5py-0.8.0a1/PKG-INFO
+-rw-r--r--   0        0        0      841 2023-05-23 20:32:29.218825 geoh5py-0.8.0a2/geoh5py/__init__.py
+-rw-r--r--   0        0        0     1486 2023-01-19 16:31:21.807961 geoh5py-0.8.0a2/geoh5py/data/__init__.py
+-rw-r--r--   0        0        0     1311 2023-01-19 16:31:21.808963 geoh5py-0.8.0a2/geoh5py/data/blob_data.py
+-rw-r--r--   0        0        0     3948 2023-03-23 18:19:17.279345 geoh5py-0.8.0a2/geoh5py/data/color_map.py
+-rw-r--r--   0        0        0     8158 2023-05-19 15:54:32.029195 geoh5py-0.8.0a2/geoh5py/data/data.py
+-rw-r--r--   0        0        0     1138 2023-01-19 16:31:21.812966 geoh5py-0.8.0a2/geoh5py/data/data_association_enum.py
+-rw-r--r--   0        0        0     9612 2023-02-16 17:03:47.933513 geoh5py-0.8.0a2/geoh5py/data/data_type.py
+-rw-r--r--   0        0        0     1138 2023-01-19 16:31:21.814488 geoh5py-0.8.0a2/geoh5py/data/data_unit.py
+-rw-r--r--   0        0        0     1340 2023-02-07 15:33:21.371480 geoh5py-0.8.0a2/geoh5py/data/datetime_data.py
+-rw-r--r--   0        0        0     3690 2023-05-23 20:32:29.220547 geoh5py-0.8.0a2/geoh5py/data/filename_data.py
+-rw-r--r--   0        0        0     1218 2023-01-19 16:31:21.818527 geoh5py-0.8.0a2/geoh5py/data/float_data.py
+-rw-r--r--   0        0        0     1625 2023-01-19 16:31:21.819552 geoh5py-0.8.0a2/geoh5py/data/geometric_data_constants.py
+-rw-r--r--   0        0        0     2415 2023-05-19 15:54:32.031196 geoh5py-0.8.0a2/geoh5py/data/integer_data.py
+-rw-r--r--   0        0        0     3473 2023-05-19 15:54:32.032196 geoh5py-0.8.0a2/geoh5py/data/numeric_data.py
+-rw-r--r--   0        0        0     1103 2023-01-19 16:31:21.823165 geoh5py-0.8.0a2/geoh5py/data/primitive_type_enum.py
+-rw-r--r--   0        0        0     1649 2023-01-19 16:31:21.824214 geoh5py-0.8.0a2/geoh5py/data/reference_value_map.py
+-rw-r--r--   0        0        0     1531 2023-01-19 16:31:21.825276 geoh5py-0.8.0a2/geoh5py/data/referenced_data.py
+-rw-r--r--   0        0        0     4445 2023-05-19 15:54:32.033195 geoh5py-0.8.0a2/geoh5py/data/text_data.py
+-rw-r--r--   0        0        0     1571 2023-01-19 16:31:21.826284 geoh5py-0.8.0a2/geoh5py/data/unknown_data.py
+-rw-r--r--   0        0        0     1587 2023-01-19 16:31:21.827538 geoh5py-0.8.0a2/geoh5py/groups/__init__.py
+-rw-r--r--   0        0        0     1495 2023-01-19 16:31:21.828547 geoh5py-0.8.0a2/geoh5py/groups/container_group.py
+-rw-r--r--   0        0        0     1449 2023-01-19 16:31:21.829603 geoh5py-0.8.0a2/geoh5py/groups/custom_group.py
+-rw-r--r--   0        0        0     1851 2023-02-16 17:03:47.936515 geoh5py-0.8.0a2/geoh5py/groups/drillhole_group.py
+-rw-r--r--   0        0        0     1498 2023-01-19 16:31:21.833020 geoh5py-0.8.0a2/geoh5py/groups/giftools_group.py
+-rw-r--r--   0        0        0     6311 2023-03-27 17:21:08.995642 geoh5py-0.8.0a2/geoh5py/groups/group.py
+-rw-r--r--   0        0        0     3698 2023-05-19 15:54:32.034195 geoh5py-0.8.0a2/geoh5py/groups/group_type.py
+-rw-r--r--   0        0        0     7362 2023-05-23 20:32:29.222736 geoh5py-0.8.0a2/geoh5py/groups/integrator_group.py
+-rw-r--r--   0        0        0     1349 2023-05-23 20:32:29.225255 geoh5py-0.8.0a2/geoh5py/groups/maps_group.py
+-rw-r--r--   0        0        0     1468 2023-01-19 16:31:21.839544 geoh5py-0.8.0a2/geoh5py/groups/notype_group.py
+-rw-r--r--   0        0        0     4449 2023-02-16 17:03:47.938518 geoh5py-0.8.0a2/geoh5py/groups/property_group.py
+-rw-r--r--   0        0        0     1593 2023-01-19 16:31:21.841554 geoh5py-0.8.0a2/geoh5py/groups/root_group.py
+-rw-r--r--   0        0        0     2107 2023-05-19 15:54:32.035199 geoh5py-0.8.0a2/geoh5py/groups/simpeg_group.py
+-rw-r--r--   0        0        0     1376 2023-05-23 20:32:29.226255 geoh5py-0.8.0a2/geoh5py/groups/survey_group.py
+-rw-r--r--   0        0        0      866 2023-01-19 16:31:21.863215 geoh5py-0.8.0a2/geoh5py/io/__init__.py
+-rw-r--r--   0        0        0    17088 2023-02-16 17:03:47.939518 geoh5py-0.8.0a2/geoh5py/io/h5_reader.py
+-rw-r--r--   0        0        0    32435 2023-05-19 15:54:32.036194 geoh5py-0.8.0a2/geoh5py/io/h5_writer.py
+-rw-r--r--   0        0        0     2223 2023-05-15 22:45:01.215418 geoh5py-0.8.0a2/geoh5py/objects/__init__.py
+-rw-r--r--   0        0        0     9496 2023-05-19 15:54:32.037194 geoh5py-0.8.0a2/geoh5py/objects/block_model.py
+-rw-r--r--   0        0        0     7803 2023-05-19 15:54:32.039194 geoh5py-0.8.0a2/geoh5py/objects/cell_object.py
+-rw-r--r--   0        0        0     6283 2023-05-19 15:54:32.040193 geoh5py-0.8.0a2/geoh5py/objects/curve.py
+-rw-r--r--   0        0        0     5129 2023-05-19 15:54:32.041196 geoh5py-0.8.0a2/geoh5py/objects/drape_model.py
+-rw-r--r--   0        0        0    25527 2023-05-19 15:54:32.042194 geoh5py-0.8.0a2/geoh5py/objects/drillhole.py
+-rw-r--r--   0        0        0    19521 2023-05-23 20:32:29.228772 geoh5py-0.8.0a2/geoh5py/objects/geo_image.py
+-rw-r--r--   0        0        0    14068 2023-05-19 15:54:32.045197 geoh5py-0.8.0a2/geoh5py/objects/grid2d.py
+-rw-r--r--   0        0        0     4775 2023-05-19 15:54:32.046194 geoh5py-0.8.0a2/geoh5py/objects/grid_object.py
+-rw-r--r--   0        0        0     1957 2023-05-23 20:32:29.230772 geoh5py-0.8.0a2/geoh5py/objects/integrator.py
+-rw-r--r--   0        0        0     2977 2023-03-23 18:19:17.298881 geoh5py-0.8.0a2/geoh5py/objects/label.py
+-rw-r--r--   0        0        0     2890 2023-03-23 18:19:17.302902 geoh5py-0.8.0a2/geoh5py/objects/notype_object.py
+-rw-r--r--   0        0        0    17763 2023-05-19 15:54:32.048200 geoh5py-0.8.0a2/geoh5py/objects/object_base.py
+-rw-r--r--   0        0        0     2748 2023-05-19 15:54:32.049219 geoh5py-0.8.0a2/geoh5py/objects/object_type.py
+-rw-r--r--   0        0        0    13349 2023-05-19 15:54:32.050215 geoh5py-0.8.0a2/geoh5py/objects/octree.py
+-rw-r--r--   0        0        0     5410 2023-05-19 15:54:32.051194 geoh5py-0.8.0a2/geoh5py/objects/points.py
+-rw-r--r--   0        0        0     2588 2023-05-19 15:54:32.052205 geoh5py-0.8.0a2/geoh5py/objects/surface.py
+-rw-r--r--   0        0        0      747 2023-01-19 16:31:21.887120 geoh5py-0.8.0a2/geoh5py/objects/surveys/__init__.py
+-rw-r--r--   0        0        0    14570 2023-05-19 15:54:32.054194 geoh5py-0.8.0a2/geoh5py/objects/surveys/direct_current.py
+-rw-r--r--   0        0        0      747 2023-01-19 16:31:21.889161 geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/__init__.py
+-rw-r--r--   0        0        0     3660 2023-05-15 22:45:01.218421 geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/airborne_fem.py
+-rw-r--r--   0        0        0     3629 2023-05-15 22:45:01.219419 geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/airborne_tem.py
+-rw-r--r--   0        0        0    35608 2023-05-19 15:54:32.055195 geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/base.py
+-rw-r--r--   0        0        0     6925 2023-05-15 22:45:01.221455 geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/ground_fem.py
+-rw-r--r--   0        0        0     7019 2023-05-15 22:45:01.222420 geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/ground_tem.py
+-rw-r--r--   0        0        0     2615 2023-05-15 22:45:01.223419 geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py
+-rw-r--r--   0        0        0     6636 2023-05-19 15:54:32.057196 geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/tipper.py
+-rw-r--r--   0        0        0     1247 2023-01-19 16:31:21.895750 geoh5py-0.8.0a2/geoh5py/objects/surveys/magnetics.py
+-rw-r--r--   0        0        0        0 2023-03-17 04:10:56.051740 geoh5py-0.8.0a2/geoh5py/py.typed
+-rw-r--r--   0        0        0     1015 2023-01-19 16:31:21.897759 geoh5py-0.8.0a2/geoh5py/shared/__init__.py
+-rw-r--r--   0        0        0    37812 2023-05-19 15:54:32.058200 geoh5py-0.8.0a2/geoh5py/shared/concatenation.py
+-rw-r--r--   0        0        0      937 2023-02-06 21:13:48.440256 geoh5py-0.8.0a2/geoh5py/shared/conversion/__init__.py
+-rw-r--r--   0        0        0     4287 2023-05-19 15:54:32.060201 geoh5py-0.8.0a2/geoh5py/shared/conversion/base.py
+-rw-r--r--   0        0        0     7599 2023-02-06 21:13:48.440256 geoh5py-0.8.0a2/geoh5py/shared/conversion/geo_image.py
+-rw-r--r--   0        0        0     8083 2023-03-14 13:51:22.342790 geoh5py-0.8.0a2/geoh5py/shared/conversion/grid2d.py
+-rw-r--r--   0        0        0    16884 2023-05-23 20:32:29.232772 geoh5py-0.8.0a2/geoh5py/shared/entity.py
+-rw-r--r--   0        0        0     4275 2023-02-16 17:03:47.959277 geoh5py-0.8.0a2/geoh5py/shared/entity_type.py
+-rw-r--r--   0        0        0     5732 2023-03-14 13:51:22.344785 geoh5py-0.8.0a2/geoh5py/shared/exceptions.py
+-rw-r--r--   0        0        0    15205 2023-05-19 15:54:32.062638 geoh5py-0.8.0a2/geoh5py/shared/utils.py
+-rw-r--r--   0        0        0     8969 2023-05-23 20:32:29.234775 geoh5py-0.8.0a2/geoh5py/shared/validators.py
+-rw-r--r--   0        0        0     2647 2023-01-19 16:31:21.906283 geoh5py-0.8.0a2/geoh5py/shared/weakref_utils.py
+-rw-r--r--   0        0        0      921 2023-01-19 16:31:21.907291 geoh5py-0.8.0a2/geoh5py/ui_json/__init__.py
+-rw-r--r--   0        0        0     2980 2023-05-23 20:32:29.236772 geoh5py-0.8.0a2/geoh5py/ui_json/constants.py
+-rw-r--r--   0        0        0    18369 2023-05-23 20:32:29.238776 geoh5py-0.8.0a2/geoh5py/ui_json/input_file.py
+-rw-r--r--   0        0        0    11946 2023-05-15 22:45:01.229425 geoh5py-0.8.0a2/geoh5py/ui_json/templates.py
+-rw-r--r--   0        0        0    11110 2023-05-23 20:32:29.240784 geoh5py-0.8.0a2/geoh5py/ui_json/utils.py
+-rw-r--r--   0        0        0    10777 2023-05-15 22:45:01.231421 geoh5py-0.8.0a2/geoh5py/ui_json/validation.py
+-rw-r--r--   0        0        0      852 2023-01-19 16:31:21.913295 geoh5py-0.8.0a2/geoh5py/workspace/__init__.py
+-rw-r--r--   0        0        0    42575 2023-05-23 20:32:29.242774 geoh5py-0.8.0a2/geoh5py/workspace/workspace.py
+-rw-r--r--   0        0        0     2111 2023-01-19 16:31:21.916738 geoh5py-0.8.0a2/package.rst
+-rw-r--r--   0        0        0     2501 2023-05-23 20:32:29.249771 geoh5py-0.8.0a2/pyproject.toml
+-rw-r--r--   0        0        0     3419 1970-01-01 00:00:00.000000 geoh5py-0.8.0a2/PKG-INFO
```

### Comparing `geoh5py-0.8.0a1/geoh5py/__init__.py` & `geoh5py-0.8.0a2/geoh5py/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
 
 # flake8: noqa
 
-__version__ = "0.8.0-alpha.1"
+__version__ = "0.8.0-alpha.2"
 
 from geoh5py.workspace import Workspace
```

### Comparing `geoh5py-0.8.0a1/geoh5py/data/__init__.py` & `geoh5py-0.8.0a2/geoh5py/data/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/data/blob_data.py` & `geoh5py-0.8.0a2/geoh5py/data/blob_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/data/color_map.py` & `geoh5py-0.8.0a2/geoh5py/data/color_map.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/data/data.py` & `geoh5py-0.8.0a2/geoh5py/data/data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/data/data_association_enum.py` & `geoh5py-0.8.0a2/geoh5py/data/data_association_enum.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/data/data_type.py` & `geoh5py-0.8.0a2/geoh5py/data/data_type.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/data/data_unit.py` & `geoh5py-0.8.0a2/geoh5py/data/data_unit.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/data/datetime_data.py` & `geoh5py-0.8.0a2/geoh5py/data/datetime_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/data/filename_data.py` & `geoh5py-0.8.0a2/geoh5py/data/filename_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 #  geoh5py is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
+
 from __future__ import annotations
 
-import os
+from pathlib import Path
 
 from .data import Data, PrimitiveTypeEnum
 from .data_type import DataType
 
 
 class FilenameData(Data):
     _file_name: str | None = None
@@ -55,29 +56,27 @@
         if not isinstance(value, (str, type(None))):
             raise ValueError(
                 f"Input 'file_name' for {self} must be of type str or None."
             )
 
         self.workspace.update_attribute(self, "values")
 
-    def save_file(self, path: str = "./", name=None):
+    def save_file(self, path: str | Path = Path(), name=None):
         """
         Save the file to disk.
 
         :param path: Directory to save the file to.
         :param name: Name given to the file.
         """
-        if not os.path.exists(path):
-            os.mkdir(path)
-
+        Path(path).mkdir(exist_ok=True)
         if name is None:
             name = getattr(self, "file_name", "image.tiff")
 
         if self.values is not None:
-            with open(os.path.join(path, name), "wb") as raw_binary:
+            with open(Path(path) / name, "wb") as raw_binary:
                 raw_binary.write(getattr(self, "values"))
 
     @property
     def values(self) -> bytes | None:
         """
         Binary :obj:`str` value representation of a file.
         """
```

### Comparing `geoh5py-0.8.0a1/geoh5py/data/float_data.py` & `geoh5py-0.8.0a2/geoh5py/data/float_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/data/geometric_data_constants.py` & `geoh5py-0.8.0a2/geoh5py/data/geometric_data_constants.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/data/integer_data.py` & `geoh5py-0.8.0a2/geoh5py/data/integer_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/data/numeric_data.py` & `geoh5py-0.8.0a2/geoh5py/data/numeric_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/data/primitive_type_enum.py` & `geoh5py-0.8.0a2/geoh5py/data/primitive_type_enum.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/data/reference_value_map.py` & `geoh5py-0.8.0a2/geoh5py/data/reference_value_map.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/data/referenced_data.py` & `geoh5py-0.8.0a2/geoh5py/data/referenced_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/data/text_data.py` & `geoh5py-0.8.0a2/geoh5py/data/text_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/data/unknown_data.py` & `geoh5py-0.8.0a2/geoh5py/data/unknown_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/groups/__init__.py` & `geoh5py-0.8.0a2/geoh5py/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/groups/container_group.py` & `geoh5py-0.8.0a2/geoh5py/groups/container_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/groups/custom_group.py` & `geoh5py-0.8.0a2/geoh5py/groups/custom_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/groups/drillhole_group.py` & `geoh5py-0.8.0a2/geoh5py/groups/drillhole_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/groups/giftools_group.py` & `geoh5py-0.8.0a2/geoh5py/groups/giftools_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/groups/group.py` & `geoh5py-0.8.0a2/geoh5py/groups/group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/groups/group_type.py` & `geoh5py-0.8.0a2/geoh5py/groups/group_type.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/groups/integrator_group.py` & `geoh5py-0.8.0a2/geoh5py/groups/integrator_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
 
+from __future__ import annotations
+
 import uuid
 
 from .group import Group, GroupType
 
 
 class AirborneTheme(Group):
     """The type for a INTEGRATOR Airborne Theme."""
```

### Comparing `geoh5py-0.8.0a1/geoh5py/groups/maps_group.py` & `geoh5py-0.8.0a2/geoh5py/groups/maps_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
 
+from __future__ import annotations
+
 import uuid
 
 from .group import Group, GroupType
 
 
 class MapsGroup(Group):
     """The type for the basic Container group."""
```

### Comparing `geoh5py-0.8.0a1/geoh5py/groups/notype_group.py` & `geoh5py-0.8.0a2/geoh5py/groups/notype_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/groups/property_group.py` & `geoh5py-0.8.0a2/geoh5py/groups/property_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/groups/root_group.py` & `geoh5py-0.8.0a2/geoh5py/groups/root_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/groups/simpeg_group.py` & `geoh5py-0.8.0a2/geoh5py/groups/simpeg_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/groups/survey_group.py` & `geoh5py-0.8.0a2/geoh5py/groups/survey_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
 
+from __future__ import annotations
+
 import uuid
 
 from .group import Group, GroupType
 
 
 class AirborneGeophysics(Group):
     """The type for the basic Container group."""
```

### Comparing `geoh5py-0.8.0a1/geoh5py/io/__init__.py` & `geoh5py-0.8.0a2/geoh5py/io/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/io/h5_reader.py` & `geoh5py-0.8.0a2/geoh5py/io/h5_reader.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/io/h5_writer.py` & `geoh5py-0.8.0a2/geoh5py/io/h5_writer.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/__init__.py` & `geoh5py-0.8.0a2/geoh5py/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/block_model.py` & `geoh5py-0.8.0a2/geoh5py/objects/block_model.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/cell_object.py` & `geoh5py-0.8.0a2/geoh5py/objects/cell_object.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/curve.py` & `geoh5py-0.8.0a2/geoh5py/objects/curve.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/drape_model.py` & `geoh5py-0.8.0a2/geoh5py/objects/drape_model.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/drillhole.py` & `geoh5py-0.8.0a2/geoh5py/objects/drillhole.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/geo_image.py` & `geoh5py-0.8.0a2/geoh5py/objects/geo_image.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
-import os
 import uuid
 import warnings
 from io import BytesIO
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Any
 
@@ -104,14 +103,101 @@
             copy_children=copy_children,
             clear_cache=clear_cache,
             **kwargs,
         )
 
         return new_entity
 
+    def copy_from_extent(  # pylint: disable=too-many-locals
+        self,
+        extent: np.ndarray,
+        parent=None,
+        copy_children: bool = True,
+        clear_cache: bool = False,
+        inverse: bool = False,
+        **kwargs,
+    ) -> GeoImage | None:
+        """
+        Sub-class extension of :func:`~geoh5py.shared.entity.Entity.copy_from_extent`.
+        """
+        if not isinstance(extent, np.ndarray):
+            raise TypeError("Expected a numpy array of extent values.")
+
+        if self.vertices is None or self.extent is None:
+            raise AttributeError("Vertices are not defined.")
+
+        if extent.shape[1] == 2:
+            extent = np.c_[extent, np.r_[-np.inf, np.inf]]
+
+        pixels = (
+            np.abs(self.extent[0, 0] - self.extent[1, 0]) / self.image.size[0],
+            np.abs(self.extent[0, 1] - self.extent[1, 1]) / self.image.size[1],
+        )
+        x_centers = np.arange(
+            self.extent[0, 0] + pixels[0] / 2,
+            self.extent[1, 0],
+            pixels[0],
+        )
+        x_ind = np.where(
+            (x_centers >= np.min(extent[:, 0])) & (x_centers <= np.max(extent[:, 0]))
+        )[0]
+        y_centers = np.arange(
+            self.extent[0, 1] + pixels[1] / 2,
+            self.extent[1, 1],
+            pixels[1],
+        )
+        y_ind = np.where(
+            (y_centers >= np.min(extent[:, 1])) & (y_centers <= np.max(extent[:, 1]))
+        )[0]
+
+        if not np.any(x_ind) or not np.any(y_ind):
+            return None
+
+        lim_x, lim_y = (x_ind[0], x_ind[-1]), (y_ind[0], y_ind[-1])
+        vertices = np.asarray(
+            [
+                [
+                    self.extent[0, 0] + lim_x[0] * pixels[0],
+                    self.extent[0, 1] + lim_y[1] * pixels[1],
+                    0,
+                ],
+                [
+                    self.extent[0, 0] + lim_x[1] * pixels[0],
+                    self.extent[0, 1] + lim_y[1] * pixels[1],
+                    0,
+                ],
+                [
+                    self.extent[0, 0] + lim_x[1] * pixels[0],
+                    self.extent[0, 1] + lim_y[0] * pixels[1],
+                    0,
+                ],
+                [
+                    self.extent[0, 0] + lim_x[0] * pixels[0],
+                    self.extent[0, 1] + lim_y[0] * pixels[1],
+                    0,
+                ],
+            ]
+        )
+        copy = super().copy(
+            parent=parent,
+            copy_children=copy_children,
+            clear_cache=clear_cache,
+            vertices=vertices,
+        )
+        copy.image = self.image.crop(
+            (
+                lim_x[0],
+                self.image.size[1] - lim_y[1],
+                lim_x[1],
+                self.image.size[1] - lim_y[0],
+            )
+        )
+
+        return copy
+
     @property
     def default_vertices(self):
         """
         Assign the default vertices based on image pixel count
         """
         if self.image is not None:
             return np.asarray(
@@ -178,15 +264,15 @@
                 )
             value = image.astype(float)
             value -= value.min()
             value *= 255.0 / value.max()
             value = value.astype("uint8")
             image = Image.fromarray(value)
         elif isinstance(image, str):
-            if not os.path.exists(image):
+            if not Path(image).is_file():
                 raise ValueError(f"Input image file {image} does not exist.")
 
             image = Image.open(image)
 
             # if the image is a tiff save tag information
             if isinstance(image, TiffImageFile):
                 self.tag = image
@@ -200,23 +286,23 @@
                 "Input 'value' for the 'image' property must be "
                 "a 2D or 3D numpy.ndarray, bytes, PIL.Image or a path to an existing image."
                 f"Get type {type(image)} instead."
             )
 
         with TemporaryDirectory() as tempdir:
             ext = getattr(image, "format")
-            temp_file = os.path.join(
-                tempdir, f"image.{ext.lower() if ext is not None else 'tiff'}"
+            temp_file = (
+                Path(tempdir) / f"image.{ext.lower() if ext is not None else 'tiff'}"
             )
             image.save(temp_file)
 
             if self.image_data is not None:
                 self.workspace.remove_entity(self.image_data)
 
-            image = self.add_file(temp_file)
+            image = self.add_file(str(temp_file))
             image.name = "GeoImageMesh_Image"
             image.entity_type.name = "GeoImageMesh_Image"
 
     def georeference(self, reference: np.ndarray | list, locations: np.ndarray | list):
         """
         Georeference the image vertices (corners) based on input reference and
         corresponding world coordinates.
@@ -440,23 +526,23 @@
             raise TypeError(
                 f"The 'name' has to be a string; a '{type(name)}' was entered instead"
             )
         if not isinstance(path, (str, Path)):
             raise TypeError(
                 f"The 'path' has to be a string or a Path; a '{type(name)}' was entered instead"
             )
-        if path != "" and not os.path.isdir(path):
+        if path != "" and not Path(path).is_dir():
             raise FileNotFoundError(f"No such file or directory: {path}")
 
         if name.endswith((".tif", ".tiff")) and self.tag is not None:
             # save the image
             image: Image = self.image_georeferenced
-            image.save(os.path.join(path, name), exif=image.getexif())
+            image.save(Path(path) / name, exif=image.getexif())
         else:
-            self.image.save(os.path.join(path, name))
+            self.image.save(Path(path) / name)
 
     def to_grid2d(
         self,
         transform: str = "GRAY",
         **grid2d_kwargs,
     ) -> objects.Grid2D:
         """
```

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/grid2d.py` & `geoh5py-0.8.0a2/geoh5py/objects/grid2d.py`

 * *Files 10% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             for ind, axis in enumerate(["x", "y", "z"]):
                 centroids[:, ind] += self.origin[axis]
 
             self._centroids = centroids
 
         return self._centroids
 
-    def copy_from_extent(
+    def copy_from_extent(  # pylint: disable=too-many-locals
         self,
         extent: np.ndarray,
         parent=None,
         copy_children: bool = True,
         clear_cache: bool = False,
         inverse: bool = False,
         **kwargs,
@@ -157,39 +157,39 @@
 
         if self.u_cell_size is None or self.v_cell_size is None:
             raise AttributeError("Cell sizes are not defined.")
 
         if extent.shape[1] == 2:
             extent = np.c_[extent, np.r_[-np.inf, np.inf]]
 
-        extent = extent.astype(float)
-        extent = np.vstack(
+        local_extent = extent.astype(float)
+        local_extent = np.vstack(
             [
-                extent[0, :],
-                np.c_[extent[0, 0], extent[1, 1], extent[0, 2]],
-                extent[1, :],
-                np.c_[extent[1, 0], extent[0, 1], extent[1, 2]],
+                local_extent[0, :],
+                np.c_[local_extent[0, 0], local_extent[1, 1], local_extent[0, 2]],
+                local_extent[1, :],
+                np.c_[local_extent[1, 0], local_extent[0, 1], local_extent[1, 2]],
             ]
         )
-        z_extent = extent[:, 2]
+        z_extent = local_extent[:, 2]
         origin = np.r_[self.origin["x"], self.origin["y"], self.origin["z"]].astype(
             float
         )
-        extent[:, :2] -= origin[:2]
+        local_extent[:, :2] -= origin[:2]
         if self.rotation != 0.0:
-            extent[:, 2] = 0
+            local_extent[:, 2] = 0
             rot = xy_rotation_matrix(-np.deg2rad(self.rotation))
-            extent = np.dot(rot, extent.T).T
-            extent[:, 2] = z_extent
+            local_extent = np.dot(rot, local_extent.T).T
+            local_extent[:, 2] = z_extent
 
-        u_ind = (self.cell_center_u <= np.max(extent[:, 0])) & (
-            self.cell_center_u >= np.min(extent[:, 0])
+        u_ind = (self.cell_center_u <= np.max(local_extent[:, 0])) & (
+            self.cell_center_u >= np.min(local_extent[:, 0])
         )
-        v_ind = (self.cell_center_v <= np.max(extent[:, 1])) & (
-            self.cell_center_v >= np.min(extent[:, 1])
+        v_ind = (self.cell_center_v <= np.max(local_extent[:, 1])) & (
+            self.cell_center_v >= np.min(local_extent[:, 1])
         )
 
         indices = np.kron(v_ind, u_ind).flatten()
 
         if not np.any(indices):
             return None
 
@@ -209,24 +209,34 @@
                         origin[2],
                     ],
                     "u_count": np.sum(u_ind),
                     "v_count": np.sum(v_ind),
                 }
             )
         else:
-            indices = ~indices
+            indices = GridObject.mask_by_extent(self, extent, inverse=inverse)
 
-        return super(GridObject, self).copy(
+        copy = super(GridObject, self).copy(
             parent=parent,
             copy_children=copy_children,
             clear_cache=clear_cache,
             mask=indices,
             **kwargs,
         )
 
+        if not inverse:
+            for child in copy.children:
+                if isinstance(child.values, np.ndarray):
+                    indices = child.mask_by_extent(extent, inverse=inverse)
+                    values = child.values
+                    values[~indices] = np.nan
+                    child.values = values
+
+        return copy
+
     @classmethod
     def default_type_uid(cls) -> uuid.UUID:
         """
         :return: Default unique identifier
         """
         return cls.__TYPE_UID
```

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/grid_object.py` & `geoh5py-0.8.0a2/geoh5py/objects/grid_object.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/integrator.py` & `geoh5py-0.8.0a2/geoh5py/objects/integrator.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
 
+from __future__ import annotations
+
 import uuid
 
 from .object_base import ObjectType
 from .points import Points
 from .surface import Surface
```

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/label.py` & `geoh5py-0.8.0a2/geoh5py/objects/label.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/notype_object.py` & `geoh5py-0.8.0a2/geoh5py/objects/notype_object.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/object_base.py` & `geoh5py-0.8.0a2/geoh5py/objects/object_base.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/object_type.py` & `geoh5py-0.8.0a2/geoh5py/objects/object_type.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/octree.py` & `geoh5py-0.8.0a2/geoh5py/objects/octree.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/points.py` & `geoh5py-0.8.0a2/geoh5py/objects/points.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/surface.py` & `geoh5py-0.8.0a2/geoh5py/objects/surface.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/surveys/__init__.py` & `geoh5py-0.8.0a2/geoh5py/objects/surveys/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/surveys/direct_current.py` & `geoh5py-0.8.0a2/geoh5py/objects/surveys/direct_current.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/__init__.py` & `geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/airborne_fem.py` & `geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/airborne_fem.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/airborne_tem.py` & `geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/airborne_tem.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/base.py` & `geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/base.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/ground_fem.py` & `geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/ground_fem.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/ground_tem.py` & `geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/ground_tem.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py` & `geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/surveys/electromagnetics/tipper.py` & `geoh5py-0.8.0a2/geoh5py/objects/surveys/electromagnetics/tipper.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/objects/surveys/magnetics.py` & `geoh5py-0.8.0a2/geoh5py/objects/surveys/magnetics.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/shared/__init__.py` & `geoh5py-0.8.0a2/geoh5py/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/shared/concatenation.py` & `geoh5py-0.8.0a2/geoh5py/shared/concatenation.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/shared/conversion/__init__.py` & `geoh5py-0.8.0a2/geoh5py/shared/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/shared/conversion/base.py` & `geoh5py-0.8.0a2/geoh5py/shared/conversion/base.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/shared/conversion/geo_image.py` & `geoh5py-0.8.0a2/geoh5py/shared/conversion/geo_image.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/shared/conversion/grid2d.py` & `geoh5py-0.8.0a2/geoh5py/shared/conversion/grid2d.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/shared/entity.py` & `geoh5py-0.8.0a2/geoh5py/shared/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
 
 # pylint: disable=R0904
 
 from __future__ import annotations
 
-import os
 import uuid
 from abc import ABC, abstractmethod
+from pathlib import Path
 from typing import TYPE_CHECKING
 
 import numpy as np
 
 from geoh5py.shared.utils import str2uuid
 
 if TYPE_CHECKING:
@@ -88,21 +88,21 @@
 
     def add_file(self, file: str):
         """
         Add a file to the object or group stored as bytes on a FilenameData
 
         :param file: File name with path to import.
         """
-        if not os.path.exists(file):
+        if not Path(file).is_file():
             raise ValueError(f"Input file '{file}' does not exist.")
 
         with open(file, "rb") as raw_binary:
             blob = raw_binary.read()
 
-        _, name = os.path.split(file)
+        name = Path(file).name
         attributes = {
             "name": name,
             "file_name": name,
             "association": "OBJECT",
             "parent": self,
             "values": blob,
         }
```

### Comparing `geoh5py-0.8.0a1/geoh5py/shared/entity_type.py` & `geoh5py-0.8.0a2/geoh5py/shared/entity_type.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/shared/exceptions.py` & `geoh5py-0.8.0a2/geoh5py/shared/exceptions.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/shared/utils.py` & `geoh5py-0.8.0a2/geoh5py/shared/utils.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/shared/validators.py` & `geoh5py-0.8.0a2/geoh5py/shared/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
             )
             return
 
         if not isinstance(valid, (Entity, Workspace)):
             raise ValueError(
                 "'AssociationValidator.validate' requires a 'valid'"
                 " input of type 'Entity', 'Workspace' or None. "
-                f"Provided '{valid}' or type {type(valid)} for parameter '{name}'"
+                f"Provided '{valid}' of type {type(valid)} for parameter '{name}'"
             )
 
         if isinstance(value, UUID):
             uid = value
         elif isinstance(value, (Entity, PropertyGroup)):
             uid = value.uid
         else:
```

### Comparing `geoh5py-0.8.0a1/geoh5py/shared/weakref_utils.py` & `geoh5py-0.8.0a2/geoh5py/shared/weakref_utils.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/ui_json/__init__.py` & `geoh5py-0.8.0a2/geoh5py/ui_json/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/ui_json/constants.py` & `geoh5py-0.8.0a2/geoh5py/ui_json/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
 
 
 from __future__ import annotations
 
+from pathlib import Path
 from uuid import UUID
 
 from ..groups import PropertyGroup
 from ..shared import Entity
 from ..workspace import Workspace
 
 default_ui_json = {
@@ -70,21 +71,21 @@
     "title": {"required": True, "types": [str]},
     "conda_environment": {
         "types": [str, type(None)],
     },
     "conda_environment_boolean": {
         "types": [bool],
     },
-    "geoh5": {"required": True, "types": [str, Workspace, type(None)]},
+    "geoh5": {"required": True, "types": [str, Path, Workspace, type(None)]},
     "monitoring_directory": {
-        "types": [str, type(None)],
+        "types": [str, Path, type(None)],
     },
     "run_command": {
         "types": [str, type(None)],
     },
     "run_command_boolean": {
         "types": [bool],
     },
     "workspace": {
-        "types": [str, Workspace, type(None)],
+        "types": [str, Path, Workspace, type(None)],
     },
 }
```

### Comparing `geoh5py-0.8.0a1/geoh5py/ui_json/input_file.py` & `geoh5py-0.8.0a2/geoh5py/ui_json/input_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 #
 #  geoapps is distributed under the terms and conditions of the MIT License
 #  (see LICENSE file at the root of this source code package).
 
 from __future__ import annotations
 
 import json
-import os
 import warnings
 from copy import deepcopy
 from pathlib import Path
 from typing import Any
 from uuid import UUID
 
 from geoh5py import Workspace
@@ -92,22 +91,22 @@
         self.validation_options = validation_options
         self.validate = validate
         self.validations = validations
         self.ui_json = ui_json
         self.data = data
 
     @property
-    def data(self):
-        if getattr(self, "_data", None) is None and self.ui_json is not None:
+    def data(self) -> dict[str, Any] | None:
+        if self._data is None and self.ui_json is not None:
             self.data = flatten(self.ui_json)
 
         return self._data
 
     @data.setter
-    def data(self, value: dict[str, Any]):
+    def data(self, value: dict[str, Any] | None):
         if value is not None:
             if not isinstance(value, dict):
                 raise ValueError("Input 'data' must be of type dict or None.")
 
             if self._ui_json is None:
                 raise AttributeError("'ui_json' must be set before setting data.")
 
@@ -149,48 +148,46 @@
 
     @property
     def path(self) -> str | None:
         """
         Directory for the input/output ui.json file.
         """
         if getattr(self, "_path", None) is None and self.geoh5 is not None:
-            self.path = os.path.dirname(self.geoh5.h5file)
+            self.path = str(Path(self.geoh5.h5file).parent)
 
         return self._path
 
     @path.setter
     def path(self, path: str):
-        if not os.path.isdir(path):
-            raise ValueError(f"The specified path: '{path}' does not exist.")
+        dir_path = Path(path).resolve(strict=True)
+        if not dir_path.is_dir():
+            raise ValueError(f"The specified path is not a directory: {path}")
 
-        self._path = path
+        self._path = str(dir_path)
 
     @property
     def path_name(self) -> str | None:
         if self.path is not None and self.name is not None:
-            return os.path.join(self.path, self.name)
+            return str(Path(self.path) / self.name)
 
         return None
 
     @staticmethod
     def read_ui_json(json_file: str | Path, **kwargs):
         """
         Read and create an InputFile from ui.json
         """
-        if isinstance(json_file, Path):
-            json_file = str(json_file)
 
-        if not isinstance(json_file, str) or not json_file.endswith(".ui.json"):
-            raise ValueError(
-                "Input file should be a str or Path with extension *.ui.json"
-            )
+        json_file_path = Path(json_file).resolve()
+        if "".join(json_file_path.suffixes[-2:]) != ".ui.json":
+            raise ValueError("Input file should have the extension .ui.json")
 
         input_file = InputFile(**kwargs)
-        input_file.path = os.path.dirname(os.path.abspath(json_file))
-        input_file.name = os.path.basename(json_file)
+        input_file.path = str(json_file_path.parent)
+        input_file.name = json_file_path.name
 
         with open(json_file, encoding="utf-8") as file:
             input_file.ui_json = json.load(file)
 
         if isinstance(input_file.geoh5, Workspace):
             input_file.geoh5.close()
 
@@ -358,30 +355,29 @@
         """Geoh5 workspace."""
         if self._geoh5 is None and self.data is not None:
             self._geoh5 = self.data["geoh5"]
         return self._geoh5
 
     @geoh5.setter
     def geoh5(self, geoh5: Workspace | None):
-        if geoh5 is not None:
-            if self._geoh5 is not None:
-                raise UserWarning(
-                    "Attribute 'geoh5' already set. "
-                    "Consider creating a new InputFile from arguments."
-                )
-
-            if not isinstance(geoh5, Workspace):
-                raise ValueError(
-                    "Input 'geoh5' must be a valid :obj:`geoh5py.workspace.Workspace`."
-                )
+        if geoh5 is None:
+            return
 
+        if self._geoh5 is not None:
+            raise UserWarning(
+                "Attribute 'geoh5' already set. "
+                "Consider creating a new InputFile from arguments."
+            )
+        if not isinstance(geoh5, Workspace):
+            raise ValueError(
+                "Input 'geoh5' must be a valid :obj:`geoh5py.workspace.Workspace`."
+            )
         self._geoh5 = geoh5
-
         if self.validators is not None:
-            self.validators.geoh5 = geoh5
+            self.validators.geoh5 = self.geoh5
 
     def write_ui_json(
         self,
         name: str | None = None,
         path: str | Path | None = None,
     ):
         """
@@ -391,15 +387,15 @@
         :param path: Directory to write the ui.json to.
         """
 
         if name is not None:
             self.name = name
 
         if path is not None:
-            self.path = os.path.abspath(path)
+            self.path = str(path)
 
         if self.path_name is None:
             raise AttributeError(
                 "The input file requires 'path' and 'name' to be set before writing out."
             )
 
         if self.ui_json is None:
@@ -418,14 +414,15 @@
     def set_data_value(self, key: str, value):
         """
         Set the data and json form values from a dictionary.
 
         :param key: Parameter name to update.
         :param value: Value to update with.
         """
+        assert self.data is not None
         if self.validate and self.validations is not None and key in self.validations:
             if "association" in self.validations[key]:
                 validations = deepcopy(self.validations[key])
                 parent = self.data[self.validations[key]["association"]]
                 if isinstance(parent, UUID):
                     parent = self.geoh5.get_entity(parent)[0]
                 validations["association"] = parent
@@ -495,16 +492,20 @@
 
             mappers = [str2none, str2inf, str2uuid, path2workspace]
             ui_json[key] = dict_mapper(value, mappers)
 
         return ui_json
 
     @classmethod
-    def demote(cls, var: dict[str, Any]) -> dict[str, str]:
-        """Converts promoted parameter values to their string representations."""
+    def demote(cls, var: dict[str, Any]) -> dict[str, Any]:
+        """
+        Converts promoted parameter values to their string representations.
+
+        Other parameters are left unchanged.
+        """
         mappers = [entity2uuid, as_str_if_uuid, workspace2path, container_group2name]
         for key, value in var.items():
             if isinstance(value, dict):
                 var[key] = cls.demote(value)
 
             elif isinstance(value, (list, tuple)):
                 var[key] = [dict_mapper(val, mappers) for val in value]
```

### Comparing `geoh5py-0.8.0a1/geoh5py/ui_json/templates.py` & `geoh5py-0.8.0a2/geoh5py/ui_json/templates.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/ui_json/utils.py` & `geoh5py-0.8.0a2/geoh5py/ui_json/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,27 @@
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
+import shutil
 import warnings
-from os import mkdir, path
-from shutil import move
+from io import BytesIO
+from pathlib import Path
 from time import time
 from typing import Any
 
 import numpy as np
 
 from geoh5py import Workspace
 from geoh5py.groups import ContainerGroup
 from geoh5py.objects import ObjectBase
+from geoh5py.shared.utils import fetch_active_workspace
 
 
 def flatten(ui_json: dict[str, dict]) -> dict[str, Any]:
     """Flattens ui.json format to simple key/value pair."""
     data: dict[str, Any] = {}
     for name, value in ui_json.items():
         if isinstance(value, dict):
@@ -293,15 +295,17 @@
     if value in ["inf", "-inf"]:
         return float(value)
     return value
 
 
 def workspace2path(value):
     if isinstance(value, Workspace):
-        return value.h5file
+        if isinstance(value.h5file, BytesIO):
+            return "[in-memory]"
+        return str(value.h5file)
     return value
 
 
 def path2workspace(value):
     if isinstance(value, str) and ".geoh5" in value:
         workspace = Workspace(value, mode="r")
         workspace.close()
@@ -313,34 +317,31 @@
     if isinstance(value, ContainerGroup):
         return value.name
     return value
 
 
 def monitored_directory_copy(
     directory: str, entity: ObjectBase, copy_children: bool = True
-):
+) -> str:
     """
     Create a temporary geoh5 file in the monitoring folder and export entity for update.
 
     :param directory: Monitoring directory
     :param entity: Entity to be updated
     :param copy_children: Option to copy children entities.
     """
-    working_path = path.join(directory, ".working")
-
-    if not path.exists(working_path):
-        mkdir(working_path)
+    directory_path = Path(directory)
+    working_path = directory_path / ".working"
+    working_path.mkdir(exist_ok=True)
 
     temp_geoh5 = f"temp{time():.3f}.geoh5"
 
-    if getattr(entity.workspace, "_geoh5") is None:
-        entity.workspace.open(mode="r")
-
-    with Workspace(path.join(working_path, temp_geoh5)) as w_s:
-        entity.copy(parent=w_s, copy_children=copy_children)
-
-    move(
-        path.join(working_path, temp_geoh5),
-        path.join(directory, temp_geoh5),
+    with fetch_active_workspace(entity.workspace, mode="r"):
+        with Workspace(working_path / temp_geoh5) as w_s:
+            entity.copy(parent=w_s, copy_children=copy_children)
+
+    shutil.move(
+        working_path / temp_geoh5,
+        directory_path / temp_geoh5,
     )
 
-    return path.join(directory, temp_geoh5)
+    return str(directory_path / temp_geoh5)
```

### Comparing `geoh5py-0.8.0a1/geoh5py/ui_json/validation.py` & `geoh5py-0.8.0a2/geoh5py/ui_json/validation.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/workspace/__init__.py` & `geoh5py-0.8.0a2/geoh5py/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/geoh5py/workspace/workspace.py` & `geoh5py-0.8.0a2/geoh5py/workspace/workspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 # pylint: disable=too-many-lines, too-many-public-methods, too-many-arguments, too-many-locals
 
 from __future__ import annotations
 
 import inspect
 import io
-import os
 import shutil
 import subprocess
 import tempfile
 import uuid
 import warnings
 import weakref
 from contextlib import AbstractContextManager, contextmanager
@@ -185,25 +184,23 @@
                     self.update_attribute(entity, "concatenated_attributes")
 
             self._io_call(H5Writer.save_entity, self.root, add_children=True, mode="r+")
 
         self.geoh5.close()
         self._data = {}
         if self.repack and not isinstance(self.h5file, io.BytesIO):
-            temp_file = os.path.join(
-                tempfile.gettempdir(), os.path.basename(self.h5file)
-            )
+            temp_file = Path(tempfile.gettempdir()) / Path(self.h5file).name
             try:
                 subprocess.run(
                     f'h5repack --native "{self.h5file}" "{temp_file}"',
                     check=True,
                     shell=True,
                     stdout=subprocess.DEVNULL,
                 )
-                os.remove(self.h5file)
+                Path(self.h5file).unlink()
                 shutil.move(temp_file, self.h5file)
             except CalledProcessError:
                 pass
 
             self.repack = False
 
     @property
@@ -935,15 +932,15 @@
         :str: Target *geoh5* file name with path.
         """
         return self._h5file
 
     @h5file.setter
     def h5file(self, file: str | Path | io.BytesIO):
         if isinstance(file, (str, Path)):
-            if not str(file).endswith("geoh5"):
+            if Path(file).suffix != ".geoh5":
                 raise ValueError("Input 'h5file' file must have a 'geoh5' extension.")
         elif not isinstance(file, io.BytesIO):
             raise ValueError(
                 "The 'h5file' attribute must be a str, "
                 "pathlib.Path or bytes to the target geoh5 file. "
                 f"Provided {file} of type({type(file)})"
             )
```

### Comparing `geoh5py-0.8.0a1/package.rst` & `geoh5py-0.8.0a2/package.rst`

 * *Files identical despite different names*

### Comparing `geoh5py-0.8.0a1/pyproject.toml` & `geoh5py-0.8.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geoh5py"
-version = "0.8.0-alpha.1"
+version = "0.8.0-alpha.2"
 license = "LGPL-3.0-or-later"
 description = "Python API for geoh5, an open file format for geoscientific data"
 authors = ["Mira Geoscience <support@mirageoscience.com>"]
 repository = "https://github.com/MiraGeoscience/geoh5py"
 documentation = "https://geoh5py.readthedocs.io/en/latest/"
 homepage = "https://mirageoscience.com"
 readme = "package.rst"
@@ -35,15 +35,15 @@
 pylint = "*"
 pytest = "*"
 pytest-cov = "*"
 scipy = "^1.4.1"
 sphinx = "^3.0"
 sphinx-autodoc-typehints = "^1.10"
 sphinx-rtd-theme = "^0.4.3"
-toml = "*"
+tomli = "*"
 
 [tool.poetry.extras]
 
 [tool.poetry.scripts]
 publish = 'devtools.publish:publish'
 
 [tool.dephell.main]
```

### Comparing `geoh5py-0.8.0a1/PKG-INFO` & `geoh5py-0.8.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoh5py
-Version: 0.8.0a1
+Version: 0.8.0a2
 Summary: Python API for geoh5, an open file format for geoscientific data
 Home-page: https://mirageoscience.com
 License: LGPL-3.0-or-later
 Keywords: geology,geophysics,data,interoperability
 Author: Mira Geoscience
 Author-email: support@mirageoscience.com
 Requires-Python: >=3.8,<3.11
```

