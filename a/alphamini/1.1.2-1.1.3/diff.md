# Comparing `tmp/alphamini-1.1.2.tar.gz` & `tmp/alphamini-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphamini-1.1.2.tar", last modified: Tue May 17 10:27:42 2022, max compression
+gzip compressed data, was "dist/alphamini-1.1.3.tar", last modified: Tue May 23 07:36:36 2023, max compression
```

## Comparing `alphamini-1.1.2.tar` & `alphamini-1.1.3.tar`

### file list

```diff
@@ -1,126 +1,138 @@
-drwxrwxr-x   0 lzc       (1000) lzc       (1000)        0 2022-05-17 10:27:42.913604 alphamini-1.1.2/
--rw-rw-r--   0 lzc       (1000) lzc       (1000)      590 2022-05-17 10:27:42.913604 alphamini-1.1.2/PKG-INFO
--rw-rw-r--   0 lzc       (1000) lzc       (1000)      149 2022-05-17 10:21:05.000000 alphamini-1.1.2/README.md
-drwxrwxr-x   0 lzc       (1000) lzc       (1000)        0 2022-05-17 10:27:42.905604 alphamini-1.1.2/alphamini.egg-info/
--rw-rw-r--   0 lzc       (1000) lzc       (1000)      590 2022-05-17 10:27:42.000000 alphamini-1.1.2/alphamini.egg-info/PKG-INFO
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3819 2022-05-17 10:27:42.000000 alphamini-1.1.2/alphamini.egg-info/SOURCES.txt
--rw-rw-r--   0 lzc       (1000) lzc       (1000)        1 2022-05-17 10:27:42.000000 alphamini-1.1.2/alphamini.egg-info/dependency_links.txt
--rw-rw-r--   0 lzc       (1000) lzc       (1000)      485 2022-05-17 10:27:42.000000 alphamini-1.1.2/alphamini.egg-info/entry_points.txt
--rw-rw-r--   0 lzc       (1000) lzc       (1000)        1 2022-05-17 10:27:42.000000 alphamini-1.1.2/alphamini.egg-info/not-zip-safe
--rw-rw-r--   0 lzc       (1000) lzc       (1000)       33 2022-05-17 10:27:42.000000 alphamini-1.1.2/alphamini.egg-info/requires.txt
--rw-rw-r--   0 lzc       (1000) lzc       (1000)        5 2022-05-17 10:27:42.000000 alphamini-1.1.2/alphamini.egg-info/top_level.txt
-drwxrwxr-x   0 lzc       (1000) lzc       (1000)        0 2022-05-17 10:27:42.905604 alphamini-1.1.2/mini/
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     1359 2022-05-17 10:21:05.000000 alphamini-1.1.2/mini/__init__.py
-drwxrwxr-x   0 lzc       (1000) lzc       (1000)        0 2022-05-17 10:27:42.909604 alphamini-1.1.2/mini/apis/
--rw-rw-r--   0 lzc       (1000) lzc       (1000)      487 2022-05-17 10:21:05.000000 alphamini-1.1.2/mini/apis/__init__.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)    11214 2022-05-17 10:21:05.000000 alphamini-1.1.2/mini/apis/api_action.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     5180 2022-05-17 10:21:05.000000 alphamini-1.1.2/mini/apis/api_behavior.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4276 2022-05-17 10:21:05.000000 alphamini-1.1.2/mini/apis/api_config.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4693 2022-05-17 10:21:05.000000 alphamini-1.1.2/mini/apis/api_content.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     7082 2022-05-17 10:21:05.000000 alphamini-1.1.2/mini/apis/api_expression.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)    15901 2022-05-17 10:21:05.000000 alphamini-1.1.2/mini/apis/api_observe.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)    13007 2022-05-17 10:24:58.000000 alphamini-1.1.2/mini/apis/api_sence.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3807 2022-05-17 10:21:05.000000 alphamini-1.1.2/mini/apis/api_setup.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)    23331 2022-05-17 10:21:05.000000 alphamini-1.1.2/mini/apis/api_sound.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     6651 2022-05-17 10:21:05.000000 alphamini-1.1.2/mini/apis/base_api.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3118 2022-05-17 10:21:05.000000 alphamini-1.1.2/mini/apis/cmdid.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     8862 2022-05-17 10:21:05.000000 alphamini-1.1.2/mini/apis/errors.py
-drwxrwxr-x   0 lzc       (1000) lzc       (1000)        0 2022-05-17 10:27:42.909604 alphamini-1.1.2/mini/channels/
--rw-rw-r--   0 lzc       (1000) lzc       (1000)       50 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/channels/__init__.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     1883 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/channels/msg_utils.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)    11044 2022-05-17 10:21:05.000000 alphamini-1.1.2/mini/channels/websocket_client.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3285 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/channels/websocket_server.py
-drwxrwxr-x   0 lzc       (1000) lzc       (1000)        0 2022-05-17 10:27:42.909604 alphamini-1.1.2/mini/dns/
--rw-rw-r--   0 lzc       (1000) lzc       (1000)       58 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/dns/__init__.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     5361 2022-05-17 10:21:05.000000 alphamini-1.1.2/mini/dns/dns_browser.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)   100660 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/dns/zeroconf.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)    32604 2022-05-17 10:21:05.000000 alphamini-1.1.2/mini/mini_sdk.py
-drwxrwxr-x   0 lzc       (1000) lzc       (1000)        0 2022-05-17 10:27:42.913604 alphamini-1.1.2/mini/pb2/
--rw-rw-r--   0 lzc       (1000) lzc       (1000)       20 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/__init__.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3978 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/blebindorswitchwifi_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3810 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/bthandshake_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3993 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/cloudstorageurls_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)    13329 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/cloudtranslate_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3416 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/cloudwiki_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4548 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/cmprivacymode_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     5620 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_actioninfo_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4018 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_changerobotvolume_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4409 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_controlbehavior_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     5259 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_controlfindface_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3889 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_controlmouthlamp_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     6147 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_controlregisterface_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     6165 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_controlrobotrecord_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4861 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_controlrunningprogram_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4241 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_controltts_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3509 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_expressioninfo_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4592 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_faceanalyze_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4722 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_facedetect_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     6624 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_facedetecttask_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     5040 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_faceinfo_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     5107 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_facerecognise_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     7024 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_facerecognisetask_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     5123 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_getactionlist_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     5959 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_getaudiolist_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3876 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_getinfrareddistance_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4284 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_getregisterfaces_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3844 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_getrobotexpression_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     2963 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_getrobotsid_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3900 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_getserverinfo_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3341 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_handshake_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4188 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_moverobot_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4802 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_observebutterystatus_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3538 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_observefallclimb_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3561 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_observeheadracket_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4960 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_observeinfrareddistance_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4396 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_observevolumekeypress_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3826 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_playaction_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4479 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_playaudio_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4005 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_playcustomaction_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4395 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_playexpression_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4386 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_playonlinemusic_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4835 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_recogniseobject_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3428 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_revertorigin_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3839 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_searchfaces_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     6077 2022-05-17 10:21:05.000000 alphamini-1.1.2/mini/pb2/codemao_setmouthlamp_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4401 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_speechrecognise_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3370 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_stopaction_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3341 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_stopaudio_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4005 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_stopcustomaction_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4330 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_stopspeechrecognise_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4813 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_switchtranslatemodel_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4261 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_takepicture_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4035 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_translate_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3829 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/codemao_wiki_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3680 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/detectconfig_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     2921 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/httpserverconfig_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     2597 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/pccodemao_disconnection_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3841 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/pccodemao_getappversion_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4128 2022-05-17 10:21:05.000000 alphamini-1.1.2/mini/pb2/pccodemao_getrobotlanguage_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     2563 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/pccodemao_message_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     2793 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/pccodemao_messageheader_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     6736 2022-05-17 10:21:05.000000 alphamini-1.1.2/mini/pb2/pccodemao_setrobotlanguage_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4214 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/pccodemao_takepicture_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4842 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/programme_facedetecting_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4997 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/programme_facetrack_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     2857 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/programme_resource_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     7526 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/programme_startrun_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3665 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/receiver_udpdata_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     2384 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/robotpushmessage_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     2649 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/pb2/terminaltype_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)    20030 2022-05-17 10:21:05.000000 alphamini-1.1.2/mini/pkg_tool.py
-drwxrwxr-x   0 lzc       (1000) lzc       (1000)        0 2022-05-17 10:27:42.913604 alphamini-1.1.2/mini/tool/
--rw-rw-r--   0 lzc       (1000) lzc       (1000)       21 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/tool/__init__.py
-drwxrwxr-x   0 lzc       (1000) lzc       (1000)        0 2022-05-17 10:27:42.913604 alphamini-1.1.2/mini/tool/pb2/
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3556 2022-05-17 10:21:05.000000 alphamini-1.1.2/mini/tool/pb2/PyPi_AdbSwitch_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3668 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/tool/pb2/PyPi_GetWheelInfo_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3643 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/tool/pb2/PyPi_GetWheelList_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4496 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/tool/pb2/PyPi_InstallWheel_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     3946 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/tool/pb2/PyPi_RunWheel_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     4132 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/tool/pb2/PyPi_UninstallWheel_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     6175 2022-05-17 10:21:05.000000 alphamini-1.1.2/mini/tool/pb2/PyPi_UploadScript_pb2.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)       20 2022-05-17 10:19:58.000000 alphamini-1.1.2/mini/tool/pb2/__init__.py
-drwxrwxr-x   0 lzc       (1000) lzc       (1000)        0 2022-05-17 10:27:42.913604 alphamini-1.1.2/mini/tool/script/
--rw-rw-r--   0 lzc       (1000) lzc       (1000)        0 2022-04-20 07:02:07.000000 alphamini-1.1.2/mini/tool/script/__init__.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     7057 2022-05-17 10:21:05.000000 alphamini-1.1.2/mini/tool/script/cli.py
--rw-rw-r--   0 lzc       (1000) lzc       (1000)       38 2022-05-17 10:27:42.913604 alphamini-1.1.2/setup.cfg
--rw-rw-r--   0 lzc       (1000) lzc       (1000)     1717 2022-05-17 10:27:39.000000 alphamini-1.1.2/setup.py
+drwxrwxr-x   0 logic     (1000) logic     (1000)        0 2023-05-23 07:36:36.000000 alphamini-1.1.3/
+-rw-r--r--   0 logic     (1000) logic     (1000)     1062 2020-08-06 07:48:17.000000 alphamini-1.1.3/LICENSE
+-rw-rw-r--   0 logic     (1000) logic     (1000)      477 2023-05-23 07:36:36.000000 alphamini-1.1.3/PKG-INFO
+-rw-r--r--   0 logic     (1000) logic     (1000)       71 2023-05-23 03:35:31.000000 alphamini-1.1.3/README.md
+drwxrwxr-x   0 logic     (1000) logic     (1000)        0 2023-05-23 07:36:36.000000 alphamini-1.1.3/alphamini.egg-info/
+-rw-rw-r--   0 logic     (1000) logic     (1000)      477 2023-05-23 07:36:36.000000 alphamini-1.1.3/alphamini.egg-info/PKG-INFO
+-rw-rw-r--   0 logic     (1000) logic     (1000)     4054 2023-05-23 07:36:36.000000 alphamini-1.1.3/alphamini.egg-info/SOURCES.txt
+-rw-rw-r--   0 logic     (1000) logic     (1000)        1 2023-05-23 07:36:36.000000 alphamini-1.1.3/alphamini.egg-info/dependency_links.txt
+-rw-rw-r--   0 logic     (1000) logic     (1000)      484 2023-05-23 07:36:36.000000 alphamini-1.1.3/alphamini.egg-info/entry_points.txt
+-rw-rw-r--   0 logic     (1000) logic     (1000)        1 2023-05-23 03:32:33.000000 alphamini-1.1.3/alphamini.egg-info/not-zip-safe
+-rw-rw-r--   0 logic     (1000) logic     (1000)       33 2023-05-23 07:36:36.000000 alphamini-1.1.3/alphamini.egg-info/requires.txt
+-rw-rw-r--   0 logic     (1000) logic     (1000)        5 2023-05-23 07:36:36.000000 alphamini-1.1.3/alphamini.egg-info/top_level.txt
+drwxrwxr-x   0 logic     (1000) logic     (1000)        0 2023-05-23 07:36:36.000000 alphamini-1.1.3/mini/
+-rw-r--r--   0 logic     (1000) logic     (1000)     1359 2021-08-17 09:26:43.000000 alphamini-1.1.3/mini/__init__.py
+drwxrwxr-x   0 logic     (1000) logic     (1000)        0 2023-05-23 07:36:36.000000 alphamini-1.1.3/mini/apis/
+-rw-r--r--   0 logic     (1000) logic     (1000)      487 2020-08-06 07:48:17.000000 alphamini-1.1.3/mini/apis/__init__.py
+-rw-r--r--   0 logic     (1000) logic     (1000)    11214 2021-08-17 09:26:43.000000 alphamini-1.1.3/mini/apis/api_action.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     5180 2021-08-17 09:26:43.000000 alphamini-1.1.3/mini/apis/api_behavior.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4276 2021-08-17 09:26:43.000000 alphamini-1.1.3/mini/apis/api_config.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4693 2021-08-17 09:26:43.000000 alphamini-1.1.3/mini/apis/api_content.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     7082 2021-08-17 09:26:43.000000 alphamini-1.1.3/mini/apis/api_expression.py
+-rw-r--r--   0 logic     (1000) logic     (1000)    15901 2021-08-17 09:26:43.000000 alphamini-1.1.3/mini/apis/api_observe.py
+-rw-rw-r--   0 logic     (1000) logic     (1000)    13007 2023-05-22 07:21:55.000000 alphamini-1.1.3/mini/apis/api_sence.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3807 2021-08-17 09:26:43.000000 alphamini-1.1.3/mini/apis/api_setup.py
+-rw-r--r--   0 logic     (1000) logic     (1000)    23331 2021-08-17 09:26:43.000000 alphamini-1.1.3/mini/apis/api_sound.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     6651 2021-08-17 09:26:43.000000 alphamini-1.1.3/mini/apis/base_api.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3118 2021-08-17 09:26:43.000000 alphamini-1.1.3/mini/apis/cmdid.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     8862 2021-08-17 09:26:43.000000 alphamini-1.1.3/mini/apis/errors.py
+drwxrwxr-x   0 logic     (1000) logic     (1000)        0 2023-05-23 07:36:36.000000 alphamini-1.1.3/mini/channels/
+-rw-r--r--   0 logic     (1000) logic     (1000)       50 2021-08-17 09:24:21.000000 alphamini-1.1.3/mini/channels/__init__.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     1883 2021-08-17 09:26:43.000000 alphamini-1.1.3/mini/channels/msg_utils.py
+-rw-r--r--   0 logic     (1000) logic     (1000)    11044 2021-08-17 09:26:43.000000 alphamini-1.1.3/mini/channels/websocket_client.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3285 2020-08-06 07:48:17.000000 alphamini-1.1.3/mini/channels/websocket_server.py
+drwxrwxr-x   0 logic     (1000) logic     (1000)        0 2023-05-23 07:36:36.000000 alphamini-1.1.3/mini/dns/
+-rw-r--r--   0 logic     (1000) logic     (1000)       58 2021-08-17 09:24:21.000000 alphamini-1.1.3/mini/dns/__init__.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     5361 2021-08-17 09:26:43.000000 alphamini-1.1.3/mini/dns/dns_browser.py
+-rw-r--r--   0 logic     (1000) logic     (1000)   100660 2020-08-06 07:48:17.000000 alphamini-1.1.3/mini/dns/zeroconf.py
+-rw-r--r--   0 logic     (1000) logic     (1000)    32775 2023-05-22 07:23:59.000000 alphamini-1.1.3/mini/mini_sdk.py
+drwxrwxr-x   0 logic     (1000) logic     (1000)        0 2023-05-23 07:36:36.000000 alphamini-1.1.3/mini/pb2/
+-rw-r--r--   0 logic     (1000) logic     (1000)       20 2020-08-06 07:48:17.000000 alphamini-1.1.3/mini/pb2/__init__.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3978 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/blebindorswitchwifi_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3810 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/bthandshake_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3993 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/cloudstorageurls_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)    13329 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/cloudtranslate_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3416 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/cloudwiki_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4548 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/cmprivacymode_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     5620 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_actioninfo_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4018 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_changerobotvolume_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4409 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_controlbehavior_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     5259 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_controlfindface_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3889 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_controlmouthlamp_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     6147 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_controlregisterface_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     6165 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_controlrobotrecord_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4861 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_controlrunningprogram_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4241 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_controltts_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3509 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_expressioninfo_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4592 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_faceanalyze_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4722 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_facedetect_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     6624 2021-08-17 09:24:21.000000 alphamini-1.1.3/mini/pb2/codemao_facedetecttask_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     5040 2021-08-17 09:24:21.000000 alphamini-1.1.3/mini/pb2/codemao_faceinfo_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     5107 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_facerecognise_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     7024 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_facerecognisetask_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     5123 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_getactionlist_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     5959 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_getaudiolist_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3876 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_getinfrareddistance_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4284 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_getregisterfaces_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3844 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_getrobotexpression_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     2963 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_getrobotsid_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3900 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_getserverinfo_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3341 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_handshake_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4188 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_moverobot_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4802 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_observebutterystatus_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3538 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_observefallclimb_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3561 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_observeheadracket_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4960 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_observeinfrareddistance_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4396 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_observevolumekeypress_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3826 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_playaction_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4479 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_playaudio_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4005 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_playcustomaction_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4395 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_playexpression_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4386 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_playonlinemusic_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4835 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_recogniseobject_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3428 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_revertorigin_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3839 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_searchfaces_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     6077 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_setmouthlamp_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4401 2021-08-17 09:26:17.000000 alphamini-1.1.3/mini/pb2/codemao_speechrecognise_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3370 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_stopaction_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3341 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_stopaudio_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4005 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_stopcustomaction_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4330 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_stopspeechrecognise_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4813 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_switchtranslatemodel_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4261 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_takepicture_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4035 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_translate_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3829 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/codemao_wiki_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3680 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/detectconfig_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     2921 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/httpserverconfig_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     2597 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/pccodemao_disconnection_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3841 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/pccodemao_getappversion_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4128 2021-08-17 09:26:43.000000 alphamini-1.1.3/mini/pb2/pccodemao_getrobotlanguage_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     2563 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/pccodemao_message_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     2793 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/pccodemao_messageheader_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     6736 2021-08-17 09:26:43.000000 alphamini-1.1.3/mini/pb2/pccodemao_setrobotlanguage_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4214 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/pccodemao_takepicture_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4842 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/programme_facedetecting_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4997 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/programme_facetrack_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     2857 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/programme_resource_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     7526 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/programme_startrun_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3665 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/receiver_udpdata_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     2384 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/robotpushmessage_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     2649 2021-08-05 07:44:53.000000 alphamini-1.1.3/mini/pb2/terminaltype_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)    20030 2021-08-17 09:26:43.000000 alphamini-1.1.3/mini/pkg_tool.py
+drwxrwxr-x   0 logic     (1000) logic     (1000)        0 2023-05-23 07:36:36.000000 alphamini-1.1.3/mini/tool/
+-rw-r--r--   0 logic     (1000) logic     (1000)       21 2021-08-17 09:24:21.000000 alphamini-1.1.3/mini/tool/__init__.py
+drwxrwxr-x   0 logic     (1000) logic     (1000)        0 2023-05-23 07:36:36.000000 alphamini-1.1.3/mini/tool/pb2/
+-rw-r--r--   0 logic     (1000) logic     (1000)     3556 2021-08-17 09:26:43.000000 alphamini-1.1.3/mini/tool/pb2/PyPi_AdbSwitch_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3668 2020-10-21 05:48:36.000000 alphamini-1.1.3/mini/tool/pb2/PyPi_GetWheelInfo_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3643 2020-10-21 05:48:37.000000 alphamini-1.1.3/mini/tool/pb2/PyPi_GetWheelList_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4496 2020-10-21 05:48:37.000000 alphamini-1.1.3/mini/tool/pb2/PyPi_InstallWheel_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     3946 2020-10-21 05:48:37.000000 alphamini-1.1.3/mini/tool/pb2/PyPi_RunWheel_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     4132 2020-10-21 05:48:37.000000 alphamini-1.1.3/mini/tool/pb2/PyPi_UninstallWheel_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     6175 2021-08-17 09:26:43.000000 alphamini-1.1.3/mini/tool/pb2/PyPi_UploadScript_pb2.py
+-rw-r--r--   0 logic     (1000) logic     (1000)       20 2020-08-06 07:48:17.000000 alphamini-1.1.3/mini/tool/pb2/__init__.py
+drwxrwxr-x   0 logic     (1000) logic     (1000)        0 2023-05-23 07:36:36.000000 alphamini-1.1.3/mini/tool/script/
+-rw-r--r--   0 logic     (1000) logic     (1000)        0 2020-08-06 07:48:17.000000 alphamini-1.1.3/mini/tool/script/__init__.py
+-rw-r--r--   0 logic     (1000) logic     (1000)     7057 2021-08-17 09:26:43.000000 alphamini-1.1.3/mini/tool/script/cli.py
+-rw-rw-r--   0 logic     (1000) logic     (1000)       38 2023-05-23 07:36:36.000000 alphamini-1.1.3/setup.cfg
+-rw-rw-r--   0 logic     (1000) logic     (1000)     1713 2023-05-23 03:40:19.000000 alphamini-1.1.3/setup.py
+drwxrwxr-x   0 logic     (1000) logic     (1000)        0 2023-05-23 07:36:36.000000 alphamini-1.1.3/test/
+-rw-rw-r--   0 logic     (1000) logic     (1000)     3553 2023-05-23 03:02:26.000000 alphamini-1.1.3/test/test_action.py
+-rw-rw-r--   0 logic     (1000) logic     (1000)     2919 2023-05-23 03:02:31.000000 alphamini-1.1.3/test/test_connect.py
+-rw-rw-r--   0 logic     (1000) logic     (1000)     2602 2023-05-23 03:02:35.000000 alphamini-1.1.3/test/test_content.py
+-rw-rw-r--   0 logic     (1000) logic     (1000)     8210 2023-05-23 03:02:38.000000 alphamini-1.1.3/test/test_event.py
+-rw-rw-r--   0 logic     (1000) logic     (1000)     5358 2023-05-23 03:02:42.000000 alphamini-1.1.3/test/test_expression.py
+-rw-rw-r--   0 logic     (1000) logic     (1000)     1173 2023-05-23 03:02:48.000000 alphamini-1.1.3/test/test_pkg_tool.py
+-rw-rw-r--   0 logic     (1000) logic     (1000)     4501 2023-05-23 03:02:45.000000 alphamini-1.1.3/test/test_pkg_tool_upload_script.py
+-rw-rw-r--   0 logic     (1000) logic     (1000)    10724 2023-05-23 03:02:50.000000 alphamini-1.1.3/test/test_sence.py
+-rw-rw-r--   0 logic     (1000) logic     (1000)     9591 2023-05-23 03:02:52.000000 alphamini-1.1.3/test/test_sound.py
+-rw-rw-r--   0 logic     (1000) logic     (1000)     1014 2023-05-23 03:02:55.000000 alphamini-1.1.3/test/test_wifi_browser.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `alphamini-1.1.2/alphamini.egg-info/SOURCES.txt` & `alphamini-1.1.3/alphamini.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 alphamini.egg-info/PKG-INFO
 alphamini.egg-info/SOURCES.txt
 alphamini.egg-info/dependency_links.txt
 alphamini.egg-info/entry_points.txt
 alphamini.egg-info/not-zip-safe
@@ -107,8 +108,18 @@
 mini/tool/pb2/PyPi_GetWheelList_pb2.py
 mini/tool/pb2/PyPi_InstallWheel_pb2.py
 mini/tool/pb2/PyPi_RunWheel_pb2.py
 mini/tool/pb2/PyPi_UninstallWheel_pb2.py
 mini/tool/pb2/PyPi_UploadScript_pb2.py
 mini/tool/pb2/__init__.py
 mini/tool/script/__init__.py
-mini/tool/script/cli.py
+mini/tool/script/cli.py
+test/test_action.py
+test/test_connect.py
+test/test_content.py
+test/test_event.py
+test/test_expression.py
+test/test_pkg_tool.py
+test/test_pkg_tool_upload_script.py
+test/test_sence.py
+test/test_sound.py
+test/test_wifi_browser.py
```

### Comparing `alphamini-1.1.2/mini/__init__.py` & `alphamini-1.1.3/mini/__init__.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/apis/api_action.py` & `alphamini-1.1.3/mini/apis/api_action.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/apis/api_behavior.py` & `alphamini-1.1.3/mini/apis/api_behavior.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/apis/api_config.py` & `alphamini-1.1.3/mini/apis/api_config.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/apis/api_content.py` & `alphamini-1.1.3/mini/apis/api_content.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/apis/api_expression.py` & `alphamini-1.1.3/mini/apis/api_expression.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/apis/api_observe.py` & `alphamini-1.1.3/mini/apis/api_observe.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/apis/api_sence.py` & `alphamini-1.1.3/mini/apis/api_sence.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/apis/api_setup.py` & `alphamini-1.1.3/mini/apis/api_setup.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/apis/api_sound.py` & `alphamini-1.1.3/mini/apis/api_sound.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/apis/base_api.py` & `alphamini-1.1.3/mini/apis/base_api.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/apis/cmdid.py` & `alphamini-1.1.3/mini/apis/cmdid.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/apis/errors.py` & `alphamini-1.1.3/mini/apis/errors.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/channels/msg_utils.py` & `alphamini-1.1.3/mini/channels/msg_utils.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/channels/websocket_client.py` & `alphamini-1.1.3/mini/channels/websocket_client.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/channels/websocket_server.py` & `alphamini-1.1.3/mini/channels/websocket_server.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/dns/dns_browser.py` & `alphamini-1.1.3/mini/dns/dns_browser.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/dns/zeroconf.py` & `alphamini-1.1.3/mini/dns/zeroconf.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/mini_sdk.py` & `alphamini-1.1.3/mini/mini_sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,38 +114,41 @@
 
     Args:
         devices: Set[WiFiDevice] or None
     """
     devices: Set[WiFiDevice]
 
     def __init__(self, devices):
-        self.devices: Set[WiFiDevice] = devices or set()
+        self.devices: Set[WiFiDevice] = devices if devices else set()
 
     def on_device_updated(self, device: WiFiDevice) -> None:
         """
         机器人设备更新了
         Args:
             device: WiFiDevice
         """
+        _log.info(f"on_device_updated: {device}")
         self.devices.update([device])
 
     def on_device_removed(self, device: WiFiDevice) -> None:
         """
         机器人设备从局域网中移除了
         Args:
             device: WFiDevice
         """
+        _log.info(f"on_device_removed: {device}")
         self.devices.remove(device)
 
     def on_device_found(self, device: WiFiDevice) -> None:
         """
         扫描到一个机器人设备
         Args:
             device: WFiDevice
         """
+        _log.info(f"on_device_found: {device}")
         self.devices.add(device)
 
 
 async def _get_user_input(devices: tuple) -> int:
     try:
         i: int = 0
         for device in devices:
@@ -237,20 +240,21 @@
     Args:
         timeout: 超时时间
 
     Returns:
         Optional[WiFiDevice]
     """
     devices: Set[WiFiDevice] = set()
-    browser.add_listener(_GetWiFiDeviceListListener(devices))
+    l=_GetWiFiDeviceListListener(devices)
+    browser.add_listener(l)
     browser.start_scan(0)
     await asyncio.sleep(timeout)
     browser.remove_all_listener()
     browser.stop_scan()
-    return tuple(devices)
+    return tuple(l.devices)
 
 
 async def _connect(device: WiFiDevice) -> bool:
     """
     连接机器人设备
 
     Args:
```

### Comparing `alphamini-1.1.2/mini/pb2/blebindorswitchwifi_pb2.py` & `alphamini-1.1.3/mini/pb2/blebindorswitchwifi_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/bthandshake_pb2.py` & `alphamini-1.1.3/mini/pb2/bthandshake_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/cloudstorageurls_pb2.py` & `alphamini-1.1.3/mini/pb2/cloudstorageurls_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/cloudtranslate_pb2.py` & `alphamini-1.1.3/mini/pb2/cloudtranslate_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/cloudwiki_pb2.py` & `alphamini-1.1.3/mini/pb2/cloudwiki_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/cmprivacymode_pb2.py` & `alphamini-1.1.3/mini/pb2/cmprivacymode_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_actioninfo_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_actioninfo_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_changerobotvolume_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_changerobotvolume_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_controlbehavior_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_controlbehavior_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_controlfindface_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_controlfindface_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_controlmouthlamp_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_controlmouthlamp_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_controlregisterface_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_controlregisterface_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_controlrobotrecord_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_controlrobotrecord_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_controlrunningprogram_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_controlrunningprogram_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_controltts_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_controltts_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_expressioninfo_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_expressioninfo_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_faceanalyze_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_faceanalyze_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_facedetect_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_facedetect_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_facedetecttask_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_facedetecttask_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_faceinfo_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_faceinfo_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_facerecognise_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_facerecognise_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_facerecognisetask_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_facerecognisetask_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_getactionlist_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_getactionlist_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_getaudiolist_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_getaudiolist_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_getinfrareddistance_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_getinfrareddistance_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_getregisterfaces_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_getregisterfaces_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_getrobotexpression_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_getrobotexpression_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_getrobotsid_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_getrobotsid_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_getserverinfo_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_getserverinfo_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_handshake_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_handshake_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_moverobot_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_moverobot_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_observebutterystatus_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_observebutterystatus_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_observefallclimb_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_observefallclimb_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_observeheadracket_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_observeheadracket_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_observeinfrareddistance_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_observeinfrareddistance_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_observevolumekeypress_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_observevolumekeypress_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_playaction_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_playaction_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_playaudio_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_playaudio_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_playcustomaction_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_playcustomaction_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_playexpression_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_playexpression_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_playonlinemusic_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_playonlinemusic_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_recogniseobject_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_recogniseobject_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_revertorigin_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_revertorigin_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_searchfaces_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_searchfaces_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_setmouthlamp_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_setmouthlamp_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_speechrecognise_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_speechrecognise_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_stopaction_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_stopaction_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_stopaudio_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_stopaudio_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_stopcustomaction_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_stopcustomaction_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_stopspeechrecognise_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_stopspeechrecognise_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_switchtranslatemodel_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_switchtranslatemodel_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_takepicture_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_takepicture_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_translate_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_translate_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/codemao_wiki_pb2.py` & `alphamini-1.1.3/mini/pb2/codemao_wiki_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/detectconfig_pb2.py` & `alphamini-1.1.3/mini/pb2/detectconfig_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/httpserverconfig_pb2.py` & `alphamini-1.1.3/mini/pb2/httpserverconfig_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/pccodemao_disconnection_pb2.py` & `alphamini-1.1.3/mini/pb2/pccodemao_disconnection_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/pccodemao_getappversion_pb2.py` & `alphamini-1.1.3/mini/pb2/pccodemao_getappversion_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/pccodemao_getrobotlanguage_pb2.py` & `alphamini-1.1.3/mini/pb2/pccodemao_getrobotlanguage_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/pccodemao_message_pb2.py` & `alphamini-1.1.3/mini/pb2/pccodemao_message_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/pccodemao_messageheader_pb2.py` & `alphamini-1.1.3/mini/pb2/pccodemao_messageheader_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/pccodemao_setrobotlanguage_pb2.py` & `alphamini-1.1.3/mini/pb2/pccodemao_setrobotlanguage_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/pccodemao_takepicture_pb2.py` & `alphamini-1.1.3/mini/pb2/pccodemao_takepicture_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/programme_facedetecting_pb2.py` & `alphamini-1.1.3/mini/pb2/programme_facedetecting_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/programme_facetrack_pb2.py` & `alphamini-1.1.3/mini/pb2/programme_facetrack_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/programme_resource_pb2.py` & `alphamini-1.1.3/mini/pb2/programme_resource_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/programme_startrun_pb2.py` & `alphamini-1.1.3/mini/pb2/programme_startrun_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/receiver_udpdata_pb2.py` & `alphamini-1.1.3/mini/pb2/receiver_udpdata_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/robotpushmessage_pb2.py` & `alphamini-1.1.3/mini/pb2/robotpushmessage_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pb2/terminaltype_pb2.py` & `alphamini-1.1.3/mini/pb2/terminaltype_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/pkg_tool.py` & `alphamini-1.1.3/mini/pkg_tool.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/tool/pb2/PyPi_AdbSwitch_pb2.py` & `alphamini-1.1.3/mini/tool/pb2/PyPi_AdbSwitch_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/tool/pb2/PyPi_GetWheelInfo_pb2.py` & `alphamini-1.1.3/mini/tool/pb2/PyPi_GetWheelInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/tool/pb2/PyPi_GetWheelList_pb2.py` & `alphamini-1.1.3/mini/tool/pb2/PyPi_GetWheelList_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/tool/pb2/PyPi_InstallWheel_pb2.py` & `alphamini-1.1.3/mini/tool/pb2/PyPi_InstallWheel_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/tool/pb2/PyPi_RunWheel_pb2.py` & `alphamini-1.1.3/mini/tool/pb2/PyPi_RunWheel_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/tool/pb2/PyPi_UninstallWheel_pb2.py` & `alphamini-1.1.3/mini/tool/pb2/PyPi_UninstallWheel_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/tool/pb2/PyPi_UploadScript_pb2.py` & `alphamini-1.1.3/mini/tool/pb2/PyPi_UploadScript_pb2.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/mini/tool/script/cli.py` & `alphamini-1.1.3/mini/tool/script/cli.py`

 * *Files identical despite different names*

### Comparing `alphamini-1.1.2/setup.py` & `alphamini-1.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,24 +8,24 @@
     long_desc = f.read()
 
 with open("LICENSE", "r", encoding="UTF-8") as f:
     license_txt = f.read()
 
 setuptools.setup(
     name="alphamini",
-    version="1.1.2",
+    version="1.1.3",
     author='logic.peng',
     author_email='logic.peng@ubtrobot.com',
     description="python sdk for ubtech alpha mini robot",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     license="GPLv3",
     python_requires='>=3.7',
     # url="",
-    packages=setuptools.find_packages(exclude=["*.test", "*.test.*"]),  # 排除掉测试包
+    packages=setuptools.find_packages(exclude=["test", "test.*"]),  # 排除掉测试包
     # packages=setuptools.find_namespace_packages(where=os.curdir + "/mini"),
     # packages=['mini'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

