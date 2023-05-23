# Comparing `tmp/miniworldmaker-2.8.0.0.tar.gz` & `tmp/miniworldmaker-2.9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniworldmaker-2.8.0.0.tar", last modified: Mon Jun 13 14:22:26 2022, max compression
+gzip compressed data, was "miniworldmaker-2.9.0.0.tar", last modified: Mon Jun 20 21:26:19 2022, max compression
```

## Comparing `miniworldmaker-2.8.0.0.tar` & `miniworldmaker-2.9.0.0.tar`

### file list

```diff
@@ -1,141 +1,142 @@
-drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-13 14:22:26.746848 miniworldmaker-2.8.0.0/
--rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)     1060 2022-03-01 12:28:39.000000 miniworldmaker-2.8.0.0/LICENSE.txt
--rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)       38 2022-03-01 12:28:39.000000 miniworldmaker-2.8.0.0/MANIFEST.in
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3630 2022-06-13 14:22:26.746848 miniworldmaker-2.8.0.0/PKG-INFO
--rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)     2980 2022-04-20 14:55:08.000000 miniworldmaker-2.8.0.0/README.md
-drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-13 14:22:26.733514 miniworldmaker-2.8.0.0/miniworldmaker/
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     5643 2022-05-20 05:11:20.000000 miniworldmaker-2.8.0.0/miniworldmaker/__init__.py
-drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-13 14:22:26.736848 miniworldmaker-2.8.0.0/miniworldmaker/appearances/
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/appearances/__init__.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)    20407 2022-06-13 06:18:06.000000 miniworldmaker-2.8.0.0/miniworldmaker/appearances/appearance.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     6935 2022-06-13 06:19:45.000000 miniworldmaker-2.8.0.0/miniworldmaker/appearances/appearance_base.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     9561 2022-06-13 06:37:12.000000 miniworldmaker-2.8.0.0/miniworldmaker/appearances/appearances_manager.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     5125 2022-06-13 13:42:39.000000 miniworldmaker-2.8.0.0/miniworldmaker/appearances/background.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1405 2022-06-12 15:54:50.000000 miniworldmaker-2.8.0.0/miniworldmaker/appearances/backgrounds_manager.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     4310 2022-06-13 06:20:59.000000 miniworldmaker-2.8.0.0/miniworldmaker/appearances/costume.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     2335 2022-06-12 15:55:45.000000 miniworldmaker-2.8.0.0/miniworldmaker/appearances/costumes_manager.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1893 2022-06-11 09:32:46.000000 miniworldmaker-2.8.0.0/miniworldmaker/appearances/hex_costume.py
-drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-13 14:22:26.736848 miniworldmaker-2.8.0.0/miniworldmaker/appearances/managers/
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/appearances/managers/__init__.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1227 2022-04-18 05:11:46.000000 miniworldmaker-2.8.0.0/miniworldmaker/appearances/managers/font_manager.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)      674 2022-04-18 05:11:50.000000 miniworldmaker-2.8.0.0/miniworldmaker/appearances/managers/image_background_manager.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)    10412 2022-06-13 06:40:23.000000 miniworldmaker-2.8.0.0/miniworldmaker/appearances/managers/image_manager.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1184 2022-04-18 05:11:58.000000 miniworldmaker-2.8.0.0/miniworldmaker/appearances/managers/transformations_background_manager.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1026 2022-04-18 05:12:02.000000 miniworldmaker-2.8.0.0/miniworldmaker/appearances/managers/transformations_costume_manager.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)    10439 2022-04-12 08:04:24.000000 miniworldmaker-2.8.0.0/miniworldmaker/appearances/managers/transformations_manager.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     4600 2022-06-10 11:52:04.000000 miniworldmaker-2.8.0.0/miniworldmaker/appearances/shape_costume.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1088 2022-06-10 13:34:05.000000 miniworldmaker-2.8.0.0/miniworldmaker/appearances/text_costume.py
-drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-13 14:22:26.736848 miniworldmaker-2.8.0.0/miniworldmaker/base/
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/base/__init__.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3843 2022-04-18 05:12:15.000000 miniworldmaker-2.8.0.0/miniworldmaker/base/app.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3811 2022-04-18 05:12:21.000000 miniworldmaker-2.8.0.0/miniworldmaker/base/container_manager.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     4234 2022-05-22 11:21:22.000000 miniworldmaker-2.8.0.0/miniworldmaker/base/event_manager.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     2653 2022-05-16 18:43:23.000000 miniworldmaker-2.8.0.0/miniworldmaker/base/file_manager.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1218 2022-04-18 05:12:35.000000 miniworldmaker-2.8.0.0/miniworldmaker/base/sound_manager.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3613 2022-04-30 10:52:49.000000 miniworldmaker-2.8.0.0/miniworldmaker/base/window.py
-drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-13 14:22:26.736848 miniworldmaker-2.8.0.0/miniworldmaker/board_positions/
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/board_positions/__init__.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3525 2022-05-10 09:38:26.000000 miniworldmaker-2.8.0.0/miniworldmaker/board_positions/board_direction.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     4031 2022-05-14 09:39:53.000000 miniworldmaker-2.8.0.0/miniworldmaker/board_positions/board_position.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)      973 2022-04-24 12:16:39.000000 miniworldmaker-2.8.0.0/miniworldmaker/board_positions/board_rect.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)    10044 2022-05-10 18:51:53.000000 miniworldmaker-2.8.0.0/miniworldmaker/board_positions/board_vector.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     9976 2022-05-11 08:03:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/board_positions/hex_elements.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     9388 2022-05-11 08:03:21.000000 miniworldmaker-2.8.0.0/miniworldmaker/board_positions/tile_elements.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)      505 2022-04-22 07:00:18.000000 miniworldmaker-2.8.0.0/miniworldmaker/board_positions/tile_factory.py
-drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-13 14:22:26.740181 miniworldmaker-2.8.0.0/miniworldmaker/boards/
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-04-18 04:46:33.000000 miniworldmaker-2.8.0.0/miniworldmaker/boards/__init__.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)    21056 2022-06-09 14:11:20.000000 miniworldmaker-2.8.0.0/miniworldmaker/boards/board.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)    13739 2022-06-10 09:40:38.000000 miniworldmaker-2.8.0.0/miniworldmaker/boards/board_base.py
-drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-13 14:22:26.740181 miniworldmaker-2.8.0.0/miniworldmaker/boards/board_manager/
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/boards/board_manager/__init__.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3886 2022-04-23 06:03:20.000000 miniworldmaker-2.8.0.0/miniworldmaker/boards/board_manager/board_collision_manager.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     9762 2022-06-13 06:31:32.000000 miniworldmaker-2.8.0.0/miniworldmaker/boards/board_manager/board_event_manager.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)      964 2022-05-02 10:39:21.000000 miniworldmaker-2.8.0.0/miniworldmaker/boards/board_manager/board_mouse_manager.py
-drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-13 14:22:26.740181 miniworldmaker-2.8.0.0/miniworldmaker/boards/data/
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/boards/data/__init__.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1169 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/boards/data/db_manager.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     2947 2022-04-24 05:47:29.000000 miniworldmaker-2.8.0.0/miniworldmaker/boards/data/export_factory.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     2284 2022-04-18 05:13:53.000000 miniworldmaker-2.8.0.0/miniworldmaker/boards/data/import_factory.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     6485 2022-05-11 04:53:27.000000 miniworldmaker-2.8.0.0/miniworldmaker/boards/hex_board.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)    10025 2022-05-02 09:49:33.000000 miniworldmaker-2.8.0.0/miniworldmaker/boards/physics_board.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)       86 2022-04-18 05:16:45.000000 miniworldmaker-2.8.0.0/miniworldmaker/boards/pixel_board.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)    15614 2022-05-23 10:43:55.000000 miniworldmaker-2.8.0.0/miniworldmaker/boards/tiled_board.py
-drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-13 14:22:26.740181 miniworldmaker-2.8.0.0/miniworldmaker/boards/token_connectors/
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/boards/token_connectors/__init__.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)      859 2022-06-09 15:12:07.000000 miniworldmaker-2.8.0.0/miniworldmaker/boards/token_connectors/hex_board_connector.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     2093 2022-06-09 15:09:11.000000 miniworldmaker-2.8.0.0/miniworldmaker/boards/token_connectors/physics_board_connector.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)      694 2022-06-09 12:13:13.000000 miniworldmaker-2.8.0.0/miniworldmaker/boards/token_connectors/pixel_board_connector.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1805 2022-06-09 12:09:26.000000 miniworldmaker-2.8.0.0/miniworldmaker/boards/token_connectors/tiled_board_connector.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3318 2022-06-13 06:36:21.000000 miniworldmaker-2.8.0.0/miniworldmaker/boards/token_connectors/token_connector.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)       66 2022-04-18 05:08:27.000000 miniworldmaker-2.8.0.0/miniworldmaker/conf.py
-drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-13 14:22:26.740181 miniworldmaker-2.8.0.0/miniworldmaker/containers/
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/containers/__init__.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)    10046 2022-04-18 05:17:09.000000 miniworldmaker-2.8.0.0/miniworldmaker/containers/actionbar.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)      981 2022-05-16 08:48:41.000000 miniworldmaker-2.8.0.0/miniworldmaker/containers/color_toolbar.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)      995 2022-05-20 07:20:50.000000 miniworldmaker-2.8.0.0/miniworldmaker/containers/console.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3466 2022-05-19 06:47:44.000000 miniworldmaker-2.8.0.0/miniworldmaker/containers/container.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)      570 2022-04-18 05:17:28.000000 miniworldmaker-2.8.0.0/miniworldmaker/containers/event_console.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     4570 2022-06-11 09:22:38.000000 miniworldmaker-2.8.0.0/miniworldmaker/containers/inspect_actor_toolbar.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     6227 2022-06-11 09:23:06.000000 miniworldmaker-2.8.0.0/miniworldmaker/containers/level_designer_toolbar.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     9320 2022-05-22 11:22:31.000000 miniworldmaker-2.8.0.0/miniworldmaker/containers/toolbar.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)    16250 2022-06-13 06:31:32.000000 miniworldmaker-2.8.0.0/miniworldmaker/containers/widgets.py
-drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-13 14:22:26.740181 miniworldmaker-2.8.0.0/miniworldmaker/dialogs/
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/dialogs/__init__.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1410 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/dialogs/ask.py
-drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-13 14:22:26.743514 miniworldmaker-2.8.0.0/miniworldmaker/exceptions/
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/exceptions/__init__.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     7100 2022-06-10 09:41:52.000000 miniworldmaker-2.8.0.0/miniworldmaker/exceptions/miniworldmaker_exception.py
-drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-13 14:22:26.743514 miniworldmaker-2.8.0.0/miniworldmaker/resources/
--rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)     1343 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/resources/down.png
--rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)     1021 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/resources/left.png
--rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)     8231 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/resources/logo_big.png
--rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)     7774 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/resources/logo_small.png
--rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)     3978 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/resources/logo_small_32.png
--rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)      473 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/resources/pause.png
--rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)      448 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/resources/play.png
--rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)     1408 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/resources/question.png
--rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)      434 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/resources/reset.png
--rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)     1011 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/resources/right.png
--rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)      468 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/resources/run.png
--rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)     1358 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/resources/up.png
-drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-13 14:22:26.743514 miniworldmaker-2.8.0.0/miniworldmaker/tokens/
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/tokens/__init__.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     2234 2022-04-27 05:59:34.000000 miniworldmaker-2.8.0.0/miniworldmaker/tokens/number_token.py
-drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-13 14:22:26.743514 miniworldmaker-2.8.0.0/miniworldmaker/tokens/physics/
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/tokens/physics/__init__.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)    18192 2022-04-23 18:15:09.000000 miniworldmaker-2.8.0.0/miniworldmaker/tokens/physics/token_physics.py
-drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-13 14:22:26.743514 miniworldmaker-2.8.0.0/miniworldmaker/tokens/positions/
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/tokens/positions/__init__.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3591 2022-06-09 12:18:18.000000 miniworldmaker-2.8.0.0/miniworldmaker/tokens/positions/token_hex_position_manager.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3676 2022-06-09 12:17:49.000000 miniworldmaker-2.8.0.0/miniworldmaker/tokens/positions/token_physics_position_manager.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     2060 2022-06-09 12:17:39.000000 miniworldmaker-2.8.0.0/miniworldmaker/tokens/positions/token_pixel_position_manager.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)    12697 2022-06-13 13:15:55.000000 miniworldmaker-2.8.0.0/miniworldmaker/tokens/positions/token_position_manager.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     2618 2022-06-09 12:17:19.000000 miniworldmaker-2.8.0.0/miniworldmaker/tokens/positions/token_tiled_position_manager.py
-drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-13 14:22:26.746848 miniworldmaker-2.8.0.0/miniworldmaker/tokens/sensors/
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/tokens/sensors/__init__.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     6558 2022-06-13 13:14:24.000000 miniworldmaker-2.8.0.0/miniworldmaker/tokens/sensors/token_boardsensor.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     5934 2022-04-28 19:57:44.000000 miniworldmaker-2.8.0.0/miniworldmaker/tokens/sensors/token_pixelboardsensor.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     4449 2022-06-13 13:14:02.000000 miniworldmaker-2.8.0.0/miniworldmaker/tokens/sensors/token_tiledboardsensor.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)    12488 2022-06-09 18:37:29.000000 miniworldmaker-2.8.0.0/miniworldmaker/tokens/shapes.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1832 2022-06-09 19:18:58.000000 miniworldmaker-2.8.0.0/miniworldmaker/tokens/text_token.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)    59443 2022-06-13 13:39:06.000000 miniworldmaker-2.8.0.0/miniworldmaker/tokens/token.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     6215 2022-06-10 09:57:05.000000 miniworldmaker-2.8.0.0/miniworldmaker/tokens/token_base.py
-drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-13 14:22:26.746848 miniworldmaker-2.8.0.0/miniworldmaker/tools/
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/tools/__init__.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)      241 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/tools/binding.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)       99 2022-06-13 06:31:32.000000 miniworldmaker-2.8.0.0/miniworldmaker/tools/board_inspection.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)      415 2022-03-03 16:30:17.000000 miniworldmaker-2.8.0.0/miniworldmaker/tools/color.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1152 2022-06-13 06:30:45.000000 miniworldmaker-2.8.0.0/miniworldmaker/tools/inspection.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1419 2022-03-01 12:28:40.000000 miniworldmaker-2.8.0.0/miniworldmaker/tools/keys.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1366 2022-05-22 11:22:59.000000 miniworldmaker-2.8.0.0/miniworldmaker/tools/method_caller.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3058 2022-05-23 06:17:09.000000 miniworldmaker-2.8.0.0/miniworldmaker/tools/timer.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1863 2022-05-08 18:47:19.000000 miniworldmaker-2.8.0.0/miniworldmaker/tools/token_class_inspection.py
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)      697 2022-06-13 06:31:32.000000 miniworldmaker-2.8.0.0/miniworldmaker/tools/token_inspection.py
-drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-13 14:22:26.733514 miniworldmaker-2.8.0.0/miniworldmaker.egg-info/
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3630 2022-06-13 14:22:26.000000 miniworldmaker-2.8.0.0/miniworldmaker.egg-info/PKG-INFO
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)     5035 2022-06-13 14:22:26.000000 miniworldmaker-2.8.0.0/miniworldmaker.egg-info/SOURCES.txt
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)        1 2022-06-13 14:22:26.000000 miniworldmaker-2.8.0.0/miniworldmaker.egg-info/dependency_links.txt
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)       63 2022-06-13 14:22:26.000000 miniworldmaker-2.8.0.0/miniworldmaker.egg-info/requires.txt
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)       15 2022-06-13 14:22:26.000000 miniworldmaker-2.8.0.0/miniworldmaker.egg-info/top_level.txt
--rw-r--r--   0 asiebel   (1000) asiebel   (1000)       38 2022-06-13 14:22:26.746848 miniworldmaker-2.8.0.0/setup.cfg
--rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)     1388 2022-06-13 14:20:56.000000 miniworldmaker-2.8.0.0/setup.py
+drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-20 21:26:19.213439 miniworldmaker-2.9.0.0/
+-rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)     1060 2022-03-01 12:28:39.000000 miniworldmaker-2.9.0.0/LICENSE.txt
+-rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)       38 2022-03-01 12:28:39.000000 miniworldmaker-2.9.0.0/MANIFEST.in
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3630 2022-06-20 21:26:19.213439 miniworldmaker-2.9.0.0/PKG-INFO
+-rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)     2980 2022-04-20 14:55:08.000000 miniworldmaker-2.9.0.0/README.md
+drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-20 21:26:19.200106 miniworldmaker-2.9.0.0/miniworldmaker/
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     5643 2022-06-16 10:50:20.000000 miniworldmaker-2.9.0.0/miniworldmaker/__init__.py
+drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-20 21:26:19.203439 miniworldmaker-2.9.0.0/miniworldmaker/appearances/
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/appearances/__init__.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)    20725 2022-06-20 19:42:49.000000 miniworldmaker-2.9.0.0/miniworldmaker/appearances/appearance.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     7236 2022-06-20 21:03:13.000000 miniworldmaker-2.9.0.0/miniworldmaker/appearances/appearance_base.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)    11052 2022-06-20 21:18:03.000000 miniworldmaker-2.9.0.0/miniworldmaker/appearances/appearances_manager.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     4666 2022-06-19 12:06:51.000000 miniworldmaker-2.9.0.0/miniworldmaker/appearances/background.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1381 2022-06-20 19:39:35.000000 miniworldmaker-2.9.0.0/miniworldmaker/appearances/backgrounds_manager.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     4617 2022-06-20 20:42:19.000000 miniworldmaker-2.9.0.0/miniworldmaker/appearances/costume.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     2001 2022-06-20 21:05:42.000000 miniworldmaker-2.9.0.0/miniworldmaker/appearances/costumes_manager.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1956 2022-06-20 17:50:02.000000 miniworldmaker-2.9.0.0/miniworldmaker/appearances/hex_costume.py
+drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-20 21:26:19.203439 miniworldmaker-2.9.0.0/miniworldmaker/appearances/managers/
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/appearances/managers/__init__.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1442 2022-06-19 10:28:33.000000 miniworldmaker-2.9.0.0/miniworldmaker/appearances/managers/font_manager.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)      674 2022-04-18 05:11:50.000000 miniworldmaker-2.9.0.0/miniworldmaker/appearances/managers/image_background_manager.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)    10448 2022-06-20 19:59:58.000000 miniworldmaker-2.9.0.0/miniworldmaker/appearances/managers/image_manager.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1182 2022-06-19 12:05:53.000000 miniworldmaker-2.9.0.0/miniworldmaker/appearances/managers/transformations_background_manager.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1026 2022-04-18 05:12:02.000000 miniworldmaker-2.9.0.0/miniworldmaker/appearances/managers/transformations_costume_manager.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)    10946 2022-06-20 18:07:33.000000 miniworldmaker-2.9.0.0/miniworldmaker/appearances/managers/transformations_manager.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     5021 2022-06-20 17:44:24.000000 miniworldmaker-2.9.0.0/miniworldmaker/appearances/shape_costume.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1253 2022-06-20 17:47:10.000000 miniworldmaker-2.9.0.0/miniworldmaker/appearances/text_costume.py
+drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-20 21:26:19.203439 miniworldmaker-2.9.0.0/miniworldmaker/base/
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/base/__init__.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3853 2022-06-18 16:20:38.000000 miniworldmaker-2.9.0.0/miniworldmaker/base/app.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3811 2022-04-18 05:12:21.000000 miniworldmaker-2.9.0.0/miniworldmaker/base/container_manager.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     4234 2022-05-22 11:21:22.000000 miniworldmaker-2.9.0.0/miniworldmaker/base/event_manager.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     2653 2022-06-17 17:29:38.000000 miniworldmaker-2.9.0.0/miniworldmaker/base/file_manager.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1218 2022-04-18 05:12:35.000000 miniworldmaker-2.9.0.0/miniworldmaker/base/sound_manager.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3613 2022-04-30 10:52:49.000000 miniworldmaker-2.9.0.0/miniworldmaker/base/window.py
+drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-20 21:26:19.206772 miniworldmaker-2.9.0.0/miniworldmaker/board_positions/
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/board_positions/__init__.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3737 2022-06-17 15:30:34.000000 miniworldmaker-2.9.0.0/miniworldmaker/board_positions/board_direction.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     4356 2022-06-20 18:01:53.000000 miniworldmaker-2.9.0.0/miniworldmaker/board_positions/board_position.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)      986 2022-06-16 13:08:07.000000 miniworldmaker-2.9.0.0/miniworldmaker/board_positions/board_rect.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)    10044 2022-05-10 18:51:53.000000 miniworldmaker-2.9.0.0/miniworldmaker/board_positions/board_vector.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     9976 2022-05-11 08:03:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/board_positions/hex_elements.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     9388 2022-05-11 08:03:21.000000 miniworldmaker-2.9.0.0/miniworldmaker/board_positions/tile_elements.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)      505 2022-04-22 07:00:18.000000 miniworldmaker-2.9.0.0/miniworldmaker/board_positions/tile_factory.py
+drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-20 21:26:19.206772 miniworldmaker-2.9.0.0/miniworldmaker/boards/
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-04-18 04:46:33.000000 miniworldmaker-2.9.0.0/miniworldmaker/boards/__init__.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)    22235 2022-06-20 18:10:30.000000 miniworldmaker-2.9.0.0/miniworldmaker/boards/board.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)    13090 2022-06-18 23:05:55.000000 miniworldmaker-2.9.0.0/miniworldmaker/boards/board_base.py
+drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-20 21:26:19.206772 miniworldmaker-2.9.0.0/miniworldmaker/boards/board_manager/
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/boards/board_manager/__init__.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     5840 2022-06-20 18:45:49.000000 miniworldmaker-2.9.0.0/miniworldmaker/boards/board_manager/board_camera_manager.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3886 2022-06-17 13:57:14.000000 miniworldmaker-2.9.0.0/miniworldmaker/boards/board_manager/board_collision_manager.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     9762 2022-06-13 06:31:32.000000 miniworldmaker-2.9.0.0/miniworldmaker/boards/board_manager/board_event_manager.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)      964 2022-05-02 10:39:21.000000 miniworldmaker-2.9.0.0/miniworldmaker/boards/board_manager/board_mouse_manager.py
+drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-20 21:26:19.206772 miniworldmaker-2.9.0.0/miniworldmaker/boards/data/
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/boards/data/__init__.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1169 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/boards/data/db_manager.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     2947 2022-04-24 05:47:29.000000 miniworldmaker-2.9.0.0/miniworldmaker/boards/data/export_factory.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     2284 2022-04-18 05:13:53.000000 miniworldmaker-2.9.0.0/miniworldmaker/boards/data/import_factory.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     6308 2022-06-17 14:37:48.000000 miniworldmaker-2.9.0.0/miniworldmaker/boards/hex_board.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)    10025 2022-05-02 09:49:33.000000 miniworldmaker-2.9.0.0/miniworldmaker/boards/physics_board.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)       86 2022-04-18 05:16:45.000000 miniworldmaker-2.9.0.0/miniworldmaker/boards/pixel_board.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)    15633 2022-06-17 14:37:35.000000 miniworldmaker-2.9.0.0/miniworldmaker/boards/tiled_board.py
+drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-20 21:26:19.206772 miniworldmaker-2.9.0.0/miniworldmaker/boards/token_connectors/
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/boards/token_connectors/__init__.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)      859 2022-06-09 15:12:07.000000 miniworldmaker-2.9.0.0/miniworldmaker/boards/token_connectors/hex_board_connector.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     2093 2022-06-09 15:09:11.000000 miniworldmaker-2.9.0.0/miniworldmaker/boards/token_connectors/physics_board_connector.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)      694 2022-06-09 12:13:13.000000 miniworldmaker-2.9.0.0/miniworldmaker/boards/token_connectors/pixel_board_connector.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1633 2022-06-19 09:12:01.000000 miniworldmaker-2.9.0.0/miniworldmaker/boards/token_connectors/tiled_board_connector.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3425 2022-06-20 20:35:11.000000 miniworldmaker-2.9.0.0/miniworldmaker/boards/token_connectors/token_connector.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)       66 2022-04-18 05:08:27.000000 miniworldmaker-2.9.0.0/miniworldmaker/conf.py
+drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-20 21:26:19.210106 miniworldmaker-2.9.0.0/miniworldmaker/containers/
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/containers/__init__.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)    10046 2022-04-18 05:17:09.000000 miniworldmaker-2.9.0.0/miniworldmaker/containers/actionbar.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)      981 2022-05-16 08:48:41.000000 miniworldmaker-2.9.0.0/miniworldmaker/containers/color_toolbar.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)      995 2022-05-20 07:20:50.000000 miniworldmaker-2.9.0.0/miniworldmaker/containers/console.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3466 2022-05-19 06:47:44.000000 miniworldmaker-2.9.0.0/miniworldmaker/containers/container.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)      570 2022-04-18 05:17:28.000000 miniworldmaker-2.9.0.0/miniworldmaker/containers/event_console.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     4570 2022-06-11 09:22:38.000000 miniworldmaker-2.9.0.0/miniworldmaker/containers/inspect_actor_toolbar.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     6227 2022-06-11 09:23:06.000000 miniworldmaker-2.9.0.0/miniworldmaker/containers/level_designer_toolbar.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     9320 2022-05-22 11:22:31.000000 miniworldmaker-2.9.0.0/miniworldmaker/containers/toolbar.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)    16250 2022-06-13 06:31:32.000000 miniworldmaker-2.9.0.0/miniworldmaker/containers/widgets.py
+drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-20 21:26:19.210106 miniworldmaker-2.9.0.0/miniworldmaker/dialogs/
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/dialogs/__init__.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1410 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/dialogs/ask.py
+drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-20 21:26:19.210106 miniworldmaker-2.9.0.0/miniworldmaker/exceptions/
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/exceptions/__init__.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     7100 2022-06-10 09:41:52.000000 miniworldmaker-2.9.0.0/miniworldmaker/exceptions/miniworldmaker_exception.py
+drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-20 21:26:19.210106 miniworldmaker-2.9.0.0/miniworldmaker/resources/
+-rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)     1343 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/resources/down.png
+-rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)     1021 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/resources/left.png
+-rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)     8231 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/resources/logo_big.png
+-rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)     7774 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/resources/logo_small.png
+-rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)     3978 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/resources/logo_small_32.png
+-rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)      473 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/resources/pause.png
+-rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)      448 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/resources/play.png
+-rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)     1408 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/resources/question.png
+-rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)      434 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/resources/reset.png
+-rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)     1011 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/resources/right.png
+-rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)      468 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/resources/run.png
+-rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)     1358 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/resources/up.png
+drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-20 21:26:19.210106 miniworldmaker-2.9.0.0/miniworldmaker/tokens/
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/tokens/__init__.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     2293 2022-06-18 16:12:17.000000 miniworldmaker-2.9.0.0/miniworldmaker/tokens/number_token.py
+drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-20 21:26:19.210106 miniworldmaker-2.9.0.0/miniworldmaker/tokens/physics/
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/tokens/physics/__init__.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)    18307 2022-06-20 17:51:21.000000 miniworldmaker-2.9.0.0/miniworldmaker/tokens/physics/token_physics.py
+drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-20 21:26:19.210106 miniworldmaker-2.9.0.0/miniworldmaker/tokens/positions/
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/tokens/positions/__init__.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3544 2022-06-18 16:12:46.000000 miniworldmaker-2.9.0.0/miniworldmaker/tokens/positions/token_hex_position_manager.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3676 2022-06-09 12:17:49.000000 miniworldmaker-2.9.0.0/miniworldmaker/tokens/positions/token_physics_position_manager.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     2872 2022-06-20 18:35:35.000000 miniworldmaker-2.9.0.0/miniworldmaker/tokens/positions/token_pixel_position_manager.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)    13108 2022-06-20 20:58:24.000000 miniworldmaker-2.9.0.0/miniworldmaker/tokens/positions/token_position_manager.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3176 2022-06-19 09:56:27.000000 miniworldmaker-2.9.0.0/miniworldmaker/tokens/positions/token_tiled_position_manager.py
+drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-20 21:26:19.213439 miniworldmaker-2.9.0.0/miniworldmaker/tokens/sensors/
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/tokens/sensors/__init__.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     6591 2022-06-19 07:44:04.000000 miniworldmaker-2.9.0.0/miniworldmaker/tokens/sensors/token_boardsensor.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     5174 2022-06-19 11:16:04.000000 miniworldmaker-2.9.0.0/miniworldmaker/tokens/sensors/token_pixelboardsensor.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     4449 2022-06-13 13:14:02.000000 miniworldmaker-2.9.0.0/miniworldmaker/tokens/sensors/token_tiledboardsensor.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)    11794 2022-06-20 16:15:02.000000 miniworldmaker-2.9.0.0/miniworldmaker/tokens/shapes.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1866 2022-06-19 10:00:32.000000 miniworldmaker-2.9.0.0/miniworldmaker/tokens/text_token.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)    60197 2022-06-20 21:17:17.000000 miniworldmaker-2.9.0.0/miniworldmaker/tokens/token.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     6497 2022-06-20 20:55:57.000000 miniworldmaker-2.9.0.0/miniworldmaker/tokens/token_base.py
+drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-20 21:26:19.213439 miniworldmaker-2.9.0.0/miniworldmaker/tools/
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)        0 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/tools/__init__.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)      241 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/tools/binding.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)       99 2022-06-13 06:31:32.000000 miniworldmaker-2.9.0.0/miniworldmaker/tools/board_inspection.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)      415 2022-03-03 16:30:17.000000 miniworldmaker-2.9.0.0/miniworldmaker/tools/color.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1152 2022-06-13 06:30:45.000000 miniworldmaker-2.9.0.0/miniworldmaker/tools/inspection.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1419 2022-03-01 12:28:40.000000 miniworldmaker-2.9.0.0/miniworldmaker/tools/keys.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1366 2022-05-22 11:22:59.000000 miniworldmaker-2.9.0.0/miniworldmaker/tools/method_caller.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3058 2022-05-23 06:17:09.000000 miniworldmaker-2.9.0.0/miniworldmaker/tools/timer.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     1863 2022-05-08 18:47:19.000000 miniworldmaker-2.9.0.0/miniworldmaker/tools/token_class_inspection.py
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)      697 2022-06-13 06:31:32.000000 miniworldmaker-2.9.0.0/miniworldmaker/tools/token_inspection.py
+drwxr-xr-x   0 asiebel   (1000) asiebel   (1000)        0 2022-06-20 21:26:19.200106 miniworldmaker-2.9.0.0/miniworldmaker.egg-info/
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     3630 2022-06-20 21:26:19.000000 miniworldmaker-2.9.0.0/miniworldmaker.egg-info/PKG-INFO
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)     5095 2022-06-20 21:26:19.000000 miniworldmaker-2.9.0.0/miniworldmaker.egg-info/SOURCES.txt
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)        1 2022-06-20 21:26:19.000000 miniworldmaker-2.9.0.0/miniworldmaker.egg-info/dependency_links.txt
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)       63 2022-06-20 21:26:19.000000 miniworldmaker-2.9.0.0/miniworldmaker.egg-info/requires.txt
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)       15 2022-06-20 21:26:19.000000 miniworldmaker-2.9.0.0/miniworldmaker.egg-info/top_level.txt
+-rw-r--r--   0 asiebel   (1000) asiebel   (1000)       38 2022-06-20 21:26:19.213439 miniworldmaker-2.9.0.0/setup.cfg
+-rwxr-xr-x   0 asiebel   (1000) asiebel   (1000)     1388 2022-06-20 21:23:59.000000 miniworldmaker-2.9.0.0/setup.py
```

### Comparing `miniworldmaker-2.8.0.0/LICENSE.txt` & `miniworldmaker-2.9.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/PKG-INFO` & `miniworldmaker-2.9.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniworldmaker
-Version: 2.8.0.0
+Version: 2.9.0.0
 Summary: Create 2D Miniworlds and Games
 Home-page: https://github.com/asbl/miniworldmaker
 Download-URL: https://github.com/asbl/miniworldmaker
 Author: Andreas Siebel
 Author-email: andreas.siebel@it-teaching.de
 License: OSI Approved :: MIT License
 Keywords: games,education,mini-worlds,pygame
```

### Comparing `miniworldmaker-2.8.0.0/README.md` & `miniworldmaker-2.9.0.0/README.md`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/__init__.py` & `miniworldmaker-2.9.0.0/miniworldmaker/__init__.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/appearances/appearance.py` & `miniworldmaker-2.9.0.0/miniworldmaker/appearances/appearance.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,16 +19,15 @@
         
     @property
     def font_size(self):
         return self.font_manager.font_size
 
     @font_size.setter
     def font_size(self, value):
-        self.font_manager.font_size = value
-        self.reload_transformations_after("write_text")
+        self.font_manager.set_font_size(value, update = True)      
 
     def set_font(self, font, font_size):
         self.font_manager.font_path = font
         self.font_manager.font_size = font_size
 
     def set_animation_speed(self, value):
         self.animation_speed = value
@@ -72,15 +71,15 @@
 
         """
         return self._is_textured
 
     @is_textured.setter
     def is_textured(self, value):
         self._is_textured = value
-        self.reload_transformations_after("texture")
+        self.set_dirty("texture", Appearance.RELOAD_ACTUAL_IMAGE)
 
     @property
     def is_rotatable(self):
         """If True, costume will be rotated with token direction
 
         Examples:
 
@@ -111,25 +110,25 @@
 
         """
         return self._is_rotatable
 
     @is_rotatable.setter
     def is_rotatable(self, value):
         self._is_rotatable = value
-        self.dirty = 1
+        self.set_dirty("all", Appearance.RELOAD_ACTUAL_IMAGE)
 
     @property
     def is_centered(self):
         """ """
         return self._is_centered
 
     @is_centered.setter
     def is_centered(self, value):
         self._is_centered = value
-        self.dirty = 1
+        self.set_dirty("all", Appearance.RELOAD_ACTUAL_IMAGE)
 
     @property
     def orientation(self):
         """bool: If True, the image will be rotated by parent orientation before it is rotated.
 
         Examples:
 
@@ -167,15 +166,15 @@
 
         """
         return self._orientation
 
     @orientation.setter
     def orientation(self, value):
         self._orientation = value
-        self.reload_transformations_after("orientation")
+        self.set_dirty("orientation", Appearance.RELOAD_ACTUAL_IMAGE)
 
     @property
     def is_flipped(self):
         """Flips the costume or background. The image is mirrored over the y-axis of costume/background.
 
         Examples:
 
@@ -209,15 +208,15 @@
 
         """
         return self._is_flipped
 
     @is_flipped.setter
     def is_flipped(self, value):
         self._is_flipped = value
-        self.reload_transformations_after("flip")
+        self.set_dirty("all", Appearance.RELOAD_ACTUAL_IMAGE)
 
     def flip(self, value):
         self.is_flipped = value
 
     @property
     def is_scaled(self):
         """Scales the actor to parent-size without remaining aspect-ratio.
@@ -248,15 +247,15 @@
     @is_scaled.setter
     def is_scaled(self, value):
         if value:
             self._is_upscaled = False
             self._is_scaled_to_height = False
             self._is_scaled_to_width = False
         self._is_scaled = value
-        self.reload_transformations_after("scale")
+        self.set_dirty("scale", Appearance.RELOAD_ACTUAL_IMAGE)
 
     @property
     def is_upscaled(self):
         """If True, the image will be upscaled remaining aspect-ratio.
 
         Examples:
 
@@ -281,80 +280,80 @@
     @is_upscaled.setter
     def is_upscaled(self, value):
         if value:
             self._is_scaled = False
             self._is_scaled_to_height = False
             self._is_scaled_to_width = False
         self._is_upscaled = value
-        self.reload_transformations_after("scale")
+        self.set_dirty("scale", Appearance.RELOAD_ACTUAL_IMAGE)
 
     @property
     def is_scaled_to_width(self):
         return self._is_scaled_to_width
 
     @is_scaled_to_width.setter
     def is_scaled_to_width(self, value):
         if value:
             self._is_upscaled = False
             self.is_scaled = False
             self._is_scaled_to_height = False
         self.is_scaled = False
         self._is_scaled_to_width = value
-        self.reload_transformations_after("scale")
+        self.set_dirty("scale", Appearance.RELOAD_ACTUAL_IMAGE)
 
     @property
     def is_scaled_to_height(self):
         return self._is_scaled_to_height
 
     @is_scaled_to_height.setter
     def is_scaled_to_height(self, value):
         if value:
             self._is_upscaled = False
             self.is_scaled = False
             self._is_scaled_to_height = False
         self.is_scaled = False
         self._is_scaled_to_height = value
-        self.reload_transformations_after("scale")
+        self.set_dirty("scale", Appearance.RELOAD_ACTUAL_IMAGE)
 
     @property
     def fill_color(self):
         return self._fill_color
 
     @fill_color.setter
     def fill_color(self, value):
         self._fill_color = value
-        self.reload_transformations_after("all")
+        self.set_dirty("all", Appearance.RELOAD_ACTUAL_IMAGE)
 
     @property
     def coloring(self):
         """
         Defines a colored layer. Coloring is True or false. The color is defined by the attribute appearance.color
 
         """
         return self._coloring
 
     @coloring.setter
     def coloring(self, value):
         self._coloring = value
-        self.reload_transformations_after("coloring")
+        self.set_dirty("coloring", Appearance.RELOAD_ACTUAL_IMAGE)
 
     @property
     def transparency(self):
         """Defines a transparency.
 
         If ``transparency``is ``True``, the che transparency value
         is defined by the attribute ``appearance.alpha``
 
         """
         return self._transparency
 
     @transparency.setter
     def transparency(self, value):
         self._transparency = value
-        self.reload_transformations_after("transparency")
+        self.set_dirty("transparency", Appearance.RELOAD_ACTUAL_IMAGE)
 
     @property
     def alpha(self):
         """defines transparency of Token: 0: transparent, 255: visible
         If value < 1, it will be multiplied with 255.
 
         Examples:
@@ -386,15 +385,15 @@
             value = value * 255
         if value == 255:
             self.transparency = False
         else:
             self.transparency = True
 
     def get_text_width(self):
-        return self.font_manager.get_font_width()
+        return self.font_manager.get_text_width()
 
     def remove_last_image(self):
         self.image_manager.remove_last_image()
 
     def add_image(self, source: Union[str, pygame.Surface, Tuple] = None) -> int:
         """Adds an image to the appearance
 
@@ -492,14 +491,15 @@
             board.run()
 
         .. video:: ../_static/animate.webm
             :autoplay:
             :width: 300
             :height: 100
         """
+        self._animation_start_frame = self.board.frame
         self.is_animated = True
 
     def after_animation(self):
         """
         the method is overwritten in subclasses costume and appearance
 
         Examples:
@@ -633,29 +633,29 @@
 
 
     def fill(self, value):
         """Set default fill color for borders and lines"""
         self._is_filled = value
         if self.is_filled != None and self.is_filled != False and self.is_filled != True:
             self.fill_color = color.Color(value).get()
-        self.reload_transformations_after("all")
+        self.set_dirty("all", Appearance.RELOAD_ACTUAL_IMAGE)
 
     @property
     def is_filled(self):
         """Is token filled with color?"""
         return self._is_filled
 
     @is_filled.setter
     def is_filled(self, value):
         """Defines if costume is filled with a color.
 
         if ``_is_filled`` set to a color-value, ``self.fill_color`` is set to the color.
         
         """
-        self.fill(value)
+        self._is_filled = value
 
     @property
     def stroke_color(self):
         """see border color"""
         return self._border_color
 
     @stroke_color.setter
@@ -667,15 +667,15 @@
         """border color of token"""
         return self._border_color
 
     @border_color.setter
     def border_color(self, value: int):
         if value != None:
             self._border_color = value
-            self.reload_transformations_after("all")
+            self.set_dirty("all", Appearance.RELOAD_ACTUAL_IMAGE)
         else:
             self.border = None
 
     @property
     def border(self):
         """The border-size of token.
 
@@ -689,15 +689,15 @@
     @border.setter
     def border(self, value : Union[int, None]):
         if not value:
             value = 0
         if type(value) != int:
             raise TypeError("border value should be of type int")
         self._border = value
-        self.reload_transformations_after("all")
+        self.set_dirty("all", Appearance.RELOAD_ACTUAL_IMAGE)
 
     def get_color(self, position):
         x = int(position[0])
         y = int(position[1])
         if 0 <= x < self.image.get_width() and 0 <= y < self.image.get_height():
             return self.image.get_at((x,y))
         else:
@@ -712,14 +712,14 @@
         elif type(source) == tuple:
             self.draw_color_on_image(source, position, width, height)
 
     def draw_on_image(self, path, position, width, height):
         file = self.image_manager.find_image_file(path)
         surface = self.image_manager.load_image(file)
         self.draw_image_append(surface, pygame.Rect(position[0], position[1], width, height))
-        self.reload_transformations_after("all")
+        self.set_dirty("draw_images", Appearance.RELOAD_ACTUAL_IMAGE)
 
     def draw_color_on_image(self, color, position, width, height):
         surface = pygame.Surface((width, height))
         surface.fill(color)
         self.draw_image_append(surface, pygame.Rect(position[0], position[1], width, height))
-        self.reload_transformations_after("all")
+        self.set_dirty("draw_images", Appearance.RELOAD_ACTUAL_IMAGE)
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/appearances/appearance_base.py` & `miniworldmaker-2.9.0.0/miniworldmaker/appearances/appearance_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,26 +10,30 @@
 
 from miniworldmaker.exceptions.miniworldmaker_exception import MiniworldMakerError
 from miniworldmaker.appearances.managers.image_manager import ImageManager
 
 
 class MetaAppearance(type):
     def __call__(cls, *args, **kwargs):
-        instance = super().__call__(*args, **kwargs)
+        instance = type.__call__(cls, *args, **kwargs)  # create a new Appearance of type...
         instance.after_init()
         return instance
 
 
 class AppearanceBase(metaclass=MetaAppearance):
     counter = 0
 
+    RELOAD_ACTUAL_IMAGE = 1
+    LOAD_NEW_IMAGE = 2
+
     def __init__(self):
         self.id = AppearanceBase.counter + 1
         AppearanceBase.counter += 1
         self.initialized = False
+        self._flag_transformation_pipeline = False
         self.parent = None
         self.board = None
         self.draw_shapes = []
         self.draw_images = []
         self._is_flipped = False
         self._is_animated = False
         self._is_textured = False
@@ -48,100 +52,107 @@
         self._border_color = None
         self._alpha = 255
         self._dirty = 0
         self._image = pygame.Surface((0, 0))  # size set in image()-method
         self.surface_loaded = False
         self.last_image = None
         self.font_manager = font_manager.FontManager(self)
-        self.image_manager = image_manager.ImageManager(self)
+        self.image_manager : "image_manager.ImageManager" = image_manager.ImageManager(self)
         self.transformations_manager = transformations_manager.TransformationsManager(self)
         self.image_manager.add_default_image()
         # properties
         self.texture_size = (0, 0)
-        self.animation_speed = 100  #: The animation speed for animations
+        self.animation_speed = 10  #: The animation speed for animations
         self.loop = False
         self.animation_length = 0
-        self.dirty = 1
-
+        self._animation_start_frame = 0
 
     def after_init(self):
         # Called in metaclass
-        self.reload_transformations_after(
-            "all",
-        )
+        self.set_dirty("all", AppearanceBase.LOAD_NEW_IMAGE)
         self.initialized = True
 
-    def reload_transformations_after(self, value):
-        if hasattr(self, "transformations_manager"):
-            self.transformations_manager.reload_transformations_after(value)
-            self.dirty = 1
-
     def draw_shape_append(self, shape, arguments):
         self.draw_shapes.append((shape, arguments))
-        self.reload_transformations_after("all")
 
     def draw_shape_set(self, shape, arguments):
         self.draw_shapes = [(shape, arguments)]
-        self.reload_transformations_after("all")
 
     def draw_image_append(self, surface, rect):
         self.draw_images.append((surface, rect))
-        self.reload_transformations_after("all")
 
     def draw_image_set(self, surface, rect):
         self.draw_images = [(surface, rect)]
-        self.reload_transformations_after("all")
 
     @property
     def dirty(self):
         return self._dirty
 
     @dirty.setter
     def dirty(self, value):
-        self._dirty = value
-        if self.parent and value == 1:
-            self.parent.dirty = 1
-            
-    def _reload_image(self):
-        """If dirty, the image will be reloaded.
-        The image pipeline will be  processed, defined by "reload_transformations_after"
-        """
-        if self.dirty == 1:
-            self._reload_dirty_image()
+        if value == 0:
+            self._dirty = 0
+        else:
+            self.set_dirty(value)
 
-    def _reload_dirty_image(self):
-        """Reloads image from image_index in image_manager.images_list and processes transformations pipeline
-        
-        Called by property `image`, if image is dirty
-        Sets dirty to 0.
-        """
-        self.dirty = 0
-        image = self.image_manager.load_image_by_image_index()
-        image = self.transformations_manager.process_transformation_pipeline(image, self)
-        self._image = image
+    def set_dirty(self, value="all", status=1):
+        if hasattr(self, "transformations_manager"):
+            if value != None:
+                self.transformations_manager.flag_reload_actions_for_transformation_pipeline(value)
+            if status >= self._dirty:
+                self._dirty = status
+            if self.parent:
+                self.parent.dirty = 1
 
     @property
     def image(self) -> pygame.Surface:
         """Performs all actions in image pipeline"""
-        self._reload_image()
+        return self.get_image()
+    
+    def get_image(self):
+        """If dirty, the image will be reloaded.
+        The image pipeline will be  processed, defined by "set_dirty"
+        """
+        if self.dirty >= self.RELOAD_ACTUAL_IMAGE or not self._image and not self._flag_transformation_pipeline:
+            dirty = self.dirty
+            self.dirty = 0
+            self._flag_transformation_pipeline = True
+            self._before_transformation_pipeline()
+            image = self.image
+            if dirty >= self.RELOAD_ACTUAL_IMAGE:
+                # @todo: Not working: Replace RELOAD_ACTUAL_IMAGE with LOAD NEW IMAGE
+                image = self.image_manager.load_image_from_image_index()
+            if dirty >= self.RELOAD_ACTUAL_IMAGE:
+                image = self.transformations_manager.process_transformation_pipeline(image, self)
+                self._after_transformation_pipeline()
+                self._flag_transformation_pipeline = False
+            self._image = image
         return self._image
 
-    def add_images(self, sources : list):
+    def _before_transformation_pipeline(self):
+        pass
+    def _after_transformation_pipeline(self):
+        pass
+
+
+    def add_images(self, sources: list):
         assert type(sources) == list
         for image in sources:
             self.add_image(image)
-        
+
     def add_image(self, source: Union[str, Tuple, pygame.Surface]) -> int:
         """Adds an image to the appearance
 
         Returns:
             Index of the created image.
         """
         if type(source) not in [str, pygame.Surface, tuple]:
-            raise MiniworldMakerError(f"Error: Image source has wrong format (expected str or pygame.Surface, got {type(source)}")
+            raise MiniworldMakerError(
+                f"Error: Image source has wrong format (expected str or pygame.Surface, got {type(source)}"
+            )
         self.image_manager.add_image(source)
 
     def set_image(self, source: Union[int, "AppearanceBase"]) -> bool:
         if type(source) == int:
             return self.image_manager.set_image_index(source)
         elif type(source) == tuple:
             surface = image_manager.ImageManager.get_surface_from_color(source)
@@ -151,34 +162,21 @@
         """Loads the next image,
         called 1/frame"""
         asyncio.run(self.image_manager.update())
         return 1
 
     def __str__(self):
         return (
-                self.__class__.__name__
-                + "with ID ["
-                + str(self.id)
-                + "] for parent:["
-                + str(self.parent)
-                + "], images: "
-                + str(self.image_manager.images_list)
-        )
-
-    def rotated(self):
-        self.reload_transformations_after("rotate")
-
-    def resized(self):
-        self.reload_transformations_after(
-            "scale",
-        )
-
-    def visible(self):
-        self.reload_transformations_after(
-            "all",
+            self.__class__.__name__
+            + "with ID ["
+            + str(self.id)
+            + "] for parent:["
+            + str(self.parent)
+            + "], images: "
+            + str(self.image_manager.images_list)
         )
 
     def register(self, method: callable):
         """
         Register method for decorator. Registers method to token or background.
         """
         bound_method = binding.bind_method(self, method)
@@ -198,17 +196,15 @@
         """
         return self.font_manager.text
 
     @text.setter
     def text(self, value):
         if value == "":
             self.font_manager.text = ""
-            self.dirty = 1
+            self.set_dirty("write_text", AppearanceBase.RELOAD_ACTUAL_IMAGE)
         else:
             self.font_manager.text = value
-        self.reload_transformations_after(
-            "all",
-        )
+        self.set_dirty("write_text",AppearanceBase.RELOAD_ACTUAL_IMAGE)
 
     @property
     def images(self):
-        return self.image_manager.images_list
+        return self.image_manager.images_list
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/appearances/appearances_manager.py` & `miniworldmaker-2.9.0.0/miniworldmaker/appearances/appearances_manager.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Union, Tuple, List
 
 import pygame
 import miniworldmaker
 import miniworldmaker.appearances.appearance as appearance_mod
 from miniworldmaker.appearances import costume
+from miniworldmaker.appearances import appearance_base
 import miniworldmaker.exceptions.miniworldmaker_exception as miniworldmaker_exception
 from miniworldmaker.exceptions.miniworldmaker_exception import MiniworldMakerError
 
 
 class AppearancesManager:
     def __init__(self, parent):
         self.appearances_list = []
@@ -18,15 +19,16 @@
         self.is_animated = None
         self.animation_speed = 10
         self.is_upscaled = None
         self.is_scaled = None
         self.is_scaled_to_width = None
         self.is_scaled_to_height = None
         self.has_appearance = False
-
+        self._iter_index = 0   
+    
     @property
     def image(self):
         if self.appearance:
             return self.appearance.image
         else:
             return pygame.Surface((1, 1))
 
@@ -36,57 +38,61 @@
         if source is None:
             appearance = self.create_appearance()
         elif type(source) in [str, pygame.Surface, tuple]:
             appearance = self.create_appearance()
             appearance.add_image(source)
         return appearance
 
-    def add_new_appearances(self, sources: "List"):
+    def add_new_appearances(self, sources: List):
         if type(sources) in [list]:
             for appearance in sources:
                 self.add_new_appearance(appearance)
         else:
             raise MiniworldMakerError(f"Appearances must be list, got {type(sources)}")
 
     def add_new_appearance_from_list(self, sources: List) -> "appearance_mod.Appearance":
         head = sources[0]
         tail = sources[1:]
         appearance = self.add_new_appearance(head)
         for source in tail:
             appearance.add_image(source)
         return appearance
 
-    def _add_default_appearance(self):
-        appearance = self.create_appearance()
-        return self._add_first_appearance(appearance)
 
     def create_appearance(self) -> "appearance_mod.Appearance":
         """Returns a new appearance (Background instance or Costume instance)"""
         pass
 
     def add_new_appearance(
-        self, source: Union[str, pygame.Surface, "costume.Costume", Tuple]
+        self, source: Union[str, pygame.Surface, "costume.Costume", Tuple, None]
     ) -> "appearance_mod.Appearance":
         """Adds a new Appearance (costume or background) to manager.
 
         called by ``add_costume`` and ``add_background`` in subclasses.
         """
-        if type(source) not in [str, pygame.Surface, tuple] and not isinstance(source, costume.Costume):
-            raise MiniworldMakerError(
-                f"Error: Got wrong type for appearance. Expected: str, pygame.Surface, Costume, tuple;  got {type(source)}, {source}"
-            )
+
         appearance: "appearance_mod.Appearance" = self._create_appearance_from_source(source)
         if not self.has_appearance and source:
             self.has_appearance = True
             return self._add_first_appearance(appearance)
+        elif not self.has_appearance and not source:
+            self.has_appearance = False
+            return self._add_default_appearance
         elif source:
             return self._add_appearance_to_manager(appearance)
         else:
-            raise MiniworldMakerError("unexpected behaviour")
+            raise MiniworldMakerError(
+                f"Error: Got wrong type for appearance. Expected: str, pygame.Surface, Costume, tuple;  got {type(source)}, {source}"
+            )
+
 
+    def _add_default_appearance(self):
+        appearance = self.create_appearance()
+        return self._add_first_appearance(appearance)
+    
     def _add_first_appearance(self, appearance: "appearance_mod.Appearance") -> "appearance_mod.Appearance":
         self.appearances_list = []
         self._add_appearance_to_manager(appearance)
         return appearance
 
     def _add_appearance_to_manager(self, appearance: "appearance_mod.Appearance") -> "appearance_mod.Appearance":
         self.appearance = appearance
@@ -101,19 +107,17 @@
             appearance.is_upscaled = self.is_upscaled
         if self.is_scaled_to_width is not None:
             appearance.is_scaled_to_width = self.is_scaled_to_width
         if self.is_scaled_to_height is not None:
             appearance.is_scaled_to_height = self.is_scaled_to_height
         if self.is_scaled is not None:
             appearance.is_scaled = self.is_scaled
+        self.appearance.set_dirty("all", self.appearance.LOAD_NEW_IMAGE)
         return appearance
 
-    def remove(self, index):
-        del self.appearances_list[index]
-
     def next_appearance(self) -> "appearance_mod.Appearance":
         """Switches to next appearance
 
         Returns:
             appearance_mod.Appearance: the switched appearance
         """
         index = self.find_appearance(self.appearance)
@@ -125,34 +129,41 @@
 
     def length(self) -> int:
         """Number of appearance in appearance manager
 
         Returns:
             int: _description_
         """
-        return len(self.appearances_list)
-    
-
-    def get_appearance_at_index(self, index) -> "appearance_mod.Appearance":
-        return self.appearances_list[index]
+        if self.has_appearance:
+            return len(self.appearances_list)
+        else:
+            return 0
+        
+    def __len__(self) -> int:
+        return self.length()
+
+    def get_appearance_at_index(self, index) -> Union["appearance_mod.Appearance", None]:
+        if 0 <= index < len(self.appearances_list):
+            return self.appearances_list[index]
+        else:
+            return None
 
-    def find_appearance(self, appearance: "appearance_mod.Appearance") -> int :
+    def find_appearance(self, appearance: "appearance_mod.Appearance") -> int:
         """Searches for appearance; returns index of appearance
 
         Returns:
             int: Index of found appearance; -1 if appearance was not found.
         """
         for index, a_appearance in enumerate(self.appearances_list):
             if a_appearance == appearance:
                 return index
         return -1
 
     def _set_all(self, attribute, value):
-        """Sets attribute for all appearance in manager.
-        """
+        """Sets attribute for all appearance in manager."""
         for appearance in self.appearances_list:
             setattr(appearance, attribute, value)
 
     def set_animated(self, value):
         self.is_animated = value
         self._set_all("is_animated", value)
 
@@ -187,68 +198,104 @@
             List[appearance_mod.Appearance]: All appearances in manager as list
         """
         return self.appearances_list
 
     def __str__(self):
         return str(len(self.appearances_list)) + " Appearances: " + str(self.appearances_list)
 
-    def _remove_appearance_at_index(self, index : int):
-        appearance = self.get_appearance_at_index(index)
-        self._remove_appearance_from_manager(appearance)
-
-    def _remove_appearance_from_manager(self, appearance : "appearance_mod.Appearance"):
-        if self.has_appearance and self.count():
+    def _remove_appearance_from_manager(self, appearance: "appearance_mod.Appearance"):
+        if self.has_appearance and self.length() > 0:
             if appearance == self.appearance:
-                index = self.find_appearance(appearance)
-                self.appearances_list.remove(appearance)
-                if index == 0:
-                    self.has_costume = False
+                if self.length() == 1:
+                    self.appearances_list.remove(appearance)
+                    del appearance
                     self._add_default_appearance()
-                self.switch_appearance(self.get_appearance_at_index(index - 1))
+                    self.has_appearance = False
+                else:
+                    first_appearance = self.get_appearance_at_index(0)
+                    self.switch_appearance(first_appearance)
+                    self.appearances_list.remove(appearance)
+                    del appearance
 
     def remove_appearance(self, source: Union[int, "appearance_mod.Appearance"] = -1):
         """Removes an appearance (costume or background) from manager
 
         Defaults:
             Removes last costume.
 
         Args:
             source: The index of the new appearance or the Appearance which should be removed Defaults to -1
             (last costume)
         """
+
         if type(source) == int:
-            self._remove_appearance_at_index(source)
-        elif isinstance(source, appearance_mod.Appearance):
+            source = self.get_appearance_at_index(source)
+        if source and isinstance(source, appearance_mod.Appearance):
             self._remove_appearance_from_manager(source)
+        else:
+            raise MiniworldMakerError(f"Expected type int or Appearance (Costume or Background), got {type(source)}")
 
     def switch_appearance(self, source: Union[int, "appearance_mod.Appearance"]) -> "appearance_mod.Appearance":
         if type(source) == int:
             if source >= self.length():
                 raise miniworldmaker_exception.CostumeOutOfBoundsError(self.parent, self.length(), source)
             new_appearance = self.get_appearance_at_index(source)
         elif isinstance(source, appearance_mod.Appearance) or isinstance(source, miniworldmaker.Appearance):
             new_appearance = source
         self.appearance = new_appearance
         self.appearance.image_manager.end_animation(new_appearance)
-        self.appearance.dirty = 1
+        self.appearance.set_image(0)
+        self.appearance.set_dirty("all", self.appearance.LOAD_NEW_IMAGE)
         return self.appearance
 
-    def animate(self, speed):
+    def animate(self, speed : int):
         self.appearance.animation_speed = speed
         self.appearance.animate()
 
+    def get_board(self):
+        """Implemented in subclasses
+        """
+        pass
+    
     def animate_appearance(self, appearance, speed):
         if appearance is None:
             raise miniworldmaker_exception.CostumeIsNoneError()
         self.switch_appearance(appearance)
-        self.costume.animation_speed = speed
-        self.costume.animate()
+        self.appearance.animation_speed = speed
+        self.appearance.animate()
 
     def self_remove(self):
         """Implemented in subclasses"""
         pass
 
-    def count(self):
-        if self.has_appearance:
-            return len(self.appearances_list)
+    def __iter__(self):
+        self._iter_index = 0
+        return self
+
+    def __next__(self):
+        if self._iter_index < len(self.appearances_list):
+            apperance_at_position = self.get_appearance_at_index(self._iter_index)
+            self._iter_index += 1
+            return apperance_at_position
         else:
-            return 0
+            raise StopIteration
+        
+    @property
+    def orientation(self):
+        return [appearance.orientation for appearance in self.appearances_list]
+    
+    @orientation.setter
+    def orientation(self, value):
+        for appearance in self.appearances_list:
+            appearance.orientation = value
+
+    @property
+    def animation_speed(self):
+        return self.appearance.animation_speed
+    
+    @animation_speed.setter
+    def animation_speed(self, value):
+        for appearance in self.appearances_list:
+            appearance.animation_speed = value        
+            
+    def get_actual_appearance(self):
+        return self.appearance
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/appearances/background.py` & `miniworldmaker-2.9.0.0/miniworldmaker/appearances/background.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,26 +51,22 @@
         self.parent = board  #: The parent of a Background is the associated board.
         if not board:
             board = app.App.board
         self.board = board
         # Register image actions which you can be triggered
         self._grid = False
         self._grid_color = (255, 0, 255)
-        self.surface = None
+        self.surface = pygame.Surface((self.board.container_width, self.board.container_height))
         self._is_scaled_to_tile = False
         self._image = pygame.Surface((self.parent.width, self.parent.height))  # size set in image()-method
         self.reload_costumes_queue = []
         self.is_scaled = True
         self.transformations_manager = transformations_background_manager.TransformationsBackgroundManager(self)
         self.image_manager = image_background_manager.ImageBackgroundManager(self)
 
-    def add_image(self, source: Union[str, pygame.Surface, Tuple] = None) -> int:
-        super().add_image(source)
-        return self.parent.app.window.display_update()
-
     def show_grid(self):
         self.grid = True
 
     @property
     def grid(self) -> Union[bool, tuple]:
         """Shows a grid-overlay
 
@@ -100,55 +96,43 @@
 
         """
         return self._grid
 
     @grid.setter
     def grid(self, value):
         self._grid = value
-        self.reload_transformations_after("all")
+        self.set_dirty("all", Background.LOAD_NEW_IMAGE)
 
     def repaint(self):
         """Called 1/frame from board"""
         self.board.tokens.clear(self.surface, self.image)
         repaint_rects = self.board.tokens.draw(self.surface)
         self.board.app.window.repaint_areas.extend(repaint_rects)
 
-    def reload_transformations_after(self, value):
-        """reloads all transformations (scale, upscale, draw shape, rotate for shape)
-
-        The transformation pipeline is not run through completely,
-        but starting from the passed parameter -
-        The remaining transformations are loaded from the cache.
-
-        "all": Reloads all Transformations
-        "scale": Reloads transformations after scale
-        ...
-        """
-        super().reload_transformations_after(value)
-
     def _update_all_costumes(self):
         """updates costumes for all tokens on board"""
         [token.costume.update() for token in self.reload_costumes_queue]
         self.reload_costumes_queue = []
         if hasattr(self.board, "dynamic_tokens"):
             dynamic_tokens = self.board.dynamic_tokens.copy()
             [token.costume.update() for token in dynamic_tokens]
             del(dynamic_tokens)
 
-    def _reload_dirty_image(self):
-        """ Reloads dirty image
-        
-        Called by property `image`, if image is dirty.
-        """
-        super()._reload_dirty_image()
+    def _after_transformation_pipeline(self):
         self.surface = pygame.Surface((self.board.container_width, self.board.container_height))
         self.surface.blit(self.image, self.surface.get_rect())
-        for token in self.board.tokens:
+        for token in self.board.camera.get_tokens_in_viewport():
             token.dirty = 1
         self._blit_to_window_surface()
         self._update_all_costumes()
 
     def _blit_to_window_surface(self):
         """Blits background to window surface"""
         self.parent.app.window.surface.blit(self.image, (0, 0))
         self.parent.app.window.add_display_to_repaint_areas()
         self.repaint()
+
+    def add_image(self, source: Union[str, Tuple, pygame.Surface]) -> int:
+        super().add_image(source)
+        self._blit_to_window_surface()
+        self._update_all_costumes()
+        return self.parent.app.window.display_update()
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/appearances/backgrounds_manager.py` & `miniworldmaker-2.9.0.0/miniworldmaker/appearances/backgrounds_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Union
 
 import miniworldmaker.appearances.appearances_manager as appearances_manager
 import miniworldmaker.appearances.background as background
+from miniworldmaker.appearances import appearance
 
 
 class BackgroundsManager(appearances_manager.AppearancesManager):
     def __init__(self, parent):
         super().__init__(parent)
         self.repaint_all: int = 1
 
@@ -42,9 +43,9 @@
             token.dirty = 1
         return background
 
     @property
     def backgrounds(self):
         return self.appearances_list
     
-    def remove_background(self, source: Union[int, "appearance_mod.Appearance"] = -1):
-        self.remove_appearance(source)
+    def get_board(self):
+        return self.parent
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/appearances/costume.py` & `miniworldmaker-2.9.0.0/miniworldmaker/appearances/costume.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,17 +22,17 @@
         self.is_rotatable = False
         self.fill_color = None
         self.border_color = None
         self.transformations_manager = transformations_costume_manager.TransformationsCostumeManager(self)
 
     def after_init(self):
         # Called in metaclass
-        super().after_init()
         self._set_default_color_values()
-        self._update_draw_shape()
+        super().after_init()
+
         
     def _set_default_color_values(self):
         self._set_token_default_values()
         self._set_board_default_values()
         
     def _set_token_default_values(self):
         self._info_overlay = False
@@ -59,27 +59,22 @@
             color: Color of info_overlay
         """
         return self._info_overlay
 
     @info_overlay.setter
     def info_overlay(self, value):
         self._info_overlay = value
-        self.reload_transformations_after(
-            "all",
+        self.set_dirty("all",Costume.RELOAD_ACTUAL_IMAGE
         )
-
-    def _reload_dirty_image(self):
-        """Reloads a dirty image. 
         
-        Called by property `image`, if image is dirty.
-        
-        called by ...
-        """
-        self._update_draw_shape()
-        super()._reload_dirty_image()
+    def set_dirty(self, value, status):
+        if value != None and self.parent and self.images:
+            self._update_draw_shape()
+        super().set_dirty(value, status)
+
 
     def set_image(self, source) -> bool:
         super().set_image(source)
 
     def _inner_shape(self) -> pygame.Rect:
         """Returns inner shape of costume
 
@@ -94,22 +89,22 @@
         Returns:
             pygame.Rect: Outer shape (Rectangle with size of tokens without filling.)
         """
         return pygame.draw.rect, [pygame.Rect(0, 0, self.parent.size[0], self.parent.size[1]), self.border]
 
     def _update_draw_shape(self):
         self.draw_shapes = []
-        if self._inner_shape():
+        if self._inner_shape() and self.image_manager:
             if self.is_filled and not self.image_manager.is_image():
                 self.draw_shape_append(self._inner_shape()[0], self._inner_shape_arguments())
         if self._outer_shape() and self.border:
             self.draw_shape_append(self._outer_shape()[0], self._outer_shape_arguments())
 
     def _inner_shape_arguments(self) -> List:
-        """Gets arguments for inner shape
+        """def setGets arguments for inner shape
 
         Returns:
             List[]: List of arguments
         """
         
         color = self.fill_color
         return [
@@ -122,7 +117,18 @@
         Returns:
             List[]: List of arguments
         """
         color = self.border_color
         return [
             color,
         ] + self._outer_shape()[1]
+
+    def rotated(self):
+        if self.board.camera.is_token_in_viewport(self.token):
+            self.set_dirty("rotate", self.RELOAD_ACTUAL_IMAGE)
+
+    def resized(self):
+        self.set_dirty("scale", self.RELOAD_ACTUAL_IMAGE)
+
+    def visible(self):
+        if self.board.camera.is_token_in_viewport(self.token):
+            self.set_dirty("all", self.RELOAD_ACTUAL_IMAGE)
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/appearances/costumes_manager.py` & `miniworldmaker-2.9.0.0/miniworldmaker/appearances/costumes_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,56 +3,40 @@
 import miniworldmaker.appearances.costume as costume_mod
 import miniworldmaker.appearances.appearance as appearance
 
 
 class CostumesManager(appearances_manager.AppearancesManager):
     
     @property
-    def costume(self):
-        return self.appearance
-
-    @costume.setter
-    def costume(self, value):
-        self.appearance = value
-
-    @property
     def token(self):
         return self.parent
 
     @token.setter
     def token(self, value):
         self.parent = value
 
     def get_costume_at_index(self, index):
         return super().get_appearance_at_index(index)
 
-    def add_costume(self, source: Union[str, List[str], "appearance.Appearance"] = None) -> "costume_mod.Costume":
+    def add_new_appearance(self, source: Union[str, List[str], "appearance.Appearance"] = None) -> "costume_mod.Costume":
         """
         Adds a new costume to token.
         The costume can be switched with self.switch_costume(index)
 
         Args:
             path: Path to the first image of new costume
 
         Returns:
             The new costume.
 
         """
-        new_costume = self.add_new_appearance(source)
-        self.costume._update_draw_shape()
-        self.costume.dirty = 1
+        new_costume = super().add_new_appearance(source)
+        self.appearance.set_dirty("all", self.appearance.LOAD_NEW_IMAGE)
         return new_costume
     
-    def add_costume_from_list(self, sources: List) -> "appearance.Appearance":
-        return super().add_new_appearance_from_list(sources)
-
-    def add_costumes(self, source_list):
-        for source in source_list:
-            self.add_costume(source)
-
     def create_appearance(self) -> "costume_mod.Costume":
         """Creates a new costume 
 
         Returns:
             _type_: _description_
         """
         new_costume = self.token._get_new_costume()
@@ -76,8 +60,11 @@
     def has_costume(self, value):
         self.has_appearance = value
 
     def next_costume(self) -> "costume_mod.Costume":
         return self.next_appearance()
 
     def _add_appearance_to_manager(self, appearance):
-        return super()._add_appearance_to_manager(appearance)
+        return super()._add_appearance_to_manager(appearance)
+    
+    def get_board(self):
+        return self.parent.board
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/appearances/hex_costume.py` & `miniworldmaker-2.9.0.0/miniworldmaker/appearances/hex_costume.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,24 +18,24 @@
         self.fill_color = (180, 180, 180, 255)
         self.border = 1
         self.border_color = (100, 100, 100, 255)
         
     def _update_draw_shape(self):
         self.mod_pointlist = []
         board = self.token.board
-        if board.is_tile(self.token.position):
-            tile = self.token.board.get_tile(self.token.position)
+        if board.is_tile(self.token.position_manager.get_position()):
+            tile = self.token.board.get_tile(self.token.position_manager.get_position())
             self.mod_pointlist = tile.get_local_corner_points()
         super()._update_draw_shape()
 
     def _inner_shape(self):
         board = self.token.board
         if board.is_tile(self.token.position):
             return pygame.draw.polygon, [self.mod_pointlist, 0]
-        elif board.is_corner(self.token.position):
+        elif board.is_corner(self.token.position_manager.position):
             return pygame.draw.rect, [pygame.Rect(0, 0, self.token.size[0], self.token.size[1]), 0]
         elif board.is_edge(self.token.position):
             return pygame.draw.rect, [pygame.Rect(0, 0, self.token.size[0], self.token.size[1]), 0]
 
     def _outer_shape(self):
         board = self.token.board
         if board.is_tile(self.token.position):
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/appearances/managers/font_manager.py` & `miniworldmaker-2.9.0.0/miniworldmaker/appearances/managers/font_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import pygame
 
-from miniworldmaker.appearances import appearance
-
 
 class FontManager:
     def __init__(self, appearance):
         self.font_size = 0  #: font_size if token-text != ""
         self.text_position = (0, 0)  #: Position of text relative to the top-left pixel of token
         self.font_path = None  #: Path to font-file
         self.font_style = "monospace"
@@ -17,20 +15,26 @@
         font_size = self.font_size
         if self.font_path is None:
             font = pygame.font.SysFont(self.font_style, font_size)
         else:
             font = pygame.font.Font(self.font_path, font_size)
         return font
 
-    def get_font_width(self):
+    def get_text_width(self):
         font = self._get_font_object()
         return font.size(self.text)[0]
 
     def transformation_write_text(self, image: pygame.Surface, parent, color) -> pygame.Surface:
+        # called from write_text in transformations_manager
         font = self._get_font_object()
         if self.appearance.parent.color == None:
             color = (255,255,255)
         else:
             color = self.appearance.parent.color
-        label = font.render(self.text, 1, color)
-        image.blit(label, self.text_position)
+        rendered_text = font.render(self.text, 1, color)
+        image.blit(rendered_text, self.text_position)
         return image
+
+    def set_font_size(self, value, update = True):
+        self.font_size = value
+        if update:
+            self.appearance.set_dirty("write_text", self.appearance.RELOAD_ACTUAL_IMAGE)
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/appearances/managers/image_background_manager.py` & `miniworldmaker-2.9.0.0/miniworldmaker/appearances/managers/image_background_manager.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/appearances/managers/image_manager.py` & `miniworldmaker-2.9.0.0/miniworldmaker/appearances/managers/image_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         """called in init
         """
         if not self.has_image and len(self.images_list) == 0:
             self.appearance.is_scaled = True
             surf = pygame.Surface((1, 1), pygame.SRCALPHA)
             surf.fill(self.appearance.fill_color)
             self.images_list.append({"image": surf, "type": ImageManager.COLOR})
-            self.appearance.dirty = 1
+            self.appearance.set_dirty("all", self.appearance.LOAD_NEW_IMAGE)
             return len(self.images_list) - 1
 
     def add_image(self, source: Union[str, pygame.Surface, Tuple]) -> int:
         """Adds an image to the appearance
 
         Args:
             path (str): Path to the image relative to actual directory
@@ -148,17 +148,15 @@
         surf = pygame.Surface((1, 1), pygame.SRCALPHA)
         surf.fill(color)
         return surf
 
     def add_image_from_color(self, color : tuple) -> int:
         surf = ImageManager.get_surface_from_color(color)
         self.images_list.append({"image" : surf, "type": ImageManager.COLOR, "source": color})
-        self.appearance.reload_transformations_after(
-            "all",
-        )
+        self.appearance.set_dirty("all",self.appearance.LOAD_NEW_IMAGE)
         return len(self.images_list) - 1
 
     def get_source_from_current_image(self) -> Union[str, pygame.Surface, tuple]:
         """Returns color, path or surface
         """
         return self.images_list[self.image_index]["source"]
 
@@ -172,17 +170,15 @@
             self.add_image_from_path(path)
 
     def add_image_from_path(self, path: str) -> int:
         path = self.find_image_file(path)
         # set image by path
         _image = self.load_image(path)
         self.images_list.append({"image" : _image, "type": ImageManager.IMAGE, "source": path})
-        self.appearance.reload_transformations_after(
-            "all",
-        )
+        self.appearance.set_dirty("all",self.appearance.LOAD_NEW_IMAGE)
         return len(self.images_list) - 1
 
     def add_image_from_appearance(self, appearance, index):
         appearance.image_manager.get_surface(index)
 
     def add_image_from_surface(self, surface) -> int:
         """Adds an image to the appearance
@@ -190,80 +186,75 @@
         Args:
             path (str): Path to the image relative to actual directory
 
         Returns:
             Index of the created image.
         """
         self.images_list.append({"image" : surface, "type": ImageManager.SURFACE, "source": None})
-        self.appearance.reload_transformations_after(
-            "all",
-        )
+        self.appearance.set_dirty("all",self.appearance.LOAD_NEW_IMAGE)
         return len(self.images_list) - 1
 
     def get_surface(self, index):
         try:
             return self.images_list[index]
         except Exception:
             raise ImageIndexNotExistsError(index, self)
 
     def replace_image(self, image, type, source):
         self.images_list[self.image_index] = {"image" : image, "type": type, "source": source}
-        self.appearance.reload_transformations_after(
-            "all",
-        )
+        self.appearance.set_dirty("all",self.appearance.LOAD_NEW_IMAGE)
 
     def reset_image_index(self):
         if self.current_animation_images:
             self.image_index = len(self.images_list) - 1
 
     async def update(self):
         """Loads the image,
         * switches image if neccessary
         * processes transformations pipeline if neccessary
         """
-        if self.appearance.is_animated:
+        if self.appearance.is_animated and self.appearance._animation_start_frame != self.board.frame:
             if self.board.frame != 0 and self.board.frame % self.appearance.animation_speed == 0:
                 await self.next_image()
-        self.appearance._reload_image()
+        self.appearance.get_image()
 
     async def next_image(self):
         """Switches to the next image of the appearance."""
         if self.appearance.is_animated:
             if self.image_index < len(self.images_list) - 1:
                 self.image_index = self.image_index + 1
             else:
                 if not self.appearance.loop:
                     self.appearance.is_animated = False
                     self.appearance.after_animation()
                 self.image_index = 0
-            self.appearance.dirty = 1
-            self.appearance.parent.dirty = 1
-            self.appearance.reload_transformations_after("all")
+            self.appearance.set_dirty("all",self.appearance.LOAD_NEW_IMAGE)
+            
 
     async def first_image(self):
         """Switches to the first image of the appearance."""
         self.image_index = 0
-        self.reload_transformations_after("all")
+        self.set_dirty("all", self.appearance.LOAD_NEW_IMAGE)
 
-    def load_image_by_image_index(self):
+    def load_image_from_image_index(self):
         if self.images_list and self.image_index < len(self.images_list) and self.images_list[self.image_index]:
             # if there is a image list load image by index
             image = self.images_list[self.image_index]["image"]
         else:  # no image files - Render raw surface
             image = self.load_surface()
         return image
 
     def set_image_index(self, value) -> bool:
         if value == -1:
             value = len(self.images_list) - 1
         if 0 <= value < len(self.images_list):
             old_index = self.image_index
             self.image_index = value
             if old_index != self.image_index:
-                self.appearance.reload_transformations_after("all")
+                self.appearance.set_dirty("all",self.appearance.LOAD_NEW_IMAGE)
             return True
         else:
             raise ImageIndexNotExistsError(value, self)
 
     def load_surface(self) -> pygame.Surface:
         if not self.appearance.surface_loaded:
             image = pygame.Surface((self.appearance.parent.width, self.appearance.parent.height), pygame.SRCALPHA)
@@ -275,8 +266,8 @@
         appearance.loop = False
         appearance.set_image(0)
         self.animation_frame = 0
 
     def remove_last_image(self):
         del self.images_list[-1]
         self.set_image(-1)
-        self.appearance.reload_transformations_after("all")
+        self.appearance.set_dirty("all", self.appearance.LOAD_NEW_IMAGE)
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/appearances/managers/transformations_background_manager.py` & `miniworldmaker-2.9.0.0/miniworldmaker/appearances/managers/transformations_background_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,10 +21,11 @@
             i += parent.tile_size
         while j <= parent.width:
             pygame.draw.line(image, appearance._grid_color, (j, 0), (j, parent.height), 1)
             j += parent.tile_size
 
         return image
 
-    def reload_transformations_after(self, transformation_string):
-        super().reload_transformations_after(transformation_string)
-        self.appearance.repaint()
+    #def set_dirty(self, transformation_string, status):
+    #    super().set_dirty(transformation_string, status)
+    #    self.appearance.repaint()
+    # not needed?
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/appearances/managers/transformations_costume_manager.py` & `miniworldmaker-2.9.0.0/miniworldmaker/appearances/managers/transformations_costume_manager.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/appearances/managers/transformations_manager.py` & `miniworldmaker-2.9.0.0/miniworldmaker/appearances/managers/transformations_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,18 @@
         """All, reload_transformations will be set to false
         => next image will completly loaded from cache.
         """
         for key in self.reload_transformations.keys():
             self.reload_transformations[key] = False
 
     def process_transformation_pipeline(self, image, appearance):
+        """Processes the transformation pipeline for a given image.
+
+        The transformations pipeline will be loaded from cache, if nothing is cleared
+        """
         for transformation in self.transformations_pipeline:
             # If an image action is to be executed again,
             # load the last cached image from the pipeline and execute
             # all subsequent image actions.
             if (
                 transformation[0] in self.reload_transformations
                 and self.reload_transformations[transformation[0]] is False
@@ -219,17 +223,25 @@
 
     def transformation_draw_shapes(self, image: pygame.Surface, appearance) -> pygame.Surface:
         for draw_action in appearance.draw_shapes:
             draw_action[0](image, *draw_action[1])
         self.surface = image
         return image
 
-    def reload_transformations_after(self, transformation_string):
+    def flag_reload_actions_for_transformation_pipeline(self, transformation_string):
+        """Reloads transformations in transformation pipeline with given transformation string.
+        
+        e.g. "scale": reloads everything after scale. Actions before scale are loaded from cache.
+
+        Pipeline:
+        
+        texture, scale, upscale, flip, coloring, transparency, write_text, draw_images, draw_shapes, rotate
+
+        """
         reload = False
         for transformation in self.transformations_pipeline:
             if transformation[0] == transformation_string or transformation_string == "all":
                 reload = True  # reload image action
             if reload:
-                self.reload_transformations[transformation[0]] = True  # reload all actions after image action
+                self.reload_transformations[transformation[0]] = True  # reload all actions starting with image action
         if self.appearance.parent:
-            self.appearance.dirty = 1
-            self.appearance.parent.dirty = 1
+            self.appearance.parent.dirty = 1
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/appearances/shape_costume.py` & `miniworldmaker-2.9.0.0/miniworldmaker/appearances/shape_costume.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 
 
 class ShapeCostume(costume.Costume):
     def __init__(self, token):
         super().__init__(token)
         self.set_image((0, 0, 0, 0))
         
-    def after_init(self):
-        super().after_init()
-
     def _set_token_default_values(self):
         self._info_overlay = False
         self._is_rotatable = True
         self.is_scaled = True
         self.is_upscaled = False
         self.is_filled = True
         self.fill_color = (255, 255, 255, 50)
@@ -30,15 +27,15 @@
         return pygame.draw.circle, [
             (self.parent.size[0] / 2, self.parent.size[0] / 2),
             self.parent.radius,
             self.border,
         ]
 
     def _update_draw_shape(self):
-        self.parent.size = (self.parent.radius * 2, self.parent.radius * 2)
+        self.parent.position_manager.size = (self.parent.radius * 2, self.parent.radius * 2)
         super()._update_draw_shape()
 
 
 class EllipseCostume(ShapeCostume):
     def _inner_shape(self):
         return pygame.draw.ellipse, [pygame.Rect(0, 0, self.parent.size[0], self.parent.size[1]), 0]
 
@@ -63,24 +60,22 @@
             math.radians(self.parent.end_angle),
             1,
         ]
 
 
 class LineCostume(ShapeCostume):
     def __init__(self, token):
+        self.local_start_position, self.local_end_position = (0,0), (0,0)
         super().__init__(token)
-        self.local_start_position, self.local_end_position = 0, 0
-        self._update_draw_shape()
-        # set in update_draw_shape
-
+        
     def _update_draw_shape(self):
         super()._update_draw_shape()
-        box = self.parent.get_bounding_box()
-        width, height = box[2], box[3]
-        self.parent.size = (width, height)
+        box = self.get_bounding_box()
+        self.parent.topleft = box.topleft
+        self.parent.size = (box.width, box.height) 
         # mod_start: Start of line
         _x_start = self.parent.start_position[0] - box.topleft[0] - self.border
         _y_start = self.parent.start_position[1] - box.topleft[1] - self.border
         self.local_start_position = (_x_start, _y_start)
         # mod end: End of line
         _x_end = self.parent.end_position[0] - box.topleft[0] - self.border
         _y_end = self.parent.end_position[1] - box.topleft[1] - self.border
@@ -88,14 +83,24 @@
 
     def _inner_shape(self):
         return pygame.draw.line, [self.local_start_position, self.local_end_position, 0]
 
     def _outer_shape(self):
         return pygame.draw.line, [self.local_start_position, self.local_end_position, self.border]
 
+    def get_bounding_box(self):
+        width = abs(self.parent.start_position[0] - self.parent.end_position[0]) + 2 * self.border
+        height = abs(self.parent.start_position[1] - self.parent.end_position[1]) + 2 * self.border
+        box = pygame.Rect(
+            min(self.parent.start_position[0], self.parent.end_position[0]) - self.border,
+            min(self.parent.start_position[1], self.parent.end_position[1]) - self.border,
+            width,
+            height,
+        )
+        return box
 
 class RectangleCostume(ShapeCostume):
     def _inner_shape(self):
         return pygame.draw.rect, [pygame.Rect(0, 0, self.token.size[0], self.token.size[1]), 0]
 
     def _outer_shape(self):
         return pygame.draw.rect, [pygame.Rect(0, 0, self.token.size[0], self.token.size[1]), self.border]
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/appearances/text_costume.py` & `miniworldmaker-2.9.0.0/miniworldmaker/appearances/text_costume.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,23 +11,24 @@
     def _set_token_default_values(self):
         self.fill_color = (255, 255, 255, 255)
         self.border = 0
         self.is_rotatable = True
         self.border_color = (100, 100, 100, 255)
         self.border = 0
         
-    
     def _inner_shape(self):
         return None
 
     def _outer_shape(self):
         return pygame.draw.rect, [pygame.Rect(0, 0, self.parent.size[0], self.parent.size[1]), self.border]
 
     def _update_draw_shape(self):
         super()._update_draw_shape()
         """Sets self.size by costume.font_size"""
         if not self.token.board.tokens_fixed_size:
-            self.token.set_size((self.get_text_width(), self.font_size))
+            self.token.position_manager.set_size((self.get_text_width(), self.font_size))
         if self.board.tokens_fixed_size:
-            self.font_size = 0
-            while self.get_text_width() < self.token.size[0] and self.font_size < self.token.size[1]:
-                self.font_size += 1
+            _font_size = 0
+            self.font_manager.set_font_size(_font_size, update = False)
+            while self.font_manager.get_text_width() < self.token.size[0] and self.font_size < self.token.size[1]:
+                _font_size += 1
+                self.font_manager.set_font_size(_font_size, update = False)
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/base/app.py` & `miniworldmaker-2.9.0.0/miniworldmaker/base/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         self.window.recalculate_dimensions()
         self.window.display_update()
         image_manager.ImageManager.cache_images_in_image_folder()
 
     def start_mainloop(self):
         self._mainloop_started = True
         self.board.dirty = 1
-        self.board.background.dirty = 1
+        self.board.background.set_dirty("all", 2)
         while not self._quit:
             self._update()
         pygame.display.quit()
         sys.exit(self._exit_code)
 
     def _update(self):
         """
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/base/container_manager.py` & `miniworldmaker-2.9.0.0/miniworldmaker/base/container_manager.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/base/event_manager.py` & `miniworldmaker-2.9.0.0/miniworldmaker/base/event_manager.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/base/file_manager.py` & `miniworldmaker-2.9.0.0/miniworldmaker/base/file_manager.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/base/sound_manager.py` & `miniworldmaker-2.9.0.0/miniworldmaker/base/sound_manager.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/base/window.py` & `miniworldmaker-2.9.0.0/miniworldmaker/base/window.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/board_positions/board_direction.py` & `miniworldmaker-2.9.0.0/miniworldmaker/board_positions/board_direction.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,25 +25,31 @@
             # tuple with two points
             _dir_obj = cls.from_two_points(direction[0], direction[1])
         elif type(direction) == Direction:
             return direction
         else:
             raise MoveInDirectionTypeError(direction)
         return _dir_obj
-
+    
     @classmethod
-    def create_from_token(cls, token : "token_mod.Token", direction : Union[int, float, "Direction"]) -> "Direction":
+    def from_token_towards_direction(cls, token, direction):
         if type(direction) in [int, str]:
             direction = cls._value_from_token_to_direction(token, direction)
-            _dir_obj = cls(direction)
-        elif type(direction) == tuple:
-            _dir_obj = cls.from_two_points(token.position, (direction[0], direction[1]))
-        else:
-            raise MoveInDirectionTypeError(direction)
-        return _dir_obj
+            return cls(direction)
+        elif isinstance(direction, Direction):
+            return direction
+        
+    @classmethod
+    def from_token_to_position(cls, t1: "token_mod.Token", pos = Union[tuple, "board_position.Position"]):
+        t1center = board_position.Position.create(t1.center)
+        return Direction.from_two_points(t1center, pos)
+        
+    @classmethod
+    def from_tokens(cls, t1 : "token_mod.Token", t2 : "token_mod.Token"):
+        return Direction.from_token_to_position(t1, t2.center)
 
     @classmethod
     def from_two_points(cls, pos1: Union[tuple, "board_position.BoardPosition"], pos2 : Union[tuple, "board_position.BoardPosition"]) -> "Direction":
         x = pos2[0] - pos1[0]
         y = pos2[1] - pos1[1]
         if x != 0:
             m = y / x
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/board_positions/board_position.py` & `miniworldmaker-2.9.0.0/miniworldmaker/board_positions/board_position.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 import miniworldmaker.base.app as app
 import miniworldmaker.board_positions.board_vector as board_vector
 from typing import Union, Tuple
 import numpy as np
 import math
 
 
-class Position(collections.namedtuple('Position', ['x', 'y'])):
+class Position(collections.namedtuple("Position", ["x", "y"])):
     """
     A Position Object represents a position on a Board.
 
     As a subclass of namedtuple, Position is for
-    performance reasons not mutable. 
+    performance reasons not mutable.
 
     On a tiled board, the Position does not describe pixels
     but tiles coordinates.
     """
 
     def __str__(self):
         return str("Pos(" + str(round(self.x, 3)) + "," + str(round(self.y, 3)) + ")")
@@ -111,23 +111,35 @@
     def to_int(self):
         """
         Transforms both coordinates of a position to integers
         :return: Tuple (x,y) , x and y are integers.
         """
         return (int(self.x), int(self.y))
 
-    def is_close(self, other : Union["Position", Tuple], error : int =1):
+    def is_close(self, other: Union["Position", Tuple], error: int = 1):
         """
         Is a position close to another position
 
         :param other: The other position
         :param error: The error for both coordinates.
         :return: If x-other.x < error and y-other.y < error, is_close() returns True
         """
         if abs(self.x - other[0]) < error and abs(self.y - other[1] < error):
             return True
         return False
 
+    def up(self, value):
+        return self.__class__(self.x, self.y - value)
+
+    def down(self, value):
+        return self.__class__(self.x, self.y + value)
+
+    def left(self, value):
+        return self.__class__(self.x - value, self.y)
+
+    def right(self, value):
+        return self.__class__(self.x + value, self.y)
+
 
 class BoardPosition(Position):
     # legacy
     pass
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/board_positions/board_rect.py` & `miniworldmaker-2.9.0.0/miniworldmaker/board_positions/board_rect.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,12 +23,12 @@
         else:
             new_rect = pygame.Rect(0, 0, dimensions[0], dimensions[1])
         new_rect.topleft = position
         return new_rect
 
     @classmethod
     def from_token(cls, token):
-        return Rect.create(token.rect)
+        return Rect.create(token.get_global_rect())
 
     @property
     def board(self):
         return app.App.board
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/board_positions/board_vector.py` & `miniworldmaker-2.9.0.0/miniworldmaker/board_positions/board_vector.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/board_positions/hex_elements.py` & `miniworldmaker-2.9.0.0/miniworldmaker/board_positions/hex_elements.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/board_positions/tile_elements.py` & `miniworldmaker-2.9.0.0/miniworldmaker/board_positions/tile_elements.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/boards/board.py` & `miniworldmaker-2.9.0.0/miniworldmaker/boards/board.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Type, Union, Tuple
+from typing import Type, Union, Tuple, ValuesView
 
 import pygame
 
 import miniworldmaker.appearances.appearance as appearance
 import miniworldmaker.appearances.background as background
 import miniworldmaker.board_positions.board_position as board_position
 import miniworldmaker.boards.board_base as board_base
@@ -214,56 +214,103 @@
         """Gets height of board in pixels.
 
         (for tiledboard: rows * tile_size)
         """
         return self.container_height
 
     @property
-    def rows(self) -> int:
-        """The number of rows"""
-        return self._rows
+    def boundary_x(self) -> int:
+        """The x-boundary (defaults to view_size)"""
+        return self.camera.boundary_x
 
-    @rows.setter
-    def rows(self, value: int):
-        self._rows = value
-        self.app.window.dirty = 1
-        self.background.reload_transformations_after("all")
+    @boundary_x.setter
+    def boundary_x(self, value: int):
+        self.camera.boundary_x = value
+
+    @property
+    def boundary_y(self) -> int:
+        """The y-boundary (defaults to view_size)"""
+        return self.camera.boundary_y
+
+    @boundary_y.setter
+    def boundary_y(self, value: int):
+        self.camera.boundary_y = value
+
+    @property
+    def viewport_width(self) -> int:
+        return self.camera.viewport_width
+
+    @viewport_width.setter
+    def viewport_width(self, value: int):
+        self.camera.viewport_width = value
+
+    @property
+    def viewport_height(self) -> int:
+        """The y-boundary (defaults to view_size)"""
+        return self.camera.viewport_height
+
+    @viewport_height.setter
+    def viewport_height(self, value: int):
+        self.camera.viewport_height = value
 
     @property
     def columns(self) -> int:
-        """The number of columns"""
-        return self._columns
+        return self.camera.viewport_width
 
     @columns.setter
     def columns(self, value: int):
-        self._columns = value
-        self.app.window.dirty = 1
-        self.background.reload_transformations_after("all")
+        self.camera.viewport_width = value
+        self.boundary_x = value
+ 
+    @property
+    def rows(self) -> int:
+        return self.camera.viewport_height
+
+    @rows.setter
+    def rows(self, value: int):
+        self.viewport_height = value
+        self.boundary_y = value     
 
     @property
+    def camera_x(self):
+        return self.camera.x
+    
+    @camera_x.setter
+    def camera_x(self, value):
+        self.camera.x = value
+        
+    @property
+    def camera_y(self):
+        return self.camera.y
+    
+    @camera_y.setter
+    def camera_y(self, value):
+        self.camera.y = value
+        
+    @property
     def size(self) -> tuple:
         """Set the size of board
 
         Examples:
 
           Create a board with 800 columns and 600 rows:
 
           .. code-block:: python
 
             board = miniworldmaker.PixelBoard()
             board.size = (800, 600)
         """
-        return self.columns, self.rows
+        return self.boundary_x, self.boundary_y
 
     @size.setter
     def size(self, value: tuple):
-        self.columns = value[0]
-        self.rows = value[1]
-        self.background.reload_transformations_after("all")
-        self.app.window.dirty = 1
+        self.boundary_x = value[0]
+        self.boundary_y = value[1]
+        self.viewport_width = value[0]
+        self.viewport_height = value[1]
 
     @property
     def default_fill_color(self):
         """Set default fill color for borders and lines"""
         return self._default_fill_color
 
     @default_fill_color.setter
@@ -672,17 +719,17 @@
             .. code-block:: python
 
               def on_sensing_collision_with_pipe(self, other, info):
                   self.board.is_running = False
                   self.board.reset()
         """
         self.app.event_manager.event_queue.clear()
-        self.clean()
         for background in self.backgrounds:
-            self.remove_background(background)
+            self.backgrounds_manager.remove_appearance(background)
+        self.clean()
         if hasattr(self, "on_setup"):
             self.on_setup()
 
 
     def switch_board(self, new_board: "board_base.BaseBoard"):
         """Switches to another board
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/boards/board_base.py` & `miniworldmaker-2.9.0.0/miniworldmaker/boards/board_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,49 +21,53 @@
 import miniworldmaker.tokens.token as token_module
 import miniworldmaker.tools.board_inspection as board_inspection
 from miniworldmaker.exceptions.miniworldmaker_exception import (
     BoardArgumentsError,
     BoardInstanceError,
     NotImplementedOrRegisteredError,
 )
+from miniworldmaker.boards.board_manager import board_camera_manager
+from abc import ABC, abstractmethod
+import asyncio
 
-
-class BaseBoard(container.Container):
+class BaseBoard(container.Container, ABC):
     subclasses = None
 
     def __init__(
             self,
-            columns: Union[int, Tuple[int]] = 400,
-            rows: int = 400,
+            view_x: Union[int, Tuple[int]] = 400,
+            view_y: int = 400,
             tile_size: int = 1,
     ):
-        if self.__class__ == BaseBoard:
-            raise BoardInstanceError()
-        if type(columns) != int or type(rows) != int:
-            if type(columns) == tuple:
-                size = columns
-                columns = size[0]
-                rows = size[1]
+        #if self.__class__ == BaseBoard:
+        #    raise BoardInstanceError()
+        if type(view_x) != int or type(view_y) != int:
+            # If first param is tuple, generate board from tuple-data
+            if type(view_x) == tuple:
+                size = view_x
+                view_x = size[0]
+                view_y = size[1]
             else:
-                raise BoardArgumentsError(columns, rows)
-        self._columns, self._rows, self._tile_size = columns, rows, tile_size
+                raise BoardArgumentsError(view_x, view_y)
+        self._tile_size = tile_size
+        self.camera = self._get_camera_manager_class()(view_x, view_y, self)
         self._tokens = pygame.sprite.LayeredDirty()
         self.event_manager: event_manager.BoardEventHandler = event_manager.BoardEventHandler(self)
         super().__init__()
         self.backgrounds_manager: "backgrounds_manager.BackgroundsManager" = backgrounds_manager.BackgroundsManager(
             self
         )
         self.mouse_manager: "mouse_manager.BoardMouseManager" = mouse_manager.BoardMouseManager(self)
         self.ask: "ask.Ask" = ask.Ask(self)
         pygame.init()
         self._is_setup: bool = False
         self._fps: int = 60
         self._key_pressed: bool = False
         self._animated: bool = False
-        self._orientation: int = 0
+        self._orientation: int = 0 
         self._static: bool = False
         self._speed: int = 1  # All tokens are acting on n'th frame with n = self.speed
         self._default_is_filled = False
         self._default_fill_color = None
         self._default_border_color = None
         self._default_border = None
         self.is_running: bool = True
@@ -77,21 +81,26 @@
         self.background.update()
         self.collision_manager: "coll_manager.BoardCollisionHandler" = coll_manager.BoardCollisionHandler(self)
         self.timed_objects: list = []
         self.app.event_manager.send_event_to_containers("setup", self)
         self.dynamic_tokens = set()
         self._registered_methods = []
         self.tokens_fixed_size = False
-        self._container_width = self.columns * self.tile_size
-        self._container_height = self.rows * self.tile_size
+        self._container_width = self.camera.get_viewport_width()
+        self._container_height = self.camera.get_viewport_height() 
+        
 
     def get_token_connector(self, token) -> token_connector.TokenConnector:
         return self._get_token_connector_class()(self, token)
 
     @staticmethod
+    def _get_camera_manager_class():
+        return board_camera_manager.CameraManager
+    
+    @staticmethod
     def _get_token_connector_class():
         return token_connector.TokenConnector
 
     def load_board_from_db(self, file: str):
         """
         Loads a sqlite db file.
         """
@@ -129,22 +138,22 @@
         return "{0} with {1} columns and {2} rows".format(self.__class__.__name__, self.columns, self.rows)
 
     @property
     def container_width(self) -> int:
         """
         The width of the container
         """
-        return self.columns * self.tile_size
+        return self.camera.get_viewport_width_in_pixels()
 
     @property
     def container_height(self) -> int:
         """
         The height of the container
         """
-        return self.rows * self.tile_size
+        return self.camera.get_viewport_height_in_pixels()
 
     @property
     def has_background(self) -> bool:
         return self.backgrounds_manager.has_background
 
     @property
     def window(self) -> "app.App":
@@ -219,30 +228,14 @@
         return self.get_tokens_from_pixel(position)
 
     @property
     def image(self) -> pygame.Surface:
         """The current displayed image"""
         return self.backgrounds_manager.image
 
-    def remove_tokens_from_rect(self, rect, token_class=None, exclude=None):
-        """Removes all tokens in an area
-
-        Args:
-            rect: A rectangle or a tuple (which is automated converted to a rectangle with tile_size).
-            token_class: The class of the tokens which should be removed
-            exclude: A token which should not be removed e.g. the actor itself
-
-        Returns: all tokens in the area
-        """
-        rect = board_rect.Rect(self).create(rect)
-        tokens = self.get_tokens_at_rect(rect)
-        for token in tokens:
-            if token is not None:
-                [token.remove() for token in BaseBoard.filter_actor_list(tokens, token_class)]
-
     def repaint(self):
         self.background.repaint()  # called 1/frame in container.repaint()
 
     def update(self):
         # This is the board-mainloop()
         # Called in miniworldwindow.update as container.update()
         if self.is_running or self.frame == 0:
@@ -287,17 +280,14 @@
             data: The data of the event (e.g. ["S","s"], (155,3), ...
         """
         self.event_manager.handle_event(event, data)
 
     def find_colors(self, rect, color, threshold=(20, 20, 20, 20)):
         return self.backgrounds_manager.find_colors(rect, color, threshold)
 
-    def _update_event_handling(self):
-        self.event_manager.update_event_handling()
-
     def register(self, method: callable) -> callable:
         """
         Used as decorator
         e.g.
         @register
         def method...
         """
@@ -309,20 +299,14 @@
     def unregister(self, method: callable):
         self._registered_methods.remove(method)
         board_inspection.BoardInspection(self).unbind_method(method)
         
     def add_container(self, container, dock, size=None):
         return self.app.container_manager.add_container(container, dock, size)
 
-    def get_tokens_by_class_name(self, classname: str):
-        return [token for token in self._tokens if token.__class__.__name__ == classname]
-
-    def get_tokens_by_class(self, classname: str):
-        return [token for token in self._tokens if isinstance(token, classname)]
-
     def on_started(self):
         """The on_started method is executed after starting the board.
         Afterwards the individual lines are executed step by step with some delay (depending on board.speed).
 
         Examples:
 
         Registering an on_started-Method
@@ -384,8 +368,8 @@
     @tile_size.setter
     def tile_size(self, value: int):
         self.set_tile_size(value)
 
     def set_tile_size(self, value):
         self._tile_size = value
         self.app.window.dirty = 1
-        self.background.reload_transformations_after("all")
+        self.background.set_dirty("all", background.Background.RELOAD_ACTUAL_IMAGE)
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/boards/board_manager/board_collision_manager.py` & `miniworldmaker-2.9.0.0/miniworldmaker/boards/board_manager/board_collision_manager.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/boards/board_manager/board_event_manager.py` & `miniworldmaker-2.9.0.0/miniworldmaker/boards/board_manager/board_event_manager.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/boards/board_manager/board_mouse_manager.py` & `miniworldmaker-2.9.0.0/miniworldmaker/boards/board_manager/board_mouse_manager.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/boards/data/db_manager.py` & `miniworldmaker-2.9.0.0/miniworldmaker/boards/data/db_manager.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/boards/data/export_factory.py` & `miniworldmaker-2.9.0.0/miniworldmaker/boards/data/export_factory.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/boards/data/import_factory.py` & `miniworldmaker-2.9.0.0/miniworldmaker/boards/data/import_factory.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/boards/hex_board.py` & `miniworldmaker-2.9.0.0/miniworldmaker/boards/hex_board.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,32 @@
 
 import miniworldmaker.board_positions.board_position as board_position
 import miniworldmaker.board_positions.hex_elements as hex_elements
 import miniworldmaker.board_positions.tile_factory as tile_factory
 import miniworldmaker.boards.tiled_board as tiled_board
 import miniworldmaker.boards.token_connectors.hex_board_connector as hex_board_connector
 from miniworldmaker.exceptions import miniworldmaker_exception
-
+from miniworldmaker.boards.board_manager import board_camera_manager
 
 class HexBoard(tiled_board.TiledBoard):
     """
     A hexboard is a board that consists of hexagonal tiles.
 
     Each token can be positioned either at a tile, at an edge or at a corner.
 
     
     """
-    def __init__(self, columns: int = 20, rows: int = 16, empty=False):
-        super().__init__(columns, rows, empty)
+    def __init__(self, view_x: int = 20, view_y: int = 16, empty=False):
+        super().__init__(view_x, view_y, empty)
         self.lookup_table = []
 
+    @staticmethod
+    def _get_camera_manager_class():
+        return board_camera_manager.HexCameraManager
+    
     def _get_tile_factory(self):
         return tile_factory.HexTileFactory()
 
     def _templates(self):
         return hex_elements.HexTile, hex_elements.HexEdge, hex_elements.HexCorner
 
     def get_type(self, position):
@@ -157,16 +161,7 @@
     @staticmethod
     def _get_token_connector_class():
         return hex_board_connector.HexBoardConnector
 
     def set_tile_size(self, value):
         super().set_tile_size(value)
 
-    @property
-    def container_width(self) -> int:
-        """The width of the container"""
-        return self.columns * self.get_tile_width() + 1 / 2 * self.get_tile_width()
-
-    @property
-    def container_height(self) -> int:
-        """The height of the container"""
-        return self.rows * self.get_tile_height() * 3 / 4 + self.get_tile_height() / 4
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/boards/physics_board.py` & `miniworldmaker-2.9.0.0/miniworldmaker/boards/physics_board.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/boards/tiled_board.py` & `miniworldmaker-2.9.0.0/miniworldmaker/boards/tiled_board.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import miniworldmaker.board_positions.board_position as board_position
 import miniworldmaker.board_positions.tile_elements as tile_elements
 import miniworldmaker.board_positions.tile_factory as tile_factory
 import miniworldmaker.boards.board as board
 import miniworldmaker.boards.token_connectors.tiled_board_connector as tiled_board_connector
 from miniworldmaker.exceptions import miniworldmaker_exception
 from miniworldmaker.exceptions.miniworldmaker_exception import TiledBoardTooBigError
-
+from miniworldmaker.boards.board_manager import board_camera_manager
 
 class TiledBoard(board.Board):
     """
     A TiledBoard is a Board where each Token is placed in one Tile.
 
     With Tiled Board, you can realize RPGs and Boardgames.
 
@@ -52,26 +52,26 @@
             board.run()
 
 
         .. image:: /_images/tilecorneredge.png
             :alt: Placing Tokens on a Tile, on a Corner or in a Edge
     """
 
-    def __init__(self, columns: int = 20, rows: int = 16, empty=False):
+    def __init__(self, view_x: int = 20, view_y: int = 16, empty=False):
         """Initializes the TiledBoard
 
         Args:
-            columns: The number of columns
-            rows: The number of rows
+            view_x: The number of columns
+            view_y: The number of rows
             empty: The board has no tiles, edges, and corners. They must be created manually
         """
         self.default_token_speed: int = 1
-        if columns > 1000 or rows > 1000:
-            raise TiledBoardTooBigError(columns, rows, 40)
-        super().__init__(columns=columns, rows=rows)
+        if view_x > 1000 or view_y > 1000:
+            raise TiledBoardTooBigError(view_x, view_y, 40)
+        super().__init__(view_x=view_x, view_y=view_y)
         self.tile_factory = self._get_tile_factory()
         self.tile_size = 40
         self.speed = 20
         self.dynamic_tokens_dict: defaultdict = defaultdict(list)  # the dict is regularly updated
         self.dynamic_tokens: set = set()  # Set with all dynamic actors
         self.static_tokens_dict: defaultdict = defaultdict(list)
         self.tokens_fixed_size = True
@@ -136,20 +136,27 @@
 
                 board.run()
         """
         self.tiles.clear()
         self.corners.clear()
         self.edges.clear()
 
+    @staticmethod
+    def _get_camera_manager_class():
+        return board_camera_manager.TiledCameraManager
+    
     def setup_board(self):
         """In this method, corners and edges are created.
         """
         if not self.empty:
+            print("setup tiles")
             self._setup_tiles()
+            print("setup corners")
             self._setup_corners()
+            print("setup edges")
             self._setup_edges()
 
     def _templates(self):
         """Returns Classes for Tile, Edge and Corner
         """
         return tile_elements.Tile, tile_elements.Edge, tile_elements.Corner
 
@@ -179,16 +186,16 @@
         else:
             self.edges[edge_pos].merge(edge)
         return self.edges[edge_pos]
 
     def _setup_tiles(self):
         """Adds Tile to Board for each BoardPosition
         """
-        for x in range(self.columns):
-            for y in range(self.rows):
+        for x in range(self.boundary_x):
+            for y in range(self.boundary_y):
                 self.add_tile_to_board((x, y))
 
     def _setup_corners(self):
         """Add all Corner to Board for each Tile.
 
         Merges identical corners for different Tiles
         """
@@ -459,17 +466,7 @@
             return False
 
     def to_pixel(self, position, size=(0, 0), origin=(0, 0)):
         """Converts BoardPosition to pixel coordinates"""
         x = position[0] * self.tile_size + origin[0]
         y = position[1] * self.tile_size + origin[1]
         return board_position.Position(x, y)
-    
-    @property
-    def container_width(self) -> int:
-        """The width of the container"""
-        return self.columns * self.tile_size
-
-    @property
-    def container_height(self) -> int:
-        """The height of the container"""
-        return self.rows * self.tile_size
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/boards/token_connectors/hex_board_connector.py` & `miniworldmaker-2.9.0.0/miniworldmaker/boards/token_connectors/hex_board_connector.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/boards/token_connectors/physics_board_connector.py` & `miniworldmaker-2.9.0.0/miniworldmaker/boards/token_connectors/physics_board_connector.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/boards/token_connectors/pixel_board_connector.py` & `miniworldmaker-2.9.0.0/miniworldmaker/boards/token_connectors/pixel_board_connector.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/boards/token_connectors/tiled_board_connector.py` & `miniworldmaker-2.9.0.0/miniworldmaker/boards/token_connectors/tiled_board_connector.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,12 +33,10 @@
             and self.token in self.board.static_tokens_dict[self.token.position]
         ):
             self.board.static_tokens_dict[self.token.position].remove(self.token)
 
     def set_static(self, value):
         super().set_static(value)
         if self.token._static:
-            _token_connector = self.board.get_token_connector(self.token)
-            _token_connector.add_static_token()
+            self.add_static_token()
         else:
-            _token_connector = self.board.get_token_connector(self.token)
-            _token_connector.remove_static_token()
+            self.remove_static_token()
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/boards/token_connectors/token_connector.py` & `miniworldmaker-2.9.0.0/miniworldmaker/boards/token_connectors/token_connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,27 +40,29 @@
         return None
 
     @staticmethod
     def get_board_sensor_class():
         return None
 
     def add_token_to_board(self, position):
+        self.board.camera.clear_camera_cache()
         self.board.tokens.add(self.token)
         self.set_static(self.token.static)
-        self.token.costume.reload_transformations_after("all")
+        self.token.costume.set_dirty("all", costume.Costume.LOAD_NEW_IMAGE)
         if hasattr(self.token, "on_setup"):
             self.token.on_setup()
             self.board.background.reload_costumes_queue.append(self.token)
         if not self.token.static:
             self.token.board.event_manager.register_events_for_token(self.token)
       
     def remove_token_from_board(self, token):
         """
         Implemented in subclasses
         """
+        self.board.camera.clear_camera_cache()
         self.board.event_manager.unregister_instance(token)
         if self in self.board.background.reload_costumes_queue:
             self.board.background.reload_costumes_queue.remove(self)
         if not self.token._static:
             _token_connector = self.board.get_token_connector(self.token)
             _token_connector.remove_dynamic_token()
         self.board.tokens.remove(token)
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/containers/actionbar.py` & `miniworldmaker-2.9.0.0/miniworldmaker/containers/actionbar.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/containers/color_toolbar.py` & `miniworldmaker-2.9.0.0/miniworldmaker/containers/color_toolbar.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/containers/console.py` & `miniworldmaker-2.9.0.0/miniworldmaker/containers/console.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/containers/container.py` & `miniworldmaker-2.9.0.0/miniworldmaker/containers/container.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/containers/event_console.py` & `miniworldmaker-2.9.0.0/miniworldmaker/containers/event_console.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/containers/inspect_actor_toolbar.py` & `miniworldmaker-2.9.0.0/miniworldmaker/containers/inspect_actor_toolbar.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/containers/level_designer_toolbar.py` & `miniworldmaker-2.9.0.0/miniworldmaker/containers/level_designer_toolbar.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/containers/toolbar.py` & `miniworldmaker-2.9.0.0/miniworldmaker/containers/toolbar.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/containers/widgets.py` & `miniworldmaker-2.9.0.0/miniworldmaker/containers/widgets.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/dialogs/ask.py` & `miniworldmaker-2.9.0.0/miniworldmaker/dialogs/ask.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/exceptions/miniworldmaker_exception.py` & `miniworldmaker-2.9.0.0/miniworldmaker/exceptions/miniworldmaker_exception.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/resources/down.png` & `miniworldmaker-2.9.0.0/miniworldmaker/resources/down.png`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/resources/left.png` & `miniworldmaker-2.9.0.0/miniworldmaker/resources/left.png`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/resources/logo_big.png` & `miniworldmaker-2.9.0.0/miniworldmaker/resources/logo_big.png`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/resources/logo_small.png` & `miniworldmaker-2.9.0.0/miniworldmaker/resources/logo_small.png`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/resources/logo_small_32.png` & `miniworldmaker-2.9.0.0/miniworldmaker/resources/logo_small_32.png`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/resources/question.png` & `miniworldmaker-2.9.0.0/miniworldmaker/resources/question.png`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/resources/right.png` & `miniworldmaker-2.9.0.0/miniworldmaker/resources/right.png`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/resources/up.png` & `miniworldmaker-2.9.0.0/miniworldmaker/resources/up.png`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/tokens/number_token.py` & `miniworldmaker-2.9.0.0/miniworldmaker/tokens/number_token.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import miniworldmaker.tokens.text_token as text_token
-
+from miniworldmaker.appearances import costume
 
 class Number(text_token.TextToken):
     """
     A number token shows a Number.
 
     You have to set the size of the token with self.size() manually so that
     the complete text can be seen.
@@ -71,14 +71,14 @@
         Examples:
             
             Gets the number stored in the NumberToken::
             
                 number = self.number_token.get_number()
             
         """
-        self.costume.reload_transformations_after("text changed")
+        self.costume.set_dirty("text changed", costume.Costume.LOAD_NEW_IMAGE)
         return int(self.costume.text)
 
 
 class NumberToken(Number):
     """Alias for legacy code"""
     pass
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/tokens/physics/token_physics.py` & `miniworldmaker-2.9.0.0/miniworldmaker/tokens/physics/token_physics.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,27 +60,27 @@
         """
         if not hasattr(other, "physics"):
             raise TypeError("Other token has no attribute physics")
         my_body = self._body
         other_body = other.physics._body
         pj = pymunk.PinJoint(my_body, other_body, (0, 0), (0, 0))
         self.board.space.add(pj)
-        return self.token.position, other.position
+        return self.token.position_manager.get_position(), other.position
 
     def join(self, other: "token.Token"):
         """joins two tokens at their center points
         """
         if not hasattr(other, "physics"):
             raise TypeError("Other token has no attribute physics")
         my_body = self._body
         other_body = other.physics._body
         pj = pymunk.PinJoint(my_body, other_body, (0, 0), (0, 0))
         self.joints.append(pj)
         self.board.space.add(pj)
-        return self.token.position, other.position
+        return self.token.position_manager.get_position(), other.position
 
     def remove_join(self, other: "token.Token"):
         """Remove a joint between two tokens.
 
         Removes a joint between two tokens, if a joint exists.
 
         Examples:
@@ -156,28 +156,28 @@
                                            )
         elif self.shape_type.lower() == "circle":
             shape = pymunk.Circle(self._body,
                                   self.size[0] * self.token.width / 2,
                                   (0, 0),
                                   )
         elif self.shape_type.lower() == "line":
-            shift_x = self.token.size[0] / 2 + self.token.position[0]
-            shift_y = self.token.size[1] / 2 + self.token.position[1]
+            shift_x = self.token.size[0] / 2 + self.token.position_manager.get_position()[0]
+            shift_y = self.token.size[1] / 2 + self.token.position_manager.get_position()[1]
             start = pymunk.pygame_util.from_pygame(
                 (self.token.start_position[0] - shift_x, self.token.start_position[1] - shift_y),
                 self.token.board.image)
             end = pymunk.pygame_util.from_pygame(
                 (self.token.end_position[0] - shift_x, self.token.end_position[1] - shift_y), self.token.board.image)
             shape = pymunk.Segment(self._body, start, end, self.token.border)
         else:
             raise AttributeError("No shape set!")
         return shape
 
     def _setup_physics_model(self):
-        if self.dirty and self.token.position:  # if token is on board
+        if self.dirty and self.token.position_manager.get_position():  # if token is on board
             # create body
             self.has_physics = False
             self._body = pymunk_engine.Body(body_type=self.body_type)
             self._set_pymunk_position()
             self._set_pymunk_direction()
             self._body.size = (self.size[0] * self.token.width, self.size[1] * self.token.height)
             # disable velocity for tokens if token has no gravity
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/tokens/positions/token_hex_position_manager.py` & `miniworldmaker-2.9.0.0/miniworldmaker/tokens/positions/token_tiled_position_manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,89 @@
+import math
+from typing import Tuple, Union
+
 import pygame
 
-import miniworldmaker.board_positions.board_position as board_position
-import miniworldmaker.board_positions.hex_elements as hex_elements
-import miniworldmaker.tokens.positions.token_tiled_position_manager as tiled_positionmanager
-import miniworldmaker.board_positions.board_direction as board_direction
-from miniworldmaker.exceptions.miniworldmaker_exception import MoveInDirectionTypeError
-from typing import Union
+import miniworldmaker.board_positions.tile_elements as tile_elements
+import miniworldmaker.tokens.positions.token_position_manager as token_position_manager
+from miniworldmaker.board_positions import board_position
+from miniworldmaker.board_positions import board_direction
+from miniworldmaker.appearances import costume
 
 
-class HexBoardPositionManager(tiled_positionmanager.TiledBoardPositionManager):
+class TiledBoardPositionManager(token_position_manager.TokenPositionManager):
     def __init__(self, token, board):
         super().__init__(token, board)
-        self._position = hex_elements.CubeCoord.create((0, 0))
+        self._scaled_size = (1, 1)
 
-    def get_rect(self):
-        if self.token.costume:
-            rect = self.token.costume.image.get_rect()
-        else:
-            rect = pygame.Rect(0, 0, self.token.size[0], self.token.size[1])
+    def get_global_rect(self):
+        rect = super().get_global_rect()
         if self.token.board.is_tile(self.token.position):
-            topleft = hex_elements.HexTile.from_position(self.token.position).to_pixel()
-            if self._scaled_size != (1, 1):
-                shift_x = (self.size[0] - self.token.board.get_tile_width()) / 2
-                shift_y = (self.size[1] - self.token.board.get_tile_height()) / 2
-                pos = board_position.Position(shift_x, shift_y)
-                topleft = topleft - pos
-            rect.topleft = topleft
-
+            rect.topleft = tile_elements.Tile.from_position(self.token.position).to_pixel()
         if self.token.board.is_corner(self.token.position):
-            rect.center = hex_elements.HexCorner.from_position(self.token.position).to_pixel()
+            rect.center = tile_elements.Corner.from_position(self.token.position).to_pixel()
         if self.token.board.is_edge(self.token.position):
-            rect.center = hex_elements.HexEdge.from_position(self.token.position).to_pixel()
+            rect.center = tile_elements.Edge.from_position(self.token.position).to_pixel()
+        return rect
+
+    def get_local_rect(self):
+        rect = self.get_global_rect()
         return rect
 
     @property
     def size(self):
         if self.token.board:
             return (
-                self.token.board.get_tile_width() * self._scaled_size[0] + self.token.board.get_tile_width() // 10,
-                self.token.board.get_tile_height() * self._scaled_size[1],
+                self.token.board.tile_size * self._scaled_size[0],
+                self.token.board.tile_size * self._scaled_size[1],
             )
         else:
             return 0
 
     @size.setter
-    def size(self, value):
+    def size(self, value: Union[int, Tuple]):
         if type(value) == int or type(value) == float:  # convert int to tuple
             value = (value, value)
         self._scaled_size = value
-        self.token.costume.reload_transformations_after("all")
+        self.token.costume.set_dirty("scale", costume.Costume.RELOAD_ACTUAL_IMAGE)
 
-    def get_position(self) -> "hex_elements.CubeCoord":
-        """Position is stores as CubeCoord on HexBoard
+    def point_towards_position(self, destination) -> float:
         """
-        return self._position
-    
+        Token points towards a given position
 
-    def set_position(self, value : Union[tuple, "board_position.BoardPosition"]) -> "hex_elements.CubeCoord":
-        self.last_position = self.position
-        self.last_direction = self.direction
-        self._position = hex_elements.CubeCoord.create(value)
-        if self.last_position != self._position:
-            self.token.dirty = 1
-            if self.token.board:
-                self.token.board.app.event_manager.send_event_to_containers("token_moved", self.token)
-        return self.position
-
-    def set_direction(self, value):
-        self.last_direction = self.direction
-        direction = board_direction.Direction.create(value)
-        self._direction = direction
-        if self.last_direction != self._direction:
-            self.token.costume.reload_transformations_after("all")
-
-    def move_in_direction(self, direction: Union[int, str, "board_position.Position", tuple], distance=1):
-        old_direction = self.token.direction
-        direction = board_direction.Direction.create_from_token(self.token, direction).value
-        self.set_direction(direction)
-        self.move(distance)
-        self.direction = old_direction
-        return self
+        Args:
+            destination: The position to which the actor should pointing
+
+        Returns:
+            The new direction
+
+        """
+        pos = self.token.position
+        x = destination[0] - pos[0]
+        y = destination[1] - pos[1]
+        if x != 0:
+            m = y / x
+            if x < 0:
+                # destination is left
+                self.token.direction = math.degrees(math.atan(m)) - 90
+            else:
+                # destination is right
+                self.token.direction = math.degrees(math.atan(m)) + 90
+            return self.token.direction
+        else:
+            m = 0
+            if destination[1] > self.token.position[1]:
+                self.token.direction = 180
+                return self.token.direction
+            else:
+                self.token.direction = 0
+                return self.token.direction
+
+    def move_towards_position(self, position, distance=1):
+        tkn_center = board_position.Position.create(self.token.position)
+        if tkn_center.is_close(position):
+            return self
+        else:
+            direction = board_direction.Direction.from_two_points(self.token.position, position).value
+            self.set_direction(direction)
+            self.move(distance)
+            return self
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/tokens/positions/token_physics_position_manager.py` & `miniworldmaker-2.9.0.0/miniworldmaker/tokens/positions/token_physics_position_manager.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/tokens/positions/token_pixel_position_manager.py` & `miniworldmaker-2.9.0.0/miniworldmaker/tokens/positions/token_pixel_position_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,36 +5,63 @@
 import miniworldmaker.tokens.positions.token_position_manager as token_positionmanager
 from miniworldmaker.exceptions.miniworldmaker_exception import NoValidBoardPositionError
 
 
 class PixelBoardPositionManager(token_positionmanager.TokenPositionManager):
     def __init__(self, token, board):
         super().__init__(token, board)
-        self.size = (0, 0)
-        self.set_position((0, 0))
-        self.size=(40, 40)
+        self._position = (0, 0)
+        self._size = (40, 40)
 
-    def get_rect(self) -> pygame.Rect:
+    def get_local_rect(self) -> pygame.Rect:
         """Pixelboard-Rects are positioned at center of position
         """
+        # if costume is set, get rect coordinates from costume.
+        _rect = self.get_global_rect()
+        _rect.topleft = self.token.board.camera.get_local_position(_rect)
+        return _rect
+    
+    def get_global_rect(self) -> pygame.Rect:
+        """Pixelboard-Rects are positioned at center of position
+        """
+        # if costume is set, get rect coordinates from costume.
         if self.token.costume:
-            _rect = self.token.costume.image.get_rect()
+            _rect = self.token.costume.get_image().get_rect()
         else:
-            _rect = pygame.Rect(self.position[0], self._position[1], self.token.size[0], self.token.size[1])
-        _rect_center_pos = super().get_position()
-        _rect.center = _rect_center_pos[0], _rect_center_pos[1]
+            _rect = pygame.Rect(0,0 , self.token.size[0], self.token.size[1])
+        _rect_center = self.center
+        # board position without shift is the center position
+        _rect.center = _rect_center
         return _rect
-
+    
     def get_position(self):    
         shift_x = self.size[0] / 2
         shift_y = self.size[1] / 2
         rect_center = super().get_position()
         pos = rect_center[0] - shift_x, rect_center[1] - shift_y
         return board_position.Position.create(pos)
-    
+
+    @property
+    def center_x(self):
+        """x-value of token center-position"""
+        return self._position[0]
+
+    @center_x.setter
+    def center_x(self, value):
+        self.set_center((value, self.center_y))
+
+    @property
+    def center_y(self):
+        """y-value of token center-position"""
+        return self._position[1]
+
+    @center_y.setter
+    def center_y(self, value):
+        self.set_center((self.center_x, value))
+        
     def set_position(self, value):
         """Because Pixelboard-Rects are positioned at center of position, newly created Objects are shifted down right.
 
         """
         if value:
             shift_x = self.size[0] / 2.0
             shift_y = self.size[1] / 2.0
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/tokens/positions/token_position_manager.py` & `miniworldmaker-2.9.0.0/miniworldmaker/tokens/positions/token_position_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,45 +4,54 @@
 
 import pygame
 
 import miniworldmaker.board_positions.board_position as board_position
 import miniworldmaker.board_positions.board_vector as board_vector
 import miniworldmaker.board_positions.board_direction as board_direction
 import miniworldmaker.board_positions.board_rect as board_rect
-from miniworldmaker.exceptions.miniworldmaker_exception import MoveInDirectionTypeError
+from miniworldmaker.exceptions.miniworldmaker_exception import MiniworldMakerError, MoveInDirectionTypeError
 from miniworldmaker.exceptions.miniworldmaker_exception import NoCostumeSetError
 from miniworldmaker.tokens import token as token_mod
 from miniworldmaker.boards import board
+from miniworldmaker.appearances import costume
+
 
 class TokenPositionManager:
-    def __init__(self, token : "token_mod.Token", board : "board.Board"):
+    def __init__(self, token: "token_mod.Token", board: "board.Board"):
         self.token = token
         self.last_position = (0, 0)
         self.last_direction = 90
         self._size = (0, 0)  # Tuple with size
         self._old_size = (0, 0)
         self._size = (1, 1)
         self.is_static = False
         self._position = (0, 0)
         self._direction = 0
         self._initial_direction = 0
         self._position = board_position.Position.create((0, 0))
 
-    def move_vector(self, vector : "board_vector.Vector") -> "token_mod.Token":
+    def move_vector(self, vector: "board_vector.Vector") -> "token_mod.Token":
         position = self.get_position()
         position = vector.add_to_position(position)
         self.set_position(position)
         return self.token
 
     @property
     def rect(self):
-        return self.get_rect()
+        return self.get_local_rect()
 
-    def get_rect(self) -> "board_rect.Rect":
-        return board_rect.Rect(self.token.position[0], self.token.position[1], self.size[0], self.size[1])
+    def get_global_rect(self) -> "board_rect.Rect":
+        if self.token.costume:
+            rect = self.token.costume.image.get_rect()
+        else:
+            rect = pygame.Rect(0, 0, self.token.size[0], self.token.size[1])
+        return rect
+
+    def get_local_rect(self) -> "board_rect.Rect":
+        pass
 
     @classmethod
     def from_center(cls, center_position: "board_position.Position"):
         """
         Creates a token with center at center_position
 
         Args:
@@ -60,15 +69,15 @@
     def direction(self, value: int):
         self.set_direction(value)
 
     def get_direction(self):
         direction = (self._direction + 180) % 360 - 180
         return direction
 
-    def set_direction(self, value : Union[int, float, str, board_direction.Direction]):
+    def set_direction(self, value: Union[int, float, str, board_direction.Direction]):
         if type(value) not in [int, float, str, board_direction.Direction, board_vector.Vector]:
             raise ValueError(f"Direction must be int, float, Direction or Vector but is {type(value)}")
         self.last_direction = self.direction
         direction = board_direction.Direction.create(value)
         self._direction = direction
         if self.last_direction != self._direction:
             self.token.costume.rotated()
@@ -77,38 +86,38 @@
     def size(self):
         return self._size
 
     @size.setter
     def size(self, value: Union[int, float, tuple]):
         self.set_size(value)
 
-    def set_size(self, value : Union[int, float, tuple]):
+    def set_size(self, value: Union[int, float, tuple]):
         """Sets size of token
 
         Args:
-            value (Union[int, float, tuple]): 
+            value (Union[int, float, tuple]):
                 An int or float will be converted to tuple (e.g. 2 => (2,2) )
 
         Raises:
             ValueError: Raises ValueError, if type not in [int, float, tuple]
 
         Returns:
             The token with changed values
         """
         if type(value) in [int, float]:
             if value < 0:
                 raise ValueError("token.size must be >= 0")
             else:
                 value = (value, value)
-        if type(value) == tuple:                
+        if type(value) == tuple:
             if value != self._size:
                 self._old_size = self._size
                 self._size = value
                 if self.token.costume:
-                    self.token.costume.reload_transformations_after("all")
+                    self.token.costume.set_dirty("scale", costume.Costume.RELOAD_ACTUAL_IMAGE)
         else:
             raise ValueError("token size must be int, float or tuple")
         return self.token
 
     def scale_width(self, value):
         old_width = self.token.size[0]
         old_height = self.token.size[1]
@@ -116,15 +125,15 @@
         self.set_size((value, old_height * scale_factor))
 
     def scale_height(self, value):
         old_width = self.token.size[0]
         old_height = self.token.size[1]
         scale_factor = value / old_height
         self.set_size((old_width * scale_factor, value))
-                
+
     def set_width(self, value):
         if value < 0:
             raise ValueError("token width must be >= 0")
         self.set_size((value, self.token.size[1]))
 
     def set_height(self, value):
         if value < 0:
@@ -141,43 +150,42 @@
     @position.setter
     def position(self, value: tuple):
         self.set_position(value)
 
     def get_position(self) -> "board_position.Position":
         return board_position.Position.create(self._position)
 
-    def set_position(self, value : Union[tuple, "board_position.BoardPosition"]) -> "board_position.BoardPosition":
+    def set_position(self, value: Union[tuple, "board_position.BoardPosition"]) -> "board_position.BoardPosition":
         self.last_position = self.position
         self.last_direction = self.direction
         self._position = board_position.Position.create(value)
+        self.token.board.camera.fetch_token(self.token)
         if self.last_position != self._position:
             self.token.dirty = 1
-            if self.token.board:
-                self.token.board.app.event_manager.send_event_to_containers("token_moved", self.token)
         return self.position
 
     @property
     def center(self) -> "board_position.Position":
         return self.get_center()
 
     @property
     def center_x(self):
         """x-value of token center-position"""
         if self.token.costume:
-            return self.rect.centerx
+            return self.get_global_rect().centerx
 
     @center_x.setter
     def center_x(self, value):
         self.set_center((value, self.center_y))
 
     @property
     def center_y(self):
         """y-value of token center-position"""
         if self.token.costume:
-            return self.rect.centery
+            return self.get_global_rect().centery
 
     @center_y.setter
     def center_y(self, value):
         if self.costume is None:
             raise NoCostumeSetError(self.token)
         self.set_center((self.center_x, value))
 
@@ -188,60 +196,62 @@
     def get_center(self):
         return board_position.Position.create((self.center_x, self.center_y))
 
     @property
     def local_center(self) -> "board_position.Position":
         return board_position.Position.create((self.center_x - self.topleft[0], self.center_y - self.topleft[1]))
 
-    def set_center(self, value :  Union[tuple, "board_position.Position"] ) -> "token_mod.Token":
+    def set_center(self, value: Union[tuple, "board_position.Position"]) -> "token_mod.Token":
         if self.token.costume is None:
             raise NoCostumeSetError(self.token)
         new_center = board_position.Position(value)
         self.last_position = self.position
-        rect = pygame.Rect.copy(self.rect)
+        rect = pygame.Rect.copy(self.get_global_rect)
         rect.center = new_center
-        # rect.centerx = value[0]
-        # rect.centery = value[1]
         self.set_position(rect.topleft)
         return self.token
 
     @property
     def topleft(self) -> "board_position.Position":
-        return board_position.Position.create(self.rect.topleft)
+        return board_position.Position.create(self.get_global_rect().topleft)
 
     @topleft.setter
     def topleft(self, value):
         self.last_position = self.position
         self.set_position(value)
 
     def move(self, distance: int = 0):
         if distance == 0:
             distance = self.token.speed
         destination = self.token.board_sensor.get_destination(self.position, self.direction, distance)
         self.position = destination
         return self
 
-    def move_towards_position(self, position):
-        tkn_position = board_position.Position.create(self.token.position)
-        if tkn_position.is_close(position):
+    def move_towards_position(self, position, distance=1):
+        tkn_center = board_position.Position.create(self.token.center)
+        if tkn_center.is_close(position):
             return self
         else:
-            direction = board_direction.Direction.create_from_token(self.token, position).value
+            direction = board_direction.Direction.from_token_to_position(self.token, position).value
             self.set_direction(direction)
-            self.move()
+            self.move(distance)
             return self
 
-    def move_in_direction(self, direction: Union[int, str, "board_position.Position", tuple], distance=1):
+    def move_in_direction(self, direction: Union[int, str, "board_direction.Direction"], distance=1):
         if type(direction) in [int, str]:
-            direction = board_direction.Direction.create_from_token(self.token, direction).value
+            direction = board_direction.Direction.from_token_towards_direction(self.token, direction).value
             self.set_direction(direction)
             self.move(distance)
             return self
-        else:
+        elif type(direction) in [tuple, board_position.Position]:
             return self.move_towards_position(direction)
+        else:
+            raise MiniworldMakerError(
+                f"No valid type in method move_in_direction - Expected int, str, Position or tuple, got {type(direction)}"
+            )
 
     def move_back(self):
         self.position = self.last_position
         self.direction = self.last_direction
         return self
 
     def move_to(self, new_center_position: Union[Tuple, "board_position.Position"]):
@@ -330,15 +340,17 @@
         Returns:
             int: new direction
         """
         self.turn_left(180)
         self.token.costume.flip(not self.token.costume.is_flipped)
         return self.direction
 
-    def point_in_direction(self, direction: Union[int, float, board_direction.Direction, str]) -> "board_direction.Direction":
+    def point_in_direction(
+        self, direction: Union[int, float, board_direction.Direction, str]
+    ) -> "board_direction.Direction":
         self.direction = board_direction.Direction.create(direction)
         return self.direction
 
     def self_remove(self):
         """
         Method is overwritten in subclasses
         """
@@ -359,15 +371,17 @@
     @y.setter
     def y(self, value: float):
         self.set_position((self.x, value))
 
     def draw_position(self):
         return (self.x, self.y)
 
-    def point_towards_position(self, destination : Union[int, float, str, board_direction.Direction]) -> "board_direction.Direction":
+    def point_towards_position(
+        self, destination: Union[int, float, str, board_direction.Direction]
+    ) -> "board_direction.Direction":
         """
         Token points towards a given position
 
         Args:
             destination: The position to which the actor should pointing
 
         Returns:
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/tokens/sensors/token_boardsensor.py` & `miniworldmaker-2.9.0.0/miniworldmaker/tokens/sensors/token_boardsensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import miniworldmaker.base.app as app
 import miniworldmaker.board_positions.board_position as board_position
 import miniworldmaker.board_positions.board_rect as board_rect
 import miniworldmaker.boards.board as board_mod
 import miniworldmaker.tokens.token as token_mod
 import miniworldmaker.tools.token_class_inspection as token_class_inspection
 from miniworldmaker.exceptions.miniworldmaker_exception import NotImplementedOrRegisteredError
+from abc import ABC, abstractmethod
 
-
-class TokenBoardSensor:
+class TokenBoardSensor(ABC):
     def __init__(self, token: "token_mod.Token", board: "board_mod.Board"):
         super().__init__()
         self.token: "token_mod.Token" = token
         self.board: "board_mod.Board" = board
 
     def remove_from_board(self):
         """Removes a token from board"""
@@ -34,15 +34,15 @@
         if token_list is None:
             return []
         # Filter tokens by class name
         if not token_filter:
             return token_list
         if type(token_filter) == str:
             token_list = self.filter_tokens_by_classname(token_list, token_filter)
-        elif isinstance(token_mod.Token, token_filter):
+        elif isinstance(token_filter, token_mod.Token):
             token_list = self.filter_tokens_by_instance(token_list, token_filter)
         elif issubclass(token_filter, token_mod.Token):
             token_list = self.filter_tokens_by_class(token_list, token_filter)
         return token_list
 
     def filter_tokens_by_class(
         self, token_list: List["token_mod.Token"], token_filter: Union[Type["token_mod.Token"], None]
@@ -78,18 +78,18 @@
     def sensing_token(self, token_filter=None) -> Union["token_mod.Token", None]:
         raise NotImplementedOrRegisteredError(self.sensing_token)
 
     def sensing_tokens(self, token_filter=None) -> List["token_mod.Token"]:
         raise NotImplementedOrRegisteredError(self.sensing_tokens)
 
     def sensing_point(self, pixel_position):
-        return self.token.rect.collidepoint(pixel_position)
+        return self.token.get_global_rect().collidepoint(pixel_position)
 
     def sensing_rect(self, rect):
-        return self.token.rect.colliderect(rect)
+        return self.token.get_global_rect().colliderect(rect)
 
     def sensing_on_board(self, distance: int) -> bool:
         raise NotImplementedOrRegisteredError(self.sensing_on_board)
 
     def sensing_borders(self, distance: int) -> list:
         raise NotImplementedOrRegisteredError(self.sensing_borders)
 
@@ -111,33 +111,31 @@
     @staticmethod
     def get_destination(start, direction, distance) -> "board_position.Position":
         exact_position_x = start[0] + math.sin(math.radians(direction)) * distance
         exact_position_y = start[1] - math.cos(math.radians(direction)) * distance
         pos = board_position.Position.create((exact_position_x, exact_position_y))
         return pos
 
-    @staticmethod
-    def is_position_on_board(pos):
+    def is_position_on_board(self, pos):
         """
         Checks if Position is on board
 
         Returns:
             True, if Position is on board.
         """
-        board = app.App.board
-        if 0 <= pos[0] < board.columns and 0 <= pos[1] < board.rows:
+        board = self.board
+        if 0 <= pos[0] < board.boundary_x and 0 <= pos[1] < board.boundary_y:
             return True
         else:
             return False
 
-    @classmethod
-    def is_rect_completly_on_board(cls, rect):
+    def is_rect_completly_on_board(self, rect):
         rect = board_rect.Rect.create(rect)
-        topleft_on_board = cls.is_position_on_board(rect.topleft)
-        bottom_right_on_board = TokenBoardSensor.is_position_on_board(rect.bottomright)
+        topleft_on_board = self.is_position_on_board(rect.topleft)
+        bottom_right_on_board = self.is_position_on_board(rect.bottomright)
         return topleft_on_board or bottom_right_on_board
 
     def get_borders_from_rect(self, rect):
         """
         Gets all borders the rect ist touching.
 
         Returns: A list of borders as strings: "left", "bottom", "right", or "top"
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/tokens/sensors/token_pixelboardsensor.py` & `miniworldmaker-2.9.0.0/miniworldmaker/tokens/sensors/token_pixelboardsensor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import math
-from typing import Union, Optional
+from typing import Union, Optional, List
 
 import pygame
 
 import miniworldmaker.board_positions.board_position as board_position
 import miniworldmaker.board_positions.board_rect as board_rect
 import miniworldmaker.boards.board as board_mod
 import miniworldmaker.tokens.sensors.token_boardsensor as boardsensor
@@ -14,16 +14,15 @@
     """Sensor for Tokens on PixelBoard.
     """
 
     def __init__(self, token: "token_mod.Token", board: "board_mod.Board"):
         super().__init__(token, board)
 
     def sensing_on_board(self, distance: int = 0) -> bool:
-        target_rect = self.get_destination_rect(distance)
-        return self.is_rect_completly_on_board(target_rect)
+        return self.token.board.camera.is_token_in_viewport(self.token)
 
     def sensing_borders(self, distance: int = 0) -> list:
         """
         The function compares the rectangle (or alternatively the
         path that the rectangle of the object **distance** pixels travels)
         with the edges of the playing field.
         """
@@ -58,76 +57,57 @@
                                                range(1, sampling_rate + 1))]
 
     @staticmethod
     def filter_actor_list(a_list, actor_type):
         return [actor for actor in a_list if type(token_mod.Token) == actor_type]
 
     def sensing_tokens(self, token_filter=None) -> list:
-        tokens = self.get_tokens_at_rect(self.token.rect)
+        tokens = pygame.sprite.spritecollide(self.token, self.token.board.camera.get_tokens_in_viewport(),  False, pygame.sprite.collide_rect)  
+        tokens_list = self.remove_self_from_token_list(tokens)
+        if tokens_list:
+            tokens_list = self._detect_token(tokens_list, self.token.collision_type)
+        if tokens_list:
+            tokens_list = self.filter_token_list(tokens_list, token_filter)
+        if tokens_list and len(tokens_list) >= 1:
+            return tokens_list
+        else: 
+            return []
+
+    def sensing_token(self, token_filter=None) -> Union["token_mod.Token", None]:
+        token = pygame.sprite.spritecollideany(self.token, self.token.board.camera.get_tokens_in_viewport(), None)
+        tokens_list = self.remove_self_from_token_list([token])
+        if tokens_list:
+            tokens_list = self._detect_token(tokens_list, self.token.collision_type)
+        if tokens_list:
+            tokens_list = self.filter_token_list(tokens_list, token_filter)
+        if tokens_list and len(tokens_list) >= 1:
+            return tokens_list[0]
+        else: 
+            return []
+    
+    def _detect_token(self, tokens, collision_type) -> List:
         tokens_list = []
-        if self.token.collision_type == "default":
-            collision_type = "mask"
-        else:
-            collision_type = self.token.collision_type
         if collision_type == "circle":
             tokens_list = [
                 token for token in tokens if pygame.sprite.collide_circle(self.token, token)]
         elif collision_type == "rect" or collision_type == "static-rect":
             tokens_list = [
                 token for token in tokens if pygame.sprite.collide_rect(self.token, token)]
         elif collision_type == "mask":
             tokens_list = [
                 token for token in tokens if pygame.sprite.collide_mask(self.token, token)]
-        tokens_list = self.remove_self_from_token_list(tokens_list)
-        tokens_list = self.filter_token_list(tokens_list, token_filter)
         return tokens_list
 
-    def sensing_token(self, token_filter=None) -> Union["token_mod.Token", None]:
-        tokens = [self.get_single_token_at_rect(self.token.rect)]
-        tokens = self.filter_token_list(tokens, token_filter)
-        if self.token.collision_type == "default":
-            collision_type = "mask"
-        else:
-            collision_type = self.token.collision_type
-        if not tokens:
-            return None
-        for token in tokens:
-            if collision_type == "circle" and pygame.sprite.collide_circle(self.token, token):
-                return token
-            if collision_type == "rect" or collision_type == "static-rect" and pygame.sprite.collide_rect(self.token,
-                                                                                                          token):
-                return token
-            if collision_type == "mask" and pygame.sprite.collide_mask(self.token, token):
-                return token
-        return tokens[0]
-
     def sensing_tokens_at(self, direction: int = 0, distance: int = 1) -> list:
         if direction == 0:
             direction = self.token.direction
         destination = self.get_destination(self.token.center, direction, distance)
         return self.get_tokens_at_position(destination)
 
     def get_tokens_at_position(self, position):
         tokens = []
         for token in self.board.tokens:
-            if token.rect.collidepoint(position[0], position[1]):
+            if token.get_global_rect().collidepoint(position[0], position[1]):
                 tokens.append(token)
         if self.token in tokens:
             tokens.remove(self.token)
         return tokens
-
-    def get_single_token_at_rect(self, rect: pygame.Rect) -> Optional["token_mod.Token"]:
-        # Get first colliding token
-        for token in self.board.tokens.sprites():
-            if token.rect.colliderect(rect) and token != self.token:
-                return token
-        return None
-
-    def get_tokens_at_rect(self, rect: pygame.Rect) -> list:
-        """Returns all tokens that collide with a rectangle.
-
-        Args:
-            rect: A rectangle
-
-        Returns all tokens in a rect
-        """
-        return [token for token in self.board.tokens if token.rect.colliderect(rect)]
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/tokens/sensors/token_tiledboardsensor.py` & `miniworldmaker-2.9.0.0/miniworldmaker/tokens/sensors/token_tiledboardsensor.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/tokens/shapes.py` & `miniworldmaker-2.9.0.0/miniworldmaker/tokens/shapes.py`

 * *Files 7% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         If you change the circle-size (e.g. with self.size = (x, y), the radius value will be changed too.
         """
         return self._radius
 
     @radius.setter
     def radius(self, value):
         self._radius = value
-        self.costume._update_draw_shape()
+        self.costume.set_dirty("scale", self.costume.RELOAD_ACTUAL_IMAGE)
 
     def set_physics_default_values(self):
         self.physics.shape_type = "circle"
         self.physics.can_move = True
         self.physics.stable = False
 
 
@@ -152,15 +152,14 @@
             height: float = 10,
     ):
         self.check_arguments(position, width, height)
         super().__init__(position)
         self.costume = shape_costume.EllipseCostume(self)
         self._border = 1
         self.size = (width, height)
-        self.costume._update_draw_shape()
 
     def check_arguments(self, position, width, height):
         if type(position) not in [tuple, board_position.Position, None]:
             raise EllipseWrongArgumentsError()
 
     @classmethod
     def from_topleft(cls, position: tuple, width: float, height: float):
@@ -202,24 +201,24 @@
     @property
     def start_angle(self):
         return self._start_angle
 
     @start_angle.setter
     def start_angle(self, value):
         self._start_angle = value
-        self.costume._update_draw_shape()
+        self.costume.set_dirty("draw_shapes", self.costume.RELOAD_ACTUAL_IMAGE)
 
     @property
     def end_angle(self):
         return self._end_angle
 
     @end_angle.setter
     def end_angle(self, value):
         self._end_angle = value
-        self.costume._update_draw_shape()
+        self.costume.set_dirty("draw_shapes", self.costume.RELOAD_ACTUAL_IMAGE)
 
     @classmethod
     def from_topleft(cls, position: tuple, width: float, height: float, start_angle, end_angle):
         """Creates a rectangle with topleft at position"""
         rectangle = cls(position, width, height, start_angle, end_angle).center
         return rectangle
 
@@ -268,55 +267,37 @@
             raise LineFirstArgumentError(start_position)
         if type(end_position) not in [tuple, board_position.Position, None]:
             raise LineSecondArgumentError(end_position)
         self._start_position = start_position
         self._end_position = end_position
         super().__init__(start_position)
         self.costume = shape_costume.LineCostume(self)
-        self.position = start_position
-        self.costume._update_draw_shape()
-        box = self.get_bounding_box()
-        self.position = box.topleft
-
+        
     def set_physics_default_values(self):
         self.physics.shape_type = "line"
         self.physics.simulation = "static"
 
-    def get_bounding_box(self):
-        width = abs(self.start_position[0] - self.end_position[0]) + 2 * self.border
-        height = abs(self.start_position[1] - self.end_position[1]) + 2 * self.border
-        box = pygame.Rect(
-            min(self.start_position[0], self.end_position[0]) - self.border,
-            min(self.start_position[1], self.end_position[1]) - self.border,
-            width,
-            height,
-        )
-        self.position = box[0], box[1]
-        width, height = box[2], box[3]
-        self.width = width
-        self.height = height
-        return box
-
     @property
     def start_position(self):
         return self._start_position
 
     @start_position.setter
     def start_position(self, value: Tuple):
         self._start_position = value
-        self.costume._update_draw_shape()
-
+        self.costume.set_dirty("all", 1)
+        
     @property
     def end_position(self):
         return self._end_position
 
     @end_position.setter
     def end_position(self, value: Tuple):
         self._end_position = value
-        self.costume._update_draw_shape()
+        self.costume.set_dirty("all", 1)
+        
 
     @property
     def thickness(self):
         """-> see border"""
         return self.border
 
     @thickness.setter
@@ -353,15 +334,15 @@
             width: float = 10,
             height: float = 10,
     ):
         self.check_arguments(topleft, width, height)
         super().__init__(topleft)
         self.costume = shape_costume.RectangleCostume(self)
         self.size = (width, height)
-        self.costume._update_draw_shape()
+
 
     def check_arguments(self, topleft, width, height):
         if type(topleft) != tuple and type(topleft) != board_position.Position:
             raise RectFirstArgumentError(topleft)
         if type(width) not in [int, float]:
             raise TypeError("width of Rectangle should be int or float " + str(type(width)))
         if type(height) not in [int, float]:
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/tokens/text_token.py` & `miniworldmaker-2.9.0.0/miniworldmaker/tokens/text_token.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,25 +37,25 @@
     @property
     def font_size(self):
         return self.costume.font_size
 
     @font_size.setter
     def font_size(self, value):
         self.costume.font_size = value
-        self.costume._update_draw_shape()
+        self.costume.set_dirty("write_text", self.costume.RELOAD_ACTUAL_IMAGE)
 
     def set_text(self, text):
         """
         Sets the text of the token
 
         Args:
             text: The text
         """
         self.costume.text = text
-        self.costume._update_draw_shape()
+        
 
     def get_text(self):
         """Gets the currently displayed tex
 
         Returns:
             The currently displayed text
 
@@ -68,14 +68,14 @@
         return self.get_text()
 
     @text.setter
     def text(self, value):
         if value == "":
             value = " "
         self.set_text(value)
-        self.costume._update_draw_shape()
+        self.costume.set_dirty("all", self.costume.RELOAD_ACTUAL_IMAGE)
 
 
 class TextToken(Text):
     """Alias for legacy code"""
 
     pass
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/tokens/token.py` & `miniworldmaker-2.9.0.0/miniworldmaker/tokens/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import pygame.rect
 
 import miniworldmaker.appearances.appearance as appearance
 import miniworldmaker.appearances.costume as costume
 import miniworldmaker.board_positions.board_position as board_position
 import miniworldmaker.tokens.token_base as token_base
+from miniworldmaker.board_positions import board_direction
 from miniworldmaker.exceptions.miniworldmaker_exception import (
     MiniworldMakerError,
     NotImplementedOrRegisteredError,
 )
 
 
 class Token(token_base.BaseToken):
@@ -114,15 +115,18 @@
 
         * `static-rect`: Are tokens colliding when checking circle with radius = bounding-box-radius.(Only PixelBoard)
 
         * `circle`: Are tokens colliding when checking circle with radius = bounding-box-radius.(Only PixelBoard)
 
         * `mask`: Are tokens colliding when checkig if their image masks are overlapping.
         """
-        return self._collision_type
+        if self._collision_type == "default":
+            return "mask"
+        else:
+            return self._collision_type
 
     @collision_type.setter
     def collision_type(self, value: str):
         self._collision_type = value
 
     @property
     def layer(self) -> int:
@@ -176,15 +180,15 @@
                 assert token.costume_count == 1
                 board.run()
 
 
         Returns:
             int: _description_
         """
-        return self.costume_manager.count()
+        return self.costume_manager.length()
 
     @property
     def is_flipped(self) -> bool:
         """
         If a token is flipped, it is mirrored via the y-axis. You can use this property in 2d-plattformers
         to change the direction of token.
 
@@ -276,15 +280,15 @@
                 <source src="../_static/flipthefish.webm" type="video/webm">
                 Your browser does not support the video tag.
                 </video>
 
         """
         return self.position_manager.flip_x()
 
-    def add_costume(self, source: Union[Tuple, str, List]) -> costume.Costume:
+    def add_costume(self, source: Union[None, Tuple, str, List] = None) -> costume.Costume:
         """Adds a new costume to token.
         The costume can be switched with self.switch_costume(index)
 
         Args:
             source: Path to the first image of new costume or Tuple with color-value
 
         Examples:
@@ -354,25 +358,25 @@
                 :alt: Create multiple costumes and switch between costumes
 
         Returns:
             The new costume.
 
         """
         
-        if type(source) in [str, tuple]:
-            return self.costume_manager.add_costume(source)
+        if not source or type(source) in [str, tuple]:
+            return self.costume_manager.add_new_appearance(source)
         elif type(source) == list:
-            return self.costume_manager.add_costume_from_list(source)
+            return self.costume_manager.add_new_appearance_from_list(source)
         else:
             raise MiniworldMakerError(f"Wrong type for appearance. Expected: list, tuple or str, got {type(source)}")
 
     def add_costumes(self, sources : list) -> costume.Costume:
         """Adds multiple costumes
         """
-        return self.costume_manager.add_costumes(sources)
+        return self.costume_manager.add_new_appearances(sources)
 
     def remove_costume(self, source: Union[int, "costume.Costume"] = None):
         """Removes a costume from token
 
         Args:
             source: The index of the new costume or costume-object. Defaults to actual costume
         """
@@ -421,26 +425,28 @@
         """
         self.costume_manager.next_costume()
 
     @property
     def costume(self) -> costume.Costume:
         """Gets the costume of token
         """
-        if hasattr(self, "_costume_manager") and self._costume_manager:
-            return self.costume_manager.costume
+        if hasattr(self, "costume_manager") and self.costume_manager is not None:
+            return self.costume_manager.get_actual_appearance()
 
     @costume.setter
     def costume(self, value):
-        self.costume_manager.costume = value
+        self.costume_manager.appearance = value
 
     @property
     def costumes(self) -> list:
-        """Gets a list of all costumes.
+        """Gets the costume manager
+        
+        The costume manager can be iterated to get all costumes
         """
-        return self.costume_manager.costumes
+        return self.costume_manager
 
     @property
     def orientation(self) -> int:
         return self.costume.orientation
 
     @orientation.setter
     def orientation(self, value: int):
@@ -712,15 +718,15 @@
         Args:
             other: The other token
 
         Returns:
             The new direction
 
         """
-        pos = other.rect.center
+        pos = other.get_global_rect().center
         return self.point_towards_position(pos)
 
     @property
     def size(self) -> tuple:
         """Size of the token"""
         return self.position_manager.size
 
@@ -849,20 +855,20 @@
     def center_x(self):
         """x-value of token center-position"""
         return self.position_manager.center_x
 
     @property
     def topleft_x(self):
         """x-value of token topleft-position"""
-        return self.rect.topleft[0]
+        return self.get_global_rect.topleft[0]
 
     @property
     def topleft_y(self):
         """x-value of token topleft-position"""
-        return self.rect.topleft[1]
+        return self.get_global_rect.topleft[1]
 
     @property
     def topleft(self) -> "board_position.Position":
         return self.position_manager.topleft
 
     @topleft.setter
     def topleft(self, value: Union[Tuple, "board_position.Position"]):
@@ -957,19 +963,21 @@
             .. code-block:: python
 
                 def on_sensing_wall(self, wall):
                     self.move_back()
 
         """
         return self.position_manager.move_back()
+    
+    undo_move = move_back
 
     def move_towards(self, position):
         return self.position_manager.move_towards_position(position)
 
-    def move_in_direction(self, direction: Union[int, str, tuple, "board_position.Position"], distance=1):
+    def move_in_direction(self, direction: Union[int, str, tuple, "board_direction.Direction", "board_position.Position"], distance=1):
         """Moves token *distance* steps into a *direction* or towards a position
 
         .. image:: ../_images/move_in_direction.png
 
         Options
             * 0, "up" - Look up
             * 90, "right", - Look right
@@ -982,15 +990,20 @@
             direction: Direction as angle
             distance: Senses obj "distance" steps in front of current token.
 
         Returns:
             The token itself
 
         """
-        return self.position_manager.move_in_direction(direction, distance)
+        if type(direction) in [int, str, board_direction.Direction]:
+            return self.position_manager.move_in_direction(direction, distance)
+        elif type(direction) == tuple or isinstance(direction, board_position.Position):
+            return self.position_manager.move_towards_position(direction, distance)
+        else:
+            raise MiniworldMakerError(f"Expected direction or position, got f{type(direction)}, ({direction})")
 
     def move_to(self, position: "board_position.Position"):
         """Moves token *distance* to a specific board_posiition
 
         Args:
             position: The position to which the actor should move. The position can be a 2-tuple (x, y)
             which will be converted to a board_position
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/tokens/token_base.py` & `miniworldmaker-2.9.0.0/miniworldmaker/tokens/token_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,18 +34,18 @@
 
 
 class BaseToken(pygame.sprite.DirtySprite, metaclass=Meta):
     token_count: int = 0
     class_image: str = ""
 
     def __init__(self, position: Optional[Union[Tuple, "board_position.Position"]] = (0,0)):
-        self._collision_type: str = "rect"
+        self._collision_type: str = "mask"
+        self._dirty = 0
         self._layer: int = 0
         self._inner = 0
-        self._dirty = 1
         self._size = (0, 0)
         self._static = False
         self._position: "board_position.Position" = position
         self._managers: list = list()
         self.token_id: int = BaseToken.token_count + 1
         self.board: "board.Board" = app.App.board
         self._board_sensor: token_boardsensor.TokenBoardSensor = self._init_board_sensor()
@@ -53,14 +53,15 @@
         self._costume_manager: costumes_manager.CostumesManager = self._init_costume_manager()
         if not self.board:
             raise NoBoardError()
         pygame.sprite.DirtySprite.__init__(self)
         BaseToken.token_count += 1
         self.speed: int = 1
         self.ask: "ask.Ask" = ask.Ask(self.board)
+        self._dirty = 1
         
     def _get_new_costume(self):
         return self.board.get_token_connector(self).create_costume()
         
     def _init_board_sensor(self):
         self._board_sensor = self.board.get_token_connector(self).create_board_sensor()
         self._managers.append(self._board_sensor)
@@ -77,27 +78,23 @@
         self._position_manager.position = self._position
         self._managers.append(self._position_manager)
         return self._position_manager
 
     @property
     def position_manager(self):
         if not hasattr(self, "_position_manager") or not self._position_manager:
-            self._init_position_manager()
+            return None
         return self._position_manager
 
     @property
     def board_sensor(self):
-        if not hasattr(self, "_position_manager") or not self._board_sensor:
-            self._init_board_sensor()
         return self._board_sensor
     
     @property
     def costume_manager(self):
-        if not hasattr(self, "_position_manager") or not self._costume_manager:
-            self._init_costume_manager()
         return self._costume_manager
 
     @property
     def position(self) -> "board_position.Position":
         """
         The position of the token as Position (x, y)
         """
@@ -145,26 +142,39 @@
 
             int: 1 if token is dirty/0 otherwise
         """
         return self._dirty
 
     @dirty.setter
     def dirty(self, value: int):
-        self._dirty = value
+        if not self._dirty and self.position_manager and self.board.camera.is_token_in_viewport(self) and value == 1:
+            self._dirty = 1
+        elif value == 0:
+            self._dirty = 0
+        else:
+            pass
 
     @property
     def rect(self) -> pygame.Rect:
         """
         The surrounding Rectangle as pygame.Rect.
         Warning: If the token is rotated, the rect vertices are not the vertices of the token image.
         """
-        return self.position_manager.rect
+        return self.position_manager.get_local_rect()
 
     def get_rect(self) -> pygame.Rect:
-        return self.position_manager.rect
+        return self.position_manager.get_local_rect()
+    
+    def get_local_rect(self) -> pygame.Rect:
+        return self.position_manager.get_local_rect()
+    
+    def get_global_rect(self) -> pygame.Rect:
+        if self.position_manager:
+            return self.position_manager.get_global_rect()
+        return pygame.Rect(-1,-1,0,0)
 
     def register(self, method: callable):
         """This method is used for the @register decorator. It adds a method to an object
 
         Args:
             method (callable): The method which should be added to the token
         """
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/tools/inspection.py` & `miniworldmaker-2.9.0.0/miniworldmaker/tools/inspection.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/tools/keys.py` & `miniworldmaker-2.9.0.0/miniworldmaker/tools/keys.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/tools/method_caller.py` & `miniworldmaker-2.9.0.0/miniworldmaker/tools/method_caller.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/tools/timer.py` & `miniworldmaker-2.9.0.0/miniworldmaker/tools/timer.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/tools/token_class_inspection.py` & `miniworldmaker-2.9.0.0/miniworldmaker/tools/token_class_inspection.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker/tools/token_inspection.py` & `miniworldmaker-2.9.0.0/miniworldmaker/tools/token_inspection.py`

 * *Files identical despite different names*

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker.egg-info/PKG-INFO` & `miniworldmaker-2.9.0.0/miniworldmaker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniworldmaker
-Version: 2.8.0.0
+Version: 2.9.0.0
 Summary: Create 2D Miniworlds and Games
 Home-page: https://github.com/asbl/miniworldmaker
 Download-URL: https://github.com/asbl/miniworldmaker
 Author: Andreas Siebel
 Author-email: andreas.siebel@it-teaching.de
 License: OSI Approved :: MIT License
 Keywords: games,education,mini-worlds,pygame
```

### Comparing `miniworldmaker-2.8.0.0/miniworldmaker.egg-info/SOURCES.txt` & `miniworldmaker-2.9.0.0/miniworldmaker.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 miniworldmaker/boards/board.py
 miniworldmaker/boards/board_base.py
 miniworldmaker/boards/hex_board.py
 miniworldmaker/boards/physics_board.py
 miniworldmaker/boards/pixel_board.py
 miniworldmaker/boards/tiled_board.py
 miniworldmaker/boards/board_manager/__init__.py
+miniworldmaker/boards/board_manager/board_camera_manager.py
 miniworldmaker/boards/board_manager/board_collision_manager.py
 miniworldmaker/boards/board_manager/board_event_manager.py
 miniworldmaker/boards/board_manager/board_mouse_manager.py
 miniworldmaker/boards/data/__init__.py
 miniworldmaker/boards/data/db_manager.py
 miniworldmaker/boards/data/export_factory.py
 miniworldmaker/boards/data/import_factory.py
```

### Comparing `miniworldmaker-2.8.0.0/setup.py` & `miniworldmaker-2.9.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') \
         as f: long_description = f.read()
 
 setup(name='miniworldmaker',
-      version='2.8.0.0',
+      version='2.9.0.0',
       description='Create 2D Miniworlds and Games',
       long_description=long_description,
       long_description_content_type='text/markdown',
       keywords=['games', 'education', 'mini-worlds', 'pygame'],  # arbitrary keywords
       author='Andreas Siebel',
       author_email='andreas.siebel@it-teaching.de',
       url='https://github.com/asbl/miniworldmaker',
```

