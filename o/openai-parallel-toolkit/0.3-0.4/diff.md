# Comparing `tmp/openai_parallel_toolkit-0.3-py3-none-any.whl.zip` & `tmp/openai_parallel_toolkit-0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 18368 bytes, number of entries: 19
+Zip file size: 18474 bytes, number of entries: 19
 -rw-r--r--  2.0 unx      213 b- defN 23-May-17 02:40 openai_parallel_toolkit/__init__.py
 -rw-r--r--  2.0 unx       20 b- defN 23-May-17 01:58 openai_parallel_toolkit/config.py
 -rw-r--r--  2.0 unx      113 b- defN 23-May-17 12:36 openai_parallel_toolkit/api/__init__.py
 -rw-r--r--  2.0 unx     1769 b- defN 23-May-17 12:36 openai_parallel_toolkit/api/api.py
--rw-r--r--  2.0 unx     5253 b- defN 23-May-17 12:36 openai_parallel_toolkit/api/keys.py
+-rw-r--r--  2.0 unx     5810 b- defN 23-May-23 11:48 openai_parallel_toolkit/api/keys.py
 -rw-r--r--  2.0 unx     2906 b- defN 23-May-18 11:47 openai_parallel_toolkit/api/request.py
 -rw-r--r--  2.0 unx       95 b- defN 23-May-17 01:02 openai_parallel_toolkit/core/__init__.py
 -rw-r--r--  2.0 unx     4575 b- defN 23-May-17 08:17 openai_parallel_toolkit/core/main.py
 -rw-r--r--  2.0 unx     4852 b- defN 23-May-18 11:47 openai_parallel_toolkit/core/multithread.py
 -rw-r--r--  2.0 unx      214 b- defN 23-May-17 12:36 openai_parallel_toolkit/utils/__init__.py
 -rw-r--r--  2.0 unx     1042 b- defN 23-May-18 11:32 openai_parallel_toolkit/utils/logger.py
 -rw-r--r--  2.0 unx     4114 b- defN 23-May-23 04:55 openai_parallel_toolkit/utils/reader.py
 -rw-r--r--  2.0 unx      913 b- defN 23-May-17 11:15 openai_parallel_toolkit/utils/token.py
 -rw-r--r--  2.0 unx      753 b- defN 23-May-18 11:47 openai_parallel_toolkit/utils/tqdm.py
--rw-r--r--  2.0 unx     1063 b- defN 23-May-23 04:57 openai_parallel_toolkit-0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx    13578 b- defN 23-May-23 04:57 openai_parallel_toolkit-0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-23 04:57 openai_parallel_toolkit-0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-May-23 04:57 openai_parallel_toolkit-0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1773 b- defN 23-May-23 04:57 openai_parallel_toolkit-0.3.dist-info/RECORD
-19 files, 43362 bytes uncompressed, 15390 bytes compressed:  64.5%
+-rw-r--r--  2.0 unx     1063 b- defN 23-May-23 12:01 openai_parallel_toolkit-0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13578 b- defN 23-May-23 12:01 openai_parallel_toolkit-0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-23 12:01 openai_parallel_toolkit-0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-May-23 12:01 openai_parallel_toolkit-0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1773 b- defN 23-May-23 12:01 openai_parallel_toolkit-0.4.dist-info/RECORD
+19 files, 43919 bytes uncompressed, 15496 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: openai_parallel_toolkit/utils/token.py
 Comment: 
 
 Filename: openai_parallel_toolkit/utils/tqdm.py
 Comment: 
 
-Filename: openai_parallel_toolkit-0.3.dist-info/LICENSE
+Filename: openai_parallel_toolkit-0.4.dist-info/LICENSE
 Comment: 
 
-Filename: openai_parallel_toolkit-0.3.dist-info/METADATA
+Filename: openai_parallel_toolkit-0.4.dist-info/METADATA
 Comment: 
 
-Filename: openai_parallel_toolkit-0.3.dist-info/WHEEL
+Filename: openai_parallel_toolkit-0.4.dist-info/WHEEL
 Comment: 
 
-Filename: openai_parallel_toolkit-0.3.dist-info/top_level.txt
+Filename: openai_parallel_toolkit-0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: openai_parallel_toolkit-0.3.dist-info/RECORD
+Filename: openai_parallel_toolkit-0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openai_parallel_toolkit/api/keys.py

```diff
@@ -40,24 +40,23 @@
         cls.check_key_available(cls._instance)
         return cls._instance
 
     def __init_once(self, api_keys):
         """
         Initialize the instance.
         """
-        random.shuffle(api_keys)  # Randomize the order of keys
         self._api_keys = api_keys  # Store the keys
         self._key_lock = threading.Lock()  # Lock to manage concurrent access to keys
         self._key_failure_times = {key: None for key in api_keys}  # Record the failure time of each key
         self._key_status_lock = threading.Lock()  # Lock to manage concurrent access to key status
         self._key_status = {key: True for key in api_keys}  # The initial status of each key is True (available)
-        openai.api_key = api_keys[0]  # Set the OpenAI API key to the first key in the list
+        openai.api_key = self.get_key  # Set the OpenAI API key to the first key in the list
 
     @property
-    def api_keys(self):
+    def get_key(self):
         """
         Getter for the keys, which shuffles the keys and returns the first one.
         """
         self.check_key_available()
         random.shuffle(self._api_keys)
         return self._api_keys[0]
 
@@ -67,23 +66,25 @@
         """
         with self._key_lock:
             if key in self._api_keys:
                 self._api_keys.remove(key)
                 self._key_failure_times.pop(key)
                 self._key_status.pop(key)
                 logging.warning(f"{LOG_LABEL}Removed key: {key}")
-                self.check_key_available()
-                openai.api_key = self.api_keys()
+                openai.api_key = self.get_key
+                logging.info(f"{LOG_LABEL}Switched to key: {openai.api_key}")
 
     def check_key_available(self):
         """
         Check if there is at least one key available.
         """
         if len(self._api_keys) == 0:
-            raise ValueError("No OpenAi keys available")
+            logging.error(
+                f"{LOG_LABEL} No OpenAI keys available. Please terminate the program and add keys to the config file.")
+            raise Exception("No OpenAi keys available")
 
     def switch_api_key(self, openai_model: OpenAIModel):
         """Function to switch the API key, which is called when a rate limit error is encountered"""
         with self._key_status_lock:
             self._key_status[openai.api_key] = False
         with self._key_lock:
             if self._key_status[openai.api_key]:
@@ -91,19 +92,21 @@
             try:
                 # Try generating a completion with the current key
                 completion = openai_model.generate()
                 return completion
             except Exception as e:
                 # If a rate limit error occurs
                 if "Rate limit" in str(e):
+                    logging.info(f"{LOG_LABEL}Rate limit error encountered")
                     # Record the failure time of the current key
                     self._key_failure_times[openai.api_key] = datetime.datetime.now()
                     # Find a key that hasn't failed yet
                     for key, value in self._key_failure_times.items():
                         if value is None:
+                            logging.info(f"{LOG_LABEL}Switched to key: {key}")
                             openai.api_key = key
                             return None
                     # Find keys that have been idle for at least 60 seconds
                     available_keys = [key for key, value in self._key_failure_times.items()
                                       if (datetime.datetime.now() - value).total_seconds() >= 60]
                     if available_keys:
                         # Switch to the first available key
@@ -111,13 +114,18 @@
                         logging.info(f"{LOG_LABEL}Switched to key: {openai.api_key}")
                     else:
                         # If no keys are available, find the one that will be available soonest
                         min_key, min_value = min(self._key_failure_times.items(), key=lambda item: item[1])
                         next_time = min_value + datetime.timedelta(seconds=60)
                         # Wait until the next key becomes available
                         time_to_wait = (next_time - datetime.datetime.now()).total_seconds()
+                        logging.info(
+                            f"{LOG_LABEL}Waiting for key: {min_key} to become available in {time_to_wait} seconds")
                         time.sleep(time_to_wait)
+                        logging.info(f"{LOG_LABEL}Switched to key: {min_key}")
                         openai.api_key = min_key
+                else:
+                    return None
             finally:
                 # Mark the key as available
                 with self._key_status_lock:
                     self._key_status[openai.api_key] = True
```

## Comparing `openai_parallel_toolkit-0.3.dist-info/LICENSE` & `openai_parallel_toolkit-0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `openai_parallel_toolkit-0.3.dist-info/METADATA` & `openai_parallel_toolkit-0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-parallel-toolkit
-Version: 0.3
+Version: 0.4
 Summary: OpenAI-Parallel-Toolkit is a Python library for handling multiple OpenAI API keys and parallel tasks. It provides API key rotation, multithreading for faster task execution, and utility functions to boost your OpenAI integration. Ideal for efficient large-scale OpenAI usage.
 Home-page: https://github.com/CZT0/OpenAI-Parallel-Toolkit
 Author: Jellow
 Author-email: dvdx@foxmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `openai_parallel_toolkit-0.3.dist-info/RECORD` & `openai_parallel_toolkit-0.4.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 openai_parallel_toolkit/__init__.py,sha256=GOaSwAXBRlbKqwi42SH2g6G3OOJBs_cyCTPYwv7JY6A,213
 openai_parallel_toolkit/config.py,sha256=UvWwqK1cxCx4XId6pswW4jkSF1XDozEg58RftfY8yxU,20
 openai_parallel_toolkit/api/__init__.py,sha256=eabIIe9ATUy6StxNz50Ul9Dr7iPPuc3I7ebAyGWvNLQ,113
 openai_parallel_toolkit/api/api.py,sha256=kePe00bV_6M9OL0-TvvYA_Uu65Riv4YmSr4pXVFA_E4,1769
-openai_parallel_toolkit/api/keys.py,sha256=2R4fXTCgSGH7_NksKiMTnOCdl982mi-LuMaRXJGeoho,5253
+openai_parallel_toolkit/api/keys.py,sha256=baQWRfNl3e0p1m1oem1H5GfBRhCLBSnNBaPpSZuaccY,5810
 openai_parallel_toolkit/api/request.py,sha256=zyFWK7syojup7QUK6ZCJpnMDiEoVJaCZtDCtFhwlC9w,2906
 openai_parallel_toolkit/core/__init__.py,sha256=bgIhoLSNMQAno1ICwhMfEhEZQMHqVCwEcnKvxZuXd70,95
 openai_parallel_toolkit/core/main.py,sha256=Q-8ixhJLjsg0EFDMSFJvnoaEA7O2RaoEVaGNaEFknv0,4575
 openai_parallel_toolkit/core/multithread.py,sha256=v8GPaJ7Wukxfv43i1szqreOvtCgzbK6yjh_PkiZ3qnY,4852
 openai_parallel_toolkit/utils/__init__.py,sha256=zgDb7rU1behG7hcrbLgxGOen_ojX_hUuBn5t9jnr3nk,214
 openai_parallel_toolkit/utils/logger.py,sha256=6PnPaAsBTr0PnA8tslgR0L7WSQcMZF08e8iqv-_Tvjo,1042
 openai_parallel_toolkit/utils/reader.py,sha256=UzPqVFjH5udZpyGwoeI8sk4JdJoVmn-L830xB3U4h0o,4114
 openai_parallel_toolkit/utils/token.py,sha256=lN3oasNGcHesWjoBiIfn5hMwjPYb3wTcRFUCIFtNY4k,913
 openai_parallel_toolkit/utils/tqdm.py,sha256=Xc4ymtGfZzCdbmWdqNR6bAoGDWQWOtjQqvNpvrxv-KY,753
-openai_parallel_toolkit-0.3.dist-info/LICENSE,sha256=GcBhJWMnrpUPC70Dvfs6cFG8fLIitA0WwucEgQjGWcw,1063
-openai_parallel_toolkit-0.3.dist-info/METADATA,sha256=LzYzLFDJQfgq5M3IIs7oe2eoG0O693Uk21xhrWHNyY4,13578
-openai_parallel_toolkit-0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-openai_parallel_toolkit-0.3.dist-info/top_level.txt,sha256=EaHQWFuNRtse4G2kzDTEMstiiaGFy0zIAHBJ0Mm9a_E,24
-openai_parallel_toolkit-0.3.dist-info/RECORD,,
+openai_parallel_toolkit-0.4.dist-info/LICENSE,sha256=GcBhJWMnrpUPC70Dvfs6cFG8fLIitA0WwucEgQjGWcw,1063
+openai_parallel_toolkit-0.4.dist-info/METADATA,sha256=4IZl3miOFtCgeJr7b2cAsa3b6qj1Xcr_opjA-IIbVrI,13578
+openai_parallel_toolkit-0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+openai_parallel_toolkit-0.4.dist-info/top_level.txt,sha256=EaHQWFuNRtse4G2kzDTEMstiiaGFy0zIAHBJ0Mm9a_E,24
+openai_parallel_toolkit-0.4.dist-info/RECORD,,
```

