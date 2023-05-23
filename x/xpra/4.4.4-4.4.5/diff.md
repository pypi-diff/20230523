# Comparing `tmp/xpra-4.4.4.tar.gz` & `tmp/xpra-4.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpra-4.4.4.tar", last modified: Fri Mar 10 09:32:39 2023, max compression
+gzip compressed data, was "xpra-4.4.5.tar", last modified: Tue May 23 12:16:26 2023, max compression
```

## Comparing `xpra-4.4.4.tar` & `xpra-4.4.5.tar`

### file list

```diff
@@ -1,1490 +1,1490 @@
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.616879 xpra-4.4.4/
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.487880 xpra-4.4.4/.github/
--rw-r--r--   0 antoine   (1000) antoine   (1000)       15 2023-02-24 14:18:37.000000 xpra-4.4.4/.github/FUNDING.yml
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.487880 xpra-4.4.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      623 2023-01-13 05:35:59.000000 xpra-4.4.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)      604 2023-01-13 05:35:59.000000 xpra-4.4.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4142 2023-02-24 14:18:37.000000 xpra-4.4.4/.gitignore
--rw-r--r--   0 antoine   (1000) antoine   (1000)    17987 2023-03-10 09:32:07.000000 xpra-4.4.4/COPYING
--rw-r--r--   0 antoine   (1000) antoine   (1000)      918 2023-03-10 09:32:07.000000 xpra-4.4.4/MANIFEST.in
--rw-r--r--   0 antoine   (1000) antoine   (1000)      440 2023-03-10 09:32:39.615879 xpra-4.4.4/PKG-INFO
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4408 2023-03-10 09:32:07.000000 xpra-4.4.4/README.md
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.488880 xpra-4.4.4/docs/
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.488880 xpra-4.4.4/docs/Build/
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3746 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Build/Debian.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     8384 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Build/Dependencies.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)      997 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Build/MSWindows.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1642 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Build/MacOS.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4894 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Build/Other.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1016 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Build/README.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2431 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Build/RPM.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)   119794 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/CHANGELOG.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     7792 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/FAQ.md
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.490880 xpra-4.4.4/docs/Features/
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3483 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Features/Audio.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     7617 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Features/Clipboard.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4604 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Features/DPI.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)      363 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Features/Display.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1602 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Features/File-Transfers.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2023 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Features/Image-Depth.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2619 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Features/Keyboard.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1365 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Features/Notifications.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3818 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Features/Printing.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1293 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Features/README.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1385 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Features/System-Tray.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2479 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Features/Webcam.md
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.490880 xpra-4.4.4/docs/Network/
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3177 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Network/AES.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)      489 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Network/Encryption.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1057 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Network/Multicast-DNS.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3810 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Network/README.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4668 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Network/SSH.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5634 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Network/SSL.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2285 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/README.md
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.492880 xpra-4.4.4/docs/Usage/
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1718 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Usage/Apache-Proxy.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)    11800 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Usage/Authentication.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3833 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Usage/Client-OpenGL.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2735 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Usage/Client.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1615 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Usage/Configuration.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     7359 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Usage/Encodings.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     6558 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Usage/Logging.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4082 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Usage/NVENC.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2476 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Usage/OpenGL.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     8928 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Usage/Proxy-Server.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4628 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Usage/README.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)      954 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Usage/Seamless.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)    17482 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Usage/Security.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1211 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Usage/Service.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3429 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Usage/Shadow-Server.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1942 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Usage/Start-Desktop.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3721 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Usage/WSL.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     6536 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/Usage/Xdummy.md
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.493880 xpra-4.4.4/docs/images/
--rw-r--r--   0 antoine   (1000) antoine   (1000)    29145 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/Xpra-Proxy.png
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.495880 xpra-4.4.4/docs/images/icons/
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3531 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/icons/X11.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2083 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/icons/authentication.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1441 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/icons/clipboard.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1664 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/icons/connect.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)      496 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/icons/debian.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2971 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/icons/encoding.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3857 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/icons/freebsd.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3090 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/icons/keyboard.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1506 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/icons/mdns.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3757 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/icons/nvidia.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2711 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/icons/opengl.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3555 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/icons/osx.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1932 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/icons/package.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3317 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/icons/printer.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1816 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/icons/rpm.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1326 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/icons/server-connected.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5009 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/icons/sound.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4227 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/icons/ssh.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     7147 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/icons/ubuntu.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2617 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/icons/upload.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2581 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/icons/webcam.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3944 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/icons/windows.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)    37557 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/mdns-gui.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)    29526 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/pavucontrol-client.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)    31507 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/pavucontrol-server.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)    45427 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/session-info-graphs.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)    39729 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/session-info-sound.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3934 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/upload.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)    10673 2023-03-10 09:32:07.000000 xpra-4.4.4/docs/images/win32-shadow-tray-menu.png
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.495880 xpra-4.4.4/fs/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      598 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/README.md
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.495880 xpra-4.4.4/fs/bin/
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    13395 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/bin/add_build_info.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      152 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/bin/links-to-html.lua
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4026 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/bin/run_scaled
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1848 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/bin/set_source_version
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2611 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/bin/xdummy_cvt_gen.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      187 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/bin/xpra
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2596 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/bin/xpra_Xdummy
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      272 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/bin/xpra_launcher
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.495880 xpra-4.4.4/fs/etc/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      864 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/README.md
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.477880 xpra-4.4.4/fs/etc/X11/
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.496880 xpra-4.4.4/fs/etc/X11/xorg.conf.d/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      226 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/X11/xorg.conf.d/90-xpra-virtual.conf
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.477880 xpra-4.4.4/fs/etc/dbus-1/
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.496880 xpra-4.4.4/fs/etc/dbus-1/system.d/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      499 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/dbus-1/system.d/xpra.conf
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.496880 xpra-4.4.4/fs/etc/default/
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      242 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/default/xpra
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.496880 xpra-4.4.4/fs/etc/init.d/
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2279 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/init.d/xpra
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.496880 xpra-4.4.4/fs/etc/pam.d/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      760 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/pam.d/xpra
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.496880 xpra-4.4.4/fs/etc/sysconfig/
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      242 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/sysconfig/xpra
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.497880 xpra-4.4.4/fs/etc/xpra/
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.498880 xpra-4.4.4/fs/etc/xpra/conf.d/
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1115 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/conf.d/05_features.conf.in
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1883 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/conf.d/10_network.conf.in
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1678 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/conf.d/12_ssl.conf.in
--rw-r--r--   0 antoine   (1000) antoine   (1000)      501 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/conf.d/15_file_transfers.conf.in
--rw-r--r--   0 antoine   (1000) antoine   (1000)      769 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/conf.d/16_printing.conf.in
--rw-r--r--   0 antoine   (1000) antoine   (1000)      943 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/conf.d/20_sound.conf.in
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2270 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/conf.d/30_picture.conf.in
--rw-r--r--   0 antoine   (1000) antoine   (1000)      175 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/conf.d/35_webcam.conf.in
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1856 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/conf.d/40_client.conf.in
--rw-r--r--   0 antoine   (1000) antoine   (1000)      981 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/conf.d/42_client_keyboard.conf.in
--rw-r--r--   0 antoine   (1000) antoine   (1000)      232 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/conf.d/45_osx.conf.in
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2226 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/conf.d/50_server_network.conf.in
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1421 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/conf.d/55_server_x11.conf.in
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3249 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/conf.d/60_server.conf.in
--rw-r--r--   0 antoine   (1000) antoine   (1000)      379 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/conf.d/65_proxy.conf.in
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.498880 xpra-4.4.4/fs/etc/xpra/content-categories/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      644 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/content-categories/10_default.conf
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.498880 xpra-4.4.4/fs/etc/xpra/content-parent/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      147 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/content-parent/10_default.conf
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.498880 xpra-4.4.4/fs/etc/xpra/content-type/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      262 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/content-type/10_role.conf
--rw-r--r--   0 antoine   (1000) antoine   (1000)      735 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/content-type/30_title.conf
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4653 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/content-type/50_class.conf
--rw-r--r--   0 antoine   (1000) antoine   (1000)      158 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/content-type/70_commands.conf
--rw-r--r--   0 antoine   (1000) antoine   (1000)      674 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/cuda.conf
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.499880 xpra-4.4.4/fs/etc/xpra/http-headers/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      121 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/http-headers/00_nocache.txt
--rw-r--r--   0 antoine   (1000) antoine   (1000)      397 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/http-headers/10_content_security_policy.txt
--rw-r--r--   0 antoine   (1000) antoine   (1000)      137 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/nvenc.keys
--rw-r--r--   0 antoine   (1000) antoine   (1000)      214 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/nvfbc.keys
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2872 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/xorg-randr1.6.conf
--rw-r--r--   0 antoine   (1000) antoine   (1000)   154106 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/xorg-uinput.conf
--rw-r--r--   0 antoine   (1000) antoine   (1000)   154253 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/xorg.conf
--rw-r--r--   0 antoine   (1000) antoine   (1000)      734 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/etc/xpra/xpra.conf.in
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.499880 xpra-4.4.4/fs/lib/
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1132 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/lib/README.md
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.477880 xpra-4.4.4/fs/lib/cups/
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.499880 xpra-4.4.4/fs/lib/cups/backend/
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     6922 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/lib/cups/backend/xpraforwarder
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.499880 xpra-4.4.4/fs/lib/pkgconfig/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      208 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/lib/pkgconfig/README.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)      231 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/lib/pkgconfig/cuda.pc
--rw-r--r--   0 antoine   (1000) antoine   (1000)      220 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/lib/pkgconfig/nvenc.pc
--rw-r--r--   0 antoine   (1000) antoine   (1000)      218 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/lib/pkgconfig/nvfbc.pc
--rw-r--r--   0 antoine   (1000) antoine   (1000)      233 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/lib/pkgconfig/nvjpeg.pc
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.478880 xpra-4.4.4/fs/lib/systemd/
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.499880 xpra-4.4.4/fs/lib/systemd/system/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      751 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/lib/systemd/system/xpra-nosocketactivation.service
--rw-r--r--   0 antoine   (1000) antoine   (1000)      816 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/lib/systemd/system/xpra.service
--rw-r--r--   0 antoine   (1000) antoine   (1000)      300 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/lib/systemd/system/xpra.socket
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.499880 xpra-4.4.4/fs/lib/sysusers.d/
--rw-r--r--   0 antoine   (1000) antoine   (1000)       10 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/lib/sysusers.d/xpra.conf
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.500880 xpra-4.4.4/fs/lib/tmpfiles.d/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      174 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/lib/tmpfiles.d/xpra.conf
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.478880 xpra-4.4.4/fs/lib/udev/
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.500880 xpra-4.4.4/fs/lib/udev/rules.d/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      491 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/lib/udev/rules.d/71-xpra-virtual-pointer.rules
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.478880 xpra-4.4.4/fs/libexec/
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.500880 xpra-4.4.4/fs/libexec/xpra/
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)       94 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/libexec/xpra/auth_dialog
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3748 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/libexec/xpra/gnome-open
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3748 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/libexec/xpra/gvfs-open
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3748 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/libexec/xpra/xdg-open
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      674 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/libexec/xpra/xpra_signal_listener
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      397 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/libexec/xpra/xpra_udev_product_version
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.479880 xpra-4.4.4/fs/share/
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.500880 xpra-4.4.4/fs/share/applications/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      193 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/applications/xpra-gui.desktop
--rw-r--r--   0 antoine   (1000) antoine   (1000)      304 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/applications/xpra-launcher.desktop
--rw-r--r--   0 antoine   (1000) antoine   (1000)      270 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/applications/xpra-shadow.desktop
--rw-r--r--   0 antoine   (1000) antoine   (1000)      602 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/applications/xpra.desktop
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.501880 xpra-4.4.4/fs/share/icons/
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1474 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/icons/xpra-mdns.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1326 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/icons/xpra-shadow.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)   434275 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/icons/xpra.icns
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3011 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/icons/xpra.png
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.478880 xpra-4.4.4/fs/share/man/
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.502880 xpra-4.4.4/fs/share/man/man1/
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2061 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/man/man1/run_scaled.1
--rw-r--r--   0 antoine   (1000) antoine   (1000)    73349 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/man/man1/xpra.1
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2243 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/man/man1/xpra_launcher.1
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.502880 xpra-4.4.4/fs/share/metainfo/
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1978 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/metainfo/xpra.appdata.xml
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.478880 xpra-4.4.4/fs/share/mime/
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.502880 xpra-4.4.4/fs/share/mime/packages/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      256 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/mime/packages/application-x-xpraconfig.xml
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.479880 xpra-4.4.4/fs/share/selinux/
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.502880 xpra-4.4.4/fs/share/selinux/cups_xpra/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      256 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/selinux/cups_xpra/README.TXT
--rw-r--r--   0 antoine   (1000) antoine   (1000)       90 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/selinux/cups_xpra/cups_xpra.fc
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1282 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/selinux/cups_xpra/cups_xpra.te
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.502880 xpra-4.4.4/fs/share/selinux/xpra_socketactivation/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      343 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/selinux/xpra_socketactivation/README.TXT
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1393 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/selinux/xpra_socketactivation/xpra_socketactivation.fc
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5354 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/selinux/xpra_socketactivation/xpra_socketactivation.te
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.502880 xpra-4.4.4/fs/share/xpra/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      258 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/autostart.desktop
--rw-r--r--   0 antoine   (1000) antoine   (1000)    24648 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/bell.wav
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.503880 xpra-4.4.4/fs/share/xpra/css/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      493 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/css/10_header_bar.css
--rw-r--r--   0 antoine   (1000) antoine   (1000)      355 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/css/20_progress_bar.css
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.503880 xpra-4.4.4/fs/share/xpra/cuda/
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1072 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/cuda/BGRA_to_RGBAP.cu
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2873 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/cuda/BGRX_to_NV12.cu
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1039 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/cuda/BGRX_to_RGB.cu
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1330 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/cuda/BGRX_to_YUV444.cu
--rw-r--r--   0 antoine   (1000) antoine   (1000)      281 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/cuda/README.md
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1072 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/cuda/RGBA_to_RGBAP.cu
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1039 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/cuda/RGBX_to_RGB.cu
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2882 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/cuda/XRGB_to_NV12.cu
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1332 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/cuda/XRGB_to_YUV444.cu
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.516880 xpra-4.4.4/fs/share/xpra/icons/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      659 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/audio.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/authentication.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2083 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/authentication.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4161 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/bandwidth_limit.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/bell.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1636 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/bell.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/browse.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3739 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/browse.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1136 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/browser.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9462 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/bugs.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2283 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/bugs.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/clipboard.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1441 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/clipboard.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3629 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/close.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2343 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/compressed.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1664 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/connect.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)    16958 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/cuda.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/directory.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2407 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/disconnected.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)    12774 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/display.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1170 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/documentation.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3887 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/download.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1304 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/empty.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/encoding.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2971 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/encoding.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5633 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/eye-off.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5385 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/eye-on.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/features.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2889 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/features.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1789 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/fluxbox.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/font.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1607 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/font.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4198 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/forward.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3857 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/freebsd.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/gears.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4332 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/gnome-session.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4332 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/gnome.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/gstreamer.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)    25214 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/gtk.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/information.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2742 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/information.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4463 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/kde.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)    67646 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/keyboard.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3090 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/keyboard.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/keymap.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3173 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/linux.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2305 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/list.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/loop.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3062 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/lxde.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3555 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/macos.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2284 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/matchbox.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3875 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/maximize.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/mdns.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1506 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/mdns.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/microphone.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3748 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/microphone.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)      819 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/minimize.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/network.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)      133 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/noicon.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/nvidia.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2331 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/open.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1760 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/openbox.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5242 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/openbsd.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/opengl.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2711 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/opengl.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1932 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/package.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1477 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/picture.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2018 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/pointer.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/printer.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3317 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/printer.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)    16958 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/python.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1703 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/qr.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1013 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/quit.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3067 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/raise.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4907 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/reinitialize.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1618 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/retry.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1999 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/sawfish.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1272 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/scaling.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/screenshot.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1883 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/screenshot.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)    19246 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/server-connected.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1326 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/server-connected.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)    34494 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/server-notconnected.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1046 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/server-notconnected.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)      527 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/server.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)      874 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/shutdown.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1085 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/slider.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4384 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/speaker-off.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/speaker.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4583 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/speaker.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3337 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/speed.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/sql.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/sqlite.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1586 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/sqlite.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9318 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/start.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1851 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/statistics.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)      794 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/ticked-small.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     8814 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/ticked.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1251 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/timer.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2060 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/toolbox.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1157 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/transfer.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/transparent.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)      312 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/transparent.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)      290 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/unticked-small.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     8711 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/unticked.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4905 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/update.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)    14087 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/upload.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3480 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/user.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)      902 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/video.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)    16958 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/webcam.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2581 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/webcam.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3944 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/win32.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4304 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/windowmaker.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2146 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/windows.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/xpra.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2353 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/xpra.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3774 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/xpra_txt.ico
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1498 2023-03-10 09:32:07.000000 xpra-4.4.4/fs/share/xpra/icons/xterm.png
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.480880 xpra-4.4.4/packaging/
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.518880 xpra-4.4.4/packaging/MSWindows/
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      464 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MSWindows/ALL_RELEASE_BUILDS.sh
--rw-r--r--   0 antoine   (1000) antoine   (1000)      687 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MSWindows/BUILD_CUDA_KERNEL.BAT
--rw-r--r--   0 antoine   (1000) antoine   (1000)   143740 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MSWindows/DirectShow.tlb
--rw-r--r--   0 antoine   (1000) antoine   (1000)    21443 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MSWindows/MINGW_BUILD.sh
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3376 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MSWindows/MINGW_SETUP.sh
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1202 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MSWindows/SIGN_ALL.sh
--rw-r--r--   0 antoine   (1000) antoine   (1000)     6832 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MSWindows/TaskbarLib.tlb
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MSWindows/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      446 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MSWindows/gen_win32con.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1029 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MSWindows/msi.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     8585 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MSWindows/msi.xml
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.518880 xpra-4.4.4/packaging/MSWindows/pkgconfig/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      233 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MSWindows/pkgconfig/cuda.pc
--rw-r--r--   0 antoine   (1000) antoine   (1000)      325 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MSWindows/pkgconfig/nvenc.pc
--rw-r--r--   0 antoine   (1000) antoine   (1000)      193 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MSWindows/pkgconfig/nvfbc.pc
--rw-r--r--   0 antoine   (1000) antoine   (1000)      251 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MSWindows/pkgconfig/nvjpeg.pc
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.518880 xpra-4.4.4/packaging/MSWindows/service/
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.519879 xpra-4.4.4/packaging/MSWindows/service/DesktopLogon/
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3599 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MSWindows/service/DesktopLogon/DesktopLogon.cs
--rw-r--r--   0 antoine   (1000) antoine   (1000)     6066 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MSWindows/service/DesktopLogon/DesktopLogon.csproj
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1482 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MSWindows/service/DesktopLogon/DesktopLogon.sln
--rw-r--r--   0 antoine   (1000) antoine   (1000)    15694 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MSWindows/service/Xpra-Service.cpp
--rw-r--r--   0 antoine   (1000) antoine   (1000)      644 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MSWindows/service/event_log.mc
--rw-r--r--   0 antoine   (1000) antoine   (1000)       41 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MSWindows/website.url
--rw-r--r--   0 antoine   (1000) antoine   (1000)   154542 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MSWindows/xpra-logo.bmp
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9798 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MSWindows/xpra.bmp
--rw-r--r--   0 antoine   (1000) antoine   (1000)    13700 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MSWindows/xpra.iss
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.522879 xpra-4.4.4/packaging/MacOS/
--rw-r--r--   0 antoine   (1000) antoine   (1000)   494603 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Blank.dmg.bz2
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1422 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/C-wrapper.c
--rw-r--r--   0 antoine   (1000) antoine   (1000)    61482 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/GPL.rtf
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.525879 xpra-4.4.4/packaging/MacOS/Helpers/
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      292 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Auth_Dialog
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      280 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Browser
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      288 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Bug_Report
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      273 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Config_info
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      280 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Encoding_info
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      299 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Example-Colors
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      308 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Example-Colors-Gradient
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      305 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Example-Colors-Plain
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      311 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Example-OpenGL-Colors-Gradient
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      311 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Example-Transparent-Colors
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      311 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Example-Transparent-Window
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      276 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Feature_info
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      279 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/GStreamer_info
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      275 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/GTK_info
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      287 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Keyboard_Tool
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      276 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Keyboard_info
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      276 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Keymap_info
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      306 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Launcher
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      510 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Manual
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      271 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/NativeGUI_info
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      271 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Network_info
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      287 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/OpenGL_check
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      273 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Path_info
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      278 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/PowerMonitor
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      295 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Print
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      187 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Python
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3495 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/PythonExecWrapper
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      287 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/SQL_auth_tool
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      290 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/SQLite_auth_tool
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      560 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Shadow
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      283 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/U2F_Tool
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      274 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Version_info
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      289 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Webcam_Test
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      415 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Helpers/Xpra
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1452 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Info-template.plist
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2497 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Info.plist
--rw-r--r--   0 antoine   (1000) antoine   (1000)      291 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Inherit.entitlements
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1683 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Shell-wrapper.c
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3486 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Xpra.bundle
--rw-r--r--   0 antoine   (1000) antoine   (1000)      861 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Xpra.entitlements
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.479880 xpra-4.4.4/packaging/MacOS/Xpra_NoDock.app/
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.526879 xpra-4.4.4/packaging/MacOS/Xpra_NoDock.app/Contents/
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1449 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/Xpra_NoDock.app/Contents/Info.plist
--rw-r--r--   0 antoine   (1000) antoine   (1000)     8989 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/background.png
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.526879 xpra-4.4.4/packaging/MacOS/dmg-icons/
--rw-r--r--   0 antoine   (1000) antoine   (1000)    16374 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/dmg-icons/background.jpg
--rw-r--r--   0 antoine   (1000) antoine   (1000)    28638 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/dmg-icons/icon.png
--rw-r--r--   0 antoine   (1000) antoine   (1000)       57 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/gtkrc
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2110 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/make-DMG.sh
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4273 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/make-PKG.sh
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      154 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/make-all.sh
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    15399 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/make-app.sh
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4608 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/make-appstore-PKG.sh
--rw-r--r--   0 antoine   (1000) antoine   (1000)      353 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/org.xpra.Agent.plist
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1734 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/postinstall
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      341 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/sign-app.sh
--rw-r--r--   0 antoine   (1000) antoine   (1000)   434275 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/MacOS/xpra.icns
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.526879 xpra-4.4.4/packaging/debian/
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      217 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/build.sh
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.480880 xpra-4.4.4/packaging/debian/libcuda1/
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.526879 xpra-4.4.4/packaging/debian/libcuda1/DEBIAN/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      314 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/libcuda1/DEBIAN/control
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)       51 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/libcuda1.sh
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.480880 xpra-4.4.4/packaging/debian/libnvidia-fbc1/
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.526879 xpra-4.4.4/packaging/debian/libnvidia-fbc1/DEBIAN/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      325 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/libnvidia-fbc1/DEBIAN/control
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)       63 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/libnvidia-fbc1.sh
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.528880 xpra-4.4.4/packaging/debian/xpra/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      402 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xpra/README.Debian
--rw-r--r--   0 antoine   (1000) antoine   (1000)    93326 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xpra/changelog
--rw-r--r--   0 antoine   (1000) antoine   (1000)        3 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xpra/compat
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5307 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xpra/control
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3557 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xpra/copyright
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.528880 xpra-4.4.4/packaging/debian/xpra/patches/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      785 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xpra/patches/pam.patch
--rw-r--r--   0 antoine   (1000) antoine   (1000)       31 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xpra/patches/series
--rw-r--r--   0 antoine   (1000) antoine   (1000)      432 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xpra/patches/service-config.patch
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1246 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xpra/rules
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.528880 xpra-4.4.4/packaging/debian/xpra/source/
--rw-r--r--   0 antoine   (1000) antoine   (1000)       12 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xpra/source/format
--rw-r--r--   0 antoine   (1000) antoine   (1000)       19 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xpra/source/options
--rw-r--r--   0 antoine   (1000) antoine   (1000)       64 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xpra/watch
--rw-r--r--   0 antoine   (1000) antoine   (1000)       10 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xpra/xpra.docs
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1008 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xpra/xpra.install
--rw-r--r--   0 antoine   (1000) antoine   (1000)       57 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xpra/xpra.links
--rw-r--r--   0 antoine   (1000) antoine   (1000)      301 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xpra/xpra.lintian-overrides
--rw-r--r--   0 antoine   (1000) antoine   (1000)       83 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xpra/xpra.manpages
--rw-r--r--   0 antoine   (1000) antoine   (1000)      544 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xpra/xpra.postinst
--rw-r--r--   0 antoine   (1000) antoine   (1000)      204 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xpra/xpra.postrm
--rw-r--r--   0 antoine   (1000) antoine   (1000)      824 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xpra/xpra.service
--rw-r--r--   0 antoine   (1000) antoine   (1000)      300 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xpra/xpra.socket
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2141 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xpra.sh
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.529879 xpra-4.4.4/packaging/debian/xserver-xorg-video-dummy/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      989 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xserver-xorg-video-dummy/changelog
--rw-r--r--   0 antoine   (1000) antoine   (1000)        2 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xserver-xorg-video-dummy/compat
--rw-r--r--   0 antoine   (1000) antoine   (1000)      838 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xserver-xorg-video-dummy/control
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1420 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xserver-xorg-video-dummy/copyright
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.529879 xpra-4.4.4/packaging/debian/xserver-xorg-video-dummy/patches/
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3180 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xserver-xorg-video-dummy/patches/0002-Constant-DPI.patch
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1776 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xserver-xorg-video-dummy/patches/0006-Dummy-Disconnect.patch
--rw-r--r--   0 antoine   (1000) antoine   (1000)       51 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xserver-xorg-video-dummy/patches/series
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      271 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xserver-xorg-video-dummy/rules
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      661 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/debian/xserver-xorg-video-dummy.sh
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.531880 xpra-4.4.4/packaging/rpm/
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.532879 xpra-4.4.4/packaging/rpm/distros/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      224 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/distros/almalinux.list
--rw-r--r--   0 antoine   (1000) antoine   (1000)      187 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/distros/arm64.list
--rw-r--r--   0 antoine   (1000) antoine   (1000)      238 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/distros/centos-8.list
--rw-r--r--   0 antoine   (1000) antoine   (1000)      208 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/distros/centos-arm64.list
--rw-r--r--   0 antoine   (1000) antoine   (1000)      207 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/distros/centos-stream9.list
--rw-r--r--   0 antoine   (1000) antoine   (1000)      187 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/distros/default.list
--rw-r--r--   0 antoine   (1000) antoine   (1000)      202 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/distros/fedora-37.list
--rw-r--r--   0 antoine   (1000) antoine   (1000)      243 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/distros/oraclelinux.list
--rw-r--r--   0 antoine   (1000) antoine   (1000)      224 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/distros/rockylinux.list
--rw-r--r--   0 antoine   (1000) antoine   (1000)      370 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/fake-cuda.spec
--rw-r--r--   0 antoine   (1000) antoine   (1000)    11873 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/ffmpeg-xpra.spec
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1596 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/gstreamer1-plugin-timestamp.spec
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1777 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/libfakeXinerama.spec
--rw-r--r--   0 antoine   (1000) antoine   (1000)     8115 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/libyuv.spec
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1305 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/nasm.spec
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.534880 xpra-4.4.4/packaging/rpm/patches/
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3180 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/patches/0002-Constant-DPI.patch
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1776 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/patches/0006-Dummy-Disconnect.patch
--rw-r--r--   0 antoine   (1000) antoine   (1000)      770 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/patches/libyuv-0001-Use-a-proper-so-version.patch
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1040 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/patches/libyuv-0002-Link-against-shared-library.patch
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1467 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/patches/libyuv-0003-Disable-static-library.patch
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1313 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/patches/libyuv-0004-Don-t-install-conversion-tool.patch
--rw-r--r--   0 antoine   (1000) antoine   (1000)      648 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/patches/libyuv-0005-Use-library-suffix-during-installation.patch
--rw-r--r--   0 antoine   (1000) antoine   (1000)      592 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/patches/libyuv-0006-Link-main-library-against-libjpeg.patch
--rw-r--r--   0 antoine   (1000) antoine   (1000)      513 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/patches/libyuv-0007-nojpeg.patch
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2451 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/patches/nasm-SourceSans-font-name.patch
--rw-r--r--   0 antoine   (1000) antoine   (1000)      319 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/patches/python-rencode-nowheelreq.patch
--rw-r--r--   0 antoine   (1000) antoine   (1000)    16815 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/patches/python-rencode-readdmissingpyx.patch
--rw-r--r--   0 antoine   (1000) antoine   (1000)      318 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/patches/python-rencode-rename.patch
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1123 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/patches/python-rencode-typecode-dos.patch
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1882 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/python3-Cython.spec
--rw-r--r--   0 antoine   (1000) antoine   (1000)    10523 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/python3-cairo.spec
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1687 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/python3-lz4.spec
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1641 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/python3-pbr.spec
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1362 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/python3-pkgconfig.spec
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5218 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/python3-pycuda.spec
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2740 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/python3-pynvml.spec
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5870 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/python3-pyopengl.spec
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3005 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/python3-pytools.spec
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2145 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/python3-pyu2f.spec
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4297 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/python3-rencode.spec
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3785 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/python3-uinput.spec
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2450 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/x264-xpra.spec
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2961 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/xorg-x11-drv-dummy.spec
--rw-r--r--   0 antoine   (1000) antoine   (1000)    99461 2023-03-10 09:32:07.000000 xpra-4.4.4/packaging/rpm/xpra.spec
--rw-r--r--   0 antoine   (1000) antoine   (1000)       38 2023-03-10 09:32:39.616879 xpra-4.4.4/setup.cfg
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)   105778 2023-03-10 09:32:07.000000 xpra-4.4.4/setup.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.534880 xpra-4.4.4/tests/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      112 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/__init__.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.534880 xpra-4.4.4/tests/perf/
--rw-r--r--   0 antoine   (1000) antoine   (1000)    12710 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/perf/perf_config_default.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    47773 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/perf/test_measure_perf.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    15741 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/perf/test_measure_perf_chartreps.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    14540 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/perf/test_measure_perf_charts.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.534880 xpra-4.4.4/tests/scripts/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      113 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/scripts/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      258 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/scripts/cProfile
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    27771 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/scripts/pycallgraph
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.535879 xpra-4.4.4/tests/unittests/
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1478 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/run
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.536879 xpra-4.4.4/tests/unittests/unit/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/__init__.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.536879 xpra-4.4.4/tests/unittests/unit/buffers/
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2526 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/buffers/cyxor_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3360 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/child_reaper_test.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.537879 xpra-4.4.4/tests/unittests/unit/client/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      189 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3608 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/auth_handlers_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      874 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/border_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3198 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/keyboard_helper_test.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.539879 xpra-4.4.4/tests/unittests/unit/client/mixins/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/mixins/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     7331 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/mixins/audioclient_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3650 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/mixins/clientmixintest_util.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1105 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/mixins/clipboard_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1642 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/mixins/display_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2191 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/mixins/encodings_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1844 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/mixins/mmap_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1106 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/mixins/networkstate_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      737 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/mixins/notifications_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1645 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/mixins/remotelogging_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1436 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/mixins/serverinfo_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      961 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/mixins/stubclient_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      935 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/mixins/tray_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1121 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/mixins/webcam_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1239 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/mixins/window_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      933 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/osxlike_clipboard_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      665 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/paint_colors_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3174 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/splash_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     5341 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/x11_client_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1155 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/x11_client_test_util.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      931 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/x11_clipboard_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3739 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/client/x11_clipboard_test_util.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.540879 xpra-4.4.4/tests/unittests/unit/codecs/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/codecs/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2652 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/codecs/argb_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2438 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/codecs/codecs_selftest_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3594 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/codecs/csc_colorspace_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     5000 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/codecs/image_wrapper_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      826 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/codecs/nvutil_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4549 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/codecs/pillow_encoder_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2736 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/codecs/pillow_header_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2474 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/codecs/rgb_transform_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4716 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/codecs/video_colorspace_test.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.540879 xpra-4.4.4/tests/unittests/unit/dbus/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/dbus/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2393 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/dbus/dbus_helper_test.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.541879 xpra-4.4.4/tests/unittests/unit/gtk_common/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/gtk_common/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      651 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/gtk_common/keymap_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      695 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/keyboard_layout_test.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.542879 xpra-4.4.4/tests/unittests/unit/net/
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1011 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/net/HMAC_test.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/net/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    39961 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/net/bencode_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4119 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/net/brotli_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2463 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/net/common_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4123 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/net/compression_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4036 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/net/crypto_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1095 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/net/d3des_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1759 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/net/digest_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1670 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/net/file_transfer_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4048 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/net/lz4_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2633 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/net/net_util_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1361 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/net/packet_encoding_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1948 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/net/packet_header_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    10107 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/net/protocol_test.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.542879 xpra-4.4.4/tests/unittests/unit/net/rfb/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/net/rfb/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1690 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/net/rfb/rfb_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      688 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/net/ssh_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     5944 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/net/subprocess_wrapper_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1784 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/net/websocket_header_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1463 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/net/websocket_response_headers_test.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.542879 xpra-4.4.4/tests/unittests/unit/notifications/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/notifications/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1538 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/notifications/common_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3493 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/os_util_test.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.543879 xpra-4.4.4/tests/unittests/unit/platformtests/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/platformtests/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1621 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/platformtests/displayfd_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      584 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/platformtests/features_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      663 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/platformtests/info_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1039 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/platformtests/init_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2349 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/platformtests/mainmodule_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    12682 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/process_test_util.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3415 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/queue_scheduler_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3519 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/rectangle_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3309 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/run.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.543879 xpra-4.4.4/tests/unittests/unit/scripts/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/scripts/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     7902 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/scripts/main_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4309 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/scripts/parse_display_name_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2675 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/scripts/parsing_test.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.544879 xpra-4.4.4/tests/unittests/unit/server/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    17214 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/auth_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1787 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/background_worker_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4981 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/cystats_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2426 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/dbus_test.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.547879 xpra-4.4.4/tests/unittests/unit/server/mixins/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/mixins/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2372 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/mixins/audio_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3616 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/mixins/child_command_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1189 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/mixins/clipboard_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1488 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/mixins/display_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1461 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/mixins/encoding_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1399 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/mixins/fileprint_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      820 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/mixins/input_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1867 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/mixins/logging_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      977 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/mixins/mmap_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3215 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/mixins/networkstate_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1966 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/mixins/notification_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1047 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/mixins/remotelogging_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     7380 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/mixins/server_mixins_option_test_util.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3698 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/mixins/servermixintest_util.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      535 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/mixins/shadow_option_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      761 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/mixins/start_option_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      614 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/mixins/startdesktop_option_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1700 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/mixins/stub_mixin_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4526 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/mixins/webcam_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      924 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/mixins/window_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    12214 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/motion_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1406 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/proxy_server_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3559 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/server_auth_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     9798 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/server_sockets_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4025 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/shadow_server_test.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.547879 xpra-4.4.4/tests/unittests/unit/server/source/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/source/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    14583 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/source/source_mixins_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     6010 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/video_scoring_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     5206 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/video_subregion_test.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.547879 xpra-4.4.4/tests/unittests/unit/server/window/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/window/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2034 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server/window/batch_config_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     6794 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/server_test_util.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1045 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/simple_stats_test.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.547879 xpra-4.4.4/tests/unittests/unit/sound/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/sound/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1089 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/sound/common_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1374 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/test_util.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     5839 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/util_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1322 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/version_util_test.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.548879 xpra-4.4.4/tests/unittests/unit/x11/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/x11/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1123 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/x11/common_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1366 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/x11/display_util_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1687 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/x11/fakexinerama_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2320 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/x11/keyboard_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2228 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/x11/size_hints_util_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     7967 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/x11/x11_server_test.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3097 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/unittests/unit/x11/xsettings_test.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.548879 xpra-4.4.4/tests/xpra/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      113 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/__init__.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.548879 xpra-4.4.4/tests/xpra/clients/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      113 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/clients/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4455 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/clients/fake_client.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1199 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/clients/fake_gtk_client.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1342 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/clients/test_DoS_client.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.549879 xpra-4.4.4/tests/xpra/codecs/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/codecs/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3621 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/codecs/benchmark.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1130 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/codecs/benchmark_bgra_to_rgb.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1119 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/codecs/benchmark_bgra_to_rgba.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1101 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/codecs/benchmark_bgrx_to_rgb.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3115 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/codecs/benchmark_picture_encoders.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1716 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/codecs/evdi_glib.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      913 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/codecs/evdi_test.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.549879 xpra-4.4.4/tests/xpra/keyboard/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      113 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/keyboard/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      578 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/keyboard/test_get_keycode_mappings.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      535 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/keyboard/test_x11keycodes_down.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.549879 xpra-4.4.4/tests/xpra/net/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      113 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/net/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      744 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/net/vsock_client_test.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1224 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/net/vsock_server_test.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.550879 xpra-4.4.4/tests/xpra/server/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/server/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      402 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/server/test_open_display.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    19078 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/server/test_region.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.553879 xpra-4.4.4/tests/xpra/test_apps/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      113 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1017 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/dbus_video_region_detection.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1009 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/dbus_video_region_enabled.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1199 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/dump_xshape.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1913 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/fps.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1041 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/screensaver_listener.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1141 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/send_dbus_video_exclusion_zone.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1198 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/simulate_console_typing.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1098 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/simulate_console_user.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      765 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_command_change.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      595 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_copy_image_from_clipboard.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      843 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_copy_image_to_clipboard.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1477 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_cursor_pixbuf.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1958 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_custom_cursor.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      627 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_drop_down.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      856 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_fast_cursor.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      613 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_form_input.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1381 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_frame_extents.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2073 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_gtk3_window.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      662 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_hostname.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      649 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_modal_window.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1064 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_notification.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1070 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_right_click_menu.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1418 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_show_desktop.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3316 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_system_tray.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      865 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_window_bypass_compositor.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      962 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_window_content_type.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1195 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_window_eclipse_fixed_size.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1001 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_window_icon_from_files.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      407 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_window_iconify.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      863 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_window_initial_position.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2509 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_window_maximize.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      545 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_window_maxsize_GTK3.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      900 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_window_move.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2486 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_window_moveresize.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1400 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_window_quality_speed_hints.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1269 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_window_raise.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1865 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_window_resize.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      589 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_window_title_fixed.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      525 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_window_withicon.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1274 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_window_xterm_size_hints.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      903 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_windows_at.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      800 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/test_apps/test_wmclass_change.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.553879 xpra-4.4.4/tests/xpra/x11/
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      682 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/x11/print_atom.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      571 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/x11/print_xpra_props.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1023 2023-03-10 09:32:07.000000 xpra-4.4.4/tests/xpra/x11/xres_get_pid.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.555879 xpra-4.4.4/xpra/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      294 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/__init__.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.556879 xpra-4.4.4/xpra/buffers/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/buffers/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2565 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/buffers/cyxor.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1304 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/buffers/memalign.c
--rw-r--r--   0 antoine   (1000) antoine   (1000)      447 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/buffers/memalign.h
--rw-r--r--   0 antoine   (1000) antoine   (1000)      713 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/buffers/membuf.pxd
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4524 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/buffers/membuf.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)      384 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/buffers/xxh.pxd
--rw-r--r--   0 antoine   (1000) antoine   (1000)      756 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/buffers/xxh.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2394 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/buffers/xxh3.h
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1855 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/buffers/xxhash.c
--rw-r--r--   0 antoine   (1000) antoine   (1000)   228839 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/buffers/xxhash.h
--rw-r--r--   0 antoine   (1000) antoine   (1000)      706 2023-03-10 09:32:39.000000 xpra-4.4.4/xpra/build_info.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     8601 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/child_reaper.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.558879 xpra-4.4.4/xpra/client/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/__init__.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.558879 xpra-4.4.4/xpra/client/auth/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/auth/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      581 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/auth/env_handler.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1137 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/auth/file_handler.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2363 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/auth/gss_handler.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2597 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/auth/kerberos_handler.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      703 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/auth/prompt_handler.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3118 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/auth/u2f_handler.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      502 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/auth/uri_handler.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    49200 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/client_base.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9184 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/client_tray.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3363 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/client_widget_base.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    39668 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/client_window_base.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1342 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/fake_window_backing.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.559879 xpra-4.4.4/xpra/client/gl/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      219 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gl/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    19450 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gl/gl_check.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4642 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gl/gl_colorspace_conversions.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1690 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gl/gl_drivers.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1048 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gl/gl_spinner.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    62226 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gl/gl_window_backing_base.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.559879 xpra-4.4.4/xpra/client/gl/gtk3/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gl/gtk3/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4616 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gl/gtk3/gl_client_window.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3719 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gl/gtk3/gl_drawing_area.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1091 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gl/gtk3/nativegl_client_window.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     8848 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gl/window_backend.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    29419 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gobject_client_base.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.560879 xpra-4.4.4/xpra/client/gtk3/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      666 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk3/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4426 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk3/cairo_backing.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    10117 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk3/cairo_workaround.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2537 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk3/client.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      727 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk3/client_window.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     8409 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk3/gtk3_client_window.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1128 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk3/gtk3_notifier.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5743 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk3/qrcode_client.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5202 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk3/show_shortcuts.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    10165 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk3/splash_screen.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      354 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk3/tray_menu.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5013 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk3/window_menu.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.563879 xpra-4.4.4/xpra/client/gtk_base/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      330 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    15434 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/bug_report.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    12662 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/cairo_backing_base.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    49713 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/client_launcher.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3720 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/confirm_dialog.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2177 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/css_overrides.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.565879 xpra-4.4.4/xpra/client/gtk_base/example/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/example/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1678 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/example/bell.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3091 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/example/clicks.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3891 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/example/colors.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     5267 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/example/colors_gradient.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2810 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/example/colors_plain.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2114 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/example/cursors.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      954 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/example/file_chooser.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     5699 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/example/fontrendering.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4820 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/example/grabs.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2182 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/example/header_bar.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4505 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/example/initiate_moveresize.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1799 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/example/text_entry.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3594 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/example/transparent_colors.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2649 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/example/transparent_window.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     6651 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/example/tray.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3880 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/example/window_focus.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     6293 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/example/window_geometry_hints.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1624 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/example/window_opacity.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1571 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/example/window_overrideredirect.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     5039 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/example/window_states.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1672 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/example/window_title.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2823 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/example/window_transient.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    66985 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/gtk_client_base.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)   103805 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/gtk_client_window_base.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3708 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/gtk_keyboard_helper.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1674 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/gtk_spinner.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    73876 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/gtk_tray_menu_base.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3888 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/mdns_gui.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    18598 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/menu_helper.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    13551 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/open_requests.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4301 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/pass_dialog.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     9619 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/server_commands.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    62843 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/session_info.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    19605 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/sessions_gui.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     7046 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/start_new_command.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     7025 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/statusicon_tray.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     7293 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/toolbox.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4477 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/u2f_tool.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4974 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/update_status.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    10506 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/gtk_base/window_info.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    14668 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/keyboard_helper.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     6625 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/keyboard_shortcuts_parser.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      537 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/mixin_features.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.566879 xpra-4.4.4/xpra/client/mixins/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/mixins/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    27030 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/mixins/audio.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    15243 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/mixins/clipboard.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    26996 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/mixins/display.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    14129 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/mixins/encodings.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     8264 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/mixins/fileprint_mixin.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5839 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/mixins/mmap.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    10291 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/mixins/network_listener.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    14835 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/mixins/network_state.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     7384 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/mixins/notifications.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     6295 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/mixins/remote_logging.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4305 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/mixins/rpc.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4533 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/mixins/serverinfo_mixin.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3238 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/mixins/stub_client_mixin.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5248 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/mixins/tray.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    13862 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/mixins/webcam.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    69521 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/mixins/window_manager.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2504 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/paint_colors.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    11888 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/rfb_protocol.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5729 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/scaling_parser.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      765 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/spinner.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    30722 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/top_client.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5210 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/tray_base.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    35134 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/ui_client_base.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    38810 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/window_backing_base.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      965 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/client/window_border.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.567879 xpra-4.4.4/xpra/clipboard/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/clipboard/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    31444 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/clipboard/clipboard_core.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5896 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/clipboard/clipboard_timeout_helper.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.567879 xpra-4.4.4/xpra/codecs/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/__init__.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.568879 xpra-4.4.4/xpra/codecs/argb/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      272 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/argb/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      579 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/argb/argb.pxd
--rw-r--r--   0 antoine   (1000) antoine   (1000)    29601 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/argb/argb.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4822 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/argb/encoder.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      810 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/argb/scale.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.568879 xpra-4.4.4/xpra/codecs/avif/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/avif/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    20278 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/avif/avif.pxd
--rw-r--r--   0 antoine   (1000) antoine   (1000)     8417 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/avif/decoder.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)     7391 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/avif/encoder.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)    26106 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/codec_checks.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     7001 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/codec_constants.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      710 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/codec_debug.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.568879 xpra-4.4.4/xpra/codecs/csc_cython/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      219 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/csc_cython/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    39950 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/csc_cython/colorspace_converter.pyx
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.569879 xpra-4.4.4/xpra/codecs/csc_libyuv/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      219 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/csc_libyuv/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    20006 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/csc_libyuv/colorspace_converter.pyx
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.569879 xpra-4.4.4/xpra/codecs/csc_swscale/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      219 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/csc_swscale/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    24047 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/csc_swscale/colorspace_converter.pyx
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.569879 xpra-4.4.4/xpra/codecs/cuda_common/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/cuda_common/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    22747 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/cuda_common/cuda_context.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.569879 xpra-4.4.4/xpra/codecs/dec_avcodec2/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      219 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/dec_avcodec2/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    38227 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/dec_avcodec2/decoder.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)      468 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/dec_avcodec2/register_compat.c
--rw-r--r--   0 antoine   (1000) antoine   (1000)      243 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/dec_avcodec2/register_compat.h
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.569879 xpra-4.4.4/xpra/codecs/drm/
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3441 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/drm/drm.pyx
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.569879 xpra-4.4.4/xpra/codecs/enc_ffmpeg/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/enc_ffmpeg/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    74079 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/enc_ffmpeg/encoder.pyx
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.570879 xpra-4.4.4/xpra/codecs/enc_proxy/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/enc_proxy/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4469 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/enc_proxy/encoder.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.570879 xpra-4.4.4/xpra/codecs/enc_x264/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      219 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/enc_x264/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    42251 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/enc_x264/encoder.pyx
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.570879 xpra-4.4.4/xpra/codecs/enc_x265/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/enc_x265/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    25341 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/enc_x265/encoder.pyx
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.570879 xpra-4.4.4/xpra/codecs/evdi/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/evdi/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    19890 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/evdi/capture.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1058 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/evdi/evdi_compat.h
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1626 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/evdi/load.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4754 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/icon_util.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     7832 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/image_wrapper.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.571879 xpra-4.4.4/xpra/codecs/jpeg/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/jpeg/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    13828 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/jpeg/decoder.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)    16913 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/jpeg/encoder.pyx
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.571879 xpra-4.4.4/xpra/codecs/libav_common/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/libav_common/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      326 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/libav_common/av_log.pxd
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4337 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/libav_common/av_log.pyx
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    17150 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/loader.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    15649 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/nv_util.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.571879 xpra-4.4.4/xpra/codecs/nvenc/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/nvenc/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)   184280 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/nvenc/encoder.pyx
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.572879 xpra-4.4.4/xpra/codecs/nvfbc/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/nvfbc/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2860 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/nvfbc/capture.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2992 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/nvfbc/cuda_image_wrapper.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    39225 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/nvfbc/fbc_capture_linux.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)    44173 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/nvfbc/fbc_capture_win.pyx
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.572879 xpra-4.4.4/xpra/codecs/nvjpeg/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/nvjpeg/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4116 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/nvjpeg/common.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)    11273 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/nvjpeg/decoder.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)    22564 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/nvjpeg/encoder.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5278 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/nvjpeg/nvjpeg.pxd
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.572879 xpra-4.4.4/xpra/codecs/pillow/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      982 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/pillow/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     7083 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/pillow/decoder.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    10966 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/pillow/encoder.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3780 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/rgb_transform.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.573879 xpra-4.4.4/xpra/codecs/spng/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/spng/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4660 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/spng/decoder.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)     8253 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/spng/encoder.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2750 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/spng/spng.pxd
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.573879 xpra-4.4.4/xpra/codecs/v4l2/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/v4l2/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    19326 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/v4l2/pusher.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)      321 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/v4l2/video.h
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    19408 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/video_helper.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.573879 xpra-4.4.4/xpra/codecs/vpx/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      219 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/vpx/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    10724 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/vpx/decoder.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)    29312 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/vpx/encoder.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1732 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/vpx/vpx.pxd
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.573879 xpra-4.4.4/xpra/codecs/webp/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      218 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/webp/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    15610 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/webp/decoder.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)    34416 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/codecs/webp/encoder.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4681 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/colorstreamhandler.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3888 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/common.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.574879 xpra-4.4.4/xpra/dbus/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/dbus/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      900 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/dbus/common.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4232 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/dbus/helper.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     6747 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/dbus/notifications_forwarder.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2631 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/exit_codes.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.575879 xpra-4.4.4/xpra/gtk_common/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      369 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/gtk_common/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2745 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/gtk_common/about.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4028 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/gtk_common/auth_dialog.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      837 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/gtk_common/cursor_names.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5680 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/gtk_common/desktop_greeter.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     8113 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/gtk_common/error.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2720 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/gtk_common/gobject_compat.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1449 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/gtk_common/gobject_util.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     6114 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/gtk_common/graph.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     7651 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/gtk_common/gtk2_notifier-LICENSE.txt
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.576879 xpra-4.4.4/xpra/gtk_common/gtk3/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/gtk_common/gtk3/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2092 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/gtk_common/gtk3/gdk_atoms.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)      742 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/gtk_common/gtk3/gdk_bindings.pxd
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4398 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/gtk_common/gtk3/gdk_bindings.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5601 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/gtk_common/gtk_clipboard.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    14794 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/gtk_common/gtk_notifier.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    29404 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/gtk_common/gtk_util.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     9861 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/gtk_common/gtk_view_clipboard.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     6488 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/gtk_common/gtk_view_keyboard.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9498 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/gtk_common/gui.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2774 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/gtk_common/keymap.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    48405 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/gtk_common/start_gui.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.576879 xpra-4.4.4/xpra/keyboard/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/keyboard/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    28201 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/keyboard/layouts.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1654 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/keyboard/mask.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    18994 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/log.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      873 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/make_thread.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.579879 xpra-4.4.4/xpra/net/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      218 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/__init__.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.580879 xpra-4.4.4/xpra/net/bencode/
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1334 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/bencode/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3563 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/bencode/bencode.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5622 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/bencode/cython_bencode.pyx
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.580879 xpra-4.4.4/xpra/net/brotli/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/brotli/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3970 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/brotli/compressor.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5218 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/brotli/decompressor.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)    23619 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/bytestreams.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3227 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/common.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     7953 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/compression.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     8574 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/crypto.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    13099 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/d3des.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3814 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/digest.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1536 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/fake_jitter.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    43937 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/file_transfer.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1621 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/header.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    16757 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/http_handler.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5549 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/libproxy.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3852 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/lz4.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)      412 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/lz4_compat.h
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.580879 xpra-4.4.4/xpra/net/mdns/
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1647 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/mdns/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4845 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/mdns/avahi_listener.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    10322 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/mdns/avahi_publisher.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3626 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/mdns/zeroconf_listener.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     7874 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/mdns/zeroconf_publisher.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    14618 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/mmap_pipe.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    21708 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/net_util.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5122 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/packet_encoding.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    58692 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/protocol.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      986 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/protocol_classes.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5364 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/pycryptography_backend.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2210 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/qrcode.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2434 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/qrencode.pyx
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.581879 xpra-4.4.4/xpra/net/rencodeplus/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/rencodeplus/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    16719 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/rencodeplus/rencodeplus.pyx
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.581879 xpra-4.4.4/xpra/net/rfb/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/rfb/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     6743 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/rfb/rfb_const.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3996 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/rfb/rfb_encode.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    11666 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/rfb/rfb_protocol.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    53813 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/socket_util.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    50855 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/ssh.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2982 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/sshfp.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    17520 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/subprocess_wrapper.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9713 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/upnp.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5347 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/vsock.pyx
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.582879 xpra-4.4.4/xpra/net/websockets/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/websockets/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4301 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/websockets/common.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4961 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/websockets/handler.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2448 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/websockets/header.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.582879 xpra-4.4.4/xpra/net/websockets/headers/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/websockets/headers/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      917 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/websockets/headers/browser_cookie.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      609 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/websockets/headers/default.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      501 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/websockets/headers/env_cookie.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2727 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/websockets/mask.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5950 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/net/websockets/protocol.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.583879 xpra-4.4.4/xpra/notifications/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/notifications/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1920 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/notifications/common.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9328 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/notifications/dbus_notifier.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2791 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/notifications/notifier_base.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2121 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/notifications/pynotify_notifier.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    29649 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/os_util.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.585879 xpra-4.4.4/xpra/platform/
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3946 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      423 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/autostart.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.587879 xpra-4.4.4/xpra/platform/darwin/
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1700 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/darwin/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/darwin/dotxpra.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      569 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/darwin/features.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2002 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/darwin/gdk3_bindings.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)     7065 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/darwin/gl_context.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    31962 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/darwin/gui.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      495 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/darwin/info.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9820 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/darwin/keyboard.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4346 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/darwin/keyboard_config.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4341 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/darwin/netdev_query.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      434 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/darwin/nsevent_glue.h
--rw-r--r--   0 antoine   (1000) antoine   (1000)      554 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/darwin/nsevent_glue.m
--rw-r--r--   0 antoine   (1000) antoine   (1000)    12377 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/darwin/osx_clipboard.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    18449 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/darwin/osx_menu.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4108 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/darwin/osx_tray.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     7508 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/darwin/paths.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      362 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/darwin/printing.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    10074 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/darwin/shadow_server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      301 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/darwin/transparency_glue.h
--rw-r--r--   0 antoine   (1000) antoine   (1000)      434 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/darwin/transparency_glue.m
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3023 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/displayfd.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    10344 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/dotxpra.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      486 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/dotxpra_common.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2990 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/features.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1340 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/gl_context.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    11575 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/gui.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2495 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/info.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2693 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/keyboard.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3955 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/keyboard_base.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2098 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/menu_helper.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2716 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/netdev_query.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    12793 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/paths.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     6313 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/printing.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      397 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/proxy_server.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    20039 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/pycups_printing.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      400 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/shadow_server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     6376 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/ui_thread_watcher.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2901 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/webcam.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.592879 xpra-4.4.4/xpra/platform/win32/
--rw-r--r--   0 antoine   (1000) antoine   (1000)    15246 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    31372 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/clipboard.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    28672 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/common.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3104 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/comtypes_util.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    98698 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/constants.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    18295 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/create_process_lib.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    25114 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/desktoplogon_lib.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2490 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/directsound.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3150 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/dotxpra.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2251 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/dpi.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3642 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/dwm_color.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      992 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/features.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9457 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/gdi_screen_capture.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     8651 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/gl_context.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3466 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/glwin32.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    54632 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/gui.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3242 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/icon_util.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      806 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/info.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    13837 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/keyboard.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    17618 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/keyboard_config.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    24048 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/lsa_logon_lib.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4174 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/menu_helper.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.592879 xpra-4.4.4/xpra/platform/win32/namedpipes/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/namedpipes/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     7677 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/namedpipes/common.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9034 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/namedpipes/connection.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    12862 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/namedpipes/listener.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3843 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/netdev_query.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9530 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/paths.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     8001 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/pdfium.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    17904 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/printer_notify.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9118 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/printing.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1491 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/propsys.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5422 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/proxy_server.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.593879 xpra-4.4.4/xpra/platform/win32/scripts/
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      709 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/scripts/exec.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1175 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/scripts/execfile.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)       95 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/scripts/proxy.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1492 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/scripts/shadow_server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2811 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/setappid.cpp
--rw-r--r--   0 antoine   (1000) antoine   (1000)       94 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/setappid.h
--rw-r--r--   0 antoine   (1000) antoine   (1000)    25502 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/shadow_server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1834 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/webcam.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    20363 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/win32_NotifyIcon.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4821 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/win32_balloon.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     8423 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/win32_events.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3062 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/win32_notifier.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     7749 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/win32_printing.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4265 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/win32_tray.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3146 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/win32_webcam.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     6867 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/window_hooks.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    22692 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/wndproc_events.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     9257 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/win32/wtsapi.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.594879 xpra-4.4.4/xpra/platform/xposix/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      211 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/xposix/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     6410 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/xposix/appindicator_tray.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1546 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/xposix/autostart.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/xposix/dotxpra.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1807 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/xposix/features.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     8172 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/xposix/gl_context.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    41287 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/xposix/gui.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      219 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/xposix/info.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     8630 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/xposix/keyboard.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    19414 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/xposix/menu_helper.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9307 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/xposix/netdev_query.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5665 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/xposix/paths.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      276 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/xposix/printing.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1376 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/xposix/proc.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3053 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/xposix/sd_listen.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)      325 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/xposix/shadow_server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     6796 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/platform/xposix/webcam.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4027 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/queue_scheduler.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     7872 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/rectangle.pyx
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.596879 xpra-4.4.4/xpra/scripts/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      211 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/scripts/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1324 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/scripts/bug_report.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    65162 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/scripts/config.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4179 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/scripts/fdproxy.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1150 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/scripts/gtk_info.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)   151690 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/scripts/main.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)   100996 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/scripts/parsing.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     9536 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/scripts/pinentry_wrapper.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    63443 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/scripts/server.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2097 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/scripts/show_webcam.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1109 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/scripts/version.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2031 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/scripts/win32_service.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.597879 xpra-4.4.4/xpra/server/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      307 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/__init__.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.600879 xpra-4.4.4/xpra/server/auth/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      236 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      529 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/allow_auth.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2089 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/auth_helper.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1168 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/capability_auth.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      644 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/env_auth.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3476 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/exec_auth.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      310 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/fail_auth.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1737 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/file_auth.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3527 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/file_auth_base.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3164 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/gss_auth.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3405 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/hosts_auth.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3372 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/kerberos_password_auth.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3838 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/kerberos_token_auth.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     7885 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/keycloak_auth.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     5616 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/ldap3_auth.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     6647 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/ldap_auth.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4539 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/multifile_auth.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2620 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/mysql_auth.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      740 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/none_auth.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3512 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/otp_auth.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2430 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/pam_auth.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      607 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/password_auth.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4323 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/peercred_auth.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1146 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/reject_auth.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1914 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/sql_auth.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     7108 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/sqlauthbase.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3416 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/sqlite_auth.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9636 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/sys_auth_base.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     5811 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/u2f_auth.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3130 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/auth/win32_auth.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3475 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/background_worker.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     6031 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/control_command.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     7443 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/cystats.pyx
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.601879 xpra-4.4.4/xpra/server/dbus/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/dbus/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1010 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/dbus/dbus_common.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    14093 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/dbus/dbus_server.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2793 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/dbus/dbus_server_base.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     6122 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/dbus/dbus_source.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2599 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/dbus/dbus_start.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    13985 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/gtk_server_base.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2627 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/keyboard_config_base.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     8564 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/menu_provider.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.603879 xpra-4.4.4/xpra/server/mixins/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/mixins/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    18552 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/mixins/audio_server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    17620 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/mixins/child_command_server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    10467 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/mixins/clipboard_server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3287 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/mixins/dbusrpc_server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    14947 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/mixins/display_manager.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    10349 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/mixins/encoding_server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    14384 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/mixins/fileprint_server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    18261 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/mixins/input_server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     7797 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/mixins/logging_server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1094 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/mixins/mmap_server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     7569 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/mixins/networkstate_server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     8599 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/mixins/notification_forwarder.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    38802 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/mixins/server_base_controlcommands.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      949 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/mixins/shell_server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4094 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/mixins/stub_server_mixin.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5048 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/mixins/webcam_server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    16274 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/mixins/window_server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    11210 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/pam.pyx
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.603879 xpra-4.4.4/xpra/server/proxy/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/proxy/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1282 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/proxy/proxy_dbus_server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    37464 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/proxy/proxy_instance.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    14672 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/proxy/proxy_instance_process.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2618 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/proxy/proxy_instance_thread.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    31865 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/proxy/proxy_server.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.603879 xpra-4.4.4/xpra/server/rfb/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/rfb/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4886 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/rfb/rfb_protocol.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     8509 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/rfb/rfb_server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5622 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/rfb/rfb_source.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    40869 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/server_base.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)   104945 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/server_core.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      653 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/server_features.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    18820 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/server_util.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      947 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/server_uuid.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.604879 xpra-4.4.4/xpra/server/shadow/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/shadow/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2690 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/shadow/gtk_root_window_model.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    19050 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/shadow/gtk_shadow_server_base.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     6640 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/shadow/root_window_model.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)      643 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/shadow/shadow_dbus_server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    18655 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/shadow/shadow_server_base.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.606879 xpra-4.4.4/xpra/server/source/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/source/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    24062 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/source/audio_mixin.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3989 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/source/avsync_mixin.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    17154 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/source/client_connection.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     6888 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/source/client_connection_factory.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     6746 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/source/clientdisplay_mixin.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     6585 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/source/clientinfo_mixin.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     6445 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/source/clipboard_connection.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1478 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/source/dbus_mixin.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    24538 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/source/encodings_mixin.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     7417 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/source/fileprint_mixin.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4907 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/source/idle_mixin.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5386 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/source/input_mixin.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     6187 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/source/mmap_connection.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4708 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/source/networkstate_mixin.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3279 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/source/notification_mixin.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2621 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/source/shell_mixin.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    16093 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/source/source_stats.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2225 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/source/stub_source_mixin.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9442 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/source/webcam_mixin.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    28287 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/source/windows_mixin.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    22977 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/ssh.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.607879 xpra-4.4.4/xpra/server/window/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/window/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5789 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/window/batch_config.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    16186 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/window/batch_delay_calculator.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    10846 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/window/content_guesser.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2688 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/window/filters.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5835 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/window/metadata.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    14048 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/window/motion.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9986 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/window/video_scoring.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    25816 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/window/video_subregion.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)   128230 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/window/window_source.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    14756 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/window/window_stats.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)   117437 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/window/window_video_source.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    11608 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/server/window/windowicon_source.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4934 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/simple_stats.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.608879 xpra-4.4.4/xpra/sound/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      241 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/sound/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1909 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/sound/common.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    36453 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/sound/gstreamer_util.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.608879 xpra-4.4.4/xpra/sound/pulseaudio/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      241 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/sound/pulseaudio/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2420 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/sound/pulseaudio/pulseaudio_common_util.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1003 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/sound/pulseaudio/pulseaudio_none_util.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     7730 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/sound/pulseaudio/pulseaudio_pactl_util.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2733 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/sound/pulseaudio/pulseaudio_util.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    21065 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/sound/sink.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    17106 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/sound/sound_pipeline.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    18118 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/sound/src.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    16585 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/sound/wrapper.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)       70 2023-03-10 09:32:39.000000 xpra-4.4.4/xpra/src_info.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    32992 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/util.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    10548 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/version_util.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.610879 xpra-4.4.4/xpra/x11/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      368 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/__init__.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.612879 xpra-4.4.4/xpra/x11/bindings/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      277 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/bindings/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      437 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/bindings/core_bindings.pxd
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4423 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/bindings/core_bindings.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)      363 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/bindings/display_source.pxd
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1117 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/bindings/display_source.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)    45040 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/bindings/keyboard_bindings.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2457 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/bindings/posix_display_source.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)    51994 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/bindings/randr_bindings.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)      642 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/bindings/randr_info.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3548 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/bindings/res_bindings.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1083 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/bindings/wait_for_x_server.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)    50094 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/bindings/window_bindings.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)    26109 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/bindings/xi2_bindings.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)    32988 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/bindings/ximage.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)    17304 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/bindings/xlib.pxd
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2240 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/bindings/xwait.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)      871 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/common.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.612879 xpra-4.4.4/xpra/x11/dbus/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/dbus/__init__.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1061 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/dbus/x11_dbus_server.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.612879 xpra-4.4.4/xpra/x11/desktop/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/desktop/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     6090 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/desktop/desktop_model.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5667 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/desktop/desktop_server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    13827 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/desktop/desktop_server_base.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     6084 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/desktop/model_base.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3771 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/desktop/monitor_model.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    14785 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/desktop/monitor_server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5312 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/expand_server.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)     5373 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/fakeXinerama.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.613879 xpra-4.4.4/xpra/x11/gtk3/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      326 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/gtk3/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    43991 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/gtk3/gdk_bindings.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2266 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/gtk3/gdk_display_source.pyx
--rw-r--r--   0 antoine   (1000) antoine   (1000)      827 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/gtk3/gdk_display_util.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      380 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/gtk3/gdk_x11_macros.c
--rw-r--r--   0 antoine   (1000) antoine   (1000)      253 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/gtk3/gdk_x11_macros.h
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.614879 xpra-4.4.4/xpra/x11/gtk_x11/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      590 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/gtk_x11/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    31650 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/gtk_x11/clipboard.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5316 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/gtk_x11/composite.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1925 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/gtk_x11/gdk_bindings.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)      533 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/gtk_x11/gdk_display_source.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1903 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/gtk_x11/keys.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5890 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/gtk_x11/prop.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     7195 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/gtk_x11/selection.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2506 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/gtk_x11/send_wm.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    11570 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/gtk_x11/tray.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     8052 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/gtk_x11/window_damage.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    20258 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/gtk_x11/wm.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     4626 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/gtk_x11/wm_check.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     9893 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/gtk_x11/world_window.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.615879 xpra-4.4.4/xpra/x11/models/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/models/__init__.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    30898 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/models/base.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    35552 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/models/core.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5204 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/models/model_stub.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1815 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/models/or_window.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     3474 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/models/size_hints_util.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1940 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/models/systray.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    40553 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/models/window.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    11750 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/prop_conv.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    62819 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    35500 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/server_keyboard_config.py
--rwxr-xr-x   0 antoine   (1000) antoine   (1000)    18278 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/shadow_x11_server.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5916 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/uinput_device.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    20404 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/vfb_util.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1151 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/window_info.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    19651 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/x11_server_base.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    46670 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/x11_server_core.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     2956 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/x11_window_filters.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)    35516 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/xkbhelper.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     1828 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/xroot_props.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     5370 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/xsettings.py
--rw-r--r--   0 antoine   (1000) antoine   (1000)     8187 2023-03-10 09:32:07.000000 xpra-4.4.4/xpra/x11/xsettings_prop.py
-drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-03-10 09:32:39.555879 xpra-4.4.4/xpra.egg-info/
--rw-r--r--   0 antoine   (1000) antoine   (1000)      440 2023-03-10 09:32:39.000000 xpra-4.4.4/xpra.egg-info/PKG-INFO
--rw-r--r--   0 antoine   (1000) antoine   (1000)    45302 2023-03-10 09:32:39.000000 xpra-4.4.4/xpra.egg-info/SOURCES.txt
--rw-r--r--   0 antoine   (1000) antoine   (1000)        1 2023-03-10 09:32:39.000000 xpra-4.4.4/xpra.egg-info/dependency_links.txt
--rw-r--r--   0 antoine   (1000) antoine   (1000)        5 2023-03-10 09:32:39.000000 xpra-4.4.4/xpra.egg-info/top_level.txt
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.344651 xpra-4.4.5/
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.218652 xpra-4.4.5/.github/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)       15 2023-02-24 14:18:37.000000 xpra-4.4.5/.github/FUNDING.yml
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.218652 xpra-4.4.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      623 2023-01-13 05:35:59.000000 xpra-4.4.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      604 2023-01-13 05:35:59.000000 xpra-4.4.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4183 2023-03-29 10:24:57.000000 xpra-4.4.5/.gitignore
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    17987 2023-05-23 12:16:20.000000 xpra-4.4.5/COPYING
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      918 2023-05-23 12:16:20.000000 xpra-4.4.5/MANIFEST.in
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      440 2023-05-23 12:16:26.344651 xpra-4.4.5/PKG-INFO
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4408 2023-05-23 12:16:20.000000 xpra-4.4.5/README.md
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.219652 xpra-4.4.5/docs/
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.219652 xpra-4.4.5/docs/Build/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3746 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Build/Debian.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     8384 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Build/Dependencies.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      997 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Build/MSWindows.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1642 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Build/MacOS.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4894 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Build/Other.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1016 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Build/README.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2431 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Build/RPM.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)   129367 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/CHANGELOG.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     7792 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/FAQ.md
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.220652 xpra-4.4.5/docs/Features/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3483 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Features/Audio.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     7617 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Features/Clipboard.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4604 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Features/DPI.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      363 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Features/Display.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1602 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Features/File-Transfers.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2023 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Features/Image-Depth.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2619 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Features/Keyboard.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1365 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Features/Notifications.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3818 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Features/Printing.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1293 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Features/README.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1385 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Features/System-Tray.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2479 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Features/Webcam.md
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.221652 xpra-4.4.5/docs/Network/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3177 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Network/AES.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      489 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Network/Encryption.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1057 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Network/Multicast-DNS.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3810 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Network/README.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4668 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Network/SSH.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5634 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Network/SSL.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2285 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/README.md
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.222652 xpra-4.4.5/docs/Usage/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1718 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Usage/Apache-Proxy.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    11800 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Usage/Authentication.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3833 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Usage/Client-OpenGL.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2735 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Usage/Client.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1615 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Usage/Configuration.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     7359 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Usage/Encodings.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     6558 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Usage/Logging.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4082 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Usage/NVENC.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2476 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Usage/OpenGL.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     8928 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Usage/Proxy-Server.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4628 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Usage/README.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      954 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Usage/Seamless.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    17482 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Usage/Security.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1211 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Usage/Service.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3429 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Usage/Shadow-Server.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1942 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Usage/Start-Desktop.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3721 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Usage/WSL.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     6536 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/Usage/Xdummy.md
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.223652 xpra-4.4.5/docs/images/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    29145 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/Xpra-Proxy.png
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.225652 xpra-4.4.5/docs/images/icons/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3531 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/icons/X11.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2083 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/icons/authentication.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1441 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/icons/clipboard.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1664 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/icons/connect.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      496 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/icons/debian.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2971 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/icons/encoding.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3857 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/icons/freebsd.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3090 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/icons/keyboard.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1506 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/icons/mdns.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3757 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/icons/nvidia.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2711 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/icons/opengl.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3555 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/icons/osx.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1932 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/icons/package.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3317 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/icons/printer.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1816 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/icons/rpm.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1326 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/icons/server-connected.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5009 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/icons/sound.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4227 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/icons/ssh.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     7147 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/icons/ubuntu.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2617 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/icons/upload.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2581 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/icons/webcam.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3944 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/icons/windows.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    37557 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/mdns-gui.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    29526 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/pavucontrol-client.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    31507 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/pavucontrol-server.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    45427 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/session-info-graphs.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    39729 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/session-info-sound.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3934 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/upload.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    10673 2023-05-23 12:16:20.000000 xpra-4.4.5/docs/images/win32-shadow-tray-menu.png
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.225652 xpra-4.4.5/fs/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      598 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/README.md
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.226652 xpra-4.4.5/fs/bin/
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    13395 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/bin/add_build_info.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      152 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/bin/links-to-html.lua
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4026 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/bin/run_scaled
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1848 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/bin/set_source_version
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2611 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/bin/xdummy_cvt_gen.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      187 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/bin/xpra
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2596 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/bin/xpra_Xdummy
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      272 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/bin/xpra_launcher
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.226652 xpra-4.4.5/fs/etc/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      864 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/README.md
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.211652 xpra-4.4.5/fs/etc/X11/
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.226652 xpra-4.4.5/fs/etc/X11/xorg.conf.d/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      226 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/X11/xorg.conf.d/90-xpra-virtual.conf
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.211652 xpra-4.4.5/fs/etc/dbus-1/
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.226652 xpra-4.4.5/fs/etc/dbus-1/system.d/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      499 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/dbus-1/system.d/xpra.conf
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.226652 xpra-4.4.5/fs/etc/default/
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      242 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/default/xpra
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.226652 xpra-4.4.5/fs/etc/init.d/
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2279 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/init.d/xpra
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.226652 xpra-4.4.5/fs/etc/pam.d/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      760 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/pam.d/xpra
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.227652 xpra-4.4.5/fs/etc/sysconfig/
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      242 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/sysconfig/xpra
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.227652 xpra-4.4.5/fs/etc/xpra/
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.229652 xpra-4.4.5/fs/etc/xpra/conf.d/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1115 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/conf.d/05_features.conf.in
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1883 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/conf.d/10_network.conf.in
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1678 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/conf.d/12_ssl.conf.in
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      501 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/conf.d/15_file_transfers.conf.in
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      769 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/conf.d/16_printing.conf.in
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      943 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/conf.d/20_sound.conf.in
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2270 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/conf.d/30_picture.conf.in
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      175 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/conf.d/35_webcam.conf.in
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1856 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/conf.d/40_client.conf.in
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      981 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/conf.d/42_client_keyboard.conf.in
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      232 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/conf.d/45_osx.conf.in
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2226 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/conf.d/50_server_network.conf.in
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1421 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/conf.d/55_server_x11.conf.in
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3249 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/conf.d/60_server.conf.in
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      379 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/conf.d/65_proxy.conf.in
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.229652 xpra-4.4.5/fs/etc/xpra/content-categories/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      644 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/content-categories/10_default.conf
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.229652 xpra-4.4.5/fs/etc/xpra/content-parent/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      147 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/content-parent/10_default.conf
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.229652 xpra-4.4.5/fs/etc/xpra/content-type/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      262 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/content-type/10_role.conf
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      735 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/content-type/30_title.conf
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4653 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/content-type/50_class.conf
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      158 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/content-type/70_commands.conf
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      674 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/cuda.conf
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.229652 xpra-4.4.5/fs/etc/xpra/http-headers/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      121 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/http-headers/00_nocache.txt
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      397 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/http-headers/10_content_security_policy.txt
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      137 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/nvenc.keys
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      214 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/nvfbc.keys
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2872 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/xorg-randr1.6.conf
+-rw-r--r--   0 antoine   (1000) antoine   (1000)   154106 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/xorg-uinput.conf
+-rw-r--r--   0 antoine   (1000) antoine   (1000)   154253 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/xorg.conf
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      734 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/etc/xpra/xpra.conf.in
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.229652 xpra-4.4.5/fs/lib/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1132 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/lib/README.md
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.211652 xpra-4.4.5/fs/lib/cups/
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.229652 xpra-4.4.5/fs/lib/cups/backend/
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     6922 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/lib/cups/backend/xpraforwarder
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.230652 xpra-4.4.5/fs/lib/pkgconfig/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      208 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/lib/pkgconfig/README.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      231 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/lib/pkgconfig/cuda.pc
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      220 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/lib/pkgconfig/nvenc.pc
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      218 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/lib/pkgconfig/nvfbc.pc
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      233 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/lib/pkgconfig/nvjpeg.pc
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.212652 xpra-4.4.5/fs/lib/systemd/
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.230652 xpra-4.4.5/fs/lib/systemd/system/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      751 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/lib/systemd/system/xpra-nosocketactivation.service
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      816 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/lib/systemd/system/xpra.service
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      300 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/lib/systemd/system/xpra.socket
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.230652 xpra-4.4.5/fs/lib/sysusers.d/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)       10 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/lib/sysusers.d/xpra.conf
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.231652 xpra-4.4.5/fs/lib/tmpfiles.d/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      174 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/lib/tmpfiles.d/xpra.conf
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.212652 xpra-4.4.5/fs/lib/udev/
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.231652 xpra-4.4.5/fs/lib/udev/rules.d/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      491 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/lib/udev/rules.d/71-xpra-virtual-pointer.rules
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.212652 xpra-4.4.5/fs/libexec/
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.231652 xpra-4.4.5/fs/libexec/xpra/
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)       94 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/libexec/xpra/auth_dialog
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3748 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/libexec/xpra/gnome-open
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3748 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/libexec/xpra/gvfs-open
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3748 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/libexec/xpra/xdg-open
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      674 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/libexec/xpra/xpra_signal_listener
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      397 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/libexec/xpra/xpra_udev_product_version
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.212652 xpra-4.4.5/fs/share/
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.232652 xpra-4.4.5/fs/share/applications/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      193 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/applications/xpra-gui.desktop
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      304 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/applications/xpra-launcher.desktop
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      270 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/applications/xpra-shadow.desktop
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      602 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/applications/xpra.desktop
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.233652 xpra-4.4.5/fs/share/icons/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1474 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/icons/xpra-mdns.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1326 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/icons/xpra-shadow.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)   434275 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/icons/xpra.icns
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3011 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/icons/xpra.png
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.212652 xpra-4.4.5/fs/share/man/
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.233652 xpra-4.4.5/fs/share/man/man1/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2061 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/man/man1/run_scaled.1
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    73349 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/man/man1/xpra.1
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2243 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/man/man1/xpra_launcher.1
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.233652 xpra-4.4.5/fs/share/metainfo/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1978 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/metainfo/xpra.appdata.xml
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.212652 xpra-4.4.5/fs/share/mime/
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.233652 xpra-4.4.5/fs/share/mime/packages/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      256 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/mime/packages/application-x-xpraconfig.xml
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.212652 xpra-4.4.5/fs/share/selinux/
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.234652 xpra-4.4.5/fs/share/selinux/cups_xpra/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      256 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/selinux/cups_xpra/README.TXT
+-rw-r--r--   0 antoine   (1000) antoine   (1000)       90 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/selinux/cups_xpra/cups_xpra.fc
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1282 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/selinux/cups_xpra/cups_xpra.te
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.234652 xpra-4.4.5/fs/share/selinux/xpra_socketactivation/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      343 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/selinux/xpra_socketactivation/README.TXT
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1393 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/selinux/xpra_socketactivation/xpra_socketactivation.fc
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5354 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/selinux/xpra_socketactivation/xpra_socketactivation.te
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.234652 xpra-4.4.5/fs/share/xpra/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      258 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/autostart.desktop
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    24648 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/bell.wav
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.234652 xpra-4.4.5/fs/share/xpra/css/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      493 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/css/10_header_bar.css
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      355 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/css/20_progress_bar.css
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.235652 xpra-4.4.5/fs/share/xpra/cuda/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1072 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/cuda/BGRA_to_RGBAP.cu
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2873 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/cuda/BGRX_to_NV12.cu
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1039 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/cuda/BGRX_to_RGB.cu
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1330 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/cuda/BGRX_to_YUV444.cu
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      281 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/cuda/README.md
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1072 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/cuda/RGBA_to_RGBAP.cu
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1039 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/cuda/RGBX_to_RGB.cu
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2882 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/cuda/XRGB_to_NV12.cu
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1332 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/cuda/XRGB_to_YUV444.cu
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.249652 xpra-4.4.5/fs/share/xpra/icons/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      659 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/audio.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/authentication.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2083 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/authentication.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4161 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/bandwidth_limit.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/bell.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1636 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/bell.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/browse.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3739 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/browse.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1136 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/browser.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9462 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/bugs.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2283 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/bugs.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/clipboard.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1441 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/clipboard.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3629 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/close.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2343 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/compressed.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1664 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/connect.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    16958 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/cuda.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/directory.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2407 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/disconnected.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    12774 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/display.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1170 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/documentation.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3887 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/download.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1304 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/empty.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/encoding.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2971 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/encoding.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5633 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/eye-off.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5385 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/eye-on.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/features.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2889 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/features.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1789 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/fluxbox.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/font.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1607 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/font.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4198 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/forward.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3857 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/freebsd.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/gears.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4332 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/gnome-session.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4332 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/gnome.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/gstreamer.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    25214 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/gtk.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/information.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2742 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/information.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4463 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/kde.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    67646 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/keyboard.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3090 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/keyboard.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/keymap.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3173 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/linux.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2305 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/list.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/loop.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3062 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/lxde.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3555 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/macos.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2284 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/matchbox.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3875 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/maximize.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/mdns.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1506 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/mdns.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/microphone.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3748 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/microphone.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      819 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/minimize.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/network.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      133 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/noicon.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/nvidia.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2331 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/open.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1760 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/openbox.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5242 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/openbsd.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/opengl.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2711 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/opengl.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1932 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/package.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1477 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/picture.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2018 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/pointer.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/printer.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3317 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/printer.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    16958 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/python.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1703 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/qr.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1013 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/quit.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3067 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/raise.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4907 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/reinitialize.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1618 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/retry.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1999 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/sawfish.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1272 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/scaling.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/screenshot.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1883 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/screenshot.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    19246 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/server-connected.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1326 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/server-connected.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    34494 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/server-notconnected.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1046 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/server-notconnected.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      527 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/server.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      874 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/shutdown.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1085 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/slider.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4384 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/speaker-off.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/speaker.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4583 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/speaker.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3337 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/speed.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/sql.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/sqlite.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1586 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/sqlite.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9318 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/start.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1851 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/statistics.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      794 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/ticked-small.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     8814 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/ticked.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1251 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/timer.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2060 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/toolbox.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1157 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/transfer.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/transparent.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      312 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/transparent.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      290 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/unticked-small.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     8711 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/unticked.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4905 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/update.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    14087 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/upload.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3480 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/user.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      902 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/video.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    16958 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/webcam.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2581 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/webcam.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3944 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/win32.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4304 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/windowmaker.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2146 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/windows.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9662 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/xpra.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2353 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/xpra.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3774 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/xpra_txt.ico
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1498 2023-05-23 12:16:20.000000 xpra-4.4.5/fs/share/xpra/icons/xterm.png
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.213652 xpra-4.4.5/packaging/
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.251652 xpra-4.4.5/packaging/MSWindows/
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      464 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MSWindows/ALL_RELEASE_BUILDS.sh
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      687 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MSWindows/BUILD_CUDA_KERNEL.BAT
+-rw-r--r--   0 antoine   (1000) antoine   (1000)   143740 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MSWindows/DirectShow.tlb
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    21443 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MSWindows/MINGW_BUILD.sh
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3376 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MSWindows/MINGW_SETUP.sh
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1202 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MSWindows/SIGN_ALL.sh
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     6832 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MSWindows/TaskbarLib.tlb
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MSWindows/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      446 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MSWindows/gen_win32con.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1029 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MSWindows/msi.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     8585 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MSWindows/msi.xml
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.251652 xpra-4.4.5/packaging/MSWindows/pkgconfig/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      233 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MSWindows/pkgconfig/cuda.pc
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      325 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MSWindows/pkgconfig/nvenc.pc
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      193 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MSWindows/pkgconfig/nvfbc.pc
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      251 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MSWindows/pkgconfig/nvjpeg.pc
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.251652 xpra-4.4.5/packaging/MSWindows/service/
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.252652 xpra-4.4.5/packaging/MSWindows/service/DesktopLogon/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3599 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MSWindows/service/DesktopLogon/DesktopLogon.cs
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     6066 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MSWindows/service/DesktopLogon/DesktopLogon.csproj
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1482 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MSWindows/service/DesktopLogon/DesktopLogon.sln
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    15694 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MSWindows/service/Xpra-Service.cpp
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      644 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MSWindows/service/event_log.mc
+-rw-r--r--   0 antoine   (1000) antoine   (1000)       41 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MSWindows/website.url
+-rw-r--r--   0 antoine   (1000) antoine   (1000)   154542 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MSWindows/xpra-logo.bmp
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9798 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MSWindows/xpra.bmp
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    13700 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MSWindows/xpra.iss
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.254652 xpra-4.4.5/packaging/MacOS/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)   494603 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Blank.dmg.bz2
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1422 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/C-wrapper.c
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    61482 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/GPL.rtf
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.258652 xpra-4.4.5/packaging/MacOS/Helpers/
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      292 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Auth_Dialog
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      280 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Browser
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      288 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Bug_Report
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      273 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Config_info
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      280 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Encoding_info
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      299 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Example-Colors
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      308 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Example-Colors-Gradient
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      305 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Example-Colors-Plain
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      311 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Example-OpenGL-Colors-Gradient
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      311 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Example-Transparent-Colors
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      311 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Example-Transparent-Window
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      276 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Feature_info
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      279 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/GStreamer_info
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      275 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/GTK_info
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      287 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Keyboard_Tool
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      276 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Keyboard_info
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      276 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Keymap_info
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      306 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Launcher
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      510 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Manual
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      271 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/NativeGUI_info
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      271 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Network_info
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      287 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/OpenGL_check
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      273 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Path_info
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      278 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/PowerMonitor
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      295 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Print
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      187 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Python
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3495 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/PythonExecWrapper
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      287 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/SQL_auth_tool
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      290 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/SQLite_auth_tool
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      560 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Shadow
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      283 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/U2F_Tool
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      274 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Version_info
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      289 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Webcam_Test
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      415 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Helpers/Xpra
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1452 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Info-template.plist
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2497 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Info.plist
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      291 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Inherit.entitlements
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1683 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Shell-wrapper.c
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3486 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Xpra.bundle
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      861 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Xpra.entitlements
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.213652 xpra-4.4.5/packaging/MacOS/Xpra_NoDock.app/
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.258652 xpra-4.4.5/packaging/MacOS/Xpra_NoDock.app/Contents/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1449 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/Xpra_NoDock.app/Contents/Info.plist
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     8989 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/background.png
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.258652 xpra-4.4.5/packaging/MacOS/dmg-icons/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    16374 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/dmg-icons/background.jpg
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    28638 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/dmg-icons/icon.png
+-rw-r--r--   0 antoine   (1000) antoine   (1000)       57 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/gtkrc
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2046 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/make-DMG.sh
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4209 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/make-PKG.sh
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      154 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/make-all.sh
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    15666 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/make-app.sh
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4608 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/make-appstore-PKG.sh
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      353 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/org.xpra.Agent.plist
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1734 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/postinstall
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      341 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/sign-app.sh
+-rw-r--r--   0 antoine   (1000) antoine   (1000)   434275 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/MacOS/xpra.icns
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.259652 xpra-4.4.5/packaging/debian/
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      217 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/build.sh
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.213652 xpra-4.4.5/packaging/debian/libcuda1/
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.259652 xpra-4.4.5/packaging/debian/libcuda1/DEBIAN/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      314 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/libcuda1/DEBIAN/control
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)       51 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/libcuda1.sh
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.213652 xpra-4.4.5/packaging/debian/libnvidia-fbc1/
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.259652 xpra-4.4.5/packaging/debian/libnvidia-fbc1/DEBIAN/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      325 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/libnvidia-fbc1/DEBIAN/control
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)       63 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/libnvidia-fbc1.sh
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.260652 xpra-4.4.5/packaging/debian/xpra/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      402 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xpra/README.Debian
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    96785 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xpra/changelog
+-rw-r--r--   0 antoine   (1000) antoine   (1000)        3 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xpra/compat
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5318 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xpra/control
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3557 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xpra/copyright
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.261652 xpra-4.4.5/packaging/debian/xpra/patches/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      785 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xpra/patches/pam.patch
+-rw-r--r--   0 antoine   (1000) antoine   (1000)       31 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xpra/patches/series
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      432 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xpra/patches/service-config.patch
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1246 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xpra/rules
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.261652 xpra-4.4.5/packaging/debian/xpra/source/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)       12 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xpra/source/format
+-rw-r--r--   0 antoine   (1000) antoine   (1000)       19 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xpra/source/options
+-rw-r--r--   0 antoine   (1000) antoine   (1000)       64 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xpra/watch
+-rw-r--r--   0 antoine   (1000) antoine   (1000)       10 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xpra/xpra.docs
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1008 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xpra/xpra.install
+-rw-r--r--   0 antoine   (1000) antoine   (1000)       57 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xpra/xpra.links
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      301 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xpra/xpra.lintian-overrides
+-rw-r--r--   0 antoine   (1000) antoine   (1000)       83 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xpra/xpra.manpages
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      544 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xpra/xpra.postinst
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      204 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xpra/xpra.postrm
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      824 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xpra/xpra.service
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      300 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xpra/xpra.socket
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2141 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xpra.sh
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.261652 xpra-4.4.5/packaging/debian/xserver-xorg-video-dummy/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      989 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xserver-xorg-video-dummy/changelog
+-rw-r--r--   0 antoine   (1000) antoine   (1000)        2 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xserver-xorg-video-dummy/compat
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      838 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xserver-xorg-video-dummy/control
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1420 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xserver-xorg-video-dummy/copyright
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.262652 xpra-4.4.5/packaging/debian/xserver-xorg-video-dummy/patches/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3180 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xserver-xorg-video-dummy/patches/0002-Constant-DPI.patch
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1776 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xserver-xorg-video-dummy/patches/0006-Dummy-Disconnect.patch
+-rw-r--r--   0 antoine   (1000) antoine   (1000)       51 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xserver-xorg-video-dummy/patches/series
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      271 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xserver-xorg-video-dummy/rules
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      661 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/debian/xserver-xorg-video-dummy.sh
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.264652 xpra-4.4.5/packaging/rpm/
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.265652 xpra-4.4.5/packaging/rpm/distros/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      224 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/distros/almalinux.list
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      187 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/distros/arm64.list
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      238 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/distros/centos-8.list
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      208 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/distros/centos-arm64.list
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      207 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/distros/centos-stream9.list
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      187 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/distros/default.list
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      202 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/distros/fedora-37.list
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      243 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/distros/oraclelinux.list
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      224 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/distros/rockylinux.list
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      370 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/fake-cuda.spec
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    11873 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/ffmpeg-xpra.spec
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1596 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/gstreamer1-plugin-timestamp.spec
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1777 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/libfakeXinerama.spec
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     8115 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/libyuv.spec
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1305 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/nasm.spec
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.266652 xpra-4.4.5/packaging/rpm/patches/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3180 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/patches/0002-Constant-DPI.patch
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1776 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/patches/0006-Dummy-Disconnect.patch
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      770 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/patches/libyuv-0001-Use-a-proper-so-version.patch
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1040 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/patches/libyuv-0002-Link-against-shared-library.patch
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1467 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/patches/libyuv-0003-Disable-static-library.patch
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1313 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/patches/libyuv-0004-Don-t-install-conversion-tool.patch
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      648 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/patches/libyuv-0005-Use-library-suffix-during-installation.patch
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      592 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/patches/libyuv-0006-Link-main-library-against-libjpeg.patch
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      513 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/patches/libyuv-0007-nojpeg.patch
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2451 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/patches/nasm-SourceSans-font-name.patch
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      319 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/patches/python-rencode-nowheelreq.patch
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    16815 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/patches/python-rencode-readdmissingpyx.patch
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      318 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/patches/python-rencode-rename.patch
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1123 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/patches/python-rencode-typecode-dos.patch
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1818 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/python3-Cython.spec
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    10668 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/python3-cairo.spec
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1687 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/python3-lz4.spec
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1641 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/python3-pbr.spec
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1362 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/python3-pkgconfig.spec
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5765 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/python3-pycuda.spec
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2740 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/python3-pynvml.spec
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5870 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/python3-pyopengl.spec
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3005 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/python3-pytools.spec
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2145 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/python3-pyu2f.spec
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4313 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/python3-rencode.spec
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3785 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/python3-uinput.spec
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2450 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/x264-xpra.spec
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3061 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/xorg-x11-drv-dummy.spec
+-rw-r--r--   0 antoine   (1000) antoine   (1000)   102543 2023-05-23 12:16:20.000000 xpra-4.4.5/packaging/rpm/xpra.spec
+-rw-r--r--   0 antoine   (1000) antoine   (1000)       38 2023-05-23 12:16:26.344651 xpra-4.4.5/setup.cfg
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)   106090 2023-05-23 12:16:20.000000 xpra-4.4.5/setup.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.266652 xpra-4.4.5/tests/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      112 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/__init__.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.267652 xpra-4.4.5/tests/perf/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    12710 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/perf/perf_config_default.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    47773 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/perf/test_measure_perf.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    15741 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/perf/test_measure_perf_chartreps.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    14540 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/perf/test_measure_perf_charts.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.267652 xpra-4.4.5/tests/scripts/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      113 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/scripts/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      258 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/scripts/cProfile
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    27771 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/scripts/pycallgraph
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.267652 xpra-4.4.5/tests/unittests/
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1478 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/run
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.268652 xpra-4.4.5/tests/unittests/unit/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/__init__.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.268652 xpra-4.4.5/tests/unittests/unit/buffers/
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2526 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/buffers/cyxor_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3360 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/child_reaper_test.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.269652 xpra-4.4.5/tests/unittests/unit/client/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      189 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3608 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/auth_handlers_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      874 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/border_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3198 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/keyboard_helper_test.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.270652 xpra-4.4.5/tests/unittests/unit/client/mixins/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/mixins/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     7331 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/mixins/audioclient_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3650 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/mixins/clientmixintest_util.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1105 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/mixins/clipboard_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1642 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/mixins/display_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2191 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/mixins/encodings_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1844 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/mixins/mmap_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1106 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/mixins/networkstate_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      737 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/mixins/notifications_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1645 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/mixins/remotelogging_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1436 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/mixins/serverinfo_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      961 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/mixins/stubclient_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      935 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/mixins/tray_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1121 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/mixins/webcam_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1239 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/mixins/window_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      933 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/osxlike_clipboard_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      665 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/paint_colors_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3174 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/splash_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     5341 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/x11_client_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1155 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/x11_client_test_util.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      931 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/x11_clipboard_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3739 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/client/x11_clipboard_test_util.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.271652 xpra-4.4.5/tests/unittests/unit/codecs/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/codecs/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2652 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/codecs/argb_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2438 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/codecs/codecs_selftest_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3594 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/codecs/csc_colorspace_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     5000 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/codecs/image_wrapper_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      826 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/codecs/nvutil_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4549 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/codecs/pillow_encoder_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2736 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/codecs/pillow_header_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2474 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/codecs/rgb_transform_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4716 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/codecs/video_colorspace_test.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.271652 xpra-4.4.5/tests/unittests/unit/dbus/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/dbus/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2393 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/dbus/dbus_helper_test.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.271652 xpra-4.4.5/tests/unittests/unit/gtk_common/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/gtk_common/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      651 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/gtk_common/keymap_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      695 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/keyboard_layout_test.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.273652 xpra-4.4.5/tests/unittests/unit/net/
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1011 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/net/HMAC_test.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/net/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    39961 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/net/bencode_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4119 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/net/brotli_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2463 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/net/common_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4123 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/net/compression_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4036 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/net/crypto_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1095 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/net/d3des_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1759 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/net/digest_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1670 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/net/file_transfer_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4048 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/net/lz4_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2633 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/net/net_util_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1361 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/net/packet_encoding_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1948 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/net/packet_header_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    10107 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/net/protocol_test.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.273652 xpra-4.4.5/tests/unittests/unit/net/rfb/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/net/rfb/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1690 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/net/rfb/rfb_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      688 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/net/ssh_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     5944 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/net/subprocess_wrapper_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1784 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/net/websocket_header_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1463 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/net/websocket_response_headers_test.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.273652 xpra-4.4.5/tests/unittests/unit/notifications/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/notifications/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1538 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/notifications/common_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3493 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/os_util_test.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.274652 xpra-4.4.5/tests/unittests/unit/platformtests/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/platformtests/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1621 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/platformtests/displayfd_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      584 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/platformtests/features_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      663 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/platformtests/info_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1039 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/platformtests/init_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2349 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/platformtests/mainmodule_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    12682 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/process_test_util.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3415 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/queue_scheduler_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3519 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/rectangle_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3309 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/run.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.274652 xpra-4.4.5/tests/unittests/unit/scripts/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/scripts/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     8123 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/scripts/main_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4309 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/scripts/parse_display_name_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2675 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/scripts/parsing_test.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.275652 xpra-4.4.5/tests/unittests/unit/server/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    17214 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/auth_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1787 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/background_worker_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4981 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/cystats_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2426 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/dbus_test.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.278652 xpra-4.4.5/tests/unittests/unit/server/mixins/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/mixins/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2372 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/mixins/audio_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3616 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/mixins/child_command_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1189 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/mixins/clipboard_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1488 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/mixins/display_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1461 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/mixins/encoding_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1399 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/mixins/fileprint_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      820 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/mixins/input_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1867 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/mixins/logging_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      977 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/mixins/mmap_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3215 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/mixins/networkstate_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1966 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/mixins/notification_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1047 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/mixins/remotelogging_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     7380 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/mixins/server_mixins_option_test_util.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3698 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/mixins/servermixintest_util.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      535 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/mixins/shadow_option_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      761 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/mixins/start_option_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      614 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/mixins/startdesktop_option_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1700 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/mixins/stub_mixin_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4526 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/mixins/webcam_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      924 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/mixins/window_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    12214 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/motion_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1406 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/proxy_server_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3559 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/server_auth_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     9798 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/server_sockets_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4025 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/shadow_server_test.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.278652 xpra-4.4.5/tests/unittests/unit/server/source/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/source/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    14583 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/source/source_mixins_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     6010 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/video_scoring_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     5206 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/video_subregion_test.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.278652 xpra-4.4.5/tests/unittests/unit/server/window/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/window/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2034 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server/window/batch_config_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     6794 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/server_test_util.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1045 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/simple_stats_test.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.278652 xpra-4.4.5/tests/unittests/unit/sound/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/sound/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1089 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/sound/common_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1374 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/test_util.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     5839 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/util_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1322 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/version_util_test.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.279651 xpra-4.4.5/tests/unittests/unit/x11/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/x11/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1123 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/x11/common_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1366 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/x11/display_util_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1687 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/x11/fakexinerama_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2320 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/x11/keyboard_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2228 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/x11/size_hints_util_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     7967 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/x11/x11_server_test.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3097 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/unittests/unit/x11/xsettings_test.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.279651 xpra-4.4.5/tests/xpra/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      113 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/__init__.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.279651 xpra-4.4.5/tests/xpra/clients/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      113 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/clients/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4455 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/clients/fake_client.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1199 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/clients/fake_gtk_client.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1342 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/clients/test_DoS_client.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.280652 xpra-4.4.5/tests/xpra/codecs/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/codecs/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3621 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/codecs/benchmark.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1130 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/codecs/benchmark_bgra_to_rgb.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1119 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/codecs/benchmark_bgra_to_rgba.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1101 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/codecs/benchmark_bgrx_to_rgb.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3115 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/codecs/benchmark_picture_encoders.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1716 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/codecs/evdi_glib.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      913 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/codecs/evdi_test.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.280652 xpra-4.4.5/tests/xpra/keyboard/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      113 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/keyboard/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      578 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/keyboard/test_get_keycode_mappings.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      535 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/keyboard/test_x11keycodes_down.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.280652 xpra-4.4.5/tests/xpra/net/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      113 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/net/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      744 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/net/vsock_client_test.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1224 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/net/vsock_server_test.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.281652 xpra-4.4.5/tests/xpra/server/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      107 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/server/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      402 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/server/test_open_display.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    19078 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/server/test_region.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.284652 xpra-4.4.5/tests/xpra/test_apps/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      113 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1017 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/dbus_video_region_detection.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1009 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/dbus_video_region_enabled.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1199 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/dump_xshape.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1913 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/fps.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1041 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/screensaver_listener.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1141 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/send_dbus_video_exclusion_zone.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1198 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/simulate_console_typing.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1098 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/simulate_console_user.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      765 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_command_change.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      595 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_copy_image_from_clipboard.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      843 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_copy_image_to_clipboard.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1477 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_cursor_pixbuf.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1958 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_custom_cursor.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      627 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_drop_down.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      856 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_fast_cursor.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      613 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_form_input.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1381 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_frame_extents.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2073 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_gtk3_window.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      662 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_hostname.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      649 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_modal_window.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1064 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_notification.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1070 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_right_click_menu.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1418 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_show_desktop.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3316 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_system_tray.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      865 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_window_bypass_compositor.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      962 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_window_content_type.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1195 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_window_eclipse_fixed_size.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1001 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_window_icon_from_files.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      407 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_window_iconify.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      863 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_window_initial_position.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2509 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_window_maximize.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      545 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_window_maxsize_GTK3.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      900 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_window_move.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2486 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_window_moveresize.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1400 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_window_quality_speed_hints.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1269 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_window_raise.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1865 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_window_resize.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      589 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_window_title_fixed.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      525 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_window_withicon.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1274 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_window_xterm_size_hints.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      903 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_windows_at.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      800 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/test_apps/test_wmclass_change.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.284652 xpra-4.4.5/tests/xpra/x11/
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      682 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/x11/print_atom.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      571 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/x11/print_xpra_props.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1023 2023-05-23 12:16:20.000000 xpra-4.4.5/tests/xpra/x11/xres_get_pid.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.286651 xpra-4.4.5/xpra/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      294 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/__init__.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.287651 xpra-4.4.5/xpra/buffers/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/buffers/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2565 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/buffers/cyxor.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1304 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/buffers/memalign.c
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      447 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/buffers/memalign.h
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      713 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/buffers/membuf.pxd
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4524 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/buffers/membuf.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      313 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/buffers/xxh.pxd
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      550 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/buffers/xxh.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2394 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/buffers/xxh3.h
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1855 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/buffers/xxhash.c
+-rw-r--r--   0 antoine   (1000) antoine   (1000)   228839 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/buffers/xxhash.h
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      727 2023-05-23 12:16:25.000000 xpra-4.4.5/xpra/build_info.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     8601 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/child_reaper.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.289651 xpra-4.4.5/xpra/client/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/__init__.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.290651 xpra-4.4.5/xpra/client/auth/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/auth/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      581 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/auth/env_handler.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1137 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/auth/file_handler.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2363 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/auth/gss_handler.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2597 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/auth/kerberos_handler.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      703 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/auth/prompt_handler.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3118 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/auth/u2f_handler.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      502 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/auth/uri_handler.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    49200 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/client_base.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9184 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/client_tray.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3363 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/client_widget_base.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    39668 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/client_window_base.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1342 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/fake_window_backing.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.290651 xpra-4.4.5/xpra/client/gl/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      219 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gl/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    19450 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gl/gl_check.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4642 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gl/gl_colorspace_conversions.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1690 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gl/gl_drivers.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1048 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gl/gl_spinner.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    62226 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gl/gl_window_backing_base.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.290651 xpra-4.4.5/xpra/client/gl/gtk3/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gl/gtk3/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4616 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gl/gtk3/gl_client_window.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3719 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gl/gtk3/gl_drawing_area.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1091 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gl/gtk3/nativegl_client_window.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     8848 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gl/window_backend.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    29419 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gobject_client_base.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.291652 xpra-4.4.5/xpra/client/gtk3/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      666 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk3/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4426 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk3/cairo_backing.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    10117 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk3/cairo_workaround.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2537 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk3/client.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      727 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk3/client_window.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     8409 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk3/gtk3_client_window.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1128 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk3/gtk3_notifier.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5743 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk3/qrcode_client.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5202 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk3/show_shortcuts.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    10165 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk3/splash_screen.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      354 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk3/tray_menu.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5013 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk3/window_menu.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.294651 xpra-4.4.5/xpra/client/gtk_base/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      330 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    15434 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/bug_report.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    12662 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/cairo_backing_base.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    49713 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/client_launcher.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3720 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/confirm_dialog.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2177 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/css_overrides.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.296651 xpra-4.4.5/xpra/client/gtk_base/example/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/example/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1678 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/example/bell.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3091 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/example/clicks.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3891 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/example/colors.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     5267 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/example/colors_gradient.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2810 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/example/colors_plain.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2114 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/example/cursors.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      954 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/example/file_chooser.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     5699 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/example/fontrendering.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4820 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/example/grabs.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2182 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/example/header_bar.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4505 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/example/initiate_moveresize.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1799 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/example/text_entry.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3594 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/example/transparent_colors.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2649 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/example/transparent_window.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     6651 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/example/tray.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3880 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/example/window_focus.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     6293 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/example/window_geometry_hints.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1624 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/example/window_opacity.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1571 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/example/window_overrideredirect.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     5039 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/example/window_states.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1672 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/example/window_title.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2823 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/example/window_transient.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    66985 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/gtk_client_base.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)   104324 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/gtk_client_window_base.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3708 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/gtk_keyboard_helper.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1674 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/gtk_spinner.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    73876 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/gtk_tray_menu_base.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3888 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/mdns_gui.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    18598 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/menu_helper.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    13551 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/open_requests.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4301 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/pass_dialog.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     9619 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/server_commands.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    62947 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/session_info.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    19605 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/sessions_gui.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     7046 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/start_new_command.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     7025 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/statusicon_tray.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     7293 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/toolbox.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4477 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/u2f_tool.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4974 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/update_status.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    10529 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/gtk_base/window_info.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    14788 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/keyboard_helper.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     6625 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/keyboard_shortcuts_parser.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      537 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/mixin_features.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.298652 xpra-4.4.5/xpra/client/mixins/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/mixins/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    27030 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/mixins/audio.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    15243 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/mixins/clipboard.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    27009 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/mixins/display.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    14129 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/mixins/encodings.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     8264 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/mixins/fileprint_mixin.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5839 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/mixins/mmap.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    10297 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/mixins/network_listener.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    14856 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/mixins/network_state.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     7384 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/mixins/notifications.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     6295 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/mixins/remote_logging.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4305 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/mixins/rpc.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4533 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/mixins/serverinfo_mixin.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3238 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/mixins/stub_client_mixin.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5248 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/mixins/tray.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    13862 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/mixins/webcam.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    69404 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/mixins/window_manager.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2504 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/paint_colors.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    11888 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/rfb_protocol.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5729 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/scaling_parser.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      765 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/spinner.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    30722 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/top_client.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5210 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/tray_base.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    35194 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/ui_client_base.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    38810 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/window_backing_base.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      965 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/client/window_border.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.298652 xpra-4.4.5/xpra/clipboard/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/clipboard/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    31444 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/clipboard/clipboard_core.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5896 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/clipboard/clipboard_timeout_helper.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.299651 xpra-4.4.5/xpra/codecs/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/__init__.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.299651 xpra-4.4.5/xpra/codecs/argb/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      272 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/argb/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      579 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/argb/argb.pxd
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    29601 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/argb/argb.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4822 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/argb/encoder.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      810 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/argb/scale.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.300651 xpra-4.4.5/xpra/codecs/avif/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/avif/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    20278 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/avif/avif.pxd
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     8417 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/avif/decoder.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     7391 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/avif/encoder.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    26106 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/codec_checks.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     7001 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/codec_constants.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      710 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/codec_debug.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.300651 xpra-4.4.5/xpra/codecs/csc_cython/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      219 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/csc_cython/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    39950 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/csc_cython/colorspace_converter.pyx
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.300651 xpra-4.4.5/xpra/codecs/csc_libyuv/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      219 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/csc_libyuv/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    20006 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/csc_libyuv/colorspace_converter.pyx
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.300651 xpra-4.4.5/xpra/codecs/csc_swscale/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      219 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/csc_swscale/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    24047 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/csc_swscale/colorspace_converter.pyx
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.300651 xpra-4.4.5/xpra/codecs/cuda_common/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/cuda_common/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    22747 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/cuda_common/cuda_context.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.301651 xpra-4.4.5/xpra/codecs/dec_avcodec2/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      219 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/dec_avcodec2/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    38227 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/dec_avcodec2/decoder.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      468 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/dec_avcodec2/register_compat.c
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      243 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/dec_avcodec2/register_compat.h
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.301651 xpra-4.4.5/xpra/codecs/drm/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3441 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/drm/drm.pyx
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.301651 xpra-4.4.5/xpra/codecs/enc_ffmpeg/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/enc_ffmpeg/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    74074 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/enc_ffmpeg/encoder.pyx
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.301651 xpra-4.4.5/xpra/codecs/enc_proxy/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/enc_proxy/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4469 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/enc_proxy/encoder.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.301651 xpra-4.4.5/xpra/codecs/enc_x264/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      219 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/enc_x264/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    42251 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/enc_x264/encoder.pyx
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.302652 xpra-4.4.5/xpra/codecs/enc_x265/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/enc_x265/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    25341 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/enc_x265/encoder.pyx
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.302652 xpra-4.4.5/xpra/codecs/evdi/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/evdi/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    19890 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/evdi/capture.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1058 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/evdi/evdi_compat.h
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1626 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/evdi/load.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4754 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/icon_util.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     7832 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/image_wrapper.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.302652 xpra-4.4.5/xpra/codecs/jpeg/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/jpeg/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    13828 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/jpeg/decoder.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    16913 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/jpeg/encoder.pyx
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.302652 xpra-4.4.5/xpra/codecs/libav_common/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/libav_common/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      326 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/libav_common/av_log.pxd
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4337 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/libav_common/av_log.pyx
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    17329 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/loader.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    15649 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/nv_util.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.303651 xpra-4.4.5/xpra/codecs/nvenc/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/nvenc/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)   184280 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/nvenc/encoder.pyx
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.303651 xpra-4.4.5/xpra/codecs/nvfbc/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/nvfbc/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2860 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/nvfbc/capture.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2992 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/nvfbc/cuda_image_wrapper.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    39225 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/nvfbc/fbc_capture_linux.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    44173 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/nvfbc/fbc_capture_win.pyx
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.304651 xpra-4.4.5/xpra/codecs/nvjpeg/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/nvjpeg/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4116 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/nvjpeg/common.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    11273 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/nvjpeg/decoder.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    22564 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/nvjpeg/encoder.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5278 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/nvjpeg/nvjpeg.pxd
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.304651 xpra-4.4.5/xpra/codecs/pillow/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      982 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/pillow/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     7083 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/pillow/decoder.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    10966 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/pillow/encoder.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3780 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/rgb_transform.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.304651 xpra-4.4.5/xpra/codecs/spng/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/spng/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4660 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/spng/decoder.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     8253 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/spng/encoder.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2750 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/spng/spng.pxd
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.305651 xpra-4.4.5/xpra/codecs/v4l2/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/v4l2/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    19326 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/v4l2/pusher.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      321 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/v4l2/video.h
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    19408 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/video_helper.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.305651 xpra-4.4.5/xpra/codecs/vpx/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      219 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/vpx/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    10724 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/vpx/decoder.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    29312 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/vpx/encoder.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1732 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/vpx/vpx.pxd
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.305651 xpra-4.4.5/xpra/codecs/webp/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      218 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/webp/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    15610 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/webp/decoder.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    34416 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/codecs/webp/encoder.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4681 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/colorstreamhandler.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3888 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/common.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.306651 xpra-4.4.5/xpra/dbus/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/dbus/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      900 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/dbus/common.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4232 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/dbus/helper.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     6747 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/dbus/notifications_forwarder.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2631 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/exit_codes.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.307651 xpra-4.4.5/xpra/gtk_common/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      369 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/gtk_common/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2745 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/gtk_common/about.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4028 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/gtk_common/auth_dialog.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      837 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/gtk_common/cursor_names.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5680 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/gtk_common/desktop_greeter.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     8113 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/gtk_common/error.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2720 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/gtk_common/gobject_compat.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1449 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/gtk_common/gobject_util.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     6114 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/gtk_common/graph.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     7651 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/gtk_common/gtk2_notifier-LICENSE.txt
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.307651 xpra-4.4.5/xpra/gtk_common/gtk3/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/gtk_common/gtk3/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2092 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/gtk_common/gtk3/gdk_atoms.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      742 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/gtk_common/gtk3/gdk_bindings.pxd
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4398 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/gtk_common/gtk3/gdk_bindings.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5601 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/gtk_common/gtk_clipboard.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    14794 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/gtk_common/gtk_notifier.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    29404 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/gtk_common/gtk_util.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     9861 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/gtk_common/gtk_view_clipboard.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     6488 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/gtk_common/gtk_view_keyboard.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9498 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/gtk_common/gui.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2774 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/gtk_common/keymap.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    48405 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/gtk_common/start_gui.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.308651 xpra-4.4.5/xpra/keyboard/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/keyboard/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    28201 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/keyboard/layouts.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1654 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/keyboard/mask.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    19133 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/log.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      873 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/make_thread.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.310651 xpra-4.4.5/xpra/net/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      218 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/__init__.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.311651 xpra-4.4.5/xpra/net/bencode/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1334 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/bencode/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3563 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/bencode/bencode.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5622 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/bencode/cython_bencode.pyx
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.311651 xpra-4.4.5/xpra/net/brotli/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/brotli/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4011 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/brotli/compressor.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5218 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/brotli/decompressor.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    23619 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/bytestreams.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3227 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/common.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     7953 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/compression.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     8574 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/crypto.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    13099 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/d3des.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3814 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/digest.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1536 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/fake_jitter.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    43937 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/file_transfer.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1621 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/header.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    16757 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/http_handler.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5549 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/libproxy.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3852 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/lz4.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      412 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/lz4_compat.h
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.311651 xpra-4.4.5/xpra/net/mdns/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1647 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/mdns/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4845 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/mdns/avahi_listener.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    10322 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/mdns/avahi_publisher.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3626 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/mdns/zeroconf_listener.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     7921 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/mdns/zeroconf_publisher.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    14629 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/mmap_pipe.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    21743 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/net_util.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5122 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/packet_encoding.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    58691 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/protocol.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      986 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/protocol_classes.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5364 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/pycryptography_backend.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2210 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/qrcode.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2434 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/qrencode.pyx
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.311651 xpra-4.4.5/xpra/net/rencodeplus/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/rencodeplus/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    16719 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/rencodeplus/rencodeplus.pyx
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.312651 xpra-4.4.5/xpra/net/rfb/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/rfb/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     6743 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/rfb/rfb_const.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3996 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/rfb/rfb_encode.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    11666 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/rfb/rfb_protocol.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    53805 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/socket_util.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    50855 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/ssh.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2982 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/sshfp.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    17520 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/subprocess_wrapper.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9713 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/upnp.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5347 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/vsock.pyx
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.312651 xpra-4.4.5/xpra/net/websockets/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/websockets/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4301 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/websockets/common.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4961 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/websockets/handler.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2448 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/websockets/header.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.313651 xpra-4.4.5/xpra/net/websockets/headers/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/websockets/headers/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      917 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/websockets/headers/browser_cookie.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      609 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/websockets/headers/default.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      501 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/websockets/headers/env_cookie.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2727 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/websockets/mask.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5950 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/net/websockets/protocol.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.313651 xpra-4.4.5/xpra/notifications/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/notifications/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1920 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/notifications/common.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9328 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/notifications/dbus_notifier.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2791 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/notifications/notifier_base.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2121 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/notifications/pynotify_notifier.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    29649 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/os_util.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.315651 xpra-4.4.5/xpra/platform/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3946 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      423 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/autostart.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.316651 xpra-4.4.5/xpra/platform/darwin/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1700 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/darwin/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/darwin/dotxpra.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      569 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/darwin/features.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2002 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/darwin/gdk3_bindings.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     7065 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/darwin/gl_context.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    31966 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/darwin/gui.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      495 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/darwin/info.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9820 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/darwin/keyboard.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4346 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/darwin/keyboard_config.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4341 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/darwin/netdev_query.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      434 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/darwin/nsevent_glue.h
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      554 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/darwin/nsevent_glue.m
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    12377 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/darwin/osx_clipboard.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    18449 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/darwin/osx_menu.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4108 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/darwin/osx_tray.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     7508 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/darwin/paths.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      362 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/darwin/printing.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    10074 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/darwin/shadow_server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      301 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/darwin/transparency_glue.h
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      434 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/darwin/transparency_glue.m
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3023 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/displayfd.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    10506 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/dotxpra.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      486 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/dotxpra_common.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2990 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/features.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1340 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/gl_context.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    11575 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/gui.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2495 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/info.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2693 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/keyboard.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3955 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/keyboard_base.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2098 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/menu_helper.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2716 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/netdev_query.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    12793 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/paths.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     6313 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/printing.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      397 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/proxy_server.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    20039 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/pycups_printing.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      405 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/shadow_server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     6376 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/ui_thread_watcher.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2901 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/webcam.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.321651 xpra-4.4.5/xpra/platform/win32/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    15246 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    31372 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/clipboard.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    28672 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/common.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3104 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/comtypes_util.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    98698 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/constants.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    18295 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/create_process_lib.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    25114 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/desktoplogon_lib.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2490 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/directsound.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3150 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/dotxpra.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2251 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/dpi.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3642 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/dwm_color.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      992 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/features.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9457 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/gdi_screen_capture.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     8651 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/gl_context.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3466 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/glwin32.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    54780 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/gui.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3242 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/icon_util.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      806 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/info.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    13837 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/keyboard.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    17618 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/keyboard_config.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    24048 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/lsa_logon_lib.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4174 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/menu_helper.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.321651 xpra-4.4.5/xpra/platform/win32/namedpipes/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/namedpipes/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     7677 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/namedpipes/common.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9034 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/namedpipes/connection.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    12862 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/namedpipes/listener.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3843 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/netdev_query.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9530 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/paths.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     8001 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/pdfium.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    17904 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/printer_notify.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9118 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/printing.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1491 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/propsys.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5422 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/proxy_server.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.322651 xpra-4.4.5/xpra/platform/win32/scripts/
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      709 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/scripts/exec.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1175 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/scripts/execfile.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)       95 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/scripts/proxy.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1492 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/scripts/shadow_server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2811 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/setappid.cpp
+-rw-r--r--   0 antoine   (1000) antoine   (1000)       94 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/setappid.h
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    25623 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/shadow_server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1834 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/webcam.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    20363 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/win32_NotifyIcon.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4821 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/win32_balloon.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     8423 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/win32_events.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3062 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/win32_notifier.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     7749 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/win32_printing.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     4265 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/win32_tray.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3146 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/win32_webcam.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     6867 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/window_hooks.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    22692 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/wndproc_events.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     9257 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/win32/wtsapi.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.323651 xpra-4.4.5/xpra/platform/xposix/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      211 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/xposix/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     6687 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/xposix/appindicator_tray.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1546 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/xposix/autostart.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/xposix/dotxpra.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1807 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/xposix/features.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     8172 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/xposix/gl_context.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    41354 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/xposix/gui.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      219 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/xposix/info.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     8672 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/xposix/keyboard.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    19414 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/xposix/menu_helper.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9307 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/xposix/netdev_query.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5665 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/xposix/paths.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      276 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/xposix/printing.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1376 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/xposix/proc.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3053 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/xposix/sd_listen.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      325 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/xposix/shadow_server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     6796 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/platform/xposix/webcam.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4027 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/queue_scheduler.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     7872 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/rectangle.pyx
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.325651 xpra-4.4.5/xpra/scripts/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      211 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/scripts/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1324 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/scripts/bug_report.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    65162 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/scripts/config.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4179 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/scripts/fdproxy.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1150 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/scripts/gtk_info.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)   152198 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/scripts/main.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)   101020 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/scripts/parsing.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     9536 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/scripts/pinentry_wrapper.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    63456 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/scripts/server.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2097 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/scripts/show_webcam.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1109 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/scripts/version.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2031 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/scripts/win32_service.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.326651 xpra-4.4.5/xpra/server/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      307 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/__init__.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.329651 xpra-4.4.5/xpra/server/auth/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      236 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      529 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/allow_auth.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2089 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/auth_helper.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1168 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/capability_auth.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      644 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/env_auth.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3476 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/exec_auth.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      310 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/fail_auth.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1737 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/file_auth.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3527 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/file_auth_base.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3164 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/gss_auth.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3405 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/hosts_auth.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3372 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/kerberos_password_auth.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3838 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/kerberos_token_auth.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     7885 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/keycloak_auth.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     5616 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/ldap3_auth.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     6647 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/ldap_auth.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4539 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/multifile_auth.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2620 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/mysql_auth.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      740 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/none_auth.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3512 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/otp_auth.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2430 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/pam_auth.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      607 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/password_auth.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4323 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/peercred_auth.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1146 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/reject_auth.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1914 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/sql_auth.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     7108 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/sqlauthbase.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3416 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/sqlite_auth.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9636 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/sys_auth_base.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     5811 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/u2f_auth.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     3130 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/auth/win32_auth.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3475 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/background_worker.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     6031 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/control_command.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     7443 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/cystats.pyx
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.329651 xpra-4.4.5/xpra/server/dbus/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/dbus/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1010 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/dbus/dbus_common.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    14093 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/dbus/dbus_server.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2793 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/dbus/dbus_server_base.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     6122 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/dbus/dbus_source.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2599 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/dbus/dbus_start.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    13985 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/gtk_server_base.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2627 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/keyboard_config_base.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     8564 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/menu_provider.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.331651 xpra-4.4.5/xpra/server/mixins/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/mixins/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    18552 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/mixins/audio_server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    17620 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/mixins/child_command_server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    10467 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/mixins/clipboard_server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3287 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/mixins/dbusrpc_server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    15014 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/mixins/display_manager.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    10349 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/mixins/encoding_server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    14384 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/mixins/fileprint_server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    18261 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/mixins/input_server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     7797 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/mixins/logging_server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1094 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/mixins/mmap_server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     7569 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/mixins/networkstate_server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     8599 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/mixins/notification_forwarder.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    38802 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/mixins/server_base_controlcommands.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      949 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/mixins/shell_server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4094 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/mixins/stub_server_mixin.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5048 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/mixins/webcam_server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    16274 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/mixins/window_server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    11210 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/pam.pyx
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.331651 xpra-4.4.5/xpra/server/proxy/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/proxy/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1282 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/proxy/proxy_dbus_server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    37464 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/proxy/proxy_instance.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    14672 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/proxy/proxy_instance_process.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2618 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/proxy/proxy_instance_thread.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    31865 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/proxy/proxy_server.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.332651 xpra-4.4.5/xpra/server/rfb/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/rfb/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4886 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/rfb/rfb_protocol.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     8509 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/rfb/rfb_server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5622 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/rfb/rfb_source.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    40869 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/server_base.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)   104975 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/server_core.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      653 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/server_features.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    18820 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/server_util.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      947 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/server_uuid.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.332651 xpra-4.4.5/xpra/server/shadow/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/shadow/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2690 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/shadow/gtk_root_window_model.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    19101 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/shadow/gtk_shadow_server_base.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     6640 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/shadow/root_window_model.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)      643 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/shadow/shadow_dbus_server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    18655 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/shadow/shadow_server_base.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.334651 xpra-4.4.5/xpra/server/source/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/source/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    24062 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/source/audio_mixin.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3989 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/source/avsync_mixin.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    17154 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/source/client_connection.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     6888 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/source/client_connection_factory.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     6746 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/source/clientdisplay_mixin.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     6585 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/source/clientinfo_mixin.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     6445 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/source/clipboard_connection.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1478 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/source/dbus_mixin.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    24565 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/source/encodings_mixin.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     7417 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/source/fileprint_mixin.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4907 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/source/idle_mixin.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5386 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/source/input_mixin.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     6187 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/source/mmap_connection.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4708 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/source/networkstate_mixin.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3279 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/source/notification_mixin.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2621 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/source/shell_mixin.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    16093 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/source/source_stats.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2225 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/source/stub_source_mixin.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9442 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/source/webcam_mixin.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    28287 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/source/windows_mixin.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    22977 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/ssh.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.336651 xpra-4.4.5/xpra/server/window/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/window/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5789 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/window/batch_config.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    16186 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/window/batch_delay_calculator.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    10846 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/window/content_guesser.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2688 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/window/filters.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5835 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/window/metadata.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    14048 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/window/motion.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9986 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/window/video_scoring.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    25816 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/window/video_subregion.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)   128296 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/window/window_source.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    14756 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/window/window_stats.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)   117654 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/window/window_video_source.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    11608 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/server/window/windowicon_source.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4934 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/simple_stats.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.336651 xpra-4.4.5/xpra/sound/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      241 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/sound/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1909 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/sound/common.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    36453 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/sound/gstreamer_util.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.337651 xpra-4.4.5/xpra/sound/pulseaudio/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      241 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/sound/pulseaudio/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2420 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/sound/pulseaudio/pulseaudio_common_util.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1003 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/sound/pulseaudio/pulseaudio_none_util.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     7730 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/sound/pulseaudio/pulseaudio_pactl_util.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     2733 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/sound/pulseaudio/pulseaudio_util.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    21065 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/sound/sink.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    17106 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/sound/sound_pipeline.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    18118 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/sound/src.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    16585 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/sound/wrapper.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)       70 2023-05-23 12:16:25.000000 xpra-4.4.5/xpra/src_info.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    32992 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/util.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    10548 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/version_util.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.339651 xpra-4.4.5/xpra/x11/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      368 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/__init__.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.341651 xpra-4.4.5/xpra/x11/bindings/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      277 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/bindings/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      437 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/bindings/core_bindings.pxd
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4423 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/bindings/core_bindings.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      363 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/bindings/display_source.pxd
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1117 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/bindings/display_source.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    45040 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/bindings/keyboard_bindings.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2457 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/bindings/posix_display_source.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    51999 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/bindings/randr_bindings.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      642 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/bindings/randr_info.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3548 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/bindings/res_bindings.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1083 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/bindings/wait_for_x_server.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    51784 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/bindings/window_bindings.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    26109 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/bindings/xi2_bindings.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    32988 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/bindings/ximage.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    18864 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/bindings/xlib.pxd
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2240 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/bindings/xwait.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      871 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/common.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.341651 xpra-4.4.5/xpra/x11/dbus/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/dbus/__init__.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     1061 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/dbus/x11_dbus_server.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.341651 xpra-4.4.5/xpra/x11/desktop/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/desktop/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     6090 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/desktop/desktop_model.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5667 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/desktop/desktop_server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    13827 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/desktop/desktop_server_base.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     6084 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/desktop/model_base.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3771 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/desktop/monitor_model.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    14785 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/desktop/monitor_server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5312 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/expand_server.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)     5373 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/fakeXinerama.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.342651 xpra-4.4.5/xpra/x11/gtk3/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      326 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/gtk3/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    44034 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/gtk3/gdk_bindings.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2266 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/gtk3/gdk_display_source.pyx
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      827 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/gtk3/gdk_display_util.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      380 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/gtk3/gdk_x11_macros.c
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      253 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/gtk3/gdk_x11_macros.h
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.343651 xpra-4.4.5/xpra/x11/gtk_x11/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      590 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/gtk_x11/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    31616 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/gtk_x11/clipboard.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5316 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/gtk_x11/composite.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1925 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/gtk_x11/gdk_bindings.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      533 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/gtk_x11/gdk_display_source.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1903 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/gtk_x11/keys.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5890 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/gtk_x11/prop.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     7195 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/gtk_x11/selection.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2506 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/gtk_x11/send_wm.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    11570 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/gtk_x11/tray.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     8052 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/gtk_x11/window_damage.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    20258 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/gtk_x11/wm.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     4626 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/gtk_x11/wm_check.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     9893 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/gtk_x11/world_window.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.344651 xpra-4.4.5/xpra/x11/models/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      213 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/models/__init__.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    30891 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/models/base.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    35537 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/models/core.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5204 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/models/model_stub.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1815 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/models/or_window.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     3474 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/models/size_hints_util.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1940 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/models/systray.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    40418 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/models/window.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    11750 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/prop_conv.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    62819 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    35429 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/server_keyboard_config.py
+-rwxr-xr-x   0 antoine   (1000) antoine   (1000)    18278 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/shadow_x11_server.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5916 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/uinput_device.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    20404 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/vfb_util.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1151 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/window_info.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    19651 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/x11_server_base.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    46670 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/x11_server_core.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     2956 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/x11_window_filters.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    35516 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/xkbhelper.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     1828 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/xroot_props.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     5370 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/xsettings.py
+-rw-r--r--   0 antoine   (1000) antoine   (1000)     8187 2023-05-23 12:16:20.000000 xpra-4.4.5/xpra/x11/xsettings_prop.py
+drwxr-xr-x   0 antoine   (1000) antoine   (1000)        0 2023-05-23 12:16:26.286651 xpra-4.4.5/xpra.egg-info/
+-rw-r--r--   0 antoine   (1000) antoine   (1000)      440 2023-05-23 12:16:25.000000 xpra-4.4.5/xpra.egg-info/PKG-INFO
+-rw-r--r--   0 antoine   (1000) antoine   (1000)    45302 2023-05-23 12:16:26.000000 xpra-4.4.5/xpra.egg-info/SOURCES.txt
+-rw-r--r--   0 antoine   (1000) antoine   (1000)        1 2023-05-23 12:16:25.000000 xpra-4.4.5/xpra.egg-info/dependency_links.txt
+-rw-r--r--   0 antoine   (1000) antoine   (1000)        5 2023-05-23 12:16:25.000000 xpra-4.4.5/xpra.egg-info/top_level.txt
```

### Comparing `xpra-4.4.4/.github/ISSUE_TEMPLATE/bug_report.md` & `xpra-4.4.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/.github/ISSUE_TEMPLATE/feature_request.md` & `xpra-4.4.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/.gitignore` & `xpra-4.4.5/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 # temporary files:
 *.swp
 
 # Python cache:
 __pycache__/
 *.py[cod]
+# generated when building:
+xpra.egg-info
 
 # Coverage tools:
 .coverage
 .coverage.*
 coverage.xml
 htmlcov/
```

### Comparing `xpra-4.4.4/COPYING` & `xpra-4.4.5/COPYING`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/MANIFEST.in` & `xpra-4.4.5/MANIFEST.in`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 include xpra/buffers/memalign.c
 include xpra/buffers/xxhash.h
 include xpra/buffers/xxhash.c
 include xpra/buffers/xxh3.h
 include xpra/net/lz4_compat.h
 include xpra/x11/gtk3/gdk_x11_macros.c
 include xpra/x11/gtk3/gdk_x11_macros.h
-include xpra/codecs/evdi/evdi_compat.c
+include xpra/codecs/evdi/evdi_compat.h
 include xpra/codecs/v4l2/video.h
 include xpra/codecs/dec_avcodec2/register_compat.*
 include xpra/platform/win32/setappid.cpp
 include xpra/platform/win32/setappid.h
 prune html5
 recursive-include fs *
 recursive-include docs *
```

### Comparing `xpra-4.4.4/README.md` & `xpra-4.4.5/README.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Build/Debian.md` & `xpra-4.4.5/docs/Build/Debian.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Build/Dependencies.md` & `xpra-4.4.5/docs/Build/Dependencies.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Build/MSWindows.md` & `xpra-4.4.5/docs/Build/MSWindows.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Build/MacOS.md` & `xpra-4.4.5/docs/Build/MacOS.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Build/Other.md` & `xpra-4.4.5/docs/Build/Other.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Build/README.md` & `xpra-4.4.5/docs/Build/README.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Build/RPM.md` & `xpra-4.4.5/docs/Build/RPM.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/CHANGELOG.md` & `xpra-4.4.5/docs/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,85 @@
 # Changelog
 
+## [4.4.5] 2023-05-14
+* major fixes:
+    * [use after free crash in GTK](https://github.com/Xpra-org/xpra/commit/a0cc7229a0ee8443e6b99d587e94143905bad337)
+    * [ensure X11 errors don't propagate to GTK](https://github.com/Xpra-org/xpra/commit/ae2b0f7c827ee4731717f5607844b833a7efbf93)
+    * [windows losing focus](https://github.com/Xpra-org/xpra/commit/a2c9596b3cb89f11b4082cc6b10bdc8da71fdfd1)
+    * [fix legacy URL format parsing](https://github.com/Xpra-org/xpra/commit/f7dd338a803c1ca7ba45ece31bfd7a38a2f0f40c)
+    * [brolti errors on some platforms](https://github.com/Xpra-org/xpra/commit/cb1819ee5c0feb447276ed8c09c0b0ee99479fb7)
+    * [keyboard shortcuts with Wayland clients and NumLock](https://github.com/Xpra-org/xpra/commit/466e60625be63503c80ebc58ae8815a871bb6916)
+    * [client sockets overwriting server sockets](https://github.com/Xpra-org/xpra/commit/ae52c7c8bf6fc253955eda9e0d31c6c3deffb726)
+    * [network queue flushing](https://github.com/Xpra-org/xpra/commit/bcc39fea455898e9d51a82c0eb460aca51516431)
+    * [correct check for disabled monitors](https://github.com/Xpra-org/xpra/commit/0e426927c1076f611e26723dfda599f04bae2795)
+    * [stop as soon as we find a valid mDNS backend](https://github.com/Xpra-org/xpra/commit/515b81034422cc5a0b0add6a5a9da8a5448c887b)
+    * [only allow logging tweaks via env vars for non-root users](https://github.com/Xpra-org/xpra/commit/9c6ea192025aa88633e2f729d61c2232cb2edfce)
+* packaging:
+    * [dummy driver RPM version 0.4.1](https://github.com/Xpra-org/xpra/commit/b74bdedc873ddc2c4ecda3107e3e57e8abc96c92)
+    * [modules not excluded due to typo](https://github.com/Xpra-org/xpra/commit/364cc6b7abe966ccb56591dd8ccd9103dc52aaf5)
+    * [avoid permissions issues with mv](https://github.com/Xpra-org/xpra/commit/8891c2c16aa592f342b8130633df46cc49106696)
+    * [remove legacy MacOS bundler workaround](https://github.com/Xpra-org/xpra/commit/ed79b148cde00204dd16b9378b8a317be2477c0f)
+    * [support MacOS arm64 builds](https://github.com/Xpra-org/xpra/commit/7e7519a0b8f68f8ec144c149f56903752e484f83)
+    * [fail early with a more useful message on MacOS](https://github.com/Xpra-org/xpra/commit/b814cd88c41b3afd1a014f714a7462c9098e5416)
+    * [setuptools packaging workarounds on MacOS](https://github.com/Xpra-org/xpra/commit/ff2d8237fa66e3bdefc054801d63b6621f8c7b03)
+    * [don't ship .cpp source files in MacOS app](https://github.com/Xpra-org/xpra/commit/b38dd4ba338a17c1e3483072aca6d007ff754bb4)
+    * [compilation errors](https://github.com/Xpra-org/xpra/commit/0758655f98f6d05a7407f0bd4698b65ccb992301) [with gcc version 7 and older](https://github.com/Xpra-org/xpra/commit/9fe67037f97dd77e184762abb4c00d250203519d)
+    * [RHEL 8.x needs pycuda 2022.1 or older](https://github.com/Xpra-org/xpra/commit/7c742de33aa2e7d0d6f5cee96aa550396ab81901)
+    * [RHEL 9.x can install pandoc from EPEL](https://github.com/Xpra-org/xpra/commit/9c3828bdecdba4c6b8802ce7b9ca0de557583ba8)
+    * [silence python cryptography OpenSSL warning on MacOS](https://github.com/Xpra-org/xpra/commit/d5662c6a859503ceb397f1f739d32d86ba86dd90)
+    * [workaround even more exotic library version strings](https://github.com/Xpra-org/xpra/commit/068cd5cb42333f668665adfc5f317a4a46a0c957)
+    * [try](https://github.com/Xpra-org/xpra/commit/1058a9e6f6f978b412b829a5825ac74655eb8c01) [harder](https://github.com/Xpra-org/xpra/commit/ebfdccaa1dd78558a243cc90c764fffe54c81d4c) [to find a working appindicator DEB package](https://github.com/Xpra-org/xpra/commit/7529a2cc55c325e0bad85982c1de926dca0d07b8)
+    * [better compatibility with newer versions of Cython](https://github.com/Xpra-org/xpra/commit/a2ef12623de8f7ee76c3ceaabd20ada21254b0f5)
+    * [we never want a python2 shebang](https://github.com/Xpra-org/xpra/commit/732073c53fb3d2212f7628955be3d8f57a4448d7)
+    * [evdi file missing from MANIFEST](https://github.com/Xpra-org/xpra/commit/20419dea7a824118d2b04d183ea1ebea784554fb)
+    * [missing explicit dependency on `pkgconfig` in RPM spec file](https://github.com/Xpra-org/xpra/commit/0c54f7c2d55fa1eb24ae214e585b83940aba026e)
+    * [skip xsettings dpi when the x11 bindings are missing](https://github.com/Xpra-org/xpra/commit/a762be36c6cacca21a074376622296657579b112)
+    * [ignore setuptools generated cruft](https://github.com/Xpra-org/xpra/commit/303a2c1703ca6efd969d822cea87b3b914ee4282)
+    * [silence rencode RPM patch warnings](https://github.com/Xpra-org/xpra/commit/44ad45e51aef2eb02e7d7e6d605fb9e1cdde4a03)
+    * [missing GStreamer elements for playing `bell` on MS Windows](https://github.com/Xpra-org/xpra/commit/bfc464a17c65ad31b0bb03a8acc6836bac0c11fb)
+* encodings:
+    * [always use lossless encoding for `text`](https://github.com/Xpra-org/xpra/commit/c8950ceab353e15debb1d94958cd7efdf963d209)
+    * [continue to monitor window metadata updates](https://github.com/Xpra-org/xpra/commit/448ebe940c47f4dc26c72d71945edffc55292767)
+    * [honour png palette encodings](https://github.com/Xpra-org/xpra/commit/c5c8a105fb6c2b535bfed0169208d72433df43c5)
+    * [option parsing](https://github.com/Xpra-org/xpra/commit/21c37edd02ace34668037660f5c8703b3ad432b1)
+    * [help command error](https://github.com/Xpra-org/xpra/commit/29a2ba32de16cf7a669d5d33b02f617a0700f56b)
+    * [handle `RGBA` window icon data](https://github.com/Xpra-org/xpra/commit/22c6afead6fbb2b06ab1eddae477c77e73f714b3)
+    * [`ffmpeg` encoder error values](https://github.com/Xpra-org/xpra/commit/1dfdbc3ed8f6dee4faf4040223906f9cb522be0b)
+    * [validate NvFBC Sys capture before enabling it on MS Windows](https://github.com/Xpra-org/xpra/commit/5869397e43481ca9ca6814533443549589c9bb41)
+* minor:
+    * [X11 Atom name memory leak](https://github.com/Xpra-org/xpra/commit/4a4f45d5e39c814d495203b9cd0910cffc846a06)
+    * [handle malformed display names more gracefully](https://github.com/Xpra-org/xpra/commit/0c08c4c3d8f3253bb6fe9c67cf9761c5086f3957)
+    * [if we don't have keycodes to map, don't try to translate them](https://github.com/Xpra-org/xpra/commit/ab639645a52952d7a57b01f9537f2c013a45208a)
+    * [skip negative keyboard codes as per MS Windows specifications](https://github.com/Xpra-org/xpra/commit/0aeece96e41a59a669e1f082cb40d8d451de2dd9)
+    * [fix side buttons on MS Windows](https://github.com/Xpra-org/xpra/commit/034df57d9a4ecd6fd861d98e4e5bf0c7396f7cb6)
+    * [X11 clipboard debug logging parsing of window names](https://github.com/Xpra-org/xpra/commit/dc682aff7512a315296e8b7c92f2a40a79b03336)
+    * [remove unused, potentially problematic statement](https://github.com/Xpra-org/xpra/commit/eff316e444f7cfc9b4d011a2cbbfb75212a9ec6f)
+    * [make it possible to disable `SHA1`](https://github.com/Xpra-org/xpra/commit/77cacbb5d58142654947374e19bbe4da15bb7864)
+    * [avoid errors if `MD5` has already been removed](https://github.com/Xpra-org/xpra/commit/239602d0ad220d53b4bb4a8b539075bcd1d68d70)
+    * [don't try to show an exception that does not exist](https://github.com/Xpra-org/xpra/commit/30d7951bc8014d878d8e07c1ce9f4a769d026773)
+    * [window debug logging error](https://github.com/Xpra-org/xpra/commit/b77f15201bdfdcc6ffb35701890fb37534690de1)
+    * [correctly parse OpenGL diagnostics](https://github.com/Xpra-org/xpra/commit/94a7b28d739089cf96fa543214152bbb07af5d43)
+    * [window forwarding require encoding module](https://github.com/Xpra-org/xpra/commit/f2dd74bac2c4a459cf368ab67461a9467eb2b54d)
+    * [mmap debug flood](https://github.com/Xpra-org/xpra/commit/e9322228b526c85df8c23f4b43e01a8ee95c1016)
+    * [continue with session info despite cursor errors](https://github.com/Xpra-org/xpra/commit/3eae4604af0fcf87853ca4e546e5b65986f1c267)
+    * [handle client server uuid errors more gracefully](https://github.com/Xpra-org/xpra/commit/47f70eea0beeba963f84700a3db0285b795f281d)
+    * [silence shared socket permission warning](https://github.com/Xpra-org/xpra/commit/8f820c7f5ad36c614dc3319f5ff5946d4e7375ba)
+    * [handle missing server attributes without erroring out](https://github.com/Xpra-org/xpra/commit/58d02a34e8753364066c7fbf1ff8f9be5b1f3988)
+    * [correct default method signature](https://github.com/Xpra-org/xpra/commit/8e1be99fdbf57d91e32de97b47a311d1cf3b58a8)
+    * [missing latency data on websocket connections](https://github.com/Xpra-org/xpra/commit/3c4c2c1109c7abb5e278d8f29c948a0a8a04b713)
+    * [service update errors with newer versions of python zeroconf](https://github.com/Xpra-org/xpra/commit/72b111791e21a153eff148c3c01d5b58fa5f3ba4)
+    * [parse IPv6 when looking up network devices](https://github.com/Xpra-org/xpra/commit/773212798f8b28bdb30e3371731dd3030aeb04f0)
+    * [run servers with missing stderr](https://github.com/Xpra-org/xpra/commit/32d2704878013d0ce245ef4a1b409e087d76a411)
+    * [correct server initialization order for cleaner shutdowns on errors](https://github.com/Xpra-org/xpra/commit/7368f0292a669a7a83c1f2bae8f6dc3b3ac7b45e)
+    * [skip systemd-run tests on unsupported platforms](https://github.com/Xpra-org/xpra/commit/05315424f2df69af00388aff241fc15fc1192b22)
+    * [missing test dependency on OracleLinux 8.x](https://github.com/Xpra-org/xpra/commit/7aca69dcf562f4c80babe668cb24506923f18e60)
+    * [MacOS test tool errors](https://github.com/Xpra-org/xpra/commit/28619b69d5131d9a57a4c34796de2353751397ab)
+    * [skip useless 'unknown' message](https://github.com/Xpra-org/xpra/commit/8f6fb5b6819bea424f2cdcd8bb95349dec66361b), [typo](https://github.com/Xpra-org/xpra/commit/4996a5090394230464675f2eeeed9d20a51eaa31)
+    * [more useful codec loader validation message](https://github.com/Xpra-org/xpra/commit/1fd1f792ee6b551e4a64c8cfbb74c6ae7adc0604)
+
 ## [4.4.4] 2023-03-09
 * major fixes:
     * focus [change failures](https://github.com/Xpra-org/xpra/commit/1f12618fccf62516e0c6e71c7b3a87fc18f287cb), [errors with OR windows](https://github.com/Xpra-org/xpra/commit/0137db7f29243d0a1417e56398499b58776d379c)
     * [dpi validation failures](https://github.com/Xpra-org/xpra/commit/cb6ac21da03a19660217d456607676334d4eeda1)
     * [honour dpi when setting initial resolution](https://github.com/Xpra-org/xpra/commit/bee52599d1969b963ca341f5eebfba175738d729)
     * [match the requested desktop size exactly](https://github.com/Xpra-org/xpra/commit/6093b14c78b66596bd148d5c743a10c27eff6092)
     * [XI2 errors](https://github.com/Xpra-org/xpra/commit/f2e9710ad903a3dd8f86b9528e2e4bf418fd36f0)
```

### Comparing `xpra-4.4.4/docs/FAQ.md` & `xpra-4.4.5/docs/FAQ.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Features/Audio.md` & `xpra-4.4.5/docs/Features/Audio.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Features/Clipboard.md` & `xpra-4.4.5/docs/Features/Clipboard.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Features/DPI.md` & `xpra-4.4.5/docs/Features/DPI.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Features/File-Transfers.md` & `xpra-4.4.5/docs/Features/File-Transfers.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Features/Image-Depth.md` & `xpra-4.4.5/docs/Features/Image-Depth.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Features/Keyboard.md` & `xpra-4.4.5/docs/Features/Keyboard.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Features/Notifications.md` & `xpra-4.4.5/docs/Features/Notifications.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Features/Printing.md` & `xpra-4.4.5/docs/Features/Printing.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Features/README.md` & `xpra-4.4.5/docs/Features/README.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Features/System-Tray.md` & `xpra-4.4.5/docs/Features/System-Tray.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Features/Webcam.md` & `xpra-4.4.5/docs/Features/Webcam.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Network/AES.md` & `xpra-4.4.5/docs/Network/AES.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Network/Multicast-DNS.md` & `xpra-4.4.5/docs/Network/Multicast-DNS.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Network/README.md` & `xpra-4.4.5/docs/Network/README.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Network/SSH.md` & `xpra-4.4.5/docs/Network/SSH.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Network/SSL.md` & `xpra-4.4.5/docs/Network/SSL.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/README.md` & `xpra-4.4.5/docs/README.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Usage/Apache-Proxy.md` & `xpra-4.4.5/docs/Usage/Apache-Proxy.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Usage/Authentication.md` & `xpra-4.4.5/docs/Usage/Authentication.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Usage/Client-OpenGL.md` & `xpra-4.4.5/docs/Usage/Client-OpenGL.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Usage/Client.md` & `xpra-4.4.5/docs/Usage/Client.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Usage/Configuration.md` & `xpra-4.4.5/docs/Usage/Configuration.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Usage/Encodings.md` & `xpra-4.4.5/docs/Usage/Encodings.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Usage/Logging.md` & `xpra-4.4.5/docs/Usage/Logging.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Usage/NVENC.md` & `xpra-4.4.5/docs/Usage/NVENC.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Usage/OpenGL.md` & `xpra-4.4.5/docs/Usage/OpenGL.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Usage/Proxy-Server.md` & `xpra-4.4.5/docs/Usage/Proxy-Server.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Usage/README.md` & `xpra-4.4.5/docs/Usage/README.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Usage/Seamless.md` & `xpra-4.4.5/docs/Usage/Seamless.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Usage/Security.md` & `xpra-4.4.5/docs/Usage/Security.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Usage/Service.md` & `xpra-4.4.5/docs/Usage/Service.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Usage/Shadow-Server.md` & `xpra-4.4.5/docs/Usage/Shadow-Server.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Usage/Start-Desktop.md` & `xpra-4.4.5/docs/Usage/Start-Desktop.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Usage/WSL.md` & `xpra-4.4.5/docs/Usage/WSL.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/Usage/Xdummy.md` & `xpra-4.4.5/docs/Usage/Xdummy.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/Xpra-Proxy.png` & `xpra-4.4.5/docs/images/Xpra-Proxy.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/icons/X11.png` & `xpra-4.4.5/docs/images/icons/X11.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/icons/authentication.png` & `xpra-4.4.5/docs/images/icons/authentication.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/icons/clipboard.png` & `xpra-4.4.5/docs/images/icons/clipboard.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/icons/connect.png` & `xpra-4.4.5/docs/images/icons/connect.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/icons/encoding.png` & `xpra-4.4.5/docs/images/icons/encoding.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/icons/freebsd.png` & `xpra-4.4.5/docs/images/icons/freebsd.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/icons/keyboard.png` & `xpra-4.4.5/docs/images/icons/keyboard.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/icons/mdns.png` & `xpra-4.4.5/docs/images/icons/mdns.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/icons/nvidia.png` & `xpra-4.4.5/docs/images/icons/nvidia.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/icons/opengl.png` & `xpra-4.4.5/docs/images/icons/opengl.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/icons/osx.png` & `xpra-4.4.5/docs/images/icons/osx.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/icons/package.png` & `xpra-4.4.5/docs/images/icons/package.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/icons/printer.png` & `xpra-4.4.5/docs/images/icons/printer.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/icons/rpm.png` & `xpra-4.4.5/docs/images/icons/rpm.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/icons/server-connected.png` & `xpra-4.4.5/docs/images/icons/server-connected.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/icons/sound.png` & `xpra-4.4.5/docs/images/icons/sound.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/icons/ssh.png` & `xpra-4.4.5/docs/images/icons/ssh.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/icons/ubuntu.png` & `xpra-4.4.5/docs/images/icons/ubuntu.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/icons/upload.png` & `xpra-4.4.5/docs/images/icons/upload.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/icons/webcam.png` & `xpra-4.4.5/docs/images/icons/webcam.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/icons/windows.png` & `xpra-4.4.5/docs/images/icons/windows.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/mdns-gui.png` & `xpra-4.4.5/docs/images/mdns-gui.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/pavucontrol-client.png` & `xpra-4.4.5/docs/images/pavucontrol-client.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/pavucontrol-server.png` & `xpra-4.4.5/docs/images/pavucontrol-server.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/session-info-graphs.png` & `xpra-4.4.5/docs/images/session-info-graphs.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/session-info-sound.png` & `xpra-4.4.5/docs/images/session-info-sound.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/upload.png` & `xpra-4.4.5/docs/images/upload.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/docs/images/win32-shadow-tray-menu.png` & `xpra-4.4.5/docs/images/win32-shadow-tray-menu.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/README.md` & `xpra-4.4.5/fs/README.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/bin/add_build_info.py` & `xpra-4.4.5/fs/bin/add_build_info.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/bin/run_scaled` & `xpra-4.4.5/fs/bin/run_scaled`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/bin/set_source_version` & `xpra-4.4.5/fs/bin/set_source_version`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/bin/xdummy_cvt_gen.py` & `xpra-4.4.5/fs/bin/xdummy_cvt_gen.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/bin/xpra_Xdummy` & `xpra-4.4.5/fs/bin/xpra_Xdummy`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/etc/README.md` & `xpra-4.4.5/fs/etc/README.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/etc/init.d/xpra` & `xpra-4.4.5/fs/etc/init.d/xpra`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/etc/pam.d/xpra` & `xpra-4.4.5/fs/etc/pam.d/xpra`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/etc/xpra/conf.d/05_features.conf.in` & `xpra-4.4.5/fs/etc/xpra/conf.d/05_features.conf.in`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/etc/xpra/conf.d/10_network.conf.in` & `xpra-4.4.5/fs/etc/xpra/conf.d/10_network.conf.in`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/etc/xpra/conf.d/12_ssl.conf.in` & `xpra-4.4.5/fs/etc/xpra/conf.d/12_ssl.conf.in`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/etc/xpra/conf.d/16_printing.conf.in` & `xpra-4.4.5/fs/etc/xpra/conf.d/16_printing.conf.in`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/etc/xpra/conf.d/20_sound.conf.in` & `xpra-4.4.5/fs/etc/xpra/conf.d/20_sound.conf.in`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/etc/xpra/conf.d/30_picture.conf.in` & `xpra-4.4.5/fs/etc/xpra/conf.d/30_picture.conf.in`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/etc/xpra/conf.d/40_client.conf.in` & `xpra-4.4.5/fs/etc/xpra/conf.d/40_client.conf.in`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/etc/xpra/conf.d/42_client_keyboard.conf.in` & `xpra-4.4.5/fs/etc/xpra/conf.d/42_client_keyboard.conf.in`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/etc/xpra/conf.d/50_server_network.conf.in` & `xpra-4.4.5/fs/etc/xpra/conf.d/50_server_network.conf.in`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/etc/xpra/conf.d/55_server_x11.conf.in` & `xpra-4.4.5/fs/etc/xpra/conf.d/55_server_x11.conf.in`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/etc/xpra/conf.d/60_server.conf.in` & `xpra-4.4.5/fs/etc/xpra/conf.d/60_server.conf.in`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/etc/xpra/content-categories/10_default.conf` & `xpra-4.4.5/fs/etc/xpra/content-categories/10_default.conf`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/etc/xpra/content-type/30_title.conf` & `xpra-4.4.5/fs/etc/xpra/content-type/30_title.conf`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/etc/xpra/content-type/50_class.conf` & `xpra-4.4.5/fs/etc/xpra/content-type/50_class.conf`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/etc/xpra/cuda.conf` & `xpra-4.4.5/fs/etc/xpra/cuda.conf`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/etc/xpra/xorg-randr1.6.conf` & `xpra-4.4.5/fs/etc/xpra/xorg-randr1.6.conf`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/etc/xpra/xorg-uinput.conf` & `xpra-4.4.5/fs/etc/xpra/xorg-uinput.conf`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/etc/xpra/xorg.conf` & `xpra-4.4.5/fs/etc/xpra/xorg.conf`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/etc/xpra/xpra.conf.in` & `xpra-4.4.5/fs/etc/xpra/xpra.conf.in`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/lib/README.md` & `xpra-4.4.5/fs/lib/README.md`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/lib/cups/backend/xpraforwarder` & `xpra-4.4.5/fs/lib/cups/backend/xpraforwarder`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 
 import sys, os, syslog
 import subprocess, traceback
 from urllib.parse import urlparse, parse_qs
 
 
-__version__ = "4.4.4"
+__version__ = "4.4.5"
 
 
 #Writes a syslog entry (msg) at the default facility:
 def debug(msg):
     syslog.syslog(syslog.LOG_DEBUG, msg)
 
 def info(msg):
```

### Comparing `xpra-4.4.4/fs/lib/systemd/system/xpra-nosocketactivation.service` & `xpra-4.4.5/fs/lib/systemd/system/xpra-nosocketactivation.service`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/lib/systemd/system/xpra.service` & `xpra-4.4.5/fs/lib/systemd/system/xpra.service`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/libexec/xpra/gnome-open` & `xpra-4.4.5/fs/libexec/xpra/gnome-open`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/libexec/xpra/gvfs-open` & `xpra-4.4.5/fs/libexec/xpra/gvfs-open`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/libexec/xpra/xdg-open` & `xpra-4.4.5/fs/libexec/xpra/xdg-open`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/libexec/xpra/xpra_signal_listener` & `xpra-4.4.5/fs/libexec/xpra/xpra_signal_listener`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/applications/xpra.desktop` & `xpra-4.4.5/fs/share/applications/xpra.desktop`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/icons/xpra-mdns.png` & `xpra-4.4.5/fs/share/icons/xpra-mdns.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/icons/xpra-shadow.png` & `xpra-4.4.5/fs/share/icons/xpra-shadow.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/icons/xpra.icns` & `xpra-4.4.5/fs/share/icons/xpra.icns`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/icons/xpra.png` & `xpra-4.4.5/fs/share/icons/xpra.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/man/man1/run_scaled.1` & `xpra-4.4.5/fs/share/man/man1/run_scaled.1`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/man/man1/xpra.1` & `xpra-4.4.5/fs/share/man/man1/xpra.1`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/man/man1/xpra_launcher.1` & `xpra-4.4.5/fs/share/man/man1/xpra_launcher.1`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/metainfo/xpra.appdata.xml` & `xpra-4.4.5/fs/share/metainfo/xpra.appdata.xml`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/selinux/cups_xpra/cups_xpra.te` & `xpra-4.4.5/fs/share/selinux/cups_xpra/cups_xpra.te`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/selinux/xpra_socketactivation/xpra_socketactivation.fc` & `xpra-4.4.5/fs/share/selinux/xpra_socketactivation/xpra_socketactivation.fc`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/selinux/xpra_socketactivation/xpra_socketactivation.te` & `xpra-4.4.5/fs/share/selinux/xpra_socketactivation/xpra_socketactivation.te`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/bell.wav` & `xpra-4.4.5/fs/share/xpra/bell.wav`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/cuda/BGRA_to_RGBAP.cu` & `xpra-4.4.5/fs/share/xpra/cuda/BGRA_to_RGBAP.cu`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/cuda/BGRX_to_NV12.cu` & `xpra-4.4.5/fs/share/xpra/cuda/BGRX_to_NV12.cu`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/cuda/BGRX_to_RGB.cu` & `xpra-4.4.5/fs/share/xpra/cuda/BGRX_to_RGB.cu`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/cuda/BGRX_to_YUV444.cu` & `xpra-4.4.5/fs/share/xpra/cuda/BGRX_to_YUV444.cu`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/cuda/RGBA_to_RGBAP.cu` & `xpra-4.4.5/fs/share/xpra/cuda/RGBA_to_RGBAP.cu`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/cuda/RGBX_to_RGB.cu` & `xpra-4.4.5/fs/share/xpra/cuda/RGBX_to_RGB.cu`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/cuda/XRGB_to_NV12.cu` & `xpra-4.4.5/fs/share/xpra/cuda/XRGB_to_NV12.cu`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/cuda/XRGB_to_YUV444.cu` & `xpra-4.4.5/fs/share/xpra/cuda/XRGB_to_YUV444.cu`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/audio.png` & `xpra-4.4.5/fs/share/xpra/icons/audio.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/authentication.ico` & `xpra-4.4.5/fs/share/xpra/icons/authentication.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/authentication.png` & `xpra-4.4.5/fs/share/xpra/icons/authentication.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/bandwidth_limit.png` & `xpra-4.4.5/fs/share/xpra/icons/bandwidth_limit.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/bell.ico` & `xpra-4.4.5/fs/share/xpra/icons/bell.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/bell.png` & `xpra-4.4.5/fs/share/xpra/icons/bell.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/browse.ico` & `xpra-4.4.5/fs/share/xpra/icons/browse.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/browse.png` & `xpra-4.4.5/fs/share/xpra/icons/browse.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/browser.png` & `xpra-4.4.5/fs/share/xpra/icons/browser.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/bugs.ico` & `xpra-4.4.5/fs/share/xpra/icons/bugs.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/bugs.png` & `xpra-4.4.5/fs/share/xpra/icons/bugs.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/clipboard.ico` & `xpra-4.4.5/fs/share/xpra/icons/clipboard.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/clipboard.png` & `xpra-4.4.5/fs/share/xpra/icons/clipboard.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/close.png` & `xpra-4.4.5/fs/share/xpra/icons/close.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/compressed.png` & `xpra-4.4.5/fs/share/xpra/icons/compressed.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/connect.png` & `xpra-4.4.5/fs/share/xpra/icons/connect.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/cuda.ico` & `xpra-4.4.5/fs/share/xpra/icons/cuda.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/directory.ico` & `xpra-4.4.5/fs/share/xpra/icons/directory.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/disconnected.png` & `xpra-4.4.5/fs/share/xpra/icons/disconnected.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/display.png` & `xpra-4.4.5/fs/share/xpra/icons/display.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/documentation.png` & `xpra-4.4.5/fs/share/xpra/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/download.png` & `xpra-4.4.5/fs/share/xpra/icons/download.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/empty.png` & `xpra-4.4.5/fs/share/xpra/icons/empty.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/encoding.ico` & `xpra-4.4.5/fs/share/xpra/icons/encoding.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/encoding.png` & `xpra-4.4.5/fs/share/xpra/icons/encoding.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/eye-off.png` & `xpra-4.4.5/fs/share/xpra/icons/eye-off.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/eye-on.png` & `xpra-4.4.5/fs/share/xpra/icons/eye-on.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/features.ico` & `xpra-4.4.5/fs/share/xpra/icons/features.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/features.png` & `xpra-4.4.5/fs/share/xpra/icons/features.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/fluxbox.png` & `xpra-4.4.5/fs/share/xpra/icons/fluxbox.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/font.ico` & `xpra-4.4.5/fs/share/xpra/icons/font.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/font.png` & `xpra-4.4.5/fs/share/xpra/icons/font.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/forward.png` & `xpra-4.4.5/fs/share/xpra/icons/forward.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/freebsd.png` & `xpra-4.4.5/fs/share/xpra/icons/freebsd.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/gears.ico` & `xpra-4.4.5/fs/share/xpra/icons/gears.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/gnome-session.png` & `xpra-4.4.5/fs/share/xpra/icons/gnome-session.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/gnome.png` & `xpra-4.4.5/fs/share/xpra/icons/gnome.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/gstreamer.ico` & `xpra-4.4.5/fs/share/xpra/icons/gstreamer.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/gtk.ico` & `xpra-4.4.5/fs/share/xpra/icons/gtk.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/information.ico` & `xpra-4.4.5/fs/share/xpra/icons/information.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/information.png` & `xpra-4.4.5/fs/share/xpra/icons/information.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/kde.png` & `xpra-4.4.5/fs/share/xpra/icons/kde.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/keyboard.ico` & `xpra-4.4.5/fs/share/xpra/icons/keyboard.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/keyboard.png` & `xpra-4.4.5/fs/share/xpra/icons/keyboard.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/keymap.ico` & `xpra-4.4.5/fs/share/xpra/icons/keymap.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/linux.png` & `xpra-4.4.5/fs/share/xpra/icons/linux.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/list.png` & `xpra-4.4.5/fs/share/xpra/icons/list.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/loop.ico` & `xpra-4.4.5/fs/share/xpra/icons/loop.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/lxde.png` & `xpra-4.4.5/fs/share/xpra/icons/lxde.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/macos.png` & `xpra-4.4.5/fs/share/xpra/icons/macos.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/matchbox.png` & `xpra-4.4.5/fs/share/xpra/icons/matchbox.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/maximize.png` & `xpra-4.4.5/fs/share/xpra/icons/maximize.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/mdns.ico` & `xpra-4.4.5/fs/share/xpra/icons/mdns.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/mdns.png` & `xpra-4.4.5/fs/share/xpra/icons/mdns.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/microphone.ico` & `xpra-4.4.5/fs/share/xpra/icons/microphone.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/microphone.png` & `xpra-4.4.5/fs/share/xpra/icons/microphone.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/minimize.png` & `xpra-4.4.5/fs/share/xpra/icons/minimize.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/network.ico` & `xpra-4.4.5/fs/share/xpra/icons/network.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/nvidia.ico` & `xpra-4.4.5/fs/share/xpra/icons/nvidia.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/open.png` & `xpra-4.4.5/fs/share/xpra/icons/open.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/openbox.png` & `xpra-4.4.5/fs/share/xpra/icons/openbox.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/openbsd.png` & `xpra-4.4.5/fs/share/xpra/icons/openbsd.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/opengl.ico` & `xpra-4.4.5/fs/share/xpra/icons/opengl.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/opengl.png` & `xpra-4.4.5/fs/share/xpra/icons/opengl.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/package.png` & `xpra-4.4.5/fs/share/xpra/icons/package.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/picture.png` & `xpra-4.4.5/fs/share/xpra/icons/picture.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/pointer.png` & `xpra-4.4.5/fs/share/xpra/icons/pointer.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/printer.ico` & `xpra-4.4.5/fs/share/xpra/icons/printer.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/printer.png` & `xpra-4.4.5/fs/share/xpra/icons/printer.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/python.ico` & `xpra-4.4.5/fs/share/xpra/icons/python.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/qr.png` & `xpra-4.4.5/fs/share/xpra/icons/qr.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/quit.png` & `xpra-4.4.5/fs/share/xpra/icons/quit.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/raise.png` & `xpra-4.4.5/fs/share/xpra/icons/raise.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/reinitialize.png` & `xpra-4.4.5/fs/share/xpra/icons/reinitialize.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/retry.png` & `xpra-4.4.5/fs/share/xpra/icons/retry.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/sawfish.png` & `xpra-4.4.5/fs/share/xpra/icons/sawfish.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/scaling.png` & `xpra-4.4.5/fs/share/xpra/icons/scaling.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/screenshot.ico` & `xpra-4.4.5/fs/share/xpra/icons/screenshot.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/screenshot.png` & `xpra-4.4.5/fs/share/xpra/icons/screenshot.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/server-connected.ico` & `xpra-4.4.5/fs/share/xpra/icons/server-connected.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/server-connected.png` & `xpra-4.4.5/fs/share/xpra/icons/server-connected.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/server-notconnected.ico` & `xpra-4.4.5/fs/share/xpra/icons/server-notconnected.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/server-notconnected.png` & `xpra-4.4.5/fs/share/xpra/icons/server-notconnected.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/server.png` & `xpra-4.4.5/fs/share/xpra/icons/server.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/shutdown.png` & `xpra-4.4.5/fs/share/xpra/icons/shutdown.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/slider.png` & `xpra-4.4.5/fs/share/xpra/icons/slider.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/speaker-off.png` & `xpra-4.4.5/fs/share/xpra/icons/speaker-off.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/speaker.ico` & `xpra-4.4.5/fs/share/xpra/icons/speaker.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/speaker.png` & `xpra-4.4.5/fs/share/xpra/icons/speaker.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/speed.png` & `xpra-4.4.5/fs/share/xpra/icons/speed.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/sql.ico` & `xpra-4.4.5/fs/share/xpra/icons/sql.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/sqlite.ico` & `xpra-4.4.5/fs/share/xpra/icons/sqlite.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/sqlite.png` & `xpra-4.4.5/fs/share/xpra/icons/sqlite.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/start.png` & `xpra-4.4.5/fs/share/xpra/icons/start.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/statistics.png` & `xpra-4.4.5/fs/share/xpra/icons/statistics.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/ticked-small.png` & `xpra-4.4.5/fs/share/xpra/icons/ticked-small.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/ticked.png` & `xpra-4.4.5/fs/share/xpra/icons/ticked.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/timer.png` & `xpra-4.4.5/fs/share/xpra/icons/timer.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/toolbox.png` & `xpra-4.4.5/fs/share/xpra/icons/toolbox.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/transfer.png` & `xpra-4.4.5/fs/share/xpra/icons/transfer.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/transparent.ico` & `xpra-4.4.5/fs/share/xpra/icons/transparent.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/unticked.png` & `xpra-4.4.5/fs/share/xpra/icons/unticked.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/update.png` & `xpra-4.4.5/fs/share/xpra/icons/update.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/upload.png` & `xpra-4.4.5/fs/share/xpra/icons/upload.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/user.png` & `xpra-4.4.5/fs/share/xpra/icons/user.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/video.png` & `xpra-4.4.5/fs/share/xpra/icons/video.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/webcam.ico` & `xpra-4.4.5/fs/share/xpra/icons/webcam.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/webcam.png` & `xpra-4.4.5/fs/share/xpra/icons/webcam.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/win32.png` & `xpra-4.4.5/fs/share/xpra/icons/win32.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/windowmaker.png` & `xpra-4.4.5/fs/share/xpra/icons/windowmaker.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/windows.png` & `xpra-4.4.5/fs/share/xpra/icons/windows.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/xpra.ico` & `xpra-4.4.5/fs/share/xpra/icons/xpra.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/xpra.png` & `xpra-4.4.5/fs/share/xpra/icons/xpra.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/xpra_txt.ico` & `xpra-4.4.5/fs/share/xpra/icons/xpra_txt.ico`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/fs/share/xpra/icons/xterm.png` & `xpra-4.4.5/fs/share/xpra/icons/xterm.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MSWindows/BUILD_CUDA_KERNEL.BAT` & `xpra-4.4.5/packaging/MSWindows/BUILD_CUDA_KERNEL.BAT`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MSWindows/DirectShow.tlb` & `xpra-4.4.5/packaging/MSWindows/DirectShow.tlb`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MSWindows/MINGW_BUILD.sh` & `xpra-4.4.5/packaging/MSWindows/MINGW_BUILD.sh`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MSWindows/MINGW_SETUP.sh` & `xpra-4.4.5/packaging/MSWindows/MINGW_SETUP.sh`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MSWindows/SIGN_ALL.sh` & `xpra-4.4.5/packaging/MSWindows/SIGN_ALL.sh`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MSWindows/TaskbarLib.tlb` & `xpra-4.4.5/packaging/MSWindows/TaskbarLib.tlb`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MSWindows/msi.py` & `xpra-4.4.5/packaging/MSWindows/msi.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MSWindows/msi.xml` & `xpra-4.4.5/packaging/MSWindows/msi.xml`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MSWindows/service/DesktopLogon/DesktopLogon.cs` & `xpra-4.4.5/packaging/MSWindows/service/DesktopLogon/DesktopLogon.cs`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MSWindows/service/DesktopLogon/DesktopLogon.csproj` & `xpra-4.4.5/packaging/MSWindows/service/DesktopLogon/DesktopLogon.csproj`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MSWindows/service/DesktopLogon/DesktopLogon.sln` & `xpra-4.4.5/packaging/MSWindows/service/DesktopLogon/DesktopLogon.sln`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MSWindows/service/Xpra-Service.cpp` & `xpra-4.4.5/packaging/MSWindows/service/Xpra-Service.cpp`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MSWindows/service/event_log.mc` & `xpra-4.4.5/packaging/MSWindows/service/event_log.mc`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MSWindows/xpra-logo.bmp` & `xpra-4.4.5/packaging/MSWindows/xpra-logo.bmp`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MSWindows/xpra.bmp` & `xpra-4.4.5/packaging/MSWindows/xpra.bmp`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MSWindows/xpra.iss` & `xpra-4.4.5/packaging/MSWindows/xpra.iss`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 5b53 6574 7570 5d0d 0a41 7070 4e61 6d65  [Setup]..AppName
 00000010: 3d58 7072 610d 0a41 7070 4964 3d58 7072  =Xpra..AppId=Xpr
 00000020: 615f 6973 310d 0a41 7070 5665 7273 696f  a_is1..AppVersio
-00000030: 6e3d 342e 342e 340a 4170 7056 6572 4e61  n=4.4.4.AppVerNa
-00000040: 6d65 3d58 7072 6120 342e 342e 340a 556e  me=Xpra 4.4.4.Un
+00000030: 6e3d 342e 342e 350a 4170 7056 6572 4e61  n=4.4.5.AppVerNa
+00000040: 6d65 3d58 7072 6120 342e 342e 350a 556e  me=Xpra 4.4.5.Un
 00000050: 696e 7374 616c 6c44 6973 706c 6179 4e61  installDisplayNa
-00000060: 6d65 3d58 7072 6120 342e 342e 340a 4170  me=Xpra 4.4.4.Ap
+00000060: 6d65 3d58 7072 6120 342e 342e 350a 4170  me=Xpra 4.4.5.Ap
 00000070: 7050 7562 6c69 7368 6572 3d78 7072 612e  pPublisher=xpra.
 00000080: 6f72 670d 0a41 7070 5075 626c 6973 6865  org..AppPublishe
 00000090: 7255 524c 3d68 7474 703a 3b78 7072 612e  rURL=http:;xpra.
 000000a0: 6f72 672f 0d0a 4465 6661 756c 7444 6972  org/..DefaultDir
 000000b0: 4e61 6d65 3d7b 7066 7d5c 5870 7261 0d0a  Name={pf}\Xpra..
 000000c0: 4465 6661 756c 7447 726f 7570 4e61 6d65  DefaultGroupName
 000000d0: 3d58 7072 610d 0a44 6973 6162 6c65 5072  =Xpra..DisablePr
@@ -20,15 +20,15 @@
 00000130: 3d6e 6f6e 650d 0a3b 436f 6d70 7265 7373  =none..;Compress
 00000140: 696f 6e3d 6c7a 6d61 322f 6661 7374 0d0a  ion=lzma2/fast..
 00000150: 436f 6d70 7265 7373 696f 6e3d 6c7a 6d61  Compression=lzma
 00000160: 322f 6d61 780d 0a53 6f6c 6964 436f 6d70  2/max..SolidComp
 00000170: 7265 7373 696f 6e3d 7965 730d 0a41 6c6c  ression=yes..All
 00000180: 6f77 554e 4350 6174 683d 6661 6c73 650d  owUNCPath=false.
 00000190: 0a56 6572 7369 6f6e 496e 666f 5665 7273  .VersionInfoVers
-000001a0: 696f 6e3d 342e 342e 340a 5665 7273 696f  ion=4.4.4.Versio
+000001a0: 696f 6e3d 342e 342e 350a 5665 7273 696f  ion=4.4.5.Versio
 000001b0: 6e49 6e66 6f43 6f6d 7061 6e79 3d78 7072  nInfoCompany=xpr
 000001c0: 612e 6f72 670d 0a56 6572 7369 6f6e 496e  a.org..VersionIn
 000001d0: 666f 4465 7363 7269 7074 696f 6e3d 6d75  foDescription=mu
 000001e0: 6c74 692d 706c 6174 666f 726d 2073 6372  lti-platform scr
 000001f0: 6565 6e20 616e 6420 6170 706c 6963 6174  een and applicat
 00000200: 696f 6e20 666f 7277 6172 6469 6e67 2073  ion forwarding s
 00000210: 7973 7465 6d0d 0a57 697a 6172 6449 6d61  ystem..WizardIma
```

### Comparing `xpra-4.4.4/packaging/MacOS/Blank.dmg.bz2` & `xpra-4.4.5/packaging/MacOS/Blank.dmg.bz2`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MacOS/C-wrapper.c` & `xpra-4.4.5/packaging/MacOS/C-wrapper.c`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MacOS/GPL.rtf` & `xpra-4.4.5/packaging/MacOS/GPL.rtf`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MacOS/Helpers/PythonExecWrapper` & `xpra-4.4.5/packaging/MacOS/Helpers/PythonExecWrapper`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MacOS/Helpers/Shadow` & `xpra-4.4.5/packaging/MacOS/Helpers/Shadow`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MacOS/Info-template.plist` & `xpra-4.4.5/packaging/MacOS/Info-template.plist`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MacOS/Info.plist` & `xpra-4.4.5/packaging/MacOS/Info.plist`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MacOS/Shell-wrapper.c` & `xpra-4.4.5/packaging/MacOS/Shell-wrapper.c`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MacOS/Xpra.bundle` & `xpra-4.4.5/packaging/MacOS/Xpra.bundle`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MacOS/Xpra.entitlements` & `xpra-4.4.5/packaging/MacOS/Xpra.entitlements`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MacOS/Xpra_NoDock.app/Contents/Info.plist` & `xpra-4.4.5/packaging/MacOS/Xpra_NoDock.app/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MacOS/background.png` & `xpra-4.4.5/packaging/MacOS/background.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MacOS/dmg-icons/background.jpg` & `xpra-4.4.5/packaging/MacOS/dmg-icons/background.jpg`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MacOS/dmg-icons/icon.png` & `xpra-4.4.5/packaging/MacOS/dmg-icons/icon.png`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MacOS/make-DMG.sh` & `xpra-4.4.5/packaging/MacOS/make-DMG.sh`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,15 @@
 
 #get the version and build info from the python build records:
 export PYTHONPATH="${APP_DIR}/Contents/Resources/lib/python/"
 VERSION=`${PYTHON} -c "from xpra import __version__;import sys;sys.stdout.write(__version__)"`
 REVISION=`${PYTHON} -c "from xpra import src_info;import sys;sys.stdout.write(str(src_info.REVISION))"`
 REV_MOD=`${PYTHON} -c "from xpra import src_info;import sys;sys.stdout.write(['','M'][src_info.LOCAL_MODIFICATIONS>0])"`
 BUILD_BIT=`${PYTHON} -c "from xpra import build_info;import sys;sys.stdout.write(str(build_info.BUILD_BIT))"`
-BUILD_INFO="${BUILD_INFO}-Python3"
-if [ "$BUILD_BIT" != "32bit" ]; then
-	BUILD_INFO="${BUILD_INFO}-x86_64"
-fi
+BUILD_INFO="${BUILD_INFO}-Python3-`uname -m`"
 
 DMG_NAME="Xpra$BUILD_INFO-$VERSION-r$REVISION$REV_MOD.dmg"
 if [ "${CLIENT_ONLY}" == "1" ]; then
 	DMG_NAME="Xpra-Client$BUILD_INFO-$VERSION-r$REVISION$REV_MOD.dmg"
 fi
 echo "Creating $DMG_NAME"
```

### Comparing `xpra-4.4.4/packaging/MacOS/make-PKG.sh` & `xpra-4.4.5/packaging/MacOS/make-PKG.sh`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,15 @@
 #get the version and build info from the python build records:
 export PYTHONPATH="${APP_DIR}/Contents/Resources/lib/python/"
 PYTHON="${PYTHON:=python}"
 VERSION=`${PYTHON} -c "from xpra import __version__;import sys;sys.stdout.write(__version__)"`
 REVISION=`${PYTHON} -c "from xpra import src_info;import sys;sys.stdout.write(str(src_info.REVISION))"`
 REV_MOD=`${PYTHON} -c "from xpra import src_info;import sys;sys.stdout.write(['','M'][src_info.LOCAL_MODIFICATIONS>0])"`
 BUILD_BIT=`${PYTHON} -c "from xpra import build_info;import sys;sys.stdout.write(str(build_info.BUILD_BIT))"`
-BUILD_INFO="${BUILD_INFO}-Python3"
-if [ "$BUILD_BIT" != "32bit" ]; then
-	BUILD_INFO="${BUILD_INFO}-x86_64"
-fi
+BUILD_INFO="${BUILD_INFO}-Python3-`uname -m`"
 
 PKG_FILENAME="$APP_NAME$BUILD_INFO-$VERSION-r$REVISION$REV_MOD.pkg"
 rm -f ./image/$PKG_FILENAME >& /dev/null
 echo "Making $PKG_FILENAME"
 
 #create directory structure:
 rm -fr ./image/flat ./image/root
```

### Comparing `xpra-4.4.4/packaging/MacOS/make-app.sh` & `xpra-4.4.5/packaging/MacOS/make-app.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 #!/bin/bash
 
+if [ -z "${JHBUILD_PREFIX}" ]; then
+	echo "JHBUILD_PREFIX is not set"
+	echo "this script must be executed from jhbuild shell"
+	exit 1
+fi
+
 export PYTHON="python3"
 PYTHON_MAJOR_VERSION=`$PYTHON -c 'import sys;sys.stdout.write("%s" % sys.version_info[0])'`
 PYTHON_MINOR_VERSION=`$PYTHON -c 'import sys;sys.stdout.write("%s" % sys.version_info[1])'`
 
 echo "Building Xpra for Python ${PYTHON_MAJOR_VERSION}.${PYTHON_MINOR_VERSION}"
 
 STRIP_DEFAULT="${STRIP_DEFAULT:=1}"
@@ -68,15 +74,15 @@
 	echo
 	tail -n 20 ${BUILD_EXT_LOG}
 	exit 1
 fi
 INSTALL_LOG=`pwd`/install.log
 echo "./setup.py install ${BUILD_ARGS}"
 echo " (see ${INSTALL_LOG} for details)"
-${PYTHON} ./setup.py install --old-and-unmanageable ${BUILD_ARGS} >& ${INSTALL_LOG}
+${PYTHON} ./setup.py install --single-version-externally-managed --root=/ --prefix=$JHBUILD_PREFIX ${BUILD_ARGS} >& ${INSTALL_LOG}
 if [ "$?" != "0" ]; then
 	popd
 	echo "ERROR: install failed"
 	echo
 	tail -n 20 ${INSTALL_LOG}
 	exit 1
 fi
@@ -194,16 +200,16 @@
 fi
 popd
 
 echo
 echo "*******************************************************************************"
 echo "Add xpra/server/python scripts"
 rsync -pltv ./Helpers/* "${HELPERS_DIR}/"
-#we dont need the wrapper installed by distutils:
-rm ${MACOS_DIR}/Launcher-bin
+#we dont need the wrappers that may have been installed by distutils:
+rm -f ${MACOS_DIR}/*bin
 
 #ensure that every wrapper has a "python" executable to match:
 #(see PythonExecWrapper for why we need this "exec -a" workaround)
 for x in `ls "$HELPERS_DIR" | egrep -v "Python|gst-plugin-scanner"`; do
 	#replace underscore with space in actual binary filename:
 	target="$RSCDIR/bin/`echo $x | sed 's+_+ +g'`"
 	if [ ! -e "$target" ]; then
@@ -231,15 +237,15 @@
 
 echo
 echo "*******************************************************************************"
 echo "include all xpra modules found: "
 find $PYTHON_PACKAGES/xpra/* -type d -maxdepth 0 -exec basename {} \;
 rsync -rpl $PYTHON_PACKAGES/xpra/* $LIBDIR/python/xpra/
 echo "removing files that should not be installed in the first place (..)"
-for x in "*.c" "*.pyx" "*.pxd" "constants.pxi" "constants.txt"; do
+for x in "*.c" "*.cpp" "*.pyx" "*.pxd" "constants.pxi" "constants.txt"; do
 	echo "removing $x:"
 	find $LIBDIR/python/xpra/ -name "$x" -print -exec rm "{}" \; | sed "s+$LIBDIR/python/xpra/++g" | xargs -L 1 echo "* "
 done
 #should be redundant:
 if [ "${CLIENT_ONLY}" == "1" ]; then
 	for x in "server" "x11"; do
 		rm -fr "$LIBDIR/python/xpra/$x"
@@ -257,15 +263,15 @@
 	mkdir ${RSCDIR}/LaunchAgents
 	cp ./org.xpra.Agent.plist ${RSCDIR}/LaunchAgents/
 fi
 
 
 echo
 echo "*******************************************************************************"
-echo "Xpra without a tray..."
+echo "Xpra_NoDock: same app contents but without a dock icon"
 for app in Xpra_NoDock.app; do
 	SUB_APP="${APP_DIR}/Contents/${app}"
 	rsync -rplvtog ${app} ${APP_DIR}/Contents/
 	ln -sf ../../Resources ${SUB_APP}/Contents/Resources
 	ln -sf ../../MacOS ${SUB_APP}/Contents/MacOS
 	ln -sf ../../Helpers ${SUB_APP}/Contents/Helpers
 done
@@ -287,15 +293,16 @@
 		rm -fr ./raw/$x
 	done
 	popd
 fi
 echo " * remove numpy"
 rm -fr $LIBDIR/python/numpy
 pushd $LIBDIR/python
-zip --move -ur site-packages.zip OpenGL
+echo " * zipping OpenGL"
+zip --move -q -r site-packages.zip OpenGL
 popd
 echo " * add gobject-introspection (py2app refuses to do it)"
 rsync -rpl $PYTHON_PACKAGES/gi $LIBDIR/python/
 mkdir $LIBDIR/girepository-1.0
 GI_MODULES="Gst GObject GLib GModule Gtk Gdk GtkosxApplication HarfBuzz GL Gio Pango cairo Atk"
 for t in ${GI_MODULES}; do
 	rsync -rpl ${JHBUILD_PREFIX}/lib/girepository-1.0/$t*typelib $LIBDIR/girepository-1.0/
```

### Comparing `xpra-4.4.4/packaging/MacOS/make-appstore-PKG.sh` & `xpra-4.4.5/packaging/MacOS/make-appstore-PKG.sh`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MacOS/postinstall` & `xpra-4.4.5/packaging/MacOS/postinstall`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/MacOS/xpra.icns` & `xpra-4.4.5/packaging/MacOS/xpra.icns`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/debian/xpra/changelog` & `xpra-4.4.5/packaging/debian/xpra/changelog`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,85 @@
+xpra (4.4.5-1) UNRELEASED; urgency=low
+  * major fixes:
+    - use after free crash in GTK
+    - ensure X11 errors don't propagate to GTK
+    - windows losing focus
+    - fix legacy URL format parsing
+    - brolti errors on some platforms
+    - keyboard shortcuts with Wayland clients and NumLock
+    - client sockets overwriting server sockets
+    - network queue flushing
+    - correct check for disabled monitors
+    - stop as soon as we find a valid mDNS backend
+    - only allow logging tweaks via env vars for non-root users
+  * packaging:
+    - dummy driver RPM version 0.4.1
+    - modules not excluded due to typo
+    - avoid permissions issues with mv
+    - remove legacy MacOS bundler workaround
+    - support MacOS arm64 builds
+    - fail early with a more useful message on MacOS
+    - setuptools packaging workarounds on MacOS
+    - don't ship .cpp source files in MacOS app
+    - compilation errors with gcc version 7 and older
+    - RHEL 8.x needs pycuda 2022.1 or older
+    - RHEL 9.x can install pandoc from EPEL
+    - silence python cryptography OpenSSL warning on MacOS
+    - workaround even more exotic library version strings
+    - try harder to find a working appindicator DEB package
+    - better compatibility with newer versions of Cython
+    - we never want a python2 shebang
+    - evdi file missing from MANIFEST
+    - missing explicit dependency on `pkgconfig` in RPM spec file
+    - skip xsettings dpi when the x11 bindings are missing
+    - ignore setuptools generated cruft
+    - silence rencode RPM patch warnings
+    - missing GStreamer elements for playing 'bell' on MS Windows
+  * encodings:
+    - always use lossless encoding for `text`
+    - continue to monitor window metadata updates
+    - honour png palette encodings
+    - option parsing
+    - help command error
+    - handle `RGBA` window icon data
+    - `ffmpeg` encoder error values
+    - validate NvFBC Sys capture before enabling it on MS Windows
+  * minor:
+    - X11 Atom name memory leak
+    - handle malformed display names more gracefully
+    - if we don't have keycodes to map, don't try to translate them
+    - skip negative keyboard codes as per MS Windows specifications
+    - fix side buttons on MS Windows
+    - X11 clipboard debug logging parsing of window names
+    - remove unused, potentially problematic statement
+    - make it possible to disable `SHA1`
+    - avoid errors if `MD5` has already been removed
+    - don't try to show an exception that does not exist
+    - window debug logging error
+    - correctly parse OpenGL diagnostics
+    - window forwarding require encoding module
+    - mmap debug flood
+    - continue with session info despite cursor errors
+    - handle client server uuid errors more gracefully
+    - silence shared socket permission warning
+    - handle missing server attributes without erroring out
+    - correct default method signature
+    - missing latency data on websocket connections
+    - service update errors with newer versions of python zeroconf
+    - parse IPv6 when looking up network devices
+    - run servers with missing stderr
+    - correct server initialization order for cleaner shutdowns on errors
+    - skip systemd-run tests on unsupported platforms
+    - missing test dependency on OracleLinux 8.x
+    - MacOS test tool errors
+    - skip useless 'unknown' message, typo
+    - more useful codec loader validation message
+
+ -- Antoine Martin <antoine@nagafix.co.uk>  Sun, 21 May 2023 22:05:04 +0700
+
 xpra (4.4.4-1) UNRELEASED; urgency=low
   * major fixes:
     - focus change failures, errors with OR windows
     - dpi validation failures
     - honour dpi when setting initial resolution
     - match the requested desktop size exactly
     - XI2 errors
```

### Comparing `xpra-4.4.4/packaging/debian/xpra/control` & `xpra-4.4.5/packaging/debian/xpra/control`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,16 @@
         ,python3-dnspython
 #for connections through proxies
         ,python3-socks
 #the start-session GUI:
         ,python3-xdg
         ,python3-pyinotify
 #hope that this will allow our status icon to be shown:
-        ,gir1.2-appindicator3-0.1 | gir1.2-ayatanaappindicator3
+        ,gir1.2-appindicator3-0.1
+        ,gir1.2-ayatanaappindicator3-0.1
 #to be able to resize large svg icons:
         ,gir1.2-rsvg-2.0
 # we use dbus for many things - this provides "dbus-launch":
         ,dbus-x11
 # preferred input method:
         ,ibus
 # AES encryption:
```

### Comparing `xpra-4.4.4/packaging/debian/xpra/copyright` & `xpra-4.4.5/packaging/debian/xpra/copyright`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/debian/xpra/patches/pam.patch` & `xpra-4.4.5/packaging/debian/xpra/patches/pam.patch`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/debian/xpra/rules` & `xpra-4.4.5/packaging/debian/xpra/rules`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/debian/xpra/xpra.install` & `xpra-4.4.5/packaging/debian/xpra/xpra.install`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/debian/xpra/xpra.postinst` & `xpra-4.4.5/packaging/debian/xpra/xpra.postinst`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/debian/xpra/xpra.service` & `xpra-4.4.5/packaging/debian/xpra/xpra.service`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/debian/xpra.sh` & `xpra-4.4.5/packaging/debian/xpra.sh`

 * *Files 1% similar despite different names*

```diff
@@ -53,10 +53,10 @@
 else
 	if [ `arch` == "aarch64" ]; then
 		debuild --no-lintian -us -uc -b
 	else
 		debuild -us -uc -b
 	fi
 	ls -la ../xpra*deb
-	mv ../python*xpra*deb ../xpra*deb ../python*xpra*changes ../xpra*changes "$REPO_ARCH_PATH"
+	cp ../python*xpra*deb ../xpra*deb ../python*xpra*changes ../xpra*changes "$REPO_ARCH_PATH"
 fi
 popd
```

### Comparing `xpra-4.4.4/packaging/debian/xserver-xorg-video-dummy/changelog` & `xpra-4.4.5/packaging/debian/xserver-xorg-video-dummy/changelog`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/debian/xserver-xorg-video-dummy/control` & `xpra-4.4.5/packaging/debian/xserver-xorg-video-dummy/control`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/debian/xserver-xorg-video-dummy/copyright` & `xpra-4.4.5/packaging/debian/xserver-xorg-video-dummy/copyright`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/debian/xserver-xorg-video-dummy/patches/0002-Constant-DPI.patch` & `xpra-4.4.5/packaging/debian/xserver-xorg-video-dummy/patches/0002-Constant-DPI.patch`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/debian/xserver-xorg-video-dummy/patches/0006-Dummy-Disconnect.patch` & `xpra-4.4.5/packaging/debian/xserver-xorg-video-dummy/patches/0006-Dummy-Disconnect.patch`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/debian/xserver-xorg-video-dummy.sh` & `xpra-4.4.5/packaging/debian/xserver-xorg-video-dummy.sh`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/ffmpeg-xpra.spec` & `xpra-4.4.5/packaging/rpm/ffmpeg-xpra.spec`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/gstreamer1-plugin-timestamp.spec` & `xpra-4.4.5/packaging/rpm/gstreamer1-plugin-timestamp.spec`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/libfakeXinerama.spec` & `xpra-4.4.5/packaging/rpm/libfakeXinerama.spec`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/libyuv.spec` & `xpra-4.4.5/packaging/rpm/libyuv.spec`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/nasm.spec` & `xpra-4.4.5/packaging/rpm/nasm.spec`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/patches/0002-Constant-DPI.patch` & `xpra-4.4.5/packaging/rpm/patches/0002-Constant-DPI.patch`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/patches/0006-Dummy-Disconnect.patch` & `xpra-4.4.5/packaging/rpm/patches/0006-Dummy-Disconnect.patch`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/patches/libyuv-0001-Use-a-proper-so-version.patch` & `xpra-4.4.5/packaging/rpm/patches/libyuv-0001-Use-a-proper-so-version.patch`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/patches/libyuv-0002-Link-against-shared-library.patch` & `xpra-4.4.5/packaging/rpm/patches/libyuv-0002-Link-against-shared-library.patch`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/patches/libyuv-0003-Disable-static-library.patch` & `xpra-4.4.5/packaging/rpm/patches/libyuv-0003-Disable-static-library.patch`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/patches/libyuv-0004-Don-t-install-conversion-tool.patch` & `xpra-4.4.5/packaging/rpm/patches/libyuv-0004-Don-t-install-conversion-tool.patch`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/patches/libyuv-0005-Use-library-suffix-during-installation.patch` & `xpra-4.4.5/packaging/rpm/patches/libyuv-0005-Use-library-suffix-during-installation.patch`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/patches/libyuv-0006-Link-main-library-against-libjpeg.patch` & `xpra-4.4.5/packaging/rpm/patches/libyuv-0006-Link-main-library-against-libjpeg.patch`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/patches/libyuv-0007-nojpeg.patch` & `xpra-4.4.5/packaging/rpm/patches/libyuv-0007-nojpeg.patch`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/patches/nasm-SourceSans-font-name.patch` & `xpra-4.4.5/packaging/rpm/patches/nasm-SourceSans-font-name.patch`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/patches/python-rencode-readdmissingpyx.patch` & `xpra-4.4.5/packaging/rpm/patches/python-rencode-readdmissingpyx.patch`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/patches/python-rencode-typecode-dos.patch` & `xpra-4.4.5/packaging/rpm/patches/python-rencode-typecode-dos.patch`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/python3-Cython.spec` & `xpra-4.4.5/packaging/rpm/python3-Cython.spec`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 %prep
 sha256=`sha256sum %{SOURCE0} | awk '{print $1}'`
 if [ "${sha256}" != "e4672491fb31546b9abb63677f638e738085dc9321398170956ef6fbfc0e1726" ]; then
 	echo "invalid checksum for %{SOURCE0}"
 	exit 1
 fi
 %setup -q -n Cython-%{version}
-find -name '*.py' | xargs sed -i '1s|^#!python|#!%{__python2}|'
 
 %build
 CFLAGS="$RPM_OPT_FLAGS" %{__python3} setup.py build
 
 %install
 rm -rf %{buildroot}
 %{__python3} setup.py install -O1 --skip-build --root %{buildroot}
```

### Comparing `xpra-4.4.4/packaging/rpm/python3-cairo.spec` & `xpra-4.4.5/packaging/rpm/python3-cairo.spec`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 %define _disable_source_fetch 0
 
 Name: pycairo
 Version: 1.20.0
-Release: 4%{?dist}
+Release: 4.1%{?dist}
 Summary: Python bindings for the cairo library
 
 License: MPLv1.1 or LGPLv2
 URL: http://cairographics.org/pycairo
 Source0: https://github.com/pygobject/pycairo/releases/download/v%{version}/pycairo-%{version}.tar.gz
 
 BuildRequires: cairo-devel
 BuildRequires: gcc
 BuildRequires: pkgconfig
 BuildRequires: python3-devel
+%if !0%{?ol8}
 BuildRequires: python3-pytest
+%endif
 BuildRequires: python3-setuptools
 
 %description
 Python bindings for the cairo library.
 
 %package -n python3-cairo
 Summary: Python 3 bindings for the cairo library
@@ -46,27 +48,32 @@
 %build
 %py3_build
 
 %install
 %py3_install
 
 %check
+%if !0%{?ol8}
 %{__python3} setup.py test
+%endif
 
 %files -n python3-cairo
 %license COPYING*
 %{python3_sitearch}/cairo/
 %{python3_sitearch}/pycairo*.egg-info
 
 %files -n python3-cairo-devel
 %dir %{_includedir}/pycairo
 %{_includedir}/pycairo/py3cairo.h
 %{_libdir}/pkgconfig/py3cairo.pc
 
 %changelog
+* Sun Mar 19 2023 Antoine Martin <antoine@xpra.org> - 1.20.0-4.1
+- don't run tests on OracleLinux 8
+
 * Tue Aug 10 2021 Mohan Boddu <mboddu@redhat.com> - 1.20.0-4
 - Rebuilt for IMA sigs, glibc 2.34, aarch64 flags
   Related: rhbz#1991688
 
 * Fri Apr 16 2021 Mohan Boddu <mboddu@redhat.com> - 1.20.0-3
 - Rebuilt for RHEL 9 BETA on Apr 15th 2021. Related: rhbz#1947937
```

### Comparing `xpra-4.4.4/packaging/rpm/python3-lz4.spec` & `xpra-4.4.5/packaging/rpm/python3-lz4.spec`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/python3-pbr.spec` & `xpra-4.4.5/packaging/rpm/python3-pbr.spec`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/python3-pkgconfig.spec` & `xpra-4.4.5/packaging/rpm/python3-pkgconfig.spec`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/python3-pycuda.spec` & `xpra-4.4.5/packaging/rpm/python3-pycuda.spec`

 * *Files 7% similar despite different names*

```diff
@@ -12,21 +12,29 @@
 
 %define STUBS_DIR targets/x86_64-linux/lib/stubs/
 %ifarch aarch64
 %define STUBS_DIR targets/sbsa-linux/lib/stubs/
 %endif
 
 Name:           python3-pycuda
-Version:        2022.2
+%if !0%{?el8}
+Version:        2022.2.2
+%else
+Version:        2022.1
+%endif
 Release:        1
 URL:            http://mathema.tician.de/software/pycuda
 Summary:        Python3 wrapper CUDA
 License:        MIT
 Group:          Development/Libraries/Python
-Source0:        https://files.pythonhosted.org/packages/fa/5d/b91e8d6a8485f0a80746ac597757d39642bda78654f382d8b14147d3d7df/pycuda-%{version}.tar.gz
+%if !0%{?el8}
+Source0:        https://files.pythonhosted.org/packages/78/09/9df5358ffb74d225243b56a65ffe196de481fcd8f731f55e41f2d5d36015/pycuda-%{version}.tar.gz
+%else
+Source0:        https://files.pythonhosted.org/packages/2d/1f/48a3a5b2c715345e7af1e09361100bd98c3d72b4025371692ab233f523d3/pycuda-%{version}.tar.gz
+%endif
 BuildRoot:      %{_tmppath}/%{name}-%{version}-build
 Provides:       python3-pycuda
 
 BuildRequires:  make
 BuildRequires:  gcc-c++
 BuildRequires:  python3-devel
 BuildRequires:  python3-setuptools
@@ -43,15 +51,19 @@
 Requires:       python3-pytools
 Requires:       python3-six
 
 Suggests:       nvidia-driver-cuda-libs
 
 %prep
 sha256=`sha256sum %{SOURCE0} | awk '{print $1}'`
-if [ "${sha256}" != "da38f5325afea52f7e076954181983d0830057dd0f681de1ba68970929e75bb8" ]; then
+%if !0%{?el8}
+if [ "${sha256}" != "cd92e7246bb45ac3452955a110714112674cdf3b4a9e2f4ff25a4159c684e6bb" ]; then
+%else
+if [ "${sha256}" != "acd9030d93e76e60b122e33ad16bcf01bb1344f4c304dedff1cd2bffb0f313a3" ]; then
+%endif
 	echo "invalid checksum for %{SOURCE0}"
 	exit 1
 fi
 %setup -q -n pycuda-%{version}
 
 %build
 CUDA=/opt/cuda
@@ -76,18 +88,25 @@
 
 %files
 %defattr(-,root,root)
 %doc examples/ test/
 %{python3_sitearch}/pycuda*
 
 %changelog
+%if !0%{?el8}
+* Wed Dec 21 2022 Antoine Martin <antoine@xpra.org> - 2022.2.2-1
+- new upstream release
+
+* Wed Dec 21 2022 Antoine Martin <antoine@xpra.org> - 2022.2.1-1
+- new upstream release
+
 * Tue Nov 22 2022 Antoine Martin <antoine@xpra.org> - 2022.2-1
 - new upstream release
 - remove context cleanup failures patch (merged)
-
+%endif
 * Tue Aug 16 2022 Antoine Martin <antoine@xpra.org> - 2022.1-2
 - add patch to show context cleanup failures
 
 * Sat Jun 25 2022 Antoine Martin <antoine@xpra.org> - 2022.1-1
 - new upstream release
 
 * Sun May 02 2021 Antoine Martin <antoine@xpra.org> - 2021.1-1
```

### Comparing `xpra-4.4.4/packaging/rpm/python3-pynvml.spec` & `xpra-4.4.5/packaging/rpm/python3-pynvml.spec`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/python3-pyopengl.spec` & `xpra-4.4.5/packaging/rpm/python3-pyopengl.spec`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/python3-pytools.spec` & `xpra-4.4.5/packaging/rpm/python3-pytools.spec`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/python3-pyu2f.spec` & `xpra-4.4.5/packaging/rpm/python3-pyu2f.spec`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/python3-rencode.spec` & `xpra-4.4.5/packaging/rpm/python3-rencode.spec`

 * *Files 3% similar despite different names*

```diff
@@ -27,18 +27,18 @@
 %prep
 sha256=`sha256sum %{SOURCE0} | awk '{print $1}'`
 if [ "${sha256}" != "0ed61111f053ea37511da86ca7aed2a3cfda6bdaa1f54a237c4b86eea52f0733" ]; then
 	echo "invalid checksum for %{SOURCE0}"
 	exit 1
 fi
 %setup -qn rencode-%{version}
-%patch0 -p1
-%patch1 -p1
-%patch2 -p1
-%patch3 -p1
+%patch -P 0 -p1
+%patch -P 1 -p1
+%patch -P 2 -p1
+%patch -P 3 -p1
 
 %build
 CFLAGS="%{optflags}" %{__python3} setup.py build
 
 %install
 %{__python3} setup.py install --skip-build --root %{buildroot}
 #fix permissions on shared objects
```

### Comparing `xpra-4.4.4/packaging/rpm/python3-uinput.spec` & `xpra-4.4.5/packaging/rpm/python3-uinput.spec`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/x264-xpra.spec` & `xpra-4.4.5/packaging/rpm/x264-xpra.spec`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/packaging/rpm/xorg-x11-drv-dummy.spec` & `xpra-4.4.5/packaging/rpm/xorg-x11-drv-dummy.spec`

 * *Files 7% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 %{!?make_build: %global make_build make}
 
 %define _disable_source_fetch 0
 %undefine _hardened_build
 
 Summary:   Xorg X11 dummy video driver
 Name:      xorg-x11-drv-dummy
-Version:   0.4.0
+Version:   0.4.1
 
-Release:   3.xpra1%{?dist}
+Release:   1.xpra1%{?dist}
 URL:       http://www.x.org
 License:   MIT
 Group:     User Interface/X Hardware Support
 
 Source0:   https://xorg.freedesktop.org/archive/individual/driver/%{tarball}-%{version}.tar.xz
 Patch2:    0002-Constant-DPI.patch
 Patch6:    0006-Dummy-Disconnect.patch
@@ -29,21 +29,21 @@
 Requires: Xorg %(xserver-sdk-abi-requires videodrv)
 
 %description
 X.Org X11 dummy video driver.
 
 %prep
 sha256=`sha256sum %{SOURCE0} | awk '{print $1}'`
-if [ "${sha256}" != "e78ceae5c8c0588c7cb658f2afc3a9fac9ef665b52a75b01f8e9c5449a4e1e5a" ]; then
+if [ "${sha256}" != "351920a7fd0f759a3ac972a5999b3ffed46f07fb52a99f319bfb5b6a59d3dfaf" ]; then
 	echo "invalid checksum for %{SOURCE0}"
 	exit 1
 fi
 %setup -q -n %{tarball}-%{version}
-%patch2 -p1
-%patch6 -p1
+%patch -P 2 -p1
+%patch -P 6 -p1
 autoreconf -vif
 
 %build
 %configure --disable-static
 %make_build
 
 %install
@@ -55,14 +55,17 @@
 # should be fixed in upstream Makefile.am or whatever.
 find $RPM_BUILD_ROOT -regex ".*\.la$" | xargs rm -f --
 
 %files
 %{driverdir}/dummy_drv.so
 
 %changelog
+* Mon May 08 2023 Antoine Martin <antoine@xpra.org> - 0.4.1-1.xpra1
+- new upstream release
+
 * Fri Apr 15 2022 Antoine Martin <antoine@xpra.org> - 0.4.0-3.xpra1
 - add disconnect patch
 
 * Sun Apr 10 2022 Antoine Martin <antoine@xpra.org> - 0.4.0-2.xpra1
 - remove redundant pointer limits patch
 
 * Wed Apr 06 2022 Antoine Martin <antoine@xpra.org> - 0.4.0-1.xpra3
```

### Comparing `xpra-4.4.4/packaging/rpm/xpra.spec` & `xpra-4.4.5/packaging/rpm/xpra.spec`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file is part of Xpra.
 # Copyright (C) 2010-2021 Antoine Martin <antoine@xpra.org>
 # Xpra is released under the terms of the GNU GPL v2, or, at your option, any
 # later version. See the file COPYING for details.
 
 %define _disable_source_fetch 0
-%define version 4.4.4
+%define version 4.4.5
 
 %define CFLAGS -O2
 %define DEFAULT_BUILD_ARGS --with-Xdummy --without-enc_x265	--pkg-config-path=%{_libdir}/xpra/pkgconfig --rpath=%{_libdir}/xpra --without-cuda_rebuild
 
 %{!?nthreads: %global nthreads %(nproc)}
 %{!?update_firewall: %define update_firewall 1}
 %{!?run_tests: %define run_tests 0}
@@ -20,18 +20,14 @@
 %define with_cuda 0
 %endif
 %if 0%{?with_cuda}
 %define build_args %{DEFAULT_BUILD_ARGS}
 %else
 %define build_args %{DEFAULT_BUILD_ARGS} --without-cuda_kernels --without-nvenc --without-nvfbc --without-nvjpeg_encoder  --without-nvjpeg_decoder
 %endif
-%if 0%{?el9}
-#no pandoc!
-%define build_args %{DEFAULT_BUILD_ARGS} --without-docs
-%endif
 %global selinux_variants mls targeted
 %define selinux_modules cups_xpra xpra_socketactivation
 #we never want to depend on proprietary nvidia bits,
 #and we manage the codecs with a private library:
 %global __requires_exclude ^(libnvjpeg|libnvidia-|libavcodec|libavformat|libavutil|libswscale|libx264).*\\.so.*$
 
 # no support for centos / rhel 7:
@@ -78,17 +74,15 @@
 
 %package common
 Summary:			Common files for xpra packages
 Group:				Networking
 BuildArch:			noarch
 Requires(pre):		shadow-utils
 Conflicts:			xpra < 2.1
-%if !0%{?el9}
 BuildRequires:		pandoc
-%endif
 BuildRequires:		libfakeXinerama
 %description common
 This package contains the files which are shared between all the xpra packages.
 
 %package common-client
 Summary:			Common files for xpra client packages
 Group:				Networking
@@ -200,14 +194,15 @@
 BuildRequires:		which
 BuildRequires:		libwebp-devel
 BuildRequires:		turbojpeg-devel
 BuildRequires:		libyuv-devel
 BuildRequires:		coreutils
 BuildRequires:		gcc
 BuildRequires:		gcc-c++
+BuildRequires:		pkgconfig
 BuildRequires:		python3
 BuildRequires:		python3-devel
 BuildRequires:		python3-Cython
 BuildRequires:		python3-gobject
 BuildRequires:		pygobject3-devel
 BuildRequires:		python3-cairo-devel
 BuildRequires:		libvpx-devel
@@ -398,17 +393,15 @@
 %{_datadir}/xpra/README.md
 %{_datadir}/xpra/COPYING
 %{_datadir}/xpra/icons
 %{_datadir}/xpra/*.wav
 %{_datadir}/xpra/cuda
 %{_datadir}/man/man1/xpra*.1*
 %{_datadir}/man/man1/run_scaled.1*
-%if !0%{?el9}
 %{_docdir}/xpra
-%endif
 %{_datadir}/metainfo/xpra.appdata.xml
 %{_datadir}/icons/xpra.png
 %{_datadir}/icons/xpra-mdns.png
 %{_datadir}/icons/xpra-shadow.png
 %dir %{_sysconfdir}/xpra
 %config %{_sysconfdir}/xpra/xpra.conf
 %config %{_sysconfdir}/xpra/conf.d/05_features.conf
@@ -634,14 +627,90 @@
 fi
 
 %posttrans common
 /usr/bin/gtk-update-icon-cache %{_datadir}/icons/hicolor &>/dev/null || :
 
 
 %changelog
+* Sun May 21 2023 Antoine Martin <antoine@xpra.org> 4.4.5-10
+- major fixes:
+   use after free crash in GTK
+   ensure X11 errors don't propagate to GTK
+   windows losing focus
+   fix legacy URL format parsing
+   brolti errors on some platforms
+   keyboard shortcuts with Wayland clients and NumLock
+   client sockets overwriting server sockets
+   network queue flushing
+   correct check for disabled monitors
+   stop as soon as we find a valid mDNS backend
+   only allow logging tweaks via env vars for non-root users
+- packaging:
+   dummy driver RPM version 0.4.1
+   modules not excluded due to typo
+   avoid permissions issues with mv
+   remove legacy MacOS bundler workaround
+   support MacOS arm64 builds
+   fail early with a more useful message on MacOS
+   setuptools packaging workarounds on MacOS
+   don't ship .cpp source files in MacOS app
+   compilation errors with gcc version 7 and older
+   RHEL 8.x needs pycuda 2022.1 or older
+   RHEL 9.x can install pandoc from EPEL
+   silence python cryptography OpenSSL warning on MacOS
+   workaround even more exotic library version strings
+   try harder to find a working appindicator DEB package
+   better compatibility with newer versions of Cython
+   we never want a python2 shebang
+   evdi file missing from MANIFEST
+   missing explicit dependency on `pkgconfig` in RPM spec file
+   skip xsettings dpi when the x11 bindings are missing
+   ignore setuptools generated cruft
+   silence rencode RPM patch warnings
+   missing GStreamer elements for playing 'bell' on MS Windows
+- encodings:
+   always use lossless encoding for `text`
+   continue to monitor window metadata updates
+   honour png palette encodings
+   option parsing
+   help command error
+   handle `RGBA` window icon data
+   `ffmpeg` encoder error values
+   validate NvFBC Sys capture before enabling it on MS Windows
+- minor:
+   X11 Atom name memory leak
+   handle malformed display names more gracefully
+   if we don't have keycodes to map, don't try to translate them
+   skip negative keyboard codes as per MS Windows specifications
+   fix side buttons on MS Windows
+   X11 clipboard debug logging parsing of window names
+   remove unused, potentially problematic statement
+   make it possible to disable `SHA1`
+   avoid errors if `MD5` has already been removed
+   don't try to show an exception that does not exist
+   window debug logging error
+   correctly parse OpenGL diagnostics
+   window forwarding require encoding module
+   mmap debug flood
+   continue with session info despite cursor errors
+   handle client server uuid errors more gracefully
+   silence shared socket permission warning
+   handle missing server attributes without erroring out
+   correct default method signature
+   missing latency data on websocket connections
+   service update errors with newer versions of python zeroconf
+   parse IPv6 when looking up network devices
+   run servers with missing stderr
+   correct server initialization order for cleaner shutdowns on errors
+   skip systemd-run tests on unsupported platforms
+   missing test dependency on OracleLinux 8.x
+   MacOS test tool errors
+   skip useless 'unknown' message, typo
+   more useful codec loader validation message
+
 * Thu Mar 09 2023 Antoine Martin <antoine@xpra.org> 4.4.4-10
 - major fixes:
    focus change failures, errors with OR windows
    dpi validation failures
    honour dpi when setting initial resolution
    match the requested desktop size exactly
    XI2 errors
```

### Comparing `xpra-4.4.4/setup.py` & `xpra-4.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 def pkg_config_ok(*args):
     return get_status_output([PKG_CONFIG] + [str(x) for x in args])[0]==0
 
 def pkg_config_version(req_version, pkgname):
     r, out, _ = get_status_output([PKG_CONFIG, "--modversion", pkgname])
     if r!=0 or not out:
         return False
-    out = out.rstrip("\n\r")
+    out = out.rstrip("\n\r").split(" ")[0]  #ie: "0.155.2917 0a84d98" -> "0.155.2917"
     #workaround for libx264 invalid version numbers:
     #ie: "0.163.x" or "0.164.3094M"
     while out[-1].isalpha() or out[-1]==".":
         out = out[:-1]
     try:
         from packaging.version import parse
         return parse(out)>=parse(req_version)
@@ -470,15 +470,15 @@
                     #PIL bits that import TK:
                     "PIL._tkinter_finder", "_imagingtk", "PIL._imagingtk", "ImageTk", "PIL.ImageTk", "FixTk",
                     #formats we don't use:
                     "GimpGradientFile", "GimpPaletteFile", "BmpImagePlugin", "TiffImagePlugin",
                     #not used:
                     "curses", "pdb",
                     "tty",
-                    "setuptools", "doctest"
+                    "setuptools", "doctest",
                     "nose", "pytest", "_pytest", "pluggy", "more_itertools", "apipkg", "py", "funcsigs",
                     "Cython", "cython", "pyximport",
                     "pydoc_data",
                     ]
 if not crypto_ENABLED:
     external_excludes += ["ssl", "_ssl"]
 if not client_ENABLED:
@@ -602,15 +602,15 @@
     if not src[0].endswith(".pyx"):
         src[0] = src[0].replace(".", "/")+".pyx"
     if isinstance(pkgconfig_names, str):
         pkgconfig_names = [x for x in pkgconfig_names.split(",") if x]
     pkgc = pkgconfig(*pkgconfig_names, optimize=optimize)
     for addto in ("extra_link_args", "extra_compile_args"):
         value = kwargs.pop(addto, None)
-        if value is not None:
+        if value:
             if isinstance(value, str):
                 value = (value, )
             add_to_keywords(pkgc, addto, *value)
     pkgc.update(kwargs)
     CPP = kwargs.get("language", "")=="c++"
     if CPP:
         #default to "-std=c++11" for c++
@@ -1408,14 +1408,16 @@
                            "gdp", "matroska", "ogg", "isomp4",
                            "audioparsers", "audiorate", "audioconvert", "audioresample", "audiotestsrc",
                            "coreelements", "directsound", "directsoundsrc", "wasapi",
                            #codecs:
                            "opus", "opusparse", "flac", "lame", "mpg123", "speex", "faac", "faad",
                            "volume", "vorbis", "wavenc", "wavpack", "wavparse",
                            "autodetect",
+                           #decodebin used for playing "new-client" sound:
+                           "playback", "typefindfunctions",
                            #no longer available: "mad"
                            #untested: a52dec, voaacenc
                            )
             add_dir(os.path.join("lib", "gstreamer-1.0"), [("libgst%s.dll" % x) for x in GST_PLUGINS])
             #END OF SOUND
 
         if server_ENABLED:
@@ -2152,14 +2154,15 @@
         assert nvcc, "cannot find nvcc compiler!"
         def get_nvcc_args():
             nvcc_cmd = [nvcc, "-fatbin"]
             gcc_version = get_gcc_version()
             if gcc_version<(7, 5):
                 print("gcc versions older than 7.5 are not supported!")
                 for _ in range(5):
+                    from time import sleep
                     sleep(1)
                     print(".")
             if (8,1)<=gcc_version<(9, ):
                 #GCC 8.1 has compatibility issues with CUDA 9.2,
                 #so revert to C++03:
                 nvcc_cmd.append("-std=c++03")
             #GCC 6 uses C++11 by default:
@@ -2247,15 +2250,16 @@
         #if pycuda is built with curand, add this:
         #add_data_files("", glob.glob(f"{CUDA_BIN_DIR}/curand64*dll"))
         if nvjpeg_encoder_ENABLED or nvjpeg_decoder_ENABLED:
             add_data_files("", glob.glob(f"{CUDA_BIN_DIR}/nvjpeg64*dll"))
 
 add_data_files(CUDA_BIN, ["fs/share/xpra/cuda/README.md"])
 
-tace(nvenc_ENABLED, "xpra.codecs.nvenc.encoder", "nvenc")
+tace(nvenc_ENABLED, "xpra.codecs.nvenc.encoder", "nvenc",
+     extra_compile_args="-Wno-error=sign-compare" if get_gcc_version()<(8, ) else None)
 
 toggle_packages(argb_ENABLED, "xpra.codecs.argb")
 tace(argb_ENABLED, "xpra.codecs.argb.argb", optimize=3)
 toggle_packages(evdi_ENABLED, "xpra.codecs.evdi")
 
 tace(evdi_ENABLED, "xpra.codecs.evdi.capture", "evdi", language="c++")
 toggle_packages(drm_ENABLED, "xpra.codecs.drm")
```

### Comparing `xpra-4.4.4/tests/perf/perf_config_default.py` & `xpra-4.4.5/tests/perf/perf_config_default.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/perf/test_measure_perf.py` & `xpra-4.4.5/tests/perf/test_measure_perf.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/perf/test_measure_perf_chartreps.py` & `xpra-4.4.5/tests/perf/test_measure_perf_chartreps.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/perf/test_measure_perf_charts.py` & `xpra-4.4.5/tests/perf/test_measure_perf_charts.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/scripts/pycallgraph` & `xpra-4.4.5/tests/scripts/pycallgraph`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/run` & `xpra-4.4.5/tests/unittests/run`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/buffers/cyxor_test.py` & `xpra-4.4.5/tests/unittests/unit/buffers/cyxor_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/child_reaper_test.py` & `xpra-4.4.5/tests/unittests/unit/child_reaper_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/client/auth_handlers_test.py` & `xpra-4.4.5/tests/unittests/unit/client/auth_handlers_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/client/border_test.py` & `xpra-4.4.5/tests/unittests/unit/client/border_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/client/keyboard_helper_test.py` & `xpra-4.4.5/tests/unittests/unit/client/keyboard_helper_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/client/mixins/audioclient_test.py` & `xpra-4.4.5/tests/unittests/unit/client/mixins/audioclient_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/client/mixins/clientmixintest_util.py` & `xpra-4.4.5/tests/unittests/unit/client/mixins/clientmixintest_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/client/mixins/clipboard_test.py` & `xpra-4.4.5/tests/unittests/unit/client/mixins/clipboard_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/client/mixins/display_test.py` & `xpra-4.4.5/tests/unittests/unit/client/mixins/display_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/client/mixins/encodings_test.py` & `xpra-4.4.5/tests/unittests/unit/client/mixins/encodings_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/client/mixins/mmap_test.py` & `xpra-4.4.5/tests/unittests/unit/client/mixins/mmap_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/client/mixins/networkstate_test.py` & `xpra-4.4.5/tests/unittests/unit/client/mixins/networkstate_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/client/mixins/notifications_test.py` & `xpra-4.4.5/tests/unittests/unit/client/mixins/notifications_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/client/mixins/remotelogging_test.py` & `xpra-4.4.5/tests/unittests/unit/client/mixins/remotelogging_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/client/mixins/serverinfo_test.py` & `xpra-4.4.5/tests/unittests/unit/client/mixins/serverinfo_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/client/mixins/stubclient_test.py` & `xpra-4.4.5/tests/unittests/unit/client/mixins/stubclient_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/client/mixins/tray_test.py` & `xpra-4.4.5/tests/unittests/unit/client/mixins/tray_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/client/mixins/webcam_test.py` & `xpra-4.4.5/tests/unittests/unit/client/mixins/webcam_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/client/mixins/window_test.py` & `xpra-4.4.5/tests/unittests/unit/client/mixins/window_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/client/osxlike_clipboard_test.py` & `xpra-4.4.5/tests/unittests/unit/client/osxlike_clipboard_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/client/paint_colors_test.py` & `xpra-4.4.5/tests/unittests/unit/client/paint_colors_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/client/splash_test.py` & `xpra-4.4.5/tests/unittests/unit/client/splash_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/client/x11_client_test.py` & `xpra-4.4.5/tests/unittests/unit/client/x11_client_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/client/x11_client_test_util.py` & `xpra-4.4.5/tests/unittests/unit/client/x11_client_test_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/client/x11_clipboard_test.py` & `xpra-4.4.5/tests/unittests/unit/client/x11_clipboard_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/client/x11_clipboard_test_util.py` & `xpra-4.4.5/tests/unittests/unit/client/x11_clipboard_test_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/codecs/argb_test.py` & `xpra-4.4.5/tests/unittests/unit/codecs/argb_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/codecs/codecs_selftest_test.py` & `xpra-4.4.5/tests/unittests/unit/codecs/codecs_selftest_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/codecs/csc_colorspace_test.py` & `xpra-4.4.5/tests/unittests/unit/codecs/csc_colorspace_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/codecs/image_wrapper_test.py` & `xpra-4.4.5/tests/unittests/unit/codecs/image_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/codecs/nvutil_test.py` & `xpra-4.4.5/tests/unittests/unit/codecs/nvutil_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/codecs/pillow_encoder_test.py` & `xpra-4.4.5/tests/unittests/unit/codecs/pillow_encoder_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/codecs/pillow_header_test.py` & `xpra-4.4.5/tests/unittests/unit/codecs/pillow_header_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/codecs/rgb_transform_test.py` & `xpra-4.4.5/tests/unittests/unit/codecs/rgb_transform_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/codecs/video_colorspace_test.py` & `xpra-4.4.5/tests/unittests/unit/codecs/video_colorspace_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/dbus/dbus_helper_test.py` & `xpra-4.4.5/tests/unittests/unit/dbus/dbus_helper_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/gtk_common/keymap_test.py` & `xpra-4.4.5/tests/unittests/unit/gtk_common/keymap_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/keyboard_layout_test.py` & `xpra-4.4.5/tests/unittests/unit/keyboard_layout_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/net/HMAC_test.py` & `xpra-4.4.5/tests/unittests/unit/net/HMAC_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/net/bencode_test.py` & `xpra-4.4.5/tests/unittests/unit/net/bencode_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/net/brotli_test.py` & `xpra-4.4.5/tests/unittests/unit/net/brotli_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/net/common_test.py` & `xpra-4.4.5/tests/unittests/unit/net/common_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/net/compression_test.py` & `xpra-4.4.5/tests/unittests/unit/net/compression_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/net/crypto_test.py` & `xpra-4.4.5/tests/unittests/unit/net/crypto_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/net/d3des_test.py` & `xpra-4.4.5/tests/unittests/unit/net/d3des_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/net/digest_test.py` & `xpra-4.4.5/tests/unittests/unit/net/digest_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/net/file_transfer_test.py` & `xpra-4.4.5/tests/unittests/unit/net/file_transfer_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/net/lz4_test.py` & `xpra-4.4.5/tests/unittests/unit/net/lz4_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/net/net_util_test.py` & `xpra-4.4.5/tests/unittests/unit/net/net_util_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/net/packet_encoding_test.py` & `xpra-4.4.5/tests/unittests/unit/net/packet_encoding_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/net/packet_header_test.py` & `xpra-4.4.5/tests/unittests/unit/net/packet_header_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/net/protocol_test.py` & `xpra-4.4.5/tests/unittests/unit/net/protocol_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/net/rfb/rfb_test.py` & `xpra-4.4.5/tests/unittests/unit/net/rfb/rfb_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/net/ssh_test.py` & `xpra-4.4.5/tests/unittests/unit/net/ssh_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/net/subprocess_wrapper_test.py` & `xpra-4.4.5/tests/unittests/unit/net/subprocess_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/net/websocket_header_test.py` & `xpra-4.4.5/tests/unittests/unit/net/websocket_header_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/net/websocket_response_headers_test.py` & `xpra-4.4.5/tests/unittests/unit/net/websocket_response_headers_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/notifications/common_test.py` & `xpra-4.4.5/tests/unittests/unit/notifications/common_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/os_util_test.py` & `xpra-4.4.5/tests/unittests/unit/os_util_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/platformtests/displayfd_test.py` & `xpra-4.4.5/tests/unittests/unit/platformtests/displayfd_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/platformtests/features_test.py` & `xpra-4.4.5/tests/unittests/unit/platformtests/features_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/platformtests/info_test.py` & `xpra-4.4.5/tests/unittests/unit/platformtests/info_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/platformtests/init_test.py` & `xpra-4.4.5/tests/unittests/unit/platformtests/init_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/platformtests/mainmodule_test.py` & `xpra-4.4.5/tests/unittests/unit/platformtests/mainmodule_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/process_test_util.py` & `xpra-4.4.5/tests/unittests/unit/process_test_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/queue_scheduler_test.py` & `xpra-4.4.5/tests/unittests/unit/queue_scheduler_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/rectangle_test.py` & `xpra-4.4.5/tests/unittests/unit/rectangle_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/run.py` & `xpra-4.4.5/tests/unittests/unit/run.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/scripts/main_test.py` & `xpra-4.4.5/tests/unittests/unit/scripts/main_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # This file is part of Xpra.
-# Copyright (C) 2020-2021 Antoine Martin <antoine@xpra.org>
+# Copyright (C) 2020-2023 Antoine Martin <antoine@xpra.org>
 # Xpra is released under the terms of the GNU GPL v2, or, at your option, any
 # later version. See the file COPYING for details.
 
 import os
 import shlex
 import signal
 import tempfile
 import unittest
 from subprocess import Popen, DEVNULL, PIPE
 
-from xpra.os_util import OSEnvContext, pollwait, POSIX, OSX
+from xpra.os_util import OSEnvContext, pollwait, getuid, POSIX, OSX
 from xpra.util import AdHocStruct
 from xpra.platform.paths import get_xpra_command
 from xpra.common import noop
 from xpra.scripts.main import (
     nox, noerr,
     use_systemd_run, systemd_run_command, systemd_run_wrap,
     isdisplaytype,
@@ -38,19 +38,24 @@
             assert os.environ.get("DISPLAY") is None
 
     def test_systemd_run(self):
         for s in ("yes", "no", "auto"):
             if not use_systemd_run(s):
                 continue
             for user in (True, False):
-                for systemd_run_args in ("", "-d"):
+                for systemd_run_args in (None, "-d"):
                     assert systemd_run_command("mode", systemd_run_args, user=user)[0]=="systemd-run"
-            with OSEnvContext():
-                os.environ["XPRA_LOG_SYSTEMD_WRAP"] = "0"
-                assert systemd_run_wrap("unused", ["xpra", "--version"], stdout=DEVNULL, stderr=DEVNULL)==0
+        if not use_systemd_run("auto"):
+            return
+        with OSEnvContext():
+            os.environ["XPRA_LOG_SYSTEMD_WRAP"] = "0"
+            os.environ["XPRA_LOG_SYSTEMD_WRAP_COMMAND"] = "0"
+            r = systemd_run_wrap("unused", ["xpra", "--version"], user=getuid()!=0, stdout=DEVNULL, stderr=DEVNULL)
+            if r:
+                raise ValueError(f"expected return code 0 but got {r}")
 
     def test_display_type_check(self):
         for arg in ("ssh:host", "ssh/host", "tcp:IP", "ssl/host", "vsock:port"):
             args = [arg]
             assert isdisplaytype(args, "ssh", "tcp", "ssl", "vsock")
 
     def test_check_display(self):
```

### Comparing `xpra-4.4.4/tests/unittests/unit/scripts/parse_display_name_test.py` & `xpra-4.4.5/tests/unittests/unit/scripts/parse_display_name_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/scripts/parsing_test.py` & `xpra-4.4.5/tests/unittests/unit/scripts/parsing_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/auth_test.py` & `xpra-4.4.5/tests/unittests/unit/server/auth_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/background_worker_test.py` & `xpra-4.4.5/tests/unittests/unit/server/background_worker_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/cystats_test.py` & `xpra-4.4.5/tests/unittests/unit/server/cystats_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/dbus_test.py` & `xpra-4.4.5/tests/unittests/unit/server/dbus_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/mixins/audio_test.py` & `xpra-4.4.5/tests/unittests/unit/server/mixins/audio_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/mixins/child_command_test.py` & `xpra-4.4.5/tests/unittests/unit/server/mixins/child_command_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/mixins/clipboard_test.py` & `xpra-4.4.5/tests/unittests/unit/server/mixins/clipboard_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/mixins/display_test.py` & `xpra-4.4.5/tests/unittests/unit/server/mixins/display_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/mixins/encoding_test.py` & `xpra-4.4.5/tests/unittests/unit/server/mixins/encoding_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/mixins/fileprint_test.py` & `xpra-4.4.5/tests/unittests/unit/server/mixins/fileprint_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/mixins/input_test.py` & `xpra-4.4.5/tests/unittests/unit/server/mixins/input_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/mixins/logging_test.py` & `xpra-4.4.5/tests/unittests/unit/server/mixins/logging_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/mixins/mmap_test.py` & `xpra-4.4.5/tests/unittests/unit/server/mixins/mmap_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/mixins/networkstate_test.py` & `xpra-4.4.5/tests/unittests/unit/server/mixins/networkstate_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/mixins/notification_test.py` & `xpra-4.4.5/tests/unittests/unit/server/mixins/notification_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/mixins/remotelogging_test.py` & `xpra-4.4.5/tests/unittests/unit/server/mixins/remotelogging_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/mixins/server_mixins_option_test_util.py` & `xpra-4.4.5/tests/unittests/unit/server/mixins/server_mixins_option_test_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/mixins/servermixintest_util.py` & `xpra-4.4.5/tests/unittests/unit/server/mixins/servermixintest_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/mixins/shadow_option_test.py` & `xpra-4.4.5/tests/unittests/unit/server/mixins/shadow_option_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/mixins/start_option_test.py` & `xpra-4.4.5/tests/unittests/unit/server/mixins/start_option_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/mixins/startdesktop_option_test.py` & `xpra-4.4.5/tests/unittests/unit/server/mixins/startdesktop_option_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/mixins/stub_mixin_test.py` & `xpra-4.4.5/tests/unittests/unit/server/mixins/stub_mixin_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/mixins/webcam_test.py` & `xpra-4.4.5/tests/unittests/unit/server/mixins/webcam_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/mixins/window_test.py` & `xpra-4.4.5/tests/unittests/unit/server/mixins/window_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/motion_test.py` & `xpra-4.4.5/tests/unittests/unit/server/motion_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/proxy_server_test.py` & `xpra-4.4.5/tests/unittests/unit/server/proxy_server_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/server_auth_test.py` & `xpra-4.4.5/tests/unittests/unit/server/server_auth_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/server_sockets_test.py` & `xpra-4.4.5/tests/unittests/unit/server/server_sockets_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/shadow_server_test.py` & `xpra-4.4.5/tests/unittests/unit/server/shadow_server_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/source/source_mixins_test.py` & `xpra-4.4.5/tests/unittests/unit/server/source/source_mixins_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/video_scoring_test.py` & `xpra-4.4.5/tests/unittests/unit/server/video_scoring_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/video_subregion_test.py` & `xpra-4.4.5/tests/unittests/unit/server/video_subregion_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server/window/batch_config_test.py` & `xpra-4.4.5/tests/unittests/unit/server/window/batch_config_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/server_test_util.py` & `xpra-4.4.5/tests/unittests/unit/server_test_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/simple_stats_test.py` & `xpra-4.4.5/tests/unittests/unit/simple_stats_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/sound/common_test.py` & `xpra-4.4.5/tests/unittests/unit/sound/common_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/test_util.py` & `xpra-4.4.5/tests/unittests/unit/test_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/util_test.py` & `xpra-4.4.5/tests/unittests/unit/util_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/version_util_test.py` & `xpra-4.4.5/tests/unittests/unit/version_util_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/x11/common_test.py` & `xpra-4.4.5/tests/unittests/unit/x11/common_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/x11/display_util_test.py` & `xpra-4.4.5/tests/unittests/unit/x11/display_util_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/x11/fakexinerama_test.py` & `xpra-4.4.5/tests/unittests/unit/x11/fakexinerama_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/x11/keyboard_test.py` & `xpra-4.4.5/tests/unittests/unit/x11/keyboard_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/x11/size_hints_util_test.py` & `xpra-4.4.5/tests/unittests/unit/x11/size_hints_util_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/x11/x11_server_test.py` & `xpra-4.4.5/tests/unittests/unit/x11/x11_server_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/unittests/unit/x11/xsettings_test.py` & `xpra-4.4.5/tests/unittests/unit/x11/xsettings_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/clients/fake_client.py` & `xpra-4.4.5/tests/xpra/clients/fake_client.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/clients/fake_gtk_client.py` & `xpra-4.4.5/tests/xpra/clients/fake_gtk_client.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/clients/test_DoS_client.py` & `xpra-4.4.5/tests/xpra/clients/test_DoS_client.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/codecs/benchmark.py` & `xpra-4.4.5/tests/xpra/codecs/benchmark.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/codecs/benchmark_bgra_to_rgb.py` & `xpra-4.4.5/tests/xpra/codecs/benchmark_bgra_to_rgb.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/codecs/benchmark_bgra_to_rgba.py` & `xpra-4.4.5/tests/xpra/codecs/benchmark_bgra_to_rgba.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/codecs/benchmark_bgrx_to_rgb.py` & `xpra-4.4.5/tests/xpra/codecs/benchmark_bgrx_to_rgb.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/codecs/benchmark_picture_encoders.py` & `xpra-4.4.5/tests/xpra/codecs/benchmark_picture_encoders.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/codecs/evdi_glib.py` & `xpra-4.4.5/tests/xpra/codecs/evdi_glib.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/codecs/evdi_test.py` & `xpra-4.4.5/tests/xpra/codecs/evdi_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/keyboard/test_get_keycode_mappings.py` & `xpra-4.4.5/tests/xpra/keyboard/test_get_keycode_mappings.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/keyboard/test_x11keycodes_down.py` & `xpra-4.4.5/tests/xpra/keyboard/test_x11keycodes_down.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/net/vsock_client_test.py` & `xpra-4.4.5/tests/xpra/net/vsock_client_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/net/vsock_server_test.py` & `xpra-4.4.5/tests/xpra/net/vsock_server_test.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/server/test_region.py` & `xpra-4.4.5/tests/xpra/server/test_region.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/dbus_video_region_detection.py` & `xpra-4.4.5/tests/xpra/test_apps/dbus_video_region_detection.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/dbus_video_region_enabled.py` & `xpra-4.4.5/tests/xpra/test_apps/dbus_video_region_enabled.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/dump_xshape.py` & `xpra-4.4.5/tests/xpra/test_apps/dump_xshape.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/fps.py` & `xpra-4.4.5/tests/xpra/test_apps/fps.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/screensaver_listener.py` & `xpra-4.4.5/tests/xpra/test_apps/screensaver_listener.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/send_dbus_video_exclusion_zone.py` & `xpra-4.4.5/tests/xpra/test_apps/send_dbus_video_exclusion_zone.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/simulate_console_typing.py` & `xpra-4.4.5/tests/xpra/test_apps/simulate_console_typing.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/simulate_console_user.py` & `xpra-4.4.5/tests/xpra/test_apps/simulate_console_user.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_command_change.py` & `xpra-4.4.5/tests/xpra/test_apps/test_command_change.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_copy_image_from_clipboard.py` & `xpra-4.4.5/tests/xpra/test_apps/test_copy_image_from_clipboard.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_copy_image_to_clipboard.py` & `xpra-4.4.5/tests/xpra/test_apps/test_copy_image_to_clipboard.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_cursor_pixbuf.py` & `xpra-4.4.5/tests/xpra/test_apps/test_cursor_pixbuf.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_custom_cursor.py` & `xpra-4.4.5/tests/xpra/test_apps/test_custom_cursor.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_drop_down.py` & `xpra-4.4.5/tests/xpra/test_apps/test_drop_down.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_fast_cursor.py` & `xpra-4.4.5/tests/xpra/test_apps/test_fast_cursor.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_form_input.py` & `xpra-4.4.5/tests/xpra/test_apps/test_form_input.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_frame_extents.py` & `xpra-4.4.5/tests/xpra/test_apps/test_frame_extents.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_gtk3_window.py` & `xpra-4.4.5/tests/xpra/test_apps/test_gtk3_window.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_hostname.py` & `xpra-4.4.5/tests/xpra/test_apps/test_hostname.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_modal_window.py` & `xpra-4.4.5/tests/xpra/test_apps/test_modal_window.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_notification.py` & `xpra-4.4.5/tests/xpra/test_apps/test_notification.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_right_click_menu.py` & `xpra-4.4.5/tests/xpra/test_apps/test_right_click_menu.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_show_desktop.py` & `xpra-4.4.5/tests/xpra/test_apps/test_show_desktop.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_system_tray.py` & `xpra-4.4.5/tests/xpra/test_apps/test_system_tray.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_window_bypass_compositor.py` & `xpra-4.4.5/tests/xpra/test_apps/test_window_bypass_compositor.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_window_content_type.py` & `xpra-4.4.5/tests/xpra/test_apps/test_window_content_type.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_window_eclipse_fixed_size.py` & `xpra-4.4.5/tests/xpra/test_apps/test_window_eclipse_fixed_size.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_window_icon_from_files.py` & `xpra-4.4.5/tests/xpra/test_apps/test_window_icon_from_files.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_window_initial_position.py` & `xpra-4.4.5/tests/xpra/test_apps/test_window_initial_position.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_window_maximize.py` & `xpra-4.4.5/tests/xpra/test_apps/test_window_maximize.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_window_maxsize_GTK3.py` & `xpra-4.4.5/tests/xpra/test_apps/test_window_maxsize_GTK3.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_window_move.py` & `xpra-4.4.5/tests/xpra/test_apps/test_window_move.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_window_moveresize.py` & `xpra-4.4.5/tests/xpra/test_apps/test_window_moveresize.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_window_quality_speed_hints.py` & `xpra-4.4.5/tests/xpra/test_apps/test_window_quality_speed_hints.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_window_raise.py` & `xpra-4.4.5/tests/xpra/test_apps/test_window_raise.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_window_resize.py` & `xpra-4.4.5/tests/xpra/test_apps/test_window_resize.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_window_title_fixed.py` & `xpra-4.4.5/tests/xpra/test_apps/test_window_title_fixed.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_window_withicon.py` & `xpra-4.4.5/tests/xpra/test_apps/test_window_withicon.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_window_xterm_size_hints.py` & `xpra-4.4.5/tests/xpra/test_apps/test_window_xterm_size_hints.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_windows_at.py` & `xpra-4.4.5/tests/xpra/test_apps/test_windows_at.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/test_apps/test_wmclass_change.py` & `xpra-4.4.5/tests/xpra/test_apps/test_wmclass_change.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/x11/print_atom.py` & `xpra-4.4.5/tests/xpra/x11/print_atom.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/x11/print_xpra_props.py` & `xpra-4.4.5/tests/xpra/x11/print_xpra_props.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/tests/xpra/x11/xres_get_pid.py` & `xpra-4.4.5/tests/xpra/x11/xres_get_pid.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/buffers/cyxor.pyx` & `xpra-4.4.5/xpra/buffers/cyxor.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/buffers/memalign.c` & `xpra-4.4.5/xpra/buffers/memalign.c`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/buffers/membuf.pxd` & `xpra-4.4.5/xpra/buffers/membuf.pxd`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/buffers/membuf.pyx` & `xpra-4.4.5/xpra/buffers/membuf.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/buffers/xxh3.h` & `xpra-4.4.5/xpra/buffers/xxh3.h`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/buffers/xxhash.c` & `xpra-4.4.5/xpra/buffers/xxhash.c`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/buffers/xxhash.h` & `xpra-4.4.5/xpra/buffers/xxhash.h`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/build_info.py` & `xpra-4.4.5/xpra/build_info.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 BUILD_BIT='64bit'
 BUILD_CPU='x86_64'
-BUILD_DATE='2023-03-10'
+BUILD_DATE='2023-05-23'
 BUILD_MACHINE='x86_64'
 BUILD_OS='Linux Fedora 37 ThirtySeven'
-BUILD_TIME='16:32'
+BUILD_TIME='19:16'
 BUILT_BY='antoine'
 BUILT_ON='localhost.localdomain'
-COMPILER_VERSION='gcc (GCC) 12.2.1 20221121 (Red Hat 12.2.1-4)'
-CYTHON_VERSION='3.0.0a11'
-LINKER_VERSION='GNU ld version 2.38-25.fc37'
-PYTHON_VERSION='3.11.2'
+COMPILER_VERSION='gcc (GCC) 12.3.1 20230508 (Red Hat 12.3.1-1)'
+CYTHON_VERSION='0.29.34'
+LINKER_VERSION='GNU ld version 2.38-27.fc37'
+PYTHON_VERSION='3.11.3'
 lib_gobject_introspection='1.74.0'
 lib_gtk='3.24.37'
 lib_gtk_x11='3.24.37'
 lib_nvenc='10'
 lib_nvfbc='6.0'
 lib_py3cairo='1.21.0'
 lib_pygobject='3.42.2'
 lib_python3='3.11'
 lib_vpx='1.12.0'
 lib_x11='1.8.4'
+lib_x264='0.164.3095'
 lib_x265='3.5'
 lib_xcomposite='0.4.5'
 lib_xdamage='1.1.5'
 lib_xext='1.3.4'
 lib_xfixes='6.0.0'
 lib_xkbfile='1.1.0'
 lib_xrandr='1.5.2'
```

### Comparing `xpra-4.4.4/xpra/child_reaper.py` & `xpra-4.4.5/xpra/child_reaper.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/auth/env_handler.py` & `xpra-4.4.5/xpra/client/auth/env_handler.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/auth/file_handler.py` & `xpra-4.4.5/xpra/client/auth/file_handler.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/auth/gss_handler.py` & `xpra-4.4.5/xpra/client/auth/gss_handler.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/auth/kerberos_handler.py` & `xpra-4.4.5/xpra/client/auth/kerberos_handler.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/auth/prompt_handler.py` & `xpra-4.4.5/xpra/client/auth/prompt_handler.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/auth/u2f_handler.py` & `xpra-4.4.5/xpra/client/auth/u2f_handler.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/client_base.py` & `xpra-4.4.5/xpra/client/client_base.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/client_tray.py` & `xpra-4.4.5/xpra/client/client_tray.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/client_widget_base.py` & `xpra-4.4.5/xpra/client/client_widget_base.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/client_window_base.py` & `xpra-4.4.5/xpra/client/client_window_base.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/fake_window_backing.py` & `xpra-4.4.5/xpra/client/fake_window_backing.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gl/gl_check.py` & `xpra-4.4.5/xpra/client/gl/gl_check.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gl/gl_colorspace_conversions.py` & `xpra-4.4.5/xpra/client/gl/gl_colorspace_conversions.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gl/gl_drivers.py` & `xpra-4.4.5/xpra/client/gl/gl_drivers.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gl/gl_spinner.py` & `xpra-4.4.5/xpra/client/gl/gl_spinner.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gl/gl_window_backing_base.py` & `xpra-4.4.5/xpra/client/gl/gl_window_backing_base.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gl/gtk3/gl_client_window.py` & `xpra-4.4.5/xpra/client/gl/gtk3/gl_client_window.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gl/gtk3/gl_drawing_area.py` & `xpra-4.4.5/xpra/client/gl/gtk3/gl_drawing_area.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gl/gtk3/nativegl_client_window.py` & `xpra-4.4.5/xpra/client/gl/gtk3/nativegl_client_window.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gl/window_backend.py` & `xpra-4.4.5/xpra/client/gl/window_backend.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gobject_client_base.py` & `xpra-4.4.5/xpra/client/gobject_client_base.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk3/__init__.py` & `xpra-4.4.5/xpra/client/gtk3/__init__.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk3/cairo_backing.py` & `xpra-4.4.5/xpra/client/gtk3/cairo_backing.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk3/cairo_workaround.pyx` & `xpra-4.4.5/xpra/client/gtk3/cairo_workaround.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk3/client.py` & `xpra-4.4.5/xpra/client/gtk3/client.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk3/client_window.py` & `xpra-4.4.5/xpra/client/gtk3/client_window.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk3/gtk3_client_window.py` & `xpra-4.4.5/xpra/client/gtk3/gtk3_client_window.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk3/gtk3_notifier.py` & `xpra-4.4.5/xpra/client/gtk3/gtk3_notifier.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk3/qrcode_client.py` & `xpra-4.4.5/xpra/client/gtk3/qrcode_client.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk3/show_shortcuts.py` & `xpra-4.4.5/xpra/client/gtk3/show_shortcuts.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk3/splash_screen.py` & `xpra-4.4.5/xpra/client/gtk3/splash_screen.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk3/window_menu.py` & `xpra-4.4.5/xpra/client/gtk3/window_menu.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/bug_report.py` & `xpra-4.4.5/xpra/client/gtk_base/bug_report.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/cairo_backing_base.py` & `xpra-4.4.5/xpra/client/gtk_base/cairo_backing_base.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/client_launcher.py` & `xpra-4.4.5/xpra/client/gtk_base/client_launcher.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/confirm_dialog.py` & `xpra-4.4.5/xpra/client/gtk_base/confirm_dialog.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/css_overrides.py` & `xpra-4.4.5/xpra/client/gtk_base/css_overrides.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/example/bell.py` & `xpra-4.4.5/xpra/client/gtk_base/example/bell.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/example/clicks.py` & `xpra-4.4.5/xpra/client/gtk_base/example/clicks.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/example/colors.py` & `xpra-4.4.5/xpra/client/gtk_base/example/colors.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/example/colors_gradient.py` & `xpra-4.4.5/xpra/client/gtk_base/example/colors_gradient.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/example/colors_plain.py` & `xpra-4.4.5/xpra/client/gtk_base/example/colors_plain.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/example/cursors.py` & `xpra-4.4.5/xpra/client/gtk_base/example/cursors.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/example/file_chooser.py` & `xpra-4.4.5/xpra/client/gtk_base/example/file_chooser.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/example/fontrendering.py` & `xpra-4.4.5/xpra/client/gtk_base/example/fontrendering.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/example/grabs.py` & `xpra-4.4.5/xpra/client/gtk_base/example/grabs.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/example/header_bar.py` & `xpra-4.4.5/xpra/client/gtk_base/example/header_bar.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/example/initiate_moveresize.py` & `xpra-4.4.5/xpra/client/gtk_base/example/initiate_moveresize.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/example/text_entry.py` & `xpra-4.4.5/xpra/client/gtk_base/example/text_entry.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/example/transparent_colors.py` & `xpra-4.4.5/xpra/client/gtk_base/example/transparent_colors.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/example/transparent_window.py` & `xpra-4.4.5/xpra/client/gtk_base/example/transparent_window.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/example/tray.py` & `xpra-4.4.5/xpra/client/gtk_base/example/tray.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/example/window_focus.py` & `xpra-4.4.5/xpra/client/gtk_base/example/window_focus.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/example/window_geometry_hints.py` & `xpra-4.4.5/xpra/client/gtk_base/example/window_geometry_hints.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/example/window_opacity.py` & `xpra-4.4.5/xpra/client/gtk_base/example/window_opacity.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/example/window_overrideredirect.py` & `xpra-4.4.5/xpra/client/gtk_base/example/window_overrideredirect.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/example/window_states.py` & `xpra-4.4.5/xpra/client/gtk_base/example/window_states.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/example/window_title.py` & `xpra-4.4.5/xpra/client/gtk_base/example/window_title.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/example/window_transient.py` & `xpra-4.4.5/xpra/client/gtk_base/example/window_transient.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/gtk_client_base.py` & `xpra-4.4.5/xpra/client/gtk_base/gtk_client_base.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/gtk_client_window_base.py` & `xpra-4.4.5/xpra/client/gtk_base/gtk_client_window_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1668,22 +1668,32 @@
                 self.remove_pointer_overlay_timer = None
                 self.show_pointer_overlay(None)
             self.remove_pointer_overlay_timer = self.timeout_add(CURSOR_IDLE_TIMEOUT*1000, remove_pointer_overlay)
         if prev:
             x, y, w, h = abs_coords(*prev[2:5])
             self.repaint(x, y, w, h)
 
+    def _button_resolve(self, button):
+        if WIN32 and button in (4, 5):
+          # On Windows "X" buttons (the extra buttons sometimes found on the
+          # side of the mouse) are numbered 4 and 5, as there is a different
+          # API for scroll events. Convert them into the X11 convention of 8
+          # and 9.
+          return button + 4
+        return button
 
     def _do_button_press_event(self, event):
         #Gtk.Window.do_button_press_event(self, event)
-        self._button_action(event.button, event, True)
+        button = self._button_resolve(event.button)
+        self._button_action(button, event, True)
 
     def _do_button_release_event(self, event):
         #Gtk.Window.do_button_release_event(self, event)
-        self._button_action(event.button, event, False)
+        button = self._button_resolve(event.button)
+        self._button_action(button, event, False)
 
     ######################################################################
     # pointer motion
 
     def _do_motion_notify_event(self, event):
         #Gtk.Window.do_motion_notify_event(self, event)
         if self.moveresize_event:
@@ -2285,15 +2295,16 @@
         self.cancel_remove_pointer_overlay_timer()
         self.cancel_focus_timer()
         self.cancel_moveresize_timer()
         self.cancel_follow_handler()
         self.on_realize_cb = {}
         ClientWindowBase.destroy(self)
         Gtk.Window.destroy(self)
-        self._unfocus()
+        if self._client.has_focus(self._id):
+            self._unfocus()
         self.destroy = self.noop_destroy
 
 
     def do_unmap_event(self, event):
         self.cancel_follow_handler()
         eventslog("do_unmap_event(%s)", event)
         self._unfocus()
```

### Comparing `xpra-4.4.4/xpra/client/gtk_base/gtk_keyboard_helper.py` & `xpra-4.4.5/xpra/client/gtk_base/gtk_keyboard_helper.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/gtk_spinner.py` & `xpra-4.4.5/xpra/client/gtk_base/gtk_spinner.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/gtk_tray_menu_base.py` & `xpra-4.4.5/xpra/client/gtk_base/gtk_tray_menu_base.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/mdns_gui.py` & `xpra-4.4.5/xpra/client/gtk_base/mdns_gui.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/menu_helper.py` & `xpra-4.4.5/xpra/client/gtk_base/menu_helper.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/open_requests.py` & `xpra-4.4.5/xpra/client/gtk_base/open_requests.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/pass_dialog.py` & `xpra-4.4.5/xpra/client/gtk_base/pass_dialog.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/server_commands.py` & `xpra-4.4.5/xpra/client/gtk_base/server_commands.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/session_info.py` & `xpra-4.4.5/xpra/client/gtk_base/session_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -583,18 +583,22 @@
         for tab in self.tabs:
             p_cb = tab[3]
             if p_cb:
                 p_cb()
 
     def add_graph_button(self, tooltip, click_cb):
         button = Gtk.EventBox()
+        try:
+            arrow_down = Gdk.Cursor.new(Gdk.CursorType.BASED_ARROW_DOWN)
+        except TypeError:
+            arrow_down = None
         def set_cursor(widget):
-            cursor = Gdk.Cursor.new(Gdk.CursorType.BASED_ARROW_DOWN)
-            widget.get_window().set_cursor(cursor)
-        button.connect("realize", set_cursor)
+            widget.get_window().set_cursor(arrow_down)
+        if arrow_down:
+            button.connect("realize", set_cursor)
         graph = Gtk.Image()
         graph.set_size_request(0, 0)
         button.connect("button_press_event", click_cb, graph)
         button.add(graph)
         if tooltip:
             graph.set_tooltip_text(tooltip)
         self.graph_box.add(button)
```

### Comparing `xpra-4.4.4/xpra/client/gtk_base/sessions_gui.py` & `xpra-4.4.5/xpra/client/gtk_base/sessions_gui.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/start_new_command.py` & `xpra-4.4.5/xpra/client/gtk_base/start_new_command.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/statusicon_tray.py` & `xpra-4.4.5/xpra/client/gtk_base/statusicon_tray.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/toolbox.py` & `xpra-4.4.5/xpra/client/gtk_base/toolbox.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/u2f_tool.py` & `xpra-4.4.5/xpra/client/gtk_base/u2f_tool.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/update_status.py` & `xpra-4.4.5/xpra/client/gtk_base/update_status.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/gtk_base/window_info.py` & `xpra-4.4.5/xpra/client/gtk_base/window_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,14 +215,15 @@
         self.title_label.set_text(w.get_title())
         self.bool_icon(self.or_image, w._override_redirect)
         self.state_label.set_text(get_window_state(w))
         self.attributes_label.set_text(get_window_attributes(w))
         self.bool_icon(self.focus_image, w._focused)
         self.button_state_label.set_text(csv(b for b,s in w.button_state.items() if s) or "none")
         fps = "n/a"
+        b = w._backing
         if b:
             update_fps = getattr(b, "update_fps", None)
             if callable(update_fps):
                 update_fps()
                 fps = str(getattr(b, "fps_value", "n/a"))
         self.fps_label.set_text(fps)
         #self.group_leader_label.set_text(str(w.group_leader))
```

### Comparing `xpra-4.4.4/xpra/client/keyboard_helper.py` & `xpra-4.4.5/xpra/client/keyboard_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,25 +130,28 @@
                 log("not matched %s for %s: %s not in %s",
                     shortcut, key_name, rm, modifiers)
                 return False
             try:
                 extra_modifiers.remove(rm)
             except ValueError:
                 pass        #same modifier listed twice?
-        kmod = self.keyboard.get_keymap_modifiers()[0]
+        kmod, _, ignored = self.keyboard.get_keymap_modifiers()
         if not kmod and self.keyboard.modifier_keys:
             #fallback to server supplied map:
             kmod = self.keyboard.modifier_keys
         #ie: {'ISO_Level3_Shift': 'mod5', 'Meta_L': 'mod1', ...}
         log("keymap modifiers: %s", kmod)
         ignoremod = ("Caps_Lock", "Num_Lock")
         for x in ignoremod:
             mod = kmod.get(x)
             if mod in extra_modifiers:
                 extra_modifiers.remove(mod)
+        for mod in ignored:
+            if mod in extra_modifiers:
+                extra_modifiers.remove(mod)
         if extra_modifiers:
             log("skipping partial shortcut match %s, modifiers unmatched: %s", shortcut, extra_modifiers)
             return False
         log("matched shortcut %s", shortcut)
         if not depressed:
             #when the key is released, just ignore it - do NOT send it to the server!
             return True
```

### Comparing `xpra-4.4.4/xpra/client/keyboard_shortcuts_parser.py` & `xpra-4.4.5/xpra/client/keyboard_shortcuts_parser.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/mixin_features.py` & `xpra-4.4.5/xpra/client/mixin_features.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/mixins/audio.py` & `xpra-4.4.5/xpra/client/mixins/audio.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/mixins/clipboard.py` & `xpra-4.4.5/xpra/client/mixins/clipboard.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/mixins/display.py` & `xpra-4.4.5/xpra/client/mixins/display.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,15 +296,15 @@
             return
         root_w, root_h = self.cp(*self.get_root_size())
         maxw, maxh = root_w, root_h
         try:
             server_w, server_h = self.server_actual_desktop_size
             maxw = max(root_w, server_w)
             maxh = max(root_h, server_h)
-        except ValueError:
+        except (TypeError, ValueError):
             pass
         if maxw<=0 or maxh<=0 or maxw>=32768 or maxh>=32768:
             message = "invalid maximum desktop size: %ix%i" % (maxw, maxh)
             log(message)
             self.quit(EXIT_INTERNAL_ERROR)
             raise SystemExit(message)
         if maxw>=16384 or maxh>=16384:
```

### Comparing `xpra-4.4.4/xpra/client/mixins/encodings.py` & `xpra-4.4.5/xpra/client/mixins/encodings.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/mixins/fileprint_mixin.py` & `xpra-4.4.5/xpra/client/mixins/fileprint_mixin.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/mixins/mmap.py` & `xpra-4.4.5/xpra/client/mixins/mmap.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/mixins/network_listener.py` & `xpra-4.4.5/xpra/client/mixins/network_listener.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def init(self, opts):
         def err(msg):
             raise InitException(msg)
         self.sockets = create_sockets(opts, err)
         if opts.bind and (not WIN32 or WIN32_LOCAL_SOCKETS or opts.bind!="auto"):
             try:
                 local_sockets = setup_local_sockets(opts.bind,
-                                                None, opts.client_socket_dirs,
+                                                None, opts.client_socket_dirs, None,
                                                 str(os.getpid()), True,
                                                 opts.mmap_group, opts.socket_permissions)
             except (OSError, InitExit) as e:
                 log("setup_local_sockets bind=%s, client_socket_dirs=%s",
                     opts.bind, opts.client_socket_dirs, exc_info=True)
                 log.warn("Warning: failed to create the client sockets:")
                 log.warn(" '%s'", e)
```

### Comparing `xpra-4.4.4/xpra/client/mixins/network_state.py` & `xpra-4.4.5/xpra/client/mixins/network_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,15 +278,15 @@
         log("check_echo_timeout(%s) last_ping_echoed_time=%s", ping_time, self.last_ping_echoed_time)
         if self.last_ping_echoed_time<ping_time:
             #no point trying to use disconnect_and_quit() to tell the server here..
             self.warn_and_quit(EXIT_CONNECTION_LOST, "server ping timeout - waited %s seconds without a response" % PING_TIMEOUT)
 
     def send_ping(self):
         p = self._protocol
-        if not p or p.TYPE!="xpra":
+        if not p or p.TYPE not in ("xpra", "websocket"):
             self.ping_timer = None
             return False
         now_ms = int(1000.0*monotonic())
         self.send("ping", now_ms)
         wait = 2.0
         spl = tuple(self.server_ping_latency)
         if spl:
```

### Comparing `xpra-4.4.4/xpra/client/mixins/notifications.py` & `xpra-4.4.5/xpra/client/mixins/notifications.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/mixins/remote_logging.py` & `xpra-4.4.5/xpra/client/mixins/remote_logging.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/mixins/rpc.py` & `xpra-4.4.5/xpra/client/mixins/rpc.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/mixins/serverinfo_mixin.py` & `xpra-4.4.5/xpra/client/mixins/serverinfo_mixin.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/mixins/stub_client_mixin.py` & `xpra-4.4.5/xpra/client/mixins/stub_client_mixin.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/mixins/tray.py` & `xpra-4.4.5/xpra/client/mixins/tray.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/mixins/webcam.py` & `xpra-4.4.5/xpra/client/mixins/webcam.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/mixins/window_manager.py` & `xpra-4.4.5/xpra/client/mixins/window_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -680,21 +680,17 @@
         #adding the icon overlay (if enabled)
         from PIL import Image  # @UnresolvedImport
         coding = bytestostr(coding)
         iconlog("%s.update_icon(%s, %s, %s, %s bytes) ICON_SHRINKAGE=%s, ICON_OVERLAY=%s",
                 self, width, height, coding, len(data), ICON_SHRINKAGE, ICON_OVERLAY)
         if coding=="default":
             img = self.overlay_image
-        elif coding == "BGRA":
+        elif coding in ("BGRA", "RGBA"):
             rowstride = width*4
-            img = Image.frombytes("RGBA", (width,height), memoryview_to_bytes(data), "raw", "BGRA", rowstride, 1)
-            has_alpha = True
-        elif coding in ("BGRA", ):
-            rowstride = width*4
-            img = Image.frombytes("RGBA", (width,height), memoryview_to_bytes(data), "raw", "BGRA", rowstride, 1)
+            img = Image.frombytes("RGBA", (width,height), memoryview_to_bytes(data), "raw", coding, rowstride, 1)
             has_alpha = True
         else:
             from xpra.codecs.pillow.decoder import open_only
             img = open_only(data, ("png", ))
             if img.mode not in ("RGB", "RGBA"):
                 img = img.convert("RGBA")
             has_alpha = img.mode=="RGBA"
@@ -1284,14 +1280,17 @@
 
     ######################################################################
     # focus:
     def send_focus(self, wid):
         focuslog("send_focus(%s)", wid)
         self.send("focus", wid, self.get_current_modifiers())
 
+    def has_focus(self, wid):
+        return self._focused and self._focused==wid
+
     def update_focus(self, wid, gotit):
         focused = self._focused
         focuslog(f"update_focus({wid}, {gotit}) focused={focused}, grabbed={self._window_with_grab}")
         if gotit:
             if focused is not wid:
                 self.send_focus(wid)
                 self._focused = wid
```

### Comparing `xpra-4.4.4/xpra/client/paint_colors.py` & `xpra-4.4.5/xpra/client/paint_colors.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/rfb_protocol.py` & `xpra-4.4.5/xpra/client/rfb_protocol.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/scaling_parser.py` & `xpra-4.4.5/xpra/client/scaling_parser.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/spinner.py` & `xpra-4.4.5/xpra/client/spinner.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/top_client.py` & `xpra-4.4.5/xpra/client/top_client.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/tray_base.py` & `xpra-4.4.5/xpra/client/tray_base.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/ui_client_base.py` & `xpra-4.4.5/xpra/client/ui_client_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,16 +392,16 @@
             #we may be running inside another server!
             try:
                 from xpra.server.server_uuid import get_uuid, get_mode  #pylint: disable=import-outside-toplevel
                 if get_mode()!="shadow":
                     uuid = get_uuid()
                     if uuid:
                         caps["server_uuid"] = uuid
-            except ImportError:
-                pass
+            except (ImportError, RuntimeError):
+                log("skipped server uuid lookup", exc_info=True)
         for x in (#generic feature flags:
             "wants_events", "setting-change",
             "xdg-menu-update", "mouse",
             ):
             caps[x] = True
         caps.setdefault("wants", []).append("events")
         caps.update({
```

### Comparing `xpra-4.4.4/xpra/client/window_backing_base.py` & `xpra-4.4.5/xpra/client/window_backing_base.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/client/window_border.py` & `xpra-4.4.5/xpra/client/window_border.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/clipboard/clipboard_core.py` & `xpra-4.4.5/xpra/clipboard/clipboard_core.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/clipboard/clipboard_timeout_helper.py` & `xpra-4.4.5/xpra/clipboard/clipboard_timeout_helper.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/argb/argb.pxd` & `xpra-4.4.5/xpra/codecs/argb/argb.pxd`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/argb/argb.pyx` & `xpra-4.4.5/xpra/codecs/argb/argb.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/argb/encoder.py` & `xpra-4.4.5/xpra/codecs/argb/encoder.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/argb/scale.py` & `xpra-4.4.5/xpra/codecs/argb/scale.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/avif/avif.pxd` & `xpra-4.4.5/xpra/codecs/avif/avif.pxd`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/avif/decoder.pyx` & `xpra-4.4.5/xpra/codecs/avif/decoder.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/avif/encoder.pyx` & `xpra-4.4.5/xpra/codecs/avif/encoder.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/codec_checks.py` & `xpra-4.4.5/xpra/codecs/codec_checks.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/codec_constants.py` & `xpra-4.4.5/xpra/codecs/codec_constants.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/codec_debug.py` & `xpra-4.4.5/xpra/codecs/codec_debug.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/csc_cython/colorspace_converter.pyx` & `xpra-4.4.5/xpra/codecs/csc_cython/colorspace_converter.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/csc_libyuv/colorspace_converter.pyx` & `xpra-4.4.5/xpra/codecs/csc_libyuv/colorspace_converter.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/csc_swscale/colorspace_converter.pyx` & `xpra-4.4.5/xpra/codecs/csc_swscale/colorspace_converter.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/cuda_common/cuda_context.py` & `xpra-4.4.5/xpra/codecs/cuda_common/cuda_context.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/dec_avcodec2/decoder.pyx` & `xpra-4.4.5/xpra/codecs/dec_avcodec2/decoder.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/drm/drm.pyx` & `xpra-4.4.5/xpra/codecs/drm/drm.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/enc_ffmpeg/encoder.pyx` & `xpra-4.4.5/xpra/codecs/enc_ffmpeg/encoder.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1695,15 +1695,15 @@
 
             pixels = image.get_pixels()
             istrides = image.get_rowstride()
             assert len(pixels)==self.nplanes, "image pixels does not have %i planes! (found %s)" % (self.nplanes, len(pixels))
             assert len(istrides)==self.nplanes, "image strides does not have %i values! (found %s)" % (self.nplanes, len(istrides))
             #populate the avframe:
             ret = av_frame_make_writable(self.av_frame)
-            if not ret!=0:
+            if ret<0:
                 raise Exception(av_error_str(ret))
             for i in range(4):
                 if i<self.nplanes:
                     if PyObject_GetBuffer(pixels[i], &py_buf[i], PyBUF_ANY_CONTIGUOUS):
                         raise Exception("failed to read pixel data from %s" % type(pixels[i]))
                     #log("plane %s: %i bytes (%ix%i stride=%i)", ["Y", "U", "V"][i], buf_len, self.width, self.height, istrides[i])
                     self.av_frame.data[i] = <uint8_t *> py_buf[i].buf
```

### Comparing `xpra-4.4.4/xpra/codecs/enc_proxy/encoder.py` & `xpra-4.4.5/xpra/codecs/enc_proxy/encoder.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/enc_x264/encoder.pyx` & `xpra-4.4.5/xpra/codecs/enc_x264/encoder.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/enc_x265/encoder.pyx` & `xpra-4.4.5/xpra/codecs/enc_x265/encoder.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/evdi/capture.pyx` & `xpra-4.4.5/xpra/codecs/evdi/capture.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/evdi/evdi_compat.h` & `xpra-4.4.5/xpra/codecs/evdi/evdi_compat.h`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/evdi/load.py` & `xpra-4.4.5/xpra/codecs/evdi/load.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/icon_util.py` & `xpra-4.4.5/xpra/codecs/icon_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/image_wrapper.py` & `xpra-4.4.5/xpra/codecs/image_wrapper.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/jpeg/decoder.pyx` & `xpra-4.4.5/xpra/codecs/jpeg/decoder.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/jpeg/encoder.pyx` & `xpra-4.4.5/xpra/codecs/jpeg/encoder.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/libav_common/av_log.pyx` & `xpra-4.4.5/xpra/codecs/libav_common/av_log.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/loader.py` & `xpra-4.4.5/xpra/codecs/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,18 @@
                 init_module = getattr(ic, "init_module", None)
                 log(f"{class_module}.init_module={init_module}")
                 if init_module:
                     init_module()
 
                 if classnames:
                     for classname in classnames:
-                        clazz = getattr(ic, classname)
+                        try:
+                            clazz = getattr(ic, classname)
+                        except AttributeError as e:
+                            raise ImportError(f"cannot find {classname!r} in {ic}") from None
                         log(f"{class_module}.{classname}={clazz}")
 
                 selftest = getattr(ic, "selftest", None)
                 log(f"{name}.selftest={selftest}")
                 if SELFTEST and selftest:
                     if name in CODEC_FAIL_SELFTEST:
                         raise ImportError("codec found in fail selftest list")
```

### Comparing `xpra-4.4.4/xpra/codecs/nv_util.py` & `xpra-4.4.5/xpra/codecs/nv_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/nvenc/encoder.pyx` & `xpra-4.4.5/xpra/codecs/nvenc/encoder.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/nvfbc/capture.py` & `xpra-4.4.5/xpra/codecs/nvfbc/capture.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/nvfbc/cuda_image_wrapper.py` & `xpra-4.4.5/xpra/codecs/nvfbc/cuda_image_wrapper.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/nvfbc/fbc_capture_linux.pyx` & `xpra-4.4.5/xpra/codecs/nvfbc/fbc_capture_linux.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/nvfbc/fbc_capture_win.pyx` & `xpra-4.4.5/xpra/codecs/nvfbc/fbc_capture_win.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/nvjpeg/common.pyx` & `xpra-4.4.5/xpra/codecs/nvjpeg/common.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/nvjpeg/decoder.pyx` & `xpra-4.4.5/xpra/codecs/nvjpeg/decoder.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/nvjpeg/encoder.pyx` & `xpra-4.4.5/xpra/codecs/nvjpeg/encoder.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/nvjpeg/nvjpeg.pxd` & `xpra-4.4.5/xpra/codecs/nvjpeg/nvjpeg.pxd`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/pillow/__init__.py` & `xpra-4.4.5/xpra/codecs/pillow/__init__.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/pillow/decoder.py` & `xpra-4.4.5/xpra/codecs/pillow/decoder.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/pillow/encoder.py` & `xpra-4.4.5/xpra/codecs/pillow/encoder.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/rgb_transform.py` & `xpra-4.4.5/xpra/codecs/rgb_transform.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/spng/decoder.pyx` & `xpra-4.4.5/xpra/codecs/spng/decoder.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/spng/encoder.pyx` & `xpra-4.4.5/xpra/codecs/spng/encoder.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/spng/spng.pxd` & `xpra-4.4.5/xpra/codecs/spng/spng.pxd`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/v4l2/pusher.pyx` & `xpra-4.4.5/xpra/codecs/v4l2/pusher.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/video_helper.py` & `xpra-4.4.5/xpra/codecs/video_helper.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/vpx/decoder.pyx` & `xpra-4.4.5/xpra/codecs/vpx/decoder.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/vpx/encoder.pyx` & `xpra-4.4.5/xpra/codecs/vpx/encoder.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/vpx/vpx.pxd` & `xpra-4.4.5/xpra/codecs/vpx/vpx.pxd`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/webp/decoder.pyx` & `xpra-4.4.5/xpra/codecs/webp/decoder.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/codecs/webp/encoder.pyx` & `xpra-4.4.5/xpra/codecs/webp/encoder.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/colorstreamhandler.py` & `xpra-4.4.5/xpra/colorstreamhandler.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/common.py` & `xpra-4.4.5/xpra/common.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/dbus/common.py` & `xpra-4.4.5/xpra/dbus/common.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/dbus/helper.py` & `xpra-4.4.5/xpra/dbus/helper.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/dbus/notifications_forwarder.py` & `xpra-4.4.5/xpra/dbus/notifications_forwarder.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/exit_codes.py` & `xpra-4.4.5/xpra/exit_codes.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/gtk_common/about.py` & `xpra-4.4.5/xpra/gtk_common/about.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/gtk_common/auth_dialog.py` & `xpra-4.4.5/xpra/gtk_common/auth_dialog.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/gtk_common/cursor_names.py` & `xpra-4.4.5/xpra/gtk_common/cursor_names.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/gtk_common/desktop_greeter.py` & `xpra-4.4.5/xpra/gtk_common/desktop_greeter.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/gtk_common/error.py` & `xpra-4.4.5/xpra/gtk_common/error.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/gtk_common/gobject_compat.py` & `xpra-4.4.5/xpra/gtk_common/gobject_compat.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/gtk_common/gobject_util.py` & `xpra-4.4.5/xpra/gtk_common/gobject_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/gtk_common/graph.py` & `xpra-4.4.5/xpra/gtk_common/graph.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/gtk_common/gtk2_notifier-LICENSE.txt` & `xpra-4.4.5/xpra/gtk_common/gtk2_notifier-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/gtk_common/gtk3/gdk_atoms.pyx` & `xpra-4.4.5/xpra/gtk_common/gtk3/gdk_atoms.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/gtk_common/gtk3/gdk_bindings.pxd` & `xpra-4.4.5/xpra/gtk_common/gtk3/gdk_bindings.pxd`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/gtk_common/gtk3/gdk_bindings.pyx` & `xpra-4.4.5/xpra/gtk_common/gtk3/gdk_bindings.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/gtk_common/gtk_clipboard.py` & `xpra-4.4.5/xpra/gtk_common/gtk_clipboard.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/gtk_common/gtk_notifier.py` & `xpra-4.4.5/xpra/gtk_common/gtk_notifier.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/gtk_common/gtk_util.py` & `xpra-4.4.5/xpra/gtk_common/gtk_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/gtk_common/gtk_view_clipboard.py` & `xpra-4.4.5/xpra/gtk_common/gtk_view_clipboard.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/gtk_common/gtk_view_keyboard.py` & `xpra-4.4.5/xpra/gtk_common/gtk_view_keyboard.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/gtk_common/gui.py` & `xpra-4.4.5/xpra/gtk_common/gui.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/gtk_common/keymap.py` & `xpra-4.4.5/xpra/gtk_common/keymap.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/gtk_common/start_gui.py` & `xpra-4.4.5/xpra/gtk_common/start_gui.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/keyboard/layouts.py` & `xpra-4.4.5/xpra/keyboard/layouts.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/keyboard/mask.py` & `xpra-4.4.5/xpra/keyboard/mask.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/log.py` & `xpra-4.4.5/xpra/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 # This file is part of Xpra.
 # Copyright (C) 2008, 2009 Nathaniel Smith <njs@pobox.com>
-# Copyright (C) 2012-2022 Antoine Martin <antoine@xpra.org>
+# Copyright (C) 2012-2023 Antoine Martin <antoine@xpra.org>
 # Xpra is released under the terms of the GNU GPL v2, or, at your option, any
 # later version. See the file COPYING for details.
 
 import os
 import sys
 import logging
 import weakref
 import itertools
 # This module is used by non-GUI programs and thus must not import gtk.
 
-LOG_PREFIX = os.environ.get("XPRA_LOG_PREFIX", "")
-LOG_FORMAT = os.environ.get("XPRA_LOG_FORMAT", "%(asctime)s %(message)s")
+LOG_PREFIX = ""
+LOG_FORMAT = "%(asctime)s %(message)s"
+DEBUG_MODULES = ()
+if os.name!="posix" or os.getuid()!=0:
+    LOG_FORMAT = os.environ.get("XPRA_LOG_FORMAT", LOG_FORMAT)
+    LOG_PREFIX = os.environ.get("XPRA_LOG_PREFIX", LOG_PREFIX)
+    DEBUG_MODULES = tuple(x.strip() for x in os.environ.get("XPRA_DEBUG_MODULES", "").split(",") if x.strip())
 NOPREFIX_FORMAT = "%(message)s"
 
-DEBUG_MODULES = [x for x in os.environ.get("XPRA_DEBUG_MODULES", "").split(",") if x]
 
 logging.basicConfig(format=LOG_FORMAT)
 logging.root.setLevel(logging.INFO)
 
 #so we can keep a reference to all the loggers in use
 #we may have multiple loggers for the same key, so use a dict
 #but we don't want to prevent garbage collection so use a list of weakrefs
```

### Comparing `xpra-4.4.4/xpra/make_thread.py` & `xpra-4.4.5/xpra/make_thread.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/bencode/__init__.py` & `xpra-4.4.5/xpra/net/bencode/__init__.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/bencode/bencode.py` & `xpra-4.4.5/xpra/net/bencode/bencode.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/bencode/cython_bencode.pyx` & `xpra-4.4.5/xpra/net/bencode/cython_bencode.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/brotli/compressor.pyx` & `xpra-4.4.5/xpra/net/brotli/compressor.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -87,17 +87,17 @@
     cdef uint8_t *out = <uint8_t *> out_buf.get_mem()
 
     cdef Py_buffer in_buf
     if PyObject_GetBuffer(data, &in_buf, PyBUF_ANY_CONTIGUOUS):
         raise Exception("failed to read data from %s" % type(data))
     cdef const uint8_t *in_ptr = <const uint8_t*> in_buf.buf
 
-    cdef size_t out_size
+    cdef size_t out_size = max_size
     cdef int r
-    log("brotli.compress(%i bytes, %i)", in_buf.len, quality)
+    log("brotli.compress(%i bytes, %i) into %i byte buffer", in_buf.len, quality, out_size)
     try:
         with nogil:
             r = BrotliEncoderCompress(quality, BROTLI_DEFAULT_WINDOW,
                                       BROTLI_MODE_GENERIC,
                                       in_buf.len, in_ptr,
                                       &out_size, out)
     finally:
```

### Comparing `xpra-4.4.4/xpra/net/brotli/decompressor.pyx` & `xpra-4.4.5/xpra/net/brotli/decompressor.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/bytestreams.py` & `xpra-4.4.5/xpra/net/bytestreams.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/common.py` & `xpra-4.4.5/xpra/net/common.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/compression.py` & `xpra-4.4.5/xpra/net/compression.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/crypto.py` & `xpra-4.4.5/xpra/net/crypto.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/d3des.py` & `xpra-4.4.5/xpra/net/d3des.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/digest.py` & `xpra-4.4.5/xpra/net/digest.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/fake_jitter.py` & `xpra-4.4.5/xpra/net/fake_jitter.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/file_transfer.py` & `xpra-4.4.5/xpra/net/file_transfer.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/header.py` & `xpra-4.4.5/xpra/net/header.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/http_handler.py` & `xpra-4.4.5/xpra/net/http_handler.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/libproxy.py` & `xpra-4.4.5/xpra/net/libproxy.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/lz4.pyx` & `xpra-4.4.5/xpra/net/lz4.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/mdns/__init__.py` & `xpra-4.4.5/xpra/net/mdns/__init__.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/mdns/avahi_listener.py` & `xpra-4.4.5/xpra/net/mdns/avahi_listener.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/mdns/avahi_publisher.py` & `xpra-4.4.5/xpra/net/mdns/avahi_publisher.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/mdns/zeroconf_listener.py` & `xpra-4.4.5/xpra/net/mdns/zeroconf_listener.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/mdns/zeroconf_publisher.py` & `xpra-4.4.5/xpra/net/mdns/zeroconf_publisher.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,14 +121,15 @@
             td = self.txt_rec(text_dict or {})
             if zeroconf_version<"0.23":
                 self.args = (st, regname, self.address, port, 0, 0, td)
             else:
                 self.kwargs = {
                     "type_"         : st,       #_xpra._tcp.local.
                     "name"          : regname,
+                    "server"        : regname,
                     "port"          : port,
                     "properties"    : td,
                     "addresses"     : [self.address],
                     }
             service = ServiceInfo(*self.args, **self.kwargs)
             log("ServiceInfo(%s, %s)=%s", self.args, self.kwargs, service)
             self.service = service
```

### Comparing `xpra-4.4.4/xpra/net/mmap_pipe.py` & `xpra-4.4.5/xpra/net/mmap_pipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,9 +338,9 @@
             mmap_area.seek(end)
             mmap_area.write(memoryview_to_bytes(data[:chunk]))
             mmap_area.seek(8)
             mmap_area.write(memoryview_to_bytes(data[chunk:]))
             l2 = l-chunk
             chunks = [(end, chunk), (8, l2)]
             mmap_data_end.value = 8+l2
-    log("sending damage with mmap: %s", data)
+    log("sending damage with mmap: %s bytes", len(data))
     return chunks, mmap_free_size
```

### Comparing `xpra-4.4.4/xpra/net/net_util.py` & `xpra-4.4.5/xpra/net/net_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,37 +164,38 @@
         if if_nametoindex:
             try:
                 if_nametoindex(iface)
             except OSError:
                 return None
             else:
                 return iface
-    if ip.find(":")>=0:
-        #ipv6?
-        return None
     if any(x for x in ip if (".:0123456789").find(x)<0):
         #extra characters, assume this is a hostname:
         try:
             v = socket.getaddrinfo(ip, None)
             assert len(v)>0
         except Exception as e:
             log("socket.getaddrinfo(%s, None)", ip, exc_info=True)
-            log.error(f"Error revolving {ip!r}: {e}")
+            log.error(f"Error resolving {ip!r}: {e}")
             return None
         for i, x in enumerate(v):
             family, socktype, proto, canonname, sockaddr = x
             log("get_iface(%s) [%i]=%s", ip, i, (family, socktype, proto, canonname, sockaddr))
             if family==socket.AF_INET:
                 break
         log("get_iface(%s) sockaddr=%s", ip, sockaddr)
         ip = sockaddr[0]
 
-    ip_parts = ip.split(".")
-    if len(ip_parts)!=4:
-        return None
+    if ip.find(":")>=0:
+        #ipv6?
+        ip_parts = ip.split(":")
+    else:
+        ip_parts = ip.split(".")
+        if len(ip_parts)!=4:
+            return None
 
     best_match = None
     get_bind_IPs()
     for iface, ipmasks in iface_ipmasks.items():
         for test_ip, mask in ipmasks:
             if test_ip == ip:
                 #exact match
```

### Comparing `xpra-4.4.4/xpra/net/packet_encoding.py` & `xpra-4.4.5/xpra/net/packet_encoding.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/protocol.py` & `xpra-4.4.5/xpra/net/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     return queue
 
 def force_flush_queue(q):
     try:
         #discard all elements in the old queue and push the None marker:
         try:
             while q.qsize()>0:
-                q.read(False)
+                q.get(False)
         except Exception:
             log("force_flush_queue(%s)", q, exc_info=True)
         q.put_nowait(None)
     except Exception:
         log("force_flush_queue(%s)", q, exc_info=True)
 
 def find_xpra_header(data, index=0, max_data_size=2**16):
```

### Comparing `xpra-4.4.4/xpra/net/protocol_classes.py` & `xpra-4.4.5/xpra/net/protocol_classes.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/pycryptography_backend.py` & `xpra-4.4.5/xpra/net/pycryptography_backend.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/qrcode.py` & `xpra-4.4.5/xpra/net/qrcode.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/qrencode.pyx` & `xpra-4.4.5/xpra/net/qrencode.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/rencodeplus/rencodeplus.pyx` & `xpra-4.4.5/xpra/net/rencodeplus/rencodeplus.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/rfb/rfb_const.py` & `xpra-4.4.5/xpra/net/rfb/rfb_const.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/rfb/rfb_encode.py` & `xpra-4.4.5/xpra/net/rfb/rfb_encode.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/rfb/rfb_protocol.py` & `xpra-4.4.5/xpra/net/rfb/rfb_protocol.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/socket_util.py` & `xpra-4.4.5/xpra/net/socket_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -509,22 +509,21 @@
     #we used to strip the screen from the display string, ie: ":0.0" -> ":0"
     #but now we allow it.. (untested!)
     for char in after_sc:
         assert char in "0123456789.", "invalid character in display name '%s': %s" % (local_display_name, char)
     return local_display_name
 
 
-def setup_local_sockets(bind, socket_dir, socket_dirs, display_name, clobber,
+def setup_local_sockets(bind, socket_dir, socket_dirs, session_dir, display_name, clobber,
                         mmap_group="auto", socket_permissions="600", username="", uid=0, gid=0):
     log = get_network_logger()
-    log("setup_local_sockets%s", (bind, socket_dir, socket_dirs, display_name, clobber,
+    log("setup_local_sockets%s", (bind, socket_dir, socket_dirs, session_dir, display_name, clobber,
                                   mmap_group, socket_permissions, username, uid, gid))
     if not bind:
         return {}
-    session_dir = os.environ.get("XPRA_SESSION_DIR")
     if not socket_dir and (not socket_dirs or (len(socket_dirs)==1 and not socket_dirs[0])):
         if WIN32:
             socket_dirs = [""]
         elif not session_dir:
             raise InitExit(EXIT_SOCKET_CREATION_ERROR,
                            "at least one socket directory must be set to use unix domain sockets")
     from xpra.platform.dotxpra import DotXpra, norm_makepath
@@ -751,23 +750,24 @@
     try:
         from xpra.net import mdns
         assert mdns
         from xpra.net.mdns import XPRA_MDNS_TYPE, RFB_MDNS_TYPE
     except ImportError as e:
         log("mdns support is not installed: %s", e)
         return ()
-    PREFER_ZEROCONF = envbool("XPRA_PREFER_ZEROCONF", True)
+    PREFER_ZEROCONF = envbool("XPRA_PREFER_ZEROCONF", False)
     imports = [import_zeroconf, import_avahi]
     if not PREFER_ZEROCONF:
         imports = reversed(imports)
     MDNSPublishers = get_interface_index = None
     exceptions = []
     for i in imports:
         try:
             MDNSPublishers, get_interface_index = i()
+            break
         except ImportError as e:
             log("mdns import failure", exc_info=True)
             exceptions.append(e)
     if not MDNSPublishers or not get_interface_index:
         MDNS_WARNING = True
         log.warn("Warning: failed to load the mdns publishers")
         for e in exceptions:
```

### Comparing `xpra-4.4.4/xpra/net/ssh.py` & `xpra-4.4.5/xpra/net/ssh.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/sshfp.py` & `xpra-4.4.5/xpra/net/sshfp.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/subprocess_wrapper.py` & `xpra-4.4.5/xpra/net/subprocess_wrapper.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/upnp.py` & `xpra-4.4.5/xpra/net/upnp.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/vsock.pyx` & `xpra-4.4.5/xpra/net/vsock.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/websockets/common.py` & `xpra-4.4.5/xpra/net/websockets/common.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/websockets/handler.py` & `xpra-4.4.5/xpra/net/websockets/handler.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/websockets/header.py` & `xpra-4.4.5/xpra/net/websockets/header.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/websockets/headers/browser_cookie.py` & `xpra-4.4.5/xpra/net/websockets/headers/browser_cookie.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/websockets/headers/default.py` & `xpra-4.4.5/xpra/net/websockets/headers/default.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/websockets/mask.pyx` & `xpra-4.4.5/xpra/net/websockets/mask.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/net/websockets/protocol.py` & `xpra-4.4.5/xpra/net/websockets/protocol.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/notifications/common.py` & `xpra-4.4.5/xpra/notifications/common.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/notifications/dbus_notifier.py` & `xpra-4.4.5/xpra/notifications/dbus_notifier.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/notifications/notifier_base.py` & `xpra-4.4.5/xpra/notifications/notifier_base.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/notifications/pynotify_notifier.py` & `xpra-4.4.5/xpra/notifications/pynotify_notifier.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/os_util.py` & `xpra-4.4.5/xpra/os_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/__init__.py` & `xpra-4.4.5/xpra/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/darwin/__init__.py` & `xpra-4.4.5/xpra/platform/darwin/__init__.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/darwin/features.py` & `xpra-4.4.5/xpra/platform/darwin/features.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/darwin/gdk3_bindings.pyx` & `xpra-4.4.5/xpra/platform/darwin/gdk3_bindings.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/darwin/gl_context.py` & `xpra-4.4.5/xpra/platform/darwin/gl_context.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/darwin/gui.py` & `xpra-4.4.5/xpra/platform/darwin/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -739,29 +739,30 @@
         #opengl windows may need to be re-created since the GPU may have changed:
         if (flags & kCGDisplaySetModeFlag) and c and c.opengl_enabled:
             c.reinit_windows()
 
     def check_display(self):
         log("check_display()")
         try:
+            c = self.client
             asleep = None
             if not can_access_display():
                 asleep = True
             else:
                 did = CG.CGMainDisplayID()
                 log("check_display() CGMainDisplayID()=%#x", did)
-                if did and self.client:
+                if did and c:
                     asleep = bool(CG.CGDisplayIsAsleep(did))
                     log("check_display() CGDisplayIsAsleep(%#x)=%s", did, asleep)
-            if asleep is not None and self.display_is_asleep!=asleep:
+            if c and asleep is not None and self.display_is_asleep!=asleep:
                 self.display_is_asleep = asleep
                 if asleep:
-                    self.client.suspend()
+                    c.suspend()
                 else:
-                    self.client.resume()
+                    c.resume()
             return True
         except Exception:
             log.error("Error checking display sleep status", exc_info=True)
             self.check_display_timer = 0
             return False
 
     def run(self):
```

### Comparing `xpra-4.4.4/xpra/platform/darwin/keyboard.py` & `xpra-4.4.5/xpra/platform/darwin/keyboard.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/darwin/keyboard_config.py` & `xpra-4.4.5/xpra/platform/darwin/keyboard_config.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/darwin/netdev_query.py` & `xpra-4.4.5/xpra/platform/darwin/netdev_query.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/darwin/nsevent_glue.m` & `xpra-4.4.5/xpra/platform/darwin/nsevent_glue.m`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/darwin/osx_clipboard.py` & `xpra-4.4.5/xpra/platform/darwin/osx_clipboard.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/darwin/osx_menu.py` & `xpra-4.4.5/xpra/platform/darwin/osx_menu.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/darwin/osx_tray.py` & `xpra-4.4.5/xpra/platform/darwin/osx_tray.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/darwin/paths.py` & `xpra-4.4.5/xpra/platform/darwin/paths.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/darwin/shadow_server.py` & `xpra-4.4.5/xpra/platform/darwin/shadow_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/displayfd.py` & `xpra-4.4.5/xpra/platform/displayfd.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/dotxpra.py` & `xpra-4.4.5/xpra/platform/dotxpra.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,17 @@
             with umask_context(0):
                 os.mkdir(d, mode)
             if uid!=os.getuid() or gid!=os.getgid():
                 os.lchown(d, uid, gid)
         elif d!="/tmp":
             try:
                 st_mode = os.stat(d).st_mode & 0o777
+                if st_mode==0o750 and d.startswith("/run/xpra"):
+                    #this directory is for shared sockets, o750 is OK
+                    return
                 if st_mode!=mode:
                     #perhaps this directory lives in $XDG_RUNTIME_DIR
                     #ie: /run/user/$UID/xpra or /run/user/$UID/xpra/100
                     xrd = os.environ.get("XDG_RUNTIME_DIR")
                     if xrd and d.startswith(xrd) and os.stat(xrd).st_mode & 0o777==0o700:
                         #$XDG_RUNTIME_DIR has the correct permissions
                         return
```

### Comparing `xpra-4.4.4/xpra/platform/features.py` & `xpra-4.4.5/xpra/platform/features.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/gl_context.py` & `xpra-4.4.5/xpra/platform/gl_context.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/gui.py` & `xpra-4.4.5/xpra/platform/gui.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/info.py` & `xpra-4.4.5/xpra/platform/info.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/keyboard.py` & `xpra-4.4.5/xpra/platform/keyboard.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/keyboard_base.py` & `xpra-4.4.5/xpra/platform/keyboard_base.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/menu_helper.py` & `xpra-4.4.5/xpra/platform/menu_helper.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/netdev_query.py` & `xpra-4.4.5/xpra/platform/netdev_query.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/paths.py` & `xpra-4.4.5/xpra/platform/paths.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/printing.py` & `xpra-4.4.5/xpra/platform/printing.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/pycups_printing.py` & `xpra-4.4.5/xpra/platform/pycups_printing.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/ui_thread_watcher.py` & `xpra-4.4.5/xpra/platform/ui_thread_watcher.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/webcam.py` & `xpra-4.4.5/xpra/platform/webcam.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/__init__.py` & `xpra-4.4.5/xpra/platform/win32/__init__.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/clipboard.py` & `xpra-4.4.5/xpra/platform/win32/clipboard.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/common.py` & `xpra-4.4.5/xpra/platform/win32/common.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/comtypes_util.py` & `xpra-4.4.5/xpra/platform/win32/comtypes_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/constants.py` & `xpra-4.4.5/xpra/platform/win32/constants.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/create_process_lib.py` & `xpra-4.4.5/xpra/platform/win32/create_process_lib.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/desktoplogon_lib.py` & `xpra-4.4.5/xpra/platform/win32/desktoplogon_lib.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/directsound.py` & `xpra-4.4.5/xpra/platform/win32/directsound.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/dotxpra.py` & `xpra-4.4.5/xpra/platform/win32/dotxpra.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/dpi.py` & `xpra-4.4.5/xpra/platform/win32/dpi.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/dwm_color.py` & `xpra-4.4.5/xpra/platform/win32/dwm_color.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/features.py` & `xpra-4.4.5/xpra/platform/win32/features.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/gdi_screen_capture.py` & `xpra-4.4.5/xpra/platform/win32/gdi_screen_capture.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/gl_context.py` & `xpra-4.4.5/xpra/platform/win32/gl_context.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/glwin32.py` & `xpra-4.4.5/xpra/platform/win32/glwin32.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/gui.py` & `xpra-4.4.5/xpra/platform/win32/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1090,14 +1090,17 @@
         ALL_KEY_EVENTS = {win32con.WM_KEYDOWN       : "KEYDOWN",
                           win32con.WM_SYSKEYDOWN    : "SYSKEYDOWN",
                           win32con.WM_KEYUP         : "KEYUP",
                           win32con.WM_SYSKEYUP      : "SYSKEYUP",
                           }
         def low_level_keyboard_handler(nCode, wParam, lParam):
             log("WH_KEYBOARD_LL: %s", (nCode, wParam, lParam))
+            if nCode<0:
+                #docs say we should not process this event:
+                return CallNextHookEx(0, nCode, wParam, lParam)
             try:
                 scan_code = lParam.contents.scan_code
                 vk_code = lParam.contents.vk_code
                 focused = self.client._focused
                 #the keys we intercept before the OS:
                 keyname = {
                            win32con.VK_LWIN   : "Super_L",
```

### Comparing `xpra-4.4.4/xpra/platform/win32/icon_util.py` & `xpra-4.4.5/xpra/platform/win32/icon_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/info.py` & `xpra-4.4.5/xpra/platform/win32/info.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/keyboard.py` & `xpra-4.4.5/xpra/platform/win32/keyboard.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/keyboard_config.py` & `xpra-4.4.5/xpra/platform/win32/keyboard_config.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/lsa_logon_lib.py` & `xpra-4.4.5/xpra/platform/win32/lsa_logon_lib.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/menu_helper.py` & `xpra-4.4.5/xpra/platform/win32/menu_helper.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/namedpipes/common.py` & `xpra-4.4.5/xpra/platform/win32/namedpipes/common.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/namedpipes/connection.py` & `xpra-4.4.5/xpra/platform/win32/namedpipes/connection.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/namedpipes/listener.py` & `xpra-4.4.5/xpra/platform/win32/namedpipes/listener.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/netdev_query.py` & `xpra-4.4.5/xpra/platform/win32/netdev_query.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/paths.py` & `xpra-4.4.5/xpra/platform/win32/paths.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/pdfium.py` & `xpra-4.4.5/xpra/platform/win32/pdfium.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/printer_notify.py` & `xpra-4.4.5/xpra/platform/win32/printer_notify.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/printing.py` & `xpra-4.4.5/xpra/platform/win32/printing.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/propsys.pyx` & `xpra-4.4.5/xpra/platform/win32/propsys.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/proxy_server.py` & `xpra-4.4.5/xpra/platform/win32/proxy_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/scripts/exec.py` & `xpra-4.4.5/xpra/platform/win32/scripts/exec.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/scripts/execfile.py` & `xpra-4.4.5/xpra/platform/win32/scripts/execfile.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/scripts/shadow_server.py` & `xpra-4.4.5/xpra/platform/win32/scripts/shadow_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/setappid.cpp` & `xpra-4.4.5/xpra/platform/win32/setappid.cpp`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/shadow_server.py` & `xpra-4.4.5/xpra/platform/win32/shadow_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,14 +196,16 @@
                     if NVFBC_CUDA:
                         from xpra.codecs.nvfbc.fbc_capture_win import NvFBC_CUDACapture #@UnresolvedImport
                         capture = NvFBC_CUDACapture()
                     else:
                         from xpra.codecs.nvfbc.fbc_capture_win import NvFBC_SysCapture  #@UnresolvedImport
                         capture = NvFBC_SysCapture()
                     capture.init_context(w, h, pixel_format)
+                    #this will test the capture and ensure we can call get_image()
+                    capture.refresh()
             except Exception as e:
                 capture = None
                 log("NvFBC_Capture", exc_info=True)
                 log.warn("Warning: NvFBC screen capture initialization failed:")
                 for x in str(e).replace(". ", ":").split(":"):
                     if x.strip() and x!="nvfbc":
                         log.warn(" %s", x.strip())
```

### Comparing `xpra-4.4.4/xpra/platform/win32/webcam.py` & `xpra-4.4.5/xpra/platform/win32/webcam.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/win32_NotifyIcon.py` & `xpra-4.4.5/xpra/platform/win32/win32_NotifyIcon.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/win32_balloon.py` & `xpra-4.4.5/xpra/platform/win32/win32_balloon.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/win32_events.py` & `xpra-4.4.5/xpra/platform/win32/win32_events.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/win32_notifier.py` & `xpra-4.4.5/xpra/platform/win32/win32_notifier.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/win32_printing.py` & `xpra-4.4.5/xpra/platform/win32/win32_printing.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/win32_tray.py` & `xpra-4.4.5/xpra/platform/win32/win32_tray.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/win32_webcam.py` & `xpra-4.4.5/xpra/platform/win32/win32_webcam.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/window_hooks.py` & `xpra-4.4.5/xpra/platform/win32/window_hooks.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/wndproc_events.py` & `xpra-4.4.5/xpra/platform/win32/wndproc_events.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/win32/wtsapi.py` & `xpra-4.4.5/xpra/platform/win32/wtsapi.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/xposix/appindicator_tray.py` & `xpra-4.4.5/xpra/platform/xposix/appindicator_tray.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,16 +19,20 @@
 from xpra.util import envbool
 from xpra.os_util import osexpand
 from xpra.client.tray_base import TrayBase
 from xpra.platform.paths import get_icon_dir, get_icon_filename, get_xpra_tmp_dir
 from xpra.log import Logger
 
 import gi
-gi.require_version('AppIndicator3', '0.1')
-from gi.repository import AppIndicator3 #pylint: disable=wrong-import-order, wrong-import-position, ungrouped-imports
+try:
+    gi.require_version("AyatanaAppIndicator3", "0.1")  # @UndefinedVariable
+    from gi.repository import AyatanaAppIndicator3 as AppIndicator3 #pylint: disable=wrong-import-order, wrong-import-position, ungrouped-imports
+except ImportError:
+    gi.require_version("AppIndicator3", "0.1")  # @UndefinedVariable
+    from gi.repository import AppIndicator3 #pylint: disable=wrong-import-order, wrong-import-position, ungrouped-imports
 
 log = Logger("tray", "posix")
 
 DELETE_TEMP_FILE = envbool("XPRA_APPINDICATOR_DELETE_TEMP_FILE", True)
 
 PASSIVE = AppIndicator3.IndicatorStatus.PASSIVE
 ACTIVE = AppIndicator3.IndicatorStatus.ACTIVE
```

### Comparing `xpra-4.4.4/xpra/platform/xposix/autostart.py` & `xpra-4.4.5/xpra/platform/xposix/autostart.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/xposix/features.py` & `xpra-4.4.5/xpra/platform/xposix/features.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/xposix/gl_context.py` & `xpra-4.4.5/xpra/platform/xposix/gl_context.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/xposix/gui.py` & `xpra-4.4.5/xpra/platform/xposix/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,18 @@
         for setting_type, prop_name, value, _ in values:
             d[bytestostr(prop_name)] = (setting_type, value)
     return d
 
 
 def _get_xsettings_dpi():
     if XSETTINGS_DPI and is_X11():
-        from xpra.x11.xsettings_prop import XSettingsTypeInteger
+        try:
+            from xpra.x11.xsettings_prop import XSettingsTypeInteger
+        except ImportError:
+            return -1
         d = _get_xsettings_dict()
         for k,div in {
             "Xft.dpi"         : 1,
             "Xft/DPI"         : 1024,
             "gnome.Xft/DPI"   : 1024,
             #"Gdk/UnscaledDPI" : 1024, ??
             }.items():
```

### Comparing `xpra-4.4.4/xpra/platform/xposix/keyboard.py` & `xpra-4.4.5/xpra/platform/xposix/keyboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 
     def do_get_keymap_modifiers(self):
         if not self.keyboard_bindings:
             log.warn("keyboard bindings are not available")
             log.warn(" expect keyboard mapping problems")
             if is_Wayland():
                 log.warn(" (incomplete wayland support)")
+                return {}, [], ["mod2", ]
             return {}, [], []
         try:
             with xsync:
                 mod_mappings = self.keyboard_bindings.get_modifier_mappings()
                 if mod_mappings:
                     #ie: {"shift" : ["Shift_L", "Shift_R"], "mod1" : "Meta_L", ...]}
                     log("modifier mappings=%s", mod_mappings)
```

### Comparing `xpra-4.4.4/xpra/platform/xposix/menu_helper.py` & `xpra-4.4.5/xpra/platform/xposix/menu_helper.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/xposix/netdev_query.pyx` & `xpra-4.4.5/xpra/platform/xposix/netdev_query.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/xposix/paths.py` & `xpra-4.4.5/xpra/platform/xposix/paths.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/xposix/proc.pyx` & `xpra-4.4.5/xpra/platform/xposix/proc.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/xposix/sd_listen.pyx` & `xpra-4.4.5/xpra/platform/xposix/sd_listen.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/platform/xposix/webcam.py` & `xpra-4.4.5/xpra/platform/xposix/webcam.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/queue_scheduler.py` & `xpra-4.4.5/xpra/queue_scheduler.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/rectangle.pyx` & `xpra-4.4.5/xpra/rectangle.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/scripts/bug_report.py` & `xpra-4.4.5/xpra/scripts/bug_report.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/scripts/config.py` & `xpra-4.4.5/xpra/scripts/config.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/scripts/fdproxy.py` & `xpra-4.4.5/xpra/scripts/fdproxy.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/scripts/gtk_info.py` & `xpra-4.4.5/xpra/scripts/gtk_info.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/scripts/main.py` & `xpra-4.4.5/xpra/scripts/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,29 +105,43 @@
     from xpra.platform import clean as platform_clean, command_error, command_info
     if len(cmdline)==1:
         cmdline.append("gui")
 
     #turn off gdk scaling to make sure we get the actual window geometry:
     os.environ["GDK_SCALE"]="1"
     os.environ["GDK_DPI_SCALE"] = "1"
-    if WIN32 and os.environ.get("CRYPTOGRAPHY_OPENSSL_NO_LEGACY") is None:
+    if (WIN32 or OSX) and os.environ.get("CRYPTOGRAPHY_OPENSSL_NO_LEGACY") is None:
         os.environ["CRYPTOGRAPHY_OPENSSL_NO_LEGACY"] = "1"
     #client side decorations break window geometry,
     #disable this "feature" unless explicitly enabled:
     if os.environ.get("GTK_CSD") is None:
         os.environ["GTK_CSD"] = "0"
     if POSIX and not OSX and os.environ.get("XDG_SESSION_TYPE", "x11")=="x11" and not os.environ.get("GDK_BACKEND"):
         os.environ["GDK_BACKEND"] = "x11"
 
     if envbool("XPRA_NOMD5", False):
         import hashlib
-        def nomd5(*_args):
-            raise ValueError("md5 support is disabled")
-        hashlib.algorithms_available.remove("md5")
-        hashlib.md5 = nomd5
+        try:
+            hashlib.algorithms_available.remove("md5")  # @UndefinedVariable
+        except KeyError:
+            pass
+        else:
+            def nomd5(*_args):
+                raise ValueError("md5 support is disabled")
+            hashlib.md5 = nomd5
+    if envbool("XPRA_NOSHA1", False):
+        import hashlib  # @Reimport
+        try:
+            hashlib.algorithms_available.remove("sha1")  # @UndefinedVariable
+        except KeyError:
+            pass
+        else:
+            def nosha1(*_args):
+                raise ValueError("sha1 support is disabled")
+            hashlib.sha1 = nosha1
 
     def debug_exc(msg="run_mode error"):
         get_util_logger().debug(msg, exc_info=True)
 
     try:
         defaults = make_defaults_struct()
         fixup_defaults(defaults)
@@ -282,21 +296,21 @@
         cmd += shlex.split(systemd_run_args)
     return cmd
 
 def systemd_run_wrap(mode, args, systemd_run_args=None, **kwargs):
     cmd = systemd_run_command(mode, systemd_run_args)
     cmd += args
     cmd.append("--systemd-run=no")
-    stderr = sys.stderr
+    werr = getattr(sys.stderr, "write", None)
     LOG_SYSTEMD_WRAP = envbool("XPRA_LOG_SYSTEMD_WRAP", True)
-    if LOG_SYSTEMD_WRAP:
-        noerr(stderr.write, f"using systemd-run to wrap {mode!r} server command\n")
+    if LOG_SYSTEMD_WRAP and werr:
+        noerr(werr, f"using systemd-run to wrap {mode!r} xpra server subcommand\n")
     LOG_SYSTEMD_WRAP_COMMAND = envbool("XPRA_LOG_SYSTEMD_WRAP_COMMAND", False)
-    if LOG_SYSTEMD_WRAP_COMMAND:
-        noerr(stderr.write, "%s\n" % " ".join(["'%s'" % x for x in cmd]))
+    if LOG_SYSTEMD_WRAP_COMMAND and werr:
+        noerr(werr, "%s\n" % " ".join(["'%s'" % x for x in cmd]))
     try:
         with Popen(cmd, **kwargs) as p:
             return p.wait()
     except KeyboardInterrupt:
         return 128+signal.SIGINT
 
 
@@ -1443,15 +1457,15 @@
         if opts.encoding:
             err = opts.encoding and (opts.encoding not in app.get_encodings())
             einfo = ""
             if err and opts.encoding!="help":
                 einfo = f"invalid encoding: {opts.encoding}\n"
             if opts.encoding=="help" or err:
                 from xpra.codecs.loader import encodings_help
-                encodings = ["auto"] + app.get_encodings()
+                encodings = ["auto"] + list(app.get_encodings())
                 raise InitInfo(einfo+"%s xpra client supports the following encodings:\n * %s" %
                                (app.client_toolkit(), "\n * ".join(encodings_help(encodings))))
         def handshake_complete(*_args):
             app.show_progress(100, "connection established")
             log = get_util_logger()
             try:
                 p = app._protocol
@@ -1487,15 +1501,15 @@
                 )
             sockets = create_sockets(opts, error_cb)
             #we don't have a display,
             #so we can't automatically create sockets:
             if "auto" in opts.bind:
                 opts.bind.remove("auto")
             local_sockets = setup_local_sockets(opts.bind,
-                                                opts.socket_dir, opts.socket_dirs,
+                                                opts.socket_dir, opts.socket_dirs, None,
                                                 None, False,
                                                 opts.mmap_group, opts.socket_permissions,
                                                 get_username(), getuid, getgid)
             sockets.update(local_sockets)
             listen_cleanup = []
             socket_cleanup = []
             def new_connection(socktype, sock, handle=0):
```

### Comparing `xpra-4.4.4/xpra/scripts/parsing.py` & `xpra-4.4.5/xpra/scripts/parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,15 +413,15 @@
     #but the separator value we use thereafter can only be ":" or "/"
     #because we want strings like ssl://host:port/DISPLAY to be parsed into ["ssl", "host:port", "DISPLAY"]
     psep = ""
     if display_name[pos]==":":
         psep += ":"
         pos += 1
     scount = 0
-    while display_name[pos]=="/" and scount<2:
+    while pos<len(display_name) and display_name[pos]=="/" and scount<2:
         psep += "/"
         pos += 1
         scount += 1
     if protocol=="socket":
         #socket paths may start with a slash!
         #so socket:/path means that the slash is part of the path
         if psep==":/":
@@ -1836,16 +1836,16 @@
     return options, args
 
 def validated_encodings(encodings):
     try:
         from xpra.codecs.codec_constants import PREFERRED_ENCODING_ORDER
     except ImportError:
         return []
-    lower_encodings = [x.lower() for x in encodings]
-    validated = [x for x in PREFERRED_ENCODING_ORDER if x.lower() in lower_encodings]
+    encodings = [x.lower() for x in encodings] + list(encodings)
+    validated = [x for x in PREFERRED_ENCODING_ORDER if x in encodings]
     if not validated:
         raise InitException("no valid encodings specified")
     return validated
 
 def validate_encryption(opts):
     do_validate_encryption(opts.auth, opts.tcp_auth,
                            opts.encryption, opts.tcp_encryption, opts.encryption_keyfile, opts.tcp_encryption_keyfile)
```

### Comparing `xpra-4.4.4/xpra/scripts/pinentry_wrapper.py` & `xpra-4.4.5/xpra/scripts/pinentry_wrapper.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/scripts/server.py` & `xpra-4.4.5/xpra/scripts/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1394,15 +1394,15 @@
         gui_init()
 
     def init_local_sockets():
         progress(60, "initializing local sockets")
         #setup unix domain socket:
         netlog = get_network_logger()
         local_sockets = setup_local_sockets(opts.bind,
-                                            opts.socket_dir, opts.socket_dirs,
+                                            opts.socket_dir, opts.socket_dirs, session_dir,
                                             display_name, clobber,
                                             opts.mmap_group, opts.socket_permissions,
                                             username, uid, gid)
         netlog(f"setting up local sockets: {local_sockets}")
         sockets.update(local_sockets)
         if POSIX and (starting or upgrading or starting_desktop):
             #all unix domain sockets:
```

### Comparing `xpra-4.4.4/xpra/scripts/show_webcam.py` & `xpra-4.4.5/xpra/scripts/show_webcam.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/scripts/version.py` & `xpra-4.4.5/xpra/scripts/version.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/scripts/win32_service.py` & `xpra-4.4.5/xpra/scripts/win32_service.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/allow_auth.py` & `xpra-4.4.5/xpra/server/auth/allow_auth.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/auth_helper.py` & `xpra-4.4.5/xpra/server/auth/auth_helper.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/capability_auth.py` & `xpra-4.4.5/xpra/server/auth/capability_auth.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/env_auth.py` & `xpra-4.4.5/xpra/server/auth/env_auth.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/exec_auth.py` & `xpra-4.4.5/xpra/server/auth/exec_auth.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/file_auth.py` & `xpra-4.4.5/xpra/server/auth/file_auth.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/file_auth_base.py` & `xpra-4.4.5/xpra/server/auth/file_auth_base.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/gss_auth.py` & `xpra-4.4.5/xpra/server/auth/gss_auth.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/hosts_auth.py` & `xpra-4.4.5/xpra/server/auth/hosts_auth.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/kerberos_password_auth.py` & `xpra-4.4.5/xpra/server/auth/kerberos_password_auth.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/kerberos_token_auth.py` & `xpra-4.4.5/xpra/server/auth/kerberos_token_auth.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/keycloak_auth.py` & `xpra-4.4.5/xpra/server/auth/keycloak_auth.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/ldap3_auth.py` & `xpra-4.4.5/xpra/server/auth/ldap3_auth.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/ldap_auth.py` & `xpra-4.4.5/xpra/server/auth/ldap_auth.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/multifile_auth.py` & `xpra-4.4.5/xpra/server/auth/multifile_auth.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/mysql_auth.py` & `xpra-4.4.5/xpra/server/auth/mysql_auth.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/none_auth.py` & `xpra-4.4.5/xpra/server/auth/none_auth.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/otp_auth.py` & `xpra-4.4.5/xpra/server/auth/otp_auth.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/pam_auth.py` & `xpra-4.4.5/xpra/server/auth/pam_auth.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/password_auth.py` & `xpra-4.4.5/xpra/server/auth/password_auth.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/peercred_auth.py` & `xpra-4.4.5/xpra/server/auth/peercred_auth.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/reject_auth.py` & `xpra-4.4.5/xpra/server/auth/reject_auth.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/sql_auth.py` & `xpra-4.4.5/xpra/server/auth/sql_auth.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/sqlauthbase.py` & `xpra-4.4.5/xpra/server/auth/sqlauthbase.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/sqlite_auth.py` & `xpra-4.4.5/xpra/server/auth/sqlite_auth.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/sys_auth_base.py` & `xpra-4.4.5/xpra/server/auth/sys_auth_base.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/u2f_auth.py` & `xpra-4.4.5/xpra/server/auth/u2f_auth.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/auth/win32_auth.py` & `xpra-4.4.5/xpra/server/auth/win32_auth.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/background_worker.py` & `xpra-4.4.5/xpra/server/background_worker.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/control_command.py` & `xpra-4.4.5/xpra/server/control_command.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/cystats.pyx` & `xpra-4.4.5/xpra/server/cystats.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/dbus/dbus_common.py` & `xpra-4.4.5/xpra/server/dbus/dbus_common.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/dbus/dbus_server.py` & `xpra-4.4.5/xpra/server/dbus/dbus_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/dbus/dbus_server_base.py` & `xpra-4.4.5/xpra/server/dbus/dbus_server_base.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/dbus/dbus_source.py` & `xpra-4.4.5/xpra/server/dbus/dbus_source.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/dbus/dbus_start.py` & `xpra-4.4.5/xpra/server/dbus/dbus_start.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/gtk_server_base.py` & `xpra-4.4.5/xpra/server/gtk_server_base.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/keyboard_config_base.py` & `xpra-4.4.5/xpra/server/keyboard_config_base.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/menu_provider.py` & `xpra-4.4.5/xpra/server/menu_provider.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/mixins/audio_server.py` & `xpra-4.4.5/xpra/server/mixins/audio_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/mixins/child_command_server.py` & `xpra-4.4.5/xpra/server/mixins/child_command_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/mixins/clipboard_server.py` & `xpra-4.4.5/xpra/server/mixins/clipboard_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/mixins/dbusrpc_server.py` & `xpra-4.4.5/xpra/server/mixins/dbusrpc_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/mixins/display_manager.py` & `xpra-4.4.5/xpra/server/mixins/display_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 # This file is part of Xpra.
-# Copyright (C) 2010-2022 Antoine Martin <antoine@xpra.org>
+# Copyright (C) 2010-2023 Antoine Martin <antoine@xpra.org>
 # Xpra is released under the terms of the GNU GPL v2, or, at your option, any
 # later version. See the file COPYING for details.
 
 from xpra.util import engs, log_screen_sizes
 from xpra.os_util import bytestostr
-from xpra.scripts.config import FALSE_OPTIONS
+from xpra.scripts.config import FALSE_OPTIONS, TRUE_OPTIONS
 from xpra.common import get_refresh_rate_for_value, FULL_INFO
 from xpra.server.mixins.stub_server_mixin import StubServerMixin
 from xpra.log import Logger
 
 log = Logger("screen")
 gllog = Logger("opengl")
 
@@ -87,15 +87,15 @@
                     parts = line.split(b"=")
                     if len(parts)!=2:
                         continue
                     k = bytestostr(parts[0].strip())
                     v = bytestostr(parts[1].strip())
                     props[k] = v
                 gllog("opengl props=%s", props)
-                if props:
+                if props and props.get("success", "").lower() in TRUE_OPTIONS:
                     gllog.info(f"OpenGL is supported on display {self.display_name!r}")
                     renderer = props.get("renderer")
                     if renderer:
                         gllog.info(f" using {renderer!r} renderer")
                 else:
                     gllog.info("No OpenGL information available")
             else:
```

### Comparing `xpra-4.4.4/xpra/server/mixins/encoding_server.py` & `xpra-4.4.5/xpra/server/mixins/encoding_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/mixins/fileprint_server.py` & `xpra-4.4.5/xpra/server/mixins/fileprint_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/mixins/input_server.py` & `xpra-4.4.5/xpra/server/mixins/input_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/mixins/logging_server.py` & `xpra-4.4.5/xpra/server/mixins/logging_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/mixins/mmap_server.py` & `xpra-4.4.5/xpra/server/mixins/mmap_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/mixins/networkstate_server.py` & `xpra-4.4.5/xpra/server/mixins/networkstate_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/mixins/notification_forwarder.py` & `xpra-4.4.5/xpra/server/mixins/notification_forwarder.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/mixins/server_base_controlcommands.py` & `xpra-4.4.5/xpra/server/mixins/server_base_controlcommands.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/mixins/shell_server.py` & `xpra-4.4.5/xpra/server/mixins/shell_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/mixins/stub_server_mixin.py` & `xpra-4.4.5/xpra/server/mixins/stub_server_mixin.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/mixins/webcam_server.py` & `xpra-4.4.5/xpra/server/mixins/webcam_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/mixins/window_server.py` & `xpra-4.4.5/xpra/server/mixins/window_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/pam.pyx` & `xpra-4.4.5/xpra/server/pam.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/proxy/proxy_dbus_server.py` & `xpra-4.4.5/xpra/server/proxy/proxy_dbus_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/proxy/proxy_instance.py` & `xpra-4.4.5/xpra/server/proxy/proxy_instance.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/proxy/proxy_instance_process.py` & `xpra-4.4.5/xpra/server/proxy/proxy_instance_process.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/proxy/proxy_instance_thread.py` & `xpra-4.4.5/xpra/server/proxy/proxy_instance_thread.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/proxy/proxy_server.py` & `xpra-4.4.5/xpra/server/proxy/proxy_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/rfb/rfb_protocol.py` & `xpra-4.4.5/xpra/server/rfb/rfb_protocol.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/rfb/rfb_server.py` & `xpra-4.4.5/xpra/server/rfb/rfb_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/rfb/rfb_source.py` & `xpra-4.4.5/xpra/server/rfb/rfb_source.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/server_base.py` & `xpra-4.4.5/xpra/server/server_base.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/server_core.py` & `xpra-4.4.5/xpra/server/server_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,14 +212,15 @@
         self.tcp_encryption_keyfile = None
         self.password_file = None
         self.compression_level = 1
         self.exit_with_client = False
         self.server_idle_timeout = 0
         self.server_idle_timer = None
         self.bandwidth_limit = 0
+        self.readonly = False
 
         self.init_thread = None
         self.init_thread_callbacks = []
         self.init_thread_lock = Lock()
         self.menu_provider = None
 
         self.init_uuid()
```

### Comparing `xpra-4.4.4/xpra/server/server_features.py` & `xpra-4.4.5/xpra/server/server_features.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/server_util.py` & `xpra-4.4.5/xpra/server/server_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/server_uuid.py` & `xpra-4.4.5/xpra/server/server_uuid.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/shadow/gtk_root_window_model.py` & `xpra-4.4.5/xpra/server/shadow/gtk_root_window_model.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/shadow/gtk_shadow_server_base.py` & `xpra-4.4.5/xpra/server/shadow/gtk_shadow_server_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,14 +366,15 @@
             self.tray_menu.append(self.traymenuitem("Close Menu", "close.png", None, self.close_tray_menu))
             #maybe add: session info, clipboard, sharing, etc
             #control: disconnect clients
             self.tray_menu.connect("deactivate", self.tray_menu_deactivated)
             self.tray_widget = self.make_tray_widget()
             self.set_tray_icon(self.tray_icon  or "server-notconnected")
         except ImportError as e:
+            traylog("setup_tray()", exc_info=True)
             traylog.warn("Warning: failed to load systemtray:")
             traylog.warn(" %s", e)
         except Exception as e:
             traylog("error setting up %s", self.tray_widget, exc_info=True)
             traylog.error("Error setting up system tray:")
             traylog.error(" %s", e)
```

### Comparing `xpra-4.4.4/xpra/server/shadow/root_window_model.py` & `xpra-4.4.5/xpra/server/shadow/root_window_model.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/shadow/shadow_dbus_server.py` & `xpra-4.4.5/xpra/server/shadow/shadow_dbus_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/shadow/shadow_server_base.py` & `xpra-4.4.5/xpra/server/shadow/shadow_server_base.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/source/audio_mixin.py` & `xpra-4.4.5/xpra/server/source/audio_mixin.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/source/avsync_mixin.py` & `xpra-4.4.5/xpra/server/source/avsync_mixin.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/source/client_connection.py` & `xpra-4.4.5/xpra/server/source/client_connection.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/source/client_connection_factory.py` & `xpra-4.4.5/xpra/server/source/client_connection_factory.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/source/clientdisplay_mixin.py` & `xpra-4.4.5/xpra/server/source/clientdisplay_mixin.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/source/clientinfo_mixin.py` & `xpra-4.4.5/xpra/server/source/clientinfo_mixin.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/source/clipboard_connection.py` & `xpra-4.4.5/xpra/server/source/clipboard_connection.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/source/dbus_mixin.py` & `xpra-4.4.5/xpra/server/source/dbus_mixin.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/source/encodings_mixin.py` & `xpra-4.4.5/xpra/server/source/encodings_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     """
     Store information about the client's support for encodings.
     Runs the encode thread.
     """
 
     @classmethod
     def is_needed(cls, caps : typedict) -> bool:
-        return bool(caps.strtupleget("encodings"))
+        return bool(caps.strtupleget("encodings")) or caps.boolget("windows")
 
     def init_state(self):
         #contains default values, some of which may be supplied by the client:
         self.default_batch_config = batch_config.DamageBatchConfig()
         self.global_batch_config = self.default_batch_config.clone()      #global batch config
 
         self.supports_transparency = False
```

### Comparing `xpra-4.4.4/xpra/server/source/fileprint_mixin.py` & `xpra-4.4.5/xpra/server/source/fileprint_mixin.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/source/idle_mixin.py` & `xpra-4.4.5/xpra/server/source/idle_mixin.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/source/input_mixin.py` & `xpra-4.4.5/xpra/server/source/input_mixin.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/source/mmap_connection.py` & `xpra-4.4.5/xpra/server/source/mmap_connection.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/source/networkstate_mixin.py` & `xpra-4.4.5/xpra/server/source/networkstate_mixin.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/source/notification_mixin.py` & `xpra-4.4.5/xpra/server/source/notification_mixin.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/source/shell_mixin.py` & `xpra-4.4.5/xpra/server/source/shell_mixin.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/source/source_stats.py` & `xpra-4.4.5/xpra/server/source/source_stats.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/source/stub_source_mixin.py` & `xpra-4.4.5/xpra/server/source/stub_source_mixin.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/source/webcam_mixin.py` & `xpra-4.4.5/xpra/server/source/webcam_mixin.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/source/windows_mixin.py` & `xpra-4.4.5/xpra/server/source/windows_mixin.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/ssh.py` & `xpra-4.4.5/xpra/server/ssh.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/window/batch_config.py` & `xpra-4.4.5/xpra/server/window/batch_config.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/window/batch_delay_calculator.py` & `xpra-4.4.5/xpra/server/window/batch_delay_calculator.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/window/content_guesser.py` & `xpra-4.4.5/xpra/server/window/content_guesser.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/window/filters.py` & `xpra-4.4.5/xpra/server/window/filters.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/window/metadata.py` & `xpra-4.4.5/xpra/server/window/metadata.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/window/motion.pyx` & `xpra-4.4.5/xpra/server/window/motion.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/window/video_scoring.py` & `xpra-4.4.5/xpra/server/window/video_scoring.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/window/video_subregion.py` & `xpra-4.4.5/xpra/server/window/video_subregion.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/window/window_source.py` & `xpra-4.4.5/xpra/server/window/window_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -750,19 +750,21 @@
             window, args, self._encoding_hint, self.get_best_encoding)
         return True
 
     def window_type_changed(self, window, *args):
         self.window_type = set(window.get_property("window-type"))
         log("window_type_changed(window, %s) window_type=%s", window, args, self.window_type)
         self.assign_encoding_getter()
+        return True
 
     def window_opaque_region_changed(self, window, *args):
         self._opaque_region = window.get_property("opaque-region") or ()
         log("window_opaque_region_changed(%s, %s) opaque-region=%s", window, args, self._opaque_region)
         self.update_encoding_options()
+        return True
 
     def set_client_properties(self, properties):
         #filter out stuff we don't care about
         #to see if there is anything to set at all,
         #and if not, don't bother doing the potentially expensive update_encoding_selection()
         for k in ("workspace", b"workspace", "screen", b"screen"):
             properties.pop(k, None)
@@ -958,15 +960,15 @@
         #choose which method to use for selecting an encoding
         #first the easy ones (when there is no choice):
         if self._mmap_size>0 and self.encoding!="grayscale":
             return self.encoding_is_mmap
         if self.encoding=="png/L":
             #(png/L would look awful if we mixed it with something else)
             return self.encoding_is_pngL
-        if self.image_depth==8:
+        if self.image_depth==8 or self.encoding=="png/P":
             #limited options:
             if self.encoding=="grayscale":
                 assert "png/L" in self.common_encodings
                 return self.encoding_is_pngL
             assert "png/P" in self.common_encodings
             return self.encoding_is_pngP
         if self.strict and self.encoding!="auto":
```

### Comparing `xpra-4.4.4/xpra/server/window/window_stats.py` & `xpra-4.4.5/xpra/server/window/window_stats.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/server/window/window_video_source.py` & `xpra-4.4.5/xpra/server/window/window_video_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -545,16 +545,18 @@
     def get_best_nonvideo_encoding(self, ww, wh, options, current_encoding=None, encoding_options=()):
         if self.encoding=="grayscale":
             return self.encoding_is_grayscale(ww, wh, options, current_encoding or self.encoding)
         #if we're here, then the window has no alpha (or the client cannot handle alpha)
         #and we can ignore the current encoding
         encoding_options = encoding_options or self.non_video_encodings
         depth = self.image_depth
-        if depth==8 and "png/P" in encoding_options:
+        if (depth==8 and "png/P" in encoding_options) or self.encoding=="png/P":
             return "png/P"
+        if self.encoding=="png/L":
+            return "png/L"
         if self._mmap_size>0:
             return "mmap"
         return super().do_get_auto_encoding(ww, wh, options, current_encoding or self.encoding, encoding_options)
 
 
     def do_damage(self, ww, wh, x, y, w, h, options):
         vs = self.video_subregion
@@ -2011,17 +2013,20 @@
             compresslog(COMPRESS_SCROLL_FMT,
                  (end-start)*1000.0, w, h, x, y, self.wid, coding,
                  len(scrolls), w*h*4/1024,
                  self._damage_packet_sequence, client_options, options)
         del scrolls
         #send the rest as rectangles:
         if non_scroll:
+            if self.content_type.find("text")>=0:
+                quality = 100
+                options["quality"] = quality
             #boost quality a bit, because lossless saves refreshing,
             #more so if we have a high match percentage (less to send):
-            if self._fixed_quality<=0:
+            elif self._fixed_quality<=0:
                 quality = options.get("quality", self._current_quality)
                 quality = min(100, quality + max(60, match_pct)//2)
                 options["quality"] = quality
             nsstart = monotonic()
             client_options = options.copy()
             for sy, sh in non_scroll.items():
                 substart = monotonic()
```

### Comparing `xpra-4.4.4/xpra/server/window/windowicon_source.py` & `xpra-4.4.5/xpra/server/window/windowicon_source.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/simple_stats.py` & `xpra-4.4.5/xpra/simple_stats.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/sound/common.py` & `xpra-4.4.5/xpra/sound/common.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/sound/gstreamer_util.py` & `xpra-4.4.5/xpra/sound/gstreamer_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/sound/pulseaudio/pulseaudio_common_util.py` & `xpra-4.4.5/xpra/sound/pulseaudio/pulseaudio_common_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/sound/pulseaudio/pulseaudio_none_util.py` & `xpra-4.4.5/xpra/sound/pulseaudio/pulseaudio_none_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/sound/pulseaudio/pulseaudio_pactl_util.py` & `xpra-4.4.5/xpra/sound/pulseaudio/pulseaudio_pactl_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/sound/pulseaudio/pulseaudio_util.py` & `xpra-4.4.5/xpra/sound/pulseaudio/pulseaudio_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/sound/sink.py` & `xpra-4.4.5/xpra/sound/sink.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/sound/sound_pipeline.py` & `xpra-4.4.5/xpra/sound/sound_pipeline.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/sound/src.py` & `xpra-4.4.5/xpra/sound/src.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/sound/wrapper.py` & `xpra-4.4.5/xpra/sound/wrapper.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/util.py` & `xpra-4.4.5/xpra/util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/version_util.py` & `xpra-4.4.5/xpra/version_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/bindings/core_bindings.pyx` & `xpra-4.4.5/xpra/x11/bindings/core_bindings.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/bindings/display_source.pyx` & `xpra-4.4.5/xpra/x11/bindings/display_source.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/bindings/keyboard_bindings.pyx` & `xpra-4.4.5/xpra/x11/bindings/keyboard_bindings.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/bindings/posix_display_source.pyx` & `xpra-4.4.5/xpra/x11/bindings/posix_display_source.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/bindings/randr_bindings.pyx` & `xpra-4.4.5/xpra/x11/bindings/randr_bindings.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1119,24 +1119,24 @@
                             <uintptr_t> self.display, <uintptr_t> rsc, crtc,
                             CurrentTime, x, y, mode, RR_Rotate_0, <uintptr_t> &output, noutput)
                     r = XRRSetCrtcConfig(self.display, rsc, crtc,
                           CurrentTime, x, y, mode,
                           RR_Rotate_0, &output, noutput)
                     if r:
                         raise Exception(f"failed to set crtc config for monitor {i}")
-                    mmw = m.get("width-mm", dpi96(width))
-                    mmh = m.get("height-mm", dpi96(height))
+                    mmw = m.get("width-mm", 0) or dpi96(width)
+                    mmh = m.get("height-mm", 0) or dpi96(height)
                     self.set_output_int_property(i, "WIDTH_MM", mmw)
                     self.set_output_int_property(i, "HEIGHT_MM", mmh)
                     #this allows us to disconnect the output of this crtc:
                     self.set_output_int_property(i, "SUSPENDED", not bool(m))
                     posinfo = ""
                     if x or y:
                         posinfo = " at %i,%i" % (x, y)
-                    if width==height==mmw==mmh==0:
+                    if width==0 or height==0:
                         log.info(f"disabling dummy crtc and output {i}")
                     else:
                         log.info(f"setting dummy crtc and output {i} to {width}x{height} {hz}Hz ({mmw}x{mmh} mm){posinfo}")
                 finally:
                     if output_info:
                         XRRFreeOutputInfo(output_info)
                         output_info = NULL
```

### Comparing `xpra-4.4.4/xpra/x11/bindings/randr_info.py` & `xpra-4.4.5/xpra/x11/bindings/randr_info.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/bindings/res_bindings.pyx` & `xpra-4.4.5/xpra/x11/bindings/res_bindings.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/bindings/wait_for_x_server.pyx` & `xpra-4.4.5/xpra/x11/bindings/wait_for_x_server.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/bindings/window_bindings.pyx` & `xpra-4.4.5/xpra/x11/bindings/window_bindings.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 
 from xpra.x11.bindings.xlib cimport (
     Display, Drawable, Visual, Window, Bool, Pixmap, XID, Status, Atom, Time, CurrentTime, Cursor,
     GrabModeAsync, XGrabPointer,
     XRectangle, XEvent, XClassHint,
     XWMHints, XSizeHints,
+    XCreateWindow, XDestroyWindow,
+    XSetWindowAttributes,
     XWindowAttributes, XWindowChanges,
     XDefaultRootWindow,
     XInternAtom, XFree, XGetErrorText,
     XGetSelectionOwner, XSetSelectionOwner, XConvertSelection,
     XMapWindow, XMapRaised, XUnmapWindow, XWithdrawWindow, XReparentWindow, XIconifyWindow, XRaiseWindow,
     NextRequest, XSendEvent, XSelectInput, XAddToSaveSet, XRemoveFromSaveSet,
     XGetWindowAttributes, XGetWindowProperty, XDeleteProperty, XChangeProperty,
@@ -26,14 +28,16 @@
     XGetGeometry, XTranslateCoordinates, XConfigureWindow, XMoveResizeWindow,
     XGetInputFocus, XSetInputFocus,
     XAllocClassHint, XAllocSizeHints, XGetClassHint, XSetClassHint,
     XQueryTree,
     XKillClient,
     )
 from libc.stdlib cimport free, malloc       #pylint: disable=syntax-error
+from libc.string cimport memset
+
 
 ###################################
 # Headers, python magic
 ###################################
 
 ######
 # Xlib primitives and constants
@@ -44,23 +48,32 @@
 
 cdef extern from "X11/Xlib.h":
     int CWX
     int CWY
     int CWWidth
     int CWHeight
     int InputOnly
+    int InputOutput
     int RevertToParent
     int ClientMessage
     int ButtonPress
     int Button1
     int Button2
     int Button3
     int SelectionNotify
     int ConfigureNotify
 
+    int CopyFromParent
+
+    int CWEventMask
+    int CWColormap
+    int CWBorderWidth
+    int CWSibling
+    int CWStackMode
+
     int NoEventMask
     int KeyPressMask
     int KeyReleaseMask
     int ButtonPressMask
     int ButtonReleaseMask
     int EnterWindowMask
     int LeaveWindowMask
@@ -80,17 +93,14 @@
     int SubstructureNotifyMask
     int SubstructureRedirectMask
     int FocusChangeMask
     int PropertyChangeMask
     int ColormapChangeMask
     int OwnerGrabButtonMask
 
-    int CWBorderWidth
-    int CWSibling
-    int CWStackMode
     int AnyPropertyType
     int Success
     int PropModeReplace
     int USPosition
     int PPosition
     int USSize
     int PSize
@@ -867,14 +877,45 @@
         e.xconfigure.above = XNone
         e.xconfigure.override_redirect = attrs.override_redirect
 
         cdef Status s = XSendEvent(self.display, xwindow, False, StructureNotifyMask, &e)
         if s == 0:
             raise ValueError("failed to serialize ConfigureNotify")
 
+    def CreateCorralWindow(self, Window parent, Window xid, int x, int y):
+        self.context_check("CreateCorralWindow")
+        #copy most attributes from the window we will wrap:
+        cdef int ox, oy
+        cdef Window root
+        cdef unsigned int width, height, border_width, depth
+        if not XGetGeometry(self.display, xid, &root,
+                        &ox, &oy, &width, &height, &border_width, &depth):
+            return None
+        cdef XSetWindowAttributes attributes
+        memset(<void*> &attributes, 0, sizeof(XSetWindowAttributes))
+        # We enable PropertyChangeMask so that we can call
+        # get_server_time on this window.
+        attributes.event_mask = PropertyChangeMask | StructureNotifyMask | SubstructureNotifyMask
+        #get depth from parent window:
+        cdef int px, py
+        cdef unsigned int pw, ph, pborder, pdepth
+        if not XGetGeometry(self.display, parent, &root,
+                        &px, &py, &pw, &ph, &pborder, &pdepth):
+            return None
+        cdef unsigned long valuemask = CWEventMask
+        cdef Window window = XCreateWindow(self.display, parent,
+                                           x, y, width, height, 0, pdepth,
+                                           InputOutput, <Visual*> CopyFromParent,
+                                           valuemask, &attributes)
+        return window
+
+    def DestroyWindow(self, Window w):
+        self.context_check("DestroyWindow")
+        return XDestroyWindow(self.display, w)
+
     def ConfigureWindow(self, Window xwindow,
                         int x, int y, int width, int height, int border=0,
                         int sibling=0, int stack_mode=0,
                         int value_mask=CONFIGURE_GEOMETRY_MASK):
         self.context_check("ConfigureWindow")
         cdef XWindowChanges changes
         changes.x = x
```

### Comparing `xpra-4.4.4/xpra/x11/bindings/xi2_bindings.pyx` & `xpra-4.4.5/xpra/x11/bindings/xi2_bindings.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/bindings/ximage.pyx` & `xpra-4.4.5/xpra/x11/bindings/ximage.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/bindings/xlib.pxd` & `xpra-4.4.5/xpra/x11/bindings/xlib.pxd`

 * *Files 4% similar despite different names*

```diff
@@ -148,14 +148,31 @@
         int bits_per_rgb
 
     ctypedef struct XColor:
         unsigned long pixel                 # pixel value
         unsigned short red, green, blue     # rgb values
         char flags                          # DoRed, DoGreen, DoBlue
 
+    ctypedef struct XSetWindowAttributes:
+        Pixmap background_pixmap            # background, None, or ParentRelative
+        unsigned long background_pixel      # background pixel
+        Pixmap border_pixmap                # border of the window or CopyFromParent
+        unsigned long border_pixel          # border pixel value
+        int bit_gravity                     # one of bit gravity values
+        int win_gravity                     # one of the window gravity values
+        int backing_store                   # NotUseful, WhenMapped, Always
+        unsigned long backing_planes        # planes to be preserved if possible
+        unsigned long backing_pixel         # value to use in restoring planes
+        Bool save_under                     # should bits under be saved? (popups)
+        long event_mask                     # set of events that should be saved
+        long do_not_propagate_mask          # set of events that should not propagate
+        Bool override_redirect              # boolean value for override_redirect
+        Colormap colormap                   # color map to be associated with window
+        Cursor cursor
+
     ctypedef struct XWindowChanges:
         int x, y, width, height, border_width
         Window sibling
         int stack_mode
 
     ctypedef struct XWindowAttributes:
         int x, y, width, height, border_width
@@ -259,14 +276,20 @@
     int XAddToSaveSet(Display *, Window w)
     int XRemoveFromSaveSet(Display *, Window w)
 
     # windows:
     Status XGetWindowAttributes(Display * display, Window w,
                                 XWindowAttributes * attributes)
 
+    Window XCreateWindow(Display *display, Window parent,
+                         int x, int y, unsigned int width, unsigned int height, unsigned int border_width, int depth,
+                         unsigned int _class, Visual *visual,
+                         unsigned long valuemask, XSetWindowAttributes *attributes)
+    int XDestroyWindow(Display *display, Window w)
+
     int XConfigureWindow(Display * display, Window w,
          unsigned int value_mask, XWindowChanges * changes)
     Status XReconfigureWMWindow(Display * display, Window w, int screen_number,
                                 unsigned int value_mask, XWindowChanges *values)
     int XMoveResizeWindow(Display * display, Window w, int x, int y, int width, int height)
 
     Bool XTranslateCoordinates(Display * display,
@@ -429,14 +452,15 @@
         Window window
         Bool override_redirect
     ctypedef struct XUnmapEvent:
         Window window
     ctypedef struct XDestroyWindowEvent:
         Window window
     ctypedef struct XPropertyEvent:
+        Window window
         Atom atom
         Time time
     ctypedef struct XKeyEvent:
         unsigned int keycode, state
 
     ctypedef union XEvent:
         int type
```

### Comparing `xpra-4.4.4/xpra/x11/bindings/xwait.pyx` & `xpra-4.4.5/xpra/x11/bindings/xwait.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/common.py` & `xpra-4.4.5/xpra/x11/common.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/dbus/x11_dbus_server.py` & `xpra-4.4.5/xpra/x11/dbus/x11_dbus_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/desktop/desktop_model.py` & `xpra-4.4.5/xpra/x11/desktop/desktop_model.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/desktop/desktop_server.py` & `xpra-4.4.5/xpra/x11/desktop/desktop_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/desktop/desktop_server_base.py` & `xpra-4.4.5/xpra/x11/desktop/desktop_server_base.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/desktop/model_base.py` & `xpra-4.4.5/xpra/x11/desktop/model_base.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/desktop/monitor_model.py` & `xpra-4.4.5/xpra/x11/desktop/monitor_model.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/desktop/monitor_server.py` & `xpra-4.4.5/xpra/x11/desktop/monitor_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/expand_server.py` & `xpra-4.4.5/xpra/x11/expand_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/fakeXinerama.py` & `xpra-4.4.5/xpra/x11/fakeXinerama.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/gtk3/gdk_bindings.pyx` & `xpra-4.4.5/xpra/x11/gtk3/gdk_bindings.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -326,17 +326,18 @@
     if int(xatom) > 2**32:
         raise Exception("weirdly huge purported xatom: %s" % xatom)
     if xatom==0:
         return ""
     cdef GdkDisplay *disp = get_raw_display_for(display)
     cdef Display *xdisplay = GDK_DISPLAY_XDISPLAY(disp)
     cdef char *name = XGetAtomName(xdisplay, xatom)
-    if not name:
+    if name==NULL:
         return ""
     pyname = bytestostr(name)
+    XFree(name)
     return pyname
 
 
 # Children listing
 cdef _query_tree(pywindow):
     cdef Window root = 0, parent = 0
     cdef Window * children = <Window *> 0
@@ -811,16 +812,17 @@
         disp = get_raw_display_for(display)
         gdk_x11_display_error_trap_push(disp)
         try:
             win = GdkX11.X11Window.foreign_new_for_display(display, xwin)
         except TypeError as e:
             verbose("cannot get gdk window for %s, %#x: %s", display, xwin, e)
             return None
-        gdk_display_flush(disp)
-        error = gdk_x11_display_error_trap_pop(disp)
+        finally:
+            gdk_display_flush(disp)
+            error = gdk_x11_display_error_trap_pop(disp)
     except Exception as e:
         verbose("cannot get gdk window for %s, %#x: %s", display, xwin, e)
         if disp:
             error = gdk_x11_display_error_trap_pop(disp)
             if error:
                 verbose("ignoring XError %s in unwind", get_error_text(error))
             raise XError(e) from None
```

### Comparing `xpra-4.4.4/xpra/x11/gtk3/gdk_display_source.pyx` & `xpra-4.4.5/xpra/x11/gtk3/gdk_display_source.pyx`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/gtk3/gdk_display_util.py` & `xpra-4.4.5/xpra/x11/gtk3/gdk_display_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/gtk_x11/__init__.py` & `xpra-4.4.5/xpra/x11/gtk_x11/__init__.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/gtk_x11/clipboard.py` & `xpra-4.4.5/xpra/x11/gtk_x11/clipboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,18 +329,17 @@
         log.info(" %s", event)
 
 
     def get_wintitle(self, xid):
         data = X11Window.XGetWindowProperty(xid, "WM_NAME", "STRING")
         if data:
             return data.decode("latin1")
-        data = X11Window.XGetWindowProperty(xid, "_NET_WM_NAME", "STRING")
+        data = X11Window.XGetWindowProperty(xid, "_NET_WM_NAME", "UTF8_STRING")
         if data:
             return data.decode("utf8")
-        xid = X11Window.getParent(xid)
         return None
 
     def get_wininfo(self, xid):
         wininfo = [f"xid={xid:x}"]
         if XRes:
             with xswallow:
                 pid = XRes.get_pid(xid)
```

### Comparing `xpra-4.4.4/xpra/x11/gtk_x11/composite.py` & `xpra-4.4.5/xpra/x11/gtk_x11/composite.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/gtk_x11/gdk_bindings.py` & `xpra-4.4.5/xpra/x11/gtk_x11/gdk_bindings.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/gtk_x11/gdk_display_source.py` & `xpra-4.4.5/xpra/x11/gtk_x11/gdk_display_source.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/gtk_x11/keys.py` & `xpra-4.4.5/xpra/x11/gtk_x11/keys.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/gtk_x11/prop.py` & `xpra-4.4.5/xpra/x11/gtk_x11/prop.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/gtk_x11/selection.py` & `xpra-4.4.5/xpra/x11/gtk_x11/selection.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/gtk_x11/send_wm.py` & `xpra-4.4.5/xpra/x11/gtk_x11/send_wm.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/gtk_x11/tray.py` & `xpra-4.4.5/xpra/x11/gtk_x11/tray.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/gtk_x11/window_damage.py` & `xpra-4.4.5/xpra/x11/gtk_x11/window_damage.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/gtk_x11/wm.py` & `xpra-4.4.5/xpra/x11/gtk_x11/wm.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/gtk_x11/wm_check.py` & `xpra-4.4.5/xpra/x11/gtk_x11/wm_check.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/gtk_x11/world_window.py` & `xpra-4.4.5/xpra/x11/gtk_x11/world_window.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/models/base.py` & `xpra-4.4.5/xpra/x11/models/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -604,15 +604,15 @@
                 #we don't honour those because they make little sense, see:
                 #https://mail.gnome.org/archives/wm-spec-list/2005-May/msg00004.html
             elif atom1=="_NET_WM_STATE_MODAL":
                 update_wm_state("modal")
             elif atom1=="_NET_WM_STATE_DEMANDS_ATTENTION":
                 update_wm_state("attention-requested")
             else:
-                log.info("Unhandled _NET_WM_STATE request: '%s'", event, atom1)
+                log.info("Unhandled _NET_WM_STATE request: '%s'", atom1)
                 log.info(" event%s", event)
             return True
         if event.message_type=="WM_CHANGE_STATE":
             iconic = event.data[0]
             log("WM_CHANGE_STATE: %s, serial=%s, last unmap serial=%#x",
                 ICONIC_STATE_STRING.get(iconic, iconic), event.serial, self.last_unmap_serial)
             if (
```

### Comparing `xpra-4.4.4/xpra/x11/models/core.py` & `xpra-4.4.5/xpra/x11/models/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 if not XRes.check_xres():
     log.warn("Warning: X Resource Extension missing or too old")
     XRes = None
 
 try:
     from xpra.platform.xposix.proc import get_parent_pid
 except ImportError:
-    log("proc.get_parent_pid is not available", exc_info=True)
+    log("proc.get_parent_pid is not available")
     get_parent_pid = None
 
 FORCE_QUIT = envbool("XPRA_FORCE_QUIT", True)
 XSHAPE = envbool("XPRA_XSHAPE", True)
 FRAME_EXTENTS = envbool("XPRA_FRAME_EXTENTS", True)
 OPAQUE_REGION = envbool("XPRA_OPAQUE_REGION", True)
```

### Comparing `xpra-4.4.4/xpra/x11/models/model_stub.py` & `xpra-4.4.5/xpra/x11/models/model_stub.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/models/or_window.py` & `xpra-4.4.5/xpra/x11/models/or_window.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/models/size_hints_util.py` & `xpra-4.4.5/xpra/x11/models/size_hints_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/models/systray.py` & `xpra-4.4.5/xpra/x11/models/systray.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/models/window.py` & `xpra-4.4.5/xpra/x11/models/window.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # This file is part of Xpra.
 # Copyright (C) 2008, 2009 Nathaniel Smith <njs@pobox.com>
 # Copyright (C) 2011-2022 Antoine Martin <antoine@xpra.org>
 # Xpra is released under the terms of the GNU GPL v2, or, at your option, any
 # later version. See the file COPYING for details.
 
-from gi.repository import GObject, Gtk, Gdk
+from gi.repository import GObject, Gtk
 
 from xpra.util import envint, envbool, typedict
 from xpra.common import MAX_WINDOW_SIZE
 from xpra.gtk_common.gobject_util import one_arg_signal
 from xpra.gtk_common.error import XError, xsync, xswallow, xlog
-from xpra.x11.gtk_x11 import GDKX11Window
 from xpra.x11.gtk_x11.send_wm import send_wm_take_focus
 from xpra.x11.gtk_x11.prop import prop_set, prop_get
 from xpra.x11.prop_conv import MotifWMHints
 from xpra.x11.bindings.window_bindings import X11WindowBindings #@UnresolvedImport
 from xpra.x11.common import Unmanageable
 from xpra.x11.models.size_hints_util import sanitize_size_hints
 from xpra.x11.models.base import BaseWindowModel, constants
 from xpra.x11.models.core import sanestr
 from xpra.x11.gtk_x11.gdk_bindings import (
     add_event_receiver, remove_event_receiver,
     get_children,
     calc_constrained_size,
     x11_get_server_time,
+    get_pywindow,
     )
 
 from xpra.gtk_common.gtk_util import get_default_root_window
 from xpra.log import Logger
 
 log = Logger("x11", "window")
 workspacelog = Logger("x11", "window", "workspace")
@@ -191,21 +191,18 @@
         ogeom = self.client_window.get_geometry()
         ox, oy, ow, oh = ogeom[:4]
         # We enable PROPERTY_CHANGE_MASK so that we can call
         # x11_get_server_time on this window.
         # clamp this window to the desktop size:
         x, y = self._clamp_to_desktop(ox, oy, ow, oh)
         geomlog("setup() clamp_to_desktop(%s)=%s", ogeom, (x, y))
-        self.corral_window = GDKX11Window(self.parking_window,
-                                        x=x, y=y, width=ow, height=oh,
-                                        window_type=Gdk.WindowType.CHILD,
-                                        event_mask=Gdk.EventMask.PROPERTY_CHANGE_MASK,
-                                        title = "CorralWindow-%#x" % self.xid)
-        cxid = self.corral_window.get_xid()
-        log("setup() corral_window=%#x", cxid)
+        parking_xid = self.parking_window.get_xid()
+        cxid = X11Window.CreateCorralWindow(parking_xid, self.xid, x, y)
+        self.corral_window = get_pywindow(cxid)
+        log("setup() corral_xid=%#x, corral_window=", cxid, self.corral_window)
         prop_set(self.corral_window, "_NET_WM_NAME", "utf8", "Xpra-CorralWindow-%#x" % self.xid)
         X11Window.substructureRedirect(cxid)
         add_event_receiver(self.corral_window, self)
 
         # The child might already be mapped, in case we inherited it from
         # a previous window manager.  If so, we unmap it now, and save the
         # serial number of the request -- this way, when we get an
@@ -371,15 +368,18 @@
                     X11Window.XRemoveFromSaveSet(self.xid)
                 self.in_save_set = False
             with xswallow:
                 X11Window.sendConfigureNotify(self.xid)
             if wm_exiting:
                 self.client_window.show_unraised()
             #it is now safe to destroy the corral window:
-            cwin.destroy()
+            cxid = cwin.get_xid()
+            if cxid:
+                with xsync:
+                    X11Window.DestroyWindow(cxid)
         super().do_unmanaged(wm_exiting)
 
 
     #########################################
     # Actions specific to WindowModel
     #########################################
```

### Comparing `xpra-4.4.4/xpra/x11/prop_conv.py` & `xpra-4.4.5/xpra/x11/prop_conv.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/server.py` & `xpra-4.4.5/xpra/x11/server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/server_keyboard_config.py` & `xpra-4.4.5/xpra/x11/server_keyboard_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,33 +338,32 @@
             do_set_keymap(self.layout, self.variant, self.options, self.query_struct)
         log("set_keymap: query_struct=%r", self.query_struct)
         with xlog:
             #first clear all existing modifiers:
             clean_keyboard_state()
 
             if not self.raw:
-                has_keycodes = bool(self.x11_keycodes) or bool(self.keycodes)
-                assert has_keycodes, "client failed to provide any keycodes!"
-
                 clear_modifiers()
                 clean_keyboard_state()
 
                 #now set all the keycodes:
                 #first compute the modifier maps as this may have an influence
                 #on the keycode mappings (at least for the from_keycodes case):
                 self.compute_modifiers()
                 #key translation:
                 if self.x11_keycodes and self.query_struct:
                     #native full mapping of all keycodes:
                     self.keycode_translation = set_all_keycodes(self.x11_keycodes, self.keycodes, False, self.keynames_for_mod)
-                else:
+                elif self.keycodes:
                     #if the client does not provide a full native keymap with all the keycodes,
                     #try to preserve the initial server keycodes and translate the client keycodes instead:
                     #(used by non X11 clients like osx,win32 or HTML5)
                     self.keycode_translation = set_keycode_translation(self.x11_keycodes, self.keycodes)
+                else:
+                    self.keycode_translation = {}
                 self.add_gtk_keynames()
 
                 #now set the new modifier mappings:
                 clean_keyboard_state()
                 log("going to set modifiers, mod_meanings=%s, len(keycodes)=%s, keynames_for_mod=%s", self.mod_meanings, len(self.keycodes or []), self.keynames_for_mod)
                 if self.keynames_for_mod:
                     set_modifiers(self.keynames_for_mod)
```

### Comparing `xpra-4.4.4/xpra/x11/shadow_x11_server.py` & `xpra-4.4.5/xpra/x11/shadow_x11_server.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/uinput_device.py` & `xpra-4.4.5/xpra/x11/uinput_device.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/vfb_util.py` & `xpra-4.4.5/xpra/x11/vfb_util.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/window_info.py` & `xpra-4.4.5/xpra/x11/window_info.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/x11_server_base.py` & `xpra-4.4.5/xpra/x11/x11_server_base.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/x11_server_core.py` & `xpra-4.4.5/xpra/x11/x11_server_core.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/x11_window_filters.py` & `xpra-4.4.5/xpra/x11/x11_window_filters.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/xkbhelper.py` & `xpra-4.4.5/xpra/x11/xkbhelper.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/xroot_props.py` & `xpra-4.4.5/xpra/x11/xroot_props.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/xsettings.py` & `xpra-4.4.5/xpra/x11/xsettings.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra/x11/xsettings_prop.py` & `xpra-4.4.5/xpra/x11/xsettings_prop.py`

 * *Files identical despite different names*

### Comparing `xpra-4.4.4/xpra.egg-info/SOURCES.txt` & `xpra-4.4.5/xpra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

