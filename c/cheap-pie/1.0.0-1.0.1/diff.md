# Comparing `tmp/cheap_pie-1.0.0.tar.gz` & `tmp/cheap_pie-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheap_pie-1.0.0.tar", last modified: Mon May 22 21:34:10 2023, max compression
+gzip compressed data, was "cheap_pie-1.0.1.tar", last modified: Tue May 23 08:02:04 2023, max compression
```

## Comparing `cheap_pie-1.0.0.tar` & `cheap_pie-1.0.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-22 21:34:10.598870 cheap_pie-1.0.0/
--rwxrwxrwx   0 marco     (1000) marco     (1000)    11357 2022-12-10 01:01:26.000000 cheap_pie-1.0.0/LICENSE
--rwxrwxrwx   0 marco     (1000) marco     (1000)     8432 2023-05-22 21:34:10.599369 cheap_pie-1.0.0/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)     8091 2023-05-18 10:44:55.000000 cheap_pie-1.0.0/README.md
--rwxrwxrwx   0 marco     (1000) marco     (1000)      103 2023-05-22 21:34:10.600896 cheap_pie-1.0.0/setup.cfg
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1260 2023-05-22 21:32:25.000000 cheap_pie-1.0.0/setup.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-22 21:34:10.517321 cheap_pie-1.0.0/src/
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-22 21:34:10.528772 cheap_pie-1.0.0/src/cheap_pie/
--rwxrwxrwx   0 marco     (1000) marco     (1000)      207 2023-05-22 21:21:25.000000 cheap_pie-1.0.0/src/cheap_pie/__init__.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-22 21:34:10.553938 cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/
--rwxrwxrwx   0 marco     (1000) marco     (1000)      211 2023-05-22 20:58:17.000000 cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     7623 2023-05-21 17:00:23.000000 cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cbitfield.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2800 2023-05-21 16:18:51.000000 cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cheap_pie_main.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3232 2023-05-18 12:45:16.000000 cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cp_banner.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3388 2023-05-22 19:16:36.000000 cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cp_builder.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2691 2023-05-21 13:23:16.000000 cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cp_cli.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     8613 2023-05-22 21:20:38.000000 cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cp_hal.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)    15666 2023-05-22 20:39:24.000000 cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cp_register.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3669 2023-05-22 21:00:42.000000 cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/test.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-22 21:34:10.573128 cheap_pie-1.0.0/src/cheap_pie/parsers/
--rwxrwxrwx   0 marco     (1000) marco     (1000)      163 2023-05-22 20:56:30.000000 cheap_pie-1.0.0/src/cheap_pie/parsers/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2427 2023-05-21 15:47:51.000000 cheap_pie-1.0.0/src/cheap_pie/parsers/cp_parsers_wrapper.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3161 2023-05-21 16:42:25.000000 cheap_pie-1.0.0/src/cheap_pie/parsers/ipxact_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2643 2023-05-21 16:43:35.000000 cheap_pie-1.0.0/src/cheap_pie/parsers/ipyxact_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1166 2023-05-21 13:58:09.000000 cheap_pie-1.0.0/src/cheap_pie/parsers/rdl_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3133 2023-05-21 16:44:23.000000 cheap_pie-1.0.0/src/cheap_pie/parsers/svd_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3209 2023-05-21 16:45:01.000000 cheap_pie-1.0.0/src/cheap_pie/parsers/svd_parse_repo.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2506 2023-05-21 13:40:46.000000 cheap_pie-1.0.0/src/cheap_pie/parsers/xml_xslt.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-22 21:34:10.584553 cheap_pie-1.0.0/src/cheap_pie/tools/
--rwxrwxrwx   0 marco     (1000) marco     (1000)       92 2023-05-21 15:55:01.000000 cheap_pie-1.0.0/src/cheap_pie/tools/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     4418 2023-05-22 21:15:24.000000 cheap_pie-1.0.0/src/cheap_pie/tools/hal2doc.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2712 2023-05-22 19:30:55.000000 cheap_pie-1.0.0/src/cheap_pie/tools/rdl2any.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2651 2023-05-22 21:20:52.000000 cheap_pie-1.0.0/src/cheap_pie/tools/search.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-22 21:34:10.597032 cheap_pie-1.0.0/src/cheap_pie/transport/
--rwxrwxrwx   0 marco     (1000) marco     (1000)      219 2023-05-22 21:18:16.000000 cheap_pie-1.0.0/src/cheap_pie/transport/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2367 2023-05-21 15:28:36.000000 cheap_pie-1.0.0/src/cheap_pie/transport/cp_dummy_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2298 2023-05-21 15:27:18.000000 cheap_pie-1.0.0/src/cheap_pie/transport/cp_esptool_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1776 2023-05-21 16:01:42.000000 cheap_pie-1.0.0/src/cheap_pie/transport/cp_jlink_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1777 2023-05-21 16:11:06.000000 cheap_pie-1.0.0/src/cheap_pie/transport/cp_pyocd_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     5206 2023-05-22 20:54:15.000000 cheap_pie-1.0.0/src/cheap_pie/transport/cp_pyverilator_transport.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-22 21:34:10.542069 cheap_pie-1.0.0/src/cheap_pie.egg-info/
--rwxrwxrwx   0 marco     (1000) marco     (1000)     8432 2023-05-22 21:34:10.000000 cheap_pie-1.0.0/src/cheap_pie.egg-info/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1317 2023-05-22 21:34:10.000000 cheap_pie-1.0.0/src/cheap_pie.egg-info/SOURCES.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2023-05-22 21:34:10.000000 cheap_pie-1.0.0/src/cheap_pie.egg-info/dependency_links.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)      125 2023-05-22 21:34:10.000000 cheap_pie-1.0.0/src/cheap_pie.egg-info/requires.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)       10 2023-05-22 21:34:10.000000 cheap_pie-1.0.0/src/cheap_pie.egg-info/top_level.txt
+drwxrwxrwx   0 merlinm   (1000) merlinm   (1000)        0 2023-05-23 08:02:04.916751 cheap_pie-1.0.1/
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)    11357 2021-11-26 09:02:37.000000 cheap_pie-1.0.1/LICENSE
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)    10109 2023-05-23 08:02:04.917999 cheap_pie-1.0.1/PKG-INFO
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     8091 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/README.md
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)      103 2023-05-23 08:02:04.918998 cheap_pie-1.0.1/setup.cfg
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     1260 2023-05-23 08:00:08.000000 cheap_pie-1.0.1/setup.py
+drwxrwxrwx   0 merlinm   (1000) merlinm   (1000)        0 2023-05-23 08:02:04.773320 cheap_pie-1.0.1/src/
+drwxrwxrwx   0 merlinm   (1000) merlinm   (1000)        0 2023-05-23 08:02:04.793107 cheap_pie-1.0.1/src/cheap_pie/
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)      207 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/__init__.py
+drwxrwxrwx   0 merlinm   (1000) merlinm   (1000)        0 2023-05-23 08:02:04.841119 cheap_pie-1.0.1/src/cheap_pie/cheap_pie_core/
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)      211 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/cheap_pie_core/__init__.py
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     7623 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/cheap_pie_core/cbitfield.py
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     2800 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/cheap_pie_core/cheap_pie_main.py
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     3232 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/cheap_pie_core/cp_banner.py
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     3388 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/cheap_pie_core/cp_builder.py
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     2691 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/cheap_pie_core/cp_cli.py
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     8982 2023-05-23 07:44:25.000000 cheap_pie-1.0.1/src/cheap_pie/cheap_pie_core/cp_hal.py
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)    15666 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/cheap_pie_core/cp_register.py
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     3673 2023-05-23 07:47:29.000000 cheap_pie-1.0.1/src/cheap_pie/cheap_pie_core/test.py
+drwxrwxrwx   0 merlinm   (1000) merlinm   (1000)        0 2023-05-23 08:02:04.878461 cheap_pie-1.0.1/src/cheap_pie/parsers/
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)      163 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/parsers/__init__.py
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     2427 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/parsers/cp_parsers_wrapper.py
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     3161 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/parsers/ipxact_parse.py
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     2643 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/parsers/ipyxact_parse.py
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     1166 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/parsers/rdl_parse.py
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     3133 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/parsers/svd_parse.py
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     3209 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/parsers/svd_parse_repo.py
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     2506 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/parsers/xml_xslt.py
+drwxrwxrwx   0 merlinm   (1000) merlinm   (1000)        0 2023-05-23 08:02:04.893210 cheap_pie-1.0.1/src/cheap_pie/tools/
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)       92 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/tools/__init__.py
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     4418 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/tools/hal2doc.py
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     2712 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/tools/rdl2any.py
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     2651 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/tools/search.py
+drwxrwxrwx   0 merlinm   (1000) merlinm   (1000)        0 2023-05-23 08:02:04.913690 cheap_pie-1.0.1/src/cheap_pie/transport/
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)      219 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/transport/__init__.py
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     2367 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/transport/cp_dummy_transport.py
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     2298 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/transport/cp_esptool_transport.py
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     1776 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/transport/cp_jlink_transport.py
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     1777 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/transport/cp_pyocd_transport.py
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     5206 2023-05-23 07:38:09.000000 cheap_pie-1.0.1/src/cheap_pie/transport/cp_pyverilator_transport.py
+drwxrwxrwx   0 merlinm   (1000) merlinm   (1000)        0 2023-05-23 08:02:04.807951 cheap_pie-1.0.1/src/cheap_pie.egg-info/
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)    10109 2023-05-23 08:02:04.000000 cheap_pie-1.0.1/src/cheap_pie.egg-info/PKG-INFO
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)     1317 2023-05-23 08:02:04.000000 cheap_pie-1.0.1/src/cheap_pie.egg-info/SOURCES.txt
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)        1 2023-05-23 08:02:04.000000 cheap_pie-1.0.1/src/cheap_pie.egg-info/dependency_links.txt
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)      125 2023-05-23 08:02:04.000000 cheap_pie-1.0.1/src/cheap_pie.egg-info/requires.txt
+-rwxrwxrwx   0 merlinm   (1000) merlinm   (1000)       10 2023-05-23 08:02:04.000000 cheap_pie-1.0.1/src/cheap_pie.egg-info/top_level.txt
```

### Comparing `cheap_pie-1.0.0/LICENSE` & `cheap_pie-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.0/PKG-INFO` & `cheap_pie-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: cheap_pie
-Version: 1.0.0
-Summary: A python tool for silicon validation.
-Home-page: https://github.com/bat52/cheap_pie
-Author: Marco Merlin
-Author-email: marcomerli@gmail.com
-License: Apache 2.0
-Keywords: python silicon validation
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # cheap_pie
 A python tool for register-based chip verification and validation
 
 "Cheap Pie" is a python tool for register-based chip verification and validation.
 The name is a translitteration of "chip py" for obvious reasons.
 
 Given an input description file for the chip, it provides a register-level and 
@@ -218,9 +205,7 @@
 
 Banner created with pyfiglet
 https://www.devdungeon.com/content/create-ascii-art-text-banners-python#install_pyfiglet
 
 Cheap Pie is modeled after an original Octave/Matlab implementation that cannot
 be shared due to licensing reasons. The original code was converted to python
 using SMOP ( https://github.com/ripple-neuro/smop ).
-
-
```

### Comparing `cheap_pie-1.0.0/README.md` & `cheap_pie-1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,211 +1,223 @@
-# cheap_pie
-A python tool for register-based chip verification and validation
-
-"Cheap Pie" is a python tool for register-based chip verification and validation.
-The name is a translitteration of "chip py" for obvious reasons.
-
-Given an input description file for the chip, it provides a register-level and 
-bitfield-level read/write access, through a generic transport layer.
-
-Currently the implemented description input modes are:
-- CMSIS-SVD (https://www.keil.com/pack/doc/CMSIS/SVD/html/svd_Format_pg.html)
-- IP-XACT ( https://www.accellera.org/downloads/standards/ip-xact )
-- SystemRDL (https://www.accellera.org/activities/working-groups/systemrdl)
-
-but it should be relatively easy to add different chip description formats.
-
-Although tested on few real chips (NXP QN9080, I.MX RT1010, K64F),
-cheap_pie parser already supports dozen of devices, listed in the CMSIS-SVD 
-repository https://github.com/posborne/cmsis-svd .
-
-Currently the supported transport layers are jlink and pyocd, but it should be really easy
-to add support for different transport layers, like for instance openSDA, 
-CMSIS-DAP, Total Phase Cheetah, GDB or any other.
-
-Experimental support for pyverilator transport allows to run interactive simulation
-of register blocks generated from SystemRDL source.
-
+Metadata-Version: 2.1
+Name: cheap_pie
+Version: 1.0.1
+Summary: A python tool for silicon validation.
+Home-page: https://github.com/bat52/cheap_pie
 Author: Marco Merlin
-Tested on ipython3 (python 3.8.5) on ubuntu 20.04
-
-# IPython Example:
-        %run cheap_pie
-        inval = "0xFFFFFFFF"
-        hal.regs.ADC_ANA_CTRL.setreg(inval)
-        retval = hex(hal.regs.ADC_ANA_CTRL.getreg())
-        assert(literal_eval(inval) == literal_eval(retval))
-
-        # decimal assignement        
-        inval = 2
-        hal.regs.ADC_ANA_CTRL.setreg(inval)
-        retval = hal.regs.ADC_ANA_CTRL.getreg()        
-        assert(inval == retval)
+Author-email: marcomerli@gmail.com
+License: Apache 2.0
+Description: # cheap_pie
+        A python tool for register-based chip verification and validation
         
-        hal.regs.ADC_ANA_CTRL
-        hal.regs.ADC_ANA_CTRL.display()
+        "Cheap Pie" is a python tool for register-based chip verification and validation.
+        The name is a translitteration of "chip py" for obvious reasons.
+        
+        Given an input description file for the chip, it provides a register-level and 
+        bitfield-level read/write access, through a generic transport layer.
+        
+        Currently the implemented description input modes are:
+        - CMSIS-SVD (https://www.keil.com/pack/doc/CMSIS/SVD/html/svd_Format_pg.html)
+        - IP-XACT ( https://www.accellera.org/downloads/standards/ip-xact )
+        - SystemRDL (https://www.accellera.org/activities/working-groups/systemrdl)
+        
+        but it should be relatively easy to add different chip description formats.
+        
+        Although tested on few real chips (NXP QN9080, I.MX RT1010, K64F),
+        cheap_pie parser already supports dozen of devices, listed in the CMSIS-SVD 
+        repository https://github.com/posborne/cmsis-svd .
+        
+        Currently the supported transport layers are jlink and pyocd, but it should be really easy
+        to add support for different transport layers, like for instance openSDA, 
+        CMSIS-DAP, Total Phase Cheetah, GDB or any other.
+        
+        Experimental support for pyverilator transport allows to run interactive simulation
+        of register blocks generated from SystemRDL source.
+        
+        Author: Marco Merlin
+        Tested on ipython3 (python 3.8.5) on ubuntu 20.04
+        
+        # IPython Example:
+                %run cheap_pie
+                inval = "0xFFFFFFFF"
+                hal.regs.ADC_ANA_CTRL.setreg(inval)
+                retval = hex(hal.regs.ADC_ANA_CTRL.getreg())
+                assert(literal_eval(inval) == literal_eval(retval))
+        
+                # decimal assignement        
+                inval = 2
+                hal.regs.ADC_ANA_CTRL.setreg(inval)
+                retval = hal.regs.ADC_ANA_CTRL.getreg()        
+                assert(inval == retval)
+                
+                hal.regs.ADC_ANA_CTRL
+                hal.regs.ADC_ANA_CTRL.display()
+                        
+                print('Test bitfield methods...')
                 
-        print('Test bitfield methods...')
+                hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM
+                hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.display()
+                hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.display(2)
+                hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.setbit(inval)
+                retval = hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.getbit()
+                assert(inval == retval)
+        
+                # subscriptable register access
+                hal[0]
+                # subscriptable bitfield access
+                hal[0][0]
+                # subscriptable as a dictionary
+                hal['SYSCON_RST_SW_SET']
+                hal['ADC_ANA_CTRL']['ADC_BM']
+                
+                # assignement
+                hal['ADC_ANA_CTRL'] = 1
+                hal['ADC_ANA_CTRL']['ADC_BM'] = 2
+                # dict-based assignement in single register write
+                hal['ADC_ANA_CTRL'] = {'DITHER_EN': 1, 'CHOP_EN': 1, 'INV_CLK': 1}
+        
+                # help
+                hal.regs.ADC_ANA_CTRL.help()
+                ADC core and reference setting regsiter
+                           ADC_BM: 
+                                 : ADC bias current selection.
+                        ADC_ORDER: 
+                                 : 1 to enable SD ADC 2 order mode selection
+                        DITHER_EN: 
+                                 : 1 to enable SD ADC PN Sequence in chopper mode
+                          CHOP_EN: 
+                                 : 1 to enable SD ADC chopper
+                          INV_CLK: 
+                                 : 1 to invert SD ADC Output Clock
+                          VREF_BM: 
+                                 : SD ADC Reference Driver bias current selection.
+                       VREF_BM_X3: 
+                                 : SD ADC Reference Driver bias current triple.
+                       VINN_IN_BM: 
+                                 : PGA VlNN Input Driver bias current selection.
+                      VINN_OUT_BM: 
+                                 : PGA VlNN Output Driver bias current selection.
+                   VINN_OUT_BM_X3: 
+                                 : PGA VlNN Output Driver bias current triple.
+                      ADC_BM_DIV2: 
+                                 : SD ADC bias current half.
+        
+        # CLI Example:
+                # load RT1010 from local svd file under ./devices/
+                # automatically calls ipython and cheap_pie initialization
+                ./cheap_pie.sh -rf MIMXRT1011.svd -t jlink
+        
+                # load K64 from CMSIS-SVD
+                # need to specify vendor for svd not in ./devices/
+                ./cheap_pie.sh -rf MK64F12.svd -ve Freescale -t jlink
+        
+                # calls QN9080 with dummy transport layer 
+                # useful to explore device registers
+                ./cheap_pie.sh -t dummy
+        
+        # Default configurations Examples:
+                # calls QN9080 device with dummy transport layer
+                ./cfgs/cp_qn9080_dummy.sh
+                # calls RT1010 device with jlink transport layer
+                ./cfgs/cp_rt1010_jlink.sh
+                # calls K20 device with dummy transport layer
+                ./cfgs/cp_k20_dummy.sh
+        
+        # Verilator interactive simulation Examples:
+                ./tools/rdl2verilog.py -f ./devices/rdl/basic.rdl
+                ./cheap_pie.sh -dd  ./devices/rdl -rf basic.rdl -fmt rdl -t verilator -topv ./devices/rdl/basic/basic_rf.sv
+        
+        # Install
+        ## From pypi
+                pip3 install cheap_pie
+        ## From github
+                pip3 install git+https://github.com/bat52/cheap_pie.git@master
+        
+        # Dependencies for core (required):        
+                # for XML parsing (used by legacy svd parser and IP-XACT parser)
+                pip3 install untangle
+                # for exporting XML info into a human-readable document
+                pip3 install python-docx
+                # for dumping registers
+                pip3 install hickle
+                # CMSIS-SVD python parser including many svd files https://github.com/posborne/cmsis-svd
+                pip3 install cmsis-svd
+                # SPIRIT IP-XACT parser through ipyxact https://github.com/olofk/ipyxact
+                pip3 install ipyxact                
+                # SystemRDL to register-file verilog
+                https://github.com/hughjackson/PeakRDL-verilog
+                # SystemRDL to IP-XACT
+                https://github.com/SystemRDL/PeakRDL-ipxact
+        # Dependencies for validation/transport layers (optional):        
+                # for JLINK
+                pip3 install pylink-square
+                # pyOCD for CMSIS-DAP and JLINK support (only tested in python-venv)
+                pip3 install pyocd
+                # esptool for Espressif devices (not yet functional)
+                pip3 install esptool        
+        # Dependencies for verification (optional AND experimental):
+                # verilator
+                https://www.veripool.org/verilator/
+                # pyverilator (python verilator wrapper)
+                https://github.com/csail-csg/pyverilator        
+                # gtkwave
+                http://gtkwave.sourceforge.net/
+        
+        # Releasing
+        
+        Releases are published automatically when a tag is pushed to GitHub.
+        
+        .. code-block:: bash
+        
+           # Set next version number
+           export RELEASE=x.x.x
+        
+           # Create tags
+           git commit --allow-empty -m "Release $RELEASE"
+           git tag -a $RELEASE -m "Version $RELEASE"
+        
+           # Push
+           git push upstream --tags
+        
+        # Register description formats
+        regtool from opentitan project seems similar, using JSON to represent chip/IP structure, and I2C transport
+        https://docs.opentitan.org/doc/rm/register_tool/
+        
+        custom input, output: verilog, VHDL, YAML, JSON, TOML, Spreadsheet (XLSX, XLS, OSD, CSV)
+        https://github.com/rggen/rggen
+        
+        convert ipxact register file description into verilog register bank
+        https://github.com/oddball/ipxact2systemverilog
+        
+        # Others	
+        In conjunction with pyVISA (https://pyvisa.readthedocs.io/en/master/), used for 
+        instument control, it provides a simple and fully python-contained environment
+        for silicon validation.
+        
+        Graphical Render of bitfield structures
+        https://github.com/wavedrom/bitfield
+        
+        C++ register/bitfields access (including generation from svd)
+        https://github.com/thanks4opensource/regbits
+        
+        STM C++ regbits implementation
+        https://github.com/thanks4opensource/regbits_stm
+        
+        a barebone embedded library generator
+        https://modm.io/
+        
+        hardware descriptions for AVR and STM32 devices
+        https://github.com/modm-io/modm-devices
+        
+        STM32 Peripheral Access Crates (from svd)
+        https://github.com/stm32-rs/stm32-rs
+        
+        Banner created with pyfiglet
+        https://www.devdungeon.com/content/create-ascii-art-text-banners-python#install_pyfiglet
+        
+        Cheap Pie is modeled after an original Octave/Matlab implementation that cannot
+        be shared due to licensing reasons. The original code was converted to python
+        using SMOP ( https://github.com/ripple-neuro/smop ).
         
-        hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM
-        hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.display()
-        hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.display(2)
-        hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.setbit(inval)
-        retval = hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.getbit()
-        assert(inval == retval)
-
-        # subscriptable register access
-        hal[0]
-        # subscriptable bitfield access
-        hal[0][0]
-        # subscriptable as a dictionary
-        hal['SYSCON_RST_SW_SET']
-        hal['ADC_ANA_CTRL']['ADC_BM']
-        
-        # assignement
-        hal['ADC_ANA_CTRL'] = 1
-        hal['ADC_ANA_CTRL']['ADC_BM'] = 2
-        # dict-based assignement in single register write
-        hal['ADC_ANA_CTRL'] = {'DITHER_EN': 1, 'CHOP_EN': 1, 'INV_CLK': 1}
-
-        # help
-        hal.regs.ADC_ANA_CTRL.help()
-        ADC core and reference setting regsiter
-                   ADC_BM: 
-                         : ADC bias current selection.
-                ADC_ORDER: 
-                         : 1 to enable SD ADC 2 order mode selection
-                DITHER_EN: 
-                         : 1 to enable SD ADC PN Sequence in chopper mode
-                  CHOP_EN: 
-                         : 1 to enable SD ADC chopper
-                  INV_CLK: 
-                         : 1 to invert SD ADC Output Clock
-                  VREF_BM: 
-                         : SD ADC Reference Driver bias current selection.
-               VREF_BM_X3: 
-                         : SD ADC Reference Driver bias current triple.
-               VINN_IN_BM: 
-                         : PGA VlNN Input Driver bias current selection.
-              VINN_OUT_BM: 
-                         : PGA VlNN Output Driver bias current selection.
-           VINN_OUT_BM_X3: 
-                         : PGA VlNN Output Driver bias current triple.
-              ADC_BM_DIV2: 
-                         : SD ADC bias current half.
-
-# CLI Example:
-        # load RT1010 from local svd file under ./devices/
-        # automatically calls ipython and cheap_pie initialization
-        ./cheap_pie.sh -rf MIMXRT1011.svd -t jlink
-
-        # load K64 from CMSIS-SVD
-        # need to specify vendor for svd not in ./devices/
-        ./cheap_pie.sh -rf MK64F12.svd -ve Freescale -t jlink
-
-        # calls QN9080 with dummy transport layer 
-        # useful to explore device registers
-        ./cheap_pie.sh -t dummy
-
-# Default configurations Examples:
-        # calls QN9080 device with dummy transport layer
-        ./cfgs/cp_qn9080_dummy.sh
-        # calls RT1010 device with jlink transport layer
-        ./cfgs/cp_rt1010_jlink.sh
-        # calls K20 device with dummy transport layer
-        ./cfgs/cp_k20_dummy.sh
-
-# Verilator interactive simulation Examples:
-        ./tools/rdl2verilog.py -f ./devices/rdl/basic.rdl
-        ./cheap_pie.sh -dd  ./devices/rdl -rf basic.rdl -fmt rdl -t verilator -topv ./devices/rdl/basic/basic_rf.sv
-
-# Install
-## From pypi
-        pip3 install cheap_pie
-## From github
-        pip3 install git+https://github.com/bat52/cheap_pie.git@master
-
-# Dependencies for core (required):        
-        # for XML parsing (used by legacy svd parser and IP-XACT parser)
-        pip3 install untangle
-        # for exporting XML info into a human-readable document
-        pip3 install python-docx
-        # for dumping registers
-        pip3 install hickle
-        # CMSIS-SVD python parser including many svd files https://github.com/posborne/cmsis-svd
-        pip3 install cmsis-svd
-        # SPIRIT IP-XACT parser through ipyxact https://github.com/olofk/ipyxact
-        pip3 install ipyxact                
-        # SystemRDL to register-file verilog
-        https://github.com/hughjackson/PeakRDL-verilog
-        # SystemRDL to IP-XACT
-        https://github.com/SystemRDL/PeakRDL-ipxact
-# Dependencies for validation/transport layers (optional):        
-        # for JLINK
-        pip3 install pylink-square
-        # pyOCD for CMSIS-DAP and JLINK support (only tested in python-venv)
-        pip3 install pyocd
-        # esptool for Espressif devices (not yet functional)
-        pip3 install esptool        
-# Dependencies for verification (optional AND experimental):
-        # verilator
-        https://www.veripool.org/verilator/
-        # pyverilator (python verilator wrapper)
-        https://github.com/csail-csg/pyverilator        
-        # gtkwave
-        http://gtkwave.sourceforge.net/
-
-# Releasing
-
-Releases are published automatically when a tag is pushed to GitHub.
-
-.. code-block:: bash
-
-   # Set next version number
-   export RELEASE=x.x.x
-
-   # Create tags
-   git commit --allow-empty -m "Release $RELEASE"
-   git tag -a $RELEASE -m "Version $RELEASE"
-
-   # Push
-   git push upstream --tags
-
-# Register description formats
-regtool from opentitan project seems similar, using JSON to represent chip/IP structure, and I2C transport
-https://docs.opentitan.org/doc/rm/register_tool/
-
-custom input, output: verilog, VHDL, YAML, JSON, TOML, Spreadsheet (XLSX, XLS, OSD, CSV)
-https://github.com/rggen/rggen
-
-convert ipxact register file description into verilog register bank
-https://github.com/oddball/ipxact2systemverilog
-
-# Others	
-In conjunction with pyVISA (https://pyvisa.readthedocs.io/en/master/), used for 
-instument control, it provides a simple and fully python-contained environment
-for silicon validation.
-
-Graphical Render of bitfield structures
-https://github.com/wavedrom/bitfield
-
-C++ register/bitfields access (including generation from svd)
-https://github.com/thanks4opensource/regbits
-
-STM C++ regbits implementation
-https://github.com/thanks4opensource/regbits_stm
-
-a barebone embedded library generator
-https://modm.io/
-
-hardware descriptions for AVR and STM32 devices
-https://github.com/modm-io/modm-devices
-
-STM32 Peripheral Access Crates (from svd)
-https://github.com/stm32-rs/stm32-rs
-
-Banner created with pyfiglet
-https://www.devdungeon.com/content/create-ascii-art-text-banners-python#install_pyfiglet
-
-Cheap Pie is modeled after an original Octave/Matlab implementation that cannot
-be shared due to licensing reasons. The original code was converted to python
-using SMOP ( https://github.com/ripple-neuro/smop ).
+Keywords: python silicon validation
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `cheap_pie-1.0.0/setup.py` & `cheap_pie-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 setup(
     name='cheap_pie',
-    version='1.0.0',
+    version='1.0.1',
     license='Apache 2.0',
     author="Marco Merlin",
     author_email='marcomerli@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     description="A python tool for silicon validation.",
     long_description=long_description,
```

### Comparing `cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cbitfield.py` & `cheap_pie-1.0.1/src/cheap_pie/cheap_pie_core/cbitfield.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cheap_pie_main.py` & `cheap_pie-1.0.1/src/cheap_pie/cheap_pie_core/cheap_pie_main.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cp_banner.py` & `cheap_pie-1.0.1/src/cheap_pie/cheap_pie_core/cp_banner.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cp_builder.py` & `cheap_pie-1.0.1/src/cheap_pie/cheap_pie_core/cp_builder.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cp_cli.py` & `cheap_pie-1.0.1/src/cheap_pie/cheap_pie_core/cp_cli.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cp_hal.py` & `cheap_pie-1.0.1/src/cheap_pie/cheap_pie_core/cp_hal.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,23 @@
     """
     Cheap Pie Hardware Abstraction Layer
     """
     regs = []
     hif = None
 
     def __init__(self,regs):
-        self.regs = regs
-        if len(regs) > 0:
-            self.hif = regs[0].hif
+        if isinstance(regs,CpHal):
+            # this allows generating CpHal super-classes from a CpHal instance
+            self.regs = regs.regs
         else:
-            print('# WARNING: no register defined!')
+            self.regs = regs
+            if len(regs) > 0:
+                self.hif = regs[0].hif
+            else:
+                print('# WARNING: no register defined!')
 
     def __len__(self):
         return len(self.regs)
 
     def __iter__(self):
         return self.regs.__iter__()
 
@@ -127,14 +131,18 @@
             for line in outstrlist:
                 print(line)
         else:
             print('No differences found!!!')
 
         return outstrlist
 
+class CpHalSuper(CpHal):
+    def super_method(self):
+        print('Super Method!!!')
+
 def test_cp_hal_to_docx():
     """
     Test Function for Cheap Pie HAL to .docx
     """
     from parsers.cp_parsers_wrapper import cp_parsers_wrapper  # pylint: disable=C0415,C0413,E0401
     from cheap_pie_core.cp_cli import cp_cli                   # pylint: disable=C0415,C0413,E0401
 
@@ -265,9 +273,13 @@
     print(diff)
     assert len(diff) == 2
 
     print('# hal regs2dict')
     mydict = hal.regs2dict()
     assert isinstance(mydict,dict)
 
+    print('# CpHalSuper inheritance')
+    hal_super = CpHalSuper(hal)
+    hal_super.super_method()
+
 if __name__ == '__main__':
     test_cp_hal()
```

### Comparing `cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/cp_register.py` & `cheap_pie-1.0.1/src/cheap_pie/cheap_pie_core/cp_register.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.0/src/cheap_pie/cheap_pie_core/test.py` & `cheap_pie-1.0.1/src/cheap_pie/cheap_pie_core/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,29 +36,29 @@
 from cheap_pie.tools.rdl2any import test_rdl2any                              # pylint: disable=C0413,E0401
 
 # Transport
 from cheap_pie.transport.cp_dummy_transport import test_cp_dummy              # pylint: disable=C0413,E0401
 from cheap_pie.transport.cp_jlink_transport import test_cp_jlink              # pylint: disable=C0413,E0401
 from cheap_pie.transport.cp_pyocd_transport import test_cp_pyocd              # pylint: disable=C0413,E0401
 from cheap_pie.transport.cp_esptool_transport import test_cp_esptool          # pylint: disable=C0413,E0401
-from cheap_pie.transport.cp_pyverilator_transport import test_cp_pyverilator  # pylint: disable=C0413,E0401
+# from cheap_pie.transport.cp_pyverilator_transport import test_cp_pyverilator  # pylint: disable=C0413,E0401
 
 class CheapPieMethods(unittest.TestCase):
     """ Cheap Pie Test Class """
 
     def test_transport(self):
         """ Cheap Pie Test Transport Method """
 
         # dummy for mockup
         test_cp_dummy()
         # NB: requirements_extra.txt are needed!
         test_cp_jlink()
         test_cp_pyocd()
         test_cp_esptool()
-        test_cp_pyverilator()
+        # test_cp_pyverilator()
 
     def test_cheap_pie_core(self):
         """ Test cheap pie core classes """
         test_cp_bitfield()
         test_cp_register()
         test_cp_builder()
         test_cp_hal()
```

### Comparing `cheap_pie-1.0.0/src/cheap_pie/parsers/cp_parsers_wrapper.py` & `cheap_pie-1.0.1/src/cheap_pie/parsers/cp_parsers_wrapper.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.0/src/cheap_pie/parsers/ipxact_parse.py` & `cheap_pie-1.0.1/src/cheap_pie/parsers/ipxact_parse.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.0/src/cheap_pie/parsers/ipyxact_parse.py` & `cheap_pie-1.0.1/src/cheap_pie/parsers/ipyxact_parse.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.0/src/cheap_pie/parsers/rdl_parse.py` & `cheap_pie-1.0.1/src/cheap_pie/parsers/rdl_parse.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.0/src/cheap_pie/parsers/svd_parse.py` & `cheap_pie-1.0.1/src/cheap_pie/parsers/svd_parse.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.0/src/cheap_pie/parsers/svd_parse_repo.py` & `cheap_pie-1.0.1/src/cheap_pie/parsers/svd_parse_repo.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.0/src/cheap_pie/parsers/xml_xslt.py` & `cheap_pie-1.0.1/src/cheap_pie/parsers/xml_xslt.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.0/src/cheap_pie/tools/hal2doc.py` & `cheap_pie-1.0.1/src/cheap_pie/tools/hal2doc.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.0/src/cheap_pie/tools/rdl2any.py` & `cheap_pie-1.0.1/src/cheap_pie/tools/rdl2any.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.0/src/cheap_pie/tools/search.py` & `cheap_pie-1.0.1/src/cheap_pie/tools/search.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.0/src/cheap_pie/transport/cp_dummy_transport.py` & `cheap_pie-1.0.1/src/cheap_pie/transport/cp_dummy_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.0/src/cheap_pie/transport/cp_esptool_transport.py` & `cheap_pie-1.0.1/src/cheap_pie/transport/cp_esptool_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.0/src/cheap_pie/transport/cp_jlink_transport.py` & `cheap_pie-1.0.1/src/cheap_pie/transport/cp_jlink_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.0/src/cheap_pie/transport/cp_pyocd_transport.py` & `cheap_pie-1.0.1/src/cheap_pie/transport/cp_pyocd_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.0/src/cheap_pie/transport/cp_pyverilator_transport.py` & `cheap_pie-1.0.1/src/cheap_pie/transport/cp_pyverilator_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-1.0.0/src/cheap_pie.egg-info/PKG-INFO` & `cheap_pie-1.0.1/src/cheap_pie.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,226 +1,223 @@
 Metadata-Version: 2.1
 Name: cheap-pie
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python tool for silicon validation.
 Home-page: https://github.com/bat52/cheap_pie
 Author: Marco Merlin
 Author-email: marcomerli@gmail.com
 License: Apache 2.0
-Keywords: python silicon validation
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# cheap_pie
-A python tool for register-based chip verification and validation
-
-"Cheap Pie" is a python tool for register-based chip verification and validation.
-The name is a translitteration of "chip py" for obvious reasons.
-
-Given an input description file for the chip, it provides a register-level and 
-bitfield-level read/write access, through a generic transport layer.
-
-Currently the implemented description input modes are:
-- CMSIS-SVD (https://www.keil.com/pack/doc/CMSIS/SVD/html/svd_Format_pg.html)
-- IP-XACT ( https://www.accellera.org/downloads/standards/ip-xact )
-- SystemRDL (https://www.accellera.org/activities/working-groups/systemrdl)
-
-but it should be relatively easy to add different chip description formats.
-
-Although tested on few real chips (NXP QN9080, I.MX RT1010, K64F),
-cheap_pie parser already supports dozen of devices, listed in the CMSIS-SVD 
-repository https://github.com/posborne/cmsis-svd .
-
-Currently the supported transport layers are jlink and pyocd, but it should be really easy
-to add support for different transport layers, like for instance openSDA, 
-CMSIS-DAP, Total Phase Cheetah, GDB or any other.
-
-Experimental support for pyverilator transport allows to run interactive simulation
-of register blocks generated from SystemRDL source.
-
-Author: Marco Merlin
-Tested on ipython3 (python 3.8.5) on ubuntu 20.04
-
-# IPython Example:
-        %run cheap_pie
-        inval = "0xFFFFFFFF"
-        hal.regs.ADC_ANA_CTRL.setreg(inval)
-        retval = hex(hal.regs.ADC_ANA_CTRL.getreg())
-        assert(literal_eval(inval) == literal_eval(retval))
-
-        # decimal assignement        
-        inval = 2
-        hal.regs.ADC_ANA_CTRL.setreg(inval)
-        retval = hal.regs.ADC_ANA_CTRL.getreg()        
-        assert(inval == retval)
+Description: # cheap_pie
+        A python tool for register-based chip verification and validation
+        
+        "Cheap Pie" is a python tool for register-based chip verification and validation.
+        The name is a translitteration of "chip py" for obvious reasons.
+        
+        Given an input description file for the chip, it provides a register-level and 
+        bitfield-level read/write access, through a generic transport layer.
+        
+        Currently the implemented description input modes are:
+        - CMSIS-SVD (https://www.keil.com/pack/doc/CMSIS/SVD/html/svd_Format_pg.html)
+        - IP-XACT ( https://www.accellera.org/downloads/standards/ip-xact )
+        - SystemRDL (https://www.accellera.org/activities/working-groups/systemrdl)
+        
+        but it should be relatively easy to add different chip description formats.
+        
+        Although tested on few real chips (NXP QN9080, I.MX RT1010, K64F),
+        cheap_pie parser already supports dozen of devices, listed in the CMSIS-SVD 
+        repository https://github.com/posborne/cmsis-svd .
+        
+        Currently the supported transport layers are jlink and pyocd, but it should be really easy
+        to add support for different transport layers, like for instance openSDA, 
+        CMSIS-DAP, Total Phase Cheetah, GDB or any other.
+        
+        Experimental support for pyverilator transport allows to run interactive simulation
+        of register blocks generated from SystemRDL source.
+        
+        Author: Marco Merlin
+        Tested on ipython3 (python 3.8.5) on ubuntu 20.04
         
-        hal.regs.ADC_ANA_CTRL
-        hal.regs.ADC_ANA_CTRL.display()
+        # IPython Example:
+                %run cheap_pie
+                inval = "0xFFFFFFFF"
+                hal.regs.ADC_ANA_CTRL.setreg(inval)
+                retval = hex(hal.regs.ADC_ANA_CTRL.getreg())
+                assert(literal_eval(inval) == literal_eval(retval))
+        
+                # decimal assignement        
+                inval = 2
+                hal.regs.ADC_ANA_CTRL.setreg(inval)
+                retval = hal.regs.ADC_ANA_CTRL.getreg()        
+                assert(inval == retval)
+                
+                hal.regs.ADC_ANA_CTRL
+                hal.regs.ADC_ANA_CTRL.display()
+                        
+                print('Test bitfield methods...')
+                
+                hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM
+                hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.display()
+                hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.display(2)
+                hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.setbit(inval)
+                retval = hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.getbit()
+                assert(inval == retval)
+        
+                # subscriptable register access
+                hal[0]
+                # subscriptable bitfield access
+                hal[0][0]
+                # subscriptable as a dictionary
+                hal['SYSCON_RST_SW_SET']
+                hal['ADC_ANA_CTRL']['ADC_BM']
                 
-        print('Test bitfield methods...')
+                # assignement
+                hal['ADC_ANA_CTRL'] = 1
+                hal['ADC_ANA_CTRL']['ADC_BM'] = 2
+                # dict-based assignement in single register write
+                hal['ADC_ANA_CTRL'] = {'DITHER_EN': 1, 'CHOP_EN': 1, 'INV_CLK': 1}
+        
+                # help
+                hal.regs.ADC_ANA_CTRL.help()
+                ADC core and reference setting regsiter
+                           ADC_BM: 
+                                 : ADC bias current selection.
+                        ADC_ORDER: 
+                                 : 1 to enable SD ADC 2 order mode selection
+                        DITHER_EN: 
+                                 : 1 to enable SD ADC PN Sequence in chopper mode
+                          CHOP_EN: 
+                                 : 1 to enable SD ADC chopper
+                          INV_CLK: 
+                                 : 1 to invert SD ADC Output Clock
+                          VREF_BM: 
+                                 : SD ADC Reference Driver bias current selection.
+                       VREF_BM_X3: 
+                                 : SD ADC Reference Driver bias current triple.
+                       VINN_IN_BM: 
+                                 : PGA VlNN Input Driver bias current selection.
+                      VINN_OUT_BM: 
+                                 : PGA VlNN Output Driver bias current selection.
+                   VINN_OUT_BM_X3: 
+                                 : PGA VlNN Output Driver bias current triple.
+                      ADC_BM_DIV2: 
+                                 : SD ADC bias current half.
+        
+        # CLI Example:
+                # load RT1010 from local svd file under ./devices/
+                # automatically calls ipython and cheap_pie initialization
+                ./cheap_pie.sh -rf MIMXRT1011.svd -t jlink
+        
+                # load K64 from CMSIS-SVD
+                # need to specify vendor for svd not in ./devices/
+                ./cheap_pie.sh -rf MK64F12.svd -ve Freescale -t jlink
+        
+                # calls QN9080 with dummy transport layer 
+                # useful to explore device registers
+                ./cheap_pie.sh -t dummy
+        
+        # Default configurations Examples:
+                # calls QN9080 device with dummy transport layer
+                ./cfgs/cp_qn9080_dummy.sh
+                # calls RT1010 device with jlink transport layer
+                ./cfgs/cp_rt1010_jlink.sh
+                # calls K20 device with dummy transport layer
+                ./cfgs/cp_k20_dummy.sh
+        
+        # Verilator interactive simulation Examples:
+                ./tools/rdl2verilog.py -f ./devices/rdl/basic.rdl
+                ./cheap_pie.sh -dd  ./devices/rdl -rf basic.rdl -fmt rdl -t verilator -topv ./devices/rdl/basic/basic_rf.sv
+        
+        # Install
+        ## From pypi
+                pip3 install cheap_pie
+        ## From github
+                pip3 install git+https://github.com/bat52/cheap_pie.git@master
         
-        hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM
-        hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.display()
-        hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.display(2)
-        hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.setbit(inval)
-        retval = hal.regs.ADC_ANA_CTRL.bitfields.ADC_BM.getbit()
-        assert(inval == retval)
-
-        # subscriptable register access
-        hal[0]
-        # subscriptable bitfield access
-        hal[0][0]
-        # subscriptable as a dictionary
-        hal['SYSCON_RST_SW_SET']
-        hal['ADC_ANA_CTRL']['ADC_BM']
-        
-        # assignement
-        hal['ADC_ANA_CTRL'] = 1
-        hal['ADC_ANA_CTRL']['ADC_BM'] = 2
-        # dict-based assignement in single register write
-        hal['ADC_ANA_CTRL'] = {'DITHER_EN': 1, 'CHOP_EN': 1, 'INV_CLK': 1}
-
-        # help
-        hal.regs.ADC_ANA_CTRL.help()
-        ADC core and reference setting regsiter
-                   ADC_BM: 
-                         : ADC bias current selection.
-                ADC_ORDER: 
-                         : 1 to enable SD ADC 2 order mode selection
-                DITHER_EN: 
-                         : 1 to enable SD ADC PN Sequence in chopper mode
-                  CHOP_EN: 
-                         : 1 to enable SD ADC chopper
-                  INV_CLK: 
-                         : 1 to invert SD ADC Output Clock
-                  VREF_BM: 
-                         : SD ADC Reference Driver bias current selection.
-               VREF_BM_X3: 
-                         : SD ADC Reference Driver bias current triple.
-               VINN_IN_BM: 
-                         : PGA VlNN Input Driver bias current selection.
-              VINN_OUT_BM: 
-                         : PGA VlNN Output Driver bias current selection.
-           VINN_OUT_BM_X3: 
-                         : PGA VlNN Output Driver bias current triple.
-              ADC_BM_DIV2: 
-                         : SD ADC bias current half.
-
-# CLI Example:
-        # load RT1010 from local svd file under ./devices/
-        # automatically calls ipython and cheap_pie initialization
-        ./cheap_pie.sh -rf MIMXRT1011.svd -t jlink
-
-        # load K64 from CMSIS-SVD
-        # need to specify vendor for svd not in ./devices/
-        ./cheap_pie.sh -rf MK64F12.svd -ve Freescale -t jlink
-
-        # calls QN9080 with dummy transport layer 
-        # useful to explore device registers
-        ./cheap_pie.sh -t dummy
-
-# Default configurations Examples:
-        # calls QN9080 device with dummy transport layer
-        ./cfgs/cp_qn9080_dummy.sh
-        # calls RT1010 device with jlink transport layer
-        ./cfgs/cp_rt1010_jlink.sh
-        # calls K20 device with dummy transport layer
-        ./cfgs/cp_k20_dummy.sh
-
-# Verilator interactive simulation Examples:
-        ./tools/rdl2verilog.py -f ./devices/rdl/basic.rdl
-        ./cheap_pie.sh -dd  ./devices/rdl -rf basic.rdl -fmt rdl -t verilator -topv ./devices/rdl/basic/basic_rf.sv
-
-# Install
-## From pypi
-        pip3 install cheap_pie
-## From github
-        pip3 install git+https://github.com/bat52/cheap_pie.git@master
-
-# Dependencies for core (required):        
-        # for XML parsing (used by legacy svd parser and IP-XACT parser)
-        pip3 install untangle
-        # for exporting XML info into a human-readable document
-        pip3 install python-docx
-        # for dumping registers
-        pip3 install hickle
-        # CMSIS-SVD python parser including many svd files https://github.com/posborne/cmsis-svd
-        pip3 install cmsis-svd
-        # SPIRIT IP-XACT parser through ipyxact https://github.com/olofk/ipyxact
-        pip3 install ipyxact                
-        # SystemRDL to register-file verilog
-        https://github.com/hughjackson/PeakRDL-verilog
-        # SystemRDL to IP-XACT
-        https://github.com/SystemRDL/PeakRDL-ipxact
-# Dependencies for validation/transport layers (optional):        
-        # for JLINK
-        pip3 install pylink-square
-        # pyOCD for CMSIS-DAP and JLINK support (only tested in python-venv)
-        pip3 install pyocd
-        # esptool for Espressif devices (not yet functional)
-        pip3 install esptool        
-# Dependencies for verification (optional AND experimental):
-        # verilator
-        https://www.veripool.org/verilator/
-        # pyverilator (python verilator wrapper)
-        https://github.com/csail-csg/pyverilator        
-        # gtkwave
-        http://gtkwave.sourceforge.net/
-
-# Releasing
-
-Releases are published automatically when a tag is pushed to GitHub.
-
-.. code-block:: bash
-
-   # Set next version number
-   export RELEASE=x.x.x
-
-   # Create tags
-   git commit --allow-empty -m "Release $RELEASE"
-   git tag -a $RELEASE -m "Version $RELEASE"
-
-   # Push
-   git push upstream --tags
-
-# Register description formats
-regtool from opentitan project seems similar, using JSON to represent chip/IP structure, and I2C transport
-https://docs.opentitan.org/doc/rm/register_tool/
-
-custom input, output: verilog, VHDL, YAML, JSON, TOML, Spreadsheet (XLSX, XLS, OSD, CSV)
-https://github.com/rggen/rggen
-
-convert ipxact register file description into verilog register bank
-https://github.com/oddball/ipxact2systemverilog
-
-# Others	
-In conjunction with pyVISA (https://pyvisa.readthedocs.io/en/master/), used for 
-instument control, it provides a simple and fully python-contained environment
-for silicon validation.
-
-Graphical Render of bitfield structures
-https://github.com/wavedrom/bitfield
-
-C++ register/bitfields access (including generation from svd)
-https://github.com/thanks4opensource/regbits
-
-STM C++ regbits implementation
-https://github.com/thanks4opensource/regbits_stm
-
-a barebone embedded library generator
-https://modm.io/
-
-hardware descriptions for AVR and STM32 devices
-https://github.com/modm-io/modm-devices
-
-STM32 Peripheral Access Crates (from svd)
-https://github.com/stm32-rs/stm32-rs
-
-Banner created with pyfiglet
-https://www.devdungeon.com/content/create-ascii-art-text-banners-python#install_pyfiglet
-
-Cheap Pie is modeled after an original Octave/Matlab implementation that cannot
-be shared due to licensing reasons. The original code was converted to python
-using SMOP ( https://github.com/ripple-neuro/smop ).
-
-
+        # Dependencies for core (required):        
+                # for XML parsing (used by legacy svd parser and IP-XACT parser)
+                pip3 install untangle
+                # for exporting XML info into a human-readable document
+                pip3 install python-docx
+                # for dumping registers
+                pip3 install hickle
+                # CMSIS-SVD python parser including many svd files https://github.com/posborne/cmsis-svd
+                pip3 install cmsis-svd
+                # SPIRIT IP-XACT parser through ipyxact https://github.com/olofk/ipyxact
+                pip3 install ipyxact                
+                # SystemRDL to register-file verilog
+                https://github.com/hughjackson/PeakRDL-verilog
+                # SystemRDL to IP-XACT
+                https://github.com/SystemRDL/PeakRDL-ipxact
+        # Dependencies for validation/transport layers (optional):        
+                # for JLINK
+                pip3 install pylink-square
+                # pyOCD for CMSIS-DAP and JLINK support (only tested in python-venv)
+                pip3 install pyocd
+                # esptool for Espressif devices (not yet functional)
+                pip3 install esptool        
+        # Dependencies for verification (optional AND experimental):
+                # verilator
+                https://www.veripool.org/verilator/
+                # pyverilator (python verilator wrapper)
+                https://github.com/csail-csg/pyverilator        
+                # gtkwave
+                http://gtkwave.sourceforge.net/
+        
+        # Releasing
+        
+        Releases are published automatically when a tag is pushed to GitHub.
+        
+        .. code-block:: bash
+        
+           # Set next version number
+           export RELEASE=x.x.x
+        
+           # Create tags
+           git commit --allow-empty -m "Release $RELEASE"
+           git tag -a $RELEASE -m "Version $RELEASE"
+        
+           # Push
+           git push upstream --tags
+        
+        # Register description formats
+        regtool from opentitan project seems similar, using JSON to represent chip/IP structure, and I2C transport
+        https://docs.opentitan.org/doc/rm/register_tool/
+        
+        custom input, output: verilog, VHDL, YAML, JSON, TOML, Spreadsheet (XLSX, XLS, OSD, CSV)
+        https://github.com/rggen/rggen
+        
+        convert ipxact register file description into verilog register bank
+        https://github.com/oddball/ipxact2systemverilog
+        
+        # Others	
+        In conjunction with pyVISA (https://pyvisa.readthedocs.io/en/master/), used for 
+        instument control, it provides a simple and fully python-contained environment
+        for silicon validation.
+        
+        Graphical Render of bitfield structures
+        https://github.com/wavedrom/bitfield
+        
+        C++ register/bitfields access (including generation from svd)
+        https://github.com/thanks4opensource/regbits
+        
+        STM C++ regbits implementation
+        https://github.com/thanks4opensource/regbits_stm
+        
+        a barebone embedded library generator
+        https://modm.io/
+        
+        hardware descriptions for AVR and STM32 devices
+        https://github.com/modm-io/modm-devices
+        
+        STM32 Peripheral Access Crates (from svd)
+        https://github.com/stm32-rs/stm32-rs
+        
+        Banner created with pyfiglet
+        https://www.devdungeon.com/content/create-ascii-art-text-banners-python#install_pyfiglet
+        
+        Cheap Pie is modeled after an original Octave/Matlab implementation that cannot
+        be shared due to licensing reasons. The original code was converted to python
+        using SMOP ( https://github.com/ripple-neuro/smop ).
+        
+Keywords: python silicon validation
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `cheap_pie-1.0.0/src/cheap_pie.egg-info/SOURCES.txt` & `cheap_pie-1.0.1/src/cheap_pie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

