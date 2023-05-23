# Comparing `tmp/pyhttpx-2.10.1.tar.gz` & `tmp/pyhttpx-2.10.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyhttpx-2.10.1.tar", last modified: Tue Mar 21 12:02:49 2023, max compression
+gzip compressed data, was "dist\pyhttpx-2.10.2.tar", last modified: Tue May 23 13:58:41 2023, max compression
```

## Comparing `pyhttpx-2.10.1.tar` & `pyhttpx-2.10.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 12:02:49.000000 pyhttpx-2.10.1/
--rw-rw-rw-   0        0        0     1086 2022-08-12 14:37:21.000000 pyhttpx-2.10.1/LICENSE
--rw-rw-rw-   0        0        0       24 2022-08-15 03:00:31.000000 pyhttpx-2.10.1/MANIFEST.in
--rw-rw-rw-   0        0        0      339 2023-03-21 12:02:49.000000 pyhttpx-2.10.1/PKG-INFO
--rw-rw-rw-   0        0        0     3236 2023-02-06 04:52:08.000000 pyhttpx-2.10.1/README.md
--rw-rw-rw-   0        0        0        0 2022-08-15 02:16:12.000000 pyhttpx-2.10.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-21 12:02:48.000000 pyhttpx-2.10.1/pyhttpx/
--rw-rw-rw-   0        0        0       81 2022-12-05 09:21:49.000000 pyhttpx-2.10.1/pyhttpx/__init__.py
--rw-rw-rw-   0        0        0      262 2022-09-23 08:01:24.000000 pyhttpx-2.10.1/pyhttpx/__version__.py
--rw-rw-rw-   0        0        0      106 2022-09-23 08:01:24.000000 pyhttpx-2.10.1/pyhttpx/compat.py
--rw-rw-rw-   0        0        0     1107 2022-12-05 07:47:21.000000 pyhttpx-2.10.1/pyhttpx/exception.py
-drwxrwxrwx   0        0        0        0 2023-03-21 12:02:48.000000 pyhttpx-2.10.1/pyhttpx/layers/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.1/pyhttpx/layers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-21 12:02:48.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-21 12:02:49.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/crypto/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/crypto/__init__.py
--rw-rw-rw-   0        0        0     2308 2022-09-23 08:01:24.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/crypto/aes.py
--rw-rw-rw-   0        0        0     1114 2022-09-23 08:01:24.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/crypto/chacha20_poly1305.py
--rw-rw-rw-   0        0        0     4618 2022-09-23 08:01:24.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/crypto/cipher_aead.py
--rw-rw-rw-   0        0        0     3910 2022-09-23 08:01:24.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/crypto/cipher_block.py
--rw-rw-rw-   0        0        0      266 2022-09-23 08:01:24.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/crypto/ciphers.py
--rw-rw-rw-   0        0        0     4293 2022-09-23 08:01:24.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/crypto/ecc.py
--rw-rw-rw-   0        0        0     6180 2023-01-31 06:58:53.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/crypto/hkdf.py
--rw-rw-rw-   0        0        0      947 2022-09-23 08:01:24.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/crypto/kx_algs.py
--rw-rw-rw-   0        0        0     1771 2022-09-23 08:01:24.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/crypto/prf.py
--rw-rw-rw-   0        0        0     7804 2023-02-06 02:15:09.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/extensions.py
--rw-rw-rw-   0        0        0      123 2022-09-23 08:01:24.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/fields.py
--rw-rw-rw-   0        0        0     1232 2022-10-27 08:35:29.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/handshake.py
--rw-rw-rw-   0        0        0     6751 2023-01-31 08:35:07.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/keyexchange.py
-drwxrwxrwx   0        0        0        0 2023-03-21 12:02:49.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/linux/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/linux/__init__.py
--rw-rw-rw-   0        0        0    10884 2023-03-18 08:34:41.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/pyaiossl.py
--rw-rw-rw-   0        0        0    19222 2023-03-21 10:51:10.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/pyssl.py
--rw-rw-rw-   0        0        0     2434 2023-03-21 09:09:35.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/socks.py
--rw-rw-rw-   0        0        0     4513 2022-09-23 08:01:24.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/suites.py
--rw-rw-rw-   0        0        0    19241 2023-01-31 08:15:20.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/tls_context.py
-drwxrwxrwx   0        0        0        0 2023-03-21 12:02:49.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/window/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.1/pyhttpx/layers/tls/window/__init__.py
--rw-rw-rw-   0        0        0     9302 2023-03-08 03:35:13.000000 pyhttpx-2.10.1/pyhttpx/models.py
--rw-rw-rw-   0        0        0    16770 2023-03-18 08:28:32.000000 pyhttpx-2.10.1/pyhttpx/session.py
--rw-rw-rw-   0        0        0     1524 2023-02-24 08:59:16.000000 pyhttpx-2.10.1/pyhttpx/utils.py
--rw-rw-rw-   0        0        0     8006 2022-12-06 09:13:17.000000 pyhttpx-2.10.1/pyhttpx/websocket.py
-drwxrwxrwx   0        0        0        0 2023-03-21 12:02:48.000000 pyhttpx-2.10.1/pyhttpx.egg-info/
--rw-rw-rw-   0        0        0      339 2023-03-21 12:02:48.000000 pyhttpx-2.10.1/pyhttpx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1248 2023-03-21 12:02:48.000000 pyhttpx-2.10.1/pyhttpx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 12:02:48.000000 pyhttpx-2.10.1/pyhttpx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-08-15 06:28:23.000000 pyhttpx-2.10.1/pyhttpx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       68 2023-03-21 12:02:48.000000 pyhttpx-2.10.1/pyhttpx.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-21 12:02:48.000000 pyhttpx-2.10.1/pyhttpx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-21 12:02:49.000000 pyhttpx-2.10.1/setup.cfg
--rw-rw-rw-   0        0        0     1576 2023-03-21 12:02:47.000000 pyhttpx-2.10.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-21 12:02:49.000000 pyhttpx-2.10.1/tests/
--rw-rw-rw-   0        0        0        0 2022-08-15 03:02:17.000000 pyhttpx-2.10.1/tests/__init__.py
--rw-rw-rw-   0        0        0     1078 2023-03-21 12:02:15.000000 pyhttpx-2.10.1/tests/requestTest.py
--rw-rw-rw-   0        0        0     1910 2022-12-05 09:24:22.000000 pyhttpx-2.10.1/tests/websocketTest.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/
+-rw-rw-rw-   0        0        0     1086 2022-08-12 14:37:21.000000 pyhttpx-2.10.2/LICENSE
+-rw-rw-rw-   0        0        0       24 2022-08-15 03:00:31.000000 pyhttpx-2.10.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      339 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3197 2023-05-23 13:16:49.000000 pyhttpx-2.10.2/README.md
+-rw-rw-rw-   0        0        0        0 2022-08-15 02:16:12.000000 pyhttpx-2.10.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/pyhttpx/
+-rw-rw-rw-   0        0        0       81 2022-12-05 09:21:49.000000 pyhttpx-2.10.2/pyhttpx/__init__.py
+-rw-rw-rw-   0        0        0      262 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/__version__.py
+-rw-rw-rw-   0        0        0      106 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/compat.py
+-rw-rw-rw-   0        0        0     1107 2022-12-05 07:47:21.000000 pyhttpx-2.10.2/pyhttpx/exception.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/pyhttpx/layers/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/__init__.py
+-rw-rw-rw-   0        0        0     2308 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/aes.py
+-rw-rw-rw-   0        0        0     1114 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/chacha20_poly1305.py
+-rw-rw-rw-   0        0        0     4618 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/cipher_aead.py
+-rw-rw-rw-   0        0        0     3910 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/cipher_block.py
+-rw-rw-rw-   0        0        0      266 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/ciphers.py
+-rw-rw-rw-   0        0        0     4293 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/ecc.py
+-rw-rw-rw-   0        0        0     6180 2023-01-31 06:58:53.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/hkdf.py
+-rw-rw-rw-   0        0        0      947 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/kx_algs.py
+-rw-rw-rw-   0        0        0     1771 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/prf.py
+-rw-rw-rw-   0        0        0     8016 2023-05-23 13:46:40.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/extensions.py
+-rw-rw-rw-   0        0        0      123 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/fields.py
+-rw-rw-rw-   0        0        0     1232 2022-10-27 08:35:29.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/handshake.py
+-rw-rw-rw-   0        0        0     6750 2023-04-03 08:04:05.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/keyexchange.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/linux/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/linux/__init__.py
+-rw-rw-rw-   0        0        0    10488 2023-05-23 13:31:03.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/pyaiossl.py
+-rw-rw-rw-   0        0        0    19396 2023-05-23 13:31:03.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/pyssl.py
+-rw-rw-rw-   0        0        0     2357 2023-05-17 03:53:54.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/socks.py
+-rw-rw-rw-   0        0        0     4513 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/suites.py
+-rw-rw-rw-   0        0        0    19146 2023-05-20 08:13:11.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/tls_context.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/window/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.2/pyhttpx/layers/tls/window/__init__.py
+-rw-rw-rw-   0        0        0     9302 2023-03-08 03:35:13.000000 pyhttpx-2.10.2/pyhttpx/models.py
+-rw-rw-rw-   0        0        0    16938 2023-05-23 13:12:16.000000 pyhttpx-2.10.2/pyhttpx/session.py
+-rw-rw-rw-   0        0        0     1991 2023-05-23 12:56:47.000000 pyhttpx-2.10.2/pyhttpx/utils.py
+-rw-rw-rw-   0        0        0     8230 2023-05-23 13:39:01.000000 pyhttpx-2.10.2/pyhttpx/websocket.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/pyhttpx.egg-info/
+-rw-rw-rw-   0        0        0      339 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/pyhttpx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1248 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/pyhttpx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/pyhttpx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-08-15 06:28:23.000000 pyhttpx-2.10.2/pyhttpx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       68 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/pyhttpx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/pyhttpx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/setup.cfg
+-rw-rw-rw-   0        0        0     1576 2023-05-23 13:58:30.000000 pyhttpx-2.10.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:58:41.000000 pyhttpx-2.10.2/tests/
+-rw-rw-rw-   0        0        0        0 2022-08-15 03:02:17.000000 pyhttpx-2.10.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     1197 2023-05-23 13:57:49.000000 pyhttpx-2.10.2/tests/requestTest.py
+-rw-rw-rw-   0        0        0     1931 2023-05-23 13:43:36.000000 pyhttpx-2.10.2/tests/websocketTest.py
```

### Comparing `pyhttpx-2.10.1/LICENSE` & `pyhttpx-2.10.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.1/README.md` & `pyhttpx-2.10.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 requirement.txt
 
 ```
 cryptography==36.0.1
 rsa==4.8
 pyOpenSSL==21.0.0
+
 brotli==1.0.9
 hpack==4.0.0
 ```
 ## 查看tls指纹
 - 在线查看,https://tls.peet.ws/api/all,此方式ja3不全,建立抓包
 - 下载wireshark,查看完整握手流程
 
@@ -66,17 +67,16 @@
 ```
 >>> r = sess.post('https://httpbin.org/get',data={})
 >>> r = sess.post('https://httpbin.org/get',json={})
 ```
 
 ## HTTP PROXY
 ```
->>> proxies = {'https': '127.0.0.1:7890'}
->>> proxy_auth = (username, password)
->>> r = sess.post('https://httpbin.org/get',proxies=proxies,proxy_auth=proxy_auth)
+>>> proxies = {'https': 'http://username:password@host:port'}
+>>> r = sess.post('https://httpbin.org/get',proxies=proxies)
 ```
 
 ## ALLOW_REDIRECTS
 
   ```
 >>> r = sess.post('https://httpbin.org/get',allow_redirects=True)
 ```
```

### Comparing `pyhttpx-2.10.1/pyhttpx/exception.py` & `pyhttpx-2.10.2/pyhttpx/exception.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.1/pyhttpx/layers/tls/crypto/aes.py` & `pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.1/pyhttpx/layers/tls/crypto/chacha20_poly1305.py` & `pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/chacha20_poly1305.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.1/pyhttpx/layers/tls/crypto/cipher_aead.py` & `pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/cipher_aead.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.1/pyhttpx/layers/tls/crypto/cipher_block.py` & `pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/cipher_block.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.1/pyhttpx/layers/tls/crypto/ecc.py` & `pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/ecc.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.1/pyhttpx/layers/tls/crypto/hkdf.py` & `pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/hkdf.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.1/pyhttpx/layers/tls/crypto/kx_algs.py` & `pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/kx_algs.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.1/pyhttpx/layers/tls/crypto/prf.py` & `pyhttpx-2.10.2/pyhttpx/layers/tls/crypto/prf.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.1/pyhttpx/layers/tls/extensions.py` & `pyhttpx-2.10.2/pyhttpx/layers/tls/extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,20 +226,23 @@
     fields_desc = [
         _type,
         payload,
     ]
     def dump(self, host, context):
 
         if context.browser_type == 'chrome':
-            self.payload = '\x06\xda\xda\x03\x04\x03\x03'
-            self.payload = '\x06\x8a\x8a\x03\x04\x03\x03'
+            if getattr(context, 'tls_max') == 3:
+                self.payload = '\x04\x8a\x8a\x03\x03'
+            else:
+                self.payload = '\x06\x8a\x8a\x03\x04\x03\x03'
+
         else:
             self.payload = '\x04\x03\x04\x03\x03'
-        self.fields_desc[1] = self.payload
 
+        self.fields_desc[1] = self.payload
         return super().dump(host, context)
 
 
 class ExtCompressCertificate(_BaseExtension):
     _type = 0x1b
     payload = '\x02\x00\x02'
     fields_desc = [
@@ -264,36 +267,43 @@
             payload = _tls_ext_cls[ext_type].payload
         else:
             payload = ''
     fields_desc = [
         ext_type,
         payload,
     ]
+
     ext = type('=^_^=', (_BaseExtension,), dict(fields_desc=fields_desc))
     return ext().dump(host, context)
 
 
 def dump_extension(host, context):
 
     exts = context.exts
     exts_payload = context.exts_payload
     ext_data = []
 
     if exts_payload is None:
         exts_payload = {}
+
     if not exts:
         for e in list(_tls_ext_cls.values())[:]:
             ext_data.append(e().dump(host, context))
 
     else:
         for e in exts:
-            if _tls_ext_cls.get(e):
+
+            if e in exts_payload.keys():
+                payload = exts_payload.get(e)
+                d = make_randext(host, e, payload)
+            elif _tls_ext_cls.get(e):
                 d = _tls_ext_cls.get(e)().dump(host, context)
             else:
                 payload = exts_payload.get(e)
                 d = make_randext(host, e, payload)
+
             ext_data.append(d)
     temp = b''.join(ext_data)
     return b'%s%s' % (struct.pack('!H',len(temp)), temp)
```

### Comparing `pyhttpx-2.10.1/pyhttpx/layers/tls/handshake.py` & `pyhttpx-2.10.2/pyhttpx/layers/tls/handshake.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.1/pyhttpx/layers/tls/keyexchange.py` & `pyhttpx-2.10.2/pyhttpx/layers/tls/keyexchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 
 
         if cipher_suit is None:
             raise TLSCipherNotSupportedErrorExpetion(f'negotiation error, the cipher suite does not support {self.cipher_suit.hex()}')
 
         self.cipher_name = TLS_SUITES.get(int(self.cipher_suit.hex(), 16))['name']
         ext_len = struct.unpack('!H',flowtext[3:5])[0]
-
         ext_datas = flowtext[5:5+ext_len]
 
         while ext_datas:
             ext_type = int(ext_datas[:2].hex(), 16)
             el = struct.unpack('!H',ext_datas[2:4])[0]
             val = ext_datas[4:4+el]
             self.ext[ext_type] = val
```

### Comparing `pyhttpx-2.10.1/pyhttpx/layers/tls/pyaiossl.py` & `pyhttpx-2.10.2/pyhttpx/layers/tls/pyaiossl.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,24 +77,25 @@
 
         self.writer.write(hello.dump(self.tls_cxt))
         exchanage = True
         cache = b''
         self.server_change_cipher_spec = False
         while True:
             try:
-                recv = await self.reader.read(6324)
+                recv = await self.reader.read(8191)
 
             except (ConnectionRefusedError, ConnectionResetError, socket.timeout):
                 raise ConnectionTimeout('无法连接 %s:%s' % (self.host, self.port))
 
             recv = cache + recv
             cache = b''
 
             if recv:
                 while recv:
+
                     handshake_type = struct.unpack('!B', recv[:1])[0]
                     length = struct.unpack('!H', recv[3:5])[0]
                     flowtext = recv[5:5 + length]
                     if len(flowtext) != length:
                         cache = recv[:]
                         break
 
@@ -102,15 +103,14 @@
 
                         # 在发送verify_data处理握手层数据
                         if not self.server_change_cipher_spec:
                             self.tls_cxt.handshake_data.append(flowtext)
                             self.servercontext.load(flowtext)
 
                         if not exchanage and self.server_change_cipher_spec:
-                            # print(threading.current_thread().name,'成功握手,server Encrypted Handshake Message')
                             # 验证服务器消息,Encrypted Handshake Message,效验密钥
 
                             server_verify_data = self.tls_cxt.decrypt(flowtext, b'\x16')
                             self.tls_cxt.verify_server_message(server_verify_data)
                             return True
 
                     elif handshake_type == 0x14:
@@ -181,14 +181,15 @@
                 break
 
             s = s[5 + length:]
             if handshake_type == 0x17:
                 p = self.tls_cxt.decrypt(flowtext, b'\x17')
                 self.plaintext_reader += p
 
+
             elif handshake_type == 0x15:
                 self.isclosed = True
                 exc_alert = True
                 raise ConnectionClosed('server closed')
 
         b = self.plaintext_reader
         self.plaintext_reader = b''
@@ -200,24 +201,25 @@
 
 PROTOCOL_TLSv1_2 = b'\x03\x03'
 def default_context():
     return SSLContext(PROTOCOL_TLSv1_2)
 
 
 class SSLContext:
-    def __init__(self, protocol=None, http2=True):
+    def __init__(self, protocol=None, http2=False):
         self.protocol = protocol
         self.check_hostname: bool = False
         self.browser_type = 'chrome'
-        self.http2 = False
+        self.http2 = http2
         self.ciphers = None
         self.exts = None
         self.exts_payload = None
         self.supported_groups = None
         self.ec_points = None
+        self.tls_max = 3
 
     def set_payload(self, browser_type=None,
                     ja3=None,
                     exts_payload=None,
                     shuffle_extension_protocol=None):
         self.browser_type = browser_type or 'chrome'
         self.exts_payload = exts_payload
@@ -235,14 +237,15 @@
         ]
         def choose_grease():
 
             e = random.choice(grease_list)
             grease_list.remove(e)
             return e
 
+
         if ja3:
             self.ja3 = ja3
             if self.browser_type == 'chrome':
                 #规范ja3
                 tmp = self.ja3.split(',')
                 self.grease_group = int(tmp[3].split('-')[0])
                 supported_groups = [23,24,25,29,256,257]
@@ -293,27 +296,16 @@
         return TLSSocket(sock=sock,server_hostname=server_hostname, ssl=self)
 
     def load_cert_chain(self, certfile: str, ketfile: str):
         pass
 
 
 
-async def main():
-    host = '127.0.0.1'
-    port = 443
-    addres = (host, port)
-    context = SSLContext(PROTOCOL_TLSv1_2)
-
-    sock = context.wrap_socket()
-    await sock.connect(addres)
-
-    m = 'GET / HTTP/1.1\r\n\r\n'
-    await sock.sendall(m.encode())
-    data = await sock.recv(1024)
-    print(data)
+
+
```

### Comparing `pyhttpx-2.10.1/pyhttpx/layers/tls/pyssl.py` & `pyhttpx-2.10.2/pyhttpx/layers/tls/pyssl.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,20 +23,20 @@
     ConnectionTimeout,
     ConnectionClosed,
     TLSHandshakeFailed,
     ProxyError,
     ReadTimeout)
 
 from pyhttpx.layers.tls.socks import SocketProxy
-
+from pyhttpx.utils import _parse_proxy_url
 
 PROTOCOL_TLSv1_2 = b'\x03\x03'
 PROTOCOL_TLSv1_3 = b'\x03\x04'
 def default_context():
-    return SSLContext(PROTOCOL_TLSv1_2)
+    return SSLContext(PROTOCOL_TLSv1_3)
 
 
 class SSLContext:
 
     def __init__(self, protocol=None, http2=True):
         self.protocol = protocol
         self.check_hostname: bool = False
@@ -46,25 +46,25 @@
         self.supported_groups = None
 
         self.ec_points = None
         self.browser_type = None
         self.http2 = http2
         self.application_layer_protocol_negotitaion = 'http/1.1'
         self.tlsversion = b'\x03\x03'
-
+        self.tls_max = 4
 
     def set_payload(self, browser_type=None,
                     ja3=None,
                     exts_payload=None,
                     shuffle_extension_protocol=None):
         self.browser_type = browser_type or 'chrome'
         self.exts_payload = exts_payload
         self.shuffle_extension_protocol = shuffle_extension_protocol
-        #https://www.rfc-editor.org/rfc/rfc8701
 
+        #https://www.rfc-editor.org/rfc/rfc8701
         grease_list = [
             0x0A0A, 0x1A1A,
             0x2A2A, 0x3A3A,
             0x4A4A, 0x5A5A,
             0x6A6A, 0x7A7A,
             0x8A8A, 0x9A9A,
             0xAAAA, 0xBABA,
@@ -104,15 +104,15 @@
 
                 exts = '-'.join(map(lambda x:str(x), exts))
                 self.ja3 = f"771,{grease_ciphers}-4865-4866-4867-49195-49199-49196-49200-52393-52392-49171-49172-156-157-47-53,{exts},{self.grease_group}-29-23-24,0"
                 self.exts_payload = {grease_ext2: b'\x00'}
 
 
             else:
-                #firefox_j,a3
+                #firefox_ja3
                 exts=[0,23,65281,10,11,35,16,5,34,51,43,13,45,28,21]
                 if self.shuffle_extension_protocol:
                     random.shuffle(exts)
                 exts = '-'.join(map(lambda x:str(x), exts))
                 self.ja3 = f"771,4865-4867-4866-49195-49199-52393-52392-49196-49200-49162-49161-49171-49172-156-157-47-53,{exts},29-23-24-25-256-257,0"
 
 
@@ -145,42 +145,44 @@
     def isclosed(self):
         return getattr(self, '_closed')
 
     @isclosed.setter
     def isclosed(self, value):
         setattr(self, '_closed', value)
 
-    def connect(self,addres, timeout=None, proxies=None, proxy_auth=None):
+    def connect(self,addres, timeout=None, proxies=None):
         self.servercontext = ServerContext()
         self.tls_cxt = TLSSessionCtx()
         self.context.group_x25519_key = self.tls_cxt.group_x25519_key
         self.context.group_secp_key = self.tls_cxt.group_secp_key
         self.tls_cxt.handshake_data = []
+
         self.host,self.port = addres[0],int(addres[1])
-        self.proxy_auth = proxy_auth
+
         if not self.sock:          
             self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-            
-        self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
 
+        self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self.timeout  = timeout
         self.proxies = proxies
         
         if self.proxies and self.proxies.get('https'):
             self.sock = SocketProxy(socket.AF_INET, socket.SOCK_STREAM)
             proxy = self.proxies['https']
-            if not ':' in proxy:
-                raise ProxyError(f'ProxyError: {proxy}')
-            proxy_ip, proxy_port = proxy.split(':')
-            if self.proxy_auth:
-                username,password = proxy_auth[0], proxy_auth[1]
+            proxy_parse = _parse_proxy_url(proxy)
+            if proxy_parse.auth:
+                username,password = proxy_parse.auth.split(':')
             else:
-                username, password = None,None
+                username, password = (None, None)
 
-            self.sock.set_proxy(SocketProxy.HTTP, proxy_ip, proxy_port,username, password )
+            self.sock.set_proxy(SocketProxy.HTTP,
+                                proxy_parse.host,
+                                proxy_parse.port,
+                                username,
+                                password )
 
         try:
             self.sock.settimeout(self.timeout)
             self.sock.connect((self.host, self.port))
 
         except (ConnectionRefusedError,TimeoutError,socket.timeout):
             raise ConnectionTimeout(f'unable to connect {self.host}:{self.port}')
@@ -206,29 +208,29 @@
             length = 5
             recv_len = length
 
             head_flowtext = b''
             while len(head_flowtext) < length:
                 s = self.mutable_recv(recv_len)
                 if not s:
-                    raise TLSHandshakeFailed('handshake failed')
+                    raise ConnectionClosed('server closed connect')
 
                 head_flowtext += s
                 recv_len = length - len(head_flowtext)
 
             content_type = struct.unpack('!B', head_flowtext[:1])[0]
             length = struct.unpack('!H', head_flowtext[3:5])[0]
             flowtext = b''
             recv_len = length
 
             while len(flowtext) < length:
 
                 s = self.mutable_recv(recv_len)
                 if not s:
-                    raise TLSHandshakeFailed('handshake failed')
+                    raise ConnectionClosed('server closed connect')
                 flowtext += s
                 recv_len = length - len(flowtext)
 
 
             if content_type == 0x16:
 
                 if not self.server_change_cipher_spec:
@@ -257,15 +259,18 @@
                     if self.servercontext.serverstore.ext.get(16):
                         alpn = self.servercontext.serverstore.ext.get(16)[3:]
                         self.context.application_layer_protocol_negotitaion = alpn.decode('latin1')
 
 
                     if self.tls13:
                         self.server_change_cipher_spec = True
+
                         server_publickey = self.servercontext.serverstore.ext[51][4:]
+                        if self.servercontext.serverstore.ext[51][:2] == b'\x00\x1d' and len(server_publickey) != 32:
+                            raise ConnectionClosed('server closed connect')
                         self.tls_cxt.negotiated.ciphersuite = int(self.servercontext.serverstore.cipher_suit.hex(), 16)
                         self.tls_cxt.load_alg()
                         self.tls_cxt.make_secret(server_publickey)
 
 
                 if not self.tls13:
 
@@ -326,15 +331,15 @@
                             self.sock.sendall(changecipherspec)
                             verify_data = self.tls_cxt.compute_verify_data()
                             ciphertext = self.tls_cxt.encrypt(verify_data, b'\x17')
 
                             data = b'\x17\x03\x03' + struct.pack('!H', len(ciphertext)) + ciphertext
                             self.sock.sendall(data)
 
-                            #去掉certificate_request, 不然效验数据出错, 暂不清楚为什么
+                            #去掉certificate_request
                             if self.tls_cxt.certificate_request:
                                 self.tls_cxt.handshake_data.pop()
 
                             self.tls_cxt.derive_application_traffic_secret()
 
                             #ticket数据开始重置sequence
                             self.tls_cxt.server_ctx.sequence = 0
@@ -350,15 +355,14 @@
 
                         elif handshake_type == 0x0b:
                             #服务器证书11
                             pass
 
                         elif handshake_type == 0x0d:
                             #certificate request
-                            pass
                             self.tls_cxt.certificate_request = True
                         elif handshake_type == 0x0f:
                             #证书服务器验证15
                             pass
                         elif handshake_type == 0x08:
                             #扩展
                             payload = payload[2:]
@@ -383,14 +387,15 @@
                 if self.servercontext.done and exchanage:
 
                     self.tls_cxt.server_ctx.random = self.servercontext.serverstore.random
                     self.tls_cxt.negotiated.ciphersuite = int(self.servercontext.serverstore.cipher_suit.hex(), 16)
                     self.tls_cxt.rsa_pulicKey = self.servercontext.certificatecontext.rsa_pulicKey
                     self.tls_cxt.curve_name = self.servercontext.curve_name
                     self.tls_cxt.server_ecdhe_pubkey = self.servercontext.serverpubkey
+
                     if 23 in self.servercontext.serverstore.ext.keys():
                         self.tls_cxt.extended_master_secret = True
 
                     # 加载相关套件
                     self.tls_cxt.load_alg()
 
                     if self.tls_cxt.certificate_request:
```

### Comparing `pyhttpx-2.10.1/pyhttpx/layers/tls/socks.py` & `pyhttpx-2.10.2/pyhttpx/layers/tls/socks.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,20 +28,20 @@
         dest_addr = dest_pair[0]
         dest_port = dest_pair[1]
 
 
         http_headers = [
             (b"CONNECT " + dest_addr.encode("idna") + b":"
              + str(dest_port).encode() + b" HTTP/1.1"),
-            b"Host: " + dest_addr.encode("idna")
+
         ]
 
         if username and password:
             http_headers.append(b"Proxy-Authorization: Basic "
-                                + b64encode(username.encode('latin1') + b":" + password.encode('latin1')))
+                                 + b64encode(username.encode('latin1') + b":" + password.encode('latin1')))
 
         http_headers.append(b"\r\n")
         try:
             super(SocketProxy, self).connect((proxy_addr, proxy_port))
             self.sendall(b"\r\n".join(http_headers))
             status_line = self.recv(4096).decode()
             proto, status_code, status_msg = status_line.split(" ", 2)
@@ -69,12 +69,11 @@
             raise ProxyError(error)
         return True
 
 if __name__ == '__main__':
     sock  = socket.socket(socket.AF_INET, socket.SOCK_STREAM, 0)
     s = SocketProxy()
     s.set_proxy(1, '127.0.0.1', 7890)
-    s.connect(('www.google.com',443))
-    print(s.getsockname())
+    s.connect(('httpbin.org',443))
```

### Comparing `pyhttpx-2.10.1/pyhttpx/layers/tls/suites.py` & `pyhttpx-2.10.2/pyhttpx/layers/tls/suites.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.1/pyhttpx/layers/tls/tls_context.py` & `pyhttpx-2.10.2/pyhttpx/layers/tls/tls_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-import time
+
 from collections import namedtuple
 import hashlib
 import struct
 import os
-
 import hmac
-
 import rsa
+
 from cryptography.hazmat.primitives.asymmetric import x25519
 from cryptography.hazmat.primitives.asymmetric import ec as cg_ec
 from cryptography.hazmat.primitives import serialization
 
+from pyhttpx.layers.tls.crypto.cipher_aead import Cipher_AES_128_GCM_TLS13
 from pyhttpx.layers.tls.crypto.ecc import CryptoContextFactory
 from pyhttpx.layers.tls.crypto.prf import prf
 from pyhttpx.layers.tls.suites import (
     get_algs_from_ciphersuite_name,
     TLS_SUITES
 )
 from pyhttpx.layers.tls.crypto.hkdf import TLS13_HKDF
 from pyhttpx.exception import TLSVerifyDataExpetion
 
-import threading
-
 class TLSContext(object):
 
     def __init__(self, name):
         self.name = name
         self.handshake = None
         self.sequence = 0
         self.nonce = 0
@@ -43,14 +41,15 @@
 
 def rsa_encrypt(plaintxt, publickey):
     return rsa.encrypt(plaintxt, publickey)
 
 class TLSSessionCtx(object):
 
     def __init__(self, client=True):
+
         self.client = client
         self.server = not self.client
         self.client_ctx = TLSContext("Client TLS context")
         self.server_ctx = TLSContext("Server TLS context")
         self.certificate_request = False
         self.negotiated = namedtuple("negotiated", ["ciphersuite", "key_exchange", "encryption", "mac", "compression",
                                                     "compression_algo", "version", "sig", "resumption"])
@@ -198,14 +197,15 @@
         self.master_secret = prf(self.premaster_secret, seed, self.hash_alg, outlen=48)
         sslkey_file_name = os.environ.get('SSLKEYLOGFILE')
         if sslkey_file_name:
             with open(sslkey_file_name, 'a') as f:
                 s = f'CLIENT_RANDOM {self.client_ctx.random.hex()} {self.master_secret.hex()}'
                 f.write(s)
 
+
     def key_expandsion(self):
         seed = b'key expansion' + self.server_ctx.random + self.client_ctx.random
         self.key_block = prf(self.master_secret, seed, self.hash_alg, outlen=256)
 
 
     def negotiated_premaster_secret(self):
 
@@ -279,35 +279,29 @@
 
         self.secrets = self.hkdf.make_secret(self.premaster_secret, self.handshake_data)
 
         client_handshake_traffic_secret = self.secrets['client_handshake_traffic_secret']
         server_handshake_traffic_secret = self.secrets['server_handshake_traffic_secret']
 
         sslkey_file_name = os.environ.get('SSLKEYLOGFILE')
+
         if sslkey_file_name:
             with open(sslkey_file_name, 'a') as f:
                 s = f'CLIENT_HANDSHAKE_TRAFFIC_SECRET {self.client_ctx.random.hex()} {client_handshake_traffic_secret.hex()}\n' \
                     f'SERVER_HANDSHAKE_TRAFFIC_SECRET {self.client_ctx.random.hex()} {server_handshake_traffic_secret.hex()}\n' \
                     f'CLIENT_TRAFFIC_SECRET_0 {self.client_ctx.random.hex()} {self.secrets["client_application_traffic_secret"].hex()}\n' \
                     f'SERVER_TRAFFIC_SECRET_0 {self.client_ctx.random.hex()} {self.secrets["server_application_traffic_secret"].hex()}\n'
 
                 f.write(s)
 
-
-        import time
-        #time.sleep(11111)
         self.server_handshake_write_key = self.secrets['server_handshake_write_key']
         self.server_handshake_write_iv = self.secrets['server_handshake_write_iv']
         self.client_handshake_write_key = self.secrets['client_handshake_write_key']
         self.client_handshake_write_iv = self.secrets['client_handshake_write_iv']
-
         self.tls13_master_secret = self.secrets['tls13_master_secret']
-
-
-
         self.client_ctx.crypto_alg = self.cls_cipher_alg(self.client_handshake_write_key, self.client_handshake_write_iv)
         self.server_ctx.crypto_alg = self.cls_cipher_alg(self.server_handshake_write_key, self.server_handshake_write_iv)
 
     def derive_application_traffic_secret(self):
 
 
         client_application_traffic_secret = self.hkdf.derive_secret(self.tls13_master_secret,
@@ -340,15 +334,14 @@
         self.server_ctx = TLSContext("Server TLS context")
 
         self.negotiated = namedtuple("negotiated", ["ciphersuite", "key_exchange", "encryption", "mac", "compression",
                                                     "compression_algo", "version", "sig", "resumption"])
 
 
         self.handshake_data = []
-
         self.tls_version = b'\x03\x04'
 
         name_curve = 0x001d
         self.group_x25519_key = CryptoContextFactory.crypto_container[name_curve].client_kx_privkey.public_key().public_bytes(
                 serialization.Encoding.Raw,
                 serialization.PublicFormat.Raw
             )
@@ -370,19 +363,15 @@
             x25519.X25519PublicKey.from_public_bytes(server_publickey))
 
         self.secrets = self.hkdf.make_secret(self.premaster_secret, self.handshake_data)
         self.server_handshake_write_key = self.secrets['server_handshake_write_key']
         self.server_handshake_write_iv = self.secrets['server_handshake_write_iv']
         self.client_handshake_write_key = self.secrets['client_handshake_write_key']
         self.client_handshake_write_iv = self.secrets['client_handshake_write_iv']
-
         self.tls13_master_secret = self.secrets['tls13_master_secret']
-
-
-
         self.client_ctx.crypto_alg = self.cls_cipher_alg(self.client_handshake_write_key, self.client_handshake_write_iv)
         self.server_ctx.crypto_alg = self.cls_cipher_alg(self.server_handshake_write_key, self.server_handshake_write_iv)
 
     def derive_application_traffic_secret(self):
 
         client_application_traffic_secret = self.hkdf.derive_secret(self.tls13_master_secret,
                                                                     b"c ap traffic",
@@ -402,15 +391,15 @@
                                                                    b"key",
                                                                    b"", self.hkdf.key_len)
         self.server_application_write_iv = self.hkdf.expand_label(server_application_traffic_secret,
                                                                   b"iv",
                                                                   b"", 12)
 
 
-    def encrypt(self, P,content_type ):
+    def encrypt(self, P, content_type ):
 
         sequence = struct.pack('!Q', self.client_ctx.sequence)
         p_len = len(P)
 
         #content_type + b'\x03\x03' + len(plaintext) + tag_len
         A = content_type + b'\x03\x03' + struct.pack('!H', p_len + 16)
         data = self.client_ctx.crypto_alg.encrypt(P, A, sequence)
@@ -426,27 +415,21 @@
         data = self.server_ctx.crypto_alg.decrypt(C, A, sequence)
         self.server_ctx.sequence += 1
         return data
 
 
     def load_alg(self):
         cipher_name = TLS_SUITES.get(self.negotiated.ciphersuite)['name']
-
         kx_alg, cipher_alg, hmac_alg, hash_alg, tls1_3 = get_algs_from_ciphersuite_name(cipher_name)
         self.hash_alg = hashlib.sha256
-        from pyhttpx.layers.tls.crypto.cipher_aead import Cipher_AES_128_GCM_TLS13
-
         self.hmac_alg = hashlib.sha256
         self.cls_cipher_alg = Cipher_AES_128_GCM_TLS13
-
         self.kx_alg = kx_alg
         self.hmac_alg = hmac_alg
 
-
     def compute_verify_data(self):
         verify_data = self.hkdf.compute_verify_data(
             self.secrets['client_handshake_traffic_secret'], b''.join(self.handshake_data))
 
         #verify_data_len=3byte
         verify_data  = b'\x14' + struct.pack("!I", len(verify_data))[1:] + verify_data + b'\x16'
-
-        return verify_data
+        return verify_data
```

### Comparing `pyhttpx-2.10.1/pyhttpx/models.py` & `pyhttpx-2.10.2/pyhttpx/models.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.1/pyhttpx/session.py` & `pyhttpx-2.10.2/pyhttpx/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,16 +77,15 @@
                             )
         conn = context.wrap_socket(
             sock=None,server_hostname=None)
 
         conn.connect(
             (self.req.host,self.req.port),
             timeout=self.req.timeout,
-            proxies=self.req.proxies,
-            proxy_auth=self.req.proxy_auth)
+            proxies=self.req.proxies,)
 
         return conn
 
     def _get_conn(self):
         conn = None
         try:
             conn = self.poolconnections.get(block=False)
@@ -144,35 +143,43 @@
                 c[k] = v
         elif isinstance(set_cookies, dict):
             c.update(set_cookies)
 
         self.cookie_manger.set_cookie(req,c)
 
 
-    def request(self, method, url,update_cookies=True,timeout=None,proxies=None,proxy_auth=None,
-                params=None, data=None, headers=None, cookies=None,json=None,allow_redirects=True,verify=None):
+    def request(self, method,
+                url,
+                update_cookies=True,
+                timeout=None,
+                proxies=None,
+                params=None,
+                data=None,
+                headers=None,
+                cookies=None,
+                json=None,
+                allow_redirects=True,
+                verify=None):
 
         #多线程,采用局部变量
         req = Request(
             method=method.upper(),
             url=url,
             headers=headers or {},
             data=data or {},
             json=json,
             cookies=cookies or {},
             params=params or {},
             timeout=timeout,
             proxies=proxies,
-            proxy_auth=proxy_auth,
             allow_redirects=allow_redirects,
 
         )
         self.req = req
 
-
         if cookies:
             self.handle_cookie(req, cookies)
             _cookies = cookies
         else:
             _cookies = self.cookie_manger.get(get_top_domain(self.req.host))
         send_kw  = {}
 
@@ -215,30 +222,34 @@
         return resp
 
     def prep_request(self, req, send_kw) -> bytes:
 
         msg = b'%s %s HTTP/1.1\r\n' % (req.method.encode('latin1'), req.path.encode('latin1'))
         dh = copy.deepcopy(req.headers) or default_headers()
         dh.update(send_kw)
-        dh['host'] = req.host
-        dh=dict((k.lower(), v) for k, v in dh.items())
+        dh['Host'] = req.host
+        dh=dict((k, v) for k, v in dh.items())
         req_body = ''
-
+        
         if req.method == 'POST':
             if req.data:
                 if isinstance(req.data, str):
                     req_body = req.data
 
                 elif isinstance(req.data, dict):
                     req_body = urlencode(req.data)
 
             elif req.json:
                 req_body = json.dumps(req.json, separators=(',', ':'))
 
-            dh['content-length'] = len(req_body)
+            dh['Content-Length'] = len(req_body)
+
+        else:
+            if dh.get('Content-Length'):
+                del dh['Content-Length']
 
         for k, v in dh.items():
             msg += ('%s: %s\r\n' % (k, v)).encode('latin1')
 
         msg += b'\r\n'
         msg += req_body.encode('latin1')
         return msg
@@ -342,15 +353,15 @@
         }
         headers = copy.deepcopy(req.headers) or default_headers()
 
         for k,v in headers.items():
             k = k.lower()
             dh[k] = v
         if req.method == 'POST':
-            dh['content-length'] = len(req_body)
+            dh['Content-Length'] = len(req_body)
 
         head_block = []
         for k,v in dh.items():
             if not k in ['connection','host']:
                 head_block.append((k,v))
 
         _cookies = self.cookie_manger.get(get_top_domain(self.req.host))
```

### Comparing `pyhttpx-2.10.1/pyhttpx/websocket.py` & `pyhttpx-2.10.2/pyhttpx/websocket.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 
 import asyncio
 import struct
 import hashlib
 import base64
 import os
-
+import time
+import zlib
 from urllib.parse import urlparse
 import socket
 
 from pyhttpx.layers.tls.pyaiossl import SSLContext,PROTOCOL_TLSv1_2
 from pyhttpx.exception import (
     SwitchingProtocolError,
     SecWebSocketKeyError,
@@ -96,15 +97,15 @@
             sec_websocket_key = self.sec_websocket_key + '258EAFA5-E914-47DA-95CA-C5AB0DC85B11'
             sec_websocket_accept = head['sec-websocket-accept']
 
             b = base64.b64encode(hashlib.sha1(sec_websocket_key.encode('latin1')).digest())
             if b != sec_websocket_accept.encode():
                 raise SecWebSocketKeyError('sec_websocket_key verify failed')
         else:
-            raise SwitchingProtocolError(f"host={self.addres[0]},path={self.path},switching protocol error,status_code {status_code},text: {data}")
+            raise SwitchingProtocolError(f"connect fail!, status_code {status_code}")
 
     async def on_open(self):
 
         self.sec_websocket_key = base64.b64encode(os.urandom(16)).decode()
         self.headers['Sec-WebSocket-Key'] = self.sec_websocket_key
 
         request_header = [f'GET {self.path} HTTP/1.1']
@@ -140,22 +141,29 @@
 
         s = struct.pack('!B', head_frame)
         if len(data) < 126:
             MASK = 0b10000000
             MASK |= len(data)
             m = struct.pack('!B', MASK)
             s += m
+
         elif 126 <= len(data) <= 2 ** 16 -1:
             MASK = 0b10000000
+            #数据长度2字节
             MASK |= 126
+            #谁否掩码
             m = struct.pack('!B', MASK)
             s += m
             s += struct.pack('!H', len(data))
+
+
+
         elif 2 ** 16 -1 <  len(data) <= 2**64 -1:
             MASK = 0b10000000
+            #数据长度8字节
             MASK |= 127
             m = struct.pack('!B', MASK)
             s += m
             s += struct.pack('!Q', len(data))
 
         else:
             raise OverflowError('data length more than 64 byte')
@@ -178,14 +186,15 @@
         if len(self.cache_buffer) < 2:
             return
 
         frame_head = self.cache_buffer[0]
         FIN = frame_head >> 7
         opcode = frame_head & 0b1111
         payload_len = self.cache_buffer[1] & 0b1111111
+        per_message_compressed = frame_head >> 6 & 1
 
         if payload_len < 126:
             n = 2
             msg_len = payload_len
             msg = self.cache_buffer[n:n + msg_len]
             self.cache_buffer = self.cache_buffer[n + msg_len:]
         elif payload_len == 126:
@@ -195,19 +204,23 @@
             self.cache_buffer = self.cache_buffer[n + msg_len:]
         else:
             n = 10
             msg_len = struct.unpack('!Q', self.cache_buffer[2:n])[0]
             msg = self.cache_buffer[n:n + msg_len]
             self.cache_buffer = self.cache_buffer[n + msg_len:]
 
+
         while len(msg) < msg_len:
             #数据长度不足,缓存中的数据还属于当前帧,继续读取
-            d = self.sock.recv(msg_len)
+            d = await self.sock.recv(msg_len)
             msg += d
 
+        if per_message_compressed:
+            msg = zlib.decompressobj(-zlib.MAX_WBITS).decompress(msg)
+
         if opcode == 0x00:
             self.reader_buffer += msg
         elif opcode == 0x01:
             self.reader_buffer += msg
         elif opcode == 0x02:
             self.reader_buffer += msg
         elif opcode == 0x08:
@@ -232,14 +245,15 @@
         else:
             pass
     async def recv(self):
 
         while 1:
             #握手过程产生的缓存数据
             result = await self.handle()
+
             if result:
                 return result
             try:
                 data = await self.sock.recv(2 ** 14)
             except ConnectionResetError:
                 self.open = False
                 raise WebSocketClosed('webscoket Closed')
```

### Comparing `pyhttpx-2.10.1/pyhttpx.egg-info/SOURCES.txt` & `pyhttpx-2.10.2/pyhttpx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.1/setup.py` & `pyhttpx-2.10.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         sys.exit(errno)
 
 
 
 packages = find_packages()
 setup(
     name = "pyhttpx",
-    version = "2.10.1",
+    version = "2.10.2",
     keywords = ["pip", "pyhttpx"],
     description = "HTTP library.",
     long_description = "HTTP library, TLS supported version：tls1.2/tls1.3, HTTP supported version: http1.1/http2",
     license = "MIT Licence",
 
     url = "https://github.com/zero3301/pyhttpx",
     author = "3301",
```

### Comparing `pyhttpx-2.10.1/tests/requestTest.py` & `pyhttpx-2.10.2/tests/requestTest.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,48 +8,45 @@
 import random
 import os
 import concurrent
 import threading
 import requests
 
 headers={
-
+'Host': '*',
 'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36',
 'Pragma': 'no-cache',
 'Cache-Control': 'no-cache',
 'sec-ch-ua-platform': '"Windows"',
 'sec-ch-ua-mobile': '?0',
-#'Content-type': 'application/x-www-form-urlencoded',
 'Accept': '*/*',
 'Sec-Fetch-Site': 'cross-site',
 'Sec-Fetch-Mode': 'cors',
 'Sec-Fetch-Dest': 'empty',
 'Accept-Encoding': 'gzip, deflate, br',
 'Accept-Language': 'zh,zh-CN;q=0.9,en;q=0.8',
 
 }
 
 
 def main():
     sess = pyhttpx.HttpSession(http2=False,
-                               browser_type='chrome')
+                               browser_type='chrome',
+                               shuffle_extension_protocol=True
+                               )
 
     url='https://tls.peet.ws/api/all'
-    #url = 'https://httpbin.org/get'
+    #url = 'https://httpbin.org/ip'
+    proxies = {
+        'https': 'http://username:password@host:port'
+    }
     r = sess.get(url,headers=headers)
     print(r.status_code)
     print(r.text)
 
-
-
-
-
-
-
-
 if __name__ == '__main__':
     main()
```

### Comparing `pyhttpx-2.10.1/tests/websocketTest.py` & `pyhttpx-2.10.2/tests/websocketTest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 """
 docs
 pyhttpx.websocket
 
 """
 
 import asyncio
+import time
+
+import pyhttpx
 from pyhttpx import WebSocketClient
 
 class WSS:
     def __init__(self,url=None, headers=None, loop=None):
         self.url = url
         self.headers = headers
         self.loop = loop
-        #self.ja3 = '771,19018-4865-4866-4867-49195-49199-49196-49200-52393-52392-49171-49172-156-157-47-53,0-23-65281-10-11-35-16-5-13-18-51-45-43-27-17513,27242-29-23-24,0'
+        self.ja3 = '771,19018-4865-4866-4867-49195-49199-49196-49200-52393-52392-49171-49172-156-157-47-53,0-23-65281-10-11-35-16-5-13-18-51-45-43-27-17513,27242-29-23-24,0'
 
     async def connect(self):
-        self.sock = await WebSocketClient(url=self.url, headers=self.headers, loop=self.loop,
-                                          ).connect()
 
+        self.sock = await WebSocketClient(url=self.url,
+                                          headers=self.headers,
+                                          loop=self.loop,
+                                          ja3=self.ja3
+                                          ).connect()
 
+        print('连接成功...')
     async def send(self):
-        while 1:
-            if self.sock.open:
-                data = '3301'
-                print('send',data)
-                await self.sock.send(data, binary=True)
-                await asyncio.sleep(3)
+        await self.sock.send('666')
+        pass
 
     async def recv(self):
         while 1:
             r = await self.sock.recv()
-            print('recv',r)
-
-
+            print(r)
 def main():
     loop = asyncio.get_event_loop()
     url = 'wss://www.python-spider.com/api/challenge62'
-    print(f'connect: {url}')
     headers = {
-        'Connection': 'Upgrade' ,
+        'Host': 'www.python-spider.com',
+        'Connection': 'Upgrade',
         'Pragma': 'no-cache',
         'Cache-Control': 'no-cache',
-        'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/107.0.0.0 Safari/537.36',
+        'Origin': 'www.python-spider.com',
+        'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
         'Upgrade': 'websocket',
-        'Sec-WebSocket-Version': '13' ,
-        'Accept-Encoding': 'gzip, deflate, br' ,
-        'Accept-Language': 'zh,zh-CN;q=0.9,en;q=0.8' ,
-        'Sec-WebSocket-Key': 'p1+bsFFmXixD+hk1CHG+3w==',
-        'Sec-WebSocket-Extensions': 'permessage-deflate; client_max_window_bits' ,
-
-    }
+        'Sec-WebSocket-Version': '13',
+        'Accept-Encoding': 'gzip, deflate, br',
+        'Accept-Language': 'zh,zh-CN;q=0.9,en;q=0.8',
+        'Sec-WebSocket-Extensions': 'permessage-deflate; client_max_window_bits',
 
+}
     wss = WSS(url, headers, loop)
     loop.run_until_complete(wss.connect())
     loop.create_task(wss.send())
     loop.create_task(wss.recv())
     loop.run_forever()
 
 if __name__ == '__main__':
-    main()
+    main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

