# Comparing `tmp/atproto-0.0.7.tar.gz` & `tmp/atproto-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atproto-0.0.7.tar", max compression
+gzip compressed data, was "atproto-0.0.8.tar", max compression
```

## Comparing `atproto-0.0.7.tar` & `atproto-0.0.8.tar`

### file list

```diff
@@ -1,170 +1,361 @@
--rw-r--r--   0        0        0     1061 2023-05-20 15:15:38.757786 atproto-0.0.7/LICENSE
--rw-r--r--   0        0        0     9588 2023-05-20 15:15:38.757786 atproto-0.0.7/README.md
--rw-r--r--   0        0        0      332 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/__init__.py
--rw-r--r--   0        0        0     1761 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/car/__init__.py
--rw-r--r--   0        0        0      137 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/cid/__init__.py
--rw-r--r--   0        0        0       23 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/cli/__init__.py
--rw-r--r--   0        0        0     2790 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/codegen/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/codegen/clients/__init__.py
--rw-r--r--   0        0        0     1434 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/codegen/clients/generate_async_client.py
--rw-r--r--   0        0        0        0 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/codegen/models/__init__.py
--rw-r--r--   0        0        0     2345 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/codegen/models/builder.py
--rw-r--r--   0        0        0    19267 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/codegen/models/generator.py
--rw-r--r--   0        0        0        0 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/codegen/namespaces/__init__.py
--rw-r--r--   0        0        0     2546 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/codegen/namespaces/builder.py
--rw-r--r--   0        0        0    11836 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/codegen/namespaces/generator.py
--rw-r--r--   0        0        0      944 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/exceptions.py
--rw-r--r--   0        0        0     2569 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/leb128/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/lexicon/__init__.py
--rw-r--r--   0        0        0     4790 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/lexicon/models.py
--rw-r--r--   0        0        0     3857 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/lexicon/parser.py
--rw-r--r--   0        0        0     5295 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/nsid/__init__.py
--rw-r--r--   0        0        0     3064 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/uri/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/client/__init__.py
--rw-r--r--   0        0        0     7596 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/client/async_client.py
--rw-r--r--   0        0        0      489 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/client/async_raw.py
--rw-r--r--   0        0        0      414 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/client/auth.py
--rw-r--r--   0        0        0     3748 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/client/base.py
--rw-r--r--   0        0        0     7105 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/client/client.py
--rw-r--r--   0        0        0       76 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/client/methods_mixin/__init__.py
--rw-r--r--   0        0        0     1311 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/client/methods_mixin/session.py
--rw-r--r--   0        0        0      469 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/client/raw.py
--rw-r--r--   0        0        0    11424 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/__init__.py
--rw-r--r--   0        0        0      323 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/__init__.py
--rw-r--r--   0        0        0      323 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/__init__.py
--rw-r--r--   0        0        0      323 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/__init__.py
--rw-r--r--   0        0        0     4112 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/defs.py
--rw-r--r--   0        0        0      820 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/get_preferences.py
--rw-r--r--   0        0        0      833 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/get_profile.py
--rw-r--r--   0        0        0      889 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py
--rw-r--r--   0        0        0     1007 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py
--rw-r--r--   0        0        0      926 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/profile.py
--rw-r--r--   0        0        0      670 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/put_preferences.py
--rw-r--r--   0        0        0     1056 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/search_actors.py
--rw-r--r--   0        0        0      961 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py
--rw-r--r--   0        0        0      323 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/embed/__init__.py
--rw-r--r--   0        0        0     1773 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/embed/external.py
--rw-r--r--   0        0        0     1563 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/embed/images.py
--rw-r--r--   0        0        0     2444 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/embed/record.py
--rw-r--r--   0        0        0     1243 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py
--rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/__init__.py
--rw-r--r--   0        0        0     4340 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/defs.py
--rw-r--r--   0        0        0     1034 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py
--rw-r--r--   0        0        0     1494 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/get_likes.py
--rw-r--r--   0        0        0     1057 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py
--rw-r--r--   0        0        0      854 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/get_posts.py
--rw-r--r--   0        0        0     1178 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py
--rw-r--r--   0        0        0     1061 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py
--rw-r--r--   0        0        0      734 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/like.py
--rw-r--r--   0        0        0     2426 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/post.py
--rw-r--r--   0        0        0      738 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/repost.py
--rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/__init__.py
--rw-r--r--   0        0        0      665 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/block.py
--rw-r--r--   0        0        0     2448 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/defs.py
--rw-r--r--   0        0        0      667 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/follow.py
--rw-r--r--   0        0        0      997 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py
--rw-r--r--   0        0        0     1126 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_followers.py
--rw-r--r--   0        0        0     1116 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_follows.py
--rw-r--r--   0        0        0     1090 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_list.py
--rw-r--r--   0        0        0      997 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_list_mutes.py
--rw-r--r--   0        0        0     1026 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_lists.py
--rw-r--r--   0        0        0      992 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py
--rw-r--r--   0        0        0     1114 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/list.py
--rw-r--r--   0        0        0      705 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/listitem.py
--rw-r--r--   0        0        0      574 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py
--rw-r--r--   0        0        0      575 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/mute_actor_list.py
--rw-r--r--   0        0        0      576 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py
--rw-r--r--   0        0        0      577 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/unmute_actor_list.py
--rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/notification/__init__.py
--rw-r--r--   0        0        0      823 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py
--rw-r--r--   0        0        0     1933 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py
--rw-r--r--   0        0        0      586 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/notification/update_seen.py
--rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/richtext/__init__.py
--rw-r--r--   0        0        0     1734 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/richtext/facet.py
--rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/unspecced/__init__.py
--rw-r--r--   0        0        0     1077 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py
--rw-r--r--   0        0        0      553 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/base.py
--rw-r--r--   0        0        0      713 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/blob_ref.py
--rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/__init__.py
--rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/__init__.py
--rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/__init__.py
--rw-r--r--   0        0        0    10957 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/defs.py
--rw-r--r--   0        0        0      595 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/disable_account_invites.py
--rw-r--r--   0        0        0      705 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py
--rw-r--r--   0        0        0      594 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/enable_account_invites.py
--rw-r--r--   0        0        0     1066 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py
--rw-r--r--   0        0        0      836 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py
--rw-r--r--   0        0        0     1092 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py
--rw-r--r--   0        0        0      836 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py
--rw-r--r--   0        0        0     1230 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py
--rw-r--r--   0        0        0      879 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_record.py
--rw-r--r--   0        0        0      821 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_repo.py
--rw-r--r--   0        0        0      946 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py
--rw-r--r--   0        0        0      908 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py
--rw-r--r--   0        0        0     1126 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/search_repos.py
--rw-r--r--   0        0        0     1351 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py
--rw-r--r--   0        0        0      651 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py
--rw-r--r--   0        0        0      621 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py
--rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/identity/__init__.py
--rw-r--r--   0        0        0      880 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py
--rw-r--r--   0        0        0      586 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/identity/update_handle.py
--rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/label/__init__.py
--rw-r--r--   0        0        0     1235 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/label/defs.py
--rw-r--r--   0        0        0     1322 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/label/query_labels.py
--rw-r--r--   0        0        0     1066 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py
--rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/moderation/__init__.py
--rw-r--r--   0        0        0     1488 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/moderation/create_report.py
--rw-r--r--   0        0        0      845 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/moderation/defs.py
--rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/__init__.py
--rw-r--r--   0        0        0     2121 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py
--rw-r--r--   0        0        0     1233 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/create_record.py
--rw-r--r--   0        0        0      964 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/delete_record.py
--rw-r--r--   0        0        0     1035 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py
--rw-r--r--   0        0        0     1166 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/get_record.py
--rw-r--r--   0        0        0     1816 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/list_records.py
--rw-r--r--   0        0        0     1316 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/put_record.py
--rw-r--r--   0        0        0      727 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/rebase_repo.py
--rw-r--r--   0        0        0      644 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py
--rw-r--r--   0        0        0      736 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py
--rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/__init__.py
--rw-r--r--   0        0        0     1208 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/create_account.py
--rw-r--r--   0        0        0     1049 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/create_app_password.py
--rw-r--r--   0        0        0      873 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py
--rw-r--r--   0        0        0     1345 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py
--rw-r--r--   0        0        0     1110 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/create_session.py
--rw-r--r--   0        0        0     1293 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/defs.py
--rw-r--r--   0        0        0      659 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/delete_account.py
--rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/delete_session.py
--rw-r--r--   0        0        0     1266 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/describe_server.py
--rw-r--r--   0        0        0     1019 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py
--rw-r--r--   0        0        0      697 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/get_session.py
--rw-r--r--   0        0        0     1021 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py
--rw-r--r--   0        0        0      729 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/refresh_session.py
--rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/request_account_delete.py
--rw-r--r--   0        0        0      589 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py
--rw-r--r--   0        0        0      628 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/reset_password.py
--rw-r--r--   0        0        0      583 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py
--rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/__init__.py
--rw-r--r--   0        0        0      746 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_blob.py
--rw-r--r--   0        0        0      734 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py
--rw-r--r--   0        0        0      808 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py
--rw-r--r--   0        0        0      977 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py
--rw-r--r--   0        0        0      764 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_head.py
--rw-r--r--   0        0        0      858 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_record.py
--rw-r--r--   0        0        0      904 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_repo.py
--rw-r--r--   0        0        0      960 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py
--rw-r--r--   0        0        0     1246 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/list_repos.py
--rw-r--r--   0        0        0      637 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py
--rw-r--r--   0        0        0      640 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py
--rw-r--r--   0        0        0     2774 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py
--rw-r--r--   0        0        0      547 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/type_conversion.py
--rw-r--r--   0        0        0     3254 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/utils.py
--rw-r--r--   0        0        0        0 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/namespaces/__init__.py
--rw-r--r--   0        0        0    73557 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/namespaces/async_ns.py
--rw-r--r--   0        0        0      344 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/namespaces/base.py
--rw-r--r--   0        0        0    72513 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/namespaces/sync_ns.py
--rw-r--r--   0        0        0     4338 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/request.py
--rw-r--r--   0        0        0       43 2023-05-20 15:15:38.765786 atproto-0.0.7/atproto/xrpc_server/__init__.py
--rw-r--r--   0        0        0     2396 2023-05-20 15:16:02.758155 atproto-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    11262 1970-01-01 00:00:00.000000 atproto-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-03 00:31:59.665109 atproto-0.0.8/LICENSE
+-rw-r--r--   0        0        0     9562 2023-05-23 13:37:14.635281 atproto-0.0.8/README.md
+-rw-r--r--   0        0        0     6148 2023-05-08 17:39:02.583646 atproto-0.0.8/atproto/.DS_Store
+-rw-r--r--   0        0        0      403 2023-05-23 13:15:32.484827 atproto-0.0.8/atproto/__init__.py
+-rw-r--r--   0        0        0     1782 2023-05-23 13:15:32.484996 atproto-0.0.8/atproto/car/__init__.py
+-rw-r--r--   0        0        0     2197 2023-05-23 13:22:55.691309 atproto-0.0.8/atproto/car/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1624 2023-05-23 13:15:32.485078 atproto-0.0.8/atproto/cbor/__init__.py
+-rw-r--r--   0        0        0     1994 2023-05-23 13:22:55.691917 atproto-0.0.8/atproto/cbor/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0       49 2023-05-23 13:15:32.485288 atproto-0.0.8/atproto/cid/__init__.py
+-rw-r--r--   0        0        0      204 2023-05-23 13:22:55.742052 atproto-0.0.8/atproto/cid/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0       23 2023-05-02 22:04:44.060240 atproto-0.0.8/atproto/cli/__init__.py
+-rw-r--r--   0        0        0      152 2023-05-02 22:59:20.005964 atproto-0.0.8/atproto/cli/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2790 2023-05-20 18:39:04.305255 atproto-0.0.8/atproto/codegen/__init__.py
+-rw-r--r--   0        0        0     4302 2023-05-20 20:49:49.138233 atproto-0.0.8/atproto/codegen/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2023-05-03 12:59:20.104132 atproto-0.0.8/atproto/codegen/clients/__init__.py
+-rw-r--r--   0        0        0      164 2023-05-05 12:23:15.495715 atproto-0.0.8/atproto/codegen/clients/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1391 2023-05-22 19:34:13.989736 atproto-0.0.8/atproto/codegen/clients/__pycache__/generate_async_client.cpython-38.pyc
+-rw-r--r--   0        0        0     1434 2023-05-20 18:39:04.305537 atproto-0.0.8/atproto/codegen/clients/generate_async_client.py
+-rw-r--r--   0        0        0        0 2023-04-30 12:18:23.051063 atproto-0.0.8/atproto/codegen/models/__init__.py
+-rw-r--r--   0        0        0      163 2023-04-30 12:30:22.568782 atproto-0.0.8/atproto/codegen/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2518 2023-05-23 11:57:59.553439 atproto-0.0.8/atproto/codegen/models/__pycache__/builder.cpython-38.pyc
+-rw-r--r--   0        0        0    14688 2023-05-23 12:00:06.207961 atproto-0.0.8/atproto/codegen/models/__pycache__/generator.cpython-38.pyc
+-rw-r--r--   0        0        0     2399 2023-05-23 13:15:32.485424 atproto-0.0.8/atproto/codegen/models/builder.py
+-rw-r--r--   0        0        0    19213 2023-05-23 11:58:55.694691 atproto-0.0.8/atproto/codegen/models/generator.py
+-rw-r--r--   0        0        0        0 2023-04-30 08:15:15.429281 atproto-0.0.8/atproto/codegen/namespaces/__init__.py
+-rw-r--r--   0        0        0      167 2023-04-30 08:20:07.529986 atproto-0.0.8/atproto/codegen/namespaces/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2558 2023-05-22 19:34:14.096893 atproto-0.0.8/atproto/codegen/namespaces/__pycache__/builder.cpython-38.pyc
+-rw-r--r--   0        0        0     9693 2023-05-22 19:34:14.131154 atproto-0.0.8/atproto/codegen/namespaces/__pycache__/generator.cpython-38.pyc
+-rw-r--r--   0        0        0     2546 2023-05-20 18:39:04.306557 atproto-0.0.8/atproto/codegen/namespaces/builder.py
+-rw-r--r--   0        0        0    11836 2023-05-20 18:39:04.306950 atproto-0.0.8/atproto/codegen/namespaces/generator.py
+-rw-r--r--   0        0        0      992 2023-05-23 13:15:32.485529 atproto-0.0.8/atproto/exceptions.py
+-rw-r--r--   0        0        0     4007 2023-05-23 13:15:32.485614 atproto-0.0.8/atproto/firehose/__init__.py
+-rw-r--r--   0        0        0     3806 2023-05-23 13:22:55.742964 atproto-0.0.8/atproto/firehose/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     7424 2023-05-23 13:22:55.744233 atproto-0.0.8/atproto/firehose/__pycache__/client.cpython-38.pyc
+-rw-r--r--   0        0        0     4554 2023-05-23 13:22:55.851186 atproto-0.0.8/atproto/firehose/__pycache__/models.cpython-38.pyc
+-rw-r--r--   0        0        0     8005 2023-05-23 13:15:32.485699 atproto-0.0.8/atproto/firehose/client.py
+-rw-r--r--   0        0        0     4183 2023-05-23 13:15:32.485777 atproto-0.0.8/atproto/firehose/models.py
+-rw-r--r--   0        0        0     2569 2023-05-16 20:35:11.473690 atproto-0.0.8/atproto/leb128/__init__.py
+-rw-r--r--   0        0        0     2927 2023-05-16 20:35:48.620471 atproto-0.0.8/atproto/leb128/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2023-04-26 20:41:49.793814 atproto-0.0.8/atproto/lexicon/__init__.py
+-rw-r--r--   0        0        0      156 2023-04-29 16:30:40.077258 atproto-0.0.8/atproto/lexicon/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     7282 2023-05-20 20:49:49.141577 atproto-0.0.8/atproto/lexicon/__pycache__/models.cpython-38.pyc
+-rw-r--r--   0        0        0     3335 2023-05-20 20:49:49.154049 atproto-0.0.8/atproto/lexicon/__pycache__/parser.cpython-38.pyc
+-rw-r--r--   0        0        0     4790 2023-05-20 18:39:04.307247 atproto-0.0.8/atproto/lexicon/models.py
+-rw-r--r--   0        0        0     3857 2023-05-20 18:39:04.307561 atproto-0.0.8/atproto/lexicon/parser.py
+-rw-r--r--   0        0        0     5295 2023-05-20 18:39:04.307762 atproto-0.0.8/atproto/nsid/__init__.py
+-rw-r--r--   0        0        0     5708 2023-05-20 19:17:15.545539 atproto-0.0.8/atproto/nsid/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3064 2023-05-20 18:39:04.307957 atproto-0.0.8/atproto/uri/__init__.py
+-rw-r--r--   0        0        0     3633 2023-05-20 19:17:15.546578 atproto-0.0.8/atproto/uri/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2023-05-06 15:48:51.267229 atproto-0.0.8/atproto/xrpc_client/__init__.py
+-rw-r--r--   0        0        0      160 2023-05-08 17:46:34.999146 atproto-0.0.8/atproto/xrpc_client/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4984 2023-05-23 13:22:55.907678 atproto-0.0.8/atproto/xrpc_client/__pycache__/request.cpython-38.pyc
+-rw-r--r--   0        0        0     6148 2023-05-08 17:39:02.582090 atproto-0.0.8/atproto/xrpc_client/client/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-03 13:15:19.009756 atproto-0.0.8/atproto/xrpc_client/client/__init__.py
+-rw-r--r--   0        0        0      167 2023-05-08 17:46:35.096665 atproto-0.0.8/atproto/xrpc_client/client/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     6807 2023-05-20 19:17:15.548179 atproto-0.0.8/atproto/xrpc_client/client/__pycache__/async_client.cpython-38.pyc
+-rw-r--r--   0        0        0      839 2023-05-08 17:46:35.100346 atproto-0.0.8/atproto/xrpc_client/client/__pycache__/async_raw.cpython-38.pyc
+-rw-r--r--   0        0        0      775 2023-05-20 19:17:15.561969 atproto-0.0.8/atproto/xrpc_client/client/__pycache__/auth.cpython-38.pyc
+-rw-r--r--   0        0        0     4045 2023-05-20 19:17:15.549217 atproto-0.0.8/atproto/xrpc_client/client/__pycache__/base.cpython-38.pyc
+-rw-r--r--   0        0        0     6647 2023-05-20 19:17:15.566661 atproto-0.0.8/atproto/xrpc_client/client/__pycache__/client.cpython-38.pyc
+-rw-r--r--   0        0        0      817 2023-05-08 17:46:35.203336 atproto-0.0.8/atproto/xrpc_client/client/__pycache__/raw.cpython-38.pyc
+-rw-r--r--   0        0        0     7596 2023-05-20 18:39:04.308304 atproto-0.0.8/atproto/xrpc_client/client/async_client.py
+-rw-r--r--   0        0        0      489 2023-05-06 15:38:34.659690 atproto-0.0.8/atproto/xrpc_client/client/async_raw.py
+-rw-r--r--   0        0        0      414 2023-05-20 18:39:04.308474 atproto-0.0.8/atproto/xrpc_client/client/auth.py
+-rw-r--r--   0        0        0     3748 2023-05-20 18:39:04.308652 atproto-0.0.8/atproto/xrpc_client/client/base.py
+-rw-r--r--   0        0        0     7105 2023-05-20 18:39:04.308906 atproto-0.0.8/atproto/xrpc_client/client/client.py
+-rw-r--r--   0        0        0       76 2023-05-19 20:21:30.527343 atproto-0.0.8/atproto/xrpc_client/client/methods_mixin/__init__.py
+-rw-r--r--   0        0        0      254 2023-05-19 20:21:35.021793 atproto-0.0.8/atproto/xrpc_client/client/methods_mixin/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1824 2023-05-20 19:17:15.561351 atproto-0.0.8/atproto/xrpc_client/client/methods_mixin/__pycache__/session.cpython-38.pyc
+-rw-r--r--   0        0        0     1311 2023-05-20 18:39:04.309222 atproto-0.0.8/atproto/xrpc_client/client/methods_mixin/session.py
+-rw-r--r--   0        0        0      469 2023-05-06 15:38:34.668321 atproto-0.0.8/atproto/xrpc_client/client/raw.py
+-rw-r--r--   0        0        0    12159 2023-05-23 12:20:32.652399 atproto-0.0.8/atproto/xrpc_client/models/__init__.py
+-rw-r--r--   0        0        0     7929 2023-05-23 12:20:37.588003 atproto-0.0.8/atproto/xrpc_client/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1252 2023-05-09 15:13:37.111548 atproto-0.0.8/atproto/xrpc_client/models/__pycache__/base.cpython-38.pyc
+-rw-r--r--   0        0        0     1198 2023-05-09 15:13:37.119249 atproto-0.0.8/atproto/xrpc_client/models/__pycache__/blob_ref.cpython-38.pyc
+-rw-r--r--   0        0        0      478 2023-05-23 13:22:55.904085 atproto-0.0.8/atproto/xrpc_client/models/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0        0        0      717 2023-05-23 12:20:37.797349 atproto-0.0.8/atproto/xrpc_client/models/__pycache__/type_conversion.cpython-38.pyc
+-rw-r--r--   0        0        0     3705 2023-05-23 13:22:55.900853 atproto-0.0.8/atproto/xrpc_client/models/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0      323 2023-05-23 12:20:32.232068 atproto-0.0.8/atproto/xrpc_client/models/app/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-23 12:20:37.588371 atproto-0.0.8/atproto/xrpc_client/models/app/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      323 2023-05-23 12:20:32.231687 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/__init__.py
+-rw-r--r--   0        0        0      176 2023-05-23 12:20:37.588657 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      323 2023-05-23 12:20:32.232219 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-23 12:20:37.588931 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3611 2023-05-23 12:47:54.117354 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/__pycache__/defs.cpython-38.pyc
+-rw-r--r--   0        0        0      904 2023-05-23 12:47:54.119984 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/__pycache__/get_preferences.cpython-38.pyc
+-rw-r--r--   0        0        0      746 2023-05-23 12:47:54.120520 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/__pycache__/get_profile.cpython-38.pyc
+-rw-r--r--   0        0        0      984 2023-05-23 12:47:54.120974 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/__pycache__/get_profiles.cpython-38.pyc
+-rw-r--r--   0        0        0     1074 2023-05-23 12:47:54.121541 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/__pycache__/get_suggestions.cpython-38.pyc
+-rw-r--r--   0        0        0      845 2023-05-23 12:47:54.122123 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/__pycache__/profile.cpython-38.pyc
+-rw-r--r--   0        0        0      667 2023-05-23 12:47:54.122856 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/__pycache__/put_preferences.cpython-38.pyc
+-rw-r--r--   0        0        0     1099 2023-05-23 12:47:54.123322 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/__pycache__/search_actors.cpython-38.pyc
+-rw-r--r--   0        0        0     1059 2023-05-23 12:47:54.123945 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/__pycache__/search_actors_typeahead.cpython-38.pyc
+-rw-r--r--   0        0        0     3804 2023-05-23 12:46:04.227082 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/defs.py
+-rw-r--r--   0        0        0      759 2023-05-23 12:46:04.188467 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/get_preferences.py
+-rw-r--r--   0        0        0      800 2023-05-23 12:46:04.122115 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/get_profile.py
+-rw-r--r--   0        0        0      819 2023-05-23 12:46:04.251683 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py
+-rw-r--r--   0        0        0      916 2023-05-23 12:46:04.134673 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py
+-rw-r--r--   0        0        0      846 2023-05-23 12:46:04.201050 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/profile.py
+-rw-r--r--   0        0        0      631 2023-05-23 12:46:04.221737 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/put_preferences.py
+-rw-r--r--   0        0        0      955 2023-05-23 12:46:04.230163 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/search_actors.py
+-rw-r--r--   0        0        0      884 2023-05-23 12:46:04.146020 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py
+-rw-r--r--   0        0        0      323 2023-05-23 12:20:32.260022 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-23 12:20:37.596347 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1693 2023-05-23 12:47:54.124803 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/__pycache__/external.cpython-38.pyc
+-rw-r--r--   0        0        0     1577 2023-05-23 12:47:54.126191 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/__pycache__/images.cpython-38.pyc
+-rw-r--r--   0        0        0     2296 2023-05-23 12:47:54.127319 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/__pycache__/record.cpython-38.pyc
+-rw-r--r--   0        0        0     1207 2023-05-23 12:47:54.128605 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/__pycache__/record_with_media.cpython-38.pyc
+-rw-r--r--   0        0        0     1561 2023-05-23 12:46:04.112166 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/external.py
+-rw-r--r--   0        0        0     1397 2023-05-23 12:46:04.137452 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/images.py
+-rw-r--r--   0        0        0     2260 2023-05-23 12:46:04.097432 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/record.py
+-rw-r--r--   0        0        0     1181 2023-05-23 12:46:04.150112 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py
+-rw-r--r--   0        0        0      323 2023-05-23 12:20:32.272327 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__init__.py
+-rw-r--r--   0        0        0      181 2023-05-23 12:20:37.606251 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5207 2023-05-23 12:47:54.130034 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/defs.cpython-38.pyc
+-rw-r--r--   0        0        0     1485 2023-05-23 13:22:55.861815 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/describe_feed_generator.cpython-38.pyc
+-rw-r--r--   0        0        0      976 2023-05-23 13:22:55.862696 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/generator.cpython-38.pyc
+-rw-r--r--   0        0        0     1086 2023-05-23 13:22:55.863299 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/get_actor_feeds.cpython-38.pyc
+-rw-r--r--   0        0        0     1084 2023-05-23 12:47:54.134744 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/get_author_feed.cpython-38.pyc
+-rw-r--r--   0        0        0     1063 2023-05-23 13:22:55.864301 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/get_feed.cpython-38.pyc
+-rw-r--r--   0        0        0      975 2023-05-23 13:22:55.864907 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/get_feed_generator.cpython-38.pyc
+-rw-r--r--   0        0        0      987 2023-05-23 13:22:55.865494 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/get_feed_generators.cpython-38.pyc
+-rw-r--r--   0        0        0     1092 2023-05-23 13:22:55.866062 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/get_feed_skeleton.cpython-38.pyc
+-rw-r--r--   0        0        0     1514 2023-05-23 12:47:54.137810 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/get_likes.cpython-38.pyc
+-rw-r--r--   0        0        0     1113 2023-05-23 12:47:54.138680 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/get_post_thread.cpython-38.pyc
+-rw-r--r--   0        0        0      955 2023-05-23 12:47:54.139271 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/get_posts.cpython-38.pyc
+-rw-r--r--   0        0        0     1163 2023-05-23 12:47:54.139877 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/get_reposted_by.cpython-38.pyc
+-rw-r--r--   0        0        0     1096 2023-05-23 12:47:54.140597 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/get_timeline.cpython-38.pyc
+-rw-r--r--   0        0        0      710 2023-05-23 12:47:54.141292 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/like.cpython-38.pyc
+-rw-r--r--   0        0        0     2316 2023-05-23 12:47:54.141934 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/post.cpython-38.pyc
+-rw-r--r--   0        0        0      716 2023-05-23 12:47:54.142986 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/repost.cpython-38.pyc
+-rw-r--r--   0        0        0     5618 2023-05-23 12:46:04.089600 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/defs.py
+-rw-r--r--   0        0        0     1290 2023-05-23 13:17:54.948947 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/describe_feed_generator.py
+-rw-r--r--   0        0        0      983 2023-05-23 13:17:54.949125 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/generator.py
+-rw-r--r--   0        0        0      937 2023-05-23 13:17:54.949233 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_actor_feeds.py
+-rw-r--r--   0        0        0      934 2023-05-23 12:46:04.164219 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py
+-rw-r--r--   0        0        0      920 2023-05-23 13:17:54.949348 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_feed.py
+-rw-r--r--   0        0        0      839 2023-05-23 13:17:54.949458 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_feed_generator.py
+-rw-r--r--   0        0        0      814 2023-05-23 13:17:54.949579 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_feed_generators.py
+-rw-r--r--   0        0        0      940 2023-05-23 13:17:54.949678 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_feed_skeleton.py
+-rw-r--r--   0        0        0     1305 2023-05-23 12:46:04.104935 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_likes.py
+-rw-r--r--   0        0        0      981 2023-05-23 12:46:04.086841 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py
+-rw-r--r--   0        0        0      789 2023-05-23 12:46:04.085794 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_posts.py
+-rw-r--r--   0        0        0     1047 2023-05-23 12:46:04.207862 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py
+-rw-r--r--   0        0        0      957 2023-05-23 12:46:04.228584 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py
+-rw-r--r--   0        0        0      684 2023-05-23 12:46:04.219385 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/like.py
+-rw-r--r--   0        0        0     2205 2023-05-23 12:46:04.131722 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/post.py
+-rw-r--r--   0        0        0      688 2023-05-23 12:46:04.115640 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/repost.py
+-rw-r--r--   0        0        0      323 2023-05-23 12:20:32.297829 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-23 12:20:37.678553 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      629 2023-05-23 12:47:54.143669 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/block.cpython-38.pyc
+-rw-r--r--   0        0        0     2132 2023-05-23 12:47:54.144265 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/defs.cpython-38.pyc
+-rw-r--r--   0        0        0      632 2023-05-23 12:47:54.145318 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/follow.cpython-38.pyc
+-rw-r--r--   0        0        0     1059 2023-05-23 12:47:54.145814 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/get_blocks.cpython-38.pyc
+-rw-r--r--   0        0        0     1107 2023-05-23 12:47:54.146456 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/get_followers.cpython-38.pyc
+-rw-r--r--   0        0        0     1099 2023-05-23 12:47:54.147131 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/get_follows.cpython-38.pyc
+-rw-r--r--   0        0        0     1118 2023-05-23 12:47:54.147750 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/get_list.cpython-38.pyc
+-rw-r--r--   0        0        0     1065 2023-05-23 12:47:54.148387 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/get_list_mutes.cpython-38.pyc
+-rw-r--r--   0        0        0     1069 2023-05-23 12:47:54.148995 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/get_lists.cpython-38.pyc
+-rw-r--r--   0        0        0     1055 2023-05-23 12:47:54.149567 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/get_mutes.cpython-38.pyc
+-rw-r--r--   0        0        0      998 2023-05-23 12:47:54.150896 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/list.cpython-38.pyc
+-rw-r--r--   0        0        0      654 2023-05-23 12:47:54.151492 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/listitem.cpython-38.pyc
+-rw-r--r--   0        0        0      569 2023-05-23 12:47:54.152006 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/mute_actor.cpython-38.pyc
+-rw-r--r--   0        0        0      577 2023-05-23 12:47:54.152434 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/mute_actor_list.cpython-38.pyc
+-rw-r--r--   0        0        0      573 2023-05-23 12:47:54.152846 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/unmute_actor.cpython-38.pyc
+-rw-r--r--   0        0        0      581 2023-05-23 12:47:54.153246 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/unmute_actor_list.cpython-38.pyc
+-rw-r--r--   0        0        0      615 2023-05-23 12:46:04.220606 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/block.py
+-rw-r--r--   0        0        0     2141 2023-05-23 12:46:04.152826 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/defs.py
+-rw-r--r--   0        0        0      617 2023-05-23 12:46:04.091787 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/follow.py
+-rw-r--r--   0        0        0      906 2023-05-23 12:46:04.212768 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py
+-rw-r--r--   0        0        0     1008 2023-05-23 12:46:04.222871 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/get_followers.py
+-rw-r--r--   0        0        0     1000 2023-05-23 12:46:04.247615 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/get_follows.py
+-rw-r--r--   0        0        0      980 2023-05-23 12:46:04.143128 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/get_list.py
+-rw-r--r--   0        0        0      907 2023-05-23 12:46:04.217992 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/get_list_mutes.py
+-rw-r--r--   0        0        0      925 2023-05-23 12:46:04.171102 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/get_lists.py
+-rw-r--r--   0        0        0      902 2023-05-23 12:46:04.183851 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py
+-rw-r--r--   0        0        0     1002 2023-05-23 12:46:04.238659 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/list.py
+-rw-r--r--   0        0        0      645 2023-05-23 12:46:04.113819 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/listitem.py
+-rw-r--r--   0        0        0      541 2023-05-23 12:46:04.202067 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py
+-rw-r--r--   0        0        0      543 2023-05-23 12:46:04.128157 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/mute_actor_list.py
+-rw-r--r--   0        0        0      543 2023-05-23 12:46:04.174592 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py
+-rw-r--r--   0        0        0      545 2023-05-23 12:46:04.144595 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/unmute_actor_list.py
+-rw-r--r--   0        0        0      323 2023-05-23 12:20:32.313012 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/notification/__init__.py
+-rw-r--r--   0        0        0      189 2023-05-23 12:20:37.700822 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/notification/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      919 2023-05-23 12:47:54.153845 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/notification/__pycache__/get_unread_count.cpython-38.pyc
+-rw-r--r--   0        0        0     1811 2023-05-23 12:47:54.154456 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/notification/__pycache__/list_notifications.cpython-38.pyc
+-rw-r--r--   0        0        0      586 2023-05-23 12:47:54.155305 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/notification/__pycache__/update_seen.cpython-38.pyc
+-rw-r--r--   0        0        0      756 2023-05-23 12:46:04.126657 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py
+-rw-r--r--   0        0        0     1689 2023-05-23 12:46:04.199564 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py
+-rw-r--r--   0        0        0      552 2023-05-23 12:46:04.248985 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/notification/update_seen.py
+-rw-r--r--   0        0        0      323 2023-05-23 12:20:32.313862 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/richtext/__init__.py
+-rw-r--r--   0        0        0      185 2023-05-23 12:20:37.704189 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/richtext/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1891 2023-05-23 12:47:54.155915 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/richtext/__pycache__/facet.cpython-38.pyc
+-rw-r--r--   0        0        0     1575 2023-05-23 12:46:04.215466 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/richtext/facet.py
+-rw-r--r--   0        0        0      323 2023-05-23 12:20:32.314175 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/unspecced/__init__.py
+-rw-r--r--   0        0        0      186 2023-05-23 12:20:37.705487 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/unspecced/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1116 2023-05-23 12:47:54.156950 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/unspecced/__pycache__/get_popular.cpython-38.pyc
+-rw-r--r--   0        0        0      971 2023-05-23 12:46:04.210357 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py
+-rw-r--r--   0        0        0      553 2023-05-08 18:09:02.748635 atproto-0.0.8/atproto/xrpc_client/models/base.py
+-rw-r--r--   0        0        0      713 2023-05-08 17:32:37.842360 atproto-0.0.8/atproto/xrpc_client/models/blob_ref.py
+-rw-r--r--   0        0        0      323 2023-05-23 12:20:32.314490 atproto-0.0.8/atproto/xrpc_client/models/com/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-23 12:20:37.706508 atproto-0.0.8/atproto/xrpc_client/models/com/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      323 2023-05-23 12:20:32.315041 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/__init__.py
+-rw-r--r--   0        0        0      179 2023-05-23 12:20:37.706817 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      323 2023-05-23 12:20:32.314977 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__init__.py
+-rw-r--r--   0        0        0      185 2023-05-23 12:20:37.707109 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     7982 2023-05-23 12:47:54.158814 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/defs.cpython-38.pyc
+-rw-r--r--   0        0        0      602 2023-05-23 12:47:54.162735 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/disable_account_invites.cpython-38.pyc
+-rw-r--r--   0        0        0      698 2023-05-23 12:47:54.163183 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/disable_invite_codes.cpython-38.pyc
+-rw-r--r--   0        0        0      600 2023-05-23 12:47:54.163668 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/enable_account_invites.cpython-38.pyc
+-rw-r--r--   0        0        0     1117 2023-05-23 12:47:54.164126 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/get_invite_codes.cpython-38.pyc
+-rw-r--r--   0        0        0      768 2023-05-23 12:47:54.164829 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/get_moderation_action.cpython-38.pyc
+-rw-r--r--   0        0        0     1139 2023-05-23 12:47:54.165341 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/get_moderation_actions.cpython-38.pyc
+-rw-r--r--   0        0        0      768 2023-05-23 12:47:54.166203 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/get_moderation_report.cpython-38.pyc
+-rw-r--r--   0        0        0     1217 2023-05-23 12:47:54.166807 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/get_moderation_reports.cpython-38.pyc
+-rw-r--r--   0        0        0      793 2023-05-23 12:47:54.167491 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/get_record.cpython-38.pyc
+-rw-r--r--   0        0        0      742 2023-05-23 12:47:54.167957 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/get_repo.cpython-38.pyc
+-rw-r--r--   0        0        0      838 2023-05-23 12:47:54.168422 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/resolve_moderation_reports.cpython-38.pyc
+-rw-r--r--   0        0        0      810 2023-05-23 12:47:54.168928 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/reverse_moderation_action.cpython-38.pyc
+-rw-r--r--   0        0        0     1140 2023-05-23 12:47:54.169453 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/search_repos.cpython-38.pyc
+-rw-r--r--   0        0        0     1099 2023-05-23 12:47:54.170110 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/take_moderation_action.cpython-38.pyc
+-rw-r--r--   0        0        0      613 2023-05-23 12:47:54.170659 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/update_account_email.cpython-38.pyc
+-rw-r--r--   0        0        0      612 2023-05-23 12:47:54.171078 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/update_account_handle.cpython-38.pyc
+-rw-r--r--   0        0        0     9308 2023-05-23 12:46:04.244397 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/defs.py
+-rw-r--r--   0        0        0      560 2023-05-23 12:46:04.167950 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/disable_account_invites.py
+-rw-r--r--   0        0        0      658 2023-05-23 12:46:04.241323 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py
+-rw-r--r--   0        0        0      559 2023-05-23 12:46:04.140269 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/enable_account_invites.py
+-rw-r--r--   0        0        0      966 2023-05-23 12:46:04.082872 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py
+-rw-r--r--   0        0        0      806 2023-05-23 12:46:04.081875 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py
+-rw-r--r--   0        0        0      987 2023-05-23 12:46:04.246013 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py
+-rw-r--r--   0        0        0      806 2023-05-23 12:46:04.214076 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py
+-rw-r--r--   0        0        0     1095 2023-05-23 12:46:04.118692 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py
+-rw-r--r--   0        0        0      839 2023-05-23 12:46:04.240049 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_record.py
+-rw-r--r--   0        0        0      790 2023-05-23 12:46:04.083804 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_repo.py
+-rw-r--r--   0        0        0      880 2023-05-23 12:46:04.095464 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py
+-rw-r--r--   0        0        0      851 2023-05-23 12:46:04.232996 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py
+-rw-r--r--   0        0        0     1011 2023-05-23 12:46:04.099316 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/search_repos.py
+-rw-r--r--   0        0        0     1228 2023-05-23 12:46:04.100698 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py
+-rw-r--r--   0        0        0      605 2023-05-23 12:46:04.103528 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py
+-rw-r--r--   0        0        0      578 2023-05-23 12:46:04.176127 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py
+-rw-r--r--   0        0        0      323 2023-05-23 12:20:32.328520 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/identity/__init__.py
+-rw-r--r--   0        0        0      188 2023-05-23 12:20:37.720719 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/identity/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      910 2023-05-23 12:47:54.171703 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/identity/__pycache__/resolve_handle.cpython-38.pyc
+-rw-r--r--   0        0        0      588 2023-05-23 12:47:54.172262 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/identity/__pycache__/update_handle.cpython-38.pyc
+-rw-r--r--   0        0        0      815 2023-05-23 12:46:04.096343 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py
+-rw-r--r--   0        0        0      552 2023-05-23 12:46:04.235698 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/identity/update_handle.py
+-rw-r--r--   0        0        0      323 2023-05-23 12:20:32.330357 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/label/__init__.py
+-rw-r--r--   0        0        0      185 2023-05-23 12:20:37.722558 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/label/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      825 2023-05-23 12:47:54.172849 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/label/__pycache__/defs.cpython-38.pyc
+-rw-r--r--   0        0        0     1149 2023-05-23 12:47:54.173445 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/label/__pycache__/query_labels.cpython-38.pyc
+-rw-r--r--   0        0        0     1455 2023-05-23 13:22:55.885962 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/label/__pycache__/subscribe_labels.cpython-38.pyc
+-rw-r--r--   0        0        0     1173 2023-05-23 12:46:04.206598 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/label/defs.py
+-rw-r--r--   0        0        0     1215 2023-05-23 12:46:04.216799 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/label/query_labels.py
+-rw-r--r--   0        0        0     1214 2023-05-23 13:15:32.486009 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py
+-rw-r--r--   0        0        0      323 2023-05-23 12:20:32.331439 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/moderation/__init__.py
+-rw-r--r--   0        0        0      190 2023-05-23 12:20:37.725149 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/moderation/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1298 2023-05-23 12:47:54.175004 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/moderation/__pycache__/create_report.cpython-38.pyc
+-rw-r--r--   0        0        0      631 2023-05-23 12:47:54.175705 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/moderation/__pycache__/defs.cpython-38.pyc
+-rw-r--r--   0        0        0     1351 2023-05-23 12:46:04.080807 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/moderation/create_report.py
+-rw-r--r--   0        0        0      845 2023-05-23 12:46:04.148689 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/moderation/defs.py
+-rw-r--r--   0        0        0      323 2023-05-23 12:20:32.331744 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/__init__.py
+-rw-r--r--   0        0        0      184 2023-05-23 12:20:37.726858 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2023 2023-05-23 12:47:54.176304 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/__pycache__/apply_writes.cpython-38.pyc
+-rw-r--r--   0        0        0     1060 2023-05-23 12:47:54.177292 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/__pycache__/create_record.cpython-38.pyc
+-rw-r--r--   0        0        0      726 2023-05-23 12:47:54.177928 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/__pycache__/delete_record.cpython-38.pyc
+-rw-r--r--   0        0        0      994 2023-05-23 12:47:54.178471 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/__pycache__/describe_repo.cpython-38.pyc
+-rw-r--r--   0        0        0      980 2023-05-23 12:47:54.179077 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/__pycache__/get_record.cpython-38.pyc
+-rw-r--r--   0        0        0     1589 2023-05-23 12:47:54.179796 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/__pycache__/list_records.cpython-38.pyc
+-rw-r--r--   0        0        0     1073 2023-05-23 12:47:54.180837 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/__pycache__/put_record.cpython-38.pyc
+-rw-r--r--   0        0        0      647 2023-05-23 12:47:54.181593 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/__pycache__/rebase_repo.cpython-38.pyc
+-rw-r--r--   0        0        0      636 2023-05-23 12:47:54.182047 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/__pycache__/strong_ref.cpython-38.pyc
+-rw-r--r--   0        0        0      752 2023-05-23 12:47:54.182530 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/__pycache__/upload_blob.cpython-38.pyc
+-rw-r--r--   0        0        0     1881 2023-05-23 12:46:04.141752 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py
+-rw-r--r--   0        0        0     1093 2023-05-23 12:46:04.094591 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/create_record.py
+-rw-r--r--   0        0        0      874 2023-05-23 12:46:04.093696 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/delete_record.py
+-rw-r--r--   0        0        0      910 2023-05-23 12:46:04.254360 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py
+-rw-r--r--   0        0        0     1062 2023-05-23 12:46:04.211615 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/get_record.py
+-rw-r--r--   0        0        0     1606 2023-05-23 12:46:04.172805 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/list_records.py
+-rw-r--r--   0        0        0     1160 2023-05-23 12:46:04.203673 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/put_record.py
+-rw-r--r--   0        0        0      679 2023-05-23 12:46:04.151464 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/rebase_repo.py
+-rw-r--r--   0        0        0      604 2023-05-23 12:46:04.075614 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py
+-rw-r--r--   0        0        0      704 2023-05-23 12:46:04.182163 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py
+-rw-r--r--   0        0        0      323 2023-05-23 12:20:32.342245 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__init__.py
+-rw-r--r--   0        0        0      186 2023-05-23 12:20:37.744700 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1085 2023-05-23 12:47:54.183210 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/create_account.cpython-38.pyc
+-rw-r--r--   0        0        0     1045 2023-05-23 12:47:54.183907 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/create_app_password.cpython-38.pyc
+-rw-r--r--   0        0        0      940 2023-05-23 12:47:54.184499 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/create_invite_code.cpython-38.pyc
+-rw-r--r--   0        0        0     1468 2023-05-23 12:47:54.185098 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/create_invite_codes.cpython-38.pyc
+-rw-r--r--   0        0        0     1002 2023-05-23 12:47:54.186183 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/create_session.cpython-38.pyc
+-rw-r--r--   0        0        0     1166 2023-05-23 12:47:54.187083 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/defs.cpython-38.pyc
+-rw-r--r--   0        0        0      620 2023-05-23 12:47:54.187985 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/delete_account.cpython-38.pyc
+-rw-r--r--   0        0        0      192 2023-05-23 12:47:54.188563 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/delete_session.cpython-38.pyc
+-rw-r--r--   0        0        0     1232 2023-05-23 12:47:54.189086 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/describe_server.cpython-38.pyc
+-rw-r--r--   0        0        0     1082 2023-05-23 12:47:54.189898 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/get_account_invite_codes.cpython-38.pyc
+-rw-r--r--   0        0        0      672 2023-05-23 12:47:54.190616 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/get_session.cpython-38.pyc
+-rw-r--r--   0        0        0     1098 2023-05-23 12:47:54.191147 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/list_app_passwords.cpython-38.pyc
+-rw-r--r--   0        0        0      655 2023-05-23 12:47:54.191788 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/refresh_session.cpython-38.pyc
+-rw-r--r--   0        0        0      200 2023-05-23 12:47:54.192255 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/request_account_delete.cpython-38.pyc
+-rw-r--r--   0        0        0      600 2023-05-23 12:47:54.192577 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/request_password_reset.cpython-38.pyc
+-rw-r--r--   0        0        0      605 2023-05-23 12:47:54.192992 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/reset_password.cpython-38.pyc
+-rw-r--r--   0        0        0      593 2023-05-23 12:47:54.193444 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/revoke_app_password.cpython-38.pyc
+-rw-r--r--   0        0        0     1033 2023-05-23 12:46:04.138659 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/create_account.py
+-rw-r--r--   0        0        0      956 2023-05-23 12:46:04.231476 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/create_app_password.py
+-rw-r--r--   0        0        0      789 2023-05-23 12:46:04.084741 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py
+-rw-r--r--   0        0        0     1198 2023-05-23 12:46:04.192606 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py
+-rw-r--r--   0        0        0      973 2023-05-23 12:46:04.107533 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/create_session.py
+-rw-r--r--   0        0        0     1130 2023-05-23 12:46:04.129873 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/defs.py
+-rw-r--r--   0        0        0      603 2023-05-23 12:46:04.180564 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/delete_account.py
+-rw-r--r--   0        0        0      323 2023-05-23 12:46:15.959008 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/delete_session.py
+-rw-r--r--   0        0        0     1122 2023-05-23 12:46:04.077798 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/describe_server.py
+-rw-r--r--   0        0        0      926 2023-05-23 12:46:04.189870 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py
+-rw-r--r--   0        0        0      643 2023-05-23 12:46:04.079399 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/get_session.py
+-rw-r--r--   0        0        0      937 2023-05-23 12:46:04.147249 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py
+-rw-r--r--   0        0        0      655 2023-05-23 12:46:04.123826 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/refresh_session.py
+-rw-r--r--   0        0        0      323 2023-05-23 12:46:15.959972 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/request_account_delete.py
+-rw-r--r--   0        0        0      556 2023-05-23 12:46:04.196601 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py
+-rw-r--r--   0        0        0      581 2023-05-23 12:46:04.186742 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/reset_password.py
+-rw-r--r--   0        0        0      551 2023-05-23 12:46:04.209154 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py
+-rw-r--r--   0        0        0      323 2023-05-23 12:20:32.352400 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__init__.py
+-rw-r--r--   0        0        0      184 2023-05-23 12:20:37.764138 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      692 2023-05-23 12:47:54.194174 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/get_blob.cpython-38.pyc
+-rw-r--r--   0        0        0      714 2023-05-23 12:47:54.194706 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/get_blocks.cpython-38.pyc
+-rw-r--r--   0        0        0      733 2023-05-23 12:47:54.195227 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/get_checkout.cpython-38.pyc
+-rw-r--r--   0        0        0      970 2023-05-23 12:47:54.195765 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/get_commit_path.cpython-38.pyc
+-rw-r--r--   0        0        0      800 2023-05-23 12:47:54.196414 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/get_head.cpython-38.pyc
+-rw-r--r--   0        0        0      767 2023-05-23 12:47:54.196929 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/get_record.cpython-38.pyc
+-rw-r--r--   0        0        0      760 2023-05-23 12:47:54.197422 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/get_repo.cpython-38.pyc
+-rw-r--r--   0        0        0      954 2023-05-23 12:47:54.197919 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/list_blobs.cpython-38.pyc
+-rw-r--r--   0        0        0     1383 2023-05-23 12:47:54.198584 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/list_repos.cpython-38.pyc
+-rw-r--r--   0        0        0      591 2023-05-23 12:47:54.199365 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/notify_of_update.cpython-38.pyc
+-rw-r--r--   0        0        0      586 2023-05-23 12:47:54.199850 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/request_crawl.cpython-38.pyc
+-rw-r--r--   0        0        0     2877 2023-05-23 13:22:55.899006 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/subscribe_repos.cpython-38.pyc
+-rw-r--r--   0        0        0      706 2023-05-23 12:46:04.179091 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_blob.py
+-rw-r--r--   0        0        0      693 2023-05-23 12:46:04.109156 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py
+-rw-r--r--   0        0        0      765 2023-05-23 12:46:04.205112 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py
+-rw-r--r--   0        0        0      885 2023-05-23 12:46:04.198103 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py
+-rw-r--r--   0        0        0      701 2023-05-23 12:46:04.136114 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_head.py
+-rw-r--r--   0        0        0      789 2023-05-23 12:46:04.165888 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_record.py
+-rw-r--r--   0        0        0      847 2023-05-23 12:46:04.253097 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_repo.py
+-rw-r--r--   0        0        0      871 2023-05-23 12:46:04.156294 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py
+-rw-r--r--   0        0        0     1115 2023-05-23 12:46:04.162464 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/list_repos.py
+-rw-r--r--   0        0        0      601 2023-05-23 12:46:04.237162 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py
+-rw-r--r--   0        0        0      604 2023-05-23 12:46:04.090802 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py
+-rw-r--r--   0        0        0     2604 2023-05-23 13:15:32.486216 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py
+-rw-r--r--   0        0        0      134 2023-05-23 13:15:32.486276 atproto-0.0.8/atproto/xrpc_client/models/common.py
+-rw-r--r--   0        0        0      612 2023-05-23 12:20:32.363606 atproto-0.0.8/atproto/xrpc_client/models/type_conversion.py
+-rw-r--r--   0        0        0     3409 2023-05-23 13:15:32.486395 atproto-0.0.8/atproto/xrpc_client/models/utils.py
+-rw-r--r--   0        0        0     6148 2023-05-08 17:39:09.891512 atproto-0.0.8/atproto/xrpc_client/namespaces/.DS_Store
+-rw-r--r--   0        0        0        0 2023-04-30 08:01:01.985340 atproto-0.0.8/atproto/xrpc_client/namespaces/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-08 17:46:35.193604 atproto-0.0.8/atproto/xrpc_client/namespaces/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    69598 2023-05-23 12:47:54.250370 atproto-0.0.8/atproto/xrpc_client/namespaces/__pycache__/async_ns.cpython-38.pyc
+-rw-r--r--   0        0        0      801 2023-05-20 19:17:15.556274 atproto-0.0.8/atproto/xrpc_client/namespaces/__pycache__/base.cpython-38.pyc
+-rw-r--r--   0        0        0    68949 2023-05-23 12:47:54.264516 atproto-0.0.8/atproto/xrpc_client/namespaces/__pycache__/sync_ns.cpython-38.pyc
+-rw-r--r--   0        0        0    78721 2023-05-23 12:20:40.627807 atproto-0.0.8/atproto/xrpc_client/namespaces/async_ns.py
+-rw-r--r--   0        0        0      344 2023-05-20 18:39:04.327872 atproto-0.0.8/atproto/xrpc_client/namespaces/base.py
+-rw-r--r--   0        0        0    77605 2023-05-23 12:20:40.580068 atproto-0.0.8/atproto/xrpc_client/namespaces/sync_ns.py
+-rw-r--r--   0        0        0     4320 2023-05-23 13:15:32.486526 atproto-0.0.8/atproto/xrpc_client/request.py
+-rw-r--r--   0        0        0       43 2023-05-05 12:44:22.361781 atproto-0.0.8/atproto/xrpc_server/__init__.py
+-rw-r--r--   0        0        0      160 2023-05-05 12:44:59.992820 atproto-0.0.8/atproto/xrpc_server/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2424 2023-05-23 13:37:26.068244 atproto-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    11529 1970-01-01 00:00:00.000000 atproto-0.0.8/PKG-INFO
```

### Comparing `atproto-0.0.7/LICENSE` & `atproto-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `atproto-0.0.7/README.md` & `atproto-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     <a href="https://discord.gg/PCyVJXU9jN">
         Discord Bluesky API
     </a>
 </p>
 
 ## The AT Protocol SDK
 
-> ⚠️ Under construction. The SDK was built from scratch in 40 hours. Somewhere I speedran. I have a list of things that will break backward compatibility. Until the 1.0.0 release, I am not going to care about it. 
+> ⚠️ Under construction. Until the 1.0.0 release, I am not going to care about backward compatibility between versions. 
 
 Code snippet:
 ```python
 from atproto import Client
 
 
 def main():
@@ -62,17 +62,19 @@
 if __name__ == '__main__':
     # use run() for higher Python version
     asyncio.get_event_loop().run_until_complete(main())
 
 ```
 </details>
 
+🔥[Firehose data streaming is available!](https://atproto.blue/en/latest/firehose.html)
+
 ### Introduction
 
-This SDK attempts to implement everything that provides ATProto. Due to the unstable state of the protocol (it grows and changes fast) and a bit of outdated documentation, only the client side is supported yet. There is support for Lexicon Schemes and XRPC clients for now. All models, queries, and procedures are generated automatically. The main focus is on the lexicons of atproto.com and bsky.app, but it doesn't have a vendor lock on it. Feel free to use the code generator for your own lexicon schemes. SDK also provides utilities to work with CID, NSID, URI. The support of IPLD (dag-cbor) will be added in the near future.
+This SDK attempts to implement everything that provides ATProto. Due to the unstable state of the protocol (it grows and changes fast) and a bit of outdated documentation, only the client side is supported yet. There is support for Lexicon Schemes, XRPC clients and Firehose for now. All models, queries, and procedures are generated automatically. The main focus is on the lexicons of atproto.com and bsky.app, but it doesn't have a vendor lock on it. Feel free to use the code generator for your own lexicon schemes. SDK also provides utilities to work with CID, NSID, AT URI Scheme. DAG-CBOR, CAR files.
 
 ### Requirements
 
 - Python 3.7 or higher.
 - Access to Bsky if you don't have own server.
 
 ### Installing
@@ -140,15 +142,15 @@
 The documentation is live at [atproto.blue](https://atproto.blue/).
 
 ### Getting help
 
 You can get help in several ways:
 - Report bugs, request new features by [creating an issue](https://github.com/MarshalX/atproto/issues/new).
 - Ask questions by [starting a discussion](https://github.com/MarshalX/atproto/discussions/new).
-- Ask questions in [Discord server](https://discord.gg/ZDMSm3UGPN).
+- Ask questions in [Discord server](https://discord.gg/PCyVJXU9jN).
 
 ### Advanced usage
 
 I'll be honest. The high-level Client that was shown in the "Quick Start" section is not a real ATProto API. It's syntax sugar built upon the real XRPC methods! The high-level methods are not cover the full need of developers. To be able to do anything that you want you should know to work with low-level API. Let's dive into it!
 
 The basics:
 - Namespaces – classes that group sub-namespaces and the XRPC queries and procedures. Built upon NSID ATProto semantic.
```

### Comparing `atproto-0.0.7/atproto/codegen/__init__.py` & `atproto-0.0.8/atproto/codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.7/atproto/codegen/clients/generate_async_client.py` & `atproto-0.0.8/atproto/codegen/clients/generate_async_client.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.7/atproto/codegen/models/builder.py` & `atproto-0.0.8/atproto/codegen/models/builder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import typing as t
 
 from atproto.lexicon import models
 from atproto.lexicon.parser import lexicon_parse_dir
 from atproto.nsid import NSID
 
-_LEX_DEF_TYPES_FOR_PARAMS = {models.LexDefinitionType.QUERY, models.LexDefinitionType.PROCEDURE}
+_LEX_DEF_TYPES_FOR_PARAMS = {
+    models.LexDefinitionType.QUERY,
+    models.LexDefinitionType.PROCEDURE,
+    models.LexDefinitionType.SUBSCRIPTION,
+}
 _LEX_DEF_TYPES_FOR_RESPONSES = {models.LexDefinitionType.QUERY, models.LexDefinitionType.PROCEDURE}
 _LEX_DEF_TYPES_FOR_REFS = {models.LexDefinitionType.QUERY, models.LexDefinitionType.PROCEDURE}
 _LEX_DEF_TYPES_FOR_DATA = {models.LexDefinitionType.PROCEDURE}
 _LEX_DEF_TYPES_FOR_RECORDS = {models.LexDefinitionType.RECORD}
 _LEX_DEF_TYPES_FOR_DEF = {
     models.LexDefinitionType.OBJECT,
     models.LexPrimitiveType.STRING,
```

### Comparing `atproto-0.0.7/atproto/codegen/models/generator.py` & `atproto-0.0.8/atproto/codegen/models/generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -200,48 +200,48 @@
     if hasattr(lex_obj, 'nullable') and lex_obj.nullable:
         # TODO(MarshalX): not 100% the same thing. think about it
         required_fields = required_fields.difference(set(lex_obj.nullable))
 
     return required_fields
 
 
+def _get_field_docstring(field_name: str, field_type) -> str:
+    field_desc = field_type.description
+    if field_desc is None:
+        field_desc = gen_description_by_camel_case_name(field_name)
+    if field_desc[-1] not in {'.', '?', '!'}:
+        field_desc += '.'
+
+    return field_desc
+
+
 def _get_model_docstring(
     nsid: t.Union[str, NSID], lex_object: t.Union[models.LexObject, models.LexXrpcParameters], model_type: ModelType
 ) -> str:
     model_desc = lex_object.description or ''
     model_desc = f"{model_type.value} model for :obj:`{nsid}`. {model_desc}"
 
-    doc_string = [f'{_(1)}"""{model_desc}', '', f'{_(1)}Attributes:']
-
-    for field_name, field_type in lex_object.properties.items():
-        field_desc = field_type.description
-        if field_desc is None:
-            field_desc = gen_description_by_camel_case_name(field_name)
-        if field_desc[-1] not in {'.', '?', '!'}:
-            field_desc += '.'
-
-        doc_string.append(f'{_(2)}{field_name}: {field_desc}')
-
-    doc_string.append(f'{_(1)}"""')
-    doc_string.append('')
+    doc_string = [f'{_(1)}"""{model_desc}"""', '']
 
     return join_code(doc_string)
 
 
 def _get_model(nsid: NSID, lex_object: t.Union[models.LexObject, models.LexXrpcParameters]) -> str:
     required_fields = _get_req_fields_set(lex_object)
 
     fields = []
     optional_fields = []
 
     for field_name, field_type in lex_object.properties.items():
         is_optional = field_name not in required_fields
         type_hint = _get_model_field_typehint(nsid, field_name, field_type, optional=is_optional)
+        description = _get_field_docstring(field_name, field_type)
 
-        field_def = f'{_(1)}{field_name}: {type_hint}'  # TODO(MarshalX): Add default values. for bool, etc..
+        # TODO(MarshalX): Add default values. for bool, etc..
+        field_def = f'{_(1)}{field_name}: {type_hint} #: {description}'
         if is_optional:
             optional_fields.append(field_def)
         else:
             fields.append(field_def)
 
     optional_fields.sort()
     fields.sort()
```

### Comparing `atproto-0.0.7/atproto/codegen/namespaces/builder.py` & `atproto-0.0.8/atproto/codegen/namespaces/builder.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.7/atproto/codegen/namespaces/generator.py` & `atproto-0.0.8/atproto/codegen/namespaces/generator.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.7/atproto/exceptions.py` & `atproto-0.0.8/atproto/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -61,7 +61,11 @@
 
 class BadRequestError(RequestException):
     ...
 
 
 class InvalidAtUriError(AtProtocolError):
     ...
+
+
+class FirehoseError(AtProtocolError):
+    ...
```

### Comparing `atproto-0.0.7/atproto/leb128/__init__.py` & `atproto-0.0.8/atproto/leb128/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.7/atproto/lexicon/models.py` & `atproto-0.0.8/atproto/lexicon/models.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.7/atproto/lexicon/parser.py` & `atproto-0.0.8/atproto/lexicon/parser.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.7/atproto/nsid/__init__.py` & `atproto-0.0.8/atproto/nsid/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.7/atproto/uri/__init__.py` & `atproto-0.0.8/atproto/uri/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.7/atproto/xrpc_client/client/async_client.py` & `atproto-0.0.8/atproto/xrpc_client/client/async_client.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.7/atproto/xrpc_client/client/base.py` & `atproto-0.0.8/atproto/xrpc_client/client/base.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.7/atproto/xrpc_client/client/client.py` & `atproto-0.0.8/atproto/xrpc_client/client/client.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.7/atproto/xrpc_client/client/methods_mixin/session.py` & `atproto-0.0.8/atproto/xrpc_client/client/methods_mixin/session.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/__init__.py` & `atproto-0.0.8/atproto/xrpc_client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,33 @@
 from atproto.xrpc_client.models.app.bsky.embed import images as AppBskyEmbedImages
 from atproto.xrpc_client.models.app.bsky.embed import record as AppBskyEmbedRecord
 from atproto.xrpc_client.models.app.bsky.embed import (
     record_with_media as AppBskyEmbedRecordWithMedia,
 )
 from atproto.xrpc_client.models.app.bsky.feed import defs as AppBskyFeedDefs
 from atproto.xrpc_client.models.app.bsky.feed import (
+    describe_feed_generator as AppBskyFeedDescribeFeedGenerator,
+)
+from atproto.xrpc_client.models.app.bsky.feed import generator as AppBskyFeedGenerator
+from atproto.xrpc_client.models.app.bsky.feed import (
+    get_actor_feeds as AppBskyFeedGetActorFeeds,
+)
+from atproto.xrpc_client.models.app.bsky.feed import (
     get_author_feed as AppBskyFeedGetAuthorFeed,
 )
+from atproto.xrpc_client.models.app.bsky.feed import get_feed as AppBskyFeedGetFeed
+from atproto.xrpc_client.models.app.bsky.feed import (
+    get_feed_generator as AppBskyFeedGetFeedGenerator,
+)
+from atproto.xrpc_client.models.app.bsky.feed import (
+    get_feed_generators as AppBskyFeedGetFeedGenerators,
+)
+from atproto.xrpc_client.models.app.bsky.feed import (
+    get_feed_skeleton as AppBskyFeedGetFeedSkeleton,
+)
 from atproto.xrpc_client.models.app.bsky.feed import get_likes as AppBskyFeedGetLikes
 from atproto.xrpc_client.models.app.bsky.feed import (
     get_post_thread as AppBskyFeedGetPostThread,
 )
 from atproto.xrpc_client.models.app.bsky.feed import get_posts as AppBskyFeedGetPosts
 from atproto.xrpc_client.models.app.bsky.feed import (
     get_reposted_by as AppBskyFeedGetRepostedBy,
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/defs.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/defs.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,151 +11,112 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class ProfileViewBasic(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.actor.defs`.
+    """Definition model for :obj:`app.bsky.actor.defs`."""
 
-    Attributes:
-        did: Did.
-        handle: Handle.
-        displayName: Display name.
-        avatar: Avatar.
-        viewer: Viewer.
-        labels: Labels.
-    """
-
-    did: str
-    handle: str
-    avatar: t.Optional[str] = None
-    displayName: t.Optional[str] = None
-    labels: t.Optional[t.List['models.ComAtprotoLabelDefs.Label']] = None
-    viewer: t.Optional['models.AppBskyActorDefs.ViewerState'] = None
+    did: str  #: Did.
+    handle: str  #: Handle.
+    avatar: t.Optional[str] = None  #: Avatar.
+    displayName: t.Optional[str] = None  #: Display name.
+    labels: t.Optional[t.List['models.ComAtprotoLabelDefs.Label']] = None  #: Labels.
+    viewer: t.Optional['models.AppBskyActorDefs.ViewerState'] = None  #: Viewer.
 
     _type: str = 'app.bsky.actor.defs#profileViewBasic'
 
 
 @dataclass
 class ProfileView(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.actor.defs`.
+    """Definition model for :obj:`app.bsky.actor.defs`."""
 
-    Attributes:
-        did: Did.
-        handle: Handle.
-        displayName: Display name.
-        description: Description.
-        avatar: Avatar.
-        indexedAt: Indexed at.
-        viewer: Viewer.
-        labels: Labels.
-    """
-
-    did: str
-    handle: str
-    avatar: t.Optional[str] = None
-    description: t.Optional[str] = None
-    displayName: t.Optional[str] = None
-    indexedAt: t.Optional[str] = None
-    labels: t.Optional[t.List['models.ComAtprotoLabelDefs.Label']] = None
-    viewer: t.Optional['models.AppBskyActorDefs.ViewerState'] = None
+    did: str  #: Did.
+    handle: str  #: Handle.
+    avatar: t.Optional[str] = None  #: Avatar.
+    description: t.Optional[str] = None  #: Description.
+    displayName: t.Optional[str] = None  #: Display name.
+    indexedAt: t.Optional[str] = None  #: Indexed at.
+    labels: t.Optional[t.List['models.ComAtprotoLabelDefs.Label']] = None  #: Labels.
+    viewer: t.Optional['models.AppBskyActorDefs.ViewerState'] = None  #: Viewer.
 
     _type: str = 'app.bsky.actor.defs#profileView'
 
 
 @dataclass
 class ProfileViewDetailed(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.actor.defs`.
+    """Definition model for :obj:`app.bsky.actor.defs`."""
 
-    Attributes:
-        did: Did.
-        handle: Handle.
-        displayName: Display name.
-        description: Description.
-        avatar: Avatar.
-        banner: Banner.
-        followersCount: Followers count.
-        followsCount: Follows count.
-        postsCount: Posts count.
-        indexedAt: Indexed at.
-        viewer: Viewer.
-        labels: Labels.
-    """
-
-    did: str
-    handle: str
-    avatar: t.Optional[str] = None
-    banner: t.Optional[str] = None
-    description: t.Optional[str] = None
-    displayName: t.Optional[str] = None
-    followersCount: t.Optional[int] = None
-    followsCount: t.Optional[int] = None
-    indexedAt: t.Optional[str] = None
-    labels: t.Optional[t.List['models.ComAtprotoLabelDefs.Label']] = None
-    postsCount: t.Optional[int] = None
-    viewer: t.Optional['models.AppBskyActorDefs.ViewerState'] = None
+    did: str  #: Did.
+    handle: str  #: Handle.
+    avatar: t.Optional[str] = None  #: Avatar.
+    banner: t.Optional[str] = None  #: Banner.
+    description: t.Optional[str] = None  #: Description.
+    displayName: t.Optional[str] = None  #: Display name.
+    followersCount: t.Optional[int] = None  #: Followers count.
+    followsCount: t.Optional[int] = None  #: Follows count.
+    indexedAt: t.Optional[str] = None  #: Indexed at.
+    labels: t.Optional[t.List['models.ComAtprotoLabelDefs.Label']] = None  #: Labels.
+    postsCount: t.Optional[int] = None  #: Posts count.
+    viewer: t.Optional['models.AppBskyActorDefs.ViewerState'] = None  #: Viewer.
 
     _type: str = 'app.bsky.actor.defs#profileViewDetailed'
 
 
 @dataclass
 class ViewerState(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.actor.defs`.
+    """Definition model for :obj:`app.bsky.actor.defs`."""
 
-    Attributes:
-        muted: Muted.
-        mutedByList: Muted by list.
-        blockedBy: Blocked by.
-        blocking: Blocking.
-        following: Following.
-        followedBy: Followed by.
-    """
-
-    blockedBy: t.Optional[bool] = None
-    blocking: t.Optional[str] = None
-    followedBy: t.Optional[str] = None
-    following: t.Optional[str] = None
-    muted: t.Optional[bool] = None
-    mutedByList: t.Optional['models.AppBskyGraphDefs.ListViewBasic'] = None
+    blockedBy: t.Optional[bool] = None  #: Blocked by.
+    blocking: t.Optional[str] = None  #: Blocking.
+    followedBy: t.Optional[str] = None  #: Followed by.
+    following: t.Optional[str] = None  #: Following.
+    muted: t.Optional[bool] = None  #: Muted.
+    mutedByList: t.Optional['models.AppBskyGraphDefs.ListViewBasic'] = None  #: Muted by list.
 
     _type: str = 'app.bsky.actor.defs#viewerState'
 
 
 Preferences = t.List[
     t.Union[
-        'models.AppBskyActorDefs.AdultContentPref', 'models.AppBskyActorDefs.ContentLabelPref', 't.Dict[str, t.Any]'
+        'models.AppBskyActorDefs.AdultContentPref',
+        'models.AppBskyActorDefs.ContentLabelPref',
+        'models.AppBskyActorDefs.SavedFeedsPref',
+        't.Dict[str, t.Any]',
     ]
 ]
 
 
 @dataclass
 class AdultContentPref(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.actor.defs`.
+    """Definition model for :obj:`app.bsky.actor.defs`."""
 
-    Attributes:
-        enabled: Enabled.
-    """
-
-    enabled: bool
+    enabled: bool  #: Enabled.
 
     _type: str = 'app.bsky.actor.defs#adultContentPref'
 
 
 @dataclass
 class ContentLabelPref(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.actor.defs`.
-
-    Attributes:
-        label: Label.
-        visibility: Visibility.
-    """
+    """Definition model for :obj:`app.bsky.actor.defs`."""
 
-    label: str
-    visibility: str
+    label: str  #: Label.
+    visibility: str  #: Visibility.
 
     _type: str = 'app.bsky.actor.defs#contentLabelPref'
+
+
+@dataclass
+class SavedFeedsPref(base.ModelBase):
+
+    """Definition model for :obj:`app.bsky.actor.defs`."""
+
+    pinned: t.List[str]  #: Pinned.
+    saved: t.List[str]  #: Saved.
+
+    _type: str = 'app.bsky.actor.defs#savedFeedsPref'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/get_preferences.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/put_preferences.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,25 +8,12 @@
 from dataclasses import dataclass
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
-class Params(base.ParamsModelBase):
+class Data(base.DataModelBase):
 
-    """Parameters model for :obj:`app.bsky.actor.getPreferences`.
+    """Input data model for :obj:`app.bsky.actor.putPreferences`."""
 
-    Attributes:
-    """
-
-
-@dataclass
-class Response(base.ResponseModelBase):
-
-    """Output data model for :obj:`app.bsky.actor.getPreferences`.
-
-    Attributes:
-        preferences: Preferences.
-    """
-
-    preferences: 'models.AppBskyActorDefs.Preferences'
+    preferences: 'models.AppBskyActorDefs.Preferences'  #: Preferences.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/get_profile.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.actor.getProfile`.
+    """Parameters model for :obj:`app.bsky.actor.getProfiles`."""
 
-    Attributes:
-        actor: Actor.
-    """
+    actors: t.List[str]  #: Actors.
 
-    actor: str
 
+@dataclass
+class Response(base.ResponseModelBase):
+
+    """Output data model for :obj:`app.bsky.actor.getProfiles`."""
 
-#: Response reference to :obj:`models.AppBskyActorDefs.ProfileViewDetailed` model.
-ResponseRef: t.Type[models.AppBskyActorDefs.ProfileViewDetailed] = models.AppBskyActorDefs.ProfileViewDetailed
+    profiles: t.List['models.AppBskyActorDefs.ProfileViewDetailed']  #: Profiles.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/get_profile.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,26 +11,14 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.actor.getProfiles`.
+    """Parameters model for :obj:`app.bsky.actor.getProfile`."""
 
-    Attributes:
-        actors: Actors.
-    """
+    actor: str  #: Actor.
 
-    actors: t.List[str]
 
-
-@dataclass
-class Response(base.ResponseModelBase):
-
-    """Output data model for :obj:`app.bsky.actor.getProfiles`.
-
-    Attributes:
-        profiles: Profiles.
-    """
-
-    profiles: t.List['models.AppBskyActorDefs.ProfileViewDetailed']
+#: Response reference to :obj:`models.AppBskyActorDefs.ProfileViewDetailed` model.
+ResponseRef: t.Type[models.AppBskyActorDefs.ProfileViewDetailed] = models.AppBskyActorDefs.ProfileViewDetailed
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,30 +11,19 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.actor.getSuggestions`.
+    """Parameters model for :obj:`app.bsky.actor.searchActorsTypeahead`."""
 
-    Attributes:
-        limit: Limit.
-        cursor: Cursor.
-    """
-
-    cursor: t.Optional[str] = None
-    limit: t.Optional[int] = None
+    limit: t.Optional[int] = None  #: Limit.
+    term: t.Optional[str] = None  #: Term.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.actor.getSuggestions`.
-
-    Attributes:
-        cursor: Cursor.
-        actors: Actors.
-    """
+    """Output data model for :obj:`app.bsky.actor.searchActorsTypeahead`."""
 
-    actors: t.List['models.AppBskyActorDefs.ProfileView']
-    cursor: t.Optional[str] = None
+    actors: t.List['models.AppBskyActorDefs.ProfileViewBasic']  #: Actors.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/profile.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/profile.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,22 +11,15 @@
 from atproto.xrpc_client.models import base
 from atproto.xrpc_client.models.blob_ref import BlobRef
 
 
 @dataclass
 class Main(base.RecordModelBase):
 
-    """Record model for :obj:`app.bsky.actor.profile`.
+    """Record model for :obj:`app.bsky.actor.profile`."""
 
-    Attributes:
-        displayName: Display name.
-        description: Description.
-        avatar: Avatar.
-        banner: Banner.
-    """
-
-    avatar: t.Optional[BlobRef] = None
-    banner: t.Optional[BlobRef] = None
-    description: t.Optional[str] = None
-    displayName: t.Optional[str] = None
+    avatar: t.Optional[BlobRef] = None  #: Avatar.
+    banner: t.Optional[BlobRef] = None  #: Banner.
+    description: t.Optional[str] = None  #: Description.
+    displayName: t.Optional[str] = None  #: Display name.
 
     _type: str = 'app.bsky.actor.profile'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/put_preferences.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/get_preferences.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 from dataclasses import dataclass
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
-class Data(base.DataModelBase):
+class Params(base.ParamsModelBase):
 
-    """Input data model for :obj:`app.bsky.actor.putPreferences`.
+    """Parameters model for :obj:`app.bsky.actor.getPreferences`."""
 
-    Attributes:
-        preferences: Preferences.
-    """
 
-    preferences: 'models.AppBskyActorDefs.Preferences'
+@dataclass
+class Response(base.ResponseModelBase):
+
+    """Output data model for :obj:`app.bsky.actor.getPreferences`."""
+
+    preferences: 'models.AppBskyActorDefs.Preferences'  #: Preferences.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/search_actors.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/search_actors.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,32 +11,21 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.actor.searchActors`.
+    """Parameters model for :obj:`app.bsky.actor.searchActors`."""
 
-    Attributes:
-        term: Term.
-        limit: Limit.
-        cursor: Cursor.
-    """
-
-    cursor: t.Optional[str] = None
-    limit: t.Optional[int] = None
-    term: t.Optional[str] = None
+    cursor: t.Optional[str] = None  #: Cursor.
+    limit: t.Optional[int] = None  #: Limit.
+    term: t.Optional[str] = None  #: Term.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.actor.searchActors`.
+    """Output data model for :obj:`app.bsky.actor.searchActors`."""
 
-    Attributes:
-        cursor: Cursor.
-        actors: Actors.
-    """
-
-    actors: t.List['models.AppBskyActorDefs.ProfileView']
-    cursor: t.Optional[str] = None
+    actors: t.List['models.AppBskyActorDefs.ProfileView']  #: Actors.
+    cursor: t.Optional[str] = None  #: Cursor.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/like.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,22 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
-import typing as t
 from dataclasses import dataclass
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
-class Params(base.ParamsModelBase):
+class Main(base.RecordModelBase):
 
-    """Parameters model for :obj:`app.bsky.actor.searchActorsTypeahead`.
+    """Record model for :obj:`app.bsky.feed.like`."""
 
-    Attributes:
-        term: Term.
-        limit: Limit.
-    """
+    createdAt: str  #: Created at.
+    subject: 'models.ComAtprotoRepoStrongRef.Main'  #: Subject.
 
-    limit: t.Optional[int] = None
-    term: t.Optional[str] = None
-
-
-@dataclass
-class Response(base.ResponseModelBase):
-
-    """Output data model for :obj:`app.bsky.actor.searchActorsTypeahead`.
-
-    Attributes:
-        actors: Actors.
-    """
-
-    actors: t.List['models.AppBskyActorDefs.ProfileViewBasic']
+    _type: str = 'app.bsky.feed.like'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/embed/record.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/record.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,99 +11,74 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Main(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.embed.record`.
+    """Definition model for :obj:`app.bsky.embed.record`."""
 
-    Attributes:
-        record: Record.
-    """
-
-    record: 'models.ComAtprotoRepoStrongRef.Main'
+    record: 'models.ComAtprotoRepoStrongRef.Main'  #: Record.
 
     _type: str = 'app.bsky.embed.record'
 
 
 @dataclass
 class View(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.embed.record`.
-
-    Attributes:
-        record: Record.
-    """
+    """Definition model for :obj:`app.bsky.embed.record`."""
 
     record: t.Union[
         'models.AppBskyEmbedRecord.ViewRecord',
         'models.AppBskyEmbedRecord.ViewNotFound',
         'models.AppBskyEmbedRecord.ViewBlocked',
+        'models.AppBskyFeedDefs.GeneratorView',
         't.Dict[str, t.Any]',
-    ]
+    ]  #: Record.
 
     _type: str = 'app.bsky.embed.record#view'
 
 
 @dataclass
 class ViewRecord(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.embed.record`.
+    """Definition model for :obj:`app.bsky.embed.record`."""
 
-    Attributes:
-        uri: Uri.
-        cid: Cid.
-        author: Author.
-        value: Value.
-        labels: Labels.
-        embeds: Embeds.
-        indexedAt: Indexed at.
-    """
-
-    author: 'models.AppBskyActorDefs.ProfileViewBasic'
-    cid: str
-    indexedAt: str
-    uri: str
-    value: 'base.RecordModelBase'
+    author: 'models.AppBskyActorDefs.ProfileViewBasic'  #: Author.
+    cid: str  #: Cid.
+    indexedAt: str  #: Indexed at.
+    uri: str  #: Uri.
+    value: 'base.RecordModelBase'  #: Value.
     embeds: t.Optional[
         t.List[
             t.Union[
                 'models.AppBskyEmbedImages.View',
                 'models.AppBskyEmbedExternal.View',
                 'models.AppBskyEmbedRecord.View',
                 'models.AppBskyEmbedRecordWithMedia.View',
                 't.Dict[str, t.Any]',
             ]
         ]
-    ] = None
-    labels: t.Optional[t.List['models.ComAtprotoLabelDefs.Label']] = None
+    ] = None  #: Embeds.
+    labels: t.Optional[t.List['models.ComAtprotoLabelDefs.Label']] = None  #: Labels.
 
     _type: str = 'app.bsky.embed.record#viewRecord'
 
 
 @dataclass
 class ViewNotFound(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.embed.record`.
+    """Definition model for :obj:`app.bsky.embed.record`."""
 
-    Attributes:
-        uri: Uri.
-    """
-
-    uri: str
+    uri: str  #: Uri.
 
     _type: str = 'app.bsky.embed.record#viewNotFound'
 
 
 @dataclass
 class ViewBlocked(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.embed.record`.
-
-    Attributes:
-        uri: Uri.
-    """
+    """Definition model for :obj:`app.bsky.embed.record`."""
 
-    uri: str
+    uri: str  #: Uri.
 
     _type: str = 'app.bsky.embed.record#viewBlocked'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,34 +11,28 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Main(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.embed.recordWithMedia`.
+    """Definition model for :obj:`app.bsky.embed.recordWithMedia`."""
 
-    Attributes:
-        record: Record.
-        media: Media.
-    """
-
-    media: t.Union['models.AppBskyEmbedImages.Main', 'models.AppBskyEmbedExternal.Main', 't.Dict[str, t.Any]']
-    record: 'models.AppBskyEmbedRecord.Main'
+    media: t.Union[
+        'models.AppBskyEmbedImages.Main', 'models.AppBskyEmbedExternal.Main', 't.Dict[str, t.Any]'
+    ]  #: Media.
+    record: 'models.AppBskyEmbedRecord.Main'  #: Record.
 
     _type: str = 'app.bsky.embed.recordWithMedia'
 
 
 @dataclass
 class View(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.embed.recordWithMedia`.
-
-    Attributes:
-        record: Record.
-        media: Media.
-    """
+    """Definition model for :obj:`app.bsky.embed.recordWithMedia`."""
 
-    media: t.Union['models.AppBskyEmbedImages.View', 'models.AppBskyEmbedExternal.View', 't.Dict[str, t.Any]']
-    record: 'models.AppBskyEmbedRecord.View'
+    media: t.Union[
+        'models.AppBskyEmbedImages.View', 'models.AppBskyEmbedExternal.View', 't.Dict[str, t.Any]'
+    ]  #: Media.
+    record: 'models.AppBskyEmbedRecord.View'  #: Record.
 
     _type: str = 'app.bsky.embed.recordWithMedia#view'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/defs.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/defs.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,176 +11,186 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class PostView(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.feed.defs`.
+    """Definition model for :obj:`app.bsky.feed.defs`."""
 
-    Attributes:
-        uri: Uri.
-        cid: Cid.
-        author: Author.
-        record: Record.
-        embed: Embed.
-        replyCount: Reply count.
-        repostCount: Repost count.
-        likeCount: Like count.
-        indexedAt: Indexed at.
-        viewer: Viewer.
-        labels: Labels.
-    """
-
-    author: 'models.AppBskyActorDefs.ProfileViewBasic'
-    cid: str
-    indexedAt: str
-    record: 'base.RecordModelBase'
-    uri: str
+    author: 'models.AppBskyActorDefs.ProfileViewBasic'  #: Author.
+    cid: str  #: Cid.
+    indexedAt: str  #: Indexed at.
+    record: 'base.RecordModelBase'  #: Record.
+    uri: str  #: Uri.
     embed: t.Optional[
         t.Union[
             'models.AppBskyEmbedImages.View',
             'models.AppBskyEmbedExternal.View',
             'models.AppBskyEmbedRecord.View',
             'models.AppBskyEmbedRecordWithMedia.View',
             't.Dict[str, t.Any]',
         ]
-    ] = None
-    labels: t.Optional[t.List['models.ComAtprotoLabelDefs.Label']] = None
-    likeCount: t.Optional[int] = None
-    replyCount: t.Optional[int] = None
-    repostCount: t.Optional[int] = None
-    viewer: t.Optional['models.AppBskyFeedDefs.ViewerState'] = None
+    ] = None  #: Embed.
+    labels: t.Optional[t.List['models.ComAtprotoLabelDefs.Label']] = None  #: Labels.
+    likeCount: t.Optional[int] = None  #: Like count.
+    replyCount: t.Optional[int] = None  #: Reply count.
+    repostCount: t.Optional[int] = None  #: Repost count.
+    viewer: t.Optional['models.AppBskyFeedDefs.ViewerState'] = None  #: Viewer.
 
     _type: str = 'app.bsky.feed.defs#postView'
 
 
 @dataclass
 class ViewerState(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.feed.defs`.
+    """Definition model for :obj:`app.bsky.feed.defs`."""
 
-    Attributes:
-        repost: Repost.
-        like: Like.
-    """
-
-    like: t.Optional[str] = None
-    repost: t.Optional[str] = None
+    like: t.Optional[str] = None  #: Like.
+    repost: t.Optional[str] = None  #: Repost.
 
     _type: str = 'app.bsky.feed.defs#viewerState'
 
 
 @dataclass
 class FeedViewPost(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.feed.defs`.
+    """Definition model for :obj:`app.bsky.feed.defs`."""
 
-    Attributes:
-        post: Post.
-        reply: Reply.
-        reason: Reason.
-    """
-
-    post: 'models.AppBskyFeedDefs.PostView'
-    reason: t.Optional[t.Union['models.AppBskyFeedDefs.ReasonRepost', 't.Dict[str, t.Any]']] = None
-    reply: t.Optional['models.AppBskyFeedDefs.ReplyRef'] = None
+    post: 'models.AppBskyFeedDefs.PostView'  #: Post.
+    reason: t.Optional[t.Union['models.AppBskyFeedDefs.ReasonRepost', 't.Dict[str, t.Any]']] = None  #: Reason.
+    reply: t.Optional['models.AppBskyFeedDefs.ReplyRef'] = None  #: Reply.
 
     _type: str = 'app.bsky.feed.defs#feedViewPost'
 
 
 @dataclass
 class ReplyRef(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.feed.defs`.
-
-    Attributes:
-        root: Root.
-        parent: Parent.
-    """
+    """Definition model for :obj:`app.bsky.feed.defs`."""
 
-    parent: 'models.AppBskyFeedDefs.PostView'
-    root: 'models.AppBskyFeedDefs.PostView'
+    parent: t.Union[
+        'models.AppBskyFeedDefs.PostView',
+        'models.AppBskyFeedDefs.NotFoundPost',
+        'models.AppBskyFeedDefs.BlockedPost',
+        't.Dict[str, t.Any]',
+    ]  #: Parent.
+    root: t.Union[
+        'models.AppBskyFeedDefs.PostView',
+        'models.AppBskyFeedDefs.NotFoundPost',
+        'models.AppBskyFeedDefs.BlockedPost',
+        't.Dict[str, t.Any]',
+    ]  #: Root.
 
     _type: str = 'app.bsky.feed.defs#replyRef'
 
 
 @dataclass
 class ReasonRepost(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.feed.defs`.
+    """Definition model for :obj:`app.bsky.feed.defs`."""
 
-    Attributes:
-        by: By.
-        indexedAt: Indexed at.
-    """
-
-    by: 'models.AppBskyActorDefs.ProfileViewBasic'
-    indexedAt: str
+    by: 'models.AppBskyActorDefs.ProfileViewBasic'  #: By.
+    indexedAt: str  #: Indexed at.
 
     _type: str = 'app.bsky.feed.defs#reasonRepost'
 
 
 @dataclass
 class ThreadViewPost(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.feed.defs`.
-
-    Attributes:
-        post: Post.
-        parent: Parent.
-        replies: Replies.
-    """
+    """Definition model for :obj:`app.bsky.feed.defs`."""
 
-    post: 'models.AppBskyFeedDefs.PostView'
+    post: 'models.AppBskyFeedDefs.PostView'  #: Post.
     parent: t.Optional[
         t.Union[
             'models.AppBskyFeedDefs.ThreadViewPost',
             'models.AppBskyFeedDefs.NotFoundPost',
             'models.AppBskyFeedDefs.BlockedPost',
             't.Dict[str, t.Any]',
         ]
-    ] = None
+    ] = None  #: Parent.
     replies: t.Optional[
         t.List[
             t.Union[
                 'models.AppBskyFeedDefs.ThreadViewPost',
                 'models.AppBskyFeedDefs.NotFoundPost',
                 'models.AppBskyFeedDefs.BlockedPost',
                 't.Dict[str, t.Any]',
             ]
         ]
-    ] = None
+    ] = None  #: Replies.
 
     _type: str = 'app.bsky.feed.defs#threadViewPost'
 
 
 @dataclass
 class NotFoundPost(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.feed.defs`.
+    """Definition model for :obj:`app.bsky.feed.defs`."""
 
-    Attributes:
-        uri: Uri.
-        notFound: Not found.
-    """
-
-    notFound: bool
-    uri: str
+    notFound: bool  #: Not found.
+    uri: str  #: Uri.
 
     _type: str = 'app.bsky.feed.defs#notFoundPost'
 
 
 @dataclass
 class BlockedPost(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.feed.defs`.
-
-    Attributes:
-        uri: Uri.
-        blocked: Blocked.
-    """
+    """Definition model for :obj:`app.bsky.feed.defs`."""
 
-    blocked: bool
-    uri: str
+    blocked: bool  #: Blocked.
+    uri: str  #: Uri.
 
     _type: str = 'app.bsky.feed.defs#blockedPost'
+
+
+@dataclass
+class GeneratorView(base.ModelBase):
+
+    """Definition model for :obj:`app.bsky.feed.defs`."""
+
+    cid: str  #: Cid.
+    creator: 'models.AppBskyActorDefs.ProfileView'  #: Creator.
+    displayName: str  #: Display name.
+    indexedAt: str  #: Indexed at.
+    uri: str  #: Uri.
+    avatar: t.Optional[str] = None  #: Avatar.
+    description: t.Optional[str] = None  #: Description.
+    descriptionFacets: t.Optional[t.List['models.AppBskyRichtextFacet.Main']] = None  #: Description facets.
+    did: t.Optional[str] = None  #: Did.
+    likeCount: t.Optional[int] = None  #: Like count.
+    viewer: t.Optional['models.AppBskyFeedDefs.GeneratorViewerState'] = None  #: Viewer.
+
+    _type: str = 'app.bsky.feed.defs#generatorView'
+
+
+@dataclass
+class GeneratorViewerState(base.ModelBase):
+
+    """Definition model for :obj:`app.bsky.feed.defs`."""
+
+    like: t.Optional[str] = None  #: Like.
+
+    _type: str = 'app.bsky.feed.defs#generatorViewerState'
+
+
+@dataclass
+class SkeletonFeedPost(base.ModelBase):
+
+    """Definition model for :obj:`app.bsky.feed.defs`."""
+
+    post: str  #: Post.
+    reason: t.Optional[t.Union['models.AppBskyFeedDefs.SkeletonReasonRepost', 't.Dict[str, t.Any]']] = None  #: Reason.
+
+    _type: str = 'app.bsky.feed.defs#skeletonFeedPost'
+
+
+@dataclass
+class SkeletonReasonRepost(base.ModelBase):
+
+    """Definition model for :obj:`app.bsky.feed.defs`."""
+
+    repost: str  #: Repost.
+
+    _type: str = 'app.bsky.feed.defs#skeletonReasonRepost'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,32 +11,21 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.feed.getAuthorFeed`.
+    """Parameters model for :obj:`app.bsky.feed.getAuthorFeed`."""
 
-    Attributes:
-        actor: Actor.
-        limit: Limit.
-        cursor: Cursor.
-    """
-
-    actor: str
-    cursor: t.Optional[str] = None
-    limit: t.Optional[int] = None
+    actor: str  #: Actor.
+    cursor: t.Optional[str] = None  #: Cursor.
+    limit: t.Optional[int] = None  #: Limit.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.feed.getAuthorFeed`.
+    """Output data model for :obj:`app.bsky.feed.getAuthorFeed`."""
 
-    Attributes:
-        cursor: Cursor.
-        feed: Feed.
-    """
-
-    feed: t.List['models.AppBskyFeedDefs.FeedViewPost']
-    cursor: t.Optional[str] = None
+    feed: t.List['models.AppBskyFeedDefs.FeedViewPost']  #: Feed.
+    cursor: t.Optional[str] = None  #: Cursor.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/get_likes.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_likes.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,56 +11,36 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.feed.getLikes`.
+    """Parameters model for :obj:`app.bsky.feed.getLikes`."""
 
-    Attributes:
-        uri: Uri.
-        cid: Cid.
-        limit: Limit.
-        cursor: Cursor.
-    """
-
-    uri: str
-    cid: t.Optional[str] = None
-    cursor: t.Optional[str] = None
-    limit: t.Optional[int] = None
+    uri: str  #: Uri.
+    cid: t.Optional[str] = None  #: Cid.
+    cursor: t.Optional[str] = None  #: Cursor.
+    limit: t.Optional[int] = None  #: Limit.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.feed.getLikes`.
+    """Output data model for :obj:`app.bsky.feed.getLikes`."""
 
-    Attributes:
-        uri: Uri.
-        cid: Cid.
-        cursor: Cursor.
-        likes: Likes.
-    """
-
-    likes: t.List['models.AppBskyFeedGetLikes.Like']
-    uri: str
-    cid: t.Optional[str] = None
-    cursor: t.Optional[str] = None
+    likes: t.List['models.AppBskyFeedGetLikes.Like']  #: Likes.
+    uri: str  #: Uri.
+    cid: t.Optional[str] = None  #: Cid.
+    cursor: t.Optional[str] = None  #: Cursor.
 
 
 @dataclass
 class Like(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.feed.getLikes`.
+    """Definition model for :obj:`app.bsky.feed.getLikes`."""
 
-    Attributes:
-        indexedAt: Indexed at.
-        createdAt: Created at.
-        actor: Actor.
-    """
-
-    actor: 'models.AppBskyActorDefs.ProfileView'
-    createdAt: str
-    indexedAt: str
+    actor: 'models.AppBskyActorDefs.ProfileView'  #: Actor.
+    createdAt: str  #: Created at.
+    indexedAt: str  #: Indexed at.
 
     _type: str = 'app.bsky.feed.getLikes#like'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_posts.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,33 +11,18 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.feed.getPostThread`.
+    """Parameters model for :obj:`app.bsky.feed.getPosts`."""
 
-    Attributes:
-        uri: Uri.
-        depth: Depth.
-    """
-
-    uri: str
-    depth: t.Optional[int] = None
+    uris: t.List[str]  #: Uris.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.feed.getPostThread`.
+    """Output data model for :obj:`app.bsky.feed.getPosts`."""
 
-    Attributes:
-        thread: Thread.
-    """
-
-    thread: t.Union[
-        'models.AppBskyFeedDefs.ThreadViewPost',
-        'models.AppBskyFeedDefs.NotFoundPost',
-        'models.AppBskyFeedDefs.BlockedPost',
-        't.Dict[str, t.Any]',
-    ]
+    posts: t.List['models.AppBskyFeedDefs.PostView']  #: Posts.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/get_posts.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,26 +11,24 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.feed.getPosts`.
+    """Parameters model for :obj:`app.bsky.feed.getPostThread`."""
 
-    Attributes:
-        uris: Uris.
-    """
-
-    uris: t.List[str]
+    uri: str  #: Uri.
+    depth: t.Optional[int] = None  #: Depth.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.feed.getPosts`.
-
-    Attributes:
-        posts: Posts.
-    """
+    """Output data model for :obj:`app.bsky.feed.getPostThread`."""
 
-    posts: t.List['models.AppBskyFeedDefs.PostView']
+    thread: t.Union[
+        'models.AppBskyFeedDefs.ThreadViewPost',
+        'models.AppBskyFeedDefs.NotFoundPost',
+        'models.AppBskyFeedDefs.BlockedPost',
+        't.Dict[str, t.Any]',
+    ]  #: Thread.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,45 +4,26 @@
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 import typing as t
 from dataclasses import dataclass
 
-from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.feed.getRepostedBy`.
+    """Parameters model for :obj:`com.atproto.sync.listBlobs`."""
 
-    Attributes:
-        uri: Uri.
-        cid: Cid.
-        limit: Limit.
-        cursor: Cursor.
-    """
-
-    uri: str
-    cid: t.Optional[str] = None
-    cursor: t.Optional[str] = None
-    limit: t.Optional[int] = None
+    did: str  #: The DID of the repo.
+    earliest: t.Optional[str] = None  #: The earliest commit to start from.
+    latest: t.Optional[str] = None  #: The most recent commit.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.feed.getRepostedBy`.
+    """Output data model for :obj:`com.atproto.sync.listBlobs`."""
 
-    Attributes:
-        uri: Uri.
-        cid: Cid.
-        cursor: Cursor.
-        repostedBy: Reposted by.
-    """
-
-    repostedBy: t.List['models.AppBskyActorDefs.ProfileView']
-    uri: str
-    cid: t.Optional[str] = None
-    cursor: t.Optional[str] = None
+    cids: t.List[str]  #: Cids.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/put_record.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,39 +4,31 @@
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 import typing as t
 from dataclasses import dataclass
 
-from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
-class Params(base.ParamsModelBase):
+class Data(base.DataModelBase):
 
-    """Parameters model for :obj:`app.bsky.feed.getTimeline`.
+    """Input data model for :obj:`com.atproto.repo.putRecord`."""
 
-    Attributes:
-        algorithm: Algorithm.
-        limit: Limit.
-        cursor: Cursor.
-    """
-
-    algorithm: t.Optional[str] = None
-    cursor: t.Optional[str] = None
-    limit: t.Optional[int] = None
+    collection: str  #: The NSID of the record collection.
+    record: 'base.RecordModelBase'  #: The record to write.
+    repo: str  #: The handle or DID of the repo.
+    rkey: str  #: The key of the record.
+    swapCommit: t.Optional[str] = None  #: Compare and swap with the previous commit by cid.
+    swapRecord: t.Optional[str] = None  #: Compare and swap with the previous record by cid.
+    validate: t.Optional[bool] = None  #: Validate the record?
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.feed.getTimeline`.
+    """Output data model for :obj:`com.atproto.repo.putRecord`."""
 
-    Attributes:
-        cursor: Cursor.
-        feed: Feed.
-    """
-
-    feed: t.List['models.AppBskyFeedDefs.FeedViewPost']
-    cursor: t.Optional[str] = None
+    cid: str  #: Cid.
+    uri: str  #: Uri.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/like.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/repost.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,18 +10,13 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Main(base.RecordModelBase):
 
-    """Record model for :obj:`app.bsky.feed.like`.
+    """Record model for :obj:`app.bsky.feed.repost`."""
 
-    Attributes:
-        subject: Subject.
-        createdAt: Created at.
-    """
+    createdAt: str  #: Created at.
+    subject: 'models.ComAtprotoRepoStrongRef.Main'  #: Subject.
 
-    createdAt: str
-    subject: 'models.ComAtprotoRepoStrongRef.Main'
-
-    _type: str = 'app.bsky.feed.like'
+    _type: str = 'app.bsky.feed.repost'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/post.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/post.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,84 +11,61 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class ReplyRef(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.feed.post`.
+    """Definition model for :obj:`app.bsky.feed.post`."""
 
-    Attributes:
-        root: Root.
-        parent: Parent.
-    """
-
-    parent: 'models.ComAtprotoRepoStrongRef.Main'
-    root: 'models.ComAtprotoRepoStrongRef.Main'
+    parent: 'models.ComAtprotoRepoStrongRef.Main'  #: Parent.
+    root: 'models.ComAtprotoRepoStrongRef.Main'  #: Root.
 
     _type: str = 'app.bsky.feed.post#replyRef'
 
 
 @dataclass
 class Entity(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.feed.post`. Deprecated: use facets instead.
+    """Definition model for :obj:`app.bsky.feed.post`. Deprecated: use facets instead."""
 
-    Attributes:
-        index: Index.
-        type: Expected values are 'mention' and 'link'.
-        value: Value.
-    """
-
-    index: 'models.AppBskyFeedPost.TextSlice'
-    type: str
-    value: str
+    index: 'models.AppBskyFeedPost.TextSlice'  #: Index.
+    type: str  #: Expected values are 'mention' and 'link'.
+    value: str  #: Value.
 
     _type: str = 'app.bsky.feed.post#entity'
 
 
 @dataclass
 class TextSlice(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.feed.post`. Deprecated. Use app.bsky.richtext instead -- A text segment. Start is inclusive, end is exclusive. Indices are for utf16-encoded strings.
-
-    Attributes:
-        start: Start.
-        end: End.
-    """
+    """Definition model for :obj:`app.bsky.feed.post`. Deprecated. Use app.bsky.richtext instead -- A text segment. Start is inclusive, end is exclusive. Indices are for utf16-encoded strings."""
 
-    end: int
-    start: int
+    end: int  #: End.
+    start: int  #: Start.
 
     _type: str = 'app.bsky.feed.post#textSlice'
 
 
 @dataclass
 class Main(base.RecordModelBase):
 
-    """Record model for :obj:`app.bsky.feed.post`.
-
-    Attributes:
-        text: Text.
-        entities: Deprecated: replaced by app.bsky.richtext.facet.
-        facets: Facets.
-        reply: Reply.
-        embed: Embed.
-        createdAt: Created at.
-    """
+    """Record model for :obj:`app.bsky.feed.post`."""
 
-    createdAt: str
-    text: str
+    createdAt: str  #: Created at.
+    text: str  #: Text.
     embed: t.Optional[
         t.Union[
             'models.AppBskyEmbedImages.Main',
             'models.AppBskyEmbedExternal.Main',
             'models.AppBskyEmbedRecord.Main',
             'models.AppBskyEmbedRecordWithMedia.Main',
             't.Dict[str, t.Any]',
         ]
-    ] = None
-    entities: t.Optional[t.List['models.AppBskyFeedPost.Entity']] = None
-    facets: t.Optional[t.List['models.AppBskyRichtextFacet.Main']] = None
-    reply: t.Optional['models.AppBskyFeedPost.ReplyRef'] = None
+    ] = None  #: Embed.
+    entities: t.Optional[
+        t.List['models.AppBskyFeedPost.Entity']
+    ] = None  #: Deprecated: replaced by app.bsky.richtext.facet.
+    facets: t.Optional[t.List['models.AppBskyRichtextFacet.Main']] = None  #: Facets.
+    reply: t.Optional['models.AppBskyFeedPost.ReplyRef'] = None  #: Reply.
 
     _type: str = 'app.bsky.feed.post'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/repost.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/follow.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,25 +3,19 @@
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 from dataclasses import dataclass
 
-from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Main(base.RecordModelBase):
 
-    """Record model for :obj:`app.bsky.feed.repost`.
+    """Record model for :obj:`app.bsky.graph.follow`."""
 
-    Attributes:
-        subject: Subject.
-        createdAt: Created at.
-    """
+    createdAt: str  #: Created at.
+    subject: str  #: Subject.
 
-    createdAt: str
-    subject: 'models.ComAtprotoRepoStrongRef.Main'
-
-    _type: str = 'app.bsky.feed.repost'
+    _type: str = 'app.bsky.graph.follow'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/block.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/block.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,18 +9,13 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Main(base.RecordModelBase):
 
-    """Record model for :obj:`app.bsky.graph.block`.
+    """Record model for :obj:`app.bsky.graph.block`."""
 
-    Attributes:
-        subject: Subject.
-        createdAt: Created at.
-    """
-
-    createdAt: str
-    subject: str
+    createdAt: str  #: Created at.
+    subject: str  #: Subject.
 
     _type: str = 'app.bsky.graph.block'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/defs.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/defs.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,89 +13,60 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class ListViewBasic(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.graph.defs`.
+    """Definition model for :obj:`app.bsky.graph.defs`."""
 
-    Attributes:
-        uri: Uri.
-        name: Name.
-        purpose: Purpose.
-        avatar: Avatar.
-        viewer: Viewer.
-        indexedAt: Indexed at.
-    """
-
-    name: str
-    purpose: 'models.AppBskyGraphDefs.ListPurpose'
-    uri: str
-    avatar: t.Optional[str] = None
-    indexedAt: t.Optional[str] = None
-    viewer: t.Optional['models.AppBskyGraphDefs.ListViewerState'] = None
+    name: str  #: Name.
+    purpose: 'models.AppBskyGraphDefs.ListPurpose'  #: Purpose.
+    uri: str  #: Uri.
+    avatar: t.Optional[str] = None  #: Avatar.
+    indexedAt: t.Optional[str] = None  #: Indexed at.
+    viewer: t.Optional['models.AppBskyGraphDefs.ListViewerState'] = None  #: Viewer.
 
     _type: str = 'app.bsky.graph.defs#listViewBasic'
 
 
 @dataclass
 class ListView(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.graph.defs`.
+    """Definition model for :obj:`app.bsky.graph.defs`."""
 
-    Attributes:
-        uri: Uri.
-        creator: Creator.
-        name: Name.
-        purpose: Purpose.
-        description: Description.
-        descriptionFacets: Description facets.
-        avatar: Avatar.
-        viewer: Viewer.
-        indexedAt: Indexed at.
-    """
-
-    creator: 'models.AppBskyActorDefs.ProfileView'
-    indexedAt: str
-    name: str
-    purpose: 'models.AppBskyGraphDefs.ListPurpose'
-    uri: str
-    avatar: t.Optional[str] = None
-    description: t.Optional[str] = None
-    descriptionFacets: t.Optional[t.List['models.AppBskyRichtextFacet.Main']] = None
-    viewer: t.Optional['models.AppBskyGraphDefs.ListViewerState'] = None
+    creator: 'models.AppBskyActorDefs.ProfileView'  #: Creator.
+    indexedAt: str  #: Indexed at.
+    name: str  #: Name.
+    purpose: 'models.AppBskyGraphDefs.ListPurpose'  #: Purpose.
+    uri: str  #: Uri.
+    avatar: t.Optional[str] = None  #: Avatar.
+    description: t.Optional[str] = None  #: Description.
+    descriptionFacets: t.Optional[t.List['models.AppBskyRichtextFacet.Main']] = None  #: Description facets.
+    viewer: t.Optional['models.AppBskyGraphDefs.ListViewerState'] = None  #: Viewer.
 
     _type: str = 'app.bsky.graph.defs#listView'
 
 
 @dataclass
 class ListItemView(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.graph.defs`.
+    """Definition model for :obj:`app.bsky.graph.defs`."""
 
-    Attributes:
-        subject: Subject.
-    """
-
-    subject: 'models.AppBskyActorDefs.ProfileView'
+    subject: 'models.AppBskyActorDefs.ProfileView'  #: Subject.
 
     _type: str = 'app.bsky.graph.defs#listItemView'
 
 
 ListPurpose = te.Literal['Modlist']
 
 Modlist: te.Literal['modlist'] = 'modlist'
 
 
 @dataclass
 class ListViewerState(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.graph.defs`.
-
-    Attributes:
-        muted: Muted.
-    """
+    """Definition model for :obj:`app.bsky.graph.defs`."""
 
-    muted: t.Optional[bool] = None
+    muted: t.Optional[bool] = None  #: Muted.
 
     _type: str = 'app.bsky.graph.defs#listViewerState'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/follow.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_feed_generators.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
 
+from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
-class Main(base.RecordModelBase):
+class Params(base.ParamsModelBase):
 
-    """Record model for :obj:`app.bsky.graph.follow`.
+    """Parameters model for :obj:`app.bsky.feed.getFeedGenerators`."""
 
-    Attributes:
-        subject: Subject.
-        createdAt: Created at.
-    """
+    feeds: t.List[str]  #: Feeds.
 
-    createdAt: str
-    subject: str
 
-    _type: str = 'app.bsky.graph.follow'
+@dataclass
+class Response(base.ResponseModelBase):
+
+    """Output data model for :obj:`app.bsky.feed.getFeedGenerators`."""
+
+    feeds: t.List['models.AppBskyFeedDefs.GeneratorView']  #: Feeds.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/delete_record.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,37 +4,20 @@
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 import typing as t
 from dataclasses import dataclass
 
-from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
-class Params(base.ParamsModelBase):
+class Data(base.DataModelBase):
 
-    """Parameters model for :obj:`app.bsky.graph.getBlocks`.
+    """Input data model for :obj:`com.atproto.repo.deleteRecord`."""
 
-    Attributes:
-        limit: Limit.
-        cursor: Cursor.
-    """
-
-    cursor: t.Optional[str] = None
-    limit: t.Optional[int] = None
-
-
-@dataclass
-class Response(base.ResponseModelBase):
-
-    """Output data model for :obj:`app.bsky.graph.getBlocks`.
-
-    Attributes:
-        cursor: Cursor.
-        blocks: Blocks.
-    """
-
-    blocks: t.List['models.AppBskyActorDefs.ProfileView']
-    cursor: t.Optional[str] = None
+    collection: str  #: The NSID of the record collection.
+    repo: str  #: The handle or DID of the repo.
+    rkey: str  #: The key of the record.
+    swapCommit: t.Optional[str] = None  #: Compare and swap with the previous commit by cid.
+    swapRecord: t.Optional[str] = None  #: Compare and swap with the previous record by cid.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_followers.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,34 +11,20 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.graph.getFollowers`.
+    """Parameters model for :obj:`app.bsky.graph.getMutes`."""
 
-    Attributes:
-        actor: Actor.
-        limit: Limit.
-        cursor: Cursor.
-    """
-
-    actor: str
-    cursor: t.Optional[str] = None
-    limit: t.Optional[int] = None
+    cursor: t.Optional[str] = None  #: Cursor.
+    limit: t.Optional[int] = None  #: Limit.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.graph.getFollowers`.
+    """Output data model for :obj:`app.bsky.graph.getMutes`."""
 
-    Attributes:
-        subject: Subject.
-        cursor: Cursor.
-        followers: Followers.
-    """
-
-    followers: t.List['models.AppBskyActorDefs.ProfileView']
-    subject: 'models.AppBskyActorDefs.ProfileView'
-    cursor: t.Optional[str] = None
+    mutes: t.List['models.AppBskyActorDefs.ProfileView']  #: Mutes.
+    cursor: t.Optional[str] = None  #: Cursor.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_follows.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/get_lists.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,34 +11,21 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.graph.getFollows`.
+    """Parameters model for :obj:`app.bsky.graph.getLists`."""
 
-    Attributes:
-        actor: Actor.
-        limit: Limit.
-        cursor: Cursor.
-    """
-
-    actor: str
-    cursor: t.Optional[str] = None
-    limit: t.Optional[int] = None
+    actor: str  #: Actor.
+    cursor: t.Optional[str] = None  #: Cursor.
+    limit: t.Optional[int] = None  #: Limit.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.graph.getFollows`.
+    """Output data model for :obj:`app.bsky.graph.getLists`."""
 
-    Attributes:
-        subject: Subject.
-        cursor: Cursor.
-        follows: Follows.
-    """
-
-    follows: t.List['models.AppBskyActorDefs.ProfileView']
-    subject: 'models.AppBskyActorDefs.ProfileView'
-    cursor: t.Optional[str] = None
+    lists: t.List['models.AppBskyGraphDefs.ListView']  #: Lists.
+    cursor: t.Optional[str] = None  #: Cursor.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_list.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/get_record.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,41 +4,31 @@
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 import typing as t
 from dataclasses import dataclass
 
-from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.graph.getList`.
+    """Parameters model for :obj:`com.atproto.repo.getRecord`."""
 
-    Attributes:
-        list: List.
-        limit: Limit.
-        cursor: Cursor.
-    """
-
-    list: str
-    cursor: t.Optional[str] = None
-    limit: t.Optional[int] = None
+    collection: str  #: The NSID of the record collection.
+    repo: str  #: The handle or DID of the repo.
+    rkey: str  #: The key of the record.
+    cid: t.Optional[
+        str
+    ] = None  #: The CID of the version of the record. If not specified, then return the most recent version.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.graph.getList`.
+    """Output data model for :obj:`com.atproto.repo.getRecord`."""
 
-    Attributes:
-        cursor: Cursor.
-        list: List.
-        items: Items.
-    """
-
-    items: t.List['models.AppBskyGraphDefs.ListItemView']
-    list: 'models.AppBskyGraphDefs.ListView'
-    cursor: t.Optional[str] = None
+    uri: str  #: Uri.
+    value: 'base.RecordModelBase'  #: Value.
+    cid: t.Optional[str] = None  #: Cid.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_list_mutes.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/search_repos.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,30 +11,22 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.graph.getListMutes`.
+    """Parameters model for :obj:`com.atproto.admin.searchRepos`."""
 
-    Attributes:
-        limit: Limit.
-        cursor: Cursor.
-    """
-
-    cursor: t.Optional[str] = None
-    limit: t.Optional[int] = None
+    cursor: t.Optional[str] = None  #: Cursor.
+    invitedBy: t.Optional[str] = None  #: Invited by.
+    limit: t.Optional[int] = None  #: Limit.
+    term: t.Optional[str] = None  #: Term.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.graph.getListMutes`.
-
-    Attributes:
-        cursor: Cursor.
-        lists: Lists.
-    """
+    """Output data model for :obj:`com.atproto.admin.searchRepos`."""
 
-    lists: t.List['models.AppBskyGraphDefs.ListView']
-    cursor: t.Optional[str] = None
+    repos: t.List['models.ComAtprotoAdminDefs.RepoView']  #: Repos.
+    cursor: t.Optional[str] = None  #: Cursor.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_lists.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_actor_feeds.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,32 +11,21 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.graph.getLists`.
+    """Parameters model for :obj:`app.bsky.feed.getActorFeeds`."""
 
-    Attributes:
-        actor: Actor.
-        limit: Limit.
-        cursor: Cursor.
-    """
-
-    actor: str
-    cursor: t.Optional[str] = None
-    limit: t.Optional[int] = None
+    actor: str  #: Actor.
+    cursor: t.Optional[str] = None  #: Cursor.
+    limit: t.Optional[int] = None  #: Limit.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.graph.getLists`.
+    """Output data model for :obj:`app.bsky.feed.getActorFeeds`."""
 
-    Attributes:
-        cursor: Cursor.
-        lists: Lists.
-    """
-
-    lists: t.List['models.AppBskyGraphDefs.ListView']
-    cursor: t.Optional[str] = None
+    feeds: t.List['models.AppBskyFeedDefs.GeneratorView']  #: Feeds.
+    cursor: t.Optional[str] = None  #: Cursor.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,30 +11,21 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.graph.getMutes`.
+    """Parameters model for :obj:`com.atproto.admin.getInviteCodes`."""
 
-    Attributes:
-        limit: Limit.
-        cursor: Cursor.
-    """
-
-    cursor: t.Optional[str] = None
-    limit: t.Optional[int] = None
+    cursor: t.Optional[str] = None  #: Cursor.
+    limit: t.Optional[int] = None  #: Limit.
+    sort: t.Optional[str] = None  #: Sort.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.graph.getMutes`.
-
-    Attributes:
-        cursor: Cursor.
-        mutes: Mutes.
-    """
+    """Output data model for :obj:`com.atproto.admin.getInviteCodes`."""
 
-    mutes: t.List['models.AppBskyActorDefs.ProfileView']
-    cursor: t.Optional[str] = None
+    codes: t.List['models.ComAtprotoServerDefs.InviteCode']  #: Codes.
+    cursor: t.Optional[str] = None  #: Cursor.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/list.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/list.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,26 +12,17 @@
 from atproto.xrpc_client.models import base
 from atproto.xrpc_client.models.blob_ref import BlobRef
 
 
 @dataclass
 class Main(base.RecordModelBase):
 
-    """Record model for :obj:`app.bsky.graph.list`.
+    """Record model for :obj:`app.bsky.graph.list`."""
 
-    Attributes:
-        purpose: Purpose.
-        name: Name.
-        description: Description.
-        descriptionFacets: Description facets.
-        avatar: Avatar.
-        createdAt: Created at.
-    """
-
-    createdAt: str
-    name: str
-    purpose: 'models.AppBskyGraphDefs.ListPurpose'
-    avatar: t.Optional[BlobRef] = None
-    description: t.Optional[str] = None
-    descriptionFacets: t.Optional[t.List['models.AppBskyRichtextFacet.Main']] = None
+    createdAt: str  #: Created at.
+    name: str  #: Name.
+    purpose: 'models.AppBskyGraphDefs.ListPurpose'  #: Purpose.
+    avatar: t.Optional[BlobRef] = None  #: Avatar.
+    description: t.Optional[str] = None  #: Description.
+    descriptionFacets: t.Optional[t.List['models.AppBskyRichtextFacet.Main']] = None  #: Description facets.
 
     _type: str = 'app.bsky.graph.list'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/listitem.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/listitem.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,20 +9,14 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Main(base.RecordModelBase):
 
-    """Record model for :obj:`app.bsky.graph.listitem`.
+    """Record model for :obj:`app.bsky.graph.listitem`."""
 
-    Attributes:
-        subject: Subject.
-        list: List.
-        createdAt: Created at.
-    """
-
-    createdAt: str
-    list: str
-    subject: str
+    createdAt: str  #: Created at.
+    list: str  #: List.
+    subject: str  #: Subject.
 
     _type: str = 'app.bsky.graph.listitem'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,10 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
-    """Input data model for :obj:`app.bsky.graph.muteActor`.
+    """Input data model for :obj:`app.bsky.graph.unmuteActor`."""
 
-    Attributes:
-        actor: Actor.
-    """
-
-    actor: str
+    actor: str  #: Actor.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/mute_actor_list.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/disable_account_invites.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,10 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
-    """Input data model for :obj:`app.bsky.graph.muteActorList`.
+    """Input data model for :obj:`com.atproto.admin.disableAccountInvites`."""
 
-    Attributes:
-        list: List.
-    """
-
-    list: str
+    account: str  #: Account.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,10 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
-    """Input data model for :obj:`app.bsky.graph.unmuteActor`.
+    """Input data model for :obj:`app.bsky.graph.muteActor`."""
 
-    Attributes:
-        actor: Actor.
-    """
-
-    actor: str
+    actor: str  #: Actor.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/unmute_actor_list.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/mute_actor_list.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,10 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
-    """Input data model for :obj:`app.bsky.graph.unmuteActorList`.
+    """Input data model for :obj:`app.bsky.graph.muteActorList`."""
 
-    Attributes:
-        list: List.
-    """
-
-    list: str
+    list: str  #: List.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,26 +10,18 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.notification.getUnreadCount`.
+    """Parameters model for :obj:`app.bsky.notification.getUnreadCount`."""
 
-    Attributes:
-        seenAt: Seen at.
-    """
-
-    seenAt: t.Optional[str] = None
+    seenAt: t.Optional[str] = None  #: Seen at.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.notification.getUnreadCount`.
-
-    Attributes:
-        count: Count.
-    """
+    """Output data model for :obj:`app.bsky.notification.getUnreadCount`."""
 
-    count: int
+    count: int  #: Count.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/notification/update_seen.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/notification/update_seen.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,10 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
-    """Input data model for :obj:`app.bsky.notification.updateSeen`.
+    """Input data model for :obj:`app.bsky.notification.updateSeen`."""
 
-    Attributes:
-        seenAt: Seen at.
-    """
-
-    seenAt: str
+    seenAt: str  #: Seen at.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/richtext/facet.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/richtext/facet.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,64 +11,46 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Main(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.richtext.facet`.
-
-    Attributes:
-        index: Index.
-        features: Features.
-    """
+    """Definition model for :obj:`app.bsky.richtext.facet`."""
 
     features: t.List[
         t.Union['models.AppBskyRichtextFacet.Mention', 'models.AppBskyRichtextFacet.Link', 't.Dict[str, t.Any]']
-    ]
-    index: 'models.AppBskyRichtextFacet.ByteSlice'
+    ]  #: Features.
+    index: 'models.AppBskyRichtextFacet.ByteSlice'  #: Index.
 
     _type: str = 'app.bsky.richtext.facet'
 
 
 @dataclass
 class Mention(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.richtext.facet`. A facet feature for actor mentions.
-
-    Attributes:
-        did: Did.
-    """
+    """Definition model for :obj:`app.bsky.richtext.facet`. A facet feature for actor mentions."""
 
-    did: str
+    did: str  #: Did.
 
     _type: str = 'app.bsky.richtext.facet#mention'
 
 
 @dataclass
 class Link(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.richtext.facet`. A facet feature for links.
+    """Definition model for :obj:`app.bsky.richtext.facet`. A facet feature for links."""
 
-    Attributes:
-        uri: Uri.
-    """
-
-    uri: str
+    uri: str  #: Uri.
 
     _type: str = 'app.bsky.richtext.facet#link'
 
 
 @dataclass
 class ByteSlice(base.ModelBase):
 
-    """Definition model for :obj:`app.bsky.richtext.facet`. A text segment. Start is inclusive, end is exclusive. Indices are for utf8-encoded strings.
-
-    Attributes:
-        byteStart: Byte start.
-        byteEnd: Byte end.
-    """
+    """Definition model for :obj:`app.bsky.richtext.facet`. A text segment. Start is inclusive, end is exclusive. Indices are for utf8-encoded strings."""
 
-    byteEnd: int
-    byteStart: int
+    byteEnd: int  #: Byte end.
+    byteStart: int  #: Byte start.
 
     _type: str = 'app.bsky.richtext.facet#byteSlice'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,32 +11,21 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.unspecced.getPopular`.
+    """Parameters model for :obj:`app.bsky.unspecced.getPopular`."""
 
-    Attributes:
-        includeNsfw: Include nsfw.
-        limit: Limit.
-        cursor: Cursor.
-    """
-
-    cursor: t.Optional[str] = None
-    includeNsfw: t.Optional[bool] = None
-    limit: t.Optional[int] = None
+    cursor: t.Optional[str] = None  #: Cursor.
+    includeNsfw: t.Optional[bool] = None  #: Include nsfw.
+    limit: t.Optional[int] = None  #: Limit.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.unspecced.getPopular`.
+    """Output data model for :obj:`app.bsky.unspecced.getPopular`."""
 
-    Attributes:
-        cursor: Cursor.
-        feed: Feed.
-    """
-
-    feed: t.List['models.AppBskyFeedDefs.FeedViewPost']
-    cursor: t.Optional[str] = None
+    feed: t.List['models.AppBskyFeedDefs.FeedViewPost']  #: Feed.
+    cursor: t.Optional[str] = None  #: Cursor.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/base.py` & `atproto-0.0.8/atproto/xrpc_client/models/base.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/blob_ref.py` & `atproto-0.0.8/atproto/xrpc_client/models/blob_ref.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/disable_account_invites.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,14 +9,10 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
-    """Input data model for :obj:`com.atproto.admin.disableAccountInvites`.
+    """Input data model for :obj:`com.atproto.server.revokeAppPassword`."""
 
-    Attributes:
-        account: Account.
-    """
-
-    account: str
+    name: str  #: Name.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,16 +10,19 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
-    """Input data model for :obj:`com.atproto.admin.disableInviteCodes`.
+    """Input data model for :obj:`com.atproto.server.createInviteCode`."""
 
-    Attributes:
-        codes: Codes.
-        accounts: Accounts.
-    """
+    useCount: int  #: Use count.
+    forAccount: t.Optional[str] = None  #: For account.
 
-    accounts: t.Optional[t.List[str]] = None
-    codes: t.Optional[t.List[str]] = None
+
+@dataclass
+class Response(base.ResponseModelBase):
+
+    """Output data model for :obj:`com.atproto.server.createInviteCode`."""
+
+    code: str  #: Code.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/enable_account_invites.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_feed_generator.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,20 +3,27 @@
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 from dataclasses import dataclass
 
+from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
-class Data(base.DataModelBase):
+class Params(base.ParamsModelBase):
 
-    """Input data model for :obj:`com.atproto.admin.enableAccountInvites`.
+    """Parameters model for :obj:`app.bsky.feed.getFeedGenerator`."""
 
-    Attributes:
-        account: Account.
-    """
+    feed: str  #: Feed.
 
-    account: str
+
+@dataclass
+class Response(base.ResponseModelBase):
+
+    """Output data model for :obj:`app.bsky.feed.getFeedGenerator`."""
+
+    isOnline: bool  #: Is online.
+    isValid: bool  #: Is valid.
+    view: 'models.AppBskyFeedDefs.GeneratorView'  #: View.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,32 +11,21 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.admin.getInviteCodes`.
+    """Parameters model for :obj:`com.atproto.admin.getModerationActions`."""
 
-    Attributes:
-        sort: Sort.
-        limit: Limit.
-        cursor: Cursor.
-    """
-
-    cursor: t.Optional[str] = None
-    limit: t.Optional[int] = None
-    sort: t.Optional[str] = None
+    cursor: t.Optional[str] = None  #: Cursor.
+    limit: t.Optional[int] = None  #: Limit.
+    subject: t.Optional[str] = None  #: Subject.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`com.atproto.admin.getInviteCodes`.
+    """Output data model for :obj:`com.atproto.admin.getModerationActions`."""
 
-    Attributes:
-        cursor: Cursor.
-        codes: Codes.
-    """
-
-    codes: t.List['models.ComAtprotoServerDefs.InviteCode']
-    cursor: t.Optional[str] = None
+    actions: t.List['models.ComAtprotoAdminDefs.ActionView']  #: Actions.
+    cursor: t.Optional[str] = None  #: Cursor.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,18 +11,14 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.admin.getModerationAction`.
+    """Parameters model for :obj:`com.atproto.admin.getModerationAction`."""
 
-    Attributes:
-        id: Id.
-    """
-
-    id: int
+    id: int  #: Id.
 
 
 #: Response reference to :obj:`models.ComAtprotoAdminDefs.ActionViewDetail` model.
 ResponseRef: t.Type[models.ComAtprotoAdminDefs.ActionViewDetail] = models.ComAtprotoAdminDefs.ActionViewDetail
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,34 +9,18 @@
 from dataclasses import dataclass
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
-class Params(base.ParamsModelBase):
+class Data(base.DataModelBase):
 
-    """Parameters model for :obj:`com.atproto.admin.getModerationActions`.
+    """Input data model for :obj:`com.atproto.admin.resolveModerationReports`."""
 
-    Attributes:
-        subject: Subject.
-        limit: Limit.
-        cursor: Cursor.
-    """
-
-    cursor: t.Optional[str] = None
-    limit: t.Optional[int] = None
-    subject: t.Optional[str] = None
+    actionId: int  #: Action id.
+    createdBy: str  #: Created by.
+    reportIds: t.List[int]  #: Report ids.
 
 
-@dataclass
-class Response(base.ResponseModelBase):
-
-    """Output data model for :obj:`com.atproto.admin.getModerationActions`.
-
-    Attributes:
-        cursor: Cursor.
-        actions: Actions.
-    """
-
-    actions: t.List['models.ComAtprotoAdminDefs.ActionView']
-    cursor: t.Optional[str] = None
+#: Response reference to :obj:`models.ComAtprotoAdminDefs.ActionView` model.
+ResponseRef: t.Type[models.ComAtprotoAdminDefs.ActionView] = models.ComAtprotoAdminDefs.ActionView
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,18 +11,14 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.admin.getModerationReport`.
+    """Parameters model for :obj:`com.atproto.admin.getModerationReport`."""
 
-    Attributes:
-        id: Id.
-    """
-
-    id: int
+    id: int  #: Id.
 
 
 #: Response reference to :obj:`models.ComAtprotoAdminDefs.ReportViewDetail` model.
 ResponseRef: t.Type[models.ComAtprotoAdminDefs.ReportViewDetail] = models.ComAtprotoAdminDefs.ReportViewDetail
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,36 +11,23 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.admin.getModerationReports`.
+    """Parameters model for :obj:`com.atproto.admin.getModerationReports`."""
 
-    Attributes:
-        subject: Subject.
-        resolved: Resolved.
-        actionType: Action type.
-        limit: Limit.
-        cursor: Cursor.
-    """
-
-    actionType: t.Optional[str] = None
-    cursor: t.Optional[str] = None
-    limit: t.Optional[int] = None
-    resolved: t.Optional[bool] = None
-    subject: t.Optional[str] = None
+    actionType: t.Optional[str] = None  #: Action type.
+    cursor: t.Optional[str] = None  #: Cursor.
+    limit: t.Optional[int] = None  #: Limit.
+    resolved: t.Optional[bool] = None  #: Resolved.
+    subject: t.Optional[str] = None  #: Subject.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`com.atproto.admin.getModerationReports`.
+    """Output data model for :obj:`com.atproto.admin.getModerationReports`."""
 
-    Attributes:
-        cursor: Cursor.
-        reports: Reports.
-    """
-
-    reports: t.List['models.ComAtprotoAdminDefs.ReportView']
-    cursor: t.Optional[str] = None
+    reports: t.List['models.ComAtprotoAdminDefs.ReportView']  #: Reports.
+    cursor: t.Optional[str] = None  #: Cursor.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_record.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_record.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,20 +11,15 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.admin.getRecord`.
+    """Parameters model for :obj:`com.atproto.admin.getRecord`."""
 
-    Attributes:
-        uri: Uri.
-        cid: Cid.
-    """
-
-    uri: str
-    cid: t.Optional[str] = None
+    uri: str  #: Uri.
+    cid: t.Optional[str] = None  #: Cid.
 
 
 #: Response reference to :obj:`models.ComAtprotoAdminDefs.RecordViewDetail` model.
 ResponseRef: t.Type[models.ComAtprotoAdminDefs.RecordViewDetail] = models.ComAtprotoAdminDefs.RecordViewDetail
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_repo.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_repo.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,18 +11,14 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.admin.getRepo`.
+    """Parameters model for :obj:`com.atproto.admin.getRepo`."""
 
-    Attributes:
-        did: Did.
-    """
-
-    did: str
+    did: str  #: Did.
 
 
 #: Response reference to :obj:`models.ComAtprotoAdminDefs.RepoViewDetail` model.
 ResponseRef: t.Type[models.ComAtprotoAdminDefs.RepoViewDetail] = models.ComAtprotoAdminDefs.RepoViewDetail
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 from dataclasses import dataclass
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
-class Data(base.DataModelBase):
+class Response(base.ResponseModelBase):
 
-    """Input data model for :obj:`com.atproto.admin.resolveModerationReports`.
+    """Output data model for :obj:`com.atproto.server.listAppPasswords`."""
 
-    Attributes:
-        actionId: Action id.
-        reportIds: Report ids.
-        createdBy: Created by.
-    """
+    passwords: t.List['models.ComAtprotoServerListAppPasswords.AppPassword']  #: Passwords.
 
-    actionId: int
-    createdBy: str
-    reportIds: t.List[int]
 
+@dataclass
+class AppPassword(base.ModelBase):
+
+    """Definition model for :obj:`com.atproto.server.listAppPasswords`."""
+
+    createdAt: str  #: Created at.
+    name: str  #: Name.
 
-#: Response reference to :obj:`models.ComAtprotoAdminDefs.ActionView` model.
-ResponseRef: t.Type[models.ComAtprotoAdminDefs.ActionView] = models.ComAtprotoAdminDefs.ActionView
+    _type: str = 'com.atproto.server.listAppPasswords#appPassword'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,22 +11,16 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
-    """Input data model for :obj:`com.atproto.admin.reverseModerationAction`.
+    """Input data model for :obj:`com.atproto.admin.reverseModerationAction`."""
 
-    Attributes:
-        id: Id.
-        reason: Reason.
-        createdBy: Created by.
-    """
-
-    createdBy: str
-    id: int
-    reason: str
+    createdBy: str  #: Created by.
+    id: int  #: Id.
+    reason: str  #: Reason.
 
 
 #: Response reference to :obj:`models.ComAtprotoAdminDefs.ActionView` model.
 ResponseRef: t.Type[models.ComAtprotoAdminDefs.ActionView] = models.ComAtprotoAdminDefs.ActionView
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/search_repos.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,34 +11,24 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.admin.searchRepos`.
+    """Parameters model for :obj:`app.bsky.feed.getRepostedBy`."""
 
-    Attributes:
-        term: Term.
-        invitedBy: Invited by.
-        limit: Limit.
-        cursor: Cursor.
-    """
-
-    cursor: t.Optional[str] = None
-    invitedBy: t.Optional[str] = None
-    limit: t.Optional[int] = None
-    term: t.Optional[str] = None
+    uri: str  #: Uri.
+    cid: t.Optional[str] = None  #: Cid.
+    cursor: t.Optional[str] = None  #: Cursor.
+    limit: t.Optional[int] = None  #: Limit.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`com.atproto.admin.searchRepos`.
+    """Output data model for :obj:`app.bsky.feed.getRepostedBy`."""
 
-    Attributes:
-        cursor: Cursor.
-        repos: Repos.
-    """
-
-    repos: t.List['models.ComAtprotoAdminDefs.RepoView']
-    cursor: t.Optional[str] = None
+    repostedBy: t.List['models.AppBskyActorDefs.ProfileView']  #: Reposted by.
+    uri: str  #: Uri.
+    cid: t.Optional[str] = None  #: Cid.
+    cursor: t.Optional[str] = None  #: Cursor.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,30 +11,22 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
-    """Input data model for :obj:`com.atproto.admin.takeModerationAction`.
+    """Input data model for :obj:`com.atproto.admin.takeModerationAction`."""
 
-    Attributes:
-        action: Action.
-        subject: Subject.
-        subjectBlobCids: Subject blob cids.
-        createLabelVals: Create label vals.
-        negateLabelVals: Negate label vals.
-        reason: Reason.
-        createdBy: Created by.
-    """
-
-    action: str
-    createdBy: str
-    reason: str
-    subject: t.Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main', 't.Dict[str, t.Any]']
-    createLabelVals: t.Optional[t.List[str]] = None
-    negateLabelVals: t.Optional[t.List[str]] = None
-    subjectBlobCids: t.Optional[t.List[str]] = None
+    action: str  #: Action.
+    createdBy: str  #: Created by.
+    reason: str  #: Reason.
+    subject: t.Union[
+        'models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main', 't.Dict[str, t.Any]'
+    ]  #: Subject.
+    createLabelVals: t.Optional[t.List[str]] = None  #: Create label vals.
+    negateLabelVals: t.Optional[t.List[str]] = None  #: Negate label vals.
+    subjectBlobCids: t.Optional[t.List[str]] = None  #: Subject blob cids.
 
 
 #: Response reference to :obj:`models.ComAtprotoAdminDefs.ActionView` model.
 ResponseRef: t.Type[models.ComAtprotoAdminDefs.ActionView] = models.ComAtprotoAdminDefs.ActionView
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/enable_account_invites.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,16 +9,10 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
-    """Input data model for :obj:`com.atproto.admin.updateAccountEmail`.
+    """Input data model for :obj:`com.atproto.admin.enableAccountInvites`."""
 
-    Attributes:
-        account: The handle or DID of the repo.
-        email: Email.
-    """
-
-    account: str
-    email: str
+    account: str  #: Account.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,16 +9,11 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
-    """Input data model for :obj:`com.atproto.admin.updateAccountHandle`.
+    """Input data model for :obj:`com.atproto.admin.updateAccountHandle`."""
 
-    Attributes:
-        did: Did.
-        handle: Handle.
-    """
-
-    did: str
-    handle: str
+    did: str  #: Did.
+    handle: str  #: Handle.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,26 +10,18 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.identity.resolveHandle`.
+    """Parameters model for :obj:`com.atproto.identity.resolveHandle`."""
 
-    Attributes:
-        handle: The handle to resolve. If not supplied, will resolve the host's own handle.
-    """
-
-    handle: t.Optional[str] = None
+    handle: t.Optional[str] = None  #: The handle to resolve. If not supplied, will resolve the host's own handle.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`com.atproto.identity.resolveHandle`.
-
-    Attributes:
-        did: Did.
-    """
+    """Output data model for :obj:`com.atproto.identity.resolveHandle`."""
 
-    did: str
+    did: str  #: Did.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/identity/update_handle.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/reset_password.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,11 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
-    """Input data model for :obj:`com.atproto.identity.updateHandle`.
+    """Input data model for :obj:`com.atproto.server.resetPassword`."""
 
-    Attributes:
-        handle: Handle.
-    """
-
-    handle: str
+    password: str  #: Password.
+    token: str  #: Token.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/label/defs.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/label/defs.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,26 +10,19 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Label(base.ModelBase):
 
-    """Definition model for :obj:`com.atproto.label.defs`. Metadata tag on an atproto resource (eg, repo or record)
+    """Definition model for :obj:`com.atproto.label.defs`. Metadata tag on an atproto resource (eg, repo or record)"""
 
-    Attributes:
-        src: DID of the actor who created this label.
-        uri: AT URI of the record, repository (account), or other resource which this label applies to.
-        cid: optionally, CID specifying the specific version of 'uri' resource this label applies to.
-        val: the short string name of the value or type of this label.
-        neg: if true, this is a negation label, overwriting a previous label.
-        cts: timestamp when this label was created.
-    """
-
-    cts: str
-    src: str
-    uri: str
-    val: str
-    cid: t.Optional[str] = None
-    neg: t.Optional[bool] = None
+    cts: str  #: timestamp when this label was created.
+    src: str  #: DID of the actor who created this label.
+    uri: str  #: AT URI of the record, repository (account), or other resource which this label applies to.
+    val: str  #: the short string name of the value or type of this label.
+    cid: t.Optional[
+        str
+    ] = None  #: optionally, CID specifying the specific version of 'uri' resource this label applies to.
+    neg: t.Optional[bool] = None  #: if true, this is a negation label, overwriting a previous label.
 
     _type: str = 'com.atproto.label.defs#label'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/label/query_labels.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/label/query_labels.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,34 +11,24 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.label.queryLabels`.
+    """Parameters model for :obj:`com.atproto.label.queryLabels`."""
 
-    Attributes:
-        uriPatterns: List of AT URI patterns to match (boolean 'OR'). Each may be a prefix (ending with '*'; will match inclusive of the string leading to '*'), or a full URI.
-        sources: Optional list of label sources (DIDs) to filter on.
-        limit: Limit.
-        cursor: Cursor.
-    """
-
-    uriPatterns: t.List[str]
-    cursor: t.Optional[str] = None
-    limit: t.Optional[int] = None
-    sources: t.Optional[t.List[str]] = None
+    uriPatterns: t.List[
+        str
+    ]  #: List of AT URI patterns to match (boolean 'OR'). Each may be a prefix (ending with '*'; will match inclusive of the string leading to '*'), or a full URI.
+    cursor: t.Optional[str] = None  #: Cursor.
+    limit: t.Optional[int] = None  #: Limit.
+    sources: t.Optional[t.List[str]] = None  #: Optional list of label sources (DIDs) to filter on.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`com.atproto.label.queryLabels`.
+    """Output data model for :obj:`com.atproto.label.queryLabels`."""
 
-    Attributes:
-        cursor: Cursor.
-        labels: Labels.
-    """
-
-    labels: t.List['models.ComAtprotoLabelDefs.Label']
-    cursor: t.Optional[str] = None
+    labels: t.List['models.ComAtprotoLabelDefs.Label']  #: Labels.
+    cursor: t.Optional[str] = None  #: Cursor.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,36 +9,38 @@
 from dataclasses import dataclass
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
-class Labels(base.ModelBase):
+class Params(base.ParamsModelBase):
 
-    """Definition model for :obj:`com.atproto.label.subscribeLabels`.
+    """Parameters model for :obj:`com.atproto.label.subscribeLabels`.
 
     Attributes:
-        seq: Seq.
-        labels: Labels.
+        cursor: The last known event to backfill from.
     """
 
-    labels: t.List['models.ComAtprotoLabelDefs.Label']
-    seq: int
+    cursor: t.Optional[int] = None
+
+
+@dataclass
+class Labels(base.ModelBase):
+
+    """Definition model for :obj:`com.atproto.label.subscribeLabels`."""
+
+    labels: t.List['models.ComAtprotoLabelDefs.Label']  #: Labels.
+    seq: int  #: Seq.
 
     _type: str = 'com.atproto.label.subscribeLabels#labels'
 
 
 @dataclass
 class Info(base.ModelBase):
 
-    """Definition model for :obj:`com.atproto.label.subscribeLabels`.
-
-    Attributes:
-        name: Name.
-        message: Message.
-    """
+    """Definition model for :obj:`com.atproto.label.subscribeLabels`."""
 
-    name: str
-    message: t.Optional[str] = None
+    name: str  #: Name.
+    message: t.Optional[str] = None  #: Message.
 
     _type: str = 'com.atproto.label.subscribeLabels#info'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/moderation/create_report.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/moderation/create_report.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,40 +11,29 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
-    """Input data model for :obj:`com.atproto.moderation.createReport`.
+    """Input data model for :obj:`com.atproto.moderation.createReport`."""
 
-    Attributes:
-        reasonType: Reason type.
-        reason: Reason.
-        subject: Subject.
-    """
-
-    reasonType: 'models.ComAtprotoModerationDefs.ReasonType'
-    subject: t.Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main', 't.Dict[str, t.Any]']
-    reason: t.Optional[str] = None
+    reasonType: 'models.ComAtprotoModerationDefs.ReasonType'  #: Reason type.
+    subject: t.Union[
+        'models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main', 't.Dict[str, t.Any]'
+    ]  #: Subject.
+    reason: t.Optional[str] = None  #: Reason.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`com.atproto.moderation.createReport`.
+    """Output data model for :obj:`com.atproto.moderation.createReport`."""
 
-    Attributes:
-        id: Id.
-        reasonType: Reason type.
-        reason: Reason.
-        subject: Subject.
-        reportedBy: Reported by.
-        createdAt: Created at.
-    """
-
-    createdAt: str
-    id: int
-    reasonType: 'models.ComAtprotoModerationDefs.ReasonType'
-    reportedBy: str
-    subject: t.Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main', 't.Dict[str, t.Any]']
-    reason: t.Optional[str] = None
+    createdAt: str  #: Created at.
+    id: int  #: Id.
+    reasonType: 'models.ComAtprotoModerationDefs.ReasonType'  #: Reason type.
+    reportedBy: str  #: Reported by.
+    subject: t.Union[
+        'models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main', 't.Dict[str, t.Any]'
+    ]  #: Subject.
+    reason: t.Optional[str] = None  #: Reason.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/moderation/defs.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/moderation/defs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,79 +11,55 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
-    """Input data model for :obj:`com.atproto.repo.applyWrites`.
+    """Input data model for :obj:`com.atproto.repo.applyWrites`."""
 
-    Attributes:
-        repo: The handle or DID of the repo.
-        validate: Validate the records?
-        writes: Writes.
-        swapCommit: Swap commit.
-    """
-
-    repo: str
+    repo: str  #: The handle or DID of the repo.
     writes: t.List[
         t.Union[
             'models.ComAtprotoRepoApplyWrites.Create',
             'models.ComAtprotoRepoApplyWrites.Update',
             'models.ComAtprotoRepoApplyWrites.Delete',
             't.Dict[str, t.Any]',
         ]
-    ]
-    swapCommit: t.Optional[str] = None
-    validate: t.Optional[bool] = None
+    ]  #: Writes.
+    swapCommit: t.Optional[str] = None  #: Swap commit.
+    validate: t.Optional[bool] = None  #: Validate the records?
 
 
 @dataclass
 class Create(base.ModelBase):
 
-    """Definition model for :obj:`com.atproto.repo.applyWrites`. Create a new record.
+    """Definition model for :obj:`com.atproto.repo.applyWrites`. Create a new record."""
 
-    Attributes:
-        collection: Collection.
-        rkey: Rkey.
-        value: Value.
-    """
-
-    collection: str
-    value: 'base.RecordModelBase'
-    rkey: t.Optional[str] = None
+    collection: str  #: Collection.
+    value: 'base.RecordModelBase'  #: Value.
+    rkey: t.Optional[str] = None  #: Rkey.
 
     _type: str = 'com.atproto.repo.applyWrites#create'
 
 
 @dataclass
 class Update(base.ModelBase):
 
-    """Definition model for :obj:`com.atproto.repo.applyWrites`. Update an existing record.
+    """Definition model for :obj:`com.atproto.repo.applyWrites`. Update an existing record."""
 
-    Attributes:
-        collection: Collection.
-        rkey: Rkey.
-        value: Value.
-    """
-
-    collection: str
-    rkey: str
-    value: 'base.RecordModelBase'
+    collection: str  #: Collection.
+    rkey: str  #: Rkey.
+    value: 'base.RecordModelBase'  #: Value.
 
     _type: str = 'com.atproto.repo.applyWrites#update'
 
 
 @dataclass
 class Delete(base.ModelBase):
 
-    """Definition model for :obj:`com.atproto.repo.applyWrites`. Delete an existing record.
-
-    Attributes:
-        collection: Collection.
-        rkey: Rkey.
-    """
+    """Definition model for :obj:`com.atproto.repo.applyWrites`. Delete an existing record."""
 
-    collection: str
-    rkey: str
+    collection: str  #: Collection.
+    rkey: str  #: Rkey.
 
     _type: str = 'com.atproto.repo.applyWrites#delete'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/create_record.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/create_record.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,38 +10,24 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
-    """Input data model for :obj:`com.atproto.repo.createRecord`.
+    """Input data model for :obj:`com.atproto.repo.createRecord`."""
 
-    Attributes:
-        repo: The handle or DID of the repo.
-        collection: The NSID of the record collection.
-        rkey: The key of the record.
-        validate: Validate the record?
-        record: The record to create.
-        swapCommit: Compare and swap with the previous commit by cid.
-    """
-
-    collection: str
-    record: 'base.RecordModelBase'
-    repo: str
-    rkey: t.Optional[str] = None
-    swapCommit: t.Optional[str] = None
-    validate: t.Optional[bool] = None
+    collection: str  #: The NSID of the record collection.
+    record: 'base.RecordModelBase'  #: The record to create.
+    repo: str  #: The handle or DID of the repo.
+    rkey: t.Optional[str] = None  #: The key of the record.
+    swapCommit: t.Optional[str] = None  #: Compare and swap with the previous commit by cid.
+    validate: t.Optional[bool] = None  #: Validate the record?
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`com.atproto.repo.createRecord`.
+    """Output data model for :obj:`com.atproto.repo.createRecord`."""
 
-    Attributes:
-        uri: Uri.
-        cid: Cid.
-    """
-
-    cid: str
-    uri: str
+    cid: str  #: Cid.
+    uri: str  #: Uri.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/delete_record.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/rebase_repo.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,22 +10,11 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
-    """Input data model for :obj:`com.atproto.repo.deleteRecord`.
+    """Input data model for :obj:`com.atproto.repo.rebaseRepo`."""
 
-    Attributes:
-        repo: The handle or DID of the repo.
-        collection: The NSID of the record collection.
-        rkey: The key of the record.
-        swapRecord: Compare and swap with the previous record by cid.
-        swapCommit: Compare and swap with the previous commit by cid.
-    """
-
-    collection: str
-    repo: str
-    rkey: str
-    swapCommit: t.Optional[str] = None
-    swapRecord: t.Optional[str] = None
+    repo: str  #: The handle or DID of the repo.
+    swapCommit: t.Optional[str] = None  #: Compare and swap with the previous commit by cid.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,34 +10,22 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.repo.describeRepo`.
+    """Parameters model for :obj:`com.atproto.repo.describeRepo`."""
 
-    Attributes:
-        repo: The handle or DID of the repo.
-    """
-
-    repo: str
+    repo: str  #: The handle or DID of the repo.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`com.atproto.repo.describeRepo`.
+    """Output data model for :obj:`com.atproto.repo.describeRepo`."""
 
-    Attributes:
-        handle: Handle.
-        did: Did.
-        didDoc: Did doc.
-        collections: Collections.
-        handleIsCorrect: Handle is correct.
-    """
-
-    collections: t.List[str]
-    did: str
-    didDoc: 'base.RecordModelBase'
-    handle: str
-    handleIsCorrect: bool
+    collections: t.List[str]  #: Collections.
+    did: str  #: Did.
+    didDoc: 'base.RecordModelBase'  #: Did doc.
+    handle: str  #: Handle.
+    handleIsCorrect: bool  #: Handle is correct.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/get_record.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,42 +4,38 @@
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 import typing as t
 from dataclasses import dataclass
 
+from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
-class Params(base.ParamsModelBase):
+class Data(base.DataModelBase):
 
-    """Parameters model for :obj:`com.atproto.repo.getRecord`.
+    """Input data model for :obj:`com.atproto.server.createInviteCodes`."""
 
-    Attributes:
-        repo: The handle or DID of the repo.
-        collection: The NSID of the record collection.
-        rkey: The key of the record.
-        cid: The CID of the version of the record. If not specified, then return the most recent version.
-    """
-
-    collection: str
-    repo: str
-    rkey: str
-    cid: t.Optional[str] = None
+    codeCount: int  #: Code count.
+    useCount: int  #: Use count.
+    forAccounts: t.Optional[t.List[str]] = None  #: For accounts.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`com.atproto.repo.getRecord`.
+    """Output data model for :obj:`com.atproto.server.createInviteCodes`."""
 
-    Attributes:
-        uri: Uri.
-        cid: Cid.
-        value: Value.
-    """
-
-    uri: str
-    value: 'base.RecordModelBase'
-    cid: t.Optional[str] = None
+    codes: t.List['models.ComAtprotoServerCreateInviteCodes.AccountCodes']  #: Codes.
+
+
+@dataclass
+class AccountCodes(base.ModelBase):
+
+    """Definition model for :obj:`com.atproto.server.createInviteCodes`."""
+
+    account: str  #: Account.
+    codes: t.List[str]  #: Codes.
+
+    _type: str = 'com.atproto.server.createInviteCodes#accountCodes'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/list_records.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/list_records.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,58 +11,37 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.repo.listRecords`.
+    """Parameters model for :obj:`com.atproto.repo.listRecords`."""
 
-    Attributes:
-        repo: The handle or DID of the repo.
-        collection: The NSID of the record type.
-        limit: The number of records to return.
-        cursor: Cursor.
-        rkeyStart: DEPRECATED: The lowest sort-ordered rkey to start from (exclusive).
-        rkeyEnd: DEPRECATED: The highest sort-ordered rkey to stop at (exclusive).
-        reverse: Reverse the order of the returned records?
-    """
-
-    collection: str
-    repo: str
-    cursor: t.Optional[str] = None
-    limit: t.Optional[int] = None
-    reverse: t.Optional[bool] = None
-    rkeyEnd: t.Optional[str] = None
-    rkeyStart: t.Optional[str] = None
+    collection: str  #: The NSID of the record type.
+    repo: str  #: The handle or DID of the repo.
+    cursor: t.Optional[str] = None  #: Cursor.
+    limit: t.Optional[int] = None  #: The number of records to return.
+    reverse: t.Optional[bool] = None  #: Reverse the order of the returned records?
+    rkeyEnd: t.Optional[str] = None  #: DEPRECATED: The highest sort-ordered rkey to stop at (exclusive).
+    rkeyStart: t.Optional[str] = None  #: DEPRECATED: The lowest sort-ordered rkey to start from (exclusive).
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`com.atproto.repo.listRecords`.
+    """Output data model for :obj:`com.atproto.repo.listRecords`."""
 
-    Attributes:
-        cursor: Cursor.
-        records: Records.
-    """
-
-    records: t.List['models.ComAtprotoRepoListRecords.Record']
-    cursor: t.Optional[str] = None
+    records: t.List['models.ComAtprotoRepoListRecords.Record']  #: Records.
+    cursor: t.Optional[str] = None  #: Cursor.
 
 
 @dataclass
 class Record(base.ModelBase):
 
-    """Definition model for :obj:`com.atproto.repo.listRecords`.
+    """Definition model for :obj:`com.atproto.repo.listRecords`."""
 
-    Attributes:
-        uri: Uri.
-        cid: Cid.
-        value: Value.
-    """
-
-    cid: str
-    uri: str
-    value: 'base.RecordModelBase'
+    cid: str  #: Cid.
+    uri: str  #: Uri.
+    value: 'base.RecordModelBase'  #: Value.
 
     _type: str = 'com.atproto.repo.listRecords#record'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/put_record.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/generator.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,46 +4,25 @@
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 import typing as t
 from dataclasses import dataclass
 
+from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
+from atproto.xrpc_client.models.blob_ref import BlobRef
 
 
 @dataclass
-class Data(base.DataModelBase):
+class Main(base.RecordModelBase):
 
-    """Input data model for :obj:`com.atproto.repo.putRecord`.
+    """Record model for :obj:`app.bsky.feed.generator`."""
 
-    Attributes:
-        repo: The handle or DID of the repo.
-        collection: The NSID of the record collection.
-        rkey: The key of the record.
-        validate: Validate the record?
-        record: The record to write.
-        swapRecord: Compare and swap with the previous record by cid.
-        swapCommit: Compare and swap with the previous commit by cid.
-    """
-
-    collection: str
-    record: 'base.RecordModelBase'
-    repo: str
-    rkey: str
-    swapCommit: t.Optional[str] = None
-    swapRecord: t.Optional[str] = None
-    validate: t.Optional[bool] = None
+    createdAt: str  #: Created at.
+    did: str  #: Did.
+    displayName: str  #: Display name.
+    avatar: t.Optional[BlobRef] = None  #: Avatar.
+    description: t.Optional[str] = None  #: Description.
+    descriptionFacets: t.Optional[t.List['models.AppBskyRichtextFacet.Main']] = None  #: Description facets.
 
-
-@dataclass
-class Response(base.ResponseModelBase):
-
-    """Output data model for :obj:`com.atproto.repo.putRecord`.
-
-    Attributes:
-        uri: Uri.
-        cid: Cid.
-    """
-
-    cid: str
-    uri: str
+    _type: str = 'app.bsky.feed.generator'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/rebase_repo.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 import typing as t
 from dataclasses import dataclass
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
-class Data(base.DataModelBase):
+class Params(base.ParamsModelBase):
 
-    """Input data model for :obj:`com.atproto.repo.rebaseRepo`.
+    """Parameters model for :obj:`com.atproto.sync.getCheckout`."""
 
-    Attributes:
-        repo: The handle or DID of the repo.
-        swapCommit: Compare and swap with the previous commit by cid.
-    """
+    did: str  #: The DID of the repo.
+    commit: t.Optional[str] = None  #: The commit to get the checkout from. Defaults to current HEAD.
 
-    repo: str
-    swapCommit: t.Optional[str] = None
+
+#: Response raw data type.
+Response: t.Union[t.Type[str], t.Type[bytes]] = bytes
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,10 @@
 #: Data raw data type.
 Data: t.Union[t.Type[str], t.Type[bytes]] = bytes
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`com.atproto.repo.uploadBlob`.
+    """Output data model for :obj:`com.atproto.repo.uploadBlob`."""
 
-    Attributes:
-        blob: Blob.
-    """
-
-    blob: BlobRef
+    blob: BlobRef  #: Blob.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/create_account.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/create_account.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,42 +10,26 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
-    """Input data model for :obj:`com.atproto.server.createAccount`.
+    """Input data model for :obj:`com.atproto.server.createAccount`."""
 
-    Attributes:
-        email: Email.
-        handle: Handle.
-        did: Did.
-        inviteCode: Invite code.
-        password: Password.
-        recoveryKey: Recovery key.
-    """
-
-    email: str
-    handle: str
-    password: str
-    did: t.Optional[str] = None
-    inviteCode: t.Optional[str] = None
-    recoveryKey: t.Optional[str] = None
+    email: str  #: Email.
+    handle: str  #: Handle.
+    password: str  #: Password.
+    did: t.Optional[str] = None  #: Did.
+    inviteCode: t.Optional[str] = None  #: Invite code.
+    recoveryKey: t.Optional[str] = None  #: Recovery key.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`com.atproto.server.createAccount`.
+    """Output data model for :obj:`com.atproto.server.createAccount`."""
 
-    Attributes:
-        accessJwt: Access jwt.
-        refreshJwt: Refresh jwt.
-        handle: Handle.
-        did: Did.
-    """
-
-    accessJwt: str
-    did: str
-    handle: str
-    refreshJwt: str
+    accessJwt: str  #: Access jwt.
+    did: str  #: Did.
+    handle: str  #: Handle.
+    refreshJwt: str  #: Refresh jwt.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/create_app_password.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_head.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,26 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
-import typing as t
 from dataclasses import dataclass
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
-class Data(base.DataModelBase):
+class Params(base.ParamsModelBase):
 
-    """Input data model for :obj:`com.atproto.server.createAppPassword`.
+    """Parameters model for :obj:`com.atproto.sync.getHead`."""
 
-    Attributes:
-        name: Name.
-    """
-
-    name: str
+    did: str  #: The DID of the repo.
 
 
 @dataclass
-class AppPassword(base.ModelBase):
-
-    """Definition model for :obj:`com.atproto.server.createAppPassword`.
-
-    Attributes:
-        name: Name.
-        password: Password.
-        createdAt: Created at.
-    """
-
-    createdAt: str
-    name: str
-    password: str
-
-    _type: str = 'com.atproto.server.createAppPassword#appPassword'
+class Response(base.ResponseModelBase):
 
+    """Output data model for :obj:`com.atproto.sync.getHead`."""
 
-#: Response reference to :obj:`AppPassword` model.
-ResponseRef: t.Type[AppPassword] = AppPassword
+    root: str  #: Root.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/defs.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,34 +4,36 @@
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 import typing as t
 from dataclasses import dataclass
 
+from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
-class Data(base.DataModelBase):
+class InviteCode(base.ModelBase):
 
-    """Input data model for :obj:`com.atproto.server.createInviteCode`.
+    """Definition model for :obj:`com.atproto.server.defs`."""
 
-    Attributes:
-        useCount: Use count.
-        forAccount: For account.
-    """
+    available: int  #: Available.
+    code: str  #: Code.
+    createdAt: str  #: Created at.
+    createdBy: str  #: Created by.
+    disabled: bool  #: Disabled.
+    forAccount: str  #: For account.
+    uses: t.List['models.ComAtprotoServerDefs.InviteCodeUse']  #: Uses.
 
-    useCount: int
-    forAccount: t.Optional[str] = None
+    _type: str = 'com.atproto.server.defs#inviteCode'
 
 
 @dataclass
-class Response(base.ResponseModelBase):
+class InviteCodeUse(base.ModelBase):
 
-    """Output data model for :obj:`com.atproto.server.createInviteCode`.
+    """Definition model for :obj:`com.atproto.server.defs`."""
 
-    Attributes:
-        code: Code.
-    """
+    usedAt: str  #: Used at.
+    usedBy: str  #: Used by.
 
-    code: str
+    _type: str = 'com.atproto.server.defs#inviteCodeUse'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/delete_account.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/get_session.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
-class Data(base.DataModelBase):
+class Response(base.ResponseModelBase):
 
-    """Input data model for :obj:`com.atproto.server.deleteAccount`.
+    """Output data model for :obj:`com.atproto.server.getSession`."""
 
-    Attributes:
-        did: Did.
-        password: Password.
-        token: Token.
-    """
-
-    did: str
-    password: str
-    token: str
+    did: str  #: Did.
+    handle: str  #: Handle.
+    email: t.Optional[str] = None  #: Email.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/describe_server.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/describe_server.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,34 +11,23 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`com.atproto.server.describeServer`.
+    """Output data model for :obj:`com.atproto.server.describeServer`."""
 
-    Attributes:
-        inviteCodeRequired: Invite code required.
-        availableUserDomains: Available user domains.
-        links: Links.
-    """
-
-    availableUserDomains: t.List[str]
-    inviteCodeRequired: t.Optional[bool] = None
-    links: t.Optional['models.ComAtprotoServerDescribeServer.Links'] = None
+    availableUserDomains: t.List[str]  #: Available user domains.
+    inviteCodeRequired: t.Optional[bool] = None  #: Invite code required.
+    links: t.Optional['models.ComAtprotoServerDescribeServer.Links'] = None  #: Links.
 
 
 @dataclass
 class Links(base.ModelBase):
 
-    """Definition model for :obj:`com.atproto.server.describeServer`.
+    """Definition model for :obj:`com.atproto.server.describeServer`."""
 
-    Attributes:
-        privacyPolicy: Privacy policy.
-        termsOfService: Terms of service.
-    """
-
-    privacyPolicy: t.Optional[str] = None
-    termsOfService: t.Optional[str] = None
+    privacyPolicy: t.Optional[str] = None  #: Privacy policy.
+    termsOfService: t.Optional[str] = None  #: Terms of service.
 
     _type: str = 'com.atproto.server.describeServer#links'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,28 +11,19 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.server.getAccountInviteCodes`.
+    """Parameters model for :obj:`com.atproto.server.getAccountInviteCodes`."""
 
-    Attributes:
-        includeUsed: Include used.
-        createAvailable: Create available.
-    """
-
-    createAvailable: t.Optional[bool] = None
-    includeUsed: t.Optional[bool] = None
+    createAvailable: t.Optional[bool] = None  #: Create available.
+    includeUsed: t.Optional[bool] = None  #: Include used.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`com.atproto.server.getAccountInviteCodes`.
-
-    Attributes:
-        codes: Codes.
-    """
+    """Output data model for :obj:`com.atproto.server.getAccountInviteCodes`."""
 
-    codes: t.List['models.ComAtprotoServerDefs.InviteCode']
+    codes: t.List['models.ComAtprotoServerDefs.InviteCode']  #: Codes.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/refresh_session.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/refresh_session.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,20 +9,13 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`com.atproto.server.refreshSession`.
+    """Output data model for :obj:`com.atproto.server.refreshSession`."""
 
-    Attributes:
-        accessJwt: Access jwt.
-        refreshJwt: Refresh jwt.
-        handle: Handle.
-        did: Did.
-    """
-
-    accessJwt: str
-    did: str
-    handle: str
-    refreshJwt: str
+    accessJwt: str  #: Access jwt.
+    did: str  #: Did.
+    handle: str  #: Handle.
+    refreshJwt: str  #: Refresh jwt.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/unmute_actor_list.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,10 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
-    """Input data model for :obj:`com.atproto.server.requestPasswordReset`.
+    """Input data model for :obj:`app.bsky.graph.unmuteActorList`."""
 
-    Attributes:
-        email: Email.
-    """
-
-    email: str
+    list: str  #: List.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/reset_password.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/delete_account.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,16 +9,12 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
-    """Input data model for :obj:`com.atproto.server.resetPassword`.
+    """Input data model for :obj:`com.atproto.server.deleteAccount`."""
 
-    Attributes:
-        token: Token.
-        password: Password.
-    """
-
-    password: str
-    token: str
+    did: str  #: Did.
+    password: str  #: Password.
+    token: str  #: Token.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_blob.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_blob.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,20 +10,15 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.sync.getBlob`.
+    """Parameters model for :obj:`com.atproto.sync.getBlob`."""
 
-    Attributes:
-        did: The DID of the repo.
-        cid: The CID of the blob to fetch.
-    """
-
-    cid: str
-    did: str
+    cid: str  #: The CID of the blob to fetch.
+    did: str  #: The DID of the repo.
 
 
 #: Response raw data type.
 Response: t.Union[t.Type[str], t.Type[bytes]] = bytes
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,20 +10,15 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.sync.getBlocks`.
+    """Parameters model for :obj:`com.atproto.sync.getBlocks`."""
 
-    Attributes:
-        did: The DID of the repo.
-        cids: Cids.
-    """
-
-    cids: t.List[str]
-    did: str
+    cids: t.List[str]  #: Cids.
+    did: str  #: The DID of the repo.
 
 
 #: Response raw data type.
 Response: t.Union[t.Type[str], t.Type[bytes]] = bytes
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_record.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,20 +10,17 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.sync.getCheckout`.
+    """Parameters model for :obj:`com.atproto.sync.getRecord`."""
 
-    Attributes:
-        did: The DID of the repo.
-        commit: The commit to get the checkout from. Defaults to current HEAD.
-    """
-
-    did: str
-    commit: t.Optional[str] = None
+    collection: str  #: Collection.
+    did: str  #: The DID of the repo.
+    rkey: str  #: Rkey.
+    commit: t.Optional[str] = None  #: An optional past commit CID.
 
 
 #: Response raw data type.
 Response: t.Union[t.Type[str], t.Type[bytes]] = bytes
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,30 +10,20 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.sync.getCommitPath`.
+    """Parameters model for :obj:`com.atproto.sync.getCommitPath`."""
 
-    Attributes:
-        did: The DID of the repo.
-        latest: The most recent commit.
-        earliest: The earliest commit to start from.
-    """
-
-    did: str
-    earliest: t.Optional[str] = None
-    latest: t.Optional[str] = None
+    did: str  #: The DID of the repo.
+    earliest: t.Optional[str] = None  #: The earliest commit to start from.
+    latest: t.Optional[str] = None  #: The most recent commit.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`com.atproto.sync.getCommitPath`.
+    """Output data model for :obj:`com.atproto.sync.getCommitPath`."""
 
-    Attributes:
-        commits: Commits.
-    """
-
-    commits: t.List[str]
+    commits: t.List[str]  #: Commits.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_repo.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_repo.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,22 +10,16 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.sync.getRepo`.
+    """Parameters model for :obj:`com.atproto.sync.getRepo`."""
 
-    Attributes:
-        did: The DID of the repo.
-        earliest: The earliest commit in the commit range (not inclusive).
-        latest: The latest commit in the commit range (inclusive).
-    """
-
-    did: str
-    earliest: t.Optional[str] = None
-    latest: t.Optional[str] = None
+    did: str  #: The DID of the repo.
+    earliest: t.Optional[str] = None  #: The earliest commit in the commit range (not inclusive).
+    latest: t.Optional[str] = None  #: The latest commit in the commit range (inclusive).
 
 
 #: Response raw data type.
 Response: t.Union[t.Type[str], t.Type[bytes]] = bytes
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py` & `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/get_list_mutes.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,36 +4,27 @@
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 import typing as t
 from dataclasses import dataclass
 
+from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.sync.listBlobs`.
+    """Parameters model for :obj:`app.bsky.graph.getListMutes`."""
 
-    Attributes:
-        did: The DID of the repo.
-        latest: The most recent commit.
-        earliest: The earliest commit to start from.
-    """
-
-    did: str
-    earliest: t.Optional[str] = None
-    latest: t.Optional[str] = None
+    cursor: t.Optional[str] = None  #: Cursor.
+    limit: t.Optional[int] = None  #: Limit.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`com.atproto.sync.listBlobs`.
+    """Output data model for :obj:`app.bsky.graph.getListMutes`."""
 
-    Attributes:
-        cids: Cids.
-    """
-
-    cids: t.List[str]
+    lists: t.List['models.AppBskyGraphDefs.ListView']  #: Lists.
+    cursor: t.Optional[str] = None  #: Cursor.
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/list_repos.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/list_repos.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,46 +11,31 @@
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.sync.listRepos`.
+    """Parameters model for :obj:`com.atproto.sync.listRepos`."""
 
-    Attributes:
-        limit: Limit.
-        cursor: Cursor.
-    """
-
-    cursor: t.Optional[str] = None
-    limit: t.Optional[int] = None
+    cursor: t.Optional[str] = None  #: Cursor.
+    limit: t.Optional[int] = None  #: Limit.
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`com.atproto.sync.listRepos`.
-
-    Attributes:
-        cursor: Cursor.
-        repos: Repos.
-    """
+    """Output data model for :obj:`com.atproto.sync.listRepos`."""
 
-    repos: t.List['models.ComAtprotoSyncListRepos.Repo']
-    cursor: t.Optional[str] = None
+    repos: t.List['models.ComAtprotoSyncListRepos.Repo']  #: Repos.
+    cursor: t.Optional[str] = None  #: Cursor.
 
 
 @dataclass
 class Repo(base.ModelBase):
 
-    """Definition model for :obj:`com.atproto.sync.listRepos`.
-
-    Attributes:
-        did: Did.
-        head: Head.
-    """
+    """Definition model for :obj:`com.atproto.sync.listRepos`."""
 
-    did: str
-    head: str
+    did: str  #: Did.
+    head: str  #: Head.
 
     _type: str = 'com.atproto.sync.listRepos#repo'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py` & `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,128 +10,96 @@
 
 from atproto import CID
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
-class Commit(base.ModelBase):
+class Params(base.ParamsModelBase):
 
-    """Definition model for :obj:`com.atproto.sync.subscribeRepos`.
+    """Parameters model for :obj:`com.atproto.sync.subscribeRepos`.
 
     Attributes:
-        seq: Seq.
-        rebase: Rebase.
-        tooBig: Too big.
-        repo: Repo.
-        commit: Commit.
-        prev: Prev.
-        blocks: CAR file containing relevant blocks.
-        ops: Ops.
-        blobs: Blobs.
-        time: Time.
+        cursor: The last known event to backfill from.
     """
 
-    blobs: t.List[CID]
-    blocks: t.Union[str, bytes]
-    commit: CID
-    ops: t.List['models.ComAtprotoSyncSubscribeRepos.RepoOp']
-    rebase: bool
-    repo: str
-    seq: int
-    time: str
-    tooBig: bool
-    prev: t.Optional[CID] = None
+    cursor: t.Optional[int] = None
+
+
+@dataclass
+class Commit(base.ModelBase):
+
+    """Definition model for :obj:`com.atproto.sync.subscribeRepos`."""
+
+    blobs: t.List[CID]  #: Blobs.
+    blocks: t.Union[str, bytes]  #: CAR file containing relevant blocks.
+    commit: CID  #: Commit.
+    ops: t.List['models.ComAtprotoSyncSubscribeRepos.RepoOp']  #: Ops.
+    rebase: bool  #: Rebase.
+    repo: str  #: Repo.
+    seq: int  #: Seq.
+    time: str  #: Time.
+    tooBig: bool  #: Too big.
+    prev: t.Optional[CID] = None  #: Prev.
 
     _type: str = 'com.atproto.sync.subscribeRepos#commit'
 
 
 @dataclass
 class Handle(base.ModelBase):
 
-    """Definition model for :obj:`com.atproto.sync.subscribeRepos`.
+    """Definition model for :obj:`com.atproto.sync.subscribeRepos`."""
 
-    Attributes:
-        seq: Seq.
-        did: Did.
-        handle: Handle.
-        time: Time.
-    """
-
-    did: str
-    handle: str
-    seq: int
-    time: str
+    did: str  #: Did.
+    handle: str  #: Handle.
+    seq: int  #: Seq.
+    time: str  #: Time.
 
     _type: str = 'com.atproto.sync.subscribeRepos#handle'
 
 
 @dataclass
 class Migrate(base.ModelBase):
 
-    """Definition model for :obj:`com.atproto.sync.subscribeRepos`.
-
-    Attributes:
-        seq: Seq.
-        did: Did.
-        migrateTo: Migrate to.
-        time: Time.
-    """
+    """Definition model for :obj:`com.atproto.sync.subscribeRepos`."""
 
-    did: str
-    seq: int
-    time: str
-    migrateTo: t.Optional[str] = None
+    did: str  #: Did.
+    seq: int  #: Seq.
+    time: str  #: Time.
+    migrateTo: t.Optional[str] = None  #: Migrate to.
 
     _type: str = 'com.atproto.sync.subscribeRepos#migrate'
 
 
 @dataclass
 class Tombstone(base.ModelBase):
 
-    """Definition model for :obj:`com.atproto.sync.subscribeRepos`.
-
-    Attributes:
-        seq: Seq.
-        did: Did.
-        time: Time.
-    """
+    """Definition model for :obj:`com.atproto.sync.subscribeRepos`."""
 
-    did: str
-    seq: int
-    time: str
+    did: str  #: Did.
+    seq: int  #: Seq.
+    time: str  #: Time.
 
     _type: str = 'com.atproto.sync.subscribeRepos#tombstone'
 
 
 @dataclass
 class Info(base.ModelBase):
 
-    """Definition model for :obj:`com.atproto.sync.subscribeRepos`.
+    """Definition model for :obj:`com.atproto.sync.subscribeRepos`."""
 
-    Attributes:
-        name: Name.
-        message: Message.
-    """
-
-    name: str
-    message: t.Optional[str] = None
+    name: str  #: Name.
+    message: t.Optional[str] = None  #: Message.
 
     _type: str = 'com.atproto.sync.subscribeRepos#info'
 
 
 @dataclass
 class RepoOp(base.ModelBase):
 
-    """Definition model for :obj:`com.atproto.sync.subscribeRepos`.
-
-    Attributes:
-        action: Action.
-        path: Path.
-        cid: Cid.
-    """
+    """Definition model for :obj:`com.atproto.sync.subscribeRepos`."""
 
-    action: str
-    path: str
-    cid: t.Optional[CID] = None
+    action: str  #: Action.
+    path: str  #: Path.
+    cid: t.Optional[CID] = None  #: Cid.
 
     _type: str = 'com.atproto.sync.subscribeRepos#repoOp'
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/type_conversion.py` & `atproto-0.0.8/atproto/xrpc_client/models/type_conversion.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from atproto.xrpc_client import models
 
 RECORD_TYPE_TO_MODEL_CLASS = {
+    'app.bsky.feed.generator': models.AppBskyFeedGenerator.Main,
     'app.bsky.actor.profile': models.AppBskyActorProfile.Main,
     'app.bsky.feed.repost': models.AppBskyFeedRepost.Main,
     'app.bsky.graph.listitem': models.AppBskyGraphListitem.Main,
     'app.bsky.feed.like': models.AppBskyFeedLike.Main,
     'app.bsky.graph.follow': models.AppBskyGraphFollow.Main,
     'app.bsky.graph.list': models.AppBskyGraphList.Main,
     'app.bsky.graph.block': models.AppBskyGraphBlock.Main,
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/models/utils.py` & `atproto-0.0.8/atproto/xrpc_client/models/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import dataclasses
 import json
 import typing as t
+from enum import Enum
 
 from dacite import Config, exceptions, from_dict
 
 from atproto.cid import CID
 from atproto.exceptions import (
     MissingValueError,
     ModelError,
@@ -23,20 +24,27 @@
 
 
 def _record_model_type_hook(data: dict) -> RecordModelBase:
     record_type = data.pop('$type')
     return get_or_create_model(data, RECORD_TYPE_TO_MODEL_CLASS[record_type])
 
 
+def _decode_cid_hook(ref: t.Union[CID, str]) -> CID:
+    if isinstance(ref, CID):
+        return ref
+
+    return CID.decode(ref)
+
+
 _TYPE_HOOKS = {
     BlobRef: lambda ref: BlobRef.from_dict(ref),
-    CID: lambda ref: CID.decode(ref),
+    CID: _decode_cid_hook,
     RecordModelBase: _record_model_type_hook,
 }
-_DACITE_CONFIG = Config(type_hooks=_TYPE_HOOKS)
+_DACITE_CONFIG = Config(cast=[Enum], type_hooks=_TYPE_HOOKS)
 
 
 def get_or_create_model(model_data: t.Union[dict], model: t.Type[M]) -> t.Optional[M]:
     if model_data is None:
         return None
 
     if isinstance(model_data, model):
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/namespaces/async_ns.py` & `atproto-0.0.8/atproto/xrpc_client/namespaces/async_ns.py`

 * *Files 3% similar despite different names*

```diff
@@ -189,14 +189,277 @@
         response = await self._client.invoke_query(
             'app.bsky.actor.searchActorsTypeahead', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyActorSearchActorsTypeahead.Response)
 
 
 @dataclass
+class FeedNamespace(NamespaceBase):
+    async def describe_feed_generator(self, **kwargs) -> models.AppBskyFeedDescribeFeedGenerator.Response:
+        """Returns information about a given feed generator including TOS & offered feed URIs.
+
+        Args:
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedDescribeFeedGenerator.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        response = await self._client.invoke_query(
+            'app.bsky.feed.describeFeedGenerator', output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedDescribeFeedGenerator.Response)
+
+    async def get_actor_feeds(
+        self, params: t.Union[dict, 'models.AppBskyFeedGetActorFeeds.Params'], **kwargs
+    ) -> models.AppBskyFeedGetActorFeeds.Response:
+        """Retrieve a list of feeds created by a given actor.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetActorFeeds.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetActorFeeds.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.feed.getActorFeeds', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetActorFeeds.Response)
+
+    async def get_author_feed(
+        self, params: t.Union[dict, 'models.AppBskyFeedGetAuthorFeed.Params'], **kwargs
+    ) -> models.AppBskyFeedGetAuthorFeed.Response:
+        """A view of an actor's feed.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetAuthorFeed.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetAuthorFeed.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.feed.getAuthorFeed', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetAuthorFeed.Response)
+
+    async def get_feed(
+        self, params: t.Union[dict, 'models.AppBskyFeedGetFeed.Params'], **kwargs
+    ) -> models.AppBskyFeedGetFeed.Response:
+        """Compose and hydrate a feed from a user's selected feed generator.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetFeed.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetFeed.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.feed.getFeed', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetFeed.Response)
+
+    async def get_feed_generator(
+        self, params: t.Union[dict, 'models.AppBskyFeedGetFeedGenerator.Params'], **kwargs
+    ) -> models.AppBskyFeedGetFeedGenerator.Response:
+        """Get information about a specific feed offered by a feed generator, such as its online status.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetFeedGenerator.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetFeedGenerator.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.feed.getFeedGenerator', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetFeedGenerator.Response)
+
+    async def get_feed_generators(
+        self, params: t.Union[dict, 'models.AppBskyFeedGetFeedGenerators.Params'], **kwargs
+    ) -> models.AppBskyFeedGetFeedGenerators.Response:
+        """Get information about a list of feed generators.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetFeedGenerators.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetFeedGenerators.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.feed.getFeedGenerators', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetFeedGenerators.Response)
+
+    async def get_feed_skeleton(
+        self, params: t.Union[dict, 'models.AppBskyFeedGetFeedSkeleton.Params'], **kwargs
+    ) -> models.AppBskyFeedGetFeedSkeleton.Response:
+        """A skeleton of a feed provided by a feed generator.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetFeedSkeleton.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetFeedSkeleton.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.feed.getFeedSkeleton', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetFeedSkeleton.Response)
+
+    async def get_likes(
+        self, params: t.Union[dict, 'models.AppBskyFeedGetLikes.Params'], **kwargs
+    ) -> models.AppBskyFeedGetLikes.Response:
+        """Get likes.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetLikes.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetLikes.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.feed.getLikes', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetLikes.Response)
+
+    async def get_post_thread(
+        self, params: t.Union[dict, 'models.AppBskyFeedGetPostThread.Params'], **kwargs
+    ) -> models.AppBskyFeedGetPostThread.Response:
+        """Get post thread.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetPostThread.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetPostThread.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.feed.getPostThread', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetPostThread.Response)
+
+    async def get_posts(
+        self, params: t.Union[dict, 'models.AppBskyFeedGetPosts.Params'], **kwargs
+    ) -> models.AppBskyFeedGetPosts.Response:
+        """A view of an actor's feed.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetPosts.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetPosts.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.feed.getPosts', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetPosts.Response)
+
+    async def get_reposted_by(
+        self, params: t.Union[dict, 'models.AppBskyFeedGetRepostedBy.Params'], **kwargs
+    ) -> models.AppBskyFeedGetRepostedBy.Response:
+        """Get reposted by.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetRepostedBy.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetRepostedBy.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.feed.getRepostedBy', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetRepostedBy.Response)
+
+    async def get_timeline(
+        self, params: t.Optional[t.Union[dict, 'models.AppBskyFeedGetTimeline.Params']] = None, **kwargs
+    ) -> models.AppBskyFeedGetTimeline.Response:
+        """A view of the user's home timeline.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetTimeline.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetTimeline.Params)
+        response = await self._client.invoke_query(
+            'app.bsky.feed.getTimeline', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetTimeline.Response)
+
+
+@dataclass
 class GraphNamespace(NamespaceBase):
     async def get_blocks(
         self, params: t.Optional[t.Union[dict, 'models.AppBskyGraphGetBlocks.Params']] = None, **kwargs
     ) -> models.AppBskyGraphGetBlocks.Response:
         """Who is the requester's account blocking?
 
         Args:
@@ -426,149 +689,14 @@
         response = await self._client.invoke_procedure(
             'app.bsky.graph.unmuteActorList', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
 
 @dataclass
-class FeedNamespace(NamespaceBase):
-    async def get_author_feed(
-        self, params: t.Union[dict, 'models.AppBskyFeedGetAuthorFeed.Params'], **kwargs
-    ) -> models.AppBskyFeedGetAuthorFeed.Response:
-        """A view of an actor's feed.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyFeedGetAuthorFeed.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyFeedGetAuthorFeed.Params)
-        response = await self._client.invoke_query(
-            'app.bsky.feed.getAuthorFeed', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyFeedGetAuthorFeed.Response)
-
-    async def get_likes(
-        self, params: t.Union[dict, 'models.AppBskyFeedGetLikes.Params'], **kwargs
-    ) -> models.AppBskyFeedGetLikes.Response:
-        """Get likes.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyFeedGetLikes.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyFeedGetLikes.Params)
-        response = await self._client.invoke_query(
-            'app.bsky.feed.getLikes', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyFeedGetLikes.Response)
-
-    async def get_post_thread(
-        self, params: t.Union[dict, 'models.AppBskyFeedGetPostThread.Params'], **kwargs
-    ) -> models.AppBskyFeedGetPostThread.Response:
-        """Get post thread.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyFeedGetPostThread.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyFeedGetPostThread.Params)
-        response = await self._client.invoke_query(
-            'app.bsky.feed.getPostThread', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyFeedGetPostThread.Response)
-
-    async def get_posts(
-        self, params: t.Union[dict, 'models.AppBskyFeedGetPosts.Params'], **kwargs
-    ) -> models.AppBskyFeedGetPosts.Response:
-        """A view of an actor's feed.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyFeedGetPosts.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyFeedGetPosts.Params)
-        response = await self._client.invoke_query(
-            'app.bsky.feed.getPosts', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyFeedGetPosts.Response)
-
-    async def get_reposted_by(
-        self, params: t.Union[dict, 'models.AppBskyFeedGetRepostedBy.Params'], **kwargs
-    ) -> models.AppBskyFeedGetRepostedBy.Response:
-        """Get reposted by.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyFeedGetRepostedBy.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyFeedGetRepostedBy.Params)
-        response = await self._client.invoke_query(
-            'app.bsky.feed.getRepostedBy', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyFeedGetRepostedBy.Response)
-
-    async def get_timeline(
-        self, params: t.Optional[t.Union[dict, 'models.AppBskyFeedGetTimeline.Params']] = None, **kwargs
-    ) -> models.AppBskyFeedGetTimeline.Response:
-        """A view of the user's home timeline.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyFeedGetTimeline.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyFeedGetTimeline.Params)
-        response = await self._client.invoke_query(
-            'app.bsky.feed.getTimeline', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyFeedGetTimeline.Response)
-
-
-@dataclass
 class UnspeccedNamespace(NamespaceBase):
     async def get_popular(
         self, params: t.Optional[t.Union[dict, 'models.AppBskyUnspeccedGetPopular.Params']] = None, **kwargs
     ) -> models.AppBskyUnspeccedGetPopular.Response:
         """An unspecced view of globally popular items.
 
         Args:
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/namespaces/sync_ns.py` & `atproto-0.0.8/atproto/xrpc_client/namespaces/sync_ns.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,14 +189,277 @@
         response = self._client.invoke_query(
             'app.bsky.actor.searchActorsTypeahead', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyActorSearchActorsTypeahead.Response)
 
 
 @dataclass
+class FeedNamespace(NamespaceBase):
+    def describe_feed_generator(self, **kwargs) -> models.AppBskyFeedDescribeFeedGenerator.Response:
+        """Returns information about a given feed generator including TOS & offered feed URIs.
+
+        Args:
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedDescribeFeedGenerator.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        response = self._client.invoke_query(
+            'app.bsky.feed.describeFeedGenerator', output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedDescribeFeedGenerator.Response)
+
+    def get_actor_feeds(
+        self, params: t.Union[dict, 'models.AppBskyFeedGetActorFeeds.Params'], **kwargs
+    ) -> models.AppBskyFeedGetActorFeeds.Response:
+        """Retrieve a list of feeds created by a given actor.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetActorFeeds.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetActorFeeds.Params)
+        response = self._client.invoke_query(
+            'app.bsky.feed.getActorFeeds', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetActorFeeds.Response)
+
+    def get_author_feed(
+        self, params: t.Union[dict, 'models.AppBskyFeedGetAuthorFeed.Params'], **kwargs
+    ) -> models.AppBskyFeedGetAuthorFeed.Response:
+        """A view of an actor's feed.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetAuthorFeed.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetAuthorFeed.Params)
+        response = self._client.invoke_query(
+            'app.bsky.feed.getAuthorFeed', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetAuthorFeed.Response)
+
+    def get_feed(
+        self, params: t.Union[dict, 'models.AppBskyFeedGetFeed.Params'], **kwargs
+    ) -> models.AppBskyFeedGetFeed.Response:
+        """Compose and hydrate a feed from a user's selected feed generator.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetFeed.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetFeed.Params)
+        response = self._client.invoke_query(
+            'app.bsky.feed.getFeed', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetFeed.Response)
+
+    def get_feed_generator(
+        self, params: t.Union[dict, 'models.AppBskyFeedGetFeedGenerator.Params'], **kwargs
+    ) -> models.AppBskyFeedGetFeedGenerator.Response:
+        """Get information about a specific feed offered by a feed generator, such as its online status.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetFeedGenerator.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetFeedGenerator.Params)
+        response = self._client.invoke_query(
+            'app.bsky.feed.getFeedGenerator', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetFeedGenerator.Response)
+
+    def get_feed_generators(
+        self, params: t.Union[dict, 'models.AppBskyFeedGetFeedGenerators.Params'], **kwargs
+    ) -> models.AppBskyFeedGetFeedGenerators.Response:
+        """Get information about a list of feed generators.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetFeedGenerators.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetFeedGenerators.Params)
+        response = self._client.invoke_query(
+            'app.bsky.feed.getFeedGenerators', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetFeedGenerators.Response)
+
+    def get_feed_skeleton(
+        self, params: t.Union[dict, 'models.AppBskyFeedGetFeedSkeleton.Params'], **kwargs
+    ) -> models.AppBskyFeedGetFeedSkeleton.Response:
+        """A skeleton of a feed provided by a feed generator.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetFeedSkeleton.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetFeedSkeleton.Params)
+        response = self._client.invoke_query(
+            'app.bsky.feed.getFeedSkeleton', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetFeedSkeleton.Response)
+
+    def get_likes(
+        self, params: t.Union[dict, 'models.AppBskyFeedGetLikes.Params'], **kwargs
+    ) -> models.AppBskyFeedGetLikes.Response:
+        """Get likes.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetLikes.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetLikes.Params)
+        response = self._client.invoke_query(
+            'app.bsky.feed.getLikes', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetLikes.Response)
+
+    def get_post_thread(
+        self, params: t.Union[dict, 'models.AppBskyFeedGetPostThread.Params'], **kwargs
+    ) -> models.AppBskyFeedGetPostThread.Response:
+        """Get post thread.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetPostThread.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetPostThread.Params)
+        response = self._client.invoke_query(
+            'app.bsky.feed.getPostThread', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetPostThread.Response)
+
+    def get_posts(
+        self, params: t.Union[dict, 'models.AppBskyFeedGetPosts.Params'], **kwargs
+    ) -> models.AppBskyFeedGetPosts.Response:
+        """A view of an actor's feed.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetPosts.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetPosts.Params)
+        response = self._client.invoke_query(
+            'app.bsky.feed.getPosts', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetPosts.Response)
+
+    def get_reposted_by(
+        self, params: t.Union[dict, 'models.AppBskyFeedGetRepostedBy.Params'], **kwargs
+    ) -> models.AppBskyFeedGetRepostedBy.Response:
+        """Get reposted by.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetRepostedBy.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetRepostedBy.Params)
+        response = self._client.invoke_query(
+            'app.bsky.feed.getRepostedBy', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetRepostedBy.Response)
+
+    def get_timeline(
+        self, params: t.Optional[t.Union[dict, 'models.AppBskyFeedGetTimeline.Params']] = None, **kwargs
+    ) -> models.AppBskyFeedGetTimeline.Response:
+        """A view of the user's home timeline.
+
+        Args:
+            params: Parameters.
+            **kwargs: Arbitrary arguments to HTTP request.
+
+        Returns:
+            :obj:`models.AppBskyFeedGetTimeline.Response`: Output model.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        params = get_or_create_model(params, models.AppBskyFeedGetTimeline.Params)
+        response = self._client.invoke_query(
+            'app.bsky.feed.getTimeline', params=params, output_encoding='application/json', **kwargs
+        )
+        return get_response_model(response, models.AppBskyFeedGetTimeline.Response)
+
+
+@dataclass
 class GraphNamespace(NamespaceBase):
     def get_blocks(
         self, params: t.Optional[t.Union[dict, 'models.AppBskyGraphGetBlocks.Params']] = None, **kwargs
     ) -> models.AppBskyGraphGetBlocks.Response:
         """Who is the requester's account blocking?
 
         Args:
@@ -426,149 +689,14 @@
         response = self._client.invoke_procedure(
             'app.bsky.graph.unmuteActorList', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
 
 @dataclass
-class FeedNamespace(NamespaceBase):
-    def get_author_feed(
-        self, params: t.Union[dict, 'models.AppBskyFeedGetAuthorFeed.Params'], **kwargs
-    ) -> models.AppBskyFeedGetAuthorFeed.Response:
-        """A view of an actor's feed.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyFeedGetAuthorFeed.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyFeedGetAuthorFeed.Params)
-        response = self._client.invoke_query(
-            'app.bsky.feed.getAuthorFeed', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyFeedGetAuthorFeed.Response)
-
-    def get_likes(
-        self, params: t.Union[dict, 'models.AppBskyFeedGetLikes.Params'], **kwargs
-    ) -> models.AppBskyFeedGetLikes.Response:
-        """Get likes.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyFeedGetLikes.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyFeedGetLikes.Params)
-        response = self._client.invoke_query(
-            'app.bsky.feed.getLikes', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyFeedGetLikes.Response)
-
-    def get_post_thread(
-        self, params: t.Union[dict, 'models.AppBskyFeedGetPostThread.Params'], **kwargs
-    ) -> models.AppBskyFeedGetPostThread.Response:
-        """Get post thread.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyFeedGetPostThread.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyFeedGetPostThread.Params)
-        response = self._client.invoke_query(
-            'app.bsky.feed.getPostThread', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyFeedGetPostThread.Response)
-
-    def get_posts(
-        self, params: t.Union[dict, 'models.AppBskyFeedGetPosts.Params'], **kwargs
-    ) -> models.AppBskyFeedGetPosts.Response:
-        """A view of an actor's feed.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyFeedGetPosts.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyFeedGetPosts.Params)
-        response = self._client.invoke_query(
-            'app.bsky.feed.getPosts', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyFeedGetPosts.Response)
-
-    def get_reposted_by(
-        self, params: t.Union[dict, 'models.AppBskyFeedGetRepostedBy.Params'], **kwargs
-    ) -> models.AppBskyFeedGetRepostedBy.Response:
-        """Get reposted by.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyFeedGetRepostedBy.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyFeedGetRepostedBy.Params)
-        response = self._client.invoke_query(
-            'app.bsky.feed.getRepostedBy', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyFeedGetRepostedBy.Response)
-
-    def get_timeline(
-        self, params: t.Optional[t.Union[dict, 'models.AppBskyFeedGetTimeline.Params']] = None, **kwargs
-    ) -> models.AppBskyFeedGetTimeline.Response:
-        """A view of the user's home timeline.
-
-        Args:
-            params: Parameters.
-            **kwargs: Arbitrary arguments to HTTP request.
-
-        Returns:
-            :obj:`models.AppBskyFeedGetTimeline.Response`: Output model.
-
-        Raises:
-            :class:`atproto.exceptions.AtProtocolError`: Base exception.
-        """
-
-        params = get_or_create_model(params, models.AppBskyFeedGetTimeline.Params)
-        response = self._client.invoke_query(
-            'app.bsky.feed.getTimeline', params=params, output_encoding='application/json', **kwargs
-        )
-        return get_response_model(response, models.AppBskyFeedGetTimeline.Response)
-
-
-@dataclass
 class UnspeccedNamespace(NamespaceBase):
     def get_popular(
         self, params: t.Optional[t.Union[dict, 'models.AppBskyUnspeccedGetPopular.Params']] = None, **kwargs
     ) -> models.AppBskyUnspeccedGetPopular.Response:
         """An unspecced view of globally popular items.
 
         Args:
```

### Comparing `atproto-0.0.7/atproto/xrpc_client/request.py` & `atproto-0.0.8/atproto/xrpc_client/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 import json
 import typing as t
 from dataclasses import dataclass
 
 import httpx
 
 from atproto import exceptions
+from atproto.xrpc_client.models.common import XrpcError
 from atproto.xrpc_client.models.utils import get_or_create_model, is_json
 
 
 @dataclass
 class Response:
     success: bool
     status_code: int
     content: t.Optional[t.Union[dict, bytes, 'XrpcError']]
     headers: t.Dict[str, t.Any]
 
 
-@dataclass
-class XrpcError:
-    error: str
-    message: t.Optional[str]
-
-
 def _parse_response(response: httpx.Response) -> Response:
     content = response.content
     if response.headers.get('content-type') == 'application/json; charset=utf-8':
         content = response.json()
 
     return Response(
         success=True,
```

### Comparing `atproto-0.0.7/pyproject.toml` & `atproto-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "atproto"
-version = "0.0.7" # placeholder. Dynamic version from Git Tag
+version = "0.0.8" # placeholder. Dynamic version from Git Tag
 description = "The AT Protocol SDK"
 authors = ["Ilya (Marshal) <ilya@marshal.dev>"]
 license = "MIT"
 repository = "https://github.com/MarshalX/atproto"
 readme = "README.md"
 keywords = ["library", "sdk", "codegen", "xrpc", "xrpc-client", "atprotocol", "atproto", "lexicon", "parser", "schema", "bluesky", "bluesky-api", "at", "uri", "atp", "nsid", "did", "cid"]
 classifiers = [
@@ -35,14 +35,15 @@
 python = ">=3.7,<3.12"
 httpx = ">=0.24.0,<0.25.0"
 dacite = ">=1.8.0,<1.9.0"
 multiformats = ">=0.2.1,<0.3.0"
 typing-extensions = ">=4.5.0,<4.6.0"
 dag-cbor = ">=0.3.2,<0.4.0"
 pyjwt = ">=2.7.0,<2.8.0"
+httpx-ws = ">=0.3.1,<0.4.0"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 isort = "5.11.5"
 sphinx = "5.3.0"
```

### Comparing `atproto-0.0.7/PKG-INFO` & `atproto-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atproto
-Version: 0.0.7
+Version: 0.0.8
 Summary: The AT Protocol SDK
 Home-page: https://github.com/MarshalX/atproto
 License: MIT
 Keywords: library,sdk,codegen,xrpc,xrpc-client,atprotocol,atproto,lexicon,parser,schema,bluesky,bluesky-api,at,uri,atp,nsid,did,cid
 Author: Ilya (Marshal)
 Author-email: ilya@marshal.dev
 Requires-Python: >=3.7,<3.12
@@ -17,20 +17,26 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Pre-processors
 Requires-Dist: dacite (>=1.8.0,<1.9.0)
 Requires-Dist: dag-cbor (>=0.3.2,<0.4.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: httpx-ws (>=0.3.1,<0.4.0)
 Requires-Dist: multiformats (>=0.2.1,<0.3.0)
 Requires-Dist: pyjwt (>=2.7.0,<2.8.0)
 Requires-Dist: typing-extensions (>=4.5.0,<4.6.0)
 Project-URL: Author, https://github.com/MarshalX
 Project-URL: Documentation, https://atproto.blue
 Project-URL: Repository, https://github.com/MarshalX/atproto
 Project-URL: Tracker, https://github.com/MarshalX/atproto/issues
@@ -54,15 +60,15 @@
     <a href="https://discord.gg/PCyVJXU9jN">
         Discord Bluesky API
     </a>
 </p>
 
 ## The AT Protocol SDK
 
-> ⚠️ Under construction. The SDK was built from scratch in 40 hours. Somewhere I speedran. I have a list of things that will break backward compatibility. Until the 1.0.0 release, I am not going to care about it. 
+> ⚠️ Under construction. Until the 1.0.0 release, I am not going to care about backward compatibility between versions. 
 
 Code snippet:
 ```python
 from atproto import Client
 
 
 def main():
@@ -100,17 +106,19 @@
 if __name__ == '__main__':
     # use run() for higher Python version
     asyncio.get_event_loop().run_until_complete(main())
 
 ```
 </details>
 
+🔥[Firehose data streaming is available!](https://atproto.blue/en/latest/firehose.html)
+
 ### Introduction
 
-This SDK attempts to implement everything that provides ATProto. Due to the unstable state of the protocol (it grows and changes fast) and a bit of outdated documentation, only the client side is supported yet. There is support for Lexicon Schemes and XRPC clients for now. All models, queries, and procedures are generated automatically. The main focus is on the lexicons of atproto.com and bsky.app, but it doesn't have a vendor lock on it. Feel free to use the code generator for your own lexicon schemes. SDK also provides utilities to work with CID, NSID, URI. The support of IPLD (dag-cbor) will be added in the near future.
+This SDK attempts to implement everything that provides ATProto. Due to the unstable state of the protocol (it grows and changes fast) and a bit of outdated documentation, only the client side is supported yet. There is support for Lexicon Schemes, XRPC clients and Firehose for now. All models, queries, and procedures are generated automatically. The main focus is on the lexicons of atproto.com and bsky.app, but it doesn't have a vendor lock on it. Feel free to use the code generator for your own lexicon schemes. SDK also provides utilities to work with CID, NSID, AT URI Scheme. DAG-CBOR, CAR files.
 
 ### Requirements
 
 - Python 3.7 or higher.
 - Access to Bsky if you don't have own server.
 
 ### Installing
@@ -178,15 +186,15 @@
 The documentation is live at [atproto.blue](https://atproto.blue/).
 
 ### Getting help
 
 You can get help in several ways:
 - Report bugs, request new features by [creating an issue](https://github.com/MarshalX/atproto/issues/new).
 - Ask questions by [starting a discussion](https://github.com/MarshalX/atproto/discussions/new).
-- Ask questions in [Discord server](https://discord.gg/ZDMSm3UGPN).
+- Ask questions in [Discord server](https://discord.gg/PCyVJXU9jN).
 
 ### Advanced usage
 
 I'll be honest. The high-level Client that was shown in the "Quick Start" section is not a real ATProto API. It's syntax sugar built upon the real XRPC methods! The high-level methods are not cover the full need of developers. To be able to do anything that you want you should know to work with low-level API. Let's dive into it!
 
 The basics:
 - Namespaces – classes that group sub-namespaces and the XRPC queries and procedures. Built upon NSID ATProto semantic.
```

