# Comparing `tmp/pyteseo-0.0.5.tar.gz` & `tmp/pyteseo-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyteseo-0.0.5.tar", last modified: Fri Jan 20 07:17:11 2023, max compression
+gzip compressed data, was "pyteseo-0.0.6.tar", last modified: Tue May 23 15:50:47 2023, max compression
```

## Comparing `pyteseo-0.0.5.tar` & `pyteseo-0.0.6.tar`

### file list

```diff
@@ -1,130 +1,521 @@
--rw-r--r--   0        0        0    53248 2023-01-19 16:56:25.218033 pyteseo-0.0.5/.coverage
--rw-r--r--   0        0        0      146 2023-01-16 10:54:35.633143 pyteseo-0.0.5/.flake8
--rw-r--r--   0        0        0     1356 2023-01-19 17:26:11.438053 pyteseo-0.0.5/.github/workflows/docs.yml
--rw-r--r--   0        0        0      849 2023-01-16 17:30:19.103271 pyteseo-0.0.5/.github/workflows/tests.yml
--rw-r--r--   0        0        0      180 2023-01-19 16:35:42.748020 pyteseo-0.0.5/.gitignore
--rw-r--r--   0        0        0      504 2023-01-16 10:53:29.863142 pyteseo-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1819 2023-01-19 16:35:42.748020 pyteseo-0.0.5/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2023-01-09 15:21:18.437908 pyteseo-0.0.5/LICENSE.md
--rw-r--r--   0        0        0     4436 2023-01-17 07:05:42.131705 pyteseo-0.0.5/README.md
--rw-r--r--   0        0        0      634 2022-12-28 11:40:36.607121 pyteseo-0.0.5/docs/Makefile
--rw-r--r--   0        0        0    31102 2022-12-28 11:40:36.627121 pyteseo-0.0.5/docs/_static/TESEO_logo.png
--rw-r--r--   0        0        0    84936 2023-01-09 07:22:45.451292 pyteseo-0.0.5/docs/_static/doc_snapshoot.png
--rw-r--r--   0        0        0    28715 2022-12-28 11:40:36.627121 pyteseo-0.0.5/docs/_static/pyTESEO_logo.png
--rw-r--r--   0        0        0       55 2023-01-13 08:20:28.115803 pyteseo-0.0.5/docs/changelog.md
--rw-r--r--   0        0        0     1548 2023-01-19 17:47:12.458066 pyteseo-0.0.5/docs/conf.py
--rw-r--r--   0        0        0     2350 2023-01-13 08:20:28.115803 pyteseo-0.0.5/docs/get-started.md
--rw-r--r--   0        0        0     2211 2023-01-13 08:20:28.115803 pyteseo-0.0.5/docs/index.md
--rw-r--r--   0        0        0      800 2022-12-28 11:40:36.627121 pyteseo-0.0.5/docs/make.bat
--rw-r--r--   0        0        0   319832 2023-01-19 17:19:42.158048 pyteseo-0.0.5/docs/notebooks/01_read_domain.ipynb
--rw-r--r--   0        0        0    42092 2023-01-19 17:19:29.668048 pyteseo-0.0.5/docs/notebooks/02_read_forcings.ipynb
--rw-r--r--   0        0        0   938683 2023-01-20 07:12:44.885533 pyteseo-0.0.5/docs/notebooks/03_export_results.ipynb
--rw-r--r--   0        0        0      715 2023-01-19 16:35:42.758020 pyteseo-0.0.5/docs/notebooks/04_floater_simulation.ipynb
--rw-r--r--   0        0        0      711 2023-01-19 16:35:42.758020 pyteseo-0.0.5/docs/notebooks/05_oil_simulation.ipynb
--rw-r--r--   0        0        0      711 2023-01-19 16:35:42.758020 pyteseo-0.0.5/docs/notebooks/06_hns_simulation.ipynb
--rw-r--r--   0        0        0      757 2023-01-19 16:35:42.758020 pyteseo-0.0.5/docs/notebooks/07_stochastic_montecarlo.ipynb
--rw-r--r--   0        0        0      753 2023-01-19 16:35:42.758020 pyteseo-0.0.5/docs/notebooks/08_stochastic_kmeans.ipynb
--rw-r--r--   0        0        0      974 2023-01-11 10:07:46.886424 pyteseo-0.0.5/docs/user-guide.md
--rw-r--r--   0        0        0      296 2023-01-13 09:50:35.295832 pyteseo-0.0.5/environment-dev.yml
--rw-r--r--   0        0        0      181 2023-01-13 08:20:28.115803 pyteseo-0.0.5/environment.yml
--rw-r--r--   0        0        0     1867 2023-01-19 16:35:42.758020 pyteseo-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      193 2023-01-19 16:53:59.988032 pyteseo-0.0.5/pyteseo/__init__.py
--rw-r--r--   0        0        0      421 2023-01-19 16:35:42.768020 pyteseo-0.0.5/pyteseo/config.py
--rw-r--r--   0        0        0     2780 2023-01-19 16:35:42.768020 pyteseo-0.0.5/pyteseo/defaults.json
--rw-r--r--   0        0        0      322 2023-01-19 16:54:05.698032 pyteseo-0.0.5/pyteseo/defaults.py
--rw-r--r--   0        0        0     6897 2023-01-19 16:54:21.228032 pyteseo-0.0.5/pyteseo/export.py
--rw-r--r--   0        0        0    19360 2023-01-19 16:54:13.038032 pyteseo-0.0.5/pyteseo/io.py
--rw-r--r--   0        0        0      477 2023-01-13 13:57:58.135913 pyteseo-0.0.5/pyteseo/plot.py
--rw-r--r--   0        0        0      291 2023-01-13 08:20:28.115803 pyteseo-0.0.5/pyteseo/tests/__init__.py
--rw-r--r--   0        0        0     1080 2022-11-28 12:31:04.243939 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000000.txt
--rw-r--r--   0        0        0     1440 2022-11-28 12:31:25.250905 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000005.txt
--rw-r--r--   0        0        0     1320 2022-11-28 12:31:42.101870 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000010.txt
--rw-r--r--   0        0        0     1440 2022-11-28 12:31:56.340847 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000015.txt
--rw-r--r--   0        0        0     1800 2022-11-28 12:32:08.201821 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000020.txt
--rw-r--r--   0        0        0     1920 2022-11-28 12:32:19.311799 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000025.txt
--rw-r--r--   0        0        0     1800 2022-11-28 12:32:30.205778 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000030.txt
--rw-r--r--   0        0        0     1920 2022-11-28 12:32:40.120760 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000035.txt
--rw-r--r--   0        0        0     1920 2022-11-28 12:32:49.096757 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000040.txt
--rw-r--r--   0        0        0     2040 2022-11-28 12:32:56.968763 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000045.txt
--rw-r--r--   0        0        0     2280 2022-11-28 12:33:04.886785 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000050.txt
--rw-r--r--   0        0        0     2640 2022-11-28 12:33:12.049766 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000055.txt
--rw-r--r--   0        0        0     2640 2022-11-28 12:33:19.004754 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000060.txt
--rw-r--r--   0        0        0     3240 2022-11-28 12:33:49.743762 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000065.txt
--rw-r--r--   0        0        0     3840 2022-11-28 12:33:56.320750 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000070.txt
--rw-r--r--   0        0        0     3960 2022-11-28 12:34:03.214770 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000075.txt
--rw-r--r--   0        0        0     4440 2022-11-28 12:34:09.897757 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000080.txt
--rw-r--r--   0        0        0     4920 2022-11-28 12:34:17.619757 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000085.txt
--rw-r--r--   0        0        0     5280 2022-11-28 12:34:25.163765 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000090.txt
--rw-r--r--   0        0        0     1080 2022-11-28 12:31:04.243939 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000000.txt
--rw-r--r--   0        0        0     1440 2022-11-28 12:31:25.250905 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000005.txt
--rw-r--r--   0        0        0     1320 2022-11-28 12:31:42.101870 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000010.txt
--rw-r--r--   0        0        0     1440 2022-11-28 12:31:56.340847 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000015.txt
--rw-r--r--   0        0        0     1800 2022-11-28 12:32:08.201821 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000020.txt
--rw-r--r--   0        0        0     1920 2022-11-28 12:32:19.311799 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000025.txt
--rw-r--r--   0        0        0     1800 2022-11-28 12:32:30.205778 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000030.txt
--rw-r--r--   0        0        0     1920 2022-11-28 12:32:40.120760 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000035.txt
--rw-r--r--   0        0        0     1920 2022-11-28 12:32:49.096757 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000040.txt
--rw-r--r--   0        0        0     2040 2022-11-28 12:32:56.968763 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000045.txt
--rw-r--r--   0        0        0     2280 2022-11-28 12:33:04.886785 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000050.txt
--rw-r--r--   0        0        0     2640 2022-11-28 12:33:12.049766 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000055.txt
--rw-r--r--   0        0        0     2640 2022-11-28 12:33:19.004754 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000060.txt
--rw-r--r--   0        0        0     3240 2022-11-28 12:33:49.743762 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000065.txt
--rw-r--r--   0        0        0     3840 2022-11-28 12:33:56.320750 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000070.txt
--rw-r--r--   0        0        0     3960 2022-11-28 12:34:03.214770 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000075.txt
--rw-r--r--   0        0        0     4440 2022-11-28 12:34:09.897757 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000080.txt
--rw-r--r--   0        0        0     4920 2022-11-28 12:34:17.619757 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000085.txt
--rw-r--r--   0        0        0     5280 2022-11-28 12:34:25.163765 pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000090.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:31:04.219939 pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000000.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:31:25.362903 pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000005.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:31:42.232868 pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000010.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:31:56.503846 pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000015.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:32:08.296824 pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000020.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:32:19.402804 pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000025.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:32:30.379778 pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000030.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:32:40.259760 pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000035.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:32:49.222751 pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000040.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:32:57.430761 pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000045.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:33:04.996780 pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000050.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:33:12.191766 pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000055.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:33:19.144753 pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000060.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:33:49.896767 pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000065.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:33:56.794749 pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000070.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:34:03.348770 pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000075.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:34:10.956756 pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000080.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:34:18.079761 pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000085.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:34:25.335761 pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000090.txt
--rw-r--r--   0        0        0   121220 2022-11-28 12:59:56.013665 pyteseo-0.0.5/pyteseo/tests/data/cas1_properties_001.txt
--rw-r--r--   0        0        0   121220 2022-11-28 12:59:56.013665 pyteseo-0.0.5/pyteseo/tests/data/cas1_properties_002.txt
--rw-r--r--   0        0        0   574769 2023-01-13 08:20:28.115803 pyteseo-0.0.5/pyteseo/tests/data/coastline.dat
--rw-r--r--   0        0        0   574787 2023-01-13 08:20:28.125803 pyteseo-0.0.5/pyteseo/tests/data/coastline_error_range.dat
--rw-r--r--   0        0        0   574787 2023-01-13 08:20:28.125803 pyteseo-0.0.5/pyteseo/tests/data/coastline_othernanformat.dat
--rw-r--r--   0        0        0   558324 2015-03-24 16:18:44.000000 pyteseo-0.0.5/pyteseo/tests/data/costa_poligono1.dat
--rw-r--r--   0        0        0     3861 2015-03-24 16:18:44.000000 pyteseo-0.0.5/pyteseo/tests/data/costa_poligono2.dat
--rw-r--r--   0        0        0    10412 2023-01-13 08:20:28.125803 pyteseo-0.0.5/pyteseo/tests/data/costa_poligono3.dat
--rw-r--r--   0        0        0     2183 2023-01-13 08:20:28.125803 pyteseo-0.0.5/pyteseo/tests/data/costa_poligono4.dat
--rw-r--r--   0        0        0      732 2022-11-14 07:58:35.871414 pyteseo-0.0.5/pyteseo/tests/data/currents_000h.txt
--rw-r--r--   0        0        0      732 2023-01-09 17:03:42.920654 pyteseo-0.0.5/pyteseo/tests/data/currents_000h_error_range.txt
--rw-r--r--   0        0        0      732 2023-01-09 17:03:42.920654 pyteseo-0.0.5/pyteseo/tests/data/currents_000h_error_sort.txt
--rw-r--r--   0        0        0      912 2023-01-09 17:03:12.460654 pyteseo-0.0.5/pyteseo/tests/data/currents_000h_error_var.txt
--rw-r--r--   0        0        0      732 2022-11-14 07:58:35.950414 pyteseo-0.0.5/pyteseo/tests/data/currents_001h.txt
--rw-r--r--   0        0        0      732 2022-11-14 07:58:36.019414 pyteseo-0.0.5/pyteseo/tests/data/currents_002h.txt
--rw-r--r--   0        0        0      732 2022-11-14 07:58:36.125414 pyteseo-0.0.5/pyteseo/tests/data/currents_003h.txt
--rw-r--r--   0        0        0  3177300 2015-03-24 16:18:44.000000 pyteseo-0.0.5/pyteseo/tests/data/grid.dat
--rw-r--r--   0        0        0  1969957 2022-11-28 12:30:41.129982 pyteseo-0.0.5/pyteseo/tests/data/grid_coordinates.txt
--rw-r--r--   0        0        0  3177300 2023-01-09 16:47:33.450649 pyteseo-0.0.5/pyteseo/tests/data/grid_error_range.dat
--rw-r--r--   0        0        0  3177300 2023-01-09 16:47:49.940649 pyteseo-0.0.5/pyteseo/tests/data/grid_error_sort.dat
--rw-r--r--   0        0        0  3177492 2023-01-09 16:48:14.190649 pyteseo-0.0.5/pyteseo/tests/data/grid_error_var.dat
--rw-r--r--   0        0        0       72 2023-01-09 16:55:02.280651 pyteseo-0.0.5/pyteseo/tests/data/lstcurr_UVW.pre
--rw-r--r--   0        0        0       84 2023-01-09 17:06:06.370655 pyteseo-0.0.5/pyteseo/tests/data/lstcurr_UVW_error_range.pre
--rw-r--r--   0        0        0       83 2023-01-09 17:06:06.380655 pyteseo-0.0.5/pyteseo/tests/data/lstcurr_UVW_error_sort.pre
--rw-r--r--   0        0        0       82 2023-01-09 17:06:06.360655 pyteseo-0.0.5/pyteseo/tests/data/lstcurr_UVW_error_var.pre
--rw-r--r--   0        0        0       60 2023-01-13 08:20:28.125803 pyteseo-0.0.5/pyteseo/tests/data/lstwinds.pre
--rw-r--r--   0        0        0      732 2022-11-14 07:58:35.871414 pyteseo-0.0.5/pyteseo/tests/data/winds_000h.txt
--rw-r--r--   0        0        0      732 2022-11-14 07:58:35.950414 pyteseo-0.0.5/pyteseo/tests/data/winds_001h.txt
--rw-r--r--   0        0        0      732 2022-11-14 07:58:36.019414 pyteseo-0.0.5/pyteseo/tests/data/winds_002h.txt
--rw-r--r--   0        0        0      732 2022-11-14 07:58:36.125414 pyteseo-0.0.5/pyteseo/tests/data/winds_003h.txt
--rw-r--r--   0        0        0      441 2023-01-19 16:56:19.048033 pyteseo-0.0.5/pyteseo/tests/test_defaults.py
--rw-r--r--   0        0        0     2598 2023-01-19 16:35:42.768020 pyteseo-0.0.5/pyteseo/tests/test_export.py
--rw-r--r--   0        0        0     8961 2023-01-19 16:55:07.558032 pyteseo-0.0.5/pyteseo/tests/test_io.py
--rw-r--r--   0        0        0        0 2023-01-09 16:30:26.000643 pyteseo-0.0.5/pyteseo/tests/test_plot.py
--rw-r--r--   0        0        0     6178 1970-01-01 00:00:00.000000 pyteseo-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    53248 2023-05-23 10:32:12.589254 pyteseo-0.0.6/.coverage
+-rw-r--r--   0        0        0      169 2023-01-23 16:09:52.078560 pyteseo-0.0.6/.flake8
+-rw-r--r--   0        0        0     1545 2023-04-17 10:00:47.217406 pyteseo-0.0.6/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1101 2023-05-12 06:59:34.879572 pyteseo-0.0.6/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      179 2023-04-25 08:09:50.561302 pyteseo-0.0.6/.gitignore
+-rw-r--r--   0        0        0      504 2023-01-16 10:53:29.863142 pyteseo-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2710 2023-05-23 11:45:21.401972 pyteseo-0.0.6/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2023-05-22 06:33:42.865296 pyteseo-0.0.6/LICENSE.md
+-rw-r--r--   0        0        0     4271 2023-05-23 11:38:39.646969 pyteseo-0.0.6/README.md
+-rw-r--r--   0        0        0      634 2022-12-28 11:40:36.607121 pyteseo-0.0.6/docs/Makefile
+-rw-r--r--   0        0        0    31102 2022-12-28 11:40:36.627121 pyteseo-0.0.6/docs/_static/TESEO_logo.png
+-rw-r--r--   0        0        0    84936 2023-01-09 07:22:45.451292 pyteseo-0.0.6/docs/_static/doc_snapshoot.png
+-rw-r--r--   0        0        0    28715 2022-12-28 11:40:36.627121 pyteseo-0.0.6/docs/_static/pyTESEO_logo.png
+-rw-r--r--   0        0        0       55 2023-01-13 08:20:28.115803 pyteseo-0.0.6/docs/changelog.md
+-rw-r--r--   0        0        0     1822 2023-01-20 10:27:58.065661 pyteseo-0.0.6/docs/conf.py
+-rw-r--r--   0        0        0     2350 2023-01-13 08:20:28.115803 pyteseo-0.0.6/docs/get-started.md
+-rw-r--r--   0        0        0     2211 2023-01-13 08:20:28.115803 pyteseo-0.0.6/docs/index.md
+-rw-r--r--   0        0        0      800 2022-12-28 11:40:36.627121 pyteseo-0.0.6/docs/make.bat
+-rw-r--r--   0        0        0   263466 2023-05-15 10:11:00.364302 pyteseo-0.0.6/docs/notebooks/01_read_domain.ipynb
+-rw-r--r--   0        0        0    42212 2023-05-11 13:51:39.835822 pyteseo-0.0.6/docs/notebooks/02_read_forcings.ipynb
+-rw-r--r--   0        0        0   947681 2023-05-11 13:51:51.776549 pyteseo-0.0.6/docs/notebooks/03_export_results.ipynb
+-rw-r--r--   0        0        0    17456 2023-05-11 13:52:48.710040 pyteseo-0.0.6/docs/notebooks/04_generate_forcings_from_cmems.ipynb
+-rw-r--r--   0        0        0   116574 2023-05-11 13:59:37.901052 pyteseo-0.0.6/docs/notebooks/05_drift_simulation.ipynb
+-rw-r--r--   0        0        0      711 2023-01-19 16:35:42.758020 pyteseo-0.0.6/docs/notebooks/06_hns_simulation.ipynb
+-rw-r--r--   0        0        0      686 2023-05-11 13:54:12.425183 pyteseo-0.0.6/docs/notebooks/07_stochastic_montecarlo.ipynb
+-rw-r--r--   0        0        0      753 2023-01-19 16:35:42.758020 pyteseo-0.0.6/docs/notebooks/08_stochastic_kmeans.ipynb
+-rw-r--r--   0        0        0      974 2023-01-11 10:07:46.886424 pyteseo-0.0.6/docs/user-guide.md
+-rw-r--r--   0        0        0      407 2023-05-17 07:12:34.718790 pyteseo-0.0.6/environment-dev.yml
+-rw-r--r--   0        0        0      235 2023-05-17 07:12:57.360321 pyteseo-0.0.6/environment.yml
+-rw-r--r--   0        0        0     1933 2023-05-23 15:33:31.407192 pyteseo-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      361 2023-04-18 11:50:41.715252 pyteseo-0.0.6/pyteseo/__init__.py
+-rw-r--r--   0        0        0     7776 2023-05-22 08:13:07.751692 pyteseo-0.0.6/pyteseo/classes.py
+-rw-r--r--   0        0        0        0 2023-02-13 12:13:20.197722 pyteseo-0.0.6/pyteseo/connections/__init__.py
+-rw-r--r--   0        0        0     2346 2023-05-18 14:24:41.952116 pyteseo-0.0.6/pyteseo/connections/bathymetries.py
+-rw-r--r--   0        0        0     5957 2023-05-22 06:19:42.815869 pyteseo-0.0.6/pyteseo/connections/cmems.py
+-rw-r--r--   0        0        0     3132 2023-05-23 10:26:56.283747 pyteseo-0.0.6/pyteseo/connections/coastlines.py
+-rw-r--r--   0        0        0     2535 2023-05-22 06:18:49.791063 pyteseo-0.0.6/pyteseo/connections/noaa_opendap.py
+-rw-r--r--   0        0        0    13416 2023-05-18 06:18:08.958963 pyteseo-0.0.6/pyteseo/data/substances/hns.xlsx
+-rw-r--r--   0        0        0     5208 2023-05-18 06:16:20.039757 pyteseo-0.0.6/pyteseo/data/substances/hns_units.xlsx
+-rw-r--r--   0        0        0     5849 2023-05-18 06:16:00.696375 pyteseo-0.0.6/pyteseo/data/substances/oil.xlsx
+-rw-r--r--   0        0        0     5079 2023-05-18 06:16:00.696375 pyteseo-0.0.6/pyteseo/data/substances/oil_units.xlsx
+-rw-r--r--   0        0        0     6521 2023-05-22 08:03:45.257543 pyteseo-0.0.6/pyteseo/defaults.py
+-rw-r--r--   0        0        0      194 2023-02-02 09:27:00.724058 pyteseo-0.0.6/pyteseo/export/__init__.py
+-rw-r--r--   0        0        0     4827 2023-04-19 07:13:56.452163 pyteseo-0.0.6/pyteseo/export/grids.py
+-rw-r--r--   0        0        0     3236 2023-04-14 11:07:51.005172 pyteseo-0.0.6/pyteseo/export/particles.py
+-rw-r--r--   0        0        0     1627 2023-02-10 07:53:13.427520 pyteseo-0.0.6/pyteseo/export/properties.py
+-rw-r--r--   0        0        0      193 2023-02-02 09:18:50.744064 pyteseo-0.0.6/pyteseo/io/__init__.py
+-rw-r--r--   0        0        0    16833 2023-05-17 10:24:34.307917 pyteseo-0.0.6/pyteseo/io/cfg.py
+-rw-r--r--   0        0        0     4499 2023-05-18 14:49:34.064244 pyteseo-0.0.6/pyteseo/io/coastline.py
+-rw-r--r--   0        0        0     6698 2023-05-22 06:57:42.067158 pyteseo-0.0.6/pyteseo/io/forcings.py
+-rw-r--r--   0        0        0     2608 2023-05-18 14:48:33.935729 pyteseo-0.0.6/pyteseo/io/grid.py
+-rw-r--r--   0        0        0     3448 2023-04-17 07:20:52.886042 pyteseo-0.0.6/pyteseo/io/hns_calib.py
+-rw-r--r--   0        0        0     6628 2023-04-17 09:25:25.739679 pyteseo-0.0.6/pyteseo/io/results.py
+-rw-r--r--   0        0        0     4797 2023-04-17 09:22:03.598328 pyteseo-0.0.6/pyteseo/io/run.py
+-rw-r--r--   0        0        0     1941 2023-05-22 07:08:05.418464 pyteseo-0.0.6/pyteseo/io/substances.py
+-rw-r--r--   0        0        0     1915 2023-05-10 15:18:33.918998 pyteseo-0.0.6/pyteseo/io/utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 08:24:20.888146 pyteseo-0.0.6/pyteseo/plot/__init__.py
+-rw-r--r--   0        0        0     6833 2023-05-15 10:29:06.337329 pyteseo-0.0.6/pyteseo/plot/animations.py
+-rw-r--r--   0        0        0     4883 2023-05-18 15:14:13.389991 pyteseo-0.0.6/pyteseo/plot/basics.py
+-rw-r--r--   0        0        0     2231 2023-05-18 15:19:31.369304 pyteseo-0.0.6/pyteseo/plot/figures.py
+-rw-r--r--   0        0        0     4277 2023-05-23 08:14:04.746173 pyteseo-0.0.6/pyteseo/services.py
+-rw-r--r--   0        0        0      309 2023-05-12 06:12:32.629928 pyteseo-0.0.6/pyteseo/tests/__init__.py
+-rw-r--r--   0        0        0     1080 2022-11-28 12:31:04.243939 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000000.txt
+-rw-r--r--   0        0        0     1440 2022-11-28 12:31:25.250905 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000005.txt
+-rw-r--r--   0        0        0     1320 2022-11-28 12:31:42.101870 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000010.txt
+-rw-r--r--   0        0        0     1440 2022-11-28 12:31:56.340847 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000015.txt
+-rw-r--r--   0        0        0     1800 2022-11-28 12:32:08.201821 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000020.txt
+-rw-r--r--   0        0        0     1920 2022-11-28 12:32:19.311799 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000025.txt
+-rw-r--r--   0        0        0     1800 2022-11-28 12:32:30.205778 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000030.txt
+-rw-r--r--   0        0        0     1920 2022-11-28 12:32:40.120760 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000035.txt
+-rw-r--r--   0        0        0     1920 2022-11-28 12:32:49.096757 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000040.txt
+-rw-r--r--   0        0        0     2040 2022-11-28 12:32:56.968763 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000045.txt
+-rw-r--r--   0        0        0     2280 2022-11-28 12:33:04.886785 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000050.txt
+-rw-r--r--   0        0        0     2640 2022-11-28 12:33:12.049766 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000055.txt
+-rw-r--r--   0        0        0     2640 2022-11-28 12:33:19.004754 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000060.txt
+-rw-r--r--   0        0        0     3240 2022-11-28 12:33:49.743762 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000065.txt
+-rw-r--r--   0        0        0     3840 2022-11-28 12:33:56.320750 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000070.txt
+-rw-r--r--   0        0        0     3960 2022-11-28 12:34:03.214770 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000075.txt
+-rw-r--r--   0        0        0     4440 2022-11-28 12:34:09.897757 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000080.txt
+-rw-r--r--   0        0        0     4920 2022-11-28 12:34:17.619757 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000085.txt
+-rw-r--r--   0        0        0     5280 2022-11-28 12:34:25.163765 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000090.txt
+-rw-r--r--   0        0        0     1080 2022-11-28 12:31:04.243939 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000000.txt
+-rw-r--r--   0        0        0     1440 2022-11-28 12:31:25.250905 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000005.txt
+-rw-r--r--   0        0        0     1320 2022-11-28 12:31:42.101870 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000010.txt
+-rw-r--r--   0        0        0     1440 2022-11-28 12:31:56.340847 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000015.txt
+-rw-r--r--   0        0        0     1800 2022-11-28 12:32:08.201821 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000020.txt
+-rw-r--r--   0        0        0     1920 2022-11-28 12:32:19.311799 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000025.txt
+-rw-r--r--   0        0        0     1800 2022-11-28 12:32:30.205778 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000030.txt
+-rw-r--r--   0        0        0     1920 2022-11-28 12:32:40.120760 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000035.txt
+-rw-r--r--   0        0        0     1920 2022-11-28 12:32:49.096757 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000040.txt
+-rw-r--r--   0        0        0     2040 2022-11-28 12:32:56.968763 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000045.txt
+-rw-r--r--   0        0        0     2280 2022-11-28 12:33:04.886785 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000050.txt
+-rw-r--r--   0        0        0     2640 2022-11-28 12:33:12.049766 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000055.txt
+-rw-r--r--   0        0        0     2640 2022-11-28 12:33:19.004754 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000060.txt
+-rw-r--r--   0        0        0     3240 2022-11-28 12:33:49.743762 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000065.txt
+-rw-r--r--   0        0        0     3840 2022-11-28 12:33:56.320750 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000070.txt
+-rw-r--r--   0        0        0     3960 2022-11-28 12:34:03.214770 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000075.txt
+-rw-r--r--   0        0        0     4440 2022-11-28 12:34:09.897757 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000080.txt
+-rw-r--r--   0        0        0     4920 2022-11-28 12:34:17.619757 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000085.txt
+-rw-r--r--   0        0        0     5280 2022-11-28 12:34:25.163765 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000090.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:31:04.219939 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000000.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:31:25.362903 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000005.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:31:42.232868 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000010.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:31:56.503846 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000015.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:32:08.296824 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000020.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:32:19.402804 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000025.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:32:30.379778 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000030.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:32:40.259760 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000035.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:32:49.222751 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000040.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:32:57.430761 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000045.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:33:04.996780 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000050.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:33:12.191766 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000055.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:33:19.144753 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000060.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:33:49.896767 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000065.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:33:56.794749 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000070.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:34:03.348770 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000075.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:34:10.956756 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000080.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:34:18.079761 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000085.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:34:25.335761 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000090.txt
+-rw-r--r--   0        0        0   121220 2022-11-28 12:59:56.013665 pyteseo-0.0.6/pyteseo/tests/data/cas1_properties_001.txt
+-rw-r--r--   0        0        0   121220 2022-11-28 12:59:56.013665 pyteseo-0.0.6/pyteseo/tests/data/cas1_properties_002.txt
+-rw-r--r--   0        0        0   574769 2023-01-13 08:20:28.115803 pyteseo-0.0.6/pyteseo/tests/data/coastline.dat
+-rw-r--r--   0        0        0   574787 2023-01-13 08:20:28.125803 pyteseo-0.0.6/pyteseo/tests/data/coastline_error_range.dat
+-rw-r--r--   0        0        0   574787 2023-01-13 08:20:28.125803 pyteseo-0.0.6/pyteseo/tests/data/coastline_othernanformat.dat
+-rw-r--r--   0        0        0   558324 2015-03-24 16:18:44.000000 pyteseo-0.0.6/pyteseo/tests/data/costa_poligono1.dat
+-rw-r--r--   0        0        0     3861 2015-03-24 16:18:44.000000 pyteseo-0.0.6/pyteseo/tests/data/costa_poligono2.dat
+-rw-r--r--   0        0        0    10412 2023-01-13 08:20:28.125803 pyteseo-0.0.6/pyteseo/tests/data/costa_poligono3.dat
+-rw-r--r--   0        0        0     2183 2023-01-13 08:20:28.125803 pyteseo-0.0.6/pyteseo/tests/data/costa_poligono4.dat
+-rw-r--r--   0        0        0    33889 2023-05-16 06:59:34.843214 pyteseo-0.0.6/pyteseo/tests/data/currents.nc
+-rw-r--r--   0        0        0      732 2022-11-14 07:58:35.871414 pyteseo-0.0.6/pyteseo/tests/data/currents_000h.txt
+-rw-r--r--   0        0        0      732 2022-11-14 07:58:35.950414 pyteseo-0.0.6/pyteseo/tests/data/currents_001h.txt
+-rw-r--r--   0        0        0      732 2022-11-14 07:58:36.019414 pyteseo-0.0.6/pyteseo/tests/data/currents_002h.txt
+-rw-r--r--   0        0        0      732 2022-11-14 07:58:36.125414 pyteseo-0.0.6/pyteseo/tests/data/currents_003h.txt
+-rw-r--r--   0        0        0     6679 2023-05-08 11:03:41.464391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1.cfg
+-rw-r--r--   0        0        0     1539 2023-05-08 11:03:41.464391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1.run
+-rw-r--r--   0        0        0      616 2023-05-08 11:03:41.464391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000060.txt
+-rw-r--r--   0        0        0      704 2023-05-08 11:03:41.464391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000120.txt
+-rw-r--r--   0        0        0      880 2023-05-08 11:03:41.464391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000180.txt
+-rw-r--r--   0        0        0      880 2023-05-08 11:03:41.464391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000240.txt
+-rw-r--r--   0        0        0      880 2023-05-08 11:03:41.464391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000300.txt
+-rw-r--r--   0        0        0     1232 2023-05-08 11:03:41.464391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000360.txt
+-rw-r--r--   0        0        0      968 2023-05-08 11:03:41.464391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000420.txt
+-rw-r--r--   0        0        0      616 2023-05-08 11:03:41.464391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000480.txt
+-rw-r--r--   0        0        0      176 2023-05-08 11:03:41.464391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000540.txt
+-rw-r--r--   0        0        0      880 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_002_000060.txt
+-rw-r--r--   0        0        0      176 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_002_000120.txt
+-rw-r--r--   0        0        0       99 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000000.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000060.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000120.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000180.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000240.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000300.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000360.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000420.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000480.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000540.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000600.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000660.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000720.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000780.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000840.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000900.txt
+-rw-r--r--   0        0        0     1173 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_properties_001.txt
+-rw-r--r--   0        0        0     1173 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_properties_002.txt
+-rw-r--r--   0        0        0  1129110 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/grid_coordinates.txt
+-rw-r--r--   0        0        0    63326 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa.dat
+-rw-r--r--   0        0        0    36930 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono1.dat
+-rw-r--r--   0        0        0      330 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono10.dat
+-rw-r--r--   0        0        0      390 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono11.dat
+-rw-r--r--   0        0        0      360 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono12.dat
+-rw-r--r--   0        0        0      390 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono13.dat
+-rw-r--r--   0        0        0      360 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono14.dat
+-rw-r--r--   0        0        0      270 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono15.dat
+-rw-r--r--   0        0        0      210 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono16.dat
+-rw-r--r--   0        0        0      240 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono17.dat
+-rw-r--r--   0        0        0      300 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono18.dat
+-rw-r--r--   0        0        0      240 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono19.dat
+-rw-r--r--   0        0        0    12810 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono2.dat
+-rw-r--r--   0        0        0      270 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono20.dat
+-rw-r--r--   0        0        0      270 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono21.dat
+-rw-r--r--   0        0        0      180 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono22.dat
+-rw-r--r--   0        0        0      210 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono23.dat
+-rw-r--r--   0        0        0      300 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono24.dat
+-rw-r--r--   0        0        0      210 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono25.dat
+-rw-r--r--   0        0        0      270 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono26.dat
+-rw-r--r--   0        0        0      240 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono27.dat
+-rw-r--r--   0        0        0      240 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono28.dat
+-rw-r--r--   0        0        0      330 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono29.dat
+-rw-r--r--   0        0        0     1590 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono3.dat
+-rw-r--r--   0        0        0      240 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono30.dat
+-rw-r--r--   0        0        0      270 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono31.dat
+-rw-r--r--   0        0        0      210 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono32.dat
+-rw-r--r--   0        0        0      210 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono33.dat
+-rw-r--r--   0        0        0      210 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono34.dat
+-rw-r--r--   0        0        0      120 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono35.dat
+-rw-r--r--   0        0        0      120 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono36.dat
+-rw-r--r--   0        0        0     1170 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono4.dat
+-rw-r--r--   0        0        0      510 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono5.dat
+-rw-r--r--   0        0        0      900 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono6.dat
+-rw-r--r--   0        0        0     1020 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono7.dat
+-rw-r--r--   0        0        0      510 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono8.dat
+-rw-r--r--   0        0        0      600 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono9.dat
+-rw-r--r--   0        0        0     8517 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_000h.txt
+-rw-r--r--   0        0        0     8502 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_001h.txt
+-rw-r--r--   0        0        0     8482 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_002h.txt
+-rw-r--r--   0        0        0     8466 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_003h.txt
+-rw-r--r--   0        0        0     8455 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_004h.txt
+-rw-r--r--   0        0        0     8446 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_005h.txt
+-rw-r--r--   0        0        0     8439 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_006h.txt
+-rw-r--r--   0        0        0     8430 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_007h.txt
+-rw-r--r--   0        0        0     8444 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_008h.txt
+-rw-r--r--   0        0        0     8461 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_009h.txt
+-rw-r--r--   0        0        0     8467 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_010h.txt
+-rw-r--r--   0        0        0     8475 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_011h.txt
+-rw-r--r--   0        0        0     8493 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_012h.txt
+-rw-r--r--   0        0        0     8498 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_013h.txt
+-rw-r--r--   0        0        0     8507 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_014h.txt
+-rw-r--r--   0        0        0     8506 2023-05-08 11:59:05.257117 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_015h.txt
+-rw-r--r--   0        0        0  1270777 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/grid.dat
+-rw-r--r--   0        0        0      288 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/lstcurr_UVW.pre
+-rw-r--r--   0        0        0        6 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/lstwaves.pre
+-rw-r--r--   0        0        0      195 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/lstwinds.pre
+-rw-r--r--   0        0        0     3967 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_000h.txt
+-rw-r--r--   0        0        0     3968 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_001h.txt
+-rw-r--r--   0        0        0     3965 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_002h.txt
+-rw-r--r--   0        0        0     3959 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_003h.txt
+-rw-r--r--   0        0        0     3957 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_004h.txt
+-rw-r--r--   0        0        0     3951 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_005h.txt
+-rw-r--r--   0        0        0     3947 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_006h.txt
+-rw-r--r--   0        0        0     3968 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_007h.txt
+-rw-r--r--   0        0        0     3958 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_008h.txt
+-rw-r--r--   0        0        0     3946 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_009h.txt
+-rw-r--r--   0        0        0     3937 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_010h.txt
+-rw-r--r--   0        0        0     3941 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_011h.txt
+-rw-r--r--   0        0        0     3943 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_012h.txt
+-rw-r--r--   0        0        0    58941 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/grids_001.nc
+-rw-r--r--   0        0        0    21981 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/grids_002.nc
+-rw-r--r--   0        0        0   527627 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/particles_001.csv
+-rw-r--r--   0        0        0   792030 2023-05-10 16:13:08.419088 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/particles_001.geojson
+-rw-r--r--   0        0        0   447138 2023-05-08 11:03:41.514392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/particles_002.csv
+-rw-r--r--   0        0        0   739116 2023-05-10 16:13:08.439088 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/particles_002.geojson
+-rw-r--r--   0        0        0      548 2023-05-08 11:03:41.514392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/properties_001.csv
+-rw-r--r--   0        0        0     1487 2023-05-10 16:13:08.429088 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/properties_001.json
+-rw-r--r--   0        0        0      554 2023-05-08 11:03:41.514392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/properties_002.csv
+-rw-r--r--   0        0        0     1503 2023-05-10 16:13:08.419088 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/properties_002.json
+-rw-r--r--   0        0        0  3177300 2015-03-24 16:18:44.000000 pyteseo-0.0.6/pyteseo/tests/data/grid.dat
+-rw-r--r--   0        0        0  1969957 2022-11-28 12:30:41.129982 pyteseo-0.0.6/pyteseo/tests/data/grid_coordinates.txt
+-rw-r--r--   0        0        0  3177492 2023-01-09 16:48:14.190649 pyteseo-0.0.6/pyteseo/tests/data/grid_error_var.dat
+-rw-r--r--   0        0        0     6725 2023-05-08 11:25:26.958241 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1.cfg
+-rw-r--r--   0        0        0     1539 2023-05-08 11:25:26.958241 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1.run
+-rw-r--r--   0        0        0      456 2023-05-08 11:25:27.208257 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_grid_001_000060.txt
+-rw-r--r--   0        0        0      760 2023-05-08 11:25:27.768293 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_grid_001_000120.txt
+-rw-r--r--   0        0        0      608 2023-05-08 11:25:28.078313 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_grid_001_000180.txt
+-rw-r--r--   0        0        0      456 2023-05-08 11:25:28.188320 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_grid_001_000240.txt
+-rw-r--r--   0        0        0      304 2023-05-08 11:25:27.208257 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_grid_002_000060.txt
+-rw-r--r--   0        0        0      760 2023-05-08 11:25:27.768293 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_grid_002_000120.txt
+-rw-r--r--   0        0        0       99 2023-05-08 11:25:27.018245 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000000.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:25:27.218258 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000060.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:25:27.768293 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000120.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:25:28.088313 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000180.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:25:28.188320 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000240.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:25:28.288326 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000300.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:25:28.388333 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000360.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:25:28.488339 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000420.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:25:28.588345 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000480.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:25:28.658350 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000540.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:25:28.688352 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000600.txt
+-rw-r--r--   0        0        0     5808 2023-05-08 11:25:28.688352 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_properties_001.txt
+-rw-r--r--   0        0        0     5808 2023-05-08 11:25:28.688352 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_properties_002.txt
+-rw-r--r--   0        0        0   748950 2023-05-08 11:25:27.018245 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/grid_coordinates.txt
+-rw-r--r--   0        0        0     3011 2023-05-10 16:13:08.419088 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/cas1_HNS.calib
+-rw-r--r--   0        0        0    63326 2023-05-08 10:31:26.468993 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa.dat
+-rw-r--r--   0        0        0    36930 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono1.dat
+-rw-r--r--   0        0        0      330 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono10.dat
+-rw-r--r--   0        0        0      390 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono11.dat
+-rw-r--r--   0        0        0      360 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono12.dat
+-rw-r--r--   0        0        0      390 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono13.dat
+-rw-r--r--   0        0        0      360 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono14.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono15.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono16.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono17.dat
+-rw-r--r--   0        0        0      300 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono18.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono19.dat
+-rw-r--r--   0        0        0    12810 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono2.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono20.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono21.dat
+-rw-r--r--   0        0        0      180 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono22.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono23.dat
+-rw-r--r--   0        0        0      300 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono24.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono25.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono26.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono27.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono28.dat
+-rw-r--r--   0        0        0      330 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono29.dat
+-rw-r--r--   0        0        0     1590 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono3.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono30.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono31.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono32.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono33.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono34.dat
+-rw-r--r--   0        0        0      120 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono35.dat
+-rw-r--r--   0        0        0      120 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono36.dat
+-rw-r--r--   0        0        0     1170 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono4.dat
+-rw-r--r--   0        0        0      510 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono5.dat
+-rw-r--r--   0        0        0      900 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono6.dat
+-rw-r--r--   0        0        0     1020 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono7.dat
+-rw-r--r--   0        0        0      510 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono8.dat
+-rw-r--r--   0        0        0      600 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono9.dat
+-rw-r--r--   0        0        0     5829 2023-05-08 11:25:13.507384 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_000h.txt
+-rw-r--r--   0        0        0     5820 2023-05-08 11:25:13.507384 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_001h.txt
+-rw-r--r--   0        0        0     5805 2023-05-08 11:25:13.517384 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_002h.txt
+-rw-r--r--   0        0        0     5793 2023-05-08 11:25:13.517384 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_003h.txt
+-rw-r--r--   0        0        0     5785 2023-05-08 11:25:13.517384 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_004h.txt
+-rw-r--r--   0        0        0     5777 2023-05-08 11:25:13.527385 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_005h.txt
+-rw-r--r--   0        0        0     5773 2023-05-08 11:25:13.527385 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_006h.txt
+-rw-r--r--   0        0        0     5764 2023-05-08 11:25:13.527385 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_007h.txt
+-rw-r--r--   0        0        0     5771 2023-05-08 11:25:13.527385 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_008h.txt
+-rw-r--r--   0        0        0     5780 2023-05-08 11:25:13.527385 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_009h.txt
+-rw-r--r--   0        0        0     5787 2023-05-08 11:25:13.537386 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_010h.txt
+-rw-r--r--   0        0        0   840169 2023-05-08 10:31:25.578990 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/grid.dat
+-rw-r--r--   0        0        0      198 2023-05-08 11:25:13.527385 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/lstcurr_UVW.pre
+-rw-r--r--   0        0        0        6 2023-05-08 11:25:26.928239 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/lstwaves.pre
+-rw-r--r--   0        0        0      165 2023-05-08 11:25:26.878236 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/lstwinds.pre
+-rw-r--r--   0        0        0     3967 2023-05-08 11:25:26.848234 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_000h.txt
+-rw-r--r--   0        0        0     3968 2023-05-08 11:25:26.858235 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_001h.txt
+-rw-r--r--   0        0        0     3965 2023-05-08 11:25:26.858235 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_002h.txt
+-rw-r--r--   0        0        0     3959 2023-05-08 11:25:26.858235 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_003h.txt
+-rw-r--r--   0        0        0     3957 2023-05-08 11:25:26.868235 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_004h.txt
+-rw-r--r--   0        0        0     3951 2023-05-08 11:25:26.868235 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_005h.txt
+-rw-r--r--   0        0        0     3947 2023-05-08 11:25:26.868235 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_006h.txt
+-rw-r--r--   0        0        0     3968 2023-05-08 11:25:26.868235 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_007h.txt
+-rw-r--r--   0        0        0     3958 2023-05-08 11:25:26.878236 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_008h.txt
+-rw-r--r--   0        0        0     3946 2023-05-08 11:25:26.878236 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_009h.txt
+-rw-r--r--   0        0        0     3937 2023-05-08 11:25:26.878236 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_010h.txt
+-rw-r--r--   0        0        0    35005 2023-05-08 11:25:29.558407 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/grids_001.nc
+-rw-r--r--   0        0        0    24093 2023-05-08 11:25:29.568408 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/grids_002.nc
+-rw-r--r--   0        0        0   348805 2023-05-08 11:25:29.208385 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/particles_001.csv
+-rw-r--r--   0        0        0   527846 2023-05-10 16:13:08.429088 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/particles_001.geojson
+-rw-r--r--   0        0        0   302691 2023-05-08 11:25:29.218386 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/particles_002.csv
+-rw-r--r--   0        0        0   497813 2023-05-10 16:13:08.429088 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/particles_002.geojson
+-rw-r--r--   0        0        0     2188 2023-05-08 11:25:29.238387 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/properties_001.csv
+-rw-r--r--   0        0        0     7169 2023-05-10 16:13:08.429088 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/properties_001.json
+-rw-r--r--   0        0        0     2251 2023-05-08 11:25:29.238387 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/properties_002.csv
+-rw-r--r--   0        0        0     7242 2023-05-10 16:13:08.429088 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/properties_002.json
+-rw-r--r--   0        0        0    63326 2023-05-08 10:31:26.468993 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa.dat
+-rw-r--r--   0        0        0    36930 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono1.dat
+-rw-r--r--   0        0        0      330 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono10.dat
+-rw-r--r--   0        0        0      390 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono11.dat
+-rw-r--r--   0        0        0      360 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono12.dat
+-rw-r--r--   0        0        0      390 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono13.dat
+-rw-r--r--   0        0        0      360 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono14.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono15.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono16.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono17.dat
+-rw-r--r--   0        0        0      300 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono18.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono19.dat
+-rw-r--r--   0        0        0    12810 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono2.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono20.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono21.dat
+-rw-r--r--   0        0        0      180 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono22.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono23.dat
+-rw-r--r--   0        0        0      300 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono24.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono25.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono26.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono27.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono28.dat
+-rw-r--r--   0        0        0      330 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono29.dat
+-rw-r--r--   0        0        0     1590 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono3.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono30.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono31.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono32.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono33.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono34.dat
+-rw-r--r--   0        0        0      120 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono35.dat
+-rw-r--r--   0        0        0      120 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono36.dat
+-rw-r--r--   0        0        0     1170 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono4.dat
+-rw-r--r--   0        0        0      510 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono5.dat
+-rw-r--r--   0        0        0      900 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono6.dat
+-rw-r--r--   0        0        0     1020 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono7.dat
+-rw-r--r--   0        0        0      510 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono8.dat
+-rw-r--r--   0        0        0      600 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono9.dat
+-rw-r--r--   0        0        0   840169 2023-05-08 10:31:25.578990 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/grid.dat
+-rw-r--r--   0        0        0   777758 2023-05-08 10:31:27.838997 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/ibiza_domain.png
+-rw-r--r--   0        0        0       72 2023-01-09 16:55:02.280651 pyteseo-0.0.6/pyteseo/tests/data/lstcurr.pre
+-rw-r--r--   0        0        0       36 2023-01-27 13:50:37.678084 pyteseo-0.0.6/pyteseo/tests/data/lstcurr_UVW_cte.pre
+-rw-r--r--   0        0        0       45 2023-05-17 11:10:20.837289 pyteseo-0.0.6/pyteseo/tests/data/lstcurr_depthavg.pre
+-rw-r--r--   0        0        0       60 2023-01-30 12:26:16.443318 pyteseo-0.0.6/pyteseo/tests/data/lstwaves.pre
+-rw-r--r--   0        0        0       32 2023-01-31 09:57:32.253738 pyteseo-0.0.6/pyteseo/tests/data/lstwaves_cte.pre
+-rw-r--r--   0        0        0       60 2023-01-13 08:20:28.125803 pyteseo-0.0.6/pyteseo/tests/data/lstwinds.pre
+-rw-r--r--   0        0        0       36 2023-01-31 09:57:32.253738 pyteseo-0.0.6/pyteseo/tests/data/lstwinds_cte.pre
+-rw-r--r--   0        0        0     6701 2023-05-08 11:24:40.005250 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1.cfg
+-rw-r--r--   0        0        0     1539 2023-05-08 11:24:40.005250 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1.run
+-rw-r--r--   0        0        0      357 2023-05-08 11:24:40.275267 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_grid_001_000060.txt
+-rw-r--r--   0        0        0      595 2023-05-08 11:24:40.825302 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_grid_001_000120.txt
+-rw-r--r--   0        0        0      595 2023-05-08 11:24:41.105320 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_grid_001_000180.txt
+-rw-r--r--   0        0        0      357 2023-05-08 11:24:41.205326 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_grid_001_000240.txt
+-rw-r--r--   0        0        0      357 2023-05-08 11:24:40.275267 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_grid_002_000060.txt
+-rw-r--r--   0        0        0      476 2023-05-08 11:24:40.825302 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_grid_002_000120.txt
+-rw-r--r--   0        0        0       99 2023-05-08 11:24:40.065253 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000000.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:24:40.275267 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000060.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:24:40.825302 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000120.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:24:41.105320 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000180.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:24:41.205326 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000240.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:24:41.305333 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000300.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:24:41.405339 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000360.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:24:41.515346 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000420.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:24:41.615352 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000480.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:24:41.685357 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000540.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:24:41.715359 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000600.txt
+-rw-r--r--   0        0        0     5004 2023-05-08 11:24:41.715359 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_properties_001.txt
+-rw-r--r--   0        0        0     5004 2023-05-08 11:24:41.715359 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_properties_002.txt
+-rw-r--r--   0        0        0   748950 2023-05-08 11:24:40.065253 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/grid_coordinates.txt
+-rw-r--r--   0        0        0    63326 2023-05-08 10:31:26.468993 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa.dat
+-rw-r--r--   0        0        0    36930 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono1.dat
+-rw-r--r--   0        0        0      330 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono10.dat
+-rw-r--r--   0        0        0      390 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono11.dat
+-rw-r--r--   0        0        0      360 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono12.dat
+-rw-r--r--   0        0        0      390 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono13.dat
+-rw-r--r--   0        0        0      360 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono14.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono15.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono16.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono17.dat
+-rw-r--r--   0        0        0      300 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono18.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono19.dat
+-rw-r--r--   0        0        0    12810 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono2.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono20.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono21.dat
+-rw-r--r--   0        0        0      180 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono22.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono23.dat
+-rw-r--r--   0        0        0      300 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono24.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono25.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono26.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono27.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono28.dat
+-rw-r--r--   0        0        0      330 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono29.dat
+-rw-r--r--   0        0        0     1590 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono3.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono30.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono31.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono32.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono33.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono34.dat
+-rw-r--r--   0        0        0      120 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono35.dat
+-rw-r--r--   0        0        0      120 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono36.dat
+-rw-r--r--   0        0        0     1170 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono4.dat
+-rw-r--r--   0        0        0      510 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono5.dat
+-rw-r--r--   0        0        0      900 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono6.dat
+-rw-r--r--   0        0        0     1020 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono7.dat
+-rw-r--r--   0        0        0      510 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono8.dat
+-rw-r--r--   0        0        0      600 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono9.dat
+-rw-r--r--   0        0        0     5829 2023-05-08 11:23:49.021999 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_000h.txt
+-rw-r--r--   0        0        0     5820 2023-05-08 11:23:49.031999 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_001h.txt
+-rw-r--r--   0        0        0     5805 2023-05-08 11:23:49.031999 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_002h.txt
+-rw-r--r--   0        0        0     5793 2023-05-08 11:23:49.042000 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_003h.txt
+-rw-r--r--   0        0        0     5785 2023-05-08 11:23:49.042000 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_004h.txt
+-rw-r--r--   0        0        0     5777 2023-05-08 11:23:49.042000 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_005h.txt
+-rw-r--r--   0        0        0     5773 2023-05-08 11:23:49.042000 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_006h.txt
+-rw-r--r--   0        0        0     5764 2023-05-08 11:23:49.042000 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_007h.txt
+-rw-r--r--   0        0        0     5771 2023-05-08 11:23:49.052000 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_008h.txt
+-rw-r--r--   0        0        0     5780 2023-05-08 11:23:49.052000 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_009h.txt
+-rw-r--r--   0        0        0     5787 2023-05-08 11:23:49.052000 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_010h.txt
+-rw-r--r--   0        0        0   840169 2023-05-08 10:31:25.578990 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/grid.dat
+-rw-r--r--   0        0        0      198 2023-05-08 11:23:49.052000 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/lstcurr_UVW.pre
+-rw-r--r--   0        0        0        6 2023-05-08 11:24:39.975248 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/lstwaves.pre
+-rw-r--r--   0        0        0      165 2023-05-08 11:24:39.925244 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/lstwinds.pre
+-rw-r--r--   0        0        0     3967 2023-05-08 11:24:39.895243 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_000h.txt
+-rw-r--r--   0        0        0     3968 2023-05-08 11:24:39.905243 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_001h.txt
+-rw-r--r--   0        0        0     3965 2023-05-08 11:24:39.905243 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_002h.txt
+-rw-r--r--   0        0        0     3959 2023-05-08 11:24:39.905243 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_003h.txt
+-rw-r--r--   0        0        0     3957 2023-05-08 11:24:39.915244 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_004h.txt
+-rw-r--r--   0        0        0     3951 2023-05-08 11:24:39.915244 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_005h.txt
+-rw-r--r--   0        0        0     3947 2023-05-08 11:24:39.915244 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_006h.txt
+-rw-r--r--   0        0        0     3968 2023-05-08 11:24:39.915244 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_007h.txt
+-rw-r--r--   0        0        0     3958 2023-05-08 11:24:39.915244 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_008h.txt
+-rw-r--r--   0        0        0     3946 2023-05-08 11:24:39.925244 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_009h.txt
+-rw-r--r--   0        0        0     3937 2023-05-08 11:24:39.925244 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_010h.txt
+-rw-r--r--   0        0        0    31485 2023-05-08 11:24:42.585414 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/grids_001.nc
+-rw-r--r--   0        0        0    23229 2023-05-08 11:24:42.595415 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/grids_002.nc
+-rw-r--r--   0        0        0   348848 2023-05-08 11:24:42.235392 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/particles_001.csv
+-rw-r--r--   0        0        0   527956 2023-05-10 16:13:08.419088 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/particles_001.geojson
+-rw-r--r--   0        0        0   302657 2023-05-08 11:24:42.245392 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/particles_002.csv
+-rw-r--r--   0        0        0   497752 2023-05-10 16:13:08.439088 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/particles_002.geojson
+-rw-r--r--   0        0        0     1853 2023-05-08 11:24:42.265394 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/properties_001.csv
+-rw-r--r--   0        0        0     6125 2023-05-10 16:13:08.429088 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/properties_001.json
+-rw-r--r--   0        0        0     1858 2023-05-08 11:24:42.265394 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/properties_002.csv
+-rw-r--r--   0        0        0     6139 2023-05-10 16:13:08.419088 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/properties_002.json
+-rw-r--r--   0        0        0        6 2023-05-10 16:13:08.419088 pyteseo-0.0.6/pyteseo/tests/data/shapefile_cantabria/Cantabria.cpg
+-rw-r--r--   0        0        0      382 2023-05-09 14:10:49.121228 pyteseo-0.0.6/pyteseo/tests/data/shapefile_cantabria/Cantabria.dbf
+-rw-r--r--   0        0        0      413 2023-05-10 16:13:08.429088 pyteseo-0.0.6/pyteseo/tests/data/shapefile_cantabria/Cantabria.prj
+-rw-r--r--   0        0        0      132 2023-05-09 14:10:49.121228 pyteseo-0.0.6/pyteseo/tests/data/shapefile_cantabria/Cantabria.sbn
+-rw-r--r--   0        0        0      116 2023-05-09 14:10:49.131229 pyteseo-0.0.6/pyteseo/tests/data/shapefile_cantabria/Cantabria.sbx
+-rw-r--r--   0        0        0   259168 2023-05-09 14:10:49.131229 pyteseo-0.0.6/pyteseo/tests/data/shapefile_cantabria/Cantabria.shp
+-rw-r--r--   0        0        0    10465 2023-05-09 14:10:49.151231 pyteseo-0.0.6/pyteseo/tests/data/shapefile_cantabria/Cantabria.shp.xml
+-rw-r--r--   0        0        0      108 2023-05-09 14:10:49.151231 pyteseo-0.0.6/pyteseo/tests/data/shapefile_cantabria/Cantabria.shx
+-rw-r--r--   0        0        0      456 2023-01-30 12:28:00.313319 pyteseo-0.0.6/pyteseo/tests/data/waves_000h.txt
+-rw-r--r--   0        0        0      480 2023-01-30 12:28:28.243319 pyteseo-0.0.6/pyteseo/tests/data/waves_001h.txt
+-rw-r--r--   0        0        0      480 2023-01-30 12:28:40.053319 pyteseo-0.0.6/pyteseo/tests/data/waves_002h.txt
+-rw-r--r--   0        0        0      516 2023-01-31 09:57:32.263738 pyteseo-0.0.6/pyteseo/tests/data/waves_003h.txt
+-rw-r--r--   0        0        0    25121 2023-05-16 06:59:43.223472 pyteseo-0.0.6/pyteseo/tests/data/winds.nc
+-rw-r--r--   0        0        0      732 2022-11-14 07:58:35.871414 pyteseo-0.0.6/pyteseo/tests/data/winds_000h.txt
+-rw-r--r--   0        0        0      732 2022-11-14 07:58:35.950414 pyteseo-0.0.6/pyteseo/tests/data/winds_001h.txt
+-rw-r--r--   0        0        0      732 2022-11-14 07:58:36.019414 pyteseo-0.0.6/pyteseo/tests/data/winds_002h.txt
+-rw-r--r--   0        0        0      732 2022-11-14 07:58:36.125414 pyteseo-0.0.6/pyteseo/tests/data/winds_003h.txt
+-rw-r--r--   0        0        0        0 2023-02-10 07:53:13.427520 pyteseo-0.0.6/pyteseo/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1585 2023-05-22 06:19:42.815869 pyteseo-0.0.6/pyteseo/tests/integration/test_cmems.py
+-rw-r--r--   0        0        0     1025 2023-05-23 11:05:59.240771 pyteseo-0.0.6/pyteseo/tests/integration/test_create_domain.py
+-rw-r--r--   0        0        0      974 2023-05-22 06:39:28.861207 pyteseo-0.0.6/pyteseo/tests/integration/test_noaa_gfs.py
+-rw-r--r--   0        0        0     9785 2023-05-18 10:41:21.720535 pyteseo-0.0.6/pyteseo/tests/integration/test_simulation_cmems.py
+-rw-r--r--   0        0        0     9609 2023-05-18 10:41:21.720535 pyteseo-0.0.6/pyteseo/tests/integration/test_simulation_cte_forcing.py
+-rw-r--r--   0        0        0        0 2023-02-10 07:53:13.427520 pyteseo-0.0.6/pyteseo/tests/unit/__init__.py
+-rw-r--r--   0        0        0     4635 2023-05-18 10:41:21.720535 pyteseo-0.0.6/pyteseo/tests/unit/test_cfg.py
+-rw-r--r--   0        0        0     6183 2023-05-22 08:08:53.659923 pyteseo-0.0.6/pyteseo/tests/unit/test_clasess.py
+-rw-r--r--   0        0        0     2879 2023-05-10 16:02:05.526185 pyteseo-0.0.6/pyteseo/tests/unit/test_export.py
+-rw-r--r--   0        0        0     3286 2023-05-10 13:10:41.515296 pyteseo-0.0.6/pyteseo/tests/unit/test_io_coastline.py
+-rw-r--r--   0        0        0     3589 2023-05-17 14:25:17.630330 pyteseo-0.0.6/pyteseo/tests/unit/test_io_forcings.py
+-rw-r--r--   0        0        0     2552 2023-05-10 15:10:22.789296 pyteseo-0.0.6/pyteseo/tests/unit/test_io_grid.py
+-rw-r--r--   0        0        0     1685 2023-05-10 16:00:06.143520 pyteseo-0.0.6/pyteseo/tests/unit/test_io_results.py
+-rw-r--r--   0        0        0     1892 2023-05-23 08:06:52.405460 pyteseo-0.0.6/pyteseo/tests/unit/test_plot.py
+-rw-r--r--   0        0        0      898 2023-05-22 13:51:54.858831 pyteseo-0.0.6/pyteseo/tests/unit/test_services.py
+-rw-r--r--   0        0        0      946 2023-05-22 06:31:48.943904 pyteseo-0.0.6/pyteseo/tests/unit/test_substances.py
+-rw-r--r--   0        0        0    14063 2023-05-22 08:25:22.029789 pyteseo-0.0.6/pyteseo/wrapper.py
+-rw-r--r--   0        0        0     6073 1970-01-01 00:00:00.000000 pyteseo-0.0.6/PKG-INFO
```

### Comparing `pyteseo-0.0.5/CHANGELOG.md` & `pyteseo-0.0.6/CHANGELOG.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,32 @@
 # Changelog
 
+## v0.0.6 - ??/??/2023
+### Added:
+1) Classes for forcings
+2) Create null forcings
+3) Create TeseoWrapper class
+4) Create cfg and run files
+5) Create *_hns.calib file
+6) First integration tests runing teseo v1.2.8 (drifter, oil and hns) with cte forcings with and without coastline
+7) Add general attributes to netcdf results
+8) Run simulations with 2d forcings (winds and currents)
+9) Add plot package with basic plots, figures and animations
+### Changed:
+1) modules are getting too big, I split structure into subpackages
+2) generalize i/o of forcings to spatially cte or 2d
+3) downgrade netcdf version to hotfix netcdf library bug introduced in new versions
+4) notebooks will not be a priority from now on
+### Fixed:
+1) notebooks to run documentation ci
+2) access CMEMS from the notebooks (github secret)
+3) Tests in github actions (downgrade netcdf. netcdf problem, not us!)
+<br/><br/>
+
+
 ## v0.0.5 - 19/01/2023
 ### Added:
 1) read results (particles, properties, and grids)
 2) add mod calculation to read_currents and read_winds
 3) notebook 02
 4) add py3.11 to test workflow
 5) exclude windows w/ py3.7
```

### Comparing `pyteseo-0.0.5/LICENSE.md` & `pyteseo-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/README.md` & `pyteseo-0.0.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-## :warning: Package under development!
-## :soon: First usable version (v1.0.0) will be released soon!
+## Package under development!
 ---
 
 <p align="center">
 <img align="center" width="600" src="https://ihcantabria.github.io/pyteseo/_images/pyTESEO_logo.png">
 </p>
 
 [![pypi](https://img.shields.io/pypi/v/pyteseo)](https://pypi.org/project/pyteseo/)
@@ -22,39 +21,42 @@
 **pyTESEO** is a python package developed by [IHCantabria](https://ihcantabria.com/en/) to simplify and facilitate the setup and processing of [TESEO](https://ihcantabria.com/en/specialized-software/teseo/) simulations *(TESEO is a lagrangian numerical model also developed by IHCantabria.)*
 
 
 ---
 
 ## :computer: Installation
 
-|                         | Linux  | MacOS  | Windows|
-|:-----------------------:|:------:|:------:|:------:|
-| Required python version | >= 3.7 | >= 3.7 | >= 3.8 |
+1 - Install the python library using pip:
 
-
-* From `github` repository using `pip`:
 ```bash
-pip install git+https://github.com/IHCantabria/pyteseo
-# To install extra dev dependencies: pip install git+https://github.com/IHCantabria/pyteseo[dev]
-# Using editable mode: pip install -e git+https://github.com/IHCantabria/pyteseo[dev]
+# From pypi repository
+pip install pyteseo
 
+# Or directly from github repository
+pip install git+https://github.com/IHCantabria/pyteseo
 ```
 
-:warning: `UNDER DEVELOPMENT` :construction: - * From `pypi` using `pip`:
+2 - Install TESEO model binary (**Not available yet!**):
+- Get access to the binary: https://github.com/IHCantabria/TESEO/blob/main/bin
+- Set up environment variable "TESEO_PATH" with the path to the model executable. You can use the command following CLI command after activate the python environement (python-dotenv library)
+
+    ```bash
+        dotenv set TESEO_PATH /path/to/teseo_executable
+    ```
+3 - Opendap connection to some [CMEMS products](https://data.marine.copernicus.eu/products) is available at the library `pyteseo/connections/cmems.py` but needs authetication through the following environement variables:
 ```bash
-pip install pyteseo
+dotenv set CMEMS_username your_username_at_CMEMS
 ```
-:warning: `UNDER DEVELOPMENT` :construction: - * From `conda-forge` using `conda`:
 ```bash
-conda install -c conda-forge pyteseo
+dotenv set CMEMS_password your_password_at_CMEMS
 ```
 
 ---
 
-## :heavy_check_mark: Testing & Coverage
+## :heavy_check_mark: Tests
 Tests are located in `pyteseo/tests/` and data required for tests are located in `pyteseo/tests/data/`.
 Tests have been developed using [pytest](https://docs.pytest.org/).
 
 Run tests to verify your package installation:
 ```bash
 pyteseo-test        # Run tests and prompt pytest-report
 ```
@@ -64,36 +66,29 @@
 # Commands should be executed from the root directory of the repo
 
 coverage run        # For run tests and generate ".coverage" file
 coverage report     # For prompt results from ".coverage" file
 coverage html       # For generate html report on "htmlcov" folder
 ```
 
-
 ---
 
 ## :recycle: Continuous integration (CI)
 
-
 * Build and deploy documentation on Github Pages in [.github/workflows/docs.yml](.github/workflows/docs.yml)
 * Install and test package in diferent environments in [.github/workflows/tests.yml](.github/workflows/tests.yml)
 * Precommit hooks for formats and linting in [.pre-commit-config.yaml](.pre-commit-config.yaml)
 
 *For Linux, Windows, MacOS and compatible python versions defined in installation section*
 
 ---
 
 ## :books: Documentation
 
-Comprenhensive documentation is developed and mantained at https://ihcantabria.github.io/pyteseo
-
-Documentation of all the package, usage and examples based on mockup input data are provided in [Jupyter Notebooks](https://jupyter.org/) format and ready to be used under [Google Colab](https://colab.research.google.com/) online platform.
-
-
-![pyteseo_doc](docs/_static/doc_snapshoot.png)
+Documentation is available at https://ihcantabria.github.io/pyteseo
 
 ---
 
 ## :copyright: Credits
 Developed and maintained by :man_technologist: [German Aragon](https://github.com/aragong) @ :office: [IHCantabria](https://github.com/IHCantabria).
 
 ---
```

### Comparing `pyteseo-0.0.5/docs/Makefile` & `pyteseo-0.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/docs/_static/TESEO_logo.png` & `pyteseo-0.0.6/docs/_static/TESEO_logo.png`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/docs/_static/doc_snapshoot.png` & `pyteseo-0.0.6/docs/_static/doc_snapshoot.png`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/docs/_static/pyTESEO_logo.png` & `pyteseo-0.0.6/docs/_static/pyTESEO_logo.png`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/docs/conf.py` & `pyteseo-0.0.6/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,27 @@
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 from pyteseo.__init__ import __version__
 
+
 project = "pyTESEO"
 copyright = "2022, Germán Aragón Caminero"
 author = "Germán Aragón Caminero"
-release = __version__
+version = release = __version__
+
+html_context = {
+    "display_github": True,  # Integrate GitHub
+    "github_user": "ihcantabria",  # Username
+    "github_repo": "pyteseo",  # Repo name
+    "github_version": "main",  # Version
+    "conf_py_path": "/docs/",
+}
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.napoleon",
@@ -28,14 +37,15 @@
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = "sphinx_rtd_theme"
 html_theme_options = {
     "display_version": True,
+    "style_external_links": False,
 }
 # html_theme = 'furo'
 # html_theme = 'sphinx_book_theme'
 
 html_static_path = ["_static"]
 html_logo = "_static/pyTESEO_logo.png"
 html_title = " v" + release
```

### Comparing `pyteseo-0.0.5/docs/get-started.md` & `pyteseo-0.0.6/docs/get-started.md`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/docs/index.md` & `pyteseo-0.0.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/docs/make.bat` & `pyteseo-0.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/docs/notebooks/02_read_forcings.ipynb` & `pyteseo-0.0.6/docs/notebooks/02_read_forcings.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9907752029814119%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(4, '- If you are using this notebook in your own local "*

 * *            'machine you need to install the library from the local repo `pip install .` or pypi '*

 * *            "`pip install pyteseo`.')], delete: [4]}}, 3: {'execution_count': 1}, 5: "*

 * *            "{'execution_count': 2}, 7: {'execution_count': 3, 'outputs': [OrderedDict([('name', "*

 * *            "'stdout'), ('output_type', 'stream'), ('text', ['\\n', 'WARNING - .env file has not "*

 * *            "been loaded!\\n'])] […]*

```diff
@@ -20,20 +20,20 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Install pyTESEO\n",
                 "- If you are running this notebook from `Google colab` uncomment and run `!pip install pyteseo && pyteseo-tests` in the cell below. \n",
                 "Doing this you will install `pyteseo` from `pypi` repository and run `pyteseo-tests` to check the installation (all tests have to succeed).\n",
                 "\n",
-                "- If you are using this notebook in your own local environement you should have installed all the requiered dependencies defined in `pyproject.toml` or `environment.yml`."
+                "- If you are using this notebook in your own local machine you need to install the library from the local repo `pip install .` or pypi `pip install pyteseo`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# !pip install pyteseo && pyteseo-tests"
             ]
         },
         {
@@ -42,15 +42,15 @@
             "metadata": {},
             "source": [
                 "## Read TESEO's forcings files (currents and winds) and plot them.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import warnings\n",
                 "\n",
                 "warnings.simplefilter(action=\"ignore\")"
             ]
@@ -61,37 +61,46 @@
             "metadata": {},
             "source": [
                 "1. Define Paths"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 3,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\n",
+                        "WARNING - .env file has not been loaded!\n"
+                    ]
+                }
+            ],
             "source": [
                 "from pathlib import Path\n",
                 "import pyteseo.tests as tests_\n",
                 "\n",
                 "data_path = Path(tests_.__file__).parent / \"data\"\n",
-                "lstcurr_path = data_path / \"lstcurr_UVW.pre\"\n",
+                "lstcurr_path = data_path / \"lstcurr.pre\"\n",
                 "lstwinds_path = data_path / \"lstwinds.pre\""
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "2. Read bathymetry and coastline from TESEO's format files"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -112,115 +121,114 @@
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>time</th>\n",
                             "      <th>lon</th>\n",
                             "      <th>lat</th>\n",
                             "      <th>u</th>\n",
                             "      <th>v</th>\n",
-                            "      <th>mod</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>0.0</td>\n",
                             "      <td>9.618706</td>\n",
                             "      <td>43.98785</td>\n",
                             "      <td>-3.765736</td>\n",
                             "      <td>0.509148</td>\n",
-                            "      <td>3.8</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>0.0</td>\n",
                             "      <td>9.618706</td>\n",
                             "      <td>44.11285</td>\n",
                             "      <td>-3.765736</td>\n",
                             "      <td>0.509148</td>\n",
-                            "      <td>3.8</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>0.0</td>\n",
                             "      <td>9.618706</td>\n",
                             "      <td>44.23785</td>\n",
                             "      <td>-3.765736</td>\n",
                             "      <td>0.509148</td>\n",
-                            "      <td>3.8</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>0.0</td>\n",
                             "      <td>9.743706</td>\n",
                             "      <td>43.98785</td>\n",
                             "      <td>-3.765736</td>\n",
                             "      <td>0.509148</td>\n",
-                            "      <td>3.8</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
                             "      <td>0.0</td>\n",
                             "      <td>9.743706</td>\n",
                             "      <td>44.11285</td>\n",
                             "      <td>-3.765736</td>\n",
                             "      <td>0.509148</td>\n",
-                            "      <td>3.8</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "   time       lon       lat         u         v  mod\n",
-                            "0   0.0  9.618706  43.98785 -3.765736  0.509148  3.8\n",
-                            "1   0.0  9.618706  44.11285 -3.765736  0.509148  3.8\n",
-                            "2   0.0  9.618706  44.23785 -3.765736  0.509148  3.8\n",
-                            "3   0.0  9.743706  43.98785 -3.765736  0.509148  3.8\n",
-                            "4   0.0  9.743706  44.11285 -3.765736  0.509148  3.8"
+                            "   time       lon       lat         u         v\n",
+                            "0   0.0  9.618706  43.98785 -3.765736  0.509148\n",
+                            "1   0.0  9.618706  44.11285 -3.765736  0.509148\n",
+                            "2   0.0  9.618706  44.23785 -3.765736  0.509148\n",
+                            "3   0.0  9.743706  43.98785 -3.765736  0.509148\n",
+                            "4   0.0  9.743706  44.11285 -3.765736  0.509148"
                         ]
                     },
-                    "execution_count": 23,
+                    "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "from pyteseo.io import read_currents, read_winds\n",
+                "from pyteseo.io.forcings import read_forcing\n",
                 "\n",
-                "currents_df, n_files, n_nodes = read_currents(lstcurr_path)\n",
-                "winds_df, n_files, n_nodes = read_winds(lstwinds_path)\n",
+                "currents_df = read_forcing(lstcurr_path, forcing_type=\"currents\")\n",
+                "winds_df = read_forcing(lstwinds_path, forcing_type=\"winds\")\n",
                 "winds_df.head(5)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "3. Plot velocity fields"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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HB0dS1sSERERVSClCjFPnjzBwIEDsXLlStja2uabn5CQgJEjRyIsLAxKpbLY9bVo0QLz589H//79oVKpim1PREREVKoQM2LECAQGBsLf3z/fvJycHAQFBWHixIlo0EB3Z8inp6cjNTVV40FEREQVh9Yn9oaHhyMuLg6xsQX/ONncuXOhUCgwevToMhdXlNDQUMyYMUOnf4OIiIgMl1Z7YuLj4zFmzBhs3LgRZmZm+eYfP34cixYtwrp163R+iV9ISAhSUlLUj/j4eJ3+PSIiIjIsWoWY48ePIykpCc2aNYNCoYBCoUBUVBQWL14MhUKByMhIJCUloUaNGur5N2/exPjx4+Hu7v5KC1epVLC2ttZ4EBERUcWh1eGkTp064cyZMxrTgoODUa9ePUyePBlOTk4ICAjQmB8QEICgoCAEBweXvVoiIiKi/6dViLGyskLDhg01pllYWMDe3l493d7eXmO+UqmEo6MjPD091dMGDRoEFxcXhIaGAgAyMjJw/vx59f8nJCTg5MmTsLS0RO3atUFERESUl17u2Hvr1i2YmPx7JCsxMRFNmzZVP1+wYAEWLFgAX19fREZG6qFCIiIiMnT87SQiIiLSm7Jsv8v0swNERERE+sIQQ0RERJLEEENERESSxBBDREREksQQQ0RERJLEEENERESSxBBDREREksQQQ0RERJLEEENERESSxBBDREREksQQQ0RERJLEEENERESSxBBDREREksQQQ0RERJLEEENERESSxBBDREREksQQQ0RERJLEEENERESSxBBDREREksQQQ0RERJLEEENERESSxBBDREREksQQQ0RERJLEEENERESSxBBDREREksQQQ0RERJLEEENERESSxBBDREREksQQQ0RERJLEEENERESSxBBDREREksQQQ0RERJLEEENERESSxBBDREREksQQQ0RERJLEEENERESSxBBDREREksQQQ0RERJLEEENUiJwcgdu3U/VdBhmhhIRUZGfn6LsMMjIPHqTh6dMMfZdRrhT6LuBV+/TT3xEQ0ABt29aAjY2ZvsshCTMxkeGXXy7iyy+j4efnDl9fN/j5ucPNrbK+SyOJe/DgGdq2XQtvbwf1+6pxYwfI5fxeSaVnZqZAYOAmZGbmwM/vxfuqTZvqsLAw1XdpOiMTQgh9F/EqpKamwsbGBsAUAGYwMZHhtdec1B8Q7dox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",
+                        "image/png": "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HB0dS1sSERERVSClCjFPnjzBwIEDsXLlStja2uabn5CQgJEjRyIsLAxKpbLY9bVo0QLz589H//79oVKpim1PREREVKoQM2LECAQGBsLf3z/fvJycHAQFBWHixIlo0EB3Z8inp6cjNTVV40FEREQVh9Yn9oaHhyMuLg6xsQX/ONncuXOhUCgwevToMhdXlNDQUMyYMUOnf4OIiIgMl1Z7YuLj4zFmzBhs3LgRZmZm+eYfP34cixYtwrp163R+iV9ISAhSUlLUj/j4eJ3+PSIiIjIsWoWY48ePIykpCc2aNYNCoYBCoUBUVBQWL14MhUKByMhIJCUloUaNGur5N2/exPjx4+Hu7v5KC1epVLC2ttZ4EBERUcWh1eGkTp064cyZMxrTgoODUa9ePUyePBlOTk4ICAjQmB8QEICgoCAEBweXvVoiIiKi/6dViLGyskLDhg01pllYWMDe3l493d7eXmO+UqmEo6MjPD091dMGDRoEFxcXhIaGAgAyMjJw/vx59f8nJCTg5MmTsLS0RO3atUFERESUl17u2Hvr1i2YmPx7JCsxMRFNmzZVP1+wYAEWLFgAX19fREZG6qFCIiIiMnT87SQiIiLSm7Jsv8v0swNERERE+sIQQ0RERJLEEENERESSxBBDREREksQQQ0RERJLEEENERESSxBBDREREksQQQ0RERJLEEENERESSxBBDREREksQQQ0RERJLEEENERESSxBBDREREksQQQ0RERJLEEENERESSxBBDREREksQQQ0RERJLEEENERESSxBBDREREksQQQ0RERJLEEENERESSxBBDREREksQQQ0RERJLEEENERESSxBBDREREksQQQ0RERJLEEENERESSxBBDREREksQQQ0RERJLEEENERESSxBBDREREksQQQ0RERJLEEENERESSxBBDREREksQQQ0RERJLEEENERESSxBBDREREksQQQ0RERJLEEENUiJwcgdu3U/VdBhmhhIRUZGfn6LsMMjIPHqTh6dMMfZdRrhT6LuBV+/TT3xEQ0ABt29aAjY2ZvsshCTMxkeGXXy7iyy+j4efnDl9fN/j5ucPNrbK+SyOJe/DgGdq2XQtvbwf1+6pxYwfI5fxeSaVnZqZAYOAmZGbmwM/vxfuqTZvqsLAw1XdpOiMTQgh9F/EqpKamwsbGBsAUAGYwMZHhtdec1B8Q7dox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",
                         "text/plain": [
                             "<Figure size 640x480 with 2 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "from matplotlib import pyplot as plt\n",
+                "import numpy as np\n",
+                "\n",
+                "\n",
+                "currents_df[\"mod\"] = np.sqrt(currents_df.u**2 + currents_df.v**2)\n",
+                "winds_df[\"mod\"] = np.sqrt(winds_df.u**2 + winds_df.v**2)\n",
                 "\n",
                 "currents_time = 1\n",
                 "currents = currents_df.loc[currents_df[\"time\"] == currents_time]\n",
                 "\n",
                 "winds_time = 3\n",
                 "winds = winds_df.loc[winds_df[\"time\"] == winds_time]\n",
                 "\n",
@@ -264,15 +272,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.8"
+            "version": "3.11.3"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "792594d832ea4326378f39c6741adae5559c80a209244a934d002d1e59cc9c68"
             }
         }
```

### Comparing `pyteseo-0.0.5/docs/notebooks/04_floater_simulation.ipynb` & `pyteseo-0.0.6/docs/notebooks/06_hns_simulation.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921875%*

 * *Differences: {"'cells'": "{0: {'source': ['# Hns simulation']}}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Floater simulation"
+                "# Hns simulation"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `pyteseo-0.0.5/docs/notebooks/05_oil_simulation.ipynb` & `pyteseo-0.0.6/docs/notebooks/07_stochastic_montecarlo.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9817708333333334%*

 * *Differences: {"'cells'": "{0: {'source': ['# Montecarlo stochastic methodology']}}",*

 * * "'metadata'": "{'kernelspec': {'display_name': 'pyteseo-dev'}, 'language_info': {'version': "*

 * *               "'3.11.3'}, 'vscode': {'interpreter': {'hash': "*

 * *               "'792594d832ea4326378f39c6741adae5559c80a209244a934d002d1e59cc9c68'}}}"}*

```diff
@@ -1,40 +1,40 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Oil simulation"
+                "# Montecarlo stochastic methodology"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "print(\"To be completed...\")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "pyteseo-dev",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "name": "python",
-            "version": "3.8.10 (default, Jun 22 2022, 20:18:18) \n[GCC 9.4.0]"
+            "version": "3.11.3"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
-                "hash": "916dbcbb3f70747c44a77c7bcd40155683ae19c65e1c03b4aa3499c5328201f1"
+                "hash": "792594d832ea4326378f39c6741adae5559c80a209244a934d002d1e59cc9c68"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `pyteseo-0.0.5/docs/notebooks/07_stochastic_montecarlo.ipynb` & `pyteseo-0.0.6/docs/notebooks/08_stochastic_kmeans.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921875%*

 * *Differences: {"'cells'": "{0: {'source': ['# Kmeans clustering methodology']}}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Montecarlo stochastic methodology"
+                "# Kmeans clustering methodology"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `pyteseo-0.0.5/docs/user-guide.md` & `pyteseo-0.0.6/docs/user-guide.md`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyproject.toml` & `pyteseo-0.0.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,40 +4,46 @@
 
 
 [project]
 name = "pyteseo"
 authors = [{name = "German Aragon Caminero", email = "german.aragon@unican.es"}]
 mantainers = [{name = "German Aragon Caminero", email = "german.aragon@unican.es"}]
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Physics",
     "Development Status :: 1 - Planning",
     "Programming Language :: Python",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
+    # "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["version", "description"]
 
 dependencies = [
+    "geopandas",
+    "owslib",
     "xarray",
     "dask",
-    "netcdf4",
+    "netcdf4<=1.5.8",
     "bottleneck",
     "ipykernel",
     "matplotlib",
     "geojson",
     "pytest >=7",
+    "lxml",
+    "scipy",
+    "python-dotenv",
+    "pydap",
+    "openpyxl"
 ]
 
 
 [project.optional-dependencies]
 dev = ["flit", "black", "sphinx", "coverage[toml]", "myst-nb", "sphinx-autoapi", "sphinx_rtd_theme"]
 
 
@@ -49,15 +55,15 @@
 
 
 [project.scripts]
 pyteseo-tests = "pyteseo.tests.__init__:run_tests"
 
 
 [tool.pytest.ini_options]
-addopts = "-v --durations=0 --durations-min=0.1"
+addopts = "--durations=0 --durations-min=0.1"
 testpaths = "pyteseo"
 
 
 [tool.coverage.run]
 command_line = "-m pytest"
 omit = ["*/tests/*"]
 source = ["pyteseo"]
```

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000000.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000000.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000005.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000005.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000010.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000010.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000015.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000015.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000020.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000020.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000025.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000025.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000030.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000030.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000035.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000035.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000040.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000040.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000045.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000045.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000050.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000050.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000055.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000055.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000060.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000060.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000065.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000065.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000070.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000070.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000075.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000075.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000080.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000080.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000085.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000085.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_001_000090.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000090.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000000.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000000.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000005.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000005.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000010.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000010.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000015.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000015.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000020.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000020.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000025.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000025.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000030.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000030.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000035.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000035.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000040.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000040.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000045.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000045.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000050.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000050.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000055.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000055.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000060.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000060.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000065.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000065.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000070.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000070.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000075.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000075.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000080.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000080.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000085.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000085.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_grid_002_000090.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000090.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000000.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000000.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000005.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000005.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000010.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000010.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000015.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000015.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000020.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000020.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000025.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000025.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000030.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000030.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000035.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000035.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000040.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000040.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000045.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000045.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000050.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000050.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000055.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000055.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000060.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000060.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000065.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000065.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000070.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000070.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000075.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000075.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000080.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000080.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000085.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000085.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_particles_000090.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000090.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_properties_001.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_properties_001.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/cas1_properties_002.txt` & `pyteseo-0.0.6/pyteseo/tests/data/cas1_properties_002.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/coastline.dat` & `pyteseo-0.0.6/pyteseo/tests/data/coastline.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/coastline_error_range.dat` & `pyteseo-0.0.6/pyteseo/tests/data/coastline_error_range.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/coastline_othernanformat.dat` & `pyteseo-0.0.6/pyteseo/tests/data/coastline_othernanformat.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/costa_poligono1.dat` & `pyteseo-0.0.6/pyteseo/tests/data/costa_poligono1.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/costa_poligono2.dat` & `pyteseo-0.0.6/pyteseo/tests/data/costa_poligono2.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/costa_poligono3.dat` & `pyteseo-0.0.6/pyteseo/tests/data/costa_poligono3.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/costa_poligono4.dat` & `pyteseo-0.0.6/pyteseo/tests/data/costa_poligono4.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/currents_000h.txt` & `pyteseo-0.0.6/pyteseo/tests/data/currents_000h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/currents_000h_error_range.txt` & `pyteseo-0.0.6/pyteseo/tests/data/winds_000h.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-196.870594e+00 4.39878497e+01 -3.76573616e+00 5.09147505e-01
+9.61870594e+00 4.39878497e+01 -3.76573616e+00 5.09147505e-01
 9.61870594e+00 4.41128497e+01 -3.76573616e+00 5.09147505e-01
 9.61870594e+00 4.42378497e+01 -3.76573616e+00 5.09147505e-01
 9.74370594e+00 4.39878497e+01 -3.76573616e+00 5.09147505e-01
 9.74370594e+00 4.41128497e+01 -3.76573616e+00 5.09147505e-01
 9.74370594e+00 4.42378497e+01 -3.76573616e+00 5.09147505e-01
 9.86870594e+00 4.39878497e+01 -3.76573616e+00 5.09147505e-01
 9.86870594e+00 4.41128497e+01 -3.76573616e+00 5.09147505e-01
```

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/currents_000h_error_sort.txt` & `pyteseo-0.0.6/pyteseo/tests/data/currents_001h.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-9.61870594e+00 4.59878497e+01 -3.76573616e+00 5.09147505e-01
-9.61870594e+00 4.41128497e+01 -3.76573616e+00 5.09147505e-01
-9.61870594e+00 4.42378497e+01 -3.76573616e+00 5.09147505e-01
-9.74370594e+00 4.39878497e+01 -3.76573616e+00 5.09147505e-01
-9.74370594e+00 4.41128497e+01 -3.76573616e+00 5.09147505e-01
-9.74370594e+00 4.42378497e+01 -3.76573616e+00 5.09147505e-01
-9.86870594e+00 4.39878497e+01 -3.76573616e+00 5.09147505e-01
-9.86870594e+00 4.41128497e+01 -3.76573616e+00 5.09147505e-01
-9.86870594e+00 4.42378497e+01 -3.76573616e+00 5.09147505e-01
-9.99370594e+00 4.39878497e+01 -3.76573616e+00 5.09147505e-01
-9.99370594e+00 4.41128497e+01 -3.76573616e+00 5.09147505e-01
-9.99370594e+00 4.42378497e+01 -3.76573616e+00 5.09147505e-01
+9.61870594e+00 4.39878497e+01 -4.72918749e+00 2.80798605e+00
+9.61870594e+00 4.41128497e+01 -4.72918749e+00 2.80798605e+00
+9.61870594e+00 4.42378497e+01 -4.72918749e+00 2.80798605e+00
+9.74370594e+00 4.39878497e+01 -4.72918749e+00 2.80798605e+00
+9.74370594e+00 4.41128497e+01 -4.72918749e+00 2.80798605e+00
+9.74370594e+00 4.42378497e+01 -4.72918749e+00 2.80798605e+00
+9.86870594e+00 4.39878497e+01 -4.72918749e+00 2.80798605e+00
+9.86870594e+00 4.41128497e+01 -4.72918749e+00 2.80798605e+00
+9.86870594e+00 4.42378497e+01 -4.72918749e+00 2.80798605e+00
+9.99370594e+00 4.39878497e+01 -4.72918749e+00 2.80798605e+00
+9.99370594e+00 4.41128497e+01 -4.72918749e+00 2.80798605e+00
+9.99370594e+00 4.42378497e+01 -4.72918749e+00 2.80798605e+00
```

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/currents_001h.txt` & `pyteseo-0.0.6/pyteseo/tests/data/winds_001h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/currents_002h.txt` & `pyteseo-0.0.6/pyteseo/tests/data/currents_002h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/currents_003h.txt` & `pyteseo-0.0.6/pyteseo/tests/data/currents_003h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/grid.dat` & `pyteseo-0.0.6/pyteseo/tests/data/grid.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/grid_coordinates.txt` & `pyteseo-0.0.6/pyteseo/tests/data/grid_coordinates.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/grid_error_range.dat` & `pyteseo-0.0.6/pyteseo/tests/data/grid_error_var.dat`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-  -182.09897e+00   4.3382352e+01  -9.9990000e+03
-  -3.8449897e+00   4.3382858e+01  -9.9990000e+03
-  -3.8449897e+00   4.3383363e+01  -9.9990000e+03
-  -3.8449897e+00   4.3383868e+01  -9.9990000e+03
-  -3.8449897e+00   4.3384373e+01  -9.9990000e+03
-  -3.8449897e+00   4.3384878e+01  -9.9990000e+03
-  -3.8449897e+00   4.3385383e+01  -9.9990000e+03
-  -3.8449897e+00   4.3385888e+01  -9.9990000e+03
-  -3.8449897e+00   4.3386393e+01  -9.9990000e+03
-  -3.8449897e+00   4.3386898e+01  -9.9990000e+03
-  -3.8449897e+00   4.3387403e+01  -9.9990000e+03
-  -3.8449897e+00   4.3387908e+01  -9.9990000e+03
+  -3.8449897e+00   4.3382352e+01  -9.9990000e+03  -9.9990000e+03
+  -3.8449897e+00   4.3382858e+01  -9.9990000e+03  -9.9990000e+03
+  -3.8449897e+00   4.3383363e+01  -9.9990000e+03  -9.9990000e+03
+  -3.8449897e+00   4.3383868e+01  -9.9990000e+03  -9.9990000e+03
+  -3.8449897e+00   4.3384373e+01  -9.9990000e+03  -9.9990000e+03
+  -3.8449897e+00   4.3384878e+01  -9.9990000e+03  -9.9990000e+03
+  -3.8449897e+00   4.3385383e+01  -9.9990000e+03  -9.9990000e+03
+  -3.8449897e+00   4.3385888e+01  -9.9990000e+03  -9.9990000e+03
+  -3.8449897e+00   4.3386393e+01  -9.9990000e+03  -9.9990000e+03
+  -3.8449897e+00   4.3386898e+01  -9.9990000e+03  -9.9990000e+03
+  -3.8449897e+00   4.3387403e+01  -9.9990000e+03  -9.9990000e+03
+  -3.8449897e+00   4.3387908e+01  -9.9990000e+03  -9.9990000e+03
   -3.8449897e+00   4.3388413e+01  -9.9990000e+03
   -3.8449897e+00   4.3388918e+01  -9.9990000e+03
   -3.8449897e+00   4.3389423e+01  -9.9990000e+03
   -3.8449897e+00   4.3389928e+01  -9.9990000e+03
   -3.8449897e+00   4.3390434e+01  -9.9990000e+03
   -3.8449897e+00   4.3390939e+01  -9.9990000e+03
   -3.8449897e+00   4.3391444e+01  -9.9990000e+03
```

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/winds_002h.txt` & `pyteseo-0.0.6/pyteseo/tests/data/winds_002h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/data/winds_003h.txt` & `pyteseo-0.0.6/pyteseo/tests/data/winds_003h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.5/pyteseo/tests/test_export.py` & `pyteseo-0.0.6/pyteseo/tests/unit/test_export.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from pathlib import Path
 from shutil import rmtree
+
 import pytest
+
 from pyteseo.__init__ import __version__ as v
-from pyteseo.export import (
-    export_particles,
-    export_properties,
-    export_grids,
-)
-from pyteseo.io import (
+from pyteseo.export.grids import export_grids
+from pyteseo.export.particles import export_particles
+from pyteseo.export.properties import export_properties
+from pyteseo.io.results import (
+    read_grids_results,
     read_particles_results,
     read_properties_results,
-    read_grids_results,
 )
 
-
-data_path = Path(__file__).parent / "data"
+# data_path = Path(__file__).parent.parent / "data"
+# data_path = Path(__file__).parent.parent / "data/drift_simulation"
+data_path = Path(__file__).parent.parent / "data/oil_simulation"
+# data_path = Path(__file__).parent.parent / "data/hns_simulation"
 tmp_path = Path(f"./tmp_pyteseo_{v}_tests")
 
 
 @pytest.fixture
 def setup_teardown():
     if not tmp_path.exists():
         tmp_path.mkdir()
```

### Comparing `pyteseo-0.0.5/PKG-INFO` & `pyteseo-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 Metadata-Version: 2.1
 Name: pyteseo
-Version: 0.0.5
-Summary: Python package developed to simplify and facilitate the setup and processing of TESEO simulations (TESEO is a lagrangian numerical model developed by IHCantabria)
+Version: 0.0.6
+Summary: Python package developed to simplify and facilitate the setup and processing of TESEO simulations (https://ihcantabria.com/en/specialized-software/teseo/)
 Author-email: German Aragon Caminero <german.aragon@unican.es>
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: geopandas
+Requires-Dist: owslib
 Requires-Dist: xarray
 Requires-Dist: dask
-Requires-Dist: netcdf4
+Requires-Dist: netcdf4<=1.5.8
 Requires-Dist: bottleneck
 Requires-Dist: ipykernel
 Requires-Dist: matplotlib
 Requires-Dist: geojson
 Requires-Dist: pytest >=7
+Requires-Dist: lxml
+Requires-Dist: scipy
+Requires-Dist: python-dotenv
+Requires-Dist: pydap
+Requires-Dist: openpyxl
 Requires-Dist: flit ; extra == "dev"
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: sphinx ; extra == "dev"
 Requires-Dist: coverage[toml] ; extra == "dev"
 Requires-Dist: myst-nb ; extra == "dev"
 Requires-Dist: sphinx-autoapi ; extra == "dev"
 Requires-Dist: sphinx_rtd_theme ; extra == "dev"
 Project-URL: changelog, https://github.com/IHCantabria/pyteseo/blob/main/CHANGELOG.md
 Project-URL: documentation, https://ihcantabria.github.io/pyteseo
 Project-URL: home, https://ihcantabria.com/specialized-software/english-teseo/
 Project-URL: repository, https://github.com/IHCantabria/pyteseo
 Provides-Extra: dev
 
-## :warning: Package under development!
-## :soon: First usable version (v1.0.0) will be released soon!
+## Package under development!
 ---
 
 <p align="center">
 <img align="center" width="600" src="https://ihcantabria.github.io/pyteseo/_images/pyTESEO_logo.png">
 </p>
 
 [![pypi](https://img.shields.io/pypi/v/pyteseo)](https://pypi.org/project/pyteseo/)
@@ -62,39 +66,42 @@
 **pyTESEO** is a python package developed by [IHCantabria](https://ihcantabria.com/en/) to simplify and facilitate the setup and processing of [TESEO](https://ihcantabria.com/en/specialized-software/teseo/) simulations *(TESEO is a lagrangian numerical model also developed by IHCantabria.)*
 
 
 ---
 
 ## :computer: Installation
 
-|                         | Linux  | MacOS  | Windows|
-|:-----------------------:|:------:|:------:|:------:|
-| Required python version | >= 3.7 | >= 3.7 | >= 3.8 |
+1 - Install the python library using pip:
 
-
-* From `github` repository using `pip`:
 ```bash
-pip install git+https://github.com/IHCantabria/pyteseo
-# To install extra dev dependencies: pip install git+https://github.com/IHCantabria/pyteseo[dev]
-# Using editable mode: pip install -e git+https://github.com/IHCantabria/pyteseo[dev]
+# From pypi repository
+pip install pyteseo
 
+# Or directly from github repository
+pip install git+https://github.com/IHCantabria/pyteseo
 ```
 
-:warning: `UNDER DEVELOPMENT` :construction: - * From `pypi` using `pip`:
+2 - Install TESEO model binary (**Not available yet!**):
+- Get access to the binary: https://github.com/IHCantabria/TESEO/blob/main/bin
+- Set up environment variable "TESEO_PATH" with the path to the model executable. You can use the command following CLI command after activate the python environement (python-dotenv library)
+
+    ```bash
+        dotenv set TESEO_PATH /path/to/teseo_executable
+    ```
+3 - Opendap connection to some [CMEMS products](https://data.marine.copernicus.eu/products) is available at the library `pyteseo/connections/cmems.py` but needs authetication through the following environement variables:
 ```bash
-pip install pyteseo
+dotenv set CMEMS_username your_username_at_CMEMS
 ```
-:warning: `UNDER DEVELOPMENT` :construction: - * From `conda-forge` using `conda`:
 ```bash
-conda install -c conda-forge pyteseo
+dotenv set CMEMS_password your_password_at_CMEMS
 ```
 
 ---
 
-## :heavy_check_mark: Testing & Coverage
+## :heavy_check_mark: Tests
 Tests are located in `pyteseo/tests/` and data required for tests are located in `pyteseo/tests/data/`.
 Tests have been developed using [pytest](https://docs.pytest.org/).
 
 Run tests to verify your package installation:
 ```bash
 pyteseo-test        # Run tests and prompt pytest-report
 ```
@@ -104,36 +111,29 @@
 # Commands should be executed from the root directory of the repo
 
 coverage run        # For run tests and generate ".coverage" file
 coverage report     # For prompt results from ".coverage" file
 coverage html       # For generate html report on "htmlcov" folder
 ```
 
-
 ---
 
 ## :recycle: Continuous integration (CI)
 
-
 * Build and deploy documentation on Github Pages in [.github/workflows/docs.yml](.github/workflows/docs.yml)
 * Install and test package in diferent environments in [.github/workflows/tests.yml](.github/workflows/tests.yml)
 * Precommit hooks for formats and linting in [.pre-commit-config.yaml](.pre-commit-config.yaml)
 
 *For Linux, Windows, MacOS and compatible python versions defined in installation section*
 
 ---
 
 ## :books: Documentation
 
-Comprenhensive documentation is developed and mantained at https://ihcantabria.github.io/pyteseo
-
-Documentation of all the package, usage and examples based on mockup input data are provided in [Jupyter Notebooks](https://jupyter.org/) format and ready to be used under [Google Colab](https://colab.research.google.com/) online platform.
-
-
-![pyteseo_doc](docs/_static/doc_snapshoot.png)
+Documentation is available at https://ihcantabria.github.io/pyteseo
 
 ---
 
 ## :copyright: Credits
 Developed and maintained by :man_technologist: [German Aragon](https://github.com/aragong) @ :office: [IHCantabria](https://github.com/IHCantabria).
 
 ---
```

