# Comparing `tmp/py-eodms-rapi-1.5.3.tar.gz` & `tmp/py-eodms-rapi-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-eodms-rapi-1.5.3.tar", last modified: Fri Feb 17 19:59:04 2023, max compression
+gzip compressed data, was "py-eodms-rapi-1.5.4.tar", last modified: Tue May 23 19:05:36 2023, max compression
```

## Comparing `py-eodms-rapi-1.5.3.tar` & `py-eodms-rapi-1.5.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-02-17 19:59:04.402149 py-eodms-rapi-1.5.3/
--rw-rw-rw-   0        0        0     1180 2023-02-17 19:07:52.000000 py-eodms-rapi-1.5.3/LICENSE
--rw-rw-rw-   0        0        0     2841 2023-02-17 19:59:04.403129 py-eodms-rapi-1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     2034 2022-06-16 17:33:17.000000 py-eodms-rapi-1.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-02-17 19:59:04.355688 py-eodms-rapi-1.5.3/eodms_rapi/
--rw-rw-rw-   0        0        0      535 2023-02-17 19:08:00.000000 py-eodms-rapi-1.5.3/eodms_rapi/__init__.py
--rw-rw-rw-   0        0        0   126773 2023-02-17 19:08:14.000000 py-eodms-rapi-1.5.3/eodms_rapi/eodms.py
--rw-rw-rw-   0        0        0    24662 2022-10-13 17:59:38.000000 py-eodms-rapi-1.5.3/eodms_rapi/geo.py
-drwxrwxrwx   0        0        0        0 2023-02-17 19:59:04.388064 py-eodms-rapi-1.5.3/py_eodms_rapi.egg-info/
--rw-rw-rw-   0        0        0     2841 2023-02-17 19:59:04.000000 py-eodms-rapi-1.5.3/py_eodms_rapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-02-17 19:59:04.000000 py-eodms-rapi-1.5.3/py_eodms_rapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-17 19:59:04.000000 py-eodms-rapi-1.5.3/py_eodms_rapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-02-17 19:59:04.000000 py-eodms-rapi-1.5.3/py_eodms_rapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-02-17 19:59:04.000000 py-eodms-rapi-1.5.3/py_eodms_rapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      827 2023-02-17 19:59:04.407011 py-eodms-rapi-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1151 2023-02-17 19:07:58.000000 py-eodms-rapi-1.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-17 19:59:04.399129 py-eodms-rapi-1.5.3/test/
--rw-rw-rw-   0        0        0     6987 2022-10-13 18:00:49.000000 py-eodms-rapi-1.5.3/test/test_pyeodmsrapi.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:05:36.478029 py-eodms-rapi-1.5.4/
+-rw-rw-rw-   0        0        0     1180 2023-02-17 19:07:52.000000 py-eodms-rapi-1.5.4/LICENSE
+-rw-rw-rw-   0        0        0     2841 2023-05-23 19:05:36.478029 py-eodms-rapi-1.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2034 2022-06-16 17:33:17.000000 py-eodms-rapi-1.5.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 19:05:36.411837 py-eodms-rapi-1.5.4/eodms_rapi/
+-rw-rw-rw-   0        0        0      535 2023-03-06 20:45:07.000000 py-eodms-rapi-1.5.4/eodms_rapi/__init__.py
+-rw-rw-rw-   0        0        0   130009 2023-05-23 18:55:00.000000 py-eodms-rapi-1.5.4/eodms_rapi/eodms.py
+-rw-rw-rw-   0        0        0    24662 2022-10-13 17:59:38.000000 py-eodms-rapi-1.5.4/eodms_rapi/geo.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:05:36.446720 py-eodms-rapi-1.5.4/py_eodms_rapi.egg-info/
+-rw-rw-rw-   0        0        0     2841 2023-05-23 19:05:35.000000 py-eodms-rapi-1.5.4/py_eodms_rapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-05-23 19:05:35.000000 py-eodms-rapi-1.5.4/py_eodms_rapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 19:05:35.000000 py-eodms-rapi-1.5.4/py_eodms_rapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-23 19:05:35.000000 py-eodms-rapi-1.5.4/py_eodms_rapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-23 19:05:35.000000 py-eodms-rapi-1.5.4/py_eodms_rapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      827 2023-05-23 19:05:36.481042 py-eodms-rapi-1.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     1151 2023-03-06 21:00:57.000000 py-eodms-rapi-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 19:05:36.474722 py-eodms-rapi-1.5.4/test/
+-rw-rw-rw-   0        0        0     6987 2022-10-13 18:00:49.000000 py-eodms-rapi-1.5.4/test/test_pyeodmsrapi.py
```

### Comparing `py-eodms-rapi-1.5.3/LICENSE` & `py-eodms-rapi-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py-eodms-rapi-1.5.3/PKG-INFO` & `py-eodms-rapi-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-eodms-rapi
-Version: 1.5.3
+Version: 1.5.4
 Summary: EODMS RAPI Client is a Python3 package used to access the REST API service provided by the Earth Observation Data Management System (EODMS) from Natural Resources Canada.
 Home-page: https://py-eodms-rapi.readthedocs.io/en/latest/
 Author: Kevin Ballantyne (Natural Resources Canada)
 Author-email: kevin.ballantyne@nrcan-rncan.gc.ca
 License: LICENSE
 Project-URL: Source, https://github.com/eodms-sgdot/py-eodms-rapi
 Project-URL: Bug Tracker, https://github.com/eodms-sgdot/py-eodms-rapi/issues
```

### Comparing `py-eodms-rapi-1.5.3/README.md` & `py-eodms-rapi-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `py-eodms-rapi-1.5.3/eodms_rapi/__init__.py` & `py-eodms-rapi-1.5.4/eodms_rapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __title__ = 'py-eodms-rapi'
 __name__ = 'eodms_rapi'
 __author__ = 'Kevin Ballantyne'
 __copyright__ = 'Copyright (c) His Majesty the King in Right of Canada, ' \
                 'as represented by the Minister of Natural Resources, 2022'
 __license__ = 'MIT License'
 __description__ = 'A Python package to access the EODMS RAPI service.'
-__version__ = '1.5.3'
+__version__ = '1.5.4'
 __maintainer__ = 'Kevin Ballantyne'
 __email__ = 'eodms-sgdot@nrcan-rncan.gc.ca'
 
 from .eodms import EODMSRAPI
 from .eodms import QueryError
 from .geo import EODMSGeo
```

### Comparing `py-eodms-rapi-1.5.3/eodms_rapi/eodms.py` & `py-eodms-rapi-1.5.4/eodms_rapi/eodms.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,14 +165,15 @@
         self.start = datetime.datetime.now()
         self.logger = logger
         self.err_occurred = False
         self.auth_err = False
         self.err_msg = None
         self.order_json = None
         self.show_timestamp = show_timestamp
+        self.msg = ''
 
         self.geo = EODMSGeo(self)
 
         # self._map_fields()
 
         self._header = '| EODMSRAPI | '
 
@@ -258,15 +259,16 @@
                                  'LUTApplied', 'CATALOG_IMAGE.OPEN_DATA',
                                  'RCM.POLARIZATION',
                                  'PRODUCT_FORMAT.FORMAT_NAME_E',
                                  'ARCHIVE_IMAGE.PRODUCT_TYPE', 'RCM.ORBIT_REL',
                                  'RCM.WITHIN_ORBIT_TUBE',
                                  'CATALOG_IMAGE.SEQUENCE_ID',
                                  'RCM.SPECIAL_HANDLING_REQUIRED',
-                                 'RCM.ORBIT_DATA_SOURCE'],
+                                 'RCM.ORBIT_DATA_SOURCE',
+                                 'CATALOG_IMAGE.PUBLIC_GOOD'],
             'RCMScienceData': ['SENSOR_BEAM.SPATIAL_RESOLUTION',
                                'RCM.ORBIT_DIRECTION', 'RCM.INCIDENCE_ANGLE',
                                'RCM.SBEAM', 'RCM.BEAM_MNEMONIC',
                                'CUF_RCM.TR_POL', 'CUF_RCM.REC_POL',
                                'RCM.DOWNLINK_SEGMENT_ID'],
             'SGBAirPhotos': ['ARCHIVE_IMAGE.ORDER_KEY',
                              'FLIGHT_SEGMENT.SCALE', 'ROLL.ROLL_NUMBER',
@@ -439,22 +441,22 @@
                 try:
                     out_date = datetime.datetime.strptime(date, form)
                     if out == 'date':
                         return out_date
                     else:
                         return out_date.strftime(out_form)
                 except ValueError as e:
-                    msg = f"{str(e).capitalize()}. Date will not be included " \
-                          f"in query."
+                    self.msg = f"{str(e).capitalize()}. Date will not be " \
+                        f"included in query."
 
-                    self.log_msg(msg, 'warning')
+                    self.log_msg(self.msg, 'warning')
                     pass
                 except Exception:
-                    msg = traceback.format_exc()
-                    self.log_msg(msg, 'warning')
+                    self.msg = traceback.format_exc()
+                    self.log_msg(self.msg, 'warning')
                     pass
 
     def _convert_field(self, field, collection, field_type='search'):
         """
         Converts a field to either a field name or a field ID, depending on
             the input.
 
@@ -533,16 +535,16 @@
         self.results
         :rtype:  list
         """
 
         metadata_fields = self._get_meta_keys()
 
         if isinstance(metadata_fields, QueryError):
-            msg = "Could not generate metadata for the results."
-            self.log_msg(msg, 'warning')
+            self.msg = "Could not generate metadata for the results."
+            self.log_msg(self.msg, 'warning')
             return None
 
         if isinstance(self.results, dict):
             self.results = [self.results]
 
         if show_progress:
             n_urls = len(self.results)
@@ -854,26 +856,44 @@
 
         :return: The complete OR statement for the list of values.
         :rtype: str
         """
 
         if d_type == 'String':
             or_query = '%s' % ' OR '.join([f"{field_id}{op}'{v}'"
-                                           for v in values])
+                                           for v in values if not v == ''])
+        elif d_type == 'Boolean':
+            vals_str = []
+            for v in values:
+                
+                if v == '': continue
+                
+                val_query = None
+                if v[0].lower().find('t') > -1 \
+                    or v[0].lower().find('y') > -1:
+                    val_query = f"{field_id}{op}True"
+                elif v[0].lower().find('f') > -1 \
+                    or v[0].lower().find('n') > -1:
+                    val_query = f"{field_id}{op}False"
+                
+                if val_query is None: continue
+
+                vals_str.append(val_query)
+            or_query = '%s' % ' OR '.join(vals_str)
         elif d_type == 'DateTimeRange':
             date_vals = []
             for val in values:
                 date = dateutil.parser.parse(val)
                 iso_date = date.isoformat()
                 date_vals.append(iso_date)
             or_query = '%s' % ' OR '.join([f"{field_id}{op}'{v}'"
                                            for v in date_vals])
         else:
             or_query = '%s' % ' OR '.join([f"{field_id}{op}{v}"
-                                           for v in values])
+                                           for v in values if not v == ''])
 
         return or_query
 
     def log_msg(self, messages, msg_type='info', log_indent='', out_indent=''):
         """
         Logs a message to the logger.
 
@@ -1096,17 +1116,17 @@
             for idx, f in enumerate(feats):
                 op = f[0].upper()
                 src = f[1]
 
                 self.geoms = self.geo.add_geom(src)
 
                 if self.geoms is None or isinstance(self.geoms, SyntaxError):
-                    msg = f"Geometry feature #{str(idx + 1)} could not be " \
-                          f"determined. Excluding it from search."
-                    self.log_msg(msg, 'warning')
+                    self.msg = f"Geometry feature #{str(idx + 1)} could " \
+                            f"not be determined. Excluding it from search."
+                    self.log_msg(self.msg, 'warning')
                 else:
                     field_id = self._get_field_id('Footprint')
 
                     if self.err_occurred:
                         return None
 
                     self.geoms = [self.geoms] \
@@ -1127,73 +1147,104 @@
 
                 field_id = self._get_field_id(field)
 
                 if self.err_occurred:
                     return None
 
                 if field_id is None:
-                    msg = f"No available field named '{field}'."
-                    self.log_msg(msg, 'warning')
+                    self.msg = f"No available field named '{field}'."
+                    self.log_msg(self.msg, 'warning')
                     continue
 
                 d_type = self._get_field_type(self.collection, field_id)
 
                 # print("d_type: %s" % d_type)
 
                 op = values[0]
                 val = values[1]
 
+                if val is None or val == '': continue
+
                 if not any(c in op for c in '=><'):
                     op = ' %s ' % op
 
+                if not isinstance(val, list) and not isinstance(val, tuple):
+                    val = [val]
+
                 if field == 'Incidence Angle' or field == 'Scale' or \
                         field == 'Spacial Resolution' or \
                         field == 'Absolute Orbit':
-                    if isinstance(val, list) or isinstance(val, tuple):
-                        for v in val:
-                            if v.find('-') > -1:
-                                start, end = v.split('-')
-                                val_query = self._parse_range(field_id, start,
-                                                              end)
-                            else:
-                                val_query = f"{field_id}{op}{v}"
-                            query_lst.append(val_query)
-                        continue
-                    else:
-                        if str(val).find('-') > -1:
-                            start, end = str(val).split('-')
-                            val_query = self._parse_range(field_id, start, end)
+                    for v in val:
+                        if v.find('-') > -1:
+                            start, end = v.split('-')
+                            val_query = self._parse_range(field_id, start,
+                                                            end)
                         else:
-                            val_query = f"{field_id}{op}{val}"
+                            val_query = f"{field_id}{op}{v}"
+                        query_lst.append(val_query)
+                    continue
+                    # else:
+                    #     if str(val).find('-') > -1:
+                    #         start, end = str(val).split('-')
+                    #         val_query = self._parse_range(field_id, start, end)
+                    #     else:
+                    #         val_query = f"{field_id}{op}{val}"
+
+                elif field_id == 'RCM.SPECIAL_HANDLING_REQUIRED':
+                    val_query = f"{field_id}{op}{val[0]}"
+
                 elif field == 'Footprint':
 
                     pnts = []
-                    vals = val.split(' ')
+                    vals = val[0].split(' ')
                     for idx in range(0, len(vals), 2):
                         if vals[idx].strip() == '':
                             continue
 
                         pnts.append((float(vals[idx]), float(vals[idx + 1])))
 
                     self.geoms = self.geo.add_geom(pnts)
 
                     val_query = f"{field_id}{op}{self.geoms}"
 
                 else:
-                    if isinstance(val, list) or isinstance(val, tuple):
+                    # Convert choice to value
+                    choices = self.get_field_choices(self.collection, 
+                                                     field_id, True)
+                    valid_vals = []
+                    for v in val:
+                        new_val = None
+                        for c in choices:
+                            if c.get('label') == v:
+                                new_val = c.get('value')
+                                valid_vals.append(new_val)
+                                break
+                        if not new_val:
+                            valid_vals.append(v)
+
+                    val = valid_vals
+
+                    if len(val) > 1:
                         val_query = self._build_or(field_id, op, val, d_type)
                     else:
                         if d_type == 'String':
-                            val_query = f"{field_id}{op}'{val}'"
+                            val_query = f"{field_id}{op}'{val[0]}'"
+                        elif d_type == 'Boolean':
+                            if val[0].lower().find('t') > -1 \
+                                or val[0].lower().find('y') > -1:
+                                val_query = f"{field_id}{op}True"
+                            elif val[0].lower().find('f') > -1 \
+                                or val[0].lower().find('n') > -1:
+                                val_query = f"{field_id}{op}False"
                         elif d_type == 'DateTimeRange':
-                            date = dateutil.parser.parse(val)
+                            date = dateutil.parser.parse(val[0])
                             iso_date = date.isoformat()
                             val_query = f"{field_id}{op}'{iso_date}'"
                         else:
-                            val_query = f"{field_id}{op}{val}"
+                            val_query = f"{field_id}{op}{val[0]}"
 
                 query_lst.append(val_query)
 
         if len(query_lst) > 1:
             query_lst = ['(%s)' % q if q.find(' OR ') > -1 else q
                          for q in query_lst]
 
@@ -1586,14 +1637,24 @@
         Gets the error message of this class after an error occurred.
 
         :return: The error message
         :rtype: str
         """
 
         return self.err_msg
+    
+    def get_msg(self):
+        """
+        Gets the latest self.msg
+
+        :return: The self.msg
+        :rtype: str
+        """
+
+        return self.msg
 
     def set_query_timeout(self, timeout):
         """
         Sets the timeout limit for a query to the RAPI.
 
         :param timeout: The value of the timeout in seconds.
         :type  timeout: float
@@ -1671,24 +1732,24 @@
         """
 
         # If we have an existing local file, check the filesize against the
         #   manifest
         if os.path.exists(dest_fn):
             # if all-good, continue to next file
             if os.stat(dest_fn).st_size == fsize:
-                msg = f"No download necessary. Local file already exists: " \
-                      f"{dest_fn}"
-                self.log_msg(msg)
+                self.msg = f"No download necessary. Local file already " \
+                    f"exists: {dest_fn}"
+                self.log_msg(self.msg)
                 return None
             # Otherwise, delete the incomplete/malformed local file and
             #   redownload
             else:
-                msg = f'Filesize mismatch with {os.path.basename(dest_fn)}. ' \
-                      f'Re-downloading...'
-                self.log_msg(msg, 'warning')
+                self.msg = f'Filesize mismatch with ' \
+                    f'{os.path.basename(dest_fn)}. Re-downloading...'
+                self.log_msg(self.msg, 'warning')
                 os.remove(dest_fn)
 
         if self._check_auth():
             return None
 
         # Use streamed download so we can wrap nicely with tqdm
         if show_progress:
@@ -1703,16 +1764,16 @@
                     ) as file_out:
                         for chunk in stream.iter_content(chunk_size=1024):
                             file_out.write(chunk)
         else:
             response = self._session.get(url, stream=True, verify=self.verify)
             open(dest_fn, "wb").write(response.content)
 
-        msg = f'{dest_fn} has been downloaded.'
-        self.log_msg(msg)
+        self.msg = f'{dest_fn} has been downloaded.'
+        self.log_msg(self.msg)
 
     def download(self, items, dest, wait=10.0, max_attempts=None,
                  show_progress=True):
         """
         Downloads a list of order items from the EODMS RAPI.
 
         :param items: A list of order items returned from the RAPI.
@@ -1759,39 +1820,39 @@
         :rtype: list
         """
 
         msg = "Downloading images..."
         self.log_msg(msg, log_indent='\n\n\t', out_indent='\n')
 
         if items is None:
-            msg = "No images to download."
-            self.log_msg(msg)
+            self.msg = "No images to download."
+            self.log_msg(self.msg)
             return []
 
         if isinstance(items, dict):
             if 'items' in items.keys():
                 items = items['items']
 
         if len(items) == 0:
-            msg = "No images to download."
-            self.log_msg(msg)
+            self.msg = "No images to download."
+            self.log_msg(self.msg)
             return []
 
         unique_items = self.remove_duplicate_orders(items)
 
         attempt = 0
         complete_items = []
         while len(unique_items) > len(complete_items):
             time.sleep(wait)
             attempt += 1
 
             if max_attempts is not None and not max_attempts == '':
                 if attempt > max_attempts:
-                    msg = "Maximum number of attempts reached."
-                    self.log_msg(msg, log_indent='\n\n\t', out_indent='\n')
+                    self.msg = "Maximum number of attempts reached."
+                    self.log_msg(self.msg, log_indent='\n\n\t', out_indent='\n')
                     return complete_items
 
             # start, end = self._get_dateRange(unique_items)
             # orders = self.get_orders(dtstart=start, dtend=end)
             # print(f"max_downloads: {max_downloads}")
             # answer = input("Press enter...")
             # max_orders = max_downloads + int((max_downloads / 4))
@@ -1804,22 +1865,22 @@
             #     print(f"  recordId: {order.get('recordId')}")
             # answer = input("Press enter...")
 
             if self.err_occurred:
                 return complete_items
 
             if orders is None:
-                msg = "An error occurred while getting a list of orders. " \
-                      "Downloads unsuccessful."
-                self.log_msg(msg)
+                self.msg = "An error occurred while getting a list of " \
+                    "orders. Downloads unsuccessful."
+                self.log_msg(self.msg)
                 return []
 
             if len(orders) == 0:
-                msg = "No orders could be found."
-                self.log_msg(msg)
+                self.msg = "No orders could be found."
+                self.log_msg(self.msg)
                 return []
 
             new_count = len(complete_items)
 
             for itm in unique_items:
                 item_id = itm['itemId']
                 cur_item = self._get_item_from_orders(item_id, orders)
@@ -1832,40 +1893,40 @@
                 if self._check_complete(complete_items, record_id):
                     continue
 
                 if status in self.failed_status:
                     if status == 'FAILED':
                         # If the order has failed, inform user
                         status_mess = cur_item.get('statusMessage')
-                        msg = "\n  The following Order Item has failed:"
+                        self.msg = "\n  The following Order Item has failed:"
                         if status_mess is None:
-                            msg += f"\n    Order Item Id: " \
+                            self.msg += f"\n    Order Item Id: " \
                                    f"{cur_item['itemId']}\n" \
                                    f"    Order Id: {order_id}\n" \
                                    f"    Record Id: {cur_item['recordId']}" \
                                    f"    Collection: {coll_id}\n"
 
                         else:
-                            msg += f"\n    Order Item Id: " \
+                            self.msg += f"\n    Order Item Id: " \
                                    f"{cur_item['itemId']}\n" \
                                    f"    Order Id: {order_id}\n" \
                                    f"    Record Id: {cur_item['recordId']}\n" \
                                    f"    Collection: {coll_id}\n" \
                                    f"    Reason for Failure: " \
                                    f"{cur_item['statusMessage']}"
                     else:
                         # If the order was unsuccessful with another status,
                         #   inform user
-                        msg = f"\n  The following Order Item has status " \
+                        self.msg = f"\n  The following Order Item has status " \
                               f"'{status}' and will not be downloaded:"
-                        msg += f"\n    Order Item Id: {cur_item['itemId']}\n" \
+                        self.msg += f"\n    Order Item Id: {cur_item['itemId']}\n" \
                                f"    Record Id: {cur_item['recordId']}\n" \
                                f"    Collection: {coll_id}\n"
 
-                    self.log_msg(msg)
+                    self.log_msg(self.msg)
 
                     cur_item['downloaded'] = 'False'
 
                     complete_items.append(cur_item)
 
                 elif status == 'AVAILABLE_FOR_DOWNLOAD':
                     cur_item['downloaded'] = 'True'
@@ -1887,16 +1948,16 @@
                         root = ElementTree.fromstring(str_val)
                         url = root.text
                         url = url.split("?")[0]
 
                         fn = os.path.basename(url)
 
                         # Download the image
-                        msg = f"Downloading image from Collection {coll_id} " \
-                              f"with Record Id {record_id} ({fn})."
+                        msg = f"Downloading image from Collection " \
+                            f"{coll_id} with Record Id {record_id} ({fn})."
                         self.log_msg(msg)
 
                         # Save the image contents to the 'downloads' folder
                         out_fn = os.path.join(dest, fn)
                         full_path = os.path.realpath(out_fn)
 
                         if not os.path.exists(dest):
@@ -1916,19 +1977,19 @@
                         download_paths.append(dest_info)
 
                     cur_item['downloadPaths'] = download_paths
 
                     complete_items.append(cur_item)
 
             if new_count == 0 and len(complete_items) == 0:
-                msg = "No items are ready for download yet."
-                self.log_msg(msg)
+                self.msg = "No items are ready for download yet."
+                self.log_msg(self.msg)
             elif new_count == len(complete_items):
-                msg = "No new items are ready for download yet."
-                self.log_msg(msg)
+                self.msg = "No new items are ready for download yet."
+                self.log_msg(self.msg)
 
         return complete_items
 
     def get_available_fields(self, collection=None, name_type='all',
                              ui_fields=False):
         """
         Gets a dictionary of available fields for a collection from the RAPI.
@@ -2001,15 +2062,15 @@
             for r in coll_res['resultFields']:
                 res_fields[r['title']] = r
 
             fields['results'] = res_fields
 
         return fields
 
-    def get_field_choices(self, collection, field=None):
+    def get_field_choices(self, collection, field=None, full=False):
         """
         Gets the available choices for a specified field. If no choices exist,
         then the data type is returned.
 
         :param collection: The collection containing the field.
         :type  collection: str
         :param field: The field name or field ID.
@@ -2027,29 +2088,35 @@
 
         all_fields = {}
         for f, v in fields['search'].items():
             choices = []
             if field is None:
                 field_choices = v.get('choices')
                 if field_choices is not None:
-                    for c in field_choices:
-                        value = c['value']
-                        if not value == '':
-                            choices.append(value)
+                    if full:
+                        choices = field_choices
+                    else:
+                        for c in field_choices:
+                            value = c['value']
+                            if not value == '':
+                                choices.append(value)
                     all_fields[f] = choices
                 else:
                     all_fields[f] = {'data_type': v.get('datatype')}
             else:
                 if f == field or v['id'] == field:
                     field_choices = v.get('choices')
                     if field_choices is not None:
-                        for c in field_choices:
-                            value = c['value']
-                            if not value == '':
-                                choices.append(value)
+                        if full:
+                            choices = field_choices
+                        else:
+                            for c in field_choices:
+                                value = c['value']
+                                if not value == '':
+                                    choices.append(value)
                         return choices
                     else:
                         return {'data_type': v.get('datatype')}
 
         return all_fields
 
     def get_collections(self, as_list=False, opt='id', redo=False):
@@ -2089,15 +2156,14 @@
         query_url = f"{self.rapi_root}/collections?format=json"
 
         msg = "Getting Collection information, please wait..."
         self.log_msg(msg)
         logger.debug(f"RAPI URL: {query_url}")
 
         # Send the query URL
-        # print(f"query_url: {query_url}")
         coll_res = self._submit(query_url, timeout=20.0)
 
         if coll_res is None or self.err_occurred:
             return None
 
         # If an error occurred
         if isinstance(coll_res, QueryError):
@@ -2193,19 +2259,19 @@
         res = self._submit(query_url, timeout=self.timeout_query, quiet=False)
 
         if self.err_occurred:
             return None
 
         if res is None or isinstance(res, QueryError):
             if isinstance(res, QueryError):
-                msg = f"Could not get order with Order ID {order_id} due " \
+                self.msg = f"Could not get order with Order ID {order_id} due " \
                       f"to {res.get_msgs(True)}."
             else:
-                msg = f"Could not get order with Order ID {order_id}."
-            self.log_msg(msg, 'warning')
+                self.msg = f"Could not get order with Order ID {order_id}."
+            self.log_msg(self.msg, 'warning')
             return None
 
         if 'items' in res.keys():
             return res['items']
         else:
             return res
 
@@ -2258,20 +2324,20 @@
                                    quiet=False)
 
                 if self.err_occurred:
                     return None
 
                 if res is None or isinstance(res, QueryError):
                     if isinstance(res, QueryError):
-                        msg = f"Order submission was unsuccessful due to: " \
-                              f"{res.get_msgs(True)}."
+                        self.msg = f"Order submission was unsuccessful due " \
+                            f"to: {res.get_msgs(True)}."
 
                     else:
-                        msg = "Order submission was unsuccessful."
-                    self.log_msg(msg, 'warning')
+                        self.msg = "Order submission was unsuccessful."
+                    self.log_msg(self.msg, 'warning')
                     continue
 
                 if 'items' in res.keys():
                     res = res['items']
 
                 all_orders += res
 
@@ -2294,20 +2360,20 @@
         res = self._submit(query_url, timeout=self.timeout_query, quiet=False)
 
         if self.err_occurred:
             return None
 
         if res is None or isinstance(res, QueryError):
             if isinstance(res, QueryError):
-                msg = f"Order submission was unsuccessful due to: " \
+                self.msg = f"Order submission was unsuccessful due to: " \
                       f"{res.get_msgs(True)}."
 
             else:
-                msg = "Order submission was unsuccessful."
-            self.log_msg(msg, 'warning')
+                self.msg = "Order submission was unsuccessful."
+            self.log_msg(self.msg, 'warning')
             return None
 
         if 'items' in res.keys():
             res = res['items']
 
         if status is not None:
             status_res = [r for r in res if r.get('status') == status.upper()]
@@ -2327,16 +2393,16 @@
         """
 
         if isinstance(records, dict):
             if 'items' in records.keys():
                 records = records['items']
 
         if records is None or len(records) == 0:
-            msg = "Cannot get orders as no image items provided."
-            self.log_msg(msg, log_indent='\n\n\t', out_indent='\n')
+            self.msg = "Cannot get orders as no image items provided."
+            self.log_msg(self.msg, log_indent='\n\n\t', out_indent='\n')
             return None
 
         if not all("orderId" in keys for keys in records):
             # msg = "Cannot get orders as no orderId is provided in the " \
             #       "results."
             orders = self.get_orders()
             # self.log_msg(msg, log_indent='\n\n\t', out_indent='\n')
@@ -2382,22 +2448,22 @@
 
             # Get the most recent order item with the given recordId
             filt_recs = [r for r in rec_orders if r['recordId'] == rec_id]
             order_item = max(filt_recs, key=lambda x: x['dateSubmitted'])
 
             found_orders.append(order_item)
 
-        msg = f"Found {len(found_orders)} order items for the following " \
+        self.msg = f"Found {len(found_orders)} order items for the following " \
               f"records: {', '.join([r['recordId'] for r in found_orders])}"
-        self.log_msg(msg)
+        self.log_msg(self.msg)
 
         if len(unfound) > 0:
-            msg = f"No order items found for the following records: " \
+            self.msg = f"No order items found for the following records: " \
                   f"{', '.join(unfound)}"
-            self.log_msg(msg)
+            self.log_msg(self.msg)
 
         return found_orders
 
     def get_order_parameters(self, collection, record_id):
         """
         Gets the list of available Order parameters for a given image record.
 
@@ -2442,17 +2508,17 @@
             self.err_occurred = True
             print()
             return None
 
         if not param_res.ok:
             err = self._get_exception(param_res)
             if isinstance(err, list):
-                msg = '; '.join(err)
-                self.log_msg(msg, 'warning')
-                return msg
+                self.msg = '; '.join(err)
+                self.log_msg(self.msg, 'warning')
+                return self.msg
 
         # msg = "Order removed successfully."
         # self.log_msg(msg)
 
         return param_res.json()
 
     def get_rapi_url(self):
@@ -2486,17 +2552,17 @@
 
         self.results = self._submit(self._rapi_url)
 
         if self.err_occurred:
             return None
 
         if isinstance(self.results, QueryError):
-            msg = self.results.get_msgs()
-            self.log_msg(msg, 'warning')
-            return {'errors': msg}
+            self.msg = self.results.get_msgs()
+            self.log_msg(self.msg, 'warning')
+            return {'errors': self.msg}
 
         if output == 'geojson':
             feat = self.geo.convert_to_geojson(self.results, 'list')
             return feat
         elif output == 'raw':
             return self.results
         else:
@@ -2545,20 +2611,20 @@
         #     self.err_occurred = True
         #     print()
         #     return None
 
         if not cancel_res.ok:
             err = self._get_exception(cancel_res)
             if isinstance(err, list):
-                msg = '; '.join(err)
-                self.log_msg(msg, 'warning')
-                return msg
+                self.msg = '; '.join(err)
+                self.log_msg(self.msg, 'warning')
+                return self.msg
 
-        msg = "Order removed successfully."
-        self.log_msg(msg)
+        self.msg = "Order removed successfully."
+        self.log_msg(self.msg)
 
         return cancel_res.content
 
     def create_destination(self, dest_type, dest_name, **kwargs):
         """
         Create a new destination using the given dest_type and dest_name.
 
@@ -2835,17 +2901,17 @@
 
         self.results = self._submit(self._rapi_url)
 
         if self.err_occurred:
             return None
 
         if isinstance(self.results, QueryError):
-            msg = self.results.get_msgs()
-            self.log_msg(msg, 'warning')
-            return {'errors': msg}
+            self.msg = self.results.get_msgs()
+            self.log_msg(self.msg, 'warning')
+            return {'errors': self.msg}
 
         return self.results
 
     def search_url(self, url, **kwargs):
         """
         Submits a URL to the RAPI.
 
@@ -2942,24 +3008,24 @@
 
         if self.err_occurred:
             return None
 
         self.res_mdata = None
 
         if isinstance(self.search_results, QueryError):
-            msg = self.search_results.get_msgs()
+            msgs = self.search_results.get_msgs()
             if isinstance(msgs, list):
                 self.log_msg(': '.join(msgs), 'warning')
             else:
                 self.log_msg(msgs, 'warning')
             return {'errors': msg}
 
-        msg = f"Number of {self.collection} images returned from RAPI: " \
+        self.msg = f"Number of {self.collection} images returned from RAPI: " \
               f"{len(self.search_results)}"
-        self.log_msg(msg)
+        self.log_msg(self.msg)
 
         self.results += self.search_results
 
     def search(self, collection, filters=None, features=None, dates=None,
                result_fields=None, max_results=None):
         """
         Sends a search to the RAPI to search for image results.
@@ -3031,18 +3097,18 @@
         result_field = []
         for field in result_fields:
             field_id = self._get_field_id(field, field_type='results')
             if self.err_occurred:
                 return None
 
             if field_id is None:
-                msg = f"Field '{field}'' does not exist for collection " \
+                self.msg = f"Field '{field}'' does not exist for collection " \
                       f"'{self.collection}'. Excluding it from resultField " \
                       f"entry."
-                self.log_msg(msg, 'warning')
+                self.log_msg(self.msg, 'warning')
             else:
                 result_field.append(field_id)
 
         # Get the geometry field and add it to resultField
         footprint_id = self._get_field_id('Footprint', field_type='results')
         if self.err_occurred:
             return None
@@ -3097,20 +3163,35 @@
             msgs = self.search_results.get_msgs()
             if isinstance(msgs, list):
                 self.log_msg(': '.join(msgs), 'warning')
             else:
                 self.log_msg(msgs, 'warning')
             return {'errors': msgs}
 
-        msg = f"Number of {self.collection} images returned from RAPI: " \
+        self.msg = f"Number of {self.collection} images returned from RAPI: " \
               f"{len(self.search_results)}"
-        self.log_msg(msg)
+        self.log_msg(self.msg)
 
         self.results += self.search_results
 
+    def reset(self):
+        """
+        Resets specific values for the EODMSRAPI.
+
+        :return: n/a
+        """
+
+        self.clear_results()
+        self.err_msg = None
+        self.msg = ''
+        self.err_occurred = False
+        self.auth_err = False
+        self.order_json = None
+        self.search_results = None
+
     def clear_results(self):
         """
         Clears the cumulative results.
 
         :return: n/a
         """
 
@@ -3138,17 +3219,17 @@
 
         :return: A dictionary of the results from self.results variable.
         :rtype:  dict
 
         """
 
         if self.results is None:
-            msg = "No results exist. Please use search() to run a search " \
-                  "on the RAPI."
-            self.log_msg(msg, 'warning')
+            self.msg = "No results exist. Please use search() to run a " \
+                "search on the RAPI."
+            self.log_msg(self.msg, 'warning')
             return None
 
         if isinstance(self.results, QueryError):
             return [{'errors': self.results.get_msgs()}]
 
         if len(self.results) == 0:
             return self.results
@@ -3357,17 +3438,17 @@
 
             if self.err_occurred:
                 return None
 
             if order_res is None:
                 err = self._get_exception(order_res)
                 if isinstance(err, list):
-                    msg = '; '.join(err)
-                    self.log_msg(msg, 'warning')
-                    return msg
+                    self.msg = '; '.join(err)
+                    self.log_msg(self.msg, 'warning')
+                    return self.msg
 
             if isinstance(order_res, requests.Response) and not order_res.ok:
                 self.err_msg = "Order submission failed."
                 self.log_msg(self.err_msg, 'error')
                 self.err_occurred = True
                 return self.err_msg
 
@@ -3377,11 +3458,11 @@
             for i in items:
                 i['dateRapiOrdered'] = time_submitted
 
             all_items += items
 
         final_res = {'items': all_items}
 
-        msg = "Order submitted successfully."
-        self.log_msg(msg)
+        self.msg = "Order submitted successfully."
+        self.log_msg(self.msg)
 
         return final_res
```

### Comparing `py-eodms-rapi-1.5.3/eodms_rapi/geo.py` & `py-eodms-rapi-1.5.4/eodms_rapi/geo.py`

 * *Files identical despite different names*

### Comparing `py-eodms-rapi-1.5.3/py_eodms_rapi.egg-info/PKG-INFO` & `py-eodms-rapi-1.5.4/py_eodms_rapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-eodms-rapi
-Version: 1.5.3
+Version: 1.5.4
 Summary: EODMS RAPI Client is a Python3 package used to access the REST API service provided by the Earth Observation Data Management System (EODMS) from Natural Resources Canada.
 Home-page: https://py-eodms-rapi.readthedocs.io/en/latest/
 Author: Kevin Ballantyne (Natural Resources Canada)
 Author-email: kevin.ballantyne@nrcan-rncan.gc.ca
 License: LICENSE
 Project-URL: Source, https://github.com/eodms-sgdot/py-eodms-rapi
 Project-URL: Bug Tracker, https://github.com/eodms-sgdot/py-eodms-rapi/issues
```

### Comparing `py-eodms-rapi-1.5.3/setup.cfg` & `py-eodms-rapi-1.5.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 792d 656f 646d 732d 7261 7069   = py-eodms-rapi
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 352e  ..version = 1.5.
-00000030: 330d 0a61 7574 686f 7220 3d20 4b65 7669  3..author = Kevi
+00000030: 340d 0a61 7574 686f 7220 3d20 4b65 7669  4..author = Kevi
 00000040: 6e20 4261 6c6c 616e 7479 6e65 2028 4e61  n Ballantyne (Na
 00000050: 7475 7261 6c20 5265 736f 7572 6365 7320  tural Resources 
 00000060: 4361 6e61 6461 290d 0a61 7574 686f 725f  Canada)..author_
 00000070: 656d 6169 6c20 3d20 6b65 7669 6e2e 6261  email = kevin.ba
 00000080: 6c6c 616e 7479 6e65 406e 7263 616e 2d72  llantyne@nrcan-r
 00000090: 6e63 616e 2e67 632e 6361 0d0a 6465 7363  ncan.gc.ca..desc
 000000a0: 7269 7074 696f 6e20 3d20 454f 444d 5320  ription = EODMS
```

### Comparing `py-eodms-rapi-1.5.3/setup.py` & `py-eodms-rapi-1.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='py-eodms-rapi',
-    version='1.5.3', 
+    version='1.5.4', 
     author='Kevin Ballantyne (Natural Resources Canada)',
     author_email='kevin.ballantyne@nrcan-rncan.gc.ca',
     packages=find_packages(),
     include_package_data=True, 
     url='https://py-eodms-rapi.readthedocs.io/en/latest/',
     license='LICENSE',
     description='EODMS RAPI Client is a Python3 package used to access the REST API service provided by the Earth Observation Data Management System (EODMS) from Natural Resources Canada.',
```

### Comparing `py-eodms-rapi-1.5.3/test/test_pyeodmsrapi.py` & `py-eodms-rapi-1.5.4/test/test_pyeodmsrapi.py`

 * *Files identical despite different names*

