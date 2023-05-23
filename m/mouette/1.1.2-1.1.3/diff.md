# Comparing `tmp/mouette-1.1.2.tar.gz` & `tmp/mouette-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mouette-1.1.2.tar", last modified: Mon Apr  3 13:04:11 2023, max compression
+gzip compressed data, was "mouette-1.1.3.tar", last modified: Tue May 23 09:12:52 2023, max compression
```

## Comparing `mouette-1.1.2.tar` & `mouette-1.1.3.tar`

### file list

```diff
@@ -1,202 +1,202 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.567036 mouette-1.1.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.551036 mouette-1.1.2/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.551036 mouette-1.1.2/.github/workflows/
--rw-rw-r--   0 root         (0) root         (0)      343 2022-09-01 08:22:07.000000 mouette-1.1.2/.github/workflows/docs.yml
--rw-rw-r--   0 root         (0) root         (0)     1091 2022-08-23 12:53:25.000000 mouette-1.1.2/.github/workflows/python-publish.yml
--rw-rw-r--   0 root         (0) root         (0)     1843 2022-08-21 17:58:18.000000 mouette-1.1.2/.gitignore
--rw-rw-r--   0 root         (0) root         (0)     1075 2022-08-21 17:58:18.000000 mouette-1.1.2/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      134 2023-04-03 08:10:35.000000 mouette-1.1.2/Makefile
--rw-r--r--   0 root         (0) root         (0)     1956 2023-04-03 13:04:11.567036 mouette-1.1.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1698 2023-02-05 20:34:49.000000 mouette-1.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.551036 mouette-1.1.2/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.551036 mouette-1.1.2/docs/Algorithms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.551036 mouette-1.1.2/docs/Algorithms/Frame Fields/
--rw-rw-r--   0 root         (0) root         (0)     1722 2023-02-06 14:19:10.000000 mouette-1.1.2/docs/Algorithms/Frame Fields/00_framefields.md
--rw-rw-r--   0 root         (0) root         (0)      102 2023-02-06 13:49:38.000000 mouette-1.1.2/docs/Algorithms/Frame Fields/01_2dFF.md
--rw-rw-r--   0 root         (0) root         (0)      164 2023-02-06 14:08:01.000000 mouette-1.1.2/docs/Algorithms/Frame Fields/02_Curvature.md
--rw-rw-r--   0 root         (0) root         (0)     1213 2023-02-06 14:42:19.000000 mouette-1.1.2/docs/Algorithms/Frame Fields/03_3dFF.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.555036 mouette-1.1.2/docs/Algorithms/Parametrization/
--rw-rw-r--   0 root         (0) root         (0)       88 2023-04-03 08:35:48.000000 mouette-1.1.2/docs/Algorithms/Parametrization/00_distortion.md
--rw-rw-r--   0 root         (0) root         (0)      305 2023-02-06 15:04:20.000000 mouette-1.1.2/docs/Algorithms/Parametrization/Tutte.md
--rw-rw-r--   0 root         (0) root         (0)      387 2023-02-06 15:12:47.000000 mouette-1.1.2/docs/Algorithms/Parametrization/cotan_embedding.md
--rw-rw-r--   0 root         (0) root         (0)      355 2023-02-06 14:58:37.000000 mouette-1.1.2/docs/Algorithms/Parametrization/lscm.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.555036 mouette-1.1.2/docs/Algorithms/Trees/
--rw-rw-r--   0 root         (0) root         (0)        4 2022-08-30 12:42:01.000000 mouette-1.1.2/docs/Algorithms/Trees/tree.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.555036 mouette-1.1.2/docs/Attributes/
--rw-rw-r--   0 root         (0) root         (0)       62 2022-09-26 16:03:21.000000 mouette-1.1.2/docs/Attributes/01_global.md
--rw-rw-r--   0 root         (0) root         (0)       65 2022-09-26 16:03:26.000000 mouette-1.1.2/docs/Attributes/02_vertices.md
--rw-rw-r--   0 root         (0) root         (0)       59 2022-09-26 16:03:34.000000 mouette-1.1.2/docs/Attributes/03_edges.md
--rw-rw-r--   0 root         (0) root         (0)       59 2022-09-26 16:01:39.000000 mouette-1.1.2/docs/Attributes/04_faces.md
--rw-rw-r--   0 root         (0) root         (0)       68 2022-09-26 16:01:35.000000 mouette-1.1.2/docs/Attributes/05_corners.md
--rw-rw-r--   0 root         (0) root         (0)       59 2022-09-26 16:01:32.000000 mouette-1.1.2/docs/Attributes/06_cells.md
--rw-rw-r--   0 root         (0) root         (0)       75 2022-09-26 16:03:32.000000 mouette-1.1.2/docs/Attributes/07_interpolation.md
--rw-rw-r--   0 root         (0) root         (0)      424 2023-04-03 08:29:29.000000 mouette-1.1.2/docs/Dependencies.md
--rw-rw-r--   0 root         (0) root         (0)      176 2022-08-21 17:58:18.000000 mouette-1.1.2/docs/Design Philosophy.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.555036 mouette-1.1.2/docs/Geometry/
--rw-rw-r--   0 root         (0) root         (0)      654 2023-02-06 14:42:17.000000 mouette-1.1.2/docs/Geometry/spherical_harmonics.md
--rw-rw-r--   0 root         (0) root         (0)       36 2022-08-21 17:58:18.000000 mouette-1.1.2/docs/Loading and Saving.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.555036 mouette-1.1.2/docs/Meshes and Datastructures/
--rw-rw-r--   0 root         (0) root         (0)       73 2023-04-03 08:55:54.000000 mouette-1.1.2/docs/Meshes and Datastructures/00_RawMeshData.md
--rw-rw-r--   0 root         (0) root         (0)      294 2023-04-03 09:30:16.000000 mouette-1.1.2/docs/Meshes and Datastructures/01_PointClouds.md
--rw-rw-r--   0 root         (0) root         (0)      445 2023-04-03 09:30:18.000000 mouette-1.1.2/docs/Meshes and Datastructures/02_PolyLines.md
--rw-rw-r--   0 root         (0) root         (0)      422 2023-04-03 10:41:25.000000 mouette-1.1.2/docs/Meshes and Datastructures/03_SurfaceMeshes.md
--rw-rw-r--   0 root         (0) root         (0)       64 2023-04-03 08:34:41.000000 mouette-1.1.2/docs/Meshes and Datastructures/04_VolumeMeshes.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.555036 mouette-1.1.2/docs/Utilities/
--rw-rw-r--   0 root         (0) root         (0)       64 2023-02-07 13:44:55.000000 mouette-1.1.2/docs/Utilities/priority_queue.md
--rw-rw-r--   0 root         (0) root         (0)       55 2023-02-07 14:12:00.000000 mouette-1.1.2/docs/Utilities/union_find.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.555036 mouette-1.1.2/docs/_img/
--rw-rw-r--   0 root         (0) root         (0)   269170 2023-04-03 10:40:50.000000 mouette-1.1.2/docs/_img/bunny_tri.jpeg
--rw-rw-r--   0 root         (0) root         (0)   155178 2023-04-03 09:26:50.000000 mouette-1.1.2/docs/_img/duck_polyline.jpeg
--rw-rw-r--   0 root         (0) root         (0)   166130 2023-04-03 09:07:13.000000 mouette-1.1.2/docs/_img/point_cloud_cad_example.jpeg
--rw-rw-r--   0 root         (0) root         (0)     1585 2022-09-05 13:21:43.000000 mouette-1.1.2/docs/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.559036 mouette-1.1.2/examples/
--rw-rw-r--   0 root         (0) root         (0)     2120 2023-02-07 13:59:53.000000 mouette-1.1.2/examples/framefield2D.py
--rw-rw-r--   0 root         (0) root         (0)      421 2022-09-26 15:25:06.000000 mouette-1.1.2/examples/framefield3D.py
--rw-rw-r--   0 root         (0) root         (0)      391 2022-09-26 15:23:43.000000 mouette-1.1.2/examples/lscm.py
--rw-rw-r--   0 root         (0) root         (0)      792 2023-04-03 09:19:59.000000 mouette-1.1.2/mkdocs.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.559036 mouette-1.1.2/mouette/
--rw-rw-r--   0 root         (0) root         (0)      590 2023-03-28 12:25:47.000000 mouette-1.1.2/mouette/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.559036 mouette-1.1.2/mouette/attributes/
--rw-rw-r--   0 root         (0) root         (0)      181 2022-08-21 17:58:18.000000 mouette-1.1.2/mouette/attributes/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3469 2022-09-26 16:06:27.000000 mouette-1.1.2/mouette/attributes/glob.py
--rw-rw-r--   0 root         (0) root         (0)     4296 2022-12-23 14:05:48.000000 mouette-1.1.2/mouette/attributes/interpolate.py
--rw-rw-r--   0 root         (0) root         (0)     3142 2022-09-26 16:21:57.000000 mouette-1.1.2/mouette/attributes/misc_cells.py
--rw-rw-r--   0 root         (0) root         (0)     3081 2022-10-05 08:17:26.000000 mouette-1.1.2/mouette/attributes/misc_corners.py
--rw-rw-r--   0 root         (0) root         (0)     3627 2022-11-17 16:57:39.000000 mouette-1.1.2/mouette/attributes/misc_edges.py
--rw-rw-r--   0 root         (0) root         (0)     8500 2023-02-04 13:53:10.000000 mouette-1.1.2/mouette/attributes/misc_faces.py
--rw-rw-r--   0 root         (0) root         (0)     6836 2023-02-04 13:52:44.000000 mouette-1.1.2/mouette/attributes/misc_vertices.py
--rw-rw-r--   0 root         (0) root         (0)     1172 2022-09-01 08:24:31.000000 mouette-1.1.2/mouette/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.559036 mouette-1.1.2/mouette/geometry/
--rw-rw-r--   0 root         (0) root         (0)    15644 2023-04-03 08:58:44.000000 mouette-1.1.2/mouette/geometry/SphericalHarmonics.py
--rw-rw-r--   0 root         (0) root         (0)      105 2022-08-21 17:58:18.000000 mouette-1.1.2/mouette/geometry/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6085 2022-11-26 16:01:37.000000 mouette-1.1.2/mouette/geometry/geometry.py
--rw-rw-r--   0 root         (0) root         (0)     2408 2022-09-26 15:52:39.000000 mouette-1.1.2/mouette/geometry/rotations.py
--rw-rw-r--   0 root         (0) root         (0)     3876 2022-09-26 15:52:39.000000 mouette-1.1.2/mouette/geometry/transform.py
--rw-rw-r--   0 root         (0) root         (0)     1738 2022-10-03 15:16:09.000000 mouette-1.1.2/mouette/geometry/vector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.559036 mouette-1.1.2/mouette/mesh/
--rw-rw-r--   0 root         (0) root         (0)      201 2022-08-21 17:58:18.000000 mouette-1.1.2/mouette/mesh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.559036 mouette-1.1.2/mouette/mesh/datatypes/
--rw-rw-r--   0 root         (0) root         (0)      216 2022-08-21 17:58:18.000000 mouette-1.1.2/mouette/mesh/datatypes/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      574 2022-08-21 18:04:49.000000 mouette-1.1.2/mouette/mesh/datatypes/base.py
--rw-rw-r--   0 root         (0) root         (0)     5250 2023-04-03 11:04:41.000000 mouette-1.1.2/mouette/mesh/datatypes/linear.py
--rw-rw-r--   0 root         (0) root         (0)      904 2023-04-03 09:18:41.000000 mouette-1.1.2/mouette/mesh/datatypes/pointcloud.py
--rw-rw-r--   0 root         (0) root         (0)    20178 2023-04-03 11:10:23.000000 mouette-1.1.2/mouette/mesh/datatypes/surface.py
--rw-rw-r--   0 root         (0) root         (0)     1767 2023-02-06 08:16:44.000000 mouette-1.1.2/mouette/mesh/datatypes/type_checks.py
--rw-rw-r--   0 root         (0) root         (0)    20556 2023-01-13 14:12:51.000000 mouette-1.1.2/mouette/mesh/datatypes/volume.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.559036 mouette-1.1.2/mouette/mesh/io/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-21 17:58:18.000000 mouette-1.1.2/mouette/mesh/io/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    14527 2022-08-21 22:39:01.000000 mouette-1.1.2/mouette/mesh/io/geogram_ascii.py
--rw-rw-r--   0 root         (0) root         (0)     1218 2022-08-21 17:58:18.000000 mouette-1.1.2/mouette/mesh/io/io.py
--rw-rw-r--   0 root         (0) root         (0)     4999 2022-08-21 17:58:18.000000 mouette-1.1.2/mouette/mesh/io/medit.py
--rw-rw-r--   0 root         (0) root         (0)     4237 2023-03-07 15:31:45.000000 mouette-1.1.2/mouette/mesh/io/obj.py
--rw-rw-r--   0 root         (0) root         (0)     2191 2022-09-26 15:52:39.000000 mouette-1.1.2/mouette/mesh/io/off.py
--rw-rw-r--   0 root         (0) root         (0)     1494 2022-09-26 15:52:39.000000 mouette-1.1.2/mouette/mesh/io/tet.py
--rw-rw-r--   0 root         (0) root         (0)      870 2022-09-26 15:52:39.000000 mouette-1.1.2/mouette/mesh/io/xyz.py
--rw-rw-r--   0 root         (0) root         (0)     5596 2022-09-26 15:52:39.000000 mouette-1.1.2/mouette/mesh/mesh.py
--rw-rw-r--   0 root         (0) root         (0)    12499 2023-03-07 15:31:43.000000 mouette-1.1.2/mouette/mesh/mesh_attributes.py
--rw-rw-r--   0 root         (0) root         (0)    10057 2023-02-10 12:43:27.000000 mouette-1.1.2/mouette/mesh/mesh_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.559036 mouette-1.1.2/mouette/operators/
--rw-rw-r--   0 root         (0) root         (0)       49 2022-08-21 17:58:18.000000 mouette-1.1.2/mouette/operators/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2247 2022-09-26 15:52:39.000000 mouette-1.1.2/mouette/operators/adjacency.py
--rw-rw-r--   0 root         (0) root         (0)     9252 2023-02-06 13:27:42.000000 mouette-1.1.2/mouette/operators/laplacian.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.559036 mouette-1.1.2/mouette/optimize/
--rw-rw-r--   0 root         (0) root         (0)       77 2023-02-28 17:07:06.000000 mouette-1.1.2/mouette/optimize/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1291 2022-10-03 12:39:49.000000 mouette-1.1.2/mouette/optimize/eigensolve.py
--rw-rw-r--   0 root         (0) root         (0)    12794 2023-03-31 14:53:04.000000 mouette-1.1.2/mouette/optimize/levenberg_marquardt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.559036 mouette-1.1.2/mouette/procedural/
--rw-rw-r--   0 root         (0) root         (0)      278 2022-08-21 17:58:18.000000 mouette-1.1.2/mouette/procedural/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1791 2022-09-26 15:52:39.000000 mouette-1.1.2/mouette/procedural/cylinder.py
--rw-rw-r--   0 root         (0) root         (0)     1567 2022-09-26 15:52:39.000000 mouette-1.1.2/mouette/procedural/hexahedra.py
--rw-rw-r--   0 root         (0) root         (0)     3109 2022-09-26 15:52:39.000000 mouette-1.1.2/mouette/procedural/platonic.py
--rw-rw-r--   0 root         (0) root         (0)     2787 2022-12-23 16:00:47.000000 mouette-1.1.2/mouette/procedural/rings.py
--rw-rw-r--   0 root         (0) root         (0)     3690 2022-09-26 15:52:39.000000 mouette-1.1.2/mouette/procedural/sphere.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.559036 mouette-1.1.2/mouette/processing/
--rw-rw-r--   0 root         (0) root         (0)      559 2023-03-28 12:25:34.000000 mouette-1.1.2/mouette/processing/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3919 2022-09-26 15:52:39.000000 mouette-1.1.2/mouette/processing/border.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.563037 mouette-1.1.2/mouette/processing/combinatorics/
--rw-rw-r--   0 root         (0) root         (0)       63 2022-08-21 17:58:18.000000 mouette-1.1.2/mouette/processing/combinatorics/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    17363 2023-04-01 09:08:53.000000 mouette-1.1.2/mouette/processing/combinatorics/cutting.py
--rw-rw-r--   0 root         (0) root         (0)     8183 2023-04-03 08:02:11.000000 mouette-1.1.2/mouette/processing/combinatorics/subdivide.py
--rw-rw-r--   0 root         (0) root         (0)     7776 2023-03-31 11:49:03.000000 mouette-1.1.2/mouette/processing/connection.py
--rw-rw-r--   0 root         (0) root         (0)     9206 2023-01-10 09:34:21.000000 mouette-1.1.2/mouette/processing/features.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.563037 mouette-1.1.2/mouette/processing/framefield/
--rw-rw-r--   0 root         (0) root         (0)       92 2023-03-28 12:25:46.000000 mouette-1.1.2/mouette/processing/framefield/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1348 2023-02-06 16:09:04.000000 mouette-1.1.2/mouette/processing/framefield/base.py
--rw-rw-r--   0 root         (0) root         (0)    13554 2023-02-06 13:24:01.000000 mouette-1.1.2/mouette/processing/framefield/cells.py
--rw-rw-r--   0 root         (0) root         (0)     3871 2023-02-06 08:04:19.000000 mouette-1.1.2/mouette/processing/framefield/curvature_faces.py
--rw-rw-r--   0 root         (0) root         (0)     8467 2023-02-06 08:16:41.000000 mouette-1.1.2/mouette/processing/framefield/curvature_vertex.py
--rw-rw-r--   0 root         (0) root         (0)    14527 2023-03-31 14:24:31.000000 mouette-1.1.2/mouette/processing/framefield/faces2d.py
--rw-rw-r--   0 root         (0) root         (0)    10844 2023-03-31 14:22:05.000000 mouette-1.1.2/mouette/processing/framefield/framefield.py
--rw-rw-r--   0 root         (0) root         (0)    18227 2023-03-30 12:48:19.000000 mouette-1.1.2/mouette/processing/framefield/vertex2d.py
--rw-rw-r--   0 root         (0) root         (0)    12249 2023-02-06 13:26:49.000000 mouette-1.1.2/mouette/processing/framefield/vertex3d.py
--rw-rw-r--   0 root         (0) root         (0)     2933 2023-03-30 13:16:33.000000 mouette-1.1.2/mouette/processing/misc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.563037 mouette-1.1.2/mouette/processing/parametrization/
--rw-rw-r--   0 root         (0) root         (0)      147 2022-12-04 21:19:32.000000 mouette-1.1.2/mouette/processing/parametrization/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1534 2023-04-01 10:34:36.000000 mouette-1.1.2/mouette/processing/parametrization/base.py
--rw-rw-r--   0 root         (0) root         (0)    10003 2023-04-01 10:37:07.000000 mouette-1.1.2/mouette/processing/parametrization/cotan_emb.py
--rw-rw-r--   0 root         (0) root         (0)    12940 2023-04-01 09:46:25.000000 mouette-1.1.2/mouette/processing/parametrization/distortion.py
--rw-rw-r--   0 root         (0) root         (0)     5991 2023-04-01 10:31:45.000000 mouette-1.1.2/mouette/processing/parametrization/lscm.py
--rw-rw-r--   0 root         (0) root         (0)     4555 2023-04-01 10:31:43.000000 mouette-1.1.2/mouette/processing/parametrization/tutte.py
--rw-rw-r--   0 root         (0) root         (0)     8822 2023-03-06 08:49:04.000000 mouette-1.1.2/mouette/processing/paths.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.563037 mouette-1.1.2/mouette/processing/trees/
--rw-rw-r--   0 root         (0) root         (0)      198 2022-08-21 17:58:18.000000 mouette-1.1.2/mouette/processing/trees/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3225 2022-09-26 15:52:39.000000 mouette-1.1.2/mouette/processing/trees/base.py
--rw-rw-r--   0 root         (0) root         (0)     3223 2022-08-21 17:58:18.000000 mouette-1.1.2/mouette/processing/trees/cell_sp.py
--rw-rw-r--   0 root         (0) root         (0)     8242 2022-09-26 15:52:39.000000 mouette-1.1.2/mouette/processing/trees/edge_sp.py
--rw-rw-r--   0 root         (0) root         (0)     3399 2023-03-06 08:03:29.000000 mouette-1.1.2/mouette/processing/trees/face_sp.py
--rw-rw-r--   0 root         (0) root         (0)      451 2022-08-21 18:01:16.000000 mouette-1.1.2/mouette/processing/worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.563037 mouette-1.1.2/mouette/utils/
--rw-rw-r--   0 root         (0) root         (0)      174 2023-02-03 15:31:47.000000 mouette-1.1.2/mouette/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2159 2023-02-03 16:51:10.000000 mouette-1.1.2/mouette/utils/argument_check.py
--rw-rw-r--   0 root         (0) root         (0)     1744 2022-10-06 15:31:15.000000 mouette-1.1.2/mouette/utils/iterators.py
--rw-rw-r--   0 root         (0) root         (0)     1476 2023-03-28 11:32:27.000000 mouette-1.1.2/mouette/utils/maths.py
--rw-rw-r--   0 root         (0) root         (0)     2031 2023-04-03 12:41:10.000000 mouette-1.1.2/mouette/utils/priority_queue.py
--rw-rw-r--   0 root         (0) root         (0)     8788 2023-04-03 13:03:23.000000 mouette-1.1.2/mouette/utils/unionfind.py
--rw-rw-r--   0 root         (0) root         (0)     1106 2023-04-03 12:05:05.000000 mouette-1.1.2/mouette/utils/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.559036 mouette-1.1.2/mouette.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1956 2023-04-03 13:04:11.000000 mouette-1.1.2/mouette.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5117 2023-04-03 13:04:11.000000 mouette-1.1.2/mouette.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-03 13:04:11.000000 mouette-1.1.2/mouette.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-03 13:04:11.000000 mouette-1.1.2/mouette.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-03 13:04:11.000000 mouette-1.1.2/mouette.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      756 2022-11-26 20:56:26.000000 mouette-1.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-03 13:04:11.567036 mouette-1.1.2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      555 2023-04-03 13:03:54.000000 mouette-1.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.563037 mouette-1.1.2/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:04:11.567036 mouette-1.1.2/tests/data/
--rw-rw-r--   0 root         (0) root         (0)       98 2022-08-21 17:58:18.000000 mouette-1.1.2/tests/data/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    43817 2022-08-21 17:58:18.000000 mouette-1.1.2/tests/data/circle.mesh
--rw-rw-r--   0 root         (0) root         (0)      246 2022-08-21 17:58:18.000000 mouette-1.1.2/tests/data/cube.tet
--rw-rw-r--   0 root         (0) root         (0)     3331 2022-08-21 17:58:18.000000 mouette-1.1.2/tests/data/cube86.mesh
--rw-rw-r--   0 root         (0) root         (0)     7649 2022-08-21 17:58:18.000000 mouette-1.1.2/tests/data/feature2.obj
--rw-rw-r--   0 root         (0) root         (0)     4451 2022-08-21 17:58:18.000000 mouette-1.1.2/tests/data/half_sphere1.obj
--rw-rw-r--   0 root         (0) root         (0)   318541 2022-08-21 17:58:18.000000 mouette-1.1.2/tests/data/join.tet
--rw-rw-r--   0 root         (0) root         (0)      170 2022-08-21 17:58:18.000000 mouette-1.1.2/tests/data/one_ring_permut.obj
--rw-rw-r--   0 root         (0) root         (0)   158537 2022-08-21 17:58:18.000000 mouette-1.1.2/tests/data/p01.mesh
--rw-rw-r--   0 root         (0) root         (0)      634 2022-08-21 18:01:16.000000 mouette-1.1.2/tests/data/pointclouds.py
--rw-rw-r--   0 root         (0) root         (0)    26740 2022-08-21 17:58:18.000000 mouette-1.1.2/tests/data/pointy.obj
--rw-rw-r--   0 root         (0) root         (0)      945 2023-04-03 09:28:37.000000 mouette-1.1.2/tests/data/polylines.py
--rw-rw-r--   0 root         (0) root         (0)     1893 2022-08-21 17:58:18.000000 mouette-1.1.2/tests/data/quad_split2.geogram_ascii
--rw-rw-r--   0 root         (0) root         (0)      120 2022-08-21 17:58:18.000000 mouette-1.1.2/tests/data/quads.obj
--rw-rw-r--   0 root         (0) root         (0)     9018 2022-08-21 17:58:18.000000 mouette-1.1.2/tests/data/spline03.mesh
--rw-rw-r--   0 root         (0) root         (0)     2151 2023-04-01 09:44:06.000000 mouette-1.1.2/tests/data/surfaces.py
--rw-rw-r--   0 root         (0) root         (0)     1647 2022-08-21 17:58:18.000000 mouette-1.1.2/tests/data/two_pieces.obj
--rw-rw-r--   0 root         (0) root         (0)    19263 2023-04-01 09:43:05.000000 mouette-1.1.2/tests/data/uv_sphere_nopoles_quad.obj
--rw-rw-r--   0 root         (0) root         (0)      723 2023-02-06 13:13:45.000000 mouette-1.1.2/tests/data/volumes.py
--rw-rw-r--   0 root         (0) root         (0)     5812 2023-02-03 15:42:26.000000 mouette-1.1.2/tests/test_attributes.py
--rw-rw-r--   0 root         (0) root         (0)      736 2023-02-05 19:53:22.000000 mouette-1.1.2/tests/test_features.py
--rw-rw-r--   0 root         (0) root         (0)     4835 2023-03-31 08:42:39.000000 mouette-1.1.2/tests/test_ff_surface.py
--rw-rw-r--   0 root         (0) root         (0)      543 2023-03-31 08:45:22.000000 mouette-1.1.2/tests/test_ff_volumes.py
--rw-rw-r--   0 root         (0) root         (0)     3043 2022-08-21 22:36:17.000000 mouette-1.1.2/tests/test_geometry.py
--rw-rw-r--   0 root         (0) root         (0)     2479 2023-03-31 08:47:32.000000 mouette-1.1.2/tests/test_levenberg_marquardt.py
--rw-rw-r--   0 root         (0) root         (0)     1196 2023-04-03 12:35:46.000000 mouette-1.1.2/tests/test_maths.py
--rw-rw-r--   0 root         (0) root         (0)      730 2022-08-21 22:38:15.000000 mouette-1.1.2/tests/test_operators.py
--rw-rw-r--   0 root         (0) root         (0)     3747 2023-04-02 19:27:48.000000 mouette-1.1.2/tests/test_param.py
--rw-rw-r--   0 root         (0) root         (0)     1305 2022-08-21 18:01:16.000000 mouette-1.1.2/tests/test_procedural.py
--rw-rw-r--   0 root         (0) root         (0)     1020 2022-08-21 18:01:16.000000 mouette-1.1.2/tests/test_quantities.py
--rw-rw-r--   0 root         (0) root         (0)     1997 2022-08-21 18:01:16.000000 mouette-1.1.2/tests/test_surfaces.py
--rw-rw-r--   0 root         (0) root         (0)     2135 2022-08-21 18:01:16.000000 mouette-1.1.2/tests/test_tree.py
--rw-rw-r--   0 root         (0) root         (0)     4885 2023-04-03 13:03:21.000000 mouette-1.1.2/tests/test_utils.py
--rw-rw-r--   0 root         (0) root         (0)      823 2022-08-21 18:01:16.000000 mouette-1.1.2/tests/test_vec.py
--rw-rw-r--   0 root         (0) root         (0)      614 2022-08-21 18:01:16.000000 mouette-1.1.2/tests/test_volumes.py
--rw-rw-r--   0 root         (0) root         (0)      971 2022-08-21 18:01:16.000000 mouette-1.1.2/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.265868 mouette-1.1.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.245868 mouette-1.1.3/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.245868 mouette-1.1.3/.github/workflows/
+-rw-rw-r--   0 root         (0) root         (0)      343 2022-09-01 08:22:07.000000 mouette-1.1.3/.github/workflows/docs.yml
+-rw-rw-r--   0 root         (0) root         (0)     1091 2022-08-23 12:53:25.000000 mouette-1.1.3/.github/workflows/python-publish.yml
+-rw-rw-r--   0 root         (0) root         (0)     1843 2022-08-21 17:58:18.000000 mouette-1.1.3/.gitignore
+-rw-rw-r--   0 root         (0) root         (0)     1075 2022-08-21 17:58:18.000000 mouette-1.1.3/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      134 2023-05-23 09:12:42.000000 mouette-1.1.3/Makefile
+-rw-r--r--   0 root         (0) root         (0)     1956 2023-05-23 09:12:52.265868 mouette-1.1.3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1698 2023-02-05 20:34:49.000000 mouette-1.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.245868 mouette-1.1.3/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.245868 mouette-1.1.3/docs/Algorithms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.249868 mouette-1.1.3/docs/Algorithms/Frame Fields/
+-rw-rw-r--   0 root         (0) root         (0)     1722 2023-02-06 14:19:10.000000 mouette-1.1.3/docs/Algorithms/Frame Fields/00_framefields.md
+-rw-rw-r--   0 root         (0) root         (0)      102 2023-02-06 13:49:38.000000 mouette-1.1.3/docs/Algorithms/Frame Fields/01_2dFF.md
+-rw-rw-r--   0 root         (0) root         (0)      164 2023-02-06 14:08:01.000000 mouette-1.1.3/docs/Algorithms/Frame Fields/02_Curvature.md
+-rw-rw-r--   0 root         (0) root         (0)     1213 2023-02-06 14:42:19.000000 mouette-1.1.3/docs/Algorithms/Frame Fields/03_3dFF.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.249868 mouette-1.1.3/docs/Algorithms/Parametrization/
+-rw-rw-r--   0 root         (0) root         (0)       88 2023-04-03 08:35:48.000000 mouette-1.1.3/docs/Algorithms/Parametrization/00_distortion.md
+-rw-rw-r--   0 root         (0) root         (0)      305 2023-02-06 15:04:20.000000 mouette-1.1.3/docs/Algorithms/Parametrization/Tutte.md
+-rw-rw-r--   0 root         (0) root         (0)      387 2023-02-06 15:12:47.000000 mouette-1.1.3/docs/Algorithms/Parametrization/cotan_embedding.md
+-rw-rw-r--   0 root         (0) root         (0)      355 2023-02-06 14:58:37.000000 mouette-1.1.3/docs/Algorithms/Parametrization/lscm.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.249868 mouette-1.1.3/docs/Algorithms/Trees/
+-rw-rw-r--   0 root         (0) root         (0)        4 2022-08-30 12:42:01.000000 mouette-1.1.3/docs/Algorithms/Trees/tree.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.249868 mouette-1.1.3/docs/Attributes/
+-rw-rw-r--   0 root         (0) root         (0)       62 2022-09-26 16:03:21.000000 mouette-1.1.3/docs/Attributes/01_global.md
+-rw-rw-r--   0 root         (0) root         (0)       65 2022-09-26 16:03:26.000000 mouette-1.1.3/docs/Attributes/02_vertices.md
+-rw-rw-r--   0 root         (0) root         (0)       59 2022-09-26 16:03:34.000000 mouette-1.1.3/docs/Attributes/03_edges.md
+-rw-rw-r--   0 root         (0) root         (0)       59 2022-09-26 16:01:39.000000 mouette-1.1.3/docs/Attributes/04_faces.md
+-rw-rw-r--   0 root         (0) root         (0)       68 2022-09-26 16:01:35.000000 mouette-1.1.3/docs/Attributes/05_corners.md
+-rw-rw-r--   0 root         (0) root         (0)       59 2022-09-26 16:01:32.000000 mouette-1.1.3/docs/Attributes/06_cells.md
+-rw-rw-r--   0 root         (0) root         (0)       75 2022-09-26 16:03:32.000000 mouette-1.1.3/docs/Attributes/07_interpolation.md
+-rw-rw-r--   0 root         (0) root         (0)      424 2023-04-03 08:29:29.000000 mouette-1.1.3/docs/Dependencies.md
+-rw-rw-r--   0 root         (0) root         (0)      176 2022-08-21 17:58:18.000000 mouette-1.1.3/docs/Design Philosophy.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.249868 mouette-1.1.3/docs/Geometry/
+-rw-rw-r--   0 root         (0) root         (0)      654 2023-02-06 14:42:17.000000 mouette-1.1.3/docs/Geometry/spherical_harmonics.md
+-rw-rw-r--   0 root         (0) root         (0)       36 2022-08-21 17:58:18.000000 mouette-1.1.3/docs/Loading and Saving.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.249868 mouette-1.1.3/docs/Meshes and Datastructures/
+-rw-rw-r--   0 root         (0) root         (0)       73 2023-04-03 08:55:54.000000 mouette-1.1.3/docs/Meshes and Datastructures/00_RawMeshData.md
+-rw-rw-r--   0 root         (0) root         (0)      294 2023-04-03 09:30:16.000000 mouette-1.1.3/docs/Meshes and Datastructures/01_PointClouds.md
+-rw-rw-r--   0 root         (0) root         (0)      445 2023-04-03 09:30:18.000000 mouette-1.1.3/docs/Meshes and Datastructures/02_PolyLines.md
+-rw-rw-r--   0 root         (0) root         (0)      422 2023-04-03 10:41:25.000000 mouette-1.1.3/docs/Meshes and Datastructures/03_SurfaceMeshes.md
+-rw-rw-r--   0 root         (0) root         (0)       64 2023-04-03 08:34:41.000000 mouette-1.1.3/docs/Meshes and Datastructures/04_VolumeMeshes.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.249868 mouette-1.1.3/docs/Utilities/
+-rw-rw-r--   0 root         (0) root         (0)       64 2023-02-07 13:44:55.000000 mouette-1.1.3/docs/Utilities/priority_queue.md
+-rw-rw-r--   0 root         (0) root         (0)       55 2023-02-07 14:12:00.000000 mouette-1.1.3/docs/Utilities/union_find.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.253868 mouette-1.1.3/docs/_img/
+-rw-rw-r--   0 root         (0) root         (0)   269170 2023-04-03 10:40:50.000000 mouette-1.1.3/docs/_img/bunny_tri.jpeg
+-rw-rw-r--   0 root         (0) root         (0)   155178 2023-04-03 09:26:50.000000 mouette-1.1.3/docs/_img/duck_polyline.jpeg
+-rw-rw-r--   0 root         (0) root         (0)   166130 2023-04-03 09:07:13.000000 mouette-1.1.3/docs/_img/point_cloud_cad_example.jpeg
+-rw-rw-r--   0 root         (0) root         (0)     1585 2022-09-05 13:21:43.000000 mouette-1.1.3/docs/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.253868 mouette-1.1.3/examples/
+-rw-rw-r--   0 root         (0) root         (0)     2120 2023-02-07 13:59:53.000000 mouette-1.1.3/examples/framefield2D.py
+-rw-rw-r--   0 root         (0) root         (0)      421 2022-09-26 15:25:06.000000 mouette-1.1.3/examples/framefield3D.py
+-rw-rw-r--   0 root         (0) root         (0)      391 2022-09-26 15:23:43.000000 mouette-1.1.3/examples/lscm.py
+-rw-rw-r--   0 root         (0) root         (0)      792 2023-04-03 09:19:59.000000 mouette-1.1.3/mkdocs.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.253868 mouette-1.1.3/mouette/
+-rw-rw-r--   0 root         (0) root         (0)      590 2023-03-28 12:25:47.000000 mouette-1.1.3/mouette/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.253868 mouette-1.1.3/mouette/attributes/
+-rw-rw-r--   0 root         (0) root         (0)      181 2022-08-21 17:58:18.000000 mouette-1.1.3/mouette/attributes/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3469 2022-09-26 16:06:27.000000 mouette-1.1.3/mouette/attributes/glob.py
+-rw-rw-r--   0 root         (0) root         (0)     4296 2022-12-23 14:05:48.000000 mouette-1.1.3/mouette/attributes/interpolate.py
+-rw-rw-r--   0 root         (0) root         (0)     3142 2022-09-26 16:21:57.000000 mouette-1.1.3/mouette/attributes/misc_cells.py
+-rw-rw-r--   0 root         (0) root         (0)     3081 2022-10-05 08:17:26.000000 mouette-1.1.3/mouette/attributes/misc_corners.py
+-rw-rw-r--   0 root         (0) root         (0)     3627 2022-11-17 16:57:39.000000 mouette-1.1.3/mouette/attributes/misc_edges.py
+-rw-rw-r--   0 root         (0) root         (0)     8500 2023-02-04 13:53:10.000000 mouette-1.1.3/mouette/attributes/misc_faces.py
+-rw-rw-r--   0 root         (0) root         (0)     6836 2023-02-04 13:52:44.000000 mouette-1.1.3/mouette/attributes/misc_vertices.py
+-rw-rw-r--   0 root         (0) root         (0)     1172 2022-09-01 08:24:31.000000 mouette-1.1.3/mouette/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.253868 mouette-1.1.3/mouette/geometry/
+-rw-rw-r--   0 root         (0) root         (0)    15644 2023-04-03 08:58:44.000000 mouette-1.1.3/mouette/geometry/SphericalHarmonics.py
+-rw-rw-r--   0 root         (0) root         (0)      105 2022-08-21 17:58:18.000000 mouette-1.1.3/mouette/geometry/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6085 2022-11-26 16:01:37.000000 mouette-1.1.3/mouette/geometry/geometry.py
+-rw-rw-r--   0 root         (0) root         (0)     2408 2022-09-26 15:52:39.000000 mouette-1.1.3/mouette/geometry/rotations.py
+-rw-rw-r--   0 root         (0) root         (0)     3876 2022-09-26 15:52:39.000000 mouette-1.1.3/mouette/geometry/transform.py
+-rw-rw-r--   0 root         (0) root         (0)     1738 2022-10-03 15:16:09.000000 mouette-1.1.3/mouette/geometry/vector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.253868 mouette-1.1.3/mouette/mesh/
+-rw-rw-r--   0 root         (0) root         (0)      201 2022-08-21 17:58:18.000000 mouette-1.1.3/mouette/mesh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.257868 mouette-1.1.3/mouette/mesh/datatypes/
+-rw-rw-r--   0 root         (0) root         (0)      216 2022-08-21 17:58:18.000000 mouette-1.1.3/mouette/mesh/datatypes/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      574 2022-08-21 18:04:49.000000 mouette-1.1.3/mouette/mesh/datatypes/base.py
+-rw-rw-r--   0 root         (0) root         (0)     5250 2023-04-03 11:04:41.000000 mouette-1.1.3/mouette/mesh/datatypes/linear.py
+-rw-rw-r--   0 root         (0) root         (0)      904 2023-04-03 09:18:41.000000 mouette-1.1.3/mouette/mesh/datatypes/pointcloud.py
+-rw-rw-r--   0 root         (0) root         (0)    20178 2023-04-03 11:10:23.000000 mouette-1.1.3/mouette/mesh/datatypes/surface.py
+-rw-rw-r--   0 root         (0) root         (0)     1767 2023-02-06 08:16:44.000000 mouette-1.1.3/mouette/mesh/datatypes/type_checks.py
+-rw-rw-r--   0 root         (0) root         (0)    20556 2023-01-13 14:12:51.000000 mouette-1.1.3/mouette/mesh/datatypes/volume.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.257868 mouette-1.1.3/mouette/mesh/io/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-21 17:58:18.000000 mouette-1.1.3/mouette/mesh/io/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    14541 2023-05-23 09:11:47.000000 mouette-1.1.3/mouette/mesh/io/geogram_ascii.py
+-rw-rw-r--   0 root         (0) root         (0)     1218 2022-08-21 17:58:18.000000 mouette-1.1.3/mouette/mesh/io/io.py
+-rw-rw-r--   0 root         (0) root         (0)     4999 2022-08-21 17:58:18.000000 mouette-1.1.3/mouette/mesh/io/medit.py
+-rw-rw-r--   0 root         (0) root         (0)     4237 2023-03-07 15:31:45.000000 mouette-1.1.3/mouette/mesh/io/obj.py
+-rw-rw-r--   0 root         (0) root         (0)     2191 2022-09-26 15:52:39.000000 mouette-1.1.3/mouette/mesh/io/off.py
+-rw-rw-r--   0 root         (0) root         (0)     1494 2022-09-26 15:52:39.000000 mouette-1.1.3/mouette/mesh/io/tet.py
+-rw-rw-r--   0 root         (0) root         (0)      870 2022-09-26 15:52:39.000000 mouette-1.1.3/mouette/mesh/io/xyz.py
+-rw-rw-r--   0 root         (0) root         (0)     5596 2022-09-26 15:52:39.000000 mouette-1.1.3/mouette/mesh/mesh.py
+-rw-rw-r--   0 root         (0) root         (0)    12499 2023-03-07 15:31:43.000000 mouette-1.1.3/mouette/mesh/mesh_attributes.py
+-rw-rw-r--   0 root         (0) root         (0)    10057 2023-02-10 12:43:27.000000 mouette-1.1.3/mouette/mesh/mesh_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.257868 mouette-1.1.3/mouette/operators/
+-rw-rw-r--   0 root         (0) root         (0)       49 2022-08-21 17:58:18.000000 mouette-1.1.3/mouette/operators/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2247 2022-09-26 15:52:39.000000 mouette-1.1.3/mouette/operators/adjacency.py
+-rw-rw-r--   0 root         (0) root         (0)     9252 2023-02-06 13:27:42.000000 mouette-1.1.3/mouette/operators/laplacian.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.257868 mouette-1.1.3/mouette/optimize/
+-rw-rw-r--   0 root         (0) root         (0)       77 2023-02-28 17:07:06.000000 mouette-1.1.3/mouette/optimize/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1291 2022-10-03 12:39:49.000000 mouette-1.1.3/mouette/optimize/eigensolve.py
+-rw-rw-r--   0 root         (0) root         (0)    12794 2023-03-31 14:53:04.000000 mouette-1.1.3/mouette/optimize/levenberg_marquardt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.257868 mouette-1.1.3/mouette/procedural/
+-rw-rw-r--   0 root         (0) root         (0)      278 2022-08-21 17:58:18.000000 mouette-1.1.3/mouette/procedural/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1791 2022-09-26 15:52:39.000000 mouette-1.1.3/mouette/procedural/cylinder.py
+-rw-rw-r--   0 root         (0) root         (0)     1567 2022-09-26 15:52:39.000000 mouette-1.1.3/mouette/procedural/hexahedra.py
+-rw-rw-r--   0 root         (0) root         (0)     3109 2022-09-26 15:52:39.000000 mouette-1.1.3/mouette/procedural/platonic.py
+-rw-rw-r--   0 root         (0) root         (0)     2787 2022-12-23 16:00:47.000000 mouette-1.1.3/mouette/procedural/rings.py
+-rw-rw-r--   0 root         (0) root         (0)     3690 2022-09-26 15:52:39.000000 mouette-1.1.3/mouette/procedural/sphere.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.257868 mouette-1.1.3/mouette/processing/
+-rw-rw-r--   0 root         (0) root         (0)      559 2023-03-28 12:25:34.000000 mouette-1.1.3/mouette/processing/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3907 2023-05-12 13:23:14.000000 mouette-1.1.3/mouette/processing/border.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.257868 mouette-1.1.3/mouette/processing/combinatorics/
+-rw-rw-r--   0 root         (0) root         (0)       63 2022-08-21 17:58:18.000000 mouette-1.1.3/mouette/processing/combinatorics/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    17363 2023-04-01 09:08:53.000000 mouette-1.1.3/mouette/processing/combinatorics/cutting.py
+-rw-rw-r--   0 root         (0) root         (0)     8183 2023-04-03 08:02:11.000000 mouette-1.1.3/mouette/processing/combinatorics/subdivide.py
+-rw-rw-r--   0 root         (0) root         (0)     7776 2023-03-31 11:49:03.000000 mouette-1.1.3/mouette/processing/connection.py
+-rw-rw-r--   0 root         (0) root         (0)     9206 2023-01-10 09:34:21.000000 mouette-1.1.3/mouette/processing/features.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.257868 mouette-1.1.3/mouette/processing/framefield/
+-rw-rw-r--   0 root         (0) root         (0)       92 2023-03-28 12:25:46.000000 mouette-1.1.3/mouette/processing/framefield/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1348 2023-02-06 16:09:04.000000 mouette-1.1.3/mouette/processing/framefield/base.py
+-rw-rw-r--   0 root         (0) root         (0)    13554 2023-02-06 13:24:01.000000 mouette-1.1.3/mouette/processing/framefield/cells.py
+-rw-rw-r--   0 root         (0) root         (0)     3871 2023-02-06 08:04:19.000000 mouette-1.1.3/mouette/processing/framefield/curvature_faces.py
+-rw-rw-r--   0 root         (0) root         (0)     8467 2023-02-06 08:16:41.000000 mouette-1.1.3/mouette/processing/framefield/curvature_vertex.py
+-rw-rw-r--   0 root         (0) root         (0)    14527 2023-04-06 09:20:05.000000 mouette-1.1.3/mouette/processing/framefield/faces2d.py
+-rw-rw-r--   0 root         (0) root         (0)    10844 2023-04-06 10:38:09.000000 mouette-1.1.3/mouette/processing/framefield/framefield.py
+-rw-rw-r--   0 root         (0) root         (0)    18227 2023-04-06 10:33:42.000000 mouette-1.1.3/mouette/processing/framefield/vertex2d.py
+-rw-rw-r--   0 root         (0) root         (0)    12249 2023-02-06 13:26:49.000000 mouette-1.1.3/mouette/processing/framefield/vertex3d.py
+-rw-rw-r--   0 root         (0) root         (0)     2933 2023-03-30 13:16:33.000000 mouette-1.1.3/mouette/processing/misc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.257868 mouette-1.1.3/mouette/processing/parametrization/
+-rw-rw-r--   0 root         (0) root         (0)      147 2022-12-04 21:19:32.000000 mouette-1.1.3/mouette/processing/parametrization/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1534 2023-04-01 10:34:36.000000 mouette-1.1.3/mouette/processing/parametrization/base.py
+-rw-rw-r--   0 root         (0) root         (0)    10003 2023-04-01 10:37:07.000000 mouette-1.1.3/mouette/processing/parametrization/cotan_emb.py
+-rw-rw-r--   0 root         (0) root         (0)    12940 2023-04-01 09:46:25.000000 mouette-1.1.3/mouette/processing/parametrization/distortion.py
+-rw-rw-r--   0 root         (0) root         (0)     5991 2023-04-01 10:31:45.000000 mouette-1.1.3/mouette/processing/parametrization/lscm.py
+-rw-rw-r--   0 root         (0) root         (0)     5517 2023-05-12 13:32:31.000000 mouette-1.1.3/mouette/processing/parametrization/tutte.py
+-rw-rw-r--   0 root         (0) root         (0)     8822 2023-03-06 08:49:04.000000 mouette-1.1.3/mouette/processing/paths.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.261868 mouette-1.1.3/mouette/processing/trees/
+-rw-rw-r--   0 root         (0) root         (0)      198 2022-08-21 17:58:18.000000 mouette-1.1.3/mouette/processing/trees/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3225 2022-09-26 15:52:39.000000 mouette-1.1.3/mouette/processing/trees/base.py
+-rw-rw-r--   0 root         (0) root         (0)     3223 2022-08-21 17:58:18.000000 mouette-1.1.3/mouette/processing/trees/cell_sp.py
+-rw-rw-r--   0 root         (0) root         (0)     8242 2022-09-26 15:52:39.000000 mouette-1.1.3/mouette/processing/trees/edge_sp.py
+-rw-rw-r--   0 root         (0) root         (0)     3399 2023-03-06 08:03:29.000000 mouette-1.1.3/mouette/processing/trees/face_sp.py
+-rw-rw-r--   0 root         (0) root         (0)      451 2022-08-21 18:01:16.000000 mouette-1.1.3/mouette/processing/worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.261868 mouette-1.1.3/mouette/utils/
+-rw-rw-r--   0 root         (0) root         (0)      174 2023-02-03 15:31:47.000000 mouette-1.1.3/mouette/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2159 2023-02-03 16:51:10.000000 mouette-1.1.3/mouette/utils/argument_check.py
+-rw-rw-r--   0 root         (0) root         (0)     1744 2022-10-06 15:31:15.000000 mouette-1.1.3/mouette/utils/iterators.py
+-rw-rw-r--   0 root         (0) root         (0)     1476 2023-03-28 11:32:27.000000 mouette-1.1.3/mouette/utils/maths.py
+-rw-rw-r--   0 root         (0) root         (0)     2031 2023-04-03 12:41:10.000000 mouette-1.1.3/mouette/utils/priority_queue.py
+-rw-rw-r--   0 root         (0) root         (0)     8788 2023-04-03 13:03:23.000000 mouette-1.1.3/mouette/utils/unionfind.py
+-rw-rw-r--   0 root         (0) root         (0)     1106 2023-04-03 12:05:05.000000 mouette-1.1.3/mouette/utils/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.253868 mouette-1.1.3/mouette.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1956 2023-05-23 09:12:52.000000 mouette-1.1.3/mouette.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5117 2023-05-23 09:12:52.000000 mouette-1.1.3/mouette.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 09:12:52.000000 mouette-1.1.3/mouette.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-23 09:12:52.000000 mouette-1.1.3/mouette.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-23 09:12:52.000000 mouette-1.1.3/mouette.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      756 2023-05-23 09:12:36.000000 mouette-1.1.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 09:12:52.265868 mouette-1.1.3/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      555 2023-05-23 09:12:41.000000 mouette-1.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.261868 mouette-1.1.3/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 09:12:52.265868 mouette-1.1.3/tests/data/
+-rw-rw-r--   0 root         (0) root         (0)       98 2022-08-21 17:58:18.000000 mouette-1.1.3/tests/data/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    43817 2022-08-21 17:58:18.000000 mouette-1.1.3/tests/data/circle.mesh
+-rw-rw-r--   0 root         (0) root         (0)      246 2022-08-21 17:58:18.000000 mouette-1.1.3/tests/data/cube.tet
+-rw-rw-r--   0 root         (0) root         (0)     3331 2022-08-21 17:58:18.000000 mouette-1.1.3/tests/data/cube86.mesh
+-rw-rw-r--   0 root         (0) root         (0)     7649 2022-08-21 17:58:18.000000 mouette-1.1.3/tests/data/feature2.obj
+-rw-rw-r--   0 root         (0) root         (0)     4451 2022-08-21 17:58:18.000000 mouette-1.1.3/tests/data/half_sphere1.obj
+-rw-rw-r--   0 root         (0) root         (0)   318541 2022-08-21 17:58:18.000000 mouette-1.1.3/tests/data/join.tet
+-rw-rw-r--   0 root         (0) root         (0)      170 2022-08-21 17:58:18.000000 mouette-1.1.3/tests/data/one_ring_permut.obj
+-rw-rw-r--   0 root         (0) root         (0)   158537 2022-08-21 17:58:18.000000 mouette-1.1.3/tests/data/p01.mesh
+-rw-rw-r--   0 root         (0) root         (0)      634 2022-08-21 18:01:16.000000 mouette-1.1.3/tests/data/pointclouds.py
+-rw-rw-r--   0 root         (0) root         (0)    26740 2022-08-21 17:58:18.000000 mouette-1.1.3/tests/data/pointy.obj
+-rw-rw-r--   0 root         (0) root         (0)      945 2023-04-03 09:28:37.000000 mouette-1.1.3/tests/data/polylines.py
+-rw-rw-r--   0 root         (0) root         (0)     1893 2022-08-21 17:58:18.000000 mouette-1.1.3/tests/data/quad_split2.geogram_ascii
+-rw-rw-r--   0 root         (0) root         (0)      120 2022-08-21 17:58:18.000000 mouette-1.1.3/tests/data/quads.obj
+-rw-rw-r--   0 root         (0) root         (0)     9018 2022-08-21 17:58:18.000000 mouette-1.1.3/tests/data/spline03.mesh
+-rw-rw-r--   0 root         (0) root         (0)     2151 2023-04-01 09:44:06.000000 mouette-1.1.3/tests/data/surfaces.py
+-rw-rw-r--   0 root         (0) root         (0)     1647 2022-08-21 17:58:18.000000 mouette-1.1.3/tests/data/two_pieces.obj
+-rw-rw-r--   0 root         (0) root         (0)    19263 2023-04-01 09:43:05.000000 mouette-1.1.3/tests/data/uv_sphere_nopoles_quad.obj
+-rw-rw-r--   0 root         (0) root         (0)      723 2023-02-06 13:13:45.000000 mouette-1.1.3/tests/data/volumes.py
+-rw-rw-r--   0 root         (0) root         (0)     5812 2023-02-03 15:42:26.000000 mouette-1.1.3/tests/test_attributes.py
+-rw-rw-r--   0 root         (0) root         (0)      736 2023-02-05 19:53:22.000000 mouette-1.1.3/tests/test_features.py
+-rw-rw-r--   0 root         (0) root         (0)     4835 2023-03-31 08:42:39.000000 mouette-1.1.3/tests/test_ff_surface.py
+-rw-rw-r--   0 root         (0) root         (0)      543 2023-03-31 08:45:22.000000 mouette-1.1.3/tests/test_ff_volumes.py
+-rw-rw-r--   0 root         (0) root         (0)     3043 2022-08-21 22:36:17.000000 mouette-1.1.3/tests/test_geometry.py
+-rw-rw-r--   0 root         (0) root         (0)     2479 2023-03-31 08:47:32.000000 mouette-1.1.3/tests/test_levenberg_marquardt.py
+-rw-rw-r--   0 root         (0) root         (0)     1196 2023-04-03 12:35:46.000000 mouette-1.1.3/tests/test_maths.py
+-rw-rw-r--   0 root         (0) root         (0)      730 2022-08-21 22:38:15.000000 mouette-1.1.3/tests/test_operators.py
+-rw-rw-r--   0 root         (0) root         (0)     3747 2023-04-02 19:27:48.000000 mouette-1.1.3/tests/test_param.py
+-rw-rw-r--   0 root         (0) root         (0)     1305 2022-08-21 18:01:16.000000 mouette-1.1.3/tests/test_procedural.py
+-rw-rw-r--   0 root         (0) root         (0)     1020 2022-08-21 18:01:16.000000 mouette-1.1.3/tests/test_quantities.py
+-rw-rw-r--   0 root         (0) root         (0)     1997 2022-08-21 18:01:16.000000 mouette-1.1.3/tests/test_surfaces.py
+-rw-rw-r--   0 root         (0) root         (0)     2135 2022-08-21 18:01:16.000000 mouette-1.1.3/tests/test_tree.py
+-rw-rw-r--   0 root         (0) root         (0)     4885 2023-04-03 13:03:21.000000 mouette-1.1.3/tests/test_utils.py
+-rw-rw-r--   0 root         (0) root         (0)      823 2022-08-21 18:01:16.000000 mouette-1.1.3/tests/test_vec.py
+-rw-rw-r--   0 root         (0) root         (0)      614 2022-08-21 18:01:16.000000 mouette-1.1.3/tests/test_volumes.py
+-rw-rw-r--   0 root         (0) root         (0)      971 2022-08-21 18:01:16.000000 mouette-1.1.3/tests/utils.py
```

### Comparing `mouette-1.1.2/.github/workflows/python-publish.yml` & `mouette-1.1.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/.gitignore` & `mouette-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/LICENSE` & `mouette-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/PKG-INFO` & `mouette-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mouette
-Version: 1.1.2
+Version: 1.1.3
 Summary: Mesh, Tools and Geometry Processing
 Home-page: https://github.com/GCoiffier/mouette
 Author: GCoiffier
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mouette-1.1.2/README.md` & `mouette-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/docs/Algorithms/Frame Fields/00_framefields.md` & `mouette-1.1.3/docs/Algorithms/Frame Fields/00_framefields.md`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/docs/Algorithms/Frame Fields/03_3dFF.md` & `mouette-1.1.3/docs/Algorithms/Frame Fields/03_3dFF.md`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/docs/Geometry/spherical_harmonics.md` & `mouette-1.1.3/docs/Geometry/spherical_harmonics.md`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/docs/_img/bunny_tri.jpeg` & `mouette-1.1.3/docs/_img/bunny_tri.jpeg`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/docs/_img/duck_polyline.jpeg` & `mouette-1.1.3/docs/_img/duck_polyline.jpeg`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/docs/_img/point_cloud_cad_example.jpeg` & `mouette-1.1.3/docs/_img/point_cloud_cad_example.jpeg`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/docs/index.md` & `mouette-1.1.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/examples/framefield2D.py` & `mouette-1.1.3/examples/framefield2D.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mkdocs.yml` & `mouette-1.1.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/__init__.py` & `mouette-1.1.3/mouette/__init__.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/attributes/glob.py` & `mouette-1.1.3/mouette/attributes/glob.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/attributes/interpolate.py` & `mouette-1.1.3/mouette/attributes/interpolate.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/attributes/misc_cells.py` & `mouette-1.1.3/mouette/attributes/misc_cells.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/attributes/misc_corners.py` & `mouette-1.1.3/mouette/attributes/misc_corners.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/attributes/misc_edges.py` & `mouette-1.1.3/mouette/attributes/misc_edges.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/attributes/misc_faces.py` & `mouette-1.1.3/mouette/attributes/misc_faces.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/attributes/misc_vertices.py` & `mouette-1.1.3/mouette/attributes/misc_vertices.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/config.py` & `mouette-1.1.3/mouette/config.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/geometry/SphericalHarmonics.py` & `mouette-1.1.3/mouette/geometry/SphericalHarmonics.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/geometry/geometry.py` & `mouette-1.1.3/mouette/geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/geometry/rotations.py` & `mouette-1.1.3/mouette/geometry/rotations.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/geometry/transform.py` & `mouette-1.1.3/mouette/geometry/transform.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/geometry/vector.py` & `mouette-1.1.3/mouette/geometry/vector.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/mesh/datatypes/base.py` & `mouette-1.1.3/mouette/mesh/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/mesh/datatypes/linear.py` & `mouette-1.1.3/mouette/mesh/datatypes/linear.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/mesh/datatypes/pointcloud.py` & `mouette-1.1.3/mouette/mesh/datatypes/pointcloud.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/mesh/datatypes/surface.py` & `mouette-1.1.3/mouette/mesh/datatypes/surface.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/mesh/datatypes/type_checks.py` & `mouette-1.1.3/mouette/mesh/datatypes/type_checks.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/mesh/datatypes/volume.py` & `mouette-1.1.3/mouette/mesh/datatypes/volume.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/mesh/io/geogram_ascii.py` & `mouette-1.1.3/mouette/mesh/io/geogram_ascii.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
             for j in range(attr.elemsize):
                 if attr.type==Attribute.Type.Bool:
                     f.write(f"{int(attr[i][j])}\n")
                 else:
                     f.write(f"{attr[i][j]}\n")
 
 def export_geogram_ascii(mesh : RawMeshData, path):
-    with open(path, "w") as f:
+    with open(path, "w", newline="\n") as f:
         f.write("[HEAD]\n\"GEOGRAM\"\n\"1.0\"\n")
         
         # Vertices
         n_vert = len(mesh.vertices)
         f.write("[ATTS]\n\"GEO::Mesh::vertices\"\n{}\n".format(n_vert))
         f.write("[ATTR]\n\"GEO::Mesh::vertices\"\n\"point\"\n\"double\"\n8\n3\n")
         for i in range(n_vert):
```

### Comparing `mouette-1.1.2/mouette/mesh/io/io.py` & `mouette-1.1.3/mouette/mesh/io/io.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/mesh/io/medit.py` & `mouette-1.1.3/mouette/mesh/io/medit.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/mesh/io/obj.py` & `mouette-1.1.3/mouette/mesh/io/obj.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/mesh/io/off.py` & `mouette-1.1.3/mouette/mesh/io/off.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/mesh/io/tet.py` & `mouette-1.1.3/mouette/mesh/io/tet.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/mesh/io/xyz.py` & `mouette-1.1.3/mouette/mesh/io/xyz.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/mesh/mesh.py` & `mouette-1.1.3/mouette/mesh/mesh.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/mesh/mesh_attributes.py` & `mouette-1.1.3/mouette/mesh/mesh_attributes.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/mesh/mesh_data.py` & `mouette-1.1.3/mouette/mesh/mesh_data.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/operators/adjacency.py` & `mouette-1.1.3/mouette/operators/adjacency.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/operators/laplacian.py` & `mouette-1.1.3/mouette/operators/laplacian.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/optimize/eigensolve.py` & `mouette-1.1.3/mouette/optimize/eigensolve.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/optimize/levenberg_marquardt.py` & `mouette-1.1.3/mouette/optimize/levenberg_marquardt.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/procedural/cylinder.py` & `mouette-1.1.3/mouette/procedural/cylinder.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/procedural/hexahedra.py` & `mouette-1.1.3/mouette/procedural/hexahedra.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/procedural/platonic.py` & `mouette-1.1.3/mouette/procedural/platonic.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/procedural/rings.py` & `mouette-1.1.3/mouette/procedural/rings.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/procedural/sphere.py` & `mouette-1.1.3/mouette/procedural/sphere.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/processing/__init__.py` & `mouette-1.1.3/mouette/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/processing/border.py` & `mouette-1.1.3/mouette/processing/border.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ..mesh.mesh_data import RawMeshData
 from ..utils import keyify
 from ..mesh.datatypes import *
 from ..mesh.mesh_attributes import Attribute
 
 @allowed_mesh_types(SurfaceMesh)
-def extract_border_cycle(mesh : SurfaceMesh, starting_point : int = None) -> PolyLine:
+def extract_border_cycle(mesh : SurfaceMesh, starting_point : int = None):
     """
     Extracts a list of vertices that are on the border of the mesh.
 
     Parameters:
         mesh (Mesh): The mesh
         starting_point (int): Origin point. Should be on border
```

### Comparing `mouette-1.1.2/mouette/processing/combinatorics/cutting.py` & `mouette-1.1.3/mouette/processing/combinatorics/cutting.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/processing/combinatorics/subdivide.py` & `mouette-1.1.3/mouette/processing/combinatorics/subdivide.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/processing/connection.py` & `mouette-1.1.3/mouette/processing/connection.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/processing/features.py` & `mouette-1.1.3/mouette/processing/features.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/processing/framefield/base.py` & `mouette-1.1.3/mouette/processing/framefield/base.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/processing/framefield/cells.py` & `mouette-1.1.3/mouette/processing/framefield/cells.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/processing/framefield/curvature_faces.py` & `mouette-1.1.3/mouette/processing/framefield/curvature_faces.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/processing/framefield/curvature_vertex.py` & `mouette-1.1.3/mouette/processing/framefield/curvature_vertex.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/processing/framefield/faces2d.py` & `mouette-1.1.3/mouette/processing/framefield/faces2d.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/processing/framefield/framefield.py` & `mouette-1.1.3/mouette/processing/framefield/framefield.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/processing/framefield/vertex2d.py` & `mouette-1.1.3/mouette/processing/framefield/vertex2d.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/processing/framefield/vertex3d.py` & `mouette-1.1.3/mouette/processing/framefield/vertex3d.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/processing/misc.py` & `mouette-1.1.3/mouette/processing/misc.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/processing/parametrization/base.py` & `mouette-1.1.3/mouette/processing/parametrization/base.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/processing/parametrization/cotan_emb.py` & `mouette-1.1.3/mouette/processing/parametrization/cotan_emb.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/processing/parametrization/distortion.py` & `mouette-1.1.3/mouette/processing/parametrization/distortion.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/processing/parametrization/lscm.py` & `mouette-1.1.3/mouette/processing/parametrization/lscm.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/processing/parametrization/tutte.py` & `mouette-1.1.3/mouette/processing/parametrization/tutte.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,57 +15,67 @@
 
 class TutteEmbedding(BaseParametrization):
     """
     Tutte's embedding parametrization method for a disk inside a fixed boundary.
     The parametrization is locally injective (Floater, 1997) provided the boundary is convex.
 
     References:
-        How to draw a graph, Tutte, 1963.
+        [1] How to draw a graph, Tutte, 1963.
+        [2] Parametrization and smooth approximation of surface triangulations, Floater, 1996.
     """
 
     class BoundaryMode(Enum):
         """
         Enum that represents the shape of the boundary curve.
         """
         CIRCLE = 0
         SQUARE = 1
+        CUSTOM = 2
 
         @staticmethod
         def from_string(s :str):
             if "circle" in s.lower():
                 return TutteEmbedding.BoundaryMode.CIRCLE
             if "square" in s.lower():
                 return TutteEmbedding.BoundaryMode.SQUARE
-            raise Exception(f"'{s}' does correspond to any boundary mode. Choices are : 'circle', 'square'")
+            if "custom" in s.lower():
+                return TutteEmbedding.BoundaryMode.CUSTOM
+            raise Exception(f"'{s}' does correspond to any boundary mode. Choices are : 'circle', 'square', 'custom'")
 
-    def __init__(self, mesh:SurfaceMesh, boundary_mode:str = "circle", verbose:bool=True, **kwargs):
+    def __init__(self, mesh:SurfaceMesh, boundary_mode:str = "circle", use_cotan:bool=False, verbose:bool=True, **kwargs):
         """
         Initializer of the Tutte's embedding tool.
 
         Args:
             mesh (SurfaceMesh): the mesh to embed. Should be a surface with disk topology.
             boundary_mode (str, optional): Shape of the boundary. Possible choices are ["square", "circle"]. Defaults to "circle".
+            use_cotan (bool, optional): whether to use Tutte's original barycentric embedding [1], or use cotangents as weights in the laplacian matrix ([2]). Defaults to False.
             verbose (bool, optional): verbose mode. Defaults to True.
             save_on_corners (bool, optional): whether to store the results on face corners or vertices. Defaults to True
+            custom_boundary (np.ndarray, optionnal): a Nx2 array containing custom coordinates for the boundary vertices. If provided, the boundary_mode argument is ignored. Defaults to None.
         
-
         Raises:
             InvalidArgumentValueError : if 'boundary_mode' is not "square" or "circle".
         """
         check_argument("boundary_mode", boundary_mode, str, ["square", "circle"])
         super().__init__("Tutte", mesh, verbose, **kwargs)
-        self._bnd_mode : TutteEmbedding.BoundaryMode = TutteEmbedding.BoundaryMode.from_string(boundary_mode)
+        self._custom_bnd : np.ndarray = kwargs.get("custom_boundary", None)
+        self._use_cotan : bool = use_cotan
+        if self._custom_bnd is None:
+            self._bnd_mode = TutteEmbedding.BoundaryMode.from_string(boundary_mode)
+        else:
+            self._bnd_mode = TutteEmbedding.BoundaryMode.CUSTOM
 
     def run(self) :
         if euler_characteristic(self.mesh)!=1:
             raise Exception("Mesh is not a topological disk. Cannot run parametrization.")
 
         Ubnd,Vbnd = self._initialize_boundary(self._bnd_mode)
 
-        lap = operators.laplacian(self.mesh, cotan=False)
+        lap = operators.laplacian(self.mesh, cotan=self._use_cotan)
         freeInds = self.mesh.interior_vertices
         bndInds, _ = extract_border_cycle(self.mesh)
 
         LI = lap[freeInds, :][:, freeInds]
         LB = lap[freeInds, :][:, bndInds]
 
         U = linalg.spsolve(LI, -LB.dot(Ubnd))
@@ -85,15 +95,17 @@
                 self.uvs[v] = Vec(U[i], V[i])
             for i,v in enumerate(bndInds):
                 self.uvs[v] = Vec(Ubnd[i], Vbnd[i])
 
     def _initialize_boundary(self, boundary_mode):
         n = len(self.mesh.boundary_vertices)
         U, V = np.zeros(n), np.zeros(n)
-        if boundary_mode == TutteEmbedding.BoundaryMode.CIRCLE:
+        if boundary_mode == TutteEmbedding.BoundaryMode.CUSTOM:
+            U,V = self._custom_bnd[:,0], self._custom_bnd[:,1]
+        elif boundary_mode == TutteEmbedding.BoundaryMode.CIRCLE:
             for i in range(n):
                 rt = cmath.rect(1., 2*pi*i/n)
                 U[i] = rt.real
                 V[i] = rt.imag
         elif boundary_mode == TutteEmbedding.BoundaryMode.SQUARE:
             corners = [0, n//4, n//2, (3*n)//4]
             U[corners[0]], V[corners[0]] = 0,0
```

### Comparing `mouette-1.1.2/mouette/processing/paths.py` & `mouette-1.1.3/mouette/processing/paths.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/processing/trees/base.py` & `mouette-1.1.3/mouette/processing/trees/base.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/processing/trees/cell_sp.py` & `mouette-1.1.3/mouette/processing/trees/cell_sp.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/processing/trees/edge_sp.py` & `mouette-1.1.3/mouette/processing/trees/edge_sp.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/processing/trees/face_sp.py` & `mouette-1.1.3/mouette/processing/trees/face_sp.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/utils/argument_check.py` & `mouette-1.1.3/mouette/utils/argument_check.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/utils/iterators.py` & `mouette-1.1.3/mouette/utils/iterators.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/utils/maths.py` & `mouette-1.1.3/mouette/utils/maths.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/utils/priority_queue.py` & `mouette-1.1.3/mouette/utils/priority_queue.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/utils/unionfind.py` & `mouette-1.1.3/mouette/utils/unionfind.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette/utils/utilities.py` & `mouette-1.1.3/mouette/utils/utilities.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/mouette.egg-info/PKG-INFO` & `mouette-1.1.3/mouette.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mouette
-Version: 1.1.2
+Version: 1.1.3
 Summary: Mesh, Tools and Geometry Processing
 Home-page: https://github.com/GCoiffier/mouette
 Author: GCoiffier
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mouette-1.1.2/mouette.egg-info/SOURCES.txt` & `mouette-1.1.3/mouette.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/pyproject.toml` & `mouette-1.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   "osqp"
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mouette"
-version = "1.0.5"
+version = "1.1.3"
 authors = [
   { name="Guillaume Coiffier" },
 ]
 description = "Geometry Processing and mesh handling in python"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `mouette-1.1.2/setup.py` & `mouette-1.1.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file_handle:
     long_description = file_handle.read()
 
 setuptools.setup(
     name="mouette",
-    version='1.1.2',
+    version='1.1.3',
     author="GCoiffier",
     description="Mesh, Tools and Geometry Processing",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/GCoiffier/mouette",
     license="MIT",
     packages=setuptools.find_packages(),
```

### Comparing `mouette-1.1.2/tests/data/circle.mesh` & `mouette-1.1.3/tests/data/circle.mesh`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/data/cube86.mesh` & `mouette-1.1.3/tests/data/cube86.mesh`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/data/feature2.obj` & `mouette-1.1.3/tests/data/feature2.obj`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/data/half_sphere1.obj` & `mouette-1.1.3/tests/data/half_sphere1.obj`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/data/join.tet` & `mouette-1.1.3/tests/data/join.tet`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/data/p01.mesh` & `mouette-1.1.3/tests/data/p01.mesh`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/data/pointclouds.py` & `mouette-1.1.3/tests/data/pointclouds.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/data/pointy.obj` & `mouette-1.1.3/tests/data/pointy.obj`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/data/polylines.py` & `mouette-1.1.3/tests/data/polylines.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/data/quad_split2.geogram_ascii` & `mouette-1.1.3/tests/data/quad_split2.geogram_ascii`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/data/spline03.mesh` & `mouette-1.1.3/tests/data/spline03.mesh`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/data/surfaces.py` & `mouette-1.1.3/tests/data/surfaces.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/data/two_pieces.obj` & `mouette-1.1.3/tests/data/two_pieces.obj`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/data/uv_sphere_nopoles_quad.obj` & `mouette-1.1.3/tests/data/uv_sphere_nopoles_quad.obj`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/data/volumes.py` & `mouette-1.1.3/tests/data/volumes.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/test_attributes.py` & `mouette-1.1.3/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/test_features.py` & `mouette-1.1.3/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/test_ff_surface.py` & `mouette-1.1.3/tests/test_ff_surface.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/test_ff_volumes.py` & `mouette-1.1.3/tests/test_ff_volumes.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/test_geometry.py` & `mouette-1.1.3/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/test_levenberg_marquardt.py` & `mouette-1.1.3/tests/test_levenberg_marquardt.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/test_maths.py` & `mouette-1.1.3/tests/test_maths.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/test_operators.py` & `mouette-1.1.3/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/test_param.py` & `mouette-1.1.3/tests/test_param.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/test_procedural.py` & `mouette-1.1.3/tests/test_procedural.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/test_quantities.py` & `mouette-1.1.3/tests/test_quantities.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/test_surfaces.py` & `mouette-1.1.3/tests/test_surfaces.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/test_tree.py` & `mouette-1.1.3/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/test_utils.py` & `mouette-1.1.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/test_vec.py` & `mouette-1.1.3/tests/test_vec.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/test_volumes.py` & `mouette-1.1.3/tests/test_volumes.py`

 * *Files identical despite different names*

### Comparing `mouette-1.1.2/tests/utils.py` & `mouette-1.1.3/tests/utils.py`

 * *Files identical despite different names*

