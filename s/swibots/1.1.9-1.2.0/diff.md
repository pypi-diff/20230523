# Comparing `tmp/swibots-1.1.9.tar.gz` & `tmp/swibots-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swibots-1.1.9.tar", last modified: Wed May 17 11:43:15 2023, max compression
+gzip compressed data, was "swibots-1.2.0.tar", last modified: Tue May 23 03:39:53 2023, max compression
```

## Comparing `swibots-1.1.9.tar` & `swibots-1.2.0.tar`

### file list

```diff
@@ -1,215 +1,218 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.529919 swibots-1.1.9/
--rw-rw-rw-   0        0        0     1892 2023-05-17 11:43:15.528923 swibots-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     1538 2023-02-13 07:44:30.000000 swibots-1.1.9/README.md
--rw-rw-rw-   0        0        0       42 2023-05-17 11:43:15.529919 swibots-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0      758 2023-05-17 11:42:12.000000 swibots-1.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.012921 swibots-1.1.9/swibots/
--rw-rw-rw-   0        0        0      236 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.068923 swibots-1.1.9/swibots/api/
--rw-rw-rw-   0        0        0      140 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/__init__.py
--rw-rw-rw-   0        0        0     2236 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/api_client.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.073934 swibots-1.1.9/swibots/api/auth/
--rw-rw-rw-   0        0        0       85 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/auth/__init__.py
--rw-rw-rw-   0        0        0     1220 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/auth/auth_client.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.082935 swibots-1.1.9/swibots/api/auth/controllers/
--rw-rw-rw-   0        0        0       73 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/auth/controllers/__init__.py
--rw-rw-rw-   0        0        0     1514 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/auth/controllers/user_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.093924 swibots-1.1.9/swibots/api/auth/methods/
--rw-rw-rw-   0        0        0       94 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/auth/methods/__init__.py
--rw-rw-rw-   0        0        0      650 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/auth/methods/get_me.py
--rw-rw-rw-   0        0        0      837 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/auth/methods/login.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.100923 swibots-1.1.9/swibots/api/auth/models/
--rw-rw-rw-   0        0        0       56 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/auth/models/__init__.py
--rw-rw-rw-   0        0        0     4642 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/auth/models/auth_user.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.108922 swibots-1.1.9/swibots/api/bot/
--rw-rw-rw-   0        0        0       83 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/bot/__init__.py
--rw-rw-rw-   0        0        0     1141 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/bot/bot_client.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.116923 swibots-1.1.9/swibots/api/bot/controllers/
--rw-rw-rw-   0        0        0       71 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/bot/controllers/__init__.py
--rw-rw-rw-   0        0        0     1790 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/bot/controllers/bot_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.132923 swibots-1.1.9/swibots/api/bot/methods/
--rw-rw-rw-   0        0        0      209 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/bot/methods/__init__.py
--rw-rw-rw-   0        0        0      540 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/bot/methods/delete_bot_info.py
--rw-rw-rw-   0        0        0      582 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/bot/methods/get_bot_info.py
--rw-rw-rw-   0        0        0      615 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/bot/methods/update_bot_info.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.144923 swibots-1.1.9/swibots/api/bot/models/
--rw-rw-rw-   0        0        0      116 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/bot/models/__init__.py
--rw-rw-rw-   0        0        0      955 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/bot/models/bot_command_info.py
--rw-rw-rw-   0        0        0     1585 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/bot/models/bot_info.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.151926 swibots-1.1.9/swibots/api/chat/
--rw-rw-rw-   0        0        0      107 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/__init__.py
--rw-rw-rw-   0        0        0     5372 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/chat_client.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.158927 swibots-1.1.9/swibots/api/chat/controllers/
--rw-rw-rw-   0        0        0       83 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/controllers/__init__.py
--rw-rw-rw-   0        0        0    21518 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/controllers/message_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.182927 swibots-1.1.9/swibots/api/chat/events/
--rw-rw-rw-   0        0        0      326 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/events/__init__.py
--rw-rw-rw-   0        0        0     2073 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/events/callback_query_event.py
--rw-rw-rw-   0        0        0     2731 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/events/chat_event.py
--rw-rw-rw-   0        0        0     2095 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/events/command_event.py
--rw-rw-rw-   0        0        0     2103 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/events/inline_query_event.py
--rw-rw-rw-   0        0        0     2434 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/events/message_event.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.258924 swibots-1.1.9/swibots/api/chat/methods/
--rw-rw-rw-   0        0        0     1709 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/methods/__init__.py
--rw-rw-rw-   0        0        0      654 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/methods/answer_inline_query.py
--rw-rw-rw-   0        0        0      693 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/methods/clear_conversation.py
--rw-rw-rw-   0        0        0      705 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/methods/delete_message.py
--rw-rw-rw-   0        0        0      707 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/methods/delete_messages_from_user.py
--rw-rw-rw-   0        0        0     1358 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/methods/download_media.py
--rw-rw-rw-   0        0        0      750 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/methods/edit_message.py
--rw-rw-rw-   0        0        0      853 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/methods/edit_message_text.py
--rw-rw-rw-   0        0        0      693 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/methods/flag_message.py
--rw-rw-rw-   0        0        0     1192 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/methods/forward_message.py
--rw-rw-rw-   0        0        0     1139 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/methods/get_channel_chat_history.py
--rw-rw-rw-   0        0        0      725 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/methods/get_community_media_files.py
--rw-rw-rw-   0        0        0      883 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/methods/get_community_media_files_by_status.py
--rw-rw-rw-   0        0        0      636 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/methods/get_flag_messages.py
--rw-rw-rw-   0        0        0     1090 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/methods/get_group_chat_history.py
--rw-rw-rw-   0        0        0      649 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/methods/get_message.py
--rw-rw-rw-   0        0        0      707 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/methods/get_messages.py
--rw-rw-rw-   0        0        0     1102 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/methods/get_messages_between_users.py
--rw-rw-rw-   0        0        0      560 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/methods/get_unread_messages_count.py
--rw-rw-rw-   0        0        0      785 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/methods/get_user_media_files.py
--rw-rw-rw-   0        0        0      881 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/methods/reply_message.py
--rw-rw-rw-   0        0        0     1032 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/methods/reply_message_text.py
--rw-rw-rw-   0        0        0      849 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/methods/send_message.py
--rw-rw-rw-   0        0        0     1136 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/methods/send_text.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.280922 swibots-1.1.9/swibots/api/chat/models/
--rw-rw-rw-   0        0        0      305 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/models/__init__.py
--rw-rw-rw-   0        0        0      920 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/models/group_chat_history.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.313921 swibots-1.1.9/swibots/api/chat/models/inline/
--rw-rw-rw-   0        0        0      565 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/models/inline/__init__.py
--rw-rw-rw-   0        0        0     1371 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/models/inline/base_typed_inline_query_result.py
--rw-rw-rw-   0        0        0     2533 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/models/inline/inline_query.py
--rw-rw-rw-   0        0        0     1871 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/models/inline/inline_query_answer.py
--rw-rw-rw-   0        0        0      991 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/models/inline/inline_query_result.py
--rw-rw-rw-   0        0        0     1158 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/models/inline/inline_query_result_article.py
--rw-rw-rw-   0        0        0     1273 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/models/inline/inline_query_result_document.py
--rw-rw-rw-   0        0        0     1620 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/models/inline/inline_query_result_photo.py
--rw-rw-rw-   0        0        0     1760 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/models/inline/inline_query_result_video.py
--rw-rw-rw-   0        0        0      581 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/models/inline/input_message_content.py
--rw-rw-rw-   0        0        0      201 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/models/inline/types.py
--rw-rw-rw-   0        0        0      886 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/models/inline_keyboard_button.py
--rw-rw-rw-   0        0        0      170 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/models/inline_keyboard_color.py
--rw-rw-rw-   0        0        0      146 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/models/inline_keyboard_size.py
--rw-rw-rw-   0        0        0     2065 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/models/inline_markup.py
--rw-rw-rw-   0        0        0    10769 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/chat/models/message.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.316924 swibots-1.1.9/swibots/api/common/
--rw-rw-rw-   0        0        0       44 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.320925 swibots-1.1.9/swibots/api/common/events/
--rw-rw-rw-   0        0        0       46 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/common/events/__init__.py
--rw-rw-rw-   0        0        0     2789 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/common/events/event.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.330923 swibots-1.1.9/swibots/api/common/models/
--rw-rw-rw-   0        0        0      101 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/common/models/__init__.py
--rw-rw-rw-   0        0        0     2004 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/common/models/media.py
--rw-rw-rw-   0        0        0     1565 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/common/models/media_upload_request.py
--rw-rw-rw-   0        0        0     1706 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/common/models/user.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.334922 swibots-1.1.9/swibots/api/community/
--rw-rw-rw-   0        0        0       90 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/community/__init__.py
--rw-rw-rw-   0        0        0     5180 2023-05-16 11:13:47.000000 swibots-1.1.9/swibots/api/community/community_client.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.343924 swibots-1.1.9/swibots/api/community/controllers/
--rw-rw-rw-   0        0        0      102 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/community/controllers/__init__.py
--rw-rw-rw-   0        0        0      595 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/community/controllers/channel_controller.py
--rw-rw-rw-   0        0        0      616 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/community/controllers/community_controller.py
--rw-rw-rw-   0        0        0      576 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/community/controllers/group_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.371925 swibots-1.1.9/swibots/api/community/events/
--rw-rw-rw-   0        0        0      566 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/community/events/__init__.py
--rw-rw-rw-   0        0        0     1428 2023-05-16 11:13:47.000000 swibots-1.1.9/swibots/api/community/events/channel_created_event.py
--rw-rw-rw-   0        0        0     1428 2023-05-16 11:13:47.000000 swibots-1.1.9/swibots/api/community/events/channel_deleted_event.py
--rw-rw-rw-   0        0        0     1428 2023-05-16 11:13:47.000000 swibots-1.1.9/swibots/api/community/events/channel_updated_event.py
--rw-rw-rw-   0        0        0     2303 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/community/events/community_event.py
--rw-rw-rw-   0        0        0     1383 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/community/events/community_updated_event.py
--rw-rw-rw-   0        0        0     1422 2023-05-16 11:13:47.000000 swibots-1.1.9/swibots/api/community/events/group_created_event.py
--rw-rw-rw-   0        0        0     1422 2023-05-16 11:13:47.000000 swibots-1.1.9/swibots/api/community/events/group_deleted_event.py
--rw-rw-rw-   0        0        0     1422 2023-05-16 11:13:47.000000 swibots-1.1.9/swibots/api/community/events/group_updated_event.py
--rw-rw-rw-   0        0        0     1421 2023-05-16 11:13:47.000000 swibots-1.1.9/swibots/api/community/events/member_joined_event.py
--rw-rw-rw-   0        0        0     1418 2023-05-16 11:13:47.000000 swibots-1.1.9/swibots/api/community/events/member_left_event.py
--rw-rw-rw-   0        0        0     1414 2023-05-16 11:13:47.000000 swibots-1.1.9/swibots/api/community/events/user_banned_event.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.381924 swibots-1.1.9/swibots/api/community/methods/
--rw-rw-rw-   0        0        0      194 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/community/methods/__init__.py
--rw-rw-rw-   0        0        0      643 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/community/methods/get_channel.py
--rw-rw-rw-   0        0        0      668 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/community/methods/get_community.py
--rw-rw-rw-   0        0        0      619 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/community/methods/get_group.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.389928 swibots-1.1.9/swibots/api/community/models/
--rw-rw-rw-   0        0        0      132 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/community/models/__init__.py
--rw-rw-rw-   0        0        0     2743 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/community/models/channel.py
--rw-rw-rw-   0        0        0     2954 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/community/models/community.py
--rw-rw-rw-   0        0        0     2720 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/api/community/models/group.py
--rw-rw-rw-   0        0        0     9347 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/app.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.406924 swibots-1.1.9/swibots/base/
--rw-rw-rw-   0        0        0      262 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/base/__init__.py
--rw-rw-rw-   0        0        0       69 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/base/rest_controller.py
--rw-rw-rw-   0        0        0      370 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/base/rest_request.py
--rw-rw-rw-   0        0        0      644 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/base/rest_response.py
--rw-rw-rw-   0        0        0     4261 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/base/switch_client.py
--rw-rw-rw-   0        0        0     1180 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/base/switch_object.py
--rw-rw-rw-   0        0        0      543 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/base/switch_ws_async_client.py
--rw-rw-rw-   0        0        0     4329 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bot_app.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.417921 swibots-1.1.9/swibots/bots/
--rw-rw-rw-   0        0        0      201 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/__init__.py
--rw-rw-rw-   0        0        0     4646 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/bot.py
--rw-rw-rw-   0        0        0     1646 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/bot_context.py
--rw-rw-rw-   0        0        0      109 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.455923 swibots-1.1.9/swibots/bots/decorators/
--rw-rw-rw-   0        0        0      999 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/decorators/__init__.py
--rw-rw-rw-   0        0        0      540 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/decorators/on_callback_query.py
--rw-rw-rw-   0        0        0      510 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/decorators/on_channel_created.py
--rw-rw-rw-   0        0        0      544 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/decorators/on_channel_deleted.py
--rw-rw-rw-   0        0        0      541 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/decorators/on_channel_updated.py
--rw-rw-rw-   0        0        0      574 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/decorators/on_command.py
--rw-rw-rw-   0        0        0      544 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/decorators/on_community_updated.py
--rw-rw-rw-   0        0        0      536 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/decorators/on_group_created.py
--rw-rw-rw-   0        0        0      536 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/decorators/on_group_deleted.py
--rw-rw-rw-   0        0        0      534 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/decorators/on_group_updated.py
--rw-rw-rw-   0        0        0      537 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/decorators/on_inline_query.py
--rw-rw-rw-   0        0        0      534 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/decorators/on_member_joined.py
--rw-rw-rw-   0        0        0      529 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/decorators/on_member_left.py
--rw-rw-rw-   0        0        0      503 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/decorators/on_message.py
--rw-rw-rw-   0        0        0      543 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/decorators/on_unknown_command.py
--rw-rw-rw-   0        0        0      509 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/decorators/on_user_banned.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.460926 swibots-1.1.9/swibots/bots/filters/
--rw-rw-rw-   0        0        0       22 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/filters/__init__.py
--rw-rw-rw-   0        0        0     8057 2023-05-16 11:13:47.000000 swibots-1.1.9/swibots/bots/filters/filter.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.500924 swibots-1.1.9/swibots/bots/handlers/
--rw-rw-rw-   0        0        0     1300 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/handlers/__init__.py
--rw-rw-rw-   0        0        0     1048 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/handlers/base_handler.py
--rw-rw-rw-   0        0        0      985 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/handlers/callback_query_handler.py
--rw-rw-rw-   0        0        0      704 2023-05-16 11:13:47.000000 swibots-1.1.9/swibots/bots/handlers/channel_created_handler.py
--rw-rw-rw-   0        0        0      711 2023-05-16 11:13:47.000000 swibots-1.1.9/swibots/bots/handlers/channel_deleted_handler.py
--rw-rw-rw-   0        0        0      758 2023-05-16 11:13:47.000000 swibots-1.1.9/swibots/bots/handlers/channel_updated_handler.py
--rw-rw-rw-   0        0        0     1514 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/handlers/command_handler.py
--rw-rw-rw-   0        0        0      686 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/handlers/community_updated_handler.py
--rw-rw-rw-   0        0        0     1325 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/handlers/event_handler.py
--rw-rw-rw-   0        0        0      703 2023-05-16 11:13:47.000000 swibots-1.1.9/swibots/bots/handlers/group_created_handler.py
--rw-rw-rw-   0        0        0      800 2023-05-16 11:13:47.000000 swibots-1.1.9/swibots/bots/handlers/group_deleted_handler.py
--rw-rw-rw-   0        0        0      800 2023-05-16 11:13:47.000000 swibots-1.1.9/swibots/bots/handlers/group_updated_handler.py
--rw-rw-rw-   0        0        0      867 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/handlers/inline_query_handler.py
--rw-rw-rw-   0        0        0      702 2023-05-16 11:13:47.000000 swibots-1.1.9/swibots/bots/handlers/member_joined_handler.py
--rw-rw-rw-   0        0        0      697 2023-05-16 11:13:47.000000 swibots-1.1.9/swibots/bots/handlers/member_left_handler.py
--rw-rw-rw-   0        0        0      960 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/handlers/message_handler.py
--rw-rw-rw-   0        0        0      885 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/handlers/unknown_command_handler.py
--rw-rw-rw-   0        0        0      693 2023-05-16 11:13:47.000000 swibots-1.1.9/swibots/bots/handlers/user_banned_handler.py
--rw-rw-rw-   0        0        0      285 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/bots/register_command.py
--rw-rw-rw-   0        0        0     1649 2023-05-17 11:35:00.000000 swibots-1.1.9/swibots/config.py
--rw-rw-rw-   0        0        0     1333 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/error.py
--rw-rw-rw-   0        0        0      878 2023-05-16 11:13:47.000000 swibots-1.1.9/swibots/types.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.507919 swibots-1.1.9/swibots/utils/
--rw-rw-rw-   0        0        0       75 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/utils/__init__.py
--rw-rw-rw-   0        0        0     5880 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/utils/rest_client.py
--rw-rw-rw-   0        0        0     2475 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/utils/types.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.510922 swibots-1.1.9/swibots/utils/ws/
--rw-rw-rw-   0        0        0       48 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/utils/ws/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.518921 swibots-1.1.9/swibots/utils/ws/asyncstomp/
--rw-rw-rw-   0        0        0      150 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/utils/ws/asyncstomp/__init__.py
--rw-rw-rw-   0        0        0     9743 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/utils/ws/asyncstomp/async_ws_client.py
--rw-rw-rw-   0        0        0      980 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/utils/ws/asyncstomp/async_ws_subscription.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.525923 swibots-1.1.9/swibots/utils/ws/common/
--rw-rw-rw-   0        0        0      100 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/utils/ws/common/__init__.py
--rw-rw-rw-   0        0        0     1654 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/utils/ws/common/ws_frame.py
--rw-rw-rw-   0        0        0      430 2023-02-13 07:44:31.000000 swibots-1.1.9/swibots/utils/ws/common/ws_message.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:43:15.061922 swibots-1.1.9/swibots.egg-info/
--rw-rw-rw-   0        0        0     1892 2023-05-17 11:43:14.000000 swibots-1.1.9/swibots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7283 2023-05-17 11:43:14.000000 swibots-1.1.9/swibots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 11:43:14.000000 swibots-1.1.9/swibots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-05-17 11:43:14.000000 swibots-1.1.9/swibots.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-17 11:43:14.000000 swibots-1.1.9/swibots.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:53.382433 swibots-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-05-23 03:39:53.381596 swibots-1.2.0/PKG-INFO
+-r---w----   0 root         (0) root         (0)     1538 2023-01-19 02:17:00.000000 swibots-1.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 03:39:53.382882 swibots-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      731 2023-05-23 03:39:47.000000 swibots-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.077372 swibots-1.2.0/swibots/
+-rw-r--r--   0 root         (0) root         (0)      236 2023-01-16 12:19:14.000000 swibots-1.2.0/swibots/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.125857 swibots-1.2.0/swibots/api/
+-rw-r--r--   0 root         (0) root         (0)      140 2023-01-16 06:31:11.000000 swibots-1.2.0/swibots/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2023-01-21 06:26:21.000000 swibots-1.2.0/swibots/api/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.135942 swibots-1.2.0/swibots/api/auth/
+-rw-r--r--   0 root         (0) root         (0)       85 2023-01-16 07:03:12.000000 swibots-1.2.0/swibots/api/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-01-23 17:55:04.000000 swibots-1.2.0/swibots/api/auth/auth_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.147394 swibots-1.2.0/swibots/api/auth/controllers/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-01-09 05:33:14.000000 swibots-1.2.0/swibots/api/auth/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1514 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/auth/controllers/user_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.164875 swibots-1.2.0/swibots/api/auth/methods/
+-rwxr-xr-x   0 root         (0) root         (0)       94 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/auth/methods/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      650 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/auth/methods/get_me.py
+-rw-r--r--   0 root         (0) root         (0)      837 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/auth/methods/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.181886 swibots-1.2.0/swibots/api/auth/models/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-01-13 05:35:17.000000 swibots-1.2.0/swibots/api/auth/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4642 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/api/auth/models/auth_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.195972 swibots-1.2.0/swibots/api/bot/
+-rwxr-xr-x   0 root         (0) root         (0)       83 2023-01-16 06:01:42.000000 swibots-1.2.0/swibots/api/bot/__init__.py
+-r---w----   0 root         (0) root         (0)     1141 2023-01-23 17:54:24.000000 swibots-1.2.0/swibots/api/bot/bot_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.205715 swibots-1.2.0/swibots/api/bot/controllers/
+-r---w----   0 root         (0) root         (0)       71 2023-01-15 12:54:24.000000 swibots-1.2.0/swibots/api/bot/controllers/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1790 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/bot/controllers/bot_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.239243 swibots-1.2.0/swibots/api/bot/methods/
+-rwxr-xr-x   0 root         (0) root         (0)      209 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/bot/methods/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      540 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/bot/methods/delete_bot_info.py
+-rwxr-xr-x   0 root         (0) root         (0)      582 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/bot/methods/get_bot_info.py
+-rwxr-xr-x   0 root         (0) root         (0)      615 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/bot/methods/update_bot_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.262712 swibots-1.2.0/swibots/api/bot/models/
+-rwxr-xr-x   0 root         (0) root         (0)      116 2023-01-15 13:00:36.000000 swibots-1.2.0/swibots/api/bot/models/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      955 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/api/bot/models/bot_command_info.py
+-rwxr-xr-x   0 root         (0) root         (0)     1585 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/api/bot/models/bot_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.279439 swibots-1.2.0/swibots/api/chat/
+-rw-r--r--   0 root         (0) root         (0)      107 2023-01-16 06:01:20.000000 swibots-1.2.0/swibots/api/chat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5372 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/chat_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.296010 swibots-1.2.0/swibots/api/chat/controllers/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-01-15 12:53:45.000000 swibots-1.2.0/swibots/api/chat/controllers/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    21518 2023-02-08 08:21:26.000000 swibots-1.2.0/swibots/api/chat/controllers/message_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.338514 swibots-1.2.0/swibots/api/chat/events/
+-rwxr-xr-x   0 root         (0) root         (0)      326 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/events/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2073 2023-02-06 20:56:35.000000 swibots-1.2.0/swibots/api/chat/events/callback_query_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     2731 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/events/chat_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     2095 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/events/command_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     2103 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/events/inline_query_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     2434 2023-02-06 21:23:12.000000 swibots-1.2.0/swibots/api/chat/events/message_event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.505224 swibots-1.2.0/swibots/api/chat/methods/
+-rwxr-xr-x   0 root         (0) root         (0)     1709 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/methods/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      654 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/methods/answer_inline_query.py
+-rwxr-xr-x   0 root         (0) root         (0)      693 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/api/chat/methods/clear_conversation.py
+-rwxr-xr-x   0 root         (0) root         (0)      705 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/chat/methods/delete_message.py
+-rwxr-xr-x   0 root         (0) root         (0)      707 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/chat/methods/delete_messages_from_user.py
+-rwxr-xr-x   0 root         (0) root         (0)     1358 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/methods/download_media.py
+-rwxr-xr-x   0 root         (0) root         (0)      750 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/methods/edit_message.py
+-rwxr-xr-x   0 root         (0) root         (0)      853 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/methods/edit_message_text.py
+-rwxr-xr-x   0 root         (0) root         (0)      693 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/chat/methods/flag_message.py
+-rwxr-xr-x   0 root         (0) root         (0)     1192 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/methods/forward_message.py
+-rwxr-xr-x   0 root         (0) root         (0)     1139 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/chat/methods/get_channel_chat_history.py
+-rwxr-xr-x   0 root         (0) root         (0)      725 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/api/chat/methods/get_community_media_files.py
+-rwxr-xr-x   0 root         (0) root         (0)      883 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/chat/methods/get_community_media_files_by_status.py
+-rwxr-xr-x   0 root         (0) root         (0)      636 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/api/chat/methods/get_flag_messages.py
+-rwxr-xr-x   0 root         (0) root         (0)     1090 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/chat/methods/get_group_chat_history.py
+-rwxr-xr-x   0 root         (0) root         (0)      649 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/chat/methods/get_message.py
+-rwxr-xr-x   0 root         (0) root         (0)      707 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/chat/methods/get_messages.py
+-rwxr-xr-x   0 root         (0) root         (0)     1102 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/chat/methods/get_messages_between_users.py
+-rwxr-xr-x   0 root         (0) root         (0)      560 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/methods/get_unread_messages_count.py
+-rwxr-xr-x   0 root         (0) root         (0)      785 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/chat/methods/get_user_media_files.py
+-rwxr-xr-x   0 root         (0) root         (0)      881 2023-02-08 08:22:32.000000 swibots-1.2.0/swibots/api/chat/methods/reply_message.py
+-rwxr-xr-x   0 root         (0) root         (0)     1032 2023-02-08 08:20:23.000000 swibots-1.2.0/swibots/api/chat/methods/reply_message_text.py
+-rwxr-xr-x   0 root         (0) root         (0)      849 2023-02-08 08:19:39.000000 swibots-1.2.0/swibots/api/chat/methods/send_message.py
+-rwxr-xr-x   0 root         (0) root         (0)     1136 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/methods/send_text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.548102 swibots-1.2.0/swibots/api/chat/models/
+-rw-r--r--   0 root         (0) root         (0)      305 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/models/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      920 2023-02-06 20:55:52.000000 swibots-1.2.0/swibots/api/chat/models/group_chat_history.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.616204 swibots-1.2.0/swibots/api/chat/models/inline/
+-rwxr-xr-x   0 root         (0) root         (0)      565 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/models/inline/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1371 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/models/inline/base_typed_inline_query_result.py
+-rwxr-xr-x   0 root         (0) root         (0)     2533 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/models/inline/inline_query.py
+-rwxr-xr-x   0 root         (0) root         (0)     1871 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/models/inline/inline_query_answer.py
+-rwxr-xr-x   0 root         (0) root         (0)      991 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/models/inline/inline_query_result.py
+-rwxr-xr-x   0 root         (0) root         (0)     1158 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/models/inline/inline_query_result_article.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/models/inline/inline_query_result_document.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/models/inline/inline_query_result_photo.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/models/inline/inline_query_result_video.py
+-rwxr-xr-x   0 root         (0) root         (0)      581 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/models/inline/input_message_content.py
+-rwxr-xr-x   0 root         (0) root         (0)      201 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/chat/models/inline/types.py
+-rwxr-xr-x   0 root         (0) root         (0)      886 2023-02-08 07:21:24.000000 swibots-1.2.0/swibots/api/chat/models/inline_keyboard_button.py
+-rwxr-xr-x   0 root         (0) root         (0)      170 2023-01-18 20:49:52.000000 swibots-1.2.0/swibots/api/chat/models/inline_keyboard_color.py
+-rwxr-xr-x   0 root         (0) root         (0)      146 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/chat/models/inline_keyboard_size.py
+-rwxr-xr-x   0 root         (0) root         (0)     2065 2023-02-08 07:22:42.000000 swibots-1.2.0/swibots/api/chat/models/inline_markup.py
+-rw-r--r--   0 root         (0) root         (0)    10769 2023-02-08 09:10:55.000000 swibots-1.2.0/swibots/api/chat/models/message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.623780 swibots-1.2.0/swibots/api/common/
+-rwxr-xr-x   0 root         (0) root         (0)       44 2023-01-16 06:01:00.000000 swibots-1.2.0/swibots/api/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.634432 swibots-1.2.0/swibots/api/common/events/
+-rwxr-xr-x   0 root         (0) root         (0)       46 2023-01-13 06:20:04.000000 swibots-1.2.0/swibots/api/common/events/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2789 2023-01-23 19:39:48.000000 swibots-1.2.0/swibots/api/common/events/event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.656408 swibots-1.2.0/swibots/api/common/models/
+-rwxr-xr-x   0 root         (0) root         (0)      101 2023-02-06 20:55:52.000000 swibots-1.2.0/swibots/api/common/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-02-07 07:11:30.000000 swibots-1.2.0/swibots/api/common/models/media.py
+-rwxr-xr-x   0 root         (0) root         (0)     1565 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/common/models/media_upload_request.py
+-rwxr-xr-x   0 root         (0) root         (0)     1706 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/common/models/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.667875 swibots-1.2.0/swibots/api/community/
+-rwxr-xr-x   0 root         (0) root         (0)       90 2023-01-16 06:00:40.000000 swibots-1.2.0/swibots/api/community/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5059 2023-03-20 17:15:06.000000 swibots-1.2.0/swibots/api/community/community_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.692242 swibots-1.2.0/swibots/api/community/controllers/
+-rw-r--r--   0 root         (0) root         (0)      102 2023-02-06 20:55:52.000000 swibots-1.2.0/swibots/api/community/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      595 2023-02-06 20:55:52.000000 swibots-1.2.0/swibots/api/community/controllers/channel_controller.py
+-rwxr-xr-x   0 root         (0) root         (0)      616 2023-02-06 20:55:52.000000 swibots-1.2.0/swibots/api/community/controllers/community_controller.py
+-rw-r--r--   0 root         (0) root         (0)      576 2023-02-06 20:55:52.000000 swibots-1.2.0/swibots/api/community/controllers/group_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.816542 swibots-1.2.0/swibots/api/community/events/
+-rwxr-xr-x   0 root         (0) root         (0)      566 2023-01-16 23:20:36.000000 swibots-1.2.0/swibots/api/community/events/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1387 2023-03-20 17:12:26.000000 swibots-1.2.0/swibots/api/community/events/channel_created_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1387 2023-03-20 17:12:56.000000 swibots-1.2.0/swibots/api/community/events/channel_deleted_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1387 2023-03-20 17:12:44.000000 swibots-1.2.0/swibots/api/community/events/channel_updated_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     2303 2023-01-23 19:25:02.000000 swibots-1.2.0/swibots/api/community/events/community_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1383 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/community/events/community_updated_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1381 2023-03-20 17:13:37.000000 swibots-1.2.0/swibots/api/community/events/group_created_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1381 2023-03-20 17:14:02.000000 swibots-1.2.0/swibots/api/community/events/group_deleted_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1381 2023-03-20 17:13:49.000000 swibots-1.2.0/swibots/api/community/events/group_updated_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1380 2023-03-20 17:14:48.000000 swibots-1.2.0/swibots/api/community/events/member_joined_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1377 2023-03-20 17:15:06.000000 swibots-1.2.0/swibots/api/community/events/member_left_event.py
+-rwxr-xr-x   0 root         (0) root         (0)     1373 2023-03-20 17:14:14.000000 swibots-1.2.0/swibots/api/community/events/user_banned_event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.866744 swibots-1.2.0/swibots/api/community/methods/
+-rwxr-xr-x   0 root         (0) root         (0)      194 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/community/methods/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      643 2023-02-06 20:55:52.000000 swibots-1.2.0/swibots/api/community/methods/get_channel.py
+-rwxr-xr-x   0 root         (0) root         (0)      668 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/api/community/methods/get_community.py
+-rw-r--r--   0 root         (0) root         (0)      619 2023-02-06 20:55:52.000000 swibots-1.2.0/swibots/api/community/methods/get_group.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.914798 swibots-1.2.0/swibots/api/community/models/
+-rwxr-xr-x   0 root         (0) root         (0)      132 2023-01-13 05:39:45.000000 swibots-1.2.0/swibots/api/community/models/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2743 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/api/community/models/channel.py
+-rwxr-xr-x   0 root         (0) root         (0)     2954 2023-01-21 07:06:56.000000 swibots-1.2.0/swibots/api/community/models/community.py
+-rwxr-xr-x   0 root         (0) root         (0)     2720 2023-01-21 07:07:04.000000 swibots-1.2.0/swibots/api/community/models/group.py
+-rwxr-xr-x   0 root         (0) root         (0)     9347 2023-04-17 03:16:12.000000 swibots-1.2.0/swibots/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.980568 swibots-1.2.0/swibots/base/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-01-16 05:59:47.000000 swibots-1.2.0/swibots/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       69 2023-01-09 05:33:14.000000 swibots-1.2.0/swibots/base/rest_controller.py
+-rw-r--r--   0 root         (0) root         (0)      370 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/base/rest_request.py
+-rw-r--r--   0 root         (0) root         (0)      644 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/base/rest_response.py
+-rw-r--r--   0 root         (0) root         (0)     4261 2023-02-06 20:55:52.000000 swibots-1.2.0/swibots/base/switch_client.py
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-01-21 06:58:45.000000 swibots-1.2.0/swibots/base/switch_object.py
+-rwxr-xr-x   0 root         (0) root         (0)      543 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/base/switch_ws_async_client.py
+-rwxr-xr-x   0 root         (0) root         (0)     4329 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/bot_app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:53.018929 swibots-1.2.0/swibots/bots/
+-rwxr-xr-x   0 root         (0) root         (0)      201 2023-01-17 03:43:24.000000 swibots-1.2.0/swibots/bots/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4646 2023-04-20 23:47:00.000000 swibots-1.2.0/swibots/bots/bot.py
+-rwxr-xr-x   0 root         (0) root         (0)     1646 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/bots/bot_context.py
+-rwxr-xr-x   0 root         (0) root         (0)      109 2023-01-14 17:55:20.000000 swibots-1.2.0/swibots/bots/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:53.136066 swibots-1.2.0/swibots/bots/decorators/
+-rwxr-xr-x   0 root         (0) root         (0)      999 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/bots/decorators/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      540 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/bots/decorators/on_callback_query.py
+-rwxr-xr-x   0 root         (0) root         (0)      510 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/bots/decorators/on_channel_created.py
+-rwxr-xr-x   0 root         (0) root         (0)      544 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/bots/decorators/on_channel_deleted.py
+-rwxr-xr-x   0 root         (0) root         (0)      541 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/bots/decorators/on_channel_updated.py
+-rwxr-xr-x   0 root         (0) root         (0)      574 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/bots/decorators/on_command.py
+-rwxr-xr-x   0 root         (0) root         (0)      544 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/bots/decorators/on_community_updated.py
+-rwxr-xr-x   0 root         (0) root         (0)      536 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/bots/decorators/on_group_created.py
+-rwxr-xr-x   0 root         (0) root         (0)      536 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/bots/decorators/on_group_deleted.py
+-rwxr-xr-x   0 root         (0) root         (0)      534 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/bots/decorators/on_group_updated.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/bots/decorators/on_inline_query.py
+-rwxr-xr-x   0 root         (0) root         (0)      534 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/bots/decorators/on_member_joined.py
+-rwxr-xr-x   0 root         (0) root         (0)      529 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/bots/decorators/on_member_left.py
+-rwxr-xr-x   0 root         (0) root         (0)      503 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/bots/decorators/on_message.py
+-rwxr-xr-x   0 root         (0) root         (0)      543 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/bots/decorators/on_unknown_command.py
+-rwxr-xr-x   0 root         (0) root         (0)      509 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/bots/decorators/on_user_banned.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:53.146654 swibots-1.2.0/swibots/bots/filters/
+-rwxr-xr-x   0 root         (0) root         (0)       22 2023-01-16 03:25:36.000000 swibots-1.2.0/swibots/bots/filters/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7785 2023-04-21 00:39:37.000000 swibots-1.2.0/swibots/bots/filters/filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:53.284005 swibots-1.2.0/swibots/bots/handlers/
+-rwxr-xr-x   0 root         (0) root         (0)     1300 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/bots/handlers/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1048 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/bots/handlers/base_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      985 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/bots/handlers/callback_query_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      681 2023-03-20 17:12:26.000000 swibots-1.2.0/swibots/bots/handlers/channel_created_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      688 2023-03-20 17:12:57.000000 swibots-1.2.0/swibots/bots/handlers/channel_deleted_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      734 2023-03-20 17:12:44.000000 swibots-1.2.0/swibots/bots/handlers/channel_updated_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)     1514 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/bots/handlers/command_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      686 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/bots/handlers/community_updated_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)     1325 2023-04-21 00:21:17.000000 swibots-1.2.0/swibots/bots/handlers/event_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      680 2023-03-20 17:13:37.000000 swibots-1.2.0/swibots/bots/handlers/group_created_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      775 2023-03-20 17:14:02.000000 swibots-1.2.0/swibots/bots/handlers/group_deleted_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      775 2023-03-20 17:13:49.000000 swibots-1.2.0/swibots/bots/handlers/group_updated_handler.py
+-rw-r--r--   0 root         (0) root         (0)      867 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/bots/handlers/inline_query_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      679 2023-03-20 17:14:48.000000 swibots-1.2.0/swibots/bots/handlers/member_joined_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      674 2023-03-20 17:15:07.000000 swibots-1.2.0/swibots/bots/handlers/member_left_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      960 2023-02-04 19:02:01.000000 swibots-1.2.0/swibots/bots/handlers/message_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      885 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/bots/handlers/unknown_command_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      670 2023-03-20 17:14:14.000000 swibots-1.2.0/swibots/bots/handlers/user_banned_handler.py
+-rwxr-xr-x   0 root         (0) root         (0)      285 2023-01-23 21:16:29.000000 swibots-1.2.0/swibots/bots/register_command.py
+-rwxr-xr-x   0 root         (0) root         (0)     1621 2023-05-23 03:35:50.000000 swibots-1.2.0/swibots/config.py
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/error.py
+-rwxr-xr-x   0 root         (0) root         (0)      854 2023-03-20 17:15:29.000000 swibots-1.2.0/swibots/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:53.303750 swibots-1.2.0/swibots/utils/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-01-16 05:53:47.000000 swibots-1.2.0/swibots/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5880 2023-04-20 23:47:11.000000 swibots-1.2.0/swibots/utils/rest_client.py
+-rw-r--r--   0 root         (0) root         (0)     2475 2023-02-04 19:02:18.000000 swibots-1.2.0/swibots/utils/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:53.311462 swibots-1.2.0/swibots/utils/ws/
+-rw-r--r--   0 root         (0) root         (0)       48 2023-01-19 05:23:27.000000 swibots-1.2.0/swibots/utils/ws/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:53.335318 swibots-1.2.0/swibots/utils/ws/asyncstomp/
+-rw-r--r--   0 root         (0) root         (0)      150 2023-01-09 05:33:14.000000 swibots-1.2.0/swibots/utils/ws/asyncstomp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9743 2023-01-21 06:34:39.000000 swibots-1.2.0/swibots/utils/ws/asyncstomp/async_ws_client.py
+-rw-r--r--   0 root         (0) root         (0)      980 2023-01-19 01:21:52.000000 swibots-1.2.0/swibots/utils/ws/asyncstomp/async_ws_subscription.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:53.356755 swibots-1.2.0/swibots/utils/ws/common/
+-rw-r--r--   0 root         (0) root         (0)      100 2023-01-09 05:33:14.000000 swibots-1.2.0/swibots/utils/ws/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-01-09 05:33:14.000000 swibots-1.2.0/swibots/utils/ws/common/ws_frame.py
+-rw-r--r--   0 root         (0) root         (0)      430 2023-01-09 05:33:14.000000 swibots-1.2.0/swibots/utils/ws/common/ws_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:52.112336 swibots-1.2.0/swibots.egg-info/
+-rwxr-xr-x   0 root         (0) root         (0)     1817 2023-05-23 03:39:51.000000 swibots-1.2.0/swibots.egg-info/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     7316 2023-05-23 03:39:51.000000 swibots-1.2.0/swibots.egg-info/SOURCES.txt
+-rwxr-xr-x   0 root         (0) root         (0)        1 2023-05-23 03:39:51.000000 swibots-1.2.0/swibots.egg-info/dependency_links.txt
+-rwxr-xr-x   0 root         (0) root         (0)       31 2023-05-23 03:39:51.000000 swibots-1.2.0/swibots.egg-info/requires.txt
+-rwxr-xr-x   0 root         (0) root         (0)       14 2023-05-23 03:39:51.000000 swibots-1.2.0/swibots.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 03:39:53.374575 swibots-1.2.0/tests/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 05:56:05.000000 swibots-1.2.0/tests/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      202 2023-01-15 22:26:25.000000 swibots-1.2.0/tests/tests.py
```

### Comparing `swibots-1.1.9/README.md` & `swibots-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/setup.py` & `swibots-1.2.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from setuptools import setup, find_packages
-
-with open("requirements.txt", encoding="utf-8") as r:
-    requires = [i.strip() for i in r]
-
-try:
-    import pypandoc
-
-    long_description = pypandoc.convert_file("README.md", "rst")
-except (IOError, ImportError):
-    long_description = open("README.md").read()
-
-
-setup(
-    name="swibots",
-    version="1.1.9",
-    packages=find_packages(),
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/switchcollab/Switch-Bots-Python-Library",
-    description="Switch bot api",
-    author="switchadmin",
-    author_email="support@switch.pe",
-    license="LGPLv3",
-    python_requires=">=3.10",
-    install_requires=requires,
-)
+from setuptools import setup, find_packages
+
+with open("requirements.txt", encoding="utf-8") as r:
+    requires = [i.strip() for i in r]
+
+try:
+    import pypandoc
+
+    long_description = pypandoc.convert_file("README.md", "rst")
+except (IOError, ImportError):
+    long_description = open("README.md").read()
+
+
+setup(
+    name="swibots",
+    version="1.2.0",
+    packages=find_packages(),
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/switchcollab/Switch-Bots-Python-Library",
+    description="Switch bot api",
+    author="switchadmin",
+    author_email="support@switch.pe",
+    license="LGPLv3",
+    python_requires=">=3.10",
+    install_requires=requires,
+)
```

### Comparing `swibots-1.1.9/swibots/api/api_client.py` & `swibots-1.2.0/swibots/api/api_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/auth/auth_client.py` & `swibots-1.2.0/swibots/api/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/auth/controllers/user_controller.py` & `swibots-1.2.0/swibots/api/auth/controllers/user_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/auth/methods/get_me.py` & `swibots-1.2.0/swibots/api/auth/methods/get_me.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/auth/methods/login.py` & `swibots-1.2.0/swibots/api/auth/methods/login.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/auth/models/auth_user.py` & `swibots-1.2.0/swibots/api/auth/models/auth_user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/bot/bot_client.py` & `swibots-1.2.0/swibots/api/bot/bot_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/bot/controllers/bot_controller.py` & `swibots-1.2.0/swibots/api/bot/controllers/bot_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/bot/methods/delete_bot_info.py` & `swibots-1.2.0/swibots/api/bot/methods/delete_bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/bot/methods/get_bot_info.py` & `swibots-1.2.0/swibots/api/bot/methods/get_bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/bot/methods/update_bot_info.py` & `swibots-1.2.0/swibots/api/bot/methods/update_bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/bot/models/bot_command_info.py` & `swibots-1.2.0/swibots/api/bot/models/bot_command_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/bot/models/bot_info.py` & `swibots-1.2.0/swibots/api/bot/models/bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/chat_client.py` & `swibots-1.2.0/swibots/api/chat/chat_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/controllers/message_controller.py` & `swibots-1.2.0/swibots/api/chat/controllers/message_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/events/callback_query_event.py` & `swibots-1.2.0/swibots/api/chat/events/callback_query_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/events/chat_event.py` & `swibots-1.2.0/swibots/api/chat/events/chat_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/events/command_event.py` & `swibots-1.2.0/swibots/api/chat/events/command_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/events/inline_query_event.py` & `swibots-1.2.0/swibots/api/chat/events/inline_query_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/events/message_event.py` & `swibots-1.2.0/swibots/api/chat/events/message_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/methods/__init__.py` & `swibots-1.2.0/swibots/api/chat/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/methods/answer_inline_query.py` & `swibots-1.2.0/swibots/api/chat/methods/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/methods/clear_conversation.py` & `swibots-1.2.0/swibots/api/chat/methods/clear_conversation.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/methods/delete_message.py` & `swibots-1.2.0/swibots/api/chat/methods/delete_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/methods/delete_messages_from_user.py` & `swibots-1.2.0/swibots/api/chat/methods/delete_messages_from_user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/methods/download_media.py` & `swibots-1.2.0/swibots/api/chat/methods/download_media.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/methods/edit_message.py` & `swibots-1.2.0/swibots/api/chat/methods/edit_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/methods/edit_message_text.py` & `swibots-1.2.0/swibots/api/chat/methods/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/methods/flag_message.py` & `swibots-1.2.0/swibots/api/chat/methods/flag_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/methods/forward_message.py` & `swibots-1.2.0/swibots/api/chat/methods/forward_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/methods/get_channel_chat_history.py` & `swibots-1.2.0/swibots/api/chat/methods/get_channel_chat_history.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/methods/get_community_media_files.py` & `swibots-1.2.0/swibots/api/chat/methods/get_community_media_files.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/methods/get_community_media_files_by_status.py` & `swibots-1.2.0/swibots/api/chat/methods/get_community_media_files_by_status.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/methods/get_flag_messages.py` & `swibots-1.2.0/swibots/api/chat/methods/get_flag_messages.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/methods/get_group_chat_history.py` & `swibots-1.2.0/swibots/api/chat/methods/get_group_chat_history.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/methods/get_message.py` & `swibots-1.2.0/swibots/api/chat/methods/get_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/methods/get_messages.py` & `swibots-1.2.0/swibots/api/chat/methods/get_messages.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/methods/get_messages_between_users.py` & `swibots-1.2.0/swibots/api/chat/methods/get_messages_between_users.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/methods/get_unread_messages_count.py` & `swibots-1.2.0/swibots/api/chat/methods/get_unread_messages_count.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/methods/get_user_media_files.py` & `swibots-1.2.0/swibots/api/chat/methods/get_user_media_files.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/methods/reply_message.py` & `swibots-1.2.0/swibots/api/chat/methods/reply_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/methods/reply_message_text.py` & `swibots-1.2.0/swibots/api/chat/methods/reply_message_text.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/methods/send_message.py` & `swibots-1.2.0/swibots/api/chat/methods/send_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/methods/send_text.py` & `swibots-1.2.0/swibots/api/chat/methods/send_text.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/models/group_chat_history.py` & `swibots-1.2.0/swibots/api/chat/models/group_chat_history.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/models/inline/__init__.py` & `swibots-1.2.0/swibots/api/chat/models/inline/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/models/inline/base_typed_inline_query_result.py` & `swibots-1.2.0/swibots/api/chat/models/inline/base_typed_inline_query_result.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/models/inline/inline_query.py` & `swibots-1.2.0/swibots/api/chat/models/inline/inline_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/models/inline/inline_query_answer.py` & `swibots-1.2.0/swibots/api/chat/models/inline/inline_query_answer.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/models/inline/inline_query_result.py` & `swibots-1.2.0/swibots/api/chat/models/inline/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/models/inline/inline_query_result_article.py` & `swibots-1.2.0/swibots/api/chat/models/inline/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/models/inline/inline_query_result_document.py` & `swibots-1.2.0/swibots/api/chat/models/inline/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/models/inline/inline_query_result_photo.py` & `swibots-1.2.0/swibots/api/chat/models/inline/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/models/inline/inline_query_result_video.py` & `swibots-1.2.0/swibots/api/chat/models/inline/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/models/inline/input_message_content.py` & `swibots-1.2.0/swibots/api/chat/models/inline/input_message_content.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/models/inline_keyboard_button.py` & `swibots-1.2.0/swibots/api/chat/models/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/models/inline_markup.py` & `swibots-1.2.0/swibots/api/chat/models/inline_markup.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/chat/models/message.py` & `swibots-1.2.0/swibots/api/chat/models/message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/common/events/event.py` & `swibots-1.2.0/swibots/api/common/events/event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/common/models/media.py` & `swibots-1.2.0/swibots/api/common/models/media.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/common/models/media_upload_request.py` & `swibots-1.2.0/swibots/api/common/models/media_upload_request.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/common/models/user.py` & `swibots-1.2.0/swibots/api/common/models/user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/community/community_client.py` & `swibots-1.2.0/swibots/api/community/community_client.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-import json
-from swibots.api.auth.models.auth_user import AuthUser
-from swibots.api.community.events import *
-from swibots.base import SwitchRestClient, SwitchWSAsyncClient
-from swibots.config import get_config
-from swibots.error import SwitchError
-from swibots.utils.ws.asyncstomp.async_ws_subscription import AsyncWsSubscription
-from swibots.utils.ws.common.ws_message import WsMessage
-from swibots.types import EventType
-from .controllers import ChannelController, GroupController, CommunityController
-import swibots
-
-
-class CommunityClient(SwitchRestClient):
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        base_url: str = None,
-        ws_url: str = None,
-    ):
-        base_url = base_url or get_config()["COMMUNITY_SERVICE"]["BASE_URL"]
-        self._ws_url = ws_url or get_config()["COMMUNITY_SERVICE"]["WS_URL"]
-        super().__init__(app, base_url)
-        self._channels = None
-        self._groups = None
-        self._communities = None
-        self._ws: SwitchWSAsyncClient = None
-        self._started = False
-
-    @property
-    def channels(self) -> ChannelController:
-        """Get the channels controller"""
-        if self._channels is None:
-            self._channels = ChannelController(self)
-        return self._channels
-
-    @property
-    def groups(self) -> GroupController:
-        """Get the channels controller"""
-        if self._groups is None:
-            self._groups = GroupController(self)
-        return self._groups
-
-    @property
-    def communities(self) -> CommunityController:
-        """Get the channels controller"""
-        if self._communities is None:
-            self._communities = CommunityController(self)
-        return self._communities
-
-    @property
-    def ws(self) -> SwitchWSAsyncClient:
-        if self._ws is None:
-            self._ws = SwitchWSAsyncClient(self._ws_url, self.token)
-        return self._ws
-
-    @property
-    async def subscribe(self, endpoint: str, callback=None) -> AsyncWsSubscription:
-        if self.user is None:
-            raise SwitchError("User is not set")
-        if callback is None:
-            raise SwitchError("Callback is not set")
-        return await self.ws.subscribe(endpoint, callback=callback)
-
-    async def subscribe_to_notifications(self, callback=None) -> AsyncWsSubscription:
-        subscription = await self.ws.subscribe(
-            "/user/queue/events",
-            callback=lambda event: callback(self._parse_event(event)),
-        )
-        return subscription
-
-    def _parse_event(self, raw_message: WsMessage) -> CommunityEvent:
-        json_data = json.loads(raw_message.body)
-        type = json_data.get("type", "COMMUNITY")
-        evt = None
-        if type == EventType.COMMUNITY_CHANNEL_CREATE.value:
-            evt = self.build_object(ChannelCreatedEvent, json_data)
-            # return ChannelCreatedEvent.build_from_json(json_data)
-        elif type == EventType.COMMUNITY_CHANNEL_UPDATE.value:
-            evt = self.build_object(ChannelUpdatedEvent, json_data)
-            # return ChannelUpdatedEvent.build_from_json(json_data)
-        elif type == EventType.COMMUNITY_CHANNEL_DELETE.value:
-            evt = self.build_object(ChannelDeletedEvent, json_data)
-            # return ChannelDeletedEvent.build_from_json(json_data)
-        elif type == EventType.COMMUNITY_UPDATE.value:
-            evt = self.build_object(CommunityUpdatedEvent, json_data)
-            # return CommunityUpdatedEvent.build_from_json(json_data)
-        elif type == EventType.COMMUNITY_GROUP_CREATE.value:
-            evt = self.build_object(GroupCreatedEvent, json_data)
-            # return GroupCreatedEvent.build_from_json(json_data)
-        elif type == EventType.COMMUNITY_GROUP_UPDATE.value:
-            evt = self.build_object(GroupUpdatedEvent, json_data)
-            # return GroupUpdatedEvent.build_from_json(json_data)
-        elif type == EventType.COMMUNITY_GROUP_DELETE.value:
-            evt = self.build_object(GroupDeletedEvent, json_data)
-            # return GroupDeletedEvent.build_from_json(json_data)
-        elif type == EventType.COMMUNITY_USER_BAN.value:
-            evt = self.build_object(UserBannedEvent, json_data)
-            # return UserBannedEvent.build_from_json(json_data)
-        elif type == EventType.COMMUNITY_MEMBER_JOIN.value:
-            evt = self.build_object(MemberJoinedEvent, json_data)
-            # return MemberJoinedEvent.build_from_json(json_data)
-        elif type == EventType.COMMUNITY_MEMBER_LEAVE.value:
-            evt = self.build_object(MemberLeftEvent, json_data)
-            # return MemberLeftEvent.build_from_json(json_data)
-        else:
-            evt = self.build_object(CommunityEvent, json_data)
-
-        return evt
-
-    async def start(self):
-        """Start the community client"""
-        if self.user is None:
-            raise SwitchError("User is not set")
-        await self.ws.connect()
-        self._started = True
-
-    async def stop(self):
-        if self._started:
-            await self.ws.disconnect()
-            self._started = False
+import json
+from swibots.api.auth.models.auth_user import AuthUser
+from swibots.api.community.events import *
+from swibots.base import SwitchRestClient, SwitchWSAsyncClient
+from swibots.config import get_config
+from swibots.error import SwitchError
+from swibots.utils.ws.asyncstomp.async_ws_subscription import AsyncWsSubscription
+from swibots.utils.ws.common.ws_message import WsMessage
+from swibots.types import EventType
+from .controllers import ChannelController, GroupController, CommunityController
+import swibots
+
+
+class CommunityClient(SwitchRestClient):
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        base_url: str = None,
+        ws_url: str = None,
+    ):
+        base_url = base_url or get_config()["COMMUNITY_SERVICE"]["BASE_URL"]
+        self._ws_url = ws_url or get_config()["COMMUNITY_SERVICE"]["WS_URL"]
+        super().__init__(app, base_url)
+        self._channels = None
+        self._groups = None
+        self._communities = None
+        self._ws: SwitchWSAsyncClient = None
+        self._started = False
+
+    @property
+    def channels(self) -> ChannelController:
+        """Get the channels controller"""
+        if self._channels is None:
+            self._channels = ChannelController(self)
+        return self._channels
+
+    @property
+    def groups(self) -> GroupController:
+        """Get the channels controller"""
+        if self._groups is None:
+            self._groups = GroupController(self)
+        return self._groups
+
+    @property
+    def communities(self) -> CommunityController:
+        """Get the channels controller"""
+        if self._communities is None:
+            self._communities = CommunityController(self)
+        return self._communities
+
+    @property
+    def ws(self) -> SwitchWSAsyncClient:
+        if self._ws is None:
+            self._ws = SwitchWSAsyncClient(self._ws_url, self.token)
+        return self._ws
+
+    @property
+    async def subscribe(self, endpoint: str, callback=None) -> AsyncWsSubscription:
+        if self.user is None:
+            raise SwitchError("User is not set")
+        if callback is None:
+            raise SwitchError("Callback is not set")
+        return await self.ws.subscribe(endpoint, callback=callback)
+
+    async def subscribe_to_notifications(self, callback=None) -> AsyncWsSubscription:
+        subscription = await self.ws.subscribe(
+            "/user/queue/events",
+            callback=lambda event: callback(self._parse_event(event)),
+        )
+        return subscription
+
+    def _parse_event(self, raw_message: WsMessage) -> CommunityEvent:
+        json_data = json.loads(raw_message.body)
+        type = json_data.get("type", "COMMUNITY")
+        evt = None
+        if type == EventType.COMMUNITY_CHANNEL_CREATE.value:
+            evt = self.build_object(ChannelCreatedEvent, json_data)
+            # return ChannelCreatedEvent.build_from_json(json_data)
+        elif type == EventType.COMMUNITY_CHANNEL_UPDATE.value:
+            evt = self.build_object(ChannelUpdatedEvent, json_data)
+            # return ChannelUpdatedEvent.build_from_json(json_data)
+        elif type == EventType.COMMUNITY_CHANNEL_DELETE.value:
+            evt = self.build_object(ChannelDeletedEvent, json_data)
+            # return ChannelDeletedEvent.build_from_json(json_data)
+        elif type == EventType.COMMUNITY_UPDATE.value:
+            evt = self.build_object(CommunityUpdatedEvent, json_data)
+            # return CommunityUpdatedEvent.build_from_json(json_data)
+        elif type == EventType.COMMUNITY_GROUP_CREATE.value:
+            evt = self.build_object(GroupCreatedEvent, json_data)
+            # return GroupCreatedEvent.build_from_json(json_data)
+        elif type == EventType.COMMUNITY_GROUP_UPDATE.value:
+            evt = self.build_object(GroupUpdatedEvent, json_data)
+            # return GroupUpdatedEvent.build_from_json(json_data)
+        elif type == EventType.COMMUNITY_GROUP_DELETE.value:
+            evt = self.build_object(GroupDeletedEvent, json_data)
+            # return GroupDeletedEvent.build_from_json(json_data)
+        elif type == EventType.COMMUNITY_USER_BAN.value:
+            evt = self.build_object(UserBannedEvent, json_data)
+            # return UserBannedEvent.build_from_json(json_data)
+        elif type == EventType.COMMUNITY_MEMBER_JOIN.value:
+            evt = self.build_object(MemberJoinedEvent, json_data)
+            # return MemberJoinedEvent.build_from_json(json_data)
+        elif type == EventType.COMMUNITY_MEMBER_LEAVE.value:
+            evt = self.build_object(MemberLeftEvent, json_data)
+            # return MemberLeftEvent.build_from_json(json_data)
+        else:
+            evt = self.build_object(CommunityEvent, json_data)
+
+        return evt
+
+    async def start(self):
+        """Start the community client"""
+        if self.user is None:
+            raise SwitchError("User is not set")
+        await self.ws.connect()
+        self._started = True
+
+    async def stop(self):
+        if self._started:
+            await self.ws.disconnect()
+            self._started = False
```

### Comparing `swibots-1.1.9/swibots/api/community/controllers/channel_controller.py` & `swibots-1.2.0/swibots/api/community/controllers/channel_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/community/controllers/community_controller.py` & `swibots-1.2.0/swibots/api/community/controllers/community_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/community/controllers/group_controller.py` & `swibots-1.2.0/swibots/api/community/controllers/group_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/community/events/__init__.py` & `swibots-1.2.0/swibots/api/community/events/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/community/events/channel_created_event.py` & `swibots-1.2.0/swibots/api/community/events/channel_created_event.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from typing import Optional
-import swibots
-from .community_event import CommunityEvent
-from swibots.api.community.models.channel import Channel
-from swibots.api.community.models.community import Community
-from swibots.api.community.models.group import Group
-from swibots.api.common.models.user import User
-from swibots.types import EventType
-
-
-class ChannelCreatedEvent(CommunityEvent["ChannelCreatedEvent"]):
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        community_id: Optional[str] = None,
-        community: Optional[Community] = None,
-        group_id: Optional[str] = None,
-        group: Optional[Group] = None,
-        channel_id: Optional[str] = None,
-        channel: Optional[Channel] = None,
-        action_by_id: Optional[str] = None,
-        action_by: Optional[User] = None,
-        data: Optional[dict] = None,
-        user_id: Optional[str] = None,
-        user: Optional[User] = None,
-    ):
-        super().__init__(
-            app=app,
-            type=EventType.COMMUNITY_CHANNEL_CREATE,
-            data=data,
-            action_by=action_by,
-            action_by_id=action_by_id,
-            community=community,
-            community_id=community_id,
-            group=group,
-            group_id=group_id,
-            channel=channel,
-            channel_id=channel_id,
-            user=user,
-            user_id=user_id,
-        )
+from typing import Optional
+import swibots
+from .community_event import CommunityEvent
+from swibots.api.community.models.channel import Channel
+from swibots.api.community.models.community import Community
+from swibots.api.community.models.group import Group
+from swibots.api.common.models.user import User
+from swibots.types import EventType
+
+
+class ChannelCreatedEvent(CommunityEvent["ChannelCreatedEvent"]):
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        community_id: Optional[str] = None,
+        community: Optional[Community] = None,
+        group_id: Optional[str] = None,
+        group: Optional[Group] = None,
+        channel_id: Optional[str] = None,
+        channel: Optional[Channel] = None,
+        action_by_id: Optional[str] = None,
+        action_by: Optional[User] = None,
+        data: Optional[dict] = None,
+        user_id: Optional[str] = None,
+        user: Optional[User] = None,
+    ):
+        super().__init__(
+            app=app,
+            type=EventType.COMMUNITY_CHANNEL_CREATE,
+            data=data,
+            action_by=action_by,
+            action_by_id=action_by_id,
+            community=community,
+            community_id=community_id,
+            group=group,
+            group_id=group_id,
+            channel=channel,
+            channel_id=channel_id,
+            user=user,
+            user_id=user_id,
+        )
```

### Comparing `swibots-1.1.9/swibots/api/community/events/channel_deleted_event.py` & `swibots-1.2.0/swibots/api/community/events/community_updated_event.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from typing import Optional
-import swibots
-from .community_event import CommunityEvent
-from swibots.api.community.models.channel import Channel
-from swibots.api.community.models.community import Community
-from swibots.api.community.models.group import Group
-from swibots.api.common.models.user import User
-from swibots.types import EventType
-
-
-class ChannelDeletedEvent(CommunityEvent["ChannelDeletedEvent"]):
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        community_id: Optional[str] = None,
-        community: Optional[Community] = None,
-        group_id: Optional[str] = None,
-        group: Optional[Group] = None,
-        channel_id: Optional[str] = None,
-        channel: Optional[Channel] = None,
-        action_by_id: Optional[str] = None,
-        action_by: Optional[User] = None,
-        data: Optional[dict] = None,
-        user_id: Optional[str] = None,
-        user: Optional[User] = None,
-    ):
-        super().__init__(
-            app=app,
-            type=EventType.COMMUNITY_CHANNEL_DELETE,
-            data=data,
-            action_by=action_by,
-            action_by_id=action_by_id,
-            community=community,
-            community_id=community_id,
-            group=group,
-            group_id=group_id,
-            channel=channel,
-            channel_id=channel_id,
-            user=user,
-            user_id=user_id,
-        )
+from typing import Optional
+import swibots
+from .community_event import CommunityEvent
+from swibots.api.community.models.channel import Channel
+from swibots.api.community.models.community import Community
+from swibots.api.community.models.group import Group
+from swibots.api.common.models.user import User
+from swibots.types import EventType
+
+
+class CommunityUpdatedEvent(CommunityEvent["CommunityUpdatedEvent"]):
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        community_id: Optional[str] = None,
+        community: Optional[Community] = None,
+        group_id: Optional[str] = None,
+        group: Optional[Group] = None,
+        channel_id: Optional[str] = None,
+        channel: Optional[Channel] = None,
+        action_by_id: Optional[str] = None,
+        action_by: Optional[User] = None,
+        data: Optional[dict] = None,
+        user_id: Optional[str] = None,
+        user: Optional[User] = None,
+    ):
+        super().__init__(
+            app=app,
+            type=EventType.COMMUNITY_UPDATE,
+            data=data,
+            action_by=action_by,
+            action_by_id=action_by_id,
+            community=community,
+            community_id=community_id,
+            group=group,
+            group_id=group_id,
+            channel=channel,
+            channel_id=channel_id,
+            user=user,
+            user_id=user_id,
+        )
```

### Comparing `swibots-1.1.9/swibots/api/community/events/channel_updated_event.py` & `swibots-1.2.0/swibots/api/community/events/member_left_event.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from typing import Optional
-import swibots
-from .community_event import CommunityEvent
-from swibots.api.community.models.channel import Channel
-from swibots.api.community.models.community import Community
-from swibots.api.community.models.group import Group
-from swibots.api.common.models.user import User
-from swibots.types import EventType
-
-
-class ChannelUpdatedEvent(CommunityEvent["ChannelUpdatedEvent"]):
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        community_id: Optional[str] = None,
-        community: Optional[Community] = None,
-        group_id: Optional[str] = None,
-        group: Optional[Group] = None,
-        channel_id: Optional[str] = None,
-        channel: Optional[Channel] = None,
-        action_by_id: Optional[str] = None,
-        action_by: Optional[User] = None,
-        data: Optional[dict] = None,
-        user_id: Optional[str] = None,
-        user: Optional[User] = None,
-    ):
-        super().__init__(
-            app=app,
-            type=EventType.COMMUNITY_CHANNEL_UPDATE,
-            data=data,
-            action_by=action_by,
-            action_by_id=action_by_id,
-            community=community,
-            community_id=community_id,
-            group=group,
-            group_id=group_id,
-            channel=channel,
-            channel_id=channel_id,
-            user=user,
-            user_id=user_id,
-        )
+from typing import Optional
+import swibots
+from .community_event import CommunityEvent
+from swibots.api.community.models.channel import Channel
+from swibots.api.community.models.community import Community
+from swibots.api.community.models.group import Group
+from swibots.api.common.models.user import User
+from swibots.types import EventType
+
+
+class MemberLeftEvent(CommunityEvent["MemberLeftEvent"]):
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        community_id: Optional[str] = None,
+        community: Optional[Community] = None,
+        group_id: Optional[str] = None,
+        group: Optional[Group] = None,
+        channel_id: Optional[str] = None,
+        channel: Optional[Channel] = None,
+        action_by_id: Optional[str] = None,
+        action_by: Optional[User] = None,
+        data: Optional[dict] = None,
+        user_id: Optional[str] = None,
+        user: Optional[User] = None,
+    ):
+        super().__init__(
+            app=app,
+            type=EventType.COMMUNITY_MEMBER_LEAVE,
+            data=data,
+            action_by=action_by,
+            action_by_id=action_by_id,
+            community=community,
+            community_id=community_id,
+            group=group,
+            group_id=group_id,
+            channel=channel,
+            channel_id=channel_id,
+            user=user,
+            user_id=user_id,
+        )
```

### Comparing `swibots-1.1.9/swibots/api/community/events/community_event.py` & `swibots-1.2.0/swibots/api/community/events/community_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/community/events/community_updated_event.py` & `swibots-1.2.0/swibots/api/community/events/channel_updated_event.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from swibots.api.community.models.channel import Channel
 from swibots.api.community.models.community import Community
 from swibots.api.community.models.group import Group
 from swibots.api.common.models.user import User
 from swibots.types import EventType
 
 
-class CommunityUpdatedEvent(CommunityEvent["CommunityUpdatedEvent"]):
+class ChannelUpdatedEvent(CommunityEvent["ChannelUpdatedEvent"]):
     def __init__(
         self,
         app: "swibots.App" = None,
         community_id: Optional[str] = None,
         community: Optional[Community] = None,
         group_id: Optional[str] = None,
         group: Optional[Group] = None,
@@ -22,15 +22,15 @@
         action_by: Optional[User] = None,
         data: Optional[dict] = None,
         user_id: Optional[str] = None,
         user: Optional[User] = None,
     ):
         super().__init__(
             app=app,
-            type=EventType.COMMUNITY_UPDATE,
+            type=EventType.COMMUNITY_CHANNEL_UPDATE,
             data=data,
             action_by=action_by,
             action_by_id=action_by_id,
             community=community,
             community_id=community_id,
             group=group,
             group_id=group_id,
```

### Comparing `swibots-1.1.9/swibots/api/community/events/group_deleted_event.py` & `swibots-1.2.0/swibots/api/community/events/group_created_event.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from typing import Optional
-import swibots
-from .community_event import CommunityEvent
-from swibots.api.community.models.channel import Channel
-from swibots.api.community.models.community import Community
-from swibots.api.community.models.group import Group
-from swibots.api.common.models.user import User
-from swibots.types import EventType
-
-
-class GroupDeletedEvent(CommunityEvent["GroupDeletedEvent"]):
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        community_id: Optional[str] = None,
-        community: Optional[Community] = None,
-        group_id: Optional[str] = None,
-        group: Optional[Group] = None,
-        channel_id: Optional[str] = None,
-        channel: Optional[Channel] = None,
-        action_by_id: Optional[str] = None,
-        action_by: Optional[User] = None,
-        data: Optional[dict] = None,
-        user_id: Optional[str] = None,
-        user: Optional[User] = None,
-    ):
-        super().__init__(
-            app=app,
-            type=EventType.COMMUNITY_GROUP_DELETE,
-            data=data,
-            action_by=action_by,
-            action_by_id=action_by_id,
-            community=community,
-            community_id=community_id,
-            group=group,
-            group_id=group_id,
-            channel=channel,
-            channel_id=channel_id,
-            user=user,
-            user_id=user_id,
-        )
+from typing import Optional
+import swibots
+from .community_event import CommunityEvent
+from swibots.api.community.models.channel import Channel
+from swibots.api.community.models.community import Community
+from swibots.api.community.models.group import Group
+from swibots.api.common.models.user import User
+from swibots.types import EventType
+
+
+class GroupCreatedEvent(CommunityEvent["GroupCreatedEvent"]):
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        community_id: Optional[str] = None,
+        community: Optional[Community] = None,
+        group_id: Optional[str] = None,
+        group: Optional[Group] = None,
+        channel_id: Optional[str] = None,
+        channel: Optional[Channel] = None,
+        action_by_id: Optional[str] = None,
+        action_by: Optional[User] = None,
+        data: Optional[dict] = None,
+        user_id: Optional[str] = None,
+        user: Optional[User] = None,
+    ):
+        super().__init__(
+            app=app,
+            type=EventType.COMMUNITY_GROUP_CREATE,
+            data=data,
+            action_by=action_by,
+            action_by_id=action_by_id,
+            community=community,
+            community_id=community_id,
+            group=group,
+            group_id=group_id,
+            channel=channel,
+            channel_id=channel_id,
+            user=user,
+            user_id=user_id,
+        )
```

### Comparing `swibots-1.1.9/swibots/api/community/events/group_updated_event.py` & `swibots-1.2.0/swibots/api/community/events/group_updated_event.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from typing import Optional
-import swibots
-from .community_event import CommunityEvent
-from swibots.api.community.models.channel import Channel
-from swibots.api.community.models.community import Community
-from swibots.api.community.models.group import Group
-from swibots.api.common.models.user import User
-from swibots.types import EventType
-
-
-class GroupUpdatedEvent(CommunityEvent["GroupUpdatedEvent"]):
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        community_id: Optional[str] = None,
-        community: Optional[Community] = None,
-        group_id: Optional[str] = None,
-        group: Optional[Group] = None,
-        channel_id: Optional[str] = None,
-        channel: Optional[Channel] = None,
-        action_by_id: Optional[str] = None,
-        action_by: Optional[User] = None,
-        data: Optional[dict] = None,
-        user_id: Optional[str] = None,
-        user: Optional[User] = None,
-    ):
-        super().__init__(
-            app=app,
-            type=EventType.COMMUNITY_GROUP_UPDATE,
-            data=data,
-            action_by=action_by,
-            action_by_id=action_by_id,
-            community=community,
-            community_id=community_id,
-            group=group,
-            group_id=group_id,
-            channel=channel,
-            channel_id=channel_id,
-            user=user,
-            user_id=user_id,
-        )
+from typing import Optional
+import swibots
+from .community_event import CommunityEvent
+from swibots.api.community.models.channel import Channel
+from swibots.api.community.models.community import Community
+from swibots.api.community.models.group import Group
+from swibots.api.common.models.user import User
+from swibots.types import EventType
+
+
+class GroupUpdatedEvent(CommunityEvent["GroupUpdatedEvent"]):
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        community_id: Optional[str] = None,
+        community: Optional[Community] = None,
+        group_id: Optional[str] = None,
+        group: Optional[Group] = None,
+        channel_id: Optional[str] = None,
+        channel: Optional[Channel] = None,
+        action_by_id: Optional[str] = None,
+        action_by: Optional[User] = None,
+        data: Optional[dict] = None,
+        user_id: Optional[str] = None,
+        user: Optional[User] = None,
+    ):
+        super().__init__(
+            app=app,
+            type=EventType.COMMUNITY_GROUP_UPDATE,
+            data=data,
+            action_by=action_by,
+            action_by_id=action_by_id,
+            community=community,
+            community_id=community_id,
+            group=group,
+            group_id=group_id,
+            channel=channel,
+            channel_id=channel_id,
+            user=user,
+            user_id=user_id,
+        )
```

### Comparing `swibots-1.1.9/swibots/api/community/events/member_joined_event.py` & `swibots-1.2.0/swibots/api/community/events/member_joined_event.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from typing import Optional
-import swibots
-from .community_event import CommunityEvent
-from swibots.api.community.models.channel import Channel
-from swibots.api.community.models.community import Community
-from swibots.api.community.models.group import Group
-from swibots.api.common.models.user import User
-from swibots.types import EventType
-
-
-class MemberJoinedEvent(CommunityEvent["MemberJoinedEvent"]):
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        community_id: Optional[str] = None,
-        community: Optional[Community] = None,
-        group_id: Optional[str] = None,
-        group: Optional[Group] = None,
-        channel_id: Optional[str] = None,
-        channel: Optional[Channel] = None,
-        action_by_id: Optional[str] = None,
-        action_by: Optional[User] = None,
-        data: Optional[dict] = None,
-        user_id: Optional[str] = None,
-        user: Optional[User] = None,
-    ):
-        super().__init__(
-            app=app,
-            type=EventType.COMMUNITY_MEMBER_JOIN,
-            data=data,
-            action_by=action_by,
-            action_by_id=action_by_id,
-            community=community,
-            community_id=community_id,
-            group=group,
-            group_id=group_id,
-            channel=channel,
-            channel_id=channel_id,
-            user=user,
-            user_id=user_id,
-        )
+from typing import Optional
+import swibots
+from .community_event import CommunityEvent
+from swibots.api.community.models.channel import Channel
+from swibots.api.community.models.community import Community
+from swibots.api.community.models.group import Group
+from swibots.api.common.models.user import User
+from swibots.types import EventType
+
+
+class MemberJoinedEvent(CommunityEvent["MemberJoinedEvent"]):
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        community_id: Optional[str] = None,
+        community: Optional[Community] = None,
+        group_id: Optional[str] = None,
+        group: Optional[Group] = None,
+        channel_id: Optional[str] = None,
+        channel: Optional[Channel] = None,
+        action_by_id: Optional[str] = None,
+        action_by: Optional[User] = None,
+        data: Optional[dict] = None,
+        user_id: Optional[str] = None,
+        user: Optional[User] = None,
+    ):
+        super().__init__(
+            app=app,
+            type=EventType.COMMUNITY_MEMBER_JOIN,
+            data=data,
+            action_by=action_by,
+            action_by_id=action_by_id,
+            community=community,
+            community_id=community_id,
+            group=group,
+            group_id=group_id,
+            channel=channel,
+            channel_id=channel_id,
+            user=user,
+            user_id=user_id,
+        )
```

### Comparing `swibots-1.1.9/swibots/api/community/events/user_banned_event.py` & `swibots-1.2.0/swibots/api/community/events/channel_deleted_event.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from typing import Optional
-import swibots
-from .community_event import CommunityEvent
-from swibots.api.community.models.channel import Channel
-from swibots.api.community.models.community import Community
-from swibots.api.community.models.group import Group
-from swibots.api.common.models.user import User
-from swibots.types import EventType
-
-
-class UserBannedEvent(CommunityEvent["UserBannedEvent"]):
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        community_id: Optional[str] = None,
-        community: Optional[Community] = None,
-        group_id: Optional[str] = None,
-        group: Optional[Group] = None,
-        channel_id: Optional[str] = None,
-        channel: Optional[Channel] = None,
-        action_by_id: Optional[str] = None,
-        action_by: Optional[User] = None,
-        data: Optional[dict] = None,
-        user_id: Optional[str] = None,
-        user: Optional[User] = None,
-    ):
-        super().__init__(
-            app=app,
-            type=EventType.COMMUNITY_USER_BAN,
-            data=data,
-            action_by=action_by,
-            action_by_id=action_by_id,
-            community=community,
-            community_id=community_id,
-            group=group,
-            group_id=group_id,
-            channel=channel,
-            channel_id=channel_id,
-            user=user,
-            user_id=user_id,
-        )
+from typing import Optional
+import swibots
+from .community_event import CommunityEvent
+from swibots.api.community.models.channel import Channel
+from swibots.api.community.models.community import Community
+from swibots.api.community.models.group import Group
+from swibots.api.common.models.user import User
+from swibots.types import EventType
+
+
+class ChannelDeletedEvent(CommunityEvent["ChannelDeletedEvent"]):
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        community_id: Optional[str] = None,
+        community: Optional[Community] = None,
+        group_id: Optional[str] = None,
+        group: Optional[Group] = None,
+        channel_id: Optional[str] = None,
+        channel: Optional[Channel] = None,
+        action_by_id: Optional[str] = None,
+        action_by: Optional[User] = None,
+        data: Optional[dict] = None,
+        user_id: Optional[str] = None,
+        user: Optional[User] = None,
+    ):
+        super().__init__(
+            app=app,
+            type=EventType.COMMUNITY_CHANNEL_DELETE,
+            data=data,
+            action_by=action_by,
+            action_by_id=action_by_id,
+            community=community,
+            community_id=community_id,
+            group=group,
+            group_id=group_id,
+            channel=channel,
+            channel_id=channel_id,
+            user=user,
+            user_id=user_id,
+        )
```

### Comparing `swibots-1.1.9/swibots/api/community/methods/get_channel.py` & `swibots-1.2.0/swibots/api/community/methods/get_channel.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/community/methods/get_community.py` & `swibots-1.2.0/swibots/api/community/methods/get_community.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/community/methods/get_group.py` & `swibots-1.2.0/swibots/api/community/methods/get_group.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/community/models/channel.py` & `swibots-1.2.0/swibots/api/community/models/channel.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/community/models/community.py` & `swibots-1.2.0/swibots/api/community/models/community.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/api/community/models/group.py` & `swibots-1.2.0/swibots/api/community/models/group.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/app.py` & `swibots-1.2.0/swibots/app.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/base/rest_response.py` & `swibots-1.2.0/swibots/base/rest_response.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/base/switch_client.py` & `swibots-1.2.0/swibots/base/switch_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/base/switch_object.py` & `swibots-1.2.0/swibots/base/switch_object.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/base/switch_ws_async_client.py` & `swibots-1.2.0/swibots/base/switch_ws_async_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bot_app.py` & `swibots-1.2.0/swibots/bot_app.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bots/bot.py` & `swibots-1.2.0/swibots/bots/bot.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bots/bot_context.py` & `swibots-1.2.0/swibots/bots/bot_context.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bots/decorators/__init__.py` & `swibots-1.2.0/swibots/bots/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bots/decorators/on_callback_query.py` & `swibots-1.2.0/swibots/bots/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bots/decorators/on_channel_deleted.py` & `swibots-1.2.0/swibots/bots/decorators/on_channel_deleted.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bots/decorators/on_channel_updated.py` & `swibots-1.2.0/swibots/bots/decorators/on_channel_updated.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bots/decorators/on_command.py` & `swibots-1.2.0/swibots/bots/decorators/on_command.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bots/decorators/on_community_updated.py` & `swibots-1.2.0/swibots/bots/decorators/on_community_updated.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bots/decorators/on_group_created.py` & `swibots-1.2.0/swibots/bots/decorators/on_group_created.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bots/decorators/on_group_deleted.py` & `swibots-1.2.0/swibots/bots/decorators/on_group_deleted.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bots/decorators/on_group_updated.py` & `swibots-1.2.0/swibots/bots/decorators/on_group_updated.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bots/decorators/on_inline_query.py` & `swibots-1.2.0/swibots/bots/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bots/decorators/on_member_joined.py` & `swibots-1.2.0/swibots/bots/decorators/on_member_joined.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bots/decorators/on_member_left.py` & `swibots-1.2.0/swibots/bots/decorators/on_member_left.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bots/decorators/on_unknown_command.py` & `swibots-1.2.0/swibots/bots/decorators/on_unknown_command.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bots/filters/filter.py` & `swibots-1.2.0/swibots/bots/filters/filter.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,272 +1,272 @@
-import re
-from typing import Optional
-from swibots.api.chat.events import MessageEvent
-from swibots.api.chat.events.chat_event import ChatEvent
-from swibots.api.common.events import Event
-from swibots.bots.bot_context import BotContext
-from swibots.utils.types import SCT, FilterCallback
-from swibots.types import EventType
-from typing import Callable, Union, List, Pattern
-
-
-class Filter:
-    async def __call__(self, ctx: BotContext) -> bool:
-        raise NotImplementedError
-
-    def __invert__(self):
-        return InvertFilter(self)
-
-    def __and__(self, other):
-        return AndFilter(self, other)
-
-    def __or__(self, other):
-        return OrFilter(self, other)
-
-
-class InvertFilter(Filter):
-    def __init__(self, base):
-        self.base = base
-
-    async def __call__(self, ctx: BotContext) -> bool:
-        result = await self.base(ctx)
-        return not result
-
-
-class AndFilter(Filter):
-    def __init__(self, base, other):
-        self.base = base
-        self.other = other
-
-    async def __call__(self, ctx: BotContext) -> bool:
-        r1 = await self.base(ctx)
-        # short circuit
-        if not r1:
-            return False
-        r2 = await self.other(ctx)
-
-        return r1 and r2
-
-
-class OrFilter(Filter):
-    def __init__(self, base, other):
-        self.base = base
-        self.other = other
-
-    async def __call__(self, ctx: BotContext) -> bool:
-        r1 = await self.base(ctx)
-        # short circuit
-        if r1:
-            return True
-
-        return await self.other(ctx)
-
-
-CUSTOM_FILTER_NAME = "CustomFilter"
-
-
-def create(func: FilterCallback, name: str = None, **kwargs) -> Filter:
-    return type(
-        name or func.__name__ or CUSTOM_FILTER_NAME, (Filter,), {
-            "__call__": func, **kwargs}
-    )()
-
-
-async def all_filter(self, ctx: BotContext):
-    return True
-
-
-all = create(all_filter)
-"""Filter all messages."""
-
-
-async def self_filter(self, ctx: BotContext[MessageEvent]):
-    return bool(
-        ctx.event.message is not None
-        and ctx.event.message.user_id == ctx.event.message.receiver_id
-    )
-
-
-self = create(self_filter)
-"""Filter messages generated by the same user."""
-
-
-async def bot_filter(self, ctx: BotContext[MessageEvent]):
-    return bool(
-        ctx.event.message is not None and ctx.event.user is not None and ctx.event.user.is_bot
-    )
-
-
-is_bot = create(bot_filter)
-"""Filter messages coming from bots."""
-
-
-async def me_filter(self, ctx: BotContext[MessageEvent]):
-    return bool(ctx.event.message is not None and ctx.event.message.user_id == ctx.user.id)
-
-
-me = create(me_filter)
-"""Filter messages coming from your user."""
-
-
-async def incoming_filter(self, ctx: BotContext[MessageEvent]):
-    return bool(ctx.event.message is not None and ctx.event.message.receiver_id == ctx.user.id)
-
-
-incoming = create(incoming_filter)
-"""Filter incoming messages. Messages that are sent to the users recipient."""
-
-
-async def outgoing_filter(self, ctx: BotContext[MessageEvent]):
-    return not incoming(ctx)
-
-
-outgoing = create(outgoing_filter)
-"""Filter outgoing messages. Messages that are sent by the user."""
-
-
-class community(Filter, set):
-    """Filter events comming from a specific community or communities"""
-
-    def __init__(self, community_id: Optional[SCT[str]]):
-        community_id = community_id
-
-    async def __call__(self, ctx: BotContext[Event]):
-        community_id = self.community_id
-        if community_id is None:
-            return bool(ctx.event.community_id is not None)
-        if isinstance(community_id, str):
-            community_id = frozenset({community_id})
-        else:
-            community_id = frozenset(community_id)
-        return bool(ctx.event.community_id in community_id)
-
-
-class channel(Filter, set):
-    """Filter events comming from a specific channel or channels"""
-
-    def __init__(self, channel_id: Optional[SCT[str]]):
-        channel_id = channel_id
-
-    async def __call__(self, ctx: BotContext[Event]):
-        channel_id = self.channel_id
-        if channel_id is None:
-            return bool(ctx.event.channel_id is not None)
-        if isinstance(channel_id, str):
-            channel_id = frozenset({channel_id})
-        else:
-            channel_id = frozenset(channel_id)
-        return bool(ctx.event.channel_id in channel_id)
-
-
-class group(Filter, set):
-    def __init__(self, group_id: Optional[SCT[str]]):
-        group_id = group_id
-
-    async def __call__(self, ctx: BotContext[Event]):
-        group_id = self.group_id
-        if group_id is None:
-            return bool(ctx.event.group_id is not None)
-        if isinstance(group_id, str):
-            group_id = frozenset({group_id})
-        else:
-            group_id = frozenset(group_id)
-        return bool(ctx.event.group_id in group_id)
-
-
-class user(Filter, set):
-    def __init__(self, user_id: Optional[SCT[int]]):
-        user_id = user_id
-
-    async def __call__(self, ctx: BotContext[Event]):
-        user_id = self.user_id
-        if user_id is None:
-            return bool(ctx.event.action_by_id is not None)
-        if isinstance(user_id, int):
-            user_id = frozenset({user_id})
-        else:
-            user_id = frozenset(user_id)
-        return bool(ctx.event.action_by_id in user_id)
-
-
-def text(text: Optional[SCT[str]]):
-    async def func(self, ctx: BotContext[MessageEvent]):
-        text = self.text
-        if text is None:
-            return bool(ctx.event.message is not None and ctx.event.message.message is not None)
-        if isinstance(text, str):
-            text = frozenset({text})
-        else:
-            text = frozenset(text)
-
-        if ctx.event.type == EventType.MESSAGE:
-            value = ctx.event.message.message
-        elif ctx.event.type == EventType.COMMAND:
-            value = ctx.event.command
-        elif ctx.event.type == EventType.CALLBACK_QUERY:
-            value = ctx.event.callback_data
-
-        for t in text:
-            if t in value:
-                return True
-            else:
-                try:
-                    regexp = re.compile(t)
-                    if regexp.search(value):
-                        return True
-                except re.error:
-                    pass
-        return False
-
-    return create(func, name="TextFilter", text=text)
-
-
-""" Filter messages by text. """
-
-
-def regexp(regexp: Optional[SCT[str]]):
-    async def func(self, ctx: BotContext[MessageEvent]):
-        regexp = self.regexp
-        if regexp is None:
-            return bool(ctx.event.message is not None and ctx.event.message.message is not None)
-        if isinstance(regexp, str):
-            regexp = frozenset({regexp})
-        else:
-            regexp = frozenset(regexp)
-
-        if ctx.event.type == EventType.MESSAGE:
-            value = ctx.event.message.message
-        elif ctx.event.type == EventType.COMMAND:
-            value = ctx.event.command
-        elif ctx.event.type == EventType.CALLBACK_QUERY:
-            value = ctx.event.callback_data
-
-        if value is None:
-            return False
-
-        for r in regexp:
-            try:
-
-                cr = re.compile(r)
-                if cr.match(value):
-                    return True
-            except re.error:
-                pass
-        return False
-
-    return create(func, name="RegexpFilter", regexp=regexp)
-
-
-""" Filter messages by regexp. """
-
-
-async def message_type(types: Optional[SCT[int]]):
-    async def func(self, ctx: BotContext[MessageEvent]):
-        types = self.types
-        if types is None:
-            return bool(ctx.event.message.status is not None)
-        if isinstance(types, int):
-            types = frozenset({types})
-        else:
-            types = frozenset(types)
-        return bool(ctx.event.message.status in types)
-    return create(func, name="MessageType", types=types)
+import re
+from typing import Optional
+from swibots.api.chat.events import MessageEvent
+from swibots.api.chat.events.chat_event import ChatEvent
+from swibots.api.common.events import Event
+from swibots.bots.bot_context import BotContext
+from swibots.utils.types import SCT, FilterCallback
+from swibots.types import EventType
+from typing import Callable, Union, List, Pattern
+
+
+class Filter:
+    async def __call__(self, ctx: BotContext) -> bool:
+        raise NotImplementedError
+
+    def __invert__(self):
+        return InvertFilter(self)
+
+    def __and__(self, other):
+        return AndFilter(self, other)
+
+    def __or__(self, other):
+        return OrFilter(self, other)
+
+
+class InvertFilter(Filter):
+    def __init__(self, base):
+        self.base = base
+
+    async def __call__(self, ctx: BotContext) -> bool:
+        result = await self.base(ctx)
+        return not result
+
+
+class AndFilter(Filter):
+    def __init__(self, base, other):
+        self.base = base
+        self.other = other
+
+    async def __call__(self, ctx: BotContext) -> bool:
+        r1 = await self.base(ctx)
+        # short circuit
+        if not r1:
+            return False
+        r2 = await self.other(ctx)
+
+        return r1 and r2
+
+
+class OrFilter(Filter):
+    def __init__(self, base, other):
+        self.base = base
+        self.other = other
+
+    async def __call__(self, ctx: BotContext) -> bool:
+        r1 = await self.base(ctx)
+        # short circuit
+        if r1:
+            return True
+
+        return await self.other(ctx)
+
+
+CUSTOM_FILTER_NAME = "CustomFilter"
+
+
+def create(func: FilterCallback, name: str = None, **kwargs) -> Filter:
+    return type(
+        name or func.__name__ or CUSTOM_FILTER_NAME, (Filter,), {
+            "__call__": func, **kwargs}
+    )()
+
+
+async def all_filter(self, ctx: BotContext):
+    return True
+
+
+all = create(all_filter)
+"""Filter all messages."""
+
+
+async def self_filter(self, ctx: BotContext[MessageEvent]):
+    return bool(
+        ctx.event.message is not None
+        and ctx.event.message.user_id == ctx.event.message.receiver_id
+    )
+
+
+self = create(self_filter)
+"""Filter messages generated by the same user."""
+
+
+async def bot_filter(self, ctx: BotContext[MessageEvent]):
+    return bool(
+        ctx.event.message is not None and ctx.event.user is not None and ctx.event.user.is_bot
+    )
+
+
+is_bot = create(bot_filter)
+"""Filter messages coming from bots."""
+
+
+async def me_filter(self, ctx: BotContext[MessageEvent]):
+    return bool(ctx.event.message is not None and ctx.event.message.user_id == ctx.user.id)
+
+
+me = create(me_filter)
+"""Filter messages coming from your user."""
+
+
+async def incoming_filter(self, ctx: BotContext[MessageEvent]):
+    return bool(ctx.event.message is not None and ctx.event.message.receiver_id == ctx.user.id)
+
+
+incoming = create(incoming_filter)
+"""Filter incoming messages. Messages that are sent to the users recipient."""
+
+
+async def outgoing_filter(self, ctx: BotContext[MessageEvent]):
+    return not incoming(ctx)
+
+
+outgoing = create(outgoing_filter)
+"""Filter outgoing messages. Messages that are sent by the user."""
+
+
+class community(Filter, set):
+    """Filter events comming from a specific community or communities"""
+
+    def __init__(self, community_id: Optional[SCT[str]]):
+        community_id = community_id
+
+    async def __call__(self, ctx: BotContext[Event]):
+        community_id = self.community_id
+        if community_id is None:
+            return bool(ctx.event.community_id is not None)
+        if isinstance(community_id, str):
+            community_id = frozenset({community_id})
+        else:
+            community_id = frozenset(community_id)
+        return bool(ctx.event.community_id in community_id)
+
+
+class channel(Filter, set):
+    """Filter events comming from a specific channel or channels"""
+
+    def __init__(self, channel_id: Optional[SCT[str]]):
+        channel_id = channel_id
+
+    async def __call__(self, ctx: BotContext[Event]):
+        channel_id = self.channel_id
+        if channel_id is None:
+            return bool(ctx.event.channel_id is not None)
+        if isinstance(channel_id, str):
+            channel_id = frozenset({channel_id})
+        else:
+            channel_id = frozenset(channel_id)
+        return bool(ctx.event.channel_id in channel_id)
+
+
+class group(Filter, set):
+    def __init__(self, group_id: Optional[SCT[str]]):
+        group_id = group_id
+
+    async def __call__(self, ctx: BotContext[Event]):
+        group_id = self.group_id
+        if group_id is None:
+            return bool(ctx.event.group_id is not None)
+        if isinstance(group_id, str):
+            group_id = frozenset({group_id})
+        else:
+            group_id = frozenset(group_id)
+        return bool(ctx.event.group_id in group_id)
+
+
+class user(Filter, set):
+    def __init__(self, user_id: Optional[SCT[int]]):
+        user_id = user_id
+
+    async def __call__(self, ctx: BotContext[Event]):
+        user_id = self.user_id
+        if user_id is None:
+            return bool(ctx.event.action_by_id is not None)
+        if isinstance(user_id, int):
+            user_id = frozenset({user_id})
+        else:
+            user_id = frozenset(user_id)
+        return bool(ctx.event.action_by_id in user_id)
+
+
+def text(text: Optional[SCT[str]]):
+    async def func(self, ctx: BotContext[MessageEvent]):
+        text = self.text
+        if text is None:
+            return bool(ctx.event.message is not None and ctx.event.message.message is not None)
+        if isinstance(text, str):
+            text = frozenset({text})
+        else:
+            text = frozenset(text)
+
+        if ctx.event.type == EventType.MESSAGE:
+            value = ctx.event.message.message
+        elif ctx.event.type == EventType.COMMAND:
+            value = ctx.event.command
+        elif ctx.event.type == EventType.CALLBACK_QUERY:
+            value = ctx.event.callback_data
+
+        for t in text:
+            if t in value:
+                return True
+            else:
+                try:
+                    regexp = re.compile(t)
+                    if regexp.search(value):
+                        return True
+                except re.error:
+                    pass
+        return False
+
+    return create(func, name="TextFilter", text=text)
+
+
+""" Filter messages by text. """
+
+
+def regexp(regexp: Optional[SCT[str]]):
+    async def func(self, ctx: BotContext[MessageEvent]):
+        regexp = self.regexp
+        if regexp is None:
+            return bool(ctx.event.message is not None and ctx.event.message.message is not None)
+        if isinstance(regexp, str):
+            regexp = frozenset({regexp})
+        else:
+            regexp = frozenset(regexp)
+
+        if ctx.event.type == EventType.MESSAGE:
+            value = ctx.event.message.message
+        elif ctx.event.type == EventType.COMMAND:
+            value = ctx.event.command
+        elif ctx.event.type == EventType.CALLBACK_QUERY:
+            value = ctx.event.callback_data
+
+        if value is None:
+            return False
+
+        for r in regexp:
+            try:
+
+                cr = re.compile(r)
+                if cr.match(value):
+                    return True
+            except re.error:
+                pass
+        return False
+
+    return create(func, name="RegexpFilter", regexp=regexp)
+
+
+""" Filter messages by regexp. """
+
+
+async def message_type(types: Optional[SCT[int]]):
+    async def func(self, ctx: BotContext[MessageEvent]):
+        types = self.types
+        if types is None:
+            return bool(ctx.event.message.status is not None)
+        if isinstance(types, int):
+            types = frozenset({types})
+        else:
+            types = frozenset(types)
+        return bool(ctx.event.message.status in types)
+    return create(func, name="MessageType", types=types)
```

### Comparing `swibots-1.1.9/swibots/bots/handlers/__init__.py` & `swibots-1.2.0/swibots/bots/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bots/handlers/base_handler.py` & `swibots-1.2.0/swibots/bots/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bots/handlers/callback_query_handler.py` & `swibots-1.2.0/swibots/bots/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bots/handlers/channel_created_handler.py` & `swibots-1.2.0/swibots/bots/handlers/group_updated_handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-from typing import TYPE_CHECKING, Optional, TypeVar
-from swibots.api.community.events import ChannelCreatedEvent
-from swibots.bots.filters import Filter
-
-from swibots.bots import BotContext
-from .event_handler import EventHandler
-from swibots.types import EventType
-from swibots.utils.types import HandlerCallback
-
-if TYPE_CHECKING:
-    pass
-
-ResType = TypeVar("ResType")
-
-
-class ChannelCreatedHandler(EventHandler):
-    def __init__(
-        self,
-        callback: HandlerCallback[BotContext[ChannelCreatedEvent], ResType],
-        filter: Optional[Filter] = None,
-        **kwargs,
-    ):
-        super().__init__(EventType.COMMUNITY_CHANNEL_CREATE, callback, filter, **kwargs)
+from typing import TYPE_CHECKING, Optional, TypeVar
+from swibots.api.chat.events import MessageEvent
+from swibots.api.community.events import GroupUpdatedEvent
+from swibots.bots.filters.filter import Filter
+
+from swibots.bots.handlers import BaseHandler
+from swibots.bots import BotContext
+from .event_handler import EventHandler
+from swibots.types import EventType
+from swibots.utils.types import HandlerCallback
+
+if TYPE_CHECKING:
+    pass
+
+ResType = TypeVar("ResType")
+
+
+class GroupUpdatedHandler(EventHandler):
+    def __init__(
+        self,
+        callback: HandlerCallback[BotContext[GroupUpdatedEvent], ResType],
+        filter: Optional[Filter] = None,
+        **kwargs,
+    ):
+        super().__init__(EventType.COMMUNITY_GROUP_UPDATE, callback, filter, **kwargs)
```

### Comparing `swibots-1.1.9/swibots/bots/handlers/channel_deleted_handler.py` & `swibots-1.2.0/swibots/bots/handlers/channel_deleted_handler.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import TYPE_CHECKING, Optional, TypeVar
-from swibots.api.community.events import ChannelDeletedEvent
-from swibots.bots.filters.filter import Filter
-
-from swibots.bots import BotContext
-from .event_handler import EventHandler
-from swibots.types import EventType
-from swibots.utils.types import HandlerCallback
-
-if TYPE_CHECKING:
-    pass
-
-ResType = TypeVar("ResType")
-
-
-class ChannelDeletedHandler(EventHandler):
-    def __init__(
-        self,
-        callback: HandlerCallback[BotContext[ChannelDeletedEvent], ResType],
-        filter: Optional[Filter] = None,
-        **kwargs,
-    ):
-        super().__init__(EventType.COMMUNITY_CHANNEL_DELETE, callback, filter, **kwargs)
+from typing import TYPE_CHECKING, Optional, TypeVar
+from swibots.api.community.events import ChannelDeletedEvent
+from swibots.bots.filters.filter import Filter
+
+from swibots.bots import BotContext
+from .event_handler import EventHandler
+from swibots.types import EventType
+from swibots.utils.types import HandlerCallback
+
+if TYPE_CHECKING:
+    pass
+
+ResType = TypeVar("ResType")
+
+
+class ChannelDeletedHandler(EventHandler):
+    def __init__(
+        self,
+        callback: HandlerCallback[BotContext[ChannelDeletedEvent], ResType],
+        filter: Optional[Filter] = None,
+        **kwargs,
+    ):
+        super().__init__(EventType.COMMUNITY_CHANNEL_DELETE, callback, filter, **kwargs)
```

### Comparing `swibots-1.1.9/swibots/bots/handlers/channel_updated_handler.py` & `swibots-1.2.0/swibots/bots/handlers/member_joined_handler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-from typing import TYPE_CHECKING, Optional, TypeVar
-from swibots.api.community.events import ChannelUpdatedEvent
-from swibots.bots.filters.filter import Filter
-
-from swibots.bots.handlers import BaseHandler
-from swibots.bots import BotContext
-from .event_handler import EventHandler
-from swibots.types import EventType
-from swibots.utils.types import HandlerCallback
-
-if TYPE_CHECKING:
-    pass
-
-ResType = TypeVar("ResType")
-
-
-class ChannelUpdatedHandler(EventHandler):
-    def __init__(
-        self,
-        callback: HandlerCallback[BotContext[ChannelUpdatedEvent], ResType],
-        filter: Optional[Filter] = None,
-        **kwargs,
-    ):
-        super().__init__(EventType.COMMUNITY_CHANNEL_UPDATE, callback, filter, **kwargs)
+from typing import TYPE_CHECKING, Optional, TypeVar
+from swibots.api.community.events import MemberJoinedEvent
+from swibots.bots.filters.filter import Filter
+
+from swibots.bots import BotContext
+from .event_handler import EventHandler
+from swibots.types import EventType
+from swibots.utils.types import HandlerCallback
+
+if TYPE_CHECKING:
+    pass
+
+ResType = TypeVar("ResType")
+
+
+class MemberJoinedHandler(EventHandler):
+    def __init__(
+        self,
+        callback: HandlerCallback[BotContext[MemberJoinedEvent], ResType],
+        filter: Optional[Filter] = None,
+        **kwargs,
+    ):
+        super().__init__(EventType.COMMUNITY_MEMBER_JOIN, callback, filter, **kwargs)
```

### Comparing `swibots-1.1.9/swibots/bots/handlers/command_handler.py` & `swibots-1.2.0/swibots/bots/handlers/command_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bots/handlers/community_updated_handler.py` & `swibots-1.2.0/swibots/bots/handlers/community_updated_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bots/handlers/event_handler.py` & `swibots-1.2.0/swibots/bots/handlers/event_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bots/handlers/group_created_handler.py` & `swibots-1.2.0/swibots/bots/handlers/group_deleted_handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-from typing import TYPE_CHECKING, Optional, TypeVar
-from swibots.api.community.events import GroupCreatedEvent
-from swibots.bots.filters.filter import Filter
-
-from swibots.bots import BotContext
-from .event_handler import EventHandler
-from swibots.types import EventType
-from swibots.utils.types import HandlerCallback
-
-if TYPE_CHECKING:
-    pass
-
-ResType = TypeVar("ResType")
-
-
-class GroupCreatedHandler(EventHandler):
-    def __init__(
-        self,
-        callback: HandlerCallback[BotContext[GroupCreatedEvent], ResType],
-        filter: Optional[Filter] = None,
-        **kwargs,
-    ):
-        super().__init__(EventType.COMMUNITY_GROUP_CREATE, callback, filter, **kwargs)
+from typing import TYPE_CHECKING, Optional, TypeVar
+from swibots.api.chat.events import MessageEvent
+from swibots.api.community.events import GroupDeletedEvent
+from swibots.bots.filters.filter import Filter
+
+from swibots.bots.handlers import BaseHandler
+from swibots.bots import BotContext
+from .event_handler import EventHandler
+from swibots.types import EventType
+from swibots.utils.types import HandlerCallback
+
+if TYPE_CHECKING:
+    pass
+
+ResType = TypeVar("ResType")
+
+
+class GroupDeletedHandler(EventHandler):
+    def __init__(
+        self,
+        callback: HandlerCallback[BotContext[GroupDeletedEvent], ResType],
+        filter: Optional[Filter] = None,
+        **kwargs,
+    ):
+        super().__init__(EventType.COMMUNITY_GROUP_DELETE, callback, filter, **kwargs)
```

### Comparing `swibots-1.1.9/swibots/bots/handlers/group_deleted_handler.py` & `swibots-1.2.0/swibots/bots/handlers/channel_updated_handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-from typing import TYPE_CHECKING, Optional, TypeVar
-from swibots.api.chat.events import MessageEvent
-from swibots.api.community.events import GroupDeletedEvent
-from swibots.bots.filters.filter import Filter
-
-from swibots.bots.handlers import BaseHandler
-from swibots.bots import BotContext
-from .event_handler import EventHandler
-from swibots.types import EventType
-from swibots.utils.types import HandlerCallback
-
-if TYPE_CHECKING:
-    pass
-
-ResType = TypeVar("ResType")
-
-
-class GroupDeletedHandler(EventHandler):
-    def __init__(
-        self,
-        callback: HandlerCallback[BotContext[GroupDeletedEvent], ResType],
-        filter: Optional[Filter] = None,
-        **kwargs,
-    ):
-        super().__init__(EventType.COMMUNITY_GROUP_DELETE, callback, filter, **kwargs)
+from typing import TYPE_CHECKING, Optional, TypeVar
+from swibots.api.community.events import ChannelUpdatedEvent
+from swibots.bots.filters.filter import Filter
+
+from swibots.bots.handlers import BaseHandler
+from swibots.bots import BotContext
+from .event_handler import EventHandler
+from swibots.types import EventType
+from swibots.utils.types import HandlerCallback
+
+if TYPE_CHECKING:
+    pass
+
+ResType = TypeVar("ResType")
+
+
+class ChannelUpdatedHandler(EventHandler):
+    def __init__(
+        self,
+        callback: HandlerCallback[BotContext[ChannelUpdatedEvent], ResType],
+        filter: Optional[Filter] = None,
+        **kwargs,
+    ):
+        super().__init__(EventType.COMMUNITY_CHANNEL_UPDATE, callback, filter, **kwargs)
```

### Comparing `swibots-1.1.9/swibots/bots/handlers/group_updated_handler.py` & `swibots-1.2.0/swibots/bots/handlers/user_banned_handler.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-from typing import TYPE_CHECKING, Optional, TypeVar
-from swibots.api.chat.events import MessageEvent
-from swibots.api.community.events import GroupUpdatedEvent
-from swibots.bots.filters.filter import Filter
-
-from swibots.bots.handlers import BaseHandler
-from swibots.bots import BotContext
-from .event_handler import EventHandler
-from swibots.types import EventType
-from swibots.utils.types import HandlerCallback
-
-if TYPE_CHECKING:
-    pass
-
-ResType = TypeVar("ResType")
-
-
-class GroupUpdatedHandler(EventHandler):
-    def __init__(
-        self,
-        callback: HandlerCallback[BotContext[GroupUpdatedEvent], ResType],
-        filter: Optional[Filter] = None,
-        **kwargs,
-    ):
-        super().__init__(EventType.COMMUNITY_GROUP_UPDATE, callback, filter, **kwargs)
+from typing import TYPE_CHECKING, Optional, TypeVar
+from swibots.api.community.events import UserBannedEvent
+from swibots.bots.filters.filter import Filter
+
+from swibots.bots import BotContext
+from .event_handler import EventHandler
+from swibots.types import EventType
+from swibots.utils.types import HandlerCallback
+
+if TYPE_CHECKING:
+    pass
+
+ResType = TypeVar("ResType")
+
+
+class UserBannedHandler(EventHandler):
+    def __init__(
+        self,
+        callback: HandlerCallback[BotContext[UserBannedEvent], ResType],
+        filter: Optional[Filter] = None,
+        **kwargs,
+    ):
+        super().__init__(EventType.COMMUNITY_USER_BAN, callback, filter, **kwargs)
```

### Comparing `swibots-1.1.9/swibots/bots/handlers/inline_query_handler.py` & `swibots-1.2.0/swibots/bots/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bots/handlers/member_joined_handler.py` & `swibots-1.2.0/swibots/bots/handlers/member_left_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import TYPE_CHECKING, Optional, TypeVar
-from swibots.api.community.events import MemberJoinedEvent
-from swibots.bots.filters.filter import Filter
-
-from swibots.bots import BotContext
-from .event_handler import EventHandler
-from swibots.types import EventType
-from swibots.utils.types import HandlerCallback
-
-if TYPE_CHECKING:
-    pass
-
-ResType = TypeVar("ResType")
-
-
-class MemberJoinedHandler(EventHandler):
-    def __init__(
-        self,
-        callback: HandlerCallback[BotContext[MemberJoinedEvent], ResType],
-        filter: Optional[Filter] = None,
-        **kwargs,
-    ):
-        super().__init__(EventType.COMMUNITY_MEMBER_JOIN, callback, filter, **kwargs)
+from typing import TYPE_CHECKING, Optional, TypeVar
+from swibots.api.community.events import MemberLeftEvent
+from swibots.bots.filters.filter import Filter
+
+from swibots.bots import BotContext
+from .event_handler import EventHandler
+from swibots.types import EventType
+from swibots.utils.types import HandlerCallback
+
+if TYPE_CHECKING:
+    pass
+
+ResType = TypeVar("ResType")
+
+
+class MemberLeftHandler(EventHandler):
+    def __init__(
+        self,
+        callback: HandlerCallback[BotContext[MemberLeftEvent], ResType],
+        filter: Optional[Filter] = None,
+        **kwargs,
+    ):
+        super().__init__(EventType.COMMUNITY_MEMBER_LEAVE, callback, filter, **kwargs)
```

### Comparing `swibots-1.1.9/swibots/bots/handlers/message_handler.py` & `swibots-1.2.0/swibots/bots/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/bots/handlers/unknown_command_handler.py` & `swibots-1.2.0/swibots/bots/handlers/unknown_command_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/config.py` & `swibots-1.2.0/swibots/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 
 
 APP_CONFIG = {
     "CHAT_SERVICE": {
-        "BASE_URL": os.getenv("CHAT_SERVICE_BASE_URL") or "https://api-gateway.switch.pe",
+        "BASE_URL": os.getenv("CHAT_SERVICE_BASE_URL") or "https://chat.switch.pe",
         "WS_URL": os.getenv("CHAT_SERVICE_WS_URL")
         or "wss://api-gateway.switch.pe/v1/websocket/message/ws",
     },
     "BOT_SERVICE": {
-        "BASE_URL": os.getenv("BOT_SERVICE_BASE_URL") or "https://api-gateway.switch.pe",
+        "BASE_URL": os.getenv("BOT_SERVICE_BASE_URL") or "https://chat.switch.pe",
     },
     "AUTH_SERVICE": {
         "BASE_URL": os.getenv("AUTH_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/api",
     },
     "COMMUNITY_SERVICE": {
         "BASE_URL": os.getenv("COMMUNITY_SERVICE_BASE_URL") or "https://api-gateway.switch.pe",
         "WS_URL": os.getenv("COMMUNITY_SERVICE_WS_URL")
@@ -23,19 +23,19 @@
 
 def get_config():
     return APP_CONFIG
 
 
 def reload_config():
     APP_CONFIG["CHAT_SERVICE"]['BASE_URL'] = os.getenv(
-        "CHAT_SERVICE_BASE_URL") or "https://api-gateway.switch.pe"
+        "CHAT_SERVICE_BASE_URL") or "https://chat.switch.pe"
     APP_CONFIG["CHAT_SERVICE"]['WS_URL'] = os.getenv(
         "CHAT_SERVICE_WS_URL") or "wss://api-gateway.switch.pe/v1/websocket/message/ws"
     APP_CONFIG["BOT_SERVICE"]['BASE_URL'] = os.getenv(
-        "BOT_SERVICE_BASE_URL") or "https://api-gateway.switch.pe"
+        "BOT_SERVICE_BASE_URL") or "https://chat.switch.pe"
     APP_CONFIG["AUTH_SERVICE"]['BASE_URL'] = os.getenv(
         "AUTH_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/api"
     APP_CONFIG["COMMUNITY_SERVICE"]['BASE_URL'] = os.getenv(
         "COMMUNITY_SERVICE_BASE_URL") or "https://api-gateway.switch.pe"
     APP_CONFIG["COMMUNITY_SERVICE"]['WS_URL'] = os.getenv(
         "COMMUNITY_SERVICE_WS_URL") or "wss://api-gateway.switch.pe/v1/websocket/community/ws"
```

### Comparing `swibots-1.1.9/swibots/error.py` & `swibots-1.2.0/swibots/error.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/types.py` & `swibots-1.2.0/swibots/types.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import enum
-
-
-class EventType(enum.Enum):
-    """Represents the type of a event."""
-
-    # Chat
-    MESSAGE = "MESSAGE"
-    COMMAND = "COMMAND"
-    CALLBACK_QUERY = "CALLBACK_QUERY"
-    INLINE_QUERY = "INLINE_QUERY"
-    # Community
-    COMMUNITY_CHANNEL_CREATE = "COMMUNITY_CHANNEL_CREATE"
-    COMMUNITY_CHANNEL_UPDATE = "COMMUNITY_CHANNEL_UPDATE"
-    COMMUNITY_CHANNEL_DELETE = "COMMUNITY_CHANNEL_DELETE"
-    COMMUNITY_GROUP_CREATE = "COMMUNITY_GROUP_CREATE"
-    COMMUNITY_GROUP_UPDATE = "COMMUNITY_GROUP_UPDATE"
-    COMMUNITY_GROUP_DELETE = "COMMUNITY_GROUP_DELETE"
-    COMMUNITY_USER_BAN = "COMMUNITY_USER_BAN"
-    COMMUNITY_USER_UNBAN = "COMMUNITY_USER_UNBAN"
-    COMMUNITY_MEMBER_JOIN = "COMMUNITY_MEMBER_JOIN"
-    COMMUNITY_MEMBER_LEAVE = "COMMUNITY_MEMBER_LEAVE"
-    COMMUNITY_UPDATE = "COMMUNITY_UPDATE"
-    COMMUNITY_DELETE = "COMMUNITY_DELETE"
+import enum
+
+
+class EventType(enum.Enum):
+    """Represents the type of a event."""
+
+    # Chat
+    MESSAGE = "MESSAGE"
+    COMMAND = "COMMAND"
+    CALLBACK_QUERY = "CALLBACK_QUERY"
+    INLINE_QUERY = "INLINE_QUERY"
+    # Community
+    COMMUNITY_CHANNEL_CREATE = "COMMUNITY_CHANNEL_CREATE"
+    COMMUNITY_CHANNEL_UPDATE = "COMMUNITY_CHANNEL_UPDATE"
+    COMMUNITY_CHANNEL_DELETE = "COMMUNITY_CHANNEL_DELETE"
+    COMMUNITY_GROUP_CREATE = "COMMUNITY_GROUP_CREATE"
+    COMMUNITY_GROUP_UPDATE = "COMMUNITY_GROUP_UPDATE"
+    COMMUNITY_GROUP_DELETE = "COMMUNITY_GROUP_DELETE"
+    COMMUNITY_USER_BAN = "COMMUNITY_USER_BAN"
+    COMMUNITY_USER_UNBAN = "COMMUNITY_USER_UNBAN"
+    COMMUNITY_MEMBER_JOIN = "COMMUNITY_MEMBER_JOIN"
+    COMMUNITY_MEMBER_LEAVE = "COMMUNITY_MEMBER_LEAVE"
+    COMMUNITY_UPDATE = "COMMUNITY_UPDATE"
+    COMMUNITY_DELETE = "COMMUNITY_DELETE"
```

### Comparing `swibots-1.1.9/swibots/utils/rest_client.py` & `swibots-1.2.0/swibots/utils/rest_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/utils/types.py` & `swibots-1.2.0/swibots/utils/types.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/utils/ws/asyncstomp/async_ws_client.py` & `swibots-1.2.0/swibots/utils/ws/asyncstomp/async_ws_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/utils/ws/asyncstomp/async_ws_subscription.py` & `swibots-1.2.0/swibots/utils/ws/asyncstomp/async_ws_subscription.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots/utils/ws/common/ws_frame.py` & `swibots-1.2.0/swibots/utils/ws/common/ws_frame.py`

 * *Files identical despite different names*

### Comparing `swibots-1.1.9/swibots.egg-info/SOURCES.txt` & `swibots-1.2.0/swibots.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -171,8 +171,10 @@
 swibots/utils/types.py
 swibots/utils/ws/__init__.py
 swibots/utils/ws/asyncstomp/__init__.py
 swibots/utils/ws/asyncstomp/async_ws_client.py
 swibots/utils/ws/asyncstomp/async_ws_subscription.py
 swibots/utils/ws/common/__init__.py
 swibots/utils/ws/common/ws_frame.py
-swibots/utils/ws/common/ws_message.py
+swibots/utils/ws/common/ws_message.py
+tests/__init__.py
+tests/tests.py
```

