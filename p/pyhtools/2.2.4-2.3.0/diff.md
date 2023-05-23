# Comparing `tmp/pyhtools-2.2.4.tar.gz` & `tmp/pyhtools-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhtools-2.2.4.tar", max compression
+gzip compressed data, was "pyhtools-2.3.0.tar", max compression
```

## Comparing `pyhtools-2.2.4.tar` & `pyhtools-2.3.0.tar`

### file list

```diff
@@ -1,73 +1,43 @@
--rw-r--r--   0        0        0     1076 2023-05-20 13:10:37.960043 pyhtools-2.2.4/LICENSE
--rw-r--r--   0        0        0     6823 2023-05-20 13:10:37.960043 pyhtools-2.2.4/README.md
--rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/UI/__init__.py
--rw-r--r--   0        0        0      283 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/UI/colors.py
--rw-r--r--   0        0        0     6464 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/UI/functions.py
--rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/__init__.py
--rw-r--r--   0        0        0      286 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/__main__.py
--rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Android/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Android/forensics/__init__.py
--rw-r--r--   0        0        0     2876 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Android/forensics/data_harvester.py
--rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Android/mitm/__init__.py
--rw-r--r--   0        0        0     6596 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Android/mitm/cert_pin.py
--rw-r--r--   0        0        0      563 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Android/mitm/utils.py
--rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Network/__init__.py
--rw-r--r--   0        0        0     6629 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Network/arpspoofer.py
--rw-r--r--   0        0        0     4868 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Network/code_injector.py
--rw-r--r--   0        0        0     3726 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Network/dnsspoofer.py
--rw-r--r--   0        0        0     5075 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Network/downloads_replacer.py
--rw-r--r--   0        0        0     4580 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Network/machngr.py
--rw-r--r--   0        0        0     2552 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Network/network_jammer.py
--rw-r--r--   0        0        0     2177 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Network/nwscan.py
--rw-r--r--   0        0        0     2831 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Network/pkt_sniffer.py
--rw-r--r--   0        0        0     7372 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/Network/tcp_proxy.py
--rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/__init__.py
--rw-r--r--   0        0        0     4669 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/attackers.py
--rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/web/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/web/api/__init__.py
--rw-r--r--   0        0        0     6643 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/web/api/discover.py
--rw-r--r--   0        0        0     3012 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/web/enumerate.py
--rw-r--r--   0        0        0     2141 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/web/get_forms.py
--rw-r--r--   0        0        0     1357 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/web/login_guesser.py
--rw-r--r--   0        0        0     3403 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/web/spider.py
--rw-r--r--   0        0        0     4529 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/web/utils.py
--rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/web/vuln_scanner/__init__.py
--rw-r--r--   0        0        0     2901 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/web/vuln_scanner/__main__.py
--rw-r--r--   0        0        0     7036 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/web/vuln_scanner/scanner.py
--rw-r--r--   0        0        0     2132 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/attackers/web/vuln_scanner/sqli.py
--rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/detectors/__init__.py
--rw-r--r--   0        0        0     2254 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/detectors/arp_spoof_detector.py
--rw-r--r--   0        0        0     1757 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/detectors/win_block_usb.py
--rw-r--r--   0        0        0     4132 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/evil_files/exec_generator.py
--rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/evil_files/malwares/__init__.py
--rw-r--r--   0        0        0     3352 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/evil_files/malwares/backdoor/ssh/backdoor.py
--rw-r--r--   0        0        0     2272 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/evil_files/malwares/backdoor/ssh/handler.py
--rw-r--r--   0        0        0     1850 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/evil_files/malwares/data_harvesters/credential_harvester.py
--rw-r--r--   0        0        0     1632 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/evil_files/malwares/data_harvesters/ssh_cred_harvester.py
--rw-r--r--   0        0        0     4868 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/evil_files/malwares/data_harvesters/telegram_data_harvester.py
--rw-r--r--   0        0        0     2230 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/evil_files/malwares/data_harvesters/wireless_password_harvester.py
--rw-r--r--   0        0        0        0 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/evil_files/malwares/installer/__init__.py
--rw-r--r--   0        0        0     1566 2023-05-20 13:10:37.960043 pyhtools-2.2.4/pyhtools/evil_files/malwares/installer/cert.py
--rw-r--r--   0        0        0        0 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/keylogger/__init__.py
--rw-r--r--   0        0        0     2599 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/keylogger/keylogger.py
--rw-r--r--   0        0        0        0 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/__init__.py
--rw-r--r--   0        0        0     1338 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/backdoor.py
--rw-r--r--   0        0        0     1147 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/reverse_backdoor/HTTP/listener.py
--rw-r--r--   0        0        0        0 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/reverse_backdoor/TCP/__init__.py
--rw-r--r--   0        0        0     5247 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/reverse_backdoor/TCP/listener.py
--rw-r--r--   0        0        0     5727 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/reverse_backdoor/TCP/reverse_backdoor.py
--rw-r--r--   0        0        0        0 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/reverse_backdoor/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/reverse_backdoor/ssh/__init__.py
--rw-r--r--   0        0        0     5015 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/reverse_backdoor/ssh/backdoor.py
--rw-r--r--   0        0        0     4349 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/telegram_remote_code_executor/TelegramRemoteCodeExecutor.py
--rw-r--r--   0        0        0        0 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/telegram_remote_code_executor/__init__.py
--rw-r--r--   0        0        0     2589 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/malwares/utils.py
--rw-r--r--   0        0        0        0 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/ransomwares/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/ransomwares/dmsec/__init__.py
--rw-r--r--   0        0        0     2130 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/ransomwares/dmsec/decrypter.py
--rw-r--r--   0        0        0     2242 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/ransomwares/dmsec/encrypter.py
--rw-r--r--   0        0        0        0 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/worms/__init__.py
--rw-r--r--   0        0        0     3857 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/evil_files/worms/dir_cloner.py
--rw-r--r--   0        0        0      710 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyhtools/utils.py
--rw-r--r--   0        0        0     1822 2023-05-20 13:10:37.964043 pyhtools-2.2.4/pyproject.toml
--rw-r--r--   0        0        0     9119 1970-01-01 00:00:00.000000 pyhtools-2.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-23 09:21:19.144008 pyhtools-2.3.0/LICENSE
+-rw-r--r--   0        0        0     7109 2023-05-23 09:21:19.144008 pyhtools-2.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/UI/__init__.py
+-rw-r--r--   0        0        0      283 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/UI/colors.py
+-rw-r--r--   0        0        0     6464 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/UI/functions.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/__init__.py
+-rw-r--r--   0        0        0      286 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/Android/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/Android/forensics/__init__.py
+-rw-r--r--   0        0        0     2876 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/Android/forensics/data_harvester.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/Android/mitm/__init__.py
+-rw-r--r--   0        0        0     6596 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/Android/mitm/cert_pin.py
+-rw-r--r--   0        0        0      563 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/Android/mitm/utils.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/Network/__init__.py
+-rw-r--r--   0        0        0     6629 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/Network/arpspoofer.py
+-rw-r--r--   0        0        0     4868 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/Network/code_injector.py
+-rw-r--r--   0        0        0     3726 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/Network/dnsspoofer.py
+-rw-r--r--   0        0        0     5075 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/Network/downloads_replacer.py
+-rw-r--r--   0        0        0     4580 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/Network/machngr.py
+-rw-r--r--   0        0        0     2552 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/Network/network_jammer.py
+-rw-r--r--   0        0        0     2177 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/Network/nwscan.py
+-rw-r--r--   0        0        0     2831 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/Network/pkt_sniffer.py
+-rw-r--r--   0        0        0     7372 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/Network/tcp_proxy.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/__init__.py
+-rw-r--r--   0        0        0     4669 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/attackers.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/web/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/web/api/__init__.py
+-rw-r--r--   0        0        0     6643 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/web/api/discover.py
+-rw-r--r--   0        0        0     3012 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/web/enumerate.py
+-rw-r--r--   0        0        0     2141 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/web/get_forms.py
+-rw-r--r--   0        0        0     1357 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/web/login_guesser.py
+-rw-r--r--   0        0        0     3403 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/web/spider.py
+-rw-r--r--   0        0        0     4529 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/web/utils.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/web/vuln_scanner/__init__.py
+-rw-r--r--   0        0        0     2901 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/web/vuln_scanner/__main__.py
+-rw-r--r--   0        0        0     7036 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/web/vuln_scanner/scanner.py
+-rw-r--r--   0        0        0     2132 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/attackers/web/vuln_scanner/sqli.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/detectors/__init__.py
+-rw-r--r--   0        0        0     2254 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/detectors/arp_spoof_detector.py
+-rw-r--r--   0        0        0     1757 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/detectors/win_block_usb.py
+-rw-r--r--   0        0        0      710 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyhtools/utils.py
+-rw-r--r--   0        0        0     1822 2023-05-23 09:21:19.144008 pyhtools-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9405 1970-01-01 00:00:00.000000 pyhtools-2.3.0/PKG-INFO
```

### Comparing `pyhtools-2.2.4/LICENSE` & `pyhtools-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/README.md` & `pyhtools-2.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,21 @@
 
 ## Disclaimer
 
 The disclaimer advises users to use the open source project for ethical and legitimate purposes only and refrain from using it for any malicious activities. The creators and contributors of the project are not responsible for any illegal activities or damages that may arise from the misuse of the project. Users are solely responsible for their use of the project and should exercise caution and diligence when using it. Any unauthorized or malicious use of the project may result in legal action and other consequences.
 
 [Read More](./DISCLAIMER.md)
 
+### Notice
+
+To comply with PyPi's [Acceptable Use Policy](https://pypi.org/policy/acceptable-use-policy/)
+
+All Evil files are moved to another repository: [pyhtools-evil-files](https://github.com/dmdhrumilmistry/pyhtools-evil-files)
+
+Never use provided resources for malicious purpose.
 
 ## Join Our Discord Community
 
 [![Join our Discord server!](https://invidget.switchblade.xyz/DJrnAg4nv2)](http://discord.gg/DJrnAg4nv2)
 
 ## How To Videos
```

### Comparing `pyhtools-2.2.4/pyhtools/UI/functions.py` & `pyhtools-2.3.0/pyhtools/UI/functions.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/attackers/Android/forensics/data_harvester.py` & `pyhtools-2.3.0/pyhtools/attackers/Android/forensics/data_harvester.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/attackers/Android/mitm/cert_pin.py` & `pyhtools-2.3.0/pyhtools/attackers/Android/mitm/cert_pin.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/attackers/Android/mitm/utils.py` & `pyhtools-2.3.0/pyhtools/attackers/Android/mitm/utils.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/attackers/Network/arpspoofer.py` & `pyhtools-2.3.0/pyhtools/attackers/Network/arpspoofer.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/attackers/Network/code_injector.py` & `pyhtools-2.3.0/pyhtools/attackers/Network/code_injector.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/attackers/Network/dnsspoofer.py` & `pyhtools-2.3.0/pyhtools/attackers/Network/dnsspoofer.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/attackers/Network/downloads_replacer.py` & `pyhtools-2.3.0/pyhtools/attackers/Network/downloads_replacer.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/attackers/Network/machngr.py` & `pyhtools-2.3.0/pyhtools/attackers/Network/machngr.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/attackers/Network/network_jammer.py` & `pyhtools-2.3.0/pyhtools/attackers/Network/network_jammer.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/attackers/Network/nwscan.py` & `pyhtools-2.3.0/pyhtools/attackers/Network/nwscan.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/attackers/Network/pkt_sniffer.py` & `pyhtools-2.3.0/pyhtools/attackers/Network/pkt_sniffer.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/attackers/Network/tcp_proxy.py` & `pyhtools-2.3.0/pyhtools/attackers/Network/tcp_proxy.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/attackers/attackers.py` & `pyhtools-2.3.0/pyhtools/attackers/attackers.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/attackers/web/api/discover.py` & `pyhtools-2.3.0/pyhtools/attackers/web/api/discover.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/attackers/web/enumerate.py` & `pyhtools-2.3.0/pyhtools/attackers/web/enumerate.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/attackers/web/get_forms.py` & `pyhtools-2.3.0/pyhtools/attackers/web/get_forms.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/attackers/web/login_guesser.py` & `pyhtools-2.3.0/pyhtools/attackers/web/login_guesser.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/attackers/web/spider.py` & `pyhtools-2.3.0/pyhtools/attackers/web/spider.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/attackers/web/utils.py` & `pyhtools-2.3.0/pyhtools/attackers/web/utils.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/attackers/web/vuln_scanner/__main__.py` & `pyhtools-2.3.0/pyhtools/attackers/web/vuln_scanner/__main__.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/attackers/web/vuln_scanner/scanner.py` & `pyhtools-2.3.0/pyhtools/attackers/web/vuln_scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/attackers/web/vuln_scanner/sqli.py` & `pyhtools-2.3.0/pyhtools/attackers/web/vuln_scanner/sqli.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/detectors/arp_spoof_detector.py` & `pyhtools-2.3.0/pyhtools/detectors/arp_spoof_detector.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/detectors/win_block_usb.py` & `pyhtools-2.3.0/pyhtools/detectors/win_block_usb.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyhtools/utils.py` & `pyhtools-2.3.0/pyhtools/utils.py`

 * *Files identical despite different names*

### Comparing `pyhtools-2.2.4/pyproject.toml` & `pyhtools-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyhtools"
-version = "2.2.4"
+version = "2.3.0"
 description = "Python Hacking Tools (PyHTools) (pht) is a collection of python written hacking tools consisting of network scanner, arp spoofer and detector, dns spoofer, code injector, packet sniffer, network jammer, email sender, downloader, wireless password harvester credential harvester, keylogger, download&execute, and reverse_backdoor along with website login bruteforce, scraper, web spider etc. PHT also includes malwares which are undetectable by the antiviruses."
 authors = ["Dhrumil Mistry <contact@dmdhrumilmistry.tech>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
```

### Comparing `pyhtools-2.2.4/PKG-INFO` & `pyhtools-2.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhtools
-Version: 2.2.4
+Version: 2.3.0
 Summary: Python Hacking Tools (PyHTools) (pht) is a collection of python written hacking tools consisting of network scanner, arp spoofer and detector, dns spoofer, code injector, packet sniffer, network jammer, email sender, downloader, wireless password harvester credential harvester, keylogger, download&execute, and reverse_backdoor along with website login bruteforce, scraper, web spider etc. PHT also includes malwares which are undetectable by the antiviruses.
 License: MIT
 Author: Dhrumil Mistry
 Author-email: contact@dmdhrumilmistry.tech
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -57,14 +57,21 @@
 
 ## Disclaimer
 
 The disclaimer advises users to use the open source project for ethical and legitimate purposes only and refrain from using it for any malicious activities. The creators and contributors of the project are not responsible for any illegal activities or damages that may arise from the misuse of the project. Users are solely responsible for their use of the project and should exercise caution and diligence when using it. Any unauthorized or malicious use of the project may result in legal action and other consequences.
 
 [Read More](./DISCLAIMER.md)
 
+### Notice
+
+To comply with PyPi's [Acceptable Use Policy](https://pypi.org/policy/acceptable-use-policy/)
+
+All Evil files are moved to another repository: [pyhtools-evil-files](https://github.com/dmdhrumilmistry/pyhtools-evil-files)
+
+Never use provided resources for malicious purpose.
 
 ## Join Our Discord Community
 
 [![Join our Discord server!](https://invidget.switchblade.xyz/DJrnAg4nv2)](http://discord.gg/DJrnAg4nv2)
 
 ## How To Videos
```

