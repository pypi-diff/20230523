# Comparing `tmp/gopro-overlay-0.94.0.tar.gz` & `tmp/gopro-overlay-0.95.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gopro-overlay-0.94.0.tar", last modified: Mon May 22 14:26:26 2023, max compression
+gzip compressed data, was "gopro-overlay-0.95.0.tar", last modified: Tue May 23 11:06:31 2023, max compression
```

## Comparing `gopro-overlay-0.94.0.tar` & `gopro-overlay-0.95.0.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-22 14:26:26.294604 gopro-overlay-0.94.0/
--rw-rw-r--   0 richja    (1000) richja    (1000)    35691 2023-05-22 13:30:42.000000 gopro-overlay-0.94.0/LICENSE.md
--rw-rw-r--   0 richja    (1000) richja    (1000)       70 2022-02-02 12:18:46.000000 gopro-overlay-0.94.0/MANIFEST.in
--rw-rw-r--   0 richja    (1000) richja    (1000)    12144 2023-05-22 14:26:26.294604 gopro-overlay-0.94.0/PKG-INFO
--rw-rw-r--   0 richja    (1000) richja    (1000)    11351 2023-05-22 14:25:26.000000 gopro-overlay-0.94.0/README.md
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-22 14:26:26.282604 gopro-overlay-0.94.0/bin/
--rw-rw-r--   0 richja    (1000) richja    (1000)     3153 2022-05-23 15:18:05.000000 gopro-overlay-0.94.0/bin/gopro-contrib-data-extract.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1450 2022-02-03 15:47:43.000000 gopro-overlay-0.94.0/bin/gopro-cut.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    15036 2023-05-22 09:35:24.000000 gopro-overlay-0.94.0/bin/gopro-dashboard.py
--rwxrwxr-x   0 richja    (1000) richja    (1000)      770 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/bin/gopro-debug.py
--rwxrwxr-x   0 richja    (1000) richja    (1000)      596 2022-11-29 16:44:06.000000 gopro-overlay-0.94.0/bin/gopro-extract.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1035 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/bin/gopro-join.py
--rwxrwxr-x   0 richja    (1000) richja    (1000)     5527 2023-05-06 09:06:40.000000 gopro-overlay-0.94.0/bin/gopro-layout.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3578 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/bin/gopro-rename.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5783 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/bin/gopro-to-csv.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3412 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/bin/gopro-to-gpx.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-22 14:26:26.286604 gopro-overlay-0.94.0/gopro_overlay/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2022-02-02 11:42:38.000000 gopro-overlay-0.94.0/gopro_overlay/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      299 2023-05-22 14:24:40.000000 gopro-overlay-0.94.0/gopro_overlay/__version__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     7063 2023-05-22 08:55:54.000000 gopro-overlay-0.94.0/gopro_overlay/arguments.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5447 2023-05-08 10:30:40.000000 gopro-overlay-0.94.0/gopro_overlay/buffering.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      690 2022-11-29 17:00:53.000000 gopro-overlay-0.94.0/gopro_overlay/common.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      207 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/counter.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      483 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/date_overlap.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      531 2023-02-07 21:58:09.000000 gopro-overlay-0.94.0/gopro_overlay/dimensions.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1719 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/entry.py
--rw-rw-r--   0 richja    (1000) richja    (1000)       34 2022-11-23 14:47:58.000000 gopro-overlay-0.94.0/gopro_overlay/exceptions.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1345 2023-05-06 10:59:08.000000 gopro-overlay-0.94.0/gopro_overlay/execution.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3671 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/fake.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    10025 2023-05-22 09:32:45.000000 gopro-overlay-0.94.0/gopro_overlay/ffmpeg.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1285 2023-05-22 09:02:15.000000 gopro-overlay-0.94.0/gopro_overlay/ffmpeg_profile.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1803 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/filenaming.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2279 2023-05-01 11:53:38.000000 gopro-overlay-0.94.0/gopro_overlay/fit.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      122 2021-12-03 14:46:33.000000 gopro-overlay-0.94.0/gopro_overlay/font.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    10542 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/framemeta.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3000 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/framemeta_gpx.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      478 2022-05-27 13:38:56.000000 gopro-overlay-0.94.0/gopro_overlay/functional.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5703 2023-02-08 14:26:51.000000 gopro-overlay-0.94.0/gopro_overlay/geo.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2426 2023-02-09 10:45:34.000000 gopro-overlay-0.94.0/gopro_overlay/geo_render.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      272 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/geocode.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     8689 2023-03-15 08:32:52.000000 gopro-overlay-0.94.0/gopro_overlay/gpmd.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3275 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/gpmd_calculate.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3482 2022-11-23 14:02:47.000000 gopro-overlay-0.94.0/gopro_overlay/gpmd_visitors.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3420 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/gpmd_visitors_cori.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      525 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/gpmd_visitors_debug.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     8588 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/gpmd_visitors_gps.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2859 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/gpmd_visitors_grav.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4709 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/gpmd_visitors_xyz.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2963 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/gpx.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-22 14:26:26.290604 gopro-overlay-0.94.0/gopro_overlay/icons/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2021-09-22 14:27:16.000000 gopro-overlay-0.94.0/gopro_overlay/icons/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    13448 2021-09-30 11:08:46.000000 gopro-overlay-0.94.0/gopro_overlay/icons/bicycle.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     8077 2021-09-30 11:08:22.000000 gopro-overlay-0.94.0/gopro_overlay/icons/car.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    22971 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/icons/faq.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    34059 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/icons/forbidden.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    19173 2021-09-20 15:22:09.000000 gopro-overlay-0.94.0/gopro_overlay/icons/gauge-1.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    15425 2021-09-20 15:24:33.000000 gopro-overlay-0.94.0/gopro_overlay/icons/gauge.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    12719 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/icons/gps_lock_2d.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     9239 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/icons/gps_lock_3d.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    32100 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/icons/gps_lock_none.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    28140 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/icons/gps_lock_unknown.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    13732 2021-09-21 11:34:05.000000 gopro-overlay-0.94.0/gopro_overlay/icons/heartbeat.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     5700 2021-09-30 11:09:17.000000 gopro-overlay-0.94.0/gopro_overlay/icons/ice-cream-van.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    20413 2021-09-20 15:26:49.000000 gopro-overlay-0.94.0/gopro_overlay/icons/mountain-range.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    13636 2021-09-20 15:27:04.000000 gopro-overlay-0.94.0/gopro_overlay/icons/mountain.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     8451 2022-11-06 20:16:59.000000 gopro-overlay-0.94.0/gopro_overlay/icons/power.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    14622 2021-09-20 15:58:10.000000 gopro-overlay-0.94.0/gopro_overlay/icons/ruler.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    15485 2021-09-20 15:27:45.000000 gopro-overlay-0.94.0/gopro_overlay/icons/slope-triangle.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    10147 2021-09-20 15:27:28.000000 gopro-overlay-0.94.0/gopro_overlay/icons/slope.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    15997 2021-09-20 15:22:31.000000 gopro-overlay-0.94.0/gopro_overlay/icons/speedometer-variant-tool-symbol.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     7655 2021-09-20 15:26:02.000000 gopro-overlay-0.94.0/gopro_overlay/icons/thermometer-1.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    10579 2021-09-20 15:25:42.000000 gopro-overlay-0.94.0/gopro_overlay/icons/thermometer.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    11096 2021-09-30 11:51:55.000000 gopro-overlay-0.94.0/gopro_overlay/icons/user.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     6958 2021-09-30 11:09:29.000000 gopro-overlay-0.94.0/gopro_overlay/icons/van-black-side-view.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     2074 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/journey.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3337 2023-05-06 09:06:40.000000 gopro-overlay-0.94.0/gopro_overlay/layout.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1025 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/layout_components.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    26241 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/layout_xml.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1067 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/layout_xml_attribute.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5498 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/layout_xml_cairo.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-22 14:26:26.290604 gopro-overlay-0.94.0/gopro_overlay/layouts/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2021-09-22 14:27:16.000000 gopro-overlay-0.94.0/gopro_overlay/layouts/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3294 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/layouts/default-1920x1080.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     3515 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/layouts/default-2704x1520.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     3302 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/layouts/default-3840x2160.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     1510 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/layouts/example-2.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     8388 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/layouts/example.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     3802 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/layouts/power-1920x1080.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)      145 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/log.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      736 2021-09-30 11:21:57.000000 gopro-overlay-0.94.0/gopro_overlay/models.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      294 2022-02-09 11:24:51.000000 gopro-overlay-0.94.0/gopro_overlay/parsing.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     6672 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/point.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      575 2021-09-22 14:35:02.000000 gopro-overlay-0.94.0/gopro_overlay/privacy.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      329 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/process.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      891 2022-05-21 21:20:30.000000 gopro-overlay-0.94.0/gopro_overlay/progress_frames.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2297 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/rdp.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1224 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/smoothing.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2966 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/timeseries.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3005 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/timeseries_process.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1974 2022-09-24 19:15:22.000000 gopro-overlay-0.94.0/gopro_overlay/timeunits.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1287 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/timing.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      365 2022-11-29 15:04:43.000000 gopro-overlay-0.94.0/gopro_overlay/units.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-22 14:26:26.290604 gopro-overlay-0.94.0/gopro_overlay/widgets/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2022-11-02 15:56:34.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4453 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/asi.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2121 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/bar.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-22 14:26:26.294604 gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2227 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/angle.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3671 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/annotation.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      643 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/background.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     6174 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/bordered.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      183 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/box.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3676 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/cairo.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1825 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/cap.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4190 2023-02-09 12:46:37.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/circuit.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1835 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/colour.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4777 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/ellipse.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      833 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/face.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5749 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/gauge_marker.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4184 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/gauge_round_254.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      424 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/line.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3619 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/needle.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      513 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/reading.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1923 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/scale.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      189 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/tick.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2412 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/chart.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3451 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/compass.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2226 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/compass_arrow.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      517 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/gps.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3687 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/gradient_bar.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2204 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/info.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    10811 2023-02-08 14:26:51.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/map.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      789 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/profile.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3107 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/text.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     8038 2023-05-06 09:06:40.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/widgets.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1509 2023-02-07 21:54:02.000000 gopro-overlay-0.94.0/gopro_overlay/widgets/widgets_experimental.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-22 14:26:26.286604 gopro-overlay-0.94.0/gopro_overlay.egg-info/
--rw-rw-r--   0 richja    (1000) richja    (1000)    12144 2023-05-22 14:26:26.000000 gopro-overlay-0.94.0/gopro_overlay.egg-info/PKG-INFO
--rw-rw-r--   0 richja    (1000) richja    (1000)     4192 2023-05-22 14:26:26.000000 gopro-overlay-0.94.0/gopro_overlay.egg-info/SOURCES.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)        1 2023-05-22 14:26:26.000000 gopro-overlay-0.94.0/gopro_overlay.egg-info/dependency_links.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)      132 2023-05-22 14:26:26.000000 gopro-overlay-0.94.0/gopro_overlay.egg-info/requires.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)       14 2023-05-22 14:26:26.000000 gopro-overlay-0.94.0/gopro_overlay.egg-info/top_level.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)       38 2023-05-22 14:26:26.294604 gopro-overlay-0.94.0/setup.cfg
--rw-rw-r--   0 richja    (1000) richja    (1000)     1933 2023-05-22 14:24:40.000000 gopro-overlay-0.94.0/setup.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-23 11:06:31.393513 gopro-overlay-0.95.0/
+-rw-rw-r--   0 richja    (1000) richja    (1000)    35691 2023-05-22 13:30:42.000000 gopro-overlay-0.95.0/LICENSE.md
+-rw-rw-r--   0 richja    (1000) richja    (1000)       70 2022-02-02 12:18:46.000000 gopro-overlay-0.95.0/MANIFEST.in
+-rw-rw-r--   0 richja    (1000) richja    (1000)    11380 2023-05-23 11:06:31.393513 gopro-overlay-0.95.0/PKG-INFO
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10587 2023-05-23 11:05:26.000000 gopro-overlay-0.95.0/README.md
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-23 11:06:31.377513 gopro-overlay-0.95.0/bin/
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3153 2022-05-23 15:18:05.000000 gopro-overlay-0.95.0/bin/gopro-contrib-data-extract.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1450 2022-02-03 15:47:43.000000 gopro-overlay-0.95.0/bin/gopro-cut.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    15036 2023-05-22 09:35:24.000000 gopro-overlay-0.95.0/bin/gopro-dashboard.py
+-rwxrwxr-x   0 richja    (1000) richja    (1000)      770 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/bin/gopro-debug.py
+-rwxrwxr-x   0 richja    (1000) richja    (1000)      596 2022-11-29 16:44:06.000000 gopro-overlay-0.95.0/bin/gopro-extract.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1035 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/bin/gopro-join.py
+-rwxrwxr-x   0 richja    (1000) richja    (1000)     5527 2023-05-06 09:06:40.000000 gopro-overlay-0.95.0/bin/gopro-layout.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3702 2023-05-23 10:54:25.000000 gopro-overlay-0.95.0/bin/gopro-rename.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5783 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/bin/gopro-to-csv.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3412 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/bin/gopro-to-gpx.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-23 11:06:31.385513 gopro-overlay-0.95.0/gopro_overlay/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2022-02-02 11:42:38.000000 gopro-overlay-0.95.0/gopro_overlay/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      299 2023-05-23 11:04:16.000000 gopro-overlay-0.95.0/gopro_overlay/__version__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     7063 2023-05-22 08:55:54.000000 gopro-overlay-0.95.0/gopro_overlay/arguments.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5447 2023-05-08 10:30:40.000000 gopro-overlay-0.95.0/gopro_overlay/buffering.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      690 2022-11-29 17:00:53.000000 gopro-overlay-0.95.0/gopro_overlay/common.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      207 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/counter.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      483 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/date_overlap.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      531 2023-02-07 21:58:09.000000 gopro-overlay-0.95.0/gopro_overlay/dimensions.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1719 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/entry.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)       34 2022-11-23 14:47:58.000000 gopro-overlay-0.95.0/gopro_overlay/exceptions.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1345 2023-05-06 10:59:08.000000 gopro-overlay-0.95.0/gopro_overlay/execution.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3671 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/fake.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10025 2023-05-22 09:32:45.000000 gopro-overlay-0.95.0/gopro_overlay/ffmpeg.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1285 2023-05-22 09:02:15.000000 gopro-overlay-0.95.0/gopro_overlay/ffmpeg_profile.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1803 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/filenaming.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2279 2023-05-01 11:53:38.000000 gopro-overlay-0.95.0/gopro_overlay/fit.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      122 2021-12-03 14:46:33.000000 gopro-overlay-0.95.0/gopro_overlay/font.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10542 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/framemeta.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3000 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/framemeta_gpx.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      478 2022-05-27 13:38:56.000000 gopro-overlay-0.95.0/gopro_overlay/functional.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5703 2023-02-08 14:26:51.000000 gopro-overlay-0.95.0/gopro_overlay/geo.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2426 2023-02-09 10:45:34.000000 gopro-overlay-0.95.0/gopro_overlay/geo_render.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      525 2023-05-23 10:54:25.000000 gopro-overlay-0.95.0/gopro_overlay/geocode.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8689 2023-03-15 08:32:52.000000 gopro-overlay-0.95.0/gopro_overlay/gpmd.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3275 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/gpmd_calculate.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3482 2022-11-23 14:02:47.000000 gopro-overlay-0.95.0/gopro_overlay/gpmd_visitors.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3420 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/gpmd_visitors_cori.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      525 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/gpmd_visitors_debug.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8588 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/gpmd_visitors_gps.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2859 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/gpmd_visitors_grav.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4709 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/gpmd_visitors_xyz.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2963 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/gpx.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-23 11:06:31.389513 gopro-overlay-0.95.0/gopro_overlay/icons/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2021-09-22 14:27:16.000000 gopro-overlay-0.95.0/gopro_overlay/icons/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    13448 2021-09-30 11:08:46.000000 gopro-overlay-0.95.0/gopro_overlay/icons/bicycle.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8077 2021-09-30 11:08:22.000000 gopro-overlay-0.95.0/gopro_overlay/icons/car.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    22971 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/icons/faq.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    34059 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/icons/forbidden.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    19173 2021-09-20 15:22:09.000000 gopro-overlay-0.95.0/gopro_overlay/icons/gauge-1.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    15425 2021-09-20 15:24:33.000000 gopro-overlay-0.95.0/gopro_overlay/icons/gauge.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    12719 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/icons/gps_lock_2d.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     9239 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/icons/gps_lock_3d.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    32100 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/icons/gps_lock_none.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    28140 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/icons/gps_lock_unknown.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    13732 2021-09-21 11:34:05.000000 gopro-overlay-0.95.0/gopro_overlay/icons/heartbeat.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5700 2021-09-30 11:09:17.000000 gopro-overlay-0.95.0/gopro_overlay/icons/ice-cream-van.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    20413 2021-09-20 15:26:49.000000 gopro-overlay-0.95.0/gopro_overlay/icons/mountain-range.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    13636 2021-09-20 15:27:04.000000 gopro-overlay-0.95.0/gopro_overlay/icons/mountain.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8451 2022-11-06 20:16:59.000000 gopro-overlay-0.95.0/gopro_overlay/icons/power.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    14622 2021-09-20 15:58:10.000000 gopro-overlay-0.95.0/gopro_overlay/icons/ruler.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    15485 2021-09-20 15:27:45.000000 gopro-overlay-0.95.0/gopro_overlay/icons/slope-triangle.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10147 2021-09-20 15:27:28.000000 gopro-overlay-0.95.0/gopro_overlay/icons/slope.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    15997 2021-09-20 15:22:31.000000 gopro-overlay-0.95.0/gopro_overlay/icons/speedometer-variant-tool-symbol.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     7655 2021-09-20 15:26:02.000000 gopro-overlay-0.95.0/gopro_overlay/icons/thermometer-1.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10579 2021-09-20 15:25:42.000000 gopro-overlay-0.95.0/gopro_overlay/icons/thermometer.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    11096 2021-09-30 11:51:55.000000 gopro-overlay-0.95.0/gopro_overlay/icons/user.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     6958 2021-09-30 11:09:29.000000 gopro-overlay-0.95.0/gopro_overlay/icons/van-black-side-view.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2074 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/journey.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3337 2023-05-06 09:06:40.000000 gopro-overlay-0.95.0/gopro_overlay/layout.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1025 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/layout_components.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    26241 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/layout_xml.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1067 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/layout_xml_attribute.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5498 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/layout_xml_cairo.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-23 11:06:31.389513 gopro-overlay-0.95.0/gopro_overlay/layouts/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2021-09-22 14:27:16.000000 gopro-overlay-0.95.0/gopro_overlay/layouts/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3294 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/layouts/default-1920x1080.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3515 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/layouts/default-2704x1520.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3302 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/layouts/default-3840x2160.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1510 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/layouts/example-2.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8388 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/layouts/example.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3802 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/layouts/power-1920x1080.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)      145 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/log.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      736 2021-09-30 11:21:57.000000 gopro-overlay-0.95.0/gopro_overlay/models.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      294 2022-02-09 11:24:51.000000 gopro-overlay-0.95.0/gopro_overlay/parsing.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     6672 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/point.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      575 2021-09-22 14:35:02.000000 gopro-overlay-0.95.0/gopro_overlay/privacy.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      329 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/process.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      891 2022-05-21 21:20:30.000000 gopro-overlay-0.95.0/gopro_overlay/progress_frames.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2297 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/rdp.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1224 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/smoothing.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2966 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/timeseries.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3005 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/timeseries_process.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1974 2022-09-24 19:15:22.000000 gopro-overlay-0.95.0/gopro_overlay/timeunits.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1287 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/timing.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      365 2022-11-29 15:04:43.000000 gopro-overlay-0.95.0/gopro_overlay/units.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-23 11:06:31.389513 gopro-overlay-0.95.0/gopro_overlay/widgets/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2022-11-02 15:56:34.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4453 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/asi.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2121 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/bar.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-23 11:06:31.393513 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2227 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/angle.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3671 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/annotation.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      643 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/background.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     6174 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/bordered.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      183 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/box.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3676 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/cairo.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1825 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/cap.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4190 2023-02-09 12:46:37.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/circuit.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1835 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/colour.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4777 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/ellipse.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      833 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/face.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5749 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/gauge_marker.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4184 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/gauge_round_254.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      424 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/line.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3619 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/needle.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      513 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/reading.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1923 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/scale.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      189 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/tick.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2412 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/chart.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3451 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/compass.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2226 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/compass_arrow.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      517 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/gps.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3687 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/gradient_bar.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2204 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/info.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10811 2023-02-08 14:26:51.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/map.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      789 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/profile.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3107 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/text.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8038 2023-05-06 09:06:40.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/widgets.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1509 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/widgets_experimental.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-23 11:06:31.385513 gopro-overlay-0.95.0/gopro_overlay.egg-info/
+-rw-rw-r--   0 richja    (1000) richja    (1000)    11380 2023-05-23 11:06:31.000000 gopro-overlay-0.95.0/gopro_overlay.egg-info/PKG-INFO
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4192 2023-05-23 11:06:31.000000 gopro-overlay-0.95.0/gopro_overlay.egg-info/SOURCES.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)        1 2023-05-23 11:06:31.000000 gopro-overlay-0.95.0/gopro_overlay.egg-info/dependency_links.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)      132 2023-05-23 11:06:31.000000 gopro-overlay-0.95.0/gopro_overlay.egg-info/requires.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)       14 2023-05-23 11:06:31.000000 gopro-overlay-0.95.0/gopro_overlay.egg-info/top_level.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)       38 2023-05-23 11:06:31.393513 gopro-overlay-0.95.0/setup.cfg
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1933 2023-05-23 11:04:16.000000 gopro-overlay-0.95.0/setup.py
```

### Comparing `gopro-overlay-0.94.0/LICENSE.md` & `gopro-overlay-0.95.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/PKG-INFO` & `gopro-overlay-0.95.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gopro-overlay
-Version: 0.94.0
+Version: 0.95.0
 Summary: Overlay graphics dashboards onto GoPro footage
 Home-page: https://github.com/time4tea/gopro-dashboard-overlay
 Author: James Richardson
 Author-email: james+gopro@time4tea.net
 License: MIT
 Project-URL: Source, https://github.com/time4tea/gopro-dashboard-overlay
 Classifier: Development Status :: 5 - Production/Stable
@@ -233,14 +233,15 @@
 https://github.com/progweb/gpx2video
 
 https://github.com/JuanIrache/gopro-telemetry
 
 ## Latest Changes
 
 If you find any issues with new releases, please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/discussions)
+- 0.95.0 [Feature] Add api key support for geocode.xyz - [#117](https://github.com/time4tea/gopro-dashboard-overlay/issues/117) Thanks [@mishuha](https://github.com/mishuha) for raising.
 - 0.94.0 [Change] Update docker image to python3.11/ffmpeg 6.0 
 - 0.93.0 [Feature] Support for *fully gpu* decoding/overlay/encoding. Huge performance increase now possible. It takes a bit of work, but now can render at 12x realtime. See [docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md)
   - [Breaking] Remove support for `--output-size` as it didn't really work properly anyway. 
 - 0.92.0 [Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially much faster rendering, but may not work on all architectures. Speed improvements highly dependent on `ffmpeg` performance. Likely much faster when using `--generate overlay`. Feedback welcomed.
 - 0.91.0 [Fix] Ignore FIT data items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/patkoscsaba) for raising.
 - 0.90.0 [Change] `cairo-circuit` now draws much more quickly. 
 - [Change] Map rendering caches tile images more efficiently, so draws more quickly.
@@ -248,18 +249,10 @@
 - 0.88.0 [Fix] Journey Map broke when no there were no locked GPS points in the movie.
   - Thanks [@shahargli](https://github.com/shahargli) for reporting
 - 0.87.0 [Fix/Breaking Possibly] `chart` - discovered a few bugs, now fixed. Removed `alpha`, instead use alpha of each colour.
 - 0.86.0 [Feature] New component `cairo-gauge-marker` - a nice clean gauge component, with a marker for the current value.. See docs [docs/xml/examples/06-cairo-gauge-marker](docs/xml/examples/06-cairo-gauge-marker)
 - 0.85.0 [Feature/Breaking Possibly] Add validation to attributes in layout files. This may cause some custom layouts to break! - But they wouldn't have been working as intended.
   - [Change/Breaking] Change some `zone-bar` attribute names, aiming for standardisation
   - [Change/Breaking] Change some `cairo-circuit-map` attribute names, aiming for standardisation
-- 0.84.0 [Feature] New component `zone-bar` - a 3-zone bar control that can be used for HR/Cadence/Power zones. See docs in [docs/xml/examples/07-zone-bar](docs/xml/examples/07-zone-bar)
-  - Many thanks to [@jchinte](https://github.com/jchinte) for contributing!
-- 0.83.0 [Change] No longer require --overlay-size when using --use-gpx-only, but supplying input video
-  - [Fix] Give better error message when video and GPX don't overlap in time, but told to sync 
-  - Thanks to [@mfloryan](https://github.com/mfloryan) for reporting both of these
-- 0.82.0 [Change] Support for changing units in layouts from the command line. Use `--units-speed` etc to control. Examples are in [docs/bin](docs/bin)
-  - Thanks to [@matzeruegge](https://github.com/matzeruegge) for the suggestion.
-- 0.81.0 [Fix] gopro-rename was broken when using `--dirs` - added tests so hopefully won't reoccur. Thanks to [matzeruegge](https://github.com/matzeruegge) for reporting 
 
 Older changes are in [CHANGELOG.md](CHANGELOG.md)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gopro-overlay Version: 0.94.0 Summary: Overlay
+Metadata-Version: 2.1 Name: gopro-overlay Version: 0.95.0 Summary: Overlay
 graphics dashboards onto GoPro footage Home-page: https://github.com/time4tea/
 gopro-dashboard-overlay Author: James Richardson Author-email:
 james+gopro@time4tea.net License: MIT Project-URL: Source, https://github.com/
 time4tea/gopro-dashboard-overlay Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.10
@@ -99,48 +99,38 @@
 copyright) Some Maps Â© [Thunderforest](http://www.thunderforest.com/) ##
 References https://github.com/juanmcasillas/gopro2gpx https://github.com/
 JuanIrache/gopro-telemetry https://github.com/gopro/gpmf-parser https://
 coderunner.io/how-to-compress-gopro-movies-and-keep-metadata/ ## Other Related
 Software https://github.com/progweb/gpx2video https://github.com/JuanIrache/
 gopro-telemetry ## Latest Changes If you find any issues with new releases,
 please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-
-dashboard-overlay/discussions) - 0.94.0 [Change] Update docker image to
-python3.11/ffmpeg 6.0 - 0.93.0 [Feature] Support for *fully gpu* decoding/
-overlay/encoding. Huge performance increase now possible. It takes a bit of
-work, but now can render at 12x realtime. See [docs/bin/PERFORMANCE_GUIDE.md]
-(docs/bin/PERFORMANCE_GUIDE.md) - [Breaking] Remove support for `--output-size`
-as it didn't really work properly anyway. - 0.92.0 [Feature] `--double-buffer`
-- EXPERIMENTAL double-buffering. Potentially much faster rendering, but may not
-work on all architectures. Speed improvements highly dependent on `ffmpeg`
-performance. Likely much faster when using `--generate overlay`. Feedback
-welcomed. - 0.91.0 [Fix] Ignore FIT data items that don't have a GPS location.
-[#122](https://github.com/time4tea/gopro-dashboard-overlay/issues/122) Thanks
-[@patkoscsaba](https://github.com/patkoscsaba) for raising. - 0.90.0 [Change]
-`cairo-circuit` now draws much more quickly. - [Change] Map rendering caches
-tile images more efficiently, so draws more quickly. - 0.89.0 [Feature] New
-component `cairo-gauge-round-annotated` - A bit like a car speedometer - See
-docs [docs/xml/examples/06-cairo-gauge-round-annotated](docs/xml/examples/06-
-cairo-gauge-round-annotated) - 0.88.0 [Fix] Journey Map broke when no there
-were no locked GPS points in the movie. - Thanks [@shahargli](https://
-github.com/shahargli) for reporting - 0.87.0 [Fix/Breaking Possibly] `chart` -
-discovered a few bugs, now fixed. Removed `alpha`, instead use alpha of each
-colour. - 0.86.0 [Feature] New component `cairo-gauge-marker` - a nice clean
-gauge component, with a marker for the current value.. See docs [docs/xml/
-examples/06-cairo-gauge-marker](docs/xml/examples/06-cairo-gauge-marker) -
-0.85.0 [Feature/Breaking Possibly] Add validation to attributes in layout
-files. This may cause some custom layouts to break! - But they wouldn't have
-been working as intended. - [Change/Breaking] Change some `zone-bar` attribute
-names, aiming for standardisation - [Change/Breaking] Change some `cairo-
-circuit-map` attribute names, aiming for standardisation - 0.84.0 [Feature] New
-component `zone-bar` - a 3-zone bar control that can be used for HR/Cadence/
-Power zones. See docs in [docs/xml/examples/07-zone-bar](docs/xml/examples/07-
-zone-bar) - Many thanks to [@jchinte](https://github.com/jchinte) for
-contributing! - 0.83.0 [Change] No longer require --overlay-size when using --
-use-gpx-only, but supplying input video - [Fix] Give better error message when
-video and GPX don't overlap in time, but told to sync - Thanks to [@mfloryan]
-(https://github.com/mfloryan) for reporting both of these - 0.82.0 [Change]
-Support for changing units in layouts from the command line. Use `--units-
-speed` etc to control. Examples are in [docs/bin](docs/bin) - Thanks to
-[@matzeruegge](https://github.com/matzeruegge) for the suggestion. - 0.81.0
-[Fix] gopro-rename was broken when using `--dirs` - added tests so hopefully
-won't reoccur. Thanks to [matzeruegge](https://github.com/matzeruegge) for
-reporting Older changes are in [CHANGELOG.md](CHANGELOG.md)
+dashboard-overlay/discussions) - 0.95.0 [Feature] Add api key support for
+geocode.xyz - [#117](https://github.com/time4tea/gopro-dashboard-overlay/
+issues/117) Thanks [@mishuha](https://github.com/mishuha) for raising. - 0.94.0
+[Change] Update docker image to python3.11/ffmpeg 6.0 - 0.93.0 [Feature]
+Support for *fully gpu* decoding/overlay/encoding. Huge performance increase
+now possible. It takes a bit of work, but now can render at 12x realtime. See
+[docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md) - [Breaking]
+Remove support for `--output-size` as it didn't really work properly anyway. -
+0.92.0 [Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially
+much faster rendering, but may not work on all architectures. Speed
+improvements highly dependent on `ffmpeg` performance. Likely much faster when
+using `--generate overlay`. Feedback welcomed. - 0.91.0 [Fix] Ignore FIT data
+items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-
+dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/
+patkoscsaba) for raising. - 0.90.0 [Change] `cairo-circuit` now draws much more
+quickly. - [Change] Map rendering caches tile images more efficiently, so draws
+more quickly. - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` -
+A bit like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-
+round-annotated](docs/xml/examples/06-cairo-gauge-round-annotated) - 0.88.0
+[Fix] Journey Map broke when no there were no locked GPS points in the movie. -
+Thanks [@shahargli](https://github.com/shahargli) for reporting - 0.87.0 [Fix/
+Breaking Possibly] `chart` - discovered a few bugs, now fixed. Removed `alpha`,
+instead use alpha of each colour. - 0.86.0 [Feature] New component `cairo-
+gauge-marker` - a nice clean gauge component, with a marker for the current
+value.. See docs [docs/xml/examples/06-cairo-gauge-marker](docs/xml/examples/
+06-cairo-gauge-marker) - 0.85.0 [Feature/Breaking Possibly] Add validation to
+attributes in layout files. This may cause some custom layouts to break! - But
+they wouldn't have been working as intended. - [Change/Breaking] Change some
+`zone-bar` attribute names, aiming for standardisation - [Change/Breaking]
+Change some `cairo-circuit-map` attribute names, aiming for standardisation
+Older changes are in [CHANGELOG.md](CHANGELOG.md)
```

### Comparing `gopro-overlay-0.94.0/README.md` & `gopro-overlay-0.95.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -212,14 +212,15 @@
 https://github.com/progweb/gpx2video
 
 https://github.com/JuanIrache/gopro-telemetry
 
 ## Latest Changes
 
 If you find any issues with new releases, please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/discussions)
+- 0.95.0 [Feature] Add api key support for geocode.xyz - [#117](https://github.com/time4tea/gopro-dashboard-overlay/issues/117) Thanks [@mishuha](https://github.com/mishuha) for raising.
 - 0.94.0 [Change] Update docker image to python3.11/ffmpeg 6.0 
 - 0.93.0 [Feature] Support for *fully gpu* decoding/overlay/encoding. Huge performance increase now possible. It takes a bit of work, but now can render at 12x realtime. See [docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md)
   - [Breaking] Remove support for `--output-size` as it didn't really work properly anyway. 
 - 0.92.0 [Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially much faster rendering, but may not work on all architectures. Speed improvements highly dependent on `ffmpeg` performance. Likely much faster when using `--generate overlay`. Feedback welcomed.
 - 0.91.0 [Fix] Ignore FIT data items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/patkoscsaba) for raising.
 - 0.90.0 [Change] `cairo-circuit` now draws much more quickly. 
 - [Change] Map rendering caches tile images more efficiently, so draws more quickly.
@@ -227,18 +228,10 @@
 - 0.88.0 [Fix] Journey Map broke when no there were no locked GPS points in the movie.
   - Thanks [@shahargli](https://github.com/shahargli) for reporting
 - 0.87.0 [Fix/Breaking Possibly] `chart` - discovered a few bugs, now fixed. Removed `alpha`, instead use alpha of each colour.
 - 0.86.0 [Feature] New component `cairo-gauge-marker` - a nice clean gauge component, with a marker for the current value.. See docs [docs/xml/examples/06-cairo-gauge-marker](docs/xml/examples/06-cairo-gauge-marker)
 - 0.85.0 [Feature/Breaking Possibly] Add validation to attributes in layout files. This may cause some custom layouts to break! - But they wouldn't have been working as intended.
   - [Change/Breaking] Change some `zone-bar` attribute names, aiming for standardisation
   - [Change/Breaking] Change some `cairo-circuit-map` attribute names, aiming for standardisation
-- 0.84.0 [Feature] New component `zone-bar` - a 3-zone bar control that can be used for HR/Cadence/Power zones. See docs in [docs/xml/examples/07-zone-bar](docs/xml/examples/07-zone-bar)
-  - Many thanks to [@jchinte](https://github.com/jchinte) for contributing!
-- 0.83.0 [Change] No longer require --overlay-size when using --use-gpx-only, but supplying input video
-  - [Fix] Give better error message when video and GPX don't overlap in time, but told to sync 
-  - Thanks to [@mfloryan](https://github.com/mfloryan) for reporting both of these
-- 0.82.0 [Change] Support for changing units in layouts from the command line. Use `--units-speed` etc to control. Examples are in [docs/bin](docs/bin)
-  - Thanks to [@matzeruegge](https://github.com/matzeruegge) for the suggestion.
-- 0.81.0 [Fix] gopro-rename was broken when using `--dirs` - added tests so hopefully won't reoccur. Thanks to [matzeruegge](https://github.com/matzeruegge) for reporting 
 
 Older changes are in [CHANGELOG.md](CHANGELOG.md)
```

#### html2text {}

```diff
@@ -89,48 +89,38 @@
 Â© [Thunderforest](http://www.thunderforest.com/) ## References https://
 github.com/juanmcasillas/gopro2gpx https://github.com/JuanIrache/gopro-
 telemetry https://github.com/gopro/gpmf-parser https://coderunner.io/how-to-
 compress-gopro-movies-and-keep-metadata/ ## Other Related Software https://
 github.com/progweb/gpx2video https://github.com/JuanIrache/gopro-telemetry ##
 Latest Changes If you find any issues with new releases, please discuss in
 [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/
-discussions) - 0.94.0 [Change] Update docker image to python3.11/ffmpeg 6.0 -
-0.93.0 [Feature] Support for *fully gpu* decoding/overlay/encoding. Huge
-performance increase now possible. It takes a bit of work, but now can render
-at 12x realtime. See [docs/bin/PERFORMANCE_GUIDE.md](docs/bin/
-PERFORMANCE_GUIDE.md) - [Breaking] Remove support for `--output-size` as it
-didn't really work properly anyway. - 0.92.0 [Feature] `--double-buffer` -
-EXPERIMENTAL double-buffering. Potentially much faster rendering, but may not
-work on all architectures. Speed improvements highly dependent on `ffmpeg`
-performance. Likely much faster when using `--generate overlay`. Feedback
-welcomed. - 0.91.0 [Fix] Ignore FIT data items that don't have a GPS location.
-[#122](https://github.com/time4tea/gopro-dashboard-overlay/issues/122) Thanks
-[@patkoscsaba](https://github.com/patkoscsaba) for raising. - 0.90.0 [Change]
-`cairo-circuit` now draws much more quickly. - [Change] Map rendering caches
-tile images more efficiently, so draws more quickly. - 0.89.0 [Feature] New
-component `cairo-gauge-round-annotated` - A bit like a car speedometer - See
-docs [docs/xml/examples/06-cairo-gauge-round-annotated](docs/xml/examples/06-
-cairo-gauge-round-annotated) - 0.88.0 [Fix] Journey Map broke when no there
-were no locked GPS points in the movie. - Thanks [@shahargli](https://
-github.com/shahargli) for reporting - 0.87.0 [Fix/Breaking Possibly] `chart` -
-discovered a few bugs, now fixed. Removed `alpha`, instead use alpha of each
-colour. - 0.86.0 [Feature] New component `cairo-gauge-marker` - a nice clean
-gauge component, with a marker for the current value.. See docs [docs/xml/
-examples/06-cairo-gauge-marker](docs/xml/examples/06-cairo-gauge-marker) -
-0.85.0 [Feature/Breaking Possibly] Add validation to attributes in layout
-files. This may cause some custom layouts to break! - But they wouldn't have
-been working as intended. - [Change/Breaking] Change some `zone-bar` attribute
-names, aiming for standardisation - [Change/Breaking] Change some `cairo-
-circuit-map` attribute names, aiming for standardisation - 0.84.0 [Feature] New
-component `zone-bar` - a 3-zone bar control that can be used for HR/Cadence/
-Power zones. See docs in [docs/xml/examples/07-zone-bar](docs/xml/examples/07-
-zone-bar) - Many thanks to [@jchinte](https://github.com/jchinte) for
-contributing! - 0.83.0 [Change] No longer require --overlay-size when using --
-use-gpx-only, but supplying input video - [Fix] Give better error message when
-video and GPX don't overlap in time, but told to sync - Thanks to [@mfloryan]
-(https://github.com/mfloryan) for reporting both of these - 0.82.0 [Change]
-Support for changing units in layouts from the command line. Use `--units-
-speed` etc to control. Examples are in [docs/bin](docs/bin) - Thanks to
-[@matzeruegge](https://github.com/matzeruegge) for the suggestion. - 0.81.0
-[Fix] gopro-rename was broken when using `--dirs` - added tests so hopefully
-won't reoccur. Thanks to [matzeruegge](https://github.com/matzeruegge) for
-reporting Older changes are in [CHANGELOG.md](CHANGELOG.md)
+discussions) - 0.95.0 [Feature] Add api key support for geocode.xyz - [#117]
+(https://github.com/time4tea/gopro-dashboard-overlay/issues/117) Thanks
+[@mishuha](https://github.com/mishuha) for raising. - 0.94.0 [Change] Update
+docker image to python3.11/ffmpeg 6.0 - 0.93.0 [Feature] Support for *fully
+gpu* decoding/overlay/encoding. Huge performance increase now possible. It
+takes a bit of work, but now can render at 12x realtime. See [docs/bin/
+PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md) - [Breaking] Remove
+support for `--output-size` as it didn't really work properly anyway. - 0.92.0
+[Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially much
+faster rendering, but may not work on all architectures. Speed improvements
+highly dependent on `ffmpeg` performance. Likely much faster when using `--
+generate overlay`. Feedback welcomed. - 0.91.0 [Fix] Ignore FIT data items that
+don't have a GPS location. [#122](https://github.com/time4tea/gopro-dashboard-
+overlay/issues/122) Thanks [@patkoscsaba](https://github.com/patkoscsaba) for
+raising. - 0.90.0 [Change] `cairo-circuit` now draws much more quickly. -
+[Change] Map rendering caches tile images more efficiently, so draws more
+quickly. - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` - A bit
+like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-round-
+annotated](docs/xml/examples/06-cairo-gauge-round-annotated) - 0.88.0 [Fix]
+Journey Map broke when no there were no locked GPS points in the movie. -
+Thanks [@shahargli](https://github.com/shahargli) for reporting - 0.87.0 [Fix/
+Breaking Possibly] `chart` - discovered a few bugs, now fixed. Removed `alpha`,
+instead use alpha of each colour. - 0.86.0 [Feature] New component `cairo-
+gauge-marker` - a nice clean gauge component, with a marker for the current
+value.. See docs [docs/xml/examples/06-cairo-gauge-marker](docs/xml/examples/
+06-cairo-gauge-marker) - 0.85.0 [Feature/Breaking Possibly] Add validation to
+attributes in layout files. This may cause some custom layouts to break! - But
+they wouldn't have been working as intended. - [Change/Breaking] Change some
+`zone-bar` attribute names, aiming for standardisation - [Change/Breaking]
+Change some `cairo-circuit-map` attribute names, aiming for standardisation
+Older changes are in [CHANGELOG.md](CHANGELOG.md)
```

### Comparing `gopro-overlay-0.94.0/bin/gopro-contrib-data-extract.py` & `gopro-overlay-0.95.0/bin/gopro-contrib-data-extract.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/bin/gopro-cut.py` & `gopro-overlay-0.95.0/bin/gopro-cut.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/bin/gopro-dashboard.py` & `gopro-overlay-0.95.0/bin/gopro-dashboard.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/bin/gopro-debug.py` & `gopro-overlay-0.95.0/bin/gopro-debug.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/bin/gopro-extract.py` & `gopro-overlay-0.95.0/bin/gopro-extract.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/bin/gopro-join.py` & `gopro-overlay-0.95.0/bin/gopro-join.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/bin/gopro-layout.py` & `gopro-overlay-0.95.0/bin/gopro-layout.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/bin/gopro-rename.py` & `gopro-overlay-0.95.0/bin/gopro-rename.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     parser.add_argument("file", type=pathlib.Path, nargs="+", help="The files to rename, or directory/ies containing files")
     parser.add_argument("-t", "--touch", action="store_true", help="change the modification time of the file")
     parser.add_argument("-to", "--touch-only", action="store_true", help="change the modification time of the file only - don't rename")
     parser.add_argument("--desc", help="a descriptive name to add to the filename - the filename will be yyyymmdd-hhmmss-{desc}.MP4")
     parser.add_argument("--geo", action="store_true", help="[EXPERIMENTAL] Use Geocode.xyz to add description for you (city-state) - see https://geocode.xyz/pricing for terms")
     parser.add_argument("-y", "--yes", action="store_true", help="Rename the files, don't just print what would be done")
     parser.add_argument("--dirs", action="store_true", help="Allow directory")
+    parser.add_argument("--geocode-key", help="geocode.xyz api key")
 
     args = parser.parse_args()
 
     if not args.yes:
         log("*** DRY RUN - NOT ACTUALLY DOING ANYTHING ***")
 
     inputs: List[pathlib.Path] = args.file
@@ -38,28 +39,30 @@
     potentials = functional.flatten([filenaming.gopro_files_in(path) for path in inputs])
     potentials = filter(None, potentials)
     file_list = sorted(potentials)
 
     should_touch = args.touch or args.touch_only
     should_rename = not args.touch_only
 
+    geocoder = geocode.GeoCode(key=args.geocode_key)
+
     for file in file_list:
         meta = GoproMeta.parse(ffmpeg.load_gpmd_from(file))
         found = meta.accept(DetermineFirstLockedGPSUVisitor())
         gps_datetime = found.packet_time
         if gps_datetime is None:
             log(f"Unable to determine GPS date for {file} - GPS never locked")
             continue
 
         formatted_datetime = gps_datetime.strftime("%Y%m%d-%H%M%S")
 
         if args.desc:
             new_name = f"{formatted_datetime}-{args.desc}.MP4"
         elif args.geo:
-            geojson = geocode.geocode_location(found.point.lat, found.point.lon)
+            geojson = geocoder.geocode_location(found.point.lat, found.point.lon)
             city = geojson["city"].lower()
             if "state" in geojson:
                 state = geojson["state"].lower()
             elif "region" in geojson:
                 state = geojson["region"].lower()
             elif "prov" in geojson:
                 state = geojson["prov"].lower()
```

### Comparing `gopro-overlay-0.94.0/bin/gopro-to-csv.py` & `gopro-overlay-0.95.0/bin/gopro-to-csv.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/bin/gopro-to-gpx.py` & `gopro-overlay-0.95.0/bin/gopro-to-gpx.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/arguments.py` & `gopro-overlay-0.95.0/gopro_overlay/arguments.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/buffering.py` & `gopro-overlay-0.95.0/gopro_overlay/buffering.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/common.py` & `gopro-overlay-0.95.0/gopro_overlay/common.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/dimensions.py` & `gopro-overlay-0.95.0/gopro_overlay/dimensions.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/entry.py` & `gopro-overlay-0.95.0/gopro_overlay/entry.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/execution.py` & `gopro-overlay-0.95.0/gopro_overlay/execution.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/fake.py` & `gopro-overlay-0.95.0/gopro_overlay/fake.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/ffmpeg.py` & `gopro-overlay-0.95.0/gopro_overlay/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/ffmpeg_profile.py` & `gopro-overlay-0.95.0/gopro_overlay/ffmpeg_profile.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/filenaming.py` & `gopro-overlay-0.95.0/gopro_overlay/filenaming.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/fit.py` & `gopro-overlay-0.95.0/gopro_overlay/fit.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/framemeta.py` & `gopro-overlay-0.95.0/gopro_overlay/framemeta.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/framemeta_gpx.py` & `gopro-overlay-0.95.0/gopro_overlay/framemeta_gpx.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/geo.py` & `gopro-overlay-0.95.0/gopro_overlay/geo.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/geo_render.py` & `gopro-overlay-0.95.0/gopro_overlay/geo_render.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/gpmd.py` & `gopro-overlay-0.95.0/gopro_overlay/gpmd.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/gpmd_calculate.py` & `gopro-overlay-0.95.0/gopro_overlay/gpmd_calculate.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/gpmd_visitors.py` & `gopro-overlay-0.95.0/gopro_overlay/gpmd_visitors.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/gpmd_visitors_cori.py` & `gopro-overlay-0.95.0/gopro_overlay/gpmd_visitors_cori.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/gpmd_visitors_debug.py` & `gopro-overlay-0.95.0/gopro_overlay/gpmd_visitors_debug.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/gpmd_visitors_gps.py` & `gopro-overlay-0.95.0/gopro_overlay/gpmd_visitors_gps.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/gpmd_visitors_grav.py` & `gopro-overlay-0.95.0/gopro_overlay/gpmd_visitors_grav.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/gpmd_visitors_xyz.py` & `gopro-overlay-0.95.0/gopro_overlay/gpmd_visitors_xyz.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/gpx.py` & `gopro-overlay-0.95.0/gopro_overlay/gpx.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/icons/bicycle.png` & `gopro-overlay-0.95.0/gopro_overlay/icons/bicycle.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/icons/car.png` & `gopro-overlay-0.95.0/gopro_overlay/icons/car.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/icons/faq.png` & `gopro-overlay-0.95.0/gopro_overlay/icons/faq.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/icons/forbidden.png` & `gopro-overlay-0.95.0/gopro_overlay/icons/forbidden.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/icons/gauge-1.png` & `gopro-overlay-0.95.0/gopro_overlay/icons/gauge-1.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/icons/gauge.png` & `gopro-overlay-0.95.0/gopro_overlay/icons/gauge.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/icons/gps_lock_2d.png` & `gopro-overlay-0.95.0/gopro_overlay/icons/gps_lock_2d.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/icons/gps_lock_3d.png` & `gopro-overlay-0.95.0/gopro_overlay/icons/gps_lock_3d.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/icons/gps_lock_none.png` & `gopro-overlay-0.95.0/gopro_overlay/icons/gps_lock_none.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/icons/gps_lock_unknown.png` & `gopro-overlay-0.95.0/gopro_overlay/icons/gps_lock_unknown.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/icons/heartbeat.png` & `gopro-overlay-0.95.0/gopro_overlay/icons/heartbeat.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/icons/ice-cream-van.png` & `gopro-overlay-0.95.0/gopro_overlay/icons/ice-cream-van.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/icons/mountain-range.png` & `gopro-overlay-0.95.0/gopro_overlay/icons/mountain-range.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/icons/mountain.png` & `gopro-overlay-0.95.0/gopro_overlay/icons/mountain.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/icons/power.png` & `gopro-overlay-0.95.0/gopro_overlay/icons/power.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/icons/ruler.png` & `gopro-overlay-0.95.0/gopro_overlay/icons/ruler.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/icons/slope-triangle.png` & `gopro-overlay-0.95.0/gopro_overlay/icons/slope-triangle.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/icons/slope.png` & `gopro-overlay-0.95.0/gopro_overlay/icons/slope.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/icons/speedometer-variant-tool-symbol.png` & `gopro-overlay-0.95.0/gopro_overlay/icons/speedometer-variant-tool-symbol.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/icons/thermometer-1.png` & `gopro-overlay-0.95.0/gopro_overlay/icons/thermometer-1.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/icons/thermometer.png` & `gopro-overlay-0.95.0/gopro_overlay/icons/thermometer.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/icons/user.png` & `gopro-overlay-0.95.0/gopro_overlay/icons/user.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/icons/van-black-side-view.png` & `gopro-overlay-0.95.0/gopro_overlay/icons/van-black-side-view.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/journey.py` & `gopro-overlay-0.95.0/gopro_overlay/journey.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/layout.py` & `gopro-overlay-0.95.0/gopro_overlay/layout.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/layout_components.py` & `gopro-overlay-0.95.0/gopro_overlay/layout_components.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/layout_xml.py` & `gopro-overlay-0.95.0/gopro_overlay/layout_xml.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/layout_xml_attribute.py` & `gopro-overlay-0.95.0/gopro_overlay/layout_xml_attribute.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/layout_xml_cairo.py` & `gopro-overlay-0.95.0/gopro_overlay/layout_xml_cairo.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/layouts/default-1920x1080.xml` & `gopro-overlay-0.95.0/gopro_overlay/layouts/default-1920x1080.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/layouts/default-2704x1520.xml` & `gopro-overlay-0.95.0/gopro_overlay/layouts/default-2704x1520.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/layouts/default-3840x2160.xml` & `gopro-overlay-0.95.0/gopro_overlay/layouts/default-3840x2160.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/layouts/example-2.xml` & `gopro-overlay-0.95.0/gopro_overlay/layouts/example-2.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/layouts/example.xml` & `gopro-overlay-0.95.0/gopro_overlay/layouts/example.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/layouts/power-1920x1080.xml` & `gopro-overlay-0.95.0/gopro_overlay/layouts/power-1920x1080.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/models.py` & `gopro-overlay-0.95.0/gopro_overlay/models.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/point.py` & `gopro-overlay-0.95.0/gopro_overlay/point.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/privacy.py` & `gopro-overlay-0.95.0/gopro_overlay/privacy.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/progress_frames.py` & `gopro-overlay-0.95.0/gopro_overlay/progress_frames.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/rdp.py` & `gopro-overlay-0.95.0/gopro_overlay/rdp.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/smoothing.py` & `gopro-overlay-0.95.0/gopro_overlay/smoothing.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/timeseries.py` & `gopro-overlay-0.95.0/gopro_overlay/timeseries.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/timeseries_process.py` & `gopro-overlay-0.95.0/gopro_overlay/timeseries_process.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/timeunits.py` & `gopro-overlay-0.95.0/gopro_overlay/timeunits.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/timing.py` & `gopro-overlay-0.95.0/gopro_overlay/timing.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/asi.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/asi.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/bar.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/bar.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/angle.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/angle.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/annotation.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/annotation.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/background.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/background.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/bordered.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/bordered.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/cairo.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/cairo.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/cap.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/cap.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/circuit.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/circuit.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/colour.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/colour.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/ellipse.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/ellipse.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/face.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/face.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/gauge_marker.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/gauge_marker.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/gauge_round_254.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/gauge_round_254.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/needle.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/needle.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/reading.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/reading.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/cairo/scale.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/scale.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/chart.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/chart.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/compass.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/compass.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/compass_arrow.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/compass_arrow.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/gps.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/gps.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/gradient_bar.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/gradient_bar.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/info.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/info.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/map.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/map.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/profile.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/profile.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/text.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/text.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/widgets.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/widgets.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay/widgets/widgets_experimental.py` & `gopro-overlay-0.95.0/gopro_overlay/widgets/widgets_experimental.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/gopro_overlay.egg-info/PKG-INFO` & `gopro-overlay-0.95.0/gopro_overlay.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gopro-overlay
-Version: 0.94.0
+Version: 0.95.0
 Summary: Overlay graphics dashboards onto GoPro footage
 Home-page: https://github.com/time4tea/gopro-dashboard-overlay
 Author: James Richardson
 Author-email: james+gopro@time4tea.net
 License: MIT
 Project-URL: Source, https://github.com/time4tea/gopro-dashboard-overlay
 Classifier: Development Status :: 5 - Production/Stable
@@ -233,14 +233,15 @@
 https://github.com/progweb/gpx2video
 
 https://github.com/JuanIrache/gopro-telemetry
 
 ## Latest Changes
 
 If you find any issues with new releases, please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/discussions)
+- 0.95.0 [Feature] Add api key support for geocode.xyz - [#117](https://github.com/time4tea/gopro-dashboard-overlay/issues/117) Thanks [@mishuha](https://github.com/mishuha) for raising.
 - 0.94.0 [Change] Update docker image to python3.11/ffmpeg 6.0 
 - 0.93.0 [Feature] Support for *fully gpu* decoding/overlay/encoding. Huge performance increase now possible. It takes a bit of work, but now can render at 12x realtime. See [docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md)
   - [Breaking] Remove support for `--output-size` as it didn't really work properly anyway. 
 - 0.92.0 [Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially much faster rendering, but may not work on all architectures. Speed improvements highly dependent on `ffmpeg` performance. Likely much faster when using `--generate overlay`. Feedback welcomed.
 - 0.91.0 [Fix] Ignore FIT data items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/patkoscsaba) for raising.
 - 0.90.0 [Change] `cairo-circuit` now draws much more quickly. 
 - [Change] Map rendering caches tile images more efficiently, so draws more quickly.
@@ -248,18 +249,10 @@
 - 0.88.0 [Fix] Journey Map broke when no there were no locked GPS points in the movie.
   - Thanks [@shahargli](https://github.com/shahargli) for reporting
 - 0.87.0 [Fix/Breaking Possibly] `chart` - discovered a few bugs, now fixed. Removed `alpha`, instead use alpha of each colour.
 - 0.86.0 [Feature] New component `cairo-gauge-marker` - a nice clean gauge component, with a marker for the current value.. See docs [docs/xml/examples/06-cairo-gauge-marker](docs/xml/examples/06-cairo-gauge-marker)
 - 0.85.0 [Feature/Breaking Possibly] Add validation to attributes in layout files. This may cause some custom layouts to break! - But they wouldn't have been working as intended.
   - [Change/Breaking] Change some `zone-bar` attribute names, aiming for standardisation
   - [Change/Breaking] Change some `cairo-circuit-map` attribute names, aiming for standardisation
-- 0.84.0 [Feature] New component `zone-bar` - a 3-zone bar control that can be used for HR/Cadence/Power zones. See docs in [docs/xml/examples/07-zone-bar](docs/xml/examples/07-zone-bar)
-  - Many thanks to [@jchinte](https://github.com/jchinte) for contributing!
-- 0.83.0 [Change] No longer require --overlay-size when using --use-gpx-only, but supplying input video
-  - [Fix] Give better error message when video and GPX don't overlap in time, but told to sync 
-  - Thanks to [@mfloryan](https://github.com/mfloryan) for reporting both of these
-- 0.82.0 [Change] Support for changing units in layouts from the command line. Use `--units-speed` etc to control. Examples are in [docs/bin](docs/bin)
-  - Thanks to [@matzeruegge](https://github.com/matzeruegge) for the suggestion.
-- 0.81.0 [Fix] gopro-rename was broken when using `--dirs` - added tests so hopefully won't reoccur. Thanks to [matzeruegge](https://github.com/matzeruegge) for reporting 
 
 Older changes are in [CHANGELOG.md](CHANGELOG.md)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gopro-overlay Version: 0.94.0 Summary: Overlay
+Metadata-Version: 2.1 Name: gopro-overlay Version: 0.95.0 Summary: Overlay
 graphics dashboards onto GoPro footage Home-page: https://github.com/time4tea/
 gopro-dashboard-overlay Author: James Richardson Author-email:
 james+gopro@time4tea.net License: MIT Project-URL: Source, https://github.com/
 time4tea/gopro-dashboard-overlay Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.10
@@ -99,48 +99,38 @@
 copyright) Some Maps Â© [Thunderforest](http://www.thunderforest.com/) ##
 References https://github.com/juanmcasillas/gopro2gpx https://github.com/
 JuanIrache/gopro-telemetry https://github.com/gopro/gpmf-parser https://
 coderunner.io/how-to-compress-gopro-movies-and-keep-metadata/ ## Other Related
 Software https://github.com/progweb/gpx2video https://github.com/JuanIrache/
 gopro-telemetry ## Latest Changes If you find any issues with new releases,
 please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-
-dashboard-overlay/discussions) - 0.94.0 [Change] Update docker image to
-python3.11/ffmpeg 6.0 - 0.93.0 [Feature] Support for *fully gpu* decoding/
-overlay/encoding. Huge performance increase now possible. It takes a bit of
-work, but now can render at 12x realtime. See [docs/bin/PERFORMANCE_GUIDE.md]
-(docs/bin/PERFORMANCE_GUIDE.md) - [Breaking] Remove support for `--output-size`
-as it didn't really work properly anyway. - 0.92.0 [Feature] `--double-buffer`
-- EXPERIMENTAL double-buffering. Potentially much faster rendering, but may not
-work on all architectures. Speed improvements highly dependent on `ffmpeg`
-performance. Likely much faster when using `--generate overlay`. Feedback
-welcomed. - 0.91.0 [Fix] Ignore FIT data items that don't have a GPS location.
-[#122](https://github.com/time4tea/gopro-dashboard-overlay/issues/122) Thanks
-[@patkoscsaba](https://github.com/patkoscsaba) for raising. - 0.90.0 [Change]
-`cairo-circuit` now draws much more quickly. - [Change] Map rendering caches
-tile images more efficiently, so draws more quickly. - 0.89.0 [Feature] New
-component `cairo-gauge-round-annotated` - A bit like a car speedometer - See
-docs [docs/xml/examples/06-cairo-gauge-round-annotated](docs/xml/examples/06-
-cairo-gauge-round-annotated) - 0.88.0 [Fix] Journey Map broke when no there
-were no locked GPS points in the movie. - Thanks [@shahargli](https://
-github.com/shahargli) for reporting - 0.87.0 [Fix/Breaking Possibly] `chart` -
-discovered a few bugs, now fixed. Removed `alpha`, instead use alpha of each
-colour. - 0.86.0 [Feature] New component `cairo-gauge-marker` - a nice clean
-gauge component, with a marker for the current value.. See docs [docs/xml/
-examples/06-cairo-gauge-marker](docs/xml/examples/06-cairo-gauge-marker) -
-0.85.0 [Feature/Breaking Possibly] Add validation to attributes in layout
-files. This may cause some custom layouts to break! - But they wouldn't have
-been working as intended. - [Change/Breaking] Change some `zone-bar` attribute
-names, aiming for standardisation - [Change/Breaking] Change some `cairo-
-circuit-map` attribute names, aiming for standardisation - 0.84.0 [Feature] New
-component `zone-bar` - a 3-zone bar control that can be used for HR/Cadence/
-Power zones. See docs in [docs/xml/examples/07-zone-bar](docs/xml/examples/07-
-zone-bar) - Many thanks to [@jchinte](https://github.com/jchinte) for
-contributing! - 0.83.0 [Change] No longer require --overlay-size when using --
-use-gpx-only, but supplying input video - [Fix] Give better error message when
-video and GPX don't overlap in time, but told to sync - Thanks to [@mfloryan]
-(https://github.com/mfloryan) for reporting both of these - 0.82.0 [Change]
-Support for changing units in layouts from the command line. Use `--units-
-speed` etc to control. Examples are in [docs/bin](docs/bin) - Thanks to
-[@matzeruegge](https://github.com/matzeruegge) for the suggestion. - 0.81.0
-[Fix] gopro-rename was broken when using `--dirs` - added tests so hopefully
-won't reoccur. Thanks to [matzeruegge](https://github.com/matzeruegge) for
-reporting Older changes are in [CHANGELOG.md](CHANGELOG.md)
+dashboard-overlay/discussions) - 0.95.0 [Feature] Add api key support for
+geocode.xyz - [#117](https://github.com/time4tea/gopro-dashboard-overlay/
+issues/117) Thanks [@mishuha](https://github.com/mishuha) for raising. - 0.94.0
+[Change] Update docker image to python3.11/ffmpeg 6.0 - 0.93.0 [Feature]
+Support for *fully gpu* decoding/overlay/encoding. Huge performance increase
+now possible. It takes a bit of work, but now can render at 12x realtime. See
+[docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md) - [Breaking]
+Remove support for `--output-size` as it didn't really work properly anyway. -
+0.92.0 [Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially
+much faster rendering, but may not work on all architectures. Speed
+improvements highly dependent on `ffmpeg` performance. Likely much faster when
+using `--generate overlay`. Feedback welcomed. - 0.91.0 [Fix] Ignore FIT data
+items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-
+dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/
+patkoscsaba) for raising. - 0.90.0 [Change] `cairo-circuit` now draws much more
+quickly. - [Change] Map rendering caches tile images more efficiently, so draws
+more quickly. - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` -
+A bit like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-
+round-annotated](docs/xml/examples/06-cairo-gauge-round-annotated) - 0.88.0
+[Fix] Journey Map broke when no there were no locked GPS points in the movie. -
+Thanks [@shahargli](https://github.com/shahargli) for reporting - 0.87.0 [Fix/
+Breaking Possibly] `chart` - discovered a few bugs, now fixed. Removed `alpha`,
+instead use alpha of each colour. - 0.86.0 [Feature] New component `cairo-
+gauge-marker` - a nice clean gauge component, with a marker for the current
+value.. See docs [docs/xml/examples/06-cairo-gauge-marker](docs/xml/examples/
+06-cairo-gauge-marker) - 0.85.0 [Feature/Breaking Possibly] Add validation to
+attributes in layout files. This may cause some custom layouts to break! - But
+they wouldn't have been working as intended. - [Change/Breaking] Change some
+`zone-bar` attribute names, aiming for standardisation - [Change/Breaking]
+Change some `cairo-circuit-map` attribute names, aiming for standardisation
+Older changes are in [CHANGELOG.md](CHANGELOG.md)
```

### Comparing `gopro-overlay-0.94.0/gopro_overlay.egg-info/SOURCES.txt` & `gopro-overlay-0.95.0/gopro_overlay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.94.0/setup.py` & `gopro-overlay-0.95.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 test_requirements = [
     "pytest"
 ]
 
 setup(
     name="gopro-overlay",
-    version="0.94.0",
+    version="0.95.0",
     description="Overlay graphics dashboards onto GoPro footage",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/time4tea/gopro-dashboard-overlay",
     author="James Richardson",
     author_email="james+gopro@time4tea.net",
     license="MIT",
```

