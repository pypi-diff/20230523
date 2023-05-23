# Comparing `tmp/os2borgerpc_client-2.2.0.tar.gz` & `tmp/os2borgerpc_client-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os2borgerpc_client-2.2.0.tar", last modified: Thu Mar  9 09:58:02 2023, max compression
+gzip compressed data, was "os2borgerpc_client-2.2.1.tar", last modified: Tue May 23 08:59:34 2023, max compression
```

## Comparing `os2borgerpc_client-2.2.0.tar` & `os2borgerpc_client-2.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-03-09 09:58:02.433328 os2borgerpc_client-2.2.0/
--rw-r--r--   0 m         (1000) m         (1000)    35149 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.0/LICENSE
--rw-rw-r--   0 m         (1000) m         (1000)     1190 2023-03-09 09:58:02.432328 os2borgerpc_client-2.2.0/PKG-INFO
--rw-rw-r--   0 m         (1000) m         (1000)      755 2023-02-28 13:56:42.000000 os2borgerpc_client-2.2.0/README.rst
-drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-03-09 09:58:02.431328 os2borgerpc_client-2.2.0/bin/
--rwxr-xr-x   0 m         (1000) m         (1000)      561 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.0/bin/admin_connect.sh
--rwxr-xr-x   0 m         (1000) m         (1000)      731 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.0/bin/get_os2borgerpc_config
--rwxrwxr-x   0 m         (1000) m         (1000)     1766 2023-03-09 08:36:07.000000 os2borgerpc_client-2.2.0/bin/jobmanager
--rwxr-xr-x   0 m         (1000) m         (1000)      227 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.0/bin/os2borgerpc_find_gateway
--rwxrwxr-x   0 m         (1000) m         (1000)      949 2023-02-28 13:56:42.000000 os2borgerpc_client-2.2.0/bin/os2borgerpc_push_config_keys
--rwxrwxr-x   0 m         (1000) m         (1000)      845 2023-02-28 13:56:42.000000 os2borgerpc_client-2.2.0/bin/os2borgerpc_register_in_admin
--rwxr-xr-x   0 m         (1000) m         (1000)     1862 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.0/bin/randomize_jobmanager.sh
--rwxrwxr-x   0 m         (1000) m         (1000)     5145 2023-02-28 13:56:42.000000 os2borgerpc_client-2.2.0/bin/register_new_os2borgerpc_client.sh
--rwxr-xr-x   0 m         (1000) m         (1000)      606 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.0/bin/set_os2borgerpc_config
-drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-03-09 09:58:02.429328 os2borgerpc_client-2.2.0/os2borgerpc/
-drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-03-09 09:58:02.431328 os2borgerpc_client-2.2.0/os2borgerpc/client/
--rw-r--r--   0 m         (1000) m         (1000)       38 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.0/os2borgerpc/client/__init__.py
--rw-r--r--   0 m         (1000) m         (1000)     3841 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.0/os2borgerpc/client/admin_client.py
--rw-r--r--   0 m         (1000) m         (1000)     5518 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.0/os2borgerpc/client/config.py
--rw-r--r--   0 m         (1000) m         (1000)     1618 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.0/os2borgerpc/client/gateway.py
--rw-rw-r--   0 m         (1000) m         (1000)    19243 2023-02-28 13:56:42.000000 os2borgerpc_client-2.2.0/os2borgerpc/client/jobmanager.py
--rw-r--r--   0 m         (1000) m         (1000)      542 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.0/os2borgerpc/client/proxy_setup.py
-drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-03-09 09:58:02.432328 os2borgerpc_client-2.2.0/os2borgerpc/client/security/
--rw-r--r--   0 m         (1000) m         (1000)       53 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.0/os2borgerpc/client/security/__init__.py
--rw-r--r--   0 m         (1000) m         (1000)      391 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.0/os2borgerpc/client/security/csv_writer.py
--rw-r--r--   0 m         (1000) m         (1000)     1029 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.0/os2borgerpc/client/security/log_read.py
--rw-r--r--   0 m         (1000) m         (1000)     5254 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.0/os2borgerpc/client/security/security.py
--rw-rw-r--   0 m         (1000) m         (1000)     1382 2023-03-07 12:27:46.000000 os2borgerpc_client-2.2.0/os2borgerpc/client/updater.py
--rw-r--r--   0 m         (1000) m         (1000)     2768 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.0/os2borgerpc/client/utils.py
-drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-03-09 09:58:02.432328 os2borgerpc_client-2.2.0/os2borgerpc_client.egg-info/
--rwxr-xr-x   0 m         (1000) m         (1000)     1190 2023-03-09 09:58:01.000000 os2borgerpc_client-2.2.0/os2borgerpc_client.egg-info/PKG-INFO
--rwxr-xr-x   0 m         (1000) m         (1000)      942 2023-03-09 09:58:02.000000 os2borgerpc_client-2.2.0/os2borgerpc_client.egg-info/SOURCES.txt
--rwxr-xr-x   0 m         (1000) m         (1000)        1 2023-03-09 09:58:01.000000 os2borgerpc_client-2.2.0/os2borgerpc_client.egg-info/dependency_links.txt
--rwxr-xr-x   0 m         (1000) m         (1000)        1 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.0/os2borgerpc_client.egg-info/not-zip-safe
--rwxr-xr-x   0 m         (1000) m         (1000)       38 2023-03-09 09:58:02.000000 os2borgerpc_client-2.2.0/os2borgerpc_client.egg-info/requires.txt
--rwxr-xr-x   0 m         (1000) m         (1000)       12 2023-03-09 09:58:02.000000 os2borgerpc_client-2.2.0/os2borgerpc_client.egg-info/top_level.txt
--rw-rw-r--   0 m         (1000) m         (1000)       38 2023-03-09 09:58:02.433328 os2borgerpc_client-2.2.0/setup.cfg
--rw-rw-r--   0 m         (1000) m         (1000)     1221 2023-03-09 09:57:35.000000 os2borgerpc_client-2.2.0/setup.py
+drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-05-23 08:59:34.165174 os2borgerpc_client-2.2.1/
+-rw-r--r--   0 m         (1000) m         (1000)    35149 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.1/LICENSE
+-rw-rw-r--   0 m         (1000) m         (1000)     1190 2023-05-23 08:59:34.165174 os2borgerpc_client-2.2.1/PKG-INFO
+-rw-rw-r--   0 m         (1000) m         (1000)      755 2023-02-28 13:56:42.000000 os2borgerpc_client-2.2.1/README.rst
+drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-05-23 08:59:34.164174 os2borgerpc_client-2.2.1/bin/
+-rwxr-xr-x   0 m         (1000) m         (1000)      561 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.1/bin/admin_connect.sh
+-rwxr-xr-x   0 m         (1000) m         (1000)      731 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.1/bin/get_os2borgerpc_config
+-rwxrwxr-x   0 m         (1000) m         (1000)     1766 2023-05-23 08:51:25.000000 os2borgerpc_client-2.2.1/bin/jobmanager
+-rwxr-xr-x   0 m         (1000) m         (1000)      227 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.1/bin/os2borgerpc_find_gateway
+-rwxrwxr-x   0 m         (1000) m         (1000)      949 2023-02-28 13:56:42.000000 os2borgerpc_client-2.2.1/bin/os2borgerpc_push_config_keys
+-rwxrwxr-x   0 m         (1000) m         (1000)      845 2023-02-28 13:56:42.000000 os2borgerpc_client-2.2.1/bin/os2borgerpc_register_in_admin
+-rwxr-xr-x   0 m         (1000) m         (1000)     1862 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.1/bin/randomize_jobmanager.sh
+-rwxrwxr-x   0 m         (1000) m         (1000)     5260 2023-05-23 08:56:56.000000 os2borgerpc_client-2.2.1/bin/register_new_os2borgerpc_client.sh
+-rwxr-xr-x   0 m         (1000) m         (1000)      606 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.1/bin/set_os2borgerpc_config
+drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-05-23 08:59:34.163174 os2borgerpc_client-2.2.1/os2borgerpc/
+drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-05-23 08:59:34.164174 os2borgerpc_client-2.2.1/os2borgerpc/client/
+-rw-r--r--   0 m         (1000) m         (1000)       38 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.1/os2borgerpc/client/__init__.py
+-rw-r--r--   0 m         (1000) m         (1000)     3841 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.1/os2borgerpc/client/admin_client.py
+-rw-r--r--   0 m         (1000) m         (1000)     5518 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.1/os2borgerpc/client/config.py
+-rw-r--r--   0 m         (1000) m         (1000)     1618 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.1/os2borgerpc/client/gateway.py
+-rw-rw-r--   0 m         (1000) m         (1000)    19243 2023-02-28 13:56:42.000000 os2borgerpc_client-2.2.1/os2borgerpc/client/jobmanager.py
+-rw-r--r--   0 m         (1000) m         (1000)      542 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.1/os2borgerpc/client/proxy_setup.py
+drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-05-23 08:59:34.164174 os2borgerpc_client-2.2.1/os2borgerpc/client/security/
+-rw-r--r--   0 m         (1000) m         (1000)       53 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.1/os2borgerpc/client/security/__init__.py
+-rw-r--r--   0 m         (1000) m         (1000)      391 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.1/os2borgerpc/client/security/csv_writer.py
+-rw-r--r--   0 m         (1000) m         (1000)     1029 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.1/os2borgerpc/client/security/log_read.py
+-rw-r--r--   0 m         (1000) m         (1000)     5254 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.1/os2borgerpc/client/security/security.py
+-rw-rw-r--   0 m         (1000) m         (1000)     1382 2023-03-09 17:01:12.000000 os2borgerpc_client-2.2.1/os2borgerpc/client/updater.py
+-rw-r--r--   0 m         (1000) m         (1000)     2768 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.1/os2borgerpc/client/utils.py
+drwxrwxr-x   0 m         (1000) m         (1000)        0 2023-05-23 08:59:34.165174 os2borgerpc_client-2.2.1/os2borgerpc_client.egg-info/
+-rwxr-xr-x   0 m         (1000) m         (1000)     1190 2023-05-23 08:59:34.000000 os2borgerpc_client-2.2.1/os2borgerpc_client.egg-info/PKG-INFO
+-rwxr-xr-x   0 m         (1000) m         (1000)      942 2023-05-23 08:59:34.000000 os2borgerpc_client-2.2.1/os2borgerpc_client.egg-info/SOURCES.txt
+-rwxr-xr-x   0 m         (1000) m         (1000)        1 2023-05-23 08:59:34.000000 os2borgerpc_client-2.2.1/os2borgerpc_client.egg-info/dependency_links.txt
+-rwxr-xr-x   0 m         (1000) m         (1000)        1 2022-11-03 09:54:35.000000 os2borgerpc_client-2.2.1/os2borgerpc_client.egg-info/not-zip-safe
+-rwxr-xr-x   0 m         (1000) m         (1000)       38 2023-05-23 08:59:34.000000 os2borgerpc_client-2.2.1/os2borgerpc_client.egg-info/requires.txt
+-rwxr-xr-x   0 m         (1000) m         (1000)       12 2023-05-23 08:59:34.000000 os2borgerpc_client-2.2.1/os2borgerpc_client.egg-info/top_level.txt
+-rw-rw-r--   0 m         (1000) m         (1000)       38 2023-05-23 08:59:34.165174 os2borgerpc_client-2.2.1/setup.cfg
+-rw-rw-r--   0 m         (1000) m         (1000)     1221 2023-05-23 08:56:56.000000 os2borgerpc_client-2.2.1/setup.py
```

### Comparing `os2borgerpc_client-2.2.0/LICENSE` & `os2borgerpc_client-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.2.0/PKG-INFO` & `os2borgerpc_client-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os2borgerpc_client
-Version: 2.2.0
+Version: 2.2.1
 Summary: Client for the OS2borgerPC system
 Home-page: https://github.com/OS2borgerPC/
 Author: Magenta ApS
 Author-email: info@magenta-aps.dk
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `os2borgerpc_client-2.2.0/README.rst` & `os2borgerpc_client-2.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.2.0/bin/admin_connect.sh` & `os2borgerpc_client-2.2.1/bin/admin_connect.sh`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.2.0/bin/get_os2borgerpc_config` & `os2borgerpc_client-2.2.1/bin/get_os2borgerpc_config`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.2.0/bin/jobmanager` & `os2borgerpc_client-2.2.1/bin/jobmanager`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.2.0/bin/os2borgerpc_push_config_keys` & `os2borgerpc_client-2.2.1/bin/os2borgerpc_push_config_keys`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.2.0/bin/os2borgerpc_register_in_admin` & `os2borgerpc_client-2.2.1/bin/os2borgerpc_register_in_admin`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.2.0/bin/randomize_jobmanager.sh` & `os2borgerpc_client-2.2.1/bin/randomize_jobmanager.sh`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.2.0/bin/register_new_os2borgerpc_client.sh` & `os2borgerpc_client-2.2.1/bin/register_new_os2borgerpc_client.sh`

 * *Files 7% similar despite different names*

```diff
@@ -3,53 +3,53 @@
 SHARED_CONFIG="/tmp/os2borgerpc.conf"
 
 # Current directory
 DIR=$(dirname "${BASH_SOURCE[0]}")
 
 while true; do
     fatal() {
-        echo "Kritisk fejl, stopper:" "$@"
+        echo "Critical error. Halting registration:" "$@"
         while true; do
-            echo "[B]egynd forfra eller [S]top?"
+            echo "[R]estart or [C]ancel registration?"
             stty -echo
             read -rn 1 VALUE
             stty echo
             case "$VALUE" in
-                b|B)
+                r|R)
                     rm -f "$SHARED_CONFIG"
                     return 0 ;;
-                s|S)
+                c|C)
                     return 1 ;;
             esac
         done
     }
 
     # Get hold of config parameters, connect to admin system.
 
     # Attempt to get shared config file from gateway.
     # It this fails, the user must enter the corresponding data (site and
     # admin_url) manually.
     if [ "$(id -u)" != "0" ]
     then
-        fatal "Dette program skal køres som root" && continue || exit 1
+        fatal "This program must be run as root" && continue || exit 1
     fi
 
-    echo "Indtast gateway, tryk <ENTER> for ingen gateway eller automatisk opsætning"
+    echo "Press <ENTER> for no gateway or automatic setup. Alternatively, enter a gateway address:"
     read -r GATEWAY_IP
 
     if [[ -z "$GATEWAY_IP" ]]
     then
         # No gateway entered by user
         GATEWAY_SITE="http://$(os2borgerpc_find_gateway 2> /dev/null)"
     else
         # User entered IP address or hostname - test if reachable by ping
-        echo "Checker forbindelsen til gateway ..."
+        echo "Checking connection to the gateway ..."
         if ! ping -c 1 "$GATEWAY_IP" > /dev/null 2>&1
         then
-            fatal "Ugyldig gateway-adresse ($GATEWAY_IP)" && continue || exit 1
+            fatal "Invalid gateway address ($GATEWAY_IP)" && continue || exit 1
         else
             echo "OK"
         fi
         # Gateway is pingable - we assume that means it's OK.
         GATEWAY_SITE="http://$GATEWAY_IP"
         set_os2borgerpc_config gateway "$GATEWAY_IP"
     fi
@@ -57,116 +57,119 @@
     curl -s "$GATEWAY_SITE/os2borgerpc.conf" -o "$SHARED_CONFIG"
 
     unset HAS_GATEWAY
     if [[ -f "$SHARED_CONFIG" ]]
     then
         HAS_GATEWAY=1
     fi
+
+    echo ""
+
     # The following config parameters are needed to finalize the
     # installation:
     # - hostname
     #   Prompt user for new host name
-    echo "Indtast venligst et nyt navn for denne computer:" \
-         "Navnet skal have en længde ml. 1-63 tegn," \
-         "og gyldige tegn er a-z, A-Z, 0-9 og bindestreg (-)."
+    echo "Please enter a new name for this computer." \
+         "The name must have a length of 1-63 characters," \
+         "and valid characters are a-z, A-Z, 0-9 and hyphen (-):"
     # https://www.man7.org/linux/man-pages/man7/hostname.7.html
     read -r NEW_COMPUTER_NAME
     while [[ ! "$NEW_COMPUTER_NAME" =~ ^[0-9a-zA-Z][0-9a-zA-Z-]{1,63}$ ]]; do
-        echo "Ugyldigt computernavn.  Prøv igen."
+        echo "Invalid computer name. Try again:"
         read -r NEW_COMPUTER_NAME
     done
 
     # Idea: Allow uppercase in the computername due to popular demand,
     # but lowercase it so it's a valid hostname which is case insensitive
     NEW_HOSTNAME=$(echo "$NEW_COMPUTER_NAME" | tr '[:upper:]' '[:lower:]')
 
     echo "$NEW_HOSTNAME" > /etc/hostname
     set_os2borgerpc_config hostname "$NEW_HOSTNAME"
     hostname "$NEW_HOSTNAME"
     sed --in-place /127.0.1.1/d /etc/hosts
     sed --in-place "2i 127.0.1.1	$NEW_HOSTNAME" /etc/hosts
 
+    echo ""
 
     # - site
     #   TODO: Get site from gateway, if none present prompt user
     unset SITE
     if [[ -n "$HAS_GATEWAY" ]]
     then
         SITE="$(get_os2borgerpc_config site "$SHARED_CONFIG")"
     fi
 
     if [[ -z "$SITE" ]]
     then
-        echo "Indtast UID for det site, computeren skal tilmeldes:"
+        echo "Enter your site UID:"
         read -r SITE
     fi
 
     if [[ -n "$SITE" ]]
     then
         set_os2borgerpc_config site "$SITE"
     else
-        fatal "Computeren kan ikke registreres uden site" && continue || exit 1
+        fatal "The computer cannot be registered without a site" && continue || exit 1
     fi
 
 
     # - distribution
     # Detect OS version and prompt user for verification
 
     unset DISTRO
     if [[ -r /etc/os-release ]]; then
         # shellcheck source=/dev/null
-    	. /etc/os-release
+        . /etc/os-release
         DISTRO="$ID""$VERSION_ID"
     else
-        echo "Vi kan ikke se hvilket operativ system der er installeret." \
-             "Indtast venligst ID for PC'ens distribution:"
+        echo "We cannot detect the installed operating system." \
+             "Please enter an ID for the PC distribution:"
         read -r DISTRO
     fi
 
-    echo "Distributions ID: $DISTRO"
-
     set_os2borgerpc_config distribution "$DISTRO"
 
 
     # - mac
     #   Get the mac-address
     set_os2borgerpc_config mac "$(ip addr | grep link/ether | awk 'FNR==1{print $2}')"
 
+    echo ""
 
     # - admin_url
     #   Get from gateway, otherwise prompt user.
     unset ADMIN_URL
     if [[ -n "$HAS_GATEWAY" ]]
     then
         ADMIN_URL=$(get_os2borgerpc_config admin_url "$SHARED_CONFIG")
     fi
     if [[ -z "$ADMIN_URL" ]]
     then
         ADMIN_URL="https://os2borgerpc-admin.magenta.dk"
-        echo "Indtast admin-url hvis det ikke er $ADMIN_URL"
+        echo "Press <ENTER> to register with the following admin portal: $ADMIN_URL."
+        echo "Alternatively, type in your URL to another instance of the admin portal here:"
         read -r NEW_ADMIN_URL
         if [[ -n "$NEW_ADMIN_URL" ]]
         then
             ADMIN_URL="$NEW_ADMIN_URL"
         fi
     fi
     set_os2borgerpc_config admin_url "$ADMIN_URL"
 
     # OK, we got the config.
     # Do the deed.
     if ! os2borgerpc_register_in_admin "$NEW_COMPUTER_NAME"; then
-        fatal "Tilmelding mislykkedes" && continue || exit 1
+        fatal "Registration failed" && continue || exit 1
     fi
 
     # Now setup cron job
     if [[ -f $(command -v jobmanager) ]]
     then
         echo 'PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin' > /etc/cron.d/os2borgerpc-jobmanager
         echo "*/5 * * * * root $(command -v jobmanager)" >> /etc/cron.d/os2borgerpc-jobmanager
     fi
 
     # Now randomize cron job to avoid everybody hitting the server every five minutes.
     "$DIR/randomize_jobmanager.sh" 5 > /dev/null
 
-
     break
 done
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `os2borgerpc_client-2.2.0/bin/set_os2borgerpc_config` & `os2borgerpc_client-2.2.1/bin/set_os2borgerpc_config`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.2.0/os2borgerpc/client/admin_client.py` & `os2borgerpc_client-2.2.1/os2borgerpc/client/admin_client.py`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.2.0/os2borgerpc/client/config.py` & `os2borgerpc_client-2.2.1/os2borgerpc/client/config.py`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.2.0/os2borgerpc/client/gateway.py` & `os2borgerpc_client-2.2.1/os2borgerpc/client/gateway.py`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.2.0/os2borgerpc/client/jobmanager.py` & `os2borgerpc_client-2.2.1/os2borgerpc/client/jobmanager.py`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.2.0/os2borgerpc/client/proxy_setup.py` & `os2borgerpc_client-2.2.1/os2borgerpc/client/proxy_setup.py`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.2.0/os2borgerpc/client/security/log_read.py` & `os2borgerpc_client-2.2.1/os2borgerpc/client/security/log_read.py`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.2.0/os2borgerpc/client/security/security.py` & `os2borgerpc_client-2.2.1/os2borgerpc/client/security/security.py`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.2.0/os2borgerpc/client/updater.py` & `os2borgerpc_client-2.2.1/os2borgerpc/client/updater.py`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.2.0/os2borgerpc/client/utils.py` & `os2borgerpc_client-2.2.1/os2borgerpc/client/utils.py`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.2.0/os2borgerpc_client.egg-info/PKG-INFO` & `os2borgerpc_client-2.2.1/os2borgerpc_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os2borgerpc-client
-Version: 2.2.0
+Version: 2.2.1
 Summary: Client for the OS2borgerPC system
 Home-page: https://github.com/OS2borgerPC/
 Author: Magenta ApS
 Author-email: info@magenta-aps.dk
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `os2borgerpc_client-2.2.0/os2borgerpc_client.egg-info/SOURCES.txt` & `os2borgerpc_client-2.2.1/os2borgerpc_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `os2borgerpc_client-2.2.0/setup.py` & `os2borgerpc_client-2.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 setup(
     # Keep this name in sync with the one in os2borgerpc_client/jobmanager.py
     name="os2borgerpc_client",
-    version="2.2.0",
+    version="2.2.1",
     description="Client for the OS2borgerPC system",
     long_description=long_description,
     url="https://github.com/OS2borgerPC/",
     author="Magenta ApS",
     author_email="info@magenta-aps.dk",
     license="GPLv3",
     packages=["os2borgerpc.client", "os2borgerpc.client.security"],
```

