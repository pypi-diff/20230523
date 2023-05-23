# Comparing `tmp/cloudmesh-vpn-4.3.4.tar.gz` & `tmp/cloudmesh-vpn-4.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudmesh-vpn-4.3.4.tar", last modified: Thu Mar 23 13:24:41 2023, max compression
+gzip compressed data, was "cloudmesh-vpn-4.3.5.tar", last modified: Tue May 23 12:37:56 2023, max compression
```

## Comparing `cloudmesh-vpn-4.3.4.tar` & `cloudmesh-vpn-4.3.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-03-23 13:24:41.922721 cloudmesh-vpn-4.3.4/
--rw-r--r--   0 grey       (502) staff       (20)      769 2021-05-21 10:48:27.000000 cloudmesh-vpn-4.3.4/LICENSE
--rw-r--r--   0 grey       (502) staff       (20)       99 2021-05-21 10:48:27.000000 cloudmesh-vpn-4.3.4/MANIFEST.in
--rw-r--r--   0 grey       (502) staff       (20)     3426 2023-03-23 13:24:41.922787 cloudmesh-vpn-4.3.4/PKG-INFO
--rw-r--r--   0 grey       (502) staff       (20)     2675 2022-09-24 14:17:45.000000 cloudmesh-vpn-4.3.4/README.md
--rw-r--r--   0 grey       (502) staff       (20)        5 2023-03-23 13:24:30.000000 cloudmesh-vpn-4.3.4/VERSION
-drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-03-23 13:24:41.921071 cloudmesh-vpn-4.3.4/cloudmesh/
--rw-r--r--   0 grey       (502) staff       (20)       63 2021-05-21 10:48:27.000000 cloudmesh-vpn-4.3.4/cloudmesh/__init__.py
-drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-03-23 13:24:41.921444 cloudmesh-vpn-4.3.4/cloudmesh/vpn/
--rw-r--r--   0 grey       (502) staff       (20)       22 2023-03-23 13:24:30.000000 cloudmesh-vpn-4.3.4/cloudmesh/vpn/__init__.py
--rw-r--r--   0 grey       (502) staff       (20)       18 2023-03-23 13:24:30.000000 cloudmesh-vpn-4.3.4/cloudmesh/vpn/__version__.py
-drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-03-23 13:24:41.921733 cloudmesh-vpn-4.3.4/cloudmesh/vpn/command/
--rw-r--r--   0 grey       (502) staff       (20)        0 2021-05-21 10:48:27.000000 cloudmesh-vpn-4.3.4/cloudmesh/vpn/command/__init__.py
--rw-r--r--   0 grey       (502) staff       (20)     1894 2022-07-21 09:21:59.000000 cloudmesh-vpn-4.3.4/cloudmesh/vpn/command/vpn.py
--rw-r--r--   0 grey       (502) staff       (20)     8234 2023-03-23 13:24:20.000000 cloudmesh-vpn-4.3.4/cloudmesh/vpn/vpn.py
-drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-03-23 13:24:41.922612 cloudmesh-vpn-4.3.4/cloudmesh_vpn.egg-info/
--rw-r--r--   0 grey       (502) staff       (20)     3426 2023-03-23 13:24:41.000000 cloudmesh-vpn-4.3.4/cloudmesh_vpn.egg-info/PKG-INFO
--rw-r--r--   0 grey       (502) staff       (20)      521 2023-03-23 13:24:41.000000 cloudmesh-vpn-4.3.4/cloudmesh_vpn.egg-info/SOURCES.txt
--rw-r--r--   0 grey       (502) staff       (20)        1 2023-03-23 13:24:41.000000 cloudmesh-vpn-4.3.4/cloudmesh_vpn.egg-info/dependency_links.txt
--rw-r--r--   0 grey       (502) staff       (20)       10 2023-03-23 13:24:41.000000 cloudmesh-vpn-4.3.4/cloudmesh_vpn.egg-info/namespace_packages.txt
--rw-r--r--   0 grey       (502) staff       (20)        1 2023-03-23 13:24:41.000000 cloudmesh-vpn-4.3.4/cloudmesh_vpn.egg-info/not-zip-safe
--rw-r--r--   0 grey       (502) staff       (20)       90 2023-03-23 13:24:41.000000 cloudmesh-vpn-4.3.4/cloudmesh_vpn.egg-info/requires.txt
--rw-r--r--   0 grey       (502) staff       (20)       10 2023-03-23 13:24:41.000000 cloudmesh-vpn-4.3.4/cloudmesh_vpn.egg-info/top_level.txt
--rw-r--r--   0 grey       (502) staff       (20)       29 2022-07-19 23:33:31.000000 cloudmesh-vpn-4.3.4/requirements-dev.txt
--rw-r--r--   0 grey       (502) staff       (20)      714 2023-03-23 13:24:20.000000 cloudmesh-vpn-4.3.4/requirements.txt
--rw-r--r--   0 grey       (502) staff       (20)       67 2023-03-23 13:24:41.922978 cloudmesh-vpn-4.3.4/setup.cfg
--rw-r--r--   0 grey       (502) staff       (20)     2815 2022-07-18 14:53:05.000000 cloudmesh-vpn-4.3.4/setup.py
+drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 12:37:56.674718 cloudmesh-vpn-4.3.5/
+-rw-r--r--   0 grey       (502) staff       (20)      769 2021-05-21 10:48:27.000000 cloudmesh-vpn-4.3.5/LICENSE
+-rw-r--r--   0 grey       (502) staff       (20)       99 2021-05-21 10:48:27.000000 cloudmesh-vpn-4.3.5/MANIFEST.in
+-rw-r--r--   0 grey       (502) staff       (20)     3405 2023-05-23 12:37:56.674785 cloudmesh-vpn-4.3.5/PKG-INFO
+-rw-r--r--   0 grey       (502) staff       (20)     2654 2023-05-23 11:59:09.000000 cloudmesh-vpn-4.3.5/README.md
+-rw-r--r--   0 grey       (502) staff       (20)        5 2023-05-23 12:37:39.000000 cloudmesh-vpn-4.3.5/VERSION
+drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 12:37:56.673004 cloudmesh-vpn-4.3.5/cloudmesh/
+-rw-r--r--   0 grey       (502) staff       (20)       63 2021-05-21 10:48:27.000000 cloudmesh-vpn-4.3.5/cloudmesh/__init__.py
+drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 12:37:56.673382 cloudmesh-vpn-4.3.5/cloudmesh/vpn/
+-rw-r--r--   0 grey       (502) staff       (20)       22 2023-05-23 12:37:39.000000 cloudmesh-vpn-4.3.5/cloudmesh/vpn/__init__.py
+-rw-r--r--   0 grey       (502) staff       (20)       18 2023-05-23 12:37:39.000000 cloudmesh-vpn-4.3.5/cloudmesh/vpn/__version__.py
+drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 12:37:56.673601 cloudmesh-vpn-4.3.5/cloudmesh/vpn/command/
+-rw-r--r--   0 grey       (502) staff       (20)        0 2021-05-21 10:48:27.000000 cloudmesh-vpn-4.3.5/cloudmesh/vpn/command/__init__.py
+-rw-r--r--   0 grey       (502) staff       (20)     2640 2023-05-23 12:37:21.000000 cloudmesh-vpn-4.3.5/cloudmesh/vpn/command/vpn.py
+-rw-r--r--   0 grey       (502) staff       (20)     8776 2023-05-23 12:31:19.000000 cloudmesh-vpn-4.3.5/cloudmesh/vpn/vpn.py
+drwxr-xr-x   0 grey       (502) staff       (20)        0 2023-05-23 12:37:56.674591 cloudmesh-vpn-4.3.5/cloudmesh_vpn.egg-info/
+-rw-r--r--   0 grey       (502) staff       (20)     3405 2023-05-23 12:37:56.000000 cloudmesh-vpn-4.3.5/cloudmesh_vpn.egg-info/PKG-INFO
+-rw-r--r--   0 grey       (502) staff       (20)      521 2023-05-23 12:37:56.000000 cloudmesh-vpn-4.3.5/cloudmesh_vpn.egg-info/SOURCES.txt
+-rw-r--r--   0 grey       (502) staff       (20)        1 2023-05-23 12:37:56.000000 cloudmesh-vpn-4.3.5/cloudmesh_vpn.egg-info/dependency_links.txt
+-rw-r--r--   0 grey       (502) staff       (20)       10 2023-05-23 12:37:56.000000 cloudmesh-vpn-4.3.5/cloudmesh_vpn.egg-info/namespace_packages.txt
+-rw-r--r--   0 grey       (502) staff       (20)        1 2023-05-23 12:37:56.000000 cloudmesh-vpn-4.3.5/cloudmesh_vpn.egg-info/not-zip-safe
+-rw-r--r--   0 grey       (502) staff       (20)       90 2023-05-23 12:37:56.000000 cloudmesh-vpn-4.3.5/cloudmesh_vpn.egg-info/requires.txt
+-rw-r--r--   0 grey       (502) staff       (20)       10 2023-05-23 12:37:56.000000 cloudmesh-vpn-4.3.5/cloudmesh_vpn.egg-info/top_level.txt
+-rw-r--r--   0 grey       (502) staff       (20)       29 2022-07-19 23:33:31.000000 cloudmesh-vpn-4.3.5/requirements-dev.txt
+-rw-r--r--   0 grey       (502) staff       (20)      714 2023-03-23 13:24:20.000000 cloudmesh-vpn-4.3.5/requirements.txt
+-rw-r--r--   0 grey       (502) staff       (20)       67 2023-05-23 12:37:56.675212 cloudmesh-vpn-4.3.5/setup.cfg
+-rw-r--r--   0 grey       (502) staff       (20)     2815 2022-07-18 14:53:05.000000 cloudmesh-vpn-4.3.5/setup.py
```

### Comparing `cloudmesh-vpn-4.3.4/LICENSE` & `cloudmesh-vpn-4.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudmesh-vpn-4.3.4/PKG-INFO` & `cloudmesh-vpn-4.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudmesh-vpn
-Version: 4.3.4
+Version: 4.3.5
 Summary: A command called vpn and foo for the cloudmesh shell
 Home-page: https://github.com/cloudmesh/cloudmesh-vpn
 Author: Gregor von Laszewski
 Author-email: laszewski@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -18,16 +18,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cms vpn
 
 ## Windows
 
-This requires installation of the Cisco AnyConnect
-Secure Mobility Client located at <https://in.virginia.edu/vpn>.
+This requires installation of the Cisco
+Secure Client located at <https://in.virginia.edu/vpn>.
 
 To connect to the UVA Anywhere VPN, run
 
 ```bash
 cms vpn connect
 ```
 
@@ -43,15 +43,15 @@
 cms vpn info
 ```
 
 ## Linux
 
 ### Requirements
 
-On Linux we use the comamnd `openconnect`. To check if it is available please use
+On Linux we use the command `openconnect`. To check if it is available please use
 
 ```bash
 $ which openconnect
 ```
 
 If it is not available, you can install it un Ubuntu with 
 
@@ -72,34 +72,34 @@
 We have tested this tool only with University of Virginia, but it should be simple to adapt. Just follow the 
 instructions to obtain the certificates from your provider.
 
 At UVA you find the certificate and other documentation at 
 
 * <https://www.rc.virginia.edu/userinfo/linux/uva-anywhere-vpn-linux/>
 
-we place all certifcates into ~/.ssh/uva
+we place all certificates into ~/.ssh/uva
 
 ```
 mkdir -p You will receive a file ending in .p12. In this example we will assume it is named mst3k.p12.
 cd ~/.ssh/uva
 wget https://download.its.virginia.edu/local-auth/universal/usher.cer
 ```
 
 To get a certificate for your device, go to 
 
 * <https://cloud.securew2.com/public/82116/limited/?device=Unknown>
 
 Fill it out and get the key. You will receive a 
 file ending in .p12. In this example we will assume it 
-is named mst3k.p12 and palce it into ~/.ssh/uva/user.p12
+is named mst3k.p12 and place it into ~/.ssh/uva/user.p12
 
 It is important for us to rename this key to user.p12
-so we have a simplere way of identifying it and writing this documentation.
+so we have a simpler way of identifying it and writing this documentation.
 
-Now converte the keys and certificates with the following commands
+Now convert the keys and certificates with the following commands
 
 ```bash
 cd ~/.ssh/uva
 openssl pkcs12 -in mst3k.p12 -nocerts -nodes -out mst3k.key
 openssl pkcs12 -in mst3k.p12 -clcerts -nokeys -out mst3k.crt
 openssl x509 -inform DER -in usher.cer -out usher.crt
 ```
@@ -133,18 +133,18 @@
 To show the status use
 
 ```bash
 $ cms vpn connect 
 ```
 
 
-To diconnect
+To disconnect
 
 ```bash
 $ cms vpn disconnect
 ```
 
 ## Acknowledgments
 
 This work was in part funded by the NSF
 CyberTraining: CIC: CyberTraining for Students and Technologies
-from Generation Z with the awadrd numbers 1829704 and 2200409.
+from Generation Z with the award numbers 1829704 and 2200409.
```

### Comparing `cloudmesh-vpn-4.3.4/README.md` & `cloudmesh-vpn-4.3.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # cms vpn
 
 ## Windows
 
-This requires installation of the Cisco AnyConnect
-Secure Mobility Client located at <https://in.virginia.edu/vpn>.
+This requires installation of the Cisco
+Secure Client located at <https://in.virginia.edu/vpn>.
 
 To connect to the UVA Anywhere VPN, run
 
 ```bash
 cms vpn connect
 ```
 
@@ -23,15 +23,15 @@
 cms vpn info
 ```
 
 ## Linux
 
 ### Requirements
 
-On Linux we use the comamnd `openconnect`. To check if it is available please use
+On Linux we use the command `openconnect`. To check if it is available please use
 
 ```bash
 $ which openconnect
 ```
 
 If it is not available, you can install it un Ubuntu with 
 
@@ -52,34 +52,34 @@
 We have tested this tool only with University of Virginia, but it should be simple to adapt. Just follow the 
 instructions to obtain the certificates from your provider.
 
 At UVA you find the certificate and other documentation at 
 
 * <https://www.rc.virginia.edu/userinfo/linux/uva-anywhere-vpn-linux/>
 
-we place all certifcates into ~/.ssh/uva
+we place all certificates into ~/.ssh/uva
 
 ```
 mkdir -p You will receive a file ending in .p12. In this example we will assume it is named mst3k.p12.
 cd ~/.ssh/uva
 wget https://download.its.virginia.edu/local-auth/universal/usher.cer
 ```
 
 To get a certificate for your device, go to 
 
 * <https://cloud.securew2.com/public/82116/limited/?device=Unknown>
 
 Fill it out and get the key. You will receive a 
 file ending in .p12. In this example we will assume it 
-is named mst3k.p12 and palce it into ~/.ssh/uva/user.p12
+is named mst3k.p12 and place it into ~/.ssh/uva/user.p12
 
 It is important for us to rename this key to user.p12
-so we have a simplere way of identifying it and writing this documentation.
+so we have a simpler way of identifying it and writing this documentation.
 
-Now converte the keys and certificates with the following commands
+Now convert the keys and certificates with the following commands
 
 ```bash
 cd ~/.ssh/uva
 openssl pkcs12 -in mst3k.p12 -nocerts -nodes -out mst3k.key
 openssl pkcs12 -in mst3k.p12 -clcerts -nokeys -out mst3k.crt
 openssl x509 -inform DER -in usher.cer -out usher.crt
 ```
@@ -113,18 +113,18 @@
 To show the status use
 
 ```bash
 $ cms vpn connect 
 ```
 
 
-To diconnect
+To disconnect
 
 ```bash
 $ cms vpn disconnect
 ```
 
 ## Acknowledgments
 
 This work was in part funded by the NSF
 CyberTraining: CIC: CyberTraining for Students and Technologies
-from Generation Z with the awadrd numbers 1829704 and 2200409.
+from Generation Z with the award numbers 1829704 and 2200409.
```

### Comparing `cloudmesh-vpn-4.3.4/cloudmesh/vpn/command/vpn.py` & `cloudmesh-vpn-4.3.5/cloudmesh/vpn/command/vpn.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,30 +9,53 @@
     # noinspection PyUnusedLocal
     @command
     def do_vpn(self, args, arguments):
         """
         ::
 
           Usage:
-                vpn connect [--service=SERVICE] [-v]
+                vpn connect [--service=SERVICE] [--timeout=TIMEOUT] [-v]
                 vpn disconnect [-v]
                 vpn status [-v]
                 vpn info
 
           This command manages the von connection
 
           Options:
               -v      debug [default: False]
 
+          Description:
+            vpn info
+               prints out information about your current location as
+               obtained via the vpn connection.
+
+            vpn status
+                prints out "True" if the vpn is connected
+                and "False" if it is not.
+
+            vpn disconnect
+                disconnects from the VPN.
+
+            vpn connect
+                connects to the UVA Anywhere VPN.
+
+                If the VPN is already connected a warning is shown.
+
+                You can connect to other VPNs while specifying their names
+                as given to you by the VPN provider with e service option.
+
+
         """
 
-        map_parameters(arguments, "service")
+        map_parameters(arguments, "service", "timeout")
 
         from cloudmesh.vpn.vpn import Vpn
-        vpn = Vpn(arguments.service, debug=arguments["-v"])
+        vpn = Vpn(arguments.service,
+                  timeout=arguments.timeout,
+                  debug=arguments["-v"])
 
         if arguments.connect:
             Console.ok("Connecting ... ")
             vpn.connect()
             if vpn.enabled():
                 Console.ok("ok")
             else:
```

### Comparing `cloudmesh-vpn-4.3.4/cloudmesh/vpn/vpn.py` & `cloudmesh-vpn-4.3.5/cloudmesh/vpn/vpn.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from cloudmesh.common.systeminfo import os_is_linux
 from cloudmesh.common.systeminfo import os_is_mac
 from cloudmesh.common.systeminfo import os_is_windows
 
 if os_is_windows():
     import pyuac
 
+# mac /opt/cisco/secureclient/bin/vpn
 # mac: /opt/cisco/anyconnect/bin
 
 # windows
 # $ 'C:\Program Files (x86)\Cisco\Cisco AnyConnect Secure Mobility Client\vpncli.exe'
 # Cisco AnyConnect Secure Mobility Client (version 4.10.05095) .
 #
 # Copyright (c) 2004 - 2022 Cisco Systems, Inc.  All Rights Reserved.
@@ -42,20 +43,33 @@
 # more security:
 #   /opt/cisco/anyconnect/bin/vpn connect "UVA More Secure Network";
 # close:
 #   /opt/cisco/anyconnect/bin/vpn disconnect;
 
 class Vpn:
 
-    def __init__(self, service=None, debug=False):
+    def __init__(self,
+                 service=None,
+                 timeout=None,
+                 debug=False):
+
+        if timeout is None:
+            self.timeout = 60
 
         if os_is_windows():
-            self.anyconnect = r'C:\Program Files (x86)\Cisco\Cisco AnyConnect Secure Mobility Client\vpncli.exe'
+            self.anyconnect = r'C:\Program Files (x86)\Cisco\Cisco Secure Client\vpncli.exe'
         elif os_is_mac():
-            self.anyconnect = "/opt/cisco/anyconnect/bin/vpn"
+            self.anyconnect = None
+            for command in ["/opt/cisco/anyconnect/bin/vpn",
+                            "/opt/cisco/secureclient/bin/vpn"]:
+                if os.path.isfile(command):
+                    self.anyconnect = command
+                    break;
+            if self.anyconnect is None:
+                raise NotImplementedError("vpn cCLI not found")
         elif os_is_linux():
             self.anyconnect = "/opt/cisco/anyconnect/bin/vpn"
         else:
             raise NotImplementedError("OS is not yet supported for anyconnect")
 
         self.debug = debug
         if service is None or service == "uva":
@@ -71,15 +85,15 @@
     def enabled(self=None):
         state = False
         result = ""
         if os_is_windows():
             result = Shell.run("route print").strip()
             state = "Cisco AnyConnect" in result
         elif os_is_mac():
-            command = f'echo state | /opt/cisco/anyconnect/bin/vpn -s'
+            command = f'echo state | {self.anyconnect} -s'
             result = Shell.run(command)
             state = "state: Connected" in result
         elif os_is_linux():
             result = requests.get("https://ipinfo.io")
             state = "University of Virginia" in result.json()["org"]
         if self:
             Vpn._debug(self, result)
@@ -119,29 +133,37 @@
             while not service_started:
                 r = pexpect.popen_spawn.PopenSpawn(mycommand)
                 r.timeout = 3
                 sys.stdout.reconfigure(encoding='utf-8')
                 r.logfile = sys.stdout.buffer
                 result = r.expect([pexpect.TIMEOUT,
                                    r"^.*accept.*$",
-                                   r"^.*Another AnyConnect application.*$",
-                                   r"^.*The VPN Service is not available.*$",
+                                   r"^.*Another Cisco Secure Client.*$",
+                                   r"^.*VPN service is unavailable.*$",
                                    pexpect.EOF])
                 if result in [0, 2, 3]:
                     Console.warning('Restarting vpnagent to avoid conflict')
+
+                    try:
+                        r = os.system('taskkill /im vpnagent.exe /F')
+                    except:
+                        pass
+
                     try:
-                        r = Shell.run('net stop vpnagent')
+                        r = Shell.run('net stop csc_vpnagent')
                     except:
                         pass
+
                     try:
-                        r = Shell.run('net start vpnagent')
+                        r = Shell.run('net start csc_vpnagent')
                     except:
                         pass
+
                     try:
-                        r = os.system('taskkill /im vpnui.exe /F')
+                        r = os.system('taskkill /im csc_ui.exe /F')
                     except:
                         pass
 
                 if result == 1:
                     service_started = True
                     r.sendline('y')
                     result2 = r.expect([pexpect.TIMEOUT, "^.*Connected.*$", pexpect.EOF])
@@ -151,15 +173,15 @@
 
         elif os_is_mac():
 
             mycommand = rf'{self.anyconnect} connect "UVA Anywhere"'
             service_started = False
             while not service_started:
                 r = pexpect.spawn(mycommand)
-                r.timeout = 3
+                r.timeout = self.timeout
                 sys.stdout.reconfigure(encoding='utf-8')
                 r.logfile = sys.stdout.buffer
                 result = r.expect([pexpect.TIMEOUT,
                                    r"^.*accept.*$",
                                    r"^.*Another AnyConnect application.*$",
                                    r"^.*The VPN Service is not available.*$",
                                    pexpect.EOF])
@@ -201,27 +223,27 @@
 
     def disconnect(self):
         if not self.enabled():
             Console.warning("VPN is already deactivated")
             return ""
 
         if os_is_windows():
-            mycommand = fr'C:\Program Files (x86)\Cisco\Cisco AnyConnect Secure Mobility Client\vpncli.exe disconnect "{self.service}"'
+            mycommand = fr'{self.anyconnect} disconnect "{self.service}"'
             # mycommand = mycommand.replace("\\", "/")
             r = pexpect.popen_spawn.PopenSpawn(mycommand)
             sys.stdout.reconfigure(encoding='utf-8')
             r.logfile = sys.stdout.buffer
             # time.sleep(5)
             # r.sendline('y')
 
             result = r.expect([pexpect.TIMEOUT, r"^.*Disconnected.*$", pexpect.EOF])
             if result == 1:
                 Console.ok('Successfully disconnected')
         elif os_is_mac():
-            command = f'/opt/cisco/anyconnect/bin/vpn disconnect "{self.service}"'
+            command = f'{self.anyconnect} disconnect "{self.service}"'
             result = Shell.run(command)
         elif os_is_linux():
             from cloudmesh.common.sudo import Sudo
             Sudo.password()
 
             command = f'sudo pkill -SIGINT openconnect &> /dev/null'
             result = Shell.run(command)
```

### Comparing `cloudmesh-vpn-4.3.4/cloudmesh_vpn.egg-info/PKG-INFO` & `cloudmesh-vpn-4.3.5/cloudmesh_vpn.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudmesh-vpn
-Version: 4.3.4
+Version: 4.3.5
 Summary: A command called vpn and foo for the cloudmesh shell
 Home-page: https://github.com/cloudmesh/cloudmesh-vpn
 Author: Gregor von Laszewski
 Author-email: laszewski@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -18,16 +18,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cms vpn
 
 ## Windows
 
-This requires installation of the Cisco AnyConnect
-Secure Mobility Client located at <https://in.virginia.edu/vpn>.
+This requires installation of the Cisco
+Secure Client located at <https://in.virginia.edu/vpn>.
 
 To connect to the UVA Anywhere VPN, run
 
 ```bash
 cms vpn connect
 ```
 
@@ -43,15 +43,15 @@
 cms vpn info
 ```
 
 ## Linux
 
 ### Requirements
 
-On Linux we use the comamnd `openconnect`. To check if it is available please use
+On Linux we use the command `openconnect`. To check if it is available please use
 
 ```bash
 $ which openconnect
 ```
 
 If it is not available, you can install it un Ubuntu with 
 
@@ -72,34 +72,34 @@
 We have tested this tool only with University of Virginia, but it should be simple to adapt. Just follow the 
 instructions to obtain the certificates from your provider.
 
 At UVA you find the certificate and other documentation at 
 
 * <https://www.rc.virginia.edu/userinfo/linux/uva-anywhere-vpn-linux/>
 
-we place all certifcates into ~/.ssh/uva
+we place all certificates into ~/.ssh/uva
 
 ```
 mkdir -p You will receive a file ending in .p12. In this example we will assume it is named mst3k.p12.
 cd ~/.ssh/uva
 wget https://download.its.virginia.edu/local-auth/universal/usher.cer
 ```
 
 To get a certificate for your device, go to 
 
 * <https://cloud.securew2.com/public/82116/limited/?device=Unknown>
 
 Fill it out and get the key. You will receive a 
 file ending in .p12. In this example we will assume it 
-is named mst3k.p12 and palce it into ~/.ssh/uva/user.p12
+is named mst3k.p12 and place it into ~/.ssh/uva/user.p12
 
 It is important for us to rename this key to user.p12
-so we have a simplere way of identifying it and writing this documentation.
+so we have a simpler way of identifying it and writing this documentation.
 
-Now converte the keys and certificates with the following commands
+Now convert the keys and certificates with the following commands
 
 ```bash
 cd ~/.ssh/uva
 openssl pkcs12 -in mst3k.p12 -nocerts -nodes -out mst3k.key
 openssl pkcs12 -in mst3k.p12 -clcerts -nokeys -out mst3k.crt
 openssl x509 -inform DER -in usher.cer -out usher.crt
 ```
@@ -133,18 +133,18 @@
 To show the status use
 
 ```bash
 $ cms vpn connect 
 ```
 
 
-To diconnect
+To disconnect
 
 ```bash
 $ cms vpn disconnect
 ```
 
 ## Acknowledgments
 
 This work was in part funded by the NSF
 CyberTraining: CIC: CyberTraining for Students and Technologies
-from Generation Z with the awadrd numbers 1829704 and 2200409.
+from Generation Z with the award numbers 1829704 and 2200409.
```

### Comparing `cloudmesh-vpn-4.3.4/cloudmesh_vpn.egg-info/SOURCES.txt` & `cloudmesh-vpn-4.3.5/cloudmesh_vpn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudmesh-vpn-4.3.4/requirements.txt` & `cloudmesh-vpn-4.3.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `cloudmesh-vpn-4.3.4/setup.py` & `cloudmesh-vpn-4.3.5/setup.py`

 * *Files identical despite different names*

