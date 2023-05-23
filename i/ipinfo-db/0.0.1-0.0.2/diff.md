# Comparing `tmp/ipinfo_db-0.0.1-py3-none-any.whl.zip` & `tmp/ipinfo_db-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,10 @@
-Zip file size: 7641 bytes, number of entries: 11
+Zip file size: 7184 bytes, number of entries: 8
 -rw-rw-r--  2.0 unx       27 b- defN 23-May-15 06:09 ipinfo_db/__init__.py
--rw-rw-r--  2.0 unx     2158 b- defN 23-May-15 06:26 ipinfo_db/client.py
--rw-rw-r--  2.0 unx       22 b- defN 23-May-15 06:09 ipinfo_db/version.py
--rw-rw-r--  2.0 unx       27 b- defN 23-May-15 06:09 ipinfodb/__init__.py
--rw-rw-r--  2.0 unx     2157 b- defN 23-May-15 06:09 ipinfodb/client.py
--rw-rw-r--  2.0 unx       22 b- defN 23-May-15 06:09 ipinfodb/version.py
--rw-rw-r--  2.0 unx    10255 b- defN 23-May-15 06:28 ipinfo_db-0.0.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx      648 b- defN 23-May-15 06:28 ipinfo_db-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-15 06:28 ipinfo_db-0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-May-15 06:28 ipinfo_db-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      847 b- defN 23-May-15 06:28 ipinfo_db-0.0.1.dist-info/RECORD
-11 files, 16265 bytes uncompressed, 6211 bytes compressed:  61.8%
+-rw-rw-r--  2.0 unx     5647 b- defN 23-May-23 08:21 ipinfo_db/client.py
+-rw-rw-r--  2.0 unx       22 b- defN 23-May-23 08:21 ipinfo_db/version.py
+-rw-rw-r--  2.0 unx    10255 b- defN 23-May-23 08:25 ipinfo_db-0.0.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      671 b- defN 23-May-23 08:25 ipinfo_db-0.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-23 08:25 ipinfo_db-0.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-May-23 08:25 ipinfo_db-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      623 b- defN 23-May-23 08:25 ipinfo_db-0.0.2.dist-info/RECORD
+8 files, 17347 bytes uncompressed, 6096 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -3,32 +3,23 @@
 
 Filename: ipinfo_db/client.py
 Comment: 
 
 Filename: ipinfo_db/version.py
 Comment: 
 
-Filename: ipinfodb/__init__.py
+Filename: ipinfo_db-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: ipinfodb/client.py
+Filename: ipinfo_db-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: ipinfodb/version.py
+Filename: ipinfo_db-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: ipinfo_db-0.0.1.dist-info/LICENSE
+Filename: ipinfo_db-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: ipinfo_db-0.0.1.dist-info/METADATA
-Comment: 
-
-Filename: ipinfo_db-0.0.1.dist-info/WHEEL
-Comment: 
-
-Filename: ipinfo_db-0.0.1.dist-info/top_level.txt
-Comment: 
-
-Filename: ipinfo_db-0.0.1.dist-info/RECORD
+Filename: ipinfo_db-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ipinfo_db/client.py

```diff
@@ -6,60 +6,143 @@
 DB_DOWNLOAD_URL = "https://ipinfo.io/data/free/country_asn.mmdb?token="
 DEFAULT_APP_PATH = appdirs.user_data_dir(appname='ipinfo_db', appauthor='ipinfo') 
 DEFAULT_DB_PATH = os.path.join(DEFAULT_APP_PATH, 'files/country_asn.mmdb')
 
 class Client:
 
     def __init__(self, access_token=None, path=None, replace=False):
+        f'''ipinfo_db handler method.
+
+        :param access_token: Optional. Type: str. IPinfo access token to download the IP to Country ASN database required in case of data download.
+        :param path: Optional. Type: str. Download path for the database. Default is set to: {DEFAULT_DB_PATH}
+        :param replace: Optional. Type: bool. Set it to True if you want to replace your older downloaded database.
+        :return: Client handler object.
+        '''
         self.access_token = access_token
         self.path = path
         self.replace = replace
 
         if self.access_token is None and self.path is None:
             raise SyntaxError("Token or Path is required")
             
         if self.path is None:
             self.path = DEFAULT_DB_PATH
 
         # Check if file already exists to skip the download.
-        if os.path.exists(self.path) and not self.replace:
+        if os.path.isfile(self.path) and not self.replace:
             pass
         else:
             if self.access_token is None:
                 raise SyntaxError("Token is required to download the file")
             
-            # Create directory if doesn't exist and download file.
+            # Create directory if doesn't exist.
             directory = os.path.dirname(self.path)
             if directory and not os.path.exists(directory):
                 os.makedirs(directory)
-                urllib.request.urlretrieve(DB_DOWNLOAD_URL+self.access_token, self.path)
+                
+            # Download file.
+            urllib.request.urlretrieve(DB_DOWNLOAD_URL+self.access_token, self.path)
 
         # Read the mmdb file.
         self.db = maxminddb.open_database(self.path)
 
     def getDetails(self, ip):
+        '''Returns all the country and ASN level IP information available for the input IP address in a dictionary format.
+
+        :param ip: Input IP address. Supports both IPv4 and IPv6 address.
+        :return: All available country and ASN level information of the IP address.
+        :rtype: dict
+        '''
         return self.db.get(ip)
 
     def getCountry(self, ip):
+        '''Returns the ISO 3166 country code of the input.
+
+        :param ip: Input IP address. Supports both IPv4 and IPv6 address.
+        :return: Country code of the IP address.
+        :rtype: str
+        '''
         return self._get_data_field(ip, 'country')
     
     def getCountryName(self, ip):
+        '''Returns the country name of the input IP address.
+
+        :param ip: Input IP address. Supports both IPv4 and IPv6 address.
+        :return: Country name of the IP address.
+        :rtype: str
+        '''
         return self._get_data_field(ip, 'country_name')
     
     def getContinent(self, ip):
+        '''Returns the continent shortcode of the input IP address.
+
+        :param ip: Input IP address. Supports both IPv4 and IPv6 address.
+        :return: Continent code of the IP address.
+        :rtype: str
+        '''
         return self._get_data_field(ip, 'continent')
     
     def getContinentName(self, ip):
+        '''Returns the name of the continent of the input IP address.
+
+        :param ip: Input IP address. Supports both IPv4 and IPv6 address.
+        :return: Continent name of the IP address.
+        :rtype: str
+        '''
         return self._get_data_field(ip, 'continent_name')
     
     def getASN(self, ip):
+        '''Returns the ASN (Autonomous System Number) of the input IP address.
+
+        :param ip: Input IP address. Supports both IPv4 and IPv6 address.
+        :return: ASN (i.e. 	AS2381) of the IP address.
+        :rtype: str
+        '''
         return self._get_data_field(ip, 'asn')
     
     def getASNName(self, ip):
+        '''Returns the AS (Autonomous System) organization of the input ip address.
+
+        :param ip: Input IP address. Supports both IPv4 and IPv6 address.
+        :return: AS name of the IP address.
+        :rtype: str
+        '''
         return self._get_data_field(ip, 'as_name')
     
     def getASNDomain(self, ip):
+        '''Returns the domain or the official website of the input IP address.
+
+        :param ip: Input IP address. Supports both IPv4 and IPv6 address.
+        :return: Domain or website of the AS organization owning the IP address.
+        :rtype: str
+        '''
         return self._get_data_field(ip, 'as_domain')
+
+    def getCountryDetails(self, ip):
+        '''Returns the country level geolocation information of the input ip address.
+        country, country_name, continent, and continent_name
+
+        :param ip: Input IP address. Supports both IPv4 and IPv6 address.
+        :return: Country and continent information of the IP address.
+        :rtype: dict
+        '''
+        fields = ["country", "country_name", "continent", "continent_name"]
+        return self._get_data_dictionary(ip, fields)
+
+    def getASNDetails(self, ip):
+        '''Returns all the available ASN-level information of the input IP address.
+        asn, as name, and as_domain
+
+        :param ip: Input IP address. Supports both IPv4 and IPv6 address.
+        :return: ASN-level information of the IP address.
+        :rtype: dict
+        '''
+        fields = ["asn", "as_domain", "as_name"]
+        return self._get_data_dictionary(ip, fields)
     
     def _get_data_field(self, ip, field):
         data = self.db.get(ip)
         return data[field] if data else None
+
+    def _get_data_dictionary(self, ip, fields):
+        data = self.db.get(ip)
+        return {k:data[key] for key in fields if key in data}
```

## ipinfo_db/version.py

```diff
@@ -1 +1 @@
-SDK_VERSION = "0.0.1"
+SDK_VERSION = "0.0.2"
```

## Comparing `ipinfo_db-0.0.1.dist-info/LICENSE` & `ipinfo_db-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ipinfo_db-0.0.1.dist-info/METADATA` & `ipinfo_db-0.0.2.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: ipinfo-db
-Version: 0.0.1
+Version: 0.0.2
 Summary: Official Python free database library for IPinfo
 Home-page: https://github.com/ipinfo/python-db
 Author: IPinfo
 Author-email: support@ipinfo.io
 License: Apache License 2.0
 Platform: UNKNOWN
 License-File: LICENSE
+Requires-Dist: appdirs
 Requires-Dist: maxminddb
 
 
 The official Python free database library for IPinfo.
 
 IPinfo prides itself on being the most reliable, accurate, and in-depth source of IP address data available anywhere.
 We process terabytes of data to produce our custom IP geolocation, company, carrier and IP type data sets.
```

## Comparing `ipinfo_db-0.0.1.dist-info/RECORD` & `ipinfo_db-0.0.2.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 ipinfo_db/__init__.py,sha256=MF64bwUCd4sm3dvcxZnkb4ujHtxT_KeuXdD0nVieEt4,27
-ipinfo_db/client.py,sha256=qOYKjP42O2LFRwZeQlS7TOkchs5KvMPdD4gfgGpgAe0,2158
-ipinfo_db/version.py,sha256=aZbIyQe6POouZ1sCSZbG4hu13YFln93adMF700r_wKM,22
-ipinfodb/__init__.py,sha256=MF64bwUCd4sm3dvcxZnkb4ujHtxT_KeuXdD0nVieEt4,27
-ipinfodb/client.py,sha256=KC7_c_XjaBhP2GS7pamnzx-iB_XM-ybAC_mCDZ-2VOA,2157
-ipinfodb/version.py,sha256=aZbIyQe6POouZ1sCSZbG4hu13YFln93adMF700r_wKM,22
-ipinfo_db-0.0.1.dist-info/LICENSE,sha256=TRD-XzqhdrBbIpokiGa61wuDTBc_ElKoFP9HSNihODc,10255
-ipinfo_db-0.0.1.dist-info/METADATA,sha256=utQG41CzTlYmAYw8keD3UI_mm6fg-_8HFZvYpsqY_2g,648
-ipinfo_db-0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ipinfo_db-0.0.1.dist-info/top_level.txt,sha256=e16qTDTi6ccT-ZmjRO3opo1s-PUfQnF0L-l7wJ-4h-U,10
-ipinfo_db-0.0.1.dist-info/RECORD,,
+ipinfo_db/client.py,sha256=wLWigEEVZ-UJCBFD0SbFueMrUPGVWrKjOGVj1yOizns,5647
+ipinfo_db/version.py,sha256=tCyaVVl4yu5eab5T7PjyCz95_vhoiTntp2_iC2ydDcw,22
+ipinfo_db-0.0.2.dist-info/LICENSE,sha256=TRD-XzqhdrBbIpokiGa61wuDTBc_ElKoFP9HSNihODc,10255
+ipinfo_db-0.0.2.dist-info/METADATA,sha256=Qbg7_Tk8xR1MXLHt4tffBVBMNRovR7c0jlurKQW_bPs,671
+ipinfo_db-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ipinfo_db-0.0.2.dist-info/top_level.txt,sha256=e16qTDTi6ccT-ZmjRO3opo1s-PUfQnF0L-l7wJ-4h-U,10
+ipinfo_db-0.0.2.dist-info/RECORD,,
```

