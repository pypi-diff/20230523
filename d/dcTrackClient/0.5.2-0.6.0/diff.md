# Comparing `tmp/dctrackclient-0.5.2.tar.gz` & `tmp/dctrackclient-0.6.0.tar.gz`

## Comparing `dctrackclient-0.5.2.tar` & `dctrackclient-0.6.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11747 2020-02-02 00:00:00.000000 dctrackclient-0.5.2/src/dcTrackClient/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.5.2/.gitignore
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 dctrackclient-0.5.2/pyproject.toml
--rw-r--r--   0        0        0    15356 2020-02-02 00:00:00.000000 dctrackclient-0.5.2/../README.md
--rw-r--r--   0        0        0    15978 2020-02-02 00:00:00.000000 dctrackclient-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    14009 2020-02-02 00:00:00.000000 dctrackclient-0.6.0/src/dcTrackClient/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.6.0/.gitignore
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 dctrackclient-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    17375 2020-02-02 00:00:00.000000 dctrackclient-0.6.0/../README.md
+-rw-r--r--   0        0        0    17997 2020-02-02 00:00:00.000000 dctrackclient-0.6.0/PKG-INFO
```

### Comparing `dctrackclient-0.5.2/src/dcTrackClient/__init__.py` & `dctrackclient-0.6.0/src/dcTrackClient/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,19 +33,19 @@
         """Delete an item using the item ID."""
         return self.__request('DELETE', '/api/v2/dcimoperations/items/' + str(id) + '/?')
 
     def searchItems(self, pageNumber: int, pageSize: int, payload: dict):
         """Search for items using criteria JSON object. Search criteria can be any of the fields applicable to items, including custom fields. Specify the fields to be included in the response. This API supports pagination. Returns a list of items with the specified information."""
         return self.__request('POST', '/api/v2/quicksearch/items/?pageNumber=' + str(pageNumber) + '&pageSize=' + str(pageSize) + '&', payload)
 
-    def cabinetItems(self, CabinetId: int):
+    def getCabinetItems(self, CabinetId: int):
         """Returns a list of Items contained in a Cabinet using the ItemID of the Cabinet. The returned list includes all of the Cabinet's Items including Passive Items."""
         return self.__request('GET', '/api/v2/items/cabinetItems/' + str(CabinetId) + '/?')
 
-    def manageItemsBulk(self, payload: dict):
+    def createItemsBulk(self, payload: dict):
         """Add/Update/Delete Items."""
         return self.__request('POST', '/api/v2/dcimoperations/items/bulk/?', payload)
 
     def getMakes(self):
         """Returns a list of makes with basic information."""
         return self.__request('GET', '/api/v2/makes/?')
 
@@ -57,17 +57,17 @@
         """Modify a Make. Returns JSON entity containing Make information that was passed in from the Request payload."""
         return self.__request('PUT', '/api/v2/makes/' + str(makeId) + '/?', payload)
 
     def deleteMake(self, makeId: int):
         """Delete a Make."""
         return self.__request('DELETE', '/api/v2/makes/' + str(makeId) + '/?')
 
-    def searchMakes(self, makeName: str):
+    def searchMakes(self, makeName: str, payload: dict):
         """Search for a make using the make name. Returns a list of makes with basic information."""
-        return self.__request('GET', '/api/v2/dcimoperations/search/makes/' + str(makeName) + '/?')
+        return self.__request('POST', '/api/v2/dcimoperations/search/makes/' + str(makeName) + '/?', payload)
 
     def getModel(self, modelId: int, usedCounts: int):
         """Get Model fields for the specified Model ID. usedCounts is an optional parameter that determines if the count of Items for the specified model is returned in the response. If set to "true" the counts will be included in the response, if omitted or set to "false" the item count will not be included in the response."""
         return self.__request('GET', '/api/v2/models/' + str(modelId) + '/?usedCounts=' + str(usedCounts) + '&')
 
     def createModel(self, returnDetails: bool, proceedOnWarning: bool, payload: dict):
         """Add a new Model. Returns JSON entity containing Make information that was passed in from the Request payload. "proceedOnWarning" relates to the warning messages that are thrown in dcTrack when you try to delete custom fields that are in use. The "proceedOnWarning" value can equal either "true" or "false." If "proceedOnWarning" equals "true," business warnings will be ignored. If "proceedOnWarning" equals "false," business warnings will not be ignored. Fields that are not in the payload will remain unchanged."""
@@ -93,15 +93,15 @@
         """Add a new Connector. Returns JSON entity containing Connector information that was passed in from the Request payload."""
         return self.__request('POST', '/api/v2/settings/connectors/?', payload)
 
     def updateConnector(self, connectorId: int, payload: dict):
         """Update an existing Connector. Returns JSON entity containing Connector information that was passed in from the Request payload."""
         return self.__request('PUT', '/api/v2/settings/connectors/' + str(connectorId) + '/?', payload)
 
-    def deleteConnector(self, payload: dict):
+    def removeConnector(self, payload: dict):
         """Delete one or more Connector records."""
         return self.__request('POST', '/api/v2/settings/connectors/delete/?', payload)
 
     def searchConnectors(self, pageNumber: int, pageSize: int, usedCount: bool, payload: dict):
         """Retrieve a List of Connectors. Returns JSON entity containing Connector information that was passed in from the Request payload. Please note, Compatible Connectors are not returned by this API, but can be returned when querying a single Connector using the /api/v2/settings/connectors/{connectorId} API."""
         return self.__request('POST', '/api/v2/settings/connectors/quicksearch/?pageNumber=' + str(pageNumber) + '&pageSize=' + str(pageSize) + '&usedCount=' + str(usedCount) + '&', payload)
 
@@ -140,7 +140,35 @@
     def updatePowerPort(self, itemId: int, portId: int, proceedOnWarning: bool, payload: dict):
         """Use the REST API to create power ports for an existing item. If ports are already defined for the item because it is included in the Item Models Library, you can use the REST API to create additional ports for the item."""
         return self.__request('PUT', '/api/v1/items/' + str(itemId) + '/powerports/' + str(portId) + '/?proceedOnWarning=' + str(proceedOnWarning) + '&', payload)
 
     def getCompatibleConnector(self, itemId: int, portId: int, connectorId: int):
         """Use the REST API to determine if a Connector is compatible with a specific Power Port."""
         return self.__request('GET', '/api/v1/items/' + str(itemId) + '/powerports/' + str(portId) + '/connectors/' + str(connectorId) + '/isCompatible/?')
+
+    def getLocations(self):
+        """Returns a list for all Locations."""
+        return self.__request('GET', '/api/v1/locations/?')
+
+    def getLocation(self, locationId: int):
+        """Get a single Location. Returns json containing location data for the specified ID."""
+        return self.__request('GET', '/api/v1/locations' + str(locationId) + '/?')
+
+    def createLocation(self, proceedOnWarning: bool, payload: dict):
+        """Add a Location. Returns the JSON entity containing location info that was passed in. Note: "proceedOnWarning" relates to the warning messages that are thrown in dcTrack when you try to delete custom fields that are in use. The "proceedOnWarning" value can equal either "true" or "false." If "proceedOnWarning" equals "true," business warnings will be ignored. If "proceedOnWarning" equals "false," business warnings will not be ignored."""
+        return self.__request('POST', '/api/v1/locations/?proceedOnWarning=' + str(proceedOnWarning) + '&', payload)
+
+    def updateLocation(self, locationId: int, proceedOnWarning: bool, payload: dict):
+        """Modify Location details for a single Location. Payload contains new location details. You do not have have to provide all details, but only those that you want to modify. Returns JSON entity containing Location information that was passed in from the Request payload."""
+        return self.__request('PUT', '/api/v1/locations/' + str(locationId) + '/?proceedOnWarning=' + str(proceedOnWarning) + '&', payload)
+
+    def deleteLocation(self, locationId: int):
+        """Delete a Location."""
+        return self.__request('DELETE', '/api/v1/locations/' + str(locationId) + '/?')
+
+    def searchLocations(self, pageNumber: int, pageSize: int, payload: dict):
+        """Search for Locations by user supplied search criteria. Returns a list of Locations with the "selectedColumns" returned in the payload."""
+        return self.__request('POST', '/api/v2/quicksearch/locations/?pageNumber=' + str(pageNumber) + '&pageSize=' + str(pageSize) + '&', payload)
+
+    def getLocationFieldList(self):
+        """Returns a list of all Location fields."""
+        return self.__request('GET', '/api/v2/quicksearch/locations/locationListFields/?')
```

### Comparing `dctrackclient-0.5.2/pyproject.toml` & `dctrackclient-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcTrackClient"
-version = "0.5.2"
+version = "0.6.0"
 authors = [
   { name="Nicolas Ventura", email="ventura@lbl.gov" },
 ]
 description = "Sunbird dcTrack API client in Python"
 readme = "../README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dctrackclient-0.5.2/../README.md` & `dctrackclient-0.6.0/../README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 Sunbird [dcTrack](https://www.sunbirddcim.com/) API clients in Python and JavaScript
 
 ## Installation
 > dcTrackClient can be installed from the package manager of your choice.
 
 ### Python
 ```shell
-pip install dcTrackClient==0.5.2
+pip install dcTrackClient==0.6.0
 ```
 
 ### JavaScript
 ```shell
-npm i dctrackclient@0.5.2
+npm i dctrackclient@0.6.0
 ```
 
 ## Initialize a connection to the dcTrack API
 > Authentication is by using a base URL (the same URL to access the GUI) and a username and password, or a base URL and an API token.
 
 ### Python
 ```py
@@ -65,15 +65,15 @@
 });
 console.log(response);
 ```
 
 ### On Success
 This function returns the JSON object for the newly created item. This is an example response if `returnDetails` was set to false.
 ```json
-{ "item": { "id": 1234, "tiName": "item" } }
+{ "item": { "id": 1234, "tiName": "item name" } }
 ```
 
 ### On Failure
 This function returns a JSON object containing the error message.
 
 ## Retrieve item details
 > This example shows the usage of the [`getItem`](#getitemid) function.
@@ -100,20 +100,20 @@
 ```
 
 ## Modify an existing item
 > This example shows the usage of the [`updateItem`](#updateitemid-returndetails-payload) function. Any number of attributes can be included in the payload to be modified.
 
 ### Python
 ```py
-response = api.updateItem(976, False, {'tiSerialNumber': 12345})
+response = api.updateItem(1234, False, {'tiSerialNumber': 12345})
 ```
 
 ### JavaScript
 ```js
-let response = await api.updateItem(977, false, { 'tiSerialNumber': 12345 });
+let response = await api.updateItem(1234, false, { 'tiSerialNumber': 12345 });
 ```
 
 ## Search for an item
 > This example demonstrates usage of the [`searchItems`](#searchitemspagenumber-pagesize-payload) function. Follow [this guide](https://www.sunbirddcim.com/help/dcTrack/v900/API/en/Default.htm#APIGuide/v2_Advanced_Search_API.htm) for details on creating the request payload.
 
 ### Python
 ```py
@@ -230,24 +230,24 @@
 ```
 |Parameter|Type|
 |---|---|
 |pageNumber|number|
 |pageSize|number|
 |payload|object|
 
-## cabinetItems(CabinetId)
+## getCabinetItems(CabinetId)
 > Returns a list of Items contained in a Cabinet using the ItemID of the Cabinet. The returned list includes all of the Cabinet's Items including Passive Items.
 ```
 GET api/v2/items/cabinetItems/{CabinetId}
 ```
 |Parameter|Type|
 |---|---|
 |CabinetId|number|
 
-## manageItemsBulk(payload)
+## createItemsBulk(payload)
 > Add/Update/Delete Items.
 ```
 POST api/v2/dcimoperations/items/bulk payload
 ```
 |Parameter|Type|
 |---|---|
 |payload|object|
@@ -283,22 +283,23 @@
 ```
 DELETE api/v2/makes/{makeId}
 ```
 |Parameter|Type|
 |---|---|
 |makeId|number|
 
-## searchMakes(makeName)
+## searchMakes(makeName, payload)
 > Search for a make using the make name. Returns a list of makes with basic information.
 ```
-GET api/v2/dcimoperations/search/makes/{makeName}
+POST api/v2/dcimoperations/search/makes/{makeName} payload
 ```
 |Parameter|Type|
 |---|---|
 |makeName|string|
+|payload|object|
 
 ## getModel(modelId, usedCounts)
 > Get Model fields for the specified Model ID. usedCounts is an optional parameter that determines if the count of Items for the specified model is returned in the response. If set to "true" the counts will be included in the response, if omitted or set to "false" the item count will not be included in the response.
 ```
 GET api/v2/models/{modelId}
 ```
 |Parameter|Type|
@@ -372,15 +373,15 @@
 PUT api/v2/settings/connectors/{connectorId} payload
 ```
 |Parameter|Type|
 |---|---|
 |connectorId|number|
 |payload|object|
 
-## deleteConnector(payload)
+## removeConnector(payload)
 > Delete one or more Connector records.
 ```
 POST api/v2/settings/connectors/delete payload
 ```
 |Parameter|Type|
 |---|---|
 |payload|object|
@@ -493,7 +494,71 @@
 GET api/v1/items/{itemId}/powerports/{portId}/connectors/{connectorId}/isCompatible
 ```
 |Parameter|Type|
 |---|---|
 |itemId|number|
 |portId|number|
 |connectorId|number|
+
+## getLocations()
+> Returns a list for all Locations.
+```
+GET api/v1/locations
+```
+*No parameters.*
+
+## getLocation(locationId)
+> Get a single Location. Returns json containing location data for the specified ID.
+```
+GET api/v1/locations{locationId}
+```
+|Parameter|Type|
+|---|---|
+|locationId|number|
+
+## createLocation(proceedOnWarning, payload)
+> Add a Location. Returns the JSON entity containing location info that was passed in. Note: "proceedOnWarning" relates to the warning messages that are thrown in dcTrack when you try to delete custom fields that are in use. The "proceedOnWarning" value can equal either "true" or "false." If "proceedOnWarning" equals "true," business warnings will be ignored. If "proceedOnWarning" equals "false," business warnings will not be ignored.
+```
+POST api/v1/locations payload
+```
+|Parameter|Type|
+|---|---|
+|proceedOnWarning|boolean|
+|payload|object|
+
+## updateLocation(locationId, proceedOnWarning, payload)
+> Modify Location details for a single Location. Payload contains new location details. You do not have have to provide all details, but only those that you want to modify. Returns JSON entity containing Location information that was passed in from the Request payload.
+```
+PUT api/v1/locations/{locationId} payload
+```
+|Parameter|Type|
+|---|---|
+|locationId|number|
+|proceedOnWarning|boolean|
+|payload|object|
+
+## deleteLocation(locationId)
+> Delete a Location.
+```
+DELETE api/v1/locations/{locationId}
+```
+|Parameter|Type|
+|---|---|
+|locationId|number|
+
+## searchLocations(pageNumber, pageSize, payload)
+> Search for Locations by user supplied search criteria. Returns a list of Locations with the "selectedColumns" returned in the payload.
+```
+POST api/v2/quicksearch/locations payload
+```
+|Parameter|Type|
+|---|---|
+|pageNumber|number|
+|pageSize|number|
+|payload|object|
+
+## getLocationFieldList()
+> Returns a list of all Location fields.
+```
+GET api/v2/quicksearch/locations/locationListFields
+```
+*No parameters.*
```

### Comparing `dctrackclient-0.5.2/PKG-INFO` & `dctrackclient-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcTrackClient
-Version: 0.5.2
+Version: 0.6.0
 Summary: Sunbird dcTrack API client in Python
 Project-URL: Homepage, https://github.com/nicfv/dcTrackClient/
 Project-URL: Bug Tracker, https://github.com/nicfv/dcTrackClient/pulls
 Author-email: Nicolas Ventura <ventura@lbl.gov>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -20,20 +20,20 @@
 Sunbird [dcTrack](https://www.sunbirddcim.com/) API clients in Python and JavaScript
 
 ## Installation
 > dcTrackClient can be installed from the package manager of your choice.
 
 ### Python
 ```shell
-pip install dcTrackClient==0.5.2
+pip install dcTrackClient==0.6.0
 ```
 
 ### JavaScript
 ```shell
-npm i dctrackclient@0.5.2
+npm i dctrackclient@0.6.0
 ```
 
 ## Initialize a connection to the dcTrack API
 > Authentication is by using a base URL (the same URL to access the GUI) and a username and password, or a base URL and an API token.
 
 ### Python
 ```py
@@ -81,15 +81,15 @@
 });
 console.log(response);
 ```
 
 ### On Success
 This function returns the JSON object for the newly created item. This is an example response if `returnDetails` was set to false.
 ```json
-{ "item": { "id": 1234, "tiName": "item" } }
+{ "item": { "id": 1234, "tiName": "item name" } }
 ```
 
 ### On Failure
 This function returns a JSON object containing the error message.
 
 ## Retrieve item details
 > This example shows the usage of the [`getItem`](#getitemid) function.
@@ -116,20 +116,20 @@
 ```
 
 ## Modify an existing item
 > This example shows the usage of the [`updateItem`](#updateitemid-returndetails-payload) function. Any number of attributes can be included in the payload to be modified.
 
 ### Python
 ```py
-response = api.updateItem(976, False, {'tiSerialNumber': 12345})
+response = api.updateItem(1234, False, {'tiSerialNumber': 12345})
 ```
 
 ### JavaScript
 ```js
-let response = await api.updateItem(977, false, { 'tiSerialNumber': 12345 });
+let response = await api.updateItem(1234, false, { 'tiSerialNumber': 12345 });
 ```
 
 ## Search for an item
 > This example demonstrates usage of the [`searchItems`](#searchitemspagenumber-pagesize-payload) function. Follow [this guide](https://www.sunbirddcim.com/help/dcTrack/v900/API/en/Default.htm#APIGuide/v2_Advanced_Search_API.htm) for details on creating the request payload.
 
 ### Python
 ```py
@@ -246,24 +246,24 @@
 ```
 |Parameter|Type|
 |---|---|
 |pageNumber|number|
 |pageSize|number|
 |payload|object|
 
-## cabinetItems(CabinetId)
+## getCabinetItems(CabinetId)
 > Returns a list of Items contained in a Cabinet using the ItemID of the Cabinet. The returned list includes all of the Cabinet's Items including Passive Items.
 ```
 GET api/v2/items/cabinetItems/{CabinetId}
 ```
 |Parameter|Type|
 |---|---|
 |CabinetId|number|
 
-## manageItemsBulk(payload)
+## createItemsBulk(payload)
 > Add/Update/Delete Items.
 ```
 POST api/v2/dcimoperations/items/bulk payload
 ```
 |Parameter|Type|
 |---|---|
 |payload|object|
@@ -299,22 +299,23 @@
 ```
 DELETE api/v2/makes/{makeId}
 ```
 |Parameter|Type|
 |---|---|
 |makeId|number|
 
-## searchMakes(makeName)
+## searchMakes(makeName, payload)
 > Search for a make using the make name. Returns a list of makes with basic information.
 ```
-GET api/v2/dcimoperations/search/makes/{makeName}
+POST api/v2/dcimoperations/search/makes/{makeName} payload
 ```
 |Parameter|Type|
 |---|---|
 |makeName|string|
+|payload|object|
 
 ## getModel(modelId, usedCounts)
 > Get Model fields for the specified Model ID. usedCounts is an optional parameter that determines if the count of Items for the specified model is returned in the response. If set to "true" the counts will be included in the response, if omitted or set to "false" the item count will not be included in the response.
 ```
 GET api/v2/models/{modelId}
 ```
 |Parameter|Type|
@@ -388,15 +389,15 @@
 PUT api/v2/settings/connectors/{connectorId} payload
 ```
 |Parameter|Type|
 |---|---|
 |connectorId|number|
 |payload|object|
 
-## deleteConnector(payload)
+## removeConnector(payload)
 > Delete one or more Connector records.
 ```
 POST api/v2/settings/connectors/delete payload
 ```
 |Parameter|Type|
 |---|---|
 |payload|object|
@@ -509,7 +510,71 @@
 GET api/v1/items/{itemId}/powerports/{portId}/connectors/{connectorId}/isCompatible
 ```
 |Parameter|Type|
 |---|---|
 |itemId|number|
 |portId|number|
 |connectorId|number|
+
+## getLocations()
+> Returns a list for all Locations.
+```
+GET api/v1/locations
+```
+*No parameters.*
+
+## getLocation(locationId)
+> Get a single Location. Returns json containing location data for the specified ID.
+```
+GET api/v1/locations{locationId}
+```
+|Parameter|Type|
+|---|---|
+|locationId|number|
+
+## createLocation(proceedOnWarning, payload)
+> Add a Location. Returns the JSON entity containing location info that was passed in. Note: "proceedOnWarning" relates to the warning messages that are thrown in dcTrack when you try to delete custom fields that are in use. The "proceedOnWarning" value can equal either "true" or "false." If "proceedOnWarning" equals "true," business warnings will be ignored. If "proceedOnWarning" equals "false," business warnings will not be ignored.
+```
+POST api/v1/locations payload
+```
+|Parameter|Type|
+|---|---|
+|proceedOnWarning|boolean|
+|payload|object|
+
+## updateLocation(locationId, proceedOnWarning, payload)
+> Modify Location details for a single Location. Payload contains new location details. You do not have have to provide all details, but only those that you want to modify. Returns JSON entity containing Location information that was passed in from the Request payload.
+```
+PUT api/v1/locations/{locationId} payload
+```
+|Parameter|Type|
+|---|---|
+|locationId|number|
+|proceedOnWarning|boolean|
+|payload|object|
+
+## deleteLocation(locationId)
+> Delete a Location.
+```
+DELETE api/v1/locations/{locationId}
+```
+|Parameter|Type|
+|---|---|
+|locationId|number|
+
+## searchLocations(pageNumber, pageSize, payload)
+> Search for Locations by user supplied search criteria. Returns a list of Locations with the "selectedColumns" returned in the payload.
+```
+POST api/v2/quicksearch/locations payload
+```
+|Parameter|Type|
+|---|---|
+|pageNumber|number|
+|pageSize|number|
+|payload|object|
+
+## getLocationFieldList()
+> Returns a list of all Location fields.
+```
+GET api/v2/quicksearch/locations/locationListFields
+```
+*No parameters.*
```

