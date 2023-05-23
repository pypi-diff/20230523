# Comparing `tmp/rapidpro_flow_tools-0.2.0.tar.gz` & `tmp/rapidpro_flow_tools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpro_flow_tools-0.2.0.tar", max compression
+gzip compressed data, was "rapidpro_flow_tools-0.3.0.tar", max compression
```

## Comparing `rapidpro_flow_tools-0.2.0.tar` & `rapidpro_flow_tools-0.3.0.tar`

### file list

```diff
@@ -1,157 +1,155 @@
--rw-r--r--   0        0        0      500 2023-05-23 20:09:46.478636 rapidpro_flow_tools-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-23 19:56:00.546855 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/__init__.py
--rw-r--r--   0        0        0      432 2023-05-09 14:52:38.982087 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/credentials.json
--rw-r--r--   0        0        0     1222 2023-05-17 15:46:39.488657 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/flow_converter.py
--rw-r--r--   0        0        0        0 2023-05-08 22:11:19.527477 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/__init__.py
--rw-r--r--   0        0        0      170 2023-05-09 00:10:28.581047 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0        0 2023-05-08 22:11:19.528476 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/__init__.py
--rw-r--r--   0        0        0      177 2023-05-09 00:10:28.589045 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6513 2023-05-09 00:33:05.120904 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/__pycache__/cellparser.cpython-311.pyc
--rw-r--r--   0        0        0     4351 2023-05-09 00:40:17.721630 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/__pycache__/rowdatasheet.cpython-311.pyc
--rw-r--r--   0        0        0    12710 2023-05-09 00:10:28.592570 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/__pycache__/rowparser.cpython-311.pyc
--rw-r--r--   0        0        0     4042 2023-05-09 00:40:17.718628 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/__pycache__/sheetparser.cpython-311.pyc
--rw-r--r--   0        0        0     4152 2023-05-08 22:11:19.528476 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/cellparser.py
--rw-r--r--   0        0        0     3205 2023-05-08 22:11:19.528476 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/rowdatasheet.py
--rw-r--r--   0        0        0    15945 2023-05-08 22:11:19.529476 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/rowparser.py
--rw-r--r--   0        0        0     1849 2023-05-08 22:11:19.529476 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/sheetparser.py
--rw-r--r--   0        0        0        0 2023-05-08 22:11:19.530479 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/tests/__init__.py
--rw-r--r--   0        0        0      163 2023-05-08 22:11:19.530479 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/tests/mock_cell_parser.py
--rw-r--r--   0        0        0      292 2023-05-08 22:11:19.530479 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/tests/mock_row_parser.py
--rw-r--r--   0        0        0      826 2023-05-08 22:11:19.531487 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/tests/mock_sheetparser.py
--rw-r--r--   0        0        0      600 2023-05-08 22:11:19.532477 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/tests/models.py
--rw-r--r--   0        0        0     6080 2023-05-08 22:11:19.532477 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/tests/test_cellparser.py
--rw-r--r--   0        0        0     3508 2023-05-08 22:11:19.533482 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/tests/test_differentways.py
--rw-r--r--   0        0        0     5026 2023-05-08 22:11:19.534481 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/tests/test_full_rows.py
--rw-r--r--   0        0        0     3050 2023-05-08 22:11:19.534481 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/tests/test_rowdatasheet.py
--rw-r--r--   0        0        0     2022 2023-05-08 22:11:19.535494 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/tests/test_sheetparser.py
--rw-r--r--   0        0        0     4684 2023-05-08 22:11:19.535494 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/tests/test_unparse.py
--rw-r--r--   0        0        0        0 2023-05-08 22:11:19.535494 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/__init__.py
--rw-r--r--   0        0        0      179 2023-05-09 00:10:28.582044 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    10375 2023-05-09 00:10:28.585042 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/__pycache__/contentindexparser.cpython-311.pyc
--rw-r--r--   0        0        0     1948 2023-05-09 00:10:28.588039 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/__pycache__/contentindexrowmodel.cpython-311.pyc
--rw-r--r--   0        0        0      553 2023-05-09 14:53:32.970178 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/__pycache__/datarowmodel.cpython-311.pyc
--rw-r--r--   0        0        0    31826 2023-05-09 00:40:18.077840 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/__pycache__/flowparser.cpython-311.pyc
--rw-r--r--   0        0        0     5701 2023-05-09 00:40:18.053361 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/__pycache__/flowrowmodel.cpython-311.pyc
--rw-r--r--   0        0        0      152 2023-05-08 22:11:19.536490 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/constants.py
--rw-r--r--   0        0        0     7020 2023-05-08 22:11:19.536490 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/contentindexparser.py
--rw-r--r--   0        0        0      932 2023-05-08 22:11:19.536490 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/contentindexrowmodel.py
--rw-r--r--   0        0        0      102 2023-05-08 22:11:19.537511 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/datarowmodel.py
--rw-r--r--   0        0        0    26665 2023-05-08 22:11:19.538499 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/flowparser.py
--rw-r--r--   0        0        0     5242 2023-05-08 22:11:19.538499 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/flowrowmodel.py
--rw-r--r--   0        0        0     1016 2023-05-08 22:11:19.539488 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/template_sheet_parser.py
--rw-r--r--   0        0        0        0 2023-05-08 22:11:19.539488 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/tests/__init__.py
--rw-r--r--   0        0        0      179 2023-05-08 22:11:19.539488 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/tests/datarowmodels/evalmodels.py
--rw-r--r--   0        0        0      444 2023-05-08 22:11:19.540493 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/tests/datarowmodels/listmodel.py
--rw-r--r--   0        0        0      557 2023-05-08 22:11:19.540493 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/tests/datarowmodels/nestedmodel.py
--rw-r--r--   0        0        0      133 2023-05-08 22:11:19.541498 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/tests/datarowmodels/simplemodel.py
--rw-r--r--   0        0        0      478 2023-05-08 22:11:19.541498 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/tests/mock_sheetreader.py
--rw-r--r--   0        0        0     1030 2023-05-08 22:11:19.541498 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/tests/row_data.py
--rw-r--r--   0        0        0    17043 2023-05-08 22:11:19.542498 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/tests/test_contentindexparser.py
--rw-r--r--   0        0        0    39668 2023-05-08 22:11:19.543511 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/tests/test_flowparser.py
--rw-r--r--   0        0        0    14789 2023-05-08 22:11:19.543511 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/tests/test_to_row_model.py
--rw-r--r--   0        0        0      259 2023-05-08 22:11:19.543511 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/tests/utils.py
--rw-r--r--   0        0        0        0 2023-05-08 22:11:19.544512 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/sheets/__init__.py
--rw-r--r--   0        0        0      177 2023-05-09 00:40:18.079823 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/sheets/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1856 2023-05-09 00:40:18.081823 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/sheets/__pycache__/csv_sheet_reader.cpython-311.pyc
--rw-r--r--   0        0        0     5435 2023-05-17 13:48:55.572103 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/sheets/__pycache__/google_sheet_reader.cpython-311.pyc
--rw-r--r--   0        0        0     1799 2023-05-09 00:40:18.082822 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/sheets/__pycache__/xlsx_sheet_reader.cpython-311.pyc
--rw-r--r--   0        0        0      626 2023-05-08 22:11:19.544512 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/sheets/csv_sheet_reader.py
--rw-r--r--   0        0        0     3199 2023-05-17 13:33:29.457039 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/sheets/google_sheet_reader.py
--rw-r--r--   0        0        0      711 2023-05-08 22:11:19.545511 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/sheets/xlsx_sheet_reader.py
--rw-r--r--   0        0        0        0 2023-05-08 22:11:19.545511 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/__init__.py
--rw-r--r--   0        0        0      171 2023-05-09 00:40:18.041350 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      408 2023-05-09 00:40:18.047361 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0    20155 2023-05-09 00:40:18.060364 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/models/__pycache__/actions.cpython-311.pyc
--rw-r--r--   0        0        0     1367 2023-05-09 00:40:18.062829 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/models/__pycache__/common.cpython-311.pyc
--rw-r--r--   0        0        0    15080 2023-05-09 00:40:18.045351 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/models/__pycache__/containers.cpython-311.pyc
--rw-r--r--   0        0        0    30325 2023-05-09 00:40:18.051365 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/models/__pycache__/nodes.cpython-311.pyc
--rw-r--r--   0        0        0    30571 2023-05-09 00:40:18.067821 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/models/__pycache__/routers.cpython-311.pyc
--rw-r--r--   0        0        0    11728 2023-05-08 22:11:19.546511 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/models/actions.py
--rw-r--r--   0        0        0     1004 2023-05-08 22:11:19.547498 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/models/common.py
--rw-r--r--   0        0        0    10931 2023-05-08 22:11:19.547498 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/models/containers.py
--rw-r--r--   0        0        0    20809 2023-05-08 22:11:19.547498 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/models/nodes.py
--rw-r--r--   0        0        0    18753 2023-05-08 22:11:19.548498 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/models/routers.py
--rw-r--r--   0        0        0        0 2023-05-08 22:11:19.549493 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/__init__.py
--rw-r--r--   0        0        0      154 2023-05-08 22:11:19.550002 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/add_contact_urn.json
--rw-r--r--   0        0        0      225 2023-05-08 22:11:19.551016 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/add_input_labels.json
--rw-r--r--   0        0        0      260 2023-05-08 22:11:19.551016 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/call_classifier.json
--rw-r--r--   0        0        0      123 2023-05-08 22:11:19.552016 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/call_resthook.json
--rw-r--r--   0        0        0      258 2023-05-08 22:11:19.552016 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/call_webhook.json
--rw-r--r--   0        0        0      199 2023-05-08 22:11:19.552016 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/enter_flow.json
--rw-r--r--   0        0        0      466 2023-05-08 22:11:19.552016 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/open_ticket.json
--rw-r--r--   0        0        0      140 2023-05-08 22:11:19.553020 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/play_audio.json
--rw-r--r--   0        0        0      242 2023-05-08 22:11:19.553020 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/remove_contact_groups.json
--rw-r--r--   0        0        0      213 2023-05-08 22:11:19.553020 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/say_msg.json
--rw-r--r--   0        0        0      214 2023-05-08 22:11:19.554019 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/send_broadcast.json
--rw-r--r--   0        0        0      258 2023-05-08 22:11:19.554019 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/send_email.json
--rw-r--r--   0        0        0      512 2023-05-08 22:11:19.554019 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/send_msg.json
--rw-r--r--   0        0        0      573 2023-05-08 22:11:19.555032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/send_msg_with_attachments.json
--rw-r--r--   0        0        0      549 2023-05-08 22:11:19.555032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/send_msg_with_quick_replies.json
--rw-r--r--   0        0        0      211 2023-05-08 22:11:19.555032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/set_contact_channel.json
--rw-r--r--   0        0        0      190 2023-05-08 22:11:19.556033 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/set_contact_field.json
--rw-r--r--   0        0        0      117 2023-05-08 22:11:19.556033 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/set_contact_language.json
--rw-r--r--   0        0        0      115 2023-05-08 22:11:19.557020 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/set_contact_name.json
--rw-r--r--   0        0        0      117 2023-05-08 22:11:19.557020 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/set_contact_status.json
--rw-r--r--   0        0        0      127 2023-05-08 22:11:19.558020 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/set_contact_timezone.json
--rw-r--r--   0        0        0      154 2023-05-08 22:11:19.558020 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/set_run_result.json
--rw-r--r--   0        0        0      395 2023-05-08 22:11:19.558020 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/start_session.json
--rw-r--r--   0        0        0      195 2023-05-08 22:11:19.559032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/transfer_airtime.json
--rw-r--r--   0        0        0      294 2023-05-08 22:11:19.559032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/containers/flow_container_minimal.json
--rw-r--r--   0        0        0      987 2023-05-08 22:11:19.559032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/containers/flow_container_node_ui.json
--rw-r--r--   0        0        0    23480 2023-05-08 22:11:19.560019 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/containers/flow_container_ui.json
--rw-r--r--   0        0        0     1383 2023-05-08 22:11:19.561020 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/containers/rapidpro_container_minimal.json
--rw-r--r--   0        0        0      119 2023-05-08 22:11:19.561020 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/exits/exit.json
--rw-r--r--   0        0        0       81 2023-05-08 22:11:19.562032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/groups/group.json
--rw-r--r--   0        0        0      653 2023-05-08 22:11:19.563033 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/nodes/node_basic.json
--rw-r--r--   0        0        0     1596 2023-05-08 22:11:19.564032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/nodes/node_enter_flow.json
--rw-r--r--   0        0        0      766 2023-05-08 22:11:19.564032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/nodes/node_random_router.json
--rw-r--r--   0        0        0     1135 2023-05-08 22:11:19.565015 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/nodes/node_switch_router.json
--rw-r--r--   0        0        0     2581 2023-05-08 22:11:19.566012 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/nodes/ui.json
--rw-r--r--   0        0        0      181 2023-05-08 22:11:19.567011 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/routers/case.json
--rw-r--r--   0        0        0      130 2023-05-08 22:11:19.567011 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/routers/category.json
--rw-r--r--   0        0        0      611 2023-05-08 22:11:19.568010 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/routers/exits.json
--rw-r--r--   0        0        0      518 2023-05-08 22:11:19.568010 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/routers/router_random_simple.json
--rw-r--r--   0        0        0      549 2023-05-08 22:11:19.569023 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/routers/router_random_with_result.json
--rw-r--r--   0        0        0     1393 2023-05-08 22:11:19.569023 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/routers/router_switch_simple.json
--rw-r--r--   0        0        0     1423 2023-05-08 22:11:19.569023 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/routers/router_switch_with_result.json
--rw-r--r--   0        0        0      715 2023-05-08 22:11:19.570019 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/routers/router_switch_with_wait.json
--rw-r--r--   0        0        0      986 2023-05-08 22:11:19.570019 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/routers/router_switch_with_wait_category.json
--rw-r--r--   0        0        0      542 2023-05-08 22:11:19.571032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/test_actions.py
--rw-r--r--   0        0        0     3453 2023-05-08 22:11:19.571032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/test_containers.py
--rw-r--r--   0        0        0     4525 2023-05-08 22:11:19.571032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/test_import_export.py
--rw-r--r--   0        0        0     1304 2023-05-08 22:11:19.572033 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/test_nodes.py
--rw-r--r--   0        0        0     6368 2023-05-08 22:11:19.572033 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/test_routers.py
--rw-r--r--   0        0        0       73 2023-05-08 22:11:19.572033 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/utils.py
--rw-r--r--   0        0        0        0 2023-05-08 22:11:19.573034 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/__init__.py
--rw-r--r--   0        0        0      168 2023-05-09 14:53:32.953533 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    12112 2023-05-08 22:11:19.574032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/all_test_flows.xlsx
--rw-r--r--   0        0        0      282 2023-05-09 00:55:58.543348 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/epicsa_chatbot/epicsa_models.py
--rw-r--r--   0        0        0      229 2023-05-08 22:11:19.574032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/example1/content_index.csv
--rw-r--r--   0        0        0     8443 2023-05-08 22:11:19.575032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/example1/content_index.xlsx
--rw-r--r--   0        0        0       62 2023-05-08 22:11:19.575032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/example1/my_basic_flow.csv
--rw-r--r--   0        0        0      127 2023-05-08 22:11:19.576032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/example1/my_template.csv
--rw-r--r--   0        0        0       97 2023-05-08 22:11:19.576032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/example1/nesteddata.csv
--rw-r--r--   0        0        0      557 2023-05-08 22:11:19.576032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/example1/nestedmodel.py
--rw-r--r--   0        0        0      844 2023-05-08 22:11:19.577032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/groups_and_flows.csv
--rw-r--r--   0        0        0     1134 2023-05-08 22:11:19.577032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/loop_and_multiple_conditions.csv
--rw-r--r--   0        0        0      577 2023-05-08 22:11:19.577032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/loop_from_start.csv
--rw-r--r--   0        0        0      276 2023-05-08 22:11:19.578032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/master_sheet.csv
--rw-r--r--   0        0        0     1833 2023-05-08 22:11:19.578032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/no_switch_nodes.csv
--rw-r--r--   0        0        0     1770 2023-05-08 22:11:19.579032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/no_switch_nodes_without_row_ids.csv
--rw-r--r--   0        0        0     5926 2023-05-09 00:55:58.543348 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/parenttext/parenttext_models.py
--rw-r--r--   0        0        0     2231 2023-05-09 00:55:58.544345 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/parenttext/parenttext_models_delivery.py
--rw-r--r--   0        0        0      907 2023-05-08 22:11:19.579032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/rejoin.csv
--rw-r--r--   0        0        0     5627 2023-05-09 14:53:32.953533 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/srh_chatbot/__pycache__/srh_models.cpython-311.pyc
--rw-r--r--   0        0        0     1818 2023-05-09 00:55:58.544345 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/srh_chatbot/srh_models.py
--rw-r--r--   0        0        0     2402 2023-05-08 22:11:19.579032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/switch_nodes.csv
--rw-r--r--   0        0        0      498 2023-05-08 22:11:19.580032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/templates/yes_no_template.csv
--rw-r--r--   0        0        0      169 2023-05-08 22:11:19.580032 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/templates/yes_no_template_instances.csv
--rw-r--r--   0        0        0    50323 2023-05-08 22:11:19.581036 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/output/all_test_flows.json
--rw-r--r--   0        0        0     2194 2023-05-08 22:11:19.582013 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/test_contentindexparser.py
--rw-r--r--   0        0        0     6373 2023-05-08 22:11:19.582013 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/test_flowparser.py
--rw-r--r--   0        0        0     2997 2023-05-08 22:11:19.583013 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/test_flowparser_reverse.py
--rw-r--r--   0        0        0     2437 2023-05-08 22:11:19.584014 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/test_template_sheet_parser.py
--rw-r--r--   0        0        0    11693 2023-05-08 22:11:19.584014 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/utils.py
--rw-r--r--   0        0        0      647 2023-05-17 13:48:56.704915 rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/token.json
--rw-r--r--   0        0        0        0 2023-05-23 19:56:00.546855 rapidpro_flow_tools-0.2.0/README.md
--rw-r--r--   0        0        0      500 1970-01-01 00:00:00.000000 rapidpro_flow_tools-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      502 2023-05-23 20:31:03.813297 rapidpro_flow_tools-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-23 19:56:00.546855 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 22:11:19.528476 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/__init__.py
+-rw-r--r--   0        0        0      177 2023-05-09 00:10:28.589045 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6513 2023-05-09 00:33:05.120904 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/__pycache__/cellparser.cpython-311.pyc
+-rw-r--r--   0        0        0     4351 2023-05-09 00:40:17.721630 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/__pycache__/rowdatasheet.cpython-311.pyc
+-rw-r--r--   0        0        0    12710 2023-05-09 00:10:28.592570 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/__pycache__/rowparser.cpython-311.pyc
+-rw-r--r--   0        0        0     4042 2023-05-09 00:40:17.718628 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/__pycache__/sheetparser.cpython-311.pyc
+-rw-r--r--   0        0        0     4152 2023-05-08 22:11:19.528476 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/cellparser.py
+-rw-r--r--   0        0        0     3205 2023-05-08 22:11:19.528476 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/rowdatasheet.py
+-rw-r--r--   0        0        0    15945 2023-05-08 22:11:19.529476 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/rowparser.py
+-rw-r--r--   0        0        0     1849 2023-05-08 22:11:19.529476 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/sheetparser.py
+-rw-r--r--   0        0        0        0 2023-05-08 22:11:19.530479 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/tests/__init__.py
+-rw-r--r--   0        0        0      163 2023-05-08 22:11:19.530479 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/tests/mock_cell_parser.py
+-rw-r--r--   0        0        0      292 2023-05-08 22:11:19.530479 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/tests/mock_row_parser.py
+-rw-r--r--   0        0        0      826 2023-05-08 22:11:19.531487 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/tests/mock_sheetparser.py
+-rw-r--r--   0        0        0      600 2023-05-08 22:11:19.532477 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/tests/models.py
+-rw-r--r--   0        0        0     6080 2023-05-08 22:11:19.532477 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/tests/test_cellparser.py
+-rw-r--r--   0        0        0     3508 2023-05-08 22:11:19.533482 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/tests/test_differentways.py
+-rw-r--r--   0        0        0     5026 2023-05-08 22:11:19.534481 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/tests/test_full_rows.py
+-rw-r--r--   0        0        0     3050 2023-05-08 22:11:19.534481 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/tests/test_rowdatasheet.py
+-rw-r--r--   0        0        0     2022 2023-05-08 22:11:19.535494 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/tests/test_sheetparser.py
+-rw-r--r--   0        0        0     4684 2023-05-08 22:11:19.535494 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/tests/test_unparse.py
+-rw-r--r--   0        0        0        0 2023-05-08 22:11:19.535494 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/__init__.py
+-rw-r--r--   0        0        0      179 2023-05-09 00:10:28.582044 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    10375 2023-05-09 00:10:28.585042 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/__pycache__/contentindexparser.cpython-311.pyc
+-rw-r--r--   0        0        0     1948 2023-05-09 00:10:28.588039 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/__pycache__/contentindexrowmodel.cpython-311.pyc
+-rw-r--r--   0        0        0      553 2023-05-09 14:53:32.970178 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/__pycache__/datarowmodel.cpython-311.pyc
+-rw-r--r--   0        0        0    31826 2023-05-09 00:40:18.077840 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/__pycache__/flowparser.cpython-311.pyc
+-rw-r--r--   0        0        0     5701 2023-05-09 00:40:18.053361 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/__pycache__/flowrowmodel.cpython-311.pyc
+-rw-r--r--   0        0        0      152 2023-05-08 22:11:19.536490 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/constants.py
+-rw-r--r--   0        0        0     7020 2023-05-08 22:11:19.536490 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/contentindexparser.py
+-rw-r--r--   0        0        0      932 2023-05-08 22:11:19.536490 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/contentindexrowmodel.py
+-rw-r--r--   0        0        0      102 2023-05-08 22:11:19.537511 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/datarowmodel.py
+-rw-r--r--   0        0        0    26665 2023-05-08 22:11:19.538499 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/flowparser.py
+-rw-r--r--   0        0        0     5242 2023-05-08 22:11:19.538499 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/flowrowmodel.py
+-rw-r--r--   0        0        0     1016 2023-05-08 22:11:19.539488 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/template_sheet_parser.py
+-rw-r--r--   0        0        0        0 2023-05-08 22:11:19.539488 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/tests/__init__.py
+-rw-r--r--   0        0        0      179 2023-05-08 22:11:19.539488 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/tests/datarowmodels/evalmodels.py
+-rw-r--r--   0        0        0      444 2023-05-08 22:11:19.540493 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/tests/datarowmodels/listmodel.py
+-rw-r--r--   0        0        0      557 2023-05-08 22:11:19.540493 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/tests/datarowmodels/nestedmodel.py
+-rw-r--r--   0        0        0      133 2023-05-08 22:11:19.541498 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/tests/datarowmodels/simplemodel.py
+-rw-r--r--   0        0        0      478 2023-05-08 22:11:19.541498 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/tests/mock_sheetreader.py
+-rw-r--r--   0        0        0     1030 2023-05-08 22:11:19.541498 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/tests/row_data.py
+-rw-r--r--   0        0        0    17043 2023-05-08 22:11:19.542498 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/tests/test_contentindexparser.py
+-rw-r--r--   0        0        0    39668 2023-05-08 22:11:19.543511 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/tests/test_flowparser.py
+-rw-r--r--   0        0        0    14789 2023-05-08 22:11:19.543511 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/tests/test_to_row_model.py
+-rw-r--r--   0        0        0      259 2023-05-08 22:11:19.543511 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/tests/utils.py
+-rw-r--r--   0        0        0      432 2023-05-09 14:52:38.982087 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/credentials.json
+-rw-r--r--   0        0        0     1181 2023-05-23 20:24:29.455479 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/flow_converter.py
+-rw-r--r--   0        0        0    20155 2023-05-09 00:40:18.060364 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/models/__pycache__/actions.cpython-311.pyc
+-rw-r--r--   0        0        0     1367 2023-05-09 00:40:18.062829 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/models/__pycache__/common.cpython-311.pyc
+-rw-r--r--   0        0        0    15080 2023-05-09 00:40:18.045351 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/models/__pycache__/containers.cpython-311.pyc
+-rw-r--r--   0        0        0    30325 2023-05-09 00:40:18.051365 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/models/__pycache__/nodes.cpython-311.pyc
+-rw-r--r--   0        0        0    30571 2023-05-09 00:40:18.067821 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/models/__pycache__/routers.cpython-311.pyc
+-rw-r--r--   0        0        0    11728 2023-05-08 22:11:19.546511 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/models/actions.py
+-rw-r--r--   0        0        0     1004 2023-05-08 22:11:19.547498 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/models/common.py
+-rw-r--r--   0        0        0    10931 2023-05-08 22:11:19.547498 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/models/containers.py
+-rw-r--r--   0        0        0    20809 2023-05-08 22:11:19.547498 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/models/nodes.py
+-rw-r--r--   0        0        0    18753 2023-05-08 22:11:19.548498 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/models/routers.py
+-rw-r--r--   0        0        0        0 2023-05-08 22:11:19.545511 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-09 00:40:18.041350 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      408 2023-05-09 00:40:18.047361 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2023-05-08 22:11:19.549493 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/__init__.py
+-rw-r--r--   0        0        0      154 2023-05-08 22:11:19.550002 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/add_contact_urn.json
+-rw-r--r--   0        0        0      225 2023-05-08 22:11:19.551016 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/add_input_labels.json
+-rw-r--r--   0        0        0      260 2023-05-08 22:11:19.551016 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/call_classifier.json
+-rw-r--r--   0        0        0      123 2023-05-08 22:11:19.552016 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/call_resthook.json
+-rw-r--r--   0        0        0      258 2023-05-08 22:11:19.552016 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/call_webhook.json
+-rw-r--r--   0        0        0      199 2023-05-08 22:11:19.552016 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/enter_flow.json
+-rw-r--r--   0        0        0      466 2023-05-08 22:11:19.552016 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/open_ticket.json
+-rw-r--r--   0        0        0      140 2023-05-08 22:11:19.553020 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/play_audio.json
+-rw-r--r--   0        0        0      242 2023-05-08 22:11:19.553020 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/remove_contact_groups.json
+-rw-r--r--   0        0        0      213 2023-05-08 22:11:19.553020 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/say_msg.json
+-rw-r--r--   0        0        0      214 2023-05-08 22:11:19.554019 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/send_broadcast.json
+-rw-r--r--   0        0        0      258 2023-05-08 22:11:19.554019 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/send_email.json
+-rw-r--r--   0        0        0      512 2023-05-08 22:11:19.554019 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/send_msg.json
+-rw-r--r--   0        0        0      573 2023-05-08 22:11:19.555032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/send_msg_with_attachments.json
+-rw-r--r--   0        0        0      549 2023-05-08 22:11:19.555032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/send_msg_with_quick_replies.json
+-rw-r--r--   0        0        0      211 2023-05-08 22:11:19.555032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/set_contact_channel.json
+-rw-r--r--   0        0        0      190 2023-05-08 22:11:19.556033 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/set_contact_field.json
+-rw-r--r--   0        0        0      117 2023-05-08 22:11:19.556033 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/set_contact_language.json
+-rw-r--r--   0        0        0      115 2023-05-08 22:11:19.557020 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/set_contact_name.json
+-rw-r--r--   0        0        0      117 2023-05-08 22:11:19.557020 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/set_contact_status.json
+-rw-r--r--   0        0        0      127 2023-05-08 22:11:19.558020 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/set_contact_timezone.json
+-rw-r--r--   0        0        0      154 2023-05-08 22:11:19.558020 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/set_run_result.json
+-rw-r--r--   0        0        0      395 2023-05-08 22:11:19.558020 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/start_session.json
+-rw-r--r--   0        0        0      195 2023-05-08 22:11:19.559032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/transfer_airtime.json
+-rw-r--r--   0        0        0      294 2023-05-08 22:11:19.559032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/containers/flow_container_minimal.json
+-rw-r--r--   0        0        0      987 2023-05-08 22:11:19.559032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/containers/flow_container_node_ui.json
+-rw-r--r--   0        0        0    23480 2023-05-08 22:11:19.560019 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/containers/flow_container_ui.json
+-rw-r--r--   0        0        0     1383 2023-05-08 22:11:19.561020 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/containers/rapidpro_container_minimal.json
+-rw-r--r--   0        0        0      119 2023-05-08 22:11:19.561020 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/exits/exit.json
+-rw-r--r--   0        0        0       81 2023-05-08 22:11:19.562032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/groups/group.json
+-rw-r--r--   0        0        0      653 2023-05-08 22:11:19.563033 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/nodes/node_basic.json
+-rw-r--r--   0        0        0     1596 2023-05-08 22:11:19.564032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/nodes/node_enter_flow.json
+-rw-r--r--   0        0        0      766 2023-05-08 22:11:19.564032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/nodes/node_random_router.json
+-rw-r--r--   0        0        0     1135 2023-05-08 22:11:19.565015 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/nodes/node_switch_router.json
+-rw-r--r--   0        0        0     2581 2023-05-08 22:11:19.566012 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/nodes/ui.json
+-rw-r--r--   0        0        0      181 2023-05-08 22:11:19.567011 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/routers/case.json
+-rw-r--r--   0        0        0      130 2023-05-08 22:11:19.567011 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/routers/category.json
+-rw-r--r--   0        0        0      611 2023-05-08 22:11:19.568010 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/routers/exits.json
+-rw-r--r--   0        0        0      518 2023-05-08 22:11:19.568010 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/routers/router_random_simple.json
+-rw-r--r--   0        0        0      549 2023-05-08 22:11:19.569023 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/routers/router_random_with_result.json
+-rw-r--r--   0        0        0     1393 2023-05-08 22:11:19.569023 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/routers/router_switch_simple.json
+-rw-r--r--   0        0        0     1423 2023-05-08 22:11:19.569023 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/routers/router_switch_with_result.json
+-rw-r--r--   0        0        0      715 2023-05-08 22:11:19.570019 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/routers/router_switch_with_wait.json
+-rw-r--r--   0        0        0      986 2023-05-08 22:11:19.570019 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/routers/router_switch_with_wait_category.json
+-rw-r--r--   0        0        0      542 2023-05-08 22:11:19.571032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/test_actions.py
+-rw-r--r--   0        0        0     3453 2023-05-08 22:11:19.571032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/test_containers.py
+-rw-r--r--   0        0        0     4525 2023-05-08 22:11:19.571032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/test_import_export.py
+-rw-r--r--   0        0        0     1304 2023-05-08 22:11:19.572033 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/test_nodes.py
+-rw-r--r--   0        0        0     6368 2023-05-08 22:11:19.572033 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/test_routers.py
+-rw-r--r--   0        0        0       73 2023-05-08 22:11:19.572033 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/utils.py
+-rw-r--r--   0        0        0        0 2023-05-08 22:11:19.544512 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/sheets/__init__.py
+-rw-r--r--   0        0        0      177 2023-05-09 00:40:18.079823 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/sheets/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1856 2023-05-09 00:40:18.081823 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/sheets/__pycache__/csv_sheet_reader.cpython-311.pyc
+-rw-r--r--   0        0        0     5435 2023-05-17 13:48:55.572103 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/sheets/__pycache__/google_sheet_reader.cpython-311.pyc
+-rw-r--r--   0        0        0     1799 2023-05-09 00:40:18.082822 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/sheets/__pycache__/xlsx_sheet_reader.cpython-311.pyc
+-rw-r--r--   0        0        0      626 2023-05-08 22:11:19.544512 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/sheets/csv_sheet_reader.py
+-rw-r--r--   0        0        0     3199 2023-05-17 13:33:29.457039 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/sheets/google_sheet_reader.py
+-rw-r--r--   0        0        0      711 2023-05-08 22:11:19.545511 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/sheets/xlsx_sheet_reader.py
+-rw-r--r--   0        0        0        0 2023-05-08 22:11:19.573034 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/__init__.py
+-rw-r--r--   0        0        0      168 2023-05-09 14:53:32.953533 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    12112 2023-05-08 22:11:19.574032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/all_test_flows.xlsx
+-rw-r--r--   0        0        0      282 2023-05-09 00:55:58.543348 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/epicsa_chatbot/epicsa_models.py
+-rw-r--r--   0        0        0      229 2023-05-08 22:11:19.574032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/example1/content_index.csv
+-rw-r--r--   0        0        0     8443 2023-05-08 22:11:19.575032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/example1/content_index.xlsx
+-rw-r--r--   0        0        0       62 2023-05-08 22:11:19.575032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/example1/my_basic_flow.csv
+-rw-r--r--   0        0        0      127 2023-05-08 22:11:19.576032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/example1/my_template.csv
+-rw-r--r--   0        0        0       97 2023-05-08 22:11:19.576032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/example1/nesteddata.csv
+-rw-r--r--   0        0        0      557 2023-05-08 22:11:19.576032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/example1/nestedmodel.py
+-rw-r--r--   0        0        0      844 2023-05-08 22:11:19.577032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/groups_and_flows.csv
+-rw-r--r--   0        0        0     1134 2023-05-08 22:11:19.577032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/loop_and_multiple_conditions.csv
+-rw-r--r--   0        0        0      577 2023-05-08 22:11:19.577032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/loop_from_start.csv
+-rw-r--r--   0        0        0      276 2023-05-08 22:11:19.578032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/master_sheet.csv
+-rw-r--r--   0        0        0     1833 2023-05-08 22:11:19.578032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/no_switch_nodes.csv
+-rw-r--r--   0        0        0     1770 2023-05-08 22:11:19.579032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/no_switch_nodes_without_row_ids.csv
+-rw-r--r--   0        0        0     5926 2023-05-09 00:55:58.543348 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/parenttext/parenttext_models.py
+-rw-r--r--   0        0        0     2231 2023-05-09 00:55:58.544345 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/parenttext/parenttext_models_delivery.py
+-rw-r--r--   0        0        0      907 2023-05-08 22:11:19.579032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/rejoin.csv
+-rw-r--r--   0        0        0     5627 2023-05-09 14:53:32.953533 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/srh_chatbot/__pycache__/srh_models.cpython-311.pyc
+-rw-r--r--   0        0        0     1818 2023-05-09 00:55:58.544345 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/srh_chatbot/srh_models.py
+-rw-r--r--   0        0        0     2402 2023-05-08 22:11:19.579032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/switch_nodes.csv
+-rw-r--r--   0        0        0      498 2023-05-08 22:11:19.580032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/templates/yes_no_template.csv
+-rw-r--r--   0        0        0      169 2023-05-08 22:11:19.580032 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/templates/yes_no_template_instances.csv
+-rw-r--r--   0        0        0    50323 2023-05-08 22:11:19.581036 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/output/all_test_flows.json
+-rw-r--r--   0        0        0     2194 2023-05-08 22:11:19.582013 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/test_contentindexparser.py
+-rw-r--r--   0        0        0     6373 2023-05-08 22:11:19.582013 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/test_flowparser.py
+-rw-r--r--   0        0        0     2997 2023-05-08 22:11:19.583013 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/test_flowparser_reverse.py
+-rw-r--r--   0        0        0     2437 2023-05-08 22:11:19.584014 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/test_template_sheet_parser.py
+-rw-r--r--   0        0        0    11693 2023-05-08 22:11:19.584014 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/utils.py
+-rw-r--r--   0        0        0      647 2023-05-17 13:48:56.704915 rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/token.json
+-rw-r--r--   0        0        0        0 2023-05-23 19:56:00.546855 rapidpro_flow_tools-0.3.0/README.md
+-rw-r--r--   0        0        0      500 1970-01-01 00:00:00.000000 rapidpro_flow_tools-0.3.0/PKG-INFO
```

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/flow_converter.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/flow_converter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
-from parsers.creation.contentindexparser import ContentIndexParser
-from parsers.sheets.csv_sheet_reader import CSVSheetReader
-from parsers.sheets.xlsx_sheet_reader import XLSXSheetReader
-from parsers.sheets.google_sheet_reader import GoogleSheetReader
-from rapidpro.models.containers import RapidProContainer
+from creation.contentindexparser import ContentIndexParser
+from sheets.csv_sheet_reader import CSVSheetReader
+from sheets.xlsx_sheet_reader import XLSXSheetReader
+from sheets.google_sheet_reader import GoogleSheetReader
+from models.containers import RapidProContainer
 
 def convert_flow(command, input_file, output_file, sheet_format, data_models=None, credentials=None, token=None):
     if command != 'create_flows':
         print(f"Command {command} currently unsupported.")
         return
 
     if sheet_format == 'csv':
```

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/__pycache__/cellparser.cpython-311.pyc` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/__pycache__/cellparser.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/__pycache__/rowdatasheet.cpython-311.pyc` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/__pycache__/rowdatasheet.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/__pycache__/rowparser.cpython-311.pyc` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/__pycache__/rowparser.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/__pycache__/sheetparser.cpython-311.pyc` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/__pycache__/sheetparser.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/cellparser.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/cellparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/rowdatasheet.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/rowdatasheet.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/rowparser.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/rowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/sheetparser.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/sheetparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/tests/mock_sheetparser.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/tests/mock_sheetparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/tests/models.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/tests/models.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/tests/test_cellparser.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/tests/test_cellparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/tests/test_differentways.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/tests/test_differentways.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/tests/test_full_rows.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/tests/test_full_rows.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/tests/test_rowdatasheet.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/tests/test_rowdatasheet.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/tests/test_sheetparser.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/tests/test_sheetparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/common/tests/test_unparse.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/common/tests/test_unparse.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/__pycache__/contentindexparser.cpython-311.pyc` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/__pycache__/contentindexparser.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/__pycache__/contentindexrowmodel.cpython-311.pyc` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/__pycache__/contentindexrowmodel.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/__pycache__/datarowmodel.cpython-311.pyc` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/__pycache__/datarowmodel.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/__pycache__/flowparser.cpython-311.pyc` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/__pycache__/flowparser.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/__pycache__/flowrowmodel.cpython-311.pyc` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/__pycache__/flowrowmodel.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/contentindexparser.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/contentindexrowmodel.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/contentindexrowmodel.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/flowparser.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/flowrowmodel.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/flowrowmodel.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/template_sheet_parser.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/template_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/tests/datarowmodels/nestedmodel.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/tests/datarowmodels/nestedmodel.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/tests/row_data.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/tests/row_data.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/tests/test_contentindexparser.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/tests/test_contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/tests/test_flowparser.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/tests/test_flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/creation/tests/test_to_row_model.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/creation/tests/test_to_row_model.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/sheets/__pycache__/csv_sheet_reader.cpython-311.pyc` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/sheets/__pycache__/csv_sheet_reader.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/sheets/__pycache__/google_sheet_reader.cpython-311.pyc` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/sheets/__pycache__/google_sheet_reader.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/sheets/__pycache__/xlsx_sheet_reader.cpython-311.pyc` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/sheets/__pycache__/xlsx_sheet_reader.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/sheets/csv_sheet_reader.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/sheets/csv_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/sheets/google_sheet_reader.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/sheets/google_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/parsers/sheets/xlsx_sheet_reader.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/sheets/xlsx_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/models/__pycache__/actions.cpython-311.pyc` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/models/__pycache__/actions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/models/__pycache__/common.cpython-311.pyc` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/models/__pycache__/common.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/models/__pycache__/containers.cpython-311.pyc` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/models/__pycache__/containers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/models/__pycache__/nodes.cpython-311.pyc` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/models/__pycache__/nodes.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/models/__pycache__/routers.cpython-311.pyc` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/models/__pycache__/routers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/models/actions.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/models/actions.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/models/common.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/models/common.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/models/containers.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/models/containers.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/models/nodes.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/models/nodes.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/models/routers.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/models/routers.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/send_msg.json` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/send_msg.json`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/send_msg_with_attachments.json` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/send_msg_with_attachments.json`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/actions/send_msg_with_quick_replies.json` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/actions/send_msg_with_quick_replies.json`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/containers/flow_container_node_ui.json` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/containers/flow_container_node_ui.json`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/containers/flow_container_ui.json` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/containers/flow_container_ui.json`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/containers/rapidpro_container_minimal.json` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/containers/rapidpro_container_minimal.json`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/nodes/node_basic.json` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/nodes/node_basic.json`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/nodes/node_enter_flow.json` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/nodes/node_enter_flow.json`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/nodes/node_random_router.json` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/nodes/node_random_router.json`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/nodes/node_switch_router.json` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/nodes/node_switch_router.json`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/nodes/ui.json` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/nodes/ui.json`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/routers/exits.json` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/routers/exits.json`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/routers/router_random_simple.json` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/routers/router_random_simple.json`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/routers/router_random_with_result.json` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/routers/router_random_with_result.json`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/routers/router_switch_simple.json` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/routers/router_switch_simple.json`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/routers/router_switch_with_result.json` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/routers/router_switch_with_result.json`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/routers/router_switch_with_wait.json` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/routers/router_switch_with_wait.json`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/data/routers/router_switch_with_wait_category.json` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/data/routers/router_switch_with_wait_category.json`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/test_actions.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/test_containers.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/test_import_export.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/test_import_export.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/test_nodes.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/rapidpro/tests/test_routers.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/rapidpro/tests/test_routers.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/all_test_flows.xlsx` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/all_test_flows.xlsx`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/example1/content_index.xlsx` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/example1/content_index.xlsx`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/example1/nestedmodel.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/example1/nestedmodel.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/groups_and_flows.csv` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/groups_and_flows.csv`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/loop_and_multiple_conditions.csv` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/loop_and_multiple_conditions.csv`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/loop_from_start.csv` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/loop_from_start.csv`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/no_switch_nodes.csv` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/no_switch_nodes.csv`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/no_switch_nodes_without_row_ids.csv` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/no_switch_nodes_without_row_ids.csv`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/parenttext/parenttext_models.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/parenttext/parenttext_models.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/parenttext/parenttext_models_delivery.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/parenttext/parenttext_models_delivery.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/rejoin.csv` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/rejoin.csv`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/srh_chatbot/__pycache__/srh_models.cpython-311.pyc` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/srh_chatbot/__pycache__/srh_models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/srh_chatbot/srh_models.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/srh_chatbot/srh_models.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/input/switch_nodes.csv` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/input/switch_nodes.csv`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/output/all_test_flows.json` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/output/all_test_flows.json`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/test_contentindexparser.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/test_contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/test_flowparser.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/test_flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/test_flowparser_reverse.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/test_flowparser_reverse.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/test_template_sheet_parser.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/test_template_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/tests/utils.py` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/tests/utils.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-0.2.0/rapidpro_flow_tools/token.json` & `rapidpro_flow_tools-0.3.0/rapidpro_flow_tools/token.json`

 * *Files identical despite different names*

