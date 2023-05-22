# Comparing `tmp/rasterio-1.3b2.tar.gz` & `tmp/rasterio-1.3b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasterio-1.3b2.tar", last modified: Wed Jun 22 15:41:06 2022, max compression
+gzip compressed data, was "rasterio-1.3b3.tar", last modified: Mon Jun 27 23:34:46 2022, max compression
```

## Comparing `rasterio-1.3b2.tar` & `rasterio-1.3b3.tar`

### file list

```diff
@@ -1,318 +1,318 @@
-drwxrwxr-x   0 root         (0) root         (0)        0 2022-06-22 15:41:06.328488 rasterio-1.3b2/
--rw-rw-r--   0 root         (0) root         (0)     1713 2021-11-03 20:50:17.000000 rasterio-1.3b2/AUTHORS.txt
--rw-rw-r--   0 root         (0) root         (0)    80366 2022-06-22 14:19:46.000000 rasterio-1.3b2/CHANGES.txt
--rw-rw-r--   0 root         (0) root         (0)     1457 2021-11-03 20:50:17.000000 rasterio-1.3b2/LICENSE.txt
--rw-rw-r--   0 root         (0) root         (0)    13426 2022-06-22 15:41:06.340489 rasterio-1.3b2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    12298 2022-05-10 14:17:12.000000 rasterio-1.3b2/README.rst
--rw-rw-r--   0 root         (0) root         (0)        5 2022-06-22 15:40:54.000000 rasterio-1.3b2/VERSION.txt
-drwxrwxr-x   0 root         (0) root         (0)        0 2022-06-22 15:11:53.413522 rasterio-1.3b2/docs/
-drwxrwxr-x   0 root         (0) root         (0)        0 2022-06-22 15:11:53.421522 rasterio-1.3b2/docs/api/
--rw-rw-r--   0 root         (0) root         (0)       69 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/index.rst
--rw-rw-r--   0 root         (0) root         (0)      135 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio._base.rst
--rw-rw-r--   0 root         (0) root         (0)      132 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio._env.rst
--rw-rw-r--   0 root         (0) root         (0)      132 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio._err.rst
--rw-rw-r--   0 root         (0) root         (0)      144 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio._example.rst
--rw-rw-r--   0 root         (0) root         (0)      147 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio._features.rst
--rw-rw-r--   0 root         (0) root         (0)      165 2022-04-01 01:21:36.000000 rasterio-1.3b2/docs/api/rasterio._filepath.rst
--rw-rw-r--   0 root         (0) root         (0)      135 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio._fill.rst
--rw-rw-r--   0 root         (0) root         (0)      129 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio._io.rst
--rw-rw-r--   0 root         (0) root         (0)      162 2022-04-01 01:22:16.000000 rasterio-1.3b2/docs/api/rasterio._loading.rst
--rw-rw-r--   0 root         (0) root         (0)      168 2022-04-01 01:22:47.000000 rasterio-1.3b2/docs/api/rasterio._transform.rst
--rw-rw-r--   0 root         (0) root         (0)      135 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio._warp.rst
--rw-rw-r--   0 root         (0) root         (0)      139 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.control.rst
--rw-rw-r--   0 root         (0) root         (0)      136 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.coords.rst
--rw-rw-r--   0 root         (0) root         (0)      127 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.crs.rst
--rw-rw-r--   0 root         (0) root         (0)      139 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.drivers.rst
--rw-rw-r--   0 root         (0) root         (0)      136 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.dtypes.rst
--rw-rw-r--   0 root         (0) root         (0)      133 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.enums.rst
--rw-rw-r--   0 root         (0) root         (0)      147 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.env.rst
--rw-rw-r--   0 root         (0) root         (0)      136 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.errors.rst
--rw-rw-r--   0 root         (0) root         (0)      142 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.features.rst
--rw-rw-r--   0 root         (0) root         (0)      130 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.fill.rst
--rw-rw-r--   0 root         (0) root         (0)      144 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.io.rst
--rw-rw-r--   0 root         (0) root         (0)      130 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.mask.rst
--rw-rw-r--   0 root         (0) root         (0)      133 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.merge.rst
--rw-rw-r--   0 root         (0) root         (0)      130 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.path.rst
--rw-rw-r--   0 root         (0) root         (0)      130 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.plot.rst
--rw-rw-r--   0 root         (0) root         (0)      142 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.profiles.rst
--rw-rw-r--   0 root         (0) root         (0)      148 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rio.blocks.rst
--rw-rw-r--   0 root         (0) root         (0)      148 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rio.bounds.rst
--rw-rw-r--   0 root         (0) root         (0)      142 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rio.calc.rst
--rw-rw-r--   0 root         (0) root         (0)      142 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rio.clip.rst
--rw-rw-r--   0 root         (0) root         (0)      151 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rio.convert.rst
--rw-rw-r--   0 root         (0) root         (0)      159 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rio.edit_info.rst
--rw-rw-r--   0 root         (0) root         (0)      139 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rio.env.rst
--rw-rw-r--   0 root         (0) root         (0)      142 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rio.gcps.rst
--rw-rw-r--   0 root         (0) root         (0)      151 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rio.helpers.rst
--rw-rw-r--   0 root         (0) root         (0)      142 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rio.info.rst
--rw-rw-r--   0 root         (0) root         (0)      142 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rio.insp.rst
--rw-rw-r--   0 root         (0) root         (0)      142 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rio.main.rst
--rw-rw-r--   0 root         (0) root         (0)      142 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rio.mask.rst
--rw-rw-r--   0 root         (0) root         (0)      145 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rio.merge.rst
--rw-rw-r--   0 root         (0) root         (0)      151 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rio.options.rst
--rw-rw-r--   0 root         (0) root         (0)      154 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rio.overview.rst
--rw-rw-r--   0 root         (0) root         (0)      157 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rio.rasterize.rst
--rw-rw-r--   0 root         (0) root         (0)      136 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rio.rm.rst
--rw-rw-r--   0 root         (0) root         (0)      718 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rio.rst
--rw-rw-r--   0 root         (0) root         (0)      148 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rio.sample.rst
--rw-rw-r--   0 root         (0) root         (0)      148 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rio.shapes.rst
--rw-rw-r--   0 root         (0) root         (0)      145 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rio.stack.rst
--rw-rw-r--   0 root         (0) root         (0)      157 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rio.transform.rst
--rw-rw-r--   0 root         (0) root         (0)      142 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rio.warp.rst
--rw-rw-r--   0 root         (0) root         (0)      132 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.rpc.rst
--rw-rw-r--   0 root         (0) root         (0)      698 2022-04-01 16:18:26.000000 rasterio-1.3b2/docs/api/rasterio.rst
--rw-rw-r--   0 root         (0) root         (0)      136 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.sample.rst
--rw-rw-r--   0 root         (0) root         (0)      159 2022-04-01 01:23:16.000000 rasterio-1.3b2/docs/api/rasterio.session.rst
--rw-rw-r--   0 root         (0) root         (0)      136 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.shutil.rst
--rw-rw-r--   0 root         (0) root         (0)      133 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.tools.rst
--rw-rw-r--   0 root         (0) root         (0)      145 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.transform.rst
--rw-rw-r--   0 root         (0) root         (0)      147 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.vrt.rst
--rw-rw-r--   0 root         (0) root         (0)      130 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.warp.rst
--rw-rw-r--   0 root         (0) root         (0)      136 2022-04-01 01:06:40.000000 rasterio-1.3b2/docs/api/rasterio.windows.rst
--rw-rw-r--   0 root         (0) root         (0)    19977 2022-03-30 20:54:05.000000 rasterio-1.3b2/docs/cli.rst
--rw-rw-r--   0 root         (0) root         (0)      407 2021-12-14 22:59:41.000000 rasterio-1.3b2/docs/contributing.rst
--rw-rw-r--   0 root         (0) root         (0)     3299 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/faq.rst
--rw-rw-r--   0 root         (0) root         (0)     1644 2022-04-01 01:19:48.000000 rasterio-1.3b2/docs/index.rst
--rw-rw-r--   0 root         (0) root         (0)     4729 2021-12-14 22:59:41.000000 rasterio-1.3b2/docs/installation.rst
--rw-rw-r--   0 root         (0) root         (0)     2743 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/intro.rst
--rw-rw-r--   0 root         (0) root         (0)    11434 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/quickstart.rst
-drwxrwxr-x   0 root         (0) root         (0)        0 2022-06-22 15:11:53.421522 rasterio-1.3b2/docs/topics/
--rw-rw-r--   0 root         (0) root         (0)     3611 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/calc.rst
--rw-rw-r--   0 root         (0) root         (0)     2581 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/color.rst
--rw-rw-r--   0 root         (0) root         (0)     6216 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/concurrency.rst
--rw-rw-r--   0 root         (0) root         (0)     3347 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/configuration.rst
--rw-rw-r--   0 root         (0) root         (0)     1852 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/datasets.rst
--rw-rw-r--   0 root         (0) root         (0)      121 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/errors.rst
--rw-rw-r--   0 root         (0) root         (0)     3258 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/features.rst
--rw-rw-r--   0 root         (0) root         (0)       71 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/fillnodata.rst
--rw-rw-r--   0 root         (0) root         (0)     4688 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/georeferencing.rst
--rw-rw-r--   0 root         (0) root         (0)     3080 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/image_options.rst
--rw-rw-r--   0 root         (0) root         (0)     1054 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/image_processing.rst
--rw-rw-r--   0 root         (0) root         (0)      443 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/index.rst
--rw-rw-r--   0 root         (0) root         (0)     1728 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/masking-by-shapefile.rst
--rw-rw-r--   0 root         (0) root         (0)     9114 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/masks.rst
--rw-rw-r--   0 root         (0) root         (0)     2796 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/memory-files.rst
--rw-rw-r--   0 root         (0) root         (0)     8371 2021-12-14 22:59:41.000000 rasterio-1.3b2/docs/topics/migrating-to-v1.rst
--rw-rw-r--   0 root         (0) root         (0)     2086 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/overviews.rst
--rw-rw-r--   0 root         (0) root         (0)     3935 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/plotting.rst
--rw-rw-r--   0 root         (0) root         (0)     2307 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/profiles.rst
--rw-rw-r--   0 root         (0) root         (0)     4706 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/reading.rst
--rw-rw-r--   0 root         (0) root         (0)     8295 2022-03-30 20:54:05.000000 rasterio-1.3b2/docs/topics/reproject.rst
--rw-rw-r--   0 root         (0) root         (0)     2267 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/resampling.rst
--rw-rw-r--   0 root         (0) root         (0)    13663 2022-03-30 20:54:05.000000 rasterio-1.3b2/docs/topics/switch.rst
--rw-rw-r--   0 root         (0) root         (0)     2921 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/tags.rst
--rw-rw-r--   0 root         (0) root         (0)     4394 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/transforms.rst
--rw-rw-r--   0 root         (0) root         (0)     5870 2022-03-30 20:54:05.000000 rasterio-1.3b2/docs/topics/virtual-warping.rst
--rw-rw-r--   0 root         (0) root         (0)     1536 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/vsi.rst
--rw-rw-r--   0 root         (0) root         (0)     7412 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/windowed-rw.rst
--rw-rw-r--   0 root         (0) root         (0)     2316 2021-11-03 20:50:17.000000 rasterio-1.3b2/docs/topics/writing.rst
-drwxrwxr-x   0 root         (0) root         (0)        0 2022-06-22 15:11:53.425522 rasterio-1.3b2/examples/
--rw-rw-r--   0 root         (0) root         (0)     3259 2021-11-03 20:50:17.000000 rasterio-1.3b2/examples/async-rasterio.py
--rw-rw-r--   0 root         (0) root         (0)      761 2021-11-03 20:50:17.000000 rasterio-1.3b2/examples/decimate.py
--rw-rw-r--   0 root         (0) root         (0)      222 2021-11-03 20:50:17.000000 rasterio-1.3b2/examples/polygonize.py
--rw-rw-r--   0 root         (0) root         (0)     1869 2021-11-03 20:50:17.000000 rasterio-1.3b2/examples/rasterio_polygonize.py
--rw-rw-r--   0 root         (0) root         (0)      810 2021-11-03 20:50:17.000000 rasterio-1.3b2/examples/rasterize_geometry.py
--rw-rw-r--   0 root         (0) root         (0)     1747 2021-11-03 20:50:17.000000 rasterio-1.3b2/examples/reproject.py
--rw-rw-r--   0 root         (0) root         (0)     1154 2021-11-03 20:50:17.000000 rasterio-1.3b2/examples/sieve.py
--rw-rw-r--   0 root         (0) root         (0)     2435 2021-11-03 20:50:17.000000 rasterio-1.3b2/examples/thread_pool_executor.py
--rw-rw-r--   0 root         (0) root         (0)     1318 2021-11-03 20:50:17.000000 rasterio-1.3b2/examples/total.py
--rw-rw-r--   0 root         (0) root         (0)      333 2022-03-30 20:56:44.000000 rasterio-1.3b2/pyproject.toml
-drwxrwxr-x   0 root         (0) root         (0)        0 2022-06-22 15:11:53.425522 rasterio-1.3b2/rasterio/
--rw-rw-r--   0 root         (0) root         (0)    12728 2022-06-15 16:14:22.000000 rasterio-1.3b2/rasterio/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1277 2022-04-20 19:19:56.000000 rasterio-1.3b2/rasterio/_base.pxd
--rw-rw-r--   0 root         (0) root         (0)    47275 2022-06-22 14:18:07.000000 rasterio-1.3b2/rasterio/_base.pyx
--rw-rw-r--   0 root         (0) root         (0)      155 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/_env.pxd
--rw-rw-r--   0 root         (0) root         (0)    14589 2022-05-24 14:08:54.000000 rasterio-1.3b2/rasterio/_env.pyx
--rw-rw-r--   0 root         (0) root         (0)      294 2022-06-21 19:37:02.000000 rasterio-1.3b2/rasterio/_err.pxd
--rw-rw-r--   0 root         (0) root         (0)     4883 2022-06-22 14:18:07.000000 rasterio-1.3b2/rasterio/_err.pyx
--rw-rw-r--   0 root         (0) root         (0)      804 2022-05-24 14:08:54.000000 rasterio-1.3b2/rasterio/_example.pyx
--rw-rw-r--   0 root         (0) root         (0)     1440 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/_features.pxd
--rw-rw-r--   0 root         (0) root         (0)    26197 2022-05-24 14:08:54.000000 rasterio-1.3b2/rasterio/_features.pyx
--rw-rw-r--   0 root         (0) root         (0)      199 2022-04-13 21:33:25.000000 rasterio-1.3b2/rasterio/_filepath.pxd
--rw-rw-r--   0 root         (0) root         (0)     8293 2022-05-24 14:08:54.000000 rasterio-1.3b2/rasterio/_filepath.pyx
--rw-rw-r--   0 root         (0) root         (0)     1289 2022-05-24 14:08:54.000000 rasterio-1.3b2/rasterio/_fill.pyx
--rw-rw-r--   0 root         (0) root         (0)      972 2022-03-30 20:54:05.000000 rasterio-1.3b2/rasterio/_io.pxd
--rw-rw-r--   0 root         (0) root         (0)    83132 2022-06-15 16:14:22.000000 rasterio-1.3b2/rasterio/_io.pyx
--rw-rw-r--   0 root         (0) root         (0)     1026 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/_loading.py
--rw-rw-r--   0 root         (0) root         (0)     5117 2022-04-05 21:03:57.000000 rasterio-1.3b2/rasterio/_path.py
--rw-rw-r--   0 root         (0) root         (0)     2491 2022-04-20 23:32:49.000000 rasterio-1.3b2/rasterio/_show_versions.py
--rw-rw-r--   0 root         (0) root         (0)    11957 2022-05-24 14:08:54.000000 rasterio-1.3b2/rasterio/_transform.pyx
--rw-rw-r--   0 root         (0) root         (0)      502 2022-05-10 14:17:12.000000 rasterio-1.3b2/rasterio/_version.pxd
--rw-rw-r--   0 root         (0) root         (0)     2171 2022-05-24 14:08:54.000000 rasterio-1.3b2/rasterio/_version.pyx
--rw-rw-r--   0 root         (0) root         (0)     1901 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/_warp.pxd
--rw-rw-r--   0 root         (0) root         (0)    57632 2022-06-22 14:18:07.000000 rasterio-1.3b2/rasterio/_warp.pyx
--rw-rw-r--   0 root         (0) root         (0)     2066 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/control.py
--rw-rw-r--   0 root         (0) root         (0)     1450 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/coords.py
--rw-rw-r--   0 root         (0) root         (0)      138 2022-04-01 01:19:48.000000 rasterio-1.3b2/rasterio/crs.pxd
--rw-rw-r--   0 root         (0) root         (0)    34865 2022-05-24 14:08:54.000000 rasterio-1.3b2/rasterio/crs.pyx
--rw-rw-r--   0 root         (0) root         (0)     2274 2022-05-10 14:17:12.000000 rasterio-1.3b2/rasterio/drivers.py
--rw-rw-r--   0 root         (0) root         (0)     5891 2022-06-15 16:14:22.000000 rasterio-1.3b2/rasterio/dtypes.py
--rw-rw-r--   0 root         (0) root         (0)     5550 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/enums.py
--rw-rw-r--   0 root         (0) root         (0)    21566 2022-04-20 19:19:56.000000 rasterio-1.3b2/rasterio/env.py
--rw-rw-r--   0 root         (0) root         (0)     4458 2022-04-06 16:17:05.000000 rasterio-1.3b2/rasterio/errors.py
--rw-rw-r--   0 root         (0) root         (0)    23810 2022-06-15 16:14:22.000000 rasterio-1.3b2/rasterio/features.py
--rw-rw-r--   0 root         (0) root         (0)     2853 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/fill.py
--rw-rw-r--   0 root         (0) root         (0)    32446 2022-06-15 16:14:22.000000 rasterio-1.3b2/rasterio/gdal.pxi
--rw-rw-r--   0 root         (0) root         (0)     9059 2022-04-11 21:55:44.000000 rasterio-1.3b2/rasterio/io.py
--rw-rw-r--   0 root         (0) root         (0)     7437 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/mask.py
--rw-rw-r--   0 root         (0) root         (0)    13981 2022-05-16 17:19:28.000000 rasterio-1.3b2/rasterio/merge.py
--rw-rw-r--   0 root         (0) root         (0)      520 2022-04-05 21:03:57.000000 rasterio-1.3b2/rasterio/path.py
--rw-rw-r--   0 root         (0) root         (0)    11394 2022-03-30 20:54:05.000000 rasterio-1.3b2/rasterio/plot.py
--rw-rw-r--   0 root         (0) root         (0)     1359 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/profiles.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2022-06-22 15:11:53.413522 rasterio-1.3b2/rasterio/rio/
--rw-rw-r--   0 root         (0) root         (0)       50 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/rio/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4926 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/rio/blocks.py
--rw-rw-r--   0 root         (0) root         (0)     3883 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/rio/bounds.py
--rw-rw-r--   0 root         (0) root         (0)     7630 2022-03-30 20:54:05.000000 rasterio-1.3b2/rasterio/rio/calc.py
--rw-rw-r--   0 root         (0) root         (0)     6475 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/rio/clip.py
--rw-rw-r--   0 root         (0) root         (0)     3395 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/rio/convert.py
--rw-rw-r--   0 root         (0) root         (0)     9165 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/rio/edit_info.py
--rw-rw-r--   0 root         (0) root         (0)     1316 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/rio/env.py
--rw-rw-r--   0 root         (0) root         (0)     3711 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/rio/gcps.py
--rw-rw-r--   0 root         (0) root         (0)     3598 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/rio/helpers.py
--rw-rw-r--   0 root         (0) root         (0)     5321 2022-04-21 21:28:34.000000 rasterio-1.3b2/rasterio/rio/info.py
--rw-rw-r--   0 root         (0) root         (0)     2790 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/rio/insp.py
--rw-rw-r--   0 root         (0) root         (0)     3335 2022-04-20 23:32:49.000000 rasterio-1.3b2/rasterio/rio/main.py
--rw-rw-r--   0 root         (0) root         (0)     4744 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/rio/mask.py
--rw-rw-r--   0 root         (0) root         (0)     2531 2022-05-02 14:22:13.000000 rasterio-1.3b2/rasterio/rio/merge.py
--rw-rw-r--   0 root         (0) root         (0)    12074 2022-04-14 22:54:19.000000 rasterio-1.3b2/rasterio/rio/options.py
--rw-rw-r--   0 root         (0) root         (0)     4865 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/rio/overview.py
--rw-rw-r--   0 root         (0) root         (0)    10105 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/rio/rasterize.py
--rw-rw-r--   0 root         (0) root         (0)      946 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/rio/rm.py
--rw-rw-r--   0 root         (0) root         (0)     2526 2022-04-06 16:17:05.000000 rasterio-1.3b2/rasterio/rio/sample.py
--rw-rw-r--   0 root         (0) root         (0)     4405 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/rio/shapes.py
--rw-rw-r--   0 root         (0) root         (0)     3959 2021-11-03 20:50:17.000000 rasterio-1.3b2/rasterio/rio/stack.py
--rw-rw-r--   0 root         (0) root         (0)     1901 2022-04-06 16:17:05.000000 rasterio-1.3b2/rasterio/rio/transform.py
--rw-rw-r--   0 root         (0) root         (0)    15036 2022-04-15 17:31:35.000000 rasterio-1.3b2/rasterio/rio/warp.py
--rw-rw-r--   0 root         (0) root         (0)     4202 2022-04-08 17:51:58.000000 rasterio-1.3b2/rasterio/rpc.py
--rw-rw-r--   0 root         (0) root         (0)     2205 2022-04-11 21:55:44.000000 rasterio-1.3b2/rasterio/sample.py
--rw-rw-r--   0 root         (0) root         (0)    17818 2022-04-05 21:03:57.000000 rasterio-1.3b2/rasterio/session.py
--rw-rw-r--   0 root         (0) root         (0)     7291 2022-05-24 14:08:54.000000 rasterio-1.3b2/rasterio/shutil.pyx
--rw-rw-r--   0 root         (0) root         (0)     2289 2021-12-14 22:59:41.000000 rasterio-1.3b2/rasterio/tools.py
--rw-rw-r--   0 root         (0) root         (0)    17868 2022-04-08 17:51:58.000000 rasterio-1.3b2/rasterio/transform.py
--rw-rw-r--   0 root         (0) root         (0)    10723 2022-04-13 21:32:58.000000 rasterio-1.3b2/rasterio/vrt.py
--rw-rw-r--   0 root         (0) root         (0)    20433 2022-05-10 14:17:12.000000 rasterio-1.3b2/rasterio/warp.py
--rw-rw-r--   0 root         (0) root         (0)    21922 2022-06-22 14:18:07.000000 rasterio-1.3b2/rasterio/windows.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2022-06-22 15:41:06.336488 rasterio-1.3b2/rasterio.egg-info/
--rw-rw-r--   0 root         (0) root         (0)    13426 2022-06-22 15:41:06.000000 rasterio-1.3b2/rasterio.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     7499 2022-06-22 15:41:06.000000 rasterio-1.3b2/rasterio.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2022-06-22 15:41:06.000000 rasterio-1.3b2/rasterio.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)      761 2022-06-22 15:41:06.000000 rasterio-1.3b2/rasterio.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2022-05-09 21:49:31.000000 rasterio-1.3b2/rasterio.egg-info/not-zip-safe
--rw-rw-r--   0 root         (0) root         (0)      433 2022-06-22 15:41:06.000000 rasterio-1.3b2/rasterio.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)        9 2022-06-22 15:41:06.000000 rasterio-1.3b2/rasterio.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)     1216 2022-06-22 15:41:06.344488 rasterio-1.3b2/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)    10873 2022-05-10 14:17:12.000000 rasterio-1.3b2/setup.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2022-06-22 15:11:53.437522 rasterio-1.3b2/tests/
--rw-rw-r--   0 root         (0) root         (0)      719 2021-12-14 22:59:41.000000 rasterio-1.3b2/tests/README.rst
--rw-rw-r--   0 root         (0) root         (0)        0 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    15498 2022-06-15 16:14:22.000000 rasterio-1.3b2/tests/conftest.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2022-06-22 15:11:53.437522 rasterio-1.3b2/tests/data/
--rw-rw-r--   0 root         (0) root         (0)      526 2021-12-14 22:59:41.000000 rasterio-1.3b2/tests/data/README.rst
--rw-rw-r--   0 root         (0) root         (0)     3663 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/rangehttpserver.py
--rw-rw-r--   0 root         (0) root         (0)     4366 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test__env.py
--rw-rw-r--   0 root         (0) root         (0)      755 2022-04-20 19:19:56.000000 rasterio-1.3b2/tests/test__version.py
--rw-rw-r--   0 root         (0) root         (0)      332 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_band.py
--rw-rw-r--   0 root         (0) root         (0)     5539 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_band_masks.py
--rw-rw-r--   0 root         (0) root         (0)     8097 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_blocks.py
--rw-rw-r--   0 root         (0) root         (0)     7613 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_boundless_read.py
--rw-rw-r--   0 root         (0) root         (0)     1767 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_checksum.py
--rw-rw-r--   0 root         (0) root         (0)      562 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_cli_main.py
--rw-rw-r--   0 root         (0) root         (0)     3062 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_colorinterp.py
--rw-rw-r--   0 root         (0) root         (0)     1009 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_colormap.py
--rw-rw-r--   0 root         (0) root         (0)     2840 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_complex_dtypes.py
--rw-rw-r--   0 root         (0) root         (0)     1378 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_coords.py
--rw-rw-r--   0 root         (0) root         (0)      821 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_creation_options.py
--rw-rw-r--   0 root         (0) root         (0)    22013 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_crs.py
--rw-rw-r--   0 root         (0) root         (0)      344 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_data_paths.py
--rw-rw-r--   0 root         (0) root         (0)     2819 2022-04-20 23:37:58.000000 rasterio-1.3b2/tests/test_dataset.py
--rw-rw-r--   0 root         (0) root         (0)     6509 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_dataset_mask.py
--rw-rw-r--   0 root         (0) root         (0)     2058 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_dataset_rw.py
--rw-rw-r--   0 root         (0) root         (0)      432 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_deprecated.py
--rw-rw-r--   0 root         (0) root         (0)     1018 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_descriptions.py
--rw-rw-r--   0 root         (0) root         (0)     1413 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_driver_management.py
--rw-rw-r--   0 root         (0) root         (0)      291 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_driver_policy.py
--rw-rw-r--   0 root         (0) root         (0)     4422 2022-06-15 16:14:22.000000 rasterio-1.3b2/tests/test_dtypes.py
--rw-rw-r--   0 root         (0) root         (0)      508 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_enums.py
--rw-rw-r--   0 root         (0) root         (0)    30861 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_env.py
--rw-rw-r--   0 root         (0) root         (0)     2662 2022-06-22 14:18:07.000000 rasterio-1.3b2/tests/test_err.py
--rw-rw-r--   0 root         (0) root         (0)    37839 2022-06-15 16:14:22.000000 rasterio-1.3b2/tests/test_features.py
--rw-rw-r--   0 root         (0) root         (0)     6102 2022-03-30 20:54:05.000000 rasterio-1.3b2/tests/test_filepath.py
--rw-rw-r--   0 root         (0) root         (0)     1111 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_fillnodata.py
--rw-rw-r--   0 root         (0) root         (0)     4712 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_gcps.py
--rw-rw-r--   0 root         (0) root         (0)     3462 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_gdal_raster_io.py
--rw-rw-r--   0 root         (0) root         (0)     1937 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_image_structure.py
--rw-rw-r--   0 root         (0) root         (0)     9043 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_indexing.py
--rw-rw-r--   0 root         (0) root         (0)     1441 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_int8.py
--rw-rw-r--   0 root         (0) root         (0)     1006 2022-04-05 17:59:03.000000 rasterio-1.3b2/tests/test_io.py
--rw-rw-r--   0 root         (0) root         (0)     3385 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_io_mixins.py
--rw-rw-r--   0 root         (0) root         (0)    11029 2022-03-30 20:54:05.000000 rasterio-1.3b2/tests/test_mask.py
--rw-rw-r--   0 root         (0) root         (0)     3335 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_mask_creation.py
--rw-rw-r--   0 root         (0) root         (0)    14670 2022-04-11 15:57:36.000000 rasterio-1.3b2/tests/test_memoryfile.py
--rw-rw-r--   0 root         (0) root         (0)     3554 2022-05-16 17:19:28.000000 rasterio-1.3b2/tests/test_merge.py
--rw-rw-r--   0 root         (0) root         (0)      859 2021-12-14 22:59:41.000000 rasterio-1.3b2/tests/test_meta.py
--rw-rw-r--   0 root         (0) root         (0)      914 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_no_georef.py
--rw-rw-r--   0 root         (0) root         (0)     2977 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_nodata.py
--rw-rw-r--   0 root         (0) root         (0)      908 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_open.py
--rw-rw-r--   0 root         (0) root         (0)      810 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_open_options.py
--rw-rw-r--   0 root         (0) root         (0)      597 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_open_overview_level.py
--rw-rw-r--   0 root         (0) root         (0)     1439 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_open_sharing.py
--rw-rw-r--   0 root         (0) root         (0)      507 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_options.py
--rw-rw-r--   0 root         (0) root         (0)     5836 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_overviews.py
--rw-rw-r--   0 root         (0) root         (0)      309 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_pad.py
--rw-rw-r--   0 root         (0) root         (0)     7364 2022-04-05 21:03:57.000000 rasterio-1.3b2/tests/test_path.py
--rw-rw-r--   0 root         (0) root         (0)     9049 2021-12-13 19:56:15.000000 rasterio-1.3b2/tests/test_plot.py
--rw-rw-r--   0 root         (0) root         (0)      659 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_png.py
--rw-rw-r--   0 root         (0) root         (0)      796 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_process_pool_executor.py
--rw-rw-r--   0 root         (0) root         (0)     2894 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_profile.py
--rw-rw-r--   0 root         (0) root         (0)    12989 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_read.py
--rw-rw-r--   0 root         (0) root         (0)     6280 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_read_boundless.py
--rw-rw-r--   0 root         (0) root         (0)     1141 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_read_dtype.py
--rw-rw-r--   0 root         (0) root         (0)     4154 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_read_resample.py
--rw-rw-r--   0 root         (0) root         (0)      720 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_reshape_image.py
--rw-rw-r--   0 root         (0) root         (0)      842 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_revolvingdoor.py
--rw-rw-r--   0 root         (0) root         (0)     4756 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_rio_blocks.py
--rw-rw-r--   0 root         (0) root         (0)     1192 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_rio_bounds.py
--rw-rw-r--   0 root         (0) root         (0)     7459 2021-12-14 22:59:41.000000 rasterio-1.3b2/tests/test_rio_calc.py
--rw-rw-r--   0 root         (0) root         (0)     5144 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_rio_clip.py
--rw-rw-r--   0 root         (0) root         (0)     6635 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_rio_convert.py
--rw-rw-r--   0 root         (0) root         (0)    14474 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_rio_edit_info.py
--rw-rw-r--   0 root         (0) root         (0)     2506 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_rio_gcp.py
--rw-rw-r--   0 root         (0) root         (0)     2093 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_rio_helpers.py
--rw-rw-r--   0 root         (0) root         (0)    12345 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_rio_info.py
--rw-rw-r--   0 root         (0) root         (0)      974 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_rio_insp.py
--rw-rw-r--   0 root         (0) root         (0)      765 2022-04-20 23:32:49.000000 rasterio-1.3b2/tests/test_rio_main.py
--rw-rw-r--   0 root         (0) root         (0)     6325 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_rio_mask.py
--rw-rw-r--   0 root         (0) root         (0)    22281 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_rio_merge.py
--rw-rw-r--   0 root         (0) root         (0)     6399 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_rio_options.py
--rw-rw-r--   0 root         (0) root         (0)     3379 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_rio_overview.py
--rw-rw-r--   0 root         (0) root         (0)    11001 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_rio_rasterize.py
--rw-rw-r--   0 root         (0) root         (0)     1267 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_rio_rm.py
--rw-rw-r--   0 root         (0) root         (0)     2011 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_rio_sample.py
--rw-rw-r--   0 root         (0) root         (0)     6751 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_rio_shapes.py
--rw-rw-r--   0 root         (0) root         (0)     2050 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_rio_stack.py
--rw-rw-r--   0 root         (0) root         (0)    22534 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_rio_warp.py
--rw-rw-r--   0 root         (0) root         (0)    10729 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_rpcs.py
--rw-rw-r--   0 root         (0) root         (0)     1634 2021-12-14 22:59:41.000000 rasterio-1.3b2/tests/test_sampling.py
--rw-rw-r--   0 root         (0) root         (0)     1595 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_scale_offset.py
--rw-rw-r--   0 root         (0) root         (0)    10965 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_session.py
--rw-rw-r--   0 root         (0) root         (0)     1163 2022-04-20 23:32:49.000000 rasterio-1.3b2/tests/test_show_versions.py
--rw-rw-r--   0 root         (0) root         (0)     4983 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_shutil.py
--rw-rw-r--   0 root         (0) root         (0)      481 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_subdatasets.py
--rw-rw-r--   0 root         (0) root         (0)     1020 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_tag_item.py
--rw-rw-r--   0 root         (0) root         (0)      468 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_tag_ns.py
--rw-rw-r--   0 root         (0) root         (0)     2461 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_tags.py
--rw-rw-r--   0 root         (0) root         (0)      806 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_thread_pool_executor.py
--rw-rw-r--   0 root         (0) root         (0)     2146 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_threading.py
--rw-rw-r--   0 root         (0) root         (0)      792 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_tools.py
--rw-rw-r--   0 root         (0) root         (0)    13468 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_transform.py
--rw-rw-r--   0 root         (0) root         (0)      875 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_units.py
--rw-rw-r--   0 root         (0) root         (0)     3536 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_update.py
--rw-rw-r--   0 root         (0) root         (0)      846 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_vrt.py
--rw-rw-r--   0 root         (0) root         (0)     1530 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_warnings.py
--rw-rw-r--   0 root         (0) root         (0)    65032 2022-06-22 14:18:07.000000 rasterio-1.3b2/tests/test_warp.py
--rw-rw-r--   0 root         (0) root         (0)     9922 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_warp_transform.py
--rw-rw-r--   0 root         (0) root         (0)    23891 2022-05-10 14:17:12.000000 rasterio-1.3b2/tests/test_warpedvrt.py
--rw-rw-r--   0 root         (0) root         (0)    21532 2022-04-11 19:18:03.000000 rasterio-1.3b2/tests/test_windows.py
--rw-rw-r--   0 root         (0) root         (0)     3847 2021-11-03 20:50:17.000000 rasterio-1.3b2/tests/test_windows_mixins.py
--rw-rw-r--   0 root         (0) root         (0)    19326 2022-06-15 16:14:22.000000 rasterio-1.3b2/tests/test_write.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 23:34:46.721561 rasterio-1.3b3/
+-rw-rw-r--   0 root         (0) root         (0)     1713 2021-11-03 20:50:17.000000 rasterio-1.3b3/AUTHORS.txt
+-rw-rw-r--   0 root         (0) root         (0)    80572 2022-06-27 19:32:45.000000 rasterio-1.3b3/CHANGES.txt
+-rw-rw-r--   0 root         (0) root         (0)     1457 2021-11-03 20:50:17.000000 rasterio-1.3b3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    13426 2022-06-27 23:34:46.721561 rasterio-1.3b3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    12298 2022-05-10 14:17:12.000000 rasterio-1.3b3/README.rst
+-rw-rw-r--   0 root         (0) root         (0)        5 2022-06-27 23:34:35.000000 rasterio-1.3b3/VERSION.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 23:34:46.677560 rasterio-1.3b3/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 23:34:46.689561 rasterio-1.3b3/docs/api/
+-rw-rw-r--   0 root         (0) root         (0)       69 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/index.rst
+-rw-rw-r--   0 root         (0) root         (0)      135 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio._base.rst
+-rw-rw-r--   0 root         (0) root         (0)      132 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio._env.rst
+-rw-rw-r--   0 root         (0) root         (0)      132 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio._err.rst
+-rw-rw-r--   0 root         (0) root         (0)      144 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio._example.rst
+-rw-rw-r--   0 root         (0) root         (0)      147 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio._features.rst
+-rw-rw-r--   0 root         (0) root         (0)      165 2022-04-01 01:21:36.000000 rasterio-1.3b3/docs/api/rasterio._filepath.rst
+-rw-rw-r--   0 root         (0) root         (0)      135 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio._fill.rst
+-rw-rw-r--   0 root         (0) root         (0)      129 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio._io.rst
+-rw-rw-r--   0 root         (0) root         (0)      162 2022-04-01 01:22:16.000000 rasterio-1.3b3/docs/api/rasterio._loading.rst
+-rw-rw-r--   0 root         (0) root         (0)      168 2022-04-01 01:22:47.000000 rasterio-1.3b3/docs/api/rasterio._transform.rst
+-rw-rw-r--   0 root         (0) root         (0)      135 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio._warp.rst
+-rw-rw-r--   0 root         (0) root         (0)      139 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.control.rst
+-rw-rw-r--   0 root         (0) root         (0)      136 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.coords.rst
+-rw-rw-r--   0 root         (0) root         (0)      127 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.crs.rst
+-rw-rw-r--   0 root         (0) root         (0)      139 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.drivers.rst
+-rw-rw-r--   0 root         (0) root         (0)      136 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.dtypes.rst
+-rw-rw-r--   0 root         (0) root         (0)      133 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.enums.rst
+-rw-rw-r--   0 root         (0) root         (0)      147 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.env.rst
+-rw-rw-r--   0 root         (0) root         (0)      136 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.errors.rst
+-rw-rw-r--   0 root         (0) root         (0)      142 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.features.rst
+-rw-rw-r--   0 root         (0) root         (0)      130 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.fill.rst
+-rw-rw-r--   0 root         (0) root         (0)      144 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.io.rst
+-rw-rw-r--   0 root         (0) root         (0)      130 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.mask.rst
+-rw-rw-r--   0 root         (0) root         (0)      133 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.merge.rst
+-rw-rw-r--   0 root         (0) root         (0)      130 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.path.rst
+-rw-rw-r--   0 root         (0) root         (0)      130 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.plot.rst
+-rw-rw-r--   0 root         (0) root         (0)      142 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.profiles.rst
+-rw-rw-r--   0 root         (0) root         (0)      148 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rio.blocks.rst
+-rw-rw-r--   0 root         (0) root         (0)      148 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rio.bounds.rst
+-rw-rw-r--   0 root         (0) root         (0)      142 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rio.calc.rst
+-rw-rw-r--   0 root         (0) root         (0)      142 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rio.clip.rst
+-rw-rw-r--   0 root         (0) root         (0)      151 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rio.convert.rst
+-rw-rw-r--   0 root         (0) root         (0)      159 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rio.edit_info.rst
+-rw-rw-r--   0 root         (0) root         (0)      139 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rio.env.rst
+-rw-rw-r--   0 root         (0) root         (0)      142 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rio.gcps.rst
+-rw-rw-r--   0 root         (0) root         (0)      151 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rio.helpers.rst
+-rw-rw-r--   0 root         (0) root         (0)      142 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rio.info.rst
+-rw-rw-r--   0 root         (0) root         (0)      142 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rio.insp.rst
+-rw-rw-r--   0 root         (0) root         (0)      142 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rio.main.rst
+-rw-rw-r--   0 root         (0) root         (0)      142 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rio.mask.rst
+-rw-rw-r--   0 root         (0) root         (0)      145 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rio.merge.rst
+-rw-rw-r--   0 root         (0) root         (0)      151 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rio.options.rst
+-rw-rw-r--   0 root         (0) root         (0)      154 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rio.overview.rst
+-rw-rw-r--   0 root         (0) root         (0)      157 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rio.rasterize.rst
+-rw-rw-r--   0 root         (0) root         (0)      136 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rio.rm.rst
+-rw-rw-r--   0 root         (0) root         (0)      718 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rio.rst
+-rw-rw-r--   0 root         (0) root         (0)      148 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rio.sample.rst
+-rw-rw-r--   0 root         (0) root         (0)      148 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rio.shapes.rst
+-rw-rw-r--   0 root         (0) root         (0)      145 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rio.stack.rst
+-rw-rw-r--   0 root         (0) root         (0)      157 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rio.transform.rst
+-rw-rw-r--   0 root         (0) root         (0)      142 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rio.warp.rst
+-rw-rw-r--   0 root         (0) root         (0)      132 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.rpc.rst
+-rw-rw-r--   0 root         (0) root         (0)      698 2022-04-01 16:18:26.000000 rasterio-1.3b3/docs/api/rasterio.rst
+-rw-rw-r--   0 root         (0) root         (0)      136 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.sample.rst
+-rw-rw-r--   0 root         (0) root         (0)      159 2022-04-01 01:23:16.000000 rasterio-1.3b3/docs/api/rasterio.session.rst
+-rw-rw-r--   0 root         (0) root         (0)      136 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.shutil.rst
+-rw-rw-r--   0 root         (0) root         (0)      133 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.tools.rst
+-rw-rw-r--   0 root         (0) root         (0)      145 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.transform.rst
+-rw-rw-r--   0 root         (0) root         (0)      147 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.vrt.rst
+-rw-rw-r--   0 root         (0) root         (0)      130 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.warp.rst
+-rw-rw-r--   0 root         (0) root         (0)      136 2022-04-01 01:06:40.000000 rasterio-1.3b3/docs/api/rasterio.windows.rst
+-rw-rw-r--   0 root         (0) root         (0)    19977 2022-03-30 20:54:05.000000 rasterio-1.3b3/docs/cli.rst
+-rw-rw-r--   0 root         (0) root         (0)      407 2021-12-14 22:59:41.000000 rasterio-1.3b3/docs/contributing.rst
+-rw-rw-r--   0 root         (0) root         (0)     3299 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/faq.rst
+-rw-rw-r--   0 root         (0) root         (0)     1644 2022-04-01 01:19:48.000000 rasterio-1.3b3/docs/index.rst
+-rw-rw-r--   0 root         (0) root         (0)     4729 2021-12-14 22:59:41.000000 rasterio-1.3b3/docs/installation.rst
+-rw-rw-r--   0 root         (0) root         (0)     2743 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/intro.rst
+-rw-rw-r--   0 root         (0) root         (0)    11434 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/quickstart.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 23:34:46.693561 rasterio-1.3b3/docs/topics/
+-rw-rw-r--   0 root         (0) root         (0)     3611 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/calc.rst
+-rw-rw-r--   0 root         (0) root         (0)     2581 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/color.rst
+-rw-rw-r--   0 root         (0) root         (0)     6216 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/concurrency.rst
+-rw-rw-r--   0 root         (0) root         (0)     3347 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/configuration.rst
+-rw-rw-r--   0 root         (0) root         (0)     1852 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/datasets.rst
+-rw-rw-r--   0 root         (0) root         (0)      121 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/errors.rst
+-rw-rw-r--   0 root         (0) root         (0)     3258 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/features.rst
+-rw-rw-r--   0 root         (0) root         (0)       71 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/fillnodata.rst
+-rw-rw-r--   0 root         (0) root         (0)     4688 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/georeferencing.rst
+-rw-rw-r--   0 root         (0) root         (0)     3080 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/image_options.rst
+-rw-rw-r--   0 root         (0) root         (0)     1054 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/image_processing.rst
+-rw-rw-r--   0 root         (0) root         (0)      443 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/index.rst
+-rw-rw-r--   0 root         (0) root         (0)     1728 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/masking-by-shapefile.rst
+-rw-rw-r--   0 root         (0) root         (0)     9114 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/masks.rst
+-rw-rw-r--   0 root         (0) root         (0)     2796 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/memory-files.rst
+-rw-rw-r--   0 root         (0) root         (0)     8371 2021-12-14 22:59:41.000000 rasterio-1.3b3/docs/topics/migrating-to-v1.rst
+-rw-rw-r--   0 root         (0) root         (0)     2086 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/overviews.rst
+-rw-rw-r--   0 root         (0) root         (0)     3935 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/plotting.rst
+-rw-rw-r--   0 root         (0) root         (0)     2307 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/profiles.rst
+-rw-rw-r--   0 root         (0) root         (0)     4706 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/reading.rst
+-rw-rw-r--   0 root         (0) root         (0)     8295 2022-03-30 20:54:05.000000 rasterio-1.3b3/docs/topics/reproject.rst
+-rw-rw-r--   0 root         (0) root         (0)     2267 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/resampling.rst
+-rw-rw-r--   0 root         (0) root         (0)    13663 2022-03-30 20:54:05.000000 rasterio-1.3b3/docs/topics/switch.rst
+-rw-rw-r--   0 root         (0) root         (0)     2921 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/tags.rst
+-rw-rw-r--   0 root         (0) root         (0)     4394 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/transforms.rst
+-rw-rw-r--   0 root         (0) root         (0)     5870 2022-03-30 20:54:05.000000 rasterio-1.3b3/docs/topics/virtual-warping.rst
+-rw-rw-r--   0 root         (0) root         (0)     1536 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/vsi.rst
+-rw-rw-r--   0 root         (0) root         (0)     7412 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/windowed-rw.rst
+-rw-rw-r--   0 root         (0) root         (0)     2316 2021-11-03 20:50:17.000000 rasterio-1.3b3/docs/topics/writing.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 23:34:46.697561 rasterio-1.3b3/examples/
+-rw-rw-r--   0 root         (0) root         (0)     3259 2021-11-03 20:50:17.000000 rasterio-1.3b3/examples/async-rasterio.py
+-rw-rw-r--   0 root         (0) root         (0)      761 2021-11-03 20:50:17.000000 rasterio-1.3b3/examples/decimate.py
+-rw-rw-r--   0 root         (0) root         (0)      222 2021-11-03 20:50:17.000000 rasterio-1.3b3/examples/polygonize.py
+-rw-rw-r--   0 root         (0) root         (0)     1869 2021-11-03 20:50:17.000000 rasterio-1.3b3/examples/rasterio_polygonize.py
+-rw-rw-r--   0 root         (0) root         (0)      810 2021-11-03 20:50:17.000000 rasterio-1.3b3/examples/rasterize_geometry.py
+-rw-rw-r--   0 root         (0) root         (0)     1747 2021-11-03 20:50:17.000000 rasterio-1.3b3/examples/reproject.py
+-rw-rw-r--   0 root         (0) root         (0)     1154 2021-11-03 20:50:17.000000 rasterio-1.3b3/examples/sieve.py
+-rw-rw-r--   0 root         (0) root         (0)     2435 2021-11-03 20:50:17.000000 rasterio-1.3b3/examples/thread_pool_executor.py
+-rw-rw-r--   0 root         (0) root         (0)     1318 2021-11-03 20:50:17.000000 rasterio-1.3b3/examples/total.py
+-rw-rw-r--   0 root         (0) root         (0)      333 2022-03-30 20:56:44.000000 rasterio-1.3b3/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 23:34:46.701561 rasterio-1.3b3/rasterio/
+-rw-rw-r--   0 root         (0) root         (0)    12728 2022-06-23 22:38:50.000000 rasterio-1.3b3/rasterio/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1165 2022-06-23 22:26:44.000000 rasterio-1.3b3/rasterio/_base.pxd
+-rw-rw-r--   0 root         (0) root         (0)    45718 2022-06-23 22:26:44.000000 rasterio-1.3b3/rasterio/_base.pyx
+-rw-rw-r--   0 root         (0) root         (0)      155 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/_env.pxd
+-rw-rw-r--   0 root         (0) root         (0)    14568 2022-06-23 22:26:44.000000 rasterio-1.3b3/rasterio/_env.pyx
+-rw-rw-r--   0 root         (0) root         (0)      294 2022-06-21 19:37:02.000000 rasterio-1.3b3/rasterio/_err.pxd
+-rw-rw-r--   0 root         (0) root         (0)     4883 2022-06-22 14:18:07.000000 rasterio-1.3b3/rasterio/_err.pyx
+-rw-rw-r--   0 root         (0) root         (0)      804 2022-05-24 14:08:54.000000 rasterio-1.3b3/rasterio/_example.pyx
+-rw-rw-r--   0 root         (0) root         (0)     1440 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/_features.pxd
+-rw-rw-r--   0 root         (0) root         (0)    26197 2022-05-24 14:08:54.000000 rasterio-1.3b3/rasterio/_features.pyx
+-rw-rw-r--   0 root         (0) root         (0)      199 2022-04-13 21:33:25.000000 rasterio-1.3b3/rasterio/_filepath.pxd
+-rw-rw-r--   0 root         (0) root         (0)     8293 2022-05-24 14:08:54.000000 rasterio-1.3b3/rasterio/_filepath.pyx
+-rw-rw-r--   0 root         (0) root         (0)     1289 2022-05-24 14:08:54.000000 rasterio-1.3b3/rasterio/_fill.pyx
+-rw-rw-r--   0 root         (0) root         (0)      972 2022-03-30 20:54:05.000000 rasterio-1.3b3/rasterio/_io.pxd
+-rw-rw-r--   0 root         (0) root         (0)    83127 2022-06-23 22:26:44.000000 rasterio-1.3b3/rasterio/_io.pyx
+-rw-rw-r--   0 root         (0) root         (0)     1026 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/_loading.py
+-rw-rw-r--   0 root         (0) root         (0)     5117 2022-04-05 21:03:57.000000 rasterio-1.3b3/rasterio/_path.py
+-rw-rw-r--   0 root         (0) root         (0)     2491 2022-04-20 23:32:49.000000 rasterio-1.3b3/rasterio/_show_versions.py
+-rw-rw-r--   0 root         (0) root         (0)    11957 2022-05-24 14:08:54.000000 rasterio-1.3b3/rasterio/_transform.pyx
+-rw-rw-r--   0 root         (0) root         (0)      502 2022-05-10 14:17:12.000000 rasterio-1.3b3/rasterio/_version.pxd
+-rw-rw-r--   0 root         (0) root         (0)     2171 2022-05-24 14:08:54.000000 rasterio-1.3b3/rasterio/_version.pyx
+-rw-rw-r--   0 root         (0) root         (0)     1901 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/_warp.pxd
+-rw-rw-r--   0 root         (0) root         (0)    56327 2022-06-23 22:26:44.000000 rasterio-1.3b3/rasterio/_warp.pyx
+-rw-rw-r--   0 root         (0) root         (0)     2066 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/control.py
+-rw-rw-r--   0 root         (0) root         (0)     1450 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/coords.py
+-rw-rw-r--   0 root         (0) root         (0)      138 2022-04-01 01:19:48.000000 rasterio-1.3b3/rasterio/crs.pxd
+-rw-rw-r--   0 root         (0) root         (0)    34951 2022-06-23 22:26:44.000000 rasterio-1.3b3/rasterio/crs.pyx
+-rw-rw-r--   0 root         (0) root         (0)     2274 2022-05-10 14:17:12.000000 rasterio-1.3b3/rasterio/drivers.py
+-rw-rw-r--   0 root         (0) root         (0)     5891 2022-06-15 16:14:22.000000 rasterio-1.3b3/rasterio/dtypes.py
+-rw-rw-r--   0 root         (0) root         (0)     5550 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/enums.py
+-rw-rw-r--   0 root         (0) root         (0)    21566 2022-04-20 19:19:56.000000 rasterio-1.3b3/rasterio/env.py
+-rw-rw-r--   0 root         (0) root         (0)     4458 2022-04-06 16:17:05.000000 rasterio-1.3b3/rasterio/errors.py
+-rw-rw-r--   0 root         (0) root         (0)    23810 2022-06-15 16:14:22.000000 rasterio-1.3b3/rasterio/features.py
+-rw-rw-r--   0 root         (0) root         (0)     2853 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/fill.py
+-rw-rw-r--   0 root         (0) root         (0)    32446 2022-06-15 16:14:22.000000 rasterio-1.3b3/rasterio/gdal.pxi
+-rw-rw-r--   0 root         (0) root         (0)     9059 2022-04-11 21:55:44.000000 rasterio-1.3b3/rasterio/io.py
+-rw-rw-r--   0 root         (0) root         (0)     7437 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/mask.py
+-rw-rw-r--   0 root         (0) root         (0)    13981 2022-05-16 17:19:28.000000 rasterio-1.3b3/rasterio/merge.py
+-rw-rw-r--   0 root         (0) root         (0)      520 2022-04-05 21:03:57.000000 rasterio-1.3b3/rasterio/path.py
+-rw-rw-r--   0 root         (0) root         (0)    11368 2022-06-23 22:26:44.000000 rasterio-1.3b3/rasterio/plot.py
+-rw-rw-r--   0 root         (0) root         (0)     1359 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/profiles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 23:34:46.677560 rasterio-1.3b3/rasterio/rio/
+-rw-rw-r--   0 root         (0) root         (0)       50 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/rio/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4926 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/rio/blocks.py
+-rw-rw-r--   0 root         (0) root         (0)     3883 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/rio/bounds.py
+-rw-rw-r--   0 root         (0) root         (0)     7630 2022-03-30 20:54:05.000000 rasterio-1.3b3/rasterio/rio/calc.py
+-rw-rw-r--   0 root         (0) root         (0)     6475 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/rio/clip.py
+-rw-rw-r--   0 root         (0) root         (0)     3395 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/rio/convert.py
+-rw-rw-r--   0 root         (0) root         (0)     9165 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/rio/edit_info.py
+-rw-rw-r--   0 root         (0) root         (0)     1316 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/rio/env.py
+-rw-rw-r--   0 root         (0) root         (0)     3711 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/rio/gcps.py
+-rw-rw-r--   0 root         (0) root         (0)     3598 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/rio/helpers.py
+-rw-rw-r--   0 root         (0) root         (0)     5321 2022-04-21 21:28:34.000000 rasterio-1.3b3/rasterio/rio/info.py
+-rw-rw-r--   0 root         (0) root         (0)     2790 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/rio/insp.py
+-rw-rw-r--   0 root         (0) root         (0)     3335 2022-04-20 23:32:49.000000 rasterio-1.3b3/rasterio/rio/main.py
+-rw-rw-r--   0 root         (0) root         (0)     4744 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/rio/mask.py
+-rw-rw-r--   0 root         (0) root         (0)     2531 2022-05-02 14:22:13.000000 rasterio-1.3b3/rasterio/rio/merge.py
+-rw-rw-r--   0 root         (0) root         (0)    12074 2022-04-14 22:54:19.000000 rasterio-1.3b3/rasterio/rio/options.py
+-rw-rw-r--   0 root         (0) root         (0)     4865 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/rio/overview.py
+-rw-rw-r--   0 root         (0) root         (0)    10105 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/rio/rasterize.py
+-rw-rw-r--   0 root         (0) root         (0)      946 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/rio/rm.py
+-rw-rw-r--   0 root         (0) root         (0)     2526 2022-04-06 16:17:05.000000 rasterio-1.3b3/rasterio/rio/sample.py
+-rw-rw-r--   0 root         (0) root         (0)     4405 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/rio/shapes.py
+-rw-rw-r--   0 root         (0) root         (0)     3959 2021-11-03 20:50:17.000000 rasterio-1.3b3/rasterio/rio/stack.py
+-rw-rw-r--   0 root         (0) root         (0)     1901 2022-04-06 16:17:05.000000 rasterio-1.3b3/rasterio/rio/transform.py
+-rw-rw-r--   0 root         (0) root         (0)    15036 2022-04-15 17:31:35.000000 rasterio-1.3b3/rasterio/rio/warp.py
+-rw-rw-r--   0 root         (0) root         (0)     4202 2022-04-08 17:51:58.000000 rasterio-1.3b3/rasterio/rpc.py
+-rw-rw-r--   0 root         (0) root         (0)     2205 2022-04-11 21:55:44.000000 rasterio-1.3b3/rasterio/sample.py
+-rw-rw-r--   0 root         (0) root         (0)    17818 2022-04-05 21:03:57.000000 rasterio-1.3b3/rasterio/session.py
+-rw-rw-r--   0 root         (0) root         (0)     7291 2022-05-24 14:08:54.000000 rasterio-1.3b3/rasterio/shutil.pyx
+-rw-rw-r--   0 root         (0) root         (0)     2289 2021-12-14 22:59:41.000000 rasterio-1.3b3/rasterio/tools.py
+-rw-rw-r--   0 root         (0) root         (0)    17868 2022-04-08 17:51:58.000000 rasterio-1.3b3/rasterio/transform.py
+-rw-rw-r--   0 root         (0) root         (0)    10723 2022-04-13 21:32:58.000000 rasterio-1.3b3/rasterio/vrt.py
+-rw-rw-r--   0 root         (0) root         (0)    20552 2022-06-23 22:26:44.000000 rasterio-1.3b3/rasterio/warp.py
+-rw-rw-r--   0 root         (0) root         (0)    21922 2022-06-22 14:18:07.000000 rasterio-1.3b3/rasterio/windows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 23:34:46.701561 rasterio-1.3b3/rasterio.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)    13426 2022-06-27 23:34:46.000000 rasterio-1.3b3/rasterio.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     7499 2022-06-27 23:34:46.000000 rasterio-1.3b3/rasterio.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2022-06-27 23:34:46.000000 rasterio-1.3b3/rasterio.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)      761 2022-06-27 23:34:46.000000 rasterio-1.3b3/rasterio.egg-info/entry_points.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2022-05-09 21:49:31.000000 rasterio-1.3b3/rasterio.egg-info/not-zip-safe
+-rw-rw-r--   0 root         (0) root         (0)      433 2022-06-27 23:34:46.000000 rasterio-1.3b3/rasterio.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)        9 2022-06-27 23:34:46.000000 rasterio-1.3b3/rasterio.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)     1216 2022-06-27 23:34:46.721561 rasterio-1.3b3/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)    10873 2022-05-10 14:17:12.000000 rasterio-1.3b3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 23:34:46.721561 rasterio-1.3b3/tests/
+-rw-rw-r--   0 root         (0) root         (0)      719 2021-12-14 22:59:41.000000 rasterio-1.3b3/tests/README.rst
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    15390 2022-06-23 22:26:44.000000 rasterio-1.3b3/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 23:34:46.721561 rasterio-1.3b3/tests/data/
+-rw-rw-r--   0 root         (0) root         (0)      526 2021-12-14 22:59:41.000000 rasterio-1.3b3/tests/data/README.rst
+-rw-rw-r--   0 root         (0) root         (0)     3663 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/rangehttpserver.py
+-rw-rw-r--   0 root         (0) root         (0)     4366 2022-05-10 14:17:12.000000 rasterio-1.3b3/tests/test__env.py
+-rw-rw-r--   0 root         (0) root         (0)      755 2022-04-20 19:19:56.000000 rasterio-1.3b3/tests/test__version.py
+-rw-rw-r--   0 root         (0) root         (0)      332 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_band.py
+-rw-rw-r--   0 root         (0) root         (0)     5539 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_band_masks.py
+-rw-rw-r--   0 root         (0) root         (0)     8097 2022-05-10 14:17:12.000000 rasterio-1.3b3/tests/test_blocks.py
+-rw-rw-r--   0 root         (0) root         (0)     7613 2022-05-10 14:17:12.000000 rasterio-1.3b3/tests/test_boundless_read.py
+-rw-rw-r--   0 root         (0) root         (0)     1767 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_checksum.py
+-rw-rw-r--   0 root         (0) root         (0)      562 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_cli_main.py
+-rw-rw-r--   0 root         (0) root         (0)     3062 2022-05-10 14:17:12.000000 rasterio-1.3b3/tests/test_colorinterp.py
+-rw-rw-r--   0 root         (0) root         (0)     1009 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_colormap.py
+-rw-rw-r--   0 root         (0) root         (0)     2840 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_complex_dtypes.py
+-rw-rw-r--   0 root         (0) root         (0)     1378 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_coords.py
+-rw-rw-r--   0 root         (0) root         (0)      821 2022-05-10 14:17:12.000000 rasterio-1.3b3/tests/test_creation_options.py
+-rw-rw-r--   0 root         (0) root         (0)    21855 2022-06-23 22:26:44.000000 rasterio-1.3b3/tests/test_crs.py
+-rw-rw-r--   0 root         (0) root         (0)      344 2022-05-10 14:17:12.000000 rasterio-1.3b3/tests/test_data_paths.py
+-rw-rw-r--   0 root         (0) root         (0)     2819 2022-04-20 23:37:58.000000 rasterio-1.3b3/tests/test_dataset.py
+-rw-rw-r--   0 root         (0) root         (0)     6509 2022-05-10 14:17:12.000000 rasterio-1.3b3/tests/test_dataset_mask.py
+-rw-rw-r--   0 root         (0) root         (0)     2058 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_dataset_rw.py
+-rw-rw-r--   0 root         (0) root         (0)      432 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_deprecated.py
+-rw-rw-r--   0 root         (0) root         (0)     1018 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_descriptions.py
+-rw-rw-r--   0 root         (0) root         (0)     1413 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_driver_management.py
+-rw-rw-r--   0 root         (0) root         (0)      291 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_driver_policy.py
+-rw-rw-r--   0 root         (0) root         (0)     4422 2022-06-15 16:14:22.000000 rasterio-1.3b3/tests/test_dtypes.py
+-rw-rw-r--   0 root         (0) root         (0)      508 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_enums.py
+-rw-rw-r--   0 root         (0) root         (0)    30861 2022-05-10 14:17:12.000000 rasterio-1.3b3/tests/test_env.py
+-rw-rw-r--   0 root         (0) root         (0)     2662 2022-06-22 14:18:07.000000 rasterio-1.3b3/tests/test_err.py
+-rw-rw-r--   0 root         (0) root         (0)    37839 2022-06-15 16:14:22.000000 rasterio-1.3b3/tests/test_features.py
+-rw-rw-r--   0 root         (0) root         (0)     6102 2022-03-30 20:54:05.000000 rasterio-1.3b3/tests/test_filepath.py
+-rw-rw-r--   0 root         (0) root         (0)     1111 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_fillnodata.py
+-rw-rw-r--   0 root         (0) root         (0)     4712 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_gcps.py
+-rw-rw-r--   0 root         (0) root         (0)     3462 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_gdal_raster_io.py
+-rw-rw-r--   0 root         (0) root         (0)     1937 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_image_structure.py
+-rw-rw-r--   0 root         (0) root         (0)     9043 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_indexing.py
+-rw-rw-r--   0 root         (0) root         (0)     1441 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_int8.py
+-rw-rw-r--   0 root         (0) root         (0)     1006 2022-04-05 17:59:03.000000 rasterio-1.3b3/tests/test_io.py
+-rw-rw-r--   0 root         (0) root         (0)     3385 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_io_mixins.py
+-rw-rw-r--   0 root         (0) root         (0)    11029 2022-03-30 20:54:05.000000 rasterio-1.3b3/tests/test_mask.py
+-rw-rw-r--   0 root         (0) root         (0)     3335 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_mask_creation.py
+-rw-rw-r--   0 root         (0) root         (0)    14670 2022-04-11 15:57:36.000000 rasterio-1.3b3/tests/test_memoryfile.py
+-rw-rw-r--   0 root         (0) root         (0)     3554 2022-05-16 17:19:28.000000 rasterio-1.3b3/tests/test_merge.py
+-rw-rw-r--   0 root         (0) root         (0)      859 2021-12-14 22:59:41.000000 rasterio-1.3b3/tests/test_meta.py
+-rw-rw-r--   0 root         (0) root         (0)      914 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_no_georef.py
+-rw-rw-r--   0 root         (0) root         (0)     2977 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_nodata.py
+-rw-rw-r--   0 root         (0) root         (0)      908 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_open.py
+-rw-rw-r--   0 root         (0) root         (0)      810 2022-05-10 14:17:12.000000 rasterio-1.3b3/tests/test_open_options.py
+-rw-rw-r--   0 root         (0) root         (0)      597 2022-05-10 14:17:12.000000 rasterio-1.3b3/tests/test_open_overview_level.py
+-rw-rw-r--   0 root         (0) root         (0)     1439 2022-05-10 14:17:12.000000 rasterio-1.3b3/tests/test_open_sharing.py
+-rw-rw-r--   0 root         (0) root         (0)      507 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_options.py
+-rw-rw-r--   0 root         (0) root         (0)     5836 2022-05-10 14:17:12.000000 rasterio-1.3b3/tests/test_overviews.py
+-rw-rw-r--   0 root         (0) root         (0)      309 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_pad.py
+-rw-rw-r--   0 root         (0) root         (0)     7364 2022-04-05 21:03:57.000000 rasterio-1.3b3/tests/test_path.py
+-rw-rw-r--   0 root         (0) root         (0)     9049 2021-12-13 19:56:15.000000 rasterio-1.3b3/tests/test_plot.py
+-rw-rw-r--   0 root         (0) root         (0)      659 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_png.py
+-rw-rw-r--   0 root         (0) root         (0)      796 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_process_pool_executor.py
+-rw-rw-r--   0 root         (0) root         (0)     2894 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_profile.py
+-rw-rw-r--   0 root         (0) root         (0)    12989 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_read.py
+-rw-rw-r--   0 root         (0) root         (0)     6280 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_read_boundless.py
+-rw-rw-r--   0 root         (0) root         (0)     1141 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_read_dtype.py
+-rw-rw-r--   0 root         (0) root         (0)     4154 2022-05-10 14:17:12.000000 rasterio-1.3b3/tests/test_read_resample.py
+-rw-rw-r--   0 root         (0) root         (0)      720 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_reshape_image.py
+-rw-rw-r--   0 root         (0) root         (0)      842 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_revolvingdoor.py
+-rw-rw-r--   0 root         (0) root         (0)     4756 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_rio_blocks.py
+-rw-rw-r--   0 root         (0) root         (0)     1192 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_rio_bounds.py
+-rw-rw-r--   0 root         (0) root         (0)     7459 2021-12-14 22:59:41.000000 rasterio-1.3b3/tests/test_rio_calc.py
+-rw-rw-r--   0 root         (0) root         (0)     5144 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_rio_clip.py
+-rw-rw-r--   0 root         (0) root         (0)     6635 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_rio_convert.py
+-rw-rw-r--   0 root         (0) root         (0)    14474 2022-05-10 14:17:12.000000 rasterio-1.3b3/tests/test_rio_edit_info.py
+-rw-rw-r--   0 root         (0) root         (0)     2506 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_rio_gcp.py
+-rw-rw-r--   0 root         (0) root         (0)     2093 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_rio_helpers.py
+-rw-rw-r--   0 root         (0) root         (0)    12345 2022-05-10 14:17:12.000000 rasterio-1.3b3/tests/test_rio_info.py
+-rw-rw-r--   0 root         (0) root         (0)      974 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_rio_insp.py
+-rw-rw-r--   0 root         (0) root         (0)      765 2022-04-20 23:32:49.000000 rasterio-1.3b3/tests/test_rio_main.py
+-rw-rw-r--   0 root         (0) root         (0)     6325 2022-05-10 14:17:12.000000 rasterio-1.3b3/tests/test_rio_mask.py
+-rw-rw-r--   0 root         (0) root         (0)    22281 2022-05-10 14:17:12.000000 rasterio-1.3b3/tests/test_rio_merge.py
+-rw-rw-r--   0 root         (0) root         (0)     6399 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_rio_options.py
+-rw-rw-r--   0 root         (0) root         (0)     3379 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_rio_overview.py
+-rw-rw-r--   0 root         (0) root         (0)    11001 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_rio_rasterize.py
+-rw-rw-r--   0 root         (0) root         (0)     1267 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_rio_rm.py
+-rw-rw-r--   0 root         (0) root         (0)     2011 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_rio_sample.py
+-rw-rw-r--   0 root         (0) root         (0)     6751 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_rio_shapes.py
+-rw-rw-r--   0 root         (0) root         (0)     2050 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_rio_stack.py
+-rw-rw-r--   0 root         (0) root         (0)    22534 2022-05-10 14:17:12.000000 rasterio-1.3b3/tests/test_rio_warp.py
+-rw-rw-r--   0 root         (0) root         (0)    10729 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_rpcs.py
+-rw-rw-r--   0 root         (0) root         (0)     1634 2021-12-14 22:59:41.000000 rasterio-1.3b3/tests/test_sampling.py
+-rw-rw-r--   0 root         (0) root         (0)     1595 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_scale_offset.py
+-rw-rw-r--   0 root         (0) root         (0)    10965 2022-05-10 14:17:12.000000 rasterio-1.3b3/tests/test_session.py
+-rw-rw-r--   0 root         (0) root         (0)     1163 2022-04-20 23:32:49.000000 rasterio-1.3b3/tests/test_show_versions.py
+-rw-rw-r--   0 root         (0) root         (0)     4983 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_shutil.py
+-rw-rw-r--   0 root         (0) root         (0)      481 2022-05-10 14:17:12.000000 rasterio-1.3b3/tests/test_subdatasets.py
+-rw-rw-r--   0 root         (0) root         (0)     1020 2022-05-10 14:17:12.000000 rasterio-1.3b3/tests/test_tag_item.py
+-rw-rw-r--   0 root         (0) root         (0)      468 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_tag_ns.py
+-rw-rw-r--   0 root         (0) root         (0)     2461 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_tags.py
+-rw-rw-r--   0 root         (0) root         (0)      806 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_thread_pool_executor.py
+-rw-rw-r--   0 root         (0) root         (0)     2146 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_threading.py
+-rw-rw-r--   0 root         (0) root         (0)      792 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_tools.py
+-rw-rw-r--   0 root         (0) root         (0)    13468 2022-05-10 14:17:12.000000 rasterio-1.3b3/tests/test_transform.py
+-rw-rw-r--   0 root         (0) root         (0)      875 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_units.py
+-rw-rw-r--   0 root         (0) root         (0)     3135 2022-06-23 22:26:44.000000 rasterio-1.3b3/tests/test_update.py
+-rw-rw-r--   0 root         (0) root         (0)      846 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_vrt.py
+-rw-rw-r--   0 root         (0) root         (0)     1530 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_warnings.py
+-rw-rw-r--   0 root         (0) root         (0)    65032 2022-06-23 22:26:44.000000 rasterio-1.3b3/tests/test_warp.py
+-rw-rw-r--   0 root         (0) root         (0)     9922 2022-05-10 14:17:12.000000 rasterio-1.3b3/tests/test_warp_transform.py
+-rw-rw-r--   0 root         (0) root         (0)    23891 2022-05-10 14:17:12.000000 rasterio-1.3b3/tests/test_warpedvrt.py
+-rw-rw-r--   0 root         (0) root         (0)    21532 2022-04-11 19:18:03.000000 rasterio-1.3b3/tests/test_windows.py
+-rw-rw-r--   0 root         (0) root         (0)     3847 2021-11-03 20:50:17.000000 rasterio-1.3b3/tests/test_windows_mixins.py
+-rw-rw-r--   0 root         (0) root         (0)    19292 2022-06-23 22:26:44.000000 rasterio-1.3b3/tests/test_write.py
```

### Comparing `rasterio-1.3b2/AUTHORS.txt` & `rasterio-1.3b3/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/CHANGES.txt` & `rasterio-1.3b3/CHANGES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 Changes
 =======
 
 1.3.0 (TBD)
 -----------
 
+1.3b3 (2022-06-27)
+------------------
+
+Bug fixes:
+
+- A bottleneck in construction of non-EPSG CRS objects has been fixed (#2488).
+- The last runtime checks for GDAL version 3.1+ have been removed (#2463).
+
 1.3b2 (2022-06-22)
 ------------------
 
 Changes:
 
 - The merge tool has new "sum" and "count" merge methods (#2457).
```

### Comparing `rasterio-1.3b2/LICENSE.txt` & `rasterio-1.3b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/PKG-INFO` & `rasterio-1.3b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasterio
-Version: 1.3b2
+Version: 1.3b3
 Summary: Fast and direct raster I/O for use with Numpy and SciPy
 Home-page: https://github.com/rasterio/rasterio
 Author: Sean Gillies
 Author-email: sean@mapbox.com
 License: BSD
 Keywords: raster gdal
 Platform: UNKNOWN
```

### Comparing `rasterio-1.3b2/README.rst` & `rasterio-1.3b3/README.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/api/rasterio.rio.rst` & `rasterio-1.3b3/docs/api/rasterio.rio.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/api/rasterio.rst` & `rasterio-1.3b3/docs/api/rasterio.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/cli.rst` & `rasterio-1.3b3/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/faq.rst` & `rasterio-1.3b3/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/index.rst` & `rasterio-1.3b3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/installation.rst` & `rasterio-1.3b3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/intro.rst` & `rasterio-1.3b3/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/quickstart.rst` & `rasterio-1.3b3/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/calc.rst` & `rasterio-1.3b3/docs/topics/calc.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/color.rst` & `rasterio-1.3b3/docs/topics/color.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/concurrency.rst` & `rasterio-1.3b3/docs/topics/concurrency.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/configuration.rst` & `rasterio-1.3b3/docs/topics/configuration.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/datasets.rst` & `rasterio-1.3b3/docs/topics/datasets.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/features.rst` & `rasterio-1.3b3/docs/topics/features.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/georeferencing.rst` & `rasterio-1.3b3/docs/topics/georeferencing.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/image_options.rst` & `rasterio-1.3b3/docs/topics/image_options.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/image_processing.rst` & `rasterio-1.3b3/docs/topics/image_processing.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/masking-by-shapefile.rst` & `rasterio-1.3b3/docs/topics/masking-by-shapefile.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/masks.rst` & `rasterio-1.3b3/docs/topics/masks.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/memory-files.rst` & `rasterio-1.3b3/docs/topics/memory-files.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/migrating-to-v1.rst` & `rasterio-1.3b3/docs/topics/migrating-to-v1.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/overviews.rst` & `rasterio-1.3b3/docs/topics/overviews.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/plotting.rst` & `rasterio-1.3b3/docs/topics/plotting.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/profiles.rst` & `rasterio-1.3b3/docs/topics/profiles.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/reading.rst` & `rasterio-1.3b3/docs/topics/reading.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/reproject.rst` & `rasterio-1.3b3/docs/topics/reproject.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/resampling.rst` & `rasterio-1.3b3/docs/topics/resampling.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/switch.rst` & `rasterio-1.3b3/docs/topics/switch.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/tags.rst` & `rasterio-1.3b3/docs/topics/tags.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/transforms.rst` & `rasterio-1.3b3/docs/topics/transforms.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/virtual-warping.rst` & `rasterio-1.3b3/docs/topics/virtual-warping.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/vsi.rst` & `rasterio-1.3b3/docs/topics/vsi.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/windowed-rw.rst` & `rasterio-1.3b3/docs/topics/windowed-rw.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/docs/topics/writing.rst` & `rasterio-1.3b3/docs/topics/writing.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/examples/async-rasterio.py` & `rasterio-1.3b3/examples/async-rasterio.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/examples/decimate.py` & `rasterio-1.3b3/examples/decimate.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/examples/rasterio_polygonize.py` & `rasterio-1.3b3/examples/rasterio_polygonize.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/examples/rasterize_geometry.py` & `rasterio-1.3b3/examples/rasterize_geometry.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/examples/reproject.py` & `rasterio-1.3b3/examples/reproject.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/examples/sieve.py` & `rasterio-1.3b3/examples/sieve.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/examples/thread_pool_executor.py` & `rasterio-1.3b3/examples/thread_pool_executor.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/examples/total.py` & `rasterio-1.3b3/examples/total.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/__init__.py` & `rasterio-1.3b3/rasterio/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         have_vsi_plugin = True
     except ImportError:
         class FilePath:
             pass
         have_vsi_plugin = False
 
 __all__ = ['band', 'open', 'pad', 'Env', 'CRS']
-__version__ = "1.3b2"
+__version__ = "1.3b3"
 __gdal_version__ = gdal_version()
 __proj_version__ = ".".join([str(version) for version in get_proj_version()])
 __geos_version__ = ".".join([str(version) for version in get_geos_version()])
 
 # Rasterio attaches NullHandler to the 'rasterio' logger and its
 # descendents. See
 # https://docs.python.org/2/howto/logging.html#configuring-logging-for-a-library
```

### Comparing `rasterio-1.3b2/rasterio/_base.pxd` & `rasterio-1.3b3/rasterio/_base.pxd`

 * *Files 4% similar despite different names*

```diff
@@ -28,11 +28,10 @@
     cdef public object _rpcs
     cdef public object _env
     cdef GDALDatasetH handle(self) except NULL
     cdef GDALRasterBandH band(self, int bidx) except NULL
 
 
 cdef const char *get_driver_name(GDALDriverH driver)
-cdef OGRSpatialReferenceH _osr_from_crs(object crs) except NULL
-cdef _safe_osr_release(OGRSpatialReferenceH srs)
+
 cdef void osr_set_traditional_axis_mapping_strategy(OGRSpatialReferenceH hSrs)
 cdef GDALDatasetH open_dataset(object filename, int mode, object allowed_drivers, object open_options, object siblings) except NULL
```

### Comparing `rasterio-1.3b2/rasterio/_base.pyx` & `rasterio-1.3b3/rasterio/_base.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from contextlib import ExitStack
 import logging
 import math
 import os
 import warnings
 
 from libc.string cimport strncmp
+from rasterio.crs cimport CRS
 
 from rasterio._err import (
     GDALError, CPLE_BaseError, CPLE_IllegalArgError, CPLE_OpenFailedError,
     CPLE_NotSupportedError)
 from rasterio._err cimport exc_wrap_pointer, exc_wrap_int, exc_wrap
 
 from rasterio.control import GroundControlPoint
@@ -1450,39 +1451,37 @@
 
 
 def _transform(src_crs, dst_crs, xs, ys, zs):
     """Transform input arrays from src to dst CRS."""
     cdef double *x = NULL
     cdef double *y = NULL
     cdef double *z = NULL
-    cdef OGRSpatialReferenceH src = NULL
-    cdef OGRSpatialReferenceH dst = NULL
     cdef OGRCoordinateTransformationH transform = NULL
     cdef int i
 
     assert len(xs) == len(ys)
     assert zs is None or len(xs) == len(zs)
 
-    src = _osr_from_crs(src_crs)
-    dst = _osr_from_crs(dst_crs)
+    cdef CRS src = CRS.from_user_input(src_crs)
+    cdef CRS dst = CRS.from_user_input(dst_crs)
 
     n = len(xs)
     x = <double *>CPLMalloc(n*sizeof(double))
     y = <double *>CPLMalloc(n*sizeof(double))
     for i in range(n):
         x[i] = xs[i]
         y[i] = ys[i]
 
     if zs is not None:
         z = <double *>CPLMalloc(n*sizeof(double))
         for i in range(n):
             z[i] = zs[i]
 
     try:
-        transform = OCTNewCoordinateTransformation(src, dst)
+        transform = OCTNewCoordinateTransformation(src._osr, dst._osr)
         transform = exc_wrap_pointer(transform)
         # OCTTransform() returns TRUE/FALSE contrary to most GDAL API functions
         exc_wrap_int(OCTTransform(transform, n, x, y, z) == 0)
     else:
         res_xs = [0]*n
         res_ys = [0]*n
         for i in range(n):
@@ -1496,55 +1495,14 @@
         else:
             return (res_xs, res_ys)
     finally:
         CPLFree(x)
         CPLFree(y)
         CPLFree(z)
         OCTDestroyCoordinateTransformation(transform)
-        _safe_osr_release(src)
-        _safe_osr_release(dst)
-
-
-cdef OGRSpatialReferenceH _osr_from_crs(object crs) except NULL:
-    """Returns a reference to memory that must be deallocated
-    by the caller."""
-    crs = CRS.from_user_input(crs)
-
-    # EPSG is a special case.
-    init = crs.get('init')
-    if init:
-        auth, val = init.strip().split(':')
-
-        if not val or auth.upper() != 'EPSG':
-            raise CRSError("Invalid CRS: {!r}".format(crs))
-        proj = 'EPSG:{}'.format(val).encode('utf-8')
-    else:
-        proj = crs.to_string().encode('utf-8')
-        log.debug("PROJ.4 to be imported: %r", proj)
-
-    cdef OGRSpatialReferenceH osr = OSRNewSpatialReference(NULL)
-    try:
-        retval = exc_wrap_int(OSRSetFromUserInput(osr, <const char *>proj))
-        if retval:
-            _safe_osr_release(osr)
-            raise CRSError("Invalid CRS: {!r}".format(crs))
-    except CPLE_BaseError as exc:
-        _safe_osr_release(osr)
-        raise CRSError(str(exc))
-    else:
-        osr_set_traditional_axis_mapping_strategy(osr)
-        return osr
-
-
-cdef _safe_osr_release(OGRSpatialReferenceH srs):
-    """Wrapper to handle OSR release when NULL."""
-
-    if srs != NULL:
-        OSRRelease(srs)
-    srs = NULL
 
 
 def _can_create_osr(crs):
     """Evaluate if a valid OGRSpatialReference can be created from crs.
 
     Specifically, it must not be None or an empty dict or string.
 
@@ -1554,30 +1512,18 @@
 
     Returns
     -------
     out: bool
         True if source coordinate reference appears valid.
     """
 
-    cdef char *wkt = NULL
-    cdef OGRSpatialReferenceH osr = NULL
-
     try:
-        # Note: _osr_from_crs() has "except NULL" in its signature.
-        # It raises, it does not return NULL.
-        osr = _osr_from_crs(crs)
-        OSRExportToWkt(osr, &wkt)
-
+        wkt = CRS.from_user_input(crs).to_wkt()
         # If input was empty, WKT can be too; otherwise the conversion
         # didn't work properly and indicates an error.
-        return wkt != NULL and bool(crs) == (wkt[0] != 0)
-
+        return bool(wkt)
     except CRSError:
         return False
 
-    finally:
-        _safe_osr_release(osr)
-        CPLFree(wkt)
-
 
 cdef void osr_set_traditional_axis_mapping_strategy(OGRSpatialReferenceH hSrs):
     OSRSetAxisMappingStrategy(hSrs, OAMS_TRADITIONAL_GIS_ORDER)
```

### Comparing `rasterio-1.3b2/rasterio/_env.pyx` & `rasterio-1.3b3/rasterio/_env.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from contextlib import contextmanager
 import logging
 import os
 import os.path
 import sys
 import threading
 
-from rasterio._base cimport _safe_osr_release
 from rasterio._err import CPLE_BaseError
 from rasterio._err cimport exc_wrap_ogrerr, exc_wrap_int
 from rasterio._filepath cimport install_filepath_plugin, uninstall_filepath_plugin
 from rasterio._version import gdal_version
 
 from libc.stdio cimport stderr
 
@@ -308,15 +307,16 @@
             with catch_errors():
                 exc_wrap_ogrerr(exc_wrap_int(OSRImportFromProj4(osr, "+init=epsg:4326")))
         except CPLE_BaseError:
             return False
         else:
             return True
         finally:
-            _safe_osr_release(osr)
+            if osr != NULL:
+                OSRRelease(osr)
 
 
     def search(self, prefix=None):
         """Returns PROJ data directory
 
         Note well that os.environ is not consulted.
```

### Comparing `rasterio-1.3b2/rasterio/_err.pyx` & `rasterio-1.3b3/rasterio/_err.pyx`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/_example.pyx` & `rasterio-1.3b3/rasterio/_example.pyx`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/_features.pxd` & `rasterio-1.3b3/rasterio/_features.pxd`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/_features.pyx` & `rasterio-1.3b3/rasterio/_features.pyx`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/_filepath.pyx` & `rasterio-1.3b3/rasterio/_filepath.pyx`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/_fill.pyx` & `rasterio-1.3b3/rasterio/_fill.pyx`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/_io.pxd` & `rasterio-1.3b3/rasterio/_io.pxd`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/_io.pyx` & `rasterio-1.3b3/rasterio/_io.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,15 @@
 from rasterio.windows import Window, intersection
 
 from libc.stdio cimport FILE
 
 from rasterio.enums import Resampling
 from rasterio.env import GDALVersion
 from rasterio.errors import ResamplingAlgorithmError, DatasetIOShapeError
-from rasterio._base cimport (
-    _osr_from_crs, _safe_osr_release, get_driver_name, DatasetBase)
+from rasterio._base cimport get_driver_name, DatasetBase
 from rasterio._err cimport exc_wrap_int, exc_wrap_pointer, exc_wrap_vsilfile
 
 cimport numpy as np
 
 log = logging.getLogger(__name__)
 
 gdal33_version_checked = False
@@ -1997,23 +1996,23 @@
                 gcplist[i].dfGCPPixel = obj.col
                 gcplist[i].dfGCPLine = obj.row
                 gcplist[i].dfGCPX = obj.x
                 gcplist[i].dfGCPY = obj.y
                 gcplist[i].dfGCPZ = obj.z or 0.0
 
             # Try to use the primary crs if possible.
-            if not crs:
+            if crs is None:
                 crs = self.crs
-
-            osr = _osr_from_crs(crs)
-            OSRExportToWkt(osr, <char**>&srcwkt)
+            else:
+                crs = CRS.from_user_input(crs)
+            srcwkt_b = crs.to_wkt().encode('utf-8')
+            srcwkt = srcwkt_b
             GDALSetGCPs(self.handle(), len(gcps), gcplist, srcwkt)
         finally:
             CPLFree(gcplist)
-            CPLFree(srcwkt)
 
         # Invalidate cached value.
         self._gcps = None
 
     def _set_rpcs(self, rpcs):
         if hasattr(rpcs, 'to_gdal'):
             rpcs = rpcs.to_gdal()
```

### Comparing `rasterio-1.3b2/rasterio/_loading.py` & `rasterio-1.3b3/rasterio/_loading.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/_path.py` & `rasterio-1.3b3/rasterio/_path.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/_show_versions.py` & `rasterio-1.3b3/rasterio/_show_versions.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/_transform.pyx` & `rasterio-1.3b3/rasterio/_transform.pyx`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/_version.pyx` & `rasterio-1.3b3/rasterio/_version.pyx`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/_warp.pxd` & `rasterio-1.3b3/rasterio/_warp.pxd`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/_warp.pyx` & `rasterio-1.3b3/rasterio/_warp.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -31,28 +31,25 @@
     WarpOperationError)
 from rasterio.transform import Affine, from_bounds, guard_transform, tastes_like_gdal
 
 cimport cython
 cimport numpy as np
 from libc.math cimport HUGE_VAL
 
-from rasterio._base cimport _osr_from_crs, get_driver_name, _safe_osr_release
+from rasterio._base cimport get_driver_name
 from rasterio._err cimport exc_wrap, exc_wrap_pointer, exc_wrap_int
 from rasterio._io cimport (
     DatasetReaderBase, MemoryDataset, in_dtype_range, io_auto)
 from rasterio._features cimport GeomBuilder, OGRGeomBuilder
-
+from rasterio.crs cimport CRS
 
 log = logging.getLogger(__name__)
 
 # Gauss (7) is not supported for warp
-SUPPORTED_RESAMPLING = [r for r in Resampling if r.value != 7 and r.value <= 12]
-# sum supported since GDAL 3.1
-if GDALVersion.runtime().at_least('3.1'):
-    SUPPORTED_RESAMPLING.append(Resampling.sum)
+SUPPORTED_RESAMPLING = [r for r in Resampling if r.value != 7 and r.value <= 13]
 # rms supported since GDAL 3.3
 if GDALVersion.runtime().at_least('3.3'):
     SUPPORTED_RESAMPLING.append(Resampling.rms)
 
 def recursive_round(val, precision):
     """Recursively round coordinates."""
     if isinstance(val, (int, float)):
@@ -91,27 +88,21 @@
 
 
 def _transform_geom(
         src_crs, dst_crs, geom, antimeridian_cutting, antimeridian_offset,
         int precision):
     """Return a transformed geometry."""
     cdef char **options = NULL
-    cdef OGRSpatialReferenceH src = NULL
-    cdef OGRSpatialReferenceH dst = NULL
     cdef OGRCoordinateTransformationH transform = NULL
     cdef OGRGeometryFactory *factory = NULL
 
-    src = _osr_from_crs(src_crs)
-    dst = _osr_from_crs(dst_crs)
+    cdef CRS src = CRS.from_user_input(src_crs)
+    cdef CRS dst = CRS.from_user_input(dst_crs)
 
-    try:
-        transform = exc_wrap_pointer(OCTNewCoordinateTransformation(src, dst))
-    finally:
-        _safe_osr_release(src)
-        _safe_osr_release(dst)
+    transform = exc_wrap_pointer(OCTNewCoordinateTransformation(src._osr, dst._osr))
 
     # GDAL cuts on the antimeridian by default and using different
     # logic in versions >= 2.2.
     if GDALVersion().runtime() < GDALVersion.parse('2.2'):
         valb = str(antimeridian_offset).encode('utf-8')
         options = CSLSetNameValue(options, "DATELINEOFFSET", <const char *>valb)
         if antimeridian_cutting:
@@ -631,15 +622,14 @@
 ):
     """Wraps GDAL's algorithm."""
     cdef void *hTransformArg = NULL
     cdef int npixels = 0
     cdef int nlines = 0
     cdef double extent[4]
     cdef double geotransform[6]
-    cdef OGRSpatialReferenceH osr = NULL
     cdef char *wkt = NULL
     cdef GDALDatasetH hds = NULL
     cdef char **imgProjOptions = NULL
     cdef char **papszMD = NULL
     cdef bint bUseApproxTransformer = True
 
     extent[:] = [0.0, 0.0, 0.0, 0.0]
@@ -649,43 +639,33 @@
         transform = from_bounds(left, bottom, right, top, width, height)
     elif any(x is not None for x in (left, bottom, right, top)):
         raise ValueError(
             "Some, but not all, bounding box parameters were provided.")
     else:
         transform = None
 
-    try:
-        osr = _osr_from_crs(dst_crs)
-        exc_wrap_int(OSRExportToWkt(osr, &wkt))
-    except CPLE_BaseError as exc:
-        raise CRSError("Could not convert to WKT. {}".format(str(exc)))
-    finally:
-        _safe_osr_release(osr)
-
-    if isinstance(src_crs, str):
-        src_crs = CRS.from_string(src_crs)
-    elif isinstance(src_crs, dict):
-        src_crs = CRS(**src_crs)
-
+    dst_crs = CRS.from_user_input(dst_crs)
+    wkt_b = dst_crs.to_wkt().encode('utf-8')
+    wkt = wkt_b
+    if src_crs is not None:
+        src_crs = CRS.from_user_input(src_crs)
     # The transformer at the heart of this function requires a dataset.
     # We use an in-memory VRT dataset.
     vrt_doc = _suggested_proxy_vrt_doc(
         width,
         height,
         transform=transform,
         crs=src_crs,
         gcps=gcps
-    ).decode('ascii')
+    ).decode('utf-8')
     hds = open_dataset(vrt_doc, 0x00 | 0x02 | 0x04, ['VRT'], {}, None)
-
     try:
         imgProjOptions = CSLSetNameValue(imgProjOptions, "GCPS_OK", "TRUE")
         imgProjOptions = CSLSetNameValue(imgProjOptions, "MAX_GCP_ORDER", "0")
         imgProjOptions = CSLSetNameValue(imgProjOptions, "DST_SRS", wkt)
-
         for key, val in kwargs.items():
             key = key.upper().encode('utf-8')
 
             if key in {b"RPC_DEM", b"COORDINATE_OPERATION"}:
                 # don't .upper() since might be a path.
                 val = str(val).encode('utf-8')
             else:
@@ -727,16 +707,14 @@
             )
         )
 
     except CPLE_NotSupportedError as err:
         raise CRSError(err.errmsg)
 
     finally:
-        if wkt != NULL:
-            CPLFree(wkt)
         if hTransformArg != NULL:
             GDALDestroyGenImgProjTransformer(hTransformArg)
         if hds != NULL:
             GDALClose(hds)
         if imgProjOptions != NULL:
             CPLFree(imgProjOptions)
         if papszMD != NULL:
@@ -962,31 +940,21 @@
                 self.src_gcps, self.src_crs = self.src_dataset.get_gcps()
             except ValueError:
                 pass
 
         self.dst_crs = CRS.from_user_input(crs) if crs is not None else self.src_crs
 
         # Convert CRSes to C WKT strings.
-        try:
-            if not self.src_crs:
-                src_crs_wkt = NULL
-            else:
-                osr = _osr_from_crs(self.src_crs)
-                OSRExportToWkt(osr, &src_crs_wkt)
-        finally:
-            if osr != NULL:
-                OSRRelease(osr)
-            osr = NULL
+        if self.src_crs is not None:
+            src_crs_wkt_b = self.src_crs.to_wkt().encode("utf-8")
+            src_crs_wkt = src_crs_wkt_b
 
         if self.dst_crs is not None:
-            try:
-                osr = _osr_from_crs(self.dst_crs)
-                OSRExportToWkt(osr, &dst_crs_wkt)
-            finally:
-                _safe_osr_release(osr)
+            dst_crs_wkt_b = self.dst_crs.to_wkt().encode("utf-8")
+            dst_crs_wkt = dst_crs_wkt_b
 
         log.debug("Exported CRS to WKT.")
 
         log.debug("Warp_extras: %r", self.warp_extras)
 
         for key, val in self.warp_extras.items():
             key = key.upper().encode('utf-8')
@@ -1056,16 +1024,14 @@
                     dst_crs_wkt,
                     c_resampling,
                     c_tolerance,
                     psWOptions,
                     <const char **>c_warp_extras,
                 )
             finally:
-                CPLFree(dst_crs_wkt)
-                CPLFree(src_crs_wkt)
                 CSLDestroy(c_warp_extras)
                 if psWOptions != NULL:
                     GDALDestroyWarpOptions(psWOptions)
 
         else:
             # Case 1
             if self.dst_transform and self.dst_width and self.dst_height:
@@ -1111,16 +1077,14 @@
                 self.dst_transform = self.dst_transform * Affine.scale(
                     width / self.dst_width, height / self.dst_height
                 )
 
             # If we get here it's because the tests above are buggy.
             # We raise a Python exception to indicate that.
             else:
-                CPLFree(dst_crs_wkt)
-                CPLFree(src_crs_wkt)
                 CSLDestroy(c_warp_extras)
                 if psWOptions != NULL:
                     GDALDestroyWarpOptions(psWOptions)
                 raise RuntimeError("Parameterization error")
 
             # Continue with finishing cases 1-3, which have been
             # generalized.
@@ -1151,16 +1115,14 @@
                 psWOptions.pTransformerArg = hTransformArg
 
                 with nogil:
                     hds_warped = GDALCreateWarpedVRT(hds, c_width, c_height, dst_gt, psWOptions)
                     GDALSetProjection(hds_warped, dst_crs_wkt)
 
             finally:
-                CPLFree(dst_crs_wkt)
-                CPLFree(src_crs_wkt)
                 CSLDestroy(c_warp_extras)
                 if psWOptions != NULL:
                     GDALDestroyWarpOptions(psWOptions)
 
         # End of the 4 cases.
 
         try:
@@ -1468,36 +1430,29 @@
     return max_value
 
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 def _transform_bounds(
-    src_crs,
-    dst_crs,
+    CRS src_crs,
+    CRS dst_crs,
     double left,
     double bottom,
     double right,
     double top,
     int densify_pts,
 ):
-    src_crs = CRS.from_user_input(src_crs)
-    dst_crs = CRS.from_user_input(dst_crs)
-
     IF (CTE_GDAL_MAJOR_VERSION, CTE_GDAL_MINOR_VERSION) >= (3, 4):
         cdef double out_left = np.inf
         cdef double out_bottom = np.inf
         cdef double out_right = np.inf
         cdef double out_top = np.inf
-        cdef OGRSpatialReferenceH src = NULL
-        cdef OGRSpatialReferenceH dst = NULL
         cdef OGRCoordinateTransformationH transform = NULL
-        src = _osr_from_crs(src_crs)
-        dst = _osr_from_crs(dst_crs)
-        transform = OCTNewCoordinateTransformation(src, dst)
+        transform = OCTNewCoordinateTransformation(src_crs._osr, dst_crs._osr)
         transform = exc_wrap_pointer(transform)
 
         # OCTTransformBounds() returns TRUE/FALSE contrary to most GDAL API functions
         cdef int status = 0
 
         try:
             status = OCTTransformBounds(
@@ -1505,17 +1460,14 @@
                 left, bottom, right, top,
                 &out_left, &out_bottom, &out_right, &out_top,
                 densify_pts
             )
             exc_wrap_int(status == 0)
         finally:
             OCTDestroyCoordinateTransformation(transform)
-            _safe_osr_release(src)
-            _safe_osr_release(dst)
-
         return out_left, out_bottom, out_right, out_top
 
     ELSE:
         if src_crs == dst_crs:
             return (left, bottom, right, top)
 
         if densify_pts < 0:
```

### Comparing `rasterio-1.3b2/rasterio/control.py` & `rasterio-1.3b3/rasterio/control.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/coords.py` & `rasterio-1.3b3/rasterio/coords.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/crs.pyx` & `rasterio-1.3b3/rasterio/crs.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 import re
 
 import rasterio._env
 from rasterio._err import CPLE_BaseError, CPLE_NotSupportedError
 from rasterio.errors import CRSError
 from rasterio.enums import WktVersion
 
-from rasterio._base cimport _osr_from_crs as osr_from_crs
-from rasterio._base cimport _safe_osr_release, osr_set_traditional_axis_mapping_strategy
+from rasterio._base cimport osr_set_traditional_axis_mapping_strategy
 from rasterio._err cimport exc_wrap_ogrerr, exc_wrap_int, exc_wrap_pointer
 
 
 log = logging.getLogger(__name__)
 
 
 _RE_PROJ_PARAM = re.compile(r"""
@@ -45,14 +44,22 @@
     (?P<param>\w+)    # capture parameter name
     \=?             # match both key only and key-value parameters
     (?P<value>\S+)? # capture all characters up to next space (None if no value)
     \s*?            # consume remaining whitespace, if any
 """, re.X)
 
 
+
+cdef _safe_osr_release(OGRSpatialReferenceH srs):
+    """Wrapper to handle OSR release when NULL."""
+    if srs != NULL:
+        OSRRelease(srs)
+    srs = NULL
+
+
 cdef class CRS:
     """A geographic or projected coordinate reference system.
 
     CRS objects may be created by passing PROJ parameters as keyword
     arguments to the standard constructor or by passing EPSG codes, PROJ
     mappings, PROJ strings, or WKT strings to the from_epsg, from_dict,
     from_string, or from_wkt static methods.
```

### Comparing `rasterio-1.3b2/rasterio/drivers.py` & `rasterio-1.3b3/rasterio/drivers.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/dtypes.py` & `rasterio-1.3b3/rasterio/dtypes.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/enums.py` & `rasterio-1.3b3/rasterio/enums.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/env.py` & `rasterio-1.3b3/rasterio/env.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/errors.py` & `rasterio-1.3b3/rasterio/errors.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/features.py` & `rasterio-1.3b3/rasterio/features.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/fill.py` & `rasterio-1.3b3/rasterio/fill.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/gdal.pxi` & `rasterio-1.3b3/rasterio/gdal.pxi`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/io.py` & `rasterio-1.3b3/rasterio/io.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/mask.py` & `rasterio-1.3b3/rasterio/mask.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/merge.py` & `rasterio-1.3b3/rasterio/merge.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/path.py` & `rasterio-1.3b3/rasterio/path.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/plot.py` & `rasterio-1.3b3/rasterio/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,17 +64,17 @@
         each band so that they fall between 0 and 1 before plotting. If
         True, values will be adjusted by the min / max of each band. If
         False, no adjustment will be applied.
     **kwargs : key, value pairings optional
         These will be passed to the matplotlib imshow or contour method
         depending on contour argument.
         See full lists at:
-        http://matplotlib.org/api/axes_api.html?highlight=imshow#matplotlib.axes.Axes.imshow
+        https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.imshow.html
         or
-        http://matplotlib.org/api/axes_api.html?highlight=imshow#matplotlib.axes.Axes.contour
+        https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.contour.html
 
     Returns
     -------
     ax : matplotlib Axes
         Axes with plot.
     """
     plt = get_plt()
```

### Comparing `rasterio-1.3b2/rasterio/profiles.py` & `rasterio-1.3b3/rasterio/profiles.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/rio/blocks.py` & `rasterio-1.3b3/rasterio/rio/blocks.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/rio/bounds.py` & `rasterio-1.3b3/rasterio/rio/bounds.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/rio/calc.py` & `rasterio-1.3b3/rasterio/rio/calc.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/rio/clip.py` & `rasterio-1.3b3/rasterio/rio/clip.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/rio/convert.py` & `rasterio-1.3b3/rasterio/rio/convert.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/rio/edit_info.py` & `rasterio-1.3b3/rasterio/rio/edit_info.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/rio/env.py` & `rasterio-1.3b3/rasterio/rio/env.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/rio/gcps.py` & `rasterio-1.3b3/rasterio/rio/gcps.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/rio/helpers.py` & `rasterio-1.3b3/rasterio/rio/helpers.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/rio/info.py` & `rasterio-1.3b3/rasterio/rio/info.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/rio/insp.py` & `rasterio-1.3b3/rasterio/rio/insp.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/rio/main.py` & `rasterio-1.3b3/rasterio/rio/main.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/rio/mask.py` & `rasterio-1.3b3/rasterio/rio/mask.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/rio/merge.py` & `rasterio-1.3b3/rasterio/rio/merge.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/rio/options.py` & `rasterio-1.3b3/rasterio/rio/options.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/rio/overview.py` & `rasterio-1.3b3/rasterio/rio/overview.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/rio/rasterize.py` & `rasterio-1.3b3/rasterio/rio/rasterize.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/rio/rm.py` & `rasterio-1.3b3/rasterio/rio/rm.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/rio/sample.py` & `rasterio-1.3b3/rasterio/rio/sample.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/rio/shapes.py` & `rasterio-1.3b3/rasterio/rio/shapes.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/rio/stack.py` & `rasterio-1.3b3/rasterio/rio/stack.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/rio/transform.py` & `rasterio-1.3b3/rasterio/rio/transform.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/rio/warp.py` & `rasterio-1.3b3/rasterio/rio/warp.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/rpc.py` & `rasterio-1.3b3/rasterio/rpc.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/sample.py` & `rasterio-1.3b3/rasterio/sample.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/session.py` & `rasterio-1.3b3/rasterio/session.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/shutil.pyx` & `rasterio-1.3b3/rasterio/shutil.pyx`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/tools.py` & `rasterio-1.3b3/rasterio/tools.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/transform.py` & `rasterio-1.3b3/rasterio/transform.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/vrt.py` & `rasterio-1.3b3/rasterio/vrt.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio/warp.py` & `rasterio-1.3b3/rasterio/warp.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import numpy as np
 
 import rasterio._loading
 with rasterio._loading.add_gdal_dll_directories():
     import rasterio
 
     from rasterio._base import _transform
+    from rasterio.crs import CRS
     from rasterio.enums import Resampling
     from rasterio.env import ensure_env, require_gdal_version
     from rasterio.errors import TransformError, RPCError
     from rasterio.transform import array_bounds
     from rasterio._warp import (
         _calculate_default_transform,
         _reproject,
@@ -141,14 +142,16 @@
         worse performance.  Default: 21 (gdal default).
 
     Returns
     -------
     left, bottom, right, top: float
         Outermost coordinates in target coordinate reference system.
     """
+    src_crs = CRS.from_user_input(src_crs)
+    dst_crs = CRS.from_user_input(dst_crs)
     return _transform_bounds(
         src_crs,
         dst_crs,
         left,
         bottom,
         right,
         top,
```

### Comparing `rasterio-1.3b2/rasterio/windows.py` & `rasterio-1.3b3/rasterio/windows.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio.egg-info/PKG-INFO` & `rasterio-1.3b3/rasterio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasterio
-Version: 1.3b2
+Version: 1.3b3
 Summary: Fast and direct raster I/O for use with Numpy and SciPy
 Home-page: https://github.com/rasterio/rasterio
 Author: Sean Gillies
 Author-email: sean@mapbox.com
 License: BSD
 Keywords: raster gdal
 Platform: UNKNOWN
```

### Comparing `rasterio-1.3b2/rasterio.egg-info/SOURCES.txt` & `rasterio-1.3b3/rasterio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/rasterio.egg-info/entry_points.txt` & `rasterio-1.3b3/rasterio.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/setup.cfg` & `rasterio-1.3b3/setup.cfg`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/setup.py` & `rasterio-1.3b3/setup.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/README.rst` & `rasterio-1.3b3/tests/README.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/conftest.py` & `rasterio-1.3b3/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -624,18 +624,14 @@
         self.__geo_interface__ = geojson
 
 
 # Define helpers to skip tests based on GDAL version
 gdal_version = GDALVersion.runtime()
 
 
-requires_gdal31 = pytest.mark.skipif(
-    not gdal_version.at_least("3.1"), reason="Requires GDAL 3.1.x"
-)
-
 requires_gdal32 = pytest.mark.skipif(
     not gdal_version.at_least('3.2'),
     reason="Requires GDAL 3.2.x")
 
 requires_gdal33 = pytest.mark.skipif(
     not gdal_version.at_least('3.3'),
     reason="Requires GDAL 3.3.x")
```

### Comparing `rasterio-1.3b2/tests/data/README.rst` & `rasterio-1.3b3/tests/data/README.rst`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/rangehttpserver.py` & `rasterio-1.3b3/tests/rangehttpserver.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test__env.py` & `rasterio-1.3b3/tests/test__env.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test__version.py` & `rasterio-1.3b3/tests/test__version.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_band_masks.py` & `rasterio-1.3b3/tests/test_band_masks.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_blocks.py` & `rasterio-1.3b3/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_boundless_read.py` & `rasterio-1.3b3/tests/test_boundless_read.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_checksum.py` & `rasterio-1.3b3/tests/test_checksum.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_cli_main.py` & `rasterio-1.3b3/tests/test_cli_main.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_colorinterp.py` & `rasterio-1.3b3/tests/test_colorinterp.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_colormap.py` & `rasterio-1.3b3/tests/test_colormap.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_complex_dtypes.py` & `rasterio-1.3b3/tests/test_complex_dtypes.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_coords.py` & `rasterio-1.3b3/tests/test_coords.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_creation_options.py` & `rasterio-1.3b3/tests/test_creation_options.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_crs.py` & `rasterio-1.3b3/tests/test_crs.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 import rasterio
 from rasterio._base import _can_create_osr
 from rasterio.crs import CRS, epsg_treats_as_latlong, epsg_treats_as_northingeasting
 from rasterio.enums import WktVersion
 from rasterio.env import env_ctx_if_needed, Env
 from rasterio.errors import CRSError
 
-from .conftest import requires_gdal31
-
 # Items like "D_North_American_1983" characterize the Esri dialect
 # of WKT SRS.
 ESRI_PROJECTION_STRING = (
     'PROJCS["USA_Contiguous_Albers_Equal_Area_Conic_USGS_version",'
     'GEOGCS["GCS_North_American_1983",DATUM["D_North_American_1983",'
     'SPHEROID["GRS_1980",6378137.0,298.257222101]],'
     'PRIMEM["Greenwich",0.0],'
@@ -615,52 +613,45 @@
 def test_tmerc_no_match():
     """Should not match an authority, see issue #2293."""
     s = "+proj=tmerc +lat_0=0 +lon_0=10.7584 +k=0.9996 +x_0=0 +y_0=0 +datum=WGS84 +units=m +no_defs"
     crs = CRS.from_string(s)
     assert crs.to_epsg() is None
 
 
-@requires_gdal31
 def test_crs_to_json_dict():
     aeqd_crs = CRS(proj="aeqd", lon_0=-80, lat_0=40.5)
     json_dict = aeqd_crs.to_dict(projjson=True)
     assert json_dict["type"] == "ProjectedCRS"
 
 
-@requires_gdal31
 def test_crs_to_json_dict__empty():
     crs = CRS()
     assert crs.to_dict(projjson=True) == {}
 
 
-@requires_gdal31
 def test_crs_from_json_dict():
     aeqd_crs = CRS(proj="aeqd", lon_0=-80, lat_0=40.5)
     assert CRS.from_dict(aeqd_crs.to_dict(projjson=True)) == aeqd_crs
 
 
-@requires_gdal31
 def test_crs_from_json_dict__user_input():
     aeqd_crs = CRS(proj="aeqd", lon_0=-80, lat_0=40.5)
     assert CRS.from_user_input(aeqd_crs.to_dict(projjson=True)) == aeqd_crs
 
 
-@requires_gdal31
 def test_crs_from_json_dict__init():
     aeqd_crs = CRS(proj="aeqd", lon_0=-80, lat_0=40.5)
     assert CRS(aeqd_crs.to_dict(projjson=True)) == aeqd_crs
 
 
-@requires_gdal31
 def test_crs_proj_json__user_input():
     aeqd_crs = CRS(proj="aeqd", lon_0=-80, lat_0=40.5)
     assert CRS.from_user_input(json.dumps(aeqd_crs.to_dict(projjson=True))) == aeqd_crs
 
 
-@requires_gdal31
 def test_crs_proj_json__from_string():
     aeqd_crs = CRS(proj="aeqd", lon_0=-80, lat_0=40.5)
     assert CRS.from_string(json.dumps(aeqd_crs.to_dict(projjson=True))) == aeqd_crs
 
 
 def test_crs_compound_epsg():
     assert CRS.from_string("EPSG:4326+3855").to_wkt().startswith("COMPD")
```

### Comparing `rasterio-1.3b2/tests/test_dataset.py` & `rasterio-1.3b3/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_dataset_mask.py` & `rasterio-1.3b3/tests/test_dataset_mask.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_dataset_rw.py` & `rasterio-1.3b3/tests/test_dataset_rw.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_descriptions.py` & `rasterio-1.3b3/tests/test_descriptions.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_driver_management.py` & `rasterio-1.3b3/tests/test_driver_management.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_dtypes.py` & `rasterio-1.3b3/tests/test_dtypes.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_env.py` & `rasterio-1.3b3/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_err.py` & `rasterio-1.3b3/tests/test_err.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_features.py` & `rasterio-1.3b3/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_filepath.py` & `rasterio-1.3b3/tests/test_filepath.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_fillnodata.py` & `rasterio-1.3b3/tests/test_fillnodata.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_gcps.py` & `rasterio-1.3b3/tests/test_gcps.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_gdal_raster_io.py` & `rasterio-1.3b3/tests/test_gdal_raster_io.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_image_structure.py` & `rasterio-1.3b3/tests/test_image_structure.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_indexing.py` & `rasterio-1.3b3/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_int8.py` & `rasterio-1.3b3/tests/test_int8.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_io.py` & `rasterio-1.3b3/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_io_mixins.py` & `rasterio-1.3b3/tests/test_io_mixins.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_mask.py` & `rasterio-1.3b3/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_mask_creation.py` & `rasterio-1.3b3/tests/test_mask_creation.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_memoryfile.py` & `rasterio-1.3b3/tests/test_memoryfile.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_merge.py` & `rasterio-1.3b3/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_meta.py` & `rasterio-1.3b3/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_no_georef.py` & `rasterio-1.3b3/tests/test_no_georef.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_nodata.py` & `rasterio-1.3b3/tests/test_nodata.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_open.py` & `rasterio-1.3b3/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_open_options.py` & `rasterio-1.3b3/tests/test_open_options.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_open_overview_level.py` & `rasterio-1.3b3/tests/test_open_overview_level.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_open_sharing.py` & `rasterio-1.3b3/tests/test_open_sharing.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_overviews.py` & `rasterio-1.3b3/tests/test_overviews.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_path.py` & `rasterio-1.3b3/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_plot.py` & `rasterio-1.3b3/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_png.py` & `rasterio-1.3b3/tests/test_png.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_process_pool_executor.py` & `rasterio-1.3b3/tests/test_process_pool_executor.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_profile.py` & `rasterio-1.3b3/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_read.py` & `rasterio-1.3b3/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_read_boundless.py` & `rasterio-1.3b3/tests/test_read_boundless.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_read_dtype.py` & `rasterio-1.3b3/tests/test_read_dtype.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_read_resample.py` & `rasterio-1.3b3/tests/test_read_resample.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_reshape_image.py` & `rasterio-1.3b3/tests/test_reshape_image.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_revolvingdoor.py` & `rasterio-1.3b3/tests/test_revolvingdoor.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_rio_blocks.py` & `rasterio-1.3b3/tests/test_rio_blocks.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_rio_bounds.py` & `rasterio-1.3b3/tests/test_rio_bounds.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_rio_calc.py` & `rasterio-1.3b3/tests/test_rio_calc.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_rio_clip.py` & `rasterio-1.3b3/tests/test_rio_clip.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_rio_convert.py` & `rasterio-1.3b3/tests/test_rio_convert.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_rio_edit_info.py` & `rasterio-1.3b3/tests/test_rio_edit_info.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_rio_gcp.py` & `rasterio-1.3b3/tests/test_rio_gcp.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_rio_helpers.py` & `rasterio-1.3b3/tests/test_rio_helpers.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_rio_info.py` & `rasterio-1.3b3/tests/test_rio_info.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_rio_insp.py` & `rasterio-1.3b3/tests/test_rio_insp.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_rio_main.py` & `rasterio-1.3b3/tests/test_rio_main.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_rio_mask.py` & `rasterio-1.3b3/tests/test_rio_mask.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_rio_merge.py` & `rasterio-1.3b3/tests/test_rio_merge.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_rio_options.py` & `rasterio-1.3b3/tests/test_rio_options.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_rio_overview.py` & `rasterio-1.3b3/tests/test_rio_overview.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_rio_rasterize.py` & `rasterio-1.3b3/tests/test_rio_rasterize.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_rio_rm.py` & `rasterio-1.3b3/tests/test_rio_rm.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_rio_sample.py` & `rasterio-1.3b3/tests/test_rio_sample.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_rio_shapes.py` & `rasterio-1.3b3/tests/test_rio_shapes.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_rio_stack.py` & `rasterio-1.3b3/tests/test_rio_stack.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_rio_warp.py` & `rasterio-1.3b3/tests/test_rio_warp.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_rpcs.py` & `rasterio-1.3b3/tests/test_rpcs.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_sampling.py` & `rasterio-1.3b3/tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_scale_offset.py` & `rasterio-1.3b3/tests/test_scale_offset.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_session.py` & `rasterio-1.3b3/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_show_versions.py` & `rasterio-1.3b3/tests/test_show_versions.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_shutil.py` & `rasterio-1.3b3/tests/test_shutil.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_tag_item.py` & `rasterio-1.3b3/tests/test_tag_item.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_tags.py` & `rasterio-1.3b3/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_thread_pool_executor.py` & `rasterio-1.3b3/tests/test_thread_pool_executor.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_threading.py` & `rasterio-1.3b3/tests/test_threading.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_tools.py` & `rasterio-1.3b3/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_transform.py` & `rasterio-1.3b3/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_units.py` & `rasterio-1.3b3/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_update.py` & `rasterio-1.3b3/tests/test_update.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,25 +61,14 @@
     tiffname = str(data.join('RGB.byte.tif'))
     with rasterio.open(tiffname, 'r+') as f:
         f.nodata = 255
     with rasterio.open(tiffname) as f:
         assert f.nodatavals == (255, 255, 255)
 
 
-@pytest.mark.skipif(
-    GDALVersion.runtime().at_least('2.1'),
-    reason='Tests behavior specific to GDAL versions < 2.1')
-def test_update_nodatavals_none_fails(data):
-    """GDAL 2.0 doesn't support un-setting nodata values."""
-    tiffname = str(data.join('RGB.byte.tif'))
-    with rasterio.open(tiffname, 'r+') as f:
-        with pytest.raises(NotImplementedError):
-            f.nodata = None
-
-
 def test_update_nodatavals_none(data):
     """GDAL 2.1 does support un-setting nodata values."""
     tiffname = str(data.join('RGB.byte.tif'))
     with rasterio.open(tiffname, 'r+') as f:
         f.nodata = None
     with rasterio.open(tiffname) as f:
         assert f.nodatavals == (None, None, None)
```

### Comparing `rasterio-1.3b2/tests/test_vrt.py` & `rasterio-1.3b3/tests/test_vrt.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_warnings.py` & `rasterio-1.3b3/tests/test_warnings.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_warp.py` & `rasterio-1.3b3/tests/test_warp.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,16 +281,16 @@
             479360.16562217404),
     )
 
 
 @pytest.mark.parametrize(
     "density,expected",
     [
-        (0, (-1684649.41338, -350356.81377, 1684649.41338, 2234551.18559)),
-        (100, (-1684649.41338, -555777.79210, 1684649.41338, 2234551.18559)),
+        (0, (-1688721.99764, -350040.36880, 1688799.61159, 2236495.86829)),
+        (100, (-1688721.99764, -555239.84875, 1688799.61159, 2236495.86829)),
     ],
 )
 def test_transform_bounds_densify(density, expected):
     # This transform is non-linear along the edges, so densification produces
     # a different result than otherwise
     src_crs = CRS.from_epsg(4326)
     dst_crs = CRS.from_epsg(2163)
```

### Comparing `rasterio-1.3b2/tests/test_warp_transform.py` & `rasterio-1.3b3/tests/test_warp_transform.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_warpedvrt.py` & `rasterio-1.3b3/tests/test_warpedvrt.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_windows.py` & `rasterio-1.3b3/tests/test_windows.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_windows_mixins.py` & `rasterio-1.3b3/tests/test_windows_mixins.py`

 * *Files identical despite different names*

### Comparing `rasterio-1.3b2/tests/test_write.py` & `rasterio-1.3b3/tests/test_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 import subprocess
 
 import affine
 import numpy as np
 import pytest
 
-from .conftest import requires_gdal31, requires_gdal35, gdal_version
+from .conftest import requires_gdal35, gdal_version
 
 import rasterio
 from rasterio.drivers import blacklist
 from rasterio.enums import MaskFlags, Resampling
 from rasterio.env import Env
 from rasterio.errors import RasterioIOError
 
@@ -427,15 +427,14 @@
         src.write(data, 1)
 
     captured = capsys.readouterr()
     assert "ERROR 4" not in captured.err
     assert "ERROR 4" not in captured.out
 
 
-@requires_gdal31
 def test_write_cog(tmpdir, path_rgb_byte_tif):
     """Show resolution of issue #2102"""
     with rasterio.open(path_rgb_byte_tif) as src:
         profile = src.profile
         profile.update(driver="COG", extent=src.bounds, resampling=Resampling.bilinear)
         with rasterio.open(str(tmpdir.join("test.tif")), "w", **profile) as cog:
             cog.write(src.read())
```

