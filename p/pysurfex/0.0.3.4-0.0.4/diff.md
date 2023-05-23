# Comparing `tmp/pysurfex-0.0.3.4.tar.gz` & `tmp/pysurfex-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysurfex-0.0.3.4.tar", max compression
+gzip compressed data, was "pysurfex-0.0.4.tar", max compression
```

## Comparing `pysurfex-0.0.3.4.tar` & `pysurfex-0.0.4.tar`

### file list

```diff
@@ -1,44 +1,46 @@
--rw-r--r--   0        0        0     3318 2023-05-02 21:46:14.544019 pysurfex-0.0.3.4/README.rst
--rw-r--r--   0        0        0     5202 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pyproject.toml
--rw-r--r--   0        0        0      142 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/__init__.py
--rw-r--r--   0        0        0    30965 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/binary_input.py
--rw-r--r--   0        0        0    18837 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/bufr.py
--rw-r--r--   0        0        0    10460 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/cache.py
--rw-r--r--   0        0        0    19335 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/cfg/config.yml
--rw-r--r--   0        0        0     8985 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/cfg/config_exp_surfex.toml
--rw-r--r--   0        0        0      135 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/cfg/default_thredds.cfg
--rw-r--r--   0        0        0     5253 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/cfg/first_guess.yml
--rw-r--r--   0        0        0      192 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/cfg/qc_codes.json
--rw-r--r--   0        0        0      370 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/cfg/user.yml
--rw-r--r--   0        0        0    62389 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/cli.py
--rw-r--r--   0        0        0    62271 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/cmd_parsing.py
--rw-r--r--   0        0        0    32663 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/configuration.py
--rw-r--r--   0        0        0     1291 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/datetime_utils.py
--rw-r--r--   0        0        0     8511 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/ecoclimap.py
--rw-r--r--   0        0        0     3891 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/fa.py
--rw-r--r--   0        0        0    58096 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/file.py
--rw-r--r--   0        0        0    35668 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/forcing.py
--rw-r--r--   0        0        0    33675 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/geo.py
--rw-r--r--   0        0        0    22471 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/grib.py
--rw-r--r--   0        0        0    14928 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/input_methods.py
--rw-r--r--   0        0        0    18924 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/interpolation.py
--rw-r--r--   0        0        0   100050 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/namelist.py
--rw-r--r--   0        0        0    34770 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/netcdf.py
--rw-r--r--   0        0        0    37729 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/obs.py
--rw-r--r--   0        0        0     4483 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/observation.py
--rw-r--r--   0        0        0    12016 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/obsmon.py
--rw-r--r--   0        0        0     6415 2023-05-02 21:46:14.552019 pysurfex-0.0.3.4/pysurfex/obsoul.py
--rw-r--r--   0        0        0    16227 2023-05-02 21:46:14.556019 pysurfex-0.0.3.4/pysurfex/platform.py
--rw-r--r--   0        0        0       20 2023-05-02 21:46:14.556019 pysurfex-0.0.3.4/pysurfex/plot.py
--rw-r--r--   0        0        0    17168 2023-05-02 21:46:14.556019 pysurfex-0.0.3.4/pysurfex/read.py
--rw-r--r--   0        0        0    11682 2023-05-02 21:46:14.556019 pysurfex-0.0.3.4/pysurfex/run.py
--rw-r--r--   0        0        0     2254 2023-05-02 21:46:14.556019 pysurfex-0.0.3.4/pysurfex/settings/assimilation.json
--rw-r--r--   0        0        0        0 2023-05-02 21:46:14.556019 pysurfex-0.0.3.4/pysurfex/settings/filetype.json
--rw-r--r--   0        0        0     1075 2023-05-02 21:46:14.556019 pysurfex-0.0.3.4/pysurfex/settings/forecast.json
--rw-r--r--   0        0        0     1305 2023-05-02 21:46:14.556019 pysurfex-0.0.3.4/pysurfex/settings/pgd.json
--rw-r--r--   0        0        0      952 2023-05-02 21:46:14.556019 pysurfex-0.0.3.4/pysurfex/settings/prep.json
--rw-r--r--   0        0        0     3499 2023-05-02 21:46:14.556019 pysurfex-0.0.3.4/pysurfex/timeseries.py
--rw-r--r--   0        0        0    67688 2023-05-02 21:46:14.556019 pysurfex-0.0.3.4/pysurfex/titan.py
--rw-r--r--   0        0        0     3463 2023-05-02 21:46:14.556019 pysurfex-0.0.3.4/pysurfex/util.py
--rw-r--r--   0        0        0    19977 2023-05-02 21:46:14.556019 pysurfex-0.0.3.4/pysurfex/variable.py
--rw-r--r--   0        0        0     4606 1970-01-01 00:00:00.000000 pysurfex-0.0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     3318 2023-05-23 10:11:39.709958 pysurfex-0.0.4/README.rst
+-rw-r--r--   0        0        0     5200 2023-05-23 10:11:39.713958 pysurfex-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      142 2023-05-23 10:11:39.713958 pysurfex-0.0.4/pysurfex/__init__.py
+-rw-r--r--   0        0        0    25713 2023-05-23 10:11:39.713958 pysurfex-0.0.4/pysurfex/binary_input.py
+-rw-r--r--   0        0        0    27141 2023-05-23 10:11:39.713958 pysurfex-0.0.4/pysurfex/binary_input_legacy.py
+-rw-r--r--   0        0        0    18837 2023-05-23 10:11:39.713958 pysurfex-0.0.4/pysurfex/bufr.py
+-rw-r--r--   0        0        0    10460 2023-05-23 10:11:39.713958 pysurfex-0.0.4/pysurfex/cache.py
+-rw-r--r--   0        0        0    19335 2023-05-23 10:11:39.713958 pysurfex-0.0.4/pysurfex/cfg/config.yml
+-rw-r--r--   0        0        0     8835 2023-05-23 10:11:39.713958 pysurfex-0.0.4/pysurfex/cfg/config_exp_surfex.toml
+-rw-r--r--   0        0        0      135 2023-05-23 10:11:39.713958 pysurfex-0.0.4/pysurfex/cfg/default_thredds.cfg
+-rw-r--r--   0        0        0     5253 2023-05-23 10:11:39.713958 pysurfex-0.0.4/pysurfex/cfg/first_guess.yml
+-rw-r--r--   0        0        0      192 2023-05-23 10:11:39.713958 pysurfex-0.0.4/pysurfex/cfg/qc_codes.json
+-rw-r--r--   0        0        0      370 2023-05-23 10:11:39.713958 pysurfex-0.0.4/pysurfex/cfg/user.yml
+-rw-r--r--   0        0        0    65246 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/cli.py
+-rw-r--r--   0        0        0    61684 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/cmd_parsing.py
+-rw-r--r--   0        0        0    32484 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/configuration.py
+-rw-r--r--   0        0        0     1291 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/datetime_utils.py
+-rw-r--r--   0        0        0     8730 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/ecoclimap.py
+-rw-r--r--   0        0        0     3891 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/fa.py
+-rw-r--r--   0        0        0    58096 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/file.py
+-rw-r--r--   0        0        0    35668 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/forcing.py
+-rw-r--r--   0        0        0    32941 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/geo.py
+-rw-r--r--   0        0        0    22471 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/grib.py
+-rw-r--r--   0        0        0    14928 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/input_methods.py
+-rw-r--r--   0        0        0    18924 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/interpolation.py
+-rw-r--r--   0        0        0    24223 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/namelist.py
+-rw-r--r--   0        0        0   100554 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/namelist_legacy.py
+-rw-r--r--   0        0        0    34770 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/netcdf.py
+-rw-r--r--   0        0        0    37729 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/obs.py
+-rw-r--r--   0        0        0     4483 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/observation.py
+-rw-r--r--   0        0        0    12016 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/obsmon.py
+-rw-r--r--   0        0        0     6415 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/obsoul.py
+-rw-r--r--   0        0        0    18146 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/platform_deps.py
+-rw-r--r--   0        0        0       20 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/plot.py
+-rw-r--r--   0        0        0    17168 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/read.py
+-rw-r--r--   0        0        0    11679 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/run.py
+-rw-r--r--   0        0        0     2254 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/settings/assimilation.json
+-rw-r--r--   0        0        0        0 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/settings/filetype.json
+-rw-r--r--   0        0        0     1075 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/settings/forecast.json
+-rw-r--r--   0        0        0     1305 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/settings/pgd.json
+-rw-r--r--   0        0        0      952 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/settings/prep.json
+-rw-r--r--   0        0        0     3499 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/timeseries.py
+-rw-r--r--   0        0        0    67688 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/titan.py
+-rw-r--r--   0        0        0     3463 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/util.py
+-rw-r--r--   0        0        0    19977 2023-05-23 10:11:39.717959 pysurfex-0.0.4/pysurfex/variable.py
+-rw-r--r--   0        0        0     4604 1970-01-01 00:00:00.000000 pysurfex-0.0.4/PKG-INFO
```

### Comparing `pysurfex-0.0.3.4/README.rst` & `pysurfex-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pyproject.toml` & `pysurfex-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
     name = "pysurfex"
-    version = "0.0.3.4"
+    version = "0.0.4"
     description = "Python API to SURFEX"
     authors = ["Trygve Aspelien"]
     license = "MIT"
     readme = "README.rst"
     repository = "https://github.com/metno/pysurfex"
     documentation = "https://metno.github.io/pysurfex/"
```

### Comparing `pysurfex-0.0.3.4/pysurfex/binary_input.py` & `pysurfex-0.0.4/pysurfex/binary_input_legacy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,178 +1,31 @@
 """Input data for surfex binaries."""
-import json
 import logging
 import os
-import subprocess
-from abc import ABC, abstractmethod
+from warnings import warn
 
+from .binary_input import JsonInputData
 from .datetime_utils import as_datetime, as_timedelta
 from .ecoclimap import Ecoclimap, EcoclimapSG, ExternalSurfexInputFile
 from .file import AsciiSurfexFile, FaSurfexFile, NCSurfexFile
 
 
-class InputDataToSurfexBinaries(ABC):
-    """Abstract input data."""
-
-    @abstractmethod
-    def __init__(self):
-        """Construct."""
-        return NotImplementedError
-
-    @abstractmethod
-    def prepare_input(self):
-        """Prepare input."""
-        return NotImplementedError
-
-
-class OutputDataFromSurfexBinaries(ABC):
-    """Abstract output data."""
-
-    @abstractmethod
-    def __init__(self):
-        """Construct."""
-        return NotImplementedError
-
-    @abstractmethod
-    def archive_files(self):
-        """Archive files."""
-        return NotImplementedError
-
-
-class JsonOutputData(OutputDataFromSurfexBinaries):
-    """Output data."""
-
-    def __init__(self, data):
-        """Output data from dict.
-
-        Args:
-            data (dict): Output data.
-
-        """
-        OutputDataFromSurfexBinaries.__init__(self)
-        self.data = data
-
-    def archive_files(self):
-        """Archive files."""
-        for output_file, target in self.data.items():
-
-            logging.info("%s -> %s", output_file, target)
-            command = "mv"
-            if isinstance(target, dict):
-                for key in target:
-                    logging.debug("%s %s %s", output_file, key, target[key])
-                    command = target[key]
-                    target = key
-
-            cmd = command + " " + output_file + " " + target
-            try:
-                logging.info(cmd)
-                subprocess.check_call(cmd, shell=True)  # noqaS602
-            except IOError:
-                logging.error("%s failed", cmd)
-                raise RuntimeError(cmd + " failed") from IOError
-
-
-class JsonOutputDataFromFile(JsonOutputData):
-    """JSON output data."""
-
-    def __init__(self, file):
-        """Construct from json file."""
-        with open(file, mode="r", encoding="utf-8") as file_handler:
-            data = json.load(file_handler)
-        JsonOutputData.__init__(self, data)
-
-    def archive_files(self):
-        """Archive files."""
-        JsonOutputData.archive_files(self)
-
-
-class JsonInputData(InputDataToSurfexBinaries):
-    """JSON input data."""
-
-    def __init__(self, data):
-        """Construct input data.
-
-        Args:
-            data (dict): Input data.
-        """
-        InputDataToSurfexBinaries.__init__(self)
-        self.data = data
-
-    def prepare_input(self):
-        """Prepare input."""
-        for target, input_file in self.data.items():
-
-            logging.info("%s -> %s", target, input_file)
-            logging.debug(os.path.realpath(target))
-            command = None
-            if isinstance(input_file, dict):
-                for key in input_file:
-                    logging.debug(key)
-                    logging.debug(input_file[key])
-                    command = str(input_file[key])
-                    input_file = str(key)
-                    command = command.replace("@INPUT@", input_file)
-                    command = command.replace("@TARGET@", target)
-
-            if os.path.realpath(target) == os.path.realpath(input_file):
-                logging.info("Target and input file is the same file")
-            else:
-                if command is None:
-                    cmd = "ln -sf " + input_file + " " + target
-                else:
-                    cmd = command
-                try:
-                    logging.info(cmd)
-                    subprocess.check_call(cmd, shell=True)  # noqaS602
-                except IOError:
-                    raise (cmd + " failed") from IOError
-
-    def add_data(self, data):
-        """Add data.
-
-        Args:
-            data (dict): Data to add
-        """
-        for key in data:
-            value = data[key]
-            self.data.update({key: value})
-
-
-class JsonInputDataFromFile(JsonInputData):
-    """JSON input data."""
-
-    def __init__(self, file):
-        """Construct JSON input data.
-
-        Args:
-            file (str): JSON file name
-
-        """
-        with open(file, mode="r", encoding="utf-8") as file_handler:
-            data = json.load(file_handler)
-        JsonInputData.__init__(self, data)
-
-    def prepare_input(self):
-        """Prepare input."""
-        JsonInputData.prepare_input(self)
-
-
 class PgdInputData(JsonInputData):
     """PGD input."""
 
     def __init__(self, config, system_file_paths, check_existence=True):
         """Construct PD input.
 
         Args:
             config (Configuration): Surfex configuration
             system_file_paths (SystemFilePaths): System file paths
             check_existence (bool, optional): Check if input files exist. Defaults to True.
 
         """
+        warn("This is deprecated", DeprecationWarning, stacklevel=2)
         # Ecoclimap settings
         eco_sg = config.get_setting("SURFEX#COVER#SG")
         if eco_sg:
             ecoclimap = EcoclimapSG(config, system_file_paths=system_file_paths)
         else:
             ecoclimap = Ecoclimap(config, system_file_paths=system_file_paths)
 
@@ -265,14 +118,15 @@
             config (Configuration): Surfex configuration
             system_file_paths (SystemFilePaths): System file paths
             check_existence (bool, optional): Check if input files exist. Defaults to True.
             prep_file (str, optional): Prep input file. Defaults to None.
             prep_pgdfile (str, optional): Filetype for prep input. Defaults to None.
 
         """
+        warn("This is deprecated", DeprecationWarning, stacklevel=2)
         data = {}
         # Ecoclimap settings
         eco_sg = config.get_setting("SURFEX#COVER#SG")
         if not eco_sg:
             ecoclimap = Ecoclimap(config, system_file_paths)
             data.update(ecoclimap.set_bin_files(check_existence=check_existence))
 
@@ -314,14 +168,15 @@
             system_file_paths (SystemFilePaths): System file paths
             check_existence (bool, optional): Check if input files exist. Defaults to True.
 
         Raises:
             NotImplementedError: Filetype not implemented
 
         """
+        warn("This is deprecated", DeprecationWarning, stacklevel=2)
         data = {}
         # Ecoclimap settings
         eco_sg = config.get_setting("SURFEX#COVER#SG")
         if not eco_sg:
             ecoclimap = Ecoclimap(config, system_file_paths)
             data.update(ecoclimap.set_bin_files(check_existence=check_existence))
 
@@ -349,14 +204,15 @@
 
         Args:
             config (Configuration): Surfex configuration
             system_file_paths (SystemFilePaths): System file paths
             check_existence (bool, optional): Check if input files exist. Defaults to True.
 
         """
+        warn("This is deprecated", DeprecationWarning, stacklevel=2)
         data = {}
         # Ecoclimap settings
         eco_sg = config.get_setting("SURFEX#COVER#SG")
         if not eco_sg:
             ecoclimap = Ecoclimap(config, system_file_paths)
             data.update(ecoclimap.set_bin_files(check_existence=check_existence))
 
@@ -382,14 +238,15 @@
             system_file_paths (SystemFilePaths): System file paths
             check_existence (bool, optional): Check if input files exist. Defaults to True.
             masterodb (bool, optional): Files produced with masterodb. Defaults to True.
             perturbed_file_pattern (str, optional): File pattern for perturbed files. Defaults to None.
             dtg (datetime, optional): Basetime. Defaults to None.
 
         """
+        warn("This is deprecated", DeprecationWarning, stacklevel=2)
         self.config = config
         self.system_file_paths = system_file_paths
         self.file_paths = ExternalSurfexInputFile(self.system_file_paths)
         if dtg is not None:
             if isinstance(dtg, str):
                 dtg = as_datetime(dtg)
         self.dtg = dtg
```

### Comparing `pysurfex-0.0.3.4/pysurfex/bufr.py` & `pysurfex-0.0.4/pysurfex/bufr.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pysurfex/cache.py` & `pysurfex-0.0.4/pysurfex/cache.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pysurfex/cfg/config.yml` & `pysurfex-0.0.4/pysurfex/cfg/config.yml`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pysurfex/cfg/config_exp_surfex.toml` & `pysurfex-0.0.4/pysurfex/cfg/config_exp_surfex.toml`

 * *Files 4% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 CFORCING_FILETYPE = "NETCDF"        # Offline surfex forcing format (NETCDF/ASCII)
 XTSTEP = 600                        # Surfex time step (Only used in the binary OFFLINE)
 XTSTEP_OUTPUT = 21600.0             # Output interval from the binary OFFLINE
 LSPLIT_PATCH = true                 # Split patches into separate variables in output files
 LSELECT = true                      # Only write selected diagnostics
 
 [SURFEX.COVER]                      # Land cover information
-YCOVER = "ECOCLIMAP_2_5_p.dir"      # Version of ECOCLIMAP for surfex (1,2,SG)
+YCOVER = "ECOCLIMAP_2_5_p"          # Version of ECOCLIMAP for surfex (1,2,SG)
                                     # Available versions are 1.1-1.5,2.0-2.2.1,SG and 2.5_plus if you use FLake
                                     # SG represents SecondGeneration and is now availbale for test on ECMWF. However,
                                     # please note that SG is not yet compatible with any availbale lake data base.
 SG = false                          # ECOCLIMAP second generation
-H_TREE = "new_ht_c.dir"                 # SG tree height
-ALBNIR_SOIL = 'ALB_SAT_NI_@MM@@CDD@_c.dir' # SG soil NIR albedo
-ALBNIR_VEG = 'ALB_SAT_NI_@MM@@CDD@_c.dir'  # SG vegetation NIR albedo
-ALBVIS_SOIL = 'ALB_SAT_VI_@MM@@CDD@_c.dir' # SG soil visible albedo
-ALBVIS_VEG = 'ALB_SAT_VI_@MM@@CDD@_c.dir'  # SG vgetation visible albedo
-LAI = 'LAI_SAT_@MM@@CDD@_c.dir'             # SG Leaf area index
+H_TREE = "new_ht_c"                 # SG tree height
+ALBNIR_SOIL = 'ALB_SAT_NI_@MM@@CDD@_c' # SG soil NIR albedo
+ALBNIR_VEG = 'ALB_SAT_NI_@MM@@CDD@_c'  # SG vegetation NIR albedo
+ALBVIS_SOIL = 'ALB_SAT_VI_@MM@@CDD@_c' # SG soil visible albedo
+ALBVIS_VEG = 'ALB_SAT_VI_@MM@@CDD@_c'  # SG vgetation visible albedo
+LAI = 'LAI_SAT_@MM@@CDD@_c'             # SG Leaf area index
 
 [SURFEX.ZS]                         # Orography
-YZS = "gmted2010.dir"               # Database with orography: "gmted2010"|"gtopo30"
+YZS = "gmted2010"                   # Database with orography: "gmted2010"|"gtopo30"
 
 [SURFEX.PARAMETERS]
 XRIMAX = 0.2                        # Maximum allowed Richardson number in the surface layer
 
 [SURFEX.TILES]                      # Define which tile schemes to use
 SEA = "SEAFLX"                      # Sea scheme
 INLAND_WATER = "FLAKE"              # Treatment of lakes in surfex (WATFLX|FLAKE)
@@ -75,23 +75,23 @@
 [SURFEX.ISBA]
 SCHEME = "3-L"                      # Type of ISBA scheme in SURFEX. Options: "3-L"|"2-L"|"DIF"
 NPATCH = 2                          # Number of patches over land in SURFEX (see also LISBA_CANOPY)
 MEB = false                         # Enable Multi Energy Budget (MEB) model
 CANOPY = false                      # Activates surface boundary multi layer scheme over land in SURFEX
                                     # (must be false for NPATCH>1)
 SNOW = "D95"                        # Type of snow scheme in SURFEX. Options: "D95" and "3-L"
-YSOC_TOP = "soc_top.dir"            # Soil organic carbon data. Options: "soc_top.dir"
-YSOC_SUB = "soc_sub.dir"            # Soil organic carbon data. Options: "soc_sub.dir"
+YSOC_TOP = "soc_top"                # Soil organic carbon data. Options: "soc_top"
+YSOC_SUB = "soc_sub"                # Soil organic carbon data. Options: "soc_sub"
 
-YSAND = 'sand_fao.dir'              # Soil texture input data: "sand_fao.dir"|"SAND_HWSD_MOY_V2.dir"|"sand_SOILGRID.dir"
+YSAND = 'sand_fao'                  # Soil texture input data: "sand_fao"|"SAND_HWSD_MOY_V2"|"sand_SOILGRID"
                                     # suffix json assumes namelist values provided as a json file
 
-YCLAY = "clay_fao.dir"              # Soil texture input data: "clay_fao.dir"|"CLAY_HWSD_MOY_V2.dir"|"clay_SOILGRID.dir"
+YCLAY = "clay_fao"                  # Soil texture input data: "clay_fao"|"CLAY_HWSD_MOY_V2"|"clay_SOILGRID"
                                     # suffix json assumes namelist values provided as a json file
-PERTSURF = false                    # Perturb surface parameters
+PERTSURF = true                    # Perturb surface parameters
 XCGMAX = 2.0E-5                     # Maximum value for soil heat capacity; default=2.0E-5
 XCSMAX = 2.0E-4                     # Maximum value for snow heat capacity; default=2.0E-4
 
 # Sub-grid-scale orography settings
 [SURFEX.SSO]
 SCHEME = "NONE"                     # SSO scheme used in SURFEX "NONE"|"'Z01D'"|"'BE04'"|"'OROT'"
 
@@ -132,15 +132,14 @@
 LOBSHEADER = false                          # ASCII observation file has header
 CFILE_FORMAT_OBS = "ASCII"                  # File format for observations when using SODA: "ASCII"|"FA"
 LOBSNAT = false                             # Observation ASCII file only contains nature points
 COBS_M = ["T2M","HU2M","WG2 ","LAI","SWE"]  # Observation types
 NNCO = [1, 1, 0, 0, 1]                      # Active observation types
 XERROBS_M = [1.0, 0.1, 0.1, 0.1, 20.0]      # Observation error (used in EKF)
 LSWE = false                                # Assimilate SWE, if false assimilate snow depth
-NOBSTYPE_M=2                                # Number of assimilated observations in the EnKF
 
 [SURFEX.ASSIM.SEA]
 CFILE_FORMAT_SST = "ASCII"           # File format for SST input when using SODA and SEA == "INPUT": "ASCII"|"FA"
 LREAD_SST_FROM_FILE = true           # When SEA == INPUT read SST from external file
 LEXTRAP_SEA = false                  # Extrapolate sea variables to points having LSM < 0.5
 LECSST = true                        # SST from ECMWF
```

### Comparing `pysurfex-0.0.3.4/pysurfex/cfg/first_guess.yml` & `pysurfex-0.0.4/pysurfex/cfg/first_guess.yml`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pysurfex/cli.py` & `pysurfex-0.0.4/pysurfex/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 try:
     import matplotlib.pyplot as plt
 except ModuleNotFoundError:
     plt = None
 
 
-from .binary_input import (
+from .binary_input import JsonOutputDataFromFile
+from .binary_input_legacy import (
     InlineForecastInputData,
-    JsonOutputDataFromFile,
     OfflineInputData,
     PgdInputData,
     PrepInputData,
     SodaInputData,
 )
 from .cache import Cache
 from .cmd_parsing import (
@@ -55,26 +55,27 @@
 from .datetime_utils import as_datetime, as_datetime_args, as_timedelta
 from .file import PGDFile, PREPFile, SurfexFileVariable, SURFFile
 from .forcing import modify_forcing, run_time_loop, set_forcing_config
 from .geo import LonLatVal, get_geo_object, set_domain, shape2ign
 from .grib import Grib1Variable, Grib2Variable
 from .input_methods import create_obsset_file, get_datasources, set_geo_from_obs_set
 from .interpolation import horizontal_oi
-from .namelist import BaseNamelist, Namelist
+from .namelist import NamelistGenerator
+from .namelist_legacy import BaseNamelist, Namelist
 from .netcdf import (
     create_netcdf_first_guess_template,
     oi2soda,
     read_cryoclim_nc,
     read_first_guess_netcdf_file,
     read_sentinel_nc,
     write_analysis_netcdf_file,
 )
 from .obs import Observation, sm_obs_sentinel, snow_pseudo_obs_cryoclim
 from .obsmon import write_obsmon_sqlite_file
-from .platform import SystemFilePathsFromFile
+from .platform_deps import SystemFilePathsFromFile
 from .read import ConvertedInput, Converter
 from .run import BatchJob, Masterodb, PerturbedOffline, SURFEXBinary
 from .titan import (
     TitanDataSet,
     dataset_from_file,
     define_quality_control,
     merge_json_qc_data_sets,
@@ -288,14 +289,27 @@
             check_existence = False
 
     dtg = None
     if "dtg" in kwargs:
         if kwargs["dtg"] is not None and isinstance(kwargs["dtg"], str):
             dtg = as_datetime(kwargs["dtg"])
             kwargs.update({"dtg": dtg})
+        if dtg is not None:
+            config.update_setting("SURFEX#SODA#HH", f"{dtg.hour:02d}")
+    try:
+        basetime = kwargs["basetime"]
+        if isinstance(basetime, str):
+            basetime = as_datetime(basetime)
+    except KeyError:
+        basetime = None
+
+    try:
+        input_binary_data = kwargs["input_binary_data"]
+    except KeyError:
+        input_binary_data = None
 
     # TODO
     perturbed_file_pattern = None
     if perturbed_file_pattern in kwargs:
         perturbed_file_pattern = kwargs["perturbed_file_pattern"]
 
     pgd_file_path = kwargs["pgd"]
@@ -312,40 +326,60 @@
     if archive is not None:
         if os.path.exists(archive):
             my_archive = JsonOutputDataFromFile(archive)
         else:
             raise FileNotFoundError
 
     if mode == "forecast":
-        input_data = InlineForecastInputData(
-            config, system_file_paths, check_existence=check_existence
-        )
         mode = "offline"
     elif mode == "canari":
-        input_data = SodaInputData(
-            config,
-            system_file_paths,
-            check_existence=check_existence,
-            perturbed_file_pattern=perturbed_file_pattern,
-            dtg=dtg,
-        )
         mode = "soda"
     else:
         raise NotImplementedError(mode + " is not implemented!")
 
-    blocks = False
-    if blocks:
-        my_settings = Namelist(
-            mode, config, namelist_path, dtg=dtg, fcint=3
-        ).get_namelist()
-    else:
-        my_settings = BaseNamelist(
-            mode, config, namelist_path, dtg=dtg, fcint=3
-        ).get_namelist()
-    geo.update_namelist(my_settings)
+    if os.path.isfile(namelist_path):
+        with open(namelist_path, mode="r", encoding="utf-8") as file_handler:
+            nam_defs = yaml.safe_load(file_handler)
+        nam_gen = NamelistGenerator(mode, config, nam_defs)
+        my_settings = nam_gen.nml
+        if input_binary_data is None:
+            raise RuntimeError("input_binary_data not set")
+        with open(input_binary_data, mode="r", encoding="utf-8") as file_handler:
+            input_binary_data = json.load(file_handler)
+        input_data = nam_gen.input_data_from_namelist(
+            input_binary_data, system_file_paths, validtime=dtg, basetime=basetime
+        )
+    elif os.path.isdir(namelist_path):
+        if mode == "offline":
+            input_data = InlineForecastInputData(
+                config, system_file_paths, check_existence=check_existence
+            )
+        elif mode == "soda":
+            input_data = SodaInputData(
+                config,
+                system_file_paths,
+                check_existence=check_existence,
+                perturbed_file_pattern=perturbed_file_pattern,
+                dtg=dtg,
+            )
+        else:
+            raise NotImplementedError(mode + " is not implemented!")
+
+        blocks = False
+        if blocks:
+            my_settings = Namelist(
+                mode, config, namelist_path, dtg=dtg, fcint=3
+            ).get_namelist()
+        else:
+            my_settings = BaseNamelist(
+                mode, config, namelist_path, dtg=dtg, fcint=3
+            ).get_namelist()
+        geo.update_namelist(my_settings)
+    else:
+        raise NotImplementedError
 
     # Create input
     my_format = my_settings["nam_io_offline"]["csurf_filetype"]
     my_pgdfile = my_settings["nam_io_offline"]["cpgdfile"]
     my_prepfile = my_settings["nam_io_offline"]["cprepfile"]
     my_surffile = my_settings["nam_io_offline"]["csurffile"]
     lfagmap = False
@@ -432,88 +466,85 @@
     if "tolerate_missing" in kwargs:
         if kwargs["tolerate_missing"]:
             check_existence = False
 
     prep_input_file = None
     if "prep_file" in kwargs:
         prep_input_file = kwargs["prep_file"]
+    config.update_setting("SURFEX#PREP#FILE_WITH_PATH", prep_input_file)
+    basename = prep_input_file
+    if basename is not None:
+        basename = os.path.basename(basename)
+    config.update_setting("SURFEX#PREP#FILE", basename)
     prep_input_pgdfile = None
     if "prep_pgdfile" in kwargs:
         prep_input_pgdfile = kwargs["prep_pgdfile"]
+    config.update_setting("SURFEX#PREP#PGDFILE_WITH_PATH", prep_input_pgdfile)
+    basename = prep_input_pgdfile
+    if basename is not None:
+        basename = os.path.basename(basename)
+    config.update_setting("SURFEX#PREP#FILEPGD", basename)
     prep_input_filetype = None
     if "prep_filetype" in kwargs:
         prep_input_filetype = kwargs["prep_filetype"]
+    config.update_setting("SURFEX#PREP#FILETYPE", prep_input_filetype)
     prep_input_pgdfiletype = None
     if "prep_pgdfiletype" in kwargs:
         prep_input_pgdfiletype = kwargs["prep_pgdfiletype"]
+    config.update_setting("SURFEX#PREP#FILEPGDTYPE", prep_input_pgdfiletype)
 
     # TODO
     perturbed_file_pattern = None
     if perturbed_file_pattern in kwargs:
         perturbed_file_pattern = kwargs["perturbed_file_pattern"]
 
     dtg = None
     if "dtg" in kwargs:
         if kwargs["dtg"] is not None and isinstance(kwargs["dtg"], str):
             dtg = as_datetime(kwargs["dtg"])
             kwargs.update({"dtg": dtg})
+    if dtg is not None:
+        config.update_setting("SURFEX#PREP#NYEAR", dtg.year)
+        config.update_setting("SURFEX#PREP#NMONTH", dtg.month)
+        config.update_setting("SURFEX#PREP#NDAY", dtg.day)
+        xtime = (dtg - dtg.replace(hour=0, second=0, microsecond=0)).total_seconds()
+        config.update_setting("SURFEX#PREP#XTIME", xtime)
+        config.update_setting("SURFEX#SODA#HH", f"{dtg.hour:02d}")
 
     logging.debug("kwargs: %s", str(kwargs))
-    if mode == "pgd":
-        pgd = True
-        need_pgd = False
-        need_prep = False
-        input_data = PgdInputData(
-            config, system_file_paths, check_existence=check_existence
-        )
-    elif mode == "prep":
-        prep = True
-        need_prep = False
-        input_data = PrepInputData(
-            config,
-            system_file_paths,
-            check_existence=check_existence,
-            prep_file=prep_input_file,
-            prep_pgdfile=prep_input_pgdfile,
-        )
-    elif mode == "offline":
-        input_data = OfflineInputData(
-            config, system_file_paths, check_existence=check_existence
-        )
-    elif mode == "soda":
-        input_data = SodaInputData(
-            config,
-            system_file_paths,
-            check_existence=check_existence,
-            masterodb=kwargs["masterodb"],
-            perturbed_file_pattern=perturbed_file_pattern,
-            dtg=dtg,
-        )
-    elif mode == "perturbed":
-        perturbed = True
-        input_data = OfflineInputData(
-            config, system_file_paths, check_existence=check_existence
-        )
-    else:
-        raise NotImplementedError(mode + " is not implemented!")
-
     binary = kwargs["binary"]
     rte = kwargs["rte"]
     wrapper = kwargs["wrapper"]
     namelist_path = kwargs["namelist_path"]
     force = kwargs["force"]
     output = kwargs["output"]
     archive = kwargs["archive"]
     print_namelist = kwargs["print_namelist"]
     masterodb = kwargs["masterodb"]
     logging.debug("masterodb %s", masterodb)
     forc_zs = False
     if "forc_zs" in kwargs:
         forc_zs = kwargs["forc_zs"]
 
+    if mode == "pgd":
+        pgd = True
+        need_pgd = False
+        need_prep = False
+    elif mode == "prep":
+        prep = True
+        need_prep = False
+    elif mode == "offline":
+        pass
+    elif mode == "soda":
+        pass
+    elif mode == "perturbed":
+        perturbed = True
+    else:
+        raise NotImplementedError(mode + " is not implemented!")
+
     pgd_file_path = None
     if need_pgd:
         pgd_file_path = kwargs["pgd"]
 
     prep_file_path = None
     if need_prep:
         prep_file_path = kwargs["prep"]
@@ -521,14 +552,26 @@
     pert = None
     if "pert" in kwargs:
         pert = kwargs["pert"]
     negpert = False
     if "negpert" in kwargs:
         negpert = kwargs["negpert"]
 
+    try:
+        basetime = kwargs["basetime"]
+        if isinstance(basetime, str):
+            basetime = as_datetime(basetime)
+    except KeyError:
+        basetime = None
+
+    try:
+        input_binary_data = kwargs["input_binary_data"]
+    except KeyError:
+        input_binary_data = None
+
     if os.path.exists(rte):
         with open(rte, mode="r", encoding="utf-8") as file_handler:
             rte = json.load(file_handler)
         my_batch = BatchJob(rte, wrapper=wrapper)
     else:
         raise FileNotFoundError("File not found: " + rte)
 
@@ -536,53 +579,111 @@
     if archive is not None:
         if os.path.exists(archive):
             my_archive = JsonOutputDataFromFile(archive)
         else:
             raise FileNotFoundError("File not found: " + archive)
 
     if not os.path.exists(output) or force:
-        blocks = False
-        if blocks:
-            my_settings = Namelist(
-                mode,
-                config,
-                namelist_path,
-                forc_zs=forc_zs,
-                prep_file=prep_input_file,
-                prep_filetype=prep_input_filetype,
-                prep_pgdfile=prep_input_pgdfile,
-                prep_pgdfiletype=prep_input_pgdfiletype,
-                dtg=dtg,
-                fcint=3,
-            ).get_namelist()
+        if os.path.isfile(namelist_path):
+            with open(namelist_path, mode="r", encoding="utf-8") as file_handler:
+                nam_defs = yaml.safe_load(file_handler)
+            nam_gen = NamelistGenerator(mode, config, nam_defs)
+
+            my_settings = nam_gen.nml
+            if mode == "pgd":
+                my_settings = geo.update_namelist(my_settings)
+            if input_binary_data is None:
+                raise RuntimeError("input_binary_data not set")
+            with open(input_binary_data, mode="r", encoding="utf-8") as file_handler:
+                input_binary_data = json.load(file_handler)
+
+            input_data = nam_gen.input_data_from_namelist(
+                input_binary_data, system_file_paths, validtime=dtg, basetime=basetime
+            )
+        elif os.path.isdir(namelist_path):
+            if mode == "pgd":
+                pgd = True
+                need_pgd = False
+                need_prep = False
+                input_data = PgdInputData(
+                    config, system_file_paths, check_existence=check_existence
+                )
+            elif mode == "prep":
+                prep = True
+                need_prep = False
+                input_data = PrepInputData(
+                    config,
+                    system_file_paths,
+                    check_existence=check_existence,
+                    prep_file=prep_input_file,
+                    prep_pgdfile=prep_input_pgdfile,
+                )
+            elif mode == "offline":
+                input_data = OfflineInputData(
+                    config, system_file_paths, check_existence=check_existence
+                )
+            elif mode == "soda":
+                input_data = SodaInputData(
+                    config,
+                    system_file_paths,
+                    check_existence=check_existence,
+                    masterodb=kwargs["masterodb"],
+                    perturbed_file_pattern=perturbed_file_pattern,
+                    dtg=dtg,
+                )
+            elif mode == "perturbed":
+                perturbed = True
+                input_data = OfflineInputData(
+                    config, system_file_paths, check_existence=check_existence
+                )
+            else:
+                raise NotImplementedError(mode + " is not implemented!")
+
+            blocks = False
+            if blocks:
+                my_settings = Namelist(
+                    mode,
+                    config,
+                    namelist_path,
+                    forc_zs=forc_zs,
+                    prep_file=prep_input_file,
+                    prep_filetype=prep_input_filetype,
+                    prep_pgdfile=prep_input_pgdfile,
+                    prep_pgdfiletype=prep_input_pgdfiletype,
+                    dtg=dtg,
+                    fcint=3,
+                ).get_namelist()
+            else:
+                my_settings = BaseNamelist(
+                    mode,
+                    config,
+                    namelist_path,
+                    forc_zs=forc_zs,
+                    prep_file=prep_input_file,
+                    prep_filetype=prep_input_filetype,
+                    prep_pgdfile=prep_input_pgdfile,
+                    prep_pgdfiletype=prep_input_pgdfiletype,
+                    dtg=dtg,
+                    fcint=3,
+                ).get_namelist()
+            geo.update_namelist(my_settings)
         else:
-            my_settings = BaseNamelist(
-                mode,
-                config,
-                namelist_path,
-                forc_zs=forc_zs,
-                prep_file=prep_input_file,
-                prep_filetype=prep_input_filetype,
-                prep_pgdfile=prep_input_pgdfile,
-                prep_pgdfiletype=prep_input_pgdfiletype,
-                dtg=dtg,
-                fcint=3,
-            ).get_namelist()
-        geo.update_namelist(my_settings)
+            raise NotImplementedError
 
         # Create input
         my_format = my_settings["nam_io_offline"]["csurf_filetype"]
         my_pgdfile = my_settings["nam_io_offline"]["cpgdfile"]
         my_prepfile = my_settings["nam_io_offline"]["cprepfile"]
         my_surffile = my_settings["nam_io_offline"]["csurffile"]
         lfagmap = False
         if "lfagmap" in my_settings["nam_io_offline"]:
             lfagmap = my_settings["nam_io_offline"]["lfagmap"]
 
         logging.debug("pgdfile=%s lfagmap=%s %s", my_pgdfile, lfagmap, pgd_file_path)
+        logging.debug("nam_io_offline=%s", my_settings["nam_io_offline"])
         if need_pgd:
             logging.debug("Need pgd")
             my_pgdfile = PGDFile(
                 my_format,
                 my_pgdfile,
                 input_file=pgd_file_path,
                 lfagmap=lfagmap,
@@ -673,97 +774,14 @@
                 print_namelist=print_namelist,
             )
 
     else:
         logging.info("%s already exists!", output)
 
 
-def run_create_namelist(**kwargs):
-    """Create a namelist."""
-    logging.debug("ARGS: %s", kwargs)
-    config, geo = get_geo_and_config_from_cmd(**kwargs)
-    mode = kwargs.get("mode")
-
-    system_file_paths = kwargs["system_file_paths"]
-    if os.path.exists(system_file_paths):
-        system_file_paths = SystemFilePathsFromFile(system_file_paths)
-    else:
-        raise FileNotFoundError("File not found: " + system_file_paths)
-
-    if "forcing_dir" in kwargs:
-        system_file_paths.add_system_file_path("forcing_dir", kwargs["forcing_dir"])
-
-    prep_input_file = None
-    if "prep_file" in kwargs:
-        prep_input_file = kwargs["prep_file"]
-    prep_input_pgdfile = None
-    if "prep_pgdfile" in kwargs:
-        prep_input_pgdfile = kwargs["prep_pgdfile"]
-    prep_input_filetype = None
-    if "prep_filetype" in kwargs:
-        prep_input_filetype = kwargs["prep_filetype"]
-    prep_input_pgdfiletype = None
-    if "prep_pgdfiletype" in kwargs:
-        prep_input_pgdfiletype = kwargs["prep_pgdfiletype"]
-
-    # TODO
-    perturbed_file_pattern = None
-    if perturbed_file_pattern in kwargs:
-        perturbed_file_pattern = kwargs["perturbed_file_pattern"]
-
-    output = kwargs.get("output")
-    if output is None:
-        output = "OPTIONS.nam"
-    dtg = None
-    if "dtg" in kwargs:
-        if kwargs["dtg"] is not None and isinstance(kwargs["dtg"], str):
-            dtg = as_datetime(kwargs["dtg"])
-            kwargs.update({"dtg": dtg})
-
-    logging.debug("kwargs: %s", str(kwargs))
-
-    namelist_path = kwargs["namelist_path"]
-    forc_zs = False
-    if "forc_zs" in kwargs:
-        forc_zs = kwargs["forc_zs"]
-
-    if kwargs.get("method") == "blocks":
-        my_settings = Namelist(
-            mode,
-            config,
-            namelist_path,
-            forc_zs=forc_zs,
-            prep_file=prep_input_file,
-            geo=geo,
-            prep_filetype=prep_input_filetype,
-            prep_pgdfile=prep_input_pgdfile,
-            prep_pgdfiletype=prep_input_pgdfiletype,
-            dtg=dtg,
-            fcint=3,
-        ).get_namelist()
-    else:
-        my_settings = BaseNamelist(
-            mode,
-            config,
-            namelist_path,
-            forc_zs=forc_zs,
-            prep_file=prep_input_file,
-            prep_filetype=prep_input_filetype,
-            prep_pgdfile=prep_input_pgdfile,
-            prep_pgdfiletype=prep_input_pgdfiletype,
-            geo=geo,
-            dtg=dtg,
-            fcint=3,
-        ).get_namelist()
-    geo.update_namelist(my_settings)
-    if os.path.exists(output):
-        os.remove(output)
-    my_settings.write(output)
-
-
 def run_gridpp(**kwargs):
     """Gridpp."""
     var = kwargs["var"]
     input_file = kwargs["input_file"]
     output_file = None
     if "output_file" in kwargs:
         output_file = kwargs["output_file"]
@@ -1616,14 +1634,18 @@
 
 
 def create_namelist(argv=None):
     """Command line interface.
 
     Args:
         argv(list, optional): Arguments. Defaults to None.
+
+    Raises:
+        FileNotFoundError: "File not found:"
+
     """
     if argv is None:
         argv = sys.argv[1:]
     kwargs = parse_args_create_namelist(argv)
     debug = kwargs.get("debug")
     mode = kwargs.get("mode")
     if debug:
@@ -1632,15 +1654,42 @@
             level=logging.DEBUG,
         )
     else:
         logging.basicConfig(
             format="%(asctime)s %(levelname)s %(message)s", level=logging.INFO
         )
     logging.info("************ %s ******************", mode)
-    run_create_namelist(**kwargs)
+
+    logging.debug("ARGS: %s", kwargs)
+    config, __ = get_geo_and_config_from_cmd(**kwargs)
+    mode = kwargs.get("mode")
+
+    system_file_paths = kwargs["system_file_paths"]
+    if os.path.exists(system_file_paths):
+        system_file_paths = SystemFilePathsFromFile(system_file_paths)
+    else:
+        raise FileNotFoundError("File not found: " + system_file_paths)
+
+    output = kwargs.get("output")
+    if output is None:
+        output = "OPTIONS.nam"
+
+    namelist_path = kwargs.get("namelist_path")
+
+    with open(namelist_path, mode="r", encoding="utf-8") as file_handler:
+        nam_defs = yaml.safe_load(file_handler)
+
+    config.update_setting("SURFEX#PREP#FILE", None)
+    config.update_setting("SURFEX#PREP#FILEPGD", None)
+    config.update_setting("SURFEX#SODA#HH", "00")
+
+    my_settings = NamelistGenerator(mode, config, nam_defs)
+    if os.path.exists(output):
+        os.remove(output)
+    my_settings.write(output)
 
 
 def create_lsm_file_assim(argv=None):
     """Command line interface.
 
     Args:
         argv(list, optional): Arguments. Defaults to None.
```

### Comparing `pysurfex-0.0.3.4/pysurfex/cmd_parsing.py` & `pysurfex-0.0.4/pysurfex/cmd_parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -774,14 +774,17 @@
     )
     parser.add_argument(
         "--prep", type=str, nargs="?", required=True, help="Name of the PREP file"
     )
     parser.add_argument(
         "--force", "-f", action="store_true", default=False, help="Force re-creation"
     )
+    parser.add_argument(
+        "--input_binary_data", "-i", dest="input_binary_data", required=False
+    )
     parser.add_argument("--rte", "-r", required=True, nargs="?")
     parser.add_argument("--config", "-c", required=False, nargs="?")
     parser.add_argument(
         "--system_file_paths",
         "-s",
         required=True,
         nargs="?",
@@ -923,14 +926,17 @@
     )
     parser.add_argument(
         "--masterodb",
         action="store_true",
         default=False,
         help="Input file written by masterodb",
     )
+    parser.add_argument(
+        "--input_binary_data", "-i", dest="input_binary_data", required=False
+    )
     parser.add_argument("--rte", "-r", required=True, nargs="?")
     parser.add_argument("--config", "-c", required=False, nargs="?")
     parser.add_argument(
         "--system_file_paths",
         "-s",
         required=True,
         nargs="?",
@@ -980,27 +986,15 @@
 
     """
     parser = ArgumentParser(description="Create namelist")
     parser.add_argument("--version", action="version", version=__version__)
     parser.add_argument(
         "--debug", action="store_true", help="Debug", required=False, default=False
     )
-    parser.add_argument(
-        "--wrapper", "-w", type=str, default="", help="Execution wrapper command"
-    )
     parser.add_argument("mode", type=str, help="Type of namelist")
-    parser.add_argument("--method", required=False, default="blocks", nargs="?")
-    parser.add_argument("--prep_file", required=False, default=None, nargs="?")
-    parser.add_argument("--prep_filetype", required=False, default=None, nargs="?")
-    parser.add_argument("--prep_pgdfile", required=False, default=None, nargs="?")
-    parser.add_argument("--prep_pgdfiletype", required=False, default=None, nargs="?")
-    parser.add_argument(
-        "--forc_zs", action="store_true", default=False, help="Set model ZS to forcing ZS"
-    )
-    parser.add_argument("--forcing_dir", required=False, default=None, nargs="?")
     parser.add_argument(
         "--harmonie",
         action="store_true",
         default=False,
         help="Surfex configuration created from Harmonie environment",
     )
     parser.add_argument(
@@ -1012,15 +1006,14 @@
     )
     parser.add_argument("--config", "-c", required=False, nargs="?")
     parser.add_argument("--namelist_path", "-n", required=True, nargs="?")
     parser.add_argument(
         "--domain", type=str, required=False, help="JSON file with domain"
     )
     parser.add_argument("--output", "-o", type=str, required=False)
-    parser.add_argument("--dtg", type=str, required=False, default=None)
 
     if len(argv) == 0:
         parser.print_help()
         sys.exit(1)
 
     args = parser.parse_args(argv)
     kwargs = {}
```

### Comparing `pysurfex-0.0.3.4/pysurfex/configuration.py` & `pysurfex-0.0.4/pysurfex/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import logging
 import os
 
 import toml
 
 from .geo import ConfProj
-from .platform import SystemFilePaths
+from .platform_deps import SystemFilePaths
 from .util import merge_toml_env
 
 
 class Configuration(object):
     """Configuration class."""
 
     def __init__(self, conf):
@@ -788,19 +788,14 @@
             cvar_m = list(map(str, cvar_m.split(",")))
             self.update_setting("SURFEX#ASSIM#ISBA#ENKF#CVAR_M", cvar_m)
 
         if "NENS_M" in env:
             nens_m = env["NENS_M"]
             self.update_setting("SURFEX#ASSIM#ISBA#ENKF#NENS_M", int(nens_m))
 
-        # Observations
-        if "NOBSTYPE_M" in env:
-            nobstype_m = env["NOBSTYPE_M"]
-            self.update_setting("SURFEX#ASSIM#ISBA#OBS#NOBSTYPE_M", int(nobstype_m))
-
         # ANASURF_OI_COEFF Specify use of OI coefficients file (POLYNOMES_ISBA|POLYNOMES_ISBA_MF6)
         # # POLYNOMES_ISBA_MF6 means 6 times smaller coefficients for WG2 increments
         self.update_setting("SURFEX#ASSIM#ISBA#OI#COEFFS", env["ANASURF_OI_COEFF"])
 
         # Always set SURFEX#IO#LSPLIT_PATCH False
         self.update_setting("SURFEX#IO#LSPLIT_PATCH", False)
```

### Comparing `pysurfex-0.0.3.4/pysurfex/datetime_utils.py` & `pysurfex-0.0.4/pysurfex/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pysurfex/ecoclimap.py` & `pysurfex-0.0.4/pysurfex/ecoclimap.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,14 +67,20 @@
             mbr=mbr,
             tstep=tstep,
             pert=pert,
             var=var,
             system_variables=system_variables,
         )
 
+        basename = os.path.basename(fname)
+        parts = basename.split(".")
+        if len(parts) == 1:
+            logging.info("Assume format DIRTYP or DIRECT. fname=%s", fname)
+            fname = fname + ".dir"
+
         if fname.endswith(".dir"):
             basename = os.path.splitext(os.path.basename(fname))[0]
 
             basedir = self.system_file_paths.get_system_path(
                 dtype,
                 default_dir=default_dir,
                 check_existence=check_existence,
```

### Comparing `pysurfex-0.0.3.4/pysurfex/fa.py` & `pysurfex-0.0.4/pysurfex/fa.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pysurfex/file.py` & `pysurfex-0.0.4/pysurfex/file.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pysurfex/forcing.py` & `pysurfex-0.0.4/pysurfex/forcing.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pysurfex/geo.py` & `pysurfex-0.0.4/pysurfex/geo.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 try:
     from osgeo import ogr  # type: ignore
 except Exception:
     ogr = None
 
 
-from .namelist import BaseNamelist
+from .namelist_legacy import BaseNamelist
 
 
 class Geo(object):
     """Geometry."""
 
     def __init__(self, lons, lats):
         """Construct geometry.
@@ -279,58 +279,39 @@
 
         Args:
             nml (f90nml.Namelist): Namelist object.
 
         Returns:
             nml (f90nml.Namelist): Namelist object.
         """
-        if self.ilate is None or self.ilate is None:
-            nml.update(
-                {
-                    "nam_pgd_grid": {"cgrid": self.cgrid},
-                    "nam_conf_proj": {
-                        "xlon0": self.xlon0,
-                        "xlat0": self.xlat0,
-                        "xrpk": math.sin(math.radians(self.xlat0)),
-                        "xbeta": 0,
-                    },
-                    "nam_conf_proj_grid": {
-                        "xlatcen": self.xlatcen,
-                        "xloncen": self.xloncen,
-                        "nimax": self.nimax,
-                        "njmax": self.njmax,
-                        "xdx": self.xdx,
-                        "xdy": self.xdy,
-                        "xtrunc": self.xtrunc,
-                    },
-                }
-            )
-        else:
-            nml.update(
-                {
-                    "nam_pgd_grid": {"cgrid": self.cgrid},
-                    "nam_conf_proj": {
-                        "xlon0": self.xlon0,
-                        "xlat0": self.xlat0,
-                        "xrpk": math.sin(math.radians(self.xlat0)),
-                        "xbeta": 0,
-                    },
-                    "nam_conf_proj_grid": {
-                        "ilone": self.ilone,
-                        "ilate": self.ilate,
-                        "xlatcen": self.xlatcen,
-                        "xloncen": self.xloncen,
-                        "nimax": self.nimax,
-                        "njmax": self.njmax,
-                        "xdx": self.xdx,
-                        "xdy": self.xdy,
-                        "xtrunc": self.xtrunc,
-                    },
-                }
-            )
+        nml.update(
+            {
+                "nam_pgd_grid": {"cgrid": self.cgrid},
+                "nam_conf_proj": {
+                    "xlon0": self.xlon0,
+                    "xlat0": self.xlat0,
+                    "xrpk": math.sin(math.radians(self.xlat0)),
+                    "xbeta": 0,
+                },
+                "nam_conf_proj_grid": {
+                    "xlatcen": self.xlatcen,
+                    "xloncen": self.xloncen,
+                    "nimax": self.nimax,
+                    "njmax": self.njmax,
+                    "xdx": self.xdx,
+                    "xdy": self.xdy,
+                },
+            }
+        )
+        if self.ilone is not None:
+            nml["nam_conf_proj_grid"].update({"ilone": self.ilone})
+        if self.ilate is not None:
+            nml["nam_conf_proj_grid"].update({"ilate": self.ilate})
+        if self.xtrunc is not None:
+            nml["nam_conf_proj_grid"].update({"xtrunc": self.xtrunc})
         return nml
 
     def subset(self, geo):
         """Find subset of geo.
 
         Args:
             geo (surfex.Geo): Geometry to check.
```

### Comparing `pysurfex-0.0.3.4/pysurfex/grib.py` & `pysurfex-0.0.4/pysurfex/grib.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pysurfex/input_methods.py` & `pysurfex-0.0.4/pysurfex/input_methods.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pysurfex/interpolation.py` & `pysurfex-0.0.4/pysurfex/interpolation.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pysurfex/namelist.py` & `pysurfex-0.0.4/pysurfex/namelist_legacy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-"""Namelist."""
+"""Legacy namelist module."""
 import json
 import logging
 import os
+from warnings import warn
 
 import f90nml
 import yaml
 
 from .datetime_utils import as_datetime, as_timedelta
 from .ecoclimap import Ecoclimap, EcoclimapSG
 
@@ -43,14 +44,15 @@
             geo (surfex.Geo): Surfex geometry. The domain you want to run on
 
         Raises:
             RuntimeError: Needed input
             NotImplementedError: Mode not implemented
 
         """
+        warn("This is deprecated", DeprecationWarning, stacklevel=2)
         self.config = config
         self.input_path = input_path
         self.forc_zs = forc_zs
         if dtg is not None:
             if isinstance(dtg, str):
                 dtg = as_datetime(dtg)
         self.dtg = dtg
@@ -947,14 +949,22 @@
             ldname (_type_): _description_
             linput_path (_type_): _description_
 
         Returns:
             _type_: _description_
 
         """
+        logging.debug("ldname=%s ldtype=%s", ldname, ldtype)
+        basename = os.path.basename(ldname)
+        parts = basename.split(".")
+        logging.debug("parts=%s", parts)
+        if len(parts) == 1:
+            logging.info("Assume format DIRTYP or DIRECT. ldname=%s", ldname)
+            ldname = ldname + ".dir"
+
         if ldname.endswith(".dir"):
             basename = os.path.splitext(os.path.basename(ldname))[0]
             filetype_name = ldtype
             if ldtype == "YSOC_TOP" or ldtype == "YSOC_SUB":
                 filetype_name = "YSOC"
             return {
                 "json": json.loads(
@@ -1225,14 +1235,15 @@
 
         Raises:
             RuntimeError: Input
             RuntimeError: Merged dictionary contains a @ in value
             NotImplementedError: Mode is not implemented
 
         """
+        warn("This is deprecated", DeprecationWarning, stacklevel=2)
         self.config = config
         self.input_path = input_path
         self.forc_zs = forc_zs
         if dtg is not None:
             if isinstance(dtg, str):
                 dtg = as_datetime(dtg)
         self.dtg = dtg
```

### Comparing `pysurfex-0.0.3.4/pysurfex/netcdf.py` & `pysurfex-0.0.4/pysurfex/netcdf.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pysurfex/obs.py` & `pysurfex-0.0.4/pysurfex/obs.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pysurfex/observation.py` & `pysurfex-0.0.4/pysurfex/observation.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pysurfex/obsmon.py` & `pysurfex-0.0.4/pysurfex/obsmon.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pysurfex/obsoul.py` & `pysurfex-0.0.4/pysurfex/obsoul.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pysurfex/platform.py` & `pysurfex-0.0.4/pysurfex/platform_deps.py`

 * *Files 19% similar despite different names*

```diff
@@ -256,26 +256,28 @@
         check_parsing=False,
         validtime=None,
         basedtg=None,
         mbr=None,
         tstep=None,
         pert=None,
         var=None,
+        micro="@",
     ):
         """Parse setting with date/time/experiment specific values.
 
         Args:
             setting (str): The value of dictionary key which should be processes. Parser if type is str.
             check_parsing (bool): Check if all @@ pairs were parsed
             validtime (datetime.daetime): Parse setting with this as validtime
             basedtg (datetime.datetime): Parse setting with this as base time
             mbr (int): Parse setting with this as ensemble member number (@E@/@EE@/@EEE@)
             tstep (int): Parse setting with this as timestep to get step number (@TTT@/@TTTT@)
             pert (int): Parse setting with this as perturbation number @PERT@
             var (str): Parse setting with this as the variable (@VAR@)
+            micro (str, optional): Micro character. Defaults to "@"
 
         Raises:
             RuntimeError: Setting was not substituted properly?
 
         Returns:
             setting: Possibly parsed setting is type is str
 
@@ -294,88 +296,137 @@
                 if isinstance(validtime, str):
                     validtime = as_datetime(validtime)
             else:
                 validtime = basedtg
 
             if basedtg is not None and validtime is not None:
                 lead_time = validtime - basedtg
-                setting = str(setting).replace("@YYYY_LL@", validtime.strftime("%Y"))
-                setting = str(setting).replace("@MM_LL@", validtime.strftime("%m"))
-                setting = str(setting).replace("@DD_LL@", validtime.strftime("%d"))
-                setting = str(setting).replace("@HH_LL@", validtime.strftime("%H"))
-                setting = str(setting).replace("@mm_LL@", validtime.strftime("%M"))
+                setting = str(setting).replace(
+                    f"{micro}YYYY_LL{micro}", validtime.strftime("%Y")
+                )
+                setting = str(setting).replace(
+                    f"{micro}MM_LL{micro}", validtime.strftime("%m")
+                )
+                setting = str(setting).replace(
+                    f"{micro}DD_LL{micro}", validtime.strftime("%d")
+                )
+                setting = str(setting).replace(
+                    f"{micro}HH_LL{micro}", validtime.strftime("%H")
+                )
+                setting = str(setting).replace(
+                    f"{micro}mm_LL{micro}", validtime.strftime("%M")
+                )
+                setting = str(setting).replace(
+                    f"{micro}FG_YYYY{micro}", basedtg.strftime("%Y")
+                )
+                setting = str(setting).replace(
+                    f"{micro}FG_YY{micro}", basedtg.strftime("%y")
+                )
+                setting = str(setting).replace(
+                    f"{micro}FG_MM{micro}", basedtg.strftime("%m")
+                )
+                setting = str(setting).replace(
+                    f"{micro}FG_DD{micro}", basedtg.strftime("%d")
+                )
+                setting = str(setting).replace(
+                    f"{micro}FG_HH{micro}", basedtg.strftime("%H")
+                )
+                setting = str(setting).replace(
+                    f"{micro}FG_mm{micro}", basedtg.strftime("%M")
+                )
                 lead_seconds = int(lead_time.total_seconds())
                 lead_hours = int(lead_seconds / 3600)
-                setting = str(setting).replace("@LL@", f"{lead_hours:02d}")
-                setting = str(setting).replace("@LLL@", f"{lead_hours:03d}")
-                setting = str(setting).replace("@LLLL@", f"{lead_hours:04d}")
+                setting = str(setting).replace(f"{micro}LL{micro}", f"{lead_hours:02d}")
+                setting = str(setting).replace(f"{micro}LLL{micro}", f"{lead_hours:03d}")
+                setting = str(setting).replace(f"{micro}LLLL{micro}", f"{lead_hours:04d}")
                 if tstep is not None:
                     lead_step = int(lead_seconds / tstep)
-                    setting = str(setting).replace("@TTT@", f"{lead_step:03d}")
-                    setting = str(setting).replace("@TTTT@", f"{lead_step:04d}")
+                    setting = str(setting).replace(
+                        f"{micro}TTT{micro}", f"{lead_step:03d}"
+                    )
+                    setting = str(setting).replace(
+                        f"{micro}TTTT{micro}", f"{lead_step:04d}"
+                    )
 
             if basedtg is not None:
-                setting = str(setting).replace("@YMD@", basedtg.strftime("%Y%m%d"))
-                setting = str(setting).replace("@YYYY@", basedtg.strftime("%Y"))
-                setting = str(setting).replace("@YY@", basedtg.strftime("%y"))
-                setting = str(setting).replace("@MM@", basedtg.strftime("%m"))
-                setting = str(setting).replace("@DD@", basedtg.strftime("%d"))
-                setting = str(setting).replace("@HH@", basedtg.strftime("%H"))
-                setting = str(setting).replace("@mm@", basedtg.strftime("%M"))
+                setting = str(setting).replace(
+                    f"{micro}YMD{micro}", basedtg.strftime("%Y%m%d")
+                )
+                setting = str(setting).replace(
+                    f"{micro}YYYY{micro}", basedtg.strftime("%Y")
+                )
+                setting = str(setting).replace(
+                    f"{micro}YY{micro}", basedtg.strftime("%y")
+                )
+                setting = str(setting).replace(
+                    f"{micro}MM{micro}", basedtg.strftime("%m")
+                )
+                setting = str(setting).replace(
+                    f"{micro}DD{micro}", basedtg.strftime("%d")
+                )
+                setting = str(setting).replace(
+                    f"{micro}HH{micro}", basedtg.strftime("%H")
+                )
+                setting = str(setting).replace(
+                    f"{micro}mm{micro}", basedtg.strftime("%M")
+                )
 
             if mbr is not None:
-                setting = str(setting).replace("@E@", f"mbr{int(mbr):d}")
-                setting = str(setting).replace("@EE@", f"mbr{int(mbr):02d}")
-                setting = str(setting).replace("@EEE@", f"mbr{int(mbr):03d}")
+                setting = str(setting).replace(f"{micro}E{micro}", f"mbr{int(mbr):d}")
+                setting = str(setting).replace(f"{micro}EE{micro}", f"mbr{int(mbr):02d}")
+                setting = str(setting).replace(f"{micro}EEE{micro}", f"mbr{int(mbr):03d}")
             else:
-                setting = str(setting).replace("@E@", "")
-                setting = str(setting).replace("@EE@", "")
-                setting = str(setting).replace("@EEE@", "")
+                setting = str(setting).replace(f"{micro}E{micro}", "")
+                setting = str(setting).replace(f"{micro}EE{micro}", "")
+                setting = str(setting).replace(f"{micro}EEE{micro}", "")
 
             if pert is not None:
                 logging.debug("replace %s in %s", pert, setting)
-                setting = str(setting).replace("@PERT@", str(pert))
+                setting = str(setting).replace(f"{micro}PERT{micro}", str(pert))
                 logging.debug("replaced %s in %s", pert, setting)
 
             if var is not None:
-                setting = str(setting).replace("@VAR@", var)
+                setting = str(setting).replace(f"{micro}VAR{micro}", var)
 
         if check_parsing:
-            if isinstance(setting, str) and setting.count("@") > 1:
+            if isinstance(setting, str) and setting.count(f"{micro}") > 1:
                 raise RuntimeError("Setting was not substituted properly? " + setting)
 
         return setting
 
     @staticmethod
-    def substitute_string(setting, system_variables=None):
+    def substitute_string(setting, system_variables=None, micro="@"):
         """Substitute setting if string with OS values of values from system_variables.
 
         Args:
             setting (str): if setting is string it can be subst
             system_variables (dict): Arbitrary settings to substitute @NAME@ =
                                      system_variables={"NAME": "Value"}
+            micro (str, optional): Micro character. Default to "@"
 
         Returns:
             setting: A setting possibly substituted if type is str
 
         """
         if isinstance(setting, str):
             env_vals = ["USER", "HOME", "PWD"]
             for env_val in env_vals:
                 if env_val in os.environ:
-                    setting = setting.replace("@" + env_val + "@", os.environ[env_val])
+                    setting = setting.replace(
+                        f"{micro}" + env_val + f"{micro}", os.environ[env_val]
+                    )
                 else:
                     logging.debug("%s not found in environment", env_val)
 
             if system_variables is not None:
                 logging.debug(system_variables)
                 for var in system_variables:
                     logging.debug(var, system_variables)
                     setting = setting.replace(
-                        "@" + str(var) + "@", str(system_variables[var])
+                        f"{micro}" + str(var) + f"{micro}", str(system_variables[var])
                     )
 
         return setting
 
     def add_system_file_path(
         self,
         name,
```

### Comparing `pysurfex-0.0.3.4/pysurfex/read.py` & `pysurfex-0.0.4/pysurfex/read.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pysurfex/run.py` & `pysurfex-0.0.4/pysurfex/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
             batch (_type_): _description_
             io (_type_): _description_
             pert_number (_type_): _description_
             settings (_type_): _description_
             input_data (_type_): _description_
             surfout (_type_, optional): _description_. Defaults to None.
             archive_data (_type_, optional): _description_. Defaults to None.
-            pgdfile (_type_, optional): _description_. Defaults to None.
+            pgdfile (str, optional): _description_. Defaults to None.
             print_namelist (bool, optional): _description_. Defaults to False.
             negpert (bool, optional): _description_. Defaults to False.
 
         """
         self.pert_number = pert_number
         settings["nam_io_varassim"]["LPRT"] = True
         settings["nam_var"]["nivar"] = int(pert_number)
```

### Comparing `pysurfex-0.0.3.4/pysurfex/settings/assimilation.json` & `pysurfex-0.0.4/pysurfex/settings/assimilation.json`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pysurfex/settings/forecast.json` & `pysurfex-0.0.4/pysurfex/settings/forecast.json`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pysurfex/settings/pgd.json` & `pysurfex-0.0.4/pysurfex/settings/pgd.json`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pysurfex/settings/prep.json` & `pysurfex-0.0.4/pysurfex/settings/prep.json`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pysurfex/timeseries.py` & `pysurfex-0.0.4/pysurfex/timeseries.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pysurfex/titan.py` & `pysurfex-0.0.4/pysurfex/titan.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pysurfex/util.py` & `pysurfex-0.0.4/pysurfex/util.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/pysurfex/variable.py` & `pysurfex-0.0.4/pysurfex/variable.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.4/PKG-INFO` & `pysurfex-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysurfex
-Version: 0.0.3.4
+Version: 0.0.4
 Summary: Python API to SURFEX
 Home-page: https://github.com/metno/pysurfex
 License: MIT
 Author: Trygve Aspelien
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

