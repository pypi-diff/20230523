# Comparing `tmp/swibots-1.2.0.tar.gz` & `tmp/swibots-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swibots-1.2.0.tar", last modified: Tue May 23 03:39:53 2023, max compression
+gzip compressed data, was "swibots-1.2.1.tar", last modified: Tue May 23 05:58:25 2023, max compression
```

## Comparing `swibots-1.2.0.tar` & `swibots-1.2.1.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:53.382433 swibots-1.2.0/
--rw-r--r--   0 root         (0) root         (0)     1817 2023-05-23 03:39:53.381596 swibots-1.2.0/PKG-INFO
--r---w----   0 root         (0) root         (0)     1538 2023-01-19 02:17:00.000000 swibots-1.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 03:39:53.382882 swibots-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      731 2023-05-23 03:39:47.000000 swibots-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.077372 swibots-1.2.0/swibots/
--rw-r--r--   0 root         (0) root         (0)      236 2023-01-16 12:19:14.000000 swibots-1.2.0/swibots/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.125857 swibots-1.2.0/swibots/api/
--rw-r--r--   0 root         (0) root         (0)      140 2023-01-16 06:31:11.000000 swibots-1.2.0/swibots/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2236 2023-01-21 06:26:21.000000 swibots-1.2.0/swibots/api/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.135942 swibots-1.2.0/swibots/api/auth/
--rw-r--r--   0 root         (0) root         (0)       85 2023-01-16 07:03:12.000000 swibots-1.2.0/swibots/api/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1220 2023-01-23 17:55:04.000000 swibots-1.2.0/swibots/api/auth/auth_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.147394 swibots-1.2.0/swibots/api/auth/controllers/
--rw-r--r--   0 root         (0) root         (0)       73 2023-01-09 05:33:14.000000 swibots-1.2.0/swibots/api/auth/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1514 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/auth/controllers/user_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.164875 swibots-1.2.0/swibots/api/auth/methods/
--rwxr-xr-x   0 root         (0) root         (0)       94 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/auth/methods/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      650 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/auth/methods/get_me.py
--rw-r--r--   0 root         (0) root         (0)      837 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/auth/methods/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.181886 swibots-1.2.0/swibots/api/auth/models/
--rw-r--r--   0 root         (0) root         (0)       56 2023-01-13 05:35:17.000000 swibots-1.2.0/swibots/api/auth/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4642 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/api/auth/models/auth_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.195972 swibots-1.2.0/swibots/api/bot/
--rwxr-xr-x   0 root         (0) root         (0)       83 2023-01-16 06:01:42.000000 swibots-1.2.0/swibots/api/bot/__init__.py
--r---w----   0 root         (0) root         (0)     1141 2023-01-23 17:54:24.000000 swibots-1.2.0/swibots/api/bot/bot_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.205715 swibots-1.2.0/swibots/api/bot/controllers/
--r---w----   0 root         (0) root         (0)       71 2023-01-15 12:54:24.000000 swibots-1.2.0/swibots/api/bot/controllers/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1790 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/bot/controllers/bot_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.239243 swibots-1.2.0/swibots/api/bot/methods/
--rwxr-xr-x   0 root         (0) root         (0)      209 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/bot/methods/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      540 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/bot/methods/delete_bot_info.py
--rwxr-xr-x   0 root         (0) root         (0)      582 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/bot/methods/get_bot_info.py
--rwxr-xr-x   0 root         (0) root         (0)      615 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/bot/methods/update_bot_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.262712 swibots-1.2.0/swibots/api/bot/models/
--rwxr-xr-x   0 root         (0) root         (0)      116 2023-01-15 13:00:36.000000 swibots-1.2.0/swibots/api/bot/models/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      955 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/api/bot/models/bot_command_info.py
--rwxr-xr-x   0 root         (0) root         (0)     1585 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/api/bot/models/bot_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.279439 swibots-1.2.0/swibots/api/chat/
--rw-r--r--   0 root         (0) root         (0)      107 2023-01-16 06:01:20.000000 swibots-1.2.0/swibots/api/chat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5372 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/chat_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.296010 swibots-1.2.0/swibots/api/chat/controllers/
--rw-r--r--   0 root         (0) root         (0)       83 2023-01-15 12:53:45.000000 swibots-1.2.0/swibots/api/chat/controllers/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    21518 2023-02-08 08:21:26.000000 swibots-1.2.0/swibots/api/chat/controllers/message_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.338514 swibots-1.2.0/swibots/api/chat/events/
--rwxr-xr-x   0 root         (0) root         (0)      326 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/events/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     2073 2023-02-06 20:56:35.000000 swibots-1.2.0/swibots/api/chat/events/callback_query_event.py
--rwxr-xr-x   0 root         (0) root         (0)     2731 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/events/chat_event.py
--rwxr-xr-x   0 root         (0) root         (0)     2095 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/events/command_event.py
--rwxr-xr-x   0 root         (0) root         (0)     2103 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/events/inline_query_event.py
--rwxr-xr-x   0 root         (0) root         (0)     2434 2023-02-06 21:23:12.000000 swibots-1.2.0/swibots/api/chat/events/message_event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.505224 swibots-1.2.0/swibots/api/chat/methods/
--rwxr-xr-x   0 root         (0) root         (0)     1709 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/methods/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      654 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/methods/answer_inline_query.py
--rwxr-xr-x   0 root         (0) root         (0)      693 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/api/chat/methods/clear_conversation.py
--rwxr-xr-x   0 root         (0) root         (0)      705 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/chat/methods/delete_message.py
--rwxr-xr-x   0 root         (0) root         (0)      707 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/chat/methods/delete_messages_from_user.py
--rwxr-xr-x   0 root         (0) root         (0)     1358 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/methods/download_media.py
--rwxr-xr-x   0 root         (0) root         (0)      750 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/methods/edit_message.py
--rwxr-xr-x   0 root         (0) root         (0)      853 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/methods/edit_message_text.py
--rwxr-xr-x   0 root         (0) root         (0)      693 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/chat/methods/flag_message.py
--rwxr-xr-x   0 root         (0) root         (0)     1192 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/methods/forward_message.py
--rwxr-xr-x   0 root         (0) root         (0)     1139 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/chat/methods/get_channel_chat_history.py
--rwxr-xr-x   0 root         (0) root         (0)      725 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/api/chat/methods/get_community_media_files.py
--rwxr-xr-x   0 root         (0) root         (0)      883 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/chat/methods/get_community_media_files_by_status.py
--rwxr-xr-x   0 root         (0) root         (0)      636 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/api/chat/methods/get_flag_messages.py
--rwxr-xr-x   0 root         (0) root         (0)     1090 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/chat/methods/get_group_chat_history.py
--rwxr-xr-x   0 root         (0) root         (0)      649 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/chat/methods/get_message.py
--rwxr-xr-x   0 root         (0) root         (0)      707 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/chat/methods/get_messages.py
--rwxr-xr-x   0 root         (0) root         (0)     1102 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/chat/methods/get_messages_between_users.py
--rwxr-xr-x   0 root         (0) root         (0)      560 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/methods/get_unread_messages_count.py
--rwxr-xr-x   0 root         (0) root         (0)      785 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/chat/methods/get_user_media_files.py
--rwxr-xr-x   0 root         (0) root         (0)      881 2023-02-08 08:22:32.000000 swibots-1.2.0/swibots/api/chat/methods/reply_message.py
--rwxr-xr-x   0 root         (0) root         (0)     1032 2023-02-08 08:20:23.000000 swibots-1.2.0/swibots/api/chat/methods/reply_message_text.py
--rwxr-xr-x   0 root         (0) root         (0)      849 2023-02-08 08:19:39.000000 swibots-1.2.0/swibots/api/chat/methods/send_message.py
--rwxr-xr-x   0 root         (0) root         (0)     1136 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/methods/send_text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.548102 swibots-1.2.0/swibots/api/chat/models/
--rw-r--r--   0 root         (0) root         (0)      305 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/models/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      920 2023-02-06 20:55:52.000000 swibots-1.2.0/swibots/api/chat/models/group_chat_history.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.616204 swibots-1.2.0/swibots/api/chat/models/inline/
--rwxr-xr-x   0 root         (0) root         (0)      565 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/models/inline/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1371 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/models/inline/base_typed_inline_query_result.py
--rwxr-xr-x   0 root         (0) root         (0)     2533 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/models/inline/inline_query.py
--rwxr-xr-x   0 root         (0) root         (0)     1871 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/models/inline/inline_query_answer.py
--rwxr-xr-x   0 root         (0) root         (0)      991 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/models/inline/inline_query_result.py
--rwxr-xr-x   0 root         (0) root         (0)     1158 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/models/inline/inline_query_result_article.py
--rw-r--r--   0 root         (0) root         (0)     1273 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/models/inline/inline_query_result_document.py
--rw-r--r--   0 root         (0) root         (0)     1620 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/models/inline/inline_query_result_photo.py
--rw-r--r--   0 root         (0) root         (0)     1760 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/models/inline/inline_query_result_video.py
--rwxr-xr-x   0 root         (0) root         (0)      581 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/models/inline/input_message_content.py
--rwxr-xr-x   0 root         (0) root         (0)      201 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/models/inline/types.py
--rwxr-xr-x   0 root         (0) root         (0)      886 2023-02-08 07:21:24.000000 swibots-1.2.0/swibots/api/chat/models/inline_keyboard_button.py
--rwxr-xr-x   0 root         (0) root         (0)      170 2023-01-18 20:49:52.000000 swibots-1.2.0/swibots/api/chat/models/inline_keyboard_color.py
--rwxr-xr-x   0 root         (0) root         (0)      146 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/chat/models/inline_keyboard_size.py
--rwxr-xr-x   0 root         (0) root         (0)     2065 2023-02-08 07:22:42.000000 swibots-1.2.0/swibots/api/chat/models/inline_markup.py
--rw-r--r--   0 root         (0) root         (0)    10769 2023-02-08 09:10:55.000000 swibots-1.2.0/swibots/api/chat/models/message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.623780 swibots-1.2.0/swibots/api/common/
--rwxr-xr-x   0 root         (0) root         (0)       44 2023-01-16 06:01:00.000000 swibots-1.2.0/swibots/api/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.634432 swibots-1.2.0/swibots/api/common/events/
--rwxr-xr-x   0 root         (0) root         (0)       46 2023-01-13 06:20:04.000000 swibots-1.2.0/swibots/api/common/events/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     2789 2023-01-23 19:39:48.000000 swibots-1.2.0/swibots/api/common/events/event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.656408 swibots-1.2.0/swibots/api/common/models/
--rwxr-xr-x   0 root         (0) root         (0)      101 2023-02-06 20:55:52.000000 swibots-1.2.0/swibots/api/common/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-02-07 07:11:30.000000 swibots-1.2.0/swibots/api/common/models/media.py
--rwxr-xr-x   0 root         (0) root         (0)     1565 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/common/models/media_upload_request.py
--rwxr-xr-x   0 root         (0) root         (0)     1706 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/common/models/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.667875 swibots-1.2.0/swibots/api/community/
--rwxr-xr-x   0 root         (0) root         (0)       90 2023-01-16 06:00:40.000000 swibots-1.2.0/swibots/api/community/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5059 2023-03-20 17:15:06.000000 swibots-1.2.0/swibots/api/community/community_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.692242 swibots-1.2.0/swibots/api/community/controllers/
--rw-r--r--   0 root         (0) root         (0)      102 2023-02-06 20:55:52.000000 swibots-1.2.0/swibots/api/community/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      595 2023-02-06 20:55:52.000000 swibots-1.2.0/swibots/api/community/controllers/channel_controller.py
--rwxr-xr-x   0 root         (0) root         (0)      616 2023-02-06 20:55:52.000000 swibots-1.2.0/swibots/api/community/controllers/community_controller.py
--rw-r--r--   0 root         (0) root         (0)      576 2023-02-06 20:55:52.000000 swibots-1.2.0/swibots/api/community/controllers/group_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.816542 swibots-1.2.0/swibots/api/community/events/
--rwxr-xr-x   0 root         (0) root         (0)      566 2023-01-16 23:20:36.000000 swibots-1.2.0/swibots/api/community/events/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1387 2023-03-20 17:12:26.000000 swibots-1.2.0/swibots/api/community/events/channel_created_event.py
--rwxr-xr-x   0 root         (0) root         (0)     1387 2023-03-20 17:12:56.000000 swibots-1.2.0/swibots/api/community/events/channel_deleted_event.py
--rwxr-xr-x   0 root         (0) root         (0)     1387 2023-03-20 17:12:44.000000 swibots-1.2.0/swibots/api/community/events/channel_updated_event.py
--rwxr-xr-x   0 root         (0) root         (0)     2303 2023-01-23 19:25:02.000000 swibots-1.2.0/swibots/api/community/events/community_event.py
--rwxr-xr-x   0 root         (0) root         (0)     1383 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/community/events/community_updated_event.py
--rwxr-xr-x   0 root         (0) root         (0)     1381 2023-03-20 17:13:37.000000 swibots-1.2.0/swibots/api/community/events/group_created_event.py
--rwxr-xr-x   0 root         (0) root         (0)     1381 2023-03-20 17:14:02.000000 swibots-1.2.0/swibots/api/community/events/group_deleted_event.py
--rwxr-xr-x   0 root         (0) root         (0)     1381 2023-03-20 17:13:49.000000 swibots-1.2.0/swibots/api/community/events/group_updated_event.py
--rwxr-xr-x   0 root         (0) root         (0)     1380 2023-03-20 17:14:48.000000 swibots-1.2.0/swibots/api/community/events/member_joined_event.py
--rwxr-xr-x   0 root         (0) root         (0)     1377 2023-03-20 17:15:06.000000 swibots-1.2.0/swibots/api/community/events/member_left_event.py
--rwxr-xr-x   0 root         (0) root         (0)     1373 2023-03-20 17:14:14.000000 swibots-1.2.0/swibots/api/community/events/user_banned_event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.866744 swibots-1.2.0/swibots/api/community/methods/
--rwxr-xr-x   0 root         (0) root         (0)      194 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/community/methods/__init__.py
--rw-r--r--   0 root         (0) root         (0)      643 2023-02-06 20:55:52.000000 swibots-1.2.0/swibots/api/community/methods/get_channel.py
--rwxr-xr-x   0 root         (0) root         (0)      668 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/community/methods/get_community.py
--rw-r--r--   0 root         (0) root         (0)      619 2023-02-06 20:55:52.000000 swibots-1.2.0/swibots/api/community/methods/get_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.914798 swibots-1.2.0/swibots/api/community/models/
--rwxr-xr-x   0 root         (0) root         (0)      132 2023-01-13 05:39:45.000000 swibots-1.2.0/swibots/api/community/models/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     2743 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/community/models/channel.py
--rwxr-xr-x   0 root         (0) root         (0)     2954 2023-01-21 07:06:56.000000 swibots-1.2.0/swibots/api/community/models/community.py
--rwxr-xr-x   0 root         (0) root         (0)     2720 2023-01-21 07:07:04.000000 swibots-1.2.0/swibots/api/community/models/group.py
--rwxr-xr-x   0 root         (0) root         (0)     9347 2023-04-17 03:16:12.000000 swibots-1.2.0/swibots/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.980568 swibots-1.2.0/swibots/base/
--rw-r--r--   0 root         (0) root         (0)      262 2023-01-16 05:59:47.000000 swibots-1.2.0/swibots/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)       69 2023-01-09 05:33:14.000000 swibots-1.2.0/swibots/base/rest_controller.py
--rw-r--r--   0 root         (0) root         (0)      370 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/base/rest_request.py
--rw-r--r--   0 root         (0) root         (0)      644 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/base/rest_response.py
--rw-r--r--   0 root         (0) root         (0)     4261 2023-02-06 20:55:52.000000 swibots-1.2.0/swibots/base/switch_client.py
--rw-r--r--   0 root         (0) root         (0)     1180 2023-01-21 06:58:45.000000 swibots-1.2.0/swibots/base/switch_object.py
--rwxr-xr-x   0 root         (0) root         (0)      543 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/base/switch_ws_async_client.py
--rwxr-xr-x   0 root         (0) root         (0)     4329 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/bot_app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:53.018929 swibots-1.2.0/swibots/bots/
--rwxr-xr-x   0 root         (0) root         (0)      201 2023-01-17 03:43:24.000000 swibots-1.2.0/swibots/bots/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4646 2023-04-20 23:47:00.000000 swibots-1.2.0/swibots/bots/bot.py
--rwxr-xr-x   0 root         (0) root         (0)     1646 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/bots/bot_context.py
--rwxr-xr-x   0 root         (0) root         (0)      109 2023-01-14 17:55:20.000000 swibots-1.2.0/swibots/bots/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:53.136066 swibots-1.2.0/swibots/bots/decorators/
--rwxr-xr-x   0 root         (0) root         (0)      999 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/bots/decorators/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      540 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/bots/decorators/on_callback_query.py
--rwxr-xr-x   0 root         (0) root         (0)      510 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/bots/decorators/on_channel_created.py
--rwxr-xr-x   0 root         (0) root         (0)      544 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/bots/decorators/on_channel_deleted.py
--rwxr-xr-x   0 root         (0) root         (0)      541 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/bots/decorators/on_channel_updated.py
--rwxr-xr-x   0 root         (0) root         (0)      574 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/bots/decorators/on_command.py
--rwxr-xr-x   0 root         (0) root         (0)      544 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/bots/decorators/on_community_updated.py
--rwxr-xr-x   0 root         (0) root         (0)      536 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/bots/decorators/on_group_created.py
--rwxr-xr-x   0 root         (0) root         (0)      536 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/bots/decorators/on_group_deleted.py
--rwxr-xr-x   0 root         (0) root         (0)      534 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/bots/decorators/on_group_updated.py
--rw-r--r--   0 root         (0) root         (0)      537 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/bots/decorators/on_inline_query.py
--rwxr-xr-x   0 root         (0) root         (0)      534 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/bots/decorators/on_member_joined.py
--rwxr-xr-x   0 root         (0) root         (0)      529 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/bots/decorators/on_member_left.py
--rwxr-xr-x   0 root         (0) root         (0)      503 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/bots/decorators/on_message.py
--rwxr-xr-x   0 root         (0) root         (0)      543 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/bots/decorators/on_unknown_command.py
--rwxr-xr-x   0 root         (0) root         (0)      509 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/bots/decorators/on_user_banned.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:53.146654 swibots-1.2.0/swibots/bots/filters/
--rwxr-xr-x   0 root         (0) root         (0)       22 2023-01-16 03:25:36.000000 swibots-1.2.0/swibots/bots/filters/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     7785 2023-04-21 00:39:37.000000 swibots-1.2.0/swibots/bots/filters/filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:53.284005 swibots-1.2.0/swibots/bots/handlers/
--rwxr-xr-x   0 root         (0) root         (0)     1300 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/bots/handlers/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1048 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/bots/handlers/base_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      985 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/bots/handlers/callback_query_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      681 2023-03-20 17:12:26.000000 swibots-1.2.0/swibots/bots/handlers/channel_created_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      688 2023-03-20 17:12:57.000000 swibots-1.2.0/swibots/bots/handlers/channel_deleted_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      734 2023-03-20 17:12:44.000000 swibots-1.2.0/swibots/bots/handlers/channel_updated_handler.py
--rwxr-xr-x   0 root         (0) root         (0)     1514 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/bots/handlers/command_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      686 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/bots/handlers/community_updated_handler.py
--rwxr-xr-x   0 root         (0) root         (0)     1325 2023-04-21 00:21:17.000000 swibots-1.2.0/swibots/bots/handlers/event_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      680 2023-03-20 17:13:37.000000 swibots-1.2.0/swibots/bots/handlers/group_created_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      775 2023-03-20 17:14:02.000000 swibots-1.2.0/swibots/bots/handlers/group_deleted_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      775 2023-03-20 17:13:49.000000 swibots-1.2.0/swibots/bots/handlers/group_updated_handler.py
--rw-r--r--   0 root         (0) root         (0)      867 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/bots/handlers/inline_query_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      679 2023-03-20 17:14:48.000000 swibots-1.2.0/swibots/bots/handlers/member_joined_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      674 2023-03-20 17:15:07.000000 swibots-1.2.0/swibots/bots/handlers/member_left_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      960 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/bots/handlers/message_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      885 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/bots/handlers/unknown_command_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      670 2023-03-20 17:14:14.000000 swibots-1.2.0/swibots/bots/handlers/user_banned_handler.py
--rwxr-xr-x   0 root         (0) root         (0)      285 2023-01-23 21:16:29.000000 swibots-1.2.0/swibots/bots/register_command.py
--rwxr-xr-x   0 root         (0) root         (0)     1621 2023-05-23 03:35:50.000000 swibots-1.2.0/swibots/config.py
--rw-r--r--   0 root         (0) root         (0)     1333 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/error.py
--rwxr-xr-x   0 root         (0) root         (0)      854 2023-03-20 17:15:29.000000 swibots-1.2.0/swibots/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:53.303750 swibots-1.2.0/swibots/utils/
--rw-r--r--   0 root         (0) root         (0)       75 2023-01-16 05:53:47.000000 swibots-1.2.0/swibots/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5880 2023-04-20 23:47:11.000000 swibots-1.2.0/swibots/utils/rest_client.py
--rw-r--r--   0 root         (0) root         (0)     2475 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/utils/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:53.311462 swibots-1.2.0/swibots/utils/ws/
--rw-r--r--   0 root         (0) root         (0)       48 2023-01-19 05:23:27.000000 swibots-1.2.0/swibots/utils/ws/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:53.335318 swibots-1.2.0/swibots/utils/ws/asyncstomp/
--rw-r--r--   0 root         (0) root         (0)      150 2023-01-09 05:33:14.000000 swibots-1.2.0/swibots/utils/ws/asyncstomp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9743 2023-01-21 06:34:39.000000 swibots-1.2.0/swibots/utils/ws/asyncstomp/async_ws_client.py
--rw-r--r--   0 root         (0) root         (0)      980 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/utils/ws/asyncstomp/async_ws_subscription.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:53.356755 swibots-1.2.0/swibots/utils/ws/common/
--rw-r--r--   0 root         (0) root         (0)      100 2023-01-09 05:33:14.000000 swibots-1.2.0/swibots/utils/ws/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1654 2023-01-09 05:33:14.000000 swibots-1.2.0/swibots/utils/ws/common/ws_frame.py
--rw-r--r--   0 root         (0) root         (0)      430 2023-01-09 05:33:14.000000 swibots-1.2.0/swibots/utils/ws/common/ws_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.112336 swibots-1.2.0/swibots.egg-info/
--rwxr-xr-x   0 root         (0) root         (0)     1817 2023-05-23 03:39:51.000000 swibots-1.2.0/swibots.egg-info/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     7316 2023-05-23 03:39:51.000000 swibots-1.2.0/swibots.egg-info/SOURCES.txt
--rwxr-xr-x   0 root         (0) root         (0)        1 2023-05-23 03:39:51.000000 swibots-1.2.0/swibots.egg-info/dependency_links.txt
--rwxr-xr-x   0 root         (0) root         (0)       31 2023-05-23 03:39:51.000000 swibots-1.2.0/swibots.egg-info/requires.txt
--rwxr-xr-x   0 root         (0) root         (0)       14 2023-05-23 03:39:51.000000 swibots-1.2.0/swibots.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:53.374575 swibots-1.2.0/tests/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 05:56:05.000000 swibots-1.2.0/tests/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      202 2023-01-15 22:26:25.000000 swibots-1.2.0/tests/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:25.440133 swibots-1.2.1/
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-05-23 05:58:25.438416 swibots-1.2.1/PKG-INFO
+-r---w----   0 root         (0) root         (0)     1538 2023-01-19 02:17:00.000000 swibots-1.2.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 05:58:25.441247 swibots-1.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      731 2023-05-23 05:58:15.000000 swibots-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:23.992872 swibots-1.2.1/swibots/
+-rw-r--r--   0 root         (0) root         (0)      236 2023-01-16 12:19:14.000000 swibots-1.2.1/swibots/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:24.045307 swibots-1.2.1/swibots/api/
+-rw-r--r--   0 root         (0) root         (0)      140 2023-01-16 06:31:11.000000 swibots-1.2.1/swibots/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2023-01-21 06:26:21.000000 swibots-1.2.1/swibots/api/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:24.058745 swibots-1.2.1/swibots/api/auth/
+-rw-r--r--   0 root         (0) root         (0)       85 2023-01-16 07:03:12.000000 swibots-1.2.1/swibots/api/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-01-23 17:55:04.000000 swibots-1.2.1/swibots/api/auth/auth_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:24.069199 swibots-1.2.1/swibots/api/auth/controllers/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-01-09 05:33:14.000000 swibots-1.2.1/swibots/api/auth/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1514 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/auth/controllers/user_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:24.085964 swibots-1.2.1/swibots/api/auth/methods/
+-rwxr-xr-x   0 root         (0) root         (0)       94 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/auth/methods/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      650 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/auth/methods/get_me.py
+-rw-r--r--   0 root         (0) root         (0)      837 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/auth/methods/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:24.099670 swibots-1.2.1/swibots/api/auth/models/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-01-13 05:35:17.000000 swibots-1.2.1/swibots/api/auth/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4642 2023-01-19 01:21:52.000000 swibots-1.2.1/swibots/api/auth/models/auth_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:24.113718 swibots-1.2.1/swibots/api/bot/
+-rwxr-xr-x   0 root         (0) root         (0)       83 2023-01-16 06:01:42.000000 swibots-1.2.1/swibots/api/bot/__init__.py
+-r---w----   0 root         (0) root         (0)     1141 2023-01-23 17:54:24.000000 swibots-1.2.1/swibots/api/bot/bot_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:24.150836 swibots-1.2.1/swibots/api/bot/controllers/
+-r---w----   0 root         (0) root         (0)       71 2023-01-15 12:54:24.000000 swibots-1.2.1/swibots/api/bot/controllers/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1790 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/api/bot/controllers/bot_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:24.190801 swibots-1.2.1/swibots/api/bot/methods/
+-rwxr-xr-x   0 root         (0) root         (0)      209 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/api/bot/methods/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      540 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/api/bot/methods/delete_bot_info.py
+-rwxr-xr-x   0 root         (0) root         (0)      582 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/api/bot/methods/get_bot_info.py
+-rwxr-xr-x   0 root         (0) root         (0)      615 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/api/bot/methods/update_bot_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:24.226847 swibots-1.2.1/swibots/api/bot/models/
+-rwxr-xr-x   0 root         (0) root         (0)      116 2023-01-15 13:00:36.000000 swibots-1.2.1/swibots/api/bot/models/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      955 2023-01-19 01:21:52.000000 swibots-1.2.1/swibots/api/bot/models/bot_command_info.py
+-rwxr-xr-x   0 root         (0) root         (0)     1585 2023-01-19 01:21:52.000000 swibots-1.2.1/swibots/api/bot/models/bot_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:24.245009 swibots-1.2.1/swibots/api/chat/
+-rw-r--r--   0 root         (0) root         (0)      107 2023-01-16 06:01:20.000000 swibots-1.2.1/swibots/api/chat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5372 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/chat_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:24.260480 swibots-1.2.1/swibots/api/chat/controllers/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-01-15 12:53:45.000000 swibots-1.2.1/swibots/api/chat/controllers/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    21518 2023-02-08 08:21:26.000000 swibots-1.2.1/swibots/api/chat/controllers/message_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:24.318466 swibots-1.2.1/swibots/api/chat/events/
+-rwxr-xr-x   0 root         (0) root         (0)      326 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/events/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2073 2023-02-06 20:56:35.000000 swibots-1.2.1/swibots/api/chat/events/callback_query_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     2731 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/events/chat_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     2095 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/events/command_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     2103 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/events/inline_query_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     2434 2023-02-06 21:23:12.000000 swibots-1.2.1/swibots/api/chat/events/message_event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:24.584903 swibots-1.2.1/swibots/api/chat/methods/
+-rwxr-xr-x   0 root         (0) root         (0)     1709 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/methods/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      654 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/methods/answer_inline_query.py
+-rwxr-xr-x   0 root         (0) root         (0)      693 2023-01-19 01:21:52.000000 swibots-1.2.1/swibots/api/chat/methods/clear_conversation.py
+-rwxr-xr-x   0 root         (0) root         (0)      705 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/api/chat/methods/delete_message.py
+-rwxr-xr-x   0 root         (0) root         (0)      707 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/api/chat/methods/delete_messages_from_user.py
+-rwxr-xr-x   0 root         (0) root         (0)     1358 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/methods/download_media.py
+-rwxr-xr-x   0 root         (0) root         (0)      750 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/methods/edit_message.py
+-rwxr-xr-x   0 root         (0) root         (0)      853 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/methods/edit_message_text.py
+-rwxr-xr-x   0 root         (0) root         (0)      693 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/api/chat/methods/flag_message.py
+-rwxr-xr-x   0 root         (0) root         (0)     1192 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/methods/forward_message.py
+-rwxr-xr-x   0 root         (0) root         (0)     1139 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/api/chat/methods/get_channel_chat_history.py
+-rwxr-xr-x   0 root         (0) root         (0)      725 2023-01-19 01:21:52.000000 swibots-1.2.1/swibots/api/chat/methods/get_community_media_files.py
+-rwxr-xr-x   0 root         (0) root         (0)      883 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/api/chat/methods/get_community_media_files_by_status.py
+-rwxr-xr-x   0 root         (0) root         (0)      636 2023-01-19 01:21:52.000000 swibots-1.2.1/swibots/api/chat/methods/get_flag_messages.py
+-rwxr-xr-x   0 root         (0) root         (0)     1090 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/api/chat/methods/get_group_chat_history.py
+-rwxr-xr-x   0 root         (0) root         (0)      649 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/api/chat/methods/get_message.py
+-rwxr-xr-x   0 root         (0) root         (0)      707 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/api/chat/methods/get_messages.py
+-rwxr-xr-x   0 root         (0) root         (0)     1102 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/api/chat/methods/get_messages_between_users.py
+-rwxr-xr-x   0 root         (0) root         (0)      560 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/methods/get_unread_messages_count.py
+-rwxr-xr-x   0 root         (0) root         (0)      785 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/api/chat/methods/get_user_media_files.py
+-rwxr-xr-x   0 root         (0) root         (0)      881 2023-02-08 08:22:32.000000 swibots-1.2.1/swibots/api/chat/methods/reply_message.py
+-rwxr-xr-x   0 root         (0) root         (0)     1032 2023-02-08 08:20:23.000000 swibots-1.2.1/swibots/api/chat/methods/reply_message_text.py
+-rwxr-xr-x   0 root         (0) root         (0)      849 2023-02-08 08:19:39.000000 swibots-1.2.1/swibots/api/chat/methods/send_message.py
+-rwxr-xr-x   0 root         (0) root         (0)     1136 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/methods/send_text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:24.657308 swibots-1.2.1/swibots/api/chat/models/
+-rw-r--r--   0 root         (0) root         (0)      305 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/models/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      920 2023-02-06 20:55:52.000000 swibots-1.2.1/swibots/api/chat/models/group_chat_history.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:24.738144 swibots-1.2.1/swibots/api/chat/models/inline/
+-rwxr-xr-x   0 root         (0) root         (0)      565 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/models/inline/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1371 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/models/inline/base_typed_inline_query_result.py
+-rwxr-xr-x   0 root         (0) root         (0)     2533 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/models/inline/inline_query.py
+-rwxr-xr-x   0 root         (0) root         (0)     1871 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/models/inline/inline_query_answer.py
+-rwxr-xr-x   0 root         (0) root         (0)      991 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/models/inline/inline_query_result.py
+-rwxr-xr-x   0 root         (0) root         (0)     1158 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/models/inline/inline_query_result_article.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/models/inline/inline_query_result_document.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/models/inline/inline_query_result_photo.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/models/inline/inline_query_result_video.py
+-rwxr-xr-x   0 root         (0) root         (0)      581 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/models/inline/input_message_content.py
+-rwxr-xr-x   0 root         (0) root         (0)      201 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/chat/models/inline/types.py
+-rwxr-xr-x   0 root         (0) root         (0)      886 2023-02-08 07:21:24.000000 swibots-1.2.1/swibots/api/chat/models/inline_keyboard_button.py
+-rwxr-xr-x   0 root         (0) root         (0)      170 2023-01-18 20:49:52.000000 swibots-1.2.1/swibots/api/chat/models/inline_keyboard_color.py
+-rwxr-xr-x   0 root         (0) root         (0)      146 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/api/chat/models/inline_keyboard_size.py
+-rwxr-xr-x   0 root         (0) root         (0)     2065 2023-02-08 07:22:42.000000 swibots-1.2.1/swibots/api/chat/models/inline_markup.py
+-rw-r--r--   0 root         (0) root         (0)    10769 2023-02-08 09:10:55.000000 swibots-1.2.1/swibots/api/chat/models/message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:24.745482 swibots-1.2.1/swibots/api/common/
+-rwxr-xr-x   0 root         (0) root         (0)       44 2023-01-16 06:01:00.000000 swibots-1.2.1/swibots/api/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:24.761128 swibots-1.2.1/swibots/api/common/events/
+-rwxr-xr-x   0 root         (0) root         (0)       46 2023-01-13 06:20:04.000000 swibots-1.2.1/swibots/api/common/events/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2789 2023-01-23 19:39:48.000000 swibots-1.2.1/swibots/api/common/events/event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:24.787386 swibots-1.2.1/swibots/api/common/models/
+-rwxr-xr-x   0 root         (0) root         (0)      101 2023-02-06 20:55:52.000000 swibots-1.2.1/swibots/api/common/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-02-07 07:11:30.000000 swibots-1.2.1/swibots/api/common/models/media.py
+-rwxr-xr-x   0 root         (0) root         (0)     1565 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/common/models/media_upload_request.py
+-rwxr-xr-x   0 root         (0) root         (0)     1706 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/common/models/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:24.801725 swibots-1.2.1/swibots/api/community/
+-rwxr-xr-x   0 root         (0) root         (0)       90 2023-01-16 06:00:40.000000 swibots-1.2.1/swibots/api/community/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5059 2023-03-20 17:15:06.000000 swibots-1.2.1/swibots/api/community/community_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:24.825581 swibots-1.2.1/swibots/api/community/controllers/
+-rw-r--r--   0 root         (0) root         (0)      102 2023-02-06 20:55:52.000000 swibots-1.2.1/swibots/api/community/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      595 2023-02-06 20:55:52.000000 swibots-1.2.1/swibots/api/community/controllers/channel_controller.py
+-rwxr-xr-x   0 root         (0) root         (0)      616 2023-02-06 20:55:52.000000 swibots-1.2.1/swibots/api/community/controllers/community_controller.py
+-rw-r--r--   0 root         (0) root         (0)      576 2023-02-06 20:55:52.000000 swibots-1.2.1/swibots/api/community/controllers/group_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:24.924679 swibots-1.2.1/swibots/api/community/events/
+-rwxr-xr-x   0 root         (0) root         (0)      566 2023-01-16 23:20:36.000000 swibots-1.2.1/swibots/api/community/events/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1387 2023-03-20 17:12:26.000000 swibots-1.2.1/swibots/api/community/events/channel_created_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1387 2023-03-20 17:12:56.000000 swibots-1.2.1/swibots/api/community/events/channel_deleted_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1387 2023-03-20 17:12:44.000000 swibots-1.2.1/swibots/api/community/events/channel_updated_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     2303 2023-01-23 19:25:02.000000 swibots-1.2.1/swibots/api/community/events/community_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1383 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/api/community/events/community_updated_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1381 2023-03-20 17:13:37.000000 swibots-1.2.1/swibots/api/community/events/group_created_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1381 2023-03-20 17:14:02.000000 swibots-1.2.1/swibots/api/community/events/group_deleted_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1381 2023-03-20 17:13:49.000000 swibots-1.2.1/swibots/api/community/events/group_updated_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1380 2023-03-20 17:14:48.000000 swibots-1.2.1/swibots/api/community/events/member_joined_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1377 2023-03-20 17:15:06.000000 swibots-1.2.1/swibots/api/community/events/member_left_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1373 2023-03-20 17:14:14.000000 swibots-1.2.1/swibots/api/community/events/user_banned_event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:24.952354 swibots-1.2.1/swibots/api/community/methods/
+-rwxr-xr-x   0 root         (0) root         (0)      194 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/community/methods/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      643 2023-02-06 20:55:52.000000 swibots-1.2.1/swibots/api/community/methods/get_channel.py
+-rwxr-xr-x   0 root         (0) root         (0)      668 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/api/community/methods/get_community.py
+-rw-r--r--   0 root         (0) root         (0)      619 2023-02-06 20:55:52.000000 swibots-1.2.1/swibots/api/community/methods/get_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:24.975063 swibots-1.2.1/swibots/api/community/models/
+-rwxr-xr-x   0 root         (0) root         (0)      132 2023-01-13 05:39:45.000000 swibots-1.2.1/swibots/api/community/models/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2743 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/api/community/models/channel.py
+-rwxr-xr-x   0 root         (0) root         (0)     2954 2023-01-21 07:06:56.000000 swibots-1.2.1/swibots/api/community/models/community.py
+-rwxr-xr-x   0 root         (0) root         (0)     2720 2023-01-21 07:07:04.000000 swibots-1.2.1/swibots/api/community/models/group.py
+-rwxr-xr-x   0 root         (0) root         (0)     9347 2023-04-17 03:16:12.000000 swibots-1.2.1/swibots/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:25.019589 swibots-1.2.1/swibots/base/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-01-16 05:59:47.000000 swibots-1.2.1/swibots/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       69 2023-01-09 05:33:14.000000 swibots-1.2.1/swibots/base/rest_controller.py
+-rw-r--r--   0 root         (0) root         (0)      370 2023-01-19 01:21:52.000000 swibots-1.2.1/swibots/base/rest_request.py
+-rw-r--r--   0 root         (0) root         (0)      644 2023-01-19 01:21:52.000000 swibots-1.2.1/swibots/base/rest_response.py
+-rw-r--r--   0 root         (0) root         (0)     4261 2023-02-06 20:55:52.000000 swibots-1.2.1/swibots/base/switch_client.py
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-01-21 06:58:45.000000 swibots-1.2.1/swibots/base/switch_object.py
+-rwxr-xr-x   0 root         (0) root         (0)      543 2023-01-19 01:21:52.000000 swibots-1.2.1/swibots/base/switch_ws_async_client.py
+-rwxr-xr-x   0 root         (0) root         (0)     4598 2023-05-23 05:44:17.000000 swibots-1.2.1/swibots/bot_app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:25.059301 swibots-1.2.1/swibots/bots/
+-rwxr-xr-x   0 root         (0) root         (0)      201 2023-01-17 03:43:24.000000 swibots-1.2.1/swibots/bots/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4646 2023-04-20 23:47:00.000000 swibots-1.2.1/swibots/bots/bot.py
+-rwxr-xr-x   0 root         (0) root         (0)     1646 2023-01-19 01:21:52.000000 swibots-1.2.1/swibots/bots/bot_context.py
+-rwxr-xr-x   0 root         (0) root         (0)      109 2023-01-14 17:55:20.000000 swibots-1.2.1/swibots/bots/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:25.180377 swibots-1.2.1/swibots/bots/decorators/
+-rwxr-xr-x   0 root         (0) root         (0)      999 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/bots/decorators/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      540 2023-01-19 01:21:52.000000 swibots-1.2.1/swibots/bots/decorators/on_callback_query.py
+-rwxr-xr-x   0 root         (0) root         (0)      510 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/bots/decorators/on_channel_created.py
+-rwxr-xr-x   0 root         (0) root         (0)      544 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/bots/decorators/on_channel_deleted.py
+-rwxr-xr-x   0 root         (0) root         (0)      541 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/bots/decorators/on_channel_updated.py
+-rwxr-xr-x   0 root         (0) root         (0)      574 2023-01-19 01:21:52.000000 swibots-1.2.1/swibots/bots/decorators/on_command.py
+-rwxr-xr-x   0 root         (0) root         (0)      544 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/bots/decorators/on_community_updated.py
+-rwxr-xr-x   0 root         (0) root         (0)      536 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/bots/decorators/on_group_created.py
+-rwxr-xr-x   0 root         (0) root         (0)      536 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/bots/decorators/on_group_deleted.py
+-rwxr-xr-x   0 root         (0) root         (0)      534 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/bots/decorators/on_group_updated.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/bots/decorators/on_inline_query.py
+-rwxr-xr-x   0 root         (0) root         (0)      534 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/bots/decorators/on_member_joined.py
+-rwxr-xr-x   0 root         (0) root         (0)      529 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/bots/decorators/on_member_left.py
+-rwxr-xr-x   0 root         (0) root         (0)      503 2023-01-19 01:21:52.000000 swibots-1.2.1/swibots/bots/decorators/on_message.py
+-rwxr-xr-x   0 root         (0) root         (0)      543 2023-01-19 01:21:52.000000 swibots-1.2.1/swibots/bots/decorators/on_unknown_command.py
+-rwxr-xr-x   0 root         (0) root         (0)      509 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/bots/decorators/on_user_banned.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:25.197159 swibots-1.2.1/swibots/bots/filters/
+-rwxr-xr-x   0 root         (0) root         (0)       22 2023-01-16 03:25:36.000000 swibots-1.2.1/swibots/bots/filters/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7785 2023-04-21 00:39:37.000000 swibots-1.2.1/swibots/bots/filters/filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:25.308695 swibots-1.2.1/swibots/bots/handlers/
+-rwxr-xr-x   0 root         (0) root         (0)     1300 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/bots/handlers/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1048 2023-01-19 01:21:52.000000 swibots-1.2.1/swibots/bots/handlers/base_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      985 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/bots/handlers/callback_query_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      681 2023-03-20 17:12:26.000000 swibots-1.2.1/swibots/bots/handlers/channel_created_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      688 2023-03-20 17:12:57.000000 swibots-1.2.1/swibots/bots/handlers/channel_deleted_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      734 2023-03-20 17:12:44.000000 swibots-1.2.1/swibots/bots/handlers/channel_updated_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)     1514 2023-01-19 01:21:52.000000 swibots-1.2.1/swibots/bots/handlers/command_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      686 2023-01-19 01:21:52.000000 swibots-1.2.1/swibots/bots/handlers/community_updated_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)     1325 2023-04-21 00:21:17.000000 swibots-1.2.1/swibots/bots/handlers/event_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      680 2023-03-20 17:13:37.000000 swibots-1.2.1/swibots/bots/handlers/group_created_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      775 2023-03-20 17:14:02.000000 swibots-1.2.1/swibots/bots/handlers/group_deleted_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      775 2023-03-20 17:13:49.000000 swibots-1.2.1/swibots/bots/handlers/group_updated_handler.py
+-rw-r--r--   0 root         (0) root         (0)      867 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/bots/handlers/inline_query_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      679 2023-03-20 17:14:48.000000 swibots-1.2.1/swibots/bots/handlers/member_joined_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      674 2023-03-20 17:15:07.000000 swibots-1.2.1/swibots/bots/handlers/member_left_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      960 2023-02-04 19:02:01.000000 swibots-1.2.1/swibots/bots/handlers/message_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      885 2023-01-19 01:21:52.000000 swibots-1.2.1/swibots/bots/handlers/unknown_command_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      670 2023-03-20 17:14:14.000000 swibots-1.2.1/swibots/bots/handlers/user_banned_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      285 2023-01-23 21:16:29.000000 swibots-1.2.1/swibots/bots/register_command.py
+-rwxr-xr-x   0 root         (0) root         (0)     1621 2023-05-23 05:29:40.000000 swibots-1.2.1/swibots/config.py
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/error.py
+-rwxr-xr-x   0 root         (0) root         (0)      854 2023-03-20 17:15:29.000000 swibots-1.2.1/swibots/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:25.328053 swibots-1.2.1/swibots/utils/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-01-16 05:53:47.000000 swibots-1.2.1/swibots/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5880 2023-04-20 23:47:11.000000 swibots-1.2.1/swibots/utils/rest_client.py
+-rw-r--r--   0 root         (0) root         (0)     2475 2023-02-04 19:02:18.000000 swibots-1.2.1/swibots/utils/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:25.332846 swibots-1.2.1/swibots/utils/ws/
+-rw-r--r--   0 root         (0) root         (0)       48 2023-01-19 05:23:27.000000 swibots-1.2.1/swibots/utils/ws/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:25.363834 swibots-1.2.1/swibots/utils/ws/asyncstomp/
+-rw-r--r--   0 root         (0) root         (0)      150 2023-01-09 05:33:14.000000 swibots-1.2.1/swibots/utils/ws/asyncstomp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9743 2023-01-21 06:34:39.000000 swibots-1.2.1/swibots/utils/ws/asyncstomp/async_ws_client.py
+-rw-r--r--   0 root         (0) root         (0)      980 2023-01-19 01:21:52.000000 swibots-1.2.1/swibots/utils/ws/asyncstomp/async_ws_subscription.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:25.395274 swibots-1.2.1/swibots/utils/ws/common/
+-rw-r--r--   0 root         (0) root         (0)      100 2023-01-09 05:33:14.000000 swibots-1.2.1/swibots/utils/ws/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-01-09 05:33:14.000000 swibots-1.2.1/swibots/utils/ws/common/ws_frame.py
+-rw-r--r--   0 root         (0) root         (0)      430 2023-01-09 05:33:14.000000 swibots-1.2.1/swibots/utils/ws/common/ws_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:24.033503 swibots-1.2.1/swibots.egg-info/
+-rwxr-xr-x   0 root         (0) root         (0)     1817 2023-05-23 05:58:23.000000 swibots-1.2.1/swibots.egg-info/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     7316 2023-05-23 05:58:23.000000 swibots-1.2.1/swibots.egg-info/SOURCES.txt
+-rwxr-xr-x   0 root         (0) root         (0)        1 2023-05-23 05:58:23.000000 swibots-1.2.1/swibots.egg-info/dependency_links.txt
+-rwxr-xr-x   0 root         (0) root         (0)       31 2023-05-23 05:58:23.000000 swibots-1.2.1/swibots.egg-info/requires.txt
+-rwxr-xr-x   0 root         (0) root         (0)       14 2023-05-23 05:58:23.000000 swibots-1.2.1/swibots.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 05:58:25.422717 swibots-1.2.1/tests/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 05:56:05.000000 swibots-1.2.1/tests/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      202 2023-01-15 22:26:25.000000 swibots-1.2.1/tests/tests.py
```

### Comparing `swibots-1.2.0/PKG-INFO` & `swibots-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swibots
-Version: 1.2.0
+Version: 1.2.1
 Summary: Switch bot api
 Home-page: https://github.com/switchcollab/Switch-Bots-Python-Library
 Author: switchadmin
 Author-email: support@switch.pe
 License: LGPLv3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `swibots-1.2.0/README.md` & `swibots-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/setup.py` & `swibots-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = pypandoc.convert_file("README.md", "rst")
 except (IOError, ImportError):
     long_description = open("README.md").read()
 
 
 setup(
     name="swibots",
-    version="1.2.0",
+    version="1.2.1",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/switchcollab/Switch-Bots-Python-Library",
     description="Switch bot api",
     author="switchadmin",
     author_email="support@switch.pe",
```

### Comparing `swibots-1.2.0/swibots/api/api_client.py` & `swibots-1.2.1/swibots/api/api_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/auth/auth_client.py` & `swibots-1.2.1/swibots/api/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/auth/controllers/user_controller.py` & `swibots-1.2.1/swibots/api/auth/controllers/user_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/auth/methods/get_me.py` & `swibots-1.2.1/swibots/api/auth/methods/get_me.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/auth/methods/login.py` & `swibots-1.2.1/swibots/api/auth/methods/login.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/auth/models/auth_user.py` & `swibots-1.2.1/swibots/api/auth/models/auth_user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/bot/bot_client.py` & `swibots-1.2.1/swibots/api/bot/bot_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/bot/controllers/bot_controller.py` & `swibots-1.2.1/swibots/api/bot/controllers/bot_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/bot/methods/delete_bot_info.py` & `swibots-1.2.1/swibots/api/bot/methods/delete_bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/bot/methods/get_bot_info.py` & `swibots-1.2.1/swibots/api/bot/methods/get_bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/bot/methods/update_bot_info.py` & `swibots-1.2.1/swibots/api/bot/methods/update_bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/bot/models/bot_command_info.py` & `swibots-1.2.1/swibots/api/bot/models/bot_command_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/bot/models/bot_info.py` & `swibots-1.2.1/swibots/api/bot/models/bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/chat_client.py` & `swibots-1.2.1/swibots/api/chat/chat_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/controllers/message_controller.py` & `swibots-1.2.1/swibots/api/chat/controllers/message_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/events/callback_query_event.py` & `swibots-1.2.1/swibots/api/chat/events/callback_query_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/events/chat_event.py` & `swibots-1.2.1/swibots/api/chat/events/chat_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/events/command_event.py` & `swibots-1.2.1/swibots/api/chat/events/command_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/events/inline_query_event.py` & `swibots-1.2.1/swibots/api/chat/events/inline_query_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/events/message_event.py` & `swibots-1.2.1/swibots/api/chat/events/message_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/methods/__init__.py` & `swibots-1.2.1/swibots/api/chat/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/methods/answer_inline_query.py` & `swibots-1.2.1/swibots/api/chat/methods/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/methods/clear_conversation.py` & `swibots-1.2.1/swibots/api/chat/methods/clear_conversation.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/methods/delete_message.py` & `swibots-1.2.1/swibots/api/chat/methods/delete_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/methods/delete_messages_from_user.py` & `swibots-1.2.1/swibots/api/chat/methods/delete_messages_from_user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/methods/download_media.py` & `swibots-1.2.1/swibots/api/chat/methods/download_media.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/methods/edit_message.py` & `swibots-1.2.1/swibots/api/chat/methods/edit_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/methods/edit_message_text.py` & `swibots-1.2.1/swibots/api/chat/methods/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/methods/flag_message.py` & `swibots-1.2.1/swibots/api/chat/methods/flag_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/methods/forward_message.py` & `swibots-1.2.1/swibots/api/chat/methods/forward_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/methods/get_channel_chat_history.py` & `swibots-1.2.1/swibots/api/chat/methods/get_channel_chat_history.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/methods/get_community_media_files.py` & `swibots-1.2.1/swibots/api/chat/methods/get_community_media_files.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/methods/get_community_media_files_by_status.py` & `swibots-1.2.1/swibots/api/chat/methods/get_community_media_files_by_status.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/methods/get_flag_messages.py` & `swibots-1.2.1/swibots/api/chat/methods/get_flag_messages.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/methods/get_group_chat_history.py` & `swibots-1.2.1/swibots/api/chat/methods/get_group_chat_history.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/methods/get_message.py` & `swibots-1.2.1/swibots/api/chat/methods/get_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/methods/get_messages.py` & `swibots-1.2.1/swibots/api/chat/methods/get_messages.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/methods/get_messages_between_users.py` & `swibots-1.2.1/swibots/api/chat/methods/get_messages_between_users.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/methods/get_unread_messages_count.py` & `swibots-1.2.1/swibots/api/chat/methods/get_unread_messages_count.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/methods/get_user_media_files.py` & `swibots-1.2.1/swibots/api/chat/methods/get_user_media_files.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/methods/reply_message.py` & `swibots-1.2.1/swibots/api/chat/methods/reply_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/methods/reply_message_text.py` & `swibots-1.2.1/swibots/api/chat/methods/reply_message_text.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/methods/send_message.py` & `swibots-1.2.1/swibots/api/chat/methods/send_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/methods/send_text.py` & `swibots-1.2.1/swibots/api/chat/methods/send_text.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/models/group_chat_history.py` & `swibots-1.2.1/swibots/api/chat/models/group_chat_history.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/models/inline/__init__.py` & `swibots-1.2.1/swibots/api/chat/models/inline/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/models/inline/base_typed_inline_query_result.py` & `swibots-1.2.1/swibots/api/chat/models/inline/base_typed_inline_query_result.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/models/inline/inline_query.py` & `swibots-1.2.1/swibots/api/chat/models/inline/inline_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/models/inline/inline_query_answer.py` & `swibots-1.2.1/swibots/api/chat/models/inline/inline_query_answer.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/models/inline/inline_query_result.py` & `swibots-1.2.1/swibots/api/chat/models/inline/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/models/inline/inline_query_result_article.py` & `swibots-1.2.1/swibots/api/chat/models/inline/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/models/inline/inline_query_result_document.py` & `swibots-1.2.1/swibots/api/chat/models/inline/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/models/inline/inline_query_result_photo.py` & `swibots-1.2.1/swibots/api/chat/models/inline/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/models/inline/inline_query_result_video.py` & `swibots-1.2.1/swibots/api/chat/models/inline/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/models/inline/input_message_content.py` & `swibots-1.2.1/swibots/api/chat/models/inline/input_message_content.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/models/inline_keyboard_button.py` & `swibots-1.2.1/swibots/api/chat/models/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/models/inline_markup.py` & `swibots-1.2.1/swibots/api/chat/models/inline_markup.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/chat/models/message.py` & `swibots-1.2.1/swibots/api/chat/models/message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/common/events/event.py` & `swibots-1.2.1/swibots/api/common/events/event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/common/models/media.py` & `swibots-1.2.1/swibots/api/common/models/media.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/common/models/media_upload_request.py` & `swibots-1.2.1/swibots/api/common/models/media_upload_request.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/common/models/user.py` & `swibots-1.2.1/swibots/api/common/models/user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/community/community_client.py` & `swibots-1.2.1/swibots/api/community/community_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/community/controllers/channel_controller.py` & `swibots-1.2.1/swibots/api/community/controllers/channel_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/community/controllers/community_controller.py` & `swibots-1.2.1/swibots/api/community/controllers/community_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/community/controllers/group_controller.py` & `swibots-1.2.1/swibots/api/community/controllers/group_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/community/events/__init__.py` & `swibots-1.2.1/swibots/api/community/events/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/community/events/channel_created_event.py` & `swibots-1.2.1/swibots/api/community/events/channel_created_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/community/events/channel_deleted_event.py` & `swibots-1.2.1/swibots/api/community/events/channel_deleted_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/community/events/channel_updated_event.py` & `swibots-1.2.1/swibots/api/community/events/channel_updated_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/community/events/community_event.py` & `swibots-1.2.1/swibots/api/community/events/community_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/community/events/community_updated_event.py` & `swibots-1.2.1/swibots/api/community/events/community_updated_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/community/events/group_created_event.py` & `swibots-1.2.1/swibots/api/community/events/group_created_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/community/events/group_deleted_event.py` & `swibots-1.2.1/swibots/api/community/events/group_deleted_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/community/events/group_updated_event.py` & `swibots-1.2.1/swibots/api/community/events/group_updated_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/community/events/member_joined_event.py` & `swibots-1.2.1/swibots/api/community/events/member_joined_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/community/events/member_left_event.py` & `swibots-1.2.1/swibots/api/community/events/member_left_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/community/events/user_banned_event.py` & `swibots-1.2.1/swibots/api/community/events/user_banned_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/community/methods/get_channel.py` & `swibots-1.2.1/swibots/api/community/methods/get_channel.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/community/methods/get_community.py` & `swibots-1.2.1/swibots/api/community/methods/get_community.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/community/methods/get_group.py` & `swibots-1.2.1/swibots/api/community/methods/get_group.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/community/models/channel.py` & `swibots-1.2.1/swibots/api/community/models/channel.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/community/models/community.py` & `swibots-1.2.1/swibots/api/community/models/community.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/api/community/models/group.py` & `swibots-1.2.1/swibots/api/community/models/group.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/app.py` & `swibots-1.2.1/swibots/app.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/base/rest_response.py` & `swibots-1.2.1/swibots/base/rest_response.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/base/switch_client.py` & `swibots-1.2.1/swibots/base/switch_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/base/switch_object.py` & `swibots-1.2.1/swibots/base/switch_object.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/base/switch_ws_async_client.py` & `swibots-1.2.1/swibots/base/switch_ws_async_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bot_app.py` & `swibots-1.2.1/swibots/bot_app.py`

 * *Files 9% similar despite different names*

```diff
@@ -83,14 +83,22 @@
     def add_handler(self, handler: BaseHandler | List[BaseHandler]) -> "BotApp":
         if isinstance(handler, list):
             self.handlers.extend(handler)
         else:
             self.handlers.append(handler)
         return self
 
+    def remove_handler(self, handler: BaseHandler | List[BaseHandler]) -> "BotApp":
+        if isinstance(handler, list):
+            for h in handler:
+                self.handlers.remove(h)
+        else:
+            self.handlers.remove(handler)
+        return self
+
     async def _validate_token(self):
         await super()._validate_token()
         if not isinstance(self.user, swibots.Bot):
             raise swibots.SwitchError("Invalid token")
 
         if not self.user.is_bot:
             raise swibots.SwitchError("Invalid token (not a bot)")
```

### Comparing `swibots-1.2.0/swibots/bots/bot.py` & `swibots-1.2.1/swibots/bots/bot.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/bot_context.py` & `swibots-1.2.1/swibots/bots/bot_context.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/decorators/__init__.py` & `swibots-1.2.1/swibots/bots/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/decorators/on_callback_query.py` & `swibots-1.2.1/swibots/bots/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/decorators/on_channel_deleted.py` & `swibots-1.2.1/swibots/bots/decorators/on_channel_deleted.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/decorators/on_channel_updated.py` & `swibots-1.2.1/swibots/bots/decorators/on_channel_updated.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/decorators/on_command.py` & `swibots-1.2.1/swibots/bots/decorators/on_command.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/decorators/on_community_updated.py` & `swibots-1.2.1/swibots/bots/decorators/on_community_updated.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/decorators/on_group_created.py` & `swibots-1.2.1/swibots/bots/decorators/on_group_created.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/decorators/on_group_deleted.py` & `swibots-1.2.1/swibots/bots/decorators/on_group_deleted.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/decorators/on_group_updated.py` & `swibots-1.2.1/swibots/bots/decorators/on_group_updated.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/decorators/on_inline_query.py` & `swibots-1.2.1/swibots/bots/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/decorators/on_member_joined.py` & `swibots-1.2.1/swibots/bots/decorators/on_member_joined.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/decorators/on_member_left.py` & `swibots-1.2.1/swibots/bots/decorators/on_member_left.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/decorators/on_unknown_command.py` & `swibots-1.2.1/swibots/bots/decorators/on_unknown_command.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/filters/filter.py` & `swibots-1.2.1/swibots/bots/filters/filter.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/handlers/__init__.py` & `swibots-1.2.1/swibots/bots/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/handlers/base_handler.py` & `swibots-1.2.1/swibots/bots/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/handlers/callback_query_handler.py` & `swibots-1.2.1/swibots/bots/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/handlers/channel_created_handler.py` & `swibots-1.2.1/swibots/bots/handlers/channel_created_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/handlers/channel_deleted_handler.py` & `swibots-1.2.1/swibots/bots/handlers/channel_deleted_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/handlers/channel_updated_handler.py` & `swibots-1.2.1/swibots/bots/handlers/channel_updated_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/handlers/command_handler.py` & `swibots-1.2.1/swibots/bots/handlers/command_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/handlers/community_updated_handler.py` & `swibots-1.2.1/swibots/bots/handlers/community_updated_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/handlers/event_handler.py` & `swibots-1.2.1/swibots/bots/handlers/event_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/handlers/group_created_handler.py` & `swibots-1.2.1/swibots/bots/handlers/group_created_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/handlers/group_deleted_handler.py` & `swibots-1.2.1/swibots/bots/handlers/group_deleted_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/handlers/group_updated_handler.py` & `swibots-1.2.1/swibots/bots/handlers/group_updated_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/handlers/inline_query_handler.py` & `swibots-1.2.1/swibots/bots/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/handlers/member_joined_handler.py` & `swibots-1.2.1/swibots/bots/handlers/member_joined_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/handlers/member_left_handler.py` & `swibots-1.2.1/swibots/bots/handlers/member_left_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/handlers/message_handler.py` & `swibots-1.2.1/swibots/bots/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/handlers/unknown_command_handler.py` & `swibots-1.2.1/swibots/bots/handlers/unknown_command_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/bots/handlers/user_banned_handler.py` & `swibots-1.2.1/swibots/bots/handlers/user_banned_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/config.py` & `swibots-1.2.1/swibots/config.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/error.py` & `swibots-1.2.1/swibots/error.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/types.py` & `swibots-1.2.1/swibots/types.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/utils/rest_client.py` & `swibots-1.2.1/swibots/utils/rest_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/utils/types.py` & `swibots-1.2.1/swibots/utils/types.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/utils/ws/asyncstomp/async_ws_client.py` & `swibots-1.2.1/swibots/utils/ws/asyncstomp/async_ws_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/utils/ws/asyncstomp/async_ws_subscription.py` & `swibots-1.2.1/swibots/utils/ws/asyncstomp/async_ws_subscription.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots/utils/ws/common/ws_frame.py` & `swibots-1.2.1/swibots/utils/ws/common/ws_frame.py`

 * *Files identical despite different names*

### Comparing `swibots-1.2.0/swibots.egg-info/PKG-INFO` & `swibots-1.2.1/swibots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swibots
-Version: 1.2.0
+Version: 1.2.1
 Summary: Switch bot api
 Home-page: https://github.com/switchcollab/Switch-Bots-Python-Library
 Author: switchadmin
 Author-email: support@switch.pe
 License: LGPLv3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `swibots-1.2.0/swibots.egg-info/SOURCES.txt` & `swibots-1.2.1/swibots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

