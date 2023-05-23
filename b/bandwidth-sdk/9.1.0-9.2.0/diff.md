# Comparing `tmp/bandwidth-sdk-9.1.0.tar.gz` & `tmp/bandwidth-sdk-9.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bandwidth-sdk-9.1.0.tar", last modified: Tue Mar 23 18:36:52 2021, max compression
+gzip compressed data, was "bandwidth-sdk-9.2.0.tar", last modified: Wed Jun 23 14:35:21 2021, max compression
```

## Comparing `bandwidth-sdk-9.1.0.tar` & `bandwidth-sdk-9.2.0.tar`

### file list

```diff
@@ -1,189 +1,206 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.451156 bandwidth-sdk-9.1.0/
--rw-r--r--   0 root         (0) root         (0)     1213 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      282 2021-03-23 18:36:52.451156 bandwidth-sdk-9.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.423155 bandwidth-sdk-9.1.0/bandwidth/
--rw-r--r--   0 root         (0) root         (0)      166 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14077 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/api_helper.py
--rw-r--r--   0 root         (0) root         (0)     2940 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/bandwidth_client.py
--rw-r--r--   0 root         (0) root         (0)     8604 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.423155 bandwidth-sdk-9.1.0/bandwidth/controllers/
--rw-r--r--   0 root         (0) root         (0)       38 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3095 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/controllers/base_controller.py
--rw-r--r--   0 root         (0) root         (0)      504 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.423155 bandwidth-sdk-9.1.0/bandwidth/exceptions/
--rw-r--r--   0 root         (0) root         (0)       36 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      884 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/exceptions/api_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.423155 bandwidth-sdk-9.1.0/bandwidth/http/
--rw-r--r--   0 root         (0) root         (0)      162 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1751 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/http/api_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.427155 bandwidth-sdk-9.1.0/bandwidth/http/auth/
--rw-r--r--   0 root         (0) root         (0)      130 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/http/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      925 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/http/auth/messaging_basic_auth.py
--rw-r--r--   0 root         (0) root         (0)      941 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/http/auth/two_factor_auth_basic_auth.py
--rw-r--r--   0 root         (0) root         (0)      913 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/http/auth/voice_basic_auth.py
--rw-r--r--   0 root         (0) root         (0)      918 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/http/auth/web_rtc_basic_auth.py
--rw-r--r--   0 root         (0) root         (0)     1124 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/http/http_call_back.py
--rw-r--r--   0 root         (0) root         (0)     7255 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/http/http_client.py
--rw-r--r--   0 root         (0) root         (0)      915 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/http/http_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     2826 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/http/http_request.py
--rw-r--r--   0 root         (0) root         (0)     1495 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/http/http_response.py
--rw-r--r--   0 root         (0) root         (0)     3682 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/http/requests_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.427155 bandwidth-sdk-9.1.0/bandwidth/messaging/
--rw-r--r--   0 root         (0) root         (0)       93 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/messaging/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.427155 bandwidth-sdk-9.1.0/bandwidth/messaging/controllers/
--rw-r--r--   0 root         (0) root         (0)       61 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/messaging/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19903 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/messaging/controllers/api_controller.py
--rw-r--r--   0 root         (0) root         (0)     3095 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/messaging/controllers/base_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.427155 bandwidth-sdk-9.1.0/bandwidth/messaging/exceptions/
--rw-r--r--   0 root         (0) root         (0)       42 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/messaging/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1317 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/messaging/exceptions/messaging_exception.py
--rw-r--r--   0 root         (0) root         (0)     2419 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/messaging/messaging_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.431155 bandwidth-sdk-9.1.0/bandwidth/messaging/models/
--rw-r--r--   0 root         (0) root         (0)      252 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/messaging/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2667 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/messaging/models/bandwidth_callback_message.py
--rw-r--r--   0 root         (0) root         (0)     4065 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/messaging/models/bandwidth_message.py
--rw-r--r--   0 root         (0) root         (0)     4284 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/messaging/models/bandwidth_message_item.py
--rw-r--r--   0 root         (0) root         (0)     2295 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/messaging/models/bandwidth_messages_list.py
--rw-r--r--   0 root         (0) root         (0)     1658 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/messaging/models/deferred_result.py
--rw-r--r--   0 root         (0) root         (0)     3698 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/messaging/models/media.py
--rw-r--r--   0 root         (0) root         (0)     3216 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/messaging/models/message_request.py
--rw-r--r--   0 root         (0) root         (0)     2306 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/messaging/models/page_info.py
--rw-r--r--   0 root         (0) root         (0)      560 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/messaging/models/priority_enum.py
--rw-r--r--   0 root         (0) root         (0)     1523 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/messaging/models/tag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.431155 bandwidth-sdk-9.1.0/bandwidth/models/
--rw-r--r--   0 root         (0) root         (0)        0 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.431155 bandwidth-sdk-9.1.0/bandwidth/twofactorauth/
--rw-r--r--   0 root         (0) root         (0)       99 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/twofactorauth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.431155 bandwidth-sdk-9.1.0/bandwidth/twofactorauth/controllers/
--rw-r--r--   0 root         (0) root         (0)       61 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/twofactorauth/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3095 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/twofactorauth/controllers/base_controller.py
--rw-r--r--   0 root         (0) root         (0)     9619 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/twofactorauth/controllers/mfa_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.431155 bandwidth-sdk-9.1.0/bandwidth/twofactorauth/exceptions/
--rw-r--r--   0 root         (0) root         (0)      126 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/twofactorauth/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1336 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/twofactorauth/exceptions/error_with_request_exception.py
--rw-r--r--   0 root         (0) root         (0)     1285 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/twofactorauth/exceptions/forbidden_request_exception.py
--rw-r--r--   0 root         (0) root         (0)     1294 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/twofactorauth/exceptions/unauthorized_request_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.435155 bandwidth-sdk-9.1.0/bandwidth/twofactorauth/models/
--rw-r--r--   0 root         (0) root         (0)      206 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/twofactorauth/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3294 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/twofactorauth/models/two_factor_code_request_schema.py
--rw-r--r--   0 root         (0) root         (0)     1446 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/twofactorauth/models/two_factor_messaging_response.py
--rw-r--r--   0 root         (0) root         (0)     1404 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/twofactorauth/models/two_factor_verify_code_response.py
--rw-r--r--   0 root         (0) root         (0)     2914 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/twofactorauth/models/two_factor_verify_request_schema.py
--rw-r--r--   0 root         (0) root         (0)     1407 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/twofactorauth/models/two_factor_voice_response.py
--rw-r--r--   0 root         (0) root         (0)     2424 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/twofactorauth/two_factor_auth_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.435155 bandwidth-sdk-9.1.0/bandwidth/utilities/
--rw-r--r--   0 root         (0) root         (0)       38 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      542 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/utilities/file_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.435155 bandwidth-sdk-9.1.0/bandwidth/voice/
--rw-r--r--   0 root         (0) root         (0)      104 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.435155 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/
--rw-r--r--   0 root         (0) root         (0)       43 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/__init__.py
--rw-r--r--   0 root         (0) root         (0)      907 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.439155 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/
--rw-r--r--   0 root         (0) root         (0)      727 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      350 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/base_verb.py
--rw-r--r--   0 root         (0) root         (0)     4526 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/bridge.py
--rw-r--r--   0 root         (0) root         (0)     4046 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/conference.py
--rw-r--r--   0 root         (0) root         (0)     1594 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/forward.py
--rw-r--r--   0 root         (0) root         (0)     4887 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/gather.py
--rw-r--r--   0 root         (0) root         (0)      218 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/hangup.py
--rw-r--r--   0 root         (0) root         (0)      626 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/pause.py
--rw-r--r--   0 root         (0) root         (0)      251 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/pause_recording.py
--rw-r--r--   0 root         (0) root         (0)     3993 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/phone_number.py
--rw-r--r--   0 root         (0) root         (0)     1285 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/play_audio.py
--rw-r--r--   0 root         (0) root         (0)     5555 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/record.py
--rw-r--r--   0 root         (0) root         (0)     2679 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/redirect.py
--rw-r--r--   0 root         (0) root         (0)      255 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/resume_recording.py
--rw-r--r--   0 root         (0) root         (0)      618 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/ring.py
--rw-r--r--   0 root         (0) root         (0)     1096 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/send_dtmf.py
--rw-r--r--   0 root         (0) root         (0)     4156 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/sip_uri.py
--rw-r--r--   0 root         (0) root         (0)     1531 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/speak_sentence.py
--rw-r--r--   0 root         (0) root         (0)     1441 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/start_gather.py
--rw-r--r--   0 root         (0) root         (0)     3421 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/start_recording.py
--rw-r--r--   0 root         (0) root         (0)      234 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/stop_gather.py
--rw-r--r--   0 root         (0) root         (0)      247 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/stop_recording.py
--rw-r--r--   0 root         (0) root         (0)      846 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/tag.py
--rw-r--r--   0 root         (0) root         (0)     4637 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/transfer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.439155 bandwidth-sdk-9.1.0/bandwidth/voice/controllers/
--rw-r--r--   0 root         (0) root         (0)       61 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75108 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/controllers/api_controller.py
--rw-r--r--   0 root         (0) root         (0)     3095 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/controllers/base_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.443156 bandwidth-sdk-9.1.0/bandwidth/voice/exceptions/
--rw-r--r--   0 root         (0) root         (0)       51 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1378 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/exceptions/api_error_response_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.447156 bandwidth-sdk-9.1.0/bandwidth/voice/models/
--rw-r--r--   0 root         (0) root         (0)      895 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      435 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/answer_fallback_method_enum.py
--rw-r--r--   0 root         (0) root         (0)      419 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/answer_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     6706 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/api_call_response.py
--rw-r--r--   0 root         (0) root         (0)     5493 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/api_call_state_response.py
--rw-r--r--   0 root         (0) root         (0)     6617 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/api_create_call_request.py
--rw-r--r--   0 root         (0) root         (0)     4001 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/api_modify_call_request.py
--rw-r--r--   0 root         (0) root         (0)     3839 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/api_modify_conference_request.py
--rw-r--r--   0 root         (0) root         (0)     2740 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/api_transcribe_recording_request.py
--rw-r--r--   0 root         (0) root         (0)      831 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/callback_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     3912 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/conference_detail.py
--rw-r--r--   0 root         (0) root         (0)      845 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/conference_event_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     2643 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/conference_member_detail.py
--rw-r--r--   0 root         (0) root         (0)     4204 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/conference_recording_metadata_response.py
--rw-r--r--   0 root         (0) root         (0)      437 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/direction_enum.py
--rw-r--r--   0 root         (0) root         (0)     1285 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/disconnect_cause_enum.py
--rw-r--r--   0 root         (0) root         (0)      427 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/disconnect_method_enum.py
--rw-r--r--   0 root         (0) root         (0)      412 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/file_format_enum.py
--rw-r--r--   0 root         (0) root         (0)     1401 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/modify_call_recording_state.py
--rw-r--r--   0 root         (0) root         (0)     6132 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/recording_metadata_response.py
--rw-r--r--   0 root         (0) root         (0)      439 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/redirect_fallback_method_enum.py
--rw-r--r--   0 root         (0) root         (0)      423 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/redirect_method_enum.py
--rw-r--r--   0 root         (0) root         (0)      431 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/state_1_enum.py
--rw-r--r--   0 root         (0) root         (0)      523 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/state_2_enum.py
--rw-r--r--   0 root         (0) root         (0)      524 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/state_enum.py
--rw-r--r--   0 root         (0) root         (0)      764 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/status_1_enum.py
--rw-r--r--   0 root         (0) root         (0)      854 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/status_3_enum.py
--rw-r--r--   0 root         (0) root         (0)      431 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/status_enum.py
--rw-r--r--   0 root         (0) root         (0)     1597 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/transcript.py
--rw-r--r--   0 root         (0) root         (0)     2033 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/transcription.py
--rw-r--r--   0 root         (0) root         (0)     1640 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/models/transcription_response.py
--rw-r--r--   0 root         (0) root         (0)     2411 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/voice/voice_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.447156 bandwidth-sdk-9.1.0/bandwidth/webrtc/
--rw-r--r--   0 root         (0) root         (0)       91 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/webrtc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.447156 bandwidth-sdk-9.1.0/bandwidth/webrtc/controllers/
--rw-r--r--   0 root         (0) root         (0)       61 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/webrtc/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28856 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/webrtc/controllers/api_controller.py
--rw-r--r--   0 root         (0) root         (0)     3095 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/webrtc/controllers/base_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.447156 bandwidth-sdk-9.1.0/bandwidth/webrtc/exceptions/
--rw-r--r--   0 root         (0) root         (0)       38 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/webrtc/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1296 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/webrtc/exceptions/error_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.447156 bandwidth-sdk-9.1.0/bandwidth/webrtc/models/
--rw-r--r--   0 root         (0) root         (0)      208 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/webrtc/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1922 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/webrtc/models/accounts_participants_response.py
--rw-r--r--   0 root         (0) root         (0)      452 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/webrtc/models/device_api_version_enum.py
--rw-r--r--   0 root         (0) root         (0)     3397 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/webrtc/models/participant.py
--rw-r--r--   0 root         (0) root         (0)     1508 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/webrtc/models/participant_subscription.py
--rw-r--r--   0 root         (0) root         (0)      438 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/webrtc/models/publish_permission_enum.py
--rw-r--r--   0 root         (0) root         (0)     1504 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/webrtc/models/session.py
--rw-r--r--   0 root         (0) root         (0)     2198 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/webrtc/models/subscriptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.451156 bandwidth-sdk-9.1.0/bandwidth/webrtc/utils/
--rw-r--r--   0 root         (0) root         (0)       50 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/webrtc/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      467 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/webrtc/utils/transfer_util.py
--rw-r--r--   0 root         (0) root         (0)     2413 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/bandwidth/webrtc/web_rtc_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.451156 bandwidth-sdk-9.1.0/bandwidth_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      282 2021-03-23 18:36:52.000000 bandwidth-sdk-9.1.0/bandwidth_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6459 2021-03-23 18:36:52.000000 bandwidth-sdk-9.1.0/bandwidth_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-03-23 18:36:52.000000 bandwidth-sdk-9.1.0/bandwidth_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      124 2021-03-23 18:36:52.000000 bandwidth-sdk-9.1.0/bandwidth_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2021-03-23 18:36:52.000000 bandwidth-sdk-9.1.0/bandwidth_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-03-23 18:36:52.451156 bandwidth-sdk-9.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      867 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.451156 bandwidth-sdk-9.1.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.451156 bandwidth-sdk-9.1.0/tests/controllers/
--rw-r--r--   0 root         (0) root         (0)        0 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/tests/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      882 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/tests/controllers/controller_test_base.py
--rw-r--r--   0 root         (0) root         (0)      655 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/tests/http_response_catcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-23 18:36:52.451156 bandwidth-sdk-9.1.0/tests/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/tests/integration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6434 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/tests/integration/api_tests.py
--rw-r--r--   0 root         (0) root         (0)    18389 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/tests/integration/bxml_tests.py
--rw-r--r--   0 root         (0) root         (0)     5112 2021-03-23 18:36:22.000000 bandwidth-sdk-9.1.0/tests/test_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.352018 bandwidth-sdk-9.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1213 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5815 2021-06-23 14:35:21.352018 bandwidth-sdk-9.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5529 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.332017 bandwidth-sdk-9.2.0/bandwidth/
+-rw-r--r--   0 root         (0) root         (0)      166 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14077 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/api_helper.py
+-rw-r--r--   0 root         (0) root         (0)     3554 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/bandwidth_client.py
+-rw-r--r--   0 root         (0) root         (0)    10125 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.332017 bandwidth-sdk-9.2.0/bandwidth/controllers/
+-rw-r--r--   0 root         (0) root         (0)       38 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3095 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/controllers/base_controller.py
+-rw-r--r--   0 root         (0) root         (0)      504 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.332017 bandwidth-sdk-9.2.0/bandwidth/exceptions/
+-rw-r--r--   0 root         (0) root         (0)       36 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      884 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/exceptions/api_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.336017 bandwidth-sdk-9.2.0/bandwidth/http/
+-rw-r--r--   0 root         (0) root         (0)      162 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/http/api_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.336017 bandwidth-sdk-9.2.0/bandwidth/http/auth/
+-rw-r--r--   0 root         (0) root         (0)      130 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/http/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      925 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/http/auth/messaging_basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)      923 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/http/auth/phone_number_lookup_basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)      941 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/http/auth/two_factor_auth_basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)      913 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/http/auth/voice_basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)      918 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/http/auth/web_rtc_basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/http/http_call_back.py
+-rw-r--r--   0 root         (0) root         (0)     7255 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/http/http_client.py
+-rw-r--r--   0 root         (0) root         (0)      915 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/http/http_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     2826 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/http/http_request.py
+-rw-r--r--   0 root         (0) root         (0)     1495 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/http/http_response.py
+-rw-r--r--   0 root         (0) root         (0)     3682 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/http/requests_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.336017 bandwidth-sdk-9.2.0/bandwidth/messaging/
+-rw-r--r--   0 root         (0) root         (0)       93 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/messaging/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.336017 bandwidth-sdk-9.2.0/bandwidth/messaging/controllers/
+-rw-r--r--   0 root         (0) root         (0)       61 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/messaging/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19903 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/messaging/controllers/api_controller.py
+-rw-r--r--   0 root         (0) root         (0)     3095 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/messaging/controllers/base_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.336017 bandwidth-sdk-9.2.0/bandwidth/messaging/exceptions/
+-rw-r--r--   0 root         (0) root         (0)       42 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/messaging/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1317 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/messaging/exceptions/messaging_exception.py
+-rw-r--r--   0 root         (0) root         (0)     2419 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/messaging/messaging_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.336017 bandwidth-sdk-9.2.0/bandwidth/messaging/models/
+-rw-r--r--   0 root         (0) root         (0)      252 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/messaging/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2667 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/messaging/models/bandwidth_callback_message.py
+-rw-r--r--   0 root         (0) root         (0)     4065 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/messaging/models/bandwidth_message.py
+-rw-r--r--   0 root         (0) root         (0)     4284 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/messaging/models/bandwidth_message_item.py
+-rw-r--r--   0 root         (0) root         (0)     2295 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/messaging/models/bandwidth_messages_list.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/messaging/models/deferred_result.py
+-rw-r--r--   0 root         (0) root         (0)     3698 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/messaging/models/media.py
+-rw-r--r--   0 root         (0) root         (0)     3216 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/messaging/models/message_request.py
+-rw-r--r--   0 root         (0) root         (0)     2306 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/messaging/models/page_info.py
+-rw-r--r--   0 root         (0) root         (0)      560 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/messaging/models/priority_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/messaging/models/tag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.336017 bandwidth-sdk-9.2.0/bandwidth/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.336017 bandwidth-sdk-9.2.0/bandwidth/phonenumberlookup/
+-rw-r--r--   0 root         (0) root         (0)       99 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/phonenumberlookup/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.340017 bandwidth-sdk-9.2.0/bandwidth/phonenumberlookup/controllers/
+-rw-r--r--   0 root         (0) root         (0)       59 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/phonenumberlookup/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51140 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/phonenumberlookup/controllers/api_controller.py
+-rw-r--r--   0 root         (0) root         (0)     3001 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/phonenumberlookup/controllers/base_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.340017 bandwidth-sdk-9.2.0/bandwidth/phonenumberlookup/exceptions/
+-rw-r--r--   0 root         (0) root         (0)       59 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/phonenumberlookup/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1272 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/phonenumberlookup/exceptions/accounts_tnlookup_400_error_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.340017 bandwidth-sdk-9.2.0/bandwidth/phonenumberlookup/models/
+-rw-r--r--   0 root         (0) root         (0)       91 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/phonenumberlookup/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1287 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/phonenumberlookup/models/order_request.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/phonenumberlookup/models/order_response.py
+-rw-r--r--   0 root         (0) root         (0)     2752 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/phonenumberlookup/models/order_status.py
+-rw-r--r--   0 root         (0) root         (0)     3569 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/phonenumberlookup/models/result.py
+-rw-r--r--   0 root         (0) root         (0)     3133 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/phonenumberlookup/phone_number_lookup_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.340017 bandwidth-sdk-9.2.0/bandwidth/twofactorauth/
+-rw-r--r--   0 root         (0) root         (0)       99 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/twofactorauth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.340017 bandwidth-sdk-9.2.0/bandwidth/twofactorauth/controllers/
+-rw-r--r--   0 root         (0) root         (0)       61 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/twofactorauth/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3095 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/twofactorauth/controllers/base_controller.py
+-rw-r--r--   0 root         (0) root         (0)     9619 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/twofactorauth/controllers/mfa_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.340017 bandwidth-sdk-9.2.0/bandwidth/twofactorauth/exceptions/
+-rw-r--r--   0 root         (0) root         (0)      126 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/twofactorauth/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/twofactorauth/exceptions/error_with_request_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/twofactorauth/exceptions/forbidden_request_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1294 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/twofactorauth/exceptions/unauthorized_request_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.340017 bandwidth-sdk-9.2.0/bandwidth/twofactorauth/models/
+-rw-r--r--   0 root         (0) root         (0)      206 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/twofactorauth/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3294 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/twofactorauth/models/two_factor_code_request_schema.py
+-rw-r--r--   0 root         (0) root         (0)     1446 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/twofactorauth/models/two_factor_messaging_response.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/twofactorauth/models/two_factor_verify_code_response.py
+-rw-r--r--   0 root         (0) root         (0)     2914 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/twofactorauth/models/two_factor_verify_request_schema.py
+-rw-r--r--   0 root         (0) root         (0)     1407 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/twofactorauth/models/two_factor_voice_response.py
+-rw-r--r--   0 root         (0) root         (0)     2424 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/twofactorauth/two_factor_auth_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.340017 bandwidth-sdk-9.2.0/bandwidth/utilities/
+-rw-r--r--   0 root         (0) root         (0)       38 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      542 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/utilities/file_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.340017 bandwidth-sdk-9.2.0/bandwidth/voice/
+-rw-r--r--   0 root         (0) root         (0)      104 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.340017 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/
+-rw-r--r--   0 root         (0) root         (0)       43 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      907 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.344018 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/
+-rw-r--r--   0 root         (0) root         (0)      727 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      350 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/base_verb.py
+-rw-r--r--   0 root         (0) root         (0)     4526 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/bridge.py
+-rw-r--r--   0 root         (0) root         (0)     4046 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/conference.py
+-rw-r--r--   0 root         (0) root         (0)     1594 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/forward.py
+-rw-r--r--   0 root         (0) root         (0)     4887 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/gather.py
+-rw-r--r--   0 root         (0) root         (0)      218 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/hangup.py
+-rw-r--r--   0 root         (0) root         (0)      626 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/pause.py
+-rw-r--r--   0 root         (0) root         (0)      251 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/pause_recording.py
+-rw-r--r--   0 root         (0) root         (0)     3993 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/phone_number.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/play_audio.py
+-rw-r--r--   0 root         (0) root         (0)     5555 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/record.py
+-rw-r--r--   0 root         (0) root         (0)     2679 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/redirect.py
+-rw-r--r--   0 root         (0) root         (0)      255 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/resume_recording.py
+-rw-r--r--   0 root         (0) root         (0)      618 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/ring.py
+-rw-r--r--   0 root         (0) root         (0)     1096 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/send_dtmf.py
+-rw-r--r--   0 root         (0) root         (0)     4156 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/sip_uri.py
+-rw-r--r--   0 root         (0) root         (0)     1531 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/speak_sentence.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/start_gather.py
+-rw-r--r--   0 root         (0) root         (0)     3421 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/start_recording.py
+-rw-r--r--   0 root         (0) root         (0)      234 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/stop_gather.py
+-rw-r--r--   0 root         (0) root         (0)      247 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/stop_recording.py
+-rw-r--r--   0 root         (0) root         (0)      846 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/tag.py
+-rw-r--r--   0 root         (0) root         (0)     4637 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/transfer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.344018 bandwidth-sdk-9.2.0/bandwidth/voice/controllers/
+-rw-r--r--   0 root         (0) root         (0)       61 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75108 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/controllers/api_controller.py
+-rw-r--r--   0 root         (0) root         (0)     3095 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/controllers/base_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.344018 bandwidth-sdk-9.2.0/bandwidth/voice/exceptions/
+-rw-r--r--   0 root         (0) root         (0)       51 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1378 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/exceptions/api_error_response_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.348018 bandwidth-sdk-9.2.0/bandwidth/voice/models/
+-rw-r--r--   0 root         (0) root         (0)      895 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      435 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/answer_fallback_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)      419 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/answer_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     6706 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/api_call_response.py
+-rw-r--r--   0 root         (0) root         (0)     5493 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/api_call_state_response.py
+-rw-r--r--   0 root         (0) root         (0)     6617 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/api_create_call_request.py
+-rw-r--r--   0 root         (0) root         (0)     4001 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/api_modify_call_request.py
+-rw-r--r--   0 root         (0) root         (0)     3839 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/api_modify_conference_request.py
+-rw-r--r--   0 root         (0) root         (0)     2740 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/api_transcribe_recording_request.py
+-rw-r--r--   0 root         (0) root         (0)      831 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/callback_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     3912 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/conference_detail.py
+-rw-r--r--   0 root         (0) root         (0)      845 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/conference_event_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     2643 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/conference_member_detail.py
+-rw-r--r--   0 root         (0) root         (0)     4204 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/conference_recording_metadata_response.py
+-rw-r--r--   0 root         (0) root         (0)      437 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/direction_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/disconnect_cause_enum.py
+-rw-r--r--   0 root         (0) root         (0)      427 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/disconnect_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)      412 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/file_format_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1401 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/modify_call_recording_state.py
+-rw-r--r--   0 root         (0) root         (0)     6132 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/recording_metadata_response.py
+-rw-r--r--   0 root         (0) root         (0)      439 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/redirect_fallback_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)      423 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/redirect_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)      431 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/state_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)      523 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/state_2_enum.py
+-rw-r--r--   0 root         (0) root         (0)      524 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/state_enum.py
+-rw-r--r--   0 root         (0) root         (0)      764 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/status_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)      854 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/status_3_enum.py
+-rw-r--r--   0 root         (0) root         (0)      431 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/status_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1597 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/transcript.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/transcription.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/models/transcription_response.py
+-rw-r--r--   0 root         (0) root         (0)     2411 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/voice/voice_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.348018 bandwidth-sdk-9.2.0/bandwidth/webrtc/
+-rw-r--r--   0 root         (0) root         (0)       91 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/webrtc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.348018 bandwidth-sdk-9.2.0/bandwidth/webrtc/controllers/
+-rw-r--r--   0 root         (0) root         (0)       61 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/webrtc/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28856 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/webrtc/controllers/api_controller.py
+-rw-r--r--   0 root         (0) root         (0)     3095 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/webrtc/controllers/base_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.348018 bandwidth-sdk-9.2.0/bandwidth/webrtc/exceptions/
+-rw-r--r--   0 root         (0) root         (0)       38 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/webrtc/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1296 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/webrtc/exceptions/error_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.352018 bandwidth-sdk-9.2.0/bandwidth/webrtc/models/
+-rw-r--r--   0 root         (0) root         (0)      208 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/webrtc/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/webrtc/models/accounts_participants_response.py
+-rw-r--r--   0 root         (0) root         (0)      452 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/webrtc/models/device_api_version_enum.py
+-rw-r--r--   0 root         (0) root         (0)     3397 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/webrtc/models/participant.py
+-rw-r--r--   0 root         (0) root         (0)     1508 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/webrtc/models/participant_subscription.py
+-rw-r--r--   0 root         (0) root         (0)      438 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/webrtc/models/publish_permission_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1504 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/webrtc/models/session.py
+-rw-r--r--   0 root         (0) root         (0)     2198 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/webrtc/models/subscriptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.352018 bandwidth-sdk-9.2.0/bandwidth/webrtc/utils/
+-rw-r--r--   0 root         (0) root         (0)       50 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/webrtc/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      467 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/webrtc/utils/transfer_util.py
+-rw-r--r--   0 root         (0) root         (0)     2413 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/bandwidth/webrtc/web_rtc_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.352018 bandwidth-sdk-9.2.0/bandwidth_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5815 2021-06-23 14:35:21.000000 bandwidth-sdk-9.2.0/bandwidth_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7159 2021-06-23 14:35:21.000000 bandwidth-sdk-9.2.0/bandwidth_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-06-23 14:35:21.000000 bandwidth-sdk-9.2.0/bandwidth_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      124 2021-06-23 14:35:21.000000 bandwidth-sdk-9.2.0/bandwidth_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2021-06-23 14:35:21.000000 bandwidth-sdk-9.2.0/bandwidth_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2021-06-23 14:35:21.352018 bandwidth-sdk-9.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      867 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.352018 bandwidth-sdk-9.2.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.352018 bandwidth-sdk-9.2.0/tests/controllers/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/tests/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      882 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/tests/controllers/controller_test_base.py
+-rw-r--r--   0 root         (0) root         (0)      655 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/tests/http_response_catcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 14:35:21.352018 bandwidth-sdk-9.2.0/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/tests/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7214 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/tests/integration/api_tests.py
+-rw-r--r--   0 root         (0) root         (0)    18389 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/tests/integration/bxml_tests.py
+-rw-r--r--   0 root         (0) root         (0)     5112 2021-06-23 14:34:45.000000 bandwidth-sdk-9.2.0/tests/test_helper.py
```

### Comparing `bandwidth-sdk-9.1.0/LICENSE` & `bandwidth-sdk-9.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/api_helper.py` & `bandwidth-sdk-9.2.0/bandwidth/api_helper.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/bandwidth_client.py` & `bandwidth-sdk-9.2.0/bandwidth/bandwidth_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 
 from bandwidth.decorators import lazy_property
 from bandwidth.configuration import Configuration
 from bandwidth.configuration import Environment
 from bandwidth.messaging.messaging_client import MessagingClient
 from bandwidth.twofactorauth.two_factor_auth_client import TwoFactorAuthClient
+from bandwidth.phonenumberlookup.phone_number_lookup_client import PhoneNumberLookupClient
 from bandwidth.voice.voice_client import VoiceClient
 from bandwidth.webrtc.web_rtc_client import WebRtcClient
 
 
 class BandwidthClient(object):
 
     @lazy_property
@@ -22,41 +23,49 @@
         return MessagingClient(config=self.config)
 
     @lazy_property
     def two_factor_auth_client(self):
         return TwoFactorAuthClient(config=self.config)
 
     @lazy_property
+    def phone_number_lookup_client(self):
+        return PhoneNumberLookupClient(config=self.config)
+
+    @lazy_property
     def voice_client(self):
         return VoiceClient(config=self.config)
 
     @lazy_property
     def web_rtc_client(self):
         return WebRtcClient(config=self.config)
 
     def __init__(self, timeout=60, max_retries=3, backoff_factor=0,
                  environment=Environment.PRODUCTION,
                  base_url='https://www.example.com',
                  messaging_basic_auth_user_name='TODO: Replace',
                  messaging_basic_auth_password='TODO: Replace',
                  two_factor_auth_basic_auth_user_name='TODO: Replace',
                  two_factor_auth_basic_auth_password='TODO: Replace',
+                 phone_number_lookup_basic_auth_user_name='TODO: Replace',
+                 phone_number_lookup_basic_auth_password='TODO: Replace',
                  voice_basic_auth_user_name='TODO: Replace',
                  voice_basic_auth_password='TODO: Replace',
                  web_rtc_basic_auth_user_name='TODO: Replace',
                  web_rtc_basic_auth_password='TODO: Replace', config=None):
         if config is None:
             self.config = Configuration(timeout=timeout,
                                         max_retries=max_retries,
                                         backoff_factor=backoff_factor,
                                         environment=environment,
                                         base_url=base_url,
                                         messaging_basic_auth_user_name=messaging_basic_auth_user_name,
                                         messaging_basic_auth_password=messaging_basic_auth_password,
                                         two_factor_auth_basic_auth_user_name=two_factor_auth_basic_auth_user_name,
                                         two_factor_auth_basic_auth_password=two_factor_auth_basic_auth_password,
+                                        phone_number_lookup_basic_auth_user_name=phone_number_lookup_basic_auth_user_name,
+                                        phone_number_lookup_basic_auth_password=phone_number_lookup_basic_auth_password,
                                         voice_basic_auth_user_name=voice_basic_auth_user_name,
                                         voice_basic_auth_password=voice_basic_auth_password,
                                         web_rtc_basic_auth_user_name=web_rtc_basic_auth_user_name,
                                         web_rtc_basic_auth_password=web_rtc_basic_auth_password)
         else:
             self.config = config
```

### Comparing `bandwidth-sdk-9.1.0/bandwidth/configuration.py` & `bandwidth-sdk-9.2.0/bandwidth/configuration.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 
 
 class Server(Enum):
     """An enum for API servers"""
     DEFAULT = 0
     MESSAGINGDEFAULT = 1
     TWOFACTORAUTHDEFAULT = 2
-    VOICEDEFAULT = 3
-    WEBRTCDEFAULT = 4
+    PHONENUMBERLOOKUPDEFAULT = 3
+    VOICEDEFAULT = 4
+    WEBRTCDEFAULT = 5
 
 
 class Configuration(object):
     """A class used for configuring the SDK by a user.
     """
 
     @property
@@ -67,14 +68,22 @@
         return self._two_factor_auth_basic_auth_user_name
 
     @property
     def two_factor_auth_basic_auth_password(self):
         return self._two_factor_auth_basic_auth_password
 
     @property
+    def phone_number_lookup_basic_auth_user_name(self):
+        return self._phone_number_lookup_basic_auth_user_name
+
+    @property
+    def phone_number_lookup_basic_auth_password(self):
+        return self._phone_number_lookup_basic_auth_password
+
+    @property
     def voice_basic_auth_user_name(self):
         return self._voice_basic_auth_user_name
 
     @property
     def voice_basic_auth_password(self):
         return self._voice_basic_auth_password
 
@@ -89,14 +98,16 @@
     def __init__(self, timeout=60, max_retries=3, backoff_factor=0,
                  environment=Environment.PRODUCTION,
                  base_url='https://www.example.com',
                  messaging_basic_auth_user_name='TODO: Replace',
                  messaging_basic_auth_password='TODO: Replace',
                  two_factor_auth_basic_auth_user_name='TODO: Replace',
                  two_factor_auth_basic_auth_password='TODO: Replace',
+                 phone_number_lookup_basic_auth_user_name='TODO: Replace',
+                 phone_number_lookup_basic_auth_password='TODO: Replace',
                  voice_basic_auth_user_name='TODO: Replace',
                  voice_basic_auth_password='TODO: Replace',
                  web_rtc_basic_auth_user_name='TODO: Replace',
                  web_rtc_basic_auth_password='TODO: Replace'):
         # The value to use for connection timeout
         self._timeout = timeout
 
@@ -123,14 +134,20 @@
         # The username to use with basic authentication
         self._two_factor_auth_basic_auth_user_name = two_factor_auth_basic_auth_user_name
 
         # The password to use with basic authentication
         self._two_factor_auth_basic_auth_password = two_factor_auth_basic_auth_password
 
         # The username to use with basic authentication
+        self._phone_number_lookup_basic_auth_user_name = phone_number_lookup_basic_auth_user_name
+
+        # The password to use with basic authentication
+        self._phone_number_lookup_basic_auth_password = phone_number_lookup_basic_auth_password
+
+        # The username to use with basic authentication
         self._voice_basic_auth_user_name = voice_basic_auth_user_name
 
         # The password to use with basic authentication
         self._voice_basic_auth_password = voice_basic_auth_password
 
         # The username to use with basic authentication
         self._web_rtc_basic_auth_user_name = web_rtc_basic_auth_user_name
@@ -143,39 +160,45 @@
 
     def clone_with(self, timeout=None, max_retries=None, backoff_factor=None,
                    environment=None, base_url=None,
                    messaging_basic_auth_user_name=None,
                    messaging_basic_auth_password=None,
                    two_factor_auth_basic_auth_user_name=None,
                    two_factor_auth_basic_auth_password=None,
+                   phone_number_lookup_basic_auth_user_name=None,
+                   phone_number_lookup_basic_auth_password=None,
                    voice_basic_auth_user_name=None,
                    voice_basic_auth_password=None,
                    web_rtc_basic_auth_user_name=None,
                    web_rtc_basic_auth_password=None):
         timeout = timeout or self.timeout
         max_retries = max_retries or self.max_retries
         backoff_factor = backoff_factor or self.backoff_factor
         environment = environment or self.environment
         base_url = base_url or self.base_url
         messaging_basic_auth_user_name = messaging_basic_auth_user_name or self.messaging_basic_auth_user_name
         messaging_basic_auth_password = messaging_basic_auth_password or self.messaging_basic_auth_password
         two_factor_auth_basic_auth_user_name = two_factor_auth_basic_auth_user_name or self.two_factor_auth_basic_auth_user_name
         two_factor_auth_basic_auth_password = two_factor_auth_basic_auth_password or self.two_factor_auth_basic_auth_password
+        phone_number_lookup_basic_auth_user_name = phone_number_lookup_basic_auth_user_name or self.phone_number_lookup_basic_auth_user_name
+        phone_number_lookup_basic_auth_password = phone_number_lookup_basic_auth_password or self.phone_number_lookup_basic_auth_password
         voice_basic_auth_user_name = voice_basic_auth_user_name or self.voice_basic_auth_user_name
         voice_basic_auth_password = voice_basic_auth_password or self.voice_basic_auth_password
         web_rtc_basic_auth_user_name = web_rtc_basic_auth_user_name or self.web_rtc_basic_auth_user_name
         web_rtc_basic_auth_password = web_rtc_basic_auth_password or self.web_rtc_basic_auth_password
 
         return Configuration(
             timeout=timeout, max_retries=max_retries,
             backoff_factor=backoff_factor, environment=environment, base_url=base_url,
             messaging_basic_auth_user_name=messaging_basic_auth_user_name,
             messaging_basic_auth_password=messaging_basic_auth_password,
             two_factor_auth_basic_auth_user_name=two_factor_auth_basic_auth_user_name,
             two_factor_auth_basic_auth_password=two_factor_auth_basic_auth_password,
+            phone_number_lookup_basic_auth_user_name=phone_number_lookup_basic_auth_user_name,
+            phone_number_lookup_basic_auth_password=phone_number_lookup_basic_auth_password,
             voice_basic_auth_user_name=voice_basic_auth_user_name,
             voice_basic_auth_password=voice_basic_auth_password,
             web_rtc_basic_auth_user_name=web_rtc_basic_auth_user_name,
             web_rtc_basic_auth_password=web_rtc_basic_auth_password
         )
 
     def create_http_client(self):
@@ -185,21 +208,23 @@
 
     # All the environments the SDK can run in
     environments = {
         Environment.PRODUCTION: {
             Server.DEFAULT: 'api.bandwidth.com',
             Server.MESSAGINGDEFAULT: 'https://messaging.bandwidth.com/api/v2',
             Server.TWOFACTORAUTHDEFAULT: 'https://mfa.bandwidth.com/api/v1',
+            Server.PHONENUMBERLOOKUPDEFAULT: 'https://numbers.bandwidth.com/api/v1',
             Server.VOICEDEFAULT: 'https://voice.bandwidth.com',
             Server.WEBRTCDEFAULT: 'https://api.webrtc.bandwidth.com/v1'
         },
         Environment.CUSTOM: {
             Server.DEFAULT: '{base_url}',
             Server.MESSAGINGDEFAULT: '{base_url}',
             Server.TWOFACTORAUTHDEFAULT: '{base_url}',
+            Server.PHONENUMBERLOOKUPDEFAULT: '{base_url}',
             Server.VOICEDEFAULT: '{base_url}',
             Server.WEBRTCDEFAULT: '{base_url}'
         }
     }
 
     def get_base_uri(self, server=Server.DEFAULT):
         """Generates the appropriate base URI for the environment and the
```

### Comparing `bandwidth-sdk-9.1.0/bandwidth/controllers/base_controller.py` & `bandwidth-sdk-9.2.0/bandwidth/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/exceptions/api_exception.py` & `bandwidth-sdk-9.2.0/bandwidth/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/http/api_response.py` & `bandwidth-sdk-9.2.0/bandwidth/http/api_response.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/http/auth/messaging_basic_auth.py` & `bandwidth-sdk-9.2.0/bandwidth/http/auth/messaging_basic_auth.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/http/auth/two_factor_auth_basic_auth.py` & `bandwidth-sdk-9.2.0/bandwidth/http/auth/two_factor_auth_basic_auth.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/http/auth/voice_basic_auth.py` & `bandwidth-sdk-9.2.0/bandwidth/http/auth/voice_basic_auth.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/http/auth/web_rtc_basic_auth.py` & `bandwidth-sdk-9.2.0/bandwidth/http/auth/web_rtc_basic_auth.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/http/http_call_back.py` & `bandwidth-sdk-9.2.0/bandwidth/http/http_call_back.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/http/http_client.py` & `bandwidth-sdk-9.2.0/bandwidth/http/http_client.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/http/http_method_enum.py` & `bandwidth-sdk-9.2.0/bandwidth/http/http_method_enum.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/http/http_request.py` & `bandwidth-sdk-9.2.0/bandwidth/http/http_request.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/http/http_response.py` & `bandwidth-sdk-9.2.0/bandwidth/http/http_response.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/http/requests_client.py` & `bandwidth-sdk-9.2.0/bandwidth/http/requests_client.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/messaging/controllers/api_controller.py` & `bandwidth-sdk-9.2.0/bandwidth/messaging/controllers/api_controller.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/messaging/controllers/base_controller.py` & `bandwidth-sdk-9.2.0/bandwidth/messaging/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/messaging/exceptions/messaging_exception.py` & `bandwidth-sdk-9.2.0/bandwidth/messaging/exceptions/messaging_exception.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/messaging/messaging_client.py` & `bandwidth-sdk-9.2.0/bandwidth/messaging/messaging_client.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/messaging/models/bandwidth_callback_message.py` & `bandwidth-sdk-9.2.0/bandwidth/messaging/models/bandwidth_callback_message.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/messaging/models/bandwidth_message.py` & `bandwidth-sdk-9.2.0/bandwidth/messaging/models/bandwidth_message.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/messaging/models/bandwidth_message_item.py` & `bandwidth-sdk-9.2.0/bandwidth/messaging/models/bandwidth_message_item.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/messaging/models/bandwidth_messages_list.py` & `bandwidth-sdk-9.2.0/bandwidth/messaging/models/bandwidth_messages_list.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/messaging/models/deferred_result.py` & `bandwidth-sdk-9.2.0/bandwidth/messaging/models/deferred_result.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/messaging/models/media.py` & `bandwidth-sdk-9.2.0/bandwidth/messaging/models/media.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/messaging/models/message_request.py` & `bandwidth-sdk-9.2.0/bandwidth/messaging/models/message_request.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/messaging/models/page_info.py` & `bandwidth-sdk-9.2.0/bandwidth/messaging/models/page_info.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/messaging/models/priority_enum.py` & `bandwidth-sdk-9.2.0/bandwidth/messaging/models/priority_enum.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/messaging/models/tag.py` & `bandwidth-sdk-9.2.0/bandwidth/messaging/models/tag.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/twofactorauth/controllers/base_controller.py` & `bandwidth-sdk-9.2.0/bandwidth/twofactorauth/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/twofactorauth/controllers/mfa_controller.py` & `bandwidth-sdk-9.2.0/bandwidth/twofactorauth/controllers/mfa_controller.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/twofactorauth/exceptions/error_with_request_exception.py` & `bandwidth-sdk-9.2.0/bandwidth/twofactorauth/exceptions/error_with_request_exception.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/twofactorauth/exceptions/forbidden_request_exception.py` & `bandwidth-sdk-9.2.0/bandwidth/twofactorauth/exceptions/forbidden_request_exception.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/twofactorauth/exceptions/unauthorized_request_exception.py` & `bandwidth-sdk-9.2.0/bandwidth/twofactorauth/exceptions/unauthorized_request_exception.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/twofactorauth/models/two_factor_code_request_schema.py` & `bandwidth-sdk-9.2.0/bandwidth/twofactorauth/models/two_factor_code_request_schema.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/twofactorauth/models/two_factor_messaging_response.py` & `bandwidth-sdk-9.2.0/bandwidth/twofactorauth/models/two_factor_messaging_response.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/twofactorauth/models/two_factor_verify_code_response.py` & `bandwidth-sdk-9.2.0/bandwidth/twofactorauth/models/two_factor_verify_code_response.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/twofactorauth/models/two_factor_verify_request_schema.py` & `bandwidth-sdk-9.2.0/bandwidth/twofactorauth/models/two_factor_verify_request_schema.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/twofactorauth/models/two_factor_voice_response.py` & `bandwidth-sdk-9.2.0/bandwidth/twofactorauth/models/two_factor_voice_response.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/twofactorauth/two_factor_auth_client.py` & `bandwidth-sdk-9.2.0/bandwidth/twofactorauth/two_factor_auth_client.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/utilities/file_wrapper.py` & `bandwidth-sdk-9.2.0/bandwidth/utilities/file_wrapper.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/bxml/response.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/bxml/response.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/__init__.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/__init__.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/bridge.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/bridge.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/conference.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/conference.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/forward.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/forward.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/gather.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/gather.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/pause.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/pause.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/phone_number.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/phone_number.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/play_audio.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/play_audio.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/record.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/record.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/redirect.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/redirect.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/ring.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/ring.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/send_dtmf.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/send_dtmf.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/sip_uri.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/sip_uri.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/speak_sentence.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/speak_sentence.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/start_gather.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/start_gather.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/start_recording.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/start_recording.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/tag.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/tag.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/bxml/verbs/transfer.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/bxml/verbs/transfer.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/controllers/api_controller.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/controllers/api_controller.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/controllers/base_controller.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/exceptions/api_error_response_exception.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/exceptions/api_error_response_exception.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/models/__init__.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/models/api_call_response.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/models/api_call_response.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/models/api_call_state_response.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/models/api_call_state_response.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/models/api_create_call_request.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/models/api_create_call_request.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/models/api_modify_call_request.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/models/api_modify_call_request.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/models/api_modify_conference_request.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/models/api_modify_conference_request.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/models/api_transcribe_recording_request.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/models/api_transcribe_recording_request.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/models/callback_method_enum.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/models/callback_method_enum.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/models/conference_detail.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/models/conference_detail.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/models/conference_event_method_enum.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/models/conference_event_method_enum.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/models/conference_member_detail.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/models/conference_member_detail.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/models/conference_recording_metadata_response.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/models/conference_recording_metadata_response.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/models/disconnect_cause_enum.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/models/disconnect_cause_enum.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/models/modify_call_recording_state.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/models/modify_call_recording_state.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/models/recording_metadata_response.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/models/recording_metadata_response.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/models/state_2_enum.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/models/state_2_enum.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/models/state_enum.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/models/state_enum.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/models/status_1_enum.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/models/status_1_enum.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/models/status_3_enum.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/models/status_3_enum.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/models/transcript.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/models/transcript.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/models/transcription.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/models/transcription.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/models/transcription_response.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/models/transcription_response.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/voice/voice_client.py` & `bandwidth-sdk-9.2.0/bandwidth/voice/voice_client.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/webrtc/controllers/api_controller.py` & `bandwidth-sdk-9.2.0/bandwidth/webrtc/controllers/api_controller.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/webrtc/controllers/base_controller.py` & `bandwidth-sdk-9.2.0/bandwidth/webrtc/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/webrtc/exceptions/error_exception.py` & `bandwidth-sdk-9.2.0/bandwidth/webrtc/exceptions/error_exception.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/webrtc/models/accounts_participants_response.py` & `bandwidth-sdk-9.2.0/bandwidth/webrtc/models/accounts_participants_response.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/webrtc/models/participant.py` & `bandwidth-sdk-9.2.0/bandwidth/webrtc/models/participant.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/webrtc/models/participant_subscription.py` & `bandwidth-sdk-9.2.0/bandwidth/webrtc/models/participant_subscription.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/webrtc/models/session.py` & `bandwidth-sdk-9.2.0/bandwidth/webrtc/models/session.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/webrtc/models/subscriptions.py` & `bandwidth-sdk-9.2.0/bandwidth/webrtc/models/subscriptions.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth/webrtc/web_rtc_client.py` & `bandwidth-sdk-9.2.0/bandwidth/webrtc/web_rtc_client.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/bandwidth_sdk.egg-info/SOURCES.txt` & `bandwidth-sdk-9.2.0/bandwidth_sdk.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 bandwidth/http/http_client.py
 bandwidth/http/http_method_enum.py
 bandwidth/http/http_request.py
 bandwidth/http/http_response.py
 bandwidth/http/requests_client.py
 bandwidth/http/auth/__init__.py
 bandwidth/http/auth/messaging_basic_auth.py
+bandwidth/http/auth/phone_number_lookup_basic_auth.py
 bandwidth/http/auth/two_factor_auth_basic_auth.py
 bandwidth/http/auth/voice_basic_auth.py
 bandwidth/http/auth/web_rtc_basic_auth.py
 bandwidth/messaging/__init__.py
 bandwidth/messaging/messaging_client.py
 bandwidth/messaging/controllers/__init__.py
 bandwidth/messaging/controllers/api_controller.py
@@ -39,14 +40,26 @@
 bandwidth/messaging/models/deferred_result.py
 bandwidth/messaging/models/media.py
 bandwidth/messaging/models/message_request.py
 bandwidth/messaging/models/page_info.py
 bandwidth/messaging/models/priority_enum.py
 bandwidth/messaging/models/tag.py
 bandwidth/models/__init__.py
+bandwidth/phonenumberlookup/__init__.py
+bandwidth/phonenumberlookup/phone_number_lookup_client.py
+bandwidth/phonenumberlookup/controllers/__init__.py
+bandwidth/phonenumberlookup/controllers/api_controller.py
+bandwidth/phonenumberlookup/controllers/base_controller.py
+bandwidth/phonenumberlookup/exceptions/__init__.py
+bandwidth/phonenumberlookup/exceptions/accounts_tnlookup_400_error_exception.py
+bandwidth/phonenumberlookup/models/__init__.py
+bandwidth/phonenumberlookup/models/order_request.py
+bandwidth/phonenumberlookup/models/order_response.py
+bandwidth/phonenumberlookup/models/order_status.py
+bandwidth/phonenumberlookup/models/result.py
 bandwidth/twofactorauth/__init__.py
 bandwidth/twofactorauth/two_factor_auth_client.py
 bandwidth/twofactorauth/controllers/__init__.py
 bandwidth/twofactorauth/controllers/base_controller.py
 bandwidth/twofactorauth/controllers/mfa_controller.py
 bandwidth/twofactorauth/exceptions/__init__.py
 bandwidth/twofactorauth/exceptions/error_with_request_exception.py
```

### Comparing `bandwidth-sdk-9.1.0/setup.py` & `bandwidth-sdk-9.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         long_description = fh.read()
 else:
     with open('README.md', 'r', encoding='utf-8') as fh:
         long_description = fh.read()
 
 setup(
     name='bandwidth-sdk',
-    version='9.1.0',
+    version='9.2.0',
     description='Bandwidth\'s set of APIs',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='APIMatic SDK Generator',
     author_email='support@apimatic.io',
     url='https://apimatic.io',
     packages=find_packages(),
```

### Comparing `bandwidth-sdk-9.1.0/tests/controllers/controller_test_base.py` & `bandwidth-sdk-9.2.0/tests/controllers/controller_test_base.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/tests/http_response_catcher.py` & `bandwidth-sdk-9.2.0/tests/http_response_catcher.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/tests/integration/api_tests.py` & `bandwidth-sdk-9.2.0/tests/integration/api_tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from bandwidth.bandwidth_client import BandwidthClient
 from bandwidth.messaging.exceptions.messaging_exception import MessagingException
 from bandwidth.voice.exceptions.api_error_response_exception import ApiErrorResponseException
 from bandwidth.messaging.models.message_request import MessageRequest
 from bandwidth.voice.models.api_create_call_request import ApiCreateCallRequest
 from bandwidth.twofactorauth.models.two_factor_code_request_schema import TwoFactorCodeRequestSchema
 from bandwidth.twofactorauth.models.two_factor_verify_request_schema import TwoFactorVerifyRequestSchema
+from bandwidth.phonenumberlookup.models.order_request import OrderRequest
 
 import unittest
 
 import os
 
 try:
     USERNAME = os.environ["USERNAME"]
@@ -43,19 +44,22 @@
         """
         self.bandwidth_client = BandwidthClient(
             voice_basic_auth_user_name=USERNAME,
             voice_basic_auth_password=PASSWORD,
             messaging_basic_auth_user_name=USERNAME,
             messaging_basic_auth_password=PASSWORD,
             two_factor_auth_basic_auth_user_name=USERNAME,
-            two_factor_auth_basic_auth_password=PASSWORD
+            two_factor_auth_basic_auth_password=PASSWORD,
+            phone_number_lookup_basic_auth_user_name=USERNAME,
+            phone_number_lookup_basic_auth_password=PASSWORD,
         )
         self.voice_client = self.bandwidth_client.voice_client.client
         self.messaging_client = self.bandwidth_client.messaging_client.client
         self.auth_client = self.bandwidth_client.two_factor_auth_client.mfa
+        self.tn_lookup_client = self.bandwidth_client.phone_number_lookup_client.client
 
     def test_create_message(self):
         body = MessageRequest()
         body.application_id = MESSAGING_APPLICATION_ID
         body.to = [PHONE_NUMBER_INBOUND]
         body.mfrom = PHONE_NUMBER_OUTBOUND
         body.text = "Python Monitoring"
@@ -150,9 +154,20 @@
             scope = "scope",
             code = "123456",
             expiration_time_in_minutes = 3
         )
         response = self.auth_client.create_verify_two_factor(ACCOUNT_ID, body)
         self.assertTrue(isinstance(response.body.valid, bool))
 
+    def test_tn_lookup(self):
+        body = OrderRequest()
+        body.tns = [PHONE_NUMBER_OUTBOUND]
+        response = self.tn_lookup_client.create_lookup_request(ACCOUNT_ID, body)
+        self.assertTrue(response.status_code == 202)
+
+        # test get method with the returned request_id
+        request_id = response.body.request_id
+        get_response = self.tn_lookup_client.get_lookup_request_status(ACCOUNT_ID, request_id)
+        self.assertTrue(get_response.status_code == 200)
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `bandwidth-sdk-9.1.0/tests/integration/bxml_tests.py` & `bandwidth-sdk-9.2.0/tests/integration/bxml_tests.py`

 * *Files identical despite different names*

### Comparing `bandwidth-sdk-9.1.0/tests/test_helper.py` & `bandwidth-sdk-9.2.0/tests/test_helper.py`

 * *Files identical despite different names*

