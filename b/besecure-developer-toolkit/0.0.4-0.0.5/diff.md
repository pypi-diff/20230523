# Comparing `tmp/besecure_developer_toolkit-0.0.4.tar.gz` & `tmp/besecure_developer_toolkit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "besecure_developer_toolkit-0.0.4.tar", max compression
+gzip compressed data, was "besecure_developer_toolkit-0.0.5.tar", max compression
```

## Comparing `besecure_developer_toolkit-0.0.4.tar` & `besecure_developer_toolkit-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-04-28 06:27:59.071490 besecure_developer_toolkit-0.0.4/LICENSE
--rw-r--r--   0        0        0     1243 2023-04-28 06:27:59.071490 besecure_developer_toolkit-0.0.4/README.md
--rw-r--r--   0        0        0      340 2023-04-28 06:27:59.071490 besecure_developer_toolkit-0.0.4/besecure_developer_toolkit/__init__.py
--rw-r--r--   0        0        0      203 2023-04-28 06:27:59.071490 besecure_developer_toolkit-0.0.4/besecure_developer_toolkit/__main__.py
--rw-r--r--   0        0        0     5747 2023-04-28 07:52:04.178250 besecure_developer_toolkit-0.0.4/besecure_developer_toolkit/cli.py
--rw-r--r--   0        0        0        0 2023-04-28 06:27:59.071490 besecure_developer_toolkit-0.0.4/besecure_developer_toolkit/config.py
--rw-r--r--   0        0        0     8561 2023-04-28 06:27:59.071490 besecure_developer_toolkit-0.0.4/besecure_developer_toolkit/src/create_ossp_master.py
--rw-r--r--   0        0        0     5204 2023-04-28 06:27:59.071490 besecure_developer_toolkit-0.0.4/besecure_developer_toolkit/src/create_version_data.py
--rw-r--r--   0        0        0     5254 2023-04-28 06:27:59.071490 besecure_developer_toolkit-0.0.4/besecure_developer_toolkit/src/generate_report.py
--rw-r--r--   0        0        0      612 2023-04-28 07:52:34.314499 besecure_developer_toolkit-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1804 1970-01-01 00:00:00.000000 besecure_developer_toolkit-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3127 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/README.md
+-rw-r--r--   0        0        0      341 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/__init__.py
+-rw-r--r--   0        0        0      203 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/__main__.py
+-rw-r--r--   0        0        0     9271 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/cli.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/config.py
+-rw-r--r--   0        0        0     9392 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/create_ossp_master.py
+-rw-r--r--   0        0        0     5720 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/create_version_data.py
+-rw-r--r--   0        0        0     5302 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/generate_report.py
+-rw-r--r--   0        0        0     1662 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/risk_assessment.py
+-rw-r--r--   0        0        0     5254 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/risk_summary/License_compliance.py
+-rw-r--r--   0        0        0      906 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/risk_summary/New_line_char.py
+-rw-r--r--   0        0        0     3185 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/risk_summary/Objective.py
+-rw-r--r--   0        0        0     4467 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/risk_summary/Sbom_report.py
+-rw-r--r--   0        0        0     5310 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/risk_summary/Scorecard_report.py
+-rw-r--r--   0        0        0     7109 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/risk_summary/Static_code_analysis.py
+-rw-r--r--   0        0        0    10043 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/validate_report_file.py
+-rw-r--r--   0        0        0     4644 2023-05-23 08:24:03.030484 besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/validate_version_file.py
+-rw-r--r--   0        0        0      654 2023-05-23 08:24:03.038484 besecure_developer_toolkit-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3773 1970-01-01 00:00:00.000000 besecure_developer_toolkit-0.0.5/PKG-INFO
```

### Comparing `besecure_developer_toolkit-0.0.4/LICENSE` & `besecure_developer_toolkit-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `besecure_developer_toolkit-0.0.4/besecure_developer_toolkit/src/create_ossp_master.py` & `besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/create_ossp_master.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,16 +27,23 @@
 
         Returns:
             bool: True if issue exists and False if otherwise
         """
         url = f"https://api.github.com/repos/Be-Secure/Be-Secure/issues/{issue_id}"
         try:
             response = requests.head(url, timeout=10)
+            if response.status_code == 403:
+                print(f'[red bold]Alert! [yellow]'\
+                    'GitHub API rate limit '\
+                    'exceeded for this system')
+                sys.exit(1)
             return response.status_code < 400
-        except requests.exceptions.RequestException:
+        except requests.exceptions.RequestException as exc:
+            print(response.text)
+            print(exc)
             return False
 
     def check_issue_related_to_project(self):
         """
             Check project name from issue
         """
         url = f'https://api.github.com/repos/Be-Secure/Be-Secure/issues/{self.issue_id}'
@@ -56,16 +63,22 @@
 
         Args:
             name (str): Project name
         """
         url = f"https://api.github.com/repos/Be-Secure/{name}"
         try:
             response = requests.head(url, timeout=10)
+            if response.status_code == 403:
+                print(f'[red bold]Alert! [yellow]'\
+                    'GitHub API rate limit '\
+                    'exceeded for this system')
+                sys.exit(1)
             return response.status_code < 400
-        except requests.exceptions.RequestException:
+        except requests.exceptions.RequestException as exc:
+            print(exc)
             return False
 
     def write_tech_stack(self, bes_id):
         """
             Check the tech Stack of the Project
         """
         url = f"https://api.github.com/repos/Be-Secure/Be-Secure/issues/{str(bes_id)}"
@@ -153,14 +166,21 @@
                     ossp_master_json["items"][i] = data
                     break
         else:
             ossp_master_json["items"].append(data)
         file_pointer.seek(0)
         file_pointer.write(json.dumps(ossp_master_json, indent=4))
         file_pointer.truncate()
+        if overwrite:
+            print("[bold red]Alert! [green]Data for " +
+                f"[yellow]{self.name} [green] in OSSP-Master.json has been overwritten")
+        else:
+            print("[bold red]Alert! [green]Added " +
+                f"[yellow]{self.name} [green]to OSSP-Master.json")
+
 
     def generate_ossp_master(self, overwrite: bool):
         """
             Generate ossp master json report
         """
         if self.check_issue_exists(self.issue_id) is False:
             print("[bold red]Alert! [green]Issue " +
```

### Comparing `besecure_developer_toolkit-0.0.4/besecure_developer_toolkit/src/create_version_data.py` & `besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/create_version_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -85,14 +85,16 @@
             # Fixme
             if original_data[i]["version"] == version_tag:
                 original_data[i] = version_data_new
                 break
         file_pointer.seek(0)
         file_pointer.write(json.dumps(original_data, indent=4))
         file_pointer.truncate()
+        print("[bold red]Alert! [green]Version data for " +
+              f"[yellow]{self.name} {version_tag} [green]has been overwritten")
 
     def generate_version_data(self, overwrite: bool):
         """
             generate version details page in osspoi_datastore
         """
         osspoi_dir = os.environ['OSSPOI_DIR']
         version_data_new = {
@@ -125,18 +127,23 @@
                         print(f"{message} {name}")
                         break
                 if write_flag and not overwrite:
                     original_data.append(version_data_new)
                     file_pointer.seek(0)
                     file_pointer.write(json.dumps(original_data, indent=4))
                     file_pointer.truncate()
+                    print("[bold red]Alert! [green]Appending details for [yellow]{self.name}" +
+                          f"{version_tag} into [yellow] {path}")
                 elif write_flag and overwrite:
                     self.overwrite_version_data(
                         file_pointer, version_data_new, original_data, version_tag)
                 else:
                     pass
         else:
             with open(path, "w", encoding="utf-8") as file:
                 data = []
                 data.append(version_data_new)
                 file.write(json.dumps(data, indent=4))
+                print("[bold red]Alert! [green]Created version details file for" +
+                      f"[yellow] {self.issue_id}-{self.name} "+
+                      f"[green]with version:[yellow]{version_tag}")
         self.cleanup()
```

### Comparing `besecure_developer_toolkit-0.0.4/besecure_developer_toolkit/src/generate_report.py` & `besecure_developer_toolkit-0.0.5/besecure_developer_toolkit/src/generate_report.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,17 +59,18 @@
             path = assessment_dir+'/'+self.name+'/'+self.version+'/sast'
         else:
             path = assessment_dir+'/'+self.name+'/'+self.version+'/'+self.report
         try:
             os.makedirs(path, exist_ok=True)
         except FileExistsError as err:
             print(f"error to create file Error: {err}")
-        f = open(path + '/' + self.name + '-' + self.version +
-                 '-' + self.report + '-report.json', "w", encoding="utf-8")
+        file = f"{path}/{self.name}-{self.version}-{self.report}-report.json"
+        f = open(file, "w", encoding="utf-8")
         f.write(json.dumps(data, indent=4))
+        print(f"[bold red]Alert! [green]Added [yellow]{file}")
 
     def update_version_data(self):
         """
             provide versiondetails for version and read from assessment data store
         """
         osspoi_dir = os.environ['OSSPOI_DIR']
         assessment_dir = os.environ['ASSESSMENT_DIR']
```

### Comparing `besecure_developer_toolkit-0.0.4/pyproject.toml` & `besecure_developer_toolkit-0.0.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [tool.poetry]
 name = "besecure-developer-toolkit"
-version = "0.0.4"
+version = "0.0.5"
 description = "cli tool for generating metadata and assessment report for [BeSLighthouse](https://github.com/Be-Secure/BeSLighthouse)."
 authors = ["asa1997 <arunsureshampadath@gmail.com>"]
 readme = "README.md"
 packages = [{include = "besecure_developer_toolkit"}]
 
 [tool.poetry.scripts]
 bes-dev-kit = "besecure_developer_toolkit.__main__:cli.app"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-typer = {extras = ["all"], version = "^0.7.0"}
+typer = {extras = ["all"], version = "^0.9.0"}
 pytest = "^7.3.0"
-
+requests = "^2.29.0"
+reportlab = "^3.6.8"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
```

