# Comparing `tmp/cellbrowser-1.2.3.tar.gz` & `tmp/cellbrowser-v0.4.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellbrowser-1.2.3.tar", last modified: Tue May 23 21:20:15 2023, max compression
+gzip compressed data, was "dist/cellbrowser-v0.4.27.tar", last modified: Mon Dec 17 16:26:39 2018, max compression
```

## Comparing `cellbrowser-1.2.3.tar` & `cellbrowser-v0.4.27.tar`

### file list

```diff
@@ -1,199 +1,124 @@
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2023-05-23 21:20:15.000000 cellbrowser-1.2.3/
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2023-05-23 21:20:13.000000 cellbrowser-1.2.3/src/
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2023-05-23 21:20:13.000000 cellbrowser-1.2.3/src/cbPyLib/
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2023-05-23 21:20:13.000000 cellbrowser-1.2.3/src/cbPyLib/RangeHTTPServer/
--rwxrwxr-x   0 chmalee  (30024) genecats  (1305)     3663 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/RangeHTTPServer/__init__.py
--rwxrwxr-x   0 chmalee  (30024) genecats  (1305)      594 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/RangeHTTPServer/__main__.py
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2023-05-23 21:20:15.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2023-05-23 21:20:13.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/R/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    18520 2023-01-23 21:01:33.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/R/cellbrowser.R
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2023-05-23 21:20:13.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2023-05-23 21:20:13.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/css/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    68260 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/css/MaterialIcons-Regular.eot
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    68255 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/css/MaterialIcons-Regular.ttf
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    57620 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/css/MaterialIcons-Regular.woff
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    65874 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/css/MaterialIcons-Regular.woff2
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    14275 2023-01-23 21:01:33.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/css/cellBrowser.css
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2023-05-23 21:20:14.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2023-05-23 21:20:14.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/images/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)       86 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-bg_flat_0_aaaaaa_40x100.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     3266 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_444444_256x240.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     3274 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_555555_256x240.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     3262 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_777620_256x240.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     3266 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_777777_256x240.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     3262 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_cc0000_256x240.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     3264 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_ffffff_256x240.png
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2023-05-23 21:20:13.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2023-05-23 21:20:13.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2023-05-23 21:20:14.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2023-05-23 21:20:14.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/example/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      480 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/example/d3-random-matrix.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    32231 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/example/example.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      717 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/example/gradients.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      350 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/example/package.json
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2023-05-23 21:20:14.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/hex/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     2561 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/hex/inferno.json
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     2561 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/hex/magma.json
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     2561 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/hex/plasma.json
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     2561 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/hex/viridis.json
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2023-05-23 21:20:14.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/rgb/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     8707 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/rgb/inferno.json
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     8709 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/rgb/magma.json
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     8707 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/rgb/plasma.json
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     8707 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/rgb/viridis.json
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2023-05-23 21:20:14.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/utils/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      232 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/utils/hex2rgb.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      998 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/utils/interpolate.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      438 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/utils/rgb2hex.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)       13 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/.npmignore
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      757 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/LICENSE
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      182 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/Makefile
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     2673 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/README.md
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      160 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/browser.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      226 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/build.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      110 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/inferno.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      108 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/magma.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     2741 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/package.json
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      109 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/plasma.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      110 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/temp/node_modules/scale-color-perceptual/viridis.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)   211133 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/Chart.bundle.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    14199 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/FastBitSet.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     3365 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/FileSaver.1.1.20151003.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    19452 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/OverlayScrollbars.min.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     3823 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap-dropmenu.min.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     4772 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap-submenu.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     5057 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap-submenu.min.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)   121200 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap.3.3.7.min.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)   121155 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap.min.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    37045 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    30319 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/chartjs-chart-box-and-violin-plot.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      538 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/chosen-sprite.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      777 2022-05-13 20:50:10.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/chosen-sprite@2x.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    10058 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/chosen.1.8.2.min.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    29004 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/chosen.jquery.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     3447 2023-01-23 21:01:33.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/drawImage-clipper.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    27231 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/font-awesome.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      494 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/googleMaterialIcons.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     8545 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/hamster.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    23408 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/intro.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     9960 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/introjs.2.4.0.min.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    35973 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/jquery-ui-1.12.1.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)   253668 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/jquery-ui.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    86709 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.3.1.1.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     6668 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.contextMenu.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    90609 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.contextMenu.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    17797 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.event.drag-2.3.0.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    41643 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.overlayScrollbars.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    43247 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.sparkline.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     1440 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.tipsy.1.0.3.min.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     6845 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.tipsy.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     5855 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.ui.position.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     6416 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/jsurl2.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    16032 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/lz-string.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    64000 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/materialIcons.woff
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)  1320211 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/minified.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     4862 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/mousetrap.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    10395 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/normalizeWheel.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    23234 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/pako_inflate.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    60211 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/palette.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    16713 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/papaparse.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    76717 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/reorder.v1.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    14269 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/scaleColorPerceptual.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    45130 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/science.v1.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    15196 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/select2.4.0.4.min.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    66604 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/select2.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    10947 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/selectize.bootstrap3.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)   106428 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/selectize.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     1784 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/slick.cellrangedecorator.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     5050 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/slick.cellrangeselector.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     5791 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/slick.cellselectionmodel.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    17618 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/slick.core.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    16723 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/slick.editors.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     3329 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/slick.examples.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     1802 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/slick.formatters.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     4595 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/slick.grid.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)   172843 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/slick.grid.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    11595 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/spectrum-1.8.0.css
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    41928 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/spectrum.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    20835 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/split.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     7038 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/tablesort.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      541 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/tablesort.number.min.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      917 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/tiny-queue.js
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2023-05-23 21:20:14.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/genes/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      372 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/genes/files.json
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)  5012383 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/genes/hg19.gc34.tsv
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)   636974 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/genes/hg19.json.gz
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)  5290936 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/genes/hg38.gc34.tsv
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)   691255 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/genes/hg38.json.gz
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      310 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/genes/log.txt
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     2259 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/genes/makeGenes.py
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)   592310 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/genes/mm10.json.gz
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)  3666259 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/genes/mm10.vm25.tsv
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2023-05-23 21:20:14.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2023-05-23 21:20:15.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     1612 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/README.txt
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      284 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/gtk-justify-left.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      583 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/gtk-save.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)       27 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/log.txt
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      646 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-center-16.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     1065 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-center-24.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      561 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-controller-16.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      825 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-controller-24.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      523 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-edit-16.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      386 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-gravity-west-24.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      682 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-info-16.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     1047 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-info-24.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      615 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-merge-down-16.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      565 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-scale-16.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      586 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-free-select-16.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      814 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-free-select-22.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      598 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-move-16.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      776 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-move-22.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      455 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-rect-select-16.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      443 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-rect-select-22.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      594 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-zoom-16.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      754 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-zoom-22.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)       41 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/README.md
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     1065 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/center.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      598 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/icons8-help-32.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      222 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/info.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      814 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/lasso.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      140 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/marker.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      776 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/move.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      443 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/select.png
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      754 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/zoom.png
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2023-05-23 21:20:15.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/js/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    63992 2023-01-23 21:01:33.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/js/cbData.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)   305074 2023-05-23 21:09:35.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/js/cellBrowser.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    19293 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/js/maxHeat.js
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    91870 2023-05-23 21:09:35.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/js/maxPlot.js
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2023-05-23 21:20:15.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/sampleConfig/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     7964 2023-05-23 21:09:35.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/sampleConfig/cellbrowser.conf
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     2615 2023-05-23 21:09:35.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/sampleConfig/desc.conf
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     2166 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/sampleConfig/hub.conf
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     3112 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/sampleConfig/scanpy.conf
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      978 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/sampleConfig/seurat.conf
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      456 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/sampleConfig/summary.html
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      126 2022-05-13 19:19:20.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/__init__.py
--rwxrwxr-x   0 chmalee  (30024) genecats  (1305)   270603 2023-05-23 21:09:35.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cellbrowser.py
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    30769 2023-05-23 21:09:35.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/convert.py
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    18221 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/download.py
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    14389 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/geneinfo.py
--rwxrwxr-x   0 chmalee  (30024) genecats  (1305)    22096 2023-05-23 21:09:35.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/genes.py
--rwxrwxr-x   0 chmalee  (30024) genecats  (1305)    44506 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/hubmaker.py
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    24901 2023-01-23 21:01:33.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/seurat.py
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      497 2023-05-23 21:20:15.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser/_version.py
-drwxrwxr-x   0 chmalee  (30024) genecats  (1305)        0 2023-05-23 21:20:13.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser.egg-info/
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     1523 2023-05-23 21:20:11.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser.egg-info/PKG-INFO
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    10033 2023-05-23 21:20:11.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser.egg-info/SOURCES.txt
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)        1 2023-05-23 21:20:11.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser.egg-info/dependency_links.txt
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      602 2023-05-23 21:20:11.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser.egg-info/entry_points.txt
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)        1 2022-05-13 21:01:59.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser.egg-info/not-zip-safe
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)       28 2023-05-23 21:20:11.000000 cellbrowser-1.2.3/src/cbPyLib/cellbrowser.egg-info/top_level.txt
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    35147 2022-05-13 19:19:19.000000 cellbrowser-1.2.3/LICENSE
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      614 2022-05-13 19:19:19.000000 cellbrowser-1.2.3/MANIFEST.in
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     6539 2023-01-23 21:13:18.000000 cellbrowser-1.2.3/README.rst
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)      221 2023-05-23 21:20:15.000000 cellbrowser-1.2.3/setup.cfg
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     3207 2023-01-23 21:01:33.000000 cellbrowser-1.2.3/setup.py
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)    68611 2022-05-13 19:19:21.000000 cellbrowser-1.2.3/versioneer.py
--rw-rw-r--   0 chmalee  (30024) genecats  (1305)     1523 2023-05-23 21:20:15.000000 cellbrowser-1.2.3/PKG-INFO
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/
+-rw-rw-r--   0 max       (1501) protein   (1304)     2234 2018-12-17 15:44:55.000000 cellbrowser-v0.4.27/setup.py
+-rw-rw-r--   0 max       (1501) protein   (1304)     1102 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/PKG-INFO
+-rw-rw-r--   0 max       (1501) protein   (1304)      994 2018-12-17 16:16:51.000000 cellbrowser-v0.4.27/README.rst
+-rw-rw-r--   0 max       (1501) protein   (1304)    68611 2018-12-07 13:51:58.000000 cellbrowser-v0.4.27/versioneer.py
+-rw-rw-r--   0 max       (1501) protein   (1304)      217 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/setup.cfg
+-rw-rw-r--   0 max       (1501) protein   (1304)      566 2018-12-07 13:51:59.000000 cellbrowser-v0.4.27/MANIFEST.in
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/
+-rwxrwxr-x   0 max       (1501) protein   (1304)      341 2018-11-21 10:54:55.000000 cellbrowser-v0.4.27/src/cbScanpy
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/RangeHTTPServer/
+-rwxrwxr-x   0 max       (1501) protein   (1304)     3663 2018-08-17 12:09:51.000000 cellbrowser-v0.4.27/src/cbPyLib/RangeHTTPServer/__init__.py
+-rwxrwxr-x   0 max       (1501) protein   (1304)      594 2018-08-17 12:09:51.000000 cellbrowser-v0.4.27/src/cbPyLib/RangeHTTPServer/__main__.py
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser.egg-info/
+-rw-rw-r--   0 max       (1501) protein   (1304)     5590 2018-12-17 16:26:38.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser.egg-info/SOURCES.txt
+-rw-rw-r--   0 max       (1501) protein   (1304)     1101 2018-12-17 16:26:38.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser.egg-info/PKG-INFO
+-rw-rw-r--   0 max       (1501) protein   (1304)        1 2018-12-17 16:26:38.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser.egg-info/dependency_links.txt
+-rw-rw-r--   0 max       (1501) protein   (1304)       28 2018-12-17 16:26:38.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser.egg-info/top_level.txt
+-rw-rw-r--   0 max       (1501) protein   (1304)      525 2018-12-17 16:26:38.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser.egg-info/entry_points.txt
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/html/
+-rw-rw-r--   0 max       (1501) protein   (1304)     2573 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/html/index.html
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/
+-rw-rw-r--   0 max       (1501) protein   (1304)     5855 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.ui.position.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)     9481 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/selectize.0.12.4.min.css
+-rw-rw-r--   0 max       (1501) protein   (1304)    15196 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/select2.4.0.4.min.css
+-rw-rw-r--   0 max       (1501) protein   (1304)   121155 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap.min.css
+-rw-rw-r--   0 max       (1501) protein   (1304)    20835 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/split.js
+-rw-rw-r--   0 max       (1501) protein   (1304)      538 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/chosen-sprite.png
+-rw-rw-r--   0 max       (1501) protein   (1304)    29004 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/chosen.jquery.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)    90609 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.contextMenu.js
+-rw-rw-r--   0 max       (1501) protein   (1304)      494 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/googleMaterialIcons.css
+-rw-rw-r--   0 max       (1501) protein   (1304)     3365 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/FileSaver.1.1.20151003.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)    23408 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/intro.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)     6668 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.contextMenu.css
+-rw-rw-r--   0 max       (1501) protein   (1304)    23234 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/pako_inflate.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)     4862 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/mousetrap.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)     3823 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap-dropmenu.min.css
+-rw-rw-r--   0 max       (1501) protein   (1304)     8545 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/hamster.js
+-rw-rw-r--   0 max       (1501) protein   (1304)   211133 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/Chart.bundle.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)     1440 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.tipsy.1.0.3.min.css
+-rw-rw-r--   0 max       (1501) protein   (1304)    35973 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery-ui-1.12.1.css
+-rw-rw-r--   0 max       (1501) protein   (1304)    10395 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/normalizeWheel.js
+-rw-rw-r--   0 max       (1501) protein   (1304)      541 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/tablesort.number.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)   253668 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery-ui.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)     4772 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap-submenu.js
+-rw-rw-r--   0 max       (1501) protein   (1304)    64000 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/materialIcons.woff
+-rw-rw-r--   0 max       (1501) protein   (1304)    16713 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/papaparse.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)     7038 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/tablesort.js
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/
+-rw-rw-r--   0 max       (1501) protein   (1304)     3262 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_cc0000_256x240.png
+-rw-rw-r--   0 max       (1501) protein   (1304)       86 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-bg_flat_0_aaaaaa_40x100.png
+-rw-rw-r--   0 max       (1501) protein   (1304)     3266 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_777777_256x240.png
+-rw-rw-r--   0 max       (1501) protein   (1304)     3262 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_777620_256x240.png
+-rw-rw-r--   0 max       (1501) protein   (1304)     3274 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_555555_256x240.png
+-rw-rw-r--   0 max       (1501) protein   (1304)     3264 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_ffffff_256x240.png
+-rw-rw-r--   0 max       (1501) protein   (1304)     3266 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_444444_256x240.png
+-rw-rw-r--   0 max       (1501) protein   (1304)    30319 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/chartjs-chart-box-and-violin-plot.js
+-rw-rw-r--   0 max       (1501) protein   (1304)     5057 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap-submenu.min.css
+-rw-rw-r--   0 max       (1501) protein   (1304)    45139 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/selectize.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)    41928 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/spectrum.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)    11595 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/spectrum-1.8.0.css
+-rw-rw-r--   0 max       (1501) protein   (1304)    60211 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/palette.js
+-rw-rw-r--   0 max       (1501) protein   (1304)    66604 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/select2.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)    43247 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.sparkline.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)    86709 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.3.1.1.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)     9960 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/introjs.2.4.0.min.css
+-rw-rw-r--   0 max       (1501) protein   (1304)   121200 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap.3.3.7.min.css
+-rw-rw-r--   0 max       (1501) protein   (1304)    10058 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/chosen.1.8.2.min.css
+-rw-rw-r--   0 max       (1501) protein   (1304)    14199 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/FastBitSet.js
+-rw-rw-r--   0 max       (1501) protein   (1304)     6845 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.tipsy.min.js
+-rw-rw-r--   0 max       (1501) protein   (1304)    27231 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/font-awesome.css
+-rw-rw-r--   0 max       (1501) protein   (1304)    37045 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap.min.js
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/
+-rw-rw-r--   0 max       (1501) protein   (1304)      443 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/select.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      140 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/marker.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      814 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/lasso.png
+-rw-rw-r--   0 max       (1501) protein   (1304)     1065 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/center.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      776 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/move.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      754 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/zoom.png
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/
+-rw-rw-r--   0 max       (1501) protein   (1304)     1612 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/README.txt
+-rw-rw-r--   0 max       (1501) protein   (1304)      615 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-merge-down-16.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      565 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-scale-16.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      586 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-free-select-16.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      561 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-controller-16.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      583 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/gtk-save.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      825 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-controller-24.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      594 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-zoom-16.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      284 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/gtk-justify-left.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      754 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-zoom-22.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      443 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-rect-select-22.png
+-rw-rw-r--   0 max       (1501) protein   (1304)     1047 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-info-24.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      646 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-center-16.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      523 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-edit-16.png
+-rw-rw-r--   0 max       (1501) protein   (1304)       27 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/log.txt
+-rw-rw-r--   0 max       (1501) protein   (1304)      682 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-info-16.png
+-rw-rw-r--   0 max       (1501) protein   (1304)     1065 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-center-24.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      386 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-gravity-west-24.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      455 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-rect-select-16.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      598 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-move-16.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      776 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-move-22.png
+-rw-rw-r--   0 max       (1501) protein   (1304)      814 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-free-select-22.png
+-rw-rw-r--   0 max       (1501) protein   (1304)       41 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/README.md
+-rw-rw-r--   0 max       (1501) protein   (1304)      222 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/info.png
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/css/
+-rw-rw-r--   0 max       (1501) protein   (1304)     9258 2018-12-06 15:18:38.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/css/cellBrowser.css
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/js/
+-rw-rw-r--   0 max       (1501) protein   (1304)   160782 2018-12-12 16:03:21.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/js/cellBrowser.js
+-rw-rw-r--   0 max       (1501) protein   (1304)    24701 2018-10-28 23:47:29.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/js/cbData.js
+-rw-rw-r--   0 max       (1501) protein   (1304)    64150 2018-10-29 00:23:00.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/js/maxPlot.js
+-rwxrwxr-x   0 max       (1501) protein   (1304)    36845 2018-11-28 12:06:04.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/hubmaker.py
+-rwxrwxr-x   0 max       (1501) protein   (1304)     3597 2018-10-12 14:24:25.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/guessgenes.py
+-rw-rw-r--   0 max       (1501) protein   (1304)      126 2018-12-07 13:51:59.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/__init__.py
+-rw-rw-r--   0 max       (1501) protein   (1304)    16960 2018-12-17 15:08:51.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/seurat.py
+-rw-rw-r--   0 max       (1501) protein   (1304)    17914 2018-12-17 13:09:30.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/convert.py
+-rw-rw-r--   0 max       (1501) protein   (1304)      499 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/_version.py
+-rwxrwxr-x   0 max       (1501) protein   (1304)   128622 2018-12-07 16:05:22.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cellbrowser.py
+drwxrwxr-x   0 max       (1501) protein   (1304)        0 2018-12-17 16:26:39.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/sampleConfig/
+-rw-rw-r--   0 max       (1501) protein   (1304)      697 2018-11-15 11:23:14.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/sampleConfig/seurat.conf
+-rw-rw-r--   0 max       (1501) protein   (1304)     3641 2018-11-23 18:46:31.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/sampleConfig/cellbrowser.conf
+-rw-rw-r--   0 max       (1501) protein   (1304)     2129 2018-12-06 16:01:46.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/sampleConfig/scanpy.conf
+-rw-rw-r--   0 max       (1501) protein   (1304)    15089 2018-11-29 15:25:30.000000 cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/geneinfo.py
```

### Comparing `cellbrowser-1.2.3/src/cbPyLib/RangeHTTPServer/__init__.py` & `cellbrowser-v0.4.27/src/cbPyLib/RangeHTTPServer/__init__.py`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/RangeHTTPServer/__main__.py` & `cellbrowser-v0.4.27/src/cbPyLib/RangeHTTPServer/__main__.py`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/css/cellBrowser.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/css/cellBrowser.css`

 * *Files 20% similar despite different names*

```diff
@@ -1,116 +1,46 @@
 /* tsneViewer.js class definitions */
 /* * {padding: 0; margin: 0} */ /* important, otherwise precise placement is impossible */ 
 /* body { font-family: Roboto, sans-serif } */
 body { font-family: Arial,Helvetica,sans-serif; overflow:hidden; line-height:1.0}
 canvas { user-select: none }
 
-section { font-weight: bold; padding-top: 5px; padding-bottom: 5px }
-
-#tpExprViewTitle { 
-        background-color: #eee;
-        padding: 3px;
-        /*border-bottom: 1px solid black; */
-}
-
-#tpExprView { 
-        position: absolute;
-        z-index: 100;
-        top: 1%;
-        left: 1%;
-        display: block;
-        background-color: white;
-        height: 98%;
-        width: 98%;
-        border: 1px solid grey;
-}
-
-#tpLegendBar { 
-        cursor:default; 
-        padding-left: 2px; 
-        border-left: 1px solid #D7D7D7; 
-        height:100%;
-}
-
-.tpDatasetPane { 
-        padding: 5px !important; 
-        padding-left: 10px !important; 
-        overflow: hidden;
-        line-height: 120%; 
-}
-
-#mpTitle {
-    cursor : default;
-    left : 8px;
-    width : max-content;
-    display : block;
-    position : absolute;
-    font-size : 16px;
-    color: white;
-    text-shadow:
-       1px 1px 0 #000,
-     -1px -1px 0 #000,  
-      1px -1px 0 #000,
-      -1px 1px 0 #000,
-       1px 1px 0 #000;
-}
+#tpLegendBar { cursor:default; overflow-y: scroll; padding-left: 2px; border-left: 1px solid #D7D7D7; height:100%}
 
 .tpLegend { font-size:13px; /* border: 2px solid transparent; */ cursor:default; word-wrap: break-word; clear:both}
 .tpHint { font-weight:normal; line-height:1.4; font-size: 80%}
 #tpLegendHeader { background-color:#eee; color: #777 }
-#tpLegendTitle { font-weight: bold }
-#tpLegendSubTitle { font-size: 80%; font-style: italic }
-#tpLegendCol1 { padding-left: 1px}
+#tpLegendCol1 { padding-left: 2px}
 #tpLegendCol2 { float: right; padding-right: 2px}
 .tpLegendSelect { outline: 2px solid black }
 .tpLegendLabel { display:inline; user-select: none; }
 /*.tpLegendCount { display:inline-block; position: absolute; right: 4px; color: #888} */
 .tpLegendCount { display:inline-block; float: right; color: #888} 
-.tpLegend .tpLegendCheckbox { margin-right: 2px; margin-top: 2px}
 .tpGrey { color: #bbb }
 
 .ui-helper-reset { font-size: 12px}
-.ui-tabs { padding: 0 }
-.ui-tabs { padding: 0 }
+.ui-tabs { padding: 0 !important}
+.ui-tabs { padding:0 !important}
 .ui-tabs-nav { border: 0 } /* color control should not be separated from tabs */
-.ui-tabs .ui-tabs-panel { padding-top:5px; border:1px solid lightgray; padding:0} /* for marker panels */
-.ui-tabs-anchor { padding: 3px }
+.ui-tabs .ui-tabs-panel { padding-top:5px; border:1px solid lightgray !important; padding:0} /* for marker panels */
+.ui-tabs-anchor { padding: 3px !important}
 .ui-tabs .ui-tabs-nav .ui-tabs-anchor { padding: 3px }
-
 .tab-pane { padding: .4em 1em; border: 1px solid lightgrey }
 .ui-corner-all { border-radius: 0px } /* dialogs */
 #tpOpenDatasetButton { border-radius: 4px }
 .ui-menu-item { font-size:13px }
 .ui-menu .ui-menu-item-wrapper { padding: 1px 1em 1px .4em; }
 .ui-tooltip { font-size: 13px }
-#tpButtonInfo { height: 24px; top: 1px; margin-right: 8px; width: 120px; border-radius: 4px }
-.tpDialogInput { margin-left: 12px; margin-top: 5px; margin-bottom: 12px; }
-
 .tpIconButton { padding: 1px 2px 1px 2px; border-radius: 0; height:28px; width: 28px; cursor: default}
 .tpClicked { background-color: #AAA }
 .tpClicked:hover { background-color: #AAA }
-.btn-primary.load-dataset {float: right; margin-left: 10px; color: white; font-size: 12px; margin-top: -4px;}
+.btn-primary.load-dataset {float: right; margin-left: 10px; color: white;}
 .list-group-item.active>.btn-primary {color: #337ab7;background-color: #fff;}
-.list-group-item .badge {margin-top: -2px;}
 
-.link,
-.tpDatasetPane a { 
-        text-decoration: underline; 
-        color: #0000EE; 
-        cursor: pointer; 
-}
-
-.tpDatasetPane {
-        padding-top: 10px !important;
-        border-radius: 4px;
-}
-
-.tpDatasetPane h4 {
-        margin-top: 0;
-}
+.link { text-decoration: underline; color: #0000EE; cursor: pointer; }
 
 /* modify bootstrap tooltip defaults */
 .tooltip-inner { min-width: 220px; border-radius: 0}
 
  .ui-widget-header { background: white} 
 .ui-state-active { background: green }
 
@@ -120,123 +50,28 @@
 .tpProgressLabel {
     position: absolute;
     left: 40%;
     top: 4px;
     font-weight: bold;
 }
 
-.context-menu-item { 
-        font-size: 13px; 
-        padding: 3px 
-}
-
-.contextmenu-customwidth { 
-        width: 200px !important; 
-        min-width: 200px !important
-}
-
-/* .tpGeneTable { 
-        table-layout: fixed; 
-        white-space: nowrap; 
-        border-collapse:collapse 
-}
-*/
-
-.tpGeneBarCell { 
-        font-size: 12px; 
-        color: black; 
-        padding-left:1px; 
-        padding-right:1px; 
-        border: 1px solid #AAA;
-        background: #F6;
-        /*color:#AAAAAA; */
-        display: inline-block;
-}
-
-.tpGeneBarCellSelected { 
-        outline: 1px solid black 
-}
-
-#tpPeakListTitle { 
-        padding-top: 8px;
-        padding-bottom: 6px;
-        padding-left: 3px;
-}
-
-#tpPeakList { 
-        border-top: 1px solid #CCC; 
-        border-bottom: 1px solid #CCC; 
-        border-left: 1px solid #CCC; 
-        margin-left: 4px;
-        padding: 3px;
-        padding-left: 4px;
-        background-color: #EEE;
-        height: 30%;
-        overflow-y: scroll;
-}
-
-.tpPeak > label {
-        font-weight: normal;
-}
-
-#tpPeakList > div { 
-        background-color: #EEE;
-}
-
-input[type=checkbox], input[type=radio] {
-        vertical-align : -2px; // https://stackoverflow.com/a/2806786/233871
-}
-
+.context-menu-item { font-size: 13px; padding: 3px }
+.contextmenu-customwidth { width: 200px !important; min-width: 200px !important}
+.tpGeneBarCell { font-size: 12px; width:58px; color: black; padding-left:1px; padding-right:1px; border: 1px solid #AAA; max-width: 80px; background: #DDDDDD; color:#AAAAAA }
+.tpGeneBarCellSelected { outline: 2px solid black}
+#tpGeneTable { table-layout: fixed; background-color: #EEE; white-space: nowrap; border-collapse:collapse }
 
 .tpSidebarHeader { font-weight: bold; padding-left: 4px; font-size: 16px; padding-top: 4px; height: 25px; background-color: white; text-align: center}
-
-#tpLeftSidebar { 
-        border-right: 1px solid #D7D7D7; 
-        height: 100%
-}
-#tpLeftSidebar .ui-tabs-anchor {
-        /* jquery UI tabs label */
-        font-size: 14px
-}
-
+#tpLeftSidebar { overflow-y:scroll; border-right: 1px solid #D7D7D7; height: 100%}
 #tpSideMeta { padding-left: 2px}
-
-#tpMetaPanel { 
-        background-color: white;
-        height: 100%;
-        overflow-y: auto;
-}
-
-#tpLegendRows {
-        width: 100%;
-        overflow-y: auto;
-        /* height: 100%; */
-}
-
-#tpLegendContent { 
-        width: 100%;
-        height: 100%;
-        overflow-y: scroll;
-}
-
-#tpLeftTabs { 
-        border: 0; 
-        height: 100%;
-}
-
-#tpGeneTab, #tpAnnotTab { 
-        border-top: 1px solid #AAA;
-        padding:0;
-        padding-top: 5px;
-        height: 100%;
-        overflow-y: scroll;
-}
+#tpMetaPanel { background-color: white}
+#tpLeftTabs { border: 0}
+#tpGeneTab, #tpAnnotTab { border-top: 1px solid #AAA; padding:0; padding-top: 5px }
 
 .tpMetaBox { font-size: 13px; cursor:default; overflow:hidden }
-.tpMetaHover { color: #FFF; background-color: #666}
 .tpMetaLabel { font-weight: bold; padding-left: 2px}
 .tpMetaLabelGrey { color: #666666}
 .tpMetaMultiVal { font-style: italic; color: gray }
 .tpMetaHistLabel { text-decoration: underline; color: blue }
 .tpMetaValue { height: 1.3em; margin-left: 8px; padding-left: 3px; background-color:#EEE; }
 .tpMetaSelect { outline: 2px solid black; background-color: #DEDEDE }
 .tpMetaValueSelect { background-color: #CCC}
@@ -268,16 +103,14 @@
 .sp-preview { height: 17px; width: 18px; border: none }
 .sp-dd { line-height: 11px; display:none }
 
 /* make bootstrap's navbar smaller */
 .navbar-xs { min-height:28px; height: 28px; }
 .navbar-xs .navbar-brand{ padding: 0px 12px;font-size: 16px;line-height: 28px; }
 .navbar-xs .navbar-nav > li > a {  padding-top: 0px; padding-bottom: 0px; line-height: 28px; }
-/* bootstraps badges are too dark */
-.list-group-item.active>.badge { background-color: darkgrey; color:white }
 /* bootstrap's small buttons have a lot of padding, for the toolbar, that's too much */
 .noPad {padding:0 2 0 2}
 
 /* make the navbar dividers smaller */
 .half-rule { 
     margin-left: 0;
     text-align: left;
@@ -307,45 +140,40 @@
         background: linear-gradient(#fff 20%,#f6f6f6 50%,#eee 52%,#f4f4f4 100%);
         padding: 2px
 }
 /* and selectize */
 .selectize-input {
         border-radius: 0;
         background: linear-gradient(#fff 20%,#f6f6f6 50%,#eee 52%,#f4f4f4 100%);
-        padding: 3px 3px;
+        padding: 2px;
         padding-left: 5px;
         overflow: visible; /* grrr!! otherwise baseline is ignored in tpToolBarItem */
-        min-height: 0px;
 }
 #tpToolBar > div.selectize-control.tpCombo.single {
         border-color: #aaaaaa;
         display: inline-block;
 }
 
 /* for links in the open dataset dialog */
 .ui-widget-content .tab-content a { color: blue !important; text-decoration: underline; }
 
 /* make bootstrap look more like jquery tabs */
-.nav-tabs > li.active > a { 
-        background-color: transparent; 
-        border:0;
-        color : black;
-}
+.nav-tabs>li.active>a { background-color: lightblue}
 
 .gradientBackground { background-color: #f6f6f6 }
 
 .selectize-control.single .selectize-input { background: none; background-color: #f6f6f6 }
 .selectize-input { background: none; background-color: #f6f6f6; box-shadow: none }
 
 /* make bootstrap's navbar show menus on mouse hover */
 /* ul.nav li.dropdown:hover > ul.dropdown-menu { display: block; } */
 
 /* flying-sheep's suggestions */
 .ui-dialog-titlebar { border: none }
-a.list-group-item { background-color: #EEE }
+button.list-group-item { background-color: #EEE }
 .nav-tabs > li > a { border-top-left-radius: 4px; border-top-right-radius: 4px; background-color: #EEE; padding-left: 10px; padding-right: 10px; padding-top: 4px; padding-bottom:4px}
 .nav-tabs > li.active > a { background-color: #337ab7; color: white; border: 1px solid #EEE }
 /* .nav-tabs > li { background-color: #E9E9E9 } */
 .ui-corner-all { border-radius: 4px }
 .nav-tabs > li > a:hover { background-color: #EEE;}
 .nav-tabs > li.active > a:hover  { background-color: #397cba; color: white }
 .nav-tabs > li.active > a:focus  { background-color: #397cba; color: white }
@@ -356,14 +184,15 @@
 .nav-tabs>li.active>a:hover { background-color: #DDD; color: black ; }
 .nav-tabs>li>a:focus { background-color: #DDD; color: black ; }
 .nav-tabs>li.active>a:focus { background-color: #DDD; color: black ; }
 */
 
 .chosen-container-single .chosen-single { box-shadow: none; background: none; background-color: #f6f6f6 }
 
+
 /* ----- FOR SORTTABLE.JS ------- */
 th[role=columnheader]:not(.no-sort) {
         cursor: pointer;
 }
 
 th[role=columnheader]:not(.no-sort):after {
         content: '';
@@ -390,78 +219,8 @@
         opacity: 0.4;
 }
 
 th[role=columnheader]:not(.no-sort):hover:after {
         visibility: visible;
         opacity: 1;
 }
-
 /* END: ----- FOR SORTTABLE.JS ------- */
-
-.ui-resizable-n {
-        cursor : row-resize;
-}
-.ui-resizable-handle:hover {
-        opacity : 0.5;
-        background-color: grey;
-
-}
-
-#tpOpenDialogTabs > ul > li  {
-        /*  !important here is the right choice. cannot use ID, cannot get specificty high enough with classes
-        // Read: https://css-tricks.com/when-using-important-is-the-right-choice/ */
-        border: 1px solid #D7D7D7 !important; 
-        border-radius: 4px !important ;
-        font-size: 14px !important; 
-        font-weight: bold !important;
-        line-height: 120% !important; 
-}
-
-.tpDatasetTab.ui-tabs-anchor{ 
-        /*  !important here is the right choice. cannot use ID, cannot get specificty high enough with classes
-        // Read: https://css-tricks.com/when-using-important-is-the-right-choice/ */
-        overflow:hidden !important; 
-        padding: 5px !important; 
-}
-
-
-/* obscure bugfix: https://stackoverflow.com/questions/31584544/jquery-ui-dialog-on-resizing-shrinks-the-content-of-the-dialog */
-.ui-dialog, .ui-dialog-content {
-    box-sizing: content-box;
-}
-
-/* for google material icons, http://google.github.io/material-design-icons/#icon-font-for-the-web */
-@font-face {
-  font-family: 'Material Icons';
-  font-style: normal;
-  font-weight: 400;
-  src: url(MaterialIcons-Regular.eot); /* For IE6-8 */
-  src: local('Material Icons'),
-    local('MaterialIcons-Regular'),
-    url(MaterialIcons-Regular.woff2) format('woff2'),
-    url(MaterialIcons-Regular.woff) format('woff'),
-    url(MaterialIcons-Regular.ttf) format('truetype');
-}
-.material-icons {
-  font-family: 'Material Icons';
-  font-weight: normal;
-  font-style: normal;
-  font-size: 24px;  /* Preferred icon size */
-  display: inline-block;
-  line-height: 1;
-  text-transform: none;
-  letter-spacing: normal;
-  word-wrap: normal;
-  white-space: nowrap;
-  direction: ltr;
-
-  /* Support for all WebKit browsers. */
-  -webkit-font-smoothing: antialiased;
-  /* Support for Safari and Chrome. */
-  text-rendering: optimizeLegibility;
-
-  /* Support for Firefox. */
-  -moz-osx-font-smoothing: grayscale;
-
-  /* Support for IE. */
-  font-feature-settings: 'liga';
-}
```

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_444444_256x240.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_555555_256x240.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_777620_256x240.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_777777_256x240.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_cc0000_256x240.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_ffffff_256x240.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/Chart.bundle.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/Chart.bundle.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/FastBitSet.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/FastBitSet.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/FileSaver.1.1.20151003.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/FileSaver.1.1.20151003.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap-dropmenu.min.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap-dropmenu.min.css`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap-submenu.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap-submenu.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap-submenu.min.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap-submenu.min.css`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap.3.3.7.min.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap.3.3.7.min.css`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap.min.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/chartjs-chart-box-and-violin-plot.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/chartjs-chart-box-and-violin-plot.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/chosen-sprite.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/chosen-sprite.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/chosen.1.8.2.min.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/chosen.1.8.2.min.css`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/chosen.jquery.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/chosen.jquery.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/font-awesome.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/font-awesome.css`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/hamster.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/hamster.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/intro.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/intro.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/introjs.2.4.0.min.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/introjs.2.4.0.min.css`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/jquery-ui-1.12.1.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery-ui-1.12.1.css`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/jquery-ui.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.3.1.1.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.3.1.1.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.contextMenu.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.contextMenu.css`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.contextMenu.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.contextMenu.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.sparkline.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.sparkline.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.tipsy.1.0.3.min.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.tipsy.1.0.3.min.css`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.tipsy.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.tipsy.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.ui.position.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/jquery.ui.position.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/materialIcons.woff` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/materialIcons.woff`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/mousetrap.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/mousetrap.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/normalizeWheel.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/normalizeWheel.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/pako_inflate.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/pako_inflate.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/palette.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/palette.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/papaparse.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/papaparse.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/select2.4.0.4.min.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/select2.4.0.4.min.css`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/select2.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/select2.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/spectrum-1.8.0.css` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/spectrum-1.8.0.css`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/spectrum.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/spectrum.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/split.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/split.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/tablesort.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/tablesort.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/ext/tablesort.number.min.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/ext/tablesort.number.min.js`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/README.txt` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/README.txt`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/gtk-save.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/gtk-save.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-center-16.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-center-16.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-center-24.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/center.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-controller-16.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-controller-16.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-controller-24.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-controller-24.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-edit-16.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-edit-16.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-info-16.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-info-16.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-info-24.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-info-24.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-merge-down-16.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-merge-down-16.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-scale-16.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-scale-16.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-free-select-16.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-free-select-16.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-free-select-22.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/lasso.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-move-16.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-move-16.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-move-22.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/move.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-zoom-16.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-zoom-16.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-zoom-22.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/zoom.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/center.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-center-24.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/lasso.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-free-select-22.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/move.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-move-22.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/img/zoom.png` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/img/gimpFlat/stock-tool-zoom-22.png`

 * *Files identical despite different names*

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/js/cellBrowser.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/js/cellBrowser.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -1,425 +1,209 @@
 // A viewer for (x,y) scatter plots of small circles
 // shows associated meta data (usually key->val attributes, one mapping per circle)
 // and expression data (string -> float, one mapping per circle)
 
 /* jshint -W097 */
-/* jshint -W117 */ // don't complain about unknown classes, like Set()
-/* jshint -W104 */ // allow 'const'
-/* jshint -W069 */ // object access with ["xx"]
-
-/* TODO:
- * - status bug - reset last expression array when coloring by meta */
-
 "use strict";
 
-var cellbrowser = function() {
+var tsnePlot = function() {
     var db = null; // the cbData object from cbData.js. Loads coords,
     // annotations and gene expression vectors
 
-    var gVersion = "$VERSION$"; // cellbrowser.py:copyStatic will replace this with the pip version or git release
+    var gDatasetList = null; // array of dataset descriptions (objects)
+
+    var gVersion = "0.3";
     var gCurrentCoordName = null; // currently shown coordinates
 
     // object with all information needed to map to the legend colors
     var gLegend = null;
-
-    // optional second legend, for split screen mode
-    var gOtherLegend = null;
-
     // all info about the current legend. gLegend.rows is:
     // [ colorHexStr, defaultColorHexStr, label, count, internalKey, uniqueKey ]
     // internalKey can be int or str, depending on current coloring mode.
     // E.g. in meta coloring, it's the metadata string value.
     // When doing expression coloring, it's the expression bin index.
     // uniqueKey is used to save manually defined colors to localStorage
 
     var renderer = null;
-
-    var background = null;
-
-    // last 10 genes
-    var gRecentGenes = [];
+    var gWinInfo = null; // .width and .height of the PIXI canvas
 
     // -- CONSTANTS
     var gTitle = "UCSC Cell Browser";
-    var COL_PREFIX = "col_";
-
-    var gOpenDataset = null; // while navigating the open dataset dialog, this contains the current name
-    // it's a global variable as the dialog is not a class (yet?) and it's the only piece of data
-    // it is a subset of dataset.json , e.g. name, description, cell count, etc.
+    const COL_PREFIX = "col_";
 
     // depending on the type of data, single cell or bulk RNA-seq, we call a circle a
     // "sample" or a "cell". This will adapt help menus, menus, etc.
     var gSampleDesc = "cell";
 
     // width of left meta bar in pixels
-    var metaBarWidth = 250;
+    var metaBarWidth = 200;
     // margin between left meta bar and drawing canvas
     var metaBarMargin = 0;
     // width of legend, pixels
     var legendBarWidth = 200;
     var legendBarMargin = 0;
     // width of the metaBar tooltip (histogram)
     var metaTipWidth = 400;
     // height of pull-down menu bar at the top, in pixels
     var menuBarHeight = null; // defined at runtime by div.height
     // height of the toolbar, in pixels
     var toolBarHeight = 28;
     // position of first combobox in toolbar from left, in pixels
     var toolBarComboLeft = metaBarWidth;
     var toolBarComboTop = 2;
-    // width of the collection combobox
-    var collectionComboWidth = 200;
-    var layoutComboWidth = 200;
-    // width of a single gene cell in the meta gene bar tables
-    //var gGeneCellWidth = 66;
+    var datasetComboWidth = 200;
+    var layoutComboWidth = 150;
 
     // height of bottom gene bar
     var geneBarHeight = 100;
     var geneBarMargin = 5;
     // color for missing value when coloring by expression value
     //var cNullColor = "CCCCCC";
     //const cNullColor = "DDDDDD";
-    //const cNullColor = "95DFFF"; //= light blue
-    const cNullColor = "e1f6ff"; //= light blue
+    const cNullColor = "87CEFA";
 
-    const cDefGradPalette = "tol-sq-blue"; // default legend gradient palette for gene expression
-    // this is a special palette, tol-sq with the first entry being a light blue, so 0 stands out a bit more
-    const cDefGradPaletteHeat = "tol-sq"; // default legend gradient palette for the heatmap
+    const cDefGradPalette = "tol-sq"; // default legend gradient palette for numeric ranges
     const cDefQualPalette = "rainbow"; // default legend palette for categorical values
 
-    var datasetGradPalette = cDefGradPalette;
-    var datasetQualPalette = cDefQualPalette;
-
-
     const exprBinCount = 10; //number of expression bins for genes
-    // has to match cbData.js.exprBinCount - TODO - share the constant between these two files
 
     var HIDELABELSNAME = "Hide labels";
     var SHOWLABELSNAME = "Show labels";
-    var METABOXTITLE = "By Annotation";
+    var METABOXTITLE = "Cell Annotations";
 
     // maximum number of distinct values that one can color on
-    const MAXCOLORCOUNT = 500;
+    const MAXCOLORCOUNT = 200;
 
     // histograms show only the top X values and summarize the rest into "other"
     var HISTOCOUNT = 12;
     // the sparkline is a bit shorter
     var SPARKHISTOCOUNT = 12;
 
     // links to various external databases
     var dbLinks = {
-        "HPO": "https://hpo.jax.org/app/browse/gene/", // entrez ID
+        "HPO": "http://compbio.charite.de/hpoweb/showterm?gene=", // entrez ID
         "OMIM": "https://omim.org/entry/", // OMIM ID
         "COSMIC": "http://cancer.sanger.ac.uk/cosmic/gene/analysis?ln=", // gene symbol
         "SFARI": "https://gene.sfari.org/database/human-gene/", // gene symbol
         "BrainSpLMD": "http://www.brainspan.org/lcm/search?exact_match=true&search_type=gene&search_term=", // entrez
         "BrainSpMouseDev": "http://developingmouse.brain-map.org/gene/show/", // internal Brainspan ID
         "Eurexp": "http://www.eurexpress.org/ee/databases/assay.jsp?assayID=", // internal ID
         "LMD": "http://www.brainspan.org/lcm/search?exact_match=true&search_type=gene&search_term=" // entrez
-    };
+    }
 
     var DEBUG = true;
 
     function _dump(o) {
         /* for debugging */
         console.log(JSON.stringify(o));
     }
 
-    function formatString(str) {
-        /* Stackoverflow code https://stackoverflow.com/a/18234317/233871 */
-        /* "a{0}bcd{1}ef".formatUnicorn("foo", "bar"); // yields "aFOObcdBARef" */
-        if (arguments.length) {
-            var t = typeof arguments[0];
-            var key;
-            var args = ("string" === t || "number" === t) ?
-                Array.prototype.slice.call(arguments) :
-                arguments[0];
-
-            for (key in args) {
-                str = str.replace(new RegExp("\\{" + key + "\\}", "gi"), args[key]);
-            }
-        }
-        return str;
-    }
-
-    // Median of medians: https://en.wikipedia.org/wiki/Median_of_medians
-    // find median in an unsorted array, worst-case complexity O(n).
-    // from https://gist.github.com/wlchn/ee15de1da59b8d6981a400eee4376ea4
-    const selectMedian = (arr, compare) => {
-        return _selectK(arr, Math.floor(arr.length / 2), compare);
-    };
-
-    const _selectK = (arr, k, compare) => {
-        if (!Array.isArray(arr) || arr.length === 0 || arr.length - 1 < k) {
-            return;
-        }
-        if (arr.length === 1) {
-            return arr[0];
-        }
-        let idx = _selectIdx(arr, 0, arr.length - 1, k, compare || _defaultCompare);
-        return arr[idx];
-    };
-
-    const _partition = (arr, left, right, pivot, compare) => {
-        let temp = arr[pivot];
-        arr[pivot] = arr[right];
-        arr[right] = temp;
-        let track = left;
-        for (let i = left; i < right; i++) {
-            // if (arr[i] < arr[right]) {
-            if (compare(arr[i], arr[right]) === -1) {
-                let t = arr[i];
-                arr[i] = arr[track];
-                arr[track] = t;
-                track++;
-            }
-        }
-        temp = arr[track];
-        arr[track] = arr[right];
-        arr[right] = temp;
-        return track;
-    };
-
-    const _selectIdx = (arr, left, right, k, compare) => {
-        if (left === right) {
-            return left;
-        }
-        let dest = left + k;
-        while (true) {
-            let pivotIndex =
-                right - left + 1 <= 5 ?
-                Math.floor(Math.random() * (right - left + 1)) + left :
-                _medianOfMedians(arr, left, right, compare);
-            pivotIndex = _partition(arr, left, right, pivotIndex, compare);
-            if (pivotIndex === dest) {
-                return pivotIndex;
-            } else if (pivotIndex < dest) {
-                left = pivotIndex + 1;
-            } else {
-                right = pivotIndex - 1;
-            }
-        }
-    };
-
-    const _medianOfMedians = (arr, left, right, compare) => {
-        let numMedians = Math.ceil((right - left) / 5);
-        for (let i = 0; i < numMedians; i++) {
-            let subLeft = left + i * 5;
-            let subRight = subLeft + 4;
-            if (subRight > right) {
-                subRight = right;
-            }
-            let medianIdx = _selectIdx(arr, subLeft, subRight, Math.floor((subRight - subLeft) / 2), compare);
-            let temp = arr[medianIdx];
-            arr[medianIdx] = arr[left + i];
-            arr[left + i] = temp;
-        }
-        return _selectIdx(arr, left, left + numMedians - 1, Math.floor(numMedians / 2), compare);
-    };
-
-    const _defaultCompare = (a, b) => {
-        return a < b ? -1 : a > b ? 1 : 0;
-    };
-    // End median of medians
-
     function debug(msg, args) {
         if (DEBUG) {
             console.log(formatString(msg, args));
         }
     }
 
     function warn(msg) {
         alert(msg);
     }
 
-    function getById(query) {
-        return document.getElementById(query);
-    }
-
     function cloneObj(d) {
         /* returns a copy of an object, wasteful */
         // see http://stackoverflow.com/questions/122102/what-is-the-most-efficient-way-to-deep-clone-an-object-in-javascript
         return JSON.parse(JSON.stringify(d));
     }
 
     function cloneArray(a) {
         /* returns a copy of an array */
         return a.slice();
     }
 
-    function copyNonNull(srcArr, trgArr) {
-        /* copy non-null values to trgArr */
-        if (srcArr.length !== trgArr.length)
-            alert("warning - copyNonNull - target and source array have different sizes.");
-
-        for (var i = 0; i < srcArr.length; i++) {
-            if (srcArr[i] !== null)
-                trgArr[i] = srcArr[i];
-        }
-        return trgArr;
-    }
-
-    function isEmpty(obj) {
-        for (var key in obj) {
-            if (obj.hasOwnProperty(key))
-                return false;
-        }
-        return true;
-    }
-
-    function allEmpty(arr) {
-        /* return true if all members of array are white space only strings */
-        var newArr = arr.filter(function(str) {
-            return /\S/.test(str);
-        });
-        return (newArr.length === 0);
-    }
-
-    function copyNonEmpty(srcArr, trgArr) {
-        /* copy from src to target array if value is not "". Just return trgArr is srcArr is null or lengths don't match.  */
-        if (!srcArr || (srcArr.length !== trgArr.length))
-            return trgArr;
-
-        for (var i = 0; i < srcArr.length; i++) {
-            if (srcArr[i] !== "")
-                trgArr[i] = srcArr[i];
-        }
-        return trgArr;
-    }
-
     function keys(o) {
-        /* return all keys of object as an array */
+        /* return all keys of object */
         var allKeys = [];
         for (var k in o) allKeys.push(k);
         return allKeys;
     }
 
-    function trackEvent(eventName, eventLabel) {
-        /* send an event to google analytics */
-        if (typeof gtag !== 'function')
-            return;
-        gtag('event', eventName, eventLabel);
-    }
-
-    function trackEventObj(eventName, obj) {
-        /* send an event obj to google analytics */
-        if (typeof gtag !== 'function')
-            return;
-        gtag('event', obj);
-    }
-
-    function classAddListener(className, type, listener) {
-        /* add an event listener for all elements of a class */
-        var els = document.getElementsByClassName(className);
-        for (let el of els) {
-            el.addEventListener(type, listener);
-        }
-    }
-
     function capitalize(s) {
         return s[0].toUpperCase() + s.slice(1);
     }
 
-    function cleanString(s) {
-        /* make sure that string only contains normal characters. Good when printing something that may contain
-         * dangerous ones */
-        if (s === undefined)
-            return undefined;
-        return s.replace(/[^0-9a-zA-Z _-]/g, '');
-    }
-
-    function cleanStrings(inArr) {
-        /* cleanString on arrays */
-        var outArr = [];
-        for (var i = 0; i < inArr.length; i++) {
-            var s = inArr[i];
-            outArr.push(cleanString(s));
+    function findMetaInfo(findName) {
+        /* return meta info field with name, add 'metaIndex' attribute  */
+        var metaFieldInfo = db.conf.metaFields;
+        for (var i = 0; i < metaFieldInfo.length; i++) {
+            var metaInfo = metaFieldInfo[i];
+            if (metaInfo.name === findName) {
+                metaInfo.index = i;
+                return metaInfo;
+            }
         }
-        return outArr;
+        return null;
     }
 
-    function findMetaValIndex(metaInfo, value) {
+    function findMetaValIndex(fieldIdx, value) {
         /* return the index of the value of an enum meta field */
-        var valCounts = metaInfo.valCounts;
+        var valCounts = db.conf.metaFields[fieldIdx].valCounts;
         for (var valIdx = 0; valIdx < valCounts.length; valIdx++) {
             if (valCounts[valIdx][0] === value)
                 return valIdx;
         }
     }
 
-    function intersectArrays(arrList) {
-        /* return the intersection of all arrays as an array. Non-IE11? */
-        var smallSet = new Set(arrList[0]);
-        for (var i = 1; i < arrList.length; i++) {
-            var otherSet = new Set(arrList[i]);
-            smallSet = new Set([...smallSet].filter(x => otherSet.has(x)));
-        }
-        var newArr = Array.from(smallSet);
-        // alternative without spread:
-        //function intersection(setA, setB) {
-        //  var _intersection = new Set();
-        //  for (var elem of setB) {
-        //      if (setA.has(elem)) {
-        //          _intersection.add(elem);
-        //      }
-        //  }
-        //  return _intersection;
-        //}
-        return newArr;
-    }
-
-    function saveToUrl(key, value, defaultValue) {
+    function cartSave(key, value, defaultValue) {
         /* save a value in both localStorage and the URL. If the value is defaultValue or null, remove it */
         if (value === defaultValue || value === null) {
             localStorage.removeItem(key);
             delState(key);
         } else {
             localStorage.setItem(key, value);
             addStateVar(key, value);
         }
     }
 
-    function getFromUrl(key, defaultValue) {
+    function cartGet(key, defaultValue) {
         /* get a value from localStorage or the current URL or return the default if not defined in either place.
          * The URL overrides localStorage. */
-        var val = getVar(key);
-        if (val !== undefined)
-            return val;
-
-        val = localStorage.getItem(key);
-        if (val === null)
-            return defaultValue
-        else
-            return val;
+        var val = localStorage.getItem(key);
+        if (val === null && defaultValue !== undefined)
+            val = defaultValue;
+        val = getVar(key, val);
+        return val
     }
 
-    function getBaseUrl() {
-        /* return URL of current page, without args or query part */
-        var myUrl = window.location.href;
-        myUrl = myUrl.replace("#", "");
-        var urlParts = myUrl.split("?");
-        var baseUrl = urlParts[0];
-        return baseUrl;
+    function formatString(str) {
+        /* Stackoverflow code https://stackoverflow.com/a/18234317/233871 */
+        /* "a{0}bcd{1}ef".formatUnicorn("foo", "bar"); // yields "aFOObcdBARef" */
+        if (arguments.length) {
+            var t = typeof arguments[0];
+            var key;
+            var args = ("string" === t || "number" === t) ?
+                Array.prototype.slice.call(arguments) :
+                arguments[0];
+
+            for (key in args) {
+                str = str.replace(new RegExp("\\{" + key + "\\}", "gi"), args[key]);
+            }
+        }
+        return str;
     }
 
     function copyToClipboard(element) {
         /* https://stackoverflow.com/questions/22581345/click-button-copy-to-clipboard-using-jquery */
         var $temp = $("<input>");
         $("body").append($temp);
         $temp.val($(element).text()).select();
         document.execCommand("copy");
         $temp.remove();
     }
 
     function iWantHue(n) {
         /* a palette as downloaded from iwanthue.com - not sure if this is better. Ellen likes it */
-        if (n > 30)
-            return null;
-
         var colList = ["7e4401", "244acd", "afc300", "a144cb", "00a13e",
             "f064e5", "478700", "727eff", "9ed671", "b6006c", "5fdd90", "f8384b",
             "00b199", "bb000f", "0052a3", "fcba56", "005989", "c57000", "7a3a78",
             "ccca76", "ff6591", "265e1c", "ff726c", "7b8550", "923223", "9a7e00",
             "ffa9ad", "5f5300", "ff9d76", "b3885f"
         ];
         var colList2 = ["cd6a00", "843dc3", "c9cd31", "eda3ff", "854350"];
@@ -433,15 +217,14 @@
         var ttOpt = {
             "html": true,
             "animation": false,
             "delay": {
                 "show": 350,
                 "hide": 100
             },
-            "trigger": "hover",
             container: "body"
         };
         $(selector).bsTooltip(ttOpt);
     }
 
     function menuBarHide(idStr) {
         /* hide a menu bar selector */
@@ -449,18 +232,36 @@
     }
 
     function menuBarShow(idStr) {
         /* show a menu bar entry given its selector */
         $(idStr).parent().removeClass("disabled").css("pointer-events", '');
     }
 
+    function updateToolbar() {
+        /* update the toolbar with the current dataset info */
+        var geneList = [];
+
+        for (var key in gCurrentDataset.matrixOffsets) {
+            geneList.push({
+                id: key,
+                text: key
+            });
+        }
+
+        //$('#tpGeneCombo').select2({
+        //placeholder : "Gene Symbol",
+        //ajax : {},
+        //dataAdapter : RefAdapter,
+        //});
+    }
+
     function updateMenu() {
         /* deactivate menu options based on current variables */
         // the "hide selected" etc menu options are only shown if some cells are selected
-        if (renderer.selCells.length === 0) {
+        if (renderer.selCells === null) {
             menuBarHide("#tpOnlySelectedButton");
             menuBarHide("#tpFilterButton");
         } else {
             menuBarShow("#tpOnlySelectedButton");
             menuBarShow("#tpFilterButton");
         }
 
@@ -478,1375 +279,364 @@
         //menuBarHide("#tpHideLabels");
         //if (gCurrentDataset.showLabels===true)
         //$("#tpHideLabels").text(HIDELABELSNAME);
         //else
         //$("#tpHideLabels").text(SHOWLABELSNAME);
     }
 
-    function prettySeqDist(count, addSign) {
-        /* create human-readable string from chrom distance */
-        var f = count;
-        var sign = "";
-        if (addSign && count > 0)
-            sign = "+";
-
-        if (Math.abs(count) >= 1000000) {
-            f = (count / 1000000);
-            return sign + f.toFixed(3) + "Mbp";
-        }
-        if (Math.abs(count) >= 10000) {
-            f = (count / 1000);
-            return sign + f.toFixed(2) + "kbp";
-        }
-        if (Math.abs(count) >= 1000) {
-            f = (count / 1000);
-            return sign + f.toFixed(2) + "kbp";
-        }
-        return sign + f + "bp";
-    }
-
-    function prettyNumber(count, isBp) /*str*/ {
+    function prettyNumber( /*int*/ count) /*str*/ {
         /* convert a number to a shorter string, e.g. 1200 -> 1.2k, 1200000 -> 1.2M, etc */
-        var f = count;
         if (count > 1000000) {
-            f = (count / 1000000);
+            var f = (count / 1000000);
             return f.toFixed(1) + "M";
         }
         if (count > 10000) {
-            f = (count / 1000);
+            var f = (count / 1000);
             return f.toFixed(0) + "k";
         }
         if (count > 1000) {
-            f = (count / 1000);
+            var f = (count / 1000);
             return f.toFixed(1) + "k";
         }
-        return f;
-    }
-
-    function addMd5(url, md5s, key) {
-        /* lookup key in md5s and add value to url separate by ? */
-        if (md5s && md5s[key])
-            url += "?" + md5s[key];
-        return url;
-    }
 
-    function preloadImage(url) {
-        let img = new Image();
-        img.src = url;
+        return count;
     }
 
-    function openDatasetLoadPane(datasetInfo) {
+    function openDatasetLoadPane(selDatasetIdx) {
         /* open dataset dialog: load html into the three panes  */
-        //var datasetName = datasetInfo.name;
-        //var md5 = datasetInfo.md5;
-        // the UCSC apache serves latin1, so we force it back to utf8
-        gOpenDataset = datasetInfo; // for click handlers in the right panel
-
-        $.ajaxSetup({
-            'beforeSend': function(xhr) {
-                if (xhr && xhr.overrideMimeType)
-                    xhr.overrideMimeType('text/html; charset=utf8');
-            },
+        var datasetName = gDatasetList[selDatasetIdx].name;
+        var descUrl = joinPaths([datasetName, "summary.html"]);
+        $("#pane1").load(descUrl, function(response, status, xhr) {
+            if (status === "error") {
+                $("#pane1").html("File " + descUrl + " was not found");
+            }
+            $("#tabLink1").tab("show");
         });
 
-        let datasetName = datasetInfo.name;
-        let md5 = datasetInfo.md5;
-        if (datasetInfo.hasFiles && datasetInfo.hasFiles.indexOf("datasetDesc") !== -1) {
-            // description is not through html files but a json file
-            var jsonUrl = cbUtil.joinPaths([datasetName, "desc.json"]) + "?" + md5;
-            fetch(jsonUrl)
-                .then(function(response) {
-                    if (!response.ok) {
-                        throw new Error('Could not find desc.json file');
-                    }
-                    return response.json();
-                })
-                .catch(function(err) {
-                    var msg = "File " + jsonUrl + " was not found but datasetDesc.json has 'datasetDesc' in hasFiles. Internal error. Please contact the site admin or cells@ucsc.edu";
-                    $("#pane1").html(msg);
-                    $("#pane2").html(msg);
-                    $("#pane3").html(msg);
-                    $("#pane3").show();
-                })
-                .then(function(desc) {
-                    datasetDescToHtml(datasetInfo, desc);
-                });
-        } else {
-            var message = "This dataset does not seem to have a desc.conf file. Please " +
-                "read https://cellbrowser.readthedocs.io/en/master/dataDesc.html or run 'cbBuild --init' to create one";
-            if (datasetInfo.abstract)
-                // the top-level non-hierarchy dataset.conf has a message in it. Use it here, as a fallback.
-                message = datasetInfo.abstract;
-
-            $("#pane1").html(message);
-            $("#pane2").hide();
-            $("#tabLink2").hide();
-            $("#pane3").hide();
-            $("#tabLink3").hide();
-        }
-        $("#tpOpenDialogTabs").tabs("refresh").tabs("option", "active", 0);
-    }
-
-    let descLabels = {
-        "paper_url": "Publication",
-        "other_url": "Website",
-        "geo_series": "NCBI GEO Series", // = CIRM tagsV5
-        "sra": "NCBI Short Read Archive",
-        "pmid": "PubMed Abstract",
-        "pmcid": "PubMed Fulltext",
-        "sra_study": "NCBI Short-Read Archive",
-        "ega_study": "European Genotype-Phenot. Archive Study",
-        "ega_dataset": "European Genotype-Phenot. Archive Dataset",
-        "bioproject": "NCBI Bioproject",
-        "dbgap": "NCBI DbGaP",
-        "biorxiv_url": "BioRxiv preprint",
-        "doi": "Publication Fulltext",
-        "arrayexpress": "ArrayExpress",
-        "ena_project": "European Nucleotide Archive",
-        "hca_dcp": "Human Cell Atlas Data Portal",
-        "cirm_dataset": "California Institute of Regenerative Medicine Dataset",
-    };
-
-    let descUrls = {
-        "geo_series": "https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=",
-        "sra_study": "https://trace.ncbi.nlm.nih.gov/Traces/sra/?study=",
-        "bioproject": "https://www.ncbi.nlm.nih.gov/bioproject/",
-        "ega_study": "https://ega-archive.org/studies/",
-        "ega_dataset": "https://ega-archive.org/datasets/",
-        "pmid": "https://www.ncbi.nlm.nih.gov/pubmed/",
-        "pmcid": "https://www.ncbi.nlm.nih.gov/pmc/articles/",
-        "dbgap": "https://www.ncbi.nlm.nih.gov/projects/gap/cgi-bin/study.cgi?study_id=",
-        "doi": "http://dx.doi.org/",
-        "ena_project": "https://www.ebi.ac.uk/ena/data/view/",
-        "cirm_dataset": "https://cirm.ucsc.edu/d/",
-        "arrayexpress": "https://www.ebi.ac.uk/arrayexpress/experiments/",
-        "hca_dcp": "https://data.humancellatlas.org/explore/projects/",
-    }
-
-    function htmlAddLink(htmls, desc, key, linkLabel) {
-        /* add a link to html on a new line. if desc[key] includes a space, the part after it is the link label. */
-        if (!desc[key])
-            return;
-
-        let label = "Link";
-        if (linkLabel)
-            label = linkLabel;
-        else
-            label = descLabels[key];
-
-        htmls.push("<b>");
-        htmls.push(label);
-        htmls.push(": </b>");
-
-        // for cases where more than one ID is needed, this function also accepts a list in the object
-        // for 99% of the cases, it'll be a string though
-        let urls = desc[key];
-        if (!(urls instanceof Array))
-            urls = [urls];
-
-        let frags = []; // html fragments, one per identifier
-        for (let url of urls) {
-            url = url.toString(); // in case it's an integer or float
-            let urlLabel = url;
-            let spcPos = url.indexOf(" ");
-            if (spcPos !== -1) {
-                urlLabel = url.slice(spcPos + 1);
-                url = url.slice(0, spcPos);
-            }
-
-            if (!url.startsWith("http"))
-                url = descUrls[key] + url;
-
-            let parts = []
-            parts.push("<a target=_blank href='");
-            parts.push(url);
-            parts.push("'>");
-            parts.push(urlLabel);
-            parts.push("</a>");
-            let htmlLine = parts.join("");
-            frags.push(htmlLine);
-        }
-        htmls.push(frags.join(", "));
-        htmls.push("<br>");
-    }
-
-    function buildLinkToMatrix(htmls, dsName, matFname, label) {
-        /* link to a matrix file for download, handles mtx.gz */
-        if (label)
-            htmls.push("<b> Matrix for " + label + ":</b> ");
-
-        htmls.push("<a href='" + dsName + "/" + matFname + "'>" + matFname + "</a>");
-        if (matFname.endsWith(".mtx.gz")) {
-            var prefix = "";
-            if (matFname.indexOf("_") !== -1)
-                prefix = matFname.split("_")[0] + "_";
-            var ftName = prefix + "features.tsv.gz";
-            htmls.push(", <a href='" + dsName + "/" + ftName + "'>" + ftName + "</a>");
-            var barName = prefix + "barcodes.tsv.gz";
-            htmls.push(", <a href='" + dsName + "/" + barName + "'>" + barName + "</a>");
-        }
-        htmls.push("<br>");
-    }
-
-    function buildSupplFiles(desc, dsName, htmls) {
-        /* create html with links to supplementary files */
-        if (desc.supplFiles) {
-            let supplFiles = desc.supplFiles;
-            for (let suppFile of supplFiles) {
-                let label = suppFile.label;
-                let fname = suppFile.file;
-                htmls.push("<b>" + label + ":</b> <a href='" + dsName);
-                htmls.push("/" + fname + "'>" + fname + "</a>");
-                htmls.push("<br>");
+        var methodsUrl = joinPaths([datasetName, "methods.html"]);
+        $("#pane2").load(methodsUrl, function(response, status, xhr) {
+            if (status === "error") {
+                $("#pane2").html("File " + methodsUrl + " was not found");
             }
-        }
-    }
-
-    function buildDownloadsPane(datasetInfo, desc) {
-        var htmls = [];
-        if (datasetInfo.name === "") { // the top-level desc page has no methods/downloads, it has only informative text
-            $("#pane3").hide();
-            $("#tabLink3").hide();
-        } else {
-            if (desc.coordFiles === undefined) {
-                htmls.push("To download the data for datasets in this collection: open the collection, ");
-                htmls.push("select a dataset in the list to the left, and navigate to the 'Data Download' tab. ");
-                htmls.push("This information can also be accessed while viewing a dataset by clicking the 'Info &amp; Downloads' button.");
-            } else if (desc.hideDownload === true || desc.hideDownload == "True" || desc.hideDownload == "true") {
-                htmls.push("The downloads section has been deactivated by the authors.");
-                htmls.push("Please contact the dataset authors to get access.");
-            } else {
-                if (desc.matrices) {
-                    htmls.push("<p>");
-                    for (var key in desc.matrices) {
-                        var mat = desc.matrices[key];
-                        buildLinkToMatrix(htmls, datasetInfo.name, mat.fileName, mat.label);
-                    }
-                    htmls.push("</p>");
-                } else if (desc.matrixFile !== undefined && desc.matrixFile.endsWith(".mtx.gz")) {
-                    htmls.push("<p>");
-                    var matBaseName = desc.matrixFile.split("/").pop();
-                    buildLinkToMatrix(htmls, datasetInfo.name, matBaseName, "dataset");
-                    htmls.push("</p>");
-                } else {
-                    htmls.push("<p><b>Matrix:</b> <a href='" + datasetInfo.name);
-                    htmls.push("/exprMatrix.tsv.gz'>exprMatrix.tsv.gz</a>");
-                }
-                if (desc.unitDesc)
-                    htmls.push("<br>Values in matrix are: " + desc.unitDesc);
-                htmls.push("</p>");
-
-                if (desc.rawMatrixFile) {
-                    htmls.push("<p><b>Raw count matrix:</b> <a href='" + datasetInfo.name);
-                    htmls.push("/" + desc.rawMatrixFile + "'>" + desc.rawMatrixFile + "</a>");
-                    if (desc.rawMatrixNote)
-                        htmls.push("<br>" + desc.rawMatrixNote);
-                    htmls.push("</p>");
-                }
-
-                htmls.push("<p><i><a style='float:right; padding-left: 100px'; target=_blank href='https://cellbrowser.readthedocs.io/en/master/load.html'>Help: Load matrix/meta into Seurat or Scanpy</a></i></p>");
-
-                htmls.push("<p><b>Cell meta annotations:</b> <a target=_blank href='" + datasetInfo.name);
-                htmls.push("/meta.tsv'>meta.tsv</a>");
-                if (desc.metaNote)
-                    htmls.push("<br>" + desc.metaNote);
-                htmls.push("</p>");
-
-                htmls.push("<p><b>Dimensionality reduction coordinates:</b><br>");
-                for (let fname of desc.coordFiles)
-                    htmls.push("<a target=_blank href='" + datasetInfo.name + "/" + fname + "'>" + fname + "</a><br>");
-                htmls.push("</p>");
-
-                buildSupplFiles(desc, datasetInfo.name, htmls);
-
-                htmls.push("<p><b>Dataset description</b>: ");
-                htmls.push("<a target=_blank href='" + datasetInfo.name + "/desc.json'>desc.json</a></p>");
-
-                htmls.push("<p><b>Cell Browser configuration</b>: ");
-                htmls.push("<a target=_blank href='" + datasetInfo.name + "/dataset.json'>dataset.json</a></p>");
+        });
 
-                $("#pane3").html(htmls.join(""));
-                $("#pane3").show();
-                $("#tabLink3").show();
+        var downloadUrl = joinPaths([datasetName, "downloads.html"]);
+        $("#pane3").load(downloadUrl, function(response, status, xhr) {
+            if (status === "error") {
+                $("#pane3").html("File " + downloadUrl + " was not found");
             }
-
-        }
+        });
     }
 
-    function buildImagesPane(datasetInfo, desc) {
-        if (!desc.imageSets) {
-            $("#tabLinkImg").hide();
-            $("#paneImg").hide();
-            return;
-        }
-
-        let htmls = [];
-        htmls.push("<h4>Microscopy images</h4>");
-        // TOC
-        let catIdx = 0;
-        htmls.push("<div style='padding-bottom:8px'>Jump to: ");
-        for (let catInfo of desc.imageSets) {
-            htmls.push("<a style='padding-left:12px' href='#imgCat" + catIdx + "'>" + catInfo.categoryLabel + "</a>");
-            catIdx++;
-        }
-        htmls.push("</div>");
+    function openDatasetDialog() {
+        /* build dataset open dialog */
 
-        if (desc.imageSetNote)
-            htmls.push("<p>" + desc.imageSetNote + "<p>");
+        var winWidth = window.innerWidth - 0.05 * window.innerWidth;
+        var winHeight = window.innerHeight - 0.05 * window.innerHeight;
+        var buttonWidth = 400;
+        var tabsWidth = winWidth - buttonWidth - 70;
 
-        // actual HTML
-        catIdx = 0;
-        for (let catInfo of desc.imageSets) {
-            htmls.push("<div style='padding-top:6px; padding-bottom:4px' class='tpImgCategory'>");
-            htmls.push("<a name='imgCat" + catIdx + "'></a>");
-            catIdx++;
-            htmls.push("<b>" + catInfo.categoryLabel + ":</b><br>");
-            let imgDir = datasetInfo.name + "/images/";
-            htmls.push("<div style='padding-left:1em; padding-top:4px' class='tpImgSets'>");
-
-            for (let imgSet of catInfo.categoryImageSets) {
-                let imgLinks = [];
-                if (imgSet.setLabel)
-                    htmls.push("<b>" + imgSet.setLabel + "</b><br>");
-                htmls.push("<div style='padding-left:1em;' class='tpImgSetLinks'>");
-                for (let img of imgSet.images) {
-                    imgLinks.push("Show: <a target=_blank href='" + imgDir + img.file + "'>" + img.label + "</a>");
-                }
-                htmls.push(imgLinks.join(", "));
 
-                if (imgSet.downloads) {
-                    let dlLinks = [];
-                    for (let dl of imgSet.downloads) {
-                        //dlLinks.push("<a href='"+imgDir+dl.file+"' download><span style='font-size:12px' class='material-icons-round'>get_app</span>"+dl.label+"</a>");
-                        dlLinks.push("<a href='" + imgDir + dl.file + "' download>" + dl.label + "</a>");
-                    }
-                    //htmls.push("<br><div style='padding-left: 1em'>Download: ");
-                    htmls.push("<br><div>Download: ");
-                    htmls.push(dlLinks.join(", "));
-                    htmls.push("</div>");
-                }
-                //htmls.push("<br>");
-                htmls.push("</div>"); //  tpImgSetLinks
-            }
-            htmls.push("</div>"); //  tpImgSets
-            htmls.push("</div>"); //  tpImgCategory
-        }
-        //htmls.push("</ul>");
-        $("#paneImg").html(htmls.join(""));
-        $("#paneImg").show();
-        $("#tabLinkImg").show();
-    }
-
-    function buildMethodsPane(datasetInfo, desc) {
-        // methods panel
-        //
         var htmls = [];
-        if (desc.methods) {
-            htmls.push("<p>");
-            htmls.push(desc.methods);
-            htmls.push("</p>");
-        }
-        if (desc.algParams) {
-            htmls.push("<p><b>Algorithm parameters: </b>");
-            let algParams = desc.algParams;
-            if (algParams instanceof Object)
-                algParams = Object.entries(algParams);
-
-            for (let i = 0; i < algParams.length; i++) {
-                let key = algParams[i][0];
-                let val = algParams[i][1];
-                htmls.push(key + "=" + val + ", ");
-            }
-            htmls.push("</p>");
-        }
-        if (htmls.length !== 0) {
-            $("#pane2").html(htmls.join(""));
-            $("#pane2").show();
-            $("#tabLink2").show();
-        } else {
-            $("#pane2").hide();
-            $("#tabLink2").hide();
-        }
-    }
-
-    function pageAtUcsc() {
-        // return true if current page is at ucsc.edu
-        return (window.location.hostname.endsWith("ucsc.edu"));
-    }
-
-    function buildClassification(htmls, datasetInfo, attrName, label, addSep) {
-        if (datasetInfo[attrName]) {
-            var values;
-            // in Nov 2022, the facets moved into their own object, old dataasets have them in the dataset itself as attributes
-            if (datasetInfo.facets)
-                values = datasetInfo.facets[attrName];
-            else
-                values = datasetInfo[attrName];
-
-            htmls.push(label + "=" + values.join(","));
-            if (addSep)
-                htmls.push("; ");
-        }
-    }
-
-    function datasetDescToHtml(datasetInfo, desc) {
-        /* given an object with keys title, abstract, pmid, etc, fill the dataset description tabs with html */
-        if (!desc) // http errors call this with undefined
-            return;
-
-        let htmls = [];
-
-        if (datasetInfo.name === "") // the root dataset
-            $('#tabLink1').text("Overview");
-        else
-            $('#tabLink1').text("Abstract");
-
-        if (desc.title) {
-            htmls.push("<h4>");
-            htmls.push(desc.title);
-            htmls.push("</h4>");
-        }
-        if (desc.image) {
-            htmls.push("<img style='float:right; padding-left:5px' src='");
-            htmls.push(datasetInfo.name + "/" + desc.image[0] + "'");
-            if (desc.imageMap)
-                htmls.push(" usemap='#clickmap'");
-            htmls.push(" width='" + desc.image[1] + "' height='" + desc.image[2] + "'>");
-        }
-        if (desc.imageMap) {
-            htmls.push('<map name="clickmap">');
-            htmls.push(desc.imageMap);
-            htmls.push('</map>');
-        }
-
-        if (desc.abstract) {
-            htmls.push("<p>");
-            htmls.push(desc.abstract);
-            htmls.push("</p>");
-        } else {
-            // the top-level hardcoded dataset for non-hierarchy mode has the abstract in the
-            // dataset config. It's a lot easier this way, so just pull it in here.
-            htmls.push("<p>");
-            htmls.push(datasetInfo.abstract);
-            htmls.push("</p>");
-        }
-
-        if (desc.author) {
-            htmls.push("<b>Author: </b> " + desc.author);
-            htmls.push("<br>");
-        }
-
-        if (desc.authors) {
-            htmls.push("<b>Authors: </b> " + desc.authors);
-            htmls.push("<br>");
-        }
-
-        if (desc.lab) {
-            htmls.push("<b>Lab: </b> " + desc.lab);
-            htmls.push("<br>");
-        }
-        if (desc.institution) {
-            htmls.push("<b>Institution: </b> " + desc.institution);
-            htmls.push("<br>");
-        }
-
-
-        htmlAddLink(htmls, desc, "biorxiv_url");
-        htmlAddLink(htmls, desc, "paper_url");
-        htmlAddLink(htmls, desc, "other_url");
-        htmlAddLink(htmls, desc, "geo_series");
-        htmlAddLink(htmls, desc, "pmid");
-        htmlAddLink(htmls, desc, "dbgap");
-        htmlAddLink(htmls, desc, "sra_study");
-        htmlAddLink(htmls, desc, "bioproject");
-        htmlAddLink(htmls, desc, "sra");
-        htmlAddLink(htmls, desc, "doi");
-        htmlAddLink(htmls, desc, "arrayexpress");
-        htmlAddLink(htmls, desc, "cirm_dataset");
-        htmlAddLink(htmls, desc, "ega_study");
-        htmlAddLink(htmls, desc, "ega_dataset");
-        htmlAddLink(htmls, desc, "ena_project");
-        htmlAddLink(htmls, desc, "hca_dcp");
-
-        if (desc.urls) {
-            for (let key in desc.urls)
-                htmlAddLink(htmls, desc.urls, key, key);
-        }
-
-        if (desc.custom) {
-            for (let key in desc.custom) {
-                htmls.push("<b>" + key + ": </b> " + desc.custom[key]);
-                htmls.push("<br>");
-            }
-        }
-
-        if (desc.submitter) {
-            htmls.push("<b>Submitted by: </b> " + desc.submitter);
-            if (desc.submission_date) {
-                htmls.push(" (" + desc.submission_date);
-                htmls.push(")");
-            }
-            if (desc.version)
-                htmls.push(", Version " + desc.version);
-            htmls.push("<br>");
-        }
-
-        if (desc.shepherd) {
-            htmls.push("<b>UCSC Data Shepherd: </b> " + desc.shepherd);
-            htmls.push("<br>");
-        }
-        if (desc.wrangler) {
-            htmls.push("<b>UCSC Data Wrangler: </b> " + desc.wrangler);
-            htmls.push("<br>");
-        }
-
-        // collections have no downloads tab, but multiomic-gbm wants supplementary files there, so make them appear
-        buildSupplFiles(desc, datasetInfo.name, htmls);
-
-        let topName = datasetInfo.name.split("/")[0];
-        if (pageAtUcsc()) {
-            if (datasetInfo.name !== "") {
-                // Only do this if this is not the root dataset
-                if ((datasetInfo.parents) && (datasetInfo.parents.length > 1)) {
-                    // if the dataset is a collection
-                    htmls.push("<b>Direct link to this collection for manuscripts: </b> https://" + topName + ".cells.ucsc.edu");
-                    htmls.push("<br>");
-                } else {
-                    htmls.push("<b>Direct link to this plot for manuscripts: </b> https://" + topName + ".cells.ucsc.edu");
-                    htmls.push("<br>");
-                }
-
-                console.log(datasetInfo);
-
-                if (datasetInfo.atacSearch) {
-                    htmls.push("<b>ATAC-seq search gene models: </b>" + datasetInfo.atacSearch);
-                    htmls.push("<br>");
-                }
-
-                htmls.push("<b>Dataset classification: </b>");
-
-                buildClassification(htmls, datasetInfo, "body_parts", "Organs", true);
-                buildClassification(htmls, datasetInfo, "diseases", "Diseases", true);
-                buildClassification(htmls, datasetInfo, "organisms", "Organism", true);
-                buildClassification(htmls, datasetInfo, "life_stages", "Life Stage", true);
-                buildClassification(htmls, datasetInfo, "domains", "Scientific Domain", true);
-                buildClassification(htmls, datasetInfo, "sources", "Source Database", false);
-
-                htmls.push("<p style='padding-top: 8px'>If you use the Cell Browser of this dataset, please cite the " +
-                    "original publication and " +
-                    "<a href='https://academic.oup.com/bioinformatics/article/37/23/4578/6318386' target=_blank>" +
-                    "Speir et al. 2021</a>. Feedback? Email us at <a href='cells@ucsc.edu' " +
-                    "target='_blank'>cells@ucsc.edu</a>." +
-                    "</p>");
-
-                htmls.push("<p style='padding-top: 8px'><small>Cell Browser dataset ID: " + datasetInfo.name +
-                    "</small></p>");
-
-            }
-        }
-
-        $("#pane1").html(htmls.join(""));
-
-        buildMethodsPane(datasetInfo, desc);
-        buildDownloadsPane(datasetInfo, desc);
-        buildImagesPane(datasetInfo, desc);
-
-        $("#tpOpenDialogTabs").tabs("refresh");
-        //.tabs("option", "active", 0) does not do the color change of the tab so doing this instead
-        $("#tabLink1").click();
-        $("area").click(function(ev) {
-            var dsName = ev.target.href.split("/").pop();
-            loadDataset(gOpenDataset.name + "/" + dsName, true);
-            $(".ui-dialog-content").dialog("close");
-            ev.preventDefault();
-        });
-
-    }
-
-    function buildListPanel(datasetList, listGroupHeight, leftPaneWidth, htmls, selName) {
-        /* make a dataset list and append its html lines to htmls */
-        htmls.push("<div id='tpDatasetList' class='list-group' style='float: left; margin-top: 1em; height:" + listGroupHeight + "px; overflow-y:scroll; width:" + leftPaneWidth + "px'>");
-        if (!datasetList || datasetList.length === 0) {
-            alert("No datasets are available. Please make sure that at least one dataset does not set visibility=hide " +
-                " or that at least one collection is defined. Problems? -> cells@ucsc.edu");
-            return;
-        }
-
-        var selIdx = 0;
-        for (var i = 0; i < datasetList.length; i++) {
-            var dataset = datasetList[i];
-
-            var clickClass = "tpDatasetButton";
-            if (dataset.isCollection)
-                clickClass = "tpCollectionButton";
-            if (dataset.name === selName || (selName === undefined && i === 0)) {
-                clickClass += " active";
-                selIdx = i;
-            }
-
-            var bodyPartStr = "";
-            var disStr = "";
-            var orgStr = "";
-            var projStr = "";
-            var domStr = "";
-            var lifeStr = "";
-            var sourceStr = "";
-
-            if (dataset.body_parts) {
-                bodyPartStr = cleanStrings(dataset.body_parts).join("|");
-            }
-            if (dataset.diseases) {
-                disStr = cleanStrings(dataset.diseases).join("|");
-            }
-            if (dataset.organisms) {
-                orgStr = cleanStrings(dataset.organisms).join("|");
-            }
-            if (dataset.projects) {
-                projStr = cleanStrings(dataset.projects).join("|");
-            }
-            if (dataset.domains) {
-                domStr = cleanStrings(dataset.domains).join("|");
-            }
-            if (dataset.life_stages) {
-                lifeStr = cleanStrings(dataset.life_stages).join("|");
-            }
-            if (dataset.sources) {
-                sourceStr = cleanStrings(dataset.sources).join("|");
-            }
-
-            var line = "<a id='tpDatasetButton_" + i + "' " +
-                "data-body='" + bodyPartStr + "' " +
-                "data-dis='" + disStr + "' " +
-                "data-org='" + orgStr + "' " +
-                "data-proj='" + projStr + "' " +
-                "data-dom='" + domStr + "' " +
-                "data-source='" + sourceStr + "' " +
-                "data-stage='" + lifeStr + "' " +
-                "role='button' class='tpListItem list-group-item " + clickClass + "' data-datasetid='" + i + "'>"; // bootstrap seems to remove the id
+        var activeIdx = 0;
+        htmls.push("<div class='list-group' style='width:" + buttonWidth + "px'>");
+        for (var i = 0; i < gDatasetList.length; i++) {
+            var dataset = gDatasetList[i];
+            var line = "<button id='tpDatasetButton_" + i + "' type='button' class='list-group-item' data-datasetid='" + i + "'>"; // bootstrap seems to remove the id
             htmls.push(line);
-
-            if (!dataset.isSummary)
-                htmls.push('<button type="button" class="btn btn-primary btn-xs load-dataset" data-placement="bottom">Open</button>');
+            htmls.push('<a role="button" class="btn btn-primary btn-xs load-dataset">Open dataset</a>')
 
             if (dataset.sampleCount !== undefined) {
                 var countDesc = prettyNumber(dataset.sampleCount);
-                htmls.push("<span class='badge' style='background-color: #888'>" + countDesc + "</span>");
-            }
-
-            if (dataset.datasetCount !== undefined) {
-                htmls.push("<span class='badge' style='background-color: #28a745'>" + dataset.datasetCount + " datasets</span>");
-            }
-
-            if (dataset.collectionCount !== undefined) {
-                htmls.push("<span class='badge' style='background-color: #188725'>" + dataset.collectionCount + " collections</span>");
+                htmls.push("<span class='badge'>" + countDesc + "</span>");
             }
 
-            //if (dataset.tags!==undefined) {
-            //for (var tagI = 0; tagI < dataset.tags.length; tagI++) {
-            //var tag = dataset.tags[tagI];
-            //if (tag==="smartseq2" || tag==="ATAC" || tag==="10x")
-            //continue
-            //htmls.push("<span class='badge'>"+tag+"</span>");
-            //}
-            //}
-            htmls.push(dataset.shortLabel + "</a>");
-        }
-        htmls.push("</div>"); // list-group
-        return selIdx;
-    }
-
-    function getDatasetAttrs(datasets, attrName) {
-        /* return an array of (attrName, "attrName (count)") of all attrNames (e.g. body_parts) in a dataset array */
-        var valCounts = {};
-        for (let i = 0; i < datasets.length; i++) {
-            let ds = datasets[i];
-            if (ds[attrName] === undefined)
-                continue
-            for (let bp of ds[attrName])
-                if (bp in valCounts)
-                    valCounts[bp]++;
-                else
-                    valCounts[bp] = 1;
-        }
-
-        let allValues = keys(valCounts);
-        allValues.sort();
-
-        var valLabels = {};
-        for (let i = 0; i < allValues.length; i++) {
-            var key = allValues[i];
-            var count = valCounts[key];
-            var labelKey = key;
-            if (labelKey === "")
-                labelKey = "-empty-"
-            var label = labelKey + " (" + count + ")"
-            valLabels[key] = label;
-        }
-        return Object.entries(valLabels);
-    }
-
-    function filterDatasetsDom() {
-        /* keep only datasets that fulfill the filters */
-
-        // read the current filter values of the dropboxes
-        var categories = ["Body", "Dis", "Org", "Proj", "Stage", "Dom", "Source"];
-        var filtVals = {};
-        for (var category of categories) {
-            var vals = $("#tp" + category + "Combo").val();
-            if (vals === undefined)
-                vals = [];
-
-            // strip special chars
-            var cleanVals = [];
-            for (var val of vals)
-                cleanVals.push(cleanString(val));
-
-            filtVals[category] = cleanVals;
-        }
-
-        let elList = $(".tpListItem");
-        var shownCount = 0;
-        var hideCount = 0;
-        for (let el of elList) {
-            // never touch the first/summary element
-            if (el.getAttribute("data-body") === "summary")
-                continue
-            // read the values of the current DOM element
-            var domVals = {};
-            for (var category of categories)
-                domVals[category] = el.getAttribute("data-" + category.toLowerCase());
-
-            var isShown = true;
-            // now compare filtVals and domVals
-            for (var category of categories) {
-                var filtList = filtVals[category];
-                var domList = domVals[category];
-
-                let found = false;
-                if (filtList.length === 0)
-                    found = true;
-                for (var filtVal of filtList)
-                    if (domList.indexOf(filtVal) != -1)
-                        found = true;
-
-                if (!found) {
-                    isShown = false;
-                    break;
+            if (dataset.tags !== undefined) {
+                for (var tagI = 0; tagI < dataset.tags.length; tagI++) {
+                    var tag = dataset.tags[tagI];
+                    htmls.push("<span class='badge'>" + tag + "</span>");
                 }
             }
-
-            if (isShown) {
-                el.style.display = "";
-                shownCount++;
-            } else {
-                el.style.display = "none";
-                hideCount++;
-            }
-        }
-        if (hideCount !== 0)
-            $('#tpDatasetCount').text("(filters active, " + shownCount + " datasets shown)");
-        else
-            $('#tpDatasetCount').text("(" + shownCount + " dataset collections)");
-    }
-
-    function openDatasetDialog(openDsInfo, selName) {
-        /* build dataset open dialog,
-         * - openDsInfo is the currently open object or a collection.
-         * - selName is the currently selected dataset in this list
-         */
-
-        var datasetList = [];
-        var listGroupHeight = 0;
-        var leftPaneWidth = 400;
-        var title = "Choose Cell Browser Dataset";
-
-        // inline functions
-        function openCollOrDataset(selDatasetIdx) {
-            /* click handler, opens either a collection or a dataset */
-            var dsInfo = datasetList[selDatasetIdx];
-            var datasetName = dsInfo.name;
-            if (dsInfo.isCollection)
-                showCollectionDialog(datasetName);
-            else
-                loadDataset(datasetName, true, dsInfo.md5);
-            $(".ui-dialog-content").dialog("close");
-            //changeUrl({"bp":null});
-        }
-
-        function buildFilter(html, filterVals, filterLabel, urlVar, comboId, comboLabel) {
-            /* build html for a faceting filter */
-            if (filterVals.length == 0)
-                return false;
-            html.push("<span style='margin-right:5px'>" + filterLabel + ":</span>");
-            let selPar = getVarSafe(urlVar);
-            if (selPar && selPar !== "")
-                filtList = selPar.split("|");
-            buildComboBox(html, comboId, filterVals, filtList, comboLabel, 200, {
-                multi: true
-            });
-            html.push("&nbsp;&nbsp;");
-            return true;
-        }
-
-        function connectOpenPane(selDatasetIdx, datasetList) {
-            /* set all the click handlers for the left open dataset pane */
-            $("button.list-group-item").eq(selDatasetIdx).css("z-index", "1000"); // fix up first overlap
-            $("button.list-group-item").keypress(function(e) {
-                // load the current dataset when the user presses Return
-                if (e.which === '13') {
-                    openCollOrDataset(selDatasetIdx);
-                }
-            });
-            $(".list-group-item").click(function(ev) {
-                selDatasetIdx = parseInt($(ev.target).data('datasetid')); // index of clicked dataset
-                $(".list-group-item").removeClass("active");
-                $('#tpDatasetButton_' + selDatasetIdx).bsButton("toggle"); // had to rename .button() in index.html
-                var datasetInfo = datasetList[selDatasetIdx];
-                openDatasetLoadPane(datasetInfo);
-            });
-            $(".list-group-item").dblclick(function(ev) {
-                selDatasetIdx = parseInt($(this).data('datasetid'));
-                openCollOrDataset(selDatasetIdx);
-            });
-            $(".load-dataset").click(function(ev) {
-                ev.preventDefault();
-                ev.stopPropagation();
-                selDatasetIdx = parseInt($(this).parents('.list-group-item').data('datasetid'));
-                openCollOrDataset(selDatasetIdx);
-                return false;
-            });
-            $(".list-group-item").focus(function(event) {
-                selDatasetIdx = parseInt($(event.target).data('datasetid')); // index of clicked dataset
-                // bootstrap has a bug where the blue selection frame is hidden by neighboring buttons
-                // Working around this here by bumping up the current z-index.
-                $("button.list-group-item").css("z-index", "0");
-                $("button.list-group-item").eq(selDatasetIdx).css("z-index", "1000");
-            });
-        }
-
-        function onFilterChange(ev) {
-            /* called when user changes a filter: updates list of datasets shown */
-            var filtNames = $(this).val();
-
-            var param = null;
-            if (this.id === "tpBodyCombo")
-                param = "bp";
-            else if (this.id == "tpDisCombo")
-                param = "dis";
-            else if (this.id == "tpOrgCombo")
-                param = "org";
-            else if (this.id == "tpProjCombo")
-                param = "proj";
-            else if (this.id == "tpDomCombo")
-                param = "dom";
-            else if (this.id == "tpStageCombo")
-                param = "stage";
-
-            // change the URL
-            var filtArg = filtNames.join("~");
-            var urlArgs = {}
-            urlArgs[param] = filtArg;
-            changeUrl(urlArgs);
-            filterDatasetsDom();
-        }
-
-        // -- end inline functions
-
-        gOpenDataset = openDsInfo;
-        var activeIdx = 0;
-        var onlyInfo = false;
-
-        datasetList = openDsInfo.datasets;
-
-        if (datasetList === undefined)
-            onlyInfo = true;
-
-        var noteLines = [];
-
-        // if this is a collection, not a dataset, change descriptive text in dialog
-        if (datasetList && gOpenDataset.name !== "") {
-            let dsCount = datasetList.length;
-            title = 'Select one dataset from the collection "' + openDsInfo.shortLabel + '"';
-            title = title.replace(/'/g, "&apos;");
-            noteLines.push("<p>The collection '" + openDsInfo.shortLabel + "' contains " + dsCount + " datasets. " +
-                "Double-click or click 'Open' below.<br>To move between datasets later in the cell browser, " +
-                "use the 'Collection' dropdown. </p>");
-
-            changeUrl({
-                "ds": openDsInfo.name.replace(/\//g, " ")
-            }); // + is easier to type
-        }
-
-        let doFilters = false;
-        let filtList = [];
-        let bodyParts = null;
-        let diseases = null;
-        let organisms = null;
-        let projects = null;
-        let lifeStages = null;
-        let domains = null;
-        let sources = null;
-
-        if (openDsInfo.parents === undefined && openDsInfo.datasets !== undefined) {
-            bodyParts = getDatasetAttrs(openDsInfo.datasets, "body_parts");
-            diseases = getDatasetAttrs(openDsInfo.datasets, "diseases");
-            organisms = getDatasetAttrs(openDsInfo.datasets, "organisms");
-            projects = getDatasetAttrs(openDsInfo.datasets, "projects");
-            lifeStages = getDatasetAttrs(openDsInfo.datasets, "life_stages");
-            domains = getDatasetAttrs(openDsInfo.datasets, "domains");
-            sources = getDatasetAttrs(openDsInfo.datasets, "sources");
-
-            // mirror websites are not using the filters at all. So switch off the entire filter UI if they're not used
-            if (bodyParts.length !== 0 || diseases.length !== 0 || organisms.length !== 0 || projects.length !== 0 || domains.length !== 0 || lifeStages.length !== 0 || sources.length !== 0)
-                doFilters = true;
-
-            if (doFilters) {
-                noteLines.push("<div style='margin-right: 10px; font-weight: bold'>Filters: <span id='tpDatasetCount'></span></div>");
-
-                buildFilter(noteLines, bodyParts, "Organ", "body", "tpBodyCombo", "select organs...");
-                buildFilter(noteLines, diseases, "Disease", "dis", "tpDisCombo", "select diseases...");
-                buildFilter(noteLines, organisms, "Species", "org", "tpOrgCombo", "select species...");
-                buildFilter(noteLines, projects, "Project", "proj", "tpProjCombo", "select project...");
-                noteLines.push("<div style='height:4px'></div>");
-                buildFilter(noteLines, lifeStages, "Life Stages", "stage", "tpStageCombo", "select stage...");
-                buildFilter(noteLines, domains, "Scient. Domain", "dom", "tpDomCombo", "select domain...");
-                buildFilter(noteLines, sources, "Source DB", "source", "tpSourceCombo", "select db...");
-            }
-        }
-
-        // create links to the parents of the dataset
-        if (openDsInfo && openDsInfo.parents && !onlyInfo) {
-
-            noteLines.push("Go back to: ");
-            // make the back links
-            let backLinks = [];
-            let allParents = [];
-            let parents = openDsInfo.parents;
-            for (let i = 0; i < parents.length; i++) {
-                let parentInfo = parents[i];
-                let parName = parentInfo[0];
-
-                let parLabel = parentInfo[1];
-                let childName = null;
-                if (i === parents.length - 1)
-                    childName = openDsInfo.name;
-                else
-                    childName = parents[i + 1][0];
-
-                allParents.push(parName);
-                backLinks.push("<span class='tpBackLink link' data-open-dataset='" + allParents.join("/") + "' data-sel-dataset='" + childName + "'>" + parLabel + "</span>");
-            }
-            noteLines.push(backLinks.join("&nbsp;&gt;&nbsp;"));
-        }
-
-        if (onlyInfo)
-            title = "Dataset Information";
-        else {
-            datasetList.unshift({
-                shortLabel: "Overview",
-                name: openDsInfo.name,
-                hasFiles: openDsInfo.hasFiles,
-                body_parts: ["summary"],
-                isSummary: true,
-                abstract: openDsInfo.abstract
-            });
-        }
-
-        var winWidth = window.innerWidth - 0.05 * window.innerWidth;
-        var winHeight = window.innerHeight - 0.05 * window.innerHeight;
-        var tabsWidth = winWidth - leftPaneWidth - 50;
-        listGroupHeight = winHeight - 100;
-
-        var htmls = ["<div style='line-height: 1.1em'>"];
-        htmls.push(noteLines.join(""));
-        htmls.push("</div>");
-
-        htmls.push("<div id='tpDatasetBrowser'>");
-
-        if (onlyInfo) {
-            leftPaneWidth = 0;
-            htmls.push("<div></div>"); // keep structure of the page the same, skip the left pane
-        } else {
-            activeIdx = buildListPanel(datasetList, listGroupHeight, leftPaneWidth, htmls, selName);
-            htmls.push("<div id='tpOpenDialogDatasetDesc' style='width:" + tabsWidth + "px; float:right; left: " + (leftPaneWidth + 10) + "px; margin-top: 1em; border: 0'>");
+            htmls.push(dataset.shortLabel + "</button>");
+            if (db !== null && db.name === dataset.name)
+                activeIdx = i;
         }
+        htmls.push("</div>"); // list-group
 
-        htmls.push("<div id='tpOpenDialogTabs' style='border: 0'>");
+        htmls.push("<div id='tpOpenDialogLabel' style='width:" + tabsWidth + "px; position:absolute; left: " + (buttonWidth + 40) + "px; top: 10px;'>");
+        htmls.push("<div id='tpOpenDialogTabs'>");
         htmls.push("<ul class='nav nav-tabs'>");
-        htmls.push("<li class='active'><a class='tpDatasetTab' id='tabLink1' data-toggle='tab' href='#pane1'>Abstract</a></li>");
-        htmls.push("<li><a class='tpDatasetTab' id='tabLink2' data-toggle='tab' href='#pane2'>Methods</a></li>");
-        htmls.push("<li><a class='tpDatasetTab' id='tabLink3' data-toggle='tab' style='display:none' href='#pane3'>Data Download</a></li>");
-        htmls.push("<li><a class='tpDatasetTab' id='tabLinkImg' data-toggle='tab' href='#paneImg'>Images</a></li>");
+        htmls.push("<li class='active'><a id='tabLink1' data-toggle='tab' href='#pane1'>Abstract</a></li>");
+        htmls.push("<li><a id='tabLink2' data-toggle='tab' href='#pane2'>Methods</a></li>");
+        htmls.push("<li><a id='tabLink3' data-toggle='tab' href='#pane3'>Data Download</a></li>");
         htmls.push("</ul>");
+        htmls.push("</div>");
+
+        htmls.push("<div class='tab-content'>");
 
         htmls.push("<div id='pane1' class='tpDatasetPane tab-pane'>");
         htmls.push("<p>Loading abstract...</p>");
         htmls.push("</div>");
 
         htmls.push("<div id='pane2' class='tpDatasetPane tab-pane'>");
         htmls.push("<p>Loading methods...</p>");
         htmls.push("</div>");
 
         htmls.push("<div id='pane3' class='tpDatasetPane tab-pane'>");
-        htmls.push("<p>Loading download instructions...</p>");
+        htmls.push("<p>Loading data download...</p>");
         htmls.push("</div>");
 
-        htmls.push("<div id='paneImg' class='tpDatasetPane tab-pane'>");
-        htmls.push("<p>Loading image data...</p>");
-        htmls.push("</div>");
-
-        htmls.push("</div>"); // tpOpenDialogTabs
+        htmls.push("</div>"); // tab-content
 
-        htmls.push("</div>"); // tpOpenDialogDatasetDesc
+        htmls.push("</div>"); // tpOpenDialogLabel
 
         //htmls.push("<div id='tpSelectedId' data-selectedid='0'>"); // store the currently selected datasetId in the DOM
-        htmls.push("</div>"); // tpDatasetBrowser
-
         var selDatasetIdx = 0;
 
-        var buttons = [];
+        var buttons = {}
         if (db !== null) {
-            var cancelLabel = "Cancel";
-            if (onlyInfo)
-                cancelLabel = "Close";
-            buttons.push({
-                text: cancelLabel,
-                click: function() {
-                    $(this).dialog("close");
-                    if (openDsInfo.isCollection)
-                        openDatasetDialog(openDsInfo, null); // show top-level dialog
-                }
-            });
+            buttons["Cancel"] = function() {
+                $(this).dialog("close");
+            };
         }
 
-        $(".ui-dialog-content").dialog("close"); // close the last dialog box
-
-        showDialogBox(htmls, title, {
+        showDialogBox(htmls, "Choose Cell Browser Dataset", {
             width: winWidth,
             height: winHeight,
             buttons: buttons
         });
 
-        $("#tpOpenDialogTabs").tabs();
-
-        // little helper function
-        function activateFilterCombo(valList, comboId) {
-            if (valList) {
-                activateCombobox(comboId, 200);
-                $("#" + comboId).change(onFilterChange);
+        $("button.list-group-item").eq(selDatasetIdx).css("z-index", "1000"); // fix up first overlap
+        $("button.list-group-item").keypress(function(e) {
+            // load the current dataset when the user presses Return
+            if (e.which == '13') {
+                var datasetName = gDatasetList[selDatasetIdx].name;
+                loadDataset(datasetName, true);
+                $(".ui-dialog-content").dialog("close");
             }
-        }
-
-        if (doFilters) {
-            activateFilterCombo(bodyParts, "tpBodyCombo");
-            activateFilterCombo(diseases, "tpDisCombo");
-            activateFilterCombo(organisms, "tpOrgCombo");
-            activateFilterCombo(projects, "tpProjCombo");
-            activateFilterCombo(lifeStages, "tpStageCombo");
-            activateFilterCombo(domains, "tpDomCombo");
-            activateFilterCombo(sources, "tpSourceCombo");
-        }
-
-        $('.tpBackLink').click(function(ev) {
-            let openDatasetName = $(ev.target).attr('data-open-dataset');
-            let selDatasetName = $(ev.target).attr('data-sel-dataset');
-            loadCollectionInfo(openDatasetName, function(newCollInfo) {
-                openDatasetDialog(newCollInfo, selDatasetName);
-            });
-            changeUrl({
-                "ds": openDatasetName.replace(/\//g, " ")
-            });
         });
 
-        var focused = document.activeElement;
-        var scroller = $("#tpDatasetList").overlayScrollbars({});
-        $(focused).focus();
+        $(".list-group-item").click(function(ev) {
+            selDatasetIdx = parseInt($(ev.target).data('datasetid')); // index of clicked dataset
+            $(".list-group-item").removeClass("active");
+            $('#tpDatasetButton_' + selDatasetIdx).bsButton("toggle"); // had to rename .button() in .html
+            openDatasetLoadPane(selDatasetIdx);
+        });
 
+        $(".load-dataset").click(function(ev) {
+            ev.preventDefault();
+            selDatasetIdx = parseInt($(this).parents('.list-group-item').data('datasetid'));
+            var datasetName = gDatasetList[selDatasetIdx].name;
+            loadDataset(datasetName, true);
+            $(".ui-dialog-content").dialog("close");
+            return false;
+        });
 
         $("#tabLink1").tab("show");
 
-        if (activeIdx !== null && !onlyInfo) {
-            if (activeIdx !== 0)
-                scroller.scroll($("#tpDatasetButton_" + activeIdx)); // scroll left pane to current button
-            $("tpDatasetButton_" + activeIdx).addClass("active");
-        }
+        $(".list-group-item").focus(function(event) {
+            selDatasetIdx = parseInt($(event.target).data('datasetid')); // index of clicked dataset
+            // bootstrap has a bug where the blue selection frame is hidden by neighboring buttons
+            // we're working around this here by bumping up the current z-index.
+            $("button.list-group-item").css("z-index", "0");
+            $("button.list-group-item").eq(selDatasetIdx).css("z-index", "1000");
+        });
+
+        if (activeIdx !== null)
+            $('#tpDatasetButton_' + activeIdx).bsButton("toggle"); // had to rename .button() in .html to bsButton
+
+        // this is weird, but I have not found a better way to make the tab show up
+        $("#tpOpenDialogTabs a:last").tab("show");
+        $("#tpOpenDialogTabs a:first").tab("show");
 
-        if (getVarSafe("ds") === undefined) // only filter on the top level
-            filterDatasetsDom();
-        connectOpenPane(selDatasetIdx, datasetList);
         // finally, activate the default pane and load its html
-        openDatasetLoadPane(openDsInfo);
+        $("button.list-group-item").eq(activeIdx).trigger("focus");
+        openDatasetLoadPane(activeIdx);
     }
 
-
-    function onSelChange(selection) {
-        /* called each time when the selection has been changed */
-        var cellIds = [];
-        selection.forEach(function(x) {
-            cellIds.push(x)
-        });
-        $("#tpSetBackground").parent("li").removeClass("disabled");
-
-        if (cellIds.length === 0 || cellIds === null) {
-            clearMetaAndGene();
-            clearSelectionState();
-            $("#tpSetBackground").parent("li").addClass("disabled");
-        } else if (cellIds.length === 1) {
-            $("#tpHoverHint").hide();
-            $("#tpSelectHint").show();
-            var cellId = cellIds[0];
-            var cellCountBelow = cellIds.length - 1;
-            updateMetaBarCustomFields(cellId);
-            db.loadMetaForCell(cellId, function(ci) {
-                updateMetaBarOneCell(ci, cellCountBelow);
-            }, onProgress);
-        } else {
-            $("#tpHoverHint").hide();
-            $("#tpSelectHint").show();
-            updateMetaBarManyCells(cellIds);
+    function drawLayoutMenu() {
+        /* Add the View / Layout menu to the DOM */
+        var htmls = [];
+        var coordFiles = gCurrentDataset.coordFiles;
+        for (var i = 0; i < coordFiles.length; i++) {
+            var label = coordFiles[i].shortLabel;
+            if (label === undefined) {
+                label = "Dataset " + i;
+                console.log("Dataset " + i + " has no 'shortLabel' attribute");
+            }
+            htmls.push('<li><a href="#" class="tpDataset" id="' + i + '">' + label + '</a></li>');
         }
+        $("#tpLayoutMenu").empty();
+        $("#tpLayoutMenu").append(htmls.join(""));
+    }
 
+    function onSelChange(cellIds) {
+        /* called each time when the selection has been changed */
         updateGeneTableColors(cellIds);
         if ("geneSym" in gLegend)
             buildViolinPlot();
 
-        var cols = renderer.col.arr;
-        var selectedLegends = {};
-        for (var i = 0; i < gLegend.rows.length; i++) {
-            selectedLegends[i] = 0;
-        }
-        selection.forEach(function(cellId) {
-            selectedLegends[cols[cellId]]++;
-        });
-        for (var i = 0; i < gLegend.rows.length; i++) {
-            if (selectedLegends[i] == gLegend.rows[i].count) {
-                $("#tpLegendCheckbox_" + i).prop("checked", true);
-            } else {
-                $("#tpLegendCheckbox_" + i).prop("checked", false);
-            }
-        }
-        updateLegendGrandCheckbox();
+        //if (cellIds.length===0)
+        //clearMetaAndGene();
+        //else if (cellIds.length===1)
+        //updateMetaBarOneCell(cellIds[0]);
+        //else
+        //updateMetaBarManyCells(cellIds);
     }
 
     function onSaveAsClick() {
         /* File - Save Image as ... */
         var canvas = $("canvas")[0];
         canvas.toBlob(function(blob) {
             saveAs(blob, "cellBrowser.png");
         }, "image/png");
     }
 
-    function onSaveAsSvgClick() {
-        /* File - Save Image as vector ... */
-        renderer.drawDots("svg")
-        renderer.drawLegendSvg(gLegend, 200)
-        var lines = renderer.getSvgText()
-        var blob = new Blob(lines, {
-            type: "image/svg+xml"
-        });
-        window.saveAs(blob, "cellBrowser.svg");
+    function onDownloadClick() {
+        /* user clicks one of the "download data" submenu links: matrix, meta or coords  */
+        var name = event.target.id.split("_")[1]; // the name of the dataset
+        var baseUrl = gCurrentDataset.baseUrl;
+        var url = null;
+        if (name === "matrix") {
+            url = joinPaths([baseUrl, "geneMatrix.tsv"]);
+            // hack for aparna, to send the original matrix
+            if (baseUrl === "aparna/" || baseUrl === "aparna")
+                url = joinPaths([baseUrl, "matrix.tsv.gz"]);
+            document.location.href = url;
+        }
+        if (name === "meta") {
+            url = joinPaths([baseUrl, "meta.tsv"]);
+            document.location.href = url;
+        }
     }
 
     function onSelectAllClick() {
         /* Edit - select all visible*/
-        clearSelectionState();
         renderer.selectClear();
         renderer.selectVisible();
+        //updateSelection();
         renderer.drawDots();
     }
 
     function onSelectNoneClick() {
         /* Edit - Select None */
-        clearSelectionState();
         renderer.selectClear();
         renderer.drawDots();
     }
 
-    function onSelectInvertClick() {
-        /* Edit - Invert selection */
-        clearSelectionState();
-        renderer.selectInvert();
-        renderer.drawDots();
-    }
-
-    function buildOneComboboxRow(htmls, comboWidth, rowIdx, queryExpr) {
+    function buildOneComboboxRow(htmls, comboWidth, rowIdx) {
         /* create one row of combobox elements in the select dialog */
-        htmls.push('<div class="tpSelectRow" id="tpSelectRow_' + rowIdx + '">');
-        // or &#x274e; ?
-        htmls.push('<span style="cursor: default; font-size:1.2em" id="tpSelectRemove_' + rowIdx + '">&#xd7;</span>&nbsp;'); // unicode: mult sign
+        htmls.push('<div>');
         htmls.push('<select name="type" id="tpSelectType_' + rowIdx + '">');
         htmls.push('<option value="meta">Cell annotation field</option><option value="expr">Expression of gene </option>');
         htmls.push('</select>');
 
         buildMetaFieldCombo(htmls, "tpSelectMetaComboBox_" + rowIdx, "tpSelectMetaCombo_" + rowIdx, 0);
 
         var id = "tpSelectGeneCombo_" + rowIdx;
         htmls.push('<select style="width:' + comboWidth + 'px" id="' + id + '" placeholder="gene search..." class="tpCombo">');
         htmls.push('</select>');
 
         htmls.push('<select name="operator" id="tpSelectOperator_' + rowIdx + '">');
-        htmls.push('<option value="eq" selected>is equal to</option>');
-        htmls.push('<option value="neq" selected>is not equal to</option>');
+        htmls.push('<option value="eq">is equal to</option>');
         htmls.push('<option value="gt">is greater than</option>');
         htmls.push('<option value="lt">is less than</option>');
         htmls.push('</select>');
 
-        htmls.push('<input id="tpSelectValue_' + rowIdx + '" type="text" name="exprValue">');
-        htmls.push('</input>');
+        htmls.push('<input id="tpSelectValue_' + rowIdx + '" type="text" name="exprValue"></input>');
 
-        htmls.push('<select style="max-width: 300px" id="tpSelectMetaValueEnum_' + rowIdx + '" name="metaValue">');
+        htmls.push('<select id="tpSelectMetaValueEnum_' + rowIdx + '" name="metaValue">');
         htmls.push('</select>');
-        htmls.push('</div>'); // tpSelectRow_<rowIdx>
 
         htmls.push('<p>');
     }
 
-    function findCellsUpdateMetaCombo(rowIdx, fieldIdx) {
-        /* given the row and the ID name of the field, setup the combo box row */
-        var metaInfo = db.getMetaFields()[fieldIdx];
-        var valCounts = metaInfo.valCounts;
-        var shortLabels = metaInfo.ui.shortLabels;
-        $('#tpSelectMetaCombo_' + rowIdx).val("tpMetaVal_" + fieldIdx).trigger('chosen:updated'); // update the meta dropdown
-
-        if (valCounts === undefined) {
-            // this is a numeric field
-            $('#tpSelectValue_' + rowIdx).val("");
-            $('#tpSelectValue_' + rowIdx).show();
-            $('#tpSelectMetaValueEnum_' + rowIdx).hide();
-        } else {
-            // it's an enum field
-            $('#tpSelectValue_' + rowIdx).hide();
-            $('#tpSelectMetaValueEnum_' + rowIdx).empty();
-            for (var i = 0; i < valCounts.length; i++) {
-                //var valName = valCounts[i][0];
-                var valLabel = shortLabels[i];
-                $('#tpSelectMetaValueEnum_' + rowIdx).append("<option value='" + i + "'>" + valLabel + "</option>");
-            }
-            $('#tpSelectMetaValueEnum_' + rowIdx).show();
-        }
-    }
-
-    function findCellsUpdateRowType(rowIdx, rowType) {
-        if (rowType === "meta") {
-            $("#tpSelectType_" + rowIdx).val("meta");
-            $("#tpSelectGeneCombo_" + rowIdx).next().hide();
-            $("#tpSelectValue_" + rowIdx).hide();
-            $("#tpSelectMetaComboBox_" + rowIdx).show();
-            $("#tpSelectMetaValueEnum_" + rowIdx).show();
-        } else {
-            $("#tpSelectType_" + rowIdx).val("expr");
-            $("#tpSelectGeneCombo_" + rowIdx).next().show();
-            $("#tpSelectValue_" + rowIdx).show();
-            $("#tpSelectMetaComboBox_" + rowIdx).hide();
-            $("#tpSelectMetaValueEnum_" + rowIdx).hide();
-        }
-    }
-
-    function connectOneComboboxRow(comboWidth, rowIdx, query) {
-        /* Filter dialog. Call the jquery inits and setup the change listeners for a combobox row */
-        /* Yes, a UI framework, like react or angular, would be very helpful here */
-
-        // first of all: check if the meta name actually exists in this dataset still
-        let metaInfo = null;
-        var metaName = query["m"];
-        if (metaName !== undefined) {
-            metaInfo = db.findMetaInfo(metaName);
-            if (metaInfo === null)
-                return;
-        }
+    function connectOneComboboxRow(comboWidth, rowIdx) {
+        /* call the jquery inits and setup the change listeners for a combobox row */
+        /* a UI framework, like react or angular, would be very helpful here */
 
         // auto-suggest for gene searches
         $('#tpSelectGeneCombo_' + rowIdx).selectize({
             "labelField": 'text',
             "valueField": 'id',
             "searchField": 'text',
-            "load": comboLoadGene,
+            "load": geneComboSearch
         });
         activateCombobox("tpSelectMetaCombo_" + rowIdx, comboWidth);
 
-        $('#tpSelectRemove_' + rowIdx).click(function(ev) {
-            //console.log(ev);
-            var rowToDel = (this.id).split("_")[1];
-            $("#tpSelectRow_" + rowToDel).remove();
-        });
-
-        //$("#tpSelectGeneCombo_"+rowIdx).next().hide();
-        //$("#tpSelectValue_"+rowIdx).hide();
-
-
-        var rowType = "gene";
-        var op = getQueryOp(query);
-        if (metaName === undefined) {
-            // this is a gene query
-            findCellsUpdateRowType(rowIdx, rowType);
-            selectizeSetValue("#tpSelectGeneCombo_" + rowIdx, query["g"]);
-            $("#tpSelectValue_" + rowIdx).val(query[op]);
-        } else {
-            // it's a meta query
-            rowType = "meta";
-            findCellsUpdateRowType(rowIdx, rowType);
-            findCellsUpdateMetaCombo(rowIdx, metaInfo.index);
-            var enumIdx = findMetaValIndex(metaInfo, query[op]);
-            $("#tpSelectMetaValueEnum_" + rowIdx).val(enumIdx);
-        }
-        $("#tpSelectOperator_" + rowIdx).val(op);
+        $("#tpSelectGeneCombo_" + rowIdx).next().hide();
+        $("#tpSelectValue_" + rowIdx).hide();
 
         $('#tpSelectMetaCombo_' + rowIdx).change(function(ev) {
             // when the user changes the meta field, update the list of meta field values in the dropdown
             var selVal = this.value;
-            var fieldIdx = parseInt(selVal.split("_")[1]);
-            findCellsUpdateMetaCombo(rowIdx, fieldIdx);
+            var fieldId = parseInt(selVal.split("_")[1]);
+            var valCounts = db.getMetaFields()[fieldId].valCounts;
+            if (valCounts === undefined) {
+                $('#tpSelectValue_' + rowIdx).show();
+                $('#tpSelectMetaValueEnum_' + rowIdx).hide();
+            } else {
+                $('#tpSelectValue_' + rowIdx).hide();
+                $('#tpSelectMetaValueEnum_' + rowIdx).empty();
+                for (var i = 0; i < valCounts.length; i++) {
+                    var valName = valCounts[i][0];
+                    $('#tpSelectMetaValueEnum_' + rowIdx).append("<option value='" + i + "'>" + valName + "</option>");
+                }
+                $('#tpSelectMetaValueEnum_' + rowIdx).show();
+            }
         });
 
         $('#tpSelectType_' + rowIdx).change(function(ev) {
             // when the user changes the gene expression / meta dropdown, hide/show the
             // respective other dropdowns
-            var rowType = this.value;
-            findCellsUpdateRowType(rowIdx, rowType);
+            if (this.value === "meta") {
+                $("#tpSelectGeneCombo_" + rowIdx).next().hide();
+                $("#tpSelectValue_" + rowIdx).hide();
+                $("#tpSelectMetaComboBox_" + rowIdx).show();
+                $('#tpSelectMetaCombo_' + rowIdx).val(0).trigger('chosen:updated'); // empty the meta dropdown
+                $("#tpSelectMetaValueEnum_" + rowIdx).show();
+            } else {
+                $("#tpSelectGeneCombo_" + rowIdx).next().show();
+                $("#tpSelectValue_" + rowIdx).show();
+                $("#tpSelectMetaComboBox_" + rowIdx).hide();
+                $("#tpSelectMetaValueEnum_" + rowIdx).hide();
+            }
         });
     }
 
     function readSelectForm() {
         /* convert the current state of the dialog box to a short string and return it */
         // example: [{"g":"PITX2", "gt":0.05}, {"m":"Cluster", "eq":"cluster 2"}]
         // XX TODO: non-enum meta data fields ???
         var queries = [];
 
-        var rowCount = $(".tpSelectRow").length;
-        for (var rowIdx = 0; rowIdx < rowCount; rowIdx++) {
+        var rowIdx = 1;
+        while ($("#tpSelectOperator_" + rowIdx).length > 0) {
             var query = {};
             var op = $('#tpSelectOperator_' + rowIdx).val();
 
             var queryType = $('#tpSelectType_' + rowIdx).val();
-            if (queryType === "expr") {
+            if (queryType == "expr") {
                 var gene = $('#tpSelectGeneCombo_' + rowIdx).val();
                 var val = $('#tpSelectValue_' + rowIdx).val();
                 query["g"] = gene;
                 query[op] = val;
             } else {
                 var metaValTag = $('#tpSelectMetaCombo_' + rowIdx).val();
                 var metaIdx = parseInt(metaValTag.split("_")[1]);
-                var metaInfo = db.conf.metaFields[metaIdx];
-                var metaName = metaInfo.name;
+                var metaName = db.conf.metaFields[metaIdx].name;
                 query["m"] = metaName;
 
-                var opVal = null;
-                var selOp = null;
-                if (metaInfo.type === "enum") {
-                    let selVal = $('#tpSelectMetaValueEnum_' + rowIdx).val();
-                    var valIdx = parseInt(selVal);
-                    opVal = db.conf.metaFields[metaIdx].valCounts[valIdx][0];
-                } else {
-                    let selVal = $('#tpSelectValue_' + rowIdx).val();
-                    opVal = parseFloat(selVal);
-                }
-
-                query[op] = opVal;
+                var selVal = $('#tpSelectMetaValueEnum_' + rowIdx).val();
+                var valIdx = parseInt(selVal);
+                var val = db.conf.metaFields[metaIdx].valCounts[valIdx][0];
+                query[op] = val;
             }
             queries.push(query);
+            rowIdx++;
         }
         return queries;
     }
 
     function greaterThan(x, y) {
         return (x > y);
     }
@@ -1855,42 +645,27 @@
         return (x < y);
     }
 
     function equals(x, y) {
         return (x === y);
     }
 
-    function notequals(x, y) {
-        return (x !== y);
-    }
-
-    function getQueryOp(query) {
-        if ("eq" in query) return "eq";
-        if ("neq" in query) return "neq";
-        if ("gt" in query) return "gt";
-        if ("lt" in query) return "lt";
-    }
-
     function makeFuncAndVal(query) {
         /* return a comparator function and the value given a query object */
         var compFunc = equals;
-        var val = query["eq"];
-
-        if ("lt" in query) {
+        if ("lt" in query)
             compFunc = lessThan;
-            val = query["lt"];
-        }
-        if ("gt" in query) {
+        if ("gt" in query)
             compFunc = greaterThan;
-            val = query["gt"];
-        }
-        if ("neq" in query) {
-            compFunc = notequals;
-            val = query["neq"];
-        }
+
+        var val = query["eq"]
+        if (val === undefined)
+            val = query["lt"]
+        if (val === undefined)
+            val = query["gt"]
 
         return [compFunc, val];
     }
 
     function searchArrayForFuncAndVal(arr, funcAndVal) {
         /* given an array and function and a value, return an array with the indices the matching array elements */
         var compFunc = funcAndVal[0];
@@ -1899,296 +674,126 @@
         for (var i = 0; i < arr.length; i++) {
             if (compFunc(arr[i], compVal))
                 selCells.push(i);
         }
         return selCells;
     }
 
+    function intersectArrays(arrList) {
+        /* return the intersection of all arrays as an array. Non-IE11? */
+        var smallSet = new Set(arrList[0]);
+        for (var i = 1; i < arrList.length; i++) {
+            var otherSet = new Set(arrList[i]);
+            smallSet = new Set([...smallSet].filter(x => otherSet.has(x)));
+        }
+        var newArr = Array.from(smallSet);
+        return newArr;
+    }
+
     function findCellsMatchingQueryList(queries, onDone) {
         /* given a list of dicts, return the identifiers of the matching cells */
         /* example: [{"g":"PITX2", "gt":0.05}, {"m":"Cluster", "eq":"cluster 2"}] */
 
         var doneQueries = 0;
-        var queryResults = [];
+        var queryResults = []
 
         function allQueriesDone() {
             // XX this could use a promise framework
             if (queryResults.length === 1)
                 onDone(queryResults[0]);
             else
                 onDone(intersectArrays(queryResults));
         }
 
         function gotGeneVec(exprArr, sym, desc, funcVal) {
-            funcVal[1] = Number(funcVal[1]); // for gene queries, must be a number, not string
-            var selCells = searchArrayForFuncAndVal(exprArr, funcVal);
+            var selCells = searchArrayForFuncAndVal(exprArr, funcVal)
             queryResults.push(selCells);
             doneQueries++;
-            if (doneQueries === queries.length)
+            if (doneQueries == queries.length)
                 allQueriesDone();
         }
 
         function gotMetaArr(metaArr, metaInfo, funcVal) {
-            /* filter meta data array with funcVal = function + value  */
-            if (metaInfo.origVals)
-                metaArr = metaInfo.origVals; // numerical meta fields have the original numbers stored
-            var selCells = searchArrayForFuncAndVal(metaArr, funcVal);
+            var selCells = searchArrayForFuncAndVal(metaArr, funcVal)
             queryResults.push(selCells);
             doneQueries++;
-            if (doneQueries === queries.length)
+            if (doneQueries == queries.length)
                 allQueriesDone();
         }
 
         var selCells = [];
         for (var i = 0; i < queries.length; i++) {
             var query = queries[i];
             var funcVal = makeFuncAndVal(query); // [0] = function to compare, [1] = value for comparison
             if ("g" in query) {
                 db.loadExprVec(query.g, gotGeneVec, null, funcVal);
             } else {
                 var fieldName = query.m;
                 var fieldIdx = cbUtil.findIdxWhereEq(db.conf.metaFields, "name", fieldName);
                 var findVal = funcVal[1];
-
-                var metaInfo = db.getMetaFields()[fieldIdx];
-                if (metaInfo.type === "enum")
-                    findVal = findMetaValIndex(metaInfo, findVal);
-
-                let searchDesc = [funcVal[0], findVal];
-
-                if (metaInfo.origVals)
-                    // for numeric fields, the raw data is already in memory
-                    gotMetaArr(metaInfo.origVals, metaInfo, searchDesc)
-                else
-                    // other fields may not be loaded yet
-                    db.loadMetaVec(metaInfo, gotMetaArr, null, searchDesc);
+                var fieldValIdx = findMetaValIndex(fieldIdx, findVal);
+                db.loadMetaVec(fieldIdx, gotMetaArr, null, [funcVal[0], fieldValIdx]);
             }
         }
     }
 
-    function makeSampleQuery() {
-        /* find first enum meta field and return a query for its name and its first value */
-        var metaFieldInfo = db.conf.metaFields;
-        for (var i = 0; i < metaFieldInfo.length; i++) {
-            var field = metaFieldInfo[i];
-            if (field.type !== "enum")
-                continue;
-            var fieldName = field.name;
-            var val1 = field.valCounts[0][0];
-            return {
-                "m": fieldName,
-                "eq": val1
-            };
-        }
-    }
-
-    function addNewAnnotation(fieldLabel, newMetaValue, cellIds) {
-        var metaInfo;
-        let cellCount = db.conf.sampleCount;
-        if (!db.getMetaFields()[0].isCustom) {
-            // add a new enum meta field
-            metaInfo = {
-                name: "custom",
-                label: fieldLabel,
-                type: "enum",
-                arr: Array.from(new Uint8Array(cellCount)), // cannot JSON-serialize Typed Arrays
-                ui: {
-                    shortLabels: ["No annotation"]
-                },
-                valCounts: [
-                    ["No annotation", cellCount]
-                ]
-            }
-            db.addCustomMetaField(metaInfo);
-            rebuildMetaPanel();
-            activateTab("meta");
-        } else
-            metaInfo = db.getMetaFields()[0];
-
-        metaInfo.ui.shortLabels.push(newMetaValue);
-        let newValIdx = metaInfo.valCounts.length;
-        metaInfo.valCounts.push([newMetaValue, cellIds.length]);
-        // update the "No annotation" count
-        let noAnnotCount = metaInfo.valCounts[0][1];
-        metaInfo.valCounts[0][1] = noAnnotCount - cellIds.length;
-
-        let arr = metaInfo.arr;
-        for (let i = 0; i < cellIds.length; i++)
-            arr[cellIds[i]] = newValIdx;
-        // need to update the value histogram
-        db.metaHist[metaInfo.name] = makeFieldHistogram(metaInfo, cellIds, arr);
-        updateMetaBarManyCells(cellIds); // redo, as we rebuilt the meta panel
-
-        var jsonStr = JSON.stringify(metaInfo);
-        var comprStr = LZString.compress(jsonStr);
-        localStorage.setItem(db.name + "|custom", comprStr);
-    }
-
-    function onSelectNameClick() {
-        /* Edit > Name selection */
-
-        let title = "Annotate selected " + gSampleDesc + "s";
-
-        let htmls = [];
-        htmls.push('<p>There are ' + renderer.getSelection().length + ' ' + gSampleDesc + ' in the current selection.</p>');
-
-        htmls.push('<p><b>Name of annotation field</b>:<br>');
-        htmls.push('<input class="tpDialogInput" id="tpFieldLabel" type="text" value="My custom annotations"></p>');
-        htmls.push('<p><b>Annotate selected cells as:</b><br>');
-        htmls.push('<input class="tpDialogInput" id="tpMetaVal" type="text"></p>');
-        htmls.push('<p>Remove annotations later by clicking <b>Tools > Remove all annotations</b>.</p>');
+    function onSelectComplexClick() {
+        /* Edit - Find cells */
 
         var dlgHeight = 400;
-        var dlgWidth = 800;
-        var buttons = [
-            //"Close and remove all annotations" : function() {
-            //db.getMetaFields().shift();
-            //rebuildMetaPanel();
-            //localStorage.removeItem(db.name+"|custom");
-            //resetCustomAnnotations();
-            //},
-            {
-                text: "OK",
-                click: function() {
-                    let fieldLabel = $('#tpFieldLabel').val();
-                    if (fieldLabel === "")
-                        fieldLabel = "My custom annotations";
-                    let newMetaValue = $("#tpMetaVal").val();
-                    if (newMetaValue === "")
-                        return;
-
-                    addNewAnnotation(fieldLabel, newMetaValue, renderer.getSelection());
-                    $(this).dialog("close");
-                    colorByMetaField("custom");
-                }
-            }
-        ];
-        showDialogBox(htmls, title, {
-            showClose: true,
-            height: dlgHeight,
-            width: dlgWidth,
-            buttons: buttons
-        });
-        $("#tpMetaVal").focus();
-        return true;
-    }
-
-    function onBackgroudSetClick() {
-        // Tools -> Set cells as background
-        if ($("#tpSetBackground").parent("li").hasClass("disabled")) {
-            return;
-        }
-
-        background = renderer.getSelection();
-        $("#tpResetBackground").parent("li").removeClass("disabled");
-        if ("geneSym" in gLegend)
-            buildViolinPlot();
-    }
+        var dlgWidth = 700;
+        var buttons = {
 
-    function onBackgroudResetClick() {
-        // Tools -> Reset background cells
-        background = null;
-        $("#tpResetBackground").parent("li").addClass("disabled");
-        if ("geneSym" in gLegend)
-            buildViolinPlot();
-    }
+            "Cancel": function() {
+                $(this).dialog("close");
+            },
 
-    function saveQueryList(queryList) {
-        var queryStr = JSURL.stringify(queryList);
-        changeUrl({
-            'select': queryStr
-        });
-        localStorage.setItem(db.name + "|select", queryStr);
-    }
+            "OK": function() {
+                var queryList = readSelectForm();
 
-    function selectByQueryList(queryList) {
-        /* select cells defined by query list, save to local storage and URL and redraw */
-        findCellsMatchingQueryList(queryList, function(cellIds) {
-            if (cellIds.length === 0) {
-                alert("No matching " + gSampleDesc + "s.");
-            } else {
-                renderer.selectSet(cellIds);
-                saveQueryList(queryList);
+                findCellsMatchingQueryList(queryList, function(cellIds) {
+                    if (cellIds.length === 0) {
+                        alert("No matching " + gSampleDesc + ".");
+                    } else {
+                        renderer.selectSet(cellIds);
+                        changeUrl({
+                            'select': JSON.stringify(queryList)
+                        });
+                        renderer.drawDots();
+                        $("#tpDialog").dialog("close");
+                    }
+                });
             }
-        });
-    }
 
-    function onFindCellsClick() {
-        /* Edit - Find cells */
-
-        var dlgHeight = 400;
-        var dlgWidth = 800;
-        var buttons = [
-            //{
-            //text:"Cancel",
-            //click:function() {
-            //// save state even if user presses cancel  - good idea?
-            //var queryStr = JSURL.stringify(queryList);
-            //var queryList = readSelectForm();
-            //localStorage.setItem(db.name+"|select", queryStr);
-            //$(this).dialog("close");
-            //}
-            //},
-            {
-                text: "OK",
-                click: function() {
-                    var queryList = readSelectForm();
-                    selectByQueryList(queryList);
-                    $("#tpDialog").dialog("close");
-                    renderer.drawDots();
-                }
-            }
-        ];
+        };
 
         var htmls = [];
 
-        // build from current query or create a sample query
-        var queries = [];
-        var queryStr = getVar("select");
-
-        if (queryStr === undefined)
-            queryStr = localStorage.getItem(db.name + "|select");
-
-        if (queryStr === undefined || queryStr === null)
-            queries = [makeSampleQuery()];
-        else {
-            queries = JSURL.parse(queryStr);
-        }
-
-        var comboWidth = 250;
-
-        var query;
-        for (var i = 0; i < queries.length; i++) {
-            query = queries[i];
-            buildOneComboboxRow(htmls, comboWidth, i, query);
-        }
+        var comboWidth = 150;
+        buildOneComboboxRow(htmls, comboWidth, 1);
 
         htmls.push("<div id='tpSelectAddRowLink' class='link'>Add another search criterion</div>");
 
         showDialogBox(htmls, "Find cells based on annotation or gene expression", {
             showClose: true,
             height: dlgHeight,
             width: dlgWidth,
             buttons: buttons
         });
 
+        connectOneComboboxRow(comboWidth, 1);
 
-        for (i = 0; i < queries.length; i++) {
-            query = queries[i];
-            connectOneComboboxRow(comboWidth, i, query);
-        }
-
-        var rowIdx = queries.length + 1;
+        var rowIdx = 2;
         $('#tpSelectAddRowLink').click(function(ev) {
             var htmls = [];
-            var rowIdx = $(".tpSelectRow").length;
-            var newRowQuery = makeSampleQuery();
-            buildOneComboboxRow(htmls, comboWidth, rowIdx, newRowQuery);
+            buildOneComboboxRow(htmls, comboWidth, rowIdx);
             $(htmls.join("")).insertBefore("#tpSelectAddRowLink");
-            connectOneComboboxRow(comboWidth, rowIdx, newRowQuery);
+            //$('#tpSelectAddRowLink').insertBefore();
+            connectOneComboboxRow(comboWidth, rowIdx);
+            rowIdx++;
         });
     }
 
     function onMarkClick() {
         /* Edit - mark selection (with arrows) */
         if (gCurrentDataset.markedCellIds === undefined)
             gCurrentDataset.markedCellIds = {};
@@ -2212,563 +817,175 @@
 
     function onMarkClearClick() {
         gCurrentDataset.markedCellIds = {};
         plotDots();
         renderer.render(stage);
     }
 
-    function cartSave(db) {
-        /* save db.cart dataset long-term changes that may be shared with others, like colors, labels, annotations, etc
-         * For now, save to localStorage and also to the URL. */
-
-        var datasetName = db.name;
-        var data = db.cart;
-        var key = "cart";
-
-        var fullKey = datasetName + "###" + key;
-        var jsonStr = JSON.stringify(data);
-        var comprStr = LZString.compress(jsonStr);
-        var uriStr = LZString.compressToEncodedURIComponent(jsonStr);
-        localStorage.setItem(fullKey, comprStr);
-        var urlData = {};
-        if (isEmpty(data))
-            uriStr = null;
-        urlData[key] = uriStr;
-        changeUrl(urlData);
-        console.log("Saving state: ", data);
-    }
-
-    function createMetaUiFields(db) {
-        /* This function changes db.metaFields[fieldName],
-         * it adds: .ui.shortLabels, .ui.longLabels, ui.palette and .ui.colors;
-         * ui info fields hold the final data as shown in the ui, they're calculated when the cart is loaded.
-         * apply changes like labels/color/etc stored the userMeta object to db.conf.metaFields.
-         * Potentially clean up the changes and recreate the cart object.
-         * Currently, this only does something for enum fields.
-         * */
-
-        if (db.cart === undefined)
-            db.cart = {};
-        var userMeta = db.cart;
-        if (userMeta === null)
-            alert("the 'cart' argument in the URL is invalid. Please remove cart=xxxx from the URL and reload");
-        var metaFields = db.conf.metaFields;
-
-        for (var metaIdx = 0; metaIdx < metaFields.length; metaIdx++) {
-            var metaInfo = metaFields[metaIdx];
-            var fieldChanges = userMeta[metaInfo.name] || {};
-
-            if (metaInfo.type !== "enum") {
-                metaInfo.ui = {};
-                continue;
-            }
-
-            // create shortLabels
-            var shortLabels = null;
-            var oldCounts = metaInfo.valCounts;
-            if (oldCounts) {
-                shortLabels = [];
-                for (var i = 0; i < oldCounts.length; i++)
-                    shortLabels.push(oldCounts[i][0]);
-                var newLabels = fieldChanges.shortLabels;
-                shortLabels = copyNonEmpty(newLabels, shortLabels);
-            }
-
-            // create the long labels
-            var longLabels = [];
-            if ("longLabels" in metaInfo)
-                longLabels = cloneArray(metaInfo.longLabels);
-            else
-                longLabels = cloneArray(shortLabels);
-            longLabels = copyNonEmpty(fieldChanges.longLabels, longLabels);
-
-            // create the colors: configured colors override default colors and cart overrides those
-            var colors = makeColorPalette(cDefQualPalette, metaInfo.valCounts.length);
-            if ("colors" in metaInfo)
-                copyNonNull(metaInfo.colors, colors);
-            var newColors = fieldChanges.colors;
-            colors = copyNonEmpty(newColors, colors);
-
-            var ui = {};
-            ui.colors = newColors;
-            ui.longLabels = longLabels;
-            ui.shortLabels = shortLabels;
-            metaInfo.ui = ui;
-        }
-
-        //var delFields = [];
-        //var delAttrs = [];
-        //if (metaInfo===null) { // field does not exist anymore
-        //delFields.push(fieldName);
-        //continue;
-        //}
-
-        // remove all fields and attributes that were found to be invalid in the current state
-        // so we don't accumulate crap
-        //var cleanedFields = [];
-        //for (var i = 0; i < delAttrs.length; i++) {
-        //var fieldName = delAttrs[i][0];
-        //var attrName = delAttrs[i][1];
-        //delete userMeta[fieldName][attrName];
-        //cleanedFields.push(fieldName);
-        //}
-
-        //for (var i = 0; i < delFields.length; i++) {
-        //var fieldName = delFields[i];
-        //delete userMeta[fieldName];
-        //cleanedFields.push(fieldName);
-        //}
-        //if (delAttrs.length!==0)
-        //warn("You had previously changed labels or colors or annotations but the dataset has been updated since then. "+
-        //"As a result, your annotations had to be removed. This concerned the following annotation fields: "+
-        //cleanedFields.join(", "));
-    }
-
-    function cartFieldArrayUpdate(db, metaInfo, key, pos, val) {
-        /* write val into db.cart[fieldName][key][pos], save the dataset cart and apply it.
-         * db.cart[fieldName][key] is an array of arrLen
-         * */
-        var cart = db.cart;
-        var fieldName = metaInfo.name;
-        var arrLen = metaInfo.valCounts.length;
-
-        if (!(fieldName in cart))
-            cart[fieldName] = {};
-
-        // init array
-        if (!(key in cart[fieldName])) {
-            var emptyArr = [];
-            for (var i = 0; i < arrLen; i++)
-                emptyArr.push("");
-            cart[fieldName][key] = emptyArr;
-        }
-
-        cart[fieldName][key][pos] = val;
-        cartSave(db);
-        createMetaUiFields(db);
-    }
-
-    function cartOverwrite(db, key, val) {
-        /* write val into db.cart[key][attr], save the dataset cart and apply it.
-         * attrName can be null in which case db.cart[key] will be replaced with val  */
-        var cart = db.cart;
-        if (!(key in db.cart))
-            cart[key] = {};
-
-        cart[key] = val;
-
-        cartSave(db);
-        createMetaUiFields(db);
-    }
-
-    function cartLoad(db) {
-        /* load the entire dataset cart from the URL or - if there is no cart on the URL - from localStorage */
-        var datasetName = db.name;
-        var cart = {};
-        var key = "cart";
-        var uriStr = getVar(key, null);
-        var jsonStr;
-        if (uriStr !== null) {
-            jsonStr = LZString.decompressFromEncodedURIComponent(uriStr);
-            cart = JSON.parse(jsonStr);
-            console.log("Loading cart from URL: ", cart);
-        } else {
-            var fullKey = datasetName + "###" + key;
-            var comprStr = localStorage.getItem(fullKey);
-            if (comprStr) {
-                jsonStr = LZString.decompress(comprStr);
-                cart = JSON.parse(jsonStr);
-                console.log("Loading cart from local storage: ", cart);
-            }
-        }
-        db.cart = cart;
-        createMetaUiFields(db);
-
-    }
-
-    function onRunClusteringClick() {
-        /* not used yet */
-        var myArray = new ArrayBuffer(512);
-        var longInt8View = new Uint8Array(myArray);
-
-        // generate some data
-        for (var i = 0; i < longInt8View.length; i++) {
-            longInt8View[i] = i % 256;
-        }
-
-        //let url = "http://localhost:5050/upload";
-        let url = "http://localhost:5050/bin";
-        var xhr = new XMLHttpRequest();
-        //xhr.open("POST", url, false);
-        xhr.open("GET", url, true);
-        xhr.responseType = "arraybuffer";
-        xhr.onload = function() {
-            var buf = xhr.response;
-            console.log(buf)
-        };
-        xhr.send(null);
-        //xhr.send(myArray);
-    }
-
-    function resetCustomAnnotations() {
-        db.removeAllCustomAnnots();
-        rebuildMetaPanel();
-        changeUrl({
-            "meta": null
-        });
-        colorByDefaultField();
-        localStorage.removeItem(db.name + "|custom");
-    }
-
-    function onCustomAnnotationsClick() {
-        /* */
-        if (!db.getMetaFields()[0].isCustom) {
-            alert("You have currently no custom annotations. Select a few cells and use Edit > Name selection " +
-                "to create a custom annotation field.");
-        } else {
-            resetCustomAnnotations();
-        }
-    }
-
-    function onRenameClustersClick() {
-        /* Tools - Rename Clusters */
-        var htmls = [];
-        htmls.push("<p>Change labels below. To keep the old name, leave the 'New Name' cell empty. You cannot modify the 'Orig. Name' column.</p>");
-        //htmls.push('<p>To rename a single cluster without this dialog: click onto it in the legend, then click its label.</p>');
-        htmls.push('<div id="tpGrid" style="width:100%;height:500px;"></div>');
-        var title = "Rename Clusters";
-        var dlgHeight = window.innerHeight - 100;
-        var dlgWidth = 650;
-
-        var clusterField = db.conf.labelField;
-
-        var data = [];
-
-        var buttons = [
-
-            {
-                text: "Empty All",
-                click: function() {
-                    for (var i = 0; i < data.length; i++) {
-                        var row = data[i];
-                        row["newName"] = "";
-                        row["mouseOver"] = "";
-                        row["color"] = "";
-                    }
-                    grid.invalidate();
-                }
-            }, {
-                text: "OK",
-                click: function() {
-                    Slick.GlobalEditorLock.commitCurrentEdit(); // save currently edited cell to data
-
-                    var shortLabels = [];
-                    var longLabels = [];
-                    var colors = [];
-
-                    for (var i = 0; i < data.length; i++) {
-                        var row = data[i];
-                        if (row["newName"] === row["origName"])
-                            shortLabels.push("");
-                        else
-                            shortLabels.push(row["newName"]);
-
-                        longLabels.push(row["mouseOver"]);
-                        colors.push(row["color"]);
-                    }
-
-                    var fieldMeta = {};
-
-                    if (!allEmpty(shortLabels))
-                        fieldMeta["shortLabels"] = shortLabels;
-                    if (!allEmpty(longLabels))
-                        fieldMeta["longLabels"] = longLabels;
-                    if (!allEmpty(colors))
-                        fieldMeta["colors"] = colors;
-
-                    cartOverwrite(db, clusterField, fieldMeta);
-                    var metaInfo = db.findMetaInfo(clusterField);
-
-                    renderer.setLabels(metaInfo.ui.shortLabels);
-
-                    // only need to update the legend if the current field is shown
-                    if (gLegend.type === "meta" && gLegend.metaInfo.name === clusterField) {
-                        //var shortLabels = findMetaInfo(clusterField).ui.shortLabels;
-                        legendUpdateLabels(clusterField);
-                        buildLegendBar();
-                    }
-
-                    $(this).dialog("close");
-                    renderer.drawDots();
-                }
-            },
-
-        ];
-
-        showDialogBox(htmls, title, {
-            showClose: true,
-            height: dlgHeight,
-            width: dlgWidth,
-            buttons: buttons
-        });
-
-        var columns = [{
-                id: "origName",
-                width: 100,
-                maxWidth: 200,
-                name: "Orig. Name",
-                field: "origName"
-            }, {
-                id: "newName",
-                width: 150,
-                maxWidth: 200,
-                name: "New Name",
-                field: "newName",
-                editor: Slick.Editors.Text
-            }, {
-                id: "mouseOver",
-                width: 200,
-                maxWidth: 300,
-                name: "Mouseover Label",
-                field: "mouseOver",
-                editor: Slick.Editors.Text
-            },
-            //{id: "color", width: 80, maxWidth: 120, name: "Color Code", field: "color", editor: Slick.Editors.Text}
-        ];
-
-        var options = {
-            editable: true,
-            enableCellNavigation: true,
-            enableColumnReorder: false,
-            enableAddRow: true,
-            //asyncEditorLoading: false,
-            autoEdit: true
-        };
-
-        var metaInfo = db.findMetaInfo(clusterField);
-
-        var fieldChanges = db.cart[clusterField] || {};
-
-        var shortLabels = fieldChanges["shortLabels"];
-        var longLabels = fieldChanges["longLabels"];
-        var colors = fieldChanges["colors"];
-
-        for (var i = 0; i < metaInfo.valCounts.length; i++) {
-            var shortLabel = "";
-            if (shortLabels)
-                shortLabel = shortLabels[i];
-
-            var longLabel = "";
-            if (longLabels)
-                longLabel = longLabels[i];
-
-            var color = "";
-            if (colors)
-                color = colors[i];
-
-            var valCount = metaInfo.valCounts[i];
-            var valRow = {
-                "origName": valCount[0],
-                "newName": shortLabel,
-                "mouseOver": longLabel,
-                "color": color
-            };
-            data.push(valRow);
-        }
-
-        var grid = new Slick.Grid("#tpGrid", data, columns, options);
-        grid.setSelectionModel(new Slick.CellSelectionModel());
-        grid.onAddNewRow.subscribe(function(e, args) {
-            var item = args.item;
-            grid.invalidateRow(data.length);
-            data.push(item);
-            grid.updateRowCount();
-            grid.render();
-        });
-    }
-
     function onSelectByIdClick() {
         /* Edit - select cells by ID */
-
-        function onSearchDone(searchRes) {
-            var idxArr = searchRes[0];
-            var notFoundIds = searchRes[1];
-
-            if (notFoundIds.length !== 0) {
-                $('#tpNotFoundIds').text("Could not find these IDs: " + notFoundIds.join(", "));
-                $('#tpNotFoundHint').text("Please fix them and click the OK button to try again.");
-            } else
-                $("#tpDialog").dialog("close");
-
-            renderer.selectSet(idxArr);
-            renderer.drawDots();
-        }
-
         var dlgHeight = 500;
         var dlgWidth = 500;
         var htmls = [];
-        var buttons = [{
-            text: "OK",
-            click: function() {
+        var buttons = {
+            "OK": function() {
                 var idListStr = $("#tpIdList").val();
                 idListStr = idListStr.trim().replace(/\r\n/g, "\n");
+                gSelCellIds = {};
+                if (idListStr === "")
+                    return;
+
+                // first check the IDs
+                var allCellIds = getAllCellIdsAsDict();
+                var notFoundIds = [];
                 var idList = idListStr.split("\n");
-                var re = new RegExp("\\*");
+                for (var i = 0; i < idList.length; i++) {
+                    var cellId = idList[i];
+                    if (cellId === "")
+                        continue;
+                    if (!(cellId in allCellIds))
+                        notFoundIds.push(cellId);
+                }
 
-                var hasWildcards = $("#tpHasWildcard")[0].checked;
-                db.loadFindCellIds(idList, onSearchDone, onProgressConsole, hasWildcards);
+                if (notFoundIds.length !== 0) {
+                    //alert("Could not find these "+gSampleDesc+" IDs:"+ notFoundIds.join(", "));
+                    $('#tpNotFoundIds').text("Could not find these IDs: " + notFoundIds.join(", "));
+                    $('#tpNotFoundHint').text("Please fix them and click the OK button to try again.");
+                } else {
+                    for (i = 0; i < idList.length; i++) {
+                        var cellId = idList[i];
+                        if (cellId === "")
+                            continue;
+                        gSelCellIds[cellId] = true;
+                    }
+                    $(this).dialog("close");
+                    //updateSelection();
+                    plotDots();
+                    renderer.render(stage);
+                    //alert(idList.length+ " " + gSampleDesc+"s are selected");
+                }
             }
-        }];
+        };
 
-        htmls.push("<textarea id='tpIdList' style='height:320px;width:400px;display:block'>");
+        htmls.push("<textarea id='tpIdList' style='height:320px;width:350px;display:block'>");
         htmls.push("</textarea><div id='tpNotFoundIds'></div><div id='tpNotFoundHint'></div>");
-        htmls.push("<input id='tpHasWildcard' type='checkbox' style='margin-right: 10px' /> Allow RegEx search, e.g. enter '^TH' to find all IDs that <br>start with 'TH' or '-1$' to find all IDs that end with '-1'");
         var title = "Paste a list of IDs (one per line) to select " + gSampleDesc + "s";
         showDialogBox(htmls, title, {
             showClose: true,
             height: dlgHeight,
             width: dlgWidth,
             buttons: buttons
         });
     }
 
     function onExportIdsClick() {
         /* Edit - Export cell IDs */
-        var selCells = renderer.getSelection();
-
-        function buildExportDialog(idList) {
-            /* callback when cellIds have arrived */
-            var dlgHeight = 500;
-
-            var htmls = [];
-            if (selCells.length === 0)
-                htmls.push("Shown below are the identifiers of all " + idList.length + " cells in the dataset.<p><p>");
+        var idList = [];
+        for (var cellId in gSelCellIds) {
+            idList.push(cellId);
+        }
 
-            var idListEnc = encodeURIComponent(idList.join("\n"));
-            htmls.push("<textarea style='height:320px;width:350px;display:block'>");
-            htmls.push(idList.join("\n"));
-            htmls.push("</textarea>");
-
-            var buttons = [{
-                text: "Download as file",
-                click: function() {
-                    var blob = new Blob([idList.join("\n")], {
-                        type: "text/plain;charset=utf-8"
-                    });
-                    saveAs(blob, "identifiers.txt");
-                },
-            }, {
-                text: "Copy to clipboard",
-                click: function() {
-                    $("textarea").select();
-                    document.execCommand('copy');
-                    $(this).dialog("close");
-                }
-            }];
+        var dlgHeight = 500;
 
-            let title = "List of " + idList.length + " selected IDs";
-            if (selCells.length === 0)
-                title = "No cells selected";
-
-            showDialogBox(htmls, title, {
-                showClose: true,
-                height: dlgHeight,
-                width: 500,
-                buttons: buttons
-            });
+        var htmls = [];
+        if (idList.length === 0) {
+            htmls.push("No cells are selected. Shown below are the identifiers of all cells visible on the screen.<p>");
+            for (var i = 0; i < pixelCoords.length; i++)
+                idList.push(shownCoords[i][0]);
         }
 
-        db.loadCellIds(selCells, buildExportDialog);
-    }
+        var idListEnc = encodeURIComponent(idList.join("\n"));
+        htmls.push("<textarea style='height:320px;width:350px;display:block'>");
+        htmls.push(idList.join("\n"));
+        htmls.push("</textarea>");
 
+        //htmls.push('<a style="text-decoration:underline" href="data:text/plain;charset=utf-8,'+idListEnc+'" download="identifiers.txt">Download as text file</a><br>');
 
-    function onAboutClick() {
-        /* user clicked on help > about */
-        var dlgHeight = 500;
+        //htmls.push('<a style="text-decoration:underline" href="data:text/plain;charset=utf-8,'+idListEnc+'" download="identifiers.txt">Download as text file</a><br>');
 
-        var htmls = [];
-        var title = "UCSC Cell Browser";
+        var buttons = {
+            "Download as file": function() {
+                var blob = new Blob([idList.join("\n")], {
+                    type: "text/plain;charset=utf-8"
+                });
+                saveAs(blob, "identifiers.txt");
+            },
+            "Copy to clipboard": function() {
+                $("textarea").select();
+                document.execCommand('copy');
+                $(this).dialog("close");
+            }
+        };
 
-        htmls.push("<p><b>Version:</b> " + gVersion + "</p>");
-        htmls.push("<p><b>Written by:</b> Maximilian Haeussler, Nikolay Markov (U Northwestern), Brian Raney, Lucas Seninge</p>");
-        htmls.push("<p><b>Testing / User interface / Documentation / Data import / User support:</b> Matt Speir, Brittney Wick</p>");
-        htmls.push("<p><b>Code contributions by:</b> Pablo Moreno (EBI, UK)</p>");
-        htmls.push("<p><b>Documentation:</b> <a class='link' target=_blank href='https://cellbrowser.readthedocs.io/'>Readthedocs</a></p>");
-        htmls.push("<p><b>Github Repo: </b><a class='link' target=_blank href='https://github.com/maximilianh/cellBrowser/'>cellBrowser</a></p>");
-        htmls.push("<p><b>Paper: </b><a class='link' target=_blank href='https://academic.oup.com/bioinformatics/advance-article/doi/10.1093/bioinformatics/btab503/6318386'>Speir et al, Bioinformatics 2021, DOI:10.1093/bioinformatics/btab503/6318386</a></p>");
 
-        showDialogBox(htmls, title, {
+        showDialogBox(htmls, "List of " + idList.length + " IDs", {
             showClose: true,
             height: dlgHeight,
-            width: 500
+            width: 400,
+            buttons: buttons
         });
     }
 
     function buildMenuBar() {
         /* draw the menubar at the top */
         var htmls = [];
-        htmls.push("<div style='width:" + menuBarHeight + "px' id='tpMenuBar'>");
+        htmls.push("<div id='tpMenuBar'>");
         htmls.push('<nav class="navbar navbar-default navbar-xs">');
 
         htmls.push('<div class="container-fluid">');
 
         htmls.push('<div class="navbar-header">');
         htmls.push('<a class="navbar-brand" href="#">' + gTitle + '</a>');
         htmls.push('</div>');
 
         htmls.push('<ul class="nav navbar-nav">');
 
         htmls.push('<li class="dropdown">');
         htmls.push('<a href="#" class="dropdown-toggle" data-toggle="dropdown" data-submenu role="button" aria-haspopup="true" aria-expanded="false">File</a>');
         htmls.push('<ul class="dropdown-menu">');
-        htmls.push('<li><a href="#" id="tpOpenDatasetLink"><span class="dropmenu-item-label">Open dataset...</span><span class="dropmenu-item-content">o</span></a></li>');
+        htmls.push('<li><a href="#" id="tpOpenDatasetLink"><span class="dropmenu-item-label">Open Dataset...</span><span class="dropmenu-item-content">o</span></a></li>');
         //htmls.push('<li class="dropdown-submenu"><a tabindex="0" href="#">Download Data</a>');
         //htmls.push('<ul class="dropdown-menu" id="tpDownloadMenu">');
         //htmls.push('<li><a href="#" id="tpDownload_matrix">Gene Expression Matrix</a></li>');
         //htmls.push('<li><a href="#" id="tpDownload_meta">Cell Metadata</a></li>');
         //htmls.push('<li><a href="#" id="tpDownload_coords">Visible coordinates</a></li>');
         //htmls.push('</ul>'); // Download sub-menu
-        htmls.push('<li><a href="#" id="tpSaveImage">Download bitmap image (PNG)</a></li>');
-        htmls.push('<li><a href="#" id="tpSaveImageSvg">Download vector image (SVG)</a></li>');
+        htmls.push('<li><a href="#" id="tpSaveImage">Download current image</a></li>');
         htmls.push('</li>'); // sub-menu container
 
         htmls.push('</ul>'); // File menu
         htmls.push('</li>'); // File dropdown
 
         htmls.push('<li class="dropdown">');
         htmls.push('<a href="#" class="dropdown-toggle" data-toggle="dropdown" data-submenu role="button" aria-haspopup="true" aria-expanded="false">Edit</a>');
         htmls.push('<ul class="dropdown-menu">');
-        htmls.push('<li><a id="tpSelectAll" href="#"><span class="dropmenu-item-label">Select all visible</span><span class="dropmenu-item-content">s a</span></a></li>');
-        htmls.push('<li><a id="tpSelectNone" href="#"><span class="dropmenu-item-label">Select none</span><span class="dropmenu-item-content">s n</span></a></li>');
-        htmls.push('<li><a id="tpSelectInvert" href="#"><span class="dropmenu-item-label">Invert selection</span><span class="dropmenu-item-content">s i</span></a></li>');
-        htmls.push('<li><a id="tpSelectName" href="#"><span class="dropmenu-item-label">Name selection...</span><span class="dropmenu-item-content">s s</span></a></li>');
-        htmls.push('<li><a id="tpExportIds" href="#">Export selected...</a></li>');
-        htmls.push('<li><a id="tpSelectComplex" href="#"><span class="dropmenu-item-label">Find cells...</span><span class="dropmenu-item-content">f c</span></a></li>');
+        htmls.push('<li><a id="tpSelectAll" href="#"><span class="dropmenu-item-label">Select all visible</span><span class="dropmenu-item-content">a</span></a></li>');
+        htmls.push('<li><a id="tpSelectNone" href="#"><span class="dropmenu-item-label">Select none</span><span class="dropmenu-item-content">n</span></a></li>');
+        htmls.push('<li><a id="tpSelectComplex" href="#"><span class="dropmenu-item-label">Find cells...</span><span class="dropmenu-item-content"></span></a></li>');
         //htmls.push('<li><a id="tpMark" href="#"><span class="dropmenu-item-label">Mark selected</span><span class="dropmenu-item-content">h m</span></a></li>');
         //htmls.push('<li><a id="tpMarkClear" href="#"><span class="dropmenu-item-label">Clear marks</span><span class="dropmenu-item-content">c m</span></a></li>');
-        htmls.push('<li><a id="tpSelectById" href="#">Find by ID...<span class="dropmenu-item-content">f i</span></a></li>');
+        //htmls.push('<li><a id="tpSelectById" href="#">Search for ID...</a></li>');
+        //htmls.push('<li><a id="tpExportIds" href="#">Export selected IDs...</a></li>');
         htmls.push('</ul>'); // View dropdown
         htmls.push('</li>'); // View dropdown
 
         htmls.push('<li class="dropdown">');
         htmls.push('<a href="#" class="dropdown-toggle" data-toggle="dropdown" data-submenu role="button" aria-haspopup="true" aria-expanded="false">View</a>');
         htmls.push('<ul class="dropdown-menu">');
 
         htmls.push('<li><a href="#" id="tpZoomPlus"><span class="dropmenu-item-label">Zoom in</span><span class="dropmenu-item-content">+</span></a></li>');
         htmls.push('<li><a href="#" id="tpZoomMinus"><span class="dropmenu-item-label">Zoom out</span><span class="dropmenu-item-content">-</span></a></li>');
         htmls.push('<li><a href="#" id="tpZoom100Menu"><span class="dropmenu-item-label">Zoom 100%</span><span class="dropmenu-item-content">space</span></a></li>');
-        htmls.push('<li><a href="#" id="tpSplitMenu"><span id="tpSplitMenuEntry" class="dropmenu-item-label">Split screen</span><span class="dropmenu-item-content">t</span></a></li>');
-        htmls.push('<li><a href="#" id="tpHeatMenu"><span id="tpHeatMenuEntry" class="dropmenu-item-label">Toggle Heatmap</span><span class="dropmenu-item-content">h</span></a></li>');
 
         htmls.push('<li><hr class="half-rule"></li>');
 
         //htmls.push('<li><a href="#" id="tpOnlySelectedButton">Show only selected</a></li>');
         //htmls.push('<li><a href="#" id="tpFilterButton">Hide selected '+gSampleDesc+'s</a></li>');
         //htmls.push('<li><a href="#" id="tpShowAllButton">Show all '+gSampleDesc+'</a></li>');
-        htmls.push('<li><a href="#" id="tpHideShowLabels"><span id="tpHideMenuEntry">Hide labels</span><span class="dropmenu-item-content">c l</span></a></li>');
+        htmls.push('<li><a href="#" id="tpHideShowLabels">Hide labels<span class="dropmenu-item-content">c l</span></a></li>');
         //htmls.push('<li><hr class="half-rule"></li>');
 
         //htmls.push('<li class="dropdown-submenu"><a tabindex="0" href="#">Transparency</a>');
         //htmls.push('<ul class="dropdown-menu" id="tpTransMenu">');
         //htmls.push('<li id="tpTrans0"><a href="#">0%</a></li>');
         //htmls.push('<li id="tpTrans40"><a href="#">40%</a></li>');
         //htmls.push('<li id="tpTrans60"><a href="#">60%</a></li>');
@@ -2789,31 +1006,17 @@
         //htmls.push('</ul>'); // Circle size sub-menu
         //htmls.push('</li>');   // sub-menu container
 
         htmls.push('</ul>'); // View dropdown-menu
         htmls.push('</li>'); // View dropdown container
 
         htmls.push('<li class="dropdown">');
-        htmls.push('<a href="#" class="dropdown-toggle" data-toggle="dropdown" data-submenu role="button" aria-haspopup="true" aria-expanded="false">Tools</a>');
-        htmls.push('<ul class="dropdown-menu">');
-        //htmls.push('<li><a href="#" id="tpRenameClusters">Rename clusters...<span class="dropmenu-item-content"></span></a></li>');
-        htmls.push('<li><a href="#" id="tpCustomAnnots">Remove all custom annotations<span class="dropmenu-item-content"></span></a></li>');
-        //htmls.push('<li><a href="#" id="tpCluster">Run clustering...<span class="dropmenu-item-content"></span></a></li>');
-        htmls.push('<li class="disabled"><a href="#" id="tpSetBackground">Set as background cells<span class="dropmenu-item-content">b s</span></a></li>');
-        htmls.push('<li class="disabled"><a href="#" id="tpResetBackground">Reset background cells<span class="dropmenu-item-content">b r</span></a></li>');
-        htmls.push('</ul>'); // Tools dropdown-menu
-        htmls.push('</li>'); // Tools dropdown container
-
-
-        htmls.push('<li class="dropdown">');
         htmls.push('<a href="#" class="dropdown-toggle" data-toggle="dropdown" data-submenu role="button" aria-haspopup="true" aria-expanded="false">Help</a>');
         htmls.push('<ul class="dropdown-menu">');
-        htmls.push('<li><a href="#" id="tpAboutButton">About</a></li>');
-        htmls.push('<li><a href="https://cellbrowser.readthedocs.io/en/master/interface.html" target=_blank id="tpQuickstartButton">How to use this website</a></li>');
-        htmls.push('<li><a href="#" id="tpTutorialButton">Interactive Tutorial</a></li>');
+        htmls.push('<li><a href="#" id="tpTutorialButton">Tutorial</a></li>');
         htmls.push('<li><a target=_blank href="https://github.com/maximilianh/cellBrowser#readme" id="tpGithubButton">Setup your own cell browser</a></li>');
         htmls.push('</ul>'); // Help dropdown-menu
         htmls.push('</li>'); // Help dropdown container
 
         htmls.push('</ul>'); // navbar-nav
 
         htmls.push('</div>'); // container
@@ -2823,264 +1026,169 @@
         $(document.body).append(htmls.join(""));
 
         $('#tpTransMenu li a').click(onTransClick);
         $('#tpSizeMenu li a').click(onSizeClick);
         //$('#tpFilterButton').click( onHideSelectedClick );
         //$('#tpOnlySelectedButton').click( onShowOnlySelectedClick );
         $('#tpZoom100Menu').click(onZoom100Click);
-        $('#tpSplitMenu').click(onSplitClick);
-        $('#tpHeatMenu').click(onHeatClick);
         $('#tpZoomPlus').click(onZoomInClick);
         $('#tpZoomMinus').click(onZoomOutClick);
         //$('#tpShowAllButton').click( onShowAllClick );
         $('#tpHideShowLabels').click(onHideShowLabelsClick);
         $('#tpExportIds').click(onExportIdsClick);
         $('#tpSelectById').click(onSelectByIdClick);
         $('#tpMark').click(onMarkClick);
         $('#tpMarkClear').click(onMarkClearClick);
         $('#tpTutorialButton').click(function() {
             showIntro(false);
         });
-        $('#tpAboutButton').click(onAboutClick);
-        $('#tpOpenDatasetLink').click(openCurrentDataset);
+        $('#tpOpenDatasetLink').click(openDatasetDialog);
         $('#tpSaveImage').click(onSaveAsClick);
-        $('#tpSaveImageSvg').click(onSaveAsSvgClick);
         $('#tpSelectAll').click(onSelectAllClick);
         $('#tpSelectNone').click(onSelectNoneClick);
-        $('#tpSelectInvert').click(onSelectInvertClick);
-        $('#tpSelectName').click(onSelectNameClick);
-        $('#tpSelectComplex').click(onFindCellsClick);
-
-
-        $('#tpRenameClusters').click(onRenameClustersClick);
-        $('#tpCustomAnnots').click(onCustomAnnotationsClick);
-        $('#tpSetBackground').click(onBackgroudSetClick);
-        $('#tpResetBackground').click(onBackgroudResetClick);
-        //$('#tpCluster').click( onRunClusteringClick );
+        $('#tpSelectComplex').click(onSelectComplexClick);
+        $('#tpDownloadMenu li a').click(onDownloadClick);
 
         // This version is more like OSX/Windows:
         // - menus only open when you click on them
         // - once you have clicked, they start to open on hover
         // - a click anywhere else will stop the hovering
         var doHover = false;
         $(".nav > .dropdown").click(function() {
-            doHover = !doHover;
-            return true;
+            doHover = true;
         });
         $(".nav > .dropdown").hover(
             function(event) {
                 if (doHover) {
                     $(".dropdown-submenu").removeClass("open");
                     $(".dropdown").removeClass("open");
                     $(this).addClass('open');
                 }
             });
-
         $(document).click(function() {
             doHover = false;
         });
 
-        // when user releases the mouse outside the canvas, remove the zooming marquee
-        $(document).mouseup(function(ev) {
-            if (ev.target.nodeName !== "canvas") {
-                renderer.resetMarquee();
-            }
-        });
-
         $('[data-submenu]').submenupicker();
 
     }
 
-    function resizeDivs(skipRenderer) {
+    function resizeDivs() {
         /* resize all divs and the renderer to current window size */
         var rendererLeft = metaBarWidth + metaBarMargin;
         var rendererHeight = window.innerHeight - menuBarHeight - toolBarHeight;
 
         var rendererWidth = window.innerWidth - legendBarWidth - rendererLeft;
         var legendBarLeft = rendererWidth + metaBarMargin + metaBarWidth;
 
-        var heatWidth, heatHeight;
-        if (db && db.heatmap) {
-            heatWidth = rendererWidth;
-            heatHeight = db.heatmap.height;
-            rendererHeight = rendererHeight - heatHeight;
-            db.heatmap.setSize(heatWidth, heatHeight);
-            let heatTop = window.innerHeight - heatHeight;
-            db.heatmap.div.style.top = heatTop + "px";
-            db.heatmap.draw();
-        }
-
-        $("#tpToolBar").css("width", rendererWidth + "px");
-
-        $("#tpToolBar").css("height", toolBarHeight + "px");
-        $("#tpLeftSidebar").css("height", (window.innerHeight - menuBarHeight) + "px");
-
-        // when this is run the first time, these elements don't exist yet.
-        // Note that the whole concept of forcing these DIVs to go up to the screen size is strange, but
-        // I have not found a way in CSS to make them go to the end of the screen. They need to have a fixed size,
-        // as otherwise the scroll bars of tpLegendBar and tpMetaPanel won't appear
-        if ($('#tpMetaPanel').length !== 0)
-            $("#tpMetaPanel").css("height", (window.innerHeight - $('#tpMetaPanel').offset().top) + "px");
-        if ($('#tpLegendRows').length !== 0)
-            $("#tpLegendBar").css("height", (window.innerHeight - $('#tpLegendBar').offset().top) + "px");
+        $("#tpToolBar").css("width", rendererWidth);
+        $("#tpToolBar").css("height", toolBarHeight);
+        $("#tpLeftSidebar").css("height", window.innerHeight - menuBarHeight);
+        $("#tpLegendBar").css("height", window.innerHeight - menuBarHeight);
         $('#tpLegendBar').css('left', legendBarLeft + "px");
 
-        if (skipRenderer !== true)
-            renderer.setSize(rendererWidth, rendererHeight, true);
-
+        renderer.setSize(rendererWidth, rendererHeight);
     }
 
-    var progressUrls = {};
+    var progressUrls = [];
 
     function onProgressConsole(ev) {
-        //console.log(ev);
+        console.log(ev);
     }
 
     function onProgress(ev) {
-        /* update progress bars. The DOM elements of these were added in maxPlot (not optimal?)  */
-        console.log(ev);
-        if (ev.text !== undefined) {
-            // image loaders just show a little watermark
-            renderer.setWatermark(ev.text);
-            return;
-        }
-
-        var url = null;
-        var domEl = ev.currentTarget;
-        if (domEl)
-            url = domEl.responseURL;
-        else
-            url = ev.src; // when loading an image, we're getting the <img> domEl, not sure why no event
-
-        url = url.split("?")[0]; // strip off the md5 checksum
-
-        if (url.search("exprMatrix.bin") !== -1) // never show progress bar for single gene vector requests
+        /* show progress bars */
+        var url = ev.currentTarget.responseURL;
+        if (url.search("exprMatrix.bin") !== -1)
             return;
 
-        var progressRowIdx = progressUrls[url]; // there can be multiple progress bars
-        if (progressRowIdx === undefined) {
-            // if there is none yet, find the first free index
-            progressRowIdx = 0;
-            for (var oldUrl in progressUrls) {
-                progressRowIdx = Math.max(progressRowIdx, progressUrls[oldUrl]);
-
-            }
-            progressRowIdx++;
-            progressUrls[url] = progressRowIdx;
+        var index = progressUrls.indexOf(url);
+        if (index === -1) {
+            progressUrls.push(url);
+            index = progressUrls.length - 1;
         }
 
         var label = url;
         if (url.endsWith("coords.bin"))
             label = "Loading Coordinates";
         else if (url.endsWith(".bin"))
             label = "Loading cell annotations";
-
-        var labelId = "#mpProgressLabel" + progressRowIdx;
+        var labelId = "#tpProgressLabel" + index;
         $(labelId).html(label);
 
         var percent = Math.round(100 * (ev.loaded / ev.total));
 
-        if (percent >= 99) {
-            $("#mpProgress" + progressRowIdx).css("width", percent + "%");
-            $("#mpProgress" + progressRowIdx).show(0);
-            //progressUrls.splice(index, 1);
-            delete progressUrls[url];
-            $("#mpProgressDiv" + progressRowIdx).css("display", "none");
+        if (percent === 100) {
+            $("#tpProgress" + index).css("width", percent + "%");
+            $("#tpProgress" + index).show(0);
+            progressUrls.splice(index, 1);
+            $("#tpProgressDiv" + index).css("display", "none");
         } else {
-            $("#mpProgress" + progressRowIdx).css("width", percent + "%");
-            $("#mpProgressDiv" + progressRowIdx).css("display", "inherit");
+            $("#tpProgress" + index).css("width", percent + "%");
+            $("#tpProgressDiv" + index).css("display", "inherit");
         }
     }
 
-
     function colorByMetaField(fieldName, doneLoad) {
-        /* load the meta data for a field, setup the colors, send it all to the renderer and call doneLoad. if doneLoad is undefined, redraw everything  */
-
-        function onMetaArrLoaded(metaArr, metaInfo) {
-            gLegend = buildLegendForMeta(metaInfo);
-            buildLegendBar();
-            var renderColors = legendGetColors(gLegend.rows);
-            renderer.setColors(renderColors);
-            renderer.setColorArr(metaArr);
-            metaInfo.arr = metaArr;
-            doneLoad();
-        }
-
+        /* load the meta data for a field, setup the colors, send it all to the renderer and call doneLoad */
         if (doneLoad === undefined)
             doneLoad = function() {
                 renderer.drawDots();
             };
 
-        if (fieldName === null || fieldName === undefined) {
+        if (fieldName === null) {
             // obscure hacky option: you can set the default color field to "None"
             // so there is no coloring at all on startup
             renderer.setColors(["black"]);
             var cellCount = db.conf.sampleCount;
             renderer.setColorArr(new Uint8Array(cellCount));
             gLegend.rows = [];
-            gLegend.title = "Nothing selected";
-            gLegend.rows.push({
-                color: "000000",
-                defColor: null,
-                label: "No Value",
-                count: cellCount,
-                intKey: 0,
-                strKey: null
-            });
+            gLegend.rows.push(["000000", null, "No Value", cellCount, 0, null]);
             doneLoad();
             return;
         }
 
-        var metaInfo = db.findMetaInfo(fieldName);
+        var fieldIdx = db.fieldNameToIndex(fieldName);
         console.log("Color by meta field " + fieldName);
 
-        // cbData always keeps the most recent expression array. Reset it now.
-        if (db.lastExprArr)
-            delete db.lastExprArr;
-
-        var defaultMetaField = db.getDefaultColorField()[1];
-
         // internal field names cannot contain non-alpha chars, so tolerate user errors here
         // otherwise throw an error
-        if (metaInfo === null && fieldName !== undefined) {
-            metaInfo = db.findMetaInfo(fieldName.replace(/[^0-9a-z]/gi, ''));
-            if (metaInfo === null) {
+        if (fieldIdx === null) {
+            fieldIdx = db.fieldNameToIndex(fieldName.replace(/[^0-9a-z]/gi, ''));
+            if (fieldIdx === null) {
                 alert("The field " + fieldName + " does not exist in the sample/cell annotations. Cannot color on it.");
-                metaInfo = db.findMetaInfo(defaultMetaField);
+                return;
             }
         }
 
-        if (metaInfo.type === "uniqueString") {
-            warn("This field contains a unique identifier. You cannot color on such a field. However, you can search for values in this field using 'Edit > Find by ID'.");
-            return null;
-        }
+        var fieldInfo = db.getMetaFields()[fieldIdx];
 
-        if (metaInfo.diffValCount > MAXCOLORCOUNT && metaInfo.type === "enum") {
-            warn("This field has " + metaInfo.diffValCount + " different values. Coloring on a field that has more than " + MAXCOLORCOUNT + " different values is not supported.");
+        if (fieldInfo.diffValCount > MAXCOLORCOUNT && fieldInfo.binMethod === undefined) {
+            warn("This field has " + fieldInfo.diffValCount + " different values. Coloring on a field that has more than " + MAXCOLORCOUNT + " different values is not supported.");
             return null;
         }
 
-
-        if (fieldName === defaultMetaField)
-            changeUrl({
-                "meta": null,
-                "gene": null
-            });
-        else
+        var defaultMetaField = db.getDefaultColorField()[1];
+        if (fieldName !== defaultMetaField)
             changeUrl({
                 "meta": fieldName,
                 "gene": null
             });
 
-        if (metaInfo.arr) // eg custom fields
-            onMetaArrLoaded(metaInfo.arr, metaInfo);
-        else
-            db.loadMetaVec(metaInfo, onMetaArrLoaded, onProgress);
 
+        buildLegendForMetaIdx(fieldIdx);
+        var renderColors = legendGetColors(gLegend.rows);
+        renderer.setColors(renderColors);
+
+        db.loadMetaVec(fieldIdx, function(carr) {
+            renderer.setColorArr(carr);
+            doneLoad();
+        }, onProgress);
 
+        //changeUrl({"gene":null, "meta":fieldName});
         changeUrl({
             "pal": null
         });
         // clear the gene search box
         var select = $('#tpGeneCombo')[0].selectize.clear();
     }
 
@@ -3112,29 +1220,29 @@
             warn("internal error - splitExprByMeta: exprVec has diff length from splitArr");
         }
 
         var arr1 = [];
         var arr2 = [];
 
         // code duplication, not very elegant, but avoids creating an array just for the indices
-        if (selCells.length === 0)
+        if (selCells === null)
             // the version if no cells are selected
             for (var cellIdx = 0; cellIdx < exprVec.length; cellIdx++) {
                 var val = exprVec[cellIdx];
-                if (splitArr[cellIdx] === 0)
+                if (splitArr[cellIdx] == 0)
                     arr1.push(val);
                 else
                     arr2.push(val);
             }
         else
             // the version with a cell selection
             for (var i = 0; i < selCells.length; i++) {
-                let cellIdx = selCells[i];
-                let val = exprVec[cellIdx];
-                if (splitArr[cellIdx] === 0)
+                var cellIdx = selCells[i];
+                var val = exprVec[cellIdx];
+                if (splitArr[cellIdx] == 0)
                     arr1.push(val);
                 else
                     arr2.push(val);
             }
 
         if (db.conf.violinDoLog2) {
             console.time("log2");
@@ -3166,89 +1274,99 @@
 
         console.timeEnd("splitExpr");
         return [sel, unsel];
     }
 
     function buildViolinFromValues(labelList, dataList) {
         /* make a violin plot given the labels and the values for them */
+        console.time("violinDraw");
+        //removeViolinPlot();
         if ("violinChart" in window)
             window.violinChart.destroy();
 
+        //var htmls = [];
+        //$('#tpLegendContent').append(htmls.join(""));
+
         var labelLines = [];
-        labelLines[0] = labelList[0].split("\n");
-        labelLines[0].push(dataList[0].length);
-        if (dataList.length > 1) {
-            labelLines[1] = labelList[1].split("\n");
-            labelLines[1].push(dataList[1].length);
-        }
+        //labelLines.push([labelList[0], dataList[0].length+" cells"]);
+        labelLines.push([labelList[0], dataList[0].length]);
+        if (dataList.length > 1)
+            //labelLines.push([labelList[1], dataList[1].length+" cells"]);
+            labelLines.push([labelList[1], dataList[1].length]);
 
-        const ctx = getById("tpViolinCanvas").getContext("2d");
+        const ctx = document.getElementById("tpViolinCanvas").getContext("2d");
 
-        var violinData = {
+        var boxplotData = {
             labels: labelLines,
             datasets: [{
                 data: dataList,
-                label: 'Mean',
+                label: 'Dataset 1',
                 backgroundColor: 'rgba(255,0,0,0.5)',
                 borderColor: 'red',
                 borderWidth: 1,
                 outlierColor: '#999999',
                 padding: 7,
                 itemRadius: 0
             }]
         };
 
+        //scales: {
+        //xAxes: [{
+        //ticks: {
+        //autoSkip: false,
+        //maxRotation: 40,
+        //minRotation: 40
+        //}
+        //}],
+        //},
+        //responsive: true,
         var optDict = {
             maintainAspectRatio: false,
             legend: {
                 display: false
             },
             title: {
                 display: false
             }
         };
 
         var yLabel = null;
         if (db.conf.unit === undefined && db.conf.matrixArrType === "Uint32")
-            yLabel = "read/UMI count";
+            yLabel = "read/UMI count"
         if (db.conf.unit !== undefined)
             yLabel = db.conf.unit;
 
         if (yLabel !== null)
             optDict.scales = {
                 yAxes: [{
                     scaleLabel: {
                         display: true,
                         labelString: yLabel
                     }
                 }]
             };
 
-        window.setTimeout(function() {
-            console.time("violinDraw");
-            window.violinChart = new Chart(ctx, {
-                type: 'violin',
-                data: violinData,
-                options: optDict
-            });
-            console.timeEnd("violinDraw");
-        }, 10);
+        window.violinChart = new Chart(ctx, {
+            type: 'violin',
+            data: boxplotData,
+            options: optDict
+        });
+        console.timeEnd("violinDraw");
     }
 
 
     function buildViolinFromMeta(exprVec, metaName, selCells) {
         /* load a binary meta vector, split the exprVector by it and make two violin plots, one meta value vs the other.  */
-        var metaInfo = db.findMetaInfo(metaName);
+        var metaInfo = findMetaInfo(metaName);
         if (metaInfo.valCounts.length !== 2) {
             alert("Config error: meta field in 'violinField', '" + db.conf.violinField + "' does not have two distinct values.");
             return;
         }
-
         var labelList = [metaInfo.valCounts[0][0], metaInfo.valCounts[1][0]];
-        db.loadMetaVec(metaInfo,
+        db.loadMetaVec(metaInfo.index,
             function(metaArr) {
                 var dataList = splitExprByMeta(exprVec, metaArr, selCells);
                 buildViolinFromValues(labelList, dataList);
             },
             null);
     }
 
@@ -3264,382 +1382,140 @@
         var exprVec = gLegend.exprVec;
         if (exprVec === undefined)
             return;
 
         var dataList = [];
         var labelList = [];
         var selCells = renderer.getSelection();
-
-        // filter exprVec by background
-        if (background !== null) {
-            var ourSelCells = {};
-            for (var i = 0; i < selCells.length; i++) {
-                ourSelCells[selCells[i]] = true;
-            }
-            var ourCells = {};
-            for (i = 0; i < background.length; i++) {
-                ourCells[background[i]] = true;
-            }
-
-            var result = [];
-            var renamedSelCells = [];
-            for (i = 0; i < exprVec.length; i++) {
-                if (i in ourSelCells) {
-                    renamedSelCells.push(result.length);
-                    result.push(exprVec[i]);
-                } else if (i in ourCells) {
-                    result.push(exprVec[i]);
-                }
-            }
-            exprVec = result;
-            selCells = renamedSelCells;
-        }
         // if we have a violin meta field to split on, make two violin plots, one meta vs, the other meta
         // restrict the plot to the selected cells, if any
-        if (db.conf.violinField !== undefined) {
+        if (db.conf.violinField != undefined) {
             buildViolinFromMeta(exprVec, db.conf.violinField, selCells);
         } else {
             // there is no violin field
-            if (selCells.length === 0) {
+            if (selCells === null || selCells.length === 0) {
                 // no selection, no violinField: default to a single violin plot
                 dataList = [Array.prototype.slice.call(exprVec)];
-                if (background === null) {
-                    labelList = ['All cells'];
-                } else {
-                    labelList = ['Background\ncells'];
-                }
+                labelList = ['All cells'];
                 buildViolinFromValues(labelList, dataList);
             } else {
                 // cells are selected and no violin field: make two violin plots, selected against other cells
                 dataList = splitExpr(exprVec, selCells);
-                if (background === null) {
-                    labelList = ['Selected', 'Others'];
-                } else {
-                    labelList = ['Selected', 'Background'];
-                }
+                labelList = ['Selected', 'Others'];
                 if (dataList[1].length === 0) {
                     dataList = [dataList[0]];
                     labelList = ['All Selected'];
                 }
                 buildViolinFromValues(labelList, dataList);
             }
         }
     }
 
-    function selectizeSetValue(selector, name) {
-        /* little convenience method to set a selective dropdown to a given
-         * value. does not trigger the change event. */
-        if (name === undefined)
-            return;
-        var sel = $(selector)[0].selectize;
-        sel.addOption({
-            id: name,
-            text: name
-        });
-        sel.setValue(name, 1); // 1 = do not fire change
-    }
-
-    function colorByLocus(locusStr, onDone, locusLabel) {
-        /* color by a gene or peak, load the array into the renderer and call onDone or just redraw 
-         * peak can be in format: +chr1:1-1000
-         * gene can be in format: geneSym or geneSym=geneId
-         * */
-        if (onDone === undefined || onDone === null)
+    function loadGeneAndColor(geneSym, onDone) {
+        /* color by a gene, load the array into the renderer and call onDone or just redraw */
+        if (onDone === undefined)
             onDone = function() {
                 renderer.drawDots();
             };
 
-        function gotGeneVec(exprArr, decArr, locusStr, geneDesc, binInfo) {
-            /* called when the expression vector has been loaded and binning is done */
+        function gotGeneVec(exprArr, decArr, geneSym, geneDesc, binInfo) {
+            /* called when the expression vector has been loaded */
             if (decArr === null)
                 return;
-            console.log("Received expression vector, for " + locusStr + ", desc: " + geneDesc);
-            // update the URL and possibly the gene combo box
-            var fullLocusStr = locusStr;
-            if (locusStr.indexOf("|") > -1) {
-                fullLocusStr = peakListSerialize(); // the locus str can be +chr1:1-1000 to add a single gene, but we want all
-                changeUrl({
-                    "locus": locusStr,
-                    "meta": null
-                });
-            } else {
-                changeUrl({
-                    "gene": locusStr,
-                    "meta": null
-                });
-            }
-
-
-            makeLegendExpr(fullLocusStr, geneDesc, binInfo, exprArr, decArr);
+            console.log("Received expression vector, gene " + geneSym + ", geneId " + geneDesc);
+            _dump(binInfo);
+            makeLegendExpr(geneSym, geneDesc, binInfo, exprArr, decArr);
+            //if (db.quickExpr===undefined)
+            //db.quickExpr = {};
+            //db.quickExpr[geneSym] = [exprArr, geneDesc, binInfo];
             renderer.setColors(legendGetColors(gLegend.rows));
             renderer.setColorArr(decArr);
             buildLegendBar();
             onDone();
 
-            // update the "recent genes" div
-            for (var i = 0; i < gRecentGenes.length; i++) {
-                // remove previous gene entry with the same symbol
-                if (gRecentGenes[i][0] === locusStr || gRecentGenes[i][1] === locusStr) { // match symbol or ID
-                    gRecentGenes.splice(i, 1);
-                    break;
-                }
-            }
-
-            // make sure that recent genes table has symbol and Id
-            var locusWithSym = locusStr;
-            var geneInfo = db.getGeneInfo(locusStr);
-            if (!db.isAtacMode() && (geneInfo.sym !== geneInfo.geneId))
-                locusWithSym = geneInfo.id + "|" + geneInfo.sym;
-
-            gRecentGenes.unshift([locusWithSym, geneDesc]); // insert at position 0
-            gRecentGenes = gRecentGenes.slice(0, 9); // keep only nine last
-            buildGeneTable(null, "tpRecentGenes", null, null, gRecentGenes);
-            $('#tpRecentGenes .tpGeneBarCell').click(onGeneClick);
-            resizeGeneTableDivs("tpRecentGenes");
+            // update the gene combo box
+            var sel = $('#tpGeneCombo')[0].selectize;
+            sel.addOption({
+                text: geneSym,
+                value: geneSym
+            });
+            sel.refreshOptions();
+            sel.setTextboxValue(geneSym);
         }
 
+        changeUrl({
+            "gene": geneSym,
+            "meta": null,
+            "pal": null
+        });
+        console.log("Loading gene expression vector for " + geneSym);
+        db.loadExprAndDiscretize(geneSym, gotGeneVec, onProgress, exprBinCount);
+
         // clear the meta combo
         $('#tpMetaCombo').val(0).trigger('chosen:updated');
-
-        console.log("Loading gene expression vector for " + locusStr);
-
-        db.loadExprAndDiscretize(locusStr, gotGeneVec, onProgress, db.conf.binStrategy);
-
     }
 
-    function gotCoords(coords, info, clusterInfo, newRadius) {
+    function gotCoords(coords, info, clusterMids) {
         /* called when the coordinates have been loaded */
         if (coords.length === 0)
             alert("cellBrowser.js/gotCoords: coords.bin seems to be empty");
-        var opts = {};
-        if (newRadius)
-            opts["radius"] = newRadius;
-
-        // label text can be overriden by the user cart
-        var labelField = db.conf.labelField;
-
-        if (!db.gLabelCoordCache)
-            db.gLabelCoordCache = {};
-
-        if (clusterInfo) {
-            var origLabels = [];
-            var clusterMids = clusterInfo.labels;
-            // old-style files contain just coordinates, no order
-            if (clusterMids === undefined) {
-                clusterMids = clusterInfo;
-            }
-
-            db.gLabelCoordCache[labelField] = clusterMids;
-            for (var i = 0; i < clusterMids.length; i++) {
-                origLabels.push(clusterMids[i][2]);
-            }
-            renderer.origLabels = origLabels;
-            clusterMids = [];
-        }
-
-        if (clusterInfo && clusterInfo.lines) {
-            opts["lines"] = clusterInfo.lines;
-            opts["lineWidth"] = db.conf.lineWidth;
-            opts["lineColor"] = db.conf.lineColor;
-            opts["lineAlpha"] = db.conf.lineAlpha;
-        }
-
-        renderer.setCoords(coords, clusterMids, info, opts);
-    }
-
-    function computeAndSetLabels(values, metaInfo) {
-        /* recompute the label positions and redraw everything. Uses a cache for the label positions */
-        var labelCoords;
-        if (db.gLabelCoordCache[metaInfo.label] !== undefined) {
-            labelCoords = db.gLabelCoordCache[metaInfo.label];
-        } else {
-            var coords = renderer.coords.orig;
-            var names = null;
-            if (metaInfo.type !== "float" && metaInfo.type !== "int") {
-                var names = metaInfo.ui.shortLabels;
-            }
-
-            // console.log(metaInfo);
-
-            console.time("cluster centers");
-            var calc = renderer.calcMedian(coords, values, names, metaInfo.origVals);
-
-            labelCoords = [];
-            for (var label in calc) {
-                var labelInfo = calc[label];
-                var midX = selectMedian(labelInfo[0]);
-                var midY = selectMedian(labelInfo[1]);
-                labelCoords.push([midX, midY, label]);
-            }
-            console.timeEnd("cluster centers");
-            db.gLabelCoordCache[metaInfo.label] = labelCoords;
-        }
-        renderer.setLabelCoords(labelCoords);
-        setLabelDropdown(metaInfo.name);
-    }
-
-    function setLabelField(labelField) {
-        /* change the field that is used for drawing the labels. Do not redraw. */
-        var metaInfo = db.findMetaInfo(labelField);
-        db.conf.activeLabelField = metaInfo.name;
-
-        if (metaInfo.arr) // preloaded
-            computeAndSetLabels(metaInfo.arr, metaInfo);
-        else
-            db.loadMetaVec(metaInfo, computeAndSetLabels);
-    }
-
-    function setColorByDropdown(fieldName) {
-        /* set the meta 'color by' dropdown to a given value. The value is the meta field name, not its label, nor its index */
-        var fieldIdx = db.fieldNameToIndex(fieldName);
-        $('#tpMetaCombo').val("tpMetaVal_" + fieldIdx).trigger('chosen:updated');
-    }
-
-    function setLabelDropdown(fieldName) {
-        /* set the meta 'label by' dropdown to a given value. The value is the meta field name, nor its short label, nor its index */
-        var fieldIdx = db.fieldNameToIndex(fieldName);
-        $('#tpLabelCombo').val("tpMetaVal_" + fieldIdx).trigger('chosen:updated');
-    }
-
-    function colorByDefaultField(onDone) {
-        /* get the default coloring field from the config or the URL and start coloring by it.
-         * Call onDone() when done. */
-        var colorByInfo = db.getDefaultColorField();
-        var colorType = colorByInfo[0];
-        var colorBy = colorByInfo[1];
-
-        // allow to override coloring by URL args
-        if (getVar("gene") !== undefined) {
-            colorType = "gene";
-            colorBy = getVar("gene");
-            activateTab("gene");
-        } else if (getVar("meta") !== undefined) {
-            colorType = "meta";
-            colorBy = getVar("meta");
-            activateTab("meta");
-        } else if (getVar("locus") !== undefined) {
-            colorType = "locus";
-            colorBy = getVar("locus");
-            activateTab("gene");
-        }
-
-        gLegend = {};
-        if (colorType === "meta") {
-            colorByMetaField(colorBy, onDone);
-            // update the meta field combo box
-            var fieldIdx = db.fieldNameToIndex(colorBy);
-            if (fieldIdx === null) {
-                alert("Default coloring is configured to be on field " + colorBy +
-                    " but cannot find a field with this name, using field 1 instead.");
-                fieldIdx = 1;
-            }
-
-            setColorByDropdown(colorBy);
-            $('#tpMetaBox_' + fieldIdx).addClass('tpMetaSelect');
-        } else if (colorType === "locus") {
-            colorByLocus(colorBy, onDone);
-            peakListSetStatus(colorBy);
-        } else
-            // must be gene then
-            colorByLocus(colorBy, onDone);
-    }
-
-    function makeFullLabel(db) {
-        /* return full name of current dataset, including parent names */
-        var nameParts = [];
-        var parents = db.conf.parents;
-        if (parents)
-            for (var i = 0; i < parents.length; i++)
-                if (parents[i][0] != "") // "" is the root dataset = no need to add
-                    nameParts.push(parents[i][1]);
-
-        nameParts.push(db.conf.shortLabel);
-        var datasetLabel = nameParts.join(" - ");
-        return datasetLabel;
-    }
-
-    function gotSpatial(img) {
-        /* called when the spatial image has been loaded */
-        renderer.setBackground(img);
-        if (renderer.readyToDraw())
-            renderer.drawDots();
-        else
-            console.log("got spatial, but cannot draw yet");
+        renderer.setCoords(coords, clusterMids, info.minX, info.maxX, info.minY, info.maxY);
     }
 
     function renderData() {
-        /* init the basic UI parts, the main renderer in the center, start loading and draw data when ready
+        /* init the renderer, start loading and draw data when ready
          */
         var forcePalName = getVar("pal", null);
 
         var loadsDone = 0;
 
-        var selList = null; // search expression to select, in format accepted by findCellsMatchingQueryList()
-
         function doneOnePart() {
             /* make sure renderer only draws when both coords and other data have loaded */
             loadsDone += 1;
             if (loadsDone === 2) {
                 buildLegendBar();
 
-                if (db.conf.labelField)
-                    setLabelField(db.conf.labelField);
-
                 if (forcePalName !== null) {
                     legendChangePaletteAndRebuild(forcePalName);
                 } else
                     renderer.setColors(legendGetColors(gLegend.rows));
 
-
-                renderer.setTitle("Dataset: " + makeFullLabel(db));
-
-                if (selList)
-                    findCellsMatchingQueryList(selList, function(cellIds) {
-                        renderer.selectSet(cellIds);
-                        renderer.drawDots();
-                    });
-                else
-                    renderer.drawDots();
-
-                //if (db.conf.multiModal && db.conf.multiModal.splitPrefix)
-                //renderer.split();
+                renderer.setTitle("Dataset: " + db.conf.shortLabel);
+                renderer.drawDots();
             }
         }
 
         function guessRadiusAlpha(dotCount) {
             /* return reasonable radius and alpha values for a number of dots */
             if (dotCount < 3000)
-                return [4, 0.7];
-            if (dotCount < 6000)
-                return [4, 0.6];
-            if (dotCount < 10000)
-                return [3, 0.5];
-            if (dotCount < 35000)
-                return [2, 0.3];
-            if (dotCount < 60000)
-                return [1, 0.5];
-            // everything else
-            return [0, 0.3];
+                return [4.0, 0.5];
+            if (dotCount < 5000)
+                return [3.0, 0.5];
+            if (dotCount < 9000)
+                return [2.0, 0.5];
+            if (dotCount < 15000)
+                return [3.0, 0.4];
+            if (dotCount < 50000)
+                return [0.0, 0.3];
         }
 
         function makeRendConf(dbConf, dotCount) {
             /* return the 'args' object for the renderer, based on dbConf and count of dots */
             var rendConf = {};
 
             var radius = dbConf.radius;
             var alpha = dbConf.alpha;
 
-            if (radius === undefined || alpha === undefined) {
+            if (radius === undefined || alpha === undefined)
                 var radiusAlpha = guessRadiusAlpha(dotCount);
 
-                if (radius === undefined)
-                    radius = radiusAlpha[0];
-                if (alpha === undefined)
-                    alpha = radiusAlpha[1];
-            }
+            if (radius === undefined)
+                radius = radiusAlpha[0];
+            if (alpha === undefined)
+                alpha = radiusAlpha[1];
 
             rendConf["radius"] = radius;
             rendConf["alpha"] = alpha;
 
             rendConf["mode"] = "move"; // default mode, one of "move", "select" or "zoom"
 
             return rendConf;
@@ -3650,44 +1526,50 @@
             gotCoords(coords, info, clusterMids);
             doneOnePart();
         }
 
         var rendConf = makeRendConf(db.conf, db.conf.sampleCount);
         renderer.initPlot(rendConf);
 
-        if (db.conf.showLabels === false)
-            renderer.setShowLabels(false);
-
         buildLeftSidebar();
-        buildToolBar(db.conf.coords, db.conf, metaBarWidth + metaBarMargin, menuBarHeight);
+        buildToolBar(db.conf.coords, db.conf.name, metaBarWidth + metaBarMargin, toolBarHeight);
+        //activateMode("move");
 
-        db.loadCoords(0, gotFirstCoords, gotSpatial, onProgress);
+        db.loadCoords(0, gotFirstCoords, onProgress);
 
-        if (getVar("select") !== undefined) {
-            selList = JSURL.parse(getVar("select"));
-        }
+        var colorByInfo = db.getDefaultColorField();
+        var colorType = colorByInfo[0];
+        var colorBy = colorByInfo[1];
 
-        colorByDefaultField(doneOnePart);
+        // allow to override coloring by URL args
+        if (getVar("gene", null) !== null) {
+            colorType = "gene";
+            colorBy = getVar("gene");
+            activateTab("gene");
+        } else if (getVar("meta", null) !== null) {
+            colorType = "meta";
+            colorBy = getVar("meta");
+            activateTab("meta");
+        }
 
-        if (db.conf.atacSearch)
-            db.loadGeneLocs(db.conf.atacSearch, db.conf.fileVersions.geneLocs);
-        // pre-load the dataset description file, as the users will often go directly to the info dialog
-        // and the following pre-loads risk blocking this load.
-        var jsonUrl = cbUtil.joinPaths([db.conf.name, "desc.json"]) + "?" + db.conf.md5;
-        fetch(jsonUrl);
+        gLegend = {};
+        if (colorType === "meta") {
+            colorByMetaField(colorBy, doneOnePart);
+            // update the meta field combo box
+            var fieldIdx = db.fieldNameToIndex(colorBy);
+            $('#tpMetaCombo').val(fieldIdx).trigger('chosen:updated');
+        } else {
+            loadGeneAndColor(colorBy, doneOnePart);
+        }
 
-        //if (db.conf.sampleCount < 50000) {
         if (db.conf.quickGenes)
             db.preloadGenes(db.conf.quickGenes, function() {
                 updateGeneTableColors(null);
-                if (getVar("heat") === "1")
-                    onHeatClick();
-            }, onProgressConsole, db.conf.binStrategy);
+            }, onProgressConsole, exprBinCount);
         db.preloadAllMeta();
-        //}
     }
 
     function onTransClick(ev) {
         /* user has clicked transparency menu entry */
         var transText = ev.target.innerText;
         var transStr = transText.slice(0, -1); // remove last char
         var transFloat = 1.0 - (parseFloat(transStr) / 100.0);
@@ -3701,20 +1583,20 @@
     function legendSort(sortBy) {
         /* sort the legend by "name" or "count" */
         var rows = gLegend.rows;
 
         if (sortBy === "name") {
             // index 2 is the label
             rows.sort(function(a, b) {
-                return naturalSort(a.label, b.label);
+                return naturalSort(a[2], b[2]);
             });
         } else {
             // sort this list by count = index 3
             rows.sort(function(a, b) {
-                return b.count - a.count;
+                return b[3] - a[3];
             }); // reverse-sort by count
         }
         buildLegendBar();
     }
 
     //function filterCoordsAndUpdate(cellIds, mode) {
     /* hide/show currently selected cell IDs or "show all". Rebuild the legend and the coloring. */
@@ -3769,20 +1651,20 @@
         menuBarHide("#tpShowAllButton");
         gLegend.lastClicked = null;
         renderer.render(stage);
     } */
 
     function onHideShowLabelsClick(ev) {
         /* user clicked the hide labels / show labels menu entry */
-        if ($("#tpHideMenuEntry").text() === SHOWLABELSNAME) {
+        if ($("#tpHideShowLabels").text() === SHOWLABELSNAME) {
             renderer.setShowLabels(true);
-            $("#tpHideMenuEntry").text(HIDELABELSNAME);
+            $("#tpHideShowLabels").text(HIDELABELSNAME);
         } else {
             renderer.setShowLabels(false);
-            $("#tpHideMenuEntry").text(SHOWLABELSNAME);
+            $("#tpHideShowLabels").text(SHOWLABELSNAME);
         }
 
         renderer.drawDots();
     }
 
     function onSizeClick(ev) {
         /* user clicked circle size menu entry */
@@ -3799,14 +1681,15 @@
         /* in addition to zooming (done by maxPlot already), reset the URL */
         changeUrl({
             'zoom': null
         });
         renderer.zoom100();
         renderer.drawDots();
         $("#tpZoom100Button").blur(); // remove focus
+        //#$("#tpZoom100Button").tooltip('hide');
         ev.preventDefault();
         return false;
     }
 
     function activateMode(modeName) {
         renderer.activateMode(modeName);
     }
@@ -3823,60 +1706,48 @@
         pushZoomState(zoomRange);
         renderer.drawDots();
         ev.preventDefault();
     }
 
     function onWindowResize(ev) {
         /* called when window is resized by user */
-        if (ev.target.id === "tpHeat") // hack: do not do anything if jquery resizable() started this.
-            return;
         resizeDivs();
     }
 
     function onColorPaletteClick(ev) {
         /* called when users clicks a color palette */
         var palName = ev.target.getAttribute("data-palette");
-        if (palName === "default")
-            legendSetColors(gLegend, null) // reset the colors
         legendChangePaletteAndRebuild(palName);
         renderer.drawDots();
     }
 
     function buildEmptyLegendBar(fromLeft, fromTop) {
         // create an empty right side legend bar
         var htmls = [];
         htmls.push("<div id='tpLegendBar' style='position:absolute;top:" + fromTop + "px;left:" + fromLeft + "px; width:" + legendBarWidth + "px'>");
-        htmls.push("<div class='tpSidebarHeader'><div style='float:left'>Legend</div>");
+        htmls.push("<div class='tpSidebarHeader'>Legend");
 
         //htmls.push("<div id='tpToolbarButtons' style='padding-bottom: 2px'>");
         htmls.push("<div style='float:right' class='btn-group btn-group-xs'>");
         htmls.push("<button type='button' class='btn btn-default dropdown-toggle' data-toggle='dropdown' aria-haspopup='true' aria-expanded='false' id='tpChangeColorScheme'>Colors&nbsp;<span class='caret'> </span></button>");
         htmls.push('<ul class="dropdown-menu pull-right">');
         htmls.push('<li><a class="tpColorLink" data-palette="default" href="#">Reset to Default</a></li>');
-        htmls.push('<li><a class="tpColorLink" data-palette="rainbow" href="#">Qualitative: Rainbow</a></li>');
-        htmls.push('<li><a class="tpColorLink" data-palette="tatarize" href="#">Qualitative: Tatarize</a></li>');
-        htmls.push('<li><a class="tpColorLink" data-palette="iwanthue" href="#">Qualitative: Iwanthue</a></li>');
-        htmls.push('<li><a class="tpColorLink" data-palette="tol-dv" href="#">Semi-Qualitative: Paul Tol&#39;s</a></li>');
-        //htmls.push('<li><a class="tpColorLink" data-palette="cb-Paired" href="#">Qualitative: paired</a></li>');
-        //htmls.push('<li><a class="tpColorLink" data-palette="cb-Set3" href="#">Qualitative: pastel</a></li>');
-        htmls.push('<li><a class="tpColorLink" data-palette="blues" href="#">Gradient: shades of blue</a></li>');
-        htmls.push('<li><a class="tpColorLink" data-palette="reds" href="#">Gradient: shades of red</a></li>');
-        htmls.push('<li><a class="tpColorLink" data-palette="tol-sq-blue" href="#">Gradient: beige to red</a></li>');
-        htmls.push('<li><a class="tpColorLink" data-palette="tol-rainbow" href="#">Gradient: blue to red</a></li>');
-        htmls.push('<li><a class="tpColorLink" data-palette="viridis" href="#">Gradient: Viridis</a></li>');
-        htmls.push('<li><a class="tpColorLink" data-palette="magma" href="#">Gradient: Magma</a></li>');
-        htmls.push('<li><a class="tpColorLink" data-palette="inferno" href="#">Gradient: Inferno</a></li>');
-        htmls.push('<li><a class="tpColorLink" data-palette="plasma" href="#">Gradient: Plasma</a></li>');
+        htmls.push('<li><a class="tpColorLink" data-palette="rainbow" href="#">Rainbow Qualitative</a></li>');
+        htmls.push('<li><a class="tpColorLink" data-palette="tol-dv" href="#">Paul Tol&#39;s Qualitative</a></li>');
+        htmls.push('<li><a class="tpColorLink" data-palette="blues" href="#">Shades of Blues</a></li>');
+        htmls.push('<li><a class="tpColorLink" data-palette="reds" href="#">Shades of Reds</a></li>');
+        htmls.push('<li><a class="tpColorLink" data-palette="tol-sq" href="#">Beige to red</a></li>');
+        htmls.push('<li><a class="tpColorLink" data-palette="tol-rainbow" href="#">Blue to red</a></li>');
         htmls.push('</ul>');
         htmls.push("</div>"); // btn-group
         //htmls.push("</div>"); // tpToolbarButtons
 
         htmls.push("</div>"); // tpSidebarHeader
 
-        //htmls.push("<div id='tpLegendTitleBox' style='position:relative; width:100%; height:1.5em'>");
+        htmls.push("<div id='tpLegendTitleBox' style='position:relative; width:100%; height:1.5em; font-weight: bold'>");
         htmls.push("<div id='tpLegendContent'>");
         htmls.push("</div>"); // content
         htmls.push("</div>"); // bar
         $(document.body).append(htmls.join(""));
 
         $(".tpColorLink").click(onColorPaletteClick);
     }
@@ -3906,357 +1777,216 @@
         }
         return table;
     }
 
     function legendGetColors(rows) {
         /* go over the legend lines: create an array of colors in the order of their meta value indexes.
          * (the values in the legend may be sorted not in the order of their internal indices) */
-        if (rows === undefined)
-            return [];
-
         var colArr = [];
         for (var i = 0; i < rows.length; i++) {
             var row = rows[i];
-            var col = row.color;
+            var col = row[0];
             if (col === null)
-                col = row.defColor; // only use default color if nothing else set
+                col = row[1]; // only use default color if nothing else set
 
-            var idx = row.intKey;
+            var idx = row[4]; // 4 = meta val index or expression bin XX
             colArr[idx] = col; // 0 = color
         }
 
         return colArr;
     }
 
-    function legendUpdateLabels(fieldName) {
-        /* re-copy the labels into the legend rows */
-        // rows have attributes like these: defColor, currColor, label, count, valueIndex, uniqueKey
-        var shortLabels = db.findMetaInfo(fieldName).ui.shortLabels;
-        var rows = gLegend.rows;
-        for (var i = 0; i < rows.length; i++) {
-            var row = rows[i];
-            var valIdx = row.intKey;
-            var shortLabel = shortLabels[valIdx];
-            row.label = shortLabel;
-        }
-    }
-
-    function legendRemoveManualColors(gLegend) {
-        /* remove all manually defined colors from the legend */
-        // reset the legend object
-        legendSetColors(gLegend, null, "color");
-
-        // reset the URL and local storage settings
-        var rows = gLegend.rows;
-        var urlChanges = {};
-        for (var i = 0; i < rows.length; i++) {
-            var row = rows[i];
-            var urlVar = COL_PREFIX + row.strKey;
-            localStorage.removeItem(urlVar);
-            urlChanges[urlVar] = null;
-
-        }
-        changeUrl(urlChanges);
-    }
-
-    function legendChangePaletteAndRebuild(palName, resetManual) {
+    function legendChangePaletteAndRebuild(palName) {
         /* change the legend color palette and put it into the URL */
-        var success = legendSetPalette(gLegend, palName);
+        var rows = gLegend.rows;
+        var success = legendSetPalette(gLegend, palName, gLegend.metaFieldIdx);
         if (success) {
-            if (palName === "default") {
-                legendRemoveManualColors(gLegend);
+            if (palName === "default")
                 changeUrl({
                     "pal": null
                 });
-            } else
+            else
                 changeUrl({
                     "pal": palName
                 });
             buildLegendBar();
             var colors = legendGetColors(gLegend.rows);
             renderer.setColors(colors);
         }
     }
 
-    function legendSetColors(legend, colors, keyName) {
-        /* set the colors for all legend rows, keyName can be "color" or "defColor", depending on
-         * whether the current row color or the row default color should be changed.
-         * colors can also be null to reset all values to null. */
-        if (!keyName)
-            keyName = "color";
-        var rows = legend.rows;
-        for (let i = 0; i < rows.length; i++) {
-            var colorVal = null;
-            if (colors)
-                colorVal = colors[i];
-
-            var legendRow = rows[i];
-            if (legendRow.label == "0" && legend.type == "expr")
-                colorVal = cNullColor;
-            legendRow[keyName] = colorVal;
-        }
-    }
-
-    function legendSetPalette(legend, origPalName) {
+    function legendSetPalette(legend, origPalName, metaFieldIndex) {
         /* update the defColor [1] attribute of all legend rows. pal is an array of hex colors.
-         * Will use the predefined colors that are
-         * in the legend.metaInfo.colors configuration, if present.
+         * metaFieldIndex is optional. If it is set, will use the predefined colors that are
+         * in the field configuration.
          * */
         var palName = origPalName;
+
+        //palName = getVar("pal", palName);
+
         if (origPalName === "default") {
+            legendResetColors();
+            //changeUrl({"pal":null});
             if (legend.rowType === "category")
-                palName = datasetQualPalette;
+                palName = cDefQualPalette;
             else
-                palName = datasetGradPalette;
+                palName = cDefGradPalette;
         }
 
         var rows = legend.rows;
         var n = rows.length;
         var pal = null;
         var usePredefined = false;
-
-        pal = makeColorPalette(palName, n);
-        // if this is a field for which colors were defined manually during the cbBuild, use them
-        if (legend.metaInfo !== undefined && legend.metaInfo.colors !== undefined && origPalName === "default") {
-            // the order of the color values in the metaInfo object is the same as the order of the order of the values in the
-            // JSON file. But the legend has been sorted now, so we cannot just copy over the array as it is
-            var rows = legend.rows;
-            var predefColors = legend.metaInfo.colors;
-            for (var i = 0; i < rows.length; i++) {
-                var origIndex = rows[i].intKey;
-                var col = predefColors[origIndex];
-                if (col !== null)
-                    pal[i] = col;
-            }
+        // if this is a field for which colors were defined manually, use them
+        if (metaFieldIndex !== undefined && db.conf.metaFields[metaFieldIndex].colors !== undefined && origPalName === "default") {
+            pal = db.conf.metaFields[metaFieldIndex].colors;
             usePredefined = true;
         } else
             pal = makeColorPalette(palName, n);
 
         if (pal === null) {
-            alert("Sorry, palette '" + palName + "' does not have " + rows.length + " different colors");
+            alert("Sorry, this palette does not have " + rows.length + " different colors");
             return false;
         }
 
-        legendSetColors(legend, pal, "defColor");
+        for (var i = 0; i < rows.length; i++) {
+            rows[i][1] = pal[i];
+        }
         legend.palName = palName;
 
         // update the dropdown menu
         $('.tpColorLink').parent().removeClass("active");
         // force the menu to the "defaults" entry if we're using predefined colors
         if (usePredefined)
             palName = "default";
         $('.tpColorLink[data-palette="' + palName + '"]').parent().addClass("active");
         return true;
     }
 
-    function labelForBinMinMax(binMin, binMax, isAllInt) {
-        /* given the min/max of a numeric value bin, return a good legend for it */
-        // pretty print the numbers
-        var minDig = 2;
-        //if (binMin % 1 === 0) // % 1 = fractional part
-        //minDig = 0
-
-        var maxDig = 2;
-        //if (binMin % 1 === 0)
-        //   maxDig = 0
-
-
-        if (isAllInt) {
-            minDig = 0;
-            maxDig = 0
-        }
-
-        var legLabel = "";
-        if (binMax === 0 && binMax === 0)
-            legLabel = "0";
-        else if (binMin === "Unknown")
-            legLabel = "Unknown";
-        else if (binMin !== binMax) {
-            if (Math.abs(binMin) > 1000000)
-                binMin = binMin.toPrecision(4);
-            if (Math.abs(binMax) > 1000000)
-                binMax = binMax.toPrecision(4);
-            if (typeof(binMin) === 'number')
-                binMin = binMin.toFixed(minDig);
-            if (typeof(binMax) === 'number')
-                binMax = binMax.toFixed(minDig);
-
-            legLabel = binMin + '&ndash;' + binMax;
-        } else
-            legLabel = binMin.toFixed(minDig);
-        return legLabel;
-    }
-
     function makeLegendRowsNumeric(binInfo) {
         /* return an array of legend lines given bin info from gene expression or a numeric meta field  */
         var legendRows = [];
+        //var zeroIsGrey = false;
 
-        // figure out if all our ranges are integers
-        var isAllInt = true;
-        for (var binIdx = 0; binIdx < binInfo.length; binIdx++) {
-            let oneBin = binInfo[binIdx];
-            var binMin = oneBin[0];
-            var binMax = oneBin[1];
-
-            var restMin = binMin - Math.trunc(binMin);
-            var restMax = binMax - Math.trunc(binMax);
-            if (restMin !== 0 || restMax !== 0)
-                isAllInt = false;
-        }
+        // special case for the first "0" element = no value, make this always grey
+        //var bin0Min = binInfo[0][0];
+        //var bin0Max = binInfo[0][1];
+        //if (bin0Min===0 && bin0Max===0)
+        //zeroIsGrey = true;
 
+        //var defColors = makeColorPalette(10, true, zeroIsGrey);
         var colIdx = 0;
         for (var binIdx = 0; binIdx < binInfo.length; binIdx++) {
-            let oneBin = binInfo[binIdx];
-
-            var binMin = oneBin[0];
-            var binMax = oneBin[1];
-            var count = oneBin[2];
+            var binMin = binInfo[binIdx][0];
+            var binMax = binInfo[binIdx][1];
 
+            var count = binInfo[binIdx][2];
             var legendId = binIdx;
 
-            var legLabel = labelForBinMinMax(binMin, binMax, isAllInt);
+            // pretty print the numbers
+            var minDig = 2;
+            //if (binMin % 1 === 0) // % 1 = fractional part
+            //minDig = 0
+
+            var maxDig = 2;
+            //if (binMin % 1 === 0)
+            //   maxDig = 0
+
+            var legLabel = null;
+            if (binMin === "Unknown")
+                legLabel = "Unknown";
+            else if (binMin !== binMax)
+                legLabel = binMin.toFixed(minDig) + ' - ' + binMax.toFixed(maxDig);
+            else
+                legLabel = binMin.toFixed(minDig);
 
             var uniqueKey = legLabel;
+            var legColor = null;
 
             // override any color with the color specified in the current URL
             var savKey = COL_PREFIX + legLabel;
             var legColor = getVar(savKey, null);
 
             if (binMin === 0 && binMax === 0) {
-                uniqueKey = "noExpr";
-                legColor = cNullColor;
-            } else if (binMin === "Unknown" && binMax === "Unknown") {
+                legLabel = "No Value";
                 uniqueKey = "noExpr";
                 legColor = cNullColor;
             } else
                 colIdx++;
 
-            legendRows.push({
-                "color": legColor,
-                "defColor": null,
-                "label": legLabel,
-                "count": count,
-                "intKey": binIdx,
-                "strKey": uniqueKey
-            });
+            legendRows.push([legColor, null, legLabel, count, binIdx, uniqueKey]);
         }
         return legendRows;
     }
 
-    function makeLegendExpr(geneSym, mouseOver, binInfo, exprVec, decExprVec) {
+    function makeLegendExpr(geneSym, geneId, binInfo, exprVec, decExprVec) {
         /* build gLegend object for coloring by expression
          * return the colors as an array of hex codes */
 
         activateTooltip("#tpGeneSym");
 
         var legendRows = makeLegendRowsNumeric(binInfo);
+        var colors = legendGetColors(legendRows);
 
-        gLegend = {};
-        gLegend.type = "expr";
         gLegend.rows = legendRows;
-        var subTitle = null;
-        if (db.conf.atacSearch)
-            gLegend.title = ("sum of " + geneSym.split("+").length) + " peaks";
-        else {
-            //  make a best effort to find the gene sym and gene ID
-            var geneInfo = db.getGeneInfo(geneSym);
-            geneSym = geneInfo.sym;
-            subTitle = geneInfo.id;
-            gLegend.title = getGeneLabel() + ": " + geneSym;
-        }
-
-        gLegend.titleHover = mouseOver;
+        gLegend.title = "Gene: " + geneSym;
+        gLegend.titleHover = geneId;
         gLegend.geneSym = geneSym;
-        gLegend.subTitle = mouseOver;
         gLegend.rowType = "range";
         gLegend.exprVec = exprVec; // raw expression values, e.g. floats
         gLegend.decExprVec = decExprVec; // expression values as deciles, array of bytes
-        gLegend.selectionDirection = "all";
-        var oldPal = getVar("pal", "default")
-        legendSetPalette(gLegend, oldPal);
-
-        var colors = legendGetColors(legendRows);
+        legendSetPalette(gLegend, "default");
         return colors;
     }
 
-    function alphaNumSearch(genes, saneSym) {
-        /* use alpha-num-only search in gene list for saneSym */
-        for (var i = 0; i < genes.length; i++) {
-            var geneSym = genes[i][0];
-            if (saneSym === onlyAlphaNum(geneSym))
-                return geneSym;
-        }
-        return null;
-    }
-
-    function phoneHome() {
-        /* add empty javascript to document so we can count usage at UCSC for grant reports */
-        /* -> does this pose a data protection issue? Need to document. Does it require opt-in ? */
-        var s = document.createElement('script');
-        s.setAttribute('src', "https://cells.ucsc.edu/js/cbTrackUsage.js");
-        s.async = true;
-        document.body.appendChild(s);
-    }
-
     function onGeneClick(event) {
         /* user clicked on a gene in the gene table */
-        var locusId = event.target.getAttribute("data-geneId"); // the geneId of the gene
-        var locusLabel = event.target.textContent;
+        var geneIdx = parseInt(event.target.id.split("_")[1]); // the index of the gene
         $('.tpMetaBox').removeClass('tpMetaSelect');
         $('.tpGeneBarCell').removeClass("tpGeneBarCellSelected");
-        // XX TODO: How find all the elements with this ID?
-        var saneId = onlyAlphaNum(locusId)
-        $('#tpGeneBarCell_' + saneId).addClass("tpGeneBarCellSelected");
-
-        colorByLocus(locusId, null, locusLabel);
-        event.stopPropagation();
+        $('#tpGeneBarCell_' + geneIdx).addClass("tpGeneBarCellSelected");
+        var geneSym = db.conf.quickGenes[geneIdx][0];
+        loadGeneAndColor(geneSym);
     }
 
     function showDialogBox(htmlLines, title, options) {
         /* show a dialog box with html in it */
         $('#tpDialog').remove();
 
         var addStr = "";
         if (options.width !== undefined)
             addStr = "max-width:" + options.width + "px;";
         var maxHeight = $(window).height() - 200;
         // unshift = insert at pos 0
-        //htmlLines.unshift("<div style='display:none;"+addStr+"max-height:"+maxHeight+"px' id='tpDialog' title='"+title+"'>");
-        htmlLines.unshift("<div style='display:none;" + addStr + "' id='tpDialog' title='" + title + "'>");
+        htmlLines.unshift("<div style='display:none;" + addStr + "max-height:" + maxHeight + "px' id='tpDialog' title='" + title + "'>");
         htmlLines.push("</div>");
         $(document.body).append(htmlLines.join(""));
 
         var dialogOpts = {
             modal: true,
             closeOnEscape: true
         };
         if (options.width !== undefined)
             dialogOpts["width"] = options.width;
         if (options.height !== undefined)
             dialogOpts["height"] = options.height;
-        //dialogOpts["maxHeight"] = maxHeight;
+        dialogOpts["maxHeight"] = maxHeight;
         if (options.buttons !== undefined)
             dialogOpts["buttons"] = options.buttons;
         else
-            dialogOpts["buttons"] = [];
+            dialogOpts["buttons"] = {};
 
-        if (options.showClose !== undefined)
-            dialogOpts["buttons"].unshift({
-                text: "Cancel",
-                click: function() {
-                    $(this).dialog("close");
-                }
-            });
         if (options.showOk !== undefined)
-            dialogOpts["buttons"].push({
-                text: "OK",
-                click: function() {
-                    $(this).dialog("close");
-                }
-            });
+            dialogOpts["buttons"].OK = function() {
+                $(this).dialog("close");
+            };
+        if (options.showClose != undefined)
+            dialogOpts["buttons"].Cancel = function() {
+                $(this).dialog("close");
+            };
         //dialogOpts["position"] = "center";
         //dialogOpts["height"] = "auto";
         //dialogOpts["width"] = "auto";
 
         $("#tpDialog").dialog(dialogOpts);
     }
 
@@ -4271,18 +2001,17 @@
             htmls.push(geneFields[i][1] + "\r\n");
         }
         htmls.push("</textarea>");
         //htmls.push("<p>");
         //htmls.push("<button style='float:center;' id='tpGeneDialogOk' class='ui-button ui-widget ui-corner-all'>OK</button>");
         //htmls.push("</div>");
         //htmls.push("</div>");
-        var buttons = [{
-            text: "OK",
-            click: onGeneDialogOkClick
-        }];
+        var buttons = {
+            "OK": onGeneDialogOkClick
+        };
         showDialogBox(htmls, "Genes of interest", {
             height: 500,
             width: 400,
             buttons: buttons
         });
 
         $('#tpGeneDialogOk').click(onGeneDialogOkClick);
@@ -4302,15 +2031,15 @@
         // newExprData cellId -> list of values (one per gene)
 
         // initialize an empty dict cellId = floats, one per gene
         var newExprData = {};
         var geneCount = gLoad_geneList.length;
         var cellIdCount = cellIds.length;
         for (var i = 0; i < cellIdCount; i++) {
-            let cellId = cellIds[i];
+            cellId = cellIds[i];
             newExprData[cellId] = new Float32Array(gLoad_geneList); // XX or a = [] + a.length = x ?
         }
 
         // do the data transform
         var newGeneFields = [];
         var newDeciles = {};
         for (var geneI = 0; geneI < gLoad_geneList.length; geneI++) {
@@ -4320,27 +2049,28 @@
             var geneId = geneInfo[0];
             var geneVec = geneInfo[1];
             var deciles = geneInfo[2];
             newGeneFields.push([geneSym, geneId]);
             newDeciles[geneSym] = deciles;
 
             for (var cellI = 0; cellI < cellIdCount; cellI++) {
-                let cellId = cellIds[cellI];
+                cellId = cellIds[cellI];
                 newExprData[cellId][geneI] = geneVec[cellI];
             }
         }
 
         gLoad_geneList = null;
         gLoad_geneExpr = null;
 
         gCurrentDataset.preloadExpr = {};
         gCurrentDataset.preloadExpr.genes = newGeneFields;
         gCurrentDataset.preloadExpr.cellExpr = newExprData;
         gCurrentDataset.preloadExpr.deciles = newDeciles;
 
+        //tpGeneTable();
     }
 
     //function onReceiveExprLineProgress(line) {
     /* called when a line of the expression matrix has been loaded: parse line and upd. progressbar */
     //var symbol = this.geneSymbol;
     //console.log("Got gene "+symbol);
     //var exprTuple = parseMatrixLine(line);
@@ -4355,14 +2085,27 @@
     //$( "#tpProgressLabel" ).text(symbol);
     //
     //var progrMax = progressbar.progressbar("option", "max");
     //if (val >= progrMax)
     //onGeneLoadComplete();
     //}
 
+    /**
+     from https://stackoverflow.com/questions/29855098/is-there-a-built-in-javascript-function-similar-to-os-path-join:
+     * Joins 2 paths together and makes sure there aren't any duplicate seperators
+     * @param parts the parts of the url to join. eg: ['http://google.com/', '/my-custom/path/']
+     * @param separator The separator for the path, defaults to '/'
+     * @returns {string} The combined path
+     */
+    function joinPaths(parts, separator) {
+        return parts.map(function(part) {
+            return part.trim().replace(/(^[\/]*|[\/]*$)/g, '');
+        }).join(separator || '/');
+    }
+
     //function singleExprDone() {
     ///* called when both cellIds(header) and single line of the expr matrix have been read */
     //    var sExpr = gCurrentDataset.singleExpr;
     //    if (sExpr.exprVec===undefined || gCurrentDataset.matrixCellIds==undefined)
     //        // don't proceed if one part of the data is not here yet
     //        return;
 
@@ -4420,15 +2163,15 @@
         $("#tpDialog").remove();
 
         gLoad_geneList = [];
         gLoad_geneExpr = {};
 
         var notFoundGenes = [];
         var baseUrl = gCurrentDataset.baseUrl;
-        var url = cbUtil.joinPaths([baseUrl, "geneMatrix.tsv"]);
+        var url = joinPaths([baseUrl, "geneMatrix.tsv"]);
         var validCount = 0; // needed for progressbar later
         var matrixOffsets = gCurrentDataset.matrixOffsets;
         for (var i = 0; i < genes.length; i++) {
             var gene = genes[i];
             if (gene.length === 0) // skip empty lines
                 continue;
             if (!(gene in matrixOffsets)) {
@@ -4449,130 +2192,72 @@
                 success: onReceiveExprLineProgress
             });
         }
 
         var htmls = [];
         htmls.push("<div id='tpGeneProgress'><div class='tpProgressLabel' id='tpProgressLabel'>Loading...</div></div>");
 
-        if (notFoundGenes.length !== 0) {
+        if (notFoundGenes.length != 0) {
             htmls.push("<div id='tpNotFoundGenes'>Could not find the following gene symbols: ");
             htmls.push(notFoundGenes.join(", "));
             htmls.push("</div>");
             //htmls.push("<button style='float:center;' id='tpGeneDialogOk' class='ui-button ui-widget ui-corner-all'>OK</button>");
             //for (var i = 0; i < notFoundGenes.length; i++) {
             //htmls.push(notFoundGenes[i]);
             //}
             //htmls.push("<p>Could not find the following gene symbols:</p>");
             //showDialogBox(htmls, "Warning", 400);
         }
 
-        var showOk = (notFoundGenes.length !== 0);
+        var showOk = (notFoundGenes.length != 0);
         showDialogBox(htmls, "Downloading expression data", {
             width: 350,
             showOk: true
         });
 
         var progressLabel = $("#tpProgressLabel");
         $("#tpGeneProgress").progressbar({
             value: false,
             max: gLoad_geneList.length
         });
 
     }
 
-    function buildGeneTable(htmls, divId, title, subtitle, geneInfos, noteStr, helpText) {
-        /* create gene expression info table. if htmls is null, update DIV with divId in-place. 
-         * geneInfos is array of [gene, mouseover]. gene can be geneId+"|"+symbol. 
-         * You must run activateTooltip(".hasTooltip") after adding the htmls.
-         * */
-        var doUpdate = false;
-        if (htmls === null) {
-            htmls = [];
-            doUpdate = true;
-        }
-
-        var tableWidth = metaBarWidth;
-
-        if (title) {
-            htmls.push("<div style='margin-top:8px' id='" + divId + "_title'>");
-            htmls.push("<div style='display: inline; padding-left:3px; font-weight:bold'>" + title + "</div>");
-            if (helpText) {
-                // https://fontawesome.com/icons/circle-info?s=solid
-                var iconHtml = '<svg style="width:0.9em" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"><!--! Font Awesome Pro 6.1.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2022 Fonticons, Inc. --><path d="M256 0C114.6 0 0 114.6 0 256s114.6 256 256 256s256-114.6 256-256S397.4 0 256 0zM256 128c17.67 0 32 14.33 32 32c0 17.67-14.33 32-32 32S224 177.7 224 160C224 142.3 238.3 128 256 128zM296 384h-80C202.8 384 192 373.3 192 360s10.75-24 24-24h16v-64H224c-13.25 0-24-10.75-24-24S210.8 224 224 224h32c13.25 0 24 10.75 24 24v88h16c13.25 0 24 10.75 24 24S309.3 384 296 384z"/></svg>';
-                htmls.push("<span class='hasTooltip' title='" + helpText + "'>&nbsp;" + iconHtml + "</span>");
-            }
-            if (subtitle) {
-                htmls.push('<div style="margin-top:6px" class="tpHint">');
-                htmls.push(subtitle);
-                htmls.push('</div>');
-            }
-            htmls.push("</div>"); // divId_title
+    function buildGeneTable(htmls, tableWidth, cellWidth, geneInfos) {
+        /* create gene expression info table */
+        $('#tpGenes').remove();
 
-        }
+        if (db.conf.quickGenes === undefined)
+            return;
 
-        if (doUpdate) {
-            $('#' + divId).empty();
-        }
 
-        htmls.push("<div id='" + divId + "'>");
+        htmls.push("<div style='margin-top:8px' id='tpGenes'>");
+        htmls.push("<div style='padding-left:3px; font-weight:bold'>Quick Genes<div>");
+        htmls.push('<div style="margin-top:6px" class="tpHint">');
+        htmls.push('Hover or select cells to update colors.');
+        htmls.push('</div>');
+        htmls.push('<table style="margin-top:10px" id="tpGeneTable"><tr>');
+        //htmls.push('<td><button id="tpChangeGenes" title="Change the list of genes that are displayed in this table" class = "ui-button ui-widget ui-corner-all" style="width:95%">Change</button></td>');
 
-        if (geneInfos === undefined || geneInfos === null || geneInfos.length === 0) {
-            if (noteStr !== undefined)
-                htmls.push("<div style='font-style:80%'>" + noteStr + "</div>");
-            htmls.push("</div>");
-            return;
-        }
+        var colsPerRow = Math.round(tableWidth / cellWidth);
+        var cellWidth = Math.round(tableWidth / colsPerRow);
 
-        var i = 0;
-        while (i < geneInfos.length) {
+        var currWidth = 1;
+        for (var i = 0; i < geneInfos.length; i++) {
             var geneInfo = geneInfos[i];
-            var geneIdOrSym = geneInfo[0];
+            var geneId = geneInfo[0];
             var geneDesc = geneInfo[1];
-            if (geneDesc === undefined)
-                geneDesc = geneId;
-
-            // geneIdOrSym can be just the symbol (if we all we have is symbols) or geneId|symbol
-            var geneId
-            var sym;
-            if (geneIdOrSym.indexOf("|") !== -1) {
-                var parts = geneIdOrSym.split("|");
-                geneId = parts[0];
-                sym = parts[1];
-            } else {
-                geneId = geneIdOrSym;
-                sym = geneId;
+            var pubDesc = geneInfo[2];
+            if (((i % colsPerRow) == 0) && (i != 0)) {
+                htmls.push("</tr><tr>");
             }
-
-            htmls.push('<span title="' + geneDesc + '" style="width: fit-content;" data-geneId="' + geneId + '" id="tpGeneBarCell_' + onlyAlphaNum(geneId) + '" class="tpGeneBarCell">' + sym + '</span>');
-            i++;
+            htmls.push('<td title="' + geneDesc + '" id="tpGeneBarCell_' + i + '" class="tpGeneBarCell">' + geneId + '</td>');
         }
-        htmls.push("</div>"); // divId
+        htmls.push("</tr></table>");
 
-        if (doUpdate) {
-            $('#' + divId).html(htmls.join(""));
-        }
-    }
-
-    function resizeGeneTableDivs(tableId) {
-        /* the size of the DIVs in the gene table depends on the size of the longest DIV in pixels and we know that only once the table is shown. so resize here now */
-        var tdEls = document.getElementById(tableId).querySelectorAll("span");
-        var maxWidth = 0;
-        var totalWidth = 0;
-        for (var el of tdEls) {
-            maxWidth = Math.max(maxWidth, el.offsetWidth + 2); // 2 pixel borders
-            totalWidth = totalWidth + el.offsetWidth;
-        }
-
-        // if we have less than one row, make the cells cover the whole row, but limit the total size a little
-        if (totalWidth < (metaBarWidth - (tdEls.length * 6))) // 6 pixels for the borders = 2 + 2 + 2 for the selection border.
-            maxWidth = Math.min(70, Math.floor(metaBarWidth / tdEls.length) - 6);
-
-        for (var el of tdEls) {
-            el.style.minWidth = maxWidth + "px";
-        }
     }
 
     function likeEmptyString(label) {
         /* some special values like "undefined" and empty string get colored in grey  */
         return (label === null || label.trim() === "" || label === "none" || label === "None" || label === "unknown" ||
             label === "nd" || label === "n.d." ||
             label === "Unknown" || label === "NaN" || label === "NA" || label === "undefined" || label === "Na");
@@ -4581,1436 +2266,640 @@
     function numMetaToBinInfo(fieldInfo) {
         /* convert a numeric meta field info to look like gene expression info for the legend:
          * an array of [start, end, count] */
         var binInfo = [];
         var binMethod = fieldInfo.binMethod;
         if (binMethod === "uniform") {
             // old method, not used anymore
-            let binMin = fieldInfo.minVal;
+            var binMin = fieldInfo.minVal;
             var stepSize = fieldInfo.stepSize;
-            let binCounts = fieldInfo.binCounts;
-            let binCount = fieldInfo.binCounts.length;
+            var binCounts = fieldInfo.binCounts;
+            var binCount = fieldInfo.binCounts.length;
             for (var i = 0; i < binCount; i++) {
                 binInfo.push([binMin, binMin + stepSize, binCounts[i]]);
                 binMin += stepSize;
             }
         } else if (binMethod === "quantiles") {
-            // newer method for pre-quantified fields
-            let binMin = fieldInfo.minVal;
-            let breaks = fieldInfo.breaks;
-            let binCounts = fieldInfo.binCounts;
-            let binCountsLen = fieldInfo.binCounts.length;
-            let binIdx = 0;
-            if (breaks[0] === "Unknown") {
+            var binMin = fieldInfo.minVal;
+            var breaks = fieldInfo.breaks;
+            var binCounts = fieldInfo.binCounts;
+            var binCountsLen = fieldInfo.binCounts.length;
+            var binIdx = 0;
+            if (breaks[0] == "Unknown") {
                 binInfo.push(["Unknown", "Unknown", binCounts[0]]);
                 binIdx = 1;
             }
 
             for (; binIdx < binCountsLen; binIdx++) {
-                let binMin = breaks[binIdx];
-                let binMax = breaks[binIdx + 1];
-                let binCount = binCounts[binIdx];
+                var binMin = breaks[binIdx];
+                var binMax = breaks[binIdx + 1];
+                var binCount = binCounts[binIdx];
                 binInfo.push([binMin, binMax, binCount]);
             }
         } else if (binMethod === "raw") {
             // no binning was done at all, this happens when there are not enough distinct values
-            let values = fieldInfo.values;
-            let binCounts = fieldInfo.binCounts;
-            for (let i = 0; i < values.length; i++) {
-                let value = values[i];
-                let valCount = binCounts[i];
+            var values = fieldInfo.values;
+            var binCounts = fieldInfo.binCounts;
+            for (var i = 0; i < values.length; i++) {
+                var value = values[i];
+                var valCount = binCounts[i];
                 binInfo.push([value, value, valCount]);
             }
         } else
-            // these days, we don't pre-quantify anymore. The binning is done on the client now
-            // and the meta loading function adds the bin info to the field info object
-            //alert("invalid value for meta field binMethod: "+binMethod);
-            binInfo = fieldInfo.binInfo;
+            alert("invalid value for meta field binMethod: " + binMethod);
 
         return binInfo;
     }
 
-    function getFieldColors(metaInfo) {
-        /* return a list with the color codes for a field, taking into account field type and cart settings */
-
-        let palName = metaInfo.ui.palette;
-        let colCount;
-        if (!palName)
-            if (metaInfo.type === "int" || metaInfo.type === "float") {
-                palName = datasetGradPalette;
-                colCount = exprBinCount + 1; // +1 because <unknown> is a special bin
-            }
-        else {
-            palName = cDefQualPalette;
-            colCount = metaInfo.valCounts.length;
-        }
-
-        var colors = makeColorPalette(palName, colCount);
-
-        let colOverrides = metaInfo.ui.colors;
-        if (colOverrides)
-            for (let i = 0; i < colOverrides.length; i++)
-                if (colOverrides[i])
-                    colors[i] = colOverrides[i];
-
-        return colors;
-    }
-
-    function makeLegendMeta(metaInfo, sortBy) {
-        /* Build a new legend object and return it */
+    function makeLegendMeta(metaIndex, sortBy) {
+        /* Build a new gLegend object and return it */
         var legend = {};
         legend.type = "meta";
+        legend.metaFieldIdx = metaIndex;
         legend.titleHover = null;
 
-        legend.title = metaInfo.label.replace(/_/g, " ");
-        legend.metaInfo = metaInfo;
+        var fieldInfo = db.getMetaFields()[metaIndex];
+        legend.fieldName = fieldInfo.label;
+        legend.title = legend.fieldName.replace(/_/g, " ");
 
         // numeric meta fields are a special case
-        if (metaInfo.type === "int" || metaInfo.type === "float") {
-            var binInfo = numMetaToBinInfo(metaInfo);
+        if (fieldInfo.type === "int" || fieldInfo.type === "float") {
+            var binInfo = numMetaToBinInfo(fieldInfo);
             legend.rows = makeLegendRowsNumeric(binInfo);
             legend.rowType = "range";
-            legendSetPalette(legend, "default");
+            legendSetPalette(legend, "default", metaIndex);
             return legend;
         }
 
-        if (metaInfo.diffValCount > MAXCOLORCOUNT) {
-            warn("This field has " + metaInfo.diffValCount + " different values. Coloring on a " +
-                "field that has more than " + MAXCOLORCOUNT + " different values is not supported.");
+        if (fieldInfo.diffValCount > MAXCOLORCOUNT) {
+            warn("This field has " + fieldInfo.diffValCount + " different values. Coloring on a field that has more than " + MAXCOLORCOUNT + " different values is not supported.");
             return null;
         }
 
-        var metaCounts = metaInfo.valCounts; // array of [count, value]
+        var metaCounts = fieldInfo.valCounts;
 
         // we are going to sort this list later, so we need to keep track of what the original
         // index in the list was, as every meta data value is stored by its index, not
-        // its label. Simply append the index as [2] of the metaCounts array.
-        for (var valIdx = 0; valIdx < metaCounts.length; valIdx++)
-            metaCounts[valIdx].push(valIdx);
+        // its label. We store the index as [2] of the metaCounts array.
+        if (metaCounts[0].length !== 3)
+            for (var valIdx = 0; valIdx < metaCounts.length; valIdx++)
+                metaCounts[valIdx].push(valIdx);
 
-        var oldSortBy = getFromUrl("SORT");
-        // URL overrides default value
+        var oldSortBy = cartGet("SORT", legend.fieldName);
         if (sortBy === undefined && oldSortBy !== undefined)
             sortBy = oldSortBy;
 
-        // default sorting can be specfied with "sortBy" in cellbrowser.conf
-        if (sortBy === undefined && metaInfo.sortBy)
-            sortBy = metaInfo.sortBy;
-        if (sortBy !== undefined && sortBy !== "freq" && sortBy !== "name" && sortBy !== "none") {
-            alert("sortBy is '" + cleanString(sortBy) + ' but it can only be "freq" or "name"');
-            sortBy = undefined;
-        }
-
-        var fieldName = metaInfo.label;
+        var fieldName = fieldInfo.label;
 
         // force field names that look like "cluster" to a rainbow palette
-        // even if they are numbers
+        // even if they look like numbers
         if (sortBy === undefined) {
             // should cluster fields be sorted by their name
-            if (metaInfo.type === "float" || metaInfo.type === "int" || (metaCounts.length > 60))
-                // long lists are easier to grasp if they're sorted by name
-                sortBy = "name";
-            else if (fieldName.indexOf("luster") || fieldName.indexOf("ouvain") || fieldName.indexOf("res."))
+            if (fieldName.indexOf("luster") || fieldName.indexOf("ouvain"))
                 sortBy = "count";
+            else if (fieldInfo.type === "float" || fieldInfo.type === "int")
+                sortBy = "name";
             else
                 sortBy = "count";
         }
 
         // sort like numbers if the strings are mostly numbers, otherwise sort like strings
         var sortResult = sortPairsBy(metaCounts, sortBy);
         var countListSorted = sortResult.list;
 
-        var useGradient = (metaInfo.type === "float" || metaInfo.type === "int");
+        var useGradient = (fieldInfo.type === "float" || fieldInfo.type === "int");
         //var defaultColors = makeColorPalette(countListSorted.length, useGradient);
 
         var rows = [];
-        var shortLabels = metaInfo.ui.shortLabels;
-        var longLabels = metaInfo.ui.longLabels;
+        //var defColIdx = 0;
         for (var legRowIdx = 0; legRowIdx < countListSorted.length; legRowIdx++) {
             var legRowInfo = countListSorted[legRowIdx];
-            let valIdx = legRowInfo[2]; // index of the original field in fieldInfo
-            var label = shortLabels[valIdx];
-
-            var desc = null;
-            if (longLabels)
-                desc = longLabels[valIdx];
-
-            // first use the default palette, then try to get from URL
+            var label = legRowInfo[0];
             var count = legRowInfo[1];
+            var valIdx = legRowInfo[2];
             var uniqueKey = label;
-            if (uniqueKey === "")
-                uniqueKey = "_EMPTY_";
 
+            //var defColor = defaultColors[legRowIdx];
             if (likeEmptyString(label))
                 color = cNullColor;
+            //else {
+            //defColor = defaultColors[defColIdx];
+            //defColIdx++;
+            //    }
             // override any color with the color specified in the current URL
-            var savKey = COL_PREFIX + uniqueKey;
-            var color = getFromUrl(savKey, null);
+            var savKey = COL_PREFIX + label;
+            var color = cartGet(savKey, null);
 
-            rows.push({
-                "color": color,
-                "defColor": null,
-                "label": label,
-                "count": count,
-                "intKey": valIdx,
-                "strKey": uniqueKey,
-                "longLabel": desc,
-            });
+            rows.push([color, null, label, count, valIdx, uniqueKey]);
         }
 
         legend.rows = rows;
         legend.isSortedByName = sortResult.isSortedByName;
         legend.rowType = "category";
-        legend.selectionDirection = "all";
-        legendSetPalette(legend, "default");
+        legendSetPalette(legend, "default", metaIndex);
         return legend;
     }
 
-    function legendSetTitle(label) {
-        $('#tpLegendTitle').text(label);
-    }
-
-    function buildLegendForMeta(metaInfo) {
-        /* build the gLegend for a meta field */
-        var legend = makeLegendMeta(metaInfo);
-        if (legend === null)
+    function findCellIdsForLegendIds(cellIdToLegendId, legendIds, cellIds) {
+        /* given a legendId, return an object with cellIds that are associated to a given class */
+        if (cellIds == undefined)
+            cellIds = {};
+        for (var i = 0; i < legendIds.length; i++) {
+            var legendId = legendIds[i];
+            for (var cellId in cellIdToLegendId) {
+                if (gClasses[cellId] == legendId)
+                    cellIds[cellId] = true;
+            }
+        }
+        return cellIds;
+    }
+
+    function buildLegendForMetaIdx(fieldId) {
+        /* build the legend for a meta field */
+        var legend = makeLegendMeta(fieldId);
+        if (legend == null)
             return;
 
-        var metaIdx = db.fieldNameToIndex(metaInfo.name);
         $('.tpMetaBox').removeClass('tpMetaSelect');
         $('.tpMetaValue').removeClass('tpMetaValueSelect');
-        $('#tpMetaBox_' + metaIdx).addClass('tpMetaSelect');
-        $('#tpMeta_' + metaIdx).addClass('tpMetaValueSelect');
+        $('#tpMetaBox_' + fieldId).addClass('tpMetaSelect');
+        $('#tpMeta_' + fieldId).addClass('tpMetaValueSelect');
         $('.tpGeneBarCell').removeClass('tpGeneBarCellSelected');
-        //$('#tpLegendTitle').text(legend.metaInfo.label.replace(/_/g, " "));
-        legendSetTitle(legend.metaInfo.label.replace(/_/g, " "));
 
-        return legend;
+        gLegend = legend;
+        buildLegendBar();
+        $('#tpLegendTitle').text(legend.fieldName.replace(/_/g, " "));
     }
 
     function onMetaClick(event) {
         /* called when user clicks a meta data field or label */
-        var fieldName = event.target.dataset.fieldName;
-        if (isNaN(fieldName)) {
-            // try up one level in the DOM tree, in case the user clicked the little child div in the meta list
-            fieldName = event.target.parentElement.dataset.fieldName;
+        var fieldId = parseInt(event.target.id.split("_")[1]);
+        if (isNaN(fieldId)) {
+            // try up one level in the DOM tree
+            fieldId = parseInt(event.target.parentElement.id.split("_")[1]);
         }
-        setColorByDropdown(fieldName);
+        var fieldName = db.getMetaFields()[fieldId].name;
         colorByMetaField(fieldName);
     }
 
-    function addMetaTipBar(htmls, valFrac, valStr, valFracCategory) {
+    function addMetaTipBar(htmls, valFrac, valStr) {
         /* add another bar to a simple histogram built from divs */
         htmls.push("<div>&nbsp;");
         htmls.push("<div class='tpMetaTipPerc'>" + (100 * valFrac).toFixed(1) + "%</div>");
-        htmls.push("<div class='tpMetaTipName'>" + valStr);
-        if (valFracCategory !== undefined) {
-            htmls.push(" <small>(" + (100 * valFracCategory).toFixed(1) + "% of all cells with this value)</small>");
-        }
-        htmls.push("</div>");
+        htmls.push("<div class='tpMetaTipName'>" + valStr + "</div>");
         //htmls.push("<span class='tpMetaTipCount'>"+valCount+"</span>");
         var pxSize = (valFrac * metaTipWidth).toFixed(0);
         htmls.push("<div style='width:" + pxSize + "px' class='tpMetaTipBar'>&nbsp</div>");
         htmls.push("</div>");
     }
 
-    function binInfoToValCounts(binInfo) {
-        /* given an array of (start, end, count), return an array of (label, count) */
-        var valCounts = [];
+    function onMetaMouseOver(event) {
+        /* called when user hovers over meta element: shows the histogram of selected values */
+        var metaHist = gCurrentDataset.metaHist;
+        if (metaHist === undefined)
+            return;
 
-        for (var binIdx = 0; binIdx < binInfo.length; binIdx++) {
-            var binMin = binInfo[binIdx][0];
-            var binMax = binInfo[binIdx][1];
-            var count = binInfo[binIdx][2];
-            var label = labelForBinMinMax(binMin, binMax);
-            valCounts.push([label, count]);
-        }
-        return valCounts;
-    }
+        // mouseover over spans or divs will not find the id, so look at their parent, which is the main DIV
+        var target = event.target;
+        if (target.id === "")
+            target = event.target.parentNode;
+        if (target.id === "")
+            target = event.target.parentNode;
+        var targetId = target.id;
 
-    function buildMetaTip(metaInfo, valHist, htmls) {
-        /* build the content of the tooltip that summarizes the multi selection */
-        var valCounts = metaInfo.valCounts;
-        var shortLabels = metaInfo.ui.shortLabels;
-        if (valCounts === undefined) // for client-side discretized fields, we have to discretize first
-            valCounts = binInfoToValCounts(metaInfo.binInfo);
+        var fieldId = parseInt(targetId.split("_")[1]);
 
+        var valHist = metaHist[fieldId];
+        var htmls = [];
         var otherCount = 0;
         var totalSum = 0;
         for (var i = 0; i < valHist.length; i++) {
             var valInfo = valHist[i];
             var valCount = valInfo[0];
             var valFrac = valInfo[1];
-            var valIdx = valInfo[2];
-            var valFracCategory = valInfo[3];
-            //var valStr   = valCounts[valIdx][0]; // 0 = label, 1 = count
-            var label = shortLabels[valIdx];
+            var valStr = valInfo[2];
 
             totalSum += valCount;
             // only show the top values, summarize everything else into "other"
             if (i > HISTOCOUNT) {
                 otherCount += valCount;
                 continue;
             }
 
-            if (label === "")
-                label = "<span style='color:indigo'>(empty)</span>";
-            addMetaTipBar(htmls, valFrac, label, valFracCategory);
+            if (valStr === "")
+                valStr = "<span style='color:indigo'>(empty)</span>";
+            addMetaTipBar(htmls, valFrac, valStr);
         }
 
         if (otherCount !== 0) {
             var otherFrac = (otherCount / totalSum);
             addMetaTipBar(htmls, otherFrac, "<span style='color:indigo'>(other)</span>");
         }
-        return htmls;
-    }
-
-    function metaInfoFromElement(target) {
-        /* get the metaInfo object given a DOM element  */
-        if (target.dataset.fieldName === undefined)
-            target = target.parentNode;
-        if (target.dataset.fieldName === undefined)
-            target = target.parentNode;
-        var fieldName = target.dataset.fieldName;
-        var metaInfo = db.findMetaInfo(fieldName);
-        return metaInfo;
-    }
-
-    function onMetaMouseOver(event) {
-        /* called when user hovers over meta element: shows the histogram of selected cells */
-        var metaHist = db.metaHist;
-        if (metaHist === undefined || metaHist === null)
-            return;
-
-        // mouseover over spans or divs will not find the id, so look at their parent, which is the main DIV
-        var target = event.target;
-
-        var metaInfo = metaInfoFromElement(target);
-        var fieldName = metaInfo.name;
-
-        // change style of this field a little
-        var metaSel = "#tpMetaBox_" + metaInfo.index;
-        //var backCol = "#666";
-        //var foreCol = "#FFF";
-        //$(metaSel).css({color: foreCol, backgroundColor: backCol});
-        //$(metaSel).children().css({color: foreCol, backgroundColor: backCol});
-        //$(metaSel).children().children().css({color: foreCol, backgroundColor: backCol});
-        $(metaSel).addClass("tpMetaHover");
-        $(metaSel + " .tpMetaValue").addClass("tpMetaHover");
-
-        var htmls = [];
-
-        if (metaInfo.type === "uniqueString")
-            htmls.push("<div>Cannot summarize: this is a field with unique values</div>");
-        else
-            htmls = buildMetaTip(metaInfo, metaHist[fieldName], htmls);
 
         $('#tpMetaTip').html(htmls.join(""));
-
-        // make sure that tooltip doesn't go outside of screen
-        //var tipTop = event.target.offsetTop;
-        var tipTop = event.target.getBoundingClientRect().top - 8;
-        var tipHeight = $('#tpMetaTip').height();
-        var screenHeight = $(window).height();
-        if (tipTop + tipHeight > screenHeight)
-            tipTop = screenHeight - tipHeight - 8;
-
         $('#tpMetaTip').css({
-            top: tipTop + "px",
+            top: event.target.offsetTop + "px",
             left: metaBarWidth + "px",
             width: metaTipWidth + "px"
         });
         $('#tpMetaTip').show();
     }
 
-    function buildComboBox(htmls, id, entries, selIdx, placeholder, width, opts) {
-        /* make html for a combo box and add lines to htmls list.
-         * selIdx is an array of values if opt.multi exists, otherwise it's an int or 'undefined' if none. */
-
-        let addStr = "";
-        if (opts && opts.multi)
-            addStr = " multiple";
-
-        htmls.push('<select style=width:"' + width + 'px" id="' + id + '"' + addStr + ' data-placeholder="' + placeholder + '" class="tpCombo">');
+    function buildComboBox(htmls, id, entries, selIdx, placeholder, width) {
+        /* make html for a combo box and add lines to htmls list */
+        htmls.push('<select style="' + width + 'px" id="' + id + '" data-placeholder="' + placeholder + '" class="tpCombo">');
         for (var i = 0; i < entries.length; i++) {
             var isSelStr = "";
             var entry = entries[i];
-
-            // entries can be either key-val or just values
-            var name, label;
-            if (Array.isArray(entry)) {
-                name = entry[0];
-                label = entry[1];
-            } else {
-                name = label = entry;
-            }
-
-            // determine if element is selected
-            let isSel = false;
-            if (opts && opts.multi) {
-                if (selIdx.indexOf(i) !== -1 || selIdx.indexOf(name) !== -1)
-                    isSel = true;
-            } else if ((selIdx !== undefined && i === selIdx))
-                isSel = true;
-
-            if (isSel)
-                isSelStr = " selected";
-
-            htmls.push('<option value="' + name + '"' + isSelStr + '>' + label + '</option>');
+            if ((selIdx !== undefined && i === selIdx))
+                isSelStr = " selected"
+            htmls.push('<option value="' + entry[0] + '"' + isSelStr + '>' + entry[1] + '</option>');
         }
         htmls.push('</select>');
     }
 
-    function loadCoordSet(coordIdx, labelFieldName) {
-        /* load coordinates and color by meta data */
-        var newRadius = db.conf.coords[coordIdx].radius;
-        var colorOnMetaField = db.conf.coords[coordIdx].colorOnMeta;
-        renderer.background = null; // remove the background image
-
+    function loadCoordSet(coordIdx) {
         db.loadCoords(coordIdx,
-            function(coords, info, clusterMids) {
-                gotCoords(coords, info, clusterMids, newRadius);
-
-                setLabelField(labelFieldName);
-                setLabelDropdown(labelFieldName);
-
-                if (colorOnMetaField !== undefined) {
-                    setColorByDropdown(colorOnMetaField);
-                    colorByMetaField(colorOnMetaField, undefined);
-                } else
-                    renderer.drawDots();
+            function(a, b, c) {
+                gotCoords(a, b, c);
+                renderer.drawDots();
             },
-            gotSpatial,
             onProgress);
     }
 
     function onLayoutChange(ev, params) {
         /* user changed the layout in the combobox */
         var coordIdx = parseInt(params.selected);
-
-        var labelFieldIdx = parseInt($("#tpLabelCombo").val().split("_")[1]);
-        var labelFieldName = db.getMetaFields()[labelFieldIdx].name;
-
-        loadCoordSet(coordIdx, labelFieldName);
-
+        loadCoordSet(coordIdx);
         changeUrl({
             "layout": coordIdx,
             "zoom": null
         });
-        renderer.coordIdx = coordIdx;
-
         // remove the focus from the combo box
         removeFocus();
     }
 
-    function onGeneComboChange(ev) {
+    function onGeneChange(ev) {
         /* user changed the gene in the combobox */
-        var geneId = ev.target.value;
-        if (geneId === "")
+        var geneSym = ev.target.value;
+        if (geneSym === "")
             return; // do nothing if user just deleted the current gene
-        if (db.conf.atacSearch) {
-            updatePeakListWithGene(geneId);
-        } else {
-            // in the normal, gene-matrix mode.
-            var locusStr = null;
-            var geneInfo = db.getGeneInfo(geneId);
-            colorByLocus(geneInfo.id);
-        }
+        loadGeneAndColor(geneSym);
+        $(this).blur(); // remove focus
     }
 
     function onMetaComboChange(ev, choice) {
         /* called when user changes the meta field combo box */
         //if (choice.selected==="_none")
         var fieldId = parseInt(choice.selected.split("_")[1]);
         var fieldName = db.getMetaFields()[fieldId].name;
         console.log(choice);
         console.log(ev);
 
         colorByMetaField(fieldName);
     }
 
-    function onLabelComboChange(ev, choice) {
-        /* called when user changes the label field combo box */
-        var fieldId = parseInt(choice.selected.split("_")[1]);
-        var fieldName = db.getMetaFields()[fieldId].name;
-        setLabelField(fieldName);
-        renderer.drawDots();
-    }
-
-    function showCollectionDialog(collName) {
-        /* load collection with given name and open dialog box for it */
-        loadCollectionInfo(collName, function(collData) {
-            openDatasetDialog(collData)
-        });
-    }
-
-    function onConfigLoaded(datasetName) {
-        // this is a collection if it does not have any field information
-        if (db.conf.sampleDesc)
-            gSampleDesc = db.conf.sampleDesc;
-        else
-            gSampleDesc = "cell";
-
-        // allow config to override the default palettes
-        datasetGradPalette = cDefGradPalette;
-        datasetQualPalette = cDefQualPalette;
-        if (db.conf.defQuantPal)
-            datasetGradPalette = db.conf.defQuantPal;
-        if (db.conf.defCatPal)
-            datasetQualPalette = db.conf.defCatPal;
-
-        if (db.conf.metaBarWidth)
-            metaBarWidth = db.conf.metaBarWidth;
-        else
-            metaBarWidth = 250;
-
-        renderer.setPos(null, metaBarWidth + metaBarMargin);
-
-        if (!db.conf.metaFields) {
-            // pablo often has single-dataset installations, there is no need to open the
-            // dataset selection box then.
-            if (db.conf.datasets && db.conf.datasets.length === 1 && datasetName === "") // "" is the root dataset
-                loadDataset(db.conf.datasets[0].name, false);
-            else
-                showCollectionDialog(datasetName);
-            return;
-        }
-
-        let binData = localStorage.getItem(db.name + "|custom");
-        if (binData) {
-            let jsonStr = LZString.decompress(binData);
-            let customMeta = JSON.parse(jsonStr);
-            db.conf.metaFields.unshift(customMeta);
-        }
-
-        cartLoad(db);
-        renderData();
-        resizeDivs(true);
-
-        if (getVar("openDialog"))
-            openDatasetDialog(db.conf, db.name); // open Info dialog
-        cartSave(db); // = set the current URL from local storage settings
-
-        // start the tutorial after a while
-        var introShownBefore = localStorage.getItem("introShown");
-        if (introShownBefore === undefined)
-            setTimeout(function() {
-                showIntro(true);
-            }, 3000); // shown after 5 secs
-    }
-
-    function loadDataset(datasetName, resetVars, md5) {
+    function loadDataset(datasetName, resetVars) {
         /* load a dataset and optionally reset all the URL variables.
          * When a dataset is opened through the UI, the variables have to
          * be reset, as their values (gene or meta data) may not exist
          * there. If it's opened via a URL, the variables must stay. */
-
-        // collections are not real datasets, so ask user which one they want
-        if (db !== null && db.heatmap)
-            removeHeatmap();
-        removeSplit();
-
         db = new CbDbFile(datasetName);
-        cellbrowser.db = db; // easier debugging
 
-        var vars;
+        var vars = undefined;
         if (resetVars)
             vars = {};
 
-        if (datasetName !== "")
-            changeUrl({
-                "ds": datasetName.replace(/\//g, " ")
-            }, vars); // + is easier to type than %23
-
-        db.loadConfig(onConfigLoaded, md5);
-        trackEvent("open_dataset", datasetName);
-        trackEventObj("select_content", {
-            content_type: "dataset",
-            item_id: datasetName
+        changeUrl({
+            "ds": datasetName
+        }, vars);
+        db.loadConfig(function() {
+            renderData()
         });
-    }
 
-    function loadCollectionInfo(collName, onDone) {
-        /* load collection info and run onDone */
-        var jsonUrl = cbUtil.joinPaths([collName, "dataset.json"]);
-        cbUtil.loadJson(jsonUrl, onDone);
+        // start the tutorial after a while
+        var introShownBefore = localStorage.getItem("introShown");
+        if (introShownBefore == undefined)
+            setTimeout(function() {
+                showIntro(true);
+            }, 5000); // show after 5 secs
+
     }
 
     function onDatasetChange(ev, params) {
-        /* user changed the dataset in the collection dropdown box */
-        /* jshint validthis: true */
+        /* user changed the dataset in the dropbox */
+        var datasetIdx = parseInt(params.selected);
+        var datasetName = gDatasetList[datasetIdx].name;
         $(this).blur();
         removeFocus();
-
-        var parts = params.selected.split("?");
-        var datasetName = parts[0];
-        var md5 = parts[1];
-        loadDataset(datasetName, true, md5);
+        loadDataset(datasetName, true);
     }
 
-    function buildLayoutCombo(coordLabel, htmls, files, id, width, left, top) {
+    function buildLayoutCombo(htmls, files, id, width, left, top) {
         /* files is a list of elements with a shortLabel attribute. Build combobox for them. */
-        if (!coordLabel)
-            coordLabel = "Layout";
-
-        htmls.push('<div class="tpToolBarItem" style="position:absolute;left:' + left + 'px;top:' + top + 'px"><label for="' + id + '">');
-        htmls.push(coordLabel);
-        htmls.push("</label>");
-
+        htmls.push('<div class="tpToolBarItem" style="position:absolute;left:' + left + 'px;top:' + top + 'px"><label for="' + id + '">Layout</label>');
         var entries = [];
         for (var i = 0; i < files.length; i++) {
             var coordFiles = files[i];
             var label = coordFiles.shortLabel;
             if (label === undefined)
-                warn("Layout coordinate file " + i + " has no .shortLabel attribute");
+                warn("Layout coordinate file " + i + " has no .shortLabel attribute")
             entries.push([i, label]);
         }
         buildComboBox(htmls, id, entries, 0, "Select a layout algorithm...", width);
         htmls.push('</div>');
     }
 
-    function buildCollectionCombo(htmls, id, width, left, top) {
-        /* build combobox with shortLabels of all datasets that are part of same collection */
-        htmls.push('<div class="tpToolBarItem" style="position:absolute;width:' + width + 'px;left:' + left + 'px;top:' + top + 'px"><label for="' + id + '">Jump to...</label>');
-
+    function buildDatasetCombo(htmls, datasets, id, width, left, top) {
+        /* datasets with a list of elements with a shortLabel attribute. Build combobox for them. */
+        htmls.push('<div class="tpToolBarItem" style="position:absolute;width:150px;left:' + left + 'px;top:' + top + 'px"><label for="' + id + '">Dataset</label>');
         var entries = [];
-        //var linkedDatasets = parentConf.datasets;
-        //for (var i = 0; i < linkedDatasets.length; i++) {
-        //var dsInfo = linkedDatasets[i];
-        //entries.push( [i, dsInfo.shortLabel] );
-        //}
-
+        for (var i = 0; i < datasets.length; i++) {
+            var dataset = datasets[i];
+            var label = dataset.shortLabel;
+            if (label === undefined)
+                label = "Dataset " + i;
+            entries.push([i, label]);
+        }
         buildComboBox(htmls, id, entries, 0, "Select a dataset...", width);
         htmls.push('</div>');
     }
 
-    function buildMetaFieldCombo(htmls, idOuter, id, left, selectedField) {
+    function buildMetaFieldCombo(htmls, idOuter, id, left) {
         var metaFieldInfo = db.getMetaFields();
         htmls.push('<div id="' + idOuter + '" style="padding-left:2px; display:inline">');
-        //var entries = [["_none", ""]];
-        var entries = [];
-        var selIdx = 0;
-        for (var i = 1; i < metaFieldInfo.length; i++) { // starts at 1, skip ID field
+        var entries = [
+            ["_none", ""]
+        ];
+        for (var i = 0; i < metaFieldInfo.length; i++) {
             var field = metaFieldInfo[i];
             var fieldName = field.label;
-            // cannot label on something that is a number or has a ton of values
-            var hasTooManyVals = (field.diffValCount > MAXCOLORCOUNT || field.type === "int" || field.type === "float");
+            var hasTooManyVals = (field.diffValCount > 100);
             if (hasTooManyVals)
                 continue;
-
             entries.push(["tpMetaVal_" + i, fieldName]);
-            if (selectedField == fieldName) {
-                selIdx = i;
-            }
         }
 
-        buildComboBox(htmls, id, entries, selIdx, "select a field...", metaBarWidth + 50);
+        buildComboBox(htmls, id, entries, 0, "select a field...", metaBarWidth);
         htmls.push('</div>');
     }
 
-    function getGeneLabel() {
-        /* some datasets have data not on genes, but on other things e.g. "lipids". The config can
-         * define a label for the rows in the expression matrix */
-        var geneLabel = "Gene";
-        if (db.conf.atacSearch)
-            geneLabel = "Range";
-        if (db.conf.geneLabel)
-            geneLabel = db.conf.geneLabel;
-        return geneLabel;
-    }
-
     function buildGeneCombo(htmls, id, left, width) {
-        /* Combobox that allows searching for genes */
+        /* datasets with a list of elements with a shortLabel attribute. Build combobox for them. */
+        //htmls.push('<div class="tpToolBarItem" style="position:absolute;left:'+left+'px;top:'+toolBarComboTop+'px">');
         htmls.push('<div class="tpToolBarItem" style="padding-left: 3px">');
-        var title = "Color by " + getGeneLabel();
-        if (db.conf.atacSearch)
-            title = "Find peaks at or close to:"
-        htmls.push('<label style="display:block; margin-bottom:8px; padding-top: 8px;" for="' + id + '">' + title + '</label>');
-        var geneLabel = getGeneLabel().toLowerCase();
-        var boxLabel = 'search for ' + geneLabel + '...';
-        if (db.conf.atacSearch)
-            boxLabel = "enter gene or chrom:start-end";
-        htmls.push('<select style="width:' + width + 'px" id="' + id + '" placeholder="' + boxLabel + '" class="tpCombo">');
+        htmls.push('<label style="display:block; margin-bottom:8px; padding-top: 8px;" for="' + id + '">Color by Gene</label>');
+        htmls.push('<select style="width:' + width + 'px" id="' + id + '" placeholder="search for gene..." class="tpCombo">');
         htmls.push('</select>');
         htmls.push('</div>');
         //htmls.push("<button>Multi-Gene</button>");
     }
 
 
     function activateCombobox(id, widthPx) {
         $('#' + id).chosen({
             inherit_select_classes: true,
             disable_search_threshold: 10,
             width: widthPx
         });
     }
 
-    function updateCollectionCombo(id, collData) {
-        /* load dataset sibling labels into collection combobox from json */
-        var htmls = [];
-        var datasets = collData.datasets;
-        for (var i = 0; i < datasets.length; i++) {
-            var ds = datasets[i];
-            var selStr = "";
-            if (ds.name === db.conf.name)
-                selStr = "selected";
-            var val = ds["name"] + "?" + ds["md5"];
-            htmls.push('<option value="' + val + '"' + selStr + '>' + ds.shortLabel + '</option>');
-        }
-        $('#' + id).html(htmls.join(""));
-        $("#" + id).trigger("chosen:updated");
-    }
-
-    /* ----- PEAK LIST START ----- */
-
-    function buildPeakList(htmls) {
-        /* add a container for the list of peaks to htmls */
-        htmls.push("<div id='tpPeakListTitle'>Peaks found</div>");
-
-        htmls.push("<div id='tpPeakList' style='height: 30%'>");
-        htmls.push("<span id='noPeaks'>No genes or ranges found</span>");
-        htmls.push("</div>");
-        htmls.push("<div id='tpPeakListSelector'>");
-        //htmls.push("<input id='tpPeakListAuto' style='margin-right: 3px' type='checkbox' checked>");
-        htmls.push("<div id='tpPeakListButtons' style='margin-left: 4px'>");
-        htmls.push('<button title="Select all peaks in the list above" id="tpPeakListAll">All</button>');
-        htmls.push('<button title="Select no peaks in the list above" id="tpPeakListNone">None</button>');
-        htmls.push('<button title="Select only peaks within a certain distance upstream from the TSS. Click on the field to edit the distance. Click the button to select the peaks." id="tpPeakListUpstream">');
-        htmls.push('<input id="tpPeakListAutoDist" type="text" value="2" style="width:2em;border: 0;height: 0.8em;">');
-        htmls.push('kbp upstream</button>');
-        htmls.push("<div id='tpPeakListButtons'>");
-
-        //htmls.push("<label for='tpPeakListAuto' style='display:inline; font-weight:normal'>Peaks ");
-        //htmls.push("<input id='tpPeakListAutoDist' style='width:2em; height:1.3em; margin-right: 0.3em' type='text' value='2'>");
-        //htmls.push("kbp upstream</input>");
-        //htmls.push("<button id='tpPeakListUpstream' style='float:right; margin-top: 2px'>Select</button>");
-        //htmls.push("</label>");
-        htmls.push("</div>");
-    }
-
-    function peakListShowTitle(sym, chrom, start, end) {
-        /* update the peak list box title */
-        var el = getById("tpPeakListTitle");
-        if (sym)
-            el.innerHTML = "<b>" + sym + "</b>, TSS at <span id='tpTss'>" + chrom + ":" + start + "</span>";
-        else
-            el.innerHTML = "Peaks at <b>" + chrom + ":" + prettySeqDist(start) + "-" + prettySeqDist(end) + "</b>";
-    }
-
-    function peakListSetStatus(str) {
-        /* given a string like "chr1|1000|2000+chr2|3000|4000" set the corresponding checkboxes */
-        if (!db.conf.atacSearch)
-            return;
-        let activePeaks = str.split("+");
-        let inEls = document.querySelectorAll(".tpPeak > input");
-        for (let el of inEls) {
-            let parts = el.id.split(":");
-            let peakId = parts[1] + "|" + parts[2] + "|" + parts[3];
-            el.checked = (activeRanges.includes(peakId));
-        }
-    }
-
-    function peakListGetPeaksWith(status) {
-        /* return array of objects , e.g. [ {chrom:"chr1", start:1000, end:2000, dist:-70000, el:<domObject>} ]
-         * status can be "on" or "off" = will only return ranges that are checked or unchecked.
-         * */
-        let ranges = [];
-        let inEls = document.querySelectorAll(".tpPeak > input");
-        for (let el of inEls) {
-            if (status === "on" && !el.checked)
-                continue;
-            else if (status === "off" && el.checked)
-                continue;
-            let parts = el.id.split(":");
-            ranges.push({
-                "chrom": parts[1],
-                start: parseInt(parts[2]),
-                end: parseInt(parts[3]),
-                dist: parseInt(parts[4]),
-                el: el,
-                locusName: parts[1] + "|" + parts[2] + "|" + parts[3]
-            });
-        }
-        return ranges;
-    }
-
-    function peakListSerialize() {
-        /* return a summary of all currently selected peaks, e.g. "chr1|1000|2000+chr2|3000|4000" */
-        let ranges = [];
-        for (let r of peakListGetPeaksWith("on")) {
-            let locusId = r.chrom + "|" + r.start + "|" + r.end;
-            ranges.push(locusId);
-        }
-        return ranges.join("+");
-    }
-
-    function onPeakChange(ev) {
-        /* user checks or unchecks a peak */
-        let el = ev.currentTarget.firstChild; // user may have clicked the label
-        var isChecked = el.checked;
-        var peakInfos = el.id.split(":");
-        let chrom = peakInfos[1];
-        let start = peakInfos[2];
-        let end = peakInfos[3];
-        let prefix = "+";
-        if (!isChecked)
-            prefix = "-";
-        let rangeStr = prefix + chrom + "|" + start + "|" + end;
-        colorByLocus(rangeStr);
-    }
-
-    function peakListShowRanges(chrom, foundRanges, searchStart) {
-        /* load a list of ranges (arrays of [start, end] into the peak list box */
-        var htmls = [];
-        var i = 0;
-        if (foundRanges.length === 0) {
-            htmls.push("No peaks around this gene");
-        } else
-            for (let rangeInfo of foundRanges) {
-                let foundStart = rangeInfo[0];
-                let foundEnd = rangeInfo[1];
-                //let label = chrom+":"+foundStart+"-"+foundEnd;
-                let dist = foundStart - searchStart;
-                let label = prettySeqDist(dist, true);
-                let regLen = foundEnd - foundStart;
-                if (regLen !== 0)
-                    label += ", " + (foundEnd - foundStart) + " bp long";
-                let checkBoxId = "range:" + chrom + ":" + foundStart + ":" + foundEnd + ":" + dist;
-                htmls.push("<div class='tpPeak'>");
-                htmls.push("<input style='margin-right: 4px' id='" + checkBoxId + "' type='checkbox'>");
-                htmls.push("<label for='" + checkBoxId + "'>" + label + "</label>");
-                htmls.push("</div>");
-                i++;
-            }
-        var divEl = document.getElementById("tpPeakList");
-        divEl.innerHTML = htmls.join(""); // set the DIV
-        classAddListener("tpPeak", "input", onPeakChange);
-    }
-
-    function onPeakAll(ev) {
-        /* select all peaks */
-        let peaks = peakListGetPeaksWith("off");
-        let peakNames = [];
-        if (peaks.length > 100) {
-            alert("More than 100 peaks to select. This will take too long. Please contact us if you need this feature.");
-            return;
-        }
-        for (let p of peaks) {
-            peakNames.push(p.locusName);
-            p.el.checked = true;
-        }
-        if (peakNames.length === 0)
-            return;
-
-        let locusStr = "+" + peakNames.join("+");
-        colorByLocus(locusStr);
-    }
-
-    function onPeakNone(ev) {
-        /* unselect all peaks */
-        let peaks = peakListGetPeaksWith("on");
-        let peakNames = [];
-        for (let p of peaks) {
-            peakNames.push(p.locusName);
-            p.el.checked = false;
-        }
-        if (peakNames.length === 0)
-            return;
-        let locusStr = "-" + peakNames.join("-");
-        colorByLocus(locusStr);
-    }
-
-    function onPeakUpstream(ev) {
-        /* select all peaks that are closer than the distance in #tpPeakListAutoDist */
-        if (ev.target.id === "tpPeakListAutoDist")
-            // user actually clicked the input box = do nothing
-            return;
-        let maxDistStr = document.getElementById("tpPeakListAutoDist").value;
-        let maxDist = parseInt(maxDistStr);
-        if (isNaN(maxDist)) {
-            alert(maxDistStr + " is not a number");
-            return;
-        }
-        if (maxDist > 2000) {
-            alert("The distance filter is too high: " + maxDistStr + ". It cannot be larger than 2000, = 2Mbp. If you think this is too restrictive, please contact us.");
-            return;
-        }
-        maxDist = -1 * maxDist * 1000; // needs to be negative
-
-        let addPeaks = [];
-        let peaks = peakListGetPeaksWith("off");
-        for (let p of peaks) {
-            let dist = p.dist;
-            if (dist < 0 && dist > maxDist) {
-                addPeaks.push(p.chrom + "|" + p.start + "|" + p.end);
-                p.el.checked = true;
-            }
-        }
-
-        if (addPeaks.length === 0) {
-            alert("Either there is no active gene search or TSS or no peaks are at " + maxDist + " bp relative to the TSS");
-            return;
-        }
-
-        let loadStr = addPeaks.join("+")
-
-        colorByLocus(loadStr);
-        ev.stopPropagation();
-    }
-
-    /* ----- PEAK LIST END ----- */
-
-    function selectizeSendGenes(arr, callback) {
-        /* given an array of strings s, return an array of objects with id=s and call callback with it.*/
-        let foundArr = [];
-        for (let o of arr) {
-            var text = o.sym;
-            if (o.sym !== o.id)
-                text = o.sym + " (" + o.id + ")";
-            foundArr.push({
-                "id": o.id,
-                "text": text
-            });
-        }
-        callback(foundArr);
-    }
-
-    function comboLoadGene(query, callback) {
-        /* The load() function for selectize for genes.
-         * called when the user types something into the gene box, returns matching gene symbols */
-        if (!query.length)
-            return callback();
-        this.clearOptions();
-        var genes = db.findGenes(query);
-        selectizeSendGenes(genes, callback);
-    }
-
-    function updatePeakListWithGene(geneId) {
-        /* update the peak list box with all peaks close to a gene's TSS */
-        var peaksInView = db.findRangesByGene(geneId);
-        var gene = db.getGeneInfoAtac(geneId);
-        peakListShowTitle(gene.sym, gene.chrom, gene.chromStart);
-        peakListShowRanges(gene.chrom, peaksInView.ranges, gene.chromStart);
-    }
-
-    function comboLoadAtac(query, callback) {
-        /* The load() function for selectize for ATAC datasets.
-         * called when the user types something into the gene box, calls callback with matching gene symbols or peaks
-         * or shows the peaks in the peakList box */
+    function geneComboSearch(query, callback) {
+        /* called when the user types something into the gene box, returns matching gene symbols */
         if (!query.length)
             return callback();
 
-        this.clearOptions();
-        this.renderCache = {};
-
-        var range = cbUtil.parseRange(query);
-        if (range === null) {
-            if (!db.geneToTss || db.geneToTss === undefined)
-                db.indexGenesAtac();
-
-            var geneInfos = db.findGenesAtac(query);
-
-            if (geneInfos.length === 0)
-                return;
-
-            if (geneInfos.length > 1)
-                selectizeSendGenes(geneInfos, callback);
-            else {
-                var geneId = geneInfos[0].id;
-                updatePeakListWithGene(geneId);
-            }
-        } else {
-            // user entered a range e.g. chr1:0-190k or chr1:1m-2m
-            let searchStart = range.start;
-            let searchEnd = range.end;
-            peakListShowTitle(null, range.chrom, range.start, range.end);
-            let foundRanges = db.findOffsetsWithinPos(range.chrom, searchStart, searchEnd);
-            peakListShowRanges(range.chrom, foundRanges, searchStart);
-        }
-    }
+        //var geneList = [];
 
-    function comboRender(item, escape) {
-        if (item.dist)
-            return '<div style="display:block">' + escape(item.text) + '<div style="text-color: darkgrey; font-size:80%;float:right">+' + prettyNumber(item.dist, "bp") + '</div>';
-        else
-            return '<div>' + escape(item.text) + '</div>';
+        //for (var geneSym in db.getGenes()) {
+        //if (geneSym.toLowerCase().startsWith(query.toLowerCase()))
+        //geneList.push({"id":geneSym, "text":geneSym});
+        //}
+        db.searchGenes(query.toLowerCase(), callback);
     }
 
     function arrayBufferToString(buf, callback) {
         /* https://stackoverflow.com/questions/8936984/uint8array-to-string-in-javascript */
         var bb = new Blob([new Uint8Array(buf)]);
         var f = new FileReader();
         f.onload = function(e) {
             callback(e.target.result);
         };
         f.readAsText(bb);
     }
 
 
-    function makeXenaUrl(metaFieldName, geneSyms, geneSym, actMeta) {
-        /* return URL to Xena view with this dataset and geneSyms loaded */
-        var xenaId = db.conf.xenaId;
-        var phenoId = db.conf.xenaPhenoId;
-        var browser = 'https://singlecell.xenabrowser.net/';
-        var view = [{
-            name: phenoId,
-            host: 'https://singlecellnew.xenahubs.net',
-            fields: metaFieldName,
-            columnLabel: 'Cell Annotations',
-            fieldLabel: metaFieldName
-        }];
-
-        if (geneSyms.length !== 0)
-            view.push({
-                name: xenaId,
-                host: 'https://singlecellnew.xenahubs.net',
-                fields: geneSyms.join(" "),
-                width: 15 * geneSyms.length,
-                columnLabel: 'Dataset genes',
-                fieldLabel: geneSyms.join(" ")
-            });
-
-        if (actMeta)
-            view.push({
-                name: phenoId,
-                host: 'https://singlecellnew.xenahubs.net',
-                fields: actMeta,
-                width: 120,
-                columnLabel: 'Current Meta',
-                fieldLabel: actMeta
-            });
-
-        if (geneSym)
-            view.push({
-                name: xenaId,
-                host: 'https://singlecellnew.xenahubs.net',
-                fields: geneSym,
-                width: 120,
-                columnLabel: 'Current Gene',
-                fieldLabel: geneSym
-            });
-
-        var heatmap = {
-            "showWelcome": false
-        };
-
-        var url = browser + 'heatmap/?columns=' +
-            encodeURIComponent(JSON.stringify(view)) +
-            '&heatmap=' + encodeURIComponent(JSON.stringify(heatmap));
-        return url;
-    }
-
     function makeHubUrl(geneSym) {
         /* return URL of the hub.txt file, possibly jumping to a given gene  */
         var hubUrl = db.conf.hubUrl;
-
-        if (hubUrl === undefined)
+        if (hubUrl == undefined)
             return null;
-
-        // we accept full session links in the hubUrl statement and just pass these through
-        if (hubUrl && hubUrl.indexOf("genome.ucsc.edu/s/") !== -1)
-            return hubUrl;
-
         var ucscDb = db.conf.ucscDb;
         if (ucscDb === undefined) {
             alert("Internal error: ucscDb is not defined in cellbrowser.conf. Example values: hg19, hg38, mm10, etc. You have to set this variable to make track hubs work.");
             return "";
         }
+        var fullUrl = "https://genome.ucsc.edu/cgi-bin/hgTracks?hubUrl=" + hubUrl + "&genome=" + ucscDb;
 
-        var fullUrl = null;
-        if (hubUrl.indexOf("/") === -1) {
-            // no slash -> it's not a URL at all but just a track name (e.g. "tabulamuris")
-            var trackName = hubUrl;
-            fullUrl = "https://genome.ucsc.edu/cgi-bin/hgTracks?" + trackName + "=full&genome=" + ucscDb;
-        } else {
-            // it's a url to a hub.txt file: either relative or absolute
-            if (!hubUrl.startsWith("http")) {
-                // relative URL to a hub.txt file -> make absolute now
-                //hubUrl = getBaseUrl()+db.name+"/"+hubUrl
-                hubUrl = cbUtil.absPath("", cbUtil.joinPaths([getBaseUrl(), db.name, hubUrl]));
-            }
-            // URL is an absolute link to a hub.txt URL
-            fullUrl = "https://genome.ucsc.edu/cgi-bin/hgTracks?hubUrl=" + hubUrl + "&genome=" + ucscDb;
-        }
-
-        if (geneSym && !geneSym.startsWith("atac-"))
+        if (geneSym !== undefined)
             fullUrl += "&position=" + geneSym + "&singleSearch=knownCanonical";
 
         return fullUrl;
     }
 
-    function onGenomeButtonClick(ev) {
-        /* run when the user clicks the 'genome browser' button */
-        let actSym = null;
-        if (gLegend.type === "expr")
-            actSym = gLegend.geneSym;
-        var fullUrl = makeHubUrl(actSym);
-        db.gbWin = window.open(fullUrl, 'gbTab');
-        return false;
-    }
-
-    function onXenaButtonClick(ev) {
-        /* run when the user clicks the xena button */
-        var geneInfos = db.conf.quickGenes;
-        var syms = []
-        if (geneInfos != undefined) {
-            for (var i = 0; i < geneInfos.length; i++)
-                syms.push(geneInfos[i][0]); // make array of symbols
-        }
-
-        var actSym = null;
-        var actMeta = null;
-        if (gLegend.type === "expr")
-            actSym = gLegend.geneSym;
-        else
-            actMeta = gLegend.metaInfo.label;
-
-        if (syms.length === 0 && actSym === null) {
-            alert("Sorry, the view is not colored by a gene and there are no 'Dataset genes' " +
-                " defined, so there are no genes active " +
-                "that could be shown on the heatmap. Please color by a gene first, " +
-                "then click the button again.");
-            return;
-        }
-
-        var fullUrl = makeXenaUrl(db.conf.labelField, syms, actSym, actMeta);
-        //if (!db.xenaWin)
-        db.xenaWin = window.open(fullUrl, 'xenaTab');
-        //else
-        //db.xenaWin.location.href = fullUrl;
-        return false;
-    }
-
-    function openCurrentDataset() {
-        /* open dataset dialog with current dataset highlighted */
-        $(this).blur(); // remove focus = tooltip disappears
-        var parentNames = db.name.split("/");
-        parentNames.pop();
-        var newPath = cbUtil.joinPaths([parentNames.join("/"), "dataset.json"]);
-        cbUtil.loadJson(newPath, function(parentConf) {
-            openDatasetDialog(parentConf, db.name);
-        });
-    }
-
-    function buildToolBar(coordInfo, dataset, fromLeft, fromTop) {
+    function buildToolBar(coordInfo, datasetName, fromLeft, fromTop) {
         /* add the tool bar with icons of tools and add under body to the DOM */
         $("#tpToolBar").remove();
 
         var htmls = [];
-
         htmls.push("<div id='tpToolBar' style='position:absolute;left:" + fromLeft + "px;top:" + fromTop + "px'>");
-        htmls.push('<button title="More info about this dataset: abstract, methods, data download, etc." id="tpButtonInfo" type="button" class="ui-button tpIconButton" data-placement="bottom">Info &amp; Download</button>');
+        //htmls.push('<div id="tpIcons" style="display:inline-block">');
+        //htmls.push('<div class="btn-group" role="group" style="vertical-align:top">');
+        //htmls.push('<button data-placement="bottom" data-toggle="tooltip" title="Zoom-to-rectangle mode.<br>Keyboard: Windows/Command or z" id="tpIconModeZoom" class="ui-button tpIconButton" style="margin-right:0"><img src="img/zoom.png"></button>');
+        //htmls.push('<button data-placement="bottom" title="Move mode. Keyboard: Alt or m" id="tpIconModeMove" data-toggle="tooltip" class="ui-button tpIconButton" style="margin-right:0"><img src="img/move.png"></button>');
+        //htmls.push('<button data-placement="bottom" title="Select mode.<br>Keyboard: shift or s" id="tpIconModeSelect" class="ui-button tpIconButton" style="margin-right:0"><img src="img/select.png"></button>');
+        //htmls.push('</div>');
+
+        //htmls.push('&emsp;');
+        //htmls.push('<button title="Zoom in" id="tpIconZoomIn" type="button" class="btn-small btn-outline-primary noPad"><i class="material-icons">zoom_in</i></button>');
+        //htmls.push('<button title="Zoom out" id="tpIconZoomOut" type="button" class="btn-small btn-outline-primary noPad"><i class="material-icons">zoom_out</i></button>');
+        //htmls.push('<button title="Zoom to 100%, showing all data, keyboard: space" data-placement="bottom" data-toggle="tooltip" id="tpZoom100Button" class="ui-button tpIconButton" style="margin-right:0"><img src="img/center.png"></button>');
+
+        //htmls.push("&emsp;");
+
+        //htmls.push('<div class="btn-group" role="group" style="vertical-align:top">');
+        //htmls.push('<button title="More info about this dataset" id="tpIconDatasetInfo" type="button" class="ui-button tpIconButton"><img title="More info about this dataset" src="img/info.png"></button>');
+        //htmls.push('</div>');
+        //htmls.push('<img class="tpIconButton" id="tpIconDatasetInfo" data-placement="bottom" data-toggle="tooltip" title="More info about this dataset" src="img/info.png" style="height:18px;position:absolute;top:4px; left:'+(toolBarComboLeft+datasetComboWidth+60)+'px">');
+
+        //htmls.push("&emsp;");
+        var layoutLeft = 150;
+        if (db.conf.hubUrl !== undefined)
+            layoutLeft = 290;
+        buildLayoutCombo(htmls, coordInfo, "tpLayoutCombo", 300, layoutLeft, 2);
+        //buildDatasetCombo(htmls, gDatasetList, "tpDatasetCombo", 100, 220, 0);
 
-        if (!getVar("suppressOpenButton", false))
-            htmls.push('<button id="tpOpenDatasetButton" class="gradientBackground ui-button ui-widget ui-corner-all" style="margin-top:3px; height: 24px; border-radius:3px; padding-top:3px" title="Open another dataset" data-placement="bottom">Open...</button>');
+        htmls.push('<button id="tpOpenDatasetButton" class="gradientBackground ui-button ui-widget ui-corner-all" style="margin-top:3px; height: 24px; border-radius:3px; padding-top:3px">Open Dataset...</button>');
 
-        var nextLeft = 220;
-        if (db.conf.hubUrl !== undefined) {
-            htmls.push('<a target=_blank href="#" id="tpOpenGenome" class="gradientBackground ui-button ui-widget ui-corner-all" style="margin-left: 10px; margin-top:3px; height: 24px; border-radius:3px; padding-top:3px" title="Show sequencing read coverage and gene expression on UCSC Genome Browser" data-placement="bottom">Genome Browser</a>');
-            nextLeft += 155;
-        }
-
-        var xenaId = db.conf.xenaId;
-        if (xenaId !== undefined) {
-            htmls.push('<a target=_blank href="#" id="tpOpenXena" class="gradientBackground ui-button ui-widget ui-corner-all" style="margin-left: 10px; margin-top:3px; height: 24px; border-radius:3px; padding-top:3px" title="Show gene expression heatmap on UCSC Xena Browser, creates heatmap of current gene (if coloring by gene) and all dataset genes. Click this button also if you have an active Xena window open and want to update the view there." data-placement="bottom">Xena</a>');
-            nextLeft += 80;
-        }
-
-        if (coordInfo[coordInfo.length - 1].shortLabel.length > 20)
-            //$('.chosen-drop').css({"width": "300px"});
-            layoutComboWidth += 50
-        buildLayoutCombo(dataset.coordLabel, htmls, coordInfo, "tpLayoutCombo", layoutComboWidth, nextLeft, 2);
-        nextLeft += 65 + layoutComboWidth;
-
-        var nameParts = dataset.name.split("/");
-        var parentName = null;
-        if (nameParts.length > 1) {
-            buildCollectionCombo(htmls, "tpCollectionCombo", 330, nextLeft, 0);
-            nameParts.pop();
-            parentName = nameParts.join("/");
+        var hubUrl = db.conf.hubUrl;
+        if (hubUrl !== undefined) {
+            var fullUrl = makeHubUrl();
+            htmls.push('<a target=_blank href="' + fullUrl + '" id="tpOpenUcsc" class="gradientBackground ui-button ui-widget ui-corner-all" style="margin-left: 10px; margin-top:3px; height: 24px; border-radius:3px; padding-top:3px">Genome Browser</a>');
         }
 
         htmls.push("</div>");
 
         $(document.body).append(htmls.join(""));
 
-        $('#tpOpenXena').click(onXenaButtonClick);
-        $('#tpOpenGenome').click(onGenomeButtonClick);
+        //var el = document.getElementById('tpOpenUcsc');
+        //el.addEventListener("click"
 
         activateTooltip('.tpIconButton');
-        activateTooltip('#tpOpenUcsc');
-        activateTooltip('#tpOpenDatasetButton');
 
-        $('#tpButtonInfo').click(function() {
-            openDatasetDialog(db.conf, db.name)
+        //$('#tpIconModeMove').click( function() { activateMode("move")} );
+        //$('#tpIconModeZoom').click( function() { activateMode("zoom")} );
+        //$('#tpIconModeSelect').click( function() { activateMode("select")} );
+        //$('#tpZoom100Button').click( onZoom100Click );
+        $('#tpIconDatasetInfo').click(function() {
+            openDatasetDialog()
         });
 
-        activateCombobox("tpLayoutCombo", layoutComboWidth);
-
-        if (parentName !== null) {
-            activateCombobox("tpCollectionCombo", collectionComboWidth);
-            loadCollectionInfo(parentName, function(dataset) {
-                updateCollectionCombo("tpCollectionCombo", dataset);
-            });
-        }
-
-        // selective gene or ATAC Color by search box
-        var comboLoad = comboLoadGene;
-        if (db.conf.atacSearch) {
-            comboLoad = comboLoadAtac;
-            getById("tpPeakListUpstream").addEventListener("click", onPeakUpstream);
-            getById("tpPeakListAll").addEventListener("click", onPeakAll);
-            getById("tpPeakListNone").addEventListener("click", onPeakNone);
-            activateTooltip("#tpPeakListButtons > button");
+        //$('#tpIconZoomIn').click( onZoomInClick );
+        //$('#tpIconZoomOut').click( onZoomOutClick );
+        //$('#tpIconZoom100').click( onZoom100Click );
 
-        }
-
-        // This is a hack to deactivate the "sifter" functionality of selectize.
-        // It turns out that selectize is a very bad dropdown choice for us,
-        // as it makes a strong assumption that matching is done on a keyword basis
-        // which is not true for chrom ranges.
-        // https://gist.github.com/rhyzx/2281e8d1662b7be21716
-        Selectize.prototype.search = function(query) {
-            return {
-                query: query,
-                tokens: [], // disable highlight
-                items: $.map(this.options, function(item, key) {
-                    return {
-                        id: key
-                    }
-                })
-            }
-        };
+        activateCombobox("tpDatasetCombo", datasetComboWidth);
+        activateCombobox("tpLayoutCombo", layoutComboWidth);
 
-        var select = $('#tpGeneCombo').selectize({
-            maxItems: 1,
-            valueField: 'id',
+        //$('#tpGeneCombo').select2({ placeholder : "Gene Symbol"}); // preliminary setup, real setup will be in updateToolbar()
+        $('#tpGeneCombo').selectize({
             labelField: 'text',
+            valueField: 'id',
             searchField: 'text',
-            closeAfterSelect: true,
-            load: comboLoad,
-            render: {
-                option: comboRender
-            }
+            load: geneComboSearch
         });
 
-        select.on("change", onGeneComboChange);
-
-        $('#tpCollectionCombo').change(onDatasetChange);
+        $('#tpDatasetCombo').change(onDatasetChange);
         // update the combobox, select the right dataset
+        var datasetIdx = cbUtil.findIdxWhereEq(gDatasetList, "name", datasetName);
+        $("#tpDatasetCombo").val(datasetIdx).trigger("chosen:updated");
         $('#tpLayoutCombo').change(onLayoutChange);
-        $('#tpOpenDatasetButton').click(openCurrentDataset);
+        $('#tpGeneCombo').change(onGeneChange);
+        $('#tpOpenDatasetButton').click(openDatasetDialog);
     }
 
     function metaFieldToLabel(fieldName) {
         /* convert the internal meta field string to the label shown in the UI. Fix underscores, _id, etc */
         if (fieldName === "_id")
             fieldName = capitalize(gSampleDesc) + " identifier";
         else
             fieldName = fieldName.replace(/_/g, " ");
         return fieldName;
     }
 
     function buildMetaPanel(htmls) {
-        /* add html strings for the meta panel to the left side bar */
-        var metaFields = db.conf.metaFields;
-        for (var i = 0; i < metaFields.length; i++) {
-            var metaInfo = metaFields[i];
-            var fieldLabel = metaInfo.label;
-            fieldLabel = fieldLabel.replace(/_/g, " ");
-            var fieldMouseOver = metaInfo.desc;
+        var metaFieldInfo = db.conf.metaFields;
+        htmls.push("<div id='tpMetaPanel'>");
+        for (var i = 0; i < metaFieldInfo.length; i++) {
+            var field = metaFieldInfo[i];
+            var fieldName = field.label;
 
             // fields without binning and with too many unique values are greyed out
-            var isGrey = (metaInfo === "enum" && metaInfo.diffValCount > MAXCOLORCOUNT && metaInfo.binMethod === undefined);
+            var isGrey = (field.diffValCount > 100 && field.binMethod !== undefined);
 
             var addClass = "";
             var addTitle = "";
-            htmls.push("<div class='tpMetaBox' data-field-name='" + metaInfo.name + "' id='tpMetaBox_" + i + "'>");
+            htmls.push("<div class='tpMetaBox' id='tpMetaBox_" + i + "'>");
             if (isGrey) {
                 addClass = " tpMetaLabelGrey";
                 addTitle = " title='This field contains too many different values. You cannot click it to color on it.'";
             }
-
-            let divId = "tpMetaLabel_" + i;
-
-            htmls.push("<div id='" + divId + "' class='tpMetaLabel" + addClass + "'" + addTitle + ">" + fieldLabel);
-            if (fieldMouseOver)
-                htmls.push('<i title="' + fieldMouseOver + '" ' +
-                    ' class="material-icons tpMetaLabelHelp" style="float:right;font-size:16px">help_outline</i>');
-            htmls.push("</div>");
+            htmls.push("<div id='tpMetaLabel_" + i + "' class='tpMetaLabel" + addClass + "'" + addTitle + ">" + fieldName + "</div>");
 
             var styleAdd = "";
-            if (metaInfo.opt !== undefined) {
-                var opt = metaInfo.opt;
+            if (field.opt !== undefined) {
+                var opt = field.opt;
                 if (opt.fontSize !== undefined)
-                    styleAdd = ";font-size:" + metaInfo.opt.fontSize;
+                    styleAdd = ";font-size:" + field.opt.fontSize;
             }
 
-            htmls.push("<div class='tpMetaValue' style='width:" + (metaBarWidth - 2 * metaBarMargin) + "px" + styleAdd +
-                "' data-field-name='" + metaInfo.name + "' id='tpMeta_" + i + "'>&nbsp;</div>");
+            htmls.push("<div class='tpMetaValue' style='width:" + (metaBarWidth - 2 * metaBarMargin) + "px" + styleAdd + "' id='tpMeta_" + i + "'>&nbsp;</div>");
             htmls.push("</div>"); // tpMetaBox
         }
         htmls.push("<div style='background-color:white; float:right' id='tpMetaNote' style='display:none; height:1em'></div>");
-    }
-
-    function rebuildMetaPanel() {
-        $("#tpMetaPanel").empty();
-        let htmls = [];
-        buildMetaPanel(htmls);
-        $("#tpMetaPanel").html(htmls.join(""));
-        connectMetaPanel();
-    }
-
-    function connectMetaPanel() {
-        activateTooltip(".tpMetaLabelHelp");
-        $(".tpMetaLabel").click(onMetaClick);
-        $(".tpMetaValue").click(onMetaClick);
-        $(".tpMetaValue").mouseover(onMetaMouseOver);
-        $(".tpMetaValue").mouseleave(function() {
-            $('#tpMetaTip').hide();
-            $('.tpMetaBox').removeClass("tpMetaHover");
-            $('.tpMetaBox .tpMetaValue').removeClass("tpMetaHover");
-        });
-
-        // setup the right-click menu
-        //var menuItems = [{name: "Use as cluster label"},{name: "Copy field value to clipboard"}];
-        var menuItems = [{
-            name: "Copy field value to clipboard"
-        }];
-        var menuOpt = {
-            selector: ".tpMetaBox",
-            items: menuItems,
-            className: 'contextmenu-customwidth',
-            callback: onMetaRightClick
-        };
-        $.contextMenu(menuOpt);
-
-        var menuItemsCust = [{
-            name: "Copy field value to clipboard"
-        }, {
-            name: "Remove custom annotations"
-        }];
-        var menuOptCust = {
-            selector: "#tpMetaBox_custom",
-            items: menuItemsCust,
-            className: 'contextmenu-customwidth',
-            callback: onMetaRightClick
-        };
-        $.contextMenu(menuOptCust);
-        // setup the tooltips
-        //$('[title!=""]').tooltip();
+        htmls.push("</div>"); // tpMetaPanel
     }
 
     function buildLeftSidebar() {
         /* add the left sidebar with the meta data fields. db.loadConf
          * must have completed before this can be run, we need the meta field info. */
         $("#tpLeftSidebar").remove();
         // setup the tabs
         var tabsWidth = metaBarWidth;
 
         var htmls = [];
-        htmls.push("<div id='tpMetaTip' style='display:none'></div>");
         htmls.push("<div id='tpLeftSidebar' style='position:absolute;left:0px;top:" + menuBarHeight + "px;width:" + metaBarWidth + "px'>");
 
-        //htmls.push("<div class='tpSidebarHeader'>Color By</div>");
+        htmls.push("<div class='tpSidebarHeader'>Color Control</div>");
 
         // a bar with the tabs
         htmls.push("<div id='tpLeftTabs'>");
         htmls.push("<ul>");
-        htmls.push("<li><a href='#tpAnnotTab'>Annotation</a></li>");
-        htmls.push("<li><a href='#tpGeneTab'>" + getGeneLabel() + "</a></li>");
-        //htmls.push("<li><a href='#tpLayoutTab'>Layout</a></li>");
+        htmls.push("<li><a href='#tpAnnotTab'>Cell Annotations</a></li>");
+        htmls.push("<li><a href='#tpGeneTab'>Genes</a></li>");
         htmls.push("</ul>");
 
         htmls.push("<div id='tpAnnotTab'>");
-
         htmls.push('<label style="padding-left: 2px; margin-bottom:8px; padding-top:8px" for="' + "tpMetaCombo" + '">Color by Annotation</label>');
         buildMetaFieldCombo(htmls, "tpMetaComboBox", "tpMetaCombo", 0);
-        htmls.push('<label style="padding-left: 2px; margin-bottom:8px; padding-top:8px" for="tpLabelCombo">Label by non-num. Annotation</label>');
-        buildMetaFieldCombo(htmls, "tpLabelComboBox", "tpLabelCombo", 0, db.conf.labelField);
-
-        htmls.push('<div style="padding-top:4px; padding-bottom: 4px; padding-left:2px" id="tpHoverHint" class="tpHint">Hover over a ' + gSampleDesc + ' to update data below</div>');
-        htmls.push('<div style="padding-top:4px; padding-bottom: 4px; padding-left:2px; display: none" id="tpSelectHint" class="tpHint">Cells selected. No update on hover.</div>');
-
-        htmls.push("<div id='tpMetaPanel'>");
+        htmls.push('<div style="padding-top:4px; padding-bottom: 4px; padding-left:2px" class="tpHint">Hover over a ' + gSampleDesc + ' to show it below</div>');
         buildMetaPanel(htmls);
-        htmls.push("</div>"); // tpMetaPanel
 
         htmls.push("</div>"); // tpAnnotTab
 
         htmls.push("<div id='tpGeneTab'>");
 
         buildGeneCombo(htmls, "tpGeneCombo", 0, metaBarWidth - 10);
-
-        if (db.conf.multiModal && db.conf.multiModal.splitPrefix)
-            htmls.push('<input type="checkbox" id="splitJoinBox" name="splitJoin" value="splitJoin" /> <label for="subscribeNews">Show on both screens</label>');
-        // var myGenes = loadMyGenes();
-
-        if (db.conf.atacSearch)
-            buildPeakList(htmls);
-
-        var geneLabel = getGeneLabel();
-        var recentHelp = "Shown below are the 10 most recently searched genes. Click any gene to color the plot on the right-hand side by the gene.";
-
-        buildGeneTable(htmls, "tpRecentGenes", "Recent " + geneLabel + "s",
-            "Hover or select cells to update colors here<br>Click to color by gene", gRecentGenes, null, recentHelp);
-
-
-        var noteStr = "No genes or peaks defined. Use the setting quickGenesFile in "
-        "cellbrowser.conf to add a file with gene symbols or peaks that will be shown here";
-        var geneHelp = "The dataset genes were defined by the dataset submitter, publication author or data wrangler at UCSC. " +
-            "Click any of them to color the plot on the right hand side by the gene.";
-        buildGeneTable(htmls, "tpGenes", "Dataset " + geneLabel + "s", null, db.conf.quickGenes, noteStr, geneHelp);
+        buildGeneTable(htmls, metaBarWidth, 66, db.conf.quickGenes);
 
         htmls.push("</div>"); // tpGeneTab
 
-        //htmls.push("<div id='tpLayoutTab'>");
-        //buildLayoutCombo(dataset.coordLabel, htmls, coordInfo, "tpLayoutCombo", layoutComboWidth, nextLeft, 2);
-        //htmls.push("</div>");
-
         htmls.push("</div>"); // tpLeftSidebar
 
         $(document.body).append(htmls.join(""));
 
-        activateTooltip('.hasTooltip');
-
-        resizeGeneTableDivs("tpRecentGenes");
-        resizeGeneTableDivs("tpGenes");
-
         $("#tpLeftTabs").tabs();
         $('#tpLeftTabs').tabs("option", "active", 0); // open the first tab
 
         $('.tpGeneBarCell').click(onGeneClick);
         $('#tpChangeGenes').click(onChangeGenesClick);
 
         activateCombobox("tpMetaCombo", metaBarWidth - 10);
         $("#tpMetaCombo").change(onMetaComboChange);
+        $(".tpMetaLabel").click(onMetaClick);
+        $(".tpMetaValue").click(onMetaClick);
+        //$(".tpMetaValue").mouseover( onMetaMouseOver );
+        $(".tpMetaValue").mouseleave(function() {
+            $('#tpMetaTip').hide()
+        });
 
-        activateCombobox("tpLabelCombo", metaBarWidth - 10);
-        $("#tpLabelCombo").change(onLabelComboChange);
-        connectMetaPanel();
-    }
-
-    function makeTooltipCont() {
-        /* make a div for the tooltips */
-        var ttDiv = document.createElement('div');
-        ttDiv.id = "tpTooltip";
-        ttDiv.style.position = "absolute";
-        //ttDiv.style.left = left+"px";
-        //ttDiv.style.top = top+"px";
-        ttDiv.style["padding"] = "2px";
-        ttDiv.style["border"] = "1px solid black";
-        ttDiv.style["border-radius"] = "2px";
-        ttDiv.style["display"] = "none";
-        ttDiv.style["cursor"] = "pointer";
-        ttDiv.style["background-color"] = "white";
-        ttDiv.style["box-shadow"] = "0px 2px 4px rgba(0,0,0,0.3)";
-        ttDiv.style["user-select"] = "none";
-        ttDiv.style["z-index"] = "10";
-        return ttDiv;
+        // setup the right-click menu
+        //var menuItems = [{name: "Use as cluster label"},{name: "Copy field value to clipboard"}];
+        var menuItems = [{
+            name: "Copy field value to clipboard"
+        }];
+        var menuOpt = {
+            selector: ".tpMetaBox",
+            items: menuItems,
+            className: 'contextmenu-customwidth',
+            callback: onMetaRightClick
+        };
+        $.contextMenu(menuOpt);
+        // setup the tooltips
+        //$('[title!=""]').tooltip();
     }
 
     function showIntro(addFirst) {
         /* add the intro.js data */
         //var htmls = [];
         //htmls.push("<a href='http://example.com/' data-intro='Hello step one!'></a>");
         //$(document.body).append(htmls.join(""));
@@ -6033,29 +2922,29 @@
                 intro: "Are you here for the first time and wondering what this is?<br>The tutorial takes only 1 minute. To skip the tutorial now, click 'I know' below or press Esc.<br>You can always show it again by clicking 'Help > Tutorial'.",
             });
         }
 
         intro.addSteps(
             [{
                     intro: "In the middle of the screen, each circle represents a " + gSampleDesc + ". You can click the cluster label text to show the marker gene lists of the cluster.",
-                    element: document.querySelector('#mpCanvas'),
+                    element: document.querySelector('#tpCanvas'),
                     position: 'auto'
                 }, {
                     element: document.querySelector('#tpLeftSidebar'),
-                    intro: "Info and color control: move the mouse over a circle to show its annotation data.<br>Select an annotation field from the dropdown or simply click it, to color by the field. Click a gene from the list of pre-selected genes or search for a gene in the dropdown to color by it.<br>",
+                    intro: "Info and color control: move the mouse over a circle to show its annotation data.<br>Pick an annotation field or a gene to color on it.<br>",
                     position: 'auto'
                 },
                 //{
                 //element: document.querySelector('#tpGeneBar'),
                 //intro: "Expression data: when you move the mouse, expression values will be shown here.<br>Click on a gene to color the circles by gene expression level (log'ed).",
                 //position: 'top'
                 //},
                 {
                     element: document.querySelector('#tpLegendBar'),
-                    intro: "Click into the legend to select " + gSampleDesc + "s.<br>Click a color to change it or select a palette from the 'Colors' menu.<br>If you need a dataset, send us a link to it. If you have a new dataset in your lab, send it to cells@ucsc.edu so we can add it (hidden until publication).<br>To setup your own cell browser on your own webserver, see 'Help - Setup your own'.",
+                    intro: "Click into the legend to select " + gSampleDesc + "s.<br>Click a color to change it or select a palette from the 'Colors' menu.<br>To setup your own cell browser, see 'Help - Setup your own'",
                     position: 'left'
                 },
             ]);
         intro.start();
     }
 
     /**
@@ -6078,15 +2967,15 @@
         if (t < 2 / 3) return p + (q - p) * (2 / 3 - t) * 6;
         return p;
     }
 
     function hslToRgb(h, s, l) {
         var r, g, b;
 
-        if (s === 0) {
+        if (s == 0) {
             r = g = b = l; // achromatic
         } else {
             var q = l < 0.5 ? l * (1 + s) : l + s - l * s;
             var p = 2 * l - q;
 
             r = hue2rgb(p, q, h + 1 / 3);
             g = hue2rgb(p, q, h);
@@ -6115,88 +3004,26 @@
         var b = (rgb >> 0) & 0xff; // extract blue
 
         var luma = 0.2126 * r + 0.7152 * g + 0.0722 * b; // per ITU-R BT.709
 
         return (luma < 40);
     }
 
-    function makePercPalette(palName, n) {
-        /* palettes from https://github.com/politiken-journalism/scale-color-perceptual */
-        var pal = [];
-        var step = 1 / n;
-
-        var func = null;
-        switch (palName) {
-            case 'inferno':
-                func = scale.color.perceptual.inferno;
-                break;
-            case 'viridis':
-                func = scale.color.perceptual.viridis;
-                break;
-            case 'magma':
-                func = scale.color.perceptual.magma;
-                break;
-            case 'plasma':
-                func = scale.color.perceptual.plasma;
-                break;
-        }
-
-        for (let x = 0; x < n; x++) {
-            pal.push(func(x * step).substr(1));
-        }
-
-        if (pal.length !== n)
-            console.log("palette is too small");
-        return pal;
-    }
-
-    function makeTatarizePalette(n) {
-        /* suggested by Niko Papadopoulos from Detlev Arendt's group see http://godsnotwheregodsnot.blogspot.com/2012/09/color-distribution-methodology.html */
-        var pal = ["000000", "FFFF00", "1CE6FF", "FF34FF", "FF4A46", "008941", "006FA6", "A30059",
-            "FFDBE5", "7A4900", "0000A6", "63FFAC", "B79762", "004D43", "8FB0FF", "997D87",
-            "5A0007", "809693", "FEFFE6", "1B4400", "4FC601", "3B5DFF", "4A3B53", "FF2F80",
-            "61615A", "BA0900", "6B7900", "00C2A0", "FFAA92", "FF90C9", "B903AA", "D16100",
-            "DDEFFF", "000035", "7B4F4B", "A1C299", "300018", "0AA6D8", "013349", "00846F",
-            "372101", "FFB500", "C2FFED", "A079BF", "CC0744", "C0B9B2", "C2FF99", "001E09",
-            "00489C", "6F0062", "0CBD66", "EEC3FF", "456D75", "B77B68", "7A87A1", "788D66",
-            "885578", "FAD09F", "FF8A9A", "D157A0", "BEC459", "456648", "0086ED", "886F4C",
-            "34362D", "B4A8BD", "00A6AA", "452C2C", "636375", "A3C8C9", "FF913F", "938A81",
-            "575329", "00FECF", "B05B6F", "8CD0FF", "3B9700", "04F757", "C8A1A1", "1E6E00",
-            "7900D7", "A77500", "6367A9", "A05837", "6B002C", "772600", "D790FF", "9B9700",
-            "549E79", "FFF69F", "201625", "72418F", "BC23FF", "99ADC0", "3A2465", "922329",
-            "5B4534", "FDE8DC", "404E55", "0089A3", "CB7E98", "A4E804", "324E72", "6A3A4C"
-        ];
-        return pal.slice(0, n);
-    }
-
     function makeColorPalette(palName, n) {
         /* return an array with n color hex strings */
-        /* Use Google's palette functions for now, first Paul Tol's colors, if that fails, use the usual HSV rainbow
-         * This code understands our special palette, tol-sq-blue
-         */
+        // Use Google's palette functions for now, first Paul Tol's colors, if that fails, use the usual HSV rainbow
         var pal = [];
         if (palName === "blues")
             pal = makeHslPalette(0.6, n);
-        else if (palName === "magma" || palName === "viridis" || palName === "inferno" || palName == "plasma")
-            pal = makePercPalette(palName, n);
-        else if (palName === "iwanthue")
-            pal = iWantHue(n);
         else if (palName === "reds")
             pal = makeHslPalette(0.0, n);
-        else if (palName === "tatarize")
-            pal = makeTatarizePalette(n);
         else {
-            if (n === 2)
-                pal = ["ADD8E6", "FF0000"];
-            else {
-                var realPalName = palName.replace("tol-sq-blue", "tol-sq");
-                pal = palette(realPalName, n);
-                if (palName === "tol-sq-blue")
-                    pal[0] = 'f4f7ff';
-            }
+            pal = palette(palName, n);
+            if (palName === "tol-sq")
+                pal[0] = 'f4f7ff';
         }
 
         return pal;
     }
 
     function colorByCluster() {
         /* called when meta and coordinates have been loaded: scale data and color by meta field  */
@@ -6241,16 +3068,15 @@
             document.activeElement.blur();
         }
 
     }
 
     function setupKeyboard() {
         /* bind the keyboard shortcut keys */
-        phoneHome();
-        Mousetrap.bind('o', openCurrentDataset);
+        Mousetrap.bind('o', openDatasetDialog);
         Mousetrap.bind('c m', onMarkClearClick);
         Mousetrap.bind('h m', onMarkClick);
 
         Mousetrap.bind('space', onZoom100Click);
 
         Mousetrap.bind('z', function() {
             activateMode("zoom");
@@ -6260,89 +3086,35 @@
         });
         Mousetrap.bind('s', function() {
             activateMode("select");
         });
 
         Mousetrap.bind('-', onZoomOutClick);
         Mousetrap.bind('+', onZoomInClick);
-        Mousetrap.bind('s n', onSelectNoneClick);
-        Mousetrap.bind('s a', onSelectAllClick);
-        Mousetrap.bind('s i', onSelectInvertClick);
-        Mousetrap.bind('s s', onSelectNameClick);
-
-        Mousetrap.bind('b s', onBackgroudSetClick);
-        Mousetrap.bind('b r', onBackgroudResetClick);
-
-        Mousetrap.bind('m', function() {
-            $('#tpMetaCombo').trigger("chosen:open");
-            return false;
-        });
+        Mousetrap.bind('n', onSelectNoneClick);
+        Mousetrap.bind('a', onSelectAllClick);
         Mousetrap.bind('d', function() {
             $('#tpDatasetCombo').trigger("chosen:open");
             return false;
         });
-        //Mousetrap.bind('l', function() {$('#tpLayoutCombo').trigger("chosen:open"); return false;});
+        Mousetrap.bind('l', function() {
+            $('#tpLayoutCombo').trigger("chosen:open");
+            return false;
+        });
         Mousetrap.bind('g', function() {
             $("#tpGeneCombo").selectize()[0].selectize.focus();
             return false;
         });
         Mousetrap.bind('c l', onHideShowLabelsClick);
-        Mousetrap.bind('f c', onFindCellsClick);
-        Mousetrap.bind('f i', function() {
-            onSelectByIdClick();
-            return false;
-        });
-        Mousetrap.bind('t', onSplitClick);
-        Mousetrap.bind('h', onHeatClick);
-
-        Mousetrap.bind('up', function() {
-            renderer.movePerc(0, 0.1);
-            renderer.drawDots();
-        });
-        Mousetrap.bind('left', function() {
-            renderer.movePerc(-0.1, 0);
-            renderer.drawDots();
-        });
-        Mousetrap.bind('right', function() {
-            renderer.movePerc(0.1, 0);
-            renderer.drawDots();
-        });
-        Mousetrap.bind('down', function() {
-            renderer.movePerc(0, -0.1);
-            renderer.drawDots();
-        });
-
-        // yay vim
-        Mousetrap.bind('i', function() {
-            renderer.movePerc(0, 0.1);
-            renderer.drawDots();
-        });
-        Mousetrap.bind('j', function() {
-            renderer.movePerc(-0.1, 0);
-            renderer.drawDots();
-        });
-        Mousetrap.bind('l', function() {
-            renderer.movePerc(0.1, 0);
-            renderer.drawDots();
-        });
-        Mousetrap.bind('k', function() {
-            renderer.movePerc(0, -0.1);
-            renderer.drawDots();
-        });
 
-        //Mousetrap.stopCallback = function(e, element, combo) {
-        //var doStop = (element.tagName == 'INPUT' || element.tagName == 'SELECT' || element.tagName == 'TEXTAREA' || (element.contentEditable && element.contentEditable == 'true'));
-        //console.log(e, element, combo);
-        //return doStop;
-        //};
     }
 
     // https://stackoverflow.com/a/33861088/233871
     function isInt(x) {
-        return (typeof x === 'number') && x % 1 === 0;
+        return (typeof x === 'number') && x % 1 == 0;
     }
 
     function naturalSort(a, b) {
         /* copied from https://github.com/Bill4Time/javascript-natural-sort/blob/master/naturalSort.js */
         /* "use strict"; */
         var re = /(^([+\-]?(?:0|[1-9]\d*)(?:\.\d*)?(?:[eE][+\-]?\d+)?)?$|^0x[0-9a-f]+$|\d+)/gi,
             sre = /(^[ ]*|[ ]*$)/g,
@@ -6388,56 +3160,98 @@
                 return -1;
             }
             if (oFxNcL > oFyNcL) {
                 return 1;
             }
         }
         return 0;
-    }
+    };
 
     function sortPairsBy(countList, sortBy) {
         /* sort an array in the format [name, count] by either name (using naturalSort) or count */
+        // XX no need anymore to return a dict, just return the list
+        // convert the dict to a list of (count, key)
+        //var countList = [];
+        //var numCount = 0;
+        //var count = null;
+        //var useGradient = false; // use a rainbow or gradient palette?
+        //for (var key in dict) {
+        //count = dict[key];
+        //if (!isNaN(key)) // key looks like a number
+        //numCount++;
+        //countList.push( [count, key] );
+        //}
+
+        // auto-detect: sort list by name if most names are numbers
+        //if ((countList.length >= 4 && numCount >= countList.length-1)) {
+        //if (sortBy===undefined)
+        //sortBy = "name";
+        //useGradient = true;
+        //}
+
         var isSortedByName = null;
 
         if (sortBy === "name") {
             countList.sort(function(a, b) {
                 return naturalSort(a[0], b[0]);
             }); // I have a feeling that this is very slow...
             isSortedByName = true;
-        } else if (sortBy == "count") {
+        } else {
             // sort this list by count
             countList = countList.sort(function(a, b) {
                 return b[1] - a[1];
             }); // reverse-sort by count
             isSortedByName = false;
-        } else {
-            isSortedByName = false;
         }
 
         var ret = {};
         ret.list = countList;
         ret.isSortedByName = isSortedByName;
         // pallette should be a gradient for data types where this makes sense
         return ret;
     }
 
+    function assignColors(fieldIdx, countList, doReset) {
+        /* given an array of (count, value), assign a color to every value.
+         Returns an dict of value : (color as integer, color as hex string without #)
+         Will check if user has a manually defined color for this field before and use it, if present.
+         If doReset is true, will delete of manual definitions.
+         */
+    }
+
     function plotSelection(coords) {
         /* redraw block dots of current selection
            Redrawing makes sure that they are not hidden underneath others.
         */
         for (var i = 0; i < coords.length; i++) {
             var x = coords[i][0];
             var y = coords[i][1];
             var fill = coords[i][2];
             var dot = drawCircle(x, y, fill, 0x000000);
             stage.addChild(dot);
             visibleGlyps.push(dot);
         }
     }
 
+    function findDotsWithMeta(metaIdx, hlValue) {
+        /* return array of cellIds with a given meta value */
+        var metaData = gCurrentDataset.metaData;
+        ret = [];
+        for (var i = 0; i < pixelCoords.length; i++) {
+            var cellId = pixelCoords[i][0];
+            var x = pixelCoords[i][1];
+            var y = pixelCoords[i][2];
+            var metaRow = metaData[cellId];
+            var metaVal = metaRow[metaIdx];
+            if (metaVal === hlValue) {
+                ret.push(cellId);
+            }
+        }
+    }
+
     function removeCellIds(coords, cellIds) {
         /* remove all coords that are in an object of cellIds */
         var newCoords = [];
         for (var i = 0; i < coords.length; i++) {
             var coord = coords[i];
             var cellId = coord[0];
             if (!(cellId in cellIds))
@@ -6454,106 +3268,88 @@
             var cellId = coord[0];
             if (cellId in cellIds)
                 newCoords.push(coord);
         }
         return newCoords;
     }
 
-    function countValues(arr) {
-        var counts = {};
-        for (var i = 0; i < arr.length; i++) {
-            counts[arr[i]] = 1 + (counts[arr[i]] || 0);
-        }
-        var countArr = Object.entries(counts);
-        return countArr
-    }
-
-    function makeLabelRenames(metaInfo) {
-        /* return an obj with old cluster name -> new cluster name */
-        var valCounts = metaInfo.valCounts;
-        if (valCounts === undefined) { // 'int' and 'float' types do not have their values counted yet
-            // this doesn't work because the values are not loaded yet, requires moving this call to
-            // later
-            //metaInfo.valCounts = countValues(metaInfo.arr);
-            alert("cannot label on numeric fields, please use the enumFields option in cellbrowser.conf");
-        }
-        var newLabels = metaInfo.ui.shortLabels;
-
-        var oldToNew = {};
-        for (var i = 0; i < valCounts.length; i++) {
-            var oldLabel = valCounts[i][0];
-            var newLabel = newLabels[i];
-            oldToNew[oldLabel] = newLabel;
-        }
-        return oldToNew;
-    }
-
-    function getClusterFieldInfo() {
-        var clusterField = db.conf.activeLabelField;
-        var clusterMetaInfo = db.findMetaInfo(clusterField);
-        return clusterMetaInfo;
-    }
-
-    function rendererUpdateLabels(metaInfo) {
-        /* update the labels in the renderer from the metaInfo data. */
-        var oldToNew = makeLabelRenames(metaInfo);
-
-        var oldRendLabels = null;
-        if (renderer.origLabels) {
-            oldRendLabels = renderer.origLabels;
+    function onLegendLabelClick(ev) {
+        /* called when user clicks on legend entry. */
+        var legendId = parseInt(ev.target.id.split("_")[1]);
+        if (("lastClicked" in gLegend) && gLegend.lastClicked == legendId) {
+            // user clicked the same entry as before: clear selection
+            gLegend.lastClicked = null;
+            renderer.selectClear();
+            $('#tpLegend_' + legendId).removeClass('tpLegendSelect');
+            menuBarHide("#tpFilterButton");
+            menuBarHide("#tpOnlySelectedButton");
+            updateGeneTableColors(null);
         } else {
-            oldRendLabels = renderer.getLabels();
-            renderer.origLabels = oldRendLabels;
-        }
-
-        var newRendLabels = [];
-        for (var i = 0; i < oldRendLabels.length; i++) {
-            var oldLabel = oldRendLabels[i];
-            var newLabel = oldToNew[oldLabel];
-            newRendLabels.push(newLabel);
+            if (!ev.shiftKey && !ev.ctrlKey && !ev.metaKey) {
+                renderer.selectClear();
+                $('.tpLegend').removeClass('tpLegendSelect');
+            }
+            console.log(ev);
+            var colIdx = gLegend.rows[legendId][4];
+            //gSelCellIds = findCellIdsForLegendIds(gClasses, [legendId], gSelCellIds);
+            renderer.selectByColor(colIdx);
+            menuBarShow("#tpFilterButton");
+            menuBarShow("#tpOnlySelectedButton");
+            $('#tpLegend_' + legendId).addClass('tpLegendSelect');
+            gLegend.lastClicked = legendId;
+            //updateSelection();
         }
-        renderer.setLabels(newRendLabels);
+        renderer.drawDots();
     }
 
-    function onLegendLabelClick(ev) {
-        /* called when user clicks on legend entry. */
-
-        var legendId = parseInt(ev.target.id.split("_")[1]);
-        var colorIndex = gLegend.rows[legendId].intKey;
-        $("#tpLegendCheckbox_" + colorIndex).click();
+    function legendResetColors() {
+        /* reset all manual colors in legend to defaults */
+        var rows = gLegend.rows;
+        if (rows === undefined)
+            return;
+        for (var i = 0; i < rows.length; i++) {
+            var colorHex = rows[i][0];
+            var defColor = rows[i][1];
+            gLegend.rows[i][0] = null;
+            var saveKey = rows[i][5];
+            // also clear localStorage
+            localStorage.removeItem(saveKey);
+        }
     }
 
     function onSortByClick(ev) {
         /* flip the current legend sorting */
         var sortBy = null;
-        if (ev.target.parentElement.id.endsWith("Col1")) // column 1 is the Name
+        if (ev.target.id.endsWith("Col1")) // column 1 is the Name
             sortBy = "name"
         else
             sortBy = "freq";
 
-        saveToUrl("s_" + gLegend.metaInfo.name, sortBy, gLegend.defaultSortBy);
+        cartSave("s_" + gLegend.fieldName, sortBy, gLegend.defaultSortBy);
         legendSort(sortBy);
-        $(".tooltip").hide();
         buildLegendBar();
     }
 
 
     function onMetaRightClick(key, options) {
         /* user right-clicks on a meta field */
-        var metaName = options.$trigger[0].id.split("_")[1];
+        var metaIdx = parseInt(options.$trigger[0].id.split("_")[1]);
 
         //if (key==0) {
         //gCurrentDataset.labelField = gCurrentDataset.metaFields[metaIdx];
         //gClusterMids = null; // force recalc
         //plotDots();
         //renderer.render(stage);
         //updateMenu();
         //}
-        if (key === 0) {
-            copyToClipboard("#tpMeta_" + metaName);
+        if (key == 0) {
+            copyToClipboard("#tpMeta_" + metaIdx);
+            //$("textarea").select();
+            //document.execCommand('copy');
+            //console.log(val);
         }
 
     }
 
     //function onLegendRightClick (key, options) {
     /* user right-clicks on a legend label */
     //var selEls = $(".tpLegendSelect")
@@ -6572,273 +3368,174 @@
     //mode = "showOnly";
     //filterCoordsAndUpdate(cellIds, mode);
     //}
 
     function setLegendHeaders(type) {
         /* set the headers of the right-hand legend */
         if (type === "category") {
-            $('#tpLegendCol1').html('<span title="select all checkboxes below" id="tpLegendClear">&#9745;</span><span class="tpLegendHover" title="click to sort by name"> Name<span class="caret"></span></span>');
-            $('#tpLegendCol2').html('<span class="tpLegendHover" title="click to sort by frequency"> Frequency<span class="caret"></span></span>');
+            $('#tpLegendCol1').html('Name<span class="caret"></span>');
+            $('#tpLegendCol2').html('Frequency<span class="caret"></span>');
         } else {
-            $('#tpLegendCol1').html('<span title="select all checkboxes below" id="tpLegendClear">&#9745;</span> Range<span');
+            $('#tpLegendCol1').html('Range');
             $('#tpLegendCol2').html('Frequency');
         }
-        activateTooltip("#tpLegendClear");
-        activateTooltip(".tpLegendHover");
-    }
-
-    function updateLegendGrandCheckbox() {
-        var checkbox = $("#tpLegendClear");
-        var total = renderer.getCount();
-        var selected = renderer.selCells.size;
-        if (gLegend.selectionDirection == "all" && total == selected) {
-            gLegend.selectionDirection = "none";
-            checkbox.html("&#9746;");
-            // from https://stackoverflow.com/questions/9501921/change-twitter-bootstrap-tooltip-content-on-click
-            checkbox.attr('title', "unselect all checkboxes below");
-            var tip = checkbox.bsTooltip('fixTitle').data('bs.tooltip').$tip;
-            if (tip) {
-                tip.find('.tooltip-inner')
-                    .text("unselect all checkboxes below");
-            }
-        } else if (gLegend.selectionDirection == "none" && selected === 0) {
-            gLegend.selectionDirection = "all";
-            checkbox.html("&#9745;");
-            checkbox.attr('title', "select all checkboxes below");
-            var tip = checkbox.bsTooltip('fixTitle').data('bs.tooltip').$tip;
-            if (tip) {
-                tip.find('.tooltip-inner')
-                    .text("select all checkboxes below");
-            }
-        }
-    }
-
-    function onLegendClearClick(ev) {
-        /* unselect all checkboxes in the legend and clear the selection */
-        if (gLegend.selectionDirection == "all") {
-            clearSelectionState();
-            renderer.selectAll();
-            renderer.drawDots();
-        } else {
-            onSelectNoneClick();
-        }
-        ev.stopPropagation();
-    }
-
-    function onLegendApplyLimitsClick(ev) {
-        /* user clicked the apply button: apply limits to the plot and redraw */
-        makeLegendExpr(gLegend.geneSym, gLegend.titleHover, binInfo, exprArr, decArr);
     }
 
-    function onLegendCheckboxClick(ev) {
-        /* user clicked the small checkboxes in the legend */
-        var valIdx = parseInt(ev.target.getAttribute("data-value-index"));
-        if ($(this).is(':checked'))
-            renderer.selectByColor(valIdx);
-        else
-            renderer.unselectByColor(valIdx);
-        renderer.drawDots();
-        ev.stopPropagation();
-        $(this).blur();
-    }
-
-    function buildMinMaxPart(htmls) {
-        /* create the min/max and apply/reset buttons */
-        htmls.push("<div>");
-        htmls.push("<table style='margin: 4px; margin-top: 6px'>");
-        htmls.push("<tr>");
-        htmls.push("<td><label for='exprMin'>Min:</label></td>");
-        htmls.push("<td><input name='exprMin' size='8' type='text'></td>");
-        htmls.push("<td><button id='tpExprLimitApply' style='border-radius: 4px; margin-left: 4px; padding: 3px 6px 3px 6px' class='ui-button'>Apply</button></td>");
-        htmls.push("</tr>");
-
-        htmls.push("<tr>");
-        htmls.push("<td><label for='exprMax'>Max:</label></td>");
-        htmls.push("<td><input name='exprMax' size='8' type='text'></td>");
-        htmls.push("<td><button id='tpExprLimitClear' style='border-radius: 4px; margin-left: 4px; padding: 3px 6px 3px 6px' class='ui-button'>Clear</button></td>");
-        htmls.push("</tr>");
-        htmls.push("</table>");
-        htmls.push("</div>");
-    }
-
-
-    function buildLegendBar() {
+    function buildLegendBar(sortBy) {
         /* draws current legend as specified by gLegend.rows
+         * sortBy can be "name" or "count" or "undefined" (=auto-detect)
          * */
-        if (gLegend.rows === undefined)
+        if (gLegend.rows == undefined)
             return;
 
         $('#tpLegendContent').empty();
 
         var htmls = [];
 
         var colors = [];
         var rows = gLegend.rows;
 
-        var legTitle = gLegend.title;
-        var subTitle = gLegend.subTitle;
-
-        htmls.push('<span id="tpLegendTitle" title="' + gLegend.titleHover + '">' + legTitle + "</span>");
-        if (subTitle)
-            htmls.push('<div id="tpLegendSubTitle" >' + subTitle + "</div>");
-        htmls.push('<div class="tpHint">Check boxes below to select ' + gSampleDesc + 's</small></div>');
+        htmls.push('<span id="tpLegendTitle" title="' + gLegend.titleHover + '">' + gLegend.title + "</span>");
+        htmls.push('<div class="tpHint">Click below to select ' + gSampleDesc + 's</small></div>');
         htmls.push("</div>"); // title
         htmls.push('<div id="tpLegendHeader"><span id="tpLegendCol1"></span><span id="tpLegendCol2"></span></div>');
-        htmls.push('<div id="tpLegendRows">');
 
         // get the sum of all, to calculate frequency
         var sum = 0;
         for (var i = 0; i < rows.length; i++) {
-            let count = rows[i].count;
+            var count = rows[i][3];
             sum += count;
         }
 
-        for (i = 0; i < rows.length; i++) {
+        var acronyms = db.conf.acronyms;
+        if (acronyms === undefined)
+            acronyms = {};
+
+        for (var i = 0; i < rows.length; i++) {
             var row = rows[i];
-            var colorHex = row.color; // manual color
+            var colorHex = row[0]; // manual color
             if (colorHex === null)
-                colorHex = row.defColor; // default color
+                colorHex = row[1]; // default color
 
-            var label = row.label;
-            var longLabel = row.longLabel;
+            var label = row[2];
 
-            let count = row.count;
-            var valueIndex = row.intKey;
+            var count = row[3];
             var freq = 100 * count / sum;
 
-            if (count === 0) // never output categories with 0 count.
-                continue;
-
             var labelClass = "tpLegendLabel";
             label = label.replace(/_/g, " ").replace(/'/g, "&#39;").trim();
-            if (longLabel)
-                longLabel = longLabel.replace(/_/g, " ").trim();
 
             if (likeEmptyString(label)) {
                 labelClass += " tpGrey";
+                colorHex = cNullColor;
             }
             if (label === "") {
                 label = "(empty)";
             }
 
-            colors.push([i, colorHex]); // save for later
+            colors.push(colorHex); // save for later
 
-            var mouseOver = "";
-            // only show the full value on mouse over if the label is long, "" suppresses mouse over
-            if (longLabel && longLabel != label)
-                mouseOver = longLabel;
-            else {
-                if (label.length > 20)
-                    mouseOver = label;
+            var labelDesc = label;
+            var labelDesc = acronyms[label] || null;
+            if (labelDesc === null) {
+                // only show the full value on mouse over if the label is long, "" suppresses mouse over
+                if (label.length > 20 || labelDesc === null)
+                    labelDesc = label;
+                else
+                    labelDesc = "";
             }
 
             var classStr = "tpLegend";
-            var line = "<div id='tpLegend_" + valueIndex + "' class='" + classStr + "'>";
+            var line = "<div id='tpLegend_" + i + "' class='" + classStr + "'>";
             htmls.push(line);
-            htmls.push("<input class='tpLegendCheckbox' data-value-index='" + valueIndex + "' " +
-                "id='tpLegendCheckbox_" + valueIndex + "' type='checkbox'>");
             htmls.push("<input class='tpColorPicker' id='tpLegendColorPicker_" + i + "' />");
 
-            htmls.push("<span class='" + labelClass + "' id='tpLegendLabel_" + i + "' data-placement='auto top' title='" + mouseOver + "'>");
+            htmls.push("<span class='" + labelClass + "' id='tpLegendLabel_" + i + "' data-placement='auto top' title='" + labelDesc + "'>");
             htmls.push(label);
             htmls.push("</span>");
+            //htmls.push("<span class='tpLegendCount'>"+count+"</div>");
             var prec = 1;
             if (freq < 1)
                 prec = 2;
-            htmls.push("<span class='tpLegendCount' title='" + count + " of " + sum + "'>" + freq.toFixed(prec) + "%</span>");
+            htmls.push("<span class='tpLegendCount' title='" + count + " of " + sum + "'>" + freq.toFixed(prec) + "%</div>");
             htmls.push("</span>");
 
             htmls.push("</div>");
+            //htmls.push("<input class='tpLegendCheckbox' id='tpLegendCheckbox_"+i+"' type='checkbox' checked style='float:right; margin-right: 5px'>");
         }
-        htmls.push('</div>'); // tpLegendRows
 
         // add the div where the violin plot will later be shown
         htmls.push("<div id='tpViolin'>");
         htmls.push("<canvas style='height:200px; padding-top: 10px; padding-bottom:30px' id='tpViolinCanvas'></canvas>");
         htmls.push("</div>"); // violin
 
         var htmlStr = htmls.join("");
         $('#tpLegendContent').append(htmlStr);
         setLegendHeaders(gLegend.rowType);
 
-        // tpLegendContent has to go only up to the bottom of the screen.
-        // This is done again in resizeDivs()
-        // I have not found a way to do this in CSS...
-        $("#tpLegendBar").css("height", (window.innerHeight - $('#tpLegendBar').offset().top) + "px");
-
         activateTooltip("#tpResetColors");
         activateTooltip("#tpSortBy");
-
         $("#tpLegendCol1").click(onSortByClick);
         $("#tpLegendCol2").click(onSortByClick);
-        $(".tpLegendCheckbox").click(onLegendCheckboxClick);
-        $("#tpLegendClear").click(onLegendClearClick);
-        $("#tpExprLimitApply").click(onLegendApplyLimitsClick);
 
         $('.tpLegend').click(onLegendLabelClick);
         //$('.tpLegendLabel').attr( "title", "Click to select samples with this value. Shift click to select multiple values.");
+        //$('#tpResetColors').click( onResetColorsClick );
+        //$('#tpSortBy').click( onSortByClick );
         activateTooltip(".tpLegendLabel");
         activateTooltip(".tpLegendCount");
 
         // setup the right-click menu
         //var menuItems = [{name: "Hide "+gSampleDesc+"s with this value"}, {name:"Show only "+gSampleDesc+"s with this value"}];
         //var menuOpt = {
         //selector: ".tpLegend",
         //items: menuItems,
         //className: 'contextmenu-customwidth',
         //callback: onLegendRightClick
         //};
         //$.contextMenu( menuOpt );
 
         // activate the color pickers
-        for (let i = 0; i < colors.length; i++) {
-            var colInfo = colors[i];
-            var rowIdx = colInfo[0];
-            var hexCode = colInfo[1];
-
+        for (var i = 0; i < colors.length; i++) {
             var opt = {
                 hideAfterPaletteSelect: true,
-                color: hexCode,
+                color: colors[i],
                 showPalette: true,
-                allowEmpty: true,
+                //allowEmpty : true,
                 showInput: true,
                 preferredFormat: "hex",
                 change: onColorPickerChange
             }
-            $("#tpLegendColorPicker_" + rowIdx).spectrum(opt);
+            $("#tpLegendColorPicker_" + i).spectrum(opt);
         }
 
         buildViolinPlot();
+
     }
 
-    function onColorPickerChange(color, ev) {
+    function onColorPickerChange(color) {
         /* called when user manually selects a color in the legend with the color picker */
-        console.log(ev);
-        /* jshint validthis: true */
         var valueIdx = parseInt(this.id.split("_")[1]);
         var rows = gLegend.rows;
         var clickedRow = rows[valueIdx];
-        var oldColorHex = clickedRow.color;
-        var defColorHex = clickedRow.defColor;
-        var valueKey = clickedRow.strKey;
-        if (valueKey === "")
-            valueKey = "_EMPTY_";
+        var oldColorHex = clickedRow[0];
+        var defColorHex = clickedRow[1];
 
-        /* jshint validthis: true */
         var newCol = $(this).spectrum('get');
 
         var newColHex = "";
         if (newCol === null)
             newColHex = oldColorHex; // if user clicked abort, revert to default color
         else
             newColHex = newCol.toHex();
-        clickedRow.color = newColHex;
+        clickedRow[0] = newColHex;
 
+        var saveKey = COL_PREFIX + clickedRow[5];
         // save color to cart if necessary
-        saveToUrl(COL_PREFIX + valueKey, newColHex, defColorHex);
+        cartSave(saveKey, newColHex, defColorHex);
 
         var colors = legendGetColors(gLegend.rows);
         renderer.setColors(colors);
         renderer.drawDots();
     }
 
     function updateGeneTableColors(cellIds) {
@@ -6846,681 +3543,303 @@
         var quickGenes = db.conf.quickGenes;
         if (quickGenes === undefined)
             return;
 
         if (cellIds === null)
             cellIds = [];
 
-        var pal = makeColorPalette(datasetGradPalette, exprBinCount);
+        var pal = makeColorPalette(cDefGradPalette, exprBinCount);
 
-        //console.time("avgCalc");
+        console.time("avgCalc");
         for (var i = 0; i < quickGenes.length; i++) {
             var sym = quickGenes[i][0];
             //console.log("updating colors of "+sym+" for "+cellIds.length+" cells");
             var geneExpr = db.quickExpr[sym];
             if (geneExpr === undefined) { // if any gene is not loaded yet, just quit
                 console.log(sym + " is not loaded yet, not updating expr table colors");
                 return;
             }
             var vec = geneExpr[0];
             var binInfo = geneExpr[1];
             var sum = 0;
 
             var avg = 0;
-            if (cellIds !== null && cellIds.length !== 0) {
+            if (cellIds !== null && cellIds.length != 0) {
                 for (var ci = 0; ci < cellIds.length; ci++) {
                     sum += vec[cellIds[ci]];
                 }
                 avg = Math.round(sum / cellIds.length);
+                //console.log("sum "+sum+" avg "+avg);
             }
             var color = pal[avg];
+            //console.log("color "+color);
+            $("#tpGeneBarCell_" + i).css("background-color", "#" + color);
             var fontColor = "#333333";
             if (isDark(color))
                 fontColor = "white";
-            $("#tpGeneBarCell_" + onlyAlphaNum(sym)).css({
-                "background-color": "#" + color,
-                "color": fontColor
-            });
+            $("#tpGeneBarCell_" + i).css("color", fontColor);
         }
-        //console.timeEnd("avgCalc");
+        console.timeEnd("avgCalc");
     }
 
-    function makeFieldHistogram(metaInfo, selCellIds, metaVec) {
-        /* count the values in metaInfo and return a sorted array of [count, fraction, valIndex] */
-        let cellCount = selCellIds.length;
-        if (!metaInfo.ui.shortLabels && (metaInfo.type === "float" || metaInfo.type === "int")) {
-            // it's a numeric field, so let's create the labels now, they are derived from the bins
-            let shortLabels = [];
-            for (let bin of metaInfo.binInfo)
-                shortLabels.push(labelForBinMinMax(bin[0], bin[1])); // 0,1 is min,max of the bin
-            metaInfo.ui.shortLabels = shortLabels;
-        }
-
+    function countValues(arr) {
+        /* count values in array, return an array of [value, count], sorted by count */
+        // first make a list of all possible meta values and their counts
+        var metaData = gCurrentDataset.metaData;
         var metaCounts = {};
-        // make an object with value -> count in the cells
-        for (var i = 0; i < cellCount; i++) {
-            var cellId = selCellIds[i];
-            var metaVal = metaVec[cellId];
+        for (var i = 0; i < pixelCoords.length; i++) {
+            var cellId = pixelCoords[i][0];
+            var metaRow = metaData[cellId];
+            var metaVal = metaRow[metaIndex];
             metaCounts[metaVal] = 1 + (metaCounts[metaVal] || 0);
         }
-        var categories = metaInfo.binInfo;
-        var catCountIdx = 2;
-        if (categories === undefined) {
-            categories = metaInfo.valCounts;
-            catCountIdx = 1;
-        }
-
-        // convert the object to an array (count, percent, value) and sort it by count
-        var histoList = [];
-        for (var key in metaCounts) {
-            let intKey = parseInt(key);
-            let count = metaCounts[key];
-            let frac = (count / cellCount);
-            let fracOfCategory;
-            if (categories) {
-                let catCellCount = categories[intKey][catCountIdx];
-                fracOfCategory = count / catCellCount;
-            }
-            histoList.push([count, frac, intKey, fracOfCategory]);
-        }
-        if (metaInfo.type !== "float" && metaInfo.type !== "int") {
-            histoList = histoList.sort(function(a, b) {
-                return b[0] - a[0];
-            }); // reverse-sort by count
+
+        var counts = {};
+        for (var i = 0; i < arr.length; i++) {
+            var val = arr[i];
+            counts[val] = (counts[num] || 0) + 1;
+            var metaVal = metaRow[metaIndex];
         }
-        return histoList;
     }
 
     function updateMetaBarManyCells(cellIds) {
         /* update the meta fields on the left to reflect/summarize a list of cellIds */
-        var metaFieldInfos = db.getMetaFields();
-        //var metaData = gCurrentDataset.metaData;
+        var metaFields = gCurrentDataset.metaFields;
+        var metaData = gCurrentDataset.metaData;
         var cellCount = cellIds.length;
-
-        if (db.allMeta === undefined) {
-            alert("The meta information has not been loaded yet. Please wait and try again in a few seconds.");
-            return;
-        }
-
         $('#tpMetaTitle').text("Meta data of " + cellCount + " " + gSampleDesc + "s");
 
         // for every field...
         var metaHist = {};
-        for (var metaIdx = 0; metaIdx < metaFieldInfos.length; metaIdx++) {
-            var metaInfo = metaFieldInfos[metaIdx];
-
-            var metaVec = [];
-            if (metaInfo.isCustom)
-                metaVec = metaInfo.arr;
-            else
-                metaVec = db.allMeta[metaInfo.name];
-
-            if (metaVec === undefined) {
-                var metaMsg = null;
-                if (metaInfo.type !== "uniqueString") {
-                    console.log("cellBrowser.js:updateMetaBarManyCells - could not find meta info");
-                    metaMsg = "(still loading - please wait and retry)";
-                } else
-                    metaMsg = "(unique identifier field)";
-                $('#tpMeta_' + metaIdx).html(metaMsg);
-                continue;
+        for (var metaIdx = 0; metaIdx < metaFields.length; metaIdx++) {
+            var metaCounts = {};
+            // make an object of value -> count in the cells
+            for (var i = 0; i < cellCount; i++) {
+                var cellId = cellIds[i];
+                var metaVal = metaData[cellId][metaIdx];
+                metaCounts[metaVal] = 1 + (metaCounts[metaVal] || 0);
+            }
+            // convert the object to an array (count, percent, value) and sort it by count
+            var histoList = [];
+            for (var key in metaCounts) {
+                var count = metaCounts[key];
+                var frac = (count / cellCount);
+                histoList.push([count, frac, key]);
             }
-
-            var histoList = makeFieldHistogram(metaInfo, cellIds, metaVec); // reverse-sort by count
-            metaHist[metaInfo.name] = histoList;
+            histoList = histoList.sort(function(a, b) {
+                return b[0] - a[0];
+            }); // reverse-sort by count
+            metaHist[metaIdx] = histoList;
 
             // make a quick list of the top values for the sparklines, ignore the rest
             var countList = [];
             var otherCount = 0;
-            for (let i = 0; i < histoList.length; i++) {
-                let count = histoList[i][0];
+            for (var i = 0; i < histoList.length; i++) {
+                var count = histoList[i][0];
                 if (i < SPARKHISTOCOUNT)
                     countList.push(count);
                 else
                     otherCount += count;
             }
             if (otherCount !== 0)
                 countList.push(otherCount);
 
             // update the UI
 
             var topCount = histoList[0][0];
             var topPerc = histoList[0][1];
-            var topVal = metaInfo.ui.shortLabels[histoList[0][2]];
+            var topVal = histoList[0][2];
             var percStr = (100 * topPerc).toFixed(1) + "%";
 
             if (topVal.length > 14)
                 topVal = topVal.substring(0, 14) + "...";
 
             var label = "";
-            if (histoList.length === 1) {
+            if (histoList.length !== 1) {
+                if (histoList[0][0] === 1)
+                    label = "<span class='tpMetaMultiVal'>" + histoList.length + " unique values</span>";
+                else
+                    //label = "<span class='tpMetaMultiVal'>" + histoList.length + " values</span><span class='tpMetaHistLabel'> Histogram </span>&nbsp;&nbsp;<span id='tpMetaSpark_"+metaIdx+"'></span>";
+                    //label = "<span class='tpMetaMultiVal'>" + histoList.length + " values</span>&nbsp;<span id='tpMetaSpark_"+metaIdx+"'></span>";
+                    label = "<span class='tpMetaMultiVal'>" + percStr + " " + topVal + "</span>&nbsp;<span class='tpMetaSpark' id='tpMetaSpark_" + metaIdx + "'></span>";
+            } else
                 label = topVal;
-            } else {
-                // numeric type, calculate mean and sd
-                if (metaInfo.origVals && (metaInfo.type === "float" || metaInfo.type === "int")) {
-                    var sum = 0;
-                    for (var i = 0, I = cellIds.length; i < I; i++) {
-                        sum += metaInfo.origVals[cellIds[i]];
-                    }
-                    var mean = sum / cellIds.length;
-                    sum = 0;
-                    for (i = 0, I = cellIds.length; i < I; i++) {
-                        sum += (metaInfo.origVals[cellIds[i]] - mean) ** 2;
-                    }
-                    var sd = Math.sqrt(sum / cellIds.length);
-                    label = "<span class='tpMetaMultiVal'>mean = " + mean.toFixed(2) + "; sd = " + sd.toFixed(2) + "</span>";
-                } else {
-                    if (histoList[0][0] === 1) {
-                        label = "<span class='tpMetaMultiVal'>" + histoList.length + " unique values</span>";
-                    } else {
-                        label = "<span class='tpMetaMultiVal'>" + percStr + " " + topVal + "</span>";
-                    }
-                }
-            }
 
             $('#tpMeta_' + metaIdx).html(label);
+            $('#tpMetaSpark_' + metaIdx).sparkline(countList, {
+                type: "bar",
+                barSpacing: 0,
+                disableTooltips: true
+            });
+
+            //var topCount = countList[0][0];
+            //var topPerc  = countList[0][1];
+            //var topVal   = countList[0][2];
+            //$('#tpMeta_'+metaIdx).text(topVal);
+            //var label = metaFieldToLabel(metaFields[metaIdx]);
+            //$('#tpMetaLabel_'+metaIdx).html(label+"<span class='tpMetaPerc'>"+(100*topPerc).toFixed(1)+"%</span>");
         }
-        db.metaHist = metaHist;
+        gCurrentDataset.metaHist = metaHist;
     }
 
     function clearMetaAndGene() {
-        /* called when user hovers over nothing - clear the meta and gene field field info, hide the tooltip */
-        if (db === null) // users moved the mouse while the db is still loading
-            return;
-
-        $('#tpMeta_custom').html("");
-        $(".tpMetaValue").html("");
-
-        var fieldCount = db.getMetaFields();
-        for (let metaInfo of db.getMetaFields()) {
-            $('#tpMeta_' + metaInfo.name).attr('title', "").html("");
+        /* clear the meta and gene field field info */
+        var fieldCount = db.getMetaFields().length;
+        for (var i = 0; i < fieldCount; i++) {
+            $('#tpMeta_' + i).attr('title', "");
+            $('#tpMeta_' + i).html("");
         }
-        $('#tpMetaNote').hide();
         updateGeneTableColors(null);
     }
 
-    function updateMetaBarCustomFields(cellId) {
-        /* update custom meta fields with custom data */
-        if (!db.getMetaFields()[0].isCustom)
-            return;
-
-        let metaInfo = db.getMetaFields()[0];
-        let intVal = metaInfo.arr[cellId];
-        let strVal = metaInfo.ui.shortLabels[intVal];
-        let rowDiv = $('#tpMeta_custom').html(strVal);
-    }
-
-    function updateMetaBarOneCell(cellInfo, otherCellCount) {
+    function updateMetaBarOneCell(cellInfo) {
         /* update the meta bar with meta data from a single cellId */
         $('#tpMetaTitle').text(METABOXTITLE);
-
-        let customCount = 0;
-        if (db.getMetaFields()[0].isCustom)
-            customCount = 1;
-
-        let fieldInfos = db.getMetaFields();
-
         for (var i = 0; i < cellInfo.length; i++) {
             var fieldValue = cellInfo[i];
-            let metaIdx = i + customCount;
-            let metaInfo = fieldInfos[metaIdx];
-
-            let rowDiv = $('#tpMeta_' + i);
             if (fieldValue.startsWith("http") && fieldValue.endsWith(".png")) {
-                rowDiv.css('height', "40px");
-                rowDiv.html("<img src='" + fieldValue + "'></img>");
+                $('#tpMeta_' + i).css('height', "40px");
+                $('#tpMeta_' + i).html("<img src='" + fieldValue + "'></img>");
             } else
-                rowDiv.html(fieldValue);
-            rowDiv.attr('title', cellInfo[i]);
-        }
-
-        if (otherCellCount === 0)
-            $("#tpMetaNote").hide();
-        else {
-            $("#tpMetaNote").html("...and " + (otherCellCount) + " other " + gSampleDesc + "s underneath");
-            $("#tpMetaNote").show();
+                $('#tpMeta_' + i).html(fieldValue);
+            $('#tpMeta_' + i).attr('title', cellInfo[i]);
         }
     }
 
-    function clearSelectionState() {
-        /* clear URL variable with select state, called when user clicks cells or unselects them */
-        delState("select");
+    function onDotMouseOver(mouseData) {
+        /* user hovers over a circle with the mouse */
+        if (mouseDownX != null) // user is currently zooming
+            return;
+        if (!(gSelCellIds === null || jQuery.isEmptyObject(gSelCellIds))) // some cells are selected
+            return;
+        var cellId = mouseData.target.cellId;
+        this.alpha = 1.0;
+        //renderer.render(stage);
 
-        $("#tpHoverHint").show();
-        $("#tpSelectHint").hide();
+        //db.loadMetaForCell(cellId, function(ci) { updateMetaBarOneCell(ci);} onProgress);
+        updateGeneTableColors([cellId]);
     }
 
     function onCellClickOrHover(cellIds, ev) {
         /* user clicks onto a circle with the mouse or hovers over one.
-         * ev is undefined if not a click. cellIds is none if click was on empty background. */
+         * ev is undefined if not a click. */
 
-        // do nothing if only hover but something is already selected
+        // do nothing if only hover but we already have a selection
         var selCells = renderer.getSelection();
-        if (ev === undefined && selCells.length !== 0) {
-            $("#tpHoverHint").hide();
-            $("#tpSelectHint").show();
+        if (ev === undefined && selCells !== null && selCells.length !== 0)
             return;
-        }
-
-        $("#tpHoverHint").show();
-        $("#tpSelectHint").hide();
 
-        // if click into background, remove any legend selection
-        if (cellIds === null)
-            $(".tpLegendLabel").removeClass("tpLegendSelect");
-
-        if (cellIds === null || cellIds.length === 0) {
+        if (cellIds === null || cellIds.length === 0)
             clearMetaAndGene();
-        } else {
+        else {
             var cellId = cellIds[0];
-            var cellCountBelow = cellIds.length - 1;
-            updateMetaBarCustomFields(cellId);
             db.loadMetaForCell(cellId, function(ci) {
-                updateMetaBarOneCell(ci, cellCountBelow);
+                updateMetaBarOneCell(ci);
             }, onProgress);
+            if (cellIds.length === 1)
+                $("#tpMetaNote").hide();
+            else {
+                $("#tpMetaNote").html("...and " + (cellIds.length - 1) + " other " + gSampleDesc + "s underneath");
+                $("#tpMetaNote").show();
+            }
         }
 
         updateGeneTableColors(cellIds);
 
-        if (ev === undefined) {
-            db.metaHist = null;
-        } else {
-            // it was a click -> we have at least one cell ID
-            let cellId = cellIds[0];
+        if (ev !== undefined) {
+            // it was a click
             if (!ev.shiftKey && !ev.ctrlKey && !ev.metaKey)
                 renderer.selectClear();
-            clearSelectionState();
             renderer.selectAdd(cellId);
             renderer.drawDots();
             event.stopPropagation();
         }
     }
 
-    function showTooltip(x, y, labelStr) {
-        $("#tpTooltip").css({
-            "display": "block",
-            "left": x,
-            "top": y,
-        }).html(labelStr);
-    }
-
-    function hideTooltip() {
-        $("#tpTooltip").hide();
-    }
-
-    function onClusterNameHover(clusterName, nameIdx, ev) {
+    function onClusterNameHover(clusterName, ev) {
         /* user hovers over cluster label */
-        var labelLines = [clusterName];
-
-        var labelField = db.conf.labelField;
-        var metaInfo = db.findMetaInfo(labelField);
-        var longLabels = metaInfo.ui.longLabels;
-        if (longLabels) {
-            for (let i = 0; i < longLabels.length; i++) {
-                let shortLabel = metaInfo.ui.shortLabels[i];
-                let longLabel = longLabels[i];
-                if (clusterName === shortLabel && longLabel !== shortLabel) {
-                    labelLines.push(longLabels[i]);
-                    break;
-                }
-            }
-        }
-
-        if (labelField == db.conf.activeLabelField) {
-            if (db.conf.topMarkers !== undefined) {
-                labelLines.push("Top enriched/depleted markers: " + db.conf.topMarkers[clusterName].join(", "));
-            }
-            labelLines.push("");
-
-            if (db.conf.markers !== undefined)
-                labelLines.push("Click to show full marker gene list.");
-
-            if (db.conf.clusterPngDir !== undefined) {
-                var fullPath = cbUtil.joinPaths([db.name, db.conf.clusterPngDir, clusterName + ".png"]);
-                labelLines.push("<img src='" + fullPath + "'>");
-            }
-        }
-
-        labelLines.push("Alt/Option-Click to select cluster; Shift-Click to add cluster to selection");
-        showTooltip(ev.clientX + 15, ev.clientY, labelLines.join("<br>"));
-    }
-
-    function onNoClusterNameHover(ev) {
-        hideTooltip();
+        //var htmls = [];
+        //htmls.push("<div class='tpHover'>"+clusterName+"</div>");
+        //$(document.body).append(htmls.join(""));
+        console.log("Hover over " + clusterName);
+        console.log(ev);
     }
 
     function sanitizeName(name) {
         /* ported from cellbrowser.py: remove non-alpha, allow underscores */
-        var newName = name.replace(/\+/g, "Plus").replace(/-/g, "Minus").replace(/%/g, "Perc");
-        var newName = newName.replace(/[^a-zA-Z_0-9+]/g, "");
-        return newName;
-    }
-
-    function onlyAlphaNum(name) {
-        /* only allow alphanumeric characters */
-        var newName = name.replace(/[^a-zA-Z0-9+]/g, "");
+        var newName = name.replace(/[^a-zA-Z_0-9+]/g, "");
         return newName;
     }
 
-    function onActRendChange(otherRend) {
-        /* called after the user has activated a view with a click */
-        renderer.legend = gLegend;
-        renderer = otherRend;
-        gLegend = otherRend.legend;
-        $("#tpLayoutCombo").val(otherRend.coordIdx).trigger('chosen:updated');
-        buildLegendBar();
-    }
-
-    function removeSplit(renderer) {
-        /* stop split screen mode */
-        if (!renderer)
-            return;
-        if (!renderer.childPlot && !renderer.parentPlot)
-            return;
-        if (!renderer.isMain) {
-            // make sure the left renderer is the active one
-            renderer.childPlot.activatePlot();
-        }
-        renderer.unsplit();
-        $("#tpSplitMenuEntry").text("Split Screen");
-    }
-
-    function onSplitClick() {
-        /* user clicked on View > Split Screen */
-        if (!renderer.childPlot && !renderer.parentPlot) {
-            // nothing is split yet -> start the split
-            renderer.onActiveChange = onActRendChange;
-
-            var currCoordIdx = $("#tpLayoutCombo").val();
-            renderer.legend = gLegend;
-            renderer.coordIdx = currCoordIdx; // keep for onActRendChange
-            renderer.isMain = true;
-
-            renderer.split();
-
-            renderer.childPlot.legend = gLegend;
-            renderer.childPlot.coordIdx = currCoordIdx; // keep for onActRendChange
-
-            $("#tpSplitMenuEntry").text("Unsplit Screen");
-            $("#mpCloseButton").click(renderer.unsplit);
-            //$("#mpCloseButton").click(onSplitClick);
-
-        } else {
-            removeSplit(renderer);
-        }
-        renderer.drawDots();
-    }
-
-    function groupAverages(geneArrs, arrGroups, groupCount) {
-        /* given an array of gene expression vectors (ints), and a 2nd array that assigns these to groups,
-        return an array of the arrays with the averages for the groups (as integers)
-        */
-        let geneAvgs = [];
-
-        for (let geneIdx = 0; geneIdx < geneArrs.length; geneIdx++) {
-            let geneArr = geneArrs[geneIdx];
-
-            let groupSums = new Uint32Array(groupCount);
-            let groupCounts = new Uint32Array(groupCount);
-            //for (var groupIdx=0; groupIdx < groupCount; groupIdx++) {
-            //    groupSums.push(0);
-            //    groupCounts.push(0);
-            //}
-
-            for (let i = 0; i < geneArr.length; i++) {
-                let group = arrGroups[i];
-                groupSums[group] += geneArr[i];
-                groupCounts[group]++;
-            }
-
-            let groupAvgs = [];
-            for (var groupIdx = 0; groupIdx < groupCount; groupIdx++)
-                groupAvgs.push(Math.round(groupSums[groupIdx] / groupCounts[groupIdx]));
-            geneAvgs.push(groupAvgs);
-
-        }
-        return geneAvgs;
-    }
-
-    function onHeatCellClick(geneName, clusterName) {
-        /* color by gene and select all cells in cluster */
-        colorByLocus(geneName);
-        // clusterName?
-        selectByColor
-    }
-
-    function onHeatCellHover(rowIdx, colIdx, rowName, colName, value, ev) {
-        /* user hovers over a cell on the heatmap */
-        let htmls = [];
-        if (rowName)
-            htmls.push(rowName);
-        if (colName)
-            htmls.push(colName)
-        if (value !== null)
-            htmls.push(" " + (value * 10) + "-" + ((value + 1) * 10) + "%");
-        showTooltip(ev.clientX + 15, ev.clientY, htmls.join(" "));
-    }
-
-    function plotHeatmap(clusterMetaInfo, exprVecs, geneSyms) {
-        /* Create the heatmap from exprVecs.
-         */
-        if (!geneSyms || geneSyms.length === 0) {
-            alert("No quick genes are defined. Heatmaps currently only work on pre-defined gene sets.");
-            return;
-        }
-
-        var clusterCount = clusterMetaInfo.valCounts.length;
-
-        var clusterNames = [];
-        for (let valInfo of clusterMetaInfo.valCounts) {
-            clusterNames.push(valInfo[0]); // 0=name, 1=count
-        }
-
-        var clusterArr = clusterMetaInfo.arr;
-        var geneAvgs = groupAverages(exprVecs, clusterArr, clusterCount);
-
-        var div = document.createElement("div");
-        //let heatHeight = Math.min(150, 16*exprVecs.length);
-        let heatHeight = parseInt(renderer.height * 0.5);
-        div.id = "tpHeat";
-        div.style.height = heatHeight + "px";
-
-        renderer.setSize(renderer.getWidth(), renderer.height - heatHeight, true);
-
-        var canvLeft = metaBarWidth + metaBarMargin;
-        var heatWidth = window.innerWidth - canvLeft - legendBarWidth;
-        // create the div for the heat map view
-        div.style.width = heatWidth + "px";
-        div.style.left = metaBarWidth + "px";
-        div.style.top = (menuBarHeight + toolBarHeight + renderer.height) + "px";
-        div.style.position = "absolute";
-        document.body.appendChild(div);
-
-        var heatmap = new MaxHeat(div, {
-            mainRenderer: renderer
-        });
-        //var colors = getFieldColors(clusterMetaInfo)
-        var colors = makeColorPalette(cDefGradPaletteHeat, 10);
-
-        heatmap.loadData(geneSyms, clusterNames, geneAvgs, colors);
-        heatmap.draw();
-        heatmap.onCellHover = onHeatCellHover;
-        heatmap.onClick = onHeatCellClick;
-        db.heatmap = heatmap;
-    }
-
-
-    function removeHeatmap() {
-        /* remove the heatmap */
-        let heatHeight = db.heatmap.height;
-        document.getElementById("tpHeat").remove();
-        delete db.heatmap;
-        renderer.setSize(renderer.getWidth(), renderer.height + heatHeight, true);
-        changeUrl({
-            'heat': null
-        });
-    }
-
-    function onHeatClick() {
-        // TODO: rewrite this one day with promises...
-        let resultCount = 0;
-        let exprVecs = [];
-        let geneSyms = [];
-        let metaInfo = null;
-
-        function partDone() {
-            resultCount++;
-            if (resultCount === 2)
-                plotHeatmap(metaInfo, exprVecs, geneSyms);
-        }
-
-        function onClusterMetaDone(metaArr, metaInfo) {
-            metaInfo.arr = metaArr;
-            partDone();
-        }
-
-        function onGenesDone(geneVecs) {
-            /* */
-            for (var geneInfo of geneVecs) {
-                geneSyms.push(geneInfo[0]); // gene symbol
-                exprVecs.push(geneInfo[1]); // binned expression vector
-            }
-            partDone();
-        }
-
-        /* user clicked on View > Heatmap */
-        if (db && db.heatmap) {
-            removeHeatmap();
-        } else {
-            if (!db.conf.quickGenes) {
-                alert("No quick genes defined for this dataset. Heatmaps currently only work if " +
-                    "a list of dataset-specific genes is defined. " +
-                    "Add a statement quickGenesFile to cellbrowser.conf and put a few gene symbols " +
-                    "into the file, one per line.");
-                return;
-            }
-            db.loadGeneSetExpr(onGenesDone);
-            metaInfo = getClusterFieldInfo();
-            db.loadMetaVec(metaInfo, onClusterMetaDone, onProgress);
-            changeUrl({
-                "heat": "1"
-            });
-        }
-    }
-
-    function onClusterNameClick(clusterName, _, event) {
+    function onClusterNameClick(clusterName) {
         /* build and open the dialog with the marker genes table for a given cluster */
-        var metaInfo = getClusterFieldInfo();
-        var isNumber = false;
-        var nameIdx = null;
-        if (metaInfo.type == "int" || metaInfo.type == "float") {
-            isNumber = true;
-        } else {
-            nameIdx = metaInfo.ui.shortLabels.indexOf(clusterName);
-        }
-        if (event.altKey || event.shiftKey) {
-            db.loadMetaVec(metaInfo, function(values) {
-                var clusterCells = [];
-                for (var i = 0, I = values.length; i < I; i++) {
-                    if (isNumber && metaInfo.origVals[i].toFixed(2) == clusterName) {
-                        clusterCells.push(i);
-                    } else if (!isNumber && values[i] == nameIdx) {
-                        clusterCells.push(i);
-                    }
-                }
-                if (event.altKey) {
-                    renderer.selectSet(clusterCells);
-                } else if (event.shiftKey) {
-                    var selection = renderer.getSelection();
-                    selection = selection.concat(clusterCells);
-                    renderer.selectSet(selection);
-                }
-                renderer.drawDots();
-            });
-            return;
-        }
-
-        // if current label field does not have markers, do nothing else
-        if (metaInfo.name != db.conf.activeLabelField) {
-            alert("There are no markers for this field");
-            return;
-        }
-
         var tabInfo = db.conf.markers; // list with (label, subdirectory)
 
         console.log("building marker genes window for " + clusterName);
         var htmls = [];
         htmls.push("<div id='tpPaneHeader' style='padding:0.4em 1em'>");
 
-        var buttons = [];
+        var buttons = {};
 
         if (tabInfo === undefined || tabInfo.length === 0) {
             tabInfo = [];
-            buttons.push({
-                text: "Close",
-                click: function() {
-                    $(this).dialog("close")
-                }
-            });
+            buttons["Close"] = function() {
+                $(this).dialog("close")
+            };
             htmls.push("No marker genes are available in this dataset. " +
                 "To add marker genes, contact the original authors of the dataset and ask them to add " +
                 " them to the cell browser.");
         } else {
             htmls.push("Click gene symbols below to color plot by gene<br>");
-            buttons.push({
-                text: "Download as file",
-                click: function() {
-                    document.location.href = markerTsvUrl;
-                }
-            });
+            buttons["Download as file"] = function() {
+                //url = joinPaths([baseUrl,"geneMatrix.tsv"]);
+                document.location.href = markerTsvUrl;
+            };
+
         }
         htmls.push("</div>");
 
         var doTabs = (tabInfo.length > 1);
 
+        //var hubUrl = db.conf.hubUrl;
+        //if (hubUrl!==undefined) {
+        //htmls.push("<p>");
+        //htmls.push("<a target=_blank class='link' href='"+hubUrl+"'>Show Sequencing Reads on UCSC Genome Browser</a><p>");
+        //}
+
         if (doTabs) {
             htmls.push("<div id='tabs'>");
             htmls.push("<ul>");
             for (var tabIdx = 0; tabIdx < tabInfo.length; tabIdx++) {
                 var tabLabel = tabInfo[tabIdx].shortLabel;
                 htmls.push("<li><a href='#tabs-" + tabIdx + "'>" + tabLabel + "</a>");
             }
             htmls.push("</ul>");
         }
 
-        for (let tabIdx = 0; tabIdx < tabInfo.length; tabIdx++) {
+        for (var tabIdx = 0; tabIdx < tabInfo.length; tabIdx++) {
             var divName = "tabs-" + tabIdx;
             var tabDir = tabInfo[tabIdx].name;
             var sanName = sanitizeName(clusterName);
-            var markerTsvUrl = cbUtil.joinPaths([db.name, "markers", tabDir, sanName + ".tsv.gz"]);
+            var markerTsvUrl = joinPaths([db.name, "markers", tabDir, sanName + ".tsv.gz"]);
             htmls.push("<div id='" + divName + "'>");
             htmls.push("Loading...");
             htmls.push("</div>");
 
             loadClusterTsv(markerTsvUrl, loadMarkersFromTsv, divName, clusterName);
         }
 
         htmls.push("</div>"); // tabs
 
         var winWidth = window.innerWidth - 0.10 * window.innerWidth;
         var winHeight = window.innerHeight - 0.10 * window.innerHeight;
         var title = "Cluster markers for &quot;" + clusterName + "&quot;";
-
-        var metaInfo = getClusterFieldInfo();
-        if (metaInfo.ui.longLabels) {
-            //var nameIdx = cbUtil.findIdxWhereEq(metaInfo.ui.shortLabels, 0, clusterName);
-            //var acronyms = db.conf.acronyms;
-            //title += " - "+acronyms[clusterName];
-            var longLabel = metaInfo.ui.longLabels[nameIdx];
-            if (clusterName !== longLabel)
-                title += " - " + metaInfo.ui.longLabels[nameIdx];
-        }
-
-        //if (acronyms!==undefined && clusterName in acronyms)
-        //title += " - "+acronyms[clusterName];
+        var acronyms = db.conf.acronyms;
+        if (acronyms !== undefined && clusterName in acronyms)
+            title += " - " + acronyms[clusterName];
         showDialogBox(htmls, title, {
             width: winWidth,
             height: winHeight,
             "buttons": buttons
         });
         $(".ui-widget-content").css("padding", "0");
         $("#tabs").tabs();
@@ -7573,15 +3892,14 @@
 
         htmls.push("<table class='table' id='tpMarkerTable'>");
         htmls.push("<thead>");
         var hprdCol = null;
         var geneListCol = null;
         var exprCol = null;
         var pValCol = null
-        //var doDescSort = false;
         for (var i = 1; i < headerRow.length; i++) {
             var colLabel = headerRow[i];
             var isNumber = false;
 
             if (colLabel.indexOf('|') > -1) {
                 var parts = colLabel.split("|");
                 colLabel = parts[0];
@@ -7590,19 +3908,17 @@
                     isNumber = true;
             }
 
             var width = null;
             if (colLabel === "_geneLists") {
                 colLabel = "Gene Lists";
                 geneListCol = i;
-            } else if (colLabel === "P_value" || colLabel === "p_val" || colLabel === "pVal") {
+            } else if (colLabel === "P_value" || colLabel === "p_val" || colLabel == "pVal") {
                 colLabel = "P-value";
                 pValCol = i;
-                //if (i===2)
-                //doDescSort = true;
             } else if (colLabel === "_expr") {
                 colLabel = "Expression";
                 exprCol = i;
             } else if (colLabel === "_hprdClass") {
                 hprdCol = i;
                 colLabel = "Protein Class (HPRD)";
                 width = "200px";
@@ -7612,37 +3928,31 @@
             if (isNumber)
                 addStr = " data-sort-method='number'";
 
             if (width === null)
                 htmls.push("<th" + addStr + ">");
             else
                 htmls.push("<th style='width:" + width + "'" + addStr + ">");
-            colLabel = colLabel.replace(/_/g, " ");
             htmls.push(colLabel);
             htmls.push("</th>");
         }
         htmls.push("</thead>");
 
         var hubUrl = makeHubUrl();
 
         htmls.push("<tbody>");
-        for (let i = 1; i < rows.length; i++) {
+        for (var i = 1; i < rows.length; i++) {
             var row = rows[i];
             if ((row.length === 1) && row[0] === "") // papaparse sometimes adds empty lines to files
                 continue;
 
             htmls.push("<tr>");
             var geneId = row[0];
-
-            // old marker files still have the format geneId|sym, so tolerate this here
-            if (geneId.indexOf("|") > -1)
-                geneId = geneId.split("|")[0];
-
             var geneSym = row[1];
-            htmls.push("<td><a data-gene='" + geneId + "' class='link tpLoadGeneLink'>" + geneSym + "</a>");
+            htmls.push("<td><a data-gene='" + geneSym + "' class='link tpLoadGeneLink'>" + geneSym + "</a>");
             if (hubUrl !== null) {
                 var fullHubUrl = hubUrl + "&position=" + geneSym + "&singleSearch=knownCanonical";
                 htmls.push("<a target=_blank class='link' style='margin-left: 10px; font-size:80%; color:#AAA' title='link to UCSC Genome Browser' href='" + fullHubUrl + "'>Genome</a>");
             }
             htmls.push("</td>");
 
             for (var j = 2; j < row.length; j++) {
@@ -7654,74 +3964,59 @@
                     var imgUrl = val.replace("./", db.url + "/");
                     var imgHtml = '<img width="100px" src="' + imgUrl + '">';
                     val = "<a data-toggle='tooltip' data-placement='auto' class='tpPlots link' target=_blank title='" + imgHtml + "' href='" + imgUrl + "'>plot</a>";
                 }
                 if (j === geneListCol || j === exprCol)
                     geneListFormat(htmls, val, geneSym);
                 else if (j === pValCol)
-                    htmls.push(parseFloat(val).toPrecision(5)); // five digits ought to be enough for everyone
+                    htmls.push(parseFloat(val).toFixed(4)); // four digits ought to be enough for everyone
                 else
                     htmls.push(val);
                 htmls.push("</td>");
             }
             htmls.push("</tr>");
         }
 
         htmls.push("</tbody>");
         htmls.push("</table>");
 
-        // sub function ----
         function onMarkerGeneClick(ev) {
             /* user clicks onto a gene in the table of the marker gene dialog window */
-            var geneIdOrSym = ev.target.getAttribute("data-gene");
-
-            // old marker tables do not contain the geneIds. For these we need to resolve the symbol to an ID
-            if (!db.isAtacMode() && db.geneOffsets[geneIdOrSym] === undefined) {
-                var geneIds = db.findGenesExact(geneIdOrSym);
-                if (geneIds.length !== 1)
-                    alert("symbol " + geneIdOrSym + " resolves to more than one geneId. Internal error? Please contact us at cells@ucsc.edu");
-                geneIdOrSym = geneIds[0];
-            }
-
+            var geneSym = ev.target.getAttribute("data-gene");
             $(".ui-dialog").remove(); // close marker dialog box
             if (selectOnClick) {
-                clusterField = db.conf.labelField;
+                var clusterField = db.conf.labelField;
                 var queryList = [{
                     'm': clusterField,
                     'eq': clusterName
                 }];
                 findCellsMatchingQueryList(queryList, function(cellIds) {
                     renderer.selectSet(cellIds);
                     //changeUrl({'select':JSON.stringify(queryList)});
                 });
             }
-
-            // the marker table historically only contains symbols (this was a mistake)
-            // colorByLocus will automatically resolve them to IDs.
-            colorByLocus(geneIdOrSym);
+            loadGeneAndColor(geneSym);
         }
-        // ----
 
         $("#" + divId).html(htmls.join(""));
-        var sortOpt = {};
-        //if (doDescSort)
-        //sortOpt.descending=true;
         new Tablesort(document.getElementById('tpMarkerTable'));
         $(".tpLoadGeneLink").on("click", onMarkerGeneClick);
         activateTooltip(".link");
 
         var ttOpt = {
             "html": true,
             "animation": false,
             "delay": {
                 "show": 100,
                 "hide": 100
             }
         };
         $(".tpPlots").bsTooltip(ttOpt);
+
+        removeFocus();
     }
 
     var digitTest = /^\d+$/,
         keyBreaker = /([^\[\]]+)|(\[\])/g,
         plus = /\+/g,
         paramTest = /([^?#]*)(#.*)?$/;
 
@@ -7736,34 +4031,33 @@
             current;
 
         for (var i = 0; i < pairs.length; i++) {
             current = data;
             var pair = pairs[i].split('=');
 
             // if we find foo=1+1=2
-            if (pair.length !== 2) {
-                pair = [pair[0], pair.slice(1).join("=")];
+            if (pair.length != 2) {
+                pair = [pair[0], pair.slice(1).join("=")]
             }
 
             var key = decodeURIComponent(pair[0].replace(plus, " ")),
                 value = decodeURIComponent(pair[1].replace(plus, " ")),
                 parts = key.match(keyBreaker);
 
             for (var j = 0; j < parts.length - 1; j++) {
                 var part = parts[j];
                 if (!current[part]) {
                     // if what we are pointing to looks like an array
-                    current[part] = digitTest.test(parts[j + 1]) || parts[j + 1] === "[]" ? [] : {};
+                    current[part] = digitTest.test(parts[j + 1]) || parts[j + 1] == "[]" ? [] : {}
                 }
                 current = current[part];
-
             }
             var lastPart = parts[parts.length - 1];
-            if (lastPart === "[]") {
-                current.push(value);
+            if (lastPart == "[]") {
+                current.push(value)
             } else {
                 current[lastPart] = value;
             }
         }
         return data;
     }
 
@@ -7771,89 +4065,61 @@
         /* push the variables (object) into the history as the current URL. key=null deletes a variable. */
         // first get the current variables from the URL of the window
         var myUrl = window.location.href;
         myUrl = myUrl.replace("#", "");
         var urlParts = myUrl.split("?");
         var baseUrl = urlParts[0];
 
-        let urlVars;
         if (oldVars === undefined) {
             var queryStr = urlParts[1];
-            urlVars = deparam(queryStr); // parse key=val&... string to object
+            var urlVars = deparam(queryStr); // parse key=val&... string to object
         } else {
-            urlVars = oldVars;
+            urlVars = oldVars
         }
 
         // overwrite everthing that we got
         for (var key in vars) {
             var val = vars[key];
-            if (val === null || val === "") {
-                if (key in urlVars)
-                    delete urlVars[key];
-            } else
+            if (val === null || val in urlVars)
+                delete urlVars[key];
+            else
                 urlVars[key] = val;
         }
 
         var argStr = jQuery.param(urlVars); // convert to query-like string
-        argStr = argStr.replace(/%20/g, "+");
-
-        var dsName = "noname";
-        if (db !== null)
-            dsName = db.getName();
-
-        if (argStr.length > 1000)
-            warn("Cannot save current changes to the URL, the URL would be too long. " +
-                "You can try to shorten some cluster labels to work around the problem temporarily. " +
-                "But please contact us at cells@ucsc.edu and tell us about the error. Thanks!");
-        else
-            history.pushState({}, dsName, baseUrl + "?" + argStr);
-    }
-
-    function delVars(varNames) {
-        /* remove a CGI variable from the URL */
-        var o = {};
-        for (var varName of varNames)
-            o[varName] = null;
-        changeUrl(o);
+        history.pushState({}, db.getName(), baseUrl + "?" + argStr);
     }
 
     function delState(varName) {
         /* remove a CGI variable from the URL */
         var o = {};
         o[varName] = null;
         changeUrl(o);
     }
 
     function addStateVar(varName, varVal) {
-        /* add a CGI variable to the URL */
+        /* add a CGI variable from the URL */
         var o = {};
         o[varName] = varVal;
         changeUrl(o);
     }
 
     function getVar(name, defVal) {
         /* get query variable from current URL or default value if undefined */
         var myUrl = window.location.href;
-        myUrl = myUrl.split("#")[0]; // remove anchor from URL
+        myUrl = myUrl.replace("#", "");
         var urlParts = myUrl.split("?");
         var queryStr = urlParts[1];
         var varDict = deparam(queryStr); // parse key=val&... string to object
         if (varDict[name] === undefined)
             return defVal;
         else
             return varDict[name];
     }
 
-    function getVarSafe(name, defVal) {
-        let val = getVar(name, defVal);
-        if (val)
-            val = val.replace(/\W/g, '');
-        return val;
-    }
-
     function pushZoomState(zoomRange) {
         /* write the current zoom range to the URL. Null to remove it from the URL. */
         if (zoomRange === null)
             changeUrl({
                 zoom: null
             });
         else
@@ -7864,15 +4130,15 @@
 
     function getZoomRangeFromUrl() {
         /* return a zoomRange object based on current URL */
         var zoomStr = getVar("zoom", null);
         if (zoomStr === null)
             return null;
         var zs = zoomStr.split("_");
-        if (zs.length !== 4)
+        if (zs.length != 4)
             return null;
         var zoomRange = {};
         zoomRange.minX = parseFloat(zs[0]);
         zoomRange.maxX = parseFloat(zs[1]);
         zoomRange.minY = parseFloat(zs[2]);
         zoomRange.maxY = parseFloat(zs[3]);
         return zoomRange;
@@ -7900,96 +4166,88 @@
                 window.location.replace(newUrl);
                 return true;
             }
             return false;
         }
     }
 
-    function getDatasetNameFromUrl() {
+    function extractDatasetFromUrl() {
         /* search for the "ds" parameter or a DNS hostname that indicates the dataset */
         // if ds=xxx was found in the URL, load the respective dataset
         var datasetName = getVar("ds");
-        if (datasetName)
-            datasetName = datasetName.replace(/ /g, "/"); // + is easier to type than %23
 
-        if (datasetName === undefined)
-            datasetName = "";
+        //if (datasetName===undefined)
+        //datasetName = datasetList[0].name;
         // hacks for July 2018 and for backwards compatibility with previous version
-        else if (datasetName === "autism10X" || datasetName === "autism10x")
+        if (datasetName === "autism10X" || datasetName === "autism10x")
             datasetName = "autism";
-        else if (datasetName === "aparna")
+        if (datasetName === "aparna")
             datasetName = "cortex-dev";
-        else if (datasetName && datasetName.toLowerCase() === "adultpancreas")
-            datasetName = "adultPancreas"
-        else
-            // adult pancreas is the only dataset with an uppercase letter
-            // make sure that at least at UCSC, dataset names are always lowercased.
-            // The reason is that at UCSC, the datasetname can be part of the URL as a hostname,
-            // e.g. cortex-dev.cells.ucsc.edu, which the user could enter as CoRTex-dev.cells.ucsc.edu
-            // On all other servers, this is not an issue
-            // (But never do this for subdatasets, because they often include uppercase letters and are not
-            // in the URL hostname part)
-            if (datasetName && pageAtUcsc() && datasetName.indexOf("/") === -1)
-                datasetName = datasetName.toLowerCase();
         return datasetName;
     }
 
     /* ==== MAIN ==== ENTRY FUNCTION */
-    function main(rootMd5) {
-        /* start the data loaders, show first dataset. If in  */
+    function loadData(datasetList, globalOpts) {
+        /* start the data loaders, show first dataset */
         if (redirectIfSubdomain())
             return;
+        gDatasetList = datasetList;
+
+        if (globalOpts != undefined) {
+            if ("sampleType" in globalOpts)
+                gSampleDesc = globalOpts["sampleType"];
+            if ("title" in globalOpts)
+                gTitle = globalOpts["title"];
+        }
 
         setupKeyboard();
         buildMenuBar();
 
-        var datasetName = getDatasetNameFromUrl()
-        // pre-load dataset.json here?
+        var datasetName = extractDatasetFromUrl(datasetList)
+
+        //menuBarHide("#tpShowAllButton");
+
         menuBarHeight = $('#tpMenuBar').outerHeight(true);
 
         var canvLeft = metaBarWidth + metaBarMargin;
         var canvTop = menuBarHeight + toolBarHeight;
         var canvWidth = window.innerWidth - canvLeft - legendBarWidth;
         var canvHeight = window.innerHeight - menuBarHeight - toolBarHeight;
 
         if (renderer === null) {
             var div = document.createElement('div');
             div.id = "tpMaxPlot";
             renderer = new MaxPlot(div, canvTop, canvLeft, canvWidth, canvHeight);
             document.body.appendChild(div);
-            activateTooltip(".mpButton"); // tpMaxPlot has no special tooltip support itself
-
-            self.tooltipDiv = makeTooltipCont();
-            document.body.appendChild(self.tooltipDiv);
         }
 
         buildEmptyLegendBar(metaBarWidth + metaBarMargin + renderer.width, toolBarHeight);
 
         renderer.setupMouse();
         $(window).resize(onWindowResize);
 
         renderer.onLabelClick = onClusterNameClick;
         renderer.onLabelHover = onClusterNameHover;
-        renderer.onNoLabelHover = onNoClusterNameHover;
         renderer.onCellClick = onCellClickOrHover;
         renderer.onCellHover = onCellClickOrHover;
         renderer.onNoCellHover = clearMetaAndGene;
         renderer.onZoom100Click = onZoom100Click;
         renderer.onSelChange = onSelChange;
-        renderer.canvas.addEventListener("mouseleave", hideTooltip);
 
-        loadDataset(datasetName, false, rootMd5);
+        if (datasetName === undefined)
+            openDatasetDialog();
+        else
+            loadDataset(datasetName, false);
+
     }
 
     // only export these functions
     return {
-        "main": main
+        "loadData": loadData
     }
 
 }();
 
-
-
 function _tpReset() {
     /* for debugging: reset the intro setting */
     localStorage.removeItem("introShown");
 }
```

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/cbWeb/js/maxPlot.js` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/cbWeb/js/maxPlot.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -1,228 +1,168 @@
 'use strict';
 // maxPlot: a fast scatter plot class
 /*jshint globalstrict: true*/
-/*jshint -W069 */
-/*jshint -W104 */
-/*jshint -W117 */
 
 // TODO:
+// remove onNoHover
 // fix mouseout into body -> marquee stays
+// fix the aspect ratio of the zoom marquee
 
 function getAttr(obj, attrName, def) {
     var val = obj[attrName];
     if (val === undefined)
         return def;
     else
         return val;
 }
 
 function cloneObj(d) {
-    /* returns a deep copy of an object, wasteful and destroys old references */
+    /* returns a copy of an object, wasteful */
     // see http://stackoverflow.com/questions/122102/what-is-the-most-efficient-way-to-deep-clone-an-object-in-javascript
     return JSON.parse(JSON.stringify(d));
 }
 
-function copyObj(src, trg) {
-    /* object copying: copies all values from src to trg */
-    var key;
-    for (key in src) {
-        trg[key] = src[key]; // copies each property to the objCopy object
-    }
-}
-
-function debug(msg) {
-    if (window.doDebug)
-        console.log(msg);
-}
 
 function MaxPlot(div, top, left, width, height, args) {
     // a class that draws circles onto a canvas, like a scatter plot
     // div is a div DOM element under which the canvas will be created
     // top, left: position in pixels, integers
     // width and height: integers, in pixels, includes the status line
 
-    const HIDCOORD = 12345; // magic value for missing coordinates
-    // In rare instances, coordinates are saved but should not be shown. This way of implementing hiding
-    // may look hacky, but it simplifies the logic and improves performance.
-
-    // export this special value so other part of the code can use it
-    this.hiddenCoord = HIDCOORD;
-
-    var self = this; // 'this' has two conflicting meanings in javascript.
+    var self = this; // 'this' has two conflicting meanings in javascript. 
     // I use 'self' to refer to object variables, so I can use 'this' to refer to the caller context
 
     const gTextSize = 16; // size of cluster labels
     const gTitleSize = 18; // size of title text
-    const gStatusHeight = 14; // height of status bar
+    const gStatusHeight = 12; // height of status bar
     const gZoomButtonSize = 30; // size of zoom buttons
-    const gZoomFromLeft = 10; // position of zoom buttons from left
-    const gZoomFromBottom = 140; // position of zoom buttons from bottom
-    const gButtonBackground = "rgb(230, 230, 230, 0.85)" // grey level of buttons
+    const gZoomFromRight = 60; // position of zoom buttons from right
+    const gZoomFromBottom = 120; // position of zoom buttons from bottom
+    const gButtonBackground = "rgb(230, 230, 230, 0.6)" // grey level of buttons
     const gButtonBackgroundClicked = "rgb(180, 180, 180, 0.6)"; // grey of buttons when clicked
-    const gCloseButtonFromRight = 60; // distance of "close" button from right edge
 
     // the rest of the initialization is done at the end of this file,
     // because the init involves many functions that are not defined yet here
 
     this.initCanvas = function(div, top, left, width, height) {
         /* initialize a new Canvas */
 
-        div.style.top = top + "px";
-        div.style.left = left + "px";
-        div.style.position = "absolute";
-        div.style.display = "block";
         self.div = div;
-
         self.gSampleDescription = "cell";
         self.ctx = null; // the canvas context
         self.canvas = addCanvasToDiv(div, top, left, width, height - gStatusHeight);
 
-        self.interact = false;
-
-        if (args && args.showClose === true) {
-            self.closeButton = addChildControls(10, width - gCloseButtonFromRight);
-        }
-
-        if (args === undefined || (args["interact"] !== false)) {
-            self.interact = true;
-
-            addZoomButtons(height - gZoomFromBottom, gZoomFromLeft, self);
-            addModeButtons(10, 10, self);
-            addStatusLine(height - gStatusHeight, left, width, gStatusHeight);
-            addTitleDiv(height - gTitleSize - gStatusHeight - 4, 8);
-
-            /* add the div used for the mouse selection/zoom rectangle to the DOM */
-            var selectDiv = document.createElement('div');
-            selectDiv.id = "mpSelectBox";
-            selectDiv.style.border = "1px dotted black";
-            selectDiv.style.position = "absolute";
-            selectDiv.style.display = "none";
-            selectDiv.style.pointerEvents = "none";
-            self.div.appendChild(selectDiv);
-
-            // callbacks when user clicks or hovers over label or cell
-            self.onLabelClick = null; // called on label click, args: text of label and event
-            self.onCellClick = null; // called on cell click, args: array of cellIds and event
-            self.onCellHover = null; // called on cell hover, arg: array of cellIds
-            self.onNoCellHover = null; // called on hover over empty background
-            self.onSelChange = null; // called when the selection has been changed, arg: array of cell Ids
-            self.onLabelHover = null; // called when mouse hovers over a label
-            self.onNoLabelHover = null; // called when mouse does not hover over a label
-            // self.onZoom100Click: called when user clicks the zoom100 button. Implemented below.
-            self.selectBox = selectDiv; // we need this later
-            self.setupMouse();
-
-            // connected plots
-            self.childPlot = null; // plot that is syncing from us, see split()
-            self.parentPlot = null; // plot that syncs to us, see split()
-        }
-
+        addZoomButtons(top + height - gZoomFromBottom, left + width - gZoomFromRight, self);
+        addModeButtons(top + 10, left + 10, self);
+        addStatusLine(top + height - gStatusHeight, left, width, gStatusHeight);
         addProgressBars(top + Math.round(height * 0.3), left + 30);
+        addTitleDiv(top + height - gTitleSize - gStatusHeight, left + 5);
+
+        /* add the div used for the mouse selection/zoom rectangle to the DOM */
+        var selectDiv = document.createElement('div');
+        selectDiv.id = "mpSelectBox";
+        selectDiv.style.border = "1px dotted black";
+        selectDiv.style.position = "absolute";
+        selectDiv.style.display = "none";
+        selectDiv.pointerEvents = "none";
+        self.div.appendChild(selectDiv);
+        self.selectBox = selectDiv; // we need this later
+
+        self.setupMouse();
+
+        // callbacks when user clicks or hovers over label or cell 
+        self.onLabelClick = null; // called on label click, args: text of label and event
+        self.onCellClick = null; // called on cell click, args: array of cellIds and event
+        self.onCellHover = null; // called on cell hover, arg: array of cellIds
+        self.onNoCellHover = null; // called on hover over empty background
+        self.onSelChange = null; // called when the selection has been changed, arg: array of cell Ids
+        // self.onZoom100Click: called when user clicks the zoom100 button. Implemented below.
 
         // timer that is reset on every mouse move
         self.timer = null;
-    }
-
-    function isHidden(x, y) {
-        /* special coords are used for circles that are off-screen or otherwise not visible */
-        return ((x === HIDCOORD && y === HIDCOORD)) // not shown (e.g. no coordinate or off-screen)
-    }
 
-    this.initPort = function(args) {
-        /* init all viewport related state (zoom, radius, alpha) */
-        self.port = {};
-        self.port.zoomRange = {}; // object with keys minX, , maxX, minY, maxY, in data units
-        self.port.radius = getAttr(args, "radius", null); // current radius of the circles, 0=one pixel dots
+        // all other object variables are added by the "initPlot(args)" function below
 
-        // we keep a copy of the 'initial' arguments at 100% zoom
-        self.port.initZoom = {};
-        self.port.initRadius = self.port.radius; // circle radius at full zoom
-        self.port.initAlpha = getAttr(args, "alpha", 0.3);
-    };
+        // when the user starts to select but lifts the mouse button outside
+        // the canvas, the current selection must be reset
+        //self.canvas.addEventListener("mouseleave", function() {self.resetMarquee();});
+
+        //document.body.addEventListener("mouseup", function(evt) {
+        //var targetId = evt.target.id;
+        //console.log("mouseup on body");
+        //if(targetId !== "mpCanvas" && targetId!=="mpSelectBox") {  // do nothing on the canvas
+        //console.log("mouseup outside of canvas, resetting marquee");
+        //self.resetMarquee();
+        //evt.stopPropagation();
+        //}
+        //});
+        // for this to work, the body has to really cover the whole page
+        //document.body.style.height = "100vh";
+    }
 
     this.initPlot = function(args) {
         /* create a new scatter plot on the canvas */
         if (args === undefined)
             args = {};
 
-        self.scalingDone = false;
-
-        self.globalOpts = args;
-
         self.mode = 1; // drawing mode
 
-        // everything related to circle coordinates
-        self.coords = {};
-        self.coords.orig = null; // coordinates of cells in original coordinates
-        self.coords.labels = null; // cluster label positions in pixels, array of [x,y,text]
+        self.zoomRange = null; // object with keys minX, , maxX, minY, maxY
+        self.coords = null;
+        self.clusterLabels = null; // cluster labels, array of [x,y,text]
+
+        self.pxCoords = null; // coordinates of cells as screen pixels or 0,0 if not shown
+        self.pxLabels = null; // cluster labels in pixels, array of [x,y,text] 
+        self.pxLabelBbox = null; // cluster label bounding boxes, array of [x1,x2,x2,y2]
 
-        self.coords.px = null; // coordinates of cells and labels as screen pixels or (HIDCOORD,HIDCOORD) if not shown
-        self.coords.labelBbox = null; // cluster label bounding boxes, array of [x1,x2,x2,y2]
-
-
-        self.col = {};
-        self.col.pal = null; // list of six-digit hex codes
-        self.col.arr = null; // length is coords.px/2, one byte per cell = index into self.col.pal
+        self.doDrawLabels = true; // should cluster labels be drawn?
 
-        self.selCells = new Set(); // IDs of cells that are selected (drawn in black)
+        self.colors = null; // list of six-digit hex codes
+        self.colorArr = null; // length is pxCoords/2, one byte per cell = index into self.colors
+        self.radius = getAttr(args, "radius", null); // current radius of the circles, 0=one pixel dots
+        self.alpha = getAttr(args, "alpha", 0.3);
+        self.selCells = null; // IDs of cells that are "selected" and as such highlighted in some way
 
-        self.doDrawLabels = true; // should cluster labels be drawn?
-        self.initPort(args);
+        // we keep a copy of the 'initial' arguments at 100% zoom
+        self.initZoom = cloneObj(self.zoomRange);
+        self.initRadius = self.radius; // circle radius at full zoom
 
         // mouse drag is modal: can be "select", "move" or "zoom"
         self.dragMode = "select";
 
         // for zooming and panning
         self.mouseDownX = null;
         self.mouseDownY = null;
         self.panCopy = null;
 
         // to detect if user just clicked on a dot
         self.dotClickX = null;
         self.dotClickY = null;
 
-        // the background image for spatial mode
-        self.background = null;
-
         self.activateMode(getAttr(args, "mode", "move"));
     };
 
     // call the constructor
     //self.newObject(div, top, left, width, height, args);
 
     this.clear = function() {
-        clearCanvas(self.ctx, self.canvas.width, self.canvas.height);
+        clearCanvas(self.ctx, self.width, self.height);
     };
 
-    //this.setPos = function(left, top) {
-    /* position the canvas on the page */
-    //self.div.style.left = left+"px";
-    //self.div.style.top = top+"px";
-    //};
+    this.setPos = function(left, top) {
+        /* position the canvas on the page */
+        self.canvas.style.left = left + "px";
+        self.canvas.style.top = top + "px";
+    };
 
     this.setTitle = function(text) {
         self.title = text;
         self.titleDiv.innerHTML = text;
     };
 
-    this.setWatermark = function(text) {
-        if (text === "") {
-            //var elem = gebi("tpWatermark");
-            self.watermark.parentNode.removeChild(self.watermark);
-            self.watermark = undefined;
-        } else {
-            var elem = document.createElement('div');
-            elem.id = "tpWatermark";
-            elem.style.cssText = 'pointer-events: none;position: absolute; width: 1000px; opacity: 0.3; z-index: 1000; top: 100px; left: 100px; text-align: left; vertical-align: top; color: black; font-size: xx-large;';
-            elem.textContent = text;
-            gebi("tpMaxPlot").appendChild(elem);
-            self.watermark = elem;
-        }
-    }
 
     // -- (private) helper functions
     // -- these are normal functions, not methods, they do not access "self"
 
     function gebi(idStr) {
         return document.getElementById(idStr);
     }
@@ -231,15 +171,15 @@
         var el = gebi(idStr);
         if (el !== null) {
             el.parentNode.removeChild(el);
         }
     }
 
     function activateTooltip(selector) {
-        /* uses bootstrap tooltip. Use noconflict in html, I had to rename BS's tooltip to avoid overwrite by jquery
+        /* uses bootstrap tooltip. Use noconflict in html, I had to rename BS's tooltip to avoid overwrite by jquery 
          */
         if (window.jQuery && $.fn.bsTooltip !== undefined) {
             var ttOpt = {
                 "html": true,
                 "animation": false,
                 "delay": {
                     "show": 400,
@@ -259,21 +199,20 @@
             return 2;
         else if (coordCount > 4000)
             return 4;
         else
             return 5;
     }
 
-    function createButton(width, height, id, title, text, imgFname, paddingTop, paddingBottom, addSep, addThickSep) {
-        /* make a light-grey div that behaves like a button, with text and/or an image on it
+    function createButton(width, height, id, title, text, imgFname, paddingTop, addSep) {
+        /* make a light-grey div that behaves like a button, with text and/or an image on it 
          * Images are hard to vertically center, so padding top can be specified.
          * */
         var div = document.createElement('div');
         div.id = id;
-        div.className = "mpButton";
         div.style.backgroundColor = gButtonBackground;
         div.style.width = width + "px";
         div.style.height = height + "px";
         div.style["text-align"] = "center";
         div.style["vertical-align"] = "middle";
         div.style["line-height"] = height + "px";
         if (text !== null)
@@ -284,29 +223,23 @@
         div.style["font-weight"] = "bold";
         div.style["font-family"] = "sans-serif";
 
         if (title !== null)
             div.title = title;
         if (text !== null)
             div.textContent = text;
-        if (imgFname !== null && imgFname !== undefined) {
+        if (imgFname !== null && imgFname != undefined) {
             var img = document.createElement('img');
             img.src = imgFname;
-            if (paddingTop !== null && paddingTop !== undefined) {
+            if (paddingTop !== null && paddingTop != undefined)
                 img.style.paddingTop = paddingTop + "px";
-                if (paddingBottom)
-                    img.style.paddingBottom = paddingBottom + "px";
-            }
             div.appendChild(img);
         }
         if (addSep === true)
             div.style["border-bottom"] = "1px solid #D7D7D7";
-        if (addThickSep === true)
-            div.style["border-bottom"] = "2px solid #C7C7C7";
-
 
         // make color dark grey when mouse is pressed
         div.addEventListener("mousedown", function() {
             this.style.backgroundColor = gButtonBackgroundClicked;
         });
 
         div.addEventListener("mouseup", function() {
@@ -332,27 +265,26 @@
     }
 
     function addZoomButtons(top, left, self) {
         /* add the plus/minus buttons to the DOM and place at position x,y on the screen */
         var width = gZoomButtonSize;
         var height = gZoomButtonSize;
 
-        var plusDiv = createButton(width, height, "mpCtrlZoomPlus", "Zoom in. Keyboard: +", "+", null, null, null, true);
+        var plusDiv = createButton(width, height, "mpCtrlZoomPlus", "Zoom in", "+", null, null, true);
         //plusDiv.style["border-bottom"] = "1px solid #D7D7D7";
 
-        var fullDiv = createButton(width, height, "mpCtrlZoom100", "Zoom in. Keyboard: space", "100%", null, null, null, true);
+        var fullDiv = createButton(width, height, "mpCtrlZoom100", "Zoom in", "100%", null, null, true);
         //full.style["border-bottom"] = "1px solid #D7D7D7";
 
-        var minusDiv = createButton(width, height, "mpCtrlZoomMinus", "Zoom out. Keyboard: -", "-");
+        var minusDiv = createButton(width, height, "mpCtrlZoomMinus", "Zoom out", "-");
 
         var ctrlDiv = makeCtrlContainer(top, left);
         ctrlDiv.appendChild(plusDiv);
         ctrlDiv.appendChild(fullDiv);
         ctrlDiv.appendChild(minusDiv);
-        self.zoomDiv = ctrlDiv;
 
         self.div.appendChild(ctrlDiv);
 
         minusDiv.addEventListener('click', function() {
             self.zoomBy(0.75);
             self.drawDots();
         });
@@ -363,73 +295,70 @@
         plusDiv.addEventListener('click', function() {
             self.zoomBy(1.333);
             self.drawDots();
         });
     }
 
     function addTitleDiv(top, left) {
-        var div = document.createElement('div');
-        div.className = "tpTitle";
-        div.style.top = top + "px";
-        div.style.left = left + "px";
-        div.style.fontSize = gTitleSize;
-        div.id = 'mpTitle';
-        self.div.appendChild(div);
-        self.titleDiv = div;
-    }
-
-    function addCloseButton(top, left) {
-        /* add close button and sync checkbox */
+        //var ctx = self.ctx;
+        //ctx.save();
+        //ctx.font = "bold "+gTextSize+"px Sans-serif"
+        //ctx.fillStyle = "rgba(220, 220, 220)";
+        //ctx.textBaseline = "top";
+        //ctx.fillText(self.title,5,self.height - gTextSize - 3); 
+        //ctx.restore();
         var div = document.createElement('div');
         div.style.cursor = "default";
         div.style.left = left + "px";
         div.style.top = top + "px";
         div.style.display = "block";
         div.style.position = "absolute";
         div.style.fontSize = gTitleSize;
-        div.style.padding = "3px";
-        div.style.borderRadius = "3px";
-        div.style.border = "1px solid #c5c5c5";
-        div.style.backgroundColor = "#f6f6f6";
-        div.style.color = "#454545";
-        div.id = 'mpCloseButton';
-        div.textContent = "Close";
+        div.id = 'mpTitle';
+        //div.innerHTML = title;
+        div.style['color'] = "lightgrey";
         self.div.appendChild(div);
-        return div;
-    }
-
-    function addChildControls(top, left) {
-        addCloseButton(top, left);
+        self.titleDiv = div;
     }
 
     function appendButton(parentDiv, id, title, imgName) {
         /* add a div styled like a button under div */
         var div = document.createElement('div');
         div.title = title;
         div.id = id;
 
     }
 
     function addModeButtons(top, left, self) {
         /* add the zoom/move/select control buttons to the DOM */
+        //var htmls = [];
+        //htmls.push('<div id="mpIcons" style="display:inline-block">');
+        //htmls.push('<div style="vertical-align:top">');
+        //htmls.push('<div title="Select mode.<br>Keyboard: shift or s" id="mpIconModeSelect"><img src="img/select.png"></button>');
+        //htmls.push('<div title="Zoom-to-rectangle mode. Keyboard: Windows/Command or z" id="mpIconModeZoom" style="display: block; margin-right:0"><img src="img/zoom.png"></button>');
+        //htmls.push('<div data-placement="bottom" title="Move mode. Keyboard: Alt or m" id="mpIconModeMove" data-toggle="tooltip" class="ui-button tpIconButton" class="mpModeButton" style="margin-right:0"><img src="img/move.png"></button>');
+        //htmls.push('</div>');
+        //htmls.push('<button title="Zoom to 100%, showing all data, keyboard: space" data-placement="bottom" data-toggle="tooltip" id="mpZoom100Button" class="ui-button tpIconButton" style="font-size:10px; font-weight: bold; margin-top: 4px; margin-right:0; display:block; padding:0">100%</button>');
+        //<img style="width:22px; height:22px" src="img/center.png">
+
         var ctrlDiv = makeCtrlContainer(top, left);
 
         var bSize = gZoomButtonSize;
 
-        var selectButton = createButton(bSize, bSize, "mpIconModeSelect", "Select mode. Keyboard: shift or s", null, "img/select.png", 0, 4, true, true);
+        var selectButton = createButton(bSize, bSize, "mpIconModeSelect", "Select mode. Keyboard: shift or s", null, "img/select.png", 4, true);
         selectButton.addEventListener('click', function() {
             self.activateMode("select")
         }, false);
 
-        var zoomButton = createButton(bSize, bSize, "mpIconModeZoom", "Zoom-to-rectangle mode. Keyboard: Windows/Command or z", null, "img/zoom.png", 4, 4, true);
+        var zoomButton = createButton(bSize, bSize, "mpIconModeZoom", "Zoom-to-rectangle mode. Keyboard: Windows/Command or z", null, "img/zoom.png", 4, true);
         zoomButton.addEventListener('click', function() {
             self.activateMode("zoom")
         }, false);
 
-        var moveButton = createButton(bSize, bSize, "mpIconModeMove", "Move mode. Keyboard: Alt or m", null, "img/move.png", 4, 4);
+        var moveButton = createButton(bSize, bSize, "mpIconModeMove", "Move mode. Keyboard: Alt or m", null, "img/move.png", 4);
         moveButton.addEventListener('click', function() {
             self.activateMode("move");
         }, false);
 
         self.icons = {};
         self.icons["move"] = moveButton;
         self.icons["select"] = selectButton;
@@ -437,37 +366,43 @@
 
         //ctrlDiv.innerHTML = htmls.join("");
         ctrlDiv.appendChild(moveButton);
         ctrlDiv.appendChild(selectButton);
         ctrlDiv.appendChild(zoomButton);
 
         self.div.appendChild(ctrlDiv);
-        self.toolDiv = ctrlDiv;
 
         activateTooltip('.mpIconButton');
+
+        //gebi('mpZoom100Button').addEventListener ('click', function(ev) { return self.onZoom100Click(ev) } );
     }
 
     function setStatus(text) {
         self.statusLine.innerHTML = text;
     }
 
     function addStatusLine(top, left, width, height) {
         /* add a status line div */
         var div = document.createElement('div');
         div.id = "mpStatus";
         div.style.backgroundColor = "rgb(240, 240, 240)";
         div.style.position = "absolute";
         div.style.top = top + "px";
-        //div.style.left = left+"px";
+        div.style.left = left + "px";
         div.style.width = width + "px";
         div.style.height = height + "px";
         div.style["border-left"] = "1px solid #DDD";
         div.style["border-right"] = "1px solid #DDD";
         div.style["border-top"] = "1px solid #DDD";
+        //div.style["border-bottom"]="1px solid #DDD";
         div.style["font-size"] = (gStatusHeight - 1) + "px";
+        //div.style["vertical-align"]="middle";
+        //div.style["line-height"]=(height-2)+"px";
+        //div.style["box-shadow"]="0px 2px 4px rgba(0,0,0,0.3)";
+        //div.style["border-radius"]="2px";
         div.style["cursor"] = "pointer";
         div.style["font-family"] = "sans-serif";
         self.div.appendChild(div);
         self.statusLine = div;
     }
 
     function addProgressBars(top, left) {
@@ -496,16 +431,16 @@
         canv.id = 'mpCanvas';
         //canv.style.border = "1px solid #AAAAAA";
         canv.style.backgroundColor = "white";
         canv.style.position = "absolute";
         canv.style.display = "block";
         canv.style.width = width + "px";
         canv.style.height = height + "px";
-        //canv.style.top = top+"px";
-        //canv.style.left = left+"px";
+        canv.style.top = top + "px";
+        canv.style.left = left + "px";
         // No scaling = one unit on screen is one pixel. Essential for speed.
         canv.width = width;
         canv.height = height;
 
         // need to keep these as ints, need them all the time
         self.width = width;
         self.height = height;
@@ -544,89 +479,33 @@
         var pxLabels = [];
         for (var i = 0; i < labels.length; i++) {
             var annot = labels[i];
             var x = annot[0];
             var y = annot[1];
             var text = annot[2];
             // XX ignore anything outside of current zoom range. Performance?
-            if (isHidden(x, y) || (x < minX) || (x > maxX) || (y < minY) || (y > maxY)) {
+            if ((x < minX) || (x > maxX) || (y < minY) || (y > maxY)) {
                 pxLabels.push(null);
-            } else {
-                var xPx = Math.round((x - minX) * xMult) + borderSize;
-                var yPx = winHeight - Math.round((y - minY) * yMult) + borderSize;
-                pxLabels.push([xPx, yPx, text]);
+                continue;
             }
+            var xPx = Math.round((x - minX) * xMult) + borderSize;
+            var yPx = winHeight - Math.round((y - minY) * yMult) + borderSize;
+            pxLabels.push([xPx, yPx, text]);
         }
         return pxLabels;
     }
 
-    function constrainVal(x, min, max) {
-        /* if x is not in range min, max, limit to min or max */
-        if (x < min)
-            return min;
-        if (x > max)
-            return max;
-        return x;
-    }
-
-    function scaleLines(lines, zoomRange, winWidth, winHeight) {
-        /* scale an array of (x1, y1, x2, y2), cutting lines at the screen edges */
-        var minX = zoomRange.minX;
-        var maxX = zoomRange.maxX;
-        var minY = zoomRange.minY;
-        var maxY = zoomRange.maxY;
-
-        var spanX = maxX - minX;
-        var spanY = maxY - minY;
-        var xMult = winWidth / spanX;
-        var yMult = winHeight / spanY;
-
-        // transform from data floats to screen pixel coordinates
-        var pxLines = [];
-        for (var lineIdx = 0; lineIdx < lines.length; lineIdx++) {
-            var line = lines[lineIdx];
-            var x1 = line[0];
-            var y1 = line[1];
-            var x2 = line[2];
-            var y2 = line[3];
-
-            var startInvis = ((x1 < minX) || (x1 > maxX) || (y1 < minY) || (y1 > maxY));
-            var endInvis = ((x2 < minX) || (x2 > maxX) || (y2 < minY) || (y2 > maxY));
-
-            // line is entirely hidden
-            if (startInvis && endInvis)
-                continue
-            if (startInvis) {
-                x1 = constrainVal(x1, minX, maxX);
-                y1 = constrainVal(y1, minY, maxY);
-            }
-            if (endInvis) {
-                x2 = constrainVal(x2, minX, maxX);
-                y2 = constrainVal(y2, minY, maxY);
-            }
-
-            var x1Px = Math.round((x1 - minX) * xMult);
-            var y1Px = winHeight - Math.round((y1 - minY) * yMult);
-            var x2Px = Math.round((x2 - minX) * xMult);
-            var y2Px = winHeight - Math.round((y2 - minY) * yMult);
-            pxLines.push([x1Px, y1Px, x2Px, y2Px]);
-        }
-        return pxLines;
-    }
-
     function scaleCoords(coords, borderSize, zoomRange, winWidth, winHeight, annots) {
         /* scale list of [x (float),y (float)] to integer pixels on screen and
          * annots is an array with on-screen annotations in the format (x, y,
          * otherInfo) that is also scaled.  return [array of (x (int), y (int)),
          * scaled annots array]. Take into account the current zoom range.      *
          * Canvas origin is top-left, but usually plotting origin is bottom-left,
-         * so also flip the Y axis. sets invisible coords to HIDCOORD
+         * so also flip the Y axis.
          * */
-        if (coords === null)
-            return;
         console.time("scale");
         var minX = zoomRange.minX;
         var maxX = zoomRange.maxX;
         var minY = zoomRange.minY;
         var maxY = zoomRange.maxY;
 
         winWidth = winWidth - (2 * borderSize);
@@ -638,228 +517,85 @@
         var yMult = winHeight / spanY;
 
         // transform from data floats to screen pixel coordinates
         var pixelCoords = new Uint16Array(coords.length);
         for (var i = 0; i < coords.length / 2; i++) {
             var x = coords[i * 2];
             var y = coords[i * 2 + 1];
-            // set everything outside of current zoom range to hidden
-            if ((x < minX) || (x > maxX) || (y < minY) || (y > maxY)) {
-                pixelCoords[2 * i] = HIDCOORD; // see isHidden()
-                pixelCoords[2 * i + 1] = HIDCOORD;
-            } else {
-                var xPx = Math.round((x - minX) * xMult) + borderSize;
-                // our y-axis is flipped compared to matplotlib/R, so we do winHeight - pixel value
-                // to make sure that our plot looks like the figures in the papers
-                var yPx = winHeight - Math.round((y - minY) * yMult) + borderSize;
-                pixelCoords[2 * i] = xPx;
-                pixelCoords[2 * i + 1] = yPx;
-            }
+            // simply ignore anything outside of current zoom range.
+            if ((x < minX) || (x > maxX) || (y < minY) || (y > maxY))
+                continue;
+            var xPx = Math.round((x - minX) * xMult) + borderSize;
+            // flipY: y-axis is flipped, so we do winHeight - pixel value
+            var yPx = winHeight - Math.round((y - minY) * yMult) + borderSize;
+            pixelCoords[2 * i] = xPx;
+            pixelCoords[2 * i + 1] = yPx;
         }
 
         console.timeEnd("scale");
         return pixelCoords;
     }
 
     function drawRect(ctx, pxCoords, coordColors, colors, radius, alpha, selCells) {
-        /* draw not circles but tiny rectangles. Maybe good enough for 2pixels sizes */
-        debug("Drawing " + coordColors.length + " rectangles, with fillRect");
+        console.log("Drawing " + coordColors.length + " rectangles, with fillRect");
         ctx.save();
         ctx.globalAlpha = alpha;
         var dblSize = 2 * radius;
         var count = 0;
         for (var i = 0; i < pxCoords.length / 2; i++) {
             var pxX = pxCoords[2 * i];
             var pxY = pxCoords[2 * i + 1];
-            if (isHidden(pxX, pxY))
+            if (pxX === 0 && pxY === 0)
                 continue;
             var col = colors[coordColors[i]];
             ctx.fillStyle = "#" + col;
             ctx.fillRect(pxX - radius, pxY - radius, dblSize, dblSize);
             count++;
         }
 
         // draw the selection as black rectangles
         ctx.globalAlpha = 0.7;
         ctx.fillStyle = "black";
-        selCells.forEach(function(cellId) {
-            let pxX = pxCoords[2 * cellId];
-            let pxY = pxCoords[2 * cellId + 1];
-            ctx.fillRect(pxX - radius, pxY - radius, dblSize, dblSize);
-            count += 1;
-        })
-        debug(count + " rectangles drawn (including selection)");
+        if (selCells !== null)
+            for (i = 0; i < selCells.length; i++) {
+                var cellId = selCells[i];
+                var pxX = pxCoords[2 * cellId];
+                var pxY = pxCoords[2 * cellId + 1];
+                ctx.fillRect(pxX - radius, pxY - radius, dblSize, dblSize);
+                count += 1;
+            }
+        console.log(count + " rectangles drawn (including selection)");
         ctx.restore();
-        return count;
     }
 
     function drawCirclesStupid(ctx, pxCoords, coordColors, colors, radius, alpha, selCells) {
         /* draw little circles onto canvas. pxCoords are the centers.  */
-        debug("Drawing " + coordColors.length + " circles with stupid renderer");
+        console.log("Drawing " + coordColors.length + " circles with stupid renderer");
         ctx.globalAlpha = alpha;
         var dblSize = 2 * radius;
-        var count = 0;
         for (var i = 0; i < pxCoords.length / 2; i++) {
             var pxX = pxCoords[2 * i];
             var pxY = pxCoords[2 * i + 1];
-            if (isHidden(pxX, pxY))
-                continue;
             var col = colors[coordColors[i]];
             ctx.fillStyle = "#" + col;
             //ctx.fillRect(pxX-size, pxY-size, dblSize, dblSize);
             ctx.beginPath();
             ctx.arc(pxX, pxY, radius, 0, 2 * Math.PI);
             ctx.closePath();
             ctx.fill();
-            count++;
         }
-        return count;
     }
 
     function intersectRect(r1left, r1right, r1top, r1bottom, r2left, r2right, r2top, r2bottom) {
-        /* return true if two rectangles overlap,
+        /* return true if two rectangles overlap, 
        https://stackoverflow.com/questions/2752349/fast-rectangle-to-rectangle-intersection
 	*/
         return !(r2left > r1right || r2right < r1left || r2top > r1bottom || r2bottom < r1top);
     }
 
-    function drawLines(ctx, pxLines, width, height, attrs) {
-        /* draw lines defined by array with (x1, y1, x2, y2) arrays.
-         * color is a CSS name, so usually prefixed by # if a hexcode
-         * width is the width in pixels.
-         * */
-        ctx.save();
-        //ctx.globalAlpha = 1.0;
-
-        ctx.strokeStyle = attrs.lineColor || "#888888";
-        ctx.lineWidth = attrs.lineWidth || 3;
-        ctx.globalAlpha = attrs.lineAlpha || 0.5;
-        //ctx.miterLimit =2;
-        //ctx.strokeStyle = "rgba(200, 200, 200, 0.3)";
-
-        for (var i = 0; i < pxLines.length; i++) {
-            var line = pxLines[i];
-            var x1 = line[0];
-            var y1 = line[1];
-            var x2 = line[2];
-            var y2 = line[3];
-
-            ctx.beginPath();
-            ctx.moveTo(x1, y1);
-            ctx.lineTo(x2, y2);
-            ctx.stroke();
-        }
-        ctx.restore();
-    }
-
-    function drawLabelsSvg(svgLines, labelCoords, winWidth, winHeight, zoomFact) {
-        /* given an array of [x, y, text], draw the text. returns bounding
-         * boxes as array of [x1, y1, x2, y2]  */
-
-        //ctx.strokeStyle = '#EEEEEE';
-        //ctx.lineWidth = 5;
-        //ctx.miterLimit =2;
-        //ctx.strokeStyle = "rgba(200, 200, 200, 0.3)";
-        //ctx.textBaseline = "top";
-        //
-        //ctx.shadowBlur=6;
-        //ctx.shadowColor="white";
-        //ctx.fillStyle = "rgba(0,0,0,0.8)";
-        //ctx.textAlign = "left";
-        //
-        for (var i = 0; i < labelCoords.length; i++) {
-            var coord = labelCoords[i];
-            if (coord === null) { // outside of view range, push a null to avoid messing up the order of bboxArr
-                continue;
-            }
-
-            var x = coord[0];
-            var y = coord[1];
-            var text = coord[2];
-
-            // don't draw labels where the midpoint is off-screen
-            if (x < 0 || y < 0 || x > winWidth || y > winHeight) {
-                continue;
-            }
-
-            svgLines.push("<text font-family='sans-serif' font-size='" + gTextSize + "' fill='black' text-anchor='middle' x='" + x + "' y='" + y + "'>" + text + "</text>");
-        }
-    }
-
-    self.drawLegendSvg = function(legend, legWidth) {
-        /* draw a legend onto the SVG given a legend object. */
-        var svgLines = self.svgLines;
-
-        var rows = legend.rows;
-
-        var legTitle = legend.title;
-        var subTitle = legend.subTitle;
-
-        var left = self.canvas.width; // x position where legend starts
-
-        var lineHeight = 18;
-
-        var x = left + 11;
-        var y = lineHeight;
-        svgLines.push("<text font-family='sans-serif' font-size='" + gTextSize + "' fill='black' x='" + x + "' y='" + y + "'>" + legTitle + "</text>");
-        y += lineHeight;
-
-        if (subTitle) {
-            htmls.push('<div id="tpLegendSubTitle" >' + subTitle + "</div>");
-            svgLines.push("<text font-family='sans-serif' font-size='" + gTextSize + "' fill='black' text-anchor='middle' x='" + x + "' y='" + y + "'>" + subTitle + "</text>");
-            y += lineHeight;
-        }
-
-        y += lineHeight;
-
-        // get the sum of all rows, to calculate frequency
-        var sum = 0;
-        for (var i = 0; i < rows.length; i++) {
-            let count = rows[i].count;
-            sum += count;
-        }
-
-        for (i = 0; i < rows.length; i++) {
-            // a lot was copied from cellBrowser:buildLegend(), could use some refactoring to reduce duplication
-            var row = rows[i];
-            var colorHex = row.color; // manual color
-            if (colorHex === null)
-                colorHex = row.defColor; // default color
-
-            var label = row.label;
-            var longLabel = row.longLabel;
-
-            let count = row.count;
-            var valueIndex = row.intKey;
-            var freq = 100 * count / sum;
-
-            if (count === 0) // never output categories with 0 count.
-                continue;
-
-            // this was copied from cellbrowser:buildLegend - refactor soon
-            label = label.replace(/_/g, " ").replace(/'/g, "&#39;").trim();
-            if (label === "") {
-                label = "(empty)";
-            }
-
-            svgLines.push("<rect width='15' height='15' fill='#" + colorHex + "' x='" + x + "' y='" + y + "'></rect>");
-            y += lineHeight;
-
-            var prec = 1;
-            if (freq < 1)
-                prec = 2;
-
-            svgLines.push("<text font-family='sans-serif' font-size='" + gTextSize + "' fill='black' text-anchor='start' x='" + (x + 18) + "' y='" + (y - 4) + "'>" + label + "</text>");
-            svgLines.push("<text font-family='sans-serif' font-size='" + gTextSize + "' fill='black' text-anchor='end' x='" + (left + legWidth - 3) + "' y='" + y + "'>" + freq.toFixed(prec) + "%</text>");
-            y += lineHeight;
-
-        }
-        // cannot draw violin plots in SVG right now
-    };
-
     function drawLabels(ctx, labelCoords, winWidth, winHeight, zoomFact) {
         /* given an array of [x, y, text], draw the text. returns bounding
          * boxes as array of [x1, y1, x2, y2]  */
 
         console.time("labels");
         ctx.save();
         ctx.font = "bold " + gTextSize + "px Sans-serif"
@@ -877,70 +613,99 @@
         ctx.textAlign = "left";
 
         var addMargin = 1; // how many pixels to extend the bbox around the text, make clicking easier
         var bboxArr = []; // array of click hit boxes
 
         for (var i = 0; i < labelCoords.length; i++) {
             var coord = labelCoords[i];
-            if (coord === null) { // outside of view range, push a null to avoid messing up the order of bboxArr
+            if (coord === null) { // outside of view range
                 bboxArr.push(null);
-                continue;
+                continue
             }
 
             var x = coord[0];
             var y = coord[1];
             var text = coord[2];
 
             var textWidth = Math.round(ctx.measureText(text).width);
             // move x to the left, so text is centered on x
             x = x - Math.round(textWidth * 0.5);
 
+            // don't draw labels where the midpoint is off-screen
+            if (x < 0 || y < 0 || x > winWidth || y > winWidth) {
+                bboxArr.push(null);
+                continue;
+            }
+
             var textX1 = x;
             var textY1 = y;
             var textX2 = Math.round(x + textWidth);
             var textY2 = y + gTextSize;
 
-            // don't draw labels where the midpoint is off-screen
-            if (x < 0 || y < 0 || x > winWidth || y > winHeight) {
-                bboxArr.push(null);
-                continue;
+            if (zoomFact === 1.0) {
+                // at 100% zoom, make some minimal effort to keep labels on screen
+                if (x < 0)
+                    x = 0;
+                if ((x + textWidth) > winWidth)
+                    x = winWidth - textWidth;
+                if (y + gTextSize > winHeight)
+                    y = winHeight - gTextSize;
+
+                // also only at 100% zoom, make a minimal effort to avoid label overlaps
+                // a perfect solution would take much more time
+                for (var j = 0; j < bboxArr.length; j++) {
+                    var bbox = bboxArr[j];
+                    if (bbox === null) // = outside of screen
+                        continue;
+                    var bx1 = bbox[0];
+                    var by1 = bbox[1];
+                    var bx2 = bbox[2];
+                    var by2 = bbox[3];
+                    if (intersectRect(textX1, textX2, textY1, textY2, bx1, bx2, by1, by2)) {
+                        // push the overlapping label away a little
+                        var diff = Math.round(0.75 * gTextSize);
+                        if (textY1 < by1)
+                            y -= diff;
+                        else
+                            y += diff;
+                    }
+                }
             }
 
-
             ctx.strokeText(text, x, y);
             ctx.fillText(text, x, y);
 
             bboxArr.push([textX1 - addMargin, textY1 - addMargin, textX2 + addMargin, textY2 + addMargin]);
         }
         ctx.restore();
         console.timeEnd("labels");
         return bboxArr;
     }
 
-    // function drawLabels_dom(ctx, labelCoords, isFull) {
-    //     /* given an array of [x, y, text], draw the text. returns bounding boxes as array of [x1, y1, x2, y2]  */
-    //     for (var i=0; i < labelCoords.length; i++) {
-    //         var coord = labelCoords[i];
-    //         var x = coord[0];
-    //         var y = coord[1];
-    //         var text = coord[2];
-
-    //         var div = document.createElement('div');
-    //         div.id = id;
-    //         //div.style.border = "1px solid #DDDDDD";
-    //         div.style.backgroundColor = "rgb(230, 230, 230, 0.6)";
-    //         div.style.width = width+"px";
-    //         div.style.height = height+"px";
-    //         div.style["text-align"]="center";
-    //         div.style["vertical-align"]="middle";
-    //         div.style["line-height"]=height+"px";
-    //     }
-    //     ctx.restore();
-    //     return bboxArr;
-    // }
+    function drawLabels_dom(ctx, labelCoords, isFull) {
+        /* given an array of [x, y, text], draw the text. returns bounding boxes as array of [x1, y1, x2, y2]  */
+        for (var i = 0; i < labelCoords.length; i++) {
+            var coord = labelCoords[i];
+            var x = coord[0];
+            var y = coord[1];
+            var text = coord[2];
+
+            var div = document.createElement('div');
+            div.id = id;
+            //div.style.border = "1px solid #DDDDDD";
+            div.style.backgroundColor = "rgb(230, 230, 230, 0.6)";
+            div.style.width = width + "px";
+            div.style.height = height + "px";
+            div.style["text-align"] = "center";
+            div.style["vertical-align"] = "middle";
+            div.style["line-height"] = height + "px";
+        }
+        ctx.restore();
+        return bboxArr;
+    }
 
     // https://stackoverflow.com/questions/5560248/programmatically-lighten-or-darken-a-hex-color-or-rgb-and-blend-colors
     function shadeColor(color, percent) {
         var f = parseInt(color, 16),
             t = percent < 0 ? 0 : 255,
             p = percent < 0 ? percent * -1 : percent,
             R = f >> 16,
@@ -952,15 +717,15 @@
     function drawCirclesDrawImage(ctx, pxCoords, coordColors, colors, radius, alpha, selCells) {
         /* predraw and copy circles into canvas. pxCoords are the centers.  */
         // almost copied from by https://stackoverflow.com/questions/13916066/speed-up-the-drawing-of-many-points-on-a-html5-canvas-element
         // around 2x faster than drawing full circles
         // create an off-screen canvas
 
         ctx.save();
-        debug("Drawing " + coordColors.length + " coords with drawImg renderer, radius=" + radius);
+        console.log("Drawing " + coordColors.length + " coords with drawImg renderer, radius=" + radius);
         var off = document.createElement('canvas'); // not added to DOM, will be gc'ed
         var diam = Math.round(2 * radius);
         var tileWidth = diam + 2; // must add one pixel on each side, space for antialising
         var tileHeight = tileWidth; // otherwise circles look cut off
         off.width = (colors.length + 1) * tileWidth;
         off.height = tileHeight;
         var ctxOff = off.getContext('2d');
@@ -973,15 +738,15 @@
             // arc(x, y, r, 0, 2*pi)
             ctxOff.arc(i * tileWidth + radius + 1, radius + 1, radius, 0, 2 * Math.PI);
             ctxOff.closePath();
             ctxOff.fill();
 
             // only draw outline for big circles
             ctxOff.lineWidth = 1.0;
-            if (radius > 5) {
+            if (radius > 6) {
                 var strokeCol = "#" + shadeColor(colors[i], 0.9);
                 ctxOff.strokeStyle = strokeCol;
 
                 ctxOff.beginPath();
                 ctxOff.arc(i * tileWidth + radius + 1, radius + 1, radius, 0, 2 * Math.PI);
                 ctxOff.closePath();
                 ctxOff.stroke();
@@ -999,42 +764,44 @@
         ctxOff.stroke();
 
         if (alpha !== undefined)
             ctx.globalAlpha = alpha;
 
         // blit the circles onto the main canvas
         var count = 0;
-        for (let i = 0; i < pxCoords.length / 2; i++) {
+        for (var i = 0; i < pxCoords.length / 2; i++) {
             var pxX = pxCoords[2 * i];
             var pxY = pxCoords[2 * i + 1];
-            if (isHidden(pxX, pxY))
+            if (pxX === 0 && pxY === 0)
                 continue;
             var col = coordColors[i];
             count++;
             // drawImage(img,sx,sy,swidth,sheight,x,y,width,height);
             ctx.drawImage(off, col * tileWidth, 0, tileWidth, tileHeight, pxX - radius - 1, pxY - radius - 1, tileWidth, tileHeight);
         }
 
         // overdraw the selection as solid black circle outlines
         ctx.globalAlpha = 0.7;
-        selCells.forEach(function(cellId) {
-            let pxX = pxCoords[2 * cellId];
-            let pxY = pxCoords[2 * cellId + 1];
-            if (isHidden(pxX, pxY))
-                return;
-            // make sure that old leftover overlapping black circles don't shine through
-            let col = coordColors[cellId];
-            ctx.drawImage(off, col * tileWidth, 0, tileWidth, tileHeight, pxX - radius - 1, pxY - radius - 1, tileWidth, tileHeight);
+        if (selCells !== null) {
+            for (i = 0; i < selCells.length; i++) {
+                var cellId = selCells[i];
+                var pxX = pxCoords[2 * cellId];
+                var pxY = pxCoords[2 * cellId + 1];
+                if (pxX === 0 && pxY === 0)
+                    continue;
+                // make sure that old leftover overlapping black circles don't shine through
+                var col = coordColors[cellId];
+                ctx.drawImage(off, col * tileWidth, 0, tileWidth, tileHeight, pxX - radius - 1, pxY - radius - 1, tileWidth, tileHeight);
 
-            ctx.drawImage(off, selImgId * tileWidth, 0, tileWidth, tileHeight, pxX - radius - 1, pxY - radius - 1, tileWidth, tileHeight);
-        })
+                ctx.drawImage(off, selImgId * tileWidth, 0, tileWidth, tileHeight, pxX - radius - 1, pxY - radius - 1, tileWidth, tileHeight);
+            }
+        }
 
-        debug(count + " circles drawn");
+        console.log(count + " circles drawn");
         ctx.restore();
-        return count;
     }
 
     function hexToInt(colors) {
         /* convert a list of hex values to ints */
         var intList = [];
         for (var i = 0; i < colors.length; i++) {
             var colHex = colors[i];
@@ -1056,15 +823,15 @@
         var rgbColors = hexToInt(colors);
         var invAlpha = 1.0 - alpha;
 
         // alpha-blend pixels into array
         for (var i = 0; i < pxCoords.length / 2; i++) {
             var pxX = pxCoords[2 * i];
             var pxY = pxCoords[2 * i + 1];
-            if (isHidden(pxX, pxY))
+            if (pxX === 0 && pxY === 0)
                 continue;
             var p = 4 * (pxY * width + pxX); // pointer to red value of pixel at x,y
 
             var oldR = cData[p];
             var oldG = cData[p + 1];
             var oldB = cData[p + 2];
 
@@ -1080,57 +847,31 @@
             cData[p] = mixR;
             cData[p + 1] = mixG;
             cData[p + 2] = mixB;
             cData[p + 3] = 255; // no transparency... ever?
         }
     }
 
-    function drawBackground(ctx, back) {
-        /* draw the background image onto the canvas ctx */
-        if (!back)
-            return;
-        console.time("image");
-        //var ctxWidth = ctx.canvas.width; // size of the canvas on the screen in pixels
-        //var ctxHeight = ctx.canvas.height;
-
-        //var clipWidth = backuwidth;
-        //var clipHeight = back.height;
-
-        // arguments are: (imgObject, x/y coord on image for clipping, width / height of clipped image, where to place the image, width/height of image)
-        //var a = getSafeRect(back.image.width, back.image.height, back.clipX, back.clipY, back.image.width, back.image.height, 0, 0, ctxWidth, ctxHeight);
-        //console.log("drawing fixed coords", a.sx, a.sy, a.sw, a.sh, a.dx, a.dy, a.dw, a.dh);
-        //self.ctx.drawImage(back.image, a.sx, a.sy, a.sw, a.sh, a.dx, a.dy, a.dw, a.dh);
-        //self.ctx.drawImage(back.image, a.sx, a.sy, back.width, back.height, a.dx, a.dy, a.dw, a.dh);
-        console.log("drawImage sx, sy, sw, sh, dx, dy, dw, dh", back.sx, back.sy, back.sw, back.sh, back.dx, back.dy, back.dw, back.dh);
-        //self.ctx.drawImage(back.image, back.sx, back.sy, back.width, back.height, 0, 0, ctxWidth, ctxHeight);
-        self.ctx.drawImage(back.image, back.sx, back.sy, back.sw, back.sh, back.dx, back.dy, back.dw, back.dh);
-
-        console.timeEnd("image");
-    }
-
-
     function drawPixels(ctx, width, height, pxCoords, colorArr, colors, alpha, selCells) {
         /* draw single pixels into a pixel buffer and copy the buffer into a canvas */
 
         // by default the canvas has black pixels
         // so not doing: var canvasData = ctx.createImageData(width, height);
         // XX is this really faster than manually zero'ing the array?
         var canvasData = ctx.getImageData(0, 0, width, height);
         var cData = canvasData.data;
 
         var rgbColors = hexToInt(colors);
         var invAlpha = 1.0 - alpha;
 
-        var count = 0;
-
         // alpha-blend pixels into array
         for (var i = 0; i < pxCoords.length / 2; i++) {
             var pxX = pxCoords[2 * i];
             var pxY = pxCoords[2 * i + 1];
-            if (isHidden(pxX, pxY))
+            if (pxX === 0 && pxY === 0)
                 continue;
             var p = 4 * (pxY * width + pxX); // pointer to red value of pixel at x,y
 
             var oldR = cData[p];
             var oldG = cData[p + 1];
             var oldB = cData[p + 2];
 
@@ -1143,31 +884,31 @@
             var mixG = ~~(oldG * invAlpha + newG * alpha);
             var mixB = ~~(oldB * invAlpha + newB * alpha);
 
             cData[p] = mixR;
             cData[p + 1] = mixG;
             cData[p + 2] = mixB;
             cData[p + 3] = 255; // no transparency... ever?
-            count++;
         }
 
         // overdraw the selection as black pixels
-        selCells.forEach(function(cellId) {
-            let pxX = pxCoords[2 * cellId];
-            let pxY = pxCoords[2 * cellId + 1];
-            if (isHidden(pxX, pxY))
-                return;
-            let p = 4 * (pxY * width + pxX); // pointer to red value of pixel at x,y
-            cData[p] = 0;
-            cData[p + 1] = 0;
-            cData[p + 2] = 0;
-        })
+        if (selCells !== null)
+            for (i = 0; i < selCells.length; i++) {
+                var cellId = selCells[i];
+                var pxX = pxCoords[2 * cellId];
+                var pxY = pxCoords[2 * cellId + 1];
+                if (pxX === 0 && pxY === 0)
+                    continue;
+                var p = 4 * (pxY * width + pxX); // pointer to red value of pixel at x,y
+                cData[p] = 0;
+                cData[p + 1] = 0;
+                cData[p + 2] = 0;
+            }
 
         self.ctx.putImageData(canvasData, 0, 0);
-        return count;
     }
 
     function findRange(coords) {
         /* find range of pairs-array and return obj with attributes minX/maxX/minY/maxY */
         var minX = 9999999;
         var maxX = -9999999;
         var minY = 9999999;
@@ -1191,517 +932,276 @@
         obj.maxY = maxY;
         return obj; // not needed, but more explicit
     }
 
     function clearCanvas(ctx, width, height) {
         /* clear with a white background */
         // jsperf says this is fastest on Chrome, and still OK-ish in FF
-        //console.time("clear");
+        console.time("clear");
         ctx.save();
         ctx.globalAlpha = 1.0;
         ctx.fillStyle = "rgb(255,255,255)";
         ctx.fillRect(0, 0, width, height);
         ctx.restore();
-        //console.timeEnd("clear");
+        console.timeEnd("clear");
     }
 
     // -- object methods (=access the self object)
 
     this.onZoom100Click = function(ev) {
         self.zoom100();
         self.drawDots();
     };
 
-    this.setBackground = function(img) {
-        /* */
-        if (self.background === undefined || self.background === null)
-            self.background = {};
-        self.background.image = img;
-        self.scaleBackground(self.background, self.port.initZoom, self.port.zoomRange);
-        if (self.childPlot)
-            self.childPlot.setBackground(img);
-    };
-
-    function getSafeRect(width, height, sx, sy, sw, sh, dx, dy, dw, dh) {
-        if (sw < 0) {
-            sx += sw;
-            sw = Math.abs(sw);
-        }
-        if (sh < 0) {
-            sy += sh;
-            sh = Math.abs(sh);
-        }
-        if (dw < 0) {
-            dx += dw;
-            dw = Math.abs(dw);
-        }
-        if (dh < 0) {
-            dy += dh;
-            dh = Math.abs(dh);
-        }
-        const x1 = Math.max(sx, 0);
-        const x2 = Math.min(sx + sw, width);
-        const y1 = Math.max(sy, 0);
-        const y2 = Math.min(sy + sh, height);
-        const w_ratio = dw / sw;
-        const h_ratio = dh / sh;
-
-    }
-
-    this.scaleBackground = function(background, dataRange, zoomRange) {
-        /* determine the (x,y,width,height) in pixels of the current rectangle of the background bitmap on the canvas */
-        if (!background)
-            return;
-
-        var width = background.image.width; // source image width
-        var height = background.image.height; // source image height
-
-        var ctxWidth = self.canvas.width;
-        var ctxHeight = self.canvas.height;
-
-        var coordHeight = dataRange.maxX - dataRange.minX;
-        var coordWidth = dataRange.maxY - dataRange.minY;
-
-        var scaleX = width / coordHeight; // this is px/dataUnit to convert background image pixels to canvas pixels
-        var scaleY = height / coordHeight;
-
-        var sx1 = zoomRange.minX * scaleX; // sx = x position on source image
-        var sx2 = zoomRange.maxX * scaleX;
-
-        var sy1 = (coordHeight - zoomRange.maxY) * scaleY; // Y-positions must be subtracted from coordHeight - y axis is flipped!
-        var sy2 = (coordHeight - zoomRange.minY) * scaleY; // Our y-axis is always flipped!
-
-        var sw = sx2 - sx1; // size of slice of background image that is currently shown, in source pixels
-        var sh = sy2 - sy1;
-
-        var ctxWidth = self.canvas.width;
-        var ctxHeight = self.canvas.height;
-
-        // lame: since I wasn't able to figure out how to transform negative sx, sy to corrected dx, dy, coords - safari doesn't understand negative sx/sy - I simply use the scaleData function
-        // somehow https://gist.github.com/Kaiido/ca9c837382d89b9d0061e96181d1d862 didn't work for me
-        //var coords = [0.0, 0.0, dataRange.maxX, dataRange.maxY];
-        //var newCoords = scaleCoords(coords, 0, zoomRange, ctxWidth, ctxHeight, [])
-
-        var dx = 0;
-        var dy = 0;
-        var dw = ctxWidth;
-        var dh = ctxHeight;
-
-        //if (sx1 < 0) {
-        //sx1 = 0;
-        //sw = width;
-        //dx = newCoords[0];
-        //dw = newCoords[2] - dx;
-        //}
-
-        //if (sy1 < 0) {
-        //sy1 = 0;
-        //sh = height;
-        //dy = newCoords[1];
-        //dh = newCoords[3] - dy;
-        //}
-
-        background.sx = sx1;
-        background.sy = sy1;
-        background.sw = sw;
-        background.sh = sh;
-
-        background.dx = dx;
-        background.dy = dy;
-        background.dw = dw;
-        background.dh = dh;
-    }
-
     this.scaleData = function() {
         /* scale coords and labels to current zoom range, write results to pxCoords and pxLabels */
-        if (!self.coords) // window resize can call this before coordinates are loaded.
-            return;
-
-        var borderMargin = self.port.radius;
-        self.calcRadius();
+        var borderMargin = self.radius;
+        self.pxCoords = scaleCoords(self.coords, borderMargin, self.zoomRange, self.canvas.width, self.canvas.height);
 
-        self.coords.px = scaleCoords(self.coords.orig, borderMargin, self.port.zoomRange, self.canvas.width, self.canvas.height);
-        if (self.coords.lines)
-            self.coords.pxLines = scaleLines(self.coords.lines, self.port.zoomRange, self.canvas.width, self.canvas.height);
-        self.scaleBackground(self.background, self.port.initZoom, self.port.zoomRange);
-        self.scalingDone = true;
+        self.pxLabels = null;
+        if (self.clusterLabels !== undefined && self.clusterLabels !== null)
+            self.pxLabels = scaleLabels(self.clusterLabels, self.zoomRange, borderMargin, self.canvas.width, self.canvas.height);
     }
 
-    this.readyToDraw = function() {
-        return (self.scalingDone)
-    }
-
-    this.setTopLeft = function(top, left) {
-        /* set top and left position in pixels of the canvas */
-        self.top = top;
-        self.left = left; // keep an integer version of these numbers
-        self.div.style.top = top + "px";
-        self.div.style.left = left + "px";
-
-        self.setSize(self.width, self.height, false); // resize the various buttons
-    }
-
-    this.quickResize = function(width, height) {
-        /* resize the canvas and move the status line, don't rescale or draw  */
-        self.div.style.width = width + "px";
-        self.div.style.height = height + "px";
-
-        if (self.childPlot) {
-            width = width / 2;
-            //self.childPlot.left = self.left+width;
-            //self.childPlot.canvas.style.left = self.childPlot.left+"px";
-            self.childPlot.setPos(null, self.left + width);
-            self.childPlot.setSize(width, height, true);
-        }
+    this.setSize = function(width, height) {
+        /* resize canvas on the page re-scale the data and re-draw */
 
-        if (self.closeButton) {
-            self.closeButton.style.left = width - gCloseButtonFromRight;
-        }
+        // css and canvas sizes: these must be identical, otherwise canvas gets super slow
+        var canvWidth = width;
+        var canvHeight = height - gStatusHeight;
+        self.canvas.style.width = canvWidth + "px";
+        self.canvas.style.height = canvHeight + "px";
+        self.canvas.width = canvWidth;
+        self.canvas.height = canvHeight;
 
-        // css and actual canvas sizes: these must be identical, otherwise canvas gets super slow
-        self.canvas.style.width = width + "px";
         self.width = width;
         self.height = height;
-        //let canvHeight = height - gStatusHeight;
 
-        let canvHeight = height - gStatusHeight;
-        self.canvas.height = canvHeight;
-        self.canvas.width = width;
-        self.canvas.style.height = canvHeight + "px";
-        self.zoomDiv.style.top = (height - gZoomFromBottom) + "px";
-        self.zoomDiv.style.left = (gZoomFromLeft) + "px";
+        var zoomDiv = gebi('mpCtrls');
+        zoomDiv.style.top = (self.top + height - gZoomFromBottom) + "px";
+        zoomDiv.style.left = (self.left + width - gZoomFromRight) + "px";
 
         var statusDiv = self.statusLine;
-        statusDiv.style.top = (height - gStatusHeight) + "px";
+        statusDiv.style.top = (self.top + height - gStatusHeight) + "px";
         statusDiv.style.width = width + "px";
 
-        self.titleDiv.style.top = (height - gStatusHeight - gTitleSize) + "px";
-
-    }
-
-    this.setPos = function(top, left) {
-        /* position canvas. Does not affect child  */
-        if (top) {
-            self.top = top;
-            self.div.style.top = top + "px";
-        }
-        if (left) {
-            self.left = left;
-            self.div.style.left = left + "px";
-        }
-    }
-
-    this.setSize = function(width, height, doRedraw) {
-        /* resize canvas on the page re-scale the data and re-draw, unless doRedraw is false */
-        if (width === null)
-            width = self.div.getBoundingClientRect().width;
-
-        self.quickResize(width, height);
-
-        if (self.coords)
-            self.scaleData();
+        self.titleDiv.style.top = (self.top + height - gStatusHeight - gTitleSize) + "px";
 
-        if (doRedraw === undefined || doRedraw === true)
-            self.drawDots();
+        self.scaleData();
+        //clearCanvas(self.ctx, width, height);
+        self.drawDots();
     };
 
-    this.setCoords = function(coords, clusterLabels, coordInfo, opts) {
+    this.setCoords = function(coords, clusterLabels, minX, maxX, minY, maxY) {
         /* specify new coordinates of circles to draw, an array of (x,y) coordinates */
         /* Scale data to current screen dimensions */
         /* clusterLabels is optional: array of [x, y, labelString]*/
-        /* minX, maxX, etc are optional
-         * opts are optional arguments like radius, alpha etc, see initPlot/args */
-        self.scalingDone = false;
+        /* minX, maxX, etc are optional */
+        // "==null" checks for both undefined and null
         if (coords.length === 0)
             alert("cbDraw-setCoords called with no coordinates");
 
-        var minX = coordInfo.minX;
-        var maxX = coordInfo.maxX;
-        var minY = coordInfo.minY;
-        var maxY = coordInfo.maxY;
-        var useRaw = coordInfo.useRaw;
-
-        var coordOpts = cloneObj(self.globalOpts);
-        copyObj(opts, coordOpts);
-
-        var oldRadius = self.port.initRadius;
-        var oldAlpha = self.port.initAlpha;
-        var oldLabels = self.coords.pxLabels;
-        self.port = {};
-        self.initPort(coordOpts);
-        if (oldRadius)
-            self.port.initRadius = oldRadius;
-        if (oldAlpha)
-            self.port.initAlpha = oldAlpha;
-        self.coords = {};
-
-        var newZr = {};
         if (minX === undefined || maxX === undefined || minY === undefined || maxY === undefined)
-            newZr = findRange(coords);
-        else {
-            newZr = {
+            self.initZoom = findRange(coords);
+        else
+            self.initZoom = {
                 minX: minX,
                 maxX: maxX,
                 minY: minY,
                 maxY: maxY
-            };
-        }
-
-        // switch off any moving of the spots to the minimum position
-        if (useRaw) {
-            newZr.minX = 0.0;
-            newZr.minY = 0.0;
-        }
-
-        // we need the maximal min-max ranges of the original coordinates for later
-        copyObj(newZr, self.port.initZoom);
-        // the current min-max ranges of the values are the maximal values, so copy them = zoom 100%
-        copyObj(newZr, self.port.zoomRange);
-
-        self.coords.orig = coords;
-        self.coords.labels = clusterLabels;
-
-        var count = 0;
-        for (var i = 0; i < coords.length / 2; i++) {
-            var cellX = coords[i * 2];
-            var cellY = coords[i * 2 + 1];
-            if (!(isHidden(cellX, cellY)))
-                count++;
-        }
+            }
+        self.zoomRange = cloneObj(self.initZoom);
 
-        setStatus(count + " visible " + self.gSampleDescription + "s loaded");
+        self.coords = coords;
+        self.clusterLabels = clusterLabels;
+        setStatus((coords.length / 2) + " " + self.gSampleDescription + "s loaded");
 
-        if (opts.lines)
-            self._setLines(opts["lines"], opts);
         self.scaleData();
-    };
-
-    this.setLabelCoords = function(labelCoords) {
-        /* set the label coords and return true if there were any labels before */
-        var hadLabelsBefore = self.coords.labels.length > 0;
-        self.coords.labels = labelCoords;
-        return hadLabelsBefore;
+        if (self.radius === null || self.radius == undefined) {
+            self.radius = guessRadius(coords.length);
+            self.initRadius = self.radius;
+        }
     };
 
     this.setColorArr = function(colorArr) {
         /* set the color array, one array with one index per coordinate */
-        self.col.arr = colorArr;
+        self.colorArr = colorArr;
     };
 
     this.setColors = function(colors) {
         /* set the colors, one for each value of a in setColorArr(a). colors is an
          * array of six-digit hex strings. Not #-prefixed! */
-        self.col.pal = colors;
+        self.colors = colors;
     };
 
-    this.calcRadius = function() {
-        /* calculate the radius from current zoom factor and set radius, alpha and zoomFact in self.port */
-        // make the circles a bit smaller than expected
-        var zr = self.port.zoomRange;
-        var iz = self.port.initZoom;
-        var initAlpha = self.port.initAlpha;
-        var initSpan = iz.maxX - iz.minX;
-        var currentSpan = zr.maxX - zr.minX;
-        var zoomFact = initSpan / currentSpan;
-
-        var baseRadius = self.port.initRadius;
-        if (baseRadius === 0)
-            baseRadius = 0.7;
-        var radius = Math.floor(baseRadius * Math.sqrt(zoomFact));
-
-        // the higher the zoom factor, the higher the alpha value
-        var zoomFrac = Math.min(1.0, zoomFact / 100.0); // zoom as fraction, max is 1.0
-        var alpha = initAlpha + 3.0 * zoomFrac * (1.0 - initAlpha);
-        alpha = Math.min(0.8, alpha);
-        debug("Zoom factor: ", zoomFact, ", Radius: " + radius + ", alpha: " + alpha);
-
-        self.port.zoomFact = zoomFact;
-        self.port.alpha = alpha;
-        self.port.radius = radius;
-    }
+    //this.drawTitle = function() {
+    //var ctx = self.ctx;
+    //ctx.save();
+    //ctx.font = "bold "+gTextSize+"px Sans-serif"
+    //ctx.fillStyle = "rgba(220, 220, 220)";
+    //ctx.textBaseline = "top";
+    //ctx.fillText(self.title,5,self.height - gTextSize - 3); 
+    //ctx.restore();
+    //};
 
-    this.drawDots = function(doSvg) {
+    this.drawDots = function() {
         /* draw coordinates to canvas with current colors */
         console.time("draw");
 
         self.clear();
 
-        var radius = self.port.radius;
-        var alpha = self.port.alpha;
-        var zoomFact = self.port.zoomFact;
-        var coords = self.coords.px;
-        var pal = self.col.pal;
-        var colArr = self.col.arr;
-        var count = 0;
+        //if (self.title!==undefined)
+        //self.drawTitle();
 
-        if (alpha === undefined)
+        if (self.alpha === undefined)
             alert("internal error: alpha is not defined");
-        if (coords === null)
+        if (self.pxCoords === null)
             alert("internal error: cannot draw if coordinates are not set yet");
-        if (colArr.length !== (coords.length >> 1))
-            alert("internal error: cbDraw.drawDots - colorArr is not 1/2 of coords array. Got " + pal.length + " color values but coordinates for " + (coords.length / 2) + " cells.");
+        if (self.colorArr.length !== (self.pxCoords.length >> 1))
+            alert("internal error: cbDraw.drawDots - colorArr is not 1/2 of coords array. Got " + self.colors.length + " color values but coordinates for " + (self.pxCoords.length / 2) + " cells.");
 
-        if (doSvg !== undefined) {
-            self.svgLines = [];
-            var legWidth = 200;
-            self.svgLines.push("<svg  xmlns='http://www.w3.org/2000/svg' height='" + self.canvas.height + "' width='" + (self.canvas.width + legWidth) + "'>\n");
-            drawCirclesSvg(self.svgLines, coords, colArr, pal, radius, alpha, self.selCells);
-            drawLabelsSvg(self.svgLines, self.coords.pxLabels, self.canvas.width, self.canvas.height, self.port.zoomFact);
-            return;
-        }
+        self.zoomFact = ((self.initZoom.maxX - self.initZoom.minX) / (self.zoomRange.maxX - self.zoomRange.minX));
 
-        drawBackground(self.ctx, self.background)
+        console.log("Zoom factor: " + self.zoomFact);
+        // make the circles a bit smaller than expected
+        var baseRadius = self.initRadius;
+        if (baseRadius === 0)
+            baseRadius = 0.7;
+        self.radius = Math.floor(baseRadius * Math.sqrt(self.zoomFact));
+
+        // the higher the zoom factor, the higher the alpha value
+        var zoomFrac = Math.min(1.0, self.zoomFact / 100.0); // zoom as fraction, max is 1.0
+        var alpha = self.alpha + 3.0 * zoomFrac * (1.0 - self.alpha);
+        alpha = Math.min(0.8, alpha);
+        console.log("Radius: " + self.radius + ", alpha: " + alpha);
 
-        if (radius === 0) {
-            count = drawPixels(self.ctx, self.canvas.width, self.canvas.height, coords,
-                colArr, pal, alpha, self.selCells);
-        } else if (radius === 1 || radius === 2) {
-            count = drawRect(self.ctx, coords, colArr, pal, radius, alpha, self.selCells);
+        if (self.radius === 0) {
+            drawPixels(self.ctx, self.canvas.width, self.canvas.height, self.pxCoords,
+                self.colorArr, self.colors, alpha, self.selCells);
+        } else if (self.radius === 1 || self.radius === 2) {
+            drawRect(self.ctx, self.pxCoords, self.colorArr, self.colors, self.radius, alpha, self.selCells);
         } else {
+
             switch (self.mode) {
                 case 0:
-                    count = drawCirclesStupid(self.ctx, coords, colArr, pal, radius, alpha, self.selCells);
+                    drawCirclesStupid(self.ctx, self.pxCoords, self.colorArr, self.colors, self.radius, alpha, self.selCells);
                     break;
                 case 1:
-                    count = drawCirclesDrawImage(self.ctx, coords, colArr, pal, radius, alpha, self.selCells);
+                    drawCirclesDrawImage(self.ctx, self.pxCoords, self.colorArr, self.colors, self.radius, alpha, self.selCells);
                     break;
                 case 2:
                     break;
             }
         }
 
-        self.count = count;
-
         console.timeEnd("draw");
 
-        if (self.doDrawLabels === true && self.coords.labels !== null && self.coords.labels !== undefined) {
-            self.redrawLabels();
+        if (self.doDrawLabels === true && self.pxLabels !== null) {
+            self.pxLabelBbox = drawLabels(self.ctx, self.pxLabels, self.canvas.width, self.canvas.height, self.zoomFact);
         }
-
-        if (self.coords.pxLines) {
-            console.time("draw lines");
-            drawLines(self.ctx, self.coords.pxLines, self.canvas.width, self.canvas.height, self.coords.lineAttrs);
-            console.timeEnd("draw lines");
-        }
-
-        if (self.childPlot)
-            self.childPlot.drawDots();
-    };
-
-    this.getSvgText = function() {
-        /* close and return the accumulated svg lines and clear the svg line buffer */
-        var svgLines = self.svgLines;
-        svgLines.push("</svg>\n");
-        self.svgLines = null;
-        return svgLines;
-    }
-
-    this.redrawLabels = function() {
-        /* draw only the labels */
-        self.coords.pxLabels = scaleLabels(
-            self.coords.labels,
-            self.port.zoomRange,
-            self.port.radius,
-            self.canvas.width,
-            self.canvas.height
-        );
-        self.coords.labelBbox = drawLabels(
-            self.ctx,
-            self.coords.pxLabels,
-            self.canvas.width,
-            self.canvas.height,
-            self.port.zoomFact
-        );
     };
 
     this.cellsAtPixel = function(x, y) {
         /* return the Ids of all cells at a particular pixel */
         var res = [];
-        var pxCoords = self.coords.px;
-        for (var i = 0; i < pxCoords.length / 2; i++) {
+        var pxCoords = self.pxCoords;
+        for (var i = 0; i < self.pxCoords.length / 2; i++) {
             var cellX = pxCoords[i * 2];
             var cellY = pxCoords[i * 2 + 1];
             if (cellX === x || cellY === y)
                 res.push(i);
         }
         return res;
     };
 
     this.cellsInRect = function(x1, y1, x2, y2) {
         /* return the Ids of all cells within certain pixel boundaries */
         var res = [];
-        var pxCoords = self.coords.px;
-        for (var i = 0; i < pxCoords.length / 2; i++) {
+        var pxCoords = self.pxCoords;
+        for (var i = 0; i < self.pxCoords.length / 2; i++) {
             var cellX = pxCoords[i * 2];
             var cellY = pxCoords[i * 2 + 1];
             if ((cellX >= x1) && (cellX <= x2) && (cellY >= y1) && (cellY <= y2))
                 res.push(i);
         }
         return res;
     };
 
+    //this.setSelection = function (idList) {
+    /* select some dots. idList is a list of integers. Specify null to clear. */
+    //self.selCells = new FastBitSet(idList);
+    //};
+
     this.zoom100 = function() {
         /* zoom to 100% and redraw */
-        copyObj(self.port.initZoom, self.port.zoomRange);
+        self.zoomRange = cloneObj(self.initZoom);
         self.scaleData();
-        //self.drawDots();
+        self.radius = self.initRadius;
+        self.drawDots();
     };
 
     this.zoomTo = function(x1, y1, x2, y2) {
         /* zoom to rectangle defined by two points */
         // make sure that x1<x2 and y1<y2 - can happen if mouse movement was upwards
-        debug("Zooming to pixels: ", x1, y1, x2, y2);
         var pxMinX = Math.min(x1, x2);
         var pxMaxX = Math.max(x1, x2);
 
         var pxMinY = Math.min(y1, y2);
         var pxMaxY = Math.max(y1, y2);
 
-        var zoomRange = self.port.zoomRange;
+        // force the zoom rectangle to have the same aspect ratio as our canvas
+        // by adapting the height. This is what Microsoft software does
+        // It may be better to fix the aspect ratio of the zoom rectangle while zooming?
+        // We probably do not want to distort the ratio.
+        var aspectRatio = self.width / self.height;
+        var rectWidth = (pxMaxX - pxMinX);
+        var newHeight = rectWidth / aspectRatio;
+        pxMaxY = pxMinY + newHeight;
+
+        var zoomRange = self.zoomRange;
         // window size in data coordinates
         var spanX = zoomRange.maxX - zoomRange.minX;
         var spanY = zoomRange.maxY - zoomRange.minY;
 
         // multiplier to convert from pixels to data coordinates
-        var xMult = spanX / self.canvas.width; // multiplier dataRange/pixel
-        var yMult = spanY / self.canvas.height;
+        var xMult = spanX / self.width; // multiplier dataRange/pixel
+        var yMult = spanY / self.height;
 
         var oldMinX = zoomRange.minX;
         var oldMinY = zoomRange.minY;
 
         zoomRange.minX = oldMinX + (pxMinX * xMult);
         zoomRange.minY = oldMinY + (pxMinY * yMult);
 
         zoomRange.maxX = oldMinX + (pxMaxX * xMult);
         zoomRange.maxY = oldMinY + (pxMaxY * yMult);
 
-        self.port.zoomRange = zoomRange;
-        debug("Marquee zoom window: " + JSON.stringify(self.port.zoomRange));
+        self.zoomRange = zoomRange;
 
         self.scaleData();
     };
 
     this.zoomBy = function(zoomFact, xPx, yPx) {
-        /* zoom centered around xPx,yPx by a given factor. Returns new zoom range.
+        /* zoom centered around xPx,yPx by a given factor. Returns new zoom range. 
          * zoomFact = 1.2 means zoom +20%
          * zoomFact = 0.8 means zoom -20%
          * */
-        var zr = self.port.zoomRange;
-        var iz = self.port.initZoom;
+        var zr = self.zoomRange;
+        var iz = self.initZoom;
 
-        debug("old zoomfact " + self.port.zoomFact);
+        console.log("zoomfact " + self.zoomFact);
 
         var xRange = Math.abs(zr.maxX - zr.minX);
         var yRange = Math.abs(zr.maxY - zr.minY);
 
         var minWeightX = 0.5; // how zooming should be distributed between min/max
         var minWeightY = 0.5;
         if (xPx !== undefined) {
             minWeightX = (xPx / self.width);
-            minWeightY = (yPx / self.canvas.height);
+            minWeightY = (yPx / self.height);
         }
         var scale = (1.0 - zoomFact);
 
         var newRange = {};
         newRange.minX = zr.minX - (xRange * scale * minWeightX);
         newRange.maxX = zr.maxX + (xRange * scale * (1 - minWeightX));
 
@@ -1711,62 +1211,36 @@
 
         // extreme zoom factors don't make sense, at some point we reach
         // the limit of the floating point numbers
         var newZoom = ((iz.maxX - iz.minX) / (newRange.maxX - newRange.minX));
         if (newZoom < 0.01 || newZoom > 1500)
             return zr;
 
-        debug("x min max " + zr.minX + " " + zr.maxX);
-        debug("y min max " + zr.minY + " " + zr.maxY);
-
-        self.port.zoomRange = newRange;
+        console.log("x min max " + zr.minX + " " + zr.maxX);
+        console.log("y min max " + zr.minY + " " + zr.maxY);
 
+        self.zoomRange = newRange;
         self.scaleData();
-
-        // a special case for connected plots that are not sharing our pixel coordinates
-        if (self.childPlot && self.coords !== self.childPlot.coords) {
-            self.childPlot.zoomBy(zoomFact, xPx, yPx);
-        }
-
         return newRange;
     };
 
-    this.movePerc = function(xDiffFrac, yDiffFrac) {
-        /* move a certain percentage of current view. xDiff/yDiff are floats, e.g. 0.1 is 10% up */
-        var zr = self.port.zoomRange;
-        var xRange = Math.abs(zr.maxX - zr.minX);
-        var yRange = Math.abs(zr.maxY - zr.minY);
-
-        var xDiffAbs = xRange * xDiffFrac;
-        var yDiffAbs = yRange * yDiffFrac;
-
-        var newRange = {};
-        newRange.minX = zr.minX + xDiffAbs;
-        newRange.maxX = zr.maxX + xDiffAbs;
-        newRange.minY = zr.minY + yDiffAbs;
-        newRange.maxY = zr.maxY + yDiffAbs;
-
-        copyObj(newRange, self.port.zoomRange);
-        self.scaleData();
-    };
-
     this.panStart = function() {
         /* called when starting a panning sequence, makes a snapshop of the current image */
         self.panCopy = document.createElement('canvas'); // not added to DOM, will be gc'ed
         self.panCopy.width = self.canvas.width;
         self.panCopy.height = self.canvas.height;
         var destCtx = self.panCopy.getContext("2d", {
             alpha: false
         });
         destCtx.drawImage(self.canvas, 0, 0);
     }
 
     this.panBy = function(xDiff, yDiff) {
         /* pan current image by x/y pixels */
-        debug('panning by ' + xDiff + ' ' + yDiff);
+        console.log('panning by ' + xDiff + ' ' + yDiff);
 
         //var srcCtx = self.panCopy.getContext("2d", { alpha: false });
         clearCanvas(self.ctx, self.canvas.width, self.canvas.height);
         self.ctx.drawImage(self.panCopy, -xDiff, -yDiff);
         // keep these for panEnd
         self.panDiffX = xDiff;
         self.panDiffY = yDiff;
@@ -1776,542 +1250,395 @@
         /* end a sequence of panBy calls, called when the mouse is released */
         self.moveBy(self.panDiffX, -self.panDiffY); // -1 because of flipY
         self.panCopy = null;
         self.panDiffX = null;
         self.panDiffY = null;
     }
 
-    // BEGIN SELECTION METHODS (could be an object?)
-
-    this.selectClear = function(skipNotify) {
+    this.selectClear = function() {
         /* clear selection */
-        self.selCells.clear();
+        self.selCells = null;
         setStatus("");
-        if (self.onSelChange !== null && skipNotify !== true)
-            self.onSelChange(self.selCells);
+        if (self.onSelChange !== null)
+            self.onSelChange([]);
     };
 
     this.selectSet = function(cellIds) {
         /* set selection to an array of integer cellIds */
-        self.selCells.clear();
-        //self.selCells.push(...cellIds); // "extend" = array spread syntax, https://davidwalsh.name/spread-operator
-        let selCells = self.selCells;
-        for (let i = 0; i < cellIds.length; i++)
-            selCells.add(cellIds[i]);
+        self.selCells = cellIds;
         self._selUpdate();
     };
 
     this.selectAdd = function(cellIdx) {
         /* add a single cell to the selection. If it already exists, remove it. */
+        if (self.selCells === null) {
+            self.selCells = [cellIdx];
+            self._selUpdate();
+            return;
+        }
+
         console.time("selectAdd");
-        if (self.selCells.has(cellIdx))
-            self.selCells.delete(cellIdx);
+        var foundIdx = self.selCells.indexOf(cellIdx);
+        if (foundIdx === -1)
+            self.selCells.push(cellIdx);
         else
-            self.selCells.add(cellIdx);
+            self.selCells.splice(foundIdx, 1);
         console.time("selectAdd");
         self._selUpdate();
     };
 
-    this.selectAll = function(cellIdx) {
-        /* add all cells to selection */
-        var selCells = self.selCells;
-        var pxCoords = self.coords.px;
-        for (var i = 0, I = pxCoords.length / 2; i < I; i++) {
-            selCells.add(i);
-        }
-        self.selCells = selCells;
-        self._selUpdate();
-    };
-
     this.selectVisible = function() {
         /* add all visible cells to selection */
+        if (self.selCells === null)
+            self.selCells = [];
+
         var selCells = self.selCells;
-        var pxCoords = self.coords.px;
+        var pxCoords = self.pxCoords;
         for (var i = 0; i < pxCoords.length / 2; i++) {
             var pxX = pxCoords[2 * i];
             var pxY = pxCoords[2 * i + 1];
-            if (isHidden(pxX, pxY))
+            if (pxX === 0 && pxY === 0)
                 continue;
-            selCells.add(i);
+            selCells.push(i);
         }
         self.selCells = selCells;
         self._selUpdate();
     }
 
     this.selectByColor = function(colIdx) {
         /* add all cells with a given color to the selection */
-        var colArr = self.col.arr;
-        var selCells = self.selCells;
-        var cnt = 0;
-        for (var i = 0; i < colArr.length; i++) {
-            if (colArr[i] === colIdx) {
-                selCells.add(i);
-                cnt++;
-            }
-        }
-        self.selCells = selCells;
-        debug(cnt + " cells appended to selection, by color");
-        self._selUpdate();
-    };
-
-    this.unselectByColor = function(colIdx) {
-        /* remove all cells with a given color from the selection */
-        var colArr = self.col.arr;
+        var colArr = self.colorArr;
         var selCells = self.selCells;
-        var cnt = 0;
+        if (selCells === null)
+            selCells = [];
         for (var i = 0; i < colArr.length; i++) {
-            if (colArr[i] === colIdx) {
-                selCells.delete(i);
-                cnt++;
-            }
+            if (colArr[i] === colIdx)
+                selCells.push(i);
         }
-
         self.selCells = selCells;
-        debug(cnt + " cells removed from selection, by color");
+        console.log(self.selCells.length + " cells selected, by color");
         self._selUpdate();
     };
 
     this.selectInRect = function(x1, y1, x2, y2) {
         /* find all cells within a rectangle and add them to the selection. */
         var minX = Math.min(x1, x2);
         var maxX = Math.max(x1, x2);
 
         var minY = Math.min(y1, y2);
         var maxY = Math.max(y1, y2);
 
         console.time("select");
-        var pxCoords = self.coords.px;
+        if (self.selCells === null)
+            self.selCells = [];
+
+        var pxCoords = self.pxCoords;
         for (var i = 0; i < pxCoords.length / 2; i++) {
             var pxX = pxCoords[2 * i];
             var pxY = pxCoords[2 * i + 1];
-            if (isHidden(pxX, pxY))
+            if (pxX === 0 && pxY === 0)
                 continue;
             if ((minX <= pxX) && (pxX <= maxX) && (minY <= pxY) && (pxY <= maxY)) {
-                self.selCells.add(i);
+                self.selCells.push(i);
             }
 
         }
         console.timeEnd("select");
         self._selUpdate();
     };
 
-    this.getSelection = function() {
-        /* return selected cells as a list of ints */
-        var cellIds = [];
-        self.selCells.forEach(function(x) {
-            cellIds.push(x)
-        });
-        return cellIds;
-    };
-
-    this.selectInvert = function() {
-        /* invert selection */
-        var selCells = self.selCells;
-        var cellCount = self.getCount();
-        for (let i = 0; i < cellCount; i++) {
-            if (selCells.has(i)) {
-                selCells.delete(i);
-            } else {
-                selCells.add(i);
-            }
-        }
-        self.selCells = selCells;
-        self._selUpdate();
-    };
-
-    this.getCount = function() {
-        /* return maximum number of cells in dataset, may include hidden cells, see isHidden() */
-        return self.coords.orig.length / 2;
-    };
-
-    // END SELECTION METHODS (could be an object?)
-
     this._selUpdate = function() {
         /* called after the selection has been updated, calls the onSelChange callback */
-        setStatus(self.selCells.size + " " + self.gSampleDescription + "s selected");
+        setStatus(self.selCells.length + " " + self.gSampleDescription + "s selected");
         if (self.onSelChange !== null)
             self.onSelChange(self.selCells);
     }
 
     this.moveBy = function(xDiff, yDiff) {
         /* update the pxCoords by a certain x/y distance and redraw */
 
         // convert pixel range to data scale range
-        var zr = self.port.zoomRange;
+        var zr = self.zoomRange;
         var xDiffData = xDiff * ((zr.maxX - zr.minX) / self.canvas.width);
         var yDiffData = yDiff * ((zr.maxY - zr.minY) / self.canvas.height);
 
-        // move zoom range
+        // move zoom range 
         zr.minX = zr.minX + xDiffData;
         zr.maxX = zr.maxX + xDiffData;
         zr.minY = zr.minY + yDiffData;
         zr.maxY = zr.maxY + yDiffData;
 
         self.scaleData();
-
-        // a special case for connected plots that are not sharing our pixel coordinates
-        if (self.childPlot && self.coords !== self.childPlot.coords) {
-            self.childPlot.moveBy(xDiff, yDiff);
-        }
     };
 
     this.labelAt = function(x, y) {
-        /* return the index and the text of the label at position x,y or null if nothing there */
+        /* return the text of the label at position x,y or null if nothing there */
         //console.time("labelCheck");
-        var clusterLabels = self.coords.labels;
+        var clusterLabels = self.clusterLabels;
         if (clusterLabels === null || clusterLabels === undefined)
             return null;
-        var labelCoords = self.coords.labels;
-        var boxes = self.coords.labelBbox;
-
-        if (boxes == null) // no cluster labels
-            return null;
+        var labelCoords = self.pxLabels;
+        var boxes = self.pxLabelBbox;
 
         if (labelCoords.length !== clusterLabels.length)
             alert("internal error maxPLot.js: coordinates of labels are different from clusterLabels");
 
         for (var i = 0; i < labelCoords.length; i++) {
             var box = boxes[i];
             if (box === null) // = outside of the screen
                 continue;
+            var labelText = clusterLabels[i][2];
             var x1 = box[0];
             var y1 = box[1];
             var x2 = box[2];
             var y2 = box[3];
             if ((x >= x1) && (x <= x2) && (y >= y1) && (y <= y2)) {
                 //console.timeEnd("labelCheck");
-                var labelText = clusterLabels[i][2];
-                return [labelText, i];
+                return labelText;
             }
         }
         //console.timeEnd("labelCheck");
         return null;
     }
 
     this.cellsAt = function(x, y) {
         /* check which cell's bounding boxes contain (x, y), return a list of the cell IDs, sorted by distance */
-        //console.time("cellSearch");
-        var pxCoords = self.coords.px;
+        console.time("cellSearch");
+        var pxCoords = self.pxCoords;
         if (pxCoords === null)
             return null;
         var possIds = [];
-        var radius = self.port.radius;
         for (var i = 0; i < pxCoords.length / 2; i++) {
             var pxX = pxCoords[2 * i];
             var pxY = pxCoords[2 * i + 1];
-            if (isHidden(pxX, pxY))
+            if (pxX === 0 && pxY === 0)
                 continue;
-            var x1 = pxX - radius;
-            var y1 = pxY - radius;
-            var x2 = pxX + radius;
-            var y2 = pxY + radius;
+            var x1 = pxX - self.radius;
+            var y1 = pxY - self.radius;
+            var x2 = pxX + self.radius;
+            var y2 = pxY + self.radius;
             if ((x >= x1) && (x <= x2) && (y >= y1) && (y <= y2)) {
                 var dist = Math.sqrt(Math.pow(x - pxX, 2) + Math.pow(y - pxY, 2));
                 possIds.push([dist, i]);
             }
         }
 
-        //console.timeEnd("cellSearch");
+        console.timeEnd("cellSearch");
         if (possIds.length === 0)
             return null;
         else {
             possIds.sort(function(a, b) {
                 return a[0] - b[0]
             }); // sort by distance
 
             // strip the distance information
             var ret = [];
-            for (let i = 0; i < possIds.length; i++) {
+            for (var i = 0; i < possIds.length; i++) {
                 ret.push(possIds[i][1]);
             }
             return ret;
         }
     };
 
+    this.getSelection = function() {
+        /* return selected cells as a list of ints */
+        return self.selCells;
+    };
+
     this.resetMarquee = function() {
         /* make the marquee disappear and reset its internal status */
-        if (!self.interact)
-            return;
-
         self.mouseDownX = null;
         self.mouseDownY = null;
         self.lastPanX = null;
         self.lastPanY = null;
         self.selectBox.style.display = "none";
         self.selectBox.style.width = 0;
         self.selectBox.style.height = 0;
     };
 
-    this.drawMarquee = function(x1, y1, x2, y2, forceAspect) {
+    this.drawMarquee = function(x1, y1, x2, y2) {
         /* draw the selection or zooming marquee using the DIVs created by setupMouse */
         var selectWidth = Math.abs(x1 - x2);
-        var selectHeight = 0;
-        if (forceAspect) {
-            var aspectRatio = self.width / self.canvas.height;
-            selectHeight = selectWidth / aspectRatio;
-        } else
-            selectHeight = Math.abs(y1 - y2);
-
+        var selectHeight = Math.abs(y1 - y2);
         var minX = Math.min(x1, x2);
         var minY = Math.min(y1, y2);
         var div = self.selectBox;
-        div.style.left = (minX - self.left) + "px";
-        div.style.top = (minY - self.top) + "px";
+        div.style.left = minX + "px";
+        div.style.top = minY + "px";
         div.style.width = selectWidth + "px";
         div.style.height = selectHeight + "px";
         div.style.display = "block";
     };
 
-    this.activatePlot = function() {
-        /* draw black border around plot, remove black border from all connected plots, call onActive */
-        if (self.parentPlot === null)
-            return false;
-
-        // only need to do something if we're not already the active plot
-        self.canvas.style["border"] = "2px solid black";
-        self.parentPlot.canvas.style["border"] = "2px solid white";
-
-        // flip the parent/child relationship
-        self.childPlot = self.parentPlot;
-        self.childPlot.parentPlot = self;
-        self.parentPlot = null;
-        self.childPlot.childPlot = null;
-
-        // hide/show the tool and zoom buttons
-        self.childPlot.zoomDiv.style.display = "none";
-        self.childPlot.toolDiv.style.display = "none";
-        self.zoomDiv.style.display = "block";
-        self.toolDiv.style.display = "block";
-
-        // notify the UI
-        self.onActiveChange(self);
-        return true;
-    }
+    //this.onHamster = function(ev, delta, deltaX, deltaY) {
+    //console.log(delta, deltaX, deltaY);
+    //console.log(ev);
+    //var pxX = ev.originalEvent.clientX - self.left;
+    //var pxY = ev.originalEvent.clientY - self.top;
+    //self.zoomBy(1+(0.01*delta), pxX, pxY);
+    //self.drawDots();
+    //ev.preventDefault();
+    //};
 
     this.onMouseMove = function(ev) {
         /* called when the mouse is moved over the Canvas */
 
         // set a timer so we can get "hover" functionality without too much CPU
-        if (self.timer !== null)
+        if (self.timer != null)
             clearTimeout(self.timer);
-        self.timer = setTimeout(self.onNoMouseMove, 130);
+        self.timer = setTimeout(self.onNoMouseMove, 170);
         // save mouse pos for onNoMouseMove timer handler
         self.lastMouseX = ev.clientX;
         self.lastMouseY = ev.clientY;
 
         // label hit check requires canvas coordinates x/y
         var clientX = ev.clientX;
         var clientY = ev.clientY;
         var canvasTop = self.top;
         var canvasLeft = self.left;
         var xCanvas = clientX - canvasLeft;
         var yCanvas = clientY - canvasTop;
 
-        // when the cursor is over a label, change it to a hand, but only when there is no marquee
-        if (self.coords.labelBbox !== null && self.mouseDownX === null) {
+        // when the cursor is over a label, change it to a hand
+        if (self.pxLabelBbox !== null && self.pxLabels !== null) {
             var labelInfo = self.labelAt(xCanvas, yCanvas);
-            if (labelInfo === null) {
+            if (labelInfo === null)
                 self.canvas.style.cursor = self.canvasCursor;
-                self.onNoLabelHover(ev);
-            } else {
+            else {
                 self.canvas.style.cursor = 'pointer'; // not 'hand' anymore ! and not 'grab' yet!
                 if (self.onLabelHover !== null)
-                    self.onLabelHover(labelInfo[0], labelInfo[1], ev);
+                    self.onLabelHover(labelInfo, ev);
             }
         }
 
         if (self.mouseDownX !== null) {
-            // we're panning
-            if (((ev.altKey || self.dragMode === "move")) && self.panCopy !== null) {
+            if ((ev.altKey || self.dragMode === "move") && self.panCopy !== null) {
                 var xDiff = self.mouseDownX - clientX;
                 var yDiff = self.mouseDownY - clientY;
                 self.panBy(xDiff, yDiff);
-            } else {
-                // zooming or selecting
-                var forceAspect = false;
-                var anyKey = (ev.metaKey || ev.altKey || ev.shiftKey);
-                if ((self.dragMode === "zoom" && !anyKey) || ev.metaKey)
-                    forceAspect = true;
-                self.drawMarquee(self.mouseDownX, self.mouseDownY, clientX, clientY, forceAspect);
-            }
+            } else
+                self.drawMarquee(self.mouseDownX, self.mouseDownY, clientX, clientY);
         }
     };
 
     this.onNoMouseMove = function() {
         /* called after some time has elapsed and the mouse has not been moved */
-        if (self.coords.px === null)
-            return;
         var x = self.lastMouseX - self.left; // need canvas, not screen coordinates
         var y = self.lastMouseY - self.top;
         var cellIds = self.cellsAt(x, y);
         // only call onNoCellHover if callback exists and there is nothing selected
         if (cellIds === null && self.onNoCellHover !== null && self.selCells === null)
             self.onNoCellHover();
         else if (self.onCellHover !== null)
             self.onCellHover(cellIds);
     };
 
-
     this.onMouseDown = function(ev) {
         /* user clicks onto canvas */
-        if (self.activatePlot())
-            return; // ignore the first click into the plot, if it was the activating click
-        debug("background mouse down");
+        console.log("background mouse down");
         var clientX = ev.clientX;
         var clientY = ev.clientY;
-        if ((ev.altKey || self.dragMode === "move") && !ev.shiftKey && !ev.metaKey) {
-            debug("alt key or move mode: starting panning");
+        if (ev.altKey || self.dragMode === "move") {
+            console.log("alt key or move mode: starting panning");
             self.panStart();
         }
         self.mouseDownX = clientX;
         self.mouseDownY = clientY;
     };
 
     this.onMouseUp = function(ev) {
-        debug("background mouse up");
+        console.log("background mouse up");
         // these are screen coordinates
         var clientX = ev.clientX;
         var clientY = ev.clientY;
         var mouseDidNotMove = (self.mouseDownX === clientX && self.mouseDownY === clientY);
 
         if (self.panCopy !== null && !mouseDidNotMove) {
-            debug("ending panning operation");
+            console.log("ending panning operation");
             self.panEnd();
             self.mouseDownX = null;
             self.mouseDownY = null;
             self.drawDots();
             return;
-        } else {
-            // abort panning
-            self.panCopy = null;
         }
 
         if (self.mouseDownX === null && self.lastPanX === null) {
             // user started the click outside of the canvas: do nothing
-            debug("first click must have been outside of canvas");
+            console.log("first click must have been outside of canvas");
             return;
         }
 
         // the subsequent operations require canvas coordinates x/y
         var canvasTop = self.top;
         var canvasLeft = self.left;
         var x1 = self.mouseDownX - canvasLeft;
         var y1 = self.mouseDownY - canvasTop;
         var x2 = clientX - canvasLeft;
         var y2 = clientY - canvasTop;
 
         // user did not move the mouse, so this is a click
         if (mouseDidNotMove) {
-            // recognize a double click -> zoom
-            if (self.lastClick !== undefined && x2 === self.lastClick[0] && y2 === self.lastClick[1]) {
-                self.zoomBy(1.33);
-                self.lastClick = [-1, -1];
-            } else {
-                self.lastClick = [x2, y2];
-            }
-
-            var labelInfo = self.labelAt(x2, y2);
-            if (labelInfo !== null && self.doDrawLabels)
-                self.onLabelClick(labelInfo[0], labelInfo[1], ev);
+            var clickedLabel = self.labelAt(x2, y2);
+            if (clickedLabel !== null)
+                self.onLabelClick(clickedLabel, ev);
             else {
                 var clickedCellIds = self.cellsAt(x2, y2);
-                // click on a cell -> update selection and redraw
                 if (clickedCellIds !== null && self.onCellClick !== null) {
-                    self.selectClear(true);
-                    for (var i = 0; i < clickedCellIds.length; i++) {
-                        self.selCells.add(clickedCellIds[i]);
-                    }
-                    self.drawDots();
+                    self.selCells = clickedCellIds;
                     self.onCellClick(clickedCellIds, ev);
-
+                    self.drawDots();
                 } else {
                     // user clicked onto background:
                     // reset selection and redraw
-                    debug("not moved at all: reset " + clientX + " " + self.mouseDownX + " " + self.mouseDownY + " " + clientY);
+                    console.log("not moved at all: reset " + clientX + " " + self.mouseDownX + " " + self.mouseDownY + " " + clientY);
                     self.selectClear();
-
                     self.drawDots();
                 }
 
                 self.lastPanX = null;
                 self.lastPanY = null;
             }
             self.mouseDownX = null;
             self.mouseDownY = null;
             return;
         }
-        //debug("moved: reset "+x+" "+mouseDownX+" "+mouseDownY+" "+y);
+        //console.log("moved: reset "+x+" "+mouseDownX+" "+mouseDownY+" "+y);
 
         // it wasn't a click, so it was a drag
         var anyKey = (ev.metaKey || ev.altKey || ev.shiftKey);
 
         // zooming
-        if ((self.dragMode === "zoom" && !anyKey) || ev.metaKey) {
-            // get current coords of the marquee in canvas pixels
-            var div = self.selectBox;
-            let zoomX1 = parseInt(div.style.left.replace("px", ""));
-            let zoomY1 = parseInt(div.style.top.replace("px", ""));
-            let zoomX2 = zoomX1 + parseInt(div.style.width.replace("px", ""));
-            let zoomY2 = zoomY1 + parseInt(div.style.height.replace("px", ""));
-            zoomY1 = self.canvas.height - zoomY1;
-            zoomY2 = self.canvas.height - zoomY2;
-            self.zoomTo(zoomX1, zoomY1, zoomX2, zoomY2);
-            // switch back to the mode before zoom was clicked
-            if (self.prevMode) {
-                self.activateMode(self.prevMode);
-                self.prevMode = null;
-            }
-
-
-        }
-        // marquee select
+        if ((self.dragMode === "zoom" && !anyKey) || ev.metaKey)
+            self.zoomTo(x1, y1, x2, y2);
+        // marquee select 
         else if ((self.dragMode === "select" && !anyKey) || ev.shiftKey) {
             if (!ev.shiftKey)
-                self.selectClear(true);
+                self.selectClear();
             self.selectInRect(x1, y1, x2, y2);
         } else {
-            debug("Internal error: no mode?");
+            console.log("Internal error: no mode?");
         }
 
         self.resetMarquee();
 
         self.drawDots();
     };
 
-    function drawCirclesSvg(svgLines, pxCoords, coordColors, colors, radius, alpha, selCells) {
-        /* add SVG text to the array svgLines */
-        debug("Drawing " + coordColors.length + " circles with SVG renderer");
-        var count = 0;
-        for (var i = 0; i < pxCoords.length / 2; i++) {
-            var pxX = pxCoords[2 * i];
-            var pxY = pxCoords[2 * i + 1];
-            if (isHidden(pxX, pxY))
-                continue;
-            var col = colors[coordColors[i]];
-
-            svgLines.push("<circle cx='" + pxX + "' cy='" + pxY + "' r='" + radius + "' fill-opacity='" + alpha + "' fill='#" + col + "' />");
-            count++;
-        }
-        return count;
-    }
-
     this.onWheel = function(ev) {
         /* called when the user moves the mouse wheel */
-        if (self.parentPlot !== null)
-            return;
-        debug(ev);
+        console.log(ev);
         var normWheel = normalizeWheel(ev);
-        debug(normWheel);
+        console.log(normWheel);
         var pxX = ev.clientX - self.left;
         var pxY = ev.clientY - self.top;
         var spinFact = 0.1;
-        if (ev.ctrlKey) // = OSX pinch and zoom gesture (and no other OS/mouse combination?)
-            spinFact = 0.08; // is too fast, so slow it down a little
+        if (ev.ctrlKey) // = OSX pinch and zoom gesture
+            spinFact = 0.02; // is too fast, so slow it down a little
         var zoomFact = 1 - (spinFact * normWheel.spinY);
-        debug("Wheel Zoom by " + zoomFact);
+        console.log("Wheel Zoom by " + zoomFact);
         self.zoomBy(zoomFact, pxX, pxY);
         self.drawDots();
         ev.preventDefault();
         ev.stopPropagation();
     };
 
     this.setupMouse = function() {
@@ -2326,228 +1653,64 @@
         self.canvas.addEventListener("wheel", self.onWheel);
     };
 
     this.setShowLabels = function(doShow) {
         self.doDrawLabels = doShow;
     };
 
-    this.getLabels = function() {
-        /* get current labels */
-        var ret = [];
-        var labels = self.coords.labels;
-        for (var i = 0; i < labels.length; i++)
-            ret.push(labels[i][2]);
-        return ret;
-    }
-
-    this.setLabels = function(newLabels) {
-        /* set new label text */
-        if (newLabels.length !== self.coords.labels.length) {
-            debug("maxPlot:setLabels error: new labels have wrong length.");
-            return;
-        }
-
-        for (var i = 0; i < newLabels.length; i++)
-            self.coords.labels[i][2] = newLabels[i];
-
-        self.coords.pxLabels = scaleLabels(self.coords.labels, self.port.zoomRange, self.port.radius,
-            self.canvas.width, self.canvas.height);
-
-        // a special case for connected plots that are not sharing our pixel coordinates
-        if (self.childPlot && self.coords !== self.childPlot.coords) {
-            self.childPlot.setLabels(newLabels);
-        }
-    };
-
-    this._setLines = function(lines, attrs) {
-        if (lines === undefined)
-            return;
-        self.coords.lines = lines;
-
-        if (!attrs)
-            self.coords.lineAttrs = {};
-        else
-            self.coords.lineAttrs = attrs;
-    }
-
     this.activateMode = function(modeName) {
         /* switch to one of the mouse drag modes: zoom, select or move */
-        if (modeName === "zoom")
-            self.prevMode = self.dragMode;
-        else
-            self.prevMode = null;
-
         self.dragMode = modeName;
 
         var cursor = null;
 
         if (modeName === "move")
             cursor = 'all-scroll';
         else if (modeName === "zoom")
-            cursor = "zoom-in"
-        else if (modeName == "select")
             cursor = 'crosshair';
-        //else
-        //cursor= 'default';
+        else
+            cursor = 'default';
 
         self.canvas.style.cursor = cursor;
         self.canvasCursor = cursor;
 
         self.resetMarquee();
 
-        if (self.interact) {
-            self.icons["move"].style.backgroundColor = gButtonBackground;
-            self.icons["zoom"].style.backgroundColor = gButtonBackground;
-            self.icons["select"].style.backgroundColor = gButtonBackground;
-            self.icons[modeName].style.backgroundColor = gButtonBackgroundClicked;
-        }
-        if (self.childPlot)
-            self.childPlot.activateMode(modeName);
+        self.icons["move"].style.backgroundColor = gButtonBackground;
+        self.icons["zoom"].style.backgroundColor = gButtonBackground;
+        self.icons["select"].style.backgroundColor = gButtonBackground;
+        self.icons[modeName].style.backgroundColor = gButtonBackgroundClicked;
+
+        //var upModeName = modeName[0].toUpperCase() + modeName.slice(1);
+        //var buttonId = "mpIconMode"+upModeName;
     }
 
     this.randomDots = function(n, radius, mode) {
         /* draw x random dots with x random colors*/
-        function randomArray(ArrType, length, max) {
+        function randomArray(arrType, length, max) {
             /* make Array and fill it with random numbers up to max */
-            var arr = new ArrType(length);
+            var arr = new arrType(length);
             for (var i = 0; i < length; i++) {
                 arr[i] = Math.round(Math.random() * max);
             }
             return arr;
         }
 
         if (mode !== undefined)
             self.mode = mode;
-        self.port.radius = radius;
+        self.radius = radius;
         self.setCoords(randomArray(Uint16Array, 2 * n, 65535));
         self.setColors(["FF0000", "00FF00", "0000FF", "CC00CC", "008800"]);
         self.setColorArr(randomArray(Uint8Array, n, 4));
 
         console.time("draw");
         self.drawDots();
         console.timeEnd("draw");
         return self;
-    };
-
-    this.split = function() {
-        /* reduce width of renderer, create new renderer and place both side-by-side.
-         * They initially share the .coords but setCoords() can break that relationship.
-         * */
-        var canvHeight = self.canvas.height;
-        var canvLeft = self.left;
-        var newWidth = self.width / 2;
-        var newTop = self.top;
-        var newLeft = self.left + newWidth;
-        var newHeight = canvHeight + gStatusHeight;
-
-        var newDiv = document.createElement('div');
-        newDiv.id = "mpPlot2";
-        document.body.appendChild(newDiv);
-
-        var opts = cloneObj(self.globalOpts);
-        opts.showClose = true;
-
-        var plot2 = new MaxPlot(newDiv, newTop, newLeft, newWidth, newHeight, {
-            "showClose": true
-        });
-        //plot2.canvas.style.borderLeft = "1px solid grey";
-
-        plot2.statusLine.style.display = "none";
-
-        plot2.port = self.port;
-        plot2.selCells = self.selCells;
-
-        plot2.coords = self.coords;
 
-        plot2.col = {};
-        plot2.col.pal = self.col.pal;
-        plot2.col.arr = self.col.arr;
-
-        if (self.background)
-            plot2.setBackground(self.background.img);
-
-        self.setSize(newWidth, newHeight, false); // will call scaleData(), but not redraw.
-
-        plot2.onLabelClick = self.onLabelClick;
-        plot2.onCellClick = self.onCellClick;
-        plot2.onCellHover = self.onCellHover;
-        plot2.onNoCellHover = self.onNoCellHover;
-        plot2.onSelChange = self.onSelChange;
-        plot2.onLabelHover = self.onLabelHover;
-        plot2.onNoLabelHover = self.onNoLabelHover;
-        plot2.onActiveChange = self.onActiveChange;
-
-        plot2.drawDots();
-
-        self.childPlot = plot2;
-        plot2.parentPlot = self;
-
-        // add a thick border and hide the menus in the child
-        self.canvas.style["border"] = "2px solid black";
-        self.childPlot.zoomDiv.style.display = "none";
-        self.childPlot.toolDiv.style.display = "none";
-
-        return plot2;
     };
 
-    this.unsplit = function() {
-        /* remove the connected non-active renderer */
-        //var canvWidth = window.innerWidth - canvLeft - legendBarWidth;
-        var otherRend = self.childPlot;
-        self.childPlot = undefined;
-        if (!otherRend) {
-            otherRend = self.parentPlot;
-            self.parentPlot = undefined;
-        }
-        self.setSize(self.width * 2, self.height, false);
-
-
-        otherRend.div.remove();
-        self.canvas.style["border"] = "none";
-        return;
-    }
-
-    this.getWidth = function() {
-        /* return total size of renderer, including any split child renderers */
-        if (self.childPlot)
-            return self.width + self.childPlot.width;
-        else
-            return self.width;
-    }
-
-    this.calcMedian = function(coords, values, names, numNames) {
-        /* given an array of coordinates (x at even positions, y at odd positions) and an array of names for each of them
-         * return the median for each name as an object name -> array of [x, y, count]
-         * if names is undefined, will use numNames and convert to two decimals 
-         * */
-        var calc = {};
-        for (var i = 0, I = values.length; i < I; i++) {
-            var label = null;
-            if (names) {
-                label = names[values[i]];
-            } else {
-                label = numNames[i].toFixed(2);
-            }
-            if (calc[label] === undefined) {
-                calc[label] = [
-                    [],
-                    [], 0
-                ]; // all X, all Y, count
-            }
-            var x = coords[i * 2];
-            var y = coords[i * 2 + 1];
-
-            if (isHidden(x, y))
-                continue;
-
-            calc[label][0].push(x);
-            calc[label][1].push(y);
-            calc[label][2] += 1;
-        }
-        return calc;
-    }
-
     // object constructor code
     self.initCanvas(div, top, left, width, height);
     self.initPlot(args);
 
 }
```

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/convert.py` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/hubmaker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,762 +1,890 @@
-# various format converters for single cell data:
-# - cellranger, mtx to tsv, matcat, metaCat etc
+# create a track hub from an expression matrix
 
-import logging, optparse, io, sys, os, shutil, operator, glob, re, json, subprocess
-from collections import defaultdict, OrderedDict
+import subprocess, colorsys
+import logging, sys, optparse, re, unicodedata, string, glob, distutils.spawn, gzip
+from collections import defaultdict, namedtuple
+from os.path import join, basename, dirname, isfile, isdir, splitext
+import os
+
+import sys
+import cellbrowser
+
+CBEMAIL = os.getenv("CBEMAIL", "unknown")
+
+# ==== functions =====
+    
+def cbHub_parseArgs():
+    " setup logging, parse command line arguments and options. -h shows auto-generated help page "
+    parser = optparse.OptionParser("""usage: %prog [options] - create a UCSC track hub for a single cell dataset
 
-from .cellbrowser import runGzip, openFile, errAbort, setDebug, moveOrGzip, makeDir, iterItems
-from .cellbrowser import mtxToTsvGz, writeCellbrowserConf, getAllFields, readMatrixAnndata, adataStringFix
-from .cellbrowser import anndataMatrixToTsv, loadConfig, sanitizeName, lineFileNextRow, scanpyToCellbrowser, build
-from .cellbrowser import generateHtmls, getObsKeys, renameFile, getMatrixFormat, generateDataDesc
-from .cellbrowser import copyFileIfDiffSize
+    Run the program with "--init" to write a sample cellbrowser.conf into the current directory.
+    Adapt this file to your needs. For %prog, only the parts under "hub" are relevant.
 
-from os.path import join, basename, dirname, isfile, isdir, relpath, abspath, getsize, getmtime, expanduser
+    Call the program without any arguments if there is cellbrowser.conf in the current dir:
+    %prog
+    It will read cellbrowser.conf, create hub.txt and write the job scripts.
+    You can then run the job scripts as described below.
+
+    This will create one shell script per cell cluster, with names like 'job-xxx.sh',
+    in the current directory. To run these scripts in parallel on a big server,
+    e.g. with 10 processes use the Unix command "parallel":
+      ls *.sh | parallel -j 10 bash
+
+    Each job will write a log of stdout/stderr to files named e.g. job-1.log
+
+    Requirements that have to be installed on this machine with binaries in PATH:
+    - samtools https://github.com/samtools/samtools
+    - wiggletools https://github.com/Ensembl/WiggleTools
+    - intronProspector https://github.com/diekhans/intronProspector
+    - UCSC tools wigToBigWig, bedToBigBed from http://hgdownload.soe.ucsc.edu/admin/exe/
 
-def cbToolCli_parseArgs(showHelp=False):
-    " setup logging, parse command line arguments and options. -h shows auto-generated help page "
-    parser = optparse.OptionParser("""usage: %prog [options] command filenames - convert various single-cell related files
+    Run the UCSC tool hubCheck on the resulting hub.txt to make sure that all jobs
+    have successfully completed.
 
-Command is one of:
-    mtx2tsv   - convert matrix market to .tsv.gz
-    matCatCells - merge expression matrices into a big tsv.gz matrix.
-        If you have files from different cells, same assay, same genes, this
-        allows to merge them into a bigger matrix. Format is one-line-per-gene.
-        Matrices must have identical genes in the same order and the same number of
-        lines. Handles .csv files, otherwise defaults to tab-sep input. gzip OK.
-    matCatGenes - concatenate expression matrices. If you have data from the same cells but with different
-        assays (multi-modal), this allows to merge them and add a prefix to every gene.
-    metaCat - concat/join meta tables on the first (cell ID) field or reorder their fields
-    reorder - reorder the meta fields
-
-Examples:
-    - %prog mtx2tsv matrix.mtx genes.tsv barcodes.tsv exprMatrix.tsv.gz - convert .mtx to .tsv.gz file
-    - %prog matCatCells mat1.tsv.gz mat2.tsv.gz exprMatrix.tsv.gz - merge expression matrices
-    - %prog matCatGenes mat1.csv.gz mat2.tsv.gz=atac- exprMatrix.tsv.gz - concatenate expression matrices
-           and prefix all genes in the second file with 'atac-'
-    - %prog metaCat meta.tsv seurat/meta.tsv scanpy/meta.tsv newMeta.tsv - merge meta matrices
-    - %prog reorder meta.tsv meta.newOrder.tsv --delete samId --order=cluster,cellType,age - reorder meta fields
+    You can override some settings in cellbrowser.conf with the command line options:
+    %prog -m metaFname -c clusterField -m exprMatrix -o hubDir
     """)
 
-    parser.add_option("-d", "--debug", dest="debug", action="store_true",
-        help="show debug messages")
-    parser.add_option("", "--fixDots", dest="fixDots", action="store_true",
-            help="for reorder and metaCat: try to fix R's mangling of various special chars to '.' in the cell IDs")
-    parser.add_option("", "--order", dest="order", action="store",
-        help="only for reorder and metaCat: new order of fields, comma-sep, e.g. 'disease,age'. Do not include cellId, it's always the first field by definition. Fields that are in the file but not specified here will be appended as the last columns.")
-    parser.add_option("", "--del", dest="delFields", action="store",
-        help="only for reorder and metaCat: names of fields to remove")
-
+    parser.add_option("", "--init", dest="init", action="store_true", \
+            help="write a sample cellbrowser.conf to the current directory")
 
+    parser.add_option("-i", "--inConf", dest="inConf", action="store", \
+            help="a cellbrowser.conf input file to read all options from, default %default", \
+            default = "cellbrowser.conf")
+
+    #parser.add_option("-g", "--genome", dest="genome", action="store", \
+            #help="a ucsc assembly identifier, like hg19, hg38 or mm10")
+
+    parser.add_option("-m", "--metaFname", dest="meta", action="store", \
+            help="a csv or tsv matrix, one row per cell")
+
+    parser.add_option("-e", "--exprMatrix", dest="exprMatrix", action="store", \
+            help="exprMatrix is a tsv or csv expression matrix, one line per cell")
+
+    parser.add_option("-c", "--clusterField", dest="clusterField", action="store", \
+            help="field in expr matrix that contains the cluster name")
+
+    parser.add_option("-o", "--hubDir", dest="hubDir", action="store", \
+            help="the output directory for the hub, default is %default")
+
+    parser.add_option("-d", "--debug", dest="debug", action="store_true", help="show debug messages")
+    #parser.add_option("", "--fixDot", dest="fixDot", action="store_true", help="replace dots in cell meta IDs with dashes (for R)")
+    #parser.add_option("-t", "--geneType", dest="geneType", help="type of gene IDs in expression matrix. values like 'symbols', or 'gencode22', 'gencode28' or 'gencode-m13'.")
+    #parser.add_option("", "--bamDir", dest="bamDir", help="directory with BAM files, one per cell. Merges small BAM files into one per cell cluster.")
+    parser.add_option("", "--clusterOrder", dest="clusterOrder", help="file with cluster names in the order that they should appear in the track. default is alphabetical order.")
+    parser.add_option("-s", "--skipBarchart", dest="skipBarchart", help="do not create the bar chart graph", action="store_true")
+    #parser.add_option("", "--name", dest="name", help="name of track hub.")
+    #parser.add_option("", "--email", dest="email", help="contact email for track hub. Default is %default, taken from the env. variable CBEMAIL", default=CBEMAIL)
+    #parser.add_option("-f", "--file", dest="file", action="store", help="run on file") 
+    #parser.add_option("", "--test", dest="test", action="store_true", help="do something") 
     (options, args) = parser.parse_args()
 
-    if showHelp:
+    if not options.exprMatrix and not isfile(options.inConf) and not options.init:
         parser.print_help()
         exit(1)
 
-    setDebug(options.debug)
+    cellbrowser.setDebug(options.debug)
     return args, options
 
-def cbToolCli():
-    " run various tools from the command line "
-    args, options = cbToolCli_parseArgs()
+def parseClustersFromMeta(metaFname, clusterFieldName, fixDot):
+    " parse cluster -> cellId assignment from meta file, return as dict clusterName -> list of cellIds "
+    logging.info("Parsing and using first field as the cell ID in file %s" % metaFname)
+    clusterToCells = defaultdict(list)
+    metaCellIds = set()
+    skipCount = 0
+    for row in cellbrowser.lineFileNextRow(metaFname):
+        clusterName = row._asdict()[clusterFieldName]
+        cellId = row[0]
+        if fixDot:
+            cellId = cellId.replace(".", "-")
+
+        # skip all cells assigned to the "" cluster
+        if clusterName=="":
+            skipCount +=1
+            continue
+
+        if cellId in metaCellIds:
+            errAbort("duplicated cell ID %s in meta data" % cellId)
+
+        metaCellIds.add(cellId)
+        clusterToCells[clusterName].append(cellId)
+
+    logging.info("Got %d clusters and %d cell IDs assigned to them" % (len(clusterToCells), len(metaCellIds)))
+    if skipCount!=0:
+        logging.info("Skipped %d meta rows with empty cluster names" % skipCount)
+    return clusterToCells
+
+# ----------- main --------------
+
+def writeHubStanza(tfh, hubName, db, email):
+    "  write a single-file hub.txt "
+    tfh.write("""hub scHub
+shortLabel %s
+longLabel %s
+useOneFile on
+email %s
+descriptionUrl hub.txt
+
+genome %s
+
+""" % (hubName, hubName, email, db))
+
+def writeDescPages(hubDir, hubName, hubUrl, refHtmlFname):
+    saneHubName = sanitizeName(hubName)
+    readDesc = join(hubDir, saneHubName+".html")
+    readFh = open(readDesc, "w")
+    hubBase = hubUrl.rsplit("/")[0]
+    refHtml = ""
+    if refHtmlFname is not None:
+        refHtml = open(refHtmlFname).read()
+
+    readFh.write("""
+<h2>Description</h2>
+<p>This track shows the alignment of sequencing reads to the genome, their coverage and the splice junctions in them. This can be helpful for quality checking of cluster markers, when designing in-situ probes or when trying to determine how specific a transcript is for a given cell type.
+
+<h2>Display Conventions and Configuration</h2>
+
+<p>This track has multiple "Views", which can be configured independently. See
+the <a href="/goldenPath/help/multiView.html">documentation on Multi-View
+tracks</a>. There are three different types of view sub tracks in this track:</a>
+
+<p><b>BAM Reads:</b> Alignable regions are shown in black, unalignable regions
+between two alignable ones shown with thin lines. For configuration options,
+see <a href="https://genome.ucsc.edu/goldenpath/help/hgBamTrackHelp.html">the
+BAM tracks help page</a>. By default, these tracks are hideen, set any of them to "squish" or "pack" (=clickable) on the track configuration page to see the reads. Click reads to show the alignment and read group.</p>
+
+<p><b>Coverage:</b> bar graphs indicate the number of reads at this base pair.
+You may want to switch on auto-scaling of the y axis. For configuration
+options, see <a
+href="https://genome.ucsc.edu/goldenpath/help/hgWiggleTrackHelp.html">the graph
+tracks configuration help page</a>. These tracks are shown in "dense" by default, set any of the tracks to "full" to see the detailed coverage plot.</p>
+
+<p><b>Splice Junctions:</b> thick rectangles show exons around a splice site,
+connected by a line that indicates the intron. These gaps are shown and are
+annotated with the number of reads, in the 'score' field. You can use the
+'score' filter on the track configuration page to show only introns with a
+certain number of supporting reads. The maximum number of reads that are shown
+is 1000, even if more reads support an intron. These tracks are shown in dense by default, set this track to "pack" to see. Then click the splice junctions to see their score.</p>
+
+<h2>Methods</h2>
+<p>BAM files were provided by the data submitters, one (single end) or two files (paired end) per cell. The BAM alignments were used as submitted. They were merged with "samtools merge" into a single BAM file per cluster. The readgroup (RG) BAM tag indicates the original cell.</p>
+
+<p>From the resulting merged BAM file, coverage was obtained using "wiggletools coverage" a tool written by Daniel Zerbino and the result was converted with the UCSC tool "wigToBigWig".</p>
+
+<p>Also on the merged BAM file, the software IntronProspector was run with default settings. It retains reads with a gap longer than 70 bp and shorter than 500 kbp and merges them into annotated splice junctions.</p>
+
+<h2>Data Access</h2>
+<p>The merged BAM files, coverage bigWig files and splice junctions in bigBed format can be downloaded from the <a href='{hubBase}'>track hub directory</a>.</p>
+
+<p>Since the splice junction .bigBed files have their scores capped at 1000, the original IntronProspector .bed files can also be downloaded from the <a href='{hubBase}'>track hub directory</a>. You can also find there *.calls.tsv files with more details about each junction, e.g. the number of uniquely mapping reads.</p>
+
+<h2>Credits</h2>
+<p>WiggleTools was written by Daniel Zerbino, IntronProspector was written by Mark Diekhans, track hubs were written to a large extent by Brian Raney.</p>
+
+<h2>References</h2>
+<p>
+Zerbino DR, Johnson N, Juettemann T, Wilder SP, Flicek P.
+<a href="https://academic.oup.com/bioinformatics/article-lookup/doi/10.1093/bioinformatics/btt737"
+target="_blank">
+WiggleTools: parallel processing of large collections of genome-wide datasets for visualization and
+statistical analysis</a>.
+<em>Bioinformatics</em>. 2014 Apr 1;30(7):1008-9.
+PMID: <a href="https://www.ncbi.nlm.nih.gov/pubmed/24363377" target="_blank">24363377</a>; PMC: <a
+href="https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3967112/" target="_blank">PMC3967112</a>
+</p>
+
+<p>
+Mark Diekhans,
+<a href="https://github.com/diekhans/intronProspector"
+target="_blank">
+IntronProspector GitHub Repository </a>.
+<em>Github</em> 2018
+</p>
+
+<p>
+{refHtml}
+</p>""".format(**locals()))
+    readFh.close()
+
+def writeParentStanzas(tfh, saneHubName, hubName, cellCount):
+    " write tdb entries for the composite parent tracks "
+    tfh.write("""track %s\n""" % (saneHubName))
+    tfh.write("""shortLabel %s\n""" % (hubName))
+    tfh.write("""longLabel %s - %d cells\n""" % (hubName, cellCount))
+    tfh.write("compositeTrack on\n")
+    tfh.write("subGroup1 view Views reads=Reads cov=Coverage junc=Junctions\n")
+    tfh.write("type bed 3\n")
+    tfh.write("visibility dense\n")
+    tfh.write("\n")
+
+    tfh.write("""track %sViewReads\n""" % (saneHubName))
+    tfh.write("""shortLabel Reads\n""")
+    tfh.write("""longLabel %s Reads - %d cells\n""" % (hubName, cellCount))
+    tfh.write("parent %s\n" % saneHubName)
+    tfh.write("type bam\n")
+    tfh.write("visibility hide\n")
+    tfh.write("view reads\n")
+    tfh.write("\n")
+
+    tfh.write("""track %sViewCov\n""" % (saneHubName))
+    tfh.write("""shortLabel Coverage\n""")
+    tfh.write("""longLabel %s Coverage - %d cells\n""" % (hubName, cellCount))
+    tfh.write("parent %s\n" % saneHubName)
+    tfh.write("type bigWig\n")
+    tfh.write("visibility dense\n")
+    tfh.write("view cov\n")
+    tfh.write("\n")
+
+    tfh.write("""track %sViewJunc\n""" % (saneHubName))
+    tfh.write("""shortLabel Splicing\n""")
+    tfh.write("""longLabel %s Splice Junctions - %d cells\n""" % (hubName, cellCount))
+    tfh.write("parent %s\n" % saneHubName)
+    tfh.write("spectrum on\n")
+    tfh.write("type bigBed 12\n")
+    tfh.write("visibility dense\n")
+    tfh.write("view junc\n")
+    tfh.write("\n")
+
+    #tfh.write("""track %sCov\n""" % (saneHubName))
+    #tfh.write("""shortLabel %s Coverage\n""" % (hubName))
+    #tfh.write("""longLabel %s Read Coverage - %d cells\n""" % (hubName, cellCount))
+    #tfh.write("compositeTrack on\n")
+    #tfh.write("type bigWig\n")
+    #tfh.write("visibility dense\n")
+    #tfh.write("\n")
+
+    #tfh.write("""track %sJunc\n""" % (saneHubName))
+    #tfh.write("""shortLabel %s Introns\n""" % (hubName))
+    #tfh.write("""longLabel %s Intron Support - %d cells\n""" % (hubName, cellCount))
+    #tfh.write("compositeTrack on\n")
+    #tfh.write("type bigBed 12 +\n")
+    #tfh.write("visibility dense\n")
+    #tfh.write("\n")
+
+def findProgram(name):
+    " search PATH for binary and return full path "
+    progPath = distutils.spawn.find_executable(name)
+    if progPath==None:
+        errAbort("Cannot find program '%s' in PATH." % name)
+    return progPath
+
+def writeJobScript(jobFn, cmds):
+    " write commands to a shell script with file name "
+    jobFh = open(jobFn, "w")
+    logFname = splitext(jobFn)[0]+'.log'
+
+    jobFh.write("#!/bin/bash\n")
+    jobFh.write("set -e # = abort on error\n")
+    jobFh.write("set -o pipefail # = even in pipes\n")
+    jobFh.write("echo Job %s start, stdout/stderr go to %s\n" % (jobFn, logFname))
+    jobFh.write("exec 1> %s\n" % logFname)
+    jobFh.write("exec 2>&1\n");
+    jobFh.write("echo PID=$$\n");
+    for cmd in cmds:
+        jobFh.write(cmd+"\n")
+    jobFh.close()
+
+    logging.info("Wrote job script %s" % jobFn)
+
+def writeTdbStanzas(tfh, clusterName, saneHubName, cellCount):
+    " write the track db statements for a one cluster "
+    #saneClusterName = filter(str.isalnum, clusterName) # remove non alpha chars
+    saneClusterName = sanitizeName(clusterName)
+
+    tfh.write("""track %sReads\n""" % saneClusterName)
+    tfh.write("""shortLabel %s BAM\n""" % clusterName)
+    tfh.write("""longLabel %s sequencing reads from BAM (%d cells)\n""" % (clusterName, cellCount))
+    tfh.write("type bam\n")
+    tfh.write("view reads\n")
+    tfh.write("parent %sViewReads\n" % saneHubName)
+    tfh.write("subGroups view=reads\n")
+    tfh.write("bigDataUrl %s\n" % (saneClusterName+".bam"))
+    tfh.write("visibility dense\n")
+    tfh.write("\n")
+
+    tfh.write("""track %sCov\n""" % saneClusterName)
+    tfh.write("""shortLabel %s Cov\n""" % (clusterName))
+    tfh.write("""longLabel %s Coverage (%d cells)\n""" % (clusterName, cellCount))
+    tfh.write("type bigWig\n")
+    tfh.write("view cov\n")
+    tfh.write("parent %sViewCov\n" % saneHubName)
+    tfh.write("subGroups view=cov\n")
+    tfh.write("autoScale on\n")
+    tfh.write("bigDataUrl %s\n" % (saneClusterName+".bw"))
+    tfh.write("visibility dense\n")
+    tfh.write("\n")
+
+    tfh.write("""track %sJunc\n""" % saneClusterName)
+    tfh.write("""shortLabel %s Junc\n""" % (clusterName))
+    tfh.write("""longLabel %s Splice Junctions (%d cells)\n""" % (clusterName, cellCount))
+    tfh.write("type bigBed 12 +\n")
+    tfh.write("spectrum on\n")
+    tfh.write("scoreLabel Number of supporting reads (max: 1000)\n")
+    tfh.write("parent %sViewJunc\n" % saneHubName)
+    tfh.write("subGroups view=junc\n")
+    tfh.write("bigDataUrl %s\n" % (saneClusterName+".junctions.bb"))
+    tfh.write("visibility dense\n")
+    tfh.write("\n")
+
+def cellIdsForBam(bamPath):
+    # we try different ways to map the bam file name to a cellID:
+    # 1) remove the file ext, e.g. 123.3.bam -> cellId 123.3
+    # 2) remove everything after the first dot, 123.3.bam -> cellId 123
+    # 3 and 4) like 1) and 2) but with dashes replaced with dots (->R)
+    basePath = basename(bamPath)
+    cellId = splitext(basePath)[0]
+    yield cellId.replace("_R1", "").replace("_R2", "")
+
+    cellId2 = basePath.split(".")[0]
+    yield cellId2.replace("_R1", "").replace("_R2", "")
+
+    cellId3 = cellId.replace("-", ".")
+    yield cellId3.replace("_R1", "").replace("_R2", "")
+
+    cellId4 = cellId2.replace("-", ".")
+    yield cellId4.replace("_R1", "").replace("_R2", "")
+
+def findBams(bamDir, clusterToCells):
+    """
+    create dict with cluster -> (cellIds, bamFnames)
+    """
+    metaCellIds = set()
+    for cluster, cellIds in clusterToCells.iteritems():
+        for cellId in cellIds:
+            metaCellIds.add(cellId)
+
+    bamMask =join(bamDir, "*.bam")
+    logging.info("Getting list of BAM files matching %s" % bamMask)
+    bamPaths = glob.glob(bamMask)
+    bamPaths.sort()
+    logging.info("Found %d BAM files for %d meta cell IDs" % (len(bamPaths), len(metaCellIds)))
+
+    # make map cellId -> bam files
+    cellIdToBamFnames = defaultdict(list)
+    fileCount = 0
+    for bamPath in bamPaths:
+        logging.debug("BAM file name: %s" % bamPath)
+
+        cellId = None
+        for tryCellId in cellIdsForBam(bamPath):
+            logging.debug("Trying cell ID %s" % tryCellId)
 
-    if len(args)<=1:
-        cbToolCli_parseArgs(showHelp=True)
-        sys.exit(1)
+            if tryCellId in metaCellIds:
+                cellId = tryCellId
+                break
 
-    cmd = args[0]
+            logging.debug("%s is not in meta data" % tryCellId)
 
-    cmds = ["mtx2tsv", "matCatCells", "matCatGenes" "metaCat", "reorder", "cxg"]
+        if cellId==None:
+            logging.debug("Could not resolve %s to any cellId in meta" % (bamPath))
+        else:
+            logging.debug("Found file %s -> cellId=%s" % (bamPath, cellId))
+            fileCount += 1
+            cellIdToBamFnames[cellId].append(bamPath)
 
-    if cmd=="mtx2tsv":
-        mtxFname = args[1]
-        geneFname = args[2]
-        barcodeFname = args[3]
-        outFname = args[4]
-        mtxToTsvGz(mtxFname, geneFname, barcodeFname, outFname)
-    elif cmd=="matCatCells":
-        inFnames = args[1:-1]
-        outFname = args[-1]
-        matCat(inFnames, outFname)
-    elif cmd=="matCatGenes":
-        inFnames = args[1:-1]
-        outFname = args[-1]
-        matCatGenes(inFnames, outFname)
-    elif cmd=="cxg":
-        subCmd = args[1]
-        if subCmd=="allDatasets":
-            printRows(getCxgAllDatasets())
-        elif subCmd=="asset":
-            dsIds = args[2:]
-            getCxgAssets(dsIds)
-        elif subCmd=="allAssets":
-            getCxgAllAssets()
-        elif subCmd=="cp":
-            dsId = args[2]
-            assetId = args[3]
-            outFname = args[4]
-            url = getCxgAssetUrl(dsId, assetId)
-            cmd = ["curl", url, "--output", outFname]
-            subprocess.run(cmd)
-        elif subCmd=="desc":
-            collId = args[2]
-            getCxgColl(collId)
-
-    elif cmd=="metaCat" or cmd=="reorder":
-        inFnames = args[1:-1]
-        outFname = args[-1]
-
-        if len(inFnames)==0:
-            errAbort("You must provide at least two filenames: one input filename and one output filename")
-
-        if len(inFnames)==1 and isfile(outFname):
-            errAbort("You provided only one input file and the output file already exists. To avoid "
-            "accidentally overwriting a file, please either remove the output file or provide at least "
-            "three filenames: two input files and one output file. The second input file can be 'none', "
-            "which will suppress this error message.")
+    clusterBams = dict()
 
-        if len(inFnames)==2 and inFnames[1]=="none":
-            inFnames.pop()
+    #logging.info("Got %s BAM files and %s cell ids in the meta data" % (len(metaCellIds), len(cellIdToBamFnames)))
 
-        metaCat(inFnames, outFname, options)
-    else:
-        errAbort("Command %s is not a valid command. Valid commands are: %s" % (cmd, ", ".join(cmds)))
+    emptyClusterCount = 0
+    for clusterName, cellIds in clusterToCells.iteritems():
 
-def getLabels(l):
-    " given a list of dicts, return a |-sep list of 'label' values "
-    labels = []
-    for d in l:
-        if type(d)==str:
-            labels.append(d)
-        else:
-            labels.append(d["label"])
-    return "|".join(labels)
+        bamFnames = []
+        for cellId in cellIds:
+            cellBams = cellIdToBamFnames[cellId]
+            bamFnames.extend(cellBams)
 
-def printRows(iterator, headDone=False):
-    " print all rows gotten from an iterator "
-    #headDone = False
-    for row in iterator:
-        if headDone is False:
-            print("\t".join(row.keys()))
-            headDone = True
-        print("\t".join(row.values()))
-
-def getCxgAssetUrl(datasetId, assetId):
-    " cxg has signed links, get one for an asset ID "
-    url = 'https://api.cellxgene.cziscience.com/dp/v1/datasets/%s/asset/%s' % (datasetId, assetId)
-    import requests
-    ret = requests.post(url=url).json()
-    # keys: dataset_id, file_name, presigned_url
-    return ret["presigned_url"]
-
-def getCxgAllDatasets():
-    " yield all cxg datasets as ordered dicts "
-    import requests
-    url = "https://api.cellxgene.cziscience.com/dp/v1/datasets/index"
-    datasets = requests.get(url=url).json()
-    attrs = ['id', 'name', 'organism', 'collection_id', 'assay', 'explorer_url', 'is_primary_data', \
-            'cell_count', 'mean_genes_per_cell',
-            'development_stage', 'development_stage_ancestors', \
-            'disease', \
-            'published_at', 'revised_at', 'schema_version', 'self_reported_ethnicity', 'sex', 'tissue', \
-            'tissue_ancestors', 'cell_type', 'cell_type_ancestors']
-    for dataset in datasets:
-        row = OrderedDict()
-        for attr in attrs:
-            val = dataset.get(attr, "UNDEFINED")
-            if type(val)==type([]):
-                strVal = getLabels(val)
-            else:
-                strVal = str(val)
-            row[attr] = strVal
-        yield row
-
-def getCxgAllAssets():
-    ""
-    headDone = False
-    for ds in getCxgAllDatasets():
-        printRows(getCxgAssets([ds["id"]]), headDone)
-        headDone = True
-
-def getCxgAssets(dsIds, headDone=False):
-    " download assets for a list of cxg datasets "
-    import requests
-    attrs = ['dataset_id', 'dataset', 'filename', 'filetype', 'id', 's3_uri', 'created_at', 'updated_at', 'user_submitted']
-    #if not headDone:
-        #print("\t".join(attrs))
-
-    for dsId in dsIds:
-        url = "https://api.cellxgene.cziscience.com/dp/v1/datasets/%s/assets" % dsId
-        ret = requests.get(url=url).json()
-        for asset in ret["assets"]:
-            #row = []
-            row = OrderedDict()
-            for attr in attrs:
-                val = asset[attr]
-                if attr == "dataset":
-                    val = val["name"]
-                #row.append(str(val))
-                row[attr] = str(val)
-            #print("\t".join(row))
-            yield row
-
-def getCxgColl(collId):
-    " "
-
-def matCat(inFnames, outFname):
-    tmpFname = outFname+".tmp"
-    ofh = openFile(tmpFname, "w")
-
-    ifhs = []
-
-    sep = "\t"
-    if ".csv" in inFnames[0]:
-        sep = ","
-
-    for fn in inFnames:
-        ifhs.append( openFile(fn) )
-
-    headers, colCounts = getAllFields(ifhs, sep)
-    ofh.write("\t".join(headers))
-    ofh.write("\n")
-
-    for i, ifh in enumerate(ifhs):
-        logging.info("File %s: %d columns with values" % (ifhs[i].name, colCounts[i]-1)) 
-
-    fileCount = len(inFnames)
-    progressStep = 1000
-
-    doProcess = True
-    lineCount = 0
-
-    while doProcess:
-        geneId = None
-
-        lineCount += 1
-        if lineCount % progressStep == 0:
-            logging.info("Processed %d rows" % (lineCount))
-
-        for i, ifh in enumerate(ifhs):
-            lineStr = ifh.readline()
-            # check if we're at EOF
-            if lineStr=='':
-                doProcess = False
-                break
+        if len(bamFnames)==0:
+            logging.warn("No single BAM file found for cluster %s!" % clusterName)
+            emptyClusterCount += 1
+            continue
+        elif len(bamFnames)==1:
+            logging.warn("Only 1 BAM file for cluster %s?" % clusterName)
 
-            fields = lineStr.rstrip('\r\n').split(sep)
-            fields = [x.strip('"') for x in fields]
-            if (len(fields)!=colCounts[i]): # check number of columns against header count
-                raise Exception("Illegal number of fields: file %s, line %d, field count: %d, expected %d" % 
-                    (ifh.name, lineCount, len(fields), colCounts[i]))
-
-            # check the gene ID
-            if i==0: # get the gene ID from the first file
-                geneId = fields[0]
-                allVals = [geneId]
-            else:
-                #assert(geneId == fields[0]) # if this fails, then the rows are not in the same order
-                if geneId != fields[0]:
-                    print("Error: File %s has gene IDs that is out of order." % ifh.name)
-                    print("Expected geneID: %s, got geneID: %s" % (geneId, fields[0]))
-                    sys.exit(1)
+        logging.info("Cluster: %s, %d cell IDs in meta, found %d BAM files, example %s" % (clusterName, len(cellIds), len(bamFnames), bamFnames[0]))
 
-            allVals.extend(fields[1:])
+        clusterBams[clusterName] = (cellIds, bamFnames)
 
-        ofh.write("\t".join(allVals))
-        ofh.write("\n")
+    # now do some sanity checks
+    missMeta = set(cellIdToBamFnames) - metaCellIds
+    missBam = set(metaCellIds) - set(cellIdToBamFnames)
+    allCellIds = set(cellIdToBamFnames).intersection(metaCellIds)
+    logging.info("%d BAM cell ids have no meta data. Examples: %s" % (len(missMeta), " ".join(list(missMeta)[:10])))
+    logging.info("%d meta cell ids have no BAM file. Examples: %s" % (len(missBam), " ".join(list(missBam)[:10])))
 
-    # make sure that we've read through all files
-    for ifh in ifhs:
-        assert(ifh.readline()=='') # a file has still lines left to read?
+    return clusterBams, metaCellIds, cellIdToBamFnames
 
-    ofh.close()
-    moveOrGzip(tmpFname, outFname)
-    logging.info("Wrote %d lines (not counting header)" % lineCount)
+def writeDebugReport(allMetaCellIds, cellIdToBams, clusterBams, idReportFname):
+    """ write a three-column table for debugging BAM file name <-> meta differences.
+    Return number of cells with both at least one BAM file and meta data as a number.
+    """
+    logging.info("Writing %s to help track down BAM file problems" % idReportFname)
+    cellCount = 0
+    ofh = open(idReportFname, "w")
+    ofh.write("#cellId\thasMeta\tcluster\tbamFname1\tbamFname2OrMore\n")
 
-def matCatGenes(inFnames, outFname):
-    " cat the lines several tab-sep or csv files, check headers and skip the header lines "
-    tmpFname = outFname+".tmp"
-    ofh = openFile(tmpFname, "w")
-
-    otherHeaders = None
-    lineCount = 0
-    for fn in inFnames:
-        prefix = ""
-        if "=" in fn:
-            fn, prefix = fn.split("=")
-
-        sep = "\t"
-        if ".csv" in fn:
-            sep = ","
-
-        headers = None
-        logging.info("Reading %s" % fn)
-
-        doReorder = False
-        fieldOrder = None
-
-        for line in openFile(fn):
-            row = line.rstrip("\n\r").split(sep)
-            row = [x.strip('"') for x in row]
-
-            if otherHeaders is None:
-                otherHeaders = row
-                ofh.write("\t".join(otherHeaders))
-                ofh.write("\n")
-            if headers is None:
-                headers = row
-                if (headers != otherHeaders): # all files must have identical columns = identical header line
-                    logging.warn("Headers are not identical, need to re-order columns, this will be pretty slow")
-                    doReorder = True
-
-                    fieldOrder = [0]
-                    for h in otherHeaders[1:]:
-                        idx = headers.index(h)
-                        assert(idx!=0) # internal logic error. Should never happen.
-                        fieldOrder.append( idx ) # if this fails, then one file has a column that the other one doesn't have. Not clear what should happen then -> just fail.
-                continue
+    allMetaCellIds = set(allMetaCellIds)
 
-            if prefix!="":
-                row[0] = prefix+row[0]
+    allCellIds = set(allMetaCellIds).union(cellIdToBams)
 
-            if doReorder:
-                ofh.write("\t".join([row[i] for i in fieldOrder]))
-            else:
-                ofh.write("\t".join(row))
+    cellToCluster = {}
+    for clusterName, (cellIds, bamFnames) in clusterBams.iteritems():
+        for cellId in cellIds:
+            cellToCluster[cellId] = clusterName
 
-            ofh.write("\n")
-            lineCount += 1
+    for cellId in allCellIds:
+        ofh.write(cellId+"\t")
 
-        logging.info("Wrote %d lines to output file (not counting header)" % lineCount)
-
-    ofh.close()
-    logging.info("Compressing %s", outFname)
-    moveOrGzip(tmpFname, outFname)
-
-def reorderFields(row, firstFields, skipFields):
-    " reorder the row to have firstFields first "
-    #logging.debug("Reordering row to have %s fields first" % firstFields)
-    newRow = [row[0]]
-    for idx in firstFields:
-        newRow.append(row[idx])
-
-    for i in range(1, len(row)):
-        if i not in firstFields and i not in skipFields:
-            newRow.append(row[i])
-
-    return newRow
-
-def metaCat(inFnames, outFname, options):
-    " merge all tsv/csv columns in inFnames into a new file, outFname. Column 1 is ID to join on. "
-    logging.debug("In fnames: %s, out fname: %s" % (repr(inFnames), repr(outFname)))
-    allHeaders = ["cellId"]
-    allRows = defaultdict(dict) # cellId -> fileIdx -> list of non-ID fields
-    fieldCounts = {} # fileIdx -> number of non-ID fields
-    allIds = set() # set with all cellIds
-
-    firstFields = []
-    if options.order!="" and options.order is not None:
-        firstFields = options.order.split(",")
-
-    delFields = []
-    if options.delFields!="" and options.delFields is not None:
-        delFields = options.delFields.split(",")
-
-    for fileIdx, fname in enumerate(inFnames):
-        logging.info("Reading %s" % fname)
-        headers = None
-        rowCount = 0
-        for row in lineFileNextRow(fname, headerIsRow=True):
-            if headers is None:
-                headers = row[1:]
-                logging.info("Reading %s, %d columns:  %s" % (fname, len(headers), repr(headers)))
-                allHeaders.extend(headers)
-                fieldCounts[fileIdx] = len(headers)
-                continue
+        if cellId in allMetaCellIds:
+            ofh.write("Yes\t")
+        else:
+            ofh.write("No\t")
 
-            rowCount +=1
-            cellId = row[0]
-            allIds.add(cellId)
-            allRows[cellId][fileIdx] = row[1:]
-        logging.info("Read %d rows" % rowCount)
-
-    nonCharRe = re.compile(r'[^a-zA-Z0-9]')
-
-    if options.fixDots:
-        # first create a map realId -> rId
-        rToReal = {}
-        for cellId, rowData in iterItems(allRows):
-            rId = nonCharRe.sub(".", cellId)
-            if rId!=cellId and rId in allRows:
-                assert(rId not in rToReal) # Uh-oh! Mapping R <-> realId is not simple. May need some manual work.
-                rToReal[rId]=cellId
-        logging.info("Found %d cell IDs that look like they've been mangled by R" % (len(rToReal)))
-
-        # now merge the R-id entries into the real ID entries
-        newRows = {}
-        for rId, readlId in iterItems(rToReal):
-            allRows[cellId].update(allRows[rId])
-        for rId in rToReal.keys():
-            del allRows[rId]
-        logging.info("Merged back rIds into normal data")
-
-    # find the field indices of the fields we're putting first
-    firstFieldIdx = []
-    for h in firstFields:
-        try:
-            idx = allHeaders.index(h)
-            firstFieldIdx.append(idx)
-        except ValueError:
-            logging.warning("Field %s specified on command line --order is not in the meta data file" % repr(h))
-
-    # and those of fields we will skip
-    delFieldIdx = []
-    for h in delFields:
-        try:
-            idx = allHeaders.index(h)
-        except ValueError:
-            errAbort("Field %s specified on command line with --del is not in the meta data file" % repr(h))
-        delFieldIdx.append(idx)
-
-    if len(firstFields)!=0:
-        logging.info("Order of fields that come first: %s" % firstFields)
-    if len(delFields)!=0:
-        logging.info("Removing these fields: %s" % delFields)
+        clusterName = cellToCluster.get(cellId, "!noClusterFound")
+        ofh.write("%s\t" % clusterName)
 
+        bamFnames = cellIdToBams[cellId]
+        if len(bamFnames)==0:
+            ofh.write("!noBamFound\t!noBamFound\n")
+            continue
 
-    if outFname=="stdout" or outFname=="/dev/stdout":
-        ofh = sys.stdout
-    else:
-        tmpFname = outFname+".tmp"
-        ofh = openFile(tmpFname, "w")
+        if cellId in allMetaCellIds:
+            cellCount += 1
 
-    allHeaders = reorderFields(allHeaders, firstFieldIdx, delFieldIdx)
-    ofh.write("\t".join(allHeaders))
-    ofh.write("\n")
-
-    for cellId, rowData in iterItems(allRows):
-        row = [cellId]
-        for fileIdx in range(0, len(inFnames)):
-            if fileIdx in rowData:
-                row.extend(rowData[fileIdx])
-            else:
-                row.extend([""]*fieldCounts[fileIdx])
+        ofh.write(bamFnames[0])
+        ofh.write("\t")
 
-        row = reorderFields(row, firstFieldIdx, delFieldIdx)
-        ofh.write("\t".join(row))
+        if len(bamFnames)>1:
+            ofh.write(",".join(bamFnames[1:]))
         ofh.write("\n")
 
     ofh.close()
-    if ofh!=sys.stdout:
-        renameFile(tmpFname, outFname)
-    logging.info("Output field order is: %s" % allHeaders)
-    logging.info("Wrote %d lines (not counting header)" % len(allRows))
-
-def importCellrangerMatrix(inDir, outDir):
-    " convert the cellranger 2 or 3 matrix, use the .mtx or .h5 file, whatever is available "
-    outExprFname = join(outDir, "exprMatrix.tsv.gz")
-    # cellranger 2: filtered_feature_bc_matrix/<db>/matrix.mtx and not gzipped
-    mask1 = join(inDir, "filtered_gene_bc_matrices/*/matrix.mtx")
-    # cellranger 3: filtered_gene_bc_matrices and gzipped
-    mask2 = join(inDir, "filtered_feature_bc_matrix/matrix.mtx.gz")
-    # h5 file as fallback, requires scanpy
-    # cellranger3: filtered_feature_bc_matrix.h5
-    mask3 = join(inDir, "*filtered_*matri*.h5") # should work for cr 1, 2 and 3
-    matFnames1 = glob.glob(mask1)
-    matFnames2 = glob.glob(mask2)
-    matFnames3 = glob.glob(mask3)
-    logging.info("Looking for %s (cellranger 1/2) or %s (cellranger3) or %s" % (mask1, mask2, mask3))
-
-    # ugly code warning
-    if len(matFnames1)!=0:
-        # cellranger 1/2 mtx files are not gziped
-        assert(len(matFnames1)==1)
-        matFname = matFnames1[0]
-        logging.info("Found %s" % matFname)
-        barcodeFname = matFname.replace("matrix.mtx", "barcodes.tsv")
-        geneFname = matFname.replace("matrix.mtx", "genes.tsv")
-        mtxToTsvGz(matFname, geneFname, barcodeFname, outExprFname)
-    elif len(matFnames2)!=0:
-        # cellranger 3 mtx files are gzipped
-        assert(len(matFnames2)==1)
-        matFname = matFnames2[0]
-        logging.info("Found %s" % matFname)
-        barcodeFname = matFname.replace("matrix.mtx.gz", "barcodes.tsv.gz")
-        geneFname = matFname.replace("matrix.mtx.gz", "features.tsv.gz")
-        mtxToTsvGz(matFname, geneFname, barcodeFname, outExprFname)
-    elif len(matFnames3)!=0:
-        # h5 files of cellranger 1/2/3 are read via scanpy
-        matFnames3 = glob.glob(mask3)
-        logging.info("Found %s" % matFnames3)
-        assert(len(matFnames3)==1)
-        matFname = matFnames3[0]
-
-        import scanpy.api as sc
-        logging.info("Reading matrix %s" % matFname)
-        adata = readMatrixAnndata(matFname)
-        anndataMatrixToTsv(adata, outExprFname)
-    else:
-        errAbort("Could not find matrix, neither as %s, %s nor %s" % (mask1, mask2, mask3))
-        logging.info("Looking for %s" % mask3)
+    return cellCount
 
-    return matFname
 
-def crangerToCellbrowser(datasetName, inDir, outDir, noMat):
-    " convert cellranger output to a cellbrowser directory "
-    makeDir(outDir)
-    # copy over the clusters
-    clustFname = join(inDir, "analysis/clustering/graphclust/clusters.csv")
-    if not isfile(clustFname):
-        logging.warn("Cannot find %s" % clustFname)
-        clustFname = join(inDir, "analysis/kmeans/10_clusters/clusters.csv")
-        logging.warn("Using%s instead" % clustFname)
-    metaFname = join(outDir, "meta.csv")
-    shutil.copy(clustFname, metaFname)
-
-    # copy over the t-SNE coords
-    tsneFname = join(inDir, "analysis/tsne/2_components/projection.csv")
-    if not isfile(tsneFname):
-        tsneFname = join(inDir, "analysis/tsne/projection.csv")
-    coordFname = join(outDir, "tsne.coords.csv")
-    shutil.copy(tsneFname, coordFname)
-
-    # copy over the markers
-    dgeFname = join(inDir, "analysis/diffexp/graphclust/differential_expression.csv")
-    if not isfile(dgeFname):
-        logging.warn("Not found: %s" % dgeFname)
-        dgeFname = join(inDir, "analysis/kmeans/10_clusters/differential_expression.csv")
-        logging.warn("Using instead: %s" % dgeFname)
-
-    markerFname = join(outDir, "markers.tsv")
-    geneFname = join(outDir, "gene2sym.tsv")
-    crangerSignMarkers(dgeFname, markerFname, geneFname, 0.01, 100)
+def mergeBams(hubName, db, tfh, bamDir, clusterToCells, outDir):
+    logging.info("*** Merging and analyzing BAM files")
 
-    if not noMat:
-        matFname = importCellrangerMatrix(inDir, outDir)
-    else:
-        matFname = "unknown"
+    clusterBams, allMetaCellIds, cellIdToBams = findBams(bamDir, clusterToCells)
 
-    confName = join(outDir, "cellbrowser.conf")
-    coordDescs = [{"file":"tsne.coords.csv", "shortLabel":"CellRanger t-SNE"}]
-    confArgs =  {"meta" : "meta.csv", "clusterField" : "Cluster", "tags" : ["10x"]}
-    writeCellbrowserConf(datasetName, coordDescs, confName, confArgs)
-
-    crangerWriteMethods(inDir, outDir, matFname)
-    generateHtmls(datasetName, outDir)
-
-def crangerWriteMethods(inDir, outDir, matFname):
-    htmlFname = join(outDir, "methods.html")
-    if isfile(htmlFname):
-        logging.info("%s exists, not overwriting" % htmlFname)
-        return
-
-    import csv
-    csvMask = join(inDir, "*_metrics_summary.csv")
-    csvFnames = glob.glob(csvMask)
-
-    jsonFname = join(inDir, "summary.json")
-    if len(csvFnames)==0:
-        if isfile(jsonFname):
-            qcVals = json.load(open(jsonFname))
-        else:
-            logging.warn("Cannot find %s nor %s, not writing %s" % (csvMask, jsonFname, htmlFname))
-            return
-    else:
-        qcVals = list(csv.DictReader(open(csvFnames[0])))[0]
-
-    ofh = open(htmlFname, "w")
-    ofh.write("<p>This dataset was imported from a CellRanger analysis directory with cbCellranger.</p>\n")
-    ofh.write("<p><b>QC metrics reported by CellRanger:</b></p>\n")
-
-    for key, value in iterItems(qcVals):
-        ofh.write("<i>%s:</i> %s<br>\n" % (key, str(value)))
-    ofh.close()
-    logging.info("Wrote %s" % ofh.name)
+    idReportFname = join(outDir, "metaBamMatch.txt")
+    cellCount = writeDebugReport(allMetaCellIds, cellIdToBams, clusterBams, idReportFname)
 
-def crangerSignMarkers(dgeFname, markerFname, geneFname, maxPval, maxGenes):
-    " convert cellranger diff exp file to markers.tsv file "
-    # Old Cellranger 1 format:
-    # Gene ID,Gene Name,Cluster 1 Weight,Cluster 1 UMI counts/cell,Cluster 2 Weight,Cluster 2 UMI counts/cell,Cluster 3 Weight,Cluster 3 UMI counts/cell,Cluster 4 Weight,Cluster 4 UMI counts/cell,Cluster 5 Weight,Cluster 5 UMI counts/cell,Cluster 6 Weight,Cluster 6 UMI counts/cell,Cluster 7 Weight,Cluster 7 UMI counts/cell,Cluster 8 Weight,Cluster 8 UMI counts/cell,Cluster 9 Weight,Cluster 9 UMI counts/cell,Cluster 10 Weight,Cluster 10 UMI counts/cell
-
-    ofh = open(markerFname, "w")
-    ofh.write("cluster\tgene\tAdj. P-Value\tLog2 fold change\tMean UMI Counts\n")
-
-    clusterToGenes = defaultdict(list)
-
-    # read the significant markers and their p-Values
-    logging.info("Reading %s" % dgeFname)
-    ifh = open(dgeFname)
-
-    # determine file format
-    line1 = ifh.readline()
-    # cellranger 3
-    fileVersion = None
-    if line1.startswith("Feature ID"):
-        fieldsProCluster = 3
-        fileVersion = 3
-    # cellranger 1 or 2
-    elif line1.startswith("Gene ID"):
-        if "Cluster 1 Weight" in line1:
-            fieldsProCluster = 2
-            fileVersion = 1
-        else:
-            fieldsProCluster = 3
-            fileVersion = 2
-    assert(fileVersion is not None) # unknown cellranger version?
-
-    for line in ifh:
-        row = line.rstrip("\n\r").split(",")
-        geneId = row[0]
-        sym = row[1]
-        clusterCount = int((len(row)-2) / fieldsProCluster)
-        for clusterIdx in range(0, clusterCount):
-            startField = (clusterIdx*fieldsProCluster)+2
-            if fileVersion>=2:
-                mean = float(row[startField])
-                fc = float(row[startField+1])
-                pVal = float(row[startField+2])
-            else:
-                fc = float(row[startField])
-                mean = float(row[startField+1])
-                pVal = 0.0001
-
-            if pVal < maxPval:
-                clusterToGenes[clusterIdx+1].append((fc, mean, pVal, sym))
-
-    # write out the markers
-    for clusterId, clusterGenes in iterItems(clusterToGenes):
-        clusterGenes.sort(key=operator.itemgetter(2)) # sort by fold change
-        maxIdx = min(maxGenes, len(clusterGenes))
-        for i in range(0, maxIdx):
-            fc, mean, pVal, sym = clusterGenes[i]
-            ofh.write("%d\t%s\t%g\t%f\t%f\n" % (clusterId, sym, pVal, fc, mean))
+    jlFh = open("jobList", "w")
 
-    ofh.close()
-    logging.info("Wrote %s" % ofh.name)
+    #cellCount = 0
+    for clusterName, (cellIds, bamFnames) in clusterBams.iteritems():
+        uniqueCellIds = set(cellIds)
+        #cellCount += len(uniqueCellIds)
 
-def cbCellrangerCli():
-    args, options = cbCellrangerCli_parseArgs()
+    logging.info("Merging BAM files and writing hub")
+    saneHubName = sanitizeName(hubName)
+    writeParentStanzas(tfh, saneHubName, hubName, cellCount)
 
-    if options.outDir is None or options.inDir is None or options.datasetName is None:
-        logging.error("You have to specify at least an input and an output directory and a dataset name.")
-        cbCellrangerCli_parseArgs(showHelp=True)
+    chromSizes = cellbrowser.getSizesFname(db)
 
-    crangerToCellbrowser(options.datasetName, options.inDir, options.outDir, options.noMat)
+    jobNo = 0
+    emptyClusterCount = 0
+    for clusterName, (cellIds, bamFnames) in clusterBams.iteritems():
+        saneClusterName = sanitizeName(clusterName)
+        logging.info("Processing cluster %s, %d cellIds/BAM files, examples: %s" % (clusterName, len(cellIds), cellIds[0]))
+        cmds = []
 
-def cbCellrangerCli_parseArgs(showHelp=False):
-    " setup logging, parse command line arguments and options. -h shows auto-generated help page "
-    parser = optparse.OptionParser("""usage: %prog [options] -i cellRangerDir -o outputDir - convert the cellranger output to cellbrowser format and create a cellranger.conf file
+        outBam = join(outDir, saneClusterName+".bam")
+        outStat = join(outDir, saneClusterName+".stats.txt")
+        outCalls = join(outDir, saneClusterName+".calls.tsv")
+        junctionBed = join(outDir, saneClusterName+".junctions.bed")
+        intronBed = join(outDir, saneClusterName+".introns.bed")
 
-    """)
+        junctionBedSorted = junctionBed.replace(".bed", ".sorted.bed")
+        intronBedSorted = intronBed.replace(".bed", ".sorted.bed")
 
-    parser.add_option("-d", "--debug", dest="debug", action="store_true",
-        help="show debug messages")
+        junctionBb = junctionBed.replace(".bed", ".bb")
+        intronBb = intronBed.replace(".bed", ".bb")
 
-    parser.add_option("-i", "--inDir", dest="inDir", action="store", help="input folder with the cellranger analysis output. This is the directory with the two directories 'analysis' and 'filtered_gene_bc_matrices'")
-    parser.add_option("-o", "--outDir", dest="outDir", action="store", help="output directory")
-    #parser.add_option("-g", "--geneSet", dest="geneSet", action="store", help="geneset, e.g. gencode28 or gencode-m13 or similar. Default: %default", default="gencode24")
-    parser.add_option("-n", "--name", dest="datasetName", action="store", help="name of the dataset. No spaces or special characters.")
-    parser.add_option("-m", "--noMat", dest="noMat", action="store_true", help="do not export the matrix again, saves some time if you changed something small since the last run")
+        cmd = "echo merging %d bam files for %d cell IDs" % (len(bamFnames), len(set(cellIds)))
+        cmds.append(cmd)
 
-    (options, args) = parser.parse_args()
+        intronProspector = findProgram("intronProspector")
+        samtools = findProgram("samtools")
+        if len(bamFnames)==1:
+            # samtools merge aborts if only one input BAM file
+            cmd = "cat %s " % (bamFnames[0])
+        else:
+            # -r construct read groups
+            # -f overwrite output files if needed
+            cmd = samtools+" merge -f -r - %s " % (" ".join(bamFnames))
+
+        cmd += "| tee %s | %s -p /dev/stdout -U -c %s -j %s -n %s " % \
+            (outBam, intronProspector, outCalls, junctionBed, intronBed)
+        cmd += "| samtools flagstat - > %s" % outStat
+        cmds.append(cmd)
+        
+        #cmd = "echo running intronprospector on merged BAM file"
+        #cmds.append(cmd)
+
+        # XX could be part of the samtools merge command, in a pipe
+        #cmds.append(cmd)
+
+        cmd = "samtools index %s" % outBam
+        cmds.append(cmd)
+
+        cmd = """export LC_COLLATE=C; cat %s | awk '($5>1000) {$5=1000;} { OFS="\\t"; print}'  | sort -k1,1 -k2,2n > %s""" % (junctionBed, junctionBedSorted)
+        cmds.append(cmd)
+
+        cmd = """export LC_COLLATE=C; cat %s | awk '($5>1000) {$5=1000;} { OFS="\\t"; print}' | sort -k1,1 -k2,2n > %s""" % (intronBed, intronBedSorted)
+        cmds.append(cmd)
+
+        bigBed = findProgram("bedToBigBed")
+        cmd = bigBed+" %s %s %s -type=bed6 -tab" % (intronBedSorted, chromSizes, intronBb)
+        cmds.append(cmd)
+
+        cmd = bigBed+" %s %s %s -type=bed12 -tab" % (junctionBedSorted, chromSizes, junctionBb)
+        cmds.append(cmd)
+
+        # alternative, 4x slower, silently drops ERCC chroms(?)
+        # ~/bin/x86_64/bamToPsl in.bam stdout -chromAlias=mm10.chromAlias.tab -nohead | pslToBed stdin stdout | bedItemOverlapCount mm10 stdin -bed12 > hub/largeintestinegobletcell.bedgraph
+        cmd = "echo creating coverage for merged BAM file"
+        cmds.append(cmd)
+
+        wiggletools = findProgram("wiggletools")
+        outWig = join(outDir, saneClusterName+".wig")
+        outBw = join(outDir, saneClusterName+".bw")
+        # fix up the chrom field and the chrom=xxx stepSize fields
+        # For wiggle files with Ensembl chrom names, we need UCSC chrom names
+        cmd = wiggletools+ """ coverage %s | awk '($1 ~ /^[0-9XYM]/ && (NF==4)) { if ($1=="MT") {$1="M"}; $1="chr"$1 } ($2 ~ /^chrom=[0-9XYM]/) {split($2,a, "="); if (a[2]=="MT") {a[2]="M"}; $2="chrom=chr"a[2]} // {OFS=" "; print}' > %s""" % (outBam, outWig)
+        cmds.append(cmd)
+
+        wigToBigWig = findProgram("wigToBigWig")
+        # -clip also means to not check the sequence names against chrom.sizes anymore
+        # clip is needed so GL and KI seqs in hg38 don't mess up the conversion
+        cmd = wigToBigWig+ " %s %s %s -clip" % (outWig, chromSizes, outBw)
+        cmds.append(cmd)
+
+        cmd = "rm -f %s %s %s" % (outWig, intronBedSorted, junctionBedSorted)
+        cmds.append(cmd)
+
+        #if False:
+        if isfile(outBw):
+            logging.info("Not running anything for %s, file %s already exists" % (saneClusterName, outBw))
+        else:
+            jobFn = "job-%d.sh" % jobNo
+            writeJobScript(jobFn, cmds)
+            jlFh.write("/bin/bash %s {check out exists %s}\n" % (jobFn, outBw))
+        jobNo+=1
 
-    if showHelp:
-        parser.print_help()
-        exit(1)
+        writeTdbStanzas(tfh, clusterName, saneHubName, len(cellIds))
 
-    setDebug(options.debug)
+    if emptyClusterCount==len(clusterToCells):
+        logging.error("No single BAM file could be linked to the meta data. Please check the identifiers in the meta data table against the file names in %s." % (bamDir))
+        sys.exit(1)
 
-    return args, options
+    jlFh.close()
+    logging.info("Wrote jobList file %s" % jlFh.name)
 
-def cbImportScanpy_parseArgs(showHelp=False):
-    " setup logging, parse command line arguments and options. -h shows auto-generated help page "
-    parser = optparse.OptionParser("""usage: %prog [options] -i inFilename -o outDir - convert Scanpy AnnData object to cellbrowser. inFilename can be an .h5ad or .loom file. 
-    Exports raw.X by default, or .X alternatively, see --proc. Exports all meta data. Writes .tsv by default, or alternatively .mtx.gz
+    logging.info("Wrote %s" % tfh.name)
 
-    Example:
-    - %prog -i pbmc3k.h5ad -o pbmc3kScanpy - convert pbmc3k to directory with tab-separated files
-    """)
+def clamp(x):
+    return max(0, min(int(x), 255))
 
-    parser.add_option("-d", "--debug", dest="debug", action="store_true",
-        help="show debug messages")
+def toHex(rgb):
+    r = rgb[0]
+    g = rgb[1]
+    b = rgb[2]
+    return "#{0:02x}{1:02x}{2:02x}".format(clamp(r*255), clamp(g*255), clamp(b*255))
+
+def writeBarChartTdb(tfh, bbFname, clusterNames, unitName):
+    " write the barChart tdb stanza "
+    stepSize = 1.0 / len(clusterNames)
+    colorCodes = []
+    x = 0
+    while x < 1.0:
+        colorCodes.append(colorsys.hsv_to_rgb(x, 1.0, 1.0))
+        x+=stepSize
+
+    hexCodes = [toHex(x) for x in colorCodes]
+
+    tfh.write('track barChart\n')
+    tfh.write('type bigBarChart\n')
+    tfh.write('visibility full\n')
+    tfh.write('shortLabel Cluster expression\n')
+    tfh.write('longLabel Median Cluster expression\n')
+
+    # only remove spaces, this is more readable than sanitizeName
+    saneClusterNames = []
+    for cn in clusterNames:
+        cn = cn.replace(" ", "_")
+        #cn = ''.join(ch for ch in newName if (ch.isalnum() or ch=="_"))
+        saneClusterNames.append(cn)
+
+    tfh.write('barChartBars %s\n' % " ".join(saneClusterNames))
+    tfh.write('barChartColors %s\n' % " ".join(hexCodes))
+    tfh.write('barChartMetric median\n')
+    tfh.write('barChartUnit %s\n' % unitName)
+    tfh.write('barChartMatrixUrl exprMatrix.tsv\n')
+    tfh.write('barChartSampleUrl clusters.tsv\n')
+    tfh.write('defaultLabelFields name2\n')
+    tfh.write('labelFields name2,name\n')
+    tfh.write('bigDataUrl barChart.bb\n\n')
+
+def to_camel_case(snake_str):
+    components = snake_str.split('_')
+    # We capitalize the first letter of each component except the first one
+    # with the 'title' method and join them together.
+    return components[0] + ''.join(x.title() for x in components[1:])
+
+def sanitizeName(name):
+    " remove all nonalpha chars and camel case name "
+    newName = to_camel_case(name.replace(" ", "_"))
+    newName = ''.join(ch for ch in newName if (ch.isalnum() or ch=="_"))
+    return newName
+
+def writeCatFile(clusterToCells, catFname):
+    " write file with cellId<tab>clusterName "
+    logging.info("Writing %s" % catFname)
+    ofh = open(catFname, "w")
+    for clusterName, cellIds in clusterToCells.iteritems():
+        for cellId in cellIds:
+            ofh.write("%s\t%s\n" % (cellId, clusterName))
+    ofh.close()
 
-    parser.add_option("-i", "--inFile", dest="inFile", action="store",
-        help="input .h5ad file. Required parameter")
+def makeBarGraphBigBed(genome, inMatrixFname, outMatrixFname, geneType, clusterToCells, \
+        clusterOrder, clusterFname, bbFname):
+    """ create a barGraph bigBed file for an expression matrix
+    clusterToCells is a dict clusterName -> list of cellIDs
+    clusterOrder is a list of the clusterNames in the right order
+    """
+    logging.info("*** Creating barChartGraph bigbed file")
+    if geneType.startswith("symbol"):
+        # create a mapping from symbol -> gene locations
+        if "/" in geneType:
+            defGenes = geneType.split("/")[1]
+        elif genome=="hg38":
+            defGenes = "gencode24"
+        elif genome=="hg19":
+            defGenes = "gencode19"
+        elif genome=="mm10":
+            defGenes = "gencode-m13"
+        else:
+            errAbort("Unclear how to map symbols to genome for db %s. Please adapt cellbrowser.py" % genome)
 
-    parser.add_option("", "--proc", dest="useProc", action="store_true",
-        help="when exporting, do not use the raw input data, instead use the normalized and corrected matrix scanpy. This has no effect if the anndata.raw attribute is not used in the anndata object")
+        logging.info("Using %s to map symbols to genome" % defGenes)
 
-    parser.add_option("-o", "--outDir", dest="outDir", action="store",
-        help="Output directory. Required parameter")
+        geneToSym = cellbrowser.readGeneSymbols({'geneIdType':defGenes})
+        geneLocsId = cellbrowser.parseGeneLocs(defGenes)
+        geneLocs = {}
+        for geneId, locs in iterItems(geneLocsId):
+            sym = geneToSym[geneId]
+            geneLocs[sym] = locs
+    else:
+        geneToSym = cellbrowser.readGeneSymbols({'geneIdType':geneType})
+        geneLocs = cellbrowser.parseGeneLocs(geneType)
 
-    parser.add_option("-n", "--name", dest="datasetName", action="store",
-        help="Dataset name for generated cellbrowser.conf. If not specified, the last component of -o will be used")
+    matOfh = open(outMatrixFname, "w")
+    clustOfh = open(clusterFname, "w")
 
-    parser.add_option("", "--htmlDir", dest="htmlDir", action="store",
-        help="do not only convert to tab-sep files but also run cbBuild to"
-            "convert the data and add the dataset under htmlDir")
+    mr = cellbrowser.MatrixTsvReader()
+    mr.open(inMatrixFname)
+    matType, cellNames = mr.matType, mr.sampleNames
+
+    cellIds = range(0, len(cellNames))
+    cellNameToId = dict(zip(cellNames, cellIds))
+
+    # make a list of lists of cellIds, one per cluster, in the right order
+    clusterCellIds = [] # list of tuples with cell-indexes, one per cluster
+    allCellNames = [] # list for cellIds, with a matrix, meta and with bam file
+    allCellIndices = [] # position of all cellIds in allCellNames
+    for clusterName in clusterOrder:
+        cellIdxList = []
+        for cellName in clusterToCells[clusterName]:
+            if cellName not in cellNameToId:
+                logging.warn("%s is in meta but not in expression matrix." % cellName)
+                continue
+            idx = cellNameToId[cellName]
+            cellIdxList.append(idx)
+            allCellNames.append(cellName)
+            allCellIndices.append(idx)
+            sanClusterName = clusterName.replace(" ", "_")
+            clustOfh.write("%s\t%s\n" % (cellName, sanClusterName))
+
+        if len(cellIdxList)==0:
+            logging.warn("No cells assigned to cluster %s" % clusterName)
+
+        clusterCellIds.append(tuple(cellIdxList))
+    clustOfh.close()
+
+    # write header line
+    matOfh.write("#gene\t")
+    matOfh.write("\t".join(allCellNames))
+    matOfh.write("\n")
+
+    # make the barchart bed file. format:
+    # chr14 95086227 95158010 ENSG00000100697.10 999 - DICER1 5 10.94,11.60,8.00,6.69,4.89 93153 26789
+    #bedFname = join(outDir, "barchart.bed")
+    bedFname = bbFname.replace(".bb", ".bed")
+    assert(bedFname!=bbFname)
+
+    bedFh = open(bedFname, "w")
+
+    skipCount = 0
+    for geneId, sym, exprArr in mr.iterRows():
+        logging.debug("Writing BED and matrix line for %s" % geneId)
+
+        # write the new matrix row
+        offset = matOfh.tell()
+        rowHeader = "%s\t" % (geneId)
+        matOfh.write(rowHeader)
+
+        newRow = []
+        for idx in allCellIndices:
+            newRow.append(str(exprArr[idx]))
+        newLine = "\t".join(newRow)
+        matOfh.write(newLine)
+        matOfh.write("\n")
+        lineLen = len(geneId)+len(newLine)+2 # include tab and newline
+
+        medianList = []
+
+        for cellIds in clusterCellIds:
+            exprList = []
+            for cellId in cellIds:
+                exprList.append(exprArr[cellId])
+            n = len(cellIds)
+            if len(exprList)==0:
+                median = 0
+            else:
+                median = sorted(exprList)[n//2] # approx OK, no special case for even n's
+            medianList.append(str(median))
+            bedScore = len([x for x in exprList if x!=0]) # score = non-zero medians
+            bedScore = min(1000, bedScore)
+
+        if geneId not in geneLocs:
+            geneId2 = geneId.replace(".", "-", 1) # does this make sense? (for R)
+            if geneId2 not in geneLocs:
+                logging.warn("Cannot place gene '%s' onto genome, dropping it" % geneId)
+                skipCount += 1
+                continue
+            else:
+                geneId = geneId2
 
-    parser.add_option("-p", "--port", dest="port", action="store", type="int",
-            help="only with --htmlDir: start webserver on port to serve htmlDir")
+        bedRows = geneLocs[geneId]
 
-    parser.add_option("", "--markerField", dest="markerField", action="store",
-            help="name of the marker genes field, default: %default", default="rank_genes_groups")
+        # one geneId may have multiple placements, e.g. Ensembl's rule for duplicate genes
+        for bedRow in bedRows:
+            sym = geneToSym.get(geneId, geneId)
+            bedRow[4] = str(bedScore) # 4 = score field
+            bedRow.append(sym)
+            bedRow.append(str(len(medianList)))
+            bedRow.append(",".join(medianList))
+            bedRow.append(str(offset))
+            bedRow.append(str(lineLen))
 
-    parser.add_option("", "--clusterField", dest="clusterField", action="store",
-            help="if no marker genes are present, use this field to calculate them. Default is to try a list of common field names, like 'Cluster' or 'louvain' and a few others")
+            bedFh.write("\t".join(bedRow))
+            bedFh.write("\n")
 
-    parser.add_option("-f", "--matrixFormat", dest="matrixFormat", action="store", default="mtx",
-            help="Output matrix file format. 'mtx' or 'tsv'. default: mtx",)
+    bedFh.close()
 
-    parser.add_option("-m", "--skipMatrix", dest="skipMatrix", action="store_true",
-        help="do not convert the matrix, saves time if the same one has been exported before to the "
-        "same directory")
+    if skipCount != 0:
+        logging.info("Could not place %d genes, these were skipped" % skipCount)
 
-    parser.add_option("", "--skipMarkers", dest="skipMarkers", action="store_true",
-            help="do not try to calculate cluster-specific marker genes. Only useful for the rare datasets where a bug in scanpy crashes the marker gene calculation.")
+    bedFname2 = bedFname.replace(".bed", ".sorted.bed")
+    cmd = "LC_COLLATE=C sort -k1,1 -k2,2n %s > %s" % (bedFname, bedFname2)
+    cellbrowser.runCommand(cmd)
 
-    (options, args) = parser.parse_args()
+    # convert to .bb using .as file
+    # from https://genome.ucsc.edu/goldenpath/help/examples/barChart/barChartBed.as
+    #asFname = join(dataDir, )
+    asFname = cellbrowser.getStaticFile(["genomes", "barChartBed.as"])
+    sizesFname = cellbrowser.getSizesFname(genome)
 
-    if showHelp:
-        parser.print_help()
-        exit(1)
+    cmd = "bedToBigBed -as=%s -type=bed6+5 -tab %s %s %s" % (asFname, bedFname2, sizesFname, bbFname)
+    cellbrowser.runCommand(cmd)
 
-    setDebug(options.debug)
-    return args, options
+def buildTrackHub(db, inMatrixFname, metaFname, clusterFieldName, clusterOrderFile, hubName, bamDir, fixDot, geneType, unitName, email, refHtmlFname, hubUrl, skipBarchart, outDir):
 
-def cbImportScanpyCli():
-    " convert h5ad to directory "
-    args, options = cbImportScanpy_parseArgs()
+    clusterToCells = parseClustersFromMeta(metaFname, clusterFieldName, fixDot)
 
-    if len(args)==0 and not options.inFile and not options.outDir:
-        cbImportScanpy_parseArgs(showHelp=True)
-        sys.exit(1)
+    if clusterOrderFile is None:
+        clusterOrder = list(sorted(clusterToCells.keys()))
+        logging.info("No cluster order specified, using clusters in alphabetical order")
+    else:
+        logging.info("Reading cluster order from %s" % clusterOrderFile)
+        clusterOrder = open(clusterOrderFile).read().splitlines()
 
-    inFname = options.inFile
-    outDir = options.outDir
-    if None in [inFname, outDir]:
-        errAbort("You need to specify at least an input .h5ad file and an output directory")
+    assert(set(clusterOrder)==set(clusterToCells)) # cluster order has to match actual cluster names
 
-    datasetName = options.datasetName
-    if datasetName is None:
-        datasetName = basename(abspath(outDir))
+    tdbFname = join(outDir, "hub.txt")
+    logging.info("Creating %s" % tdbFname)
+    tfh = open(tdbFname, "w")
 
-    markerField = options.markerField
-    clusterField = options.clusterField
-    skipMarkers = options.skipMarkers
-    matrixFormat = getMatrixFormat(options)
+    writeHubStanza(tfh, hubName, db, email)
 
-    ad = readMatrixAnndata(inFname, reqCoords=True)
+    matrixFname = join(outDir, "exprMatrix.tsv")
 
-    scanpyToCellbrowser(ad, outDir, datasetName, skipMatrix=options.skipMatrix, useRaw=(not options.useProc),
-            markerField=markerField, clusterField=clusterField, skipMarkers=skipMarkers, matrixFormat=matrixFormat)
+    bbFname = join(outDir, 'barChart.bb')
+    catFname = join(outDir, 'clusters.tsv')
+    if skipBarchart:
+        logging.info("Not creating barChart file, got command line option")
+    else:
+        writeBarChartTdb(tfh, bbFname, clusterOrder, unitName)
+        if isfile(bbFname):
+            logging.info("Not creating barChart file, %s already exists" % bbFname)
+        else:
+            makeBarGraphBigBed(db, inMatrixFname, matrixFname, geneType, clusterToCells, clusterOrder, catFname, bbFname)
 
-    copyFileIfDiffSize(inFname, join(outDir, basename(inFname)))
-    generateDataDesc(datasetName, outDir, other={"supplFiles": [{"label":"Scanpy H5AD", "file":basename(inFname)}]})
+    if bamDir:
+        mergeBams(hubName, db, tfh, bamDir, clusterToCells, outDir)
 
-    if options.port and not options.htmlDir:
-        errAbort("--port requires --htmlDir")
+    tfh.close()
 
-    if options.htmlDir:
-        build(outDir, options.htmlDir, port=options.port)
+    writeDescPages(outDir, hubName, hubUrl, refHtmlFname)
 
+def cbTrackHub(options):
+    " make track hub given meta file and directory with bam files "
+    if options.init:
+        cellbrowser.copyPkgFile("sampleConfig/cellbrowser.conf")
+        sys.exit(0)
+
+    if isfile(options.inConf):
+        conf = cellbrowser.loadConfig(options.inConf)
+
+        db = conf["ucscDb"]
+        inMatrixFname = conf["exprMatrix"]
+        metaFname = conf["meta"]
+        clusterFieldName = conf["clusterField"]
+        clusterOrderFile = conf.get("clusterOrder")
+        bamDir = conf.get("bamDir", "bam")
+        fixDot = conf.get("fixDot", False)
+        email = conf.get("hubEmail", CBEMAIL)
+        geneType = conf["geneIdType"]
+        outDir = conf["hubDir"]
+        unitName = conf.get("unit", "TPM")
+        hubUrl = conf.get("hubUrl", "")
+        refHtmlFname = conf.get("refHtml", None)
+
+        # use name, shortLabel or hubName from conf
+        hubName = conf.get("hubName", conf.get("shortLabel", conf["name"]))
+
+    if options.hubDir:
+        outDir = options.hubDir
+    if options.exprMatrix:
+        inMatrixFname = options.exprMatrix
+    if options.meta:
+        metaFname = options.meta
+    if options.clusterField:
+        clusterFieldName = options.clusterField
+    if options.clusterOrder:
+        clusterOrderFile = options.clusterOrder
+    if options.hubDir:
+        outDir = options.hubDir
+    skipBarchart = options.skipBarchart
+
+    if not isdir(outDir):
+        logging.info("Making %s" % outDir)
+        os.makedirs(outDir)
+
+    buildTrackHub(db, inMatrixFname, metaFname, clusterFieldName, clusterOrderFile, hubName, bamDir, fixDot, geneType, unitName, email, refHtmlFname, hubUrl, skipBarchart, outDir)
+
+def cbHubCli():
+    args, options = cbHub_parseArgs()
+    cbTrackHub(options, *args)
```

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/download.py` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/convert.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,480 +1,457 @@
-# download data from single cell repos
+# various format converters for single cell data:
+# - cellranger, mtx to tsv, matConcat, etc
 
-import logging, optparse, io, sys, os, shutil, operator
-from collections import defaultdict, OrderedDict, Counter
+import logging, optparse, io, sys, os, shutil, operator, glob, re
+from collections import defaultdict
 
 from .cellbrowser import runGzip, openFile, errAbort, setDebug, moveOrGzip, makeDir, iterItems
-from .cellbrowser import mtxToTsvGz, writeCellbrowserConf, parseIntoColumns, readMatrixAnndata, splitOnce
-from .cellbrowser import generateHtmls, writePyConf
+from .cellbrowser import mtxToTsvGz, writeCellbrowserConf, getAllFields, readMatrixAnndata
+from .cellbrowser import anndataToTsv, loadConfig, sanitizeName, lineFileNextRow, scanpyToCellbrowser, build
 
 from os.path import join, basename, dirname, isfile, isdir, relpath, abspath, getsize, getmtime, expanduser
 
-def cbGet_parseArgs(showHelp=False):
+def cbToolCli_parseArgs(showHelp=False):
     " setup logging, parse command line arguments and options. -h shows auto-generated help page "
-    parser = optparse.OptionParser("""usage: %prog [options] <repo> <accession> - import single cell data from repositories
+    parser = optparse.OptionParser("""usage: %prog [options] mtx2tsv|matCat|metaCat - convert various single-cell related files
 
-    The only valid repo right now is: ebi
+    mtx2tsv   - convert matrix market to .tsv.gz
+    matCat - merge expression matrices with one line per gene into a big matrix.
+        Matrices must have identical genes in the same order and the same number of
+        lines. Handles .csv files, otherwise defaults to tab-sep input. gzip OK.
+    metaCat - concat meta tables
 
     Examples:
-    - %prog ebi -a E-GEOD-100058 -o myEbiDataset - import E-GEOD-10058 to myEbiDataset/
-    - %prog ebi -i E-GEOD-100058-mirror/ -o myEbiDataset - convert E-GEOD-10058 FTP mirror to myEbiDataset/
+    - %prog mtx2tsv matrix.mtx genes.tsv barcodes.tsv exprMatrix.tsv.gz - convert .mtx to .tsv.gz file
+    - %prog matCat mat1.tsv.gz mat2.tsv.gz exprMatrix.tsv.gz - concatenate expression matrices
+    - %prog metaCat meta.tsv seurat/meta.tsv scanpy/meta.tsv newMeta.tsv - merge meta matrices
     """)
 
     parser.add_option("-d", "--debug", dest="debug", action="store_true",
         help="show debug messages")
-    parser.add_option("-a", "--accession", dest="acc", action="store",
-        help="Accession in source database")
-    parser.add_option("-i", "--inDir", dest="inDir", action="store",
-        help="Input directory")
-    parser.add_option("-o", "--outDir", dest="outDir", action="store",
-        help="Output directory")
+    parser.add_option("", "--fixDots", dest="fixDots", action="store_true",
+        help="try to fix R's mangling of various special chars to '.' in the cell IDs")
+
 
     (options, args) = parser.parse_args()
 
     if showHelp:
         parser.print_help()
         exit(1)
 
     setDebug(options.debug)
     return args, options
 
-def mirrorFtp(hostName, ftpDir, localDir):
-    " mirror an ftp directory to local disk "
-    makeDir(localDir)
-    from ftplib import FTP
-    logging.info("FTP: connecting to %s, dir %s" % (hostName, ftpDir))
-    ftp = FTP(hostName)
-    ftp.login()
-    ftp.cwd(ftpDir)
-
-    ls = ftp.nlst()
-    count = len(ls)
-    curr = 0
-    logging.info("Found {} files".format(count))
-    for fn in ls:
-        if fn=="complete":
-            continue
-        curr += 1
-        logging.info('Downloading file {} ... {} of {} ...'.format(fn, curr, count))
-        outPath = join(localDir, fn)
-        ftp.retrbinary('RETR ' + fn, open(outPath, 'wb').write)
-
-    ftp.quit()
-
-    complFn = join(localDir, "complete")
-    open(complFn, "w").close() # = create 0-size file
-    logging.info("FTP download complete.")
-
-#def downloadFromEbi(acc, outDir):
-    #" download files to outDir/orig and then create cell browser files in outDir/ "
-    #for fExt in [".clusters.tsv"]:
-        #fname = acc+fExt
-        #fileUrl = baseUrl+"/"+fname
-        #localPath = join(outDir, fname)
-
-def parseClusters(fname):
-    """ find the optimal K number in the clusters file and the cluster assignment
-    return a the value of K and a dictionary with sampleName -> clusterNumber
-    """
-    logging.info("Parsing %s" % fname)
-    bestK = None
-    for line in open(fname):
-        row = line.rstrip("\n\r").split("\t")
-        if row[0]=="sel.K":
-            sampleNames = row[2:]
-            continue
-        selK = row[0]
-        lastRow = row
-        if selK=="TRUE":
-            bestK = row[1]
-            clusters = row[2:]
-            break
-
-    if bestK is None:
-        logging.warn("No best K found, using last K")
-        bestK = lastRow[1]
-        clusters = lastK[2:]
-
-    return bestK, dict(zip(sampleNames, clusters))
-
-def parseCondSdrf(cellIds, fname):
-    """ parse the condensed sdrf into cellId -> dict of key-val """
-    cellIds = set(cellIds)
-    cellMeta = defaultdict(dict)
-    for line in open(fname):
-        #E-MTAB-7303             ERR2847884      characteristic  organism        Homo sapiens    http://purl.obolibrary.org/obo/NCBITaxon_9606
-        #E-MTAB-4850		SAMEA50486668	characteristic	age	42 year
-        row = line.rstrip("\n\r").split("\t")
-        dsId, _, cellId, _, fieldName, val = row[:6]
-        if cellId not in cellIds:
-            continue
-        cellMeta[cellId][fieldName] = val
-    return cellMeta
+def cbToolCli():
+    " run various tools from the command line "
+    args, options = cbToolCli_parseArgs()
 
-def parseSdrfFieldNames(sdrfFname):
-    " return list of field names in sdrf file "
-    ifh = open(sdrfFname)
-
-    #Source Name	Comment[ENA_SAMPLE]	Comment[BioSD_SAMPLE]	Characteristics[organism]	Characteristics[disease]	Characteristics[disease staging]	Characteristics[age]	Unit[time unit]	Characteristics[sex]	Characteristics[organism part]	Characteristics[cell type]	Characteristics[cell line]	Characteristics[single cell well quality]	Comment[single cell quality]	Material Type	Protocol REF	Protocol REF	Extract Name	Comment[LIBRARY_LAYOUT]	Comment[LIBRARY_SELECTION]	Comment[LIBRARY_SOURCE]	Comment[LIBRARY_STRAND]	Comment[LIBRARY_STRATEGY]	Comment[NOMINAL_LENGTH]	Comment[NOMINAL_SDEV]	Comment[ORIENTATION]	Comment[single cell isolation]	Comment[library construction]	Comment[input molecule]	Comment[primer]	Comment[end bias]	Protocol REF	Performer	Assay Name	Comment[technical replicate group]	Technology Type	Comment[ENA_EXPERIMENT]	Scan Name	Comment[SUBMITTED_FILE_NAME]	Comment[ENA_RUN]	Comment[FASTQ_URI]	Comment[SPOT_LENGTH]	Comment[READ_INDEX_1_BASE_COORD]	Factor value[cell line]	Factor Value[stimulus]	Factor Value[single cell identifier]
-
-    fieldNames = ifh.readline().strip("\n\r").split("\t")
-
-    newNames = []
-    for fieldName in fieldNames:
-        if "[" in fieldName:
-            fieldName = fieldName.split("[")[1].rstrip("]")
-        newNames.append(fieldName)
-    return newNames
-
-#def parseSdrf(srdfFname):
-    #""" parse EBI srdf file to list of fieldNames. Remove fields with only a single value.
-    #return a dict with the fields and values where all lines contain the same value.
-    #Also remove filename and URI fields.
-    #"""
-    #logging.debug("Parsing %s" % srdfFname)
-    #columns = parseIntoColumns(srdfFname)
-    ##cleanList = []
-    #fieldList = []
-    #genInfo = {}
-    #for fieldName, values in columns:
-        #if "[" in fieldName:
-            #fieldName = fieldName.split("[")[1].rstrip("]")
-
-        #valSet = set(values)
-
-        #logging.debug(fieldName)
-        #logging.debug(valSet)
-        #if len(valSet)==1:
-            #logging.debug("Field has only a single value, adding to info dict: %s=%s" % (fieldName, values[0]))
-            #genInfo[fieldName] = values[0]
-        #else:
-            #cleanList.append( (fieldName, values) )
-            #fieldList.append(fieldName)
-
-    #return fieldList, genInfo
-
-def parseIdf(fname):
-    " parse idf and return as dict key = value "
-    logging.debug("Parsing %s" % fname)
-    data = OrderedDict()
-    for line in open(fname, "Ut"):
-        if line.startswith("\n"):
-            continue
-        line = line.rstrip("\n")
-        key, val = splitOnce(line, "\t")
-        data[key] = val
-    return data
-
-def toStr(s):
-    " prettify raw IDF tab-sep list to a normal string "
-    return s.strip("\t").replace("\t", ", ")
-
-def translateIdf(idf):
-    " convert dict read from IDF to a simple key-value format for the cell browser desc.conf "
-    desc = OrderedDict()
-    desc["title"] = toStr(idf["Investigation Title"])
-    desc["abstract"] = toStr(idf["Experiment Description"])
-    desc["design"] = toStr(idf["Experimental Design"])
-    desc["expType"] = toStr(idf["Comment[EAExperimentType]"])
-    desc["methods"] = toStr(idf["Protocol Description"])
-    desc["curator"] = toStr(idf["Comment[EACurator]"])+", EBI Single Cell Expression Atlas"
-    desc["submitter"] = toStr(idf["Person First Name"])+" "+toStr(idf["Person Last Name"])+" <"+toStr(idf["Person Email"])+">"
-    desc["submission_date"] = toStr(idf["Public Release Date"])
-    if "PubMed ID" in idf:
-        desc["pmid"] = toStr(idf["PubMed ID"])
-    if "Publication DOI" in idf:
-        desc["doi"] = toStr(idf["Publication DOI"])
-
-    if "Comment[ArrayExpressAccession]" in idf:
-        desc["arrayexpress"] = toStr(idf["Comment[ArrayExpressAccession]"])
-
-    if "Comment [SecondaryAccession]" in idf:
-        desc["ena_project"] = toStr(idf["Comment [SecondaryAccession]"])
-
-    return desc
-
-def convertCoords(coordFname, newCoordFname):
-    " simply reorder columns"
-    ofh = open(newCoordFname, "w")
-    for line in open(coordFname):
-        row = line.rstrip("\n\r").split("\t")
-        newRow = (row[2], row[0], row[1])
-        ofh.write("\t".join(newRow))
-        ofh.write("\n")
-    ofh.close()
-    logging.info("Wrote %s" % newCoordFname)
+    if len(args)<=1:
+        cbToolCli_parseArgs(showHelp=True)
+        sys.exit(1)
 
-def convertMarkers(inFname, outFname):
-    " reorder columns and reheader and return list of one top marker per cluster "
-    #names	groups	scores	logfc	pvals	pvals_adj
-    #ENSG00000112096	0	9.120421	1.4149776	3.5174541399729827e-15	5.52275474517158e-11
-    ofh = open(outFname, "w")
-    clusterToMarkers = defaultdict(list)
-    for line in open(inFname):
-        row = line.rstrip("\n\r").split("\t")
-        #cluster, pval, auroc, gene = row
-        geneId, cluster, score, logfc, pval, pvalAdj = row
-        if row[0]=="names":
-            newRow = ["Cluster", "Gene", "p-Value Adj.", "p-Value", "logFC", "score"]
-        else:
-            newRow = (row[1], row[0], row[5], row[4], row[3], row[2])
-            clusterToMarkers[cluster].append( (float(pvalAdj), geneId) )
+    cmd = args[0]
 
-        ofh.write("\t".join(newRow))
-        ofh.write("\n")
+    cmds = ["mtx2tsv", "matCat", "metaCat"]
 
-    ofh.close()
-    logging.info("Wrote %s" % outFname)
+    if cmd=="mtx2tsv":
+        mtxFname = args[1]
+        geneFname = args[2]
+        barcodeFname = args[3]
+        outFname = args[4]
+        mtxToTsvGz(mtxFname, geneFname, barcodeFname, outFname)
+    elif cmd=="matCat":
+        inFnames = args[1:-1]
+        outFname = args[-1]
+        matCat(inFnames, outFname)
+    elif cmd=="metaCat":
+        inFnames = args[1:-1]
+        outFname = args[-1]
+        metaCat(inFnames, outFname, options)
+    else:
+        errAbort("Command %s is not a valid command. Valid commands are: %s" % (cmd, ", ".join(cmds)))
 
-    topMarkers = {}
-    for cluster, pValGenes in iterItems(clusterToMarkers):
-        pValGenes.sort()
-        topGene = pValGenes[0][1]
-        topMarkers[cluster] = topGene
-
-    return topMarkers
-
-def writeQuickGenes(topGenes, outFname):
-    " given cluster -> gene, create a quickGenes file "
-    ofh = open(outFname, "w")
-    for cluster, gene in iterItems(topGenes):
-        ofh.write("%s\tCluster %s\n"% (gene, cluster))
-    ofh.close()
-    logging.info("Wrote %s" % outFname)
+def matCat(inFnames, outFname):
+    tmpFname = outFname+".tmp"
+    ofh = openFile(tmpFname, "w")
 
-def makeBasicCbConf(name, shortLabel, hasInferred, matrixFname="exprMatrix.tsv.gz"):
-    " just fill a basic conf dict and return it "
-    c = OrderedDict()
-    c["name"] = name
-    c["shortLabel"] = shortLabel
-    c["exprMatrix"] = matrixFname
-    c["meta"] = "meta.tsv"
-    c["#priority"] = "10"
-    c["tags"] = ["ebi"]
-    c["enumFields"] = "cluster"
-
-    if hasInferred:
-        clusterField = "inferred cell type"
-        c["acroFname"] = "acronyms.tsv"
-    else:
-        clusterField = "cluster"
+    ifhs = []
+
+    sep = "\t"
+    if ".csv" in inFnames[0]:
+        sep = ","
+
+    for fn in inFnames:
+        ifhs.append( openFile(fn) )
+
+    headers, colCounts = getAllFields(ifhs, sep)
+    ofh.write("\t".join(headers))
+    ofh.write("\n")
+
+    for i, ifh in enumerate(ifhs):
+        logging.info("File %s: %d columns with values" % (ifhs[i].name, colCounts[i]-1)) 
 
-    c["clusterField"] = clusterField
-    c["labelField"] = clusterField
+    fileCount = len(inFnames)
+    progressStep = 1000
 
-    c["#unit"] = "TPM"
-    c["coords"] = [{"file":"tsne_perp25.coords.tsv", "shortLabel" : "t-SNE Perp=25"}]
-    c["markers"] = [{"file":"markers.tsv", "shortLabel":"Cluster-specific genes"}]
-    c["quickGenesFile"] = "quickGenes.tsv"
-    return c
-
-def writeMeta(clusters, cellIds, sdrfFields, boringFields, cellMeta, metaFname):
-    " write a meta.tsv file, add in the clusters "
-    #idIdx = None
-    #fieldNames = []
-    #for fieldIdx, (fieldName, vals) in enumerate(metaColumns):
-        #if fieldName=="ENA_RUN":
-            #idIdx = fieldIdx
-            #break
-        #fieldNames.append(fieldName)
-
-    #if idIdx is None:
-        #errAbort("Couldn't find the main ID field in the sdrf file. Possible field names: %s" % ",".join(fieldNames))
-
-    # basic check of the ID field
-    #idName = metaColumns[idIdx][0]
-    #idList = metaColumns[idIdx][1]
-    #if len(idList)!=len(set(idList)):
-        #idCounts = Counter(idList)
-        #errAbort("field %s was identified as the ID field, but it is not unique" % idCounts)
-
-    # put the id field first
-    #newOrder = []
-    #newOrder.append(metaColumns[idIdx])
-    #for i in range(0, idList):
-        #if i==idIdx or i==0: # remove the first source name field
-            #continue
-        #newOrder.append(metaColumns[i])
-
-    # add the cluster field
-    #clustVals = []
-    #for cellId in newOrder[0][1]:
-        #clustId = clusters[cellId]
-        #clustVals.append(clustId)
-
-    #newOrder.insert(1, ("Cluster", clustVals))
-
-    #headers = [f[0] for f in newOrder]
-
-    #fieldValues = [x[1] for x in newOrder]
-    #for i in range(0, len(idList)):
-        #row = []
-        #for field in fieldValues:
-            #row.append(field[i])
-        #ofh.write("\t".join(row))
-        #ofh.write("\n")
-    #ofh.close()
-    #logging.info("Wrote %s" % newCoordFname)
-
-    logging.debug("Fields in the SDRF: %s" % sdrfFields)
-    logging.debug("Boring fields: %s" % boringFields.keys())
-
-    allFields = set()
-    for cellId in cellIds:
-        meta = cellMeta[cellId]
-        allFields.update(meta.keys())
-    logging.debug("All fields from the condensed: %s" % allFields)
-
-    fieldOrder = []
-    doneFields = set()
-    for fn in sdrfFields:
-        if fn not in boringFields and fn in allFields and fn not in doneFields:
-            fieldOrder.append(fn)
-            doneFields.add(fn)
-
-    logging.debug("final field order: %s" % fieldOrder)
-    assert(len(set(fieldOrder))==len(fieldOrder)) # fields must not appear twice
-
-    ofh = open(metaFname, "w")
-    ofh.write("cell ID\tcluster\t")
-    ofh.write("\t".join(fieldOrder))
+    doProcess = True
+    lineCount = 0
+
+    while doProcess:
+        geneId = None
+
+        lineCount += 1
+        if lineCount % progressStep == 0:
+            logging.info("Processed %d rows" % (lineCount))
+
+        for i, ifh in enumerate(ifhs):
+            lineStr = ifh.readline()
+            # check if we're at EOF
+            if lineStr=='':
+                doProcess = False
+                break
+
+            fields = lineStr.rstrip('\r\n').split(sep)
+            fields = [x.strip('"') for x in fields]
+            if (len(fields)!=colCounts[i]): # check number of columns against header count
+                raise Exception("Illegal number of fields: file %s, line %d, field count: %d, expected %d" % 
+                    (ifh.name, lineCount, len(fields), colCounts[i]))
+
+            # check the gene ID
+            if i==0: # get the gene ID from the first file
+                geneId = fields[0]
+                allVals = [geneId]
+            else:
+                #assert(geneId == fields[0]) # if this fails, then the rows are not in the same order
+                if geneId != fields[0]:
+                    print("Error: File %s has gene IDs that is out of order." % ifh.name)
+                    print("Expected geneID: %s, got geneID: %s" % (geneId, fields[0]))
+                    sys.exit(1)
+
+            allVals.extend(fields[1:])
+
+        ofh.write("\t".join(allVals))
+        ofh.write("\n")
+
+    # make sure that we've read through all files
+    for ifh in ifhs:
+        assert(ifh.readline()=='') # a file has still lines left to read?
+
+    ofh.close()
+    moveOrGzip(tmpFname, outFname)
+    logging.info("Wrote %d lines (not counting header)" % lineCount)
+
+def metaCat(inFnames, outFname, options):
+    " merge all tsv/csv columns in inFnames into a new file, outFname. Column 1 is ID to join on. "
+    allHeaders = ["cellId"]
+    allRows = defaultdict(dict) # cellId -> fileIdx -> list of non-ID fields
+    fieldCounts = {} # fileIdx -> number of non-ID fields
+    allIds = set() # set with all cellIds
+
+    for fileIdx, fname in enumerate(inFnames):
+        headers = None
+        for row in lineFileNextRow(fname):
+            if headers is None:
+                headers = row._fields[1:]
+                logging.info("Reading %s, %d columns:  %s" % (fname, len(headers), repr(headers)))
+                allHeaders.extend(headers)
+                fieldCounts[fileIdx] = len(headers)
+
+            cellId = row[0]
+            allIds.add(cellId)
+            allRows[cellId][fileIdx] = row[1:]
+
+    nonCharRe = re.compile(r'[^a-zA-Z0-9]')
+
+    if options.fixDots:
+        # first create a map realId -> rId
+        rToReal = {}
+        for cellId, rowData in iterItems(allRows):
+            rId = nonCharRe.sub(".", cellId)
+            if rId!=cellId and rId in allRows:
+                assert(rId not in rToReal) # Uh-oh! Mapping R <-> realId is not simple. May need some manual work.
+                rToReal[rId]=cellId
+        logging.info("Found %d cell IDs that look like they've been mangled by R" % (len(rToReal)))
+
+        # now merge the R-id entries into the real ID entries
+        newRows = {}
+        for rId, readlId in iterItems(rToReal):
+            allRows[cellId].update(allRows[rId])
+        for rId in rToReal.keys():
+            del allRows[rId]
+        logging.info("Merged back rIds into normal data")
+
+    tmpFname = outFname+".tmp"
+    ofh = openFile(tmpFname, "w")
+    ofh.write("\t".join(allHeaders))
     ofh.write("\n")
 
-    for cellId, meta in iterItems(cellMeta):
-        row = [cellId]
-        clustId = clusters.get(cellId, "Unknown")
-        row.append(clustId)
-        for fieldName in fieldOrder:
-            val = meta.get(fieldName, "")
-            row.append(val)
+    for cellId, rowData in iterItems(allRows):
+        row = []
+        for fileIdx in range(0, len(inFnames)):
+            if fileIdx in rowData:
+                row.extend(rowData[fileIdx])
+            else:
+                row.extend([""]*fieldCounts[fileIdx])
+
+        ofh.write(cellId)
+        ofh.write("\t")
         ofh.write("\t".join(row))
         ofh.write("\n")
+
+    ofh.close()
+    os.rename(tmpFname, outFname)
+    logging.info("Wrote %d lines (not counting header)" % len(allRows))
+
+def crangerToCellbrowser(datasetName, inDir, outDir):
+    " convert cellranger output to a cellbrowser directory "
+    makeDir(outDir)
+    # copy over the clusters
+    clustFname = join(inDir, "analysis/clustering/graphclust/clusters.csv")
+    if not isfile(clustFname):
+        logging.warn("Cannot find %s" % clustFname)
+        clustFname = join(inDir, "analysis/kmeans/10_clusters/clusters.csv")
+        logging.warn("Using%s instead" % clustFname)
+    metaFname = join(outDir, "meta.csv")
+    shutil.copy(clustFname, metaFname)
+
+    # copy over the t-SNE coords
+    tsneFname = join(inDir, "analysis/tsne/2_components/projection.csv")
+    if not isfile(tsneFname):
+        tsneFname = join(inDir, "analysis/tsne/projection.csv")
+    coordFname = join(outDir, "tsne.coords.csv")
+    shutil.copy(tsneFname, coordFname)
+
+    # copy over the markers
+    dgeFname = join(inDir, "analysis/diffexp/graphclust/differential_expression.csv")
+    if not isfile(dgeFname):
+        logging.warn("Not found: %s" % dgeFname)
+        dgeFname = join(inDir, "analysis/kmeans/10_clusters/differential_expression.csv")
+        logging.warn("Using instead: %s" % dgeFname)
+
+    markerFname = join(outDir, "markers.tsv")
+    geneFname = join(outDir, "gene2sym.tsv")
+    crangerSignMarkers(dgeFname, markerFname, geneFname, 0.01, 100)
+
+    # convert the matrix
+    outExprFname = join(outDir, "exprMatrix.tsv.gz")
+    mask1 = join(inDir, "filtered_gene_bc_matrices/*/matrix.mtx")
+    logging.info("Looking for %s" % mask1)
+    matFnames = glob.glob(mask1)
+    if len(matFnames)!=0:
+        assert(len(matFnames)==1)
+        matFname = matFnames[0]
+        barcodeFname = matFname.replace("matrix.mtx", "barcodes.tsv")
+        geneFname = matFname.replace("matrix.mtx", "genes.tsv")
+        mtxToTsvGz(matFname, geneFname, barcodeFname, outExprFname)
+    else:
+        mask2 = join(inDir, "*_filtered_gene_bc_matrices_h5.h5")
+        logging.info("Looking for %s" % mask2)
+        matFnames = glob.glob(mask2)
+        if len(matFnames)==0:
+            errAbort("Could not find matrix, neither as %s nor as %s" % (mask1, mask2))
+        import scanpy.api as sc
+        logging.info("Reading matrix %s" % matFname)
+        adata = readMatrixAnndata(matFname)
+        anndataToTsv(adata, outExprFname)
+
+    confName = join(outDir, "cellbrowser.conf")
+    coordDescs = [{"file":"tsne.coords.csv", "shortLabel":"CellRanger t-SNE"}]
+    confArgs =  {"meta" : "meta.csv", "clusterField" : "Cluster", "tags" : ["10x"]}
+    writeCellbrowserConf(datasetName, coordDescs, confName, confArgs)
+
+    crangerWriteMethods(inDir, outDir, matFname)
+    generateDownloads(datasetName, outDir)
+
+def crangerWriteMethods(inDir, outDir, matFname):
+    htmlFname = join(outDir, "methods.html")
+    if isfile(htmlFname):
+        logging.info("%s exists, not overwriting" % htmlFname)
+        return
+
+    import csv
+    csvMask = join(inDir, "*_metrics_summary.csv")
+    csvFnames = glob.glob(csvMask)
+    if len(csvFnames)==0:
+        logging.warn("Cannot find %s, not writing %s" % (csvMask, htmlFname))
+        return
+
+    qcVals = list(csv.DictReader(open(csvFnames[0])))[0]
+
+    ofh = open(htmlFname, "w")
+    ofh.write("This dataset was imported from a CellRanger analysis directory with cbCellranger.<p><p>")
+    ofh.write("<p><b>QC metrics reported by CellRanger:</b></p>\n")
+
+    for key, value in iterItems(qcVals):
+        ofh.write("%s: %s<br>\n" % (key, value))
     ofh.close()
     logging.info("Wrote %s" % ofh.name)
 
-def findBoringFields(cellMetaDict):
-    """ return a dict of all fieldNames that have only a single value. The keys of this dict are the field names, 
-    the values of this dict are the single values."""
-    fieldValues = defaultdict(set)
-    for cellId, cellMeta in iterItems(cellMetaDict):
-        for fieldName, val in iterItems(cellMeta):
-            fieldValues[fieldName].add(val)
-
-    boringFields = {}
-    for fieldName, vals in iterItems(fieldValues):
-        if fieldName.endswith("_FILE_NAME") or fieldName.endswith("_URI") or fieldName=="single cell identifier":
-            logging.debug("Skipping field %s" % fieldName)
-            boringFields[fieldName] = None
+def generateDownloads(datasetName, outDir):
+    htmlFname = join(outDir, "downloads.html")
+    if isfile(htmlFname):
+        logging.info("%s exists, not overwriting" % htmlFname)
+        return
+
+    ofh = open(htmlFname, "w")
+    ofh.write("<b>Expression matrix:</b> <a href='%s/exprMatrix.tsv.gz'>exprMatrix.tsv.gz</a><p>\n" % datasetName)
+
+    cFname = join(outDir, "cellbrowser.conf")
+    if isfile(cFname):
+        conf = loadConfig(cFname)
+        if "unit" in conf:
+            ofh.write("Unit of expression matrix: %s<p>\n" % conf["unit"])
+
+    ofh.write("<b>Cell meta annotations:</b> <a href='%s/meta.tsv'>meta.tsv</a><p>" % datasetName)
+
+    coordDescs = conf["coords"]
+    for coordDesc in coordDescs:
+        coordLabel = coordDesc["shortLabel"]
+        cleanName = sanitizeName(coordLabel.replace(" ", "_"))
+        coordFname = cleanName+".coords.tsv.gz"
+        ofh.write("<b>%s coordinates:</b> <a href='%s/%s'>%s</a><br>" % (coordLabel, datasetName, coordFname, coordFname))
+
+    rdsFname = join(datasetName, "seurat.rds")
+    if isfile(rdsFname):
+        ofh.write("<b>Seurat R data file:</b> <a href='%s'>seurat.rds</a><p>" % rdsFname)
+
+    scriptFname = join(datasetName, "runSeurat.R")
+    if isfile(scriptFname):
+        ofh.write("<b>Seurat R analysis script:</b> <a href='%s'>runSeurat.R</a><p>" % scriptFname)
+
+    logFname = join(datasetName, "analysisLog.txt")
+    if isfile(logFname):
+        ofh.write("<b>Analysis Log File:</b> <a href='%s'>analysisLog.txt</a><p>" % logFname)
+
+def crangerSignMarkers(dgeFname, markerFname, geneFname, maxPval, maxGenes):
+    " convert cellranger diff exp file to markers.tsv file "
+    # Old Cellranger 1 format:
+    # Gene ID,Gene Name,Cluster 1 Weight,Cluster 1 UMI counts/cell,Cluster 2 Weight,Cluster 2 UMI counts/cell,Cluster 3 Weight,Cluster 3 UMI counts/cell,Cluster 4 Weight,Cluster 4 UMI counts/cell,Cluster 5 Weight,Cluster 5 UMI counts/cell,Cluster 6 Weight,Cluster 6 UMI counts/cell,Cluster 7 Weight,Cluster 7 UMI counts/cell,Cluster 8 Weight,Cluster 8 UMI counts/cell,Cluster 9 Weight,Cluster 9 UMI counts/cell,Cluster 10 Weight,Cluster 10 UMI counts/cell
+
+    ofh = open(markerFname, "w")
+    ofh.write("cluster\tgene\tAdj. P-Value\tLog2 fold change\tMean UMI Counts\n")
+
+    clusterToGenes = defaultdict(list)
+
+    # read the significant markers and their p-Values
+    for line in open(dgeFname):
+        if line.startswith("Gene ID"):
+            if "Cluster 1 Weight" in line:
+                fieldsProCluster = 2
+                fileVersion = 1
+            else:
+                fieldsProCluster = 3
+                fileVersion = 2
             continue
-        if len(vals)==1:
-            boringFields[fieldName] = list(vals)[0]
-    return boringFields
-
-def writeAcronyms(cellMeta, acroFname):
-    " extract acronyms from inferred cell name field "
-    ofh = open(acroFname, "w")
-    for cellId, metaDict in iterItems(cellMeta):
-        cellName = metaDict.get("inferred cell type")
-        if cellName and "(" in cellName:
-            longName, shortName = cellName.split("(")
-            longName = longName.strip()
-            shortName = shortName.strip(")")
-            metaDict["inferred cell type"] = shortName
-            ofh.write(shortName+"\t"+longName+"\n")
+        row = line.rstrip("\n\r").split(",")
+        geneId = row[0]
+        sym = row[1]
+        clusterCount = int((len(row)-2) / fieldsProCluster)
+        for clusterIdx in range(0, clusterCount):
+            startField = (clusterIdx*fieldsProCluster)+2
+            if fileVersion==2:
+                mean = float(row[startField])
+                fc = float(row[startField+1])
+                pVal = float(row[startField+2])
+            else:
+                fc = float(row[startField])
+                mean = float(row[startField+1])
+                pVal = 0.0001
+
+            if pVal < maxPval:
+                clusterToGenes[clusterIdx+1].append((fc, mean, pVal, sym))
+
+    # write out the markers
+    for clusterId, clusterGenes in iterItems(clusterToGenes):
+        clusterGenes.sort(key=operator.itemgetter(2)) # sort by fold change
+        maxIdx = min(maxGenes, len(clusterGenes))
+        for i in range(0, maxIdx):
+            fc, mean, pVal, sym = clusterGenes[i]
+            ofh.write("%d\t%s\t%g\t%f\t%f\n" % (clusterId, sym, pVal, fc, mean))
+
     ofh.close()
     logging.info("Wrote %s" % ofh.name)
-    return cellMeta
 
-def convertFromEbi(origDir, acc, outDir):
-    " convert single cell expression files to cell browser format "
-    # cluster is a special meta data attribute, parse it into a dict
-    clusterFname = join(origDir, acc+".clusters.tsv")
-    bestK, clusters = parseClusters(clusterFname)
-
-    # best K determines marker file name
-    markerFname = join(origDir, acc+".marker_genes_%s.tsv" % bestK)
-    newMarkerFname = join(outDir, "markers.tsv")
-    topGenes = convertMarkers(markerFname, newMarkerFname)
-
-    quickGeneFname = join(outDir, "quickGenes.tsv")
-    writeQuickGenes(topGenes, quickGeneFname)
-
-    # make sure we use the same cellID order in meta and matrix
-    sampleNameFname = join(origDir, acc+".aggregated_filtered_counts.mtx_cols")
-    sampleNames = open(sampleNameFname).read().splitlines()
-
-    # meta data
-    sdrfFname = join(origDir, acc+".sdrf.txt")
-    #fieldNames, sdrfInfo = parseSdrf(sdrfFname)
-    fieldNames = parseSdrfFieldNames(sdrfFname) # we're doing this to get them in the proper order
-    condSdrfFname = join(origDir, acc+".condensed-sdrf.tsv")
-    cellMeta = parseCondSdrf(sampleNames, condSdrfFname)
-    boringFields = findBoringFields(cellMeta)
-
-    # default perp is 25
-    coordFname = join(origDir, acc+".tsne_perp_25.tsv")
-    newCoordFname = join(outDir, "tsne_perp25.coords.tsv")
-    convertCoords(coordFname, newCoordFname)
-
-    # dataset descriptor
-    idfFname = join(origDir, acc+".idf.txt")
-    idfInfo = parseIdf(idfFname)
-    datasetDesc = translateIdf(idfInfo)
-    datasetDesc["custom"] = boringFields
-    descFname = join(outDir, "desc.conf")
-    writePyConf(datasetDesc, descFname)
-
-    # write acronyms and add the short names to the meta data
-    hasInferred = ("inferred cell type" in fieldNames)
-    if hasInferred:
-        acroFname = join(outDir, "acronyms.tsv")
-        cellMeta = writeAcronyms(cellMeta, acroFname)
-
-    # write the meta 
-    metaFname = join(outDir, "meta.tsv")
-    writeMeta(clusters, sampleNames, fieldNames, boringFields, cellMeta, metaFname)
-
-    # cellbrowser.conf file
-    confFname = join(outDir, "cellbrowser.conf")
-    conf = makeBasicCbConf(acc, datasetDesc["title"], hasInferred)
-    writePyConf(conf, confFname)
-
-    mtxName = join(origDir, acc+".aggregated_filtered_counts.mtx.gz")
-    sampleNamesFname = join(origDir, acc+".aggregated_filtered_counts.mtx_cols")
-    geneNamesFname = join(origDir, acc+".aggregated_filtered_counts.decorated.mtx_rows")
-    outMatName = join(outDir, "exprMatrix.tsv.gz")
-    #runGzip(inMatName, outMatName)
-    if not isfile(outMatName):
-        mtxToTsvGz(mtxName, geneNamesFname, sampleNamesFname, outMatName)
-
-def cbGetCli():
-    " run downloaders "
-    args, options = cbGet_parseArgs()
+def cbCellrangerCli():
+    args, options = cbCellrangerCli_parseArgs()
+
+    if options.outDir is None or options.inDir is None or options.datasetName is None:
+        logging.error("You have to specify at least an input and an output directory and a dataset name.")
+        cbCellrangerCli_parseArgs(showHelp=True)
+
+    crangerToCellbrowser(options.datasetName, options.inDir, options.outDir)
+
+def cbCellrangerCli_parseArgs(showHelp=False):
+    " setup logging, parse command line arguments and options. -h shows auto-generated help page "
+    parser = optparse.OptionParser("""usage: %prog [options] -i cellRangerDir -o outputDir - convert the cellranger output to cellbrowser format and create a cellranger.conf file
 
-    if len(args)<1:
-        cbGet_parseArgs(showHelp=True)
+    """)
+
+    parser.add_option("-d", "--debug", dest="debug", action="store_true",
+        help="show debug messages")
+
+    parser.add_option("-i", "--inDir", dest="inDir", action="store", help="input folder with the cellranger analysis output. This is the directory with the two directories 'analysis' and 'filtered_gene_bc_matrices'")
+    parser.add_option("-o", "--outDir", dest="outDir", action="store", help="output directory")
+    #parser.add_option("-g", "--geneSet", dest="geneSet", action="store", help="geneset, e.g. gencode28 or gencode-m13 or similar. Default: %default", default="gencode24")
+    parser.add_option("-n", "--name", dest="datasetName", action="store", help="name of the dataset")
+
+    (options, args) = parser.parse_args()
+
+    if showHelp:
+        parser.print_help()
+        exit(1)
+
+    setDebug(options.debug)
+
+    return args, options
+
+def cbImportScanpy_parseArgs(showHelp=False):
+    " setup logging, parse command line arguments and options. -h shows auto-generated help page "
+    parser = optparse.OptionParser("""usage: %prog [options] input.h5ad outDir datasetName - convert Scanpy AnnData object to cellbrowser
+
+    Example:
+    - %prog pbmc3k.h5ad pbmc3kScanpy pbmc3kScanpy - convert pbmc3k to directory with tab-separated files
+    """)
+
+    parser.add_option("-d", "--debug", dest="debug", action="store_true",
+        help="show debug messages")
+
+    parser.add_option("", "--htmlDir", dest="htmlDir", action="store",
+        help="do not only convert to tab-sep files but also run cbBuild to"
+            "convert the data and add the dataset under htmlDir")
+
+    parser.add_option("-p", "--port", dest="port", action="store", type="int",
+            help="only with --htmlDir: start webserver on port to serve htmlDir")
+
+    parser.add_option("-m", "--skipMatrix", dest="skipMatrix", action="store_true",
+        help="do not convert the matrix, saves time if the same one has been exported before to the "
+        "same directory")
+
+    (options, args) = parser.parse_args()
+
+    if showHelp:
+        parser.print_help()
+        exit(1)
+
+    setDebug(options.debug)
+    return args, options
+
+def cbImportScanpyCli():
+    " convert h5ad to directory "
+    args, options = cbImportScanpy_parseArgs()
+
+    if len(args)<3:
+        cbImportScanpy_parseArgs(showHelp=True)
         sys.exit(1)
 
-    outDir = options.outDir
-    if outDir is None:
-        outDir = acc
+    inFname, outDir, datasetName = args
 
-    cmd = args[0]
+    import anndata
+    ad = anndata.read_h5ad(inFname)
+    scanpyToCellbrowser(ad, outDir, datasetName, skipMatrix=options.skipMatrix)
 
-    cmds = ["ebi"]
+    if options.port and not options.htmlDir:
+        errAbort("--port requires --htmlDir")
+
+    if options.htmlDir:
+        build(outDir, options.htmlDir, port=options.port)
 
-    if cmd=="ebi":
-        acc = options.acc
-        if options.inDir:
-            origDir = options.inDir
-        else:
-            origDir = join(outDir, "orig")
-            flagFname = join(origDir, "complete")
-            logging.debug("Checking %s" % flagFname)
-            if not isfile(flagFname):
-                hostName = "ftp.ebi.ac.uk"
-                ftpDir = "/pub/databases/microarray/data/atlas/sc_experiments/%s" % acc
-                mirrorFtp(hostName, ftpDir, origDir)
-        convertFromEbi(origDir, acc, outDir)
-    else:
-        errAbort("Repository %s is not valid. Valid repos are: %s" % (cmd, ", ".join(cmds)))
```

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser/geneinfo.py` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser/geneinfo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 # annotate a list of gene IDs with links to various external databases
 
 import logging, sys, optparse, re, unicodedata, string, csv
 from collections import defaultdict, namedtuple
 from os.path import join, basename, dirname, isfile
 
-from .cellbrowser import openStaticFile, staticFileNextRow, openFile, splitOnce, iterItems, lineFileNextRow, setDebug
-from .cellbrowser import readGeneSymbols
-
 dataDir = "geneAnnot"
 
-# no spaces/special chars in filenames - otherwise the URL will be rejected as invalid by urllib2
 HPRD = join(dataDir, "HPRD_molecular_class_081914.txt")
 HGNC = join(dataDir, "hgnc_complete_set_05Dec17.txt")
 SFARI = join(dataDir, "SFARI-Gene_genes_export06-12-2017.csv")
 OMIM = join(dataDir, "mim2gene.txt")
-COSMIC = join(dataDir, "Census_allWed_Dec__6_18_35_54_2017.tsv")
+COSMIC = join(dataDir, "Census_allWed Dec  6 18_35_54 2017.tsv")
 HPO = join(dataDir, "hpo_frequent_7Dec17.txt")
 BRAINSPANLMD = join(dataDir, "brainspan_genes.csv")
 BRAINSPANMOUSEDEV = join(dataDir, "brainspanMouse_9Dec17.txt")
 MGIORTHO = join(dataDir, "mgi_HGNC_homologene_8Dec17.txt")
 EUREXPRESS = join(dataDir, "eurexpress_7Dec17.txt")
 DDD = join(dataDir, "DDG2P_18_10_2018.csv.gz")
 
+from cellbrowser import openStaticFile, staticFileNextRow, openFile
 
 # ==== functions =====
     
 def parseArgs():
     " setup logging, parse command line arguments and options. -h shows auto-generated help page "
     parser = optparse.OptionParser("""usage: %prog [options] inFname outFname - annotate a tab-sep gene list file with information from other databases
             
-    A minimal input file has a header line with at one field called "gene" (=symbol or ENS/Entrez geneID) and
+    A minimal input file has a header line with at one field called "gene" (=symbol) and
     one field called "cluster".
     
     In the cellbrowser, the cluster name should match the cluster name in the meta data file.""")
 
     parser.add_option("-d", "--debug", dest="debug", action="store_true", help="show debug messages")
     parser.add_option("", "--hprd", dest="hprd", action="store", help="location of HPRD file, default %default", default=HPRD)
     parser.add_option("", "--hgnc", dest="hgnc", action="store", help="location of HGNC file, default %default", default=HGNC)
@@ -49,21 +46,72 @@
     #parser.add_option("", "--test", dest="test", action="store_true", help="do something") 
     (options, args) = parser.parse_args()
 
     if args==[]:
         parser.print_help()
         exit(1)
 
-    setDebug(options.debug)
+    if options.debug:
+        logging.basicConfig(level=logging.DEBUG)
+    else:
+        logging.basicConfig(level=logging.INFO)
     return args, options
 
+def lineFileNextRow(inFile):
+    """
+    parses tab-sep file with headers in first line
+    yields collection.namedtuples
+    strips "#"-prefix from header line
+    """
+
+    if isinstance(inFile, str):
+        fh = openFile(inFile)
+    else:
+        fh = inFile
+
+    line1 = fh.readline()
+    line1 = line1.strip("\n").lstrip("#")
+    headers = line1.split("\t")
+    headers = [re.sub("[^a-zA-Z0-9_]","_", h) for h in headers]
+    headers = [re.sub("^_","", h) for h in headers] # remove _ prefix
+    headers = [x if x!="" else "noName" for x in headers]
+
+    filtHeads = []
+    for h in headers:
+        if h[0].isdigit():
+            filtHeads.append("x"+h)
+        else:
+            filtHeads.append(h)
+    headers = filtHeads
+
+
+    Record = namedtuple('tsvRec', headers)
+    for line in fh:
+        if line.startswith("#"):
+            continue
+        line = line.decode("latin1")
+        # skip special chars in meta data and keep only ASCII
+        line = unicodedata.normalize('NFKD', line).encode('ascii','ignore')
+        line = line.rstrip("\n").rstrip("\r")
+        fields = string.split(line, "\t", maxsplit=len(headers)-1)
+        try:
+            rec = Record(*fields)
+        except Exception as e:
+            logging.error("Exception occured while parsing line, %s" % e)
+            logging.error("Filename %s" % fh.name)
+            logging.error("Line was: %s" % line)
+            logging.error("Does number of fields match headers?")
+            logging.error("Headers are: %s" % headers)
+            raise Exception("header count: %d != field count: %d wrong field count in line %s" % (len(headers), len(fields), line))
+        yield rec
+
 # ----------- main --------------
 def parseBrainspanLmd(inFname):
     " return entrez -> brainspanGeneId with all entrez IDs that are in the brainspan LMD set "
-    with openStaticFile(inFname, 'r') as csvfile:
+    with openStaticFile(inFname, 'rb') as csvfile:
         ret = {}
         cr = csv.reader(csvfile)
         headers = None
         for row in cr:
             if headers == None:
                 assert(row==['row_num','gene_id','ensembl_gene_id','gene_symbol','entrez_id'])
                 headers = row
@@ -83,15 +131,15 @@
             "4" : "Autism, 4 - Minimal evidence",
             "5" : "Autism, 5 - Hypothesized but untested",
             "6" : "Autism, 6 - Evidence does not support role",
     }
     # ['status', 'gene-symbol', 'gene-name', 'chromosome', 'genetic-category', 'gene-score', 'syndromic', 'number-of-reports']
     headers = None
     ret = {}
-    with openStaticFile(inFname, 'r') as csvfile:
+    with openStaticFile(inFname, 'rb') as csvfile:
         spamreader = csv.reader(csvfile)
         for row in spamreader:
             if headers == None:
                 headers = row
                 assert(headers[5]=="gene-score")
                 continue
             score = row[5]
@@ -155,15 +203,15 @@
             continue
         row = line.rstrip("\n").split("\t")
         entrez = row[2]
         hpoName = row[4]
         geneToNames[entrez].add(hpoName)
 
     ret = {}
-    for entrez, names in iterItems(geneToNames):
+    for entrez, names in geneToNames.iteritems():
         names = list(names)
         names.sort()
         ret[entrez] = ", ".join(names)
     return ret
 
 def parseMgiOrtho(hgncIdToEntrez, inFname):
     " return dict with mouse entrezId -> human entrez "
@@ -197,71 +245,54 @@
         if row.EMAP_Term!="":
             entrezToTerms[humanEntrez].add(row.EMAP_Term)
         entrezToEuroexpress[humanEntrez] = row.Assay_ID
 
     logging.info("Eurexpress mouse entrez IDs: %d mappable, %d not-mappable to human " % (len(entrezToEuroexpress),len(skippedMouseIds)))
     logging.debug("Eurexpress mouse: mouse entrez IDs not mappable to human: %s" % ",".join(skippedMouseIds))
     ret = {}
-    for entrezId, terms in iterItems(entrezToTerms):
+    for entrezId, terms in entrezToTerms.iteritems():
         eurexpId = entrezToEuroexpress[entrezId]
         ret[entrezId] = (eurexpId, ", ".join(sorted(list(terms))))
 
     return ret
 
 def parseDDD(fname):
     " parse DDD phenotype file "
     ret = {}
-    #for row in staticFileNextRow(inFname):
-        #print row
+    for row in staticFileNextRow(inFname):
+        print row
     return ret
     
 def parseSimpleMap(inFname):
     " parse simple tab-sep key-value file and return as dict "
     ret = {}
     for line in openStaticFile(inFname):
         row = line.rstrip("\n").split("\t")
         ret[row[0]] = row[1]
     return ret
 
 def tabGeneAnnotate(inFname, symToEntrez, symToSfari, entrezToClass, entrezToOmim, entrezToCosmic, entrezToHpo, entrezToLmd, entrezToEuroexpress, humanToMouseEntrezList, mouseEntrezToBrainspanMouseDev):
     " "
     headers = None
-    geneToSym = -1
     for row in lineFileNextRow(inFname):
         if headers is None:
             headers = list(row._fields)
             headers.append("_hprdClass")
             headers.append("_expr")
             headers.append("_geneLists")
             yield headers
-        sym = row[1]
-        if "|" in sym: # marker gene lists can carry geneId|symbol, strip the symbol in this case and re-convert below
-            sym = sym.split("|")[0]
-        if "." in sym: # remove Ensembl version identifier
-            sym = sym.split(".")[0]
-
-        # convert gene IDs to symbols
-        if geneToSym is -1:
-            geneToSym = readGeneSymbols(None, [sym])
-        if geneToSym is not None:
-            geneId = geneToSym.get(sym)
-            if geneId is None:
-                logging.debug("Cannot find NCBI Gene ID for symbol: %s" % sym)
-                geneId = sym
-            sym = geneId
-
+        sym = row.gene
         hprdClass = ""
         entrezId = symToEntrez.get(sym)
-
-        if entrezId == None:
-            logging.debug("Cannot find entrezId for symbol %s" % sym)
+        omimId = entrezToOmim.get(entrezId, "")
+        if entrezId != None:
+            hprdClass = entrezToClass.get(entrezId, "")
 
         # now summarize the presence/absence of this gene in various specialized gene lists:
         # OMIM, COSMIC, SFARI
-        hprdClass = entrezToClass.get(entrezId, "")
         geneLists = []
         if sym!="":
             # SFARI
             sfariInfo = symToSfari.get(sym)
             if sfariInfo is not None:
                 sfariInfo = "SFARI||"+sfariInfo
                 geneLists.append(sfariInfo)
@@ -298,15 +329,14 @@
 
             mouseEntrezList = humanToMouseEntrezList[entrezId]
             for mouseEntrez in mouseEntrezList:
                 if mouseEntrez in mouseEntrezToBrainspanMouseDev:
                     exprParts.append("BrainSpMouseDev|"+mouseEntrezToBrainspanMouseDev[mouseEntrez])
 
         row = list(row)
-        row[1] = sym # in case the original ID was a geneID, not a symbol
 
         row.append(hprdClass)
         row.append(";".join(exprParts))
         row.append(";".join(geneLists))
 
         yield row
 
@@ -325,18 +355,14 @@
     symToSfari = parseSfari(options.sfari)
     entrezToClass = parseHprd(options.hprd)
     #symToDdd = parseDdd(DDD)
 
     filename = args[0]
     outFname = args[1]
 
-    rowCount = 0
     ofh = open(outFname, "w")
     for row in tabGeneAnnotate(filename, symToEntrez, symToSfari, entrezToClass, entrezToOmim, entrezToCosmic, entrezToHpo, entrezToLmd, entrezToEuroexpress, humanToMouseEntrezList, entrezToBrainspanMouseDev):
         ofh.write("\t".join(row))
         ofh.write("\n")
-        rowCount +=1
     ofh.close()
 
-    logging.info("Annotated %d marker gene rows, output written to %s" % (rowCount, outFname))
-
```

### Comparing `cellbrowser-1.2.3/src/cbPyLib/cellbrowser.egg-info/entry_points.txt` & `cellbrowser-v0.4.27/src/cbPyLib/cellbrowser.egg-info/entry_points.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 [console_scripts]
 cbBuild = cellbrowser.cellbrowser:cbBuildCli
-cbGenes = cellbrowser.genes:cbGenesCli
 cbGuessGencode = cellbrowser.guessgenes:cbGuessGencodeCli
-cbHub = cellbrowser.hubmaker:cbHubCli
 cbImportCellranger = cellbrowser.convert:cbCellrangerCli
 cbImportScanpy = cellbrowser.convert:cbImportScanpyCli
-cbImportSeurat = cellbrowser.seurat:cbImportSeuratCli
+cbImportSeurat2 = cellbrowser.seurat:cbImportSeurat2Cli
 cbMarkerAnnotate = cellbrowser.geneinfo:cbMarkerAnnotateCli
 cbScanpy = cellbrowser.cellbrowser:cbScanpyCli
 cbSeurat = cellbrowser.seurat:cbSeuratCli
 cbTool = cellbrowser.convert:cbToolCli
-cbUpgrade = cellbrowser.cellbrowser:cbUpgradeCli
+cbUpgrade = cellbrowser.cellbrowser:cbMake_cli
```

### Comparing `cellbrowser-1.2.3/MANIFEST.in` & `cellbrowser-v0.4.27/MANIFEST.in`

 * *Files 8% similar despite different names*

```diff
@@ -6,10 +6,8 @@
 #include ../src/cbPyLib/cellbrowser/sampleConfig/cellbrowser.conf
 #include ../src/cbPyLib/cellbrowser/sampleConfig/scanpy.conf
 #include ../src/cbPyLib/cellbrowser/sampleConfig/seurat.conf
 #include cellbrowser/sampleConfig/cellbrowser.conf
 #include cellbrowser/sampleConfig/scanpy.conf
 ##include cellbrowser/sampleConfig/seurat.conf
 include versioneer.py
-include LICENSE
 include src/cbPyLib/cellbrowser/_version.py
-graft src/cbPyLib/cellbrowser/R
```

### Comparing `cellbrowser-1.2.3/versioneer.py` & `cellbrowser-v0.4.27/versioneer.py`

 * *Files identical despite different names*

