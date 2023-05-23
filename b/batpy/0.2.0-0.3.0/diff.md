# Comparing `tmp/batpy-0.2.0.tar.gz` & `tmp/batpy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batpy-0.2.0.tar", max compression
+gzip compressed data, was "batpy-0.3.0.tar", max compression
```

## Comparing `batpy-0.2.0.tar` & `batpy-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,34 @@
--rwxr-xr-x   0        0        0     1073 2023-05-20 15:23:23.687684 batpy-0.2.0/LICENSE
--rw-r--r--   0        0        0     5818 2023-05-20 15:23:23.687684 batpy-0.2.0/README.md
--rw-r--r--   0        0        0     1922 2023-05-20 15:23:59.608070 batpy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      236 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/__init__.py
--rw-r--r--   0        0        0     5658 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/batpac_battery.py
--rw-r--r--   0        0        0    30838 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/batpac_tool.py
--rw-r--r--   0        0        0    12208 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/brightway.py
--rw-r--r--   0        0        0   209566 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.0.0/batpy_batpac_battery_design.toml
--rw-r--r--   0        0        0     2158 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.0.0/batpy_batpac_calculation_and_validation_results.toml
--rw-r--r--   0        0        0    30666 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.0.0/batpy_batpac_config.toml
--rw-r--r--   0        0        0    57647 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.0.0/batpy_batpac_summary_of_results.toml
--rw-r--r--   0        0        0    83193 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.0.0/batpy_batpac_user_input_cells.toml
--rw-r--r--   0        0        0    48449 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.0.0/batpy_batteries_config.toml
--rw-r--r--   0        0        0     2232 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.1.0/batpy_batpac2brightway.toml
--rw-r--r--   0        0        0   209566 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.1.0/batpy_batpac_battery_design.toml
--rw-r--r--   0        0        0     2158 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.1.0/batpy_batpac_calculation_and_validation_results.toml
--rw-r--r--   0        0        0    30666 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.1.0/batpy_batpac_config.toml
--rw-r--r--   0        0        0    57647 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.1.0/batpy_batpac_summary_of_results.toml
--rw-r--r--   0        0        0    83193 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.1.0/batpy_batpac_user_input_cells.toml
--rw-r--r--   0        0        0    48449 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/0.1.0/batpy_batteries_config.toml
--rw-r--r--   0        0        0      145 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/data/__init__.py
--rw-r--r--   0        0        0     3979 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/datasets.py
--rw-r--r--   0        0        0    10048 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/formula_engine.py
--rw-r--r--   0        0        0     3799 2023-05-20 15:23:23.695684 batpy-0.2.0/src/batpy/utility_functions.py
--rw-r--r--   0        0        0     6724 1970-01-01 00:00:00.000000 batpy-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1073 2023-05-23 04:45:53.698635 batpy-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2671 2023-05-23 04:45:53.698635 batpy-0.3.0/README.md
+-rw-r--r--   0        0        0     1922 2023-05-23 04:46:36.295195 batpy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      236 2023-05-23 04:45:53.698635 batpy-0.3.0/src/batpy/__init__.py
+-rw-r--r--   0        0        0     5658 2023-05-23 04:45:53.698635 batpy-0.3.0/src/batpy/batpac_battery.py
+-rw-r--r--   0        0        0    22987 2023-05-23 04:45:53.698635 batpy-0.3.0/src/batpy/batpac_tool.py
+-rw-r--r--   0        0        0     6536 2023-05-23 04:45:53.698635 batpy-0.3.0/src/batpy/batpy_workbook.py
+-rw-r--r--   0        0        0     6234 2023-05-23 04:45:53.698635 batpy-0.3.0/src/batpy/brightway.py
+-rw-r--r--   0        0        0   282104 2023-05-23 04:45:53.702635 batpy-0.3.0/src/batpy/data/0.0.0/batpy_batpac_battery_design.toml
+-rw-r--r--   0        0        0     3129 2023-05-23 04:45:53.702635 batpy-0.3.0/src/batpy/data/0.0.0/batpy_batpac_calculation_and_validation_results.toml
+-rw-r--r--   0        0        0    46126 2023-05-23 04:45:53.702635 batpy-0.3.0/src/batpy/data/0.0.0/batpy_batpac_config.toml
+-rw-r--r--   0        0        0    67362 2023-05-23 04:45:53.702635 batpy-0.3.0/src/batpy/data/0.0.0/batpy_batpac_summary_of_results.toml
+-rw-r--r--   0        0        0   123865 2023-05-23 04:45:53.702635 batpy-0.3.0/src/batpy/data/0.0.0/batpy_batpac_user_input_cells.toml
+-rw-r--r--   0        0        0    70611 2023-05-23 04:45:53.702635 batpy-0.3.0/src/batpy/data/0.0.0/batpy_batteries_config.toml
+-rw-r--r--   0        0        0     2232 2023-05-23 04:45:53.702635 batpy-0.3.0/src/batpy/data/0.1.0/batpy_batpac2brightway.toml
+-rw-r--r--   0        0        0   209566 2023-05-23 04:45:53.702635 batpy-0.3.0/src/batpy/data/0.1.0/batpy_batpac_battery_design.toml
+-rw-r--r--   0        0        0     2158 2023-05-23 04:45:53.702635 batpy-0.3.0/src/batpy/data/0.1.0/batpy_batpac_calculation_and_validation_results.toml
+-rw-r--r--   0        0        0    30666 2023-05-23 04:45:53.702635 batpy-0.3.0/src/batpy/data/0.1.0/batpy_batpac_config.toml
+-rw-r--r--   0        0        0    57647 2023-05-23 04:45:53.702635 batpy-0.3.0/src/batpy/data/0.1.0/batpy_batpac_summary_of_results.toml
+-rw-r--r--   0        0        0    83193 2023-05-23 04:45:53.702635 batpy-0.3.0/src/batpy/data/0.1.0/batpy_batpac_user_input_cells.toml
+-rw-r--r--   0        0        0    48449 2023-05-23 04:45:53.702635 batpy-0.3.0/src/batpy/data/0.1.0/batpy_batteries_config.toml
+-rw-r--r--   0        0        0     2495 2023-05-23 04:45:53.702635 batpy-0.3.0/src/batpy/data/0.3.0/batpy_batpac2brightway.toml
+-rw-r--r--   0        0        0   282102 2023-05-23 04:45:53.706635 batpy-0.3.0/src/batpy/data/0.3.0/batpy_batpac_battery_design.toml
+-rw-r--r--   0        0        0     3127 2023-05-23 04:45:53.706635 batpy-0.3.0/src/batpy/data/0.3.0/batpy_batpac_calculation_and_validation_results.toml
+-rw-r--r--   0        0        0    46124 2023-05-23 04:45:53.706635 batpy-0.3.0/src/batpy/data/0.3.0/batpy_batpac_config.toml
+-rw-r--r--   0        0        0    67360 2023-05-23 04:45:53.706635 batpy-0.3.0/src/batpy/data/0.3.0/batpy_batpac_summary_of_results.toml
+-rw-r--r--   0        0        0   123863 2023-05-23 04:45:53.706635 batpy-0.3.0/src/batpy/data/0.3.0/batpy_batpac_user_input_cells.toml
+-rw-r--r--   0        0        0    70609 2023-05-23 04:45:53.706635 batpy-0.3.0/src/batpy/data/0.3.0/batpy_batteries_config.toml
+-rw-r--r--   0        0        0      145 2023-05-23 04:45:53.706635 batpy-0.3.0/src/batpy/data/__init__.py
+-rw-r--r--   0        0        0   259536 2023-05-23 04:45:53.706635 batpy-0.3.0/src/batpy/data/excel_workbooks/BatPaC-Brightway.xlsx
+-rw-r--r--   0        0        0     7696 2023-05-23 04:45:53.706635 batpy-0.3.0/src/batpy/datasets.py
+-rw-r--r--   0        0        0    10048 2023-05-23 04:45:53.706635 batpy-0.3.0/src/batpy/formula_engine.py
+-rw-r--r--   0        0        0     3799 2023-05-23 04:45:53.706635 batpy-0.3.0/src/batpy/utility_functions.py
+-rw-r--r--   0        0        0     3577 1970-01-01 00:00:00.000000 batpy-0.3.0/PKG-INFO
```

### Comparing `batpy-0.2.0/LICENSE` & `batpy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `batpy-0.2.0/pyproject.toml` & `batpy-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "batpy"
-version = "0.2.0"
+version = "0.3.0"
 description = "A python package to read, write, and calculate batteries in the BatPaC tool."
 authors = ["Raphael Ginster <r.ginster@tu-braunschweig.de>"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://rginster.github.io/batpy/"
 repository = "https://github.com/rginster/batpy"
```

### Comparing `batpy-0.2.0/src/batpy/batpac_battery.py` & `batpy-0.3.0/src/batpy/batpac_battery.py`

 * *Files identical despite different names*

### Comparing `batpy-0.2.0/src/batpy/batpac_tool.py` & `batpy-0.3.0/src/batpy/batpac_tool.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,36 @@
 # -*- coding: UTF-8 -*-
 """Module, which includes the class BatpacTool
 """
 import logging
 from pathlib import Path
 
-import semantic_version
-import toml
-import xlwings as xw
 from prettytable import PrettyTable
 from tqdm import tqdm
 
-import batpy
 from batpy.batpac_battery import BatpacBattery
-from batpy.utility_functions import is_version_compatible, load_configuration
+from batpy.batpy_workbook import BatpyWorkbook
 
 
-class BatpacTool:
+class BatpacTool(BatpyWorkbook):
     """BatPaC class which interacts with the BatPaC Excel tool
 
     This BatPaC class is used to interact directly with the BatPaC Excel tool
     and can store individual batteries (class BatPaC_battery) and additional
     parameters of the BatPaC Excel tool in the dictionary properties.
     """
 
-    def _load_user_file(self, path_to_user_file: Path | str) -> dict:
-        """Load user file configuration
-
-        Load the user configuration from a TOML user file.
-
-        Parameters
-        ----------
-        path_to_user_file : Path | str
-            Path to the TOML user file or configuration as string.
-
-        Returns
-        -------
-        dict
-            Returns dictionary representation of read TOML file.
-        """
-        config = load_configuration(path_to_user_file)
-        config_metadata = config.pop("batpy")
-        self.is_version_compatible(
-            semantic_version.Version(config_metadata["BatPaC SemVer"])
-        )
-        return config
-
     def __init__(
         self,
         batpac_workbook_path: Path,
         cell_definition_user_input_toml_path: Path | str,
         cell_definition_calculation_validation_results: Path | str = None,
         # cell_definition_additional_user_input_toml_path: Path = None,
         # cell_definition_additional_user_results_toml_path: Path = None,
-        excel_visible: bool = False,
+        workbook_visible: bool = False,
     ) -> None:
         """Initialize BatPaC
 
         Initialize the BatPaC object.
 
         Parameters
         ----------
@@ -74,119 +48,47 @@
             Path to the TOML file, which contains additional cells for user
             input, that are not included in the standard user inputs in the
             BatPaC Excel tool, by default None.
         cell_definition_additional_user_results_toml_path : Path, optional
             Path to the TOML file, which contains additional cells for  user
             input, that are not included in the standard user inputs in the
             BatPaC Excel tool, by default None.
-        excel_visible : bool, optional
-            True, if Excel should be visible during operation, by default
+        workbook_visible : bool, optional
+            True, if workbook should be visible during operation, by default
             False.
         """
-        logging.info(
-            "[ ] Create BatPaC from %s and load cell references from %s",
-            batpac_workbook_path,
-            cell_definition_user_input_toml_path,
-        )
-        self.version = semantic_version.Version(batpy.__version__)
 
-        self.excel_cells = self._load_user_file(
+        super().__init__(batpac_workbook_path, workbook_visible)
+
+        self.excel_cells = self._load_user_configuration(
             cell_definition_user_input_toml_path
         )
         if cell_definition_calculation_validation_results:
-            self.toml_calculation_validation_results = self._load_user_file(
-                cell_definition_calculation_validation_results
+            self.toml_calculation_validation_results = (
+                self._load_user_configuration(
+                    cell_definition_calculation_validation_results
+                )
             )
         self.batteries = []
-        self.workbook = xw.Book(batpac_workbook_path)
-        # self.app = self.workbook.app
-        self.workbook.app.visible = excel_visible
         self.max_batteries = 7
-        self.properties = {}
-        logging.info(
-            "[+] Created BatPaC from %s and load \
-                    cell references from %s",
-            batpac_workbook_path,
-            cell_definition_user_input_toml_path,
-        )
-
-    def __del__(self) -> None:
-        """Destructor of BatPac object
-
-        Set the Excel calculation method to "automatic" and the
-        "screen_updating" to True after object destruction.
-        """
-        try:
-            self.workbook.app.calculation = "automatic"
-            self.workbook.app.screen_updating = True
-        except BaseException as error:
-            logging.error("An exception occurred: %s", error)
-            raise KeyError(
-                "Could not access the workbook (may already be closed)."
-            ) from error
-
-    def is_version_compatible(
-        self,
-        version_to_check: semantic_version.Version,
-        include_minor: bool = False,
-    ) -> bool:
-        """Check for version compatibility
-
-        Check if two versions (major.minor.patch) are compatible. Thereby a
-        version is compatible if major is equal. If minor should also be
-        included a version is compatible if major is equal and minor is greater
-        or equal.
-
-        Parameters
-        ----------
-        version_to_check : semantic_version.Version
-            Version to be checked against self.version.
-        include_minor : bool, optional
-            Check if minor version of version_to_check is greater or equal to
-            self.version's minor, by default False.
-
-        Returns
-        -------
-        bool
-            True, if version is compatible.
-
-        Raises
-        ------
-        ValueError
-            If version is not compatible a ValueError will occur.
-        """
-        return is_version_compatible(
-            self.version, version_to_check, include_minor
-        )
 
     def load_batpac_file(self, path_to_batpac_file: Path | str) -> None:
         """Load BatPaC configuration
 
         Load the properties for the BatPaC object from a TOML battery
         configuration file.
 
         Parameters
         ----------
         path_to_batpac_file : Path | str
             Path to the TOML BatPaC configuration file.
         """
-        logging.info("[ ] Load BatPaC file from %s", path_to_batpac_file)
-
-        try:
-            Path.exists(Path(path_to_batpac_file))
-            config = toml.load(path_to_batpac_file)
-        except (AttributeError, OSError):
-            config = toml.loads(path_to_batpac_file)
-        config_metadata = config.pop("batpy")
-        if self.is_version_compatible(
-            semantic_version.Version(config_metadata["BatPaC SemVer"])
-        ):
-            self.properties = config
-            logging.info("[+] Loaded BatPaC file from %s", path_to_batpac_file)
-            logging.debug("[ ] BatPaC properties %s", self.properties)
+        self.properties = self._load_user_configuration(path_to_batpac_file)
+        logging.info("[+] Loaded BatPaC file from %s", path_to_batpac_file)
+        logging.debug("[ ] BatPaC properties %s", self.properties)
 
     def add_battery(self, batteries: list[BatpacBattery]) -> None:
         """Add battery object to BatPaC object
 
         Add multiple battery objects to the BatPaC object.
 
         Parameters
@@ -257,63 +159,14 @@
                 battery.name,
                 battery.properties,
             )
         logging.info(
             "[+] Batteries from file %s loaded", path_to_batteries_file
         )
 
-    def _write_value_direct(
-        self, worksheet: str, cell_range: str, value: any
-    ) -> None:
-        """Write value in BatPaC Excel tool
-
-        Write a value directly in the BatPaC Excel tool.
-
-        Parameters
-        ----------
-        worksheet : str
-            Name of the BatPaC Excel tool worksheet.
-        cell_range : str
-            Cell range of the BatPaC Excel tool.
-        value : any
-            Value to write in the BatPaC Excel tool.
-        """
-        self.workbook.sheets[worksheet][cell_range].value = value
-
-    def _read_value_direct(self, worksheet: str, cell_range: str) -> any:
-        """Read value from BatPaC Excel tool
-
-        Read a value directly from the BatPaC Excel tool.
-
-        Parameters
-        ----------
-        worksheet : str
-            Name of the BatPaC Excel tool worksheet.
-        cell_range : str
-            Cell range of the BatPaC Excel tool.
-
-        Returns
-        -------
-        any
-            Value of the BatPaC Excel tool cell.
-
-        Raises
-        ------
-        KeyError
-            Raises KeyError if the specified worksheet or range could not be
-            found.
-        """
-        try:
-            value = self.workbook.sheets[worksheet][cell_range].value
-            return value
-        except BaseException as error:
-            logging.error("An exception occurred: %s", error)
-            logging.warning("[!] Key %s , %s not found", worksheet, cell_range)
-            raise KeyError from error
-
     def _wb_helper_range(
         self,
         worksheet: str,
         name: str,
         battery: BatpacBattery = None,
         additional_cell_config: Path | dict | str = None,
     ) -> str:
@@ -347,15 +200,17 @@
             found.
         """
         try:
             if additional_cell_config is not None:
                 if isinstance(additional_cell_config, dict):
                     range_dict = additional_cell_config
                 else:
-                    range_dict = self._load_user_file(additional_cell_config)
+                    range_dict = self._load_user_configuration(
+                        additional_cell_config
+                    )
             else:
                 range_dict = self.excel_cells
 
             if battery is None:
                 cell_range = range_dict[worksheet][name]
             else:
                 cell_range = range_dict[worksheet][
@@ -363,97 +218,36 @@
                 ][name]
             return cell_range
         except BaseException as error:
             logging.error("An exception occurred: %s", error)
             logging.warning("[!] Key %s , %s not found", worksheet, name)
             raise KeyError from error
 
-    def write_value(self, worksheet: str, name: str, value: any) -> None:
-        """Write value in BatPaC Excel tool
-
-        Write value in BatPaC Excel tool without input the exact cell range.
-
-        Parameters
-        ----------
-        worksheet : str
-            Name of the BatPaC Excel tool worksheet.
-        name : str
-            Name of the BatPaC Excel cell description.
-        value : any
-            Value to write in the BatPaC Excel tool.
-        """
-        self._write_value_direct(
-            worksheet, self._wb_helper_range(worksheet, name), value
-        )
-        logging.debug(
-            "[ ] Write in %s %s (%s) = %s",
-            worksheet,
-            self._wb_helper_range(worksheet, name),
-            name,
-            value,
-        )
-
     def read_value(
         self,
         worksheet: str,
         name: str,
+        battery: BatpacBattery = None,
         additional_cell_config: Path | dict | str = None,
     ) -> any:
         """Read value from BatPaC Excel tool
 
-        Read value from BatPaC Excel tool without input the exact cell range.
-
-        Parameters
-        ----------
-        worksheet : str
-            Name of the BatPaC Excel tool worksheet.
-        name : str
-            Name of the BatPaC Excel cell description.
-        additional_cell_config : Path | dict | str, optional
-            Path to TOML file or dictionary or string (default dataset), which
-            contains additional cell configuration to consider,
-            by default None.
-
-        Returns
-        -------
-        any
-            Value of the BatPaC Excel tool cell.
-        """
-        return self._read_value_direct(
-            worksheet,
-            self._wb_helper_range(
-                worksheet,
-                name,
-                battery=None,
-                additional_cell_config=additional_cell_config,
-            ),
-        )
-
-    def read_value_battery(
-        self,
-        worksheet: str,
-        name: str,
-        battery: BatpacBattery,
-        additional_cell_config: Path | dict | str = None,
-    ) -> any:
-        """Read battery specific value from BatPaC Excel tool
-
-        Read battery specific value from BatPaC Excel tool without input the
+        Read (battery specific) value from BatPaC Excel tool without input the
         exact cell range.
 
         Parameters
         ----------
         worksheet : str
             Name of the BatPaC Excel tool worksheet.
         name : str
             Name of the BatPaC Excel cell description.
-        battery : BatPaC_battery
+        battery : BatPaC_battery, optional
             BatPaC_battery object, if the returned cell is battery specific, by
             default None.
-        additional_cell_config : Path | dict, optional
+        additional_cell_config : Path | dict | str, optional
             Path to TOML file or dictionary or string (default dataset), which
             contains additional cell configuration to consider,
             by default None.
 
         Returns
         -------
         any
@@ -462,62 +256,64 @@
         return self._read_value_direct(
             worksheet,
             self._wb_helper_range(
                 worksheet, name, battery, additional_cell_config
             ),
         )
 
-    def write_value_battery(
-        self, worksheet: str, name: str, battery: BatpacBattery, value: any
+    def write_value(
+        self,
+        worksheet: str,
+        name: str,
+        value: any,
+        battery: BatpacBattery = None,
     ) -> None:
-        """Write specific battery value in BatPaC Excel tool
+        """Write value in BatPaC Excel tool
 
-        Write a speicif battery value in the BatPaC Excel tool without input
+        Write (specific battery) value in the BatPaC Excel tool without input
         the exact cell range.
 
         Parameters
         ----------
         worksheet : str
             Name of the BatPaC Excel tool worksheet.
         name : str
             Name of the BatPaC Excel cell description.
-        battery : BatPaC_battery
-            BatPaC_battery object, if the returned cell is battery specific,
-            by default None.
         value : any
             Value to write in the BatPaC Excel tool.
+        battery : BatPaC_battery, optional
+            BatPaC_battery object, if the returned cell is battery specific,
+            by default None.
         """
         self._write_value_direct(
             worksheet, self._wb_helper_range(worksheet, name, battery), value
         )
         logging.debug(
             "[ ] Write for %s in %s %s (%s) = %s",
-            battery.name,
+            battery.name if battery else "BatPaC tool",
             worksheet,
             self._wb_helper_range(worksheet, name, battery),
             name,
             value,
         )
 
     def stop_automatic_calculation(self) -> None:
         """Stop automatic Excel calculation
         Stop the automatic Excel and BatPaC calculation.
         """
         self.write_value("Dashboard", "Restart (0/1)", 0)
-        self.workbook.app.calculation = "manual"
-        self.workbook.app.screen_updating = False
+        super().stop_automatic_calculation()
 
     def start_automatic_calculation(self) -> None:
         """Start automatic Excel calculation
         Start the automatic Excel and BatPaC calculation.
         """
         reset_macro = self.workbook.macro("Module1.Reset")
         reset_macro()
-        self.workbook.app.calculation = "automatic"
-        self.workbook.app.screen_updating = True
+        super().start_automatic_calculation()
 
     def read_from_user_input(self, user_read_file: Path | str) -> dict:
         """Read user specified input from BatPaC Excel tool
 
         Read additional cell values from BatPaC Excel tool specified by user
         input.
 
@@ -529,15 +325,15 @@
 
         Returns
         -------
         dict
             Dictionary in the format {"sheet" : {"name" : value} }
         """
 
-        additional_cells = self._load_user_file(user_read_file)
+        additional_cells = self._load_user_configuration(user_read_file)
         values_dict = additional_cells
         for sheet_name, sheet_key in additional_cells.items():
             for batpac_key, batpac_cell_range in sheet_key.items():
                 if isinstance(batpac_cell_range, dict):
                     for (
                         battery_key,
                         battery_cell_range,
@@ -584,68 +380,70 @@
                 logging.warning(
                     "[!] No toml file for calculation and validation found."
                 )
                 raise KeyError(
                     "No configuration for calculation and validation found."
                 )
         else:
-            self.toml_calculation_validation_results = self._load_user_file(
-                toml_file_calculation_validation_results
+            self.toml_calculation_validation_results = (
+                self._load_user_configuration(
+                    toml_file_calculation_validation_results
+                )
             )
 
         config_errors = ["Configuration Errors (see table to right)"]
         config_warnings = ["Configuration Warnings (see table  to right)"]
         plant_size = ["Plant Size, GWh"]
         power_to_energy = ["Power-to-energy ratio"]
         adequacy_cooling = ["Adequacy of cooling"]
         cathode_thickness = ["Cathode thickness limited by"]
         table_columns = ["Parameter"]
         for battery in self.batteries:
             config_errors.append(
-                self.read_value_battery(
+                self.read_value(
                     "Dashboard",
                     "Configuration Errors (see table to right)",
                     battery,
                     self.toml_calculation_validation_results,
                 )
             )
             config_warnings.append(
-                self.read_value_battery(
+                self.read_value(
                     "Dashboard",
                     "Configuration Warnings (see table  to right)",
                     battery,
                     self.toml_calculation_validation_results,
                 )
             )
             plant_size.append(
-                self.read_value_battery(
+                self.read_value(
                     "Dashboard",
                     "Plant Size, GWh",
                     battery,
                     self.toml_calculation_validation_results,
                 )
             )
             power_to_energy.append(
-                self.read_value_battery(
+                self.read_value(
                     "Dashboard",
                     "Power-to-energy ratio",
                     battery,
                     self.toml_calculation_validation_results,
                 )
             )
             adequacy_cooling.append(
-                self.read_value_battery(
+                self.read_value(
                     "Dashboard",
                     "Adequacy of cooling",
                     battery,
                     self.toml_calculation_validation_results,
                 )
             )
             cathode_thickness.append(
-                self.read_value_battery(
+                self.read_value(
                     "Dashboard",
                     "Cathode thickness limited by",
                     battery,
                     self.toml_calculation_validation_results,
                 )
             )
             table_columns.append(battery.name)
@@ -708,57 +506,19 @@
             for i, battery in enumerate(self.batteries):
                 if sheet in battery.properties:
                     for key, value in battery.properties[sheet].items():
                         if key not in sheet_buffer:
                             sheet_buffer[key] = [None] * self.max_batteries
                         sheet_buffer[key][i] = value
             for key, value in sheet_buffer.items():
-                self.write_value_battery(sheet, key, self.batteries[0], value)
+                self.write_value(sheet, key, value, self.batteries[0])
 
         self.start_automatic_calculation()
         logging.info("[+] Finished calculation")
 
-    def save(self, path: Path = None) -> None:
-        """Save BatPaC Excel tool
-
-        Save the BatPaC Excel tool or save the BatPaC Excel tool in another
-        path.
-
-        Parameters
-        ----------
-        path : Path, optional
-            If the path is specified, the BatPaC Excel tool will be saved under
-            the path, by default None will overwrite the current BatPaC Excel
-            tool.
-        """
-        logging.info("[ ] Save workbook")
-        self.workbook.save(path)
-        self.workbook = xw.Book(path)
-        # self.app = self.workbook.app
-        logging.info("[+] Saved workbook in %s", path)
-
-    def close(self) -> bool:
-        """Close BatPaC Excel tool
-
-        Close the BatPaC Excel tool if other workbooks are open, otherwise the
-        Excel instance will be closed.
-
-        Returns
-        -------
-        bool
-            True, if BatPaC Excel tool is closed.
-        """
-        if len(self.workbook.app.books) == 1:
-            self.workbook.app.quit()
-            logging.info("[+] Workbook and Excel closed")
-            return True
-        self.workbook.close()
-        logging.info("[+] Workbook closed")
-        return True
-
     def _save_batpac_config(self, batpac_path: Path = None) -> None:
         """Save BatPaC_tool configuration
 
         Read all BatPaC_tool properties from the BatPaC Excel tool, save
         these properties in the BatPaC_tool object, and write them as TOML
         file.
```

### Comparing `batpy-0.2.0/src/batpy/data/0.0.0/batpy_batpac_battery_design.toml` & `batpy-0.3.0/src/batpy/data/0.1.0/batpy_batpac_battery_design.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ["batpy"]
 "BatPaC version" = "BatPaC 5.0 2022-07-22"
-"BatPaC SemVer" = "0.0.0"
+"BatPaC SemVer" = "0.1.0"
 
 ["Battery Design"."Battery 1"]
 # Battery System Parameters
 # Key inputs and general pack structure used in the calculations
 'Battery System Parameters, Number of packs per vehicle (parallel or series)' = 'G12'
 'Battery System Parameters, Parallel (P) or series (S) packs' = 'G13'
 'Battery System Parameters, Total target battery system acceleration power, kW' = 'G14'
```

### Comparing `batpy-0.2.0/src/batpy/data/0.0.0/batpy_batpac_calculation_and_validation_results.toml` & `batpy-0.3.0/src/batpy/data/0.1.0/batpy_batpac_calculation_and_validation_results.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ["batpy"]
 "BatPaC version" = "BatPaC 5.0 2022-07-22"
-"BatPaC SemVer" = "0.0.0"
+"BatPaC SemVer" = "0.1.0"
 
 ["Dashboard"."Battery 1"]
 ## Calculation and Validation
 "Configuration Errors (see table to right)" = "D129"
 "Configuration Warnings (see table  to right)" = "D130"
 "Plant Size, GWh" = "D131"
 "Power-to-energy ratio" = "D132"
```

### Comparing `batpy-0.2.0/src/batpy/data/0.0.0/batpy_batpac_config.toml` & `batpy-0.3.0/src/batpy/data/0.1.0/batpy_batpac_config.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ["batpy"]
 "BatPaC version" = "BatPaC 5.0 2022-07-22"
-"BatPaC SemVer" = "0.0.0"
+"BatPaC SemVer" = "0.1.0"
 
 ["Dashboard"]
 'Electrode Couple' = 'NMC811-G (Energy)'
 'Positive active material specific capacity, mAh/g' = 200.0
 'Void volume fraction, % of positive electrode' = 20.0
 'Positive foil thickness, mm' = 10.0
 'Maximum positive electrode thickness, µm' = 110.0
```

### Comparing `batpy-0.2.0/src/batpy/data/0.0.0/batpy_batpac_summary_of_results.toml` & `batpy-0.3.0/src/batpy/data/0.1.0/batpy_batpac_summary_of_results.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ["batpy"]
 "BatPaC version" = "BatPaC 5.0 2022-07-22"
-"BatPaC SemVer" = "0.0.0"
+"BatPaC SemVer" = "0.1.0"
 
 ["Summary of Results"."Battery 1"]
 # Calculated Parameters
 "Battery System Parameters, Battery System Configuration and Performance, Number of battery packs" = "G17"
 "Battery System Parameters, Battery System Configuration and Performance, Packs in series or parallel" = "G18"
 "Battery System Parameters, Battery System Configuration and Performance, Battery system average OCV, V" = "G19"
 "Battery System Parameters, Battery System Configuration and Performance, Battery system nominal operating voltage, V" = "G20"
```

### Comparing `batpy-0.2.0/src/batpy/data/0.0.0/batpy_batpac_user_input_cells.toml` & `batpy-0.3.0/src/batpy/data/0.1.0/batpy_batpac_user_input_cells.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ["batpy"]
 "BatPaC version" = "BatPaC 5.0 2022-07-22"
-"BatPaC SemVer" = "0.0.0"
+"BatPaC SemVer" = "0.1.0"
 
 ["Dashboard"]
 "Restart (0/1)" = "D6"
 # Chemistry
 ## Positive Electrode
 "Electrode Couple" = "E13"
 "Positive active material specific capacity, mAh/g" = "E15"
```

### Comparing `batpy-0.2.0/src/batpy/data/0.0.0/batpy_batteries_config.toml` & `batpy-0.3.0/src/batpy/data/0.1.0/batpy_batteries_config.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ["batpy"]
 "BatPaC version" = "BatPaC 5.0 2022-07-22"
-"BatPaC SemVer" = "0.0.0"
+"BatPaC SemVer" = "0.1.0"
 
 ["Battery 1"."Dashboard"]
 'Number of modules in parallel' = 10000.0
 'Target rated peak power of pack, kW' = 100.0
 'Duration at rated power, s' = 10.0
 'Override duration at rated peak power, s' = 2.0
 'Operating initial SOC for rated peak power, %' = 20.0
```

### Comparing `batpy-0.2.0/src/batpy/data/0.1.0/batpy_batpac2brightway.toml` & `batpy-0.3.0/src/batpy/data/0.1.0/batpy_batpac2brightway.toml`

 * *Files identical despite different names*

### Comparing `batpy-0.2.0/src/batpy/data/0.1.0/batpy_batpac_calculation_and_validation_results.toml` & `batpy-0.3.0/src/batpy/data/0.0.0/batpy_batpac_calculation_and_validation_results.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,67 @@
 ["batpy"]
-"BatPaC version" = "BatPaC 5.0 2022-07-22"
-"BatPaC SemVer" = "0.1.0"
+    "BatPaC version" = "BatPaC 5.0 2022-07-22"
+    "BatPaC SemVer"  = "0.0.0"
+    "information"    = "Configuration for calculation and validation results in BatPaC Excel"
 
 ["Dashboard"."Battery 1"]
-## Calculation and Validation
-"Configuration Errors (see table to right)" = "D129"
-"Configuration Warnings (see table  to right)" = "D130"
-"Plant Size, GWh" = "D131"
-"Power-to-energy ratio" = "D132"
-"Adequacy of cooling" = "D133"
-"Cathode thickness limited by" = "D134"
+    ## Calculation and Validation
+    "Configuration Errors (see table to right)"    = "D129"
+    "Configuration Warnings (see table  to right)" = "D130"
+    "Plant Size, GWh"                              = "D131"
+    "Power-to-energy ratio"                        = "D132"
+    "Adequacy of cooling"                          = "D133"
+    "Cathode thickness limited by"                 = "D134"
 
 ["Dashboard"."Battery 2"]
-## Calculation and Validation
-"Configuration Errors (see table to right)" = "E129"
-"Configuration Warnings (see table  to right)" = "E130"
-"Plant Size, GWh" = "E131"
-"Power-to-energy ratio" = "E132"
-"Adequacy of cooling" = "E133"
-"Cathode thickness limited by" = "E134"
+    ## Calculation and Validation
+    "Configuration Errors (see table to right)"    = "E129"
+    "Configuration Warnings (see table  to right)" = "E130"
+    "Plant Size, GWh"                              = "E131"
+    "Power-to-energy ratio"                        = "E132"
+    "Adequacy of cooling"                          = "E133"
+    "Cathode thickness limited by"                 = "E134"
 
 ["Dashboard"."Battery 3"]
-## Calculation and Validation
-"Configuration Errors (see table to right)" = "F129"
-"Configuration Warnings (see table  to right)" = "F130"
-"Plant Size, GWh" = "F131"
-"Power-to-energy ratio" = "F132"
-"Adequacy of cooling" = "F133"
-"Cathode thickness limited by" = "F134"
+    ## Calculation and Validation
+    "Configuration Errors (see table to right)"    = "F129"
+    "Configuration Warnings (see table  to right)" = "F130"
+    "Plant Size, GWh"                              = "F131"
+    "Power-to-energy ratio"                        = "F132"
+    "Adequacy of cooling"                          = "F133"
+    "Cathode thickness limited by"                 = "F134"
 
 ["Dashboard"."Battery 4"]
-## Calculation and Validation
-"Configuration Errors (see table to right)" = "G129"
-"Configuration Warnings (see table  to right)" = "G130"
-"Plant Size, GWh" = "G131"
-"Power-to-energy ratio" = "G132"
-"Adequacy of cooling" = "G133"
-"Cathode thickness limited by" = "G134"
+    ## Calculation and Validation
+    "Configuration Errors (see table to right)"    = "G129"
+    "Configuration Warnings (see table  to right)" = "G130"
+    "Plant Size, GWh"                              = "G131"
+    "Power-to-energy ratio"                        = "G132"
+    "Adequacy of cooling"                          = "G133"
+    "Cathode thickness limited by"                 = "G134"
 
 ["Dashboard"."Battery 5"]
-## Calculation and Validation
-"Configuration Errors (see table to right)" = "H129"
-"Configuration Warnings (see table  to right)" = "H130"
-"Plant Size, GWh" = "H131"
-"Power-to-energy ratio" = "H132"
-"Adequacy of cooling" = "H133"
-"Cathode thickness limited by" = "H134"
+    ## Calculation and Validation
+    "Configuration Errors (see table to right)"    = "H129"
+    "Configuration Warnings (see table  to right)" = "H130"
+    "Plant Size, GWh"                              = "H131"
+    "Power-to-energy ratio"                        = "H132"
+    "Adequacy of cooling"                          = "H133"
+    "Cathode thickness limited by"                 = "H134"
 
 ["Dashboard"."Battery 6"]
-## Calculation and Validation
-"Configuration Errors (see table to right)" = "I129"
-"Configuration Warnings (see table  to right)" = "I130"
-"Plant Size, GWh" = "I131"
-"Power-to-energy ratio" = "I132"
-"Adequacy of cooling" = "I133"
-"Cathode thickness limited by" = "I134"
+    ## Calculation and Validation
+    "Configuration Errors (see table to right)"    = "I129"
+    "Configuration Warnings (see table  to right)" = "I130"
+    "Plant Size, GWh"                              = "I131"
+    "Power-to-energy ratio"                        = "I132"
+    "Adequacy of cooling"                          = "I133"
+    "Cathode thickness limited by"                 = "I134"
 
 ["Dashboard"."Battery 7"]
-## Calculation and Validation
-"Configuration Errors (see table to right)" = "J129"
-"Configuration Warnings (see table  to right)" = "J130"
-"Plant Size, GWh" = "J131"
-"Power-to-energy ratio" = "J132"
-"Adequacy of cooling" = "J133"
-"Cathode thickness limited by" = "J134"
+    ## Calculation and Validation
+    "Configuration Errors (see table to right)"    = "J129"
+    "Configuration Warnings (see table  to right)" = "J130"
+    "Plant Size, GWh"                              = "J131"
+    "Power-to-energy ratio"                        = "J132"
+    "Adequacy of cooling"                          = "J133"
+    "Cathode thickness limited by"                 = "J134"
```

### Comparing `batpy-0.2.0/src/batpy/data/0.1.0/batpy_batpac_summary_of_results.toml` & `batpy-0.3.0/src/batpy/data/0.0.0/batpy_batpac_summary_of_results.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,885 +1,886 @@
 ["batpy"]
-"BatPaC version" = "BatPaC 5.0 2022-07-22"
-"BatPaC SemVer" = "0.1.0"
+    "BatPaC version" = "BatPaC 5.0 2022-07-22"
+    "BatPaC SemVer"  = "0.0.0"
+    "information"    = "Configuration for worksheet Summary of Results in BatPaC Excel"
 
 ["Summary of Results"."Battery 1"]
-# Calculated Parameters
-"Battery System Parameters, Battery System Configuration and Performance, Number of battery packs" = "G17"
-"Battery System Parameters, Battery System Configuration and Performance, Packs in series or parallel" = "G18"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system average OCV, V" = "G19"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system nominal operating voltage, V" = "G20"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system capacity, Ah" = "G21"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system total energy, kWh" = "G22"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system useable energy, kWh(Useable)" = "G23"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system power at target % OCV, kW" = "G24"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system rated power, kW" = "G25"
-"Battery System Parameters, Battery System Configuration and Performance, Target SOC at full power, %" = "G26"
-"Battery System Parameters, Battery System Configuration and Performance, Pulse time at rated power, s" = "G27"
-"Battery System Parameters, Battery System Configuration and Performance, % OCV at rated power (adjusted for thickness limit), %" = "G28"
-"Battery System Parameters, Battery System Configuration and Performance, Cooling system power requirement, W" = "G29"
-
-"Battery System Parameters, Battery System Size, Battery system volume (all packs and cooling), L" = "G32"
-"Battery System Parameters, Battery System Size, Battery system mass (all packs and cooling), kg" = "G33"
-
-"Battery System Parameters, Battery System Metrics, Battery system energy density, Wh/L" = "G36"
-"Battery System Parameters, Battery System Metrics, Battery system specific energy, Wh/kg" = "G37"
-"Battery System Parameters, Battery System Metrics, Battery system useable energy density, Wh(Useable)/L" = "G38"
-"Battery System Parameters, Battery System Metrics, Battery system useable specific energy, Wh(Useable)/kg" = "G39"
-
-"Pack Parameters, Pack Configuration and Performance, Number of cells per pack" = "G43"
-"Pack Parameters, Pack Configuration and Performance, Number of modules per pack" = "G44"
-"Pack Parameters, Pack Configuration and Performance, Pack average OCV, V" = "G45"
-"Pack Parameters, Pack Configuration and Performance, Pack nominal operating voltage, V" = "G46"
-"Pack Parameters, Pack Configuration and Performance, Pack capacity, Ah" = "G47"
-"Pack Parameters, Pack Configuration and Performance, Pack total energy, kWh" = "G48"
-"Pack Parameters, Pack Configuration and Performance, Pack useable energy, kWh(Useable)" = "G49"
-"Pack Parameters, Pack Configuration and Performance, Pack power at target %OCV, kW" = "G50"
-"Pack Parameters, Pack Configuration and Performance, Pack power at rated power, kW" = "G51"
-
-"Pack Parameters, Pack Size, Pack length, mm" = "G54"
-"Pack Parameters, Pack Size, Pack width, mm" = "G55"
-"Pack Parameters, Pack Size, Pack height, mm" = "G56"
-"Pack Parameters, Pack Size, Pack volume, L" = "G57"
-"Pack Parameters, Pack Size, Pack total mass, kg" = "G58"
-
-"Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to power at target %OCV)" = "G61"
-"Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to rated power)" = "G62"
-"Pack Parameters, Pack Metrics, Pack energy density, Wh/L" = "G63"
-"Pack Parameters, Pack Metrics, Pack specific energy, Wh/kg" = "G64"
-"Pack Parameters, Pack Metrics, Pack useable energy density, Wh(Useable)/L" = "G65"
-"Pack Parameters, Pack Metrics, Pack useable specific energy, Wh(Useable)/kg" = "G66"
-
-"Module Parameters, Module Configuration and Performance, Number of cells per module" = "G70"
-"Module Parameters, Module Configuration and Performance, Module average OCV, V" = "G71"
-"Module Parameters, Module Configuration and Performance, Module nominal operating voltage, V" = "G72"
-"Module Parameters, Module Configuration and Performance, Module capacity, Ah" = "G73"
-"Module Parameters, Module Configuration and Performance, Module total energy, kWh" = "G74"
-"Module Parameters, Module Configuration and Performance, Module useable energy, kWh(Useable)" = "G75"
-"Module Parameters, Module Configuration and Performance, Module power at target %OCV, kW" = "G76"
-"Module Parameters, Module Configuration and Performance, Module power at rated power, kW" = "G77"
-
-"Module Parameters, Module Size, Module length, mm" = "G80"
-"Module Parameters, Module Size, Module width, mm" = "G81"
-"Module Parameters, Module Size, Module height, mm" = "G82"
-"Module Parameters, Module Size, Module volume, L" = "G83"
-"Module Parameters, Module Size, Module volume per pack, L" = "G84"
-"Module Parameters, Module Size, Module mass, kg" = "G85"
-"Module Parameters, Module Size, Module mass per pack, kg" = "G86"
-
-"Module Parameters, Module Metrics, Module energy density, Wh/L" = "G89"
-"Module Parameters, Module Metrics, Module specific energy, Wh/kg" = "G90"
-"Module Parameters, Module Metrics, Module useable energy density, Wh(Useable)/L" = "G91"
-"Module Parameters, Module Metrics, Module useable specific energy, Wh(Useable)/kg" = "G92"
-
-"Cell Parameters, Cell Performance, Cell average OCV, V" = "G96"
-"Cell Parameters, Cell Performance, Cell nominal operating voltage, V" = "G97"
-"Cell Parameters, Cell Performance, Cell capacity, Ah" = "G98"
-"Cell Parameters, Cell Performance, Cell total energy, kWh" = "G99"
-"Cell Parameters, Cell Performance, Cell useable energy, kWh(Useable)" = "G100"
-"Cell Parameters, Cell Performance, Cell power at target %OCV, kW" = "G101"
-"Cell Parameters, Cell Performance, Cell power at rated power, kW" = "G102"
-
-"Cell Parameters, Cell Size,Cell length, mm" = "G105"
-"Cell Parameters, Cell Size,Cell width, mm" = "G106"
-"Cell Parameters, Cell Size,Cell thickness, mm" = "G107"
-"Cell Parameters, Cell Size,Cell volume, L" = "G108"
-"Cell Parameters, Cell Size,Cell volume per pack, L" = "G109"
-"Cell Parameters, Cell Size,Cell mass, kg" = "G110"
-"Cell Parameters, Cell Size,Cell mass per pack, kg" = "G111"
-
-"Cell Parameters, Cell Metrics, Cell energy density, Wh/L" = "G114"
-"Cell Parameters, Cell Metrics, Cell specific energy, Wh/kg" = "G115"
-"Cell Parameters, Cell Metrics, Cell useable energy density, Wh(Useable)/L" = "G116"
-"Cell Parameters, Cell Metrics, Cell useable specific energy, Wh(Useable)/kg" = "G117"
-
-"Cell Parameters, Additional Cell Information, Positive electrode thickness, µm" = "G120"
-"Cell Parameters, Additional Cell Information, Negative electrode thickness, µm" = "G121"
-"Cell Parameters, Additional Cell Information, Positive electode areal capacity, mAh/cm²" = "G122"
-"Cell Parameters, Additional Cell Information, Negative electrode areal capacity, mAh/cm²" = "G123"
-
-# Manufacturing Information
-"Plant Size, GWh" = "G128"
-"Packs manufactured at 100% utilization (pack/year)" = "G129"
-"Packs manufactured per year (packs/year)" = "G130"
-"Modules manufactured per year (modules/year)" = "G131"
-"Accepted cells manufactured per year (cells/year)" = "G132"
-
-# Calculated Costs
-"Costs, Battery System, Battery system cost, $" = "G149"
-"Costs, Battery System, Battery system cost, $/kWh" = "G150"
-"Costs, Battery System, Battery system cost, $/kWh(Useable)" = "G151"
-
-"Costs, Pack, Pack cost, $/pack" = "G154"
-"Costs, Pack, Pack cost, $/kWh" = "G155"
-"Costs, Pack, Pack cost, $/kWh(Useable)" = "G156"
-
-"Costs, Module, Module cost, $/module" = "G159"
-"Costs, Module, Module cost per pack, $/pack" = "G160"
-"Costs, Module, Module cost, $/kWh" = "G161"
-"Costs, Module, Module cost, $/kWh(Useable)" = "G162"
-
-"Costs, Cell, Cell cost, $/cell" = "G165"
-"Costs, Cell, Cell cost, $/module" = "G166"
-"Costs, Cell, Cell cost, $/pack" = "G167"
-"Costs, Cell, Cell cost, $/kWh" = "G168"
-"Costs, Cell, Cell cost, $/kWh(Useable)" = "G169"
-
-"Costs, Additional Considerations, Module fraction of pack cost" = "G172"
-"Costs, Additional Considerations, Cell fraction of module cost" = "G173"
-"Costs, Additional Considerations, Cell fraction of pack cost" = "G174"
+    # Calculated Parameters
+    "Battery System Parameters, Battery System Configuration and Performance, Number of battery packs"                                = "G17"
+    "Battery System Parameters, Battery System Configuration and Performance, Packs in series or parallel"                            = "G18"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system average OCV, V"                          = "G19"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system nominal operating voltage, V"            = "G20"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system capacity, Ah"                            = "G21"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system total energy, kWh"                       = "G22"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system useable energy, kWh(Useable)"            = "G23"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system power at target % OCV, kW"               = "G24"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system rated power, kW"                         = "G25"
+    "Battery System Parameters, Battery System Configuration and Performance, Target SOC at full power, %"                            = "G26"
+    "Battery System Parameters, Battery System Configuration and Performance, Pulse time at rated power, s"                           = "G27"
+    "Battery System Parameters, Battery System Configuration and Performance, % OCV at rated power (adjusted for thickness limit), %" = "G28"
+    "Battery System Parameters, Battery System Configuration and Performance, Cooling system power requirement, W"                    = "G29"
+
+    "Battery System Parameters, Battery System Size, Battery system volume (all packs and cooling), L" = "G32"
+    "Battery System Parameters, Battery System Size, Battery system mass (all packs and cooling), kg"  = "G33"
+
+    "Battery System Parameters, Battery System Metrics, Battery system energy density, Wh/L"                    = "G36"
+    "Battery System Parameters, Battery System Metrics, Battery system specific energy, Wh/kg"                  = "G37"
+    "Battery System Parameters, Battery System Metrics, Battery system useable energy density, Wh(Useable)/L"   = "G38"
+    "Battery System Parameters, Battery System Metrics, Battery system useable specific energy, Wh(Useable)/kg" = "G39"
+
+    "Pack Parameters, Pack Configuration and Performance, Number of cells per pack"          = "G43"
+    "Pack Parameters, Pack Configuration and Performance, Number of modules per pack"        = "G44"
+    "Pack Parameters, Pack Configuration and Performance, Pack average OCV, V"               = "G45"
+    "Pack Parameters, Pack Configuration and Performance, Pack nominal operating voltage, V" = "G46"
+    "Pack Parameters, Pack Configuration and Performance, Pack capacity, Ah"                 = "G47"
+    "Pack Parameters, Pack Configuration and Performance, Pack total energy, kWh"            = "G48"
+    "Pack Parameters, Pack Configuration and Performance, Pack useable energy, kWh(Useable)" = "G49"
+    "Pack Parameters, Pack Configuration and Performance, Pack power at target %OCV, kW"     = "G50"
+    "Pack Parameters, Pack Configuration and Performance, Pack power at rated power, kW"     = "G51"
+
+    "Pack Parameters, Pack Size, Pack length, mm"     = "G54"
+    "Pack Parameters, Pack Size, Pack width, mm"      = "G55"
+    "Pack Parameters, Pack Size, Pack height, mm"     = "G56"
+    "Pack Parameters, Pack Size, Pack volume, L"      = "G57"
+    "Pack Parameters, Pack Size, Pack total mass, kg" = "G58"
+
+    "Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to power at target %OCV)" = "G61"
+    "Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to rated power)"          = "G62"
+    "Pack Parameters, Pack Metrics, Pack energy density, Wh/L"                                         = "G63"
+    "Pack Parameters, Pack Metrics, Pack specific energy, Wh/kg"                                       = "G64"
+    "Pack Parameters, Pack Metrics, Pack useable energy density, Wh(Useable)/L"                        = "G65"
+    "Pack Parameters, Pack Metrics, Pack useable specific energy, Wh(Useable)/kg"                      = "G66"
+
+    "Module Parameters, Module Configuration and Performance, Number of cells per module"          = "G70"
+    "Module Parameters, Module Configuration and Performance, Module average OCV, V"               = "G71"
+    "Module Parameters, Module Configuration and Performance, Module nominal operating voltage, V" = "G72"
+    "Module Parameters, Module Configuration and Performance, Module capacity, Ah"                 = "G73"
+    "Module Parameters, Module Configuration and Performance, Module total energy, kWh"            = "G74"
+    "Module Parameters, Module Configuration and Performance, Module useable energy, kWh(Useable)" = "G75"
+    "Module Parameters, Module Configuration and Performance, Module power at target %OCV, kW"     = "G76"
+    "Module Parameters, Module Configuration and Performance, Module power at rated power, kW"     = "G77"
+
+    "Module Parameters, Module Size, Module length, mm"         = "G80"
+    "Module Parameters, Module Size, Module width, mm"          = "G81"
+    "Module Parameters, Module Size, Module height, mm"         = "G82"
+    "Module Parameters, Module Size, Module volume, L"          = "G83"
+    "Module Parameters, Module Size, Module volume per pack, L" = "G84"
+    "Module Parameters, Module Size, Module mass, kg"           = "G85"
+    "Module Parameters, Module Size, Module mass per pack, kg"  = "G86"
+
+    "Module Parameters, Module Metrics, Module energy density, Wh/L"                    = "G89"
+    "Module Parameters, Module Metrics, Module specific energy, Wh/kg"                  = "G90"
+    "Module Parameters, Module Metrics, Module useable energy density, Wh(Useable)/L"   = "G91"
+    "Module Parameters, Module Metrics, Module useable specific energy, Wh(Useable)/kg" = "G92"
+
+    "Cell Parameters, Cell Performance, Cell average OCV, V"               = "G96"
+    "Cell Parameters, Cell Performance, Cell nominal operating voltage, V" = "G97"
+    "Cell Parameters, Cell Performance, Cell capacity, Ah"                 = "G98"
+    "Cell Parameters, Cell Performance, Cell total energy, kWh"            = "G99"
+    "Cell Parameters, Cell Performance, Cell useable energy, kWh(Useable)" = "G100"
+    "Cell Parameters, Cell Performance, Cell power at target %OCV, kW"     = "G101"
+    "Cell Parameters, Cell Performance, Cell power at rated power, kW"     = "G102"
+
+    "Cell Parameters, Cell Size,Cell length, mm"         = "G105"
+    "Cell Parameters, Cell Size,Cell width, mm"          = "G106"
+    "Cell Parameters, Cell Size,Cell thickness, mm"      = "G107"
+    "Cell Parameters, Cell Size,Cell volume, L"          = "G108"
+    "Cell Parameters, Cell Size,Cell volume per pack, L" = "G109"
+    "Cell Parameters, Cell Size,Cell mass, kg"           = "G110"
+    "Cell Parameters, Cell Size,Cell mass per pack, kg"  = "G111"
+
+    "Cell Parameters, Cell Metrics, Cell energy density, Wh/L"                    = "G114"
+    "Cell Parameters, Cell Metrics, Cell specific energy, Wh/kg"                  = "G115"
+    "Cell Parameters, Cell Metrics, Cell useable energy density, Wh(Useable)/L"   = "G116"
+    "Cell Parameters, Cell Metrics, Cell useable specific energy, Wh(Useable)/kg" = "G117"
+
+    "Cell Parameters, Additional Cell Information, Positive electrode thickness, µm"           = "G120"
+    "Cell Parameters, Additional Cell Information, Negative electrode thickness, µm"           = "G121"
+    "Cell Parameters, Additional Cell Information, Positive electode areal capacity, mAh/cm²"  = "G122"
+    "Cell Parameters, Additional Cell Information, Negative electrode areal capacity, mAh/cm²" = "G123"
+
+    # Manufacturing Information
+    "Plant Size, GWh"                                    = "G128"
+    "Packs manufactured at 100% utilization (pack/year)" = "G129"
+    "Packs manufactured per year (packs/year)"           = "G130"
+    "Modules manufactured per year (modules/year)"       = "G131"
+    "Accepted cells manufactured per year (cells/year)"  = "G132"
+
+    # Calculated Costs
+    "Costs, Battery System, Battery system cost, $"              = "G149"
+    "Costs, Battery System, Battery system cost, $/kWh"          = "G150"
+    "Costs, Battery System, Battery system cost, $/kWh(Useable)" = "G151"
+
+    "Costs, Pack, Pack cost, $/pack"         = "G154"
+    "Costs, Pack, Pack cost, $/kWh"          = "G155"
+    "Costs, Pack, Pack cost, $/kWh(Useable)" = "G156"
+
+    "Costs, Module, Module cost, $/module"        = "G159"
+    "Costs, Module, Module cost per pack, $/pack" = "G160"
+    "Costs, Module, Module cost, $/kWh"           = "G161"
+    "Costs, Module, Module cost, $/kWh(Useable)"  = "G162"
+
+    "Costs, Cell, Cell cost, $/cell"         = "G165"
+    "Costs, Cell, Cell cost, $/module"       = "G166"
+    "Costs, Cell, Cell cost, $/pack"         = "G167"
+    "Costs, Cell, Cell cost, $/kWh"          = "G168"
+    "Costs, Cell, Cell cost, $/kWh(Useable)" = "G169"
+
+    "Costs, Additional Considerations, Module fraction of pack cost" = "G172"
+    "Costs, Additional Considerations, Cell fraction of module cost" = "G173"
+    "Costs, Additional Considerations, Cell fraction of pack cost"   = "G174"
 
 ["Summary of Results"."Battery 2"]
-# Calculated Parameters
-"Battery System Parameters, Battery System Configuration and Performance, Number of battery packs" = "H17"
-"Battery System Parameters, Battery System Configuration and Performance, Packs in series or parallel" = "H18"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system average OCV, V" = "H19"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system nominal operating voltage, V" = "H20"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system capacity, Ah" = "H21"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system total energy, kWh" = "H22"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system useable energy, kWh(Useable)" = "H23"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system power at target % OCV, kW" = "H24"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system rated power, kW" = "H25"
-"Battery System Parameters, Battery System Configuration and Performance, Target SOC at full power, %" = "H26"
-"Battery System Parameters, Battery System Configuration and Performance, Pulse time at rated power, s" = "H27"
-"Battery System Parameters, Battery System Configuration and Performance, % OCV at rated power (adjusted for thickness limit), %" = "H28"
-"Battery System Parameters, Battery System Configuration and Performance, Cooling system power requirement, W" = "H29"
-
-"Battery System Parameters, Battery System Size, Battery system volume (all packs and cooling), L" = "H32"
-"Battery System Parameters, Battery System Size, Battery system mass (all packs and cooling), kg" = "H33"
-
-"Battery System Parameters, Battery System Metrics, Battery system energy density, Wh/L" = "H36"
-"Battery System Parameters, Battery System Metrics, Battery system specific energy, Wh/kg" = "H37"
-"Battery System Parameters, Battery System Metrics, Battery system useable energy density, Wh(Useable)/L" = "H38"
-"Battery System Parameters, Battery System Metrics, Battery system useable specific energy, Wh(Useable)/kg" = "H39"
-
-"Pack Parameters, Pack Configuration and Performance, Number of cells per pack" = "H43"
-"Pack Parameters, Pack Configuration and Performance, Number of modules per pack" = "H44"
-"Pack Parameters, Pack Configuration and Performance, Pack average OCV, V" = "H45"
-"Pack Parameters, Pack Configuration and Performance, Pack nominal operating voltage, V" = "H46"
-"Pack Parameters, Pack Configuration and Performance, Pack capacity, Ah" = "H47"
-"Pack Parameters, Pack Configuration and Performance, Pack total energy, kWh" = "H48"
-"Pack Parameters, Pack Configuration and Performance, Pack useable energy, kWh(Useable)" = "H49"
-"Pack Parameters, Pack Configuration and Performance, Pack power at target %OCV, kW" = "H50"
-"Pack Parameters, Pack Configuration and Performance, Pack power at rated power, kW" = "H51"
-
-"Pack Parameters, Pack Size, Pack length, mm" = "H54"
-"Pack Parameters, Pack Size, Pack width, mm" = "H55"
-"Pack Parameters, Pack Size, Pack height, mm" = "H56"
-"Pack Parameters, Pack Size, Pack volume, L" = "H57"
-"Pack Parameters, Pack Size, Pack total mass, kg" = "H58"
-
-"Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to power at target %OCV)" = "H61"
-"Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to rated power)" = "H62"
-"Pack Parameters, Pack Metrics, Pack energy density, Wh/L" = "H63"
-"Pack Parameters, Pack Metrics, Pack specific energy, Wh/kg" = "H64"
-"Pack Parameters, Pack Metrics, Pack useable energy density, Wh(Useable)/L" = "H65"
-"Pack Parameters, Pack Metrics, Pack useable specific energy, Wh(Useable)/kg" = "H66"
-
-"Module Parameters, Module Configuration and Performance, Number of cells per module" = "H70"
-"Module Parameters, Module Configuration and Performance, Module average OCV, V" = "H71"
-"Module Parameters, Module Configuration and Performance, Module nominal operating voltage, V" = "H72"
-"Module Parameters, Module Configuration and Performance, Module capacity, Ah" = "H73"
-"Module Parameters, Module Configuration and Performance, Module total energy, kWh" = "H74"
-"Module Parameters, Module Configuration and Performance, Module useable energy, kWh(Useable)" = "H75"
-"Module Parameters, Module Configuration and Performance, Module power at target %OCV, kW" = "H76"
-"Module Parameters, Module Configuration and Performance, Module power at rated power, kW" = "H77"
-
-"Module Parameters, Module Size, Module length, mm" = "H80"
-"Module Parameters, Module Size, Module width, mm" = "H81"
-"Module Parameters, Module Size, Module height, mm" = "H82"
-"Module Parameters, Module Size, Module volume, L" = "H83"
-"Module Parameters, Module Size, Module volume per pack, L" = "H84"
-"Module Parameters, Module Size, Module mass, kg" = "H85"
-"Module Parameters, Module Size, Module mass per pack, kg" = "H86"
-
-"Module Parameters, Module Metrics, Module energy density, Wh/L" = "H89"
-"Module Parameters, Module Metrics, Module specific energy, Wh/kg" = "H90"
-"Module Parameters, Module Metrics, Module useable energy density, Wh(Useable)/L" = "H91"
-"Module Parameters, Module Metrics, Module useable specific energy, Wh(Useable)/kg" = "H92"
-
-"Cell Parameters, Cell Performance, Cell average OCV, V" = "H96"
-"Cell Parameters, Cell Performance, Cell nominal operating voltage, V" = "H97"
-"Cell Parameters, Cell Performance, Cell capacity, Ah" = "H98"
-"Cell Parameters, Cell Performance, Cell total energy, kWh" = "H99"
-"Cell Parameters, Cell Performance, Cell useable energy, kWh(Useable)" = "H100"
-"Cell Parameters, Cell Performance, Cell power at target %OCV, kW" = "H101"
-"Cell Parameters, Cell Performance, Cell power at rated power, kW" = "H102"
-
-"Cell Parameters, Cell Size,Cell length, mm" = "H105"
-"Cell Parameters, Cell Size,Cell width, mm" = "H106"
-"Cell Parameters, Cell Size,Cell thickness, mm" = "H107"
-"Cell Parameters, Cell Size,Cell volume, L" = "H108"
-"Cell Parameters, Cell Size,Cell volume per pack, L" = "H109"
-"Cell Parameters, Cell Size,Cell mass, kg" = "H110"
-"Cell Parameters, Cell Size,Cell mass per pack, kg" = "H111"
-
-"Cell Parameters, Cell Metrics, Cell energy density, Wh/L" = "H114"
-"Cell Parameters, Cell Metrics, Cell specific energy, Wh/kg" = "H115"
-"Cell Parameters, Cell Metrics, Cell useable energy density, Wh(Useable)/L" = "H116"
-"Cell Parameters, Cell Metrics, Cell useable specific energy, Wh(Useable)/kg" = "H117"
-
-"Cell Parameters, Additional Cell Information, Positive electrode thickness, µm" = "H120"
-"Cell Parameters, Additional Cell Information, Negative electrode thickness, µm" = "H121"
-"Cell Parameters, Additional Cell Information, Positive electode areal capacity, mAh/cm²" = "H122"
-"Cell Parameters, Additional Cell Information, Negative electrode areal capacity, mAh/cm²" = "H123"
-
-# Manufacturing Information
-"Plant Size, GWh" = "H128"
-"Packs manufactured at 100% utilization (pack/year)" = "H129"
-"Packs manufactured per year (packs/year)" = "H130"
-"Modules manufactured per year (modules/year)" = "H131"
-"Accepted cells manufactured per year (cells/year)" = "H132"
-
-# Calculated Costs
-"Costs, Battery System, Battery system cost, $" = "H149"
-"Costs, Battery System, Battery system cost, $/kWh" = "H150"
-"Costs, Battery System, Battery system cost, $/kWh(Useable)" = "H151"
-
-"Costs, Pack, Pack cost, $/pack" = "H154"
-"Costs, Pack, Pack cost, $/kWh" = "H155"
-"Costs, Pack, Pack cost, $/kWh(Useable)" = "H156"
-
-"Costs, Module, Module cost, $/module" = "H159"
-"Costs, Module, Module cost per pack, $/pack" = "H160"
-"Costs, Module, Module cost, $/kWh" = "H161"
-"Costs, Module, Module cost, $/kWh(Useable)" = "H162"
-
-"Costs, Cell, Cell cost, $/cell" = "H165"
-"Costs, Cell, Cell cost, $/module" = "H166"
-"Costs, Cell, Cell cost, $/pack" = "H167"
-"Costs, Cell, Cell cost, $/kWh" = "H168"
-"Costs, Cell, Cell cost, $/kWh(Useable)" = "H169"
-
-"Costs, Additional Considerations, Module fraction of pack cost" = "H172"
-"Costs, Additional Considerations, Cell fraction of module cost" = "H173"
-"Costs, Additional Considerations, Cell fraction of pack cost" = "H174"
+    # Calculated Parameters
+    "Battery System Parameters, Battery System Configuration and Performance, Number of battery packs"                                = "H17"
+    "Battery System Parameters, Battery System Configuration and Performance, Packs in series or parallel"                            = "H18"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system average OCV, V"                          = "H19"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system nominal operating voltage, V"            = "H20"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system capacity, Ah"                            = "H21"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system total energy, kWh"                       = "H22"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system useable energy, kWh(Useable)"            = "H23"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system power at target % OCV, kW"               = "H24"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system rated power, kW"                         = "H25"
+    "Battery System Parameters, Battery System Configuration and Performance, Target SOC at full power, %"                            = "H26"
+    "Battery System Parameters, Battery System Configuration and Performance, Pulse time at rated power, s"                           = "H27"
+    "Battery System Parameters, Battery System Configuration and Performance, % OCV at rated power (adjusted for thickness limit), %" = "H28"
+    "Battery System Parameters, Battery System Configuration and Performance, Cooling system power requirement, W"                    = "H29"
+
+    "Battery System Parameters, Battery System Size, Battery system volume (all packs and cooling), L" = "H32"
+    "Battery System Parameters, Battery System Size, Battery system mass (all packs and cooling), kg"  = "H33"
+
+    "Battery System Parameters, Battery System Metrics, Battery system energy density, Wh/L"                    = "H36"
+    "Battery System Parameters, Battery System Metrics, Battery system specific energy, Wh/kg"                  = "H37"
+    "Battery System Parameters, Battery System Metrics, Battery system useable energy density, Wh(Useable)/L"   = "H38"
+    "Battery System Parameters, Battery System Metrics, Battery system useable specific energy, Wh(Useable)/kg" = "H39"
+
+    "Pack Parameters, Pack Configuration and Performance, Number of cells per pack"          = "H43"
+    "Pack Parameters, Pack Configuration and Performance, Number of modules per pack"        = "H44"
+    "Pack Parameters, Pack Configuration and Performance, Pack average OCV, V"               = "H45"
+    "Pack Parameters, Pack Configuration and Performance, Pack nominal operating voltage, V" = "H46"
+    "Pack Parameters, Pack Configuration and Performance, Pack capacity, Ah"                 = "H47"
+    "Pack Parameters, Pack Configuration and Performance, Pack total energy, kWh"            = "H48"
+    "Pack Parameters, Pack Configuration and Performance, Pack useable energy, kWh(Useable)" = "H49"
+    "Pack Parameters, Pack Configuration and Performance, Pack power at target %OCV, kW"     = "H50"
+    "Pack Parameters, Pack Configuration and Performance, Pack power at rated power, kW"     = "H51"
+
+    "Pack Parameters, Pack Size, Pack length, mm"     = "H54"
+    "Pack Parameters, Pack Size, Pack width, mm"      = "H55"
+    "Pack Parameters, Pack Size, Pack height, mm"     = "H56"
+    "Pack Parameters, Pack Size, Pack volume, L"      = "H57"
+    "Pack Parameters, Pack Size, Pack total mass, kg" = "H58"
+
+    "Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to power at target %OCV)" = "H61"
+    "Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to rated power)"          = "H62"
+    "Pack Parameters, Pack Metrics, Pack energy density, Wh/L"                                         = "H63"
+    "Pack Parameters, Pack Metrics, Pack specific energy, Wh/kg"                                       = "H64"
+    "Pack Parameters, Pack Metrics, Pack useable energy density, Wh(Useable)/L"                        = "H65"
+    "Pack Parameters, Pack Metrics, Pack useable specific energy, Wh(Useable)/kg"                      = "H66"
+
+    "Module Parameters, Module Configuration and Performance, Number of cells per module"          = "H70"
+    "Module Parameters, Module Configuration and Performance, Module average OCV, V"               = "H71"
+    "Module Parameters, Module Configuration and Performance, Module nominal operating voltage, V" = "H72"
+    "Module Parameters, Module Configuration and Performance, Module capacity, Ah"                 = "H73"
+    "Module Parameters, Module Configuration and Performance, Module total energy, kWh"            = "H74"
+    "Module Parameters, Module Configuration and Performance, Module useable energy, kWh(Useable)" = "H75"
+    "Module Parameters, Module Configuration and Performance, Module power at target %OCV, kW"     = "H76"
+    "Module Parameters, Module Configuration and Performance, Module power at rated power, kW"     = "H77"
+
+    "Module Parameters, Module Size, Module length, mm"         = "H80"
+    "Module Parameters, Module Size, Module width, mm"          = "H81"
+    "Module Parameters, Module Size, Module height, mm"         = "H82"
+    "Module Parameters, Module Size, Module volume, L"          = "H83"
+    "Module Parameters, Module Size, Module volume per pack, L" = "H84"
+    "Module Parameters, Module Size, Module mass, kg"           = "H85"
+    "Module Parameters, Module Size, Module mass per pack, kg"  = "H86"
+
+    "Module Parameters, Module Metrics, Module energy density, Wh/L"                    = "H89"
+    "Module Parameters, Module Metrics, Module specific energy, Wh/kg"                  = "H90"
+    "Module Parameters, Module Metrics, Module useable energy density, Wh(Useable)/L"   = "H91"
+    "Module Parameters, Module Metrics, Module useable specific energy, Wh(Useable)/kg" = "H92"
+
+    "Cell Parameters, Cell Performance, Cell average OCV, V"               = "H96"
+    "Cell Parameters, Cell Performance, Cell nominal operating voltage, V" = "H97"
+    "Cell Parameters, Cell Performance, Cell capacity, Ah"                 = "H98"
+    "Cell Parameters, Cell Performance, Cell total energy, kWh"            = "H99"
+    "Cell Parameters, Cell Performance, Cell useable energy, kWh(Useable)" = "H100"
+    "Cell Parameters, Cell Performance, Cell power at target %OCV, kW"     = "H101"
+    "Cell Parameters, Cell Performance, Cell power at rated power, kW"     = "H102"
+
+    "Cell Parameters, Cell Size,Cell length, mm"         = "H105"
+    "Cell Parameters, Cell Size,Cell width, mm"          = "H106"
+    "Cell Parameters, Cell Size,Cell thickness, mm"      = "H107"
+    "Cell Parameters, Cell Size,Cell volume, L"          = "H108"
+    "Cell Parameters, Cell Size,Cell volume per pack, L" = "H109"
+    "Cell Parameters, Cell Size,Cell mass, kg"           = "H110"
+    "Cell Parameters, Cell Size,Cell mass per pack, kg"  = "H111"
+
+    "Cell Parameters, Cell Metrics, Cell energy density, Wh/L"                    = "H114"
+    "Cell Parameters, Cell Metrics, Cell specific energy, Wh/kg"                  = "H115"
+    "Cell Parameters, Cell Metrics, Cell useable energy density, Wh(Useable)/L"   = "H116"
+    "Cell Parameters, Cell Metrics, Cell useable specific energy, Wh(Useable)/kg" = "H117"
+
+    "Cell Parameters, Additional Cell Information, Positive electrode thickness, µm"           = "H120"
+    "Cell Parameters, Additional Cell Information, Negative electrode thickness, µm"           = "H121"
+    "Cell Parameters, Additional Cell Information, Positive electode areal capacity, mAh/cm²"  = "H122"
+    "Cell Parameters, Additional Cell Information, Negative electrode areal capacity, mAh/cm²" = "H123"
+
+    # Manufacturing Information
+    "Plant Size, GWh"                                    = "H128"
+    "Packs manufactured at 100% utilization (pack/year)" = "H129"
+    "Packs manufactured per year (packs/year)"           = "H130"
+    "Modules manufactured per year (modules/year)"       = "H131"
+    "Accepted cells manufactured per year (cells/year)"  = "H132"
+
+    # Calculated Costs
+    "Costs, Battery System, Battery system cost, $"              = "H149"
+    "Costs, Battery System, Battery system cost, $/kWh"          = "H150"
+    "Costs, Battery System, Battery system cost, $/kWh(Useable)" = "H151"
+
+    "Costs, Pack, Pack cost, $/pack"         = "H154"
+    "Costs, Pack, Pack cost, $/kWh"          = "H155"
+    "Costs, Pack, Pack cost, $/kWh(Useable)" = "H156"
+
+    "Costs, Module, Module cost, $/module"        = "H159"
+    "Costs, Module, Module cost per pack, $/pack" = "H160"
+    "Costs, Module, Module cost, $/kWh"           = "H161"
+    "Costs, Module, Module cost, $/kWh(Useable)"  = "H162"
+
+    "Costs, Cell, Cell cost, $/cell"         = "H165"
+    "Costs, Cell, Cell cost, $/module"       = "H166"
+    "Costs, Cell, Cell cost, $/pack"         = "H167"
+    "Costs, Cell, Cell cost, $/kWh"          = "H168"
+    "Costs, Cell, Cell cost, $/kWh(Useable)" = "H169"
+
+    "Costs, Additional Considerations, Module fraction of pack cost" = "H172"
+    "Costs, Additional Considerations, Cell fraction of module cost" = "H173"
+    "Costs, Additional Considerations, Cell fraction of pack cost"   = "H174"
 
 ["Summary of Results"."Battery 3"]
-# Calculated Parameters
-"Battery System Parameters, Battery System Configuration and Performance, Number of battery packs" = "I17"
-"Battery System Parameters, Battery System Configuration and Performance, Packs in series or parallel" = "I18"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system average OCV, V" = "I19"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system nominal operating voltage, V" = "I20"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system capacity, Ah" = "I21"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system total energy, kWh" = "I22"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system useable energy, kWh(Useable)" = "I23"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system power at target % OCV, kW" = "I24"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system rated power, kW" = "I25"
-"Battery System Parameters, Battery System Configuration and Performance, Target SOC at full power, %" = "I26"
-"Battery System Parameters, Battery System Configuration and Performance, Pulse time at rated power, s" = "I27"
-"Battery System Parameters, Battery System Configuration and Performance, % OCV at rated power (adjusted for thickness limit), %" = "I28"
-"Battery System Parameters, Battery System Configuration and Performance, Cooling system power requirement, W" = "I29"
-
-"Battery System Parameters, Battery System Size, Battery system volume (all packs and cooling), L" = "I32"
-"Battery System Parameters, Battery System Size, Battery system mass (all packs and cooling), kg" = "I33"
-
-"Battery System Parameters, Battery System Metrics, Battery system energy density, Wh/L" = "I36"
-"Battery System Parameters, Battery System Metrics, Battery system specific energy, Wh/kg" = "I37"
-"Battery System Parameters, Battery System Metrics, Battery system useable energy density, Wh(Useable)/L" = "I38"
-"Battery System Parameters, Battery System Metrics, Battery system useable specific energy, Wh(Useable)/kg" = "I39"
-
-"Pack Parameters, Pack Configuration and Performance, Number of cells per pack" = "I43"
-"Pack Parameters, Pack Configuration and Performance, Number of modules per pack" = "I44"
-"Pack Parameters, Pack Configuration and Performance, Pack average OCV, V" = "I45"
-"Pack Parameters, Pack Configuration and Performance, Pack nominal operating voltage, V" = "I46"
-"Pack Parameters, Pack Configuration and Performance, Pack capacity, Ah" = "I47"
-"Pack Parameters, Pack Configuration and Performance, Pack total energy, kWh" = "I48"
-"Pack Parameters, Pack Configuration and Performance, Pack useable energy, kWh(Useable)" = "I49"
-"Pack Parameters, Pack Configuration and Performance, Pack power at target %OCV, kW" = "I50"
-"Pack Parameters, Pack Configuration and Performance, Pack power at rated power, kW" = "I51"
-
-"Pack Parameters, Pack Size, Pack length, mm" = "I54"
-"Pack Parameters, Pack Size, Pack width, mm" = "I55"
-"Pack Parameters, Pack Size, Pack height, mm" = "I56"
-"Pack Parameters, Pack Size, Pack volume, L" = "I57"
-"Pack Parameters, Pack Size, Pack total mass, kg" = "I58"
-
-"Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to power at target %OCV)" = "I61"
-"Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to rated power)" = "I62"
-"Pack Parameters, Pack Metrics, Pack energy density, Wh/L" = "I63"
-"Pack Parameters, Pack Metrics, Pack specific energy, Wh/kg" = "I64"
-"Pack Parameters, Pack Metrics, Pack useable energy density, Wh(Useable)/L" = "I65"
-"Pack Parameters, Pack Metrics, Pack useable specific energy, Wh(Useable)/kg" = "I66"
-
-"Module Parameters, Module Configuration and Performance, Number of cells per module" = "I70"
-"Module Parameters, Module Configuration and Performance, Module average OCV, V" = "I71"
-"Module Parameters, Module Configuration and Performance, Module nominal operating voltage, V" = "I72"
-"Module Parameters, Module Configuration and Performance, Module capacity, Ah" = "I73"
-"Module Parameters, Module Configuration and Performance, Module total energy, kWh" = "I74"
-"Module Parameters, Module Configuration and Performance, Module useable energy, kWh(Useable)" = "I75"
-"Module Parameters, Module Configuration and Performance, Module power at target %OCV, kW" = "I76"
-"Module Parameters, Module Configuration and Performance, Module power at rated power, kW" = "I77"
-
-"Module Parameters, Module Size, Module length, mm" = "I80"
-"Module Parameters, Module Size, Module width, mm" = "I81"
-"Module Parameters, Module Size, Module height, mm" = "I82"
-"Module Parameters, Module Size, Module volume, L" = "I83"
-"Module Parameters, Module Size, Module volume per pack, L" = "I84"
-"Module Parameters, Module Size, Module mass, kg" = "I85"
-"Module Parameters, Module Size, Module mass per pack, kg" = "I86"
-
-"Module Parameters, Module Metrics, Module energy density, Wh/L" = "I89"
-"Module Parameters, Module Metrics, Module specific energy, Wh/kg" = "I90"
-"Module Parameters, Module Metrics, Module useable energy density, Wh(Useable)/L" = "I91"
-"Module Parameters, Module Metrics, Module useable specific energy, Wh(Useable)/kg" = "I92"
-
-"Cell Parameters, Cell Performance, Cell average OCV, V" = "I96"
-"Cell Parameters, Cell Performance, Cell nominal operating voltage, V" = "I97"
-"Cell Parameters, Cell Performance, Cell capacity, Ah" = "I98"
-"Cell Parameters, Cell Performance, Cell total energy, kWh" = "I99"
-"Cell Parameters, Cell Performance, Cell useable energy, kWh(Useable)" = "I100"
-"Cell Parameters, Cell Performance, Cell power at target %OCV, kW" = "I101"
-"Cell Parameters, Cell Performance, Cell power at rated power, kW" = "I102"
-
-"Cell Parameters, Cell Size,Cell length, mm" = "I105"
-"Cell Parameters, Cell Size,Cell width, mm" = "I106"
-"Cell Parameters, Cell Size,Cell thickness, mm" = "I107"
-"Cell Parameters, Cell Size,Cell volume, L" = "I108"
-"Cell Parameters, Cell Size,Cell volume per pack, L" = "I109"
-"Cell Parameters, Cell Size,Cell mass, kg" = "I110"
-"Cell Parameters, Cell Size,Cell mass per pack, kg" = "I111"
-
-"Cell Parameters, Cell Metrics, Cell energy density, Wh/L" = "I114"
-"Cell Parameters, Cell Metrics, Cell specific energy, Wh/kg" = "I115"
-"Cell Parameters, Cell Metrics, Cell useable energy density, Wh(Useable)/L" = "I116"
-"Cell Parameters, Cell Metrics, Cell useable specific energy, Wh(Useable)/kg" = "I117"
-
-"Cell Parameters, Additional Cell Information, Positive electrode thickness, µm" = "I120"
-"Cell Parameters, Additional Cell Information, Negative electrode thickness, µm" = "I121"
-"Cell Parameters, Additional Cell Information, Positive electode areal capacity, mAh/cm²" = "I122"
-"Cell Parameters, Additional Cell Information, Negative electrode areal capacity, mAh/cm²" = "I123"
-
-# Manufacturing Information
-"Plant Size, GWh" = "I128"
-"Packs manufactured at 100% utilization (pack/year)" = "I129"
-"Packs manufactured per year (packs/year)" = "I130"
-"Modules manufactured per year (modules/year)" = "I131"
-"Accepted cells manufactured per year (cells/year)" = "I132"
-
-# Calculated Costs
-"Costs, Battery System, Battery system cost, $" = "I149"
-"Costs, Battery System, Battery system cost, $/kWh" = "I150"
-"Costs, Battery System, Battery system cost, $/kWh(Useable)" = "I151"
-
-"Costs, Pack, Pack cost, $/pack" = "I154"
-"Costs, Pack, Pack cost, $/kWh" = "I155"
-"Costs, Pack, Pack cost, $/kWh(Useable)" = "I156"
-
-"Costs, Module, Module cost, $/module" = "I159"
-"Costs, Module, Module cost per pack, $/pack" = "I160"
-"Costs, Module, Module cost, $/kWh" = "I161"
-"Costs, Module, Module cost, $/kWh(Useable)" = "I162"
-
-"Costs, Cell, Cell cost, $/cell" = "I165"
-"Costs, Cell, Cell cost, $/module" = "I166"
-"Costs, Cell, Cell cost, $/pack" = "I167"
-"Costs, Cell, Cell cost, $/kWh" = "I168"
-"Costs, Cell, Cell cost, $/kWh(Useable)" = "I169"
-
-"Costs, Additional Considerations, Module fraction of pack cost" = "I172"
-"Costs, Additional Considerations, Cell fraction of module cost" = "I173"
-"Costs, Additional Considerations, Cell fraction of pack cost" = "I174"
+    # Calculated Parameters
+    "Battery System Parameters, Battery System Configuration and Performance, Number of battery packs"                                = "I17"
+    "Battery System Parameters, Battery System Configuration and Performance, Packs in series or parallel"                            = "I18"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system average OCV, V"                          = "I19"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system nominal operating voltage, V"            = "I20"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system capacity, Ah"                            = "I21"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system total energy, kWh"                       = "I22"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system useable energy, kWh(Useable)"            = "I23"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system power at target % OCV, kW"               = "I24"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system rated power, kW"                         = "I25"
+    "Battery System Parameters, Battery System Configuration and Performance, Target SOC at full power, %"                            = "I26"
+    "Battery System Parameters, Battery System Configuration and Performance, Pulse time at rated power, s"                           = "I27"
+    "Battery System Parameters, Battery System Configuration and Performance, % OCV at rated power (adjusted for thickness limit), %" = "I28"
+    "Battery System Parameters, Battery System Configuration and Performance, Cooling system power requirement, W"                    = "I29"
+
+    "Battery System Parameters, Battery System Size, Battery system volume (all packs and cooling), L" = "I32"
+    "Battery System Parameters, Battery System Size, Battery system mass (all packs and cooling), kg"  = "I33"
+
+    "Battery System Parameters, Battery System Metrics, Battery system energy density, Wh/L"                    = "I36"
+    "Battery System Parameters, Battery System Metrics, Battery system specific energy, Wh/kg"                  = "I37"
+    "Battery System Parameters, Battery System Metrics, Battery system useable energy density, Wh(Useable)/L"   = "I38"
+    "Battery System Parameters, Battery System Metrics, Battery system useable specific energy, Wh(Useable)/kg" = "I39"
+
+    "Pack Parameters, Pack Configuration and Performance, Number of cells per pack"          = "I43"
+    "Pack Parameters, Pack Configuration and Performance, Number of modules per pack"        = "I44"
+    "Pack Parameters, Pack Configuration and Performance, Pack average OCV, V"               = "I45"
+    "Pack Parameters, Pack Configuration and Performance, Pack nominal operating voltage, V" = "I46"
+    "Pack Parameters, Pack Configuration and Performance, Pack capacity, Ah"                 = "I47"
+    "Pack Parameters, Pack Configuration and Performance, Pack total energy, kWh"            = "I48"
+    "Pack Parameters, Pack Configuration and Performance, Pack useable energy, kWh(Useable)" = "I49"
+    "Pack Parameters, Pack Configuration and Performance, Pack power at target %OCV, kW"     = "I50"
+    "Pack Parameters, Pack Configuration and Performance, Pack power at rated power, kW"     = "I51"
+
+    "Pack Parameters, Pack Size, Pack length, mm"     = "I54"
+    "Pack Parameters, Pack Size, Pack width, mm"      = "I55"
+    "Pack Parameters, Pack Size, Pack height, mm"     = "I56"
+    "Pack Parameters, Pack Size, Pack volume, L"      = "I57"
+    "Pack Parameters, Pack Size, Pack total mass, kg" = "I58"
+
+    "Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to power at target %OCV)" = "I61"
+    "Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to rated power)"          = "I62"
+    "Pack Parameters, Pack Metrics, Pack energy density, Wh/L"                                         = "I63"
+    "Pack Parameters, Pack Metrics, Pack specific energy, Wh/kg"                                       = "I64"
+    "Pack Parameters, Pack Metrics, Pack useable energy density, Wh(Useable)/L"                        = "I65"
+    "Pack Parameters, Pack Metrics, Pack useable specific energy, Wh(Useable)/kg"                      = "I66"
+
+    "Module Parameters, Module Configuration and Performance, Number of cells per module"          = "I70"
+    "Module Parameters, Module Configuration and Performance, Module average OCV, V"               = "I71"
+    "Module Parameters, Module Configuration and Performance, Module nominal operating voltage, V" = "I72"
+    "Module Parameters, Module Configuration and Performance, Module capacity, Ah"                 = "I73"
+    "Module Parameters, Module Configuration and Performance, Module total energy, kWh"            = "I74"
+    "Module Parameters, Module Configuration and Performance, Module useable energy, kWh(Useable)" = "I75"
+    "Module Parameters, Module Configuration and Performance, Module power at target %OCV, kW"     = "I76"
+    "Module Parameters, Module Configuration and Performance, Module power at rated power, kW"     = "I77"
+
+    "Module Parameters, Module Size, Module length, mm"         = "I80"
+    "Module Parameters, Module Size, Module width, mm"          = "I81"
+    "Module Parameters, Module Size, Module height, mm"         = "I82"
+    "Module Parameters, Module Size, Module volume, L"          = "I83"
+    "Module Parameters, Module Size, Module volume per pack, L" = "I84"
+    "Module Parameters, Module Size, Module mass, kg"           = "I85"
+    "Module Parameters, Module Size, Module mass per pack, kg"  = "I86"
+
+    "Module Parameters, Module Metrics, Module energy density, Wh/L"                    = "I89"
+    "Module Parameters, Module Metrics, Module specific energy, Wh/kg"                  = "I90"
+    "Module Parameters, Module Metrics, Module useable energy density, Wh(Useable)/L"   = "I91"
+    "Module Parameters, Module Metrics, Module useable specific energy, Wh(Useable)/kg" = "I92"
+
+    "Cell Parameters, Cell Performance, Cell average OCV, V"               = "I96"
+    "Cell Parameters, Cell Performance, Cell nominal operating voltage, V" = "I97"
+    "Cell Parameters, Cell Performance, Cell capacity, Ah"                 = "I98"
+    "Cell Parameters, Cell Performance, Cell total energy, kWh"            = "I99"
+    "Cell Parameters, Cell Performance, Cell useable energy, kWh(Useable)" = "I100"
+    "Cell Parameters, Cell Performance, Cell power at target %OCV, kW"     = "I101"
+    "Cell Parameters, Cell Performance, Cell power at rated power, kW"     = "I102"
+
+    "Cell Parameters, Cell Size,Cell length, mm"         = "I105"
+    "Cell Parameters, Cell Size,Cell width, mm"          = "I106"
+    "Cell Parameters, Cell Size,Cell thickness, mm"      = "I107"
+    "Cell Parameters, Cell Size,Cell volume, L"          = "I108"
+    "Cell Parameters, Cell Size,Cell volume per pack, L" = "I109"
+    "Cell Parameters, Cell Size,Cell mass, kg"           = "I110"
+    "Cell Parameters, Cell Size,Cell mass per pack, kg"  = "I111"
+
+    "Cell Parameters, Cell Metrics, Cell energy density, Wh/L"                    = "I114"
+    "Cell Parameters, Cell Metrics, Cell specific energy, Wh/kg"                  = "I115"
+    "Cell Parameters, Cell Metrics, Cell useable energy density, Wh(Useable)/L"   = "I116"
+    "Cell Parameters, Cell Metrics, Cell useable specific energy, Wh(Useable)/kg" = "I117"
+
+    "Cell Parameters, Additional Cell Information, Positive electrode thickness, µm"           = "I120"
+    "Cell Parameters, Additional Cell Information, Negative electrode thickness, µm"           = "I121"
+    "Cell Parameters, Additional Cell Information, Positive electode areal capacity, mAh/cm²"  = "I122"
+    "Cell Parameters, Additional Cell Information, Negative electrode areal capacity, mAh/cm²" = "I123"
+
+    # Manufacturing Information
+    "Plant Size, GWh"                                    = "I128"
+    "Packs manufactured at 100% utilization (pack/year)" = "I129"
+    "Packs manufactured per year (packs/year)"           = "I130"
+    "Modules manufactured per year (modules/year)"       = "I131"
+    "Accepted cells manufactured per year (cells/year)"  = "I132"
+
+    # Calculated Costs
+    "Costs, Battery System, Battery system cost, $"              = "I149"
+    "Costs, Battery System, Battery system cost, $/kWh"          = "I150"
+    "Costs, Battery System, Battery system cost, $/kWh(Useable)" = "I151"
+
+    "Costs, Pack, Pack cost, $/pack"         = "I154"
+    "Costs, Pack, Pack cost, $/kWh"          = "I155"
+    "Costs, Pack, Pack cost, $/kWh(Useable)" = "I156"
+
+    "Costs, Module, Module cost, $/module"        = "I159"
+    "Costs, Module, Module cost per pack, $/pack" = "I160"
+    "Costs, Module, Module cost, $/kWh"           = "I161"
+    "Costs, Module, Module cost, $/kWh(Useable)"  = "I162"
+
+    "Costs, Cell, Cell cost, $/cell"         = "I165"
+    "Costs, Cell, Cell cost, $/module"       = "I166"
+    "Costs, Cell, Cell cost, $/pack"         = "I167"
+    "Costs, Cell, Cell cost, $/kWh"          = "I168"
+    "Costs, Cell, Cell cost, $/kWh(Useable)" = "I169"
+
+    "Costs, Additional Considerations, Module fraction of pack cost" = "I172"
+    "Costs, Additional Considerations, Cell fraction of module cost" = "I173"
+    "Costs, Additional Considerations, Cell fraction of pack cost"   = "I174"
 
 ["Summary of Results"."Battery 4"]
-# Calculated Parameters
-"Battery System Parameters, Battery System Configuration and Performance, Number of battery packs" = "J17"
-"Battery System Parameters, Battery System Configuration and Performance, Packs in series or parallel" = "J18"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system average OCV, V" = "J19"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system nominal operating voltage, V" = "J20"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system capacity, Ah" = "J21"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system total energy, kWh" = "J22"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system useable energy, kWh(Useable)" = "J23"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system power at target % OCV, kW" = "J24"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system rated power, kW" = "J25"
-"Battery System Parameters, Battery System Configuration and Performance, Target SOC at full power, %" = "J26"
-"Battery System Parameters, Battery System Configuration and Performance, Pulse time at rated power, s" = "J27"
-"Battery System Parameters, Battery System Configuration and Performance, % OCV at rated power (adjusted for thickness limit), %" = "J28"
-"Battery System Parameters, Battery System Configuration and Performance, Cooling system power requirement, W" = "J29"
-
-"Battery System Parameters, Battery System Size, Battery system volume (all packs and cooling), L" = "J32"
-"Battery System Parameters, Battery System Size, Battery system mass (all packs and cooling), kg" = "J33"
-
-"Battery System Parameters, Battery System Metrics, Battery system energy density, Wh/L" = "J36"
-"Battery System Parameters, Battery System Metrics, Battery system specific energy, Wh/kg" = "J37"
-"Battery System Parameters, Battery System Metrics, Battery system useable energy density, Wh(Useable)/L" = "J38"
-"Battery System Parameters, Battery System Metrics, Battery system useable specific energy, Wh(Useable)/kg" = "J39"
-
-"Pack Parameters, Pack Configuration and Performance, Number of cells per pack" = "J43"
-"Pack Parameters, Pack Configuration and Performance, Number of modules per pack" = "J44"
-"Pack Parameters, Pack Configuration and Performance, Pack average OCV, V" = "J45"
-"Pack Parameters, Pack Configuration and Performance, Pack nominal operating voltage, V" = "J46"
-"Pack Parameters, Pack Configuration and Performance, Pack capacity, Ah" = "J47"
-"Pack Parameters, Pack Configuration and Performance, Pack total energy, kWh" = "J48"
-"Pack Parameters, Pack Configuration and Performance, Pack useable energy, kWh(Useable)" = "J49"
-"Pack Parameters, Pack Configuration and Performance, Pack power at target %OCV, kW" = "J50"
-"Pack Parameters, Pack Configuration and Performance, Pack power at rated power, kW" = "J51"
-
-"Pack Parameters, Pack Size, Pack length, mm" = "J54"
-"Pack Parameters, Pack Size, Pack width, mm" = "J55"
-"Pack Parameters, Pack Size, Pack height, mm" = "J56"
-"Pack Parameters, Pack Size, Pack volume, L" = "J57"
-"Pack Parameters, Pack Size, Pack total mass, kg" = "J58"
-
-"Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to power at target %OCV)" = "J61"
-"Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to rated power)" = "J62"
-"Pack Parameters, Pack Metrics, Pack energy density, Wh/L" = "J63"
-"Pack Parameters, Pack Metrics, Pack specific energy, Wh/kg" = "J64"
-"Pack Parameters, Pack Metrics, Pack useable energy density, Wh(Useable)/L" = "J65"
-"Pack Parameters, Pack Metrics, Pack useable specific energy, Wh(Useable)/kg" = "J66"
-
-"Module Parameters, Module Configuration and Performance, Number of cells per module" = "J70"
-"Module Parameters, Module Configuration and Performance, Module average OCV, V" = "J71"
-"Module Parameters, Module Configuration and Performance, Module nominal operating voltage, V" = "J72"
-"Module Parameters, Module Configuration and Performance, Module capacity, Ah" = "J73"
-"Module Parameters, Module Configuration and Performance, Module total energy, kWh" = "J74"
-"Module Parameters, Module Configuration and Performance, Module useable energy, kWh(Useable)" = "J75"
-"Module Parameters, Module Configuration and Performance, Module power at target %OCV, kW" = "J76"
-"Module Parameters, Module Configuration and Performance, Module power at rated power, kW" = "J77"
-
-"Module Parameters, Module Size, Module length, mm" = "J80"
-"Module Parameters, Module Size, Module width, mm" = "J81"
-"Module Parameters, Module Size, Module height, mm" = "J82"
-"Module Parameters, Module Size, Module volume, L" = "J83"
-"Module Parameters, Module Size, Module volume per pack, L" = "J84"
-"Module Parameters, Module Size, Module mass, kg" = "J85"
-"Module Parameters, Module Size, Module mass per pack, kg" = "J86"
-
-"Module Parameters, Module Metrics, Module energy density, Wh/L" = "J89"
-"Module Parameters, Module Metrics, Module specific energy, Wh/kg" = "J90"
-"Module Parameters, Module Metrics, Module useable energy density, Wh(Useable)/L" = "J91"
-"Module Parameters, Module Metrics, Module useable specific energy, Wh(Useable)/kg" = "J92"
-
-"Cell Parameters, Cell Performance, Cell average OCV, V" = "J96"
-"Cell Parameters, Cell Performance, Cell nominal operating voltage, V" = "J97"
-"Cell Parameters, Cell Performance, Cell capacity, Ah" = "J98"
-"Cell Parameters, Cell Performance, Cell total energy, kWh" = "J99"
-"Cell Parameters, Cell Performance, Cell useable energy, kWh(Useable)" = "J100"
-"Cell Parameters, Cell Performance, Cell power at target %OCV, kW" = "J101"
-"Cell Parameters, Cell Performance, Cell power at rated power, kW" = "J102"
-
-"Cell Parameters, Cell Size,Cell length, mm" = "J105"
-"Cell Parameters, Cell Size,Cell width, mm" = "J106"
-"Cell Parameters, Cell Size,Cell thickness, mm" = "J107"
-"Cell Parameters, Cell Size,Cell volume, L" = "J108"
-"Cell Parameters, Cell Size,Cell volume per pack, L" = "J109"
-"Cell Parameters, Cell Size,Cell mass, kg" = "J110"
-"Cell Parameters, Cell Size,Cell mass per pack, kg" = "J111"
-
-"Cell Parameters, Cell Metrics, Cell energy density, Wh/L" = "J114"
-"Cell Parameters, Cell Metrics, Cell specific energy, Wh/kg" = "J115"
-"Cell Parameters, Cell Metrics, Cell useable energy density, Wh(Useable)/L" = "J116"
-"Cell Parameters, Cell Metrics, Cell useable specific energy, Wh(Useable)/kg" = "J117"
-
-"Cell Parameters, Additional Cell Information, Positive electrode thickness, µm" = "J120"
-"Cell Parameters, Additional Cell Information, Negative electrode thickness, µm" = "J121"
-"Cell Parameters, Additional Cell Information, Positive electode areal capacity, mAh/cm²" = "J122"
-"Cell Parameters, Additional Cell Information, Negative electrode areal capacity, mAh/cm²" = "J123"
-
-# Manufacturing Information
-"Plant Size, GWh" = "J128"
-"Packs manufactured at 100% utilization (pack/year)" = "J129"
-"Packs manufactured per year (packs/year)" = "J130"
-"Modules manufactured per year (modules/year)" = "J131"
-"Accepted cells manufactured per year (cells/year)" = "J132"
-
-# Calculated Costs
-"Costs, Battery System, Battery system cost, $" = "J149"
-"Costs, Battery System, Battery system cost, $/kWh" = "J150"
-"Costs, Battery System, Battery system cost, $/kWh(Useable)" = "J151"
-
-"Costs, Pack, Pack cost, $/pack" = "J154"
-"Costs, Pack, Pack cost, $/kWh" = "J155"
-"Costs, Pack, Pack cost, $/kWh(Useable)" = "J156"
-
-"Costs, Module, Module cost, $/module" = "J159"
-"Costs, Module, Module cost per pack, $/pack" = "J160"
-"Costs, Module, Module cost, $/kWh" = "J161"
-"Costs, Module, Module cost, $/kWh(Useable)" = "J162"
-
-"Costs, Cell, Cell cost, $/cell" = "J165"
-"Costs, Cell, Cell cost, $/module" = "J166"
-"Costs, Cell, Cell cost, $/pack" = "J167"
-"Costs, Cell, Cell cost, $/kWh" = "J168"
-"Costs, Cell, Cell cost, $/kWh(Useable)" = "J169"
-
-"Costs, Additional Considerations, Module fraction of pack cost" = "J172"
-"Costs, Additional Considerations, Cell fraction of module cost" = "J173"
-"Costs, Additional Considerations, Cell fraction of pack cost" = "J174"
+    # Calculated Parameters
+    "Battery System Parameters, Battery System Configuration and Performance, Number of battery packs"                                = "J17"
+    "Battery System Parameters, Battery System Configuration and Performance, Packs in series or parallel"                            = "J18"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system average OCV, V"                          = "J19"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system nominal operating voltage, V"            = "J20"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system capacity, Ah"                            = "J21"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system total energy, kWh"                       = "J22"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system useable energy, kWh(Useable)"            = "J23"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system power at target % OCV, kW"               = "J24"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system rated power, kW"                         = "J25"
+    "Battery System Parameters, Battery System Configuration and Performance, Target SOC at full power, %"                            = "J26"
+    "Battery System Parameters, Battery System Configuration and Performance, Pulse time at rated power, s"                           = "J27"
+    "Battery System Parameters, Battery System Configuration and Performance, % OCV at rated power (adjusted for thickness limit), %" = "J28"
+    "Battery System Parameters, Battery System Configuration and Performance, Cooling system power requirement, W"                    = "J29"
+
+    "Battery System Parameters, Battery System Size, Battery system volume (all packs and cooling), L" = "J32"
+    "Battery System Parameters, Battery System Size, Battery system mass (all packs and cooling), kg"  = "J33"
+
+    "Battery System Parameters, Battery System Metrics, Battery system energy density, Wh/L"                    = "J36"
+    "Battery System Parameters, Battery System Metrics, Battery system specific energy, Wh/kg"                  = "J37"
+    "Battery System Parameters, Battery System Metrics, Battery system useable energy density, Wh(Useable)/L"   = "J38"
+    "Battery System Parameters, Battery System Metrics, Battery system useable specific energy, Wh(Useable)/kg" = "J39"
+
+    "Pack Parameters, Pack Configuration and Performance, Number of cells per pack"          = "J43"
+    "Pack Parameters, Pack Configuration and Performance, Number of modules per pack"        = "J44"
+    "Pack Parameters, Pack Configuration and Performance, Pack average OCV, V"               = "J45"
+    "Pack Parameters, Pack Configuration and Performance, Pack nominal operating voltage, V" = "J46"
+    "Pack Parameters, Pack Configuration and Performance, Pack capacity, Ah"                 = "J47"
+    "Pack Parameters, Pack Configuration and Performance, Pack total energy, kWh"            = "J48"
+    "Pack Parameters, Pack Configuration and Performance, Pack useable energy, kWh(Useable)" = "J49"
+    "Pack Parameters, Pack Configuration and Performance, Pack power at target %OCV, kW"     = "J50"
+    "Pack Parameters, Pack Configuration and Performance, Pack power at rated power, kW"     = "J51"
+
+    "Pack Parameters, Pack Size, Pack length, mm"     = "J54"
+    "Pack Parameters, Pack Size, Pack width, mm"      = "J55"
+    "Pack Parameters, Pack Size, Pack height, mm"     = "J56"
+    "Pack Parameters, Pack Size, Pack volume, L"      = "J57"
+    "Pack Parameters, Pack Size, Pack total mass, kg" = "J58"
+
+    "Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to power at target %OCV)" = "J61"
+    "Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to rated power)"          = "J62"
+    "Pack Parameters, Pack Metrics, Pack energy density, Wh/L"                                         = "J63"
+    "Pack Parameters, Pack Metrics, Pack specific energy, Wh/kg"                                       = "J64"
+    "Pack Parameters, Pack Metrics, Pack useable energy density, Wh(Useable)/L"                        = "J65"
+    "Pack Parameters, Pack Metrics, Pack useable specific energy, Wh(Useable)/kg"                      = "J66"
+
+    "Module Parameters, Module Configuration and Performance, Number of cells per module"          = "J70"
+    "Module Parameters, Module Configuration and Performance, Module average OCV, V"               = "J71"
+    "Module Parameters, Module Configuration and Performance, Module nominal operating voltage, V" = "J72"
+    "Module Parameters, Module Configuration and Performance, Module capacity, Ah"                 = "J73"
+    "Module Parameters, Module Configuration and Performance, Module total energy, kWh"            = "J74"
+    "Module Parameters, Module Configuration and Performance, Module useable energy, kWh(Useable)" = "J75"
+    "Module Parameters, Module Configuration and Performance, Module power at target %OCV, kW"     = "J76"
+    "Module Parameters, Module Configuration and Performance, Module power at rated power, kW"     = "J77"
+
+    "Module Parameters, Module Size, Module length, mm"         = "J80"
+    "Module Parameters, Module Size, Module width, mm"          = "J81"
+    "Module Parameters, Module Size, Module height, mm"         = "J82"
+    "Module Parameters, Module Size, Module volume, L"          = "J83"
+    "Module Parameters, Module Size, Module volume per pack, L" = "J84"
+    "Module Parameters, Module Size, Module mass, kg"           = "J85"
+    "Module Parameters, Module Size, Module mass per pack, kg"  = "J86"
+
+    "Module Parameters, Module Metrics, Module energy density, Wh/L"                    = "J89"
+    "Module Parameters, Module Metrics, Module specific energy, Wh/kg"                  = "J90"
+    "Module Parameters, Module Metrics, Module useable energy density, Wh(Useable)/L"   = "J91"
+    "Module Parameters, Module Metrics, Module useable specific energy, Wh(Useable)/kg" = "J92"
+
+    "Cell Parameters, Cell Performance, Cell average OCV, V"               = "J96"
+    "Cell Parameters, Cell Performance, Cell nominal operating voltage, V" = "J97"
+    "Cell Parameters, Cell Performance, Cell capacity, Ah"                 = "J98"
+    "Cell Parameters, Cell Performance, Cell total energy, kWh"            = "J99"
+    "Cell Parameters, Cell Performance, Cell useable energy, kWh(Useable)" = "J100"
+    "Cell Parameters, Cell Performance, Cell power at target %OCV, kW"     = "J101"
+    "Cell Parameters, Cell Performance, Cell power at rated power, kW"     = "J102"
+
+    "Cell Parameters, Cell Size,Cell length, mm"         = "J105"
+    "Cell Parameters, Cell Size,Cell width, mm"          = "J106"
+    "Cell Parameters, Cell Size,Cell thickness, mm"      = "J107"
+    "Cell Parameters, Cell Size,Cell volume, L"          = "J108"
+    "Cell Parameters, Cell Size,Cell volume per pack, L" = "J109"
+    "Cell Parameters, Cell Size,Cell mass, kg"           = "J110"
+    "Cell Parameters, Cell Size,Cell mass per pack, kg"  = "J111"
+
+    "Cell Parameters, Cell Metrics, Cell energy density, Wh/L"                    = "J114"
+    "Cell Parameters, Cell Metrics, Cell specific energy, Wh/kg"                  = "J115"
+    "Cell Parameters, Cell Metrics, Cell useable energy density, Wh(Useable)/L"   = "J116"
+    "Cell Parameters, Cell Metrics, Cell useable specific energy, Wh(Useable)/kg" = "J117"
+
+    "Cell Parameters, Additional Cell Information, Positive electrode thickness, µm"           = "J120"
+    "Cell Parameters, Additional Cell Information, Negative electrode thickness, µm"           = "J121"
+    "Cell Parameters, Additional Cell Information, Positive electode areal capacity, mAh/cm²"  = "J122"
+    "Cell Parameters, Additional Cell Information, Negative electrode areal capacity, mAh/cm²" = "J123"
+
+    # Manufacturing Information
+    "Plant Size, GWh"                                    = "J128"
+    "Packs manufactured at 100% utilization (pack/year)" = "J129"
+    "Packs manufactured per year (packs/year)"           = "J130"
+    "Modules manufactured per year (modules/year)"       = "J131"
+    "Accepted cells manufactured per year (cells/year)"  = "J132"
+
+    # Calculated Costs
+    "Costs, Battery System, Battery system cost, $"              = "J149"
+    "Costs, Battery System, Battery system cost, $/kWh"          = "J150"
+    "Costs, Battery System, Battery system cost, $/kWh(Useable)" = "J151"
+
+    "Costs, Pack, Pack cost, $/pack"         = "J154"
+    "Costs, Pack, Pack cost, $/kWh"          = "J155"
+    "Costs, Pack, Pack cost, $/kWh(Useable)" = "J156"
+
+    "Costs, Module, Module cost, $/module"        = "J159"
+    "Costs, Module, Module cost per pack, $/pack" = "J160"
+    "Costs, Module, Module cost, $/kWh"           = "J161"
+    "Costs, Module, Module cost, $/kWh(Useable)"  = "J162"
+
+    "Costs, Cell, Cell cost, $/cell"         = "J165"
+    "Costs, Cell, Cell cost, $/module"       = "J166"
+    "Costs, Cell, Cell cost, $/pack"         = "J167"
+    "Costs, Cell, Cell cost, $/kWh"          = "J168"
+    "Costs, Cell, Cell cost, $/kWh(Useable)" = "J169"
+
+    "Costs, Additional Considerations, Module fraction of pack cost" = "J172"
+    "Costs, Additional Considerations, Cell fraction of module cost" = "J173"
+    "Costs, Additional Considerations, Cell fraction of pack cost"   = "J174"
 
 ["Summary of Results"."Battery 5"]
-# Calculated Parameters
-"Battery System Parameters, Battery System Configuration and Performance, Number of battery packs" = "K17"
-"Battery System Parameters, Battery System Configuration and Performance, Packs in series or parallel" = "K18"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system average OCV, V" = "K19"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system nominal operating voltage, V" = "K20"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system capacity, Ah" = "K21"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system total energy, kWh" = "K22"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system useable energy, kWh(Useable)" = "K23"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system power at target % OCV, kW" = "K24"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system rated power, kW" = "K25"
-"Battery System Parameters, Battery System Configuration and Performance, Target SOC at full power, %" = "K26"
-"Battery System Parameters, Battery System Configuration and Performance, Pulse time at rated power, s" = "K27"
-"Battery System Parameters, Battery System Configuration and Performance, % OCV at rated power (adjusted for thickness limit), %" = "K28"
-"Battery System Parameters, Battery System Configuration and Performance, Cooling system power requirement, W" = "K29"
-
-"Battery System Parameters, Battery System Size, Battery system volume (all packs and cooling), L" = "K32"
-"Battery System Parameters, Battery System Size, Battery system mass (all packs and cooling), kg" = "K33"
-
-"Battery System Parameters, Battery System Metrics, Battery system energy density, Wh/L" = "K36"
-"Battery System Parameters, Battery System Metrics, Battery system specific energy, Wh/kg" = "K37"
-"Battery System Parameters, Battery System Metrics, Battery system useable energy density, Wh(Useable)/L" = "K38"
-"Battery System Parameters, Battery System Metrics, Battery system useable specific energy, Wh(Useable)/kg" = "K39"
-
-"Pack Parameters, Pack Configuration and Performance, Number of cells per pack" = "K43"
-"Pack Parameters, Pack Configuration and Performance, Number of modules per pack" = "K44"
-"Pack Parameters, Pack Configuration and Performance, Pack average OCV, V" = "K45"
-"Pack Parameters, Pack Configuration and Performance, Pack nominal operating voltage, V" = "K46"
-"Pack Parameters, Pack Configuration and Performance, Pack capacity, Ah" = "K47"
-"Pack Parameters, Pack Configuration and Performance, Pack total energy, kWh" = "K48"
-"Pack Parameters, Pack Configuration and Performance, Pack useable energy, kWh(Useable)" = "K49"
-"Pack Parameters, Pack Configuration and Performance, Pack power at target %OCV, kW" = "K50"
-"Pack Parameters, Pack Configuration and Performance, Pack power at rated power, kW" = "K51"
-
-"Pack Parameters, Pack Size, Pack length, mm" = "K54"
-"Pack Parameters, Pack Size, Pack width, mm" = "K55"
-"Pack Parameters, Pack Size, Pack height, mm" = "K56"
-"Pack Parameters, Pack Size, Pack volume, L" = "K57"
-"Pack Parameters, Pack Size, Pack total mass, kg" = "K58"
-
-"Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to power at target %OCV)" = "K61"
-"Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to rated power)" = "K62"
-"Pack Parameters, Pack Metrics, Pack energy density, Wh/L" = "K63"
-"Pack Parameters, Pack Metrics, Pack specific energy, Wh/kg" = "K64"
-"Pack Parameters, Pack Metrics, Pack useable energy density, Wh(Useable)/L" = "K65"
-"Pack Parameters, Pack Metrics, Pack useable specific energy, Wh(Useable)/kg" = "K66"
-
-"Module Parameters, Module Configuration and Performance, Number of cells per module" = "K70"
-"Module Parameters, Module Configuration and Performance, Module average OCV, V" = "K71"
-"Module Parameters, Module Configuration and Performance, Module nominal operating voltage, V" = "K72"
-"Module Parameters, Module Configuration and Performance, Module capacity, Ah" = "K73"
-"Module Parameters, Module Configuration and Performance, Module total energy, kWh" = "K74"
-"Module Parameters, Module Configuration and Performance, Module useable energy, kWh(Useable)" = "K75"
-"Module Parameters, Module Configuration and Performance, Module power at target %OCV, kW" = "K76"
-"Module Parameters, Module Configuration and Performance, Module power at rated power, kW" = "K77"
-
-"Module Parameters, Module Size, Module length, mm" = "K80"
-"Module Parameters, Module Size, Module width, mm" = "K81"
-"Module Parameters, Module Size, Module height, mm" = "K82"
-"Module Parameters, Module Size, Module volume, L" = "K83"
-"Module Parameters, Module Size, Module volume per pack, L" = "K84"
-"Module Parameters, Module Size, Module mass, kg" = "K85"
-"Module Parameters, Module Size, Module mass per pack, kg" = "K86"
-
-"Module Parameters, Module Metrics, Module energy density, Wh/L" = "K89"
-"Module Parameters, Module Metrics, Module specific energy, Wh/kg" = "K90"
-"Module Parameters, Module Metrics, Module useable energy density, Wh(Useable)/L" = "K91"
-"Module Parameters, Module Metrics, Module useable specific energy, Wh(Useable)/kg" = "K92"
-
-"Cell Parameters, Cell Performance, Cell average OCV, V" = "K96"
-"Cell Parameters, Cell Performance, Cell nominal operating voltage, V" = "K97"
-"Cell Parameters, Cell Performance, Cell capacity, Ah" = "K98"
-"Cell Parameters, Cell Performance, Cell total energy, kWh" = "K99"
-"Cell Parameters, Cell Performance, Cell useable energy, kWh(Useable)" = "K100"
-"Cell Parameters, Cell Performance, Cell power at target %OCV, kW" = "K101"
-"Cell Parameters, Cell Performance, Cell power at rated power, kW" = "K102"
-
-"Cell Parameters, Cell Size,Cell length, mm" = "K105"
-"Cell Parameters, Cell Size,Cell width, mm" = "K106"
-"Cell Parameters, Cell Size,Cell thickness, mm" = "K107"
-"Cell Parameters, Cell Size,Cell volume, L" = "K108"
-"Cell Parameters, Cell Size,Cell volume per pack, L" = "K109"
-"Cell Parameters, Cell Size,Cell mass, kg" = "K110"
-"Cell Parameters, Cell Size,Cell mass per pack, kg" = "K111"
-
-"Cell Parameters, Cell Metrics, Cell energy density, Wh/L" = "K114"
-"Cell Parameters, Cell Metrics, Cell specific energy, Wh/kg" = "K115"
-"Cell Parameters, Cell Metrics, Cell useable energy density, Wh(Useable)/L" = "K116"
-"Cell Parameters, Cell Metrics, Cell useable specific energy, Wh(Useable)/kg" = "K117"
-
-"Cell Parameters, Additional Cell Information, Positive electrode thickness, µm" = "K120"
-"Cell Parameters, Additional Cell Information, Negative electrode thickness, µm" = "K121"
-"Cell Parameters, Additional Cell Information, Positive electode areal capacity, mAh/cm²" = "K122"
-"Cell Parameters, Additional Cell Information, Negative electrode areal capacity, mAh/cm²" = "K123"
-
-# Manufacturing Information
-"Plant Size, GWh" = "K128"
-"Packs manufactured at 100% utilization (pack/year)" = "K129"
-"Packs manufactured per year (packs/year)" = "K130"
-"Modules manufactured per year (modules/year)" = "K131"
-"Accepted cells manufactured per year (cells/year)" = "K132"
-
-# Calculated Costs
-"Costs, Battery System, Battery system cost, $" = "K149"
-"Costs, Battery System, Battery system cost, $/kWh" = "K150"
-"Costs, Battery System, Battery system cost, $/kWh(Useable)" = "K151"
-
-"Costs, Pack, Pack cost, $/pack" = "K154"
-"Costs, Pack, Pack cost, $/kWh" = "K155"
-"Costs, Pack, Pack cost, $/kWh(Useable)" = "K156"
-
-"Costs, Module, Module cost, $/module" = "K159"
-"Costs, Module, Module cost per pack, $/pack" = "K160"
-"Costs, Module, Module cost, $/kWh" = "K161"
-"Costs, Module, Module cost, $/kWh(Useable)" = "K162"
-
-"Costs, Cell, Cell cost, $/cell" = "K165"
-"Costs, Cell, Cell cost, $/module" = "K166"
-"Costs, Cell, Cell cost, $/pack" = "K167"
-"Costs, Cell, Cell cost, $/kWh" = "K168"
-"Costs, Cell, Cell cost, $/kWh(Useable)" = "K169"
-
-"Costs, Additional Considerations, Module fraction of pack cost" = "K172"
-"Costs, Additional Considerations, Cell fraction of module cost" = "K173"
-"Costs, Additional Considerations, Cell fraction of pack cost" = "K174"
+    # Calculated Parameters
+    "Battery System Parameters, Battery System Configuration and Performance, Number of battery packs"                                = "K17"
+    "Battery System Parameters, Battery System Configuration and Performance, Packs in series or parallel"                            = "K18"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system average OCV, V"                          = "K19"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system nominal operating voltage, V"            = "K20"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system capacity, Ah"                            = "K21"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system total energy, kWh"                       = "K22"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system useable energy, kWh(Useable)"            = "K23"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system power at target % OCV, kW"               = "K24"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system rated power, kW"                         = "K25"
+    "Battery System Parameters, Battery System Configuration and Performance, Target SOC at full power, %"                            = "K26"
+    "Battery System Parameters, Battery System Configuration and Performance, Pulse time at rated power, s"                           = "K27"
+    "Battery System Parameters, Battery System Configuration and Performance, % OCV at rated power (adjusted for thickness limit), %" = "K28"
+    "Battery System Parameters, Battery System Configuration and Performance, Cooling system power requirement, W"                    = "K29"
+
+    "Battery System Parameters, Battery System Size, Battery system volume (all packs and cooling), L" = "K32"
+    "Battery System Parameters, Battery System Size, Battery system mass (all packs and cooling), kg"  = "K33"
+
+    "Battery System Parameters, Battery System Metrics, Battery system energy density, Wh/L"                    = "K36"
+    "Battery System Parameters, Battery System Metrics, Battery system specific energy, Wh/kg"                  = "K37"
+    "Battery System Parameters, Battery System Metrics, Battery system useable energy density, Wh(Useable)/L"   = "K38"
+    "Battery System Parameters, Battery System Metrics, Battery system useable specific energy, Wh(Useable)/kg" = "K39"
+
+    "Pack Parameters, Pack Configuration and Performance, Number of cells per pack"          = "K43"
+    "Pack Parameters, Pack Configuration and Performance, Number of modules per pack"        = "K44"
+    "Pack Parameters, Pack Configuration and Performance, Pack average OCV, V"               = "K45"
+    "Pack Parameters, Pack Configuration and Performance, Pack nominal operating voltage, V" = "K46"
+    "Pack Parameters, Pack Configuration and Performance, Pack capacity, Ah"                 = "K47"
+    "Pack Parameters, Pack Configuration and Performance, Pack total energy, kWh"            = "K48"
+    "Pack Parameters, Pack Configuration and Performance, Pack useable energy, kWh(Useable)" = "K49"
+    "Pack Parameters, Pack Configuration and Performance, Pack power at target %OCV, kW"     = "K50"
+    "Pack Parameters, Pack Configuration and Performance, Pack power at rated power, kW"     = "K51"
+
+    "Pack Parameters, Pack Size, Pack length, mm"     = "K54"
+    "Pack Parameters, Pack Size, Pack width, mm"      = "K55"
+    "Pack Parameters, Pack Size, Pack height, mm"     = "K56"
+    "Pack Parameters, Pack Size, Pack volume, L"      = "K57"
+    "Pack Parameters, Pack Size, Pack total mass, kg" = "K58"
+
+    "Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to power at target %OCV)" = "K61"
+    "Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to rated power)"          = "K62"
+    "Pack Parameters, Pack Metrics, Pack energy density, Wh/L"                                         = "K63"
+    "Pack Parameters, Pack Metrics, Pack specific energy, Wh/kg"                                       = "K64"
+    "Pack Parameters, Pack Metrics, Pack useable energy density, Wh(Useable)/L"                        = "K65"
+    "Pack Parameters, Pack Metrics, Pack useable specific energy, Wh(Useable)/kg"                      = "K66"
+
+    "Module Parameters, Module Configuration and Performance, Number of cells per module"          = "K70"
+    "Module Parameters, Module Configuration and Performance, Module average OCV, V"               = "K71"
+    "Module Parameters, Module Configuration and Performance, Module nominal operating voltage, V" = "K72"
+    "Module Parameters, Module Configuration and Performance, Module capacity, Ah"                 = "K73"
+    "Module Parameters, Module Configuration and Performance, Module total energy, kWh"            = "K74"
+    "Module Parameters, Module Configuration and Performance, Module useable energy, kWh(Useable)" = "K75"
+    "Module Parameters, Module Configuration and Performance, Module power at target %OCV, kW"     = "K76"
+    "Module Parameters, Module Configuration and Performance, Module power at rated power, kW"     = "K77"
+
+    "Module Parameters, Module Size, Module length, mm"         = "K80"
+    "Module Parameters, Module Size, Module width, mm"          = "K81"
+    "Module Parameters, Module Size, Module height, mm"         = "K82"
+    "Module Parameters, Module Size, Module volume, L"          = "K83"
+    "Module Parameters, Module Size, Module volume per pack, L" = "K84"
+    "Module Parameters, Module Size, Module mass, kg"           = "K85"
+    "Module Parameters, Module Size, Module mass per pack, kg"  = "K86"
+
+    "Module Parameters, Module Metrics, Module energy density, Wh/L"                    = "K89"
+    "Module Parameters, Module Metrics, Module specific energy, Wh/kg"                  = "K90"
+    "Module Parameters, Module Metrics, Module useable energy density, Wh(Useable)/L"   = "K91"
+    "Module Parameters, Module Metrics, Module useable specific energy, Wh(Useable)/kg" = "K92"
+
+    "Cell Parameters, Cell Performance, Cell average OCV, V"               = "K96"
+    "Cell Parameters, Cell Performance, Cell nominal operating voltage, V" = "K97"
+    "Cell Parameters, Cell Performance, Cell capacity, Ah"                 = "K98"
+    "Cell Parameters, Cell Performance, Cell total energy, kWh"            = "K99"
+    "Cell Parameters, Cell Performance, Cell useable energy, kWh(Useable)" = "K100"
+    "Cell Parameters, Cell Performance, Cell power at target %OCV, kW"     = "K101"
+    "Cell Parameters, Cell Performance, Cell power at rated power, kW"     = "K102"
+
+    "Cell Parameters, Cell Size,Cell length, mm"         = "K105"
+    "Cell Parameters, Cell Size,Cell width, mm"          = "K106"
+    "Cell Parameters, Cell Size,Cell thickness, mm"      = "K107"
+    "Cell Parameters, Cell Size,Cell volume, L"          = "K108"
+    "Cell Parameters, Cell Size,Cell volume per pack, L" = "K109"
+    "Cell Parameters, Cell Size,Cell mass, kg"           = "K110"
+    "Cell Parameters, Cell Size,Cell mass per pack, kg"  = "K111"
+
+    "Cell Parameters, Cell Metrics, Cell energy density, Wh/L"                    = "K114"
+    "Cell Parameters, Cell Metrics, Cell specific energy, Wh/kg"                  = "K115"
+    "Cell Parameters, Cell Metrics, Cell useable energy density, Wh(Useable)/L"   = "K116"
+    "Cell Parameters, Cell Metrics, Cell useable specific energy, Wh(Useable)/kg" = "K117"
+
+    "Cell Parameters, Additional Cell Information, Positive electrode thickness, µm"           = "K120"
+    "Cell Parameters, Additional Cell Information, Negative electrode thickness, µm"           = "K121"
+    "Cell Parameters, Additional Cell Information, Positive electode areal capacity, mAh/cm²"  = "K122"
+    "Cell Parameters, Additional Cell Information, Negative electrode areal capacity, mAh/cm²" = "K123"
+
+    # Manufacturing Information
+    "Plant Size, GWh"                                    = "K128"
+    "Packs manufactured at 100% utilization (pack/year)" = "K129"
+    "Packs manufactured per year (packs/year)"           = "K130"
+    "Modules manufactured per year (modules/year)"       = "K131"
+    "Accepted cells manufactured per year (cells/year)"  = "K132"
+
+    # Calculated Costs
+    "Costs, Battery System, Battery system cost, $"              = "K149"
+    "Costs, Battery System, Battery system cost, $/kWh"          = "K150"
+    "Costs, Battery System, Battery system cost, $/kWh(Useable)" = "K151"
+
+    "Costs, Pack, Pack cost, $/pack"         = "K154"
+    "Costs, Pack, Pack cost, $/kWh"          = "K155"
+    "Costs, Pack, Pack cost, $/kWh(Useable)" = "K156"
+
+    "Costs, Module, Module cost, $/module"        = "K159"
+    "Costs, Module, Module cost per pack, $/pack" = "K160"
+    "Costs, Module, Module cost, $/kWh"           = "K161"
+    "Costs, Module, Module cost, $/kWh(Useable)"  = "K162"
+
+    "Costs, Cell, Cell cost, $/cell"         = "K165"
+    "Costs, Cell, Cell cost, $/module"       = "K166"
+    "Costs, Cell, Cell cost, $/pack"         = "K167"
+    "Costs, Cell, Cell cost, $/kWh"          = "K168"
+    "Costs, Cell, Cell cost, $/kWh(Useable)" = "K169"
+
+    "Costs, Additional Considerations, Module fraction of pack cost" = "K172"
+    "Costs, Additional Considerations, Cell fraction of module cost" = "K173"
+    "Costs, Additional Considerations, Cell fraction of pack cost"   = "K174"
 
 ["Summary of Results"."Battery 6"]
-# Calculated Parameters
-"Battery System Parameters, Battery System Configuration and Performance, Number of battery packs" = "L17"
-"Battery System Parameters, Battery System Configuration and Performance, Packs in series or parallel" = "L18"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system average OCV, V" = "L19"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system nominal operating voltage, V" = "L20"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system capacity, Ah" = "L21"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system total energy, kWh" = "L22"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system useable energy, kWh(Useable)" = "L23"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system power at target % OCV, kW" = "L24"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system rated power, kW" = "L25"
-"Battery System Parameters, Battery System Configuration and Performance, Target SOC at full power, %" = "L26"
-"Battery System Parameters, Battery System Configuration and Performance, Pulse time at rated power, s" = "L27"
-"Battery System Parameters, Battery System Configuration and Performance, % OCV at rated power (adjusted for thickness limit), %" = "L28"
-"Battery System Parameters, Battery System Configuration and Performance, Cooling system power requirement, W" = "L29"
-
-"Battery System Parameters, Battery System Size, Battery system volume (all packs and cooling), L" = "L32"
-"Battery System Parameters, Battery System Size, Battery system mass (all packs and cooling), kg" = "L33"
-
-"Battery System Parameters, Battery System Metrics, Battery system energy density, Wh/L" = "L36"
-"Battery System Parameters, Battery System Metrics, Battery system specific energy, Wh/kg" = "L37"
-"Battery System Parameters, Battery System Metrics, Battery system useable energy density, Wh(Useable)/L" = "L38"
-"Battery System Parameters, Battery System Metrics, Battery system useable specific energy, Wh(Useable)/kg" = "L39"
-
-"Pack Parameters, Pack Configuration and Performance, Number of cells per pack" = "L43"
-"Pack Parameters, Pack Configuration and Performance, Number of modules per pack" = "L44"
-"Pack Parameters, Pack Configuration and Performance, Pack average OCV, V" = "L45"
-"Pack Parameters, Pack Configuration and Performance, Pack nominal operating voltage, V" = "L46"
-"Pack Parameters, Pack Configuration and Performance, Pack capacity, Ah" = "L47"
-"Pack Parameters, Pack Configuration and Performance, Pack total energy, kWh" = "L48"
-"Pack Parameters, Pack Configuration and Performance, Pack useable energy, kWh(Useable)" = "L49"
-"Pack Parameters, Pack Configuration and Performance, Pack power at target %OCV, kW" = "L50"
-"Pack Parameters, Pack Configuration and Performance, Pack power at rated power, kW" = "L51"
-
-"Pack Parameters, Pack Size, Pack length, mm" = "L54"
-"Pack Parameters, Pack Size, Pack width, mm" = "L55"
-"Pack Parameters, Pack Size, Pack height, mm" = "L56"
-"Pack Parameters, Pack Size, Pack volume, L" = "L57"
-"Pack Parameters, Pack Size, Pack total mass, kg" = "L58"
-
-"Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to power at target %OCV)" = "L61"
-"Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to rated power)" = "L62"
-"Pack Parameters, Pack Metrics, Pack energy density, Wh/L" = "L63"
-"Pack Parameters, Pack Metrics, Pack specific energy, Wh/kg" = "L64"
-"Pack Parameters, Pack Metrics, Pack useable energy density, Wh(Useable)/L" = "L65"
-"Pack Parameters, Pack Metrics, Pack useable specific energy, Wh(Useable)/kg" = "L66"
-
-"Module Parameters, Module Configuration and Performance, Number of cells per module" = "L70"
-"Module Parameters, Module Configuration and Performance, Module average OCV, V" = "L71"
-"Module Parameters, Module Configuration and Performance, Module nominal operating voltage, V" = "L72"
-"Module Parameters, Module Configuration and Performance, Module capacity, Ah" = "L73"
-"Module Parameters, Module Configuration and Performance, Module total energy, kWh" = "L74"
-"Module Parameters, Module Configuration and Performance, Module useable energy, kWh(Useable)" = "L75"
-"Module Parameters, Module Configuration and Performance, Module power at target %OCV, kW" = "L76"
-"Module Parameters, Module Configuration and Performance, Module power at rated power, kW" = "L77"
-
-"Module Parameters, Module Size, Module length, mm" = "L80"
-"Module Parameters, Module Size, Module width, mm" = "L81"
-"Module Parameters, Module Size, Module height, mm" = "L82"
-"Module Parameters, Module Size, Module volume, L" = "L83"
-"Module Parameters, Module Size, Module volume per pack, L" = "L84"
-"Module Parameters, Module Size, Module mass, kg" = "L85"
-"Module Parameters, Module Size, Module mass per pack, kg" = "L86"
-
-"Module Parameters, Module Metrics, Module energy density, Wh/L" = "L89"
-"Module Parameters, Module Metrics, Module specific energy, Wh/kg" = "L90"
-"Module Parameters, Module Metrics, Module useable energy density, Wh(Useable)/L" = "L91"
-"Module Parameters, Module Metrics, Module useable specific energy, Wh(Useable)/kg" = "L92"
-
-"Cell Parameters, Cell Performance, Cell average OCV, V" = "L96"
-"Cell Parameters, Cell Performance, Cell nominal operating voltage, V" = "L97"
-"Cell Parameters, Cell Performance, Cell capacity, Ah" = "L98"
-"Cell Parameters, Cell Performance, Cell total energy, kWh" = "L99"
-"Cell Parameters, Cell Performance, Cell useable energy, kWh(Useable)" = "L100"
-"Cell Parameters, Cell Performance, Cell power at target %OCV, kW" = "L101"
-"Cell Parameters, Cell Performance, Cell power at rated power, kW" = "L102"
-
-"Cell Parameters, Cell Size,Cell length, mm" = "L105"
-"Cell Parameters, Cell Size,Cell width, mm" = "L106"
-"Cell Parameters, Cell Size,Cell thickness, mm" = "L107"
-"Cell Parameters, Cell Size,Cell volume, L" = "L108"
-"Cell Parameters, Cell Size,Cell volume per pack, L" = "L109"
-"Cell Parameters, Cell Size,Cell mass, kg" = "L110"
-"Cell Parameters, Cell Size,Cell mass per pack, kg" = "L111"
-
-"Cell Parameters, Cell Metrics, Cell energy density, Wh/L" = "L114"
-"Cell Parameters, Cell Metrics, Cell specific energy, Wh/kg" = "L115"
-"Cell Parameters, Cell Metrics, Cell useable energy density, Wh(Useable)/L" = "L116"
-"Cell Parameters, Cell Metrics, Cell useable specific energy, Wh(Useable)/kg" = "L117"
-
-"Cell Parameters, Additional Cell Information, Positive electrode thickness, µm" = "L120"
-"Cell Parameters, Additional Cell Information, Negative electrode thickness, µm" = "L121"
-"Cell Parameters, Additional Cell Information, Positive electode areal capacity, mAh/cm²" = "L122"
-"Cell Parameters, Additional Cell Information, Negative electrode areal capacity, mAh/cm²" = "L123"
-
-# Manufacturing Information
-"Plant Size, GWh" = "L128"
-"Packs manufactured at 100% utilization (pack/year)" = "L129"
-"Packs manufactured per year (packs/year)" = "L130"
-"Modules manufactured per year (modules/year)" = "L131"
-"Accepted cells manufactured per year (cells/year)" = "L132"
-
-# Calculated Costs
-"Costs, Battery System, Battery system cost, $" = "L149"
-"Costs, Battery System, Battery system cost, $/kWh" = "L150"
-"Costs, Battery System, Battery system cost, $/kWh(Useable)" = "L151"
-
-"Costs, Pack, Pack cost, $/pack" = "L154"
-"Costs, Pack, Pack cost, $/kWh" = "L155"
-"Costs, Pack, Pack cost, $/kWh(Useable)" = "L156"
-
-"Costs, Module, Module cost, $/module" = "L159"
-"Costs, Module, Module cost per pack, $/pack" = "L160"
-"Costs, Module, Module cost, $/kWh" = "L161"
-"Costs, Module, Module cost, $/kWh(Useable)" = "L162"
-
-"Costs, Cell, Cell cost, $/cell" = "L165"
-"Costs, Cell, Cell cost, $/module" = "L166"
-"Costs, Cell, Cell cost, $/pack" = "L167"
-"Costs, Cell, Cell cost, $/kWh" = "L168"
-"Costs, Cell, Cell cost, $/kWh(Useable)" = "L169"
-
-"Costs, Additional Considerations, Module fraction of pack cost" = "L172"
-"Costs, Additional Considerations, Cell fraction of module cost" = "L173"
-"Costs, Additional Considerations, Cell fraction of pack cost" = "L174"
+    # Calculated Parameters
+    "Battery System Parameters, Battery System Configuration and Performance, Number of battery packs"                                = "L17"
+    "Battery System Parameters, Battery System Configuration and Performance, Packs in series or parallel"                            = "L18"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system average OCV, V"                          = "L19"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system nominal operating voltage, V"            = "L20"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system capacity, Ah"                            = "L21"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system total energy, kWh"                       = "L22"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system useable energy, kWh(Useable)"            = "L23"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system power at target % OCV, kW"               = "L24"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system rated power, kW"                         = "L25"
+    "Battery System Parameters, Battery System Configuration and Performance, Target SOC at full power, %"                            = "L26"
+    "Battery System Parameters, Battery System Configuration and Performance, Pulse time at rated power, s"                           = "L27"
+    "Battery System Parameters, Battery System Configuration and Performance, % OCV at rated power (adjusted for thickness limit), %" = "L28"
+    "Battery System Parameters, Battery System Configuration and Performance, Cooling system power requirement, W"                    = "L29"
+
+    "Battery System Parameters, Battery System Size, Battery system volume (all packs and cooling), L" = "L32"
+    "Battery System Parameters, Battery System Size, Battery system mass (all packs and cooling), kg"  = "L33"
+
+    "Battery System Parameters, Battery System Metrics, Battery system energy density, Wh/L"                    = "L36"
+    "Battery System Parameters, Battery System Metrics, Battery system specific energy, Wh/kg"                  = "L37"
+    "Battery System Parameters, Battery System Metrics, Battery system useable energy density, Wh(Useable)/L"   = "L38"
+    "Battery System Parameters, Battery System Metrics, Battery system useable specific energy, Wh(Useable)/kg" = "L39"
+
+    "Pack Parameters, Pack Configuration and Performance, Number of cells per pack"          = "L43"
+    "Pack Parameters, Pack Configuration and Performance, Number of modules per pack"        = "L44"
+    "Pack Parameters, Pack Configuration and Performance, Pack average OCV, V"               = "L45"
+    "Pack Parameters, Pack Configuration and Performance, Pack nominal operating voltage, V" = "L46"
+    "Pack Parameters, Pack Configuration and Performance, Pack capacity, Ah"                 = "L47"
+    "Pack Parameters, Pack Configuration and Performance, Pack total energy, kWh"            = "L48"
+    "Pack Parameters, Pack Configuration and Performance, Pack useable energy, kWh(Useable)" = "L49"
+    "Pack Parameters, Pack Configuration and Performance, Pack power at target %OCV, kW"     = "L50"
+    "Pack Parameters, Pack Configuration and Performance, Pack power at rated power, kW"     = "L51"
+
+    "Pack Parameters, Pack Size, Pack length, mm"     = "L54"
+    "Pack Parameters, Pack Size, Pack width, mm"      = "L55"
+    "Pack Parameters, Pack Size, Pack height, mm"     = "L56"
+    "Pack Parameters, Pack Size, Pack volume, L"      = "L57"
+    "Pack Parameters, Pack Size, Pack total mass, kg" = "L58"
+
+    "Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to power at target %OCV)" = "L61"
+    "Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to rated power)"          = "L62"
+    "Pack Parameters, Pack Metrics, Pack energy density, Wh/L"                                         = "L63"
+    "Pack Parameters, Pack Metrics, Pack specific energy, Wh/kg"                                       = "L64"
+    "Pack Parameters, Pack Metrics, Pack useable energy density, Wh(Useable)/L"                        = "L65"
+    "Pack Parameters, Pack Metrics, Pack useable specific energy, Wh(Useable)/kg"                      = "L66"
+
+    "Module Parameters, Module Configuration and Performance, Number of cells per module"          = "L70"
+    "Module Parameters, Module Configuration and Performance, Module average OCV, V"               = "L71"
+    "Module Parameters, Module Configuration and Performance, Module nominal operating voltage, V" = "L72"
+    "Module Parameters, Module Configuration and Performance, Module capacity, Ah"                 = "L73"
+    "Module Parameters, Module Configuration and Performance, Module total energy, kWh"            = "L74"
+    "Module Parameters, Module Configuration and Performance, Module useable energy, kWh(Useable)" = "L75"
+    "Module Parameters, Module Configuration and Performance, Module power at target %OCV, kW"     = "L76"
+    "Module Parameters, Module Configuration and Performance, Module power at rated power, kW"     = "L77"
+
+    "Module Parameters, Module Size, Module length, mm"         = "L80"
+    "Module Parameters, Module Size, Module width, mm"          = "L81"
+    "Module Parameters, Module Size, Module height, mm"         = "L82"
+    "Module Parameters, Module Size, Module volume, L"          = "L83"
+    "Module Parameters, Module Size, Module volume per pack, L" = "L84"
+    "Module Parameters, Module Size, Module mass, kg"           = "L85"
+    "Module Parameters, Module Size, Module mass per pack, kg"  = "L86"
+
+    "Module Parameters, Module Metrics, Module energy density, Wh/L"                    = "L89"
+    "Module Parameters, Module Metrics, Module specific energy, Wh/kg"                  = "L90"
+    "Module Parameters, Module Metrics, Module useable energy density, Wh(Useable)/L"   = "L91"
+    "Module Parameters, Module Metrics, Module useable specific energy, Wh(Useable)/kg" = "L92"
+
+    "Cell Parameters, Cell Performance, Cell average OCV, V"               = "L96"
+    "Cell Parameters, Cell Performance, Cell nominal operating voltage, V" = "L97"
+    "Cell Parameters, Cell Performance, Cell capacity, Ah"                 = "L98"
+    "Cell Parameters, Cell Performance, Cell total energy, kWh"            = "L99"
+    "Cell Parameters, Cell Performance, Cell useable energy, kWh(Useable)" = "L100"
+    "Cell Parameters, Cell Performance, Cell power at target %OCV, kW"     = "L101"
+    "Cell Parameters, Cell Performance, Cell power at rated power, kW"     = "L102"
+
+    "Cell Parameters, Cell Size,Cell length, mm"         = "L105"
+    "Cell Parameters, Cell Size,Cell width, mm"          = "L106"
+    "Cell Parameters, Cell Size,Cell thickness, mm"      = "L107"
+    "Cell Parameters, Cell Size,Cell volume, L"          = "L108"
+    "Cell Parameters, Cell Size,Cell volume per pack, L" = "L109"
+    "Cell Parameters, Cell Size,Cell mass, kg"           = "L110"
+    "Cell Parameters, Cell Size,Cell mass per pack, kg"  = "L111"
+
+    "Cell Parameters, Cell Metrics, Cell energy density, Wh/L"                    = "L114"
+    "Cell Parameters, Cell Metrics, Cell specific energy, Wh/kg"                  = "L115"
+    "Cell Parameters, Cell Metrics, Cell useable energy density, Wh(Useable)/L"   = "L116"
+    "Cell Parameters, Cell Metrics, Cell useable specific energy, Wh(Useable)/kg" = "L117"
+
+    "Cell Parameters, Additional Cell Information, Positive electrode thickness, µm"           = "L120"
+    "Cell Parameters, Additional Cell Information, Negative electrode thickness, µm"           = "L121"
+    "Cell Parameters, Additional Cell Information, Positive electode areal capacity, mAh/cm²"  = "L122"
+    "Cell Parameters, Additional Cell Information, Negative electrode areal capacity, mAh/cm²" = "L123"
+
+    # Manufacturing Information
+    "Plant Size, GWh"                                    = "L128"
+    "Packs manufactured at 100% utilization (pack/year)" = "L129"
+    "Packs manufactured per year (packs/year)"           = "L130"
+    "Modules manufactured per year (modules/year)"       = "L131"
+    "Accepted cells manufactured per year (cells/year)"  = "L132"
+
+    # Calculated Costs
+    "Costs, Battery System, Battery system cost, $"              = "L149"
+    "Costs, Battery System, Battery system cost, $/kWh"          = "L150"
+    "Costs, Battery System, Battery system cost, $/kWh(Useable)" = "L151"
+
+    "Costs, Pack, Pack cost, $/pack"         = "L154"
+    "Costs, Pack, Pack cost, $/kWh"          = "L155"
+    "Costs, Pack, Pack cost, $/kWh(Useable)" = "L156"
+
+    "Costs, Module, Module cost, $/module"        = "L159"
+    "Costs, Module, Module cost per pack, $/pack" = "L160"
+    "Costs, Module, Module cost, $/kWh"           = "L161"
+    "Costs, Module, Module cost, $/kWh(Useable)"  = "L162"
+
+    "Costs, Cell, Cell cost, $/cell"         = "L165"
+    "Costs, Cell, Cell cost, $/module"       = "L166"
+    "Costs, Cell, Cell cost, $/pack"         = "L167"
+    "Costs, Cell, Cell cost, $/kWh"          = "L168"
+    "Costs, Cell, Cell cost, $/kWh(Useable)" = "L169"
+
+    "Costs, Additional Considerations, Module fraction of pack cost" = "L172"
+    "Costs, Additional Considerations, Cell fraction of module cost" = "L173"
+    "Costs, Additional Considerations, Cell fraction of pack cost"   = "L174"
 
 ["Summary of Results"."Battery 7"]
-# Calculated Parameters
-"Battery System Parameters, Battery System Configuration and Performance, Number of battery packs" = "M17"
-"Battery System Parameters, Battery System Configuration and Performance, Packs in series or parallel" = "M18"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system average OCV, V" = "M19"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system nominal operating voltage, V" = "M20"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system capacity, Ah" = "M21"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system total energy, kWh" = "M22"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system useable energy, kWh(Useable)" = "M23"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system power at target % OCV, kW" = "M24"
-"Battery System Parameters, Battery System Configuration and Performance, Battery system rated power, kW" = "M25"
-"Battery System Parameters, Battery System Configuration and Performance, Target SOC at full power, %" = "M26"
-"Battery System Parameters, Battery System Configuration and Performance, Pulse time at rated power, s" = "M27"
-"Battery System Parameters, Battery System Configuration and Performance, % OCV at rated power (adjusted for thickness limit), %" = "M28"
-"Battery System Parameters, Battery System Configuration and Performance, Cooling system power requirement, W" = "M29"
-
-"Battery System Parameters, Battery System Size, Battery system volume (all packs and cooling), L" = "M32"
-"Battery System Parameters, Battery System Size, Battery system mass (all packs and cooling), kg" = "M33"
-
-"Battery System Parameters, Battery System Metrics, Battery system energy density, Wh/L" = "M36"
-"Battery System Parameters, Battery System Metrics, Battery system specific energy, Wh/kg" = "M37"
-"Battery System Parameters, Battery System Metrics, Battery system useable energy density, Wh(Useable)/L" = "M38"
-"Battery System Parameters, Battery System Metrics, Battery system useable specific energy, Wh(Useable)/kg" = "M39"
-
-"Pack Parameters, Pack Configuration and Performance, Number of cells per pack" = "M43"
-"Pack Parameters, Pack Configuration and Performance, Number of modules per pack" = "M44"
-"Pack Parameters, Pack Configuration and Performance, Pack average OCV, V" = "M45"
-"Pack Parameters, Pack Configuration and Performance, Pack nominal operating voltage, V" = "M46"
-"Pack Parameters, Pack Configuration and Performance, Pack capacity, Ah" = "M47"
-"Pack Parameters, Pack Configuration and Performance, Pack total energy, kWh" = "M48"
-"Pack Parameters, Pack Configuration and Performance, Pack useable energy, kWh(Useable)" = "M49"
-"Pack Parameters, Pack Configuration and Performance, Pack power at target %OCV, kW" = "M50"
-"Pack Parameters, Pack Configuration and Performance, Pack power at rated power, kW" = "M51"
-
-"Pack Parameters, Pack Size, Pack length, mm" = "M54"
-"Pack Parameters, Pack Size, Pack width, mm" = "M55"
-"Pack Parameters, Pack Size, Pack height, mm" = "M56"
-"Pack Parameters, Pack Size, Pack volume, L" = "M57"
-"Pack Parameters, Pack Size, Pack total mass, kg" = "M58"
-
-"Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to power at target %OCV)" = "M61"
-"Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to rated power)" = "M62"
-"Pack Parameters, Pack Metrics, Pack energy density, Wh/L" = "M63"
-"Pack Parameters, Pack Metrics, Pack specific energy, Wh/kg" = "M64"
-"Pack Parameters, Pack Metrics, Pack useable energy density, Wh(Useable)/L" = "M65"
-"Pack Parameters, Pack Metrics, Pack useable specific energy, Wh(Useable)/kg" = "M66"
-
-"Module Parameters, Module Configuration and Performance, Number of cells per module" = "M70"
-"Module Parameters, Module Configuration and Performance, Module average OCV, V" = "M71"
-"Module Parameters, Module Configuration and Performance, Module nominal operating voltage, V" = "M72"
-"Module Parameters, Module Configuration and Performance, Module capacity, Ah" = "M73"
-"Module Parameters, Module Configuration and Performance, Module total energy, kWh" = "M74"
-"Module Parameters, Module Configuration and Performance, Module useable energy, kWh(Useable)" = "M75"
-"Module Parameters, Module Configuration and Performance, Module power at target %OCV, kW" = "M76"
-"Module Parameters, Module Configuration and Performance, Module power at rated power, kW" = "M77"
-
-"Module Parameters, Module Size, Module length, mm" = "M80"
-"Module Parameters, Module Size, Module width, mm" = "M81"
-"Module Parameters, Module Size, Module height, mm" = "M82"
-"Module Parameters, Module Size, Module volume, L" = "M83"
-"Module Parameters, Module Size, Module volume per pack, L" = "M84"
-"Module Parameters, Module Size, Module mass, kg" = "M85"
-"Module Parameters, Module Size, Module mass per pack, kg" = "M86"
-
-"Module Parameters, Module Metrics, Module energy density, Wh/L" = "M89"
-"Module Parameters, Module Metrics, Module specific energy, Wh/kg" = "M90"
-"Module Parameters, Module Metrics, Module useable energy density, Wh(Useable)/L" = "M91"
-"Module Parameters, Module Metrics, Module useable specific energy, Wh(Useable)/kg" = "M92"
-
-"Cell Parameters, Cell Performance, Cell average OCV, V" = "M96"
-"Cell Parameters, Cell Performance, Cell nominal operating voltage, V" = "M97"
-"Cell Parameters, Cell Performance, Cell capacity, Ah" = "M98"
-"Cell Parameters, Cell Performance, Cell total energy, kWh" = "M99"
-"Cell Parameters, Cell Performance, Cell useable energy, kWh(Useable)" = "M100"
-"Cell Parameters, Cell Performance, Cell power at target %OCV, kW" = "M101"
-"Cell Parameters, Cell Performance, Cell power at rated power, kW" = "M102"
-
-"Cell Parameters, Cell Size,Cell length, mm" = "M105"
-"Cell Parameters, Cell Size,Cell width, mm" = "M106"
-"Cell Parameters, Cell Size,Cell thickness, mm" = "M107"
-"Cell Parameters, Cell Size,Cell volume, L" = "M108"
-"Cell Parameters, Cell Size,Cell volume per pack, L" = "M109"
-"Cell Parameters, Cell Size,Cell mass, kg" = "M110"
-"Cell Parameters, Cell Size,Cell mass per pack, kg" = "M111"
-
-"Cell Parameters, Cell Metrics, Cell energy density, Wh/L" = "M114"
-"Cell Parameters, Cell Metrics, Cell specific energy, Wh/kg" = "M115"
-"Cell Parameters, Cell Metrics, Cell useable energy density, Wh(Useable)/L" = "M116"
-"Cell Parameters, Cell Metrics, Cell useable specific energy, Wh(Useable)/kg" = "M117"
-
-"Cell Parameters, Additional Cell Information, Positive electrode thickness, µm" = "M120"
-"Cell Parameters, Additional Cell Information, Negative electrode thickness, µm" = "M121"
-"Cell Parameters, Additional Cell Information, Positive electode areal capacity, mAh/cm²" = "M122"
-"Cell Parameters, Additional Cell Information, Negative electrode areal capacity, mAh/cm²" = "M123"
-
-# Manufacturing Information
-"Plant Size, GWh" = "M128"
-"Packs manufactured at 100% utilization (pack/year)" = "M129"
-"Packs manufactured per year (packs/year)" = "M130"
-"Modules manufactured per year (modules/year)" = "M131"
-"Accepted cells manufactured per year (cells/year)" = "M132"
-
-# Calculated Costs
-"Costs, Battery System, Battery system cost, $" = "M149"
-"Costs, Battery System, Battery system cost, $/kWh" = "M150"
-"Costs, Battery System, Battery system cost, $/kWh(Useable)" = "M151"
-
-"Costs, Pack, Pack cost, $/pack" = "M154"
-"Costs, Pack, Pack cost, $/kWh" = "M155"
-"Costs, Pack, Pack cost, $/kWh(Useable)" = "M156"
-
-"Costs, Module, Module cost, $/module" = "M159"
-"Costs, Module, Module cost per pack, $/pack" = "M160"
-"Costs, Module, Module cost, $/kWh" = "M161"
-"Costs, Module, Module cost, $/kWh(Useable)" = "M162"
-
-"Costs, Cell, Cell cost, $/cell" = "M165"
-"Costs, Cell, Cell cost, $/module" = "M166"
-"Costs, Cell, Cell cost, $/pack" = "M167"
-"Costs, Cell, Cell cost, $/kWh" = "M168"
-"Costs, Cell, Cell cost, $/kWh(Useable)" = "M169"
-
-"Costs, Additional Considerations, Module fraction of pack cost" = "M172"
-"Costs, Additional Considerations, Cell fraction of module cost" = "M173"
-"Costs, Additional Considerations, Cell fraction of pack cost" = "M174"
+    # Calculated Parameters
+    "Battery System Parameters, Battery System Configuration and Performance, Number of battery packs"                                = "M17"
+    "Battery System Parameters, Battery System Configuration and Performance, Packs in series or parallel"                            = "M18"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system average OCV, V"                          = "M19"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system nominal operating voltage, V"            = "M20"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system capacity, Ah"                            = "M21"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system total energy, kWh"                       = "M22"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system useable energy, kWh(Useable)"            = "M23"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system power at target % OCV, kW"               = "M24"
+    "Battery System Parameters, Battery System Configuration and Performance, Battery system rated power, kW"                         = "M25"
+    "Battery System Parameters, Battery System Configuration and Performance, Target SOC at full power, %"                            = "M26"
+    "Battery System Parameters, Battery System Configuration and Performance, Pulse time at rated power, s"                           = "M27"
+    "Battery System Parameters, Battery System Configuration and Performance, % OCV at rated power (adjusted for thickness limit), %" = "M28"
+    "Battery System Parameters, Battery System Configuration and Performance, Cooling system power requirement, W"                    = "M29"
+
+    "Battery System Parameters, Battery System Size, Battery system volume (all packs and cooling), L" = "M32"
+    "Battery System Parameters, Battery System Size, Battery system mass (all packs and cooling), kg"  = "M33"
+
+    "Battery System Parameters, Battery System Metrics, Battery system energy density, Wh/L"                    = "M36"
+    "Battery System Parameters, Battery System Metrics, Battery system specific energy, Wh/kg"                  = "M37"
+    "Battery System Parameters, Battery System Metrics, Battery system useable energy density, Wh(Useable)/L"   = "M38"
+    "Battery System Parameters, Battery System Metrics, Battery system useable specific energy, Wh(Useable)/kg" = "M39"
+
+    "Pack Parameters, Pack Configuration and Performance, Number of cells per pack"          = "M43"
+    "Pack Parameters, Pack Configuration and Performance, Number of modules per pack"        = "M44"
+    "Pack Parameters, Pack Configuration and Performance, Pack average OCV, V"               = "M45"
+    "Pack Parameters, Pack Configuration and Performance, Pack nominal operating voltage, V" = "M46"
+    "Pack Parameters, Pack Configuration and Performance, Pack capacity, Ah"                 = "M47"
+    "Pack Parameters, Pack Configuration and Performance, Pack total energy, kWh"            = "M48"
+    "Pack Parameters, Pack Configuration and Performance, Pack useable energy, kWh(Useable)" = "M49"
+    "Pack Parameters, Pack Configuration and Performance, Pack power at target %OCV, kW"     = "M50"
+    "Pack Parameters, Pack Configuration and Performance, Pack power at rated power, kW"     = "M51"
+
+    "Pack Parameters, Pack Size, Pack length, mm"     = "M54"
+    "Pack Parameters, Pack Size, Pack width, mm"      = "M55"
+    "Pack Parameters, Pack Size, Pack height, mm"     = "M56"
+    "Pack Parameters, Pack Size, Pack volume, L"      = "M57"
+    "Pack Parameters, Pack Size, Pack total mass, kg" = "M58"
+
+    "Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to power at target %OCV)" = "M61"
+    "Pack Parameters, Pack Metrics, Pack power to energy ratio (with respect to rated power)"          = "M62"
+    "Pack Parameters, Pack Metrics, Pack energy density, Wh/L"                                         = "M63"
+    "Pack Parameters, Pack Metrics, Pack specific energy, Wh/kg"                                       = "M64"
+    "Pack Parameters, Pack Metrics, Pack useable energy density, Wh(Useable)/L"                        = "M65"
+    "Pack Parameters, Pack Metrics, Pack useable specific energy, Wh(Useable)/kg"                      = "M66"
+
+    "Module Parameters, Module Configuration and Performance, Number of cells per module"          = "M70"
+    "Module Parameters, Module Configuration and Performance, Module average OCV, V"               = "M71"
+    "Module Parameters, Module Configuration and Performance, Module nominal operating voltage, V" = "M72"
+    "Module Parameters, Module Configuration and Performance, Module capacity, Ah"                 = "M73"
+    "Module Parameters, Module Configuration and Performance, Module total energy, kWh"            = "M74"
+    "Module Parameters, Module Configuration and Performance, Module useable energy, kWh(Useable)" = "M75"
+    "Module Parameters, Module Configuration and Performance, Module power at target %OCV, kW"     = "M76"
+    "Module Parameters, Module Configuration and Performance, Module power at rated power, kW"     = "M77"
+
+    "Module Parameters, Module Size, Module length, mm"         = "M80"
+    "Module Parameters, Module Size, Module width, mm"          = "M81"
+    "Module Parameters, Module Size, Module height, mm"         = "M82"
+    "Module Parameters, Module Size, Module volume, L"          = "M83"
+    "Module Parameters, Module Size, Module volume per pack, L" = "M84"
+    "Module Parameters, Module Size, Module mass, kg"           = "M85"
+    "Module Parameters, Module Size, Module mass per pack, kg"  = "M86"
+
+    "Module Parameters, Module Metrics, Module energy density, Wh/L"                    = "M89"
+    "Module Parameters, Module Metrics, Module specific energy, Wh/kg"                  = "M90"
+    "Module Parameters, Module Metrics, Module useable energy density, Wh(Useable)/L"   = "M91"
+    "Module Parameters, Module Metrics, Module useable specific energy, Wh(Useable)/kg" = "M92"
+
+    "Cell Parameters, Cell Performance, Cell average OCV, V"               = "M96"
+    "Cell Parameters, Cell Performance, Cell nominal operating voltage, V" = "M97"
+    "Cell Parameters, Cell Performance, Cell capacity, Ah"                 = "M98"
+    "Cell Parameters, Cell Performance, Cell total energy, kWh"            = "M99"
+    "Cell Parameters, Cell Performance, Cell useable energy, kWh(Useable)" = "M100"
+    "Cell Parameters, Cell Performance, Cell power at target %OCV, kW"     = "M101"
+    "Cell Parameters, Cell Performance, Cell power at rated power, kW"     = "M102"
+
+    "Cell Parameters, Cell Size,Cell length, mm"         = "M105"
+    "Cell Parameters, Cell Size,Cell width, mm"          = "M106"
+    "Cell Parameters, Cell Size,Cell thickness, mm"      = "M107"
+    "Cell Parameters, Cell Size,Cell volume, L"          = "M108"
+    "Cell Parameters, Cell Size,Cell volume per pack, L" = "M109"
+    "Cell Parameters, Cell Size,Cell mass, kg"           = "M110"
+    "Cell Parameters, Cell Size,Cell mass per pack, kg"  = "M111"
+
+    "Cell Parameters, Cell Metrics, Cell energy density, Wh/L"                    = "M114"
+    "Cell Parameters, Cell Metrics, Cell specific energy, Wh/kg"                  = "M115"
+    "Cell Parameters, Cell Metrics, Cell useable energy density, Wh(Useable)/L"   = "M116"
+    "Cell Parameters, Cell Metrics, Cell useable specific energy, Wh(Useable)/kg" = "M117"
+
+    "Cell Parameters, Additional Cell Information, Positive electrode thickness, µm"           = "M120"
+    "Cell Parameters, Additional Cell Information, Negative electrode thickness, µm"           = "M121"
+    "Cell Parameters, Additional Cell Information, Positive electode areal capacity, mAh/cm²"  = "M122"
+    "Cell Parameters, Additional Cell Information, Negative electrode areal capacity, mAh/cm²" = "M123"
+
+    # Manufacturing Information
+    "Plant Size, GWh"                                    = "M128"
+    "Packs manufactured at 100% utilization (pack/year)" = "M129"
+    "Packs manufactured per year (packs/year)"           = "M130"
+    "Modules manufactured per year (modules/year)"       = "M131"
+    "Accepted cells manufactured per year (cells/year)"  = "M132"
+
+    # Calculated Costs
+    "Costs, Battery System, Battery system cost, $"              = "M149"
+    "Costs, Battery System, Battery system cost, $/kWh"          = "M150"
+    "Costs, Battery System, Battery system cost, $/kWh(Useable)" = "M151"
+
+    "Costs, Pack, Pack cost, $/pack"         = "M154"
+    "Costs, Pack, Pack cost, $/kWh"          = "M155"
+    "Costs, Pack, Pack cost, $/kWh(Useable)" = "M156"
+
+    "Costs, Module, Module cost, $/module"        = "M159"
+    "Costs, Module, Module cost per pack, $/pack" = "M160"
+    "Costs, Module, Module cost, $/kWh"           = "M161"
+    "Costs, Module, Module cost, $/kWh(Useable)"  = "M162"
+
+    "Costs, Cell, Cell cost, $/cell"         = "M165"
+    "Costs, Cell, Cell cost, $/module"       = "M166"
+    "Costs, Cell, Cell cost, $/pack"         = "M167"
+    "Costs, Cell, Cell cost, $/kWh"          = "M168"
+    "Costs, Cell, Cell cost, $/kWh(Useable)" = "M169"
+
+    "Costs, Additional Considerations, Module fraction of pack cost" = "M172"
+    "Costs, Additional Considerations, Cell fraction of module cost" = "M173"
+    "Costs, Additional Considerations, Cell fraction of pack cost"   = "M174"
```

### Comparing `batpy-0.2.0/src/batpy/formula_engine.py` & `batpy-0.3.0/src/batpy/formula_engine.py`

 * *Files identical despite different names*

### Comparing `batpy-0.2.0/src/batpy/utility_functions.py` & `batpy-0.3.0/src/batpy/utility_functions.py`

 * *Files identical despite different names*

