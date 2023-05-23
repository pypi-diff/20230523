# Comparing `tmp/rekuest-0.1.8.tar.gz` & `tmp/rekuest-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rekuest-0.1.8.tar", max compression
+gzip compressed data, was "rekuest-0.1.9.tar", max compression
```

## Comparing `rekuest-0.1.8.tar` & `rekuest-0.1.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     1517 2022-12-12 13:50:52.137107 rekuest-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       22 2022-08-25 12:20:46.369966 rekuest-0.1.8/rekuest/__init__.py
--rw-r--r--   0        0        0        1 2022-08-25 10:31:18.596463 rekuest-0.1.8/rekuest/actors/__init__.py
--rw-r--r--   0        0        0     3586 2022-12-12 13:46:33.108527 rekuest-0.1.8/rekuest/actors/actify.py
--rw-r--r--   0        0        0     7031 2022-12-06 17:30:19.488474 rekuest-0.1.8/rekuest/actors/base.py
--rw-r--r--   0        0        0      613 2022-12-05 15:15:47.261117 rekuest-0.1.8/rekuest/actors/builder.py
--rw-r--r--   0        0        0     1603 2022-12-05 14:32:45.913282 rekuest-0.1.8/rekuest/actors/contexts.py
--rw-r--r--   0        0        0      362 2022-12-05 13:19:02.249265 rekuest-0.1.8/rekuest/actors/errors.py
--rw-r--r--   0        0        0    12906 2022-12-06 17:34:36.992666 rekuest-0.1.8/rekuest/actors/functional.py
--rw-r--r--   0        0        0     1263 2022-12-05 14:39:02.873555 rekuest-0.1.8/rekuest/actors/helper.py
--rw-r--r--   0        0        0        0 2022-12-01 15:45:42.916521 rekuest-0.1.8/rekuest/actors/reactive/__init__.py
--rw-r--r--   0        0        0     1247 2022-12-05 15:05:17.796217 rekuest-0.1.8/rekuest/actors/reactive/api.py
--rw-r--r--   0        0        0      896 2022-12-05 13:19:57.921368 rekuest-0.1.8/rekuest/actors/vars.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.624462 rekuest-0.1.8/rekuest/agents/__init__.py
--rw-r--r--   0        0        0     6054 2022-12-05 15:15:16.293077 rekuest-0.1.8/rekuest/agents/base.py
--rw-r--r--   0        0        0      220 2022-08-25 10:31:18.632462 rekuest-0.1.8/rekuest/agents/errors.py
--rw-r--r--   0        0        0     3249 2022-08-25 10:35:28.798383 rekuest-0.1.8/rekuest/agents/stateful.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.632462 rekuest-0.1.8/rekuest/agents/transport/__init__.py
--rw-r--r--   0        0        0     3175 2022-09-27 09:09:22.881016 rekuest-0.1.8/rekuest/agents/transport/base.py
--rw-r--r--   0        0        0      461 2022-08-25 10:34:32.742780 rekuest-0.1.8/rekuest/agents/transport/errors.py
--rw-r--r--   0        0        0     2782 2022-12-02 15:00:09.037818 rekuest-0.1.8/rekuest/agents/transport/mock.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.636462 rekuest-0.1.8/rekuest/agents/transport/protocols/__init__.py
--rw-r--r--   0        0        0     3653 2022-12-01 15:23:53.003087 rekuest-0.1.8/rekuest/agents/transport/protocols/agent_json.py
--rw-r--r--   0        0        0    10082 2022-11-23 16:04:14.281104 rekuest-0.1.8/rekuest/agents/transport/websocket.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.656462 rekuest-0.1.8/rekuest/api/__init__.py
--rw-r--r--   0        0        0    67401 2022-12-12 10:58:02.194161 rekuest-0.1.8/rekuest/api/schema.py
--rw-r--r--   0        0        0     1271 2022-10-20 14:03:19.356166 rekuest-0.1.8/rekuest/contrib/fakts/websocket_agent_transport.py
--rw-r--r--   0        0        0     1211 2022-08-25 12:29:20.810549 rekuest-0.1.8/rekuest/contrib/fakts/websocket_postman_transport.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.728461 rekuest-0.1.8/rekuest/definition/__init__.py
--rw-r--r--   0        0        0    19776 2022-12-12 13:50:51.045105 rekuest-0.1.8/rekuest/definition/define.py
--rw-r--r--   0        0        0      249 2022-12-05 15:08:46.848542 rekuest-0.1.8/rekuest/definition/errors.py
--rw-r--r--   0        0        0     6774 2022-12-12 13:41:25.791605 rekuest-0.1.8/rekuest/definition/registry.py
--rw-r--r--   0        0        0      646 2022-12-05 15:05:49.416268 rekuest-0.1.8/rekuest/definition/validate.py
--rw-r--r--   0        0        0       90 2022-11-30 13:49:18.470756 rekuest-0.1.8/rekuest/errors.py
--rw-r--r--   0        0        0      920 2022-08-25 10:47:01.999333 rekuest-0.1.8/rekuest/funcs.py
--rw-r--r--   0        0        0     2095 2022-12-05 17:05:20.434796 rekuest-0.1.8/rekuest/messages.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.744461 rekuest-0.1.8/rekuest/postmans/__init__.py
--rw-r--r--   0        0        0      643 2022-12-05 16:17:31.519175 rekuest-0.1.8/rekuest/postmans/base.py
--rw-r--r--   0        0        0      151 2022-12-01 14:49:59.808507 rekuest-0.1.8/rekuest/postmans/errors.py
--rw-r--r--   0        0        0     8723 2022-09-23 09:25:56.259978 rekuest-0.1.8/rekuest/postmans/graphql.py
--rw-r--r--   0        0        0     4298 2022-12-05 16:54:26.530043 rekuest-0.1.8/rekuest/postmans/stateful.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.748461 rekuest-0.1.8/rekuest/postmans/transport/__init__.py
--rw-r--r--   0        0        0     1280 2022-12-05 16:39:10.928875 rekuest-0.1.8/rekuest/postmans/transport/base.py
--rw-r--r--   0        0        0     1021 2022-08-25 10:49:34.430923 rekuest-0.1.8/rekuest/postmans/transport/errors.py
--rw-r--r--   0        0        0     8087 2022-12-05 17:08:29.899229 rekuest-0.1.8/rekuest/postmans/transport/mock.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.748461 rekuest-0.1.8/rekuest/postmans/transport/protocols/__init__.py
--rw-r--r--   0        0        0     4991 2022-12-05 16:58:37.734336 rekuest-0.1.8/rekuest/postmans/transport/protocols/postman_json.py
--rw-r--r--   0        0        0    10175 2022-08-25 10:49:28.822937 rekuest-0.1.8/rekuest/postmans/transport/websocket.py
--rw-r--r--   0        0        0    21597 2022-12-06 14:29:03.394722 rekuest-0.1.8/rekuest/postmans/utils.py
--rw-r--r--   0        0        0      186 2022-08-25 10:31:18.752461 rekuest-0.1.8/rekuest/postmans/vars.py
--rw-r--r--   0        0        0        0 2022-08-25 11:16:08.136616 rekuest-0.1.8/rekuest/qt/__init__.py
--rw-r--r--   0        0        0     4121 2022-12-06 17:36:21.501006 rekuest-0.1.8/rekuest/qt/builders.py
--rw-r--r--   0        0        0     1268 2022-11-21 13:26:05.412588 rekuest-0.1.8/rekuest/rath.py
--rw-r--r--   0        0        0     2544 2022-12-05 14:15:28.460731 rekuest-0.1.8/rekuest/rekuest.py
--rw-r--r--   0        0        0     3498 2022-12-01 15:36:15.091875 rekuest-0.1.8/rekuest/scalars.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.792461 rekuest-0.1.8/rekuest/structures/__init__.py
--rw-r--r--   0        0        0     2181 2022-11-28 14:20:15.138457 rekuest-0.1.8/rekuest/structures/annotations.py
--rw-r--r--   0        0        0      587 2022-11-28 12:45:12.088963 rekuest-0.1.8/rekuest/structures/builder.py
--rw-r--r--   0        0        0      814 2022-11-28 12:16:43.444977 rekuest-0.1.8/rekuest/structures/default.py
--rw-r--r--   0        0        0     1180 2022-11-30 13:50:37.642886 rekuest-0.1.8/rekuest/structures/errors.py
--rw-r--r--   0        0        0     9294 2022-11-21 09:42:40.677788 rekuest-0.1.8/rekuest/structures/registry.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.796461 rekuest-0.1.8/rekuest/structures/serialization/__init__.py
--rw-r--r--   0        0        0     7918 2022-12-12 11:04:10.482091 rekuest-0.1.8/rekuest/structures/serialization/actor.py
--rw-r--r--   0        0        0     8427 2022-11-30 13:28:41.156812 rekuest-0.1.8/rekuest/structures/serialization/postman.py
--rw-r--r--   0        0        0     4010 2022-11-30 12:57:40.854191 rekuest-0.1.8/rekuest/structures/serialization/utils.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.808461 rekuest-0.1.8/rekuest/traits/__init__.py
--rw-r--r--   0        0        0     1647 2022-08-25 10:31:18.808461 rekuest-0.1.8/rekuest/traits/node.py
--rw-r--r--   0        0        0     5290 2022-12-06 10:25:13.668992 rekuest-0.1.8/rekuest/traits/ports.py
--rw-r--r--   0        0        0      741 2022-12-01 15:45:42.916521 rekuest-0.1.8/rekuest/utils.py
--rw-r--r--   0        0        0      705 2022-11-30 13:48:53.622714 rekuest-0.1.8/rekuest/widgets.py
--rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 rekuest-0.1.8/setup.py
--rw-r--r--   0        0        0      842 1970-01-01 00:00:00.000000 rekuest-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1517 2022-12-12 13:51:24.301171 rekuest-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       22 2022-08-25 12:20:46.369966 rekuest-0.1.9/rekuest/__init__.py
+-rw-r--r--   0        0        0        1 2022-08-25 10:31:18.596463 rekuest-0.1.9/rekuest/actors/__init__.py
+-rw-r--r--   0        0        0     3586 2022-12-12 13:46:33.108527 rekuest-0.1.9/rekuest/actors/actify.py
+-rw-r--r--   0        0        0     7031 2022-12-06 17:30:19.488474 rekuest-0.1.9/rekuest/actors/base.py
+-rw-r--r--   0        0        0      613 2022-12-05 15:15:47.261117 rekuest-0.1.9/rekuest/actors/builder.py
+-rw-r--r--   0        0        0     1603 2022-12-05 14:32:45.913282 rekuest-0.1.9/rekuest/actors/contexts.py
+-rw-r--r--   0        0        0      362 2022-12-05 13:19:02.249265 rekuest-0.1.9/rekuest/actors/errors.py
+-rw-r--r--   0        0        0    12906 2022-12-06 17:34:36.992666 rekuest-0.1.9/rekuest/actors/functional.py
+-rw-r--r--   0        0        0     1263 2022-12-05 14:39:02.873555 rekuest-0.1.9/rekuest/actors/helper.py
+-rw-r--r--   0        0        0        0 2022-12-01 15:45:42.916521 rekuest-0.1.9/rekuest/actors/reactive/__init__.py
+-rw-r--r--   0        0        0     1247 2022-12-05 15:05:17.796217 rekuest-0.1.9/rekuest/actors/reactive/api.py
+-rw-r--r--   0        0        0      896 2022-12-05 13:19:57.921368 rekuest-0.1.9/rekuest/actors/vars.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.624462 rekuest-0.1.9/rekuest/agents/__init__.py
+-rw-r--r--   0        0        0     6054 2022-12-05 15:15:16.293077 rekuest-0.1.9/rekuest/agents/base.py
+-rw-r--r--   0        0        0      220 2022-08-25 10:31:18.632462 rekuest-0.1.9/rekuest/agents/errors.py
+-rw-r--r--   0        0        0     3249 2022-08-25 10:35:28.798383 rekuest-0.1.9/rekuest/agents/stateful.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.632462 rekuest-0.1.9/rekuest/agents/transport/__init__.py
+-rw-r--r--   0        0        0     3175 2022-09-27 09:09:22.881016 rekuest-0.1.9/rekuest/agents/transport/base.py
+-rw-r--r--   0        0        0      461 2022-08-25 10:34:32.742780 rekuest-0.1.9/rekuest/agents/transport/errors.py
+-rw-r--r--   0        0        0     2782 2022-12-02 15:00:09.037818 rekuest-0.1.9/rekuest/agents/transport/mock.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.636462 rekuest-0.1.9/rekuest/agents/transport/protocols/__init__.py
+-rw-r--r--   0        0        0     3653 2022-12-01 15:23:53.003087 rekuest-0.1.9/rekuest/agents/transport/protocols/agent_json.py
+-rw-r--r--   0        0        0    10082 2022-11-23 16:04:14.281104 rekuest-0.1.9/rekuest/agents/transport/websocket.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.656462 rekuest-0.1.9/rekuest/api/__init__.py
+-rw-r--r--   0        0        0    67401 2022-12-12 10:58:02.194161 rekuest-0.1.9/rekuest/api/schema.py
+-rw-r--r--   0        0        0     1271 2022-10-20 14:03:19.356166 rekuest-0.1.9/rekuest/contrib/fakts/websocket_agent_transport.py
+-rw-r--r--   0        0        0     1211 2022-08-25 12:29:20.810549 rekuest-0.1.9/rekuest/contrib/fakts/websocket_postman_transport.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.728461 rekuest-0.1.9/rekuest/definition/__init__.py
+-rw-r--r--   0        0        0    19717 2022-12-12 13:51:14.385152 rekuest-0.1.9/rekuest/definition/define.py
+-rw-r--r--   0        0        0      249 2022-12-05 15:08:46.848542 rekuest-0.1.9/rekuest/definition/errors.py
+-rw-r--r--   0        0        0     6774 2022-12-12 13:41:25.791605 rekuest-0.1.9/rekuest/definition/registry.py
+-rw-r--r--   0        0        0      646 2022-12-05 15:05:49.416268 rekuest-0.1.9/rekuest/definition/validate.py
+-rw-r--r--   0        0        0       90 2022-11-30 13:49:18.470756 rekuest-0.1.9/rekuest/errors.py
+-rw-r--r--   0        0        0      920 2022-08-25 10:47:01.999333 rekuest-0.1.9/rekuest/funcs.py
+-rw-r--r--   0        0        0     2095 2022-12-05 17:05:20.434796 rekuest-0.1.9/rekuest/messages.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.744461 rekuest-0.1.9/rekuest/postmans/__init__.py
+-rw-r--r--   0        0        0      643 2022-12-05 16:17:31.519175 rekuest-0.1.9/rekuest/postmans/base.py
+-rw-r--r--   0        0        0      151 2022-12-01 14:49:59.808507 rekuest-0.1.9/rekuest/postmans/errors.py
+-rw-r--r--   0        0        0     8723 2022-09-23 09:25:56.259978 rekuest-0.1.9/rekuest/postmans/graphql.py
+-rw-r--r--   0        0        0     4298 2022-12-05 16:54:26.530043 rekuest-0.1.9/rekuest/postmans/stateful.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.748461 rekuest-0.1.9/rekuest/postmans/transport/__init__.py
+-rw-r--r--   0        0        0     1280 2022-12-05 16:39:10.928875 rekuest-0.1.9/rekuest/postmans/transport/base.py
+-rw-r--r--   0        0        0     1021 2022-08-25 10:49:34.430923 rekuest-0.1.9/rekuest/postmans/transport/errors.py
+-rw-r--r--   0        0        0     8087 2022-12-05 17:08:29.899229 rekuest-0.1.9/rekuest/postmans/transport/mock.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.748461 rekuest-0.1.9/rekuest/postmans/transport/protocols/__init__.py
+-rw-r--r--   0        0        0     4991 2022-12-05 16:58:37.734336 rekuest-0.1.9/rekuest/postmans/transport/protocols/postman_json.py
+-rw-r--r--   0        0        0    10175 2022-08-25 10:49:28.822937 rekuest-0.1.9/rekuest/postmans/transport/websocket.py
+-rw-r--r--   0        0        0    21597 2022-12-06 14:29:03.394722 rekuest-0.1.9/rekuest/postmans/utils.py
+-rw-r--r--   0        0        0      186 2022-08-25 10:31:18.752461 rekuest-0.1.9/rekuest/postmans/vars.py
+-rw-r--r--   0        0        0        0 2022-08-25 11:16:08.136616 rekuest-0.1.9/rekuest/qt/__init__.py
+-rw-r--r--   0        0        0     4121 2022-12-06 17:36:21.501006 rekuest-0.1.9/rekuest/qt/builders.py
+-rw-r--r--   0        0        0     1268 2022-11-21 13:26:05.412588 rekuest-0.1.9/rekuest/rath.py
+-rw-r--r--   0        0        0     2544 2022-12-05 14:15:28.460731 rekuest-0.1.9/rekuest/rekuest.py
+-rw-r--r--   0        0        0     3498 2022-12-01 15:36:15.091875 rekuest-0.1.9/rekuest/scalars.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.792461 rekuest-0.1.9/rekuest/structures/__init__.py
+-rw-r--r--   0        0        0     2181 2022-11-28 14:20:15.138457 rekuest-0.1.9/rekuest/structures/annotations.py
+-rw-r--r--   0        0        0      587 2022-11-28 12:45:12.088963 rekuest-0.1.9/rekuest/structures/builder.py
+-rw-r--r--   0        0        0      814 2022-11-28 12:16:43.444977 rekuest-0.1.9/rekuest/structures/default.py
+-rw-r--r--   0        0        0     1180 2022-11-30 13:50:37.642886 rekuest-0.1.9/rekuest/structures/errors.py
+-rw-r--r--   0        0        0     9294 2022-11-21 09:42:40.677788 rekuest-0.1.9/rekuest/structures/registry.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.796461 rekuest-0.1.9/rekuest/structures/serialization/__init__.py
+-rw-r--r--   0        0        0     7918 2022-12-12 11:04:10.482091 rekuest-0.1.9/rekuest/structures/serialization/actor.py
+-rw-r--r--   0        0        0     8427 2022-11-30 13:28:41.156812 rekuest-0.1.9/rekuest/structures/serialization/postman.py
+-rw-r--r--   0        0        0     4010 2022-11-30 12:57:40.854191 rekuest-0.1.9/rekuest/structures/serialization/utils.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.808461 rekuest-0.1.9/rekuest/traits/__init__.py
+-rw-r--r--   0        0        0     1647 2022-08-25 10:31:18.808461 rekuest-0.1.9/rekuest/traits/node.py
+-rw-r--r--   0        0        0     5290 2022-12-06 10:25:13.668992 rekuest-0.1.9/rekuest/traits/ports.py
+-rw-r--r--   0        0        0      741 2022-12-01 15:45:42.916521 rekuest-0.1.9/rekuest/utils.py
+-rw-r--r--   0        0        0      705 2022-11-30 13:48:53.622714 rekuest-0.1.9/rekuest/widgets.py
+-rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 rekuest-0.1.9/setup.py
+-rw-r--r--   0        0        0      842 1970-01-01 00:00:00.000000 rekuest-0.1.9/PKG-INFO
```

### Comparing `rekuest-0.1.8/pyproject.toml` & `rekuest-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rekuest"
-version = "0.1.8"
+version = "0.1.9"
 description = "rpc and node backbone"
 authors = ["jhnnsrs <jhnnsrs@gmail.com>"]
 license = "CC BY-NC 3.0"
 packages = [{ include = "rekuest" }]
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `rekuest-0.1.8/rekuest/actors/actify.py` & `rekuest-0.1.9/rekuest/actors/actify.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/actors/base.py` & `rekuest-0.1.9/rekuest/actors/base.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/actors/builder.py` & `rekuest-0.1.9/rekuest/actors/builder.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/actors/contexts.py` & `rekuest-0.1.9/rekuest/actors/contexts.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/actors/functional.py` & `rekuest-0.1.9/rekuest/actors/functional.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/actors/helper.py` & `rekuest-0.1.9/rekuest/actors/helper.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/actors/reactive/api.py` & `rekuest-0.1.9/rekuest/actors/reactive/api.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/actors/vars.py` & `rekuest-0.1.9/rekuest/actors/vars.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/agents/base.py` & `rekuest-0.1.9/rekuest/agents/base.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/agents/stateful.py` & `rekuest-0.1.9/rekuest/agents/stateful.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/agents/transport/base.py` & `rekuest-0.1.9/rekuest/agents/transport/base.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/agents/transport/mock.py` & `rekuest-0.1.9/rekuest/agents/transport/mock.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/agents/transport/protocols/agent_json.py` & `rekuest-0.1.9/rekuest/agents/transport/protocols/agent_json.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/agents/transport/websocket.py` & `rekuest-0.1.9/rekuest/agents/transport/websocket.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/api/schema.py` & `rekuest-0.1.9/rekuest/api/schema.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/contrib/fakts/websocket_agent_transport.py` & `rekuest-0.1.9/rekuest/contrib/fakts/websocket_agent_transport.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/contrib/fakts/websocket_postman_transport.py` & `rekuest-0.1.9/rekuest/contrib/fakts/websocket_postman_transport.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/definition/define.py` & `rekuest-0.1.9/rekuest/definition/define.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,20 +300,17 @@
                 key=key,
                 default=default,
                 nullable=nullable,
                 annotations=annotations,
                 description=description,
             )
 
-    print(widget)
-
     identifier = registry.get_identifier_for_structure(cls)
     default_converter = registry.get_default_converter_for_structure(cls)
     widget = widget or registry.get_widget_input(cls)
-    print(widget)
 
     return ArgPortInput(
         kind=PortKindInput.STRUCTURE,
         identifier=identifier,
         widget=widget,
         key=key,
         default=default_converter(default) if default else None,
@@ -510,15 +507,14 @@
         if omitlast is not None and index > omitlast:
             continue
         if key in omitkeys:
             continue
 
         widget = widgets.get(key, None)
         cls = value.annotation
-        print(widget)
 
         try:
             args.append(
                 convert_argument_to_port(
                     cls,
                     key,
                     structure_registry,
```

### Comparing `rekuest-0.1.8/rekuest/definition/registry.py` & `rekuest-0.1.9/rekuest/definition/registry.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/definition/validate.py` & `rekuest-0.1.9/rekuest/definition/validate.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/funcs.py` & `rekuest-0.1.9/rekuest/funcs.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/messages.py` & `rekuest-0.1.9/rekuest/messages.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/postmans/base.py` & `rekuest-0.1.9/rekuest/postmans/base.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/postmans/graphql.py` & `rekuest-0.1.9/rekuest/postmans/graphql.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/postmans/stateful.py` & `rekuest-0.1.9/rekuest/postmans/stateful.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/postmans/transport/base.py` & `rekuest-0.1.9/rekuest/postmans/transport/base.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/postmans/transport/errors.py` & `rekuest-0.1.9/rekuest/postmans/transport/errors.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/postmans/transport/mock.py` & `rekuest-0.1.9/rekuest/postmans/transport/mock.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/postmans/transport/protocols/postman_json.py` & `rekuest-0.1.9/rekuest/postmans/transport/protocols/postman_json.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/postmans/transport/websocket.py` & `rekuest-0.1.9/rekuest/postmans/transport/websocket.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/postmans/utils.py` & `rekuest-0.1.9/rekuest/postmans/utils.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/qt/builders.py` & `rekuest-0.1.9/rekuest/qt/builders.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/rath.py` & `rekuest-0.1.9/rekuest/rath.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/rekuest.py` & `rekuest-0.1.9/rekuest/rekuest.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/scalars.py` & `rekuest-0.1.9/rekuest/scalars.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/structures/annotations.py` & `rekuest-0.1.9/rekuest/structures/annotations.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/structures/builder.py` & `rekuest-0.1.9/rekuest/structures/builder.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/structures/default.py` & `rekuest-0.1.9/rekuest/structures/default.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/structures/errors.py` & `rekuest-0.1.9/rekuest/structures/errors.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/structures/registry.py` & `rekuest-0.1.9/rekuest/structures/registry.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/structures/serialization/actor.py` & `rekuest-0.1.9/rekuest/structures/serialization/actor.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/structures/serialization/postman.py` & `rekuest-0.1.9/rekuest/structures/serialization/postman.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/structures/serialization/utils.py` & `rekuest-0.1.9/rekuest/structures/serialization/utils.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/traits/node.py` & `rekuest-0.1.9/rekuest/traits/node.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/traits/ports.py` & `rekuest-0.1.9/rekuest/traits/ports.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/utils.py` & `rekuest-0.1.9/rekuest/utils.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/rekuest/widgets.py` & `rekuest-0.1.9/rekuest/widgets.py`

 * *Files identical despite different names*

### Comparing `rekuest-0.1.8/setup.py` & `rekuest-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
  'pytest-aiohttp>=1.0.4,<2.0.0',
  'pytest-asyncio>=0.20.2,<0.21.0',
  'rath>=0.3.4',
  'websockets>=10.0,<11.0']
 
 setup_kwargs = {
     'name': 'rekuest',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'rpc and node backbone',
     'long_description': 'None',
     'author': 'jhnnsrs',
     'author_email': 'jhnnsrs@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `rekuest-0.1.8/PKG-INFO` & `rekuest-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rekuest
-Version: 0.1.8
+Version: 0.1.9
 Summary: rpc and node backbone
 License: CC BY-NC 3.0
 Author: jhnnsrs
 Author-email: jhnnsrs@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

