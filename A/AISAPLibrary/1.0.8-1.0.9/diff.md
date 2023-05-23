# Comparing `tmp/AISAPLibrary-1.0.8.tar.gz` & `tmp/AISAPLibrary-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Annas\SAP Modified\Build Wheel\AISAPLibrary\dist\.tmp-8cy6s965\AISAPLibrary-1.0.8.tar", last modified: Wed May 17 01:44:51 2023, max compression
+gzip compressed data, was "D:\Annas\SAP Modified\Build Wheel\AISAPLibrary\dist\.tmp-uanvqet_\AISAPLibrary-1.0.9.tar", last modified: Wed May 17 04:09:04 2023, max compression
```

## Comparing `AISAPLibrary-1.0.8.tar` & `AISAPLibrary-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 01:44:51.000000 AISAPLibrary-1.0.8/
--rw-rw-rw-   0        0        0      310 2023-05-17 01:44:51.000000 AISAPLibrary-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-03-13 07:56:31.000000 AISAPLibrary-1.0.8/README.md
--rw-rw-rw-   0        0        0      482 2023-05-17 01:42:12.000000 AISAPLibrary-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-17 01:44:51.000000 AISAPLibrary-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-17 01:44:51.000000 AISAPLibrary-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-17 01:44:51.000000 AISAPLibrary-1.0.8/src/AISAPLibrary/
--rw-rw-rw-   0        0        0    54413 2023-05-17 01:40:53.000000 AISAPLibrary-1.0.8/src/AISAPLibrary/AISAPLibrary.py
--rw-rw-rw-   0        0        0       38 2023-03-10 07:38:40.000000 AISAPLibrary-1.0.8/src/AISAPLibrary/__init__.py
--rw-rw-rw-   0        0        0      497 2023-05-16 03:58:34.000000 AISAPLibrary-1.0.8/src/AISAPLibrary/send_vkey_multithread.py
-drwxrwxrwx   0        0        0        0 2023-05-17 01:44:51.000000 AISAPLibrary-1.0.8/src/AISAPLibrary.egg-info/
--rw-rw-rw-   0        0        0      310 2023-05-17 01:44:51.000000 AISAPLibrary-1.0.8/src/AISAPLibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-05-17 01:44:51.000000 AISAPLibrary-1.0.8/src/AISAPLibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 01:44:51.000000 AISAPLibrary-1.0.8/src/AISAPLibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-17 01:44:51.000000 AISAPLibrary-1.0.8/src/AISAPLibrary.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 04:09:04.000000 AISAPLibrary-1.0.9/
+-rw-rw-rw-   0        0        0      310 2023-05-17 04:09:04.000000 AISAPLibrary-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-03-13 07:56:31.000000 AISAPLibrary-1.0.9/README.md
+-rw-rw-rw-   0        0        0      482 2023-05-17 04:08:34.000000 AISAPLibrary-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-17 04:09:04.000000 AISAPLibrary-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-17 04:09:04.000000 AISAPLibrary-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-17 04:09:04.000000 AISAPLibrary-1.0.9/src/AISAPLibrary/
+-rw-rw-rw-   0        0        0    54800 2023-05-17 04:07:02.000000 AISAPLibrary-1.0.9/src/AISAPLibrary/AISAPLibrary.py
+-rw-rw-rw-   0        0        0       38 2023-03-10 07:38:40.000000 AISAPLibrary-1.0.9/src/AISAPLibrary/__init__.py
+-rw-rw-rw-   0        0        0      497 2023-05-16 03:58:34.000000 AISAPLibrary-1.0.9/src/AISAPLibrary/send_vkey_multithread.py
+drwxrwxrwx   0        0        0        0 2023-05-17 04:09:04.000000 AISAPLibrary-1.0.9/src/AISAPLibrary.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-05-17 04:09:03.000000 AISAPLibrary-1.0.9/src/AISAPLibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-05-17 04:09:04.000000 AISAPLibrary-1.0.9/src/AISAPLibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 04:09:03.000000 AISAPLibrary-1.0.9/src/AISAPLibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-17 04:09:04.000000 AISAPLibrary-1.0.9/src/AISAPLibrary.egg-info/top_level.txt
```

### Comparing `AISAPLibrary-1.0.8/src/AISAPLibrary/AISAPLibrary.py` & `AISAPLibrary-1.0.9/src/AISAPLibrary/AISAPLibrary.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,14 +312,15 @@
         except com_error:
             self.take_screenshot()
             message = "Cannot send Vkey to given window, is window wnd[% s] actually open?" % window
             raise ValueError(message)
         time.sleep(self.explicit_wait)
         
     def send_vkey_other_session_process(self, vkey_id, window=0, session_num='1'):
+        ''' send vkey to other session in multithread or different process '''
         Popen(["python", os.path.dirname(os.path.realpath(__file__))+'\\send_vkey_multithread.py',self.connection_name,vkey_id,str(window),session_num])
         
     def connect_to_session(self, explicit_wait=0):
         """Connects to an open session SAP.
 
         See `Opening a connection / Before running tests` for details about requirements before connecting to a session.
 
@@ -986,29 +987,31 @@
     def close_sap(self):
         '''Fungsi untuk melakukan close SAP
         
             contoh penggunaan :
                 Close Sap
         '''
         
-        for i in range(3):
+        children_count = self.connection.children.count
+        for child_num in range(children_count):  
+            for i in range(3):
+                try:
+                    self.send_vkey_other_session(12,0,str(children_count-child_num-1))
+                except:
+                    pass
+            
             try:
-                self.send_vkey(12)
+                self.run_transaction_other_session('/nexit',str(children_count-child_num-1))
+            except:
+                pass
+            
+            try:
+                self.send_vkey_other_session(15,0,str(children_count-child_num-1))
             except:
                 pass
-        
-        try:
-            self.run_transaction('/nexit')
-        except:
-            pass
-        
-        try:
-            self.send_vkey(15)
-        except:
-            pass
         
         try:
             self.click_element('wnd[1]/usr/btnSPOP-OPTION1')
         except:
             pass
         
     def shell_content_dynamic_selection(self,shell_element=None,interactions='expand',node_num='1'):
```

