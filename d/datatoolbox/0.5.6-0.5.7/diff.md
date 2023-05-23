# Comparing `tmp/datatoolbox-0.5.6.tar.gz` & `tmp/datatoolbox-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatoolbox-0.5.6.tar", last modified: Wed May 10 09:20:56 2023, max compression
+gzip compressed data, was "datatoolbox-0.5.7.tar", last modified: Tue May 23 12:46:58 2023, max compression
```

## Comparing `datatoolbox-0.5.6.tar` & `datatoolbox-0.5.7.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:56.000000 datatoolbox-0.5.6/
--rwxrwx---   0 root         (0) vboxsf     (999)      159 2022-05-25 07:15:53.000000 datatoolbox-0.5.6/.gitignore
--rwxrwx---   0 root         (0) vboxsf     (999)      950 2022-10-19 13:17:33.000000 datatoolbox-0.5.6/.gitlab-ci.yml
--rwxrwx---   0 root         (0) vboxsf     (999)      703 2020-10-14 14:04:18.000000 datatoolbox-0.5.6/.travis.yml
--rwxrwx---   0 root         (0) vboxsf     (999)     1073 2020-10-14 14:04:18.000000 datatoolbox-0.5.6/LICENSE
--rwxrwx---   0 root         (0) vboxsf     (999)     1037 2023-05-10 09:20:56.000000 datatoolbox-0.5.6/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (999)      771 2022-05-25 07:15:53.000000 datatoolbox-0.5.6/README.md
--rwxrwx---   0 root         (0) vboxsf     (999)     1225 2020-10-14 14:04:18.000000 datatoolbox-0.5.6/appveyor.yml
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/ci/
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/ci/appveyor/
--rwxrwx---   0 root         (0) vboxsf     (999)     3111 2020-10-14 14:04:18.000000 datatoolbox-0.5.6/ci/appveyor/install.ps1
--rwxrwx---   0 root         (0) vboxsf     (999)     1842 2020-10-14 14:04:18.000000 datatoolbox-0.5.6/ci/appveyor/run_with_env.cmd
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/datatoolbox/
--rwxrwx---   0 root         (0) vboxsf     (999)     4362 2023-05-04 12:41:44.000000 datatoolbox-0.5.6/datatoolbox/__init__.py
--rwxrwx---   0 root         (0) vboxsf     (999)    15385 2023-03-30 07:48:47.000000 datatoolbox-0.5.6/datatoolbox/admin.py
--rwxrwx---   0 root         (0) vboxsf     (999)     6655 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/config.py
--rwxrwx---   0 root         (0) vboxsf     (999)    18640 2022-12-01 09:27:15.000000 datatoolbox-0.5.6/datatoolbox/converters.py
--rwxrwx---   0 root         (0) vboxsf     (999)    11733 2022-12-19 11:17:33.000000 datatoolbox-0.5.6/datatoolbox/core.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/datatoolbox/data/
--rwxrwx---   0 root         (0) vboxsf     (999)    15781 2020-10-14 14:04:18.000000 datatoolbox-0.5.6/datatoolbox/data/GHG_alternative_naming.pkl
--rwxrwx---   0 root         (0) vboxsf     (999)    13482 2020-10-14 14:04:18.000000 datatoolbox-0.5.6/datatoolbox/data/GHG_properties_2019_CA.csv
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/datatoolbox/data/SANDBOX_datashelf/
--rwxrwx---   0 root         (0) vboxsf     (999)      286 2023-05-09 08:12:07.000000 datatoolbox-0.5.6/datatoolbox/data/SANDBOX_datashelf/inventory.csv
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/datatoolbox/data/SANDBOX_datashelf/mappings/
--rwxrwx---   0 root         (0) vboxsf     (999)    10757 2023-05-09 08:12:04.000000 datatoolbox-0.5.6/datatoolbox/data/SANDBOX_datashelf/mappings/continent.csv
--rwxrwx---   0 root         (0) vboxsf     (999)     8466 2023-05-09 08:12:04.000000 datatoolbox-0.5.6/datatoolbox/data/SANDBOX_datashelf/mappings/country_codes.csv
--rwxrwx---   0 root         (0) vboxsf     (999)      999 2023-05-09 08:12:04.000000 datatoolbox-0.5.6/datatoolbox/data/SANDBOX_datashelf/mappings/regions.csv
--rwxrwx---   0 root         (0) vboxsf     (999)      161 2023-05-09 08:12:07.000000 datatoolbox-0.5.6/datatoolbox/data/SANDBOX_datashelf/sources.csv
--rwxrwx---   0 root         (0) vboxsf     (999)    22865 2020-10-14 14:04:18.000000 datatoolbox-0.5.6/datatoolbox/data/all.csv
--rwxrwx---   0 root         (0) vboxsf     (999)    14615 2020-10-14 14:04:18.000000 datatoolbox-0.5.6/datatoolbox/data/compatible1_5_unfiltered.xlsx
--rwxrwx---   0 root         (0) vboxsf     (999)    10757 2020-04-20 12:32:09.000000 datatoolbox-0.5.6/datatoolbox/data/continent.csv
--rwxrwx---   0 root         (0) vboxsf     (999)     8466 2021-09-15 15:48:16.000000 datatoolbox-0.5.6/datatoolbox/data/country_codes.csv
--rwxrwx---   0 root         (0) vboxsf     (999)     1711 2022-05-25 07:15:53.000000 datatoolbox-0.5.6/datatoolbox/data/datashelf_contents.csv
--rwxrwx---   0 root         (0) vboxsf     (999)     2923 2021-12-16 12:32:58.000000 datatoolbox-0.5.6/datatoolbox/data/external_mappings.py
--rwxrwx---   0 root         (0) vboxsf     (999)      178 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/data/personal_template.py
--rwxrwx---   0 root         (0) vboxsf     (999)      999 2019-08-14 10:00:22.000000 datatoolbox-0.5.6/datatoolbox/data/regions.csv
--rwxrwx---   0 root         (0) vboxsf     (999)   237054 2023-04-28 11:35:43.000000 datatoolbox-0.5.6/datatoolbox/data_readers.py
--rwxrwx---   0 root         (0) vboxsf     (999)    68067 2023-05-04 07:37:43.000000 datatoolbox-0.5.6/datatoolbox/data_structures.py
--rwxrwx---   0 root         (0) vboxsf     (999)    64211 2023-05-10 08:59:02.000000 datatoolbox-0.5.6/datatoolbox/database.py
--rwxrwx---   0 root         (0) vboxsf     (999)     6730 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/greenhouse_gas_database.py
--rwxrwx---   0 root         (0) vboxsf     (999)     3542 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/init_tools.py
--rwxrwx---   0 root         (0) vboxsf     (999)    21652 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/interfaces.py
--rwxrwx---   0 root         (0) vboxsf     (999)    10991 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/io_tools.py
--rwxrwx---   0 root         (0) vboxsf     (999)    41818 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/mapping.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2854 2022-12-01 09:27:15.000000 datatoolbox-0.5.6/datatoolbox/naming_convention.py
--rwxrwx---   0 root         (0) vboxsf     (999)     3305 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/patches.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2175 2022-11-16 12:15:23.000000 datatoolbox-0.5.6/datatoolbox/pint_definitions.txt
--rwxrwx---   0 root         (0) vboxsf     (999)        0 2020-06-08 07:09:19.000000 datatoolbox-0.5.6/datatoolbox/relations.py
--rwxrwx---   0 root         (0) vboxsf     (999)    26527 2023-04-05 07:52:48.000000 datatoolbox-0.5.6/datatoolbox/sets.py
--rwxrwx---   0 root         (0) vboxsf     (999)        0 2020-06-08 07:09:19.000000 datatoolbox-0.5.6/datatoolbox/storage.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1632 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/templates.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/datatoolbox/tools/
--rwxrwx---   0 root         (0) vboxsf     (999)    16351 2021-04-19 11:31:45.000000 datatoolbox-0.5.6/datatoolbox/tools/CRF_extract_CA_2021.xlsx
--rwxrwx---   0 root         (0) vboxsf     (999)    28022 2021-02-02 15:17:26.000000 datatoolbox-0.5.6/datatoolbox/tools/EQW_SPLIT_EFF0460_CATEFFEXT_210120.SCEN
--rwxrwx---   0 root         (0) vboxsf     (999)    17445 2021-02-02 12:48:44.000000 datatoolbox-0.5.6/datatoolbox/tools/IEA_B2DS_4.SCEN
--rwxrwx---   0 root         (0) vboxsf     (999)    17375 2019-12-20 11:46:57.000000 datatoolbox-0.5.6/datatoolbox/tools/WEO_2019_test.SCEN
--rwxrwx---   0 root         (0) vboxsf     (999)      390 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/__init__.py
--rwxrwx---   0 root         (0) vboxsf     (999)     4320 2022-11-17 09:58:39.000000 datatoolbox-0.5.6/datatoolbox/tools/conversion_to_v0.3.py
--rwxrwx---   0 root         (0) vboxsf     (999)    42729 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/excel.py
--rwxrwx---   0 root         (0) vboxsf     (999)      370 2022-11-17 09:58:39.000000 datatoolbox-0.5.6/datatoolbox/tools/export_all.py
--rwxrwx---   0 root         (0) vboxsf     (999)     4441 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/for_datatables.py
--rwxrwx---   0 root         (0) vboxsf     (999)     8132 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/html.py
--rwxrwx---   0 root         (0) vboxsf     (999)      182 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/install_support.py
--rwxrwx---   0 root         (0) vboxsf     (999)     7188 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/kaya_idendentiy_decomposition.py
--rwxrwx---   0 root         (0) vboxsf     (999)     4283 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/magicc6.py
--rwxrwx---   0 root         (0) vboxsf     (999)     5931 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/matplotlib.py
--rwxrwx---   0 root         (0) vboxsf     (999)     3797 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/pandas.py
--rwxrwx---   0 root         (0) vboxsf     (999)     5533 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/py_magicc_tools.py
--rwxrwx---   0 root         (0) vboxsf     (999)     7869 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/pyam.py
--rwxrwx---   0 root         (0) vboxsf     (999)      965 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/renaming_DB.py
--rwxrwx---   0 root         (0) vboxsf     (999)    84992 2019-08-14 10:26:08.000000 datatoolbox-0.5.6/datatoolbox/tools/run_MAGICC_startup_simple.xlsx
--rwxrwx---   0 root         (0) vboxsf     (999)     1830 2021-02-02 14:03:36.000000 datatoolbox-0.5.6/datatoolbox/tools/run_magicc6.m
--rwxrwx---   0 root         (0) vboxsf     (999)     1044 2022-11-17 09:58:40.000000 datatoolbox-0.5.6/datatoolbox/tools/statistics.py
--rwxrwx---   0 root         (0) vboxsf     (999)    61174 2021-06-03 14:06:07.000000 datatoolbox-0.5.6/datatoolbox/tools/test.docx
--rwxrwx---   0 root         (0) vboxsf     (999)     8625 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/word.py
--rwxrwx---   0 root         (0) vboxsf     (999)     9617 2023-03-30 13:29:22.000000 datatoolbox-0.5.6/datatoolbox/tools/xarray.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:56.000000 datatoolbox-0.5.6/datatoolbox/tutorials/
--rwxrwx---   0 root         (0) vboxsf     (999)     2996 2022-05-25 07:15:53.000000 datatoolbox-0.5.6/datatoolbox/tutorials/00_search_find_and_access_data.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1019 2020-10-14 14:04:18.000000 datatoolbox-0.5.6/datatoolbox/tutorials/01_emission_comparison.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2096 2022-05-25 07:15:53.000000 datatoolbox-0.5.6/datatoolbox/tutorials/02_unit_conversion.py
--rwxrwx---   0 root         (0) vboxsf     (999)     5685 2020-10-14 14:04:18.000000 datatoolbox-0.5.6/datatoolbox/tutorials/03_intermediate_example.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1416 2020-10-14 14:04:19.000000 datatoolbox-0.5.6/datatoolbox/tutorials/04_sources.py
--rwxrwx---   0 root         (0) vboxsf     (999)      382 2020-10-14 14:04:19.000000 datatoolbox-0.5.6/datatoolbox/tutorials/05_plot_source_content.py
--rwxrwx---   0 root         (0) vboxsf     (999)      734 2020-12-22 15:09:15.000000 datatoolbox-0.5.6/datatoolbox/tutorials/06_xarray_examples.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1142 2021-05-11 13:19:29.000000 datatoolbox-0.5.6/datatoolbox/tutorials/07_renewable_share_compuation.py
--rwxrwx---   0 root         (0) vboxsf     (999)      793 2021-05-11 12:59:38.000000 datatoolbox-0.5.6/datatoolbox/tutorials/08_low_carbon_fuel_computation.py
--rwxrwx---   0 root         (0) vboxsf     (999)   137631 2020-10-14 14:04:19.000000 datatoolbox-0.5.6/datatoolbox/tutorials/introduction_v1.ipynb
--rwxrwx---   0 root         (0) vboxsf     (999)     4631 2022-03-22 14:54:50.000000 datatoolbox-0.5.6/datatoolbox/tutorials/jump_start.py
--rwxrwx---   0 root         (0) vboxsf     (999)      300 2022-11-21 13:35:45.000000 datatoolbox-0.5.6/datatoolbox/units.py
--rwxrwx---   0 root         (0) vboxsf     (999)    43915 2022-11-22 09:50:19.000000 datatoolbox-0.5.6/datatoolbox/util.py
--rwxrwx---   0 root         (0) vboxsf     (999)      176 2023-05-10 09:20:54.000000 datatoolbox-0.5.6/datatoolbox/version.py
--rwxrwx---   0 root         (0) vboxsf     (999)      746 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/workflows.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/datatoolbox.egg-info/
--rwxrwx---   0 root         (0) vboxsf     (999)     1037 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/datatoolbox.egg-info/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (999)     3714 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/datatoolbox.egg-info/SOURCES.txt
--rwxrwx---   0 root         (0) vboxsf     (999)        1 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/datatoolbox.egg-info/dependency_links.txt
--rwxrwx---   0 root         (0) vboxsf     (999)      149 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/datatoolbox.egg-info/requires.txt
--rwxrwx---   0 root         (0) vboxsf     (999)       12 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/datatoolbox.egg-info/top_level.txt
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:56.000000 datatoolbox-0.5.6/doc/
--rwxrwx---   0 root         (0) vboxsf     (999)     7755 2020-10-14 14:04:19.000000 datatoolbox-0.5.6/doc/Makefile
--rwxrwx---   0 root         (0) vboxsf     (999)     9684 2020-12-22 15:09:15.000000 datatoolbox-0.5.6/doc/conf.py
--rwxrwx---   0 root         (0) vboxsf     (999)       79 2021-01-05 10:54:01.000000 datatoolbox-0.5.6/doc/core.rst
--rwxrwx---   0 root         (0) vboxsf     (999)      149 2020-12-22 15:09:15.000000 datatoolbox-0.5.6/doc/data_structures.rst
--rwxrwx---   0 root         (0) vboxsf     (999)      122 2021-01-11 16:19:59.000000 datatoolbox-0.5.6/doc/database.rst
--rwxrwx---   0 root         (0) vboxsf     (999)       91 2021-01-11 16:18:53.000000 datatoolbox-0.5.6/doc/database_database.rst
--rwxrwx---   0 root         (0) vboxsf     (999)      130 2021-01-11 16:21:50.000000 datatoolbox-0.5.6/doc/database_gitrepomanager.rst
--rwxrwx---   0 root         (0) vboxsf     (999)       93 2021-01-11 16:03:03.000000 datatoolbox-0.5.6/doc/excel.rst
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:56.000000 datatoolbox-0.5.6/doc/figures/
--rwxrwx---   0 root         (0) vboxsf     (999)    21579 2020-11-09 13:08:35.000000 datatoolbox-0.5.6/doc/figures/ID_meta_data.svg
--rwxrwx---   0 root         (0) vboxsf     (999)    67463 2021-05-17 15:08:58.000000 datatoolbox-0.5.6/doc/figures/config_input.png
--rwxrwx---   0 root         (0) vboxsf     (999)     7157 2021-05-17 15:04:37.000000 datatoolbox-0.5.6/doc/first_steps.md
--rwxrwx---   0 root         (0) vboxsf     (999)      100 2020-12-22 15:09:15.000000 datatoolbox-0.5.6/doc/foo.rst_template
--rwxrwx---   0 root         (0) vboxsf     (999)       77 2020-12-22 15:09:15.000000 datatoolbox-0.5.6/doc/help.rst
--rwxrwx---   0 root         (0) vboxsf     (999)      463 2021-01-11 16:06:28.000000 datatoolbox-0.5.6/doc/index.rst
--rwxrwx---   0 root         (0) vboxsf     (999)     1754 2021-05-21 08:03:28.000000 datatoolbox-0.5.6/doc/installation.md
--rwxrwx---   0 root         (0) vboxsf     (999)     1080 2020-12-22 15:09:15.000000 datatoolbox-0.5.6/doc/license.rst
--rwxrwx---   0 root         (0) vboxsf     (999)     7353 2020-10-14 14:04:19.000000 datatoolbox-0.5.6/doc/make.bat
--rwxrwx---   0 root         (0) vboxsf     (999)      103 2021-01-11 16:09:22.000000 datatoolbox-0.5.6/doc/matplotlib.rst
--rwxrwx---   0 root         (0) vboxsf     (999)       95 2021-01-11 16:10:43.000000 datatoolbox-0.5.6/doc/pandas.rst
--rwxrwx---   0 root         (0) vboxsf     (999)      133 2021-01-11 16:20:57.000000 datatoolbox-0.5.6/doc/tools.rst
--rwxrwx---   0 root         (0) vboxsf     (999)       95 2021-01-11 16:09:13.000000 datatoolbox-0.5.6/doc/xarray.rst
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:56.000000 datatoolbox-0.5.6/documentation/
--rwxrwx---   0 root         (0) vboxsf     (999)     7761 2020-12-22 15:09:15.000000 datatoolbox-0.5.6/documentation/Datatoolbox - First steps.md
--rwxrwx---   0 root         (0) vboxsf     (999)      381 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/environment.yml
--rwxrwx---   0 root         (0) vboxsf     (999)      418 2020-10-14 14:04:19.000000 datatoolbox-0.5.6/make_proj.sh
--rwxrwx---   0 root         (0) vboxsf     (999)      558 2021-01-12 15:45:18.000000 datatoolbox-0.5.6/readthedocs.yml
--rwxrwx---   0 root         (0) vboxsf     (999)      215 2022-10-19 13:17:33.000000 datatoolbox-0.5.6/requirements.txt
--rwxrwx---   0 root         (0) vboxsf     (999)       38 2023-05-10 09:20:56.000000 datatoolbox-0.5.6/setup.cfg
--rwxrwx---   0 root         (0) vboxsf     (999)     1839 2023-05-03 11:16:28.000000 datatoolbox-0.5.6/setup.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:56.000000 datatoolbox-0.5.6/tests/
--rwxrwx---   0 root         (0) vboxsf     (999)     7292 2022-12-19 11:29:58.000000 datatoolbox-0.5.6/tests/test_calculations.py
--rwxrwx---   0 root         (0) vboxsf     (999)      696 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/tests/test_converters.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2836 2022-11-21 11:08:31.000000 datatoolbox-0.5.6/tests/test_database.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1640 2023-03-30 13:32:13.000000 datatoolbox-0.5.6/tests/test_dataset.py
--rwxrwx---   0 root         (0) vboxsf     (999)     7741 2022-05-25 07:15:53.000000 datatoolbox-0.5.6/tests/test_datatable.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1063 2022-11-16 11:59:46.000000 datatoolbox-0.5.6/tests/test_io.py
--rwxrwx---   0 root         (0) vboxsf     (999)      390 2022-11-22 09:54:34.000000 datatoolbox-0.5.6/tests/test_linked_functions.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1563 2023-05-04 07:49:24.000000 datatoolbox-0.5.6/tests/test_pyam.py
--rwxrwx---   0 root         (0) vboxsf     (999)     3570 2022-05-25 07:15:53.000000 datatoolbox-0.5.6/tests/test_tableset.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2610 2022-05-25 07:15:53.000000 datatoolbox-0.5.6/tests/test_tools.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1227 2022-11-21 13:23:54.000000 datatoolbox-0.5.6/tests/test_units.py
--rwxrwx---   0 root         (0) vboxsf     (999)      870 2020-10-14 14:04:19.000000 datatoolbox-0.5.6/tests/test_utilities.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2437 2022-10-19 13:17:33.000000 datatoolbox-0.5.6/tests/test_xarray.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2959 2022-05-25 07:15:53.000000 datatoolbox-0.5.6/tests/util_for_testing.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 12:46:58.000000 datatoolbox-0.5.7/
+-rwxrwx---   0 root         (0) vboxsf     (999)      159 2022-05-25 07:15:53.000000 datatoolbox-0.5.7/.gitignore
+-rwxrwx---   0 root         (0) vboxsf     (999)      950 2022-10-19 13:17:33.000000 datatoolbox-0.5.7/.gitlab-ci.yml
+-rwxrwx---   0 root         (0) vboxsf     (999)      703 2020-10-14 14:04:18.000000 datatoolbox-0.5.7/.travis.yml
+-rwxrwx---   0 root         (0) vboxsf     (999)     1073 2020-10-14 14:04:18.000000 datatoolbox-0.5.7/LICENSE
+-rwxrwx---   0 root         (0) vboxsf     (999)     1037 2023-05-23 12:46:58.000000 datatoolbox-0.5.7/PKG-INFO
+-rwxrwx---   0 root         (0) vboxsf     (999)      771 2022-05-25 07:15:53.000000 datatoolbox-0.5.7/README.md
+-rwxrwx---   0 root         (0) vboxsf     (999)     1225 2020-10-14 14:04:18.000000 datatoolbox-0.5.7/appveyor.yml
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 12:46:57.000000 datatoolbox-0.5.7/ci/
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 12:46:57.000000 datatoolbox-0.5.7/ci/appveyor/
+-rwxrwx---   0 root         (0) vboxsf     (999)     3111 2020-10-14 14:04:18.000000 datatoolbox-0.5.7/ci/appveyor/install.ps1
+-rwxrwx---   0 root         (0) vboxsf     (999)     1842 2020-10-14 14:04:18.000000 datatoolbox-0.5.7/ci/appveyor/run_with_env.cmd
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 12:46:57.000000 datatoolbox-0.5.7/datatoolbox/
+-rwxrwx---   0 root         (0) vboxsf     (999)     4362 2023-05-04 12:41:44.000000 datatoolbox-0.5.7/datatoolbox/__init__.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    15385 2023-03-30 07:48:47.000000 datatoolbox-0.5.7/datatoolbox/admin.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     6655 2022-11-18 16:16:07.000000 datatoolbox-0.5.7/datatoolbox/config.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    18622 2023-05-23 08:37:11.000000 datatoolbox-0.5.7/datatoolbox/converters.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    12133 2023-05-12 12:29:10.000000 datatoolbox-0.5.7/datatoolbox/core.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 12:46:57.000000 datatoolbox-0.5.7/datatoolbox/data/
+-rwxrwx---   0 root         (0) vboxsf     (999)    15781 2020-10-14 14:04:18.000000 datatoolbox-0.5.7/datatoolbox/data/GHG_alternative_naming.pkl
+-rwxrwx---   0 root         (0) vboxsf     (999)    13482 2020-10-14 14:04:18.000000 datatoolbox-0.5.7/datatoolbox/data/GHG_properties_2019_CA.csv
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 12:46:57.000000 datatoolbox-0.5.7/datatoolbox/data/SANDBOX_datashelf/
+-rwxrwx---   0 root         (0) vboxsf     (999)      286 2023-05-12 12:11:16.000000 datatoolbox-0.5.7/datatoolbox/data/SANDBOX_datashelf/inventory.csv
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 12:46:57.000000 datatoolbox-0.5.7/datatoolbox/data/SANDBOX_datashelf/mappings/
+-rwxrwx---   0 root         (0) vboxsf     (999)    10757 2023-05-12 12:11:14.000000 datatoolbox-0.5.7/datatoolbox/data/SANDBOX_datashelf/mappings/continent.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)     8466 2023-05-12 12:11:14.000000 datatoolbox-0.5.7/datatoolbox/data/SANDBOX_datashelf/mappings/country_codes.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)      999 2023-05-12 12:11:14.000000 datatoolbox-0.5.7/datatoolbox/data/SANDBOX_datashelf/mappings/regions.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)      161 2023-05-12 12:11:16.000000 datatoolbox-0.5.7/datatoolbox/data/SANDBOX_datashelf/sources.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)    22865 2020-10-14 14:04:18.000000 datatoolbox-0.5.7/datatoolbox/data/all.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)    14615 2020-10-14 14:04:18.000000 datatoolbox-0.5.7/datatoolbox/data/compatible1_5_unfiltered.xlsx
+-rwxrwx---   0 root         (0) vboxsf     (999)    10757 2020-04-20 12:32:09.000000 datatoolbox-0.5.7/datatoolbox/data/continent.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)     8466 2021-09-15 15:48:16.000000 datatoolbox-0.5.7/datatoolbox/data/country_codes.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)     1711 2022-05-25 07:15:53.000000 datatoolbox-0.5.7/datatoolbox/data/datashelf_contents.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)     2923 2021-12-16 12:32:58.000000 datatoolbox-0.5.7/datatoolbox/data/external_mappings.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      178 2022-11-18 16:16:07.000000 datatoolbox-0.5.7/datatoolbox/data/personal_template.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      999 2019-08-14 10:00:22.000000 datatoolbox-0.5.7/datatoolbox/data/regions.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)   237054 2023-04-28 11:35:43.000000 datatoolbox-0.5.7/datatoolbox/data_readers.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    69372 2023-05-23 08:25:42.000000 datatoolbox-0.5.7/datatoolbox/data_structures.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    64211 2023-05-10 08:59:02.000000 datatoolbox-0.5.7/datatoolbox/database.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     6730 2022-11-18 16:16:07.000000 datatoolbox-0.5.7/datatoolbox/greenhouse_gas_database.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     3542 2022-11-18 16:16:07.000000 datatoolbox-0.5.7/datatoolbox/init_tools.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    21652 2022-11-18 16:16:07.000000 datatoolbox-0.5.7/datatoolbox/interfaces.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    11001 2023-05-22 11:47:04.000000 datatoolbox-0.5.7/datatoolbox/io_tools.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    41818 2022-11-18 16:16:07.000000 datatoolbox-0.5.7/datatoolbox/mapping.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2854 2022-12-01 09:27:15.000000 datatoolbox-0.5.7/datatoolbox/naming_convention.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     3305 2022-11-18 16:16:07.000000 datatoolbox-0.5.7/datatoolbox/patches.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2189 2023-05-12 10:35:54.000000 datatoolbox-0.5.7/datatoolbox/pint_definitions.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)        0 2020-06-08 07:09:19.000000 datatoolbox-0.5.7/datatoolbox/relations.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    26527 2023-04-05 07:52:48.000000 datatoolbox-0.5.7/datatoolbox/sets.py
+-rwxrwx---   0 root         (0) vboxsf     (999)        0 2020-06-08 07:09:19.000000 datatoolbox-0.5.7/datatoolbox/storage.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1632 2022-11-18 16:16:07.000000 datatoolbox-0.5.7/datatoolbox/templates.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 12:46:57.000000 datatoolbox-0.5.7/datatoolbox/tools/
+-rwxrwx---   0 root         (0) vboxsf     (999)    16351 2021-04-19 11:31:45.000000 datatoolbox-0.5.7/datatoolbox/tools/CRF_extract_CA_2021.xlsx
+-rwxrwx---   0 root         (0) vboxsf     (999)    28022 2021-02-02 15:17:26.000000 datatoolbox-0.5.7/datatoolbox/tools/EQW_SPLIT_EFF0460_CATEFFEXT_210120.SCEN
+-rwxrwx---   0 root         (0) vboxsf     (999)    17445 2021-02-02 12:48:44.000000 datatoolbox-0.5.7/datatoolbox/tools/IEA_B2DS_4.SCEN
+-rwxrwx---   0 root         (0) vboxsf     (999)    17375 2019-12-20 11:46:57.000000 datatoolbox-0.5.7/datatoolbox/tools/WEO_2019_test.SCEN
+-rwxrwx---   0 root         (0) vboxsf     (999)      390 2022-11-18 16:16:07.000000 datatoolbox-0.5.7/datatoolbox/tools/__init__.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     4320 2022-11-17 09:58:39.000000 datatoolbox-0.5.7/datatoolbox/tools/conversion_to_v0.3.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    42729 2022-11-18 16:16:07.000000 datatoolbox-0.5.7/datatoolbox/tools/excel.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      370 2022-11-17 09:58:39.000000 datatoolbox-0.5.7/datatoolbox/tools/export_all.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     4441 2022-11-18 16:16:07.000000 datatoolbox-0.5.7/datatoolbox/tools/for_datatables.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     8132 2022-11-18 16:16:07.000000 datatoolbox-0.5.7/datatoolbox/tools/html.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      182 2022-11-18 16:16:07.000000 datatoolbox-0.5.7/datatoolbox/tools/install_support.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     7188 2022-11-18 16:16:07.000000 datatoolbox-0.5.7/datatoolbox/tools/kaya_idendentiy_decomposition.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     4283 2022-11-18 16:16:07.000000 datatoolbox-0.5.7/datatoolbox/tools/magicc6.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     5931 2022-11-18 16:16:07.000000 datatoolbox-0.5.7/datatoolbox/tools/matplotlib.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     3797 2022-11-18 16:16:07.000000 datatoolbox-0.5.7/datatoolbox/tools/pandas.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     5533 2022-11-18 16:16:07.000000 datatoolbox-0.5.7/datatoolbox/tools/py_magicc_tools.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     7869 2022-11-18 16:16:07.000000 datatoolbox-0.5.7/datatoolbox/tools/pyam.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      965 2022-11-18 16:16:07.000000 datatoolbox-0.5.7/datatoolbox/tools/renaming_DB.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    84992 2019-08-14 10:26:08.000000 datatoolbox-0.5.7/datatoolbox/tools/run_MAGICC_startup_simple.xlsx
+-rwxrwx---   0 root         (0) vboxsf     (999)     1830 2021-02-02 14:03:36.000000 datatoolbox-0.5.7/datatoolbox/tools/run_magicc6.m
+-rwxrwx---   0 root         (0) vboxsf     (999)     1044 2022-11-17 09:58:40.000000 datatoolbox-0.5.7/datatoolbox/tools/statistics.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    61174 2021-06-03 14:06:07.000000 datatoolbox-0.5.7/datatoolbox/tools/test.docx
+-rwxrwx---   0 root         (0) vboxsf     (999)     8625 2022-11-18 16:16:07.000000 datatoolbox-0.5.7/datatoolbox/tools/word.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     9617 2023-03-30 13:29:22.000000 datatoolbox-0.5.7/datatoolbox/tools/xarray.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 12:46:57.000000 datatoolbox-0.5.7/datatoolbox/tutorials/
+-rwxrwx---   0 root         (0) vboxsf     (999)     2996 2022-05-25 07:15:53.000000 datatoolbox-0.5.7/datatoolbox/tutorials/00_search_find_and_access_data.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1019 2020-10-14 14:04:18.000000 datatoolbox-0.5.7/datatoolbox/tutorials/01_emission_comparison.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2096 2022-05-25 07:15:53.000000 datatoolbox-0.5.7/datatoolbox/tutorials/02_unit_conversion.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     5685 2020-10-14 14:04:18.000000 datatoolbox-0.5.7/datatoolbox/tutorials/03_intermediate_example.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1416 2020-10-14 14:04:19.000000 datatoolbox-0.5.7/datatoolbox/tutorials/04_sources.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      382 2020-10-14 14:04:19.000000 datatoolbox-0.5.7/datatoolbox/tutorials/05_plot_source_content.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      734 2020-12-22 15:09:15.000000 datatoolbox-0.5.7/datatoolbox/tutorials/06_xarray_examples.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1142 2021-05-11 13:19:29.000000 datatoolbox-0.5.7/datatoolbox/tutorials/07_renewable_share_compuation.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      793 2021-05-11 12:59:38.000000 datatoolbox-0.5.7/datatoolbox/tutorials/08_low_carbon_fuel_computation.py
+-rwxrwx---   0 root         (0) vboxsf     (999)   137631 2020-10-14 14:04:19.000000 datatoolbox-0.5.7/datatoolbox/tutorials/introduction_v1.ipynb
+-rwxrwx---   0 root         (0) vboxsf     (999)     4631 2022-03-22 14:54:50.000000 datatoolbox-0.5.7/datatoolbox/tutorials/jump_start.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      417 2023-05-12 14:15:39.000000 datatoolbox-0.5.7/datatoolbox/units.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    43915 2022-11-22 09:50:19.000000 datatoolbox-0.5.7/datatoolbox/util.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      176 2023-05-23 12:46:56.000000 datatoolbox-0.5.7/datatoolbox/version.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      746 2022-11-18 16:16:07.000000 datatoolbox-0.5.7/datatoolbox/workflows.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 12:46:57.000000 datatoolbox-0.5.7/datatoolbox.egg-info/
+-rwxrwx---   0 root         (0) vboxsf     (999)     1037 2023-05-23 12:46:57.000000 datatoolbox-0.5.7/datatoolbox.egg-info/PKG-INFO
+-rwxrwx---   0 root         (0) vboxsf     (999)     3714 2023-05-23 12:46:57.000000 datatoolbox-0.5.7/datatoolbox.egg-info/SOURCES.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)        1 2023-05-23 12:46:57.000000 datatoolbox-0.5.7/datatoolbox.egg-info/dependency_links.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)      149 2023-05-23 12:46:57.000000 datatoolbox-0.5.7/datatoolbox.egg-info/requires.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)       12 2023-05-23 12:46:57.000000 datatoolbox-0.5.7/datatoolbox.egg-info/top_level.txt
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 12:46:57.000000 datatoolbox-0.5.7/doc/
+-rwxrwx---   0 root         (0) vboxsf     (999)     7755 2020-10-14 14:04:19.000000 datatoolbox-0.5.7/doc/Makefile
+-rwxrwx---   0 root         (0) vboxsf     (999)     9684 2020-12-22 15:09:15.000000 datatoolbox-0.5.7/doc/conf.py
+-rwxrwx---   0 root         (0) vboxsf     (999)       79 2021-01-05 10:54:01.000000 datatoolbox-0.5.7/doc/core.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)      149 2020-12-22 15:09:15.000000 datatoolbox-0.5.7/doc/data_structures.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)      122 2021-01-11 16:19:59.000000 datatoolbox-0.5.7/doc/database.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)       91 2021-01-11 16:18:53.000000 datatoolbox-0.5.7/doc/database_database.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)      130 2021-01-11 16:21:50.000000 datatoolbox-0.5.7/doc/database_gitrepomanager.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)       93 2021-01-11 16:03:03.000000 datatoolbox-0.5.7/doc/excel.rst
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 12:46:57.000000 datatoolbox-0.5.7/doc/figures/
+-rwxrwx---   0 root         (0) vboxsf     (999)    21579 2020-11-09 13:08:35.000000 datatoolbox-0.5.7/doc/figures/ID_meta_data.svg
+-rwxrwx---   0 root         (0) vboxsf     (999)    67463 2021-05-17 15:08:58.000000 datatoolbox-0.5.7/doc/figures/config_input.png
+-rwxrwx---   0 root         (0) vboxsf     (999)     7157 2021-05-17 15:04:37.000000 datatoolbox-0.5.7/doc/first_steps.md
+-rwxrwx---   0 root         (0) vboxsf     (999)      100 2020-12-22 15:09:15.000000 datatoolbox-0.5.7/doc/foo.rst_template
+-rwxrwx---   0 root         (0) vboxsf     (999)       77 2020-12-22 15:09:15.000000 datatoolbox-0.5.7/doc/help.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)      463 2021-01-11 16:06:28.000000 datatoolbox-0.5.7/doc/index.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)     1754 2021-05-21 08:03:28.000000 datatoolbox-0.5.7/doc/installation.md
+-rwxrwx---   0 root         (0) vboxsf     (999)     1080 2020-12-22 15:09:15.000000 datatoolbox-0.5.7/doc/license.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)     7353 2020-10-14 14:04:19.000000 datatoolbox-0.5.7/doc/make.bat
+-rwxrwx---   0 root         (0) vboxsf     (999)      103 2021-01-11 16:09:22.000000 datatoolbox-0.5.7/doc/matplotlib.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)       95 2021-01-11 16:10:43.000000 datatoolbox-0.5.7/doc/pandas.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)      133 2021-01-11 16:20:57.000000 datatoolbox-0.5.7/doc/tools.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)       95 2021-01-11 16:09:13.000000 datatoolbox-0.5.7/doc/xarray.rst
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 12:46:57.000000 datatoolbox-0.5.7/documentation/
+-rwxrwx---   0 root         (0) vboxsf     (999)     7761 2020-12-22 15:09:15.000000 datatoolbox-0.5.7/documentation/Datatoolbox - First steps.md
+-rwxrwx---   0 root         (0) vboxsf     (999)      385 2023-05-12 12:15:15.000000 datatoolbox-0.5.7/environment.yml
+-rwxrwx---   0 root         (0) vboxsf     (999)      418 2020-10-14 14:04:19.000000 datatoolbox-0.5.7/make_proj.sh
+-rwxrwx---   0 root         (0) vboxsf     (999)      558 2021-01-12 15:45:18.000000 datatoolbox-0.5.7/readthedocs.yml
+-rwxrwx---   0 root         (0) vboxsf     (999)      215 2022-10-19 13:17:33.000000 datatoolbox-0.5.7/requirements.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)       38 2023-05-23 12:46:58.000000 datatoolbox-0.5.7/setup.cfg
+-rwxrwx---   0 root         (0) vboxsf     (999)     1839 2023-05-03 11:16:28.000000 datatoolbox-0.5.7/setup.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-23 12:46:58.000000 datatoolbox-0.5.7/tests/
+-rwxrwx---   0 root         (0) vboxsf     (999)     7292 2022-12-19 11:29:58.000000 datatoolbox-0.5.7/tests/test_calculations.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      696 2022-11-18 16:16:07.000000 datatoolbox-0.5.7/tests/test_converters.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2836 2022-11-21 11:08:31.000000 datatoolbox-0.5.7/tests/test_database.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1640 2023-03-30 13:32:13.000000 datatoolbox-0.5.7/tests/test_dataset.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     7741 2022-05-25 07:15:53.000000 datatoolbox-0.5.7/tests/test_datatable.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1063 2022-11-16 11:59:46.000000 datatoolbox-0.5.7/tests/test_io.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      390 2022-11-22 09:54:34.000000 datatoolbox-0.5.7/tests/test_linked_functions.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1563 2023-05-04 07:49:24.000000 datatoolbox-0.5.7/tests/test_pyam.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     3570 2022-05-25 07:15:53.000000 datatoolbox-0.5.7/tests/test_tableset.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2610 2022-05-25 07:15:53.000000 datatoolbox-0.5.7/tests/test_tools.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1831 2023-05-12 12:19:06.000000 datatoolbox-0.5.7/tests/test_units.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      870 2020-10-14 14:04:19.000000 datatoolbox-0.5.7/tests/test_utilities.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2437 2022-10-19 13:17:33.000000 datatoolbox-0.5.7/tests/test_xarray.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2959 2022-05-25 07:15:53.000000 datatoolbox-0.5.7/tests/util_for_testing.py
```

### Comparing `datatoolbox-0.5.6/.gitlab-ci.yml` & `datatoolbox-0.5.7/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/.travis.yml` & `datatoolbox-0.5.7/.travis.yml`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/LICENSE` & `datatoolbox-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/PKG-INFO` & `datatoolbox-0.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatoolbox
-Version: 0.5.6
+Version: 0.5.7
 Summary: The Python Data Toolbox
 Home-page: https://gitlab.com/climateanalytics/datatoolbox
 Author: Andreas Geiges
 Author-email: a.geiges@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `datatoolbox-0.5.6/README.md` & `datatoolbox-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/appveyor.yml` & `datatoolbox-0.5.7/appveyor.yml`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/ci/appveyor/install.ps1` & `datatoolbox-0.5.7/ci/appveyor/install.ps1`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/ci/appveyor/run_with_env.cmd` & `datatoolbox-0.5.7/ci/appveyor/run_with_env.cmd`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/__init__.py` & `datatoolbox-0.5.7/datatoolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/admin.py` & `datatoolbox-0.5.7/datatoolbox/admin.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/config.py` & `datatoolbox-0.5.7/datatoolbox/config.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/converters.py` & `datatoolbox-0.5.7/datatoolbox/converters.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,14 +119,21 @@
     for table in table_iterable:
 
         for dim in dimensions:
 
             dims[dim] = dims.get(dim, set()).union(_get_unique_labels(table, dim))
     return dims
 
+def _get_stacked_levels(index, st_dim, sub_dims):
+    df = index.to_frame()
+    # for st_dim, sub_dims in stacked_dims.items():
+    df[st_dim] = df.loc[:, sub_dims].agg('__'.join, axis=1)
+    df = df.set_index([st_dim] + list(sub_dims))
+    return df.index.codes[0], df.index.levels[0]
+
 
 def _to_xarray(tables, dimensions, stacked_dims):
     """
     Return a database query result as an xarray . This constuctor allows only for
     one unit, since the full array is quantified using pint-xarray.
     The xarray dimensions (coordiantes) are defined
     by the provided dimensions. A multi-index for a coordinate can be created
@@ -299,15 +306,43 @@
     wdf['variable'] = xarr.name
     wdf['unit'] = str(xarr.pint.units)
     wdf.set_index('variable', append=True, inplace=True)
     wdf.set_index('unit', append=True, inplace=True)
     wdf.columns = wdf.columns.droplevel(0)
     return wdf
 
+#%% Public functions
 
+def multi_index_df_to_datatables(df, index_col_name = 'region'):
+    #%%
+    if not index_col_name in df.index.names:
+        raise(Exception(f'New index columns name {index_col_name} must be in mult-index'))
+    groupby_levels = [x for x in df.index.names if x != index_col_name]
+    
+    tables =  list()
+    for idx, sub_df in df.groupby(groupby_levels):
+        
+        table = dt.Datatable.from_multi_indexed_dataframe(sub_df)
+        tables.append(table)
+    return tables
+    #%%
+
+def datatables_to_multi_index_df(tables,
+                                 exclude_meta =['ID', 'creator', 'source_name','source_year'],
+                                 use_index_names = None):
+    
+    dfs = list()
+    for table in tables:
+        dfs.append(table.to_multi_index_dataframe(exclude_meta=exclude_meta,
+                                                  use_index_names=use_index_names))
+    index_names = set([x.index.names for x in dfs])
+    if len(index_names) > 1:
+        raise(Exception(f'Index level names do not aligen, please check: {index_names}'))
+    return pd.concat(dfs)
+    
 def to_pyam(data):
     """
     Converts known data tyes to a tableset. Recognized data types are:
         - xarray.Dataset
 
     Parameters
     ----------
@@ -439,20 +474,14 @@
             tables.add(table)
 
         return tables
     else:
         raise (Exception(f'{type(data)} is not implemented'))
 
 
-def _get_stacked_levels(index, st_dim, sub_dims):
-    df = index.to_frame()
-    # for st_dim, sub_dims in stacked_dims.items():
-    df[st_dim] = df.loc[:, sub_dims].agg('__'.join, axis=1)
-    df = df.set_index([st_dim] + list(sub_dims))
-    return df.index.codes[0], df.index.levels[0]
 
 
 def idf_to_xdset(idf, stacked_dims={'pathway': ('model', 'scenario')}):
 
     df_ = idf._data.unstack(level=['variable', 'unit'])
     # df_.drop([])
     coords_flatten = []
@@ -550,49 +579,22 @@
         ds = idf_to_xdset(data, stacked_dims)
         return ds
 
     else:
         raise (Exception(f'Data type {type(data)} conversion not implemented'))
 
 
-#%%
-# idf = dt.findp(source='IPCC_AR6', variable = 'Secondary Energy|Heat|Geothermal').as_pyam()
-# #%%
-# tt = time()
-# ds1 = idf_to_xdset(idf, stacked_dims={'pathway': ('model', 'scenario')})
-# print(time()-tt)
-
-# tt = time()
-# ds2 = to_xdataset(idf, stacked_dims={'pathway': ('model', 'scenario')})
-# print(time()-tt)
 
 
 #%%
 if __name__ == '__main__':
 
-    #%test
+    
     import datatoolbox as dt
 
-    # local_data_file = '/media/sf_Documents/python/ca_data_management/data/IPCC_AR6/AR6_Scenarios_Database_World_v1.0.csv'#,
-    # data = pd.read_csv(local_data_file)
-    # dimensions = ['Model', 'Scenario', 'Region', 'year']
-    # stacked_dims = {'Pathway': ('Model', 'Scenario'),
-    #                 'varunit' : ("Variable", "Unit")}
-    # data = data.set_index(data.columns[:5].tolist()).rename_axis(columns= 'year').stack()
-
-    # from datatoolbox.tools.pyam import idf_to_xarray
-
-    # xds = idf_to_xarray(data, stacked_dims= stacked_dims)
-
-    # tbs = dt.getTables(dt.find(source='IAMC15_2019_R2').index[:10])
-    # idf = tbs.to_IamDataFrame()
-    # # xda = idf_to_xarray(idf)
-    # stacked_dims= {'pathway': ('model', 'scenario')}
-
-    # index, labels = _pack_dimensions(idf.index, **stacked_dims)
     xdata = dt.findp(
         variable=[
             'Emissions|CO2|Energy|Supply|Electricity',
             'Secondary Energy|Electricity',
         ],
         source='IPCC_SR15',
         pathway='**SSP1-19**',
```

### Comparing `datatoolbox-0.5.6/datatoolbox/core.py` & `datatoolbox-0.5.7/datatoolbox/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,31 +18,34 @@
 from datatoolbox import naming_convention
 
 tt = time.time()
 
 #%% Pint unit handling
 gases = {
     "CO2eq": "carbon_dioxide_equivalent",
-    "CO2e": "CO2eq",
+    # "CO2e": "CO2eq",
     "NO2": "NO2",
     'PM25': 'PM25',
 }
 
 from openscm_units import unit_registry as ur
 
 
 try:
+    
     ur._add_gases(gases)
+    
     ur.define('fraction = [] = frac')
     ur.define('percent = 1e-2 frac = pct')
     ur.define('ppm = 1e-6 fraction')
     ur.define('sqkm = km * km')
     ur.define('none = dimensionless')
 
     ur.load_definitions(config.PATH_PINT_DEFINITIONS)
+    ur.define('CO2eq = CO2')
 except pint.errors.DefinitionSyntaxError:
     # avoid double import of units defintions
     pass
 
 import pint
 
 #
@@ -277,15 +280,15 @@
     """
     if (config.OS == 'win32') | (config.OS == "Windows"):
         return True
     else:
         return False
 
 
-def getUnit(string):
+def getUnit(string, ur=ur):
     """
     Return the pint unit for a given unit string. Compared to the original
     pint this functions replaces special characters $ € and % by a string
     reprentation.
 
     Parameters
     ----------
@@ -379,23 +382,32 @@
 
     Returns
     -------
     TYPE
         DESCRIPTION.
 
     """
+    
+    if context == 'GWPAR4':
+        import warnings
+        warnings.warn('The context "AR4GWP" is depricated. Pleases use "AR4GWP100" instead')
+        context = "AR4GWP100"
     if context is None:
         return getUnit(unitFrom).to(getUnit(unitTo)).m
-    elif context == 'GWPAR4':
+    # elif context == 'GWPAR4':
 
-        return _AR4_conversionFactor(unitFrom, unitTo)
-
-    else:
-        raise (BaseException('unkown context'))
+    #     return _AR4_conversionFactor(unitFrom, unitTo)
 
+    # else:
+    #     raise (BaseException('unkown context'))
+    else:   
+        with ur.context(context) as urc:
+            factor =getUnit(unitFrom, ur=urc).to(getUnit(unitTo, ur=urc))
+            
+        return factor.m
 
 def _findGases(string, candidateList):
     hits = list()
     for key in candidateList:
         if key in string:
             hits.append(key)
             string = string.replace(key, '')
```

### Comparing `datatoolbox-0.5.6/datatoolbox/data/GHG_alternative_naming.pkl` & `datatoolbox-0.5.7/datatoolbox/data/GHG_alternative_naming.pkl`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/data/GHG_properties_2019_CA.csv` & `datatoolbox-0.5.7/datatoolbox/data/GHG_properties_2019_CA.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/data/SANDBOX_datashelf/mappings/continent.csv` & `datatoolbox-0.5.7/datatoolbox/data/SANDBOX_datashelf/mappings/continent.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/data/SANDBOX_datashelf/mappings/country_codes.csv` & `datatoolbox-0.5.7/datatoolbox/data/SANDBOX_datashelf/mappings/country_codes.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/data/SANDBOX_datashelf/mappings/regions.csv` & `datatoolbox-0.5.7/datatoolbox/data/SANDBOX_datashelf/mappings/regions.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/data/all.csv` & `datatoolbox-0.5.7/datatoolbox/data/all.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/data/compatible1_5_unfiltered.xlsx` & `datatoolbox-0.5.7/datatoolbox/data/compatible1_5_unfiltered.xlsx`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/data/continent.csv` & `datatoolbox-0.5.7/datatoolbox/data/continent.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/data/country_codes.csv` & `datatoolbox-0.5.7/datatoolbox/data/country_codes.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/data/datashelf_contents.csv` & `datatoolbox-0.5.7/datatoolbox/data/datashelf_contents.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/data/external_mappings.py` & `datatoolbox-0.5.7/datatoolbox/data/external_mappings.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/data/regions.csv` & `datatoolbox-0.5.7/datatoolbox/data/regions.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/data_readers.py` & `datatoolbox-0.5.7/datatoolbox/data_readers.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/data_structures.py` & `datatoolbox-0.5.7/datatoolbox/data_structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     ^^^^^^^^^
 
     Datatable is derrived from pandas dataframe.
     """
 
     _metadata = ['meta', 'ID', 'attrs']
 
+    #%% magicc methods
     def __init__(self, *args, **kwargs):
 
         # pop meta out of kwargs since pandas is not expecting it
         overwrite_meta = kwargs.pop(
             'meta', {}
         )  # return empty dict if no meta is provide
 
@@ -74,17 +75,360 @@
         if ('_timeformat' in self.meta.keys()) and (
             self.meta['_timeformat'] != '%Y' and self.meta['_timeformat'] != 'Y'
         ):
             self.columns_to_datetime()
 
         self.attrs = self.meta
 
+    def __add__(self, other):
+       """
+       Private function to add two dataframes. The added table is converted to
+       the unit of first table.
+
+       Parameters
+       ----------
+       other : datatble
+           Data to add.
+
+       Returns
+       -------
+       out : datatable
+           DESCRIPTION.
+
+       """
+       if isinstance(other, (Datatable, pint.Quantity)):
+             
+           if self.meta['unit'] == other.units:
+               factor = 1
+           else:
+               factor = core.getUnit(other.units).to(self.meta['unit']).m
+           if isinstance(other, pint.Quantity):
+               rhs = other.m
+           else:
+               rhs = pd.DataFrame(other * factor)
+           out = Datatable(super(Datatable, self.copy()).__add__(rhs))
+
+           out.meta['unit'] = self.meta['unit']
+           out.meta['source'] = 'calculation'
+           
+       # elif isinstance(ur(df1.meta['unit']),pint.Quantity):
+           
+       else:
+           out = Datatable(super(Datatable, self).__add__(other))
+           out.meta['unit'] = self.meta['unit']
+           out.meta['source'] = 'calculation'
+       return out
+
+    __radd__ = __add__
+
+
+
+    def __finalize__(self, other, method=None, **kwargs):
+        """propagate metadata from other to self"""
+        # merge operation: using metadata of the left object
+        if method == 'merge':
+            for name in self._metadata:
+                object.__setattr__(self, name, copy(getattr(other.left, name, None)))
+        # concat operation: using metadata of the first object
+        elif method == 'concat':
+            for name in self._metadata:
+                object.__setattr__(self, name, copy(getattr(other.objs[0], name, None)))
+        else:
+            for name in self._metadata:
+                # print(other)
+                object.__setattr__(self, name, copy(getattr(other, name, None)))
+        return self
+
+    def __appendMetaData__(self, metaDict):
+        """
+        Private function to append meta data.
+
+        Parameters
+        ----------
+        metaDict : dict
+            New meta data.
+
+
+        """
+
+        for metaKey in config.REQUIRED_META_FIELDS:
+            if (
+                metaKey not in metaDict.keys()
+                or metaDict[metaKey] == ''
+                or pd.isna(metaDict[metaKey])
+            ):
+
+                # Overwrite with default or empty string
+                if metaKey in config.META_DEFAULTS:
+                    metaDict[metaKey] = config.META_DEFAULTS[metaKey]
+                else:
+                    metaDict[metaKey] = ''
+
+        self.__setattr__('meta', metaDict.copy())
+
+        assert core.getUnit(self.meta['unit'])
+        
+    def __sub__(self, other):
+       """
+       Private function to subract two dataframes. The subracted table is converted to
+       the unit of first table.
+
+       Parameters
+       ----------
+       other : datatble
+           Data to substract.
+
+       Returns
+       -------
+       out : datatable
+           DESCRIPTION.
+
+       """
+       if isinstance(other, (Datatable, pint.Quantity)):
+           if self.meta['unit'] == other.units:
+               factor = 1
+           else:
+               factor = core.getUnit(other.units).to(self.meta['unit']).m
+           if isinstance(other, pint.Quantity):
+               rhs = other.m
+           else:
+               rhs = pd.DataFrame(other * factor)
+           out = Datatable(super(Datatable, self).__sub__(rhs))
+           out.meta['unit'] = self.meta['unit']
+           out.meta['source'] = 'calculation'
+       else:
+           out = Datatable(super(Datatable, self).__sub__(other))
+           out.meta['unit'] = self.meta['unit']
+           out.meta['source'] = 'calculation'
+       return out
+
+    def __rsub__(self, other):
+       """
+       Equivalent to __sub__
+       """
+       if isinstance(other, (Datatable, pint.Quantity)):
+           if self.meta['unit'] == other.units:
+               factor = 1
+           else:
+               factor = core.getUnit(other.units).to(self.meta['unit']).m
+           if isinstance(other, pint.Quantity):
+               other = other.m
+           out = Datatable(super(Datatable, self).__rsub__(other * factor))
+           out.meta['unit'] = self.meta['unit']
+           out.meta['source'] = 'calculation'
+       else:
+           out = Datatable(super(Datatable, self).__rsub__(other))
+           out.meta['unit'] = self.meta['unit']
+           out.meta['source'] = 'calculation'
+       return out
+
+    def __mul__(self, other):
+       if isinstance(other, (Datatable, pint.Quantity)):
+           newUnit = core.getUnit(self.meta['unit']) * core.getUnit(other.units)
+           if isinstance(other, pint.Quantity):
+               other = other.m
+           out = Datatable(super(Datatable, self).__mul__(other))
+           out.meta['unit'] = str(newUnit.u)
+           out.meta['source'] = 'calculation'
+           out.values[:] *= newUnit.m
+       else:
+           out = Datatable(super(Datatable, self).__mul__(other))
+           out.meta['unit'] = self.meta['unit']
+           out.meta['source'] = 'calculation'
+       return out
+
+    __rmul__ = __mul__
+
+    def __truediv__(self, other):
+       if isinstance(other, (Datatable, pint.Quantity)):
+           newUnit = core.getUnit(self.meta['unit']) / core.getUnit(other.units)
+           if isinstance(other, pint.Quantity):
+               other = other.m
+           out = Datatable(super(Datatable, self).__truediv__(other))
+           out.meta['unit'] = str(newUnit.u)
+           out.meta['source'] = 'calculation'
+           out.values[:] *= newUnit.m
+       else:
+           out = Datatable(super(Datatable, self).__truediv__(other))
+           out.meta['unit'] = self.meta['unit']
+           out.meta['source'] = 'calculation'
+       return out
+
+    #    __rtruediv__ = __truediv__
+    def __rtruediv__(self, other):
+       if isinstance(other, (Datatable, pint.Quantity)):
+           newUnit = core.getUnit(other.units) / core.getUnit(self.meta['unit'])
+           if isinstance(other, pint.Quantity):
+               other = other.m
+           out = Datatable(super(Datatable, self).__rtruediv__(other))
+           out.meta['unit'] = str(newUnit.u)
+           out.meta['source'] = 'calculation'
+           out.values[:] *= newUnit.m
+       else:
+           out = Datatable(super(Datatable, self).__rtruediv__(other))
+           out.meta['unit'] = str((core.getUnit(self.meta['unit']) ** -1).u)
+           out.meta['source'] = 'calculation'
+       return out
+
+    def __repr__(self):
+       outStr = """"""
+       if 'ID' in self.meta.keys():
+           outStr += '=== Datatable - ' + self.meta['ID'] + ' ===\n'
+       else:
+           outStr += '=== Datatable ===\n'
+       for key in self.meta.keys():
+           if self.meta[key] is not None and not str(self.meta[key]).startswith('_'):
+               outStr += key + ': ' + str(self.meta[key]) + ' \n'
+       outStr += super(Datatable, self).__repr__()
+       return outStr
+
+    def _repr_html_(self):
+       outStr = """"""
+       if 'ID' in self.meta.keys():
+           outStr += '=== Datatable - ' + self.meta['ID'] + ' ===<br/>\n'
+       else:
+           outStr += '=== Datatable ===<br/>\n'
+       for key in self.meta.keys():
+           if self.meta[key] is not None and not str(self.meta[key]).startswith('_'):
+               outStr += key + ': ' + str(self.meta[key]) + ' <br/>\n'
+       outStr += super(Datatable, self)._repr_html_()
+       return outStr
+
+    #%% private methods
+    @property
+    def _constructor(self):
+        return Datatable
+    
+    def _to_xarray(self):
+
+        return core.xr.DataArray(
+            self.values,
+            coords=[self.index, self.columns],
+            dims=['space', 'time'],
+            attrs=self.meta,
+        )
+    def _update_meta(self):
+        self.meta = core._update_meta(self.meta)
+
+    #%% public methods
+    
+    def aggregate_region(self, mapping, skipna=False):
+        """
+        This functions added the aggregates to the table according to the provided
+        mapping.( See datatools.mapp.regions)
+
+        Returns the result, but does not inplace add it.
+        """
+        from datatoolbox.tools.for_datatables import aggregate_region
+
+        return aggregate_region(self, mapping, skipna)
+    
+    def append(self, other, **kwargs):
+        """
+        Append data to the datatable
+
+
+        Parameters
+        ----------
+        other : datatable
+            New data that will be added to the datatable.
+        **kwargs : TYPE
+            Default pandas append arguments.
+
+        Returns
+        -------
+        datatable
+
+        """
+        kwargs.setdefault("sort", True)
+
+        if isinstance(other, Datatable):
+
+            if other.meta['entity'] != self.meta['entity']:
+                #                print(other.meta['entity'] )
+                #                print(self.meta['entity'])
+                raise (BaseException('Physical entities do not match, please correct'))
+            if other.units != self.meta['unit']:
+                other = other.convert(self.meta['unit'])
+
+        out = pd.concat([self, other], **kwargs)
+
+        # only copy required keys
+        out.meta = {
+            key: value
+            for key, value in self.meta.items()
+            if key in config.REQUIRED_META_FIELDS
+        }
+
+        # overwrite scenario
+        out.meta['scenario'] = (
+            'computed: ' + self.meta['scenario'] + '+' + other.meta['scenario']
+        )
+        return out
+    
+    def clean(self):
+        """
+        Clean up the dataframe to only recogniszed regions, years and numeric values.
+        Removed columns and rows with only nan values.
+
+        Returns
+        -------
+        datatable
+            DESCRIPTION.
+
+        """
+        return util.cleanDataTable(self)
+    
+    def copy(self, deep=True):
+        """
+        Make a copy of this Datatable object
+        Parameters
+        ----------
+        deep : boolean, default True
+            Make a deep copy, i.e. also copy data
+        Returns
+        -------
+        copy : Datatable
+        """
+        # FIXME: this will likely be unnecessary in pandas >= 0.13
+        data = self._data
+        if deep:
+            data = data.copy(deep=True)
+        return Datatable(data).__finalize__(self)
+    
+    def columns_to_datetime(self):
+        self.columns = pd.to_datetime(self.columns, format=self.meta['_timeformat'])
+    
+
+    def diff(self, periods=1, axis=0):
+        """
+        Compute the difference between different years in the datatable
+        Equivalent do pandas diff but return datatable.
+
+        Parameters
+        ----------
+        periods : int, optional
+            DESCRIPTION. The default is 1.
+        axis : int, optional
+            DESCRIPTION. The default is 0.
+
+        Returns
+        -------
+        out : TYPE
+            DESCRIPTION.
+
+        """
+        out = super(Datatable, self).diff(periods=periods, axis=axis)
+        out.meta['unit'] = self.meta['unit']
+
+        return out    
     @property
     def units(self):
         return self.meta['unit']
+    
     def info(self):
         """
         Returns information about the dataframe like shape, index and column
         extend and the number of non-nan entries.
 
         Returns
         -------
@@ -97,14 +441,25 @@
             return 'Empty Datatable'
         idx_ext = self.index[0], self.index[-1]
         time_ext = self.columns[0], self.columns[-1]
         n_entries = (~self.isnull()).sum().sum()
         return f'{shp[0]}x{shp[1]} Datatable with {n_entries} entries, index from {idx_ext[0]} to {idx_ext[1]} and time from {time_ext[0]} to {time_ext[0]}'
 
     @classmethod
+    def from_multi_indexed_dataframe(cls, df):
+        #find unique index
+        idx_ames_to_meta = [x for x in df.index.names if (len(df.index.unique(x)) ==1) and x !='region']
+        table = cls(df.copy())
+        table.meta = {x : df.index.unique(x)[0] for x in idx_ames_to_meta}
+        table.index = table.index.droplevel(idx_ames_to_meta)
+        return table
+    
+    
+    
+    @classmethod
     def from_pyam(cls, idf, **kwargs):
         """
         Create a datatable from an iam dataframe.
 
         Parameters
         ----------
         cls : datatable class
@@ -177,114 +532,19 @@
         """
         if sheetName is None:
             sheetNames = None
         else:
             sheetNames = [sheetNames]
         return read_excel(filepath, sheetNames=sheetNames)
 
-    def _to_xarray(self):
-
-        return core.xr.DataArray(
-            self.values,
-            coords=[self.index, self.columns],
-            dims=['space', 'time'],
-            attrs=self.meta,
-        )
-
-    @property
-    def _constructor(self):
-        return Datatable
-
-    def __finalize__(self, other, method=None, **kwargs):
-        """propagate metadata from other to self"""
-        # merge operation: using metadata of the left object
-        if method == 'merge':
-            for name in self._metadata:
-                object.__setattr__(self, name, copy(getattr(other.left, name, None)))
-        # concat operation: using metadata of the first object
-        elif method == 'concat':
-            for name in self._metadata:
-                object.__setattr__(self, name, copy(getattr(other.objs[0], name, None)))
-        else:
-            for name in self._metadata:
-                # print(other)
-                object.__setattr__(self, name, copy(getattr(other, name, None)))
-        return self
-
-    def __appendMetaData__(self, metaDict):
-        """
-        Private function to append meta data.
+    
 
-        Parameters
-        ----------
-        metaDict : dict
-            New meta data.
 
 
-        """
 
-        for metaKey in config.REQUIRED_META_FIELDS:
-            if (
-                metaKey not in metaDict.keys()
-                or metaDict[metaKey] == ''
-                or pd.isna(metaDict[metaKey])
-            ):
-
-                # Overwrite with default or empty string
-                if metaKey in config.META_DEFAULTS:
-                    metaDict[metaKey] = config.META_DEFAULTS[metaKey]
-                else:
-                    metaDict[metaKey] = ''
-
-        self.__setattr__('meta', metaDict.copy())
-
-        assert core.getUnit(self.meta['unit'])
-
-    def columns_to_datetime(self):
-        self.columns = pd.to_datetime(self.columns, format=self.meta['_timeformat'])
-
-    def copy(self, deep=True):
-        """
-        Make a copy of this Datatable object
-        Parameters
-        ----------
-        deep : boolean, default True
-            Make a deep copy, i.e. also copy data
-        Returns
-        -------
-        copy : Datatable
-        """
-        # FIXME: this will likely be unnecessary in pandas >= 0.13
-        data = self._data
-        if deep:
-            data = data.copy(deep=True)
-        return Datatable(data).__finalize__(self)
-
-    def diff(self, periods=1, axis=0):
-        """
-        Compute the difference between different years in the datatable
-        Equivalent do pandas diff but return datatable.
-
-        Parameters
-        ----------
-        periods : int, optional
-            DESCRIPTION. The default is 1.
-        axis : int, optional
-            DESCRIPTION. The default is 0.
-
-        Returns
-        -------
-        out : TYPE
-            DESCRIPTION.
-
-        """
-        out = super(Datatable, self).diff(periods=periods, axis=axis)
-        out.meta['unit'] = self.meta['unit']
-
-        return out
 
     def reduce(self, method='linear_piece_wise', eps=1e-6):
         """
         Reduce data that is piecewise linear to the core data points (kinks).
         """
 
         # assert monotonic incease of decrease
@@ -449,15 +709,41 @@
 
     def to_IamDataFrame(self, **kwargs):
         """
         Function to sustain backwars compatibility
         Depreciated.
 
         """
+        
         return self.to_pyam(**kwargs)
+        
+    def to_multi_index_dataframe(self, 
+                            exclude_meta =['ID', 'creator', 'source_name','source_year'],
+                            use_index_names = None):
+        """
+        Return a new datatable with a mult-index that has all meta data assigned
+        
+        Parameters
+        -------
+        exclude_meta: optinal list of meta keys that should be ignored
+        Returns
+        -------
+        Datatable
+            New Datatable with multi_index and not meta data.
+
+        """
+ 
+        from pandas_indexing import assignlevel
+        
+        if use_index_names is None:
+            meta_for_index = {x: self.meta[x] for x in sorted(self.meta.keys()) if not x in exclude_meta}
+        else:
+            meta_for_index = {x: self.meta[x] for x in sorted(use_index_names) if x!='region' }
+        
+        return assignlevel(self, **meta_for_index)
 
     def convert(self, newUnit, context=None):
         """
         Convert datatable to different unit and returns converted
         datatable.
 
         Parameters
@@ -483,24 +769,14 @@
         factor = core.conversionFactor(self.meta['unit'], newUnit, context)
 
         dfNew.loc[:] = self.values * factor
         dfNew.meta['unit'] = newUnit
         dfNew.meta['modified'] = core.get_time_string()
         return dfNew
 
-    def aggregate_region(self, mapping, skipna=False):
-        """
-        This functions added the aggregates to the table according to the provided
-        mapping.( See datatools.mapp.regions)
-
-        Returns the result, but does not inplace add it.
-        """
-        from datatoolbox.tools.for_datatables import aggregate_region
-
-        return aggregate_region(self, mapping, skipna)
 
     def interpolate(self, method="linear", add_missing_years=False):
         """
         Interpoltate missing data between year with the option to add
         missing years in the columns.
 
         Parameters
@@ -524,26 +800,15 @@
             for col in list(range(self.columns.min(), self.columns.max() + 1)):
                 if col not in self.columns:
                     self.loc[:, col] = np.nan
             self = self.loc[:, list(range(self.columns.min(), self.columns.max() + 1))]
 
         return interpolate(self, method)
 
-    def clean(self):
-        """
-        Clean up the dataframe to only recogniszed regions, years and numeric values.
-        Removed columns and rows with only nan values.
-
-        Returns
-        -------
-        datatable
-            DESCRIPTION.
 
-        """
-        return util.cleanDataTable(self)
 
     def filter(self, spaceIDs):
         """
         Filter dataframe based on a list of spatial IDs.
 
         Parameters
         ----------
@@ -633,233 +898,24 @@
         For compatibility to windows based sytems, the pipe '|' symbols is replaces
         by double underscore '__' for the csv filename.
         """
         self.generateTableID()
 
         return core.generate_table_file_name(self.ID)
 
-    def _update_meta(self):
-        self.meta = core._update_meta(self.meta)
 
     def source(self):
         """
         Return the source of the table
         """
         return self.meta['source']
 
-    def append(self, other, **kwargs):
-        """
-        Append data to the datatable
-
-
-        Parameters
-        ----------
-        other : datatable
-            New data that will be added to the datatable.
-        **kwargs : TYPE
-            Default pandas append arguments.
-
-        Returns
-        -------
-        datatable
-
-        """
-        kwargs.setdefault("sort", True)
-
-        if isinstance(other, Datatable):
-
-            if other.meta['entity'] != self.meta['entity']:
-                #                print(other.meta['entity'] )
-                #                print(self.meta['entity'])
-                raise (BaseException('Physical entities do not match, please correct'))
-            if other.units != self.meta['unit']:
-                other = other.convert(self.meta['unit'])
-
-        out = pd.concat([self, other], **kwargs)
-
-        # only copy required keys
-        out.meta = {
-            key: value
-            for key, value in self.meta.items()
-            if key in config.REQUIRED_META_FIELDS
-        }
-
-        # overwrite scenario
-        out.meta['scenario'] = (
-            'computed: ' + self.meta['scenario'] + '+' + other.meta['scenario']
-        )
-        return out
-
-    def __add__(self, other):
-        """
-        Private function to add two dataframes. The added table is converted to
-        the unit of first table.
-
-        Parameters
-        ----------
-        other : datatble
-            Data to add.
-
-        Returns
-        -------
-        out : datatable
-            DESCRIPTION.
-
-        """
-        if isinstance(other, (Datatable, pint.Quantity)):
-              
-            if self.meta['unit'] == other.units:
-                factor = 1
-            else:
-                factor = core.getUnit(other.units).to(self.meta['unit']).m
-            if isinstance(other, pint.Quantity):
-                rhs = other.m
-            else:
-                rhs = pd.DataFrame(other * factor)
-            out = Datatable(super(Datatable, self.copy()).__add__(rhs))
-
-            out.meta['unit'] = self.meta['unit']
-            out.meta['source'] = 'calculation'
-            
-        # elif isinstance(ur(df1.meta['unit']),pint.Quantity):
-            
-        else:
-            out = Datatable(super(Datatable, self).__add__(other))
-            out.meta['unit'] = self.meta['unit']
-            out.meta['source'] = 'calculation'
-        return out
-
-    __radd__ = __add__
-
-    def __sub__(self, other):
-        """
-        Private function to subract two dataframes. The subracted table is converted to
-        the unit of first table.
-
-        Parameters
-        ----------
-        other : datatble
-            Data to substract.
-
-        Returns
-        -------
-        out : datatable
-            DESCRIPTION.
-
-        """
-        if isinstance(other, (Datatable, pint.Quantity)):
-            if self.meta['unit'] == other.units:
-                factor = 1
-            else:
-                factor = core.getUnit(other.units).to(self.meta['unit']).m
-            if isinstance(other, pint.Quantity):
-                rhs = other.m
-            else:
-                rhs = pd.DataFrame(other * factor)
-            out = Datatable(super(Datatable, self).__sub__(rhs))
-            out.meta['unit'] = self.meta['unit']
-            out.meta['source'] = 'calculation'
-        else:
-            out = Datatable(super(Datatable, self).__sub__(other))
-            out.meta['unit'] = self.meta['unit']
-            out.meta['source'] = 'calculation'
-        return out
-
-    def __rsub__(self, other):
-        """
-        Equivalent to __sub__
-        """
-        if isinstance(other, (Datatable, pint.Quantity)):
-            if self.meta['unit'] == other.units:
-                factor = 1
-            else:
-                factor = core.getUnit(other.units).to(self.meta['unit']).m
-            if isinstance(other, pint.Quantity):
-                other = other.m
-            out = Datatable(super(Datatable, self).__rsub__(other * factor))
-            out.meta['unit'] = self.meta['unit']
-            out.meta['source'] = 'calculation'
-        else:
-            out = Datatable(super(Datatable, self).__rsub__(other))
-            out.meta['unit'] = self.meta['unit']
-            out.meta['source'] = 'calculation'
-        return out
-
-    def __mul__(self, other):
-        if isinstance(other, (Datatable, pint.Quantity)):
-            newUnit = core.getUnit(self.meta['unit']) * core.getUnit(other.units)
-            if isinstance(other, pint.Quantity):
-                other = other.m
-            out = Datatable(super(Datatable, self).__mul__(other))
-            out.meta['unit'] = str(newUnit.u)
-            out.meta['source'] = 'calculation'
-            out.values[:] *= newUnit.m
-        else:
-            out = Datatable(super(Datatable, self).__mul__(other))
-            out.meta['unit'] = self.meta['unit']
-            out.meta['source'] = 'calculation'
-        return out
-
-    __rmul__ = __mul__
-
-    def __truediv__(self, other):
-        if isinstance(other, (Datatable, pint.Quantity)):
-            newUnit = core.getUnit(self.meta['unit']) / core.getUnit(other.units)
-            if isinstance(other, pint.Quantity):
-                other = other.m
-            out = Datatable(super(Datatable, self).__truediv__(other))
-            out.meta['unit'] = str(newUnit.u)
-            out.meta['source'] = 'calculation'
-            out.values[:] *= newUnit.m
-        else:
-            out = Datatable(super(Datatable, self).__truediv__(other))
-            out.meta['unit'] = self.meta['unit']
-            out.meta['source'] = 'calculation'
-        return out
-
-    #    __rtruediv__ = __truediv__
-    def __rtruediv__(self, other):
-        if isinstance(other, (Datatable, pint.Quantity)):
-            newUnit = core.getUnit(other.units) / core.getUnit(self.meta['unit'])
-            if isinstance(other, pint.Quantity):
-                other = other.m
-            out = Datatable(super(Datatable, self).__rtruediv__(other))
-            out.meta['unit'] = str(newUnit.u)
-            out.meta['source'] = 'calculation'
-            out.values[:] *= newUnit.m
-        else:
-            out = Datatable(super(Datatable, self).__rtruediv__(other))
-            out.meta['unit'] = str((core.getUnit(self.meta['unit']) ** -1).u)
-            out.meta['source'] = 'calculation'
-        return out
-
-    def __repr__(self):
-        outStr = """"""
-        if 'ID' in self.meta.keys():
-            outStr += '=== Datatable - ' + self.meta['ID'] + ' ===\n'
-        else:
-            outStr += '=== Datatable ===\n'
-        for key in self.meta.keys():
-            if self.meta[key] is not None and not str(self.meta[key]).startswith('_'):
-                outStr += key + ': ' + str(self.meta[key]) + ' \n'
-        outStr += super(Datatable, self).__repr__()
-        return outStr
-
-    def _repr_html_(self):
-        outStr = """"""
-        if 'ID' in self.meta.keys():
-            outStr += '=== Datatable - ' + self.meta['ID'] + ' ===<br/>\n'
-        else:
-            outStr += '=== Datatable ===<br/>\n'
-        for key in self.meta.keys():
-            if self.meta[key] is not None and not str(self.meta[key]).startswith('_'):
-                outStr += key + ': ' + str(self.meta[key]) + ' <br/>\n'
-        outStr += super(Datatable, self)._repr_html_()
-        return outStr
+    
 
+ 
 
 
 class TableSet(dict):
     """
     Class TableSet that is inherited from the dict class. It organized multiple
     heterogeneous datatbles into one structure.
     """
```

### Comparing `datatoolbox-0.5.6/datatoolbox/database.py` & `datatoolbox-0.5.7/datatoolbox/database.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/greenhouse_gas_database.py` & `datatoolbox-0.5.7/datatoolbox/greenhouse_gas_database.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/init_tools.py` & `datatoolbox-0.5.7/datatoolbox/init_tools.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/interfaces.py` & `datatoolbox-0.5.7/datatoolbox/interfaces.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/io_tools.py` & `datatoolbox-0.5.7/datatoolbox/io_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 import re
 import os
 import pandas as pd
 import numpy as np
 from tqdm import tqdm
 import deprecated as dp
+import numpy as np
 
 from . import config
 
 from . import core
 from . import util
 from . import mapping as mapp
 from .tools.pandas import yearsColumnsOnly
@@ -99,17 +100,17 @@
 
     firstDataRow = allDf.loc['SHEET_FIRSTDATAROW', 'Unnamed: 1']
 
     # bugfix of old wrong formated PRIMAP files
     try:
         int(firstDataRow)
     except:
-        firstDataRow = pd.np.where(allDf.index == "Countries\Years")[0][0] + 3
+        firstDataRow = np.where(allDf.index == "Countries\Years")[0][0] + 3
 
-    firstMetaRow = pd.np.where(allDf.index == "&SHEET_SPECIFICATIONS")[0][0] + 1
+    firstMetaRow = np.where(allDf.index == "&SHEET_SPECIFICATIONS")[0][0] + 1
 
     metaPrimap = dict()
     for row in range(firstMetaRow, firstDataRow):
         key = allDf.index[row]
         value = allDf.iloc[row, 0]
         if key == '/':
             break
@@ -163,15 +164,15 @@
 
     firstDataRow = allDf.loc['SHEET_FIRSTDATAROW', 'Unnamed: 1']
 
     # bugfix of old wrong formated PRIMAP files
     try:
         int(firstDataRow)
     except:
-        firstDataRow = pd.np.where(allDf.index == "Countries\Years")[0][0] + 3
+        firstDataRow = np.where(allDf.index == "Countries\Years")[0][0] + 3
 
     # print(firstDataRow)
     setup = dict()
     setup['filePath'] = os.path.dirname(fileName) + '/'
     setup['fileName'] = os.path.basename(fileName)
     setup['sheetName'] = sheet_name
     setup['timeIdxList'] = ('B' + str(firstDataRow - 1), 'XX' + str(firstDataRow - 1))
```

### Comparing `datatoolbox-0.5.6/datatoolbox/mapping.py` & `datatoolbox-0.5.7/datatoolbox/mapping.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/naming_convention.py` & `datatoolbox-0.5.7/datatoolbox/naming_convention.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/patches.py` & `datatoolbox-0.5.7/datatoolbox/patches.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/pint_definitions.txt` & `datatoolbox-0.5.7/datatoolbox/pint_definitions.txt`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 DM = [demand]
 
 # climate context
 [AGWP] = [Power] * [time] / [area] / [mass]
 AGWP_CO2 =  9.17E-14 * W * yr /m**2 / kg
 #CO2eq = [CO2-equiv]
 #CO2eq = 1 * [GWP]
+CO2eq = [CO2]
 
 # social dimension
 capita = [count]
 cap = 1* capita
 person = 1 * capita
 thousands = 1000 * count
 millions = 1000000 * count
```

### Comparing `datatoolbox-0.5.6/datatoolbox/sets.py` & `datatoolbox-0.5.7/datatoolbox/sets.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/templates.py` & `datatoolbox-0.5.7/datatoolbox/templates.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tools/CRF_extract_CA_2021.xlsx` & `datatoolbox-0.5.7/datatoolbox/tools/CRF_extract_CA_2021.xlsx`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tools/EQW_SPLIT_EFF0460_CATEFFEXT_210120.SCEN` & `datatoolbox-0.5.7/datatoolbox/tools/EQW_SPLIT_EFF0460_CATEFFEXT_210120.SCEN`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tools/IEA_B2DS_4.SCEN` & `datatoolbox-0.5.7/datatoolbox/tools/IEA_B2DS_4.SCEN`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tools/WEO_2019_test.SCEN` & `datatoolbox-0.5.7/datatoolbox/tools/WEO_2019_test.SCEN`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tools/conversion_to_v0.3.py` & `datatoolbox-0.5.7/datatoolbox/tools/conversion_to_v0.3.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tools/excel.py` & `datatoolbox-0.5.7/datatoolbox/tools/excel.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tools/for_datatables.py` & `datatoolbox-0.5.7/datatoolbox/tools/for_datatables.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tools/html.py` & `datatoolbox-0.5.7/datatoolbox/tools/html.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tools/kaya_idendentiy_decomposition.py` & `datatoolbox-0.5.7/datatoolbox/tools/kaya_idendentiy_decomposition.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tools/magicc6.py` & `datatoolbox-0.5.7/datatoolbox/tools/magicc6.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tools/matplotlib.py` & `datatoolbox-0.5.7/datatoolbox/tools/matplotlib.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tools/pandas.py` & `datatoolbox-0.5.7/datatoolbox/tools/pandas.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tools/py_magicc_tools.py` & `datatoolbox-0.5.7/datatoolbox/tools/py_magicc_tools.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tools/pyam.py` & `datatoolbox-0.5.7/datatoolbox/tools/pyam.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tools/renaming_DB.py` & `datatoolbox-0.5.7/datatoolbox/tools/renaming_DB.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tools/run_MAGICC_startup_simple.xlsx` & `datatoolbox-0.5.7/datatoolbox/tools/run_MAGICC_startup_simple.xlsx`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tools/run_magicc6.m` & `datatoolbox-0.5.7/datatoolbox/tools/run_magicc6.m`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tools/statistics.py` & `datatoolbox-0.5.7/datatoolbox/tools/statistics.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tools/test.docx` & `datatoolbox-0.5.7/datatoolbox/tools/test.docx`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tools/word.py` & `datatoolbox-0.5.7/datatoolbox/tools/word.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tools/xarray.py` & `datatoolbox-0.5.7/datatoolbox/tools/xarray.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tutorials/00_search_find_and_access_data.py` & `datatoolbox-0.5.7/datatoolbox/tutorials/00_search_find_and_access_data.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tutorials/01_emission_comparison.py` & `datatoolbox-0.5.7/datatoolbox/tutorials/01_emission_comparison.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tutorials/02_unit_conversion.py` & `datatoolbox-0.5.7/datatoolbox/tutorials/02_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tutorials/03_intermediate_example.py` & `datatoolbox-0.5.7/datatoolbox/tutorials/03_intermediate_example.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tutorials/04_sources.py` & `datatoolbox-0.5.7/datatoolbox/tutorials/04_sources.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tutorials/06_xarray_examples.py` & `datatoolbox-0.5.7/datatoolbox/tutorials/06_xarray_examples.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tutorials/07_renewable_share_compuation.py` & `datatoolbox-0.5.7/datatoolbox/tutorials/07_renewable_share_compuation.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tutorials/08_low_carbon_fuel_computation.py` & `datatoolbox-0.5.7/datatoolbox/tutorials/08_low_carbon_fuel_computation.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tutorials/introduction_v1.ipynb` & `datatoolbox-0.5.7/datatoolbox/tutorials/introduction_v1.ipynb`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/tutorials/jump_start.py` & `datatoolbox-0.5.7/datatoolbox/tutorials/jump_start.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/util.py` & `datatoolbox-0.5.7/datatoolbox/util.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox/workflows.py` & `datatoolbox-0.5.7/datatoolbox/workflows.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/datatoolbox.egg-info/PKG-INFO` & `datatoolbox-0.5.7/datatoolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatoolbox
-Version: 0.5.6
+Version: 0.5.7
 Summary: The Python Data Toolbox
 Home-page: https://gitlab.com/climateanalytics/datatoolbox
 Author: Andreas Geiges
 Author-email: a.geiges@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `datatoolbox-0.5.6/datatoolbox.egg-info/SOURCES.txt` & `datatoolbox-0.5.7/datatoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/doc/Makefile` & `datatoolbox-0.5.7/doc/Makefile`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/doc/conf.py` & `datatoolbox-0.5.7/doc/conf.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/doc/figures/ID_meta_data.svg` & `datatoolbox-0.5.7/doc/figures/ID_meta_data.svg`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/doc/figures/config_input.png` & `datatoolbox-0.5.7/doc/figures/config_input.png`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/doc/first_steps.md` & `datatoolbox-0.5.7/doc/first_steps.md`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/doc/installation.md` & `datatoolbox-0.5.7/doc/installation.md`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/doc/license.rst` & `datatoolbox-0.5.7/doc/license.rst`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/doc/make.bat` & `datatoolbox-0.5.7/doc/make.bat`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/documentation/Datatoolbox - First steps.md` & `datatoolbox-0.5.7/documentation/Datatoolbox - First steps.md`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/readthedocs.yml` & `datatoolbox-0.5.7/readthedocs.yml`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/setup.py` & `datatoolbox-0.5.7/setup.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/tests/test_calculations.py` & `datatoolbox-0.5.7/tests/test_calculations.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/tests/test_converters.py` & `datatoolbox-0.5.7/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/tests/test_database.py` & `datatoolbox-0.5.7/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/tests/test_dataset.py` & `datatoolbox-0.5.7/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/tests/test_datatable.py` & `datatoolbox-0.5.7/tests/test_datatable.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/tests/test_io.py` & `datatoolbox-0.5.7/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/tests/test_pyam.py` & `datatoolbox-0.5.7/tests/test_pyam.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/tests/test_tableset.py` & `datatoolbox-0.5.7/tests/test_tableset.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/tests/test_tools.py` & `datatoolbox-0.5.7/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/tests/test_units.py` & `datatoolbox-0.5.7/tests/test_units.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,24 +17,41 @@
 def test_custom_base_conversion1():    
     obs = dt.units.conversionFactor('t oil_equivalent/capita', 'MJ/capita')
     exp = 41868
     npt.assert_almost_equal(obs, exp)
 
 
 def test_GWP_conversion_N2O():    
-    obs = dt.units.conversionFactor("Mt N2O", "Gg CO2eq", context="GWPAR4")
+    obs = dt.units.conversionFactor("Mt N2O", "Gg CO2eq", context="AR4GWP100")
     exp = 298000
     npt.assert_almost_equal(obs, exp)
 
 def test_GWP_conversion_CH4():        
-    obs = dt.units.conversionFactor("Mt CH4", "Mt CO2eq", context="GWPAR4")
+    obs = dt.units.conversionFactor("Mt CH4", "Mt CO2eq", context="AR4GWP100")
     exp = 25
     npt.assert_almost_equal(obs, exp)
     
+def test_GWP_AR6_conversion_CH4():        
+    obs = dt.units.conversionFactor("Mt CH4", "Mt CO2eq", context="AR5GWP100")
+    exp = 28
+    npt.assert_almost_equal(obs, exp)
+        
+    
+def test_context_and_missing_space():        
+    obs = dt.units.conversionFactor("MtCH4", "tCO2eq", context="AR5GWP100")
+    exp = 28
+    npt.assert_almost_equal(obs, exp)
+    
 def test_HFC_units():    
     dt.core.ur('HFC134aeq') 
     
+def test_unique_conversion():
+    assert dt.units.conversionFactor("ppm", "fraction") == 1e-6
+    assert dt.units.conversionFactor("%", "fraction") == 0.01
+    assert dt.units.conversionFactor("fraction", "percent") == 100
+    
+    
 def test_function_getUnit():
     
     dt.core.getUnit('°C')
     dt.core.getUnit('$')
     dt.core.getUnit('€')
```

### Comparing `datatoolbox-0.5.6/tests/test_utilities.py` & `datatoolbox-0.5.7/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/tests/test_xarray.py` & `datatoolbox-0.5.7/tests/test_xarray.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.6/tests/util_for_testing.py` & `datatoolbox-0.5.7/tests/util_for_testing.py`

 * *Files identical despite different names*

