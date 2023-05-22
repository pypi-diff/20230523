# Comparing `tmp/discord-typings-0.5.1.tar.gz` & `tmp/discord_typings-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-typings-0.5.1.tar", last modified: Mon Jul  4 00:06:08 2022, max compression
+gzip compressed data, was "discord_typings-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `discord-typings-0.5.1.tar` & `discord_typings-0.6.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0      149 2022-05-14 00:30:52.537559 discord-typings-0.5.1/.flake8
--rw-r--r--   0        0        0      486 2022-05-14 00:30:52.547561 discord-typings-0.5.1/.github/workflows/import.yml
--rw-r--r--   0        0        0     1369 2022-05-14 00:30:52.557558 discord-typings-0.5.1/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1077 2021-11-14 21:56:37.058725 discord-typings-0.5.1/.gitignore
--rw-r--r--   0        0        0       33 2022-05-14 00:30:52.564558 discord-typings-0.5.1/.isort.cfg
--rw-r--r--   0        0        0     1095 2021-11-15 18:26:00.285771 discord-typings-0.5.1/LICENSE
--rw-r--r--   0        0        0      998 2022-05-14 00:30:52.573558 discord-typings-0.5.1/README.md
--rw-r--r--   0        0        0      204 2022-07-02 22:36:00.752500 discord-typings-0.5.1/discord_typings/__init__.py
--rw-r--r--   0        0        0    32267 2022-07-03 23:36:01.726746 discord-typings-0.5.1/discord_typings/gateway.py
--rw-r--r--   0        0        0       78 2022-05-14 00:30:52.608559 discord-typings-0.5.1/discord_typings/interactions/__init__.py
--rw-r--r--   0        0        0    13010 2022-07-03 23:27:22.709928 discord-typings-0.5.1/discord_typings/interactions/commands.py
--rw-r--r--   0        0        0     3129 2022-06-19 00:59:52.564536 discord-typings-0.5.1/discord_typings/interactions/components.py
--rw-r--r--   0        0        0     8870 2022-07-03 23:37:09.445763 discord-typings-0.5.1/discord_typings/interactions/receiving.py
--rw-r--r--   0        0        0        0 2022-02-13 18:10:03.803919 discord-typings-0.5.1/discord_typings/py.typed
--rw-r--r--   0        0        0     1084 2022-07-02 22:36:00.794014 discord-typings-0.5.1/discord_typings/reference.py
--rw-r--r--   0        0        0      369 2022-06-19 00:59:52.566520 discord-typings-0.5.1/discord_typings/resources/__init__.py
--rw-r--r--   0        0        0     1463 2022-07-02 22:36:00.795014 discord-typings-0.5.1/discord_typings/resources/application.py
--rw-r--r--   0        0        0     2524 2022-07-03 23:31:02.880876 discord-typings-0.5.1/discord_typings/resources/audit_log.py
--rw-r--r--   0        0        0     4274 2022-07-02 22:36:00.799016 discord-typings-0.5.1/discord_typings/resources/auto_moderation.py
--rw-r--r--   0        0        0    12304 2022-07-02 22:36:00.800015 discord-typings-0.5.1/discord_typings/resources/channel.py
--rw-r--r--   0        0        0      666 2022-07-02 22:36:00.801015 discord-typings-0.5.1/discord_typings/resources/emoji.py
--rw-r--r--   0        0        0     9618 2022-07-03 23:36:55.285031 discord-typings-0.5.1/discord_typings/resources/guild.py
--rw-r--r--   0        0        0     2878 2022-07-02 22:36:00.809529 discord-typings-0.5.1/discord_typings/resources/guild_scheduled_events.py
--rw-r--r--   0        0        0      742 2022-07-02 22:36:00.810529 discord-typings-0.5.1/discord_typings/resources/guild_template.py
--rw-r--r--   0        0        0     1842 2022-06-19 00:59:52.573552 discord-typings-0.5.1/discord_typings/resources/invite.py
--rw-r--r--   0        0        0      739 2022-07-02 22:36:00.818532 discord-typings-0.5.1/discord_typings/resources/stage_instance.py
--rw-r--r--   0        0        0     1752 2022-07-02 22:36:00.820532 discord-typings-0.5.1/discord_typings/resources/sticker.py
--rw-r--r--   0        0        0     1035 2022-07-03 23:36:55.310037 discord-typings-0.5.1/discord_typings/resources/user.py
--rw-r--r--   0        0        0     1026 2022-07-02 22:36:00.821541 discord-typings-0.5.1/discord_typings/resources/voice.py
--rw-r--r--   0        0        0     1039 2022-07-02 22:36:00.822531 discord-typings-0.5.1/discord_typings/resources/webhook.py
--rw-r--r--   0        0        0     1554 2022-07-03 23:47:20.238191 discord-typings-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2216 1970-01-01 00:00:00.000000 discord-typings-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      172 2022-10-01 15:24:22.047549 discord_typings-0.6.0/.flake8
+-rw-r--r--   0        0        0      486 2022-05-14 00:30:52.547561 discord_typings-0.6.0/.github/workflows/import.yml
+-rw-r--r--   0        0        0     1369 2022-05-14 00:30:52.557558 discord_typings-0.6.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1077 2021-11-14 21:56:37.058725 discord_typings-0.6.0/.gitignore
+-rw-r--r--   0        0        0       33 2022-05-14 00:30:52.564558 discord_typings-0.6.0/.isort.cfg
+-rw-r--r--   0        0        0     1102 2023-05-17 22:50:11.811801 discord_typings-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3133 2023-05-17 23:00:22.287803 discord_typings-0.6.0/README.md
+-rw-r--r--   0        0        0      231 2022-10-19 21:35:44.398245 discord_typings-0.6.0/discord_typings/__init__.py
+-rw-r--r--   0        0        0    35503 2023-05-22 22:13:06.874750 discord_typings-0.6.0/discord_typings/_gateway.py
+-rw-r--r--   0        0        0       81 2023-05-22 21:55:37.047417 discord_typings-0.6.0/discord_typings/_interactions/__init__.py
+-rw-r--r--   0        0        0    10843 2023-05-22 21:55:37.048416 discord_typings-0.6.0/discord_typings/_interactions/_commands.py
+-rw-r--r--   0        0        0     4550 2023-05-22 21:55:36.922918 discord_typings-0.6.0/discord_typings/_interactions/_components.py
+-rw-r--r--   0        0        0    10756 2023-02-19 00:15:19.126678 discord_typings-0.6.0/discord_typings/_interactions/_receiving.py
+-rw-r--r--   0        0        0     1629 2023-02-19 00:29:12.714609 discord_typings-0.6.0/discord_typings/_oauth.py
+-rw-r--r--   0        0        0     1553 2023-02-19 00:13:30.874611 discord_typings-0.6.0/discord_typings/_reference.py
+-rw-r--r--   0        0        0      425 2023-02-19 00:13:30.882615 discord_typings-0.6.0/discord_typings/_resources/__init__.py
+-rw-r--r--   0        0        0     1860 2023-02-19 00:13:30.889612 discord_typings-0.6.0/discord_typings/_resources/_application.py
+-rw-r--r--   0        0        0     3153 2022-10-19 21:35:44.539372 discord_typings-0.6.0/discord_typings/_resources/_audit_log.py
+-rw-r--r--   0        0        0     4839 2023-02-19 00:13:30.895610 discord_typings-0.6.0/discord_typings/_resources/_auto_moderation.py
+-rw-r--r--   0        0        0    14619 2023-02-19 00:22:45.099031 discord_typings-0.6.0/discord_typings/_resources/_channel.py
+-rw-r--r--   0        0        0      668 2022-10-19 21:35:44.504372 discord_typings-0.6.0/discord_typings/_resources/_emoji.py
+-rw-r--r--   0        0        0    10226 2023-05-22 22:04:01.037891 discord_typings-0.6.0/discord_typings/_resources/_guild.py
+-rw-r--r--   0        0        0     2942 2022-10-19 21:35:44.489050 discord_typings-0.6.0/discord_typings/_resources/_guild_scheduled_events.py
+-rw-r--r--   0        0        0      745 2022-10-19 21:35:44.479244 discord_typings-0.6.0/discord_typings/_resources/_guild_template.py
+-rw-r--r--   0        0        0     1914 2022-12-16 23:06:33.379359 discord_typings-0.6.0/discord_typings/_resources/_invite.py
+-rw-r--r--   0        0        0     1029 2023-02-19 00:13:30.914610 discord_typings-0.6.0/discord_typings/_resources/_role_connection_metadata.py
+-rw-r--r--   0        0        0      801 2022-10-19 21:35:44.475243 discord_typings-0.6.0/discord_typings/_resources/_stage_instance.py
+-rw-r--r--   0        0        0     1773 2023-02-19 00:13:36.160135 discord_typings-0.6.0/discord_typings/_resources/_sticker.py
+-rw-r--r--   0        0        0     2191 2023-02-19 00:24:02.719369 discord_typings-0.6.0/discord_typings/_resources/_user.py
+-rw-r--r--   0        0        0     1041 2022-10-19 21:35:44.453244 discord_typings-0.6.0/discord_typings/_resources/_voice.py
+-rw-r--r--   0        0        0     1043 2022-10-19 21:35:44.445244 discord_typings-0.6.0/discord_typings/_resources/_webhook.py
+-rw-r--r--   0        0        0        0 2022-02-13 18:10:03.803919 discord_typings-0.6.0/discord_typings/py.typed
+-rw-r--r--   0        0        0     1644 2023-05-22 22:16:20.739368 discord_typings-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4382 1970-01-01 00:00:00.000000 discord_typings-0.6.0/PKG-INFO
```

### Comparing `discord-typings-0.5.1/.github/workflows/lint.yml` & `discord_typings-0.6.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `discord-typings-0.5.1/.gitignore` & `discord_typings-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `discord-typings-0.5.1/LICENSE` & `discord_typings-0.6.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2021 Bluenix
+Copyright (c) 2021 - 2023 Bluenix
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `discord-typings-0.5.1/discord_typings/gateway.py` & `discord_typings-0.6.0/discord_typings/_gateway.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,26 +7,28 @@
 
 from typing_extensions import Literal, NotRequired, TypeAlias, TypedDict, final
 
 if TYPE_CHECKING:
     # Flake8 complains about some of these imports where they are only used
     # inside of strings (not annotations) for the type aliases, so we have to
     # disable the check.
-    from .interactions import (  # noqa: F401
-        ApplicationCommandPermissionsData, InteractionData, Locales
+    from ._interactions import (  # noqa: F401
+        ApplicationCommandPermissionsData, InteractionData
     )
-    from .reference import Snowflake
-    from .resources import (  # noqa: F401
-        ApplicationData, AutoModerationActionData, AutoModerationRuleData,
-        AutoModerationTriggerTypes, CategoryChannelData, EmojiData, GuildData,
-        GuildFeaturesData, GuildMemberData, GuildScheduledEventData,
-        MessageData, NewsChannelData, RoleData, StageInstanceData, StickerData,
-        TextChannelData, ThreadChannelData, ThreadMemberData, ThreadMetadata,
-        UnavailableGuildData, UserData, VoiceChannelData, VoiceStateData,
-        WelcomeScreenData
+    from ._reference import Locales, Snowflake
+    from ._resources import (  # noqa: F401
+        ApplicationData, AuditLogEntryData, AutoModerationActionData,
+        AutoModerationRuleData, AutoModerationTriggerTypes,
+        CategoryChannelData, EmojiData, GuildData, GuildFeaturesData,
+        GuildMemberData, GuildScheduledEventData, IntegrationAccountData,
+        IntegrationApplicationData, IntegrationExpireBehaviors, MessageData,
+        NewsChannelData, RoleData, StageInstanceData, StickerData,
+        TextChannelData, ThreadChannelData, ThreadMemberData,
+        ThreadMetadataData, UnavailableGuildData, UserData, VoiceChannelData,
+        VoiceStateData, WelcomeScreenData
     )
 
 __all__ = (
     'HeartbeatACKEvent', 'IdentifyData', 'IdentifyConnectionProperties', 'IdentifyCommand',
     'ResumeData', 'ResumeCommand', 'HeartbeatCommand', 'RequestGuildMembersData',
     'RequestGuildMembersCommand', 'UpdateVoiceStateData', 'UpdateVoiceStateCommand',
     'PartialActivityData', 'UpdatePresenceData', 'UpdatePresenceCommand', 'HelloData',
@@ -49,30 +51,33 @@
     'GuildRoleCreateData', 'GuildRoleCreateEvent', 'GuildRoleCreateEvent',
     'GuildRoleUpdateData', 'GuildRoleUpdateEvent', 'GuildRoleDeleteData',
     'GuildRoleDeleteEvent', 'GuildScheduledEventCreateData', 'GuildScheduledEventCreateEvent',
     'GuildScheduledEventUpdateData', 'GuildScheduledEventUpdateEvent',
     'GuildScheduledEventDeleteData', 'GuildScheduledEventDeleteEvent',
     'GuildScheduledEventUserAddData', 'GuildScheduledEventUserAddEvent',
     'GuildScheduledEventUserRemoveData', 'GuildScheduledEventUserRemoveEvent',
+    'IntegrationCreateData', 'IntegrationCreateEvent', 'IntegrationUpdateData',
+    'IntegrationUpdateEvent', 'IntegrationDeleteData', 'IntegrationDeleteEvent',
     'InviteCreateData', 'InviteCreateEvent', 'InviteDeleteData', 'InviteDeleteEvent',
     'MessageCreateData', 'MessageCreateEvent', 'MessageUpdateData', 'MessageUpdateEvent',
     'MessageDeleteData', 'MessageDeleteEvent', 'MessageDeleteBulkData',
     'MessageDeleteBulkEvent', 'MessageReactionAddData', 'MessageReactionAddEvent',
     'MessageReactionRemoveData', 'MessageReactionRemoveEvent', 'MessageReactionRemoveAllData',
     'MessageReactionRemoveAllEvent', 'MessageReactionRemoveEmojiData',
     'MessageReactionRemoveEmojiEvent', 'PresenceUpdateData', 'ClientStatusData',
     'ActivityData', 'ActivityTimestampsData', 'ActivityEmojiData', 'ActivityPartyData',
     'ActivityAssetsData', 'ActivitySecretsData', 'ActivityButtonData', 'TypingStartData',
-    'TypingStartEvent', 'VoiceStateUpdateData', 'VoiceStateUpdateEvent',
-    'VoiceServerUpdateData', 'VoiceServerUpdateEvent', 'WebhooksUpdateData',
-    'WebhooksUpdateEvent', 'InteractionCreateData', 'InteractionCreateEvent',
-    'StageInstanceCreateData', 'StageInstanceCreateEvent', 'StageInstanceUpdateData',
-    'StageInstanceUpdateEvent', 'StageInstanceDeleteData', 'StageInstanceDeleteEvent',
-    'GetGatewayData', 'GetGatewayBotData', 'SessionStartLimitData', 'DispatchEvent',
-    'GatewayEvent'
+    'TypingStartEvent', 'UserUpdateData', 'UserUpdateEvent', 'VoiceStateUpdateData',
+    'VoiceStateUpdateEvent', 'VoiceServerUpdateData', 'VoiceServerUpdateEvent',
+    'WebhooksUpdateData', 'WebhooksUpdateEvent', 'InteractionCreateData',
+    'InteractionCreateEvent', 'StageInstanceCreateData', 'StageInstanceCreateEvent',
+    'StageInstanceUpdateData', 'StageInstanceUpdateEvent', 'StageInstanceDeleteData',
+    'StageInstanceDeleteEvent', 'GetGatewayData', 'GetGatewayBotData',
+    'SessionStartLimitData', 'DispatchEvent', 'GatewayEvent',
+    'GuildAuditLogEntryCreateData', 'GuildAuditLogEntryCreateEvent'
 )
 
 
 _D = TypeVar('_D', bound='Mapping[str, Any]')
 _T = TypeVar('_T', bound='str')  # Literal
 
 
@@ -90,23 +95,23 @@
     """
     op: Literal[0]
     d: _D
     s: int
     t: _T
 
 
-# https://discord.com/developers/docs/topics/gateway#heartbeating-example-gateway-heartbeat-ack
+# https://discord.com/developers/docs/topics/gateway#heartbeat-interval
 
 
 @final
 class HeartbeatACKEvent(TypedDict):
     op: Literal[11]
 
 
-# https://discord.com/developers/docs/topics/gateway#identify
+# https://discord.com/developers/docs/topics/gateway-events#identify
 
 
 @final
 class IdentifyData(TypedDict):
     token: str
     properties: IdentifyConnectionProperties
     compress: NotRequired[bool]
@@ -124,16 +129,15 @@
 
 
 @final
 class IdentifyCommand(TypedDict):
     op: Literal[2]
     d: IdentifyData
 
-
-# https://discord.com/developers/docs/topics/gateway#resume
+# https://discord.com/developers/docs/topics/gateway-events#resume
 
 
 @final
 class ResumeData(TypedDict):
     token: str
     session_id: str
     seq: int
@@ -141,24 +145,24 @@
 
 @final
 class ResumeCommand(TypedDict):
     op: Literal[6]
     d: ResumeData
 
 
-# https://discord.com/developers/docs/topics/gateway#heartbeat
+# https://discord.com/developers/docs/topics/gateway-events#heartbeat
 
 
 @final
 class HeartbeatCommand(TypedDict):
     op: Literal[1]
     d: Optional[int]
 
 
-# https://discord.com/developers/docs/topics/gateway#request-guild-members
+# https://discord.com/developers/docs/topics/gateway-events#request-guild-members
 
 
 @final
 class _QueryRequestMembersCommand(TypedDict):
     guild_id: Snowflake
     query: str
     limit: int
@@ -181,15 +185,15 @@
 
 @final
 class RequestGuildMembersCommand(TypedDict):
     op: Literal[8]
     d: RequestGuildMembersData
 
 
-# https://discord.com/developers/docs/topics/gateway#update-voice-state
+# https://discord.com/developers/docs/topics/gateway-events#update-voice-state
 
 
 @final
 class UpdateVoiceStateData(TypedDict):
     guild_id: Snowflake
     channel_id: Optional[Snowflake]
     self_mute: bool
@@ -198,15 +202,15 @@
 
 @final
 class UpdateVoiceStateCommand(TypedDict):
     op: Literal[4]
     d: UpdateVoiceStateData
 
 
-# https://discord.com/developers/docs/topics/gateway#update-presence
+# https://discord.com/developers/docs/topics/gateway-events#update-presence
 
 
 @final
 class PartialActivityData(TypedDict):
     name: str
     type: Literal[0, 1, 2, 3, 4, 5]
     url: NotRequired[str]
@@ -222,15 +226,15 @@
 
 @final
 class UpdatePresenceCommand(TypedDict):
     op: Literal[3]
     d: UpdatePresenceData
 
 
-# https://discord.com/developers/docs/topics/gateway#hello
+# https://discord.com/developers/docs/topics/gateway-events#hello
 
 
 @final
 class HelloData(TypedDict):
     heartbeat_interval: int
 
 
@@ -238,178 +242,179 @@
 class HelloEvent(TypedDict):
     op: Literal[10]
     d: HelloData
     s: None
     t: None
 
 
-# https://discord.com/developers/docs/topics/gateway#ready
+# https://discord.com/developers/docs/topics/gateway-events#ready
 
 
 @final
 class PartialApplicationData(TypedDict):
     id: Snowflake
     flags: int
 
 
 @final
 class ReadyData(TypedDict):
     v: int
     user: UserData
     guilds: List[UnavailableGuildData]
     session_id: str
+    resume_gateway_url: str
     shard: NotRequired[Union[Tuple[int, int], List[int]]]
     application: PartialApplicationData
 
 
 ReadyEvent = GenericDispatchEvent[Literal['READY'], ReadyData]
 
 
-# https://discord.com/developers/docs/topics/gateway#resumed
+# https://discord.com/developers/docs/topics/gateway-events#resumed
 
 
 @final
 class ResumedData(TypedDict):
     ...  # It only has an undocumented _trace field
 
 
 ResumedEvent = GenericDispatchEvent[Literal['RESUMED'], ResumedData]
 
 
-# https://discord.com/developers/docs/topics/gateway#reconnect
+# https://discord.com/developers/docs/topics/gateway-events#reconnect
 
 
 @final
 class ReconnectEvent(TypedDict):
     op: Literal[7]
     d: None
     s: None
     t: None
 
 
-# https://discord.com/developers/docs/topics/gateway#invalid-session
+# https://discord.com/developers/docs/topics/gateway-events#invalid-session
 
 
 @final
 class InvalidSessionEvent(TypedDict):
     op: Literal[9]
     d: bool
     s: None
     t: None
 
-# https://discord.com/developers/docs/topics/gateway#get-gateway-example-response
+# https://discord.com/developers/docs/topics/gateway-events#get-gateway-example-response
 
 
 @final
 class GetGatewayData(TypedDict):
     url: str
 
-# https://discord.com/developers/docs/topics/gateway#application-command-permissions-update
+# https://discord.com/developers/docs/topics/gateway-events#application-command-permissions-update
 
 
 ApplicationCommandPermissionsUpdateData: TypeAlias = 'ApplicationCommandPermissionsData'
 
 
 ApplicationCommandPermissionsUpdateEvent = GenericDispatchEvent[
     Literal['APPLICATION_COMMAND_PERMISSIONS_UPDATE'],
     ApplicationCommandPermissionsUpdateData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#auto-moderation-rule-create
+# https://discord.com/developers/docs/topics/gateway-events#auto-moderation-rule-create
 
 
 AutoModerationRuleCreateData: TypeAlias = 'AutoModerationRuleData'
 
 
 AutoModerationRuleCreateEvent = GenericDispatchEvent[
     Literal['AUTO_MODERATION_RULE_CREATE'],
     AutoModerationRuleCreateData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#auto-moderation-rule-update
+# https://discord.com/developers/docs/topics/gateway-events#auto-moderation-rule-update
 
 
 AutoModerationRuleUpdateData: TypeAlias = 'AutoModerationRuleData'
 
 
 AutoModerationRuleUpdateEvent = GenericDispatchEvent[
     Literal['AUTO_MODERATION_RULE_UPDATE'],
     AutoModerationRuleUpdateData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#auto-moderation-rule-delete
+# https://discord.com/developers/docs/topics/gateway-events#auto-moderation-rule-delete
 
 
 AutoModerationRuleDeleteData: TypeAlias = 'AutoModerationRuleData'
 
 
 AutoModerationRuleDeleteEvent = GenericDispatchEvent[
     Literal['AUTO_MODERATION_RULE_DELETE'],
     AutoModerationRuleDeleteData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#auto-moderation-action-execution
+# https://discord.com/developers/docs/topics/gateway-events#auto-moderation-action-execution
 
 
 @final
 class AutoModerationActionExecutionData(TypedDict):
     guild_id: Snowflake
     action: AutoModerationActionData
     rule_id: Snowflake
     rule_trigger_type: AutoModerationTriggerTypes
     user_id: Snowflake
     channel_id: NotRequired[Snowflake]
     message_id: NotRequired[Snowflake]
     alert_system_message_id: NotRequired[Snowflake]
-    content: str
+    content: NotRequired[str]
     matched_keyword: Optional[str]
-    matched_content: Optional[str]
+    matched_content: NotRequired[Optional[str]]
 
 
 AutoModerationActionExecutionEvent = GenericDispatchEvent[
     Literal['AUTO_MODERATION_ACTION_EXECUTION'],
     AutoModerationActionExecutionData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#channels
+# https://discord.com/developers/docs/topics/gateway-events#channels
 
 
 # Utility for the events below
 _GuildChannelData = Union[
     'TextChannelData', 'NewsChannelData', 'VoiceChannelData', 'CategoryChannelData'
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#channel-create
+# https://discord.com/developers/docs/topics/gateway-events#channel-create
 
 
 ChannelCreateData = _GuildChannelData
 ChannelCreateEvent = GenericDispatchEvent[Literal['CHANNEL_CREATE'], ChannelCreateData]
 
 
-# https://discord.com/developers/docs/topics/gateway#channel-update
+# https://discord.com/developers/docs/topics/gateway-events#channel-update
 
 
 ChannelUpdateData = _GuildChannelData
 ChannelUpdateEvent = GenericDispatchEvent[Literal['CHANNEL_UPDATE'], ChannelUpdateData]
 
 
-# https://discord.com/developers/docs/topics/gateway#channel-delete
+# https://discord.com/developers/docs/topics/gateway-events#channel-delete
 
 
 ChannelDeleteData = _GuildChannelData
 ChannelDeleteEvent = GenericDispatchEvent[Literal['CHANNEl_DELETE'], ChannelDeleteData]
 
 
-# https://discord.com/developers/docs/topics/gateway#thread-create
+# https://discord.com/developers/docs/topics/gateway-events#thread-create
 
 
 @final
 class ThreadCreateData(TypedDict):
     id: Snowflake
     type: Literal[10, 11, 12]
     guild_id: NotRequired[Snowflake]
@@ -417,59 +422,59 @@
     last_message_id: Optional[Snowflake]
     rate_limit_per_user: int
     owner_id: Snowflake
     parent_id: Optional[Snowflake]
     last_pin_timestamp: NotRequired[Optional[str]]
     message_count: int
     member_count: int
-    thread_metadata: ThreadMetadata
+    thread_metadata: ThreadMetadataData
     member: NotRequired[ThreadMemberData]
 
     newly_created: bool  # Extra THREAD_CREATE field
 
 
 ThreadCreateEvent = GenericDispatchEvent[Literal['THREAD_CREATE'], ThreadCreateData]
 
 
-# https://discord.com/developers/docs/topics/gateway#thread-update
+# https://discord.com/developers/docs/topics/gateway-events#thread-update
 
 
 ThreadUpdateData: TypeAlias = 'ThreadChannelData'
 ThreadUpdateEvent = GenericDispatchEvent[Literal['THREAD_UPDATE'], ThreadUpdateData]
 
 
-# https://discord.com/developers/docs/topics/gateway#thread-delete
+# https://discord.com/developers/docs/topics/gateway-events#thread-delete
 
 
 @final
 class ThreadDeleteData(TypedDict):
     id: Snowflake
     guild_id: Snowflake
     parent_id: Snowflake
     type: Literal[10, 11, 12]
 
 
 ThreadDeleteEvent = GenericDispatchEvent[Literal['THREAD_DELETE'], ThreadDeleteData]
 
 
-# https://discord.com/developers/docs/topics/gateway#thread-list-sync
+# https://discord.com/developers/docs/topics/gateway-events#thread-list-sync
 
 
 @final
 class ThreadListSyncData(TypedDict):
     guild_id: Snowflake
     channel_ids: NotRequired[List[Snowflake]]
     threads: List[ThreadChannelData]
     members: List[ThreadMemberData]
 
 
 ThreadListSyncEvent = GenericDispatchEvent[Literal['THREAD_LIST_SYNC'], ThreadListSyncData]
 
 
-# https://discord.com/developers/docs/topics/gateway#thread-member-update
+# https://discord.com/developers/docs/topics/gateway-events#thread-member-update
 
 
 @final
 class ThreadMemberUpdateData(TypedDict):
     # 'id' and 'user_id' is only missing in the GUILD_CREATE event, so we know
     # that they are present in this event (hence the missing NotRequired
     # compared to ThreadMemberData).
@@ -481,15 +486,15 @@
 
 
 ThreadMemberUpdateEvent = GenericDispatchEvent[
     Literal['THREAD_MEMBER_UPDATE'], ThreadMemberUpdateData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#thread-members-update
+# https://discord.com/developers/docs/topics/gateway-events#thread-members-update
 
 
 @final
 class ThreadMembersUpdateData(TypedDict):
     id: Snowflake
     guild_id: Snowflake
     member_count: int
@@ -498,30 +503,30 @@
 
 
 ThreadMembersUpdateEvent = GenericDispatchEvent[
     Literal['THREAD_MEMBERS_UPDATE'], ThreadMembersUpdateData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#channel-pins-update
+# https://discord.com/developers/docs/topics/gateway-events#channel-pins-update
 
 
 @final
 class ChannelPinsUpdateData(TypedDict):
     guild_id: NotRequired[Snowflake]
     channel_id: Snowflake
     last_pin_timestamp: NotRequired[Optional[str]]
 
 
 ChannelPinsUpdateEvent = GenericDispatchEvent[
     Literal['CHANNEL_PINS_UPDATE'], ChannelPinsUpdateData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#guild-create
+# https://discord.com/developers/docs/topics/gateway-events#guild-create
 
 
 @final
 class GuildCreateData(TypedDict):
     id: str
     name: str
     icon: Optional[str]
@@ -576,94 +581,104 @@
     stage_instances: List[StageInstanceData]
     guild_scheduled_events: List[GuildScheduledEventData]
 
 
 GuildCreateEvent = GenericDispatchEvent[Literal['GUILD_CREATE'], GuildCreateData]
 
 
-# https://discord.com/developers/docs/topics/gateway#guild-update
+# https://discord.com/developers/docs/topics/gateway-events#guild-update
 
 
 GuildUpdateData: TypeAlias = 'GuildData'
 GuildUpdateEvent = GenericDispatchEvent[Literal['GUILD_UPDATE'], GuildUpdateData]
 
 
-# https://discord.com/developers/docs/topics/gateway#guild-delete
+# https://discord.com/developers/docs/topics/gateway-events#guild-delete
 
 
 GuildDeleteData: TypeAlias = 'UnavailableGuildData'
 GuildDeleteEvent = GenericDispatchEvent[Literal['GUILD_DELETE'], 'GuildDeleteData']
 
 
-# https://discord.com/developers/docs/topics/gateway#guild-ban-add
+# https://discord.com/developers/docs/topics/gateway-events#guild-audit-log-entry-create
+
+
+GuildAuditLogEntryCreateData: TypeAlias = 'AuditLogEntryData'
+GuildAuditLogEntryCreateEvent = GenericDispatchEvent[
+    Literal['GUILD_AUDIT_LOG_ENTRY_CREATE'],
+    'AuditLogEntryData'
+]
+
+
+# https://discord.com/developers/docs/topics/gateway-events#guild-ban-add
 
 
 @final
 class GuildBanAddData(TypedDict):
     guild_id: Snowflake
     user: UserData
 
 
 GuildBanAddEvent = GenericDispatchEvent[Literal['GUILD_BAN_ADD'], GuildBanAddData]
 
 
-# https://discord.com/developers/docs/topics/gateway#guild-ban-remove
+# https://discord.com/developers/docs/topics/gateway-events#guild-ban-remove
 
 
 @final
 class GuildBanRemoveData(TypedDict):
     guild_id: Snowflake
     user: UserData
 
 
 GuildBanRemoveEvent = GenericDispatchEvent[Literal['GUILD_BAN_REMOVE'], GuildBanRemoveData]
 
 
-# https://discord.com/developers/docs/topics/gateway#guild-emojis-update
+# https://discord.com/developers/docs/topics/gateway-events#guild-emojis-update
 
 
 @final
 class GuildEmojisUpdateData(TypedDict):
     guild_id: Snowflake
     emojis: List[EmojiData]
 
 
 GuildEmojisUpdateEvent = GenericDispatchEvent[
     Literal['GUILD_EMOJIS_UPDATE'], GuildEmojisUpdateData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#guild-stickers-update
+# https://discord.com/developers/docs/topics/gateway-events#guild-stickers-update
 
 
 @final
 class GuildStickersUpdateData(TypedDict):
     guild_id: Snowflake
     stickers: List[StickerData]
 
 
 GuildStickersUpdateEvent = GenericDispatchEvent[
     Literal['GUILD_STICKERS_UPDATE'], GuildStickersUpdateData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#guild-integrations-update
+# https://discord.com/developers/docs/topics/gateway-events#guild-integrations-update
 
 
 @final
 class GuildIntergrationsUpdateData(TypedDict):
     guild_id: Snowflake
 
 
 GuildIntergrationsUpdateEvent = GenericDispatchEvent[
     Literal['GUILD_INTEGRATIONS_UPDATE'], GuildIntergrationsUpdateData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#guild-member-add
+# https://discord.com/developers/docs/topics/gateway-events#guild-member-add
 
 
 @final
 class GuildMemberAddData(TypedDict):
     user: UserData  # Always present in GUILD_MEMBER_ADD events
     nick: NotRequired[Optional[str]]
     avatar: NotRequired[Optional[str]]
@@ -677,36 +692,36 @@
 
     guild_id: Snowflake  # Extra field
 
 
 GuildMemberAddEvent = GenericDispatchEvent[Literal['GUILD_MEMBER_ADD'], GuildMemberAddData]
 
 
-# https://discord.com/developers/docs/topics/gateway#guild-member-remove
+# https://discord.com/developers/docs/topics/gateway-events#guild-member-remove
 
 
 @final
 class GuildMemberRemoveData(TypedDict):
     user: UserData
     guild_id: Snowflake
 
 
 GuildMemberRemoveEvent = GenericDispatchEvent[
     Literal['GUILD_MEMBER_REMOVE'], GuildMemberRemoveData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#guild-member-update
+# https://discord.com/developers/docs/topics/gateway-events#guild-member-update
 
 
 @final
 class GuildMemberUpdateData(TypedDict):
     guild_id: Snowflake
     roles: List[Snowflake]
-    user: List[UserData]
+    user: UserData
     nick: NotRequired[Optional[str]]
     avatar: Optional[str]
     joined_at: Optional[str]
     premium_since: NotRequired[Optional[str]]
     deaf: NotRequired[bool]
     mute: NotRequired[bool]
     pending: NotRequired[bool]
@@ -714,15 +729,15 @@
 
 
 GuildMemberUpdateEvent = GenericDispatchEvent[
     Literal['GUILD_MEMBER_UPDATE'], GuildMemberUpdateData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#guild-members-chunk
+# https://discord.com/developers/docs/topics/gateway-events#guild-members-chunk
 
 
 @final
 class GuildMembersChunkData(TypedDict):
     guild_id: Snowflake
     members: List[GuildMemberData]
     chunk_index: int
@@ -733,108 +748,180 @@
 
 
 GuildMembersChunkEvent = GenericDispatchEvent[
     Literal['GUILD_MEMBERS_CHUNK'], GuildMembersChunkData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#guild-role-create
+# https://discord.com/developers/docs/topics/gateway-events#guild-role-create
 
 
 @final
 class GuildRoleCreateData(TypedDict):
     guild_id: Snowflake
     role: RoleData
 
 
 GuildRoleCreateEvent = GenericDispatchEvent[Literal['GUILD_ROLE_CREATE'], GuildRoleCreateData]
 
 
-# https://discord.com/developers/docs/topics/gateway#guild-role-update
+# https://discord.com/developers/docs/topics/gateway-events#guild-role-update
 
 
 @final
 class GuildRoleUpdateData(TypedDict):
     guild_id: Snowflake
     role: RoleData
 
 
 GuildRoleUpdateEvent = GenericDispatchEvent[Literal['GUILD_ROLE_UPDATE'], GuildRoleUpdateData]
 
 
-# https://discord.com/developers/docs/topics/gateway#guild-role-delete
+# https://discord.com/developers/docs/topics/gateway-events#guild-role-delete
 
 
 @final
 class GuildRoleDeleteData(TypedDict):
     guild_id: Snowflake
     role_id: Snowflake
 
 
 GuildRoleDeleteEvent = GenericDispatchEvent[Literal['GUILD_ROLE_DELETE'], GuildRoleDeleteData]
 
 
-# https://discord.com/developers/docs/topics/gateway#guild-scheduled-event-create
+# https://discord.com/developers/docs/topics/gateway-events#guild-scheduled-event-create
 
 
 GuildScheduledEventCreateData: TypeAlias = 'GuildScheduledEventData'
 GuildScheduledEventCreateEvent = GenericDispatchEvent[
     Literal['GUILD_SCHEDULED_EVENT_CREATE'], GuildScheduledEventCreateData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#guild-scheduled-event-update
+# https://discord.com/developers/docs/topics/gateway-events#guild-scheduled-event-update
 
 
 GuildScheduledEventUpdateData: TypeAlias = 'GuildScheduledEventData'
 GuildScheduledEventUpdateEvent = GenericDispatchEvent[
     Literal['GUILD_SCHEDULED_EVENT_UPDATE'], GuildScheduledEventUpdateData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#guild-scheduled-event-delete
+# https://discord.com/developers/docs/topics/gateway-events#guild-scheduled-event-delete
 
 
 GuildScheduledEventDeleteData: TypeAlias = 'GuildScheduledEventData'
 GuildScheduledEventDeleteEvent = GenericDispatchEvent[
     Literal['GUILD_SCHEDULED_EVENT_DELETE'], GuildScheduledEventDeleteData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#guild-scheduled-event-user-add
+# https://discord.com/developers/docs/topics/gateway-events#guild-scheduled-event-user-add
 
 
 @final
 class GuildScheduledEventUserAddData(TypedDict):
     guild_scheduled_event_id: Snowflake
     user_id: Snowflake
     guild_id: Snowflake
 
 
 GuildScheduledEventUserAddEvent = GenericDispatchEvent[
     Literal['GUILD_SCHEDULED_EVENT_USER_ADD'], GuildScheduledEventUserAddData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#guild-scheduled-event-user-remove
+# https://discord.com/developers/docs/topics/gateway-events#guild-scheduled-event-user-remove
 
 
 @final
 class GuildScheduledEventUserRemoveData(TypedDict):
     guild_scheduled_event_id: Snowflake
     user_id: Snowflake
     guild_id: Snowflake
 
 
 GuildScheduledEventUserRemoveEvent = GenericDispatchEvent[
     Literal['GUILD_SCHEDULED_EVENT_USER_REMOVE'], GuildScheduledEventUserRemoveData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#invite-create
+# https://discord.com/developers/docs/topics/gateway-events#integrations
+
+
+@final
+class _StreamingIntegrationGuildData(TypedDict):
+    id: Snowflake
+    name: str
+    type: Literal['twitch', 'youtube', 'discord']
+    enabled: bool
+    syncing: bool
+    role_id: NotRequired[Snowflake]
+    enable_emoticons: bool
+    expire_behavior: IntegrationExpireBehaviors
+    expire_grace_period: int
+    user: UserData
+    account: IntegrationAccountData
+    synced_at: str
+    subscriber_count: int
+    revoked: bool
+    application: IntegrationApplicationData
+
+    guild_id: Snowflake
+
+
+@final
+class _DiscordIntegrationGuildData(TypedDict):
+    id: Snowflake
+    name: str
+    type: Literal['discord']
+    enabled: bool
+    account: IntegrationAccountData
+    application: NotRequired[IntegrationApplicationData]
+
+    guild_id: Snowflake
+
+
+# Integration object, with an additional guild_id field
+_IntegrationGuildData = Union[_StreamingIntegrationGuildData, _DiscordIntegrationGuildData]
+
+# https://discord.com/developers/docs/topics/gateway-events#integration-create
+
+
+IntegrationCreateData: TypeAlias = '_IntegrationGuildData'
+IntegrationCreateEvent = GenericDispatchEvent[
+    Literal['INTEGRATION_CREATE'], IntegrationCreateData
+]
+
+
+# https://discord.com/developers/docs/topics/gateway-events#integration-update
+
+
+IntegrationUpdateData: TypeAlias = '_IntegrationGuildData'
+IntegrationUpdateEvent = GenericDispatchEvent[
+    Literal['INTEGRATION_UPDATE'], IntegrationUpdateData
+]
+
+
+# https://discord.com/developers/docs/topics/gateway-events#integration-delete
+
+
+@final
+class IntegrationDeleteData(TypedDict):
+    id: Snowflake
+    guild_id: Snowflake
+    application_id: NotRequired[Snowflake]
+
+
+IntegrationDeleteEvent = GenericDispatchEvent[
+    Literal['INTEGRATION_DELETE'], IntegrationDeleteData
+]
+
+
+# https://discord.com/developers/docs/topics/gateway-events#invite-create
 
 
 @final
 class InviteCreateData(TypedDict):
     channel_id: Snowflake
     code: str
     created_at: str
@@ -848,70 +935,70 @@
     temporary: bool
     uses: int
 
 
 InviteCreateEvent = GenericDispatchEvent[Literal['INVITE_CREATE'], InviteCreateData]
 
 
-# https://discord.com/developers/docs/topics/gateway#invite-delete
+# https://discord.com/developers/docs/topics/gateway-events#invite-delete
 
 
 @final
 class InviteDeleteData(TypedDict):
     channel_id: Snowflake
     guild_id: NotRequired[Snowflake]
     code: str
 
 
 InviteDeleteEvent = GenericDispatchEvent[Literal['INVITE_DELETE'], InviteDeleteData]
 
 
-# https://discord.com/developers/docs/topics/gateway#message-create
+# https://discord.com/developers/docs/topics/gateway-events#message-create
 
 
 MessageCreateData: TypeAlias = 'MessageData'
 MessageCreateEvent = GenericDispatchEvent[Literal['MESSAGE_CREATE'], MessageCreateData]
 
 
-# https://discord.com/developers/docs/topics/gateway#message-update
+# https://discord.com/developers/docs/topics/gateway-events#message-update
 
 
 MessageUpdateData: TypeAlias = 'MessageData'
 MessageUpdateEvent = GenericDispatchEvent[Literal['MESSAGE_UPDATE'], MessageUpdateData]
 
 
-# https://discord.com/developers/docs/topics/gateway#message-delete
+# https://discord.com/developers/docs/topics/gateway-events#message-delete
 
 
 @final
 class MessageDeleteData(TypedDict):
     id: Snowflake
     channel_id: Snowflake
     guild_id: NotRequired[Snowflake]
 
 
 MessageDeleteEvent = GenericDispatchEvent[Literal['MESSAGE_DELETE'], MessageDeleteData]
 
 
-# https://discord.com/developers/docs/topics/gateway#message-delete-bulk
+# https://discord.com/developers/docs/topics/gateway-events#message-delete-bulk
 
 
 @final
 class MessageDeleteBulkData(TypedDict):
     ids: List[Snowflake]
     channel_id: Snowflake
     guild_id: NotRequired[Snowflake]
 
 
 MessageDeleteBulkEvent = GenericDispatchEvent[
     Literal['MESSAGE_DELETE_BULK'], MessageDeleteBulkData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#message-reaction-add
+# https://discord.com/developers/docs/topics/gateway-events#message-reaction-add
 
 
 @final
 class MessageReactionAddData(TypedDict):
     user_id: Snowflake
     channel_id: Snowflake
     message_id: Snowflake
@@ -921,15 +1008,15 @@
 
 
 MessageReactionAddEvent = GenericDispatchEvent[
     Literal['MESSAGE_REACTION_ADD'], MessageReactionAddData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#message-reaction-remove
+# https://discord.com/developers/docs/topics/gateway-events#message-reaction-remove
 
 
 @final
 class MessageReactionRemoveData(TypedDict):
     user_id: Snowflake
     channel_id: Snowflake
     message_id: Snowflake
@@ -938,30 +1025,30 @@
 
 
 MessageReactionRemoveEvent = GenericDispatchEvent[
     Literal['MESSAGE_REACTION_REMOVE'], MessageReactionRemoveData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#message-reaction-remove-all
+# https://discord.com/developers/docs/topics/gateway-events#message-reaction-remove-all
 
 
 @final
 class MessageReactionRemoveAllData(TypedDict):
     channel_id: Snowflake
     message_id: Snowflake
     guild_id: NotRequired[Snowflake]
 
 
 MessageReactionRemoveAllEvent = GenericDispatchEvent[
     Literal['MESSAGE_REACTION_REMOVE_ALL'], MessageReactionRemoveAllData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#message-reaction-remove-emoji
+# https://discord.com/developers/docs/topics/gateway-events#message-reaction-remove-emoji
 
 
 @final
 class MessageReactionRemoveEmojiData(TypedDict):
     channel_id: Snowflake
     guild_id: NotRequired[Snowflake]
     message_id: Snowflake
@@ -969,15 +1056,15 @@
 
 
 MessageReactionRemoveEmojiEvent = GenericDispatchEvent[
     Literal['MESSAGE_REACTION_REMOVE_EMOJI'], MessageReactionRemoveEmojiData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#presence-update
+# https://discord.com/developers/docs/topics/gateway-events#presence-update
 
 
 @final
 class PresenceUpdateData(TypedDict):
     user: UserData
     guild_id: Snowflake
     status: Literal['idle', 'dnd', 'online', 'offline']
@@ -988,15 +1075,15 @@
 @final
 class ClientStatusData(TypedDict):
     desktop: NotRequired[str]
     mobile: NotRequired[str]
     web: NotRequired[str]
 
 
-# https://discord.com/developers/docs/topics/gateway#activity-object-activity-structure
+# https://discord.com/developers/docs/topics/gateway-events#activity-object-activity-structure
 
 
 @final
 class ActivityData(TypedDict):
     name: str
     type: Literal[0, 1, 2, 3, 4, 5]
     url: NotRequired[Optional[str]]
@@ -1050,112 +1137,119 @@
 
 @final
 class ActivityButtonData(TypedDict):
     label: str
     url: str
 
 
-# https://discord.com/developers/docs/topics/gateway#typing-start
+# https://discord.com/developers/docs/topics/gateway-events#typing-start
 
 
 @final
 class TypingStartData(TypedDict):
     channel_id: Snowflake
     guild_id: NotRequired[Snowflake]
     user_id: Snowflake
     timestamp: int
     member: NotRequired[GuildMemberData]
 
 
 TypingStartEvent = GenericDispatchEvent[Literal['TYPING_START'], TypingStartData]
 
 
-# https://discord.com/developers/docs/topics/gateway#voice-state-update
+# https://discord.com/developers/docs/topics/gateway-events#user-update
+
+
+UserUpdateData: TypeAlias = 'UserData'
+UserUpdateEvent = GenericDispatchEvent[Literal['USER_UPDATE'], UserUpdateData]
+
+
+# https://discord.com/developers/docs/topics/gateway-events#voice-state-update
 
 
 VoiceStateUpdateData: TypeAlias = 'VoiceStateData'
 VoiceStateUpdateEvent = GenericDispatchEvent[
     Literal['VOICE_STATUS_UPDATE'], VoiceStateUpdateData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#voice-server-update
+# https://discord.com/developers/docs/topics/gateway-events#voice-server-update
 
 
 @final
 class VoiceServerUpdateData(TypedDict):
     token: str
     guild_id: Snowflake
     endpoint: Optional[str]
 
 
 VoiceServerUpdateEvent = GenericDispatchEvent[
     Literal['VOICE_SERVER_UPDATE'], VoiceServerUpdateData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#webhooks-update
+# https://discord.com/developers/docs/topics/gateway-events#webhooks-update
 
 
 @final
 class WebhooksUpdateData(TypedDict):
     guild_id: Snowflake
     channel_id: Snowflake
 
 
 WebhooksUpdateEvent = GenericDispatchEvent[Literal['WEBHOOKS_UPDATE'], WebhooksUpdateData]
 
 
-# https://discord.com/developers/docs/topics/gateway#interaction-create
+# https://discord.com/developers/docs/topics/gateway-events#interaction-create
 
 
 InteractionCreateData: TypeAlias = 'InteractionData'
 InteractionCreateEvent = GenericDispatchEvent[
     Literal['INTERACTION_CREATE'], InteractionCreateData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#stage-instance-create
+# https://discord.com/developers/docs/topics/gateway-events#stage-instance-create
 
 
 StageInstanceCreateData: TypeAlias = 'StageInstanceData'
 StageInstanceCreateEvent = GenericDispatchEvent[
     Literal['STAGE_INSTANCE_CREATE'], StageInstanceCreateData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#stage-instance-update
+# https://discord.com/developers/docs/topics/gateway-events#stage-instance-update
 
 
 StageInstanceUpdateData: TypeAlias = 'StageInstanceData'
 StageInstanceUpdateEvent = GenericDispatchEvent[
     Literal['STAGE_INSTANCE_UPDATE'], StageInstanceUpdateData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#stage-instance-delete
+# https://discord.com/developers/docs/topics/gateway-events#stage-instance-delete
 
 
 StageInstanceDeleteData: TypeAlias = 'StageInstanceData'
 StageInstanceDeleteEvent = GenericDispatchEvent[
     Literal['STAGE_INSTANCE_DELETE'], StageInstanceDeleteData
 ]
 
 
-# https://discord.com/developers/docs/topics/gateway#get-gateway-bot-json-response
+# https://discord.com/developers/docs/topics/gateway-events#get-gateway-bot-json-response
 
 
 @final
 class GetGatewayBotData(TypedDict):
     url: str
     shards: int
     session_start_limit: SessionStartLimitData
 
 
-# https://discord.com/developers/docs/topics/gateway#session-start-limit-object-session-start-limit-structure
+# https://discord.com/developers/docs/topics/gateway#session-start-limit-object
 
 
 @final
 class SessionStartLimitData(TypedDict):
     total: int
     remaining: int
     reset_after: int
```

### Comparing `discord-typings-0.5.1/discord_typings/interactions/commands.py` & `discord_typings-0.6.0/discord_typings/_interactions/_commands.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,64 +1,56 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
 from typing_extensions import Literal, NotRequired, TypedDict, final
 
 if TYPE_CHECKING:
-    from ..reference import Snowflake
+    from .._reference import Locales, Snowflake
+    from .._resources import ChannelTypes
 
 __all__ = (
     'ApplicationCommandData', 'ApplicationCommandTypes', 'SubcommandOptionData',
     'SubcommandGroupOptionData', 'AutocompleteOptionData', 'ApplicationCommandOptionData',
-    'ApplicationCommandOptionInteractionData', 'GuildApplicationCommandPermissionData',
-    'ApplicationCommandPermissionsData', 'ApplicationCommandPayload',
-    'BatchEditApplicationCommandPermissionsData', 'Locales'
+    'GuildApplicationCommandPermissionData', 'ApplicationCommandPermissionsData',
+    'ApplicationCommandPayload', 'EditApplicationCommandPermissionsData'
 )
 
 
-# https://discord.com/developers/docs/reference#locales
-
-
-Locales = Literal[
-    'da', 'de', 'en-GB', 'en-US', 'en-ES', 'fr', 'hr', 'it', 'lt', 'hu', 'nl',
-    'no', 'pl', 'pt-BR', 'ro', 'fi', 'sv-SE', 'vi', 'tr', 'cs', 'el', 'bg',
-    'ru', 'uk', 'hi', 'th', 'zh-CN', 'ja', 'zh-TW', 'ko'
-]
-
-
 # https://discord.com/developers/docs/interactions/application-commands#application-command-object-application-command-structure
 
 
 @final
 class ChatInputCommandData(TypedDict):
     id: Snowflake
     type: NotRequired[Literal[1]]
     application_id: Snowflake
     guild_id: NotRequired[Snowflake]
     name: str
     name_localizations: NotRequired[Optional[Dict[Locales, str]]]
     description: str
     description_localizations: NotRequired[Optional[Dict[Locales, str]]]
     options: List[ApplicationCommandOptionData]
-    default_permission: NotRequired[bool]
+    default_member_permissions: NotRequired[Optional[str]]
+    dm_permission: NotRequired[bool]
+    nsfw: NotRequired[bool]
     version: Snowflake
 
 
 @final
 class ContextMenuCommandData(TypedDict):
     id: Snowflake
     type: NotRequired[Literal[2, 3]]
     application_id: Snowflake
     guild_id: NotRequired[Snowflake]
     name: str
     name_localizations: NotRequired[Optional[Dict[Locales, str]]]
-    description: str
-    description_localizations: NotRequired[Optional[Dict[Locales, str]]]
-    default_permission: NotRequired[bool]
+    default_member_permissions: NotRequired[Optional[str]]
+    dm_permission: NotRequired[bool]
+    nsfw: NotRequired[bool]
     version: Snowflake
 
 
 ApplicationCommandData = Union[ChatInputCommandData, ContextMenuCommandData]
 
 
 # https://discord.com/developers/docs/interactions/application-commands#application-command-object-application-command-types
@@ -185,15 +177,15 @@
 class ChannelOptionData(TypedDict):
     type: Literal[7]
     name: str
     name_localizations: NotRequired[Optional[Dict[Locales, str]]]
     description: str
     description_localizations: NotRequired[Optional[Dict[Locales, str]]]
     required: NotRequired[bool]
-    channel_types: NotRequired[List[Literal[0, 2, 4, 5, 6, 13]]]
+    channel_types: NotRequired[List[ChannelTypes]]
 
 
 @final
 class RoleOptionData(TypedDict):
     type: Literal[8]
     name: str
     name_localizations: NotRequired[Optional[Dict[Locales, str]]]
@@ -244,15 +236,15 @@
     description_localizations: NotRequired[Optional[Dict[Locales, str]]]
     required: NotRequired[bool]
     autocomplete: NotRequired[bool]
 
 
 @final
 class AttachmentOptionData(TypedDict):
-    type: Literal[10]
+    type: Literal[11]
     name: str
     name_localizations: NotRequired[Optional[Dict[Locales, str]]]
     description: str
     description_localizations: NotRequired[Optional[Dict[Locales, str]]]
     required: NotRequired[bool]
 
 
@@ -297,114 +289,23 @@
 @final
 class NumberCommandOptionChoiceData(TypedDict):
     name: str
     name_localizations: NotRequired[Optional[Dict[Locales, str]]]
     value: Union[int, float]
 
 
-# https://discord.com/developers/docs/interactions/application-commands#application-command-object-application-command-interaction-data-option-structure
-
-
-@final
-class SubcommandOptionInteractionData(TypedDict):
-    name: str
-    type: Literal[1]
-    options: List[ApplicationCommandOptionInteractionData]
-
-
-@final
-class SubcommandGroupOptionInteractionData(TypedDict):
-    name: str
-    type: Literal[2]
-    options: List[SubcommandOptionInteractionData]
-
-
-@final
-class StringOptionInteractionData(TypedDict):
-    name: str
-    type: Literal[3]
-    value: str
-    focused: NotRequired[bool]
-
-
-@final
-class IntegerOptionInteractionData(TypedDict):
-    name: str
-    type: Literal[4]
-    value: int
-    focused: NotRequired[bool]
-
-
-@final
-class BooleanOptionInteractionData(TypedDict):
-    name: str
-    type: Literal[5]
-    value: bool
-
-
-@final
-class UserOptionInteractionData(TypedDict):
-    name: str
-    type: Literal[6]
-    value: Snowflake
-
-
-@final
-class ChannelOptionInteractionData(TypedDict):
-    name: str
-    type: Literal[7]
-    value: Snowflake
-
-
-@final
-class RoleOptionInteractionData(TypedDict):
-    name: str
-    type: Literal[8]
-    value: Snowflake
-
-
-@final
-class MentionableInteractionData(TypedDict):
-    name: str
-    type: Literal[9]
-    value: Snowflake
-
-
-@final
-class NumberInteractionData(TypedDict):
-    name: str
-    type: Literal[10]
-    value: Union[int, float]
-    focused: NotRequired[bool]
-
-
-@final
-class AttachmentInteractionData(TypedDict):
-    name: str
-    type: Literal[10]
-    value: str
-
-
-ApplicationCommandOptionInteractionData = Union[
-    SubcommandOptionInteractionData, SubcommandGroupOptionInteractionData,
-    StringOptionInteractionData, IntegerOptionInteractionData, BooleanOptionInteractionData,
-    UserOptionInteractionData, ChannelOptionInteractionData, RoleOptionInteractionData,
-    MentionableInteractionData, NumberInteractionData, AttachmentInteractionData,
-]
-
-
 # https://discord.com/developers/docs/interactions/application-commands#application-command-permissions-object-guild-application-command-permissions-structure
 
 
 @final
 class GuildApplicationCommandPermissionData(TypedDict):
     id: Snowflake
     application_id: Snowflake
     guild_id: Snowflake
-    permissions: ApplicationCommandPermissionsData
+    permissions: List[ApplicationCommandPermissionsData]
 
 
 # https://discord.com/developers/docs/interactions/application-commands#application-command-permissions-object-application-command-permissions-structure
 
 
 @final
 class ApplicationCommandPermissionsData(TypedDict):
@@ -421,20 +322,22 @@
 
 # https://discord.com/developers/docs/interactions/application-commands#create-global-application-command-json-params
 
 
 @final
 class ApplicationCommandPayload(TypedDict):
     name: str
-    description: str
+    description: NotRequired[str]
     options: NotRequired[List[ApplicationCommandOptionData]]
-    default_permission: NotRequired[bool]
+    default_member_permissions: NotRequired[Optional[str]]
+    dm_permission: NotRequired[bool]
     type: NotRequired[Literal[1, 2, 3]]
+    nsfw: NotRequired[bool]
 
 
 # https://discord.com/developers/docs/interactions/application-commands#batch-edit-application-command-permissions-example
 
 
 @final
-class BatchEditApplicationCommandPermissionsData(TypedDict):
+class EditApplicationCommandPermissionsData(TypedDict):
     id: Snowflake
     permissions: ApplicationCommandPermissionsData
```

### Comparing `discord-typings-0.5.1/discord_typings/interactions/components.py` & `discord_typings-0.6.0/discord_typings/_interactions/_components.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, List, Union
 
 from typing_extensions import Literal, NotRequired, TypedDict, final
 
 if TYPE_CHECKING:
-    from ..resources import EmojiData
+    from .._resources import ChannelTypes, EmojiData
 
 __all__ = (
     'ComponentTypes', 'ActionRowData', 'ButtonComponentData', 'ButtonStyles',
-    'SelectMenuComponentData', 'SelectMenuOptionData', 'TextInputComponentData',
-    'ComponentData'
+    'StringSelectMenuComponentData', 'UserSelectMenuComponentData',
+    'RoleSelectMenuComponentData', 'MentionableSelectMenuComponentData',
+    'ChannelSelectMenuComponentData', 'SelectMenuComponentData',
+    'SelectMenuOptionData', 'TextInputComponentData', 'ComponentData',
 )
 
 
 # https://discord.com/developers/docs/interactions/message-components#component-object-component-types
 
 
-ComponentTypes = Literal[1, 2, 3, 4]
+ComponentTypes = Literal[1, 2, 3, 4, 5, 6, 7, 8]
 
 
 # https://discord.com/developers/docs/interactions/message-components#action-rows
 
 
 @final
 class ActionRowData(TypedDict):
@@ -64,24 +66,72 @@
 ButtonStyles = Literal[1, 2, 3, 4, 5]
 
 
 # https://discord.com/developers/docs/interactions/message-components#select-menu-object-select-menu-structure
 
 
 @final
-class SelectMenuComponentData(TypedDict):
+class StringSelectMenuComponentData(TypedDict):
     type: Literal[3]
     custom_id: str
     options: List[SelectMenuOptionData]
     placeholder: NotRequired[str]
     min_values: NotRequired[int]
     max_values: NotRequired[int]
     disabled: NotRequired[bool]
 
 
+@final
+class UserSelectMenuComponentData(TypedDict):
+    type: Literal[5]
+    custom_id: str
+    placeholder: NotRequired[str]
+    min_values: NotRequired[int]
+    max_values: NotRequired[int]
+    disabled: NotRequired[bool]
+
+
+@final
+class RoleSelectMenuComponentData(TypedDict):
+    type: Literal[6]
+    custom_id: str
+    placeholder: NotRequired[str]
+    min_values: NotRequired[int]
+    max_values: NotRequired[int]
+    disabled: NotRequired[bool]
+
+
+@final
+class MentionableSelectMenuComponentData(TypedDict):
+    type: Literal[7]
+    custom_id: str
+    placeholder: NotRequired[str]
+    min_values: NotRequired[int]
+    max_values: NotRequired[int]
+    disabled: NotRequired[bool]
+
+
+@final
+class ChannelSelectMenuComponentData(TypedDict):
+    type: Literal[8]
+    custom_id: str
+    channel_types: List[ChannelTypes]
+    placeholder: NotRequired[str]
+    min_values: NotRequired[int]
+    max_values: NotRequired[int]
+    disabled: NotRequired[bool]
+
+
+SelectMenuComponentData = Union[
+    StringSelectMenuComponentData, UserSelectMenuComponentData,
+    RoleSelectMenuComponentData, MentionableSelectMenuComponentData,
+    ChannelSelectMenuComponentData,
+]
+
+
 # https://discord.com/developers/docs/interactions/message-components#select-menu-object-select-option-structure
 
 
 @final
 class SelectMenuOptionData(TypedDict):
     label: str
     value: str
```

### Comparing `discord-typings-0.5.1/discord_typings/interactions/receiving.py` & `discord_typings-0.6.0/discord_typings/_interactions/_receiving.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict, List, Union
 
 from typing_extensions import Literal, NotRequired, TypedDict, final
 
 if TYPE_CHECKING:
-    from ..reference import Snowflake
-    from ..resources import (
+    from .._reference import Snowflake
+    from .._resources import (
         AllowedMentionsData, AttachmentData, EmbedData, GuildMemberData,
-        MessageData, PartialChannelData, RoleData, UserData
-    )
-    from .commands import (
-        ApplicationCommandOptionInteractionData, AutocompleteOptionData,
-        Locales, SubcommandGroupOptionInteractionData,
-        SubcommandOptionInteractionData
-    )
-    from .components import (
-        ComponentData, SelectMenuComponentData, SelectMenuOptionData,
-        TextInputComponentData
+        MessageData, PartialAttachmentData, PartialChannelData, RoleData,
+        UserData
     )
+    from ._commands import AutocompleteOptionData, Locales
+    from ._components import ActionRowData, ComponentData, SelectMenuOptionData
 
 __all__ = (
     'InteractionData', 'InteractionType', 'ResolvedInteractionDataData',
     'MessageInteractionData', 'InteractionResponseData', 'InteractionCallbackTypes',
     'InteractionCallbackData', 'ApplicationCommandInteractionData',
     'ComponentInteractionData', 'AutocompleteInteractionData', 'InteractionData',
     'InteractionMessageCallbackData', 'InteractionAutocompleteCallbackData',
     'InteractionModalCallbackData', 'InteractionMessageResponseData',
     'InteractionAutocompleteResponseData', 'InteractionModalResponseData',
-    'InteractionNodataResponseData', 'ModalInteractionData'
+    'InteractionNodataResponseData', 'ModalInteractionData',
+    'ApplicationCommandOptionInteractionData', 'SelectMenuComponentInteractionDataData',
+    'ButtonComponentInteractionDataData', 'ChatInputCommandInteractionDataData',
+    'ContextMenuInteractionDataData', 'ComponentInteractionDataData',
+    'InteractionDataData'
 )
 
 
 # https://discord.com/developers/docs/interactions/receiving-and-responding#interaction-object-interaction-structure
 
 
 class GuildInteractionData(TypedDict):
@@ -59,91 +57,65 @@
     type: Literal[3]
     data: ComponentInteractionDataData
     message: MessageData
     app_permissions: str
 
 
 @final
+class AutocompleteGuildInteractionData(GuildInteractionData):
+    type: Literal[4]
+    data: ApplicationCommandInteractionDataData
+
+
+@final
 class ModalGuildInteractionData(GuildInteractionData):
     type: Literal[5]
-    data: ModalComponentInteractionDataData
+    data: ModalSubmitInteractionDataData
     message: MessageData
     app_permissions: str
 
 
-@final
-class AutocompleteGuildInteractionData(GuildInteractionData):
-    type: Literal[4]
-    data: ApplicationCommandInteractionDataData
-
-
 class ChannelInteractionData(TypedDict):
     id: Snowflake
     application_id: Snowflake
     channel_id: Snowflake
     user: UserData
     token: str
     version: int
     locale: Locales
 
 
 @final
 class ApplicationCommandChannelInteractionData(ChannelInteractionData):
     type: Literal[2]
-    data: ApplicationCommandInteractionDataData
-    app_permissions: str
+    data: Union[ApplicationCommandInteractionDataData, ContextMenuInteractionDataData]
 
 
 @final
 class ComponentChannelInteractionData(ChannelInteractionData):
     type: Literal[3]
     data: ComponentInteractionDataData
     message: MessageData
-    app_permissions: str
-
-
-@final
-class ModalChannelInteractionData(ChannelInteractionData):
-    type: Literal[5]
-    data: ModalComponentInteractionDataData
-    message: MessageData
-    app_permissions: str
 
 
 @final
 class AutocompleteChannelInteractionData(ChannelInteractionData):
     type: Literal[4]
     data: ApplicationCommandInteractionDataData
 
 
-class UserCommandInteractionBase(TypedDict):
-    id: Snowflake
-    application_id: Snowflake
-    type: Literal[2]
-    data: ContextMenuInteractionDataData
-    token: str
-    version: int
-    locale: Locales
-    app_permissions: str
-
-
-@final
-class GuildUserCommandInteractionData(UserCommandInteractionBase):
-    member: GuildMemberData
-    guild_locale: Locales
-
-
 @final
-class ChannelUserCommandInteractionData(UserCommandInteractionBase):
-    user: UserData
+class ModalChannelInteractionData(ChannelInteractionData):
+    type: Literal[5]
+    data: ModalSubmitInteractionDataData
+    message: MessageData
 
 
 ApplicationCommandInteractionData = Union[
     ApplicationCommandGuildInteractionData, ApplicationCommandChannelInteractionData,
-    GuildUserCommandInteractionData, ChannelUserCommandInteractionData
 ]
 
 
 ComponentInteractionData = Union[
     ComponentGuildInteractionData, ComponentChannelInteractionData
 ]
 
@@ -165,100 +137,204 @@
 
 # https://discord.com/developers/docs/interactions/receiving-and-responding#interaction-object-interaction-type
 
 
 InteractionType = Literal[1, 2, 3, 4, 5]
 
 
-# https://discord.com/developers/docs/interactions/receiving-and-responding#interaction-object-interaction-data-structure
+# https://discord.com/developers/docs/interactions/receiving-and-responding#interaction-object-application-command-data-structure
 
 
-class ApplicationCommandInteractionDataBase(TypedDict):
+@final
+class ChatInputCommandInteractionDataData(TypedDict):
     id: Snowflake
     name: str
-    type: Literal[1, 2, 3]
+    type: Literal[1]
     resolved: NotRequired[ResolvedInteractionDataData]
-    options: NotRequired[
-        List[Union[
-            SubcommandOptionInteractionData,
-            SubcommandGroupOptionInteractionData,
-            ApplicationCommandOptionInteractionData
-        ]]
-    ]
+    options: NotRequired[List[ApplicationCommandOptionInteractionData]]
+    guild_id: NotRequired[Snowflake]
 
 
 @final
-class ApplicationCommandInteractionDataData(ApplicationCommandInteractionDataBase):
-    pass
+class ContextMenuInteractionDataData(TypedDict):
+    id: Snowflake
+    name: str
+    type: Literal[2, 3]
+    resolved: NotRequired[ResolvedInteractionDataData]
+    guild_id: NotRequired[Snowflake]
+    target_id: Snowflake
 
 
-@final
-class ButtonComponentInteractionDataData(TypedDict):
-    custom_id: str
-    component_type: Literal[2]
+ApplicationCommandInteractionDataData = Union[
+    ChatInputCommandInteractionDataData, ContextMenuInteractionDataData
+]
+
+
+# https://discord.com/developers/docs/interactions/receiving-and-responding#interaction-object-message-component-data-structure
 
 
 @final
-class SelectComponentInteractionDataData(TypedDict):
+class ButtonComponentInteractionDataData(TypedDict):
     custom_id: str
-    component_type: Literal[3]
-    values: List[SelectMenuOptionData]
+    component_type: Literal[2]
 
 
 @final
-class ModalComponentInteractionDataData(TypedDict):
+class SelectMenuComponentInteractionDataData(TypedDict):
     custom_id: str
-    component_type: Literal[4]
-    components: List[Union[TextInputComponentData, SelectMenuComponentData]]
+    component_type: Literal[3, 5, 6, 7, 8]
+    values: NotRequired[List[SelectMenuOptionData]]
+    resolved: NotRequired[ResolvedInteractionDataData]
 
 
 ComponentInteractionDataData = Union[
-    ButtonComponentInteractionDataData, SelectComponentInteractionDataData,
-    ModalComponentInteractionDataData
+    ButtonComponentInteractionDataData, SelectMenuComponentInteractionDataData
 ]
 
+# https://discord.com/developers/docs/interactions/receiving-and-responding#interaction-object-modal-submit-data-structure
+
 
 @final
-class ContextMenuInteractionDataData(ApplicationCommandInteractionDataBase):
-    target_id: Snowflake
+class ModalSubmitInteractionDataData(TypedDict):
+    custom_id: str
+    component_type: Literal[4]
+    components: List[ActionRowData]
 
 
 InteractionDataData = Union[
-    ApplicationCommandInteractionDataData, ButtonComponentInteractionDataData,
-    SelectComponentInteractionDataData, ContextMenuInteractionDataData
+    ApplicationCommandInteractionDataData, ComponentInteractionDataData,
+    ModalSubmitInteractionDataData
 ]
 
 
 # https://discord.com/developers/docs/interactions/receiving-and-responding#interaction-object-resolved-data-structure
 
 
 @final
 class ResolvedInteractionDataData(TypedDict):
     users: NotRequired[Dict[Snowflake, UserData]]
     members: NotRequired[Dict[Snowflake, GuildMemberData]]
     roles: NotRequired[Dict[Snowflake, RoleData]]
     channels: NotRequired[Dict[Snowflake, PartialChannelData]]
     messages: NotRequired[Dict[Snowflake, MessageData]]
+    attachments: NotRequired[Dict[Snowflake, AttachmentData]]
+
+
+# https://discord.com/developers/docs/interactions/receiving-and-responding#interaction-object-application-command-interaction-data-option-structure
+
+
+@final
+class SubcommandOptionInteractionData(TypedDict):
+    name: str
+    type: Literal[1]
+    options: List[ApplicationCommandOptionInteractionData]
+
+
+@final
+class SubcommandGroupOptionInteractionData(TypedDict):
+    name: str
+    type: Literal[2]
+    options: List[SubcommandOptionInteractionData]
+
+
+@final
+class StringOptionInteractionData(TypedDict):
+    name: str
+    type: Literal[3]
+    value: str
+    focused: NotRequired[bool]
+
+
+@final
+class IntegerOptionInteractionData(TypedDict):
+    name: str
+    type: Literal[4]
+    value: int
+    focused: NotRequired[bool]
+
+
+@final
+class BooleanOptionInteractionData(TypedDict):
+    name: str
+    type: Literal[5]
+    value: bool
+
+
+@final
+class UserOptionInteractionData(TypedDict):
+    name: str
+    type: Literal[6]
+    value: Snowflake
+
+
+@final
+class ChannelOptionInteractionData(TypedDict):
+    name: str
+    type: Literal[7]
+    value: Snowflake
+
+
+@final
+class RoleOptionInteractionData(TypedDict):
+    name: str
+    type: Literal[8]
+    value: Snowflake
+
+
+@final
+class MentionableInteractionData(TypedDict):
+    name: str
+    type: Literal[9]
+    value: Snowflake
+
+
+@final
+class NumberInteractionData(TypedDict):
+    name: str
+    type: Literal[10]
+    value: Union[int, float]
+    focused: NotRequired[bool]
+
+
+@final
+class AttachmentInteractionData(TypedDict):
+    name: str
+    type: Literal[11]
+    value: str
+
+
+ApplicationCommandOptionInteractionData = Union[
+    SubcommandOptionInteractionData, SubcommandGroupOptionInteractionData,
+    StringOptionInteractionData, IntegerOptionInteractionData, BooleanOptionInteractionData,
+    UserOptionInteractionData, ChannelOptionInteractionData, RoleOptionInteractionData,
+    MentionableInteractionData, NumberInteractionData, AttachmentInteractionData,
+]
 
 
 # https://discord.com/developers/docs/interactions/receiving-and-responding#message-interaction-object-message-interaction-structure
 
 
 @final
 class MessageInteractionData(TypedDict):
     id: Snowflake
     type: Literal[2, 3, 4]
     name: str
     user: UserData
+    member: NotRequired[GuildMemberData]
 
 
 # https://discord.com/developers/docs/interactions/receiving-and-responding#interaction-response-object-interaction-response-structure
 
 
 @final
+class InteractionNodataResponseData(TypedDict):
+    type: Literal[1, 5, 6]
+
+
+@final
 class InteractionMessageResponseData(TypedDict):
     type: Literal[4, 7]
     data: InteractionMessageCallbackData
 
 
 @final
 class InteractionAutocompleteResponseData(TypedDict):
@@ -268,22 +344,17 @@
 
 @final
 class InteractionModalResponseData(TypedDict):
     type: Literal[9]
     data: InteractionModalCallbackData
 
 
-@final
-class InteractionNodataResponseData(TypedDict):
-    type: Literal[1, 5, 6]
-
-
 InteractionResponseData = Union[
-    InteractionMessageResponseData, InteractionAutocompleteResponseData,
-    InteractionModalResponseData, InteractionNodataResponseData
+    InteractionNodataResponseData, InteractionMessageResponseData,
+    InteractionAutocompleteResponseData, InteractionModalResponseData,
 ]
 
 
 # https://discord.com/developers/docs/interactions/receiving-and-responding#interaction-response-object-interaction-callback-type
 
 
 InteractionCallbackTypes = Literal[1, 4, 5, 6, 7, 8, 9]
@@ -296,26 +367,26 @@
 class InteractionMessageCallbackData(TypedDict):
     tts: NotRequired[bool]
     content: NotRequired[str]
     embeds: NotRequired[List[EmbedData]]
     allowed_mentions: NotRequired[AllowedMentionsData]
     flags: NotRequired[int]
     components: NotRequired[List[ComponentData]]
-    attachments: NotRequired[List[AttachmentData]]
+    attachments: NotRequired[List[PartialAttachmentData]]
 
 
 @final
 class InteractionAutocompleteCallbackData(TypedDict):
     choices: List[AutocompleteOptionData]
 
 
 @final
 class InteractionModalCallbackData(TypedDict):
     custom_id: str
     title: str
-    components: List[ComponentData]
+    components: List[ActionRowData]
 
 
 InteractionCallbackData = Union[
     InteractionMessageCallbackData, InteractionAutocompleteCallbackData,
     InteractionModalCallbackData
 ]
```

### Comparing `discord-typings-0.5.1/discord_typings/resources/application.py` & `discord_typings-0.6.0/discord_typings/_resources/_application.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,55 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, List, Optional
 
 from typing_extensions import NotRequired, TypedDict, final
 
 if TYPE_CHECKING:
-    from ..reference import Snowflake
-    from .user import UserData
+    from .._reference import Snowflake
+    from ._user import UserData
 
-__all__ = ('ApplicationData', 'TeamData', 'TeamMemberData')
+__all__ = ('ApplicationData', 'TeamData', 'TeamMemberData', 'InstallParams')
 
 
 # https://discord.com/developers/docs/resources/application#application-object-application-structure
 
 
 @final
 class ApplicationData(TypedDict):
     id: Snowflake
     name: str
     icon: Optional[str]
     description: str
-    rpc_origins: List[str]
+    rpc_origins: NotRequired[List[str]]
     bot_public: bool
     bot_require_code_grant: bool
     terms_of_service_url: NotRequired[str]
     privacy_policy_url: NotRequired[str]
     owner: NotRequired[UserData]
-    summary: str
     verify_key: str
     team: Optional[TeamData]
     guild_id: NotRequired[Snowflake]
     primary_sku_id: NotRequired[Snowflake]
     slug: NotRequired[str]
     cover_image: NotRequired[str]
     flags: NotRequired[int]
+    tags: NotRequired[List[str]]
+    install_params: NotRequired[InstallParams]
+    custom_install_url: NotRequired[str]
+    role_connections_verification_url: NotRequired[str]
+
+
+# https://discord.com/developers/docs/resources/application#install-params-object-install-params-structure
+
+
+@final
+class InstallParams(TypedDict):
+    scopes: List[str]
+    permissions: str
 
 
 # https://discord.com/developers/docs/topics/teams#data-models-team-object
 
 
 @final
 class TeamData(TypedDict):
```

### Comparing `discord-typings-0.5.1/discord_typings/resources/audit_log.py` & `discord_typings-0.6.0/discord_typings/_resources/_audit_log.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, List, Optional
 
 from typing_extensions import Literal, NotRequired, TypedDict, final
 
 if TYPE_CHECKING:
-    from ..reference import Snowflake
-    from .channel import ThreadChannelData
-    from .guild import IntegrationAccountData
-    from .user import UserData
-    from .webhook import WebhookData
+    from .._interactions import ApplicationCommandData
+    from .._reference import Snowflake
+    from ._auto_moderation import AutoModerationRuleData
+    from ._channel import ThreadChannelData
+    from ._guild import IntegrationAccountData
+    from ._guild_scheduled_events import GuildScheduledEventData
+    from ._user import UserData
+    from ._webhook import WebhookData
 
 __all__ = (
     'AuditLogData', 'AuditLogEntryData', 'OptionalAuditLogEntryData',
     'AuditLogChangeData', 'AuditLogEvents'
 )
 
 
 # https://discord.com/developers/docs/resources/audit-log#audit-log-object-audit-log-structure
 
 
 @final
 class AuditLogData(TypedDict):
+    application_commands: List[ApplicationCommandData]
     audit_log_entries: List[AuditLogEntryData]
+    auto_moderation_rules: List[AutoModerationRuleData]
+    guild_scheduled_events: List[GuildScheduledEventData]
     integrations: List[PartialIntegrationData]
     threads: List[ThreadChannelData]
     users: List[UserData]
     webhooks: List[WebhookData]
 
 
 @final
 class PartialIntegrationData(TypedDict):
     id: Snowflake
     name: str
     type: Literal['twitch', 'youtube', 'discord']
     account: IntegrationAccountData
+    application_id: Snowflake
 
 
 # https://discord.com/developers/docs/resources/audit-log#audit-log-entry-object-audit-log-entry-structure
 
 
 @final
 class AuditLogEntryData(TypedDict):
@@ -62,31 +69,36 @@
     40, 41, 42,
     50, 51, 52,
     60, 61, 62,
     72, 73, 74, 75,
     80, 81, 82, 83, 84, 85,
     90, 91, 92,
     100, 101, 102,
-    110, 111, 112
+    110, 111, 112,
+    121,
+    140, 141, 142, 143, 144, 145,
 ]
 
 
 # https://discord.com/developers/docs/resources/audit-log#audit-log-entry-object-optional-audit-entry-info
 
 
 @final
 class OptionalAuditLogEntryData(TypedDict):
+    application_id: NotRequired[Snowflake]
+    auto_moderation_rule_name: NotRequired[str]
+    auto_moderation_trigger_type: NotRequired[str]  # AutoModerationTriggerTypes
     channel_id: NotRequired[Snowflake]
     count: NotRequired[str]
     delete_member_days: NotRequired[str]
     id: NotRequired[Snowflake]
     members_removed: NotRequired[str]
-    message_id: NotRequired[str]
+    message_id: NotRequired[Snowflake]
     role_name: NotRequired[str]
-    type: NotRequired[str]
+    type: NotRequired[Literal['0', '1']]
 
 
 # https://discord.com/developers/docs/resources/audit-log#audit-log-change-object-audit-log-change-structure
 
 
 @final
 class AuditLogChangeData(TypedDict):
```

### Comparing `discord-typings-0.5.1/discord_typings/resources/auto_moderation.py` & `discord_typings-0.6.0/discord_typings/_resources/_auto_moderation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import List, Union
 
 from typing_extensions import Literal, TypedDict, final
 
-from ..reference import Snowflake
+from .._reference import Snowflake
 
 __all__ = [
     'AutoModerationRuleData', 'AutoModerationTriggerTypes',
     'AutoModerationTriggerMetadataData', 'AutoModerationKeywordPresetTypes',
     'AutoModerationEventTypes', 'AutoModerationActionData', 'AutoModerationActionTypes',
 
 ]
@@ -29,14 +29,29 @@
     actions: List[AutoModerationActionData]
     enabled: bool
     exempt_roles: List[Snowflake]
     exempt_channels: List[Snowflake]
 
 
 @final
+class SpamAutoModerationRuleData(TypedDict):
+    id: Snowflake
+    guild_id: Snowflake
+    name: str
+    creator_id: Snowflake
+    event_type: AutoModerationEventTypes
+    trigger_type: Literal[3]
+    trigger_metadata: EmptyTriggerMetadataData
+    actions: List[AutoModerationActionData]
+    enabled: bool
+    exempt_roles: List[Snowflake]
+    exempt_channels: List[Snowflake]
+
+
+@final
 class KeywordPresetAutoModerationRuleData(TypedDict):
     id: Snowflake
     guild_id: Snowflake
     name: str
     creator_id: Snowflake
     event_type: AutoModerationEventTypes
     trigger_type: Literal[4]
@@ -44,31 +59,30 @@
     actions: List[AutoModerationActionData]
     enabled: bool
     exempt_roles: List[Snowflake]
     exempt_channels: List[Snowflake]
 
 
 @final
-class HarmfulLinkSpamAutoModerationRuleData(TypedDict):
+class MentionSpamAutoModerationRuleData(TypedDict):
     id: Snowflake
     guild_id: Snowflake
     name: str
     creator_id: Snowflake
-    event_type: AutoModerationEventTypes
-    trigger_type: Literal[2, 3]
-    trigger_metadata: EmptyTriggerMetadataData
+    event_type: Literal[5]
+    trigger_metadata: MentionSpamTriggerMetadataData
     actions: List[AutoModerationActionData]
     enabled: bool
     exempt_roles: List[Snowflake]
     exempt_channels: List[Snowflake]
 
 
 AutoModerationRuleData = Union[
     KeywordAutoModerationRuleData, KeywordPresetAutoModerationRuleData,
-    HarmfulLinkSpamAutoModerationRuleData
+    SpamAutoModerationRuleData, MentionSpamAutoModerationRuleData
 ]
 
 
 # https://discord.com/developers/docs/resources/auto-moderation#auto-moderation-rule-object-trigger-types
 
 
 AutoModerationTriggerTypes = Literal[1, 2, 3, 4]
@@ -76,29 +90,37 @@
 
 # https://discord.com/developers/docs/resources/auto-moderation#auto-moderation-rule-object-trigger-metadata
 
 
 @final
 class KeywordTriggerMetadataData(TypedDict):
     keyword_filter: List[str]
+    allow_list: List[str]
+
+    regex_patterns: List[str]
 
 
 @final
 class KeywordPresetTriggerMetadataData(TypedDict):
     presets: List[AutoModerationKeywordPresetTypes]
 
 
 @final
+class MentionSpamTriggerMetadataData(TypedDict):
+    mention_total_limit: int
+
+
+@final
 class EmptyTriggerMetadataData(TypedDict):
     ...
 
 
 AutoModerationTriggerMetadataData = Union[
     KeywordTriggerMetadataData, KeywordPresetTriggerMetadataData,
-    EmptyTriggerMetadataData
+    MentionSpamTriggerMetadataData, EmptyTriggerMetadataData
 ]
 
 
 # https://discord.com/developers/docs/resources/auto-moderation#auto-moderation-rule-object-keyword-preset-types
 
 
 AutoModerationKeywordPresetTypes = Literal[1, 2, 3]
```

### Comparing `discord-typings-0.5.1/discord_typings/resources/channel.py` & `discord_typings-0.6.0/discord_typings/_resources/_channel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, List, Optional, Union
 
 from typing_extensions import Literal, NotRequired, TypedDict, final
 
-from .user import UserBase  # Subclassed for UserMentionData
+from ._user import UserBase  # Subclassed for UserMentionData
 
 if TYPE_CHECKING:
-    from ..interactions import ComponentData, MessageInteractionData
-    from ..reference import Snowflake
-    from .application import ApplicationData
-    from .emoji import EmojiData
-    from .guild import GuildMemberData
-    from .sticker import StickerItemData
-    from .user import UserData
+    from .._interactions import ComponentData, MessageInteractionData
+    from .._reference import Snowflake
+    from ._application import ApplicationData
+    from ._emoji import EmojiData
+    from ._guild import GuildMemberData
+    from ._sticker import StickerItemData
+    from ._user import UserData
 
 __all__ = (
     'PartialChannelData', 'TextChannelData', 'NewsChannelData', 'DMChannelData',
     'GroupDMChannelData', 'VoiceChannelData', 'CategoryChannelData',
     'ChannelData', 'ChannelTypes', 'VideoQualityModes', 'ChannelMessageData',
     'GuildMessageData', 'MessageData', 'UserMentionData', 'MessageTypes',
     'MessageActivityData', 'MessageActivityTypes', 'PermissionOverwriteData',
     'ThreadChannelData', 'MessageReferenceData', 'FollowedChannelData',
-    'PermissionOverwriteData', 'ThreadMetadata', 'ThreadMemberData', 'EmbedData',
+    'PermissionOverwriteData', 'ThreadMetadataData', 'ThreadMemberData', 'EmbedData',
     'EmbedThumbnailData', 'EmbedVideoData', 'EmbedImageData',
     'EmbedProviderData', 'EmbedAuthorData', 'EmbedFieldData', 'EmbedFooterData',
     'PartialAttachmentData', 'AttachmentData', 'AllowedMentionsData', 'HasMoreListThreadsData',
-    'ChannelMentionData', 'MessageReactionData',
+    'ChannelMentionData', 'MessageReactionData', 'DefaultReactionData',
+    'ForumTagData', 'ForumChannelData', 'SortOrderTypes', 'RoleSubscriptionData',
 )
 
 
 # https://discord.com/developers/docs/resources/channel#channel-object-channel-structure
 
 
 @final
@@ -52,14 +53,15 @@
     topic: Optional[str]
     nsfw: bool
     last_message_id: Optional[Snowflake]
     rate_limit_per_user: int
     parent_id: Optional[Snowflake]
     last_pin_timestamp: NotRequired[Optional[str]]
     default_auto_archive_duration: NotRequired[int]
+    flags: int
 
 
 @final
 class NewsChannelData(TypedDict):
     id: Snowflake
     type: Literal[5]
     guild_id: NotRequired[Snowflake]  # May be missing during guild dispatches
@@ -68,36 +70,40 @@
     name: str
     topic: Optional[str]
     nsfw: bool
     last_message_id: Optional[Snowflake]
     parent_id: Optional[Snowflake]
     last_pin_timestamp: NotRequired[Optional[str]]
     default_auto_archive_duration: NotRequired[int]
+    flags: int
 
 
 @final
 class DMChannelData(TypedDict):
     id: Snowflake
     type: Literal[1]
     last_message_id: Optional[Snowflake]
     recipients: List[UserData]
     last_pin_timestamp: NotRequired[Optional[str]]
+    flags: int
 
 
 @final
 class GroupDMChannelData(TypedDict):
     id: Snowflake
     type: Literal[3]
     name: str
     last_message_id: Optional[Snowflake]
     recipients: List[UserData]
     icon: Optional[str]
     owner_id: Snowflake
     application_id: NotRequired[Snowflake]
+    managed: bool
     last_pin_timestamp: NotRequired[Optional[str]]
+    flags: int
 
 
 @final
 class ThreadChannelData(TypedDict):
     id: Snowflake
     type: Literal[10, 11, 12]
     guild_id: NotRequired[Snowflake]
@@ -105,50 +111,76 @@
     last_message_id: Optional[Snowflake]
     rate_limit_per_user: int
     owner_id: Snowflake
     parent_id: Optional[Snowflake]
     last_pin_timestamp: NotRequired[Optional[str]]
     message_count: int
     member_count: int
-    thread_metadata: ThreadMetadata
+    thread_metadata: ThreadMetadataData
     member: NotRequired[ThreadMemberData]
+    flags: int
+    total_messages_sent: int
+    applied_tags: NotRequired[List[Snowflake]]
 
 
 @final
 class VoiceChannelData(TypedDict):
     id: Snowflake
     type: Literal[2, 13]
     guild_id: NotRequired[Snowflake]
     position: int
     permission_overwrites: List[PermissionOverwriteData]
     name: str
     nsfw: bool
-    last_message_id: NotRequired[None]
+    last_message_id: NotRequired[Optional[Snowflake]]
     bitrate: int
     user_limit: int
     parent_id: Optional[Snowflake]
+    last_pin_timestamp: NotRequired[Optional[str]]
     rtc_region: Optional[str]
     video_quality_mode: NotRequired[VideoQualityModes]
+    flags: int
 
 
 @final
 class CategoryChannelData(TypedDict):
     id: Snowflake
     type: Literal[4]
     guild_id: NotRequired[Snowflake]
     position: int
     permission_overwrites: List[PermissionOverwriteData]
     name: str
     nsfw: bool
-    parent_id: Optional[Snowflake]
+    flags: int
+
+
+@final
+class ForumChannelData(TypedDict):
+    id: Snowflake
+    type: Literal[15]
+    guild_id: NotRequired[Snowflake]
+    position: int
+    permission_overwrites: List[PermissionOverwriteData]
+    name: str
+    topic: Optional[str]
+    nsfw: bool
+    last_message_id: Optional[Snowflake]
+    rate_limit_per_user: int
+    default_auto_archive_duration: NotRequired[int]
+    flags: int
+    available_tags: List[ForumTagData]
+    default_reaction_emoji: Optional[DefaultReactionData]
+    default_thread_rate_limit_per_user: int
+    default_sort_order: Optional[SortOrderTypes]
+    default_forum_layout: ForumLayoutTypes
 
 
 ChannelData = Union[
     TextChannelData, NewsChannelData, DMChannelData, GroupDMChannelData,
-    ThreadChannelData, VoiceChannelData, CategoryChannelData
+    ThreadChannelData, VoiceChannelData, CategoryChannelData, ForumChannelData
 ]
 
 
 # https://discord.com/developers/docs/resources/channel#channel-object-channel-types
 
 
 ChannelTypes = Literal[0, 1, 2, 3, 4, 5, 10, 11, 12, 13, 14, 15]
@@ -156,14 +188,26 @@
 
 # https://discord.com/developers/docs/resources/channel#channel-object-video-quality-modes
 
 
 VideoQualityModes = Literal[1, 2]
 
 
+# https://discord.com/developers/docs/resources/channel#channel-object-sort-order-types
+
+
+SortOrderTypes = Literal[0, 1]
+
+
+# https://discord.com/developers/docs/resources/channel#channel-object-forum-layout-types
+
+
+ForumLayoutTypes = Literal[0, 1, 2]
+
+
 # https://discord.com/developers/docs/resources/channel#message-object-message-structure
 
 
 class MessageBase(TypedDict):
     id: Snowflake
     channel_id: Snowflake
     author: UserData
@@ -183,19 +227,21 @@
     webhook_id: NotRequired[Snowflake]
     type: MessageTypes
     activity: NotRequired[MessageActivityData]
     application: NotRequired[ApplicationData]
     application_id: NotRequired[Snowflake]
     message_reference: NotRequired[MessageReferenceData]
     flags: NotRequired[int]
-    references_message: NotRequired[Optional[MessageData]]
+    referenced_message: NotRequired[Optional[MessageData]]
     interaction: NotRequired[MessageInteractionData]
     thread: NotRequired[ThreadChannelData]
     components: NotRequired[List[ComponentData]]
     sticker_items: NotRequired[List[StickerItemData]]
+    position: NotRequired[int]
+    role_subscription_data: NotRequired[RoleSubscriptionData]
 
 
 @final
 class ChannelMessageData(MessageBase):
     pass
 
 
@@ -214,15 +260,15 @@
 
 
 # https://discord.com/developers/docs/resources/channel#message-object-message-types
 
 
 MessageTypes = Literal[
     0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 14, 15, 16, 17, 18, 19, 20,
-    21, 22, 23
+    21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32
 ]
 
 
 # https://discord.com/developers/docs/resources/channel#message-object-message-activity-structure
 
 
 @final
@@ -279,33 +325,56 @@
     deny: str
 
 
 # https://discord.com/developers/docs/resources/channel#thread-metadata-object-thread-metadata-structure
 
 
 @final
-class ThreadMetadata(TypedDict):
+class ThreadMetadataData(TypedDict):
     archived: bool
     auto_archive_duration: int
     archive_timestamp: str
     locked: bool
     invitable: NotRequired[bool]
+    create_timestamp: NotRequired[Optional[str]]
 
 
 # https://discord.com/developers/docs/resources/channel#thread-member-object-thread-member-structure
 
 
 @final
 class ThreadMemberData(TypedDict):
     id: NotRequired[Snowflake]
     user_id: NotRequired[Snowflake]
+    member: NotRequired[GuildMemberData]
     join_timestamp: str
     flags: int
 
 
+# https://discord.com/developers/docs/resources/channel#default-reaction-object-default-reaction-structure
+
+
+@final
+class DefaultReactionData(TypedDict):
+    emoji_name: Optional[str]
+    emoji_id: Optional[Snowflake]
+
+
+# https://discord.com/developers/docs/resources/channel#forum-tag-object-forum-tag-structure
+
+
+@final
+class ForumTagData(TypedDict):
+    id: Snowflake
+    name: str
+    moderated: bool
+    emoji_id: Optional[Snowflake]
+    emoji_name: Optional[Snowflake]
+
+
 # https://discord.com/developers/docs/resources/channel#embed-object-embed-structure
 
 
 @final
 class EmbedData(TypedDict):
     title: NotRequired[str]
     type: NotRequired[Literal['rich', 'image', 'video', 'gifv', 'article', 'link']]
@@ -437,14 +506,25 @@
 class AllowedMentionsData(TypedDict):
     parse: NotRequired[List[Literal['roles', 'users', 'everyone']]]
     roles: NotRequired[List[Snowflake]]
     users: NotRequired[List[Snowflake]]
     replied_user: NotRequired[bool]
 
 
+# https://discord.com/developers/docs/resources/channel#role-subscription-data-object-role-subscription-data-object-structure
+
+
+@final
+class RoleSubscriptionData(TypedDict):
+    role_subscription_listing_id: Snowflake
+    tier_name: str
+    total_months_subscribed: int
+    is_renewal: bool
+
+
 # https://discord.com/developers/docs/resources/channel#list-public-archived-threads-response-body
 
 
 @final
 class HasMoreListThreadsData(TypedDict):
     threads: List[ThreadChannelData]
     members: List[ThreadMemberData]
```

### Comparing `discord-typings-0.5.1/discord_typings/resources/emoji.py` & `discord_typings-0.6.0/discord_typings/_resources/_emoji.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, List, Optional
 
 from typing_extensions import NotRequired, TypedDict, final
 
 if TYPE_CHECKING:
-    from ..reference import Snowflake
-    from .user import UserData
+    from .._reference import Snowflake
+    from ._user import UserData
 
 __all__ = ('EmojiData',)
 
 
 # https://discord.com/developers/docs/resources/emoji#emoji-object-emoji-structure
```

### Comparing `discord-typings-0.5.1/discord_typings/resources/guild.py` & `discord_typings-0.6.0/discord_typings/_resources/_guild.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, List, Optional, Union
 
 from typing_extensions import Literal, NotRequired, TypedDict, final
 
 if TYPE_CHECKING:
-    from ..interactions import Locales
-    from ..reference import Snowflake
-    from .channel import ChannelData, ThreadChannelData, ThreadMemberData
-    from .emoji import EmojiData
-    from .sticker import StickerData
-    from .user import UserData
+    from .._oauth import OAuth2Scopes
+    from .._reference import Locales, Snowflake
+    from ._channel import ChannelData, ThreadChannelData, ThreadMemberData
+    from ._emoji import EmojiData
+    from ._sticker import StickerData
+    from ._user import UserData
 
 __all__ = (
     'GuildData', 'DefaultMessageNotificationLevels', 'ExplicitContentFilterLevels',
     'MFALevels', 'VerificationLevels', 'GuildNSFWLevels', 'PremiumTiers', 'GuildFeaturesData',
     'UnavailableGuildData', 'GuildPreviewData', 'GuildWidgetSettingsData', 'GuildWidgetData',
     'GuildMemberData', 'StreamingIntegrationData', 'DiscordIntegrationData', 'IntegrationData',
     'IntegrationExpireBehaviors', 'IntegrationAccountData', 'IntegrationApplicationData',
@@ -38,47 +38,47 @@
 
 
 # https://discord.com/developers/docs/resources/guild#guild-object-guild-structure
 
 
 @final
 class GuildData(TypedDict):
-    id: str
+    id: Snowflake
     name: str
     icon: Optional[str]
     icon_hash: NotRequired[Optional[str]]
     splash: Optional[str]
     discovery_splash: Optional[str]
     owner: NotRequired[bool]
-    owner_id: str
+    owner_id: Snowflake
     permissions: NotRequired[str]
-    afk_channel_id: Optional[str]
+    afk_channel_id: Optional[Snowflake]
     afk_timeout: int
     widget_enabled: NotRequired[bool]
-    widget_channel_id: NotRequired[Optional[str]]
+    widget_channel_id: NotRequired[Optional[Snowflake]]
     verification_level: VerificationLevels
     default_message_notifications: DefaultMessageNotificationLevels
     explicit_content_filter: ExplicitContentFilterLevels
     roles: List[RoleData]
     emojis: List[EmojiData]
     features: List[GuildFeaturesData]
     mfa_level: MFALevels
     application_id: Optional[str]
-    system_channel_id: Optional[str]
+    system_channel_id: Optional[Snowflake]
     system_channel_flags: int
-    rules_channel_id: Optional[str]
+    rules_channel_id: Optional[Snowflake]
     max_presences: NotRequired[Optional[int]]
     max_members: NotRequired[int]
     vanity_url_code: Optional[str]
     description: Optional[str]
     banner: Optional[str]
     premium_tier: PremiumTiers
     premium_subscription_count: NotRequired[int]
     preferred_locale: Locales
-    public_updates_channel_id: Optional[str]
+    public_updates_channel_id: Optional[Snowflake]
     max_video_channel_users: NotRequired[int]
     approximate_member_count: NotRequired[int]
     approximate_presence_count: NotRequired[int]
     welcome_screen: NotRequired[WelcomeScreenData]
     nsfw_level: GuildNSFWLevels
     stickers: NotRequired[List[StickerData]]
     premium_progress_bar_enabled: bool
@@ -120,21 +120,38 @@
 PremiumTiers = Literal[0, 1, 2, 3]
 
 
 # https://discord.com/developers/docs/resources/guild#guild-object-guild-features
 
 
 GuildFeaturesData = Literal[
-    'ANIMATED_ICON', 'BANNER', 'COMMERCE', 'COMMUNITY', 'DISCOVERABLE',
-    'FEATUREABLE', 'INVITE_SPLASH', 'MEMBER_VERIFICATION_GATE_ENABLED',
-    'MONETIZATION_ENABLED', 'MORE_STICKERS', 'NEWS', 'PARTNERED',
-    'PREVIEW_ENABLED', 'PRIVATE_THREADS', 'ROLE_ICONS',
-    'SEVEN_DAY_THREAD_ARCHIVE', 'THREE_DAY_THREAD_ARCHIVE',
-    'TICKETED_EVENTS_ENABLED', 'VANITY_URL', 'VERIFIED',
-    'VIP_REGIONS', 'WELCOME_SCREEN_ENABLED'
+    'ANIMATED_BANNER',
+    'ANIMATED_ICON',
+    'APPLICATION_COMMAND_PERMISSIONS_V2',
+    'AUTO_MODERATION',
+    'BANNER',
+    'COMMUNITY',
+    'DEVELOPER_SUPPORT_SERVER',
+    'DISCOVERABLE',
+    'FEATUREABLE',
+    'INVITES_DISABLED',
+    'INVITE_SPLASH',
+    'MEMBER_VERIFICATION_GATE_ENABLED',
+    'MORE_STICKERS',
+    'NEWS',
+    'PARTNERED',
+    'PREVIEW_ENABLED',
+    'ROLE_ICONS',
+    'ROLE_SUBSCRIPTIONS_AVAILABLE_FOR_PURCHASE',
+    'ROLE_SUBSCRIPTIONS_ENABLED',
+    'TICKETED_EVENTS_ENABLED',
+    'VANITY_URL',
+    'VERIFIED',
+    'VIP_REGIONS',
+    'WELCOME_SCREEN_ENABLED',
 ]
 
 
 # https://discord.com/developers/docs/resources/guild#unavailable-guild-object-example-unavailable-guild
 
 
 @final
@@ -154,14 +171,15 @@
     splash: Optional[str]
     discovery_splash: Optional[str]
     emojis: List[EmojiData]
     features: List[GuildFeaturesData]
     approximate_member_count: int
     approximate_presence_count: int
     description: Optional[str]
+    stickers: List[StickerData]
 
 
 # https://discord.com/developers/docs/resources/guild#guild-widget-object-guild-widget-structure
 
 
 @final
 class GuildWidgetSettingsData(TypedDict):
@@ -191,16 +209,18 @@
     nick: NotRequired[Optional[str]]
     avatar: NotRequired[Optional[str]]
     roles: List[Snowflake]
     joined_at: str
     premium_since: NotRequired[Optional[str]]
     deaf: bool
     mute: bool
+    flags: int
     pending: NotRequired[bool]
     permissions: NotRequired[str]
+    communication_disabled_until: NotRequired[Optional[str]]
 
 
 # https://discord.com/developers/docs/resources/guild#integration-object-integration-structure
 
 
 @final
 class StreamingIntegrationData(TypedDict):
@@ -209,30 +229,33 @@
     type: Literal['twitch', 'youtube', 'discord']
     enabled: bool
     syncing: bool
     role_id: NotRequired[Snowflake]
     enable_emoticons: bool
     expire_behavior: IntegrationExpireBehaviors
     expire_grace_period: int
-    user: UserData
+    user: NotRequired[UserData]
     account: IntegrationAccountData
     synced_at: str
     subscriber_count: int
     revoked: bool
     application: IntegrationApplicationData
+    scopes: NotRequired[List[OAuth2Scopes]]
 
 
 @final
 class DiscordIntegrationData(TypedDict):
     id: Snowflake
     name: str
     type: Literal['discord']
     enabled: bool
+    user: NotRequired[UserData]
     account: IntegrationAccountData
     application: NotRequired[IntegrationApplicationData]
+    scopes: NotRequired[List[OAuth2Scopes]]
 
 
 IntegrationData = Union[StreamingIntegrationData, DiscordIntegrationData]
 
 
 # https://discord.com/developers/docs/resources/guild#integration-object-integration-expire-behaviors
 
@@ -252,18 +275,18 @@
 # https://discord.com/developers/docs/resources/guild#integration-application-object-integration-application-structure
 
 
 @final
 class IntegrationApplicationData(TypedDict):
     id: Snowflake
     name: str
-    icon: NotRequired[str]
+    icon: Optional[str]
     description: str
     summary: str
-    bot: Optional[UserData]
+    bot: NotRequired[Optional[UserData]]
 
 
 # https://discord.com/developers/docs/resources/guild#ban-object-ban-structure
 
 
 @final
 class BanData(TypedDict):
@@ -305,15 +328,14 @@
 # https://discord.com/developers/docs/resources/guild#list-active-threads-response-body
 
 
 @final
 class ListThreadsData(TypedDict):
     threads: List[ThreadChannelData]
     members: List[ThreadMemberData]
-    has_more: bool
 
 
 # https://discord.com/developers/docs/resources/guild#modify-guild-role-positions-json-params
 
 
 @final
 class RolePositionData(TypedDict):
@@ -343,7 +365,10 @@
 
 
 @final
 class RoleTagsData(TypedDict):
     bot_id: NotRequired[Snowflake]
     integration_id: NotRequired[Snowflake]
     premium_subscriber: NotRequired[None]
+    subscription_listing_id: NotRequired[Snowflake]
+    available_for_purchase: NotRequired[None]
+    guild_connections: NotRequired[None]
```

### Comparing `discord-typings-0.5.1/discord_typings/resources/guild_scheduled_events.py` & `discord_typings-0.6.0/discord_typings/_resources/_guild_scheduled_events.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Optional, Union
 
 from typing_extensions import Literal, NotRequired, TypedDict, final
 
 if TYPE_CHECKING:
-    from ..reference import Snowflake
-    from .guild import GuildMemberData
-    from .user import UserData
+    from .._reference import Snowflake
+    from ._guild import GuildMemberData
+    from ._user import UserData
 
 __all__ = (
     'GuildScheduledEventData', 'GuildScheduledEventPrivacyLevels', 'GuildScheduledEventStatus',
-    'GuildScheduledEventEntityTypes', 'GuildScheduledEventEntityMetadata',
+    'GuildScheduledEventEntityTypes', 'GuildScheduledEventEntityMetadataData',
     'GuildScheduledEventUserData'
 )
 
 
 # https://discord.com/developers/docs/resources/guild-scheduled-event#guild-scheduled-event-object-guild-scheduled-event-structure
 
 
 class GuildScheduledEventBase(TypedDict):
     id: Snowflake
     guild_id: Snowflake
     creator_id: Snowflake
     name: str
-    description: NotRequired[str]
+    description: NotRequired[Optional[str]]
     scheduled_start_time: str
     privacy_level: GuildScheduledEventPrivacyLevels
     status: GuildScheduledEventStatus
     entity_type: GuildScheduledEventEntityTypes
     entity_id: Optional[Snowflake]
     creator: UserData
     user_count: NotRequired[int]
+    image: NotRequired[Optional[str]]
 
 
 @final
 class StageGuildScheduledEventData(GuildScheduledEventBase):
     channel_id: Snowflake
     entity_metadata: None
     scheduled_end_time: NotRequired[str]
@@ -47,15 +48,15 @@
     entity_metadata: None
     scheduled_end_time: NotRequired[str]
 
 
 @final
 class ExternalGuildScheduledEventData(GuildScheduledEventBase):
     channel_id: None
-    entity_metadata: GuildScheduledEventEntityMetadata
+    entity_metadata: GuildScheduledEventEntityMetadataData
     scheduled_end_time: str
 
 
 GuildScheduledEventData = Union[
     StageGuildScheduledEventData,
     VoiceGuildScheduledEventData,
     ExternalGuildScheduledEventData
@@ -80,15 +81,15 @@
 GuildScheduledEventStatus = Literal[1, 2, 3, 4]
 
 
 # https://discord.com/developers/docs/resources/guild-scheduled-event#guild-scheduled-event-object-guild-scheduled-event-entity-metadata
 
 
 @final
-class GuildScheduledEventEntityMetadata(TypedDict):
+class GuildScheduledEventEntityMetadataData(TypedDict):
     location: NotRequired[str]
 
 
 # https://discord.com/developers/docs/resources/guild-scheduled-event#guild-scheduled-event-user-object-guild-scheduled-event-user-structure
 
 
 @final
```

### Comparing `discord-typings-0.5.1/discord_typings/resources/guild_template.py` & `discord_typings-0.6.0/discord_typings/_resources/_guild_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Optional
 
 from typing_extensions import TypedDict, final
 
 if TYPE_CHECKING:
-    from ..reference import Snowflake
-    from .guild import GuildData
-    from .user import UserData
+    from .._reference import Snowflake
+    from ._guild import GuildData
+    from ._user import UserData
 
 __all__ = ('GuildTemplateData',)
 
 
 # https://discord.com/developers/docs/resources/invite#invite-stage-instance-object-invite-stage-instance-structure
```

### Comparing `discord-typings-0.5.1/discord_typings/resources/invite.py` & `discord_typings-0.6.0/discord_typings/_resources/_invite.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, List, Optional
 
 from typing_extensions import Literal, NotRequired, TypedDict, final
 
 if TYPE_CHECKING:
-    from .application import ApplicationData
-    from .channel import PartialChannelData
-    from .guild import GuildData, GuildMemberData
-    from .guild_scheduled_events import GuildScheduledEventData
-    from .user import UserData
+    from ._application import ApplicationData
+    from ._channel import PartialChannelData
+    from ._guild import GuildMemberData, PartialGuildData
+    from ._guild_scheduled_events import GuildScheduledEventData
+    from ._user import UserData
 
-__all__ = ('InviteData', 'InviteTargetTypes', 'InviteMetadata')
+__all__ = ('InviteData', 'InviteTargetTypes', 'InviteMetadata', 'InviteStageInstanceData')
 
 
 # https://discord.com/developers/docs/resources/invite#invite-object-invite-structure
 
 
-class InviteBase(TypedDict):
+class _InviteBase(TypedDict):
     code: str
-    guild: NotRequired[GuildData]
-    channel: PartialChannelData
+    guild: NotRequired[PartialGuildData]
+    channel: Optional[PartialChannelData]
     inviter: NotRequired[UserData]
-    target_type: InviteTargetTypes
+    target_type: NotRequired[InviteTargetTypes]
     target_user: NotRequired[UserData]
     target_application: NotRequired[ApplicationData]
     approximate_presence_count: NotRequired[int]
     approximate_member_count: NotRequired[int]
     expires_at: NotRequired[Optional[str]]
     stage_instance: NotRequired[InviteStageInstanceData]
     guild_scheduled_event: NotRequired[GuildScheduledEventData]
 
 
 @final
-class InviteData(InviteBase):
+class InviteData(_InviteBase):
     pass
 
 
 # https://discord.com/developers/docs/resources/invite#invite-object-invite-target-types
 
 
 InviteTargetTypes = Literal[1, 2]
 
 
 # https://discord.com/developers/docs/resources/invite#invite-metadata-object-invite-metadata-structure
 
 
 @final
-class InviteMetadata(InviteBase):
+class InviteMetadata(_InviteBase):
     uses: int
     max_uses: int
     max_age: int
     temporary: bool
     created_at: str
```

### Comparing `discord-typings-0.5.1/discord_typings/resources/stage_instance.py` & `discord_typings-0.6.0/discord_typings/_resources/_stage_instance.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
 from typing_extensions import Literal, TypedDict, final
 
 if TYPE_CHECKING:
-    from ..reference import Snowflake
+    from .._reference import Snowflake
 
 __all__ = ('StageInstanceData', 'StageInstancePrivacyLevels')
 
 
 # https://discord.com/developers/docs/resources/stage-instance#stage-instance-object-stage-instance-structure
 
 
@@ -17,13 +17,14 @@
 class StageInstanceData(TypedDict):
     id: Snowflake
     guild_id: Snowflake
     channel_id: Snowflake
     topic: str
     privacy_level: StageInstancePrivacyLevels
     discoverable_disabled: bool
+    guild_scheduled_event_id: Optional[Snowflake]
 
 
 # https://discord.com/developers/docs/resources/stage-instance#stage-instance-object-privacy-level
 
 
 StageInstancePrivacyLevels = Literal[1, 2]
```

### Comparing `discord-typings-0.5.1/discord_typings/resources/sticker.py` & `discord_typings-0.6.0/discord_typings/_resources/_sticker.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, List, Optional
 
 from typing_extensions import Literal, NotRequired, TypedDict, final
 
 if TYPE_CHECKING:
-    from ..reference import Snowflake
-    from .user import UserData
+    from .._reference import Snowflake
+    from ._user import UserData
 
 __all__ = [
     'StickerItemData', 'StickerTypes', 'StickerFormatTypes', 'StickerData',
     'StickerPackData',
 ]
 
 
 # https://discord.com/developers/docs/resources/sticker#sticker-item-object-sticker-item-structure
 
 
 # Because of inheritance, this class comes first even though that is not the
 # order in the documentation.
-class StickerItemBase(TypedDict):
+class _StickerItemBase(TypedDict):
     id: Snowflake
     name: str
     format_type: StickerFormatTypes
 
 
 @final
-class StickerItemData(StickerItemBase):
+class StickerItemData(_StickerItemBase):
     pass
 
 
 # https://discord.com/developers/docs/resources/sticker#sticker-object-sticker-types
 
 
 StickerTypes = Literal[1, 2]
 
 
 # https://discord.com/developers/docs/resources/sticker#sticker-object-sticker-format-types
 
 
-StickerFormatTypes = Literal[1, 2, 3]
+StickerFormatTypes = Literal[1, 2, 3, 4]
 
 
 # https://discord.com/developers/docs/resources/sticker#sticker-object-sticker-structure
 
 
 @final
-class StickerData(StickerItemBase):
+class StickerData(_StickerItemBase):
     pack_id: NotRequired[Snowflake]
     description: Optional[str]
     tags: str
     type: StickerTypes
     available: NotRequired[bool]
     guild_id: NotRequired[Snowflake]
     user: NotRequired[UserData]
@@ -64,8 +64,8 @@
 class StickerPackData(TypedDict):
     id: Snowflake
     stickers: List[StickerData]
     name: str
     sku_id: Snowflake
     cover_sticker_id: NotRequired[Snowflake]
     description: str
-    banner_asset_id: Snowflake
+    banner_asset_id: NotRequired[Snowflake]
```

### Comparing `discord-typings-0.5.1/discord_typings/resources/voice.py` & `discord_typings-0.6.0/discord_typings/_resources/_voice.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Optional
 
 from typing_extensions import NotRequired, TypedDict, final
 
 if TYPE_CHECKING:
-    from ..reference import Snowflake
-    from .guild import GuildMemberData
+    from .._reference import Snowflake
+    from ._guild import GuildMemberData
 
 __all__ = ('VoiceStateData', 'VoiceRegionData')
 
 
 # https://discord.com/developers/docs/resources/voice#voice-state-object-voice-state-structure
 
 
 @final
 class VoiceStateData(TypedDict):
     guild_id: NotRequired[Snowflake]
     channel_id: Optional[Snowflake]
     user_id: Snowflake
-    member: GuildMemberData
+    member: NotRequired[GuildMemberData]
     session_id: str
     deaf: bool
     mute: bool
     self_deaf: bool
     self_mute: bool
     self_stream: NotRequired[bool]
     self_video: bool
-    seppress: bool
+    suppress: bool
     request_to_speak_timestamp: Optional[str]
 
 
 # https://discord.com/developers/docs/resources/voice#voice-region-object-voice-region-structure
 
 
 @final
```

### Comparing `discord-typings-0.5.1/discord_typings/resources/webhook.py` & `discord_typings-0.6.0/discord_typings/_resources/_webhook.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Optional
 
 from typing_extensions import Literal, NotRequired, TypedDict, final
 
 if TYPE_CHECKING:
-    from ..reference import Snowflake
-    from .channel import PartialChannelData
-    from .guild import GuildData
-    from .user import UserData
+    from .._reference import Snowflake
+    from ._channel import PartialChannelData
+    from ._guild import GuildData
+    from ._user import UserData
 
 __all__ = ('WebhookData', 'WebhookTypes')
 
 
 # https://discord.com/developers/docs/resources/webhook#webhook-object-webhook-structure
```

### Comparing `discord-typings-0.5.1/pyproject.toml` & `discord_typings-0.6.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "discord-typings"
-version = "0.5.1"
-description = "Maintained typings of payloads that Discord sends"
+version = "0.6.0"
+description = "Python typings of payloads that Discord sends"
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [{name = "Bluenix", email = "bluenixdev@gmail.com"}]
 
 keywords = [
     "discord", "discord-api", "discord-api-wrapper", "python-3", "typing"
@@ -20,14 +20,16 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 
 # Generic TypedDicts were first added in 4.3, but possible on Python 3.9 and
 # 3.10 back in 4.2
```

